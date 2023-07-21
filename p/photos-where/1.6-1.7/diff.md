# Comparing `tmp/photos_where-1.6.tar.gz` & `tmp/photos_where-1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "photos_where-1.6.tar", last modified: Fri Jul 21 13:09:50 2023, max compression
+gzip compressed data, was "photos_where-1.7.tar", last modified: Fri Jul 21 13:12:22 2023, max compression
```

## Comparing `photos_where-1.6.tar` & `photos_where-1.7.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 visgean    (501) staff       (20)        0 2023-07-21 13:09:50.951568 photos_where-1.6/
--rw-r--r--   0 visgean    (501) staff       (20)     1063 2022-09-28 18:42:28.000000 photos_where-1.6/LICENSE
--rw-r--r--   0 visgean    (501) staff       (20)       53 2023-07-21 13:09:42.000000 photos_where-1.6/MANIFEST.in
--rw-r--r--   0 visgean    (501) staff       (20)     1943 2023-07-21 13:09:50.951447 photos_where-1.6/PKG-INFO
--rw-r--r--   0 visgean    (501) staff       (20)     1253 2023-07-01 21:31:17.000000 photos_where-1.6/README.md
-drwxr-xr-x   0 visgean    (501) staff       (20)        0 2023-07-21 13:09:50.950639 photos_where-1.6/photos_where/
--rw-r--r--   0 visgean    (501) staff       (20)       25 2023-06-30 22:30:00.000000 photos_where-1.6/photos_where/__init__.py
--rwxr-xr-x   0 visgean    (501) staff       (20)     2037 2023-06-30 18:47:13.000000 photos_where-1.6/photos_where/main.py
--rw-r--r--   0 visgean    (501) staff       (20)     5152 2023-07-01 22:17:33.000000 photos_where-1.6/photos_where/where.py
-drwxr-xr-x   0 visgean    (501) staff       (20)        0 2023-07-21 13:09:50.951272 photos_where-1.6/photos_where.egg-info/
--rw-r--r--   0 visgean    (501) staff       (20)     1943 2023-07-21 13:09:50.000000 photos_where-1.6/photos_where.egg-info/PKG-INFO
--rw-r--r--   0 visgean    (501) staff       (20)      324 2023-07-21 13:09:50.000000 photos_where-1.6/photos_where.egg-info/SOURCES.txt
--rw-r--r--   0 visgean    (501) staff       (20)        1 2023-07-21 13:09:50.000000 photos_where-1.6/photos_where.egg-info/dependency_links.txt
--rw-r--r--   0 visgean    (501) staff       (20)       57 2023-07-21 13:09:50.000000 photos_where-1.6/photos_where.egg-info/entry_points.txt
--rw-r--r--   0 visgean    (501) staff       (20)       62 2023-07-21 13:09:50.000000 photos_where-1.6/photos_where.egg-info/requires.txt
--rw-r--r--   0 visgean    (501) staff       (20)       13 2023-07-21 13:09:50.000000 photos_where-1.6/photos_where.egg-info/top_level.txt
--rw-r--r--   0 visgean    (501) staff       (20)       38 2023-07-21 13:09:50.951603 photos_where-1.6/setup.cfg
--rw-r--r--   0 visgean    (501) staff       (20)     1036 2023-07-21 13:09:42.000000 photos_where-1.6/setup.py
+drwxr-xr-x   0 visgean    (501) staff       (20)        0 2023-07-21 13:12:22.478248 photos_where-1.7/
+-rw-r--r--   0 visgean    (501) staff       (20)     1063 2022-09-28 18:42:28.000000 photos_where-1.7/LICENSE
+-rw-r--r--   0 visgean    (501) staff       (20)       66 2023-07-21 13:11:27.000000 photos_where-1.7/MANIFEST.in
+-rw-r--r--   0 visgean    (501) staff       (20)     1943 2023-07-21 13:12:22.478114 photos_where-1.7/PKG-INFO
+-rw-r--r--   0 visgean    (501) staff       (20)     1253 2023-07-01 21:31:17.000000 photos_where-1.7/README.md
+drwxr-xr-x   0 visgean    (501) staff       (20)        0 2023-07-21 13:12:22.477319 photos_where-1.7/photos_where/
+-rw-r--r--   0 visgean    (501) staff       (20)       25 2023-06-30 22:30:00.000000 photos_where-1.7/photos_where/__init__.py
+-rw-r--r--   0 visgean    (501) staff       (20)  7852501 2022-01-28 14:20:56.000000 photos_where-1.7/photos_where/cities.csv
+-rwxr-xr-x   0 visgean    (501) staff       (20)     2037 2023-06-30 18:47:13.000000 photos_where-1.7/photos_where/main.py
+-rw-r--r--   0 visgean    (501) staff       (20)     5152 2023-07-01 22:17:33.000000 photos_where-1.7/photos_where/where.py
+drwxr-xr-x   0 visgean    (501) staff       (20)        0 2023-07-21 13:12:22.477939 photos_where-1.7/photos_where.egg-info/
+-rw-r--r--   0 visgean    (501) staff       (20)     1943 2023-07-21 13:12:22.000000 photos_where-1.7/photos_where.egg-info/PKG-INFO
+-rw-r--r--   0 visgean    (501) staff       (20)      348 2023-07-21 13:12:22.000000 photos_where-1.7/photos_where.egg-info/SOURCES.txt
+-rw-r--r--   0 visgean    (501) staff       (20)        1 2023-07-21 13:12:22.000000 photos_where-1.7/photos_where.egg-info/dependency_links.txt
+-rw-r--r--   0 visgean    (501) staff       (20)       57 2023-07-21 13:12:22.000000 photos_where-1.7/photos_where.egg-info/entry_points.txt
+-rw-r--r--   0 visgean    (501) staff       (20)       62 2023-07-21 13:12:22.000000 photos_where-1.7/photos_where.egg-info/requires.txt
+-rw-r--r--   0 visgean    (501) staff       (20)       13 2023-07-21 13:12:22.000000 photos_where-1.7/photos_where.egg-info/top_level.txt
+-rw-r--r--   0 visgean    (501) staff       (20)       38 2023-07-21 13:12:22.478284 photos_where-1.7/setup.cfg
+-rw-r--r--   0 visgean    (501) staff       (20)     1036 2023-07-21 13:12:16.000000 photos_where-1.7/setup.py
```

### Comparing `photos_where-1.6/LICENSE` & `photos_where-1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `photos_where-1.6/PKG-INFO` & `photos_where-1.7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: photos_where
-Version: 1.6
+Version: 1.7
 Summary: Analyze exif data
 Home-page: https://github.com/visgean/where
 Author: Visgean
 Author-email: visgean@gmail.com
 License: MIT
 Description: # Where - day by day location from your photos
```

### Comparing `photos_where-1.6/README.md` & `photos_where-1.7/README.md`

 * *Files identical despite different names*

### Comparing `photos_where-1.6/photos_where/main.py` & `photos_where-1.7/photos_where/main.py`

 * *Files identical despite different names*

### Comparing `photos_where-1.6/photos_where/where.py` & `photos_where-1.7/photos_where/where.py`

 * *Files identical despite different names*

### Comparing `photos_where-1.6/photos_where.egg-info/PKG-INFO` & `photos_where-1.7/photos_where.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: photos-where
-Version: 1.6
+Version: 1.7
 Summary: Analyze exif data
 Home-page: https://github.com/visgean/where
 Author: Visgean
 Author-email: visgean@gmail.com
 License: MIT
 Description: # Where - day by day location from your photos
```

### Comparing `photos_where-1.6/setup.py` & `photos_where-1.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     from distutils.core import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="photos_where",
-    version="1.6",
+    version="1.7",
     description="Analyze exif data",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Visgean",
     author_email="visgean@gmail.com",
     url="https://github.com/visgean/where",
     packages=[
```

