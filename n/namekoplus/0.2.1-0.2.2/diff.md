# Comparing `tmp/namekoplus-0.2.1.tar.gz` & `tmp/namekoplus-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "namekoplus-0.2.1.tar", last modified: Fri Jul 21 07:44:52 2023, max compression
+gzip compressed data, was "namekoplus-0.2.2.tar", last modified: Fri Jul 21 08:58:36 2023, max compression
```

## Comparing `namekoplus-0.2.1.tar` & `namekoplus-0.2.2.tar`

### file list

```diff
@@ -1,46 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:44:52.043686 namekoplus-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-21 07:44:35.000000 namekoplus-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-21 07:44:35.000000 namekoplus-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-07-21 07:44:52.043686 namekoplus-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-21 07:44:35.000000 namekoplus-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:44:52.039687 namekoplus-0.2.1/namekoplus/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-21 07:44:35.000000 namekoplus-0.2.1/namekoplus/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:44:52.039687 namekoplus-0.2.1/namekoplus/chassis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 07:44:35.000000 namekoplus-0.2.1/namekoplus/chassis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-21 07:44:35.000000 namekoplus-0.2.1/namekoplus/chassis/chassis.py
--rw-r--r--   0 runner    (1001) docker     (123)     4696 2023-07-21 07:44:35.000000 namekoplus-0.2.1/namekoplus/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:44:52.039687 namekoplus-0.2.1/namekoplus/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 07:44:35.000000 namekoplus-0.2.1/namekoplus/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:44:52.039687 namekoplus-0.2.1/namekoplus/templates/all/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 07:44:35.000000 namekoplus-0.2.1/namekoplus/templates/all/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-07-21 07:44:35.000000 namekoplus-0.2.1/namekoplus/templates/all/all_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-21 07:44:35.000000 namekoplus-0.2.1/namekoplus/templates/all/config.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:44:52.039687 namekoplus-0.2.1/namekoplus/templates/demo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 07:44:35.000000 namekoplus-0.2.1/namekoplus/templates/demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-21 07:44:35.000000 namekoplus-0.2.1/namekoplus/templates/demo/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-07-21 07:44:35.000000 namekoplus-0.2.1/namekoplus/templates/demo/rpc_demo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:44:52.039687 namekoplus-0.2.1/namekoplus/templates/event/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 07:44:35.000000 namekoplus-0.2.1/namekoplus/templates/event/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-21 07:44:35.000000 namekoplus-0.2.1/namekoplus/templates/event/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-07-21 07:44:35.000000 namekoplus-0.2.1/namekoplus/templates/event/events_demo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:44:52.043686 namekoplus-0.2.1/namekoplus/templates/http/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 07:44:35.000000 namekoplus-0.2.1/namekoplus/templates/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-21 07:44:35.000000 namekoplus-0.2.1/namekoplus/templates/http/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-21 07:44:35.000000 namekoplus-0.2.1/namekoplus/templates/http/http_demo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:44:52.043686 namekoplus-0.2.1/namekoplus/templates/rpc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 07:44:35.000000 namekoplus-0.2.1/namekoplus/templates/rpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-21 07:44:35.000000 namekoplus-0.2.1/namekoplus/templates/rpc/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-21 07:44:35.000000 namekoplus-0.2.1/namekoplus/templates/rpc/rpc_demo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:44:52.043686 namekoplus-0.2.1/namekoplus/templates/timer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 07:44:35.000000 namekoplus-0.2.1/namekoplus/templates/timer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-21 07:44:35.000000 namekoplus-0.2.1/namekoplus/templates/timer/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-21 07:44:35.000000 namekoplus-0.2.1/namekoplus/templates/timer/timer_demo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:44:52.039687 namekoplus-0.2.1/namekoplus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-07-21 07:44:52.000000 namekoplus-0.2.1/namekoplus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-21 07:44:52.000000 namekoplus-0.2.1/namekoplus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 07:44:52.000000 namekoplus-0.2.1/namekoplus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-21 07:44:52.000000 namekoplus-0.2.1/namekoplus.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-21 07:44:52.000000 namekoplus-0.2.1/namekoplus.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-21 07:44:52.000000 namekoplus-0.2.1/namekoplus.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 07:44:52.043686 namekoplus-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-07-21 07:44:35.000000 namekoplus-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:58:36.876320 namekoplus-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-21 08:58:24.000000 namekoplus-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-21 08:58:24.000000 namekoplus-0.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-07-21 08:58:36.876320 namekoplus-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-21 08:58:24.000000 namekoplus-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:58:36.872321 namekoplus-0.2.2/namekoplus/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-21 08:58:24.000000 namekoplus-0.2.2/namekoplus/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:58:36.872321 namekoplus-0.2.2/namekoplus/chassis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 08:58:24.000000 namekoplus-0.2.2/namekoplus/chassis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-21 08:58:24.000000 namekoplus-0.2.2/namekoplus/chassis/chassis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:58:36.872321 namekoplus-0.2.2/namekoplus/chassis-agent/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 08:58:24.000000 namekoplus-0.2.2/namekoplus/chassis-agent/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:58:36.872321 namekoplus-0.2.2/namekoplus/chassis-agent/rabbitmq/
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-07-21 08:58:24.000000 namekoplus-0.2.2/namekoplus/chassis-agent/rabbitmq/docker-compose-rabbitmq.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4696 2023-07-21 08:58:24.000000 namekoplus-0.2.2/namekoplus/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:58:36.872321 namekoplus-0.2.2/namekoplus/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 08:58:24.000000 namekoplus-0.2.2/namekoplus/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:58:36.872321 namekoplus-0.2.2/namekoplus/templates/all/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 08:58:24.000000 namekoplus-0.2.2/namekoplus/templates/all/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-07-21 08:58:24.000000 namekoplus-0.2.2/namekoplus/templates/all/all_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-21 08:58:24.000000 namekoplus-0.2.2/namekoplus/templates/all/config.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:58:36.872321 namekoplus-0.2.2/namekoplus/templates/demo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 08:58:24.000000 namekoplus-0.2.2/namekoplus/templates/demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-21 08:58:24.000000 namekoplus-0.2.2/namekoplus/templates/demo/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-07-21 08:58:24.000000 namekoplus-0.2.2/namekoplus/templates/demo/rpc_demo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:58:36.872321 namekoplus-0.2.2/namekoplus/templates/event/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 08:58:24.000000 namekoplus-0.2.2/namekoplus/templates/event/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-21 08:58:24.000000 namekoplus-0.2.2/namekoplus/templates/event/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-07-21 08:58:24.000000 namekoplus-0.2.2/namekoplus/templates/event/events_demo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:58:36.872321 namekoplus-0.2.2/namekoplus/templates/http/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 08:58:24.000000 namekoplus-0.2.2/namekoplus/templates/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-21 08:58:24.000000 namekoplus-0.2.2/namekoplus/templates/http/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-21 08:58:24.000000 namekoplus-0.2.2/namekoplus/templates/http/http_demo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:58:36.876320 namekoplus-0.2.2/namekoplus/templates/rpc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 08:58:24.000000 namekoplus-0.2.2/namekoplus/templates/rpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-21 08:58:24.000000 namekoplus-0.2.2/namekoplus/templates/rpc/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-21 08:58:24.000000 namekoplus-0.2.2/namekoplus/templates/rpc/rpc_demo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:58:36.876320 namekoplus-0.2.2/namekoplus/templates/timer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 08:58:24.000000 namekoplus-0.2.2/namekoplus/templates/timer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-21 08:58:24.000000 namekoplus-0.2.2/namekoplus/templates/timer/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-21 08:58:24.000000 namekoplus-0.2.2/namekoplus/templates/timer/timer_demo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:58:36.872321 namekoplus-0.2.2/namekoplus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-07-21 08:58:36.000000 namekoplus-0.2.2/namekoplus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-07-21 08:58:36.000000 namekoplus-0.2.2/namekoplus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 08:58:36.000000 namekoplus-0.2.2/namekoplus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-21 08:58:36.000000 namekoplus-0.2.2/namekoplus.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-21 08:58:36.000000 namekoplus-0.2.2/namekoplus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-21 08:58:36.000000 namekoplus-0.2.2/namekoplus.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 08:58:36.876320 namekoplus-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-07-21 08:58:24.000000 namekoplus-0.2.2/setup.py
```

### Comparing `namekoplus-0.2.1/LICENSE` & `namekoplus-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `namekoplus-0.2.1/PKG-INFO` & `namekoplus-0.2.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: namekoplus
-Version: 0.2.1
+Version: 0.2.2
 Summary: A lightweight Python distributed microservice solution
 Home-page: 
 Author: Bryant He
 Author-email: bryantsisu@qq.com
 License: MIT
 Project-URL: Documentation, https://doc.bearcatlog.com/
 Project-URL: Source Code, https://github.com/Bryanthelol/namekoplus
@@ -13,15 +13,15 @@
 Platform: any
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3
+Requires-Python: >=3.8, <4
 Description-Content-Type: text/markdown
 Provides-Extra: ha
 Provides-Extra: apiflask
 Provides-Extra: rocketry
 Provides-Extra: gutter
 Provides-Extra: mysql
 Provides-Extra: ssl
```

