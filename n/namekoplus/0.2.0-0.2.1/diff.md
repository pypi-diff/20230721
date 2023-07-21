# Comparing `tmp/namekoplus-0.2.0.tar.gz` & `tmp/namekoplus-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "namekoplus-0.2.0.tar", last modified: Fri Jul 21 05:12:37 2023, max compression
+gzip compressed data, was "namekoplus-0.2.1.tar", last modified: Fri Jul 21 07:44:52 2023, max compression
```

## Comparing `namekoplus-0.2.0.tar` & `namekoplus-0.2.1.tar`

### file list

```diff
@@ -1,42 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:12:37.509815 namekoplus-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-21 05:12:22.000000 namekoplus-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-21 05:12:22.000000 namekoplus-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-07-21 05:12:37.509815 namekoplus-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-21 05:12:22.000000 namekoplus-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:12:37.509815 namekoplus-0.2.0/namekoplus/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-21 05:12:22.000000 namekoplus-0.2.0/namekoplus/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:12:37.509815 namekoplus-0.2.0/namekoplus/chassis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 05:12:22.000000 namekoplus-0.2.0/namekoplus/chassis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-21 05:12:22.000000 namekoplus-0.2.0/namekoplus/chassis/chassis.py
--rw-r--r--   0 runner    (1001) docker     (123)     4688 2023-07-21 05:12:22.000000 namekoplus-0.2.0/namekoplus/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:12:37.509815 namekoplus-0.2.0/namekoplus/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 05:12:22.000000 namekoplus-0.2.0/namekoplus/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:12:37.509815 namekoplus-0.2.0/namekoplus/templates/all/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 05:12:22.000000 namekoplus-0.2.0/namekoplus/templates/all/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-07-21 05:12:22.000000 namekoplus-0.2.0/namekoplus/templates/all/all_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-21 05:12:22.000000 namekoplus-0.2.0/namekoplus/templates/all/config.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:12:37.509815 namekoplus-0.2.0/namekoplus/templates/event/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 05:12:22.000000 namekoplus-0.2.0/namekoplus/templates/event/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-21 05:12:22.000000 namekoplus-0.2.0/namekoplus/templates/event/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-07-21 05:12:22.000000 namekoplus-0.2.0/namekoplus/templates/event/events_demo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:12:37.509815 namekoplus-0.2.0/namekoplus/templates/http/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 05:12:22.000000 namekoplus-0.2.0/namekoplus/templates/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-21 05:12:22.000000 namekoplus-0.2.0/namekoplus/templates/http/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-21 05:12:22.000000 namekoplus-0.2.0/namekoplus/templates/http/http_demo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:12:37.509815 namekoplus-0.2.0/namekoplus/templates/rpc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 05:12:22.000000 namekoplus-0.2.0/namekoplus/templates/rpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-21 05:12:22.000000 namekoplus-0.2.0/namekoplus/templates/rpc/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-21 05:12:22.000000 namekoplus-0.2.0/namekoplus/templates/rpc/rpc_demo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:12:37.509815 namekoplus-0.2.0/namekoplus/templates/timer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 05:12:22.000000 namekoplus-0.2.0/namekoplus/templates/timer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-21 05:12:22.000000 namekoplus-0.2.0/namekoplus/templates/timer/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-21 05:12:22.000000 namekoplus-0.2.0/namekoplus/templates/timer/timer_demo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:12:37.509815 namekoplus-0.2.0/namekoplus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-07-21 05:12:37.000000 namekoplus-0.2.0/namekoplus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-07-21 05:12:37.000000 namekoplus-0.2.0/namekoplus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 05:12:37.000000 namekoplus-0.2.0/namekoplus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-21 05:12:37.000000 namekoplus-0.2.0/namekoplus.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-21 05:12:37.000000 namekoplus-0.2.0/namekoplus.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-21 05:12:37.000000 namekoplus-0.2.0/namekoplus.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 05:12:37.509815 namekoplus-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-07-21 05:12:22.000000 namekoplus-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:44:52.043686 namekoplus-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-21 07:44:35.000000 namekoplus-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-21 07:44:35.000000 namekoplus-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-07-21 07:44:52.043686 namekoplus-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-21 07:44:35.000000 namekoplus-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:44:52.039687 namekoplus-0.2.1/namekoplus/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-21 07:44:35.000000 namekoplus-0.2.1/namekoplus/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:44:52.039687 namekoplus-0.2.1/namekoplus/chassis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 07:44:35.000000 namekoplus-0.2.1/namekoplus/chassis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-21 07:44:35.000000 namekoplus-0.2.1/namekoplus/chassis/chassis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4696 2023-07-21 07:44:35.000000 namekoplus-0.2.1/namekoplus/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:44:52.039687 namekoplus-0.2.1/namekoplus/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 07:44:35.000000 namekoplus-0.2.1/namekoplus/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:44:52.039687 namekoplus-0.2.1/namekoplus/templates/all/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 07:44:35.000000 namekoplus-0.2.1/namekoplus/templates/all/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-07-21 07:44:35.000000 namekoplus-0.2.1/namekoplus/templates/all/all_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-21 07:44:35.000000 namekoplus-0.2.1/namekoplus/templates/all/config.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:44:52.039687 namekoplus-0.2.1/namekoplus/templates/demo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 07:44:35.000000 namekoplus-0.2.1/namekoplus/templates/demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-21 07:44:35.000000 namekoplus-0.2.1/namekoplus/templates/demo/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-07-21 07:44:35.000000 namekoplus-0.2.1/namekoplus/templates/demo/rpc_demo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:44:52.039687 namekoplus-0.2.1/namekoplus/templates/event/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 07:44:35.000000 namekoplus-0.2.1/namekoplus/templates/event/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-21 07:44:35.000000 namekoplus-0.2.1/namekoplus/templates/event/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-07-21 07:44:35.000000 namekoplus-0.2.1/namekoplus/templates/event/events_demo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:44:52.043686 namekoplus-0.2.1/namekoplus/templates/http/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 07:44:35.000000 namekoplus-0.2.1/namekoplus/templates/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-21 07:44:35.000000 namekoplus-0.2.1/namekoplus/templates/http/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-21 07:44:35.000000 namekoplus-0.2.1/namekoplus/templates/http/http_demo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:44:52.043686 namekoplus-0.2.1/namekoplus/templates/rpc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 07:44:35.000000 namekoplus-0.2.1/namekoplus/templates/rpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-21 07:44:35.000000 namekoplus-0.2.1/namekoplus/templates/rpc/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-21 07:44:35.000000 namekoplus-0.2.1/namekoplus/templates/rpc/rpc_demo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:44:52.043686 namekoplus-0.2.1/namekoplus/templates/timer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 07:44:35.000000 namekoplus-0.2.1/namekoplus/templates/timer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-21 07:44:35.000000 namekoplus-0.2.1/namekoplus/templates/timer/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-21 07:44:35.000000 namekoplus-0.2.1/namekoplus/templates/timer/timer_demo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:44:52.039687 namekoplus-0.2.1/namekoplus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-07-21 07:44:52.000000 namekoplus-0.2.1/namekoplus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-21 07:44:52.000000 namekoplus-0.2.1/namekoplus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 07:44:52.000000 namekoplus-0.2.1/namekoplus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-21 07:44:52.000000 namekoplus-0.2.1/namekoplus.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-21 07:44:52.000000 namekoplus-0.2.1/namekoplus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-21 07:44:52.000000 namekoplus-0.2.1/namekoplus.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 07:44:52.043686 namekoplus-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-07-21 07:44:35.000000 namekoplus-0.2.1/setup.py
```

### Comparing `namekoplus-0.2.0/LICENSE` & `namekoplus-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `namekoplus-0.2.0/PKG-INFO` & `namekoplus-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: namekoplus
-Version: 0.2.0
+Version: 0.2.1
 Summary: A lightweight Python distributed microservice solution
 Home-page: 
 Author: Bryant He
 Author-email: bryantsisu@qq.com
 License: MIT
 Project-URL: Documentation, https://doc.bearcatlog.com/
 Project-URL: Source Code, https://github.com/Bryanthelol/namekoplus
```

