# Comparing `tmp/aioradio-0.9.7.tar.gz` & `tmp/aioradio-0.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aioradio-0.9.7.tar", last modified: Wed Jan  6 19:42:39 2021, max compression
+gzip compressed data, was "dist/aioradio-0.9.8.tar", last modified: Mon Feb  1 15:47:19 2021, max compression
```

## Comparing `aioradio-0.9.7.tar` & `aioradio-0.9.8.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 tim.reichard   (502) staff       (20)        0 2021-01-06 19:42:39.000000 aioradio-0.9.7/
--rw-r--r--   0 tim.reichard   (502) staff       (20)       24 2020-10-13 15:39:38.000000 aioradio-0.9.7/MANIFEST.in
--rw-r--r--   0 tim.reichard   (502) staff       (20)     9020 2021-01-06 19:42:39.000000 aioradio-0.9.7/PKG-INFO
--rw-r--r--   0 tim.reichard   (502) staff       (20)     6968 2020-11-10 19:42:27.000000 aioradio-0.9.7/README.md
-drwxr-xr-x   0 tim.reichard   (502) staff       (20)        0 2021-01-06 19:42:39.000000 aioradio-0.9.7/aioradio/
--rw-r--r--   0 tim.reichard   (502) staff       (20)        0 2020-10-13 15:39:38.000000 aioradio-0.9.7/aioradio/__init__.py
-drwxr-xr-x   0 tim.reichard   (502) staff       (20)        0 2021-01-06 19:42:39.000000 aioradio-0.9.7/aioradio/aws/
--rw-r--r--   0 tim.reichard   (502) staff       (20)     7234 2020-12-22 20:16:27.000000 aioradio-0.9.7/aioradio/aws/dynamodb.py
--rw-r--r--   0 tim.reichard   (502) staff       (20)     4331 2020-12-22 20:16:27.000000 aioradio-0.9.7/aioradio/aws/moto_server.py
--rw-r--r--   0 tim.reichard   (502) staff       (20)     3472 2020-12-22 20:16:27.000000 aioradio-0.9.7/aioradio/aws/s3.py
--rw-r--r--   0 tim.reichard   (502) staff       (20)      783 2020-12-22 20:16:27.000000 aioradio-0.9.7/aioradio/aws/secrets.py
--rw-r--r--   0 tim.reichard   (502) staff       (20)     4308 2020-12-22 20:16:27.000000 aioradio-0.9.7/aioradio/aws/sqs.py
--rw-r--r--   0 tim.reichard   (502) staff       (20)     6955 2020-12-22 20:16:27.000000 aioradio-0.9.7/aioradio/aws/utils.py
--rw-r--r--   0 tim.reichard   (502) staff       (20)    11215 2021-01-06 19:37:36.000000 aioradio-0.9.7/aioradio/file_ingestion.py
--rw-r--r--   0 tim.reichard   (502) staff       (20)     2058 2020-12-22 20:16:27.000000 aioradio-0.9.7/aioradio/jira.py
--rw-r--r--   0 tim.reichard   (502) staff       (20)     2842 2020-12-22 20:16:27.000000 aioradio-0.9.7/aioradio/logger.py
--rw-r--r--   0 tim.reichard   (502) staff       (20)     2661 2020-12-22 20:16:27.000000 aioradio-0.9.7/aioradio/pyodbc.py
--rw-r--r--   0 tim.reichard   (502) staff       (20)     5495 2020-12-22 20:16:27.000000 aioradio-0.9.7/aioradio/redis.py
-drwxr-xr-x   0 tim.reichard   (502) staff       (20)        0 2021-01-06 19:42:39.000000 aioradio-0.9.7/aioradio.egg-info/
--rw-r--r--   0 tim.reichard   (502) staff       (20)     9020 2021-01-06 19:42:38.000000 aioradio-0.9.7/aioradio.egg-info/PKG-INFO
--rw-r--r--   0 tim.reichard   (502) staff       (20)      489 2021-01-06 19:42:38.000000 aioradio-0.9.7/aioradio.egg-info/SOURCES.txt
--rw-r--r--   0 tim.reichard   (502) staff       (20)        1 2021-01-06 19:42:38.000000 aioradio-0.9.7/aioradio.egg-info/dependency_links.txt
--rw-r--r--   0 tim.reichard   (502) staff       (20)        1 2021-01-06 19:42:38.000000 aioradio-0.9.7/aioradio.egg-info/not-zip-safe
--rw-r--r--   0 tim.reichard   (502) staff       (20)      114 2021-01-06 19:42:38.000000 aioradio-0.9.7/aioradio.egg-info/requires.txt
--rw-r--r--   0 tim.reichard   (502) staff       (20)       22 2021-01-06 19:42:38.000000 aioradio-0.9.7/aioradio.egg-info/top_level.txt
--rw-r--r--   0 tim.reichard   (502) staff       (20)       63 2021-01-06 19:42:39.000000 aioradio-0.9.7/setup.cfg
--rw-r--r--   0 tim.reichard   (502) staff       (20)     1338 2021-01-06 19:36:17.000000 aioradio-0.9.7/setup.py
+drwxr-xr-x   0 tim.reichard   (502) staff       (20)        0 2021-02-01 15:47:19.000000 aioradio-0.9.8/
+-rw-r--r--   0 tim.reichard   (502) staff       (20)       24 2020-10-13 15:39:38.000000 aioradio-0.9.8/MANIFEST.in
+-rw-r--r--   0 tim.reichard   (502) staff       (20)     9020 2021-02-01 15:47:19.000000 aioradio-0.9.8/PKG-INFO
+-rw-r--r--   0 tim.reichard   (502) staff       (20)     6968 2020-11-10 19:42:27.000000 aioradio-0.9.8/README.md
+drwxr-xr-x   0 tim.reichard   (502) staff       (20)        0 2021-02-01 15:47:19.000000 aioradio-0.9.8/aioradio/
+-rw-r--r--   0 tim.reichard   (502) staff       (20)        0 2020-10-13 15:39:38.000000 aioradio-0.9.8/aioradio/__init__.py
+drwxr-xr-x   0 tim.reichard   (502) staff       (20)        0 2021-02-01 15:47:19.000000 aioradio-0.9.8/aioradio/aws/
+-rw-r--r--   0 tim.reichard   (502) staff       (20)     7416 2021-02-01 15:34:52.000000 aioradio-0.9.8/aioradio/aws/dynamodb.py
+-rw-r--r--   0 tim.reichard   (502) staff       (20)     4331 2020-12-22 20:16:27.000000 aioradio-0.9.8/aioradio/aws/moto_server.py
+-rw-r--r--   0 tim.reichard   (502) staff       (20)     3472 2021-02-01 14:44:25.000000 aioradio-0.9.8/aioradio/aws/s3.py
+-rw-r--r--   0 tim.reichard   (502) staff       (20)      995 2021-02-01 15:35:04.000000 aioradio-0.9.8/aioradio/aws/secrets.py
+-rw-r--r--   0 tim.reichard   (502) staff       (20)     4485 2021-02-01 15:25:46.000000 aioradio-0.9.8/aioradio/aws/sqs.py
+-rw-r--r--   0 tim.reichard   (502) staff       (20)     7935 2021-02-01 15:32:34.000000 aioradio-0.9.8/aioradio/aws/utils.py
+-rw-r--r--   0 tim.reichard   (502) staff       (20)    11215 2021-01-06 19:43:32.000000 aioradio-0.9.8/aioradio/file_ingestion.py
+-rw-r--r--   0 tim.reichard   (502) staff       (20)     2058 2020-12-22 20:16:27.000000 aioradio-0.9.8/aioradio/jira.py
+-rw-r--r--   0 tim.reichard   (502) staff       (20)     2842 2020-12-22 20:16:27.000000 aioradio-0.9.8/aioradio/logger.py
+-rw-r--r--   0 tim.reichard   (502) staff       (20)     2661 2020-12-22 20:16:27.000000 aioradio-0.9.8/aioradio/pyodbc.py
+-rw-r--r--   0 tim.reichard   (502) staff       (20)     5495 2020-12-22 20:16:27.000000 aioradio-0.9.8/aioradio/redis.py
+drwxr-xr-x   0 tim.reichard   (502) staff       (20)        0 2021-02-01 15:47:19.000000 aioradio-0.9.8/aioradio.egg-info/
+-rw-r--r--   0 tim.reichard   (502) staff       (20)     9020 2021-02-01 15:47:18.000000 aioradio-0.9.8/aioradio.egg-info/PKG-INFO
+-rw-r--r--   0 tim.reichard   (502) staff       (20)      489 2021-02-01 15:47:18.000000 aioradio-0.9.8/aioradio.egg-info/SOURCES.txt
+-rw-r--r--   0 tim.reichard   (502) staff       (20)        1 2021-02-01 15:47:18.000000 aioradio-0.9.8/aioradio.egg-info/dependency_links.txt
+-rw-r--r--   0 tim.reichard   (502) staff       (20)        1 2021-02-01 15:47:18.000000 aioradio-0.9.8/aioradio.egg-info/not-zip-safe
+-rw-r--r--   0 tim.reichard   (502) staff       (20)      114 2021-02-01 15:47:18.000000 aioradio-0.9.8/aioradio.egg-info/requires.txt
+-rw-r--r--   0 tim.reichard   (502) staff       (20)       22 2021-02-01 15:47:18.000000 aioradio-0.9.8/aioradio.egg-info/top_level.txt
+-rw-r--r--   0 tim.reichard   (502) staff       (20)       63 2021-02-01 15:47:19.000000 aioradio-0.9.8/setup.cfg
+-rw-r--r--   0 tim.reichard   (502) staff       (20)     1338 2021-02-01 15:39:30.000000 aioradio-0.9.8/setup.py
```

### Comparing `aioradio-0.9.7/PKG-INFO` & `aioradio-0.9.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioradio
-Version: 0.9.7
+Version: 0.9.8
 Summary: Generic asynchronous i/o python utilities for AWS services (SQS, S3, DynamoDB, Secrets Manager), Redis, MSSQL (pyodbc), JIRA and more
 Home-page: https://github.com/nrccua/aioradio
 Author: NRCCUA Architects
 Author-email: architecture@nrccua.org
 License: MIT
 Description: # aioradio
         Generic asynchronous i/o python utilities for AWS services (SQS, S3, DynamoDB, Secrets Manager), Redis, MSSQL (pyodbc), JIRA and more.
