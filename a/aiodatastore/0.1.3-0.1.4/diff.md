# Comparing `tmp/aiodatastore-0.1.3.tar.gz` & `tmp/aiodatastore-0.1.4.tar.gz`

## Comparing `aiodatastore-0.1.3.tar` & `aiodatastore-0.1.4.tar`

### file list

```diff
@@ -1,39 +1,38 @@
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 aiodatastore-0.1.3/.flake8
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 aiodatastore-0.1.3/CHANGELOG.md
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 aiodatastore-0.1.3/Makefile
--rw-r--r--   0        0        0     2345 2020-02-02 00:00:00.000000 aiodatastore-0.1.3/credentials.json
--rw-r--r--   0        0        0     8146 2020-02-02 00:00:00.000000 aiodatastore-0.1.3/main.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 aiodatastore-0.1.3/requirements.txt
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 aiodatastore-0.1.3/.github/workflows/lint.yml
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 aiodatastore-0.1.3/.github/workflows/test.yml
--rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 aiodatastore-0.1.3/aiodatastore/__init__.py
--rw-r--r--   0        0        0     7864 2020-02-02 00:00:00.000000 aiodatastore-0.1.3/aiodatastore/client.py
--rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 aiodatastore-0.1.3/aiodatastore/commit.py
--rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 aiodatastore-0.1.3/aiodatastore/constants.py
--rw-r--r--   0        0        0     2853 2020-02-02 00:00:00.000000 aiodatastore-0.1.3/aiodatastore/entity.py
--rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 aiodatastore-0.1.3/aiodatastore/filters.py
--rw-r--r--   0        0        0     2950 2020-02-02 00:00:00.000000 aiodatastore-0.1.3/aiodatastore/key.py
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 aiodatastore-0.1.3/aiodatastore/lookup.py
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 aiodatastore-0.1.3/aiodatastore/mutation.py
--rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 aiodatastore-0.1.3/aiodatastore/property.py
--rw-r--r--   0        0        0     7337 2020-02-02 00:00:00.000000 aiodatastore-0.1.3/aiodatastore/query.py
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 aiodatastore-0.1.3/aiodatastore/transaction.py
--rw-r--r--   0        0        0     5546 2020-02-02 00:00:00.000000 aiodatastore-0.1.3/aiodatastore/values.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aiodatastore-0.1.3/tests/integration/test_client.py
--rw-r--r--   0        0        0     3774 2020-02-02 00:00:00.000000 aiodatastore-0.1.3/tests/integration/test_values.py
--rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 aiodatastore-0.1.3/tests/unit/test_client.py
--rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 aiodatastore-0.1.3/tests/unit/test_commit.py
--rw-r--r--   0        0        0     4043 2020-02-02 00:00:00.000000 aiodatastore-0.1.3/tests/unit/test_entity.py
--rw-r--r--   0        0        0     2426 2020-02-02 00:00:00.000000 aiodatastore-0.1.3/tests/unit/test_filters.py
--rw-r--r--   0        0        0     4621 2020-02-02 00:00:00.000000 aiodatastore-0.1.3/tests/unit/test_key.py
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 aiodatastore-0.1.3/tests/unit/test_lookup.py
--rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 aiodatastore-0.1.3/tests/unit/test_mutation.py
--rw-r--r--   0        0        0     2409 2020-02-02 00:00:00.000000 aiodatastore-0.1.3/tests/unit/test_property.py
--rw-r--r--   0        0        0     7752 2020-02-02 00:00:00.000000 aiodatastore-0.1.3/tests/unit/test_query.py
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 aiodatastore-0.1.3/tests/unit/test_transaction.py
--rw-r--r--   0        0        0    21543 2020-02-02 00:00:00.000000 aiodatastore-0.1.3/tests/unit/test_values.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 aiodatastore-0.1.3/.gitignore
--rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 aiodatastore-0.1.3/LICENSE
--rw-r--r--   0        0        0     5479 2020-02-02 00:00:00.000000 aiodatastore-0.1.3/README.md
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 aiodatastore-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     6499 2020-02-02 00:00:00.000000 aiodatastore-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 aiodatastore-0.1.4/.flake8
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 aiodatastore-0.1.4/CHANGELOG.md
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 aiodatastore-0.1.4/Makefile
+-rw-r--r--   0        0        0     2345 2020-02-02 00:00:00.000000 aiodatastore-0.1.4/credentials.json
+-rw-r--r--   0        0        0     8146 2020-02-02 00:00:00.000000 aiodatastore-0.1.4/main.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 aiodatastore-0.1.4/requirements.txt
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 aiodatastore-0.1.4/.github/workflows/lint.yml
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 aiodatastore-0.1.4/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 aiodatastore-0.1.4/aiodatastore/__init__.py
+-rw-r--r--   0        0        0     7864 2020-02-02 00:00:00.000000 aiodatastore-0.1.4/aiodatastore/client.py
+-rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 aiodatastore-0.1.4/aiodatastore/commit.py
+-rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 aiodatastore-0.1.4/aiodatastore/constants.py
+-rw-r--r--   0        0        0     2853 2020-02-02 00:00:00.000000 aiodatastore-0.1.4/aiodatastore/entity.py
+-rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 aiodatastore-0.1.4/aiodatastore/filters.py
+-rw-r--r--   0        0        0     2950 2020-02-02 00:00:00.000000 aiodatastore-0.1.4/aiodatastore/key.py
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 aiodatastore-0.1.4/aiodatastore/lookup.py
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 aiodatastore-0.1.4/aiodatastore/mutation.py
+-rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 aiodatastore-0.1.4/aiodatastore/property.py
+-rw-r--r--   0        0        0     7337 2020-02-02 00:00:00.000000 aiodatastore-0.1.4/aiodatastore/query.py
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 aiodatastore-0.1.4/aiodatastore/transaction.py
+-rw-r--r--   0        0        0     5546 2020-02-02 00:00:00.000000 aiodatastore-0.1.4/aiodatastore/values.py
+-rw-r--r--   0        0        0     3774 2020-02-02 00:00:00.000000 aiodatastore-0.1.4/tests/integration/test_values.py
+-rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 aiodatastore-0.1.4/tests/unit/test_client.py
+-rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 aiodatastore-0.1.4/tests/unit/test_commit.py
+-rw-r--r--   0        0        0     4043 2020-02-02 00:00:00.000000 aiodatastore-0.1.4/tests/unit/test_entity.py
+-rw-r--r--   0        0        0     2426 2020-02-02 00:00:00.000000 aiodatastore-0.1.4/tests/unit/test_filters.py
+-rw-r--r--   0        0        0     4621 2020-02-02 00:00:00.000000 aiodatastore-0.1.4/tests/unit/test_key.py
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 aiodatastore-0.1.4/tests/unit/test_lookup.py
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 aiodatastore-0.1.4/tests/unit/test_mutation.py
+-rw-r--r--   0        0        0     2409 2020-02-02 00:00:00.000000 aiodatastore-0.1.4/tests/unit/test_property.py
+-rw-r--r--   0        0        0     7752 2020-02-02 00:00:00.000000 aiodatastore-0.1.4/tests/unit/test_query.py
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 aiodatastore-0.1.4/tests/unit/test_transaction.py
+-rw-r--r--   0        0        0    21543 2020-02-02 00:00:00.000000 aiodatastore-0.1.4/tests/unit/test_values.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 aiodatastore-0.1.4/.gitignore
+-rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 aiodatastore-0.1.4/LICENSE
+-rw-r--r--   0        0        0     5482 2020-02-02 00:00:00.000000 aiodatastore-0.1.4/README.md
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 aiodatastore-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     6502 2020-02-02 00:00:00.000000 aiodatastore-0.1.4/PKG-INFO
```

