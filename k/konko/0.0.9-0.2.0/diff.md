# Comparing `tmp/konko-0.0.9.tar.gz` & `tmp/konko-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "konko-0.0.9.tar", last modified: Tue Jul  4 00:00:18 2023, max compression
+gzip compressed data, was "konko-0.2.0.tar", max compression
```

## Comparing `konko-0.0.9.tar` & `konko-0.2.0.tar`

### file list

```diff
@@ -1,20 +1,11 @@
-drwxr-xr-x   0 uday.kanwar   (501) staff       (20)        0 2023-07-04 00:00:18.031524 konko-0.0.9/
--rw-r--r--   0 uday.kanwar   (501) staff       (20)      254 2023-07-04 00:00:18.031370 konko-0.0.9/PKG-INFO
--rw-r--r--   0 uday.kanwar   (501) staff       (20)       29 2023-06-01 17:28:19.000000 konko-0.0.9/README.md
--rw-r--r--   0 uday.kanwar   (501) staff       (20)      304 2023-07-03 23:59:16.000000 konko-0.0.9/pyproject.toml
--rw-r--r--   0 uday.kanwar   (501) staff       (20)       38 2023-07-04 00:00:18.031570 konko-0.0.9/setup.cfg
-drwxr-xr-x   0 uday.kanwar   (501) staff       (20)        0 2023-07-04 00:00:18.028834 konko-0.0.9/src/
-drwxr-xr-x   0 uday.kanwar   (501) staff       (20)        0 2023-07-04 00:00:18.029688 konko-0.0.9/src/konko/
--rw-r--r--   0 uday.kanwar   (501) staff       (20)      119 2023-07-03 23:52:38.000000 konko-0.0.9/src/konko/__init__.py
--rw-r--r--   0 uday.kanwar   (501) staff       (20)     1887 2023-06-15 22:41:35.000000 konko-0.0.9/src/konko/evaluate.py
--rw-r--r--   0 uday.kanwar   (501) staff       (20)     4210 2023-07-03 23:58:48.000000 konko-0.0.9/src/konko/generate.py
--rw-r--r--   0 uday.kanwar   (501) staff       (20)     1277 2023-07-01 02:14:39.000000 konko-0.0.9/src/konko/models.py
-drwxr-xr-x   0 uday.kanwar   (501) staff       (20)        0 2023-07-04 00:00:18.031159 konko-0.0.9/src/konko/utils/
--rw-r--r--   0 uday.kanwar   (501) staff       (20)        0 2023-07-03 23:40:17.000000 konko-0.0.9/src/konko/utils/__init__.py
--rw-r--r--   0 uday.kanwar   (501) staff       (20)       41 2023-06-30 21:50:53.000000 konko-0.0.9/src/konko/utils/constants.py
--rw-r--r--   0 uday.kanwar   (501) staff       (20)      209 2023-07-03 23:40:39.000000 konko-0.0.9/src/konko/utils/logs.py
-drwxr-xr-x   0 uday.kanwar   (501) staff       (20)        0 2023-07-04 00:00:18.030498 konko-0.0.9/src/konko.egg-info/
--rw-r--r--   0 uday.kanwar   (501) staff       (20)      254 2023-07-04 00:00:18.000000 konko-0.0.9/src/konko.egg-info/PKG-INFO
--rw-r--r--   0 uday.kanwar   (501) staff       (20)      323 2023-07-04 00:00:18.000000 konko-0.0.9/src/konko.egg-info/SOURCES.txt
--rw-r--r--   0 uday.kanwar   (501) staff       (20)        1 2023-07-04 00:00:18.000000 konko-0.0.9/src/konko.egg-info/dependency_links.txt
--rw-r--r--   0 uday.kanwar   (501) staff       (20)        6 2023-07-04 00:00:18.000000 konko-0.0.9/src/konko.egg-info/top_level.txt
+-rw-r--r--   0        0        0       70 2023-07-21 02:21:54.288970 konko-0.2.0/README.md
+-rw-r--r--   0        0        0      738 2023-07-21 02:34:10.654671 konko-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       95 2023-07-19 00:21:58.815710 konko-0.2.0/src/konko/__init__.py
+-rw-r--r--   0        0        0      271 2023-07-19 00:58:56.301196 konko-0.2.0/src/konko/app.py
+-rw-r--r--   0        0        0     1887 2023-07-04 09:17:33.179238 konko-0.2.0/src/konko/evaluate.py
+-rw-r--r--   0        0        0     5296 2023-07-21 02:13:06.267673 konko-0.2.0/src/konko/generate.py
+-rw-r--r--   0        0        0     2020 2023-07-19 22:59:01.411920 konko-0.2.0/src/konko/models.py
+-rw-r--r--   0        0        0        0 2023-07-04 09:17:33.179880 konko-0.2.0/src/konko/utils/__init__.py
+-rw-r--r--   0        0        0       42 2023-07-04 16:31:25.646577 konko-0.2.0/src/konko/utils/constants.py
+-rw-r--r--   0        0        0     1543 2023-07-16 00:13:06.904294 konko-0.2.0/src/konko/utils/logs.py
+-rw-r--r--   0        0        0     1061 1970-01-01 00:00:00.000000 konko-0.2.0/PKG-INFO
```

### Comparing `konko-0.0.9/src/konko/evaluate.py` & `konko-0.2.0/src/konko/evaluate.py`

 * *Files identical despite different names*

