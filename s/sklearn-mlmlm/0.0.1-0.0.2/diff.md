# Comparing `tmp/sklearn-mlmlm-0.0.1.tar.gz` & `tmp/sklearn_mlmlm-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sklearn-mlmlm-0.0.1.tar", last modified: Fri Jul 21 21:22:55 2023, max compression
+gzip compressed data, was "sklearn_mlmlm-0.0.2.tar", last modified: Fri Jul 21 21:49:29 2023, max compression
```

## Comparing `sklearn-mlmlm-0.0.1.tar` & `sklearn_mlmlm-0.0.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 dfredriksen  (1000) dfredriksen  (1000)        0 2023-07-21 21:22:55.267486 sklearn-mlmlm-0.0.1/
--rwxrwxrwx   0 dfredriksen  (1000) dfredriksen  (1000)     1556 2023-07-04 20:07:57.000000 sklearn-mlmlm-0.0.1/LICENSE
--rwxrwxrwx   0 dfredriksen  (1000) dfredriksen  (1000)       26 2023-07-04 20:07:57.000000 sklearn-mlmlm-0.0.1/MANIFEST.in
--rw-r--r--   0 dfredriksen  (1000) dfredriksen  (1000)     1435 2023-07-21 21:22:55.267486 sklearn-mlmlm-0.0.1/PKG-INFO
--rwxrwxrwx   0 dfredriksen  (1000) dfredriksen  (1000)      650 2023-07-04 21:07:46.000000 sklearn-mlmlm-0.0.1/README.rst
--rwxrwxrwx   0 dfredriksen  (1000) dfredriksen  (1000)       83 2023-07-21 21:12:25.000000 sklearn-mlmlm-0.0.1/requirements.txt
--rwxrwxrwx   0 dfredriksen  (1000) dfredriksen  (1000)      148 2023-07-21 21:22:55.267486 sklearn-mlmlm-0.0.1/setup.cfg
--rwxrwxrwx   0 dfredriksen  (1000) dfredriksen  (1000)     1945 2023-07-21 21:13:44.000000 sklearn-mlmlm-0.0.1/setup.py
-drwxr-xr-x   0 dfredriksen  (1000) dfredriksen  (1000)        0 2023-07-21 21:22:55.257486 sklearn-mlmlm-0.0.1/sklearn_mlmlm.egg-info/
--rw-r--r--   0 dfredriksen  (1000) dfredriksen  (1000)     1435 2023-07-21 21:22:55.000000 sklearn-mlmlm-0.0.1/sklearn_mlmlm.egg-info/PKG-INFO
--rw-r--r--   0 dfredriksen  (1000) dfredriksen  (1000)      405 2023-07-21 21:22:55.000000 sklearn-mlmlm-0.0.1/sklearn_mlmlm.egg-info/SOURCES.txt
--rw-r--r--   0 dfredriksen  (1000) dfredriksen  (1000)        1 2023-07-21 21:22:55.000000 sklearn-mlmlm-0.0.1/sklearn_mlmlm.egg-info/dependency_links.txt
--rw-r--r--   0 dfredriksen  (1000) dfredriksen  (1000)        1 2023-07-21 21:22:54.000000 sklearn-mlmlm-0.0.1/sklearn_mlmlm.egg-info/not-zip-safe
--rw-r--r--   0 dfredriksen  (1000) dfredriksen  (1000)      119 2023-07-21 21:22:55.000000 sklearn-mlmlm-0.0.1/sklearn_mlmlm.egg-info/requires.txt
--rw-r--r--   0 dfredriksen  (1000) dfredriksen  (1000)        4 2023-07-21 21:22:55.000000 sklearn-mlmlm-0.0.1/sklearn_mlmlm.egg-info/top_level.txt
-drwxr-xr-x   0 dfredriksen  (1000) dfredriksen  (1000)        0 2023-07-21 21:22:55.267486 sklearn-mlmlm-0.0.1/src/
--rwxrwxrwx   0 dfredriksen  (1000) dfredriksen  (1000)      137 2023-07-04 20:12:01.000000 sklearn-mlmlm-0.0.1/src/__init__.py
--rwxrwxrwx   0 dfredriksen  (1000) dfredriksen  (1000)       21 2023-07-04 20:10:27.000000 sklearn-mlmlm-0.0.1/src/_version.py
--rwxrwxrwx   0 dfredriksen  (1000) dfredriksen  (1000)     7858 2023-07-21 21:14:25.000000 sklearn-mlmlm-0.0.1/src/mlmlm.py
-drwxr-xr-x   0 dfredriksen  (1000) dfredriksen  (1000)        0 2023-07-21 21:22:55.267486 sklearn-mlmlm-0.0.1/src/tests/
--rwxrwxrwx   0 dfredriksen  (1000) dfredriksen  (1000)        0 2023-07-04 20:07:57.000000 sklearn-mlmlm-0.0.1/src/tests/__init__.py
--rwxrwxrwx   0 dfredriksen  (1000) dfredriksen  (1000)      387 2023-07-04 20:16:39.000000 sklearn-mlmlm-0.0.1/src/tests/test_common.py
--rwxrwxrwx   0 dfredriksen  (1000) dfredriksen  (1000)      602 2023-07-04 20:17:33.000000 sklearn-mlmlm-0.0.1/src/tests/test_template.py
+drwxr-xr-x   0 dfredriksen  (1000) dfredriksen  (1000)        0 2023-07-21 21:49:29.961676 sklearn_mlmlm-0.0.2/
+-rwxrwxrwx   0 dfredriksen  (1000) dfredriksen  (1000)     1556 2023-07-04 20:07:57.000000 sklearn_mlmlm-0.0.2/LICENSE
+-rwxrwxrwx   0 dfredriksen  (1000) dfredriksen  (1000)       26 2023-07-04 20:07:57.000000 sklearn_mlmlm-0.0.2/MANIFEST.in
+-rw-r--r--   0 dfredriksen  (1000) dfredriksen  (1000)     1435 2023-07-21 21:49:29.961676 sklearn_mlmlm-0.0.2/PKG-INFO
+-rwxrwxrwx   0 dfredriksen  (1000) dfredriksen  (1000)      650 2023-07-04 21:07:46.000000 sklearn_mlmlm-0.0.2/README.rst
+-rwxrwxrwx   0 dfredriksen  (1000) dfredriksen  (1000)       83 2023-07-21 21:12:25.000000 sklearn_mlmlm-0.0.2/requirements.txt
+-rwxrwxrwx   0 dfredriksen  (1000) dfredriksen  (1000)      148 2023-07-21 21:49:29.961676 sklearn_mlmlm-0.0.2/setup.cfg
+-rwxrwxrwx   0 dfredriksen  (1000) dfredriksen  (1000)     1945 2023-07-21 21:45:53.000000 sklearn_mlmlm-0.0.2/setup.py
+drwxr-xr-x   0 dfredriksen  (1000) dfredriksen  (1000)        0 2023-07-21 21:49:29.961676 sklearn_mlmlm-0.0.2/sklearn_mlmlm.egg-info/
+-rw-r--r--   0 dfredriksen  (1000) dfredriksen  (1000)     1435 2023-07-21 21:49:29.000000 sklearn_mlmlm-0.0.2/sklearn_mlmlm.egg-info/PKG-INFO
+-rw-r--r--   0 dfredriksen  (1000) dfredriksen  (1000)      405 2023-07-21 21:49:29.000000 sklearn_mlmlm-0.0.2/sklearn_mlmlm.egg-info/SOURCES.txt
+-rw-r--r--   0 dfredriksen  (1000) dfredriksen  (1000)        1 2023-07-21 21:49:29.000000 sklearn_mlmlm-0.0.2/sklearn_mlmlm.egg-info/dependency_links.txt
+-rw-r--r--   0 dfredriksen  (1000) dfredriksen  (1000)        1 2023-07-21 21:46:38.000000 sklearn_mlmlm-0.0.2/sklearn_mlmlm.egg-info/not-zip-safe
+-rw-r--r--   0 dfredriksen  (1000) dfredriksen  (1000)      119 2023-07-21 21:49:29.000000 sklearn_mlmlm-0.0.2/sklearn_mlmlm.egg-info/requires.txt
+-rw-r--r--   0 dfredriksen  (1000) dfredriksen  (1000)        4 2023-07-21 21:49:29.000000 sklearn_mlmlm-0.0.2/sklearn_mlmlm.egg-info/top_level.txt
+drwxr-xr-x   0 dfredriksen  (1000) dfredriksen  (1000)        0 2023-07-21 21:49:29.961676 sklearn_mlmlm-0.0.2/src/
+-rwxrwxrwx   0 dfredriksen  (1000) dfredriksen  (1000)      137 2023-07-04 20:12:01.000000 sklearn_mlmlm-0.0.2/src/__init__.py
+-rwxrwxrwx   0 dfredriksen  (1000) dfredriksen  (1000)       21 2023-07-21 21:49:26.000000 sklearn_mlmlm-0.0.2/src/_version.py
+-rwxrwxrwx   0 dfredriksen  (1000) dfredriksen  (1000)     7858 2023-07-21 21:14:25.000000 sklearn_mlmlm-0.0.2/src/mlmlm.py
+drwxr-xr-x   0 dfredriksen  (1000) dfredriksen  (1000)        0 2023-07-21 21:49:29.961676 sklearn_mlmlm-0.0.2/src/tests/
+-rwxrwxrwx   0 dfredriksen  (1000) dfredriksen  (1000)        0 2023-07-04 20:07:57.000000 sklearn_mlmlm-0.0.2/src/tests/__init__.py
+-rwxrwxrwx   0 dfredriksen  (1000) dfredriksen  (1000)      387 2023-07-04 20:16:39.000000 sklearn_mlmlm-0.0.2/src/tests/test_common.py
+-rwxrwxrwx   0 dfredriksen  (1000) dfredriksen  (1000)      602 2023-07-04 20:17:33.000000 sklearn_mlmlm-0.0.2/src/tests/test_template.py
```

### Comparing `sklearn-mlmlm-0.0.1/LICENSE` & `sklearn_mlmlm-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sklearn-mlmlm-0.0.1/PKG-INFO` & `sklearn_mlmlm-0.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: sklearn-mlmlm
-Version: 0.0.1
+Name: sklearn_mlmlm
+Version: 0.0.2
 Summary: A python and sklearn compatible implementation of ML-MLM.
 Home-page: https://github.com/quantyra/scikit-mlmlm
 Download-URL: https://github.com/quantyra/scikit-mlmlm
 Maintainer: Daniel E Fredriksen
 Maintainer-email: dfredriksen@quantyra.org
 License: new BSD
 Classifier: Intended Audience :: Science/Research
