# Comparing `tmp/botocore-a-la-carte-sagemaker-featurestore-runtime-1.31.6.tar.gz` & `tmp/botocore-a-la-carte-sagemaker-featurestore-runtime-1.31.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-sagemaker-featurestore-runtime-1.31.6.tar", last modified: Thu Jul 20 01:20:45 2023, max compression
+gzip compressed data, was "botocore-a-la-carte-sagemaker-featurestore-runtime-1.31.8.tar", last modified: Fri Jul 21 01:21:55 2023, max compression
```

## Comparing `botocore-a-la-carte-sagemaker-featurestore-runtime-1.31.6.tar` & `botocore-a-la-carte-sagemaker-featurestore-runtime-1.31.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:20:45.014915 botocore-a-la-carte-sagemaker-featurestore-runtime-1.31.6/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-20 01:20:44.000000 botocore-a-la-carte-sagemaker-featurestore-runtime-1.31.6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-20 01:20:45.014915 botocore-a-la-carte-sagemaker-featurestore-runtime-1.31.6/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:20:45.014915 botocore-a-la-carte-sagemaker-featurestore-runtime-1.31.6/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:20:45.014915 botocore-a-la-carte-sagemaker-featurestore-runtime-1.31.6/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:20:45.014915 botocore-a-la-carte-sagemaker-featurestore-runtime-1.31.6/botocore/data/sagemaker-featurestore-runtime/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:20:45.014915 botocore-a-la-carte-sagemaker-featurestore-runtime-1.31.6/botocore/data/sagemaker-featurestore-runtime/2020-07-01/
--rw-r--r--   0 runner    (1001) docker     (123)    17720 2023-07-20 01:19:55.000000 botocore-a-la-carte-sagemaker-featurestore-runtime-1.31.6/botocore/data/sagemaker-featurestore-runtime/2020-07-01/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-20 01:19:55.000000 botocore-a-la-carte-sagemaker-featurestore-runtime-1.31.6/botocore/data/sagemaker-featurestore-runtime/2020-07-01/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-20 01:19:55.000000 botocore-a-la-carte-sagemaker-featurestore-runtime-1.31.6/botocore/data/sagemaker-featurestore-runtime/2020-07-01/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    20573 2023-07-20 01:19:55.000000 botocore-a-la-carte-sagemaker-featurestore-runtime-1.31.6/botocore/data/sagemaker-featurestore-runtime/2020-07-01/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:20:45.014915 botocore-a-la-carte-sagemaker-featurestore-runtime-1.31.6/botocore_a_la_carte_sagemaker_featurestore_runtime.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-20 01:20:44.000000 botocore-a-la-carte-sagemaker-featurestore-runtime-1.31.6/botocore_a_la_carte_sagemaker_featurestore_runtime.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-07-20 01:20:44.000000 botocore-a-la-carte-sagemaker-featurestore-runtime-1.31.6/botocore_a_la_carte_sagemaker_featurestore_runtime.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 01:20:44.000000 botocore-a-la-carte-sagemaker-featurestore-runtime-1.31.6/botocore_a_la_carte_sagemaker_featurestore_runtime.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-20 01:20:44.000000 botocore-a-la-carte-sagemaker-featurestore-runtime-1.31.6/botocore_a_la_carte_sagemaker_featurestore_runtime.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 01:20:45.014915 botocore-a-la-carte-sagemaker-featurestore-runtime-1.31.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-07-20 01:20:44.000000 botocore-a-la-carte-sagemaker-featurestore-runtime-1.31.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:55.251547 botocore-a-la-carte-sagemaker-featurestore-runtime-1.31.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-21 01:21:55.000000 botocore-a-la-carte-sagemaker-featurestore-runtime-1.31.8/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-21 01:21:55.251547 botocore-a-la-carte-sagemaker-featurestore-runtime-1.31.8/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:55.251547 botocore-a-la-carte-sagemaker-featurestore-runtime-1.31.8/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:55.251547 botocore-a-la-carte-sagemaker-featurestore-runtime-1.31.8/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:55.251547 botocore-a-la-carte-sagemaker-featurestore-runtime-1.31.8/botocore/data/sagemaker-featurestore-runtime/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:55.251547 botocore-a-la-carte-sagemaker-featurestore-runtime-1.31.8/botocore/data/sagemaker-featurestore-runtime/2020-07-01/
+-rw-r--r--   0 runner    (1001) docker     (123)    17720 2023-07-21 01:21:06.000000 botocore-a-la-carte-sagemaker-featurestore-runtime-1.31.8/botocore/data/sagemaker-featurestore-runtime/2020-07-01/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-21 01:21:06.000000 botocore-a-la-carte-sagemaker-featurestore-runtime-1.31.8/botocore/data/sagemaker-featurestore-runtime/2020-07-01/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-21 01:21:06.000000 botocore-a-la-carte-sagemaker-featurestore-runtime-1.31.8/botocore/data/sagemaker-featurestore-runtime/2020-07-01/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    21619 2023-07-21 01:21:06.000000 botocore-a-la-carte-sagemaker-featurestore-runtime-1.31.8/botocore/data/sagemaker-featurestore-runtime/2020-07-01/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:55.251547 botocore-a-la-carte-sagemaker-featurestore-runtime-1.31.8/botocore_a_la_carte_sagemaker_featurestore_runtime.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-21 01:21:55.000000 botocore-a-la-carte-sagemaker-featurestore-runtime-1.31.8/botocore_a_la_carte_sagemaker_featurestore_runtime.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-07-21 01:21:55.000000 botocore-a-la-carte-sagemaker-featurestore-runtime-1.31.8/botocore_a_la_carte_sagemaker_featurestore_runtime.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 01:21:55.000000 botocore-a-la-carte-sagemaker-featurestore-runtime-1.31.8/botocore_a_la_carte_sagemaker_featurestore_runtime.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-21 01:21:55.000000 botocore-a-la-carte-sagemaker-featurestore-runtime-1.31.8/botocore_a_la_carte_sagemaker_featurestore_runtime.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 01:21:55.251547 botocore-a-la-carte-sagemaker-featurestore-runtime-1.31.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-07-21 01:21:55.000000 botocore-a-la-carte-sagemaker-featurestore-runtime-1.31.8/setup.py
```

### Comparing `botocore-a-la-carte-sagemaker-featurestore-runtime-1.31.6/LICENSE.txt` & `botocore-a-la-carte-sagemaker-featurestore-runtime-1.31.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-sagemaker-featurestore-runtime-1.31.6/PKG-INFO` & `botocore-a-la-carte-sagemaker-featurestore-runtime-1.31.8/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-sagemaker-featurestore-runtime
-Version: 1.31.6
+Version: 1.31.8
 Summary: sagemaker-featurestore-runtime data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-sagemaker-featurestore-runtime-1.31.6/botocore/data/sagemaker-featurestore-runtime/2020-07-01/endpoint-rule-set-1.json` & `botocore-a-la-carte-sagemaker-featurestore-runtime-1.31.8/botocore/data/sagemaker-featurestore-runtime/2020-07-01/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-sagemaker-featurestore-runtime-1.31.6/botocore/data/sagemaker-featurestore-runtime/2020-07-01/service-2.json` & `botocore-a-la-carte-sagemaker-featurestore-runtime-1.31.8/botocore/data/sagemaker-featurestore-runtime/2020-07-01/service-2.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9928028273809524%*

 * *Differences: {"'operations'": "{'PutRecord': {'documentation': '<p>The <code>PutRecord</code> API is used to "*

 * *                 'ingest a list of <code>Records</code> into your feature group. </p> <p>If a new '*

 * *                 'record’s <code>EventTime</code> is greater, the new record is written to both '*

 * *                 'the <code>OnlineStore</code> and <code>OfflineStore</code>. Otherwise, the '*

 * *                 'record is a historic record and it is written only to the '*

 * *                 '<code>OfflineStore</code> […]*

```diff
@@ -93,15 +93,15 @@
             },
             "name": "GetRecord",
             "output": {
                 "shape": "GetRecordResponse"
             }
         },
         "PutRecord": {
-            "documentation": "<p>Used for data ingestion into the <code>FeatureStore</code>. The <code>PutRecord</code> API writes to both the <code>OnlineStore</code> and <code>OfflineStore</code>. If the record is the latest record for the <code>recordIdentifier</code>, the record is written to both the <code>OnlineStore</code> and <code>OfflineStore</code>. If the record is a historic record, it is written only to the <code>OfflineStore</code>.</p>",
+            "documentation": "<p>The <code>PutRecord</code> API is used to ingest a list of <code>Records</code> into your feature group. </p> <p>If a new record\u2019s <code>EventTime</code> is greater, the new record is written to both the <code>OnlineStore</code> and <code>OfflineStore</code>. Otherwise, the record is a historic record and it is written only to the <code>OfflineStore</code>. </p> <p>You can specify the ingestion to be applied to the <code>OnlineStore</code>, <code>OfflineStore</code>, or both by using the <code>TargetStores</code> request parameter. </p> <p>You can set the ingested record to expire at a given time to live (TTL) duration after the record\u2019s event time, <code>ExpiresAt</code> = <code>EventTime</code> + <code>TtlDuration</code>, by specifying the <code>TtlDuration</code> parameter. A record level <code>TtlDuration</code> is set when specifying the <code>TtlDuration</code> parameter using the <code>PutRecord</code> API call. If the input <code>TtlDuration</code> is <code>null</code> or unspecified, <code>TtlDuration</code> is set to the default feature group level <code>TtlDuration</code>. A record level <code>TtlDuration</code> supersedes the group level <code>TtlDuration</code>.</p>",
             "errors": [
                 {
                     "shape": "ValidationError"
                 },
                 {
                     "shape": "InternalFailure"
                 },
@@ -172,16 +172,16 @@
             "min": 0,
             "type": "list"
         },
         "BatchGetRecordIdentifier": {
             "documentation": "<p>The identifier that identifies the batch of Records you are retrieving in a batch.</p>",
             "members": {
                 "FeatureGroupName": {
-                    "documentation": "<p>A <code>FeatureGroupName</code> containing Records you are retrieving in a batch.</p>",
-                    "shape": "FeatureGroupName"
+                    "documentation": "<p>The name or Amazon Resource Name (ARN) of the <code>FeatureGroup</code> containing the records you are retrieving in a batch.</p>",
+                    "shape": "FeatureGroupNameOrArn"
                 },
                 "FeatureNames": {
                     "documentation": "<p>List of names of Features to be retrieved. If not specified, the latest value for all the Features are returned.</p>",
                     "shape": "FeatureNames"
                 },
                 "RecordIdentifiersValueAsString": {
                     "documentation": "<p>The value for a list of record identifiers in string format.</p>",
@@ -205,15 +205,15 @@
         "BatchGetRecordRequest": {
             "members": {
                 "ExpirationTimeResponse": {
                     "documentation": "<p>Parameter to request <code>ExpiresAt</code> in response. If <code>Enabled</code>, <code>BatchGetRecord</code> will return the value of <code>ExpiresAt</code>, if it is not null. If <code>Disabled</code> and null, <code>BatchGetRecord</code> will return null.</p>",
                     "shape": "ExpirationTimeResponse"
                 },
                 "Identifiers": {
-                    "documentation": "<p>A list of <code>FeatureGroup</code> names, with their corresponding <code>RecordIdentifier</code> value, and Feature name that have been requested to be retrieved in batch.</p>",
+                    "documentation": "<p>A list containing the name or Amazon Resource Name (ARN) of the <code>FeatureGroup</code>, the list of names of <code>Feature</code>s to be retrieved, and the corresponding <code>RecordIdentifier</code> values as strings.</p>",
                     "shape": "BatchGetRecordIdentifiers"
                 }
             },
             "required": [
                 "Identifiers"
             ],
             "type": "structure"
@@ -237,15 +237,15 @@
                 "Records",
                 "Errors",
                 "UnprocessedIdentifiers"
             ],
             "type": "structure"
         },
         "BatchGetRecordResultDetail": {
-            "documentation": "<p>The output of Records that have been retrieved in a batch.</p>",
+            "documentation": "<p>The output of records that have been retrieved in a batch.</p>",
             "members": {
                 "ExpiresAt": {
                     "documentation": "<p>The <code>ExpiresAt</code> ISO string of the requested record.</p>",
                     "shape": "ExpiresAt"
                 },
                 "FeatureGroupName": {
                     "documentation": "<p>The <code>FeatureGroupName</code> containing Records you retrieved in a batch.</p>",
@@ -285,18 +285,18 @@
                 "EventTime": {
                     "documentation": "<p>Timestamp indicating when the deletion event occurred. <code>EventTime</code> can be used to query data at a certain point in time.</p>",
                     "location": "querystring",
                     "locationName": "EventTime",
                     "shape": "ValueAsString"
                 },
                 "FeatureGroupName": {
-                    "documentation": "<p>The name of the feature group to delete the record from. </p>",
+                    "documentation": "<p>The name or Amazon Resource Name (ARN) of the feature group to delete the record from. </p>",
                     "location": "uri",
                     "locationName": "FeatureGroupName",
-                    "shape": "FeatureGroupName"
+                    "shape": "FeatureGroupNameOrArn"
                 },
                 "RecordIdentifierValueAsString": {
                     "documentation": "<p>The value for the <code>RecordIdentifier</code> that uniquely identifies the record, in string format. </p>",
                     "location": "querystring",
                     "locationName": "RecordIdentifierValueAsString",
                     "shape": "ValueAsString"
                 },
@@ -327,18 +327,18 @@
                 "Disabled"
             ],
             "type": "string"
         },
         "ExpiresAt": {
             "type": "string"
         },
-        "FeatureGroupName": {
-            "max": 64,
+        "FeatureGroupNameOrArn": {
+            "max": 150,
             "min": 1,
-            "pattern": "^[a-zA-Z0-9]([-_]*[a-zA-Z0-9]){0,63}",
+            "pattern": "(arn:aws[a-z\\-]*:sagemaker:[a-z0-9\\-]*:[0-9]{12}:feature-group/)?([a-zA-Z0-9]([-_]*[a-zA-Z0-9]){0,63})",
             "type": "string"
         },
         "FeatureName": {
             "max": 64,
             "min": 1,
             "pattern": "^[a-zA-Z0-9]([-_]*[a-zA-Z0-9]){0,63}",
             "type": "string"
@@ -367,24 +367,24 @@
                 "ValueAsString"
             ],
             "type": "structure"
         },
         "GetRecordRequest": {
             "members": {
                 "ExpirationTimeResponse": {
-                    "documentation": "<p>Parameter to request <code>ExpiresAt</code> in response. If <code>Enabled</code>, <code>BatchGetRecord</code> will return the value of <code>ExpiresAt</code>, if it is not null. If <code>Disabled</code> and null, <code>BatchGetRecord</code> will return null.</p>",
+                    "documentation": "<p>Parameter to request <code>ExpiresAt</code> in response. If <code>Enabled</code>, <code>GetRecord</code> will return the value of <code>ExpiresAt</code>, if it is not null. If <code>Disabled</code> and null, <code>GetRecord</code> will return null.</p>",
                     "location": "querystring",
                     "locationName": "ExpirationTimeResponse",
                     "shape": "ExpirationTimeResponse"
                 },
                 "FeatureGroupName": {
-                    "documentation": "<p>The name of the feature group from which you want to retrieve a record.</p>",
+                    "documentation": "<p>The name or Amazon Resource Name (ARN) of the feature group from which you want to retrieve a record.</p>",
                     "location": "uri",
                     "locationName": "FeatureGroupName",
-                    "shape": "FeatureGroupName"
+                    "shape": "FeatureGroupNameOrArn"
                 },
                 "FeatureNames": {
                     "documentation": "<p>List of names of Features to be retrieved. If not specified, the latest value for all the Features are returned.</p>",
                     "location": "querystring",
                     "locationName": "FeatureName",
                     "shape": "FeatureNames"
                 },
@@ -432,18 +432,18 @@
         "Message": {
             "max": 2048,
             "type": "string"
         },
         "PutRecordRequest": {
             "members": {
                 "FeatureGroupName": {
-                    "documentation": "<p>The name of the feature group that you want to insert the record into.</p>",
+                    "documentation": "<p>The name or Amazon Resource Name (ARN) of the feature group that you want to insert the record into.</p>",
                     "location": "uri",
                     "locationName": "FeatureGroupName",
-                    "shape": "FeatureGroupName"
+                    "shape": "FeatureGroupNameOrArn"
                 },
                 "Record": {
                     "documentation": "<p>List of FeatureValues to be inserted. This will be a full over-write. If you only want to update few of the feature values, do the following:</p> <ul> <li> <p>Use <code>GetRecord</code> to retrieve the latest record.</p> </li> <li> <p>Update the record returned from <code>GetRecord</code>. </p> </li> <li> <p>Use <code>PutRecord</code> to update feature values.</p> </li> </ul>",
                     "shape": "Record"
                 },
                 "TargetStores": {
                     "documentation": "<p>A list of stores to which you're adding the record. By default, Feature Store adds the record to all of the stores that you're using for the <code>FeatureGroup</code>.</p>",
```

### Comparing `botocore-a-la-carte-sagemaker-featurestore-runtime-1.31.6/botocore_a_la_carte_sagemaker_featurestore_runtime.egg-info/PKG-INFO` & `botocore-a-la-carte-sagemaker-featurestore-runtime-1.31.8/botocore_a_la_carte_sagemaker_featurestore_runtime.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-sagemaker-featurestore-runtime
-Version: 1.31.6
+Version: 1.31.8
 Summary: sagemaker-featurestore-runtime data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-sagemaker-featurestore-runtime-1.31.6/botocore_a_la_carte_sagemaker_featurestore_runtime.egg-info/SOURCES.txt` & `botocore-a-la-carte-sagemaker-featurestore-runtime-1.31.8/botocore_a_la_carte_sagemaker_featurestore_runtime.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-sagemaker-featurestore-runtime-1.31.6/setup.py` & `botocore-a-la-carte-sagemaker-featurestore-runtime-1.31.8/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-sagemaker-featurestore-runtime',
-    version="1.31.6",
+    version="1.31.8",
     description='sagemaker-featurestore-runtime data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/sagemaker-featurestore-runtime/*/*.json'],
```

