# Comparing `tmp/bcdata-0.8.0a3.tar.gz` & `tmp/bcdata-0.8.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bcdata-0.8.0a3.tar", last modified: Thu Jul  6 00:10:05 2023, max compression
+gzip compressed data, was "bcdata-0.8.0b1.tar", last modified: Fri Jul 14 01:33:00 2023, max compression
```

## Comparing `bcdata-0.8.0a3.tar` & `bcdata-0.8.0b1.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 snorris    (501) staff       (20)        0 2023-07-06 00:10:05.782237 bcdata-0.8.0a3/
--rw-r--r--   0 snorris    (501) staff       (20)     7455 2023-07-06 00:08:01.000000 bcdata-0.8.0a3/CHANGES.txt
--rw-r--r--   0 snorris    (501) staff       (20)     1080 2018-01-17 01:59:21.000000 bcdata-0.8.0a3/LICENSE.txt
--rw-r--r--   0 snorris    (501) staff       (20)    16479 2023-07-06 00:10:05.782093 bcdata-0.8.0a3/PKG-INFO
--rw-r--r--   0 snorris    (501) staff       (20)    15657 2023-06-29 21:33:29.000000 bcdata-0.8.0a3/README.md
-drwxr-xr-x   0 snorris    (501) staff       (20)        0 2023-07-06 00:10:05.780479 bcdata-0.8.0a3/bcdata/
--rw-r--r--   0 snorris    (501) staff       (20)      351 2023-07-06 00:07:45.000000 bcdata-0.8.0a3/bcdata/__init__.py
--rw-r--r--   0 snorris    (501) staff       (20)     6513 2023-07-06 00:04:54.000000 bcdata-0.8.0a3/bcdata/bc2pg.py
--rw-r--r--   0 snorris    (501) staff       (20)     4483 2023-07-06 00:04:54.000000 bcdata-0.8.0a3/bcdata/bcdc.py
--rw-r--r--   0 snorris    (501) staff       (20)    10042 2023-07-06 00:04:54.000000 bcdata-0.8.0a3/bcdata/cli.py
--rw-r--r--   0 snorris    (501) staff       (20)     6342 2023-07-06 00:04:54.000000 bcdata-0.8.0a3/bcdata/database.py
--rw-r--r--   0 snorris    (501) staff       (20)     3654 2023-07-04 20:29:20.000000 bcdata-0.8.0a3/bcdata/wcs.py
--rw-r--r--   0 snorris    (501) staff       (20)    12144 2023-07-06 00:04:54.000000 bcdata-0.8.0a3/bcdata/wfs.py
-drwxr-xr-x   0 snorris    (501) staff       (20)        0 2023-07-06 00:10:05.781461 bcdata-0.8.0a3/bcdata.egg-info/
--rw-r--r--   0 snorris    (501) staff       (20)    16479 2023-07-06 00:10:05.000000 bcdata-0.8.0a3/bcdata.egg-info/PKG-INFO
--rw-r--r--   0 snorris    (501) staff       (20)      474 2023-07-06 00:10:05.000000 bcdata-0.8.0a3/bcdata.egg-info/SOURCES.txt
--rw-r--r--   0 snorris    (501) staff       (20)        1 2023-07-06 00:10:05.000000 bcdata-0.8.0a3/bcdata.egg-info/dependency_links.txt
--rw-r--r--   0 snorris    (501) staff       (20)       42 2023-07-06 00:10:05.000000 bcdata-0.8.0a3/bcdata.egg-info/entry_points.txt
--rw-r--r--   0 snorris    (501) staff       (20)        1 2019-11-08 06:25:25.000000 bcdata-0.8.0a3/bcdata.egg-info/not-zip-safe
--rw-r--r--   0 snorris    (501) staff       (20)      134 2023-07-06 00:10:05.000000 bcdata-0.8.0a3/bcdata.egg-info/requires.txt
--rw-r--r--   0 snorris    (501) staff       (20)        7 2023-07-06 00:10:05.000000 bcdata-0.8.0a3/bcdata.egg-info/top_level.txt
--rw-r--r--   0 snorris    (501) staff       (20)      173 2022-07-16 00:28:03.000000 bcdata-0.8.0a3/pyproject.toml
--rw-r--r--   0 snorris    (501) staff       (20)      115 2023-06-29 21:33:29.000000 bcdata-0.8.0a3/requirements.txt
--rw-r--r--   0 snorris    (501) staff       (20)       38 2023-07-06 00:10:05.782273 bcdata-0.8.0a3/setup.cfg
--rw-r--r--   0 snorris    (501) staff       (20)     1732 2022-07-20 16:54:44.000000 bcdata-0.8.0a3/setup.py
-drwxr-xr-x   0 snorris    (501) staff       (20)        0 2023-07-06 00:10:05.781938 bcdata-0.8.0a3/tests/
--rw-r--r--   0 snorris    (501) staff       (20)     5273 2023-07-06 00:04:54.000000 bcdata-0.8.0a3/tests/test_bc2pg.py
--rw-r--r--   0 snorris    (501) staff       (20)     6088 2023-06-29 21:33:29.000000 bcdata-0.8.0a3/tests/test_bcdata.py
--rw-r--r--   0 snorris    (501) staff       (20)    11744 2023-07-03 22:28:46.000000 bcdata-0.8.0a3/tests/test_bcdc.py
--rw-r--r--   0 snorris    (501) staff       (20)     2393 2022-07-20 16:54:44.000000 bcdata-0.8.0a3/tests/test_cli.py
+drwxr-xr-x   0 snorris    (501) staff       (20)        0 2023-07-14 01:33:00.920476 bcdata-0.8.0b1/
+-rw-r--r--   0 snorris    (501) staff       (20)     7744 2023-07-14 01:30:32.000000 bcdata-0.8.0b1/CHANGES.txt
+-rw-r--r--   0 snorris    (501) staff       (20)     1080 2018-01-17 01:59:21.000000 bcdata-0.8.0b1/LICENSE.txt
+-rw-r--r--   0 snorris    (501) staff       (20)    16856 2023-07-14 01:33:00.920328 bcdata-0.8.0b1/PKG-INFO
+-rw-r--r--   0 snorris    (501) staff       (20)    16034 2023-07-14 01:26:44.000000 bcdata-0.8.0b1/README.md
+drwxr-xr-x   0 snorris    (501) staff       (20)        0 2023-07-14 01:33:00.918708 bcdata-0.8.0b1/bcdata/
+-rw-r--r--   0 snorris    (501) staff       (20)      359 2023-07-14 01:27:42.000000 bcdata-0.8.0b1/bcdata/__init__.py
+-rw-r--r--   0 snorris    (501) staff       (20)     6521 2023-07-14 01:24:32.000000 bcdata-0.8.0b1/bcdata/bc2pg.py
+-rw-r--r--   0 snorris    (501) staff       (20)     4943 2023-07-14 01:24:32.000000 bcdata-0.8.0b1/bcdata/bcdc.py
+-rw-r--r--   0 snorris    (501) staff       (20)    10124 2023-07-14 01:24:32.000000 bcdata-0.8.0b1/bcdata/cli.py
+-rw-r--r--   0 snorris    (501) staff       (20)     6342 2023-07-06 00:04:54.000000 bcdata-0.8.0b1/bcdata/database.py
+-rw-r--r--   0 snorris    (501) staff       (20)     3654 2023-07-04 20:29:20.000000 bcdata-0.8.0b1/bcdata/wcs.py
+-rw-r--r--   0 snorris    (501) staff       (20)    17903 2023-07-14 01:24:32.000000 bcdata-0.8.0b1/bcdata/wfs.py
+drwxr-xr-x   0 snorris    (501) staff       (20)        0 2023-07-14 01:33:00.919632 bcdata-0.8.0b1/bcdata.egg-info/
+-rw-r--r--   0 snorris    (501) staff       (20)    16856 2023-07-14 01:33:00.000000 bcdata-0.8.0b1/bcdata.egg-info/PKG-INFO
+-rw-r--r--   0 snorris    (501) staff       (20)      489 2023-07-14 01:33:00.000000 bcdata-0.8.0b1/bcdata.egg-info/SOURCES.txt
+-rw-r--r--   0 snorris    (501) staff       (20)        1 2023-07-14 01:33:00.000000 bcdata-0.8.0b1/bcdata.egg-info/dependency_links.txt
+-rw-r--r--   0 snorris    (501) staff       (20)       42 2023-07-14 01:33:00.000000 bcdata-0.8.0b1/bcdata.egg-info/entry_points.txt
+-rw-r--r--   0 snorris    (501) staff       (20)        1 2019-11-08 06:25:25.000000 bcdata-0.8.0b1/bcdata.egg-info/not-zip-safe
+-rw-r--r--   0 snorris    (501) staff       (20)      134 2023-07-14 01:33:00.000000 bcdata-0.8.0b1/bcdata.egg-info/requires.txt
+-rw-r--r--   0 snorris    (501) staff       (20)        7 2023-07-14 01:33:00.000000 bcdata-0.8.0b1/bcdata.egg-info/top_level.txt
+-rw-r--r--   0 snorris    (501) staff       (20)      173 2022-07-16 00:28:03.000000 bcdata-0.8.0b1/pyproject.toml
+-rw-r--r--   0 snorris    (501) staff       (20)      115 2023-06-29 21:33:29.000000 bcdata-0.8.0b1/requirements.txt
+-rw-r--r--   0 snorris    (501) staff       (20)       38 2023-07-14 01:33:00.920509 bcdata-0.8.0b1/setup.cfg
+-rw-r--r--   0 snorris    (501) staff       (20)     1732 2022-07-20 16:54:44.000000 bcdata-0.8.0b1/setup.py
+drwxr-xr-x   0 snorris    (501) staff       (20)        0 2023-07-14 01:33:00.920169 bcdata-0.8.0b1/tests/
+-rw-r--r--   0 snorris    (501) staff       (20)     5273 2023-07-06 00:04:54.000000 bcdata-0.8.0b1/tests/test_bc2pg.py
+-rw-r--r--   0 snorris    (501) staff       (20)    11744 2023-07-03 22:28:46.000000 bcdata-0.8.0b1/tests/test_bcdc.py
+-rw-r--r--   0 snorris    (501) staff       (20)     2393 2022-07-20 16:54:44.000000 bcdata-0.8.0b1/tests/test_cli.py
+-rw-r--r--   0 snorris    (501) staff       (20)     2205 2023-07-14 01:24:32.000000 bcdata-0.8.0b1/tests/test_wcs.py
+-rw-r--r--   0 snorris    (501) staff       (20)     3814 2023-07-14 01:24:32.000000 bcdata-0.8.0b1/tests/test_wfs.py
```

### Comparing `bcdata-0.8.0a3/CHANGES.txt` & `bcdata-0.8.0b1/CHANGES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 Changes
 =======
 
