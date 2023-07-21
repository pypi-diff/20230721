# Comparing `tmp/pyntweb-0.2.tar.gz` & `tmp/pyntweb-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyntweb-0.2.tar", last modified: Fri Jul 21 15:09:58 2023, max compression
+gzip compressed data, was "pyntweb-0.2.1.tar", last modified: Fri Jul 21 15:18:27 2023, max compression
```

## Comparing `pyntweb-0.2.tar` & `pyntweb-0.2.1.tar`

### file list

```diff
@@ -1,33 +1,32 @@
-drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2023-07-21 15:09:58.159360 pyntweb-0.2/
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      653 2023-07-21 15:09:58.159360 pyntweb-0.2/PKG-INFO
-drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2023-07-21 15:09:58.156026 pyntweb-0.2/ntcss/
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      208 2023-07-21 14:57:02.000000 pyntweb-0.2/ntcss/__init__.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)       24 2023-07-21 14:57:02.000000 pyntweb-0.2/ntcss/const.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)     5462 2023-07-21 14:57:02.000000 pyntweb-0.2/ntcss/ntml_parser.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      467 2023-07-21 14:57:02.000000 pyntweb-0.2/ntcss/ntmlc.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      811 2023-07-21 14:57:02.000000 pyntweb-0.2/ntcss/setup.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)    13667 2023-07-21 14:57:02.000000 pyntweb-0.2/ntcss/tran.py
-drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2023-07-21 15:09:58.156026 pyntweb-0.2/ntml/
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      208 2023-07-21 14:57:02.000000 pyntweb-0.2/ntml/__init__.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)       24 2023-07-21 14:57:02.000000 pyntweb-0.2/ntml/const.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)     5462 2023-07-21 14:57:02.000000 pyntweb-0.2/ntml/ntml_parser.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      467 2023-07-21 14:57:02.000000 pyntweb-0.2/ntml/ntmlc.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      811 2023-07-21 14:57:02.000000 pyntweb-0.2/ntml/setup.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)    13667 2023-07-21 14:57:02.000000 pyntweb-0.2/ntml/tran.py
-drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2023-07-21 15:09:58.156026 pyntweb-0.2/pyntweb.egg-info/
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      653 2023-07-21 15:09:58.000000 pyntweb-0.2/pyntweb.egg-info/PKG-INFO
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      514 2023-07-21 15:09:58.000000 pyntweb-0.2/pyntweb.egg-info/SOURCES.txt
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)        1 2023-07-21 15:09:58.000000 pyntweb-0.2/pyntweb.egg-info/dependency_links.txt
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)        1 2023-07-21 15:09:58.000000 pyntweb-0.2/pyntweb.egg-info/not-zip-safe
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)       18 2023-07-21 15:09:58.000000 pyntweb-0.2/pyntweb.egg-info/requires.txt
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)       20 2023-07-21 15:09:58.000000 pyntweb-0.2/pyntweb.egg-info/top_level.txt
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      781 2023-07-21 14:57:02.000000 pyntweb-0.2/pyproject.toml
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)       38 2023-07-21 15:09:58.159360 pyntweb-0.2/setup.cfg
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      867 2023-07-21 14:57:02.000000 pyntweb-0.2/setup.py
-drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2023-07-21 15:09:58.159360 pyntweb-0.2/webfalco/
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      228 2023-07-21 14:57:02.000000 pyntweb-0.2/webfalco/__init__.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)       24 2023-07-21 14:57:02.000000 pyntweb-0.2/webfalco/const.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)     5524 2023-07-21 14:57:02.000000 pyntweb-0.2/webfalco/lrparser.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      811 2023-07-21 14:57:02.000000 pyntweb-0.2/webfalco/setup.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)    13667 2023-07-21 14:57:02.000000 pyntweb-0.2/webfalco/tran.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      467 2023-07-21 14:57:02.000000 pyntweb-0.2/webfalco/webfalcoc.py
+drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2023-07-21 15:18:27.073865 pyntweb-0.2.1/
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)    35149 2023-07-21 15:15:13.000000 pyntweb-0.2.1/LICENSE
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      677 2023-07-21 15:18:27.073865 pyntweb-0.2.1/PKG-INFO
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      550 2023-07-21 15:15:13.000000 pyntweb-0.2.1/README.md
+drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2023-07-21 15:18:27.027195 pyntweb-0.2.1/ntcss/
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      208 2023-07-21 15:15:13.000000 pyntweb-0.2.1/ntcss/__init__.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)       24 2023-07-21 15:15:13.000000 pyntweb-0.2.1/ntcss/const.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)     5462 2023-07-21 15:15:13.000000 pyntweb-0.2.1/ntcss/ntml_parser.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      467 2023-07-21 15:15:13.000000 pyntweb-0.2.1/ntcss/ntmlc.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)    13667 2023-07-21 15:15:13.000000 pyntweb-0.2.1/ntcss/tran.py
+drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2023-07-21 15:18:27.027195 pyntweb-0.2.1/ntml/
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      208 2023-07-21 15:15:13.000000 pyntweb-0.2.1/ntml/__init__.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)       24 2023-07-21 15:15:13.000000 pyntweb-0.2.1/ntml/const.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)     5462 2023-07-21 15:15:13.000000 pyntweb-0.2.1/ntml/ntml_parser.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      467 2023-07-21 15:15:13.000000 pyntweb-0.2.1/ntml/ntmlc.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)    13667 2023-07-21 15:15:13.000000 pyntweb-0.2.1/ntml/tran.py
+drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2023-07-21 15:18:27.070531 pyntweb-0.2.1/pyntweb.egg-info/
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      677 2023-07-21 15:18:26.000000 pyntweb-0.2.1/pyntweb.egg-info/PKG-INFO
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      485 2023-07-21 15:18:26.000000 pyntweb-0.2.1/pyntweb.egg-info/SOURCES.txt
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)        1 2023-07-21 15:18:26.000000 pyntweb-0.2.1/pyntweb.egg-info/dependency_links.txt
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)        1 2023-07-21 15:18:26.000000 pyntweb-0.2.1/pyntweb.egg-info/not-zip-safe
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)       18 2023-07-21 15:18:26.000000 pyntweb-0.2.1/pyntweb.egg-info/requires.txt
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)       20 2023-07-21 15:18:26.000000 pyntweb-0.2.1/pyntweb.egg-info/top_level.txt
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      784 2023-07-21 15:18:05.000000 pyntweb-0.2.1/pyproject.toml
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)       38 2023-07-21 15:18:27.073865 pyntweb-0.2.1/setup.cfg
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      869 2023-07-21 15:17:18.000000 pyntweb-0.2.1/setup.py
+drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2023-07-21 15:18:27.073865 pyntweb-0.2.1/webfalco/
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      228 2023-07-21 15:15:13.000000 pyntweb-0.2.1/webfalco/__init__.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)       24 2023-07-21 15:15:13.000000 pyntweb-0.2.1/webfalco/const.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)     5524 2023-07-21 15:15:13.000000 pyntweb-0.2.1/webfalco/lrparser.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)    13667 2023-07-21 15:15:13.000000 pyntweb-0.2.1/webfalco/tran.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      467 2023-07-21 15:15:13.000000 pyntweb-0.2.1/webfalco/webfalcoc.py
```

### Comparing `pyntweb-0.2/PKG-INFO` & `pyntweb-0.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,6 +1,7 @@
 Metadata-Version: 2.1
 Name: pyntweb
