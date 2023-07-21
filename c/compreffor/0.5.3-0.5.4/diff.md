# Comparing `tmp/compreffor-0.5.3.tar.gz` & `tmp/compreffor-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "compreffor-0.5.3.tar", last modified: Wed Nov 16 12:02:33 2022, max compression
+gzip compressed data, was "compreffor-0.5.4.tar", last modified: Fri Jul 21 16:43:53 2023, max compression
```

## Comparing `compreffor-0.5.3.tar` & `compreffor-0.5.4.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 12:02:33.671450 compreffor-0.5.3/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 12:02:33.655449 compreffor-0.5.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 12:02:33.659449 compreffor-0.5.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     6031 2022-11-16 12:02:22.000000 compreffor-0.5.3/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (121)      247 2022-11-16 12:02:22.000000 compreffor-0.5.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      125 2022-11-16 12:02:22.000000 compreffor-0.5.3/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (121)      168 2022-11-16 12:02:22.000000 compreffor-0.5.3/.pyup.yml
--rw-r--r--   0 runner    (1001) docker     (121)    11358 2022-11-16 12:02:22.000000 compreffor-0.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      928 2022-11-16 12:02:33.671450 compreffor-0.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      273 2022-11-16 12:02:22.000000 compreffor-0.5.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-11-16 12:02:22.000000 compreffor-0.5.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-11-16 12:02:22.000000 compreffor-0.5.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      832 2022-11-16 12:02:33.671450 compreffor-0.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     6502 2022-11-16 12:02:22.000000 compreffor-0.5.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 12:02:33.655449 compreffor-0.5.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 12:02:33.659449 compreffor-0.5.3/src/cxx/
--rw-r--r--   0 runner    (1001) docker     (121)      934 2022-11-16 12:02:22.000000 compreffor-0.5.3/src/cxx/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)     1113 2022-11-16 12:02:22.000000 compreffor-0.5.3/src/cxx/Makefile.vc
--rw-r--r--   0 runner    (1001) docker     (121)    31915 2022-11-16 12:02:22.000000 compreffor-0.5.3/src/cxx/cffCompressor.cc
--rw-r--r--   0 runner    (1001) docker     (121)     7991 2022-11-16 12:02:22.000000 compreffor-0.5.3/src/cxx/cffCompressor.h
--rw-r--r--   0 runner    (1001) docker     (121)       65 2022-11-16 12:02:22.000000 compreffor-0.5.3/src/cxx/compreff.def
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 12:02:33.663450 compreffor-0.5.3/src/cxx/mingw-std-threads/
--rw-r--r--   0 runner    (1001) docker     (121)     1296 2022-11-16 12:02:22.000000 compreffor-0.5.3/src/cxx/mingw-std-threads/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2492 2022-11-16 12:02:22.000000 compreffor-0.5.3/src/cxx/mingw-std-threads/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     8182 2022-11-16 12:02:22.000000 compreffor-0.5.3/src/cxx/mingw-std-threads/mingw.condition_variable.h
--rw-r--r--   0 runner    (1001) docker     (121)     8682 2022-11-16 12:02:22.000000 compreffor-0.5.3/src/cxx/mingw-std-threads/mingw.mutex.h
--rw-r--r--   0 runner    (1001) docker     (121)     5458 2022-11-16 12:02:22.000000 compreffor-0.5.3/src/cxx/mingw-std-threads/mingw.thread.h
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 12:02:33.663450 compreffor-0.5.3/src/cxx/mingw-std-threads/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      139 2022-11-16 12:02:22.000000 compreffor-0.5.3/src/cxx/mingw-std-threads/tests/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1592 2022-11-16 12:02:22.000000 compreffor-0.5.3/src/cxx/mingw-std-threads/tests/tests.cpp
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 12:02:33.663450 compreffor-0.5.3/src/cython/
--rw-r--r--   0 runner    (1001) docker     (121)   141787 2022-11-16 12:02:22.000000 compreffor-0.5.3/src/cython/_compreffor.cpp
--rw-r--r--   0 runner    (1001) docker     (121)      595 2022-11-16 12:02:22.000000 compreffor-0.5.3/src/cython/_compreffor.pyx
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 12:02:33.655449 compreffor-0.5.3/src/python/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 12:02:33.663450 compreffor-0.5.3/src/python/compreffor/
--rw-r--r--   0 runner    (1001) docker     (121)     6709 2022-11-16 12:02:22.000000 compreffor-0.5.3/src/python/compreffor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5440 2022-11-16 12:02:22.000000 compreffor-0.5.3/src/python/compreffor/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)      176 2022-11-16 12:02:33.000000 compreffor-0.5.3/src/python/compreffor/_version.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     6884 2022-11-16 12:02:22.000000 compreffor-0.5.3/src/python/compreffor/cxxCompressor.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    40329 2022-11-16 12:02:22.000000 compreffor-0.5.3/src/python/compreffor/pyCompressor.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 12:02:33.667450 compreffor-0.5.3/src/python/compreffor/test/
--rw-r--r--   0 runner    (1001) docker     (121)      598 2022-11-16 12:02:22.000000 compreffor-0.5.3/src/python/compreffor/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1677 2022-11-16 12:02:22.000000 compreffor-0.5.3/src/python/compreffor/test/dummy.py
--rw-r--r--   0 runner    (1001) docker     (121)    10371 2022-11-16 12:02:22.000000 compreffor-0.5.3/src/python/compreffor/test/pyCompressor_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     4260 2022-11-16 12:02:22.000000 compreffor-0.5.3/src/python/compreffor/test/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 12:02:33.667450 compreffor-0.5.3/src/python/compreffor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      928 2022-11-16 12:02:33.000000 compreffor-0.5.3/src/python/compreffor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1356 2022-11-16 12:02:33.000000 compreffor-0.5.3/src/python/compreffor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-16 12:02:33.000000 compreffor-0.5.3/src/python/compreffor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       56 2022-11-16 12:02:33.000000 compreffor-0.5.3/src/python/compreffor.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-16 12:02:33.000000 compreffor-0.5.3/src/python/compreffor.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-11-16 12:02:33.000000 compreffor-0.5.3/src/python/compreffor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-11-16 12:02:33.000000 compreffor-0.5.3/src/python/compreffor.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 12:02:33.671450 compreffor-0.5.3/tools/
--rwxr-xr-x   0 runner    (1001) docker     (121)     3425 2022-11-16 12:02:22.000000 compreffor-0.5.3/tools/analyzer.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1164 2022-11-16 12:02:22.000000 compreffor-0.5.3/tools/gen_data.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3064 2022-11-16 12:02:22.000000 compreffor-0.5.3/tools/optimizeParameter.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3311 2022-11-16 12:02:22.000000 compreffor-0.5.3/tools/simpleCffCompressor.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    11089 2022-11-16 12:02:22.000000 compreffor-0.5.3/tools/subr_grapher.py
--rw-r--r--   0 runner    (1001) docker     (121)      215 2022-11-16 12:02:22.000000 compreffor-0.5.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:43:53.548348 compreffor-0.5.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:43:53.540348 compreffor-0.5.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:43:53.540348 compreffor-0.5.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     6031 2023-07-21 16:43:42.000000 compreffor-0.5.4/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-21 16:43:42.000000 compreffor-0.5.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-21 16:43:42.000000 compreffor-0.5.4/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-21 16:43:42.000000 compreffor-0.5.4/.pyup.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-21 16:43:42.000000 compreffor-0.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-21 16:43:53.548348 compreffor-0.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-21 16:43:42.000000 compreffor-0.5.4/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-21 16:43:42.000000 compreffor-0.5.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-21 16:43:42.000000 compreffor-0.5.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-07-21 16:43:53.548348 compreffor-0.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     6533 2023-07-21 16:43:42.000000 compreffor-0.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:43:53.540348 compreffor-0.5.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:43:53.544348 compreffor-0.5.4/src/cxx/
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-21 16:43:42.000000 compreffor-0.5.4/src/cxx/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-07-21 16:43:42.000000 compreffor-0.5.4/src/cxx/Makefile.vc
+-rw-r--r--   0 runner    (1001) docker     (123)    31915 2023-07-21 16:43:42.000000 compreffor-0.5.4/src/cxx/cffCompressor.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     7991 2023-07-21 16:43:42.000000 compreffor-0.5.4/src/cxx/cffCompressor.h
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-21 16:43:42.000000 compreffor-0.5.4/src/cxx/compreff.def
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:43:53.544348 compreffor-0.5.4/src/cxx/mingw-std-threads/
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-07-21 16:43:42.000000 compreffor-0.5.4/src/cxx/mingw-std-threads/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-07-21 16:43:42.000000 compreffor-0.5.4/src/cxx/mingw-std-threads/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8182 2023-07-21 16:43:42.000000 compreffor-0.5.4/src/cxx/mingw-std-threads/mingw.condition_variable.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8682 2023-07-21 16:43:42.000000 compreffor-0.5.4/src/cxx/mingw-std-threads/mingw.mutex.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5458 2023-07-21 16:43:42.000000 compreffor-0.5.4/src/cxx/mingw-std-threads/mingw.thread.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:43:53.544348 compreffor-0.5.4/src/cxx/mingw-std-threads/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-21 16:43:42.000000 compreffor-0.5.4/src/cxx/mingw-std-threads/tests/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-07-21 16:43:42.000000 compreffor-0.5.4/src/cxx/mingw-std-threads/tests/tests.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:43:53.544348 compreffor-0.5.4/src/cython/
+-rw-r--r--   0 runner    (1001) docker     (123)   141787 2023-07-21 16:43:42.000000 compreffor-0.5.4/src/cython/_compreffor.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-21 16:43:42.000000 compreffor-0.5.4/src/cython/_compreffor.pyx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:43:53.540348 compreffor-0.5.4/src/python/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:43:53.544348 compreffor-0.5.4/src/python/compreffor/
+-rw-r--r--   0 runner    (1001) docker     (123)     6709 2023-07-21 16:43:42.000000 compreffor-0.5.4/src/python/compreffor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-07-21 16:43:42.000000 compreffor-0.5.4/src/python/compreffor/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-21 16:43:53.000000 compreffor-0.5.4/src/python/compreffor/_version.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6884 2023-07-21 16:43:42.000000 compreffor-0.5.4/src/python/compreffor/cxxCompressor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    40329 2023-07-21 16:43:42.000000 compreffor-0.5.4/src/python/compreffor/pyCompressor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:43:53.544348 compreffor-0.5.4/src/python/compreffor/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-21 16:43:42.000000 compreffor-0.5.4/src/python/compreffor/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-07-21 16:43:42.000000 compreffor-0.5.4/src/python/compreffor/test/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10371 2023-07-21 16:43:42.000000 compreffor-0.5.4/src/python/compreffor/test/pyCompressor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4260 2023-07-21 16:43:42.000000 compreffor-0.5.4/src/python/compreffor/test/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:43:53.544348 compreffor-0.5.4/src/python/compreffor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-21 16:43:53.000000 compreffor-0.5.4/src/python/compreffor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-07-21 16:43:53.000000 compreffor-0.5.4/src/python/compreffor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 16:43:53.000000 compreffor-0.5.4/src/python/compreffor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-21 16:43:53.000000 compreffor-0.5.4/src/python/compreffor.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 16:43:53.000000 compreffor-0.5.4/src/python/compreffor.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-21 16:43:53.000000 compreffor-0.5.4/src/python/compreffor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-21 16:43:53.000000 compreffor-0.5.4/src/python/compreffor.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:43:53.548348 compreffor-0.5.4/tools/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3425 2023-07-21 16:43:42.000000 compreffor-0.5.4/tools/analyzer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1164 2023-07-21 16:43:42.000000 compreffor-0.5.4/tools/gen_data.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3064 2023-07-21 16:43:42.000000 compreffor-0.5.4/tools/optimizeParameter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3311 2023-07-21 16:43:42.000000 compreffor-0.5.4/tools/simpleCffCompressor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11089 2023-07-21 16:43:42.000000 compreffor-0.5.4/tools/subr_grapher.py
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-21 16:43:42.000000 compreffor-0.5.4/tox.ini
```

### Comparing `compreffor-0.5.3/.github/workflows/ci.yml` & `compreffor-0.5.4/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `compreffor-0.5.3/LICENSE` & `compreffor-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `compreffor-0.5.3/PKG-INFO` & `compreffor-0.5.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: compreffor
-Version: 0.5.3
+Version: 0.5.4
 Summary: A CFF subroutinizer for fontTools.
 Author: Sam Fishman
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `compreffor-0.5.3/setup.cfg` & `compreffor-0.5.4/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 search = version="{current_version}"
 replace = version="{new_version}"
 
 [aliases]
 test = pytest
 
 [metadata]
-license_file = LICENSE
+license_files = LICENSE
 
 [tool:pytest]
 minversion = 2.8
 testpaths = 
 	src/python/compreffor
 python_files = 
 	*_test.py
```