+0.8.0b1 (2023-07-13)
+------------------
+- wrap all requests to WFS/BCDC with @retry to better handle network/service errors
+- modify cache structure, bcdata now caches to folder ~/.bcdata/
+- cache layer schemas to reduce request load
+- refactor wfs module to better handle caching/retrys
+
 0.8.0a3 (2023-07-05)
 ------------------
 - improve retry logic on download error, further request minimization, fix bcdc regression from #135
 
 0.8.0a2 (2023-07-03)
 ------------------
 - handle tables with schema stored in bcdc resource with format='multiple' (#135)
```

### Comparing `bcdata-0.8.0a3/LICENSE.txt` & `bcdata-0.8.0b1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bcdata-0.8.0a3/PKG-INFO` & `bcdata-0.8.0b1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bcdata
-Version: 0.8.0a3
+Version: 0.8.0b1
 Summary: Python tools for quick access to DataBC geo-data available via WFS
 Home-page: https://github.com/smnorris/bcdata
 Author: Simon Norris
 Author-email: snorris@hillcrestgeo.ca
 License: Apache
 Keywords: gis geospatial data BC DataBC download "Britsh Columbia"
 Classifier: Development Status :: 3 - Alpha
@@ -54,21 +54,26 @@
 The default target database connection (used by `bc2pg`) can be set via the `DATABASE_URL` environment variable (the password parameter should not be required if using a [.pgpass file](https://www.postgresql.org/docs/current/libpq-pgpass.html))
 
 Linux/Mac: `export DATABASE_URL=postgresql://{username}:{password}@{hostname}:{port}/{database}`
 
 Windows:   `SET DATABASE_URL=postgresql://{username}:{password}@{hostname}:{port}/{database}`
 
 
-#### Layer list cache file
+#### Layer list / layer schema cache
 
-A list of DataBC layers is cached to file to speed request validation. The cache is automatically refreshed if it is more than a day old.
-The cache file location defaults to `~/.bcdata`, but can be configured by setting the a `$BCDATA_CACHE` environment variable.
+To reduce the volume of requests, information about data requested is cached locally:
+ - the WFS GetCapabilities response xml (listing all datasets available via the service) is cached as `capabilities.xml`
+ - schemas of individual layers that have previously been requested are cached with the cache file name matching the object/table name
+
+`capabilities.xml` is automatically refreshed if it is more than a day old. The layer definition files are refreshed if more than 30 days old. These cache files are stored by default in `~/.bcdata`. Modify this location by  setting the the `$BCDATA_CACHE` environment variable:
 
 `export BCDATA_CACHE=/path/to/bcdata_cache`
 
+Force a cache refresh by deleting the files in the cache or the entire cache folder.
+
 ## Usage
 
 Typical usage will involve a manual search of the [DataBC Catalogue](https://catalogue.data.gov.bc.ca/dataset?download_audience=Public) to find a layer of interest. Once a dataset of interest is found, note the key with which to retreive it. This can be either the `id`/`package name` (the last portion of the url) or the `Object Name` (Under `Object Description`).
 
 For example, for [BC Airports]( https://catalogue.data.gov.bc.ca/dataset/bc-airports), either of these keys will work:
 
 - id/package name: `bc-airports`
@@ -143,15 +148,15 @@
   --query TEXT            A valid CQL or ECQL query
   -c, --count INTEGER     Total number of features to load
   -p, --pagesize INTEGER  Maximum request size
   -k, --primary_key TEXT  Primary key of dataset
   -s, --sortby TEXT       Name of sort field
   -e, --schema_only       Create empty table from catalogue schema
   -a, --append            Append to existing table
-  -t, --no_timestamp      Do not add download timestamp to bcdata meta table
+  -t, --no_timestamp      Do not log download to bcdata.log
   -v, --verbose           Increase verbosity.
   -q, --quiet             Decrease verbosity.
   --help                  Show this message and exit.
 ```
 
 #### cat
 
@@ -267,21 +272,21 @@
 Options:
   -r, --refresh  Refresh the cached list
   --help         Show this message and exit.
 ```
 
 #### CLI notes
 
-Note that `bc2pg` creates `public.bcdata` as a meta table tracking the most recent download date for each layer downloaded.
-Disable with the switch `--no_timestamp` if you do not wish to create this table or do not have access to `public` schema.
+Note that `bc2pg` creates `bcdata.log` and logs the most recent download date for each table downloaded.
+Disable with the switch `--no_timestamp` if you do not wish to create this table.
 
-Example of a record in `public.bcdata`:
+Example of a record in `bcdata.log`:
 
 ```
-mydb=# select * from bcdata;
+mydb=# select * from bcdata.log;
                  table_name                  |        date_downloaded
 ---------------------------------------------+-------------------------------
  whse_imagery_and_base_maps.gsr_airports_svw | 2021-02-17 11:50:34.044481-08
 ```
 
 
 #### CLI examples
```

### Comparing `bcdata-0.8.0a3/README.md` & `bcdata-0.8.0b1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -32,21 +32,26 @@
 The default target database connection (used by `bc2pg`) can be set via the `DATABASE_URL` environment variable (the password parameter should not be required if using a [.pgpass file](https://www.postgresql.org/docs/current/libpq-pgpass.html))
 
 Linux/Mac: `export DATABASE_URL=postgresql://{username}:{password}@{hostname}:{port}/{database}`
 
 Windows:   `SET DATABASE_URL=postgresql://{username}:{password}@{hostname}:{port}/{database}`
 
 
-#### Layer list cache file
+#### Layer list / layer schema cache
 
-A list of DataBC layers is cached to file to speed request validation. The cache is automatically refreshed if it is more than a day old.
-The cache file location defaults to `~/.bcdata`, but can be configured by setting the a `$BCDATA_CACHE` environment variable.
+To reduce the volume of requests, information about data requested is cached locally:
+ - the WFS GetCapabilities response xml (listing all datasets available via the service) is cached as `capabilities.xml`
+ - schemas of individual layers that have previously been requested are cached with the cache file name matching the object/table name
+
+`capabilities.xml` is automatically refreshed if it is more than a day old. The layer definition files are refreshed if more than 30 days old. These cache files are stored by default in `~/.bcdata`. Modify this location by  setting the the `$BCDATA_CACHE` environment variable:
 
 `export BCDATA_CACHE=/path/to/bcdata_cache`
 
+Force a cache refresh by deleting the files in the cache or the entire cache folder.
+
 ## Usage
 
 Typical usage will involve a manual search of the [DataBC Catalogue](https://catalogue.data.gov.bc.ca/dataset?download_audience=Public) to find a layer of interest. Once a dataset of interest is found, note the key with which to retreive it. This can be either the `id`/`package name` (the last portion of the url) or the `Object Name` (Under `Object Description`).
 
 For example, for [BC Airports]( https://catalogue.data.gov.bc.ca/dataset/bc-airports), either of these keys will work:
 
 - id/package name: `bc-airports`
@@ -121,15 +126,15 @@
   --query TEXT            A valid CQL or ECQL query
   -c, --count INTEGER     Total number of features to load
   -p, --pagesize INTEGER  Maximum request size
   -k, --primary_key TEXT  Primary key of dataset
   -s, --sortby TEXT       Name of sort field
   -e, --schema_only       Create empty table from catalogue schema
   -a, --append            Append to existing table
-  -t, --no_timestamp      Do not add download timestamp to bcdata meta table
+  -t, --no_timestamp      Do not log download to bcdata.log
   -v, --verbose           Increase verbosity.
   -q, --quiet             Decrease verbosity.
   --help                  Show this message and exit.
 ```
 
 #### cat
 
@@ -245,21 +250,21 @@
 Options:
   -r, --refresh  Refresh the cached list
   --help         Show this message and exit.
 ```
 
 #### CLI notes
 
-Note that `bc2pg` creates `public.bcdata` as a meta table tracking the most recent download date for each layer downloaded.
-Disable with the switch `--no_timestamp` if you do not wish to create this table or do not have access to `public` schema.
+Note that `bc2pg` creates `bcdata.log` and logs the most recent download date for each table downloaded.
+Disable with the switch `--no_timestamp` if you do not wish to create this table.
 
-Example of a record in `public.bcdata`:
+Example of a record in `bcdata.log`:
 
 ```
-mydb=# select * from bcdata;
+mydb=# select * from bcdata.log;
                  table_name                  |        date_downloaded
 ---------------------------------------------+-------------------------------
  whse_imagery_and_base_maps.gsr_airports_svw | 2021-02-17 11:50:34.044481-08
 ```
 
 
 #### CLI examples
```

### Comparing `bcdata-0.8.0a3/bcdata/bc2pg.py` & `bcdata-0.8.0b1/bcdata/bc2pg.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,15 +90,15 @@
         if geometry_type:
             geometry_type = geometry_type.upper()
             if geometry_type not in SUPPORTED_TYPES:
                 raise ValueError("Geometry type {geometry_type} is not supported")
 
         # if geometry type is not provided, infer from first 10 records in dataset
         if not geometry_type:
-            geometry_type = bcdata.get_types(dataset, 10)[0]
+            geometry_type = bcdata.get_spatial_types(dataset, 10)[0]
 
         # build the table definition and create table
         table = db.define_table(
             schema_name,
             table_name,
             table_details,
             geometry_type,
```

### Comparing `bcdata-0.8.0a3/bcdata/bcdc.py` & `bcdata-0.8.0b1/bcdata/bcdc.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,35 @@
 import json
 import logging
 from urllib.parse import urlparse
 
+from tenacity import retry
+from tenacity.stop import stop_after_delay
+from tenacity.wait import wait_random_exponential
 import requests
 
 import bcdata
 
 
 log = logging.getLogger(__name__)
 
 BCDC_API_URL = "https://catalogue.data.gov.bc.ca/api/3/action/"
 
 
+@retry(stop=stop_after_delay(120), wait=wait_random_exponential(multiplier=1, max=60))
 def get_table_name(package):
     """Query DataBC API to find WFS table/layer name for given package"""
     package = package.lower()  # package names are lowercase
     params = {"id": package}
-    r = requests.get(BCDC_API_URL + "package_show", params=params)
-    if r.status_code != 200:
-        raise ValueError("{d} is not present in DataBC API list".format(d=package))
+    try:
+        r = requests.get(BCDC_API_URL + "package_show", params=params)
+        if r.status_code != 200:
+            raise ValueError("{d} is not present in DataBC API list".format(d=package))
+    except Exception:
+        log.error("BCDC API Error")
     result = r.json()["result"]
     # Because the object_name in the result json is not a 100% reliable key
     # for WFS requests, parse URL in WMS resource(s).
     # Also, some packages may have >1 WFS layer - if this is the case, bail
     # and provide user with a list of layers
     layer_urls = [r["url"] for r in result["resources"] if r["format"] == "wms"]
     layer_names = [urlparse(url).path.split("/")[3] for url in layer_urls]
@@ -31,31 +38,35 @@
             "Package {} includes more than one WFS resource, specify one of the following: \n{}".format(
                 package, "\n".join(layer_names)
             )
         )
     return layer_names[0]
 
 
+@retry(stop=stop_after_delay(120), wait=wait_random_exponential(multiplier=1, max=60))
 def get_table_definition(table_name):
     """
     Given a table/object name, search BCDC for the first package/resource with a
     matching "object_name", returns tuple (table comments, table schema)
     """
     # only allow searching for tables present in WFS list
     table_name = table_name.upper()
     if table_name not in bcdata.list_tables():
         raise ValueError(
             f"Only tables available via WFS are supported, {table_name} not found"
         )
     # search the api for the provided table
-    r = requests.get(BCDC_API_URL + "package_search", params={"q": table_name})
-    # catch general api errors
-    status_code = r.status_code
-    if status_code != 200:
-        raise ValueError(f"Error searching BC Data Catalogue API: {status_code}")
+    try:
+        r = requests.get(BCDC_API_URL + "package_search", params={"q": table_name})
+        # catch general api errors
+        status_code = r.status_code
+        if status_code != 200:
+            raise ValueError(f"Error searching BC Data Catalogue API: {status_code}")
+    except Exception:
+        log.error("BCDC API Error")
     # if there are no matching results, let the user know
     if r.json()["result"]["count"] == 0:
         log.warning(
             f"BC Data Catalouge API search provides no results for: {table_name}"
         )
         return []
     else:
```

### Comparing `bcdata-0.8.0a3/bcdata/cli.py` & `bcdata-0.8.0b1/bcdata/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -289,14 +289,21 @@
         pagesize=pagesize,
         lowercase=lowercase,
     ):
         click.echo(json.dumps(feat, **dump_kwds))
 
 
 @cli.command()
+@verbose_opt
+@quiet_opt
+def clear_cache(verbose, quiet):
+    bcdata.clear_cache()
+
+
+@cli.command()
 @click.argument("dataset", type=click.STRING, shell_complete=complete_dataset_names)
 @click.option(
     "--db_url",
     "-db",
     help="Target database url, defaults to $DATABASE_URL environment variable if set",
     default=os.environ.get("DATABASE_URL"),
 )
@@ -329,15 +336,15 @@
     is_flag=True,
     help="Append to existing table",
 )
 @click.option(
     "--no_timestamp",
     "-t",
     is_flag=True,
-    help="Do not add download timestamp to bcdata meta table",
+    help="Do not log download to bcdata.log",
 )
 @verbose_opt
 @quiet_opt
 def bc2pg(
     dataset,
     db_url,
     table,
```

### Comparing `bcdata-0.8.0a3/bcdata/database.py` & `bcdata-0.8.0b1/bcdata/database.py`

 * *Files identical despite different names*

### Comparing `bcdata-0.8.0a3/bcdata/wcs.py` & `bcdata-0.8.0b1/bcdata/wcs.py`

 * *Files identical despite different names*

### Comparing `bcdata-0.8.0a3/bcdata/wfs.py` & `bcdata-0.8.0b1/bcdata/wfs.py`

 * *Files 22% similar despite different names*

```diff
@@ -23,350 +23,501 @@
 
 if not sys.warnoptions:
     warnings.simplefilter("ignore")
 
 log = logging.getLogger(__name__)
 
 
-WFS_URL = "https://openmaps.gov.bc.ca/geo/pub/wfs"
-OWS_URL = "http://openmaps.gov.bc.ca/geo/ows"
+class BCWFS(object):
+    """Wrapper around owslib WebFeatureService to manage cached resources"""
 
-
-def check_cache(path):
-    """Return true if the getcapabilities cache does not exist or is more than a day old"""
-    if not os.path.exists(path):
-        return True
-    else:
-        # check the age
-        mod_date = datetime.fromtimestamp(os.path.getmtime(path))
-        if mod_date < (datetime.now() - timedelta(days=1)):
+    def __init__(self, cache_path=None, refresh=False):
+        self.wfs_url = "https://openmaps.gov.bc.ca/geo/pub/wfs"
+        self.ows_url = "http://openmaps.gov.bc.ca/geo/ows"
+
+        # point to cache path
+        if cache_path:
+            self.cache_path = cache_path
+        else:
+            if "BCDATA_CACHE" in os.environ:
+                self.cache_path = os.environ["BCDATA_CACHE"]
+            else:
+                self.cache_path = os.path.join(str(Path.home()), ".bcdata")
+        # if a file exists in the path provided AND the file name is .bcdata, delete it
+        p = Path(self.cache_path)
+        if p.is_file():
+            if self.cache_path[-7:] == ".bcdata":
+                p.unlink()
+            # if the file is named something else, prompt user to delete it
+            else:
+                raise RuntimeError(
+                    f"Cache file exists, delete before using bcdata: {self.cache_path}"
+                )
+        # create cache folder if it does not exist
+        p.mkdir(parents=True, exist_ok=True)
+        # load capabilities
+        self.capabilities = self.get_capabilities(refresh)
+
+    def check_cached_file(self, cache_file, days=1):
+        """Return true if the file is empty / does not exist / is more than n days old"""
+        cache_file = os.path.join(self.cache_path, cache_file)
+        if not os.path.exists(os.path.join(cache_file)):
             return True
         else:
-            return False
+            mod_date = datetime.fromtimestamp(os.path.getmtime(cache_file))
+            # if file older than specified days or empty, return true
+            if (
+                mod_date < (datetime.now() - timedelta(days=days))
+                or os.stat(cache_file).st_size == 0
+            ):
+                return True
+            else:
+                return False
 
+    @retry(
+        stop=stop_after_delay(120), wait=wait_random_exponential(multiplier=1, max=60)
+    )
+    def _request_capabilities(self):
+        try:
+            capabilities = ET.tostring(
+                WebFeatureService(self.ows_url, version="2.0.0")._capabilities,
+                encoding="unicode",
+            )
+        except Exception:
+            log.error("WFS Error")
+        return capabilities
 
-def get_capabilities(refresh=False, cache_file=None):
-    """
-    Request server capabilities (layer definitions).
-    Cache response as file daily, caching to location specified by:
-      - cache_file parameter
-      - $BCDATA_CACHE environment variable
-      - default (~/.bcdata)
-    """
-    if not cache_file:
-        if "BCDATA_CACHE" in os.environ:
-            cache_file = os.environ["BCDATA_CACHE"]
+    @retry(
+        stop=stop_after_delay(120), wait=wait_random_exponential(multiplier=1, max=60)
+    )
+    def _request_schema(self, table):
+        try:
+            # self.capabilities attribute is owslib.wfs.WebFeatureService instance
+            schema = self.capabilities.get_schema("pub:" + table)
+        except Exception:
+            log.error("WFS Error")
+        return schema
+
+    @retry(
+        retry=retry_if_exception_type(requests.exceptions.HTTPError),
+        stop=stop_after_delay(120),
+        wait=wait_random_exponential(multiplier=1, max=60),
+    )
+    def _request_count(self, table, query=None):
+        payload = {
+            "service": "WFS",
+            "version": "2.0.0",
+            "request": "GetFeature",
+            "typeName": table,
+            "resultType": "hits",
+            "outputFormat": "json",
+        }
+        if query:
+            payload["CQL_FILTER"] = query
+        try:
+            r = requests.get(self.wfs_url, params=payload)
+            log.debug(r.url)
+            log.debug(r.headers)
+            r.raise_for_status()  # check status code is 200
+            return int(ET.fromstring(r.text).attrib["numberMatched"])
+        except Exception:
+            log.debug("WFS error")
+
+    @retry(
+        retry=retry_if_exception_type(requests.exceptions.HTTPError),
+        stop=stop_after_delay(120),
+        wait=wait_random_exponential(multiplier=1, max=60),
+    )
+    def _request_features(self, url):
+        """Submit a getfeature request to DataBC WFS and return features"""
+        try:
+            r = requests.get(url)
+            log.info(r.url)
+            log.debug(r.headers)
+            r.raise_for_status()  # check status code is 200, otherwise HTTPError is raised
+            return r.json()["features"]
+        except Exception:
+            log.debug("WFS error")
+
+    def get_capabilities(self, refresh=False):
+        """
+        Request server capabilities (layer definitions).
+        Cache response as file daily, caching to one of:
+          - $BCDATA_CACHE environment variable
+          - default (~/.bcdata)
+        """
+        # request capabilities if cached capabilities file is > 1 day old or refresh is specified
+        if self.check_cached_file("capabilities.xml", days=1) or refresh:
+            with open(os.path.join(self.cache_path, "capabilities.xml"), "w") as f:
+                f.write(self._request_capabilities())
+        # load cached xml from file
+        with open(os.path.join(self.cache_path, "capabilities.xml"), "r") as f:
+            return WebFeatureService(self.ows_url, version="2.0.0", xml=f.read())
+
+    def get_count(self, dataset, query=None):
+        """Ask DataBC WFS how many features there are in a table/query"""
+        # https://gis.stackexchange.com/questions/45101/only-return-the-numberoffeatures-in-a-wfs-query
+        table = self.validate_name(dataset)
+        count = self._request_count(table, query)
+        log.info(self._request_count.retry.statistics)
+        return count
+
+    def get_schema(self, table, refresh=False):
+        # download table definition if file is > 30 days old, empty, or refresh is specified
+        if self.check_cached_file(table, days=30) or refresh:
+            with open(os.path.join(self.cache_path, table), "w") as f:
+                schema = self._request_schema(table)
+                f.write(json.dumps(schema, indent=4))
+        # load cached schema
+        with open(os.path.join(self.cache_path, table), "r") as f:
+            return json.loads(f.read())
+
+    def get_sortkey(self, table):
+        """Check data for unique columns available for sorting paged requests"""
+        columns = list(self.get_schema(table)["properties"].keys())
+        # use OBJECTID as default sort key, if present
+        if "OBJECTID" in columns:
+            return "OBJECTID"
+        # if OBJECTID is not present (several GSR tables), use SEQUENCE_ID
+        elif "SEQUENCE_ID" in columns:
+            return "SEQUENCE_ID"
+        # otherwise, it should be safe to presume first column is the primary key
+        # (WHSE_FOREST_VEGETATION.VEG_COMP_LYR_R1_POLY's FEATURE_ID appears to be
+        # the only public case, and very large veg downloads are likely better
+        # accessed via some other channel)
         else:
-            cache_file = os.path.join(str(Path.home()), ".bcdata")
+            return columns[0]
 
-    # download capabilites xml if file is > 1 day old or refresh is specified
-    if check_cache(cache_file) or refresh:
-        with open(cache_file, "w") as f:
-            f.write(
-                ET.tostring(
-                    WebFeatureService(OWS_URL, version="2.0.0")._capabilities,
-                    encoding="unicode",
-                )
+    def list_tables(self):
+        """Return a list of all tables available via WFS"""
+        return [i.strip("pub:") for i in list(self.capabilities.contents)]
+
+    def validate_name(self, dataset):
+        """Check wfs/cache and the bcdc api to see if dataset name is valid"""
+        if dataset.upper() in self.list_tables():
+            return dataset.upper()
+        else:
+            return bcdata.get_table_name(dataset.upper())
+
+    def define_requests(
+        self,
+        dataset,
+        query=None,
+        crs="epsg:4326",
+        bounds=None,
+        bounds_crs="EPSG:3005",
+        count=None,
+        sortby=None,
+        pagesize=10000,
+        check_count=True,
+    ):
+        """Translate provided parameters into a list of WFS request URLs required
+        to download the dataset as specified
+
+        References:
+        - http://www.opengeospatial.org/standards/wfs
+        - http://docs.geoserver.org/stable/en/user/services/wfs/vendor.html
+        - http://docs.geoserver.org/latest/en/user/tutorials/cql/cql_tutorial.html
+        """
+        # validate the table name
+        table = self.validate_name(dataset)
+        # find out how many records are in the table
+        if not count and check_count is False:
+            raise ValueError(
+                "{count: Null, check_count=False} is invalid, either provide record count or let bcdata request it"
             )
+        elif (
+            not count and check_count is True
+        ):  # if not provided a count, get one if not told otherwise
+            count = self.get_count(table, query=query)
+        elif (
+            count and check_count is True
+        ):  # if provided a count that is bigger than actual number of records, automatically correct count
+            n = self.get_count(table, query=query)
+            if count > n:
+                count = n
+
+        log.info(f"Total features requested: {count}")
+        schema = self.get_schema(table)
+        geom_column = schema["geometry_column"]
+
+        # for datasets with >10k records, generate a list of urls based on number of features in the dataset.
+        chunks = math.ceil(count / pagesize)
+
+        # if making several requests, we need to sort by something
+        if chunks > 1 and not sortby:
+            sortby = self.get_sortkey(table)
+
+        # build the request parameters for each chunk
+        urls = []
+        for i in range(chunks):
+            request = {
+                "service": "WFS",
+                "version": "2.0.0",
+                "request": "GetFeature",
+                "typeName": table,
+                "outputFormat": "json",
+                "SRSNAME": crs,
+            }
+            if sortby:
+                request["sortby"] = sortby.upper()
+            # build the CQL based on query and bounds
+            # (the bbox param shortcut is mutually exclusive with CQL_FILTER)
+            if query and not bounds:
+                request["CQL_FILTER"] = query
+            if bounds:
+                b0, b1, b2, b3 = [str(b) for b in bounds]
+                bnd_query = (
+                    f"bbox({geom_column}, {b0}, {b1}, {b2}, {b3}, '{bounds_crs}')"
+                )
+                if not query:
+                    request["CQL_FILTER"] = bnd_query
+                else:
+                    request["CQL_FILTER"] = query + " AND " + bnd_query
+            if chunks == 1:
+                request["count"] = count
+            if chunks > 1:
+                request["startIndex"] = i * pagesize
+                if count < (request["startIndex"] + pagesize):
+                    request["count"] = count - request["startIndex"]
+                else:
+                    request["count"] = pagesize
+            urls.append(self.wfs_url + "?" + urlencode(request, doseq=True))
+        return urls
+
+    def get_data(
+        self,
+        dataset,
+        query=None,
+        crs="epsg:4326",
+        bounds=None,
+        bounds_crs="epsg:3005",
+        count=None,
+        sortby=None,
+        pagesize=10000,
+        as_gdf=False,
+        lowercase=False,
+    ):
+        """Request features from DataBC WFS and return GeoJSON featurecollection or geodataframe"""
+        urls = self.define_requests(
+            dataset,
+            query=query,
+            crs=crs,
+            bounds=bounds,
+            bounds_crs=bounds_crs,
+            count=count,
+            sortby=sortby,
+            pagesize=pagesize,
+        )
+        # loop through requests
+        results = []
+        for url in urls:
+            results.append(self._request_features(url))
+            log.info(self._request_features.retry.statistics)
+
+        outjson = dict(type="FeatureCollection", features=[])
+        for result in results:
+            outjson["features"] += result
+        # if specified, lowercasify all properties
+        if lowercase:
+            for feature in outjson["features"]:
+                feature["properties"] = {
+                    k.lower(): v for k, v in feature["properties"].items()
+                }
+        if not as_gdf:
+            # If output crs is specified, include the crs object in the json
+            # But as default, we prefer to default to 4326 and RFC7946 (no crs)
+            if crs.lower() != "epsg:4326":
+                crs_int = crs.split(":")[1]
+                outjson[
+                    "crs"
+                ] = f"""{{"type":"name","properties":{{"name":"urn:ogc:def:crs:EPSG::{crs_int}"}}}}"""
+            return outjson
+        else:
+            if len(outjson["features"]) > 0:
+                gdf = gpd.GeoDataFrame.from_features(outjson)
+                gdf.crs = {"init": crs}
+            else:
+                gdf = gpd.GeoDataFrame()
+            return gdf
 
-    # load cached xml to WFS object
-    with open(cache_file, "r") as f:
-        return WebFeatureService(OWS_URL, version="2.0.0", xml=f.read())
-
-
-def get_sortkey(table, schema):
-    """Check data for unique columns available for sorting paged requests"""
-    columns = list(schema["properties"].keys())
-    # use OBJECTID as default sort key, if present
-    if "OBJECTID" in columns:
-        return "OBJECTID"
-    # if OBJECTID is not present (several GSR tables), use SEQUENCE_ID
-    elif "SEQUENCE_ID" in columns:
-        return "SEQUENCE_ID"
-    # otherwise, it should be safe to presume first column is the primary key
-    # (WHSE_FOREST_VEGETATION.VEG_COMP_LYR_R1_POLY's FEATURE_ID appears to be
-    # the only public case, and very large veg downloads are likely better
-    # accessed via some other channel)
-    else:
-        return columns[0]
+    def get_features(
+        self,
+        dataset,
+        query=None,
+        crs="epsg:4326",
+        bounds=None,
+        bounds_crs="epsg:3005",
+        count=None,
+        sortby=None,
+        pagesize=10000,
+        lowercase=False,
+        check_count=True,
+    ):
+        """Yield features from DataBC WFS"""
+        urls = self.define_requests(
+            dataset,
+            query=query,
+            crs=crs,
+            bounds=bounds,
+            bounds_crs=bounds_crs,
+            count=count,
+            sortby=sortby,
+            pagesize=pagesize,
+            check_count=check_count,
+        )
+        for url in urls:
+            for feature in self._request_features(url):
+                if lowercase:
+                    feature["properties"] = {
+                        k.lower(): v for k, v in feature["properties"].items()
+                    }
+                yield feature
+            log.info(self._request_features.retry.statistics)
+
+    def get_spatial_types(self, dataset, count=10):
+        """Return distinct types within the first n features"""
+        # validate the table name
+        table = self.validate_name(dataset)
+        log.info("Getting feature geometry type")
+        # get first n features, examine the feature geometry type (where geometry is not empty)
+        geom_types = []
+        for f in self.get_features(
+            table, count=count, check_count=False
+        ):  # to minimize network traffic, do not check record count for this requests
+            if f["geometry"]:
+                geom_type = f["geometry"]["type"].upper()
+                # only these geometry types are expected/supported
+                if geom_type not in (
+                    "POINT",
+                    "LINESTRING",
+                    "POLYGON",
+                    "MULTIPOINT",
+                    "MULTILINESTRING",
+                    "MULTIPOLYGON",
+                ):
+                    raise ValueError("Geometry type {geomtype} is not supported")
+                # look for z dimension, modify type if found
+                if (
+                    (geom_type == "POINT" and len(f["geometry"]["coordinates"]) == 3)
+                    or (
+                        geom_type == "MULTIPOINT"
+                        and len(f["geometry"]["coordinates"][0]) == 3
+                    )
+                    or (
+                        geom_type == "LINESTRING"
+                        and len(f["geometry"]["coordinates"][0]) == 3
+                    )
+                    or (
+                        geom_type == "MULTILINESTRING"
+                        and len(f["geometry"]["coordinates"][0][0]) == 3
+                    )
+                ):
+                    geom_type = geom_type + "Z"
+                geom_types.append(geom_type)
+        geom_types = list(set(geom_types))
+        # issue warning if types are mixed
+        if len(geom_types) > 1:
+            typestring = ",".join(geom_types)
+            log.warning(f"Dataset {dataset} has multiple geometry types: {typestring}")
+        return geom_types
 
 
-def validate_name(dataset):
-    """Check wfs/cache and the bcdc api to see if dataset name is valid"""
-    if dataset.upper() in list_tables():
-        return dataset.upper()
-    else:
-        return bcdata.get_table_name(dataset.upper())
-
-
-def list_tables(cache_file=None):
-    """Return a list of all tables available via WFS"""
-    capabilites = get_capabilities(cache_file)
-    return [i.strip("pub:") for i in list(capabilites.contents)]
-
-
-@retry(
-    retry=retry_if_exception_type(requests.exceptions.HTTPError),
-    stop=stop_after_delay(120),
-    wait=wait_random_exponential(multiplier=1, max=60),
-)
-def get_count(dataset, query=None):
-    """Ask DataBC WFS how many features there are in a table/query"""
-    # https://gis.stackexchange.com/questions/45101/only-return-the-numberoffeatures-in-a-wfs-query
-    table = validate_name(dataset)
-    payload = {
-        "service": "WFS",
-        "version": "2.0.0",
-        "request": "GetFeature",
-        "typeName": table,
-        "resultType": "hits",
-        "outputFormat": "json",
-    }
-    if query:
-        payload["CQL_FILTER"] = query
-    try:
-        r = requests.get(WFS_URL, params=payload)
-        log.debug(r.url)
-        log.debug(r.headers)
-        r.raise_for_status()  # check status code is 200
-        return int(ET.fromstring(r.text).attrib["numberMatched"])
-    except Exception:
-        log.debug("Network error")
+# abstract away the WFS object
 
 
 def define_requests(
     dataset,
     query=None,
     crs="epsg:4326",
     bounds=None,
     bounds_crs="EPSG:3005",
     count=None,
     sortby=None,
     pagesize=10000,
     check_count=True,
 ):
-    """Translate provided parameters into a list of WFS request URLs required
-    to download the dataset as specified
+    WFS = BCWFS()
+    return WFS.define_requests(
+        dataset,
+        query=query,
+        crs=crs,
+        bounds=bounds,
+        count=count,
+        sortby=sortby,
+        pagesize=pagesize,
+        check_count=check_count,
+    )
 
-    References:
-    - http://www.opengeospatial.org/standards/wfs
-    - http://docs.geoserver.org/stable/en/user/services/wfs/vendor.html
-    - http://docs.geoserver.org/latest/en/user/tutorials/cql/cql_tutorial.html
-    """
-    # validate the table name
-    table = validate_name(dataset)
-    # find out how many records are in the table
-    if not count and check_count is False:
-        raise ValueError(
-            "{count: Null, check_count=False} is invalid, either provide record count or let bcdata request it"
-        )
-    elif (
-        not count and check_count is True
-    ):  # if not provided a count, get one if not told otherwise
-        count = get_count(table, query=query)
-        log.info(get_count.retry.statistics)
-    elif (
-        count and check_count is True
-    ):  # if provided a count that is bigger than actual number of records, automatically correct count
-        n = get_count(table, query=query)
-        log.info(get_count.retry.statistics)
-        if count > n:
-            count = n
-
-    log.info(f"Total features requested: {count}")
-    wfs = get_capabilities()
-    schema = wfs.get_schema("pub:" + table)
-    geom_column = schema["geometry_column"]
-
-    # for datasets with >10k records, generate a list of urls based on number of features in the dataset.
-    chunks = math.ceil(count / pagesize)
-
-    # if making several requests, we need to sort by something
-    if chunks > 1 and not sortby:
-        sortby = get_sortkey(table, schema)
-
-    # build the request parameters for each chunk
-    urls = []
-    for i in range(chunks):
-        request = {
-            "service": "WFS",
-            "version": "2.0.0",
-            "request": "GetFeature",
-            "typeName": table,
-            "outputFormat": "json",
-            "SRSNAME": crs,
-        }
-        if sortby:
-            request["sortby"] = sortby.upper()
-        # build the CQL based on query and bounds
-        # (the bbox param shortcut is mutually exclusive with CQL_FILTER)
-        if query and not bounds:
-            request["CQL_FILTER"] = query
-        if bounds:
-            b0, b1, b2, b3 = [str(b) for b in bounds]
-            bnd_query = f"bbox({geom_column}, {b0}, {b1}, {b2}, {b3}, '{bounds_crs}')"
-            if not query:
-                request["CQL_FILTER"] = bnd_query
-            else:
-                request["CQL_FILTER"] = query + " AND " + bnd_query
-        if chunks == 1:
-            request["count"] = count
-        if chunks > 1:
-            request["startIndex"] = i * pagesize
-            if count < (request["startIndex"] + pagesize):
-                request["count"] = count - request["startIndex"]
-            else:
-                request["count"] = pagesize
-        urls.append(WFS_URL + "?" + urlencode(request, doseq=True))
-    return urls
-
-
-@retry(
-    retry=retry_if_exception_type(requests.exceptions.HTTPError),
-    stop=stop_after_delay(120),
-    wait=wait_random_exponential(multiplier=1, max=60),
-)
-def make_request(url):
-    """Submit a getfeature request to DataBC WFS and return features"""
-    r = requests.get(url)
-    log.info(r.url)
-    log.debug(r.headers)
-    r.raise_for_status()  # check status code is 200, otherwise HTTPError is raised
-    return r.json()["features"]
+
+def get_count(dataset, query=None):
+    WFS = BCWFS()
+    return WFS.get_count(dataset, query=query)
 
 
 def get_data(
     dataset,
     query=None,
     crs="epsg:4326",
     bounds=None,
     bounds_crs="epsg:3005",
     count=None,
     sortby=None,
     pagesize=10000,
     as_gdf=False,
     lowercase=False,
 ):
-    """Request features from DataBC WFS and return GeoJSON featurecollection or geodataframe"""
-    urls = define_requests(
+    WFS = BCWFS()
+    return WFS.get_data(
         dataset,
         query=query,
         crs=crs,
         bounds=bounds,
         bounds_crs=bounds_crs,
         count=count,
         sortby=sortby,
         pagesize=pagesize,
+        as_gdf=as_gdf,
+        lowercase=lowercase,
     )
-    # loop through requests
-    results = []
-    for url in urls:
-        results.append(make_request(url))
-        log.info(make_request.retry.statistics)
-
-    outjson = dict(type="FeatureCollection", features=[])
-    for result in results:
-        outjson["features"] += result
-    # if specified, lowercasify all properties
-    if lowercase:
-        for feature in outjson["features"]:
-            feature["properties"] = {
-                k.lower(): v for k, v in feature["properties"].items()
-            }
-    if not as_gdf:
-        # If output crs is specified, include the crs object in the json
-        # But as default, we prefer to default to 4326 and RFC7946 (no crs)
-        if crs.lower() != "epsg:4326":
-            crs_int = crs.split(":")[1]
-            outjson[
-                "crs"
-            ] = f"""{{"type":"name","properties":{{"name":"urn:ogc:def:crs:EPSG::{crs_int}"}}}}"""
-        return outjson
-    else:
-        if len(outjson["features"]) > 0:
-            gdf = gpd.GeoDataFrame.from_features(outjson)
-            gdf.crs = {"init": crs}
-        else:
-            gdf = gpd.GeoDataFrame()
-        return gdf
 
 
 def get_features(
     dataset,
     query=None,
     crs="epsg:4326",
     bounds=None,
     bounds_crs="epsg:3005",
     count=None,
     sortby=None,
     pagesize=10000,
     lowercase=False,
     check_count=True,
 ):
-    """Yield features from DataBC WFS"""
-    urls = define_requests(
+    WFS = BCWFS()
+    return WFS.get_features(
         dataset,
         query=query,
         crs=crs,
         bounds=bounds,
         bounds_crs=bounds_crs,
         count=count,
         sortby=sortby,
         pagesize=pagesize,
+        lowercase=lowercase,
         check_count=check_count,
     )
-    for url in urls:
-        for feature in make_request(url):
-            if lowercase:
-                feature["properties"] = {
-                    k.lower(): v for k, v in feature["properties"].items()
-                }
-            yield feature
-        log.info(make_request.retry.statistics)
 
 
-def get_types(dataset, count=10):
-    """Return distinct types within the first n features"""
-    # validate the table name
-    table = validate_name(dataset)
-    log.info("Getting feature geometry type")
-    # get first n features, examine the feature geometry type (where geometry is not empty)
-    geom_types = []
-    for f in get_features(
-        table, count=count, check_count=False
-    ):  # to minimize network traffic, do not check record count for this requests
-        if f["geometry"]:
-            geom_type = f["geometry"]["type"].upper()
-            # only these geometry types are expected/supported
-            if geom_type not in (
-                "POINT",
-                "LINESTRING",
-                "POLYGON",
-                "MULTIPOINT",
-                "MULTILINESTRING",
-                "MULTIPOLYGON",
-            ):
-                raise ValueError("Geometry type {geomtype} is not supported")
-            # look for z dimension, modify type if found
-            if (
-                (geom_type == "POINT" and len(f["geometry"]["coordinates"]) == 3)
-                or (
-                    geom_type == "MULTIPOINT"
-                    and len(f["geometry"]["coordinates"][0]) == 3
-                )
-                or (
-                    geom_type == "LINESTRING"
-                    and len(f["geometry"]["coordinates"][0]) == 3
-                )
-                or (
-                    geom_type == "MULTILINESTRING"
-                    and len(f["geometry"]["coordinates"][0][0]) == 3
-                )
-            ):
-                geom_type = geom_type + "Z"
-            geom_types.append(geom_type)
-    geom_types = list(set(geom_types))
-    # issue warning if types are mixed
-    if len(geom_types) > 1:
-        typestring = ",".join(geom_types)
-        log.warning(f"Dataset {dataset} has multiple geometry types: {typestring}")
-    return geom_types
+def get_spatial_types(dataset, count=10):
+    WFS = BCWFS()
+    return WFS.get_spatial_types(dataset, count=count)
+
+
+def list_tables(refresh=False):
+    WFS = BCWFS(refresh=refresh)
+    return WFS.list_tables()
+
+
+def validate_name(dataset):
+    WFS = BCWFS()
+    return WFS.validate_name(dataset)
```

### Comparing `bcdata-0.8.0a3/bcdata.egg-info/PKG-INFO` & `bcdata-0.8.0b1/bcdata.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bcdata
-Version: 0.8.0a3
+Version: 0.8.0b1
 Summary: Python tools for quick access to DataBC geo-data available via WFS
 Home-page: https://github.com/smnorris/bcdata
 Author: Simon Norris
 Author-email: snorris@hillcrestgeo.ca
 License: Apache
 Keywords: gis geospatial data BC DataBC download "Britsh Columbia"
 Classifier: Development Status :: 3 - Alpha
@@ -54,21 +54,26 @@
 The default target database connection (used by `bc2pg`) can be set via the `DATABASE_URL` environment variable (the password parameter should not be required if using a [.pgpass file](https://www.postgresql.org/docs/current/libpq-pgpass.html))
 
 Linux/Mac: `export DATABASE_URL=postgresql://{username}:{password}@{hostname}:{port}/{database}`
 
 Windows:   `SET DATABASE_URL=postgresql://{username}:{password}@{hostname}:{port}/{database}`
 
 
-#### Layer list cache file
+#### Layer list / layer schema cache
 
-A list of DataBC layers is cached to file to speed request validation. The cache is automatically refreshed if it is more than a day old.
-The cache file location defaults to `~/.bcdata`, but can be configured by setting the a `$BCDATA_CACHE` environment variable.
+To reduce the volume of requests, information about data requested is cached locally:
+ - the WFS GetCapabilities response xml (listing all datasets available via the service) is cached as `capabilities.xml`
+ - schemas of individual layers that have previously been requested are cached with the cache file name matching the object/table name
+
+`capabilities.xml` is automatically refreshed if it is more than a day old. The layer definition files are refreshed if more than 30 days old. These cache files are stored by default in `~/.bcdata`. Modify this location by  setting the the `$BCDATA_CACHE` environment variable:
 
 `export BCDATA_CACHE=/path/to/bcdata_cache`
 
+Force a cache refresh by deleting the files in the cache or the entire cache folder.
+
 ## Usage
 
 Typical usage will involve a manual search of the [DataBC Catalogue](https://catalogue.data.gov.bc.ca/dataset?download_audience=Public) to find a layer of interest. Once a dataset of interest is found, note the key with which to retreive it. This can be either the `id`/`package name` (the last portion of the url) or the `Object Name` (Under `Object Description`).
 
 For example, for [BC Airports]( https://catalogue.data.gov.bc.ca/dataset/bc-airports), either of these keys will work:
 
 - id/package name: `bc-airports`
@@ -143,15 +148,15 @@
   --query TEXT            A valid CQL or ECQL query
   -c, --count INTEGER     Total number of features to load
   -p, --pagesize INTEGER  Maximum request size
   -k, --primary_key TEXT  Primary key of dataset
   -s, --sortby TEXT       Name of sort field
   -e, --schema_only       Create empty table from catalogue schema
   -a, --append            Append to existing table
-  -t, --no_timestamp      Do not add download timestamp to bcdata meta table
+  -t, --no_timestamp      Do not log download to bcdata.log
   -v, --verbose           Increase verbosity.
   -q, --quiet             Decrease verbosity.
   --help                  Show this message and exit.
 ```
 
 #### cat
 
@@ -267,21 +272,21 @@
 Options:
   -r, --refresh  Refresh the cached list
   --help         Show this message and exit.
 ```
 
 #### CLI notes
 
-Note that `bc2pg` creates `public.bcdata` as a meta table tracking the most recent download date for each layer downloaded.
-Disable with the switch `--no_timestamp` if you do not wish to create this table or do not have access to `public` schema.
+Note that `bc2pg` creates `bcdata.log` and logs the most recent download date for each table downloaded.
+Disable with the switch `--no_timestamp` if you do not wish to create this table.
 
-Example of a record in `public.bcdata`:
+Example of a record in `bcdata.log`:
 
 ```
-mydb=# select * from bcdata;
+mydb=# select * from bcdata.log;
                  table_name                  |        date_downloaded
 ---------------------------------------------+-------------------------------
  whse_imagery_and_base_maps.gsr_airports_svw | 2021-02-17 11:50:34.044481-08
 ```
 
 
 #### CLI examples
```

### Comparing `bcdata-0.8.0a3/setup.py` & `bcdata-0.8.0b1/setup.py`

 * *Files identical despite different names*

### Comparing `bcdata-0.8.0a3/tests/test_bc2pg.py` & `bcdata-0.8.0b1/tests/test_bc2pg.py`

 * *Files identical despite different names*

### Comparing `bcdata-0.8.0a3/tests/test_bcdc.py` & `bcdata-0.8.0b1/tests/test_bcdc.py`

 * *Files identical despite different names*

### Comparing `bcdata-0.8.0a3/tests/test_cli.py` & `bcdata-0.8.0b1/tests/test_cli.py`

 * *Files identical despite different names*

