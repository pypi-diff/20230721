# Comparing `tmp/motti-0.0.8.tar.gz` & `tmp/motti-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "motti-0.0.8.tar", last modified: Mon Jul 17 16:38:49 2023, max compression
+gzip compressed data, was "motti-0.0.9.tar", last modified: Thu Jul 20 14:59:27 2023, max compression
```

## Comparing `motti-0.0.8.tar` & `motti-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 16:38:49.230278 motti-0.0.8/
--rw-rw-rw-   0        0        0      135 2023-07-17 16:38:49.229276 motti-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      392 2023-07-17 14:13:01.000000 motti-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-07-17 16:38:49.221277 motti-0.0.8/motti/
--rw-rw-rw-   0        0        0      184 2023-07-17 16:38:11.000000 motti-0.0.8/motti/__init__.py
--rw-rw-rw-   0        0        0      203 2023-07-17 07:18:42.000000 motti-0.0.8/motti/dev.py
--rw-rw-rw-   0        0        0     1625 2023-07-17 16:37:20.000000 motti-0.0.8/motti/tools.py
-drwxrwxrwx   0        0        0        0 2023-07-17 16:38:49.227284 motti-0.0.8/motti.egg-info/
--rw-rw-rw-   0        0        0      135 2023-07-17 16:38:49.000000 motti-0.0.8/motti.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      208 2023-07-17 16:38:49.000000 motti-0.0.8/motti.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 16:38:49.000000 motti-0.0.8/motti.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-17 16:38:49.000000 motti-0.0.8/motti.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        6 2023-07-17 16:38:49.000000 motti-0.0.8/motti.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-17 16:38:49.230278 motti-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      261 2023-07-17 16:38:37.000000 motti-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-20 14:59:27.220445 motti-0.0.9/
+-rw-rw-rw-   0        0        0      135 2023-07-20 14:59:27.219456 motti-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      392 2023-07-17 14:13:01.000000 motti-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-07-20 14:59:27.211450 motti-0.0.9/motti/
+-rw-rw-rw-   0        0        0      219 2023-07-20 05:31:08.000000 motti-0.0.9/motti/__init__.py
+-rw-rw-rw-   0        0        0      203 2023-07-17 07:18:42.000000 motti-0.0.9/motti/dev.py
+-rw-rw-rw-   0        0        0     2389 2023-07-20 05:29:57.000000 motti-0.0.9/motti/tools.py
+drwxrwxrwx   0        0        0        0 2023-07-20 14:59:27.218450 motti-0.0.9/motti.egg-info/
+-rw-rw-rw-   0        0        0      135 2023-07-20 14:59:27.000000 motti-0.0.9/motti.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      208 2023-07-20 14:59:27.000000 motti-0.0.9/motti.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-20 14:59:27.000000 motti-0.0.9/motti.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-20 14:59:27.000000 motti-0.0.9/motti.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        6 2023-07-20 14:59:27.000000 motti-0.0.9/motti.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-20 14:59:27.220445 motti-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      261 2023-07-20 05:30:46.000000 motti-0.0.9/setup.py
```

