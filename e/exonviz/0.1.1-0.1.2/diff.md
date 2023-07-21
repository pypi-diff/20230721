# Comparing `tmp/exonviz-0.1.1.tar.gz` & `tmp/exonviz-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exonviz-0.1.1.tar", last modified: Fri Jul 21 06:51:47 2023, max compression
+gzip compressed data, was "exonviz-0.1.2.tar", last modified: Fri Jul 21 08:05:34 2023, max compression
```

## Comparing `exonviz-0.1.1.tar` & `exonviz-0.1.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 trijntje  (1000) trijntje  (1000)        0 2023-07-21 06:51:47.665556 exonviz-0.1.1/
--rw-rw-r--   0 trijntje  (1000) trijntje  (1000)    34523 2023-07-11 13:50:44.000000 exonviz-0.1.1/LICENSE
--rw-rw-r--   0 trijntje  (1000) trijntje  (1000)     3992 2023-07-21 06:51:47.665556 exonviz-0.1.1/PKG-INFO
--rw-rw-r--   0 trijntje  (1000) trijntje  (1000)     2986 2023-07-11 14:22:54.000000 exonviz-0.1.1/README.md
--rw-rw-r--   0 trijntje  (1000) trijntje  (1000)       38 2023-07-21 06:51:47.665556 exonviz-0.1.1/setup.cfg
--rw-rw-r--   0 trijntje  (1000) trijntje  (1000)     2812 2023-07-21 06:36:22.000000 exonviz-0.1.1/setup.py
-drwxrwxr-x   0 trijntje  (1000) trijntje  (1000)        0 2023-07-21 06:51:47.661555 exonviz-0.1.1/src/
--rw-rw-r--   0 trijntje  (1000) trijntje  (1000)        0 2023-07-11 13:50:44.000000 exonviz-0.1.1/src/conftest.py
-drwxrwxr-x   0 trijntje  (1000) trijntje  (1000)        0 2023-07-21 06:51:47.661555 exonviz-0.1.1/src/exonviz/
--rw-rw-r--   0 trijntje  (1000) trijntje  (1000)       89 2023-07-21 06:23:07.000000 exonviz-0.1.1/src/exonviz/__init__.py
--rw-rw-r--   0 trijntje  (1000) trijntje  (1000)       61 2023-07-11 13:50:44.000000 exonviz-0.1.1/src/exonviz/__main__.py
--rw-rw-r--   0 trijntje  (1000) trijntje  (1000)     2331 2023-07-21 06:35:48.000000 exonviz-0.1.1/src/exonviz/cli.py
--rw-rw-r--   0 trijntje  (1000) trijntje  (1000)     5970 2023-07-11 13:50:44.000000 exonviz-0.1.1/src/exonviz/draw.py
--rw-rw-r--   0 trijntje  (1000) trijntje  (1000)     3039 2023-07-11 13:50:44.000000 exonviz-0.1.1/src/exonviz/exon.py
--rw-rw-r--   0 trijntje  (1000) trijntje  (1000)     2056 2023-07-21 06:32:19.000000 exonviz-0.1.1/src/exonviz/mutalyzer.py
--rw-rw-r--   0 trijntje  (1000) trijntje  (1000)        0 2023-07-21 06:02:29.000000 exonviz-0.1.1/src/exonviz/py.typed
-drwxrwxr-x   0 trijntje  (1000) trijntje  (1000)        0 2023-07-21 06:51:47.661555 exonviz-0.1.1/src/exonviz.egg-info/
--rw-rw-r--   0 trijntje  (1000) trijntje  (1000)     3992 2023-07-21 06:51:47.000000 exonviz-0.1.1/src/exonviz.egg-info/PKG-INFO
--rw-rw-r--   0 trijntje  (1000) trijntje  (1000)      526 2023-07-21 06:51:47.000000 exonviz-0.1.1/src/exonviz.egg-info/SOURCES.txt
--rw-rw-r--   0 trijntje  (1000) trijntje  (1000)        1 2023-07-21 06:51:47.000000 exonviz-0.1.1/src/exonviz.egg-info/dependency_links.txt
--rw-rw-r--   0 trijntje  (1000) trijntje  (1000)       45 2023-07-21 06:51:47.000000 exonviz-0.1.1/src/exonviz.egg-info/entry_points.txt
--rw-rw-r--   0 trijntje  (1000) trijntje  (1000)        1 2023-07-11 13:51:11.000000 exonviz-0.1.1/src/exonviz.egg-info/not-zip-safe
--rw-rw-r--   0 trijntje  (1000) trijntje  (1000)        7 2023-07-21 06:51:47.000000 exonviz-0.1.1/src/exonviz.egg-info/requires.txt
--rw-rw-r--   0 trijntje  (1000) trijntje  (1000)       17 2023-07-21 06:51:47.000000 exonviz-0.1.1/src/exonviz.egg-info/top_level.txt
-drwxrwxr-x   0 trijntje  (1000) trijntje  (1000)        0 2023-07-21 06:51:47.665556 exonviz-0.1.1/tests/
--rw-rw-r--   0 trijntje  (1000) trijntje  (1000)     7408 2023-07-11 13:50:44.000000 exonviz-0.1.1/tests/test_Exon.py
--rw-rw-r--   0 trijntje  (1000) trijntje  (1000)     1090 2023-07-11 13:50:44.000000 exonviz-0.1.1/tests/test_cli.py
--rw-rw-r--   0 trijntje  (1000) trijntje  (1000)     1958 2023-07-11 13:50:44.000000 exonviz-0.1.1/tests/test_draw_exon.py
--rw-rw-r--   0 trijntje  (1000) trijntje  (1000)     1699 2023-07-11 13:50:44.000000 exonviz-0.1.1/tests/test_mutalyzer.py
+drwxrwxr-x   0 trijntje  (1000) trijntje  (1000)        0 2023-07-21 08:05:34.332402 exonviz-0.1.2/
+-rw-rw-r--   0 trijntje  (1000) trijntje  (1000)    34523 2023-07-11 13:50:44.000000 exonviz-0.1.2/LICENSE
+-rw-rw-r--   0 trijntje  (1000) trijntje  (1000)     3992 2023-07-21 08:05:34.332402 exonviz-0.1.2/PKG-INFO
+-rw-rw-r--   0 trijntje  (1000) trijntje  (1000)     2986 2023-07-11 14:22:54.000000 exonviz-0.1.2/README.md
+-rw-rw-r--   0 trijntje  (1000) trijntje  (1000)       38 2023-07-21 08:05:34.332402 exonviz-0.1.2/setup.cfg
+-rw-rw-r--   0 trijntje  (1000) trijntje  (1000)     2812 2023-07-21 08:03:27.000000 exonviz-0.1.2/setup.py
+drwxrwxr-x   0 trijntje  (1000) trijntje  (1000)        0 2023-07-21 08:05:34.332402 exonviz-0.1.2/src/
+-rw-rw-r--   0 trijntje  (1000) trijntje  (1000)        0 2023-07-11 13:50:44.000000 exonviz-0.1.2/src/conftest.py
+drwxrwxr-x   0 trijntje  (1000) trijntje  (1000)        0 2023-07-21 08:05:34.332402 exonviz-0.1.2/src/exonviz/
+-rw-rw-r--   0 trijntje  (1000) trijntje  (1000)      148 2023-07-21 08:05:03.000000 exonviz-0.1.2/src/exonviz/__init__.py
+-rw-rw-r--   0 trijntje  (1000) trijntje  (1000)       61 2023-07-11 13:50:44.000000 exonviz-0.1.2/src/exonviz/__main__.py
+-rw-rw-r--   0 trijntje  (1000) trijntje  (1000)     2331 2023-07-21 06:35:48.000000 exonviz-0.1.2/src/exonviz/cli.py
+-rw-rw-r--   0 trijntje  (1000) trijntje  (1000)     5970 2023-07-11 13:50:44.000000 exonviz-0.1.2/src/exonviz/draw.py
+-rw-rw-r--   0 trijntje  (1000) trijntje  (1000)     3039 2023-07-11 13:50:44.000000 exonviz-0.1.2/src/exonviz/exon.py
+-rw-rw-r--   0 trijntje  (1000) trijntje  (1000)     2056 2023-07-21 06:32:19.000000 exonviz-0.1.2/src/exonviz/mutalyzer.py
+-rw-rw-r--   0 trijntje  (1000) trijntje  (1000)        0 2023-07-21 06:02:29.000000 exonviz-0.1.2/src/exonviz/py.typed
+drwxrwxr-x   0 trijntje  (1000) trijntje  (1000)        0 2023-07-21 08:05:34.332402 exonviz-0.1.2/src/exonviz.egg-info/
+-rw-rw-r--   0 trijntje  (1000) trijntje  (1000)     3992 2023-07-21 08:05:34.000000 exonviz-0.1.2/src/exonviz.egg-info/PKG-INFO
+-rw-rw-r--   0 trijntje  (1000) trijntje  (1000)      526 2023-07-21 08:05:34.000000 exonviz-0.1.2/src/exonviz.egg-info/SOURCES.txt
+-rw-rw-r--   0 trijntje  (1000) trijntje  (1000)        1 2023-07-21 08:05:34.000000 exonviz-0.1.2/src/exonviz.egg-info/dependency_links.txt
+-rw-rw-r--   0 trijntje  (1000) trijntje  (1000)       45 2023-07-21 08:05:34.000000 exonviz-0.1.2/src/exonviz.egg-info/entry_points.txt
+-rw-rw-r--   0 trijntje  (1000) trijntje  (1000)        1 2023-07-11 13:51:11.000000 exonviz-0.1.2/src/exonviz.egg-info/not-zip-safe
+-rw-rw-r--   0 trijntje  (1000) trijntje  (1000)        7 2023-07-21 08:05:34.000000 exonviz-0.1.2/src/exonviz.egg-info/requires.txt
+-rw-rw-r--   0 trijntje  (1000) trijntje  (1000)       17 2023-07-21 08:05:34.000000 exonviz-0.1.2/src/exonviz.egg-info/top_level.txt
+drwxrwxr-x   0 trijntje  (1000) trijntje  (1000)        0 2023-07-21 08:05:34.332402 exonviz-0.1.2/tests/
+-rw-rw-r--   0 trijntje  (1000) trijntje  (1000)     7408 2023-07-11 13:50:44.000000 exonviz-0.1.2/tests/test_Exon.py
+-rw-rw-r--   0 trijntje  (1000) trijntje  (1000)     1090 2023-07-11 13:50:44.000000 exonviz-0.1.2/tests/test_cli.py
+-rw-rw-r--   0 trijntje  (1000) trijntje  (1000)     1958 2023-07-11 13:50:44.000000 exonviz-0.1.2/tests/test_draw_exon.py
+-rw-rw-r--   0 trijntje  (1000) trijntje  (1000)     1699 2023-07-11 13:50:44.000000 exonviz-0.1.2/tests/test_mutalyzer.py
```

### Comparing `exonviz-0.1.1/LICENSE` & `exonviz-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `exonviz-0.1.1/PKG-INFO` & `exonviz-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exonviz
-Version: 0.1.1
+Version: 0.1.2
 Summary: Visualise exons and their reading frames
 Home-page: https://github.com/redmar-van-den-berg/exonviz
 Author: Redmar van den Berg
 Author-email: RedmarvandenBerg@lumc.nl
 License: AGPL-3.0
 Project-URL: Changelog, https://github.com/redmar-van-den-berg/exonviz/blob/main/CHANGELOG.md
 Project-URL: Issue Tracker, https://github.com/redmar-van-den-berg/exonviz/issues
```