### Comparing `aiodatastore-0.1.3/Makefile` & `aiodatastore-0.1.4/Makefile`

 * *Files identical despite different names*

### Comparing `aiodatastore-0.1.3/credentials.json` & `aiodatastore-0.1.4/credentials.json`

 * *Files identical despite different names*

### Comparing `aiodatastore-0.1.3/main.py` & `aiodatastore-0.1.4/main.py`

 * *Files identical despite different names*

### Comparing `aiodatastore-0.1.3/.github/workflows/lint.yml` & `aiodatastore-0.1.4/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `aiodatastore-0.1.3/aiodatastore/__init__.py` & `aiodatastore-0.1.4/aiodatastore/__init__.py`

 * *Files identical despite different names*

### Comparing `aiodatastore-0.1.3/aiodatastore/client.py` & `aiodatastore-0.1.4/aiodatastore/client.py`

 * *Files identical despite different names*

### Comparing `aiodatastore-0.1.3/aiodatastore/commit.py` & `aiodatastore-0.1.4/aiodatastore/commit.py`

 * *Files identical despite different names*

### Comparing `aiodatastore-0.1.3/aiodatastore/constants.py` & `aiodatastore-0.1.4/aiodatastore/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import enum
 
 
 class CompositeFilterOperator(enum.Enum):
     AND = "AND"
