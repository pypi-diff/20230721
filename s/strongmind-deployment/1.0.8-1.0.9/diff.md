# Comparing `tmp/strongmind_deployment-1.0.8-py3-none-any.whl.zip` & `tmp/strongmind_deployment-1.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 7606 bytes, number of entries: 8
+Zip file size: 8492 bytes, number of entries: 8
 -rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 strongmind_deployment/__init__.py
 -rw-r--r--  2.0 unx    11433 b- defN 20-Feb-02 00:00 strongmind_deployment/container.py
--rw-r--r--  2.0 unx     7116 b- defN 20-Feb-02 00:00 strongmind_deployment/rails.py
--rw-r--r--  2.0 unx     1126 b- defN 20-Feb-02 00:00 strongmind_deployment/redis.py
-?rw-r--r--  2.0 unx      675 b- defN 20-Feb-02 00:00 strongmind_deployment-1.0.8.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 strongmind_deployment-1.0.8.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1053 b- defN 20-Feb-02 00:00 strongmind_deployment-1.0.8.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx      711 b- defN 20-Feb-02 00:00 strongmind_deployment-1.0.8.dist-info/RECORD
-8 files, 22201 bytes uncompressed, 6348 bytes compressed:  71.4%
+-rw-r--r--  2.0 unx     9638 b- defN 20-Feb-02 00:00 strongmind_deployment/rails.py
+-rw-r--r--  2.0 unx     2918 b- defN 20-Feb-02 00:00 strongmind_deployment/redis.py
+?rw-r--r--  2.0 unx      675 b- defN 20-Feb-02 00:00 strongmind_deployment-1.0.9.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 strongmind_deployment-1.0.9.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1053 b- defN 20-Feb-02 00:00 strongmind_deployment-1.0.9.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx      711 b- defN 20-Feb-02 00:00 strongmind_deployment-1.0.9.dist-info/RECORD
+8 files, 26515 bytes uncompressed, 7234 bytes compressed:  72.7%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: strongmind_deployment/rails.py
 Comment: 
 
 Filename: strongmind_deployment/redis.py
 Comment: 
 
-Filename: strongmind_deployment-1.0.8.dist-info/METADATA
+Filename: strongmind_deployment-1.0.9.dist-info/METADATA
 Comment: 
 
-Filename: strongmind_deployment-1.0.8.dist-info/WHEEL
+Filename: strongmind_deployment-1.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: strongmind_deployment-1.0.8.dist-info/licenses/LICENSE
+Filename: strongmind_deployment-1.0.9.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: strongmind_deployment-1.0.8.dist-info/RECORD
+Filename: strongmind_deployment-1.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## strongmind_deployment/rails.py

