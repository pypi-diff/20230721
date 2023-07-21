# Comparing `tmp/work_helper-0.1.4.tar.gz` & `tmp/work_helper-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "work_helper-0.1.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "work_helper-0.1.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `work_helper-0.1.4.tar` & `work_helper-0.1.5.tar`

### file list

```diff
@@ -1,16 +1,20 @@
--rw-r--r--   0        0        0     3299 2023-07-06 09:22:47.552925 work_helper-0.1.4/.gitignore
--rw-r--r--   0        0        0      137 2023-05-26 09:35:55.498254 work_helper-0.1.4/.vscode/settings.json
--rw-r--r--   0        0        0     1096 2023-05-26 05:27:24.425923 work_helper-0.1.4/LICENSE
--rw-r--r--   0        0        0     1028 2023-07-20 07:46:26.575214 work_helper-0.1.4/helper/__init__.py
--rw-r--r--   0        0        0        0 2023-05-26 09:19:44.138475 work_helper-0.1.4/helper/base/__init__.py
--rw-r--r--   0        0        0      964 2023-05-26 09:37:12.856686 work_helper-0.1.4/helper/base/logger.py
--rw-r--r--   0        0        0     6823 2023-07-11 02:47:38.373322 work_helper-0.1.4/helper/ddl.py
--rw-r--r--   0        0        0     9980 2023-07-20 07:45:48.842275 work_helper-0.1.4/helper/etl.py
--rw-r--r--   0        0        0     2781 2023-06-29 05:45:56.244212 work_helper-0.1.4/helper/hello.py
--rw-r--r--   0        0        0     2425 2023-06-13 09:22:21.003065 work_helper-0.1.4/helper/helm.py
--rw-r--r--   0        0        0     1787 2023-06-16 08:50:08.249839 work_helper-0.1.4/helper/pack.py
--rwxr-xr-x   0        0        0       31 2023-07-07 08:28:54.281342 work_helper-0.1.4/publish.bat
--rw-r--r--   0        0        0      586 2023-07-07 08:54:34.601578 work_helper-0.1.4/pyproject.toml
--rw-r--r--   0        0        0    28606 2023-07-06 08:51:45.579410 work_helper-0.1.4/samples/ddl.sample.xlsx
--rw-r--r--   0        0        0    64824 2023-07-06 08:44:39.364263 work_helper-0.1.4/samples/etl.sample.xlsx
--rw-r--r--   0        0        0      228 1970-01-01 00:00:00.000000 work_helper-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     3299 2023-07-06 09:22:47.552925 work_helper-0.1.5/.gitignore
+-rw-r--r--   0        0        0      137 2023-05-26 09:35:55.498254 work_helper-0.1.5/.vscode/settings.json
+-rw-r--r--   0        0        0     1096 2023-05-26 05:27:24.425923 work_helper-0.1.5/LICENSE
+-rw-r--r--   0        0        0       42 2023-07-21 03:17:41.170703 work_helper-0.1.5/helper/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-21 01:55:03.150596 work_helper-0.1.5/helper/base/__init__.py
+-rw-r--r--   0        0        0      964 2023-05-26 09:37:12.856686 work_helper-0.1.5/helper/base/logger.py
+-rw-r--r--   0        0        0      982 2023-07-21 01:47:33.488887 work_helper-0.1.5/helper/base/writer.py
+-rw-r--r--   0        0        0     6835 2023-07-21 01:58:25.243114 work_helper-0.1.5/helper/ddl.py
+-rw-r--r--   0        0        0     3367 2023-07-21 01:57:27.948417 work_helper-0.1.5/helper/etl.py
+-rw-r--r--   0        0        0     2781 2023-06-29 05:45:56.244212 work_helper-0.1.5/helper/hello.py
+-rw-r--r--   0        0        0     2494 2023-07-21 03:17:07.995972 work_helper-0.1.5/helper/helm.py
+-rw-r--r--   0        0        0     1787 2023-06-16 08:50:08.249839 work_helper-0.1.5/helper/pack.py
+-rw-r--r--   0        0        0        0 2023-07-20 08:24:35.264640 work_helper-0.1.5/helper/plugin/__init__.py
+-rw-r--r--   0        0        0     4097 2023-07-21 01:57:49.170293 work_helper-0.1.5/helper/plugin/etl_base.py
+-rw-r--r--   0        0        0     3443 2023-07-21 01:57:56.401119 work_helper-0.1.5/helper/plugin/etl_postgre.py
+-rwxr-xr-x   0        0        0       31 2023-07-07 08:28:54.281342 work_helper-0.1.5/publish.bat
+-rw-r--r--   0        0        0      586 2023-07-07 08:54:34.601578 work_helper-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0    28606 2023-07-06 08:51:45.579410 work_helper-0.1.5/samples/ddl.sample.xlsx
+-rw-r--r--   0        0        0    64824 2023-07-06 08:44:39.364263 work_helper-0.1.5/samples/etl.sample.xlsx
+-rw-r--r--   0        0        0      228 1970-01-01 00:00:00.000000 work_helper-0.1.5/PKG-INFO
```

