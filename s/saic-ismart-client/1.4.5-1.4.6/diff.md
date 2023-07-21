# Comparing `tmp/saic_ismart_client-1.4.5.tar.gz` & `tmp/saic_ismart_client-1.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saic_ismart_client-1.4.5.tar", last modified: Wed Jul 19 08:13:48 2023, max compression
+gzip compressed data, was "saic_ismart_client-1.4.6.tar", last modified: Fri Jul 21 15:29:59 2023, max compression
```

## Comparing `saic_ismart_client-1.4.5.tar` & `saic_ismart_client-1.4.6.tar`

### file list

```diff
@@ -1,50 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:13:48.900141 saic_ismart_client-1.4.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-19 08:13:34.000000 saic_ismart_client-1.4.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-19 08:13:34.000000 saic_ismart_client-1.4.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-19 08:13:48.900141 saic_ismart_client-1.4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-19 08:13:34.000000 saic_ismart_client-1.4.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-07-19 08:13:34.000000 saic_ismart_client-1.4.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 08:13:48.900141 saic_ismart_client-1.4.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:13:48.896141 saic_ismart_client-1.4.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:13:48.896141 saic_ismart_client-1.4.5/src/saic_ismart_client/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:13:48.896141 saic_ismart_client-1.4.5/src/saic_ismart_client/ASN.1_schema/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:13:48.896141 saic_ismart_client-1.4.5/src/saic_ismart_client/ASN.1_schema/v1_1/
--rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-07-19 08:13:34.000000 saic_ismart_client-1.4.5/src/saic_ismart_client/ASN.1_schema/v1_1/ApplicationData.asn1
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-07-19 08:13:34.000000 saic_ismart_client-1.4.5/src/saic_ismart_client/ASN.1_schema/v1_1/MP_DispatcherBody.asn1
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-19 08:13:34.000000 saic_ismart_client-1.4.5/src/saic_ismart_client/ASN.1_schema/v1_1/MP_DispatcherHeader.asn1
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:13:48.896141 saic_ismart_client-1.4.5/src/saic_ismart_client/ASN.1_schema/v2_1/
--rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-07-19 08:13:34.000000 saic_ismart_client-1.4.5/src/saic_ismart_client/ASN.1_schema/v2_1/ApplicationData.asn1
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-07-19 08:13:34.000000 saic_ismart_client-1.4.5/src/saic_ismart_client/ASN.1_schema/v2_1/MP_DispatcherBody.asn1
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-19 08:13:34.000000 saic_ismart_client-1.4.5/src/saic_ismart_client/ASN.1_schema/v2_1/MP_DispatcherHeader.asn1
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:13:48.896141 saic_ismart_client-1.4.5/src/saic_ismart_client/ASN.1_schema/v3_0/
--rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-07-19 08:13:34.000000 saic_ismart_client-1.4.5/src/saic_ismart_client/ASN.1_schema/v3_0/ApplicationData.asn1
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-07-19 08:13:34.000000 saic_ismart_client-1.4.5/src/saic_ismart_client/ASN.1_schema/v3_0/MP_DispatcherBody.asn1
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-19 08:13:34.000000 saic_ismart_client-1.4.5/src/saic_ismart_client/ASN.1_schema/v3_0/MP_DispatcherHeader.asn1
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 08:13:34.000000 saic_ismart_client-1.4.5/src/saic_ismart_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-07-19 08:13:34.000000 saic_ismart_client-1.4.5/src/saic_ismart_client/abrp_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    24245 2023-07-19 08:13:34.000000 saic_ismart_client-1.4.5/src/saic_ismart_client/common_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:13:48.896141 saic_ismart_client-1.4.5/src/saic_ismart_client/ota_v1_1/
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-19 08:13:34.000000 saic_ismart_client-1.4.5/src/saic_ismart_client/ota_v1_1/Message.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 08:13:34.000000 saic_ismart_client-1.4.5/src/saic_ismart_client/ota_v1_1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15634 2023-07-19 08:13:34.000000 saic_ismart_client-1.4.5/src/saic_ismart_client/ota_v1_1/data_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:13:48.900141 saic_ismart_client-1.4.5/src/saic_ismart_client/ota_v2_1/
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-19 08:13:34.000000 saic_ismart_client-1.4.5/src/saic_ismart_client/ota_v2_1/Message.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 08:13:34.000000 saic_ismart_client-1.4.5/src/saic_ismart_client/ota_v2_1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18407 2023-07-19 08:13:34.000000 saic_ismart_client-1.4.5/src/saic_ismart_client/ota_v2_1/data_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:13:48.900141 saic_ismart_client-1.4.5/src/saic_ismart_client/ota_v3_0/
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-07-19 08:13:34.000000 saic_ismart_client-1.4.5/src/saic_ismart_client/ota_v3_0/Message.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 08:13:34.000000 saic_ismart_client-1.4.5/src/saic_ismart_client/ota_v3_0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23497 2023-07-19 08:13:34.000000 saic_ismart_client-1.4.5/src/saic_ismart_client/ota_v3_0/data_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    44322 2023-07-19 08:13:34.000000 saic_ismart_client-1.4.5/src/saic_ismart_client/saic_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:13:48.896141 saic_ismart_client-1.4.5/src/saic_ismart_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-19 08:13:48.000000 saic_ismart_client-1.4.5/src/saic_ismart_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-07-19 08:13:48.000000 saic_ismart_client-1.4.5/src/saic_ismart_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 08:13:48.000000 saic_ismart_client-1.4.5/src/saic_ismart_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-19 08:13:48.000000 saic_ismart_client-1.4.5/src/saic_ismart_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-19 08:13:48.000000 saic_ismart_client-1.4.5/src/saic_ismart_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:13:48.900141 saic_ismart_client-1.4.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7936 2023-07-19 08:13:34.000000 saic_ismart_client-1.4.5/tests/test_Message_v1_1.py
--rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-07-19 08:13:34.000000 saic_ismart_client-1.4.5/tests/test_Message_v2_1.py
--rw-r--r--   0 runner    (1001) docker     (123)     8581 2023-07-19 08:13:34.000000 saic_ismart_client-1.4.5/tests/test_Message_v3_0.py
--rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-07-19 08:13:34.000000 saic_ismart_client-1.4.5/tests/test_abrp_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    16753 2023-07-19 08:13:34.000000 saic_ismart_client-1.4.5/tests/test_saic_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:29:59.854666 saic_ismart_client-1.4.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-21 15:29:50.000000 saic_ismart_client-1.4.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-21 15:29:50.000000 saic_ismart_client-1.4.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-21 15:29:59.854666 saic_ismart_client-1.4.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-21 15:29:50.000000 saic_ismart_client-1.4.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-07-21 15:29:50.000000 saic_ismart_client-1.4.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 15:29:59.854666 saic_ismart_client-1.4.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:29:59.846666 saic_ismart_client-1.4.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:29:59.850666 saic_ismart_client-1.4.6/src/saic_ismart_client/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:29:59.846666 saic_ismart_client-1.4.6/src/saic_ismart_client/ASN.1_schema/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:29:59.850666 saic_ismart_client-1.4.6/src/saic_ismart_client/ASN.1_schema/v1_1/
+-rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-07-21 15:29:50.000000 saic_ismart_client-1.4.6/src/saic_ismart_client/ASN.1_schema/v1_1/ApplicationData.asn1
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-07-21 15:29:50.000000 saic_ismart_client-1.4.6/src/saic_ismart_client/ASN.1_schema/v1_1/MP_DispatcherBody.asn1
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-21 15:29:50.000000 saic_ismart_client-1.4.6/src/saic_ismart_client/ASN.1_schema/v1_1/MP_DispatcherHeader.asn1
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:29:59.850666 saic_ismart_client-1.4.6/src/saic_ismart_client/ASN.1_schema/v2_1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-07-21 15:29:50.000000 saic_ismart_client-1.4.6/src/saic_ismart_client/ASN.1_schema/v2_1/ApplicationData.asn1
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-07-21 15:29:50.000000 saic_ismart_client-1.4.6/src/saic_ismart_client/ASN.1_schema/v2_1/MP_DispatcherBody.asn1
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-21 15:29:50.000000 saic_ismart_client-1.4.6/src/saic_ismart_client/ASN.1_schema/v2_1/MP_DispatcherHeader.asn1
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:29:59.850666 saic_ismart_client-1.4.6/src/saic_ismart_client/ASN.1_schema/v3_0/
+-rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-07-21 15:29:50.000000 saic_ismart_client-1.4.6/src/saic_ismart_client/ASN.1_schema/v3_0/ApplicationData.asn1
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-07-21 15:29:50.000000 saic_ismart_client-1.4.6/src/saic_ismart_client/ASN.1_schema/v3_0/MP_DispatcherBody.asn1
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-21 15:29:50.000000 saic_ismart_client-1.4.6/src/saic_ismart_client/ASN.1_schema/v3_0/MP_DispatcherHeader.asn1
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 15:29:50.000000 saic_ismart_client-1.4.6/src/saic_ismart_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-07-21 15:29:50.000000 saic_ismart_client-1.4.6/src/saic_ismart_client/abrp_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24328 2023-07-21 15:29:50.000000 saic_ismart_client-1.4.6/src/saic_ismart_client/common_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-07-21 15:29:50.000000 saic_ismart_client-1.4.6/src/saic_ismart_client/message_decoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:29:59.850666 saic_ismart_client-1.4.6/src/saic_ismart_client/ota_v1_1/
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-21 15:29:50.000000 saic_ismart_client-1.4.6/src/saic_ismart_client/ota_v1_1/Message.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 15:29:50.000000 saic_ismart_client-1.4.6/src/saic_ismart_client/ota_v1_1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15634 2023-07-21 15:29:50.000000 saic_ismart_client-1.4.6/src/saic_ismart_client/ota_v1_1/data_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:29:59.850666 saic_ismart_client-1.4.6/src/saic_ismart_client/ota_v2_1/
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-21 15:29:50.000000 saic_ismart_client-1.4.6/src/saic_ismart_client/ota_v2_1/Message.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 15:29:50.000000 saic_ismart_client-1.4.6/src/saic_ismart_client/ota_v2_1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18407 2023-07-21 15:29:50.000000 saic_ismart_client-1.4.6/src/saic_ismart_client/ota_v2_1/data_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:29:59.850666 saic_ismart_client-1.4.6/src/saic_ismart_client/ota_v3_0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-07-21 15:29:50.000000 saic_ismart_client-1.4.6/src/saic_ismart_client/ota_v3_0/Message.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 15:29:50.000000 saic_ismart_client-1.4.6/src/saic_ismart_client/ota_v3_0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23497 2023-07-21 15:29:50.000000 saic_ismart_client-1.4.6/src/saic_ismart_client/ota_v3_0/data_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44396 2023-07-21 15:29:50.000000 saic_ismart_client-1.4.6/src/saic_ismart_client/saic_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:29:59.850666 saic_ismart_client-1.4.6/src/saic_ismart_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-21 15:29:59.000000 saic_ismart_client-1.4.6/src/saic_ismart_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-07-21 15:29:59.000000 saic_ismart_client-1.4.6/src/saic_ismart_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 15:29:59.000000 saic_ismart_client-1.4.6/src/saic_ismart_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-21 15:29:59.000000 saic_ismart_client-1.4.6/src/saic_ismart_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-21 15:29:59.000000 saic_ismart_client-1.4.6/src/saic_ismart_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:29:59.854666 saic_ismart_client-1.4.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7936 2023-07-21 15:29:50.000000 saic_ismart_client-1.4.6/tests/test_Message_v1_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-07-21 15:29:50.000000 saic_ismart_client-1.4.6/tests/test_Message_v2_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8581 2023-07-21 15:29:50.000000 saic_ismart_client-1.4.6/tests/test_Message_v3_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-07-21 15:29:50.000000 saic_ismart_client-1.4.6/tests/test_abrp_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16753 2023-07-21 15:29:50.000000 saic_ismart_client-1.4.6/tests/test_saic_api.py
```

### Comparing `saic_ismart_client-1.4.5/LICENSE` & `saic_ismart_client-1.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.5/PKG-INFO` & `saic_ismart_client-1.4.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saic_ismart_client
-Version: 1.4.5
+Version: 1.4.6
 Summary: SAIC client library (MG iSMART)
 Author-email: Thomas Salm <saic-python-client@devtom.de>
 Project-URL: Homepage, https://github.com/SAIC-iSmart-API/saic-python-client
 Project-URL: Bug Tracker, https://github.com/SAIC-iSmart-API/saic-python-client/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `saic_ismart_client-1.4.5/README.md` & `saic_ismart_client-1.4.6/README.md`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.5/pyproject.toml` & `saic_ismart_client-1.4.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "saic_ismart_client"
