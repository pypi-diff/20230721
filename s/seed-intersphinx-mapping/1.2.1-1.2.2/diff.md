# Comparing `tmp/seed_intersphinx_mapping-1.2.1.tar.gz` & `tmp/seed_intersphinx_mapping-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seed_intersphinx_mapping-1.2.1.tar", last modified: Fri Apr 14 18:11:29 2023, max compression
+gzip compressed data, was "seed_intersphinx_mapping-1.2.2.tar", last modified: Fri Jul 21 08:54:27 2023, max compression
```

## Comparing `seed_intersphinx_mapping-1.2.1.tar` & `seed_intersphinx_mapping-1.2.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0 runner    (1001) docker     (122)     9702 2023-04-14 18:11:29.150884 seed_intersphinx_mapping-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     5175 2023-04-14 18:11:29.150884 seed_intersphinx_mapping-1.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)     1063 2023-04-14 18:11:29.142884 seed_intersphinx_mapping-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     7809 2023-04-14 18:11:29.150884 seed_intersphinx_mapping-1.2.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)      142 2023-04-14 18:11:29.150884 seed_intersphinx_mapping-1.2.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)     6553 2023-04-14 18:11:00.726475 seed_intersphinx_mapping-1.2.1/seed_intersphinx_mapping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-14 18:11:00.726475 seed_intersphinx_mapping-1.2.1/seed_intersphinx_mapping/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)     2960 2023-04-14 18:11:00.726475 seed_intersphinx_mapping-1.2.1/seed_intersphinx_mapping/requirements_parsers.py
--rw-r--r--   0 runner    (1001) docker     (122)     2132 2023-04-14 18:11:00.726475 seed_intersphinx_mapping-1.2.1/seed_intersphinx_mapping/fallback_mapping.json
--rw-r--r--   0 runner    (1001) docker     (122)     1583 2023-04-14 18:11:00.726475 seed_intersphinx_mapping-1.2.1/seed_intersphinx_mapping/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1318 2023-04-14 18:11:00.726475 seed_intersphinx_mapping-1.2.1/seed_intersphinx_mapping/cache.py
--rw-r--r--   0 runner    (1001) docker     (122)     4724 2023-04-14 18:11:00.726475 seed_intersphinx_mapping-1.2.1/seed_intersphinx_mapping/extension.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1063 2023-07-21 08:54:27.606316 seed_intersphinx_mapping-1.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      142 2023-07-21 08:54:27.614317 seed_intersphinx_mapping-1.2.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     7809 2023-07-21 08:54:27.614317 seed_intersphinx_mapping-1.2.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     9753 2023-07-21 08:54:27.614317 seed_intersphinx_mapping-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5229 2023-07-21 08:54:27.614317 seed_intersphinx_mapping-1.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)     1318 2023-07-21 08:53:49.006005 seed_intersphinx_mapping-1.2.2/seed_intersphinx_mapping/cache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6553 2023-07-21 08:53:49.006005 seed_intersphinx_mapping-1.2.2/seed_intersphinx_mapping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2960 2023-07-21 08:53:49.006005 seed_intersphinx_mapping-1.2.2/seed_intersphinx_mapping/requirements_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-21 08:53:49.006005 seed_intersphinx_mapping-1.2.2/seed_intersphinx_mapping/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)     1583 2023-07-21 08:53:49.006005 seed_intersphinx_mapping-1.2.2/seed_intersphinx_mapping/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2182 2023-07-21 08:53:49.006005 seed_intersphinx_mapping-1.2.2/seed_intersphinx_mapping/fallback_mapping.json
+-rw-r--r--   0 runner    (1001) docker     (122)     4724 2023-07-21 08:53:49.006005 seed_intersphinx_mapping-1.2.2/seed_intersphinx_mapping/extension.py
```

### Comparing `seed_intersphinx_mapping-1.2.1/PKG-INFO` & `seed_intersphinx_mapping-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seed-intersphinx-mapping
-Version: 1.2.1
+Version: 1.2.2
 Summary: Populate the Sphinx 'intersphinx_mapping' dictionary from the project's requirements.
 Author-email: Dominic Davis-Foster <dominic@davis-foster.co.uk>
 License: MIT
 Keywords: documentation,intersphinx,sphinx
 Home-page: https://github.com/sphinx-toolbox/seed_intersphinx_mapping
 Project-URL: Issue Tracker, https://github.com/sphinx-toolbox/seed_intersphinx_mapping/issues
 Project-URL: Source Code, https://github.com/sphinx-toolbox/seed_intersphinx_mapping
@@ -20,14 +20,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Documentation
 Classifier: Topic :: Documentation :: Sphinx
 Classifier: Topic :: Software Development :: Documentation
 Classifier: Typing :: Typed
 Requires-Python: >=3.6
@@ -141,15 +142,15 @@
 .. |license| image:: https://img.shields.io/github/license/sphinx-toolbox/seed_intersphinx_mapping
 	:target: https://github.com/sphinx-toolbox/seed_intersphinx_mapping/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/sphinx-toolbox/seed_intersphinx_mapping
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/sphinx-toolbox/seed_intersphinx_mapping/v1.2.1
+.. |commits-since| image:: https://img.shields.io/github/commits-since/sphinx-toolbox/seed_intersphinx_mapping/v1.2.2
 	:target: https://github.com/sphinx-toolbox/seed_intersphinx_mapping/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/sphinx-toolbox/seed_intersphinx_mapping
 	:target: https://github.com/sphinx-toolbox/seed_intersphinx_mapping/commit/master
 	:alt: GitHub last commit
```

### Comparing `seed_intersphinx_mapping-1.2.1/pyproject.toml` & `seed_intersphinx_mapping-1.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "whey",]
 build-backend = "whey"
 
 [project]
 name = "seed_intersphinx_mapping"
