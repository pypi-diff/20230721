# Comparing `tmp/irc_api-1.0.2.tar.gz` & `tmp/irc_api-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irc_api-1.0.2.tar", last modified: Tue Jul  4 20:25:56 2023, max compression
+gzip compressed data, was "irc_api-1.0.3.tar", last modified: Fri Jul 21 08:44:27 2023, max compression
```

## Comparing `irc_api-1.0.2.tar` & `irc_api-1.0.3.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:25:56.135182 irc_api-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-04 20:25:43.000000 irc_api-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-07-04 20:25:56.135182 irc_api-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-07-04 20:25:43.000000 irc_api-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-07-04 20:25:43.000000 irc_api-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 20:25:56.135182 irc_api-1.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:25:56.135182 irc_api-1.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:25:56.135182 irc_api-1.0.2/src/irc_api/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-04 20:25:43.000000 irc_api-1.0.2/src/irc_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13031 2023-07-04 20:25:43.000000 irc_api-1.0.2/src/irc_api/bot.py
--rw-r--r--   0 runner    (1001) docker     (123)     8765 2023-07-04 20:25:43.000000 irc_api-1.0.2/src/irc_api/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-07-04 20:25:43.000000 irc_api-1.0.2/src/irc_api/history.py
--rw-r--r--   0 runner    (1001) docker     (123)     4430 2023-07-04 20:25:43.000000 irc_api-1.0.2/src/irc_api/irc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-07-04 20:25:43.000000 irc_api-1.0.2/src/irc_api/message.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:25:56.135182 irc_api-1.0.2/src/irc_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-07-04 20:25:56.000000 irc_api-1.0.2/src/irc_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-04 20:25:56.000000 irc_api-1.0.2/src/irc_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 20:25:56.000000 irc_api-1.0.2/src/irc_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-04 20:25:56.000000 irc_api-1.0.2/src/irc_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-04 20:25:56.000000 irc_api-1.0.2/src/irc_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:44:27.862825 irc_api-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-21 08:44:18.000000 irc_api-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-07-21 08:44:27.862825 irc_api-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-21 08:44:18.000000 irc_api-1.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-07-21 08:44:18.000000 irc_api-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-21 08:44:18.000000 irc_api-1.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 08:44:27.862825 irc_api-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-21 08:44:18.000000 irc_api-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:44:27.858825 irc_api-1.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:44:27.862825 irc_api-1.0.3/src/irc_api/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-21 08:44:18.000000 irc_api-1.0.3/src/irc_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13031 2023-07-21 08:44:18.000000 irc_api-1.0.3/src/irc_api/bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8765 2023-07-21 08:44:18.000000 irc_api-1.0.3/src/irc_api/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-07-21 08:44:18.000000 irc_api-1.0.3/src/irc_api/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4430 2023-07-21 08:44:18.000000 irc_api-1.0.3/src/irc_api/irc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-07-21 08:44:18.000000 irc_api-1.0.3/src/irc_api/message.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:44:27.862825 irc_api-1.0.3/src/irc_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-07-21 08:44:27.000000 irc_api-1.0.3/src/irc_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-21 08:44:27.000000 irc_api-1.0.3/src/irc_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 08:44:27.000000 irc_api-1.0.3/src/irc_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-21 08:44:27.000000 irc_api-1.0.3/src/irc_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-21 08:44:27.000000 irc_api-1.0.3/src/irc_api.egg-info/top_level.txt
```

### Comparing `irc_api-1.0.2/LICENSE` & `irc_api-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `irc_api-1.0.2/PKG-INFO` & `irc_api-1.0.3/src/irc_api.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
-Name: irc_api
-Version: 1.0.2
+Name: irc-api
+Version: 1.0.3
 Summary: An API written in Python to make IRC bots.
 Author: Sha-chan
 Project-URL: Homepage, https://github.com/Shadow15510/irc_api
-Project-URL: Documentation, https://irc-api.readthedocs.io/en/latest/
+Project-URL: Documentation, https://irc-api.readthedocs.io/en/stable/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Development Status :: 5 - Production/Stable
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: doc
 License-File: LICENSE
 
 # IRC API
-[![Documentation Status](https://readthedocs.org/projects/irc-api/badge/?version=latest)](https://irc-api.readthedocs.io/en/latest/?badge=latest) [![Licence](https://img.shields.io/github/license/Shadow15510/irc_api?color=green)](https://github.com/Shadow15510/irc_api/blob/master/LICENSE)
+[![Documentation Status](https://readthedocs.org/projects/irc-api/badge/?version=latest)](https://irc-api.readthedocs.io/en/latest/?badge=latest)
+[![Licence](https://img.shields.io/github/license/Shadow15510/irc_api?color=green)](https://github.com/Shadow15510/irc_api/blob/master/LICENSE)
+[![Build Status](https://github.com/Shadow15510/irc_api/actions/workflows/python-publish.yml/badge.svg)](https://github.com/Shadow15510/irc_api/actions/workflows/python-publish.yml)
 
 ## Description
 IRC API is a small API to make Python IRC bots. This API is based on decorators to make commands like the `cog` module in `discord.py`.
 
 If you encounter any issue feel free to [open one](https://github.com/Shadow15510/irc_api/issues).
 A full documentation is available on [readthedocs](https://irc-api.readthedocs.io/en/latest/).
```

