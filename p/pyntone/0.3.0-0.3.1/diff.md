# Comparing `tmp/pyntone-0.3.0.tar.gz` & `tmp/pyntone-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyntone-0.3.0.tar", last modified: Fri Jul 21 01:38:09 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `pyntone-0.3.0.tar` & `pyntone-0.3.1.tar`

### file list

```diff
@@ -1,40 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:38:09.447304 pyntone-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-21 01:37:58.000000 pyntone-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-21 01:38:09.447304 pyntone-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-21 01:37:58.000000 pyntone-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:38:09.447304 pyntone-0.3.0/pyntone/
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-21 01:37:58.000000 pyntone-0.3.0/pyntone/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:38:09.447304 pyntone-0.3.0/pyntone/client/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-21 01:37:58.000000 pyntone-0.3.0/pyntone/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12708 2023-07-21 01:37:58.000000 pyntone-0.3.0/pyntone/client/app_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-07-21 01:37:58.000000 pyntone-0.3.0/pyntone/client/bulk_request_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-07-21 01:37:58.000000 pyntone-0.3.0/pyntone/client/file_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    18029 2023-07-21 01:37:58.000000 pyntone-0.3.0/pyntone/client/record_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:38:09.447304 pyntone-0.3.0/pyntone/client/types/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-21 01:37:58.000000 pyntone-0.3.0/pyntone/client/types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:38:09.447304 pyntone-0.3.0/pyntone/client/types/app/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-21 01:37:58.000000 pyntone-0.3.0/pyntone/client/types/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-21 01:37:58.000000 pyntone-0.3.0/pyntone/client/types/app/customize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:38:09.447304 pyntone-0.3.0/pyntone/http/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 01:37:58.000000 pyntone-0.3.0/pyntone/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-07-21 01:37:58.000000 pyntone-0.3.0/pyntone/http/http_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4324 2023-07-21 01:37:58.000000 pyntone-0.3.0/pyntone/kintone_request_config_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-07-21 01:37:58.000000 pyntone-0.3.0/pyntone/kintone_rest_api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:38:09.447304 pyntone-0.3.0/pyntone/types/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-21 01:37:58.000000 pyntone-0.3.0/pyntone/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-21 01:37:58.000000 pyntone-0.3.0/pyntone/types/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-21 01:37:58.000000 pyntone-0.3.0/pyntone/types/record.py
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-21 01:37:58.000000 pyntone-0.3.0/pyntone/url.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:38:09.447304 pyntone-0.3.0/pyntone.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-21 01:38:09.000000 pyntone-0.3.0/pyntone.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-21 01:38:09.000000 pyntone-0.3.0/pyntone.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 01:38:09.000000 pyntone-0.3.0/pyntone.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-21 01:38:09.000000 pyntone-0.3.0/pyntone.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-21 01:38:09.000000 pyntone-0.3.0/pyntone.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-21 01:37:58.000000 pyntone-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-07-21 01:38:09.447304 pyntone-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:38:09.447304 pyntone-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 01:37:58.000000 pyntone-0.3.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-07-21 01:37:58.000000 pyntone-0.3.0/tests/test_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-07-21 01:37:58.000000 pyntone-0.3.0/tests/test_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     5869 2023-07-21 01:37:58.000000 pyntone-0.3.0/tests/test_record.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 pyntone-0.3.1/requirements.txt
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 pyntone-0.3.1/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 pyntone-0.3.1/.github/workflows/run_tests.yaml
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 pyntone-0.3.1/pyntone/__init__.py
+-rw-r--r--   0        0        0     4324 2020-02-02 00:00:00.000000 pyntone-0.3.1/pyntone/kintone_request_config_builder.py
+-rw-r--r--   0        0        0     1300 2020-02-02 00:00:00.000000 pyntone-0.3.1/pyntone/kintone_rest_api_client.py
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 pyntone-0.3.1/pyntone/url.py
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 pyntone-0.3.1/pyntone/client/__init__.py
+-rw-r--r--   0        0        0    12708 2020-02-02 00:00:00.000000 pyntone-0.3.1/pyntone/client/app_client.py
+-rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 pyntone-0.3.1/pyntone/client/bulk_request_client.py
+-rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 pyntone-0.3.1/pyntone/client/file_client.py
+-rw-r--r--   0        0        0    18029 2020-02-02 00:00:00.000000 pyntone-0.3.1/pyntone/client/record_client.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 pyntone-0.3.1/pyntone/client/types/__init__.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 pyntone-0.3.1/pyntone/client/types/app/__init__.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 pyntone-0.3.1/pyntone/client/types/app/customize.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyntone-0.3.1/pyntone/http/__init__.py
+-rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 pyntone-0.3.1/pyntone/http/http_client.py
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 pyntone-0.3.1/pyntone/types/__init__.py
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 pyntone-0.3.1/pyntone/types/auth.py
+-rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 pyntone-0.3.1/pyntone/types/record.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyntone-0.3.1/tests/__init__.py
+-rw-r--r--   0        0        0     2662 2020-02-02 00:00:00.000000 pyntone-0.3.1/tests/test_app.py
+-rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 pyntone-0.3.1/tests/test_file.py
+-rw-r--r--   0        0        0     5869 2020-02-02 00:00:00.000000 pyntone-0.3.1/tests/test_record.py
+-rw-r--r--   0        0        0     2992 2020-02-02 00:00:00.000000 pyntone-0.3.1/.gitignore
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 pyntone-0.3.1/LICENSE
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 pyntone-0.3.1/README.md
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 pyntone-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 pyntone-0.3.1/PKG-INFO
```

