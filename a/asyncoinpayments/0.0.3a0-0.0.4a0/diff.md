# Comparing `tmp/asyncoinpayments-0.0.3a0.tar.gz` & `tmp/asyncoinpayments-0.0.4a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asyncoinpayments-0.0.3a0.tar", last modified: Thu Jul 20 22:13:59 2023, max compression
+gzip compressed data, was "asyncoinpayments-0.0.4a0.tar", last modified: Fri Jul 21 09:16:55 2023, max compression
```

## Comparing `asyncoinpayments-0.0.3a0.tar` & `asyncoinpayments-0.0.4a0.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxr-x   0 flalugli  (1000) flalugli  (1000)        0 2023-07-20 22:13:59.016072 asyncoinpayments-0.0.3a0/
--rw-rw-r--   0 flalugli  (1000) flalugli  (1000)       72 2023-07-20 22:07:25.000000 asyncoinpayments-0.0.3a0/.gitignore
--rw-rw-r--   0 flalugli  (1000) flalugli  (1000)    11328 2023-07-08 21:40:35.000000 asyncoinpayments-0.0.3a0/LICENSE.txt
--rw-rw-r--   0 flalugli  (1000) flalugli  (1000)      928 2023-07-20 22:13:59.016072 asyncoinpayments-0.0.3a0/PKG-INFO
--rw-rw-r--   0 flalugli  (1000) flalugli  (1000)      432 2023-07-08 20:18:04.000000 asyncoinpayments-0.0.3a0/README.md
-drwxrwxr-x   0 flalugli  (1000) flalugli  (1000)        0 2023-07-20 22:13:59.016072 asyncoinpayments-0.0.3a0/asyncoinpayments/
--rw-rw-r--   0 flalugli  (1000) flalugli  (1000)       92 2023-07-18 17:18:09.000000 asyncoinpayments-0.0.3a0/asyncoinpayments/__init__.py
-drwxrwxr-x   0 flalugli  (1000) flalugli  (1000)        0 2023-07-20 22:13:59.016072 asyncoinpayments-0.0.3a0/asyncoinpayments/asyncoinpayments.egg-info/
--rw-rw-r--   0 flalugli  (1000) flalugli  (1000)      928 2023-07-20 22:13:58.000000 asyncoinpayments-0.0.3a0/asyncoinpayments/asyncoinpayments.egg-info/PKG-INFO
--rw-rw-r--   0 flalugli  (1000) flalugli  (1000)      455 2023-07-20 22:13:59.000000 asyncoinpayments-0.0.3a0/asyncoinpayments/asyncoinpayments.egg-info/SOURCES.txt
--rw-rw-r--   0 flalugli  (1000) flalugli  (1000)        1 2023-07-20 22:13:58.000000 asyncoinpayments-0.0.3a0/asyncoinpayments/asyncoinpayments.egg-info/dependency_links.txt
--rw-rw-r--   0 flalugli  (1000) flalugli  (1000)       17 2023-07-20 22:13:58.000000 asyncoinpayments-0.0.3a0/asyncoinpayments/asyncoinpayments.egg-info/requires.txt
--rw-rw-r--   0 flalugli  (1000) flalugli  (1000)        1 2023-07-20 22:13:58.000000 asyncoinpayments-0.0.3a0/asyncoinpayments/asyncoinpayments.egg-info/top_level.txt
--rw-rw-r--   0 flalugli  (1000) flalugli  (1000)    21181 2023-07-20 21:49:59.000000 asyncoinpayments-0.0.3a0/asyncoinpayments/coinpayments.py
--rw-rw-r--   0 flalugli  (1000) flalugli  (1000)      155 2023-07-08 15:55:02.000000 asyncoinpayments-0.0.3a0/asyncoinpayments/errors.py
--rw-rw-r--   0 flalugli  (1000) flalugli  (1000)      647 2023-07-20 21:10:50.000000 asyncoinpayments-0.0.3a0/asyncoinpayments/utils.py
--rw-rw-r--   0 flalugli  (1000) flalugli  (1000)      711 2023-07-20 22:08:43.000000 asyncoinpayments-0.0.3a0/pyproject.toml
--rw-rw-r--   0 flalugli  (1000) flalugli  (1000)       38 2023-07-20 22:13:59.016072 asyncoinpayments-0.0.3a0/setup.cfg
--rw-rw-r--   0 flalugli  (1000) flalugli  (1000)       68 2023-07-20 21:25:48.000000 asyncoinpayments-0.0.3a0/setup.py
+drwxrwxr-x   0 flalugli  (1000) flalugli  (1000)        0 2023-07-21 09:16:55.688109 asyncoinpayments-0.0.4a0/
+-rw-rw-r--   0 flalugli  (1000) flalugli  (1000)       58 2023-07-21 09:11:52.000000 asyncoinpayments-0.0.4a0/.gitignore
+-rw-rw-r--   0 flalugli  (1000) flalugli  (1000)    11328 2023-07-08 21:40:35.000000 asyncoinpayments-0.0.4a0/LICENSE.txt
+-rw-rw-r--   0 flalugli  (1000) flalugli  (1000)     1044 2023-07-21 09:16:55.688109 asyncoinpayments-0.0.4a0/PKG-INFO
+-rw-rw-r--   0 flalugli  (1000) flalugli  (1000)      432 2023-07-08 20:18:04.000000 asyncoinpayments-0.0.4a0/README.md
+-rw-rw-r--   0 flalugli  (1000) flalugli  (1000)      842 2023-07-21 09:16:38.000000 asyncoinpayments-0.0.4a0/pyproject.toml
+-rw-rw-r--   0 flalugli  (1000) flalugli  (1000)       38 2023-07-21 09:16:55.688109 asyncoinpayments-0.0.4a0/setup.cfg
+-rw-rw-r--   0 flalugli  (1000) flalugli  (1000)       68 2023-07-20 21:25:48.000000 asyncoinpayments-0.0.4a0/setup.py
+drwxrwxr-x   0 flalugli  (1000) flalugli  (1000)        0 2023-07-21 09:16:55.684110 asyncoinpayments-0.0.4a0/src/
+drwxrwxr-x   0 flalugli  (1000) flalugli  (1000)        0 2023-07-21 09:16:55.688109 asyncoinpayments-0.0.4a0/src/asyncoinpayments/
+-rw-rw-r--   0 flalugli  (1000) flalugli  (1000)       92 2023-07-18 17:18:09.000000 asyncoinpayments-0.0.4a0/src/asyncoinpayments/__init__.py
+-rw-rw-r--   0 flalugli  (1000) flalugli  (1000)    21181 2023-07-20 21:49:59.000000 asyncoinpayments-0.0.4a0/src/asyncoinpayments/coinpayments.py
+-rw-rw-r--   0 flalugli  (1000) flalugli  (1000)      155 2023-07-08 15:55:02.000000 asyncoinpayments-0.0.4a0/src/asyncoinpayments/errors.py
+-rw-rw-r--   0 flalugli  (1000) flalugli  (1000)      647 2023-07-20 21:10:50.000000 asyncoinpayments-0.0.4a0/src/asyncoinpayments/utils.py
+drwxrwxr-x   0 flalugli  (1000) flalugli  (1000)        0 2023-07-21 09:16:55.688109 asyncoinpayments-0.0.4a0/src/asyncoinpayments.egg-info/
+-rw-rw-r--   0 flalugli  (1000) flalugli  (1000)     1044 2023-07-21 09:16:55.000000 asyncoinpayments-0.0.4a0/src/asyncoinpayments.egg-info/PKG-INFO
+-rw-rw-r--   0 flalugli  (1000) flalugli  (1000)      406 2023-07-21 09:16:55.000000 asyncoinpayments-0.0.4a0/src/asyncoinpayments.egg-info/SOURCES.txt
+-rw-rw-r--   0 flalugli  (1000) flalugli  (1000)        1 2023-07-21 09:16:55.000000 asyncoinpayments-0.0.4a0/src/asyncoinpayments.egg-info/dependency_links.txt
+-rw-rw-r--   0 flalugli  (1000) flalugli  (1000)       17 2023-07-21 09:16:55.000000 asyncoinpayments-0.0.4a0/src/asyncoinpayments.egg-info/requires.txt
+-rw-rw-r--   0 flalugli  (1000) flalugli  (1000)       17 2023-07-21 09:16:55.000000 asyncoinpayments-0.0.4a0/src/asyncoinpayments.egg-info/top_level.txt
```

### Comparing `asyncoinpayments-0.0.3a0/LICENSE.txt` & `asyncoinpayments-0.0.4a0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `asyncoinpayments-0.0.3a0/PKG-INFO` & `asyncoinpayments-0.0.4a0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 Metadata-Version: 2.1
 Name: asyncoinpayments
-Version: 0.0.3a0
+Version: 0.0.4a0
 Summary: Python Asynchronous Wrapper of the CoinPayments API
+Author-email: flalugli <flalugli.dev@gmail.com>
 License: Apache License 2.0
+Project-URL: Homepage, https://github.com/flalugli/asyncoinpayments
 Keywords: python,crypto,cryptocurrency,payment gateway,async,aiohttp
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `asyncoinpayments-0.0.3a0/asyncoinpayments/asyncoinpayments.egg-info/PKG-INFO` & `asyncoinpayments-0.0.4a0/src/asyncoinpayments.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 Metadata-Version: 2.1
 Name: asyncoinpayments
