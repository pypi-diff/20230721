# Comparing `tmp/idbadapter-1.9.3.tar.gz` & `tmp/idbadapter-1.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idbadapter-1.9.3.tar", last modified: Thu Jul 20 09:19:03 2023, max compression
+gzip compressed data, was "idbadapter-1.9.4.tar", last modified: Fri Jul 21 10:15:43 2023, max compression
```

## Comparing `idbadapter-1.9.3.tar` & `idbadapter-1.9.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-20 09:19:03.554492 idbadapter-1.9.3/
--rw-rw-rw-   0        0        0    11558 2023-05-02 13:28:55.000000 idbadapter-1.9.3/LICENSE
--rw-rw-rw-   0        0        0      697 2023-07-20 09:19:03.554492 idbadapter-1.9.3/PKG-INFO
--rw-rw-rw-   0        0        0      182 2023-05-05 13:33:15.000000 idbadapter-1.9.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-20 09:19:03.544494 idbadapter-1.9.3/idbadapter/
--rw-rw-rw-   0        0        0       61 2023-05-22 08:18:39.000000 idbadapter-1.9.3/idbadapter/__init__.py
--rw-rw-rw-   0        0        0    12394 2023-07-20 09:17:19.000000 idbadapter-1.9.3/idbadapter/schedule_loader.py
-drwxrwxrwx   0        0        0        0 2023-07-20 09:19:03.554492 idbadapter-1.9.3/idbadapter.egg-info/
--rw-rw-rw-   0        0        0      697 2023-07-20 09:19:03.000000 idbadapter-1.9.3/idbadapter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2023-07-20 09:19:03.000000 idbadapter-1.9.3/idbadapter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-20 09:19:03.000000 idbadapter-1.9.3/idbadapter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-07-20 09:19:03.000000 idbadapter-1.9.3/idbadapter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-20 09:19:03.000000 idbadapter-1.9.3/idbadapter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-20 09:19:03.555494 idbadapter-1.9.3/setup.cfg
--rw-rw-rw-   0        0        0      991 2023-07-20 09:19:00.000000 idbadapter-1.9.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 10:15:43.768760 idbadapter-1.9.4/
+-rw-rw-rw-   0        0        0    11558 2023-05-15 08:54:26.000000 idbadapter-1.9.4/LICENSE
+-rw-rw-rw-   0        0        0      697 2023-07-21 10:15:43.768760 idbadapter-1.9.4/PKG-INFO
+-rw-rw-rw-   0        0        0      182 2023-05-15 08:54:26.000000 idbadapter-1.9.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-21 10:15:43.741796 idbadapter-1.9.4/idbadapter/
+-rw-rw-rw-   0        0        0       61 2023-05-15 08:54:26.000000 idbadapter-1.9.4/idbadapter/__init__.py
+-rw-rw-rw-   0        0        0    11857 2023-07-21 10:14:59.000000 idbadapter-1.9.4/idbadapter/schedule_loader.py
+drwxrwxrwx   0        0        0        0 2023-07-21 10:15:43.767760 idbadapter-1.9.4/idbadapter.egg-info/
+-rw-rw-rw-   0        0        0      697 2023-07-21 10:15:43.000000 idbadapter-1.9.4/idbadapter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2023-07-21 10:15:43.000000 idbadapter-1.9.4/idbadapter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 10:15:43.000000 idbadapter-1.9.4/idbadapter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-07-21 10:15:43.000000 idbadapter-1.9.4/idbadapter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-21 10:15:43.000000 idbadapter-1.9.4/idbadapter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-21 10:15:43.770761 idbadapter-1.9.4/setup.cfg
+-rw-rw-rw-   0        0        0      991 2023-07-21 10:15:36.000000 idbadapter-1.9.4/setup.py
```

### Comparing `idbadapter-1.9.3/LICENSE` & `idbadapter-1.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `idbadapter-1.9.3/PKG-INFO` & `idbadapter-1.9.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idbadapter
-Version: 1.9.3
+Version: 1.9.4
 Summary: Сache module for batch loading of data
 Home-page: https://github.com/AnatolyPershinov/gpn_cache_module
 Download-URL: https://github.com/AnatolyPershinov/gpn_cache_module/archive/master.zip
 Author: Anatoly Pershinov
 Author-email: anatoliypershinov@gmail.com
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `idbadapter-1.9.3/idbadapter/schedule_loader.py` & `idbadapter-1.9.4/idbadapter/schedule_loader.py`

 * *Files 12% similar despite different names*

```diff
@@ -77,15 +77,14 @@
         if len(self.objects) == 0:
             raise Exception("Objects not found")
         
         return self
            
     def get_resources_names(self, res_type=GRANULARY):
         query = f"SELECT DISTINCT name FROM {res_type['res_table']}"