### Comparing `pyntone-0.3.0/LICENSE` & `pyntone-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyntone-0.3.0/PKG-INFO` & `pyntone-0.3.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 Metadata-Version: 2.1
 Name: pyntone
-Version: 0.3.0
+Version: 0.3.1
 Summary: API client for Kintone REST API.
-Home-page: https://github.com/kashi03/pyntone
+Project-URL: Homepage, https://github.com/kashi03/pyntone
+Project-URL: Repository, https://github.com/kashi03/pyntone
 Author: kashi03
-License: MIT
+License-Expression: MIT
+License-File: LICENSE
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.9
+Requires-Dist: requests>=2.27.1
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 # pyntone
 ![](https://img.shields.io/badge/Python-%3E%3D3.9-blue)  
 API client for Kintone REST API.
 
 ## Installation
 ```bash
@@ -30,8 +33,8 @@
 auth = ApiTokenAuth(api_token='[YOUR API TOKEN]')
 client = KintoneRestAPIClient(
     base_url='https://[YOUR SUBDOMAIN].cybozu.com',
     auth=auth
 )
 res = client.record.get_record(1, 1)
 print(res)
-```
+```
```

### Comparing `pyntone-0.3.0/pyntone/client/app_client.py` & `pyntone-0.3.1/pyntone/client/app_client.py`

 * *Files identical despite different names*

### Comparing `pyntone-0.3.0/pyntone/client/bulk_request_client.py` & `pyntone-0.3.1/pyntone/client/bulk_request_client.py`

 * *Files identical despite different names*

### Comparing `pyntone-0.3.0/pyntone/client/file_client.py` & `pyntone-0.3.1/pyntone/client/file_client.py`

 * *Files identical despite different names*

### Comparing `pyntone-0.3.0/pyntone/client/record_client.py` & `pyntone-0.3.1/pyntone/client/record_client.py`

 * *Files identical despite different names*

### Comparing `pyntone-0.3.0/pyntone/http/http_client.py` & `pyntone-0.3.1/pyntone/http/http_client.py`

 * *Files identical despite different names*

### Comparing `pyntone-0.3.0/pyntone/kintone_request_config_builder.py` & `pyntone-0.3.1/pyntone/kintone_request_config_builder.py`

 * *Files identical despite different names*

### Comparing `pyntone-0.3.0/pyntone/kintone_rest_api_client.py` & `pyntone-0.3.1/pyntone/kintone_rest_api_client.py`

 * *Files identical despite different names*

### Comparing `pyntone-0.3.0/pyntone/types/record.py` & `pyntone-0.3.1/pyntone/types/record.py`

 * *Files identical despite different names*

### Comparing `pyntone-0.3.0/tests/test_app.py` & `pyntone-0.3.1/tests/test_app.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,16 +32,15 @@
 
 
 def test_update_form_fields(client):
     pass
 
 
 def test_delete_form_fields(client):
-    result = client.app.delete_form_fields(env['APP_ID'], ['column1', 'column2'])
-    assert result.get('revision') is not None
+    pass
 
 
 def test_get_form_layout(client):
     result = client.app.get_form_layout(env['APP_ID'])
     assert result.get('revision') is not None
     assert result.get('layout') is not None
```

### Comparing `pyntone-0.3.0/tests/test_file.py` & `pyntone-0.3.1/tests/test_file.py`

 * *Files identical despite different names*

### Comparing `pyntone-0.3.0/tests/test_record.py` & `pyntone-0.3.1/tests/test_record.py`

 * *Files identical despite different names*

