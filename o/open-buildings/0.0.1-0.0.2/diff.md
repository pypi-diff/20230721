# Comparing `tmp/open-buildings-0.0.1.tar.gz` & `tmp/open-buildings-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open-buildings-0.0.1.tar", last modified: Fri Jul 21 14:21:46 2023, max compression
+gzip compressed data, was "open-buildings-0.0.2.tar", last modified: Fri Jul 21 14:48:10 2023, max compression
```

## Comparing `open-buildings-0.0.1.tar` & `open-buildings-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:21:46.697168 open-buildings-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-21 14:21:29.000000 open-buildings-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-21 14:21:29.000000 open-buildings-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-07-21 14:21:46.697168 open-buildings-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-21 14:21:29.000000 open-buildings-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:21:46.693168 open-buildings-0.0.1/open_buildings/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-21 14:21:29.000000 open-buildings-0.0.1/open_buildings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-21 14:21:29.000000 open-buildings-0.0.1/open_buildings/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-21 14:21:29.000000 open-buildings-0.0.1/open_buildings/common.py
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-21 14:21:29.000000 open-buildings-0.0.1/open_buildings/open_buildings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:21:46.697168 open-buildings-0.0.1/open_buildings.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-07-21 14:21:46.000000 open-buildings-0.0.1/open_buildings.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-21 14:21:46.000000 open-buildings-0.0.1/open_buildings.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-21 14:21:46.000000 open-buildings-0.0.1/open_buildings.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-21 14:21:46.000000 open-buildings-0.0.1/open_buildings.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 14:21:46.000000 open-buildings-0.0.1/open_buildings.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-21 14:21:46.000000 open-buildings-0.0.1/open_buildings.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-21 14:21:46.000000 open-buildings-0.0.1/open_buildings.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-21 14:21:29.000000 open-buildings-0.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-21 14:21:46.697168 open-buildings-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-07-21 14:21:29.000000 open-buildings-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:48:10.796347 open-buildings-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-21 14:48:00.000000 open-buildings-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-21 14:48:00.000000 open-buildings-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11086 2023-07-21 14:48:10.796347 open-buildings-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10323 2023-07-21 14:48:00.000000 open-buildings-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:48:10.792347 open-buildings-0.0.2/open_buildings/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-21 14:48:00.000000 open-buildings-0.0.2/open_buildings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-21 14:48:00.000000 open-buildings-0.0.2/open_buildings/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-21 14:48:00.000000 open-buildings-0.0.2/open_buildings/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19650 2023-07-21 14:48:00.000000 open-buildings-0.0.2/open_buildings/open_buildings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:48:10.792347 open-buildings-0.0.2/open_buildings.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11086 2023-07-21 14:48:10.000000 open-buildings-0.0.2/open_buildings.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-21 14:48:10.000000 open-buildings-0.0.2/open_buildings.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-21 14:48:10.000000 open-buildings-0.0.2/open_buildings.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-21 14:48:10.000000 open-buildings-0.0.2/open_buildings.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 14:48:10.000000 open-buildings-0.0.2/open_buildings.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-21 14:48:10.000000 open-buildings-0.0.2/open_buildings.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-21 14:48:10.000000 open-buildings-0.0.2/open_buildings.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-21 14:48:00.000000 open-buildings-0.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-21 14:48:10.796347 open-buildings-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-07-21 14:48:00.000000 open-buildings-0.0.2/setup.py
```

### Comparing `open-buildings-0.0.1/LICENSE` & `open-buildings-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `open-buildings-0.0.1/setup.py` & `open-buildings-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 """The setup script."""
 
 import io
 from os import path as op
 from setuptools import setup, find_packages
 
-with open('README.md') as readme_file:
+with open('README.md', encoding="utf-8") as readme_file:
     readme = readme_file.read()
 
 here = op.abspath(op.dirname(__file__))
 
 # get the dependencies and installs
 with io.open(op.join(here, "requirements.txt"), encoding="utf-8") as f:
     all_reqs = f.read().split("\n")
@@ -53,10 +53,10 @@
     keywords='open_buildings',
     name='open-buildings',
     packages=find_packages(include=['open_buildings', 'open_buildings.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/opengeos/open-buildings',
-    version='0.0.1',
+    version='0.0.2',
     zip_safe=False,
 )
```

