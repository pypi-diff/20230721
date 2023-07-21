# Comparing `tmp/pyfarmer-1.0.1.tar.gz` & `tmp/pyfarmer-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfarmer-1.0.1.tar", max compression
+gzip compressed data, was "pyfarmer-2.0.0.tar", max compression
```

## Comparing `pyfarmer-1.0.1.tar` & `pyfarmer-2.0.0.tar`

### file list

```diff
@@ -1,7 +1,9 @@
--rw-r--r--   0        0        0      259 2023-06-01 18:16:39.024165 pyfarmer-1.0.1/pyfarmer/__init__.py
--rwxr-xr-x   0        0        0    19480 2023-06-01 18:16:39.024165 pyfarmer-1.0.1/pyfarmer/_client.py
--rw-r--r--   0        0        0     4301 2023-06-01 18:16:39.024165 pyfarmer-1.0.1/pyfarmer/_pyfarmer.py
--rw-r--r--   0        0        0      147 2023-06-01 18:16:39.024165 pyfarmer-1.0.1/pyfarmer/_tmp.py
--rw-r--r--   0        0        0        0 2023-06-01 18:16:39.024165 pyfarmer-1.0.1/pyfarmer/py.typed
--rw-r--r--   0        0        0      688 2023-06-01 18:16:39.024165 pyfarmer-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      460 1970-01-01 00:00:00.000000 pyfarmer-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-21 17:28:55.592844 pyfarmer-2.0.0/LICENSE
+-rw-r--r--   0        0        0      877 2023-07-21 17:28:55.592844 pyfarmer-2.0.0/README.md
+-rw-r--r--   0        0        0     1535 2023-07-21 17:28:55.592844 pyfarmer-2.0.0/pyfarmer/__init__.py
+-rw-r--r--   0        0        0    15637 2023-07-21 17:28:55.592844 pyfarmer-2.0.0/pyfarmer/_pyfarmer.py
+-rw-r--r--   0        0        0     7542 2023-07-21 17:28:55.592844 pyfarmer-2.0.0/pyfarmer/_strategies.py
+-rw-r--r--   0        0        0     1782 2023-07-21 17:28:55.592844 pyfarmer-2.0.0/pyfarmer/_utils.py
+-rw-r--r--   0        0        0        0 2023-07-21 17:28:55.592844 pyfarmer-2.0.0/pyfarmer/py.typed
+-rw-r--r--   0        0        0     1307 2023-07-21 17:28:55.592844 pyfarmer-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1966 1970-01-01 00:00:00.000000 pyfarmer-2.0.0/PKG-INFO
```