-Version: 0.2
+Version: 0.2.1
 Summary: NTWeb - это экосистема компиляторов, которая планирует прийти на замену существующим в web стандартам: HTML, CSS, JS. На данный момент код на её языках переводится в традиционные языки web, так же традиционные языки нативно поддерживаются в самом кодеПосесите оффициальную группу проекта: https://t.me/+ft6pYhYcqtk3NDdi
 Author-email: talismanchet@vk.com
 License: GNU GPL 3.0
+License-File: LICENSE
```

### Comparing `pyntweb-0.2/ntcss/ntml_parser.py` & `pyntweb-0.2.1/ntcss/ntml_parser.py`

 * *Files identical despite different names*

### Comparing `pyntweb-0.2/ntcss/setup.py` & `pyntweb-0.2.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 """
 setup.py
 """
 
 from setuptools import setup
 
-setup(name='ntml',
-      version='0.2',
+setup(name='pyntweb',
+      version='0.2.1',
       description='''
-NTWeb - это экосистема компиляторов, которая планирует прийти на замену существующим в web стандартам: HTML, CSS, JS. На данный момент код на её языках переводится в традиционные языки web, так же традиционные языки нативно поддерживаются в самом коде
+NTWeb - это экосистема компиляторов, которая планирует прийти на замену существующим в web стандартам: 
+HTML, CSS, JS. На данный момент код на её языках переводится в традиционные языки web, так же 
+традиционные языки нативно поддерживаются в самом коде
 
-Посесите оффициальную группу проекта: https://t.me/+ft6pYhYcqtk3NDdi''',
-      packages=['ntml'],
+Посесите оффициальную группу проекта: https://t.me/+ft6pYhYcqtk3NDdi'''.replace("\n", ""),
+      packages=['ntml', 'webfalco', 'ntcss'],
       license='GNU GPL 3.0',
-      install_requires=['parglare'],
+      install_requires=['parglare', 'colorama'],
       author_email='talismanchet@vk.com',
       zip_safe=False)
```

### Comparing `pyntweb-0.2/ntcss/tran.py` & `pyntweb-0.2.1/ntcss/tran.py`

 * *Files identical despite different names*

### Comparing `pyntweb-0.2/ntml/ntml_parser.py` & `pyntweb-0.2.1/ntml/ntml_parser.py`

 * *Files identical despite different names*

### Comparing `pyntweb-0.2/ntml/setup.py` & `pyntweb-0.2.1/pyntweb.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-"""
-setup.py
-"""
-
-from setuptools import setup
-
-setup(name='ntml',
-      version='0.2',
-      description='''
-NTWeb - это экосистема компиляторов, которая планирует прийти на замену существующим в web стандартам: HTML, CSS, JS. На данный момент код на её языках переводится в традиционные языки web, так же традиционные языки нативно поддерживаются в самом коде
-
-Посесите оффициальную группу проекта: https://t.me/+ft6pYhYcqtk3NDdi''',
-      packages=['ntml'],
-      license='GNU GPL 3.0',
-      install_requires=['parglare'],
-      author_email='talismanchet@vk.com',
-      zip_safe=False)
+Metadata-Version: 2.1
+Name: pyntweb
+Version: 0.2.1
+Summary: NTWeb - это экосистема компиляторов, которая планирует прийти на замену существующим в web стандартам: HTML, CSS, JS. На данный момент код на её языках переводится в традиционные языки web, так же традиционные языки нативно поддерживаются в самом кодеПосесите оффициальную группу проекта: https://t.me/+ft6pYhYcqtk3NDdi
+Author-email: talismanchet@vk.com
+License: GNU GPL 3.0
+License-File: LICENSE
```

### Comparing `pyntweb-0.2/ntml/tran.py` & `pyntweb-0.2.1/ntml/tran.py`

 * *Files identical despite different names*

### Comparing `pyntweb-0.2/pyntweb.egg-info/PKG-INFO` & `pyntweb-0.2.1/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,6 +1,19 @@
-Metadata-Version: 2.1
-Name: pyntweb
-Version: 0.2
-Summary: NTWeb - это экосистема компиляторов, которая планирует прийти на замену существующим в web стандартам: HTML, CSS, JS. На данный момент код на её языках переводится в традиционные языки web, так же традиционные языки нативно поддерживаются в самом кодеПосесите оффициальную группу проекта: https://t.me/+ft6pYhYcqtk3NDdi
-Author-email: talismanchet@vk.com
-License: GNU GPL 3.0
+[tool.poetry]
+name = "pyntweb"
+version = "0.2.1"
+description = "NTWeb - это экосистема компиляторов, которая планирует прийти на замену существующим в web стандартам: HTML, CSS, JS. На данный момент код на её языках переводится в традиционные языки web, так же традиционные языки нативно поддерживаются в самом коде."
+authors = ["Talisman Chet <talismanchet@vk.com>"]
+license = "GNU GPL 3.0"
+readme = "README.md"
+
+[tool.poetry.dependencies]
+python = "^3.10"
+parglare = "^0.16.1"
+colorama = "^0.4.4"
+
+
+[build-system]
+requires = [
+  "setuptools >= 40.9.0",
+]
+build-backend = "setuptools.build_meta"
```

### Comparing `pyntweb-0.2/webfalco/lrparser.py` & `pyntweb-0.2.1/webfalco/lrparser.py`

 * *Files identical despite different names*

### Comparing `pyntweb-0.2/webfalco/tran.py` & `pyntweb-0.2.1/webfalco/tran.py`

 * *Files identical despite different names*

