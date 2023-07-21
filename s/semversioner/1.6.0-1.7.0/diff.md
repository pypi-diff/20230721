# Comparing `tmp/semversioner-1.6.0.tar.gz` & `tmp/semversioner-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/semversioner-1.6.0.tar", last modified: Fri Jan 20 10:52:32 2023, max compression
+gzip compressed data, was "dist/semversioner-1.7.0.tar", last modified: Fri Jul 21 09:25:04 2023, max compression
```

## Comparing `semversioner-1.6.0.tar` & `semversioner-1.7.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 10:52:32.000000 semversioner-1.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-01-20 10:52:15.000000 semversioner-1.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-01-20 10:52:15.000000 semversioner-1.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10117 2023-01-20 10:52:32.000000 semversioner-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-01-20 10:52:15.000000 semversioner-1.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-01-20 10:52:15.000000 semversioner-1.6.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 10:52:32.000000 semversioner-1.6.0/semversioner/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-01-20 10:52:15.000000 semversioner-1.6.0/semversioner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-01-20 10:52:31.000000 semversioner-1.6.0/semversioner/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5347 2023-01-20 10:52:15.000000 semversioner-1.6.0/semversioner/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5688 2023-01-20 10:52:15.000000 semversioner-1.6.0/semversioner/core.py
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-01-20 10:52:15.000000 semversioner-1.6.0/semversioner/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     6350 2023-01-20 10:52:15.000000 semversioner-1.6.0/semversioner/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 10:52:32.000000 semversioner-1.6.0/semversioner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10117 2023-01-20 10:52:32.000000 semversioner-1.6.0/semversioner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-01-20 10:52:32.000000 semversioner-1.6.0/semversioner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-20 10:52:32.000000 semversioner-1.6.0/semversioner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-01-20 10:52:32.000000 semversioner-1.6.0/semversioner.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-01-20 10:52:32.000000 semversioner-1.6.0/semversioner.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-01-20 10:52:32.000000 semversioner-1.6.0/semversioner.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-01-20 10:52:32.000000 semversioner-1.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-01-20 10:52:15.000000 semversioner-1.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 10:52:32.000000 semversioner-1.6.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 10:52:32.000000 semversioner-1.6.0/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-20 10:52:15.000000 semversioner-1.6.0/tests/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:25:04.000000 semversioner-1.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-21 09:24:50.000000 semversioner-1.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-21 09:24:50.000000 semversioner-1.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10277 2023-07-21 09:25:04.000000 semversioner-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-07-21 09:24:50.000000 semversioner-1.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-21 09:24:50.000000 semversioner-1.7.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:25:04.000000 semversioner-1.7.0/semversioner/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-21 09:24:50.000000 semversioner-1.7.0/semversioner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-21 09:25:02.000000 semversioner-1.7.0/semversioner/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5347 2023-07-21 09:24:50.000000 semversioner-1.7.0/semversioner/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5688 2023-07-21 09:24:50.000000 semversioner-1.7.0/semversioner/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-07-21 09:24:50.000000 semversioner-1.7.0/semversioner/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7493 2023-07-21 09:24:50.000000 semversioner-1.7.0/semversioner/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:25:04.000000 semversioner-1.7.0/semversioner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10277 2023-07-21 09:25:04.000000 semversioner-1.7.0/semversioner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-21 09:25:04.000000 semversioner-1.7.0/semversioner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 09:25:04.000000 semversioner-1.7.0/semversioner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-21 09:25:04.000000 semversioner-1.7.0/semversioner.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-21 09:25:04.000000 semversioner-1.7.0/semversioner.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-21 09:25:04.000000 semversioner-1.7.0/semversioner.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-21 09:25:04.000000 semversioner-1.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-07-21 09:24:50.000000 semversioner-1.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:25:04.000000 semversioner-1.7.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:25:04.000000 semversioner-1.7.0/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 09:24:50.000000 semversioner-1.7.0/tests/resources/__init__.py
```

### Comparing `semversioner-1.6.0/LICENSE` & `semversioner-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `semversioner-1.6.0/PKG-INFO` & `semversioner-1.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: semversioner
-Version: 1.6.0
+Version: 1.7.0
 Summary: Manage properly semver in your repository
 Home-page: https://github.com/raulgomis/semversioner
 Author: Raul Gomis
 Author-email: raulgomis@gmail.com
 License: MIT
 Description: # Semversioner
         The easiest way to manage [semantic versioning](https://semver.org/) in your project and generate CHANGELOG.md file automatically. 
@@ -118,14 +118,19 @@
         ---
         Made with ♥ by `Raul Gomis <https://twitter.com/rgomis>`.
         
         
         # Changelog
         Note: version releases in the 0.x.y range may introduce breaking changes.
         
+        ## 1.7.0
+        
+        - minor: Validated JSON extension in the  folder.
+        - patch: Upgraded development libraries to latest version.
+        
         ## 1.6.0
         
         - minor: Decreased packaging minimum version requirements to version 21.0
         
         ## 1.5.2
         
         - patch: Internal: improve CI/CD workflow
```

### Comparing `semversioner-1.6.0/README.md` & `semversioner-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `semversioner-1.6.0/semversioner/cli.py` & `semversioner-1.7.0/semversioner/cli.py`

 * *Files identical despite different names*

### Comparing `semversioner-1.6.0/semversioner/core.py` & `semversioner-1.7.0/semversioner/core.py`

 * *Files identical despite different names*

### Comparing `semversioner-1.6.0/semversioner/models.py` & `semversioner-1.7.0/semversioner/models.py`

 * *Files identical despite different names*

### Comparing `semversioner-1.6.0/semversioner.egg-info/PKG-INFO` & `semversioner-1.7.0/semversioner.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: semversioner
-Version: 1.6.0
+Version: 1.7.0
 Summary: Manage properly semver in your repository
 Home-page: https://github.com/raulgomis/semversioner
 Author: Raul Gomis
 Author-email: raulgomis@gmail.com
 License: MIT
 Description: # Semversioner
         The easiest way to manage [semantic versioning](https://semver.org/) in your project and generate CHANGELOG.md file automatically. 
@@ -118,14 +118,19 @@
         ---
         Made with ♥ by `Raul Gomis <https://twitter.com/rgomis>`.
         
         
         # Changelog
         Note: version releases in the 0.x.y range may introduce breaking changes.
         
+        ## 1.7.0
+        
+        - minor: Validated JSON extension in the  folder.
+        - patch: Upgraded development libraries to latest version.
+        
         ## 1.6.0
         
         - minor: Decreased packaging minimum version requirements to version 21.0
         
         ## 1.5.2
         
         - patch: Internal: improve CI/CD workflow
```

### Comparing `semversioner-1.6.0/setup.py` & `semversioner-1.7.0/setup.py`

 * *Files identical despite different names*

