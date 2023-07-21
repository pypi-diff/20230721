# Comparing `tmp/TDS2STAC-2.0.7.tar.gz` & `tmp/TDS2STAC-2.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TDS2STAC-2.0.7.tar", last modified: Thu Jul 20 18:35:59 2023, max compression
+gzip compressed data, was "TDS2STAC-2.0.8.tar", last modified: Fri Jul 21 17:38:45 2023, max compression
```

## Comparing `TDS2STAC-2.0.7.tar` & `TDS2STAC-2.0.8.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 hadizadeh-m (15144)      901        0 2023-07-20 18:35:59.647021 TDS2STAC-2.0.7/
--rw-r--r--   0 hadizadeh-m (15144)      901      168 2023-07-20 18:30:31.000000 TDS2STAC-2.0.7/AUTHORS.rst
--rw-r--r--   0 hadizadeh-m (15144)      901     3603 2023-07-20 18:30:31.000000 TDS2STAC-2.0.7/CONTRIBUTING.rst
--rw-r--r--   0 hadizadeh-m (15144)      901    13807 2023-07-20 18:30:31.000000 TDS2STAC-2.0.7/LICENSE
--rw-r--r--   0 hadizadeh-m (15144)      901      389 2023-07-20 18:30:31.000000 TDS2STAC-2.0.7/MANIFEST.in
--rw-r--r--   0 hadizadeh-m (15144)      901    10810 2023-07-20 18:35:59.647111 TDS2STAC-2.0.7/PKG-INFO
--rw-r--r--   0 hadizadeh-m (15144)      901     9403 2023-07-20 18:30:31.000000 TDS2STAC-2.0.7/README.rst
-drwxr-xr-x   0 hadizadeh-m (15144)      901        0 2023-07-20 18:35:59.644647 TDS2STAC-2.0.7/TDS2STAC.egg-info/
--rw-r--r--   0 hadizadeh-m (15144)      901    10810 2023-07-20 18:35:59.000000 TDS2STAC-2.0.7/TDS2STAC.egg-info/PKG-INFO
--rw-r--r--   0 hadizadeh-m (15144)      901      624 2023-07-20 18:35:59.000000 TDS2STAC-2.0.7/TDS2STAC.egg-info/SOURCES.txt
--rw-r--r--   0 hadizadeh-m (15144)      901        1 2023-07-20 18:35:59.000000 TDS2STAC-2.0.7/TDS2STAC.egg-info/dependency_links.txt
--rw-r--r--   0 hadizadeh-m (15144)      901      553 2023-07-20 18:35:59.000000 TDS2STAC-2.0.7/TDS2STAC.egg-info/requires.txt
--rw-r--r--   0 hadizadeh-m (15144)      901        9 2023-07-20 18:35:59.000000 TDS2STAC-2.0.7/TDS2STAC.egg-info/top_level.txt
-drwxr-xr-x   0 hadizadeh-m (15144)      901        0 2023-07-20 18:35:59.645741 TDS2STAC-2.0.7/docs/
--rw-r--r--   0 hadizadeh-m (15144)      901      609 2023-07-20 18:30:31.000000 TDS2STAC-2.0.7/docs/Makefile
--rw-r--r--   0 hadizadeh-m (15144)      901       28 2023-07-20 18:30:31.000000 TDS2STAC-2.0.7/docs/authors.rst
--rwxr-xr-x   0 hadizadeh-m (15144)      901     4870 2023-07-20 18:30:31.000000 TDS2STAC-2.0.7/docs/conf.py
--rw-r--r--   0 hadizadeh-m (15144)      901       33 2023-07-20 18:30:31.000000 TDS2STAC-2.0.7/docs/contributing.rst
--rw-r--r--   0 hadizadeh-m (15144)      901       28 2023-07-20 18:30:31.000000 TDS2STAC-2.0.7/docs/history.rst
--rw-r--r--   0 hadizadeh-m (15144)      901      296 2023-07-20 18:30:31.000000 TDS2STAC-2.0.7/docs/index.rst
--rw-r--r--   0 hadizadeh-m (15144)      901     1174 2023-07-20 18:30:31.000000 TDS2STAC-2.0.7/docs/installation.rst
--rw-r--r--   0 hadizadeh-m (15144)      901      806 2023-07-20 18:30:31.000000 TDS2STAC-2.0.7/docs/make.bat
--rw-r--r--   0 hadizadeh-m (15144)      901       27 2023-07-20 18:30:31.000000 TDS2STAC-2.0.7/docs/readme.rst
--rw-r--r--   0 hadizadeh-m (15144)      901       71 2023-07-20 18:30:31.000000 TDS2STAC-2.0.7/docs/usage.rst
--rw-r--r--   0 hadizadeh-m (15144)      901      181 2023-07-20 18:30:31.000000 TDS2STAC-2.0.7/pyproject.toml
--rw-r--r--   0 hadizadeh-m (15144)      901      227 2023-07-20 18:30:31.000000 TDS2STAC-2.0.7/requirements_dev.txt
--rw-r--r--   0 hadizadeh-m (15144)      901     1903 2023-07-20 18:35:59.647588 TDS2STAC-2.0.7/setup.cfg
--rw-r--r--   0 hadizadeh-m (15144)      901      427 2023-07-20 18:30:31.000000 TDS2STAC-2.0.7/setup.py
-drwxr-xr-x   0 hadizadeh-m (15144)      901        0 2023-07-20 18:35:59.647726 TDS2STAC-2.0.7/tds2stac/
--rw-r--r--   0 hadizadeh-m (15144)      901       99 2023-07-20 18:30:31.000000 TDS2STAC-2.0.7/tds2stac/__init__.py
--rw-r--r--   0 hadizadeh-m (15144)      901      497 2023-07-20 18:35:59.647755 TDS2STAC-2.0.7/tds2stac/_version.py
--rw-r--r--   0 hadizadeh-m (15144)      901    58825 2023-07-20 18:34:06.000000 TDS2STAC-2.0.7/tds2stac/app.py
--rw-r--r--   0 hadizadeh-m (15144)      901     2579 2023-07-20 18:30:31.000000 TDS2STAC-2.0.7/tds2stac/cli.py
--rw-r--r--   0 hadizadeh-m (15144)      901     3286 2023-07-20 18:30:31.000000 TDS2STAC-2.0.7/tds2stac/constants.py
--rw-r--r--   0 hadizadeh-m (15144)      901     7868 2023-07-20 18:30:31.000000 TDS2STAC-2.0.7/tds2stac/core.py
--rw-r--r--   0 hadizadeh-m (15144)      901     3696 2023-07-20 18:30:31.000000 TDS2STAC-2.0.7/tds2stac/utils.py
-drwxr-xr-x   0 hadizadeh-m (15144)      901        0 2023-07-20 18:35:59.646929 TDS2STAC-2.0.7/tests/
--rw-r--r--   0 hadizadeh-m (15144)      901       38 2023-07-20 18:30:31.000000 TDS2STAC-2.0.7/tests/__init__.py
--rw-r--r--   0 hadizadeh-m (15144)      901     1828 2023-07-20 18:30:31.000000 TDS2STAC-2.0.7/tests/test_tds2stac.py
--rw-r--r--   0 hadizadeh-m (15144)      901    84134 2023-07-20 18:30:31.000000 TDS2STAC-2.0.7/versioneer.py
+drwxr-xr-x   0 hadizadeh-m (15144)      901        0 2023-07-21 17:38:45.948110 TDS2STAC-2.0.8/
+-rw-r--r--   0 hadizadeh-m (15144)      901      168 2023-07-21 09:18:37.000000 TDS2STAC-2.0.8/AUTHORS.rst
+-rw-r--r--   0 hadizadeh-m (15144)      901     3603 2023-07-21 09:18:37.000000 TDS2STAC-2.0.8/CONTRIBUTING.rst
+-rw-r--r--   0 hadizadeh-m (15144)      901    13807 2023-07-21 09:18:37.000000 TDS2STAC-2.0.8/LICENSE
+-rw-r--r--   0 hadizadeh-m (15144)      901      389 2023-07-21 09:18:37.000000 TDS2STAC-2.0.8/MANIFEST.in
+-rw-r--r--   0 hadizadeh-m (15144)      901    10810 2023-07-21 17:38:45.948222 TDS2STAC-2.0.8/PKG-INFO
+-rw-r--r--   0 hadizadeh-m (15144)      901     9403 2023-07-21 09:18:37.000000 TDS2STAC-2.0.8/README.rst
+drwxr-xr-x   0 hadizadeh-m (15144)      901        0 2023-07-21 17:38:45.944575 TDS2STAC-2.0.8/TDS2STAC.egg-info/
+-rw-r--r--   0 hadizadeh-m (15144)      901    10810 2023-07-21 17:38:45.000000 TDS2STAC-2.0.8/TDS2STAC.egg-info/PKG-INFO
+-rw-r--r--   0 hadizadeh-m (15144)      901      624 2023-07-21 17:38:45.000000 TDS2STAC-2.0.8/TDS2STAC.egg-info/SOURCES.txt
+-rw-r--r--   0 hadizadeh-m (15144)      901        1 2023-07-21 17:38:45.000000 TDS2STAC-2.0.8/TDS2STAC.egg-info/dependency_links.txt
+-rw-r--r--   0 hadizadeh-m (15144)      901      553 2023-07-21 17:38:45.000000 TDS2STAC-2.0.8/TDS2STAC.egg-info/requires.txt
+-rw-r--r--   0 hadizadeh-m (15144)      901        9 2023-07-21 17:38:45.000000 TDS2STAC-2.0.8/TDS2STAC.egg-info/top_level.txt
+drwxr-xr-x   0 hadizadeh-m (15144)      901        0 2023-07-21 17:38:45.946355 TDS2STAC-2.0.8/docs/
+-rw-r--r--   0 hadizadeh-m (15144)      901      609 2023-07-21 09:18:37.000000 TDS2STAC-2.0.8/docs/Makefile
+-rw-r--r--   0 hadizadeh-m (15144)      901       28 2023-07-21 09:18:37.000000 TDS2STAC-2.0.8/docs/authors.rst
+-rwxr-xr-x   0 hadizadeh-m (15144)      901     4870 2023-07-21 09:18:37.000000 TDS2STAC-2.0.8/docs/conf.py
+-rw-r--r--   0 hadizadeh-m (15144)      901       33 2023-07-21 09:18:37.000000 TDS2STAC-2.0.8/docs/contributing.rst
+-rw-r--r--   0 hadizadeh-m (15144)      901       28 2023-07-21 09:18:37.000000 TDS2STAC-2.0.8/docs/history.rst
+-rw-r--r--   0 hadizadeh-m (15144)      901      296 2023-07-21 09:18:37.000000 TDS2STAC-2.0.8/docs/index.rst
+-rw-r--r--   0 hadizadeh-m (15144)      901     1174 2023-07-21 09:18:37.000000 TDS2STAC-2.0.8/docs/installation.rst
+-rw-r--r--   0 hadizadeh-m (15144)      901      806 2023-07-21 09:18:37.000000 TDS2STAC-2.0.8/docs/make.bat
+-rw-r--r--   0 hadizadeh-m (15144)      901       27 2023-07-21 09:18:37.000000 TDS2STAC-2.0.8/docs/readme.rst
+-rw-r--r--   0 hadizadeh-m (15144)      901       71 2023-07-21 09:18:37.000000 TDS2STAC-2.0.8/docs/usage.rst
+-rw-r--r--   0 hadizadeh-m (15144)      901      181 2023-07-21 09:18:37.000000 TDS2STAC-2.0.8/pyproject.toml
+-rw-r--r--   0 hadizadeh-m (15144)      901      227 2023-07-21 11:23:02.000000 TDS2STAC-2.0.8/requirements_dev.txt
+-rw-r--r--   0 hadizadeh-m (15144)      901     1903 2023-07-21 17:38:45.948737 TDS2STAC-2.0.8/setup.cfg
+-rw-r--r--   0 hadizadeh-m (15144)      901      427 2023-07-21 09:18:37.000000 TDS2STAC-2.0.8/setup.py
+drwxr-xr-x   0 hadizadeh-m (15144)      901        0 2023-07-21 17:38:45.948998 TDS2STAC-2.0.8/tds2stac/
+-rw-r--r--   0 hadizadeh-m (15144)      901       99 2023-07-21 09:18:37.000000 TDS2STAC-2.0.8/tds2stac/__init__.py
+-rw-r--r--   0 hadizadeh-m (15144)      901      497 2023-07-21 17:38:45.949040 TDS2STAC-2.0.8/tds2stac/_version.py
+-rw-r--r--   0 hadizadeh-m (15144)      901    59101 2023-07-21 17:37:19.000000 TDS2STAC-2.0.8/tds2stac/app.py
+-rw-r--r--   0 hadizadeh-m (15144)      901     2579 2023-07-21 09:18:37.000000 TDS2STAC-2.0.8/tds2stac/cli.py
+-rw-r--r--   0 hadizadeh-m (15144)      901     3286 2023-07-21 09:18:37.000000 TDS2STAC-2.0.8/tds2stac/constants.py
+-rw-r--r--   0 hadizadeh-m (15144)      901     7868 2023-07-21 09:18:37.000000 TDS2STAC-2.0.8/tds2stac/core.py
+-rw-r--r--   0 hadizadeh-m (15144)      901     3696 2023-07-21 09:18:37.000000 TDS2STAC-2.0.8/tds2stac/utils.py
+drwxr-xr-x   0 hadizadeh-m (15144)      901        0 2023-07-21 17:38:45.947960 TDS2STAC-2.0.8/tests/
+-rw-r--r--   0 hadizadeh-m (15144)      901       38 2023-07-21 09:18:37.000000 TDS2STAC-2.0.8/tests/__init__.py
+-rw-r--r--   0 hadizadeh-m (15144)      901     1828 2023-07-21 09:18:37.000000 TDS2STAC-2.0.8/tests/test_tds2stac.py
+-rw-r--r--   0 hadizadeh-m (15144)      901    84134 2023-07-21 09:18:37.000000 TDS2STAC-2.0.8/versioneer.py
```

### Comparing `TDS2STAC-2.0.7/CONTRIBUTING.rst` & `TDS2STAC-2.0.8/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `TDS2STAC-2.0.7/LICENSE` & `TDS2STAC-2.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `TDS2STAC-2.0.7/PKG-INFO` & `TDS2STAC-2.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TDS2STAC
-Version: 2.0.7
+Version: 2.0.8
 Summary: A STAC catalog creator from Thredds data server
 Home-page: https://codebase.helmholtz.cloud/CAT4KIT/tds2stac
 Author: Mostafa Hadizadeh
 Author-email: mostafa.hadizadeh@kit.edu
 License: EUPL-1.2
 Project-URL: Documentation, https://tds2stac.readthedocs.io/
 Project-URL: Source, https://codebase.helmholtz.cloud/CAT4KIT/tds2stac
