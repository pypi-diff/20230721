# Comparing `tmp/loggingx_py-0.2.0.tar.gz` & `tmp/loggingx-py-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loggingx_py-0.2.0.tar", max compression
+gzip compressed data, was "loggingx-py-0.3.0.tar", last modified: Fri Jul 21 10:34:32 2023, max compression
```

## Comparing `loggingx_py-0.2.0.tar` & `loggingx-py-0.3.0.tar`

### file list

```diff
@@ -1,9 +1,21 @@
--rw-r--r--   0        0        0     1088 2023-07-16 13:01:36.288401 loggingx_py-0.2.0/LICENSE
--rw-r--r--   0        0        0     1410 2023-07-18 16:29:45.150010 loggingx_py-0.2.0/README.md
--rw-r--r--   0        0        0      193 2023-07-18 15:57:53.070839 loggingx_py-0.2.0/loggingx/__init__.py
--rw-r--r--   0        0        0       87 2023-07-18 15:56:41.604948 loggingx_py-0.2.0/loggingx/config.py
--rw-r--r--   0        0        0     1443 2023-07-18 15:46:41.041730 loggingx_py-0.2.0/loggingx/context.py
--rw-r--r--   0        0        0     1536 2023-07-18 16:25:28.592550 loggingx_py-0.2.0/loggingx/formatter.py
--rw-r--r--   0        0        0       89 2023-07-18 15:55:31.592435 loggingx_py-0.2.0/loggingx/handlers.py
--rw-r--r--   0        0        0    22278 2023-07-18 16:41:22.396620 loggingx_py-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2094 1970-01-01 00:00:00.000000 loggingx_py-0.2.0/PKG-INFO
+drwxr-xr-x   0 hhk7734   (1000) hhk7734   (1000)        0 2023-07-21 10:34:32.997778 loggingx-py-0.3.0/
+-rw-r--r--   0 hhk7734   (1000) hhk7734   (1000)     4662 2023-07-21 09:47:39.000000 loggingx-py-0.3.0/.gitignore
+-rw-r--r--   0 hhk7734   (1000) hhk7734   (1000)       15 2023-07-21 09:47:39.000000 loggingx-py-0.3.0/.tool-versions
+-rw-r--r--   0 hhk7734   (1000) hhk7734   (1000)     1088 2023-07-21 09:47:39.000000 loggingx-py-0.3.0/LICENSE
+-rw-r--r--   0 hhk7734   (1000) hhk7734   (1000)      180 2023-07-21 09:47:39.000000 loggingx-py-0.3.0/Makefile
+-rw-r--r--   0 hhk7734   (1000) hhk7734   (1000)     3873 2023-07-21 10:34:32.997778 loggingx-py-0.3.0/PKG-INFO
+-rw-r--r--   0 hhk7734   (1000) hhk7734   (1000)     2131 2023-07-21 10:33:40.000000 loggingx-py-0.3.0/README.md
+drwxr-xr-x   0 hhk7734   (1000) hhk7734   (1000)        0 2023-07-21 10:34:32.994445 loggingx-py-0.3.0/loggingx/
+-rw-r--r--   0 hhk7734   (1000) hhk7734   (1000)      336 2023-07-21 10:32:05.000000 loggingx-py-0.3.0/loggingx/__init__.py
+-rw-r--r--   0 hhk7734   (1000) hhk7734   (1000)       87 2023-07-21 09:47:39.000000 loggingx-py-0.3.0/loggingx/config.py
+-rw-r--r--   0 hhk7734   (1000) hhk7734   (1000)     1443 2023-07-21 09:47:39.000000 loggingx-py-0.3.0/loggingx/context.py
+-rw-r--r--   0 hhk7734   (1000) hhk7734   (1000)     1536 2023-07-21 09:47:39.000000 loggingx-py-0.3.0/loggingx/formatter.py
+-rw-r--r--   0 hhk7734   (1000) hhk7734   (1000)       89 2023-07-21 09:47:39.000000 loggingx-py-0.3.0/loggingx/handlers.py
+drwxr-xr-x   0 hhk7734   (1000) hhk7734   (1000)        0 2023-07-21 10:34:32.997778 loggingx-py-0.3.0/loggingx_py.egg-info/
+-rw-r--r--   0 hhk7734   (1000) hhk7734   (1000)     3873 2023-07-21 10:34:32.000000 loggingx-py-0.3.0/loggingx_py.egg-info/PKG-INFO
+-rw-r--r--   0 hhk7734   (1000) hhk7734   (1000)      322 2023-07-21 10:34:32.000000 loggingx-py-0.3.0/loggingx_py.egg-info/SOURCES.txt
+-rw-r--r--   0 hhk7734   (1000) hhk7734   (1000)        1 2023-07-21 10:34:32.000000 loggingx-py-0.3.0/loggingx_py.egg-info/dependency_links.txt
+-rw-r--r--   0 hhk7734   (1000) hhk7734   (1000)        9 2023-07-21 10:34:32.000000 loggingx-py-0.3.0/loggingx_py.egg-info/top_level.txt
+-rw-r--r--   0 hhk7734   (1000) hhk7734   (1000)    32864 2023-07-21 09:47:39.000000 loggingx-py-0.3.0/poetry.lock
+-rw-r--r--   0 hhk7734   (1000) hhk7734   (1000)    22589 2023-07-21 10:29:09.000000 loggingx-py-0.3.0/pyproject.toml
+-rw-r--r--   0 hhk7734   (1000) hhk7734   (1000)       38 2023-07-21 10:34:32.997778 loggingx-py-0.3.0/setup.cfg
```

### Comparing `loggingx_py-0.2.0/LICENSE` & `loggingx-py-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `loggingx_py-0.2.0/loggingx/context.py` & `loggingx-py-0.3.0/loggingx/context.py`

 * *Files identical despite different names*

