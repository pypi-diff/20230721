# Comparing `tmp/montydb-2.5.0.tar.gz` & `tmp/montydb-2.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "montydb-2.5.0.tar", max compression
+gzip compressed data, was "montydb-2.5.1.tar", max compression
```

## Comparing `montydb-2.5.0.tar` & `montydb-2.5.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     1509 2023-02-03 21:46:00.998909 montydb-2.5.0/LICENSE
--rw-r--r--   0        0        0     9398 2023-02-03 21:46:00.998909 montydb-2.5.0/README.md
--rw-r--r--   0        0        0      670 2023-02-03 21:46:01.002909 montydb-2.5.0/montydb/__init__.py
--rw-r--r--   0        0        0      171 2023-02-03 21:46:42.539161 montydb-2.5.0/montydb/_version.py
--rw-r--r--   0        0        0     8649 2023-02-03 21:46:01.002909 montydb-2.5.0/montydb/base.py
--rw-r--r--   0        0        0     5244 2023-02-03 21:46:01.002909 montydb-2.5.0/montydb/client.py
--rw-r--r--   0        0        0    14594 2023-02-03 21:46:01.002909 montydb-2.5.0/montydb/collection.py
--rw-r--r--   0        0        0     9158 2023-02-03 21:46:01.002909 montydb-2.5.0/montydb/configure.py
--rw-r--r--   0        0        0    12501 2023-02-03 21:46:01.002909 montydb-2.5.0/montydb/cursor.py
--rw-r--r--   0        0        0     3276 2023-02-03 21:46:01.002909 montydb-2.5.0/montydb/database.py
--rw-r--r--   0        0        0        0 2023-02-03 21:46:01.002909 montydb-2.5.0/montydb/engine/__init__.py
--rw-r--r--   0        0        0    26194 2023-02-03 21:46:01.002909 montydb-2.5.0/montydb/engine/field_walker.py
--rw-r--r--   0        0        0    15567 2023-02-03 21:46:01.002909 montydb-2.5.0/montydb/engine/project.py
--rw-r--r--   0        0        0    28169 2023-02-03 21:46:01.002909 montydb-2.5.0/montydb/engine/queries.py
--rw-r--r--   0        0        0    24518 2023-02-03 21:46:01.002909 montydb-2.5.0/montydb/engine/update.py
--rw-r--r--   0        0        0     5293 2023-02-03 21:46:01.002909 montydb-2.5.0/montydb/engine/weighted.py
--rw-r--r--   0        0        0     1988 2023-02-03 21:46:01.002909 montydb-2.5.0/montydb/errors.py
--rw-r--r--   0        0        0     6302 2023-02-03 21:46:01.002909 montydb-2.5.0/montydb/results.py
--rw-r--r--   0        0        0     6134 2023-02-03 21:46:01.002909 montydb-2.5.0/montydb/storage/__init__.py
--rw-r--r--   0        0        0     8145 2023-02-03 21:46:01.002909 montydb-2.5.0/montydb/storage/flatfile.py
--rw-r--r--   0        0        0     7043 2023-02-03 21:46:01.002909 montydb-2.5.0/montydb/storage/lightning.py
--rw-r--r--   0        0        0     3861 2023-02-03 21:46:01.002909 montydb-2.5.0/montydb/storage/memory.py
--rw-r--r--   0        0        0    11920 2023-02-03 21:46:01.002909 montydb-2.5.0/montydb/storage/sqlite.py
--rw-r--r--   0        0        0      997 2023-02-03 21:46:01.002909 montydb-2.5.0/montydb/types/__init__.py
--rw-r--r--   0        0        0     2174 2023-02-03 21:46:01.002909 montydb-2.5.0/montydb/types/_bson.py
--rw-r--r--   0        0        0     7913 2023-02-03 21:46:01.002909 montydb-2.5.0/montydb/types/_nobson.py
--rw-r--r--   0        0        0     1729 2023-02-03 21:46:01.002909 montydb-2.5.0/montydb/types/bson.py
--rw-r--r--   0        0        0     1094 2023-02-03 21:46:01.002909 montydb-2.5.0/montydb/types/compat.py
--rw-r--r--   0        0        0     5484 2023-02-03 21:46:01.002909 montydb-2.5.0/montydb/types/helper.py
--rw-r--r--   0        0        0    10077 2023-02-03 21:46:01.002909 montydb-2.5.0/montydb/types/objectid.py
--rw-r--r--   0        0        0     1518 2023-02-03 21:46:01.002909 montydb-2.5.0/montydb/types/tz_util.py
--rw-r--r--   0        0        0      278 2023-02-03 21:46:01.002909 montydb-2.5.0/montydb/utils/__init__.py
--rw-r--r--   0        0        0    10678 2023-02-03 21:46:01.002909 montydb-2.5.0/montydb/utils/io.py
--rw-r--r--   0        0        0     4006 2023-02-03 21:46:01.002909 montydb-2.5.0/montydb/utils/mt_list.py
--rw-r--r--   0        0        0     1323 2023-02-03 21:46:42.539161 montydb-2.5.0/pyproject.toml
--rw-r--r--   0        0        0    10440 1970-01-01 00:00:00.000000 montydb-2.5.0/setup.py
--rw-r--r--   0        0        0    10712 1970-01-01 00:00:00.000000 montydb-2.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1509 2023-07-21 18:37:02.116268 montydb-2.5.1/LICENSE
+-rw-r--r--   0        0        0     9398 2023-07-21 18:37:02.116268 montydb-2.5.1/README.md
+-rw-r--r--   0        0        0      670 2023-07-21 18:37:02.120268 montydb-2.5.1/montydb/__init__.py
+-rw-r--r--   0        0        0      171 2023-07-21 18:37:51.440341 montydb-2.5.1/montydb/_version.py
+-rw-r--r--   0        0        0     8649 2023-07-21 18:37:02.120268 montydb-2.5.1/montydb/base.py
+-rw-r--r--   0        0        0     5244 2023-07-21 18:37:02.120268 montydb-2.5.1/montydb/client.py
+-rw-r--r--   0        0        0    14594 2023-07-21 18:37:02.120268 montydb-2.5.1/montydb/collection.py
+-rw-r--r--   0        0        0     9395 2023-07-21 18:37:02.120268 montydb-2.5.1/montydb/configure.py
+-rw-r--r--   0        0        0    12501 2023-07-21 18:37:02.120268 montydb-2.5.1/montydb/cursor.py
+-rw-r--r--   0        0        0     3276 2023-07-21 18:37:02.120268 montydb-2.5.1/montydb/database.py
+-rw-r--r--   0        0        0        0 2023-07-21 18:37:02.120268 montydb-2.5.1/montydb/engine/__init__.py
+-rw-r--r--   0        0        0    26194 2023-07-21 18:37:02.120268 montydb-2.5.1/montydb/engine/field_walker.py
+-rw-r--r--   0        0        0    15567 2023-07-21 18:37:02.120268 montydb-2.5.1/montydb/engine/project.py
+-rw-r--r--   0        0        0    28330 2023-07-21 18:37:02.120268 montydb-2.5.1/montydb/engine/queries.py
+-rw-r--r--   0        0        0    24518 2023-07-21 18:37:02.120268 montydb-2.5.1/montydb/engine/update.py
+-rw-r--r--   0        0        0     5293 2023-07-21 18:37:02.120268 montydb-2.5.1/montydb/engine/weighted.py
+-rw-r--r--   0        0        0     1988 2023-07-21 18:37:02.120268 montydb-2.5.1/montydb/errors.py
+-rw-r--r--   0        0        0     6302 2023-07-21 18:37:02.120268 montydb-2.5.1/montydb/results.py
+-rw-r--r--   0        0        0     6134 2023-07-21 18:37:02.124268 montydb-2.5.1/montydb/storage/__init__.py
+-rw-r--r--   0        0        0     8145 2023-07-21 18:37:02.124268 montydb-2.5.1/montydb/storage/flatfile.py
+-rw-r--r--   0        0        0     7043 2023-07-21 18:37:02.124268 montydb-2.5.1/montydb/storage/lightning.py
+-rw-r--r--   0        0        0     3861 2023-07-21 18:37:02.124268 montydb-2.5.1/montydb/storage/memory.py
+-rw-r--r--   0        0        0    11920 2023-07-21 18:37:02.124268 montydb-2.5.1/montydb/storage/sqlite.py
+-rw-r--r--   0        0        0      997 2023-07-21 18:37:02.124268 montydb-2.5.1/montydb/types/__init__.py
+-rw-r--r--   0        0        0     2174 2023-07-21 18:37:02.124268 montydb-2.5.1/montydb/types/_bson.py
+-rw-r--r--   0        0        0     7913 2023-07-21 18:37:02.124268 montydb-2.5.1/montydb/types/_nobson.py
+-rw-r--r--   0        0        0     1729 2023-07-21 18:37:02.124268 montydb-2.5.1/montydb/types/bson.py
+-rw-r--r--   0        0        0     1094 2023-07-21 18:37:02.124268 montydb-2.5.1/montydb/types/compat.py
+-rw-r--r--   0        0        0     5484 2023-07-21 18:37:02.124268 montydb-2.5.1/montydb/types/helper.py
+-rw-r--r--   0        0        0    10077 2023-07-21 18:37:02.124268 montydb-2.5.1/montydb/types/objectid.py
+-rw-r--r--   0        0        0     1518 2023-07-21 18:37:02.124268 montydb-2.5.1/montydb/types/tz_util.py
+-rw-r--r--   0        0        0      278 2023-07-21 18:37:02.124268 montydb-2.5.1/montydb/utils/__init__.py
+-rw-r--r--   0        0        0    10678 2023-07-21 18:37:02.124268 montydb-2.5.1/montydb/utils/io.py
+-rw-r--r--   0        0        0     4006 2023-07-21 18:37:02.124268 montydb-2.5.1/montydb/utils/mt_list.py
+-rw-r--r--   0        0        0     1323 2023-07-21 18:37:51.440341 montydb-2.5.1/pyproject.toml
+-rw-r--r--   0        0        0    10440 1970-01-01 00:00:00.000000 montydb-2.5.1/setup.py
+-rw-r--r--   0        0        0    10712 1970-01-01 00:00:00.000000 montydb-2.5.1/PKG-INFO
```

### Comparing `montydb-2.5.0/LICENSE` & `montydb-2.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `montydb-2.5.0/README.md` & `montydb-2.5.1/README.md`

 * *Files identical despite different names*

