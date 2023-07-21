# Comparing `tmp/gmlutil-0.8.1.tar.gz` & `tmp/gmlutil-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/gmlutil-0.8.1.tar", last modified: Wed May 24 00:53:51 2023, max compression
+gzip compressed data, was "dist/gmlutil-0.8.2.tar", last modified: Fri Jul 21 01:21:07 2023, max compression
```

## Comparing `gmlutil-0.8.1.tar` & `gmlutil-0.8.2.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxr-xr-x   0 phillip.kimejgallo.com   (502) staff       (20)        0 2023-05-24 00:53:51.099423 gmlutil-0.8.1/
--rw-r--r--   0 phillip.kimejgallo.com   (502) staff       (20)      905 2023-05-24 00:53:51.098928 gmlutil-0.8.1/PKG-INFO
--rw-r--r--   0 phillip.kimejgallo.com   (502) staff       (20)      199 2022-07-26 00:57:31.000000 gmlutil-0.8.1/README.md
-drwxr-xr-x   0 phillip.kimejgallo.com   (502) staff       (20)        0 2023-05-24 00:53:51.089037 gmlutil-0.8.1/gmlutil/
--rw-r--r--   0 phillip.kimejgallo.com   (502) staff       (20)       77 2022-07-25 19:26:55.000000 gmlutil-0.8.1/gmlutil/__init__.py
--rw-r--r--   0 phillip.kimejgallo.com   (502) staff       (20)    43871 2023-04-06 23:52:50.000000 gmlutil-0.8.1/gmlutil/gmlutil.py
-drwxr-xr-x   0 phillip.kimejgallo.com   (502) staff       (20)        0 2023-05-24 00:53:51.098031 gmlutil-0.8.1/gmlutil.egg-info/
--rw-r--r--   0 phillip.kimejgallo.com   (502) staff       (20)      905 2023-05-24 00:53:50.000000 gmlutil-0.8.1/gmlutil.egg-info/PKG-INFO
--rw-r--r--   0 phillip.kimejgallo.com   (502) staff       (20)      211 2023-05-24 00:53:50.000000 gmlutil-0.8.1/gmlutil.egg-info/SOURCES.txt
--rw-r--r--   0 phillip.kimejgallo.com   (502) staff       (20)        1 2023-05-24 00:53:50.000000 gmlutil-0.8.1/gmlutil.egg-info/dependency_links.txt
--rw-r--r--   0 phillip.kimejgallo.com   (502) staff       (20)      585 2023-05-24 00:53:50.000000 gmlutil-0.8.1/gmlutil.egg-info/requires.txt
--rw-r--r--   0 phillip.kimejgallo.com   (502) staff       (20)        8 2023-05-24 00:53:50.000000 gmlutil-0.8.1/gmlutil.egg-info/top_level.txt
--rw-r--r--   0 phillip.kimejgallo.com   (502) staff       (20)       38 2023-05-24 00:53:51.099598 gmlutil-0.8.1/setup.cfg
--rw-r--r--   0 phillip.kimejgallo.com   (502) staff       (20)     1825 2023-05-24 00:52:23.000000 gmlutil-0.8.1/setup.py
+drwxr-xr-x   0 phillip.kimejgallo.com   (502) staff       (20)        0 2023-07-21 01:21:07.108540 gmlutil-0.8.2/
+-rw-r--r--   0 phillip.kimejgallo.com   (502) staff       (20)      905 2023-07-21 01:21:07.107604 gmlutil-0.8.2/PKG-INFO
+-rw-r--r--   0 phillip.kimejgallo.com   (502) staff       (20)      199 2022-07-26 00:57:31.000000 gmlutil-0.8.2/README.md
+drwxr-xr-x   0 phillip.kimejgallo.com   (502) staff       (20)        0 2023-07-21 01:21:07.103271 gmlutil-0.8.2/gmlutil/
+-rw-r--r--   0 phillip.kimejgallo.com   (502) staff       (20)       77 2022-07-25 19:26:55.000000 gmlutil-0.8.2/gmlutil/__init__.py
+-rw-r--r--   0 phillip.kimejgallo.com   (502) staff       (20)    18486 2023-07-21 00:53:25.000000 gmlutil-0.8.2/gmlutil/gmlutil.py
+-rw-r--r--   0 phillip.kimejgallo.com   (502) staff       (20)    18728 2023-07-21 00:54:59.000000 gmlutil-0.8.2/gmlutil/gmlutil_ml.py
+-rw-r--r--   0 phillip.kimejgallo.com   (502) staff       (20)     6419 2023-07-21 00:56:17.000000 gmlutil-0.8.2/gmlutil/gmlutil_pre_ml.py
+drwxr-xr-x   0 phillip.kimejgallo.com   (502) staff       (20)        0 2023-07-21 01:21:07.106608 gmlutil-0.8.2/gmlutil.egg-info/
+-rw-r--r--   0 phillip.kimejgallo.com   (502) staff       (20)      905 2023-07-21 01:21:07.000000 gmlutil-0.8.2/gmlutil.egg-info/PKG-INFO
+-rw-r--r--   0 phillip.kimejgallo.com   (502) staff       (20)      259 2023-07-21 01:21:07.000000 gmlutil-0.8.2/gmlutil.egg-info/SOURCES.txt
+-rw-r--r--   0 phillip.kimejgallo.com   (502) staff       (20)        1 2023-07-21 01:21:07.000000 gmlutil-0.8.2/gmlutil.egg-info/dependency_links.txt
+-rw-r--r--   0 phillip.kimejgallo.com   (502) staff       (20)      572 2023-07-21 01:21:07.000000 gmlutil-0.8.2/gmlutil.egg-info/requires.txt
+-rw-r--r--   0 phillip.kimejgallo.com   (502) staff       (20)        8 2023-07-21 01:21:07.000000 gmlutil-0.8.2/gmlutil.egg-info/top_level.txt
+-rw-r--r--   0 phillip.kimejgallo.com   (502) staff       (20)       38 2023-07-21 01:21:07.109228 gmlutil-0.8.2/setup.cfg
+-rw-r--r--   0 phillip.kimejgallo.com   (502) staff       (20)     1807 2023-07-21 01:20:58.000000 gmlutil-0.8.2/setup.py
```

### Comparing `gmlutil-0.8.1/PKG-INFO` & `gmlutil-0.8.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: gmlutil
-Version: 0.8.1
+Version: 0.8.2
 Summary: General Machine Learning Utility Package
 Home-page: https://github.com/Phillip1982/gmlutil
 Author: Phillip Kim
 Author-email: phillip.kim@ejgallo.com
 License: BSD 2-clause
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `gmlutil-0.8.1/gmlutil.egg-info/PKG-INFO` & `gmlutil-0.8.2/gmlutil.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: gmlutil
-Version: 0.8.1
+Version: 0.8.2
 Summary: General Machine Learning Utility Package
 Home-page: https://github.com/Phillip1982/gmlutil
 Author: Phillip Kim
 Author-email: phillip.kim@ejgallo.com
 License: BSD 2-clause
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `gmlutil-0.8.1/gmlutil.egg-info/requires.txt` & `gmlutil-0.8.2/gmlutil.egg-info/requires.txt`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 folium==0.14.0
 fuzzywuzzy==0.18.0
 geopandas==0.10.2
 hana-ml
 imbalanced-learn==0.8.0
 jupyter_dash==0.4.0
 kmodes==0.11.0
-minio==4.0.6
 numpy==1.21.6
 pandas==1.3.0
 packaging==21.3
 plotly==5.4.0
 psycopg2-binary==2.9.1
 pyhdb==0.3.4
 pymssql==2.2.1
```

### Comparing `gmlutil-0.8.1/setup.py` & `gmlutil-0.8.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='gmlutil',
-    version='0.8.1',    
+    version='0.8.2',    
     description='General Machine Learning Utility Package',
     url='https://github.com/Phillip1982/gmlutil',
     author='Phillip Kim',
     author_email='phillip.kim@ejgallo.com',
     license='BSD 2-clause', ## Change this
     packages=['gmlutil'],
     install_requires=[
@@ -20,15 +20,14 @@
 		'folium==0.14.0',
 		'fuzzywuzzy==0.18.0',
 		'geopandas==0.10.2',
 		'hana-ml',
 		'imbalanced-learn==0.8.0',
 		'jupyter_dash==0.4.0',
 		'kmodes==0.11.0',
-		'minio==4.0.6',
 		'numpy==1.21.6',
 		'pandas==1.3.0',
         'packaging==21.3',
 		'plotly==5.4.0',
 		'psycopg2-binary==2.9.1',
 		'pyhdb==0.3.4',
 		'pymssql==2.2.1',
```

