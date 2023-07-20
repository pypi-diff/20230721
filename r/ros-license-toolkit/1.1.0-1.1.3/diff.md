# Comparing `tmp/ros_license_toolkit-1.1.0.tar.gz` & `tmp/ros_license_toolkit-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ros_license_toolkit-1.1.0.tar", last modified: Thu Jul 20 18:41:57 2023, max compression
+gzip compressed data, was "ros_license_toolkit-1.1.3.tar", last modified: Thu Jul 20 22:02:37 2023, max compression
```

## Comparing `ros_license_toolkit-1.1.0.tar` & `ros_license_toolkit-1.1.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 hec2le    (1002) hec2le    (1002)        0 2023-07-20 18:41:57.006402 ros_license_toolkit-1.1.0/
--rw-rw-r--   0 hec2le    (1002) hec2le    (1002)    11358 2022-12-12 09:53:16.000000 ros_license_toolkit-1.1.0/LICENSE
--rw-rw-r--   0 hec2le    (1002) hec2le    (1002)      993 2023-03-30 14:25:23.000000 ros_license_toolkit-1.1.0/NOTICE
--rw-rw-r--   0 hec2le    (1002) hec2le    (1002)    18314 2023-07-20 18:41:57.006402 ros_license_toolkit-1.1.0/PKG-INFO
--rw-rw-r--   0 hec2le    (1002) hec2le    (1002)     4269 2023-07-20 18:36:04.000000 ros_license_toolkit-1.1.0/README.md
--rw-rw-r--   0 hec2le    (1002) hec2le    (1002)     1556 2023-07-20 18:37:26.000000 ros_license_toolkit-1.1.0/pyproject.toml
--rw-rw-r--   0 hec2le    (1002) hec2le    (1002)      319 2023-07-20 18:41:57.006402 ros_license_toolkit-1.1.0/setup.cfg
-drwxrwxr-x   0 hec2le    (1002) hec2le    (1002)        0 2023-07-20 18:41:57.002402 ros_license_toolkit-1.1.0/src/
-drwxrwxr-x   0 hec2le    (1002) hec2le    (1002)        0 2023-07-20 18:41:57.002402 ros_license_toolkit-1.1.0/src/ros_license_toolkit/
--rw-rw-r--   0 hec2le    (1002) hec2le    (1002)       22 2023-07-20 18:37:26.000000 ros_license_toolkit-1.1.0/src/ros_license_toolkit/__init__.py
--rw-rw-r--   0 hec2le    (1002) hec2le    (1002)    10580 2023-07-20 14:38:25.000000 ros_license_toolkit-1.1.0/src/ros_license_toolkit/checks.py
--rw-rw-r--   0 hec2le    (1002) hec2le    (1002)     1083 2023-03-30 14:25:30.000000 ros_license_toolkit-1.1.0/src/ros_license_toolkit/common.py
--rw-rw-r--   0 hec2le    (1002) hec2le    (1002)     2966 2023-07-20 18:36:04.000000 ros_license_toolkit-1.1.0/src/ros_license_toolkit/copyright.py
--rw-rw-r--   0 hec2le    (1002) hec2le    (1002)     5487 2023-07-20 18:36:04.000000 ros_license_toolkit-1.1.0/src/ros_license_toolkit/license_tag.py
--rw-rw-r--   0 hec2le    (1002) hec2le    (1002)     5167 2023-07-20 18:36:04.000000 ros_license_toolkit-1.1.0/src/ros_license_toolkit/main.py
--rw-rw-r--   0 hec2le    (1002) hec2le    (1002)    10048 2023-07-20 18:36:04.000000 ros_license_toolkit-1.1.0/src/ros_license_toolkit/package.py
--rw-rw-r--   0 hec2le    (1002) hec2le    (1002)     3081 2023-04-21 17:10:05.000000 ros_license_toolkit-1.1.0/src/ros_license_toolkit/repo.py
--rw-rw-r--   0 hec2le    (1002) hec2le    (1002)     1830 2023-07-20 14:38:25.000000 ros_license_toolkit-1.1.0/src/ros_license_toolkit/ui_elements.py
-drwxrwxr-x   0 hec2le    (1002) hec2le    (1002)        0 2023-07-20 18:41:57.006402 ros_license_toolkit-1.1.0/src/ros_license_toolkit.egg-info/
--rw-rw-r--   0 hec2le    (1002) hec2le    (1002)    18314 2023-07-20 18:41:56.000000 ros_license_toolkit-1.1.0/src/ros_license_toolkit.egg-info/PKG-INFO
--rw-rw-r--   0 hec2le    (1002) hec2le    (1002)      651 2023-07-20 18:41:57.000000 ros_license_toolkit-1.1.0/src/ros_license_toolkit.egg-info/SOURCES.txt
--rw-rw-r--   0 hec2le    (1002) hec2le    (1002)        1 2023-07-20 18:41:56.000000 ros_license_toolkit-1.1.0/src/ros_license_toolkit.egg-info/dependency_links.txt
--rw-rw-r--   0 hec2le    (1002) hec2le    (1002)       70 2023-07-20 18:41:56.000000 ros_license_toolkit-1.1.0/src/ros_license_toolkit.egg-info/entry_points.txt
--rw-rw-r--   0 hec2le    (1002) hec2le    (1002)      116 2023-07-20 18:41:56.000000 ros_license_toolkit-1.1.0/src/ros_license_toolkit.egg-info/requires.txt
--rw-rw-r--   0 hec2le    (1002) hec2le    (1002)       20 2023-07-20 18:41:56.000000 ros_license_toolkit-1.1.0/src/ros_license_toolkit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:02:37.784420 ros_license_toolkit-1.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-20 22:02:25.000000 ros_license_toolkit-1.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-20 22:02:25.000000 ros_license_toolkit-1.1.3/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)    18314 2023-07-20 22:02:37.784420 ros_license_toolkit-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4269 2023-07-20 22:02:25.000000 ros_license_toolkit-1.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-07-20 22:02:25.000000 ros_license_toolkit-1.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-20 22:02:37.784420 ros_license_toolkit-1.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:02:37.780420 ros_license_toolkit-1.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:02:37.780420 ros_license_toolkit-1.1.3/src/ros_license_toolkit/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-20 22:02:25.000000 ros_license_toolkit-1.1.3/src/ros_license_toolkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10580 2023-07-20 22:02:25.000000 ros_license_toolkit-1.1.3/src/ros_license_toolkit/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-20 22:02:25.000000 ros_license_toolkit-1.1.3/src/ros_license_toolkit/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-07-20 22:02:25.000000 ros_license_toolkit-1.1.3/src/ros_license_toolkit/copyright.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5487 2023-07-20 22:02:25.000000 ros_license_toolkit-1.1.3/src/ros_license_toolkit/license_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5167 2023-07-20 22:02:25.000000 ros_license_toolkit-1.1.3/src/ros_license_toolkit/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10048 2023-07-20 22:02:25.000000 ros_license_toolkit-1.1.3/src/ros_license_toolkit/package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-07-20 22:02:25.000000 ros_license_toolkit-1.1.3/src/ros_license_toolkit/repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-07-20 22:02:25.000000 ros_license_toolkit-1.1.3/src/ros_license_toolkit/ui_elements.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:02:37.784420 ros_license_toolkit-1.1.3/src/ros_license_toolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18314 2023-07-20 22:02:37.000000 ros_license_toolkit-1.1.3/src/ros_license_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-20 22:02:37.000000 ros_license_toolkit-1.1.3/src/ros_license_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 22:02:37.000000 ros_license_toolkit-1.1.3/src/ros_license_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-20 22:02:37.000000 ros_license_toolkit-1.1.3/src/ros_license_toolkit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-20 22:02:37.000000 ros_license_toolkit-1.1.3/src/ros_license_toolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-20 22:02:37.000000 ros_license_toolkit-1.1.3/src/ros_license_toolkit.egg-info/top_level.txt
```

### Comparing `ros_license_toolkit-1.1.0/LICENSE` & `ros_license_toolkit-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ros_license_toolkit-1.1.0/NOTICE` & `ros_license_toolkit-1.1.3/NOTICE`

 * *Files identical despite different names*

### Comparing `ros_license_toolkit-1.1.0/PKG-INFO` & `ros_license_toolkit-1.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros_license_toolkit
-Version: 1.1.0
+Version: 1.1.3
 Summary: Checks ROS packages for correct license declaration.
 Author-email: Christian Henkel <christian.henkel2@de.bosch.com>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `ros_license_toolkit-1.1.0/README.md` & `ros_license_toolkit-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `ros_license_toolkit-1.1.0/pyproject.toml` & `ros_license_toolkit-1.1.3/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ros_license_toolkit"
