# Comparing `tmp/ms_salesforce_api-1.2.2.tar.gz` & `tmp/ms_salesforce_api-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ms_salesforce_api-1.2.2.tar", max compression
+gzip compressed data, was "ms_salesforce_api-1.2.3.tar", max compression
```

## Comparing `ms_salesforce_api-1.2.2.tar` & `ms_salesforce_api-1.2.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    35149 2023-07-20 09:03:45.688746 ms_salesforce_api-1.2.2/LICENSE
--rw-r--r--   0        0        0     8325 2023-07-20 09:03:45.688746 ms_salesforce_api-1.2.2/README.md
--rw-r--r--   0        0        0        0 2023-07-20 09:03:45.692746 ms_salesforce_api-1.2.2/ms_salesforce_api/__init__.py
--rw-r--r--   0        0        0     1491 2023-07-20 09:03:45.692746 ms_salesforce_api-1.2.2/ms_salesforce_api/salesforce/Auth.py
--rw-r--r--   0        0        0     1244 2023-07-20 09:03:45.692746 ms_salesforce_api-1.2.2/ms_salesforce_api/salesforce/JWTGenerator.py
--rw-r--r--   0        0        0     2926 2023-07-20 09:03:45.692746 ms_salesforce_api-1.2.2/ms_salesforce_api/salesforce/SalesforceQueryExecutor.py
--rw-r--r--   0        0        0        0 2023-07-20 09:03:45.692746 ms_salesforce_api-1.2.2/ms_salesforce_api/salesforce/__init__.py
--rw-r--r--   0        0        0        0 2023-07-20 09:03:45.692746 ms_salesforce_api-1.2.2/ms_salesforce_api/salesforce/__tests__/__init__.py
--rw-r--r--   0        0        0     2749 2023-07-20 09:03:45.692746 ms_salesforce_api-1.2.2/ms_salesforce_api/salesforce/__tests__/test_Auth.py
--rw-r--r--   0        0        0     2205 2023-07-20 09:03:45.692746 ms_salesforce_api-1.2.2/ms_salesforce_api/salesforce/__tests__/test_JWTGenerator.py
--rw-r--r--   0        0        0     5168 2023-07-20 09:03:45.692746 ms_salesforce_api-1.2.2/ms_salesforce_api/salesforce/__tests__/test_SalesforceRequester.py
--rw-r--r--   0        0        0     3541 2023-07-20 09:03:45.692746 ms_salesforce_api-1.2.2/ms_salesforce_api/salesforce/project/__init__.py
--rw-r--r--   0        0        0        0 2023-07-20 09:03:45.692746 ms_salesforce_api-1.2.2/ms_salesforce_api/salesforce/project/__tests__/__init__.py
--rw-r--r--   0        0        0    15342 2023-07-20 09:03:45.692746 ms_salesforce_api-1.2.2/ms_salesforce_api/salesforce/project/__tests__/test_Project.py
--rw-r--r--   0        0        0     9585 2023-07-20 09:03:45.692746 ms_salesforce_api-1.2.2/ms_salesforce_api/salesforce/project/constants.py
--rw-r--r--   0        0        0     3804 2023-07-20 09:03:45.692746 ms_salesforce_api-1.2.2/ms_salesforce_api/salesforce/project/dto/BillingLineDTO.py
--rw-r--r--   0        0        0    25094 2023-07-20 09:03:45.692746 ms_salesforce_api-1.2.2/ms_salesforce_api/salesforce/project/dto/OpportunityDTO.py
--rw-r--r--   0        0        0     2166 2023-07-20 09:03:45.692746 ms_salesforce_api-1.2.2/ms_salesforce_api/salesforce/project/dto/ProjectLineItemDTO.py
--rw-r--r--   0        0        0        0 2023-07-20 09:03:45.692746 ms_salesforce_api-1.2.2/ms_salesforce_api/salesforce/project/dto/__init__.py
--rw-r--r--   0        0        0    28320 2023-07-20 09:03:45.692746 ms_salesforce_api-1.2.2/ms_salesforce_api/salesforce/project/export_data/Bigquery.py
--rw-r--r--   0        0        0    12570 2023-07-20 09:03:45.692746 ms_salesforce_api-1.2.2/ms_salesforce_api/salesforce/project/export_data/CloudSQL.py
--rw-r--r--   0        0        0        0 2023-07-20 09:03:45.692746 ms_salesforce_api-1.2.2/ms_salesforce_api/salesforce/project/export_data/__init__.py
--rw-r--r--   0        0        0        0 2023-07-20 09:03:45.692746 ms_salesforce_api-1.2.2/ms_salesforce_api/salesforce/project/export_data/__tests__/__init__.py
--rw-r--r--   0        0        0    20129 2023-07-20 09:03:45.692746 ms_salesforce_api-1.2.2/ms_salesforce_api/salesforce/project/export_data/__tests__/test_Bigquery.py
--rw-r--r--   0        0        0    13717 2023-07-20 09:03:45.692746 ms_salesforce_api-1.2.2/ms_salesforce_api/salesforce/project/export_data/__tests__/test_CloudSQL.py
--rw-r--r--   0        0        0      303 2023-07-20 09:03:45.692746 ms_salesforce_api-1.2.2/ms_salesforce_api/salesforce/project/helpers.py
--rw-r--r--   0        0        0     1055 2023-07-20 09:03:45.692746 ms_salesforce_api-1.2.2/pyproject.toml
--rw-r--r--   0        0        0     9101 1970-01-01 00:00:00.000000 ms_salesforce_api-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-21 11:07:42.861020 ms_salesforce_api-1.2.3/LICENSE
+-rw-r--r--   0        0        0     8325 2023-07-21 11:07:42.861020 ms_salesforce_api-1.2.3/README.md
+-rw-r--r--   0        0        0        0 2023-07-21 11:07:42.861020 ms_salesforce_api-1.2.3/ms_salesforce_api/__init__.py
+-rw-r--r--   0        0        0     1491 2023-07-21 11:07:42.861020 ms_salesforce_api-1.2.3/ms_salesforce_api/salesforce/Auth.py
+-rw-r--r--   0        0        0     1244 2023-07-21 11:07:42.861020 ms_salesforce_api-1.2.3/ms_salesforce_api/salesforce/JWTGenerator.py
+-rw-r--r--   0        0        0     2926 2023-07-21 11:07:42.861020 ms_salesforce_api-1.2.3/ms_salesforce_api/salesforce/SalesforceQueryExecutor.py
+-rw-r--r--   0        0        0        0 2023-07-21 11:07:42.861020 ms_salesforce_api-1.2.3/ms_salesforce_api/salesforce/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-21 11:07:42.861020 ms_salesforce_api-1.2.3/ms_salesforce_api/salesforce/__tests__/__init__.py
+-rw-r--r--   0        0        0     2749 2023-07-21 11:07:42.861020 ms_salesforce_api-1.2.3/ms_salesforce_api/salesforce/__tests__/test_Auth.py
+-rw-r--r--   0        0        0     2205 2023-07-21 11:07:42.861020 ms_salesforce_api-1.2.3/ms_salesforce_api/salesforce/__tests__/test_JWTGenerator.py
+-rw-r--r--   0        0        0     5168 2023-07-21 11:07:42.861020 ms_salesforce_api-1.2.3/ms_salesforce_api/salesforce/__tests__/test_SalesforceRequester.py
+-rw-r--r--   0        0        0     3541 2023-07-21 11:07:42.861020 ms_salesforce_api-1.2.3/ms_salesforce_api/salesforce/project/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-21 11:07:42.865020 ms_salesforce_api-1.2.3/ms_salesforce_api/salesforce/project/__tests__/__init__.py
+-rw-r--r--   0        0        0    15342 2023-07-21 11:07:42.865020 ms_salesforce_api-1.2.3/ms_salesforce_api/salesforce/project/__tests__/test_Project.py
+-rw-r--r--   0        0        0     9629 2023-07-21 11:07:42.865020 ms_salesforce_api-1.2.3/ms_salesforce_api/salesforce/project/constants.py
+-rw-r--r--   0        0        0     3804 2023-07-21 11:07:42.865020 ms_salesforce_api-1.2.3/ms_salesforce_api/salesforce/project/dto/BillingLineDTO.py
+-rw-r--r--   0        0        0    25154 2023-07-21 11:07:42.865020 ms_salesforce_api-1.2.3/ms_salesforce_api/salesforce/project/dto/OpportunityDTO.py
+-rw-r--r--   0        0        0     2166 2023-07-21 11:07:42.865020 ms_salesforce_api-1.2.3/ms_salesforce_api/salesforce/project/dto/ProjectLineItemDTO.py
+-rw-r--r--   0        0        0        0 2023-07-21 11:07:42.865020 ms_salesforce_api-1.2.3/ms_salesforce_api/salesforce/project/dto/__init__.py
+-rw-r--r--   0        0        0    28646 2023-07-21 11:07:42.865020 ms_salesforce_api-1.2.3/ms_salesforce_api/salesforce/project/export_data/Bigquery.py
+-rw-r--r--   0        0        0    12590 2023-07-21 11:07:42.865020 ms_salesforce_api-1.2.3/ms_salesforce_api/salesforce/project/export_data/CloudSQL.py
+-rw-r--r--   0        0        0        0 2023-07-21 11:07:42.865020 ms_salesforce_api-1.2.3/ms_salesforce_api/salesforce/project/export_data/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-21 11:07:42.865020 ms_salesforce_api-1.2.3/ms_salesforce_api/salesforce/project/export_data/__tests__/__init__.py
+-rw-r--r--   0        0        0    20263 2023-07-21 11:07:42.865020 ms_salesforce_api-1.2.3/ms_salesforce_api/salesforce/project/export_data/__tests__/test_Bigquery.py
+-rw-r--r--   0        0        0    13717 2023-07-21 11:07:42.865020 ms_salesforce_api-1.2.3/ms_salesforce_api/salesforce/project/export_data/__tests__/test_CloudSQL.py
+-rw-r--r--   0        0        0      303 2023-07-21 11:07:42.865020 ms_salesforce_api-1.2.3/ms_salesforce_api/salesforce/project/helpers.py
+-rw-r--r--   0        0        0     1055 2023-07-21 11:07:42.865020 ms_salesforce_api-1.2.3/pyproject.toml
+-rw-r--r--   0        0        0     9101 1970-01-01 00:00:00.000000 ms_salesforce_api-1.2.3/PKG-INFO
```

### Comparing `ms_salesforce_api-1.2.2/LICENSE` & `ms_salesforce_api-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-1.2.2/README.md` & `ms_salesforce_api-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-1.2.2/ms_salesforce_api/salesforce/Auth.py` & `ms_salesforce_api-1.2.3/ms_salesforce_api/salesforce/Auth.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-1.2.2/ms_salesforce_api/salesforce/JWTGenerator.py` & `ms_salesforce_api-1.2.3/ms_salesforce_api/salesforce/JWTGenerator.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-1.2.2/ms_salesforce_api/salesforce/SalesforceQueryExecutor.py` & `ms_salesforce_api-1.2.3/ms_salesforce_api/salesforce/SalesforceQueryExecutor.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-1.2.2/ms_salesforce_api/salesforce/__tests__/test_Auth.py` & `ms_salesforce_api-1.2.3/ms_salesforce_api/salesforce/__tests__/test_Auth.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-1.2.2/ms_salesforce_api/salesforce/__tests__/test_JWTGenerator.py` & `ms_salesforce_api-1.2.3/ms_salesforce_api/salesforce/__tests__/test_JWTGenerator.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-1.2.2/ms_salesforce_api/salesforce/__tests__/test_SalesforceRequester.py` & `ms_salesforce_api-1.2.3/ms_salesforce_api/salesforce/__tests__/test_SalesforceRequester.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-1.2.2/ms_salesforce_api/salesforce/project/__init__.py` & `ms_salesforce_api-1.2.3/ms_salesforce_api/salesforce/project/__init__.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-1.2.2/ms_salesforce_api/salesforce/project/__tests__/test_Project.py` & `ms_salesforce_api-1.2.3/ms_salesforce_api/salesforce/project/__tests__/test_Project.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-1.2.2/ms_salesforce_api/salesforce/project/constants.py` & `ms_salesforce_api-1.2.3/ms_salesforce_api/salesforce/project/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,15 +87,15 @@
             Country__c
         FROM
             Project_Line_Items__r
     )
 FROM
     Project__c
 """
-# Project__c   WHERE Id = 'a003X000015kaPxQAI'
+# Project__c   WHERE Id = 'a00AX000002DVi1YAG'
 
 DEFAULT_PROJECT_BILLING_LINE_QUERY = """
 SELECT
     Id,
     Name,
     Project_Line_Item__r.Project__c,
     CurrencyIsoCode,
