# Comparing `tmp/shakecore-0.0.1.tar.gz` & `tmp/shakecore-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shakecore-0.0.1.tar", max compression
+gzip compressed data, was "shakecore-0.0.2.tar", max compression
```

## Comparing `shakecore-0.0.1.tar` & `shakecore-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,10 @@
--rw-r--r--   0        0        0    11357 2023-07-18 00:22:28.506824 shakecore-0.0.1/LICENSE
--rw-r--r--   0        0        0      683 2023-07-18 00:22:58.380289 shakecore-0.0.1/README.md
--rw-r--r--   0        0        0     1542 2023-07-21 07:37:07.483200 shakecore-0.0.1/pyproject.toml
--rw-r--r--   0        0        0       82 2023-07-18 04:21:08.439210 shakecore-0.0.1/shakecore/__init__.py
--rw-r--r--   0        0        0        0 2023-07-18 00:22:28.467548 shakecore-0.0.1/shakecore/config/__init__.py
--rw-r--r--   0        0        0      145 2023-07-18 00:22:28.467905 shakecore-0.0.1/shakecore/config/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      561 2023-07-18 00:22:28.468242 shakecore-0.0.1/shakecore/config/__pycache__/mwcs.cpython-310.pyc
--rw-r--r--   0        0        0      359 2023-07-18 00:22:28.468582 shakecore-0.0.1/shakecore/config/main.py
--rw-r--r--   0        0        0        0 2023-07-18 00:22:28.468988 shakecore-0.0.1/shakecore/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-07-18 00:22:28.469388 shakecore-0.0.1/shakecore/tests/test_config/__init__.py
--rw-r--r--   0        0        0      157 2023-07-18 00:22:28.469860 shakecore-0.0.1/shakecore/tests/test_config/test_main.py
--rw-r--r--   0        0        0     1602 1970-01-01 00:00:00.000000 shakecore-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-21 20:57:09.635405 shakecore-0.0.2/LICENSE
+-rw-r--r--   0        0        0      669 2023-07-21 20:57:09.635405 shakecore-0.0.2/README.md
+-rw-r--r--   0        0        0     1542 2023-07-21 20:57:09.639405 shakecore-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0       82 2023-07-21 20:57:09.639405 shakecore-0.0.2/shakecore/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-21 20:57:09.639405 shakecore-0.0.2/shakecore/config/__init__.py
+-rw-r--r--   0        0        0      359 2023-07-21 20:57:09.639405 shakecore-0.0.2/shakecore/config/main.py
+-rw-r--r--   0        0        0        0 2023-07-21 20:57:09.639405 shakecore-0.0.2/shakecore/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-21 20:57:09.639405 shakecore-0.0.2/shakecore/tests/test_config/__init__.py
+-rw-r--r--   0        0        0      157 2023-07-21 20:57:09.639405 shakecore-0.0.2/shakecore/tests/test_config/test_main.py
+-rw-r--r--   0        0        0     1588 1970-01-01 00:00:00.000000 shakecore-0.0.2/PKG-INFO
```

### Comparing `shakecore-0.0.1/LICENSE` & `shakecore-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `shakecore-0.0.1/pyproject.toml` & `shakecore-0.0.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shakecore"
-version = "0.0.1"
+version = "0.0.2"
 description = "Shake events locating and focal mechanism analysis"
 authors = ["OUCyf <oucyinfu@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 include = ["shakecore/**/*.py", "pyproject.toml"]
 classifiers = [
         "Development Status :: 2 - Pre-Alpha",
```

