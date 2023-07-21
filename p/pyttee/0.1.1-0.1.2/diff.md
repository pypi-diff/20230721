# Comparing `tmp/pyttee-0.1.1.tar.gz` & `tmp/pyttee-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyttee-0.1.1.tar", max compression
+gzip compressed data, was "pyttee-0.1.2.tar", max compression
```

## Comparing `pyttee-0.1.1.tar` & `pyttee-0.1.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1079 2023-07-18 05:59:40.501062 pyttee-0.1.1/LICENSE.txt
--rw-r--r--   0        0        0        0 2023-07-17 05:46:32.429967 pyttee-0.1.1/README.md
--rw-r--r--   0        0        0      458 2023-07-20 06:20:10.655621 pyttee-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       31 2023-07-16 06:24:34.942795 pyttee-0.1.1/pyttee/__init__.py
--rw-r--r--   0        0        0     1473 2023-07-16 06:23:22.579967 pyttee-0.1.1/pyttee/builder.py
--rw-r--r--   0        0        0      507 2023-07-18 05:33:02.523911 pyttee-0.1.1/pyttee/compiler.py
--rw-r--r--   0        0        0      230 2023-07-18 05:33:02.503911 pyttee-0.1.1/pyttee/core.py
--rw-r--r--   0        0        0      217 2023-07-18 04:53:36.202463 pyttee-0.1.1/pyttee/models.py
--rw-r--r--   0        0        0     1324 2023-07-18 05:29:58.471630 pyttee-0.1.1/pyttee/parser.py
--rw-r--r--   0        0        0      443 1970-01-01 00:00:00.000000 pyttee-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1079 2023-07-18 05:59:40.501062 pyttee-0.1.2/LICENSE.txt
+-rw-r--r--   0        0        0        0 2023-07-17 05:46:32.429967 pyttee-0.1.2/README.md
+-rw-r--r--   0        0        0      459 2023-07-21 06:18:16.587404 pyttee-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       31 2023-07-16 06:24:34.942795 pyttee-0.1.2/pyttee/__init__.py
+-rw-r--r--   0        0        0     1473 2023-07-16 06:23:22.579967 pyttee-0.1.2/pyttee/builder.py
+-rw-r--r--   0        0        0      507 2023-07-18 05:33:02.523911 pyttee-0.1.2/pyttee/compiler.py
+-rw-r--r--   0        0        0      230 2023-07-18 05:33:02.503911 pyttee-0.1.2/pyttee/core.py
+-rw-r--r--   0        0        0      217 2023-07-18 04:53:36.202463 pyttee-0.1.2/pyttee/models.py
+-rw-r--r--   0        0        0     1324 2023-07-18 05:29:58.471630 pyttee-0.1.2/pyttee/parser.py
+-rw-r--r--   0        0        0      495 1970-01-01 00:00:00.000000 pyttee-0.1.2/PKG-INFO
```

### Comparing `pyttee-0.1.1/LICENSE.txt` & `pyttee-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyttee-0.1.1/pyttee/builder.py` & `pyttee-0.1.2/pyttee/builder.py`

 * *Files identical despite different names*

### Comparing `pyttee-0.1.1/pyttee/parser.py` & `pyttee-0.1.2/pyttee/parser.py`

 * *Files identical despite different names*

