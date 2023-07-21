# Comparing `tmp/dyc_package-1.0.1.tar.gz` & `tmp/dyc_package-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dyc_package-1.0.1.tar", last modified: Fri Jul 21 02:59:40 2023, max compression
+gzip compressed data, was "dyc_package-1.0.2.tar", last modified: Fri Jul 21 03:00:07 2023, max compression
```

## Comparing `dyc_package-1.0.1.tar` & `dyc_package-1.0.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
-drwxrwxrwx   0        0        0        0 2023-07-21 02:59:40.741287 dyc_package-1.0.1/
--rw-rw-rw-   0        0        0      139 2023-07-21 02:59:40.740364 dyc_package-1.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-21 02:59:40.738502 dyc_package-1.0.1/dyc_package.egg-info/
--rw-rw-rw-   0        0        0      139 2023-07-21 02:59:40.000000 dyc_package-1.0.1/dyc_package.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      148 2023-07-21 02:59:40.000000 dyc_package-1.0.1/dyc_package.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 02:59:40.000000 dyc_package-1.0.1/dyc_package.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 02:59:40.000000 dyc_package-1.0.1/dyc_package.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-21 02:59:40.741287 dyc_package-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      396 2023-07-21 02:59:29.000000 dyc_package-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 03:00:07.231361 dyc_package-1.0.2/
+-rw-rw-rw-   0        0        0      139 2023-07-21 03:00:07.230345 dyc_package-1.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-21 03:00:07.228344 dyc_package-1.0.2/dyc_package.egg-info/
+-rw-rw-rw-   0        0        0      139 2023-07-21 03:00:07.000000 dyc_package-1.0.2/dyc_package.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      148 2023-07-21 03:00:07.000000 dyc_package-1.0.2/dyc_package.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 03:00:07.000000 dyc_package-1.0.2/dyc_package.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 03:00:07.000000 dyc_package-1.0.2/dyc_package.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-21 03:00:07.232345 dyc_package-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      396 2023-07-21 02:59:59.000000 dyc_package-1.0.2/setup.py
```