```

### Comparing `TDS2STAC-2.0.7/README.rst` & `TDS2STAC-2.0.8/README.rst`

 * *Files identical despite different names*

### Comparing `TDS2STAC-2.0.7/TDS2STAC.egg-info/PKG-INFO` & `TDS2STAC-2.0.8/TDS2STAC.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TDS2STAC
-Version: 2.0.7
+Version: 2.0.8
 Summary: A STAC catalog creator from Thredds data server
 Home-page: https://codebase.helmholtz.cloud/CAT4KIT/tds2stac
 Author: Mostafa Hadizadeh
 Author-email: mostafa.hadizadeh@kit.edu
 License: EUPL-1.2
 Project-URL: Documentation, https://tds2stac.readthedocs.io/
 Project-URL: Source, https://codebase.helmholtz.cloud/CAT4KIT/tds2stac
```

### Comparing `TDS2STAC-2.0.7/TDS2STAC.egg-info/SOURCES.txt` & `TDS2STAC-2.0.8/TDS2STAC.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `TDS2STAC-2.0.7/TDS2STAC.egg-info/requires.txt` & `TDS2STAC-2.0.8/TDS2STAC.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `TDS2STAC-2.0.7/docs/Makefile` & `TDS2STAC-2.0.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `TDS2STAC-2.0.7/docs/conf.py` & `TDS2STAC-2.0.8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `TDS2STAC-2.0.7/docs/installation.rst` & `TDS2STAC-2.0.8/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `TDS2STAC-2.0.7/docs/make.bat` & `TDS2STAC-2.0.8/docs/make.bat`

 * *Files identical despite different names*