### Comparing `namekoplus-0.2.0/namekoplus/chassis/chassis.py` & `namekoplus-0.2.1/namekoplus/chassis/chassis.py`

 * *Files identical despite different names*

### Comparing `namekoplus-0.2.0/namekoplus/command.py` & `namekoplus-0.2.1/namekoplus/command.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 @cli.command()
 @click.option('-d', '--directory',
               required=True,
               help='The directory name of nameko services')
 @click.option('-t', '--type', '_type',
               default='all',
               show_default=True,
-              type=click.Choice(['all', 'rpc', 'event', 'http', 'timer'], case_sensitive=False),
+              type=click.Choice(['all', 'rpc', 'event', 'http', 'timer', 'demo'], case_sensitive=False),
               help='The template type of nameko service')
 def init(directory, _type):
     """
     Initialize a new service via templates.
     """
     if os.access(directory, os.F_OK) and os.listdir(directory):
         click.echo('Directory {} already exists and is not empty'.format(directory), err=True)
```

### Comparing `namekoplus-0.2.0/namekoplus/templates/all/all_demo.py` & `namekoplus-0.2.1/namekoplus/templates/all/all_demo.py`

 * *Files identical despite different names*

### Comparing `namekoplus-0.2.0/namekoplus/templates/all/config.yml` & `namekoplus-0.2.1/namekoplus/templates/event/config.yml`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-AMQP_URI: pyamqp://${RABBIT_USER:guest}:${RABBIT_PASSWORD:guest}@${RABBIT_HOST:localhost}:${RABBIT_PORT:5672}/
+AMQP_URI: pyamqp://${RABBIT_USER:admin}:${RABBIT_PASSWORD:admin}@${RABBIT_HOST:localhost}:${RABBIT_PORT:5672}/
 RPC_EXCHANGE: 'nameko-rpc'
 
 max_workers: 10
 parent_calls_tracked: 20
 
 LOGGING:
     version: 1
```

