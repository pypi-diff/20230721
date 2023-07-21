# Comparing `tmp/xcalibu-0.9.9.tar.gz` & `tmp/xcalibu-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xcalibu-0.9.9.tar", last modified: Fri Jul 21 14:53:10 2023, max compression
+gzip compressed data, was "xcalibu-1.0.0.tar", last modified: Fri Jul 21 14:54:09 2023, max compression
```

## Comparing `xcalibu-0.9.9.tar` & `xcalibu-1.0.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 guilloud  (5498) soft      (3401)        0 2023-07-21 14:53:10.959477 xcalibu-0.9.9/
--rw-r--r--   0 guilloud  (5498) soft      (3401)     7652 2020-11-24 13:00:47.000000 xcalibu-0.9.9/LICENSE
--rw-r--r--   0 guilloud  (5498) soft      (3401)       64 2020-11-24 13:00:47.000000 xcalibu-0.9.9/MANIFEST.in
--rw-r--r--   0 guilloud  (5498) soft      (3401)     2868 2023-07-21 14:53:10.959477 xcalibu-0.9.9/PKG-INFO
--rw-r--r--   0 guilloud  (5498) soft      (3401)     2427 2023-02-23 08:54:10.000000 xcalibu-0.9.9/README.md
--rw-r--r--   0 guilloud  (5498) soft      (3401)      135 2023-07-21 14:53:10.963477 xcalibu-0.9.9/setup.cfg
--rw-r--r--   0 guilloud  (5498) soft      (3401)      850 2023-03-31 15:22:44.000000 xcalibu-0.9.9/setup.py
-drwxr-xr-x   0 guilloud  (5498) soft      (3401)        0 2023-07-21 14:53:10.791476 xcalibu-0.9.9/tests/
--rw-r--r--   0 guilloud  (5498) soft      (3401)     4313 2022-03-28 17:08:23.000000 xcalibu-0.9.9/tests/test_calib_table.py
-drwxr-xr-x   0 guilloud  (5498) soft      (3401)        0 2023-07-21 14:53:10.851476 xcalibu-0.9.9/xcalibu/
--rw-r--r--   0 guilloud  (5498) soft      (3401)    16352 2020-11-24 13:00:47.000000 xcalibu-0.9.9/xcalibu/Xcalibuds.py
--rw-r--r--   0 guilloud  (5498) soft      (3401)       42 2022-03-10 11:11:51.000000 xcalibu-0.9.9/xcalibu/__init__.py
--rwxr-xr-x   0 guilloud  (5498) soft      (3401)    14076 2023-03-31 15:37:13.000000 xcalibu-0.9.9/xcalibu/demo_xcalibu.py
--rwxr-xr-x   0 guilloud  (5498) soft      (3401)      839 2022-11-10 17:48:00.000000 xcalibu-0.9.9/xcalibu/device_test.py
-drwxr-xr-x   0 guilloud  (5498) soft      (3401)        0 2023-07-21 14:53:10.959477 xcalibu-0.9.9/xcalibu/examples/
--rw-r-----   0 guilloud  (5498) soft      (3401)      537 2023-02-15 21:13:36.000000 xcalibu-0.9.9/xcalibu/examples/U32a_1_table.txt
--rw-r--r--   0 guilloud  (5498) soft      (3401)      537 2023-03-31 15:19:30.000000 xcalibu-0.9.9/xcalibu/examples/U32a_table_non_monotonic.txt
--rw-r--r--   0 guilloud  (5498) soft      (3401)    33270 2023-02-15 09:04:27.000000 xcalibu-0.9.9/xcalibu/examples/book5.txt
--rw-r--r--   0 guilloud  (5498) soft      (3401)      357 2023-03-28 10:57:47.000000 xcalibu-0.9.9/xcalibu/examples/cubic.calib
--rw-r--r--   0 guilloud  (5498) soft      (3401)      252 2023-03-28 10:57:47.000000 xcalibu-0.9.9/xcalibu/examples/cubic_poly.calib
--rw-r--r--   0 guilloud  (5498) soft      (3401)      416 2019-05-20 14:51:43.000000 xcalibu-0.9.9/xcalibu/examples/gauss.calib
--rw-r--r--   0 guilloud  (5498) soft      (3401)    12349 2020-11-24 13:00:47.000000 xcalibu-0.9.9/xcalibu/examples/hpz_ring_Ry.calib
--rw-r--r--   0 guilloud  (5498) soft      (3401)    13004 2020-11-24 13:00:47.000000 xcalibu-0.9.9/xcalibu/examples/hpz_ring_Tz.calib
--rw-r--r--   0 guilloud  (5498) soft      (3401)      331 2023-02-21 12:30:03.000000 xcalibu-0.9.9/xcalibu/examples/poly.calib
--rw-r--r--   0 guilloud  (5498) soft      (3401)      296 2023-04-14 14:08:28.000000 xcalibu-0.9.9/xcalibu/examples/qepro.calib
--rw-r--r--   0 guilloud  (5498) soft      (3401)      463 2023-04-14 13:50:54.000000 xcalibu-0.9.9/xcalibu/examples/table.calib
--rw-r--r--   0 guilloud  (5498) soft      (3401)       93 2023-02-15 09:04:27.000000 xcalibu-0.9.9/xcalibu/examples/table_1_column.txt
--rw-r--r--   0 guilloud  (5498) soft      (3401)      340 2022-03-10 11:11:51.000000 xcalibu-0.9.9/xcalibu/examples/table_2_col.calib
--rw-r--r--   0 guilloud  (5498) soft      (3401)      128 2022-03-10 11:11:51.000000 xcalibu-0.9.9/xcalibu/examples/table_2_columns.txt
--rw-r--r--   0 guilloud  (5498) soft      (3401)      443 2023-03-03 08:55:18.000000 xcalibu-0.9.9/xcalibu/examples/u32a_poly.calib
--rw-r--r--   0 guilloud  (5498) soft      (3401)      476 2023-02-15 18:53:58.000000 xcalibu-0.9.9/xcalibu/examples/undu_table.calib
--rw-r--r--   0 guilloud  (5498) soft      (3401)      350 2023-03-28 10:57:47.000000 xcalibu-0.9.9/xcalibu/examples/unsorted_table.calib
--rwxr-xr-x   0 guilloud  (5498) soft      (3401)     3095 2023-03-28 10:58:48.000000 xcalibu-0.9.9/xcalibu/test_xcalibu.py
--rwxr-xr-x   0 guilloud  (5498) soft      (3401)    56072 2023-04-14 14:05:55.000000 xcalibu-0.9.9/xcalibu/xcalibu.py
-drwxr-xr-x   0 guilloud  (5498) soft      (3401)        0 2023-07-21 14:53:10.851476 xcalibu-0.9.9/xcalibu.egg-info/
--rw-r--r--   0 guilloud  (5498) soft      (3401)     2868 2023-07-21 14:53:10.000000 xcalibu-0.9.9/xcalibu.egg-info/PKG-INFO
--rw-r--r--   0 guilloud  (5498) soft      (3401)      931 2023-07-21 14:53:10.000000 xcalibu-0.9.9/xcalibu.egg-info/SOURCES.txt
--rw-r--r--   0 guilloud  (5498) soft      (3401)        1 2023-07-21 14:53:10.000000 xcalibu-0.9.9/xcalibu.egg-info/dependency_links.txt
--rw-r--r--   0 guilloud  (5498) soft      (3401)       89 2023-07-21 14:53:10.000000 xcalibu-0.9.9/xcalibu.egg-info/entry_points.txt
--rw-r--r--   0 guilloud  (5498) soft      (3401)        8 2023-07-21 14:53:10.000000 xcalibu-0.9.9/xcalibu.egg-info/top_level.txt
+drwxr-xr-x   0 guilloud  (5498) soft      (3401)        0 2023-07-21 14:54:09.395892 xcalibu-1.0.0/
+-rw-r--r--   0 guilloud  (5498) soft      (3401)     7652 2020-11-24 13:00:47.000000 xcalibu-1.0.0/LICENSE
+-rw-r--r--   0 guilloud  (5498) soft      (3401)       64 2020-11-24 13:00:47.000000 xcalibu-1.0.0/MANIFEST.in
+-rw-r--r--   0 guilloud  (5498) soft      (3401)     2868 2023-07-21 14:54:09.395892 xcalibu-1.0.0/PKG-INFO
+-rw-r--r--   0 guilloud  (5498) soft      (3401)     2427 2023-02-23 08:54:10.000000 xcalibu-1.0.0/README.md
+-rw-r--r--   0 guilloud  (5498) soft      (3401)      135 2023-07-21 14:54:09.399892 xcalibu-1.0.0/setup.cfg
+-rw-r--r--   0 guilloud  (5498) soft      (3401)      850 2023-07-21 14:53:55.000000 xcalibu-1.0.0/setup.py
+drwxr-xr-x   0 guilloud  (5498) soft      (3401)        0 2023-07-21 14:54:09.395892 xcalibu-1.0.0/tests/
+-rw-r--r--   0 guilloud  (5498) soft      (3401)     4313 2022-03-28 17:08:23.000000 xcalibu-1.0.0/tests/test_calib_table.py
+drwxr-xr-x   0 guilloud  (5498) soft      (3401)        0 2023-07-21 14:54:09.395892 xcalibu-1.0.0/xcalibu/
+-rw-r--r--   0 guilloud  (5498) soft      (3401)    16352 2020-11-24 13:00:47.000000 xcalibu-1.0.0/xcalibu/Xcalibuds.py
+-rw-r--r--   0 guilloud  (5498) soft      (3401)       42 2022-03-10 11:11:51.000000 xcalibu-1.0.0/xcalibu/__init__.py
+-rwxr-xr-x   0 guilloud  (5498) soft      (3401)    14076 2023-03-31 15:37:13.000000 xcalibu-1.0.0/xcalibu/demo_xcalibu.py
+-rwxr-xr-x   0 guilloud  (5498) soft      (3401)      839 2022-11-10 17:48:00.000000 xcalibu-1.0.0/xcalibu/device_test.py
+drwxr-xr-x   0 guilloud  (5498) soft      (3401)        0 2023-07-21 14:54:09.395892 xcalibu-1.0.0/xcalibu/examples/
+-rw-r-----   0 guilloud  (5498) soft      (3401)      537 2023-02-15 21:13:36.000000 xcalibu-1.0.0/xcalibu/examples/U32a_1_table.txt
+-rw-r--r--   0 guilloud  (5498) soft      (3401)      537 2023-03-31 15:19:30.000000 xcalibu-1.0.0/xcalibu/examples/U32a_table_non_monotonic.txt
+-rw-r--r--   0 guilloud  (5498) soft      (3401)    33270 2023-02-15 09:04:27.000000 xcalibu-1.0.0/xcalibu/examples/book5.txt
+-rw-r--r--   0 guilloud  (5498) soft      (3401)      357 2023-03-28 10:57:47.000000 xcalibu-1.0.0/xcalibu/examples/cubic.calib
+-rw-r--r--   0 guilloud  (5498) soft      (3401)      252 2023-03-28 10:57:47.000000 xcalibu-1.0.0/xcalibu/examples/cubic_poly.calib
+-rw-r--r--   0 guilloud  (5498) soft      (3401)      416 2019-05-20 14:51:43.000000 xcalibu-1.0.0/xcalibu/examples/gauss.calib
+-rw-r--r--   0 guilloud  (5498) soft      (3401)    12349 2020-11-24 13:00:47.000000 xcalibu-1.0.0/xcalibu/examples/hpz_ring_Ry.calib
+-rw-r--r--   0 guilloud  (5498) soft      (3401)    13004 2020-11-24 13:00:47.000000 xcalibu-1.0.0/xcalibu/examples/hpz_ring_Tz.calib
+-rw-r--r--   0 guilloud  (5498) soft      (3401)      331 2023-02-21 12:30:03.000000 xcalibu-1.0.0/xcalibu/examples/poly.calib
+-rw-r--r--   0 guilloud  (5498) soft      (3401)      296 2023-04-14 14:08:28.000000 xcalibu-1.0.0/xcalibu/examples/qepro.calib
+-rw-r--r--   0 guilloud  (5498) soft      (3401)      463 2023-04-14 13:50:54.000000 xcalibu-1.0.0/xcalibu/examples/table.calib
+-rw-r--r--   0 guilloud  (5498) soft      (3401)       93 2023-02-15 09:04:27.000000 xcalibu-1.0.0/xcalibu/examples/table_1_column.txt
+-rw-r--r--   0 guilloud  (5498) soft      (3401)      340 2022-03-10 11:11:51.000000 xcalibu-1.0.0/xcalibu/examples/table_2_col.calib
+-rw-r--r--   0 guilloud  (5498) soft      (3401)      128 2022-03-10 11:11:51.000000 xcalibu-1.0.0/xcalibu/examples/table_2_columns.txt
+-rw-r--r--   0 guilloud  (5498) soft      (3401)      443 2023-03-03 08:55:18.000000 xcalibu-1.0.0/xcalibu/examples/u32a_poly.calib
+-rw-r--r--   0 guilloud  (5498) soft      (3401)      476 2023-02-15 18:53:58.000000 xcalibu-1.0.0/xcalibu/examples/undu_table.calib
+-rw-r--r--   0 guilloud  (5498) soft      (3401)      350 2023-03-28 10:57:47.000000 xcalibu-1.0.0/xcalibu/examples/unsorted_table.calib
+-rwxr-xr-x   0 guilloud  (5498) soft      (3401)     3095 2023-03-28 10:58:48.000000 xcalibu-1.0.0/xcalibu/test_xcalibu.py
+-rwxr-xr-x   0 guilloud  (5498) soft      (3401)    56072 2023-04-14 14:05:55.000000 xcalibu-1.0.0/xcalibu/xcalibu.py
+drwxr-xr-x   0 guilloud  (5498) soft      (3401)        0 2023-07-21 14:54:09.395892 xcalibu-1.0.0/xcalibu.egg-info/
+-rw-r--r--   0 guilloud  (5498) soft      (3401)     2868 2023-07-21 14:54:09.000000 xcalibu-1.0.0/xcalibu.egg-info/PKG-INFO
+-rw-r--r--   0 guilloud  (5498) soft      (3401)      931 2023-07-21 14:54:09.000000 xcalibu-1.0.0/xcalibu.egg-info/SOURCES.txt
+-rw-r--r--   0 guilloud  (5498) soft      (3401)        1 2023-07-21 14:54:09.000000 xcalibu-1.0.0/xcalibu.egg-info/dependency_links.txt
+-rw-r--r--   0 guilloud  (5498) soft      (3401)       89 2023-07-21 14:54:09.000000 xcalibu-1.0.0/xcalibu.egg-info/entry_points.txt
+-rw-r--r--   0 guilloud  (5498) soft      (3401)        8 2023-07-21 14:54:09.000000 xcalibu-1.0.0/xcalibu.egg-info/top_level.txt
```

### Comparing `xcalibu-0.9.9/LICENSE` & `xcalibu-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xcalibu-0.9.9/PKG-INFO` & `xcalibu-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: xcalibu
-Version: 0.9.9
+Version: 1.0.0
 Summary: Calibration library
 Home-page: https://github.com/cguilloud/xcalibu
 Author: Cyril Guilloud (ESRF-BCU)
 Author-email: prenom.name@truc.fr
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Xcalibu
```

### Comparing `xcalibu-0.9.9/README.md` & `xcalibu-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `xcalibu-0.9.9/setup.py` & `xcalibu-1.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name="xcalibu",
-    version="0.9.9",
+    version="1.0.0",
     description="Calibration library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/cguilloud/xcalibu",
     author="Cyril Guilloud (ESRF-BCU)",
     author_email="prenom.name@truc.fr",
     packages=setuptools.find_packages(),
     include_package_data=True,
     classifiers=[
-        "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3.7",
         "License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)",
         "Operating System :: OS Independent",
     ],
     entry_points={
         "console_scripts": [
             "xcalibu = xcalibu.xcalibu:main",
             "xcalibu_server = xcalibu.Xcalibuds:main",
```