-Version: 0.0.3a0
+Version: 0.0.4a0
 Summary: Python Asynchronous Wrapper of the CoinPayments API
+Author-email: flalugli <flalugli.dev@gmail.com>
 License: Apache License 2.0
+Project-URL: Homepage, https://github.com/flalugli/asyncoinpayments
 Keywords: python,crypto,cryptocurrency,payment gateway,async,aiohttp
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `asyncoinpayments-0.0.3a0/asyncoinpayments/coinpayments.py` & `asyncoinpayments-0.0.4a0/src/asyncoinpayments/coinpayments.py`

 * *Files identical despite different names*

### Comparing `asyncoinpayments-0.0.3a0/asyncoinpayments/utils.py` & `asyncoinpayments-0.0.4a0/src/asyncoinpayments/utils.py`

 * *Files identical despite different names*

### Comparing `asyncoinpayments-0.0.3a0/pyproject.toml` & `asyncoinpayments-0.0.4a0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,31 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "asyncoinpayments"
-version = "0.0.3a"
+version = "0.0.4a"
 description = "Python Asynchronous Wrapper of the CoinPayments API"
+authors = [
+  { name="flalugli", email="flalugli.dev@gmail.com" },
+]
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = ['python', 'crypto', 'cryptocurrency', 'payment gateway', 'async', 'aiohttp']
 license = {text = "Apache License 2.0"}
 classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
     ]
 dependencies = [
     "aiohttp",
     "tenacity",
 ]
+
+[project.urls]
+Homepage = "https://github.com/flalugli/asyncoinpayments"
+
 [tool.setuptools.packages.find]
-where = ["asyncoinpayments"]
+where = ["src"]
```

