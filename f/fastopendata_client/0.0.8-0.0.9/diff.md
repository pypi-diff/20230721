# Comparing `tmp/fastopendata_client-0.0.8.tar.gz` & `tmp/fastopendata_client-0.0.9.tar.gz`

## Comparing `fastopendata_client-0.0.8.tar` & `fastopendata_client-0.0.9.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 fastopendata_client-0.0.8/src/fastopendata_client/__init__.py
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 fastopendata_client-0.0.8/src/fastopendata_client/client.py
--rw-r--r--   0        0        0    25069 2020-02-02 00:00:00.000000 fastopendata_client-0.0.8/src/fastopendata_client/session.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 fastopendata_client-0.0.8/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 fastopendata_client-0.0.8/LICENSE
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 fastopendata_client-0.0.8/README.md
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 fastopendata_client-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 fastopendata_client-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 fastopendata_client-0.0.9/src/fastopendata_client/__init__.py
+-rw-r--r--   0        0        0    11824 2020-02-02 00:00:00.000000 fastopendata_client-0.0.9/src/fastopendata_client/client.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 fastopendata_client-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 fastopendata_client-0.0.9/LICENSE
+-rw-r--r--   0        0        0     2249 2020-02-02 00:00:00.000000 fastopendata_client-0.0.9/README.md
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 fastopendata_client-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     2781 2020-02-02 00:00:00.000000 fastopendata_client-0.0.9/PKG-INFO
```

### Comparing `fastopendata_client-0.0.8/.gitignore` & `fastopendata_client-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `fastopendata_client-0.0.8/LICENSE` & `fastopendata_client-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `fastopendata_client-0.0.8/pyproject.toml` & `fastopendata_client-0.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "fastopendata_client"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Zachary Ernst", email="zac.ernst@gmail.com" },
 ]
 description = "Client for the FastOpenData API service"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

