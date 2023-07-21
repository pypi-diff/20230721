# Comparing `tmp/djgraphql-1.0.8.tar.gz` & `tmp/djgraphql-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djgraphql-1.0.8.tar", last modified: Fri Jul 21 06:02:59 2023, max compression
+gzip compressed data, was "djgraphql-1.1.0.tar", last modified: Fri Jul 21 06:15:35 2023, max compression
```

## Comparing `djgraphql-1.0.8.tar` & `djgraphql-1.1.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 06:02:59.066905 djgraphql-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-21 06:02:41.000000 djgraphql-1.0.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-21 06:02:41.000000 djgraphql-1.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-07-21 06:02:59.066905 djgraphql-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-21 06:02:41.000000 djgraphql-1.0.8/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)    15022 2023-07-21 06:02:41.000000 djgraphql-1.0.8/Pipfile.lock
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-07-21 06:02:41.000000 djgraphql-1.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 06:02:59.066905 djgraphql-1.0.8/djgraphql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 06:02:41.000000 djgraphql-1.0.8/djgraphql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-21 06:02:41.000000 djgraphql-1.0.8/djgraphql/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-21 06:02:41.000000 djgraphql-1.0.8/djgraphql/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-07-21 06:02:41.000000 djgraphql-1.0.8/djgraphql/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-07-21 06:02:41.000000 djgraphql-1.0.8/djgraphql/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 06:02:59.066905 djgraphql-1.0.8/djgraphql/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 06:02:41.000000 djgraphql-1.0.8/djgraphql/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-21 06:02:41.000000 djgraphql-1.0.8/djgraphql/test/test_routers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-21 06:02:41.000000 djgraphql-1.0.8/djgraphql/test/test_schema_generation.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-21 06:02:41.000000 djgraphql-1.0.8/djgraphql/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 06:02:59.066905 djgraphql-1.0.8/djgraphql/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 06:02:41.000000 djgraphql-1.0.8/djgraphql/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-21 06:02:41.000000 djgraphql-1.0.8/djgraphql/utils/resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-07-21 06:02:41.000000 djgraphql-1.0.8/djgraphql/utils/routes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 06:02:59.066905 djgraphql-1.0.8/djgraphql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-07-21 06:02:58.000000 djgraphql-1.0.8/djgraphql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-21 06:02:59.000000 djgraphql-1.0.8/djgraphql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 06:02:58.000000 djgraphql-1.0.8/djgraphql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-21 06:02:58.000000 djgraphql-1.0.8/djgraphql.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-21 06:02:58.000000 djgraphql-1.0.8/djgraphql.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-21 06:02:41.000000 djgraphql-1.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 06:02:59.066905 djgraphql-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-07-21 06:02:41.000000 djgraphql-1.0.8/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-21 06:02:41.000000 djgraphql-1.0.8/version
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 06:15:35.503364 djgraphql-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-21 06:15:07.000000 djgraphql-1.1.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-21 06:15:07.000000 djgraphql-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-07-21 06:15:35.503364 djgraphql-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-21 06:15:07.000000 djgraphql-1.1.0/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)    13032 2023-07-21 06:15:07.000000 djgraphql-1.1.0/Pipfile.lock
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-07-21 06:15:07.000000 djgraphql-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 06:15:35.499364 djgraphql-1.1.0/djgraphql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 06:15:07.000000 djgraphql-1.1.0/djgraphql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-21 06:15:07.000000 djgraphql-1.1.0/djgraphql/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-21 06:15:07.000000 djgraphql-1.1.0/djgraphql/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-07-21 06:15:07.000000 djgraphql-1.1.0/djgraphql/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-07-21 06:15:07.000000 djgraphql-1.1.0/djgraphql/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 06:15:35.499364 djgraphql-1.1.0/djgraphql/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 06:15:07.000000 djgraphql-1.1.0/djgraphql/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-21 06:15:07.000000 djgraphql-1.1.0/djgraphql/test/test_routers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-21 06:15:07.000000 djgraphql-1.1.0/djgraphql/test/test_schema_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-21 06:15:07.000000 djgraphql-1.1.0/djgraphql/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 06:15:35.503364 djgraphql-1.1.0/djgraphql/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 06:15:07.000000 djgraphql-1.1.0/djgraphql/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-21 06:15:07.000000 djgraphql-1.1.0/djgraphql/utils/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-07-21 06:15:07.000000 djgraphql-1.1.0/djgraphql/utils/routes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 06:15:35.499364 djgraphql-1.1.0/djgraphql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-07-21 06:15:35.000000 djgraphql-1.1.0/djgraphql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-21 06:15:35.000000 djgraphql-1.1.0/djgraphql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 06:15:35.000000 djgraphql-1.1.0/djgraphql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-21 06:15:35.000000 djgraphql-1.1.0/djgraphql.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-21 06:15:35.000000 djgraphql-1.1.0/djgraphql.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-21 06:15:07.000000 djgraphql-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 06:15:35.503364 djgraphql-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-07-21 06:15:07.000000 djgraphql-1.1.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-21 06:15:07.000000 djgraphql-1.1.0/version
```

### Comparing `djgraphql-1.0.8/LICENSE.txt` & `djgraphql-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `djgraphql-1.0.8/PKG-INFO` & `djgraphql-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: djgraphql
-Version: 1.0.8
+Version: 1.1.0
 Summary: A package that makes easier to use graphql with django.
 Home-page: https://shitalluitel.com.np
 Author: Shital Babu Luitel
 Author-email: ctalluitel@gmail.com
 License: file: LICENSE.txt
 Description: file: README.md
 Platform: UNKNOWN
```

