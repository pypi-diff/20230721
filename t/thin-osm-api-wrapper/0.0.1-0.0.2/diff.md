# Comparing `tmp/thin_osm_api_wrapper-0.0.1.tar.gz` & `tmp/thin_osm_api_wrapper-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thin_osm_api_wrapper-0.0.1.tar", last modified: Sat Dec 24 14:34:58 2022, max compression
+gzip compressed data, was "thin_osm_api_wrapper-0.0.2.tar", last modified: Fri Jul 21 14:58:39 2023, max compression
```

## Comparing `thin_osm_api_wrapper-0.0.1.tar` & `thin_osm_api_wrapper-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 mateusz   (1000) mateusz   (1001)        0 2022-12-24 14:34:58.731823 thin_osm_api_wrapper-0.0.1/
--rw-rw-r--   0 mateusz   (1000) mateusz   (1001)     1250 2022-12-24 14:34:58.730823 thin_osm_api_wrapper-0.0.1/PKG-INFO
--rw-rw-r--   0 mateusz   (1000) mateusz   (1001)      607 2022-12-24 14:33:51.000000 thin_osm_api_wrapper-0.0.1/README.md
--rw-rw-r--   0 mateusz   (1000) mateusz   (1001)       38 2022-12-24 14:34:58.731823 thin_osm_api_wrapper-0.0.1/setup.cfg
--rw-rw-r--   0 mateusz   (1000) mateusz   (1001)      740 2022-12-24 14:26:01.000000 thin_osm_api_wrapper-0.0.1/setup.py
-drwxrwxr-x   0 mateusz   (1000) mateusz   (1001)        0 2022-12-24 14:34:58.730823 thin_osm_api_wrapper-0.0.1/thin_osm_api_wrapper/
--rw-rw-r--   0 mateusz   (1000) mateusz   (1001)       31 2022-12-24 14:34:38.000000 thin_osm_api_wrapper-0.0.1/thin_osm_api_wrapper/__init__.py
--rw-rw-r--   0 mateusz   (1000) mateusz   (1001)      504 2022-12-24 14:28:09.000000 thin_osm_api_wrapper-0.0.1/thin_osm_api_wrapper/api.py
-drwxrwxr-x   0 mateusz   (1000) mateusz   (1001)        0 2022-12-24 14:34:58.730823 thin_osm_api_wrapper-0.0.1/thin_osm_api_wrapper.egg-info/
--rw-rw-r--   0 mateusz   (1000) mateusz   (1001)     1250 2022-12-24 14:34:58.000000 thin_osm_api_wrapper-0.0.1/thin_osm_api_wrapper.egg-info/PKG-INFO
--rw-rw-r--   0 mateusz   (1000) mateusz   (1001)      255 2022-12-24 14:34:58.000000 thin_osm_api_wrapper-0.0.1/thin_osm_api_wrapper.egg-info/SOURCES.txt
--rw-rw-r--   0 mateusz   (1000) mateusz   (1001)        1 2022-12-24 14:34:58.000000 thin_osm_api_wrapper-0.0.1/thin_osm_api_wrapper.egg-info/dependency_links.txt
--rw-rw-r--   0 mateusz   (1000) mateusz   (1001)       21 2022-12-24 14:34:58.000000 thin_osm_api_wrapper-0.0.1/thin_osm_api_wrapper.egg-info/top_level.txt
+drwxrwxr-x   0 mateusz   (1000) mateusz   (1001)        0 2023-07-21 14:58:39.410879 thin_osm_api_wrapper-0.0.2/
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1001)     2290 2023-07-21 14:58:39.410879 thin_osm_api_wrapper-0.0.2/PKG-INFO
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1001)     1383 2023-03-06 02:35:50.000000 thin_osm_api_wrapper-0.0.2/README.md
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1001)       38 2023-07-21 14:58:39.411879 thin_osm_api_wrapper-0.0.2/setup.cfg
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1001)      740 2023-07-21 14:58:26.000000 thin_osm_api_wrapper-0.0.2/setup.py
+drwxrwxr-x   0 mateusz   (1000) mateusz   (1001)        0 2023-07-21 14:58:39.409880 thin_osm_api_wrapper-0.0.2/thin_osm_api_wrapper/
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1001)       31 2022-12-24 14:34:38.000000 thin_osm_api_wrapper-0.0.2/thin_osm_api_wrapper/__init__.py
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1001)     4308 2023-03-06 02:35:28.000000 thin_osm_api_wrapper-0.0.2/thin_osm_api_wrapper/api.py
+drwxrwxr-x   0 mateusz   (1000) mateusz   (1001)        0 2023-07-21 14:58:39.410879 thin_osm_api_wrapper-0.0.2/thin_osm_api_wrapper.egg-info/
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1001)     2290 2023-07-21 14:58:39.000000 thin_osm_api_wrapper-0.0.2/thin_osm_api_wrapper.egg-info/PKG-INFO
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1001)      255 2023-07-21 14:58:39.000000 thin_osm_api_wrapper-0.0.2/thin_osm_api_wrapper.egg-info/SOURCES.txt
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1001)        1 2023-07-21 14:58:39.000000 thin_osm_api_wrapper-0.0.2/thin_osm_api_wrapper.egg-info/dependency_links.txt
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1001)       21 2023-07-21 14:58:39.000000 thin_osm_api_wrapper-0.0.2/thin_osm_api_wrapper.egg-info/top_level.txt
```

### Comparing `thin_osm_api_wrapper-0.0.1/setup.py` & `thin_osm_api_wrapper-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="thin_osm_api_wrapper",
-    version="0.0.1",
+    version="0.0.2",
     author="Mateusz Konieczny",
     description="thin wrapper of https://wiki.openstreetmap.org/wiki/API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/matkoniecz/thin_osm_api_python_wrapper",
     packages=setuptools.find_packages(),
     classifiers=[
```

