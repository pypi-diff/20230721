# Comparing `tmp/sklearn_mlmlm-0.0.2.tar.gz` & `tmp/sklearn_mlmlm-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sklearn_mlmlm-0.0.2.tar", last modified: Fri Jul 21 21:49:29 2023, max compression
+gzip compressed data, was "sklearn_mlmlm-0.0.3.tar", last modified: Fri Jul 21 21:54:51 2023, max compression
```

## Comparing `sklearn_mlmlm-0.0.2.tar` & `sklearn_mlmlm-0.0.3.tar`

### file list

```diff
@@ -1,23 +1,15 @@
-drwxr-xr-x   0 dfredriksen  (1000) dfredriksen  (1000)        0 2023-07-21 21:49:29.961676 sklearn_mlmlm-0.0.2/
--rwxrwxrwx   0 dfredriksen  (1000) dfredriksen  (1000)     1556 2023-07-04 20:07:57.000000 sklearn_mlmlm-0.0.2/LICENSE
--rwxrwxrwx   0 dfredriksen  (1000) dfredriksen  (1000)       26 2023-07-04 20:07:57.000000 sklearn_mlmlm-0.0.2/MANIFEST.in
--rw-r--r--   0 dfredriksen  (1000) dfredriksen  (1000)     1435 2023-07-21 21:49:29.961676 sklearn_mlmlm-0.0.2/PKG-INFO
--rwxrwxrwx   0 dfredriksen  (1000) dfredriksen  (1000)      650 2023-07-04 21:07:46.000000 sklearn_mlmlm-0.0.2/README.rst
--rwxrwxrwx   0 dfredriksen  (1000) dfredriksen  (1000)       83 2023-07-21 21:12:25.000000 sklearn_mlmlm-0.0.2/requirements.txt
--rwxrwxrwx   0 dfredriksen  (1000) dfredriksen  (1000)      148 2023-07-21 21:49:29.961676 sklearn_mlmlm-0.0.2/setup.cfg
--rwxrwxrwx   0 dfredriksen  (1000) dfredriksen  (1000)     1945 2023-07-21 21:45:53.000000 sklearn_mlmlm-0.0.2/setup.py
-drwxr-xr-x   0 dfredriksen  (1000) dfredriksen  (1000)        0 2023-07-21 21:49:29.961676 sklearn_mlmlm-0.0.2/sklearn_mlmlm.egg-info/
--rw-r--r--   0 dfredriksen  (1000) dfredriksen  (1000)     1435 2023-07-21 21:49:29.000000 sklearn_mlmlm-0.0.2/sklearn_mlmlm.egg-info/PKG-INFO
--rw-r--r--   0 dfredriksen  (1000) dfredriksen  (1000)      405 2023-07-21 21:49:29.000000 sklearn_mlmlm-0.0.2/sklearn_mlmlm.egg-info/SOURCES.txt
--rw-r--r--   0 dfredriksen  (1000) dfredriksen  (1000)        1 2023-07-21 21:49:29.000000 sklearn_mlmlm-0.0.2/sklearn_mlmlm.egg-info/dependency_links.txt
--rw-r--r--   0 dfredriksen  (1000) dfredriksen  (1000)        1 2023-07-21 21:46:38.000000 sklearn_mlmlm-0.0.2/sklearn_mlmlm.egg-info/not-zip-safe
--rw-r--r--   0 dfredriksen  (1000) dfredriksen  (1000)      119 2023-07-21 21:49:29.000000 sklearn_mlmlm-0.0.2/sklearn_mlmlm.egg-info/requires.txt
--rw-r--r--   0 dfredriksen  (1000) dfredriksen  (1000)        4 2023-07-21 21:49:29.000000 sklearn_mlmlm-0.0.2/sklearn_mlmlm.egg-info/top_level.txt
-drwxr-xr-x   0 dfredriksen  (1000) dfredriksen  (1000)        0 2023-07-21 21:49:29.961676 sklearn_mlmlm-0.0.2/src/
--rwxrwxrwx   0 dfredriksen  (1000) dfredriksen  (1000)      137 2023-07-04 20:12:01.000000 sklearn_mlmlm-0.0.2/src/__init__.py
--rwxrwxrwx   0 dfredriksen  (1000) dfredriksen  (1000)       21 2023-07-21 21:49:26.000000 sklearn_mlmlm-0.0.2/src/_version.py
--rwxrwxrwx   0 dfredriksen  (1000) dfredriksen  (1000)     7858 2023-07-21 21:14:25.000000 sklearn_mlmlm-0.0.2/src/mlmlm.py
-drwxr-xr-x   0 dfredriksen  (1000) dfredriksen  (1000)        0 2023-07-21 21:49:29.961676 sklearn_mlmlm-0.0.2/src/tests/
--rwxrwxrwx   0 dfredriksen  (1000) dfredriksen  (1000)        0 2023-07-04 20:07:57.000000 sklearn_mlmlm-0.0.2/src/tests/__init__.py
--rwxrwxrwx   0 dfredriksen  (1000) dfredriksen  (1000)      387 2023-07-04 20:16:39.000000 sklearn_mlmlm-0.0.2/src/tests/test_common.py
--rwxrwxrwx   0 dfredriksen  (1000) dfredriksen  (1000)      602 2023-07-04 20:17:33.000000 sklearn_mlmlm-0.0.2/src/tests/test_template.py
+drwxr-xr-x   0 dfredriksen  (1000) dfredriksen  (1000)        0 2023-07-21 21:54:51.329295 sklearn_mlmlm-0.0.3/
+-rwxrwxrwx   0 dfredriksen  (1000) dfredriksen  (1000)     1556 2023-07-04 20:07:57.000000 sklearn_mlmlm-0.0.3/LICENSE
+-rwxrwxrwx   0 dfredriksen  (1000) dfredriksen  (1000)       26 2023-07-04 20:07:57.000000 sklearn_mlmlm-0.0.3/MANIFEST.in
+-rw-r--r--   0 dfredriksen  (1000) dfredriksen  (1000)     1435 2023-07-21 21:54:51.329295 sklearn_mlmlm-0.0.3/PKG-INFO
+-rwxrwxrwx   0 dfredriksen  (1000) dfredriksen  (1000)      650 2023-07-04 21:07:46.000000 sklearn_mlmlm-0.0.3/README.rst
+-rwxrwxrwx   0 dfredriksen  (1000) dfredriksen  (1000)       83 2023-07-21 21:12:25.000000 sklearn_mlmlm-0.0.3/requirements.txt
+-rwxrwxrwx   0 dfredriksen  (1000) dfredriksen  (1000)      148 2023-07-21 21:54:51.329295 sklearn_mlmlm-0.0.3/setup.cfg
+-rwxrwxrwx   0 dfredriksen  (1000) dfredriksen  (1000)     1962 2023-07-21 21:54:42.000000 sklearn_mlmlm-0.0.3/setup.py
+drwxr-xr-x   0 dfredriksen  (1000) dfredriksen  (1000)        0 2023-07-21 21:54:51.329295 sklearn_mlmlm-0.0.3/sklearn_mlmlm.egg-info/
+-rw-r--r--   0 dfredriksen  (1000) dfredriksen  (1000)     1435 2023-07-21 21:54:51.000000 sklearn_mlmlm-0.0.3/sklearn_mlmlm.egg-info/PKG-INFO
+-rw-r--r--   0 dfredriksen  (1000) dfredriksen  (1000)      286 2023-07-21 21:54:51.000000 sklearn_mlmlm-0.0.3/sklearn_mlmlm.egg-info/SOURCES.txt
+-rw-r--r--   0 dfredriksen  (1000) dfredriksen  (1000)        1 2023-07-21 21:54:51.000000 sklearn_mlmlm-0.0.3/sklearn_mlmlm.egg-info/dependency_links.txt
+-rw-r--r--   0 dfredriksen  (1000) dfredriksen  (1000)        1 2023-07-21 21:46:38.000000 sklearn_mlmlm-0.0.3/sklearn_mlmlm.egg-info/not-zip-safe
+-rw-r--r--   0 dfredriksen  (1000) dfredriksen  (1000)      119 2023-07-21 21:54:51.000000 sklearn_mlmlm-0.0.3/sklearn_mlmlm.egg-info/requires.txt
+-rw-r--r--   0 dfredriksen  (1000) dfredriksen  (1000)        1 2023-07-21 21:54:51.000000 sklearn_mlmlm-0.0.3/sklearn_mlmlm.egg-info/top_level.txt
```

### Comparing `sklearn_mlmlm-0.0.2/LICENSE` & `sklearn_mlmlm-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sklearn_mlmlm-0.0.2/PKG-INFO` & `sklearn_mlmlm-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sklearn_mlmlm
-Version: 0.0.2
+Version: 0.0.3
 Summary: A python and sklearn compatible implementation of ML-MLM.
 Home-page: https://github.com/quantyra/scikit-mlmlm
 Download-URL: https://github.com/quantyra/scikit-mlmlm
 Maintainer: Daniel E Fredriksen
 Maintainer-email: dfredriksen@quantyra.org
 License: new BSD
 Classifier: Intended Audience :: Science/Research