### Comparing `montydb-2.5.0/montydb/__init__.py` & `montydb-2.5.1/montydb/__init__.py`

 * *Files identical despite different names*

### Comparing `montydb-2.5.0/montydb/base.py` & `montydb-2.5.1/montydb/base.py`

 * *Files identical despite different names*

### Comparing `montydb-2.5.0/montydb/client.py` & `montydb-2.5.1/montydb/client.py`

 * *Files identical despite different names*

### Comparing `montydb-2.5.0/montydb/collection.py` & `montydb-2.5.1/montydb/collection.py`

 * *Files identical despite different names*

### Comparing `montydb-2.5.0/montydb/configure.py` & `montydb-2.5.1/montydb/configure.py`

 * *Files 6% similar despite different names*

```diff
@@ -306,17 +306,20 @@
         patch(queries, "_regex_options_check", "_regex_options_")
         patch(queries, "_mod_remainder_not_num", "_mod_remainder_not_num_")
 
     elif version == "4.0":
         patch(queries, "_is_comparable", "_is_comparable_ver4")
         patch(queries, "_regex_options_check", "_regex_options_")
         patch(queries, "_mod_remainder_not_num", "_mod_remainder_not_num_")
+        patch(queries, "_not_subspec_op_check", "_not_validate_subspec_op_v4")
 
     elif version == "4.2":
         patch(queries, "_is_comparable", "_is_comparable_ver4")
         patch(queries, "_regex_options_check", "_regex_options_v42")
         patch(queries, "_mod_remainder_not_num", "_mod_remainder_not_num_v42")
+        patch(queries, "_not_subspec_op_check", "_not_validate_subspec_op_v4")
 
     else:
         patch(queries, "_is_comparable", "_is_comparable_ver4")
         patch(queries, "_regex_options_check", "_regex_options_")
         patch(queries, "_mod_remainder_not_num", "_mod_remainder_not_num_v42")
+        patch(queries, "_not_subspec_op_check", "_not_validate_subspec_op_v4")
```

