# Comparing `tmp/propertysync-0.6.0.tar.gz` & `tmp/propertysync-0.7.0.tar.gz`

## Comparing `propertysync-0.6.0.tar` & `propertysync-0.7.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1827 2020-02-02 00:00:00.000000 propertysync-0.6.0/CHANGELOG.md
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 propertysync-0.6.0/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 propertysync-0.6.0/.pytest_cache/README.md
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 propertysync-0.6.0/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 propertysync-0.6.0/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 propertysync-0.6.0/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 propertysync-0.6.0/propertysync/__about__.py
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 propertysync-0.6.0/propertysync/__init__.py
--rw-r--r--   0        0        0    16209 2020-02-02 00:00:00.000000 propertysync-0.6.0/propertysync/api.py
--rw-r--r--   0        0        0     4496 2020-02-02 00:00:00.000000 propertysync-0.6.0/propertysync/batch.py
--rw-r--r--   0        0        0     6720 2020-02-02 00:00:00.000000 propertysync-0.6.0/propertysync/document.py
--rw-r--r--   0        0        0     5786 2020-02-02 00:00:00.000000 propertysync-0.6.0/propertysync/search.py
--rw-r--r--   0        0        0    15944 2020-02-02 00:00:00.000000 propertysync-0.6.0/propertysync/titlesearch_batch.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 propertysync-0.6.0/tests/__init__.py
--rw-r--r--   0        0        0     4296 2020-02-02 00:00:00.000000 propertysync-0.6.0/tests/test_batch.py
--rw-r--r--   0        0        0     7397 2020-02-02 00:00:00.000000 propertysync-0.6.0/tests/test_document.py
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 propertysync-0.6.0/.gitignore
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 propertysync-0.6.0/LICENSE
--rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 propertysync-0.6.0/README.md
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 propertysync-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 propertysync-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     2371 2020-02-02 00:00:00.000000 propertysync-0.7.0/CHANGELOG.md
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 propertysync-0.7.0/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 propertysync-0.7.0/.pytest_cache/README.md
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 propertysync-0.7.0/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 propertysync-0.7.0/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 propertysync-0.7.0/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 propertysync-0.7.0/propertysync/__about__.py
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 propertysync-0.7.0/propertysync/__init__.py
+-rw-r--r--   0        0        0    17456 2020-02-02 00:00:00.000000 propertysync-0.7.0/propertysync/api.py
+-rw-r--r--   0        0        0     4496 2020-02-02 00:00:00.000000 propertysync-0.7.0/propertysync/batch.py
+-rw-r--r--   0        0        0     6720 2020-02-02 00:00:00.000000 propertysync-0.7.0/propertysync/document.py
+-rw-r--r--   0        0        0     5786 2020-02-02 00:00:00.000000 propertysync-0.7.0/propertysync/search.py
+-rw-r--r--   0        0        0    15944 2020-02-02 00:00:00.000000 propertysync-0.7.0/propertysync/titlesearch_batch.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 propertysync-0.7.0/tests/__init__.py
+-rw-r--r--   0        0        0     4296 2020-02-02 00:00:00.000000 propertysync-0.7.0/tests/test_batch.py
+-rw-r--r--   0        0        0     7397 2020-02-02 00:00:00.000000 propertysync-0.7.0/tests/test_document.py
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 propertysync-0.7.0/.gitignore
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 propertysync-0.7.0/LICENSE
+-rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 propertysync-0.7.0/README.md
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 propertysync-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 propertysync-0.7.0/PKG-INFO
```

### Comparing `propertysync-0.6.0/CHANGELOG.md` & `propertysync-0.7.0/CHANGELOG.md`

 * *Files 20% similar despite different names*

```diff
@@ -3,14 +3,22 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/)
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 Generated by [`auto-changelog`](https://github.com/CookPete/auto-changelog).
 
+## [v0.7.0](https://gitlab.com/propertysync/tools/python-api-client/compare/0.5.0...v0.7.0) - 2023-07-21
+
+### Commits
+
+- add validate_document method [`56c3ef9`](https://gitlab.com/propertysync/tools/python-api-client/commit/56c3ef94907cbebc4b24023d8af077acfb52e3dc)
+- auto-changelog [`490e736`](https://gitlab.com/propertysync/tools/python-api-client/commit/490e736661e73c38df6f51cc0b464511e6de3ae5)
+- changelog / versioning [`7e5338e`](https://gitlab.com/propertysync/tools/python-api-client/commit/7e5338edd842a38b7fd5ee6346f3e24dc6668eed)
+
 <!-- auto-changelog-above -->
 
 ## [0.5.0] - 2023-05-10
 
 ### Added
 - Lots of work to Batch and Document classes to support find and replace
 - Tests added for Batch and Document classes
```

### Comparing `propertysync-0.6.0/propertysync/api.py` & `propertysync-0.7.0/propertysync/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -364,16 +364,36 @@
     # run a document action on a batch
     def run_document_action(self, batch_id, action_id):
         url = f"{self.indexing_url}/document-groups/{self.document_group_id}/document-actions/{action_id}/execute"
         params = {
             "batchId":batch_id
         }
         return self.api_call("POST", url, params=params)
+    
+    # validate a document
+    def validate_document(self, document_json):
+        url = f"{self.indexing_url}/document-groups/{self.document_group_id}/documents/validate"
 
+        # if document_json contains an "id" key and no "json" key, it will validate the stored copy of the document
+        # if document_json contains a "json" key and no "id" key, it will validate the json
+        # if document_json contains a "json" key and no "id" key and the "json" contains a "indexingRecordId" key, it will validate the stored copy of the document
 
+        # if they are passing in "json", assume they want that validated and remove any ID keys
+        if "json" in document_json and "id" in document_json:
+            del document_json["id"]
+        if "json" in document_json and "indexingRecordId" in document_json["json"]:
+            del document_json["json"]["indexingRecordId"]
+
+        # if they are not passing in "json", assume they want the stored copy validated and ensure they have passed an ID
+        if "json" not in document_json and "id" not in document_json:
+            raise Exception("You must pass either an ID or JSON to validate a document")
+
+        return self.api_call("POST", url, body=document_json)
+        
+        
     # run a search, then create a batch and wait for the batch to fully hydrate, then retrieve the batch and optionally delete it
     def run_search_and_create_batch(self, search_query, minimum_results=1,wait_time=2,batch_name='python-api-client temp batch', delete_batch=True):
         search = self.run_search(search_query)
         search_id = search["id"]
 
         # if we don't have enough results in the search, throw an exception
         if search["count"] < minimum_results:
```

### Comparing `propertysync-0.6.0/propertysync/batch.py` & `propertysync-0.7.0/propertysync/batch.py`

 * *Files identical despite different names*

### Comparing `propertysync-0.6.0/propertysync/document.py` & `propertysync-0.7.0/propertysync/document.py`

 * *Files identical despite different names*

### Comparing `propertysync-0.6.0/propertysync/search.py` & `propertysync-0.7.0/propertysync/search.py`

 * *Files identical despite different names*

### Comparing `propertysync-0.6.0/propertysync/titlesearch_batch.py` & `propertysync-0.7.0/propertysync/titlesearch_batch.py`

 * *Files identical despite different names*

### Comparing `propertysync-0.6.0/tests/test_batch.py` & `propertysync-0.7.0/tests/test_batch.py`

 * *Files identical despite different names*

### Comparing `propertysync-0.6.0/tests/test_document.py` & `propertysync-0.7.0/tests/test_document.py`

 * *Files identical despite different names*

### Comparing `propertysync-0.6.0/LICENSE` & `propertysync-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `propertysync-0.6.0/README.md` & `propertysync-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `propertysync-0.6.0/pyproject.toml` & `propertysync-0.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `propertysync-0.6.0/PKG-INFO` & `propertysync-0.7.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: propertysync
-Version: 0.6.0
+Version: 0.7.0
 Summary: A package for interacting with the PropertySync API.
 Project-URL: Documentation, https://developer.propertysync.com/python/index.html
 Author-email: Rob Martinson <rob@limelyte.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
```

