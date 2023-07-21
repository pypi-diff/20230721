# Comparing `tmp/uw-webdriver-recorder-5.0.6.tar.gz` & `tmp/uw-webdriver-recorder-5.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uw-webdriver-recorder-5.0.6.tar", max compression
+gzip compressed data, was "uw-webdriver-recorder-5.0.7.tar", max compression
```

## Comparing `uw-webdriver-recorder-5.0.6.tar` & `uw-webdriver-recorder-5.0.7.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0    11399 2022-12-01 19:02:24.582832 uw-webdriver-recorder-5.0.6/LICENSE
--rw-r--r--   0        0        0     1233 2022-12-01 19:02:49.154738 uw-webdriver-recorder-5.0.6/pyproject.toml
--rw-r--r--   0        0        0        0 2022-12-01 19:02:24.582832 uw-webdriver-recorder-5.0.6/webdriver_recorder/__init__.py
--rw-r--r--   0        0        0    14968 2022-12-01 19:02:24.582832 uw-webdriver-recorder-5.0.6/webdriver_recorder/browser.py
--rw-r--r--   0        0        0     1645 2022-12-01 19:02:24.582832 uw-webdriver-recorder-5.0.6/webdriver_recorder/export-report.py
--rw-r--r--   0        0        0     4304 2022-12-01 19:02:24.582832 uw-webdriver-recorder-5.0.6/webdriver_recorder/models.py
--rw-r--r--   0        0        0    13209 2022-12-01 19:02:24.582832 uw-webdriver-recorder-5.0.6/webdriver_recorder/plugin.py
--rw-r--r--   0        0        0     4100 2022-12-01 19:02:24.582832 uw-webdriver-recorder-5.0.6/webdriver_recorder/report_exporter.py
--rw-r--r--   0        0        0     3100 2022-12-01 19:02:24.582832 uw-webdriver-recorder-5.0.6/webdriver_recorder/templates/help.html
--rw-r--r--   0        0        0     1924 2022-12-01 19:02:24.582832 uw-webdriver-recorder-5.0.6/webdriver_recorder/templates/modal.html
--rw-r--r--   0        0        0     1194 2022-12-01 19:02:24.582832 uw-webdriver-recorder-5.0.6/webdriver_recorder/templates/modal_link.html
--rw-r--r--   0        0        0     1302 2022-12-01 19:02:24.582832 uw-webdriver-recorder-5.0.6/webdriver_recorder/templates/report.html
--rw-r--r--   0        0        0     2622 2022-12-01 19:02:24.582832 uw-webdriver-recorder-5.0.6/webdriver_recorder/templates/report_header.html
--rw-r--r--   0        0        0     4010 2022-12-01 19:02:24.582832 uw-webdriver-recorder-5.0.6/webdriver_recorder/templates/static/report.js
--rw-r--r--   0        0        0     3517 2022-12-01 19:02:24.582832 uw-webdriver-recorder-5.0.6/webdriver_recorder/templates/static/style.css
--rw-r--r--   0        0        0     5542 2022-12-01 19:02:24.582832 uw-webdriver-recorder-5.0.6/webdriver_recorder/templates/test_case.html
--rw-r--r--   0        0        0     1167 2022-12-01 19:02:24.582832 uw-webdriver-recorder-5.0.6/webdriver_recorder/templates/test_screenshots.html
--rw-r--r--   0        0        0      542 2022-12-01 19:02:24.582832 uw-webdriver-recorder-5.0.6/webdriver_recorder/templates/toast-copied-to-clipboard.html
--rw-r--r--   0        0        0      961 2022-12-01 19:08:25.009775 uw-webdriver-recorder-5.0.6/setup.py
--rw-r--r--   0        0        0      841 2022-12-01 19:08:25.010075 uw-webdriver-recorder-5.0.6/PKG-INFO
+-rw-r--r--   0        0        0    11399 2023-07-21 02:20:56.087407 uw-webdriver-recorder-5.0.7/LICENSE
+-rw-r--r--   0        0        0   326542 2023-05-27 00:10:14.000000 uw-webdriver-recorder-5.0.7/LICENSE.chromedriver
+-rw-r--r--   0        0        0     1259 2023-07-21 02:21:21.859716 uw-webdriver-recorder-5.0.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-21 02:20:56.087407 uw-webdriver-recorder-5.0.7/webdriver_recorder/__init__.py
+-rw-r--r--   0        0        0    14968 2023-07-21 02:20:56.087407 uw-webdriver-recorder-5.0.7/webdriver_recorder/browser.py
+-rw-r--r--   0        0        0     1645 2023-07-21 02:20:56.087407 uw-webdriver-recorder-5.0.7/webdriver_recorder/export-report.py
+-rw-r--r--   0        0        0     4304 2023-07-21 02:20:56.087407 uw-webdriver-recorder-5.0.7/webdriver_recorder/models.py
+-rw-r--r--   0        0        0    13209 2023-07-21 02:20:56.087407 uw-webdriver-recorder-5.0.7/webdriver_recorder/plugin.py
+-rw-r--r--   0        0        0     4100 2023-07-21 02:20:56.087407 uw-webdriver-recorder-5.0.7/webdriver_recorder/report_exporter.py
+-rw-r--r--   0        0        0     3100 2023-07-21 02:20:56.087407 uw-webdriver-recorder-5.0.7/webdriver_recorder/templates/help.html
+-rw-r--r--   0        0        0     1924 2023-07-21 02:20:56.087407 uw-webdriver-recorder-5.0.7/webdriver_recorder/templates/modal.html
+-rw-r--r--   0        0        0     1194 2023-07-21 02:20:56.087407 uw-webdriver-recorder-5.0.7/webdriver_recorder/templates/modal_link.html
+-rw-r--r--   0        0        0     1302 2023-07-21 02:20:56.087407 uw-webdriver-recorder-5.0.7/webdriver_recorder/templates/report.html
+-rw-r--r--   0        0        0     2622 2023-07-21 02:20:56.087407 uw-webdriver-recorder-5.0.7/webdriver_recorder/templates/report_header.html
+-rw-r--r--   0        0        0     4010 2023-07-21 02:20:56.087407 uw-webdriver-recorder-5.0.7/webdriver_recorder/templates/static/report.js
+-rw-r--r--   0        0        0     3517 2023-07-21 02:20:56.087407 uw-webdriver-recorder-5.0.7/webdriver_recorder/templates/static/style.css
+-rw-r--r--   0        0        0     5542 2023-07-21 02:20:56.087407 uw-webdriver-recorder-5.0.7/webdriver_recorder/templates/test_case.html
+-rw-r--r--   0        0        0     1167 2023-07-21 02:20:56.087407 uw-webdriver-recorder-5.0.7/webdriver_recorder/templates/test_screenshots.html
+-rw-r--r--   0        0        0      542 2023-07-21 02:20:56.087407 uw-webdriver-recorder-5.0.7/webdriver_recorder/templates/toast-copied-to-clipboard.html
+-rw-r--r--   0        0        0      960 2023-07-21 02:26:25.991715 uw-webdriver-recorder-5.0.7/setup.py
+-rw-r--r--   0        0        0      790 2023-07-21 02:26:25.992017 uw-webdriver-recorder-5.0.7/PKG-INFO
```

### Comparing `uw-webdriver-recorder-5.0.6/LICENSE` & `uw-webdriver-recorder-5.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `uw-webdriver-recorder-5.0.6/pyproject.toml` & `uw-webdriver-recorder-5.0.7/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "uw-webdriver-recorder"
 # This version string is typically managed by the CI workflow,
 # and is changed anytime `poetry version [new version]` is run.
 # Do not revert this manually.
-version = "5.0.6"
+version = "5.0.7"
 description = "A pytest plugin for recording screenshots of selenium interactions, with other convenient features too."
 authors = ["Tom Thorogood <goodtom@uw.edu>"]
 license = "Apache Software License 3.0"
 classifiers = [
     "Framework :: Pytest",
     'License :: OSI Approved :: Apache Software License',
 ]
@@ -15,15 +15,15 @@
     { include = "webdriver_recorder" }
 ]
 
 [tool.poetry.plugins.pytest11]
 "uw-webdriver-recorder" = "webdriver_recorder.plugin"
 
 [tool.poetry.dependencies]
-python = ">=3.7,<3.11"
+python = "^3.8" # allow us to go >=3.8 and < 4.0
 pytest = ">=6.2.4"
 Jinja2 = "^3.0.1"
 selenium = "^4.1.0"
 pydantic = "^1.8.2"
 
 [tool.poetry.dev-dependencies]
 tox = "^3.23.1"
```

