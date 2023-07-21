# Comparing `tmp/cytoolz-0.9.0.tar.gz` & `tmp/cytoolz-0.9.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cytoolz-0.9.0.tar", last modified: Sun Dec 17 17:03:10 2017, max compression
+gzip compressed data, was "dist/cytoolz-0.9.0.1.tar", last modified: Tue Mar  6 05:47:33 2018, max compression
```

## Comparing `cytoolz-0.9.0.tar` & `cytoolz-0.9.0.1.tar`

### file list

```diff
@@ -1,61 +1,60 @@
-drwxrwxr-x   0 erik      (1000) erik      (1000)        0 2017-12-17 17:03:10.000000 cytoolz-0.9.0/
--rw-rw-r--   0 erik      (1000) erik      (1000)     4298 2017-12-17 16:56:52.000000 cytoolz-0.9.0/setup.py
-drwxrwxr-x   0 erik      (1000) erik      (1000)        0 2017-12-17 17:03:10.000000 cytoolz-0.9.0/cytoolz.egg-info/
--rw-rw-r--   0 erik      (1000) erik      (1000)     1394 2017-12-17 17:03:10.000000 cytoolz-0.9.0/cytoolz.egg-info/SOURCES.txt
--rw-rw-r--   0 erik      (1000) erik      (1000)     4869 2017-12-17 17:03:10.000000 cytoolz-0.9.0/cytoolz.egg-info/PKG-INFO
--rw-rw-r--   0 erik      (1000) erik      (1000)        1 2017-12-17 17:03:10.000000 cytoolz-0.9.0/cytoolz.egg-info/not-zip-safe
--rw-rw-r--   0 erik      (1000) erik      (1000)        8 2017-12-17 17:03:10.000000 cytoolz-0.9.0/cytoolz.egg-info/top_level.txt
--rw-rw-r--   0 erik      (1000) erik      (1000)       13 2017-12-17 17:03:10.000000 cytoolz-0.9.0/cytoolz.egg-info/requires.txt
--rw-rw-r--   0 erik      (1000) erik      (1000)        1 2017-12-17 17:03:10.000000 cytoolz-0.9.0/cytoolz.egg-info/dependency_links.txt
--rw-rw-r--   0 erik      (1000) erik      (1000)     4869 2017-12-17 17:03:10.000000 cytoolz-0.9.0/PKG-INFO
--rw-rw-r--   0 erik      (1000) erik      (1000)       38 2017-12-17 17:03:10.000000 cytoolz-0.9.0/setup.cfg
--rw-rw-r--   0 erik      (1000) erik      (1000)     2722 2017-12-17 16:56:52.000000 cytoolz-0.9.0/README.rst
--rw-rw-r--   0 erik      (1000) erik      (1000)     1489 2016-01-19 04:26:02.000000 cytoolz-0.9.0/LICENSE.txt
--rw-rw-r--   0 erik      (1000) erik      (1000)       48 2016-12-05 02:46:57.000000 cytoolz-0.9.0/MANIFEST.in
-drwxrwxr-x   0 erik      (1000) erik      (1000)        0 2017-12-17 17:03:10.000000 cytoolz-0.9.0/cytoolz/
--rw-rw-r--   0 erik      (1000) erik      (1000)     1135 2016-12-05 02:46:57.000000 cytoolz-0.9.0/cytoolz/compatibility.py
--rw-rw-r--   0 erik      (1000) erik      (1000)       50 2017-12-17 16:57:17.000000 cytoolz-0.9.0/cytoolz/_version.py
--rw-rw-r--   0 erik      (1000) erik      (1000)      497 2016-11-03 06:02:26.000000 cytoolz-0.9.0/cytoolz/cpython.pxd
--rw-rw-r--   0 erik      (1000) erik      (1000)   906950 2017-12-17 16:59:50.000000 cytoolz-0.9.0/cytoolz/functoolz.c
--rw-rw-r--   0 erik      (1000) erik      (1000)   445941 2017-12-17 16:59:49.000000 cytoolz-0.9.0/cytoolz/dicttoolz.c
--rw-rw-r--   0 erik      (1000) erik      (1000)     2075 2016-12-05 02:46:57.000000 cytoolz-0.9.0/cytoolz/utils_test.py
--rw-rw-r--   0 erik      (1000) erik      (1000)    23123 2017-12-17 16:56:52.000000 cytoolz-0.9.0/cytoolz/functoolz.pyx
--rw-rw-r--   0 erik      (1000) erik      (1000)   170807 2017-12-17 16:59:51.000000 cytoolz-0.9.0/cytoolz/utils.c
--rw-rw-r--   0 erik      (1000) erik      (1000)     4648 2016-12-05 02:46:57.000000 cytoolz-0.9.0/cytoolz/itertoolz.pxd
-drwxrwxr-x   0 erik      (1000) erik      (1000)        0 2017-12-17 17:03:10.000000 cytoolz-0.9.0/cytoolz/tests/
--rw-rw-r--   0 erik      (1000) erik      (1000)      288 2017-02-04 19:43:28.000000 cytoolz-0.9.0/cytoolz/tests/test_curried_doctests.py
--rw-rw-r--   0 erik      (1000) erik      (1000)     8602 2017-12-17 05:17:23.000000 cytoolz-0.9.0/cytoolz/tests/test_dicttoolz.py
--rw-rw-r--   0 erik      (1000) erik      (1000)      380 2016-01-19 04:26:02.000000 cytoolz-0.9.0/cytoolz/tests/test_dev_skip_test.py
--rw-rw-r--   0 erik      (1000) erik      (1000)     2933 2017-12-17 05:17:23.000000 cytoolz-0.9.0/cytoolz/tests/test_signatures.py
--rw-rw-r--   0 erik      (1000) erik      (1000)      547 2017-12-17 05:17:23.000000 cytoolz-0.9.0/cytoolz/tests/test_compatibility.py
--rw-rw-r--   0 erik      (1000) erik      (1000)     5949 2017-12-17 16:56:52.000000 cytoolz-0.9.0/cytoolz/tests/test_serialization.py
--rw-rw-r--   0 erik      (1000) erik      (1000)     1399 2016-11-03 06:02:26.000000 cytoolz-0.9.0/cytoolz/tests/test_curried_toolzlike.py
--rw-rw-r--   0 erik      (1000) erik      (1000)      435 2016-12-05 02:46:57.000000 cytoolz-0.9.0/cytoolz/tests/test_doctests.py
--rw-rw-r--   0 erik      (1000) erik      (1000)    16282 2017-12-17 16:56:52.000000 cytoolz-0.9.0/cytoolz/tests/test_inspect_args.py
--rw-rw-r--   0 erik      (1000) erik      (1000)     3034 2016-12-05 02:46:57.000000 cytoolz-0.9.0/cytoolz/tests/test_docstrings.py
--rw-rw-r--   0 erik      (1000) erik      (1000)      385 2016-12-11 21:32:25.000000 cytoolz-0.9.0/cytoolz/tests/test_utils.py
--rw-rw-r--   0 erik      (1000) erik      (1000)     3495 2016-12-05 03:13:35.000000 cytoolz-0.9.0/cytoolz/tests/test_embedded_sigs.py
--rw-rw-r--   0 erik      (1000) erik      (1000)     1003 2016-11-03 06:02:26.000000 cytoolz-0.9.0/cytoolz/tests/dev_skip_test.py
--rw-rw-r--   0 erik      (1000) erik      (1000)    16529 2017-12-17 16:56:52.000000 cytoolz-0.9.0/cytoolz/tests/test_functoolz.py
--rw-rw-r--   0 erik      (1000) erik      (1000)    17465 2017-12-17 05:17:23.000000 cytoolz-0.9.0/cytoolz/tests/test_itertoolz.py
--rw-rw-r--   0 erik      (1000) erik      (1000)     1486 2017-02-04 19:43:41.000000 cytoolz-0.9.0/cytoolz/tests/test_tlz.py
--rw-rw-r--   0 erik      (1000) erik      (1000)     3726 2017-12-17 05:17:23.000000 cytoolz-0.9.0/cytoolz/tests/test_curried.py
--rw-rw-r--   0 erik      (1000) erik      (1000)      822 2017-12-17 05:17:23.000000 cytoolz-0.9.0/cytoolz/tests/test_recipes.py
--rw-rw-r--   0 erik      (1000) erik      (1000)    11823 2016-12-05 02:46:57.000000 cytoolz-0.9.0/cytoolz/tests/test_none_safe.py
--rw-rw-r--   0 erik      (1000) erik      (1000)  1786046 2017-12-17 16:59:50.000000 cytoolz-0.9.0/cytoolz/itertoolz.c
--rw-rw-r--   0 erik      (1000) erik      (1000)      476 2017-12-16 18:04:14.000000 cytoolz-0.9.0/cytoolz/__init__.py
--rw-rw-r--   0 erik      (1000) erik      (1000)     1209 2017-12-17 16:56:52.000000 cytoolz-0.9.0/cytoolz/functoolz.pxd
--rw-rw-r--   0 erik      (1000) erik      (1000)       33 2016-05-29 21:24:27.000000 cytoolz-0.9.0/cytoolz/utils.pxd
-drwxrwxr-x   0 erik      (1000) erik      (1000)        0 2017-12-17 17:03:10.000000 cytoolz-0.9.0/cytoolz/curried/
--rw-rw-r--   0 erik      (1000) erik      (1000)      350 2016-12-05 02:46:57.000000 cytoolz-0.9.0/cytoolz/curried/exceptions.py
--rw-rw-r--   0 erik      (1000) erik      (1000)     2791 2016-12-05 02:46:57.000000 cytoolz-0.9.0/cytoolz/curried/__init__.py
--rw-rw-r--   0 erik      (1000) erik      (1000)      502 2016-11-03 06:02:26.000000 cytoolz-0.9.0/cytoolz/curried/operator.py
--rw-rw-r--   0 erik      (1000) erik      (1000)      100 2016-05-29 21:24:27.000000 cytoolz-0.9.0/cytoolz/recipes.pxd
--rw-rw-r--   0 erik      (1000) erik      (1000)     1638 2016-11-03 06:02:26.000000 cytoolz-0.9.0/cytoolz/recipes.pyx
--rw-rw-r--   0 erik      (1000) erik      (1000)     1353 2016-12-05 02:46:57.000000 cytoolz-0.9.0/cytoolz/utils.pyx
--rw-rw-r--   0 erik      (1000) erik      (1000)      750 2017-12-16 18:04:04.000000 cytoolz-0.9.0/cytoolz/__init__.pxd
--rw-rw-r--   0 erik      (1000) erik      (1000)    50375 2017-12-17 16:56:52.000000 cytoolz-0.9.0/cytoolz/itertoolz.pyx
--rw-rw-r--   0 erik      (1000) erik      (1000)     4195 2017-12-17 16:49:25.000000 cytoolz-0.9.0/cytoolz/_signatures.py
--rw-rw-r--   0 erik      (1000) erik      (1000)   233005 2017-12-17 16:59:51.000000 cytoolz-0.9.0/cytoolz/recipes.c
--rw-rw-r--   0 erik      (1000) erik      (1000)     1284 2016-11-03 06:02:26.000000 cytoolz-0.9.0/cytoolz/dicttoolz.pxd
--rw-rw-r--   0 erik      (1000) erik      (1000)    14804 2016-12-05 02:46:57.000000 cytoolz-0.9.0/cytoolz/dicttoolz.pyx
+drwxrwxr-x   0 erik      (1000) erik      (1000)        0 2018-03-06 05:47:33.000000 cytoolz-0.9.0.1/
+-rw-rw-r--   0 erik      (1000) erik      (1000)     4298 2017-12-17 16:56:52.000000 cytoolz-0.9.0.1/setup.py
+drwxrwxr-x   0 erik      (1000) erik      (1000)        0 2018-03-06 05:47:33.000000 cytoolz-0.9.0.1/cytoolz.egg-info/
+-rw-rw-r--   0 erik      (1000) erik      (1000)     1355 2018-03-06 05:47:33.000000 cytoolz-0.9.0.1/cytoolz.egg-info/SOURCES.txt
+-rw-rw-r--   0 erik      (1000) erik      (1000)     4837 2018-03-06 05:47:33.000000 cytoolz-0.9.0.1/cytoolz.egg-info/PKG-INFO
+-rw-rw-r--   0 erik      (1000) erik      (1000)        1 2018-03-06 05:35:16.000000 cytoolz-0.9.0.1/cytoolz.egg-info/not-zip-safe
+-rw-rw-r--   0 erik      (1000) erik      (1000)        8 2018-03-06 05:47:33.000000 cytoolz-0.9.0.1/cytoolz.egg-info/top_level.txt
+-rw-rw-r--   0 erik      (1000) erik      (1000)       15 2018-03-06 05:47:33.000000 cytoolz-0.9.0.1/cytoolz.egg-info/requires.txt
+-rw-rw-r--   0 erik      (1000) erik      (1000)        1 2018-03-06 05:47:33.000000 cytoolz-0.9.0.1/cytoolz.egg-info/dependency_links.txt
+-rw-rw-r--   0 erik      (1000) erik      (1000)     4837 2018-03-06 05:47:33.000000 cytoolz-0.9.0.1/PKG-INFO
+-rw-rw-r--   0 erik      (1000) erik      (1000)       59 2018-03-06 05:47:33.000000 cytoolz-0.9.0.1/setup.cfg
+-rw-rw-r--   0 erik      (1000) erik      (1000)     2722 2017-12-17 16:56:52.000000 cytoolz-0.9.0.1/README.rst
+-rw-rw-r--   0 erik      (1000) erik      (1000)     1489 2016-01-19 04:26:02.000000 cytoolz-0.9.0.1/LICENSE.txt
+-rw-rw-r--   0 erik      (1000) erik      (1000)       48 2016-12-05 02:46:57.000000 cytoolz-0.9.0.1/MANIFEST.in
+drwxrwxr-x   0 erik      (1000) erik      (1000)        0 2018-03-06 05:47:33.000000 cytoolz-0.9.0.1/cytoolz/
+-rw-rw-r--   0 erik      (1000) erik      (1000)     1135 2016-12-05 02:46:57.000000 cytoolz-0.9.0.1/cytoolz/compatibility.py
+-rw-rw-r--   0 erik      (1000) erik      (1000)       52 2018-03-06 05:47:19.000000 cytoolz-0.9.0.1/cytoolz/_version.py
+-rw-rw-r--   0 erik      (1000) erik      (1000)      497 2016-11-03 06:02:26.000000 cytoolz-0.9.0.1/cytoolz/cpython.pxd
+-rw-rw-r--   0 erik      (1000) erik      (1000)   906950 2018-03-06 05:33:28.000000 cytoolz-0.9.0.1/cytoolz/functoolz.c
+-rw-rw-r--   0 erik      (1000) erik      (1000)   445941 2018-03-06 05:33:28.000000 cytoolz-0.9.0.1/cytoolz/dicttoolz.c
+-rw-rw-r--   0 erik      (1000) erik      (1000)     2075 2018-03-06 05:31:25.000000 cytoolz-0.9.0.1/cytoolz/utils_test.py
+-rw-rw-r--   0 erik      (1000) erik      (1000)    23123 2018-01-04 05:21:55.000000 cytoolz-0.9.0.1/cytoolz/functoolz.pyx
+-rw-rw-r--   0 erik      (1000) erik      (1000)   170807 2018-03-06 05:33:28.000000 cytoolz-0.9.0.1/cytoolz/utils.c
+-rw-rw-r--   0 erik      (1000) erik      (1000)     4648 2016-12-05 02:46:57.000000 cytoolz-0.9.0.1/cytoolz/itertoolz.pxd
+drwxrwxr-x   0 erik      (1000) erik      (1000)        0 2018-03-06 05:47:33.000000 cytoolz-0.9.0.1/cytoolz/tests/
+-rw-rw-r--   0 erik      (1000) erik      (1000)     8602 2017-12-17 17:15:51.000000 cytoolz-0.9.0.1/cytoolz/tests/test_dicttoolz.py
+-rw-rw-r--   0 erik      (1000) erik      (1000)      380 2016-01-19 04:26:02.000000 cytoolz-0.9.0.1/cytoolz/tests/test_dev_skip_test.py
+-rw-rw-r--   0 erik      (1000) erik      (1000)     2933 2017-12-17 17:15:51.000000 cytoolz-0.9.0.1/cytoolz/tests/test_signatures.py
+-rw-rw-r--   0 erik      (1000) erik      (1000)      547 2017-12-17 17:15:51.000000 cytoolz-0.9.0.1/cytoolz/tests/test_compatibility.py
+-rw-rw-r--   0 erik      (1000) erik      (1000)     5949 2017-12-17 17:15:51.000000 cytoolz-0.9.0.1/cytoolz/tests/test_serialization.py
+-rw-rw-r--   0 erik      (1000) erik      (1000)     1399 2016-11-03 06:02:26.000000 cytoolz-0.9.0.1/cytoolz/tests/test_curried_toolzlike.py
+-rw-rw-r--   0 erik      (1000) erik      (1000)      435 2018-03-06 05:31:25.000000 cytoolz-0.9.0.1/cytoolz/tests/test_doctests.py
+-rw-rw-r--   0 erik      (1000) erik      (1000)    16282 2018-03-06 05:33:28.000000 cytoolz-0.9.0.1/cytoolz/tests/test_inspect_args.py
+-rw-rw-r--   0 erik      (1000) erik      (1000)     3034 2016-12-05 02:46:57.000000 cytoolz-0.9.0.1/cytoolz/tests/test_docstrings.py
+-rw-rw-r--   0 erik      (1000) erik      (1000)      385 2016-12-11 21:32:25.000000 cytoolz-0.9.0.1/cytoolz/tests/test_utils.py
+-rw-rw-r--   0 erik      (1000) erik      (1000)     3495 2016-12-05 03:13:35.000000 cytoolz-0.9.0.1/cytoolz/tests/test_embedded_sigs.py
+-rw-rw-r--   0 erik      (1000) erik      (1000)     1003 2016-11-03 06:02:26.000000 cytoolz-0.9.0.1/cytoolz/tests/dev_skip_test.py
+-rw-rw-r--   0 erik      (1000) erik      (1000)    16529 2017-12-17 17:16:04.000000 cytoolz-0.9.0.1/cytoolz/tests/test_functoolz.py
+-rw-rw-r--   0 erik      (1000) erik      (1000)    17465 2017-12-17 17:15:51.000000 cytoolz-0.9.0.1/cytoolz/tests/test_itertoolz.py
+-rw-rw-r--   0 erik      (1000) erik      (1000)     1486 2017-02-04 19:43:41.000000 cytoolz-0.9.0.1/cytoolz/tests/test_tlz.py
+-rw-rw-r--   0 erik      (1000) erik      (1000)     3726 2017-12-17 17:15:51.000000 cytoolz-0.9.0.1/cytoolz/tests/test_curried.py
+-rw-rw-r--   0 erik      (1000) erik      (1000)      822 2017-12-17 17:15:51.000000 cytoolz-0.9.0.1/cytoolz/tests/test_recipes.py
+-rw-rw-r--   0 erik      (1000) erik      (1000)    11823 2016-12-05 02:46:57.000000 cytoolz-0.9.0.1/cytoolz/tests/test_none_safe.py
+-rw-rw-r--   0 erik      (1000) erik      (1000)  1786046 2018-03-06 05:33:28.000000 cytoolz-0.9.0.1/cytoolz/itertoolz.c
+-rw-rw-r--   0 erik      (1000) erik      (1000)      476 2017-12-16 18:04:14.000000 cytoolz-0.9.0.1/cytoolz/__init__.py
+-rw-rw-r--   0 erik      (1000) erik      (1000)     1209 2017-12-17 16:56:52.000000 cytoolz-0.9.0.1/cytoolz/functoolz.pxd
+-rw-rw-r--   0 erik      (1000) erik      (1000)       33 2016-05-29 21:24:27.000000 cytoolz-0.9.0.1/cytoolz/utils.pxd
+drwxrwxr-x   0 erik      (1000) erik      (1000)        0 2018-03-06 05:47:33.000000 cytoolz-0.9.0.1/cytoolz/curried/
+-rw-rw-r--   0 erik      (1000) erik      (1000)      350 2016-12-05 02:46:57.000000 cytoolz-0.9.0.1/cytoolz/curried/exceptions.py
+-rw-rw-r--   0 erik      (1000) erik      (1000)     2791 2016-12-05 02:46:57.000000 cytoolz-0.9.0.1/cytoolz/curried/__init__.py
+-rw-rw-r--   0 erik      (1000) erik      (1000)      502 2016-11-03 06:02:26.000000 cytoolz-0.9.0.1/cytoolz/curried/operator.py
+-rw-rw-r--   0 erik      (1000) erik      (1000)      100 2016-05-29 21:24:27.000000 cytoolz-0.9.0.1/cytoolz/recipes.pxd
+-rw-rw-r--   0 erik      (1000) erik      (1000)     1638 2016-11-03 06:02:26.000000 cytoolz-0.9.0.1/cytoolz/recipes.pyx
+-rw-rw-r--   0 erik      (1000) erik      (1000)     1353 2016-12-05 02:46:57.000000 cytoolz-0.9.0.1/cytoolz/utils.pyx
+-rw-rw-r--   0 erik      (1000) erik      (1000)      750 2017-12-16 18:04:04.000000 cytoolz-0.9.0.1/cytoolz/__init__.pxd
+-rw-rw-r--   0 erik      (1000) erik      (1000)    50375 2018-01-04 05:24:01.000000 cytoolz-0.9.0.1/cytoolz/itertoolz.pyx
+-rw-rw-r--   0 erik      (1000) erik      (1000)     4195 2017-12-17 16:49:25.000000 cytoolz-0.9.0.1/cytoolz/_signatures.py
+-rw-rw-r--   0 erik      (1000) erik      (1000)   233005 2018-03-06 05:33:28.000000 cytoolz-0.9.0.1/cytoolz/recipes.c
+-rw-rw-r--   0 erik      (1000) erik      (1000)     1284 2016-11-03 06:02:26.000000 cytoolz-0.9.0.1/cytoolz/dicttoolz.pxd
+-rw-rw-r--   0 erik      (1000) erik      (1000)    14804 2016-12-05 02:46:57.000000 cytoolz-0.9.0.1/cytoolz/dicttoolz.pyx
```

### Comparing `cytoolz-0.9.0/setup.py` & `cytoolz-0.9.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `cytoolz-0.9.0/cytoolz.egg-info/SOURCES.txt` & `cytoolz-0.9.0.1/cytoolz.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -32,15 +32,14 @@
 cytoolz.egg-info/top_level.txt
 cytoolz/curried/__init__.py
 cytoolz/curried/exceptions.py
 cytoolz/curried/operator.py
 cytoolz/tests/dev_skip_test.py
 cytoolz/tests/test_compatibility.py
 cytoolz/tests/test_curried.py
-cytoolz/tests/test_curried_doctests.py
 cytoolz/tests/test_curried_toolzlike.py
 cytoolz/tests/test_dev_skip_test.py
 cytoolz/tests/test_dicttoolz.py
 cytoolz/tests/test_docstrings.py
 cytoolz/tests/test_doctests.py
 cytoolz/tests/test_embedded_sigs.py
 cytoolz/tests/test_functoolz.py
```

