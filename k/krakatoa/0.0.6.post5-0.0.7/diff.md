# Comparing `tmp/krakatoa-0.0.6.post5.tar.gz` & `tmp/krakatoa-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "krakatoa-0.0.6.post5.tar", last modified: Thu Jul 20 14:33:39 2023, max compression
+gzip compressed data, was "krakatoa-0.0.7.tar", last modified: Fri Jul 21 14:16:12 2023, max compression
```

## Comparing `krakatoa-0.0.6.post5.tar` & `krakatoa-0.0.7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:33:39.484266 krakatoa-0.0.6.post5/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-20 14:33:27.000000 krakatoa-0.0.6.post5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-07-20 14:33:39.484266 krakatoa-0.0.6.post5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-20 14:33:27.000000 krakatoa-0.0.6.post5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:33:39.480266 krakatoa-0.0.6.post5/krakatoa/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-20 14:33:27.000000 krakatoa-0.0.6.post5/krakatoa/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:33:39.484266 krakatoa-0.0.6.post5/krakatoa/future/
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-20 14:33:27.000000 krakatoa-0.0.6.post5/krakatoa/future/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13277 2023-07-20 14:33:27.000000 krakatoa-0.0.6.post5/krakatoa/future/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-20 14:33:27.000000 krakatoa-0.0.6.post5/krakatoa/future/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-07-20 14:33:27.000000 krakatoa-0.0.6.post5/krakatoa/future/experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)    12359 2023-07-20 14:33:27.000000 krakatoa-0.0.6.post5/krakatoa/future/preprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:33:39.484266 krakatoa-0.0.6.post5/krakatoa/models/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-20 14:33:27.000000 krakatoa-0.0.6.post5/krakatoa/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28354 2023-07-20 14:33:27.000000 krakatoa-0.0.6.post5/krakatoa/models/_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-07-20 14:33:27.000000 krakatoa-0.0.6.post5/krakatoa/models/_getmodels.py
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-07-20 14:33:27.000000 krakatoa-0.0.6.post5/krakatoa/models/_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    21076 2023-07-20 14:33:27.000000 krakatoa-0.0.6.post5/krakatoa/models/autotune.py
--rw-r--r--   0 runner    (1001) docker     (123)     8248 2023-07-20 14:33:27.000000 krakatoa-0.0.6.post5/krakatoa/models/quick.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:33:39.480266 krakatoa-0.0.6.post5/krakatoa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-07-20 14:33:39.000000 krakatoa-0.0.6.post5/krakatoa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-20 14:33:39.000000 krakatoa-0.0.6.post5/krakatoa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 14:33:39.000000 krakatoa-0.0.6.post5/krakatoa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-20 14:33:39.000000 krakatoa-0.0.6.post5/krakatoa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-20 14:33:39.000000 krakatoa-0.0.6.post5/krakatoa.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-20 14:33:39.484266 krakatoa-0.0.6.post5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-07-20 14:33:27.000000 krakatoa-0.0.6.post5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:16:12.974235 krakatoa-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-21 14:16:00.000000 krakatoa-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-21 14:16:12.974235 krakatoa-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-21 14:16:00.000000 krakatoa-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:16:12.974235 krakatoa-0.0.7/krakatoa/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-21 14:16:00.000000 krakatoa-0.0.7/krakatoa/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:16:12.974235 krakatoa-0.0.7/krakatoa/future/
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-21 14:16:00.000000 krakatoa-0.0.7/krakatoa/future/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13470 2023-07-21 14:16:00.000000 krakatoa-0.0.7/krakatoa/future/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-21 14:16:00.000000 krakatoa-0.0.7/krakatoa/future/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-07-21 14:16:00.000000 krakatoa-0.0.7/krakatoa/future/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12359 2023-07-21 14:16:00.000000 krakatoa-0.0.7/krakatoa/future/preprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:16:12.974235 krakatoa-0.0.7/krakatoa/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-21 14:16:00.000000 krakatoa-0.0.7/krakatoa/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28354 2023-07-21 14:16:00.000000 krakatoa-0.0.7/krakatoa/models/_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-07-21 14:16:00.000000 krakatoa-0.0.7/krakatoa/models/_getmodels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-07-21 14:16:00.000000 krakatoa-0.0.7/krakatoa/models/_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21076 2023-07-21 14:16:00.000000 krakatoa-0.0.7/krakatoa/models/autotune.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8248 2023-07-21 14:16:00.000000 krakatoa-0.0.7/krakatoa/models/quick.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:16:12.974235 krakatoa-0.0.7/krakatoa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-21 14:16:12.000000 krakatoa-0.0.7/krakatoa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-21 14:16:12.000000 krakatoa-0.0.7/krakatoa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 14:16:12.000000 krakatoa-0.0.7/krakatoa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-21 14:16:12.000000 krakatoa-0.0.7/krakatoa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-21 14:16:12.000000 krakatoa-0.0.7/krakatoa.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-21 14:16:12.974235 krakatoa-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-07-21 14:16:00.000000 krakatoa-0.0.7/setup.py
```

### Comparing `krakatoa-0.0.6.post5/LICENSE` & `krakatoa-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `krakatoa-0.0.6.post5/PKG-INFO` & `krakatoa-0.0.7/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: krakatoa
-Version: 0.0.6.post5
+Version: 0.0.7
 Summary: Machine Learning high level package.
 Home-page: https://github.com/aitec-mp/krakatoa
-Download-URL: https://github.com/aitec-mp/krakatoa/archive/refs/tags/0.0.6post5.tar.gz
+Download-URL: https://github.com/aitec-mp/krakatoa/archive/refs/tags/0.0.7.tar.gz
 Author: Matheus de Prá Andrade
 Author-email: mpandrade@ucs.br
 License: MIT
 Keywords: krakatoa,machine learning
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `krakatoa-0.0.6.post5/krakatoa/future/analysis.py` & `krakatoa-0.0.7/krakatoa/future/analysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 # ============================================================
 
 import pandas as pd
 import numpy as np
 import seaborn as sns
 from .preprocess import DataClean
 
