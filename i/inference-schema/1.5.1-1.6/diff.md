# Comparing `tmp/inference_schema-1.5.1-py3-none-any.whl.zip` & `tmp/inference_schema-1.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 21100 bytes, number of entries: 18
+Zip file size: 21210 bytes, number of entries: 18
 -rw-rw-rw-  2.0 fat      183 b- defN 22-Feb-04 18:09 inference_schema/__init__.py
 -rw-rw-rw-  2.0 fat      307 b- defN 22-Oct-28 16:24 inference_schema/_constants.py
--rw-rw-rw-  2.0 fat    12705 b- defN 22-Apr-13 16:08 inference_schema/schema_decorators.py
+-rw-rw-rw-  2.0 fat    12629 b- defN 23-Jul-21 21:43 inference_schema/schema_decorators.py
 -rw-rw-rw-  2.0 fat     4189 b- defN 22-Oct-28 16:24 inference_schema/schema_util.py
 -rw-rw-rw-  2.0 fat      421 b- defN 22-Feb-04 18:09 inference_schema/parameter_types/__init__.py
 -rw-rw-rw-  2.0 fat      642 b- defN 22-Feb-04 18:09 inference_schema/parameter_types/_constants.py
 -rw-rw-rw-  2.0 fat     4001 b- defN 22-Feb-04 18:09 inference_schema/parameter_types/_swagger_from_dtype.py
 -rw-rw-rw-  2.0 fat     4446 b- defN 22-Oct-28 16:24 inference_schema/parameter_types/_util.py
 -rw-rw-rw-  2.0 fat     5229 b- defN 22-Apr-14 14:38 inference_schema/parameter_types/abstract_parameter_type.py
 -rw-rw-rw-  2.0 fat     6953 b- defN 22-Feb-04 18:09 inference_schema/parameter_types/numpy_parameter_type.py
--rw-rw-rw-  2.0 fat     8835 b- defN 23-Jan-05 19:37 inference_schema/parameter_types/pandas_parameter_type.py
+-rw-rw-rw-  2.0 fat     9372 b- defN 23-Jul-21 21:43 inference_schema/parameter_types/pandas_parameter_type.py
 -rw-rw-rw-  2.0 fat     9647 b- defN 22-Feb-04 18:09 inference_schema/parameter_types/spark_parameter_type.py
 -rw-rw-rw-  2.0 fat     3456 b- defN 22-Mar-28 20:14 inference_schema/parameter_types/standard_py_parameter_type.py
--rw-rw-rw-  2.0 fat     1183 b- defN 23-Jan-05 19:44 inference_schema-1.5.1.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat     2450 b- defN 23-Jan-05 19:44 inference_schema-1.5.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jan-05 19:44 inference_schema-1.5.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       17 b- defN 23-Jan-05 19:44 inference_schema-1.5.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1775 b- defN 23-Jan-05 19:44 inference_schema-1.5.1.dist-info/RECORD
-18 files, 66531 bytes uncompressed, 18090 bytes compressed:  72.8%
+-rw-rw-rw-  2.0 fat     1183 b- defN 23-Jul-21 21:44 inference_schema-1.6.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat     2398 b- defN 23-Jul-21 21:44 inference_schema-1.6.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-21 21:44 inference_schema-1.6.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       17 b- defN 23-Jul-21 21:44 inference_schema-1.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1765 b- defN 23-Jul-21 21:44 inference_schema-1.6.dist-info/RECORD
+18 files, 66930 bytes uncompressed, 18220 bytes compressed:  72.8%
```

## zipnote {}

```diff
@@ -33,23 +33,23 @@
 
 Filename: inference_schema/parameter_types/spark_parameter_type.py
 Comment: 
 
 Filename: inference_schema/parameter_types/standard_py_parameter_type.py
 Comment: 
 
-Filename: inference_schema-1.5.1.dist-info/LICENSE.txt
+Filename: inference_schema-1.6.dist-info/LICENSE.txt
 Comment: 
 
