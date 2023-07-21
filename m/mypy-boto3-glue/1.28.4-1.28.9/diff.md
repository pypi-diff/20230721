# Comparing `tmp/mypy-boto3-glue-1.28.4.tar.gz` & `tmp/mypy-boto3-glue-1.28.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-glue-1.28.4.tar", last modified: Tue Jul 18 01:01:41 2023, max compression
+gzip compressed data, was "mypy-boto3-glue-1.28.9.tar", last modified: Fri Jul 21 20:32:58 2023, max compression
```

## Comparing `mypy-boto3-glue-1.28.4.tar` & `mypy-boto3-glue-1.28.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:01:41.973310 mypy-boto3-glue-1.28.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-18 01:01:17.000000 mypy-boto3-glue-1.28.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    47930 2023-07-18 01:01:41.973310 mypy-boto3-glue-1.28.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    46457 2023-07-18 01:01:17.000000 mypy-boto3-glue-1.28.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:01:41.969310 mypy-boto3-glue-1.28.4/mypy_boto3_glue/
--rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-07-18 01:01:17.000000 mypy-boto3-glue-1.28.4/mypy_boto3_glue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-07-18 01:01:17.000000 mypy-boto3-glue-1.28.4/mypy_boto3_glue/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-07-18 01:01:17.000000 mypy-boto3-glue-1.28.4/mypy_boto3_glue/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)   137259 2023-07-18 01:01:19.000000 mypy-boto3-glue-1.28.4/mypy_boto3_glue/client.py
--rw-r--r--   0 runner    (1001) docker     (123)   137031 2023-07-18 01:01:18.000000 mypy-boto3-glue-1.28.4/mypy_boto3_glue/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    20892 2023-07-18 01:01:19.000000 mypy-boto3-glue-1.28.4/mypy_boto3_glue/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    20890 2023-07-18 01:01:19.000000 mypy-boto3-glue-1.28.4/mypy_boto3_glue/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    21235 2023-07-18 01:01:19.000000 mypy-boto3-glue-1.28.4/mypy_boto3_glue/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    21214 2023-07-18 01:01:19.000000 mypy-boto3-glue-1.28.4/mypy_boto3_glue/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 01:01:17.000000 mypy-boto3-glue-1.28.4/mypy_boto3_glue/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   302062 2023-07-18 01:01:27.000000 mypy-boto3-glue-1.28.4/mypy_boto3_glue/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   301703 2023-07-18 01:01:23.000000 mypy-boto3-glue-1.28.4/mypy_boto3_glue/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-18 01:01:17.000000 mypy-boto3-glue-1.28.4/mypy_boto3_glue/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:01:41.973310 mypy-boto3-glue-1.28.4/mypy_boto3_glue.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    47930 2023-07-18 01:01:41.000000 mypy-boto3-glue-1.28.4/mypy_boto3_glue.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-18 01:01:41.000000 mypy-boto3-glue-1.28.4/mypy_boto3_glue.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 01:01:41.000000 mypy-boto3-glue-1.28.4/mypy_boto3_glue.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 01:01:41.000000 mypy-boto3-glue-1.28.4/mypy_boto3_glue.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-18 01:01:41.000000 mypy-boto3-glue-1.28.4/mypy_boto3_glue.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-18 01:01:41.000000 mypy-boto3-glue-1.28.4/mypy_boto3_glue.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 01:01:41.973310 mypy-boto3-glue-1.28.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-07-18 01:01:17.000000 mypy-boto3-glue-1.28.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:32:58.235903 mypy-boto3-glue-1.28.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-21 20:32:11.000000 mypy-boto3-glue-1.28.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    47982 2023-07-21 20:32:58.235903 mypy-boto3-glue-1.28.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    46509 2023-07-21 20:32:11.000000 mypy-boto3-glue-1.28.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:32:58.219902 mypy-boto3-glue-1.28.9/mypy_boto3_glue/
+-rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-07-21 20:32:11.000000 mypy-boto3-glue-1.28.9/mypy_boto3_glue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-07-21 20:32:11.000000 mypy-boto3-glue-1.28.9/mypy_boto3_glue/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-07-21 20:32:11.000000 mypy-boto3-glue-1.28.9/mypy_boto3_glue/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   137259 2023-07-21 20:32:12.000000 mypy-boto3-glue-1.28.9/mypy_boto3_glue/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)   137031 2023-07-21 20:32:12.000000 mypy-boto3-glue-1.28.9/mypy_boto3_glue/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    20915 2023-07-21 20:32:14.000000 mypy-boto3-glue-1.28.9/mypy_boto3_glue/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20913 2023-07-21 20:32:13.000000 mypy-boto3-glue-1.28.9/mypy_boto3_glue/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    21235 2023-07-21 20:32:13.000000 mypy-boto3-glue-1.28.9/mypy_boto3_glue/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21214 2023-07-21 20:32:12.000000 mypy-boto3-glue-1.28.9/mypy_boto3_glue/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 20:32:11.000000 mypy-boto3-glue-1.28.9/mypy_boto3_glue/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   302665 2023-07-21 20:32:22.000000 mypy-boto3-glue-1.28.9/mypy_boto3_glue/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   302306 2023-07-21 20:32:18.000000 mypy-boto3-glue-1.28.9/mypy_boto3_glue/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-21 20:32:11.000000 mypy-boto3-glue-1.28.9/mypy_boto3_glue/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:32:58.235903 mypy-boto3-glue-1.28.9/mypy_boto3_glue.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    47982 2023-07-21 20:32:58.000000 mypy-boto3-glue-1.28.9/mypy_boto3_glue.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-21 20:32:58.000000 mypy-boto3-glue-1.28.9/mypy_boto3_glue.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 20:32:58.000000 mypy-boto3-glue-1.28.9/mypy_boto3_glue.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 20:32:58.000000 mypy-boto3-glue-1.28.9/mypy_boto3_glue.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-21 20:32:58.000000 mypy-boto3-glue-1.28.9/mypy_boto3_glue.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-21 20:32:58.000000 mypy-boto3-glue-1.28.9/mypy_boto3_glue.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 20:32:58.235903 mypy-boto3-glue-1.28.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-07-21 20:32:11.000000 mypy-boto3-glue-1.28.9/setup.py
```

### Comparing `mypy-boto3-glue-1.28.4/LICENSE` & `mypy-boto3-glue-1.28.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-glue-1.28.4/PKG-INFO` & `mypy-boto3-glue-1.28.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-glue
-Version: 1.28.4
-Summary: Type annotations for boto3.Glue 1.28.4 service generated with mypy-boto3-builder 7.15.1
+Version: 1.28.9
+Summary: Type annotations for boto3.Glue 1.28.9 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-glue.svg?color=blue)](https://pypi.org/project/mypy-boto3-glue)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-glue?color=blue)](https://pypistats.org/packages/mypy-boto3-glue)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Glue 1.28.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue)
+[boto3.Glue 1.28.9](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -612,20 +612,22 @@
     ConnectionsListOutputTypeDef,
     ConnectionsListTypeDef,
     CrawlTypeDef,
     CrawlerHistoryTypeDef,
     CrawlerMetricsTypeDef,
     DeltaTargetOutputTypeDef,
     DynamoDBTargetOutputTypeDef,
+    HudiTargetOutputTypeDef,
     IcebergTargetOutputTypeDef,
     JdbcTargetOutputTypeDef,
     MongoDBTargetOutputTypeDef,
     S3TargetOutputTypeDef,
     DeltaTargetTypeDef,
     DynamoDBTargetTypeDef,
+    HudiTargetTypeDef,
     IcebergTargetTypeDef,
     JdbcTargetTypeDef,
     MongoDBTargetTypeDef,
     S3TargetTypeDef,
     LakeFormationConfigurationOutputTypeDef,
     LastCrawlInfoTypeDef,
     LineageConfigurationOutputTypeDef,
```

### Comparing `mypy-boto3-glue-1.28.4/README.md` & `mypy-boto3-glue-1.28.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-glue.svg?color=blue)](https://pypi.org/project/mypy-boto3-glue)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-glue?color=blue)](https://pypistats.org/packages/mypy-boto3-glue)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Glue 1.28.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue)
+[boto3.Glue 1.28.9](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -580,20 +580,22 @@
     ConnectionsListOutputTypeDef,
     ConnectionsListTypeDef,
     CrawlTypeDef,
     CrawlerHistoryTypeDef,
     CrawlerMetricsTypeDef,
     DeltaTargetOutputTypeDef,
     DynamoDBTargetOutputTypeDef,
+    HudiTargetOutputTypeDef,
     IcebergTargetOutputTypeDef,
     JdbcTargetOutputTypeDef,
     MongoDBTargetOutputTypeDef,
     S3TargetOutputTypeDef,
     DeltaTargetTypeDef,
     DynamoDBTargetTypeDef,
+    HudiTargetTypeDef,
     IcebergTargetTypeDef,
     JdbcTargetTypeDef,
     MongoDBTargetTypeDef,
     S3TargetTypeDef,
     LakeFormationConfigurationOutputTypeDef,
     LastCrawlInfoTypeDef,
     LineageConfigurationOutputTypeDef,
```

### Comparing `mypy-boto3-glue-1.28.4/mypy_boto3_glue/__init__.py` & `mypy-boto3-glue-1.28.9/mypy_boto3_glue/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-glue-1.28.4/mypy_boto3_glue/__init__.pyi` & `mypy-boto3-glue-1.28.9/mypy_boto3_glue/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-glue-1.28.4/mypy_boto3_glue/__main__.py` & `mypy-boto3-glue-1.28.9/mypy_boto3_glue/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Glue 1.28.4\nVersion:         1.28.4\nBuilder version:"
+        "Type annotations for boto3.Glue 1.28.9\nVersion:         1.28.9\nBuilder version:"
         " 7.15.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.4")
+    print("1.28.9")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-glue-1.28.4/mypy_boto3_glue/client.py` & `mypy-boto3-glue-1.28.9/mypy_boto3_glue/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-glue-1.28.4/mypy_boto3_glue/client.pyi` & `mypy-boto3-glue-1.28.9/mypy_boto3_glue/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-glue-1.28.4/mypy_boto3_glue/literals.py` & `mypy-boto3-glue-1.28.9/mypy_boto3_glue/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -590,14 +590,15 @@
     "medialive",
     "mediapackage",
     "mediapackage-vod",
     "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
+    "medical-imaging",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
     "migration-hub-refactor-spaces",
     "migrationhub-config",
     "migrationhuborchestrator",
```

### Comparing `mypy-boto3-glue-1.28.4/mypy_boto3_glue/literals.pyi` & `mypy-boto3-glue-1.28.9/mypy_boto3_glue/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -588,14 +588,15 @@
     "medialive",
     "mediapackage",
     "mediapackage-vod",
     "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
+    "medical-imaging",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
     "migration-hub-refactor-spaces",
     "migrationhub-config",
     "migrationhuborchestrator",
```

### Comparing `mypy-boto3-glue-1.28.4/mypy_boto3_glue/paginator.py` & `mypy-boto3-glue-1.28.9/mypy_boto3_glue/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-glue-1.28.4/mypy_boto3_glue/paginator.pyi` & `mypy-boto3-glue-1.28.9/mypy_boto3_glue/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-glue-1.28.4/mypy_boto3_glue/type_defs.py` & `mypy-boto3-glue-1.28.9/mypy_boto3_glue/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -248,20 +248,22 @@
     "ConnectionsListOutputTypeDef",
     "ConnectionsListTypeDef",
     "CrawlTypeDef",
     "CrawlerHistoryTypeDef",
     "CrawlerMetricsTypeDef",
     "DeltaTargetOutputTypeDef",
     "DynamoDBTargetOutputTypeDef",
+    "HudiTargetOutputTypeDef",
     "IcebergTargetOutputTypeDef",
     "JdbcTargetOutputTypeDef",
     "MongoDBTargetOutputTypeDef",
     "S3TargetOutputTypeDef",
     "DeltaTargetTypeDef",
     "DynamoDBTargetTypeDef",
+    "HudiTargetTypeDef",
     "IcebergTargetTypeDef",
     "JdbcTargetTypeDef",
     "MongoDBTargetTypeDef",
     "S3TargetTypeDef",
     "LakeFormationConfigurationOutputTypeDef",
     "LastCrawlInfoTypeDef",
     "LineageConfigurationOutputTypeDef",
@@ -2595,14 +2597,24 @@
     {
         "Path": str,
         "scanAll": bool,
         "scanRate": float,
     },
 )
 