-version = "1.4.5"
+version = "1.4.6"
 authors = [
     { name = "Thomas Salm", email="saic-python-client@devtom.de"},
 ]
 dependencies = [
     "asn1tools >= 0.166.0",
     "requests >= 2.31.0",
     "urllib3 >= 2.0.3",
```

### Comparing `saic_ismart_client-1.4.5/src/saic_ismart_client/ASN.1_schema/v1_1/ApplicationData.asn1` & `saic_ismart_client-1.4.6/src/saic_ismart_client/ASN.1_schema/v1_1/ApplicationData.asn1`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.5/src/saic_ismart_client/ASN.1_schema/v1_1/MP_DispatcherBody.asn1` & `saic_ismart_client-1.4.6/src/saic_ismart_client/ASN.1_schema/v1_1/MP_DispatcherBody.asn1`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.5/src/saic_ismart_client/ASN.1_schema/v2_1/ApplicationData.asn1` & `saic_ismart_client-1.4.6/src/saic_ismart_client/ASN.1_schema/v2_1/ApplicationData.asn1`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.5/src/saic_ismart_client/ASN.1_schema/v2_1/MP_DispatcherBody.asn1` & `saic_ismart_client-1.4.6/src/saic_ismart_client/ASN.1_schema/v2_1/MP_DispatcherBody.asn1`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.5/src/saic_ismart_client/ASN.1_schema/v3_0/ApplicationData.asn1` & `saic_ismart_client-1.4.6/src/saic_ismart_client/ASN.1_schema/v3_0/ApplicationData.asn1`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.5/src/saic_ismart_client/ASN.1_schema/v3_0/MP_DispatcherBody.asn1` & `saic_ismart_client-1.4.6/src/saic_ismart_client/ASN.1_schema/v3_0/MP_DispatcherBody.asn1`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.5/src/saic_ismart_client/abrp_api.py` & `saic_ismart_client-1.4.6/src/saic_ismart_client/abrp_api.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.5/src/saic_ismart_client/common_model.py` & `saic_ismart_client-1.4.6/src/saic_ismart_client/common_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -478,16 +478,18 @@
 
         decoded_message.reserved = buffered_message_bytes.read(self.reserved_size)
 
         dispatcher_message_bytes = buffered_message_bytes.read(header.dispatcher_message_length - self.header_length)
         message_body_dict = self.asn1_tool_uper.decode('MPDispatcherBody', dispatcher_message_bytes)
         message_body = decoded_message.body
         message_body.init_from_dict(message_body_dict)
-
-        if message_body.application_data_length > 0:
+        if(
+            message_body.application_data_length > 0
+            and decoded_message.application_data is not None
+        ):
             application_data_bytes = buffered_message_bytes.read(message_body.application_data_length)
             application_data_dict = self.asn1_tool_uper.decode(decoded_message.application_data.asn_type,
                                                                application_data_bytes)
             decoded_message.application_data.init_from_dict(application_data_dict)
         else:
             decoded_message.application_data = None
```

### Comparing `saic_ismart_client-1.4.5/src/saic_ismart_client/ota_v1_1/Message.py` & `saic_ismart_client-1.4.6/src/saic_ismart_client/ota_v1_1/Message.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.5/src/saic_ismart_client/ota_v1_1/data_model.py` & `saic_ismart_client-1.4.6/src/saic_ismart_client/ota_v1_1/data_model.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.5/src/saic_ismart_client/ota_v2_1/Message.py` & `saic_ismart_client-1.4.6/src/saic_ismart_client/ota_v2_1/Message.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.5/src/saic_ismart_client/ota_v2_1/data_model.py` & `saic_ismart_client-1.4.6/src/saic_ismart_client/ota_v2_1/data_model.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.5/src/saic_ismart_client/ota_v3_0/Message.py` & `saic_ismart_client-1.4.6/src/saic_ismart_client/ota_v3_0/Message.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.5/src/saic_ismart_client/ota_v3_0/data_model.py` & `saic_ismart_client-1.4.6/src/saic_ismart_client/ota_v3_0/data_model.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.5/src/saic_ismart_client/saic_api.py` & `saic_ismart_client-1.4.6/src/saic_ismart_client/saic_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import datetime
 import hashlib
 import logging
+import os
 import time
 import urllib.parse
-from enum import Enum
 from typing import cast
 
 import requests as requests
 
 from saic_ismart_client.common_model import AbstractMessage, AbstractMessageBody, Header, MessageBodyV2, MessageV2, \
     ScheduledChargingMode, TargetBatteryCode
 from saic_ismart_client.ota_v1_1.Message import MessageCoderV11
@@ -19,15 +19,17 @@
     OtaRvmVehicleStatusResp25857, RvcReqParam
 from saic_ismart_client.ota_v3_0.Message import MessageBodyV30, MessageCoderV30, MessageV30
 from saic_ismart_client.ota_v3_0.data_model import OtaChrgCtrlReq, OtaChrgCtrlStsResp, OtaChrgHeatReq, \
     OtaChrgHeatResp, OtaChrgMangDataResp, OtaChrgRsvanReq, OtaChrgSetngReq, OtaChrgSetngResp, OtaChrgRsvanResp
 
 UID_INIT = '0000000000000000000000000000000000000000000000000#'
 AVG_SMS_DELIVERY_TIME = 15
-logging.basicConfig(format='%(asctime)s %(message)s', level=logging.INFO)
+logging.basicConfig(format='%(asctime)s %(message)s')
+LOG = logging.getLogger(__name__)
+LOG.setLevel(level=os.getenv('LOG_LEVEL', 'INFO').upper())
 
 
 class SaicMessage:
     def __init__(self, message_id: int, message_type: str, title: str, message_time: datetime, sender: str,
                  content: str, read_status: int, vin: str):
         self.message_id = message_id
         self.message_type = message_type
@@ -473,15 +475,15 @@
         vehicle_control_cmd_rsp_msg = self.send_vehicle_control_command(vin_info, rvc_req_type, rvc_params)
 
         if has_app_data:
             while vehicle_control_cmd_rsp_msg.application_data is None:
                 if vehicle_control_cmd_rsp_msg.body.error_message is not None:
                     self.handle_error(vehicle_control_cmd_rsp_msg.body)
                 else:
-                    logging.debug('API request returned no application data and no error message.')
+                    LOG.debug('API request returned no application data and no error message.')
                     time.sleep(float(AVG_SMS_DELIVERY_TIME))
 
                 event_id = vehicle_control_cmd_rsp_msg.body.event_id
                 vehicle_control_cmd_rsp_msg = self.send_vehicle_control_command(vin_info, rvc_req_type, rvc_params,
                                                                                 event_id)
         else:
             retry = 1
@@ -515,15 +517,15 @@
         else:
             rsp = func()
         rsp_msg = cast(AbstractMessage, rsp)
         while rsp_msg.application_data is None:
             if rsp_msg.body.error_message is not None:
                 self.handle_error(rsp_msg.body)
             else:
-                logging.debug('API request returned no application data and no error message.')
+                LOG.debug('API request returned no application data and no error message.')
                 time.sleep(float(AVG_SMS_DELIVERY_TIME))
 
             if vin_info:
                 rsp_msg = func(vin_info, rsp_msg.body.event_id)
             else:
                 rsp_msg = func(rsp_msg.body.event_id)
         return rsp_msg
@@ -561,14 +563,15 @@
 
     def get_charging_status(self, vin_info: VinInfo, event_id: str = None) -> MessageV30:
         chrg_mgmt_data_req_msg = MessageV30(MessageBodyV30())
         application_id = '516'
         application_data_protocol_version = 768
         self.message_V3_0_coder.initialize_message(self.uid, self.get_token(), vin_info.vin, application_id,
                                                    application_data_protocol_version, 5, chrg_mgmt_data_req_msg)
+        chrg_mgmt_data_req_msg.body.ack_required = False
         if event_id is not None:
             chrg_mgmt_data_req_msg.body.event_id = event_id
         self.publish_json_request(application_id, application_data_protocol_version, chrg_mgmt_data_req_msg.get_data())
         chrg_mgmt_data_req_hex = self.message_V3_0_coder.encode_request(chrg_mgmt_data_req_msg)
         self.publish_raw_request(application_id, application_data_protocol_version, chrg_mgmt_data_req_hex)
         chrg_mgmt_data_rsp_hex = self.send_request(chrg_mgmt_data_req_hex,
                                                    urllib.parse.urljoin(self.saic_uri, '/TAP.Web/ota.mpv30'))
@@ -796,15 +799,15 @@
             raise SaicApiException(message_delete_rsp_msg.body.error_message.decode(),
                                    message_delete_rsp_msg.body.result)
 
     def publish_raw_value(self, key: str, raw: str):
         if self.on_publish_raw_value is not None:
             self.on_publish_raw_value(key, raw)
         else:
-            logging.debug(f'{key}: {raw}')
+            LOG.debug(f'{key}: {raw}')
 
     def publish_raw_request(self, application_id: str, application_data_protocol_version: int, raw: str):
         key = f'{application_id}_{application_data_protocol_version}/raw/request'
         self.publish_raw_value(key, raw)
 
     def publish_raw_response(self, application_id: str, application_data_protocol_version: int, raw: str):
         key = f'{application_id}_{application_data_protocol_version}/raw/response'
@@ -818,15 +821,15 @@
         key = f'{application_id}_{application_data_protocol_version}/json/response'
         self.publish_json(key, data)
 
     def publish_json(self, key: str, data: dict):
         if self.on_publish_json_value is not None:
             self.on_publish_json_value(key, data)
         else:
-            logging.debug(f'{key}: {data}')
+            LOG.debug(f'{key}: {data}')
 
     def send_request(self, hex_message: str, endpoint) -> str:
         headers = {
             'Accept': '*/*',
             'Content-Type': 'text/html',
             'Accept-Encoding': 'gzip, deflate, br',
             'User-Agent': 'MG iSMART/1.1.1 (iPhone; iOS 16.3; Scale/3.00)',
@@ -858,32 +861,32 @@
         message = f'application ID: {message_body.application_id},' \
                   + f' protocol version: {message_body.application_data_protocol_version},' \
                   + f' message: {message_body.error_message.decode()}' \
                   + f' result code: {message_body.result}'
 
         if message_body.result == 2:
             # re-login
-            logging.debug(message)
+            LOG.debug(message)
             if self.relogin_delay > 0:
-                logging.warning(f'The SAIC user has been logged out. '
-                                + f'Waiting {self.relogin_delay} seconds before attempting another login')
+                LOG.warning(f'The SAIC user has been logged out. '
+                            + f'Waiting {self.relogin_delay} seconds before attempting another login')
                 time.sleep(float(self.relogin_delay))
             self.login()
         elif message_body.result == 4:
             # The remote control instruction failed, please try again later.
-            logging.debug(message)
+            LOG.debug(message)
             time.sleep(float(AVG_SMS_DELIVERY_TIME))
         elif message_body.result == 6:
             # The service is not available,please try again later
-            logging.debug(message)
+            LOG.debug(message)
             time.sleep(float(AVG_SMS_DELIVERY_TIME))
         elif message_body.result == -1:
-            logging.warning(message)
+            LOG.warning(message)
         else:
-            logging.error(message)
+            LOG.error(message)
 
 
 def bool_to_bit(flag):
     return b'\x01' if flag else b'\x00'
 
 
 def bool_to_int(flag):
```

### Comparing `saic_ismart_client-1.4.5/src/saic_ismart_client.egg-info/PKG-INFO` & `saic_ismart_client-1.4.6/src/saic_ismart_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saic-ismart-client
-Version: 1.4.5
+Version: 1.4.6
 Summary: SAIC client library (MG iSMART)
 Author-email: Thomas Salm <saic-python-client@devtom.de>
 Project-URL: Homepage, https://github.com/SAIC-iSmart-API/saic-python-client
 Project-URL: Bug Tracker, https://github.com/SAIC-iSmart-API/saic-python-client/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `saic_ismart_client-1.4.5/src/saic_ismart_client.egg-info/SOURCES.txt` & `saic_ismart_client-1.4.6/src/saic_ismart_client.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 src/saic_ismart_client/__init__.py
 src/saic_ismart_client/abrp_api.py
 src/saic_ismart_client/common_model.py
+src/saic_ismart_client/message_decoder.py
 src/saic_ismart_client/saic_api.py
 src/saic_ismart_client.egg-info/PKG-INFO
 src/saic_ismart_client.egg-info/SOURCES.txt
 src/saic_ismart_client.egg-info/dependency_links.txt
 src/saic_ismart_client.egg-info/requires.txt
 src/saic_ismart_client.egg-info/top_level.txt
 src/saic_ismart_client/ASN.1_schema/v1_1/ApplicationData.asn1
```

### Comparing `saic_ismart_client-1.4.5/tests/test_Message_v1_1.py` & `saic_ismart_client-1.4.6/tests/test_Message_v1_1.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.5/tests/test_Message_v2_1.py` & `saic_ismart_client-1.4.6/tests/test_Message_v2_1.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.5/tests/test_Message_v3_0.py` & `saic_ismart_client-1.4.6/tests/test_Message_v3_0.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.5/tests/test_abrp_api.py` & `saic_ismart_client-1.4.6/tests/test_abrp_api.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.5/tests/test_saic_api.py` & `saic_ismart_client-1.4.6/tests/test_saic_api.py`

 * *Files identical despite different names*

