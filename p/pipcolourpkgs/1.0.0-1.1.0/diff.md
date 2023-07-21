# Comparing `tmp/pipcolourpkgs-1.0.0.tar.gz` & `tmp/pipcolourpkgs-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipcolourpkgs-1.0.0.tar", last modified: Fri Jul 21 15:04:25 2023, max compression
+gzip compressed data, was "pipcolourpkgs-1.1.0.tar", last modified: Fri Jul 21 15:06:30 2023, max compression
```

## Comparing `pipcolourpkgs-1.0.0.tar` & `pipcolourpkgs-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:04:25.045057 pipcolourpkgs-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      346 2023-07-21 15:04:25.045057 pipcolourpkgs-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:04:25.045057 pipcolourpkgs-1.0.0/pipcolourpkgs/
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-21 15:04:24.000000 pipcolourpkgs-1.0.0/pipcolourpkgs/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:04:25.045057 pipcolourpkgs-1.0.0/pipcolourpkgs.egg-info/
--rw-r--r--   0 root         (0) root         (0)      346 2023-07-21 15:04:24.000000 pipcolourpkgs-1.0.0/pipcolourpkgs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      182 2023-07-21 15:04:24.000000 pipcolourpkgs-1.0.0/pipcolourpkgs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 15:04:24.000000 pipcolourpkgs-1.0.0/pipcolourpkgs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-07-21 15:04:24.000000 pipcolourpkgs-1.0.0/pipcolourpkgs.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-21 15:04:25.045057 pipcolourpkgs-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      559 2023-07-21 15:04:24.000000 pipcolourpkgs-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:06:30.128660 pipcolourpkgs-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      346 2023-07-21 15:06:30.128660 pipcolourpkgs-1.1.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:06:30.124660 pipcolourpkgs-1.1.0/pipcolourpkgs/
+-rw-r--r--   0 root         (0) root         (0)    96773 2023-07-21 15:06:29.000000 pipcolourpkgs-1.1.0/pipcolourpkgs/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:06:30.128660 pipcolourpkgs-1.1.0/pipcolourpkgs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      346 2023-07-21 15:06:30.000000 pipcolourpkgs-1.1.0/pipcolourpkgs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      182 2023-07-21 15:06:30.000000 pipcolourpkgs-1.1.0/pipcolourpkgs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 15:06:30.000000 pipcolourpkgs-1.1.0/pipcolourpkgs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-07-21 15:06:30.000000 pipcolourpkgs-1.1.0/pipcolourpkgs.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-21 15:06:30.128660 pipcolourpkgs-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      559 2023-07-21 15:06:29.000000 pipcolourpkgs-1.1.0/setup.py
```

### Comparing `pipcolourpkgs-1.0.0/setup.py` & `pipcolourpkgs-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.0'
+VERSION = '1.1.0'
 DESCRIPTION = "Usefull utility package"
 LONG_DESCRIPTION = "Usefull utility package"
 
 # Setting up
 setup(
     name="pipcolourpkgs",
     version=VERSION,
```

