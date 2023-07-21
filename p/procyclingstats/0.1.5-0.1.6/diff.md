# Comparing `tmp/procyclingstats-0.1.5.tar.gz` & `tmp/procyclingstats-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "procyclingstats-0.1.5.tar", last modified: Sun Jun 18 12:21:46 2023, max compression
+gzip compressed data, was "procyclingstats-0.1.6.tar", last modified: Fri Jul 21 19:15:21 2023, max compression
```

## Comparing `procyclingstats-0.1.5.tar` & `procyclingstats-0.1.6.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 madzin    (1000) madzin    (1000)        0 2023-06-18 12:21:46.403038 procyclingstats-0.1.5/
--rw-r--r--   0 madzin    (1000) madzin    (1000)     2991 2023-06-18 12:21:46.404003 procyclingstats-0.1.5/PKG-INFO
--rw-r--r--   0 madzin    (1000) madzin    (1000)     2042 2023-03-01 16:18:11.000000 procyclingstats-0.1.5/README.rst
-drwxr-xr-x   0 madzin    (1000) madzin    (1000)        0 2023-06-18 12:21:46.394209 procyclingstats-0.1.5/procyclingstats/
--rw-r--r--   0 madzin    (1000) madzin    (1000)      599 2023-02-26 10:28:41.000000 procyclingstats-0.1.5/procyclingstats/__init__.py
--rw-r--r--   0 madzin    (1000) madzin    (1000)     4235 2023-06-18 10:18:30.000000 procyclingstats-0.1.5/procyclingstats/__main__.py
--rw-r--r--   0 madzin    (1000) madzin    (1000)     1304 2023-02-26 10:28:41.000000 procyclingstats-0.1.5/procyclingstats/errors.py
--rw-r--r--   0 madzin    (1000) madzin    (1000)     3460 2023-06-18 10:26:43.000000 procyclingstats-0.1.5/procyclingstats/race_climbs_scraper.py
--rw-r--r--   0 madzin    (1000) madzin    (1000)     6604 2023-06-17 19:29:12.000000 procyclingstats-0.1.5/procyclingstats/race_scraper.py
--rw-r--r--   0 madzin    (1000) madzin    (1000)     4567 2023-06-17 17:21:57.000000 procyclingstats-0.1.5/procyclingstats/race_startlist_scraper.py
--rw-r--r--   0 madzin    (1000) madzin    (1000)    19273 2023-06-17 17:23:51.000000 procyclingstats-0.1.5/procyclingstats/ranking_scraper.py
--rw-r--r--   0 madzin    (1000) madzin    (1000)     8398 2023-06-17 17:23:38.000000 procyclingstats-0.1.5/procyclingstats/rider_results_scraper.py
--rw-r--r--   0 madzin    (1000) madzin    (1000)     6870 2023-06-17 17:25:09.000000 procyclingstats-0.1.5/procyclingstats/rider_scraper.py
--rw-r--r--   0 madzin    (1000) madzin    (1000)     6517 2023-06-17 17:22:57.000000 procyclingstats-0.1.5/procyclingstats/scraper.py
--rw-r--r--   0 madzin    (1000) madzin    (1000)    23754 2023-06-18 11:20:14.000000 procyclingstats-0.1.5/procyclingstats/stage_scraper.py
--rw-r--r--   0 madzin    (1000) madzin    (1000)    15221 2023-06-18 11:09:12.000000 procyclingstats-0.1.5/procyclingstats/table_parser.py
--rw-r--r--   0 madzin    (1000) madzin    (1000)     9053 2023-06-17 17:24:59.000000 procyclingstats-0.1.5/procyclingstats/team_scraper.py
--rw-r--r--   0 madzin    (1000) madzin    (1000)     6364 2023-06-17 17:25:32.000000 procyclingstats-0.1.5/procyclingstats/utils.py
-drwxr-xr-x   0 madzin    (1000) madzin    (1000)        0 2023-06-18 12:21:46.401969 procyclingstats-0.1.5/procyclingstats.egg-info/
--rw-r--r--   0 madzin    (1000) madzin    (1000)     2991 2023-06-18 12:21:46.000000 procyclingstats-0.1.5/procyclingstats.egg-info/PKG-INFO
--rw-r--r--   0 madzin    (1000) madzin    (1000)      676 2023-06-18 12:21:46.000000 procyclingstats-0.1.5/procyclingstats.egg-info/SOURCES.txt
--rw-r--r--   0 madzin    (1000) madzin    (1000)        1 2023-06-18 12:21:46.000000 procyclingstats-0.1.5/procyclingstats.egg-info/dependency_links.txt
--rw-r--r--   0 madzin    (1000) madzin    (1000)       20 2023-06-18 12:21:46.000000 procyclingstats-0.1.5/procyclingstats.egg-info/requires.txt
--rw-r--r--   0 madzin    (1000) madzin    (1000)       16 2023-06-18 12:21:46.000000 procyclingstats-0.1.5/procyclingstats.egg-info/top_level.txt
--rw-r--r--   0 madzin    (1000) madzin    (1000)      108 2023-06-18 12:21:46.405004 procyclingstats-0.1.5/setup.cfg
--rw-r--r--   0 madzin    (1000) madzin    (1000)      669 2023-06-18 12:21:30.000000 procyclingstats-0.1.5/setup.py
+drwxr-xr-x   0 madzin    (1000) madzin    (1000)        0 2023-07-21 19:15:21.887991 procyclingstats-0.1.6/
+-rw-r--r--   0 madzin    (1000) madzin    (1000)     2991 2023-07-21 19:15:21.889100 procyclingstats-0.1.6/PKG-INFO
+-rw-r--r--   0 madzin    (1000) madzin    (1000)     2042 2023-03-01 16:18:11.000000 procyclingstats-0.1.6/README.rst
+drwxr-xr-x   0 madzin    (1000) madzin    (1000)        0 2023-07-21 19:15:21.880797 procyclingstats-0.1.6/procyclingstats/
+-rw-r--r--   0 madzin    (1000) madzin    (1000)      599 2023-02-26 10:28:41.000000 procyclingstats-0.1.6/procyclingstats/__init__.py
+-rw-r--r--   0 madzin    (1000) madzin    (1000)     4235 2023-06-18 10:18:30.000000 procyclingstats-0.1.6/procyclingstats/__main__.py
+-rw-r--r--   0 madzin    (1000) madzin    (1000)     1304 2023-02-26 10:28:41.000000 procyclingstats-0.1.6/procyclingstats/errors.py
+-rw-r--r--   0 madzin    (1000) madzin    (1000)     3460 2023-06-18 10:26:43.000000 procyclingstats-0.1.6/procyclingstats/race_climbs_scraper.py
+-rw-r--r--   0 madzin    (1000) madzin    (1000)     6604 2023-06-17 19:29:12.000000 procyclingstats-0.1.6/procyclingstats/race_scraper.py
+-rw-r--r--   0 madzin    (1000) madzin    (1000)     4567 2023-06-17 17:21:57.000000 procyclingstats-0.1.6/procyclingstats/race_startlist_scraper.py
+-rw-r--r--   0 madzin    (1000) madzin    (1000)    19273 2023-06-17 17:23:51.000000 procyclingstats-0.1.6/procyclingstats/ranking_scraper.py
+-rw-r--r--   0 madzin    (1000) madzin    (1000)     8398 2023-06-17 17:23:38.000000 procyclingstats-0.1.6/procyclingstats/rider_results_scraper.py
+-rw-r--r--   0 madzin    (1000) madzin    (1000)     6876 2023-07-21 18:59:24.000000 procyclingstats-0.1.6/procyclingstats/rider_scraper.py
+-rw-r--r--   0 madzin    (1000) madzin    (1000)     6517 2023-06-17 17:22:57.000000 procyclingstats-0.1.6/procyclingstats/scraper.py
+-rw-r--r--   0 madzin    (1000) madzin    (1000)    23754 2023-06-18 11:20:14.000000 procyclingstats-0.1.6/procyclingstats/stage_scraper.py
+-rw-r--r--   0 madzin    (1000) madzin    (1000)    15221 2023-06-18 11:09:12.000000 procyclingstats-0.1.6/procyclingstats/table_parser.py
+-rw-r--r--   0 madzin    (1000) madzin    (1000)     9053 2023-06-17 17:24:59.000000 procyclingstats-0.1.6/procyclingstats/team_scraper.py
+-rw-r--r--   0 madzin    (1000) madzin    (1000)     6364 2023-06-17 17:25:32.000000 procyclingstats-0.1.6/procyclingstats/utils.py
+drwxr-xr-x   0 madzin    (1000) madzin    (1000)        0 2023-07-21 19:15:21.886740 procyclingstats-0.1.6/procyclingstats.egg-info/
+-rw-r--r--   0 madzin    (1000) madzin    (1000)     2991 2023-07-21 19:15:21.000000 procyclingstats-0.1.6/procyclingstats.egg-info/PKG-INFO
+-rw-r--r--   0 madzin    (1000) madzin    (1000)      676 2023-07-21 19:15:21.000000 procyclingstats-0.1.6/procyclingstats.egg-info/SOURCES.txt
+-rw-r--r--   0 madzin    (1000) madzin    (1000)        1 2023-07-21 19:15:21.000000 procyclingstats-0.1.6/procyclingstats.egg-info/dependency_links.txt
+-rw-r--r--   0 madzin    (1000) madzin    (1000)       20 2023-07-21 19:15:21.000000 procyclingstats-0.1.6/procyclingstats.egg-info/requires.txt
+-rw-r--r--   0 madzin    (1000) madzin    (1000)       16 2023-07-21 19:15:21.000000 procyclingstats-0.1.6/procyclingstats.egg-info/top_level.txt
+-rw-r--r--   0 madzin    (1000) madzin    (1000)      108 2023-07-21 19:15:21.889736 procyclingstats-0.1.6/setup.cfg
+-rw-r--r--   0 madzin    (1000) madzin    (1000)      669 2023-07-21 19:14:58.000000 procyclingstats-0.1.6/setup.py
```

### Comparing `procyclingstats-0.1.5/PKG-INFO` & `procyclingstats-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: procyclingstats
-Version: 0.1.5
+Version: 0.1.6
 Summary: A Python API wrapper for procyclingstats.com
 Home-page: https://github.com/themm1/procyclingstats
 Author: Martin Madzin
 Author-email: madzin.m@gmail.com
 License: MIT
 Description: procyclingstats
         ===============
