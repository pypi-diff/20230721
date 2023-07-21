# Comparing `tmp/ox_secrets-0.5.3.tar.gz` & `tmp/ox_secrets-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ox_secrets-0.5.3.tar", last modified: Fri Jul 21 16:40:07 2023, max compression
+gzip compressed data, was "ox_secrets-0.5.4.tar", last modified: Fri Jul 21 19:10:56 2023, max compression
```

## Comparing `ox_secrets-0.5.3.tar` & `ox_secrets-0.5.4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxr-x   0 emin      (1000) emin      (1000)        0 2023-07-21 16:40:07.720995 ox_secrets-0.5.3/
--rw-------   0 emin      (1000) emin      (1000)     1145 2022-03-25 18:04:34.000000 ox_secrets-0.5.3/.gitignore
--rw-------   0 emin      (1000) emin      (1000)     1325 2019-05-25 18:36:31.000000 ox_secrets-0.5.3/LICENSE.txt
--rw-rw-r--   0 emin      (1000) emin      (1000)     7571 2023-07-21 16:40:07.720995 ox_secrets-0.5.3/PKG-INFO
--rw-------   0 emin      (1000) emin      (1000)     5775 2023-07-21 16:11:19.000000 ox_secrets-0.5.3/README.org
--rw-------   0 emin      (1000) emin      (1000)     5811 2023-07-21 16:11:43.000000 ox_secrets-0.5.3/README.rst
--rw-------   0 emin      (1000) emin      (1000)       73 2019-05-25 18:34:28.000000 ox_secrets-0.5.3/conftest.py
--rw-------   0 emin      (1000) emin      (1000)      458 2019-05-25 19:14:14.000000 ox_secrets-0.5.3/makefile
-drwxrwxr-x   0 emin      (1000) emin      (1000)        0 2023-07-21 16:40:07.716995 ox_secrets-0.5.3/ox_secrets/
--rw-rw-r--   0 emin      (1000) emin      (1000)     3290 2023-07-21 16:39:38.000000 ox_secrets-0.5.3/ox_secrets/__init__.py
-drwxrwxr-x   0 emin      (1000) emin      (1000)        0 2023-07-21 16:40:07.720995 ox_secrets-0.5.3/ox_secrets/core/
--rw-------   0 emin      (1000) emin      (1000)       42 2019-05-25 18:42:14.000000 ox_secrets-0.5.3/ox_secrets/core/__init__.py
--rw-rw-r--   0 emin      (1000) emin      (1000)     2374 2023-07-21 15:59:08.000000 ox_secrets-0.5.3/ox_secrets/core/awp.py
--rw-rw-r--   0 emin      (1000) emin      (1000)     5011 2023-07-21 16:37:53.000000 ox_secrets-0.5.3/ox_secrets/core/aws.py
--rw-rw-r--   0 emin      (1000) emin      (1000)    12671 2023-07-21 15:08:03.000000 ox_secrets-0.5.3/ox_secrets/core/common.py
--rw-rw-r--   0 emin      (1000) emin      (1000)     4373 2023-07-20 17:44:57.000000 ox_secrets-0.5.3/ox_secrets/core/evs.py
--rw-rw-r--   0 emin      (1000) emin      (1000)     5630 2023-07-21 16:37:17.000000 ox_secrets-0.5.3/ox_secrets/core/fss.py
--rw-rw-r--   0 emin      (1000) emin      (1000)      719 2023-07-21 15:59:00.000000 ox_secrets-0.5.3/ox_secrets/core/tss.py
--rw-rw-r--   0 emin      (1000) emin      (1000)     4457 2023-07-21 15:58:42.000000 ox_secrets-0.5.3/ox_secrets/server.py
--rw-------   0 emin      (1000) emin      (1000)     1109 2022-03-09 19:18:10.000000 ox_secrets-0.5.3/ox_secrets/settings.py
-drwxrwxr-x   0 emin      (1000) emin      (1000)        0 2023-07-21 16:40:07.720995 ox_secrets-0.5.3/ox_secrets/ui/
--rw-rw-r--   0 emin      (1000) emin      (1000)       48 2023-07-21 16:09:41.000000 ox_secrets-0.5.3/ox_secrets/ui/__init__.py
--rw-rw-r--   0 emin      (1000) emin      (1000)     2101 2023-07-21 16:03:05.000000 ox_secrets-0.5.3/ox_secrets/ui/cli.py
-drwxrwxr-x   0 emin      (1000) emin      (1000)        0 2023-07-21 16:40:07.720995 ox_secrets-0.5.3/ox_secrets.egg-info/
--rw-------   0 emin      (1000) emin      (1000)     7571 2023-07-21 16:40:07.000000 ox_secrets-0.5.3/ox_secrets.egg-info/PKG-INFO
--rw-------   0 emin      (1000) emin      (1000)      580 2023-07-21 16:40:07.000000 ox_secrets-0.5.3/ox_secrets.egg-info/SOURCES.txt
--rw-------   0 emin      (1000) emin      (1000)        1 2023-07-21 16:40:07.000000 ox_secrets-0.5.3/ox_secrets.egg-info/dependency_links.txt
--rw-------   0 emin      (1000) emin      (1000)       55 2023-07-21 16:40:07.000000 ox_secrets-0.5.3/ox_secrets.egg-info/entry_points.txt
--rw-------   0 emin      (1000) emin      (1000)        7 2023-07-21 16:40:07.000000 ox_secrets-0.5.3/ox_secrets.egg-info/requires.txt
--rw-------   0 emin      (1000) emin      (1000)       11 2023-07-21 16:40:07.000000 ox_secrets-0.5.3/ox_secrets.egg-info/top_level.txt
--rw-------   0 emin      (1000) emin      (1000)       14 2019-05-25 18:37:44.000000 ox_secrets-0.5.3/requirements.txt
--rw-rw-r--   0 emin      (1000) emin      (1000)       38 2023-07-21 16:40:07.720995 ox_secrets-0.5.3/setup.cfg
--rw-------   0 emin      (1000) emin      (1000)     1974 2023-07-21 16:01:01.000000 ox_secrets-0.5.3/setup.py
+drwxrwxr-x   0 emin      (1000) emin      (1000)        0 2023-07-21 19:10:56.415452 ox_secrets-0.5.4/
+-rw-------   0 emin      (1000) emin      (1000)     1145 2022-03-25 18:04:34.000000 ox_secrets-0.5.4/.gitignore
+-rw-------   0 emin      (1000) emin      (1000)     1325 2019-05-25 18:36:31.000000 ox_secrets-0.5.4/LICENSE.txt
+-rw-rw-r--   0 emin      (1000) emin      (1000)     7571 2023-07-21 19:10:56.415452 ox_secrets-0.5.4/PKG-INFO
+-rw-------   0 emin      (1000) emin      (1000)     5775 2023-07-21 16:11:19.000000 ox_secrets-0.5.4/README.org
+-rw-------   0 emin      (1000) emin      (1000)     5811 2023-07-21 16:11:43.000000 ox_secrets-0.5.4/README.rst
+-rw-------   0 emin      (1000) emin      (1000)       73 2019-05-25 18:34:28.000000 ox_secrets-0.5.4/conftest.py
+-rw-------   0 emin      (1000) emin      (1000)      458 2019-05-25 19:14:14.000000 ox_secrets-0.5.4/makefile
+drwxrwxr-x   0 emin      (1000) emin      (1000)        0 2023-07-21 19:10:56.415452 ox_secrets-0.5.4/ox_secrets/
+-rw-rw-r--   0 emin      (1000) emin      (1000)     3290 2023-07-21 19:10:25.000000 ox_secrets-0.5.4/ox_secrets/__init__.py
+drwxrwxr-x   0 emin      (1000) emin      (1000)        0 2023-07-21 19:10:56.415452 ox_secrets-0.5.4/ox_secrets/core/
+-rw-------   0 emin      (1000) emin      (1000)       42 2019-05-25 18:42:14.000000 ox_secrets-0.5.4/ox_secrets/core/__init__.py
+-rw-rw-r--   0 emin      (1000) emin      (1000)     2374 2023-07-21 15:59:08.000000 ox_secrets-0.5.4/ox_secrets/core/awp.py
+-rw-rw-r--   0 emin      (1000) emin      (1000)     5011 2023-07-21 16:37:53.000000 ox_secrets-0.5.4/ox_secrets/core/aws.py
+-rw-rw-r--   0 emin      (1000) emin      (1000)    12671 2023-07-21 15:08:03.000000 ox_secrets-0.5.4/ox_secrets/core/common.py
+-rw-rw-r--   0 emin      (1000) emin      (1000)     4373 2023-07-20 17:44:57.000000 ox_secrets-0.5.4/ox_secrets/core/evs.py
+-rw-rw-r--   0 emin      (1000) emin      (1000)     5628 2023-07-21 19:09:54.000000 ox_secrets-0.5.4/ox_secrets/core/fss.py
+-rw-rw-r--   0 emin      (1000) emin      (1000)      719 2023-07-21 15:59:00.000000 ox_secrets-0.5.4/ox_secrets/core/tss.py
+-rw-rw-r--   0 emin      (1000) emin      (1000)     4457 2023-07-21 15:58:42.000000 ox_secrets-0.5.4/ox_secrets/server.py
+-rw-------   0 emin      (1000) emin      (1000)     1109 2022-03-09 19:18:10.000000 ox_secrets-0.5.4/ox_secrets/settings.py
+drwxrwxr-x   0 emin      (1000) emin      (1000)        0 2023-07-21 19:10:56.415452 ox_secrets-0.5.4/ox_secrets/ui/
+-rw-rw-r--   0 emin      (1000) emin      (1000)       48 2023-07-21 16:09:41.000000 ox_secrets-0.5.4/ox_secrets/ui/__init__.py
+-rw-rw-r--   0 emin      (1000) emin      (1000)     2101 2023-07-21 16:03:05.000000 ox_secrets-0.5.4/ox_secrets/ui/cli.py
+drwxrwxr-x   0 emin      (1000) emin      (1000)        0 2023-07-21 19:10:56.415452 ox_secrets-0.5.4/ox_secrets.egg-info/
+-rw-------   0 emin      (1000) emin      (1000)     7571 2023-07-21 19:10:56.000000 ox_secrets-0.5.4/ox_secrets.egg-info/PKG-INFO
+-rw-------   0 emin      (1000) emin      (1000)      580 2023-07-21 19:10:56.000000 ox_secrets-0.5.4/ox_secrets.egg-info/SOURCES.txt
+-rw-------   0 emin      (1000) emin      (1000)        1 2023-07-21 19:10:56.000000 ox_secrets-0.5.4/ox_secrets.egg-info/dependency_links.txt
+-rw-------   0 emin      (1000) emin      (1000)       55 2023-07-21 19:10:56.000000 ox_secrets-0.5.4/ox_secrets.egg-info/entry_points.txt
+-rw-------   0 emin      (1000) emin      (1000)        7 2023-07-21 19:10:56.000000 ox_secrets-0.5.4/ox_secrets.egg-info/requires.txt
+-rw-------   0 emin      (1000) emin      (1000)       11 2023-07-21 19:10:56.000000 ox_secrets-0.5.4/ox_secrets.egg-info/top_level.txt
+-rw-------   0 emin      (1000) emin      (1000)       14 2019-05-25 18:37:44.000000 ox_secrets-0.5.4/requirements.txt
+-rw-rw-r--   0 emin      (1000) emin      (1000)       38 2023-07-21 19:10:56.415452 ox_secrets-0.5.4/setup.cfg
+-rw-------   0 emin      (1000) emin      (1000)     1974 2023-07-21 16:01:01.000000 ox_secrets-0.5.4/setup.py
```

### Comparing `ox_secrets-0.5.3/.gitignore` & `ox_secrets-0.5.4/.gitignore`

 * *Files identical despite different names*

### Comparing `ox_secrets-0.5.3/LICENSE.txt` & `ox_secrets-0.5.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ox_secrets-0.5.3/PKG-INFO` & `ox_secrets-0.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ox_secrets
-Version: 0.5.3
+Version: 0.5.4
 Summary: Simple secret server for python
 Home-page: http://github.com/emin63/ox_secrets
 Author: Emin Martinian
 Author-email: emin.martinian@gmail.com
 License: custom
 Description: Introduction
         ============
