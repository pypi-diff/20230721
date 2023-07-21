# Comparing `tmp/caped-ai-augmentations-1.0.7.tar.gz` & `tmp/caped-ai-augmentations-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caped-ai-augmentations-1.0.7.tar", last modified: Sun Jul  2 19:04:46 2023, max compression
+gzip compressed data, was "caped-ai-augmentations-1.0.8.tar", last modified: Fri Jul 21 13:39:47 2023, max compression
```

## Comparing `caped-ai-augmentations-1.0.7.tar` & `caped-ai-augmentations-1.0.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-02 19:04:46.296342 caped-ai-augmentations-1.0.7/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1512 2022-09-07 10:32:19.000000 caped-ai-augmentations-1.0.7/LICENSE
--rwxrwxrwx   0 debian    (1000) debian    (1000)      738 2023-07-02 19:04:46.290757 caped-ai-augmentations-1.0.7/PKG-INFO
--rwxrwxrwx   0 debian    (1000) debian    (1000)       75 2022-09-07 10:16:18.000000 caped-ai-augmentations-1.0.7/README.md
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-02 19:04:46.104431 caped-ai-augmentations-1.0.7/caped_ai_augmentations/
--rwxrwxrwx   0 debian    (1000) debian    (1000)    11274 2022-10-03 15:24:38.000000 caped-ai-augmentations-1.0.7/caped_ai_augmentations/AugmentTYXCsv.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    11983 2022-10-03 15:24:27.000000 caped-ai-augmentations-1.0.7/caped_ai_augmentations/AugmentTZYXCsv.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    11894 2022-12-23 20:19:23.000000 caped-ai-augmentations-1.0.7/caped_ai_augmentations/AugmentYX.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    12485 2022-12-23 15:45:33.000000 caped-ai-augmentations-1.0.7/caped_ai_augmentations/AugmentYXC.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    13152 2022-10-03 15:25:00.000000 caped-ai-augmentations-1.0.7/caped_ai_augmentations/AugmentZYX.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)      315 2022-10-12 12:10:32.000000 caped-ai-augmentations-1.0.7/caped_ai_augmentations/__init__.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)      105 2023-07-02 19:03:39.000000 caped-ai-augmentations-1.0.7/caped_ai_augmentations/_version.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     4537 2022-12-23 19:35:26.000000 caped-ai-augmentations-1.0.7/caped_ai_augmentations/utils.py
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-02 19:04:46.255970 caped-ai-augmentations-1.0.7/caped_ai_augmentations.egg-info/
--rwxrwxrwx   0 debian    (1000) debian    (1000)      738 2023-07-02 19:04:45.000000 caped-ai-augmentations-1.0.7/caped_ai_augmentations.egg-info/PKG-INFO
--rwxrwxrwx   0 debian    (1000) debian    (1000)      548 2023-07-02 19:04:45.000000 caped-ai-augmentations-1.0.7/caped_ai_augmentations.egg-info/SOURCES.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)        1 2023-07-02 19:04:45.000000 caped-ai-augmentations-1.0.7/caped_ai_augmentations.egg-info/dependency_links.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       71 2023-07-02 19:04:45.000000 caped-ai-augmentations-1.0.7/caped_ai_augmentations.egg-info/requires.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       23 2023-07-02 19:04:45.000000 caped-ai-augmentations-1.0.7/caped_ai_augmentations.egg-info/top_level.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       38 2023-07-02 19:04:46.297347 caped-ai-augmentations-1.0.7/setup.cfg
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1294 2023-07-02 19:03:29.000000 caped-ai-augmentations-1.0.7/setup.py
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-21 13:39:47.155319 caped-ai-augmentations-1.0.8/
+-rw-r--r--   0 vkapoor    (503) staff       (20)     1512 2023-07-21 10:29:24.000000 caped-ai-augmentations-1.0.8/LICENSE
+-rw-r--r--   0 vkapoor    (503) staff       (20)      738 2023-07-21 13:39:47.155216 caped-ai-augmentations-1.0.8/PKG-INFO
+-rw-r--r--   0 vkapoor    (503) staff       (20)       75 2023-07-21 10:29:24.000000 caped-ai-augmentations-1.0.8/README.md
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-21 13:39:47.154347 caped-ai-augmentations-1.0.8/caped_ai_augmentations/
+-rw-r--r--   0 vkapoor    (503) staff       (20)    11274 2023-07-21 10:29:24.000000 caped-ai-augmentations-1.0.8/caped_ai_augmentations/AugmentTYXCsv.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    11983 2023-07-21 10:29:24.000000 caped-ai-augmentations-1.0.8/caped_ai_augmentations/AugmentTZYXCsv.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    11894 2023-07-21 10:29:24.000000 caped-ai-augmentations-1.0.8/caped_ai_augmentations/AugmentYX.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    12485 2023-07-21 10:29:24.000000 caped-ai-augmentations-1.0.8/caped_ai_augmentations/AugmentYXC.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    13152 2023-07-21 10:29:24.000000 caped-ai-augmentations-1.0.8/caped_ai_augmentations/AugmentZYX.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)      315 2023-07-21 10:29:24.000000 caped-ai-augmentations-1.0.8/caped_ai_augmentations/__init__.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)      105 2023-07-21 13:39:20.000000 caped-ai-augmentations-1.0.8/caped_ai_augmentations/_version.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     4537 2023-07-21 10:29:24.000000 caped-ai-augmentations-1.0.8/caped_ai_augmentations/utils.py
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-21 13:39:47.155055 caped-ai-augmentations-1.0.8/caped_ai_augmentations.egg-info/
+-rw-r--r--   0 vkapoor    (503) staff       (20)      738 2023-07-21 13:39:47.000000 caped-ai-augmentations-1.0.8/caped_ai_augmentations.egg-info/PKG-INFO
+-rw-r--r--   0 vkapoor    (503) staff       (20)      548 2023-07-21 13:39:47.000000 caped-ai-augmentations-1.0.8/caped_ai_augmentations.egg-info/SOURCES.txt
+-rw-r--r--   0 vkapoor    (503) staff       (20)        1 2023-07-21 13:39:47.000000 caped-ai-augmentations-1.0.8/caped_ai_augmentations.egg-info/dependency_links.txt
+-rw-r--r--   0 vkapoor    (503) staff       (20)       71 2023-07-21 13:39:47.000000 caped-ai-augmentations-1.0.8/caped_ai_augmentations.egg-info/requires.txt
+-rw-r--r--   0 vkapoor    (503) staff       (20)       23 2023-07-21 13:39:47.000000 caped-ai-augmentations-1.0.8/caped_ai_augmentations.egg-info/top_level.txt
+-rw-r--r--   0 vkapoor    (503) staff       (20)       38 2023-07-21 13:39:47.155353 caped-ai-augmentations-1.0.8/setup.cfg
+-rw-r--r--   0 vkapoor    (503) staff       (20)     1294 2023-07-21 10:29:24.000000 caped-ai-augmentations-1.0.8/setup.py
```

### Comparing `caped-ai-augmentations-1.0.7/LICENSE` & `caped-ai-augmentations-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `caped-ai-augmentations-1.0.7/PKG-INFO` & `caped-ai-augmentations-1.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caped-ai-augmentations
-Version: 1.0.7
+Version: 1.0.8
 Summary: Augmentations for volume, planar segmentation, classification image segmentation and associated csv file of oneat clicks.
 Home-page: https://github.com/Kapoorlabs-CAPED/Augmentations/
 Author: Varun Kapoor
 Author-email: randomaccessiblekapoor@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `caped-ai-augmentations-1.0.7/caped_ai_augmentations/AugmentTYXCsv.py` & `caped-ai-augmentations-1.0.8/caped_ai_augmentations/AugmentTYXCsv.py`

 * *Files identical despite different names*

### Comparing `caped-ai-augmentations-1.0.7/caped_ai_augmentations/AugmentTZYXCsv.py` & `caped-ai-augmentations-1.0.8/caped_ai_augmentations/AugmentTZYXCsv.py`

 * *Files identical despite different names*

### Comparing `caped-ai-augmentations-1.0.7/caped_ai_augmentations/AugmentYX.py` & `caped-ai-augmentations-1.0.8/caped_ai_augmentations/AugmentYX.py`

 * *Files identical despite different names*

### Comparing `caped-ai-augmentations-1.0.7/caped_ai_augmentations/AugmentYXC.py` & `caped-ai-augmentations-1.0.8/caped_ai_augmentations/AugmentYXC.py`

 * *Files identical despite different names*

### Comparing `caped-ai-augmentations-1.0.7/caped_ai_augmentations/AugmentZYX.py` & `caped-ai-augmentations-1.0.8/caped_ai_augmentations/AugmentZYX.py`

 * *Files identical despite different names*

### Comparing `caped-ai-augmentations-1.0.7/caped_ai_augmentations/utils.py` & `caped-ai-augmentations-1.0.8/caped_ai_augmentations/utils.py`

 * *Files identical despite different names*

### Comparing `caped-ai-augmentations-1.0.7/caped_ai_augmentations.egg-info/PKG-INFO` & `caped-ai-augmentations-1.0.8/caped_ai_augmentations.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caped-ai-augmentations
-Version: 1.0.7
+Version: 1.0.8
 Summary: Augmentations for volume, planar segmentation, classification image segmentation and associated csv file of oneat clicks.
 Home-page: https://github.com/Kapoorlabs-CAPED/Augmentations/
 Author: Varun Kapoor
 Author-email: randomaccessiblekapoor@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `caped-ai-augmentations-1.0.7/caped_ai_augmentations.egg-info/SOURCES.txt` & `caped-ai-augmentations-1.0.8/caped_ai_augmentations.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `caped-ai-augmentations-1.0.7/setup.py` & `caped-ai-augmentations-1.0.8/setup.py`

 * *Files identical despite different names*

