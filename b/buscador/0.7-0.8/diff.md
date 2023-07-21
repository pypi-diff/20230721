# Comparing `tmp/buscador-0.7.tar.gz` & `tmp/buscador-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buscador-0.7.tar", last modified: Thu Jul 20 15:52:35 2023, max compression
+gzip compressed data, was "buscador-0.8.tar", last modified: Fri Jul 21 09:38:25 2023, max compression
```

## Comparing `buscador-0.7.tar` & `buscador-0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 samcook    (501) staff       (20)        0 2023-07-20 15:52:35.071670 buscador-0.7/
--rw-r--r--   0 samcook    (501) staff       (20)     1068 2023-07-19 21:01:14.000000 buscador-0.7/LICENSE.txt
--rw-r--r--   0 samcook    (501) staff       (20)      739 2023-07-20 15:52:35.071945 buscador-0.7/PKG-INFO
--rw-r--r--   0 samcook    (501) staff       (20)      760 2023-07-20 14:43:59.000000 buscador-0.7/README.md
-drwxr-xr-x   0 samcook    (501) staff       (20)        0 2023-07-20 15:52:35.065380 buscador-0.7/buscador/
--rw-r--r--   0 samcook    (501) staff       (20)       88 2023-07-20 14:51:08.000000 buscador-0.7/buscador/__init__.py
--rw-r--r--   0 samcook    (501) staff       (20)     1213 2023-07-20 15:34:17.000000 buscador-0.7/buscador/classJsonStuff.py
--rw-r--r--   0 samcook    (501) staff       (20)     3019 2023-07-20 15:49:46.000000 buscador-0.7/buscador/classS3Stuff.py
-drwxr-xr-x   0 samcook    (501) staff       (20)        0 2023-07-20 15:52:35.070352 buscador-0.7/buscador.egg-info/
--rw-r--r--   0 samcook    (501) staff       (20)      739 2023-07-20 15:52:35.000000 buscador-0.7/buscador.egg-info/PKG-INFO
--rw-r--r--   0 samcook    (501) staff       (20)      272 2023-07-20 15:52:35.000000 buscador-0.7/buscador.egg-info/SOURCES.txt
--rw-r--r--   0 samcook    (501) staff       (20)        1 2023-07-20 15:52:35.000000 buscador-0.7/buscador.egg-info/dependency_links.txt
--rw-r--r--   0 samcook    (501) staff       (20)       25 2023-07-20 15:52:35.000000 buscador-0.7/buscador.egg-info/requires.txt
--rw-r--r--   0 samcook    (501) staff       (20)        9 2023-07-20 15:52:35.000000 buscador-0.7/buscador.egg-info/top_level.txt
--rw-r--r--   0 samcook    (501) staff       (20)       79 2023-07-20 15:52:35.072832 buscador-0.7/setup.cfg
--rw-r--r--   0 samcook    (501) staff       (20)      998 2023-07-20 15:52:19.000000 buscador-0.7/setup.py
+drwxr-xr-x   0 samcook    (501) staff       (20)        0 2023-07-21 09:38:25.782791 buscador-0.8/
+-rw-r--r--   0 samcook    (501) staff       (20)     1068 2023-07-19 21:01:14.000000 buscador-0.8/LICENSE.txt
+-rw-r--r--   0 samcook    (501) staff       (20)      739 2023-07-21 09:38:25.783177 buscador-0.8/PKG-INFO
+-rw-r--r--   0 samcook    (501) staff       (20)      760 2023-07-21 08:23:09.000000 buscador-0.8/README.md
+drwxr-xr-x   0 samcook    (501) staff       (20)        0 2023-07-21 09:38:25.777616 buscador-0.8/buscador/
+-rw-r--r--   0 samcook    (501) staff       (20)      969 2023-07-21 08:22:56.000000 buscador-0.8/buscador/JsonStuff.py
+-rw-r--r--   0 samcook    (501) staff       (20)     3019 2023-07-21 08:22:56.000000 buscador-0.8/buscador/S3Stuff.py
+-rw-r--r--   0 samcook    (501) staff       (20)      142 2023-07-21 09:36:00.000000 buscador-0.8/buscador/__init__.py
+drwxr-xr-x   0 samcook    (501) staff       (20)        0 2023-07-21 09:38:25.781799 buscador-0.8/buscador.egg-info/
+-rw-r--r--   0 samcook    (501) staff       (20)      739 2023-07-21 09:38:25.000000 buscador-0.8/buscador.egg-info/PKG-INFO
+-rw-r--r--   0 samcook    (501) staff       (20)      262 2023-07-21 09:38:25.000000 buscador-0.8/buscador.egg-info/SOURCES.txt
+-rw-r--r--   0 samcook    (501) staff       (20)        1 2023-07-21 09:38:25.000000 buscador-0.8/buscador.egg-info/dependency_links.txt
+-rw-r--r--   0 samcook    (501) staff       (20)       25 2023-07-21 09:38:25.000000 buscador-0.8/buscador.egg-info/requires.txt
+-rw-r--r--   0 samcook    (501) staff       (20)        9 2023-07-21 09:38:25.000000 buscador-0.8/buscador.egg-info/top_level.txt
+-rw-r--r--   0 samcook    (501) staff       (20)       79 2023-07-21 09:38:25.784105 buscador-0.8/setup.cfg
+-rw-r--r--   0 samcook    (501) staff       (20)      998 2023-07-21 09:37:46.000000 buscador-0.8/setup.py
```

### Comparing `buscador-0.7/LICENSE.txt` & `buscador-0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `buscador-0.7/PKG-INFO` & `buscador-0.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: buscador
-Version: 0.7
+Version: 0.8
 Summary: Just a collection of helpful tools
 Home-page: https://github.com/SamuelBCook
-Download-URL: https://github.com/SamuelBCook/buscador/archive/refs/tags/v0.7.tar.gz
+Download-URL: https://github.com/SamuelBCook/buscador/archive/refs/tags/v0.8.tar.gz
 Author: Samuel Cook
 Author-email: samcook23@hotmail.com
 License: MIT
 Keywords: tools,json,easy
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `buscador-0.7/README.md` & `buscador-0.8/README.md`

 * *Files identical despite different names*

### Comparing `buscador-0.7/buscador/classJsonStuff.py` & `buscador-0.8/buscador/JsonStuff.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,44 +1,38 @@
-class JsonStuff:
-    def __init__(self):
-        pass
+def find_keys_value(adict: dict, key: str):
+    """Returns value of a given key, even if nested
 
-    def __str__(self) -> str:
-        pass
+    Args:
+        adict (dict): target dictionary
+        key (str): target dictionary key
 
-    def find_keys_value(adict: dict, key: str):
-        """Returns value of a given key, even if nested
-
-        Args:
-            adict (dict): target dictionary
-            key (str): target dictionary key
+    Returns:
+        Value of target dictionary key
+    """
+    stack = [adict]
+    while stack:
+        d = stack.pop()
+        if key in d:
+            return d[key]
+        for v in d.values():
+            if isinstance(v, dict):
+                stack.append(v)
+            if isinstance(v, list):
+                stack += v
 
-        Returns:
-            Value of target dictionary key
-        """
-        stack = [adict]
-        while stack:
-            d = stack.pop()
-            if key in d:
-                return d[key]
-            for v in d.values():
-                if isinstance(v, dict):
-                    stack.append(v)
-                if isinstance(v, list):
-                    stack += v
 
