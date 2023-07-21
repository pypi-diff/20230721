# Comparing `tmp/ninjakiwi_api-0.0.6.tar.gz` & `tmp/ninjakiwi_api-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ninjakiwi_api-0.0.6.tar", max compression
+gzip compressed data, was "ninjakiwi_api-0.0.7.tar", max compression
```

## Comparing `ninjakiwi_api-0.0.6.tar` & `ninjakiwi_api-0.0.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1072 2023-07-19 16:03:17.395151 ninjakiwi_api-0.0.6/LICENSE
--rw-r--r--   0        0        0      820 2023-07-20 12:50:41.021503 ninjakiwi_api-0.0.6/README.md
--rw-r--r--   0        0        0       84 2023-07-20 11:13:18.959090 ninjakiwi_api-0.0.6/ninjakiwi_api/API/BTD6/__init__.py
--rw-r--r--   0        0        0     3002 2023-07-20 11:13:18.975757 ninjakiwi_api-0.0.6/ninjakiwi_api/API/BTD6/function.py
--rw-r--r--   0        0        0       85 2023-07-20 11:13:18.942423 ninjakiwi_api-0.0.6/ninjakiwi_api/API/BTDB2/__init__.py
--rw-r--r--   0        0        0     1085 2023-07-20 11:13:18.939090 ninjakiwi_api-0.0.6/ninjakiwi_api/API/BTDB2/function.py
--rw-r--r--   0        0        0      184 2023-07-20 11:13:18.949090 ninjakiwi_api-0.0.6/ninjakiwi_api/API/__init__.py
--rw-r--r--   0        0        0      116 2023-07-20 11:38:30.257333 ninjakiwi_api-0.0.6/ninjakiwi_api/FUNCTIONS/ERROR/__init__.py
--rw-r--r--   0        0        0     1807 2023-07-20 10:44:10.487649 ninjakiwi_api-0.0.6/ninjakiwi_api/FUNCTIONS/ERROR/function.py
--rw-r--r--   0        0        0      108 2023-07-20 11:38:30.260666 ninjakiwi_api-0.0.6/ninjakiwi_api/FUNCTIONS/FETCH/__init__.py
--rw-r--r--   0        0        0      746 2023-07-20 11:43:09.057477 ninjakiwi_api-0.0.6/ninjakiwi_api/FUNCTIONS/FETCH/function.py
--rw-r--r--   0        0        0      869 2023-07-20 12:39:11.245148 ninjakiwi_api-0.0.6/ninjakiwi_api/FUNCTIONS/FETCH/model.py
--rw-r--r--   0        0        0      157 2023-07-20 11:38:30.267333 ninjakiwi_api-0.0.6/ninjakiwi_api/FUNCTIONS/__init__.py
--rw-r--r--   0        0        0      185 2023-07-20 11:13:18.952423 ninjakiwi_api-0.0.6/ninjakiwi_api/__init__.py
--rw-r--r--   0        0        0     3109 2023-07-20 12:43:41.544888 ninjakiwi_api-0.0.6/ninjakiwi_api/main.py
--rw-r--r--   0        0        0     2756 2023-07-20 12:43:41.554888 ninjakiwi_api-0.0.6/pyproject.toml
--rw-r--r--   0        0        0       43 2023-07-19 16:03:17.421818 ninjakiwi_api-0.0.6/tests/__init__.py
--rw-r--r--   0        0        0      806 2023-07-20 12:39:33.825683 ninjakiwi_api-0.0.6/tests/test_main.py
--rw-r--r--   0        0        0     2975 1970-01-01 00:00:00.000000 ninjakiwi_api-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-07-19 16:03:17.395151 ninjakiwi_api-0.0.7/LICENSE
+-rw-r--r--   0        0        0      825 2023-07-20 12:55:39.295946 ninjakiwi_api-0.0.7/README.md
+-rw-r--r--   0        0        0       84 2023-07-20 11:13:18.959090 ninjakiwi_api-0.0.7/ninjakiwi_api/API/BTD6/__init__.py
+-rw-r--r--   0        0        0     3002 2023-07-20 11:13:18.975757 ninjakiwi_api-0.0.7/ninjakiwi_api/API/BTD6/function.py
+-rw-r--r--   0        0        0       85 2023-07-20 11:13:18.942423 ninjakiwi_api-0.0.7/ninjakiwi_api/API/BTDB2/__init__.py
+-rw-r--r--   0        0        0     1085 2023-07-20 11:13:18.939090 ninjakiwi_api-0.0.7/ninjakiwi_api/API/BTDB2/function.py
+-rw-r--r--   0        0        0      184 2023-07-20 11:13:18.949090 ninjakiwi_api-0.0.7/ninjakiwi_api/API/__init__.py
+-rw-r--r--   0        0        0      116 2023-07-20 11:38:30.257333 ninjakiwi_api-0.0.7/ninjakiwi_api/FUNCTIONS/ERROR/__init__.py
+-rw-r--r--   0        0        0     1807 2023-07-20 10:44:10.487649 ninjakiwi_api-0.0.7/ninjakiwi_api/FUNCTIONS/ERROR/function.py
+-rw-r--r--   0        0        0      108 2023-07-20 11:38:30.260666 ninjakiwi_api-0.0.7/ninjakiwi_api/FUNCTIONS/FETCH/__init__.py
+-rw-r--r--   0        0        0      746 2023-07-20 11:43:09.057477 ninjakiwi_api-0.0.7/ninjakiwi_api/FUNCTIONS/FETCH/function.py
+-rw-r--r--   0        0        0     1985 2023-07-20 13:13:15.256860 ninjakiwi_api-0.0.7/ninjakiwi_api/FUNCTIONS/FETCH/model.py
+-rw-r--r--   0        0        0      157 2023-07-20 11:38:30.267333 ninjakiwi_api-0.0.7/ninjakiwi_api/FUNCTIONS/__init__.py
+-rw-r--r--   0        0        0      185 2023-07-20 11:13:18.952423 ninjakiwi_api-0.0.7/ninjakiwi_api/__init__.py
+-rw-r--r--   0        0        0     3109 2023-07-20 12:43:41.544888 ninjakiwi_api-0.0.7/ninjakiwi_api/main.py
+-rw-r--r--   0        0        0     2158 2023-07-20 13:00:29.983891 ninjakiwi_api-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0       43 2023-07-19 16:03:17.421818 ninjakiwi_api-0.0.7/tests/__init__.py
+-rw-r--r--   0        0        0      806 2023-07-20 12:39:33.825683 ninjakiwi_api-0.0.7/tests/test_main.py
+-rw-r--r--   0        0        0     2516 1970-01-01 00:00:00.000000 ninjakiwi_api-0.0.7/PKG-INFO
```

### Comparing `ninjakiwi_api-0.0.6/LICENSE` & `ninjakiwi_api-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ninjakiwi_api-0.0.6/README.md` & `ninjakiwi_api-0.0.7/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -43,7 +43,9 @@
 if __name__ == "__main__":
     main()
 ```
 
 # Coming soon...
 
 Stay tuned guys
+
+---
```

