# Comparing `tmp/coola-0.0.8.tar.gz` & `tmp/coola-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coola-0.0.8.tar", max compression
+gzip compressed data, was "coola-0.0.9.tar", max compression
```

## Comparing `coola-0.0.8.tar` & `coola-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1501 2023-06-09 05:31:29.801109 coola-0.0.8/LICENSE
--rw-r--r--   0        0        0     5043 2023-06-09 05:31:29.801109 coola-0.0.8/README.md
--rw-r--r--   0        0        0     4147 2023-06-09 05:31:29.805109 coola-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      939 2023-06-09 05:31:29.805109 coola-0.0.8/src/coola/__init__.py
--rw-r--r--   0        0        0     4251 2023-06-09 05:31:29.805109 coola-0.0.8/src/coola/_numpy.py
--rw-r--r--   0        0        0     7410 2023-06-09 05:31:29.805109 coola-0.0.8/src/coola/_torch.py
--rw-r--r--   0        0        0     2632 2023-06-09 05:31:29.805109 coola-0.0.8/src/coola/_xarray.py
--rw-r--r--   0        0        0    18491 2023-06-09 05:31:29.805109 coola-0.0.8/src/coola/allclose.py
--rw-r--r--   0        0        0    13211 2023-06-09 05:31:29.805109 coola-0.0.8/src/coola/equality.py
--rw-r--r--   0        0        0      489 2023-06-09 05:31:29.805109 coola-0.0.8/src/coola/testing.py
--rw-r--r--   0        0        0        0 2023-06-09 05:31:29.805109 coola-0.0.8/src/coola/utils/__init__.py
--rw-r--r--   0        0        0     2490 2023-06-09 05:31:29.805109 coola-0.0.8/src/coola/utils/format.py
--rw-r--r--   0        0        0     1842 2023-06-09 05:31:29.805109 coola-0.0.8/src/coola/utils/imports.py
--rw-r--r--   0        0        0     6243 1970-01-01 00:00:00.000000 coola-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1501 2023-06-10 03:30:19.217165 coola-0.0.9/LICENSE
+-rw-r--r--   0        0        0     5043 2023-06-10 03:30:19.217165 coola-0.0.9/README.md
+-rw-r--r--   0        0        0     4186 2023-06-10 03:30:19.221165 coola-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      939 2023-06-10 03:30:19.221165 coola-0.0.9/src/coola/__init__.py
+-rw-r--r--   0        0        0     4361 2023-06-10 03:30:19.221165 coola-0.0.9/src/coola/_numpy.py
+-rw-r--r--   0        0        0     7630 2023-06-10 03:30:19.221165 coola-0.0.9/src/coola/_torch.py
+-rw-r--r--   0        0        0     9046 2023-06-10 03:30:19.221165 coola-0.0.9/src/coola/_xarray.py
+-rw-r--r--   0        0        0    18587 2023-06-10 03:30:19.221165 coola-0.0.9/src/coola/allclose.py
+-rw-r--r--   0        0        0    13282 2023-06-10 03:30:19.221165 coola-0.0.9/src/coola/equality.py
+-rw-r--r--   0        0        0      489 2023-06-10 03:30:19.221165 coola-0.0.9/src/coola/testing.py
+-rw-r--r--   0        0        0        0 2023-06-10 03:30:19.221165 coola-0.0.9/src/coola/utils/__init__.py
+-rw-r--r--   0        0        0     2490 2023-06-10 03:30:19.221165 coola-0.0.9/src/coola/utils/format.py
+-rw-r--r--   0        0        0     1842 2023-06-10 03:30:19.221165 coola-0.0.9/src/coola/utils/imports.py
+-rw-r--r--   0        0        0     6237 1970-01-01 00:00:00.000000 coola-0.0.9/PKG-INFO
```

### Comparing `coola-0.0.8/LICENSE` & `coola-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `coola-0.0.8/README.md` & `coola-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `coola-0.0.8/pyproject.toml` & `coola-0.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "coola"
-version = "0.0.8"
-description = "A light library to check if two complex/nested objects are equal or not"
+version = "0.0.9"
+description = "A library to check if two complex/nested objects are equal or not"
 readme = "README.md"
 authors = ["Thibaut Durand <durand.tibo+gh@gmail.com>"]
 homepage = "https://github.com/durandtibo/coola"
 repository = "https://github.com/durandtibo/coola"
 keywords = ["equality", "complex/nested objects"]
 license = "BSD-3-Clause"
 