### Comparing `montydb-2.5.0/montydb/cursor.py` & `montydb-2.5.1/montydb/cursor.py`

 * *Files identical despite different names*

### Comparing `montydb-2.5.0/montydb/database.py` & `montydb-2.5.1/montydb/database.py`

 * *Files identical despite different names*

### Comparing `montydb-2.5.0/montydb/engine/field_walker.py` & `montydb-2.5.1/montydb/engine/field_walker.py`

 * *Files identical despite different names*

### Comparing `montydb-2.5.0/montydb/engine/project.py` & `montydb-2.5.1/montydb/engine/project.py`

 * *Files identical despite different names*

### Comparing `montydb-2.5.0/montydb/engine/queries.py` & `montydb-2.5.1/montydb/engine/queries.py`

 * *Files 2% similar despite different names*

```diff
@@ -373,16 +373,15 @@
         if isinstance(sub_spec, (RE_PATTERN_TYPE, bson.Regex)):
             return self.subparser("$not", {"$regex": sub_spec})
 
         elif is_duckument_type(sub_spec):
             for op in sub_spec:
                 if op not in self.field_ops:
                     raise OperationFailure("unknown operator: {}".format(op))
-                if op == "$regex":
-                    raise OperationFailure("$not cannot have a regex")
+                _not_subspec_op_check(op)
 
             return self.subparser("$not", sub_spec)
 
         else:
             raise OperationFailure("$not needs a regex or a document")
 
     def _parse_elemMatch(self, sub_spec):
@@ -399,14 +398,26 @@
                 raise OperationFailure("unknown operator: {}".format(op))
 
 
 def _is_expression_obj(sub_spec):
     return is_duckument_type(sub_spec) and next(iter(sub_spec)).startswith("$")
 
 
+def _not_validate_subspec_op_(op):
+    if op == "$regex":
+        raise OperationFailure("$not cannot have a regex")
+
+
+def _not_validate_subspec_op_v4(sub_spec):
+    pass
+
+
+_not_subspec_op_check = _not_validate_subspec_op_
+
+
 # Only for preserving `int` type flags to bypass
 # internal "flags must be string" type check
 class _FALG(object):
     def __init__(self, int_flags):
         self.retrieve = int_flags
 
     __slots__ = ("retrieve",)
```

