# Comparing `tmp/labelbase-0.1.2.tar.gz` & `tmp/labelbase-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "labelbase-0.1.2.tar", last modified: Fri Jul 14 22:14:44 2023, max compression
+gzip compressed data, was "labelbase-0.1.3.tar", last modified: Fri Jul 21 16:59:54 2023, max compression
```

## Comparing `labelbase-0.1.2.tar` & `labelbase-0.1.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:14:44.608208 labelbase-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-14 22:14:33.000000 labelbase-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-14 22:14:44.608208 labelbase-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-14 22:14:33.000000 labelbase-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:14:44.608208 labelbase-0.1.2/labelbase/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-14 22:14:33.000000 labelbase-0.1.2/labelbase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26651 2023-07-14 22:14:33.000000 labelbase-0.1.2/labelbase/annotate.py
--rw-r--r--   0 runner    (1001) docker     (123)    14012 2023-07-14 22:14:33.000000 labelbase-0.1.2/labelbase/connector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:14:44.608208 labelbase-0.1.2/labelbase/converters/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-14 22:14:33.000000 labelbase-0.1.2/labelbase/converters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15660 2023-07-14 22:14:33.000000 labelbase-0.1.2/labelbase/converters/coco.py
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-07-14 22:14:33.000000 labelbase-0.1.2/labelbase/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     8181 2023-07-14 22:14:33.000000 labelbase-0.1.2/labelbase/downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-07-14 22:14:33.000000 labelbase-0.1.2/labelbase/masks.py
--rw-r--r--   0 runner    (1001) docker     (123)     9948 2023-07-14 22:14:33.000000 labelbase-0.1.2/labelbase/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-07-14 22:14:33.000000 labelbase-0.1.2/labelbase/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5680 2023-07-14 22:14:33.000000 labelbase-0.1.2/labelbase/ontology.py
--rw-r--r--   0 runner    (1001) docker     (123)    26163 2023-07-14 22:14:33.000000 labelbase-0.1.2/labelbase/uploader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:14:44.608208 labelbase-0.1.2/labelbase.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-14 22:14:44.000000 labelbase-0.1.2/labelbase.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-14 22:14:44.000000 labelbase-0.1.2/labelbase.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 22:14:44.000000 labelbase-0.1.2/labelbase.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-14 22:14:44.000000 labelbase-0.1.2/labelbase.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-14 22:14:44.000000 labelbase-0.1.2/labelbase.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 22:14:44.608208 labelbase-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-14 22:14:33.000000 labelbase-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:59:54.831920 labelbase-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-21 16:59:43.000000 labelbase-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-21 16:59:54.831920 labelbase-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-21 16:59:43.000000 labelbase-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:59:54.831920 labelbase-0.1.3/labelbase/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-21 16:59:43.000000 labelbase-0.1.3/labelbase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26651 2023-07-21 16:59:43.000000 labelbase-0.1.3/labelbase/annotate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14012 2023-07-21 16:59:43.000000 labelbase-0.1.3/labelbase/connector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:59:54.831920 labelbase-0.1.3/labelbase/converters/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-21 16:59:43.000000 labelbase-0.1.3/labelbase/converters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15660 2023-07-21 16:59:43.000000 labelbase-0.1.3/labelbase/converters/coco.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-07-21 16:59:43.000000 labelbase-0.1.3/labelbase/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8181 2023-07-21 16:59:43.000000 labelbase-0.1.3/labelbase/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-07-21 16:59:43.000000 labelbase-0.1.3/labelbase/masks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9948 2023-07-21 16:59:43.000000 labelbase-0.1.3/labelbase/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-07-21 16:59:43.000000 labelbase-0.1.3/labelbase/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5680 2023-07-21 16:59:43.000000 labelbase-0.1.3/labelbase/ontology.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25499 2023-07-21 16:59:43.000000 labelbase-0.1.3/labelbase/uploader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:59:54.831920 labelbase-0.1.3/labelbase.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-21 16:59:54.000000 labelbase-0.1.3/labelbase.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-21 16:59:54.000000 labelbase-0.1.3/labelbase.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 16:59:54.000000 labelbase-0.1.3/labelbase.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-21 16:59:54.000000 labelbase-0.1.3/labelbase.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-21 16:59:54.000000 labelbase-0.1.3/labelbase.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 16:59:54.831920 labelbase-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-21 16:59:43.000000 labelbase-0.1.3/setup.py
```

### Comparing `labelbase-0.1.2/LICENSE` & `labelbase-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `labelbase-0.1.2/PKG-INFO` & `labelbase-0.1.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labelbase
-Version: 0.1.2
+Version: 0.1.3
 Summary: Labelbox Helper Library
 Home-page: https://labelbox.com
 Author: Labelbox
 Author-email: raphael@labelbox.com
 Keywords: labelbox,labelbase
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `labelbase-0.1.2/labelbase/annotate.py` & `labelbase-0.1.3/labelbase/annotate.py`

 * *Files identical despite different names*

### Comparing `labelbase-0.1.2/labelbase/connector.py` & `labelbase-0.1.3/labelbase/connector.py`

 * *Files identical despite different names*

### Comparing `labelbase-0.1.2/labelbase/converters/coco.py` & `labelbase-0.1.3/labelbase/converters/coco.py`

 * *Files identical despite different names*

### Comparing `labelbase-0.1.2/labelbase/dataset.py` & `labelbase-0.1.3/labelbase/dataset.py`

 * *Files identical despite different names*

### Comparing `labelbase-0.1.2/labelbase/downloader.py` & `labelbase-0.1.3/labelbase/downloader.py`

 * *Files identical despite different names*

### Comparing `labelbase-0.1.2/labelbase/masks.py` & `labelbase-0.1.3/labelbase/masks.py`

 * *Files identical despite different names*

### Comparing `labelbase-0.1.2/labelbase/metadata.py` & `labelbase-0.1.3/labelbase/metadata.py`

 * *Files identical despite different names*

### Comparing `labelbase-0.1.2/labelbase/models.py` & `labelbase-0.1.3/labelbase/models.py`

 * *Files identical despite different names*

### Comparing `labelbase-0.1.2/labelbase/ontology.py` & `labelbase-0.1.3/labelbase/ontology.py`

 * *Files identical despite different names*

### Comparing `labelbase-0.1.2/labelbase/uploader.py` & `labelbase-0.1.3/labelbase/uploader.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,43 +33,36 @@
         gks = global_keys[i:] if i + batch_size >= len(global_keys) else global_keys[i:i+batch_size]  
         res = client.get_data_row_ids_for_global_keys(gks, timeout_seconds=timeout_seconds)
         if res['errors']:
             raise ValueError(f"{res}")
         global_key_to_data_row_dict.update({gks[i] : res['results'][i] for i in range(0, len(gks))})
     return global_key_to_data_row_dict
 
