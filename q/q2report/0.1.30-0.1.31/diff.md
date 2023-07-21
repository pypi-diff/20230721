# Comparing `tmp/q2report-0.1.30.tar.gz` & `tmp/q2report-0.1.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "q2report-0.1.30.tar", max compression
+gzip compressed data, was "q2report-0.1.31.tar", max compression
```

## Comparing `q2report-0.1.30.tar` & `q2report-0.1.31.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    10347 2023-06-21 10:29:20.277459 q2report-0.1.30/LICENSE
--rw-r--r--   0        0        0      536 2023-07-14 11:52:23.769402 q2report-0.1.30/pyproject.toml
--rw-r--r--   0        0        0       42 2022-12-11 17:39:38.103740 q2report-0.1.30/q2report/__init__.py
--rw-r--r--   0        0        0        0 2022-12-11 17:39:38.103740 q2report-0.1.30/q2report/q2engine/__init__.py
--rw-r--r--   0        0        0      115 2022-12-11 17:39:38.103740 q2report-0.1.30/q2report/q2engine/q2engine_core.py
--rw-r--r--   0        0        0       90 2022-12-11 17:39:38.107739 q2report-0.1.30/q2report/q2engine/q2engine_pyqt.py
--rw-r--r--   0        0        0        0 2022-12-11 17:39:38.107739 q2report-0.1.30/q2report/q2printer/__init__.py
--rw-r--r--   0        0        0     8733 2023-07-12 19:54:50.695656 q2report-0.1.30/q2report/q2printer/docx_parts.py
--rw-r--r--   0        0        0     8479 2023-06-25 22:47:50.666231 q2report-0.1.30/q2report/q2printer/q2printer.py
--rw-r--r--   0        0        0    18818 2023-07-12 19:54:34.087531 q2report-0.1.30/q2report/q2printer/q2printer_docx.py
--rw-r--r--   0        0        0     6126 2023-06-21 17:49:50.189551 q2report-0.1.30/q2report/q2printer/q2printer_html.py
--rw-r--r--   0        0        0    20678 2023-06-21 17:49:55.953006 q2report-0.1.30/q2report/q2printer/q2printer_xlsx.py
--rw-r--r--   0        0        0     8792 2023-06-21 10:36:28.504330 q2report-0.1.30/q2report/q2printer/xlsx_parts.py
--rw-r--r--   0        0        0    30319 2023-07-13 08:40:44.679410 q2report-0.1.30/q2report/q2report.py
--rw-r--r--   0        0        0     1708 2023-02-10 16:01:23.063515 q2report-0.1.30/q2report/q2utils.py
--rw-r--r--   0        0        0       22 2023-07-14 11:52:30.631929 q2report-0.1.30/q2report/version.py
--rw-r--r--   0        0        0     1486 2022-12-11 17:39:38.099742 q2report-0.1.30/README.md
--rw-r--r--   0        0        0     1870 1970-01-01 00:00:00.000000 q2report-0.1.30/PKG-INFO
+-rw-r--r--   0        0        0    10347 2023-06-21 10:29:20.277459 q2report-0.1.31/LICENSE
+-rw-r--r--   0        0        0      536 2023-07-21 16:11:28.919106 q2report-0.1.31/pyproject.toml
+-rw-r--r--   0        0        0       42 2022-12-11 17:39:38.103740 q2report-0.1.31/q2report/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-11 17:39:38.103740 q2report-0.1.31/q2report/q2engine/__init__.py
+-rw-r--r--   0        0        0      115 2022-12-11 17:39:38.103740 q2report-0.1.31/q2report/q2engine/q2engine_core.py
+-rw-r--r--   0        0        0       90 2022-12-11 17:39:38.107739 q2report-0.1.31/q2report/q2engine/q2engine_pyqt.py
+-rw-r--r--   0        0        0        0 2022-12-11 17:39:38.107739 q2report-0.1.31/q2report/q2printer/__init__.py
+-rw-r--r--   0        0        0     8733 2023-07-12 19:54:50.695656 q2report-0.1.31/q2report/q2printer/docx_parts.py
+-rw-r--r--   0        0        0     8479 2023-06-25 22:47:50.666231 q2report-0.1.31/q2report/q2printer/q2printer.py
+-rw-r--r--   0        0        0    18818 2023-07-12 19:54:34.087531 q2report-0.1.31/q2report/q2printer/q2printer_docx.py
+-rw-r--r--   0        0        0     6126 2023-06-21 17:49:50.189551 q2report-0.1.31/q2report/q2printer/q2printer_html.py
+-rw-r--r--   0        0        0    20677 2023-07-21 15:58:27.016880 q2report-0.1.31/q2report/q2printer/q2printer_xlsx.py
+-rw-r--r--   0        0        0     8792 2023-06-21 10:36:28.504330 q2report-0.1.31/q2report/q2printer/xlsx_parts.py
+-rw-r--r--   0        0        0    30319 2023-07-13 08:40:44.679410 q2report-0.1.31/q2report/q2report.py
+-rw-r--r--   0        0        0     1708 2023-02-10 16:01:23.063515 q2report-0.1.31/q2report/q2utils.py
+-rw-r--r--   0        0        0       22 2023-07-21 16:11:34.573524 q2report-0.1.31/q2report/version.py
+-rw-r--r--   0        0        0     1486 2022-12-11 17:39:38.099742 q2report-0.1.31/README.md
+-rw-r--r--   0        0        0     1870 1970-01-01 00:00:00.000000 q2report-0.1.31/PKG-INFO
```

### Comparing `q2report-0.1.30/LICENSE` & `q2report-0.1.31/LICENSE`

 * *Files identical despite different names*

### Comparing `q2report-0.1.30/pyproject.toml` & `q2report-0.1.31/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "q2report"
-version = "0.1.30"
+version = "0.1.31"
 description = ""
 authors = ["Andrei Puchko <andrei.puchko@gmx.de>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1"
 pillow = "^9.4.0"
```

### Comparing `q2report-0.1.30/q2report/q2printer/docx_parts.py` & `q2report-0.1.31/q2report/q2printer/docx_parts.py`

 * *Files identical despite different names*

### Comparing `q2report-0.1.30/q2report/q2printer/q2printer.py` & `q2report-0.1.31/q2report/q2printer/q2printer.py`

 * *Files identical despite different names*

### Comparing `q2report-0.1.30/q2report/q2printer/q2printer_docx.py` & `q2report-0.1.31/q2report/q2printer/q2printer_docx.py`

 * *Files identical despite different names*

### Comparing `q2report-0.1.30/q2report/q2printer/q2printer_html.py` & `q2report-0.1.31/q2report/q2printer/q2printer_html.py`

 * *Files identical despite different names*

### Comparing `q2report-0.1.30/q2report/q2printer/q2printer_xlsx.py` & `q2report-0.1.31/q2report/q2printer/q2printer_xlsx.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,15 +104,15 @@
 
         wb_sheets = []
         wb_workbook_rels = []
         wb_images = []
         wb_content_types = []
 
         for img in range(0, len(self.xmlImageList)):
-            zipf.writestr(r"xl\media\image%s.png" % (img + 1), base64.b64decode(self.xmlImageList[img]))
+            zipf.writestr("xl/media/image%s.png" % (img + 1), base64.b64decode(self.xmlImageList[img]))
             wb_images.append(xlsx_parts["images"] % ((img + 1), (img + 1)))
 
         for x in range(0, len(self.xlsx_sheets)):
             wb_content_types.append(xlsx_parts["wb_content_types_sheet"] % (x + 1))
             drawing_det = []
             if self.xlsx_sheets[x]["drawing"]:
                 for img in range(0, len(self.xlsx_sheets[x]["drawing"])):
```

### Comparing `q2report-0.1.30/q2report/q2printer/xlsx_parts.py` & `q2report-0.1.31/q2report/q2printer/xlsx_parts.py`

 * *Files identical despite different names*

### Comparing `q2report-0.1.30/q2report/q2report.py` & `q2report-0.1.31/q2report/q2report.py`

 * *Files identical despite different names*

### Comparing `q2report-0.1.30/q2report/q2utils.py` & `q2report-0.1.31/q2report/q2utils.py`

 * *Files identical despite different names*

### Comparing `q2report-0.1.30/README.md` & `q2report-0.1.31/README.md`

 * *Files identical despite different names*

### Comparing `q2report-0.1.30/PKG-INFO` & `q2report-0.1.31/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: q2report
-Version: 0.1.30
+Version: 0.1.31
 Summary: 
 Author: Andrei Puchko
 Author-email: andrei.puchko@gmx.de
 Requires-Python: >=3.8.1
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