### Comparing `xcalibu-0.9.9/tests/test_calib_table.py` & `xcalibu-1.0.0/tests/test_calib_table.py`

 * *Files identical despite different names*

### Comparing `xcalibu-0.9.9/xcalibu/Xcalibuds.py` & `xcalibu-1.0.0/xcalibu/Xcalibuds.py`

 * *Files identical despite different names*

### Comparing `xcalibu-0.9.9/xcalibu/demo_xcalibu.py` & `xcalibu-1.0.0/xcalibu/demo_xcalibu.py`

 * *Files identical despite different names*

### Comparing `xcalibu-0.9.9/xcalibu/device_test.py` & `xcalibu-1.0.0/xcalibu/device_test.py`

 * *Files identical despite different names*

### Comparing `xcalibu-0.9.9/xcalibu/examples/U32a_1_table.txt` & `xcalibu-1.0.0/xcalibu/examples/U32a_1_table.txt`

 * *Files identical despite different names*

### Comparing `xcalibu-0.9.9/xcalibu/examples/U32a_table_non_monotonic.txt` & `xcalibu-1.0.0/xcalibu/examples/U32a_table_non_monotonic.txt`

 * *Files identical despite different names*

### Comparing `xcalibu-0.9.9/xcalibu/examples/book5.txt` & `xcalibu-1.0.0/xcalibu/examples/book5.txt`

 * *Files identical despite different names*