-def check_global_keys(client:labelboxClient, global_keys:list, batch_size=20000):
+def check_global_keys(client:labelboxClient, global_keys:list, batch_size=1000):
     """ Checks if data rows exist for a set of global keys - if data rows exist, returns as dictionary { key=data_row_id : value=global_key }
     Args:
         client                  :   Required (labelbox.client.Client) - Labelbox Client object    
         global_keys             :   Required (list(str)) - List of global key strings
         batch_size              :   Optional (int) - Query check batch size, 20,000 is recommended        
     Returns:
         existing_drid_to_gk     :   Dictinoary where { key=data_row_id : value=global_key }
                                     If this = {}, then all global keys are free to use
     """
     # Initiate a dictionary where { key=data_row_id : value=global_key }
     existing_drid_to_gk = {}
     # Enforce global keys as strings
     global_keys_list = [str(x) for x in global_keys]      
-    # Create a query job to get data row IDs given global keys
-    query_str_1 = """query get_datarow_with_global_key($global_keys:[ID!]!){dataRowsForGlobalKeys(where:{ids:$global_keys}){jobId}}"""
-    query_str_2 = """query get_job_result($job_id:ID!){dataRowsForGlobalKeysResult(jobId:{id:$job_id}){data{
-                    accessDeniedGlobalKeys\ndeletedDataRowGlobalKeys\nfetchedDataRows{id}\nnotFoundGlobalKeys}jobStatus}}"""      
     # Batch global key checks
     for i in range(0, len(global_keys_list), batch_size):
         batch_gks = global_keys_list[i:] if i + batch_size >= len(global_keys_list) else global_keys_list[i:i+batch_size]  
-        # Run the query job
-        res = None
-        while not res:
-            query_job_id = client.execute(query_str_1, {"global_keys":batch_gks})['dataRowsForGlobalKeys']['jobId']
-            res = client.execute(query_str_2, {"job_id":query_job_id})['dataRowsForGlobalKeysResult']['data']       
+        # Get the datarow ids
+        res = client.get_data_row_ids_for_global_keys(batch_gks)     
         # Check query job results for fetched data rows
-        for i in range(0, len(res["fetchedDataRows"])):
-            data_row_id = res["fetchedDataRows"][i]["id"]
+        for i in range(0, len(res["results"])):
+            data_row_id = res["results"][i]
             if data_row_id:
                 existing_drid_to_gk[data_row_id] = batch_gks[i]
     return existing_drid_to_gk
 
 def batch_create_data_rows(
     client:labelboxClient, upload_dict:dict, skip_duplicates:bool=True, 
     divider:str="___", batch_size:int=20000, verbose:bool=False):
```

### Comparing `labelbase-0.1.2/labelbase.egg-info/PKG-INFO` & `labelbase-0.1.3/labelbase.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labelbase
-Version: 0.1.2
+Version: 0.1.3
 Summary: Labelbox Helper Library
 Home-page: https://labelbox.com
 Author: Labelbox
 Author-email: raphael@labelbox.com
 Keywords: labelbox,labelbase
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `labelbase-0.1.2/setup.py` & `labelbase-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
       name='labelbase',
-      version='0.1.02',
+      version='0.1.03',
       author='Labelbox',
       author_email='raphael@labelbox.com',
       description='Labelbox Helper Library',      
       packages=setuptools.find_packages(),
       url="https://labelbox.com",
       long_description=long_description,
       long_description_content_type="text/markdown",
```

