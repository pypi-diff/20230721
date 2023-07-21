# Comparing `tmp/salure_helpers_profit-2.0.0.tar.gz` & `tmp/salure_helpers_profit-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/salure_helpers_profit-2.0.0.tar", last modified: Thu Jul 20 16:32:22 2023, max compression
+gzip compressed data, was "dist/salure_helpers_profit-2.1.0.tar", last modified: Fri Jul 21 15:32:35 2023, max compression
```

## Comparing `salure_helpers_profit-2.0.0.tar` & `salure_helpers_profit-2.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:32:22.000000 salure_helpers_profit-2.0.0/
--rw-r--r--   0 root         (0) root         (0)      262 2023-07-20 16:32:22.000000 salure_helpers_profit-2.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:32:22.000000 salure_helpers_profit-2.0.0/salure_helpers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:32:22.000000 salure_helpers_profit-2.0.0/salure_helpers/profit/
--rw-rw-rw-   0 root         (0) root         (0)      263 2023-07-20 16:32:09.000000 salure_helpers_profit-2.0.0/salure_helpers/profit/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3855 2023-07-20 16:32:09.000000 salure_helpers_profit-2.0.0/salure_helpers/profit/profit_data_cleaner.py
--rw-rw-rw-   0 root         (0) root         (0)    14489 2023-07-20 16:32:09.000000 salure_helpers_profit-2.0.0/salure_helpers/profit/profit_get.py
--rw-rw-rw-   0 root         (0) root         (0)    17456 2023-07-20 16:32:09.000000 salure_helpers_profit-2.0.0/salure_helpers/profit/profit_get_async.py
--rw-rw-rw-   0 root         (0) root         (0)   139049 2023-07-20 16:32:09.000000 salure_helpers_profit-2.0.0/salure_helpers/profit/profit_update.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:32:22.000000 salure_helpers_profit-2.0.0/salure_helpers_profit.egg-info/
--rw-r--r--   0 root         (0) root         (0)      262 2023-07-20 16:32:22.000000 salure_helpers_profit-2.0.0/salure_helpers_profit.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      472 2023-07-20 16:32:22.000000 salure_helpers_profit-2.0.0/salure_helpers_profit.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 16:32:22.000000 salure_helpers_profit-2.0.0/salure_helpers_profit.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 16:32:22.000000 salure_helpers_profit-2.0.0/salure_helpers_profit.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      130 2023-07-20 16:32:22.000000 salure_helpers_profit-2.0.0/salure_helpers_profit.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-07-20 16:32:22.000000 salure_helpers_profit-2.0.0/salure_helpers_profit.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-20 16:32:22.000000 salure_helpers_profit-2.0.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      580 2023-07-20 16:32:09.000000 salure_helpers_profit-2.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:32:35.000000 salure_helpers_profit-2.1.0/
+-rw-r--r--   0 root         (0) root         (0)      262 2023-07-21 15:32:35.000000 salure_helpers_profit-2.1.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:32:35.000000 salure_helpers_profit-2.1.0/salure_helpers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:32:35.000000 salure_helpers_profit-2.1.0/salure_helpers/profit/
+-rw-rw-rw-   0 root         (0) root         (0)      263 2023-07-21 15:32:22.000000 salure_helpers_profit-2.1.0/salure_helpers/profit/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3855 2023-07-21 15:32:22.000000 salure_helpers_profit-2.1.0/salure_helpers/profit/profit_data_cleaner.py
+-rw-rw-rw-   0 root         (0) root         (0)    14489 2023-07-21 15:32:22.000000 salure_helpers_profit-2.1.0/salure_helpers/profit/profit_get.py
+-rw-rw-rw-   0 root         (0) root         (0)    17456 2023-07-21 15:32:22.000000 salure_helpers_profit-2.1.0/salure_helpers/profit/profit_get_async.py
+-rw-rw-rw-   0 root         (0) root         (0)   142534 2023-07-21 15:32:22.000000 salure_helpers_profit-2.1.0/salure_helpers/profit/profit_update.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:32:35.000000 salure_helpers_profit-2.1.0/salure_helpers_profit.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      262 2023-07-21 15:32:35.000000 salure_helpers_profit-2.1.0/salure_helpers_profit.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      472 2023-07-21 15:32:35.000000 salure_helpers_profit-2.1.0/salure_helpers_profit.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 15:32:35.000000 salure_helpers_profit-2.1.0/salure_helpers_profit.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 15:32:35.000000 salure_helpers_profit-2.1.0/salure_helpers_profit.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      130 2023-07-21 15:32:35.000000 salure_helpers_profit-2.1.0/salure_helpers_profit.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-07-21 15:32:35.000000 salure_helpers_profit-2.1.0/salure_helpers_profit.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-21 15:32:35.000000 salure_helpers_profit-2.1.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      580 2023-07-21 15:32:22.000000 salure_helpers_profit-2.1.0/setup.py
```

### Comparing `salure_helpers_profit-2.0.0/salure_helpers/profit/profit_data_cleaner.py` & `salure_helpers_profit-2.1.0/salure_helpers/profit/profit_data_cleaner.py`

 * *Files identical despite different names*

### Comparing `salure_helpers_profit-2.0.0/salure_helpers/profit/profit_get.py` & `salure_helpers_profit-2.1.0/salure_helpers/profit/profit_get.py`

 * *Files identical despite different names*

### Comparing `salure_helpers_profit-2.0.0/salure_helpers/profit/profit_get_async.py` & `salure_helpers_profit-2.1.0/salure_helpers/profit/profit_get_async.py`

 * *Files identical despite different names*

### Comparing `salure_helpers_profit-2.0.0/salure_helpers/profit/profit_update.py` & `salure_helpers_profit-2.1.0/salure_helpers/profit/profit_update.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,14 +96,80 @@
         # Update the request body with update fields
         base_body['AfasEmployee']['Element']['Objects']['KnPerson']['Element']['Fields'].update(fields_to_update)
 
         update = requests.request(method, url, data=json.dumps(base_body), headers=self.headers)
 
         return update
 