### Comparing `loggingx_py-0.2.0/loggingx/formatter.py` & `loggingx-py-0.3.0/loggingx/formatter.py`

 * *Files identical despite different names*

### Comparing `loggingx_py-0.2.0/pyproject.toml` & `loggingx-py-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,50 @@
-[tool.poetry]
+[project]
 name = "loggingx-py"
-version = "0.2.0"
 description = "Helper for Contextual and Structured Logging in Python with logging"
-authors = ["Hyeonki Hong <hhk7734@gmail.com>"]
-packages = [{ include = "loggingx" }]
-license = "MIT"
+authors = [{ name = "Hyeonki Hong", email = "hhk7734@gmail.com" }]
+requires-python = ">=3.10,<4.0"
+
+dynamic = ["version"]
+
+license = { file = "LICENSE" }
 readme = "README.md"
-repository = "https://github.com/hhk7734/loggingx.py"
 keywords = ["logging", "contextual-logging", "structured-logging"]
-classifiers = ["Intended Audience :: Developers"]
+classifiers = [
+    "Programming Language :: Python :: 3",
+    "Intended Audience :: Developers",
+]
+
+[project.urls]
+repository = "https://github.com/hhk7734/loggingx.py"
+
+[build-system]
+requires = ["setuptools", "setuptools-scm"]
+build-backend = "setuptools.build_meta"
+
+[tool.setuptools_scm]
+
+[tool.setuptools.packages.find]
+include = ["loggingx"]
+
+[tool.poetry]
+name = "loggingx-py"
+version = "0"
+description = ""
+authors = ["Hyeonki Hong <hhk7734@gmail.com>"]
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = ">=3.10,<4.0"
 
 [tool.poetry.group.dev.dependencies]
 mypy = "^1.4.1"
 black = "^23.7.0"
 isort = "^5.12.0"
 pylint = "^2.17.4"
 
-[build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
-
 [tool.black]
 exclude = '''
 /(
     \.eggs
   | \.git
   | \.hg
   | \.mypy_cache
```