### Comparing `montydb-2.5.0/montydb/engine/update.py` & `montydb-2.5.1/montydb/engine/update.py`

 * *Files identical despite different names*

### Comparing `montydb-2.5.0/montydb/engine/weighted.py` & `montydb-2.5.1/montydb/engine/weighted.py`

 * *Files identical despite different names*

### Comparing `montydb-2.5.0/montydb/errors.py` & `montydb-2.5.1/montydb/errors.py`

 * *Files identical despite different names*

### Comparing `montydb-2.5.0/montydb/results.py` & `montydb-2.5.1/montydb/results.py`

 * *Files identical despite different names*

### Comparing `montydb-2.5.0/montydb/storage/__init__.py` & `montydb-2.5.1/montydb/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `montydb-2.5.0/montydb/storage/flatfile.py` & `montydb-2.5.1/montydb/storage/flatfile.py`

 * *Files identical despite different names*

### Comparing `montydb-2.5.0/montydb/storage/lightning.py` & `montydb-2.5.1/montydb/storage/lightning.py`

 * *Files identical despite different names*

### Comparing `montydb-2.5.0/montydb/storage/memory.py` & `montydb-2.5.1/montydb/storage/memory.py`

 * *Files identical despite different names*

### Comparing `montydb-2.5.0/montydb/storage/sqlite.py` & `montydb-2.5.1/montydb/storage/sqlite.py`

 * *Files identical despite different names*

### Comparing `montydb-2.5.0/montydb/types/__init__.py` & `montydb-2.5.1/montydb/types/__init__.py`

 * *Files identical despite different names*

### Comparing `montydb-2.5.0/montydb/types/_bson.py` & `montydb-2.5.1/montydb/types/_bson.py`

 * *Files identical despite different names*

### Comparing `montydb-2.5.0/montydb/types/_nobson.py` & `montydb-2.5.1/montydb/types/_nobson.py`

 * *Files identical despite different names*

### Comparing `montydb-2.5.0/montydb/types/bson.py` & `montydb-2.5.1/montydb/types/bson.py`

 * *Files identical despite different names*

### Comparing `montydb-2.5.0/montydb/types/compat.py` & `montydb-2.5.1/montydb/types/compat.py`

 * *Files identical despite different names*

