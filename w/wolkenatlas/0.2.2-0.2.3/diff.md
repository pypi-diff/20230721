# Comparing `tmp/wolkenatlas-0.2.2.tar.gz` & `tmp/wolkenatlas-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wolkenatlas-0.2.2.tar", last modified: Wed May 10 19:26:04 2023, max compression
+gzip compressed data, was "wolkenatlas-0.2.3.tar", last modified: Fri Jul 21 06:45:14 2023, max compression
```

## Comparing `wolkenatlas-0.2.2.tar` & `wolkenatlas-0.2.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 tkober     (502) staff       (20)        0 2023-05-10 19:26:04.476186 wolkenatlas-0.2.2/
--rw-r--r--   0 tkober     (502) staff       (20)     1063 2022-05-13 10:09:18.000000 wolkenatlas-0.2.2/LICENSE
--rw-r--r--   0 tkober     (502) staff       (20)       58 2022-07-15 11:38:43.000000 wolkenatlas-0.2.2/MANIFEST.in
--rw-r--r--   0 tkober     (502) staff       (20)     3229 2023-05-10 19:26:04.475942 wolkenatlas-0.2.2/PKG-INFO
--rw-r--r--   0 tkober     (502) staff       (20)     1113 2022-07-15 11:38:43.000000 wolkenatlas-0.2.2/Readme.md
--rw-r--r--   0 tkober     (502) staff       (20)      730 2023-05-10 18:57:49.000000 wolkenatlas-0.2.2/pyproject.toml
--rw-r--r--   0 tkober     (502) staff       (20)       38 2023-05-10 19:26:04.476250 wolkenatlas-0.2.2/setup.cfg
--rw-r--r--   0 tkober     (502) staff       (20)     3147 2023-05-10 18:58:17.000000 wolkenatlas-0.2.2/setup.py
-drwxr-xr-x   0 tkober     (502) staff       (20)        0 2023-05-10 19:26:04.471442 wolkenatlas-0.2.2/wolkenatlas/
--rw-r--r--   0 tkober     (502) staff       (20)       69 2022-05-13 10:09:18.000000 wolkenatlas-0.2.2/wolkenatlas/__init__.py
--rw-r--r--   0 tkober     (502) staff       (20)     1391 2023-05-10 13:05:08.000000 wolkenatlas-0.2.2/wolkenatlas/constants.py
--rw-r--r--   0 tkober     (502) staff       (20)     6332 2022-05-13 10:09:18.000000 wolkenatlas-0.2.2/wolkenatlas/download.py
--rw-r--r--   0 tkober     (502) staff       (20)    10278 2023-05-10 19:21:39.000000 wolkenatlas-0.2.2/wolkenatlas/embedding.py
--rw-r--r--   0 tkober     (502) staff       (20)     1849 2022-05-16 18:14:21.000000 wolkenatlas-0.2.2/wolkenatlas/encoder.py
--rw-r--r--   0 tkober     (502) staff       (20)     4682 2022-05-18 08:23:47.000000 wolkenatlas-0.2.2/wolkenatlas/preprocessing.py
-drwxr-xr-x   0 tkober     (502) staff       (20)        0 2023-05-10 19:26:04.475399 wolkenatlas-0.2.2/wolkenatlas/util/
--rw-r--r--   0 tkober     (502) staff       (20)        0 2022-05-13 10:09:18.000000 wolkenatlas-0.2.2/wolkenatlas/util/__init__.py
--rw-r--r--   0 tkober     (502) staff       (20)     6219 2023-05-10 09:45:18.000000 wolkenatlas-0.2.2/wolkenatlas/util/data_processing.py
--rw-r--r--   0 tkober     (502) staff       (20)     2249 2022-09-08 14:46:14.000000 wolkenatlas-0.2.2/wolkenatlas/util/file_processing.py
-drwxr-xr-x   0 tkober     (502) staff       (20)        0 2023-05-10 19:26:04.474146 wolkenatlas-0.2.2/wolkenatlas.egg-info/
--rw-r--r--   0 tkober     (502) staff       (20)     3229 2023-05-10 19:26:04.000000 wolkenatlas-0.2.2/wolkenatlas.egg-info/PKG-INFO
--rw-r--r--   0 tkober     (502) staff       (20)      516 2023-05-10 19:26:04.000000 wolkenatlas-0.2.2/wolkenatlas.egg-info/SOURCES.txt
--rw-r--r--   0 tkober     (502) staff       (20)        1 2023-05-10 19:26:04.000000 wolkenatlas-0.2.2/wolkenatlas.egg-info/dependency_links.txt
--rw-r--r--   0 tkober     (502) staff       (20)       39 2023-05-10 19:26:04.000000 wolkenatlas-0.2.2/wolkenatlas.egg-info/entry_points.txt
--rw-r--r--   0 tkober     (502) staff       (20)       53 2023-05-10 19:26:04.000000 wolkenatlas-0.2.2/wolkenatlas.egg-info/requires.txt
--rw-r--r--   0 tkober     (502) staff       (20)       12 2023-05-10 19:26:04.000000 wolkenatlas-0.2.2/wolkenatlas.egg-info/top_level.txt
+drwxr-xr-x   0 tkober     (502) staff       (20)        0 2023-07-21 06:45:14.936842 wolkenatlas-0.2.3/
+-rw-r--r--   0 tkober     (502) staff       (20)     1063 2022-05-13 10:09:18.000000 wolkenatlas-0.2.3/LICENSE
+-rw-r--r--   0 tkober     (502) staff       (20)       58 2022-07-15 11:38:43.000000 wolkenatlas-0.2.3/MANIFEST.in
+-rw-r--r--   0 tkober     (502) staff       (20)     3229 2023-07-21 06:45:14.936617 wolkenatlas-0.2.3/PKG-INFO
+-rw-r--r--   0 tkober     (502) staff       (20)     1113 2022-07-15 11:38:43.000000 wolkenatlas-0.2.3/Readme.md
+-rw-r--r--   0 tkober     (502) staff       (20)      730 2023-07-21 06:37:56.000000 wolkenatlas-0.2.3/pyproject.toml
+-rw-r--r--   0 tkober     (502) staff       (20)       38 2023-07-21 06:45:14.936892 wolkenatlas-0.2.3/setup.cfg
+-rw-r--r--   0 tkober     (502) staff       (20)     3147 2023-07-21 06:40:22.000000 wolkenatlas-0.2.3/setup.py
+drwxr-xr-x   0 tkober     (502) staff       (20)        0 2023-07-21 06:45:14.931727 wolkenatlas-0.2.3/wolkenatlas/
+-rw-r--r--   0 tkober     (502) staff       (20)       69 2022-05-13 10:09:18.000000 wolkenatlas-0.2.3/wolkenatlas/__init__.py
+-rw-r--r--   0 tkober     (502) staff       (20)     1391 2023-05-10 13:05:08.000000 wolkenatlas-0.2.3/wolkenatlas/constants.py
+-rw-r--r--   0 tkober     (502) staff       (20)     6332 2022-05-13 10:09:18.000000 wolkenatlas-0.2.3/wolkenatlas/download.py
+-rw-r--r--   0 tkober     (502) staff       (20)    10285 2023-07-21 06:37:56.000000 wolkenatlas-0.2.3/wolkenatlas/embedding.py
+-rw-r--r--   0 tkober     (502) staff       (20)     1849 2022-05-16 18:14:21.000000 wolkenatlas-0.2.3/wolkenatlas/encoder.py
+-rw-r--r--   0 tkober     (502) staff       (20)     4682 2022-05-18 08:23:47.000000 wolkenatlas-0.2.3/wolkenatlas/preprocessing.py
+drwxr-xr-x   0 tkober     (502) staff       (20)        0 2023-07-21 06:45:14.935941 wolkenatlas-0.2.3/wolkenatlas/util/
+-rw-r--r--   0 tkober     (502) staff       (20)        0 2022-05-13 10:09:18.000000 wolkenatlas-0.2.3/wolkenatlas/util/__init__.py
+-rw-r--r--   0 tkober     (502) staff       (20)     6219 2023-05-10 09:45:18.000000 wolkenatlas-0.2.3/wolkenatlas/util/data_processing.py
+-rw-r--r--   0 tkober     (502) staff       (20)     2249 2022-09-08 14:46:14.000000 wolkenatlas-0.2.3/wolkenatlas/util/file_processing.py
+drwxr-xr-x   0 tkober     (502) staff       (20)        0 2023-07-21 06:45:14.934414 wolkenatlas-0.2.3/wolkenatlas.egg-info/
+-rw-r--r--   0 tkober     (502) staff       (20)     3229 2023-07-21 06:45:14.000000 wolkenatlas-0.2.3/wolkenatlas.egg-info/PKG-INFO
+-rw-r--r--   0 tkober     (502) staff       (20)      516 2023-07-21 06:45:14.000000 wolkenatlas-0.2.3/wolkenatlas.egg-info/SOURCES.txt
+-rw-r--r--   0 tkober     (502) staff       (20)        1 2023-07-21 06:45:14.000000 wolkenatlas-0.2.3/wolkenatlas.egg-info/dependency_links.txt
+-rw-r--r--   0 tkober     (502) staff       (20)       39 2023-07-21 06:45:14.000000 wolkenatlas-0.2.3/wolkenatlas.egg-info/entry_points.txt
+-rw-r--r--   0 tkober     (502) staff       (20)       53 2023-07-21 06:45:14.000000 wolkenatlas-0.2.3/wolkenatlas.egg-info/requires.txt
+-rw-r--r--   0 tkober     (502) staff       (20)       12 2023-07-21 06:45:14.000000 wolkenatlas-0.2.3/wolkenatlas.egg-info/top_level.txt
```

### Comparing `wolkenatlas-0.2.2/LICENSE` & `wolkenatlas-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `wolkenatlas-0.2.2/PKG-INFO` & `wolkenatlas-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wolkenatlas
-Version: 0.2.2
+Version: 0.2.3
 Summary: NLP embedding wrapper
 Home-page: https://github.com/tttthomasssss/wolkenatlas
 Author: Thomas Kober
 Author-email: Thomas Kober <tttthomasssss@gmail.com>
 License: MIT License
         
         Copyright (c) 2020 Thomas
```

