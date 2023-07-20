# Comparing `tmp/vegafusion-1.4.0rc2.tar.gz` & `tmp/vegafusion-1.4.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vegafusion-1.4.0rc2.tar", last modified: Wed Jul  5 12:36:00 2023, max compression
+gzip compressed data, was "vegafusion-1.4.0rc3.tar", last modified: Thu Jul 20 16:58:31 2023, max compression
```

## Comparing `vegafusion-1.4.0rc2.tar` & `vegafusion-1.4.0rc3.tar`

### file list

```diff
@@ -1,38 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:36:00.862041 vegafusion-1.4.0rc2/
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-07-05 12:34:56.000000 vegafusion-1.4.0rc2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-07-05 12:36:00.862041 vegafusion-1.4.0rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-05 12:34:56.000000 vegafusion-1.4.0rc2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-05 12:34:56.000000 vegafusion-1.4.0rc2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-05 12:36:00.862041 vegafusion-1.4.0rc2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 12:34:56.000000 vegafusion-1.4.0rc2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:36:00.858041 vegafusion-1.4.0rc2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-05 12:34:56.000000 vegafusion-1.4.0rc2/tests/test_conext_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    18632 2023-07-05 12:34:56.000000 vegafusion-1.4.0rc2/tests/test_input_utc.py
--rw-r--r--   0 runner    (1001) docker     (123)    43916 2023-07-05 12:34:56.000000 vegafusion-1.4.0rc2/tests/test_pretransform.py
--rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-07-05 12:34:56.000000 vegafusion-1.4.0rc2/tests/test_pretransform_specs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-05 12:34:56.000000 vegafusion-1.4.0rc2/tests/test_row_limit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-07-05 12:34:56.000000 vegafusion-1.4.0rc2/tests/test_save.py
--rw-r--r--   0 runner    (1001) docker     (123)    14048 2023-07-05 12:34:56.000000 vegafusion-1.4.0rc2/tests/test_transformed_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-07-05 12:34:56.000000 vegafusion-1.4.0rc2/tests/test_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:36:00.858041 vegafusion-1.4.0rc2/vegafusion/
--rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-07-05 12:34:56.000000 vegafusion-1.4.0rc2/vegafusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-05 12:34:56.000000 vegafusion-1.4.0rc2/vegafusion/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-07-05 12:34:56.000000 vegafusion-1.4.0rc2/vegafusion/compilers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:36:00.862041 vegafusion-1.4.0rc2/vegafusion/connection/
--rw-r--r--   0 runner    (1001) docker     (123)     5518 2023-07-05 12:34:56.000000 vegafusion-1.4.0rc2/vegafusion/connection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13181 2023-07-05 12:34:56.000000 vegafusion-1.4.0rc2/vegafusion/connection/duckdb.py
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-05 12:34:56.000000 vegafusion-1.4.0rc2/vegafusion/embed.py
--rw-r--r--   0 runner    (1001) docker     (123)     7992 2023-07-05 12:34:56.000000 vegafusion-1.4.0rc2/vegafusion/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-05 12:34:56.000000 vegafusion-1.4.0rc2/vegafusion/jupyter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-07-05 12:34:56.000000 vegafusion-1.4.0rc2/vegafusion/local_tz.py
--rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-07-05 12:34:56.000000 vegafusion-1.4.0rc2/vegafusion/renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)    23299 2023-07-05 12:34:56.000000 vegafusion-1.4.0rc2/vegafusion/runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     4267 2023-07-05 12:34:56.000000 vegafusion-1.4.0rc2/vegafusion/save.py
--rw-r--r--   0 runner    (1001) docker     (123)     8485 2023-07-05 12:34:56.000000 vegafusion-1.4.0rc2/vegafusion/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-05 12:34:56.000000 vegafusion-1.4.0rc2/vegafusion/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:36:00.862041 vegafusion-1.4.0rc2/vegafusion.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-07-05 12:36:00.000000 vegafusion-1.4.0rc2/vegafusion.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-05 12:36:00.000000 vegafusion-1.4.0rc2/vegafusion.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 12:36:00.000000 vegafusion-1.4.0rc2/vegafusion.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-05 12:36:00.000000 vegafusion-1.4.0rc2/vegafusion.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-05 12:36:00.000000 vegafusion-1.4.0rc2/vegafusion.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:58:31.633995 vegafusion-1.4.0rc3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-07-20 16:57:29.000000 vegafusion-1.4.0rc3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-07-20 16:58:31.633995 vegafusion-1.4.0rc3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-20 16:57:29.000000 vegafusion-1.4.0rc3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-20 16:57:29.000000 vegafusion-1.4.0rc3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-07-20 16:58:31.633995 vegafusion-1.4.0rc3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 16:57:29.000000 vegafusion-1.4.0rc3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:58:31.629995 vegafusion-1.4.0rc3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-20 16:57:29.000000 vegafusion-1.4.0rc3/tests/test_conext_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18632 2023-07-20 16:57:29.000000 vegafusion-1.4.0rc3/tests/test_input_utc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43916 2023-07-20 16:57:29.000000 vegafusion-1.4.0rc3/tests/test_pretransform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-07-20 16:57:29.000000 vegafusion-1.4.0rc3/tests/test_pretransform_specs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-20 16:57:29.000000 vegafusion-1.4.0rc3/tests/test_row_limit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-07-20 16:57:29.000000 vegafusion-1.4.0rc3/tests/test_save.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14048 2023-07-20 16:57:29.000000 vegafusion-1.4.0rc3/tests/test_transformed_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-07-20 16:57:29.000000 vegafusion-1.4.0rc3/tests/test_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:58:31.633995 vegafusion-1.4.0rc3/vegafusion/
+-rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-07-20 16:57:29.000000 vegafusion-1.4.0rc3/vegafusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-20 16:57:29.000000 vegafusion-1.4.0rc3/vegafusion/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-07-20 16:57:29.000000 vegafusion-1.4.0rc3/vegafusion/compilers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:58:31.633995 vegafusion-1.4.0rc3/vegafusion/connection/
+-rw-r--r--   0 runner    (1001) docker     (123)     5518 2023-07-20 16:57:29.000000 vegafusion-1.4.0rc3/vegafusion/connection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13181 2023-07-20 16:57:29.000000 vegafusion-1.4.0rc3/vegafusion/connection/duckdb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:58:31.633995 vegafusion-1.4.0rc3/vegafusion/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-20 16:57:29.000000 vegafusion-1.4.0rc3/vegafusion/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5890 2023-07-20 16:57:29.000000 vegafusion-1.4.0rc3/vegafusion/dataset/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-07-20 16:57:29.000000 vegafusion-1.4.0rc3/vegafusion/dataset/duckdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-07-20 16:57:29.000000 vegafusion-1.4.0rc3/vegafusion/dataset/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-20 16:57:29.000000 vegafusion-1.4.0rc3/vegafusion/embed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7992 2023-07-20 16:57:29.000000 vegafusion-1.4.0rc3/vegafusion/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-20 16:57:29.000000 vegafusion-1.4.0rc3/vegafusion/jupyter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-07-20 16:57:29.000000 vegafusion-1.4.0rc3/vegafusion/local_tz.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:58:31.633995 vegafusion-1.4.0rc3/vegafusion/proto/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 16:57:29.000000 vegafusion-1.4.0rc3/vegafusion/proto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63111 2023-07-20 16:57:29.000000 vegafusion-1.4.0rc3/vegafusion/proto/datafusion_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-07-20 16:57:29.000000 vegafusion-1.4.0rc3/vegafusion/renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23574 2023-07-20 16:57:29.000000 vegafusion-1.4.0rc3/vegafusion/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4267 2023-07-20 16:57:29.000000 vegafusion-1.4.0rc3/vegafusion/save.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8485 2023-07-20 16:57:29.000000 vegafusion-1.4.0rc3/vegafusion/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-20 16:57:29.000000 vegafusion-1.4.0rc3/vegafusion/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:58:31.633995 vegafusion-1.4.0rc3/vegafusion.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-07-20 16:58:31.000000 vegafusion-1.4.0rc3/vegafusion.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-20 16:58:31.000000 vegafusion-1.4.0rc3/vegafusion.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 16:58:31.000000 vegafusion-1.4.0rc3/vegafusion.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-20 16:58:31.000000 vegafusion-1.4.0rc3/vegafusion.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-20 16:58:31.000000 vegafusion-1.4.0rc3/vegafusion.egg-info/top_level.txt
```

### Comparing `vegafusion-1.4.0rc2/LICENSE.txt` & `vegafusion-1.4.0rc3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vegafusion-1.4.0rc2/PKG-INFO` & `vegafusion-1.4.0rc3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vegafusion
-Version: 1.4.0rc2
+Version: 1.4.0rc3
 Summary: Core tools for using VegaFusion from Python
 License: BSD-3-Clause
 Keywords: vega,altair,vegafusion,arrow
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `vegafusion-1.4.0rc2/README.md` & `vegafusion-1.4.0rc3/README.md`

 * *Files identical despite different names*

