# Comparing `tmp/thin_osm_api_wrapper-0.0.2.tar.gz` & `tmp/thin_osm_api_wrapper-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thin_osm_api_wrapper-0.0.2.tar", last modified: Fri Jul 21 14:58:39 2023, max compression
+gzip compressed data, was "thin_osm_api_wrapper-0.0.3.tar", last modified: Fri Jul 21 15:08:12 2023, max compression
```

## Comparing `thin_osm_api_wrapper-0.0.2.tar` & `thin_osm_api_wrapper-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 mateusz   (1000) mateusz   (1001)        0 2023-07-21 14:58:39.410879 thin_osm_api_wrapper-0.0.2/
--rw-rw-r--   0 mateusz   (1000) mateusz   (1001)     2290 2023-07-21 14:58:39.410879 thin_osm_api_wrapper-0.0.2/PKG-INFO
--rw-rw-r--   0 mateusz   (1000) mateusz   (1001)     1383 2023-03-06 02:35:50.000000 thin_osm_api_wrapper-0.0.2/README.md
--rw-rw-r--   0 mateusz   (1000) mateusz   (1001)       38 2023-07-21 14:58:39.411879 thin_osm_api_wrapper-0.0.2/setup.cfg
--rw-rw-r--   0 mateusz   (1000) mateusz   (1001)      740 2023-07-21 14:58:26.000000 thin_osm_api_wrapper-0.0.2/setup.py
-drwxrwxr-x   0 mateusz   (1000) mateusz   (1001)        0 2023-07-21 14:58:39.409880 thin_osm_api_wrapper-0.0.2/thin_osm_api_wrapper/
--rw-rw-r--   0 mateusz   (1000) mateusz   (1001)       31 2022-12-24 14:34:38.000000 thin_osm_api_wrapper-0.0.2/thin_osm_api_wrapper/__init__.py
--rw-rw-r--   0 mateusz   (1000) mateusz   (1001)     4308 2023-03-06 02:35:28.000000 thin_osm_api_wrapper-0.0.2/thin_osm_api_wrapper/api.py
-drwxrwxr-x   0 mateusz   (1000) mateusz   (1001)        0 2023-07-21 14:58:39.410879 thin_osm_api_wrapper-0.0.2/thin_osm_api_wrapper.egg-info/
--rw-rw-r--   0 mateusz   (1000) mateusz   (1001)     2290 2023-07-21 14:58:39.000000 thin_osm_api_wrapper-0.0.2/thin_osm_api_wrapper.egg-info/PKG-INFO
--rw-rw-r--   0 mateusz   (1000) mateusz   (1001)      255 2023-07-21 14:58:39.000000 thin_osm_api_wrapper-0.0.2/thin_osm_api_wrapper.egg-info/SOURCES.txt
--rw-rw-r--   0 mateusz   (1000) mateusz   (1001)        1 2023-07-21 14:58:39.000000 thin_osm_api_wrapper-0.0.2/thin_osm_api_wrapper.egg-info/dependency_links.txt
--rw-rw-r--   0 mateusz   (1000) mateusz   (1001)       21 2023-07-21 14:58:39.000000 thin_osm_api_wrapper-0.0.2/thin_osm_api_wrapper.egg-info/top_level.txt
+drwxrwxr-x   0 mateusz   (1000) mateusz   (1001)        0 2023-07-21 15:08:12.697694 thin_osm_api_wrapper-0.0.3/
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1001)     2290 2023-07-21 15:08:12.697694 thin_osm_api_wrapper-0.0.3/PKG-INFO
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1001)     1383 2023-03-06 02:35:50.000000 thin_osm_api_wrapper-0.0.3/README.md
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1001)       38 2023-07-21 15:08:12.697694 thin_osm_api_wrapper-0.0.3/setup.cfg
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1001)      740 2023-07-21 15:08:03.000000 thin_osm_api_wrapper-0.0.3/setup.py
+drwxrwxr-x   0 mateusz   (1000) mateusz   (1001)        0 2023-07-21 15:08:12.696694 thin_osm_api_wrapper-0.0.3/thin_osm_api_wrapper/
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1001)       31 2022-12-24 14:34:38.000000 thin_osm_api_wrapper-0.0.3/thin_osm_api_wrapper/__init__.py
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1001)     4339 2023-07-21 15:07:23.000000 thin_osm_api_wrapper-0.0.3/thin_osm_api_wrapper/api.py
+drwxrwxr-x   0 mateusz   (1000) mateusz   (1001)        0 2023-07-21 15:08:12.697694 thin_osm_api_wrapper-0.0.3/thin_osm_api_wrapper.egg-info/
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1001)     2290 2023-07-21 15:08:12.000000 thin_osm_api_wrapper-0.0.3/thin_osm_api_wrapper.egg-info/PKG-INFO
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1001)      255 2023-07-21 15:08:12.000000 thin_osm_api_wrapper-0.0.3/thin_osm_api_wrapper.egg-info/SOURCES.txt
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1001)        1 2023-07-21 15:08:12.000000 thin_osm_api_wrapper-0.0.3/thin_osm_api_wrapper.egg-info/dependency_links.txt
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1001)       21 2023-07-21 15:08:12.000000 thin_osm_api_wrapper-0.0.3/thin_osm_api_wrapper.egg-info/top_level.txt
```

### Comparing `thin_osm_api_wrapper-0.0.2/PKG-INFO` & `thin_osm_api_wrapper-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thin_osm_api_wrapper
-Version: 0.0.2
+Version: 0.0.3
 Summary: thin wrapper of https://wiki.openstreetmap.org/wiki/API
 Home-page: https://github.com/matkoniecz/thin_osm_api_python_wrapper
 Author: Mateusz Konieczny
 License: UNKNOWN
 Description: # Replaced
         See [osm_easy_api](https://github.com/docentYT/osm_easy_api)
```

### Comparing `thin_osm_api_wrapper-0.0.2/README.md` & `thin_osm_api_wrapper-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `thin_osm_api_wrapper-0.0.2/setup.py` & `thin_osm_api_wrapper-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="thin_osm_api_wrapper",
-    version="0.0.2",
+    version="0.0.3",
     author="Mateusz Konieczny",
     description="thin wrapper of https://wiki.openstreetmap.org/wiki/API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/matkoniecz/thin_osm_api_python_wrapper",
     packages=setuptools.find_packages(),
     classifiers=[
```

### Comparing `thin_osm_api_wrapper-0.0.2/thin_osm_api_wrapper/api.py` & `thin_osm_api_wrapper-0.0.3/thin_osm_api_wrapper/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,8 +103,9 @@
         # not sure is it happening on poor connection or explicit request by server
         # to slow down, in either case waiting a bit is a good idea
         except urllib3.exceptions.ProtocolError as e:
             print(e)
             sleep_before_retry("urllib3.exceptions.ProtocolError", url, params, json_data)
             continue
 
-element_list_touched_by_changeset('133124436')
+if __name__ == "__main__":
+    element_list_touched_by_changeset('133124436')
```

### Comparing `thin_osm_api_wrapper-0.0.2/thin_osm_api_wrapper.egg-info/PKG-INFO` & `thin_osm_api_wrapper-0.0.3/thin_osm_api_wrapper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thin-osm-api-wrapper
-Version: 0.0.2
+Version: 0.0.3
 Summary: thin wrapper of https://wiki.openstreetmap.org/wiki/API
 Home-page: https://github.com/matkoniecz/thin_osm_api_python_wrapper
 Author: Mateusz Konieczny
 License: UNKNOWN
 Description: # Replaced
         See [osm_easy_api](https://github.com/docentYT/osm_easy_api)
```