```

### Comparing `aioradio-0.9.7/README.md` & `aioradio-0.9.8/README.md`

 * *Files identical despite different names*

### Comparing `aioradio-0.9.7/aioradio/aws/dynamodb.py` & `aioradio-0.9.8/aioradio/aws/dynamodb.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,18 +2,28 @@
 
 # pylint: disable=too-many-arguments
 
 from typing import Any, Dict, List
 
 from aioradio.aws.utils import AwsServiceManager
 
-AWS_SERVICE = AwsServiceManager(service='dynamodb', regions=['us-east-1', 'us-east-2'], module='aioboto3')
+AWS_SERVICE = AwsServiceManager(service='dynamodb', regions=['us-east-1'], module='aioboto3')
 DYNAMO = AWS_SERVICE.service_dict
 
 
+async def add_regions(regions: List[str]):
+    """Add regions to DynamoDB AWS service.
+
+    Args:
+        regions (List[str]): List of AWS regions
+    """
+
+    AWS_SERVICE.add_regions(regions)
+
+
 @AWS_SERVICE.active
 async def create_dynamo_table(
         table_name: str,
         region: str,
         attribute_definitions: List[Dict[str, str]],
         key_schema: List[Dict[str, str]],
         provisioned_throughput: Dict[str, int]) -> str:
```

### Comparing `aioradio-0.9.7/aioradio/aws/moto_server.py` & `aioradio-0.9.8/aioradio/aws/moto_server.py`

 * *Files identical despite different names*

### Comparing `aioradio-0.9.7/aioradio/aws/s3.py` & `aioradio-0.9.8/aioradio/aws/s3.py`

 * *Files identical despite different names*

### Comparing `aioradio-0.9.7/aioradio/aws/sqs.py` & `aioradio-0.9.8/aioradio/aws/sqs.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,18 +7,28 @@
 from typing import Any, Dict, List
 
 from botocore.exceptions import ClientError
 
 from aioradio.aws.utils import AwsServiceManager
 
 LOG = logging.getLogger(__name__)
-AWS_SERVICE = AwsServiceManager(service='sqs', regions=['us-east-1', 'us-east-2'])
+AWS_SERVICE = AwsServiceManager(service='sqs', regions=['us-east-1'])
 SQS = AWS_SERVICE.service_dict
 
 
+async def add_regions(regions: List[str]):
+    """Add regions to SQS AWS service.
+
+    Args:
+        regions (List[str]): List of AWS regions
+    """
+
+    AWS_SERVICE.add_regions(regions)
+
+
 @AWS_SERVICE.active
 async def create_queue(queue: str, region: str, attributes: Dict[str, str]) -> Dict[str, Any]:
     """Create SQS queue in region defined.
 
     Args:
         queue (str): sqs queue
         region (str): AWS region
```

### Comparing `aioradio-0.9.7/aioradio/aws/utils.py` & `aioradio-0.9.8/aioradio/aws/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -50,26 +50,55 @@
             if loop and loop.is_running():
                 asyncio.create_task(self.create_scheduler())
             else:
                 loop.run_until_complete(self.create_scheduler())
         except RuntimeError:
             loop = asyncio.new_event_loop().run_until_complete(self.create_scheduler())
 
+    def add_regions(self, regions: List[str]):
+        """Add regions to AWS service.
+
+        Args:
+            regions (List[str]): [description]
+        """
+
+        data = {'client': {'obj': None, 'session': None, 'busy': True}, 'active': 0}
+        if self.service == 'dynamodb':
+            data['resource'] = {'obj': None, 'session': None, 'busy': True}
+
+        for region in regions:
+            if region not in self.regions:
+                self.regions.append(region)
+                self.service_dict[region] = deepcopy(data)
+                asyncio.get_event_loop().create_task(self.spawn_aws_service_process(region))
+
     def __del__(self):
         self.scheduler.close()
 
     async def create_scheduler(self):
         """Schedule jobs."""
 
         self.scheduler = await aiojobs.create_scheduler()
         if self.regions:
             for region in self.regions:
-                await self.scheduler.spawn(self.aio_server(item='client', region=region))
-                if self.module == 'aioboto3':
-                    await self.scheduler.spawn(self.aio_server(item='resource', region=region))
+                await self.spawn_aws_service_process(region)
+        else:
+            await self.spawn_aws_service_process()
+
+    async def spawn_aws_service_process(self, region: str=''):
+        """Spawn scheduler process on a per region basis.
+
+        Args:
+            region (str, optional): AWS region. Defaults to ''.
+        """
+
+        if region:
+            await self.scheduler.spawn(self.aio_server(item='client', region=region))
+            if self.module == 'aioboto3':
+                await self.scheduler.spawn(self.aio_server(item='resource', region=region))
         else:
             await self.scheduler.spawn(self.aio_server(item='client'))
             if self.module == 'aioboto3':
                 await self.scheduler.spawn(self.aio_server(item='resource'))
 
     async def aio_server(self, item: str, region: str=''):
         """Begin long running server establishing modules service_dict object.
