# Comparing `tmp/streamlit_bmc-0.0.3.tar.gz` & `tmp/streamlit_bmc-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit_bmc-0.0.3.tar", last modified: Fri Jul 21 06:31:06 2023, max compression
+gzip compressed data, was "streamlit_bmc-0.0.4.tar", last modified: Fri Jul 21 09:59:11 2023, max compression
```

## Comparing `streamlit_bmc-0.0.3.tar` & `streamlit_bmc-0.0.4.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 teq-thuynguyen   (501) staff       (20)        0 2023-07-21 06:31:06.846464 streamlit_bmc-0.0.3/
--rw-r--r--   0 teq-thuynguyen   (501) staff       (20)     1063 2023-07-10 08:43:21.000000 streamlit_bmc-0.0.3/LICENSE
--rw-r--r--   0 teq-thuynguyen   (501) staff       (20)       47 2023-07-11 09:26:39.000000 streamlit_bmc-0.0.3/MANIFEST.in
--rw-r--r--   0 teq-thuynguyen   (501) staff       (20)      432 2023-07-21 06:31:06.846290 streamlit_bmc-0.0.3/PKG-INFO
--rw-r--r--   0 teq-thuynguyen   (501) staff       (20)     3137 2023-07-11 09:41:45.000000 streamlit_bmc-0.0.3/README.md
--rw-r--r--   0 teq-thuynguyen   (501) staff       (20)       38 2023-07-21 06:31:06.846518 streamlit_bmc-0.0.3/setup.cfg
--rw-r--r--   0 teq-thuynguyen   (501) staff       (20)      767 2023-07-21 06:30:08.000000 streamlit_bmc-0.0.3/setup.py
-drwxr-xr-x   0 teq-thuynguyen   (501) staff       (20)        0 2023-07-21 06:31:06.839146 streamlit_bmc-0.0.3/streamlit_bmc/
--rw-r--r--   0 teq-thuynguyen   (501) staff       (20)     6363 2023-07-13 02:10:00.000000 streamlit_bmc-0.0.3/streamlit_bmc/__init__.py
-drwxr-xr-x   0 teq-thuynguyen   (501) staff       (20)        0 2023-07-21 06:31:06.838115 streamlit_bmc-0.0.3/streamlit_bmc/frontend/
-drwxr-xr-x   0 teq-thuynguyen   (501) staff       (20)        0 2023-07-21 06:31:06.840510 streamlit_bmc-0.0.3/streamlit_bmc/frontend/public/
--rw-r--r--   0 teq-thuynguyen   (501) staff       (20)     8196 2023-07-15 04:44:40.000000 streamlit_bmc-0.0.3/streamlit_bmc/frontend/public/.DS_Store
-drwxr-xr-x   0 teq-thuynguyen   (501) staff       (20)        0 2023-07-21 06:31:06.841459 streamlit_bmc-0.0.3/streamlit_bmc/frontend/public/build/
--rw-r--r--   0 teq-thuynguyen   (501) staff       (20)       39 2023-07-21 06:29:51.000000 streamlit_bmc-0.0.3/streamlit_bmc/frontend/public/build/bundle.css
--rw-r--r--   0 teq-thuynguyen   (501) staff       (20)      116 2023-07-21 06:29:51.000000 streamlit_bmc-0.0.3/streamlit_bmc/frontend/public/build/bundle.css.map
--rw-r--r--   0 teq-thuynguyen   (501) staff       (20)   223732 2023-07-21 06:29:51.000000 streamlit_bmc-0.0.3/streamlit_bmc/frontend/public/build/bundle.js
--rw-r--r--   0 teq-thuynguyen   (501) staff       (20)  1117007 2023-07-21 06:29:51.000000 streamlit_bmc-0.0.3/streamlit_bmc/frontend/public/build/bundle.js.map
-drwxr-xr-x   0 teq-thuynguyen   (501) staff       (20)        0 2023-07-21 06:31:06.845988 streamlit_bmc-0.0.3/streamlit_bmc/frontend/public/img/
--rw-r--r--   0 teq-thuynguyen   (501) staff       (20)     6148 2023-07-13 08:11:33.000000 streamlit_bmc-0.0.3/streamlit_bmc/frontend/public/img/.DS_Store
--rw-r--r--   0 teq-thuynguyen   (501) staff       (20)     6308 2023-07-13 08:00:11.000000 streamlit_bmc-0.0.3/streamlit_bmc/frontend/public/img/bg-card-1.png
--rw-r--r--   0 teq-thuynguyen   (501) staff       (20)     6669 2023-07-13 08:11:00.000000 streamlit_bmc-0.0.3/streamlit_bmc/frontend/public/img/bg-card-2.png
--rw-r--r--   0 teq-thuynguyen   (501) staff       (20)     6613 2023-07-13 08:11:09.000000 streamlit_bmc-0.0.3/streamlit_bmc/frontend/public/img/bg-card-3.png
--rw-r--r--   0 teq-thuynguyen   (501) staff       (20)     6604 2023-07-13 08:11:25.000000 streamlit_bmc-0.0.3/streamlit_bmc/frontend/public/img/bg-card-4.png
--rw-r--r--   0 teq-thuynguyen   (501) staff       (20)     6517 2023-07-13 08:11:44.000000 streamlit_bmc-0.0.3/streamlit_bmc/frontend/public/img/bg-card-5.png
--rw-r--r--   0 teq-thuynguyen   (501) staff       (20)     6560 2023-07-13 08:11:52.000000 streamlit_bmc-0.0.3/streamlit_bmc/frontend/public/img/bg-card-6.png
--rw-r--r--   0 teq-thuynguyen   (501) staff       (20)     6605 2023-07-13 08:12:01.000000 streamlit_bmc-0.0.3/streamlit_bmc/frontend/public/img/bg-card-7.png
--rw-r--r--   0 teq-thuynguyen   (501) staff       (20)     6314 2023-07-13 08:12:50.000000 streamlit_bmc-0.0.3/streamlit_bmc/frontend/public/img/bg-card-8.png
--rw-r--r--   0 teq-thuynguyen   (501) staff       (20)     6620 2023-07-13 08:12:20.000000 streamlit_bmc-0.0.3/streamlit_bmc/frontend/public/img/bg-card-9.png
--rw-r--r--   0 teq-thuynguyen   (501) staff       (20)      304 2023-07-13 07:17:52.000000 streamlit_bmc-0.0.3/streamlit_bmc/frontend/public/img/bg.png
--rw-r--r--   0 teq-thuynguyen   (501) staff       (20)      554 2023-07-13 07:43:48.000000 streamlit_bmc-0.0.3/streamlit_bmc/frontend/public/img/icon-act.svg
--rw-r--r--   0 teq-thuynguyen   (501) staff       (20)      974 2023-07-13 07:44:25.000000 streamlit_bmc-0.0.3/streamlit_bmc/frontend/public/img/icon-cha.svg
--rw-r--r--   0 teq-thuynguyen   (501) staff       (20)     5088 2023-07-13 07:44:33.000000 streamlit_bmc-0.0.3/streamlit_bmc/frontend/public/img/icon-cos.svg
--rw-r--r--   0 teq-thuynguyen   (501) staff       (20)     2271 2023-07-13 07:43:33.000000 streamlit_bmc-0.0.3/streamlit_bmc/frontend/public/img/icon-par.svg
--rw-r--r--   0 teq-thuynguyen   (501) staff       (20)      585 2023-07-13 07:44:11.000000 streamlit_bmc-0.0.3/streamlit_bmc/frontend/public/img/icon-rel.svg
--rw-r--r--   0 teq-thuynguyen   (501) staff       (20)     1093 2023-07-13 07:44:20.000000 streamlit_bmc-0.0.3/streamlit_bmc/frontend/public/img/icon-res.svg
--rw-r--r--   0 teq-thuynguyen   (501) staff       (20)      668 2023-07-13 07:44:37.000000 streamlit_bmc-0.0.3/streamlit_bmc/frontend/public/img/icon-rev.svg
--rw-r--r--   0 teq-thuynguyen   (501) staff       (20)      953 2023-07-13 07:44:15.000000 streamlit_bmc-0.0.3/streamlit_bmc/frontend/public/img/icon-seg.svg
--rw-r--r--   0 teq-thuynguyen   (501) staff       (20)      886 2023-07-13 07:44:02.000000 streamlit_bmc-0.0.3/streamlit_bmc/frontend/public/img/icon-val.svg
--rw-r--r--   0 teq-thuynguyen   (501) staff       (20)     1364 2023-07-21 04:15:43.000000 streamlit_bmc-0.0.3/streamlit_bmc/frontend/public/index.html
--rw-r--r--   0 teq-thuynguyen   (501) staff       (20)     5026 2023-07-21 06:27:07.000000 streamlit_bmc-0.0.3/streamlit_bmc/frontend/public/style.css
-drwxr-xr-x   0 teq-thuynguyen   (501) staff       (20)        0 2023-07-21 06:31:06.839992 streamlit_bmc-0.0.3/streamlit_bmc.egg-info/
--rw-r--r--   0 teq-thuynguyen   (501) staff       (20)      432 2023-07-21 06:31:06.000000 streamlit_bmc-0.0.3/streamlit_bmc.egg-info/PKG-INFO
--rw-r--r--   0 teq-thuynguyen   (501) staff       (20)     1503 2023-07-21 06:31:06.000000 streamlit_bmc-0.0.3/streamlit_bmc.egg-info/SOURCES.txt
--rw-r--r--   0 teq-thuynguyen   (501) staff       (20)        1 2023-07-21 06:31:06.000000 streamlit_bmc-0.0.3/streamlit_bmc.egg-info/dependency_links.txt
--rw-r--r--   0 teq-thuynguyen   (501) staff       (20)       16 2023-07-21 06:31:06.000000 streamlit_bmc-0.0.3/streamlit_bmc.egg-info/requires.txt
--rw-r--r--   0 teq-thuynguyen   (501) staff       (20)       14 2023-07-21 06:31:06.000000 streamlit_bmc-0.0.3/streamlit_bmc.egg-info/top_level.txt
+drwxr-xr-x   0 teq-thuynguyen   (501) staff       (20)        0 2023-07-21 09:59:11.832715 streamlit_bmc-0.0.4/
+-rw-r--r--   0 teq-thuynguyen   (501) staff       (20)     1063 2023-07-10 08:43:21.000000 streamlit_bmc-0.0.4/LICENSE
+-rw-r--r--   0 teq-thuynguyen   (501) staff       (20)       47 2023-07-11 09:26:39.000000 streamlit_bmc-0.0.4/MANIFEST.in
+-rw-r--r--   0 teq-thuynguyen   (501) staff       (20)      432 2023-07-21 09:59:11.832575 streamlit_bmc-0.0.4/PKG-INFO
+-rw-r--r--   0 teq-thuynguyen   (501) staff       (20)     3075 2023-07-21 06:44:44.000000 streamlit_bmc-0.0.4/README.md
+-rw-r--r--   0 teq-thuynguyen   (501) staff       (20)       38 2023-07-21 09:59:11.832768 streamlit_bmc-0.0.4/setup.cfg
+-rw-r--r--   0 teq-thuynguyen   (501) staff       (20)      767 2023-07-21 09:58:38.000000 streamlit_bmc-0.0.4/setup.py
+drwxr-xr-x   0 teq-thuynguyen   (501) staff       (20)        0 2023-07-21 09:59:11.810532 streamlit_bmc-0.0.4/streamlit_bmc/
+-rw-r--r--   0 teq-thuynguyen   (501) staff       (20)     6362 2023-07-21 09:54:34.000000 streamlit_bmc-0.0.4/streamlit_bmc/__init__.py
+drwxr-xr-x   0 teq-thuynguyen   (501) staff       (20)        0 2023-07-21 09:59:11.808885 streamlit_bmc-0.0.4/streamlit_bmc/frontend/
+drwxr-xr-x   0 teq-thuynguyen   (501) staff       (20)        0 2023-07-21 09:59:11.814789 streamlit_bmc-0.0.4/streamlit_bmc/frontend/public/
+-rw-r--r--   0 teq-thuynguyen   (501) staff       (20)     8196 2023-07-15 04:44:40.000000 streamlit_bmc-0.0.4/streamlit_bmc/frontend/public/.DS_Store
+drwxr-xr-x   0 teq-thuynguyen   (501) staff       (20)        0 2023-07-21 09:59:11.816396 streamlit_bmc-0.0.4/streamlit_bmc/frontend/public/build/
+-rw-r--r--   0 teq-thuynguyen   (501) staff       (20)       39 2023-07-21 06:29:51.000000 streamlit_bmc-0.0.4/streamlit_bmc/frontend/public/build/bundle.css
+-rw-r--r--   0 teq-thuynguyen   (501) staff       (20)      116 2023-07-21 06:29:51.000000 streamlit_bmc-0.0.4/streamlit_bmc/frontend/public/build/bundle.css.map
+-rw-r--r--   0 teq-thuynguyen   (501) staff       (20)   223732 2023-07-21 06:29:51.000000 streamlit_bmc-0.0.4/streamlit_bmc/frontend/public/build/bundle.js
+-rw-r--r--   0 teq-thuynguyen   (501) staff       (20)  1117007 2023-07-21 06:29:51.000000 streamlit_bmc-0.0.4/streamlit_bmc/frontend/public/build/bundle.js.map
+drwxr-xr-x   0 teq-thuynguyen   (501) staff       (20)        0 2023-07-21 09:59:11.832240 streamlit_bmc-0.0.4/streamlit_bmc/frontend/public/img/
+-rw-r--r--   0 teq-thuynguyen   (501) staff       (20)     6148 2023-07-13 08:11:33.000000 streamlit_bmc-0.0.4/streamlit_bmc/frontend/public/img/.DS_Store
+-rw-r--r--   0 teq-thuynguyen   (501) staff       (20)     6308 2023-07-13 08:00:11.000000 streamlit_bmc-0.0.4/streamlit_bmc/frontend/public/img/bg-card-1.png
+-rw-r--r--   0 teq-thuynguyen   (501) staff       (20)     6669 2023-07-13 08:11:00.000000 streamlit_bmc-0.0.4/streamlit_bmc/frontend/public/img/bg-card-2.png
+-rw-r--r--   0 teq-thuynguyen   (501) staff       (20)     6613 2023-07-13 08:11:09.000000 streamlit_bmc-0.0.4/streamlit_bmc/frontend/public/img/bg-card-3.png
+-rw-r--r--   0 teq-thuynguyen   (501) staff       (20)     6604 2023-07-13 08:11:25.000000 streamlit_bmc-0.0.4/streamlit_bmc/frontend/public/img/bg-card-4.png
+-rw-r--r--   0 teq-thuynguyen   (501) staff       (20)     6517 2023-07-13 08:11:44.000000 streamlit_bmc-0.0.4/streamlit_bmc/frontend/public/img/bg-card-5.png
+-rw-r--r--   0 teq-thuynguyen   (501) staff       (20)     6560 2023-07-13 08:11:52.000000 streamlit_bmc-0.0.4/streamlit_bmc/frontend/public/img/bg-card-6.png
+-rw-r--r--   0 teq-thuynguyen   (501) staff       (20)     6605 2023-07-13 08:12:01.000000 streamlit_bmc-0.0.4/streamlit_bmc/frontend/public/img/bg-card-7.png
+-rw-r--r--   0 teq-thuynguyen   (501) staff       (20)     6314 2023-07-13 08:12:50.000000 streamlit_bmc-0.0.4/streamlit_bmc/frontend/public/img/bg-card-8.png
+-rw-r--r--   0 teq-thuynguyen   (501) staff       (20)     6620 2023-07-13 08:12:20.000000 streamlit_bmc-0.0.4/streamlit_bmc/frontend/public/img/bg-card-9.png
+-rw-r--r--   0 teq-thuynguyen   (501) staff       (20)      304 2023-07-13 07:17:52.000000 streamlit_bmc-0.0.4/streamlit_bmc/frontend/public/img/bg.png
+-rw-r--r--   0 teq-thuynguyen   (501) staff       (20)      554 2023-07-13 07:43:48.000000 streamlit_bmc-0.0.4/streamlit_bmc/frontend/public/img/icon-act.svg
+-rw-r--r--   0 teq-thuynguyen   (501) staff       (20)      974 2023-07-13 07:44:25.000000 streamlit_bmc-0.0.4/streamlit_bmc/frontend/public/img/icon-cha.svg
+-rw-r--r--   0 teq-thuynguyen   (501) staff       (20)     5088 2023-07-13 07:44:33.000000 streamlit_bmc-0.0.4/streamlit_bmc/frontend/public/img/icon-cos.svg
+-rw-r--r--   0 teq-thuynguyen   (501) staff       (20)     2271 2023-07-13 07:43:33.000000 streamlit_bmc-0.0.4/streamlit_bmc/frontend/public/img/icon-par.svg
+-rw-r--r--   0 teq-thuynguyen   (501) staff       (20)      585 2023-07-13 07:44:11.000000 streamlit_bmc-0.0.4/streamlit_bmc/frontend/public/img/icon-rel.svg
+-rw-r--r--   0 teq-thuynguyen   (501) staff       (20)     1093 2023-07-13 07:44:20.000000 streamlit_bmc-0.0.4/streamlit_bmc/frontend/public/img/icon-res.svg
+-rw-r--r--   0 teq-thuynguyen   (501) staff       (20)      668 2023-07-13 07:44:37.000000 streamlit_bmc-0.0.4/streamlit_bmc/frontend/public/img/icon-rev.svg
+-rw-r--r--   0 teq-thuynguyen   (501) staff       (20)      953 2023-07-13 07:44:15.000000 streamlit_bmc-0.0.4/streamlit_bmc/frontend/public/img/icon-seg.svg
+-rw-r--r--   0 teq-thuynguyen   (501) staff       (20)      886 2023-07-13 07:44:02.000000 streamlit_bmc-0.0.4/streamlit_bmc/frontend/public/img/icon-val.svg
+-rw-r--r--   0 teq-thuynguyen   (501) staff       (20)     1364 2023-07-21 04:15:43.000000 streamlit_bmc-0.0.4/streamlit_bmc/frontend/public/index.html
+-rw-r--r--   0 teq-thuynguyen   (501) staff       (20)     5026 2023-07-21 06:27:07.000000 streamlit_bmc-0.0.4/streamlit_bmc/frontend/public/style.css
+drwxr-xr-x   0 teq-thuynguyen   (501) staff       (20)        0 2023-07-21 09:59:11.811641 streamlit_bmc-0.0.4/streamlit_bmc.egg-info/
+-rw-r--r--   0 teq-thuynguyen   (501) staff       (20)      432 2023-07-21 09:59:11.000000 streamlit_bmc-0.0.4/streamlit_bmc.egg-info/PKG-INFO
+-rw-r--r--   0 teq-thuynguyen   (501) staff       (20)     1503 2023-07-21 09:59:11.000000 streamlit_bmc-0.0.4/streamlit_bmc.egg-info/SOURCES.txt
+-rw-r--r--   0 teq-thuynguyen   (501) staff       (20)        1 2023-07-21 09:59:11.000000 streamlit_bmc-0.0.4/streamlit_bmc.egg-info/dependency_links.txt
+-rw-r--r--   0 teq-thuynguyen   (501) staff       (20)       16 2023-07-21 09:59:11.000000 streamlit_bmc-0.0.4/streamlit_bmc.egg-info/requires.txt
+-rw-r--r--   0 teq-thuynguyen   (501) staff       (20)       14 2023-07-21 09:59:11.000000 streamlit_bmc-0.0.4/streamlit_bmc.egg-info/top_level.txt
```

### Comparing `streamlit_bmc-0.0.3/LICENSE` & `streamlit_bmc-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit_bmc-0.0.3/README.md` & `streamlit_bmc-0.0.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -96,15 +96,15 @@
 ## Demo
 
 <!-- [![Open in Streamlit][share_badge]][share_link]  -->
 
 [![Preview][share_img]][share_link]
 
 [share_badge]: https://static.streamlit.io/badges/streamlit_badge_black_white.svg