@@ -219,33 +219,36 @@
     invoicing_email  VARCHAR(500) DEFAULT NULL,
     FOREIGN KEY (project_id) REFERENCES Opportunities(project_id)
 );
 """
 
 DEFAULT_GROUPS_CREATE_TABLE_QUERY = """
 CREATE TABLE Groups (
-    id VARCHAR(255) PRIMARY KEY,
+    id SERIAL PRIMARY KEY,
+    groupid VARCHAR(255) NOT NULL,
     project_id VARCHAR(255) DEFAULT NULL,
     name VARCHAR(255) DEFAULT NULL,
     start_date VARCHAR(255) DEFAULT NULL,
     end_date VARCHAR(255) DEFAULT NULL,
     bqid VARCHAR(255) DEFAULT NULL,
     pck_type VARCHAR(255) DEFAULT NULL,
+
     FOREIGN KEY (project_id) REFERENCES Opportunities(project_id)
 );
 """
 
 DEFAULT_SUBGROUPS_CREATE_TABLE_QUERY = """
 CREATE TABLE SubGroups (
-    group_id VARCHAR(255) DEFAULT NULL,
+    id SERIAL PRIMARY KEY,
+    groupid VARCHAR(255) NOT NULL,
+    subgroupid VARCHAR(255) DEFAULT NULL,
     name VARCHAR(255) DEFAULT NULL,
     start_date VARCHAR(255) DEFAULT NULL,
     end_date VARCHAR(255) DEFAULT NULL,
-    bqid VARCHAR(255) DEFAULT NULL,
-    FOREIGN KEY (group_id) REFERENCES Groups(id)
+    bqid VARCHAR(255) DEFAULT NULL
 );
 """
 
 DEFAULT_POSTGRES_DATABASE_SCHEMAS_MAP = [
     {
         "db_name": "Opportunities",
         "query": DEFAULT_OPPORTUNITIES_CREATE_TABLE_QUERY,
```

### Comparing `ms_salesforce_api-1.2.2/ms_salesforce_api/salesforce/project/dto/BillingLineDTO.py` & `ms_salesforce_api-1.2.3/ms_salesforce_api/salesforce/project/dto/BillingLineDTO.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-1.2.2/ms_salesforce_api/salesforce/project/dto/OpportunityDTO.py` & `ms_salesforce_api-1.2.3/ms_salesforce_api/salesforce/project/dto/OpportunityDTO.py`

 * *Files 0% similar despite different names*

```diff
@@ -650,19 +650,20 @@
             "account_billing_street": self.account_billing_street,
             "account_company_invoicing": self.account_company_invoicing,
             "account_office": self.account_office,
             "account_payment_terms": self.account_payment_terms,
             "account_billing_state_code": self.account_billing_state_code,
             "account_mail_invoicing": self.account_mail_invoicing,
             "account_invoicing_email": self.account_invoicing_email,
-            "group_id": self.group_id,
+            "group_groupid": self.group_id,
             "group_name": self.group_name,
             "group_start_date": self.group_start_date,
             "group_end_date": self.group_end_date,
             "group_bqid": self.group_bqid,
             "group_pck_type": self.group_pck_type,
             "subgroup_name": self.subgroup_name,
             "subgroup_start_date": self.subgroup_start_date,
             "subgroup_end_date": self.subgroup_end_date,
             "subgroup_bqid": self.subgroup_bqid,
-            "subgroup_id": self.subgroup_id,
+            "subgroup_subgroupid": self.subgroup_id,
+            "subgroup_groupid": self.group_id,
         }
```

### Comparing `ms_salesforce_api-1.2.2/ms_salesforce_api/salesforce/project/dto/ProjectLineItemDTO.py` & `ms_salesforce_api-1.2.3/ms_salesforce_api/salesforce/project/dto/ProjectLineItemDTO.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-1.2.2/ms_salesforce_api/salesforce/project/export_data/Bigquery.py` & `ms_salesforce_api-1.2.3/ms_salesforce_api/salesforce/project/export_data/Bigquery.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,25 +112,25 @@
                 "tax_classification": "STRING",
                 "tax_id_type": "STRING",
                 "tier": "STRING",
                 "website": "STRING",
             },
             "groups": {
                 "project_id": "STRING",
-                "id": "STRING",
+                "groupid": "STRING",
                 "name": "STRING",
                 "start_date": "STRING",
                 "end_date": "STRING",
                 "bqid": "STRING",
                 "pck_type": "STRING",
             },
             "subgroups": {
-                "project_id": "STRING",
-                "group_id": "STRING",
+                "groupid": "STRING",
                 "name": "STRING",
+                "subgroupid": "STRING",
                 "start_date": "STRING",
                 "end_date": "STRING",
                 "bqid": "STRING",
             },
         }
 
         for table_name, table_schema in self.schemas.items():
@@ -142,15 +142,15 @@
         result = self.client.execute_query(
             query,
             custom_error_value,
         )
 
         if result == custom_error_value:
             logging.error(
-                "[ERROR - _execute_query]: Error executing query for {log_id} in BigQuery."
+                f"[ERROR - _execute_query]: Error executing query for {log_id} in BigQuery."
             )
             result = default_error_value
 
         return result
 
     def _export_opportunities(self, opportunities):
         opportunities_values = []
@@ -651,15 +651,17 @@
             self._execute_query(
                 query=insert_accounts_query, log_id="INSERT_accounts"
             )
 
     def _export_groups(self, opportunities):
         group_values = []
         for opp in opportunities:
-            group_id = f'"{opp["group_id"]}"' if opp["group_id"] else "NULL"
+            group_id = (
+                f'"{opp["group_groupid"]}"' if opp["group_groupid"] else "NULL"
+            )
             group_name = (
                 f'"{opp["group_name"]}"' if opp["group_name"] else "NULL"
             )
 
             group_start = (
                 f'"{opp["group_start_date"]}"'
                 if opp["group_start_date"]
@@ -697,15 +699,15 @@
                 """
             )
 
         if group_values:
             insert_group_query = f"""
                 INSERT INTO `{self.project_id}.{self.dataset_id}.groups` (
                     project_id,
-                    id,
+                    groupid,
                     name,
                     start_date,
                     end_date,
                     bqid,
                     pck_type
                 ) VALUES {', '.join(group_values)};
             """