+    def update_user(self, data: dict, method='POST') -> requests.Response:
+        """
+        :param data: Fields that are allowed are listed in allowed fields array. Update this whenever necessary
+        :param method: request type (must be post or put)
+        :return: status code for request and optional error message
+        """
+        allowed_fields = ['profit_user_code', 'person_id', 'userPrincipalName', 'mail']
+        required_fields = ['profit_user_code', 'person_id']
+
+        self.__check_fields(data=data, required_fields=required_fields, allowed_fields=allowed_fields)
+
+        url = f'https://{self.environment}.{self.base_url}/profitrestservices/connectors/KnUser'
+
+        base_body = {
+            "KnUser": {
+                "Element": {
+                    "@UsId": data['profit_user_code'],
+                    "Fields": {
+                        "MtCd": 1,
+                        "BcCo": data['person_id'],
+                        "Nm": "SALURE",
+                    }
+                }
+            }
+        }
+        fields_to_update = {}
+
+        # Add fields that you want to update a dict (adding to body itself is too much text)
+        fields_to_update.update({"Upn": data['userPrincipalName']}) if 'userPrincipalName' in data else fields_to_update
+        fields_to_update.update({"EmAd": data['mail']}) if 'mail' in data else fields_to_update
+
+        # Update the request body with update fields
+        base_body['KnUser']['Element']['Fields'].update(fields_to_update)
+
+        update = requests.request(method, url, data=json.dumps(base_body), headers=self.headers)
+
+        return update
+
+    def upload_photo(self, filepath: str, person_id: str, filename: str = None) -> requests.Response:
+        """
+        This code opens a file located at filename in binary mode, reads its contents, encodes the contents in base64, and assigns the result to filestream.
+        Then, it creates a JSON object representing an image upload request to an API endpoint.
+        This JSON object is converted to a string using json.dumps and assigned to body_image_upload.
+        :param filepath: The filepath (complete path including filename) of the image to be uploaded
+        :param filename: The filename of the image to be uploaded
+        :param person_id: The personal id number of the user in AFAS
+        """
+        open_file = open(filepath, 'rb').read()
+        filestream = base64.b64encode(open_file).decode('utf-8')
+        body_image_upload = {"KnPerson": {
+            "Element": {
+                "Fields": {
+                    "MatchPer": "0",
+                    "BcCo": person_id,
+                    "FileName": "filename" if filename is None else filename,
+                    "FileStream": filestream,
+
+                }
+            }
+        }
+        }
+        body_image_upload = json.dumps(body_image_upload)
+        url = f'https://{self.environment}.{self.base_url}/profitrestservices/connectors/KnPerson'
+        update = requests.put(url=url, data=body_image_upload, headers=self.headers)
+        return update
+
     def update_organisation(self, data: dict, method: str, custom_fields: dict = None) -> requests.Response:
         """
         This function updates organisations in CRM with the AFAS updateconnect 'KnOrganisation'.
         :param data: Deliver all the data which should be updated in list format. The data should at least contain the required_fields and can contain also the allowed fields
         :param method: Is a PUT for an update of an existing cost carrier. is a POST for an insert of a new cost carrier
         :param custom_fields: The custom fields in this dataset. Give the key of the field and the value. For example: {DFEDS8-DSF9uD-DDSA: 'Vrij veld'}
         :return: The status code from AFAS Profit
@@ -672,15 +738,15 @@
         :return: status code for request and optional error message
         """
 
         # Contract fields
         required_fields_contract = ['employee_id', 'startdate_contract']
         allowed_fields_contract = ['employee_id', 'type_of_employment', 'enddate_contract', 'termination_reason', 'termination_initiative', 'probation_period',
                                    'probation_enddate', 'cao', 'terms_of_employment', 'type_of_contract', 'employer_number', 'type_of_employee', 'employment'
-                                   'seniority_date', 'contract_chain_code', 'start_date_contract_chain']
+                                                                                                                                                 'seniority_date', 'contract_chain_code', 'start_date_contract_chain']
 
         # Function fields
         required_fields_function = ['organizational_unit', 'function_id', 'costcenter_id']
         allowed_fields_function = ['costcarrier_id']
 
         # Timetable fields
         required_fields_timetable = ['weekly_hours', 'parttime_percentage']
