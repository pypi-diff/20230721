# Comparing `tmp/sn_test-0.1.0.tar.gz` & `tmp/sn_test-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sn_test-0.1.0.tar", last modified: Fri Jul 21 05:20:04 2023, max compression
+gzip compressed data, was "dist/sn_test-0.1.3.tar", last modified: Fri Jul 21 06:00:17 2023, max compression
```

## Comparing `sn_test-0.1.0.tar` & `sn_test-0.1.3.tar`

### file list

```diff
@@ -1,10 +1,13 @@
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-21 05:20:04.000000 sn_test-0.1.0/
--rw-r--r--   0 mac        (501) staff       (20)      620 2023-07-21 05:20:04.000000 sn_test-0.1.0/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)     3318 2023-07-21 05:19:20.000000 sn_test-0.1.0/set_up.py
--rw-r--r--   0 mac        (501) staff       (20)       38 2023-07-21 05:20:04.000000 sn_test-0.1.0/setup.cfg
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-21 05:20:04.000000 sn_test-0.1.0/sn_test.egg-info/
--rw-r--r--   0 mac        (501) staff       (20)      620 2023-07-21 05:20:04.000000 sn_test-0.1.0/sn_test.egg-info/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)      163 2023-07-21 05:20:04.000000 sn_test-0.1.0/sn_test.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (501) staff       (20)        1 2023-07-21 05:20:04.000000 sn_test-0.1.0/sn_test.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (501) staff       (20)       19 2023-07-21 05:20:04.000000 sn_test-0.1.0/sn_test.egg-info/requires.txt
--rw-r--r--   0 mac        (501) staff       (20)        1 2023-07-21 05:20:04.000000 sn_test-0.1.0/sn_test.egg-info/top_level.txt
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-21 06:00:17.000000 sn_test-0.1.3/
+-rw-r--r--   0 mac        (501) staff       (20)      605 2023-07-21 06:00:17.000000 sn_test-0.1.3/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)     3180 2023-07-21 05:59:15.000000 sn_test-0.1.3/set_up.py
+-rw-r--r--   0 mac        (501) staff       (20)       38 2023-07-21 06:00:17.000000 sn_test-0.1.3/setup.cfg
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-21 06:00:17.000000 sn_test-0.1.3/sn_test/
+-rw-r--r--   0 mac        (501) staff       (20)        0 2023-07-21 05:57:44.000000 sn_test-0.1.3/sn_test/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)      211 2023-07-21 05:58:51.000000 sn_test-0.1.3/sn_test/sn_test.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-21 06:00:17.000000 sn_test-0.1.3/sn_test.egg-info/
+-rw-r--r--   0 mac        (501) staff       (20)      605 2023-07-21 06:00:17.000000 sn_test-0.1.3/sn_test.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)      202 2023-07-21 06:00:17.000000 sn_test-0.1.3/sn_test.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (501) staff       (20)        1 2023-07-21 06:00:17.000000 sn_test-0.1.3/sn_test.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (501) staff       (20)       19 2023-07-21 06:00:17.000000 sn_test-0.1.3/sn_test.egg-info/requires.txt
+-rw-r--r--   0 mac        (501) staff       (20)        8 2023-07-21 06:00:17.000000 sn_test-0.1.3/sn_test.egg-info/top_level.txt
```

### Comparing `sn_test-0.1.0/PKG-INFO` & `sn_test-0.1.3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: sn_test
-Version: 0.1.0
+Version: 0.1.3
 Summary: shuainan test
 Home-page: https://github.com/me/myproject
-Author: Soul
+Author: shuainan
 Author-email: 15294627382@163.com
 License: MIT
-Description: 
-        test
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
+
+
+test 欢迎来到世界
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `sn_test-0.1.0/set_up.py` & `sn_test-0.1.3/set_up.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 from setuptools import find_packages, setup, Command
 
 # Package meta-data.
 NAME = 'sn_test'
 DESCRIPTION = 'shuainan test'
 URL = 'https://github.com/me/myproject'
 EMAIL = '15294627382@163.com'
-AUTHOR = 'Soul'
+AUTHOR = 'shuainan'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.1.0'
+VERSION = '0.1.3'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'requests',
     'websocket'
 ]
 
@@ -95,27 +95,23 @@
     description=DESCRIPTION,
     long_description=long_description,
     long_description_content_type='text/markdown',
     author=AUTHOR,
     author_email=EMAIL,
     python_requires=REQUIRES_PYTHON,
     url=URL,
-    packages=find_packages(exclude=["tests", "*.tests", "*.tests.*", "tests.*"]),
+    packages=find_packages(),
     install_requires=REQUIRED,
     extras_require=EXTRAS,
     include_package_data=True,
     license='MIT',
     classifiers=[
         # Trove classifiers
         # Full list: https://pypi.python.org/pypi?%3Aaction=list_classifiers
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: Implementation :: CPython',
         'Programming Language :: Python :: Implementation :: PyPy'
-    ],
-    # $ setup.py publish support.
-    cmdclass={
-        'upload': UploadCommand,
-    },
+    ]
 )
```

### Comparing `sn_test-0.1.0/sn_test.egg-info/PKG-INFO` & `sn_test-0.1.3/sn_test.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: sn-test
-Version: 0.1.0
+Version: 0.1.3
 Summary: shuainan test
 Home-page: https://github.com/me/myproject
-Author: Soul
+Author: shuainan
 Author-email: 15294627382@163.com
 License: MIT
-Description: 
-        test
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
+
+
+test 欢迎来到世界
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