@@ -719,15 +721,22 @@
                 query=insert_group_query,
                 log_id="INSERT_accounts",
             )
 
     def _export_subgroups(self, opportunities):
         group_values = []
         for opp in opportunities:
-            group_id = f'"{opp["group_id"]}"' if opp["group_id"] else "NULL"
+            group_id = (
+                f'"{opp["group_groupid"]}"' if opp["group_groupid"] else "NULL"
+            )
+            subgroup_id = (
+                f'"{opp["subgroup_subgroupid"]}"'
+                if opp["subgroup_subgroupid"]
+                else "NULL"
+            )
             subgroup_name = (
                 f'"{opp["subgroup_name"]}"' if opp["subgroup_name"] else "NULL"
             )
 
             subgroup_start = (
                 f'"{opp["subgroup_start_date"]}"'
                 if opp["subgroup_start_date"]
@@ -744,26 +753,28 @@
                 f'"{opp["subgroup_bqid"]}"' if opp["subgroup_bqid"] else "NULL"
             )
 
             group_values.append(
                 f"""
                 (
                     {group_id},
+                    {subgroup_id},
                     {subgroup_name},
                     {subgroup_start},
                     {subgroup_end},
                     {subgroup_bqid}
                 )
                 """
             )
 
         if group_values:
             insert_group_query = f"""
                 INSERT INTO `{self.project_id}.{self.dataset_id}.subgroups` (
-                    group_id,
+                    groupid,
+                    subgroupid,
                     name,
                     start_date,
                     end_date,
                     bqid
                 ) VALUES {', '.join(group_values)};
             """
             insert_group_query = (
```

### Comparing `ms_salesforce_api-1.2.2/ms_salesforce_api/salesforce/project/export_data/CloudSQL.py` & `ms_salesforce_api-1.2.3/ms_salesforce_api/salesforce/project/export_data/CloudSQL.py`

 * *Files 1% similar despite different names*

```diff
@@ -291,16 +291,16 @@
             {
                 key.replace("group_", ""): (value if value != "" else None)
                 for key, value in opportunity.items()
                 if ("group_" in key and "subgroup_" not in key)
                 or "project_id" == key
             }
             for opportunity in opportunities
-            if opportunity.get("group_id") is not None
-            and opportunity.get("group_id") != ""
+            if opportunity.get("group_groupid") is not None
+            and opportunity.get("group_groupid") != ""
         ]
 
         if opportunity_fixed:
             insert_query = sql.SQL(
                 """
                 INSERT INTO Groups ({})
                 VALUES ({})
@@ -333,16 +333,16 @@
         opportunity_fixed = [
             {
                 key.replace("subgroup_", ""): (value if value != "" else None)
                 for key, value in opportunity.items()
                 if "subgroup_" in key
             }
             for opportunity in opportunities
-            if opportunity.get("group_id") is not None
-            and opportunity.get("group_id") != ""
+            if opportunity.get("group_groupid") is not None
+            and opportunity.get("group_groupid") != ""
         ]
 
         if opportunity_fixed:
             insert_query = sql.SQL(
                 """
                 INSERT INTO SubGroups ({})
                 VALUES ({})
```

### Comparing `ms_salesforce_api-1.2.2/ms_salesforce_api/salesforce/project/export_data/__tests__/test_Bigquery.py` & `ms_salesforce_api-1.2.3/ms_salesforce_api/salesforce/project/export_data/__tests__/test_Bigquery.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,25 +91,26 @@
                 "account_billing_street": "12 Strickland Avenue",
                 "account_company_invoicing": "2411",
                 "account_office": "1313X000000Y5DEQA0",
                 "account_payment_terms": "T060",
                 "account_billing_state_code": "ON",
                 "account_mail_invoicing": None,
                 "account_invoicing_email": "test@5822.group",
-                "group_id": "group_id_test",
+                "group_groupid": "group_id_test",
                 "group_name": "group_name_test",
                 "group_start_date": "group_start_date_test",
                 "group_end_date": "group_end_date_test",
                 "group_bqid": "group_bqid_test",
                 "group_pck_type": "group_pck_type_test",
                 "subgroup_name": "subgroup_name_test",
                 "subgroup_start_date": "subgroup_start_date_test",
                 "subgroup_end_date": "subgroup_end_date_test",
                 "subgroup_bqid": "subgroup_bqid_test",
-                "subgroup_id": "subgroup_id_test",
+                "subgroup_subgroupid": "subgroup_id_test",
+                "subgroup_groupid": "group_id_test",
             },
         ]
 
         self.mock_bigquery_manager = mock.patch(
             "gc_google_services_api.bigquery.BigQueryManager"
         ).start()
         from ..Bigquery import BigQueryExporter