### Comparing `cytoolz-0.9.0/cytoolz.egg-info/PKG-INFO` & `cytoolz-0.9.0.1/cytoolz.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 1.1
 Name: cytoolz
-Version: 0.9.0
+Version: 0.9.0.1
 Summary: Cython implementation of Toolz: High performance functional utilities
 Home-page: https://github.com/pytoolz/cytoolz
 Author: Erik Welch
 Author-email: erik.n.welch@gmail.com
 License: BSD
-Description-Content-Type: UNKNOWN
 Description: CyToolz
         =======
         
         |Build Status| |Version Status|
         
         Cython implementation of the
         |literal toolz|_ `package, <https://pypi.python.org/pypi/toolz/>`__ which
```

### Comparing `cytoolz-0.9.0/PKG-INFO` & `cytoolz-0.9.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 1.1
 Name: cytoolz
-Version: 0.9.0
+Version: 0.9.0.1
 Summary: Cython implementation of Toolz: High performance functional utilities
 Home-page: https://github.com/pytoolz/cytoolz
 Author: Erik Welch
 Author-email: erik.n.welch@gmail.com
 License: BSD
-Description-Content-Type: UNKNOWN
 Description: CyToolz
         =======
         
         |Build Status| |Version Status|
         
         Cython implementation of the
         |literal toolz|_ `package, <https://pypi.python.org/pypi/toolz/>`__ which
