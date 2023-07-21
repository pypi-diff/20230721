# Comparing `tmp/phc-ingestion-0.3.44.tar.gz` & `tmp/phc-ingestion-0.3.45.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phc-ingestion-0.3.44.tar", last modified: Thu Jul 20 18:23:43 2023, max compression
+gzip compressed data, was "phc-ingestion-0.3.45.tar", last modified: Fri Jul 21 19:15:11 2023, max compression
```

## Comparing `phc-ingestion-0.3.44.tar` & `phc-ingestion-0.3.45.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0       16 2023-07-20 18:23:20.575536 phc-ingestion-0.3.44/PYPI.md
--rw-r--r--   0        0        0        0 2023-07-20 18:23:20.587536 phc-ingestion-0.3.44/ingestion/__init__.py
--rw-r--r--   0        0        0       61 2023-07-20 18:23:20.587536 phc-ingestion-0.3.44/ingestion/caris/__init__.py
--rw-r--r--   0        0        0     1636 2023-07-20 18:23:20.587536 phc-ingestion-0.3.44/ingestion/caris/process.py
--rw-r--r--   0        0        0        0 2023-07-20 18:23:20.587536 phc-ingestion-0.3.44/ingestion/caris/util/__init__.py
--rw-r--r--   0        0        0     4738 2023-07-20 18:23:20.587536 phc-ingestion-0.3.44/ingestion/caris/util/cnv.py
--rw-r--r--   0        0        0     1325 2023-07-20 18:23:20.587536 phc-ingestion-0.3.44/ingestion/caris/util/detect_genome_ref.py
--rw-r--r--   0        0        0      629 2023-07-20 18:23:20.587536 phc-ingestion-0.3.44/ingestion/caris/util/ga4gh.py
--rw-r--r--   0        0        0      555 2023-07-20 18:23:20.587536 phc-ingestion-0.3.44/ingestion/caris/util/interpretation.py
--rw-r--r--   0        0        0     4676 2023-07-20 18:23:20.587536 phc-ingestion-0.3.44/ingestion/caris/util/json.py
--rw-r--r--   0        0        0    21663 2023-07-20 18:23:20.587536 phc-ingestion-0.3.44/ingestion/caris/util/metadata.py
--rw-r--r--   0        0        0     4948 2023-07-20 18:23:20.587536 phc-ingestion-0.3.44/ingestion/caris/util/structural.py
--rw-r--r--   0        0        0      482 2023-07-20 18:23:20.587536 phc-ingestion-0.3.44/ingestion/caris/util/tar.py
--rw-r--r--   0        0        0     1771 2023-07-20 18:23:20.587536 phc-ingestion-0.3.44/ingestion/caris/util/tsv.py
--rw-r--r--   0        0        0     6933 2023-07-20 18:23:20.587536 phc-ingestion-0.3.44/ingestion/caris/util/vcf.py
--rw-r--r--   0        0        0       49 2023-07-20 18:23:20.587536 phc-ingestion-0.3.44/ingestion/foundation/__init__.py
--rw-r--r--   0        0        0     3142 2023-07-20 18:23:20.587536 phc-ingestion-0.3.44/ingestion/foundation/process.py
--rw-r--r--   0        0        0        0 2023-07-20 18:23:20.587536 phc-ingestion-0.3.44/ingestion/foundation/util/__init__.py
--rw-r--r--   0        0        0     4215 2023-07-20 18:23:20.587536 phc-ingestion-0.3.44/ingestion/foundation/util/cnv.py
--rw-r--r--   0        0        0     5937 2023-07-20 18:23:20.587536 phc-ingestion-0.3.44/ingestion/foundation/util/fnv.py
--rw-r--r--   0        0        0     8876 2023-07-20 18:23:20.587536 phc-ingestion-0.3.44/ingestion/foundation/util/ga4gh.py
--rw-r--r--   0        0        0      405 2023-07-20 18:23:20.587536 phc-ingestion-0.3.44/ingestion/foundation/util/interpretation.py
--rw-r--r--   0        0        0     5501 2023-07-20 18:23:20.587536 phc-ingestion-0.3.44/ingestion/foundation/util/vcf_etl.py
--rw-r--r--   0        0        0       46 2023-07-20 18:23:20.587536 phc-ingestion-0.3.44/ingestion/nextgen/__init__.py
--rw-r--r--   0        0        0     3074 2023-07-20 18:23:20.587536 phc-ingestion-0.3.44/ingestion/nextgen/process.py
--rw-r--r--   0        0        0      297 2023-07-20 18:23:20.587536 phc-ingestion-0.3.44/ingestion/nextgen/util/interpretation.py
--rw-r--r--   0        0        0     2284 2023-07-20 18:23:20.587536 phc-ingestion-0.3.44/ingestion/nextgen/util/process_cnv.py
--rw-r--r--   0        0        0     8461 2023-07-20 18:23:20.587536 phc-ingestion-0.3.44/ingestion/nextgen/util/process_manifest.py
--rw-r--r--   0        0        0     3785 2023-07-20 18:23:20.587536 phc-ingestion-0.3.44/ingestion/nextgen/util/process_structural.py
--rw-r--r--   0        0        0     7341 2023-07-20 18:23:20.587536 phc-ingestion-0.3.44/ingestion/nextgen/util/process_vcf.py
--rw-r--r--   0        0        0       22 2023-07-20 18:23:20.587536 phc-ingestion-0.3.44/ingestion/nextgen/util/types.py
--rw-r--r--   0        0        0     2047 2023-07-20 18:23:20.587536 phc-ingestion-0.3.44/ingestion/nextgen/util/variant_table.py
--rw-r--r--   0        0        0   408290 2023-07-20 18:23:20.587536 phc-ingestion-0.3.44/ingestion/resources/GRCh37_map.csv.gz
--rw-r--r--   0        0        0   612373 2023-07-20 18:23:20.591536 phc-ingestion-0.3.44/ingestion/resources/GRCh38_map.csv.gz
--rw-r--r--   0        0        0        0 2023-07-20 18:23:20.591536 phc-ingestion-0.3.44/ingestion/shared_util/__init__.py
--rw-r--r--   0        0        0     1669 2023-07-20 18:23:20.591536 phc-ingestion-0.3.44/ingestion/shared_util/coords_to_genes.py
--rw-r--r--   0        0        0      876 2023-07-20 18:23:20.591536 phc-ingestion-0.3.44/ingestion/shared_util/gene_to_coords.py
--rw-r--r--   0        0        0     1029 2023-07-20 18:23:20.591536 phc-ingestion-0.3.44/pyproject.toml
--rw-r--r--   0        0        0      269 1970-01-01 00:00:00.000000 phc-ingestion-0.3.44/PKG-INFO
+-rw-r--r--   0        0        0       16 2023-07-21 19:14:47.718323 phc-ingestion-0.3.45/PYPI.md
+-rw-r--r--   0        0        0        0 2023-07-21 19:14:47.730323 phc-ingestion-0.3.45/ingestion/__init__.py
+-rw-r--r--   0        0        0       61 2023-07-21 19:14:47.730323 phc-ingestion-0.3.45/ingestion/caris/__init__.py
+-rw-r--r--   0        0        0     1636 2023-07-21 19:14:47.730323 phc-ingestion-0.3.45/ingestion/caris/process.py
+-rw-r--r--   0        0        0        0 2023-07-21 19:14:47.730323 phc-ingestion-0.3.45/ingestion/caris/util/__init__.py
+-rw-r--r--   0        0        0     4738 2023-07-21 19:14:47.730323 phc-ingestion-0.3.45/ingestion/caris/util/cnv.py
+-rw-r--r--   0        0        0     1325 2023-07-21 19:14:47.730323 phc-ingestion-0.3.45/ingestion/caris/util/detect_genome_ref.py
+-rw-r--r--   0        0        0      629 2023-07-21 19:14:47.730323 phc-ingestion-0.3.45/ingestion/caris/util/ga4gh.py
+-rw-r--r--   0        0        0      555 2023-07-21 19:14:47.730323 phc-ingestion-0.3.45/ingestion/caris/util/interpretation.py
+-rw-r--r--   0        0        0     4676 2023-07-21 19:14:47.730323 phc-ingestion-0.3.45/ingestion/caris/util/json.py
+-rw-r--r--   0        0        0    21646 2023-07-21 19:14:47.730323 phc-ingestion-0.3.45/ingestion/caris/util/metadata.py
+-rw-r--r--   0        0        0     4948 2023-07-21 19:14:47.730323 phc-ingestion-0.3.45/ingestion/caris/util/structural.py
+-rw-r--r--   0        0        0      482 2023-07-21 19:14:47.730323 phc-ingestion-0.3.45/ingestion/caris/util/tar.py
+-rw-r--r--   0        0        0     1771 2023-07-21 19:14:47.730323 phc-ingestion-0.3.45/ingestion/caris/util/tsv.py
+-rw-r--r--   0        0        0     6933 2023-07-21 19:14:47.730323 phc-ingestion-0.3.45/ingestion/caris/util/vcf.py
+-rw-r--r--   0        0        0       49 2023-07-21 19:14:47.730323 phc-ingestion-0.3.45/ingestion/foundation/__init__.py
+-rw-r--r--   0        0        0     3142 2023-07-21 19:14:47.730323 phc-ingestion-0.3.45/ingestion/foundation/process.py
+-rw-r--r--   0        0        0        0 2023-07-21 19:14:47.730323 phc-ingestion-0.3.45/ingestion/foundation/util/__init__.py
+-rw-r--r--   0        0        0     4215 2023-07-21 19:14:47.730323 phc-ingestion-0.3.45/ingestion/foundation/util/cnv.py
+-rw-r--r--   0        0        0     5937 2023-07-21 19:14:47.730323 phc-ingestion-0.3.45/ingestion/foundation/util/fnv.py
+-rw-r--r--   0        0        0     8742 2023-07-21 19:14:47.730323 phc-ingestion-0.3.45/ingestion/foundation/util/ga4gh.py
+-rw-r--r--   0        0        0      405 2023-07-21 19:14:47.730323 phc-ingestion-0.3.45/ingestion/foundation/util/interpretation.py
+-rw-r--r--   0        0        0     5501 2023-07-21 19:14:47.730323 phc-ingestion-0.3.45/ingestion/foundation/util/vcf_etl.py
+-rw-r--r--   0        0        0       46 2023-07-21 19:14:47.730323 phc-ingestion-0.3.45/ingestion/nextgen/__init__.py
+-rw-r--r--   0        0        0     3074 2023-07-21 19:14:47.730323 phc-ingestion-0.3.45/ingestion/nextgen/process.py
+-rw-r--r--   0        0        0      297 2023-07-21 19:14:47.730323 phc-ingestion-0.3.45/ingestion/nextgen/util/interpretation.py
+-rw-r--r--   0        0        0     2284 2023-07-21 19:14:47.730323 phc-ingestion-0.3.45/ingestion/nextgen/util/process_cnv.py
+-rw-r--r--   0        0        0     8522 2023-07-21 19:14:47.730323 phc-ingestion-0.3.45/ingestion/nextgen/util/process_manifest.py
+-rw-r--r--   0        0        0     3785 2023-07-21 19:14:47.730323 phc-ingestion-0.3.45/ingestion/nextgen/util/process_structural.py
+-rw-r--r--   0        0        0     7341 2023-07-21 19:14:47.730323 phc-ingestion-0.3.45/ingestion/nextgen/util/process_vcf.py
+-rw-r--r--   0        0        0       22 2023-07-21 19:14:47.730323 phc-ingestion-0.3.45/ingestion/nextgen/util/types.py
+-rw-r--r--   0        0        0     2047 2023-07-21 19:14:47.730323 phc-ingestion-0.3.45/ingestion/nextgen/util/variant_table.py
+-rw-r--r--   0        0        0   408290 2023-07-21 19:14:47.734323 phc-ingestion-0.3.45/ingestion/resources/GRCh37_map.csv.gz
+-rw-r--r--   0        0        0   612373 2023-07-21 19:14:47.734323 phc-ingestion-0.3.45/ingestion/resources/GRCh38_map.csv.gz
+-rw-r--r--   0        0        0        0 2023-07-21 19:14:47.734323 phc-ingestion-0.3.45/ingestion/shared_util/__init__.py
+-rw-r--r--   0        0        0     1669 2023-07-21 19:14:47.734323 phc-ingestion-0.3.45/ingestion/shared_util/coords_to_genes.py
+-rw-r--r--   0        0        0      876 2023-07-21 19:14:47.734323 phc-ingestion-0.3.45/ingestion/shared_util/gene_to_coords.py
+-rw-r--r--   0        0        0     1029 2023-07-21 19:14:47.734323 phc-ingestion-0.3.45/pyproject.toml
+-rw-r--r--   0        0        0      269 1970-01-01 00:00:00.000000 phc-ingestion-0.3.45/PKG-INFO
```

### Comparing `phc-ingestion-0.3.44/ingestion/caris/process.py` & `phc-ingestion-0.3.45/ingestion/caris/process.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.44/ingestion/caris/util/cnv.py` & `phc-ingestion-0.3.45/ingestion/caris/util/cnv.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.44/ingestion/caris/util/detect_genome_ref.py` & `phc-ingestion-0.3.45/ingestion/caris/util/detect_genome_ref.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.44/ingestion/caris/util/ga4gh.py` & `phc-ingestion-0.3.45/ingestion/caris/util/ga4gh.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.44/ingestion/caris/util/interpretation.py` & `phc-ingestion-0.3.45/ingestion/caris/util/interpretation.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.44/ingestion/caris/util/json.py` & `phc-ingestion-0.3.45/ingestion/caris/util/json.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.44/ingestion/caris/util/metadata.py` & `phc-ingestion-0.3.45/ingestion/caris/util/metadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -340,22 +340,22 @@
     test_details = data["testDetails"]
     specimen_details = data["specimenInformation"]["tumorSpecimenInformation"]
 
     physician_details = get_physician_details(data)
 
     metadata["testType"] = get_test_type(str(data))
 