### Comparing `exonviz-0.1.1/README.md` & `exonviz-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `exonviz-0.1.1/setup.py` & `exonviz-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         join(dirname(__file__), *names), encoding=kwargs.get("encoding", "utf8")
     ) as fh:
         return fh.read()
 
 
 setup(
     name="exonviz",
-    version="0.1.1",
+    version="0.1.2",
     license="AGPL-3.0",
     description="Visualise exons and their reading frames",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Redmar van den Berg",
     author_email="RedmarvandenBerg@lumc.nl",
     url="https://github.com/redmar-van-den-berg/exonviz",
```

### Comparing `exonviz-0.1.1/src/exonviz/cli.py` & `exonviz-0.1.2/src/exonviz/cli.py`

 * *Files identical despite different names*

### Comparing `exonviz-0.1.1/src/exonviz/draw.py` & `exonviz-0.1.2/src/exonviz/draw.py`

 * *Files identical despite different names*

### Comparing `exonviz-0.1.1/src/exonviz/exon.py` & `exonviz-0.1.2/src/exonviz/exon.py`

 * *Files identical despite different names*

### Comparing `exonviz-0.1.1/src/exonviz/mutalyzer.py` & `exonviz-0.1.2/src/exonviz/mutalyzer.py`

 * *Files identical despite different names*

### Comparing `exonviz-0.1.1/src/exonviz.egg-info/PKG-INFO` & `exonviz-0.1.2/src/exonviz.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exonviz
-Version: 0.1.1
+Version: 0.1.2
 Summary: Visualise exons and their reading frames
 Home-page: https://github.com/redmar-van-den-berg/exonviz
 Author: Redmar van den Berg
 Author-email: RedmarvandenBerg@lumc.nl
 License: AGPL-3.0
 Project-URL: Changelog, https://github.com/redmar-van-den-berg/exonviz/blob/main/CHANGELOG.md
 Project-URL: Issue Tracker, https://github.com/redmar-van-den-berg/exonviz/issues
```

### Comparing `exonviz-0.1.1/src/exonviz.egg-info/SOURCES.txt` & `exonviz-0.1.2/src/exonviz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `exonviz-0.1.1/tests/test_Exon.py` & `exonviz-0.1.2/tests/test_Exon.py`

 * *Files identical despite different names*

### Comparing `exonviz-0.1.1/tests/test_cli.py` & `exonviz-0.1.2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `exonviz-0.1.1/tests/test_draw_exon.py` & `exonviz-0.1.2/tests/test_draw_exon.py`

 * *Files identical despite different names*

### Comparing `exonviz-0.1.1/tests/test_mutalyzer.py` & `exonviz-0.1.2/tests/test_mutalyzer.py`

 * *Files identical despite different names*

