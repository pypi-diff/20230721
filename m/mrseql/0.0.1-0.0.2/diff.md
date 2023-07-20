# Comparing `tmp/mrseql-0.0.1.tar.gz` & `tmp/mrseql-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mrseql-0.0.1.tar", last modified: Thu Jul 20 12:11:11 2023, max compression
+gzip compressed data, was "mrseql-0.0.2.tar", last modified: Thu Jul 20 22:05:07 2023, max compression
```

## Comparing `mrseql-0.0.1.tar` & `mrseql-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:11:11.431764 mrseql-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-20 12:10:30.000000 mrseql-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-20 12:11:11.431764 mrseql-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-20 12:10:30.000000 mrseql-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     6224 2023-07-20 12:10:30.000000 mrseql-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 12:11:11.431764 mrseql-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-07-20 12:10:30.000000 mrseql-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:11:11.431764 mrseql-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:11:11.431764 mrseql-0.0.1/src/mrseql/
--rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-07-20 12:10:30.000000 mrseql-0.0.1/src/mrseql/SNode.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-20 12:10:30.000000 mrseql-0.0.1/src/mrseql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   918750 2023-07-20 12:10:51.000000 mrseql-0.0.1/src/mrseql/mrseql.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    57878 2023-07-20 12:10:30.000000 mrseql-0.0.1/src/mrseql/seql_learn.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:11:11.431764 mrseql-0.0.1/src/mrseql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-20 12:11:11.000000 mrseql-0.0.1/src/mrseql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-20 12:11:11.000000 mrseql-0.0.1/src/mrseql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 12:11:11.000000 mrseql-0.0.1/src/mrseql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-20 12:11:11.000000 mrseql-0.0.1/src/mrseql.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:05:07.140429 mrseql-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-20 22:04:36.000000 mrseql-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-20 22:04:36.000000 mrseql-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-20 22:05:07.140429 mrseql-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-20 22:04:36.000000 mrseql-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6224 2023-07-20 22:04:36.000000 mrseql-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 22:05:07.140429 mrseql-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-07-20 22:04:36.000000 mrseql-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:05:07.136429 mrseql-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:05:07.140429 mrseql-0.0.2/src/mrseql/
+-rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-07-20 22:04:36.000000 mrseql-0.0.2/src/mrseql/SNode.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-07-20 22:04:36.000000 mrseql-0.0.2/src/mrseql/SNode.h
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-20 22:04:36.000000 mrseql-0.0.2/src/mrseql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-07-20 22:04:36.000000 mrseql-0.0.2/src/mrseql/common.h
+-rw-r--r--   0 runner    (1001) docker     (123)   918750 2023-07-20 22:04:48.000000 mrseql-0.0.2/src/mrseql/mrseql.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    15201 2023-07-20 22:04:36.000000 mrseql-0.0.2/src/mrseql/mrseql.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    13417 2023-07-20 22:04:36.000000 mrseql-0.0.2/src/mrseql/sax_converter.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8626 2023-07-20 22:04:36.000000 mrseql-0.0.2/src/mrseql/seql.h
+-rw-r--r--   0 runner    (1001) docker     (123)    57878 2023-07-20 22:04:36.000000 mrseql-0.0.2/src/mrseql/seql_learn.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9278 2023-07-20 22:04:36.000000 mrseql-0.0.2/src/mrseql/seql_learn.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:05:07.140429 mrseql-0.0.2/src/mrseql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-20 22:05:07.000000 mrseql-0.0.2/src/mrseql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-20 22:05:07.000000 mrseql-0.0.2/src/mrseql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 22:05:07.000000 mrseql-0.0.2/src/mrseql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-20 22:05:07.000000 mrseql-0.0.2/src/mrseql.egg-info/top_level.txt
```

### Comparing `mrseql-0.0.1/LICENSE` & `mrseql-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mrseql-0.0.1/README.md` & `mrseql-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `mrseql-0.0.1/pyproject.toml` & `mrseql-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mrseql-0.0.1/setup.py` & `mrseql-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
                    language='c++',
                    sources=["src/mrseql/mrseql.pyx", "src/mrseql/seql_learn.cpp", "src/mrseql/SNode.cpp"],
                    extra_compile_args=["-std=c++11"],                   
                    include_dirs=['src/mrseql'])
 
 setup(
     name='mrseql',
-    version="0.0.1",
+    version="0.0.2",
     author='Thach Le Nguyen',
     author_email='thalng@protonmail.com',
     setup_requires=[
         'setuptools',  
         'cython',
         'sktime',
     ],
```

### Comparing `mrseql-0.0.1/src/mrseql/SNode.cpp` & `mrseql-0.0.2/src/mrseql/SNode.cpp`

 * *Files identical despite different names*

### Comparing `mrseql-0.0.1/src/mrseql/mrseql.cpp` & `mrseql-0.0.2/src/mrseql/mrseql.cpp`

 * *Files identical despite different names*

### Comparing `mrseql-0.0.1/src/mrseql/seql_learn.cpp` & `mrseql-0.0.2/src/mrseql/seql_learn.cpp`

 * *Files identical despite different names*

