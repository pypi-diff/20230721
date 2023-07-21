# Comparing `tmp/logdna-1.8.0.tar.gz` & `tmp/logdna-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/logdna-1.8.0.tar", last modified: Thu Apr 15 15:24:44 2021, max compression
+gzip compressed data, was "dist/logdna-1.9.0.tar", last modified: Thu Apr 15 15:26:32 2021, max compression
```

## Comparing `logdna-1.8.0.tar` & `logdna-1.9.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 logdna    (1000) logdna    (1000)        0 2021-04-15 15:24:44.000000 logdna-1.8.0/
--rw-rw-r--   0 logdna    (1000) logdna    (1000)     4821 2021-04-15 15:23:14.000000 logdna-1.8.0/.all-contributorsrc
--rw-rw-r--   0 logdna    (1000) logdna    (1000)      428 2021-04-15 15:23:14.000000 logdna-1.8.0/.config.mk
--rw-rw-r--   0 logdna    (1000) logdna    (1000)      165 2021-04-15 15:23:14.000000 logdna-1.8.0/.gitignore
--rw-rw-r--   0 logdna    (1000) logdna    (1000)     3731 2021-04-15 15:24:40.000000 logdna-1.8.0/CHANGELOG.md
--rw-rw-r--   0 logdna    (1000) logdna    (1000)     5554 2021-04-15 15:23:14.000000 logdna-1.8.0/CODE_OF_CONDUCT.md
--rw-rw-r--   0 logdna    (1000) logdna    (1000)     1626 2021-04-15 15:23:14.000000 logdna-1.8.0/CONTRIBUTING.md
--rw-r--r--   0 logdna    (1000) logdna    (1000)     1405 2021-04-15 15:24:40.000000 logdna-1.8.0/Jenkinsfile
--rw-rw-r--   0 logdna    (1000) logdna    (1000)     1073 2021-04-15 15:23:14.000000 logdna-1.8.0/LICENSE
--rw-rw-r--   0 logdna    (1000) logdna    (1000)     2683 2021-04-15 15:23:14.000000 logdna-1.8.0/Makefile
--rw-r--r--   0 logdna    (1000) logdna    (1000)    20423 2021-04-15 15:24:44.000000 logdna-1.8.0/PKG-INFO
--rw-rw-r--   0 logdna    (1000) logdna    (1000)    16386 2021-04-15 15:23:14.000000 logdna-1.8.0/README.md
-drwxr-xr-x   0 logdna    (1000) logdna    (1000)        0 2021-04-15 15:24:44.000000 logdna-1.8.0/logdna/
--rw-rw-r--   0 logdna    (1000) logdna    (1000)        6 2021-04-15 15:24:40.000000 logdna-1.8.0/logdna/VERSION
--rw-rw-r--   0 logdna    (1000) logdna    (1000)      273 2021-04-15 15:23:14.000000 logdna-1.8.0/logdna/__init__.py
--rw-rw-r--   0 logdna    (1000) logdna    (1000)      509 2021-04-15 15:23:14.000000 logdna-1.8.0/logdna/configs.py
--rw-rw-r--   0 logdna    (1000) logdna    (1000)     7488 2021-04-15 15:23:14.000000 logdna-1.8.0/logdna/logdna.py
--rw-rw-r--   0 logdna    (1000) logdna    (1000)      840 2021-04-15 15:23:14.000000 logdna-1.8.0/logdna/utils.py
-drwxr-xr-x   0 logdna    (1000) logdna    (1000)        0 2021-04-15 15:24:44.000000 logdna-1.8.0/logdna.egg-info/
--rw-r--r--   0 logdna    (1000) logdna    (1000)    20423 2021-04-15 15:24:44.000000 logdna-1.8.0/logdna.egg-info/PKG-INFO
--rw-r--r--   0 logdna    (1000) logdna    (1000)      555 2021-04-15 15:24:44.000000 logdna-1.8.0/logdna.egg-info/SOURCES.txt
--rw-r--r--   0 logdna    (1000) logdna    (1000)        1 2021-04-15 15:24:44.000000 logdna-1.8.0/logdna.egg-info/dependency_links.txt
--rw-r--r--   0 logdna    (1000) logdna    (1000)        9 2021-04-15 15:24:44.000000 logdna-1.8.0/logdna.egg-info/requires.txt
--rw-r--r--   0 logdna    (1000) logdna    (1000)        7 2021-04-15 15:24:44.000000 logdna-1.8.0/logdna.egg-info/top_level.txt
--rw-rw-r--   0 logdna    (1000) logdna    (1000)    57073 2021-04-15 15:23:14.000000 logdna-1.8.0/poetry.lock
--rw-rw-r--   0 logdna    (1000) logdna    (1000)     1398 2021-04-15 15:24:40.000000 logdna-1.8.0/pyproject.toml
-drwxr-xr-x   0 logdna    (1000) logdna    (1000)        0 2021-04-15 15:24:44.000000 logdna-1.8.0/scripts/
--rw-rw-r--   0 logdna    (1000) logdna    (1000)     1484 2021-04-15 15:23:14.000000 logdna-1.8.0/scripts/json_coverage.py
--rw-rw-r--   0 logdna    (1000) logdna    (1000)      255 2021-04-15 15:24:44.000000 logdna-1.8.0/setup.cfg
--rw-rw-r--   0 logdna    (1000) logdna    (1000)     1306 2021-04-15 15:23:14.000000 logdna-1.8.0/setup.py
-drwxr-xr-x   0 logdna    (1000) logdna    (1000)        0 2021-04-15 15:24:44.000000 logdna-1.8.0/tests/
--rw-rw-r--   0 logdna    (1000) logdna    (1000)       48 2021-04-15 15:23:14.000000 logdna-1.8.0/tests/__init__.py
-drwxr-xr-x   0 logdna    (1000) logdna    (1000)        0 2021-04-15 15:24:44.000000 logdna-1.8.0/tests/mock/
--rw-rw-r--   0 logdna    (1000) logdna    (1000)        0 2021-04-15 15:23:14.000000 logdna-1.8.0/tests/mock/__init.__.py
--rw-rw-r--   0 logdna    (1000) logdna    (1000)      391 2021-04-15 15:23:14.000000 logdna-1.8.0/tests/mock/log.py
--rw-rw-r--   0 logdna    (1000) logdna    (1000)      443 2021-04-15 15:23:14.000000 logdna-1.8.0/tests/mock/server.py
--rw-rw-r--   0 logdna    (1000) logdna    (1000)     3357 2021-04-15 15:23:14.000000 logdna-1.8.0/tests/test_logger.py
--rw-rw-r--   0 logdna    (1000) logdna    (1000)     1537 2021-04-15 15:23:14.000000 logdna-1.8.0/tests/test_utils.py
+drwxr-xr-x   0 logdna    (1000) logdna    (1000)        0 2021-04-15 15:26:32.000000 logdna-1.9.0/
+-rw-rw-r--   0 logdna    (1000) logdna    (1000)     4821 2021-04-15 15:25:03.000000 logdna-1.9.0/.all-contributorsrc
+-rw-rw-r--   0 logdna    (1000) logdna    (1000)      428 2021-04-15 15:25:03.000000 logdna-1.9.0/.config.mk
+-rw-rw-r--   0 logdna    (1000) logdna    (1000)      165 2021-04-15 15:25:03.000000 logdna-1.9.0/.gitignore
+-rw-rw-r--   0 logdna    (1000) logdna    (1000)     3756 2021-04-15 15:26:28.000000 logdna-1.9.0/CHANGELOG.md
+-rw-rw-r--   0 logdna    (1000) logdna    (1000)     5554 2021-04-15 15:25:03.000000 logdna-1.9.0/CODE_OF_CONDUCT.md
+-rw-rw-r--   0 logdna    (1000) logdna    (1000)     1626 2021-04-15 15:25:03.000000 logdna-1.9.0/CONTRIBUTING.md
+-rw-rw-r--   0 logdna    (1000) logdna    (1000)     1405 2021-04-15 15:25:03.000000 logdna-1.9.0/Jenkinsfile
+-rw-rw-r--   0 logdna    (1000) logdna    (1000)     1073 2021-04-15 15:25:03.000000 logdna-1.9.0/LICENSE
+-rw-rw-r--   0 logdna    (1000) logdna    (1000)     2683 2021-04-15 15:25:03.000000 logdna-1.9.0/Makefile
+-rw-r--r--   0 logdna    (1000) logdna    (1000)    20423 2021-04-15 15:26:32.000000 logdna-1.9.0/PKG-INFO
+-rw-rw-r--   0 logdna    (1000) logdna    (1000)    16386 2021-04-15 15:25:03.000000 logdna-1.9.0/README.md
+drwxr-xr-x   0 logdna    (1000) logdna    (1000)        0 2021-04-15 15:26:32.000000 logdna-1.9.0/logdna/
+-rw-rw-r--   0 logdna    (1000) logdna    (1000)        6 2021-04-15 15:26:28.000000 logdna-1.9.0/logdna/VERSION
+-rw-rw-r--   0 logdna    (1000) logdna    (1000)      273 2021-04-15 15:25:03.000000 logdna-1.9.0/logdna/__init__.py
+-rw-rw-r--   0 logdna    (1000) logdna    (1000)      509 2021-04-15 15:25:03.000000 logdna-1.9.0/logdna/configs.py
+-rw-rw-r--   0 logdna    (1000) logdna    (1000)     7488 2021-04-15 15:25:03.000000 logdna-1.9.0/logdna/logdna.py
+-rw-rw-r--   0 logdna    (1000) logdna    (1000)      840 2021-04-15 15:25:03.000000 logdna-1.9.0/logdna/utils.py
+drwxr-xr-x   0 logdna    (1000) logdna    (1000)        0 2021-04-15 15:26:32.000000 logdna-1.9.0/logdna.egg-info/
+-rw-r--r--   0 logdna    (1000) logdna    (1000)    20423 2021-04-15 15:26:32.000000 logdna-1.9.0/logdna.egg-info/PKG-INFO
+-rw-r--r--   0 logdna    (1000) logdna    (1000)      555 2021-04-15 15:26:32.000000 logdna-1.9.0/logdna.egg-info/SOURCES.txt
+-rw-r--r--   0 logdna    (1000) logdna    (1000)        1 2021-04-15 15:26:32.000000 logdna-1.9.0/logdna.egg-info/dependency_links.txt
+-rw-r--r--   0 logdna    (1000) logdna    (1000)        9 2021-04-15 15:26:32.000000 logdna-1.9.0/logdna.egg-info/requires.txt
+-rw-r--r--   0 logdna    (1000) logdna    (1000)        7 2021-04-15 15:26:32.000000 logdna-1.9.0/logdna.egg-info/top_level.txt
+-rw-rw-r--   0 logdna    (1000) logdna    (1000)    57073 2021-04-15 15:25:03.000000 logdna-1.9.0/poetry.lock
+-rw-rw-r--   0 logdna    (1000) logdna    (1000)     1398 2021-04-15 15:26:28.000000 logdna-1.9.0/pyproject.toml
+drwxr-xr-x   0 logdna    (1000) logdna    (1000)        0 2021-04-15 15:26:32.000000 logdna-1.9.0/scripts/
+-rw-rw-r--   0 logdna    (1000) logdna    (1000)     1484 2021-04-15 15:25:03.000000 logdna-1.9.0/scripts/json_coverage.py
+-rw-rw-r--   0 logdna    (1000) logdna    (1000)      255 2021-04-15 15:26:32.000000 logdna-1.9.0/setup.cfg
+-rw-rw-r--   0 logdna    (1000) logdna    (1000)     1306 2021-04-15 15:25:03.000000 logdna-1.9.0/setup.py
+drwxr-xr-x   0 logdna    (1000) logdna    (1000)        0 2021-04-15 15:26:32.000000 logdna-1.9.0/tests/
+-rw-rw-r--   0 logdna    (1000) logdna    (1000)       48 2021-04-15 15:25:03.000000 logdna-1.9.0/tests/__init__.py
+drwxr-xr-x   0 logdna    (1000) logdna    (1000)        0 2021-04-15 15:26:32.000000 logdna-1.9.0/tests/mock/
+-rw-rw-r--   0 logdna    (1000) logdna    (1000)        0 2021-04-15 15:25:03.000000 logdna-1.9.0/tests/mock/__init.__.py
+-rw-rw-r--   0 logdna    (1000) logdna    (1000)      391 2021-04-15 15:25:03.000000 logdna-1.9.0/tests/mock/log.py
+-rw-rw-r--   0 logdna    (1000) logdna    (1000)      443 2021-04-15 15:25:03.000000 logdna-1.9.0/tests/mock/server.py
+-rw-rw-r--   0 logdna    (1000) logdna    (1000)     3357 2021-04-15 15:25:03.000000 logdna-1.9.0/tests/test_logger.py
+-rw-rw-r--   0 logdna    (1000) logdna    (1000)     1537 2021-04-15 15:25:03.000000 logdna-1.9.0/tests/test_utils.py
```

### Comparing `logdna-1.8.0/.all-contributorsrc` & `logdna-1.9.0/.all-contributorsrc`

 * *Files identical despite different names*

### Comparing `logdna-1.8.0/CHANGELOG.md` & `logdna-1.9.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v1.9.0 (2021-04-15)
+
+
 ## v1.8.0 (2021-04-15)
 
 
 ## v1.7.0 (2021-04-07)
 
 
 ## v1.6.0 (2021-04-07)
