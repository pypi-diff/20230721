# Comparing `tmp/database-without-orm-local-0.0.13.tar.gz` & `tmp/database-without-orm-local-0.0.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "database-without-orm-local-0.0.13.tar", last modified: Thu Jul 20 14:16:34 2023, max compression
+gzip compressed data, was "database-without-orm-local-0.0.14.tar", last modified: Fri Jul 21 11:07:09 2023, max compression
```

## Comparing `database-without-orm-local-0.0.13.tar` & `database-without-orm-local-0.0.14.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:16:34.758581 database-without-orm-local-0.0.13/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 14:16:09.000000 database-without-orm-local-0.0.13/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-20 14:16:34.758581 database-without-orm-local-0.0.13/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:16:34.754581 database-without-orm-local-0.0.13/circles_local_database_python/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 14:16:09.000000 database-without-orm-local-0.0.13/circles_local_database_python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-07-20 14:16:09.000000 database-without-orm-local-0.0.13/circles_local_database_python/database.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:16:34.758581 database-without-orm-local-0.0.13/database_without_orm_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-20 14:16:34.000000 database-without-orm-local-0.0.13/database_without_orm_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-20 14:16:34.000000 database-without-orm-local-0.0.13/database_without_orm_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 14:16:34.000000 database-without-orm-local-0.0.13/database_without_orm_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-20 14:16:34.000000 database-without-orm-local-0.0.13/database_without_orm_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-20 14:16:09.000000 database-without-orm-local-0.0.13/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 14:16:34.758581 database-without-orm-local-0.0.13/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-07-20 14:16:09.000000 database-without-orm-local-0.0.13/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:07:09.414882 database-without-orm-local-0.0.14/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 11:06:44.000000 database-without-orm-local-0.0.14/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-21 11:07:09.414882 database-without-orm-local-0.0.14/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:07:09.414882 database-without-orm-local-0.0.14/circles_local_database_python/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 11:06:44.000000 database-without-orm-local-0.0.14/circles_local_database_python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-07-21 11:06:44.000000 database-without-orm-local-0.0.14/circles_local_database_python/database.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:07:09.414882 database-without-orm-local-0.0.14/database_without_orm_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-21 11:07:09.000000 database-without-orm-local-0.0.14/database_without_orm_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-21 11:07:09.000000 database-without-orm-local-0.0.14/database_without_orm_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 11:07:09.000000 database-without-orm-local-0.0.14/database_without_orm_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-21 11:07:09.000000 database-without-orm-local-0.0.14/database_without_orm_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-21 11:06:44.000000 database-without-orm-local-0.0.14/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 11:07:09.414882 database-without-orm-local-0.0.14/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-07-21 11:06:44.000000 database-without-orm-local-0.0.14/setup.py
```

### Comparing `database-without-orm-local-0.0.13/circles_local_database_python/database.py` & `database-without-orm-local-0.0.14/circles_local_database_python/database.py`

 * *Files identical despite different names*

### Comparing `database-without-orm-local-0.0.13/setup.py` & `database-without-orm-local-0.0.14/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 # used by python -m build
 setuptools.setup(
      name='database-without-orm-local',  
-     version='0.0.13', # https://pypi.org/project/database-without-orm-local/
+     version='0.0.14', # https://pypi.org/project/database-without-orm-local/
      author="Circles",
      author_email="info@circles.life",
      description="Circles Local Database without ORM Python PyPI Package",
      long_description="This is a package for sharing common Database methods",
      long_description_content_type="text/markdown",
      url="https://github.com/javatechy/dokr",
      packages=setuptools.find_packages(),
```

