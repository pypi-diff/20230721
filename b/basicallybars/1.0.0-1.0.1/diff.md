# Comparing `tmp/basicallybars-1.0.0.tar.gz` & `tmp/basicallybars-1.0.1.tar.gz`

## Comparing `basicallybars-1.0.0.tar` & `basicallybars-1.0.1.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 basicallybars-1.0.0/src/basicallybars/__init__.py
--rw-r--r--   0        0        0     2286 2020-02-02 00:00:00.000000 basicallybars-1.0.0/src/basicallybars/basicallybars.py
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 basicallybars-1.0.0/LICENCE
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 basicallybars-1.0.0/README.md
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 basicallybars-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     2044 2020-02-02 00:00:00.000000 basicallybars-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     2286 2020-02-02 00:00:00.000000 basicallybars-1.0.1/src/basicallybars/__init__.py
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 basicallybars-1.0.1/LICENCE
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 basicallybars-1.0.1/README.md
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 basicallybars-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2025 2020-02-02 00:00:00.000000 basicallybars-1.0.1/PKG-INFO
```

### Comparing `basicallybars-1.0.0/src/basicallybars/basicallybars.py` & `basicallybars-1.0.1/src/basicallybars/__init__.py`

 * *Files identical despite different names*

### Comparing `basicallybars-1.0.0/LICENCE` & `basicallybars-1.0.1/LICENCE`

 * *Files identical despite different names*

### Comparing `basicallybars-1.0.0/README.md` & `basicallybars-1.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 Yup, that's literally it. WIP; feel free
 to improve my terrible code.</p>
 
 ## Use
 
 **Import :)**
 ```
-from basicallybars import basicallybars
+import basicallybars
 ```
 
 **Create a new loading bar:**
 
 ```
 bar = basicallybars.progressbar()
 ```
```

### Comparing `basicallybars-1.0.0/pyproject.toml` & `basicallybars-1.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "basicallybars"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="Sleepy82", email="shgj7y1z@duck.com" },
 ]
 description = "A visual way to display algorithm status."
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `basicallybars-1.0.0/PKG-INFO` & `basicallybars-1.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: basicallybars
-Version: 1.0.0
+Version: 1.0.1
 Summary: A visual way to display algorithm status.
 Project-URL: Github, https://github.com/Coder2354/basicallybars/tree/master
 Author-email: Sleepy82 <shgj7y1z@duck.com>
 License-File: LICENCE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -20,15 +20,15 @@
 Yup, that's literally it. WIP; feel free
 to improve my terrible code.</p>
 
 ## Use
 
 **Import :)**
 ```
-from basicallybars import basicallybars
+import basicallybars
 ```
 
 **Create a new loading bar:**
 
 ```
 bar = basicallybars.progressbar()
 ```
```