### Comparing `TDS2STAC-2.0.7/setup.cfg` & `TDS2STAC-2.0.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `TDS2STAC-2.0.7/tds2stac/app.py` & `TDS2STAC-2.0.8/tds2stac/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,15 +72,15 @@
         self.logger_id = logger_id
         self.logger_handler_host = logger_handler_host
 
         # using 'xml_processing' we get the catalog URL with
         # XML extension and catalog id and XML content of catalog.
 
         self.logger = logging.getLogger(
-            str(self.logger_name) + str(self.logger_id)
+            str(self.logger_name) + "_" + str(self.logger_id)
         )
         self.logger.setLevel(level=logging.DEBUG)
         # self.logger.setLevel(level=logging.WARNING)
 
         logHttpFormatter = logging.Formatter(
             fmt=f"%(levelname)-8s %(asctime)s \t %(filename)s @function %(funcName)s line %(lineno)s - %(message)s",
         )
@@ -166,14 +166,15 @@
                     ex_type, ex_value, ex_traceback = sys.exc_info()
                     # print("Exception type : %s " % ex_type.__name__)
                     # print("Exception message : %s" % ex_value)
                     # print(traceback.format_exc())
                     self.logger.error("%s : %s" % (ex_type.__name__, ex_value))
         if stac is not False:
             """In this part STAC catalogs will be created"""
