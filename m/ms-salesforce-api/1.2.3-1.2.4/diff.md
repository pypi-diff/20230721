# Comparing `tmp/ms_salesforce_api-1.2.3.tar.gz` & `tmp/ms_salesforce_api-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ms_salesforce_api-1.2.3.tar", max compression
+gzip compressed data, was "ms_salesforce_api-1.2.4.tar", max compression
```

## Comparing `ms_salesforce_api-1.2.3.tar` & `ms_salesforce_api-1.2.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    35149 2023-07-21 11:07:42.861020 ms_salesforce_api-1.2.3/LICENSE
--rw-r--r--   0        0        0     8325 2023-07-21 11:07:42.861020 ms_salesforce_api-1.2.3/README.md
--rw-r--r--   0        0        0        0 2023-07-21 11:07:42.861020 ms_salesforce_api-1.2.3/ms_salesforce_api/__init__.py
--rw-r--r--   0        0        0     1491 2023-07-21 11:07:42.861020 ms_salesforce_api-1.2.3/ms_salesforce_api/salesforce/Auth.py
--rw-r--r--   0        0        0     1244 2023-07-21 11:07:42.861020 ms_salesforce_api-1.2.3/ms_salesforce_api/salesforce/JWTGenerator.py
--rw-r--r--   0        0        0     2926 2023-07-21 11:07:42.861020 ms_salesforce_api-1.2.3/ms_salesforce_api/salesforce/SalesforceQueryExecutor.py
--rw-r--r--   0        0        0        0 2023-07-21 11:07:42.861020 ms_salesforce_api-1.2.3/ms_salesforce_api/salesforce/__init__.py
--rw-r--r--   0        0        0        0 2023-07-21 11:07:42.861020 ms_salesforce_api-1.2.3/ms_salesforce_api/salesforce/__tests__/__init__.py
--rw-r--r--   0        0        0     2749 2023-07-21 11:07:42.861020 ms_salesforce_api-1.2.3/ms_salesforce_api/salesforce/__tests__/test_Auth.py
--rw-r--r--   0        0        0     2205 2023-07-21 11:07:42.861020 ms_salesforce_api-1.2.3/ms_salesforce_api/salesforce/__tests__/test_JWTGenerator.py
--rw-r--r--   0        0        0     5168 2023-07-21 11:07:42.861020 ms_salesforce_api-1.2.3/ms_salesforce_api/salesforce/__tests__/test_SalesforceRequester.py
--rw-r--r--   0        0        0     3541 2023-07-21 11:07:42.861020 ms_salesforce_api-1.2.3/ms_salesforce_api/salesforce/project/__init__.py
--rw-r--r--   0        0        0        0 2023-07-21 11:07:42.865020 ms_salesforce_api-1.2.3/ms_salesforce_api/salesforce/project/__tests__/__init__.py
--rw-r--r--   0        0        0    15342 2023-07-21 11:07:42.865020 ms_salesforce_api-1.2.3/ms_salesforce_api/salesforce/project/__tests__/test_Project.py
--rw-r--r--   0        0        0     9629 2023-07-21 11:07:42.865020 ms_salesforce_api-1.2.3/ms_salesforce_api/salesforce/project/constants.py
--rw-r--r--   0        0        0     3804 2023-07-21 11:07:42.865020 ms_salesforce_api-1.2.3/ms_salesforce_api/salesforce/project/dto/BillingLineDTO.py
--rw-r--r--   0        0        0    25154 2023-07-21 11:07:42.865020 ms_salesforce_api-1.2.3/ms_salesforce_api/salesforce/project/dto/OpportunityDTO.py
--rw-r--r--   0        0        0     2166 2023-07-21 11:07:42.865020 ms_salesforce_api-1.2.3/ms_salesforce_api/salesforce/project/dto/ProjectLineItemDTO.py
--rw-r--r--   0        0        0        0 2023-07-21 11:07:42.865020 ms_salesforce_api-1.2.3/ms_salesforce_api/salesforce/project/dto/__init__.py
--rw-r--r--   0        0        0    28646 2023-07-21 11:07:42.865020 ms_salesforce_api-1.2.3/ms_salesforce_api/salesforce/project/export_data/Bigquery.py
--rw-r--r--   0        0        0    12590 2023-07-21 11:07:42.865020 ms_salesforce_api-1.2.3/ms_salesforce_api/salesforce/project/export_data/CloudSQL.py
--rw-r--r--   0        0        0        0 2023-07-21 11:07:42.865020 ms_salesforce_api-1.2.3/ms_salesforce_api/salesforce/project/export_data/__init__.py
--rw-r--r--   0        0        0        0 2023-07-21 11:07:42.865020 ms_salesforce_api-1.2.3/ms_salesforce_api/salesforce/project/export_data/__tests__/__init__.py
--rw-r--r--   0        0        0    20263 2023-07-21 11:07:42.865020 ms_salesforce_api-1.2.3/ms_salesforce_api/salesforce/project/export_data/__tests__/test_Bigquery.py
--rw-r--r--   0        0        0    13717 2023-07-21 11:07:42.865020 ms_salesforce_api-1.2.3/ms_salesforce_api/salesforce/project/export_data/__tests__/test_CloudSQL.py
--rw-r--r--   0        0        0      303 2023-07-21 11:07:42.865020 ms_salesforce_api-1.2.3/ms_salesforce_api/salesforce/project/helpers.py
--rw-r--r--   0        0        0     1055 2023-07-21 11:07:42.865020 ms_salesforce_api-1.2.3/pyproject.toml
--rw-r--r--   0        0        0     9101 1970-01-01 00:00:00.000000 ms_salesforce_api-1.2.3/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-21 11:35:43.860589 ms_salesforce_api-1.2.4/LICENSE
+-rw-r--r--   0        0        0     8325 2023-07-21 11:35:43.860589 ms_salesforce_api-1.2.4/README.md
+-rw-r--r--   0        0        0        0 2023-07-21 11:35:43.860589 ms_salesforce_api-1.2.4/ms_salesforce_api/__init__.py
+-rw-r--r--   0        0        0     1491 2023-07-21 11:35:43.860589 ms_salesforce_api-1.2.4/ms_salesforce_api/salesforce/Auth.py
+-rw-r--r--   0        0        0     1244 2023-07-21 11:35:43.860589 ms_salesforce_api-1.2.4/ms_salesforce_api/salesforce/JWTGenerator.py
+-rw-r--r--   0        0        0     2926 2023-07-21 11:35:43.860589 ms_salesforce_api-1.2.4/ms_salesforce_api/salesforce/SalesforceQueryExecutor.py
+-rw-r--r--   0        0        0        0 2023-07-21 11:35:43.860589 ms_salesforce_api-1.2.4/ms_salesforce_api/salesforce/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-21 11:35:43.860589 ms_salesforce_api-1.2.4/ms_salesforce_api/salesforce/__tests__/__init__.py
+-rw-r--r--   0        0        0     2749 2023-07-21 11:35:43.860589 ms_salesforce_api-1.2.4/ms_salesforce_api/salesforce/__tests__/test_Auth.py
+-rw-r--r--   0        0        0     2205 2023-07-21 11:35:43.860589 ms_salesforce_api-1.2.4/ms_salesforce_api/salesforce/__tests__/test_JWTGenerator.py
+-rw-r--r--   0        0        0     5168 2023-07-21 11:35:43.860589 ms_salesforce_api-1.2.4/ms_salesforce_api/salesforce/__tests__/test_SalesforceRequester.py
+-rw-r--r--   0        0        0     3541 2023-07-21 11:35:43.860589 ms_salesforce_api-1.2.4/ms_salesforce_api/salesforce/project/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-21 11:35:43.860589 ms_salesforce_api-1.2.4/ms_salesforce_api/salesforce/project/__tests__/__init__.py
+-rw-r--r--   0        0        0    15342 2023-07-21 11:35:43.860589 ms_salesforce_api-1.2.4/ms_salesforce_api/salesforce/project/__tests__/test_Project.py
+-rw-r--r--   0        0        0     9629 2023-07-21 11:35:43.860589 ms_salesforce_api-1.2.4/ms_salesforce_api/salesforce/project/constants.py
+-rw-r--r--   0        0        0     3804 2023-07-21 11:35:43.860589 ms_salesforce_api-1.2.4/ms_salesforce_api/salesforce/project/dto/BillingLineDTO.py
+-rw-r--r--   0        0        0    25154 2023-07-21 11:35:43.860589 ms_salesforce_api-1.2.4/ms_salesforce_api/salesforce/project/dto/OpportunityDTO.py
+-rw-r--r--   0        0        0     2166 2023-07-21 11:35:43.860589 ms_salesforce_api-1.2.4/ms_salesforce_api/salesforce/project/dto/ProjectLineItemDTO.py
+-rw-r--r--   0        0        0        0 2023-07-21 11:35:43.860589 ms_salesforce_api-1.2.4/ms_salesforce_api/salesforce/project/dto/__init__.py
+-rw-r--r--   0        0        0    28712 2023-07-21 11:35:43.860589 ms_salesforce_api-1.2.4/ms_salesforce_api/salesforce/project/export_data/Bigquery.py
+-rw-r--r--   0        0        0    12590 2023-07-21 11:35:43.860589 ms_salesforce_api-1.2.4/ms_salesforce_api/salesforce/project/export_data/CloudSQL.py
+-rw-r--r--   0        0        0        0 2023-07-21 11:35:43.860589 ms_salesforce_api-1.2.4/ms_salesforce_api/salesforce/project/export_data/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-21 11:35:43.860589 ms_salesforce_api-1.2.4/ms_salesforce_api/salesforce/project/export_data/__tests__/__init__.py
+-rw-r--r--   0        0        0    20263 2023-07-21 11:35:43.860589 ms_salesforce_api-1.2.4/ms_salesforce_api/salesforce/project/export_data/__tests__/test_Bigquery.py
+-rw-r--r--   0        0        0    13717 2023-07-21 11:35:43.860589 ms_salesforce_api-1.2.4/ms_salesforce_api/salesforce/project/export_data/__tests__/test_CloudSQL.py
+-rw-r--r--   0        0        0      303 2023-07-21 11:35:43.860589 ms_salesforce_api-1.2.4/ms_salesforce_api/salesforce/project/helpers.py
+-rw-r--r--   0        0        0     1055 2023-07-21 11:35:43.860589 ms_salesforce_api-1.2.4/pyproject.toml
+-rw-r--r--   0        0        0     9101 1970-01-01 00:00:00.000000 ms_salesforce_api-1.2.4/PKG-INFO
```

### Comparing `ms_salesforce_api-1.2.3/LICENSE` & `ms_salesforce_api-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-1.2.3/README.md` & `ms_salesforce_api-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-1.2.3/ms_salesforce_api/salesforce/Auth.py` & `ms_salesforce_api-1.2.4/ms_salesforce_api/salesforce/Auth.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-1.2.3/ms_salesforce_api/salesforce/JWTGenerator.py` & `ms_salesforce_api-1.2.4/ms_salesforce_api/salesforce/JWTGenerator.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-1.2.3/ms_salesforce_api/salesforce/SalesforceQueryExecutor.py` & `ms_salesforce_api-1.2.4/ms_salesforce_api/salesforce/SalesforceQueryExecutor.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-1.2.3/ms_salesforce_api/salesforce/__tests__/test_Auth.py` & `ms_salesforce_api-1.2.4/ms_salesforce_api/salesforce/__tests__/test_Auth.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-1.2.3/ms_salesforce_api/salesforce/__tests__/test_JWTGenerator.py` & `ms_salesforce_api-1.2.4/ms_salesforce_api/salesforce/__tests__/test_JWTGenerator.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-1.2.3/ms_salesforce_api/salesforce/__tests__/test_SalesforceRequester.py` & `ms_salesforce_api-1.2.4/ms_salesforce_api/salesforce/__tests__/test_SalesforceRequester.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-1.2.3/ms_salesforce_api/salesforce/project/__init__.py` & `ms_salesforce_api-1.2.4/ms_salesforce_api/salesforce/project/__init__.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-1.2.3/ms_salesforce_api/salesforce/project/__tests__/test_Project.py` & `ms_salesforce_api-1.2.4/ms_salesforce_api/salesforce/project/__tests__/test_Project.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-1.2.3/ms_salesforce_api/salesforce/project/constants.py` & `ms_salesforce_api-1.2.4/ms_salesforce_api/salesforce/project/constants.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-1.2.3/ms_salesforce_api/salesforce/project/dto/BillingLineDTO.py` & `ms_salesforce_api-1.2.4/ms_salesforce_api/salesforce/project/dto/BillingLineDTO.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-1.2.3/ms_salesforce_api/salesforce/project/dto/OpportunityDTO.py` & `ms_salesforce_api-1.2.4/ms_salesforce_api/salesforce/project/dto/OpportunityDTO.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-1.2.3/ms_salesforce_api/salesforce/project/dto/ProjectLineItemDTO.py` & `ms_salesforce_api-1.2.4/ms_salesforce_api/salesforce/project/dto/ProjectLineItemDTO.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-1.2.3/ms_salesforce_api/salesforce/project/export_data/Bigquery.py` & `ms_salesforce_api-1.2.4/ms_salesforce_api/salesforce/project/export_data/Bigquery.py`

 * *Files 0% similar despite different names*

```diff
@@ -721,14 +721,16 @@
                 query=insert_group_query,
                 log_id="INSERT_accounts",
             )
 
     def _export_subgroups(self, opportunities):
         group_values = []
         for opp in opportunities:
