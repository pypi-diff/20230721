# Comparing `tmp/astrotitles-0.1.5.tar.gz` & `tmp/astrotitles-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astrotitles-0.1.5.tar", last modified: Fri Jul 21 19:35:26 2023, max compression
+gzip compressed data, was "astrotitles-0.1.6.tar", last modified: Fri Jul 21 21:33:16 2023, max compression
```

## Comparing `astrotitles-0.1.5.tar` & `astrotitles-0.1.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-07-21 19:35:26.102488 astrotitles-0.1.5/
--rw-r--r--   0 ben        (501) staff       (20)    34523 2023-07-19 22:08:12.000000 astrotitles-0.1.5/LICENCE.txt
--rw-r--r--   0 ben        (501) staff       (20)     4701 2023-07-21 19:35:26.102573 astrotitles-0.1.5/PKG-INFO
--rw-r--r--   0 ben        (501) staff       (20)     4324 2023-07-21 19:22:36.000000 astrotitles-0.1.5/README.md
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-07-21 19:35:26.101386 astrotitles-0.1.5/astrotitles/
--rw-r--r--   0 ben        (501) staff       (20)        0 2023-07-19 22:07:36.000000 astrotitles-0.1.5/astrotitles/__init__.py
--rw-r--r--   0 ben        (501) staff       (20)     1422 2023-07-21 19:22:26.000000 astrotitles-0.1.5/astrotitles/cli.py
--rw-r--r--   0 ben        (501) staff       (20)     2128 2023-07-21 19:29:40.000000 astrotitles-0.1.5/astrotitles/transcriber.py
--rw-r--r--   0 ben        (501) staff       (20)     1145 2023-07-21 19:29:06.000000 astrotitles-0.1.5/astrotitles/utils.py
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-07-21 19:35:26.102374 astrotitles-0.1.5/astrotitles.egg-info/
--rw-r--r--   0 ben        (501) staff       (20)     4701 2023-07-21 19:35:26.000000 astrotitles-0.1.5/astrotitles.egg-info/PKG-INFO
--rw-r--r--   0 ben        (501) staff       (20)      343 2023-07-21 19:35:26.000000 astrotitles-0.1.5/astrotitles.egg-info/SOURCES.txt
--rw-r--r--   0 ben        (501) staff       (20)        1 2023-07-21 19:35:26.000000 astrotitles-0.1.5/astrotitles.egg-info/dependency_links.txt
--rw-r--r--   0 ben        (501) staff       (20)       52 2023-07-21 19:35:26.000000 astrotitles-0.1.5/astrotitles.egg-info/entry_points.txt
--rw-r--r--   0 ben        (501) staff       (20)       20 2023-07-21 19:35:26.000000 astrotitles-0.1.5/astrotitles.egg-info/requires.txt
--rw-r--r--   0 ben        (501) staff       (20)       12 2023-07-21 19:35:26.000000 astrotitles-0.1.5/astrotitles.egg-info/top_level.txt
--rw-r--r--   0 ben        (501) staff       (20)       79 2023-07-21 19:35:26.102813 astrotitles-0.1.5/setup.cfg
--rw-r--r--   0 ben        (501) staff       (20)      765 2023-07-21 19:31:31.000000 astrotitles-0.1.5/setup.py
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-07-21 21:33:16.140975 astrotitles-0.1.6/
+-rw-r--r--   0 ben        (501) staff       (20)    34523 2023-07-19 22:08:12.000000 astrotitles-0.1.6/LICENCE.txt
+-rw-r--r--   0 ben        (501) staff       (20)     4701 2023-07-21 21:33:16.141047 astrotitles-0.1.6/PKG-INFO
+-rw-r--r--   0 ben        (501) staff       (20)     4324 2023-07-21 19:22:36.000000 astrotitles-0.1.6/README.md
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-07-21 21:33:16.139856 astrotitles-0.1.6/astrotitles/
+-rw-r--r--   0 ben        (501) staff       (20)        0 2023-07-19 22:07:36.000000 astrotitles-0.1.6/astrotitles/__init__.py
+-rw-r--r--   0 ben        (501) staff       (20)     1422 2023-07-21 21:32:25.000000 astrotitles-0.1.6/astrotitles/cli.py
+-rw-r--r--   0 ben        (501) staff       (20)     2128 2023-07-21 19:29:40.000000 astrotitles-0.1.6/astrotitles/transcriber.py
+-rw-r--r--   0 ben        (501) staff       (20)     1145 2023-07-21 19:29:06.000000 astrotitles-0.1.6/astrotitles/utils.py
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-07-21 21:33:16.140858 astrotitles-0.1.6/astrotitles.egg-info/
+-rw-r--r--   0 ben        (501) staff       (20)     4701 2023-07-21 21:33:16.000000 astrotitles-0.1.6/astrotitles.egg-info/PKG-INFO
+-rw-r--r--   0 ben        (501) staff       (20)      343 2023-07-21 21:33:16.000000 astrotitles-0.1.6/astrotitles.egg-info/SOURCES.txt
+-rw-r--r--   0 ben        (501) staff       (20)        1 2023-07-21 21:33:16.000000 astrotitles-0.1.6/astrotitles.egg-info/dependency_links.txt
+-rw-r--r--   0 ben        (501) staff       (20)       52 2023-07-21 21:33:16.000000 astrotitles-0.1.6/astrotitles.egg-info/entry_points.txt
+-rw-r--r--   0 ben        (501) staff       (20)       20 2023-07-21 21:33:16.000000 astrotitles-0.1.6/astrotitles.egg-info/requires.txt
+-rw-r--r--   0 ben        (501) staff       (20)       12 2023-07-21 21:33:16.000000 astrotitles-0.1.6/astrotitles.egg-info/top_level.txt
+-rw-r--r--   0 ben        (501) staff       (20)       79 2023-07-21 21:33:16.141269 astrotitles-0.1.6/setup.cfg
+-rw-r--r--   0 ben        (501) staff       (20)      765 2023-07-21 21:33:09.000000 astrotitles-0.1.6/setup.py
```

### Comparing `astrotitles-0.1.5/LICENCE.txt` & `astrotitles-0.1.6/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `astrotitles-0.1.5/PKG-INFO` & `astrotitles-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astrotitles
-Version: 0.1.5
+Version: 0.1.6
 Summary: Automatically generate subtitles using the Astrotitles command line interface.
 Home-page: https://github.com/Astrotitles/cli
 Download-URL: https://github.com/Astrotitles/cli.git
 Author: Ben Webster
 License: AGPL-3.0
 Keywords: AI,Whisper AI,Subtitles
 Description-Content-Type: markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: astrotitles Version: 0.1.5 Summary: Automatically
+Metadata-Version: 2.1 Name: astrotitles Version: 0.1.6 Summary: Automatically
 generate subtitles using the Astrotitles command line interface. Home-page:
 https://github.com/Astrotitles/cli Download-URL: https://github.com/
 Astrotitles/cli.git Author: Ben Webster License: AGPL-3.0 Keywords: AI,Whisper
 AI,Subtitles Description-Content-Type: markdown License-File: LICENCE.txt  [!
 [Contributors][contributors-shield]][contributors-url] [![Forks][forks-shield]]
 [forks-url] [![Stargazers][stars-shield]][stars-url] [![Issues][issues-shield]]
 [issues-url] [![MIT License][license-shield]][license-url]
```

