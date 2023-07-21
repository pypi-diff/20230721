# Comparing `tmp/namekoplus-0.1.2.tar.gz` & `tmp/namekoplus-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "namekoplus-0.1.2.tar", last modified: Thu Jul 20 05:16:28 2023, max compression
+gzip compressed data, was "namekoplus-0.2.0.tar", last modified: Fri Jul 21 05:12:37 2023, max compression
```

## Comparing `namekoplus-0.1.2.tar` & `namekoplus-0.2.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 05:16:28.947717 namekoplus-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-20 05:16:12.000000 namekoplus-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-20 05:16:12.000000 namekoplus-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-07-20 05:16:28.947717 namekoplus-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-20 05:16:12.000000 namekoplus-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 05:16:28.943717 namekoplus-0.1.2/namekoplus/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-20 05:16:12.000000 namekoplus-0.1.2/namekoplus/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 05:16:28.943717 namekoplus-0.1.2/namekoplus/chassis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 05:16:12.000000 namekoplus-0.1.2/namekoplus/chassis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-20 05:16:12.000000 namekoplus-0.1.2/namekoplus/chassis/chassis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-07-20 05:16:12.000000 namekoplus-0.1.2/namekoplus/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 05:16:28.943717 namekoplus-0.1.2/namekoplus/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 05:16:12.000000 namekoplus-0.1.2/namekoplus/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 05:16:28.943717 namekoplus-0.1.2/namekoplus/templates/all/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 05:16:12.000000 namekoplus-0.1.2/namekoplus/templates/all/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-07-20 05:16:12.000000 namekoplus-0.1.2/namekoplus/templates/all/all_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-20 05:16:12.000000 namekoplus-0.1.2/namekoplus/templates/all/config.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 05:16:28.943717 namekoplus-0.1.2/namekoplus/templates/event/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 05:16:12.000000 namekoplus-0.1.2/namekoplus/templates/event/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-20 05:16:12.000000 namekoplus-0.1.2/namekoplus/templates/event/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-07-20 05:16:12.000000 namekoplus-0.1.2/namekoplus/templates/event/events_demo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 05:16:28.947717 namekoplus-0.1.2/namekoplus/templates/http/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 05:16:12.000000 namekoplus-0.1.2/namekoplus/templates/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-20 05:16:12.000000 namekoplus-0.1.2/namekoplus/templates/http/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-20 05:16:12.000000 namekoplus-0.1.2/namekoplus/templates/http/http_demo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 05:16:28.947717 namekoplus-0.1.2/namekoplus/templates/rpc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 05:16:12.000000 namekoplus-0.1.2/namekoplus/templates/rpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-20 05:16:12.000000 namekoplus-0.1.2/namekoplus/templates/rpc/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-20 05:16:12.000000 namekoplus-0.1.2/namekoplus/templates/rpc/rpc_demo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 05:16:28.947717 namekoplus-0.1.2/namekoplus/templates/timer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 05:16:12.000000 namekoplus-0.1.2/namekoplus/templates/timer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-20 05:16:12.000000 namekoplus-0.1.2/namekoplus/templates/timer/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-20 05:16:12.000000 namekoplus-0.1.2/namekoplus/templates/timer/timer_demo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 05:16:28.943717 namekoplus-0.1.2/namekoplus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-07-20 05:16:28.000000 namekoplus-0.1.2/namekoplus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-07-20 05:16:28.000000 namekoplus-0.1.2/namekoplus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 05:16:28.000000 namekoplus-0.1.2/namekoplus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-20 05:16:28.000000 namekoplus-0.1.2/namekoplus.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-20 05:16:28.000000 namekoplus-0.1.2/namekoplus.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-20 05:16:28.000000 namekoplus-0.1.2/namekoplus.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 05:16:28.947717 namekoplus-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-07-20 05:16:12.000000 namekoplus-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:12:37.509815 namekoplus-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-21 05:12:22.000000 namekoplus-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-21 05:12:22.000000 namekoplus-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-07-21 05:12:37.509815 namekoplus-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-21 05:12:22.000000 namekoplus-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:12:37.509815 namekoplus-0.2.0/namekoplus/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-21 05:12:22.000000 namekoplus-0.2.0/namekoplus/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:12:37.509815 namekoplus-0.2.0/namekoplus/chassis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 05:12:22.000000 namekoplus-0.2.0/namekoplus/chassis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-21 05:12:22.000000 namekoplus-0.2.0/namekoplus/chassis/chassis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4688 2023-07-21 05:12:22.000000 namekoplus-0.2.0/namekoplus/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:12:37.509815 namekoplus-0.2.0/namekoplus/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 05:12:22.000000 namekoplus-0.2.0/namekoplus/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:12:37.509815 namekoplus-0.2.0/namekoplus/templates/all/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 05:12:22.000000 namekoplus-0.2.0/namekoplus/templates/all/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-07-21 05:12:22.000000 namekoplus-0.2.0/namekoplus/templates/all/all_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-21 05:12:22.000000 namekoplus-0.2.0/namekoplus/templates/all/config.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:12:37.509815 namekoplus-0.2.0/namekoplus/templates/event/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 05:12:22.000000 namekoplus-0.2.0/namekoplus/templates/event/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-21 05:12:22.000000 namekoplus-0.2.0/namekoplus/templates/event/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-07-21 05:12:22.000000 namekoplus-0.2.0/namekoplus/templates/event/events_demo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:12:37.509815 namekoplus-0.2.0/namekoplus/templates/http/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 05:12:22.000000 namekoplus-0.2.0/namekoplus/templates/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-21 05:12:22.000000 namekoplus-0.2.0/namekoplus/templates/http/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-21 05:12:22.000000 namekoplus-0.2.0/namekoplus/templates/http/http_demo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:12:37.509815 namekoplus-0.2.0/namekoplus/templates/rpc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 05:12:22.000000 namekoplus-0.2.0/namekoplus/templates/rpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-21 05:12:22.000000 namekoplus-0.2.0/namekoplus/templates/rpc/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-21 05:12:22.000000 namekoplus-0.2.0/namekoplus/templates/rpc/rpc_demo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:12:37.509815 namekoplus-0.2.0/namekoplus/templates/timer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 05:12:22.000000 namekoplus-0.2.0/namekoplus/templates/timer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-21 05:12:22.000000 namekoplus-0.2.0/namekoplus/templates/timer/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-21 05:12:22.000000 namekoplus-0.2.0/namekoplus/templates/timer/timer_demo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:12:37.509815 namekoplus-0.2.0/namekoplus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-07-21 05:12:37.000000 namekoplus-0.2.0/namekoplus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-07-21 05:12:37.000000 namekoplus-0.2.0/namekoplus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 05:12:37.000000 namekoplus-0.2.0/namekoplus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-21 05:12:37.000000 namekoplus-0.2.0/namekoplus.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-21 05:12:37.000000 namekoplus-0.2.0/namekoplus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-21 05:12:37.000000 namekoplus-0.2.0/namekoplus.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 05:12:37.509815 namekoplus-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-07-21 05:12:22.000000 namekoplus-0.2.0/setup.py
```

### Comparing `namekoplus-0.1.2/LICENSE` & `namekoplus-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `namekoplus-0.1.2/PKG-INFO` & `namekoplus-0.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 Metadata-Version: 2.1
 Name: namekoplus
-Version: 0.1.2
+Version: 0.2.0
 Summary: A lightweight Python distributed microservice solution
-Home-page: https://github.com/Bryanthelol/namekoplus
+Home-page: 
 Author: Bryant He
 Author-email: bryantsisu@qq.com
 License: MIT
+Project-URL: Documentation, https://doc.bearcatlog.com/
+Project-URL: Source Code, https://github.com/Bryanthelol/namekoplus
+Project-URL: Bug Tracker, https://github.com/Bryanthelol/namekoplus/issues
 Keywords: lightweight python distributed microservice solution
 Platform: any
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3
 Description-Content-Type: text/markdown
+Provides-Extra: ha
 Provides-Extra: apiflask
 Provides-Extra: rocketry
 Provides-Extra: gutter
 Provides-Extra: mysql
+Provides-Extra: ssl
 Provides-Extra: dev
 License-File: LICENSE
 
 # namekoplus
 
 A lightweight Python distributed microservice solution
```

