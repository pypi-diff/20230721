# Comparing `tmp/aiopegelonline-0.0.1.tar.gz` & `tmp/aiopegelonline-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiopegelonline-0.0.1.tar", last modified: Fri Jul 21 13:56:48 2023, max compression
+gzip compressed data, was "aiopegelonline-0.0.2.tar", last modified: Fri Jul 21 15:03:06 2023, max compression
```

## Comparing `aiopegelonline-0.0.1.tar` & `aiopegelonline-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-21 13:56:48.701594 aiopegelonline-0.0.1/
--rw-r--r--   0 vscode    (1000) vscode    (1000)    11357 2023-07-21 11:00:36.000000 aiopegelonline-0.0.1/LICENSE
--rw-r--r--   0 vscode    (1000) vscode    (1000)      748 2023-07-21 13:56:48.701594 aiopegelonline-0.0.1/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)       72 2023-07-21 11:00:36.000000 aiopegelonline-0.0.1/README.md
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-21 13:56:48.701594 aiopegelonline-0.0.1/aiopegelonline/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2738 2023-07-21 13:26:08.000000 aiopegelonline-0.0.1/aiopegelonline/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      300 2023-07-21 13:37:16.000000 aiopegelonline-0.0.1/aiopegelonline/const.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      434 2023-07-21 13:13:18.000000 aiopegelonline-0.0.1/aiopegelonline/exceptions.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-21 13:56:48.701594 aiopegelonline-0.0.1/aiopegelonline.egg-info/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      748 2023-07-21 13:56:48.000000 aiopegelonline-0.0.1/aiopegelonline.egg-info/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)      338 2023-07-21 13:56:48.000000 aiopegelonline-0.0.1/aiopegelonline.egg-info/SOURCES.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-07-21 13:56:48.000000 aiopegelonline-0.0.1/aiopegelonline.egg-info/dependency_links.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        8 2023-07-21 13:56:48.000000 aiopegelonline-0.0.1/aiopegelonline.egg-info/requires.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       15 2023-07-21 13:56:48.000000 aiopegelonline-0.0.1/aiopegelonline.egg-info/top_level.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-07-21 11:46:41.000000 aiopegelonline-0.0.1/aiopegelonline.egg-info/zip-safe
--rw-r--r--   0 vscode    (1000) vscode    (1000)      298 2023-07-21 13:56:48.701594 aiopegelonline-0.0.1/setup.cfg
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1202 2023-07-21 13:26:08.000000 aiopegelonline-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:03:06.948882 aiopegelonline-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-21 15:02:53.000000 aiopegelonline-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-07-21 15:03:06.948882 aiopegelonline-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-21 15:02:53.000000 aiopegelonline-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:03:06.948882 aiopegelonline-0.0.2/aiopegelonline/
+-rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-07-21 15:02:53.000000 aiopegelonline-0.0.2/aiopegelonline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-21 15:02:53.000000 aiopegelonline-0.0.2/aiopegelonline/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-21 15:02:53.000000 aiopegelonline-0.0.2/aiopegelonline/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 15:02:53.000000 aiopegelonline-0.0.2/aiopegelonline/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:03:06.948882 aiopegelonline-0.0.2/aiopegelonline.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-07-21 15:03:06.000000 aiopegelonline-0.0.2/aiopegelonline.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-21 15:03:06.000000 aiopegelonline-0.0.2/aiopegelonline.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 15:03:06.000000 aiopegelonline-0.0.2/aiopegelonline.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-21 15:03:06.000000 aiopegelonline-0.0.2/aiopegelonline.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-21 15:03:06.000000 aiopegelonline-0.0.2/aiopegelonline.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 15:03:06.000000 aiopegelonline-0.0.2/aiopegelonline.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-21 15:03:06.948882 aiopegelonline-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-07-21 15:02:53.000000 aiopegelonline-0.0.2/setup.py
```

### Comparing `aiopegelonline-0.0.1/LICENSE` & `aiopegelonline-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aiopegelonline-0.0.1/PKG-INFO` & `aiopegelonline-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiopegelonline
-Version: 0.0.1
+Version: 0.0.2
 Summary: Asynchronous library to retrieve data from PEGELONLINE.
 Home-page: https://github.com/mib1185/aiopegelonline
 Author: mib1185
 License: Apache License 2.0
 Platform: any
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -15,7 +15,9 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # aiopegelonline
 Asynchronous library to retrieve data from PEGELONLINE
+
+
```

### Comparing `aiopegelonline-0.0.1/aiopegelonline/__init__.py` & `aiopegelonline-0.0.2/aiopegelonline/__init__.py`

 * *Files identical despite different names*

### Comparing `aiopegelonline-0.0.1/aiopegelonline.egg-info/PKG-INFO` & `aiopegelonline-0.0.2/aiopegelonline.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiopegelonline
-Version: 0.0.1
+Version: 0.0.2
 Summary: Asynchronous library to retrieve data from PEGELONLINE.
 Home-page: https://github.com/mib1185/aiopegelonline
 Author: mib1185
 License: Apache License 2.0
 Platform: any
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -15,7 +15,9 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # aiopegelonline
 Asynchronous library to retrieve data from PEGELONLINE
+
+
```

### Comparing `aiopegelonline-0.0.1/setup.py` & `aiopegelonline-0.0.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Setup module for aiopegelonline."""
 from pathlib import Path
 
 from setuptools import find_packages, setup
 
 PROJECT_DIR = Path(__file__).parent.resolve()
 README_FILE = PROJECT_DIR / "README.md"
-VERSION = "0.0.1"
+VERSION = "0.0.2"
 
 
 setup(
     name="aiopegelonline",
     version=VERSION,
     license="Apache License 2.0",
     url="https://github.com/mib1185/aiopegelonline",
@@ -18,17 +18,15 @@
     long_description=README_FILE.read_text(encoding="utf-8"),
     long_description_content_type="text/markdown",
     packages=find_packages(),
     python_requires=">=3.9",
     package_data={"aiopegelonline": ["py.typed"]},
     zip_safe=True,
     platforms="any",
-    install_requires=list(
-        val.strip() for val in open("requirements.txt", encoding="utf-8")
-    ),
+    install_requires=["aiohttp"],
     classifiers=[
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
```