### Comparing `astrotitles-0.1.5/README.md` & `astrotitles-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `astrotitles-0.1.5/astrotitles/cli.py` & `astrotitles-0.1.6/astrotitles/cli.py`

 * *Files identical despite different names*

### Comparing `astrotitles-0.1.5/astrotitles/transcriber.py` & `astrotitles-0.1.6/astrotitles/transcriber.py`

 * *Files identical despite different names*

### Comparing `astrotitles-0.1.5/astrotitles/utils.py` & `astrotitles-0.1.6/astrotitles/utils.py`

 * *Files identical despite different names*

### Comparing `astrotitles-0.1.5/astrotitles.egg-info/PKG-INFO` & `astrotitles-0.1.6/astrotitles.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astrotitles
-Version: 0.1.5
+Version: 0.1.6
 Summary: Automatically generate subtitles using the Astrotitles command line interface.
 Home-page: https://github.com/Astrotitles/cli
 Download-URL: https://github.com/Astrotitles/cli.git
 Author: Ben Webster
 License: AGPL-3.0
 Keywords: AI,Whisper AI,Subtitles
 Description-Content-Type: markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: astrotitles Version: 0.1.5 Summary: Automatically
+Metadata-Version: 2.1 Name: astrotitles Version: 0.1.6 Summary: Automatically
 generate subtitles using the Astrotitles command line interface. Home-page:
 https://github.com/Astrotitles/cli Download-URL: https://github.com/
 Astrotitles/cli.git Author: Ben Webster License: AGPL-3.0 Keywords: AI,Whisper
 AI,Subtitles Description-Content-Type: markdown License-File: LICENCE.txt  [!
 [Contributors][contributors-shield]][contributors-url] [![Forks][forks-shield]]
 [forks-url] [![Stargazers][stars-shield]][stars-url] [![Issues][issues-shield]]
 [issues-url] [![MIT License][license-shield]][license-url]
```

### Comparing `astrotitles-0.1.5/setup.py` & `astrotitles-0.1.6/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
-    version="0.1.5",
+    version="0.1.6",
     name="astrotitles",
     packages=find_packages(),
     license="AGPL-3.0",
     author="Ben Webster",
     url="https://github.com/Astrotitles/cli",
     download_url="https://github.com/Astrotitles/cli.git",
     keywords=["AI", "Whisper AI", "Subtitles"],
```

