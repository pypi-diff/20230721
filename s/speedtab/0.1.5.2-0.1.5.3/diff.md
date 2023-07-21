# Comparing `tmp/speedtab-0.1.5.2.tar.gz` & `tmp/speedtab-0.1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "speedtab-0.1.5.2.tar", max compression
+gzip compressed data, was "speedtab-0.1.5.3.tar", max compression
```

## Comparing `speedtab-0.1.5.2.tar` & `speedtab-0.1.5.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      567 2023-07-19 09:28:47.751877 speedtab-0.1.5.2/pyproject.toml
--rw-r--r--   0        0        0      365 2023-06-09 12:04:52.821400 speedtab-0.1.5.2/speedtab/__init__.py
--rw-r--r--   0        0        0    51548 2023-07-19 09:36:08.833821 speedtab-0.1.5.2/speedtab/client.py
--rw-r--r--   0        0        0     6192 2023-05-19 11:01:11.239027 speedtab-0.1.5.2/speedtab/enums.py
--rw-r--r--   0        0        0     1724 2023-06-02 10:10:18.366392 speedtab-0.1.5.2/speedtab/formats.py
--rw-r--r--   0        0        0      783 2023-07-19 09:36:26.046315 speedtab-0.1.5.2/setup.py
--rw-r--r--   0        0        0      808 2023-07-19 09:36:26.046315 speedtab-0.1.5.2/PKG-INFO
+-rw-r--r--   0        0        0      567 2023-07-21 14:15:16.447146 speedtab-0.1.5.3/pyproject.toml
+-rw-r--r--   0        0        0      313 2023-07-21 14:14:08.403849 speedtab-0.1.5.3/speedtab/__init__.py
+-rw-r--r--   0        0        0    51743 2023-07-19 10:28:24.519337 speedtab-0.1.5.3/speedtab/client.py
+-rw-r--r--   0        0        0     6464 2023-07-21 14:14:08.469136 speedtab-0.1.5.3/speedtab/enums.py
+-rw-r--r--   0        0        0     1848 2023-07-21 13:53:11.575405 speedtab-0.1.5.3/speedtab/formats.py
+-rw-r--r--   0        0        0      783 2023-07-21 14:15:20.677967 speedtab-0.1.5.3/setup.py
+-rw-r--r--   0        0        0      808 2023-07-21 14:15:20.677967 speedtab-0.1.5.3/PKG-INFO
```

### Comparing `speedtab-0.1.5.2/pyproject.toml` & `speedtab-0.1.5.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "speedtab"
-version = "0.1.5.2"
+version = "0.1.5.3"
 description = "Convenient wrapper for working with Google Spreadsheets"
 authors = ["Bogdan Gergel <bogger147@gmail.com>"]
 license = "MIT"
 homepage = "https://github.com/BoggerSancho/SpeedTab-beta"
 repository = "https://github.com/BoggerSancho/SpeedTab-beta"
 
 [tool.poetry.dependencies]
```

### Comparing `speedtab-0.1.5.2/speedtab/client.py` & `speedtab-0.1.5.3/speedtab/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -838,14 +838,20 @@
                     },
                     'fields': 'gridProperties.rowCount, gridProperties.columnCount',
                 }}, self.work_zone))
 
         return self
 
     def set_size(self, size: int = None, axis: Union[str, int] = 1):
