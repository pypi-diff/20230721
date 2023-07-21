# Comparing `tmp/idem-core-functions-1.0.0.tar.gz` & `tmp/idem-core-functions-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idem-core-functions-1.0.0.tar", last modified: Mon Jun 26 15:44:03 2023, max compression
+gzip compressed data, was "idem-core-functions-2.0.0.tar", last modified: Fri Jul 21 15:31:59 2023, max compression
```

## Comparing `idem-core-functions-1.0.0.tar` & `idem-core-functions-2.0.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:44:03.840370 idem-core-functions-1.0.0/
--rw-r--r--   0 root         (0) root         (0)    11345 2023-06-26 15:43:49.000000 idem-core-functions-1.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     6551 2023-06-26 15:44:03.840370 idem-core-functions-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5737 2023-06-26 15:43:49.000000 idem-core-functions-1.0.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:44:03.836370 idem-core-functions-1.0.0/idem_core_functions/
--rw-r--r--   0 root         (0) root         (0)     1271 2023-06-26 15:43:49.000000 idem-core-functions-1.0.0/idem_core_functions/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:44:03.836370 idem-core-functions-1.0.0/idem_core_functions/exec/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:44:03.840370 idem-core-functions-1.0.0/idem_core_functions/exec/core/
--rw-r--r--   0 root         (0) root         (0)     5094 2023-06-26 15:43:49.000000 idem-core-functions-1.0.0/idem_core_functions/exec/core/collection.py
--rw-r--r--   0 root         (0) root         (0)     7624 2023-06-26 15:43:49.000000 idem-core-functions-1.0.0/idem_core_functions/exec/core/conversion.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:44:03.840370 idem-core-functions-1.0.0/idem_core_functions/exec/core/encoder/
--rw-r--r--   0 root         (0) root         (0)     2774 2023-06-26 15:43:49.000000 idem-core-functions-1.0.0/idem_core_functions/exec/core/encoder/base64.py
--rw-r--r--   0 root         (0) root         (0)     1877 2023-06-26 15:43:49.000000 idem-core-functions-1.0.0/idem_core_functions/exec/core/encoding.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:44:03.840370 idem-core-functions-1.0.0/idem_core_functions/exec/core/encryption/
--rw-r--r--   0 root         (0) root         (0)     7334 2023-06-26 15:43:49.000000 idem-core-functions-1.0.0/idem_core_functions/exec/core/encryption/gpg.py
--rw-r--r--   0 root         (0) root         (0)     1611 2023-06-26 15:43:49.000000 idem-core-functions-1.0.0/idem_core_functions/exec/core/string.py
--rw-r--r--   0 root         (0) root         (0)       18 2023-06-26 15:44:03.000000 idem-core-functions-1.0.0/idem_core_functions/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:44:03.840370 idem-core-functions-1.0.0/idem_core_functions.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6551 2023-06-26 15:44:03.000000 idem-core-functions-1.0.0/idem_core_functions.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      622 2023-06-26 15:44:03.000000 idem-core-functions-1.0.0/idem_core_functions.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-26 15:44:03.000000 idem-core-functions-1.0.0/idem_core_functions.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-06-26 15:44:03.000000 idem-core-functions-1.0.0/idem_core_functions.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       55 2023-06-26 15:44:03.000000 idem-core-functions-1.0.0/idem_core_functions.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-06-26 15:44:03.000000 idem-core-functions-1.0.0/idem_core_functions.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-06-26 15:44:03.840370 idem-core-functions-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2749 2023-06-26 15:43:49.000000 idem-core-functions-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:31:59.102599 idem-core-functions-2.0.0/
+-rw-r--r--   0 root         (0) root         (0)    11345 2023-07-21 15:31:44.000000 idem-core-functions-2.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     6552 2023-07-21 15:31:59.102599 idem-core-functions-2.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5737 2023-07-21 15:31:44.000000 idem-core-functions-2.0.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:31:59.102599 idem-core-functions-2.0.0/idem_core_functions/
+-rw-r--r--   0 root         (0) root         (0)     1271 2023-07-21 15:31:44.000000 idem-core-functions-2.0.0/idem_core_functions/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:31:59.102599 idem-core-functions-2.0.0/idem_core_functions/exec/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:31:59.102599 idem-core-functions-2.0.0/idem_core_functions/exec/core/
+-rw-r--r--   0 root         (0) root         (0)     5094 2023-07-21 15:31:44.000000 idem-core-functions-2.0.0/idem_core_functions/exec/core/collection.py
+-rw-r--r--   0 root         (0) root         (0)     7624 2023-07-21 15:31:44.000000 idem-core-functions-2.0.0/idem_core_functions/exec/core/conversion.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:31:59.102599 idem-core-functions-2.0.0/idem_core_functions/exec/core/encoder/
+-rw-r--r--   0 root         (0) root         (0)     2774 2023-07-21 15:31:44.000000 idem-core-functions-2.0.0/idem_core_functions/exec/core/encoder/base64.py
+-rw-r--r--   0 root         (0) root         (0)     1877 2023-07-21 15:31:44.000000 idem-core-functions-2.0.0/idem_core_functions/exec/core/encoding.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:31:59.102599 idem-core-functions-2.0.0/idem_core_functions/exec/core/encryption/
+-rw-r--r--   0 root         (0) root         (0)     7334 2023-07-21 15:31:44.000000 idem-core-functions-2.0.0/idem_core_functions/exec/core/encryption/gpg.py
+-rw-r--r--   0 root         (0) root         (0)     1611 2023-07-21 15:31:44.000000 idem-core-functions-2.0.0/idem_core_functions/exec/core/string.py
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-21 15:31:58.000000 idem-core-functions-2.0.0/idem_core_functions/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:31:59.102599 idem-core-functions-2.0.0/idem_core_functions.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6552 2023-07-21 15:31:59.000000 idem-core-functions-2.0.0/idem_core_functions.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      622 2023-07-21 15:31:59.000000 idem-core-functions-2.0.0/idem_core_functions.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 15:31:59.000000 idem-core-functions-2.0.0/idem_core_functions.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-07-21 15:31:59.000000 idem-core-functions-2.0.0/idem_core_functions.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       57 2023-07-21 15:31:59.000000 idem-core-functions-2.0.0/idem_core_functions.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-07-21 15:31:59.000000 idem-core-functions-2.0.0/idem_core_functions.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-21 15:31:59.102599 idem-core-functions-2.0.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2750 2023-07-21 15:31:44.000000 idem-core-functions-2.0.0/setup.py
```

### Comparing `idem-core-functions-1.0.0/LICENSE` & `idem-core-functions-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `idem-core-functions-1.0.0/PKG-INFO` & `idem-core-functions-2.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: idem-core-functions
-Version: 1.0.0
+Version: 2.0.0
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Barnali Rakshit
 Author-email: brakshit@vmware.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 5 - Production/Stable
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 ===================
 idem-core-functions
 ===================
 
@@ -54,15 +54,15 @@
 
 Getting Started
 ===============
 
 Prerequisites
 -------------
 
-* Python 3.7+
+* Python 3.8+
 * git *(if installing from source or contributing to the project)*
 
   To contribute to the project and set up your local development environment, see ``CONTRIBUTING.rst`` in the source repository for this project.
 
 Installation
 ------------
```

