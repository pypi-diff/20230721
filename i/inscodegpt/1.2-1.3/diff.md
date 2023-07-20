# Comparing `tmp/inscodegpt-1.2.tar.gz` & `tmp/inscodegpt-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inscodegpt-1.2.tar", last modified: Thu Jul 20 15:00:38 2023, max compression
+gzip compressed data, was "inscodegpt-1.3.tar", last modified: Thu Jul 20 22:24:08 2023, max compression
```

## Comparing `inscodegpt-1.2.tar` & `inscodegpt-1.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 15:00:38.602983 inscodegpt-1.2/
--rw-r--r--   0 root         (0) root         (0)      212 2023-07-20 15:00:38.602983 inscodegpt-1.2/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 15:00:38.601983 inscodegpt-1.2/inscodegpt/
--rw-r--r--   0 root         (0) root         (0)       27 2023-07-20 14:59:24.000000 inscodegpt-1.2/inscodegpt/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1186 2023-07-20 14:34:21.000000 inscodegpt-1.2/inscodegpt/inscode_gpt.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 15:00:38.602983 inscodegpt-1.2/inscodegpt.egg-info/
--rw-r--r--   0 root         (0) root         (0)      212 2023-07-20 15:00:38.000000 inscodegpt-1.2/inscodegpt.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      226 2023-07-20 15:00:38.000000 inscodegpt-1.2/inscodegpt.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 15:00:38.000000 inscodegpt-1.2/inscodegpt.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-07-20 15:00:38.000000 inscodegpt-1.2/inscodegpt.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-07-20 15:00:38.000000 inscodegpt-1.2/inscodegpt.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-20 15:00:38.602983 inscodegpt-1.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      269 2023-07-20 15:00:35.000000 inscodegpt-1.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:24:08.546293 inscodegpt-1.3/
+-rw-r--r--   0 root         (0) root         (0)      212 2023-07-20 22:24:08.546293 inscodegpt-1.3/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:24:08.545293 inscodegpt-1.3/inscodegpt/
+-rw-r--r--   0 root         (0) root         (0)       27 2023-07-20 14:59:24.000000 inscodegpt-1.3/inscodegpt/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1196 2023-07-20 22:22:36.000000 inscodegpt-1.3/inscodegpt/inscode_gpt.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:24:08.546293 inscodegpt-1.3/inscodegpt.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      212 2023-07-20 22:24:08.000000 inscodegpt-1.3/inscodegpt.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      226 2023-07-20 22:24:08.000000 inscodegpt-1.3/inscodegpt.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 22:24:08.000000 inscodegpt-1.3/inscodegpt.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-07-20 22:24:08.000000 inscodegpt-1.3/inscodegpt.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-07-20 22:24:08.000000 inscodegpt-1.3/inscodegpt.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-20 22:24:08.546293 inscodegpt-1.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      269 2023-07-20 22:23:05.000000 inscodegpt-1.3/setup.py
```

### Comparing `inscodegpt-1.2/inscodegpt/inscode_gpt.py` & `inscodegpt-1.3/inscodegpt/inscode_gpt.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 
 API_URL = "https://inscode-api.csdn.net/api/v1/gpt/"
 INSCODE_API_KEY = os.getenv("INSCODE_API_KEY")
 
 def send_question(prompt,question):
   body = {
       "messages": [{"role": "user", "content": prompt+question}],
```

