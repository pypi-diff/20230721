# Comparing `tmp/bitbucket-pipes-toolkit-3.3.1.tar.gz` & `tmp/bitbucket-pipes-toolkit-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bitbucket-pipes-toolkit-3.3.1.tar", last modified: Thu Jul  6 10:48:34 2023, max compression
+gzip compressed data, was "bitbucket-pipes-toolkit-4.0.0.tar", last modified: Fri Jul 21 07:00:55 2023, max compression
```

## Comparing `bitbucket-pipes-toolkit-3.3.1.tar` & `bitbucket-pipes-toolkit-4.0.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 10:48:34.000000 bitbucket-pipes-toolkit-3.3.1/
--rw-r--r--   0 root         (0) root         (0)     1973 2023-07-06 10:48:34.000000 bitbucket-pipes-toolkit-3.3.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1198 2023-07-06 10:48:20.000000 bitbucket-pipes-toolkit-3.3.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 10:48:34.000000 bitbucket-pipes-toolkit-3.3.1/bitbucket_pipes_toolkit/
--rw-rw-rw-   0 root         (0) root         (0)      300 2023-07-06 10:48:20.000000 bitbucket-pipes-toolkit-3.3.1/bitbucket_pipes_toolkit/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6851 2023-07-06 10:48:20.000000 bitbucket-pipes-toolkit-3.3.1/bitbucket_pipes_toolkit/annotations.py
--rw-rw-rw-   0 root         (0) root         (0)    14341 2023-07-06 10:48:20.000000 bitbucket-pipes-toolkit-3.3.1/bitbucket_pipes_toolkit/core.py
--rw-rw-rw-   0 root         (0) root         (0)     5811 2023-07-06 10:48:20.000000 bitbucket-pipes-toolkit-3.3.1/bitbucket_pipes_toolkit/helpers.py
--rw-rw-rw-   0 root         (0) root         (0)     3106 2023-07-06 10:48:20.000000 bitbucket-pipes-toolkit-3.3.1/bitbucket_pipes_toolkit/test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 10:48:34.000000 bitbucket-pipes-toolkit-3.3.1/bitbucket_pipes_toolkit.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1973 2023-07-06 10:48:34.000000 bitbucket-pipes-toolkit-3.3.1/bitbucket_pipes_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      426 2023-07-06 10:48:34.000000 bitbucket-pipes-toolkit-3.3.1/bitbucket_pipes_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 10:48:34.000000 bitbucket-pipes-toolkit-3.3.1/bitbucket_pipes_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      105 2023-07-06 10:48:34.000000 bitbucket-pipes-toolkit-3.3.1/bitbucket_pipes_toolkit.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       24 2023-07-06 10:48:34.000000 bitbucket-pipes-toolkit-3.3.1/bitbucket_pipes_toolkit.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-06 10:48:34.000000 bitbucket-pipes-toolkit-3.3.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      742 2023-07-06 10:48:20.000000 bitbucket-pipes-toolkit-3.3.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 07:00:55.307543 bitbucket-pipes-toolkit-4.0.0/
+-rw-r--r--   0 root         (0) root         (0)     1535 2023-07-21 07:00:55.307543 bitbucket-pipes-toolkit-4.0.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1199 2023-07-21 07:00:40.000000 bitbucket-pipes-toolkit-4.0.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 07:00:55.307543 bitbucket-pipes-toolkit-4.0.0/bitbucket_pipes_toolkit/
+-rw-rw-rw-   0 root         (0) root         (0)      300 2023-07-21 07:00:40.000000 bitbucket-pipes-toolkit-4.0.0/bitbucket_pipes_toolkit/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6851 2023-07-21 07:00:40.000000 bitbucket-pipes-toolkit-4.0.0/bitbucket_pipes_toolkit/annotations.py
+-rw-rw-rw-   0 root         (0) root         (0)    14341 2023-07-21 07:00:40.000000 bitbucket-pipes-toolkit-4.0.0/bitbucket_pipes_toolkit/core.py
+-rw-rw-rw-   0 root         (0) root         (0)     5811 2023-07-21 07:00:40.000000 bitbucket-pipes-toolkit-4.0.0/bitbucket_pipes_toolkit/helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)     3106 2023-07-21 07:00:40.000000 bitbucket-pipes-toolkit-4.0.0/bitbucket_pipes_toolkit/test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 07:00:55.307543 bitbucket-pipes-toolkit-4.0.0/bitbucket_pipes_toolkit.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1535 2023-07-21 07:00:55.000000 bitbucket-pipes-toolkit-4.0.0/bitbucket_pipes_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      426 2023-07-21 07:00:55.000000 bitbucket-pipes-toolkit-4.0.0/bitbucket_pipes_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 07:00:55.000000 bitbucket-pipes-toolkit-4.0.0/bitbucket_pipes_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       98 2023-07-21 07:00:55.000000 bitbucket-pipes-toolkit-4.0.0/bitbucket_pipes_toolkit.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2023-07-21 07:00:55.000000 bitbucket-pipes-toolkit-4.0.0/bitbucket_pipes_toolkit.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-21 07:00:55.307543 bitbucket-pipes-toolkit-4.0.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      735 2023-07-21 07:00:40.000000 bitbucket-pipes-toolkit-4.0.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `bitbucket-pipes-toolkit-3.3.1/PKG-INFO` & `bitbucket-pipes-toolkit-4.0.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,60 +1,59 @@
 Metadata-Version: 2.1
 Name: bitbucket-pipes-toolkit
-Version: 3.3.1
+Version: 4.0.0
 Summary: This package contains various helpers for developing bitbucket pipelines pipes
 Home-page: https://bitbucket.org/bitbucketpipelines/bitbucket-pipes-toolkit
 Author: Atlassian
 Author-email: bitbucketci-team@atlassian.com
-License: UNKNOWN
-Description: Bitbucket Pipes Toolkit
-        =========
-        
-        ![Coverage](https://bitbucket.org/bitbucketpipelines/bitbucket-pipes-toolkit/downloads/coverage.svg)
-        
-        This package contains various tools and helpers to make it more fun and easy for people to develope pipes. This includes improved colorized logging, shared data interface, array variables helpers and more.
-        
-        Installation
-        ============
-        
-        `pip install bitbucket_pipes_toolkit`
-        
-        
-        Examples
-        ========
-        
-        Simple pipe example
-        ```python3
-        import os
-        
-        from bitbucket_pipes_toolkit import Pipe
-        
-        
-        class MyPipe(Pipe):
-            def run(self):
-                super().run()
-                print("I'm a simple little pipe")
-        
-        
-        # below is a simple schema for pipe variables.
-        schema = {'USERNAME': {'required': True, 'type': 'string'},
-                  'PASSWORD': {'required': True, 'type': 'string'}}
-        
-        pipe_metadata = {
-            'name': 'My Pipe',
-            'image': 'mydockerimage:latest'
-        }
-        
-        # Set environment variables required in schema.
-        os.environ['USERNAME'] = 'user'
-        os.environ['PASSWORD'] = 'pwd'
-        
-        my_pipe = MyPipe(pipe_metadata=pipe_metadata, schema=schema)
-        my_pipe.run()
-        ```
-        
-        Documentation
-        =============
-        
-        For more details have a look at the [official documentation](https://bitbucket-pipes-toolkit.readthedocs.io).
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+
+Bitbucket Pipes Toolkit
+=========
+
+![Coverage](https://bitbucket.org/bitbucketpipelines/bitbucket-pipes-toolkit/downloads/coverage.svg)
+
+This package contains various tools and helpers to make it more fun and easy for people to develop pipes. This includes improved colorized logging, shared data interface, array variables helpers and more.
+
+Installation
+============
+
+`pip install bitbucket_pipes_toolkit`
+
+
+Examples
+========
+
+Simple pipe example
+```python3
+import os
+
+from bitbucket_pipes_toolkit import Pipe
+
+
+class MyPipe(Pipe):
+    def run(self):
+        super().run()
+        print("I'm a simple little pipe")
+
+
+# below is a simple schema for pipe variables.
+schema = {'USERNAME': {'required': True, 'type': 'string'},
+          'PASSWORD': {'required': True, 'type': 'string'}}
+
+pipe_metadata = {
+    'name': 'My Pipe',
+    'image': 'my-docker-image:latest'
+}
+
+# Set environment variables required in schema.
+os.environ['USERNAME'] = 'user'
+os.environ['PASSWORD'] = 'pwd'
+
+my_pipe = MyPipe(pipe_metadata=pipe_metadata, schema=schema)
+my_pipe.run()
+```
+
+Documentation
+=============
+
+For more details have a look at the [official documentation](https://bitbucket-pipes-toolkit.readthedocs.io).
```

