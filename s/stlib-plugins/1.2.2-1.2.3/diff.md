# Comparing `tmp/stlib-plugins-1.2.2.tar.gz` & `tmp/stlib-plugins-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stlib-plugins-1.2.2.tar", last modified: Fri Mar 31 22:02:58 2023, max compression
+gzip compressed data, was "stlib-plugins-1.2.3.tar", last modified: Thu Jul 20 22:08:48 2023, max compression
```

## Comparing `stlib-plugins-1.2.2.tar` & `stlib-plugins-1.2.3.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 22:02:58.298461 stlib-plugins-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-31 22:02:46.000000 stlib-plugins-1.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-03-31 22:02:58.298461 stlib-plugins-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-03-31 22:02:46.000000 stlib-plugins-1.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-03-31 22:02:46.000000 stlib-plugins-1.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-31 22:02:58.298461 stlib-plugins-1.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 22:02:58.294461 stlib-plugins-1.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 22:02:58.298461 stlib-plugins-1.2.2/src/stlib-plugins/
--rw-r--r--   0 runner    (1001) docker     (123)    10197 2023-03-31 22:02:46.000000 stlib-plugins-1.2.2/src/stlib-plugins/steamgifts.py
--rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-03-31 22:02:46.000000 stlib-plugins-1.2.2/src/stlib-plugins/steamtrades.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 22:02:58.298461 stlib-plugins-1.2.2/src/stlib_plugins.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-03-31 22:02:58.000000 stlib-plugins-1.2.2/src/stlib_plugins.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-03-31 22:02:58.000000 stlib-plugins-1.2.2/src/stlib_plugins.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 22:02:58.000000 stlib-plugins-1.2.2/src/stlib_plugins.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-31 22:02:58.000000 stlib-plugins-1.2.2/src/stlib_plugins.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-31 22:02:58.000000 stlib-plugins-1.2.2/src/stlib_plugins.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:08:48.495576 stlib-plugins-1.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-20 22:08:37.000000 stlib-plugins-1.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-07-20 22:08:48.495576 stlib-plugins-1.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-07-20 22:08:37.000000 stlib-plugins-1.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-20 22:08:37.000000 stlib-plugins-1.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 22:08:48.495576 stlib-plugins-1.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:08:48.491576 stlib-plugins-1.2.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:08:48.495576 stlib-plugins-1.2.3/src/stlib-plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 22:08:37.000000 stlib-plugins-1.2.3/src/stlib-plugins/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    10117 2023-07-20 22:08:37.000000 stlib-plugins-1.2.3/src/stlib-plugins/steamgifts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-07-20 22:08:37.000000 stlib-plugins-1.2.3/src/stlib-plugins/steamtrades.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:08:48.495576 stlib-plugins-1.2.3/src/stlib_plugins.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-07-20 22:08:48.000000 stlib-plugins-1.2.3/src/stlib_plugins.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-20 22:08:48.000000 stlib-plugins-1.2.3/src/stlib_plugins.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 22:08:48.000000 stlib-plugins-1.2.3/src/stlib_plugins.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-20 22:08:48.000000 stlib-plugins-1.2.3/src/stlib_plugins.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-20 22:08:48.000000 stlib-plugins-1.2.3/src/stlib_plugins.egg-info/top_level.txt
```

### Comparing `stlib-plugins-1.2.2/PKG-INFO` & `stlib-plugins-1.2.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stlib-plugins
-Version: 1.2.2
+Version: 1.2.3
 Summary: Official stlib plugins
 Author: Lara Maia
 Author-email: dev@lara.monster
 License: GPLv3
 Project-URL: homepage, https://github.com/calendulish/stlib-plugins
 Project-URL: repository, https://github.com
 Project-URL: changelog, https://github.com/calendulish/stlib-plugins/releases
@@ -15,14 +15,15 @@
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Typing :: Typed
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 Official stlib plugins
 ======================
```

### Comparing `stlib-plugins-1.2.2/README.md` & `stlib-plugins-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `stlib-plugins-1.2.2/pyproject.toml` & `stlib-plugins-1.2.3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "stlib-plugins"
-version = "1.2.2"
+version = "1.2.3"
 description = "Official stlib plugins"
 readme = "README.md"
 requires-python = ">=3.9"
 license = {text = "GPLv3"}
 keywords = ["steam-tools", "steam", "stlib", "valve"]
 authors = [{email = "dev@lara.monster"}, {name = "Lara Maia"}]
 classifiers = [
@@ -18,17 +18,18 @@
   "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
   "Operating System :: POSIX :: Linux",
   "Operating System :: Microsoft :: Windows",
   "Programming Language :: Python :: 3 :: Only",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: 3.12",
   "Typing :: Typed"
 ]
 
-dependencies = ["stlib~=1.3.0"]
+dependencies = ["stlib~=2.0"]
 
 [project.urls]
 homepage = "https://github.com/calendulish/stlib-plugins"
 repository = "https://github.com"
 changelog = "https://github.com/calendulish/stlib-plugins/releases"
```

### Comparing `stlib-plugins-1.2.2/src/stlib-plugins/steamgifts.py` & `stlib-plugins-1.2.3/src/stlib-plugins/steamgifts.py`

 * *Files 1% similar despite different names*

```diff
@@ -216,28 +216,26 @@
                 giveaways_raw += pinned.findAll('div', class_='giveaway__row-outer-wrap')
 
         for giveaway in giveaways_raw:
             if giveaway.find('div', class_='is-faded'):
                 continue
 
             temp_head = giveaway.find('a', class_='giveaway__heading__name')
-            name = temp_head.text[:22] + '...'
+            name = f'{temp_head.text[:22]}...'
             query = temp_head['href']
             id_ = temp_head['href'].split('/')[2]
 
             temp_head = giveaway.find('span', class_='giveaway__heading__thin')
 
             if 'Copies' in temp_head.text:
                 copies = int(''.join(filter(str.isdigit, temp_head.text)))
                 temp_head = temp_head.findNext('span', class_='giveaway__heading__thin')
-                points = int(''.join(filter(str.isdigit, temp_head.text)))
             else:
                 copies = 1
-                points = int(''.join(filter(str.isdigit, temp_head.text)))
-
+            points = int(''.join(filter(str.isdigit, temp_head.text)))
             try:
                 level_column = giveaway.find('div', class_='giveaway__column--contributor-level')
                 level = int(''.join(filter(str.isdigit, level_column.text)))
             except AttributeError:
                 level = 0
 
             if not return_unavailable and (user_level < level or user_points < points):
```

### Comparing `stlib-plugins-1.2.2/src/stlib-plugins/steamtrades.py` & `stlib-plugins-1.2.3/src/stlib-plugins/steamtrades.py`

 * *Files identical despite different names*

### Comparing `stlib-plugins-1.2.2/src/stlib_plugins.egg-info/PKG-INFO` & `stlib-plugins-1.2.3/src/stlib_plugins.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stlib-plugins
-Version: 1.2.2
+Version: 1.2.3
 Summary: Official stlib plugins
 Author: Lara Maia
 Author-email: dev@lara.monster
 License: GPLv3
 Project-URL: homepage, https://github.com/calendulish/stlib-plugins
 Project-URL: repository, https://github.com
 Project-URL: changelog, https://github.com/calendulish/stlib-plugins/releases
@@ -15,14 +15,15 @@
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Typing :: Typed
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 Official stlib plugins
 ======================
```