@@ -2246,37 +2312,39 @@
         for unique_period in year_period_per_administration_list:
             df_period = df[df['unique_period_year_per_administration'] == unique_period]
             # drop the columns that are not needed for the upload iteration
             df_period = df_period.sort_values(by=['booking_number', 'date_booking'])
             # pass the index payload and the dataframe to the upload method
             update = self.__create_journalentry_for_period(df=df_period)
             json_update = update.json()
+            # get values from first row of df (all rows are the same for the same period)
+            df_period_values = df.to_dict(orient='records')[0]
             if 200 <= update.status_code < 300:
-                upload_summary.append(f"Journal entries for year {df_period['year']}, period {df_period['period']}, adminstration {df_period['administration_id']} and journal {df_period['journal_id']} uploaded successfully. Status code: {update.status_code}")
+                upload_summary.append(f"Journal entries for year {df_period_values['year']}, period {df_period_values['period']}, adminstration {df_period_values['administration_id']} and journal {df_period_values['journal_id']} uploaded successfully. Status code: {update.status_code}")
                 status_codes.append(update.status_code)
             else:
-                upload_summary.append(f"Journal entries for year {df_period['year']}, period {df_period['period']}, adminstration {df_period['administration_id']} and journal {df_period['journal_id']} failed. Status code: {update.status_code} {json_update['externalMessage']}")
+                upload_summary.append(f"Journal entries for year {df_period_values['year']}, period {df_period_values['period']}, adminstration {df_period_values['administration_id']} and journal {df_period_values['journal_id']} failed. Status code: {update.status_code} {json_update['externalMessage']}")
                 status_codes.append(update.status_code)
 
         return upload_summary, status_codes
 
     def __create_journalentry_for_period(self, df: pd.DataFrame) -> requests.Response:
         """
         This function is an internal function used in conjunction with upload_journalentries. This function updates Afas profit for updateconnector: 'Fientries'.
         :param df: The dataframe with the journal entries for the year period and administration id specified in the data. This dataframe needs debit and credit values that equal out per booking number.
         :return: The response from AFAS Profit
         """
         base_body = {
             "FiEntryPar": {
                 "Element": {
                     "Fields": {
-                        "Year": df[0]['year'],
-                        "Peri": df[0]["period"],
-                        "UnId": df[0]['administration_id'],
-                        "JoCo": df[0]['journal']
+                        "Year": df.iloc[0]['year'],
+                        "Peri": df.iloc[0]["period"],
+                        "UnId": df.iloc[0]['administration_id'],
+                        "JoCo": df.iloc[0]['journal_id']
                     },
                     "Objects": [
                         {
                             "FiEntries": {
                                 "Element": []
                             }
                         }
@@ -2297,15 +2365,16 @@
                     "AmCr": row['credit']
                 },
                 "Objects": [
                     {
                         "FiDimEntries": {
                             "Element": {
                                 "Fields": {
-                                    "DiC1": row['cost_centre_id']
+                                    "DiC1": row['cost_centre_id'],
+                                    "DiC2": row['cost_carrier_id']
                                 }
                             }
                         }
                     }
                 ]
             }
             base_body['FiEntryPar']["Element"]["Objects"][0]["FiEntries"]["Element"].append(single_entry)
```

### Comparing `salure_helpers_profit-2.0.0/setup.py` & `salure_helpers_profit-2.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 
 setup(
     name='salure_helpers_profit',
-    version='2.0.0',
+    version='2.1.0',
     description='Profit wrapper from Salure',
     long_description='Profit wrapper from Salure',
     author='D&A Salure',
     author_email='support@salureconnnect.com',
     packages=["salure_helpers.profit"],
     license='Salure License',
     install_requires=[
```

