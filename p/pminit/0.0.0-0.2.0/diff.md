# Comparing `tmp/pminit-0.0.0.tar.gz` & `tmp/pminit-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pminit-0.0.0.tar", max compression
+gzip compressed data, was "pminit-0.2.0.tar", max compression
```

## Comparing `pminit-0.0.0.tar` & `pminit-0.2.0.tar`

### file list

```diff
@@ -1,3 +1,7 @@
--rw-r--r--   0        0        0      265 2023-07-05 18:45:16.595831 pminit-0.0.0/pyproject.toml
--rw-r--r--   0        0        0       28 2023-04-12 14:27:45.000000 pminit-0.0.0/src/pminit/__init__.py
--rw-r--r--   0        0        0      667 1970-01-01 00:00:00.000000 pminit-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0       55 2023-07-20 15:39:35.976209 pminit-0.2.0/pminit/__init__.py
+-rw-r--r--   0        0        0     1176 2023-07-20 15:39:35.976209 pminit-0.2.0/pminit/cli.py
+-rw-r--r--   0        0        0      581 2023-07-20 15:39:35.976209 pminit-0.2.0/post-install-hook.py
+-rw-r--r--   0        0        0     1006 2023-07-21 14:47:57.864107 pminit-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0    17097 2023-07-20 15:39:35.976209 pminit-0.2.0/pythonmonkey/package-lock.json
+-rw-r--r--   0        0        0      653 2023-07-20 15:39:35.976209 pminit-0.2.0/pythonmonkey/package.json
+-rw-r--r--   0        0        0      431 1970-01-01 00:00:00.000000 pminit-0.2.0/PKG-INFO
```

