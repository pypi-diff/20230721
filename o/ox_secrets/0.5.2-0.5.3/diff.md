# Comparing `tmp/ox_secrets-0.5.2.tar.gz` & `tmp/ox_secrets-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ox_secrets-0.5.2.tar", last modified: Fri Jul 21 16:11:43 2023, max compression
+gzip compressed data, was "ox_secrets-0.5.3.tar", last modified: Fri Jul 21 16:40:07 2023, max compression
```

## Comparing `ox_secrets-0.5.2.tar` & `ox_secrets-0.5.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxr-x   0 emin      (1000) emin      (1000)        0 2023-07-21 16:11:43.848924 ox_secrets-0.5.2/
--rw-------   0 emin      (1000) emin      (1000)     1145 2022-03-25 18:04:34.000000 ox_secrets-0.5.2/.gitignore
--rw-------   0 emin      (1000) emin      (1000)     1325 2019-05-25 18:36:31.000000 ox_secrets-0.5.2/LICENSE.txt
--rw-rw-r--   0 emin      (1000) emin      (1000)     7571 2023-07-21 16:11:43.848924 ox_secrets-0.5.2/PKG-INFO
--rw-------   0 emin      (1000) emin      (1000)     5775 2023-07-21 16:11:19.000000 ox_secrets-0.5.2/README.org
--rw-------   0 emin      (1000) emin      (1000)     5811 2023-07-21 16:11:43.000000 ox_secrets-0.5.2/README.rst
--rw-------   0 emin      (1000) emin      (1000)       73 2019-05-25 18:34:28.000000 ox_secrets-0.5.2/conftest.py
--rw-------   0 emin      (1000) emin      (1000)      458 2019-05-25 19:14:14.000000 ox_secrets-0.5.2/makefile
-drwxrwxr-x   0 emin      (1000) emin      (1000)        0 2023-07-21 16:11:43.848924 ox_secrets-0.5.2/ox_secrets/
--rw-rw-r--   0 emin      (1000) emin      (1000)     3290 2023-07-21 16:04:45.000000 ox_secrets-0.5.2/ox_secrets/__init__.py
-drwxrwxr-x   0 emin      (1000) emin      (1000)        0 2023-07-21 16:11:43.848924 ox_secrets-0.5.2/ox_secrets/core/
--rw-------   0 emin      (1000) emin      (1000)       42 2019-05-25 18:42:14.000000 ox_secrets-0.5.2/ox_secrets/core/__init__.py
--rw-rw-r--   0 emin      (1000) emin      (1000)     2374 2023-07-21 15:59:08.000000 ox_secrets-0.5.2/ox_secrets/core/awp.py
--rw-rw-r--   0 emin      (1000) emin      (1000)     4872 2023-07-20 19:48:50.000000 ox_secrets-0.5.2/ox_secrets/core/aws.py
--rw-rw-r--   0 emin      (1000) emin      (1000)    12671 2023-07-21 15:08:03.000000 ox_secrets-0.5.2/ox_secrets/core/common.py
--rw-rw-r--   0 emin      (1000) emin      (1000)     4373 2023-07-20 17:44:57.000000 ox_secrets-0.5.2/ox_secrets/core/evs.py
--rw-rw-r--   0 emin      (1000) emin      (1000)     5513 2023-07-21 14:58:12.000000 ox_secrets-0.5.2/ox_secrets/core/fss.py
--rw-rw-r--   0 emin      (1000) emin      (1000)      719 2023-07-21 15:59:00.000000 ox_secrets-0.5.2/ox_secrets/core/tss.py
--rw-rw-r--   0 emin      (1000) emin      (1000)     4457 2023-07-21 15:58:42.000000 ox_secrets-0.5.2/ox_secrets/server.py
--rw-------   0 emin      (1000) emin      (1000)     1109 2022-03-09 19:18:10.000000 ox_secrets-0.5.2/ox_secrets/settings.py
-drwxrwxr-x   0 emin      (1000) emin      (1000)        0 2023-07-21 16:11:43.848924 ox_secrets-0.5.2/ox_secrets/ui/
--rw-rw-r--   0 emin      (1000) emin      (1000)       48 2023-07-21 16:09:41.000000 ox_secrets-0.5.2/ox_secrets/ui/__init__.py
--rw-rw-r--   0 emin      (1000) emin      (1000)     2101 2023-07-21 16:03:05.000000 ox_secrets-0.5.2/ox_secrets/ui/cli.py
-drwxrwxr-x   0 emin      (1000) emin      (1000)        0 2023-07-21 16:11:43.848924 ox_secrets-0.5.2/ox_secrets.egg-info/
--rw-------   0 emin      (1000) emin      (1000)     7571 2023-07-21 16:11:43.000000 ox_secrets-0.5.2/ox_secrets.egg-info/PKG-INFO
--rw-------   0 emin      (1000) emin      (1000)      580 2023-07-21 16:11:43.000000 ox_secrets-0.5.2/ox_secrets.egg-info/SOURCES.txt
--rw-------   0 emin      (1000) emin      (1000)        1 2023-07-21 16:11:43.000000 ox_secrets-0.5.2/ox_secrets.egg-info/dependency_links.txt
--rw-------   0 emin      (1000) emin      (1000)       55 2023-07-21 16:11:43.000000 ox_secrets-0.5.2/ox_secrets.egg-info/entry_points.txt
--rw-------   0 emin      (1000) emin      (1000)        7 2023-07-21 16:11:43.000000 ox_secrets-0.5.2/ox_secrets.egg-info/requires.txt
--rw-------   0 emin      (1000) emin      (1000)       11 2023-07-21 16:11:43.000000 ox_secrets-0.5.2/ox_secrets.egg-info/top_level.txt
--rw-------   0 emin      (1000) emin      (1000)       14 2019-05-25 18:37:44.000000 ox_secrets-0.5.2/requirements.txt
--rw-rw-r--   0 emin      (1000) emin      (1000)       38 2023-07-21 16:11:43.848924 ox_secrets-0.5.2/setup.cfg
--rw-------   0 emin      (1000) emin      (1000)     1974 2023-07-21 16:01:01.000000 ox_secrets-0.5.2/setup.py
+drwxrwxr-x   0 emin      (1000) emin      (1000)        0 2023-07-21 16:40:07.720995 ox_secrets-0.5.3/
+-rw-------   0 emin      (1000) emin      (1000)     1145 2022-03-25 18:04:34.000000 ox_secrets-0.5.3/.gitignore
+-rw-------   0 emin      (1000) emin      (1000)     1325 2019-05-25 18:36:31.000000 ox_secrets-0.5.3/LICENSE.txt
+-rw-rw-r--   0 emin      (1000) emin      (1000)     7571 2023-07-21 16:40:07.720995 ox_secrets-0.5.3/PKG-INFO
+-rw-------   0 emin      (1000) emin      (1000)     5775 2023-07-21 16:11:19.000000 ox_secrets-0.5.3/README.org
+-rw-------   0 emin      (1000) emin      (1000)     5811 2023-07-21 16:11:43.000000 ox_secrets-0.5.3/README.rst
+-rw-------   0 emin      (1000) emin      (1000)       73 2019-05-25 18:34:28.000000 ox_secrets-0.5.3/conftest.py
+-rw-------   0 emin      (1000) emin      (1000)      458 2019-05-25 19:14:14.000000 ox_secrets-0.5.3/makefile
+drwxrwxr-x   0 emin      (1000) emin      (1000)        0 2023-07-21 16:40:07.716995 ox_secrets-0.5.3/ox_secrets/
+-rw-rw-r--   0 emin      (1000) emin      (1000)     3290 2023-07-21 16:39:38.000000 ox_secrets-0.5.3/ox_secrets/__init__.py
+drwxrwxr-x   0 emin      (1000) emin      (1000)        0 2023-07-21 16:40:07.720995 ox_secrets-0.5.3/ox_secrets/core/
+-rw-------   0 emin      (1000) emin      (1000)       42 2019-05-25 18:42:14.000000 ox_secrets-0.5.3/ox_secrets/core/__init__.py
+-rw-rw-r--   0 emin      (1000) emin      (1000)     2374 2023-07-21 15:59:08.000000 ox_secrets-0.5.3/ox_secrets/core/awp.py
+-rw-rw-r--   0 emin      (1000) emin      (1000)     5011 2023-07-21 16:37:53.000000 ox_secrets-0.5.3/ox_secrets/core/aws.py
+-rw-rw-r--   0 emin      (1000) emin      (1000)    12671 2023-07-21 15:08:03.000000 ox_secrets-0.5.3/ox_secrets/core/common.py
+-rw-rw-r--   0 emin      (1000) emin      (1000)     4373 2023-07-20 17:44:57.000000 ox_secrets-0.5.3/ox_secrets/core/evs.py
+-rw-rw-r--   0 emin      (1000) emin      (1000)     5630 2023-07-21 16:37:17.000000 ox_secrets-0.5.3/ox_secrets/core/fss.py
+-rw-rw-r--   0 emin      (1000) emin      (1000)      719 2023-07-21 15:59:00.000000 ox_secrets-0.5.3/ox_secrets/core/tss.py
+-rw-rw-r--   0 emin      (1000) emin      (1000)     4457 2023-07-21 15:58:42.000000 ox_secrets-0.5.3/ox_secrets/server.py
+-rw-------   0 emin      (1000) emin      (1000)     1109 2022-03-09 19:18:10.000000 ox_secrets-0.5.3/ox_secrets/settings.py
+drwxrwxr-x   0 emin      (1000) emin      (1000)        0 2023-07-21 16:40:07.720995 ox_secrets-0.5.3/ox_secrets/ui/
+-rw-rw-r--   0 emin      (1000) emin      (1000)       48 2023-07-21 16:09:41.000000 ox_secrets-0.5.3/ox_secrets/ui/__init__.py
+-rw-rw-r--   0 emin      (1000) emin      (1000)     2101 2023-07-21 16:03:05.000000 ox_secrets-0.5.3/ox_secrets/ui/cli.py
+drwxrwxr-x   0 emin      (1000) emin      (1000)        0 2023-07-21 16:40:07.720995 ox_secrets-0.5.3/ox_secrets.egg-info/
+-rw-------   0 emin      (1000) emin      (1000)     7571 2023-07-21 16:40:07.000000 ox_secrets-0.5.3/ox_secrets.egg-info/PKG-INFO
+-rw-------   0 emin      (1000) emin      (1000)      580 2023-07-21 16:40:07.000000 ox_secrets-0.5.3/ox_secrets.egg-info/SOURCES.txt
+-rw-------   0 emin      (1000) emin      (1000)        1 2023-07-21 16:40:07.000000 ox_secrets-0.5.3/ox_secrets.egg-info/dependency_links.txt
+-rw-------   0 emin      (1000) emin      (1000)       55 2023-07-21 16:40:07.000000 ox_secrets-0.5.3/ox_secrets.egg-info/entry_points.txt
+-rw-------   0 emin      (1000) emin      (1000)        7 2023-07-21 16:40:07.000000 ox_secrets-0.5.3/ox_secrets.egg-info/requires.txt
+-rw-------   0 emin      (1000) emin      (1000)       11 2023-07-21 16:40:07.000000 ox_secrets-0.5.3/ox_secrets.egg-info/top_level.txt
+-rw-------   0 emin      (1000) emin      (1000)       14 2019-05-25 18:37:44.000000 ox_secrets-0.5.3/requirements.txt
+-rw-rw-r--   0 emin      (1000) emin      (1000)       38 2023-07-21 16:40:07.720995 ox_secrets-0.5.3/setup.cfg
+-rw-------   0 emin      (1000) emin      (1000)     1974 2023-07-21 16:01:01.000000 ox_secrets-0.5.3/setup.py
```

### Comparing `ox_secrets-0.5.2/.gitignore` & `ox_secrets-0.5.3/.gitignore`

 * *Files identical despite different names*

### Comparing `ox_secrets-0.5.2/LICENSE.txt` & `ox_secrets-0.5.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ox_secrets-0.5.2/PKG-INFO` & `ox_secrets-0.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ox_secrets
-Version: 0.5.2
+Version: 0.5.3
 Summary: Simple secret server for python
 Home-page: http://github.com/emin63/ox_secrets
 Author: Emin Martinian
 Author-email: emin.martinian@gmail.com
 License: custom
 Description: Introduction
         ============