+    OR = "OR"
     UNSPECIFIED = "OPERATOR_UNSPECIFIED"
 
 
 class PropertyFilterOperator(enum.Enum):
     EQUAL = "EQUAL"
     GREATER_THAN = "GREATER_THAN"
     GREATER_THAN_OR_EQUAL = "GREATER_THAN_OR_EQUAL"
```

### Comparing `aiodatastore-0.1.3/aiodatastore/entity.py` & `aiodatastore-0.1.4/aiodatastore/entity.py`

 * *Files identical despite different names*

### Comparing `aiodatastore-0.1.3/aiodatastore/filters.py` & `aiodatastore-0.1.4/aiodatastore/filters.py`

 * *Files identical despite different names*

### Comparing `aiodatastore-0.1.3/aiodatastore/key.py` & `aiodatastore-0.1.4/aiodatastore/key.py`

 * *Files identical despite different names*

### Comparing `aiodatastore-0.1.3/aiodatastore/lookup.py` & `aiodatastore-0.1.4/aiodatastore/lookup.py`

 * *Files identical despite different names*

### Comparing `aiodatastore-0.1.3/aiodatastore/mutation.py` & `aiodatastore-0.1.4/aiodatastore/mutation.py`

 * *Files identical despite different names*

### Comparing `aiodatastore-0.1.3/aiodatastore/property.py` & `aiodatastore-0.1.4/aiodatastore/property.py`

 * *Files identical despite different names*

### Comparing `aiodatastore-0.1.3/aiodatastore/query.py` & `aiodatastore-0.1.4/aiodatastore/query.py`

 * *Files identical despite different names*

### Comparing `aiodatastore-0.1.3/aiodatastore/transaction.py` & `aiodatastore-0.1.4/aiodatastore/transaction.py`

 * *Files identical despite different names*

### Comparing `aiodatastore-0.1.3/aiodatastore/values.py` & `aiodatastore-0.1.4/aiodatastore/values.py`

 * *Files identical despite different names*

### Comparing `aiodatastore-0.1.3/tests/integration/test_values.py` & `aiodatastore-0.1.4/tests/integration/test_values.py`

 * *Files identical despite different names*

### Comparing `aiodatastore-0.1.3/tests/unit/test_client.py` & `aiodatastore-0.1.4/tests/unit/test_client.py`

 * *Files identical despite different names*

### Comparing `aiodatastore-0.1.3/tests/unit/test_commit.py` & `aiodatastore-0.1.4/tests/unit/test_commit.py`

 * *Files identical despite different names*

### Comparing `aiodatastore-0.1.3/tests/unit/test_entity.py` & `aiodatastore-0.1.4/tests/unit/test_entity.py`

 * *Files identical despite different names*

### Comparing `aiodatastore-0.1.3/tests/unit/test_filters.py` & `aiodatastore-0.1.4/tests/unit/test_filters.py`

 * *Files identical despite different names*

### Comparing `aiodatastore-0.1.3/tests/unit/test_key.py` & `aiodatastore-0.1.4/tests/unit/test_key.py`

 * *Files identical despite different names*

### Comparing `aiodatastore-0.1.3/tests/unit/test_lookup.py` & `aiodatastore-0.1.4/tests/unit/test_lookup.py`

 * *Files identical despite different names*

### Comparing `aiodatastore-0.1.3/tests/unit/test_mutation.py` & `aiodatastore-0.1.4/tests/unit/test_mutation.py`

 * *Files identical despite different names*

### Comparing `aiodatastore-0.1.3/tests/unit/test_property.py` & `aiodatastore-0.1.4/tests/unit/test_property.py`

 * *Files identical despite different names*

### Comparing `aiodatastore-0.1.3/tests/unit/test_query.py` & `aiodatastore-0.1.4/tests/unit/test_query.py`

 * *Files identical despite different names*

### Comparing `aiodatastore-0.1.3/tests/unit/test_transaction.py` & `aiodatastore-0.1.4/tests/unit/test_transaction.py`

 * *Files identical despite different names*

### Comparing `aiodatastore-0.1.3/tests/unit/test_values.py` & `aiodatastore-0.1.4/tests/unit/test_values.py`

 * *Files identical despite different names*

### Comparing `aiodatastore-0.1.3/.gitignore` & `aiodatastore-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `aiodatastore-0.1.3/LICENSE` & `aiodatastore-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `aiodatastore-0.1.3/README.md` & `aiodatastore-0.1.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 from aiodatastore import Datastore
 
 client = Datastore("project1", service_file="/path/to/file", namespace="namespace1")
 ```
 
 To use [Datastore emulator](https://cloud.google.com/datastore/docs/tools/datastore-emulator) (for tests or development), just define `DATASTORE_EMULATOR_HOST` environment variable (usually value is `127.0.0.1:8081`).
 
-## How to create [keys](https://cloud.google.com/datastore/docs/reference/data/rest/Shared.Types/Value#Key) and [entities](https://cloud.google.com/datastore/docs/reference/data/rest/Shared.Types/Value#entity)
+## How to work with [keys](https://cloud.google.com/datastore/docs/reference/data/rest/Shared.Types/Value#Key) and [entities](https://cloud.google.com/datastore/docs/reference/data/rest/Shared.Types/Value#entity)
 
 ```python
 from aiodatastore import Key, PartitionId, PathElement
 
 key = Key(PartitionId("project1"), [PathElement("Kind1")])
 ```
```

