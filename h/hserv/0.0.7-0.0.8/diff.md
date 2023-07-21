# Comparing `tmp/hserv-0.0.7.tar.gz` & `tmp/hserv-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hserv-0.0.7.tar", last modified: Fri Jul 21 15:36:46 2023, max compression
+gzip compressed data, was "hserv-0.0.8.tar", last modified: Fri Jul 21 15:51:22 2023, max compression
```

## Comparing `hserv-0.0.7.tar` & `hserv-0.0.8.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 15:36:46.159311 hserv-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (122)    35149 2023-07-21 15:36:34.000000 hserv-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       58 2023-07-21 15:36:34.000000 hserv-0.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      297 2023-07-21 15:36:46.155311 hserv-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       69 2023-07-21 15:36:34.000000 hserv-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 15:36:46.155311 hserv-0.0.7/hserv/
--rw-r--r--   0 runner    (1001) docker     (122)       36 2023-07-21 15:36:34.000000 hserv-0.0.7/hserv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       20 2023-07-21 15:36:34.000000 hserv-0.0.7/hserv/__version__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5753 2023-07-21 15:36:34.000000 hserv-0.0.7/hserv/server.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 15:36:46.155311 hserv-0.0.7/hserv/supabase/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-21 15:36:34.000000 hserv-0.0.7/hserv/supabase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3054 2023-07-21 15:36:34.000000 hserv-0.0.7/hserv/supabase/config.py
--rw-r--r--   0 runner    (1001) docker     (122)    10454 2023-07-21 15:36:34.000000 hserv-0.0.7/hserv/supabase/controller.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 15:36:46.155311 hserv-0.0.7/hserv/webproxy/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-21 15:36:34.000000 hserv-0.0.7/hserv/webproxy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      212 2023-07-21 15:36:34.000000 hserv-0.0.7/hserv/webproxy/proxy.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 15:36:46.155311 hserv-0.0.7/hserv.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      297 2023-07-21 15:36:46.000000 hserv-0.0.7/hserv.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      386 2023-07-21 15:36:46.000000 hserv-0.0.7/hserv.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-21 15:36:46.000000 hserv-0.0.7/hserv.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       47 2023-07-21 15:36:46.000000 hserv-0.0.7/hserv.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-07-21 15:36:46.000000 hserv-0.0.7/hserv.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       46 2023-07-21 15:36:34.000000 hserv-0.0.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-21 15:36:46.159311 hserv-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      704 2023-07-21 15:36:34.000000 hserv-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 15:51:22.498094 hserv-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (122)    35149 2023-07-21 15:51:09.000000 hserv-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       58 2023-07-21 15:51:09.000000 hserv-0.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      297 2023-07-21 15:51:22.498094 hserv-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2023-07-21 15:51:09.000000 hserv-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 15:51:22.498094 hserv-0.0.8/hserv/
+-rw-r--r--   0 runner    (1001) docker     (122)       36 2023-07-21 15:51:09.000000 hserv-0.0.8/hserv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       20 2023-07-21 15:51:09.000000 hserv-0.0.8/hserv/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5753 2023-07-21 15:51:09.000000 hserv-0.0.8/hserv/server.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 15:51:22.498094 hserv-0.0.8/hserv/supabase/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-21 15:51:09.000000 hserv-0.0.8/hserv/supabase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3039 2023-07-21 15:51:09.000000 hserv-0.0.8/hserv/supabase/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10742 2023-07-21 15:51:09.000000 hserv-0.0.8/hserv/supabase/controller.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 15:51:22.498094 hserv-0.0.8/hserv/webproxy/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-21 15:51:09.000000 hserv-0.0.8/hserv/webproxy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      212 2023-07-21 15:51:09.000000 hserv-0.0.8/hserv/webproxy/proxy.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 15:51:22.498094 hserv-0.0.8/hserv.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      297 2023-07-21 15:51:22.000000 hserv-0.0.8/hserv.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      386 2023-07-21 15:51:22.000000 hserv-0.0.8/hserv.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-21 15:51:22.000000 hserv-0.0.8/hserv.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       47 2023-07-21 15:51:22.000000 hserv-0.0.8/hserv.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-07-21 15:51:22.000000 hserv-0.0.8/hserv.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       46 2023-07-21 15:51:09.000000 hserv-0.0.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-21 15:51:22.498094 hserv-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      704 2023-07-21 15:51:09.000000 hserv-0.0.8/setup.py
```

### Comparing `hserv-0.0.7/LICENSE` & `hserv-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `hserv-0.0.7/hserv/server.py` & `hserv-0.0.8/hserv/server.py`

 * *Files identical despite different names*