@@ -24,15 +24,18 @@
 ]
 
 packages = [
     { include = "coola", from = "src" },
 ]
 
 [tool.poetry.dependencies]
+# Core dependencies
 python = "^3.9"
+
+# Optional dependencies
 numpy = { version = "^1.20", optional = true }
 torch = { version = ">=1.10,<3.0", optional = true}
 xarray = { version = ">=2022.3.0", optional = true}
 
 [tool.poetry.extras]
 all = ["numpy", "torch", "xarray"]
```

### Comparing `coola-0.0.8/src/coola/__init__.py` & `coola-0.0.9/src/coola/__init__.py`

 * *Files identical despite different names*

### Comparing `coola-0.0.8/src/coola/_numpy.py` & `coola-0.0.9/src/coola/_numpy.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,14 +37,16 @@
         object1: ndarray,
         object2: Any,
         rtol: float = 1e-5,
         atol: float = 1e-8,
         equal_nan: bool = False,
         show_difference: bool = False,
     ) -> bool:
+        if object1 is object2:
+            return True
         if not isinstance(object2, ndarray):
             if show_difference:
                 logger.info(f"object2 is not a numpy.ndarray: {type(object2)}")
             return False
         if self._check_dtype and object1.dtype != object2.dtype:
             if show_difference:
                 logger.info(
@@ -82,14 +84,16 @@
     def equal(
         self,
         tester: BaseEqualityTester,
         object1: ndarray,
         object2: Any,
         show_difference: bool = False,
     ) -> bool:
+        if object1 is object2:
+            return True
         if not isinstance(object2, ndarray):
             if show_difference:
                 logger.info(f"object2 is not a numpy.ndarray: {type(object2)}")
             return False
         if self._check_dtype and object1.dtype != object2.dtype:
             if show_difference:
                 logger.info(
```

### Comparing `coola-0.0.8/src/coola/_torch.py` & `coola-0.0.9/src/coola/_torch.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,16 @@
         object1: PackedSequence,
         object2: Any,
         rtol: float = 1e-5,
         atol: float = 1e-8,
         equal_nan: bool = False,
         show_difference: bool = False,
     ) -> bool:
+        if object1 is object2:
+            return True
         if not isinstance(object2, PackedSequence):
             if show_difference:
                 logger.info(
                     f"object2 is not a `torch.nn.utils.rnn.PackedSequence`: {type(object2)}"
                 )
             return False
         object_equal = (
@@ -91,14 +93,16 @@
     def equal(
         self,
         tester: BaseEqualityTester,
         object1: PackedSequence,
         object2: Any,
         show_difference: bool = False,
     ) -> bool:
+        if object1 is object2:
+            return True
         if not isinstance(object2, PackedSequence):
             if show_difference:
                 logger.info(
                     f"object2 is not a `torch.nn.utils.rnn.PackedSequence`: {type(object2)}"
                 )
             return False
         object_equal = (
@@ -127,14 +131,16 @@
         object1: Tensor,
         object2: Any,
         rtol: float = 1e-5,
         atol: float = 1e-8,
         equal_nan: bool = False,
         show_difference: bool = False,
     ) -> bool:
+        if object1 is object2:
+            return True
         if not is_tensor(object2):
             if show_difference:
                 logger.info(f"object2 is not a torch.Tensor: {type(object2)}")
             return False
         if object1.dtype != object2.dtype:
             if show_difference:
                 logger.info(
@@ -168,14 +174,16 @@
     def equal(
         self,
         tester: BaseEqualityTester,
         object1: Tensor,
         object2: Any,
         show_difference: bool = False,
     ) -> bool:
+        if object1 is object2:
+            return True
         if not is_tensor(object2):
             if show_difference:
                 logger.info(f"object2 is not a torch.Tensor: {type(object2)}")
             return False
         if object1.dtype != object2.dtype:
             if show_difference:
                 logger.info(
```

### Comparing `coola-0.0.8/src/coola/allclose.py` & `coola-0.0.9/src/coola/allclose.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,13 @@
 from __future__ import annotations
 
 __all__ = [
     "AllCloseTester",
     "BaseAllCloseOperator",
     "BaseAllCloseTester",
-    "DefaultAllCloseOperator",
-    "MappingAllCloseOperator",
-    "ScalarAllCloseOperator",
-    "SequenceAllCloseOperator",
     "objects_are_allclose",
 ]
 
 import logging
 import math
 from abc import ABC, abstractmethod
 from collections.abc import Mapping, Sequence
@@ -199,14 +195,16 @@
         object1: Any,
         object2: Any,
         rtol: float = 1e-5,
         atol: float = 1e-8,
         equal_nan: bool = False,
         show_difference: bool = False,
     ) -> bool:
+        if object1 is object2:
+            return True
         if type(object1) is not type(object2):
             if show_difference:
                 logger.info(f"Objects have different types: {type(object1)} vs {type(object2)}")
             return False
         object_equal = object1 == object2
         if show_difference and not object_equal:
             logger.info(f"Objects are different:\nobject1={object1}\nobject2={object2}")
@@ -222,14 +220,16 @@
         object1: Mapping,
         object2: Any,
         rtol: float = 1e-5,
         atol: float = 1e-8,
         equal_nan: bool = False,
         show_difference: bool = False,
     ) -> bool:
+        if object1 is object2:
+            return True
         if type(object1) is not type(object2):
             if show_difference:
                 logger.info(
                     f"The mappings have different types: {type(object1)} vs {type(object2)}"
                 )
             return False
         if len(object1) != len(object2):
@@ -267,14 +267,16 @@
         object1: bool | int | float,
         object2: Any,
         rtol: float = 1e-5,
         atol: float = 1e-8,
         equal_nan: bool = False,
         show_difference: bool = False,
     ) -> bool:
+        if object1 is object2:
+            return True
         if type(object1) is not type(object2):
             if show_difference:
                 logger.info(f"Objects have different types: {type(object1)} vs {type(object2)}")
             return False
         number_equal = math.isclose(object1, object2, rel_tol=rtol, abs_tol=atol)
         if show_difference and not number_equal:
             logger.info(f"The numbers are different: {object1} vs {object2}")
@@ -290,14 +292,16 @@
         object1: Sequence,
         object2: Any,
         rtol: float = 1e-5,
         atol: float = 1e-8,
         equal_nan: bool = False,
         show_difference: bool = False,
     ) -> bool:
+        if object1 is object2:
+            return True
         if type(object1) is not type(object2):
             if show_difference:
                 logger.info(
                     f"The sequences have different types: {type(object1)} vs {type(object2)}"
                 )
             return False
         if len(object1) != len(object2):
```

### Comparing `coola-0.0.8/src/coola/equality.py` & `coola-0.0.9/src/coola/equality.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 from __future__ import annotations
 
 __all__ = [
     "BaseEqualityOperator",
     "BaseEqualityTester",
-    "DefaultEqualityOperator",
     "EqualityTester",
-    "MappingEqualityOperator",
-    "SequenceEqualityOperator",
     "objects_are_equal",
 ]
 
 import logging
 from abc import ABC, abstractmethod
 from collections.abc import Mapping, Sequence
 from typing import Any, Generic, TypeVar
@@ -137,14 +134,16 @@
     def equal(
         self,
         tester: BaseEqualityTester,
         object1: Any,
         object2: Any,
         show_difference: bool = False,
     ) -> bool:
+        if object1 is object2:
+            return True
         if type(object1) is not type(object2):
             if show_difference:
                 logger.info(f"Objects have different types: {type(object1)} vs {type(object2)}")
             return False
         object_equal = object1 == object2
         if show_difference and not object_equal:
             logger.info(f"Objects are different:\nobject1={object1}\nobject2={object2}")
