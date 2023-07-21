# Comparing `tmp/vaex-4.9.1.tar.gz` & `tmp/vaex-4.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/vaex-4.9.1.tar", last modified: Tue Apr 12 15:42:53 2022, max compression
+gzip compressed data, was "dist/vaex-4.9.2.tar", last modified: Fri Jun  3 14:51:43 2022, max compression
```

## Comparing `vaex-4.9.1.tar` & `vaex-4.9.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-04-12 15:42:53.000000 vaex-4.9.1/
--rw-r--r--   0 runner    (1001) docker     (116)     1087 2022-04-12 15:42:43.000000 vaex-4.9.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (116)       19 2022-04-12 15:42:43.000000 vaex-4.9.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     6392 2022-04-12 15:42:53.000000 vaex-4.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     5259 2022-04-12 15:42:52.000000 vaex-4.9.1/README.md
--rw-r--r--   0 runner    (1001) docker     (116)       38 2022-04-12 15:42:53.000000 vaex-4.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1135 2022-04-12 15:42:43.000000 vaex-4.9.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-04-12 15:42:53.000000 vaex-4.9.1/vaex/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-04-12 15:42:53.000000 vaex-4.9.1/vaex/meta/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-04-12 15:42:43.000000 vaex-4.9.1/vaex/meta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)       52 2022-04-12 15:42:43.000000 vaex-4.9.1/vaex/meta/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-04-12 15:42:53.000000 vaex-4.9.1/vaex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     6392 2022-04-12 15:42:53.000000 vaex-4.9.1/vaex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      252 2022-04-12 15:42:53.000000 vaex-4.9.1/vaex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-04-12 15:42:53.000000 vaex-4.9.1/vaex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-04-12 15:42:53.000000 vaex-4.9.1/vaex.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)      163 2022-04-12 15:42:53.000000 vaex-4.9.1/vaex.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        5 2022-04-12 15:42:53.000000 vaex-4.9.1/vaex.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-03 14:51:43.000000 vaex-4.9.2/
+-rw-r--r--   0 runner    (1001) docker     (116)     1087 2022-06-03 14:51:32.000000 vaex-4.9.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       19 2022-06-03 14:51:32.000000 vaex-4.9.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (116)     6392 2022-06-03 14:51:43.000000 vaex-4.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     5259 2022-06-03 14:51:42.000000 vaex-4.9.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (116)       38 2022-06-03 14:51:43.000000 vaex-4.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)     1135 2022-06-03 14:51:32.000000 vaex-4.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-03 14:51:43.000000 vaex-4.9.2/vaex/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-03 14:51:43.000000 vaex-4.9.2/vaex/meta/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2022-06-03 14:51:32.000000 vaex-4.9.2/vaex/meta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)       52 2022-06-03 14:51:32.000000 vaex-4.9.2/vaex/meta/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-03 14:51:43.000000 vaex-4.9.2/vaex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)     6392 2022-06-03 14:51:43.000000 vaex-4.9.2/vaex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)      252 2022-06-03 14:51:43.000000 vaex-4.9.2/vaex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2022-06-03 14:51:43.000000 vaex-4.9.2/vaex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2022-06-03 14:51:43.000000 vaex-4.9.2/vaex.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (116)      163 2022-06-03 14:51:43.000000 vaex-4.9.2/vaex.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        5 2022-06-03 14:51:43.000000 vaex-4.9.2/vaex.egg-info/top_level.txt
```

### Comparing `vaex-4.9.1/LICENSE.txt` & `vaex-4.9.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vaex-4.9.1/PKG-INFO` & `vaex-4.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vaex
-Version: 4.9.1
+Version: 4.9.2
 Summary: Out-of-Core DataFrames to visualize and explore big tabular datasets
 Home-page: https://www.github.com/vaexio/vaex
 Author: Maarten A. Breddels
 Author-email: maartenbreddels@gmail.com
 License: MIT
 Description: 
         [![Documentation](https://readthedocs.org/projects/vaex/badge/?version=latest)](https://docs.vaex.io)
```

### Comparing `vaex-4.9.1/README.md` & `vaex-4.9.2/README.md`

 * *Files identical despite different names*

### Comparing `vaex-4.9.1/setup.py` & `vaex-4.9.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,20 +12,20 @@
 author = 'Maarten A. Breddels'
 author_email = 'maartenbreddels@gmail.com'
 license = 'MIT'
 version = version.__version__
 url = 'https://www.github.com/vaexio/vaex'
 
 install_requires = [
-      'vaex-core>=4.9.1,<4.10',
+      'vaex-core>=4.9.2,<4.10',
       'vaex-astro>=0.9.1,<0.10',
-      'vaex-hdf5>=0.12.1,<0.13',
-      'vaex-viz>=0.5.1,<0.6',
+      'vaex-hdf5>=0.12.2,<0.13',
+      'vaex-viz>=0.5.2,<0.6',
       'vaex-server>=0.8.1,<0.9',
-      'vaex-jupyter>=0.7.0,<0.8',
+      'vaex-jupyter>=0.8.0,<0.9',
       'vaex-ml>=0.17.0,<0.18',
       # vaex-graphql is not on conda-forge yet
 ]
 
 setup(name=name,
       version=version,
       description='Out-of-Core DataFrames to visualize and explore big tabular datasets',
```

### Comparing `vaex-4.9.1/vaex.egg-info/PKG-INFO` & `vaex-4.9.2/vaex.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vaex
-Version: 4.9.1
+Version: 4.9.2
 Summary: Out-of-Core DataFrames to visualize and explore big tabular datasets
 Home-page: https://www.github.com/vaexio/vaex
 Author: Maarten A. Breddels
 Author-email: maartenbreddels@gmail.com
 License: MIT
 Description: 
         [![Documentation](https://readthedocs.org/projects/vaex/badge/?version=latest)](https://docs.vaex.io)
```

