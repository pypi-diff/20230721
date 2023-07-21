# Comparing `tmp/confluentfucci-0.0.17.tar.gz` & `tmp/confluentfucci-0.0.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "confluentfucci-0.0.17.tar", max compression
+gzip compressed data, was "confluentfucci-0.0.18.tar", max compression
```

## Comparing `confluentfucci-0.0.17.tar` & `confluentfucci-0.0.18.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1061 2023-07-10 21:28:11.234752 confluentfucci-0.0.17/LICENSE.txt
--rw-r--r--   0        0        0     1617 2023-07-10 21:28:11.234752 confluentfucci-0.0.17/README.md
--rw-r--r--   0        0        0      351 2023-07-10 21:28:11.234752 confluentfucci-0.0.17/confluentfucci/__init__.py
--rw-r--r--   0        0        0    22573 2023-07-10 21:28:11.234752 confluentfucci-0.0.17/confluentfucci/gui.py
--rw-r--r--   0        0        0    22441 2023-07-10 21:28:11.234752 confluentfucci-0.0.17/confluentfucci/math.py
--rw-r--r--   0        0        0     3909 2023-07-10 21:28:11.234752 confluentfucci-0.0.17/confluentfucci/utils.py
--rw-r--r--   0        0        0     4793 2023-07-10 21:31:42.521841 confluentfucci-0.0.17/pyproject.toml
--rw-r--r--   0        0        0     2695 1970-01-01 00:00:00.000000 confluentfucci-0.0.17/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-07-21 16:28:40.806139 confluentfucci-0.0.18/LICENSE.txt
+-rw-r--r--   0        0        0     1617 2023-07-21 16:28:40.806139 confluentfucci-0.0.18/README.md
+-rw-r--r--   0        0        0      351 2023-07-21 16:28:40.806139 confluentfucci-0.0.18/confluentfucci/__init__.py
+-rw-r--r--   0        0        0    22575 2023-07-21 16:28:40.806139 confluentfucci-0.0.18/confluentfucci/gui.py
+-rw-r--r--   0        0        0    22441 2023-07-21 16:28:40.806139 confluentfucci-0.0.18/confluentfucci/math.py
+-rw-r--r--   0        0        0     3909 2023-07-21 16:28:40.806139 confluentfucci-0.0.18/confluentfucci/utils.py
+-rw-r--r--   0        0        0     4793 2023-07-21 16:31:47.221152 confluentfucci-0.0.18/pyproject.toml
+-rw-r--r--   0        0        0     2695 1970-01-01 00:00:00.000000 confluentfucci-0.0.18/PKG-INFO
```

### Comparing `confluentfucci-0.0.17/LICENSE.txt` & `confluentfucci-0.0.18/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `confluentfucci-0.0.17/README.md` & `confluentfucci-0.0.18/README.md`

 * *Files identical despite different names*

### Comparing `confluentfucci-0.0.17/confluentfucci/gui.py` & `confluentfucci-0.0.18/confluentfucci/gui.py`

 * *Files 0% similar despite different names*

```diff
@@ -507,15 +507,15 @@
             )
         )
 
         return sidebar
 
     def get_template(self):
         template = pn.template.BootstrapTemplate(
-            title="PyFucciTrack",
+            title="ConfluentFUCCI",
             theme_toggle=False,
             sidebar=[self.sidebar],
             main=self.main,
         )
 
         return template
```

### Comparing `confluentfucci-0.0.17/confluentfucci/math.py` & `confluentfucci-0.0.18/confluentfucci/math.py`

 * *Files identical despite different names*

### Comparing `confluentfucci-0.0.17/confluentfucci/utils.py` & `confluentfucci-0.0.18/confluentfucci/utils.py`

 * *Files identical despite different names*

### Comparing `confluentfucci-0.0.17/pyproject.toml` & `confluentfucci-0.0.18/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ConfluentFUCCI"
-version = "0.0.17"
+version = "0.0.18"
 description = ""
 authors = ["Leo Goldstien <leogoldstien@gmail.com>"]
 readme = "README.md"
 packages = [{include = "confluentfucci"}]
 
 [tool.poetry.dependencies]
 loguru = "^0.7.0"
```

### Comparing `confluentfucci-0.0.17/PKG-INFO` & `confluentfucci-0.0.18/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: confluentfucci
-Version: 0.0.17
+Version: 0.0.18
 Summary: 
 Author: Leo Goldstien
 Author-email: leogoldstien@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

