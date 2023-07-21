# Comparing `tmp/phdi-1.0.8.tar.gz` & `tmp/phdi-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phdi-1.0.8.tar", max compression
+gzip compressed data, was "phdi-1.0.9.tar", max compression
```

## Comparing `phdi-1.0.8.tar` & `phdi-1.0.9.tar`

### file list

```diff
@@ -1,68 +1,68 @@
--rw-r--r--   0        0        0     7048 2023-07-13 18:18:43.653036 phdi-1.0.8/LICENSE.md
--rw-r--r--   0        0        0    11787 2023-07-13 18:18:43.653036 phdi-1.0.8/README.md
--rw-r--r--   0        0        0       22 2023-07-13 18:18:44.137032 phdi-1.0.8/phdi/__init__.py
--rw-r--r--   0        0        0      223 2023-07-13 18:18:44.137032 phdi-1.0.8/phdi/cloud/README.md
--rw-r--r--   0        0        0        0 2023-07-13 18:18:44.137032 phdi-1.0.8/phdi/cloud/__init__.py
--rw-r--r--   0        0        0     9436 2023-07-13 18:18:44.137032 phdi-1.0.8/phdi/cloud/azure.py
--rw-r--r--   0        0        0     2516 2023-07-13 18:18:44.137032 phdi-1.0.8/phdi/cloud/core.py
--rw-r--r--   0        0        0     6055 2023-07-13 18:18:44.137032 phdi-1.0.8/phdi/cloud/gcp.py
--rw-r--r--   0        0        0      163 2023-07-13 18:18:44.137032 phdi-1.0.8/phdi/containers/README.md
--rw-r--r--   0        0        0        0 2023-07-13 18:18:44.137032 phdi-1.0.8/phdi/containers/__init__.py
--rw-r--r--   0        0        0     2776 2023-07-13 18:18:44.141032 phdi-1.0.8/phdi/containers/base_service.py
--rw-r--r--   0        0        0        0 2023-07-13 18:18:44.141032 phdi-1.0.8/phdi/fhir/__init__.py
--rw-r--r--   0        0        0      292 2023-07-13 18:18:44.141032 phdi-1.0.8/phdi/fhir/cloud/README.md
--rw-r--r--   0        0        0      119 2023-07-13 18:18:44.141032 phdi-1.0.8/phdi/fhir/cloud/__init__.py
--rw-r--r--   0        0        0     2111 2023-07-13 18:18:44.141032 phdi-1.0.8/phdi/fhir/cloud/azure.py
--rw-r--r--   0        0        0      311 2023-07-13 18:18:44.141032 phdi-1.0.8/phdi/fhir/conversion/README.md
--rw-r--r--   0        0        0       89 2023-07-13 18:18:44.141032 phdi-1.0.8/phdi/fhir/conversion/__init__.py
--rw-r--r--   0        0        0     8026 2023-07-13 18:18:44.141032 phdi-1.0.8/phdi/fhir/conversion/convert.py
--rw-r--r--   0        0        0      808 2023-07-13 18:18:44.141032 phdi-1.0.8/phdi/fhir/geospatial/README.md
--rw-r--r--   0        0        0      294 2023-07-13 18:18:44.141032 phdi-1.0.8/phdi/fhir/geospatial/__init__.py
--rw-r--r--   0        0        0     3494 2023-07-13 18:18:44.141032 phdi-1.0.8/phdi/fhir/geospatial/census.py
--rw-r--r--   0        0        0     4521 2023-07-13 18:18:44.141032 phdi-1.0.8/phdi/fhir/geospatial/core.py
--rw-r--r--   0        0        0     3640 2023-07-13 18:18:44.141032 phdi-1.0.8/phdi/fhir/geospatial/smarty.py
--rw-r--r--   0        0        0      890 2023-07-13 18:18:44.141032 phdi-1.0.8/phdi/fhir/harmonization/README.md
--rw-r--r--   0        0        0      335 2023-07-13 18:18:44.141032 phdi-1.0.8/phdi/fhir/harmonization/__init__.py
--rw-r--r--   0        0        0    11809 2023-07-13 18:18:44.141032 phdi-1.0.8/phdi/fhir/harmonization/standardization.py
--rw-r--r--   0        0        0      179 2023-07-13 18:18:44.141032 phdi-1.0.8/phdi/fhir/linkage/__init__.py
--rw-r--r--   0        0        0     3591 2023-07-13 18:18:44.141032 phdi-1.0.8/phdi/fhir/linkage/link.py
--rw-r--r--   0        0        0      412 2023-07-13 18:18:44.141032 phdi-1.0.8/phdi/fhir/tabulation/README.md
--rw-r--r--   0        0        0      367 2023-07-13 18:18:44.141032 phdi-1.0.8/phdi/fhir/tabulation/__init__.py
--rw-r--r--   0        0        0    27459 2023-07-13 18:18:44.141032 phdi-1.0.8/phdi/fhir/tabulation/tables.py
--rw-r--r--   0        0        0      397 2023-07-13 18:18:44.141032 phdi-1.0.8/phdi/fhir/transport/README.md
--rw-r--r--   0        0        0      327 2023-07-13 18:18:44.141032 phdi-1.0.8/phdi/fhir/transport/__init__.py
--rw-r--r--   0        0        0     7383 2023-07-13 18:18:44.141032 phdi-1.0.8/phdi/fhir/transport/export.py
--rw-r--r--   0        0        0     8834 2023-07-13 18:18:44.141032 phdi-1.0.8/phdi/fhir/transport/http.py
--rw-r--r--   0        0        0     7005 2023-07-13 18:18:44.141032 phdi-1.0.8/phdi/fhir/utils.py
--rw-r--r--   0        0        0      881 2023-07-13 18:18:44.141032 phdi-1.0.8/phdi/geospatial/README.md
--rw-r--r--   0        0        0      291 2023-07-13 18:18:44.141032 phdi-1.0.8/phdi/geospatial/__init__.py
--rw-r--r--   0        0        0     9294 2023-07-13 18:18:44.141032 phdi-1.0.8/phdi/geospatial/census.py
--rw-r--r--   0        0        0     2697 2023-07-13 18:18:44.141032 phdi-1.0.8/phdi/geospatial/core.py
--rw-r--r--   0        0        0     5992 2023-07-13 18:18:44.141032 phdi-1.0.8/phdi/geospatial/smarty.py
--rw-r--r--   0        0        0     1027 2023-07-13 18:18:44.141032 phdi-1.0.8/phdi/harmonization/README.md
--rw-r--r--   0        0        0      869 2023-07-13 18:18:44.141032 phdi-1.0.8/phdi/harmonization/__init__.py
--rw-r--r--   0        0        0    28162 2023-07-13 18:18:44.141032 phdi-1.0.8/phdi/harmonization/double_metaphone.py
--rw-r--r--   0        0        0    10909 2023-07-13 18:18:44.141032 phdi-1.0.8/phdi/harmonization/hl7.py
--rw-r--r--   0        0        0    36359 2023-07-13 18:18:44.141032 phdi-1.0.8/phdi/harmonization/phdi_nicknames.csv
--rw-r--r--   0        0        0    11999 2023-07-13 18:18:44.141032 phdi-1.0.8/phdi/harmonization/standardization.py
--rw-r--r--   0        0        0     1952 2023-07-13 18:18:44.141032 phdi-1.0.8/phdi/harmonization/utils.py
--rw-r--r--   0        0        0      255 2023-07-13 18:18:44.141032 phdi-1.0.8/phdi/linkage/README.md
--rw-r--r--   0        0        0     1869 2023-07-13 18:18:44.141032 phdi-1.0.8/phdi/linkage/__init__.py
--rw-r--r--   0        0        0     2555 2023-07-13 18:18:44.141032 phdi-1.0.8/phdi/linkage/algorithms.py
--rw-r--r--   0        0        0     3167 2023-07-13 18:18:44.141032 phdi-1.0.8/phdi/linkage/core.py
--rw-r--r--   0        0        0    59276 2023-07-13 18:18:44.141032 phdi-1.0.8/phdi/linkage/link.py
--rw-r--r--   0        0        0    15429 2023-07-13 18:18:44.141032 phdi-1.0.8/phdi/linkage/postgres.py
--rw-r--r--   0        0        0     2792 2023-07-13 18:18:44.141032 phdi-1.0.8/phdi/linkage/seed.py
--rw-r--r--   0        0        0      399 2023-07-13 18:18:44.141032 phdi-1.0.8/phdi/linkage/tables.ddl
--rw-r--r--   0        0        0      225 2023-07-13 18:18:44.141032 phdi-1.0.8/phdi/tabulation/README.md
--rw-r--r--   0        0        0      134 2023-07-13 18:18:44.141032 phdi-1.0.8/phdi/tabulation/__init__.py
--rw-r--r--   0        0        0    11838 2023-07-13 18:18:44.141032 phdi-1.0.8/phdi/tabulation/tables.py
--rw-r--r--   0        0        0     2046 2023-07-13 18:18:44.141032 phdi-1.0.8/phdi/tabulation/validation_schema.json
--rw-r--r--   0        0        0      225 2023-07-13 18:18:44.141032 phdi-1.0.8/phdi/transport/README.md
--rw-r--r--   0        0        0       81 2023-07-13 18:18:44.141032 phdi-1.0.8/phdi/transport/__init__.py
--rw-r--r--   0        0        0     2334 2023-07-13 18:18:44.141032 phdi-1.0.8/phdi/transport/http.py
--rw-r--r--   0        0        0     1244 2023-07-13 18:18:44.141032 phdi-1.0.8/phdi/validation/__init__.py
--rw-r--r--   0        0        0     6260 2023-07-13 18:18:44.141032 phdi-1.0.8/phdi/validation/validation.py
--rw-r--r--   0        0        0    17870 2023-07-13 18:18:44.141032 phdi-1.0.8/phdi/validation/xml_utils.py
--rw-r--r--   0        0        0     1824 2023-07-13 18:18:44.153031 phdi-1.0.8/pyproject.toml
--rw-r--r--   0        0        0    13543 1970-01-01 00:00:00.000000 phdi-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0     7048 2023-07-21 16:49:12.859192 phdi-1.0.9/LICENSE.md
+-rw-r--r--   0        0        0    11787 2023-07-21 16:49:12.859192 phdi-1.0.9/README.md
+-rw-r--r--   0        0        0       22 2023-07-21 16:49:13.403193 phdi-1.0.9/phdi/__init__.py
+-rw-r--r--   0        0        0      223 2023-07-21 16:49:13.403193 phdi-1.0.9/phdi/cloud/README.md
+-rw-r--r--   0        0        0        0 2023-07-21 16:49:13.403193 phdi-1.0.9/phdi/cloud/__init__.py
+-rw-r--r--   0        0        0     9436 2023-07-21 16:49:13.403193 phdi-1.0.9/phdi/cloud/azure.py
+-rw-r--r--   0        0        0     2516 2023-07-21 16:49:13.403193 phdi-1.0.9/phdi/cloud/core.py
+-rw-r--r--   0        0        0     6055 2023-07-21 16:49:13.403193 phdi-1.0.9/phdi/cloud/gcp.py
+-rw-r--r--   0        0        0      163 2023-07-21 16:49:13.403193 phdi-1.0.9/phdi/containers/README.md
+-rw-r--r--   0        0        0        0 2023-07-21 16:49:13.403193 phdi-1.0.9/phdi/containers/__init__.py
+-rw-r--r--   0        0        0     2776 2023-07-21 16:49:13.403193 phdi-1.0.9/phdi/containers/base_service.py
+-rw-r--r--   0        0        0        0 2023-07-21 16:49:13.403193 phdi-1.0.9/phdi/fhir/__init__.py
+-rw-r--r--   0        0        0      292 2023-07-21 16:49:13.403193 phdi-1.0.9/phdi/fhir/cloud/README.md
+-rw-r--r--   0        0        0      119 2023-07-21 16:49:13.403193 phdi-1.0.9/phdi/fhir/cloud/__init__.py
+-rw-r--r--   0        0        0     2111 2023-07-21 16:49:13.403193 phdi-1.0.9/phdi/fhir/cloud/azure.py
+-rw-r--r--   0        0        0      311 2023-07-21 16:49:13.403193 phdi-1.0.9/phdi/fhir/conversion/README.md
+-rw-r--r--   0        0        0       89 2023-07-21 16:49:13.403193 phdi-1.0.9/phdi/fhir/conversion/__init__.py
+-rw-r--r--   0        0        0     8026 2023-07-21 16:49:13.403193 phdi-1.0.9/phdi/fhir/conversion/convert.py
+-rw-r--r--   0        0        0      808 2023-07-21 16:49:13.403193 phdi-1.0.9/phdi/fhir/geospatial/README.md
+-rw-r--r--   0        0        0      294 2023-07-21 16:49:13.403193 phdi-1.0.9/phdi/fhir/geospatial/__init__.py
+-rw-r--r--   0        0        0     3494 2023-07-21 16:49:13.403193 phdi-1.0.9/phdi/fhir/geospatial/census.py
+-rw-r--r--   0        0        0     4521 2023-07-21 16:49:13.403193 phdi-1.0.9/phdi/fhir/geospatial/core.py
+-rw-r--r--   0        0        0     3640 2023-07-21 16:49:13.403193 phdi-1.0.9/phdi/fhir/geospatial/smarty.py
+-rw-r--r--   0        0        0      890 2023-07-21 16:49:13.403193 phdi-1.0.9/phdi/fhir/harmonization/README.md
+-rw-r--r--   0        0        0      335 2023-07-21 16:49:13.403193 phdi-1.0.9/phdi/fhir/harmonization/__init__.py
+-rw-r--r--   0        0        0    11809 2023-07-21 16:49:13.403193 phdi-1.0.9/phdi/fhir/harmonization/standardization.py
+-rw-r--r--   0        0        0      179 2023-07-21 16:49:13.403193 phdi-1.0.9/phdi/fhir/linkage/__init__.py
+-rw-r--r--   0        0        0     3591 2023-07-21 16:49:13.403193 phdi-1.0.9/phdi/fhir/linkage/link.py
+-rw-r--r--   0        0        0      412 2023-07-21 16:49:13.403193 phdi-1.0.9/phdi/fhir/tabulation/README.md
+-rw-r--r--   0        0        0      367 2023-07-21 16:49:13.403193 phdi-1.0.9/phdi/fhir/tabulation/__init__.py
+-rw-r--r--   0        0        0    27459 2023-07-21 16:49:13.403193 phdi-1.0.9/phdi/fhir/tabulation/tables.py
+-rw-r--r--   0        0        0      397 2023-07-21 16:49:13.403193 phdi-1.0.9/phdi/fhir/transport/README.md
+-rw-r--r--   0        0        0      327 2023-07-21 16:49:13.403193 phdi-1.0.9/phdi/fhir/transport/__init__.py
+-rw-r--r--   0        0        0     7383 2023-07-21 16:49:13.403193 phdi-1.0.9/phdi/fhir/transport/export.py
+-rw-r--r--   0        0        0     8834 2023-07-21 16:49:13.403193 phdi-1.0.9/phdi/fhir/transport/http.py
+-rw-r--r--   0        0        0     7012 2023-07-21 16:49:13.403193 phdi-1.0.9/phdi/fhir/utils.py
+-rw-r--r--   0        0        0      881 2023-07-21 16:49:13.403193 phdi-1.0.9/phdi/geospatial/README.md
+-rw-r--r--   0        0        0      291 2023-07-21 16:49:13.403193 phdi-1.0.9/phdi/geospatial/__init__.py
+-rw-r--r--   0        0        0     9294 2023-07-21 16:49:13.403193 phdi-1.0.9/phdi/geospatial/census.py
+-rw-r--r--   0        0        0     2697 2023-07-21 16:49:13.403193 phdi-1.0.9/phdi/geospatial/core.py
+-rw-r--r--   0        0        0     5992 2023-07-21 16:49:13.403193 phdi-1.0.9/phdi/geospatial/smarty.py
+-rw-r--r--   0        0        0     1027 2023-07-21 16:49:13.403193 phdi-1.0.9/phdi/harmonization/README.md
+-rw-r--r--   0        0        0      869 2023-07-21 16:49:13.403193 phdi-1.0.9/phdi/harmonization/__init__.py
+-rw-r--r--   0        0        0    28162 2023-07-21 16:49:13.403193 phdi-1.0.9/phdi/harmonization/double_metaphone.py
+-rw-r--r--   0        0        0    10909 2023-07-21 16:49:13.403193 phdi-1.0.9/phdi/harmonization/hl7.py
+-rw-r--r--   0        0        0    36359 2023-07-21 16:49:13.403193 phdi-1.0.9/phdi/harmonization/phdi_nicknames.csv
+-rw-r--r--   0        0        0    11999 2023-07-21 16:49:13.403193 phdi-1.0.9/phdi/harmonization/standardization.py
+-rw-r--r--   0        0        0     1952 2023-07-21 16:49:13.403193 phdi-1.0.9/phdi/harmonization/utils.py
+-rw-r--r--   0        0        0      255 2023-07-21 16:49:13.403193 phdi-1.0.9/phdi/linkage/README.md
+-rw-r--r--   0        0        0     1869 2023-07-21 16:49:13.403193 phdi-1.0.9/phdi/linkage/__init__.py
+-rw-r--r--   0        0        0     2555 2023-07-21 16:49:13.403193 phdi-1.0.9/phdi/linkage/algorithms.py
+-rw-r--r--   0        0        0     3167 2023-07-21 16:49:13.403193 phdi-1.0.9/phdi/linkage/core.py
+-rw-r--r--   0        0        0    60956 2023-07-21 16:49:13.403193 phdi-1.0.9/phdi/linkage/link.py
+-rw-r--r--   0        0        0    15429 2023-07-21 16:49:13.403193 phdi-1.0.9/phdi/linkage/postgres.py
+-rw-r--r--   0        0        0     3068 2023-07-21 16:49:13.407193 phdi-1.0.9/phdi/linkage/seed.py
+-rw-r--r--   0        0        0      399 2023-07-21 16:49:13.407193 phdi-1.0.9/phdi/linkage/tables.ddl
+-rw-r--r--   0        0        0      225 2023-07-21 16:49:13.407193 phdi-1.0.9/phdi/tabulation/README.md
+-rw-r--r--   0        0        0      134 2023-07-21 16:49:13.407193 phdi-1.0.9/phdi/tabulation/__init__.py
+-rw-r--r--   0        0        0    11838 2023-07-21 16:49:13.407193 phdi-1.0.9/phdi/tabulation/tables.py
+-rw-r--r--   0        0        0     2046 2023-07-21 16:49:13.407193 phdi-1.0.9/phdi/tabulation/validation_schema.json
+-rw-r--r--   0        0        0      225 2023-07-21 16:49:13.407193 phdi-1.0.9/phdi/transport/README.md
+-rw-r--r--   0        0        0       81 2023-07-21 16:49:13.407193 phdi-1.0.9/phdi/transport/__init__.py
+-rw-r--r--   0        0        0     2334 2023-07-21 16:49:13.407193 phdi-1.0.9/phdi/transport/http.py
+-rw-r--r--   0        0        0     1244 2023-07-21 16:49:13.407193 phdi-1.0.9/phdi/validation/__init__.py
+-rw-r--r--   0        0        0     6260 2023-07-21 16:49:13.407193 phdi-1.0.9/phdi/validation/validation.py
+-rw-r--r--   0        0        0    17870 2023-07-21 16:49:13.407193 phdi-1.0.9/phdi/validation/xml_utils.py
+-rw-r--r--   0        0        0     1824 2023-07-21 16:49:13.415193 phdi-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0    13543 1970-01-01 00:00:00.000000 phdi-1.0.9/PKG-INFO
```

### Comparing `phdi-1.0.8/LICENSE.md` & `phdi-1.0.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `phdi-1.0.8/README.md` & `phdi-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `phdi-1.0.8/phdi/cloud/azure.py` & `phdi-1.0.9/phdi/cloud/azure.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.8/phdi/cloud/core.py` & `phdi-1.0.9/phdi/cloud/core.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.8/phdi/cloud/gcp.py` & `phdi-1.0.9/phdi/cloud/gcp.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.8/phdi/containers/base_service.py` & `phdi-1.0.9/phdi/containers/base_service.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.8/phdi/fhir/cloud/azure.py` & `phdi-1.0.9/phdi/fhir/cloud/azure.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.8/phdi/fhir/conversion/convert.py` & `phdi-1.0.9/phdi/fhir/conversion/convert.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.8/phdi/fhir/geospatial/README.md` & `phdi-1.0.9/phdi/fhir/geospatial/README.md`

 * *Files identical despite different names*

### Comparing `phdi-1.0.8/phdi/fhir/geospatial/census.py` & `phdi-1.0.9/phdi/fhir/geospatial/census.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.8/phdi/fhir/geospatial/core.py` & `phdi-1.0.9/phdi/fhir/geospatial/core.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.8/phdi/fhir/geospatial/smarty.py` & `phdi-1.0.9/phdi/fhir/geospatial/smarty.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.8/phdi/fhir/harmonization/README.md` & `phdi-1.0.9/phdi/fhir/harmonization/README.md`

 * *Files identical despite different names*

### Comparing `phdi-1.0.8/phdi/fhir/harmonization/standardization.py` & `phdi-1.0.9/phdi/fhir/harmonization/standardization.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.8/phdi/fhir/linkage/link.py` & `phdi-1.0.9/phdi/fhir/linkage/link.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.8/phdi/fhir/tabulation/tables.py` & `phdi-1.0.9/phdi/fhir/tabulation/tables.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.8/phdi/fhir/transport/export.py` & `phdi-1.0.9/phdi/fhir/transport/export.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.8/phdi/fhir/transport/http.py` & `phdi-1.0.9/phdi/fhir/transport/http.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.8/phdi/fhir/utils.py` & `phdi-1.0.9/phdi/fhir/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 selection_criteria_types = Literal["first", "last", "random", "all"]
 
 
 def apply_selection_criteria(
     value: List[Any],
     selection_criteria: selection_criteria_types,
-) -> str:
+) -> str | List:
     """
     Returns value(s), according to the selection criteria, from a given list of values
     parsed from a FHIR resource. A single string value is returned - if the selected
     value is a complex structure (list or dict), it is converted to a string.
     :param value: A list containing the values parsed from a FHIR resource.
     :param selection_criteria: A string indicating which element(s) of a list to select.
     :return: Value(s) parsed from a FHIR resource that conform to the selection
```

### Comparing `phdi-1.0.8/phdi/geospatial/README.md` & `phdi-1.0.9/phdi/geospatial/README.md`

 * *Files identical despite different names*

### Comparing `phdi-1.0.8/phdi/geospatial/census.py` & `phdi-1.0.9/phdi/geospatial/census.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.8/phdi/geospatial/core.py` & `phdi-1.0.9/phdi/geospatial/core.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.8/phdi/geospatial/smarty.py` & `phdi-1.0.9/phdi/geospatial/smarty.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.8/phdi/harmonization/README.md` & `phdi-1.0.9/phdi/harmonization/README.md`

 * *Files identical despite different names*

### Comparing `phdi-1.0.8/phdi/harmonization/__init__.py` & `phdi-1.0.9/phdi/harmonization/__init__.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.8/phdi/harmonization/double_metaphone.py` & `phdi-1.0.9/phdi/harmonization/double_metaphone.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.8/phdi/harmonization/hl7.py` & `phdi-1.0.9/phdi/harmonization/hl7.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.8/phdi/harmonization/phdi_nicknames.csv` & `phdi-1.0.9/phdi/harmonization/phdi_nicknames.csv`

 * *Files identical despite different names*

### Comparing `phdi-1.0.8/phdi/harmonization/standardization.py` & `phdi-1.0.9/phdi/harmonization/standardization.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.8/phdi/harmonization/utils.py` & `phdi-1.0.9/phdi/harmonization/utils.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.8/phdi/linkage/__init__.py` & `phdi-1.0.9/phdi/linkage/__init__.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.8/phdi/linkage/algorithms.py` & `phdi-1.0.9/phdi/linkage/algorithms.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.8/phdi/linkage/core.py` & `phdi-1.0.9/phdi/linkage/core.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.8/phdi/linkage/link.py` & `phdi-1.0.9/phdi/linkage/link.py`

 * *Files 1% similar despite different names*

```diff
@@ -367,20 +367,18 @@
             [b.get("transformation") for b in transform_blocks],
         )
     )
     for block_dict in blocking_fields:
         block = block_dict.get("value")
         try:
             # Apply utility extractor for safe parsing
-            value = str(
-                extract_value_with_resource_path(
-                    record,
-                    LINKING_FIELDS_TO_FHIRPATHS[block],
-                    selection_criteria="first",
-                )
+            value = extract_value_with_resource_path(
+                record,
+                LINKING_FIELDS_TO_FHIRPATHS[block],
+                selection_criteria="first",
             )
             if value:
                 if block in transformations:
                     try:
                         value = transform_funcs[transformations[block]](value)
                     except KeyError:
                         raise ValueError(
@@ -392,14 +390,23 @@
                     }
                 else:
                     block_vals[block] = {"value": value}
 
         except KeyError:
             raise ValueError(f"Field {block} is not a supported extraction field.")
 
+    # Account for any incoming FHIR resources that return no data
+    # for a field--don't count this against records to-block
+    keys_to_pop = []
+    for field in block_vals:
+        if _is_empty_extraction_field(block_vals, field):
+            keys_to_pop.append(field)
+    for k in keys_to_pop:
+        block_vals.pop(k)
+
     return block_vals
 
 
 def feature_match_exact(
     record_i: List,
     record_j: List,
     feature_col: str,
@@ -1309,25 +1316,34 @@
 def _flatten_patient_field_helper(resource: dict, field: str) -> any:
     """
     Helper function that determines the correct way to flatten a patient's
     FHIR field based on the specific field in question. Names and Addresses,
     because their lists can hold multiple objects, are fetched completely,
     whereas other fields just have their first element used (since historical
     information doesn't matter there).
+
+    For any field for which the value would be `None`, instead use an empty string
+    (if the field isn't first_name or address) or a list with one element, the
+    empty string (if the field is first_name or address). This ensures that
+    future loops over the elements don't disrupt the flow of the matching
+    algorithm.
     """
     if field == "first_name":
-        return extract_value_with_resource_path(
+        vals = extract_value_with_resource_path(
             resource, LINKING_FIELDS_TO_FHIRPATHS[field], selection_criteria="all"
         )
+        return vals if vals is not None else [""]
     elif field == "address":
-        return _condense_extract_address_from_resource(resource)
+        vals = _condense_extract_address_from_resource(resource)
+        return vals if vals is not None else [""]
     else:
-        return extract_value_with_resource_path(
+        val = extract_value_with_resource_path(
             resource, LINKING_FIELDS_TO_FHIRPATHS[field], selection_criteria="first"
         )
+        return val if val is not None else ""
 
 
 def _group_patient_block_by_person(data_block: List[list]) -> dict[str, List]:
     """
     Helper method that partitions the block of patient data returned from the MPI
     into clusters of records according to their linked Person ID.
     """
@@ -1448,14 +1464,37 @@
             for key, value in block_data.items()
         ]
     )
     query = query_stub + block_query
     return query
 
 
+def _is_empty_extraction_field(block_vals: dict, field: str):
+    """
+    Helper method that determines when a field extracted from an incoming
+    record should be considered "empty" for the purpose of blocking.
+    Fields whose values are either `None` or the empty string should not
+    be used when retrieving blocked records from the MPI, since that
+    would impose an artificial constraint (e.g. if an incoming record
+    has no `last_name` field, we don't want to retrieve only records
+    from the MPI that also have no `last_name`).
+    """
+    # Means the value extractor found no data in the FHIR resource
+    if block_vals[field] == "":
+        return True
+    # Alternatively, there was "data" there, but it's empty
+    elif (
+        block_vals[field].get("value") is None
+        or block_vals[field].get("value") == ""
+        or block_vals[field].get("value") == [""]
+    ):
+        return True
+    return False
+
+
 def _write_prob_file(prob_dict: dict, file_to_write: Union[pathlib.Path, None]):
     """
     Helper method to write a probability dictionary to a JSON file, if
     a valid path is supplied.
 
     :param prob_dict: A dictionary mapping column names to the log-probability
       values computed for those columns.
```

### Comparing `phdi-1.0.8/phdi/linkage/postgres.py` & `phdi-1.0.9/phdi/linkage/postgres.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.8/phdi/linkage/seed.py` & `phdi-1.0.9/phdi/linkage/seed.py`

 * *Files 11% similar despite different names*

```diff
@@ -58,14 +58,15 @@
                 "use": "home",
             },
             {
                 "system": "phone",
                 "value": f"{data.get('cell_phone',None)}",
                 "use": "mobile",
             },
+            {"value": f"{data.get('email',None)}", "system": "email"},
         ],
         "gender": f"{data.get('sex',None)}",
         "birthDate": f"{data.get('birthdate',None)}",
         "address": [
             {
                 "use": "home",
                 "line": [f"{data.get('address',None)}"],
@@ -74,12 +75,20 @@
                 "postalCode": f"{data.get('zip',None)}",
             }
         ],
     }
 
     fhir_bundle = {
         "resourceType": "Bundle",
+        "type": "batch",
         "id": str(uuid.uuid4()),
-        "entry": [{"fullUrl": f"urn:uuid:{patient_id}", "resource": patient_resource}],
+        "entry": [
+            {
+                "fullUrl": f"urn:uuid:{patient_id}",
+                "resource": patient_resource,
+                "request": {"method": "PUT", "url": f"Patient/{patient_id}"},
+            },
+        ],
     }
 