```

### Comparing `sklearn-mlmlm-0.0.1/README.rst` & `sklearn_mlmlm-0.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `sklearn-mlmlm-0.0.1/setup.py` & `sklearn_mlmlm-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from setuptools import find_packages, setup
 
 # get __version__ from _version.py
 ver_file = os.path.join('src', '_version.py')
 with open(ver_file) as f:
     exec(f.read())
 
-DISTNAME = 'sklearn-mlmlm'
+DISTNAME = 'sklearn_mlmlm'
 DESCRIPTION = 'A python and sklearn compatible implementation of ML-MLM.'
 with codecs.open('README.rst', encoding='utf-8-sig') as f:
     LONG_DESCRIPTION = f.read()
 MAINTAINER = 'Daniel E Fredriksen'
 MAINTAINER_EMAIL = 'dfredriksen@quantyra.org'
 URL = 'https://github.com/quantyra/scikit-mlmlm'
 LICENSE = 'new BSD'
```

### Comparing `sklearn-mlmlm-0.0.1/sklearn_mlmlm.egg-info/PKG-INFO` & `sklearn_mlmlm-0.0.2/sklearn_mlmlm.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sklearn-mlmlm
-Version: 0.0.1
+Version: 0.0.2
 Summary: A python and sklearn compatible implementation of ML-MLM.
 Home-page: https://github.com/quantyra/scikit-mlmlm
 Download-URL: https://github.com/quantyra/scikit-mlmlm
 Maintainer: Daniel E Fredriksen
 Maintainer-email: dfredriksen@quantyra.org
 License: new BSD
 Classifier: Intended Audience :: Science/Research
```

### Comparing `sklearn-mlmlm-0.0.1/src/mlmlm.py` & `sklearn_mlmlm-0.0.2/src/mlmlm.py`

 * *Files identical despite different names*

### Comparing `sklearn-mlmlm-0.0.1/src/tests/test_template.py` & `sklearn_mlmlm-0.0.2/src/tests/test_template.py`

 * *Files identical despite different names*

