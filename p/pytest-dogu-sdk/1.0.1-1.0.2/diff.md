# Comparing `tmp/pytest_dogu_sdk-1.0.1.tar.gz` & `tmp/pytest_dogu_sdk-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_dogu_sdk-1.0.1.tar", max compression
+gzip compressed data, was "pytest_dogu_sdk-1.0.2.tar", max compression
```

## Comparing `pytest_dogu_sdk-1.0.1.tar` & `pytest_dogu_sdk-1.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      899 2023-07-21 05:40:53.100944 pytest_dogu_sdk-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     1690 2023-07-20 16:33:36.015474 pytest_dogu_sdk-1.0.1/README.md
--rw-r--r--   0        0        0     1031 2023-07-21 04:07:57.199858 pytest_dogu_sdk-1.0.1/src/pytest_dogu_sdk/__init__.py
--rw-r--r--   0        0        0     3258 2023-07-21 04:07:57.199858 pytest_dogu_sdk-1.0.1/src/pytest_dogu_sdk/common.py
--rw-r--r--   0        0        0     1885 2023-07-20 16:33:36.020475 pytest_dogu_sdk-1.0.1/src/pytest_dogu_sdk/dogu.config.schema.json
--rw-r--r--   0        0        0     3163 2023-07-20 16:33:36.021473 pytest_dogu_sdk-1.0.1/src/pytest_dogu_sdk/dogu_config.py
--rw-r--r--   0        0        0       89 2023-07-21 04:07:57.200858 pytest_dogu_sdk-1.0.1/src/pytest_dogu_sdk/dogu_hooks.py
--rw-r--r--   0        0        0     2721 2023-07-21 04:07:57.265860 pytest_dogu_sdk-1.0.1/src/pytest_dogu_sdk/dogu_sdk.py
--rw-r--r--   0        0        0     2832 2023-07-20 16:33:36.023474 pytest_dogu_sdk-1.0.1/src/pytest_dogu_sdk/remote_dest_report_client.py
--rw-r--r--   0        0        0     9664 2023-07-21 04:07:57.201858 pytest_dogu_sdk-1.0.1/src/pytest_dogu_sdk/remote_dest_reporter.py
--rw-r--r--   0        0        0     3037 2023-07-20 16:33:36.024474 pytest_dogu_sdk-1.0.1/src/pytest_dogu_sdk/routine_dest_report_client.py
--rw-r--r--   0        0        0     9774 2023-07-20 16:33:36.024474 pytest_dogu_sdk-1.0.1/src/pytest_dogu_sdk/routine_dest_reporter.py
--rw-r--r--   0        0        0     2218 1970-01-01 00:00:00.000000 pytest_dogu_sdk-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0      899 2023-07-21 06:19:11.695622 pytest_dogu_sdk-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1690 2023-07-20 16:33:36.015474 pytest_dogu_sdk-1.0.2/README.md
+-rw-r--r--   0        0        0     1031 2023-07-21 04:07:57.199858 pytest_dogu_sdk-1.0.2/src/pytest_dogu_sdk/__init__.py
+-rw-r--r--   0        0        0     3473 2023-07-21 06:13:11.583371 pytest_dogu_sdk-1.0.2/src/pytest_dogu_sdk/common.py
+-rw-r--r--   0        0        0     1885 2023-07-20 16:33:36.020475 pytest_dogu_sdk-1.0.2/src/pytest_dogu_sdk/dogu.config.schema.json
+-rw-r--r--   0        0        0     3163 2023-07-20 16:33:36.021473 pytest_dogu_sdk-1.0.2/src/pytest_dogu_sdk/dogu_config.py
+-rw-r--r--   0        0        0       89 2023-07-21 06:08:38.134467 pytest_dogu_sdk-1.0.2/src/pytest_dogu_sdk/dogu_hooks.py
+-rw-r--r--   0        0        0     2875 2023-07-21 06:17:25.631796 pytest_dogu_sdk-1.0.2/src/pytest_dogu_sdk/dogu_sdk.py
+-rw-r--r--   0        0        0     2832 2023-07-20 16:33:36.023474 pytest_dogu_sdk-1.0.2/src/pytest_dogu_sdk/remote_dest_report_client.py
+-rw-r--r--   0        0        0     9664 2023-07-21 04:07:57.201858 pytest_dogu_sdk-1.0.2/src/pytest_dogu_sdk/remote_dest_reporter.py
+-rw-r--r--   0        0        0     3037 2023-07-20 16:33:36.024474 pytest_dogu_sdk-1.0.2/src/pytest_dogu_sdk/routine_dest_report_client.py
+-rw-r--r--   0        0        0     9774 2023-07-20 16:33:36.024474 pytest_dogu_sdk-1.0.2/src/pytest_dogu_sdk/routine_dest_reporter.py
+-rw-r--r--   0        0        0     2218 1970-01-01 00:00:00.000000 pytest_dogu_sdk-1.0.2/PKG-INFO
```

### Comparing `pytest_dogu_sdk-1.0.1/pyproject.toml` & `pytest_dogu_sdk-1.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pytest-dogu-sdk"
-version = "1.0.1"
+version = "1.0.2"
 description = "pytest plugin for the Dogu"
 readme = "README.md"
 packages = [{include = "pytest_dogu_sdk", from = "src"}]
 authors = ["Dogu Technologies"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `pytest_dogu_sdk-1.0.1/README.md` & `pytest_dogu_sdk-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pytest_dogu_sdk-1.0.1/src/pytest_dogu_sdk/__init__.py` & `pytest_dogu_sdk-1.0.2/src/pytest_dogu_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_dogu_sdk-1.0.1/src/pytest_dogu_sdk/common.py` & `pytest_dogu_sdk-1.0.2/src/pytest_dogu_sdk/common.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from abc import ABC, abstractmethod
 from dataclasses import asdict, dataclass, field
 from enum import Enum, IntEnum, unique
-from typing import Any, Dict, List, Optional, Tuple, TypeVar
+from typing import Any, Dict, List, Optional, Tuple, Type, TypeVar
 
 from dacite import Config, from_dict
 from pytest import Item, Session, TestReport
 import requests
 
 from .dogu_config import DoguConfig
 
@@ -119,24 +119,28 @@
         pass
 
     def on_pytest_runtest_logreport(self, report: TestReport) -> None:
         pass
 
 
 class DoguClient(ABC):
+    def __init__(self) -> None:
+        super().__init__()
+        self.impl: Optional[T] = None
+
     @abstractmethod
-    def on_setup(self, dogu_config: DoguConfig):
+    def on_setup(self, dogu_config: DoguConfig) -> Any:
         pass
 
     @property
     @abstractmethod
     def dogu_results(self) -> Dict[str, Any]:
         pass
 
-    @property
     @abstractmethod
-    def instance(self) -> T:
+    def on_teardown(self) -> None:
         pass
 
-    @abstractmethod
-    def on_teardown(self):
-        pass
+    def cast(self, cls: Type[T]) -> T:
+        if not isinstance(self.impl, cls):
+            raise Exception(f"impl is not an instance of {cls}")
+        return self.impl
```

### Comparing `pytest_dogu_sdk-1.0.1/src/pytest_dogu_sdk/dogu.config.schema.json` & `pytest_dogu_sdk-1.0.2/src/pytest_dogu_sdk/dogu.config.schema.json`

 * *Files identical despite different names*

### Comparing `pytest_dogu_sdk-1.0.1/src/pytest_dogu_sdk/dogu_config.py` & `pytest_dogu_sdk-1.0.2/src/pytest_dogu_sdk/dogu_config.py`

 * *Files identical despite different names*

### Comparing `pytest_dogu_sdk-1.0.1/src/pytest_dogu_sdk/dogu_sdk.py` & `pytest_dogu_sdk-1.0.2/src/pytest_dogu_sdk/dogu_sdk.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,17 +9,22 @@
 
 class DoguSdk:
     name = "dogu_sdk"
 
     def __init__(self, config: Config) -> None:
         self._config = config
         self._dogu_config = DoguConfigFactory().create()
+
         (client,) = self._config.hook.pytest_dogu_create_client()
         self.client: DoguClient = client
-        self.client.on_setup(self._dogu_config)
+        client_impl = self.client.on_setup(self._dogu_config)
+        if not client_impl:
+            raise Exception("dogu client is not initialized on setup")
+        self.client.impl = client_impl
+
         self._routine_dest_reporter = RoutineDestReporterFactory(
             self._dogu_config
         ).create()
         self._remote_dest_reporter = RemoteDestReporterFactory(
             self._dogu_config,
             self.client,
         ).create()
```

### Comparing `pytest_dogu_sdk-1.0.1/src/pytest_dogu_sdk/remote_dest_report_client.py` & `pytest_dogu_sdk-1.0.2/src/pytest_dogu_sdk/remote_dest_report_client.py`

 * *Files identical despite different names*

### Comparing `pytest_dogu_sdk-1.0.1/src/pytest_dogu_sdk/remote_dest_reporter.py` & `pytest_dogu_sdk-1.0.2/src/pytest_dogu_sdk/remote_dest_reporter.py`

 * *Files identical despite different names*

### Comparing `pytest_dogu_sdk-1.0.1/src/pytest_dogu_sdk/routine_dest_report_client.py` & `pytest_dogu_sdk-1.0.2/src/pytest_dogu_sdk/routine_dest_report_client.py`

 * *Files identical despite different names*

### Comparing `pytest_dogu_sdk-1.0.1/src/pytest_dogu_sdk/routine_dest_reporter.py` & `pytest_dogu_sdk-1.0.2/src/pytest_dogu_sdk/routine_dest_reporter.py`

 * *Files identical despite different names*

### Comparing `pytest_dogu_sdk-1.0.1/PKG-INFO` & `pytest_dogu_sdk-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-dogu-sdk
-Version: 1.0.1
+Version: 1.0.2
 Summary: pytest plugin for the Dogu
 Author: Dogu Technologies
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

