# Comparing `tmp/tencentcloud-dlc-connector-1.0.4.tar.gz` & `tmp/tencentcloud-dlc-connector-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tencentcloud-dlc-connector-1.0.4.tar", last modified: Tue Jul 18 11:13:59 2023, max compression
+gzip compressed data, was "tencentcloud-dlc-connector-1.0.5.tar", last modified: Fri Jul 21 07:08:56 2023, max compression
```

## Comparing `tencentcloud-dlc-connector-1.0.4.tar` & `tencentcloud-dlc-connector-1.0.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 valux      (501) staff       (20)        0 2023-07-18 11:13:59.175625 tencentcloud-dlc-connector-1.0.4/
--rw-r--r--   0 valux      (501) staff       (20)     1509 2023-07-18 11:13:59.175408 tencentcloud-dlc-connector-1.0.4/PKG-INFO
--rw-r--r--   0 valux      (501) staff       (20)      593 2022-11-11 07:21:09.000000 tencentcloud-dlc-connector-1.0.4/README.md
--rw-r--r--   0 valux      (501) staff       (20)      921 2023-02-16 02:46:15.000000 tencentcloud-dlc-connector-1.0.4/README.rst
--rw-r--r--   0 valux      (501) staff       (20)       38 2023-07-18 11:13:59.175692 tencentcloud-dlc-connector-1.0.4/setup.cfg
--rw-r--r--   0 valux      (501) staff       (20)     1627 2023-07-18 09:52:03.000000 tencentcloud-dlc-connector-1.0.4/setup.py
-drwxr-xr-x   0 valux      (501) staff       (20)        0 2023-07-18 11:13:59.173959 tencentcloud-dlc-connector-1.0.4/tdlc_connector/
--rw-r--r--   0 valux      (501) staff       (20)     2970 2022-11-16 03:00:17.000000 tencentcloud-dlc-connector-1.0.4/tdlc_connector/__init__.py
--rw-r--r--   0 valux      (501) staff       (20)     8696 2022-12-29 06:21:04.000000 tencentcloud-dlc-connector-1.0.4/tdlc_connector/api.py
--rw-r--r--   0 valux      (501) staff       (20)     3980 2022-12-28 07:33:35.000000 tencentcloud-dlc-connector-1.0.4/tdlc_connector/connections.py
--rw-r--r--   0 valux      (501) staff       (20)     3224 2023-02-16 02:38:37.000000 tencentcloud-dlc-connector-1.0.4/tdlc_connector/constants.py
--rw-r--r--   0 valux      (501) staff       (20)     3840 2023-07-18 09:42:25.000000 tencentcloud-dlc-connector-1.0.4/tdlc_connector/cursors.py
--rw-r--r--   0 valux      (501) staff       (20)      428 2022-11-04 03:21:23.000000 tencentcloud-dlc-connector-1.0.4/tdlc_connector/exceptions.py
--rw-r--r--   0 valux      (501) staff       (20)     5157 2022-12-05 02:29:28.000000 tencentcloud-dlc-connector-1.0.4/tdlc_connector/formats.py
--rw-r--r--   0 valux      (501) staff       (20)     6901 2023-07-18 09:43:19.000000 tencentcloud-dlc-connector-1.0.4/tdlc_connector/results.py
--rw-r--r--   0 valux      (501) staff       (20)       17 2023-07-18 09:43:59.000000 tencentcloud-dlc-connector-1.0.4/tdlc_connector/version.py
-drwxr-xr-x   0 valux      (501) staff       (20)        0 2023-07-18 11:13:59.175111 tencentcloud-dlc-connector-1.0.4/tencentcloud_dlc_connector.egg-info/
--rw-r--r--   0 valux      (501) staff       (20)     1509 2023-07-18 11:13:59.000000 tencentcloud-dlc-connector-1.0.4/tencentcloud_dlc_connector.egg-info/PKG-INFO
--rw-r--r--   0 valux      (501) staff       (20)      518 2023-07-18 11:13:59.000000 tencentcloud-dlc-connector-1.0.4/tencentcloud_dlc_connector.egg-info/SOURCES.txt
--rw-r--r--   0 valux      (501) staff       (20)        1 2023-07-18 11:13:59.000000 tencentcloud-dlc-connector-1.0.4/tencentcloud_dlc_connector.egg-info/dependency_links.txt
--rw-r--r--   0 valux      (501) staff       (20)       42 2023-07-18 11:13:59.000000 tencentcloud-dlc-connector-1.0.4/tencentcloud_dlc_connector.egg-info/requires.txt
--rw-r--r--   0 valux      (501) staff       (20)       15 2023-07-18 11:13:59.000000 tencentcloud-dlc-connector-1.0.4/tencentcloud_dlc_connector.egg-info/top_level.txt
+drwxr-xr-x   0 valux      (501) staff       (20)        0 2023-07-21 07:08:56.071269 tencentcloud-dlc-connector-1.0.5/
+-rw-r--r--   0 valux      (501) staff       (20)     1488 2023-07-21 07:08:56.071093 tencentcloud-dlc-connector-1.0.5/PKG-INFO
+-rw-r--r--   0 valux      (501) staff       (20)      593 2022-11-11 07:21:09.000000 tencentcloud-dlc-connector-1.0.5/README.md
+-rw-r--r--   0 valux      (501) staff       (20)      921 2023-02-16 02:46:15.000000 tencentcloud-dlc-connector-1.0.5/README.rst
+-rw-r--r--   0 valux      (501) staff       (20)       38 2023-07-21 07:08:56.071321 tencentcloud-dlc-connector-1.0.5/setup.cfg
+-rw-r--r--   0 valux      (501) staff       (20)     1644 2023-07-21 07:07:29.000000 tencentcloud-dlc-connector-1.0.5/setup.py
+drwxr-xr-x   0 valux      (501) staff       (20)        0 2023-07-21 07:08:56.068343 tencentcloud-dlc-connector-1.0.5/tdlc_connector/
+-rw-r--r--   0 valux      (501) staff       (20)     2970 2022-11-16 03:00:17.000000 tencentcloud-dlc-connector-1.0.5/tdlc_connector/__init__.py
+-rw-r--r--   0 valux      (501) staff       (20)     8696 2022-12-29 06:21:04.000000 tencentcloud-dlc-connector-1.0.5/tdlc_connector/api.py
+-rw-r--r--   0 valux      (501) staff       (20)     3980 2022-12-28 07:33:35.000000 tencentcloud-dlc-connector-1.0.5/tdlc_connector/connections.py
+-rw-r--r--   0 valux      (501) staff       (20)     3224 2023-02-16 02:38:37.000000 tencentcloud-dlc-connector-1.0.5/tdlc_connector/constants.py
+-rw-r--r--   0 valux      (501) staff       (20)     3840 2023-07-18 09:42:25.000000 tencentcloud-dlc-connector-1.0.5/tdlc_connector/cursors.py
+-rw-r--r--   0 valux      (501) staff       (20)      428 2022-11-04 03:21:23.000000 tencentcloud-dlc-connector-1.0.5/tdlc_connector/exceptions.py
+-rw-r--r--   0 valux      (501) staff       (20)     5157 2022-12-05 02:29:28.000000 tencentcloud-dlc-connector-1.0.5/tdlc_connector/formats.py
+-rw-r--r--   0 valux      (501) staff       (20)     6901 2023-07-18 11:15:26.000000 tencentcloud-dlc-connector-1.0.5/tdlc_connector/results.py
+-rw-r--r--   0 valux      (501) staff       (20)       17 2023-07-21 07:08:22.000000 tencentcloud-dlc-connector-1.0.5/tdlc_connector/version.py
+drwxr-xr-x   0 valux      (501) staff       (20)        0 2023-07-21 07:08:56.070831 tencentcloud-dlc-connector-1.0.5/tencentcloud_dlc_connector.egg-info/
+-rw-r--r--   0 valux      (501) staff       (20)     1488 2023-07-21 07:08:56.000000 tencentcloud-dlc-connector-1.0.5/tencentcloud_dlc_connector.egg-info/PKG-INFO
+-rw-r--r--   0 valux      (501) staff       (20)      518 2023-07-21 07:08:56.000000 tencentcloud-dlc-connector-1.0.5/tencentcloud_dlc_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 valux      (501) staff       (20)        1 2023-07-21 07:08:56.000000 tencentcloud-dlc-connector-1.0.5/tencentcloud_dlc_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 valux      (501) staff       (20)       59 2023-07-21 07:08:56.000000 tencentcloud-dlc-connector-1.0.5/tencentcloud_dlc_connector.egg-info/requires.txt
+-rw-r--r--   0 valux      (501) staff       (20)       15 2023-07-21 07:08:56.000000 tencentcloud-dlc-connector-1.0.5/tencentcloud_dlc_connector.egg-info/top_level.txt
```

### Comparing `tencentcloud-dlc-connector-1.0.4/PKG-INFO` & `tencentcloud-dlc-connector-1.0.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 Metadata-Version: 2.1
 Name: tencentcloud-dlc-connector
