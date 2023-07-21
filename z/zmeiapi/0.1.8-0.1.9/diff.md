# Comparing `tmp/zmeiapi-0.1.8.tar.gz` & `tmp/zmeiapi-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zmeiapi-0.1.8.tar", last modified: Tue Apr 11 11:55:26 2023, max compression
+gzip compressed data, was "zmeiapi-0.1.9.tar", last modified: Tue Jun 13 08:06:53 2023, max compression
```

## Comparing `zmeiapi-0.1.8.tar` & `zmeiapi-0.1.9.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-04-11 11:55:26.468235 zmeiapi-0.1.8/
--rw-rw-r--   0 vlad      (1000) vlad      (1000)     1101 2023-03-06 08:13:19.000000 zmeiapi-0.1.8/LICENSE.txt
--rw-rw-r--   0 vlad      (1000) vlad      (1000)       27 2023-03-16 01:03:53.000000 zmeiapi-0.1.8/MANIFEST.in
--rw-rw-r--   0 vlad      (1000) vlad      (1000)      386 2023-04-11 11:55:26.468235 zmeiapi-0.1.8/PKG-INFO
--rw-rw-r--   0 vlad      (1000) vlad      (1000)        6 2023-03-06 09:47:27.000000 zmeiapi-0.1.8/README.md
--rw-rw-r--   0 vlad      (1000) vlad      (1000)       38 2023-04-11 11:55:26.468235 zmeiapi-0.1.8/setup.cfg
--rw-rw-r--   0 vlad      (1000) vlad      (1000)      816 2023-04-11 11:55:08.000000 zmeiapi-0.1.8/setup.py
-drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-04-11 11:55:26.468235 zmeiapi-0.1.8/zmeiapi/
--rw-rw-r--   0 vlad      (1000) vlad      (1000)        0 2023-03-14 01:28:36.000000 zmeiapi-0.1.8/zmeiapi/__init__.py
-drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-04-11 11:55:26.468235 zmeiapi-0.1.8/zmeiapi/abstract_factories/
--rw-rw-r--   0 vlad      (1000) vlad      (1000)     1176 2023-03-31 09:50:59.000000 zmeiapi-0.1.8/zmeiapi/abstract_factories/MaterialCreators.py
--rw-rw-r--   0 vlad      (1000) vlad      (1000)     1897 2023-04-11 11:45:05.000000 zmeiapi-0.1.8/zmeiapi/abstract_factories/PinCreators.py
--rw-rw-r--   0 vlad      (1000) vlad      (1000)        0 2023-03-16 00:25:17.000000 zmeiapi-0.1.8/zmeiapi/abstract_factories/__init__.py
-drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-04-11 11:55:26.468235 zmeiapi-0.1.8/zmeiapi/data/
--rw-rw-r--   0 vlad      (1000) vlad      (1000)      122 2023-03-16 00:55:33.000000 zmeiapi-0.1.8/zmeiapi/data/Parameters.py
--rw-rw-r--   0 vlad      (1000) vlad      (1000)        0 2023-03-16 00:24:05.000000 zmeiapi-0.1.8/zmeiapi/data/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12439 2022-12-17 12:37:40.000000 zmeiapi-0.1.8/zmeiapi/data/nuclides_dict.pkl
-drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-04-11 11:55:26.468235 zmeiapi-0.1.8/zmeiapi/factories/
--rw-rw-r--   0 vlad      (1000) vlad      (1000)        0 2023-03-16 16:32:21.000000 zmeiapi-0.1.8/zmeiapi/factories/__init__.py
-drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-04-11 11:55:26.468235 zmeiapi-0.1.8/zmeiapi/objects/
--rw-rw-r--   0 vlad      (1000) vlad      (1000)     1718 2023-04-11 11:54:57.000000 zmeiapi-0.1.8/zmeiapi/objects/BurnupInput.py
--rw-rw-r--   0 vlad      (1000) vlad      (1000)     3266 2023-04-11 08:49:11.000000 zmeiapi-0.1.8/zmeiapi/objects/Cell.py
--rw-rw-r--   0 vlad      (1000) vlad      (1000)     5987 2023-04-10 14:28:31.000000 zmeiapi-0.1.8/zmeiapi/objects/General.py
--rw-rw-r--   0 vlad      (1000) vlad      (1000)     7338 2023-04-04 13:14:05.000000 zmeiapi-0.1.8/zmeiapi/objects/Lattice.py
--rw-rw-r--   0 vlad      (1000) vlad      (1000)     7856 2023-04-07 08:21:07.000000 zmeiapi-0.1.8/zmeiapi/objects/Material.py
--rw-rw-r--   0 vlad      (1000) vlad      (1000)     3383 2023-04-07 08:21:07.000000 zmeiapi-0.1.8/zmeiapi/objects/Pin.py
--rw-rw-r--   0 vlad      (1000) vlad      (1000)     5532 2023-04-07 13:50:01.000000 zmeiapi-0.1.8/zmeiapi/objects/Surface.py
--rw-rw-r--   0 vlad      (1000) vlad      (1000)        0 2023-03-16 00:21:40.000000 zmeiapi-0.1.8/zmeiapi/objects/__init__.py
-drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-04-11 11:55:26.468235 zmeiapi-0.1.8/zmeiapi/readers/
--rw-rw-r--   0 vlad      (1000) vlad      (1000)     4486 2023-03-31 09:50:59.000000 zmeiapi-0.1.8/zmeiapi/readers/BumatReader.py
--rw-rw-r--   0 vlad      (1000) vlad      (1000)     3243 2023-03-31 09:50:59.000000 zmeiapi-0.1.8/zmeiapi/readers/SerpentOut.py
--rw-rw-r--   0 vlad      (1000) vlad      (1000)        0 2023-03-16 00:23:53.000000 zmeiapi-0.1.8/zmeiapi/readers/__init__.py
-drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-04-11 11:55:26.468235 zmeiapi-0.1.8/zmeiapi/utilities/
--rw-rw-r--   0 vlad      (1000) vlad      (1000)        0 2023-03-16 16:36:15.000000 zmeiapi-0.1.8/zmeiapi/utilities/__init__.py
-drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-04-11 11:55:26.468235 zmeiapi-0.1.8/zmeiapi/zmei_io/
--rw-rw-r--   0 vlad      (1000) vlad      (1000)      459 2023-03-07 14:08:13.000000 zmeiapi-0.1.8/zmeiapi/zmei_io/Logger.py
--rw-rw-r--   0 vlad      (1000) vlad      (1000)        0 2023-03-16 00:26:06.000000 zmeiapi-0.1.8/zmeiapi/zmei_io/__init__.py
-drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-04-11 11:55:26.468235 zmeiapi-0.1.8/zmeiapi.egg-info/
--rw-rw-r--   0 vlad      (1000) vlad      (1000)      386 2023-04-11 11:55:26.000000 zmeiapi-0.1.8/zmeiapi.egg-info/PKG-INFO
--rw-rw-r--   0 vlad      (1000) vlad      (1000)      815 2023-04-11 11:55:26.000000 zmeiapi-0.1.8/zmeiapi.egg-info/SOURCES.txt
--rw-rw-r--   0 vlad      (1000) vlad      (1000)        1 2023-04-11 11:55:26.000000 zmeiapi-0.1.8/zmeiapi.egg-info/dependency_links.txt
--rw-rw-r--   0 vlad      (1000) vlad      (1000)        8 2023-04-11 11:55:26.000000 zmeiapi-0.1.8/zmeiapi.egg-info/top_level.txt
+drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-06-13 08:06:53.529500 zmeiapi-0.1.9/
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)     1101 2023-03-06 08:13:19.000000 zmeiapi-0.1.9/LICENSE.txt
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)       27 2023-03-16 01:03:53.000000 zmeiapi-0.1.9/MANIFEST.in
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)      386 2023-06-13 08:06:53.529500 zmeiapi-0.1.9/PKG-INFO
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)        6 2023-03-06 09:47:27.000000 zmeiapi-0.1.9/README.md
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)       38 2023-06-13 08:06:53.529500 zmeiapi-0.1.9/setup.cfg
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)      816 2023-06-13 08:06:24.000000 zmeiapi-0.1.9/setup.py
+drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-06-13 08:06:53.529500 zmeiapi-0.1.9/zmeiapi/
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)        0 2023-03-14 01:28:36.000000 zmeiapi-0.1.9/zmeiapi/__init__.py
+drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-06-13 08:06:53.529500 zmeiapi-0.1.9/zmeiapi/abstract_factories/
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)     1176 2023-03-31 09:50:59.000000 zmeiapi-0.1.9/zmeiapi/abstract_factories/MaterialCreators.py
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)     1897 2023-04-11 11:45:05.000000 zmeiapi-0.1.9/zmeiapi/abstract_factories/PinCreators.py
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)        0 2023-03-16 00:25:17.000000 zmeiapi-0.1.9/zmeiapi/abstract_factories/__init__.py
+drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-06-13 08:06:53.529500 zmeiapi-0.1.9/zmeiapi/data/
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)      122 2023-03-16 00:55:33.000000 zmeiapi-0.1.9/zmeiapi/data/Parameters.py
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)        0 2023-03-16 00:24:05.000000 zmeiapi-0.1.9/zmeiapi/data/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12439 2022-12-17 12:37:40.000000 zmeiapi-0.1.9/zmeiapi/data/nuclides_dict.pkl
+drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-06-13 08:06:53.529500 zmeiapi-0.1.9/zmeiapi/factories/
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)        0 2023-03-16 16:32:21.000000 zmeiapi-0.1.9/zmeiapi/factories/__init__.py
+drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-06-13 08:06:53.529500 zmeiapi-0.1.9/zmeiapi/objects/
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)     1718 2023-04-11 11:54:57.000000 zmeiapi-0.1.9/zmeiapi/objects/BurnupInput.py
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)     3266 2023-04-11 08:49:11.000000 zmeiapi-0.1.9/zmeiapi/objects/Cell.py
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)     5987 2023-04-10 14:28:31.000000 zmeiapi-0.1.9/zmeiapi/objects/General.py
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)     7338 2023-04-04 13:14:05.000000 zmeiapi-0.1.9/zmeiapi/objects/Lattice.py
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)     7856 2023-04-07 08:21:07.000000 zmeiapi-0.1.9/zmeiapi/objects/Material.py
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)     3383 2023-04-07 08:21:07.000000 zmeiapi-0.1.9/zmeiapi/objects/Pin.py
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)     5532 2023-04-07 13:50:01.000000 zmeiapi-0.1.9/zmeiapi/objects/Surface.py
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)        0 2023-03-16 00:21:40.000000 zmeiapi-0.1.9/zmeiapi/objects/__init__.py
+drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-06-13 08:06:53.529500 zmeiapi-0.1.9/zmeiapi/readers/
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)     4486 2023-03-31 09:50:59.000000 zmeiapi-0.1.9/zmeiapi/readers/BumatReader.py
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)     3327 2023-06-13 08:06:06.000000 zmeiapi-0.1.9/zmeiapi/readers/SerpentOut.py
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)        0 2023-03-16 00:23:53.000000 zmeiapi-0.1.9/zmeiapi/readers/__init__.py
+drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-06-13 08:06:53.529500 zmeiapi-0.1.9/zmeiapi/utilities/
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)        0 2023-03-16 16:36:15.000000 zmeiapi-0.1.9/zmeiapi/utilities/__init__.py
+drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-06-13 08:06:53.529500 zmeiapi-0.1.9/zmeiapi/zmei_io/
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)      459 2023-03-07 14:08:13.000000 zmeiapi-0.1.9/zmeiapi/zmei_io/Logger.py
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)        0 2023-03-16 00:26:06.000000 zmeiapi-0.1.9/zmeiapi/zmei_io/__init__.py
+drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-06-13 08:06:53.529500 zmeiapi-0.1.9/zmeiapi.egg-info/
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)      386 2023-06-13 08:06:53.000000 zmeiapi-0.1.9/zmeiapi.egg-info/PKG-INFO
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)      815 2023-06-13 08:06:53.000000 zmeiapi-0.1.9/zmeiapi.egg-info/SOURCES.txt
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)        1 2023-06-13 08:06:53.000000 zmeiapi-0.1.9/zmeiapi.egg-info/dependency_links.txt
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)        8 2023-06-13 08:06:53.000000 zmeiapi-0.1.9/zmeiapi.egg-info/top_level.txt
```

### Comparing `zmeiapi-0.1.8/LICENSE.txt` & `zmeiapi-0.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zmeiapi-0.1.8/setup.py` & `zmeiapi-0.1.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     README = readme_file.read()
 
 with open('HISTORY.md') as history_file:
     HISTORY = history_file.read()
 
 setup_args = dict(
     name='zmeiapi',
-    version='0.1.8',
+    version='0.1.9',
     description='Useful tools to work with Zmei calculation code',
     long_description_content_type="text/markdown",
     long_description=README + '\n\n' + HISTORY,
     license='MIT',
     packages=find_packages(),
     include_package_data = True,
     author='Vladislav Romanenko',
```

### Comparing `zmeiapi-0.1.8/zmeiapi/abstract_factories/MaterialCreators.py` & `zmeiapi-0.1.9/zmeiapi/abstract_factories/MaterialCreators.py`

 * *Files identical despite different names*

### Comparing `zmeiapi-0.1.8/zmeiapi/abstract_factories/PinCreators.py` & `zmeiapi-0.1.9/zmeiapi/abstract_factories/PinCreators.py`

 * *Files identical despite different names*

### Comparing `zmeiapi-0.1.8/zmeiapi/data/nuclides_dict.pkl` & `zmeiapi-0.1.9/zmeiapi/data/nuclides_dict.pkl`

 * *Files identical despite different names*

### Comparing `zmeiapi-0.1.8/zmeiapi/objects/BurnupInput.py` & `zmeiapi-0.1.9/zmeiapi/objects/BurnupInput.py`

 * *Files identical despite different names*

### Comparing `zmeiapi-0.1.8/zmeiapi/objects/Cell.py` & `zmeiapi-0.1.9/zmeiapi/objects/Cell.py`

 * *Files identical despite different names*

### Comparing `zmeiapi-0.1.8/zmeiapi/objects/General.py` & `zmeiapi-0.1.9/zmeiapi/objects/General.py`

 * *Files identical despite different names*

### Comparing `zmeiapi-0.1.8/zmeiapi/objects/Lattice.py` & `zmeiapi-0.1.9/zmeiapi/objects/Lattice.py`

 * *Files identical despite different names*

### Comparing `zmeiapi-0.1.8/zmeiapi/objects/Material.py` & `zmeiapi-0.1.9/zmeiapi/objects/Material.py`

 * *Files identical despite different names*

### Comparing `zmeiapi-0.1.8/zmeiapi/objects/Pin.py` & `zmeiapi-0.1.9/zmeiapi/objects/Pin.py`

 * *Files identical despite different names*

### Comparing `zmeiapi-0.1.8/zmeiapi/objects/Surface.py` & `zmeiapi-0.1.9/zmeiapi/objects/Surface.py`

 * *Files identical despite different names*

### Comparing `zmeiapi-0.1.8/zmeiapi/readers/BumatReader.py` & `zmeiapi-0.1.9/zmeiapi/readers/BumatReader.py`

 * *Files identical despite different names*

### Comparing `zmeiapi-0.1.8/zmeiapi/readers/SerpentOut.py` & `zmeiapi-0.1.9/zmeiapi/readers/SerpentOut.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,14 +23,17 @@
             'INF_S0': [],
             'CMM_DIFFCOEF ': [],
             'INF_I135_YIELD': [],
             'INF_XE135_YIELD': [],
             'INF_PM149_YIELD': [],
             'INF_XE135_MICRO_ABS': [],
             'INF_SM149_MICRO_ABS': [],
+            'INF_CHIT': [],
+            'INF_CHIP': [],
+            'INF_CHID': [],
             'INF_INVV': [],
             'BETA_EFF': [],
             'LAMBDA ': [],
             'BURN_STEP': [],
             'BURNUP ': [],
             'BURN_DAYS': []
         }
```

### Comparing `zmeiapi-0.1.8/zmeiapi.egg-info/SOURCES.txt` & `zmeiapi-0.1.9/zmeiapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

