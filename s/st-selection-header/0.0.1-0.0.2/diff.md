# Comparing `tmp/st-selection-header-0.0.1.tar.gz` & `tmp/st-selection-header-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "st-selection-header-0.0.1.tar", last modified: Fri Jul 21 16:11:09 2023, max compression
+gzip compressed data, was "st-selection-header-0.0.2.tar", last modified: Fri Jul 21 16:12:33 2023, max compression
```

## Comparing `st-selection-header-0.0.1.tar` & `st-selection-header-0.0.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 elliotglas   (501) staff       (20)        0 2023-07-21 16:11:09.090508 st-selection-header-0.0.1/
--rw-r--r--   0 elliotglas   (501) staff       (20)     2340 2023-07-21 13:50:11.000000 st-selection-header-0.0.1/LICENSE
--rw-r--r--   0 elliotglas   (501) staff       (20)       55 2023-07-21 13:55:00.000000 st-selection-header-0.0.1/MANIFEST.in
--rw-r--r--   0 elliotglas   (501) staff       (20)      274 2023-07-21 16:11:09.090306 st-selection-header-0.0.1/PKG-INFO
--rw-r--r--   0 elliotglas   (501) staff       (20)       38 2023-07-21 16:11:09.090588 st-selection-header-0.0.1/setup.cfg
--rw-r--r--   0 elliotglas   (501) staff       (20)      645 2023-07-21 16:10:14.000000 st-selection-header-0.0.1/setup.py
-drwxr-xr-x   0 elliotglas   (501) staff       (20)        0 2023-07-21 16:11:09.083226 st-selection-header-0.0.1/st_selection_header/
--rw-r--r--   0 elliotglas   (501) staff       (20)      816 2023-07-21 16:07:24.000000 st-selection-header-0.0.1/st_selection_header/__init__.py
-drwxr-xr-x   0 elliotglas   (501) staff       (20)        0 2023-07-21 16:11:09.082248 st-selection-header-0.0.1/st_selection_header/frontend/
-drwxr-xr-x   0 elliotglas   (501) staff       (20)        0 2023-07-21 16:11:09.085272 st-selection-header-0.0.1/st_selection_header/frontend/build/
--rw-r--r--   0 elliotglas   (501) staff       (20)      691 2023-07-21 16:09:20.000000 st-selection-header-0.0.1/st_selection_header/frontend/build/asset-manifest.json
--rw-r--r--   0 elliotglas   (501) staff       (20)     2119 2023-07-21 16:09:20.000000 st-selection-header-0.0.1/st_selection_header/frontend/build/index.html
-drwxr-xr-x   0 elliotglas   (501) staff       (20)        0 2023-07-21 16:11:09.082445 st-selection-header-0.0.1/st_selection_header/frontend/build/static/
-drwxr-xr-x   0 elliotglas   (501) staff       (20)        0 2023-07-21 16:11:09.090021 st-selection-header-0.0.1/st_selection_header/frontend/build/static/js/
--rw-r--r--   0 elliotglas   (501) staff       (20)   924549 2023-07-21 16:09:20.000000 st-selection-header-0.0.1/st_selection_header/frontend/build/static/js/2.0a2a2974.chunk.js
--rw-r--r--   0 elliotglas   (501) staff       (20)     2484 2023-07-21 16:09:20.000000 st-selection-header-0.0.1/st_selection_header/frontend/build/static/js/2.0a2a2974.chunk.js.LICENSE.txt
--rw-r--r--   0 elliotglas   (501) staff       (20)  3811745 2023-07-21 16:09:20.000000 st-selection-header-0.0.1/st_selection_header/frontend/build/static/js/2.0a2a2974.chunk.js.map
--rw-r--r--   0 elliotglas   (501) staff       (20)     4487 2023-07-21 16:09:20.000000 st-selection-header-0.0.1/st_selection_header/frontend/build/static/js/main.dbfd7619.chunk.js
--rw-r--r--   0 elliotglas   (501) staff       (20)    13788 2023-07-21 16:09:20.000000 st-selection-header-0.0.1/st_selection_header/frontend/build/static/js/main.dbfd7619.chunk.js.map
--rw-r--r--   0 elliotglas   (501) staff       (20)     1598 2023-07-21 16:09:20.000000 st-selection-header-0.0.1/st_selection_header/frontend/build/static/js/runtime-main.39defc4e.js
--rw-r--r--   0 elliotglas   (501) staff       (20)     8383 2023-07-21 16:09:20.000000 st-selection-header-0.0.1/st_selection_header/frontend/build/static/js/runtime-main.39defc4e.js.map
-drwxr-xr-x   0 elliotglas   (501) staff       (20)        0 2023-07-21 16:11:09.084828 st-selection-header-0.0.1/st_selection_header.egg-info/
--rw-r--r--   0 elliotglas   (501) staff       (20)      274 2023-07-21 16:11:08.000000 st-selection-header-0.0.1/st_selection_header.egg-info/PKG-INFO
--rw-r--r--   0 elliotglas   (501) staff       (20)      870 2023-07-21 16:11:09.000000 st-selection-header-0.0.1/st_selection_header.egg-info/SOURCES.txt
--rw-r--r--   0 elliotglas   (501) staff       (20)        1 2023-07-21 16:11:08.000000 st-selection-header-0.0.1/st_selection_header.egg-info/dependency_links.txt
--rw-r--r--   0 elliotglas   (501) staff       (20)       16 2023-07-21 16:11:08.000000 st-selection-header-0.0.1/st_selection_header.egg-info/requires.txt
--rw-r--r--   0 elliotglas   (501) staff       (20)       20 2023-07-21 16:11:08.000000 st-selection-header-0.0.1/st_selection_header.egg-info/top_level.txt
+drwxr-xr-x   0 elliotglas   (501) staff       (20)        0 2023-07-21 16:12:33.165084 st-selection-header-0.0.2/
+-rw-r--r--   0 elliotglas   (501) staff       (20)     2340 2023-07-21 13:50:11.000000 st-selection-header-0.0.2/LICENSE
+-rw-r--r--   0 elliotglas   (501) staff       (20)       55 2023-07-21 13:55:00.000000 st-selection-header-0.0.2/MANIFEST.in
+-rw-r--r--   0 elliotglas   (501) staff       (20)      274 2023-07-21 16:12:33.164890 st-selection-header-0.0.2/PKG-INFO
+-rw-r--r--   0 elliotglas   (501) staff       (20)       38 2023-07-21 16:12:33.165217 st-selection-header-0.0.2/setup.cfg
+-rw-r--r--   0 elliotglas   (501) staff       (20)      645 2023-07-21 16:12:27.000000 st-selection-header-0.0.2/setup.py
+drwxr-xr-x   0 elliotglas   (501) staff       (20)        0 2023-07-21 16:12:33.158368 st-selection-header-0.0.2/st_selection_header/
+-rw-r--r--   0 elliotglas   (501) staff       (20)      813 2023-07-21 16:11:57.000000 st-selection-header-0.0.2/st_selection_header/__init__.py
+drwxr-xr-x   0 elliotglas   (501) staff       (20)        0 2023-07-21 16:12:33.157000 st-selection-header-0.0.2/st_selection_header/frontend/
+drwxr-xr-x   0 elliotglas   (501) staff       (20)        0 2023-07-21 16:12:33.159987 st-selection-header-0.0.2/st_selection_header/frontend/build/
+-rw-r--r--   0 elliotglas   (501) staff       (20)      691 2023-07-21 16:09:20.000000 st-selection-header-0.0.2/st_selection_header/frontend/build/asset-manifest.json
+-rw-r--r--   0 elliotglas   (501) staff       (20)     2119 2023-07-21 16:09:20.000000 st-selection-header-0.0.2/st_selection_header/frontend/build/index.html
+drwxr-xr-x   0 elliotglas   (501) staff       (20)        0 2023-07-21 16:12:33.157316 st-selection-header-0.0.2/st_selection_header/frontend/build/static/
+drwxr-xr-x   0 elliotglas   (501) staff       (20)        0 2023-07-21 16:12:33.164625 st-selection-header-0.0.2/st_selection_header/frontend/build/static/js/
+-rw-r--r--   0 elliotglas   (501) staff       (20)   924549 2023-07-21 16:09:20.000000 st-selection-header-0.0.2/st_selection_header/frontend/build/static/js/2.0a2a2974.chunk.js
+-rw-r--r--   0 elliotglas   (501) staff       (20)     2484 2023-07-21 16:09:20.000000 st-selection-header-0.0.2/st_selection_header/frontend/build/static/js/2.0a2a2974.chunk.js.LICENSE.txt
+-rw-r--r--   0 elliotglas   (501) staff       (20)  3811745 2023-07-21 16:09:20.000000 st-selection-header-0.0.2/st_selection_header/frontend/build/static/js/2.0a2a2974.chunk.js.map
+-rw-r--r--   0 elliotglas   (501) staff       (20)     4487 2023-07-21 16:09:20.000000 st-selection-header-0.0.2/st_selection_header/frontend/build/static/js/main.dbfd7619.chunk.js
+-rw-r--r--   0 elliotglas   (501) staff       (20)    13788 2023-07-21 16:09:20.000000 st-selection-header-0.0.2/st_selection_header/frontend/build/static/js/main.dbfd7619.chunk.js.map
+-rw-r--r--   0 elliotglas   (501) staff       (20)     1598 2023-07-21 16:09:20.000000 st-selection-header-0.0.2/st_selection_header/frontend/build/static/js/runtime-main.39defc4e.js
+-rw-r--r--   0 elliotglas   (501) staff       (20)     8383 2023-07-21 16:09:20.000000 st-selection-header-0.0.2/st_selection_header/frontend/build/static/js/runtime-main.39defc4e.js.map
+drwxr-xr-x   0 elliotglas   (501) staff       (20)        0 2023-07-21 16:12:33.159316 st-selection-header-0.0.2/st_selection_header.egg-info/
+-rw-r--r--   0 elliotglas   (501) staff       (20)      274 2023-07-21 16:12:33.000000 st-selection-header-0.0.2/st_selection_header.egg-info/PKG-INFO
+-rw-r--r--   0 elliotglas   (501) staff       (20)      870 2023-07-21 16:12:33.000000 st-selection-header-0.0.2/st_selection_header.egg-info/SOURCES.txt
+-rw-r--r--   0 elliotglas   (501) staff       (20)        1 2023-07-21 16:12:33.000000 st-selection-header-0.0.2/st_selection_header.egg-info/dependency_links.txt
+-rw-r--r--   0 elliotglas   (501) staff       (20)       16 2023-07-21 16:12:33.000000 st-selection-header-0.0.2/st_selection_header.egg-info/requires.txt
+-rw-r--r--   0 elliotglas   (501) staff       (20)       20 2023-07-21 16:12:33.000000 st-selection-header-0.0.2/st_selection_header.egg-info/top_level.txt
```

### Comparing `st-selection-header-0.0.1/LICENSE` & `st-selection-header-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `st-selection-header-0.0.1/st_selection_header/__init__.py` & `st-selection-header-0.0.2/st_selection_header/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 import os
 import streamlit.components.v1 as components
 from typing import List, Dict
 
-
-_RELEASE = False
-
+_RELEASE = True
 
 if not _RELEASE:
     _component_func = components.declare_component(
         "st_selection_header",
         url="http://localhost:3001",
     )
 else:
```

