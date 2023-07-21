# Comparing `tmp/bennycloth-0.0.6.tar.gz` & `tmp/bennycloth-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bennycloth-0.0.6.tar", last modified: Thu Jan 19 19:36:35 2023, max compression
+gzip compressed data, was "bennycloth-0.0.7.tar", last modified: Thu Jan 19 19:59:21 2023, max compression
```

## Comparing `bennycloth-0.0.6.tar` & `bennycloth-0.0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 mhscott   (1000) mhscott   (1000)        0 2023-01-19 19:36:35.821476 bennycloth-0.0.6/
--rw-rw-r--   0 mhscott   (1000) mhscott   (1000)     1073 2023-01-19 16:26:09.000000 bennycloth-0.0.6/LICENSE
--rw-rw-r--   0 mhscott   (1000) mhscott   (1000)      551 2023-01-19 19:36:35.821476 bennycloth-0.0.6/PKG-INFO
--rw-rw-r--   0 mhscott   (1000) mhscott   (1000)       13 2023-01-19 16:26:09.000000 bennycloth-0.0.6/README.md
-drwxrwxr-x   0 mhscott   (1000) mhscott   (1000)        0 2023-01-19 19:36:35.821476 bennycloth-0.0.6/bennycloth/
--rw-rw-r--   0 mhscott   (1000) mhscott   (1000)     7825 2023-01-19 16:27:29.000000 bennycloth-0.0.6/bennycloth/TDConcrete.py
--rw-rw-r--   0 mhscott   (1000) mhscott   (1000)      164 2023-01-19 17:16:39.000000 bennycloth-0.0.6/bennycloth/__init__.py
-drwxrwxr-x   0 mhscott   (1000) mhscott   (1000)        0 2023-01-19 19:36:35.821476 bennycloth-0.0.6/bennycloth.egg-info/
--rw-rw-r--   0 mhscott   (1000) mhscott   (1000)      551 2023-01-19 19:36:35.000000 bennycloth-0.0.6/bennycloth.egg-info/PKG-INFO
--rw-rw-r--   0 mhscott   (1000) mhscott   (1000)      210 2023-01-19 19:36:35.000000 bennycloth-0.0.6/bennycloth.egg-info/SOURCES.txt
--rw-rw-r--   0 mhscott   (1000) mhscott   (1000)        1 2023-01-19 19:36:35.000000 bennycloth-0.0.6/bennycloth.egg-info/dependency_links.txt
--rw-rw-r--   0 mhscott   (1000) mhscott   (1000)       11 2023-01-19 19:36:35.000000 bennycloth-0.0.6/bennycloth.egg-info/top_level.txt
--rw-rw-r--   0 mhscott   (1000) mhscott   (1000)       38 2023-01-19 19:36:35.821476 bennycloth-0.0.6/setup.cfg
--rw-rw-r--   0 mhscott   (1000) mhscott   (1000)      743 2023-01-19 19:36:30.000000 bennycloth-0.0.6/setup.py
+drwxrwxr-x   0 mhscott   (1000) mhscott   (1000)        0 2023-01-19 19:59:21.248328 bennycloth-0.0.7/
+-rw-rw-r--   0 mhscott   (1000) mhscott   (1000)     1073 2023-01-19 16:26:09.000000 bennycloth-0.0.7/LICENSE
+-rw-rw-r--   0 mhscott   (1000) mhscott   (1000)      473 2023-01-19 19:59:21.248328 bennycloth-0.0.7/PKG-INFO
+-rw-rw-r--   0 mhscott   (1000) mhscott   (1000)       13 2023-01-19 16:26:09.000000 bennycloth-0.0.7/README.md
+drwxrwxr-x   0 mhscott   (1000) mhscott   (1000)        0 2023-01-19 19:59:21.248328 bennycloth-0.0.7/bennycloth/
+-rw-rw-r--   0 mhscott   (1000) mhscott   (1000)     7825 2023-01-19 16:27:29.000000 bennycloth-0.0.7/bennycloth/TDConcrete.py
+-rw-rw-r--   0 mhscott   (1000) mhscott   (1000)      168 2023-01-19 19:56:15.000000 bennycloth-0.0.7/bennycloth/__init__.py
+drwxrwxr-x   0 mhscott   (1000) mhscott   (1000)        0 2023-01-19 19:59:21.248328 bennycloth-0.0.7/bennycloth.egg-info/
+-rw-rw-r--   0 mhscott   (1000) mhscott   (1000)      473 2023-01-19 19:59:21.000000 bennycloth-0.0.7/bennycloth.egg-info/PKG-INFO
+-rw-rw-r--   0 mhscott   (1000) mhscott   (1000)      210 2023-01-19 19:59:21.000000 bennycloth-0.0.7/bennycloth.egg-info/SOURCES.txt
+-rw-rw-r--   0 mhscott   (1000) mhscott   (1000)        1 2023-01-19 19:59:21.000000 bennycloth-0.0.7/bennycloth.egg-info/dependency_links.txt
+-rw-rw-r--   0 mhscott   (1000) mhscott   (1000)       11 2023-01-19 19:59:21.000000 bennycloth-0.0.7/bennycloth.egg-info/top_level.txt
+-rw-rw-r--   0 mhscott   (1000) mhscott   (1000)       38 2023-01-19 19:59:21.248328 bennycloth-0.0.7/setup.cfg
+-rw-rw-r--   0 mhscott   (1000) mhscott   (1000)      684 2023-01-19 19:59:03.000000 bennycloth-0.0.7/setup.py
```

### Comparing `bennycloth-0.0.6/LICENSE` & `bennycloth-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `bennycloth-0.0.6/bennycloth/TDConcrete.py` & `bennycloth-0.0.7/bennycloth/TDConcrete.py`

 * *Files identical despite different names*

### Comparing `bennycloth-0.0.6/setup.py` & `bennycloth-0.0.7/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.6'
+VERSION = '0.0.7'
 DESCRIPTION = 'A collection of Python functions for structural engineering'
 LONG_DESCRIPTION = 'This package contains random utilitly functions accrued over many years of structural engineering research and teaching'
 
 setup(
 	name = 'bennycloth',
 	version = VERSION,
 	author = 'Michael H. Scott',
 	author_email = 'mhscott@oregonstate.edu',
 	description = DESCRIPTION,
 	long_description = LONG_DESCRIPTION,
 	packages = find_packages(),
 	install_requires = [],
 	keywords = ['python','opensees'],
 	classifiers = ['Programming Language :: Python :: 3',
-		'Programming Language :: Python :: 3.9',
-		'Programming Language :: Python :: 3.10',
 		'Operating System :: OS Independent'
-	]
+	],
+	python_requires = '>=3.6'
 )
```

