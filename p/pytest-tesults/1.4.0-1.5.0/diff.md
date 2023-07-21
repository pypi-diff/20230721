# Comparing `tmp/pytest-tesults-1.4.0.tar.gz` & `tmp/pytest-tesults-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-tesults-1.4.0.tar", last modified: Fri Dec 23 17:20:28 2022, max compression
+gzip compressed data, was "pytest-tesults-1.5.0.tar", last modified: Fri Jul 21 00:17:17 2023, max compression
```

## Comparing `pytest-tesults-1.4.0.tar` & `pytest-tesults-1.5.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2022-12-23 17:20:28.766608 pytest-tesults-1.4.0/
--rw-r--r--   0 admin      (501) staff       (20)     1075 2022-12-23 17:14:29.000000 pytest-tesults-1.4.0/LICENSE
--rw-r--r--   0 admin      (501) staff       (20)       97 2019-03-26 12:36:50.000000 pytest-tesults-1.4.0/MANIFEST.in
--rw-r--r--   0 admin      (501) staff       (20)     2204 2022-12-23 17:20:28.766147 pytest-tesults-1.4.0/PKG-INFO
--rw-r--r--   0 admin      (501) staff       (20)      935 2021-07-31 18:31:06.000000 pytest-tesults-1.4.0/README.rst
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2022-12-23 17:20:28.765563 pytest-tesults-1.4.0/pytest_tesults.egg-info/
--rw-r--r--   0 admin      (501) staff       (20)     2204 2022-12-23 17:20:28.000000 pytest-tesults-1.4.0/pytest_tesults.egg-info/PKG-INFO
--rw-r--r--   0 admin      (501) staff       (20)      287 2022-12-23 17:20:28.000000 pytest-tesults-1.4.0/pytest_tesults.egg-info/SOURCES.txt
--rw-r--r--   0 admin      (501) staff       (20)        1 2022-12-23 17:20:28.000000 pytest-tesults-1.4.0/pytest_tesults.egg-info/dependency_links.txt
--rw-r--r--   0 admin      (501) staff       (20)       36 2022-12-23 17:20:28.000000 pytest-tesults-1.4.0/pytest_tesults.egg-info/entry_points.txt
--rw-r--r--   0 admin      (501) staff       (20)       22 2022-12-23 17:20:28.000000 pytest-tesults-1.4.0/pytest_tesults.egg-info/requires.txt
--rw-r--r--   0 admin      (501) staff       (20)       15 2022-12-23 17:20:28.000000 pytest-tesults-1.4.0/pytest_tesults.egg-info/top_level.txt
--rw-r--r--   0 admin      (501) staff       (20)    12470 2022-12-23 17:15:37.000000 pytest-tesults-1.4.0/pytest_tesults.py
--rw-r--r--   0 admin      (501) staff       (20)       38 2022-12-23 17:20:28.766757 pytest-tesults-1.4.0/setup.cfg
--rw-r--r--   0 admin      (501) staff       (20)     1785 2022-12-23 17:14:55.000000 pytest-tesults-1.4.0/setup.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-21 00:17:17.941432 pytest-tesults-1.5.0/
+-rw-r--r--   0 admin      (501) staff       (20)     1075 2023-07-20 23:44:46.000000 pytest-tesults-1.5.0/LICENSE
+-rw-r--r--   0 admin      (501) staff       (20)       97 2019-03-26 12:36:50.000000 pytest-tesults-1.5.0/MANIFEST.in
+-rw-r--r--   0 admin      (501) staff       (20)     2204 2023-07-21 00:17:17.941273 pytest-tesults-1.5.0/PKG-INFO
+-rw-r--r--   0 admin      (501) staff       (20)      935 2021-07-31 18:31:06.000000 pytest-tesults-1.5.0/README.rst
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-21 00:17:17.941018 pytest-tesults-1.5.0/pytest_tesults.egg-info/
+-rw-r--r--   0 admin      (501) staff       (20)     2204 2023-07-21 00:17:17.000000 pytest-tesults-1.5.0/pytest_tesults.egg-info/PKG-INFO
+-rw-r--r--   0 admin      (501) staff       (20)      287 2023-07-21 00:17:17.000000 pytest-tesults-1.5.0/pytest_tesults.egg-info/SOURCES.txt
+-rw-r--r--   0 admin      (501) staff       (20)        1 2023-07-21 00:17:17.000000 pytest-tesults-1.5.0/pytest_tesults.egg-info/dependency_links.txt
+-rw-r--r--   0 admin      (501) staff       (20)       36 2023-07-21 00:17:17.000000 pytest-tesults-1.5.0/pytest_tesults.egg-info/entry_points.txt
+-rw-r--r--   0 admin      (501) staff       (20)       22 2023-07-21 00:17:17.000000 pytest-tesults-1.5.0/pytest_tesults.egg-info/requires.txt
+-rw-r--r--   0 admin      (501) staff       (20)       15 2023-07-21 00:17:17.000000 pytest-tesults-1.5.0/pytest_tesults.egg-info/top_level.txt
+-rw-r--r--   0 admin      (501) staff       (20)    12546 2023-07-20 23:46:22.000000 pytest-tesults-1.5.0/pytest_tesults.py
+-rw-r--r--   0 admin      (501) staff       (20)       38 2023-07-21 00:17:17.941478 pytest-tesults-1.5.0/setup.cfg
+-rw-r--r--   0 admin      (501) staff       (20)     1785 2023-07-20 23:45:06.000000 pytest-tesults-1.5.0/setup.py
```

### Comparing `pytest-tesults-1.4.0/LICENSE` & `pytest-tesults-1.5.0/LICENSE`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 The MIT License (MIT)
 
-Copyright (c) 2022 Tesults
+Copyright (c) 2023 Tesults
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `pytest-tesults-1.4.0/PKG-INFO` & `pytest-tesults-1.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-tesults
-Version: 1.4.0
+Version: 1.5.0
 Summary: Tesults plugin for pytest
 Home-page: https://www.tesults.com/docs/pytest
 Author: Tesults
 Author-email: help@tesults.com
 Maintainer: Tesults
 Maintainer-email: help@tesults.com
 License: MIT