-    #  Get the date without the time
-    metadata["indexedDate"] = test_details["receivedDate"].split()[0]
-
     # Get date of collected and received for the specimen
     metadata["receivedDate"] = get_received_date(specimen_details)
     metadata["collDate"] = get_collected_date(specimen_details)
     metadata["reportDate"] = get_report_date(test_details, log)
 
+    #  Get the date without the time
+    metadata["indexedDate"] = metadata["reportDate"]
+
     patient = data["patientInformation"]
     metadata["bodySiteSystem"] = "http://lifeomic.com/fhir/sequence-body-site"
     metadata["reportID"] = get_report_id(test_details)
     metadata["mrn"] = patient["mrn"]
     metadata["patientLastName"] = patient["lastName"]
 
     metadata["patientDOB"] = patient["dob"]
```

### Comparing `phc-ingestion-0.3.44/ingestion/caris/util/structural.py` & `phc-ingestion-0.3.45/ingestion/caris/util/structural.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.44/ingestion/caris/util/tsv.py` & `phc-ingestion-0.3.45/ingestion/caris/util/tsv.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.44/ingestion/caris/util/vcf.py` & `phc-ingestion-0.3.45/ingestion/caris/util/vcf.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.44/ingestion/foundation/process.py` & `phc-ingestion-0.3.45/ingestion/foundation/process.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.44/ingestion/foundation/util/cnv.py` & `phc-ingestion-0.3.45/ingestion/foundation/util/cnv.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.44/ingestion/foundation/util/fnv.py` & `phc-ingestion-0.3.45/ingestion/foundation/util/fnv.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.44/ingestion/foundation/util/ga4gh.py` & `phc-ingestion-0.3.45/ingestion/foundation/util/ga4gh.py`

 * *Files 4% similar despite different names*

```diff
@@ -124,23 +124,21 @@
 
     trf = get_trf(sample)
 
     med_facil_info = get_med_facil(pmi)
 
     ordering_md_info = get_ordering_md(pmi, npi)
 
