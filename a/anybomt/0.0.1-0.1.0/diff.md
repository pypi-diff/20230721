# Comparing `tmp/anybomt-0.0.1.tar.gz` & `tmp/anybomt-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anybomt-0.0.1.tar", last modified: Fri Jul 21 08:31:10 2023, max compression
+gzip compressed data, was "anybomt-0.1.0.tar", last modified: Fri Jul 21 21:17:20 2023, max compression
```

## Comparing `anybomt-0.0.1.tar` & `anybomt-0.1.0.tar`

### file list

```diff
@@ -1,13 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-07-21 08:31:10.579538 anybomt-0.0.1/
--rw-rw-rw-   0        0        0     1092 2023-07-21 08:26:10.000000 anybomt-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     3735 2023-07-21 08:31:10.577529 anybomt-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     3255 2023-07-21 08:20:12.000000 anybomt-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-21 08:31:10.572438 anybomt-0.0.1/anybomt.egg-info/
--rw-rw-rw-   0        0        0     3735 2023-07-21 08:31:10.000000 anybomt-0.0.1/anybomt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      191 2023-07-21 08:31:10.000000 anybomt-0.0.1/anybomt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 08:31:10.000000 anybomt-0.0.1/anybomt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-21 08:31:10.000000 anybomt-0.0.1/anybomt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 08:31:10.000000 anybomt-0.0.1/anybomt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    22814 2023-07-21 08:24:45.000000 anybomt-0.0.1/anybomt.py
--rw-rw-rw-   0        0        0       42 2023-07-21 08:31:10.581737 anybomt-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      502 2023-07-21 08:30:28.000000 anybomt-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 21:17:20.525362 anybomt-0.1.0/
+-rw-rw-rw-   0        0        0     1092 2023-07-21 08:26:10.000000 anybomt-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0    24402 2023-07-21 21:17:20.523932 anybomt-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0    23973 2023-07-21 21:15:13.000000 anybomt-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-21 21:17:20.521877 anybomt-0.1.0/anybomt.egg-info/
+-rw-rw-rw-   0        0        0    24402 2023-07-21 21:17:20.000000 anybomt-0.1.0/anybomt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      161 2023-07-21 21:17:20.000000 anybomt-0.1.0/anybomt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 21:17:20.000000 anybomt-0.1.0/anybomt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 21:17:20.000000 anybomt-0.1.0/anybomt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    39320 2023-07-21 20:54:05.000000 anybomt-0.1.0/anybomt.py
+-rw-rw-rw-   0        0        0       42 2023-07-21 21:17:20.526362 anybomt-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      815 2023-07-21 21:16:55.000000 anybomt-0.1.0/setup.py
```

### Comparing `anybomt-0.0.1/LICENSE` & `anybomt-0.1.0/LICENSE`

 * *Files identical despite different names*

