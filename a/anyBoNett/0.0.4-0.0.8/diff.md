# Comparing `tmp/anyBoNett-0.0.4.tar.gz` & `tmp/anyBoNett-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anyBoNett-0.0.4.tar", last modified: Thu Jul 20 07:33:27 2023, max compression
+gzip compressed data, was "anyBoNett-0.0.8.tar", last modified: Thu Jul 20 22:16:18 2023, max compression
```

## Comparing `anyBoNett-0.0.4.tar` & `anyBoNett-0.0.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-20 07:33:26.459054 anyBoNett-0.0.4/
--rw-rw-rw-   0        0        0     1094 2023-07-20 01:37:41.000000 anyBoNett-0.0.4/LICENSE
--rw-rw-rw-   0        0        0     1023 2023-07-20 07:33:26.457914 anyBoNett-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      744 2023-07-20 07:31:17.000000 anyBoNett-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-07-20 07:33:26.444865 anyBoNett-0.0.4/anyBoNett.egg-info/
--rw-rw-rw-   0        0        0     1023 2023-07-20 07:33:23.000000 anyBoNett-0.0.4/anyBoNett.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      207 2023-07-20 07:33:24.000000 anyBoNett-0.0.4/anyBoNett.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-20 07:33:23.000000 anyBoNett-0.0.4/anyBoNett.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-07-20 07:33:23.000000 anyBoNett-0.0.4/anyBoNett.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-20 07:33:24.000000 anyBoNett-0.0.4/anyBoNett.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-20 07:33:26.455369 anyBoNett-0.0.4/anybonett/
--rw-rw-rw-   0        0        0      724 2023-07-20 06:31:01.000000 anyBoNett-0.0.4/anybonett/NET.py
--rw-rw-rw-   0        0        0       42 2023-07-20 07:33:26.459054 anyBoNett-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      464 2023-07-20 07:31:57.000000 anyBoNett-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-20 22:16:18.125024 anyBoNett-0.0.8/
+-rw-rw-rw-   0        0        0     1094 2023-07-20 01:37:41.000000 anyBoNett-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0     3817 2023-07-20 22:16:18.122403 anyBoNett-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     3531 2023-07-20 22:10:51.000000 anyBoNett-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-07-20 22:16:18.118491 anyBoNett-0.0.8/anyBoNett.egg-info/
+-rw-rw-rw-   0        0        0     3817 2023-07-20 22:16:17.000000 anyBoNett-0.0.8/anyBoNett.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      207 2023-07-20 22:16:17.000000 anyBoNett-0.0.8/anyBoNett.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-20 22:16:17.000000 anyBoNett-0.0.8/anyBoNett.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-07-20 22:16:17.000000 anyBoNett-0.0.8/anyBoNett.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-20 22:16:17.000000 anyBoNett-0.0.8/anyBoNett.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-20 22:16:18.121039 anyBoNett-0.0.8/anybonett/
+-rw-rw-rw-   0        0        0     3132 2023-07-20 22:12:01.000000 anyBoNett-0.0.8/anybonett/NET.py
+-rw-rw-rw-   0        0        0       42 2023-07-20 22:16:18.125024 anyBoNett-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      493 2023-07-20 22:15:52.000000 anyBoNett-0.0.8/setup.py
```

### Comparing `anyBoNett-0.0.4/LICENSE` & `anyBoNett-0.0.8/LICENSE`

 * *Files identical despite different names*

