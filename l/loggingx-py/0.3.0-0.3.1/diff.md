# Comparing `tmp/loggingx-py-0.3.0.tar.gz` & `tmp/loggingx-py-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loggingx-py-0.3.0.tar", last modified: Fri Jul 21 10:34:32 2023, max compression
+gzip compressed data, was "loggingx-py-0.3.1.tar", last modified: Fri Jul 21 10:54:01 2023, max compression
```

## Comparing `loggingx-py-0.3.0.tar` & `loggingx-py-0.3.1.tar`

### file list

```diff
@@ -1,21 +1,24 @@
-drwxr-xr-x   0 hhk7734   (1000) hhk7734   (1000)        0 2023-07-21 10:34:32.997778 loggingx-py-0.3.0/
--rw-r--r--   0 hhk7734   (1000) hhk7734   (1000)     4662 2023-07-21 09:47:39.000000 loggingx-py-0.3.0/.gitignore
--rw-r--r--   0 hhk7734   (1000) hhk7734   (1000)       15 2023-07-21 09:47:39.000000 loggingx-py-0.3.0/.tool-versions
--rw-r--r--   0 hhk7734   (1000) hhk7734   (1000)     1088 2023-07-21 09:47:39.000000 loggingx-py-0.3.0/LICENSE
--rw-r--r--   0 hhk7734   (1000) hhk7734   (1000)      180 2023-07-21 09:47:39.000000 loggingx-py-0.3.0/Makefile
--rw-r--r--   0 hhk7734   (1000) hhk7734   (1000)     3873 2023-07-21 10:34:32.997778 loggingx-py-0.3.0/PKG-INFO
--rw-r--r--   0 hhk7734   (1000) hhk7734   (1000)     2131 2023-07-21 10:33:40.000000 loggingx-py-0.3.0/README.md
-drwxr-xr-x   0 hhk7734   (1000) hhk7734   (1000)        0 2023-07-21 10:34:32.994445 loggingx-py-0.3.0/loggingx/
--rw-r--r--   0 hhk7734   (1000) hhk7734   (1000)      336 2023-07-21 10:32:05.000000 loggingx-py-0.3.0/loggingx/__init__.py
--rw-r--r--   0 hhk7734   (1000) hhk7734   (1000)       87 2023-07-21 09:47:39.000000 loggingx-py-0.3.0/loggingx/config.py
--rw-r--r--   0 hhk7734   (1000) hhk7734   (1000)     1443 2023-07-21 09:47:39.000000 loggingx-py-0.3.0/loggingx/context.py
--rw-r--r--   0 hhk7734   (1000) hhk7734   (1000)     1536 2023-07-21 09:47:39.000000 loggingx-py-0.3.0/loggingx/formatter.py
--rw-r--r--   0 hhk7734   (1000) hhk7734   (1000)       89 2023-07-21 09:47:39.000000 loggingx-py-0.3.0/loggingx/handlers.py
-drwxr-xr-x   0 hhk7734   (1000) hhk7734   (1000)        0 2023-07-21 10:34:32.997778 loggingx-py-0.3.0/loggingx_py.egg-info/
--rw-r--r--   0 hhk7734   (1000) hhk7734   (1000)     3873 2023-07-21 10:34:32.000000 loggingx-py-0.3.0/loggingx_py.egg-info/PKG-INFO
--rw-r--r--   0 hhk7734   (1000) hhk7734   (1000)      322 2023-07-21 10:34:32.000000 loggingx-py-0.3.0/loggingx_py.egg-info/SOURCES.txt
--rw-r--r--   0 hhk7734   (1000) hhk7734   (1000)        1 2023-07-21 10:34:32.000000 loggingx-py-0.3.0/loggingx_py.egg-info/dependency_links.txt
--rw-r--r--   0 hhk7734   (1000) hhk7734   (1000)        9 2023-07-21 10:34:32.000000 loggingx-py-0.3.0/loggingx_py.egg-info/top_level.txt
--rw-r--r--   0 hhk7734   (1000) hhk7734   (1000)    32864 2023-07-21 09:47:39.000000 loggingx-py-0.3.0/poetry.lock
--rw-r--r--   0 hhk7734   (1000) hhk7734   (1000)    22589 2023-07-21 10:29:09.000000 loggingx-py-0.3.0/pyproject.toml
--rw-r--r--   0 hhk7734   (1000) hhk7734   (1000)       38 2023-07-21 10:34:32.997778 loggingx-py-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:54:01.602028 loggingx-py-0.3.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:54:01.598028 loggingx-py-0.3.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:54:01.598028 loggingx-py-0.3.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-21 10:53:42.000000 loggingx-py-0.3.1/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4662 2023-07-21 10:53:42.000000 loggingx-py-0.3.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-21 10:53:42.000000 loggingx-py-0.3.1/.tool-versions
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-21 10:53:42.000000 loggingx-py-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-21 10:53:42.000000 loggingx-py-0.3.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-07-21 10:54:01.602028 loggingx-py-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-07-21 10:53:42.000000 loggingx-py-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:54:01.602028 loggingx-py-0.3.1/loggingx/
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-21 10:53:42.000000 loggingx-py-0.3.1/loggingx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-21 10:53:42.000000 loggingx-py-0.3.1/loggingx/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-07-21 10:53:42.000000 loggingx-py-0.3.1/loggingx/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-07-21 10:53:42.000000 loggingx-py-0.3.1/loggingx/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-21 10:53:42.000000 loggingx-py-0.3.1/loggingx/handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:54:01.602028 loggingx-py-0.3.1/loggingx_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-07-21 10:54:01.000000 loggingx-py-0.3.1/loggingx_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-21 10:54:01.000000 loggingx-py-0.3.1/loggingx_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 10:54:01.000000 loggingx-py-0.3.1/loggingx_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-21 10:54:01.000000 loggingx-py-0.3.1/loggingx_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    78091 2023-07-21 10:53:42.000000 loggingx-py-0.3.1/poetry.lock
+-rw-r--r--   0 runner    (1001) docker     (123)    22624 2023-07-21 10:53:42.000000 loggingx-py-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 10:54:01.602028 loggingx-py-0.3.1/setup.cfg
```

### Comparing `loggingx-py-0.3.0/.gitignore` & `loggingx-py-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `loggingx-py-0.3.0/LICENSE` & `loggingx-py-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `loggingx-py-0.3.0/PKG-INFO` & `loggingx-py-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loggingx-py
-Version: 0.3.0
+Version: 0.3.1
 Summary: Helper for Contextual and Structured Logging in Python with logging
 Author-email: Hyeonki Hong <hhk7734@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Hyeonki Hong <hhk7734@gmail.com>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `loggingx-py-0.3.0/README.md` & `loggingx-py-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `loggingx-py-0.3.0/loggingx/context.py` & `loggingx-py-0.3.1/loggingx/context.py`

 * *Files identical despite different names*

### Comparing `loggingx-py-0.3.0/loggingx/formatter.py` & `loggingx-py-0.3.1/loggingx/formatter.py`

 * *Files identical despite different names*

### Comparing `loggingx-py-0.3.0/loggingx_py.egg-info/PKG-INFO` & `loggingx-py-0.3.1/loggingx_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loggingx-py
-Version: 0.3.0
+Version: 0.3.1
 Summary: Helper for Contextual and Structured Logging in Python with logging
 Author-email: Hyeonki Hong <hhk7734@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Hyeonki Hong <hhk7734@gmail.com>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `loggingx-py-0.3.0/pyproject.toml` & `loggingx-py-0.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -36,14 +36,16 @@
 python = ">=3.10,<4.0"
 
 [tool.poetry.group.dev.dependencies]
 mypy = "^1.4.1"
 black = "^23.7.0"
 isort = "^5.12.0"
 pylint = "^2.17.4"
+build = "^0.10.0"
+twine = "^4.0.2"
 
 [tool.black]
 exclude = '''
 /(
     \.eggs
   | \.git
   | \.hg
```