### Comparing `vegafusion-1.4.0rc2/setup.cfg` & `vegafusion-1.4.0rc3/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [bdist_wheel]
 universal = 0
 
 [metadata]
 name = vegafusion
 description = Core tools for using VegaFusion from Python
-version = 1.4.0-rc2
+version = 1.4.0-rc3
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = vega, altair, vegafusion, arrow
 license = BSD-3-Clause
 license_file = LICENSE.txt
 python = "^3.7"
 homepage = "https://vegafusion.io"
@@ -27,17 +27,18 @@
 python_requires = >=3.7
 include_package_data = True
 install_requires = 
 	altair>=4.2.0
 	pyarrow>=5
 	pandas
 	psutil
+	protobuf
 
 [options.extras_require]
 embed = 
-	vegafusion-python-embed==1.4.0-rc2
+	vegafusion-python-embed==1.4.0-rc3
 	vl-convert-python>=0.7.0
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `vegafusion-1.4.0rc2/tests/test_conext_manager.py` & `vegafusion-1.4.0rc3/tests/test_conext_manager.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.4.0rc2/tests/test_input_utc.py` & `vegafusion-1.4.0rc3/tests/test_input_utc.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.4.0rc2/tests/test_pretransform.py` & `vegafusion-1.4.0rc3/tests/test_pretransform.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.4.0rc2/tests/test_pretransform_specs.py` & `vegafusion-1.4.0rc3/tests/test_pretransform_specs.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,15 +83,15 @@
     (transformed, _) = vf.runtime.pre_transform_spec(spec, local_tz)
     img_duckdb = imread(BytesIO(vega_to_png(transformed)))
 
     # Compare images
     assert img_datafusion.shape == img_duckdb.shape, "Size mismatch between datafusion and duckdb connections"
     similarity = ssim(img_datafusion, img_duckdb, channel_axis=2)
     print(similarity)
-    assert similarity >= 0.999, f"Similarity failed between datafusion and duckdb connections"
+    assert similarity >= 0.998, f"Similarity failed between datafusion and duckdb connections"
 
 
 def test_pretransform_extract():
     spec_file = spec_dir / "vegalite" / "rect_binned_heatmap.vg.json"
     spec = json.loads(spec_file.read_text("utf8"))
 
     vf.runtime.set_connection("datafusion")
```