-        print(query)
         df = self._execute_query(query)
         return df
         
     def get_works_names(self, work_type=GRANULARY):
         query = f"SELECT DISTINCT name FROM {work_type['table']}"
         df = self._execute_query(query)
         return df
@@ -155,25 +154,14 @@
         join granulary_works gw on gw.id = wi.id_granulary_work 
         join typed_lvl2_works tlw on tlw.id = wi.id_typed_lvl2_work 
         join processed_works pn on pn.id = wi.id_processed_work"""
         
         df = self._execute_query(query)
         return df
     
-    def get_all_resources_name(self):
-        query = f"""
-            select DISTINCT w.name as work_name, gw.name as granulary_name, tlw.name as lvl2_name, pn.name as processed_name from basic_resources w
-        join resources_info wi on w.id = wi.id_resource  
-        join granulary_resources gw on gw.id = wi.id_granulary_name
-        join typed_lvl2_resources tlw on tlw.id = wi.id_typed_lvl2_name
-        join processed_resources pn on pn.id = wi.id_processed_name"""
-        print(query)
-        df = self._execute_query(query)
-        return df
-    
     def get_works_by_pulls(self, work_pulls: list, resource_list: list = [], key=GRANULARY, path_to_log="empty_pull.txt"):
         self.path_to_log = path_to_log
         for pull in work_pulls:
             query = f"""with date_cte (date, object_id)
                 as (
                     (select date, object_id from works_names_mv wnm
                     where wnm.{key["column"]} in ({','.join(map(lambda x: f"'{x}'", pull))})
@@ -198,20 +186,22 @@
                 
             if len(resource_list) != 0:
                 query += f""" and rnm.{key["column"]} in ({",".join(map(lambda x: f"'{x}'", resource_list))})"""   
             try:
                 df = self._execute_query(query)
             except ValueError:
                 print("jsondecodeerror occurred", pull)
+                yield None
                 continue 
 
             if df.empty:
                 with open(self.path_to_log, "a", encoding="UTF-8") as f:
                     print("pull not found", pull, file=f)
                     print("empty df. pull not found")
+                yield None
                 continue
                 
             df["full_fraction"] = df["physical_volume"]
                       
                 
             yield SchedulesIterator.convert_df(df)
```

### Comparing `idbadapter-1.9.3/idbadapter.egg-info/PKG-INFO` & `idbadapter-1.9.4/idbadapter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idbadapter
-Version: 1.9.3
+Version: 1.9.4
 Summary: Сache module for batch loading of data
 Home-page: https://github.com/AnatolyPershinov/gpn_cache_module
 Download-URL: https://github.com/AnatolyPershinov/gpn_cache_module/archive/master.zip
 Author: Anatoly Pershinov
 Author-email: anatoliypershinov@gmail.com
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `idbadapter-1.9.3/setup.py` & `idbadapter-1.9.4/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 #!/usr/bin/env python
 
 from distutils.core import setup
 
-version = '1.9.3'
+version = '1.9.4'
 
 long_description = "Сache module for batch loading of data"
 
 setup(name='idbadapter',
-      version='1.9.3',
+      version='1.9.4',
       description='Сache module for batch loading of data',
       long_description=long_description,
       url="https://github.com/AnatolyPershinov/gpn_cache_module",
       download_url='https://github.com/AnatolyPershinov/gpn_cache_module/archive/master.zip',
       author='Anatoly Pershinov',
       author_email='anatoliypershinov@gmail.com',
       packages=['idbadapter'],
```

