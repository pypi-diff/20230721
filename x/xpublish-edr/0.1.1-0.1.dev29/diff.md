# Comparing `tmp/xpublish_edr-0.1.1.tar.gz` & `tmp/xpublish_edr-0.1.dev29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xpublish_edr-0.1.1.tar", last modified: Fri Jul 21 16:57:13 2023, max compression
+gzip compressed data, was "xpublish_edr-0.1.dev29.tar", last modified: Thu May 11 20:52:52 2023, max compression
```

## Comparing `xpublish_edr-0.1.1.tar` & `xpublish_edr-0.1.dev29.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:57:13.249152 xpublish_edr-0.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:57:13.245151 xpublish_edr-0.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:57:13.249152 xpublish_edr-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-21 16:56:58.000000 xpublish_edr-0.1.1/.github/workflows/pre-commit.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-07-21 16:56:58.000000 xpublish_edr-0.1.1/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-07-21 16:56:58.000000 xpublish_edr-0.1.1/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-07-21 16:56:58.000000 xpublish_edr-0.1.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-21 16:56:58.000000 xpublish_edr-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-07-21 16:57:13.249152 xpublish_edr-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-07-21 16:56:58.000000 xpublish_edr-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-07-21 16:56:58.000000 xpublish_edr-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-21 16:56:58.000000 xpublish_edr-0.1.1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 16:56:58.000000 xpublish_edr-0.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 16:57:13.249152 xpublish_edr-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:57:13.249152 xpublish_edr-0.1.1/xpublish_edr/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-21 16:56:58.000000 xpublish_edr-0.1.1/xpublish_edr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-21 16:57:13.000000 xpublish_edr-0.1.1/xpublish_edr/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:57:13.249152 xpublish_edr-0.1.1/xpublish_edr/formats/
--rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-07-21 16:56:58.000000 xpublish_edr-0.1.1/xpublish_edr/formats/to_covjson.py
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-21 16:56:58.000000 xpublish_edr-0.1.1/xpublish_edr/formats/to_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-21 16:56:58.000000 xpublish_edr-0.1.1/xpublish_edr/formats/to_netcdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-07-21 16:56:58.000000 xpublish_edr-0.1.1/xpublish_edr/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-07-21 16:56:58.000000 xpublish_edr-0.1.1/xpublish_edr/query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:57:13.249152 xpublish_edr-0.1.1/xpublish_edr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-21 16:57:13.000000 xpublish_edr-0.1.1/xpublish_edr.egg-info/SOURCES.txt
+drwxr-xr-x   0 akerney    (502) staff       (20)        0 2023-05-11 20:52:52.427673 xpublish_edr-0.1.dev29/
+drwxr-xr-x   0 akerney    (502) staff       (20)        0 2023-05-11 20:52:52.419377 xpublish_edr-0.1.dev29/.github/
+drwxr-xr-x   0 akerney    (502) staff       (20)        0 2023-05-11 20:52:52.423488 xpublish_edr-0.1.dev29/.github/workflows/
+-rw-r--r--   0 akerney    (502) staff       (20)      237 2022-07-15 20:50:57.000000 xpublish_edr-0.1.dev29/.github/workflows/pre-commit.yml
+-rw-r--r--   0 akerney    (502) staff       (20)     1766 2023-05-11 20:47:24.000000 xpublish_edr-0.1.dev29/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 akerney    (502) staff       (20)      963 2022-12-11 16:56:31.000000 xpublish_edr-0.1.dev29/.github/workflows/tests.yml
+-rw-r--r--   0 akerney    (502) staff       (20)     1472 2022-05-11 10:40:36.000000 xpublish_edr-0.1.dev29/LICENSE.txt
+-rw-r--r--   0 akerney    (502) staff       (20)      251 2023-05-11 20:51:17.000000 xpublish_edr-0.1.dev29/MANIFEST.in
+-rw-r--r--   0 akerney    (502) staff       (20)     3705 2023-05-11 20:52:52.427112 xpublish_edr-0.1.dev29/PKG-INFO
+-rw-r--r--   0 akerney    (502) staff       (20)     1309 2022-05-11 12:12:08.000000 xpublish_edr-0.1.dev29/README.md
+-rw-r--r--   0 akerney    (502) staff       (20)     1799 2023-05-11 20:51:01.000000 xpublish_edr-0.1.dev29/pyproject.toml
+-rw-r--r--   0 akerney    (502) staff       (20)      277 2022-06-14 16:26:23.000000 xpublish_edr-0.1.dev29/requirements-dev.txt
+-rw-r--r--   0 akerney    (502) staff       (20)       38 2023-05-11 20:48:24.000000 xpublish_edr-0.1.dev29/requirements.txt
+-rw-r--r--   0 akerney    (502) staff       (20)       38 2023-05-11 20:52:52.427803 xpublish_edr-0.1.dev29/setup.cfg
+drwxr-xr-x   0 akerney    (502) staff       (20)        0 2023-05-11 20:52:52.424976 xpublish_edr-0.1.dev29/xpublish_edr/
+-rw-r--r--   0 akerney    (502) staff       (20)      247 2023-05-11 20:46:59.000000 xpublish_edr-0.1.dev29/xpublish_edr/__init__.py
+-rw-r--r--   0 akerney    (502) staff       (20)      170 2023-05-11 20:52:52.000000 xpublish_edr-0.1.dev29/xpublish_edr/_version.py
+drwxr-xr-x   0 akerney    (502) staff       (20)        0 2023-05-11 20:52:52.426107 xpublish_edr-0.1.dev29/xpublish_edr/formats/
+-rw-r--r--   0 akerney    (502) staff       (20)     4141 2022-07-15 20:50:57.000000 xpublish_edr-0.1.dev29/xpublish_edr/formats/to_covjson.py
+-rw-r--r--   0 akerney    (502) staff       (20)      424 2022-07-15 20:43:58.000000 xpublish_edr-0.1.dev29/xpublish_edr/formats/to_csv.py
+-rw-r--r--   0 akerney    (502) staff       (20)      616 2022-07-15 20:43:58.000000 xpublish_edr-0.1.dev29/xpublish_edr/formats/to_netcdf.py
+-rw-r--r--   0 akerney    (502) staff       (20)     5125 2023-05-11 20:46:59.000000 xpublish_edr-0.1.dev29/xpublish_edr/plugin.py
+-rw-r--r--   0 akerney    (502) staff       (20)     1956 2022-07-15 20:43:58.000000 xpublish_edr-0.1.dev29/xpublish_edr/query.py
+drwxr-xr-x   0 akerney    (502) staff       (20)        0 2023-05-11 20:52:52.426490 xpublish_edr-0.1.dev29/xpublish_edr.egg-info/
+-rw-r--r--   0 akerney    (502) staff       (20)      380 2023-05-11 20:52:52.000000 xpublish_edr-0.1.dev29/xpublish_edr.egg-info/SOURCES.txt
```

### Comparing `xpublish_edr-0.1.1/.github/workflows/publish-to-pypi.yml` & `xpublish_edr-0.1.dev29/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `xpublish_edr-0.1.1/LICENSE.txt` & `xpublish_edr-0.1.dev29/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `xpublish_edr-0.1.1/PKG-INFO` & `xpublish_edr-0.1.dev29/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xpublish_edr
-Version: 0.1.1
+Version: 0.1.dev29
 License: Copyright 2017 AUTHOR NAME
         
         
         Redistribution and use in source and binary forms,
         with or without modification,
         are permitted provided that the following conditions are met:
         