```

### Comparing `ox_secrets-0.5.2/README.org` & `ox_secrets-0.5.3/README.org`

 * *Files identical despite different names*

### Comparing `ox_secrets-0.5.2/README.rst` & `ox_secrets-0.5.3/README.rst`

 * *Files identical despite different names*

### Comparing `ox_secrets-0.5.2/ox_secrets/__init__.py` & `ox_secrets-0.5.3/ox_secrets/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,9 +90,9 @@
     oss.get_server(mode='aws').store_secrets(
         {'test_storage':'foobar', category=AWS_PARAM_NAME,
         service_name='ssm')
 
 
 """
 
-VERSION = '0.5.2'
+VERSION = '0.5.3'
 __version__ = VERSION
```

### Comparing `ox_secrets-0.5.2/ox_secrets/core/awp.py` & `ox_secrets-0.5.3/ox_secrets/core/awp.py`

 * *Files identical despite different names*

### Comparing `ox_secrets-0.5.2/ox_secrets/core/aws.py` & `ox_secrets-0.5.3/ox_secrets/core/aws.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """AWS Secret Manager.
 
 This module provides a secret server using the AWS system.
 """
 
-
+import os
 import logging
 import typing
 import json
 
 
 try:
     import boto3
@@ -27,36 +27,41 @@
 
     @classmethod
     def load_secret_from_aws(
             cls, secret_id: str, profile_name: typing.Optional[
                 str] = None, **kwargs) -> typing.Dict[str, str]:
         """Helper to load given secret_id from AWS.
         """
+        storage = kwargs.pop('storage', os.path.splitext(
+            secret_id)[-1]).lower().lstrip('.')
         if profile_name is None:
             profile_name = settings.OX_SECRETS_AWS_PROFILE_NAME
         logging.warning(
             'Connecting to boto3 for profile %s to read secrets for %s',
             profile_name, secret_id)
         service_name = kwargs.pop('service_name', 'secretsmanager')
         session = boto3.Session(profile_name=profile_name, **kwargs)
         client = session.client(service_name=service_name)
         if service_name == 'secretsmanager':
             get_secret_value_response = client.get_secret_value(
                 SecretId=secret_id)
             secret_data = get_secret_value_response['SecretString']
-            secret_dict = json.loads(secret_data)
         elif service_name == 'ssm':
             get_secret_value_response = client.get_parameter(Name=secret_id)
             secret_data = get_secret_value_response['Parameter']['Value']
-            if secret_id[-5:].lower() == '.json':
-                secret_dict = json.loads(secret_data)
-            else:
-                secret_dict = {secret_id: secret_data}
         else:
             raise ValueError(f'Invalid service_name: {service_name}')
+
+        if storage == 'json':
+            secret_dict = json.loads(secret_data)
+        else:
+            if storage != 'raw':
+                logging.warning('Intpereting unknown storage as raw.')
+            secret_dict = {secret_id: secret_data}
+
         return secret_dict
 
     @classmethod
     def load_cache(cls, name: typing.Optional[str] = None,
                    category: typing.Optional[str] = None,
                    loader_params: typing.Optional[dict] = None):
         """Load secrets and cache them from back-end store.
```

### Comparing `ox_secrets-0.5.2/ox_secrets/core/common.py` & `ox_secrets-0.5.3/ox_secrets/core/common.py`

 * *Files identical despite different names*

### Comparing `ox_secrets-0.5.2/ox_secrets/core/evs.py` & `ox_secrets-0.5.3/ox_secrets/core/evs.py`

 * *Files identical despite different names*

### Comparing `ox_secrets-0.5.2/ox_secrets/core/fss.py` & `ox_secrets-0.5.3/ox_secrets/core/fss.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,17 @@
         if filename is None:
             filename = os.environ.get(
                 'OX_SECRETS_FILE', settings.OX_SECRETS_FILE)
         logging.warning('Opening secrets file "%s"', filename)
         with cls._lock, open(filename, 'r', encoding=encoding) as sfd:
             if file_type is None:
                 file_type = os.path.splitext(filename)[-1].lower()
-            if file_type == '.csv':
+            elif file_type == '.raw':
+                contents = [{'name': default_category, 'value': sfd.read()}]
+            elif file_type == '.csv':
                 contents = list(csv.DictReader(sfd))
             elif file_type == '.json':
                 contents = [{'name': k, 'value': v}
                             for k, v in json.load(sfd).items()]
             else:
                 raise ValueError(f'Cannot handle secrets {file_type=}')
             for line in contents:
```

### Comparing `ox_secrets-0.5.2/ox_secrets/core/tss.py` & `ox_secrets-0.5.3/ox_secrets/core/tss.py`

 * *Files identical despite different names*

### Comparing `ox_secrets-0.5.2/ox_secrets/server.py` & `ox_secrets-0.5.3/ox_secrets/server.py`

 * *Files identical despite different names*

### Comparing `ox_secrets-0.5.2/ox_secrets/settings.py` & `ox_secrets-0.5.3/ox_secrets/settings.py`

 * *Files identical despite different names*

### Comparing `ox_secrets-0.5.2/ox_secrets/ui/cli.py` & `ox_secrets-0.5.3/ox_secrets/ui/cli.py`

 * *Files identical despite different names*

### Comparing `ox_secrets-0.5.2/ox_secrets.egg-info/PKG-INFO` & `ox_secrets-0.5.3/ox_secrets.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ox-secrets
-Version: 0.5.2
+Version: 0.5.3
 Summary: Simple secret server for python
 Home-page: http://github.com/emin63/ox_secrets
 Author: Emin Martinian
 Author-email: emin.martinian@gmail.com
 License: custom
 Description: Introduction
         ============
```

### Comparing `ox_secrets-0.5.2/ox_secrets.egg-info/SOURCES.txt` & `ox_secrets-0.5.3/ox_secrets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ox_secrets-0.5.2/setup.py` & `ox_secrets-0.5.3/setup.py`

 * *Files identical despite different names*