+        '''
+        In Google Sheets, the default cell width is 100 pixels, and the default cell height is 21 pixels.
+        :param size:
+        :param axis:
+        :return:
+        '''
         axis = axis.upper() if isinstance(axis, str) else DIMENSION.get(axis)
         self._task_queue.append(Task('format', self._increment_task(), self.sheet_id, {
                 'updateDimensionProperties': {
                     'range': {
                         'sheetId': self.sheet_id,
                         'dimension': axis,
                         'startIndex': self.work_zone.get('startRowIndex') if axis == 'ROWS' else self.work_zone.get('startColumnIndex'),
```

### Comparing `speedtab-0.1.5.2/speedtab/enums.py` & `speedtab-0.1.5.3/speedtab/enums.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from speedtab.formats import Color, Number, Dollar, Percent, Date, Time, DateTime, Scientific
+from speedtab.formats import Color, Number, Dollar, Percent, Date, Time, DateTime, Scientific, Text
 
 
 class BorderStyle:
     SOLID = 'SOLID'
     SOLID_MEDIUM = 'SOLID_MEDIUM'
     SOLID_THICK = 'SOLID_THICK'
     DOTTED = 'DOTTED'
@@ -181,25 +181,38 @@
     LIGHT_MAGENTA1 = Color('#c27ba0')
     DARK_MAGENTA1 = Color('#a64d79')
     DARK_MAGENTA2 = Color('#741b47')
     DARK_MAGENTA3 = Color('#4c1130')
 
 
 class ReadyFormats:
-    NUMBER = Number()
+    DATE = Date()
+    DATETIME = DateTime()
     DECIMAL = Number('0.00')
+    DECIMAL_PERCENT = Percent('0.00%')
     DOLLAR = Dollar()
+    NUMBER = Number()
     PRETTY_DOLLAR = Dollar('_($* #,##0.00_);_($* -#,##0.00;_($* "-"??_);_(@_)')
     PERCENT = Percent()
-    DECIMAL_PERCENT = Percent('0.00%')
-    DATE = Date()
-    TIME = Time()
-    DATETIME = DateTime()
     SCIENTIFIC = Scientific()
+    TEXT = Text()
+    TIME = Time()
+
 
+class CustomFormats:
+    DATE = Date
+    DATETIME = DateTime
+    DECIMAL = Number
+    DECIMAL_PERCENT = Percent
+    DOLLAR = Dollar
+    NUMBER = Number
+    PERCENT = Percent
+    SCIENTIFIC = Scientific
+    TEXT = Text
+    TIME = Time
 
 class BorderSides:
     ALL_BORDERS = ('top', 'bottom', 'left', 'right', 'innerHorizontal', 'innerVertical')
     INNER_BORDERS = ('innerHorizontal', 'innerVertical')
     OUTER_BORDERS = ('top', 'bottom', 'left', 'right')
     TOP_BORDER = ('top',)
     BOTTOM_BORDER = ('bottom',)
```

### Comparing `speedtab-0.1.5.2/speedtab/formats.py` & `speedtab-0.1.5.3/speedtab/formats.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,14 +37,19 @@
 
 
 class Time(BaseNumberFormat):
     def __init__(self, pattern: str = 'hh:mm:ss'):
         super().__init__('TIME', pattern)
 
 
+class Text(BaseNumberFormat):
+    def __init__(self, pattern: str = None):
+        super().__init__('TEXT', pattern)
+
+
 class DateTime(BaseNumberFormat):
     def __init__(self, pattern: str = 'yyyy-mm-dd hh:mm:ss'):
         super().__init__('DATE_TIME', pattern)
 
 
 class Scientific(BaseNumberFormat):
     def __init__(self, pattern: str = '0.00E+00'):
```

### Comparing `speedtab-0.1.5.2/setup.py` & `speedtab-0.1.5.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 install_requires = \
 ['google-api-python-client>=2.58.0,<3.0.0',
  'google-auth-httplib2>=0.1.0,<0.2.0',
  'google-auth-oauthlib>=0.5.2,<0.6.0']
 
 setup_kwargs = {
     'name': 'speedtab',
-    'version': '0.1.5.2',
+    'version': '0.1.5.3',
     'description': 'Convenient wrapper for working with Google Spreadsheets',
     'long_description': None,
     'author': 'Bogdan Gergel',
     'author_email': 'bogger147@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/BoggerSancho/SpeedTab-beta',
```

### Comparing `speedtab-0.1.5.2/PKG-INFO` & `speedtab-0.1.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speedtab
-Version: 0.1.5.2
+Version: 0.1.5.3
 Summary: Convenient wrapper for working with Google Spreadsheets
 Home-page: https://github.com/BoggerSancho/SpeedTab-beta
 License: MIT
 Author: Bogdan Gergel
 Author-email: bogger147@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