### Comparing `namekoplus-0.1.2/namekoplus/chassis/chassis.py` & `namekoplus-0.2.0/namekoplus/chassis/chassis.py`

 * *Files identical despite different names*

### Comparing `namekoplus-0.1.2/namekoplus/templates/all/all_demo.py` & `namekoplus-0.2.0/namekoplus/templates/all/all_demo.py`

 * *Files identical despite different names*

### Comparing `namekoplus-0.1.2/namekoplus/templates/all/config.yml` & `namekoplus-0.2.0/namekoplus/templates/all/config.yml`

 * *Files identical despite different names*

### Comparing `namekoplus-0.1.2/namekoplus/templates/event/config.yml` & `namekoplus-0.2.0/namekoplus/templates/event/config.yml`

 * *Files identical despite different names*

### Comparing `namekoplus-0.1.2/namekoplus/templates/event/events_demo.py` & `namekoplus-0.2.0/namekoplus/templates/event/events_demo.py`

 * *Files identical despite different names*

### Comparing `namekoplus-0.1.2/namekoplus/templates/http/config.yml` & `namekoplus-0.2.0/namekoplus/templates/http/config.yml`

 * *Files identical despite different names*

### Comparing `namekoplus-0.1.2/namekoplus/templates/http/http_demo.py` & `namekoplus-0.2.0/namekoplus/templates/http/http_demo.py`

 * *Files identical despite different names*