+            if not opp["group_groupid"]:
+                continue
             group_id = (
                 f'"{opp["group_groupid"]}"' if opp["group_groupid"] else "NULL"
             )
             subgroup_id = (
                 f'"{opp["subgroup_subgroupid"]}"'
                 if opp["subgroup_subgroupid"]
                 else "NULL"
```

### Comparing `ms_salesforce_api-1.2.3/ms_salesforce_api/salesforce/project/export_data/CloudSQL.py` & `ms_salesforce_api-1.2.4/ms_salesforce_api/salesforce/project/export_data/CloudSQL.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-1.2.3/ms_salesforce_api/salesforce/project/export_data/__tests__/test_Bigquery.py` & `ms_salesforce_api-1.2.4/ms_salesforce_api/salesforce/project/export_data/__tests__/test_Bigquery.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-1.2.3/ms_salesforce_api/salesforce/project/export_data/__tests__/test_CloudSQL.py` & `ms_salesforce_api-1.2.4/ms_salesforce_api/salesforce/project/export_data/__tests__/test_CloudSQL.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-1.2.3/pyproject.toml` & `ms_salesforce_api-1.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ms-salesforce-api"
-version = "1.2.3"
+version = "1.2.4"
 description = "Python library used to extract data from Salesforce API and migrate it to Bigquery and Postgres."
 authors = ["Making Science"]
 readme = "README.md"
 packages = [{include = "ms_salesforce_api"}]
 include = ["pre-commit-config.yaml"]
 
 [tool.poetry.dependencies]
```

### Comparing `ms_salesforce_api-1.2.3/PKG-INFO` & `ms_salesforce_api-1.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ms-salesforce-api
-Version: 1.2.3
+Version: 1.2.4
 Summary: Python library used to extract data from Salesforce API and migrate it to Bigquery and Postgres.
 Author: Making Science
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