-Filename: inference_schema-1.5.1.dist-info/METADATA
+Filename: inference_schema-1.6.dist-info/METADATA
 Comment: 
 
-Filename: inference_schema-1.5.1.dist-info/WHEEL
+Filename: inference_schema-1.6.dist-info/WHEEL
 Comment: 
 
-Filename: inference_schema-1.5.1.dist-info/top_level.txt
+Filename: inference_schema-1.6.dist-info/top_level.txt
 Comment: 
 
-Filename: inference_schema-1.5.1.dist-info/RECORD
+Filename: inference_schema-1.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## inference_schema/schema_decorators.py

```diff
@@ -323,15 +323,15 @@
         if not isinstance(input_data, dict):
             raise ValueError("Invalid input data type to parse. Expected: {0} but got {1}".format(
                 sample_data_type, type(input_data)))
         sample_data_type_map = param_type.sample_data_type_map
         # parameters other than subclass of AbstractParameterType will not be handled
         for k, v in sample_data_type_map.items():
             if k not in input_data.keys():
-                raise Exception('Invalid input. Expected: key "{0}" in "{1}"'.format(k, param_name))
+                continue
             input_data[k] = _deserialize_input_argument(input_data[k], v, k)
     elif sample_data_type in (list, tuple):
         sample_data_type_list = param_type.sample_data_type_list
         if not isinstance(input_data, list) and not isinstance(input_data, tuple):
             raise ValueError("Invalid input data type to parse. Expected: {0} but got {1}".format(
                 sample_data_type, type(input_data)))
         # OpenAPI 2.x does not support mixed type in array
```

## inference_schema/parameter_types/pandas_parameter_type.py

```diff
@@ -87,15 +87,23 @@
 
         if self.enforce_column_type:
             sample_input_column_types = self.sample_input.dtypes.to_dict()
             converted_types = {x: sample_input_column_types.get(x, object) for x in data_frame.columns}
             for column_name, column_type in converted_types.items():
                 if str(column_type).startswith('timedelta'):
                     data_frame[column_name] = pd.to_timedelta(data_frame[column_name])
-            data_frame = data_frame.astype(dtype=converted_types)
+
+            try:
+                data_frame = data_frame.astype(dtype=converted_types)
+            except TypeError as e:
+                if 'Cannot use .astype to convert from timezone-naive dtype to timezone-aware dtype' in e.args[0]:
+                    raise Exception("As of pandas 2.0, can no longer convert from timezone-naive dtype to "
+                                    "timezone-aware dtype. Please make sure that the provided input data matches "
+                                    "the expected timezone handling of the provided deployment sample.") from e
+                raise
 
         if self.enforce_shape:
             expected_shape = self.sample_input.shape
             parsed_data_dims = len(data_frame.shape)
             expected_dims = len(expected_shape)
             if parsed_data_dims != expected_dims:
                 raise ValueError(
```

## Comparing `inference_schema-1.5.1.dist-info/LICENSE.txt` & `inference_schema-1.6.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `inference_schema-1.5.1.dist-info/METADATA` & `inference_schema-1.6.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inference-schema
-Version: 1.5.1
+Version: 1.6
 Summary: This package is intended to provide a uniform schema for common machine learning applications, as well as a set of decorators that can be used to aid in web based ML prediction applications.
 Author: Microsoft Corp
 License: MIT License        
             Copyright (c) Microsoft Corporation. All rights reserved.        
             Permission is hereby granted, free of charge, to any person obtaining a copy
             of this software and associated documentation files (the "Software"), to deal
             in the Software without restriction, including without limitation the rights
@@ -20,15 +20,14 @@
             LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
             OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
             SOFTWARE        
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7,<3.11
 License-File: LICENSE.txt
 Requires-Dist: python-dateutil (>=2.5.3)
 Requires-Dist: pytz (>=2017.2)