### Comparing `namekoplus-0.2.1/namekoplus/chassis/chassis.py` & `namekoplus-0.2.2/namekoplus/chassis/chassis.py`

 * *Files identical despite different names*

### Comparing `namekoplus-0.2.1/namekoplus/command.py` & `namekoplus-0.2.2/namekoplus/command.py`

 * *Files identical despite different names*

### Comparing `namekoplus-0.2.1/namekoplus/templates/all/all_demo.py` & `namekoplus-0.2.2/namekoplus/templates/all/all_demo.py`

 * *Files identical despite different names*

### Comparing `namekoplus-0.2.1/namekoplus/templates/all/config.yml` & `namekoplus-0.2.2/namekoplus/templates/all/config.yml`

 * *Files identical despite different names*

### Comparing `namekoplus-0.2.1/namekoplus/templates/event/config.yml` & `namekoplus-0.2.2/namekoplus/templates/event/config.yml`

 * *Files identical despite different names*

### Comparing `namekoplus-0.2.1/namekoplus/templates/event/events_demo.py` & `namekoplus-0.2.2/namekoplus/templates/event/events_demo.py`

 * *Files identical despite different names*

### Comparing `namekoplus-0.2.1/namekoplus/templates/http/config.yml` & `namekoplus-0.2.2/namekoplus/templates/http/config.yml`

 * *Files identical despite different names*

