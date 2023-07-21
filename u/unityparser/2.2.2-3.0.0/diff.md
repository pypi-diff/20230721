# Comparing `tmp/unityparser-2.2.2.tar.gz` & `tmp/unityparser-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unityparser-2.2.2.tar", last modified: Tue Mar 21 14:02:17 2023, max compression
+gzip compressed data, was "unityparser-3.0.0.tar", last modified: Fri Jul 21 08:42:41 2023, max compression
```

## Comparing `unityparser-2.2.2.tar` & `unityparser-3.0.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 14:02:17.031252 unityparser-2.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-03-21 14:02:00.000000 unityparser-2.2.2/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-03-21 14:02:00.000000 unityparser-2.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-03-21 14:02:00.000000 unityparser-2.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4707 2023-03-21 14:02:17.031252 unityparser-2.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-03-21 14:02:00.000000 unityparser-2.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 14:02:17.027252 unityparser-2.2.2/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-21 14:02:00.000000 unityparser-2.2.2/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-03-21 14:02:00.000000 unityparser-2.2.2/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-21 14:02:00.000000 unityparser-2.2.2/requirements/ci.in
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-03-21 14:02:00.000000 unityparser-2.2.2/requirements/ci.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-03-21 14:02:00.000000 unityparser-2.2.2/requirements/development.in
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-03-21 14:02:00.000000 unityparser-2.2.2/requirements/development.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-03-21 14:02:00.000000 unityparser-2.2.2/requirements/publish.in
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-03-21 14:02:00.000000 unityparser-2.2.2/requirements/publish.txt
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-03-21 14:02:17.031252 unityparser-2.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-03-21 14:02:00.000000 unityparser-2.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 14:02:17.031252 unityparser-2.2.2/unityparser/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-03-21 14:02:14.000000 unityparser-2.2.2/unityparser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6585 2023-03-21 14:02:00.000000 unityparser-2.2.2/unityparser/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-03-21 14:02:00.000000 unityparser-2.2.2/unityparser/composer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-03-21 14:02:00.000000 unityparser-2.2.2/unityparser/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-03-21 14:02:00.000000 unityparser-2.2.2/unityparser/constructor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-03-21 14:02:00.000000 unityparser-2.2.2/unityparser/dumper.py
--rw-r--r--   0 runner    (1001) docker     (123)     8573 2023-03-21 14:02:00.000000 unityparser-2.2.2/unityparser/emitter.py
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-03-21 14:02:00.000000 unityparser-2.2.2/unityparser/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-03-21 14:02:00.000000 unityparser-2.2.2/unityparser/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-03-21 14:02:00.000000 unityparser-2.2.2/unityparser/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-03-21 14:02:00.000000 unityparser-2.2.2/unityparser/register.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-03-21 14:02:00.000000 unityparser-2.2.2/unityparser/representer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-03-21 14:02:00.000000 unityparser-2.2.2/unityparser/resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-03-21 14:02:00.000000 unityparser-2.2.2/unityparser/scanner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-03-21 14:02:00.000000 unityparser-2.2.2/unityparser/serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5039 2023-03-21 14:02:00.000000 unityparser-2.2.2/unityparser/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 14:02:17.031252 unityparser-2.2.2/unityparser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4707 2023-03-21 14:02:16.000000 unityparser-2.2.2/unityparser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-03-21 14:02:16.000000 unityparser-2.2.2/unityparser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-21 14:02:16.000000 unityparser-2.2.2/unityparser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-03-21 14:02:16.000000 unityparser-2.2.2/unityparser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-21 14:02:16.000000 unityparser-2.2.2/unityparser.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:42:41.078597 unityparser-3.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-21 08:42:21.000000 unityparser-3.0.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-21 08:42:21.000000 unityparser-3.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-21 08:42:21.000000 unityparser-3.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4707 2023-07-21 08:42:41.078597 unityparser-3.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-07-21 08:42:21.000000 unityparser-3.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:42:41.070597 unityparser-3.0.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-21 08:42:21.000000 unityparser-3.0.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-21 08:42:21.000000 unityparser-3.0.0/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-21 08:42:21.000000 unityparser-3.0.0/requirements/ci.in
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-21 08:42:21.000000 unityparser-3.0.0/requirements/ci.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-21 08:42:21.000000 unityparser-3.0.0/requirements/development.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-07-21 08:42:21.000000 unityparser-3.0.0/requirements/development.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-21 08:42:21.000000 unityparser-3.0.0/requirements/publish.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-07-21 08:42:21.000000 unityparser-3.0.0/requirements/publish.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-21 08:42:41.078597 unityparser-3.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-07-21 08:42:21.000000 unityparser-3.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:42:41.074597 unityparser-3.0.0/unityparser/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-21 08:42:38.000000 unityparser-3.0.0/unityparser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6585 2023-07-21 08:42:21.000000 unityparser-3.0.0/unityparser/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-21 08:42:21.000000 unityparser-3.0.0/unityparser/composer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-07-21 08:42:21.000000 unityparser-3.0.0/unityparser/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-07-21 08:42:21.000000 unityparser-3.0.0/unityparser/constructor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-07-21 08:42:21.000000 unityparser-3.0.0/unityparser/dumper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8573 2023-07-21 08:42:21.000000 unityparser-3.0.0/unityparser/emitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-21 08:42:21.000000 unityparser-3.0.0/unityparser/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-07-21 08:42:21.000000 unityparser-3.0.0/unityparser/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-07-21 08:42:21.000000 unityparser-3.0.0/unityparser/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-07-21 08:42:21.000000 unityparser-3.0.0/unityparser/register.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-21 08:42:21.000000 unityparser-3.0.0/unityparser/representer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-07-21 08:42:21.000000 unityparser-3.0.0/unityparser/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-07-21 08:42:21.000000 unityparser-3.0.0/unityparser/scanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-07-21 08:42:21.000000 unityparser-3.0.0/unityparser/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5039 2023-07-21 08:42:21.000000 unityparser-3.0.0/unityparser/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:42:41.078597 unityparser-3.0.0/unityparser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4707 2023-07-21 08:42:41.000000 unityparser-3.0.0/unityparser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-21 08:42:41.000000 unityparser-3.0.0/unityparser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 08:42:41.000000 unityparser-3.0.0/unityparser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-21 08:42:41.000000 unityparser-3.0.0/unityparser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-21 08:42:41.000000 unityparser-3.0.0/unityparser.egg-info/top_level.txt
```

### Comparing `unityparser-2.2.2/LICENSE` & `unityparser-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `unityparser-2.2.2/PKG-INFO` & `unityparser-3.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: unityparser
-Version: 2.2.2
+Version: 3.0.0
 Summary: A python library to parse and dump Unity YAML files
 Home-page: https://github.com/socialpoint-labs/unity-yaml-parser
 Author: Ricard Valverde
 Author-email: ricard.valverde@socialpoint.es
 License: MIT License
 Keywords: unity,yaml,parser,serializer
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6.0
+Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 Provides-Extra: development
 License-File: LICENSE
 License-File: AUTHORS
 
 # Unity YAML Parser #
```