### Comparing `wolkenatlas-0.2.2/Readme.md` & `wolkenatlas-0.2.3/Readme.md`

 * *Files identical despite different names*

### Comparing `wolkenatlas-0.2.2/pyproject.toml` & `wolkenatlas-0.2.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "wolkenatlas"
-version = "0.2.2"
+version = "0.2.3"
 authors = [
   { name="Thomas Kober", email="tttthomasssss@gmail.com" },
 ]
 description = "NLP embedding wrapper"
 readme = "Readme.md"
 license = { file="LICENSE" }
 requires-python = ">=3.8"
```

### Comparing `wolkenatlas-0.2.2/setup.py` & `wolkenatlas-0.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 setup(
 	name='wolkenatlas',
 
 	# Versions should comply with PEP440.  For a discussion on single-sourcing
 	# the version across setup.py and the project code, see
 	# https://packaging.python.org/en/latest/single_source_version.html
-	version='0.2.2',
+	version='0.2.3',
 
 	description='NLP embedding wrapper',
 	long_description=long_description,
 
 	# The project's main homepage.
 	url='https://github.com/tttthomasssss/wolkenatlas',
```

### Comparing `wolkenatlas-0.2.2/wolkenatlas/constants.py` & `wolkenatlas-0.2.3/wolkenatlas/constants.py`

 * *Files identical despite different names*

### Comparing `wolkenatlas-0.2.2/wolkenatlas/download.py` & `wolkenatlas-0.2.3/wolkenatlas/download.py`

 * *Files identical despite different names*

### Comparing `wolkenatlas-0.2.2/wolkenatlas/embedding.py` & `wolkenatlas-0.2.3/wolkenatlas/embedding.py`

 * *Files 0% similar despite different names*

```diff
@@ -148,15 +148,15 @@
     def __contains__(self, word):
         return word in self.inverted_index_
 
     def __index__(self, word):
         return self.inverted_index_[word]
 
     def __getitem__(self, word, default=None):
-        if isinstance(word, np.ndarray):
+        if isinstance(word, (int, np.ndarray)):
             return self.fn_getitem_by_index_(index=word)
         else:
             return self.fn_getitem_(word=word, default=default)
 
     def _get_item_by_index_single_embedding(self, index):
         return self.vector_space_[index]
```

### Comparing `wolkenatlas-0.2.2/wolkenatlas/encoder.py` & `wolkenatlas-0.2.3/wolkenatlas/encoder.py`

 * *Files identical despite different names*

### Comparing `wolkenatlas-0.2.2/wolkenatlas/preprocessing.py` & `wolkenatlas-0.2.3/wolkenatlas/preprocessing.py`

 * *Files identical despite different names*

### Comparing `wolkenatlas-0.2.2/wolkenatlas/util/data_processing.py` & `wolkenatlas-0.2.3/wolkenatlas/util/data_processing.py`

 * *Files identical despite different names*

### Comparing `wolkenatlas-0.2.2/wolkenatlas/util/file_processing.py` & `wolkenatlas-0.2.3/wolkenatlas/util/file_processing.py`

 * *Files identical despite different names*

### Comparing `wolkenatlas-0.2.2/wolkenatlas.egg-info/PKG-INFO` & `wolkenatlas-0.2.3/wolkenatlas.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wolkenatlas
-Version: 0.2.2
+Version: 0.2.3
 Summary: NLP embedding wrapper
 Home-page: https://github.com/tttthomasssss/wolkenatlas
 Author: Thomas Kober
 Author-email: Thomas Kober <tttthomasssss@gmail.com>
 License: MIT License
         
         Copyright (c) 2020 Thomas
```

### Comparing `wolkenatlas-0.2.2/wolkenatlas.egg-info/SOURCES.txt` & `wolkenatlas-0.2.3/wolkenatlas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