```

### Comparing `sklearn_mlmlm-0.0.2/README.rst` & `sklearn_mlmlm-0.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `sklearn_mlmlm-0.0.2/setup.py` & `sklearn_mlmlm-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import codecs
 import os
 
 from setuptools import find_packages, setup
 
 # get __version__ from _version.py
-ver_file = os.path.join('src', '_version.py')
+ver_file = os.path.join('src', 'sklearn_mlmlm', '_version.py')
 with open(ver_file) as f:
     exec(f.read())
 
 DISTNAME = 'sklearn_mlmlm'
 DESCRIPTION = 'A python and sklearn compatible implementation of ML-MLM.'
 with codecs.open('README.rst', encoding='utf-8-sig') as f:
     LONG_DESCRIPTION = f.read()
```

### Comparing `sklearn_mlmlm-0.0.2/sklearn_mlmlm.egg-info/PKG-INFO` & `sklearn_mlmlm-0.0.3/sklearn_mlmlm.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sklearn-mlmlm
-Version: 0.0.2
+Version: 0.0.3
 Summary: A python and sklearn compatible implementation of ML-MLM.
 Home-page: https://github.com/quantyra/scikit-mlmlm
 Download-URL: https://github.com/quantyra/scikit-mlmlm
 Maintainer: Daniel E Fredriksen
 Maintainer-email: dfredriksen@quantyra.org
 License: new BSD
 Classifier: Intended Audience :: Science/Research
```