@@ -32,30 +32,26 @@
         
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 ## xpublish-edr
 
-[![PyPI](https://img.shields.io/pypi/v/xpublish-edr)](https://pypi.org/project/xpublish-edr/)
-[![Conda Version](https://img.shields.io/conda/vn/conda-forge/xpublish-edr.svg)](https://anaconda.org/conda-forge/xpublish-edr)
-
 [![Tests](https://github.com/gulfofmaine/xpublish-edr/actions/workflows/tests.yml/badge.svg)](https://github.com/gulfofmaine/xpublish-edr/actions/workflows/tests.yml)
-[![codecov](https://codecov.io/gh/xpublish-community/xpublish-edr/branch/main/graph/badge.svg?token=19AE9JWWWD)](https://codecov.io/gh/xpublish-community/xpublish-edr)
-[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/xpublish-community/xpublish-edr/main.svg)](https://results.pre-commit.ci/latest/github/xpublish-community/xpublish-edr/main)
 
 [Xpublish](https://xpublish.readthedocs.io/en/latest/) routers for the [OGC EDR API](https://ogcapi.ogc.org/edr/).
 
 ### Documentation and code
 
 URLs for the docs and code.
```

### Comparing `xpublish_edr-0.1.1/pyproject.toml` & `xpublish_edr-0.1.dev29/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -13,17 +13,18 @@
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Science/Research",
     "Operating System :: OS Independent",
     "License :: OSI Approved :: BSD License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.7",
+    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11",
     "Topic :: Scientific/Engineering",
 ]
 
 dynamic = ["version", "dependencies"]
 
 [project.entry-points."xpublish.plugin"]
 cf_edr = "xpublish_edr.plugin:CfEdrPlugin"
@@ -33,24 +34,25 @@
 csv = "xpublish_edr.formats.to_csv:to_csv"
 nc = "xpublish_edr.formats.to_netcdf:to_netcdf"
 netcdf = "xpublish_edr.formats.to_netcdf:to_netcdf"
 nc4 = "xpublish_edr.formats.to_netcdf:to_netcdf"
 netcdf4 = "xpublish_edr.formats.to_netcdf:to_netcdf"
 
 [tool.check-manifest]
-ignore = ["xpublish_edr/_version.py"]
+ignore = ["xpublish_opendap/_version.py"]
 
 [tool.setuptools]
 packages = ["xpublish_edr"]
 
 [tool.setuptools.dynamic]
 dependencies = { file = ["requirements.txt"] }
 
 [tool.setuptools_scm]
 write_to = "xpublish_edr/_version.py"
+local_scheme = "no-local-version"
 
 [tool.interrogate]
 ignore-init-method = true
 ignore-init-module = false
 ignore-magic = false
 ignore-semiprivate = false
 ignore-private = false
```

### Comparing `xpublish_edr-0.1.1/xpublish_edr/formats/to_covjson.py` & `xpublish_edr-0.1.dev29/xpublish_edr/formats/to_covjson.py`

 * *Files identical despite different names*

### Comparing `xpublish_edr-0.1.1/xpublish_edr/formats/to_netcdf.py` & `xpublish_edr-0.1.dev29/xpublish_edr/formats/to_netcdf.py`

 * *Files identical despite different names*

### Comparing `xpublish_edr-0.1.1/xpublish_edr/plugin.py` & `xpublish_edr-0.1.dev29/xpublish_edr/plugin.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 
 class CfEdrPlugin(Plugin):
     """
     OGC EDR compatible endpoints for Xpublish datasets
     """
 
-    name: str = "cf_edr"
+    name = "cf_edr"
 
     app_router_prefix: str = "/edr"
     app_router_tags: List[str] = ["edr"]
 
     dataset_router_prefix: str = "/edr"
     dataset_router_tags: List[str] = ["edr"]
```

### Comparing `xpublish_edr-0.1.1/xpublish_edr/query.py` & `xpublish_edr-0.1.dev29/xpublish_edr/query.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,36 +40,30 @@
         None,
         title="Z axis",
         description="Height or depth of query",
     ),
     datetime: Optional[str] = Query(
         None,
         title="Datetime or datetime range",
-        description=(
-            "Query by a single ISO time or a range of ISO times. "
-            "To query by a range, split the times with a slash"
-        ),
+        description="Query by a single ISO time or a range of ISO times. To query by a range, split the times with a slash",
     ),
     parameters: Optional[str] = Query(
         None,
         alias="parameter-name",
         description="xarray variables to query",
     ),
     crs: Optional[str] = Query(
         None,
         deprecated=True,
         description="CRS is not yet implemented",
     ),
     f: Optional[str] = Query(
         None,
         title="Response format",
-        description=(
-            "Data is returned as a CoverageJSON by default. "
-            "Get `/formats` to discover what other formats are accessible"
-        ),
+        description="Data is returned as a CoverageJSON by default. Get `/formats` to discover what other formats are accessible",
     ),
 ):
     """Extract EDR query params from request query strings"""
     return EDRQuery(
         coords=coords,
         z=z,
         datetime=datetime,
```