### Comparing `st-selection-header-0.0.1/st_selection_header/frontend/build/asset-manifest.json` & `st-selection-header-0.0.2/st_selection_header/frontend/build/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `st-selection-header-0.0.1/st_selection_header/frontend/build/index.html` & `st-selection-header-0.0.2/st_selection_header/frontend/build/index.html`

 * *Files identical despite different names*

### Comparing `st-selection-header-0.0.1/st_selection_header/frontend/build/static/js/2.0a2a2974.chunk.js` & `st-selection-header-0.0.2/st_selection_header/frontend/build/static/js/2.0a2a2974.chunk.js`

 * *Files identical despite different names*

### Comparing `st-selection-header-0.0.1/st_selection_header/frontend/build/static/js/2.0a2a2974.chunk.js.LICENSE.txt` & `st-selection-header-0.0.2/st_selection_header/frontend/build/static/js/2.0a2a2974.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `st-selection-header-0.0.1/st_selection_header/frontend/build/static/js/2.0a2a2974.chunk.js.map` & `st-selection-header-0.0.2/st_selection_header/frontend/build/static/js/2.0a2a2974.chunk.js.map`

 * *Files identical despite different names*

### Comparing `st-selection-header-0.0.1/st_selection_header/frontend/build/static/js/main.dbfd7619.chunk.js` & `st-selection-header-0.0.2/st_selection_header/frontend/build/static/js/main.dbfd7619.chunk.js`

 * *Files identical despite different names*

### Comparing `st-selection-header-0.0.1/st_selection_header/frontend/build/static/js/main.dbfd7619.chunk.js.map` & `st-selection-header-0.0.2/st_selection_header/frontend/build/static/js/main.dbfd7619.chunk.js.map`

 * *Files identical despite different names*

### Comparing `st-selection-header-0.0.1/st_selection_header/frontend/build/static/js/runtime-main.39defc4e.js` & `st-selection-header-0.0.2/st_selection_header/frontend/build/static/js/runtime-main.39defc4e.js`

 * *Files identical despite different names*

### Comparing `st-selection-header-0.0.1/st_selection_header/frontend/build/static/js/runtime-main.39defc4e.js.map` & `st-selection-header-0.0.2/st_selection_header/frontend/build/static/js/runtime-main.39defc4e.js.map`

 * *Files identical despite different names*

### Comparing `st-selection-header-0.0.1/st_selection_header.egg-info/SOURCES.txt` & `st-selection-header-0.0.2/st_selection_header.egg-info/SOURCES.txt`

 * *Files identical despite different names*

