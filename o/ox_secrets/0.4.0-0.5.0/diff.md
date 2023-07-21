# Comparing `tmp/ox_secrets-0.4.0.tar.gz` & `tmp/ox_secrets-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ox_secrets-0.4.0.tar", last modified: Wed Sep  7 16:40:23 2022, max compression
+gzip compressed data, was "ox_secrets-0.5.0.tar", last modified: Fri Jul 21 15:25:35 2023, max compression
```

## Comparing `ox_secrets-0.4.0.tar` & `ox_secrets-0.5.0.tar`

### file list

```diff
@@ -1,22 +1,30 @@
-drwxr-xr-x   0 emin      (1000) emin      (1000)        0 2022-09-07 16:40:23.017866 ox_secrets-0.4.0/
--rw-r--r--   0 emin      (1000) emin      (1000)     1823 2022-09-07 16:40:23.017866 ox_secrets-0.4.0/PKG-INFO
--rw-r--r--   0 emin      (1000) emin      (1000)     1151 2022-08-15 16:56:47.000000 ox_secrets-0.4.0/README.rst
-drwxr-xr-x   0 emin      (1000) emin      (1000)        0 2022-09-07 16:40:23.017866 ox_secrets-0.4.0/ox_secrets/
--rw-r--r--   0 emin      (1000) emin      (1000)     3055 2022-09-07 16:18:24.000000 ox_secrets-0.4.0/ox_secrets/__init__.py
-drwxr-xr-x   0 emin      (1000) emin      (1000)        0 2022-09-07 16:40:23.017866 ox_secrets-0.4.0/ox_secrets/core/
--rw-r--r--   0 emin      (1000) emin      (1000)       42 2020-12-16 18:45:56.000000 ox_secrets-0.4.0/ox_secrets/core/__init__.py
--rw-r--r--   0 emin      (1000) emin      (1000)     4855 2022-09-07 16:38:35.000000 ox_secrets-0.4.0/ox_secrets/core/aws.py
--rw-r--r--   0 emin      (1000) emin      (1000)     9227 2022-09-06 23:37:11.000000 ox_secrets-0.4.0/ox_secrets/core/common.py
--rw-r--r--   0 emin      (1000) emin      (1000)     4373 2022-09-07 16:33:57.000000 ox_secrets-0.4.0/ox_secrets/core/evs.py
--rw-r--r--   0 emin      (1000) emin      (1000)     4517 2022-09-07 16:38:46.000000 ox_secrets-0.4.0/ox_secrets/core/fss.py
--rw-r--r--   0 emin      (1000) emin      (1000)     2909 2022-09-07 16:37:29.000000 ox_secrets-0.4.0/ox_secrets/server.py
--rw-r--r--   0 emin      (1000) emin      (1000)     1109 2022-08-15 16:56:47.000000 ox_secrets-0.4.0/ox_secrets/settings.py
-drwxr-xr-x   0 emin      (1000) emin      (1000)        0 2022-09-07 16:40:23.017866 ox_secrets-0.4.0/ox_secrets.egg-info/
--rw-r--r--   0 emin      (1000) emin      (1000)     1823 2022-09-07 16:40:22.000000 ox_secrets-0.4.0/ox_secrets.egg-info/PKG-INFO
--rw-r--r--   0 emin      (1000) emin      (1000)      415 2022-09-07 16:40:23.000000 ox_secrets-0.4.0/ox_secrets.egg-info/SOURCES.txt
--rw-r--r--   0 emin      (1000) emin      (1000)        1 2022-09-07 16:40:22.000000 ox_secrets-0.4.0/ox_secrets.egg-info/dependency_links.txt
--rw-r--r--   0 emin      (1000) emin      (1000)       40 2022-09-07 16:40:22.000000 ox_secrets-0.4.0/ox_secrets.egg-info/entry_points.txt
--rw-r--r--   0 emin      (1000) emin      (1000)        7 2022-09-07 16:40:22.000000 ox_secrets-0.4.0/ox_secrets.egg-info/requires.txt
--rw-r--r--   0 emin      (1000) emin      (1000)       11 2022-09-07 16:40:22.000000 ox_secrets-0.4.0/ox_secrets.egg-info/top_level.txt
--rw-r--r--   0 emin      (1000) emin      (1000)       38 2022-09-07 16:40:23.017866 ox_secrets-0.4.0/setup.cfg
--rw-r--r--   0 emin      (1000) emin      (1000)     1957 2020-12-16 18:45:56.000000 ox_secrets-0.4.0/setup.py
+drwxrwxr-x   0 emin      (1000) emin      (1000)        0 2023-07-21 15:25:35.662726 ox_secrets-0.5.0/
+-rw-------   0 emin      (1000) emin      (1000)     1145 2022-03-25 18:04:34.000000 ox_secrets-0.5.0/.gitignore
+-rw-------   0 emin      (1000) emin      (1000)     1325 2019-05-25 18:36:31.000000 ox_secrets-0.5.0/LICENSE.txt
+-rw-rw-r--   0 emin      (1000) emin      (1000)     6745 2023-07-21 15:25:35.662726 ox_secrets-0.5.0/PKG-INFO
+-rw-------   0 emin      (1000) emin      (1000)     5028 2023-07-21 15:22:25.000000 ox_secrets-0.5.0/README.org
+-rw-------   0 emin      (1000) emin      (1000)     5169 2023-07-21 15:25:35.000000 ox_secrets-0.5.0/README.rst
+-rw-------   0 emin      (1000) emin      (1000)       73 2019-05-25 18:34:28.000000 ox_secrets-0.5.0/conftest.py
+-rw-------   0 emin      (1000) emin      (1000)      458 2019-05-25 19:14:14.000000 ox_secrets-0.5.0/makefile
+drwxrwxr-x   0 emin      (1000) emin      (1000)        0 2023-07-21 15:25:35.658726 ox_secrets-0.5.0/ox_secrets/
+-rw-rw-r--   0 emin      (1000) emin      (1000)     3290 2023-07-21 15:22:11.000000 ox_secrets-0.5.0/ox_secrets/__init__.py
+drwxrwxr-x   0 emin      (1000) emin      (1000)        0 2023-07-21 15:25:35.662726 ox_secrets-0.5.0/ox_secrets/core/
+-rw-------   0 emin      (1000) emin      (1000)       42 2019-05-25 18:42:14.000000 ox_secrets-0.5.0/ox_secrets/core/__init__.py
+-rw-rw-r--   0 emin      (1000) emin      (1000)     2392 2022-02-02 03:56:49.000000 ox_secrets-0.5.0/ox_secrets/core/awp.py
+-rw-rw-r--   0 emin      (1000) emin      (1000)     4872 2023-07-20 19:48:50.000000 ox_secrets-0.5.0/ox_secrets/core/aws.py
+-rw-rw-r--   0 emin      (1000) emin      (1000)    12671 2023-07-21 15:08:03.000000 ox_secrets-0.5.0/ox_secrets/core/common.py
+-rw-rw-r--   0 emin      (1000) emin      (1000)     4373 2023-07-20 17:44:57.000000 ox_secrets-0.5.0/ox_secrets/core/evs.py
+-rw-rw-r--   0 emin      (1000) emin      (1000)     5513 2023-07-21 14:58:12.000000 ox_secrets-0.5.0/ox_secrets/core/fss.py
+-rw-rw-r--   0 emin      (1000) emin      (1000)      738 2022-02-28 17:21:49.000000 ox_secrets-0.5.0/ox_secrets/core/tss.py
+-rw-rw-r--   0 emin      (1000) emin      (1000)     4422 2023-07-21 15:10:45.000000 ox_secrets-0.5.0/ox_secrets/server.py
+-rw-------   0 emin      (1000) emin      (1000)     1109 2022-03-09 19:18:10.000000 ox_secrets-0.5.0/ox_secrets/settings.py
+drwxrwxr-x   0 emin      (1000) emin      (1000)        0 2023-07-21 15:25:35.658726 ox_secrets-0.5.0/ox_secrets.egg-info/
+-rw-------   0 emin      (1000) emin      (1000)     6745 2023-07-21 15:25:35.000000 ox_secrets-0.5.0/ox_secrets.egg-info/PKG-INFO
+-rw-------   0 emin      (1000) emin      (1000)      533 2023-07-21 15:25:35.000000 ox_secrets-0.5.0/ox_secrets.egg-info/SOURCES.txt
+-rw-------   0 emin      (1000) emin      (1000)        1 2023-07-21 15:25:35.000000 ox_secrets-0.5.0/ox_secrets.egg-info/dependency_links.txt
+-rw-------   0 emin      (1000) emin      (1000)       40 2023-07-21 15:25:35.000000 ox_secrets-0.5.0/ox_secrets.egg-info/entry_points.txt
+-rw-------   0 emin      (1000) emin      (1000)        7 2023-07-21 15:25:35.000000 ox_secrets-0.5.0/ox_secrets.egg-info/requires.txt
+-rw-------   0 emin      (1000) emin      (1000)       11 2023-07-21 15:25:35.000000 ox_secrets-0.5.0/ox_secrets.egg-info/top_level.txt
+-rw-------   0 emin      (1000) emin      (1000)       14 2019-05-25 18:37:44.000000 ox_secrets-0.5.0/requirements.txt
+-rw-rw-r--   0 emin      (1000) emin      (1000)       38 2023-07-21 15:25:35.662726 ox_secrets-0.5.0/setup.cfg
+-rw-------   0 emin      (1000) emin      (1000)     1957 2019-05-25 18:41:30.000000 ox_secrets-0.5.0/setup.py
```

### Comparing `ox_secrets-0.4.0/ox_secrets/__init__.py` & `ox_secrets-0.5.0/ox_secrets/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,20 +16,27 @@
 >>> print(open(fn).read().strip())
 name,category,value,notes
 example_name,root,super_secret,example secret
 example_pw,prod/data,super_secret_pw,example secret_pw
 example_pw,test/data,unsecret_test_pw,example secret test pw
 example_pw,alt,alt_unsecret_test_pw,alt secret test pw
 