-Version: 1.0.4
+Version: 1.0.5
 Summary: Tencentcloud DLC connector, connect to DLC engines using SQL.
-Home-page: UNKNOWN
 Author: Tencentcloud DLC Team.
 Maintainer-email: valuxzhao@tencent.com
 License: Apache License Version 2.0
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -53,9 +52,7 @@
     count = cursor.execute("SELECT 1")
     cursor.fetchone()
 
 
 
 
 
-
-
```

### Comparing `tencentcloud-dlc-connector-1.0.4/README.md` & `tencentcloud-dlc-connector-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `tencentcloud-dlc-connector-1.0.4/README.rst` & `tencentcloud-dlc-connector-1.0.5/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-dlc-connector-1.0.4/setup.py` & `tencentcloud-dlc-connector-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,16 +40,16 @@
     long_description=LONG_DESCRIPTION,
     author=AUTHOR,
     maintainer_email=MAINTAINER_EMAIL,
     packages=find_packages(exclude=["test*"]),
     platforms=PLATFORMS,
     license=LICENCE,
     install_requires=[
-        "tencentcloud-sdk-python",
-        "cos-python-sdk-v5"
+        "tencentcloud-sdk-python==3.0.918",
+        "cos-python-sdk-v5==1.9.20"
     ],
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: Apache Software License',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
```