### Comparing `djgraphql-1.0.8/Pipfile.lock` & `djgraphql-1.1.0/Pipfile.lock`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9797647527910686%*

 * *Differences: {"'default'": '{\'six\': {\'markers\': "python_version >= \'2.7\' and python_version not in \'3.0, '*

 * *              '3.1, 3.2\'"}, delete: [\'backports.zoneinfo\']}',*

 * * "'develop'": '{\'decorator\': {\'markers\': "python_version > \'3.6\' and python_version < '*

 * *              '\'3.11\'"}, \'ipython\': {\'hashes\': '*

 * *              "['sha256:1d197b907b6ba441b692c48cf2a3a2de280dc0ac91a3405b39349a50272ca0a1', "*

 * *              "'sha256:248aca623f5c99a6635bc3857677b7320b9b8039f99f070ee0d20a5ca5a8e6bf'], "*

 * *            […]*

```diff
@@ -27,36 +27,14 @@
             "hashes": [
                 "sha256:89b2ef2247e3b562a16eef663bc0e2e703ec6468e2fa8a5cd61cd449786d4f6e",
                 "sha256:9e0ce3aa93a819ba5b45120216b23878cf6e8525eb3848653452b4192b92afed"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==3.7.2"
         },
-        "backports.zoneinfo": {
-            "hashes": [
-                "sha256:17746bd546106fa389c51dbea67c8b7c8f0d14b5526a579ca6ccf5ed72c526cf",
-                "sha256:1b13e654a55cd45672cb54ed12148cd33628f672548f373963b0bff67b217328",
-                "sha256:1c5742112073a563c81f786e77514969acb58649bcdf6cdf0b4ed31a348d4546",
-                "sha256:4a0f800587060bf8880f954dbef70de6c11bbe59c673c3d818921f042f9954a6",
-                "sha256:5c144945a7752ca544b4b78c8c41544cdfaf9786f25fe5ffb10e838e19a27570",
-                "sha256:7b0a64cda4145548fed9efc10322770f929b944ce5cee6c0dfe0c87bf4c0c8c9",
-                "sha256:8439c030a11780786a2002261569bdf362264f605dfa4d65090b64b05c9f79a7",
-                "sha256:8961c0f32cd0336fb8e8ead11a1f8cd99ec07145ec2931122faaac1c8f7fd987",
-                "sha256:89a48c0d158a3cc3f654da4c2de1ceba85263fafb861b98b59040a5086259722",
-                "sha256:a76b38c52400b762e48131494ba26be363491ac4f9a04c1b7e92483d169f6582",
-                "sha256:da6013fd84a690242c310d77ddb8441a559e9cb3d3d59ebac9aca1a57b2e18bc",
-                "sha256:e55b384612d93be96506932a786bbcde5a2db7a9e6a4bb4bffe8b733f5b9036b",
-                "sha256:e81b76cace8eda1fca50e345242ba977f9be6ae3945af8d46326d776b4cf78d1",
-                "sha256:e8236383a20872c0cdf5a62b554b27538db7fa1bbec52429d8d106effbaeca08",
-                "sha256:f04e857b59d9d1ccc39ce2da1021d196e47234873820cbeaad210724b1ee28ac",
-                "sha256:fadbfe37f74051d024037f223b8e001611eac868b5c5b06144ef4d8b799862f2"
-            ],
-            "markers": "python_version < '3.9'",
-            "version": "==0.2.1"
-        },
         "django": {
             "hashes": [
                 "sha256:45a747e1c5b3d6df1b141b1481e193b033fd1fdbda3ff52677dc81afdaacbaed",
                 "sha256:f7c7852a5ac5a3da5a8d5b35cc6168f31b605971441798dac845f17ca8028039"
             ],
             "index": "pypi",
             "version": "==4.2.3"
@@ -139,15 +117,15 @@
             "version": "==7.4.0"
         },
         "six": {
             "hashes": [
                 "sha256:1e61c37477a1626458e36f7b1d82aa5c9b094fa4802892072e49de9c60c4c926",
                 "sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254"
             ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
+            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2'",
             "version": "==1.16.0"
         },
         "sqlparse": {
             "hashes": [
                 "sha256:5430a4fe2ac7d0f93e66f1efc6e1338a41884b7ddf2a350cedd20ccc4d9d28f3",
                 "sha256:d446183e84b8349fa3061f0fe7f06ca94ba65b426946ffebe6e3e8295332420c"
             ],
@@ -202,15 +180,15 @@
             "version": "==0.2.0"
         },
         "decorator": {
             "hashes": [
                 "sha256:637996211036b6385ef91435e4fae22989472f9d571faba8927ba8253acbc330",
                 "sha256:b8c3f85900b9dc423225913c5aace94729fe1fa9763b38939a95226f02d37186"
             ],
-            "markers": "python_version < '3.11' and python_full_version >= '3.7.0'",
+            "markers": "python_version > '3.6' and python_version < '3.11'",
             "version": "==5.1.1"
         },
         "executing": {
             "hashes": [
                 "sha256:0314a69e37426e3608aada02473b4161d4caf5a4b244d1d0c48072b8fee7bacc",
                 "sha256:19da64c18d2d851112f09c287f8d3dbbdf725ab0e569077efb6cdcbd3497c107"
             ],
@@ -222,19 +200,19 @@
                 "sha256:e3ac6018ef05126d442af680aad863006ec19d02290561ac88b8b1c0b0cfc726"
             ],
             "index": "pypi",
             "version": "==0.13.13"
         },
         "ipython": {
             "hashes": [
-                "sha256:c7b80eb7f5a855a88efc971fda506ff7a91c280b42cdae26643e0f601ea281ea",
-                "sha256:ea8801f15dfe4ffb76dea1b09b847430ffd70d827b41735c64a0638a04103bfc"
+                "sha256:1d197b907b6ba441b692c48cf2a3a2de280dc0ac91a3405b39349a50272ca0a1",
+                "sha256:248aca623f5c99a6635bc3857677b7320b9b8039f99f070ee0d20a5ca5a8e6bf"
             ],
-            "markers": "python_version < '3.11' and python_full_version >= '3.7.0'",
-            "version": "==8.12.2"
+            "markers": "python_version > '3.6' and python_version < '3.11'",
+            "version": "==8.14.0"
         },
         "jedi": {
             "hashes": [
                 "sha256:203c1fd9d969ab8f2119ec0a3342e0b49910045abe6af0a3ae83a5764d54639e",
                 "sha256:bae794c30d07f6d910d32a7048af09b5a39ed740918da923c6b780790ebac612"
             ],
             "markers": "python_version >= '3.6'",
@@ -302,15 +280,15 @@
             "version": "==2.15.1"
         },
         "six": {
             "hashes": [
                 "sha256:1e61c37477a1626458e36f7b1d82aa5c9b094fa4802892072e49de9c60c4c926",
                 "sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254"
             ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
+            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2'",
             "version": "==1.16.0"
         },
         "stack-data": {
             "hashes": [
                 "sha256:32d2dd0376772d01b6cb9fc996f3c8b57a357089dec328ed4b6553d037eaf815",
                 "sha256:cbb2a53eb64e5785878201a97ed7c7b94883f48b87bfb0bbe8b623c74679e4a8"
             ],
@@ -328,22 +306,14 @@
             "hashes": [
                 "sha256:9e6ec080259b9a5940c797d58b613b5e31441c2257b87c2e795c5228ae80d2d8",
                 "sha256:f6cde21a9c68cf756af02035f72d5a723bf607e862e7be33ece505abf4a3bad9"
             ],
             "markers": "python_full_version >= '3.7.0'",
             "version": "==5.9.0"
         },
-        "typing-extensions": {
-            "hashes": [
-                "sha256:440d5dd3af93b060174bf433bccd69b0babc3b15b1a8dca43789fd7f61514b36",
-                "sha256:b75ddc264f0ba5615db7ba217daeb99701ad295353c45f9e95963337ceeeffb2"
-            ],
-            "markers": "python_version < '3.11'",
-            "version": "==4.7.1"
-        },
         "wcwidth": {
             "hashes": [
                 "sha256:795b138f6875577cd91bba52baf9e445cd5118fd32723b460e30a0af30ea230e",
                 "sha256:a5220780a404dbe3353789870978e472cfe477761f06ee55077256e509b156d0"
             ],
             "version": "==0.2.6"
         }
```

### Comparing `djgraphql-1.0.8/README.md` & `djgraphql-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `djgraphql-1.0.8/djgraphql/schema.py` & `djgraphql-1.1.0/djgraphql/schema.py`

 * *Files identical despite different names*

### Comparing `djgraphql-1.0.8/djgraphql/settings.py` & `djgraphql-1.1.0/djgraphql/settings.py`

 * *Files identical despite different names*

### Comparing `djgraphql-1.0.8/djgraphql/test/test_routers.py` & `djgraphql-1.1.0/djgraphql/test/test_routers.py`

 * *Files identical despite different names*

### Comparing `djgraphql-1.0.8/djgraphql/test/test_schema_generation.py` & `djgraphql-1.1.0/djgraphql/test/test_schema_generation.py`

 * *Files identical despite different names*

### Comparing `djgraphql-1.0.8/djgraphql/utils/routes.py` & `djgraphql-1.1.0/djgraphql/utils/routes.py`

 * *Files identical despite different names*

### Comparing `djgraphql-1.0.8/djgraphql.egg-info/PKG-INFO` & `djgraphql-1.1.0/djgraphql.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: djgraphql
-Version: 1.0.8
+Version: 1.1.0
 Summary: A package that makes easier to use graphql with django.
 Home-page: https://shitalluitel.com.np
 Author: Shital Babu Luitel
 Author-email: ctalluitel@gmail.com
 License: file: LICENSE.txt
 Description: file: README.md
 Platform: UNKNOWN
```

### Comparing `djgraphql-1.0.8/djgraphql.egg-info/SOURCES.txt` & `djgraphql-1.1.0/djgraphql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `djgraphql-1.0.8/setup.py` & `djgraphql-1.1.0/setup.py`

 * *Files identical despite different names*