```diff
@@ -3,18 +3,43 @@
 
 import pulumi
 import pulumi_random as random
 import pulumi_aws as aws
 from pulumi import export, Output
 
 from strongmind_deployment.container import ContainerComponent
-from strongmind_deployment.redis import RedisComponent
+from strongmind_deployment.redis import RedisComponent, QueueComponent, CacheComponent
+
+
+def sidekiq_present():  # pragma: no cover
+    return os.path.exists('../Gemfile') and 'sidekiq' in open('../Gemfile').read()
 
 
 class RailsComponent(pulumi.ComponentResource):
+    """
+    RailsComponent is a resource that produces a Rails application running on AWS Fargate.
+
+    :param name: The _unique_ name of the resource.
+    :param opts: A bag of optional settings that control this resource's behavior.
+    :param env_vars: A dictionary of environment variables to pass to the Rails application.
+    :param queue_redis: Either True to create a default queue Redis instance or a RedisComponent to use. Defaults to True if sidekiq is in the Gemfile.
+    :param cache_redis: Either True to create a default cache Redis instance or a RedisComponent to use.
+    :param web_entry_point: The entry point for the web container. Defaults to `["sh", "-c",
+                                                              "rails db:prepare db:migrate db:seed && "
+                                                              "rails assets:precompile && "
+                                                              "rails server --port 3000 -b 0.0.0.0"]`
+    :param need_worker: Whether or not to create a worker container. Defaults to True if sidekiq is in the Gemfile.
+    :param worker_entry_point: The entry point for the worker container. Defaults to `["sh", "-c", "bundle exec sidekiq"]`
+    :param cpu: The number of CPU units to reserve for the web container. Defaults to 256.
+    :param memory: The amount of memory (in MiB) to allow the web container to use. Defaults to 512.
+    :param app_path: The path to the Rails application for the web. Defaults to `./`.
+    :param worker_cpu: The number of CPU units to reserve for the worker container. Defaults to 256.
+    :param worker_memory: The amount of memory (in MiB) to allow the worker container to use. Defaults to 512.
+    :param worker_app_path: The path to the Rails application for the worker. Defaults to `./`.
+    """
     def __init__(self, name, opts=None, **kwargs):
         super().__init__('strongmind:global_build:commons:rails', name, None, opts)
         self.need_worker = None
         self.cname_record = None
         self.firewall_rule = None
         self.db_password = None
         self.web_container = None
@@ -35,24 +60,44 @@
             "repository": project,
             "service": project,
             "environment": self.env_name,
         }
 
         self.rds(project_stack)
 
-        self.redis = RedisComponent("redis",
-                                    env_vars=self.env_vars)
-        export("redis_endpoint", Output.concat(self.redis.cluster.cache_nodes[0]['address']))
+        self.setup_redis()
 
         self.ecs()
 
         self.security()
 
         self.register_outputs({})
 
+    def setup_redis(self):
+        if sidekiq_present():
+            self.env_vars['REDIS_PROVIDER'] = 'QUEUE_REDIS_URL'
+            if 'queue_redis' not in self.kwargs:
+                self.kwargs['queue_redis'] = True
+        if 'queue_redis' in self.kwargs:
+            if isinstance(self.kwargs['queue_redis'], RedisComponent):
+                self.queue_redis = self.kwargs['queue_redis']
+            elif self.kwargs['queue_redis']:
+                self.queue_redis = QueueComponent("queue-redis")
+
+            if self.queue_redis:
+                self.env_vars['QUEUE_REDIS_URL'] = self.queue_redis.url
+        if 'cache_redis' in self.kwargs:
+            if isinstance(self.kwargs['cache_redis'], RedisComponent):
+                self.cache_redis = self.kwargs['cache_redis']
+            elif self.kwargs['cache_redis']:
+                self.cache_redis = CacheComponent("cache-redis")
+
+            if self.cache_redis:
+                self.env_vars['CACHE_REDIS_URL'] = self.cache_redis.url
+
     def security(self):
         container_security_group_id = self.kwargs.get(
             'container_security_group_id',
             self.web_container.fargate_service.service.network_configuration.security_groups[0])  # pragma: no cover
 
         self.firewall_rule = aws.ec2.SecurityGroupRule(
             'rds_security_group_rule',
@@ -72,15 +117,14 @@
         master_key = os.environ['RAILS_MASTER_KEY']
         additional_env_vars = {
             'RAILS_MASTER_KEY': master_key,
             'DATABASE_HOST': self.rds_serverless_cluster.endpoint,
             'DB_USERNAME': self.rds_serverless_cluster.master_username,
             'DB_PASSWORD': self.rds_serverless_cluster.master_password,
             'DATABASE_URL': self.get_database_url(),
-            'REDIS_URL': self.get_redis_endpoint(),
             'RAILS_ENV': 'production'
         }
 
         self.env_vars.update(additional_env_vars)
         self.kwargs['env_vars'] = self.env_vars
         self.kwargs['container_image'] = container_image
 
@@ -93,17 +137,17 @@
 
         self.web_container = ContainerComponent("container",
                                                 pulumi.ResourceOptions(parent=self),
                                                 **self.kwargs
                                                 )
 
         self.need_worker = self.kwargs.get('need_worker', None)
-        if self.need_worker is None:
+        if self.need_worker is None:  # pragma: no cover
             # If we don't know if we need a worker, check for sidekiq in the Gemfile
-            self.need_worker = os.path.exists('../Gemfile') and 'sidekiq' in open('../Gemfile').read()
+            self.need_worker = sidekiq_present()
 
         if self.need_worker:
             self.setup_worker()
 
     def setup_worker(self):
         worker_entry_point = self.kwargs.get('worker_entry_point', ["sh", "-c", "bundle exec sidekiq"])
         self.kwargs['entry_point'] = worker_entry_point
@@ -156,13 +200,8 @@
     def get_database_url(self):
         return Output.concat('postgres://',
                              self.rds_serverless_cluster.master_username,
                              ':',
                              self.rds_serverless_cluster.master_password,
                              '@',
                              self.rds_serverless_cluster.endpoint,
-                             ':5432/app')
-
-    def get_redis_endpoint(self):
-        return Output.concat('redis://',
-                             self.redis.cluster.cache_nodes[0]['address'],
-                             ':6379')
+                             ':5432/app')
```

## strongmind_deployment/redis.py