```

### Comparing `procyclingstats-0.1.5/README.rst` & `procyclingstats-0.1.6/README.rst`

 * *Files identical despite different names*

### Comparing `procyclingstats-0.1.5/procyclingstats/__init__.py` & `procyclingstats-0.1.6/procyclingstats/__init__.py`

 * *Files identical despite different names*

### Comparing `procyclingstats-0.1.5/procyclingstats/__main__.py` & `procyclingstats-0.1.6/procyclingstats/__main__.py`

 * *Files identical despite different names*

### Comparing `procyclingstats-0.1.5/procyclingstats/errors.py` & `procyclingstats-0.1.6/procyclingstats/errors.py`

 * *Files identical despite different names*

### Comparing `procyclingstats-0.1.5/procyclingstats/race_climbs_scraper.py` & `procyclingstats-0.1.6/procyclingstats/race_climbs_scraper.py`

 * *Files identical despite different names*

### Comparing `procyclingstats-0.1.5/procyclingstats/race_scraper.py` & `procyclingstats-0.1.6/procyclingstats/race_scraper.py`

 * *Files identical despite different names*

### Comparing `procyclingstats-0.1.5/procyclingstats/race_startlist_scraper.py` & `procyclingstats-0.1.6/procyclingstats/race_startlist_scraper.py`

 * *Files identical despite different names*

### Comparing `procyclingstats-0.1.5/procyclingstats/ranking_scraper.py` & `procyclingstats-0.1.6/procyclingstats/ranking_scraper.py`

 * *Files identical despite different names*

### Comparing `procyclingstats-0.1.5/procyclingstats/rider_results_scraper.py` & `procyclingstats-0.1.6/procyclingstats/rider_results_scraper.py`

 * *Files identical despite different names*

### Comparing `procyclingstats-0.1.5/procyclingstats/rider_scraper.py` & `procyclingstats-0.1.6/procyclingstats/rider_scraper.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,28 +59,28 @@
         """
         Parses rider's name from HTML.
 
         :return: Rider's name.
         """
         return self.html.css_first(".page-title > .main > h1").text()
 