-[share_link]: https://share.streamlit.io/okld/streamlit-gallery/main?p=ace-editor
+[share_link]: http://bmc.dev.teqn.asia/
 [share_img]: https://raw.githubusercontent.com/teq-thuynguyen/streamlit-business_model_canvas/main/preview.png
 
 [github_badge]: https://badgen.net/badge/icon/GitHub?icon=github&color=black&label
 [github_link]: https://github.com/teq-thuynguyen/streamlit-business_model_canvas
 
-[pypi_badge]: https://badgen.net/pypi/v/streamlit-ace?icon=pypi&color=black&label
+[pypi_badge]: https://img.shields.io/badge/version-0.0.3-blue
 [pypi_link]: https://pypi.org/project/streamlit-bmc/
```

### Comparing `streamlit_bmc-0.0.3/setup.py` & `streamlit_bmc-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="streamlit_bmc",
-    version="0.0.3",
+    version="0.0.4",
     author="Ember",
     author_email="nguyencaonguyenthuy@gmail.com",
     description="A Streamlit Component for drawing Business Model Canvas",
     long_description="A Streamlit Component for drawing Business Model Canvas",
     long_description_content_type="text/plain",
     url="https://github.com/teq-thuynguyen/streamlit-business_model_canvas",
     packages=setuptools.find_packages(),
