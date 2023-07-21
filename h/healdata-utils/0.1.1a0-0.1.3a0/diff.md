# Comparing `tmp/healdata_utils-0.1.1a0.tar.gz` & `tmp/healdata_utils-0.1.3a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "healdata_utils-0.1.1a0.tar", last modified: Wed Jul 12 02:11:32 2023, max compression
+gzip compressed data, was "healdata_utils-0.1.3a0.tar", last modified: Fri Jul 21 03:58:36 2023, max compression
```

## Comparing `healdata_utils-0.1.1a0.tar` & `healdata_utils-0.1.3a0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 02:11:32.970311 healdata_utils-0.1.1a0/
--rw-r--r--   0 runner    (1001) docker     (123)     6252 2023-07-12 02:11:32.970311 healdata_utils-0.1.1a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5978 2023-07-12 02:11:19.000000 healdata_utils-0.1.1a0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 02:11:32.970311 healdata_utils-0.1.1a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-12 02:11:19.000000 healdata_utils-0.1.1a0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 02:11:32.958311 healdata_utils-0.1.1a0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 02:11:32.962311 healdata_utils-0.1.1a0/src/healdata_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 02:11:19.000000 healdata_utils-0.1.1a0/src/healdata_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8569 2023-07-12 02:11:19.000000 healdata_utils-0.1.1a0/src/healdata_utils/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-07-12 02:11:19.000000 healdata_utils-0.1.1a0/src/healdata_utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-07-12 02:11:19.000000 healdata_utils-0.1.1a0/src/healdata_utils/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 02:11:32.962311 healdata_utils-0.1.1a0/src/healdata_utils/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 02:11:19.000000 healdata_utils-0.1.1a0/src/healdata_utils/transforms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 02:11:32.962311 healdata_utils-0.1.1a0/src/healdata_utils/transforms/csvdata/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-12 02:11:19.000000 healdata_utils-0.1.1a0/src/healdata_utils/transforms/csvdata/conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 02:11:32.966311 healdata_utils-0.1.1a0/src/healdata_utils/transforms/csvtemplate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 02:11:19.000000 healdata_utils-0.1.1a0/src/healdata_utils/transforms/csvtemplate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-07-12 02:11:19.000000 healdata_utils-0.1.1a0/src/healdata_utils/transforms/csvtemplate/conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     3576 2023-07-12 02:11:19.000000 healdata_utils-0.1.1a0/src/healdata_utils/transforms/csvtemplate/mappings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 02:11:32.966311 healdata_utils-0.1.1a0/src/healdata_utils/transforms/frictionless/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-12 02:11:19.000000 healdata_utils-0.1.1a0/src/healdata_utils/transforms/frictionless/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-07-12 02:11:19.000000 healdata_utils-0.1.1a0/src/healdata_utils/transforms/frictionless/conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 02:11:32.966311 healdata_utils-0.1.1a0/src/healdata_utils/transforms/jsontemplate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 02:11:19.000000 healdata_utils-0.1.1a0/src/healdata_utils/transforms/jsontemplate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-07-12 02:11:19.000000 healdata_utils-0.1.1a0/src/healdata_utils/transforms/jsontemplate/conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-07-12 02:11:19.000000 healdata_utils-0.1.1a0/src/healdata_utils/transforms/jsontemplate/mappings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 02:11:32.966311 healdata_utils-0.1.1a0/src/healdata_utils/transforms/readstat/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 02:11:19.000000 healdata_utils-0.1.1a0/src/healdata_utils/transforms/readstat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-07-12 02:11:19.000000 healdata_utils-0.1.1a0/src/healdata_utils/transforms/readstat/conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 02:11:32.966311 healdata_utils-0.1.1a0/src/healdata_utils/transforms/redcapcsv/
--rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-07-12 02:11:19.000000 healdata_utils-0.1.1a0/src/healdata_utils/transforms/redcapcsv/conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-07-12 02:11:19.000000 healdata_utils-0.1.1a0/src/healdata_utils/transforms/redcapcsv/headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8786 2023-07-12 02:11:19.000000 healdata_utils-0.1.1a0/src/healdata_utils/transforms/redcapcsv/mappings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-07-12 02:11:19.000000 healdata_utils-0.1.1a0/src/healdata_utils/transforms/redcapcsv/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 02:11:32.966311 healdata_utils-0.1.1a0/src/healdata_utils/types/
--rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-07-12 02:11:19.000000 healdata_utils-0.1.1a0/src/healdata_utils/types/typesets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-07-12 02:11:19.000000 healdata_utils-0.1.1a0/src/healdata_utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 02:11:32.966311 healdata_utils-0.1.1a0/src/healdata_utils/validators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 02:11:19.000000 healdata_utils-0.1.1a0/src/healdata_utils/validators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-12 02:11:19.000000 healdata_utils-0.1.1a0/src/healdata_utils/validators/frictionless.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-12 02:11:19.000000 healdata_utils-0.1.1a0/src/healdata_utils/validators/jsonschema.py
--rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-07-12 02:11:19.000000 healdata_utils-0.1.1a0/src/healdata_utils/validators/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 02:11:32.962311 healdata_utils-0.1.1a0/src/healdata_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6252 2023-07-12 02:11:32.000000 healdata_utils-0.1.1a0/src/healdata_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-07-12 02:11:32.000000 healdata_utils-0.1.1a0/src/healdata_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 02:11:32.000000 healdata_utils-0.1.1a0/src/healdata_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-12 02:11:32.000000 healdata_utils-0.1.1a0/src/healdata_utils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-12 02:11:32.000000 healdata_utils-0.1.1a0/src/healdata_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-12 02:11:32.000000 healdata_utils-0.1.1a0/src/healdata_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 02:11:32.966311 healdata_utils-0.1.1a0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-07-12 02:11:19.000000 healdata_utils-0.1.1a0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    10039 2023-07-12 02:11:19.000000 healdata_utils-0.1.1a0/tests/test_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-12 02:11:19.000000 healdata_utils-0.1.1a0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 03:58:36.090678 healdata_utils-0.1.3a0/
+-rw-r--r--   0 runner    (1001) docker     (123)     6186 2023-07-21 03:58:36.090678 healdata_utils-0.1.3a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5912 2023-07-21 03:58:26.000000 healdata_utils-0.1.3a0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 03:58:36.090678 healdata_utils-0.1.3a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-21 03:58:27.000000 healdata_utils-0.1.3a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 03:58:36.082678 healdata_utils-0.1.3a0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 03:58:36.086678 healdata_utils-0.1.3a0/src/healdata_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 03:58:27.000000 healdata_utils-0.1.3a0/src/healdata_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8569 2023-07-21 03:58:27.000000 healdata_utils-0.1.3a0/src/healdata_utils/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-07-21 03:58:27.000000 healdata_utils-0.1.3a0/src/healdata_utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-07-21 03:58:27.000000 healdata_utils-0.1.3a0/src/healdata_utils/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 03:58:36.086678 healdata_utils-0.1.3a0/src/healdata_utils/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 03:58:27.000000 healdata_utils-0.1.3a0/src/healdata_utils/transforms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 03:58:36.086678 healdata_utils-0.1.3a0/src/healdata_utils/transforms/csvdata/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-21 03:58:27.000000 healdata_utils-0.1.3a0/src/healdata_utils/transforms/csvdata/conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 03:58:36.086678 healdata_utils-0.1.3a0/src/healdata_utils/transforms/csvtemplate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 03:58:27.000000 healdata_utils-0.1.3a0/src/healdata_utils/transforms/csvtemplate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-07-21 03:58:27.000000 healdata_utils-0.1.3a0/src/healdata_utils/transforms/csvtemplate/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3576 2023-07-21 03:58:27.000000 healdata_utils-0.1.3a0/src/healdata_utils/transforms/csvtemplate/mappings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 03:58:36.086678 healdata_utils-0.1.3a0/src/healdata_utils/transforms/frictionless/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-21 03:58:27.000000 healdata_utils-0.1.3a0/src/healdata_utils/transforms/frictionless/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-07-21 03:58:27.000000 healdata_utils-0.1.3a0/src/healdata_utils/transforms/frictionless/conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 03:58:36.086678 healdata_utils-0.1.3a0/src/healdata_utils/transforms/jsontemplate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 03:58:27.000000 healdata_utils-0.1.3a0/src/healdata_utils/transforms/jsontemplate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-07-21 03:58:27.000000 healdata_utils-0.1.3a0/src/healdata_utils/transforms/jsontemplate/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-07-21 03:58:27.000000 healdata_utils-0.1.3a0/src/healdata_utils/transforms/jsontemplate/mappings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 03:58:36.086678 healdata_utils-0.1.3a0/src/healdata_utils/transforms/readstat/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 03:58:27.000000 healdata_utils-0.1.3a0/src/healdata_utils/transforms/readstat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-07-21 03:58:27.000000 healdata_utils-0.1.3a0/src/healdata_utils/transforms/readstat/conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 03:58:36.086678 healdata_utils-0.1.3a0/src/healdata_utils/transforms/redcapcsv/
+-rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-07-21 03:58:27.000000 healdata_utils-0.1.3a0/src/healdata_utils/transforms/redcapcsv/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-07-21 03:58:27.000000 healdata_utils-0.1.3a0/src/healdata_utils/transforms/redcapcsv/headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8786 2023-07-21 03:58:27.000000 healdata_utils-0.1.3a0/src/healdata_utils/transforms/redcapcsv/mappings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-07-21 03:58:27.000000 healdata_utils-0.1.3a0/src/healdata_utils/transforms/redcapcsv/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 03:58:36.086678 healdata_utils-0.1.3a0/src/healdata_utils/types/
+-rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-07-21 03:58:27.000000 healdata_utils-0.1.3a0/src/healdata_utils/types/typesets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-07-21 03:58:27.000000 healdata_utils-0.1.3a0/src/healdata_utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 03:58:36.090678 healdata_utils-0.1.3a0/src/healdata_utils/validators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 03:58:27.000000 healdata_utils-0.1.3a0/src/healdata_utils/validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-21 03:58:27.000000 healdata_utils-0.1.3a0/src/healdata_utils/validators/frictionless.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-21 03:58:27.000000 healdata_utils-0.1.3a0/src/healdata_utils/validators/jsonschema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-07-21 03:58:27.000000 healdata_utils-0.1.3a0/src/healdata_utils/validators/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 03:58:36.086678 healdata_utils-0.1.3a0/src/healdata_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6186 2023-07-21 03:58:36.000000 healdata_utils-0.1.3a0/src/healdata_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-07-21 03:58:36.000000 healdata_utils-0.1.3a0/src/healdata_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 03:58:36.000000 healdata_utils-0.1.3a0/src/healdata_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-21 03:58:36.000000 healdata_utils-0.1.3a0/src/healdata_utils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-21 03:58:36.000000 healdata_utils-0.1.3a0/src/healdata_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-21 03:58:36.000000 healdata_utils-0.1.3a0/src/healdata_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 03:58:36.090678 healdata_utils-0.1.3a0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-07-21 03:58:27.000000 healdata_utils-0.1.3a0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10039 2023-07-21 03:58:27.000000 healdata_utils-0.1.3a0/tests/test_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-21 03:58:27.000000 healdata_utils-0.1.3a0/tests/test_utils.py
```

### Comparing `healdata_utils-0.1.1a0/PKG-INFO` & `healdata_utils-0.1.3a0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,41 +1,37 @@
-Metadata-Version: 2.1
-Name: healdata_utils
-Version: 0.1.1a0
-Summary: Data packaging tools for the HEAL data ecosystem
-Home-page: https://github.com/norc-heal/healdata-utils
-Author: Michael Kranz
-Author-email: kranz-michael@norc.org
-Description-Content-Type: text/markdown
-
 --8<-- [start:intro]
 
 # HEAL Data Utilities
 
