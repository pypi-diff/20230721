# Comparing `tmp/location-local-0.0.8.tar.gz` & `tmp/location-local-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "location-local-0.0.8.tar", last modified: Thu Jul 20 03:33:45 2023, max compression
+gzip compressed data, was "location-local-0.0.9.tar", last modified: Thu Jul 20 10:28:58 2023, max compression
```

## Comparing `location-local-0.0.8.tar` & `location-local-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 03:33:45.968276 location-local-0.0.8/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 03:33:45.964275 location-local-0.0.8/CirclesGetCountryName/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 03:33:32.000000 location-local-0.0.8/CirclesGetCountryName/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-07-20 03:33:32.000000 location-local-0.0.8/CirclesGetCountryName/opencage_get_country_name.py
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-20 03:33:45.964275 location-local-0.0.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 03:33:45.964275 location-local-0.0.8/location_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-20 03:33:45.000000 location-local-0.0.8/location_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-20 03:33:45.000000 location-local-0.0.8/location_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 03:33:45.000000 location-local-0.0.8/location_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-20 03:33:45.000000 location-local-0.0.8/location_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 03:33:45.968276 location-local-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-20 03:33:32.000000 location-local-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 03:33:45.964275 location-local-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-07-20 03:33:32.000000 location-local-0.0.8/tests/test_opnecage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:28:58.306768 location-local-0.0.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:28:58.302768 location-local-0.0.9/CirclesGetCountryName/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 10:28:42.000000 location-local-0.0.9/CirclesGetCountryName/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-07-20 10:28:42.000000 location-local-0.0.9/CirclesGetCountryName/opencage_get_country_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-20 10:28:58.306768 location-local-0.0.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:28:58.306768 location-local-0.0.9/location_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-20 10:28:58.000000 location-local-0.0.9/location_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-20 10:28:58.000000 location-local-0.0.9/location_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 10:28:58.000000 location-local-0.0.9/location_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-20 10:28:58.000000 location-local-0.0.9/location_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 10:28:58.306768 location-local-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-20 10:28:42.000000 location-local-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:28:58.306768 location-local-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-07-20 10:28:42.000000 location-local-0.0.9/tests/test_opnecage.py
```

### Comparing `location-local-0.0.8/CirclesGetCountryName/opencage_get_country_name.py` & `location-local-0.0.9/CirclesGetCountryName/opencage_get_country_name.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import os
 from opencage.geocoder import OpenCageGeocode
-from logger_local_python_package.localLogger import _local_logger as local_logger
+from logger_local_python_package.localLogger import logger_local
 from dotenv import load_dotenv
 load_dotenv()
 
 class Country:
     def __init__(self):
         pass
     
     @staticmethod
     def get_country_name(location):
         # Create a geocoder instance
         object1={
             'location':location
         }
-        local_logger.start(object=object1)
+        logger_local.start(object=object1)
         api_key = os.getenv("OPENCAGE_KEY")
 
         # Define the city or state
         geocoder = OpenCageGeocode(api_key)
 
         # Use geocoding to get the location details
         results = geocoder.geocode(location)
@@ -30,17 +30,17 @@
             # Extract the country from components
             country = components.get('country', '')
             if not country:
                 # If country is not found, check for country_code as an alternative
                 country = components.get('country_code', '')
         else:
             country = None
-            local_logger.error("country didnt found for %s."%location)
+            logger_local.error("country didnt found for %s."%location)
         object2={
                 'return':country
             }
-        local_logger.end(object=object2)
+        logger_local.end(object=object2)
         return country
 
 
 if __name__ == "__main__":
     pass
```

### Comparing `location-local-0.0.8/setup.py` & `location-local-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 # used by python -m build
 # python -m build needs pyproject.toml or setup.py
 setuptools.setup(
      # TODO: Please update the name
      name='location-local',
-     version='0.0.8', # https://pypi.org/project/location-local/
+     version='0.0.9', # https://pypi.org/project/location-local/
      author="Circles",
      author_email="info@circles.life",
      description="Location Locatal PyPI Package",
      long_description="This is a package for sharing common OpenCage function used in different repositories",
      long_description_content_type="text/markdown",
      url="https://github.com/javatechy/dokr",
      packages=setuptools.find_packages(),
```

### Comparing `location-local-0.0.8/tests/test_opnecage.py` & `location-local-0.0.9/tests/test_opnecage.py`

 * *Files identical despite different names*