### Comparing `uw-webdriver-recorder-5.0.6/webdriver_recorder/browser.py` & `uw-webdriver-recorder-5.0.7/webdriver_recorder/browser.py`

 * *Files identical despite different names*

### Comparing `uw-webdriver-recorder-5.0.6/webdriver_recorder/export-report.py` & `uw-webdriver-recorder-5.0.7/webdriver_recorder/export-report.py`

 * *Files identical despite different names*

### Comparing `uw-webdriver-recorder-5.0.6/webdriver_recorder/models.py` & `uw-webdriver-recorder-5.0.7/webdriver_recorder/models.py`

 * *Files identical despite different names*

### Comparing `uw-webdriver-recorder-5.0.6/webdriver_recorder/plugin.py` & `uw-webdriver-recorder-5.0.7/webdriver_recorder/plugin.py`

 * *Files identical despite different names*

### Comparing `uw-webdriver-recorder-5.0.6/webdriver_recorder/report_exporter.py` & `uw-webdriver-recorder-5.0.7/webdriver_recorder/report_exporter.py`

 * *Files identical despite different names*

### Comparing `uw-webdriver-recorder-5.0.6/webdriver_recorder/templates/help.html` & `uw-webdriver-recorder-5.0.7/webdriver_recorder/templates/help.html`

 * *Files identical despite different names*

