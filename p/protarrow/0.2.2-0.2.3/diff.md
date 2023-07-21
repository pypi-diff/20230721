# Comparing `tmp/protarrow-0.2.2.tar.gz` & `tmp/protarrow-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "protarrow-0.2.2.tar", max compression
+gzip compressed data, was "protarrow-0.2.3.tar", max compression
```

## Comparing `protarrow-0.2.2.tar` & `protarrow-0.2.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    10140 2023-07-17 11:15:48.575371 protarrow-0.2.2/LICENSE
--rw-r--r--   0        0        0     3022 2023-07-17 11:15:48.575371 protarrow-0.2.2/README.md
--rw-r--r--   0        0        0      754 2023-07-17 11:16:10.655362 protarrow-0.2.2/protarrow/__init__.py
--rw-r--r--   0        0        0    19834 2023-07-17 11:15:48.579371 protarrow-0.2.2/protarrow/arrow_to_proto.py
--rw-r--r--   0        0        0     7596 2023-07-17 11:15:48.579371 protarrow-0.2.2/protarrow/cast_to_proto.py
--rw-r--r--   0        0        0     1236 2023-07-17 11:15:48.579371 protarrow-0.2.2/protarrow/common.py
--rw-r--r--   0        0        0     4621 2023-07-17 11:15:48.579371 protarrow-0.2.2/protarrow/message_extractor.py
--rw-r--r--   0        0        0    18960 2023-07-17 11:15:48.579371 protarrow-0.2.2/protarrow/proto_to_arrow.py
--rw-r--r--   0        0        0     1859 2023-07-17 11:16:10.655362 protarrow-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     4084 1970-01-01 00:00:00.000000 protarrow-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0    10140 2023-07-21 17:02:38.710180 protarrow-0.2.3/LICENSE
+-rw-r--r--   0        0        0     3022 2023-07-21 17:02:38.710180 protarrow-0.2.3/README.md
+-rw-r--r--   0        0        0      754 2023-07-21 17:03:05.622141 protarrow-0.2.3/protarrow/__init__.py
+-rw-r--r--   0        0        0    19758 2023-07-21 17:02:38.714180 protarrow-0.2.3/protarrow/arrow_to_proto.py
+-rw-r--r--   0        0        0     7534 2023-07-21 17:02:38.714180 protarrow-0.2.3/protarrow/cast_to_proto.py
+-rw-r--r--   0        0        0     1236 2023-07-21 17:02:38.714180 protarrow-0.2.3/protarrow/common.py
+-rw-r--r--   0        0        0     4621 2023-07-21 17:02:38.714180 protarrow-0.2.3/protarrow/message_extractor.py
+-rw-r--r--   0        0        0    18482 2023-07-21 17:02:38.714180 protarrow-0.2.3/protarrow/proto_to_arrow.py
+-rw-r--r--   0        0        0     1859 2023-07-21 17:03:05.618140 protarrow-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     4084 1970-01-01 00:00:00.000000 protarrow-0.2.3/PKG-INFO
```

### Comparing `protarrow-0.2.2/LICENSE` & `protarrow-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `protarrow-0.2.2/README.md` & `protarrow-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `protarrow-0.2.2/protarrow/__init__.py` & `protarrow-0.2.3/protarrow/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from protarrow.proto_to_arrow import (
     message_type_to_schema,
     message_type_to_struct_type,
     messages_to_record_batch,
     messages_to_table,
 )
 