-version = "1.2.1"
+version = "1.2.2"
 description = "Populate the Sphinx 'intersphinx_mapping' dictionary from the project's requirements."
 readme = "README.rst"
 keywords = [ "documentation", "intersphinx", "sphinx",]
 dynamic = []
 dependencies = [
     "apeye>=1.0.1",
     "dist-meta>=0.1.2",
@@ -24,14 +24,15 @@
     "Framework :: Sphinx :: Extension",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.6",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
     "Topic :: Documentation",
@@ -61,15 +62,15 @@
     "Framework :: Sphinx :: Extension",
     "Intended Audience :: Developers",
     "Topic :: Documentation",
     "Topic :: Documentation :: Sphinx",
     "Topic :: Software Development :: Documentation",
     "Typing :: Typed",
 ]
-python-versions = [ "3.6", "3.7", "3.8", "3.9", "3.10",]
+python-versions = [ "3.6", "3.7", "3.8", "3.9", "3.10", "3.11",]
 python-implementations = [ "CPython", "PyPy",]
 platforms = [ "Windows", "macOS", "Linux",]
 license-key = "MIT"
 additional-files = [ "include seed_intersphinx_mapping/fallback_mapping.json",]
 
 [tool.mkrecipe]
 conda-channels = [ "conda-forge", "domdfcoding",]
```

### Comparing `seed_intersphinx_mapping-1.2.1/LICENSE` & `seed_intersphinx_mapping-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `seed_intersphinx_mapping-1.2.1/README.rst` & `seed_intersphinx_mapping-1.2.2/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -97,15 +97,15 @@
 .. |license| image:: https://img.shields.io/github/license/sphinx-toolbox/seed_intersphinx_mapping
 	:target: https://github.com/sphinx-toolbox/seed_intersphinx_mapping/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/sphinx-toolbox/seed_intersphinx_mapping
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/sphinx-toolbox/seed_intersphinx_mapping/v1.2.1
+.. |commits-since| image:: https://img.shields.io/github/commits-since/sphinx-toolbox/seed_intersphinx_mapping/v1.2.2
 	:target: https://github.com/sphinx-toolbox/seed_intersphinx_mapping/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/sphinx-toolbox/seed_intersphinx_mapping
 	:target: https://github.com/sphinx-toolbox/seed_intersphinx_mapping/commit/master
 	:alt: GitHub last commit
```

### Comparing `seed_intersphinx_mapping-1.2.1/seed_intersphinx_mapping/__init__.py` & `seed_intersphinx_mapping-1.2.2/seed_intersphinx_mapping/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 # this package
 from seed_intersphinx_mapping.cache import cache
 from seed_intersphinx_mapping.extension import setup
 
 __author__: str = "Dominic Davis-Foster"
 __copyright__: str = "2020 Dominic Davis-Foster"
 __license__: str = "MIT License"
-__version__: str = "1.2.1"
+__version__: str = "1.2.2"
 __email__: str = "dominic@davis-foster.co.uk"
 
 __all__ = ["get_sphinx_doc_url", "fallback_mapping", "seed_intersphinx_mapping"]
 
 _DOCUMENTATION_RE = re.compile(r"^[dD]oc(s|umentation)")
```

### Comparing `seed_intersphinx_mapping-1.2.1/seed_intersphinx_mapping/requirements_parsers.py` & `seed_intersphinx_mapping-1.2.2/seed_intersphinx_mapping/requirements_parsers.py`

 * *Files identical despite different names*

### Comparing `seed_intersphinx_mapping-1.2.1/seed_intersphinx_mapping/fallback_mapping.json` & `seed_intersphinx_mapping-1.2.2/seed_intersphinx_mapping/fallback_mapping.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9722222222222222%*

 * *Differences: {"'typing-extensions'": "'https://typing-extensions.readthedocs.io/en/latest/'",*

 * * "'typing_extensions'": "'https://typing-extensions.readthedocs.io/en/latest/'"}*

```diff
@@ -27,12 +27,12 @@
     "python-dateutil": "https://dateutil.readthedocs.io/en/stable/",
     "requests-oauthlib": "https://requests-oauthlib.readthedocs.io/en/latest/",
     "scikit-learn": "https://scikit-learn.org/stable/",
     "six": "https://six.readthedocs.io/",
     "slumber": "https://slumber.readthedocs.io/en/v0.6.0/",
     "sphinx": "https://www.sphinx-doc.org/en/3.x/",
     "typing": "https://docs.python.org/3/",
-    "typing-extensions": "https://docs.python.org/3/",
-    "typing_extensions": "https://docs.python.org/3/",
+    "typing-extensions": "https://typing-extensions.readthedocs.io/en/latest/",
+    "typing_extensions": "https://typing-extensions.readthedocs.io/en/latest/",
     "yarl": "https://yarl.readthedocs.io/en/latest/",
     "zipp": "https://zipp.readthedocs.io/en/latest/"
 }
```

### Comparing `seed_intersphinx_mapping-1.2.1/seed_intersphinx_mapping/__main__.py` & `seed_intersphinx_mapping-1.2.2/seed_intersphinx_mapping/__main__.py`

 * *Files identical despite different names*

### Comparing `seed_intersphinx_mapping-1.2.1/seed_intersphinx_mapping/cache.py` & `seed_intersphinx_mapping-1.2.2/seed_intersphinx_mapping/cache.py`

 * *Files identical despite different names*

### Comparing `seed_intersphinx_mapping-1.2.1/seed_intersphinx_mapping/extension.py` & `seed_intersphinx_mapping-1.2.2/seed_intersphinx_mapping/extension.py`

 * *Files identical despite different names*

