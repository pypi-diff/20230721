# Comparing `tmp/libtimed-0.2.1.tar.gz` & `tmp/libtimed-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libtimed-0.2.1.tar", max compression
+gzip compressed data, was "libtimed-0.3.0.tar", max compression
```

## Comparing `libtimed-0.2.1.tar` & `libtimed-0.3.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    34454 2023-07-19 10:23:55.899385 libtimed-0.2.1/LICENSE
--rw-r--r--   0        0        0      750 2023-07-19 10:23:55.899385 libtimed-0.2.1/README.md
--rw-r--r--   0        0        0     1281 2023-07-19 10:23:56.743418 libtimed-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     1061 2023-07-19 10:23:55.903385 libtimed-0.2.1/src/libtimed/__init__.py
--rw-r--r--   0        0        0     9387 2023-07-19 10:23:55.903385 libtimed-0.2.1/src/libtimed/models.py
--rw-r--r--   0        0        0     4533 2023-07-19 10:23:55.903385 libtimed-0.2.1/src/libtimed/oidc.py
--rw-r--r--   0        0        0     6026 2023-07-19 10:23:55.903385 libtimed-0.2.1/src/libtimed/transforms.py
--rw-r--r--   0        0        0     1266 1970-01-01 00:00:00.000000 libtimed-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    34454 2023-07-21 07:34:54.452994 libtimed-0.3.0/LICENSE
+-rw-r--r--   0        0        0      750 2023-07-21 07:34:54.456994 libtimed-0.3.0/README.md
+-rw-r--r--   0        0        0     1307 2023-07-21 07:34:55.493023 libtimed-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1322 2023-07-21 07:34:54.456994 libtimed-0.3.0/src/libtimed/__init__.py
+-rw-r--r--   0        0        0     9477 2023-07-21 07:34:54.456994 libtimed-0.3.0/src/libtimed/models.py
+-rw-r--r--   0        0        0     4555 2023-07-21 07:34:54.456994 libtimed-0.3.0/src/libtimed/oidc.py
+-rw-r--r--   0        0        0     6026 2023-07-21 07:34:54.456994 libtimed-0.3.0/src/libtimed/transforms.py
+-rw-r--r--   0        0        0     1313 1970-01-01 00:00:00.000000 libtimed-0.3.0/PKG-INFO
```

### Comparing `libtimed-0.2.1/LICENSE` & `libtimed-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `libtimed-0.2.1/README.md` & `libtimed-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `libtimed-0.2.1/pyproject.toml` & `libtimed-0.3.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [tool.poetry]
 name = "libtimed"
-version = "0.2.1"
+version = "0.3.0"
 description = "Library to intreact with timed webapp."
 authors = [
   "Arthur Deierlein <arthur.deierlein@adfinis.com>",
   "Gian Klug <gian.klug@adfinis.com>",
 ]
 readme = "README.md"
 packages = [{ include = "libtimed", from = "src" }]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 requests = "^2.31.0"
 keyring = "^24.1.0"
 inflection = "^0.5.1"
+requests-cache = "^1.1.0"
 
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 pytest = "^7.3.2"
 pytest-coverage = "^0.0"
 isort = "^5.12.0"
```

### Comparing `libtimed-0.2.1/src/libtimed/__init__.py` & `libtimed-0.3.0/src/libtimed/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 from inspect import isclass
 
 import requests
+import requests_cache
 
 from libtimed import models
 
 
 class TimedAPIClient:
     def __init__(self, token, url, api_namespace):
         self.token = token
         self.url = f"{url}/{api_namespace}/"
         self.session = requests.Session()
         self.session.headers["Authorization"] = f"Bearer {token}"
         self.session.headers["Content-Type"] = "application/vnd.api+json"
-
+        self.cached_session = requests_cache.CachedSession(expire_after=60 * 60 * 24)
+        self.cached_session.headers["Authorization"] = f"Bearer {token}"
+        self.cached_session.headers["Content-Type"] = "application/vnd.api+json"
         # Models
         self.users = models.Users(self)
         self.reports = models.Reports(self)
         self.overtime = models.WorktimeBalances(self)
         self.activities = models.Activities(self)
         self.customers = models.Customers(self)
         self.tasks = models.Tasks(self)
```

### Comparing `libtimed-0.2.1/src/libtimed/models.py` & `libtimed-0.3.0/src/libtimed/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,22 +108,24 @@
 
     def get(
         self,
         filters={},
         include: Optional[str] = None,
         id: Union[str, int, None] = None,
         raw=False,
+        cached=False,
     ) -> dict:
         url = f"{self.url}/{id}" if id else self.url
         if id:
             params = {"include": include}
         else:
             params = {**self._parse_filters(filters), "include": include}
 
-        resp = self.client.session.get(url, params=params)
+        session = self.client.cached_session if cached else self.client.session
+        resp = session.get(url, params=params)
         resp = resp.json()
 
         # de-serialize
         if data := ([resp.get("data")] if id else resp.get("data")):
             for item in data:
                 item = self._deserialize(item, resp.get("included", []))
         return resp if raw else resp.get("data")
```

### Comparing `libtimed-0.2.1/src/libtimed/oidc.py` & `libtimed-0.3.0/src/libtimed/oidc.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,17 @@
     def __init__(self, client_id, sso_url, sso_realm, auth_path):
         self.client_id = client_id
         self.sso_url = sso_url
         self.sso_realm = sso_realm
         self.auth_path = auth_path
 
     def autoconfig(self):
-        data = requests.get(f"{self.sso_url}/auth/realms/{self.sso_realm}/.well-known/openid-configuration").json()
+        data = requests.get(
+            f"{self.sso_url}/auth/realms/{self.sso_realm}/.well-known/openid-configuration"
+        ).json()
         self.authorization_endpoint = data["authorization_endpoint"]
         self.token_endpoint = data["token_endpoint"]
 
     def start_browser_flow(self):
         # construct the authorization request
         auth_url = f"{self.authorization_endpoint}?client_id={self.client_id}&response_type=code&scope=openid&redirect_uri=http://localhost:5000/{self.auth_path}"
         # start a temporary web server
```

### Comparing `libtimed-0.2.1/src/libtimed/transforms.py` & `libtimed-0.3.0/src/libtimed/transforms.py`

 * *Files identical despite different names*

### Comparing `libtimed-0.2.1/PKG-INFO` & `libtimed-0.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: libtimed
-Version: 0.2.1
+Version: 0.3.0
 Summary: Library to intreact with timed webapp.
 Author: Arthur Deierlein
 Author-email: arthur.deierlein@adfinis.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: inflection (>=0.5.1,<0.6.0)
 Requires-Dist: keyring (>=24.1.0,<25.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: requests-cache (>=1.1.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 # libtimed
 [![License: AGPL v3](https://img.shields.io/badge/License-AGPL%20v3-blue.svg)](https://www.gnu.org/licenses/agpl-3.0)
 
 A python library to interact with the JSON API of [timed](https://github.com/adfinis/timed-backend). It authenticates using a custom OIDC browser flow, locally on your machine.
```