```

### Comparing `cytoolz-0.9.0/README.rst` & `cytoolz-0.9.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `cytoolz-0.9.0/LICENSE.txt` & `cytoolz-0.9.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cytoolz-0.9.0/cytoolz/compatibility.py` & `cytoolz-0.9.0.1/cytoolz/compatibility.py`

 * *Files identical despite different names*

### Comparing `cytoolz-0.9.0/cytoolz/functoolz.c` & `cytoolz-0.9.0.1/cytoolz/functoolz.c`

 * *Files identical despite different names*

### Comparing `cytoolz-0.9.0/cytoolz/dicttoolz.c` & `cytoolz-0.9.0.1/cytoolz/dicttoolz.c`

 * *Files identical despite different names*

### Comparing `cytoolz-0.9.0/cytoolz/utils_test.py` & `cytoolz-0.9.0.1/cytoolz/utils_test.py`

 * *Files identical despite different names*

### Comparing `cytoolz-0.9.0/cytoolz/functoolz.pyx` & `cytoolz-0.9.0.1/cytoolz/functoolz.pyx`

 * *Files identical despite different names*

### Comparing `cytoolz-0.9.0/cytoolz/utils.c` & `cytoolz-0.9.0.1/cytoolz/utils.c`

 * *Files identical despite different names*