-    return (data["iris_id"], fhir_bundle)
+    iris_id = data.get("iris_id", None)
+    return (iris_id, fhir_bundle)
```

### Comparing `phdi-1.0.8/phdi/tabulation/tables.py` & `phdi-1.0.9/phdi/tabulation/tables.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.8/phdi/tabulation/validation_schema.json` & `phdi-1.0.9/phdi/tabulation/validation_schema.json`

 * *Files identical despite different names*

### Comparing `phdi-1.0.8/phdi/transport/http.py` & `phdi-1.0.9/phdi/transport/http.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.8/phdi/validation/__init__.py` & `phdi-1.0.9/phdi/validation/__init__.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.8/phdi/validation/validation.py` & `phdi-1.0.9/phdi/validation/validation.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.8/phdi/validation/xml_utils.py` & `phdi-1.0.9/phdi/validation/xml_utils.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.8/pyproject.toml` & `phdi-1.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "phdi"
-version = "v1.0.8"
+version = "v1.0.9"
 description = "Public health data infrastructure Building Blocks is a library to help public health departments work with their data"
 authors = ["Kenneth Chow <kenneth@skylight.digital>", "Brandon Mader <brandon@skylight.digital>", "Spencer Kathol <spencer@skylight.digital>", "Nick Clyde <nclyde@skylight.digital", "Dan Paseltiner <dan@skylight.digital>", "Brady Fausett <brady@skylight.digital>", "Marcelle Goggins <marcelle@skylight.digital", "Nick Bristow <nick@skylight.digital>", "Bryan Britten <bryan@skylight.digital>", "Emma Stephenson <emma@skylight.digital>" , "Gordon Farrell <gordon@skylight.digital>", "Robert Mitchell <rmitchell@skylight.digital>"]
 homepage = "https://github.com/CDCgov/phdi"
 repository = "https://github.com/CDCgov/phdi"
 documentation = "https://cdcgov.github.io/phdi"
 readme = "README.md"
```

### Comparing `phdi-1.0.8/PKG-INFO` & `phdi-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phdi
-Version: 1.0.8
+Version: 1.0.9
 Summary: Public health data infrastructure Building Blocks is a library to help public health departments work with their data
 Home-page: https://github.com/CDCgov/phdi
 Author: Kenneth Chow
 Author-email: kenneth@skylight.digital
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