### Comparing `ninjakiwi_api-0.0.6/ninjakiwi_api/API/BTD6/function.py` & `ninjakiwi_api-0.0.7/ninjakiwi_api/API/BTD6/function.py`

 * *Files identical despite different names*

### Comparing `ninjakiwi_api-0.0.6/ninjakiwi_api/API/BTDB2/function.py` & `ninjakiwi_api-0.0.7/ninjakiwi_api/API/BTDB2/function.py`

 * *Files identical despite different names*

### Comparing `ninjakiwi_api-0.0.6/ninjakiwi_api/FUNCTIONS/ERROR/function.py` & `ninjakiwi_api-0.0.7/ninjakiwi_api/FUNCTIONS/ERROR/function.py`

 * *Files identical despite different names*

### Comparing `ninjakiwi_api-0.0.6/ninjakiwi_api/FUNCTIONS/FETCH/function.py` & `ninjakiwi_api-0.0.7/ninjakiwi_api/FUNCTIONS/FETCH/function.py`

 * *Files identical despite different names*

### Comparing `ninjakiwi_api-0.0.6/ninjakiwi_api/main.py` & `ninjakiwi_api-0.0.7/ninjakiwi_api/main.py`

 * *Files identical despite different names*

### Comparing `ninjakiwi_api-0.0.6/pyproject.toml` & `ninjakiwi_api-0.0.7/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "ninjakiwi_api"
-version = "0.0.6"
+version = "0.0.7"
 homepage = "https://github.com/GustavoSchip/ninjakiwi_api"
 description = "NinjaKiwi API (OpenDATA) for Python! (My first library)"
 authors = [
     "Gustavo Schip <gustavoschip@proton.me>",
 ]
 maintainers = [
     "Gustavo Schip <gustavoschip@proton.me>",
@@ -39,26 +39,19 @@
 flake8-docstrings = { version = "^1.6.0", optional = true }
 pytest  = { version = "^7.0.1", optional = true}
 pytest-asyncio  = {version = "^0.21.1", optional = true}
 pytest-cov  = { version = "^3.0.0", optional = true}
 tox  = { version = "^3.24.5", optional = true}
 virtualenv  = { version = "^20.13.1", optional = true}
 pip  = { version = "^22.0.3"}
-mkdocs  = { version = "^1.2.3", optional = true}
-mkdocs-include-markdown-plugin  = { version = "^3.2.3", optional = true}
-mkdocs-material  = { version = "^8.1.11", optional = true}
-mkdocstrings  = { version = "^0.18.0", optional = true}
-mkdocs-material-extensions  = { version = "^1.0.3", optional = true}
 twine  = { version = "^3.8.0", optional = true}
-mkdocs-autorefs = {version = "^0.3.1", optional = true}
 pre-commit = {version = "^2.17.0", optional = true}
 toml = {version = "^0.10.2", optional = true}
 livereload = {version = "^2.6.3", optional = true}
 pyreadline = {version = "^2.1", optional = true}
-mike = { version="^1.1.2", optional=true}
 tornado = {version = "^6.2", optional = true}
 
 [tool.poetry.extras]
 test = [
     "pytest",
     "black",
     "isort",
@@ -66,27 +59,14 @@
     "flake8-docstrings",
     "pytest-cov",
     "pytest-asyncio"
     ]
 
 dev = ["tox", "pre-commit", "virtualenv", "pip", "twine", "toml"]
 
-doc = [
-    "pkginfo",
-    "mkdocs",
-    "mkdocs-include-markdown-plugin",
-    "mkdocs-material",
-    "mkdocstrings",
-    "mkdocs-material-extension",
-    "mkdocs-autorefs",
-    "mike"
-    ]
-
-
-
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 88
 include = '\.pyi?$'
```

### Comparing `ninjakiwi_api-0.0.6/tests/test_main.py` & `ninjakiwi_api-0.0.7/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `ninjakiwi_api-0.0.6/PKG-INFO` & `ninjakiwi_api-0.0.7/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ninjakiwi-api
-Version: 0.0.6
+Version: 0.0.7
 Summary: NinjaKiwi API (OpenDATA) for Python! (My first library)
 Home-page: https://github.com/GustavoSchip/ninjakiwi_api
 License: MIT
 Keywords: NinjaKiwi,API
 Author: Gustavo Schip
 Author-email: gustavoschip@proton.me
 Maintainer: Gustavo Schip
@@ -13,30 +13,22 @@
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: dev
-Provides-Extra: doc
 Provides-Extra: test
 Requires-Dist: aiohttp (>=3.8.1,<4.0.0)
 Requires-Dist: asyncio (>=3.4.3,<4.0.0)
 Requires-Dist: black (>=22.3.0,<23.0.0) ; extra == "test"
 Requires-Dist: flake8 (==4.0.1) ; extra == "test"
 Requires-Dist: flake8-docstrings (>=1.6.0,<2.0.0) ; extra == "test"
 Requires-Dist: isort (==5.10.1) ; extra == "test"
 Requires-Dist: livereload (>=2.6.3,<3.0.0)
-Requires-Dist: mike (>=1.1.2,<2.0.0) ; extra == "doc"
-Requires-Dist: mkdocs (>=1.2.3,<2.0.0) ; extra == "doc"
-Requires-Dist: mkdocs-autorefs (>=0.3.1,<0.4.0) ; extra == "doc"
-Requires-Dist: mkdocs-include-markdown-plugin (>=3.2.3,<4.0.0) ; extra == "doc"
-Requires-Dist: mkdocs-material (>=8.1.11,<9.0.0) ; extra == "doc"
-Requires-Dist: mkdocs-material-extensions (>=1.0.3,<2.0.0)
-Requires-Dist: mkdocstrings (>=0.18.0,<0.19.0) ; extra == "doc"
 Requires-Dist: pip (>=22.0.3,<23.0.0) ; extra == "dev"
 Requires-Dist: pre-commit (>=2.17.0,<3.0.0) ; extra == "dev"
 Requires-Dist: pyreadline (>=2.1,<3.0)
 Requires-Dist: pytest (>=7.0.1,<8.0.0) ; extra == "test"
 Requires-Dist: pytest-asyncio (>=0.21.1,<0.22.0) ; extra == "test"
 Requires-Dist: pytest-cov (>=3.0.0,<4.0.0) ; extra == "test"
 Requires-Dist: toml (>=0.10.2,<0.11.0) ; extra == "dev"
@@ -92,7 +84,9 @@
     main()
 ```
 
 # Coming soon...
 
 Stay tuned guys
 
+---
+
```

