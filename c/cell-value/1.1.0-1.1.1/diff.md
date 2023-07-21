# Comparing `tmp/cell_value-1.1.0.tar.gz` & `tmp/cell_value-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cell_value-1.1.0.tar", last modified: Fri Jul 21 06:59:59 2023, max compression
+gzip compressed data, was "dist/cell_value-1.1.1.tar", last modified: Fri Jul 21 07:06:14 2023, max compression
```

## Comparing `cell_value-1.1.0.tar` & `cell_value-1.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 caiman     (501) staff       (20)        0 2023-07-21 06:59:59.000000 cell_value-1.1.0/
--rw-r--r--   0 caiman     (501) staff       (20)      143 2023-07-21 06:59:59.000000 cell_value-1.1.0/PKG-INFO
-drwxr-xr-x   0 caiman     (501) staff       (20)        0 2023-07-21 06:59:59.000000 cell_value-1.1.0/cell_value/
--rw-r--r--   0 caiman     (501) staff       (20)     4073 2023-07-21 06:59:17.000000 cell_value-1.1.0/cell_value/__init__.py
-drwxr-xr-x   0 caiman     (501) staff       (20)        0 2023-07-21 06:59:59.000000 cell_value-1.1.0/cell_value.egg-info/
--rw-r--r--   0 caiman     (501) staff       (20)      143 2023-07-21 06:59:59.000000 cell_value-1.1.0/cell_value.egg-info/PKG-INFO
--rw-r--r--   0 caiman     (501) staff       (20)      167 2023-07-21 06:59:59.000000 cell_value-1.1.0/cell_value.egg-info/SOURCES.txt
--rw-r--r--   0 caiman     (501) staff       (20)        1 2023-07-21 06:59:59.000000 cell_value-1.1.0/cell_value.egg-info/dependency_links.txt
--rw-r--r--   0 caiman     (501) staff       (20)       11 2023-07-21 06:59:59.000000 cell_value-1.1.0/cell_value.egg-info/top_level.txt
--rw-r--r--   0 caiman     (501) staff       (20)       38 2023-07-21 06:59:59.000000 cell_value-1.1.0/setup.cfg
--rw-r--r--   0 caiman     (501) staff       (20)      276 2023-07-21 06:59:27.000000 cell_value-1.1.0/setup.py
+drwxr-xr-x   0 caiman     (501) staff       (20)        0 2023-07-21 07:06:14.000000 cell_value-1.1.1/
+-rw-r--r--   0 caiman     (501) staff       (20)      143 2023-07-21 07:06:14.000000 cell_value-1.1.1/PKG-INFO
+drwxr-xr-x   0 caiman     (501) staff       (20)        0 2023-07-21 07:06:14.000000 cell_value-1.1.1/cell_value/
+-rw-r--r--   0 caiman     (501) staff       (20)     4083 2023-07-21 07:05:29.000000 cell_value-1.1.1/cell_value/__init__.py
+drwxr-xr-x   0 caiman     (501) staff       (20)        0 2023-07-21 07:06:14.000000 cell_value-1.1.1/cell_value.egg-info/
+-rw-r--r--   0 caiman     (501) staff       (20)      143 2023-07-21 07:06:14.000000 cell_value-1.1.1/cell_value.egg-info/PKG-INFO
+-rw-r--r--   0 caiman     (501) staff       (20)      167 2023-07-21 07:06:14.000000 cell_value-1.1.1/cell_value.egg-info/SOURCES.txt
+-rw-r--r--   0 caiman     (501) staff       (20)        1 2023-07-21 07:06:14.000000 cell_value-1.1.1/cell_value.egg-info/dependency_links.txt
+-rw-r--r--   0 caiman     (501) staff       (20)       11 2023-07-21 07:06:14.000000 cell_value-1.1.1/cell_value.egg-info/top_level.txt
+-rw-r--r--   0 caiman     (501) staff       (20)       38 2023-07-21 07:06:14.000000 cell_value-1.1.1/setup.cfg
+-rw-r--r--   0 caiman     (501) staff       (20)      276 2023-07-21 07:05:53.000000 cell_value-1.1.1/setup.py
```

### Comparing `cell_value-1.1.0/cell_value/__init__.py` & `cell_value-1.1.1/cell_value/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
                 "minItems": 1,
                 "maxItems": 99,
                 "prefixItems": [
                     {"type": "string"}
                 ]
             },
             "trace_id": {
-                "type": ["string", "null"]
+                "type": ["string", "null","integer"]
             },
             "filter_method": {
                 "type": "string",
                 "enum": [member.value for member in FilterMethod]
             }
 
         },
```