### Comparing `aiodatastore-0.1.3/pyproject.toml` & `aiodatastore-0.1.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "aiodatastore"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
   { name="Max Usachev", email="maxusachev@gmail.com" },
 ]
 description = "Low level and high performance asyncio client for Google Datastore REST API"
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [
```

### Comparing `aiodatastore-0.1.3/PKG-INFO` & `aiodatastore-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiodatastore
-Version: 0.1.3
+Version: 0.1.4
 Summary: Low level and high performance asyncio client for Google Datastore REST API
 Project-URL: Homepage, https://github.com/umax/aiodatastore
 Project-URL: Source, https://github.com/umax/aiodatastore
 Project-URL: Changelog, https://github.com/umax/aiodatastore/blob/main/CHANGELOG.md
 Author-email: Max Usachev <maxusachev@gmail.com>
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
@@ -59,15 +59,15 @@
 from aiodatastore import Datastore
 
 client = Datastore("project1", service_file="/path/to/file", namespace="namespace1")
 ```
 
 To use [Datastore emulator](https://cloud.google.com/datastore/docs/tools/datastore-emulator) (for tests or development), just define `DATASTORE_EMULATOR_HOST` environment variable (usually value is `127.0.0.1:8081`).
 
-## How to create [keys](https://cloud.google.com/datastore/docs/reference/data/rest/Shared.Types/Value#Key) and [entities](https://cloud.google.com/datastore/docs/reference/data/rest/Shared.Types/Value#entity)
+## How to work with [keys](https://cloud.google.com/datastore/docs/reference/data/rest/Shared.Types/Value#Key) and [entities](https://cloud.google.com/datastore/docs/reference/data/rest/Shared.Types/Value#entity)
 
 ```python
 from aiodatastore import Key, PartitionId, PathElement
 
 key = Key(PartitionId("project1"), [PathElement("Kind1")])
 ```
```

