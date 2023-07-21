# Comparing `tmp/libtimed-0.3.0.tar.gz` & `tmp/libtimed-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libtimed-0.3.0.tar", max compression
+gzip compressed data, was "libtimed-0.3.1.tar", max compression
```

## Comparing `libtimed-0.3.0.tar` & `libtimed-0.3.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    34454 2023-07-21 07:34:54.452994 libtimed-0.3.0/LICENSE
--rw-r--r--   0        0        0      750 2023-07-21 07:34:54.456994 libtimed-0.3.0/README.md
--rw-r--r--   0        0        0     1307 2023-07-21 07:34:55.493023 libtimed-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1322 2023-07-21 07:34:54.456994 libtimed-0.3.0/src/libtimed/__init__.py
--rw-r--r--   0        0        0     9477 2023-07-21 07:34:54.456994 libtimed-0.3.0/src/libtimed/models.py
--rw-r--r--   0        0        0     4555 2023-07-21 07:34:54.456994 libtimed-0.3.0/src/libtimed/oidc.py
--rw-r--r--   0        0        0     6026 2023-07-21 07:34:54.456994 libtimed-0.3.0/src/libtimed/transforms.py
--rw-r--r--   0        0        0     1313 1970-01-01 00:00:00.000000 libtimed-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    34454 2023-07-21 12:49:36.062493 libtimed-0.3.1/LICENSE
+-rw-r--r--   0        0        0      750 2023-07-21 12:49:36.062493 libtimed-0.3.1/README.md
+-rw-r--r--   0        0        0     1307 2023-07-21 12:49:36.814494 libtimed-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     1376 2023-07-21 12:49:36.062493 libtimed-0.3.1/src/libtimed/__init__.py
+-rw-r--r--   0        0        0     9485 2023-07-21 12:49:36.062493 libtimed-0.3.1/src/libtimed/models.py
+-rw-r--r--   0        0        0     4555 2023-07-21 12:49:36.062493 libtimed-0.3.1/src/libtimed/oidc.py
+-rw-r--r--   0        0        0     6026 2023-07-21 12:49:36.062493 libtimed-0.3.1/src/libtimed/transforms.py
+-rw-r--r--   0        0        0     1313 1970-01-01 00:00:00.000000 libtimed-0.3.1/PKG-INFO
```

### Comparing `libtimed-0.3.0/LICENSE` & `libtimed-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `libtimed-0.3.0/README.md` & `libtimed-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `libtimed-0.3.0/pyproject.toml` & `libtimed-0.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "libtimed"
-version = "0.3.0"
+version = "0.3.1"
 description = "Library to intreact with timed webapp."
 authors = [
   "Arthur Deierlein <arthur.deierlein@adfinis.com>",
   "Gian Klug <gian.klug@adfinis.com>",
 ]
 readme = "README.md"
 packages = [{ include = "libtimed", from = "src" }]
```

### Comparing `libtimed-0.3.0/src/libtimed/__init__.py` & `libtimed-0.3.1/src/libtimed/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,15 +9,17 @@
 class TimedAPIClient:
     def __init__(self, token, url, api_namespace):
         self.token = token
         self.url = f"{url}/{api_namespace}/"
         self.session = requests.Session()
         self.session.headers["Authorization"] = f"Bearer {token}"
         self.session.headers["Content-Type"] = "application/vnd.api+json"
-        self.cached_session = requests_cache.CachedSession(expire_after=60 * 60 * 24)
+        self.cached_session = requests_cache.CachedSession(
+            "libtimed", expire_after=60 * 60 * 24, use_cache_dir=True
+        )
         self.cached_session.headers["Authorization"] = f"Bearer {token}"
         self.cached_session.headers["Content-Type"] = "application/vnd.api+json"
         # Models
         self.users = models.Users(self)
         self.reports = models.Reports(self)
         self.overtime = models.WorktimeBalances(self)
         self.activities = models.Activities(self)
```

### Comparing `libtimed-0.3.0/src/libtimed/models.py` & `libtimed-0.3.1/src/libtimed/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -279,15 +279,15 @@
         return self.post(**kwargs)
 
     def stop(self):
         if self.current:
             attributes = self.current["attributes"]
             relationships = self.current["relationships"]
             attributes["to-time"] = datetime.now()
-            r = self.patch(self.current["id"], attributes, relationships)
+            r = self.patch({"id": self.current["id"]}, attributes, relationships)
             return r
 
 
 class Reports(BaseModel):
     attributes = [COMMENT, DATE, DURATION, REVIEW, NOT_BILLABLE]
 
     relationships = [CURRENT_USER_RELATIONSHIP, ("task", None, Tasks)]
```

### Comparing `libtimed-0.3.0/src/libtimed/oidc.py` & `libtimed-0.3.1/src/libtimed/oidc.py`

 * *Files identical despite different names*

### Comparing `libtimed-0.3.0/src/libtimed/transforms.py` & `libtimed-0.3.1/src/libtimed/transforms.py`

 * *Files identical despite different names*

### Comparing `libtimed-0.3.0/PKG-INFO` & `libtimed-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libtimed
-Version: 0.3.0
+Version: 0.3.1
 Summary: Library to intreact with timed webapp.
 Author: Arthur Deierlein
 Author-email: arthur.deierlein@adfinis.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

