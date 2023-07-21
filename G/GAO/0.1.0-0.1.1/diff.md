# Comparing `tmp/GAO-0.1.0.tar.gz` & `tmp/GAO-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GAO-0.1.0.tar", last modified: Fri Jul 21 01:47:12 2023, max compression
+gzip compressed data, was "GAO-0.1.1.tar", last modified: Fri Jul 21 03:39:13 2023, max compression
```

## Comparing `GAO-0.1.0.tar` & `GAO-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
-drwxrwxrwx   0        0        0        0 2023-07-21 01:47:12.971567 GAO-0.1.0/
-drwxrwxrwx   0        0        0        0 2023-07-21 01:47:12.969568 GAO-0.1.0/GAO.egg-info/
--rw-rw-rw-   0        0        0      136 2023-07-21 01:47:12.000000 GAO-0.1.0/GAO.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      116 2023-07-21 01:47:12.000000 GAO-0.1.0/GAO.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 01:47:12.000000 GAO-0.1.0/GAO.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 01:47:12.000000 GAO-0.1.0/GAO.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      136 2023-07-21 01:47:12.971567 GAO-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-21 01:47:12.971567 GAO-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      332 2023-07-21 01:45:54.000000 GAO-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 03:39:13.780752 GAO-0.1.1/
+drwxrwxrwx   0        0        0        0 2023-07-21 03:39:13.778753 GAO-0.1.1/GAO.egg-info/
+-rw-rw-rw-   0        0        0      136 2023-07-21 03:39:13.000000 GAO-0.1.1/GAO.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      116 2023-07-21 03:39:13.000000 GAO-0.1.1/GAO.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 03:39:13.000000 GAO-0.1.1/GAO.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 03:39:13.000000 GAO-0.1.1/GAO.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      136 2023-07-21 03:39:13.779752 GAO-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-21 03:39:13.780752 GAO-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      332 2023-07-21 03:38:16.000000 GAO-0.1.1/setup.py
```

