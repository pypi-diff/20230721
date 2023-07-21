# Comparing `tmp/zpapollo-1.0.1.tar.gz` & `tmp/zpapollo-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/zpapollo-1.0.1.tar", last modified: Thu Jul 20 08:58:12 2023, max compression
+gzip compressed data, was "dist/zpapollo-1.1.0.tar", last modified: Fri Jul 21 07:55:23 2023, max compression
```

## Comparing `zpapollo-1.0.1.tar` & `zpapollo-1.1.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 zhidong    (503) staff       (20)        0 2023-07-20 08:58:12.000000 zpapollo-1.0.1/
--rw-r--r--   0 zhidong    (503) staff       (20)      496 2023-07-20 08:58:12.000000 zpapollo-1.0.1/PKG-INFO
--rw-r--r--   0 zhidong    (503) staff       (20)     1503 2023-07-20 07:34:11.000000 zpapollo-1.0.1/README.md
-drwxr-xr-x   0 zhidong    (503) staff       (20)        0 2023-07-20 08:58:12.000000 zpapollo-1.0.1/apollo/
--rw-r--r--   0 zhidong    (503) staff       (20)       75 2023-07-20 08:23:59.000000 zpapollo-1.0.1/apollo/__init__.py
--rw-r--r--   0 zhidong    (503) staff       (20)    10895 2023-07-20 07:34:11.000000 zpapollo-1.0.1/apollo/apollo_client.py
--rw-r--r--   0 zhidong    (503) staff       (20)      900 2023-07-20 07:34:11.000000 zpapollo-1.0.1/apollo/python_2x.py
--rw-r--r--   0 zhidong    (503) staff       (20)     1034 2023-07-20 07:34:11.000000 zpapollo-1.0.1/apollo/python_3x.py
--rw-r--r--   0 zhidong    (503) staff       (20)     1386 2023-07-20 07:34:11.000000 zpapollo-1.0.1/apollo/util.py
-drwxr-xr-x   0 zhidong    (503) staff       (20)        0 2023-07-20 08:58:12.000000 zpapollo-1.0.1/demo/
--rw-r--r--   0 zhidong    (503) staff       (20)        0 2023-07-20 07:34:11.000000 zpapollo-1.0.1/demo/__init__.py
--rw-r--r--   0 zhidong    (503) staff       (20)      410 2023-07-20 07:34:11.000000 zpapollo-1.0.1/demo/demo.py
--rw-r--r--   0 zhidong    (503) staff       (20)      787 2023-07-20 07:34:11.000000 zpapollo-1.0.1/demo/demo_listener.py
--rw-r--r--   0 zhidong    (503) staff       (20)      487 2023-07-20 07:34:11.000000 zpapollo-1.0.1/demo/demo_secret.py
--rw-r--r--   0 zhidong    (503) staff       (20)       38 2023-07-20 08:58:12.000000 zpapollo-1.0.1/setup.cfg
--rw-r--r--   0 zhidong    (503) staff       (20)      804 2023-07-20 08:53:33.000000 zpapollo-1.0.1/setup.py
-drwxr-xr-x   0 zhidong    (503) staff       (20)        0 2023-07-20 08:58:12.000000 zpapollo-1.0.1/zpapollo.egg-info/
--rw-r--r--   0 zhidong    (503) staff       (20)      496 2023-07-20 08:58:12.000000 zpapollo-1.0.1/zpapollo.egg-info/PKG-INFO
--rw-r--r--   0 zhidong    (503) staff       (20)      378 2023-07-20 08:58:12.000000 zpapollo-1.0.1/zpapollo.egg-info/SOURCES.txt
--rw-r--r--   0 zhidong    (503) staff       (20)        1 2023-07-20 08:58:12.000000 zpapollo-1.0.1/zpapollo.egg-info/dependency_links.txt
--rw-r--r--   0 zhidong    (503) staff       (20)        1 2023-07-20 08:54:53.000000 zpapollo-1.0.1/zpapollo.egg-info/not-zip-safe
--rw-r--r--   0 zhidong    (503) staff       (20)        9 2023-07-20 08:58:12.000000 zpapollo-1.0.1/zpapollo.egg-info/requires.txt
--rw-r--r--   0 zhidong    (503) staff       (20)       12 2023-07-20 08:58:12.000000 zpapollo-1.0.1/zpapollo.egg-info/top_level.txt
+drwxr-xr-x   0 zhidong    (503) staff       (20)        0 2023-07-21 07:55:23.000000 zpapollo-1.1.0/
+-rw-r--r--   0 zhidong    (503) staff       (20)      499 2023-07-21 07:55:23.000000 zpapollo-1.1.0/PKG-INFO
+-rw-r--r--   0 zhidong    (503) staff       (20)     1503 2023-07-20 07:34:11.000000 zpapollo-1.1.0/README.md
+drwxr-xr-x   0 zhidong    (503) staff       (20)        0 2023-07-21 07:55:23.000000 zpapollo-1.1.0/apollo/
+-rw-r--r--   0 zhidong    (503) staff       (20)       79 2023-07-21 07:54:26.000000 zpapollo-1.1.0/apollo/__init__.py
+-rw-r--r--   0 zhidong    (503) staff       (20)    13494 2023-07-21 07:24:41.000000 zpapollo-1.1.0/apollo/apollo_client.py
+-rw-r--r--   0 zhidong    (503) staff       (20)      900 2023-07-20 07:34:11.000000 zpapollo-1.1.0/apollo/python_2x.py
+-rw-r--r--   0 zhidong    (503) staff       (20)     1032 2023-07-20 10:08:27.000000 zpapollo-1.1.0/apollo/python_3x.py
+-rw-r--r--   0 zhidong    (503) staff       (20)     1386 2023-07-20 07:34:11.000000 zpapollo-1.1.0/apollo/util.py
+drwxr-xr-x   0 zhidong    (503) staff       (20)        0 2023-07-21 07:55:23.000000 zpapollo-1.1.0/demo/
+-rw-r--r--   0 zhidong    (503) staff       (20)        0 2023-07-20 07:34:11.000000 zpapollo-1.1.0/demo/__init__.py
+-rw-r--r--   0 zhidong    (503) staff       (20)      400 2023-07-21 04:09:11.000000 zpapollo-1.1.0/demo/demo.py
+-rw-r--r--   0 zhidong    (503) staff       (20)      777 2023-07-21 04:09:11.000000 zpapollo-1.1.0/demo/demo_listener.py
+-rw-r--r--   0 zhidong    (503) staff       (20)      477 2023-07-21 04:09:11.000000 zpapollo-1.1.0/demo/demo_secret.py
+-rw-r--r--   0 zhidong    (503) staff       (20)       38 2023-07-21 07:55:23.000000 zpapollo-1.1.0/setup.cfg
+-rw-r--r--   0 zhidong    (503) staff       (20)      804 2023-07-20 08:53:33.000000 zpapollo-1.1.0/setup.py
+drwxr-xr-x   0 zhidong    (503) staff       (20)        0 2023-07-21 07:55:23.000000 zpapollo-1.1.0/zpapollo.egg-info/
+-rw-r--r--   0 zhidong    (503) staff       (20)      499 2023-07-21 07:55:23.000000 zpapollo-1.1.0/zpapollo.egg-info/PKG-INFO
+-rw-r--r--   0 zhidong    (503) staff       (20)      378 2023-07-21 07:55:23.000000 zpapollo-1.1.0/zpapollo.egg-info/SOURCES.txt
+-rw-r--r--   0 zhidong    (503) staff       (20)        1 2023-07-21 07:55:23.000000 zpapollo-1.1.0/zpapollo.egg-info/dependency_links.txt
+-rw-r--r--   0 zhidong    (503) staff       (20)        1 2023-07-20 08:54:53.000000 zpapollo-1.1.0/zpapollo.egg-info/not-zip-safe
+-rw-r--r--   0 zhidong    (503) staff       (20)        9 2023-07-21 07:55:23.000000 zpapollo-1.1.0/zpapollo.egg-info/requires.txt
+-rw-r--r--   0 zhidong    (503) staff       (20)       12 2023-07-21 07:55:23.000000 zpapollo-1.1.0/zpapollo.egg-info/top_level.txt
```

### Comparing `zpapollo-1.0.1/README.md` & `zpapollo-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `zpapollo-1.0.1/apollo/apollo_client.py` & `zpapollo-1.1.0/apollo/apollo_client.py`

 * *Files 26% similar despite different names*

