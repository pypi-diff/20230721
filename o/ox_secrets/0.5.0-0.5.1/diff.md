# Comparing `tmp/ox_secrets-0.5.0.tar.gz` & `tmp/ox_secrets-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ox_secrets-0.5.0.tar", last modified: Fri Jul 21 15:25:35 2023, max compression
+gzip compressed data, was "ox_secrets-0.5.1.tar", last modified: Fri Jul 21 15:28:44 2023, max compression
```

## Comparing `ox_secrets-0.5.0.tar` & `ox_secrets-0.5.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 emin      (1000) emin      (1000)        0 2023-07-21 15:25:35.662726 ox_secrets-0.5.0/
--rw-------   0 emin      (1000) emin      (1000)     1145 2022-03-25 18:04:34.000000 ox_secrets-0.5.0/.gitignore
--rw-------   0 emin      (1000) emin      (1000)     1325 2019-05-25 18:36:31.000000 ox_secrets-0.5.0/LICENSE.txt
--rw-rw-r--   0 emin      (1000) emin      (1000)     6745 2023-07-21 15:25:35.662726 ox_secrets-0.5.0/PKG-INFO
--rw-------   0 emin      (1000) emin      (1000)     5028 2023-07-21 15:22:25.000000 ox_secrets-0.5.0/README.org
--rw-------   0 emin      (1000) emin      (1000)     5169 2023-07-21 15:25:35.000000 ox_secrets-0.5.0/README.rst
--rw-------   0 emin      (1000) emin      (1000)       73 2019-05-25 18:34:28.000000 ox_secrets-0.5.0/conftest.py
--rw-------   0 emin      (1000) emin      (1000)      458 2019-05-25 19:14:14.000000 ox_secrets-0.5.0/makefile
-drwxrwxr-x   0 emin      (1000) emin      (1000)        0 2023-07-21 15:25:35.658726 ox_secrets-0.5.0/ox_secrets/
--rw-rw-r--   0 emin      (1000) emin      (1000)     3290 2023-07-21 15:22:11.000000 ox_secrets-0.5.0/ox_secrets/__init__.py
-drwxrwxr-x   0 emin      (1000) emin      (1000)        0 2023-07-21 15:25:35.662726 ox_secrets-0.5.0/ox_secrets/core/
--rw-------   0 emin      (1000) emin      (1000)       42 2019-05-25 18:42:14.000000 ox_secrets-0.5.0/ox_secrets/core/__init__.py
--rw-rw-r--   0 emin      (1000) emin      (1000)     2392 2022-02-02 03:56:49.000000 ox_secrets-0.5.0/ox_secrets/core/awp.py
--rw-rw-r--   0 emin      (1000) emin      (1000)     4872 2023-07-20 19:48:50.000000 ox_secrets-0.5.0/ox_secrets/core/aws.py
--rw-rw-r--   0 emin      (1000) emin      (1000)    12671 2023-07-21 15:08:03.000000 ox_secrets-0.5.0/ox_secrets/core/common.py
--rw-rw-r--   0 emin      (1000) emin      (1000)     4373 2023-07-20 17:44:57.000000 ox_secrets-0.5.0/ox_secrets/core/evs.py
--rw-rw-r--   0 emin      (1000) emin      (1000)     5513 2023-07-21 14:58:12.000000 ox_secrets-0.5.0/ox_secrets/core/fss.py
--rw-rw-r--   0 emin      (1000) emin      (1000)      738 2022-02-28 17:21:49.000000 ox_secrets-0.5.0/ox_secrets/core/tss.py
--rw-rw-r--   0 emin      (1000) emin      (1000)     4422 2023-07-21 15:10:45.000000 ox_secrets-0.5.0/ox_secrets/server.py
--rw-------   0 emin      (1000) emin      (1000)     1109 2022-03-09 19:18:10.000000 ox_secrets-0.5.0/ox_secrets/settings.py
-drwxrwxr-x   0 emin      (1000) emin      (1000)        0 2023-07-21 15:25:35.658726 ox_secrets-0.5.0/ox_secrets.egg-info/
--rw-------   0 emin      (1000) emin      (1000)     6745 2023-07-21 15:25:35.000000 ox_secrets-0.5.0/ox_secrets.egg-info/PKG-INFO
--rw-------   0 emin      (1000) emin      (1000)      533 2023-07-21 15:25:35.000000 ox_secrets-0.5.0/ox_secrets.egg-info/SOURCES.txt
--rw-------   0 emin      (1000) emin      (1000)        1 2023-07-21 15:25:35.000000 ox_secrets-0.5.0/ox_secrets.egg-info/dependency_links.txt
--rw-------   0 emin      (1000) emin      (1000)       40 2023-07-21 15:25:35.000000 ox_secrets-0.5.0/ox_secrets.egg-info/entry_points.txt
--rw-------   0 emin      (1000) emin      (1000)        7 2023-07-21 15:25:35.000000 ox_secrets-0.5.0/ox_secrets.egg-info/requires.txt
--rw-------   0 emin      (1000) emin      (1000)       11 2023-07-21 15:25:35.000000 ox_secrets-0.5.0/ox_secrets.egg-info/top_level.txt
--rw-------   0 emin      (1000) emin      (1000)       14 2019-05-25 18:37:44.000000 ox_secrets-0.5.0/requirements.txt
--rw-rw-r--   0 emin      (1000) emin      (1000)       38 2023-07-21 15:25:35.662726 ox_secrets-0.5.0/setup.cfg
--rw-------   0 emin      (1000) emin      (1000)     1957 2019-05-25 18:41:30.000000 ox_secrets-0.5.0/setup.py
+drwxrwxr-x   0 emin      (1000) emin      (1000)        0 2023-07-21 15:28:44.492852 ox_secrets-0.5.1/
+-rw-------   0 emin      (1000) emin      (1000)     1145 2022-03-25 18:04:34.000000 ox_secrets-0.5.1/.gitignore
+-rw-------   0 emin      (1000) emin      (1000)     1325 2019-05-25 18:36:31.000000 ox_secrets-0.5.1/LICENSE.txt
+-rw-rw-r--   0 emin      (1000) emin      (1000)     6741 2023-07-21 15:28:44.492852 ox_secrets-0.5.1/PKG-INFO
+-rw-------   0 emin      (1000) emin      (1000)     5047 2023-07-21 15:28:07.000000 ox_secrets-0.5.1/README.org
+-rw-------   0 emin      (1000) emin      (1000)     5165 2023-07-21 15:28:13.000000 ox_secrets-0.5.1/README.rst
+-rw-------   0 emin      (1000) emin      (1000)       73 2019-05-25 18:34:28.000000 ox_secrets-0.5.1/conftest.py
+-rw-------   0 emin      (1000) emin      (1000)      458 2019-05-25 19:14:14.000000 ox_secrets-0.5.1/makefile
+drwxrwxr-x   0 emin      (1000) emin      (1000)        0 2023-07-21 15:28:44.488852 ox_secrets-0.5.1/ox_secrets/
+-rw-rw-r--   0 emin      (1000) emin      (1000)     3290 2023-07-21 15:28:26.000000 ox_secrets-0.5.1/ox_secrets/__init__.py
+drwxrwxr-x   0 emin      (1000) emin      (1000)        0 2023-07-21 15:28:44.492852 ox_secrets-0.5.1/ox_secrets/core/
+-rw-------   0 emin      (1000) emin      (1000)       42 2019-05-25 18:42:14.000000 ox_secrets-0.5.1/ox_secrets/core/__init__.py
+-rw-rw-r--   0 emin      (1000) emin      (1000)     2392 2022-02-02 03:56:49.000000 ox_secrets-0.5.1/ox_secrets/core/awp.py
+-rw-rw-r--   0 emin      (1000) emin      (1000)     4872 2023-07-20 19:48:50.000000 ox_secrets-0.5.1/ox_secrets/core/aws.py
+-rw-rw-r--   0 emin      (1000) emin      (1000)    12671 2023-07-21 15:08:03.000000 ox_secrets-0.5.1/ox_secrets/core/common.py
+-rw-rw-r--   0 emin      (1000) emin      (1000)     4373 2023-07-20 17:44:57.000000 ox_secrets-0.5.1/ox_secrets/core/evs.py
+-rw-rw-r--   0 emin      (1000) emin      (1000)     5513 2023-07-21 14:58:12.000000 ox_secrets-0.5.1/ox_secrets/core/fss.py
+-rw-rw-r--   0 emin      (1000) emin      (1000)      738 2022-02-28 17:21:49.000000 ox_secrets-0.5.1/ox_secrets/core/tss.py
+-rw-rw-r--   0 emin      (1000) emin      (1000)     4422 2023-07-21 15:10:45.000000 ox_secrets-0.5.1/ox_secrets/server.py
+-rw-------   0 emin      (1000) emin      (1000)     1109 2022-03-09 19:18:10.000000 ox_secrets-0.5.1/ox_secrets/settings.py
+drwxrwxr-x   0 emin      (1000) emin      (1000)        0 2023-07-21 15:28:44.488852 ox_secrets-0.5.1/ox_secrets.egg-info/
+-rw-------   0 emin      (1000) emin      (1000)     6741 2023-07-21 15:28:44.000000 ox_secrets-0.5.1/ox_secrets.egg-info/PKG-INFO
+-rw-------   0 emin      (1000) emin      (1000)      533 2023-07-21 15:28:44.000000 ox_secrets-0.5.1/ox_secrets.egg-info/SOURCES.txt
+-rw-------   0 emin      (1000) emin      (1000)        1 2023-07-21 15:28:44.000000 ox_secrets-0.5.1/ox_secrets.egg-info/dependency_links.txt
+-rw-------   0 emin      (1000) emin      (1000)       40 2023-07-21 15:28:44.000000 ox_secrets-0.5.1/ox_secrets.egg-info/entry_points.txt
+-rw-------   0 emin      (1000) emin      (1000)        7 2023-07-21 15:28:44.000000 ox_secrets-0.5.1/ox_secrets.egg-info/requires.txt
+-rw-------   0 emin      (1000) emin      (1000)       11 2023-07-21 15:28:44.000000 ox_secrets-0.5.1/ox_secrets.egg-info/top_level.txt
+-rw-------   0 emin      (1000) emin      (1000)       14 2019-05-25 18:37:44.000000 ox_secrets-0.5.1/requirements.txt
+-rw-rw-r--   0 emin      (1000) emin      (1000)       38 2023-07-21 15:28:44.492852 ox_secrets-0.5.1/setup.cfg
+-rw-------   0 emin      (1000) emin      (1000)     1957 2019-05-25 18:41:30.000000 ox_secrets-0.5.1/setup.py
```

### Comparing `ox_secrets-0.5.0/.gitignore` & `ox_secrets-0.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `ox_secrets-0.5.0/LICENSE.txt` & `ox_secrets-0.5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ox_secrets-0.5.0/PKG-INFO` & `ox_secrets-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ox_secrets
-Version: 0.5.0
+Version: 0.5.1
 Summary: Simple secret server for python
 Home-page: http://github.com/emin63/ox_secrets
 Author: Emin Martinian
 Author-email: emin.martinian@gmail.com
 License: custom
 Description: Introduction
         ============
@@ -53,16 +53,16 @@
         back-ends in case your secrets are split across various places.
         
         Usage
         =====
         
         To get started, you can simply ``pip install ox_secrets`` as usual.
         
-        The ox\ :sub:`secrets` package provides a simple secret server with
-        various back-ends. The following illustrates example usage.
+        The ``ox_secrets`` package provides a simple secret server with various
+        back-ends. The following illustrates example usage.
         
         .. code:: python
         
         
            # First we setup an example secrets file:
         
            >>> import os, tempfile, csv
```

