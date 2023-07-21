# Comparing `tmp/alia-0.2.5.tar.gz` & `tmp/alia-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alia-0.2.5.tar", last modified: Fri Jul 21 16:55:27 2023, max compression
+gzip compressed data, was "alia-0.2.6.tar", last modified: Fri Jul 21 16:58:02 2023, max compression
```

## Comparing `alia-0.2.5.tar` & `alia-0.2.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 aliavictor   (502) staff       (20)        0 2023-07-21 16:55:27.806932 alia-0.2.5/
--rw-r--r--   0 aliavictor   (502) staff       (20)     1066 2023-03-23 20:16:29.000000 alia-0.2.5/LICENSE
--rw-r--r--   0 aliavictor   (502) staff       (20)      570 2023-07-21 16:55:27.806417 alia-0.2.5/PKG-INFO
--rw-r--r--   0 aliavictor   (502) staff       (20)      529 2023-04-20 21:02:49.000000 alia-0.2.5/README.md
-drwxr-xr-x   0 aliavictor   (502) staff       (20)        0 2023-07-21 16:55:27.802406 alia-0.2.5/alia/
--rw-r--r--   0 aliavictor   (502) staff       (20)        0 2023-03-23 18:58:43.000000 alia-0.2.5/alia/__init__.py
--rw-r--r--   0 aliavictor   (502) staff       (20)    17437 2023-04-19 20:09:36.000000 alia-0.2.5/alia/colors.py
--rw-r--r--   0 aliavictor   (502) staff       (20)     5598 2023-04-05 19:22:12.000000 alia-0.2.5/alia/df_tools.py
--rw-r--r--   0 aliavictor   (502) staff       (20)    29203 2023-07-21 16:53:19.000000 alia-0.2.5/alia/tools.py
-drwxr-xr-x   0 aliavictor   (502) staff       (20)        0 2023-07-21 16:55:27.805652 alia-0.2.5/alia.egg-info/
--rw-r--r--   0 aliavictor   (502) staff       (20)      570 2023-07-21 16:55:27.000000 alia-0.2.5/alia.egg-info/PKG-INFO
--rw-r--r--   0 aliavictor   (502) staff       (20)      228 2023-07-21 16:55:27.000000 alia-0.2.5/alia.egg-info/SOURCES.txt
--rw-r--r--   0 aliavictor   (502) staff       (20)        1 2023-07-21 16:55:27.000000 alia-0.2.5/alia.egg-info/dependency_links.txt
--rw-r--r--   0 aliavictor   (502) staff       (20)       94 2023-07-21 16:55:27.000000 alia-0.2.5/alia.egg-info/requires.txt
--rw-r--r--   0 aliavictor   (502) staff       (20)        5 2023-07-21 16:55:27.000000 alia-0.2.5/alia.egg-info/top_level.txt
--rw-r--r--   0 aliavictor   (502) staff       (20)       38 2023-07-21 16:55:27.807060 alia-0.2.5/setup.cfg
--rw-r--r--   0 aliavictor   (502) staff       (20)      926 2023-07-21 16:54:26.000000 alia-0.2.5/setup.py
+drwxr-xr-x   0 aliavictor   (502) staff       (20)        0 2023-07-21 16:58:02.520010 alia-0.2.6/
+-rw-r--r--   0 aliavictor   (502) staff       (20)     1066 2023-03-23 20:16:29.000000 alia-0.2.6/LICENSE
+-rw-r--r--   0 aliavictor   (502) staff       (20)      570 2023-07-21 16:58:02.519701 alia-0.2.6/PKG-INFO
+-rw-r--r--   0 aliavictor   (502) staff       (20)      529 2023-04-20 21:02:49.000000 alia-0.2.6/README.md
+drwxr-xr-x   0 aliavictor   (502) staff       (20)        0 2023-07-21 16:58:02.516814 alia-0.2.6/alia/
+-rw-r--r--   0 aliavictor   (502) staff       (20)        0 2023-03-23 18:58:43.000000 alia-0.2.6/alia/__init__.py
+-rw-r--r--   0 aliavictor   (502) staff       (20)    17437 2023-04-19 20:09:36.000000 alia-0.2.6/alia/colors.py
+-rw-r--r--   0 aliavictor   (502) staff       (20)     5598 2023-04-05 19:22:12.000000 alia-0.2.6/alia/df_tools.py
+-rw-r--r--   0 aliavictor   (502) staff       (20)    29255 2023-07-21 16:57:20.000000 alia-0.2.6/alia/tools.py
+drwxr-xr-x   0 aliavictor   (502) staff       (20)        0 2023-07-21 16:58:02.519312 alia-0.2.6/alia.egg-info/
+-rw-r--r--   0 aliavictor   (502) staff       (20)      570 2023-07-21 16:58:02.000000 alia-0.2.6/alia.egg-info/PKG-INFO
+-rw-r--r--   0 aliavictor   (502) staff       (20)      228 2023-07-21 16:58:02.000000 alia-0.2.6/alia.egg-info/SOURCES.txt
+-rw-r--r--   0 aliavictor   (502) staff       (20)        1 2023-07-21 16:58:02.000000 alia-0.2.6/alia.egg-info/dependency_links.txt
+-rw-r--r--   0 aliavictor   (502) staff       (20)       94 2023-07-21 16:58:02.000000 alia-0.2.6/alia.egg-info/requires.txt
+-rw-r--r--   0 aliavictor   (502) staff       (20)        5 2023-07-21 16:58:02.000000 alia-0.2.6/alia.egg-info/top_level.txt
+-rw-r--r--   0 aliavictor   (502) staff       (20)       38 2023-07-21 16:58:02.520104 alia-0.2.6/setup.cfg
+-rw-r--r--   0 aliavictor   (502) staff       (20)      926 2023-07-21 16:57:32.000000 alia-0.2.6/setup.py
```

### Comparing `alia-0.2.5/LICENSE` & `alia-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `alia-0.2.5/PKG-INFO` & `alia-0.2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alia
-Version: 0.2.5
+Version: 0.2.6
 Summary: A collection of random helper tools to make life easier
 Home-page: https://github.com/aliavictor/alia
 Author: Alia
 Author-email: alia.jo.victor@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `alia-0.2.5/README.md` & `alia-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `alia-0.2.5/alia/colors.py` & `alia-0.2.6/alia/colors.py`

 * *Files identical despite different names*

