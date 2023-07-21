# Comparing `tmp/botocore-a-la-carte-connectcases-1.31.6.tar.gz` & `tmp/botocore-a-la-carte-connectcases-1.31.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-connectcases-1.31.6.tar", last modified: Thu Jul 20 01:20:11 2023, max compression
+gzip compressed data, was "botocore-a-la-carte-connectcases-1.31.8.tar", last modified: Fri Jul 21 01:21:20 2023, max compression
```

## Comparing `botocore-a-la-carte-connectcases-1.31.6.tar` & `botocore-a-la-carte-connectcases-1.31.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:20:11.638610 botocore-a-la-carte-connectcases-1.31.6/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-20 01:20:11.000000 botocore-a-la-carte-connectcases-1.31.6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-20 01:20:11.638610 botocore-a-la-carte-connectcases-1.31.6/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:20:11.638610 botocore-a-la-carte-connectcases-1.31.6/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:20:11.638610 botocore-a-la-carte-connectcases-1.31.6/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:20:11.638610 botocore-a-la-carte-connectcases-1.31.6/botocore/data/connectcases/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:20:11.638610 botocore-a-la-carte-connectcases-1.31.6/botocore/data/connectcases/2022-10-03/
--rw-r--r--   0 runner    (1001) docker     (123)    17620 2023-07-20 01:19:55.000000 botocore-a-la-carte-connectcases-1.31.6/botocore/data/connectcases/2022-10-03/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-20 01:19:55.000000 botocore-a-la-carte-connectcases-1.31.6/botocore/data/connectcases/2022-10-03/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    94848 2023-07-20 01:19:55.000000 botocore-a-la-carte-connectcases-1.31.6/botocore/data/connectcases/2022-10-03/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:20:11.638610 botocore-a-la-carte-connectcases-1.31.6/botocore_a_la_carte_connectcases.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-20 01:20:11.000000 botocore-a-la-carte-connectcases-1.31.6/botocore_a_la_carte_connectcases.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-20 01:20:11.000000 botocore-a-la-carte-connectcases-1.31.6/botocore_a_la_carte_connectcases.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 01:20:11.000000 botocore-a-la-carte-connectcases-1.31.6/botocore_a_la_carte_connectcases.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-20 01:20:11.000000 botocore-a-la-carte-connectcases-1.31.6/botocore_a_la_carte_connectcases.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 01:20:11.638610 botocore-a-la-carte-connectcases-1.31.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-07-20 01:20:11.000000 botocore-a-la-carte-connectcases-1.31.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:20.334906 botocore-a-la-carte-connectcases-1.31.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-21 01:21:20.000000 botocore-a-la-carte-connectcases-1.31.8/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-21 01:21:20.334906 botocore-a-la-carte-connectcases-1.31.8/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:20.334906 botocore-a-la-carte-connectcases-1.31.8/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:20.334906 botocore-a-la-carte-connectcases-1.31.8/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:20.334906 botocore-a-la-carte-connectcases-1.31.8/botocore/data/connectcases/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:20.334906 botocore-a-la-carte-connectcases-1.31.8/botocore/data/connectcases/2022-10-03/
+-rw-r--r--   0 runner    (1001) docker     (123)    17620 2023-07-21 01:21:06.000000 botocore-a-la-carte-connectcases-1.31.8/botocore/data/connectcases/2022-10-03/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-21 01:21:06.000000 botocore-a-la-carte-connectcases-1.31.8/botocore/data/connectcases/2022-10-03/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    96025 2023-07-21 01:21:06.000000 botocore-a-la-carte-connectcases-1.31.8/botocore/data/connectcases/2022-10-03/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:20.334906 botocore-a-la-carte-connectcases-1.31.8/botocore_a_la_carte_connectcases.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-21 01:21:20.000000 botocore-a-la-carte-connectcases-1.31.8/botocore_a_la_carte_connectcases.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-21 01:21:20.000000 botocore-a-la-carte-connectcases-1.31.8/botocore_a_la_carte_connectcases.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 01:21:20.000000 botocore-a-la-carte-connectcases-1.31.8/botocore_a_la_carte_connectcases.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-21 01:21:20.000000 botocore-a-la-carte-connectcases-1.31.8/botocore_a_la_carte_connectcases.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 01:21:20.334906 botocore-a-la-carte-connectcases-1.31.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-07-21 01:21:20.000000 botocore-a-la-carte-connectcases-1.31.8/setup.py
```

### Comparing `botocore-a-la-carte-connectcases-1.31.6/LICENSE.txt` & `botocore-a-la-carte-connectcases-1.31.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-connectcases-1.31.6/PKG-INFO` & `botocore-a-la-carte-connectcases-1.31.8/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-connectcases
-Version: 1.31.6
+Version: 1.31.8
 Summary: connectcases data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-connectcases-1.31.6/botocore/data/connectcases/2022-10-03/endpoint-rule-set-1.json` & `botocore-a-la-carte-connectcases-1.31.8/botocore/data/connectcases/2022-10-03/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-connectcases-1.31.6/botocore/data/connectcases/2022-10-03/service-2.json` & `botocore-a-la-carte-connectcases-1.31.8/botocore/data/connectcases/2022-10-03/service-2.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9986639317889316%*

 * *Differences: {"'operations'": "{'CreateDomain': {'documentation': '<p>Creates a domain, which is a container "*

 * *                 'for all case data, such as cases, fields, templates and layouts. Each Amazon '*

 * *                 'Connect instance can be associated with only one Cases domain.</p> <important> '*

 * *                 '<p>This will not associate your connect instance to Cases domain. Instead, use '*

 * *                 'the Amazon Connect <a '*

 * *                 'href="https://docs.aws.amazon.com/connect/latest/APIReferen […]*

```diff
@@ -114,15 +114,15 @@
             },
             "name": "CreateCase",
             "output": {
                 "shape": "CreateCaseResponse"
             }
         },
         "CreateDomain": {
-            "documentation": "<p>Creates a domain, which is a container for all case data, such as cases, fields, templates and layouts. Each Amazon Connect instance can be associated with only one Cases domain.</p> <important> <p>This will not associate your connect instance to Cases domain. Instead, use the Amazon Connect <a href=\"https://docs.aws.amazon.com/connect/latest/APIReference/API_CreateIntegrationAssociation.html\">CreateIntegrationAssociation</a> API. You need specific IAM permissions to successfully associate the Cases domain. For more information, see <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/required-permissions-iam-cases.html#onboard-cases-iam\">Onboard to Cases</a>.</p> </important>",
+            "documentation": "<p>Creates a domain, which is a container for all case data, such as cases, fields, templates and layouts. Each Amazon Connect instance can be associated with only one Cases domain.</p> <important> <p>This will not associate your connect instance to Cases domain. Instead, use the Amazon Connect <a href=\"https://docs.aws.amazon.com/connect/latest/APIReference/API_CreateIntegrationAssociation.html\">CreateIntegrationAssociation</a> API. You need specific IAM permissions to successfully associate the Cases domain. For more information, see <a href=\"https://docs.aws.amazon.com/connect/latest/adminguide/required-permissions-iam-cases.html#onboard-cases-iam\">Onboard to Cases</a>.</p> <pre><code> &lt;/important&gt; </code></pre>",
             "errors": [
                 {
                     "shape": "InternalServerException"
                 },
                 {
                     "shape": "ValidationException"
                 },
@@ -302,15 +302,15 @@
             },
             "name": "CreateTemplate",
             "output": {
                 "shape": "CreateTemplateResponse"
             }
         },
         "DeleteDomain": {
-            "documentation": "<p>Deletes a domain.</p>",
+            "documentation": "<p>Deletes a Cases domain.</p> <pre><code> &lt;note&gt; &lt;p&gt;After deleting your domain you must disassociate the deleted domain from your Amazon Connect instance with another API call before being able to use Cases again with this Amazon Connect instance. See &lt;a href=&quot;https://docs.aws.amazon.com/connect/latest/APIReference/API_DeleteIntegrationAssociation.html&quot;&gt;DeleteIntegrationAssociation&lt;/a&gt;.&lt;/p&gt; &lt;/note&gt; </code></pre>",
             "errors": [
                 {
                     "shape": "InternalServerException"
                 },
                 {
                     "shape": "ResourceNotFoundException"
                 },
@@ -1214,27 +1214,39 @@
                 },
                 "field": {
                     "documentation": "<p>A list of fields to filter on.</p>",
                     "shape": "FieldFilter"
                 },
                 "not": {
                     "shape": "CaseFilter"
+                },
+                "orAll": {
+                    "documentation": "<p>Provides \"or all\" filtering.</p>",
+                    "shape": "CaseFilterOrAllList"
                 }
             },
             "type": "structure",
             "union": true
         },
         "CaseFilterAndAllList": {
             "max": 10,
             "member": {
                 "shape": "CaseFilter"
             },
             "min": 0,
             "type": "list"
         },
+        "CaseFilterOrAllList": {
+            "max": 10,
+            "member": {
+                "shape": "CaseFilter"
+            },
+            "min": 0,
+            "type": "list"
+        },
         "CaseId": {
             "max": 500,
             "min": 1,
             "type": "string"
         },
         "CaseSummary": {
             "documentation": "<p>Case summary information.</p>",
@@ -1731,14 +1743,19 @@
             },
             "type": "list"
         },
         "Double": {
             "box": true,
             "type": "double"
         },
+        "EmptyFieldValue": {
+            "documentation": "<p>An empty value. You cannot set <code>EmptyFieldValue</code> on a field that is required on a case template.</p> <p>This structure will never have any data members. It signifies an empty value on a case field.</p>",
+            "members": {},
+            "type": "structure"
+        },
         "EventBridgeConfiguration": {
             "documentation": "<p>Configuration to enable EventBridge case event delivery and determine what data is delivered.</p>",
             "members": {
                 "enabled": {
                     "documentation": "<p>Indicates whether the to broadcast case event data to the customer.</p>",
                     "shape": "Boolean"
                 },
@@ -2036,14 +2053,18 @@
                     "documentation": "<p>Can be either null, or have a Boolean value type. Only one value can be provided.</p>",
                     "shape": "Boolean"
                 },
                 "doubleValue": {
                     "documentation": "<p>Can be either null, or have a Double number value type. Only one value can be provided.</p>",
                     "shape": "Double"
                 },
+                "emptyValue": {
+                    "documentation": "<p>An empty value.</p>",
+                    "shape": "EmptyFieldValue"
+                },
                 "stringValue": {
                     "documentation": "<p>String value type.</p>",
                     "shape": "FieldValueUnionStringValueString"
                 }
             },
             "type": "structure",
             "union": true
```

### Comparing `botocore-a-la-carte-connectcases-1.31.6/botocore_a_la_carte_connectcases.egg-info/PKG-INFO` & `botocore-a-la-carte-connectcases-1.31.8/botocore_a_la_carte_connectcases.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-connectcases
-Version: 1.31.6
+Version: 1.31.8
 Summary: connectcases data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-connectcases-1.31.6/setup.py` & `botocore-a-la-carte-connectcases-1.31.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-connectcases',
-    version="1.31.6",
+    version="1.31.8",
     description='connectcases data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/connectcases/*/*.json'],
```