### Comparing `cytoolz-0.9.0/cytoolz/itertoolz.pxd` & `cytoolz-0.9.0.1/cytoolz/itertoolz.pxd`

 * *Files identical despite different names*

### Comparing `cytoolz-0.9.0/cytoolz/tests/test_dicttoolz.py` & `cytoolz-0.9.0.1/cytoolz/tests/test_dicttoolz.py`

 * *Files identical despite different names*

### Comparing `cytoolz-0.9.0/cytoolz/tests/test_signatures.py` & `cytoolz-0.9.0.1/cytoolz/tests/test_signatures.py`

 * *Files identical despite different names*

### Comparing `cytoolz-0.9.0/cytoolz/tests/test_compatibility.py` & `cytoolz-0.9.0.1/cytoolz/tests/test_compatibility.py`

 * *Files identical despite different names*

### Comparing `cytoolz-0.9.0/cytoolz/tests/test_serialization.py` & `cytoolz-0.9.0.1/cytoolz/tests/test_serialization.py`

 * *Files identical despite different names*

### Comparing `cytoolz-0.9.0/cytoolz/tests/test_curried_toolzlike.py` & `cytoolz-0.9.0.1/cytoolz/tests/test_curried_toolzlike.py`

 * *Files identical despite different names*

### Comparing `cytoolz-0.9.0/cytoolz/tests/test_inspect_args.py` & `cytoolz-0.9.0.1/cytoolz/tests/test_inspect_args.py`

 * *Files identical despite different names*

