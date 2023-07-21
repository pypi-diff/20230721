# Comparing `tmp/frida-gadget-1.1.2.tar.gz` & `tmp/frida-gadget-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frida-gadget-1.1.2.tar", last modified: Fri Jul 21 17:09:38 2023, max compression
+gzip compressed data, was "frida-gadget-1.1.3.tar", last modified: Fri Jul 21 17:16:03 2023, max compression
```

## Comparing `frida-gadget-1.1.2.tar` & `frida-gadget-1.1.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-21 17:09:38.412231 frida-gadget-1.1.2/
--rw-rw-rw-   0        0        0     7738 2023-07-21 17:09:38.412231 frida-gadget-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     7067 2023-07-21 16:46:23.000000 frida-gadget-1.1.2/README.rst
-drwxrwxrwx   0        0        0        0 2023-07-21 17:09:38.402804 frida-gadget-1.1.2/frida_gadget.egg-info/
--rw-rw-rw-   0        0        0     7738 2023-07-21 17:09:38.000000 frida-gadget-1.1.2/frida_gadget.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      374 2023-07-21 17:09:38.000000 frida-gadget-1.1.2/frida_gadget.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 17:09:38.000000 frida-gadget-1.1.2/frida_gadget.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-07-21 17:09:38.000000 frida-gadget-1.1.2/frida_gadget.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       62 2023-07-21 17:09:38.000000 frida-gadget-1.1.2/frida_gadget.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-21 17:09:38.000000 frida-gadget-1.1.2/frida_gadget.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-21 17:09:38.406797 frida-gadget-1.1.2/scripts/
--rw-rw-rw-   0        0        0      699 2023-07-21 16:46:23.000000 frida-gadget-1.1.2/scripts/__init__.py
--rw-rw-rw-   0        0        0     8974 2023-07-21 17:09:05.000000 frida-gadget-1.1.2/scripts/cli.py
-drwxrwxrwx   0        0        0        0 2023-07-21 17:09:38.407797 frida-gadget-1.1.2/scripts/files/
--rw-rw-rw-   0        0        0       84 2023-07-21 16:46:23.000000 frida-gadget-1.1.2/scripts/files/README.md
--rw-rw-rw-   0        0        0     3531 2023-07-21 16:46:23.000000 frida-gadget-1.1.2/scripts/frida_github.py
--rw-rw-rw-   0        0        0      648 2023-07-21 16:46:23.000000 frida-gadget-1.1.2/scripts/logger.py
--rw-rw-rw-   0        0        0       42 2023-07-21 17:09:38.412231 frida-gadget-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1471 2023-07-21 17:08:00.000000 frida-gadget-1.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-21 17:09:38.408797 frida-gadget-1.1.2/tests/
--rw-rw-rw-   0        0        0        0 2023-07-21 16:46:23.000000 frida-gadget-1.1.2/tests/__init__.py
--rw-rw-rw-   0        0        0      418 2023-07-21 16:46:23.000000 frida-gadget-1.1.2/tests/test_cli.py
+drwxrwxrwx   0        0        0        0 2023-07-21 17:16:03.348886 frida-gadget-1.1.3/
+-rw-rw-rw-   0        0        0     7738 2023-07-21 17:16:03.347887 frida-gadget-1.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     7067 2023-07-21 16:46:23.000000 frida-gadget-1.1.3/README.rst
+drwxrwxrwx   0        0        0        0 2023-07-21 17:16:03.339887 frida-gadget-1.1.3/frida_gadget.egg-info/
+-rw-rw-rw-   0        0        0     7738 2023-07-21 17:16:03.000000 frida-gadget-1.1.3/frida_gadget.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      374 2023-07-21 17:16:03.000000 frida-gadget-1.1.3/frida_gadget.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 17:16:03.000000 frida-gadget-1.1.3/frida_gadget.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-07-21 17:16:03.000000 frida-gadget-1.1.3/frida_gadget.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       62 2023-07-21 17:16:03.000000 frida-gadget-1.1.3/frida_gadget.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-21 17:16:03.000000 frida-gadget-1.1.3/frida_gadget.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-21 17:16:03.343886 frida-gadget-1.1.3/scripts/
+-rw-rw-rw-   0        0        0      699 2023-07-21 16:46:23.000000 frida-gadget-1.1.3/scripts/__init__.py
+-rw-rw-rw-   0        0        0     8974 2023-07-21 17:09:05.000000 frida-gadget-1.1.3/scripts/cli.py
+drwxrwxrwx   0        0        0        0 2023-07-21 17:16:03.344887 frida-gadget-1.1.3/scripts/files/
+-rw-rw-rw-   0        0        0       84 2023-07-21 16:46:23.000000 frida-gadget-1.1.3/scripts/files/README.md
+-rw-rw-rw-   0        0        0     3531 2023-07-21 16:46:23.000000 frida-gadget-1.1.3/scripts/frida_github.py
+-rw-rw-rw-   0        0        0      648 2023-07-21 16:46:23.000000 frida-gadget-1.1.3/scripts/logger.py
+-rw-rw-rw-   0        0        0       42 2023-07-21 17:16:03.348886 frida-gadget-1.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1471 2023-07-21 17:15:58.000000 frida-gadget-1.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 17:16:03.346887 frida-gadget-1.1.3/tests/
+-rw-rw-rw-   0        0        0        0 2023-07-21 16:46:23.000000 frida-gadget-1.1.3/tests/__init__.py
+-rw-rw-rw-   0        0        0      418 2023-07-21 16:46:23.000000 frida-gadget-1.1.3/tests/test_cli.py
```

### Comparing `frida-gadget-1.1.2/PKG-INFO` & `frida-gadget-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frida-gadget
-Version: 1.1.2
+Version: 1.1.3
 Summary: Frida gadget into an APK
 Home-page: https://github.com/ksg97031/frida-gadget
 Author: ksg97031
 Author-email: ksg97031@gmail.com
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `frida-gadget-1.1.2/README.rst` & `frida-gadget-1.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `frida-gadget-1.1.2/frida_gadget.egg-info/PKG-INFO` & `frida-gadget-1.1.3/frida_gadget.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frida-gadget
-Version: 1.1.2
+Version: 1.1.3
 Summary: Frida gadget into an APK
 Home-page: https://github.com/ksg97031/frida-gadget
 Author: ksg97031
 Author-email: ksg97031@gmail.com
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `frida-gadget-1.1.2/scripts/__init__.py` & `frida-gadget-1.1.3/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `frida-gadget-1.1.2/scripts/cli.py` & `frida-gadget-1.1.3/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `frida-gadget-1.1.2/scripts/frida_github.py` & `frida-gadget-1.1.3/scripts/frida_github.py`

 * *Files identical despite different names*

### Comparing `frida-gadget-1.1.2/scripts/logger.py` & `frida-gadget-1.1.3/scripts/logger.py`

 * *Files identical despite different names*

### Comparing `frida-gadget-1.1.2/setup.py` & `frida-gadget-1.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     'coverage',
     'requests',
 ]
 
 setuptools.setup(
     name="frida-gadget",
     python_requires='>=3.6',
-    version="1.1.2",
+    version="1.1.3",
     author="ksg97031",
     author_email="ksg97031@gmail.com",
     description="Frida gadget into an APK",
     install_requires=requires,
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/ksg97031/frida-gadget",
```