+HudiTargetOutputTypeDef = TypedDict(
+    "HudiTargetOutputTypeDef",
+    {
+        "Paths": List[str],
+        "ConnectionName": str,
+        "Exclusions": List[str],
+        "MaximumTraversalDepth": int,
+    },
+)
+
 IcebergTargetOutputTypeDef = TypedDict(
     "IcebergTargetOutputTypeDef",
     {
         "Paths": List[str],
         "ConnectionName": str,
         "Exclusions": List[str],
         "MaximumTraversalDepth": int,
@@ -2657,14 +2669,25 @@
         "Path": str,
         "scanAll": bool,
         "scanRate": float,
     },
     total=False,
 )
 
+HudiTargetTypeDef = TypedDict(
+    "HudiTargetTypeDef",
+    {
+        "Paths": Sequence[str],
+        "ConnectionName": str,
+        "Exclusions": Sequence[str],
+        "MaximumTraversalDepth": int,
+    },
+    total=False,
+)
+
 IcebergTargetTypeDef = TypedDict(
     "IcebergTargetTypeDef",
     {
         "Paths": Sequence[str],
         "ConnectionName": str,
         "Exclusions": Sequence[str],
         "MaximumTraversalDepth": int,
@@ -7289,27 +7312,29 @@
         "S3Targets": List[S3TargetOutputTypeDef],
         "JdbcTargets": List[JdbcTargetOutputTypeDef],
         "MongoDBTargets": List[MongoDBTargetOutputTypeDef],
         "DynamoDBTargets": List[DynamoDBTargetOutputTypeDef],
         "CatalogTargets": List[CatalogTargetOutputTypeDef],
         "DeltaTargets": List[DeltaTargetOutputTypeDef],
         "IcebergTargets": List[IcebergTargetOutputTypeDef],
+        "HudiTargets": List[HudiTargetOutputTypeDef],
     },
 )
 
 CrawlerTargetsTypeDef = TypedDict(
     "CrawlerTargetsTypeDef",
     {
         "S3Targets": Sequence[S3TargetTypeDef],
         "JdbcTargets": Sequence[JdbcTargetTypeDef],
         "MongoDBTargets": Sequence[MongoDBTargetTypeDef],
         "DynamoDBTargets": Sequence[DynamoDBTargetTypeDef],
         "CatalogTargets": Sequence[CatalogTargetTypeDef],
         "DeltaTargets": Sequence[DeltaTargetTypeDef],
         "IcebergTargets": Sequence[IcebergTargetTypeDef],
+        "HudiTargets": Sequence[HudiTargetTypeDef],
     },
     total=False,
 )
 
 _RequiredListCrawlsRequestRequestTypeDef = TypedDict(
     "_RequiredListCrawlsRequestRequestTypeDef",
     {
```

### Comparing `mypy-boto3-glue-1.28.4/mypy_boto3_glue/type_defs.pyi` & `mypy-boto3-glue-1.28.9/mypy_boto3_glue/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -247,20 +247,22 @@
     "ConnectionsListOutputTypeDef",
     "ConnectionsListTypeDef",
     "CrawlTypeDef",
     "CrawlerHistoryTypeDef",
     "CrawlerMetricsTypeDef",
     "DeltaTargetOutputTypeDef",
     "DynamoDBTargetOutputTypeDef",
+    "HudiTargetOutputTypeDef",
     "IcebergTargetOutputTypeDef",
     "JdbcTargetOutputTypeDef",
     "MongoDBTargetOutputTypeDef",
     "S3TargetOutputTypeDef",
     "DeltaTargetTypeDef",
     "DynamoDBTargetTypeDef",
+    "HudiTargetTypeDef",
     "IcebergTargetTypeDef",
     "JdbcTargetTypeDef",
     "MongoDBTargetTypeDef",
     "S3TargetTypeDef",
     "LakeFormationConfigurationOutputTypeDef",
     "LastCrawlInfoTypeDef",
     "LineageConfigurationOutputTypeDef",
@@ -2554,14 +2556,24 @@
     {
         "Path": str,
         "scanAll": bool,
         "scanRate": float,
     },
 )
 
+HudiTargetOutputTypeDef = TypedDict(
+    "HudiTargetOutputTypeDef",
+    {
+        "Paths": List[str],
+        "ConnectionName": str,
+        "Exclusions": List[str],
+        "MaximumTraversalDepth": int,
+    },
+)
+
 IcebergTargetOutputTypeDef = TypedDict(
     "IcebergTargetOutputTypeDef",
     {
         "Paths": List[str],
         "ConnectionName": str,
         "Exclusions": List[str],
         "MaximumTraversalDepth": int,
@@ -2616,14 +2628,25 @@
         "Path": str,
         "scanAll": bool,
         "scanRate": float,
     },
     total=False,
 )
 
+HudiTargetTypeDef = TypedDict(
+    "HudiTargetTypeDef",
+    {
+        "Paths": Sequence[str],
+        "ConnectionName": str,
+        "Exclusions": Sequence[str],
+        "MaximumTraversalDepth": int,
+    },
+    total=False,
+)
+
 IcebergTargetTypeDef = TypedDict(
     "IcebergTargetTypeDef",
     {
         "Paths": Sequence[str],
         "ConnectionName": str,
         "Exclusions": Sequence[str],
         "MaximumTraversalDepth": int,
@@ -7090,27 +7113,29 @@
         "S3Targets": List[S3TargetOutputTypeDef],
         "JdbcTargets": List[JdbcTargetOutputTypeDef],
         "MongoDBTargets": List[MongoDBTargetOutputTypeDef],
         "DynamoDBTargets": List[DynamoDBTargetOutputTypeDef],
         "CatalogTargets": List[CatalogTargetOutputTypeDef],
         "DeltaTargets": List[DeltaTargetOutputTypeDef],
         "IcebergTargets": List[IcebergTargetOutputTypeDef],
+        "HudiTargets": List[HudiTargetOutputTypeDef],
     },
 )
 
 CrawlerTargetsTypeDef = TypedDict(
     "CrawlerTargetsTypeDef",
     {
         "S3Targets": Sequence[S3TargetTypeDef],
         "JdbcTargets": Sequence[JdbcTargetTypeDef],
         "MongoDBTargets": Sequence[MongoDBTargetTypeDef],
         "DynamoDBTargets": Sequence[DynamoDBTargetTypeDef],
         "CatalogTargets": Sequence[CatalogTargetTypeDef],
         "DeltaTargets": Sequence[DeltaTargetTypeDef],
         "IcebergTargets": Sequence[IcebergTargetTypeDef],
+        "HudiTargets": Sequence[HudiTargetTypeDef],
     },
     total=False,
 )
 
 _RequiredListCrawlsRequestRequestTypeDef = TypedDict(
     "_RequiredListCrawlsRequestRequestTypeDef",
     {
```

### Comparing `mypy-boto3-glue-1.28.4/mypy_boto3_glue.egg-info/PKG-INFO` & `mypy-boto3-glue-1.28.9/mypy_boto3_glue.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-glue
-Version: 1.28.4
-Summary: Type annotations for boto3.Glue 1.28.4 service generated with mypy-boto3-builder 7.15.1
+Version: 1.28.9
+Summary: Type annotations for boto3.Glue 1.28.9 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-glue.svg?color=blue)](https://pypi.org/project/mypy-boto3-glue)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-glue?color=blue)](https://pypistats.org/packages/mypy-boto3-glue)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Glue 1.28.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue)
+[boto3.Glue 1.28.9](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -612,20 +612,22 @@
     ConnectionsListOutputTypeDef,
     ConnectionsListTypeDef,
     CrawlTypeDef,
     CrawlerHistoryTypeDef,
     CrawlerMetricsTypeDef,
     DeltaTargetOutputTypeDef,
     DynamoDBTargetOutputTypeDef,
+    HudiTargetOutputTypeDef,
     IcebergTargetOutputTypeDef,
     JdbcTargetOutputTypeDef,
     MongoDBTargetOutputTypeDef,
     S3TargetOutputTypeDef,
     DeltaTargetTypeDef,
     DynamoDBTargetTypeDef,
+    HudiTargetTypeDef,
     IcebergTargetTypeDef,
     JdbcTargetTypeDef,
     MongoDBTargetTypeDef,
     S3TargetTypeDef,
     LakeFormationConfigurationOutputTypeDef,
     LastCrawlInfoTypeDef,
     LineageConfigurationOutputTypeDef,
```

### Comparing `mypy-boto3-glue-1.28.4/mypy_boto3_glue.egg-info/SOURCES.txt` & `mypy-boto3-glue-1.28.9/mypy_boto3_glue.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-glue-1.28.4/setup.py` & `mypy-boto3-glue-1.28.9/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-glue",
-    version="1.28.4",
+    version="1.28.9",
     packages=["mypy_boto3_glue"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Glue 1.28.4 service generated with mypy-boto3-builder 7.15.1"
+        "Type annotations for boto3.Glue 1.28.9 service generated with mypy-boto3-builder 7.15.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