-version = "1.1.0"
+version = "1.1.3"
 description = "Checks ROS packages for correct license declaration."
 readme = "README.md"
 authors = [
     {name = "Christian Henkel", email = "christian.henkel2@de.bosch.com"},
 ]
 license = {file = "LICENSE"}
 classifiers = [
```

### Comparing `ros_license_toolkit-1.1.0/src/ros_license_toolkit/checks.py` & `ros_license_toolkit-1.1.3/src/ros_license_toolkit/checks.py`

 * *Files identical despite different names*

### Comparing `ros_license_toolkit-1.1.0/src/ros_license_toolkit/common.py` & `ros_license_toolkit-1.1.3/src/ros_license_toolkit/common.py`

 * *Files identical despite different names*

### Comparing `ros_license_toolkit-1.1.0/src/ros_license_toolkit/copyright.py` & `ros_license_toolkit-1.1.3/src/ros_license_toolkit/copyright.py`

 * *Files identical despite different names*

### Comparing `ros_license_toolkit-1.1.0/src/ros_license_toolkit/license_tag.py` & `ros_license_toolkit-1.1.3/src/ros_license_toolkit/license_tag.py`

 * *Files identical despite different names*

### Comparing `ros_license_toolkit-1.1.0/src/ros_license_toolkit/main.py` & `ros_license_toolkit-1.1.3/src/ros_license_toolkit/main.py`

 * *Files identical despite different names*

### Comparing `ros_license_toolkit-1.1.0/src/ros_license_toolkit/package.py` & `ros_license_toolkit-1.1.3/src/ros_license_toolkit/package.py`

 * *Files identical despite different names*

### Comparing `ros_license_toolkit-1.1.0/src/ros_license_toolkit/repo.py` & `ros_license_toolkit-1.1.3/src/ros_license_toolkit/repo.py`

 * *Files identical despite different names*

### Comparing `ros_license_toolkit-1.1.0/src/ros_license_toolkit/ui_elements.py` & `ros_license_toolkit-1.1.3/src/ros_license_toolkit/ui_elements.py`

 * *Files identical despite different names*

### Comparing `ros_license_toolkit-1.1.0/src/ros_license_toolkit.egg-info/PKG-INFO` & `ros_license_toolkit-1.1.3/src/ros_license_toolkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-license-toolkit
-Version: 1.1.0
+Version: 1.1.3
 Summary: Checks ROS packages for correct license declaration.
 Author-email: Christian Henkel <christian.henkel2@de.bosch.com>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `ros_license_toolkit-1.1.0/src/ros_license_toolkit.egg-info/SOURCES.txt` & `ros_license_toolkit-1.1.3/src/ros_license_toolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

