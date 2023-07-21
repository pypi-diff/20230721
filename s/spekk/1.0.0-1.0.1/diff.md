# Comparing `tmp/spekk-1.0.0.tar.gz` & `tmp/spekk-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spekk-1.0.0.tar", last modified: Fri Jul 21 15:09:13 2023, max compression
+gzip compressed data, was "spekk-1.0.1.tar", last modified: Fri Jul 21 18:32:36 2023, max compression
```

## Comparing `spekk-1.0.0.tar` & `spekk-1.0.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-07-21 15:09:13.890349 spekk-1.0.0/
--rw-r--r--   0 magnus     (501) staff       (20)    11356 2023-07-21 15:08:01.000000 spekk-1.0.0/LICENSE
--rw-r--r--   0 magnus     (501) staff       (20)      174 2023-07-21 15:09:13.889663 spekk-1.0.0/PKG-INFO
--rw-r--r--   0 magnus     (501) staff       (20)     7351 2023-07-21 15:03:13.000000 spekk-1.0.0/README.md
--rw-r--r--   0 magnus     (501) staff       (20)       86 2023-07-21 15:06:26.000000 spekk-1.0.0/pyproject.toml
--rw-r--r--   0 magnus     (501) staff       (20)       38 2023-07-21 15:09:13.890705 spekk-1.0.0/setup.cfg
--rw-r--r--   0 magnus     (501) staff       (20)      302 2023-07-21 15:06:51.000000 spekk-1.0.0/setup.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-07-21 15:09:13.833264 spekk-1.0.0/spekk/
--rw-r--r--   0 magnus     (501) staff       (20)       77 2023-07-18 14:59:52.000000 spekk-1.0.0/spekk/__init__.py
--rw-r--r--   0 magnus     (501) staff       (20)    12630 2023-07-19 08:18:35.000000 spekk-1.0.0/spekk/spec.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-07-21 15:09:13.856739 spekk-1.0.0/spekk/transformations/
--rw-r--r--   0 magnus     (501) staff       (20)     6475 2023-07-21 14:41:00.000000 spekk-1.0.0/spekk/transformations/__init__.py
--rw-r--r--   0 magnus     (501) staff       (20)     2151 2023-07-18 12:37:43.000000 spekk-1.0.0/spekk/transformations/apply.py
--rw-r--r--   0 magnus     (501) staff       (20)     3619 2023-07-18 13:20:36.000000 spekk-1.0.0/spekk/transformations/axis.py
--rw-r--r--   0 magnus     (501) staff       (20)    15523 2023-07-19 07:38:43.000000 spekk-1.0.0/spekk/transformations/base.py
--rw-r--r--   0 magnus     (501) staff       (20)     2965 2023-07-19 08:22:04.000000 spekk-1.0.0/spekk/transformations/common.py
--rw-r--r--   0 magnus     (501) staff       (20)     3784 2023-07-21 14:42:27.000000 spekk-1.0.0/spekk/transformations/for_all.py
--rw-r--r--   0 magnus     (501) staff       (20)     5805 2023-07-18 13:45:41.000000 spekk-1.0.0/spekk/transformations/reduce.py
--rw-r--r--   0 magnus     (501) staff       (20)     1970 2023-07-18 13:46:06.000000 spekk-1.0.0/spekk/transformations/wrap.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-07-21 15:09:13.875084 spekk-1.0.0/spekk/trees/
--rw-r--r--   0 magnus     (501) staff       (20)      663 2023-07-19 08:08:29.000000 spekk-1.0.0/spekk/trees/__init__.py
--rw-r--r--   0 magnus     (501) staff       (20)     7070 2023-07-18 13:09:43.000000 spekk-1.0.0/spekk/trees/core.py
--rw-r--r--   0 magnus     (501) staff       (20)     5672 2023-07-21 13:57:38.000000 spekk-1.0.0/spekk/trees/registry.py
--rw-r--r--   0 magnus     (501) staff       (20)     5109 2023-07-18 13:00:44.000000 spekk-1.0.0/spekk/trees/treelens.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-07-21 15:09:13.887582 spekk-1.0.0/spekk/util/
--rw-r--r--   0 magnus     (501) staff       (20)      342 2023-07-18 13:53:37.000000 spekk-1.0.0/spekk/util/__init__.py
--rw-r--r--   0 magnus     (501) staff       (20)     5165 2023-07-18 13:46:46.000000 spekk-1.0.0/spekk/util/flatten.py
--rw-r--r--   0 magnus     (501) staff       (20)      712 2023-07-21 13:59:51.000000 spekk-1.0.0/spekk/util/shape.py
--rw-r--r--   0 magnus     (501) staff       (20)     3110 2023-07-18 13:49:24.000000 spekk-1.0.0/spekk/util/slicing.py
--rw-r--r--   0 magnus     (501) staff       (20)     8012 2023-07-18 13:58:57.000000 spekk-1.0.0/spekk/util/validation.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-07-21 15:09:13.841962 spekk-1.0.0/spekk.egg-info/
--rw-r--r--   0 magnus     (501) staff       (20)      174 2023-07-21 15:09:13.000000 spekk-1.0.0/spekk.egg-info/PKG-INFO
--rw-r--r--   0 magnus     (501) staff       (20)      673 2023-07-21 15:09:13.000000 spekk-1.0.0/spekk.egg-info/SOURCES.txt
--rw-r--r--   0 magnus     (501) staff       (20)        1 2023-07-21 15:09:13.000000 spekk-1.0.0/spekk.egg-info/dependency_links.txt
--rw-r--r--   0 magnus     (501) staff       (20)        6 2023-07-21 15:09:13.000000 spekk-1.0.0/spekk.egg-info/requires.txt
--rw-r--r--   0 magnus     (501) staff       (20)        6 2023-07-21 15:09:13.000000 spekk-1.0.0/spekk.egg-info/top_level.txt
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-07-21 18:32:36.856966 spekk-1.0.1/
+-rw-r--r--   0 magnus     (501) staff       (20)    11356 2023-07-21 15:08:01.000000 spekk-1.0.1/LICENSE
+-rw-r--r--   0 magnus     (501) staff       (20)     7896 2023-07-21 18:32:36.856439 spekk-1.0.1/PKG-INFO
+-rw-r--r--   0 magnus     (501) staff       (20)     7351 2023-07-21 15:03:13.000000 spekk-1.0.1/README.md
+-rw-r--r--   0 magnus     (501) staff       (20)      581 2023-07-21 18:32:17.000000 spekk-1.0.1/pyproject.toml
+-rw-r--r--   0 magnus     (501) staff       (20)       38 2023-07-21 18:32:36.857106 spekk-1.0.1/setup.cfg
+-rw-r--r--   0 magnus     (501) staff       (20)      302 2023-07-21 18:32:20.000000 spekk-1.0.1/setup.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-07-21 18:32:36.819606 spekk-1.0.1/spekk/
+-rw-r--r--   0 magnus     (501) staff       (20)       77 2023-07-21 18:32:25.000000 spekk-1.0.1/spekk/__init__.py
+-rw-r--r--   0 magnus     (501) staff       (20)    12630 2023-07-19 08:18:35.000000 spekk-1.0.1/spekk/spec.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-07-21 18:32:36.839609 spekk-1.0.1/spekk/transformations/
+-rw-r--r--   0 magnus     (501) staff       (20)     6475 2023-07-21 14:41:00.000000 spekk-1.0.1/spekk/transformations/__init__.py
+-rw-r--r--   0 magnus     (501) staff       (20)     2151 2023-07-18 12:37:43.000000 spekk-1.0.1/spekk/transformations/apply.py
+-rw-r--r--   0 magnus     (501) staff       (20)     3619 2023-07-18 13:20:36.000000 spekk-1.0.1/spekk/transformations/axis.py
+-rw-r--r--   0 magnus     (501) staff       (20)    15523 2023-07-19 07:38:43.000000 spekk-1.0.1/spekk/transformations/base.py
+-rw-r--r--   0 magnus     (501) staff       (20)     2965 2023-07-19 08:22:04.000000 spekk-1.0.1/spekk/transformations/common.py
+-rw-r--r--   0 magnus     (501) staff       (20)     3784 2023-07-21 14:42:27.000000 spekk-1.0.1/spekk/transformations/for_all.py
+-rw-r--r--   0 magnus     (501) staff       (20)     5805 2023-07-18 13:45:41.000000 spekk-1.0.1/spekk/transformations/reduce.py
+-rw-r--r--   0 magnus     (501) staff       (20)     1970 2023-07-18 13:46:06.000000 spekk-1.0.1/spekk/transformations/wrap.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-07-21 18:32:36.847224 spekk-1.0.1/spekk/trees/
+-rw-r--r--   0 magnus     (501) staff       (20)      663 2023-07-19 08:08:29.000000 spekk-1.0.1/spekk/trees/__init__.py
+-rw-r--r--   0 magnus     (501) staff       (20)     7070 2023-07-18 13:09:43.000000 spekk-1.0.1/spekk/trees/core.py
+-rw-r--r--   0 magnus     (501) staff       (20)     5672 2023-07-21 13:57:38.000000 spekk-1.0.1/spekk/trees/registry.py
+-rw-r--r--   0 magnus     (501) staff       (20)     5109 2023-07-18 13:00:44.000000 spekk-1.0.1/spekk/trees/treelens.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-07-21 18:32:36.854656 spekk-1.0.1/spekk/util/
+-rw-r--r--   0 magnus     (501) staff       (20)      342 2023-07-18 13:53:37.000000 spekk-1.0.1/spekk/util/__init__.py
+-rw-r--r--   0 magnus     (501) staff       (20)     5165 2023-07-18 13:46:46.000000 spekk-1.0.1/spekk/util/flatten.py
+-rw-r--r--   0 magnus     (501) staff       (20)      712 2023-07-21 13:59:51.000000 spekk-1.0.1/spekk/util/shape.py
+-rw-r--r--   0 magnus     (501) staff       (20)     3110 2023-07-18 13:49:24.000000 spekk-1.0.1/spekk/util/slicing.py
+-rw-r--r--   0 magnus     (501) staff       (20)     8012 2023-07-18 13:58:57.000000 spekk-1.0.1/spekk/util/validation.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-07-21 18:32:36.823484 spekk-1.0.1/spekk.egg-info/
+-rw-r--r--   0 magnus     (501) staff       (20)     7896 2023-07-21 18:32:36.000000 spekk-1.0.1/spekk.egg-info/PKG-INFO
+-rw-r--r--   0 magnus     (501) staff       (20)      673 2023-07-21 18:32:36.000000 spekk-1.0.1/spekk.egg-info/SOURCES.txt
+-rw-r--r--   0 magnus     (501) staff       (20)        1 2023-07-21 18:32:36.000000 spekk-1.0.1/spekk.egg-info/dependency_links.txt
+-rw-r--r--   0 magnus     (501) staff       (20)        6 2023-07-21 18:32:36.000000 spekk-1.0.1/spekk.egg-info/requires.txt
+-rw-r--r--   0 magnus     (501) staff       (20)        6 2023-07-21 18:32:36.000000 spekk-1.0.1/spekk.egg-info/top_level.txt
```

### Comparing `spekk-1.0.0/LICENSE` & `spekk-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `spekk-1.0.0/README.md` & `spekk-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `spekk-1.0.0/spekk/spec.py` & `spekk-1.0.1/spekk/spec.py`

 * *Files identical despite different names*

### Comparing `spekk-1.0.0/spekk/transformations/__init__.py` & `spekk-1.0.1/spekk/transformations/__init__.py`

 * *Files identical despite different names*

### Comparing `spekk-1.0.0/spekk/transformations/apply.py` & `spekk-1.0.1/spekk/transformations/apply.py`

 * *Files identical despite different names*

### Comparing `spekk-1.0.0/spekk/transformations/axis.py` & `spekk-1.0.1/spekk/transformations/axis.py`

 * *Files identical despite different names*

### Comparing `spekk-1.0.0/spekk/transformations/base.py` & `spekk-1.0.1/spekk/transformations/base.py`

 * *Files identical despite different names*

### Comparing `spekk-1.0.0/spekk/transformations/common.py` & `spekk-1.0.1/spekk/transformations/common.py`

 * *Files identical despite different names*

### Comparing `spekk-1.0.0/spekk/transformations/for_all.py` & `spekk-1.0.1/spekk/transformations/for_all.py`

 * *Files identical despite different names*

### Comparing `spekk-1.0.0/spekk/transformations/reduce.py` & `spekk-1.0.1/spekk/transformations/reduce.py`

 * *Files identical despite different names*

### Comparing `spekk-1.0.0/spekk/transformations/wrap.py` & `spekk-1.0.1/spekk/transformations/wrap.py`

 * *Files identical despite different names*

### Comparing `spekk-1.0.0/spekk/trees/__init__.py` & `spekk-1.0.1/spekk/trees/__init__.py`

 * *Files identical despite different names*

### Comparing `spekk-1.0.0/spekk/trees/core.py` & `spekk-1.0.1/spekk/trees/core.py`

 * *Files identical despite different names*

### Comparing `spekk-1.0.0/spekk/trees/registry.py` & `spekk-1.0.1/spekk/trees/registry.py`

 * *Files identical despite different names*

### Comparing `spekk-1.0.0/spekk/trees/treelens.py` & `spekk-1.0.1/spekk/trees/treelens.py`

 * *Files identical despite different names*

### Comparing `spekk-1.0.0/spekk/util/flatten.py` & `spekk-1.0.1/spekk/util/flatten.py`

 * *Files identical despite different names*

### Comparing `spekk-1.0.0/spekk/util/shape.py` & `spekk-1.0.1/spekk/util/shape.py`

 * *Files identical despite different names*

### Comparing `spekk-1.0.0/spekk/util/slicing.py` & `spekk-1.0.1/spekk/util/slicing.py`

 * *Files identical despite different names*

### Comparing `spekk-1.0.0/spekk/util/validation.py` & `spekk-1.0.1/spekk/util/validation.py`

 * *Files identical despite different names*

### Comparing `spekk-1.0.0/spekk.egg-info/SOURCES.txt` & `spekk-1.0.1/spekk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