-    # fallback on previous behavior for indexedDate if value is not found
-    indexedDate = get_date(pmi.get("CollDate")) or get_date(sample.get("ReceivedDate"))
-
     # store both values sperately
     receivedDate = get_date(sample.get("ReceivedDate"))
     collDate = get_date(pmi.get("CollDate"))
 
     # store date of published report
     reportDate = str(get_date(signatures.get("Signature").get("ServerTime")))[0:10]
+    indexedDate = reportDate
 
     yaml_file = {
         "name": "Foundation Medicine",
         "reference": "GRCh37",
         "sourceFileId": source_file_id,
         "testType": sample.get("TestType"),
         "indexedDate": indexedDate,
```

### Comparing `phc-ingestion-0.3.44/ingestion/foundation/util/vcf_etl.py` & `phc-ingestion-0.3.45/ingestion/foundation/util/vcf_etl.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.44/ingestion/nextgen/process.py` & `phc-ingestion-0.3.45/ingestion/nextgen/process.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.44/ingestion/nextgen/util/process_cnv.py` & `phc-ingestion-0.3.45/ingestion/nextgen/util/process_cnv.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.44/ingestion/nextgen/util/process_manifest.py` & `phc-ingestion-0.3.45/ingestion/nextgen/util/process_manifest.py`

 * *Files 0% similar despite different names*

```diff
@@ -124,14 +124,15 @@
     manifest["medFacilName"] = "IU Health"
 
     for line in patient_info_lines:
         if "reportDate" not in manifest and "Laboratory" in line:
             reportArray = line.split(" ")
             report_date = search_and_grab(reportArray, "Laboratory", 1)
             manifest["reportDate"] = transform_date(report_date)
+            manifest["indexedDate"] = manifest["reportDate"]
 
         if "collDate" not in manifest and "Collected" in line:
             collArray = line.split(" ")
             coll_date = search_and_grab(collArray, "Collected", 1)
             manifest["collDate"] = transform_date(coll_date)
 
         if "receivedDate" not in manifest and "Received" in line:
```

### Comparing `phc-ingestion-0.3.44/ingestion/nextgen/util/process_structural.py` & `phc-ingestion-0.3.45/ingestion/nextgen/util/process_structural.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.44/ingestion/nextgen/util/process_vcf.py` & `phc-ingestion-0.3.45/ingestion/nextgen/util/process_vcf.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.44/ingestion/nextgen/util/variant_table.py` & `phc-ingestion-0.3.45/ingestion/nextgen/util/variant_table.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.44/ingestion/resources/GRCh37_map.csv.gz` & `phc-ingestion-0.3.45/ingestion/resources/GRCh37_map.csv.gz`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.44/ingestion/resources/GRCh38_map.csv.gz` & `phc-ingestion-0.3.45/ingestion/resources/GRCh38_map.csv.gz`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.44/ingestion/shared_util/coords_to_genes.py` & `phc-ingestion-0.3.45/ingestion/shared_util/coords_to_genes.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.44/ingestion/shared_util/gene_to_coords.py` & `phc-ingestion-0.3.45/ingestion/shared_util/gene_to_coords.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.44/pyproject.toml` & `phc-ingestion-0.3.45/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "phc-ingestion"
-version = "0.3.44"
+version = "0.3.45"
 description = "Functions for LifeOmic PHC genomic ingestions"
 authors = [
     { name = "LifeOmic Development", email = "development@lifeomic.com" },
 ]
 dependencies = [
     "lifeomic-logging>=0.3.2,<0.4.0",
     "xmltodict==0.13.0",
```