-    def weight(self) -> int:
+    def weight(self) -> float:
         """
         Parses rider's current weight from HTML.
 
         :return: Rider's weigth in kilograms.
         """
         # normal layout
         try:
             weight_html = self.html.css(".rdr-info-cont > span")[1]
-            return int(weight_html.text().split(" ")[1])
+            return float(weight_html.text().split(" ")[1])
         # special layout
         except (AttributeError, IndexError):
             weight_html = self.html.css(".rdr-info-cont > span > span")[1]
-            return int(weight_html.text().split(" ")[1])
+            return float(weight_html.text().split(" ")[1])
 
     def height(self) -> float:
         """
         Parses rider's height from HTML.
 
         :return: Rider's height in meters.
         """
```

### Comparing `procyclingstats-0.1.5/procyclingstats/scraper.py` & `procyclingstats-0.1.6/procyclingstats/scraper.py`

 * *Files identical despite different names*

### Comparing `procyclingstats-0.1.5/procyclingstats/stage_scraper.py` & `procyclingstats-0.1.6/procyclingstats/stage_scraper.py`

 * *Files identical despite different names*

### Comparing `procyclingstats-0.1.5/procyclingstats/table_parser.py` & `procyclingstats-0.1.6/procyclingstats/table_parser.py`

 * *Files identical despite different names*

### Comparing `procyclingstats-0.1.5/procyclingstats/team_scraper.py` & `procyclingstats-0.1.6/procyclingstats/team_scraper.py`

 * *Files identical despite different names*

### Comparing `procyclingstats-0.1.5/procyclingstats/utils.py` & `procyclingstats-0.1.6/procyclingstats/utils.py`

 * *Files identical despite different names*

### Comparing `procyclingstats-0.1.5/procyclingstats.egg-info/PKG-INFO` & `procyclingstats-0.1.6/procyclingstats.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: procyclingstats
-Version: 0.1.5
+Version: 0.1.6
 Summary: A Python API wrapper for procyclingstats.com
 Home-page: https://github.com/themm1/procyclingstats
 Author: Martin Madzin
 Author-email: madzin.m@gmail.com
 License: MIT
 Description: procyclingstats
         ===============
```

### Comparing `procyclingstats-0.1.5/procyclingstats.egg-info/SOURCES.txt` & `procyclingstats-0.1.6/procyclingstats.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `procyclingstats-0.1.5/setup.py` & `procyclingstats-0.1.6/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.rst", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="procyclingstats",
-    version="0.1.5",
+    version="0.1.6",
     license="MIT",
     description="A Python API wrapper for procyclingstats.com",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     author="Martin Madzin",
     author_email="madzin.m@gmail.com",
     packages=["procyclingstats"],
```