### Comparing `tencentcloud-dlc-connector-1.0.4/tdlc_connector/__init__.py` & `tencentcloud-dlc-connector-1.0.5/tdlc_connector/__init__.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-dlc-connector-1.0.4/tdlc_connector/api.py` & `tencentcloud-dlc-connector-1.0.5/tdlc_connector/api.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-dlc-connector-1.0.4/tdlc_connector/connections.py` & `tencentcloud-dlc-connector-1.0.5/tdlc_connector/connections.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-dlc-connector-1.0.4/tdlc_connector/constants.py` & `tencentcloud-dlc-connector-1.0.5/tdlc_connector/constants.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-dlc-connector-1.0.4/tdlc_connector/cursors.py` & `tencentcloud-dlc-connector-1.0.5/tdlc_connector/cursors.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-dlc-connector-1.0.4/tdlc_connector/formats.py` & `tencentcloud-dlc-connector-1.0.5/tdlc_connector/formats.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-dlc-connector-1.0.4/tdlc_connector/results.py` & `tencentcloud-dlc-connector-1.0.5/tdlc_connector/results.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-dlc-connector-1.0.4/tencentcloud_dlc_connector.egg-info/PKG-INFO` & `tencentcloud-dlc-connector-1.0.5/tencentcloud_dlc_connector.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 Metadata-Version: 2.1
 Name: tencentcloud-dlc-connector
-Version: 1.0.4
+Version: 1.0.5
 Summary: Tencentcloud DLC connector, connect to DLC engines using SQL.
-Home-page: UNKNOWN
 Author: Tencentcloud DLC Team.
 Maintainer-email: valuxzhao@tencent.com
 License: Apache License Version 2.0
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -53,9 +52,7 @@
     count = cursor.execute("SELECT 1")
     cursor.fetchone()
 
 
 
 
 
-
-
```

### Comparing `tencentcloud-dlc-connector-1.0.4/tencentcloud_dlc_connector.egg-info/SOURCES.txt` & `tencentcloud-dlc-connector-1.0.5/tencentcloud_dlc_connector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

