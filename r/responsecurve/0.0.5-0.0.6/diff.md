# Comparing `tmp/responsecurve-0.0.5.tar.gz` & `tmp/responsecurve-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "responsecurve-0.0.5.tar", last modified: Thu Jul 20 21:35:59 2023, max compression
+gzip compressed data, was "responsecurve-0.0.6.tar", last modified: Thu Jul 20 22:33:17 2023, max compression
```

## Comparing `responsecurve-0.0.5.tar` & `responsecurve-0.0.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 ishanramrakhiani   (501) staff       (20)        0 2023-07-20 21:35:59.618784 responsecurve-0.0.5/
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)     1163 2023-07-20 18:34:56.000000 responsecurve-0.0.5/LICENSE
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)     5402 2023-07-20 21:35:59.618203 responsecurve-0.0.5/PKG-INFO
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)     5144 2023-07-20 21:35:07.000000 responsecurve-0.0.5/README.md
-drwxr-xr-x   0 ishanramrakhiani   (501) staff       (20)        0 2023-07-20 21:35:59.617177 responsecurve-0.0.5/responsecurve.egg-info/
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)     5402 2023-07-20 21:35:59.000000 responsecurve-0.0.5/responsecurve.egg-info/PKG-INFO
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)      210 2023-07-20 21:35:59.000000 responsecurve-0.0.5/responsecurve.egg-info/SOURCES.txt
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)        1 2023-07-20 21:35:59.000000 responsecurve-0.0.5/responsecurve.egg-info/dependency_links.txt
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)       43 2023-07-20 21:35:59.000000 responsecurve-0.0.5/responsecurve.egg-info/requires.txt
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)        1 2023-07-20 21:35:59.000000 responsecurve-0.0.5/responsecurve.egg-info/top_level.txt
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)       38 2023-07-20 21:35:59.619552 responsecurve-0.0.5/setup.cfg
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)      572 2023-07-20 21:35:47.000000 responsecurve-0.0.5/setup.py
+drwxr-xr-x   0 ishanramrakhiani   (501) staff       (20)        0 2023-07-20 22:33:17.112312 responsecurve-0.0.6/
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)     1163 2023-07-20 18:34:56.000000 responsecurve-0.0.6/LICENSE
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)    14824 2023-07-20 22:33:17.111777 responsecurve-0.0.6/PKG-INFO
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)    14566 2023-07-20 22:33:06.000000 responsecurve-0.0.6/README.md
+drwxr-xr-x   0 ishanramrakhiani   (501) staff       (20)        0 2023-07-20 22:33:17.110658 responsecurve-0.0.6/responsecurve.egg-info/
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)    14824 2023-07-20 22:33:16.000000 responsecurve-0.0.6/responsecurve.egg-info/PKG-INFO
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)      210 2023-07-20 22:33:17.000000 responsecurve-0.0.6/responsecurve.egg-info/SOURCES.txt
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)        1 2023-07-20 22:33:16.000000 responsecurve-0.0.6/responsecurve.egg-info/dependency_links.txt
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)       43 2023-07-20 22:33:16.000000 responsecurve-0.0.6/responsecurve.egg-info/requires.txt
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)        1 2023-07-20 22:33:16.000000 responsecurve-0.0.6/responsecurve.egg-info/top_level.txt
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)       38 2023-07-20 22:33:17.112476 responsecurve-0.0.6/setup.cfg
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)      572 2023-07-20 22:32:56.000000 responsecurve-0.0.6/setup.py
```

### Comparing `responsecurve-0.0.5/LICENSE` & `responsecurve-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `responsecurve-0.0.5/setup.py` & `responsecurve-0.0.6/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='responsecurve',
-    version='0.0.5',
+    version='0.0.6',
     packages=find_packages(),
     install_requires=[
         'pandas',
         'numpy',
         'scipy',
         'matplotlib',
         'scikit-learn'
```

