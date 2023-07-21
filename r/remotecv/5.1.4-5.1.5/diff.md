# Comparing `tmp/remotecv-5.1.4.tar.gz` & `tmp/remotecv-5.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remotecv-5.1.4.tar", last modified: Wed Jul 19 13:52:14 2023, max compression
+gzip compressed data, was "remotecv-5.1.5.tar", last modified: Fri Jul 21 14:28:35 2023, max compression
```

## Comparing `remotecv-5.1.4.tar` & `remotecv-5.1.5.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:52:14.974527 remotecv-5.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-19 13:52:10.000000 remotecv-5.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-19 13:52:10.000000 remotecv-5.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5608 2023-07-19 13:52:14.974527 remotecv-5.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-07-19 13:52:10.000000 remotecv-5.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-19 13:52:10.000000 remotecv-5.1.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:52:14.966527 remotecv-5.1.4/remotecv/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-19 13:52:10.000000 remotecv-5.1.4/remotecv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-07-19 13:52:10.000000 remotecv-5.1.4/remotecv/celery_tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:52:14.966527 remotecv-5.1.4/remotecv/detectors/
--rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-07-19 13:52:10.000000 remotecv-5.1.4/remotecv/detectors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:52:14.966527 remotecv-5.1.4/remotecv/detectors/complete_detector/
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-07-19 13:52:10.000000 remotecv-5.1.4/remotecv/detectors/complete_detector/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:52:14.970527 remotecv-5.1.4/remotecv/detectors/face_detector/
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-19 13:52:10.000000 remotecv-5.1.4/remotecv/detectors/face_detector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   676709 2023-07-19 13:52:10.000000 remotecv-5.1.4/remotecv/detectors/face_detector/haarcascade_frontalface_alt.xml
--rw-r--r--   0 runner    (1001) docker     (123)   540616 2023-07-19 13:52:10.000000 remotecv-5.1.4/remotecv/detectors/face_detector/haarcascade_frontalface_alt2.xml
--rw-r--r--   0 runner    (1001) docker     (123)  2689040 2023-07-19 13:52:10.000000 remotecv-5.1.4/remotecv/detectors/face_detector/haarcascade_frontalface_alt_tree.xml
--rw-r--r--   0 runner    (1001) docker     (123)   930127 2023-07-19 13:52:10.000000 remotecv-5.1.4/remotecv/detectors/face_detector/haarcascade_frontalface_default.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:52:14.970527 remotecv-5.1.4/remotecv/detectors/feature_detector/
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-19 13:52:10.000000 remotecv-5.1.4/remotecv/detectors/feature_detector/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:52:14.970527 remotecv-5.1.4/remotecv/detectors/glasses_detector/
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-19 13:52:10.000000 remotecv-5.1.4/remotecv/detectors/glasses_detector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   601661 2023-07-19 13:52:10.000000 remotecv-5.1.4/remotecv/detectors/glasses_detector/haarcascade_eye_tree_eyeglasses.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:52:14.970527 remotecv-5.1.4/remotecv/detectors/profile_detector/
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-07-19 13:52:10.000000 remotecv-5.1.4/remotecv/detectors/profile_detector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   828514 2023-07-19 13:52:10.000000 remotecv-5.1.4/remotecv/detectors/profile_detector/haarcascade_profileface.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-07-19 13:52:10.000000 remotecv-5.1.4/remotecv/error_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-19 13:52:10.000000 remotecv-5.1.4/remotecv/healthcheck.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-19 13:52:10.000000 remotecv-5.1.4/remotecv/http_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-19 13:52:10.000000 remotecv-5.1.4/remotecv/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-07-19 13:52:10.000000 remotecv-5.1.4/remotecv/image_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-19 13:52:10.000000 remotecv-5.1.4/remotecv/importer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:52:14.970527 remotecv-5.1.4/remotecv/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-19 13:52:10.000000 remotecv-5.1.4/remotecv/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-19 13:52:10.000000 remotecv-5.1.4/remotecv/metrics/logger_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-07-19 13:52:10.000000 remotecv-5.1.4/remotecv/pyres_tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:52:14.970527 remotecv-5.1.4/remotecv/result_store/
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-19 13:52:10.000000 remotecv-5.1.4/remotecv/result_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-19 13:52:10.000000 remotecv-5.1.4/remotecv/result_store/memcache_store.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-19 13:52:10.000000 remotecv-5.1.4/remotecv/result_store/redis_store.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-19 13:52:10.000000 remotecv-5.1.4/remotecv/timing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-07-19 13:52:10.000000 remotecv-5.1.4/remotecv/unique_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-07-19 13:52:10.000000 remotecv-5.1.4/remotecv/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8692 2023-07-19 13:52:10.000000 remotecv-5.1.4/remotecv/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:52:14.974527 remotecv-5.1.4/remotecv.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5608 2023-07-19 13:52:14.000000 remotecv-5.1.4/remotecv.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-07-19 13:52:14.000000 remotecv-5.1.4/remotecv.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 13:52:14.000000 remotecv-5.1.4/remotecv.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-19 13:52:14.000000 remotecv-5.1.4/remotecv.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-07-19 13:52:14.000000 remotecv-5.1.4/remotecv.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-19 13:52:14.000000 remotecv-5.1.4/remotecv.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-19 13:52:14.974527 remotecv-5.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-07-19 13:52:10.000000 remotecv-5.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:28:35.949366 remotecv-5.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-21 14:28:30.000000 remotecv-5.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-21 14:28:30.000000 remotecv-5.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5608 2023-07-21 14:28:35.949366 remotecv-5.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-07-21 14:28:30.000000 remotecv-5.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-21 14:28:30.000000 remotecv-5.1.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:28:35.941366 remotecv-5.1.5/remotecv/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-21 14:28:30.000000 remotecv-5.1.5/remotecv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-07-21 14:28:30.000000 remotecv-5.1.5/remotecv/celery_tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:28:35.941366 remotecv-5.1.5/remotecv/detectors/
+-rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-07-21 14:28:30.000000 remotecv-5.1.5/remotecv/detectors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:28:35.941366 remotecv-5.1.5/remotecv/detectors/complete_detector/
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-07-21 14:28:30.000000 remotecv-5.1.5/remotecv/detectors/complete_detector/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:28:35.945366 remotecv-5.1.5/remotecv/detectors/face_detector/
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-21 14:28:30.000000 remotecv-5.1.5/remotecv/detectors/face_detector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   676709 2023-07-21 14:28:30.000000 remotecv-5.1.5/remotecv/detectors/face_detector/haarcascade_frontalface_alt.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   540616 2023-07-21 14:28:30.000000 remotecv-5.1.5/remotecv/detectors/face_detector/haarcascade_frontalface_alt2.xml
+-rw-r--r--   0 runner    (1001) docker     (123)  2689040 2023-07-21 14:28:30.000000 remotecv-5.1.5/remotecv/detectors/face_detector/haarcascade_frontalface_alt_tree.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   930127 2023-07-21 14:28:30.000000 remotecv-5.1.5/remotecv/detectors/face_detector/haarcascade_frontalface_default.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:28:35.949366 remotecv-5.1.5/remotecv/detectors/feature_detector/
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-21 14:28:30.000000 remotecv-5.1.5/remotecv/detectors/feature_detector/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:28:35.949366 remotecv-5.1.5/remotecv/detectors/glasses_detector/
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-21 14:28:30.000000 remotecv-5.1.5/remotecv/detectors/glasses_detector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   601661 2023-07-21 14:28:30.000000 remotecv-5.1.5/remotecv/detectors/glasses_detector/haarcascade_eye_tree_eyeglasses.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:28:35.949366 remotecv-5.1.5/remotecv/detectors/profile_detector/
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-07-21 14:28:30.000000 remotecv-5.1.5/remotecv/detectors/profile_detector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   828514 2023-07-21 14:28:30.000000 remotecv-5.1.5/remotecv/detectors/profile_detector/haarcascade_profileface.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-07-21 14:28:30.000000 remotecv-5.1.5/remotecv/error_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-21 14:28:30.000000 remotecv-5.1.5/remotecv/healthcheck.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-21 14:28:30.000000 remotecv-5.1.5/remotecv/http_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-21 14:28:30.000000 remotecv-5.1.5/remotecv/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-07-21 14:28:30.000000 remotecv-5.1.5/remotecv/image_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-21 14:28:30.000000 remotecv-5.1.5/remotecv/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:28:35.949366 remotecv-5.1.5/remotecv/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-21 14:28:30.000000 remotecv-5.1.5/remotecv/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-21 14:28:30.000000 remotecv-5.1.5/remotecv/metrics/logger_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-07-21 14:28:30.000000 remotecv-5.1.5/remotecv/pyres_tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:28:35.949366 remotecv-5.1.5/remotecv/result_store/
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-21 14:28:30.000000 remotecv-5.1.5/remotecv/result_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-21 14:28:30.000000 remotecv-5.1.5/remotecv/result_store/memcache_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-21 14:28:30.000000 remotecv-5.1.5/remotecv/result_store/redis_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-21 14:28:30.000000 remotecv-5.1.5/remotecv/timing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-07-21 14:28:30.000000 remotecv-5.1.5/remotecv/unique_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-07-21 14:28:30.000000 remotecv-5.1.5/remotecv/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8935 2023-07-21 14:28:30.000000 remotecv-5.1.5/remotecv/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:28:35.949366 remotecv-5.1.5/remotecv.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5608 2023-07-21 14:28:35.000000 remotecv-5.1.5/remotecv.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-07-21 14:28:35.000000 remotecv-5.1.5/remotecv.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 14:28:35.000000 remotecv-5.1.5/remotecv.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-21 14:28:35.000000 remotecv-5.1.5/remotecv.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-07-21 14:28:35.000000 remotecv-5.1.5/remotecv.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-21 14:28:35.000000 remotecv-5.1.5/remotecv.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-21 14:28:35.953366 remotecv-5.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-07-21 14:28:30.000000 remotecv-5.1.5/setup.py
```

### Comparing `remotecv-5.1.4/LICENSE` & `remotecv-5.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `remotecv-5.1.4/PKG-INFO` & `remotecv-5.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remotecv
-Version: 5.1.4
+Version: 5.1.5
 Summary: remotecv is an OpenCV worker for facial and feature recognition
 Home-page: https://github.com/thumbor/remotecv
 Author: Bernardo Heynemann
 Author-email: heynemann@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `remotecv-5.1.4/README.md` & `remotecv-5.1.5/README.md`

 * *Files identical despite different names*

### Comparing `remotecv-5.1.4/remotecv/celery_tasks.py` & `remotecv-5.1.5/remotecv/celery_tasks.py`

 * *Files identical despite different names*

### Comparing `remotecv-5.1.4/remotecv/detectors/__init__.py` & `remotecv-5.1.5/remotecv/detectors/__init__.py`

 * *Files identical despite different names*

### Comparing `remotecv-5.1.4/remotecv/detectors/complete_detector/__init__.py` & `remotecv-5.1.5/remotecv/detectors/complete_detector/__init__.py`

 * *Files identical despite different names*

### Comparing `remotecv-5.1.4/remotecv/detectors/face_detector/__init__.py` & `remotecv-5.1.5/remotecv/detectors/face_detector/__init__.py`

 * *Files identical despite different names*

### Comparing `remotecv-5.1.4/remotecv/detectors/face_detector/haarcascade_frontalface_alt.xml` & `remotecv-5.1.5/remotecv/detectors/face_detector/haarcascade_frontalface_alt.xml`

 * *Files identical despite different names*

### Comparing `remotecv-5.1.4/remotecv/detectors/face_detector/haarcascade_frontalface_alt2.xml` & `remotecv-5.1.5/remotecv/detectors/face_detector/haarcascade_frontalface_alt2.xml`

 * *Files identical despite different names*

### Comparing `remotecv-5.1.4/remotecv/detectors/face_detector/haarcascade_frontalface_alt_tree.xml` & `remotecv-5.1.5/remotecv/detectors/face_detector/haarcascade_frontalface_alt_tree.xml`

 * *Files identical despite different names*

### Comparing `remotecv-5.1.4/remotecv/detectors/face_detector/haarcascade_frontalface_default.xml` & `remotecv-5.1.5/remotecv/detectors/face_detector/haarcascade_frontalface_default.xml`

 * *Files identical despite different names*

### Comparing `remotecv-5.1.4/remotecv/detectors/feature_detector/__init__.py` & `remotecv-5.1.5/remotecv/detectors/feature_detector/__init__.py`

 * *Files identical despite different names*

### Comparing `remotecv-5.1.4/remotecv/detectors/glasses_detector/haarcascade_eye_tree_eyeglasses.xml` & `remotecv-5.1.5/remotecv/detectors/glasses_detector/haarcascade_eye_tree_eyeglasses.xml`

 * *Files identical despite different names*

### Comparing `remotecv-5.1.4/remotecv/detectors/profile_detector/haarcascade_profileface.xml` & `remotecv-5.1.5/remotecv/detectors/profile_detector/haarcascade_profileface.xml`

 * *Files identical despite different names*

### Comparing `remotecv-5.1.4/remotecv/error_handler.py` & `remotecv-5.1.5/remotecv/error_handler.py`

 * *Files identical despite different names*

### Comparing `remotecv-5.1.4/remotecv/http_loader.py` & `remotecv-5.1.5/remotecv/http_loader.py`

 * *Files identical despite different names*

### Comparing `remotecv-5.1.4/remotecv/image.py` & `remotecv-5.1.5/remotecv/image.py`

 * *Files identical despite different names*

### Comparing `remotecv-5.1.4/remotecv/image_processor.py` & `remotecv-5.1.5/remotecv/image_processor.py`

 * *Files identical despite different names*

### Comparing `remotecv-5.1.4/remotecv/metrics/logger_metrics.py` & `remotecv-5.1.5/remotecv/metrics/logger_metrics.py`

 * *Files identical despite different names*

### Comparing `remotecv-5.1.4/remotecv/pyres_tasks.py` & `remotecv-5.1.5/remotecv/pyres_tasks.py`

 * *Files identical despite different names*

### Comparing `remotecv-5.1.4/remotecv/result_store/__init__.py` & `remotecv-5.1.5/remotecv/result_store/__init__.py`

 * *Files identical despite different names*

### Comparing `remotecv-5.1.4/remotecv/result_store/memcache_store.py` & `remotecv-5.1.5/remotecv/result_store/memcache_store.py`

 * *Files identical despite different names*

### Comparing `remotecv-5.1.4/remotecv/result_store/redis_store.py` & `remotecv-5.1.5/remotecv/result_store/redis_store.py`

 * *Files identical despite different names*

### Comparing `remotecv-5.1.4/remotecv/unique_queue.py` & `remotecv-5.1.5/remotecv/unique_queue.py`

 * *Files 6% similar despite different names*

```diff
@@ -87,7 +87,13 @@
 
     def register_worker(self):
         super().register_worker()
         if config.worker_ttl:
             self.resq.redis.expire(
                 f"resque:worker:{str(self)}:started", config.worker_ttl
             )