### Comparing `irc_api-1.0.2/README.md` & `irc_api-1.0.3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # IRC API
-[![Documentation Status](https://readthedocs.org/projects/irc-api/badge/?version=latest)](https://irc-api.readthedocs.io/en/latest/?badge=latest) [![Licence](https://img.shields.io/github/license/Shadow15510/irc_api?color=green)](https://github.com/Shadow15510/irc_api/blob/master/LICENSE)
+[![Documentation Status](https://readthedocs.org/projects/irc-api/badge/?version=latest)](https://irc-api.readthedocs.io/en/latest/?badge=latest)
+[![Licence](https://img.shields.io/github/license/Shadow15510/irc_api?color=green)](https://github.com/Shadow15510/irc_api/blob/master/LICENSE)
+[![Build Status](https://github.com/Shadow15510/irc_api/actions/workflows/python-publish.yml/badge.svg)](https://github.com/Shadow15510/irc_api/actions/workflows/python-publish.yml)
 
 ## Description
 IRC API is a small API to make Python IRC bots. This API is based on decorators to make commands like the `cog` module in `discord.py`.
 
 If you encounter any issue feel free to [open one](https://github.com/Shadow15510/irc_api/issues).
 A full documentation is available on [readthedocs](https://irc-api.readthedocs.io/en/latest/).
```

### Comparing `irc_api-1.0.2/pyproject.toml` & `irc_api-1.0.3/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 classifiers = [
 	"Programming Language :: Python :: 3",
 	"License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
 	"Development Status :: 5 - Production/Stable",
 ]
 dynamic = [
 	"version",
+	"dependencies"
 ]
 
 [tool.setuptools]
 license-files = [
     "LICENSE",
 ]
 
@@ -30,10 +31,14 @@
     "sphinx-rtd-theme",
     "sphinx-autodocgen",
 ]
 
 [tool.setuptools.dynamic.version]
 attr = "irc_api.__init__.__version__"
 
+[tool.setuptools.dynamic]
+dependencies = {file = ["requirements.txt"]}
+
+
 [project.urls]
 Homepage = "https://github.com/Shadow15510/irc_api"
-Documentation = "https://irc-api.readthedocs.io/en/latest/"
+Documentation = "https://irc-api.readthedocs.io/en/stable/"
```

### Comparing `irc_api-1.0.2/src/irc_api/bot.py` & `irc_api-1.0.3/src/irc_api/bot.py`

 * *Files identical despite different names*

### Comparing `irc_api-1.0.2/src/irc_api/commands.py` & `irc_api-1.0.3/src/irc_api/commands.py`

 * *Files identical despite different names*

### Comparing `irc_api-1.0.2/src/irc_api/history.py` & `irc_api-1.0.3/src/irc_api/history.py`

 * *Files identical despite different names*

### Comparing `irc_api-1.0.2/src/irc_api/irc.py` & `irc_api-1.0.3/src/irc_api/irc.py`

 * *Files identical despite different names*

### Comparing `irc_api-1.0.2/src/irc_api/message.py` & `irc_api-1.0.3/src/irc_api/message.py`

 * *Files identical despite different names*

### Comparing `irc_api-1.0.2/src/irc_api.egg-info/PKG-INFO` & `irc_api-1.0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
-Name: irc-api
-Version: 1.0.2
+Name: irc_api
+Version: 1.0.3
 Summary: An API written in Python to make IRC bots.
 Author: Sha-chan
 Project-URL: Homepage, https://github.com/Shadow15510/irc_api
-Project-URL: Documentation, https://irc-api.readthedocs.io/en/latest/
+Project-URL: Documentation, https://irc-api.readthedocs.io/en/stable/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Development Status :: 5 - Production/Stable
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: doc
 License-File: LICENSE
 
 # IRC API
-[![Documentation Status](https://readthedocs.org/projects/irc-api/badge/?version=latest)](https://irc-api.readthedocs.io/en/latest/?badge=latest) [![Licence](https://img.shields.io/github/license/Shadow15510/irc_api?color=green)](https://github.com/Shadow15510/irc_api/blob/master/LICENSE)
+[![Documentation Status](https://readthedocs.org/projects/irc-api/badge/?version=latest)](https://irc-api.readthedocs.io/en/latest/?badge=latest)
+[![Licence](https://img.shields.io/github/license/Shadow15510/irc_api?color=green)](https://github.com/Shadow15510/irc_api/blob/master/LICENSE)
+[![Build Status](https://github.com/Shadow15510/irc_api/actions/workflows/python-publish.yml/badge.svg)](https://github.com/Shadow15510/irc_api/actions/workflows/python-publish.yml)
 
 ## Description
 IRC API is a small API to make Python IRC bots. This API is based on decorators to make commands like the `cog` module in `discord.py`.
 
 If you encounter any issue feel free to [open one](https://github.com/Shadow15510/irc_api/issues).
 A full documentation is available on [readthedocs](https://irc-api.readthedocs.io/en/latest/).
```