### Comparing `namekoplus-0.2.0/namekoplus/templates/event/config.yml` & `namekoplus-0.2.1/namekoplus/templates/rpc/config.yml`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-AMQP_URI: pyamqp://${RABBIT_USER:guest}:${RABBIT_PASSWORD:guest}@${RABBIT_HOST:localhost}:${RABBIT_PORT:5672}/
+AMQP_URI: pyamqp://${RABBIT_USER:admin}:${RABBIT_PASSWORD:admin}@${RABBIT_HOST:localhost}:${RABBIT_PORT:5672}/
 RPC_EXCHANGE: 'nameko-rpc'
 
 max_workers: 10
 parent_calls_tracked: 20
 
 LOGGING:
     version: 1
```

### Comparing `namekoplus-0.2.0/namekoplus/templates/event/events_demo.py` & `namekoplus-0.2.1/namekoplus/templates/event/events_demo.py`

 * *Files identical despite different names*

### Comparing `namekoplus-0.2.0/namekoplus/templates/http/config.yml` & `namekoplus-0.2.1/namekoplus/templates/timer/config.yml`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-AMQP_URI: pyamqp://${RABBIT_USER:guest}:${RABBIT_PASSWORD:guest}@${RABBIT_HOST:localhost}:${RABBIT_PORT:5672}/
+AMQP_URI: pyamqp://${RABBIT_USER:admin}:${RABBIT_PASSWORD:admin}@${RABBIT_HOST:localhost}:${RABBIT_PORT:5672}/
 RPC_EXCHANGE: 'nameko-rpc'
 
 max_workers: 10
 parent_calls_tracked: 20
 
 LOGGING:
     version: 1
```