### Comparing `namekoplus-0.1.2/namekoplus/templates/rpc/config.yml` & `namekoplus-0.2.0/namekoplus/templates/rpc/config.yml`

 * *Files identical despite different names*

### Comparing `namekoplus-0.1.2/namekoplus/templates/rpc/rpc_demo.py` & `namekoplus-0.2.0/namekoplus/templates/rpc/rpc_demo.py`

 * *Files identical despite different names*

### Comparing `namekoplus-0.1.2/namekoplus/templates/timer/config.yml` & `namekoplus-0.2.0/namekoplus/templates/timer/config.yml`

 * *Files identical despite different names*

### Comparing `namekoplus-0.1.2/namekoplus.egg-info/PKG-INFO` & `namekoplus-0.2.0/namekoplus.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 Metadata-Version: 2.1
 Name: namekoplus
-Version: 0.1.2
+Version: 0.2.0
 Summary: A lightweight Python distributed microservice solution
-Home-page: https://github.com/Bryanthelol/namekoplus
+Home-page: 
 Author: Bryant He
 Author-email: bryantsisu@qq.com
 License: MIT
+Project-URL: Documentation, https://doc.bearcatlog.com/
+Project-URL: Source Code, https://github.com/Bryanthelol/namekoplus
+Project-URL: Bug Tracker, https://github.com/Bryanthelol/namekoplus/issues
 Keywords: lightweight python distributed microservice solution
 Platform: any
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3
 Description-Content-Type: text/markdown
+Provides-Extra: ha
 Provides-Extra: apiflask
 Provides-Extra: rocketry
 Provides-Extra: gutter
 Provides-Extra: mysql
+Provides-Extra: ssl
 Provides-Extra: dev
 License-File: LICENSE
 
 # namekoplus
 
 A lightweight Python distributed microservice solution
```

### Comparing `namekoplus-0.1.2/namekoplus.egg-info/SOURCES.txt` & `namekoplus-0.2.0/namekoplus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `namekoplus-0.1.2/setup.py` & `namekoplus-0.2.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,20 +5,24 @@
 here = path.abspath(path.dirname(__file__))
 
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='namekoplus',
-    version='0.1.2',
+    version='0.2.0',
     description='A lightweight Python distributed microservice solution',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    url='https://github.com/Bryanthelol/namekoplus',
-
+    url='',
+    project_urls={
+        'Documentation': 'https://doc.bearcatlog.com/',
+        'Source Code': 'https://github.com/Bryanthelol/namekoplus',
+        'Bug Tracker': 'https://github.com/Bryanthelol/namekoplus/issues',
+    },
     author='Bryant He',
     author_email='bryantsisu@qq.com',
 
     license='MIT',
 
     classifiers=[
         'Development Status :: 3 - Alpha',
@@ -41,33 +45,34 @@
         'console_scripts': [
             'namekoplus = namekoplus.command:cli',
         ],
     },
 
     install_requires=[
         'nameko==3.0.0rc11',
-        'nameko-sentry==1.0.0',
-        'nameko-tracer==1.4.0',
         'click==8.1.5',
-        'pytest==7.4.0',
-        'environs==9.5.0',
-        'logstash_formatter==0.5.17',
-        'statsd==4.0.1',
-        'tenacity==8.2.2',
-        'cachetools==5.3.0',
-        'circuitbreaker==2.0.0',
-        'shortuuid==1.0.11',
-        'cryptography'
+        'python-on-whales==0.62.0',
+        'pytest==7.4.0'
     ],
     extras_require={
+        'ha': ['tenacity==8.2.2',
+               'cachetools==5.3.0',
+               'circuitbreaker==2.0.0',
+               'statsd==4.0.1',
+               'logstash_formatter==0.5.17',
+               'nameko-sentry==1.0.0',
+               'nameko-tracer==1.4.0',
+               'shortuuid==1.0.11'],
         'apiflask': ['apiflask>=1.3.1',
                      'gevent>=22.10.2',
                      'gunicorn==20.1.0'],
         'rocketry': ['rocketry==2.4.0'],
         'gutter': ['gutter==0.5.0'],
         'mysql': ['pymysql==1.0.3',
                   'sqlalchemy==2.0.15',
                   'sqlacodegen==2.3.0',
                   'alembic==1.11.1'],
-        'dev': ['mako==1.2.4'],
+        'ssl': ['cryptography'],
+        'dev': ['mako==1.2.4',
+                'environs==9.5.0']
     },
 )
```

