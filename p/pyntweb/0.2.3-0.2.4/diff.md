# Comparing `tmp/pyntweb-0.2.3.tar.gz` & `tmp/pyntweb-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyntweb-0.2.3.tar", last modified: Fri Jul 21 19:15:17 2023, max compression
+gzip compressed data, was "pyntweb-0.2.4.tar", last modified: Fri Jul 21 19:36:53 2023, max compression
```

## Comparing `pyntweb-0.2.3.tar` & `pyntweb-0.2.4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2023-07-21 19:15:17.573499 pyntweb-0.2.3/
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)    35149 2023-07-21 15:15:13.000000 pyntweb-0.2.3/LICENSE
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      677 2023-07-21 19:15:17.573499 pyntweb-0.2.3/PKG-INFO
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      550 2023-07-21 15:15:13.000000 pyntweb-0.2.3/README.md
-drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2023-07-21 19:15:17.570165 pyntweb-0.2.3/ntcss/
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      208 2023-07-21 15:15:13.000000 pyntweb-0.2.3/ntcss/__init__.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)       24 2023-07-21 15:15:13.000000 pyntweb-0.2.3/ntcss/const.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)     5462 2023-07-21 15:15:13.000000 pyntweb-0.2.3/ntcss/ntml_parser.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      467 2023-07-21 15:15:13.000000 pyntweb-0.2.3/ntcss/ntmlc.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)    13667 2023-07-21 15:15:13.000000 pyntweb-0.2.3/ntcss/tran.py
-drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2023-07-21 19:15:17.570165 pyntweb-0.2.3/ntml/
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      208 2023-07-21 15:15:13.000000 pyntweb-0.2.3/ntml/__init__.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)       24 2023-07-21 15:15:13.000000 pyntweb-0.2.3/ntml/const.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)     2561 2023-07-21 15:15:13.000000 pyntweb-0.2.3/ntml/errors.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)     5462 2023-07-21 15:15:13.000000 pyntweb-0.2.3/ntml/ntml_parser.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      467 2023-07-21 15:15:13.000000 pyntweb-0.2.3/ntml/ntmlc.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)    13703 2023-07-21 16:13:25.000000 pyntweb-0.2.3/ntml/tran.py
-drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2023-07-21 19:15:17.570165 pyntweb-0.2.3/pyntweb.egg-info/
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      677 2023-07-21 19:15:17.000000 pyntweb-0.2.3/pyntweb.egg-info/PKG-INFO
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      500 2023-07-21 19:15:17.000000 pyntweb-0.2.3/pyntweb.egg-info/SOURCES.txt
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)        1 2023-07-21 19:15:17.000000 pyntweb-0.2.3/pyntweb.egg-info/dependency_links.txt
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)        1 2023-07-21 15:18:26.000000 pyntweb-0.2.3/pyntweb.egg-info/not-zip-safe
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)       18 2023-07-21 19:15:17.000000 pyntweb-0.2.3/pyntweb.egg-info/requires.txt
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)       20 2023-07-21 19:15:17.000000 pyntweb-0.2.3/pyntweb.egg-info/top_level.txt
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      784 2023-07-21 19:15:05.000000 pyntweb-0.2.3/pyproject.toml
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)       38 2023-07-21 19:15:17.573499 pyntweb-0.2.3/setup.cfg
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      869 2023-07-21 19:14:59.000000 pyntweb-0.2.3/setup.py
-drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2023-07-21 19:15:17.573499 pyntweb-0.2.3/webfalco/
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      228 2023-07-21 15:15:13.000000 pyntweb-0.2.3/webfalco/__init__.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)       24 2023-07-21 15:15:13.000000 pyntweb-0.2.3/webfalco/const.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)     5524 2023-07-21 15:15:13.000000 pyntweb-0.2.3/webfalco/lrparser.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)    13667 2023-07-21 15:15:13.000000 pyntweb-0.2.3/webfalco/tran.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      467 2023-07-21 15:15:13.000000 pyntweb-0.2.3/webfalco/webfalcoc.py
+drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2023-07-21 19:36:53.832302 pyntweb-0.2.4/
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)    35149 2023-07-21 15:15:13.000000 pyntweb-0.2.4/LICENSE
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      677 2023-07-21 19:36:53.832302 pyntweb-0.2.4/PKG-INFO
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      550 2023-07-21 15:15:13.000000 pyntweb-0.2.4/README.md
+drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2023-07-21 19:36:53.818967 pyntweb-0.2.4/ntcss/
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      208 2023-07-21 15:15:13.000000 pyntweb-0.2.4/ntcss/__init__.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)       24 2023-07-21 15:15:13.000000 pyntweb-0.2.4/ntcss/const.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)     5462 2023-07-21 15:15:13.000000 pyntweb-0.2.4/ntcss/ntml_parser.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      467 2023-07-21 15:15:13.000000 pyntweb-0.2.4/ntcss/ntmlc.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)    13667 2023-07-21 15:15:13.000000 pyntweb-0.2.4/ntcss/tran.py
+drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2023-07-21 19:36:53.818967 pyntweb-0.2.4/ntml/
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      208 2023-07-21 15:15:13.000000 pyntweb-0.2.4/ntml/__init__.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)       24 2023-07-21 15:15:13.000000 pyntweb-0.2.4/ntml/const.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)     2561 2023-07-21 15:15:13.000000 pyntweb-0.2.4/ntml/errors.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)     5553 2023-07-21 19:36:11.000000 pyntweb-0.2.4/ntml/ntml_parser.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      467 2023-07-21 15:15:13.000000 pyntweb-0.2.4/ntml/ntmlc.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)    13703 2023-07-21 16:13:25.000000 pyntweb-0.2.4/ntml/tran.py
+drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2023-07-21 19:36:53.828968 pyntweb-0.2.4/pyntweb.egg-info/
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      677 2023-07-21 19:36:53.000000 pyntweb-0.2.4/pyntweb.egg-info/PKG-INFO
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      500 2023-07-21 19:36:53.000000 pyntweb-0.2.4/pyntweb.egg-info/SOURCES.txt
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)        1 2023-07-21 19:36:53.000000 pyntweb-0.2.4/pyntweb.egg-info/dependency_links.txt
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)        1 2023-07-21 15:18:26.000000 pyntweb-0.2.4/pyntweb.egg-info/not-zip-safe
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)       18 2023-07-21 19:36:53.000000 pyntweb-0.2.4/pyntweb.egg-info/requires.txt
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)       20 2023-07-21 19:36:53.000000 pyntweb-0.2.4/pyntweb.egg-info/top_level.txt
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      784 2023-07-21 19:36:38.000000 pyntweb-0.2.4/pyproject.toml
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)       38 2023-07-21 19:36:53.832302 pyntweb-0.2.4/setup.cfg
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      869 2023-07-21 19:36:43.000000 pyntweb-0.2.4/setup.py
+drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2023-07-21 19:36:53.828968 pyntweb-0.2.4/webfalco/
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      228 2023-07-21 15:15:13.000000 pyntweb-0.2.4/webfalco/__init__.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)       24 2023-07-21 15:15:13.000000 pyntweb-0.2.4/webfalco/const.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)     5524 2023-07-21 15:15:13.000000 pyntweb-0.2.4/webfalco/lrparser.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)    13667 2023-07-21 15:15:13.000000 pyntweb-0.2.4/webfalco/tran.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      467 2023-07-21 15:15:13.000000 pyntweb-0.2.4/webfalco/webfalcoc.py
```

### Comparing `pyntweb-0.2.3/LICENSE` & `pyntweb-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyntweb-0.2.3/PKG-INFO` & `pyntweb-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 Metadata-Version: 2.1
 Name: pyntweb
