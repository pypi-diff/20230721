# Comparing `tmp/kolibri_sync_extras_plugin-0.1.2.tar.gz` & `tmp/kolibri_sync_extras_plugin-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/kolibri_sync_extras_plugin-0.1.2.tar", last modified: Tue Aug  9 17:45:46 2022, max compression
+gzip compressed data, was "kolibri_sync_extras_plugin-0.1.3.tar", last modified: Fri Jul 21 16:30:14 2023, max compression
```

## Comparing `kolibri_sync_extras_plugin-0.1.2.tar` & `kolibri_sync_extras_plugin-0.1.3.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-09 17:45:46.000000 kolibri_sync_extras_plugin-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (116)      111 2022-08-09 17:45:46.000000 kolibri_sync_extras_plugin-0.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-09 17:45:46.000000 kolibri_sync_extras_plugin-0.1.2/kolibri_sync_extras_plugin/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-09 17:45:46.000000 kolibri_sync_extras_plugin-0.1.2/kolibri_sync_extras_plugin/management/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-09 17:45:46.000000 kolibri_sync_extras_plugin-0.1.2/kolibri_sync_extras_plugin/management/commands/
--rw-r--r--   0 runner    (1001) docker     (116)     2845 2022-08-09 17:45:31.000000 kolibri_sync_extras_plugin-0.1.2/kolibri_sync_extras_plugin/management/commands/sync_proceed_to.py
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-08-09 17:45:31.000000 kolibri_sync_extras_plugin-0.1.2/kolibri_sync_extras_plugin/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-08-09 17:45:31.000000 kolibri_sync_extras_plugin-0.1.2/kolibri_sync_extras_plugin/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-09 17:45:46.000000 kolibri_sync_extras_plugin-0.1.2/kolibri_sync_extras_plugin/sync/
--rw-r--r--   0 runner    (1001) docker     (116)     6018 2022-08-09 17:45:31.000000 kolibri_sync_extras_plugin-0.1.2/kolibri_sync_extras_plugin/sync/operations.py
--rw-r--r--   0 runner    (1001) docker     (116)      735 2022-08-09 17:45:31.000000 kolibri_sync_extras_plugin-0.1.2/kolibri_sync_extras_plugin/sync/context.py
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-08-09 17:45:31.000000 kolibri_sync_extras_plugin-0.1.2/kolibri_sync_extras_plugin/sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1761 2022-08-09 17:45:31.000000 kolibri_sync_extras_plugin-0.1.2/kolibri_sync_extras_plugin/kolibri_plugin.py
--rw-r--r--   0 runner    (1001) docker     (116)     1075 2022-08-09 17:45:31.000000 kolibri_sync_extras_plugin-0.1.2/kolibri_sync_extras_plugin/options.py
--rw-r--r--   0 runner    (1001) docker     (116)      848 2022-08-09 17:45:31.000000 kolibri_sync_extras_plugin-0.1.2/kolibri_sync_extras_plugin/tasks.py
--rw-r--r--   0 runner    (1001) docker     (116)       22 2022-08-09 17:45:31.000000 kolibri_sync_extras_plugin-0.1.2/kolibri_sync_extras_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2322 2022-08-09 17:45:31.000000 kolibri_sync_extras_plugin-0.1.2/setup.py
--rw-r--r--   0 runner    (1001) docker     (116)      247 2022-08-09 17:45:31.000000 kolibri_sync_extras_plugin-0.1.2/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (116)     1084 2022-08-09 17:45:31.000000 kolibri_sync_extras_plugin-0.1.2/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-09 17:45:46.000000 kolibri_sync_extras_plugin-0.1.2/test/
--rw-r--r--   0 runner    (1001) docker     (116)      769 2022-08-09 17:45:31.000000 kolibri_sync_extras_plugin-0.1.2/test/test_tasks.py
--rw-r--r--   0 runner    (1001) docker     (116)     1416 2022-08-09 17:45:46.000000 kolibri_sync_extras_plugin-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1650 2022-08-09 17:45:31.000000 kolibri_sync_extras_plugin-0.1.2/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (116)     2659 2022-08-09 17:45:31.000000 kolibri_sync_extras_plugin-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-09 17:45:46.000000 kolibri_sync_extras_plugin-0.1.2/kolibri_sync_extras_plugin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-08-09 17:45:45.000000 kolibri_sync_extras_plugin-0.1.2/kolibri_sync_extras_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-08-09 17:45:45.000000 kolibri_sync_extras_plugin-0.1.2/kolibri_sync_extras_plugin.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)     1416 2022-08-09 17:45:45.000000 kolibri_sync_extras_plugin-0.1.2/kolibri_sync_extras_plugin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)       27 2022-08-09 17:45:45.000000 kolibri_sync_extras_plugin-0.1.2/kolibri_sync_extras_plugin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       75 2022-08-09 17:45:45.000000 kolibri_sync_extras_plugin-0.1.2/kolibri_sync_extras_plugin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)       30 2022-08-09 17:45:45.000000 kolibri_sync_extras_plugin-0.1.2/kolibri_sync_extras_plugin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)      913 2022-08-09 17:45:45.000000 kolibri_sync_extras_plugin-0.1.2/kolibri_sync_extras_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)      181 2022-08-09 17:45:31.000000 kolibri_sync_extras_plugin-0.1.2/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:30:14.215951 kolibri_sync_extras_plugin-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-21 16:30:00.000000 kolibri_sync_extras_plugin-0.1.3/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-07-21 16:30:00.000000 kolibri_sync_extras_plugin-0.1.3/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-21 16:30:00.000000 kolibri_sync_extras_plugin-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-21 16:30:00.000000 kolibri_sync_extras_plugin-0.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-07-21 16:30:14.215951 kolibri_sync_extras_plugin-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-07-21 16:30:00.000000 kolibri_sync_extras_plugin-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:30:14.215951 kolibri_sync_extras_plugin-0.1.3/kolibri_sync_extras_plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-21 16:30:00.000000 kolibri_sync_extras_plugin-0.1.3/kolibri_sync_extras_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-07-21 16:30:00.000000 kolibri_sync_extras_plugin-0.1.3/kolibri_sync_extras_plugin/kolibri_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:30:14.215951 kolibri_sync_extras_plugin-0.1.3/kolibri_sync_extras_plugin/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:30:00.000000 kolibri_sync_extras_plugin-0.1.3/kolibri_sync_extras_plugin/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:30:14.215951 kolibri_sync_extras_plugin-0.1.3/kolibri_sync_extras_plugin/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:30:00.000000 kolibri_sync_extras_plugin-0.1.3/kolibri_sync_extras_plugin/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-07-21 16:30:00.000000 kolibri_sync_extras_plugin-0.1.3/kolibri_sync_extras_plugin/management/commands/sync_proceed_to.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-21 16:30:00.000000 kolibri_sync_extras_plugin-0.1.3/kolibri_sync_extras_plugin/options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:30:14.215951 kolibri_sync_extras_plugin-0.1.3/kolibri_sync_extras_plugin/sync/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:30:00.000000 kolibri_sync_extras_plugin-0.1.3/kolibri_sync_extras_plugin/sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-21 16:30:00.000000 kolibri_sync_extras_plugin-0.1.3/kolibri_sync_extras_plugin/sync/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6018 2023-07-21 16:30:00.000000 kolibri_sync_extras_plugin-0.1.3/kolibri_sync_extras_plugin/sync/operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-21 16:30:00.000000 kolibri_sync_extras_plugin-0.1.3/kolibri_sync_extras_plugin/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:30:14.215951 kolibri_sync_extras_plugin-0.1.3/kolibri_sync_extras_plugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-07-21 16:30:14.000000 kolibri_sync_extras_plugin-0.1.3/kolibri_sync_extras_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-21 16:30:14.000000 kolibri_sync_extras_plugin-0.1.3/kolibri_sync_extras_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 16:30:14.000000 kolibri_sync_extras_plugin-0.1.3/kolibri_sync_extras_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-21 16:30:14.000000 kolibri_sync_extras_plugin-0.1.3/kolibri_sync_extras_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 16:30:14.000000 kolibri_sync_extras_plugin-0.1.3/kolibri_sync_extras_plugin.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-21 16:30:14.000000 kolibri_sync_extras_plugin-0.1.3/kolibri_sync_extras_plugin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-21 16:30:14.000000 kolibri_sync_extras_plugin-0.1.3/kolibri_sync_extras_plugin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-21 16:30:14.219951 kolibri_sync_extras_plugin-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-07-21 16:30:00.000000 kolibri_sync_extras_plugin-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:30:14.215951 kolibri_sync_extras_plugin-0.1.3/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-07-21 16:30:00.000000 kolibri_sync_extras_plugin-0.1.3/test/test_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-07-21 16:30:00.000000 kolibri_sync_extras_plugin-0.1.3/test/test_tasks.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `kolibri_sync_extras_plugin-0.1.2/kolibri_sync_extras_plugin/management/commands/sync_proceed_to.py` & `kolibri_sync_extras_plugin-0.1.3/kolibri_sync_extras_plugin/management/commands/sync_proceed_to.py`

 * *Files identical despite different names*