### Comparing `ox_secrets-0.5.0/README.org` & `ox_secrets-0.5.1/README.org`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 
+#+OPTIONS: ^:{}
+
 * Introduction
 
 The =ox_secrets= package provides a simple secret manager for
 python. You can think =ox_secrets= like an ORM for secrets with the
 following goals:
 
 - Simple, light-weight management of secrets.
@@ -38,15 +40,15 @@
 
 To get started, you can simply =pip install ox_secrets= as usual.
 
 #+COMMENT: The following is copied from /ox_secrets/__init__.py docs
 #+COMMENT: At some point we should use noweb or tangling to clean
 #+COMMENT: this up.
 
-The ox_secrets package provides a simple secret server with various
+The =ox_secrets= package provides a simple secret server with various
 back-ends. The following illustrates example usage.
 
 #+BEGIN_SRC python
 
 # First we setup an example secrets file:
 
 >>> import os, tempfile, csv
```

### Comparing `ox_secrets-0.5.0/README.rst` & `ox_secrets-0.5.1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -45,16 +45,16 @@
 back-ends in case your secrets are split across various places.
 
 Usage
 =====
 
 To get started, you can simply ``pip install ox_secrets`` as usual.
 
-The ox\ :sub:`secrets` package provides a simple secret server with
-various back-ends. The following illustrates example usage.
+The ``ox_secrets`` package provides a simple secret server with various
+back-ends. The following illustrates example usage.
 
 .. code:: python
 
 
    # First we setup an example secrets file:
 
    >>> import os, tempfile, csv