### Comparing `namekoplus-0.2.0/namekoplus/templates/http/http_demo.py` & `namekoplus-0.2.1/namekoplus/templates/http/http_demo.py`

 * *Files identical despite different names*

### Comparing `namekoplus-0.2.0/namekoplus/templates/rpc/config.yml` & `namekoplus-0.2.1/namekoplus/templates/all/config.yml`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-AMQP_URI: pyamqp://${RABBIT_USER:guest}:${RABBIT_PASSWORD:guest}@${RABBIT_HOST:localhost}:${RABBIT_PORT:5672}/
+AMQP_URI: pyamqp://${RABBIT_USER:admin}:${RABBIT_PASSWORD:admin}@${RABBIT_HOST:localhost}:${RABBIT_PORT:5672}/
+WEB_SERVER_ADDRESS: '0.0.0.0:8000'
 RPC_EXCHANGE: 'nameko-rpc'
 
 max_workers: 10
 parent_calls_tracked: 20
 
 LOGGING:
     version: 1
```

### Comparing `namekoplus-0.2.0/namekoplus/templates/rpc/rpc_demo.py` & `namekoplus-0.2.1/namekoplus/templates/rpc/rpc_demo.py`

 * *Files identical despite different names*

### Comparing `namekoplus-0.2.0/namekoplus/templates/timer/config.yml` & `namekoplus-0.2.1/namekoplus/templates/http/config.yml`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-AMQP_URI: pyamqp://${RABBIT_USER:guest}:${RABBIT_PASSWORD:guest}@${RABBIT_HOST:localhost}:${RABBIT_PORT:5672}/
+AMQP_URI: pyamqp://${RABBIT_USER:admin}:${RABBIT_PASSWORD:admin}@${RABBIT_HOST:localhost}:${RABBIT_PORT:5672}/
+WEB_SERVER_ADDRESS: '0.0.0.0:8000'
 RPC_EXCHANGE: 'nameko-rpc'
 
 max_workers: 10
 parent_calls_tracked: 20
 
 LOGGING:
     version: 1
```

### Comparing `namekoplus-0.2.0/namekoplus.egg-info/PKG-INFO` & `namekoplus-0.2.1/namekoplus.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: namekoplus
-Version: 0.2.0
+Version: 0.2.1
 Summary: A lightweight Python distributed microservice solution
 Home-page: 
 Author: Bryant He
 Author-email: bryantsisu@qq.com
 License: MIT
 Project-URL: Documentation, https://doc.bearcatlog.com/
 Project-URL: Source Code, https://github.com/Bryanthelol/namekoplus
```

### Comparing `namekoplus-0.2.0/namekoplus.egg-info/SOURCES.txt` & `namekoplus-0.2.1/namekoplus.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,17 @@
 namekoplus.egg-info/top_level.txt
 namekoplus/chassis/__init__.py
 namekoplus/chassis/chassis.py
 namekoplus/templates/__init__.py
 namekoplus/templates/all/__init__.py
 namekoplus/templates/all/all_demo.py
 namekoplus/templates/all/config.yml
+namekoplus/templates/demo/__init__.py
+namekoplus/templates/demo/config.yml
+namekoplus/templates/demo/rpc_demo.py
 namekoplus/templates/event/__init__.py
 namekoplus/templates/event/config.yml
 namekoplus/templates/event/events_demo.py
 namekoplus/templates/http/__init__.py
 namekoplus/templates/http/config.yml
 namekoplus/templates/http/http_demo.py
 namekoplus/templates/rpc/__init__.py
```

### Comparing `namekoplus-0.2.0/setup.py` & `namekoplus-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 here = path.abspath(path.dirname(__file__))
 
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='namekoplus',
-    version='0.2.0',
+    version='0.2.1',
     description='A lightweight Python distributed microservice solution',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='',
     project_urls={
         'Documentation': 'https://doc.bearcatlog.com/',
         'Source Code': 'https://github.com/Bryanthelol/namekoplus',
```