### Comparing `idem-core-functions-1.0.0/README.rst` & `idem-core-functions-2.0.0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 Getting Started
 ===============
 
 Prerequisites
 -------------
 
-* Python 3.7+
+* Python 3.8+
 * git *(if installing from source or contributing to the project)*
 
   To contribute to the project and set up your local development environment, see ``CONTRIBUTING.rst`` in the source repository for this project.
 
 Installation
 ------------
```

### Comparing `idem-core-functions-1.0.0/idem_core_functions/conf.py` & `idem-core-functions-2.0.0/idem_core_functions/conf.py`

 * *Files identical despite different names*

### Comparing `idem-core-functions-1.0.0/idem_core_functions/exec/core/collection.py` & `idem-core-functions-2.0.0/idem_core_functions/exec/core/collection.py`

 * *Files identical despite different names*

### Comparing `idem-core-functions-1.0.0/idem_core_functions/exec/core/conversion.py` & `idem-core-functions-2.0.0/idem_core_functions/exec/core/conversion.py`

 * *Files identical despite different names*

### Comparing `idem-core-functions-1.0.0/idem_core_functions/exec/core/encoder/base64.py` & `idem-core-functions-2.0.0/idem_core_functions/exec/core/encoder/base64.py`

 * *Files identical despite different names*

### Comparing `idem-core-functions-1.0.0/idem_core_functions/exec/core/encoding.py` & `idem-core-functions-2.0.0/idem_core_functions/exec/core/encoding.py`

 * *Files identical despite different names*

### Comparing `idem-core-functions-1.0.0/idem_core_functions/exec/core/encryption/gpg.py` & `idem-core-functions-2.0.0/idem_core_functions/exec/core/encryption/gpg.py`

 * *Files identical despite different names*

### Comparing `idem-core-functions-1.0.0/idem_core_functions/exec/core/string.py` & `idem-core-functions-2.0.0/idem_core_functions/exec/core/string.py`

 * *Files identical despite different names*

### Comparing `idem-core-functions-1.0.0/idem_core_functions.egg-info/PKG-INFO` & `idem-core-functions-2.0.0/idem_core_functions.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: idem-core-functions
-Version: 1.0.0
+Version: 2.0.0
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Barnali Rakshit
 Author-email: brakshit@vmware.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 5 - Production/Stable
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 ===================
 idem-core-functions
 ===================
 
@@ -54,15 +54,15 @@
 
 Getting Started
 ===============
 
 Prerequisites
 -------------
 
-* Python 3.7+
+* Python 3.8+
 * git *(if installing from source or contributing to the project)*
 
   To contribute to the project and set up your local development environment, see ``CONTRIBUTING.rst`` in the source repository for this project.
 
 Installation
 ------------
```

### Comparing `idem-core-functions-1.0.0/idem_core_functions.egg-info/SOURCES.txt` & `idem-core-functions-2.0.0/idem_core_functions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `idem-core-functions-1.0.0/setup.py` & `idem-core-functions-2.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,25 +70,25 @@
     url="",
     version=VERSION,
     install_requires=REQUIREMENTS,
     extras_require=REQUIREMENTS_EXTRA,
     description=DESC,
     long_description=LONG_DESC,
     long_description_content_type="text/x-rst",
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     classifiers=[
         "Environment :: Console",
         "Intended Audience :: Developers",
         "Intended Audience :: Information Technology",
         "Intended Audience :: System Administrators",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Development Status :: 5 - Production/Stable",
     ],
     packages=discover_packages(),
     entry_points={"console_scripts": [""]},
     cmdclass={"clean": Clean},
 )
```