```diff
@@ -27,24 +27,32 @@
                     datefmt='%d-%m-%Y:%H:%M:%S',
                     level=logging.DEBUG)
 
 
 class ApolloClient(object):
 
     def __init__(self, config_url, app_id, cluster='default', secret='', start_hot_update=True,
-                 change_listener=None):
+                 change_listener=None, namespaces=None, label='', bak_config_url=None):
+        if not config_url:
+            raise Exception("error, config url is required")
+        if config_url[-1] == '/':  # 后面会拼接地址，去除多余的斜杠
+            config_url = config_url[:-1]
+        if not namespaces:
+            namespaces = ['application']
 
         # 核心路由参数
         self.config_url = config_url
         self.cluster = cluster
         self.app_id = app_id
 
         # 非核心参数
         self.ip = init_ip()
+        self.label = label
         self.secret = secret
+        self.namespaces = namespaces
 
         # 检查参数变量
 
         # 私有控制变量
         self._cycle_time = 2
         self._stopping = False
         self._cache = {}
@@ -54,49 +62,63 @@
         self._cache_file_path = os.path.expanduser('~') + '/data/apollo/cache/'
         self._long_poll_thread = None
         self._change_listener = change_listener  # "add" "delete" "update"
         self._notification_map = {'application': -1}
         self.last_release_key = None
         # 私有启动方法
         self._path_checker()
+
+        if not self.namespace_check_ok():
+            if bak_config_url:
+                logging.warning(
+                    "error, start with main config url [{}] fail, using bak config url: {}".format(config_url, bak_config_url))
+                self.config_url = bak_config_url
+                if not self.namespace_check_ok():
+                    logging.error(
+                        "error, start with bak config url [{}] fail".format(bak_config_url))
+                    raise Exception('error, namespace_check fail')
+            else:
+                logging.error("error, start with main config url [{}] fail, no bak config url provided".format(config_url))
+                raise Exception('error, namespace_check fail')
+
         if start_hot_update:
             self._start_hot_update()
 
         # 启动心跳线程
         heartbeat = threading.Thread(target=self._heartBeat)
         heartbeat.setDaemon(True)
         heartbeat.start()
 
     def get_json_from_net(self, namespace='application'):
-        url = '{}/configs/{}/{}/{}?releaseKey={}&ip={}'.format(self.config_url, self.app_id, self.cluster, namespace,
-                                                               "", self.ip)
+        url = '{}/configs/{}/{}/{}?releaseKey={}&ip={}&label={}'.format(self.config_url, self.app_id, self.cluster, namespace,
+                                                               "", self.ip, self.label)
         try:
             code, body = http_request(url, timeout=3, headers=self._signHeaders(url))
             if code == 200:
                 data = json.loads(body)
                 data = data["configurations"]
                 return_data = {CONFIGURATIONS: data}
                 return return_data
             else:
                 return None
         except Exception as e:
             logging.getLogger(__name__).error(str(e))
             return None
 
-    def get_value(self, key, default_val=None, namespace='application'):
+    def get(self, key, default=None, namespace='application'):
         try:
             # 读取内存配置
             namespace_cache = self._cache.get(namespace)
             val = get_value_from_dict(namespace_cache, key)
             if val is not None:
                 return val
 
             no_key = no_key_cache_key(namespace, key)
             if no_key in self._no_key:
-                return default_val
+                return default
 
             # 读取网络配置
             namespace_data = self.get_json_from_net(namespace)
             val = get_value_from_dict(namespace_data, key)
             if val is not None:
                 self._update_cache_and_file(namespace_data, namespace)
                 return val
@@ -106,19 +128,54 @@
             val = get_value_from_dict(namespace_cache, key)
             if val is not None:
                 self._update_cache_and_file(namespace_cache, namespace)
                 return val
 
             # 如果全部没有获取，则把默认值返回，设置本地缓存为None
             self._set_local_cache_none(namespace, key)
-            return default_val
+            return default
         except Exception as e:
             logging.getLogger(__name__).error("get_value has error, [key is %s], [namespace is %s], [error is %s], ",
                                               key, namespace, e)
-            return default_val
+            return default
+
+    def get_all(self, namespace='application', default=None, allow_cache=True):
+        try:
+            if allow_cache:
+                # 读取内存配置
+                namespace_cache = self._cache.get(namespace)
+                if namespace_cache is not None:
+                    return namespace_cache.get(CONFIGURATIONS, default)
+
+            # 读取网络配置
+            namespace_data = self.get_json_from_net(namespace)
+            if namespace_data:
+                self._update_cache_and_file(namespace_data, namespace)
+                return namespace_data.get(CONFIGURATIONS, default)
+
+            if allow_cache:
+                # 读取文件配置
+                namespace_cache = self._get_local_cache(namespace)
+                if namespace_cache is not None:
+                    self._update_cache_and_file(namespace_cache, namespace)
+                    return namespace_cache.get(CONFIGURATIONS, default)
+
+            return default
+        except Exception as e:
+            logging.getLogger(__name__).error("get_all has error, [namespace is %s], [error is %s], ",
+                                              namespace, e)
+            return default
+
+    def namespace_check_ok(self):
+        for ns in self.namespaces:
+            configs = self.get_all(namespace=ns, allow_cache=False)
+            if configs is None:
+                logging.error("namespace [{}] check fail".format(ns))
+                return False
+        return True
 
     # 设置某个namespace的key为none，这里不设置default_val，是为了保证函数调用实时的正确性。
     # 假设用户2次default_val不一样，然而这里却用default_val填充，则可能会有问题。
     def _set_local_cache_none(self, namespace, key):
         no_key = no_key_cache_key(namespace, key)
         self._no_key[no_key] = key
```