```

## Comparing `inference_schema-1.5.1.dist-info/RECORD` & `inference_schema-1.6.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 inference_schema/__init__.py,sha256=JlCCObuOLZyNhIZlsoL51KtFxiY4xKIIzIRDBcdeu6Y,183
 inference_schema/_constants.py,sha256=oyCqVS9IFFLmBZQ5pggUdPm1pmBHY35uYNpeOCKz_jw,307
-inference_schema/schema_decorators.py,sha256=PQlvvF6m0rNXdA0C1kfRIcaK74YzPvdPkY35wRur0Gk,12705
+inference_schema/schema_decorators.py,sha256=SJcP-GMpfAy2PCs-QD7nQhPo4n8CLQFKwpNCVxsgWBo,12629
 inference_schema/schema_util.py,sha256=bWp6OSbeRcpmLWx1pmV8DD68ZPTOhoct1YUhx1eMf0M,4189
 inference_schema/parameter_types/__init__.py,sha256=ZZqhUutuAxCsQyDODYilPdx1miZx02jNdWmHVPhJt2k,421
 inference_schema/parameter_types/_constants.py,sha256=qnr_V7yT5xZJNNtt8_EqN1FfLyTqMUvJPJnbHo1_qt0,642
 inference_schema/parameter_types/_swagger_from_dtype.py,sha256=WWYVGo6-KiGoPg0CMmM3RBa_WTtbS33lTV9PS-dQ5T0,4001
 inference_schema/parameter_types/_util.py,sha256=vXKbnsTbVBpxrhBXpIHycKxYzBl1PE04dtWtQLY6G6M,4446
 inference_schema/parameter_types/abstract_parameter_type.py,sha256=qkdLkYgXlIHFA-NxGOTkYmG6FK-qdFgPenn9HMJrTzo,5229
 inference_schema/parameter_types/numpy_parameter_type.py,sha256=goBx3Vzti-9jlKvMPn55t4SS5FF416-tq-ZGEpAjb_Q,6953
-inference_schema/parameter_types/pandas_parameter_type.py,sha256=sJfMzhPV1sLArOfYG9d8yurZoE0_9EQldK4XE7Clw_U,8835
+inference_schema/parameter_types/pandas_parameter_type.py,sha256=wPYgg7IlbJq6VAQB6wRQ_fj2Wvxfpu3RcJ9gpmMVjh4,9372
 inference_schema/parameter_types/spark_parameter_type.py,sha256=vVmYWZFRSNCReouZiS1cGoR30NGu5OJlPyvQ_flgY2g,9647
 inference_schema/parameter_types/standard_py_parameter_type.py,sha256=DO5Ty02A0D5zjt4ODodxw6WeOA7r2QyfK-NswN9yOzI,3456
-inference_schema-1.5.1.dist-info/LICENSE.txt,sha256=3qkmU0GCkALiwjpzcjk-su1uJghftiPzikugr4M_MKY,1183
-inference_schema-1.5.1.dist-info/METADATA,sha256=5WJS2acplSyBuRKFVN9FlOGNBCG0m2qjnxNZZgudLrg,2450
-inference_schema-1.5.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-inference_schema-1.5.1.dist-info/top_level.txt,sha256=VppQqI390J43UCHv4CcDtEGPp8EktkSEi5Q80wWYq9M,17
-inference_schema-1.5.1.dist-info/RECORD,,
+inference_schema-1.6.dist-info/LICENSE.txt,sha256=3qkmU0GCkALiwjpzcjk-su1uJghftiPzikugr4M_MKY,1183
+inference_schema-1.6.dist-info/METADATA,sha256=U_3fCacPs26KXGknxtnmbfk5atECXHNK1HkK-0bP104,2398
+inference_schema-1.6.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+inference_schema-1.6.dist-info/top_level.txt,sha256=VppQqI390J43UCHv4CcDtEGPp8EktkSEi5Q80wWYq9M,17
+inference_schema-1.6.dist-info/RECORD,,
```

