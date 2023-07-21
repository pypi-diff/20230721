# Comparing `tmp/photos_where-1.4.tar.gz` & `tmp/photos_where-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "photos_where-1.4.tar", last modified: Fri Jul 21 13:04:14 2023, max compression
+gzip compressed data, was "photos_where-1.5.tar", last modified: Fri Jul 21 13:08:24 2023, max compression
```

## Comparing `photos_where-1.4.tar` & `photos_where-1.5.tar`

### file list

```diff
@@ -1,19 +1,18 @@
-drwxr-xr-x   0 visgean    (501) staff       (20)        0 2023-07-21 13:04:14.933468 photos_where-1.4/
--rw-r--r--   0 visgean    (501) staff       (20)     1063 2022-09-28 18:42:28.000000 photos_where-1.4/LICENSE
--rw-r--r--   0 visgean    (501) staff       (20)       84 2023-07-21 13:03:26.000000 photos_where-1.4/MANIFEST.in
--rw-r--r--   0 visgean    (501) staff       (20)     1943 2023-07-21 13:04:14.933336 photos_where-1.4/PKG-INFO
--rw-r--r--   0 visgean    (501) staff       (20)     1253 2023-07-01 21:31:17.000000 photos_where-1.4/README.md
-drwxr-xr-x   0 visgean    (501) staff       (20)        0 2023-07-21 13:04:14.932415 photos_where-1.4/photos_where/
--rw-r--r--   0 visgean    (501) staff       (20)       25 2023-06-30 22:30:00.000000 photos_where-1.4/photos_where/__init__.py
--rw-r--r--   0 visgean    (501) staff       (20)  7852501 2022-01-28 14:20:56.000000 photos_where-1.4/photos_where/cities.csv
--rwxr-xr-x   0 visgean    (501) staff       (20)     2037 2023-06-30 18:47:13.000000 photos_where-1.4/photos_where/main.py
--rw-r--r--   0 visgean    (501) staff       (20)     5152 2023-07-01 22:17:33.000000 photos_where-1.4/photos_where/where.py
-drwxr-xr-x   0 visgean    (501) staff       (20)        0 2023-07-21 13:04:14.933177 photos_where-1.4/photos_where.egg-info/
--rw-r--r--   0 visgean    (501) staff       (20)     1943 2023-07-21 13:04:14.000000 photos_where-1.4/photos_where.egg-info/PKG-INFO
--rw-r--r--   0 visgean    (501) staff       (20)      348 2023-07-21 13:04:14.000000 photos_where-1.4/photos_where.egg-info/SOURCES.txt
--rw-r--r--   0 visgean    (501) staff       (20)        1 2023-07-21 13:04:14.000000 photos_where-1.4/photos_where.egg-info/dependency_links.txt
--rw-r--r--   0 visgean    (501) staff       (20)       57 2023-07-21 13:04:14.000000 photos_where-1.4/photos_where.egg-info/entry_points.txt
--rw-r--r--   0 visgean    (501) staff       (20)       62 2023-07-21 13:04:14.000000 photos_where-1.4/photos_where.egg-info/requires.txt
--rw-r--r--   0 visgean    (501) staff       (20)       13 2023-07-21 13:04:14.000000 photos_where-1.4/photos_where.egg-info/top_level.txt
--rw-r--r--   0 visgean    (501) staff       (20)       38 2023-07-21 13:04:14.933509 photos_where-1.4/setup.cfg
--rw-r--r--   0 visgean    (501) staff       (20)     1036 2023-07-21 13:03:58.000000 photos_where-1.4/setup.py
+drwxr-xr-x   0 visgean    (501) staff       (20)        0 2023-07-21 13:08:24.403208 photos_where-1.5/
+-rw-r--r--   0 visgean    (501) staff       (20)     1063 2022-09-28 18:42:28.000000 photos_where-1.5/LICENSE
+-rw-r--r--   0 visgean    (501) staff       (20)       48 2023-07-21 13:07:36.000000 photos_where-1.5/MANIFEST.in
+-rw-r--r--   0 visgean    (501) staff       (20)     1943 2023-07-21 13:08:24.403087 photos_where-1.5/PKG-INFO
+-rw-r--r--   0 visgean    (501) staff       (20)     1253 2023-07-01 21:31:17.000000 photos_where-1.5/README.md
+drwxr-xr-x   0 visgean    (501) staff       (20)        0 2023-07-21 13:08:24.402184 photos_where-1.5/photos_where/
+-rw-r--r--   0 visgean    (501) staff       (20)       25 2023-06-30 22:30:00.000000 photos_where-1.5/photos_where/__init__.py
+-rwxr-xr-x   0 visgean    (501) staff       (20)     2037 2023-06-30 18:47:13.000000 photos_where-1.5/photos_where/main.py
+-rw-r--r--   0 visgean    (501) staff       (20)     5152 2023-07-01 22:17:33.000000 photos_where-1.5/photos_where/where.py
+drwxr-xr-x   0 visgean    (501) staff       (20)        0 2023-07-21 13:08:24.402916 photos_where-1.5/photos_where.egg-info/
+-rw-r--r--   0 visgean    (501) staff       (20)     1943 2023-07-21 13:08:24.000000 photos_where-1.5/photos_where.egg-info/PKG-INFO
+-rw-r--r--   0 visgean    (501) staff       (20)      324 2023-07-21 13:08:24.000000 photos_where-1.5/photos_where.egg-info/SOURCES.txt
+-rw-r--r--   0 visgean    (501) staff       (20)        1 2023-07-21 13:08:24.000000 photos_where-1.5/photos_where.egg-info/dependency_links.txt
+-rw-r--r--   0 visgean    (501) staff       (20)       57 2023-07-21 13:08:24.000000 photos_where-1.5/photos_where.egg-info/entry_points.txt
+-rw-r--r--   0 visgean    (501) staff       (20)       62 2023-07-21 13:08:24.000000 photos_where-1.5/photos_where.egg-info/requires.txt
+-rw-r--r--   0 visgean    (501) staff       (20)       13 2023-07-21 13:08:24.000000 photos_where-1.5/photos_where.egg-info/top_level.txt
+-rw-r--r--   0 visgean    (501) staff       (20)       38 2023-07-21 13:08:24.403243 photos_where-1.5/setup.cfg
+-rw-r--r--   0 visgean    (501) staff       (20)     1036 2023-07-21 13:08:21.000000 photos_where-1.5/setup.py
```

### Comparing `photos_where-1.4/LICENSE` & `photos_where-1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `photos_where-1.4/PKG-INFO` & `photos_where-1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: photos_where
-Version: 1.4
+Version: 1.5
 Summary: Analyze exif data
 Home-page: https://github.com/visgean/where
 Author: Visgean
 Author-email: visgean@gmail.com
 License: MIT
 Description: # Where - day by day location from your photos
```

### Comparing `photos_where-1.4/README.md` & `photos_where-1.5/README.md`

 * *Files identical despite different names*

### Comparing `photos_where-1.4/photos_where/main.py` & `photos_where-1.5/photos_where/main.py`

 * *Files identical despite different names*

### Comparing `photos_where-1.4/photos_where/where.py` & `photos_where-1.5/photos_where/where.py`

 * *Files identical despite different names*

### Comparing `photos_where-1.4/photos_where.egg-info/PKG-INFO` & `photos_where-1.5/photos_where.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: photos-where
-Version: 1.4
+Version: 1.5
 Summary: Analyze exif data
 Home-page: https://github.com/visgean/where
 Author: Visgean
 Author-email: visgean@gmail.com
 License: MIT
 Description: # Where - day by day location from your photos
```

### Comparing `photos_where-1.4/setup.py` & `photos_where-1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     from distutils.core import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="photos_where",
-    version="1.4",
+    version="1.5",
     description="Analyze exif data",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Visgean",
     author_email="visgean@gmail.com",
     url="https://github.com/visgean/where",
     packages=[
```