```

### Comparing `ox_secrets-0.5.0/ox_secrets/__init__.py` & `ox_secrets-0.5.1/ox_secrets/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,9 +90,9 @@
     oss.get_server(mode='aws').store_secrets(
         {'test_storage':'foobar', category=AWS_PARAM_NAME,
         service_name='ssm')
 
 
 """
 
-VERSION = '0.5.0'
+VERSION = '0.5.1'
 __version__ = VERSION
```

### Comparing `ox_secrets-0.5.0/ox_secrets/core/awp.py` & `ox_secrets-0.5.1/ox_secrets/core/awp.py`

 * *Files identical despite different names*

### Comparing `ox_secrets-0.5.0/ox_secrets/core/aws.py` & `ox_secrets-0.5.1/ox_secrets/core/aws.py`

 * *Files identical despite different names*

### Comparing `ox_secrets-0.5.0/ox_secrets/core/common.py` & `ox_secrets-0.5.1/ox_secrets/core/common.py`

 * *Files identical despite different names*

### Comparing `ox_secrets-0.5.0/ox_secrets/core/evs.py` & `ox_secrets-0.5.1/ox_secrets/core/evs.py`

 * *Files identical despite different names*

### Comparing `ox_secrets-0.5.0/ox_secrets/core/fss.py` & `ox_secrets-0.5.1/ox_secrets/core/fss.py`

 * *Files identical despite different names*

### Comparing `ox_secrets-0.5.0/ox_secrets/core/tss.py` & `ox_secrets-0.5.1/ox_secrets/core/tss.py`

 * *Files identical despite different names*

### Comparing `ox_secrets-0.5.0/ox_secrets/server.py` & `ox_secrets-0.5.1/ox_secrets/server.py`

 * *Files identical despite different names*

### Comparing `ox_secrets-0.5.0/ox_secrets/settings.py` & `ox_secrets-0.5.1/ox_secrets/settings.py`

 * *Files identical despite different names*

### Comparing `ox_secrets-0.5.0/ox_secrets.egg-info/PKG-INFO` & `ox_secrets-0.5.1/ox_secrets.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ox-secrets
-Version: 0.5.0
+Version: 0.5.1
 Summary: Simple secret server for python
 Home-page: http://github.com/emin63/ox_secrets
 Author: Emin Martinian
 Author-email: emin.martinian@gmail.com
 License: custom
 Description: Introduction
         ============
@@ -53,16 +53,16 @@
         back-ends in case your secrets are split across various places.
         
         Usage
         =====
         
         To get started, you can simply ``pip install ox_secrets`` as usual.
         
-        The ox\ :sub:`secrets` package provides a simple secret server with
-        various back-ends. The following illustrates example usage.
+        The ``ox_secrets`` package provides a simple secret server with various
+        back-ends. The following illustrates example usage.
         
         .. code:: python
         
         
            # First we setup an example secrets file:
         
            >>> import os, tempfile, csv
```

### Comparing `ox_secrets-0.5.0/ox_secrets.egg-info/SOURCES.txt` & `ox_secrets-0.5.1/ox_secrets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ox_secrets-0.5.0/setup.py` & `ox_secrets-0.5.1/setup.py`

 * *Files identical despite different names*