### Comparing `zpapollo-1.0.1/apollo/python_2x.py` & `zpapollo-1.1.0/apollo/python_2x.py`

 * *Files identical despite different names*

### Comparing `zpapollo-1.0.1/apollo/python_3x.py` & `zpapollo-1.1.0/apollo/python_3x.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,27 +8,27 @@
 
 import urllib.request
 from urllib.error import HTTPError
 from urllib import parse
 import requests
 
 
-def http_request(url, timeout, headers={}):
+def http_request(url, timeout, headers=None):
     try:
         # request = urllib.request.Request(url, headers=headers)
         # res = urllib.request.urlopen(request, timeout=timeout)
         # body = res.read().decode("utf-8")
         # return res.code, body
         r = requests.get(url, headers=headers, timeout=timeout)
         return r.status_code, r.text
     except HTTPError as e:
         if e.code == 304:
             logging.getLogger(__name__).warning("http_request error,code is 304, maybe you should check secret")
             return 304, None
-        logging.getLogger(__name__).warning("http_request error,code is %d, msg is %s", e.code, e.msg)
+        logging.getLogger(__name__).warning("http_request error,code is %d, msg is %s", e.code, e)
         raise e
 
 
 def url_encode(params):
     return parse.urlencode(params)
```

### Comparing `zpapollo-1.0.1/apollo/util.py` & `zpapollo-1.1.0/apollo/util.py`

 * *Files identical despite different names*

### Comparing `zpapollo-1.0.1/demo/demo_listener.py` & `zpapollo-1.1.0/demo/demo_listener.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,11 +19,11 @@
 # ('add', u'application', u'cc', u'dd')
 def listener(change_type, namespace, key, value):
     print(change_type, namespace, key, value)
 
 
 client = ApolloClient(app_id="demo-service", cluster="default", config_url=apollo_config_url,
                       change_listener=listener)
-val = client.get_value("name", default_val="defaultVal")
+val = client.get("name", default="defaultVal")
 
 print(val)
 time.sleep(100)
```

### Comparing `zpapollo-1.0.1/setup.py` & `zpapollo-1.1.0/setup.py`

 * *Files identical despite different names*