@@ -467,15 +468,15 @@
                 )
                 ;
         """
 
         expected_group_query = """
             INSERT INTO `your-project-id.your-dataset-id.groups`(
                 project_id,
-                id,
+                groupid,
                 name,
                 start_date,
                 end_date,
                 bqid,
                 pck_type
             ) VALUES(
                 "a003X000015kaPxQAI",
@@ -486,21 +487,23 @@
                 "group_bqid_test",
                 "group_pck_type_test"
             );
         """
 
         expected_subgroup_query = """
             INSERT INTO `your-project-id.your-dataset-id.subgroups`(
-                group_id,
+                groupid,
+                subgroupid,
                 name,
                 start_date,
                 end_date,
                 bqid
             ) VALUES (
                 "group_id_test",
+                "subgroup_id_test",
                 "subgroup_name_test",
                 "subgroup_start_date_test",
                 "subgroup_end_date_test",
                 "subgroup_bqid_test"
             );
         """
```

### Comparing `ms_salesforce_api-1.2.2/ms_salesforce_api/salesforce/project/export_data/__tests__/test_CloudSQL.py` & `ms_salesforce_api-1.2.3/ms_salesforce_api/salesforce/project/export_data/__tests__/test_CloudSQL.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-1.2.2/pyproject.toml` & `ms_salesforce_api-1.2.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ms-salesforce-api"
-version = "1.2.2"
+version = "1.2.3"
 description = "Python library used to extract data from Salesforce API and migrate it to Bigquery and Postgres."
 authors = ["Making Science"]
 readme = "README.md"
 packages = [{include = "ms_salesforce_api"}]
 include = ["pre-commit-config.yaml"]
 
 [tool.poetry.dependencies]
```

### Comparing `ms_salesforce_api-1.2.2/PKG-INFO` & `ms_salesforce_api-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ms-salesforce-api
-Version: 1.2.2
+Version: 1.2.3
 Summary: Python library used to extract data from Salesforce API and migrate it to Bigquery and Postgres.
 Author: Making Science
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