```

### Comparing `pytest-tesults-1.4.0/README.rst` & `pytest-tesults-1.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `pytest-tesults-1.4.0/pytest_tesults.egg-info/PKG-INFO` & `pytest-tesults-1.5.0/pytest_tesults.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-tesults
-Version: 1.4.0
+Version: 1.5.0
 Summary: Tesults plugin for pytest
 Home-page: https://www.tesults.com/docs/pytest
 Author: Tesults
 Author-email: help@tesults.com
 Maintainer: Tesults
 Maintainer-email: help@tesults.com
 License: MIT
```

### Comparing `pytest-tesults-1.4.0/pytest_tesults.py` & `pytest-tesults-1.5.0/pytest_tesults.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from _pytest.runner import runtestprotocol
 
 
 # The data variable holds test results and tesults target information, at the end of test run it is uploaded to tesults for reporting.
 data = {
   'target': 'token',
   'results': { 'cases': [] },
-  'metadata': {'integration_name': 'pytest-tesults', 'integration_version': '1.4.0', 'test_framework': 'pytest' }
+  'metadata': {'integration_name': 'pytest-tesults', 'integration_version': '1.5.0', 'test_framework': 'pytest' }
 }
 
 startTimes = {}
 
 disabled = False
 nosuites = False
 filespath = None
@@ -287,15 +287,15 @@
   global disabled
   if (disabled == True):
     return
   global data
   global saveStdOut
   reports = runtestprotocol(item, nextitem=nextitem)
   for report in reports:
-    if report.when == 'call':
+    if report.skipped == True or report.when == 'call':
       name = item.name
       suite = None
       try:
         suite = item.get_marker('suite')
         if (suite):
           if len(suite.args) > 0:
             suite = suite.args[0] #extract val from marker
@@ -317,18 +317,19 @@
           suite = str(item.parent.name)
           suite = suite.rpartition("/")[2]
           suite = suite.rpartition(".py")[0]
       testcase = {
       'name': name, 
       'result': tesultsFriendlyResult(report.outcome),
       'rawResult': report.outcome,
-      'start': startTimes[item.nodeid],
-      'end': int(round(time.time() * 1000)),
-      'reason': reasonForFailure(report)
+      'reason': reasonForFailure(report),
+      'end': int(round(time.time() * 1000))
       }
+      if item.nodeid in startTimes:
+        testcase['start'] = startTimes[item.nodeid]  
       if (suite):
         testcase['suite'] = suite
       if saveStdOut == True:
         try:
           if item._report_sections:
             report_sections = item._report_sections
             for section in report_sections:
```

### Comparing `pytest-tesults-1.4.0/setup.py` & `pytest-tesults-1.5.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 def read(fname):
     file_path = os.path.join(os.path.dirname(__file__), fname)
     return codecs.open(file_path, encoding='utf-8').read()
 
 
 setup(
     name='pytest-tesults',
-    version='1.4.0',
+    version='1.5.0',
     author='Tesults',
     author_email='help@tesults.com',
     maintainer='Tesults',
     maintainer_email='help@tesults.com',
     license='MIT',
     url='https://www.tesults.com/docs/pytest',
     description='Tesults plugin for pytest',
```