-__version__ = "0.2.2"
+__version__ = "0.2.3"
 __all__ = [
     "MessageExtractor",
     "ProtarrowConfig",
     "cast_record_batch",
     "cast_struct_array",
     "cast_table",
     "message_type_to_schema",
```

### Comparing `protarrow-0.2.2/protarrow/arrow_to_proto.py` & `protarrow-0.2.3/protarrow/arrow_to_proto.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,45 +62,45 @@
     if date == datetime.date.min:
         return Date()
     else:
         return Date(year=date.year, month=date.month, day=date.day)
 
 
 def _time_64_ns_scalar_to_proto(scalar: pa.Time64Scalar) -> TimeOfDay:
-    total_nanos = scalar.cast(pa.int64()).as_py()
+    total_nanos = scalar.value
     return TimeOfDay(
         nanos=total_nanos % 1_000_000_000,
         seconds=(total_nanos // 1_000_000_000) % 60,
         minutes=(total_nanos // 60_000_000_000) % 60,
         hours=(total_nanos // 3600_000_000_000),
     )
 
 
 def _time_64_us_scalar_to_proto(scalar: pa.Time64Scalar) -> TimeOfDay:
-    total_us = scalar.cast(pa.int64()).as_py()
+    total_us = scalar.value
     return TimeOfDay(
         nanos=(total_us % 1_000_000) * 1_000,
         seconds=(total_us // 1_000_000) % 60,
         minutes=(total_us // 60_000_000) % 60,
         hours=(total_us // 3600_000_000),
     )
 
 
 def _time_32_ms_scalar_to_proto(scalar: pa.Time32Scalar) -> TimeOfDay:
-    total_ms = scalar.cast(pa.int32()).as_py()
+    total_ms = scalar.value
     return TimeOfDay(
         nanos=(total_ms % 1_000) * 1_000_000,
         seconds=(total_ms // 1_000) % 60,
         minutes=(total_ms // 60_000) % 60,
         hours=(total_ms // 3600_000),
     )
 
 
 def _time_32_s_scalar_to_proto(scalar: pa.Time32Scalar) -> TimeOfDay:
-    total_s = scalar.cast(pa.int32()).as_py()
+    total_s = scalar.value
     return TimeOfDay(
         nanos=0,
         seconds=(total_s // 1) % 60,
         minutes=(total_s // 60) % 60,
         hours=(total_s // 3600),
     )
```

### Comparing `protarrow-0.2.2/protarrow/cast_to_proto.py` & `protarrow-0.2.3/protarrow/cast_to_proto.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,15 +125,18 @@
     source_array: Optional[pa.Array],
     num_rows: int,
     config: ProtarrowConfig,
 ) -> Tuple[pa.Array, pa.Field]:
     expected_field = field_descriptor_to_field(field_descriptor, config)
     if source_array is not None:
         casted_array = _cast_array(source_array, field_descriptor, config)
-    elif expected_field.nullable:
+    elif (
+        field_descriptor.type == FieldDescriptor.TYPE_MESSAGE
+        and field_descriptor.label != FieldDescriptor.LABEL_REPEATED
+    ):
         casted_array = pa.nulls(num_rows, expected_field.type)
         if pa.types.is_struct(expected_field.type):
             casted_array = cast_struct_array(
                 casted_array, field_descriptor.message_type, config
             )
     else:
         default_value = (
@@ -184,20 +187,16 @@
             struct_array.field(field_index) if field_index >= 0 else None,
             len(struct_array),
             config,
         )
         arrays.append(array)
         fields.append(field)
     if len(arrays) == 0:
-        # TODO: remove when this is fixed
-        #  https://github.com/apache/arrow/issues/15109
         return pa.StructArray.from_arrays(
-            arrays=[pa.nulls(len(struct_array))],
-            fields=[pa.field("null", pa.null())],
-            mask=struct_array.is_null(),
+            arrays=[], fields=[], mask=struct_array.is_null()
         ).cast(pa.struct([]))
     else:
         return pa.StructArray.from_arrays(
             arrays=arrays, fields=fields, mask=struct_array.is_null()
         )
```

### Comparing `protarrow-0.2.2/protarrow/common.py` & `protarrow-0.2.3/protarrow/common.py`

 * *Files identical despite different names*

### Comparing `protarrow-0.2.2/protarrow/message_extractor.py` & `protarrow-0.2.3/protarrow/message_extractor.py`

 * *Files identical despite different names*

### Comparing `protarrow-0.2.2/protarrow/proto_to_arrow.py` & `protarrow-0.2.3/protarrow/proto_to_arrow.py`

 * *Files 1% similar despite different names*

```diff
@@ -507,33 +507,22 @@
         fields.append(
             pa.field(
                 field_descriptor.name,
                 array.type,
                 nullable=_proto_field_nullable(field_descriptor, config),
             )
         )
-    if len(arrays) == 0:
-        # TODO: remove when this is fixed
-        #  https://github.com/apache/arrow/issues/15109
-        size = len(validity_mask) if validity_mask else len(messages)
-        return pa.StructArray.from_arrays(
-            arrays=[pa.nulls(size, pa.null())],
-            fields=[pa.field("null", pa.null())],
-            mask=pc.invert(pa.array(validity_mask, pa.bool_()))
-            if validity_mask
-            else None,
-        ).cast(pa.struct([]))
-    else:
-        return pa.StructArray.from_arrays(
-            arrays=arrays,
-            fields=fields,
-            mask=pc.invert(pa.array(validity_mask, pa.bool_()))
-            if validity_mask
-            else None,
-        )
+
+    return pa.StructArray.from_arrays(
+        arrays=arrays,
+        fields=fields,
+        mask=pc.invert(pa.array(validity_mask, pa.bool_()))
+        if validity_mask is not None
+        else pa.repeat(False, len(messages)),
+    )
 
 
 def messages_to_record_batch(
     messages: Iterable[M],
     message_type: Type[M],
     config: ProtarrowConfig = ProtarrowConfig(),
 ):
```

### Comparing `protarrow-0.2.2/pyproject.toml` & `protarrow-0.2.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 [tool.poetry]
 name = "protarrow"
-version = "0.2.2"
+version = "0.2.3"
 description = "Convert from protobuf to arrow and back"
 authors = ["Tradewell Tech <engineering@tradewelltech.co>"]
 maintainers = ["0x26res <0x26res@gmail.com>"]
 packages = [
     { include = "protarrow" }
 ]
 readme = "README.md"
```

### Comparing `protarrow-0.2.2/PKG-INFO` & `protarrow-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: protarrow
-Version: 0.2.2
+Version: 0.2.3
 Summary: Convert from protobuf to arrow and back
 Home-page: https://github.com/tradewelltech/protarrow
 License: Apache-2.0
 Keywords: apache-arrow,protobuf,data
 Author: Tradewell Tech
 Author-email: engineering@tradewelltech.co
 Maintainer: 0x26res
```