### Comparing `work_helper-0.1.4/.gitignore` & `work_helper-0.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `work_helper-0.1.4/LICENSE` & `work_helper-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `work_helper-0.1.4/helper/__init__.py` & `work_helper-0.1.5/helper/base/writer.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,7 @@
-"""helper tool"""
-__version__ = "0.1.4"
-
-
 from typing import TextIO
 
 
 class EnhancedWriter:
     def __init__(self, file: TextIO | str) -> None:
         if isinstance(file, str):
             self.writer = open(file, mode="w", encoding="utf-8")
```

### Comparing `work_helper-0.1.4/helper/base/logger.py` & `work_helper-0.1.5/helper/base/logger.py`

 * *Files identical despite different names*

### Comparing `work_helper-0.1.4/helper/ddl.py` & `work_helper-0.1.5/helper/ddl.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import argparse
 from helper.base.logger import log
 from openpyxl import load_workbook, Workbook
 from openpyxl.worksheet.worksheet import Worksheet
 from openpyxl.cell.read_only import ReadOnlyCell
 import os
 from typing import Protocol
-from helper import EnhancedWriter
+from helper.base.writer import EnhancedWriter
 
 __version__ = "0.0.3"
 
 
 class Args(Protocol):
     file: str
     lowercase: bool
```

### Comparing `work_helper-0.1.4/helper/hello.py` & `work_helper-0.1.5/helper/hello.py`

 * *Files identical despite different names*

### Comparing `work_helper-0.1.4/helper/helm.py` & `work_helper-0.1.5/helper/helm.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,15 +16,15 @@
             elif os.path.exists(os.path.join(path, "values.yaml")):
                 parse_charts(path, dir, namespace)
 
 
 def parse_charts(path: str, app: str, namespace: str):
     log.info(f"处理Helm Charts：{path}")
     os.system(
-        f"helm template {path} -n {namespace} > {os.path.join(YAMLS_DIR,app+'.yaml')}"
+        f"helm template {path} -n {namespace} | sed -e 's/imagePullPolicy:\sAlways/imagePullPolicy: IfNotPresent/' > {os.path.join(YAMLS_DIR,app+'.yaml')}"
     )
 
 
 def parse_infrastructure(path: str):
     log.info(f"处理基础定义：{path}")
     fi = open(os.path.join(YAMLS_DIR, "infrastructure.yaml"), "w", encoding="utf-8")
     for entry in os.listdir(path):
```

### Comparing `work_helper-0.1.4/helper/pack.py` & `work_helper-0.1.5/helper/pack.py`

 * *Files identical despite different names*

### Comparing `work_helper-0.1.4/pyproject.toml` & `work_helper-0.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `work_helper-0.1.4/samples/ddl.sample.xlsx` & `work_helper-0.1.5/samples/ddl.sample.xlsx`

 * *Files identical despite different names*

### Comparing `work_helper-0.1.4/samples/etl.sample.xlsx` & `work_helper-0.1.5/samples/etl.sample.xlsx`

 * *Files identical despite different names*