+from sklearn.decomposition import PCA
+
 # ============================================================
 
 
 class Analytics(DataClean):
 
     def __init__(self, target=None):
         super().__init__(target)
@@ -381,7 +383,16 @@
 
         iqr = self.iqrOutliers(column, method=method)
 
         if plot:
             sns.boxplot(df, **kwargs)
 
         return iqr
+
+    def pca(self, n_components=1, **kwargs):
+
+        pca = PCA(n_components=n_components, **kwargs)
+
+        pca.fit(self.dataset)
+
+        return pca
+
```

### Comparing `krakatoa-0.0.6.post5/krakatoa/future/evaluate.py` & `krakatoa-0.0.7/krakatoa/future/evaluate.py`

 * *Files identical despite different names*

### Comparing `krakatoa-0.0.6.post5/krakatoa/future/experiment.py` & `krakatoa-0.0.7/krakatoa/future/experiment.py`

 * *Files identical despite different names*

### Comparing `krakatoa-0.0.6.post5/krakatoa/future/preprocess.py` & `krakatoa-0.0.7/krakatoa/future/preprocess.py`

 * *Files identical despite different names*

### Comparing `krakatoa-0.0.6.post5/krakatoa/models/_config.py` & `krakatoa-0.0.7/krakatoa/models/_config.py`

 * *Files identical despite different names*

### Comparing `krakatoa-0.0.6.post5/krakatoa/models/_getmodels.py` & `krakatoa-0.0.7/krakatoa/models/_getmodels.py`

 * *Files identical despite different names*

### Comparing `krakatoa-0.0.6.post5/krakatoa/models/_metrics.py` & `krakatoa-0.0.7/krakatoa/models/_metrics.py`

 * *Files identical despite different names*

### Comparing `krakatoa-0.0.6.post5/krakatoa/models/autotune.py` & `krakatoa-0.0.7/krakatoa/models/autotune.py`

 * *Files identical despite different names*

### Comparing `krakatoa-0.0.6.post5/krakatoa/models/quick.py` & `krakatoa-0.0.7/krakatoa/models/quick.py`

 * *Files identical despite different names*

### Comparing `krakatoa-0.0.6.post5/krakatoa.egg-info/PKG-INFO` & `krakatoa-0.0.7/krakatoa.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: krakatoa
-Version: 0.0.6.post5
+Version: 0.0.7
 Summary: Machine Learning high level package.
 Home-page: https://github.com/aitec-mp/krakatoa
-Download-URL: https://github.com/aitec-mp/krakatoa/archive/refs/tags/0.0.6post5.tar.gz
+Download-URL: https://github.com/aitec-mp/krakatoa/archive/refs/tags/0.0.7.tar.gz
 Author: Matheus de Prá Andrade
 Author-email: mpandrade@ucs.br
 License: MIT
 Keywords: krakatoa,machine learning
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `krakatoa-0.0.6.post5/krakatoa.egg-info/SOURCES.txt` & `krakatoa-0.0.7/krakatoa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `krakatoa-0.0.6.post5/setup.py` & `krakatoa-0.0.7/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import setup
 
 setup(
   name = 'krakatoa',       
   packages = ['krakatoa', 'krakatoa/models', 'krakatoa/future'],  
-  version = '0.0.6post5',      
+  version = '0.0.7',      
   license='MIT',        
   description = 'Machine Learning high level package.',  
   long_description='Machine Learning high level package.',  
   author = 'Matheus de Prá Andrade',              
   author_email = 'mpandrade@ucs.br',    
   url = 'https://github.com/aitec-mp/krakatoa',  
-  download_url = 'https://github.com/aitec-mp/krakatoa/archive/refs/tags/0.0.6post5.tar.gz',    
+  download_url = 'https://github.com/aitec-mp/krakatoa/archive/refs/tags/0.0.7.tar.gz',    
   keywords = ['krakatoa', 'machine learning'],  
   install_requires=[    
           'scikit-learn',
           'numpy',
           'pandas',
           'xgboost',
           'seaborn'
```