### Comparing `compreffor-0.5.3/setup.py` & `compreffor-0.5.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 except pkg_resources.ResolutionError:
     with_cython = False
     print('Distribution mode: Compiling from Cython-generated .cpp sources.')
     from setuptools.command.build_ext import build_ext
 else:
     with_cython = True
     print('Development mode: Compiling Cython modules from .pyx sources.')
-    from Cython.Distutils import build_ext
+    from Cython.Distutils.old_build_ext import old_build_ext as build_ext
 
 
 class custom_build_ext(build_ext):
     """ Custom 'build_ext' command which allows to pass compiler-specific
     'extra_compile_args', 'define_macros' and 'undef_macros' options.
     """
```

### Comparing `compreffor-0.5.3/src/cxx/Makefile` & `compreffor-0.5.4/src/cxx/Makefile`

 * *Files identical despite different names*

### Comparing `compreffor-0.5.3/src/cxx/Makefile.vc` & `compreffor-0.5.4/src/cxx/Makefile.vc`

 * *Files identical despite different names*

### Comparing `compreffor-0.5.3/src/cxx/cffCompressor.cc` & `compreffor-0.5.4/src/cxx/cffCompressor.cc`

 * *Files identical despite different names*

### Comparing `compreffor-0.5.3/src/cxx/cffCompressor.h` & `compreffor-0.5.4/src/cxx/cffCompressor.h`

 * *Files identical despite different names*

### Comparing `compreffor-0.5.3/src/cxx/mingw-std-threads/LICENSE` & `compreffor-0.5.4/src/cxx/mingw-std-threads/LICENSE`

 * *Files identical despite different names*

### Comparing `compreffor-0.5.3/src/cxx/mingw-std-threads/README.md` & `compreffor-0.5.4/src/cxx/mingw-std-threads/README.md`

 * *Files identical despite different names*

### Comparing `compreffor-0.5.3/src/cxx/mingw-std-threads/mingw.condition_variable.h` & `compreffor-0.5.4/src/cxx/mingw-std-threads/mingw.condition_variable.h`

 * *Files identical despite different names*

### Comparing `compreffor-0.5.3/src/cxx/mingw-std-threads/mingw.mutex.h` & `compreffor-0.5.4/src/cxx/mingw-std-threads/mingw.mutex.h`

 * *Files identical despite different names*

### Comparing `compreffor-0.5.3/src/cxx/mingw-std-threads/mingw.thread.h` & `compreffor-0.5.4/src/cxx/mingw-std-threads/mingw.thread.h`

 * *Files identical despite different names*

### Comparing `compreffor-0.5.3/src/cxx/mingw-std-threads/tests/tests.cpp` & `compreffor-0.5.4/src/cxx/mingw-std-threads/tests/tests.cpp`

 * *Files identical despite different names*

### Comparing `compreffor-0.5.3/src/cython/_compreffor.cpp` & `compreffor-0.5.4/src/cython/_compreffor.cpp`

 * *Files identical despite different names*

### Comparing `compreffor-0.5.3/src/cython/_compreffor.pyx` & `compreffor-0.5.4/src/cython/_compreffor.pyx`

 * *Files identical despite different names*

### Comparing `compreffor-0.5.3/src/python/compreffor/__init__.py` & `compreffor-0.5.4/src/python/compreffor/__init__.py`

 * *Files identical despite different names*

### Comparing `compreffor-0.5.3/src/python/compreffor/__main__.py` & `compreffor-0.5.4/src/python/compreffor/__main__.py`

 * *Files identical despite different names*

### Comparing `compreffor-0.5.3/src/python/compreffor/cxxCompressor.py` & `compreffor-0.5.4/src/python/compreffor/cxxCompressor.py`

 * *Files identical despite different names*

### Comparing `compreffor-0.5.3/src/python/compreffor/pyCompressor.py` & `compreffor-0.5.4/src/python/compreffor/pyCompressor.py`

 * *Files identical despite different names*

### Comparing `compreffor-0.5.3/src/python/compreffor/test/__init__.py` & `compreffor-0.5.4/src/python/compreffor/test/__init__.py`

 * *Files identical despite different names*

### Comparing `compreffor-0.5.3/src/python/compreffor/test/dummy.py` & `compreffor-0.5.4/src/python/compreffor/test/dummy.py`

 * *Files identical despite different names*

### Comparing `compreffor-0.5.3/src/python/compreffor/test/pyCompressor_test.py` & `compreffor-0.5.4/src/python/compreffor/test/pyCompressor_test.py`

 * *Files identical despite different names*

### Comparing `compreffor-0.5.3/src/python/compreffor/test/util.py` & `compreffor-0.5.4/src/python/compreffor/test/util.py`

 * *Files identical despite different names*

### Comparing `compreffor-0.5.3/src/python/compreffor.egg-info/PKG-INFO` & `compreffor-0.5.4/src/python/compreffor.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: compreffor
-Version: 0.5.3
+Version: 0.5.4
 Summary: A CFF subroutinizer for fontTools.
 Author: Sam Fishman
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `compreffor-0.5.3/src/python/compreffor.egg-info/SOURCES.txt` & `compreffor-0.5.4/src/python/compreffor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `compreffor-0.5.3/tools/analyzer.py` & `compreffor-0.5.4/tools/analyzer.py`

 * *Files identical despite different names*

### Comparing `compreffor-0.5.3/tools/gen_data.py` & `compreffor-0.5.4/tools/gen_data.py`

 * *Files identical despite different names*

### Comparing `compreffor-0.5.3/tools/optimizeParameter.py` & `compreffor-0.5.4/tools/optimizeParameter.py`

 * *Files identical despite different names*

### Comparing `compreffor-0.5.3/tools/simpleCffCompressor.py` & `compreffor-0.5.4/tools/simpleCffCompressor.py`

 * *Files identical despite different names*

### Comparing `compreffor-0.5.3/tools/subr_grapher.py` & `compreffor-0.5.4/tools/subr_grapher.py`

 * *Files identical despite different names*