+
+    def startup(self):
+        if config.prune_dead_members:
+            self.resq.redis.delete("resque:workers")
+
+        super().startup()
```

### Comparing `remotecv-5.1.4/remotecv/utils.py` & `remotecv-5.1.5/remotecv/utils.py`

 * *Files identical despite different names*

### Comparing `remotecv-5.1.4/remotecv/worker.py` & `remotecv-5.1.5/remotecv/worker.py`

 * *Files 2% similar despite different names*

```diff
@@ -272,14 +272,22 @@
     envvar="WORKER_TTL",
     show_envvar=True,
     default=None,
     type=click.INT,
     help="TTL in seconds for worker",
 )
 @optgroup.option(
+    "--prune-dead-members",
+    envvar="PRUNE_DEAD_MEMBERS",
+    show_envvar=True,
+    is_flag=True,
+    default=False,
+    help="Prune dead members on startup",
+)
+@optgroup.option(
     "--sentry-url",
     envvar="SENTRY_URL",
     show_envvar=True,
     default=None,
     help="Sentry URL",
 )
 @optgroup.option(
@@ -319,14 +327,15 @@
     config.region = params["region"]
     config.key_id = params["key_id"]
     config.key_secret = params["key_secret"]
     config.polling_interval = params["polling_interval"]
 
     config.timeout = params["timeout"]
     config.worker_ttl = params["worker_ttl"]
+    config.prune_dead_members = params["prune_dead_members"]
     config.server_port = params["server_port"]
     config.log_level = params["level"].upper()
     config.loader = import_module(params["loader"])
     config.store = import_module(params["store"])
 
     config.metrics = params["metrics"]
```

### Comparing `remotecv-5.1.4/remotecv.egg-info/PKG-INFO` & `remotecv-5.1.5/remotecv.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remotecv
-Version: 5.1.4
+Version: 5.1.5
 Summary: remotecv is an OpenCV worker for facial and feature recognition
 Home-page: https://github.com/thumbor/remotecv
 Author: Bernardo Heynemann
 Author-email: heynemann@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `remotecv-5.1.4/remotecv.egg-info/SOURCES.txt` & `remotecv-5.1.5/remotecv.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `remotecv-5.1.4/remotecv.egg-info/requires.txt` & `remotecv-5.1.5/remotecv.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `remotecv-5.1.4/setup.py` & `remotecv-5.1.5/setup.py`

 * *Files identical despite different names*