### Comparing `cytoolz-0.9.0/cytoolz/tests/test_docstrings.py` & `cytoolz-0.9.0.1/cytoolz/tests/test_docstrings.py`

 * *Files identical despite different names*

### Comparing `cytoolz-0.9.0/cytoolz/tests/test_embedded_sigs.py` & `cytoolz-0.9.0.1/cytoolz/tests/test_embedded_sigs.py`

 * *Files identical despite different names*

### Comparing `cytoolz-0.9.0/cytoolz/tests/dev_skip_test.py` & `cytoolz-0.9.0.1/cytoolz/tests/dev_skip_test.py`

 * *Files identical despite different names*

### Comparing `cytoolz-0.9.0/cytoolz/tests/test_functoolz.py` & `cytoolz-0.9.0.1/cytoolz/tests/test_functoolz.py`

 * *Files identical despite different names*

### Comparing `cytoolz-0.9.0/cytoolz/tests/test_itertoolz.py` & `cytoolz-0.9.0.1/cytoolz/tests/test_itertoolz.py`

 * *Files identical despite different names*

### Comparing `cytoolz-0.9.0/cytoolz/tests/test_tlz.py` & `cytoolz-0.9.0.1/cytoolz/tests/test_tlz.py`

 * *Files identical despite different names*