### Comparing `xcalibu-0.9.9/xcalibu/examples/hpz_ring_Ry.calib` & `xcalibu-1.0.0/xcalibu/examples/hpz_ring_Ry.calib`

 * *Files identical despite different names*

### Comparing `xcalibu-0.9.9/xcalibu/examples/hpz_ring_Tz.calib` & `xcalibu-1.0.0/xcalibu/examples/hpz_ring_Tz.calib`

 * *Files identical despite different names*

### Comparing `xcalibu-0.9.9/xcalibu/test_xcalibu.py` & `xcalibu-1.0.0/xcalibu/test_xcalibu.py`

 * *Files identical despite different names*

### Comparing `xcalibu-0.9.9/xcalibu/xcalibu.py` & `xcalibu-1.0.0/xcalibu/xcalibu.py`

 * *Files identical despite different names*

### Comparing `xcalibu-0.9.9/xcalibu.egg-info/PKG-INFO` & `xcalibu-1.0.0/xcalibu.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: xcalibu
-Version: 0.9.9
+Version: 1.0.0
 Summary: Calibration library
 Home-page: https://github.com/cguilloud/xcalibu
 Author: Cyril Guilloud (ESRF-BCU)
 Author-email: prenom.name@truc.fr
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Xcalibu
```

### Comparing `xcalibu-0.9.9/xcalibu.egg-info/SOURCES.txt` & `xcalibu-1.0.0/xcalibu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

