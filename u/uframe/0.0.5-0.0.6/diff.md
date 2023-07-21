# Comparing `tmp/uframe-0.0.5.tar.gz` & `tmp/uframe-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uframe-0.0.5.tar", last modified: Thu Jul 20 14:33:44 2023, max compression
+gzip compressed data, was "uframe-0.0.6.tar", last modified: Fri Jul 21 06:52:15 2023, max compression
```

## Comparing `uframe-0.0.5.tar` & `uframe-0.0.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-20 14:33:44.578837 uframe-0.0.5/
--rw-rw-rw-   0        0        0     1090 2023-07-11 11:16:34.000000 uframe-0.0.5/LICENSE
--rw-rw-rw-   0        0        0     5081 2023-07-20 14:33:44.578837 uframe-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     4479 2023-07-11 11:16:34.000000 uframe-0.0.5/README.md
--rw-rw-rw-   0        0        0     1055 2023-07-20 14:33:01.000000 uframe-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0      462 2023-07-20 14:33:44.578837 uframe-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      223 2023-07-20 12:52:29.000000 uframe-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-20 14:33:44.545908 uframe-0.0.5/src/
-drwxrwxrwx   0        0        0        0 2023-07-20 14:33:44.563156 uframe-0.0.5/src/uframe/
--rw-rw-rw-   0        0        0      534 2023-07-11 11:16:34.000000 uframe-0.0.5/src/uframe/__init__.py
--rw-rw-rw-   0        0        0    61223 2023-07-20 11:22:06.000000 uframe-0.0.5/src/uframe/uframe.py
--rw-rw-rw-   0        0        0     7071 2023-07-20 09:00:36.000000 uframe-0.0.5/src/uframe/uframe_from_mice.py
--rw-rw-rw-   0        0        0    12958 2023-07-20 11:30:18.000000 uframe-0.0.5/src/uframe/uframe_instance.py
-drwxrwxrwx   0        0        0        0 2023-07-20 14:33:44.578837 uframe-0.0.5/src/uframe.egg-info/
--rw-rw-rw-   0        0        0     5081 2023-07-20 14:33:44.000000 uframe-0.0.5/src/uframe.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      409 2023-07-20 14:33:44.000000 uframe-0.0.5/src/uframe.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-20 14:33:44.000000 uframe-0.0.5/src/uframe.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-20 07:40:14.000000 uframe-0.0.5/src/uframe.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      142 2023-07-20 14:33:44.000000 uframe-0.0.5/src/uframe.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-20 14:33:44.000000 uframe-0.0.5/src/uframe.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-20 14:33:44.578837 uframe-0.0.5/tests/
--rw-rw-rw-   0        0        0      224 2023-07-11 11:16:34.000000 uframe-0.0.5/tests/test_uframe.py
--rw-rw-rw-   0        0        0     2703 2023-07-11 11:16:34.000000 uframe-0.0.5/tests/test_uframe_instance.py
+drwxrwxrwx   0        0        0        0 2023-07-21 06:52:15.364549 uframe-0.0.6/
+-rw-rw-rw-   0        0        0     1090 2023-07-11 11:16:34.000000 uframe-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0     5081 2023-07-21 06:52:15.365549 uframe-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     4479 2023-07-11 11:16:34.000000 uframe-0.0.6/README.md
+-rw-rw-rw-   0        0        0     1055 2023-07-21 06:51:42.000000 uframe-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0      462 2023-07-21 06:52:15.366549 uframe-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      223 2023-07-20 12:52:29.000000 uframe-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 06:52:15.313549 uframe-0.0.6/src/
+drwxrwxrwx   0        0        0        0 2023-07-21 06:52:15.325549 uframe-0.0.6/src/uframe/
+-rw-rw-rw-   0        0        0      534 2023-07-11 11:16:34.000000 uframe-0.0.6/src/uframe/__init__.py
+-rw-rw-rw-   0        0        0    61223 2023-07-20 11:22:06.000000 uframe-0.0.6/src/uframe/uframe.py
+-rw-rw-rw-   0        0        0     7115 2023-07-20 15:56:21.000000 uframe-0.0.6/src/uframe/uframe_from_mice.py
+-rw-rw-rw-   0        0        0    12958 2023-07-20 11:30:18.000000 uframe-0.0.6/src/uframe/uframe_instance.py
+drwxrwxrwx   0        0        0        0 2023-07-21 06:52:15.349549 uframe-0.0.6/src/uframe.egg-info/
+-rw-rw-rw-   0        0        0     5081 2023-07-21 06:52:15.000000 uframe-0.0.6/src/uframe.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      409 2023-07-21 06:52:15.000000 uframe-0.0.6/src/uframe.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 06:52:15.000000 uframe-0.0.6/src/uframe.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-20 07:40:14.000000 uframe-0.0.6/src/uframe.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      142 2023-07-21 06:52:15.000000 uframe-0.0.6/src/uframe.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-21 06:52:15.000000 uframe-0.0.6/src/uframe.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-21 06:52:15.363566 uframe-0.0.6/tests/
+-rw-rw-rw-   0        0        0      224 2023-07-11 11:16:34.000000 uframe-0.0.6/tests/test_uframe.py
+-rw-rw-rw-   0        0        0     2703 2023-07-11 11:16:34.000000 uframe-0.0.6/tests/test_uframe_instance.py
```

### Comparing `uframe-0.0.5/LICENSE` & `uframe-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `uframe-0.0.5/PKG-INFO` & `uframe-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uframe
-Version: 0.0.5
+Version: 0.0.6
 Summary: Package for handling uncertain data
 Author: Christian Amesoeder and Michael Hagn
 Author-email: Christian Amesoder <christian.amesoeder@informatik.uni-regensburg.de>, Michael Hagn <michael.hagn@stud.uni-regensburg.de>
 Project-URL: Homepage, https://github.com/URWI2/uframe
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `uframe-0.0.5/README.md` & `uframe-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `uframe-0.0.5/pyproject.toml` & `uframe-0.0.6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 warn_unreachable = true
 warn_unused_configs = true
 no_implicit_reexport = true
 
 
 [project]
 name = "uframe"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Christian Amesoder", email="christian.amesoeder@informatik.uni-regensburg.de" },
   { name="Michael Hagn", email="michael.hagn@stud.uni-regensburg.de" }
 ]
 description = "Package for handling uncertain data"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `uframe-0.0.5/src/uframe/__init__.py` & `uframe-0.0.6/src/uframe/__init__.py`

 * *Files identical despite different names*

### Comparing `uframe-0.0.5/src/uframe/uframe.py` & `uframe-0.0.6/src/uframe/uframe.py`

 * *Files identical despite different names*

### Comparing `uframe-0.0.5/src/uframe/uframe_from_mice.py` & `uframe-0.0.6/src/uframe/uframe_from_mice.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,34 +79,35 @@
     return u
 
 
 
 def generate_missing_values(complete_data, p):
     shape = complete_data.shape
     y = complete_data.copy()