### Comparing `cytoolz-0.9.0/cytoolz/tests/test_curried.py` & `cytoolz-0.9.0.1/cytoolz/tests/test_curried.py`

 * *Files identical despite different names*

### Comparing `cytoolz-0.9.0/cytoolz/tests/test_recipes.py` & `cytoolz-0.9.0.1/cytoolz/tests/test_recipes.py`

 * *Files identical despite different names*

### Comparing `cytoolz-0.9.0/cytoolz/tests/test_none_safe.py` & `cytoolz-0.9.0.1/cytoolz/tests/test_none_safe.py`

 * *Files identical despite different names*

### Comparing `cytoolz-0.9.0/cytoolz/itertoolz.c` & `cytoolz-0.9.0.1/cytoolz/itertoolz.c`

 * *Files identical despite different names*

### Comparing `cytoolz-0.9.0/cytoolz/functoolz.pxd` & `cytoolz-0.9.0.1/cytoolz/functoolz.pxd`

 * *Files identical despite different names*

### Comparing `cytoolz-0.9.0/cytoolz/curried/__init__.py` & `cytoolz-0.9.0.1/cytoolz/curried/__init__.py`

 * *Files identical despite different names*

### Comparing `cytoolz-0.9.0/cytoolz/recipes.pyx` & `cytoolz-0.9.0.1/cytoolz/recipes.pyx`

 * *Files identical despite different names*

