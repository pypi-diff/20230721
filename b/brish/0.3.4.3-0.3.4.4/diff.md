# Comparing `tmp/brish-0.3.4.3.tar.gz` & `tmp/brish-0.3.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brish-0.3.4.3.tar", max compression
+gzip compressed data, was "brish-0.3.4.4.tar", max compression
```

## Comparing `brish-0.3.4.3.tar` & `brish-0.3.4.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      425 2022-02-21 15:40:02.031680 brish-0.3.4.3/brish/__init__.py
--rw-r--r--   0        0        0      628 2021-04-08 07:27:38.876019 brish-0.3.4.3/brish/__main__.py
--rwxr-xr-x   0        0        0      569 2021-03-26 13:13:59.311397 brish-0.3.4.3/brish/brish.zsh
--rwxr-xr-x   0        0        0     1682 2023-03-03 11:28:06.010722 brish-0.3.4.3/brish/brish2.zsh
--rw-r--r--   0        0        0    18775 2023-03-03 11:18:20.926713 brish-0.3.4.3/brish/brishmod.py
--rw-r--r--   0        0        0      800 2021-10-08 15:56:49.633228 brish-0.3.4.3/brish/brishz.py
--rw-r--r--   0        0        0      523 2023-03-03 11:28:53.354744 brish-0.3.4.3/pyproject.toml
--rw-r--r--   0        0        0      676 1970-01-01 00:00:00.000000 brish-0.3.4.3/setup.py
--rw-r--r--   0        0        0      651 1970-01-01 00:00:00.000000 brish-0.3.4.3/PKG-INFO
+-rw-r--r--   0        0        0      425 2022-02-21 15:40:02.031680 brish-0.3.4.4/brish/__init__.py
+-rw-r--r--   0        0        0      628 2021-04-08 07:27:38.876019 brish-0.3.4.4/brish/__main__.py
+-rwxr-xr-x   0        0        0      569 2021-03-26 13:13:59.311397 brish-0.3.4.4/brish/brish.zsh
+-rwxr-xr-x   0        0        0     1682 2023-03-03 11:28:06.010722 brish-0.3.4.4/brish/brish2.zsh
+-rw-r--r--   0        0        0    18786 2023-07-21 01:11:52.528138 brish-0.3.4.4/brish/brishmod.py
+-rw-r--r--   0        0        0      800 2021-10-08 15:56:49.633228 brish-0.3.4.4/brish/brishz.py
+-rw-r--r--   0        0        0      523 2023-07-21 01:13:08.694391 brish-0.3.4.4/pyproject.toml
+-rw-r--r--   0        0        0      676 1970-01-01 00:00:00.000000 brish-0.3.4.4/setup.py
+-rw-r--r--   0        0        0      651 1970-01-01 00:00:00.000000 brish-0.3.4.4/PKG-INFO
```

### Comparing `brish-0.3.4.3/brish/__main__.py` & `brish-0.3.4.4/brish/__main__.py`

 * *Files identical despite different names*

### Comparing `brish-0.3.4.3/brish/brish.zsh` & `brish-0.3.4.4/brish/brish.zsh`

 * *Files identical despite different names*

### Comparing `brish-0.3.4.3/brish/brish2.zsh` & `brish-0.3.4.4/brish/brish2.zsh`

 * *Files identical despite different names*

### Comparing `brish-0.3.4.3/brish/brishmod.py` & `brish-0.3.4.4/brish/brishmod.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 def boolsh(some_bool):
     if some_bool:
         return "y"
     else:
         return ""
 
 def bool_from_str(some_bool):
-    if some_bool in ("", "n", "no", "N", "NO"):
+    if some_bool.lower() in ("", "0", "n", "no", "false"):
         return False
     else:
         return bool(some_bool)
 
 
 class NonzeroBrishException(Exception):
     pass
```

### Comparing `brish-0.3.4.3/brish/brishz.py` & `brish-0.3.4.4/brish/brishz.py`

 * *Files identical despite different names*

### Comparing `brish-0.3.4.3/pyproject.toml` & `brish-0.3.4.4/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "brish"
-version = "0.3.4.3"
+version = "0.3.4.4"
 description = "A bridge between zsh and Python."
 authors = ["NightMachinary <rudiwillalwaysloveyou@gmail.com>"]
 repository = "https://github.com/NightMachinary/brish"
 exclude = ["__pycache__"]
 
 [tool.poetry.dependencies]
 python = "==3.*,>=3.7.0"
```

### Comparing `brish-0.3.4.3/setup.py` & `brish-0.3.4.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['icecream>=2.1.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'brish',
-    'version': '0.3.4.3',
+    'version': '0.3.4.4',
     'description': 'A bridge between zsh and Python.',
     'long_description': 'None',
     'author': 'NightMachinary',
     'author_email': 'rudiwillalwaysloveyou@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/NightMachinary/brish',
```

### Comparing `brish-0.3.4.3/PKG-INFO` & `brish-0.3.4.4/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brish
-Version: 0.3.4.3
+Version: 0.3.4.4
 Summary: A bridge between zsh and Python.
 Home-page: https://github.com/NightMachinary/brish
 Author: NightMachinary
 Author-email: rudiwillalwaysloveyou@gmail.com
 Requires-Python: >=3.7.0,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