### Comparing `vegafusion-1.4.0rc2/tests/test_row_limit.py` & `vegafusion-1.4.0rc3/tests/test_row_limit.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.4.0rc2/tests/test_save.py` & `vegafusion-1.4.0rc3/tests/test_save.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.4.0rc2/tests/test_transformed_data.py` & `vegafusion-1.4.0rc3/tests/test_transformed_data.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.4.0rc2/tests/test_transformer.py` & `vegafusion-1.4.0rc3/tests/test_transformer.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.4.0rc2/vegafusion/__init__.py` & `vegafusion-1.4.0rc3/vegafusion/__init__.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.4.0rc2/vegafusion/compilers.py` & `vegafusion-1.4.0rc3/vegafusion/compilers.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.4.0rc2/vegafusion/connection/__init__.py` & `vegafusion-1.4.0rc3/vegafusion/connection/__init__.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.4.0rc2/vegafusion/connection/duckdb.py` & `vegafusion-1.4.0rc3/vegafusion/connection/duckdb.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.4.0rc2/vegafusion/evaluation.py` & `vegafusion-1.4.0rc3/vegafusion/evaluation.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.4.0rc2/vegafusion/local_tz.py` & `vegafusion-1.4.0rc3/vegafusion/local_tz.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.4.0rc2/vegafusion/renderer.py` & `vegafusion-1.4.0rc3/vegafusion/renderer.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.4.0rc2/vegafusion/runtime.py` & `vegafusion-1.4.0rc3/vegafusion/runtime.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import json
 
 import pandas as pd
 import psutil
 import pyarrow as pa
 from typing import Union
 from .connection import SqlConnection
