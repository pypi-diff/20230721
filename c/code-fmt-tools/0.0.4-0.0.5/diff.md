# Comparing `tmp/code_fmt_tools-0.0.4.tar.gz` & `tmp/code_fmt_tools-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "code_fmt_tools-0.0.4.tar", last modified: Fri Jul 21 08:34:07 2023, max compression
+gzip compressed data, was "code_fmt_tools-0.0.5.tar", last modified: Fri Jul 21 08:45:49 2023, max compression
```

## Comparing `code_fmt_tools-0.0.4.tar` & `code_fmt_tools-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 08:34:07.824633 code_fmt_tools-0.0.4/
--rw-r--r--   0 root         (0) root         (0)     1074 2023-07-12 08:42:56.000000 code_fmt_tools-0.0.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)      203 2023-07-21 08:34:07.824633 code_fmt_tools-0.0.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        5 2023-07-12 08:43:35.000000 code_fmt_tools-0.0.4/README.md
--rw-r--r--   0 root         (0) root         (0)      178 2023-07-21 08:33:40.000000 code_fmt_tools-0.0.4/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-21 08:34:07.824633 code_fmt_tools-0.0.4/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 08:34:07.824633 code_fmt_tools-0.0.4/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 08:34:07.824633 code_fmt_tools-0.0.4/src/codeUtils/
--rw-r--r--   0 root         (0) root         (0)     1416 2023-07-21 08:18:23.000000 code_fmt_tools-0.0.4/src/codeUtils/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 08:34:07.824633 code_fmt_tools-0.0.4/src/code_fmt_tools.egg-info/
--rw-r--r--   0 root         (0) root         (0)      203 2023-07-21 08:34:07.000000 code_fmt_tools-0.0.4/src/code_fmt_tools.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      245 2023-07-21 08:34:07.000000 code_fmt_tools-0.0.4/src/code_fmt_tools.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 08:34:07.000000 code_fmt_tools-0.0.4/src/code_fmt_tools.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-07-21 08:34:07.000000 code_fmt_tools-0.0.4/src/code_fmt_tools.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 08:34:07.824633 code_fmt_tools-0.0.4/tests/
--rw-r--r--   0 root         (0) root         (0)      225 2023-07-21 07:53:50.000000 code_fmt_tools-0.0.4/tests/test_code.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 08:45:49.709160 code_fmt_tools-0.0.5/
+-rw-r--r--   0 root         (0) root         (0)     1074 2023-07-12 08:42:56.000000 code_fmt_tools-0.0.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      203 2023-07-21 08:45:49.709160 code_fmt_tools-0.0.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        5 2023-07-12 08:43:35.000000 code_fmt_tools-0.0.5/README.md
+-rw-r--r--   0 root         (0) root         (0)      178 2023-07-21 08:44:02.000000 code_fmt_tools-0.0.5/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-21 08:45:49.709160 code_fmt_tools-0.0.5/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 08:45:49.709160 code_fmt_tools-0.0.5/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 08:45:49.709160 code_fmt_tools-0.0.5/src/code_fmt_tools/
+-rw-r--r--   0 root         (0) root         (0)     1416 2023-07-21 08:43:30.000000 code_fmt_tools-0.0.5/src/code_fmt_tools/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 08:45:49.709160 code_fmt_tools-0.0.5/src/code_fmt_tools.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      203 2023-07-21 08:45:49.000000 code_fmt_tools-0.0.5/src/code_fmt_tools.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      250 2023-07-21 08:45:49.000000 code_fmt_tools-0.0.5/src/code_fmt_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 08:45:49.000000 code_fmt_tools-0.0.5/src/code_fmt_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-07-21 08:45:49.000000 code_fmt_tools-0.0.5/src/code_fmt_tools.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 08:45:49.709160 code_fmt_tools-0.0.5/tests/
+-rw-r--r--   0 root         (0) root         (0)      225 2023-07-21 07:53:50.000000 code_fmt_tools-0.0.5/tests/test_code.py
```

### Comparing `code_fmt_tools-0.0.4/LICENSE` & `code_fmt_tools-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `code_fmt_tools-0.0.4/src/codeUtils/__init__.py` & `code_fmt_tools-0.0.5/src/code_fmt_tools/__init__.py`

 * *Files identical despite different names*