### Comparing `kolibri_sync_extras_plugin-0.1.2/kolibri_sync_extras_plugin/sync/operations.py` & `kolibri_sync_extras_plugin-0.1.3/kolibri_sync_extras_plugin/sync/operations.py`

 * *Files identical despite different names*

### Comparing `kolibri_sync_extras_plugin-0.1.2/kolibri_sync_extras_plugin/sync/context.py` & `kolibri_sync_extras_plugin-0.1.3/kolibri_sync_extras_plugin/sync/context.py`

 * *Files identical despite different names*

### Comparing `kolibri_sync_extras_plugin-0.1.2/kolibri_sync_extras_plugin/kolibri_plugin.py` & `kolibri_sync_extras_plugin-0.1.3/kolibri_sync_extras_plugin/kolibri_plugin.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,9 +37,9 @@
         if self._finalize_operations is None:
             self._finalize_operations = [BackgroundFinalizeJobOperation()]
         return self._finalize_operations
 
     serializing_operations = property(get_initialize_operations)
     queuing_operations = property(get_initialize_operations)
     dequeuing_operations = property(get_finalize_operations)
-    deserializing_operations = property(get_initialize_operations)
+    deserializing_operations = property(get_finalize_operations)
     cleanup_operations = property(get_finalize_operations)