```

### Comparing `ox_secrets-0.5.3/README.org` & `ox_secrets-0.5.4/README.org`

 * *Files identical despite different names*

### Comparing `ox_secrets-0.5.3/README.rst` & `ox_secrets-0.5.4/README.rst`

 * *Files identical despite different names*

### Comparing `ox_secrets-0.5.3/ox_secrets/__init__.py` & `ox_secrets-0.5.4/ox_secrets/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,9 +90,9 @@
     oss.get_server(mode='aws').store_secrets(
         {'test_storage':'foobar', category=AWS_PARAM_NAME,
         service_name='ssm')
 
 
 """
 
-VERSION = '0.5.3'
+VERSION = '0.5.4'
 __version__ = VERSION
```

### Comparing `ox_secrets-0.5.3/ox_secrets/core/awp.py` & `ox_secrets-0.5.4/ox_secrets/core/awp.py`

 * *Files identical despite different names*

### Comparing `ox_secrets-0.5.3/ox_secrets/core/aws.py` & `ox_secrets-0.5.4/ox_secrets/core/aws.py`

 * *Files identical despite different names*

### Comparing `ox_secrets-0.5.3/ox_secrets/core/common.py` & `ox_secrets-0.5.4/ox_secrets/core/common.py`

 * *Files identical despite different names*

### Comparing `ox_secrets-0.5.3/ox_secrets/core/evs.py` & `ox_secrets-0.5.4/ox_secrets/core/evs.py`

 * *Files identical despite different names*

### Comparing `ox_secrets-0.5.3/ox_secrets/core/fss.py` & `ox_secrets-0.5.4/ox_secrets/core/fss.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         if filename is None:
             filename = os.environ.get(
                 'OX_SECRETS_FILE', settings.OX_SECRETS_FILE)
         logging.warning('Opening secrets file "%s"', filename)
         with cls._lock, open(filename, 'r', encoding=encoding) as sfd:
             if file_type is None:
                 file_type = os.path.splitext(filename)[-1].lower()
-            elif file_type == '.raw':
+            if file_type == '.raw':
                 contents = [{'name': default_category, 'value': sfd.read()}]
             elif file_type == '.csv':
                 contents = list(csv.DictReader(sfd))
             elif file_type == '.json':
                 contents = [{'name': k, 'value': v}
                             for k, v in json.load(sfd).items()]
             else:
```

### Comparing `ox_secrets-0.5.3/ox_secrets/core/tss.py` & `ox_secrets-0.5.4/ox_secrets/core/tss.py`

 * *Files identical despite different names*

### Comparing `ox_secrets-0.5.3/ox_secrets/server.py` & `ox_secrets-0.5.4/ox_secrets/server.py`

 * *Files identical despite different names*

### Comparing `ox_secrets-0.5.3/ox_secrets/settings.py` & `ox_secrets-0.5.4/ox_secrets/settings.py`

 * *Files identical despite different names*

### Comparing `ox_secrets-0.5.3/ox_secrets/ui/cli.py` & `ox_secrets-0.5.4/ox_secrets/ui/cli.py`

 * *Files identical despite different names*

### Comparing `ox_secrets-0.5.3/ox_secrets.egg-info/PKG-INFO` & `ox_secrets-0.5.4/ox_secrets.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ox-secrets
-Version: 0.5.3
+Version: 0.5.4
 Summary: Simple secret server for python
 Home-page: http://github.com/emin63/ox_secrets
 Author: Emin Martinian
 Author-email: emin.martinian@gmail.com
 License: custom
 Description: Introduction
         ============
```

### Comparing `ox_secrets-0.5.3/ox_secrets.egg-info/SOURCES.txt` & `ox_secrets-0.5.4/ox_secrets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ox_secrets-0.5.3/setup.py` & `ox_secrets-0.5.4/setup.py`

 * *Files identical despite different names*