### Comparing `namekoplus-0.2.1/namekoplus/templates/http/http_demo.py` & `namekoplus-0.2.2/namekoplus/templates/http/http_demo.py`

 * *Files identical despite different names*

### Comparing `namekoplus-0.2.1/namekoplus/templates/rpc/config.yml` & `namekoplus-0.2.2/namekoplus/templates/rpc/config.yml`

 * *Files identical despite different names*

### Comparing `namekoplus-0.2.1/namekoplus/templates/rpc/rpc_demo.py` & `namekoplus-0.2.2/namekoplus/templates/rpc/rpc_demo.py`

 * *Files identical despite different names*

### Comparing `namekoplus-0.2.1/namekoplus/templates/timer/config.yml` & `namekoplus-0.2.2/namekoplus/templates/timer/config.yml`

 * *Files identical despite different names*

### Comparing `namekoplus-0.2.1/namekoplus.egg-info/PKG-INFO` & `namekoplus-0.2.2/namekoplus.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: namekoplus
-Version: 0.2.1
+Version: 0.2.2
 Summary: A lightweight Python distributed microservice solution
 Home-page: 
 Author: Bryant He
 Author-email: bryantsisu@qq.com
 License: MIT
 Project-URL: Documentation, https://doc.bearcatlog.com/
 Project-URL: Source Code, https://github.com/Bryanthelol/namekoplus
@@ -13,15 +13,15 @@
 Platform: any
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3
+Requires-Python: >=3.8, <4
 Description-Content-Type: text/markdown
 Provides-Extra: ha
 Provides-Extra: apiflask
 Provides-Extra: rocketry
 Provides-Extra: gutter
 Provides-Extra: mysql
 Provides-Extra: ssl
```

### Comparing `namekoplus-0.2.1/namekoplus.egg-info/SOURCES.txt` & `namekoplus-0.2.2/namekoplus.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 namekoplus.egg-info/SOURCES.txt
 namekoplus.egg-info/dependency_links.txt
 namekoplus.egg-info/entry_points.txt
 namekoplus.egg-info/requires.txt
 namekoplus.egg-info/top_level.txt
 namekoplus/chassis/__init__.py
 namekoplus/chassis/chassis.py
+namekoplus/chassis-agent/__init__.py
+namekoplus/chassis-agent/rabbitmq/docker-compose-rabbitmq.yml
 namekoplus/templates/__init__.py
 namekoplus/templates/all/__init__.py
 namekoplus/templates/all/all_demo.py
 namekoplus/templates/all/config.yml
 namekoplus/templates/demo/__init__.py
 namekoplus/templates/demo/config.yml
 namekoplus/templates/demo/rpc_demo.py
```

### Comparing `namekoplus-0.2.1/setup.py` & `namekoplus-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 here = path.abspath(path.dirname(__file__))
 
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='namekoplus',
-    version='0.2.1',
+    version='0.2.2',
     description='A lightweight Python distributed microservice solution',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='',
     project_urls={
         'Documentation': 'https://doc.bearcatlog.com/',
         'Source Code': 'https://github.com/Bryanthelol/namekoplus',
@@ -29,15 +29,15 @@
         'Environment :: Web Environment',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Topic :: Software Development :: Libraries :: Python Modules',
     ],
     platforms='any',
-    python_requires='>=3',
+    python_requires='>=3.8, <4',
 
     keywords='lightweight python distributed microservice solution',
 
     packages=find_packages(exclude=['contrib', 'docs', 'tests']),
     include_package_data=True,
     data_files=['README.md'],
```