+from .dataset import SqlDataset, DataFrameDataset
 from .transformer import import_pyarrow_interchange, to_arrow_table
 from .local_tz import get_local_tz
 
 try:
     from duckdb import DuckDBPyConnection
 except ImportError:
     DuckDBPyConnection = None
@@ -124,55 +125,59 @@
     def process_request_bytes(self, request):
         if self._grpc_channel:
             return self.grpc_query(request)
         else:
             # No grpc channel, get or initialize an embedded runtime
             return self.embedded_runtime.process_request_bytes(request)
 
-    def _arrowify_or_register_inline_datasets(self, inline_datasets=None):
+    def _import_or_register_inline_datasets(self, inline_datasets=None):
         from .transformer import to_arrow_ipc_bytes, arrow_table_to_ipc_bytes
         inline_datasets = inline_datasets or dict()
-        inline_arrow_datasets = dict()
+        imported_inline_datasets = dict()
         for name, value in inline_datasets.items():
-            if isinstance(value, pa.Table):
+            if isinstance(value, SqlDataset):
+                imported_inline_datasets[name] = value
+            elif isinstance(value, DataFrameDataset):
+                imported_inline_datasets[name] = value
+            elif isinstance(value, pa.Table):
                 if self._connection is not None:
                     try:
                         # Try registering Arrow Table if supported
                         self._connection.register_arrow(name, value, temporary=True)
                         continue
                     except ValueError:
                         pass
 
-                inline_arrow_datasets[name] = value
+                imported_inline_datasets[name] = value
             elif isinstance(value, pd.DataFrame):
                 if self._connection is not None:
                     try:
                         # Try registering DataFrame if supported
                         self._connection.register_pandas(name, value, temporary=True)
                         continue
                     except ValueError:
                         pass
 
-                inline_arrow_datasets[name] = to_arrow_table(value)
+                imported_inline_datasets[name] = to_arrow_table(value)
             elif hasattr(value, "__dataframe__"):
                 pi = import_pyarrow_interchange()
                 value = pi.from_dataframe(value)
                 if self._connection is not None:
                     try:
                         # Try registering Arrow Table if supported
                         self._connection.register_arrow(name, value, temporary=True)
                         continue
                     except ValueError:
                         pass
 
-                inline_arrow_datasets[name] = value
+                imported_inline_datasets[name] = value
             else:
                 raise ValueError(f"Unsupported DataFrame type: {type(value)}")
 
