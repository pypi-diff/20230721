# Comparing `tmp/botocore-a-la-carte-savingsplans-1.31.6.tar.gz` & `tmp/botocore-a-la-carte-savingsplans-1.31.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-savingsplans-1.31.6.tar", last modified: Thu Jul 20 01:20:46 2023, max compression
+gzip compressed data, was "botocore-a-la-carte-savingsplans-1.31.8.tar", last modified: Fri Jul 21 01:21:56 2023, max compression
```

## Comparing `botocore-a-la-carte-savingsplans-1.31.6.tar` & `botocore-a-la-carte-savingsplans-1.31.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:20:46.070923 botocore-a-la-carte-savingsplans-1.31.6/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-20 01:20:45.000000 botocore-a-la-carte-savingsplans-1.31.6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-20 01:20:46.070923 botocore-a-la-carte-savingsplans-1.31.6/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:20:46.070923 botocore-a-la-carte-savingsplans-1.31.6/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:20:46.070923 botocore-a-la-carte-savingsplans-1.31.6/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:20:46.070923 botocore-a-la-carte-savingsplans-1.31.6/botocore/data/savingsplans/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:20:46.070923 botocore-a-la-carte-savingsplans-1.31.6/botocore/data/savingsplans/2019-06-28/
--rw-r--r--   0 runner    (1001) docker     (123)    27074 2023-07-20 01:19:55.000000 botocore-a-la-carte-savingsplans-1.31.6/botocore/data/savingsplans/2019-06-28/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-20 01:19:55.000000 botocore-a-la-carte-savingsplans-1.31.6/botocore/data/savingsplans/2019-06-28/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-20 01:19:55.000000 botocore-a-la-carte-savingsplans-1.31.6/botocore/data/savingsplans/2019-06-28/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    35887 2023-07-20 01:19:55.000000 botocore-a-la-carte-savingsplans-1.31.6/botocore/data/savingsplans/2019-06-28/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:20:46.070923 botocore-a-la-carte-savingsplans-1.31.6/botocore_a_la_carte_savingsplans.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-20 01:20:46.000000 botocore-a-la-carte-savingsplans-1.31.6/botocore_a_la_carte_savingsplans.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-20 01:20:46.000000 botocore-a-la-carte-savingsplans-1.31.6/botocore_a_la_carte_savingsplans.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 01:20:46.000000 botocore-a-la-carte-savingsplans-1.31.6/botocore_a_la_carte_savingsplans.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-20 01:20:46.000000 botocore-a-la-carte-savingsplans-1.31.6/botocore_a_la_carte_savingsplans.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 01:20:46.070923 botocore-a-la-carte-savingsplans-1.31.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-07-20 01:20:45.000000 botocore-a-la-carte-savingsplans-1.31.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:56.343566 botocore-a-la-carte-savingsplans-1.31.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-21 01:21:56.000000 botocore-a-la-carte-savingsplans-1.31.8/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-21 01:21:56.343566 botocore-a-la-carte-savingsplans-1.31.8/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:56.343566 botocore-a-la-carte-savingsplans-1.31.8/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:56.343566 botocore-a-la-carte-savingsplans-1.31.8/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:56.343566 botocore-a-la-carte-savingsplans-1.31.8/botocore/data/savingsplans/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:56.343566 botocore-a-la-carte-savingsplans-1.31.8/botocore/data/savingsplans/2019-06-28/
+-rw-r--r--   0 runner    (1001) docker     (123)    20442 2023-07-21 01:21:06.000000 botocore-a-la-carte-savingsplans-1.31.8/botocore/data/savingsplans/2019-06-28/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-21 01:21:06.000000 botocore-a-la-carte-savingsplans-1.31.8/botocore/data/savingsplans/2019-06-28/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-21 01:21:06.000000 botocore-a-la-carte-savingsplans-1.31.8/botocore/data/savingsplans/2019-06-28/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    35888 2023-07-21 01:21:06.000000 botocore-a-la-carte-savingsplans-1.31.8/botocore/data/savingsplans/2019-06-28/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:56.343566 botocore-a-la-carte-savingsplans-1.31.8/botocore_a_la_carte_savingsplans.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-21 01:21:56.000000 botocore-a-la-carte-savingsplans-1.31.8/botocore_a_la_carte_savingsplans.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-21 01:21:56.000000 botocore-a-la-carte-savingsplans-1.31.8/botocore_a_la_carte_savingsplans.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 01:21:56.000000 botocore-a-la-carte-savingsplans-1.31.8/botocore_a_la_carte_savingsplans.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-21 01:21:56.000000 botocore-a-la-carte-savingsplans-1.31.8/botocore_a_la_carte_savingsplans.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 01:21:56.343566 botocore-a-la-carte-savingsplans-1.31.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-07-21 01:21:56.000000 botocore-a-la-carte-savingsplans-1.31.8/setup.py
```

### Comparing `botocore-a-la-carte-savingsplans-1.31.6/LICENSE.txt` & `botocore-a-la-carte-savingsplans-1.31.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-savingsplans-1.31.6/PKG-INFO` & `botocore-a-la-carte-savingsplans-1.31.8/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-savingsplans
-Version: 1.31.6
+Version: 1.31.8
 Summary: savingsplans data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-savingsplans-1.31.6/botocore/data/savingsplans/2019-06-28/endpoint-rule-set-1.json` & `botocore-a-la-carte-savingsplans-1.31.8/botocore/data/savingsplans/2019-06-28/endpoint-rule-set-1.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8977218230238341%*

 * *Differences: {"'rules'": "{0: {'conditions': {0: {'fn': 'isSet', 'argv': {0: {'ref': 'Endpoint'}}, delete: "*

 * *            "['assign']}}, 'rules': {0: {'type': 'error', 'error': 'Invalid Configuration: FIPS "*

 * *            "and custom endpoint are not supported', delete: ['rules']}, 1: {'rules': {0: "*

 * *            "{'conditions': {0: {'fn': 'booleanEquals', 'argv': {0: {'ref': 'UseDualStack'}, "*

 * *            "insert: [(1, True)], delete: [1]}}}, 'type': 'error', 'error': 'Invalid "*

 * *            "Configuration: Dualstack and cu […]*

```diff
@@ -29,563 +29,373 @@
     },
     "rules": [
         {
             "conditions": [
                 {
                     "argv": [
                         {
-                            "ref": "Region"
+                            "ref": "Endpoint"
                         }
                     ],
-                    "assign": "PartitionResult",
-                    "fn": "aws.partition"
+                    "fn": "isSet"
                 }
             ],
             "rules": [
                 {
                     "conditions": [
                         {
                             "argv": [
                                 {
-                                    "ref": "Endpoint"
-                                }
-                            ],
-                            "fn": "isSet"
-                        },
-                        {
-                            "argv": [
-                                {
-                                    "ref": "Endpoint"
-                                }
+                                    "ref": "UseFIPS"
+                                },
+                                true
                             ],
-                            "assign": "url",
-                            "fn": "parseURL"
+                            "fn": "booleanEquals"
                         }
                     ],
+                    "error": "Invalid Configuration: FIPS and custom endpoint are not supported",
+                    "type": "error"
+                },
+                {
+                    "conditions": [],
                     "rules": [
                         {
                             "conditions": [
                                 {
                                     "argv": [
                                         {
-                                            "ref": "UseFIPS"
+                                            "ref": "UseDualStack"
                                         },
                                         true
                                     ],
                                     "fn": "booleanEquals"
                                 }
                             ],
-                            "error": "Invalid Configuration: FIPS and custom endpoint are not supported",
+                            "error": "Invalid Configuration: Dualstack and custom endpoint are not supported",
                             "type": "error"
                         },
                         {
                             "conditions": [],
-                            "rules": [
-                                {
-                                    "conditions": [
-                                        {
-                                            "argv": [
-                                                {
-                                                    "ref": "UseDualStack"
-                                                },
-                                                true
-                                            ],
-                                            "fn": "booleanEquals"
-                                        }
-                                    ],
-                                    "error": "Invalid Configuration: Dualstack and custom endpoint are not supported",
-                                    "type": "error"
-                                },
-                                {
-                                    "conditions": [],
-                                    "endpoint": {
-                                        "headers": {},
-                                        "properties": {},
-                                        "url": {
-                                            "ref": "Endpoint"
-                                        }
-                                    },
-                                    "type": "endpoint"
+                            "endpoint": {
+                                "headers": {},
+                                "properties": {},
+                                "url": {
+                                    "ref": "Endpoint"
                                 }
-                            ],
-                            "type": "tree"
+                            },
+                            "type": "endpoint"
                         }
                     ],
                     "type": "tree"
-                },
+                }
+            ],
+            "type": "tree"
+        },
+        {
+            "conditions": [],
+            "rules": [
                 {
                     "conditions": [
                         {
                             "argv": [
                                 {
-                                    "argv": [
-                                        {
-                                            "ref": "PartitionResult"
-                                        },
-                                        "name"
-                                    ],
-                                    "fn": "getAttr"
-                                },
-                                "aws"
+                                    "ref": "Region"
+                                }
                             ],
-                            "fn": "stringEquals"
+                            "fn": "isSet"
                         }
                     ],
                     "rules": [
                         {
                             "conditions": [
                                 {
                                     "argv": [
                                         {
-                                            "ref": "UseFIPS"
-                                        },
-                                        true
-                                    ],
-                                    "fn": "booleanEquals"
-                                },
-                                {
-                                    "argv": [
-                                        {
-                                            "ref": "UseDualStack"
-                                        },
-                                        true
+                                            "ref": "Region"
+                                        }
                                     ],
-                                    "fn": "booleanEquals"
+                                    "assign": "PartitionResult",
+                                    "fn": "aws.partition"
                                 }
                             ],
                             "rules": [
                                 {
                                     "conditions": [
                                         {
                                             "argv": [
-                                                true,
                                                 {
                                                     "argv": [
                                                         {
                                                             "ref": "PartitionResult"
                                                         },
-                                                        "supportsFIPS"
+                                                        "name"
                                                     ],
                                                     "fn": "getAttr"
-                                                }
+                                                },
+                                                "aws"
                                             ],
-                                            "fn": "booleanEquals"
+                                            "fn": "stringEquals"
                                         },
                                         {
                                             "argv": [
-                                                true,
                                                 {
-                                                    "argv": [
-                                                        {
-                                                            "ref": "PartitionResult"
-                                                        },
-                                                        "supportsDualStack"
-                                                    ],
-                                                    "fn": "getAttr"
-                                                }
+                                                    "ref": "UseFIPS"
+                                                },
+                                                false
                                             ],
                                             "fn": "booleanEquals"
-                                        }
-                                    ],
-                                    "rules": [
+                                        },
                                         {
-                                            "conditions": [],
-                                            "endpoint": {
-                                                "headers": {},
-                                                "properties": {
-                                                    "authSchemes": [
-                                                        {
-                                                            "name": "sigv4",
-                                                            "signingName": "savingsplans",
-                                                            "signingRegion": "us-east-1"
-                                                        }
-                                                    ]
+                                            "argv": [
+                                                {
+                                                    "ref": "UseDualStack"
                                                 },
-                                                "url": "https://savingsplans-fips.{Region}.api.aws"
-                                            },
-                                            "type": "endpoint"
+                                                false
+                                            ],
+                                            "fn": "booleanEquals"
                                         }
                                     ],
-                                    "type": "tree"
+                                    "endpoint": {
+                                        "headers": {},
+                                        "properties": {
+                                            "authSchemes": [
+                                                {
+                                                    "name": "sigv4",
+                                                    "signingName": "savingsplans",
+                                                    "signingRegion": "us-east-1"
+                                                }
+                                            ]
+                                        },
+                                        "url": "https://savingsplans.amazonaws.com"
+                                    },
+                                    "type": "endpoint"
                                 },
                                 {
-                                    "conditions": [],
-                                    "error": "FIPS and DualStack are enabled, but this partition does not support one or both",
-                                    "type": "error"
-                                }
-                            ],
-                            "type": "tree"
-                        },
-                        {
-                            "conditions": [
-                                {
-                                    "argv": [
+                                    "conditions": [
                                         {
-                                            "ref": "UseFIPS"
+                                            "argv": [
+                                                {
+                                                    "ref": "UseFIPS"
+                                                },
+                                                true
+                                            ],
+                                            "fn": "booleanEquals"
                                         },
-                                        true
-                                    ],
-                                    "fn": "booleanEquals"
-                                }
-                            ],
-                            "rules": [
-                                {
-                                    "conditions": [
                                         {
                                             "argv": [
-                                                true,
                                                 {
-                                                    "argv": [
-                                                        {
-                                                            "ref": "PartitionResult"
-                                                        },
-                                                        "supportsFIPS"
-                                                    ],
-                                                    "fn": "getAttr"
-                                                }
+                                                    "ref": "UseDualStack"
+                                                },
+                                                true
                                             ],
                                             "fn": "booleanEquals"
                                         }
                                     ],
                                     "rules": [
                                         {
-                                            "conditions": [],
-                                            "endpoint": {
-                                                "headers": {},
-                                                "properties": {
-                                                    "authSchemes": [
+                                            "conditions": [
+                                                {
+                                                    "argv": [
+                                                        true,
                                                         {
-                                                            "name": "sigv4",
-                                                            "signingName": "savingsplans",
-                                                            "signingRegion": "us-east-1"
+                                                            "argv": [
+                                                                {
+                                                                    "ref": "PartitionResult"
+                                                                },
+                                                                "supportsFIPS"
+                                                            ],
+                                                            "fn": "getAttr"
                                                         }
-                                                    ]
+                                                    ],
+                                                    "fn": "booleanEquals"
                                                 },
-                                                "url": "https://savingsplans-fips.{Region}.amazonaws.com"
-                                            },
-                                            "type": "endpoint"
+                                                {
+                                                    "argv": [
+                                                        true,
+                                                        {
+                                                            "argv": [
+                                                                {
+                                                                    "ref": "PartitionResult"
+                                                                },
+                                                                "supportsDualStack"
+                                                            ],
+                                                            "fn": "getAttr"
+                                                        }
+                                                    ],
+                                                    "fn": "booleanEquals"
+                                                }
+                                            ],
+                                            "rules": [
+                                                {
+                                                    "conditions": [],
+                                                    "rules": [
+                                                        {
+                                                            "conditions": [],
+                                                            "endpoint": {
+                                                                "headers": {},
+                                                                "properties": {},
+                                                                "url": "https://savingsplans-fips.{Region}.{PartitionResult#dualStackDnsSuffix}"
+                                                            },
+                                                            "type": "endpoint"
+                                                        }
+                                                    ],
+                                                    "type": "tree"
+                                                }
+                                            ],
+                                            "type": "tree"
+                                        },
+                                        {
+                                            "conditions": [],
+                                            "error": "FIPS and DualStack are enabled, but this partition does not support one or both",
+                                            "type": "error"
                                         }
                                     ],
                                     "type": "tree"
                                 },
                                 {
-                                    "conditions": [],
-                                    "error": "FIPS is enabled but this partition does not support FIPS",
-                                    "type": "error"
-                                }
-                            ],
-                            "type": "tree"
-                        },
-                        {
-                            "conditions": [
-                                {
-                                    "argv": [
-                                        {
-                                            "ref": "UseDualStack"
-                                        },
-                                        true
-                                    ],
-                                    "fn": "booleanEquals"
-                                }
-                            ],
-                            "rules": [
-                                {
                                     "conditions": [
                                         {
                                             "argv": [
-                                                true,
                                                 {
-                                                    "argv": [
-                                                        {
-                                                            "ref": "PartitionResult"
-                                                        },
-                                                        "supportsDualStack"
-                                                    ],
-                                                    "fn": "getAttr"
-                                                }
+                                                    "ref": "UseFIPS"
+                                                },
+                                                true
                                             ],
                                             "fn": "booleanEquals"
                                         }
                                     ],
                                     "rules": [
                                         {
-                                            "conditions": [],
-                                            "endpoint": {
-                                                "headers": {},
-                                                "properties": {
-                                                    "authSchemes": [
+                                            "conditions": [
+                                                {
+                                                    "argv": [
+                                                        true,
                                                         {
-                                                            "name": "sigv4",
-                                                            "signingName": "savingsplans",
-                                                            "signingRegion": "us-east-1"
+                                                            "argv": [
+                                                                {
+                                                                    "ref": "PartitionResult"
+                                                                },
+                                                                "supportsFIPS"
+                                                            ],
+                                                            "fn": "getAttr"
                                                         }
-                                                    ]
-                                                },
-                                                "url": "https://savingsplans.{Region}.api.aws"
-                                            },
-                                            "type": "endpoint"
+                                                    ],
+                                                    "fn": "booleanEquals"
+                                                }
+                                            ],
+                                            "rules": [
+                                                {
+                                                    "conditions": [],
+                                                    "rules": [
+                                                        {
+                                                            "conditions": [],
+                                                            "endpoint": {
+                                                                "headers": {},
+                                                                "properties": {},
+                                                                "url": "https://savingsplans-fips.{Region}.{PartitionResult#dnsSuffix}"
+                                                            },
+                                                            "type": "endpoint"
+                                                        }
+                                                    ],
+                                                    "type": "tree"
+                                                }
+                                            ],
+                                            "type": "tree"
+                                        },
+                                        {
+                                            "conditions": [],
+                                            "error": "FIPS is enabled but this partition does not support FIPS",
+                                            "type": "error"
                                         }
                                     ],
                                     "type": "tree"
                                 },
                                 {
-                                    "conditions": [],
-                                    "error": "DualStack is enabled but this partition does not support DualStack",
-                                    "type": "error"
-                                }
-                            ],
-                            "type": "tree"
-                        },
-                        {
-                            "conditions": [],
-                            "endpoint": {
-                                "headers": {},
-                                "properties": {
-                                    "authSchemes": [
-                                        {
-                                            "name": "sigv4",
-                                            "signingName": "savingsplans",
-                                            "signingRegion": "us-east-1"
-                                        }
-                                    ]
-                                },
-                                "url": "https://savingsplans.amazonaws.com"
-                            },
-                            "type": "endpoint"
-                        }
-                    ],
-                    "type": "tree"
-                },
-                {
-                    "conditions": [
-                        {
-                            "argv": [
-                                {
-                                    "ref": "UseFIPS"
-                                },
-                                true
-                            ],
-                            "fn": "booleanEquals"
-                        },
-                        {
-                            "argv": [
-                                {
-                                    "ref": "UseDualStack"
-                                },
-                                true
-                            ],
-                            "fn": "booleanEquals"
-                        }
-                    ],
-                    "rules": [
-                        {
-                            "conditions": [
-                                {
-                                    "argv": [
-                                        true,
+                                    "conditions": [
                                         {
                                             "argv": [
                                                 {
-                                                    "ref": "PartitionResult"
+                                                    "ref": "UseDualStack"
                                                 },
-                                                "supportsFIPS"
+                                                true
                                             ],
-                                            "fn": "getAttr"
+                                            "fn": "booleanEquals"
                                         }
                                     ],
-                                    "fn": "booleanEquals"
-                                },
-                                {
-                                    "argv": [
-                                        true,
+                                    "rules": [
                                         {
-                                            "argv": [
+                                            "conditions": [
                                                 {
-                                                    "ref": "PartitionResult"
-                                                },
-                                                "supportsDualStack"
+                                                    "argv": [
+                                                        true,
+                                                        {
+                                                            "argv": [
+                                                                {
+                                                                    "ref": "PartitionResult"
+                                                                },
+                                                                "supportsDualStack"
+                                                            ],
+                                                            "fn": "getAttr"
+                                                        }
+                                                    ],
+                                                    "fn": "booleanEquals"
+                                                }
                                             ],
-                                            "fn": "getAttr"
-                                        }
-                                    ],
-                                    "fn": "booleanEquals"
-                                }
-                            ],
-                            "rules": [
-                                {
-                                    "conditions": [],
-                                    "endpoint": {
-                                        "headers": {},
-                                        "properties": {},
-                                        "url": "https://savingsplans-fips.{Region}.{PartitionResult#dualStackDnsSuffix}"
-                                    },
-                                    "type": "endpoint"
-                                }
-                            ],
-                            "type": "tree"
-                        },
-                        {
-                            "conditions": [],
-                            "error": "FIPS and DualStack are enabled, but this partition does not support one or both",
-                            "type": "error"
-                        }
-                    ],
-                    "type": "tree"
-                },
-                {
-                    "conditions": [
-                        {
-                            "argv": [
-                                {
-                                    "ref": "UseFIPS"
-                                },
-                                true
-                            ],
-                            "fn": "booleanEquals"
-                        }
-                    ],
-                    "rules": [
-                        {
-                            "conditions": [
-                                {
-                                    "argv": [
-                                        true,
-                                        {
-                                            "argv": [
+                                            "rules": [
                                                 {
-                                                    "ref": "PartitionResult"
-                                                },
-                                                "supportsFIPS"
+                                                    "conditions": [],
+                                                    "rules": [
+                                                        {
+                                                            "conditions": [],
+                                                            "endpoint": {
+                                                                "headers": {},
+                                                                "properties": {},
+                                                                "url": "https://savingsplans.{Region}.{PartitionResult#dualStackDnsSuffix}"
+                                                            },
+                                                            "type": "endpoint"
+                                                        }
+                                                    ],
+                                                    "type": "tree"
+                                                }
                                             ],
-                                            "fn": "getAttr"
+                                            "type": "tree"
+                                        },
+                                        {
+                                            "conditions": [],
+                                            "error": "DualStack is enabled but this partition does not support DualStack",
+                                            "type": "error"
                                         }
                                     ],
-                                    "fn": "booleanEquals"
-                                }
-                            ],
-                            "rules": [
+                                    "type": "tree"
+                                },
                                 {
                                     "conditions": [],
                                     "rules": [
                                         {
                                             "conditions": [],
                                             "endpoint": {
                                                 "headers": {},
                                                 "properties": {},
-                                                "url": "https://savingsplans-fips.{Region}.{PartitionResult#dnsSuffix}"
+                                                "url": "https://savingsplans.{Region}.{PartitionResult#dnsSuffix}"
                                             },
                                             "type": "endpoint"
                                         }
                                     ],
                                     "type": "tree"
                                 }
                             ],
                             "type": "tree"
-                        },
-                        {
-                            "conditions": [],
-                            "error": "FIPS is enabled but this partition does not support FIPS",
-                            "type": "error"
-                        }
-                    ],
-                    "type": "tree"
-                },
-                {
-                    "conditions": [
-                        {
-                            "argv": [
-                                {
-                                    "ref": "UseDualStack"
-                                },
-                                true
-                            ],
-                            "fn": "booleanEquals"
-                        }
-                    ],
-                    "rules": [
-                        {
-                            "conditions": [
-                                {
-                                    "argv": [
-                                        true,
-                                        {
-                                            "argv": [
-                                                {
-                                                    "ref": "PartitionResult"
-                                                },
-                                                "supportsDualStack"
-                                            ],
-                                            "fn": "getAttr"
-                                        }
-                                    ],
-                                    "fn": "booleanEquals"
-                                }
-                            ],
-                            "rules": [
-                                {
-                                    "conditions": [],
-                                    "endpoint": {
-                                        "headers": {},
-                                        "properties": {},
-                                        "url": "https://savingsplans.{Region}.{PartitionResult#dualStackDnsSuffix}"
-                                    },
-                                    "type": "endpoint"
-                                }
-                            ],
-                            "type": "tree"
-                        },
-                        {
-                            "conditions": [],
-                            "error": "DualStack is enabled but this partition does not support DualStack",
-                            "type": "error"
                         }
                     ],
                     "type": "tree"
                 },
                 {
                     "conditions": [],
-                    "rules": [
-                        {
-                            "conditions": [
-                                {
-                                    "argv": [
-                                        {
-                                            "ref": "Region"
-                                        },
-                                        "aws-global"
-                                    ],
-                                    "fn": "stringEquals"
-                                }
-                            ],
-                            "endpoint": {
-                                "headers": {},
-                                "properties": {
-                                    "authSchemes": [
-                                        {
-                                            "name": "sigv4",
-                                            "signingName": "savingsplans",
-                                            "signingRegion": "us-east-1"
-                                        }
-                                    ]
-                                },
-                                "url": "https://savingsplans.amazonaws.com"
-                            },
-                            "type": "endpoint"
-                        },
-                        {
-                            "conditions": [],
-                            "endpoint": {
-                                "headers": {},
-                                "properties": {},
-                                "url": "https://savingsplans.{Region}.{PartitionResult#dnsSuffix}"
-                            },
-                            "type": "endpoint"
-                        }
-                    ],
-                    "type": "tree"
+                    "error": "Invalid Configuration: Missing Region",
+                    "type": "error"
                 }
             ],
             "type": "tree"
         }
     ],
     "version": "1.0"
 }
```

### Comparing `botocore-a-la-carte-savingsplans-1.31.6/botocore/data/savingsplans/2019-06-28/service-2.json` & `botocore-a-la-carte-savingsplans-1.31.8/botocore/data/savingsplans/2019-06-28/service-2.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999949433656958%*

 * *Differences: {"'shapes'": "{'DescribeSavingsPlanRatesResponse': {'members': {'nextToken': {'documentation': "*

 * *             "'<p>The token to use to retrieve the next page of results. This value is null when "*

 * *             "there are no more results to return. </p>'}}}}"}*

```diff
@@ -341,15 +341,15 @@
                 "savingsPlanId"
             ],
             "type": "structure"
         },
         "DescribeSavingsPlanRatesResponse": {
             "members": {
                 "nextToken": {
-                    "documentation": "<p>The token to use to retrieve the next page of results. This value is null when there are no more results to return.</p>",
+                    "documentation": "<p>The token to use to retrieve the next page of results. This value is null when there are no more results to return. </p>",
                     "shape": "PaginationToken"
                 },
                 "savingsPlanId": {
                     "documentation": "<p>The ID of the Savings Plan.</p>",
                     "shape": "SavingsPlanId"
                 },
                 "searchResults": {
```

### Comparing `botocore-a-la-carte-savingsplans-1.31.6/botocore_a_la_carte_savingsplans.egg-info/PKG-INFO` & `botocore-a-la-carte-savingsplans-1.31.8/botocore_a_la_carte_savingsplans.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-savingsplans
-Version: 1.31.6
+Version: 1.31.8
 Summary: savingsplans data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-savingsplans-1.31.6/setup.py` & `botocore-a-la-carte-savingsplans-1.31.8/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-savingsplans',
-    version="1.31.6",
+    version="1.31.8",
     description='savingsplans data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/savingsplans/*/*.json'],
```

