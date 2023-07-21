# Comparing `tmp/bcmd-0.0.2.tar.gz` & `tmp/bcmd-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bcmd-0.0.2.tar", last modified: Fri Jul 21 02:30:47 2023, max compression
+gzip compressed data, was "bcmd-0.0.3.tar", last modified: Fri Jul 21 02:41:45 2023, max compression
```

## Comparing `bcmd-0.0.2.tar` & `bcmd-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-21 02:30:47.586079 bcmd-0.0.2/
--rw-rw-rw-   0        0        0      239 2023-07-21 02:30:47.585078 bcmd-0.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-21 02:30:47.576028 bcmd-0.0.2/bcmd/
--rw-rw-rw-   0        0        0        0 2023-07-21 02:19:54.000000 bcmd-0.0.2/bcmd/__init__.py
--rw-rw-rw-   0        0        0      430 2023-07-20 07:37:53.000000 bcmd-0.0.2/bcmd/dev.py
--rw-rw-rw-   0        0        0      148 2023-07-21 02:23:43.000000 bcmd-0.0.2/bcmd/main.py
-drwxrwxrwx   0        0        0        0 2023-07-21 02:30:47.584079 bcmd-0.0.2/bcmd/tasks/
--rw-rw-rw-   0        0        0        0 2023-07-20 07:37:38.000000 bcmd-0.0.2/bcmd/tasks/__init__.py
--rw-rw-rw-   0        0        0     2488 2023-07-21 02:02:14.000000 bcmd-0.0.2/bcmd/tasks/time.py
-drwxrwxrwx   0        0        0        0 2023-07-21 02:30:47.583077 bcmd-0.0.2/bcmd.egg-info/
--rw-rw-rw-   0        0        0      239 2023-07-21 02:30:47.000000 bcmd-0.0.2/bcmd.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      268 2023-07-21 02:30:47.000000 bcmd-0.0.2/bcmd.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 02:30:47.000000 bcmd-0.0.2/bcmd.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-07-21 02:30:47.000000 bcmd-0.0.2/bcmd.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      149 2023-07-21 02:30:47.000000 bcmd-0.0.2/bcmd.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-07-21 02:30:47.000000 bcmd-0.0.2/bcmd.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      622 2023-07-21 02:30:04.000000 bcmd-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-21 02:30:47.586079 bcmd-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-21 02:41:45.947798 bcmd-0.0.3/
+-rw-rw-rw-   0        0        0      239 2023-07-21 02:41:45.946798 bcmd-0.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-21 02:41:45.937795 bcmd-0.0.3/bcmd/
+-rw-rw-rw-   0        0        0        0 2023-07-21 02:19:54.000000 bcmd-0.0.3/bcmd/__init__.py
+-rw-rw-rw-   0        0        0      430 2023-07-20 07:37:53.000000 bcmd-0.0.3/bcmd/dev.py
+-rw-rw-rw-   0        0        0      148 2023-07-21 02:23:43.000000 bcmd-0.0.3/bcmd/main.py
+drwxrwxrwx   0        0        0        0 2023-07-21 02:41:45.945797 bcmd-0.0.3/bcmd/tasks/
+-rw-rw-rw-   0        0        0        0 2023-07-20 07:37:38.000000 bcmd-0.0.3/bcmd/tasks/__init__.py
+-rw-rw-rw-   0        0        0     2488 2023-07-21 02:02:14.000000 bcmd-0.0.3/bcmd/tasks/time.py
+drwxrwxrwx   0        0        0        0 2023-07-21 02:41:45.943796 bcmd-0.0.3/bcmd.egg-info/
+-rw-rw-rw-   0        0        0      239 2023-07-21 02:41:45.000000 bcmd-0.0.3/bcmd.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      268 2023-07-21 02:41:45.000000 bcmd-0.0.3/bcmd.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 02:41:45.000000 bcmd-0.0.3/bcmd.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-07-21 02:41:45.000000 bcmd-0.0.3/bcmd.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      149 2023-07-21 02:41:45.000000 bcmd-0.0.3/bcmd.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-07-21 02:41:45.000000 bcmd-0.0.3/bcmd.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      622 2023-07-21 02:40:44.000000 bcmd-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-21 02:41:45.947798 bcmd-0.0.3/setup.cfg
```

### Comparing `bcmd-0.0.2/bcmd/tasks/time.py` & `bcmd-0.0.3/bcmd/tasks/time.py`

 * *Files identical despite different names*

### Comparing `bcmd-0.0.2/pyproject.toml` & `bcmd-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # https://peps.python.org/pep-0621/#example
 
 [project]
 name = "bcmd"
-version = "0.0.2"
+version = "0.0.3"
 description = "Utils commands for Beni"
 requires-python = ">=3.10"
 keywords = ["benimang", "beni", "bcmd"]
 authors = [
   {email = "benimang@126.com"},
   {name = "Beni Mang"}
 ]
@@ -30,8 +30,8 @@
   'qiniu',
   'twine',
   'typer',
   'tzdata',
 ]
 
 [project.scripts]
-beni = "bcmd.main:run"
+bcmd = "bcmd.main:run"
```