```

### Comparing `logdna-1.8.0/CODE_OF_CONDUCT.md` & `logdna-1.9.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `logdna-1.8.0/CONTRIBUTING.md` & `logdna-1.9.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `logdna-1.8.0/Jenkinsfile` & `logdna-1.9.0/Jenkinsfile`

 * *Files identical despite different names*

### Comparing `logdna-1.8.0/LICENSE` & `logdna-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `logdna-1.8.0/Makefile` & `logdna-1.9.0/Makefile`

 * *Files identical despite different names*

### Comparing `logdna-1.8.0/PKG-INFO` & `logdna-1.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: logdna
-Version: 1.8.0
+Version: 1.9.0
 Summary: A Python Package for Sending Logs to LogDNA
 Home-page: https://github.com/logdna/python
 Author: LogDNA Inc.
 Author-email: help@logdna.com
 License: MIT
-Download-URL: https://github.com/logdna/python/tarball/1.8.0
+Download-URL: https://github.com/logdna/python/tarball/1.9.0
 Description: <p align="center">
           <a href="https://app.logdna.com">
             <img height="95" width="202" src="https://raw.githubusercontent.com/logdna/artwork/master/logo%2Bpython.png">
           </a>
           <p align="center">Python package for logging to <a href="https://app.logdna.com">LogDNA</a></p>
         </p>
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: logdna Version: 1.8.0 Summary: A Python Package for
+Metadata-Version: 2.1 Name: logdna Version: 1.9.0 Summary: A Python Package for
 Sending Logs to LogDNA Home-page: https://github.com/logdna/python Author:
 LogDNA Inc. Author-email: help@logdna.com License: MIT Download-URL: https://