### Comparing `hserv-0.0.7/hserv/supabase/config.py` & `hserv-0.0.8/hserv/supabase/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Dict, List, Union, TYPE_CHECKING
+from typing import Any, Dict, List, Union, TYPE_CHECKING
 from dataclasses import dataclass, field
 import os
 import io
 import re
 import yaml
 
 if TYPE_CHECKING:
@@ -49,48 +49,44 @@
         kongBuf = io.StringIO()
         yaml.dump(self._kong, kongBuf)
 
         # send to the server
         self.controller.server.put(envBuf, self._env_path)
         self.controller.server.put(kongBuf, self._kong_path)
 
-    def __getattr__(self, name: str):
+    def get(self, name: str, default: Any = 'raise'):
         # first check if name is in the lookup table
         if name in ENV_LOOKUP:
             names = ENV_LOOKUP[name]
         else:
             names = [name]
 
         # use only the first, as all have the same value
         name = names[0]
 
         # extract
         regex = re.search(r'%s=(.+)[\n\r]' % name, self._env)
         if regex is None:
-            raise AttributeError(f"Attriubte '{name}' is not a valid environment configuration value.")
+            if default == 'raise':
+                raise AttributeError(f"Attribute '{name}' is not a valid environment configuration value.")
+            else:
+                return default
         else:
             return regex.group(1)
-
-    def get(self, name: str, default=None):
-        try:
-            return getattr(self, name)
-        except AttributeError:
-            return default
     
-    def __setattr__(self, name: str, value: Union[str, int]):
+    def set(self, name: str, value: Union[str, int]):
         # make a list first
         if name in ENV_LOOKUP:
             names = ENV_LOOKUP[name]
         else:
             names = [name]
         
         # check that all names are in the env
         if not all([n in self._env for n in names]):
-            super().__setattr__(name, value)
-            return 
+            raise AttributeError(f"Attribute '{name}' is not a valid environment configuration value.")
         
         # still here means replace the config
         env = self._env
         for n in names:
             # get the current value
             current_val = getattr(self, n)
             env.replace(f"{n}={current_val}", f"{n}={value}")
```

### Comparing `hserv-0.0.7/hserv/supabase/controller.py` & `hserv-0.0.8/hserv/supabase/controller.py`

 * *Files 3% similar despite different names*

```diff
@@ -216,45 +216,53 @@
     def update_supabase_config(self, jwt=False, postgres=False, domain=False):
         # instantiate a Config object
         conf = SupabaseConfig(self)
         
         # update the postgres password
         if postgres:
             # set the password
-            conf.pg_password = self.pg_password
-            conf.pg_port = self.pg_port
+            conf.set('pg_password',  self.pg_password)
+            conf.set('pg_port', self.pg_port)
         
         # update the jwt secret
         if jwt:
             # replace jwt secret
-            conf.jwt_secret = self.jwt_secret
+            conf.set('jwt_secret',  self.jwt_secret)
 
             # repalce the api keys in the environment file
-            conf.anon_jwt = self.generate_jwt('anon')
-            conf.service_jwt = self.generate_jwt('service_role')
+            conf.set('anon_jwt', self.generate_jwt('anon'))
+            conf.set('service_jwt', self.generate_jwt('service_role'))
 
-            # replace the keys in the API config
+            # extract the kong config directly, there is no better way as of now
             kong = conf._kong
+
+            # replace the keys in the API config
             anon = [c for c in kong['consumers'] if c['username'] == 'anon'][0]
             anon['keyauth_credentials'] = [{"key": self.generate_jwt('anon')}]
 
             service = [c for c in kong['consumers'] if c['username'] == 'service_role'][0]
             service['keyauth_credentials'] = [{"key": self.generate_jwt('service_role')}]
             kong['consumers'] = [anon, service]
+
+            # save kong config back to the config object
+            conf._kong = kong
         
         if domain:
             # replace the domain
-            conf.site_url = self.site_url
+            conf.set('site_url',self.site_url)
 
             # replace API url
-            conf.api_url = f"{self.public_url}:{self.kong_port}"
+            conf.set('api_url', f"{self.public_url}:{self.kong_port}")
 
             # replace ports
-            conf.api_port = self.kong_port
-            conf.public_port = self.public_port
+            conf.set('api_port', self.kong_port)
+            conf.set('public_port', self.public_port)
+        
+        # finally save the config
+        conf.save()
 
     def _curl_json(self, url: str) -> dict:
         # check that curl is available
         if self.server.info.get('curl_version', 'unknown') == 'unknown':
             raise RuntimeError("Curl is not installed on the server.")
         
         try:
```

### Comparing `hserv-0.0.7/setup.py` & `hserv-0.0.8/setup.py`

 * *Files identical despite different names*