### Comparing `bitbucket-pipes-toolkit-3.3.1/README.md` & `bitbucket-pipes-toolkit-4.0.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Bitbucket Pipes Toolkit
 =========
 
 ![Coverage](https://bitbucket.org/bitbucketpipelines/bitbucket-pipes-toolkit/downloads/coverage.svg)
 
-This package contains various tools and helpers to make it more fun and easy for people to develope pipes. This includes improved colorized logging, shared data interface, array variables helpers and more.
+This package contains various tools and helpers to make it more fun and easy for people to develop pipes. This includes improved colorized logging, shared data interface, array variables helpers and more.
 
 Installation
 ============
 
 `pip install bitbucket_pipes_toolkit`
 
 
@@ -29,15 +29,15 @@
 
 # below is a simple schema for pipe variables.
 schema = {'USERNAME': {'required': True, 'type': 'string'},
           'PASSWORD': {'required': True, 'type': 'string'}}
 
 pipe_metadata = {
     'name': 'My Pipe',
-    'image': 'mydockerimage:latest'
+    'image': 'my-docker-image:latest'
 }
 
 # Set environment variables required in schema.
 os.environ['USERNAME'] = 'user'
 os.environ['PASSWORD'] = 'pwd'
 
 my_pipe = MyPipe(pipe_metadata=pipe_metadata, schema=schema)
```

### Comparing `bitbucket-pipes-toolkit-3.3.1/bitbucket_pipes_toolkit/annotations.py` & `bitbucket-pipes-toolkit-4.0.0/bitbucket_pipes_toolkit/annotations.py`

 * *Files identical despite different names*

### Comparing `bitbucket-pipes-toolkit-3.3.1/bitbucket_pipes_toolkit/core.py` & `bitbucket-pipes-toolkit-4.0.0/bitbucket_pipes_toolkit/core.py`

 * *Files identical despite different names*

### Comparing `bitbucket-pipes-toolkit-3.3.1/bitbucket_pipes_toolkit/helpers.py` & `bitbucket-pipes-toolkit-4.0.0/bitbucket_pipes_toolkit/helpers.py`

 * *Files identical despite different names*

### Comparing `bitbucket-pipes-toolkit-3.3.1/bitbucket_pipes_toolkit/test.py` & `bitbucket-pipes-toolkit-4.0.0/bitbucket_pipes_toolkit/test.py`

 * *Files identical despite different names*

### Comparing `bitbucket-pipes-toolkit-3.3.1/bitbucket_pipes_toolkit.egg-info/PKG-INFO` & `bitbucket-pipes-toolkit-4.0.0/bitbucket_pipes_toolkit.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,60 +1,59 @@
 Metadata-Version: 2.1
 Name: bitbucket-pipes-toolkit
-Version: 3.3.1
+Version: 4.0.0
 Summary: This package contains various helpers for developing bitbucket pipelines pipes
 Home-page: https://bitbucket.org/bitbucketpipelines/bitbucket-pipes-toolkit
 Author: Atlassian
 Author-email: bitbucketci-team@atlassian.com
-License: UNKNOWN
-Description: Bitbucket Pipes Toolkit
-        =========
-        
-        ![Coverage](https://bitbucket.org/bitbucketpipelines/bitbucket-pipes-toolkit/downloads/coverage.svg)
-        
-        This package contains various tools and helpers to make it more fun and easy for people to develope pipes. This includes improved colorized logging, shared data interface, array variables helpers and more.
-        
-        Installation
-        ============
-        
-        `pip install bitbucket_pipes_toolkit`
-        
-        
-        Examples
-        ========
-        
-        Simple pipe example
-        ```python3
-        import os
-        
-        from bitbucket_pipes_toolkit import Pipe
-        
-        
-        class MyPipe(Pipe):
-            def run(self):
-                super().run()
-                print("I'm a simple little pipe")
-        
-        
-        # below is a simple schema for pipe variables.
-        schema = {'USERNAME': {'required': True, 'type': 'string'},
-                  'PASSWORD': {'required': True, 'type': 'string'}}
-        
-        pipe_metadata = {
-            'name': 'My Pipe',
-            'image': 'mydockerimage:latest'
-        }
-        
-        # Set environment variables required in schema.
-        os.environ['USERNAME'] = 'user'
-        os.environ['PASSWORD'] = 'pwd'
-        
-        my_pipe = MyPipe(pipe_metadata=pipe_metadata, schema=schema)
-        my_pipe.run()
-        ```
-        
-        Documentation
-        =============
-        
-        For more details have a look at the [official documentation](https://bitbucket-pipes-toolkit.readthedocs.io).
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+
+Bitbucket Pipes Toolkit
+=========
+
+![Coverage](https://bitbucket.org/bitbucketpipelines/bitbucket-pipes-toolkit/downloads/coverage.svg)
+
+This package contains various tools and helpers to make it more fun and easy for people to develop pipes. This includes improved colorized logging, shared data interface, array variables helpers and more.
+
+Installation
+============
+
+`pip install bitbucket_pipes_toolkit`
+
+
+Examples
+========
+
+Simple pipe example
+```python3
+import os
+
+from bitbucket_pipes_toolkit import Pipe
+
+
+class MyPipe(Pipe):
+    def run(self):
+        super().run()
+        print("I'm a simple little pipe")
+
+
+# below is a simple schema for pipe variables.
+schema = {'USERNAME': {'required': True, 'type': 'string'},
+          'PASSWORD': {'required': True, 'type': 'string'}}
+
+pipe_metadata = {
+    'name': 'My Pipe',
+    'image': 'my-docker-image:latest'
+}
+
+# Set environment variables required in schema.
+os.environ['USERNAME'] = 'user'
+os.environ['PASSWORD'] = 'pwd'
+
+my_pipe = MyPipe(pipe_metadata=pipe_metadata, schema=schema)
+my_pipe.run()
+```
+
+Documentation
+=============
+
+For more details have a look at the [official documentation](https://bitbucket-pipes-toolkit.readthedocs.io).
```

### Comparing `bitbucket-pipes-toolkit-3.3.1/setup.py` & `bitbucket-pipes-toolkit-4.0.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup
 
 setup(
     name='bitbucket-pipes-toolkit',
-    version='3.3.1',
+    version='4.0.0',
     packages=['bitbucket_pipes_toolkit', ],
     url='https://bitbucket.org/bitbucketpipelines/bitbucket-pipes-toolkit',
     author='Atlassian',
     author_email='bitbucketci-team@atlassian.com',
     description='This package contains various helpers for developing bitbucket pipelines pipes',
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     install_requires=['colorama>=0.4.3',
                       'colorlog>=4.0,<7.0',
-                      'pyyaml>=5.4',
-                      'Cerberus>=1.2,<2.0',
-                      'docker[tls]>=4.2,<5.0.0',
-                      'GitPython==3.*']
+                      'PyYAML>=6.0',
+                      'Cerberus>=1.3,<2.0',
+                      'docker>=6.1.3',
+                      'GitPython>=3.1.32']
 )
```