-Version: 0.2.3
+Version: 0.2.4
 Summary: NTWeb - это экосистема компиляторов, которая планирует прийти на замену существующим в web стандартам: HTML, CSS, JS. На данный момент код на её языках переводится в традиционные языки web, так же традиционные языки нативно поддерживаются в самом кодеПосесите оффициальную группу проекта: https://t.me/+ft6pYhYcqtk3NDdi
 Author-email: talismanchet@vk.com
 License: GNU GPL 3.0
 License-File: LICENSE
```

### Comparing `pyntweb-0.2.3/README.md` & `pyntweb-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `pyntweb-0.2.3/ntcss/ntml_parser.py` & `pyntweb-0.2.4/ntcss/ntml_parser.py`

 * *Files identical despite different names*

### Comparing `pyntweb-0.2.3/ntcss/tran.py` & `pyntweb-0.2.4/ntcss/tran.py`

 * *Files identical despite different names*

### Comparing `pyntweb-0.2.3/ntml/errors.py` & `pyntweb-0.2.4/ntml/errors.py`

 * *Files identical despite different names*

### Comparing `pyntweb-0.2.3/ntml/ntml_parser.py` & `pyntweb-0.2.4/ntml/ntml_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -160,14 +160,20 @@
         return "["
 
     if data == "nl":
         return "<br/>"
     
     elif data == "sp":
         return "&nbsp;"
