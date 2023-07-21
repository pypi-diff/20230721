# Comparing `tmp/ou_tm351_jl_extensions-0.2.1.tar.gz` & `tmp/ou_tm351_jl_extensions-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ou_tm351_jl_extensions-0.2.1.tar", max compression
+gzip compressed data, was "ou_tm351_jl_extensions-0.2.2.tar", max compression
```

## Comparing `ou_tm351_jl_extensions-0.2.1.tar` & `ou_tm351_jl_extensions-0.2.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1074 2023-07-05 00:48:01.501932 ou_tm351_jl_extensions-0.2.1/LICENSE
--rw-r--r--   0        0        0     1370 2023-07-05 00:48:01.501932 ou_tm351_jl_extensions-0.2.1/README.md
--rw-r--r--   0        0        0     2388 2023-07-05 00:48:01.501932 ou_tm351_jl_extensions-0.2.1/ou_tm351_jl_extensions/__init__.py
--rw-r--r--   0        0        0      938 2023-07-05 00:48:01.501932 ou_tm351_jl_extensions-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     2691 1970-01-01 00:00:00.000000 ou_tm351_jl_extensions-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-07-21 20:51:46.057210 ou_tm351_jl_extensions-0.2.2/LICENSE
+-rw-r--r--   0        0        0     1226 2023-07-21 20:51:46.057210 ou_tm351_jl_extensions-0.2.2/README.md
+-rw-r--r--   0        0        0     2388 2023-07-21 20:51:46.061210 ou_tm351_jl_extensions-0.2.2/ou_tm351_jl_extensions/__init__.py
+-rw-r--r--   0        0        0      937 2023-07-21 20:51:46.061210 ou_tm351_jl_extensions-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     2603 1970-01-01 00:00:00.000000 ou_tm351_jl_extensions-0.2.2/PKG-INFO
```

### Comparing `ou_tm351_jl_extensions-0.2.1/LICENSE` & `ou_tm351_jl_extensions-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ou_tm351_jl_extensions-0.2.1/README.md` & `ou_tm351_jl_extensions-0.2.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -18,29 +18,26 @@
 jupyterlab-myst = "^1.1.3"
 jupyterlab-empinken-extension = "^0.4.0"
 jupyterlab-geojson = "^3.3.1"
 jupyterlab-skip-traceback = "^5.0.0"
 jupyterlab-git = "^0.41.0"
 jupytext = "^1.14.5"
 jupyter-archive = "^3.3.4"
-#jupyterlab-spellchecker = "^0.7.3"
+jupyterlab-spellchecker = "^0.8.3"
 jupyterlab-language-pack-fr-fr = "^3.6.post1"
 jupyterlab-language-pack-zh-cn = "^3.6.post1"
 jupyter-resource-usage = "^0.7.2"
 stickyland = "^0.2.1"
 #jupyterlab-tour = "^3.1.4"
 jupyter-compare-view = "^0.2.4"
 jupyterlab-filesystem-access = "^0.5.3"
 ```
 
-*NB jupyterlab-spellchecker appears to be broken atm in JL4; [related issue](https://github.com/jupyterlab-contrib/spellchecker/issues/127)*
-
 Check the installation by running:
 
-
 ```python
 import ou_tm351_jl_extensions as ou
 ou.check_install()
 ```
 
 __Maintenance__
```

### Comparing `ou_tm351_jl_extensions-0.2.1/ou_tm351_jl_extensions/__init__.py` & `ou_tm351_jl_extensions-0.2.2/ou_tm351_jl_extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `ou_tm351_jl_extensions-0.2.1/pyproject.toml` & `ou_tm351_jl_extensions-0.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ou-tm351-jl-extensions"
-version = "0.2.1"
+version = "0.2.2"
 description = ""
 authors = ["Tony Hirst <tony.hirst@gmail.com>"]
 readme = "README.md"
 packages = [{include = "ou_tm351_jl_extensions"}]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.13"
@@ -14,15 +14,15 @@
 jupyterlab-myst = "^2.0.0"
 jupyterlab-empinken-extension = "^0.4.0"
 jupyterlab-geojson = "^3.3.1"
 jupyterlab-skip-traceback = "^5.0.0"
 jupyterlab-git = "^0.41.0"
 jupytext = "^1.14.5"
 jupyter-archive = "^3.3.4"
-#jupyterlab-spellchecker = "^0.7.3"
+jupyterlab-spellchecker = "^0.8.3"
 jupyterlab-language-pack-fr-fr = "^3.6.post1"
 jupyterlab-language-pack-zh-cn = "^3.6.post1"
 jupyter-resource-usage = "^0.7.2"
 stickyland = "^0.2.1"
 #jupyterlab-tour = "^3.1.4"
 jupyter-compare-view = "^0.2.4"
 jupyterlab-filesystem-access = "^0.5.3"
```

### Comparing `ou_tm351_jl_extensions-0.2.1/PKG-INFO` & `ou_tm351_jl_extensions-0.2.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ou-tm351-jl-extensions
-Version: 0.2.1
+Version: 0.2.2
 Summary: 
 Author: Tony Hirst
 Author-email: tony.hirst@gmail.com
 Requires-Python: >=3.8,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -20,14 +20,15 @@
 Requires-Dist: jupyterlab-geojson (>=3.3.1,<4.0.0)
 Requires-Dist: jupyterlab-git (>=0.41.0,<0.42.0)
 Requires-Dist: jupyterlab-language-pack-fr-fr (>=3.6.post1,<4.0)
 Requires-Dist: jupyterlab-language-pack-zh-cn (>=3.6.post1,<4.0)
 Requires-Dist: jupyterlab-myst (>=2.0.0,<3.0.0)
 Requires-Dist: jupyterlab-ou-brand-extension (>=0.2.0,<0.3.0)
 Requires-Dist: jupyterlab-skip-traceback (>=5.0.0,<6.0.0)
+Requires-Dist: jupyterlab-spellchecker (>=0.8.3,<0.9.0)
 Requires-Dist: jupytext (>=1.14.5,<2.0.0)
 Requires-Dist: stickyland (>=0.2.1,<0.3.0)
 Description-Content-Type: text/markdown
 
 # ou-tm351-jl-extensions
 
 Install from pypi as `ou-tm351-jl-extensions`
@@ -48,29 +49,26 @@
 jupyterlab-myst = "^1.1.3"
 jupyterlab-empinken-extension = "^0.4.0"
 jupyterlab-geojson = "^3.3.1"
 jupyterlab-skip-traceback = "^5.0.0"
 jupyterlab-git = "^0.41.0"
 jupytext = "^1.14.5"
 jupyter-archive = "^3.3.4"
-#jupyterlab-spellchecker = "^0.7.3"
+jupyterlab-spellchecker = "^0.8.3"
 jupyterlab-language-pack-fr-fr = "^3.6.post1"
 jupyterlab-language-pack-zh-cn = "^3.6.post1"
 jupyter-resource-usage = "^0.7.2"
 stickyland = "^0.2.1"
 #jupyterlab-tour = "^3.1.4"
 jupyter-compare-view = "^0.2.4"
 jupyterlab-filesystem-access = "^0.5.3"
 ```
 
-*NB jupyterlab-spellchecker appears to be broken atm in JL4; [related issue](https://github.com/jupyterlab-contrib/spellchecker/issues/127)*
-
 Check the installation by running:
 
-
 ```python
 import ou_tm351_jl_extensions as ou
 ou.check_install()
 ```
 
 __Maintenance__
```