### Comparing `montydb-2.5.0/montydb/types/helper.py` & `montydb-2.5.1/montydb/types/helper.py`

 * *Files identical despite different names*

### Comparing `montydb-2.5.0/montydb/types/objectid.py` & `montydb-2.5.1/montydb/types/objectid.py`

 * *Files identical despite different names*

### Comparing `montydb-2.5.0/montydb/types/tz_util.py` & `montydb-2.5.1/montydb/types/tz_util.py`

 * *Files identical despite different names*

### Comparing `montydb-2.5.0/montydb/utils/io.py` & `montydb-2.5.1/montydb/utils/io.py`

 * *Files identical despite different names*

### Comparing `montydb-2.5.0/montydb/utils/mt_list.py` & `montydb-2.5.1/montydb/utils/mt_list.py`

 * *Files identical despite different names*

### Comparing `montydb-2.5.0/pyproject.toml` & `montydb-2.5.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "montydb"
-version = "2.5.0"
+version = "2.5.1"
 description = "Monty, Mongo tinified. MongoDB implemented in Python !"
 authors = ["davidlatwe <davidlatwe@gmail.com>"]
 license = "BSD-3-Clause License"
 readme = "README.md"
 repository = "https://github.com/davidlatwe/montydb"
 keywords = ["monty", "montydb", "pymongo", "mongodb", "database", "embedded"]
 classifiers = [
```

### Comparing `montydb-2.5.0/setup.py` & `montydb-2.5.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
  'montydb.utils']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'montydb',