```

### Comparing `kolibri_sync_extras_plugin-0.1.2/kolibri_sync_extras_plugin/options.py` & `kolibri_sync_extras_plugin-0.1.3/kolibri_sync_extras_plugin/options.py`

 * *Files identical despite different names*

### Comparing `kolibri_sync_extras_plugin-0.1.2/kolibri_sync_extras_plugin/tasks.py` & `kolibri_sync_extras_plugin-0.1.3/kolibri_sync_extras_plugin/tasks.py`

 * *Files identical despite different names*

### Comparing `kolibri_sync_extras_plugin-0.1.2/setup.py` & `kolibri_sync_extras_plugin-0.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `kolibri_sync_extras_plugin-0.1.2/LICENSE` & `kolibri_sync_extras_plugin-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `kolibri_sync_extras_plugin-0.1.2/test/test_tasks.py` & `kolibri_sync_extras_plugin-0.1.3/test/test_tasks.py`

 * *Files identical despite different names*

### Comparing `kolibri_sync_extras_plugin-0.1.2/PKG-INFO` & `kolibri_sync_extras_plugin-0.1.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,15 @@
 Metadata-Version: 2.1
 Name: kolibri_sync_extras_plugin
-Version: 0.1.2
+Version: 0.1.3
 Summary: Kolibri plugin that provides extra features for peer-to-peer syncing
 Home-page: https://github.com/learningequality/kolibri-sync-extras-plugin
 Author: Learning Equality
 Author-email: info@learningequality.org
 License: MIT
-Description: 
-        `Kolibri <https://learningequality.org/kolibri/>`_ is the offline learning platform
-        from `Learning Equality <https://learningequality.org/>`_.
-        
-        Kolibri supports syncing facility data between two instances. This plugin provides additional sync
-        related features that can be turned on to customize the behavior of those syncs.
-        
 Keywords: kolibri,syncing,morango
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
@@ -26,7 +19,18 @@
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Provides-Extra: dev
+License-File: LICENSE
+License-File: AUTHORS.rst
+
+
+`Kolibri <https://learningequality.org/kolibri/>`_ is the offline learning platform
+from `Learning Equality <https://learningequality.org/>`_.
+
+Kolibri supports syncing facility data between two instances. This plugin provides additional sync
+related features that can be turned on to customize the behavior of those syncs.
+
+
```

### Comparing `kolibri_sync_extras_plugin-0.1.2/CONTRIBUTING.rst` & `kolibri_sync_extras_plugin-0.1.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `kolibri_sync_extras_plugin-0.1.2/README.md` & `kolibri_sync_extras_plugin-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `kolibri_sync_extras_plugin-0.1.2/kolibri_sync_extras_plugin.egg-info/PKG-INFO` & `kolibri_sync_extras_plugin-0.1.3/kolibri_sync_extras_plugin.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,15 @@
 Metadata-Version: 2.1
 Name: kolibri-sync-extras-plugin
-Version: 0.1.2
+Version: 0.1.3
 Summary: Kolibri plugin that provides extra features for peer-to-peer syncing
 Home-page: https://github.com/learningequality/kolibri-sync-extras-plugin
 Author: Learning Equality
 Author-email: info@learningequality.org
 License: MIT
-Description: 
-        `Kolibri <https://learningequality.org/kolibri/>`_ is the offline learning platform
-        from `Learning Equality <https://learningequality.org/>`_.
-        
-        Kolibri supports syncing facility data between two instances. This plugin provides additional sync
-        related features that can be turned on to customize the behavior of those syncs.
-        
 Keywords: kolibri,syncing,morango
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
@@ -26,7 +19,18 @@
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Provides-Extra: dev
+License-File: LICENSE
+License-File: AUTHORS.rst
+
+
+`Kolibri <https://learningequality.org/kolibri/>`_ is the offline learning platform
+from `Learning Equality <https://learningequality.org/>`_.
+
+Kolibri supports syncing facility data between two instances. This plugin provides additional sync
+related features that can be turned on to customize the behavior of those syncs.
+
+
```

### Comparing `kolibri_sync_extras_plugin-0.1.2/kolibri_sync_extras_plugin.egg-info/SOURCES.txt` & `kolibri_sync_extras_plugin-0.1.3/kolibri_sync_extras_plugin.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -18,8 +18,9 @@
 kolibri_sync_extras_plugin.egg-info/top_level.txt
 kolibri_sync_extras_plugin/management/__init__.py
 kolibri_sync_extras_plugin/management/commands/__init__.py
 kolibri_sync_extras_plugin/management/commands/sync_proceed_to.py
 kolibri_sync_extras_plugin/sync/__init__.py
 kolibri_sync_extras_plugin/sync/context.py
 kolibri_sync_extras_plugin/sync/operations.py
+test/test_plugin.py
 test/test_tasks.py
```

