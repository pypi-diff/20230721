# Comparing `tmp/dyc_package-1.0.2.tar.gz` & `tmp/dyc_package-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dyc_package-1.0.2.tar", last modified: Fri Jul 21 03:00:07 2023, max compression
+gzip compressed data, was "dyc_package-1.0.3.tar", last modified: Fri Jul 21 03:09:14 2023, max compression
```

## Comparing `dyc_package-1.0.2.tar` & `dyc_package-1.0.3.tar`

### file list

```diff
@@ -1,9 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-21 03:00:07.231361 dyc_package-1.0.2/
--rw-rw-rw-   0        0        0      139 2023-07-21 03:00:07.230345 dyc_package-1.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-21 03:00:07.228344 dyc_package-1.0.2/dyc_package.egg-info/
--rw-rw-rw-   0        0        0      139 2023-07-21 03:00:07.000000 dyc_package-1.0.2/dyc_package.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      148 2023-07-21 03:00:07.000000 dyc_package-1.0.2/dyc_package.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 03:00:07.000000 dyc_package-1.0.2/dyc_package.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 03:00:07.000000 dyc_package-1.0.2/dyc_package.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-21 03:00:07.232345 dyc_package-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      396 2023-07-21 02:59:59.000000 dyc_package-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 03:09:14.748293 dyc_package-1.0.3/
+-rw-rw-rw-   0        0        0      139 2023-07-21 03:09:14.741184 dyc_package-1.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-21 03:09:14.732188 dyc_package-1.0.3/dyc_package/
+-rw-rw-rw-   0        0        0      128 2023-07-20 06:56:05.000000 dyc_package-1.0.3/dyc_package/main.py
+-rw-rw-rw-   0        0        0      228 2023-07-20 06:46:10.000000 dyc_package-1.0.3/dyc_package/person.py
+-rw-rw-rw-   0        0        0       35 2023-07-20 09:23:59.000000 dyc_package-1.0.3/dyc_package/test.py
+drwxrwxrwx   0        0        0        0 2023-07-21 03:09:14.739185 dyc_package-1.0.3/dyc_package.egg-info/
+-rw-rw-rw-   0        0        0      139 2023-07-21 03:09:14.000000 dyc_package-1.0.3/dyc_package.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      210 2023-07-21 03:09:14.000000 dyc_package-1.0.3/dyc_package.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 03:09:14.000000 dyc_package-1.0.3/dyc_package.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-07-21 03:09:14.000000 dyc_package-1.0.3/dyc_package.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-21 03:09:14.748798 dyc_package-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      398 2023-07-21 03:09:07.000000 dyc_package-1.0.3/setup.py
```

