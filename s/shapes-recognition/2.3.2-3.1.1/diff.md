# Comparing `tmp/shapes_recognition-2.3.2.tar.gz` & `tmp/shapes_recognition-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shapes_recognition-2.3.2.tar", last modified: Fri Jul  7 11:04:58 2023, max compression
+gzip compressed data, was "shapes_recognition-3.1.1.tar", max compression
```

## Comparing `shapes_recognition-2.3.2.tar` & `shapes_recognition-3.1.1.tar`

### file list

```diff
@@ -1,13 +1,19 @@
-drwxr-xr-x   0 boriskravtsov   (501) staff       (20)        0 2023-07-07 11:04:58.864114 shapes_recognition-2.3.2/
--rw-r--r--   0 boriskravtsov   (501) staff       (20)     1155 2023-07-07 11:04:58.863852 shapes_recognition-2.3.2/PKG-INFO
--rw-r--r--   0 boriskravtsov   (501) staff       (20)      606 2023-02-16 10:59:45.000000 shapes_recognition-2.3.2/README.md
--rw-r--r--   0 boriskravtsov   (501) staff       (20)       38 2023-07-07 11:04:58.864206 shapes_recognition-2.3.2/setup.cfg
--rw-r--r--   0 boriskravtsov   (501) staff       (20)     1198 2023-07-07 10:33:26.000000 shapes_recognition-2.3.2/setup.py
-drwxr-xr-x   0 boriskravtsov   (501) staff       (20)        0 2023-07-07 11:04:58.861003 shapes_recognition-2.3.2/shapes_recognition/
-drwxr-xr-x   0 boriskravtsov   (501) staff       (20)        0 2023-07-07 11:04:58.863360 shapes_recognition-2.3.2/shapes_recognition/pure_cython/
--rw-r--r--   0 boriskravtsov   (501) staff       (20)      301 2022-12-10 15:57:51.000000 shapes_recognition-2.3.2/shapes_recognition/pure_cython/setup.py
-drwxr-xr-x   0 boriskravtsov   (501) staff       (20)        0 2023-07-07 11:04:58.862998 shapes_recognition-2.3.2/shapes_recognition.egg-info/
--rw-r--r--   0 boriskravtsov   (501) staff       (20)     1155 2023-07-07 11:04:58.000000 shapes_recognition-2.3.2/shapes_recognition.egg-info/PKG-INFO
--rw-r--r--   0 boriskravtsov   (501) staff       (20)      226 2023-07-07 11:04:58.000000 shapes_recognition-2.3.2/shapes_recognition.egg-info/SOURCES.txt
--rw-r--r--   0 boriskravtsov   (501) staff       (20)        1 2023-07-07 11:04:58.000000 shapes_recognition-2.3.2/shapes_recognition.egg-info/dependency_links.txt
--rw-r--r--   0 boriskravtsov   (501) staff       (20)       19 2023-07-07 11:04:58.000000 shapes_recognition-2.3.2/shapes_recognition.egg-info/top_level.txt
+-rw-r--r--   0        0        0      606 2023-02-16 10:59:45.000000 shapes_recognition-3.1.1/README.md
+-rw-r--r--   0        0        0      450 2023-07-21 20:09:54.582790 shapes_recognition-3.1.1/pyproject.toml
+-rw-r--r--   0        0        0     6148 2023-07-21 19:25:32.576284 shapes_recognition-3.1.1/shapes_recognition/.DS_Store
+-rw-r--r--   0        0        0      231 2023-07-21 14:53:08.313682 shapes_recognition-3.1.1/shapes_recognition/__init__.py
+-rw-r--r--   0        0        0     6148 2023-07-21 19:38:34.562667 shapes_recognition-3.1.1/shapes_recognition/src/.DS_Store
+-rw-r--r--   0        0        0      926 2023-07-21 15:08:18.604666 shapes_recognition-3.1.1/shapes_recognition/src/cfg.py
+-rw-r--r--   0        0        0     2444 2023-07-21 15:08:18.610725 shapes_recognition-3.1.1/shapes_recognition/src/create_joint_table.py
+-rw-r--r--   0        0        0     2512 2023-07-21 15:08:18.560495 shapes_recognition-3.1.1/shapes_recognition/src/create_table.py
+-rw-r--r--   0        0        0     2068 2023-07-21 15:08:18.598622 shapes_recognition-3.1.1/shapes_recognition/src/create_template.py
+-rw-r--r--   0        0        0     1710 2023-07-21 15:08:18.593028 shapes_recognition-3.1.1/shapes_recognition/src/get_column_data.py
+-rw-r--r--   0        0        0     2667 2023-07-21 15:08:18.607481 shapes_recognition-3.1.1/shapes_recognition/src/get_peaks.py
+-rw-r--r--   0        0        0     5897 2023-07-21 15:08:18.601878 shapes_recognition-3.1.1/shapes_recognition/src/get_results.py
+-rw-r--r--   0        0        0     2452 2023-07-21 15:08:18.567925 shapes_recognition-3.1.1/shapes_recognition/src/recognition.py
+-rw-r--r--   0        0        0     1648 2023-07-21 15:12:32.259774 shapes_recognition-3.1.1/shapes_recognition/src/save_results.py
+-rw-r--r--   0        0        0     4124 2023-07-21 15:12:32.281959 shapes_recognition-3.1.1/shapes_recognition/src/self_study.py
+-rw-r--r--   0        0        0     4826 2023-07-21 15:12:32.275834 shapes_recognition-3.1.1/shapes_recognition/src/shapes_similarity.py
+-rw-r--r--   0        0        0      679 2023-07-21 15:12:32.284608 shapes_recognition-3.1.1/shapes_recognition/src/show_results.py
+-rw-r--r--   0        0        0     2577 2023-07-21 15:12:32.278948 shapes_recognition-3.1.1/shapes_recognition/src/utils.py
+-rw-r--r--   0        0        0     1193 1970-01-01 00:00:00.000000 shapes_recognition-3.1.1/PKG-INFO
```

### Comparing `shapes_recognition-2.3.2/README.md` & `shapes_recognition-3.1.1/README.md`

 * *Files identical despite different names*