+            self.logger.info("Harvesting datasets is started")
 
             # Main STAC catalog for linking other items and collections
             self.id_catalog = id_catalog
             self.xml_url_catalog = xml_url_catalog
             # Define an empty STAC catalog
             # Here we should extend the functionality of STAC catalog to fix issue #60
             self.catalog[id_catalog] = pystac.Catalog(
@@ -215,19 +216,21 @@
             else:
                 self.logger.warning(
                     "Webservices are not activated for this catalog"
                 )
                 # print(
                 #     "Warning: Webservices are not activated for this catalog"
                 # )
-
+            self.logger.info("Harvesting datasets is finished")
         if catalog_ingestion is not False:
+            self.logger.info("Ingesting catalogs is finished")
             """With enabling 'catalog_ingestion' STAC catalogs
             , collections and items ingest into the 'pgSTAC'"""
             ds2stac_ingester.Ingester(stac_dir, api_posting)
+            self.logger.info("Ingesting catalogs is finished")
 
     def datasets_harvester(self, url, web_service, xml_content):
         """This is the main function to create the STAC catalog, collections,
         and items and also is for linking them to each other"""
 
         footprint_temp = None  # Define initial bounding box
         footprint_temp_point = (
@@ -1110,15 +1113,15 @@
                                 temporal=temporal_extent,
                             )
                             self.catalog[collection_item_id].add_item(item)
                 except Exception as e:
                     ex_type, ex_value, ex_traceback = sys.exc_info()
                     print("Exception type : %s " % ex_type.__name__)
                     print("Exception message : %s" % ex_value)
-                    self.logger.critical(traceback.format_exc())
+                    self.logger.critical("%s : %s" % (ex_type.__name__, ex_value))
 
                     continue
 
             yield str(url) + "?dataset=" + str(elem.get("ID"))
         # When a collection doesn't have Spatial or Temporal extent
         if (
             type(self.catalog[catalog_colleciton_id])
```

### Comparing `TDS2STAC-2.0.7/tds2stac/cli.py` & `TDS2STAC-2.0.8/tds2stac/cli.py`

 * *Files identical despite different names*

### Comparing `TDS2STAC-2.0.7/tds2stac/constants.py` & `TDS2STAC-2.0.8/tds2stac/constants.py`

 * *Files identical despite different names*

### Comparing `TDS2STAC-2.0.7/tds2stac/core.py` & `TDS2STAC-2.0.8/tds2stac/core.py`

 * *Files identical despite different names*

### Comparing `TDS2STAC-2.0.7/tds2stac/utils.py` & `TDS2STAC-2.0.8/tds2stac/utils.py`

 * *Files identical despite different names*

### Comparing `TDS2STAC-2.0.7/tests/test_tds2stac.py` & `TDS2STAC-2.0.8/tests/test_tds2stac.py`

 * *Files identical despite different names*

### Comparing `TDS2STAC-2.0.7/versioneer.py` & `TDS2STAC-2.0.8/versioneer.py`

 * *Files identical despite different names*