-    def get_paths(my_dict: dict, path=None):
-        """
-        Get paths for nested keys in dictionaries.
-        Args:
-            my_dict (dict): Target dictionary.
-            path (list, optional): Defaults to None.
-        """
-        if path is None:
-            path = []
-        for k, v in my_dict.items():
-            newpath = path + [k]
-            if isinstance(v, dict):
-                for u in JsonStuff.get_paths(v, newpath):
-                    yield u
-            else:
-                yield newpath, v
+def get_paths(my_dict: dict, path=None):
+    """
+    Get paths for nested keys in dictionaries.
+    Args:
+        my_dict (dict): Target dictionary.
+        path (list, optional): Defaults to None.
+    """
+    if path is None:
+        path = []
+    for k, v in my_dict.items():
+        newpath = path + [k]
+        if isinstance(v, dict):
+            for u in get_paths(v, newpath):
+                yield u
+        else:
+            yield newpath, v
```

### Comparing `buscador-0.7/buscador/classS3Stuff.py` & `buscador-0.8/buscador/S3Stuff.py`

 * *Files identical despite different names*

### Comparing `buscador-0.7/buscador.egg-info/PKG-INFO` & `buscador-0.8/buscador.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: buscador
-Version: 0.7
+Version: 0.8
 Summary: Just a collection of helpful tools
 Home-page: https://github.com/SamuelBCook
-Download-URL: https://github.com/SamuelBCook/buscador/archive/refs/tags/v0.7.tar.gz
+Download-URL: https://github.com/SamuelBCook/buscador/archive/refs/tags/v0.8.tar.gz
 Author: Samuel Cook
 Author-email: samcook23@hotmail.com
 License: MIT
 Keywords: tools,json,easy
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `buscador-0.7/setup.py` & `buscador-0.8/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from distutils.core import setup
 
 setup(
     name="buscador",
     packages=["buscador"],
-    version="0.7",
+    version="0.8",
     license="MIT",
     description="Just a collection of helpful tools",
     author="Samuel Cook",
     author_email="samcook23@hotmail.com",
     url="https://github.com/SamuelBCook",
-    download_url="https://github.com/SamuelBCook/buscador/archive/refs/tags/v0.7.tar.gz",
+    download_url="https://github.com/SamuelBCook/buscador/archive/refs/tags/v0.8.tar.gz",
     keywords=["tools", "json", "easy"],
     install_requires=[
         "pandas",
         "boto3",
         "botocore",
         "io",
     ],
```