```diff
@@ -1,39 +1,83 @@
 import os
 
 import pulumi
 import pulumi_aws as aws
+from pulumi import Output
 
 
 class RedisComponent(pulumi.ComponentResource):
     def __init__(self, name, opts=None, **kwargs):
         super().__init__('strongmind:global_build:commons:redis', name, None, opts)
         self.kwargs = kwargs
         self.env_vars = self.kwargs.get('env_vars', {})
+        self.node_type = self.kwargs.get('node_type', 'cache.t4g.small')
+        self.num_cache_nodes = self.kwargs.get('num_cache_nodes', 1)
 
         self.env_name = os.environ.get('ENVIRONMENT_NAME', 'stage')
+        self.parameter_group_name = self.kwargs.get('parameter_group_name', 'default.redis7')
 
         project = pulumi.get_project()
         stack = pulumi.get_stack()
         project_stack = f"{project}-{stack}"
 
         self.tags = {
             "product": project,
             "repository": project,
             "service": project,
             "environment": self.env_name,
         }
+        dependencies = []
+        if hasattr(self, 'parameter_group'):
+            dependencies.append(self.parameter_group)
 
         self.cluster = aws.elasticache.Cluster(
-            "redis",
-            cluster_id=project_stack,
+            name,
+            cluster_id=f'{project_stack}-{name}',
             engine="redis",
-            node_type="cache.t4g.small",
+            node_type=self.node_type,
             engine_version="7.0",
-            num_cache_nodes=1,
-            parameter_group_name="default.redis7",
+            num_cache_nodes=self.num_cache_nodes,
+            parameter_group_name=self.parameter_group_name,
             port=6379,
             tags=self.tags,
-            opts=pulumi.ResourceOptions(parent=self),
+            opts=pulumi.ResourceOptions(parent=self, depends_on=dependencies),
         )
 
         self.register_outputs({})
+
+    @property
+    def url(self):
+        return Output.concat("redis://", self.cluster.cache_nodes[0].address, ":6379")
+
+
+class QueueComponent(RedisComponent):
+    def __init__(self, name, opts=None, **kwargs):
+        project = pulumi.get_project()
+        stack = pulumi.get_stack()
+        project_stack = f"{project}-{stack}"
+        kwargs['parameter_group_name'] = f"{project_stack}-queue-redis7"
+        self.parameter_group = aws.elasticache.ParameterGroup(
+            f"{name}-parameter-group",
+            name=kwargs['parameter_group_name'],
+            family="redis7",
+            parameters=[
+                aws.elasticache.ParameterGroupParameterArgs(
+                    name="maxmemory-policy",
+                    value="noeviction")
+            ]
+        )
+        super().__init__(name, opts, **kwargs)
+
+
+class CacheComponent(RedisComponent):
+    def __init__(self, name, opts=None, **kwargs):
+        project = pulumi.get_project()
+        stack = pulumi.get_stack()
+        project_stack = f"{project}-{stack}"
+        kwargs['parameter_group_name'] = f"{project_stack}-cache-redis7"
+        self.parameter_group = aws.elasticache.ParameterGroup(
+            f"{name}-parameter-group",
+            name=kwargs['parameter_group_name'],
+            family="redis7",
+        )
+        super().__init__(name, opts, **kwargs)
```

## Comparing `strongmind_deployment-1.0.8.dist-info/METADATA` & `strongmind_deployment-1.0.9.dist-info/METADATA`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strongmind_deployment
-Version: 1.0.8
+Version: 1.0.9
 Summary: Deployment tools for Strongmind
 Project-URL: Homepage, https://github.com/strongmind/public-reusable-workflows/tree/main/deployment
 Author-email: Belding <teambelding@strongmind.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

## Comparing `strongmind_deployment-1.0.8.dist-info/licenses/LICENSE` & `strongmind_deployment-1.0.9.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

## Comparing `strongmind_deployment-1.0.8.dist-info/RECORD` & `strongmind_deployment-1.0.9.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 strongmind_deployment/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 strongmind_deployment/container.py,sha256=GDoPcGQgNigXlojXjJIQ1ogOLui0_YcxBx12AkPe4vA,11433
-strongmind_deployment/rails.py,sha256=FSUHNG2j7_0EFnSgJUN9_ZBsFaiEq7dQ_zBUIzpyvg8,7116
-strongmind_deployment/redis.py,sha256=pYiSCRBQtO9TU69KVt0GrmJyB_GhGEz_hQUucw9vBUA,1126
-strongmind_deployment-1.0.8.dist-info/METADATA,sha256=Xo6y2tli0Sk3bAB7KTiT22UMEyRj5YAxe99uzcV3b8o,675
-strongmind_deployment-1.0.8.dist-info/WHEEL,sha256=9QBuHhg6FNW7lppboF2vKVbCGTVzsFykgRQjjlajrhA,87
-strongmind_deployment-1.0.8.dist-info/licenses/LICENSE,sha256=2zBZXFllrbHYl8Zg63B1X0QWHK1ed93SzZQVh9gd77c,1053
-strongmind_deployment-1.0.8.dist-info/RECORD,,
+strongmind_deployment/rails.py,sha256=-z4EImyEJscsQD_AJq5ofuvzUaItqO77fCj-xcPFthk,9638
+strongmind_deployment/redis.py,sha256=Cl7avjc0PNiqJ3E4IgG9_2js8tcG3FeSNpGbpGmCAeE,2918
+strongmind_deployment-1.0.9.dist-info/METADATA,sha256=EUMaeGEH6UjiTCgmg172MbAVMT_5_0Tit4ohgS6cFQg,675
+strongmind_deployment-1.0.9.dist-info/WHEEL,sha256=9QBuHhg6FNW7lppboF2vKVbCGTVzsFykgRQjjlajrhA,87
+strongmind_deployment-1.0.9.dist-info/licenses/LICENSE,sha256=2zBZXFllrbHYl8Zg63B1X0QWHK1ed93SzZQVh9gd77c,1053
+strongmind_deployment-1.0.9.dist-info/RECORD,,
```

