# Comparing `tmp/toRST-0.0.3.tar.gz` & `tmp/toRST-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toRST-0.0.3.tar", last modified: Wed Jul 19 01:30:59 2023, max compression
+gzip compressed data, was "toRST-0.0.4.tar", last modified: Fri Jul 21 00:52:18 2023, max compression
```

## Comparing `toRST-0.0.3.tar` & `toRST-0.0.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 jreyno     (501) staff       (20)        0 2023-07-19 01:30:59.160813 toRST-0.0.3/
--rw-r--r--   0 jreyno     (501) staff       (20)     1085 2023-07-18 19:42:12.000000 toRST-0.0.3/LICENSE
--rw-r--r--   0 jreyno     (501) staff       (20)     1755 2023-07-19 01:30:59.160884 toRST-0.0.3/PKG-INFO
--rw-r--r--   0 jreyno     (501) staff       (20)     1022 2023-07-19 00:45:51.000000 toRST-0.0.3/README.md
-drwxr-xr-x   0 jreyno     (501) staff       (20)        0 2023-07-19 01:30:59.158106 toRST-0.0.3/csv2rst/
--rw-r--r--   0 jreyno     (501) staff       (20)        0 2023-07-18 16:07:34.000000 toRST-0.0.3/csv2rst/__init__.py
--rw-r--r--   0 jreyno     (501) staff       (20)      488 2023-07-18 16:07:34.000000 toRST-0.0.3/csv2rst/csv2rst.py
-drwxr-xr-x   0 jreyno     (501) staff       (20)        0 2023-07-19 01:30:59.159009 toRST-0.0.3/funcs/
--rw-r--r--   0 jreyno     (501) staff       (20)        0 2023-07-18 16:07:34.000000 toRST-0.0.3/funcs/__init__.py
--rw-r--r--   0 jreyno     (501) staff       (20)     1179 2023-07-18 16:07:34.000000 toRST-0.0.3/funcs/command.py
--rw-r--r--   0 jreyno     (501) staff       (20)       76 2023-07-18 16:07:34.000000 toRST-0.0.3/funcs/funcs.py
-drwxr-xr-x   0 jreyno     (501) staff       (20)        0 2023-07-19 01:30:59.159292 toRST-0.0.3/json2rst/
--rw-r--r--   0 jreyno     (501) staff       (20)        0 2023-07-18 16:07:34.000000 toRST-0.0.3/json2rst/__init__.py
--rw-r--r--   0 jreyno     (501) staff       (20)      385 2023-07-18 16:07:34.000000 toRST-0.0.3/json2rst/json2rst.py
--rw-r--r--   0 jreyno     (501) staff       (20)      103 2023-07-18 20:40:47.000000 toRST-0.0.3/pyproject.toml
--rw-r--r--   0 jreyno     (501) staff       (20)      678 2023-07-19 01:30:59.161136 toRST-0.0.3/setup.cfg
--rw-r--r--   0 jreyno     (501) staff       (20)      673 2023-07-19 01:30:36.000000 toRST-0.0.3/setup.py
-drwxr-xr-x   0 jreyno     (501) staff       (20)        0 2023-07-19 01:30:59.159464 toRST-0.0.3/tests/
--rw-r--r--   0 jreyno     (501) staff       (20)      790 2023-07-18 16:07:34.000000 toRST-0.0.3/tests/test_toRST_toRST.py
-drwxr-xr-x   0 jreyno     (501) staff       (20)        0 2023-07-19 01:30:59.159941 toRST-0.0.3/toRST/
--rw-r--r--   0 jreyno     (501) staff       (20)        0 2023-07-18 16:07:34.000000 toRST-0.0.3/toRST/__init__.py
--rw-r--r--   0 jreyno     (501) staff       (20)     2965 2023-07-19 01:26:41.000000 toRST-0.0.3/toRST/toRST.py
--rw-r--r--   0 jreyno     (501) staff       (20)      374 2023-07-19 00:58:12.000000 toRST-0.0.3/toRST/write.py
-drwxr-xr-x   0 jreyno     (501) staff       (20)        0 2023-07-19 01:30:59.160683 toRST-0.0.3/toRST.egg-info/
--rw-r--r--   0 jreyno     (501) staff       (20)     1755 2023-07-19 01:30:59.000000 toRST-0.0.3/toRST.egg-info/PKG-INFO
--rw-r--r--   0 jreyno     (501) staff       (20)      404 2023-07-19 01:30:59.000000 toRST-0.0.3/toRST.egg-info/SOURCES.txt
--rw-r--r--   0 jreyno     (501) staff       (20)        1 2023-07-19 01:30:59.000000 toRST-0.0.3/toRST.egg-info/dependency_links.txt
--rw-r--r--   0 jreyno     (501) staff       (20)       44 2023-07-19 01:30:59.000000 toRST-0.0.3/toRST.egg-info/entry_points.txt
--rw-r--r--   0 jreyno     (501) staff       (20)       29 2023-07-19 01:30:59.000000 toRST-0.0.3/toRST.egg-info/top_level.txt
+drwxr-xr-x   0 jreyno     (501) staff       (20)        0 2023-07-21 00:52:18.438896 toRST-0.0.4/
+-rw-r--r--   0 jreyno     (501) staff       (20)     1085 2023-07-18 19:42:12.000000 toRST-0.0.4/LICENSE
+-rw-r--r--   0 jreyno     (501) staff       (20)     2468 2023-07-21 00:52:18.438955 toRST-0.0.4/PKG-INFO
+-rw-r--r--   0 jreyno     (501) staff       (20)     1024 2023-07-19 15:18:01.000000 toRST-0.0.4/README.md
+drwxr-xr-x   0 jreyno     (501) staff       (20)        0 2023-07-21 00:52:18.436188 toRST-0.0.4/csv2rst/
+-rw-r--r--   0 jreyno     (501) staff       (20)        0 2023-07-18 16:07:34.000000 toRST-0.0.4/csv2rst/__init__.py
+-rw-r--r--   0 jreyno     (501) staff       (20)      488 2023-07-18 16:07:34.000000 toRST-0.0.4/csv2rst/csv2rst.py
+drwxr-xr-x   0 jreyno     (501) staff       (20)        0 2023-07-21 00:52:18.437023 toRST-0.0.4/funcs/
+-rw-r--r--   0 jreyno     (501) staff       (20)        0 2023-07-18 16:07:34.000000 toRST-0.0.4/funcs/__init__.py
+-rw-r--r--   0 jreyno     (501) staff       (20)     1179 2023-07-18 16:07:34.000000 toRST-0.0.4/funcs/command.py
+-rw-r--r--   0 jreyno     (501) staff       (20)       76 2023-07-18 16:07:34.000000 toRST-0.0.4/funcs/funcs.py
+drwxr-xr-x   0 jreyno     (501) staff       (20)        0 2023-07-21 00:52:18.437345 toRST-0.0.4/json2rst/
+-rw-r--r--   0 jreyno     (501) staff       (20)        0 2023-07-18 16:07:34.000000 toRST-0.0.4/json2rst/__init__.py
+-rw-r--r--   0 jreyno     (501) staff       (20)      385 2023-07-18 16:07:34.000000 toRST-0.0.4/json2rst/json2rst.py
+-rw-r--r--   0 jreyno     (501) staff       (20)      103 2023-07-18 20:40:47.000000 toRST-0.0.4/pyproject.toml
+-rw-r--r--   0 jreyno     (501) staff       (20)      678 2023-07-21 00:52:18.439214 toRST-0.0.4/setup.cfg
+-rw-r--r--   0 jreyno     (501) staff       (20)     1386 2023-07-21 00:51:16.000000 toRST-0.0.4/setup.py
+drwxr-xr-x   0 jreyno     (501) staff       (20)        0 2023-07-21 00:52:18.437496 toRST-0.0.4/tests/
+-rw-r--r--   0 jreyno     (501) staff       (20)      790 2023-07-18 16:07:34.000000 toRST-0.0.4/tests/test_toRST_toRST.py
+drwxr-xr-x   0 jreyno     (501) staff       (20)        0 2023-07-21 00:52:18.437985 toRST-0.0.4/toRST/
+-rw-r--r--   0 jreyno     (501) staff       (20)        0 2023-07-18 16:07:34.000000 toRST-0.0.4/toRST/__init__.py
+-rw-r--r--   0 jreyno     (501) staff       (20)     2965 2023-07-19 13:36:13.000000 toRST-0.0.4/toRST/toRST.py
+-rw-r--r--   0 jreyno     (501) staff       (20)      374 2023-07-19 13:36:13.000000 toRST-0.0.4/toRST/write.py
+drwxr-xr-x   0 jreyno     (501) staff       (20)        0 2023-07-21 00:52:18.438785 toRST-0.0.4/toRST.egg-info/
+-rw-r--r--   0 jreyno     (501) staff       (20)     2468 2023-07-21 00:52:18.000000 toRST-0.0.4/toRST.egg-info/PKG-INFO
+-rw-r--r--   0 jreyno     (501) staff       (20)      404 2023-07-21 00:52:18.000000 toRST-0.0.4/toRST.egg-info/SOURCES.txt
+-rw-r--r--   0 jreyno     (501) staff       (20)        1 2023-07-21 00:52:18.000000 toRST-0.0.4/toRST.egg-info/dependency_links.txt
+-rw-r--r--   0 jreyno     (501) staff       (20)       44 2023-07-21 00:52:18.000000 toRST-0.0.4/toRST.egg-info/entry_points.txt
+-rw-r--r--   0 jreyno     (501) staff       (20)       29 2023-07-21 00:52:18.000000 toRST-0.0.4/toRST.egg-info/top_level.txt
```

### Comparing `toRST-0.0.3/LICENSE` & `toRST-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `toRST-0.0.3/README.md` & `toRST-0.0.4/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 <br>
 
 **Usage Cli**
 -------------
 example<br>
   Convert file1.csv and file2.json into RST
 ```bash
-torst file.csv file.json -o ./outputfolder
+torst file1.csv file2.json -o ./outputfolder
 ```
 
 **Positional Arguments**:
 ------------------------
 
 inputs
   One or more input files to convert to RST. Currently only CSV and JSON files are
```

### Comparing `toRST-0.0.3/funcs/command.py` & `toRST-0.0.4/funcs/command.py`

 * *Files identical despite different names*

### Comparing `toRST-0.0.3/setup.cfg` & `toRST-0.0.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `toRST-0.0.3/tests/test_toRST_toRST.py` & `toRST-0.0.4/tests/test_toRST_toRST.py`

 * *Files identical despite different names*

### Comparing `toRST-0.0.3/toRST/toRST.py` & `toRST-0.0.4/toRST/toRST.py`

 * *Files identical despite different names*