-github.com/logdna/python/tarball/1.8.0 Description:
+github.com/logdna/python/tarball/1.9.0 Description:
   [https://raw.githubusercontent.com/logdna/artwork/master/logo%2Bpython.png]
                      Python package for logging to LogDNA
  [![All Contributors](https://img.shields.io/badge/all_contributors-18-
 orange.svg?style=flat-square)](#contributors-)  --- * [Installation]
 (#installation) * [Setup](#setup) * [Usage](#usage) * [Usage with File Config]
 (#usage-with-file-config) * [API](#api) * [LogDNAHandler(key: string, [options:
 dict])](#logdnahandlerkey-string-options-dict) * [key](#key) * [options]
```

### Comparing `logdna-1.8.0/README.md` & `logdna-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `logdna-1.8.0/logdna/logdna.py` & `logdna-1.9.0/logdna/logdna.py`

 * *Files identical despite different names*

### Comparing `logdna-1.8.0/logdna/utils.py` & `logdna-1.9.0/logdna/utils.py`

 * *Files identical despite different names*

### Comparing `logdna-1.8.0/logdna.egg-info/PKG-INFO` & `logdna-1.9.0/logdna.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: logdna
-Version: 1.8.0
+Version: 1.9.0
 Summary: A Python Package for Sending Logs to LogDNA
 Home-page: https://github.com/logdna/python
 Author: LogDNA Inc.
 Author-email: help@logdna.com
 License: MIT
-Download-URL: https://github.com/logdna/python/tarball/1.8.0
+Download-URL: https://github.com/logdna/python/tarball/1.9.0
 Description: <p align="center">
           <a href="https://app.logdna.com">
             <img height="95" width="202" src="https://raw.githubusercontent.com/logdna/artwork/master/logo%2Bpython.png">
           </a>
           <p align="center">Python package for logging to <a href="https://app.logdna.com">LogDNA</a></p>
         </p>
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: logdna Version: 1.8.0 Summary: A Python Package for
+Metadata-Version: 2.1 Name: logdna Version: 1.9.0 Summary: A Python Package for
 Sending Logs to LogDNA Home-page: https://github.com/logdna/python Author:
 LogDNA Inc. Author-email: help@logdna.com License: MIT Download-URL: https://
-github.com/logdna/python/tarball/1.8.0 Description:
+github.com/logdna/python/tarball/1.9.0 Description:
   [https://raw.githubusercontent.com/logdna/artwork/master/logo%2Bpython.png]
                      Python package for logging to LogDNA
  [![All Contributors](https://img.shields.io/badge/all_contributors-18-
 orange.svg?style=flat-square)](#contributors-)  --- * [Installation]
 (#installation) * [Setup](#setup) * [Usage](#usage) * [Usage with File Config]
 (#usage-with-file-config) * [API](#api) * [LogDNAHandler(key: string, [options:
 dict])](#logdnahandlerkey-string-options-dict) * [key](#key) * [options]
```

### Comparing `logdna-1.8.0/logdna.egg-info/SOURCES.txt` & `logdna-1.9.0/logdna.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `logdna-1.8.0/poetry.lock` & `logdna-1.9.0/poetry.lock`

 * *Files identical despite different names*

### Comparing `logdna-1.8.0/pyproject.toml` & `logdna-1.9.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "logdna"
-version = "1.8.0"
+version = "1.9.0"
 description = 'A Python Package for Sending Logs to LogDNA'
 authors = ["logdna <help@logdna.com>"]
 license = "MIT"
 
 [tool.semantic_release]
 version_toml = "pyproject.toml:tool.poetry.version"
 version_pattern = "logdna/VERSION:(\\d+\\.\\d+\\.\\d+)"
```

### Comparing `logdna-1.8.0/scripts/json_coverage.py` & `logdna-1.9.0/scripts/json_coverage.py`

 * *Files identical despite different names*

### Comparing `logdna-1.8.0/setup.py` & `logdna-1.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `logdna-1.8.0/tests/test_logger.py` & `logdna-1.9.0/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `logdna-1.8.0/tests/test_utils.py` & `logdna-1.9.0/tests/test_utils.py`

 * *Files identical despite different names*