-The HEAL data utilities python package provides data packaging tools for the HEAL data ecosystem to facilitate data discovery,sharing, and harmonization with a focus on the HEAL platform data consultancy (DSC).
+The HEAL Data Utilities python package provides data packaging tools for the HEAL Data Ecosystem to facilitate data discovery, sharing, and harmonization with a focus on the HEAL Platform Data Consultancy (DSC).
  
-Currently, the focus of the repo is on generating data-dictionaries (see Variable level metadata section below). However, in the future, this will be expanded for all heal specific data packaging functions (e.g., study and file level metadata and data).
+Currently, the focus of this repository is generating data dictionaries (see Variable-level Metadata section below). However, in the future, this will be expanded for all HEAL-specific data packaging functions (e.g., study- and file-level metadata and data).
 
 ## Installation
 
 To install the latest official release of healdata-utils, from your computer's command prompt, run:
 
 `pip install healdata-utils --pre` (**NOTE: currently in pre-lease**)
 
 `pip install git+https://github.com/norc-heal/healdata-utils.git`
 
 
-## Variable level metadata (data dictionaries)
+--8<-- [end:intro]
+
+
+--8<-- [start:vlmd-intro]
+## Variable-level Metadata (Data Dictionaries)
 
 [![Binder](http://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/norc-heal/healdata-utils/HEAD?labpath=notebooks%2Fdemos%2Finputs-to-heal-data-dictionary.ipynb) 
 
-The healdata-utils variable level metadata (vlmd) tool inputs a variety of different input file types and exports HEAL-formatted data dictionaries (JSON and CSV formats). Additionally, exported validation (ie "error") reports provide the user information as to a. if the exported data dictionary is valid according to HEAL specifications (see the schema repository [here](https://github.com/norc-heal/heal-metadata-schemas/tree/main/variable-level-metadata-schema)).
+The healdata-utils variable-level metadata (vlmd) tool inputs a variety of different input file types and exports HEAL-compliant data dictionaries (JSON and CSV formats). Additionally, exported validation (i.e., "error") reports provide the user information as to a) if the exported data dictionary is valid according to HEAL specifications and b) how to modify one's data dictionary to make it HEAL-compliant.
 
-For support formats and more detailed software specific instructions and recommendations, [see here](docs/supported_input_formats.md)
+--8<-- [end:vlmd-intro]
 
+--8<-- [start:vlmd-basic-usage]
 ### Basic usage 
 
 The vlmd tool can be used via python or the command line.
 
 #### Using from python
 
 From your current working directory in python, run:
@@ -53,44 +49,44 @@
     filepath=inputpath,
     outputdir=healdir, 
     inputtype=input_type, #if not specified, looks for suffix
     data_dictionary_props={"title":title,"description":description} #data_dictionary_props is optional
 )
 ```
 
-> This will output the data dictionaries to the specified output directory (see ooutput section below) and also save the json/csv versions in the `data_dictionaries` object.
+> This will output the data dictionaries to the specified output directory (see output section below) and also save the json/csv versions in the `data_dictionaries` object.
 
-> For the available input file formats (ie the available choices for the `inputtype` parameter), one can run (from python):
+> For the available input file formats (i.e., the available choices for the `inputtype` parameter), one can run (from python):
 
 ```python
 from healdata_utils.cli import input_descriptions
 
 input_descriptions
 
 ```
 
 The `input_descriptions` object contains the choice for `inputtype` as the key and the description as the value.
 
 #### Using from the command line
 
 From your current working directory run:
-(note the `\` at the end of each line signals a line continuation for ease in understanding the long one line command.) Again the `--title` and `--description` options are optional.
+(note the `\` at the end of each line signals a line continuation for ease in understanding the long, one-line command.) Again, the `--title` and `--description` options are optional.
 For descriptions on the different flags/options, run `vlmd --help`
 
 ```bash
 
 vlmd --filepath "data/example_pyreadstat_output.sav" \
 --outputdir "output-cli" \
 --title "Healdata-utils Demonstration Data Dictionary" \
 --description "This is a proof of concept to demonstrate the healdata-utils functionality" 
 ```
 
 #### Output
 
-Both the python and command line routes will result in a JSON and CSV version of the HEAL  data dictionary in the output folder along with the validation reports in the `errors` folder. See below:
+Both the python and command line routes will result in a JSON and CSV version of the HEAL data dictionary in the output folder along with the validation reports in the `errors` folder. See below:
 
 - `input/input/my-redcap-data-dictionary-export.csv` : your input file
 
 - `output/errors/heal-csv-errors.json`: outputted validation report for table in csv file against frictionless schema
     - see schema [here](https://github.com/norc-heal/heal-metadata-schemas/blob/main/variable-level-metadata-schema/schemas/frictionless/csvtemplate/fields.json)
 - `output/errors/heal-json-errors.json`:  outputted jsonschema validation report.
     - see schema [here](https://github.com/norc-heal/heal-metadata-schemas/blob/main/variable-level-metadata-schema/schemas/jsonschema/data-dictionary.json)
@@ -117,8 +113,9 @@
 1. Generating a heal data dictionary from a variety of input files 
 
 - [click here for static notebook ](notebooks/demos/inputs-to-heal-data-dictionary.ipynb) 
 - click binder badge for interactive [![Binder](http://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/norc-heal/healdata-utils/HEAD?labpath=notebooks%2Fdemos%2Finputs-to-heal-data-dictionary.ipynb) 
 
 2. [in development] Creating and iterating over a csv data dictionary to create a valid data dictionary file [click here](notebooks/demos/demo-csvtemplate-validation.ipynb)
 
---8<-- [end:intro]
+
+--8<-- [end:vlmd-basic-usage]
```

### Comparing `healdata_utils-0.1.1a0/README.md` & `healdata_utils-0.1.3a0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,32 +1,46 @@
+Metadata-Version: 2.1
+Name: healdata_utils
+Version: 0.1.3a0
+Summary: Data packaging tools for the HEAL data ecosystem
+Home-page: https://github.com/norc-heal/healdata-utils
+Author: Michael Kranz
+Author-email: kranz-michael@norc.org
+Description-Content-Type: text/markdown
+
 --8<-- [start:intro]
 
 # HEAL Data Utilities
 
-The HEAL data utilities python package provides data packaging tools for the HEAL data ecosystem to facilitate data discovery,sharing, and harmonization with a focus on the HEAL platform data consultancy (DSC).
+The HEAL Data Utilities python package provides data packaging tools for the HEAL Data Ecosystem to facilitate data discovery, sharing, and harmonization with a focus on the HEAL Platform Data Consultancy (DSC).
  
-Currently, the focus of the repo is on generating data-dictionaries (see Variable level metadata section below). However, in the future, this will be expanded for all heal specific data packaging functions (e.g., study and file level metadata and data).
+Currently, the focus of this repository is generating data dictionaries (see Variable-level Metadata section below). However, in the future, this will be expanded for all HEAL-specific data packaging functions (e.g., study- and file-level metadata and data).
 
 ## Installation
 
 To install the latest official release of healdata-utils, from your computer's command prompt, run:
 
 `pip install healdata-utils --pre` (**NOTE: currently in pre-lease**)
 
 `pip install git+https://github.com/norc-heal/healdata-utils.git`
 
 
-## Variable level metadata (data dictionaries)
+--8<-- [end:intro]
+
+
+--8<-- [start:vlmd-intro]
+## Variable-level Metadata (Data Dictionaries)
 
 [![Binder](http://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/norc-heal/healdata-utils/HEAD?labpath=notebooks%2Fdemos%2Finputs-to-heal-data-dictionary.ipynb) 
 
-The healdata-utils variable level metadata (vlmd) tool inputs a variety of different input file types and exports HEAL-formatted data dictionaries (JSON and CSV formats). Additionally, exported validation (ie "error") reports provide the user information as to a. if the exported data dictionary is valid according to HEAL specifications (see the schema repository [here](https://github.com/norc-heal/heal-metadata-schemas/tree/main/variable-level-metadata-schema)).
+The healdata-utils variable-level metadata (vlmd) tool inputs a variety of different input file types and exports HEAL-compliant data dictionaries (JSON and CSV formats). Additionally, exported validation (i.e., "error") reports provide the user information as to a) if the exported data dictionary is valid according to HEAL specifications and b) how to modify one's data dictionary to make it HEAL-compliant.
 
-For support formats and more detailed software specific instructions and recommendations, [see here](docs/supported_input_formats.md)
+--8<-- [end:vlmd-intro]
 
+--8<-- [start:vlmd-basic-usage]
 ### Basic usage 
 
 The vlmd tool can be used via python or the command line.
 
 #### Using from python
 
 From your current working directory in python, run:
@@ -44,44 +58,44 @@
     filepath=inputpath,
     outputdir=healdir, 
     inputtype=input_type, #if not specified, looks for suffix
     data_dictionary_props={"title":title,"description":description} #data_dictionary_props is optional
 )
 ```
 
-> This will output the data dictionaries to the specified output directory (see ooutput section below) and also save the json/csv versions in the `data_dictionaries` object.
+> This will output the data dictionaries to the specified output directory (see output section below) and also save the json/csv versions in the `data_dictionaries` object.
 
-> For the available input file formats (ie the available choices for the `inputtype` parameter), one can run (from python):
+> For the available input file formats (i.e., the available choices for the `inputtype` parameter), one can run (from python):
 
 ```python
 from healdata_utils.cli import input_descriptions
 
 input_descriptions
 
 ```
 
 The `input_descriptions` object contains the choice for `inputtype` as the key and the description as the value.
 
 #### Using from the command line
 
 From your current working directory run:
-(note the `\` at the end of each line signals a line continuation for ease in understanding the long one line command.) Again the `--title` and `--description` options are optional.
+(note the `\` at the end of each line signals a line continuation for ease in understanding the long, one-line command.) Again, the `--title` and `--description` options are optional.
 For descriptions on the different flags/options, run `vlmd --help`
 
 ```bash
 
 vlmd --filepath "data/example_pyreadstat_output.sav" \
 --outputdir "output-cli" \
 --title "Healdata-utils Demonstration Data Dictionary" \
 --description "This is a proof of concept to demonstrate the healdata-utils functionality" 
 ```
 
 #### Output
 
-Both the python and command line routes will result in a JSON and CSV version of the HEAL  data dictionary in the output folder along with the validation reports in the `errors` folder. See below:
+Both the python and command line routes will result in a JSON and CSV version of the HEAL data dictionary in the output folder along with the validation reports in the `errors` folder. See below:
 
 - `input/input/my-redcap-data-dictionary-export.csv` : your input file
 
 - `output/errors/heal-csv-errors.json`: outputted validation report for table in csv file against frictionless schema
     - see schema [here](https://github.com/norc-heal/heal-metadata-schemas/blob/main/variable-level-metadata-schema/schemas/frictionless/csvtemplate/fields.json)
 - `output/errors/heal-json-errors.json`:  outputted jsonschema validation report.
     - see schema [here](https://github.com/norc-heal/heal-metadata-schemas/blob/main/variable-level-metadata-schema/schemas/jsonschema/data-dictionary.json)
@@ -108,8 +122,9 @@
 1. Generating a heal data dictionary from a variety of input files 
 
 - [click here for static notebook ](notebooks/demos/inputs-to-heal-data-dictionary.ipynb) 
 - click binder badge for interactive [![Binder](http://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/norc-heal/healdata-utils/HEAD?labpath=notebooks%2Fdemos%2Finputs-to-heal-data-dictionary.ipynb) 
 
 2. [in development] Creating and iterating over a csv data dictionary to create a valid data dictionary file [click here](notebooks/demos/demo-csvtemplate-validation.ipynb)
 
---8<-- [end:intro]
+
+--8<-- [end:vlmd-basic-usage]
```

### Comparing `healdata_utils-0.1.1a0/setup.py` & `healdata_utils-0.1.3a0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,39 @@
 from setuptools import setup, find_namespace_packages
 from pathlib import Path
+import os 
 
+os.chdir(Path(__file__).parent)
 def generate_long_description():
     return Path("README.md").read_text()
 
+def get_install_requirements():
+    return '''petl==1.7.12
+jsonschema==4.17.3
+requests==2.28.2
+PyYaml==6.0
+#frictionless==4.40.8
+pyreadstat==1.2.0
+charset_normalizer==2.1
+visions== 0.7.5
+click==8.1.3'''
+
 
 setup(
     name='healdata_utils',
-    version='0.1.1-alpha',
+    version='0.1.3-alpha',
     author='Michael Kranz',
     author_email='kranz-michael@norc.org',
     long_description=generate_long_description(),
     long_description_content_type="text/markdown",    
     description='Data packaging tools for the HEAL data ecosystem',
     #TODO: change url to HEAL once migrated.
     url='https://github.com/norc-heal/healdata-utils',
     package_dir={'': 'src'},
     packages=find_namespace_packages(where='src'),
-    install_requires=[
-        'petl==1.7.12',
-        'jsonschema==4.17.3',
-        'requests==2.28.2',
-        'PyYaml==6.0',
-        #'frictionless==4.40.8',
-        'pyreadstat==1.2.0',
-        'charset_normalizer==2.1',
-        'visions== 0.7.5',
-        "click==8.1.3"
-    ],
+    install_requires=get_install_requirements(),
     entry_points='''
         [console_scripts]
         vlmd=healdata_utils.cli:main
     '''
 
 )
```

### Comparing `healdata_utils-0.1.1a0/src/healdata_utils/cli.py` & `healdata_utils-0.1.3a0/src/healdata_utils/cli.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.1.1a0/src/healdata_utils/io.py` & `healdata_utils-0.1.3a0/src/healdata_utils/io.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.1.1a0/src/healdata_utils/schemas.py` & `healdata_utils-0.1.3a0/src/healdata_utils/schemas.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.1.1a0/src/healdata_utils/transforms/csvdata/conversion.py` & `healdata_utils-0.1.3a0/src/healdata_utils/transforms/csvdata/conversion.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.1.1a0/src/healdata_utils/transforms/csvtemplate/conversion.py` & `healdata_utils-0.1.3a0/src/healdata_utils/transforms/csvtemplate/conversion.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.1.1a0/src/healdata_utils/transforms/csvtemplate/mappings.py` & `healdata_utils-0.1.3a0/src/healdata_utils/transforms/csvtemplate/mappings.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.1.1a0/src/healdata_utils/transforms/frictionless/conversion.py` & `healdata_utils-0.1.3a0/src/healdata_utils/transforms/frictionless/conversion.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.1.1a0/src/healdata_utils/transforms/jsontemplate/conversion.py` & `healdata_utils-0.1.3a0/src/healdata_utils/transforms/jsontemplate/conversion.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,24 +4,28 @@
 from collections.abc import MutableMapping
 from .mappings import join_prop
 from healdata_utils.utils import flatten_except_if
 from os import PathLike
 
 def convert_templatejson(
     jsontemplate:str,
+    data_dictionary_props:dict=None,
     fields_name:str='data_dictionary',
     sep_iter = '|',
     sep_dict = '=',
     **kwargs
     ):
     """
     Converts a JSON file or dictionary conforming to HEAL specifications
     into a HEAL-specified data dictionary in both csv format and json format.
 
     Converts in-memory data or a path to a data dictionary file.
+
+    If data_dictionary_props is specified, any properties passed in will be
+    overwritten.
     
     Parameters
     ----------
     csvtemplate : str or path-like or an object that can be inferred as data by frictionless's Resource class.
         Data or path to data with the data being a tabular HEAL-specified data dictionary.
         This input can be any data object or path-like string excepted by a frictionless Resource object.
     data_dictionary_props : dict
@@ -33,24 +37,34 @@
     Returns
     -------
     dict
         A dictionary with two keys:
             - 'templatejson': the HEAL-specified JSON object.
             - 'templatecsv': the HEAL-specified tabular template.
 
+
+    TODO
+    ---------
+
+    Allow an array of fields to be passed in
+
     """
     if isinstance(jsontemplate,(str,PathLike)):
-        data_dictionary_props = json.loads(Path(jsontemplate).read_text())
+        jsontemplate_dict = json.loads(Path(jsontemplate).read_text())
     elif isinstance(jsontemplate, MutableMapping):
-        data_dictionary_props = jsontemplate
+        jsontemplate_dict = jsontemplate
     else:
         raise Exception("jsontemplate needs to be either dictionary-like or a path to a json")
 
+    if data_dictionary_props:
+        jsontemplate_dict.update(data_dictionary_props)
 
-    fields_json = data_dictionary_props.pop(fields_name)
+    fields_json = jsontemplate_dict.pop(fields_name)
+    data_dictionary_props = jsontemplate_dict
+    
     fields_csv = []
     for f in fields_json:
         field_flattened = flatten_except_if(f)
         field_csv = {
             propname:join_prop(propname,prop)
             for propname,prop in field_flattened.items()
         }
```

### Comparing `healdata_utils-0.1.1a0/src/healdata_utils/transforms/jsontemplate/mappings.py` & `healdata_utils-0.1.3a0/src/healdata_utils/transforms/jsontemplate/mappings.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.1.1a0/src/healdata_utils/transforms/readstat/conversion.py` & `healdata_utils-0.1.3a0/src/healdata_utils/transforms/readstat/conversion.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,16 +59,18 @@
         missing_user_values: a dict with keys being variable names. 
         Values are a list of character values (A to Z and _ for SAS, a to z for SATA) 
         representing user defined missing values in SAS and STATA. 
         This appears when using user_missing=True in read_sas7bdat or read_dta 
         if user defined missing values are present.
 
     """
-    
-    _,meta = read_pyreadstat(file_path,catalog_file=sas7bcat_file_path,user_missing=True) # get user missing values (for stata/sas will make string so need sep call to infer types)
+    metaparams = dict(file_path=file_path,user_missing=True)
+    if sas7bcat_file_path:
+        params["catalog_file"] = sas7bcat_file_path
+    _,meta = read_pyreadstat(**metaparams) # get user missing values (for stata/sas will make string so need sep call to infer types)
     df,_ = read_pyreadstat(file_path) # dont fill user defined missing vals (to get correct types)
     fields = typesets.infer_frictionless_fields(df)
 
     for field in fields:
         field.pop('extDtype',None)
         fieldname = field['name']
```

### Comparing `healdata_utils-0.1.1a0/src/healdata_utils/transforms/redcapcsv/conversion.py` & `healdata_utils-0.1.3a0/src/healdata_utils/transforms/redcapcsv/conversion.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.1.1a0/src/healdata_utils/transforms/redcapcsv/headers.py` & `healdata_utils-0.1.3a0/src/healdata_utils/transforms/redcapcsv/headers.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.1.1a0/src/healdata_utils/transforms/redcapcsv/mappings.py` & `healdata_utils-0.1.3a0/src/healdata_utils/transforms/redcapcsv/mappings.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.1.1a0/src/healdata_utils/transforms/redcapcsv/schema.py` & `healdata_utils-0.1.3a0/src/healdata_utils/transforms/redcapcsv/schema.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.1.1a0/src/healdata_utils/types/typesets.py` & `healdata_utils-0.1.3a0/src/healdata_utils/types/typesets.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,16 +93,16 @@
     # TODO: infer formats with extended dtypes (eg url, email etc)
     df,typepaths,_ = typeset.infer(df) # typepaths is list of the visions graph traversal - last item is casted type
     fields = []
 
     for col,typepath in typepaths.items():
         field = {"name":col}
         type_final = str(typepath[-1])
-        type_second_to_final = str(typepath[-2])
         if type_final=="Categorical":
+            type_second_to_final = str(typepath[-2])
             field["type"] = typeset_mapping.get(type_second_to_final,"any")
             # enums for inferred categoricals
             field["constraints"] = {"enum":list(df[col].cat.categories)}       
         else:
             field["type"] = typeset_mapping.get(str(type_final),"any")
 
         fields.append(field)
```

### Comparing `healdata_utils-0.1.1a0/src/healdata_utils/utils.py` & `healdata_utils-0.1.3a0/src/healdata_utils/utils.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.1.1a0/src/healdata_utils/validators/jsonschema.py` & `healdata_utils-0.1.3a0/src/healdata_utils/validators/jsonschema.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.1.1a0/src/healdata_utils/validators/validate.py` & `healdata_utils-0.1.3a0/src/healdata_utils/validators/validate.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.1.1a0/src/healdata_utils.egg-info/PKG-INFO` & `healdata_utils-0.1.3a0/src/healdata_utils.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,41 +1,46 @@
 Metadata-Version: 2.1
 Name: healdata-utils
-Version: 0.1.1a0
+Version: 0.1.3a0
 Summary: Data packaging tools for the HEAL data ecosystem
 Home-page: https://github.com/norc-heal/healdata-utils
 Author: Michael Kranz
 Author-email: kranz-michael@norc.org
 Description-Content-Type: text/markdown
 
 --8<-- [start:intro]
 
 # HEAL Data Utilities
 
-The HEAL data utilities python package provides data packaging tools for the HEAL data ecosystem to facilitate data discovery,sharing, and harmonization with a focus on the HEAL platform data consultancy (DSC).
+The HEAL Data Utilities python package provides data packaging tools for the HEAL Data Ecosystem to facilitate data discovery, sharing, and harmonization with a focus on the HEAL Platform Data Consultancy (DSC).
  
-Currently, the focus of the repo is on generating data-dictionaries (see Variable level metadata section below). However, in the future, this will be expanded for all heal specific data packaging functions (e.g., study and file level metadata and data).
+Currently, the focus of this repository is generating data dictionaries (see Variable-level Metadata section below). However, in the future, this will be expanded for all HEAL-specific data packaging functions (e.g., study- and file-level metadata and data).
 
 ## Installation
 
 To install the latest official release of healdata-utils, from your computer's command prompt, run:
 
 `pip install healdata-utils --pre` (**NOTE: currently in pre-lease**)
 
 `pip install git+https://github.com/norc-heal/healdata-utils.git`
 
 
-## Variable level metadata (data dictionaries)
+--8<-- [end:intro]
+
+
+--8<-- [start:vlmd-intro]
+## Variable-level Metadata (Data Dictionaries)
 
 [![Binder](http://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/norc-heal/healdata-utils/HEAD?labpath=notebooks%2Fdemos%2Finputs-to-heal-data-dictionary.ipynb) 
 
-The healdata-utils variable level metadata (vlmd) tool inputs a variety of different input file types and exports HEAL-formatted data dictionaries (JSON and CSV formats). Additionally, exported validation (ie "error") reports provide the user information as to a. if the exported data dictionary is valid according to HEAL specifications (see the schema repository [here](https://github.com/norc-heal/heal-metadata-schemas/tree/main/variable-level-metadata-schema)).
+The healdata-utils variable-level metadata (vlmd) tool inputs a variety of different input file types and exports HEAL-compliant data dictionaries (JSON and CSV formats). Additionally, exported validation (i.e., "error") reports provide the user information as to a) if the exported data dictionary is valid according to HEAL specifications and b) how to modify one's data dictionary to make it HEAL-compliant.
 
-For support formats and more detailed software specific instructions and recommendations, [see here](docs/supported_input_formats.md)
+--8<-- [end:vlmd-intro]
 
+--8<-- [start:vlmd-basic-usage]
 ### Basic usage 
 
 The vlmd tool can be used via python or the command line.
 
 #### Using from python
 
 From your current working directory in python, run:
@@ -53,44 +58,44 @@
     filepath=inputpath,
     outputdir=healdir, 
     inputtype=input_type, #if not specified, looks for suffix
     data_dictionary_props={"title":title,"description":description} #data_dictionary_props is optional
 )
 ```
 
-> This will output the data dictionaries to the specified output directory (see ooutput section below) and also save the json/csv versions in the `data_dictionaries` object.
+> This will output the data dictionaries to the specified output directory (see output section below) and also save the json/csv versions in the `data_dictionaries` object.
 
-> For the available input file formats (ie the available choices for the `inputtype` parameter), one can run (from python):
+> For the available input file formats (i.e., the available choices for the `inputtype` parameter), one can run (from python):
 
 ```python
 from healdata_utils.cli import input_descriptions
 
 input_descriptions
 
 ```
 
 The `input_descriptions` object contains the choice for `inputtype` as the key and the description as the value.
 
 #### Using from the command line
 
 From your current working directory run:
-(note the `\` at the end of each line signals a line continuation for ease in understanding the long one line command.) Again the `--title` and `--description` options are optional.
+(note the `\` at the end of each line signals a line continuation for ease in understanding the long, one-line command.) Again, the `--title` and `--description` options are optional.
 For descriptions on the different flags/options, run `vlmd --help`
 
 ```bash
 
 vlmd --filepath "data/example_pyreadstat_output.sav" \
 --outputdir "output-cli" \
 --title "Healdata-utils Demonstration Data Dictionary" \
 --description "This is a proof of concept to demonstrate the healdata-utils functionality" 
 ```
 
 #### Output
 
-Both the python and command line routes will result in a JSON and CSV version of the HEAL  data dictionary in the output folder along with the validation reports in the `errors` folder. See below:
+Both the python and command line routes will result in a JSON and CSV version of the HEAL data dictionary in the output folder along with the validation reports in the `errors` folder. See below:
 
 - `input/input/my-redcap-data-dictionary-export.csv` : your input file
 
 - `output/errors/heal-csv-errors.json`: outputted validation report for table in csv file against frictionless schema
     - see schema [here](https://github.com/norc-heal/heal-metadata-schemas/blob/main/variable-level-metadata-schema/schemas/frictionless/csvtemplate/fields.json)
 - `output/errors/heal-json-errors.json`:  outputted jsonschema validation report.
     - see schema [here](https://github.com/norc-heal/heal-metadata-schemas/blob/main/variable-level-metadata-schema/schemas/jsonschema/data-dictionary.json)
@@ -117,8 +122,9 @@
 1. Generating a heal data dictionary from a variety of input files 
 
 - [click here for static notebook ](notebooks/demos/inputs-to-heal-data-dictionary.ipynb) 
 - click binder badge for interactive [![Binder](http://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/norc-heal/healdata-utils/HEAD?labpath=notebooks%2Fdemos%2Finputs-to-heal-data-dictionary.ipynb) 
 
 2. [in development] Creating and iterating over a csv data dictionary to create a valid data dictionary file [click here](notebooks/demos/demo-csvtemplate-validation.ipynb)
 
---8<-- [end:intro]
+
+--8<-- [end:vlmd-basic-usage]
```

### Comparing `healdata_utils-0.1.1a0/src/healdata_utils.egg-info/SOURCES.txt` & `healdata_utils-0.1.3a0/src/healdata_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.1.1a0/tests/test_cli.py` & `healdata_utils-0.1.3a0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.1.1a0/tests/test_schemas.py` & `healdata_utils-0.1.3a0/tests/test_schemas.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.1.1a0/tests/test_utils.py` & `healdata_utils-0.1.3a0/tests/test_utils.py`

 * *Files identical despite different names*

