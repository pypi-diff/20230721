# Comparing `tmp/idem-tls-1.0.2.tar.gz` & `tmp/idem-tls-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idem-tls-1.0.2.tar", last modified: Thu Jul 13 16:02:45 2023, max compression
+gzip compressed data, was "idem-tls-2.0.0.tar", last modified: Fri Jul 21 19:17:33 2023, max compression
```

## Comparing `idem-tls-1.0.2.tar` & `idem-tls-2.0.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 16:02:45.194332 idem-tls-1.0.2/
--rw-r--r--   0 root         (0) root         (0)    11345 2023-07-13 16:02:31.000000 idem-tls-1.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5173 2023-07-13 16:02:45.194332 idem-tls-1.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4370 2023-07-13 16:02:31.000000 idem-tls-1.0.2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 16:02:45.190332 idem-tls-1.0.2/idem_tls/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 16:02:45.190332 idem-tls-1.0.2/idem_tls/acct/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 16:02:45.194332 idem-tls-1.0.2/idem_tls/acct/tls/
--rw-r--r--   0 root         (0) root         (0)      485 2023-07-13 16:02:31.000000 idem-tls-1.0.2/idem_tls/acct/tls/init.py
--rw-r--r--   0 root         (0) root         (0)     1319 2023-07-13 16:02:31.000000 idem-tls-1.0.2/idem_tls/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 16:02:45.190332 idem-tls-1.0.2/idem_tls/exec/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 16:02:45.194332 idem-tls-1.0.2/idem_tls/exec/tls/
--rw-r--r--   0 root         (0) root         (0)     5326 2023-07-13 16:02:31.000000 idem-tls-1.0.2/idem_tls/exec/tls/certificate.py
--rw-r--r--   0 root         (0) root         (0)      167 2023-07-13 16:02:31.000000 idem-tls-1.0.2/idem_tls/exec/tls/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 16:02:45.190332 idem-tls-1.0.2/idem_tls/states/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 16:02:45.194332 idem-tls-1.0.2/idem_tls/states/tls/
--rw-r--r--   0 root         (0) root         (0)      169 2023-07-13 16:02:31.000000 idem-tls-1.0.2/idem_tls/states/tls/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 16:02:45.190332 idem-tls-1.0.2/idem_tls/tool/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 16:02:45.194332 idem-tls-1.0.2/idem_tls/tool/tls/
--rw-r--r--   0 root         (0) root         (0)     2358 2023-07-13 16:02:31.000000 idem-tls-1.0.2/idem_tls/tool/tls/certificate.py
--rw-r--r--   0 root         (0) root         (0)       18 2023-07-13 16:02:44.000000 idem-tls-1.0.2/idem_tls/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 16:02:45.194332 idem-tls-1.0.2/idem_tls.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5173 2023-07-13 16:02:45.000000 idem-tls-1.0.2/idem_tls.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      414 2023-07-13 16:02:45.000000 idem-tls-1.0.2/idem_tls.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 16:02:45.000000 idem-tls-1.0.2/idem_tls.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-07-13 16:02:45.000000 idem-tls-1.0.2/idem_tls.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       69 2023-07-13 16:02:45.000000 idem-tls-1.0.2/idem_tls.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-07-13 16:02:45.000000 idem-tls-1.0.2/idem_tls.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-07-13 16:02:45.194332 idem-tls-1.0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2716 2023-07-13 16:02:31.000000 idem-tls-1.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 19:17:33.185519 idem-tls-2.0.0/
+-rw-r--r--   0 root         (0) root         (0)    11345 2023-07-21 19:17:18.000000 idem-tls-2.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     5174 2023-07-21 19:17:33.185519 idem-tls-2.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4370 2023-07-21 19:17:18.000000 idem-tls-2.0.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 19:17:33.185519 idem-tls-2.0.0/idem_tls/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 19:17:33.185519 idem-tls-2.0.0/idem_tls/acct/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 19:17:33.185519 idem-tls-2.0.0/idem_tls/acct/tls/
+-rw-r--r--   0 root         (0) root         (0)      485 2023-07-21 19:17:18.000000 idem-tls-2.0.0/idem_tls/acct/tls/init.py
+-rw-r--r--   0 root         (0) root         (0)     1319 2023-07-21 19:17:18.000000 idem-tls-2.0.0/idem_tls/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 19:17:33.185519 idem-tls-2.0.0/idem_tls/exec/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 19:17:33.185519 idem-tls-2.0.0/idem_tls/exec/tls/
+-rw-r--r--   0 root         (0) root         (0)     5326 2023-07-21 19:17:18.000000 idem-tls-2.0.0/idem_tls/exec/tls/certificate.py
+-rw-r--r--   0 root         (0) root         (0)      167 2023-07-21 19:17:18.000000 idem-tls-2.0.0/idem_tls/exec/tls/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 19:17:33.185519 idem-tls-2.0.0/idem_tls/states/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 19:17:33.185519 idem-tls-2.0.0/idem_tls/states/tls/
+-rw-r--r--   0 root         (0) root         (0)      169 2023-07-21 19:17:18.000000 idem-tls-2.0.0/idem_tls/states/tls/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 19:17:33.185519 idem-tls-2.0.0/idem_tls/tool/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 19:17:33.185519 idem-tls-2.0.0/idem_tls/tool/tls/
+-rw-r--r--   0 root         (0) root         (0)     2358 2023-07-21 19:17:18.000000 idem-tls-2.0.0/idem_tls/tool/tls/certificate.py
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-21 19:17:32.000000 idem-tls-2.0.0/idem_tls/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 19:17:33.185519 idem-tls-2.0.0/idem_tls.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5174 2023-07-21 19:17:33.000000 idem-tls-2.0.0/idem_tls.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      414 2023-07-21 19:17:33.000000 idem-tls-2.0.0/idem_tls.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 19:17:33.000000 idem-tls-2.0.0/idem_tls.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-07-21 19:17:33.000000 idem-tls-2.0.0/idem_tls.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       86 2023-07-21 19:17:33.000000 idem-tls-2.0.0/idem_tls.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-07-21 19:17:33.000000 idem-tls-2.0.0/idem_tls.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-21 19:17:33.185519 idem-tls-2.0.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2717 2023-07-21 19:17:18.000000 idem-tls-2.0.0/setup.py
```

### Comparing `idem-tls-1.0.2/LICENSE` & `idem-tls-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `idem-tls-1.0.2/PKG-INFO` & `idem-tls-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: idem-tls
-Version: 1.0.2
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
 
 ========
 idem-tls
 ========
 
@@ -56,15 +56,15 @@
 
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

### Comparing `idem-tls-1.0.2/README.rst` & `idem-tls-2.0.0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
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

### Comparing `idem-tls-1.0.2/idem_tls/conf.py` & `idem-tls-2.0.0/idem_tls/conf.py`

 * *Files identical despite different names*

### Comparing `idem-tls-1.0.2/idem_tls/exec/tls/certificate.py` & `idem-tls-2.0.0/idem_tls/exec/tls/certificate.py`

 * *Files identical despite different names*

### Comparing `idem-tls-1.0.2/idem_tls/tool/tls/certificate.py` & `idem-tls-2.0.0/idem_tls/tool/tls/certificate.py`

 * *Files identical despite different names*

### Comparing `idem-tls-1.0.2/idem_tls.egg-info/PKG-INFO` & `idem-tls-2.0.0/idem_tls.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: idem-tls
-Version: 1.0.2
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
 
 ========
 idem-tls
 ========
 
@@ -56,15 +56,15 @@
 
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

### Comparing `idem-tls-1.0.2/setup.py` & `idem-tls-2.0.0/setup.py`

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