```

### Comparing `streamlit_bmc-0.0.3/streamlit_bmc/__init__.py` & `streamlit_bmc-0.0.4/streamlit_bmc/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import streamlit.components.v1 as components
 
 # Create a _RELEASE constant. We'll set this to False while we're developing
 # the component, and True when we're ready to package and distribute it.
 # (This is, of course, optional - there are innumerable ways to manage your
 # release process.)
-_RELEASE = False
+_RELEASE = True
 
 # Declare a Streamlit component. `declare_component` returns a function
 # that is used to create instances of the component. We're naming this
 # function "_component_func", with an underscore prefix, because we don't want
 # to expose it directly to users. Instead, we will create a custom wrapper
 # function, below, that will serve as our component's public API.
```

### Comparing `streamlit_bmc-0.0.3/streamlit_bmc/frontend/public/.DS_Store` & `streamlit_bmc-0.0.4/streamlit_bmc/frontend/public/.DS_Store`

 * *Files identical despite different names*

### Comparing `streamlit_bmc-0.0.3/streamlit_bmc/frontend/public/build/bundle.js` & `streamlit_bmc-0.0.4/streamlit_bmc/frontend/public/build/bundle.js`

 * *Files identical despite different names*

### Comparing `streamlit_bmc-0.0.3/streamlit_bmc/frontend/public/build/bundle.js.map` & `streamlit_bmc-0.0.4/streamlit_bmc/frontend/public/build/bundle.js.map`

 * *Files identical despite different names*

### Comparing `streamlit_bmc-0.0.3/streamlit_bmc/frontend/public/img/.DS_Store` & `streamlit_bmc-0.0.4/streamlit_bmc/frontend/public/img/.DS_Store`

 * *Files identical despite different names*

### Comparing `streamlit_bmc-0.0.3/streamlit_bmc/frontend/public/img/bg-card-1.png` & `streamlit_bmc-0.0.4/streamlit_bmc/frontend/public/img/bg-card-1.png`

 * *Files identical despite different names*

### Comparing `streamlit_bmc-0.0.3/streamlit_bmc/frontend/public/img/bg-card-2.png` & `streamlit_bmc-0.0.4/streamlit_bmc/frontend/public/img/bg-card-2.png`

 * *Files identical despite different names*

### Comparing `streamlit_bmc-0.0.3/streamlit_bmc/frontend/public/img/bg-card-3.png` & `streamlit_bmc-0.0.4/streamlit_bmc/frontend/public/img/bg-card-3.png`

 * *Files identical despite different names*

### Comparing `streamlit_bmc-0.0.3/streamlit_bmc/frontend/public/img/bg-card-4.png` & `streamlit_bmc-0.0.4/streamlit_bmc/frontend/public/img/bg-card-4.png`

 * *Files identical despite different names*

### Comparing `streamlit_bmc-0.0.3/streamlit_bmc/frontend/public/img/bg-card-5.png` & `streamlit_bmc-0.0.4/streamlit_bmc/frontend/public/img/bg-card-5.png`

 * *Files identical despite different names*

### Comparing `streamlit_bmc-0.0.3/streamlit_bmc/frontend/public/img/bg-card-6.png` & `streamlit_bmc-0.0.4/streamlit_bmc/frontend/public/img/bg-card-6.png`

 * *Files identical despite different names*

### Comparing `streamlit_bmc-0.0.3/streamlit_bmc/frontend/public/img/bg-card-7.png` & `streamlit_bmc-0.0.4/streamlit_bmc/frontend/public/img/bg-card-7.png`

 * *Files identical despite different names*

### Comparing `streamlit_bmc-0.0.3/streamlit_bmc/frontend/public/img/bg-card-8.png` & `streamlit_bmc-0.0.4/streamlit_bmc/frontend/public/img/bg-card-8.png`

 * *Files identical despite different names*

### Comparing `streamlit_bmc-0.0.3/streamlit_bmc/frontend/public/img/bg-card-9.png` & `streamlit_bmc-0.0.4/streamlit_bmc/frontend/public/img/bg-card-9.png`

 * *Files identical despite different names*

### Comparing `streamlit_bmc-0.0.3/streamlit_bmc/frontend/public/img/icon-act.svg` & `streamlit_bmc-0.0.4/streamlit_bmc/frontend/public/img/icon-act.svg`

 * *Files identical despite different names*

### Comparing `streamlit_bmc-0.0.3/streamlit_bmc/frontend/public/img/icon-cha.svg` & `streamlit_bmc-0.0.4/streamlit_bmc/frontend/public/img/icon-cha.svg`

 * *Files identical despite different names*

### Comparing `streamlit_bmc-0.0.3/streamlit_bmc/frontend/public/img/icon-cos.svg` & `streamlit_bmc-0.0.4/streamlit_bmc/frontend/public/img/icon-cos.svg`

 * *Files identical despite different names*

### Comparing `streamlit_bmc-0.0.3/streamlit_bmc/frontend/public/img/icon-par.svg` & `streamlit_bmc-0.0.4/streamlit_bmc/frontend/public/img/icon-par.svg`

 * *Files identical despite different names*

### Comparing `streamlit_bmc-0.0.3/streamlit_bmc/frontend/public/img/icon-rel.svg` & `streamlit_bmc-0.0.4/streamlit_bmc/frontend/public/img/icon-rel.svg`

 * *Files identical despite different names*

### Comparing `streamlit_bmc-0.0.3/streamlit_bmc/frontend/public/img/icon-res.svg` & `streamlit_bmc-0.0.4/streamlit_bmc/frontend/public/img/icon-res.svg`

 * *Files identical despite different names*

### Comparing `streamlit_bmc-0.0.3/streamlit_bmc/frontend/public/img/icon-rev.svg` & `streamlit_bmc-0.0.4/streamlit_bmc/frontend/public/img/icon-rev.svg`

 * *Files identical despite different names*

### Comparing `streamlit_bmc-0.0.3/streamlit_bmc/frontend/public/img/icon-seg.svg` & `streamlit_bmc-0.0.4/streamlit_bmc/frontend/public/img/icon-seg.svg`

 * *Files identical despite different names*

### Comparing `streamlit_bmc-0.0.3/streamlit_bmc/frontend/public/img/icon-val.svg` & `streamlit_bmc-0.0.4/streamlit_bmc/frontend/public/img/icon-val.svg`

 * *Files identical despite different names*

### Comparing `streamlit_bmc-0.0.3/streamlit_bmc/frontend/public/index.html` & `streamlit_bmc-0.0.4/streamlit_bmc/frontend/public/index.html`

 * *Files identical despite different names*

### Comparing `streamlit_bmc-0.0.3/streamlit_bmc/frontend/public/style.css` & `streamlit_bmc-0.0.4/streamlit_bmc/frontend/public/style.css`

 * *Files identical despite different names*

### Comparing `streamlit_bmc-0.0.3/streamlit_bmc.egg-info/SOURCES.txt` & `streamlit_bmc-0.0.4/streamlit_bmc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