### Comparing `unityparser-2.2.2/README.md` & `unityparser-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `unityparser-2.2.2/requirements/ci.txt` & `unityparser-3.0.0/requirements/ci.txt`

 * *Files identical despite different names*

### Comparing `unityparser-2.2.2/requirements/development.txt` & `unityparser-3.0.0/requirements/development.txt`

 * *Files identical despite different names*

### Comparing `unityparser-2.2.2/requirements/publish.txt` & `unityparser-3.0.0/requirements/publish.txt`

 * *Files identical despite different names*

### Comparing `unityparser-2.2.2/setup.py` & `unityparser-3.0.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     description='A python library to parse and dump Unity YAML files',
     long_description=readme,
     long_description_content_type='text/markdown',
     author='Ricard Valverde',
     author_email='ricard.valverde@socialpoint.es',
     url='https://github.com/socialpoint-labs/unity-yaml-parser',
     license='MIT License',
-    python_requires='>=3.6.0',
+    python_requires='>=3.7.0',
     packages=['unityparser'],
     keywords=['unity', 'yaml', 'parser', 'serializer'],
     install_requires=requirements.pop('base'),
     extras_require=requirements,
     classifiers=[
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3 :: Only',
```

### Comparing `unityparser-2.2.2/unityparser/commands.py` & `unityparser-3.0.0/unityparser/commands.py`

 * *Files identical despite different names*

### Comparing `unityparser-2.2.2/unityparser/composer.py` & `unityparser-3.0.0/unityparser/composer.py`

 * *Files identical despite different names*

### Comparing `unityparser-2.2.2/unityparser/constants.py` & `unityparser-3.0.0/unityparser/constants.py`

 * *Files identical despite different names*

### Comparing `unityparser-2.2.2/unityparser/constructor.py` & `unityparser-3.0.0/unityparser/constructor.py`

 * *Files identical despite different names*

### Comparing `unityparser-2.2.2/unityparser/dumper.py` & `unityparser-3.0.0/unityparser/dumper.py`

 * *Files identical despite different names*

### Comparing `unityparser-2.2.2/unityparser/emitter.py` & `unityparser-3.0.0/unityparser/emitter.py`

 * *Files identical despite different names*

### Comparing `unityparser-2.2.2/unityparser/loader.py` & `unityparser-3.0.0/unityparser/loader.py`

 * *Files identical despite different names*

### Comparing `unityparser-2.2.2/unityparser/parser.py` & `unityparser-3.0.0/unityparser/parser.py`

 * *Files identical despite different names*

### Comparing `unityparser-2.2.2/unityparser/resolver.py` & `unityparser-3.0.0/unityparser/resolver.py`

 * *Files identical despite different names*

### Comparing `unityparser-2.2.2/unityparser/scanner.py` & `unityparser-3.0.0/unityparser/scanner.py`

 * *Files identical despite different names*

### Comparing `unityparser-2.2.2/unityparser/serializer.py` & `unityparser-3.0.0/unityparser/serializer.py`

 * *Files identical despite different names*

### Comparing `unityparser-2.2.2/unityparser/utils.py` & `unityparser-3.0.0/unityparser/utils.py`

 * *Files identical despite different names*

### Comparing `unityparser-2.2.2/unityparser.egg-info/PKG-INFO` & `unityparser-3.0.0/unityparser.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: unityparser
-Version: 2.2.2
+Version: 3.0.0
 Summary: A python library to parse and dump Unity YAML files
 Home-page: https://github.com/socialpoint-labs/unity-yaml-parser
 Author: Ricard Valverde
 Author-email: ricard.valverde@socialpoint.es
 License: MIT License
 Keywords: unity,yaml,parser,serializer
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6.0
+Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 Provides-Extra: development
 License-File: LICENSE
 License-File: AUTHORS
 
 # Unity YAML Parser #
```

### Comparing `unityparser-2.2.2/unityparser.egg-info/SOURCES.txt` & `unityparser-3.0.0/unityparser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