-        return inline_arrow_datasets
+        return imported_inline_datasets
 
     def pre_transform_spec(
         self,
         spec,
         local_tz=None,
         default_input_tz=None,
         row_limit=None,
@@ -227,27 +232,27 @@
                     'Unsupported': No transforms in the provided Vega specification were
                         eligible for pre-transforming
         """
         if self._grpc_channel:
             raise ValueError("pre_transform_spec not yet supported over gRPC")
         else:
             local_tz = local_tz or get_local_tz()
-            inline_arrow_dataset = self._arrowify_or_register_inline_datasets(inline_datasets)
+            imported_inline_dataset = self._import_or_register_inline_datasets(inline_datasets)
 
             # Parse input keep signals and datasets
             keep_signals = parse_variables(keep_signals)
             keep_datasets = parse_variables(keep_datasets)
             try:
                 new_spec, warnings = self.embedded_runtime.pre_transform_spec(
                     spec,
                     local_tz=local_tz,
                     default_input_tz=default_input_tz,
                     row_limit=row_limit,
                     preserve_interactivity=preserve_interactivity,
-                    inline_datasets=inline_arrow_dataset,
+                    inline_datasets=imported_inline_dataset,
                     keep_signals=keep_signals,
                     keep_datasets=keep_datasets,
                 )
             finally:
                 # Clean up temporary tables
                 if self._connection is not None:
                     self._connection.unregister_temporary_tables()
@@ -296,15 +301,15 @@
         else:
             local_tz = local_tz or get_local_tz()
 
             # Build input variables
             pre_tx_vars = parse_variables(datasets)
 
             # Serialize inline datasets
-            inline_arrow_dataset = self._arrowify_or_register_inline_datasets(inline_datasets)
+            inline_arrow_dataset = self._import_or_register_inline_datasets(inline_datasets)
             try:
                 values, warnings = self.embedded_runtime.pre_transform_datasets(
                     spec,
                     pre_tx_vars,
                     local_tz=local_tz,
                     default_input_tz=default_input_tz,
                     row_limit=row_limit,
@@ -384,15 +389,15 @@
                     'Planner': Planner warning
         """
         if self._grpc_channel:
             raise ValueError("pre_transform_spec not yet supported over gRPC")
         else:
             local_tz = local_tz or get_local_tz()
 
-            inline_arrow_dataset = self._arrowify_or_register_inline_datasets(inline_datasets)
+            inline_arrow_dataset = self._import_or_register_inline_datasets(inline_datasets)
             try:
                 new_spec, datasets, warnings = self.embedded_runtime.pre_transform_extract(
                     spec,
                     local_tz=local_tz,
                     default_input_tz=default_input_tz,
                     preserve_interactivity=preserve_interactivity,
                     inline_datasets=inline_arrow_dataset
```

### Comparing `vegafusion-1.4.0rc2/vegafusion/save.py` & `vegafusion-1.4.0rc3/vegafusion/save.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.4.0rc2/vegafusion/transformer.py` & `vegafusion-1.4.0rc3/vegafusion/transformer.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.4.0rc2/vegafusion/utils.py` & `vegafusion-1.4.0rc3/vegafusion/utils.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.4.0rc2/vegafusion.egg-info/PKG-INFO` & `vegafusion-1.4.0rc3/vegafusion.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vegafusion
-Version: 1.4.0rc2
+Version: 1.4.0rc3
 Summary: Core tools for using VegaFusion from Python
 License: BSD-3-Clause
 Keywords: vega,altair,vegafusion,arrow
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `vegafusion-1.4.0rc2/vegafusion.egg-info/SOURCES.txt` & `vegafusion-1.4.0rc3/vegafusion.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -25,8 +25,14 @@
 vegafusion/utils.py
 vegafusion.egg-info/PKG-INFO
 vegafusion.egg-info/SOURCES.txt
 vegafusion.egg-info/dependency_links.txt
 vegafusion.egg-info/requires.txt
 vegafusion.egg-info/top_level.txt
 vegafusion/connection/__init__.py
-vegafusion/connection/duckdb.py
+vegafusion/connection/duckdb.py
+vegafusion/dataset/__init__.py
+vegafusion/dataset/dataframe.py
+vegafusion/dataset/duckdb.py
+vegafusion/dataset/sql.py
+vegafusion/proto/__init__.py
+vegafusion/proto/datafusion_pb2.py
```