+Now that we have a secrets file, we can read some secrets:
+
 >>> from ox_secrets import settings, server as oss
 >>> oss.settings.OX_SECRETS_FILE = fn # default is ~/.ox_secrets.csv
 >>> oss.forget_secrets()  # Clear it to make sure we start fresh
 >>> oss.get_secret('example_name')
 'super_secret'
 
+We can also get a dictionary of all the secrets for a given category:
+
+>>> oss.get_secret_dict(category='test/data')
+{'example_pw': 'unsecret_test_pw'}
+
 Sometimes it is nice to be able to just pass a dictionary of
 credential information to get_secret:
 
 >>> creds = {'name': 'example_name', 'category': 'root', 'server': 'fss'}
 >>> oss.get_secret(**creds)
 'super_secret'
 
@@ -83,8 +90,9 @@
     oss.get_server(mode='aws').store_secrets(
         {'test_storage':'foobar', category=AWS_PARAM_NAME,
         service_name='ssm')
 
 
 """
 
-VERSION = '0.4.0'
+VERSION = '0.5.0'
+__version__ = VERSION
```

### Comparing `ox_secrets-0.4.0/ox_secrets/core/aws.py` & `ox_secrets-0.5.0/ox_secrets/core/aws.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,16 @@
         logging.warning(
             'Connecting to boto3 for profile %s to read secrets for %s',
             profile_name, secret_id)
         service_name = kwargs.pop('service_name', 'secretsmanager')
         session = boto3.Session(profile_name=profile_name, **kwargs)
         client = session.client(service_name=service_name)
         if service_name == 'secretsmanager':
-            get_secret_value_response = client.get_secret_value(SecretId=secret_id)
+            get_secret_value_response = client.get_secret_value(
+                SecretId=secret_id)
             secret_data = get_secret_value_response['SecretString']
             secret_dict = json.loads(secret_data)
         elif service_name == 'ssm':
             get_secret_value_response = client.get_parameter(Name=secret_id)
             secret_data = get_secret_value_response['Parameter']['Value']
             if secret_id[-5:].lower() == '.json':
                 secret_dict = json.loads(secret_data)
```

### Comparing `ox_secrets-0.4.0/ox_secrets/core/common.py` & `ox_secrets-0.5.0/ox_secrets/core/common.py`

 * *Files 14% similar despite different names*

```diff
@@ -30,15 +30,17 @@
     def load_cache(cls, name: typing.Optional[str] = None,
                    category: typing.Optional[str] = None,
                    loader_params: typing.Optional[dict] = None):
         """Load secrets and cache them from back-end store.
 
         :param name:  String name of secret desired. Some back-ends can load
                       the cache for all secrets at once while others require
-                      the name and/or category.
+                      the name and/or category. You should be able to pass
+                      None for name to indicate loading everything for
+                      the given category.
 
         :param category:  String name of secret desired. Some back-ends can
                           load the cache for all secrets at once while others
                           require the name and/or category.
 
 
         ~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-
@@ -100,64 +102,142 @@
         :param allow_update=True:  Whether to loading cache if secret not
                                    found.
 
         :param loader_params: Optional dict of parameters which gets
                               passed to load_cache for back-end. This allows
                               a way to pass back-end specific info if desired.
 
-        :param service_name: Optional string to add as loader_params['service_name']. The
-                             service_name is used by the AWS secret manager and parameter
-                             store and nice to be able to specify directly.
+        :param service_name: Optional string to add as
+                             loader_params['service_name']. The
+                             service_name is used by the AWS secret manager
+                             and parameter store and nice to be able to
+                             specify directly.
 
         ~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-
 
         :return:   Value of secret.
 
         ~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-
 
         PURPOSE:   Simple way to lookup secrets.
 
         """
         category = cls.maybe_replace_category(category)
         result = cls.secret_from_env(name, category, allow_env)
         if result is not None:
             return result
-        with cls._lock:  # get the lock to prevent multiple read/write cache
-            cdict = cls._cache.get(category, None)
-            if cdict is not None:
+        with cls._lock:
+            cdict = cls._cache.get(category, {})
+            if name in cdict:
                 return cdict[name]
-        assert cdict is None  # must be here if category not in cache
-        if allow_update:
-            if service_name is not None:
-                if loader_params is None:
-                    loader_params = {}
-                loader_params['service_name'] = service_name
-            cls.load_cache(name=name, category=category,
-                           loader_params=loader_params)
-            return cls.get_secret(
-                name, category,
-                allow_env=False,  # already tried env, so don't retry
-                allow_update=False,  # don't get into infinite loop
-                loader_params=loader_params)
-        logging.error('Unable to find category %s for secret manager class %s',
-                      category, cls.__name__)
-        raise KeyError(category)
+            # Secret not found so clear cache to rebuild
+            cls._cache[category] = None
+            del cls._cache[category]
+        cls._prepare_secrets_dict(category, allow_update,
+                                  loader_params, service_name)
+
+        with cls._lock:  # must lock since cdict may refernce cls._cdict
+            cdict = cls._cache[category]
+            return cdict[name]
+
+    @classmethod
+    def get_secret_dict(cls, category: str = 'root',
+                        allow_update: bool = True,
+                        loader_params: typing.Optional[dict] = None,
+                        service_name: typing.Optional[str] = None):
+        """Lookup secret with given name and return it.
+
+        :param category='root':  Optional string category for secret
+
+        :param allow_update=True:  Whether to loading cache if secret not
+                                   found.
+
+        :param loader_params: Optional dict of parameters which gets
+                              passed to load_cache for back-end. This allows
+                              a way to pass back-end specific info if desired.
+
+        :param service_name: Optional string to add as
+                             loader_params['service_name']. The service_name
+                              is used by the AWS secret manager and parameter
+                             store and nice to be able to specify directly.
+
+        ~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-
+
+        :return:   Value of secret.
+
+        ~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-
+
+        PURPOSE:   Simple way to lookup secrets.
+
+        """
+        category = cls.maybe_replace_category(category)
+        cls._prepare_secrets_dict(category, allow_update, loader_params,
+                                  service_name)
+        with cls._lock:
+            return dict(cls._cache[category])  # return shallow copy
+
+    @classmethod
+    def _prepare_secrets_dict(
+            cls, category: str, allow_update: bool,
+            loader_params: typing.Optional[dict] = None,
+            service_name: typing.Optional[str] = None):
+        """Help prepare secrets in cls._cache for get_secret and get_secret.
+
+        :param category:  String category for secrets.
+
+        :param allow_update=True:  Whether to loading cache if secret not
+                                   found.
+
+        :param loader_params: Optional dict of parameters which gets
+                              passed to load_cache for back-end. This allows
+                              a way to pass back-end specific info if desired.
+
+        :param service_name: Optional string to add as
+                             loader_params['service_name']. The service_name
+                              is used by the AWS secret manager and parameter
+                             store and nice to be able to specify directly.
+
+        ~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-
+
+        PURPOSE:   This is a helper function to only be called by
+                   get_secret and get_secret_dict. If cls._cache[category]
+                   is non-empty, then this does nothign since we assume
+                   we already have secrets loaded
+
+        """
+
+        if cls._cache.get(category):  # have something so no need to reload
+            return
+        if not allow_update:
+            with cls._lock:
+                cdict = cls._cache.get(category, None)
+                if cdict is not None:   # did have something there
+                    return              # so stop processing
+                logging.error(          # otherwise indicate an error
+                    'Unable to find category %s for secret manager class %s',
+                    category, cls.__name__)
+                raise KeyError(category)  # no data and no update allowed
+        if service_name is not None:
+            if loader_params is None:
+                loader_params = {}
+            loader_params['service_name'] = service_name
+        cls.load_cache(name=None, category=category,
+                       loader_params=loader_params)
 
     @staticmethod
     def maybe_replace_category(category):
         """Replace input based on OX_SECRETS_CATEGORY_REGEXP.
 
 Meant to be called by get_secret.
         """
         if settings.OX_SECRETS_CATEGORY_REGEXP:
             return re.sub(settings.OX_SECRETS_CATEGORY_REGEXP,
                           settings.OX_SECRETS_CATEGORY_REPLACE, category)
         return category
 
-
     @classmethod
     def list_secret_names(cls, category: str) -> typing.List[str]:
         "Return list of secret names for given category."
 
         with cls._lock:  # get the lock to prevent modification while we look
             cdict = cls._cache.get(category, [])
             return list(cdict)
```

### Comparing `ox_secrets-0.4.0/ox_secrets/core/evs.py` & `ox_secrets-0.5.0/ox_secrets/core/evs.py`

 * *Files identical despite different names*

### Comparing `ox_secrets-0.4.0/ox_secrets/core/fss.py` & `ox_secrets-0.5.0/ox_secrets/core/fss.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,59 +5,79 @@
 """
 
 
 import logging
 import csv
 import os
 import typing
+import json
 
 from ox_secrets import settings
 from ox_secrets.core import common
 
 
 class FileSecretServer(common.SecretServer):
     """Class to handle getting secrets from file.
     """
 
     @classmethod
-    def load_secrets_file(cls, filename=None, encoding='utf8'):
+    def load_secrets_file(cls, filename=None, encoding='utf8',
+                          file_type=None, default_category='root'):
         """Load secrets file from given filename.
 
         :param filename=None:    Optional filename for secrets. This
                                  defaults to ~/.ox_secrets.csv.
                                  It shall be a CSV file with header
-                                 category,name,value,notes.
+                                 category,name,value,notes. You can also
+                                 provide a .json file containing a dict
+                                 of name value pairs which will all go
+                                 in the default_category.
+
+        :param encoding='utf8':  Default encoding for opening files.
+
+        :param file_type:  Either .csv or .json or None if you want to
+                           select based on file extension.
+
+        :param default_category='root':  Category to use when cannot
+                                         otherwise find it.
 
         ~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-~-
 
         PURPOSE:  Fill cls._cache with data from secrets file.
 
         """
         if filename is None:
             filename = os.environ.get(
                 'OX_SECRETS_FILE', settings.OX_SECRETS_FILE)
         logging.warning('Opening secrets file "%s"', filename)
-        with open(filename, 'r', encoding=encoding) as sfd:
-            reader = csv.DictReader(sfd)
-            with cls._lock:
-                for line in reader:
-                    if line['category'] not in cls._cache:
-                        cls._cache[line['category']] = {}
-                    cls._cache[line['category']][line['name']] = line[
-                        'value']
+        with cls._lock, open(filename, 'r', encoding=encoding) as sfd:
+            if file_type is None:
+                file_type = os.path.splitext(filename)[-1].lower()
+            if file_type == '.csv':
+                contents = list(csv.DictReader(sfd))
+            elif file_type == '.json':
+                contents = [{'name': k, 'value': v}
+                            for k, v in json.load(sfd).items()]
+            else:
+                raise ValueError(f'Cannot handle secrets {file_type=}')
+            for line in contents:
+                line_category = line.get('category', default_category)
+                if line_category not in cls._cache:
+                    cls._cache[line_category] = {}
+                cls._cache[line_category][line['name']] = line[
+                    'value']
 
     @classmethod
     def load_cache(cls, name: typing.Optional[str] = None,
                    category: typing.Optional[str] = None,
                    loader_params: typing.Optional[dict] = None):
         "Implement loading cache from a file."
         loader_params = loader_params if loader_params is not None else {}
-        logging.debug('Ignoring name=%s/category=%s for %s', name,
-                      category, cls.__name__)
-        return cls.load_secrets_file(**loader_params)
+        return cls.load_secrets_file(default_category=category,
+                                     **loader_params)
 
     @classmethod
     def store_secrets(cls, new_secret_dict: typing.Dict[str, str],
                       category: str, **storage_params):
         """Implement as required by parent class.
         """
         cls.store_secrets_to_file(new_secret_dict, category, **storage_params)
```

### Comparing `ox_secrets-0.4.0/ox_secrets/settings.py` & `ox_secrets-0.5.0/ox_secrets/settings.py`

 * *Files identical despite different names*

### Comparing `ox_secrets-0.4.0/setup.py` & `ox_secrets-0.5.0/setup.py`

 * *Files identical despite different names*