```

### Comparing `aioradio-0.9.7/aioradio/file_ingestion.py` & `aioradio-0.9.8/aioradio/file_ingestion.py`

 * *Files identical despite different names*

### Comparing `aioradio-0.9.7/aioradio/jira.py` & `aioradio-0.9.8/aioradio/jira.py`

 * *Files identical despite different names*

### Comparing `aioradio-0.9.7/aioradio/logger.py` & `aioradio-0.9.8/aioradio/logger.py`

 * *Files identical despite different names*

### Comparing `aioradio-0.9.7/aioradio/pyodbc.py` & `aioradio-0.9.8/aioradio/pyodbc.py`

 * *Files identical despite different names*

### Comparing `aioradio-0.9.7/aioradio/redis.py` & `aioradio-0.9.8/aioradio/redis.py`

 * *Files identical despite different names*

### Comparing `aioradio-0.9.7/aioradio.egg-info/PKG-INFO` & `aioradio-0.9.8/aioradio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioradio
-Version: 0.9.7
+Version: 0.9.8
 Summary: Generic asynchronous i/o python utilities for AWS services (SQS, S3, DynamoDB, Secrets Manager), Redis, MSSQL (pyodbc), JIRA and more
 Home-page: https://github.com/nrccua/aioradio
 Author: NRCCUA Architects
 Author-email: architecture@nrccua.org
 License: MIT
 Description: # aioradio
         Generic asynchronous i/o python utilities for AWS services (SQS, S3, DynamoDB, Secrets Manager), Redis, MSSQL (pyodbc), JIRA and more.
```

### Comparing `aioradio-0.9.7/setup.py` & `aioradio-0.9.8/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from setuptools import setup
 
 with open('README.md', 'r') as fileobj:
     long_description = fileobj.read()
 
 setup(name='aioradio',
-    version='0.9.7',
+    version='0.9.8',
     description='Generic asynchronous i/o python utilities for AWS services (SQS, S3, DynamoDB, Secrets Manager), Redis, MSSQL (pyodbc), JIRA and more',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/nrccua/aioradio',
     author='NRCCUA Architects',
     author_email='architecture@nrccua.org',
     license="MIT",
```