### Comparing `cytoolz-0.9.0/cytoolz/utils.pyx` & `cytoolz-0.9.0.1/cytoolz/utils.pyx`

 * *Files identical despite different names*

### Comparing `cytoolz-0.9.0/cytoolz/__init__.pxd` & `cytoolz-0.9.0.1/cytoolz/__init__.pxd`

 * *Files identical despite different names*

### Comparing `cytoolz-0.9.0/cytoolz/itertoolz.pyx` & `cytoolz-0.9.0.1/cytoolz/itertoolz.pyx`

 * *Files identical despite different names*

### Comparing `cytoolz-0.9.0/cytoolz/_signatures.py` & `cytoolz-0.9.0.1/cytoolz/_signatures.py`

 * *Files identical despite different names*

### Comparing `cytoolz-0.9.0/cytoolz/recipes.c` & `cytoolz-0.9.0.1/cytoolz/recipes.c`

 * *Files identical despite different names*

### Comparing `cytoolz-0.9.0/cytoolz/dicttoolz.pxd` & `cytoolz-0.9.0.1/cytoolz/dicttoolz.pxd`

 * *Files identical despite different names*

### Comparing `cytoolz-0.9.0/cytoolz/dicttoolz.pyx` & `cytoolz-0.9.0.1/cytoolz/dicttoolz.pyx`

 * *Files identical despite different names*