### Comparing `uw-webdriver-recorder-5.0.6/webdriver_recorder/templates/modal.html` & `uw-webdriver-recorder-5.0.7/webdriver_recorder/templates/modal.html`

 * *Files identical despite different names*

### Comparing `uw-webdriver-recorder-5.0.6/webdriver_recorder/templates/modal_link.html` & `uw-webdriver-recorder-5.0.7/webdriver_recorder/templates/modal_link.html`

 * *Files identical despite different names*

### Comparing `uw-webdriver-recorder-5.0.6/webdriver_recorder/templates/report.html` & `uw-webdriver-recorder-5.0.7/webdriver_recorder/templates/report.html`

 * *Files identical despite different names*

### Comparing `uw-webdriver-recorder-5.0.6/webdriver_recorder/templates/report_header.html` & `uw-webdriver-recorder-5.0.7/webdriver_recorder/templates/report_header.html`

 * *Files identical despite different names*

### Comparing `uw-webdriver-recorder-5.0.6/webdriver_recorder/templates/static/report.js` & `uw-webdriver-recorder-5.0.7/webdriver_recorder/templates/static/report.js`

 * *Files identical despite different names*

### Comparing `uw-webdriver-recorder-5.0.6/webdriver_recorder/templates/static/style.css` & `uw-webdriver-recorder-5.0.7/webdriver_recorder/templates/static/style.css`

 * *Files identical despite different names*

### Comparing `uw-webdriver-recorder-5.0.6/webdriver_recorder/templates/test_case.html` & `uw-webdriver-recorder-5.0.7/webdriver_recorder/templates/test_case.html`

 * *Files identical despite different names*

### Comparing `uw-webdriver-recorder-5.0.6/webdriver_recorder/templates/test_screenshots.html` & `uw-webdriver-recorder-5.0.7/webdriver_recorder/templates/test_screenshots.html`

 * *Files identical despite different names*

### Comparing `uw-webdriver-recorder-5.0.6/webdriver_recorder/templates/toast-copied-to-clipboard.html` & `uw-webdriver-recorder-5.0.7/webdriver_recorder/templates/toast-copied-to-clipboard.html`

 * *Files identical despite different names*

### Comparing `uw-webdriver-recorder-5.0.6/setup.py` & `uw-webdriver-recorder-5.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,24 +14,24 @@
  'selenium>=4.1.0,<5.0.0']
 
 entry_points = \
 {'pytest11': ['uw-webdriver-recorder = webdriver_recorder.plugin']}
 
 setup_kwargs = {
     'name': 'uw-webdriver-recorder',
-    'version': '5.0.6',
+    'version': '5.0.7',
     'description': 'A pytest plugin for recording screenshots of selenium interactions, with other convenient features too.',
     'long_description': None,
     'author': 'Tom Thorogood',
     'author_email': 'goodtom@uw.edu',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
-    'python_requires': '>=3.7,<3.11',
+    'python_requires': '>=3.8,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `uw-webdriver-recorder-5.0.6/PKG-INFO` & `uw-webdriver-recorder-5.0.7/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: uw-webdriver-recorder
-Version: 5.0.6
+Version: 5.0.7
 Summary: A pytest plugin for recording screenshots of selenium interactions, with other convenient features too.
 License: Apache Software License 3.0
 Author: Tom Thorogood
 Author-email: goodtom@uw.edu
-Requires-Python: >=3.7,<3.11
+Requires-Python: >=3.8,<4.0
 Classifier: Framework :: Pytest
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: Jinja2 (>=3.0.1,<4.0.0)
 Requires-Dist: pydantic (>=1.8.2,<2.0.0)
 Requires-Dist: pytest (>=6.2.4)
 Requires-Dist: selenium (>=4.1.0,<5.0.0)
```

