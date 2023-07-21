# Comparing `tmp/healdata_utils-0.1.3a0.tar.gz` & `tmp/healdata_utils-0.1.4a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "healdata_utils-0.1.3a0.tar", last modified: Fri Jul 21 03:58:36 2023, max compression
+gzip compressed data, was "healdata_utils-0.1.4a0.tar", last modified: Fri Jul 21 13:43:11 2023, max compression
```

## Comparing `healdata_utils-0.1.3a0.tar` & `healdata_utils-0.1.4a0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 03:58:36.090678 healdata_utils-0.1.3a0/
--rw-r--r--   0 runner    (1001) docker     (123)     6186 2023-07-21 03:58:36.090678 healdata_utils-0.1.3a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5912 2023-07-21 03:58:26.000000 healdata_utils-0.1.3a0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 03:58:36.090678 healdata_utils-0.1.3a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-21 03:58:27.000000 healdata_utils-0.1.3a0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 03:58:36.082678 healdata_utils-0.1.3a0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 03:58:36.086678 healdata_utils-0.1.3a0/src/healdata_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 03:58:27.000000 healdata_utils-0.1.3a0/src/healdata_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8569 2023-07-21 03:58:27.000000 healdata_utils-0.1.3a0/src/healdata_utils/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-07-21 03:58:27.000000 healdata_utils-0.1.3a0/src/healdata_utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-07-21 03:58:27.000000 healdata_utils-0.1.3a0/src/healdata_utils/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 03:58:36.086678 healdata_utils-0.1.3a0/src/healdata_utils/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 03:58:27.000000 healdata_utils-0.1.3a0/src/healdata_utils/transforms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 03:58:36.086678 healdata_utils-0.1.3a0/src/healdata_utils/transforms/csvdata/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-21 03:58:27.000000 healdata_utils-0.1.3a0/src/healdata_utils/transforms/csvdata/conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 03:58:36.086678 healdata_utils-0.1.3a0/src/healdata_utils/transforms/csvtemplate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 03:58:27.000000 healdata_utils-0.1.3a0/src/healdata_utils/transforms/csvtemplate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-07-21 03:58:27.000000 healdata_utils-0.1.3a0/src/healdata_utils/transforms/csvtemplate/conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     3576 2023-07-21 03:58:27.000000 healdata_utils-0.1.3a0/src/healdata_utils/transforms/csvtemplate/mappings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 03:58:36.086678 healdata_utils-0.1.3a0/src/healdata_utils/transforms/frictionless/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-21 03:58:27.000000 healdata_utils-0.1.3a0/src/healdata_utils/transforms/frictionless/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-07-21 03:58:27.000000 healdata_utils-0.1.3a0/src/healdata_utils/transforms/frictionless/conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 03:58:36.086678 healdata_utils-0.1.3a0/src/healdata_utils/transforms/jsontemplate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 03:58:27.000000 healdata_utils-0.1.3a0/src/healdata_utils/transforms/jsontemplate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-07-21 03:58:27.000000 healdata_utils-0.1.3a0/src/healdata_utils/transforms/jsontemplate/conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-07-21 03:58:27.000000 healdata_utils-0.1.3a0/src/healdata_utils/transforms/jsontemplate/mappings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 03:58:36.086678 healdata_utils-0.1.3a0/src/healdata_utils/transforms/readstat/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 03:58:27.000000 healdata_utils-0.1.3a0/src/healdata_utils/transforms/readstat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-07-21 03:58:27.000000 healdata_utils-0.1.3a0/src/healdata_utils/transforms/readstat/conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 03:58:36.086678 healdata_utils-0.1.3a0/src/healdata_utils/transforms/redcapcsv/
--rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-07-21 03:58:27.000000 healdata_utils-0.1.3a0/src/healdata_utils/transforms/redcapcsv/conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-07-21 03:58:27.000000 healdata_utils-0.1.3a0/src/healdata_utils/transforms/redcapcsv/headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8786 2023-07-21 03:58:27.000000 healdata_utils-0.1.3a0/src/healdata_utils/transforms/redcapcsv/mappings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-07-21 03:58:27.000000 healdata_utils-0.1.3a0/src/healdata_utils/transforms/redcapcsv/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 03:58:36.086678 healdata_utils-0.1.3a0/src/healdata_utils/types/
--rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-07-21 03:58:27.000000 healdata_utils-0.1.3a0/src/healdata_utils/types/typesets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-07-21 03:58:27.000000 healdata_utils-0.1.3a0/src/healdata_utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 03:58:36.090678 healdata_utils-0.1.3a0/src/healdata_utils/validators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 03:58:27.000000 healdata_utils-0.1.3a0/src/healdata_utils/validators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-21 03:58:27.000000 healdata_utils-0.1.3a0/src/healdata_utils/validators/frictionless.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-21 03:58:27.000000 healdata_utils-0.1.3a0/src/healdata_utils/validators/jsonschema.py
--rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-07-21 03:58:27.000000 healdata_utils-0.1.3a0/src/healdata_utils/validators/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 03:58:36.086678 healdata_utils-0.1.3a0/src/healdata_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6186 2023-07-21 03:58:36.000000 healdata_utils-0.1.3a0/src/healdata_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-07-21 03:58:36.000000 healdata_utils-0.1.3a0/src/healdata_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 03:58:36.000000 healdata_utils-0.1.3a0/src/healdata_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-21 03:58:36.000000 healdata_utils-0.1.3a0/src/healdata_utils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-21 03:58:36.000000 healdata_utils-0.1.3a0/src/healdata_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-21 03:58:36.000000 healdata_utils-0.1.3a0/src/healdata_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 03:58:36.090678 healdata_utils-0.1.3a0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-07-21 03:58:27.000000 healdata_utils-0.1.3a0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    10039 2023-07-21 03:58:27.000000 healdata_utils-0.1.3a0/tests/test_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-21 03:58:27.000000 healdata_utils-0.1.3a0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:43:11.021076 healdata_utils-0.1.4a0/
+-rw-r--r--   0 runner    (1001) docker     (123)     6186 2023-07-21 13:43:11.021076 healdata_utils-0.1.4a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5912 2023-07-21 13:43:01.000000 healdata_utils-0.1.4a0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 13:43:11.021076 healdata_utils-0.1.4a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-21 13:43:01.000000 healdata_utils-0.1.4a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:43:11.017076 healdata_utils-0.1.4a0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:43:11.017076 healdata_utils-0.1.4a0/src/healdata_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 13:43:01.000000 healdata_utils-0.1.4a0/src/healdata_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8569 2023-07-21 13:43:01.000000 healdata_utils-0.1.4a0/src/healdata_utils/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-07-21 13:43:01.000000 healdata_utils-0.1.4a0/src/healdata_utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-07-21 13:43:01.000000 healdata_utils-0.1.4a0/src/healdata_utils/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:43:11.017076 healdata_utils-0.1.4a0/src/healdata_utils/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 13:43:01.000000 healdata_utils-0.1.4a0/src/healdata_utils/transforms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:43:11.021076 healdata_utils-0.1.4a0/src/healdata_utils/transforms/csvdata/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-21 13:43:01.000000 healdata_utils-0.1.4a0/src/healdata_utils/transforms/csvdata/conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:43:11.021076 healdata_utils-0.1.4a0/src/healdata_utils/transforms/csvtemplate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 13:43:01.000000 healdata_utils-0.1.4a0/src/healdata_utils/transforms/csvtemplate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-07-21 13:43:01.000000 healdata_utils-0.1.4a0/src/healdata_utils/transforms/csvtemplate/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3576 2023-07-21 13:43:01.000000 healdata_utils-0.1.4a0/src/healdata_utils/transforms/csvtemplate/mappings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:43:11.021076 healdata_utils-0.1.4a0/src/healdata_utils/transforms/frictionless/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-21 13:43:01.000000 healdata_utils-0.1.4a0/src/healdata_utils/transforms/frictionless/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-07-21 13:43:01.000000 healdata_utils-0.1.4a0/src/healdata_utils/transforms/frictionless/conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:43:11.021076 healdata_utils-0.1.4a0/src/healdata_utils/transforms/jsontemplate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 13:43:01.000000 healdata_utils-0.1.4a0/src/healdata_utils/transforms/jsontemplate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-07-21 13:43:01.000000 healdata_utils-0.1.4a0/src/healdata_utils/transforms/jsontemplate/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-07-21 13:43:01.000000 healdata_utils-0.1.4a0/src/healdata_utils/transforms/jsontemplate/mappings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:43:11.021076 healdata_utils-0.1.4a0/src/healdata_utils/transforms/readstat/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 13:43:01.000000 healdata_utils-0.1.4a0/src/healdata_utils/transforms/readstat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5018 2023-07-21 13:43:01.000000 healdata_utils-0.1.4a0/src/healdata_utils/transforms/readstat/conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:43:11.021076 healdata_utils-0.1.4a0/src/healdata_utils/transforms/redcapcsv/
+-rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-07-21 13:43:01.000000 healdata_utils-0.1.4a0/src/healdata_utils/transforms/redcapcsv/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-07-21 13:43:01.000000 healdata_utils-0.1.4a0/src/healdata_utils/transforms/redcapcsv/headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8786 2023-07-21 13:43:01.000000 healdata_utils-0.1.4a0/src/healdata_utils/transforms/redcapcsv/mappings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-07-21 13:43:01.000000 healdata_utils-0.1.4a0/src/healdata_utils/transforms/redcapcsv/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:43:11.021076 healdata_utils-0.1.4a0/src/healdata_utils/types/
+-rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-07-21 13:43:01.000000 healdata_utils-0.1.4a0/src/healdata_utils/types/typesets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-07-21 13:43:01.000000 healdata_utils-0.1.4a0/src/healdata_utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:43:11.021076 healdata_utils-0.1.4a0/src/healdata_utils/validators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 13:43:01.000000 healdata_utils-0.1.4a0/src/healdata_utils/validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-21 13:43:01.000000 healdata_utils-0.1.4a0/src/healdata_utils/validators/frictionless.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-21 13:43:01.000000 healdata_utils-0.1.4a0/src/healdata_utils/validators/jsonschema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-07-21 13:43:01.000000 healdata_utils-0.1.4a0/src/healdata_utils/validators/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:43:11.017076 healdata_utils-0.1.4a0/src/healdata_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6186 2023-07-21 13:43:11.000000 healdata_utils-0.1.4a0/src/healdata_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-07-21 13:43:11.000000 healdata_utils-0.1.4a0/src/healdata_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 13:43:11.000000 healdata_utils-0.1.4a0/src/healdata_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-21 13:43:11.000000 healdata_utils-0.1.4a0/src/healdata_utils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-21 13:43:11.000000 healdata_utils-0.1.4a0/src/healdata_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-21 13:43:11.000000 healdata_utils-0.1.4a0/src/healdata_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:43:11.021076 healdata_utils-0.1.4a0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-07-21 13:43:01.000000 healdata_utils-0.1.4a0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10039 2023-07-21 13:43:01.000000 healdata_utils-0.1.4a0/tests/test_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-21 13:43:01.000000 healdata_utils-0.1.4a0/tests/test_utils.py
```

### Comparing `healdata_utils-0.1.3a0/PKG-INFO` & `healdata_utils-0.1.4a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: healdata_utils
-Version: 0.1.3a0
+Version: 0.1.4a0
 Summary: Data packaging tools for the HEAL data ecosystem
 Home-page: https://github.com/norc-heal/healdata-utils
 Author: Michael Kranz
 Author-email: kranz-michael@norc.org
 Description-Content-Type: text/markdown
 
 --8<-- [start:intro]