-    'version': '2.5.0',
+    'version': '2.5.1',
     'description': 'Monty, Mongo tinified. MongoDB implemented in Python !',
     'long_description': '\n<img src="artwork/logo.png" alt="drawing" width="600"/>\n\n[![Python package](https://github.com/davidlatwe/montydb/actions/workflows/python-package.yml/badge.svg)](https://github.com/davidlatwe/montydb/actions/workflows/python-package.yml)\n[![Version](http://img.shields.io/pypi/v/montydb.svg?style=flat)](https://pypi.python.org/pypi/montydb)\n[![PyPi downloads](https://img.shields.io/pypi/dm/montydb)](https://pypistats.org/packages/montydb)\n\n> Monty, Mongo tinified. MongoDB implemented in Python!\n\n_Inspired by [TinyDB](https://github.com/msiemens/tinydb) and it\'s extension [TinyMongo](https://github.com/schapman1974/tinymongo)_\n\n\n## What is it?\n\nA pure Python-implemented database that looks and works like [MongoDB](https://www.mongodb.com/).\n\n```python\n>>> from montydb import MontyClient\n\n>>> col = MontyClient(":memory:").db.test\n>>> col.insert_many( [{"stock": "A", "qty": 6}, {"stock": "A", "qty": 2}] )\n>>> cur = col.find( {"stock": "A", "qty": {"$gt": 4}} )\n>>> next(cur)\n{\'_id\': ObjectId(\'5ad34e537e8dd45d9c61a456\'), \'stock\': \'A\', \'qty\': 6}\n```\n\nMost of the CRUD operators have been implemented. You can visit [issue #14](https://github.com/davidlatwe/montydb/issues/14) to see the full list.\n\nThis project is tested against:\n\n- MongoDB: 3.6, 4.0, 4.2 (4.4 on the way💦)\n- Python: 3.7, 3.8, 3.9, 3.10, 3.11\n\n\n## Install\n\n```sh\npip install montydb\n```\n\n- optional, to use *real* `bson` in operation (`pymongo` will be installed)\n    _For minimum requirements, `montydb` ships with it\'s own fork of `ObjectId` in `montydb.types`, so you may ignore this option if `ObjectId` is all you need from `bson`_\n\n    ```sh\n    pip install montydb[bson]\n    ```\n- optional, to use lightning memory-mapped db as storage engine\n    ```sh\n    pip install montydb[lmdb]\n    ```\n\n\n## Storage\n\n🦄 Available storage engines:\n\n* in-memory\n* flat-file\n* sqlite\n* lmdb (lightning memory-mapped db)\n\nDepending on which one you use, you may have to configure the storage engine before you start.\n\n> ⚠️\n>\n> The configuration process only required on repository creation or modification. And, one repository (the parent level of databases) can only assign one storage engine.\n\nTo configure a storage, see flat-file storage for example:\n\n```python\nfrom montydb import set_storage, MontyClient\n\n\nset_storage(\n    # general settings\n    \n    repository="/db/repo",  # dir path for database to live on disk, default is {cwd}\n    storage="flatfile",     # storage name, default "flatfile"\n    mongo_version="4.0",    # try matching behavior with this mongodb version\n    use_bson=False,         # default None, and will import pymongo\'s bson if None or True\n\n    # any other kwargs are storage engine settings.\n    \n    cache_modified=10,       # the only setting that flat-file have\n)\n\n# ready to go\n```\n\nOnce that done, there should be a file named `monty.storage.cfg` saved in your db repository path. It would be `/db/repo` for the above examples.\n\n\n## Configuration\n\nNow let\'s moving on to each storage engine\'s config settings.\n\n### 🌟 In-Memory\n  \n`memory` storage does not need nor have any configuration, nothing saved to disk.\n\n```python\nfrom montydb import MontyClient\n\n\nclient = MontyClient(":memory:")\n\n# ready to go\n```\n\n### 🔰 Flat-File\n  \n`flatfile` is the default on-disk storage engine.\n\n```python\nfrom montydb import set_storage, MontyClient\n\n\nset_storage("/db/repo", cache_modified=5)  # optional step\nclient = MontyClient("/db/repo")  # use current working dir if no path given\n\n# ready to go\n```\n\nFlatFile config:\n\n```ini\n[flatfile]\ncache_modified: 0  # how many document CRUD cached before flush to disk.\n```\n\n### 💎 SQLite\n  \n`sqlite` is NOT the default on-disk storage, need configuration first before getting client.\n\n> Pre-existing sqlite storage file which saved by `montydb<=1.3.0` is not read/writeable after `montydb==2.0.0`.\n\n```python\nfrom montydb import set_storage, MontyClient\n\n\nset_storage("/db/repo", storage="sqlite")  # required, to set sqlite as engine\nclient = MontyClient("/db/repo")\n\n# ready to go\n```\n\nSQLite config:\n\n```ini\n[sqlite]\njournal_mode: WAL\n```\n\nSQLite write concern:\n\n```python\nclient = MontyClient("/db/repo",\n                     synchronous=1,\n                     automatic_index=False,\n                     busy_timeout=5000)\n```\n\n### 🚀 LMDB (Lightning Memory-Mapped Database)\n\n`lightning` is NOT the default on-disk storage, need configuration first before get client.\n\n> Newly implemented.\n\n```python\nfrom montydb import set_storage, MontyClient\n\n\nset_storage("/db/repo", storage="lightning")  # required, to set lightning as engine\nclient = MontyClient("/db/repo")\n\n# ready to go\n```\n\nLMDB config:\n\n```ini\n[lightning]\nmap_size: 10485760  # Maximum size database may grow to.\n```\n\n## URI\n\nOptionally, You could prefix the repository path with montydb URI scheme.\n\n```python\nclient = MontyClient("montydb:///db/repo")\n```\n\n## Utilities\n\n> Pymongo `bson` may required.\n\n* #### `montyimport`\n\n  Imports content from an Extended JSON file into a MontyCollection instance.\n  The JSON file could be generated from `montyexport` or `mongoexport`.\n\n  ```python\n  from montydb import open_repo, utils\n  \n\n  with open_repo("foo/bar"):\n      utils.montyimport("db", "col", "/path/dump.json")\n  \n  ```\n\n* #### `montyexport`\n\n  Produces a JSON export of data stored in a MontyCollection instance.\n  The JSON file could be loaded by `montyimport` or `mongoimport`.\n\n  ```python\n  from montydb import open_repo, utils\n  \n\n  with open_repo("foo/bar"):\n      utils.montyexport("db", "col", "/data/dump.json")\n  \n  ```\n\n* #### `montyrestore`\n\n  Loads a binary database dump into a MontyCollection instance.\n  The BSON file could be generated from `montydump` or `mongodump`.\n\n  ```python\n  from montydb import open_repo, utils\n  \n\n  with open_repo("foo/bar"):\n      utils.montyrestore("db", "col", "/path/dump.bson")\n  \n  ```\n\n* ####  `montydump`\n\n  Creates a binary export from a MontyCollection instance.\n  The BSON file could be loaded by `montyrestore` or `mongorestore`.\n\n  ```python\n  from montydb import open_repo, utils\n  \n\n  with open_repo("foo/bar"):\n      utils.montydump("db", "col", "/data/dump.bson")\n  \n  ```\n\n* #### `MongoQueryRecorder`\n\n  Record MongoDB query results in a period of time.\n  *Requires to access database profiler.*\n\n  This works via filtering the database profile data and reproduce the queries of `find` and `distinct` commands.\n\n  ```python\n  from pymongo import MongoClient\n  from montydb.utils import MongoQueryRecorder\n  \n  client = MongoClient()\n  recorder = MongoQueryRecorder(client["mydb"])\n  recorder.start()\n  \n  # Make some queries or run the App...\n  recorder.stop()\n  recorder.extract()\n  {<collection_1>: [<doc_1>, <doc_2>, ...], ...}\n  \n  ```\n\n* ####  `MontyList`\n\n  Experimental, a subclass of `list`, combined the common CRUD methods from Mongo\'s Collection and Cursor.\n\n  ```python\n  from montydb.utils import MontyList\n  \n  mtl = MontyList([1, 2, {"a": 1}, {"a": 5}, {"a": 8}])\n  mtl.find({"a": {"$gt": 3}})\n  MontyList([{\'a\': 5}, {\'a\': 8}])\n  \n  ```\n\n## Development\n\nmontydb uses [Poetry](https://python-poetry.org/) to make it easy manage dependencies and set up the development environment. \n\n### Initial setup\n\nAfter cloning the repository, you need to run the following commands to set up the development environment:\n\n```bash\nmake install\n```\n\nThis will create a virtual environment and download the required dependencies.\n\n### updating dependencies\n\nTo keep dependencies updated after git operations such as local updates or merging changes into local dev branch\n\n```bash\nmake update\n```\n### Makefile\n\nA makefile is used to simplify common operations such as updating, testing, and deploying etc.\n\n```bash\nmake or make help\n\ninstall                        install all dependencies locally\nupdate                         update project dependencies locally (run after git update)\nci                             Run all checks (codespell, lint, bandit, test)\ntest                           Run tests\nlint                           Run linting with flake8\ncodespell                      Find typos with codespell\nbandit                         Run static security analysis with bandit\nbuild                          Build project using poetry\nclean                          Clean project\n```\n\n### Run mongo docker image\nMost of our tests compare montydb CRUD results against real mongodb instance, therefore we must have a running\nmongodb before testing.\n\nFor example, if we want to test against mongo 4.4:\n```shell\ndocker run --name monty-4.4 -p 30044:27017 -d mongo:4.4\n```\n\n### Tests\n```shell\npoetry run pytest --storage {storage engin name} --mongodb {mongo instance url} [--use-bson]\n```\nExample:\n```shell\npoetry run pytest --storage memory --mongodb localhost:30044 --use-bson\n```\n\n## Why did I make this?\n\nMainly for personal skill practicing and fun.\n\nI work in the VFX industry and some of my production needs (mostly edge-case) requires to run in a limited environment (e.g. outsourced render farms), which may have problem to run or connect a MongoDB instance. And I found this project really helps.\n\n---\n\n<p align=center>\n    <a href="https://jb.gg/OpenSource"><i>This project is supported by JetBrains</i></a>\n</p>\n\n<p align="center">\n    <img src="artwork/icon.png" alt="drawing" width="100"/>\n  &nbsp;&nbsp;\n    <img src="artwork/jetbrains.png" alt="drawing" width="100"/>\n</p>\n',
     'author': 'davidlatwe',
     'author_email': 'davidlatwe@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/davidlatwe/montydb',
```

### Comparing `montydb-2.5.0/PKG-INFO` & `montydb-2.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: montydb
-Version: 2.5.0
+Version: 2.5.1
 Summary: Monty, Mongo tinified. MongoDB implemented in Python !
 Home-page: https://github.com/davidlatwe/montydb
 License: BSD-3-Clause License
 Keywords: monty,montydb,pymongo,mongodb,database,embedded
 Author: davidlatwe
 Author-email: davidlatwe@gmail.com
 Requires-Python: >=3.7,<3.12
```

