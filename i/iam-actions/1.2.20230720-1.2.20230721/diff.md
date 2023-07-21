# Comparing `tmp/iam_actions-1.2.20230720.tar.gz` & `tmp/iam_actions-1.2.20230721.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iam_actions-1.2.20230720.tar", max compression
+gzip compressed data, was "iam_actions-1.2.20230721.tar", max compression
```

## Comparing `iam_actions-1.2.20230720.tar` & `iam_actions-1.2.20230721.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1071 2023-07-20 02:27:19.671966 iam_actions-1.2.20230720/LICENSE
--rw-r--r--   0        0        0     2302 2023-07-20 02:27:19.671966 iam_actions-1.2.20230720/README.md
--rw-r--r--   0        0        0      228 2023-07-20 02:27:19.671966 iam_actions-1.2.20230720/iam_actions/__init__.py
--rw-r--r--   0        0        0  4369784 2023-07-20 02:28:53.588926 iam_actions-1.2.20230720/iam_actions/actions.json
--rw-r--r--   0        0        0      496 2023-07-20 02:27:19.671966 iam_actions-1.2.20230720/iam_actions/data.py
--rw-r--r--   0        0        0       80 2023-07-20 02:27:19.671966 iam_actions-1.2.20230720/iam_actions/generate/__init__.py
--rw-r--r--   0        0        0     3097 2023-07-20 02:27:19.675966 iam_actions-1.2.20230720/iam_actions/generate/action_map.py
--rw-r--r--   0        0        0    23329 2023-07-20 02:27:19.675966 iam_actions-1.2.20230720/iam_actions/generate/aws_docs.py
--rw-r--r--   0        0        0     3739 2023-07-20 02:27:19.675966 iam_actions-1.2.20230720/iam_actions/generate/generate.py
--rw-r--r--   0        0        0     3272 2023-07-20 02:27:19.675966 iam_actions-1.2.20230720/iam_actions/generate/notifier.py
--rw-r--r--   0        0        0     1902 2023-07-20 02:27:19.675966 iam_actions-1.2.20230720/iam_actions/generate/resource_type.py
--rw-r--r--   0        0        0     2277 2023-07-20 02:27:19.675966 iam_actions-1.2.20230720/iam_actions/generate/services.py
--rw-r--r--   0        0        0   561962 2023-07-20 02:28:53.588926 iam_actions-1.2.20230720/iam_actions/policies.json
--rw-r--r--   0        0        0   197396 2023-07-20 02:28:53.588926 iam_actions-1.2.20230720/iam_actions/resourcetypes.json
--rw-r--r--   0        0        0   545071 2023-07-20 02:28:53.588926 iam_actions-1.2.20230720/iam_actions/services.json
--rw-r--r--   0        0        0     1154 2023-07-20 02:28:54.384934 iam_actions-1.2.20230720/pyproject.toml
--rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230720/setup.py
--rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230720/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-21 02:29:38.151328 iam_actions-1.2.20230721/LICENSE
+-rw-r--r--   0        0        0     2302 2023-07-21 02:29:38.151328 iam_actions-1.2.20230721/README.md
+-rw-r--r--   0        0        0      228 2023-07-21 02:29:38.151328 iam_actions-1.2.20230721/iam_actions/__init__.py
+-rw-r--r--   0        0        0  4374432 2023-07-21 02:31:28.925346 iam_actions-1.2.20230721/iam_actions/actions.json
+-rw-r--r--   0        0        0      496 2023-07-21 02:29:38.151328 iam_actions-1.2.20230721/iam_actions/data.py
+-rw-r--r--   0        0        0       80 2023-07-21 02:29:38.151328 iam_actions-1.2.20230721/iam_actions/generate/__init__.py
+-rw-r--r--   0        0        0     3097 2023-07-21 02:29:38.151328 iam_actions-1.2.20230721/iam_actions/generate/action_map.py
+-rw-r--r--   0        0        0    23329 2023-07-21 02:29:38.151328 iam_actions-1.2.20230721/iam_actions/generate/aws_docs.py
+-rw-r--r--   0        0        0     3739 2023-07-21 02:29:38.151328 iam_actions-1.2.20230721/iam_actions/generate/generate.py
+-rw-r--r--   0        0        0     3272 2023-07-21 02:29:38.151328 iam_actions-1.2.20230721/iam_actions/generate/notifier.py
+-rw-r--r--   0        0        0     1902 2023-07-21 02:29:38.151328 iam_actions-1.2.20230721/iam_actions/generate/resource_type.py
+-rw-r--r--   0        0        0     2277 2023-07-21 02:29:38.151328 iam_actions-1.2.20230721/iam_actions/generate/services.py
+-rw-r--r--   0        0        0   562970 2023-07-21 02:31:28.925346 iam_actions-1.2.20230721/iam_actions/policies.json
+-rw-r--r--   0        0        0   197420 2023-07-21 02:31:28.925346 iam_actions-1.2.20230721/iam_actions/resourcetypes.json
+-rw-r--r--   0        0        0   546046 2023-07-21 02:31:28.925346 iam_actions-1.2.20230721/iam_actions/services.json
+-rw-r--r--   0        0        0     1154 2023-07-21 02:31:29.741361 iam_actions-1.2.20230721/pyproject.toml
+-rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230721/setup.py
+-rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230721/PKG-INFO
```

### Comparing `iam_actions-1.2.20230720/LICENSE` & `iam_actions-1.2.20230721/LICENSE`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230720/README.md` & `iam_actions-1.2.20230721/README.md`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230720/iam_actions/actions.json` & `iam_actions-1.2.20230721/iam_actions/actions.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9971001826651639%*

 * *Differences: {"'ds'": "{'UpdateAuthorizedApplication': OrderedDict([('access_level', 'Undocumented'), "*

 * *         "('action', 'UpdateAuthorizedApplication'), ('condition_keys', []), ('description', 'Not "*

 * *         "Documented by AWS'), ('orphan', False), ('resources', [])])}",*

 * * "'grafana'": "{'ListVersions': {'access_level': 'List', 'description': 'Grants permission to list "*

 * *              'all available supported Grafana versions. Optionally, include a workspace to list '*

 * *              "the versions to which it can be u […]*

```diff
@@ -42408,14 +42408,22 @@
             "condition_keys": [],
             "description": "Grants permission to stop the directory sharing between the directory owner and consumer accounts",
             "orphan": false,
             "resources": [
                 "directory"
             ]
         },
+        "UpdateAuthorizedApplication": {
+            "access_level": "Undocumented",
+            "action": "UpdateAuthorizedApplication",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "UpdateConditionalForwarder": {
             "access_level": "Write",
             "action": "UpdateConditionalForwarder",
             "condition_keys": [],
             "description": "Grants permission to update a conditional forwarder that has been set up for your AWS directory",
             "orphan": false,
             "resources": [
@@ -69808,20 +69816,22 @@
             "description": "Grants permission to list tags associated with a workspace",
             "orphan": false,
             "resources": [
                 "workspace"
             ]
         },
         "ListVersions": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "ListVersions",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to list all available supported Grafana versions. Optionally, include a workspace to list the versions to which it can be upgraded",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "workspace"
+            ]
         },
         "ListWorkspaces": {
             "access_level": "Read",
             "action": "ListWorkspaces",
             "condition_keys": [],
             "description": "Grants permission to list workspaces",
             "orphan": false,
@@ -98093,14 +98103,160 @@
             "description": "Grants permission to update the VOD source with the specified VOD source name on the source location with the specified source location name",
             "orphan": false,
             "resources": [
                 "vodSource"
             ]
         }
     },
+    "medical-imaging": {
+        "CopyImageSet": {
+            "access_level": "Undocumented",
+            "action": "CopyImageSet",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "CreateDatastore": {
+            "access_level": "Undocumented",
+            "action": "CreateDatastore",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "DeleteDatastore": {
+            "access_level": "Undocumented",
+            "action": "DeleteDatastore",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "DeleteImageSet": {
+            "access_level": "Undocumented",
+            "action": "DeleteImageSet",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "GetDICOMImportJob": {
+            "access_level": "Undocumented",
+            "action": "GetDICOMImportJob",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "GetDatastore": {
+            "access_level": "Undocumented",
+            "action": "GetDatastore",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "GetImageFrame": {
+            "access_level": "Undocumented",
+            "action": "GetImageFrame",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "GetImageSet": {
+            "access_level": "Undocumented",
+            "action": "GetImageSet",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "GetImageSetMetadata": {
+            "access_level": "Undocumented",
+            "action": "GetImageSetMetadata",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ListDICOMImportJobs": {
+            "access_level": "Undocumented",
+            "action": "ListDICOMImportJobs",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ListDatastores": {
+            "access_level": "Undocumented",
+            "action": "ListDatastores",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ListImageSetVersions": {
+            "access_level": "Undocumented",
+            "action": "ListImageSetVersions",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ListTagsForResource": {
+            "access_level": "Undocumented",
+            "action": "ListTagsForResource",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "SearchImageSets": {
+            "access_level": "Undocumented",
+            "action": "SearchImageSets",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "StartDICOMImportJob": {
+            "access_level": "Undocumented",
+            "action": "StartDICOMImportJob",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "TagResource": {
+            "access_level": "Undocumented",
+            "action": "TagResource",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "UntagResource": {
+            "access_level": "Undocumented",
+            "action": "UntagResource",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "UpdateImageSetMetadata": {
+            "access_level": "Undocumented",
+            "action": "UpdateImageSetMetadata",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        }
+    },
     "memorydb": {
         "BatchUpdateCluster": {
             "access_level": "Write",
             "action": "BatchUpdateCluster",
             "condition_keys": [
                 "aws:ResourceTag/${TagKey}"
             ],
@@ -132972,22 +133128,46 @@
             "access_level": "List",
             "action": "ListSubscribers",
             "condition_keys": [],
             "description": "Grants permission to list all subscribers",
             "orphan": false,
             "resources": []
         },
+        "ListTagsForResource": {
+            "access_level": "Undocumented",
+            "action": "ListTagsForResource",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "RegisterDataLakeDelegatedAdministrator": {
             "access_level": "Write",
             "action": "RegisterDataLakeDelegatedAdministrator",
             "condition_keys": [],
             "description": "Grants permission to designate an account as the Amazon Security Lake administrator account for the organization",
             "orphan": false,
             "resources": []
         },
+        "TagResource": {
+            "access_level": "Undocumented",
+            "action": "TagResource",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "UntagResource": {
+            "access_level": "Undocumented",
+            "action": "UntagResource",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "UpdateDataLake": {
             "access_level": "Write",
             "action": "UpdateDataLake",
             "condition_keys": [],
             "description": "Grants permission to update a security data lake",
             "orphan": false,
             "resources": [
```

### Comparing `iam_actions-1.2.20230720/iam_actions/generate/action_map.py` & `iam_actions-1.2.20230721/iam_actions/generate/action_map.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230720/iam_actions/generate/aws_docs.py` & `iam_actions-1.2.20230721/iam_actions/generate/aws_docs.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230720/iam_actions/generate/generate.py` & `iam_actions-1.2.20230721/iam_actions/generate/generate.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230720/iam_actions/generate/notifier.py` & `iam_actions-1.2.20230721/iam_actions/generate/notifier.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230720/iam_actions/generate/resource_type.py` & `iam_actions-1.2.20230721/iam_actions/generate/resource_type.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230720/iam_actions/generate/services.py` & `iam_actions-1.2.20230721/iam_actions/generate/services.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230720/iam_actions/policies.json` & `iam_actions-1.2.20230721/iam_actions/policies.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9997152019229161%*

 * *Differences: {"'serviceMap'": "{'AWS Directory Service': {'Actions': {insert: [(66, "*

 * *                 "'UpdateAuthorizedApplication')]}}, 'Amazon Security Lake': {'Actions': {insert: "*

 * *                 "[(23, 'ListTagsForResource'), (25, 'TagResource'), (26, 'UntagResource')]}, "*

 * *                 "'conditionKeys': ['aws:RequestTag/${TagKey}', 'aws:ResourceTag/${TagKey}', "*

 * *                 "'aws:TagKeys']}, 'AWS HealthImaging': OrderedDict([('StringPrefix', "*

 * *                 "'medical-imaging'), ('Actions', ['CopyImag […]*

```diff
@@ -3200,14 +3200,15 @@
                 "RemoveTagsFromResource",
                 "ResetUserPassword",
                 "RestoreFromSnapshot",
                 "ShareDirectory",
                 "StartSchemaExtension",
                 "UnauthorizeApplication",
                 "UnshareDirectory",
+                "UpdateAuthorizedApplication",
                 "UpdateConditionalForwarder",
                 "UpdateDirectorySetup",
                 "UpdateNumberOfDomainControllers",
                 "UpdateRadius",
                 "UpdateSettings",
                 "UpdateTrust",
                 "VerifyTrust"
@@ -4457,14 +4458,45 @@
             "HasResource": true,
             "StringPrefix": "health",
             "conditionKeys": [
                 "health:eventTypeCode",
                 "health:service"
             ]
         },
+        "AWS HealthImaging": {
+            "ARNFormat": "arn:aws:medical-imaging:${Region}:${Account}:${ResourceType}/${ResourceName}",
+            "ARNRegex": "^arn:aws:medical-imaging:.+:.+:.+",
+            "Actions": [
+                "CopyImageSet",
+                "CreateDatastore",
+                "DeleteDatastore",
+                "DeleteImageSet",
+                "GetDICOMImportJob",
+                "GetDatastore",
+                "GetImageFrame",
+                "GetImageSet",
+                "GetImageSetMetadata",
+                "ListDICOMImportJobs",
+                "ListDatastores",
+                "ListImageSetVersions",
+                "ListTagsForResource",
+                "SearchImageSets",
+                "StartDICOMImportJob",
+                "TagResource",
+                "UntagResource",
+                "UpdateImageSetMetadata"
+            ],
+            "HasResource": true,
+            "StringPrefix": "medical-imaging",
+            "conditionKeys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:ResourceTag/${TagKey}",
+                "aws:TagKeys"
+            ]
+        },
         "AWS IAM Access Analyzer": {
             "ARNFormat": "arn:aws:access-analyzer:${Region}:${Account}:analyzer/${AnalyzerName}",
             "ARNRegex": "^arn:aws:access-analyzer:.+",
             "Actions": [
                 "ApplyArchiveRule",
                 "CancelPolicyGeneration",
                 "CreateAccessPreview",
@@ -19143,22 +19175,30 @@
                 "GetDataLakeOrganizationConfiguration",
                 "GetDataLakeSources",
                 "GetSubscriber",
                 "ListDataLakeExceptions",
                 "ListDataLakes",
                 "ListLogSources",
                 "ListSubscribers",
+                "ListTagsForResource",
                 "RegisterDataLakeDelegatedAdministrator",
+                "TagResource",
+                "UntagResource",
                 "UpdateDataLake",
                 "UpdateDataLakeExceptionSubscription",
                 "UpdateSubscriber",
                 "UpdateSubscriberNotification"
             ],
             "HasResource": true,
-            "StringPrefix": "securitylake"
+            "StringPrefix": "securitylake",
+            "conditionKeys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:ResourceTag/${TagKey}",
+                "aws:TagKeys"
+            ]
         },
         "Amazon Session Manager Message Gateway Service": {
             "Actions": [
                 "CreateControlChannel",
                 "CreateDataChannel",
                 "OpenControlChannel",
                 "OpenDataChannel"
```

### Comparing `iam_actions-1.2.20230720/iam_actions/resourcetypes.json` & `iam_actions-1.2.20230721/iam_actions/resourcetypes.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9972602739726028%*

 * *Differences: {"'medical-imaging'": 'OrderedDict()'}*

```diff
@@ -4252,14 +4252,15 @@
             "condition_keys": "aws:ResourceTag/${TagKey}"
         },
         "vodSource": {
             "arn_pattern": "arn:*:mediatailor:*:*:vodSource/*/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         }
     },
+    "medical-imaging": {},
     "memorydb": {
         "acl": {
             "arn_pattern": "arn:*:memorydb:*:*:acl/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         },
         "cluster": {
             "arn_pattern": "arn:*:memorydb:*:*:cluster/*",
```

### Comparing `iam_actions-1.2.20230720/iam_actions/services.json` & `iam_actions-1.2.20230721/iam_actions/services.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9971335288005638%*

 * *Differences: {"'ds'": "{'Actions': {insert: [(66, 'UpdateAuthorizedApplication')]}}",*

 * * "'medical-imaging'": "OrderedDict([('Actions', ['CopyImageSet', 'CreateDatastore', "*

 * *                      "'DeleteDatastore', 'DeleteImageSet', 'GetDICOMImportJob', 'GetDatastore', "*

 * *                      "'GetImageFrame', 'GetImageSet', 'GetImageSetMetadata', "*

 * *                      "'ListDICOMImportJobs', 'ListDatastores', 'ListImageSetVersions', "*

 * *                      "'ListTagsForResource', 'SearchImageSets', 'StartDICOMImportJo […]*

```diff
@@ -6288,14 +6288,15 @@
             "RemoveTagsFromResource",
             "ResetUserPassword",
             "RestoreFromSnapshot",
             "ShareDirectory",
             "StartSchemaExtension",
             "UnauthorizeApplication",
             "UnshareDirectory",
+            "UpdateAuthorizedApplication",
             "UpdateConditionalForwarder",
             "UpdateDirectorySetup",
             "UpdateNumberOfDomainControllers",
             "UpdateRadius",
             "UpdateSettings",
             "UpdateTrust",
             "VerifyTrust"
@@ -13716,14 +13717,51 @@
             "aws:TagKeys"
         ],
         "HasResource": true,
         "ServiceNames": [
             "AWS Elemental MediaTailor"
         ]
     },
+    "medical-imaging": {
+        "ARNFormats": [
+            "arn:aws:medical-imaging:${Region}:${Account}:${ResourceType}/${ResourceName}"
+        ],
+        "ARNRegexes": [
+            "^arn:aws:medical-imaging:.+:.+:.+"
+        ],
+        "Actions": [
+            "CopyImageSet",
+            "CreateDatastore",
+            "DeleteDatastore",
+            "DeleteImageSet",
+            "GetDICOMImportJob",
+            "GetDatastore",
+            "GetImageFrame",
+            "GetImageSet",
+            "GetImageSetMetadata",
+            "ListDICOMImportJobs",
+            "ListDatastores",
+            "ListImageSetVersions",
+            "ListTagsForResource",
+            "SearchImageSets",
+            "StartDICOMImportJob",
+            "TagResource",
+            "UntagResource",
+            "UpdateImageSetMetadata"
+        ],
+        "ConditionKeys": [
+            "aws:RequestTag/${TagKey}",
+            "aws:ResourceTag/${TagKey}",
+            "aws:TagKeys"
+        ],
+        "HasResource": true,
+        "ServiceNames": [
+            "AWS HealthImaging"
+        ]
+    },
     "memorydb": {
         "ARNFormats": [
             "arn:aws:memorydb:${Region}:${Account}:${ResourceType}/${ResourceName}"
         ],
         "ARNRegexes": [
             "^arn:aws:memorydb:.+:.+:.+"
         ],
@@ -18421,21 +18459,28 @@
             "GetDataLakeOrganizationConfiguration",
             "GetDataLakeSources",
             "GetSubscriber",
             "ListDataLakeExceptions",
             "ListDataLakes",
             "ListLogSources",
             "ListSubscribers",
+            "ListTagsForResource",
             "RegisterDataLakeDelegatedAdministrator",
+            "TagResource",
+            "UntagResource",
             "UpdateDataLake",
             "UpdateDataLakeExceptionSubscription",
             "UpdateSubscriber",
             "UpdateSubscriberNotification"
         ],
-        "ConditionKeys": [],
+        "ConditionKeys": [
+            "aws:RequestTag/${TagKey}",
+            "aws:ResourceTag/${TagKey}",
+            "aws:TagKeys"
+        ],
         "HasResource": true,
         "ServiceNames": [
             "Amazon Security Lake"
         ]
     },
     "serverlessrepo": {
         "ARNFormats": [
```

### Comparing `iam_actions-1.2.20230720/pyproject.toml` & `iam_actions-1.2.20230721/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iam-actions"
-version = "1.2.20230720"
+version = "1.2.20230721"
 description = "JSON of AWS policy components"
 authors = ["Constable <info@constableapp.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/constableapp/iam_actions"
 packages = [{include = "iam_actions"}]
```

### Comparing `iam_actions-1.2.20230720/setup.py` & `iam_actions-1.2.20230721/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['iam_actions', 'iam_actions.generate']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'iam-actions',
-    'version': '1.2.20230720',
+    'version': '1.2.20230721',
     'description': 'JSON of AWS policy components',
     'long_description': '# iam_actions\n\n`iam_actions` is a python module which contains a dictionary of AWS IAM information. Ideally, it is a complete catalog of all AWS services, actions, and resource types. The information is scraped from the AWS documentation pages.\n\nNightly, the scraping service runs, and publishes a new version with the date appended. \n\nThe package is meant to be used as a consumable package, but it also contains the code to generate the definitions for packaging.\n\nThere are three "roots" that you can consume: actions, resource_types, and services. They all currently return as dict\'s. *However, in a future release, it will be returned as python data structures*\n\n## Actions\n\nActions is a listing of all the actions for a given service. The structure is as follows:\n```\n{\n    "service_name": {\n        "action_name: {\n            "access_level": access_level,\n            "action": action_name,\n            "condition_keys": [condition_key1, ...],\n            "description": description\n        }\n    }\n}\n```\n\nTherefore, you can find information about an action as follows\n\n```\n>>> iam_actions.actions[\'s3\'][\'GetObject\']\n{\'access_level\': \'Read\', \'action\': \'GetObject\', \'condition_keys\': [\'s3:AccessPointNetworkOrigin\', \'s3:DataAccessPointAccount\', \'s3:DataAccessPointArn\', \'s3:ExistingObjectTag/<key>\', \'s3:ResourceAccount\', \'s3:TlsVersion\', \'s3:authType\', \'s3:signatureAge\', \'s3:signatureversion\', \'s3:x-amz-content-sha256\'], \'description\': \'Grants permission to retrieve objects from Amazon S3\', \'orphan\': False, \'resources\': [\'object\']}\n```\n\n## Services\n\nServices list information about the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "Actions": [action1, ...]\n        "ServiceNames": [service_name1, ...]\n        "ARNFormats": [arn_format1, ...]\n        "ConditionKeys": [condition_key1, ...]\n        "HasResource": bool\n    }\n}\n```\n\n## Resource Types\n\nResource Types list information about the resource types for the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "resource_name": {\n            "arn_pattern": arn_pattern,\n            "condition_keys": [condition_key1, ...]\n        }\n    }\n}\n```\n\n## Usage\n\n```python\nimport iam_actions\n\nprint(item_actions.services)\nprint(item_actions.actions)\nprint(item_actions.resource_types)\n```\n',
     'author': 'Constable',
     'author_email': 'info@constableapp.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/constableapp/iam_actions',
```

### Comparing `iam_actions-1.2.20230720/PKG-INFO` & `iam_actions-1.2.20230721/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iam-actions
-Version: 1.2.20230720
+Version: 1.2.20230721
 Summary: JSON of AWS policy components
 Home-page: https://github.com/constableapp/iam_actions
 License: MIT
 Author: Constable
 Author-email: info@constableapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