```

### Comparing `healdata_utils-0.1.3a0/README.md` & `healdata_utils-0.1.4a0/README.md`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.1.3a0/setup.py` & `healdata_utils-0.1.4a0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 charset_normalizer==2.1
 visions== 0.7.5
 click==8.1.3'''
 
 
 setup(
     name='healdata_utils',
-    version='0.1.3-alpha',
+    version='0.1.4-alpha',
     author='Michael Kranz',
     author_email='kranz-michael@norc.org',
     long_description=generate_long_description(),
     long_description_content_type="text/markdown",    
     description='Data packaging tools for the HEAL data ecosystem',
     #TODO: change url to HEAL once migrated.
     url='https://github.com/norc-heal/healdata-utils',
```

### Comparing `healdata_utils-0.1.3a0/src/healdata_utils/cli.py` & `healdata_utils-0.1.4a0/src/healdata_utils/cli.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.1.3a0/src/healdata_utils/io.py` & `healdata_utils-0.1.4a0/src/healdata_utils/io.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.1.3a0/src/healdata_utils/schemas.py` & `healdata_utils-0.1.4a0/src/healdata_utils/schemas.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.1.3a0/src/healdata_utils/transforms/csvdata/conversion.py` & `healdata_utils-0.1.4a0/src/healdata_utils/transforms/csvdata/conversion.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.1.3a0/src/healdata_utils/transforms/csvtemplate/conversion.py` & `healdata_utils-0.1.4a0/src/healdata_utils/transforms/csvtemplate/conversion.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.1.3a0/src/healdata_utils/transforms/csvtemplate/mappings.py` & `healdata_utils-0.1.4a0/src/healdata_utils/transforms/csvtemplate/mappings.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.1.3a0/src/healdata_utils/transforms/frictionless/conversion.py` & `healdata_utils-0.1.4a0/src/healdata_utils/transforms/frictionless/conversion.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.1.3a0/src/healdata_utils/transforms/jsontemplate/conversion.py` & `healdata_utils-0.1.4a0/src/healdata_utils/transforms/jsontemplate/conversion.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.1.3a0/src/healdata_utils/transforms/jsontemplate/mappings.py` & `healdata_utils-0.1.4a0/src/healdata_utils/transforms/jsontemplate/mappings.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.1.3a0/src/healdata_utils/transforms/readstat/conversion.py` & `healdata_utils-0.1.4a0/src/healdata_utils/transforms/readstat/conversion.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         representing user defined missing values in SAS and STATA. 
         This appears when using user_missing=True in read_sas7bdat or read_dta 
         if user defined missing values are present.
 
     """
     metaparams = dict(file_path=file_path,user_missing=True)
     if sas7bcat_file_path:
-        params["catalog_file"] = sas7bcat_file_path
+        metaparams["catalog_file"] = sas7bcat_file_path
     _,meta = read_pyreadstat(**metaparams) # get user missing values (for stata/sas will make string so need sep call to infer types)
     df,_ = read_pyreadstat(file_path) # dont fill user defined missing vals (to get correct types)
     fields = typesets.infer_frictionless_fields(df)
 
     for field in fields:
         field.pop('extDtype',None)
         fieldname = field['name']
```

### Comparing `healdata_utils-0.1.3a0/src/healdata_utils/transforms/redcapcsv/conversion.py` & `healdata_utils-0.1.4a0/src/healdata_utils/transforms/redcapcsv/conversion.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.1.3a0/src/healdata_utils/transforms/redcapcsv/headers.py` & `healdata_utils-0.1.4a0/src/healdata_utils/transforms/redcapcsv/headers.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.1.3a0/src/healdata_utils/transforms/redcapcsv/mappings.py` & `healdata_utils-0.1.4a0/src/healdata_utils/transforms/redcapcsv/mappings.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.1.3a0/src/healdata_utils/transforms/redcapcsv/schema.py` & `healdata_utils-0.1.4a0/src/healdata_utils/transforms/redcapcsv/schema.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.1.3a0/src/healdata_utils/types/typesets.py` & `healdata_utils-0.1.4a0/src/healdata_utils/types/typesets.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.1.3a0/src/healdata_utils/utils.py` & `healdata_utils-0.1.4a0/src/healdata_utils/utils.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.1.3a0/src/healdata_utils/validators/jsonschema.py` & `healdata_utils-0.1.4a0/src/healdata_utils/validators/jsonschema.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.1.3a0/src/healdata_utils/validators/validate.py` & `healdata_utils-0.1.4a0/src/healdata_utils/validators/validate.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.1.3a0/src/healdata_utils.egg-info/PKG-INFO` & `healdata_utils-0.1.4a0/src/healdata_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: healdata-utils
-Version: 0.1.3a0
+Version: 0.1.4a0
 Summary: Data packaging tools for the HEAL data ecosystem
 Home-page: https://github.com/norc-heal/healdata-utils
 Author: Michael Kranz
 Author-email: kranz-michael@norc.org
 Description-Content-Type: text/markdown
 
 --8<-- [start:intro]
```

### Comparing `healdata_utils-0.1.3a0/src/healdata_utils.egg-info/SOURCES.txt` & `healdata_utils-0.1.4a0/src/healdata_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.1.3a0/tests/test_cli.py` & `healdata_utils-0.1.4a0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.1.3a0/tests/test_schemas.py` & `healdata_utils-0.1.4a0/tests/test_schemas.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.1.3a0/tests/test_utils.py` & `healdata_utils-0.1.4a0/tests/test_utils.py`

 * *Files identical despite different names*

