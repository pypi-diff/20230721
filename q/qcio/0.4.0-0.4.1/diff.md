# Comparing `tmp/qcio-0.4.0.tar.gz` & `tmp/qcio-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qcio-0.4.0.tar", max compression
+gzip compressed data, was "qcio-0.4.1.tar", max compression
```

## Comparing `qcio-0.4.0.tar` & `qcio-0.4.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1079 2023-07-20 04:00:09.992243 qcio-0.4.0/LICENSE
--rw-r--r--   0        0        0      898 2023-07-20 04:00:09.992243 qcio-0.4.0/README.md
--rw-r--r--   0        0        0     1246 2023-07-20 04:00:09.992243 qcio-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      573 2023-07-20 04:00:09.992243 qcio-0.4.0/qcio/__init__.py
--rw-r--r--   0        0        0       89 2023-07-20 04:00:09.992243 qcio-0.4.0/qcio/constants.py
--rw-r--r--   0        0        0      483 2023-07-20 04:00:09.992243 qcio-0.4.0/qcio/helper_types.py
--rw-r--r--   0        0        0      235 2023-07-20 04:00:09.992243 qcio-0.4.0/qcio/models/__init__.py
--rw-r--r--   0        0        0     9738 2023-07-20 04:00:09.992243 qcio-0.4.0/qcio/models/base_models.py
--rw-r--r--   0        0        0     3082 2023-07-20 04:00:09.992243 qcio-0.4.0/qcio/models/inputs.py
--rw-r--r--   0        0        0     2286 2023-07-20 04:00:09.992243 qcio-0.4.0/qcio/models/inputs_base.py
--rw-r--r--   0        0        0     8302 2023-07-20 04:00:09.992243 qcio-0.4.0/qcio/models/molecule.py
--rw-r--r--   0        0        0     8595 2023-07-20 04:00:09.992243 qcio-0.4.0/qcio/models/outputs.py
--rw-r--r--   0        0        0     1935 2023-07-20 04:00:09.992243 qcio-0.4.0/qcio/models/outputs_base.py
--rw-r--r--   0        0        0     4569 2023-07-20 04:00:09.992243 qcio-0.4.0/qcio/qcel.py
--rw-r--r--   0        0        0      838 2023-07-20 04:00:09.992243 qcio-0.4.0/qcio/utils.py
--rw-r--r--   0        0        0     1673 1970-01-01 00:00:00.000000 qcio-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1079 2023-07-20 22:32:15.701838 qcio-0.4.1/LICENSE
+-rw-r--r--   0        0        0      898 2023-07-20 22:32:15.701838 qcio-0.4.1/README.md
+-rw-r--r--   0        0        0     1246 2023-07-20 22:32:15.701838 qcio-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0      573 2023-07-20 22:32:15.701838 qcio-0.4.1/qcio/__init__.py
+-rw-r--r--   0        0        0       89 2023-07-20 22:32:15.701838 qcio-0.4.1/qcio/constants.py
+-rw-r--r--   0        0        0      483 2023-07-20 22:32:15.701838 qcio-0.4.1/qcio/helper_types.py
+-rw-r--r--   0        0        0      235 2023-07-20 22:32:15.701838 qcio-0.4.1/qcio/models/__init__.py
+-rw-r--r--   0        0        0     9738 2023-07-20 22:32:15.701838 qcio-0.4.1/qcio/models/base_models.py
+-rw-r--r--   0        0        0     3082 2023-07-20 22:32:15.701838 qcio-0.4.1/qcio/models/inputs.py
+-rw-r--r--   0        0        0     2286 2023-07-20 22:32:15.701838 qcio-0.4.1/qcio/models/inputs_base.py
+-rw-r--r--   0        0        0     8302 2023-07-20 22:32:15.701838 qcio-0.4.1/qcio/models/molecule.py
+-rw-r--r--   0        0        0     8693 2023-07-20 22:32:15.701838 qcio-0.4.1/qcio/models/outputs.py
+-rw-r--r--   0        0        0     1935 2023-07-20 22:32:15.701838 qcio-0.4.1/qcio/models/outputs_base.py
+-rw-r--r--   0        0        0     4569 2023-07-20 22:32:15.701838 qcio-0.4.1/qcio/qcel.py
+-rw-r--r--   0        0        0      838 2023-07-20 22:32:15.701838 qcio-0.4.1/qcio/utils.py
+-rw-r--r--   0        0        0     1673 1970-01-01 00:00:00.000000 qcio-0.4.1/PKG-INFO
```

### Comparing `qcio-0.4.0/LICENSE` & `qcio-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `qcio-0.4.0/README.md` & `qcio-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `qcio-0.4.0/pyproject.toml` & `qcio-0.4.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "qcio"
-version = "0.4.0"
+version = "0.4.1"
 description = "Beautiful and user friendly data structures for quantum chemistry."
 authors = ["Colton Hicks <github@coltonhicks.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `qcio-0.4.0/qcio/__init__.py` & `qcio-0.4.1/qcio/__init__.py`

 * *Files identical despite different names*

### Comparing `qcio-0.4.0/qcio/models/base_models.py` & `qcio-0.4.1/qcio/models/base_models.py`

 * *Files identical despite different names*

### Comparing `qcio-0.4.0/qcio/models/inputs.py` & `qcio-0.4.1/qcio/models/inputs.py`

 * *Files identical despite different names*

### Comparing `qcio-0.4.0/qcio/models/inputs_base.py` & `qcio-0.4.1/qcio/models/inputs_base.py`

 * *Files identical despite different names*

### Comparing `qcio-0.4.0/qcio/models/molecule.py` & `qcio-0.4.1/qcio/models/molecule.py`

 * *Files identical despite different names*

### Comparing `qcio-0.4.0/qcio/models/outputs.py` & `qcio-0.4.1/qcio/models/outputs.py`

 * *Files 5% similar despite different names*

```diff
@@ -172,17 +172,20 @@
         final_molecule: The final, optimized molecule.
         trajectory: The SinglePointOutput objects for each step of the optimization.
     """
 
     trajectory: List[SinglePointOutput] = []
 
     @property
-    def final_molecule(self) -> Molecule:
+    def final_molecule(self) -> Optional[Molecule]:
         """The final molecule in the optimization."""
-        return self.trajectory[-1].input_data.molecule
+        try:
+            return self.trajectory[-1].input_data.molecule
+        except IndexError:  # Empty trajectory
+            return None
 
     @property
     def energies(self) -> List[float]:
         """The energies for each step of the optimization."""
         # or 0.0 covers null case for mypy
         return [output.results.energy or 0.0 for output in self.trajectory]
```

### Comparing `qcio-0.4.0/qcio/models/outputs_base.py` & `qcio-0.4.1/qcio/models/outputs_base.py`

 * *Files identical despite different names*

### Comparing `qcio-0.4.0/qcio/qcel.py` & `qcio-0.4.1/qcio/qcel.py`

 * *Files identical despite different names*

### Comparing `qcio-0.4.0/qcio/utils.py` & `qcio-0.4.1/qcio/utils.py`

 * *Files identical despite different names*

### Comparing `qcio-0.4.0/PKG-INFO` & `qcio-0.4.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qcio
-Version: 0.4.0
+Version: 0.4.1
 Summary: Beautiful and user friendly data structures for quantum chemistry.
 License: MIT
 Author: Colton Hicks
 Author-email: github@coltonhicks.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