+    np.random.seed(seed)
     missing = np.random.binomial(1, p, shape)
     
     y[missing.astype('bool')] = np.nan
     return y, missing
 
 
 def uframe_from_array_mice_2(a: np.ndarray, p=0.1, mice_iterations=5, kernel="stats.gaussian_kde",
-                           scaler= "min_max", cat_indices=[], **kwargs):
+                           scaler= "min_max", cat_indices=[],seed = None, **kwargs):
 
-    x, missing = generate_missing_values(a, p)
+    x, missing = generate_missing_values(a, p,seed)
 
     distr = {}
     cat_distr = {}
     index_dict={}
 
     # train mice imputation correctly
     kds = mf.ImputationKernel(
         x,
         save_all_iterations=True,
-        random_state=100)
+        random_state=seed)
 
     kds.mice(mice_iterations)
     for i in range(x.shape[0]):
         # print("Line", i)
         imp_distr = None
         imp_arrays = []
         cat_distributions = []
```

### Comparing `uframe-0.0.5/src/uframe/uframe_instance.py` & `uframe-0.0.6/src/uframe/uframe_instance.py`

 * *Files identical despite different names*

### Comparing `uframe-0.0.5/src/uframe.egg-info/PKG-INFO` & `uframe-0.0.6/src/uframe.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uframe
-Version: 0.0.5
+Version: 0.0.6
 Summary: Package for handling uncertain data
 Author: Christian Amesoeder and Michael Hagn
 Author-email: Christian Amesoder <christian.amesoeder@informatik.uni-regensburg.de>, Michael Hagn <michael.hagn@stud.uni-regensburg.de>
 Project-URL: Homepage, https://github.com/URWI2/uframe
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `uframe-0.0.5/tests/test_uframe_instance.py` & `uframe-0.0.6/tests/test_uframe_instance.py`

 * *Files identical despite different names*