+
+    elif data == "per":
+        return "&37;"
+
+    elif data == "tag":
+        return "#"
     
     elif data in ("c", "cp", "copy"):
         return "&copy;"
     
     elif data in list("()[]{}\\/"):
         return data
```

### Comparing `pyntweb-0.2.3/ntml/tran.py` & `pyntweb-0.2.4/ntml/tran.py`

 * *Files identical despite different names*

### Comparing `pyntweb-0.2.3/pyntweb.egg-info/PKG-INFO` & `pyntweb-0.2.4/pyntweb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 Metadata-Version: 2.1
 Name: pyntweb
-Version: 0.2.3
+Version: 0.2.4
 Summary: NTWeb - это экосистема компиляторов, которая планирует прийти на замену существующим в web стандартам: HTML, CSS, JS. На данный момент код на её языках переводится в традиционные языки web, так же традиционные языки нативно поддерживаются в самом кодеПосесите оффициальную группу проекта: https://t.me/+ft6pYhYcqtk3NDdi
 Author-email: talismanchet@vk.com
 License: GNU GPL 3.0
 License-File: LICENSE
```

### Comparing `pyntweb-0.2.3/pyproject.toml` & `pyntweb-0.2.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyntweb"
-version = "0.2.3"
+version = "0.2.4"
 description = "NTWeb - это экосистема компиляторов, которая планирует прийти на замену существующим в web стандартам: HTML, CSS, JS. На данный момент код на её языках переводится в традиционные языки web, так же традиционные языки нативно поддерживаются в самом коде."
 authors = ["Talisman Chet <talismanchet@vk.com>"]
 license = "GNU GPL 3.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `pyntweb-0.2.3/setup.py` & `pyntweb-0.2.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 setup.py
 """
 
 from setuptools import setup
 
 setup(name='pyntweb',
-      version='0.2.3',
+      version='0.2.4',
       description='''
 NTWeb - это экосистема компиляторов, которая планирует прийти на замену существующим в web стандартам: 
 HTML, CSS, JS. На данный момент код на её языках переводится в традиционные языки web, так же 
 традиционные языки нативно поддерживаются в самом коде
 
 Посесите оффициальную группу проекта: https://t.me/+ft6pYhYcqtk3NDdi'''.replace("\n", ""),
       packages=['ntml', 'webfalco', 'ntcss'],
```

### Comparing `pyntweb-0.2.3/webfalco/lrparser.py` & `pyntweb-0.2.4/webfalco/lrparser.py`

 * *Files identical despite different names*

### Comparing `pyntweb-0.2.3/webfalco/tran.py` & `pyntweb-0.2.4/webfalco/tran.py`

 * *Files identical despite different names*

