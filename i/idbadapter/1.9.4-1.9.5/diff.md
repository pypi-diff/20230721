# Comparing `tmp/idbadapter-1.9.4.tar.gz` & `tmp/idbadapter-1.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idbadapter-1.9.4.tar", last modified: Fri Jul 21 10:15:43 2023, max compression
+gzip compressed data, was "idbadapter-1.9.5.tar", last modified: Fri Jul 21 12:01:54 2023, max compression
```

## Comparing `idbadapter-1.9.4.tar` & `idbadapter-1.9.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-21 10:15:43.768760 idbadapter-1.9.4/
--rw-rw-rw-   0        0        0    11558 2023-05-15 08:54:26.000000 idbadapter-1.9.4/LICENSE
--rw-rw-rw-   0        0        0      697 2023-07-21 10:15:43.768760 idbadapter-1.9.4/PKG-INFO
--rw-rw-rw-   0        0        0      182 2023-05-15 08:54:26.000000 idbadapter-1.9.4/README.md
-drwxrwxrwx   0        0        0        0 2023-07-21 10:15:43.741796 idbadapter-1.9.4/idbadapter/
--rw-rw-rw-   0        0        0       61 2023-05-15 08:54:26.000000 idbadapter-1.9.4/idbadapter/__init__.py
--rw-rw-rw-   0        0        0    11857 2023-07-21 10:14:59.000000 idbadapter-1.9.4/idbadapter/schedule_loader.py
-drwxrwxrwx   0        0        0        0 2023-07-21 10:15:43.767760 idbadapter-1.9.4/idbadapter.egg-info/
--rw-rw-rw-   0        0        0      697 2023-07-21 10:15:43.000000 idbadapter-1.9.4/idbadapter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2023-07-21 10:15:43.000000 idbadapter-1.9.4/idbadapter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 10:15:43.000000 idbadapter-1.9.4/idbadapter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-07-21 10:15:43.000000 idbadapter-1.9.4/idbadapter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-21 10:15:43.000000 idbadapter-1.9.4/idbadapter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-21 10:15:43.770761 idbadapter-1.9.4/setup.cfg
--rw-rw-rw-   0        0        0      991 2023-07-21 10:15:36.000000 idbadapter-1.9.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 12:01:54.532580 idbadapter-1.9.5/
+-rw-rw-rw-   0        0        0    11558 2023-05-15 08:54:26.000000 idbadapter-1.9.5/LICENSE
+-rw-rw-rw-   0        0        0      697 2023-07-21 12:01:54.532580 idbadapter-1.9.5/PKG-INFO
+-rw-rw-rw-   0        0        0      182 2023-05-15 08:54:26.000000 idbadapter-1.9.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-21 12:01:54.507974 idbadapter-1.9.5/idbadapter/
+-rw-rw-rw-   0        0        0       61 2023-05-15 08:54:26.000000 idbadapter-1.9.5/idbadapter/__init__.py
+-rw-rw-rw-   0        0        0    12395 2023-07-21 11:59:19.000000 idbadapter-1.9.5/idbadapter/schedule_loader.py
+drwxrwxrwx   0        0        0        0 2023-07-21 12:01:54.530603 idbadapter-1.9.5/idbadapter.egg-info/
+-rw-rw-rw-   0        0        0      697 2023-07-21 12:01:54.000000 idbadapter-1.9.5/idbadapter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2023-07-21 12:01:54.000000 idbadapter-1.9.5/idbadapter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 12:01:54.000000 idbadapter-1.9.5/idbadapter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-07-21 12:01:54.000000 idbadapter-1.9.5/idbadapter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-21 12:01:54.000000 idbadapter-1.9.5/idbadapter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-21 12:01:54.534571 idbadapter-1.9.5/setup.cfg
+-rw-rw-rw-   0        0        0      991 2023-07-21 12:01:39.000000 idbadapter-1.9.5/setup.py
```

### Comparing `idbadapter-1.9.4/LICENSE` & `idbadapter-1.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `idbadapter-1.9.4/PKG-INFO` & `idbadapter-1.9.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idbadapter
-Version: 1.9.4
+Version: 1.9.5
 Summary: Сache module for batch loading of data
 Home-page: https://github.com/AnatolyPershinov/gpn_cache_module
 Download-URL: https://github.com/AnatolyPershinov/gpn_cache_module/archive/master.zip
 Author: Anatoly Pershinov
 Author-email: anatoliypershinov@gmail.com
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `idbadapter-1.9.4/idbadapter/schedule_loader.py` & `idbadapter-1.9.5/idbadapter/schedule_loader.py`

 * *Files 9% similar despite different names*

```diff
@@ -154,14 +154,25 @@
         join granulary_works gw on gw.id = wi.id_granulary_work 
         join typed_lvl2_works tlw on tlw.id = wi.id_typed_lvl2_work 
         join processed_works pn on pn.id = wi.id_processed_work"""
         
         df = self._execute_query(query)
         return df
     
+    def get_all_resources_name(self):
+        query = f"""
+        select DISTINCT w.name as name, gw.name as granulary_name, tlw.name as lvl2_name, pn.name as processed_name from basic_resources w
+        join resources_info wi on w.id = wi.id_resource  
+        join granulary_resources gw on gw.id = wi.id_granulary_name
+        join typed_lvl2_resources tlw on tlw.id = wi.id_typed_lvl2_name
+        join processed_resources pn on pn.id = wi.id_processed_name"""
+
+        df = self._execute_query(query)
+        return df
+
     def get_works_by_pulls(self, work_pulls: list, resource_list: list = [], key=GRANULARY, path_to_log="empty_pull.txt"):
         self.path_to_log = path_to_log
         for pull in work_pulls:
             query = f"""with date_cte (date, object_id)
                 as (
                     (select date, object_id from works_names_mv wnm
                     where wnm.{key["column"]} in ({','.join(map(lambda x: f"'{x}'", pull))})
```

### Comparing `idbadapter-1.9.4/idbadapter.egg-info/PKG-INFO` & `idbadapter-1.9.5/idbadapter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idbadapter
-Version: 1.9.4
+Version: 1.9.5
 Summary: Сache module for batch loading of data
 Home-page: https://github.com/AnatolyPershinov/gpn_cache_module
 Download-URL: https://github.com/AnatolyPershinov/gpn_cache_module/archive/master.zip
 Author: Anatoly Pershinov
 Author-email: anatoliypershinov@gmail.com
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `idbadapter-1.9.4/setup.py` & `idbadapter-1.9.5/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 #!/usr/bin/env python
 
 from distutils.core import setup
 
-version = '1.9.4'
+version = '1.9.5'
 
 long_description = "Сache module for batch loading of data"
 
 setup(name='idbadapter',
-      version='1.9.4',
+      version='1.9.5',
       description='Сache module for batch loading of data',
       long_description=long_description,
       url="https://github.com/AnatolyPershinov/gpn_cache_module",
       download_url='https://github.com/AnatolyPershinov/gpn_cache_module/archive/master.zip',
       author='Anatoly Pershinov',
       author_email='anatoliypershinov@gmail.com',
       packages=['idbadapter'],
```

