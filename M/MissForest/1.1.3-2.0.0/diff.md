# Comparing `tmp/MissForest-1.1.3.tar.gz` & `tmp/MissForest-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MissForest-1.1.3.tar", last modified: Fri Feb 25 05:01:57 2022, max compression
+gzip compressed data, was "MissForest-2.0.0.tar", last modified: Fri Jul 21 12:51:06 2023, max compression
```

## Comparing `MissForest-1.1.3.tar` & `MissForest-2.0.0.tar`

### file list

```diff
@@ -1,16 +1,14 @@
-drwxrwxrwx   0        0        0        0 2022-02-25 05:01:57.126968 MissForest-1.1.3/
--rw-rw-rw-   0        0        0     1081 2021-06-14 10:27:46.000000 MissForest-1.1.3/LICENSE.txt
--rw-rw-rw-   0        0        0     2051 2022-02-25 05:01:57.126968 MissForest-1.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     1251 2021-12-10 02:25:11.000000 MissForest-1.1.3/README.md
--rw-rw-rw-   0        0        0      177 2021-05-03 14:48:39.000000 MissForest-1.1.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-02-25 05:01:57.127968 MissForest-1.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1104 2022-02-25 05:01:50.000000 MissForest-1.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2022-02-25 05:01:57.096583 MissForest-1.1.3/src/
-drwxrwxrwx   0        0        0        0 2022-02-25 05:01:57.123967 MissForest-1.1.3/src/MissForest.egg-info/
--rw-rw-rw-   0        0        0     2051 2022-02-25 05:01:56.000000 MissForest-1.1.3/src/MissForest.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      254 2022-02-25 05:01:56.000000 MissForest-1.1.3/src/MissForest.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-02-25 05:01:56.000000 MissForest-1.1.3/src/MissForest.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2022-02-25 05:01:56.000000 MissForest-1.1.3/src/MissForest.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-02-25 05:01:57.125968 MissForest-1.1.3/src/missforest/
--rw-rw-rw-   0        0        0        0 2022-02-25 04:41:07.000000 MissForest-1.1.3/src/missforest/__init__.py
--rw-rw-rw-   0        0        0     4064 2022-02-25 05:00:17.000000 MissForest-1.1.3/src/missforest/miss_forest.py
+drwxrwxrwx   0        0        0        0 2023-07-21 12:51:06.359460 MissForest-2.0.0/
+-rw-rw-rw-   0        0        0     2081 2023-07-21 12:51:06.358457 MissForest-2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1566 2023-07-21 12:22:18.000000 MissForest-2.0.0/README.md
+-rw-rw-rw-   0        0        0      638 2023-07-21 12:50:41.000000 MissForest-2.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-21 12:51:06.359460 MissForest-2.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-21 12:51:06.340459 MissForest-2.0.0/src/
+drwxrwxrwx   0        0        0        0 2023-07-21 12:51:06.355458 MissForest-2.0.0/src/MissForest.egg-info/
+-rw-rw-rw-   0        0        0     2081 2023-07-21 12:51:06.000000 MissForest-2.0.0/src/MissForest.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      232 2023-07-21 12:51:06.000000 MissForest-2.0.0/src/MissForest.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 12:51:06.000000 MissForest-2.0.0/src/MissForest.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-07-21 12:51:06.000000 MissForest-2.0.0/src/MissForest.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-21 12:51:06.357459 MissForest-2.0.0/src/missforest/
+-rw-rw-rw-   0        0        0        0 2023-07-21 12:07:03.000000 MissForest-2.0.0/src/missforest/__init__.py
+-rw-rw-rw-   0        0        0    11565 2023-07-21 12:50:41.000000 MissForest-2.0.0/src/missforest/missforest.py
```

