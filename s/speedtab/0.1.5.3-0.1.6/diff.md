# Comparing `tmp/speedtab-0.1.5.3.tar.gz` & `tmp/speedtab-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "speedtab-0.1.5.3.tar", max compression
+gzip compressed data, was "speedtab-0.1.6.tar", max compression
```

## Comparing `speedtab-0.1.5.3.tar` & `speedtab-0.1.6.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      567 2023-07-21 14:15:16.447146 speedtab-0.1.5.3/pyproject.toml
--rw-r--r--   0        0        0      313 2023-07-21 14:14:08.403849 speedtab-0.1.5.3/speedtab/__init__.py
--rw-r--r--   0        0        0    51743 2023-07-19 10:28:24.519337 speedtab-0.1.5.3/speedtab/client.py
--rw-r--r--   0        0        0     6464 2023-07-21 14:14:08.469136 speedtab-0.1.5.3/speedtab/enums.py
--rw-r--r--   0        0        0     1848 2023-07-21 13:53:11.575405 speedtab-0.1.5.3/speedtab/formats.py
--rw-r--r--   0        0        0      783 2023-07-21 14:15:20.677967 speedtab-0.1.5.3/setup.py
--rw-r--r--   0        0        0      808 2023-07-21 14:15:20.677967 speedtab-0.1.5.3/PKG-INFO
+-rw-r--r--   0        0        0      565 2023-07-21 15:38:15.828874 speedtab-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      313 2023-07-21 14:14:08.403849 speedtab-0.1.6/speedtab/__init__.py
+-rw-r--r--   0        0        0    51816 2023-07-21 15:37:22.088653 speedtab-0.1.6/speedtab/client.py
+-rw-r--r--   0        0        0     6464 2023-07-21 14:14:08.469136 speedtab-0.1.6/speedtab/enums.py
+-rw-r--r--   0        0        0     1848 2023-07-21 13:53:11.575405 speedtab-0.1.6/speedtab/formats.py
+-rw-r--r--   0        0        0      781 2023-07-21 15:38:47.322866 speedtab-0.1.6/setup.py
+-rw-r--r--   0        0        0      806 2023-07-21 15:38:47.323866 speedtab-0.1.6/PKG-INFO
```

### Comparing `speedtab-0.1.5.3/pyproject.toml` & `speedtab-0.1.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "speedtab"
-version = "0.1.5.3"
+version = "0.1.6"
 description = "Convenient wrapper for working with Google Spreadsheets"
 authors = ["Bogdan Gergel <bogger147@gmail.com>"]
 license = "MIT"
 homepage = "https://github.com/BoggerSancho/SpeedTab-beta"
 repository = "https://github.com/BoggerSancho/SpeedTab-beta"
 
 [tool.poetry.dependencies]
```

### Comparing `speedtab-0.1.5.3/speedtab/client.py` & `speedtab-0.1.6/speedtab/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from google_auth_oauthlib.flow import InstalledAppFlow
 from googleapiclient.discovery import build
 from googleapiclient.errors import HttpError
 from googleapiclient.http import MediaIoBaseDownload
 
 from speedtab.enums import MergeType, BorderStyle, HorizontalAlignment, VerticalAlignment, WrapStrategy, ShareRole, \
     ChartType, StackedType, LegendPosition, AxisPosition, BooleanConditionTypes, BorderSides
-from speedtab.formats import Color, Border, Number, BaseNumberFormat
+from speedtab.formats import Color, Border, Number, BaseNumberFormat, Text
 
 SCOPES = ['https://www.googleapis.com/auth/spreadsheets', 'https://www.googleapis.com/auth/drive', 'https://www.googleapis.com/auth/drive.file']
 SHIFT_DIM = {
     'startRowIndex': 0,
     'startColumnIndex': 0,
     'endRowIndex': 1,
     'endColumnIndex': 1,
@@ -138,21 +138,21 @@
         self._get_metadata()
         self._task_queue = []
 
     def _regroup_tasks(self):
         groups = []
         for id in [x.get('sheetId') for x in self.sheets.values()]:
             current_id_tasks = [x for x in self._task_queue if x.sheetId == id]
-            clear_ids = [0] + [i for i, x in enumerate(current_id_tasks) if x.task_type == 'clear']
-            groups_ids = clear_ids[:1] + [clear_ids[i] for i in range(1, len(clear_ids))
-                                          if clear_ids[i] - clear_ids[i - 1] > 1] + [len(current_id_tasks)]
+            clear_ids = [i for i, x in enumerate(current_id_tasks) if x.task_type == 'clear']
+            group_ids = tuple(set([0] + [j for i, j in zip([-2] + clear_ids, clear_ids) if j - i != 1] + [len(current_id_tasks)]))
+            splitted_tasks = [current_id_tasks[i:j] for i, j in zip(group_ids, group_ids[1:])]
 
             merged_group = []
             shift = []
-            for elem in [current_id_tasks[i:j] for i, j in [groups_ids[i:i + 2] for i in range(0, len(groups_ids) - 1, 1)]]:
+            for elem in splitted_tasks:
                 if not any(d.task_type == 'data' for d in elem):
                     shift += elem
                 else:
                     merged_group.append(elem + shift)
                     shift = []
             if shift:
                 merged_group.append(shift)
@@ -815,15 +815,19 @@
                 },
                 'fields': 'gridProperties.frozenRowCount, gridProperties.frozenColumnCount'
             }
         }, self.work_zone))
         return self
 
     def set_num_format(self, default_format: BaseNumberFormat = Number):
-        self._task_queue.append(Task('format', self._increment_task(), self.sheet_id, {
+        if isinstance(default_format, Text):
+            task_type = 'clear'
+        else:
+            task_type = 'format'
+        self._task_queue.append(Task(task_type, self._increment_task(), self.sheet_id, {
                 'repeatCell': {
                     'range': self.work_zone,
                     **default_format.__dict__,
                 }}, self.work_zone))
         return self
 
     def set_sheet_size(self, rows: int, columns: int):
```

### Comparing `speedtab-0.1.5.3/speedtab/enums.py` & `speedtab-0.1.6/speedtab/enums.py`

 * *Files identical despite different names*

### Comparing `speedtab-0.1.5.3/speedtab/formats.py` & `speedtab-0.1.6/speedtab/formats.py`

 * *Files identical despite different names*

### Comparing `speedtab-0.1.5.3/setup.py` & `speedtab-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 install_requires = \
 ['google-api-python-client>=2.58.0,<3.0.0',
  'google-auth-httplib2>=0.1.0,<0.2.0',
  'google-auth-oauthlib>=0.5.2,<0.6.0']
 
 setup_kwargs = {
     'name': 'speedtab',
-    'version': '0.1.5.3',
+    'version': '0.1.6',
     'description': 'Convenient wrapper for working with Google Spreadsheets',
     'long_description': None,
     'author': 'Bogdan Gergel',
     'author_email': 'bogger147@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/BoggerSancho/SpeedTab-beta',
```

### Comparing `speedtab-0.1.5.3/PKG-INFO` & `speedtab-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speedtab
-Version: 0.1.5.3
+Version: 0.1.6
 Summary: Convenient wrapper for working with Google Spreadsheets
 Home-page: https://github.com/BoggerSancho/SpeedTab-beta
 License: MIT
 Author: Bogdan Gergel
 Author-email: bogger147@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

