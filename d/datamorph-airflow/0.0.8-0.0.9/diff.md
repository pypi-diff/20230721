# Comparing `tmp/datamorph-airflow-0.0.8.tar.gz` & `tmp/datamorph-airflow-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datamorph-airflow-0.0.8.tar", last modified: Fri May  6 00:09:09 2022, max compression
+gzip compressed data, was "datamorph-airflow-0.0.9.tar", last modified: Mon May  9 18:51:36 2022, max compression
```

## Comparing `datamorph-airflow-0.0.8.tar` & `datamorph-airflow-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,9 @@
-drwxr-xr-x   0 sowmyaannadatha   (501) staff       (20)        0 2022-05-06 00:09:09.205907 datamorph-airflow-0.0.8/
--rw-r--r--   0 sowmyaannadatha   (501) staff       (20)      731 2022-05-06 00:09:09.205319 datamorph-airflow-0.0.8/PKG-INFO
-drwxr-xr-x   0 sowmyaannadatha   (501) staff       (20)        0 2022-05-06 00:09:09.196992 datamorph-airflow-0.0.8/datamorph_airflow.egg-info/
--rw-r--r--   0 sowmyaannadatha   (501) staff       (20)      731 2022-05-06 00:09:08.000000 datamorph-airflow-0.0.8/datamorph_airflow.egg-info/PKG-INFO
--rw-r--r--   0 sowmyaannadatha   (501) staff       (20)      422 2022-05-06 00:09:09.000000 datamorph-airflow-0.0.8/datamorph_airflow.egg-info/SOURCES.txt
--rw-r--r--   0 sowmyaannadatha   (501) staff       (20)        1 2022-05-06 00:09:08.000000 datamorph-airflow-0.0.8/datamorph_airflow.egg-info/dependency_links.txt
--rw-r--r--   0 sowmyaannadatha   (501) staff       (20)       17 2022-05-06 00:09:09.000000 datamorph-airflow-0.0.8/datamorph_airflow.egg-info/top_level.txt
-drwxr-xr-x   0 sowmyaannadatha   (501) staff       (20)        0 2022-05-06 00:09:09.204427 datamorph-airflow-0.0.8/datamorphairflow/
--rw-r--r--   0 sowmyaannadatha   (501) staff       (20)      122 2022-05-03 20:44:02.000000 datamorph-airflow-0.0.8/datamorphairflow/__init__.py
--rw-r--r--   0 sowmyaannadatha   (501) staff       (20)       76 2022-05-06 00:09:05.000000 datamorph-airflow-0.0.8/datamorphairflow/__version__.py
--rw-r--r--   0 sowmyaannadatha   (501) staff       (20)      372 2022-05-03 20:36:50.000000 datamorph-airflow-0.0.8/datamorphairflow/helper_classes.py
--rw-r--r--   0 sowmyaannadatha   (501) staff       (20)     3831 2022-05-03 20:36:50.000000 datamorph-airflow-0.0.8/datamorphairflow/utils.py
--rw-r--r--   0 sowmyaannadatha   (501) staff       (20)     3963 2022-05-06 00:08:24.000000 datamorph-airflow-0.0.8/datamorphairflow/workflow_custom_operators.py
--rw-r--r--   0 sowmyaannadatha   (501) staff       (20)     4494 2022-05-03 20:44:02.000000 datamorph-airflow-0.0.8/datamorphairflow/workflow_dag_builder.py
--rw-r--r--   0 sowmyaannadatha   (501) staff       (20)     5004 2022-05-03 20:44:02.000000 datamorph-airflow-0.0.8/datamorphairflow/workflow_dag_factory.py
--rw-r--r--   0 sowmyaannadatha   (501) staff       (20)       38 2022-05-06 00:09:09.206096 datamorph-airflow-0.0.8/setup.cfg
--rw-r--r--   0 sowmyaannadatha   (501) staff       (20)     2863 2022-05-03 20:56:45.000000 datamorph-airflow-0.0.8/setup.py
+drwxr-xr-x   0 sowmyaannadatha   (501) staff       (20)        0 2022-05-09 18:51:36.836637 datamorph-airflow-0.0.9/
+-rw-r--r--   0 sowmyaannadatha   (501) staff       (20)      731 2022-05-09 18:51:36.836327 datamorph-airflow-0.0.9/PKG-INFO
+drwxr-xr-x   0 sowmyaannadatha   (501) staff       (20)        0 2022-05-09 18:51:36.835828 datamorph-airflow-0.0.9/datamorph_airflow.egg-info/
+-rw-r--r--   0 sowmyaannadatha   (501) staff       (20)      731 2022-05-09 18:51:36.000000 datamorph-airflow-0.0.9/datamorph_airflow.egg-info/PKG-INFO
+-rw-r--r--   0 sowmyaannadatha   (501) staff       (20)      172 2022-05-09 18:51:36.000000 datamorph-airflow-0.0.9/datamorph_airflow.egg-info/SOURCES.txt
+-rw-r--r--   0 sowmyaannadatha   (501) staff       (20)        1 2022-05-09 18:51:36.000000 datamorph-airflow-0.0.9/datamorph_airflow.egg-info/dependency_links.txt
+-rw-r--r--   0 sowmyaannadatha   (501) staff       (20)        1 2022-05-09 18:51:36.000000 datamorph-airflow-0.0.9/datamorph_airflow.egg-info/top_level.txt
+-rw-r--r--   0 sowmyaannadatha   (501) staff       (20)       38 2022-05-09 18:51:36.836743 datamorph-airflow-0.0.9/setup.cfg
+-rw-r--r--   0 sowmyaannadatha   (501) staff       (20)     2903 2022-05-09 18:50:50.000000 datamorph-airflow-0.0.9/setup.py
```

### Comparing `datamorph-airflow-0.0.8/PKG-INFO` & `datamorph-airflow-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datamorph-airflow
-Version: 0.0.8
+Version: 0.0.9
 Summary: DataMorph's application to dynamically build Airflow DAGs from JSON files 
 Author: Annapurna Annadatha
 Author-email: sowmya@kwartile.com
 License: MIT
 Keywords: airflow
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `datamorph-airflow-0.0.8/datamorph_airflow.egg-info/PKG-INFO` & `datamorph-airflow-0.0.9/datamorph_airflow.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datamorph-airflow
-Version: 0.0.8
+Version: 0.0.9
 Summary: DataMorph's application to dynamically build Airflow DAGs from JSON files 
 Author: Annapurna Annadatha
 Author-email: sowmya@kwartile.com
 License: MIT
 Keywords: airflow
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `datamorph-airflow-0.0.8/setup.py` & `datamorph-airflow-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,16 @@
 PKG_NAME = "datamorphairflow"
 DESCRIPTION = "DataMorph's application to dynamically build Airflow DAGs from JSON files "
 EMAIL = "sowmya@kwartile.com"
 AUTHOR = "Annapurna Annadatha"
 REQUIRES_PYTHON = ">=3.6.0"
 VERSION = None
 
-here = os.path.abspath(os.path.dirname(__file__))
+maindir = os.path.abspath(os.path.dirname(__file__))
+here = os.path.join(maindir, "dags")
 
 REQUIRED = []
 
 try:
     with io.open(os.path.join(here, "README.md"), encoding="utf-8") as f:
         long_description = "\n" + f.read()
 except FileNotFoundError:
```