@@ -157,14 +156,16 @@
     def equal(
         self,
         tester: BaseEqualityTester,
         object1: Mapping,
         object2: Any,
         show_difference: bool = False,
     ) -> bool:
+        if object1 is object2:
+            return True
         if type(object1) is not type(object2):
             if show_difference:
                 logger.info(
                     f"The mappings have different types: {type(object1)} vs {type(object2)}"
                 )
             return False
         if len(object1) != len(object2):
@@ -197,14 +198,16 @@
     def equal(
         self,
         tester: BaseEqualityTester,
         object1: Sequence,
         object2: Any,
         show_difference: bool = False,
     ) -> bool:
+        if object1 is object2:
+            return True
         if type(object1) is not type(object2):
             if show_difference:
                 logger.info(
                     f"The sequences have different types: {type(object1)} vs {type(object2)}"
                 )
             return False
         if len(object1) != len(object2):
```

### Comparing `coola-0.0.8/src/coola/utils/format.py` & `coola-0.0.9/src/coola/utils/format.py`

 * *Files identical despite different names*

### Comparing `coola-0.0.8/src/coola/utils/imports.py` & `coola-0.0.9/src/coola/utils/imports.py`

 * *Files identical despite different names*

### Comparing `coola-0.0.8/PKG-INFO` & `coola-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: coola
-Version: 0.0.8
-Summary: A light library to check if two complex/nested objects are equal or not
+Version: 0.0.9
+Summary: A library to check if two complex/nested objects are equal or not
 Home-page: https://github.com/durandtibo/coola
 License: BSD-3-Clause
 Keywords: equality,complex/nested objects
 Author: Thibaut Durand
 Author-email: durand.tibo+gh@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: coola Version: 0.0.8 Summary: A light library to
-check if two complex/nested objects are equal or not Home-page: https://
-github.com/durandtibo/coola License: BSD-3-Clause Keywords: equality,complex/
-nested objects Author: Thibaut Durand Author-email: durand.tibo+gh@gmail.com
-Requires-Python: >=3.9,<4.0 Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
-Information Technology Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: BSD License Classifier: Operating System
-:: POSIX :: Linux Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
-Topic :: Scientific/Engineering Classifier: Topic :: Software Development ::
-Libraries Provides-Extra: all Requires-Dist: numpy (>=1.20,<2.0) ; extra ==
-"all" Requires-Dist: torch (>=1.10,<3.0) ; extra == "all" Requires-Dist: xarray
+Metadata-Version: 2.1 Name: coola Version: 0.0.9 Summary: A library to check if
+two complex/nested objects are equal or not Home-page: https://github.com/
+durandtibo/coola License: BSD-3-Clause Keywords: equality,complex/nested
+objects Author: Thibaut Durand Author-email: durand.tibo+gh@gmail.com Requires-
+Python: >=3.9,<4.0 Classifier: Development Status :: 4 - Beta Classifier:
+Intended Audience :: Developers Classifier: Intended Audience :: Information
+Technology Classifier: Intended Audience :: Science/Research Classifier:
+License :: OSI Approved :: BSD License Classifier: Operating System :: POSIX ::
+Linux Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Classifier: Topic ::
+Scientific/Engineering Classifier: Topic :: Software Development :: Libraries
+Provides-Extra: all Requires-Dist: numpy (>=1.20,<2.0) ; extra == "all"
+Requires-Dist: torch (>=1.10,<3.0) ; extra == "all" Requires-Dist: xarray
 (>=2022.3.0) ; extra == "all" Project-URL: Repository, https://github.com/
 durandtibo/coola Description-Content-Type: text/markdown # coola
           [CI] [CI] [Codecov] [https://api.codeclimate.com/v1/badges/
  83ebb50e6c6f67b0570d/maintainability] [https://api.codeclimate.com/v1/badges/
                      83ebb50e6c6f67b0570d/test_coverage]
 [PYPI_version] [Python] [BSD-3-Clause] [Code_style:_black] [Doc_style:_google]
                        [Downloads] [Monthly_downloads]
```