### Comparing `alia-0.2.5/alia/df_tools.py` & `alia-0.2.6/alia/df_tools.py`

 * *Files identical despite different names*

### Comparing `alia-0.2.5/alia/tools.py` & `alia-0.2.6/alia/tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -898,24 +898,25 @@
         prefix (str): Target files that start with this prefix
         raise_err (bool): If False FileNotFoundErrors will fail silently
 
     Returns:
         A list containing all the filenames in the given directory."""
     if ext and "." not in ext:
         ext = f".{ext.strip()}"
+    blacklist = [".DS_Store"]
 
     try:
         if ext and prefix:
             return [i for i in os.listdir(dirpath) if i.startswith(prefix) and i.endswith(ext)]
         elif ext:
             return [i for i in os.listdir(dirpath) if i.endswith(ext)]
         elif prefix:
             return [i for i in os.listdir(dirpath) if i.startswith(prefix)]
         else:
-            return [i for i in os.listdir(dirpath)]
+            return [i for i in os.listdir(dirpath) if i not in blacklist]
     except FileNotFoundError:
         if raise_err:
             raise FileNotFoundError
         else:
             red("<b>Can't locate directory</b>")
             return None
```

### Comparing `alia-0.2.5/alia.egg-info/PKG-INFO` & `alia-0.2.6/alia.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alia
-Version: 0.2.5
+Version: 0.2.6
 Summary: A collection of random helper tools to make life easier
 Home-page: https://github.com/aliavictor/alia
 Author: Alia
 Author-email: alia.jo.victor@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `alia-0.2.5/setup.py` & `alia-0.2.6/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="alia",
-    version="0.2.5",
+    version="0.2.6",
     description="A collection of random helper tools to make life easier",
     author="Alia",
     author_email="alia.jo.victor@gmail.com",
     url="https://github.com/aliavictor/alia",
     packages=find_packages(),
     install_requires=[
         # i.e. 'numpy>=1.18.0'
```

