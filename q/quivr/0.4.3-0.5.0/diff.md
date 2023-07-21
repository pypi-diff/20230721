# Comparing `tmp/quivr-0.4.3.tar.gz` & `tmp/quivr-0.5.0.tar.gz`

## Comparing `quivr-0.4.3.tar` & `quivr-0.5.0.tar`

### file list

```diff
@@ -1,18 +1,20 @@
--rw-r--r--   0        0        0     2148 2020-02-02 00:00:00.000000 quivr-0.4.3/quivr/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 quivr-0.4.3/quivr/__version__.py
--rw-r--r--   0        0        0     3984 2020-02-02 00:00:00.000000 quivr-0.4.3/quivr/attributes.py
--rw-r--r--   0        0        0    34132 2020-02-02 00:00:00.000000 quivr-0.4.3/quivr/columns.py
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 quivr-0.4.3/quivr/concat.py
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 quivr-0.4.3/quivr/defragment.py
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 quivr-0.4.3/quivr/errors.py
--rw-r--r--   0        0        0     2337 2020-02-02 00:00:00.000000 quivr-0.4.3/quivr/indexing.py
--rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 quivr-0.4.3/quivr/matrix.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 quivr-0.4.3/quivr/py.typed
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 quivr-0.4.3/quivr/schemagraph.py
--rw-r--r--   0        0        0    31283 2020-02-02 00:00:00.000000 quivr-0.4.3/quivr/tables.py
--rw-r--r--   0        0        0     5810 2020-02-02 00:00:00.000000 quivr-0.4.3/quivr/validators.py
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 quivr-0.4.3/.gitignore
--rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 quivr-0.4.3/LICENSE
--rw-r--r--   0        0        0    10737 2020-02-02 00:00:00.000000 quivr-0.4.3/README.md
--rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 quivr-0.4.3/pyproject.toml
--rw-r--r--   0        0        0    11174 2020-02-02 00:00:00.000000 quivr-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0     2588 2020-02-02 00:00:00.000000 quivr-0.5.0/quivr/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 quivr-0.5.0/quivr/__version__.py
+-rw-r--r--   0        0        0     5277 2020-02-02 00:00:00.000000 quivr-0.5.0/quivr/attributes.py
+-rw-r--r--   0        0        0    39655 2020-02-02 00:00:00.000000 quivr-0.5.0/quivr/columns.py
+-rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 quivr-0.5.0/quivr/concat.py
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 quivr-0.5.0/quivr/defragment.py
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 quivr-0.5.0/quivr/errors.py
+-rw-r--r--   0        0        0     2071 2020-02-02 00:00:00.000000 quivr-0.5.0/quivr/indexing.py
+-rw-r--r--   0        0        0    13144 2020-02-02 00:00:00.000000 quivr-0.5.0/quivr/linkage.py
+-rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 quivr-0.5.0/quivr/matrix.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 quivr-0.5.0/quivr/py.typed
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 quivr-0.5.0/quivr/schemagraph.py
+-rw-r--r--   0        0        0    38124 2020-02-02 00:00:00.000000 quivr-0.5.0/quivr/tables.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 quivr-0.5.0/quivr/typevars.py
+-rw-r--r--   0        0        0     7082 2020-02-02 00:00:00.000000 quivr-0.5.0/quivr/validators.py
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 quivr-0.5.0/.gitignore
+-rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 quivr-0.5.0/LICENSE
+-rw-r--r--   0        0        0    10737 2020-02-02 00:00:00.000000 quivr-0.5.0/README.md
+-rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 quivr-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0    11432 2020-02-02 00:00:00.000000 quivr-0.5.0/PKG-INFO
```

### Comparing `quivr-0.4.3/quivr/__init__.py` & `quivr-0.5.0/quivr/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,35 @@
 from .__version__ import __version__
 from .attributes import FloatAttribute, IntAttribute, StringAttribute
 from .columns import (
     BinaryColumn,
+    BooleanColumn,
+    Byteslike,
     Column,
     Date32Column,
     Date64Column,
     Decimal128Column,
     Decimal256Column,
     DictionaryColumn,
     DurationColumn,
+    FixedSizeBinaryColumn,
+    FixedSizeListColumn,
     Float16Column,
     Float32Column,
     Float64Column,
     Int8Column,
     Int16Column,
     Int32Column,
     Int64Column,
     LargeBinaryColumn,
     LargeListColumn,
     LargeStringColumn,
     ListColumn,
     MapColumn,
+    MetadataDict,
     MonthDayNanoIntervalColumn,
     NullColumn,
     RunEndEncodedColumn,
     StringColumn,
     StructColumn,
     SubTableColumn,
     Time32Column,
@@ -35,17 +40,18 @@
     UInt32Column,
     UInt64Column,
 )
 from .concat import concatenate
 from .defragment import defragment
 from .errors import InvariantViolatedError, TableFragmentedError, ValidationError
 from .indexing import StringIndex
+from .linkage import Linkage, MultiKeyLinkage
 from .matrix import MatrixArray, MatrixExtensionType
-from .tables import Table
-from .validators import and_, eq, ge, gt, is_in, le, lt
+from .tables import AnyTable, AttributeValueType, DataSourceType, Table
+from .validators import Validator, and_, eq, ge, gt, is_in, le, lt
 
 __all__ = [
     "__version__",
     "Table",
     "MatrixArray",
     "MatrixExtensionType",
     "concatenate",
@@ -56,17 +62,20 @@
     "Int16Column",
     "Int32Column",
     "Int64Column",
     "UInt8Column",
     "UInt16Column",
     "UInt32Column",
     "UInt64Column",
+    "FixedSizeBinaryColumn",
+    "FixedSizeListColumn",
     "Float16Column",
     "Float32Column",
     "Float64Column",
+    "BooleanColumn",
     "StringColumn",
     "LargeBinaryColumn",
     "LargeStringColumn",
     "Date32Column",
     "Date64Column",
     "TimestampColumn",
     "Time32Column",
@@ -89,12 +98,20 @@
     "lt",
     "le",
     "gt",
     "ge",
     "eq",
     "and_",
     "is_in",
+    "Validator",
     "StringAttribute",
     "IntAttribute",
     "FloatAttribute",
     "defragment",
+    "AttributeValueType",
+    "DataSourceType",
+    "AnyTable",
+    "MetadataDict",
+    "Byteslike",
+    "Linkage",
+    "MultiKeyLinkage",
 ]
```

### Comparing `quivr-0.4.3/quivr/attributes.py` & `quivr-0.5.0/quivr/attributes.py`

 * *Files 23% similar despite different names*

```diff
@@ -70,14 +70,21 @@
         """
         Convert a string to a value. Used for CSV reading.
         """
         raise NotImplementedError
 
 
 class StringAttribute(Attribute[str]):
+    """StringAttribute represents a string which is stored as UTF-8
+    bytes in Table metadata.
+
+    :param default: The default value for this attribute. If no default is provided,
+        then the attribute must be set whenever constructing a table that uses it.
+    """
+
     _type = str
 
     def __init__(self, default: Optional[str] = None):
         super().__init__(default=default)
 
     def to_bytes(self, value: str) -> bytes:
         return value.encode("utf8")
@@ -89,14 +96,26 @@
         return value
 
     def from_string(self, raw: str) -> str:
         return raw
 
 
 class IntAttribute(Attribute[int]):
+    """IntAttribute represents an integer which is stored as little-endian
+    bytes in Table metadata.
+
+    The number of bytes used to store the integer must be specified
+    up-front, as well as whether it is signed.
+
+    :param default: The default value for this attribute. If no default is provided,
+        then the attribute must be set whenever constructing a table that uses it.
+    :param nbytes: The number of bytes to use to store the integer. Must be 1, 2, 4 or 8.
+    :param signed: Whether the integer is signed or unsigned.
+    """
+
     _type = int
 
     def __init__(self, default: Optional[int] = None, nbytes: int = 8, signed: bool = True):
         self.nbytes = nbytes
         self.signed = signed
         super().__init__(default=default)
 
@@ -110,14 +129,26 @@
         return str(value)
 
     def from_string(self, raw: str) -> int:
         return int(raw)
 
 
 class FloatAttribute(Attribute[float]):
+    """
+    FloatAttribute represents a floating-point number which is stored as little-endian
+    bytes in Table metadata.
+
+    The number of bytes used to store the float must be specified
+    up-front.
+
+    :param default: The default value for this attribute. If no default is provided,
+        then the attribute must be set whenever constructing a table that uses it.
+    :param nbytes: The number of bytes to use to store the float. Must be 2, 4 or 8.
+    """
+
     _type = float
 
     def __init__(self, default: Optional[float] = None, nbytes: int = 8):
         if nbytes == 8:
             self._struct_fmt = "<d"
         elif nbytes == 4:
             self._struct_fmt = "<f"
```

### Comparing `quivr-0.4.3/quivr/columns.py` & `quivr-0.5.0/quivr/columns.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,30 +8,43 @@
     from typing import TypeAlias
 
 if sys.version_info < (3, 11):
     from typing_extensions import Self
 else:
     from typing import Self
 
-from typing import TYPE_CHECKING, Generic, Optional, TypeVar, Union, overload
+from typing import Dict, Generic, Optional, TypeVar, Union, overload
 
 import pyarrow as pa
 
-from . import validators
+from . import tables, validators
 
-if TYPE_CHECKING:
-    from .tables import Table
-
-Byteslike: TypeAlias = Union[bytes, bytearray, memoryview, str]
-MetadataDict: TypeAlias = dict[Byteslike, Byteslike]
+Byteslike: TypeAlias = Union[bytes, str]
+MetadataDict: TypeAlias = Dict[Byteslike, Byteslike]
 
 
 class Column:
-    """
-    A Column is an accessor for data in a Table, and also a descriptor for the Table's structure.
+    """A Column is an accessor for data in a Table, and also a
+    descriptor for the Table's structure.
+
+    This is a base class for all column types. It is not intended to
+    be used directly; instead, use on of its subclasses.
+
+    Columns implement the descriptor protocol, so they should be used
+    as class attributes on a Table subclass.
+
+    :param dtype: The pyarrow data type of the column.
+    :param nullable: Whether the column can contain null values.
+    :param metadata: A dictionary of metadata to attach to the column.
+    :param validator: A validator to use when setting the column.
+
+    :ivar dtype: The pyarrow data type of the column.
+    :ivar nullable: Whether the column can contain null values.
+    :ivar metadata: A dictionary of metadata to attach to the column.
+    :ivar validator: A validator to use when setting the column.
     """
 
     def __init__(
         self,
         dtype: pa.DataType,
         nullable: bool = True,
         metadata: Optional[MetadataDict] = None,
@@ -43,56 +56,80 @@
         self.validator = validator
 
     @overload
     def __get__(self, obj: None, objtype: type) -> Self:
         ...
 
     @overload
-    def __get__(self, obj: Table, objtype: type) -> pa.Array:
+    def __get__(self, obj: tables.Table, objtype: type) -> pa.Array:
         ...
 
-    def __get__(self, obj: Union[Table, None], objtype: type) -> Union[Self, pa.Array]:
+    def __get__(self, obj: Union[tables.Table, None], objtype: type) -> Union[Self, pa.Array]:
+        """
+
+        Gets the Column object from a Table class, or the associated data from a Table instance.
+
+        This method is part of the `descriptor protocol <https://docs.python.org/3/howto/descriptor.html>`_.
+
+        """
         if obj is None:
             return self
         return obj.table.column(self.name)
 
-    def __set__(self, obj: Table, value: pa.Array) -> None:
+    def __set__(self, obj: tables.Table, value: pa.Array) -> None:
+        """
+        Sets the data for this column on a Table instance.
+
+        This method is part of the `descriptor protocol <https://docs.python.org/3/howto/descriptor.html>`_.
+        """
         idx = obj.table.schema.get_field_index(self.name)
         obj.table = obj.table.set_column(idx, self.pyarrow_field(), [value])
 
     def __set_name__(self, owner: type, name: str) -> None:
+        """
+        Sets the name of the column.
+
+        This method is part of the `descriptor protocol <https://docs.python.org/3/howto/descriptor.html>`_.
+        """
         self.name = name
 
     def pyarrow_field(self) -> pa.Field:
+        """
+        Returns a pyarrow Field object for this column.
+        """
         return pa.field(self.name, self.dtype, self.nullable, self.metadata)
 
 
-T = TypeVar("T", bound="Table")
+T = TypeVar("T", bound=tables.Table)
 
 
 class SubTableColumn(Column, Generic[T]):
     """
     A column which represents an embedded Quivr table.
+
+    :param table_type: The type of the table to embed.
+    :param nullable: Whether the column can contain null values.
+    :param metadata: A dictionary of metadata to attach to the column.
     """
 
     def __init__(self, table_type: type[T], nullable: bool = True, metadata: Optional[MetadataDict] = None):
         self.table_type = table_type
         self.schema = table_type.schema
         dtype = pa.struct(table_type.schema)
         super().__init__(dtype, nullable=nullable, metadata=metadata)
 
     @overload
     def __get__(self, obj: None, objtype: type) -> Self:
         ...
 
     @overload
-    def __get__(self, obj: Table, objtype: type) -> T:
+    def __get__(self, obj: tables.Table, objtype: type) -> T:
         ...
 
-    def __get__(self, obj: Optional["Table"], objtype: type) -> Union[Self, T]:
+    def __get__(self, obj: Optional[tables.Table], objtype: type) -> Union[Self, T]:
         if obj is None:
             return self
         array = obj.table.column(self.name)
 
         metadata = self.metadata
         if metadata is None:
             metadata = {}
@@ -108,28 +145,28 @@
     """
     A column for storing 8-bit integers.
     """
 
     def __init__(
         self,
         nullable: bool = True,
-        validator: Optional[validators.Validator] = None,
         metadata: Optional[MetadataDict] = None,
+        validator: Optional[validators.Validator] = None,
     ):
         super().__init__(pa.int8(), nullable=nullable, metadata=metadata, validator=validator)
 
     @overload
     def __get__(self, obj: None, objtype: type) -> Self:
         ...
 
     @overload
-    def __get__(self, obj: "Table", objtype: type) -> pa.Int8Array:
+    def __get__(self, obj: tables.Table, objtype: type) -> pa.Int8Array:
         ...
 
-    def __get__(self, obj: Optional["Table"], objtype: type) -> Union[Self, pa.Int8Array]:
+    def __get__(self, obj: Optional[tables.Table], objtype: type) -> Union[Self, pa.Int8Array]:
         if obj is None:
             return self
         return obj.table[self.name].combine_chunks()
 
 
 class Int16Column(Column):
     """
@@ -145,156 +182,180 @@
         super().__init__(pa.int16(), nullable=nullable, metadata=metadata, validator=validator)
 
     @overload
     def __get__(self, obj: None, objtype: type) -> Self:
         ...
 
     @overload
-    def __get__(self, obj: "Table", objtype: type) -> pa.Int16Array:
+    def __get__(self, obj: tables.Table, objtype: type) -> pa.Int16Array:
         ...
 
-    def __get__(self, obj: Optional["Table"], objtype: type) -> Union[Self, pa.Int16Array]:
+    def __get__(self, obj: Optional[tables.Table], objtype: type) -> Union[Self, pa.Int16Array]:
         if obj is None:
             return self
         return obj.table[self.name].combine_chunks()
 
 
 class Int32Column(Column):
+    """
+    A column for storing 32-bit integers.
+    """
+
     def __init__(
         self,
         nullable: bool = True,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
     ):
         super().__init__(pa.int32(), nullable=nullable, metadata=metadata, validator=validator)
 
     @overload
     def __get__(self, obj: None, objtype: type) -> Self:
         ...
 
     @overload
-    def __get__(self, obj: "Table", objtype: type) -> pa.Int32Array:
+    def __get__(self, obj: tables.Table, objtype: type) -> pa.Int32Array:
         ...
 
-    def __get__(self, obj: Optional["Table"], objtype: type) -> Union[Self, pa.Int32Array]:
+    def __get__(self, obj: Optional[tables.Table], objtype: type) -> Union[Self, pa.Int32Array]:
         if obj is None:
             return self
         return obj.table[self.name].combine_chunks()
 
 
 class Int64Column(Column):
+    """
+    A column for storing 64-bit integers.
+    """
+
     def __init__(
         self,
         nullable: bool = True,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
     ):
         super().__init__(pa.int64(), nullable=nullable, metadata=metadata, validator=validator)
 
     @overload
     def __get__(self, obj: None, objtype: type) -> Self:
         ...
 
     @overload
-    def __get__(self, obj: "Table", objtype: type) -> pa.Int64Array:
+    def __get__(self, obj: tables.Table, objtype: type) -> pa.Int64Array:
         ...
 
-    def __get__(self, obj: Optional["Table"], objtype: type) -> Union[Self, pa.Int64Array]:
+    def __get__(self, obj: Optional[tables.Table], objtype: type) -> Union[Self, pa.Int64Array]:
         if obj is None:
             return self
         return obj.table[self.name].combine_chunks()
 
 
 class UInt8Column(Column):
+    """
+    A column for storing 8-bit unsigned integers.
+    """
+
     def __init__(
         self,
         nullable: bool = True,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
     ):
         super().__init__(pa.uint8(), nullable=nullable, metadata=metadata, validator=validator)
 
     @overload
     def __get__(self, obj: None, objtype: type) -> Self:
         ...
 
     @overload
-    def __get__(self, obj: "Table", objtype: type) -> pa.UInt8Array:
+    def __get__(self, obj: tables.Table, objtype: type) -> pa.UInt8Array:
         ...
 
-    def __get__(self, obj: Optional["Table"], objtype: type) -> Union[Self, pa.UInt8Array]:
+    def __get__(self, obj: Optional[tables.Table], objtype: type) -> Union[Self, pa.UInt8Array]:
         if obj is None:
             return self
         return obj.table[self.name].combine_chunks()
 
 
 class UInt16Column(Column):
+    """
+    A column for storing 16-bit unsigned integers.
+    """
+
     def __init__(
         self,
         nullable: bool = True,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
     ):
         super().__init__(pa.uint16(), nullable=nullable, metadata=metadata, validator=validator)
 
     @overload
     def __get__(self, obj: None, objtype: type) -> Self:
         ...
 
     @overload
-    def __get__(self, obj: "Table", objtype: type) -> pa.UInt16Array:
+    def __get__(self, obj: tables.Table, objtype: type) -> pa.UInt16Array:
         ...
 
-    def __get__(self, obj: Optional["Table"], objtype: type) -> Union[Self, pa.UInt16Array]:
+    def __get__(self, obj: Optional[tables.Table], objtype: type) -> Union[Self, pa.UInt16Array]:
         if obj is None:
             return self
         return obj.table[self.name].combine_chunks()
 
 
 class UInt32Column(Column):
+    """
+    A column for storing 32-bit unsigned integers.
+    """
+
     def __init__(
         self,
         nullable: bool = True,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
     ):
         super().__init__(pa.uint32(), nullable=nullable, metadata=metadata, validator=validator)
 
     @overload
     def __get__(self, obj: None, objtype: type) -> Self:
         ...
 
     @overload
-    def __get__(self, obj: "Table", objtype: type) -> pa.UInt32Array:
+    def __get__(self, obj: tables.Table, objtype: type) -> pa.UInt32Array:
         ...
 
-    def __get__(self, obj: Optional["Table"], objtype: type) -> Union[Self, pa.UInt32Array]:
+    def __get__(self, obj: Optional[tables.Table], objtype: type) -> Union[Self, pa.UInt32Array]:
         if obj is None:
             return self
         return obj.table[self.name].combine_chunks()
 
 
 class UInt64Column(Column):
+    """
+    A column for storing 64-bit unsigned integers.
+    """
+
     def __init__(
         self,
         nullable: bool = True,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
     ):
         super().__init__(pa.uint64(), nullable=nullable, metadata=metadata, validator=validator)
 
     @overload
     def __get__(self, obj: None, objtype: type) -> Self:
         ...
 
     @overload
-    def __get__(self, obj: "Table", objtype: type) -> pa.UInt64Array:
+    def __get__(self, obj: tables.Table, objtype: type) -> pa.UInt64Array:
         ...
 
-    def __get__(self, obj: Optional["Table"], objtype: type) -> Union[Self, pa.UInt64Array]:
+    def __get__(self, obj: Optional[tables.Table], objtype: type) -> Union[Self, pa.UInt64Array]:
         if obj is None:
             return self
         return obj.table[self.name].combine_chunks()
 
 
 class Float16Column(Column):
     """
@@ -310,18 +371,18 @@
         super().__init__(pa.float16(), nullable=nullable, metadata=metadata, validator=validator)
 
     @overload
     def __get__(self, obj: None, objtype: type) -> Self:
         ...
 
     @overload
-    def __get__(self, obj: "Table", objtype: type) -> pa.lib.HalfFloatArray:
+    def __get__(self, obj: tables.Table, objtype: type) -> pa.lib.HalfFloatArray:
         ...
 
-    def __get__(self, obj: Optional["Table"], objtype: type) -> Union[Self, pa.lib.HalfFloatArray]:
+    def __get__(self, obj: Optional[tables.Table], objtype: type) -> Union[Self, pa.lib.HalfFloatArray]:
         if obj is None:
             return self
         return obj.table[self.name].combine_chunks()
 
 
 class Float32Column(Column):
     """
@@ -337,18 +398,18 @@
         super().__init__(pa.float32(), nullable=nullable, metadata=metadata, validator=validator)
 
     @overload
     def __get__(self, obj: None, objtype: type) -> Self:
         ...
 
     @overload
-    def __get__(self, obj: "Table", objtype: type) -> pa.lib.FloatArray:
+    def __get__(self, obj: tables.Table, objtype: type) -> pa.lib.FloatArray:
         ...
 
-    def __get__(self, obj: Optional["Table"], objtype: type) -> Union[Self, pa.lib.FloatArray]:
+    def __get__(self, obj: Optional[tables.Table], objtype: type) -> Union[Self, pa.lib.FloatArray]:
         if obj is None:
             return self
         return obj.table[self.name].combine_chunks()
 
 
 class Float64Column(Column):
     """
@@ -364,18 +425,43 @@
         super().__init__(pa.float64(), nullable=nullable, metadata=metadata, validator=validator)
 
     @overload
     def __get__(self, obj: None, objtype: type) -> Self:
         ...
 
     @overload
-    def __get__(self, obj: "Table", objtype: type) -> pa.lib.DoubleArray:
+    def __get__(self, obj: tables.Table, objtype: type) -> pa.lib.DoubleArray:
         ...
 
-    def __get__(self, obj: Optional["Table"], objtype: type) -> Union[Self, pa.lib.DoubleArray]:
+    def __get__(self, obj: Optional[tables.Table], objtype: type) -> Union[Self, pa.lib.DoubleArray]:
+        if obj is None:
+            return self
+        return obj.table[self.name].combine_chunks()
+
+
+class BooleanColumn(Column):
+    """A column for storing booleans."""
+
+    def __init__(
+        self,
+        nullable: bool = True,
+        metadata: Optional[MetadataDict] = None,
+        validator: Optional[validators.Validator] = None,
+    ):
+        super().__init__(pa.bool_(), nullable=nullable, metadata=metadata, validator=validator)
+
+    @overload
+    def __get__(self, obj: None, objtype: type) -> Self:
+        ...
+
+    @overload
+    def __get__(self, obj: tables.Table, objtype: type) -> pa.BooleanArray:
+        ...
+
+    def __get__(self, obj: Optional[tables.Table], objtype: type) -> Union[pa.BooleanArray, Self]:
         if obj is None:
             return self
         return obj.table[self.name].combine_chunks()
 
 
 class StringColumn(Column):
     """A column for storing strings.
@@ -395,26 +481,26 @@
         super().__init__(pa.string(), nullable=nullable, metadata=metadata, validator=validator)
 
     @overload
     def __get__(self, obj: None, objtype: type) -> Self:
         ...
 
     @overload
-    def __get__(self, obj: Table, objtype: type) -> pa.StringArray:
+    def __get__(self, obj: tables.Table, objtype: type) -> pa.StringArray:
         ...
 
-    def __get__(self, obj: Optional[Table], objtype: type) -> Union[pa.StringArray, Self]:
+    def __get__(self, obj: Optional[tables.Table], objtype: type) -> Union[pa.StringArray, Self]:
         if obj is None:
             return self
         return obj.table[self.name].combine_chunks()
 
 
 class LargeBinaryColumn(Column):
-    """
-    A column for storing large binary objects. Large binary data is stored in
+    r"""
+    A column for storing large binary objects (over 2\ :sup:`31` bytes long). Large binary data is stored in
     variable-length chunks.
     """
 
     def __init__(
         self,
         nullable: bool = True,
         metadata: Optional[MetadataDict] = None,
@@ -423,26 +509,26 @@
         super().__init__(pa.large_binary(), nullable=nullable, metadata=metadata, validator=validator)
 
     @overload
     def __get__(self, obj: None, objtype: type) -> Self:
         ...
 
     @overload
-    def __get__(self, obj: "Table", objtype: type) -> pa.LargeBinaryArray:
+    def __get__(self, obj: tables.Table, objtype: type) -> pa.LargeBinaryArray:
         ...
 
-    def __get__(self, obj: Optional["Table"], objtype: type) -> Union[Self, pa.LargeBinaryArray]:
+    def __get__(self, obj: Optional[tables.Table], objtype: type) -> Union[Self, pa.LargeBinaryArray]:
         if obj is None:
             return self
         return obj.table[self.name].combine_chunks()
 
 
 class LargeStringColumn(Column):
-    """
-    A column for storing large strings. Large string data is stored in
+    r"""
+    A column for storing large strings (over 2\ :sup:`31` bytes long). Large string data is stored in
     variable-length chunks.
     """
 
     def __init__(
         self,
         nullable: bool = True,
         metadata: Optional[MetadataDict] = None,
@@ -451,18 +537,18 @@
         super().__init__(pa.large_string(), nullable=nullable, metadata=metadata, validator=validator)
 
     @overload
     def __get__(self, obj: None, objtype: type) -> Self:
         ...
 
     @overload
-    def __get__(self, obj: "Table", objtype: type) -> pa.LargeStringArray:
+    def __get__(self, obj: tables.Table, objtype: type) -> pa.LargeStringArray:
         ...
 
-    def __get__(self, obj: Optional["Table"], objtype: type) -> Union[Self, pa.LargeStringArray]:
+    def __get__(self, obj: Optional[tables.Table], objtype: type) -> Union[Self, pa.LargeStringArray]:
         if obj is None:
             return self
         return obj.table[self.name].combine_chunks()
 
 
 class Date32Column(Column):
     """A column for storing dates.
@@ -481,18 +567,18 @@
         super().__init__(pa.date32(), nullable=nullable, metadata=metadata, validator=validator)
 
     @overload
     def __get__(self, obj: None, objtype: type) -> Self:
         ...
 
     @overload
-    def __get__(self, obj: "Table", objtype: type) -> pa.Date32Array:
+    def __get__(self, obj: tables.Table, objtype: type) -> pa.Date32Array:
         ...
 
-    def __get__(self, obj: Optional["Table"], objtype: type) -> Union[Self, pa.Date32Array]:
+    def __get__(self, obj: Optional[tables.Table], objtype: type) -> Union[Self, pa.Date32Array]:
         if obj is None:
             return self
         return obj.table[self.name].combine_chunks()
 
 
 class Date64Column(Column):
     """A column for storing dates.
@@ -511,18 +597,18 @@
         super().__init__(pa.date64(), nullable=nullable, metadata=metadata, validator=validator)
 
     @overload
     def __get__(self, obj: None, objtype: type) -> Self:
         ...
 
     @overload
-    def __get__(self, obj: "Table", objtype: type) -> pa.Date64Array:
+    def __get__(self, obj: tables.Table, objtype: type) -> pa.Date64Array:
         ...
 
-    def __get__(self, obj: Optional["Table"], objtype: type) -> Union[Self, pa.Date64Array]:
+    def __get__(self, obj: Optional[tables.Table], objtype: type) -> Union[Self, pa.Date64Array]:
         if obj is None:
             return self
         return obj.table[self.name].combine_chunks()
 
 
 class TimestampColumn(Column):
     """A column for storing timestamps.
@@ -535,14 +621,21 @@
 
     Internally, a timestamp is a 64-bit integer which represents time
     since 1970-01-01 00:00:00 UTC (the UNIX epoch), and is optionally
     annotated with a timezone.
 
     Timestamp values do not include any leap seconds (in other words,
     all days are considered 86,400 seconds long).
+
+    :param unit: The unit of time to use for the timestamp. Valid
+        values are "s", "ms", "us", and "ns".
+    :param tz: An optional timezone to associate with the timestamp.
+    :param nullable: Whether the column can contain null values.
+    :param metadata: Optional metadata to associate with the column.
+    :param validator: An optional validator to apply to the column.
     """
 
     def __init__(
         self,
         unit: str,
         tz: Optional[str] = None,
         nullable: bool = True,
@@ -552,32 +645,37 @@
         super().__init__(pa.timestamp(unit, tz), nullable=nullable, metadata=metadata, validator=validator)
 
     @overload
     def __get__(self, obj: None, objtype: type) -> Self:
         ...
 
     @overload
-    def __get__(self, obj: "Table", objtype: type) -> pa.TimestampArray:
+    def __get__(self, obj: tables.Table, objtype: type) -> pa.TimestampArray:
         ...
 
-    def __get__(self, obj: Optional["Table"], objtype: type) -> Union[Self, pa.TimestampArray]:
+    def __get__(self, obj: Optional[tables.Table], objtype: type) -> Union[Self, pa.TimestampArray]:
         if obj is None:
             return self
         return obj.table[self.name].combine_chunks()
 
 
 class Time32Column(Column):
     """
     A column for storing time values.
 
     Time data can be stored in one of two units for this 32-bit type:
         - seconds
         - milliseconds
 
     Internally, a time32 value is a 32-bit integer which an elapsed time since midnight.
+
+    :param unit: The unit of time to use for the time. Valid values are "s" and "ms".
+    :param nullable: Whether the column can contain null values.
+    :param metadata: Optional metadata to associate with the column.
+    :param validator: An optional validator to apply to the column.
     """
 
     def __init__(
         self,
         unit: str,
         nullable: bool = True,
         metadata: Optional[MetadataDict] = None,
@@ -586,32 +684,37 @@
         super().__init__(pa.time32(unit), nullable=nullable, metadata=metadata, validator=validator)
 
     @overload
     def __get__(self, obj: None, objtype: type) -> Self:
         ...
 
     @overload
-    def __get__(self, obj: "Table", objtype: type) -> pa.Time32Array:
+    def __get__(self, obj: tables.Table, objtype: type) -> pa.Time32Array:
         ...
 
-    def __get__(self, obj: Optional["Table"], objtype: type) -> Union[Self, pa.Time32Array]:
+    def __get__(self, obj: Optional[tables.Table], objtype: type) -> Union[Self, pa.Time32Array]:
         if obj is None:
             return self
         return obj.table[self.name].combine_chunks()
 
 
 class Time64Column(Column):
     """
     A column for storing time values with high precision.
 
     Time data can be stored in one of two units for this 64-bit type:
         - microseconds
         - nanoseconds
 
     Internally, a time64 value is a 64-bit integer which an elapsed time since midnight.
+
+    :param unit: The unit of time to use for the time. Valid values are "us" and "ns".
+    :param nullable: Whether the column can contain null values.
+    :param metadata: Optional metadata to associate with the column.
+    :param validator: An optional validator to apply to the column.
     """
 
     def __init__(
         self,
         unit: str,
         nullable: bool = True,
         metadata: Optional[MetadataDict] = None,
@@ -620,32 +723,32 @@
         super().__init__(pa.time64(unit), nullable=nullable, metadata=metadata, validator=validator)
 
     @overload
     def __get__(self, obj: None, objtype: type) -> Self:
         ...
 
     @overload
-    def __get__(self, obj: "Table", objtype: type) -> pa.Time64Array:
+    def __get__(self, obj: tables.Table, objtype: type) -> pa.Time64Array:
         ...
 
-    def __get__(self, obj: Optional["Table"], objtype: type) -> Union[Self, pa.Time64Array]:
+    def __get__(self, obj: Optional[tables.Table], objtype: type) -> Union[Self, pa.Time64Array]:
         if obj is None:
             return self
         return obj.table[self.name].combine_chunks()
 
 
 class DurationColumn(Column):
     """
-    An absolute length of time unrelated to any calendar artifacts.
-
-    The resolution defaults to millisecond, but can be any of the other
-    supported time unit values (seconds, milliseconds, microseconds,
-    nanoseconds).
+    A column which stores an absolute length of time.
 
-    Internall, a duration value is always represented as an 8-byte integer.
+    Internally, a duration value is always represented as an 64-bit integer.
+    :param unit: The unit of time to use for the duration. Valid values are "s", "ms", "us", and "ns".
+    :param nullable: Whether the column can contain null values.
+    :param metadata: Optional metadata to associate with the column.
+    :param validator: An optional validator to apply to the column.
     """
 
     def __init__(
         self,
         unit: str,
         nullable: bool = True,
         metadata: Optional[MetadataDict] = None,
@@ -654,18 +757,18 @@
         super().__init__(pa.duration(unit), nullable=nullable, metadata=metadata, validator=validator)
 
     @overload
     def __get__(self, obj: None, objtype: type) -> Self:
         ...
 
     @overload
-    def __get__(self, obj: "Table", objtype: type) -> pa.DurationArray:
+    def __get__(self, obj: tables.Table, objtype: type) -> pa.DurationArray:
         ...
 
-    def __get__(self, obj: Optional["Table"], objtype: type) -> Union[Self, pa.DurationArray]:
+    def __get__(self, obj: Optional[tables.Table], objtype: type) -> Union[Self, pa.DurationArray]:
         if obj is None:
             return self
         return obj.table[self.name].combine_chunks()
 
 
 class MonthDayNanoIntervalColumn(Column):
     """A column for storing calendar intervals (an elapsed number of months,
@@ -690,124 +793,155 @@
         )
 
     @overload
     def __get__(self, obj: None, objtype: type) -> Self:
         ...
 
     @overload
-    def __get__(self, obj: "Table", objtype: type) -> pa.MonthDayNanoIntervalArray:
+    def __get__(self, obj: tables.Table, objtype: type) -> pa.MonthDayNanoIntervalArray:
         ...
 
-    def __get__(self, obj: Optional["Table"], objtype: type) -> Union[Self, pa.MonthDayNanoIntervalArray]:
+    def __get__(
+        self, obj: Optional[tables.Table], objtype: type
+    ) -> Union[Self, pa.MonthDayNanoIntervalArray]:
         if obj is None:
             return self
         return obj.table[self.name].combine_chunks()
 
 
 class BinaryColumn(Column):
-    """A column for storing opaque binary data.
+    """A column for storing opaque binary data."""
+
+    def __init__(
+        self,
+        nullable: bool = True,
+        metadata: Optional[MetadataDict] = None,
+        validator: Optional[validators.Validator] = None,
+    ):
+        super().__init__(pa.binary(-1), nullable=nullable, metadata=metadata, validator=validator)
+
+    @overload
+    def __get__(self, obj: None, objtype: type) -> Self:
+        ...
+
+    @overload
+    def __get__(self, obj: tables.Table, objtype: type) -> pa.BinaryArray:
+        ...
 
-    The data can be either variable-length or fixed-length, depending
-    on the 'length' parameter passed in the initializer.
+    def __get__(self, obj: Optional[tables.Table], objtype: type) -> Union[Self, pa.BinaryArray]:
+        if obj is None:
+            return self
+        return obj.table[self.name].combine_chunks()
 
-    If length is -1 (the default) then the data is variable-length. If
-    length is greater than or equal to 0, then the data is
-    fixed-length.
 
+class FixedSizeBinaryColumn(Column):
+    """A column for storing opaque fixed-size binary data.
+
+    :param byte_width: The number of bytes per value.
     """
 
     def __init__(
         self,
-        length: int = -1,
+        byte_width: int,
         nullable: bool = True,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
     ):
-        super().__init__(pa.binary(length), nullable=nullable, metadata=metadata, validator=validator)
+        self.byte_width = byte_width
+        super().__init__(pa.binary(byte_width), nullable=nullable, metadata=metadata, validator=validator)
 
     @overload
     def __get__(self, obj: None, objtype: type) -> Self:
         ...
 
     @overload
-    def __get__(self, obj: "Table", objtype: type) -> pa.BinaryArray:
+    def __get__(self, obj: tables.Table, objtype: type) -> pa.FixedSizeBinaryArray:
         ...
 
-    def __get__(self, obj: Optional["Table"], objtype: type) -> Union[Self, pa.BinaryArray]:
+    def __get__(self, obj: Optional[tables.Table], objtype: type) -> Union[Self, pa.FixedSizeBinaryArray]:
         if obj is None:
             return self
         return obj.table[self.name].combine_chunks()
 
 
 class Decimal128Column(Column):
     """A column for storing arbitrary-precision decimal numbers.
 
     Arrow decimals are fixed-point decimal numbers encoded as a scaled
     integer. The precision is the number of significant digits that the
     decimal type can represent; the scale is the number of digits after
     the decimal point (note the scale can be negative).
 
-    As an example, Decimal128Column(7, 3) can exactly represent the numbers
+    As an example, ``Decimal128Column(7, 3)`` can exactly represent the numbers
     1234.567 and -1234.567 (encoded internally as the 128-bit integers
     1234567 and -1234567, respectively), but neither 12345.67 nor
     123.4567.
 
-    DecimalColumn(5, -3) can exactly represent the number 12345000
+    ``DecimalColumn(5, -3)`` can exactly represent the number 12345000
     (encoded internally as the 128-bit integer 12345), but neither
     123450000 nor 1234500.
 
     If you need a precision higher than 38 significant digits,
-    consider using Decimal256Column.
+    consider using :class:`Decimal256Column`.
 
+    :param precision: The number of significant digits.
+    :param scale: The number of digits after the decimal point.
+    :param nullable: Whether the column can contain nulls.
+    :param metadata: A dictionary of metadata to attach to the column.
     """
 
     def __init__(
         self, precision: int, scale: int, nullable: bool = True, metadata: Optional[MetadataDict] = None
     ):
         super().__init__(pa.decimal128(precision, scale), nullable=nullable, metadata=metadata)
 
     @overload
     def __get__(self, obj: None, objtype: type) -> Self:
         ...
 
     @overload
-    def __get__(self, obj: "Table", objtype: type) -> pa.Decimal128Array:
+    def __get__(self, obj: tables.Table, objtype: type) -> pa.Decimal128Array:
         ...
 
-    def __get__(self, obj: Optional["Table"], objtype: type) -> Union[Self, pa.Decimal128Array]:
+    def __get__(self, obj: Optional[tables.Table], objtype: type) -> Union[Self, pa.Decimal128Array]:
         if obj is None:
             return self
         return obj.table[self.name].combine_chunks()
 
 
 class Decimal256Column(Column):
     """A column for storing arbitrary-precision decimal numbers.
 
     Arrow decimals are fixed-point decimal numbers encoded as a scaled
     integer. The precision is the number of significant digits that the
     decimal type can represent; the scale is the number of digits after
     the decimal point (note the scale can be negative).
 
     Values are stored as 256-bit integers.
+
+    :param precision: The number of significant digits.
+    :param scale: The number of digits after the decimal point.
+    :param nullable: Whether the column can contain nulls.
+    :param metadata: A dictionary of metadata to attach to the column.
     """
 
     def __init__(
         self, precision: int, scale: int, nullable: bool = True, metadata: Optional[MetadataDict] = None
     ):
         super().__init__(pa.decimal256(precision, scale), nullable=nullable, metadata=metadata)
 
     @overload
     def __get__(self, obj: None, objtype: type) -> Self:
         ...
 
     @overload
-    def __get__(self, obj: "Table", objtype: type) -> pa.Decimal256Array:
+    def __get__(self, obj: tables.Table, objtype: type) -> pa.Decimal256Array:
         ...
 
-    def __get__(self, obj: Optional["Table"], objtype: type) -> Union[Self, pa.Decimal256Array]:
+    def __get__(self, obj: Optional[tables.Table], objtype: type) -> Union[Self, pa.Decimal256Array]:
         if obj is None:
             return self
         return obj.table[self.name].combine_chunks()
 
 
 class NullColumn(Column):
     """A column for storing null values.
@@ -826,228 +960,218 @@
         super().__init__(pa.null(), nullable=nullable, metadata=metadata, validator=validator)
 
     @overload
     def __get__(self, obj: None, objtype: type) -> Self:
         ...
 
     @overload
-    def __get__(self, obj: "Table", objtype: type) -> pa.NullArray:
+    def __get__(self, obj: tables.Table, objtype: type) -> pa.NullArray:
         ...
 
-    def __get__(self, obj: Optional["Table"], objtype: type) -> Union[Self, pa.NullArray]:
+    def __get__(self, obj: Optional[tables.Table], objtype: type) -> Union[Self, pa.NullArray]:
         if obj is None:
             return self
         return obj.table[self.name].combine_chunks()
 
 
 # Complex types follow
 
 
 class ListColumn(Column):
-    """A column for storing lists of values.
+    """A column for storing variably-sized lists of values.
 
     The values in the list can be of any type.
 
-    Note that all quivr Tables are storing lists of values, so this
+    Note that all quivr tables.Tables are storing lists of values, so this
     column type is only useful for storing lists of lists.
 
-
-
+    :param value_type: The type of the values in the list.
+    :param nullable: Whether the list can contain null values.
+    :param metadata: A dictionary of metadata to attach to the column.
+    :param validator: A validator to run against the column's values.
     """
 
     def __init__(
         self,
         value_type: Union[pa.DataType, pa.Field, Column],
-        list_size: int = -1,
         nullable: bool = True,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
     ):
-        """
-        Parameters
-        ----------
-        value_type : Union[pa.DataType, pa.Field, Column]
-            The type of the values in the list.
-
-        list_size : int
-            The size of the list. If -1, then the list is variable-length.
+        if isinstance(value_type, Column):
+            value_type = value_type.dtype
+        super().__init__(pa.list_(value_type, -1), nullable=nullable, metadata=metadata, validator=validator)
 
-        nullable : bool
-            Whether the list can contain null values.
+    @overload
+    def __get__(self, obj: None, objtype: type) -> Self:
+        ...
 
-        metadata : Optional[MetadataDict]
-            A dictionary of metadata to attach to the column.
+    @overload
+    def __get__(self, obj: tables.Table, objtype: type) -> pa.ListArray:
+        ...
 
-        validator: Optional[validators.Validator]
-            A validator to run against the column's values.
-        """
+    def __get__(self, obj: Optional[tables.Table], objtype: type) -> Union[Self, pa.ListArray]:
+        if obj is None:
+            return self
+        return obj.table[self.name].combine_chunks()
+
+
+class FixedSizeListColumn(Column):
+    """A column for storing lists of values of a fixed size.
+
+    The values in the list can be of any type.
+
+    Note that all quivr Tables are storing lists of values, so this
+    column type is only useful for storing lists of lists.
+
+    :param value_type: The type of the values in the list.
+    :param list_size: The size of the list. Must be greater than 0.
+    :param nullable: Whether the list can contain null values.
+    :param metadata: A dictionary of metadata to attach to the column.
+    :param validator: A validator to run against the column's values.
+    """
+
+    def __init__(
+        self,
+        value_type: Union[pa.DataType, pa.Field, Column],
+        list_size: int,
+        nullable: bool = True,
+        metadata: Optional[MetadataDict] = None,
+        validator: Optional[validators.Validator] = None,
+    ):
+        if list_size <= 0:
+            raise ValueError("list_size must be greater than 0")
         if isinstance(value_type, Column):
             value_type = value_type.dtype
         super().__init__(
             pa.list_(value_type, list_size), nullable=nullable, metadata=metadata, validator=validator
         )
 
     @overload
     def __get__(self, obj: None, objtype: type) -> Self:
         ...
 
     @overload
-    def __get__(self, obj: "Table", objtype: type) -> pa.ListArray:
+    def __get__(self, obj: tables.Table, objtype: type) -> pa.FixedSizeListArray:
         ...
 
-    def __get__(self, obj: Optional["Table"], objtype: type) -> Union[Self, pa.ListArray]:
+    def __get__(self, obj: Optional[tables.Table], objtype: type) -> Union[Self, pa.FixedSizeListArray]:
         if obj is None:
             return self
         return obj.table[self.name].combine_chunks()
 
 
 class LargeListColumn(Column):
-    """A column for storing large lists of values.
+    r"""A column for storing large lists of values (over 2\ :sup:`31` objects).
 
     Unless you need to represent data with more than 2**31 elements,
     prefer ListColumn.
 
     The values in the list can be of any type.
 
     Note that all quivr Tables are storing lists of values, so this
     column type is only useful for storing lists of lists.
+
+    :param value_type: The type of the values in the list.
+    :param nullable: Whether the list can contain null values.
+    :param metadata: A dictionary of metadata to attach to the column.
+    :param validator: A validator to run against the column's values.
     """
 
     def __init__(
         self,
         value_type: Union[pa.DataType, pa.Field, Column],
         nullable: bool = True,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
     ):
-        """
-        Parameters
-        ----------
-        value_type : Union[pa.DataType, pa.Field, Column]
-            The type of the values in the list.
-
-        nullable : bool
-            Whether the list can contain null values.
-
-        metadata : Optional[MetadataDict]
-            A dictionary of metadata to attach to the column.
-
-        validator: Optional[validators.Validator]
-            A validator to run against the column's values.
-        """
         if isinstance(value_type, Column):
             value_type = value_type.dtype
         super().__init__(pa.large_list(value_type), nullable=nullable, metadata=metadata, validator=validator)
 
     @overload
     def __get__(self, obj: None, objtype: type) -> Self:
         ...
 
     @overload
-    def __get__(self, obj: "Table", objtype: type) -> pa.LargeListArray:
+    def __get__(self, obj: tables.Table, objtype: type) -> pa.LargeListArray:
         ...
 
-    def __get__(self, obj: Optional["Table"], objtype: type) -> Union[Self, pa.LargeListArray]:
+    def __get__(self, obj: Optional[tables.Table], objtype: type) -> Union[Self, pa.LargeListArray]:
         if obj is None:
             return self
         return obj.table[self.name].combine_chunks()
 
 
 class MapColumn(Column):
     """A column for storing maps of key-value pairs.
 
     The keys and values can be of any type, as long as the keys are
     hashable and unique.
+
+    :param key_type: The type of the keys in the map.
+    :param item_type: The type of the values in the map.
+    :param nullable: Whether the map can contain null key-value pairs.
+    :param metadata: A dictionary of metadata to attach to the column.
+    :param validator: A validator to run against the column's values.
     """
 
     def __init__(
         self,
         key_type: Union[pa.DataType, pa.Field, Column],
         item_type: Union[pa.DataType, pa.Field, Column],
         nullable: bool = True,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
     ):
-        """
-        Parameters
-        ----------
-        key_type : Union[pa.DataType, pa.Field, Column]
-            The type of the keys in the map.
-
-        item_type : Union[pa.DataType, pa.Field, Column]
-            The type of the values in the map.
-
-        nullable : bool
-            Whether the map can contain null values.
-
-        metadata : Optional[MetadataDict]
-            A dictionary of metadata to attach to the column.
-
-        validator: Optional[validators.Validator]
-            A validator to run against the column's values.
-        """
         if isinstance(key_type, Column):
             key_type = key_type.dtype
         if isinstance(item_type, Column):
             item_type = item_type.dtype
         super().__init__(
             pa.map_(key_type, item_type), nullable=nullable, metadata=metadata, validator=validator
         )
 
     @overload
     def __get__(self, obj: None, objtype: type) -> Self:
         ...
 
     @overload
-    def __get__(self, obj: "Table", objtype: type) -> pa.MapArray:
+    def __get__(self, obj: tables.Table, objtype: type) -> pa.MapArray:
         ...
 
-    def __get__(self, obj: Optional["Table"], objtype: type) -> Union[Self, pa.MapArray]:
+    def __get__(self, obj: Optional[tables.Table], objtype: type) -> Union[Self, pa.MapArray]:
         if obj is None:
             return self
         return obj.table[self.name].combine_chunks()
 
 
 class DictionaryColumn(Column):
     """A column for storing dictionary-encoded values.
 
     This is intended for use with categorical data. See MapColumn for a
     more general mapping type.
+
+    :param index_type: The type of the dictionary indices. Must be an integer type.
+    :param value_type: The type of the values in the dictionary.
+    :param ordered: Whether the dictionary is ordered.
+    :param nullable: Whether the dictionary can contain null values.
+    :param metadata: A dictionary of metadata to attach to the column.
+    :param validator: A validator to run against the column's values.
     """
 
     def __init__(
         self,
         index_type: pa.DataType,
         value_type: Union[pa.DataType, pa.Field, Column],
         ordered: bool = False,
         nullable: bool = True,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
     ):
-        """
-        Parameters
-        ----------
-        index_type : IntegerDataType
-            The type of the dictionary indices. Must be an integer type.
-
-        value_type : Union[pa.DataType, pa.Field, Column]
-            The type of the values in the dictionary.
-
-        ordered : bool
-            Whether the dictionary is ordered.
-
-        nullable : bool
-            Whether the dictionary can contain null values.
-
-        metadata : Optional[MetadataDict]
-            A dictionary of metadata to attach to the column.
-
-        validator: Optional[validators.Validator]
-            A validator to run against the column's values.
-        """
         if isinstance(index_type, Column):
             index_type = index_type.dtype
         if isinstance(value_type, Column):
             value_type = value_type.dtype
         super().__init__(
             pa.dictionary(index_type, value_type, ordered=ordered),
             nullable=nullable,
@@ -1056,53 +1180,43 @@
         )
 
     @overload
     def __get__(self, obj: None, objtype: type) -> Self:
         ...
 
     @overload
-    def __get__(self, obj: "Table", objtype: type) -> pa.DictionaryArray:
+    def __get__(self, obj: tables.Table, objtype: type) -> pa.DictionaryArray:
         ...
 
-    def __get__(self, obj: Optional["Table"], objtype: type) -> Union[Self, pa.DictionaryArray]:
+    def __get__(self, obj: Optional[tables.Table], objtype: type) -> Union[Self, pa.DictionaryArray]:
         if obj is None:
             return self
         return obj.table[self.name].combine_chunks()
 
 
 class StructColumn(Column):
     """A column for storing structured data.
 
     In general, prefer to define Tables and use their as_column method
     instead of using StructColumn.
 
+    :param fields: The fields in the struct.
+    :param nullable: Whether the struct can contain null values.
+    :param metadata: A dictionary of metadata to attach to the column.
+    :param validator: A validator to run against the column's values.
+
     """
 
     def __init__(
         self,
         fields: list[pa.Field],
         nullable: bool = True,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
     ):
-        """
-        Parameters
-        ----------
-        fields : List[pa.Field]
-            The fields in the struct.
-
-        nullable : bool
-            Whether the struct can contain null values.
-
-        metadata : Optional[MetadataDict]
-            A dictionary of metadata to attach to the column.
-
-        validator: Optional[validators.Validator]
-            A validator to run against the column's values.
-        """
         super().__init__(pa.struct(fields), nullable=nullable, metadata=metadata, validator=validator)
 
 
 class RunEndEncodedColumn(Column):
     """A column for storing run-end encoded data.
 
     This is a special column type that is used to efficiently store
@@ -1113,41 +1227,29 @@
       reduced to a single element
     - An array of run lengths, with the length of each run
 
     This is more compact than storing the redundant values and also
     allow for very efficient computations like aggregations upon the
     data.
 
+
+    :param run_end_type: The type of the run-end encoded values. Must be a 16-, 32-, or 64-bit integer type.
+    :param value_type: The type of the values in the run-end encoded data.
+    :param nullable: Whether the data can contain null values.
+    :param metadata: A dictionary of metadata to attach to the column.
+    :param validator: A validator to run against the column's values.
     """
 
     def __init__(
         self,
         run_end_type: pa.DataType,
         value_type: pa.DataType,
         nullable: bool = True,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
     ):
-        """
-        Parameters
-        ----------
-        run_end_type : pa.DataType
-            The type of the run-end encoded values. Must be a 16-, 32-, or 64-bit integer type.
-
-        value_type : pa.DataType
-            The type of the values in the run-end encoded data.
-
-        nullable : bool
-            Whether the data can contain null values.
-
-        metadata : Optional[MetadataDict]
-            A dictionary of metadata to attach to the column.
-
-        validator: Optional[validators.Validator]
-            A validator to run against the column's values.
-        """
         super().__init__(
             pa.run_end_encoded(run_end_type, value_type),
             nullable=nullable,
             metadata=metadata,
             validator=validator,
         )
```

### Comparing `quivr-0.4.3/quivr/concat.py` & `quivr-0.5.0/quivr/concat.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,35 +1,38 @@
-from typing import Iterator, TypeVar
+from typing import Iterator
 
 import pyarrow as pa
 
+from . import tables
 from .defragment import defragment
-from .tables import Table
 
-T = TypeVar("T", bound=Table)
 
-
-def concatenate(values: Iterator[T], defrag: bool = True) -> T:
+def concatenate(values: Iterator[tables.AnyTable], defrag: bool = True) -> tables.AnyTable:
     """Concatenate a collection of Tables into a single Table.
 
     All input Tables must have the same schema (typically, this will
     be from being the same class).
 
     By default, results are compacted to be contiguous in memory,
     which involves a copy. In a tight loop, this can be very
     inefficient, so you can set the 'defrag' parameter to False to
-    skip this compaction step, and instead call quiver.defragment on
+    skip this compaction step, and instead call :func:`defragment` on
     the result after the loop is complete.
 
+    :param values: An iterator of :class:`Table` instances to concatenate.
+    :param defrag: Whether to compact the result to be contiguous in
+        memory. Defaults to True.
     """
     batches = []
     first = True
     for v in values:
         batches += v.table.to_batches()
         if first:
             cls = v.__class__
             first = False
+    if len(batches) == 0:
+        raise ValueError("No values to concatenate")
     table = pa.Table.from_batches(batches)
     result = cls(table=table)
     if defrag:
         result = defragment(result)
     return result
```

### Comparing `quivr-0.4.3/quivr/indexing.py` & `quivr-0.5.0/quivr/indexing.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,22 +10,14 @@
 
 
 class StringIndex(Generic[T]):
     """StringIndex is a simple index that maps a string column to a
     list of row indices. It can be used for fast lookups of sub-slices
     of a Table based on string values.
 
-    Example usage:
-
-    >>> from indexing import StringIndex
-    >>> from examples.coordinates import create_example_orbits
-    >>> orbits = create_example_orbits(1000)
-    >>> index = StringIndex(orbits, 'object_id')
-    >>> index.lookup('id990')
-    Orbit(size=1)
 
     This is equivalent to calling table.select("object_id", "id990"),
     but it is about 5x faster. The tradeoff is that building the
     StringIndex takes about 450 microseconds for this example.
 
     """
```

### Comparing `quivr-0.4.3/quivr/matrix.py` & `quivr-0.5.0/quivr/matrix.py`

 * *Files identical despite different names*

### Comparing `quivr-0.4.3/quivr/schemagraph.py` & `quivr-0.5.0/quivr/schemagraph.py`

 * *Files identical despite different names*

### Comparing `quivr-0.4.3/quivr/tables.py` & `quivr-0.5.0/quivr/tables.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,56 +1,82 @@
+from __future__ import annotations
+
 import os
 import sys
 from io import IOBase
 
 if sys.version_info < (3, 11):
     from typing_extensions import Self
 else:
     from typing import Self
 
-from typing import Any, ClassVar, Iterator, Optional, Type, TypeAlias, Union
+from typing import Any, ClassVar, Iterator, Optional, Type, TypeAlias, TypeVar, Union
 
 import numpy as np
 import numpy.typing as npt
 import pandas as pd
 import pyarrow as pa
 import pyarrow.compute as pc
 import pyarrow.csv
 import pyarrow.feather
 import pyarrow.parquet
 
+from . import columns
 from .attributes import Attribute
-from .columns import Column, MetadataDict, SubTableColumn
 from .errors import TableFragmentedError, ValidationError
 from .schemagraph import _walk_schema
 from .validators import Validator
 
 AttributeValueType: TypeAlias = Union[int, float, str]
 DataSourceType: TypeAlias = Union[pa.Array, list[Any], "Table", pd.Series, npt.NDArray[Any]]
+AnyTable = TypeVar("AnyTable", bound="Table")
 
 
 class Table:
+    """Table is the primary data structure in quivr.
+
+    Tables are used to represent tabular data with a fixed schema. The
+    schema is defined by subclassing Table, providing Column objects
+    as class attributes. The Table class will then generate a pyarrow
+    schema from those columns.
+
+    Table instances can then be created from data, either by passing
+    in a pyarrow Table, or by passing in data in a variety of other
+    formats. The data will be validated against the schema, and
+    converted to a pyarrow Table.
+
+    Table instances are immutable, but can be sliced, filtered,
+    sorted, or otherwise manipulated, resulting in new Table
+    instances.
+
+    :cvar schema: The pyarrow schema for this table.
+    :vartype schema: pyarrow.Schema
+
+    :ivar table: The underlying :class:`pyarrow.Table` for this Table instance.
+    :vartype table: pyarrow.Table
+    """
+
     schema: ClassVar[pa.Schema]
     table: pa.Table
 
-    _quivr_subtables: ClassVar[dict[str, SubTableColumn[Any]]]
+    _quivr_subtables: ClassVar[dict[str, columns.SubTableColumn[Any]]]
     _quivr_attributes: ClassVar[dict[str, Attribute[Any]]]
     _column_validators: ClassVar[dict[str, Validator]]
 
     def __init_subclass__(cls: Type["Table"], **kwargs: Any):
         fields = []
         column_validators = {}
         subtables = {}
         attributes = {}
         for name, obj in cls.__dict__.items():
-            if isinstance(obj, Column):
+            if isinstance(obj, columns.Column):
                 fields.append(obj.pyarrow_field())
                 if obj.validator is not None:
                     column_validators[name] = obj.validator
-                if isinstance(obj, SubTableColumn):
+                if isinstance(obj, columns.SubTableColumn):
                     subtables[name] = obj
             elif isinstance(obj, Attribute):
                 attributes[name] = obj
 
         # Generate a pyarrow schema
         schema = pa.schema(fields)
         cls.schema = schema
@@ -85,49 +111,51 @@
     @classmethod
     def from_data(
         cls,
         data: Union[pa.Table, dict[str, Any], list[Any], pd.DataFrame, None] = None,
         validate: bool = True,
         **kwargs: Union[AttributeValueType, DataSourceType],
     ) -> Self:
-        """
-        Create an instance of the Table and populate it with data.
+        """Create an instance of the Table and populate it with data.
 
         This is a convenience method which tries to infer the right
         underlying constructors to use based on the type of data. It
         can also accept keyword-style arguments to pass data in. If
         you know the data's structure well in advance, the more
         precise constructors (from_arrays, from_pylist, etc) should be
         preferred.
 
         If the validate argument is True, the data will be validated
         against the table's schema. If validation fails, a
-        ValidationError will be raised.
+        :class:`ValidationError` will be raised.
+
+        For example:
 
-        Examples:
             >>> import quivr
-            >>> class MyTable(quivr.TableBase):
-            ...     schema = pyarrow.schema([
-            ...         pyarrow.field("a", pyarrow.string()),
-            ...         pyarrow.field("b", pyarrow.int64()),
-            ...     ])
+            >>> class MyTable(quivr.Table):
+            ...     a = quivr.StringColumn()
+            ...     b = quivr.Int64Column()
             ...
             >>> # All of these are equivalent:
-            >>> MyTable.from_data([["a", 1], ["b", 2]])
-            MyTable(size=2)
             >>> MyTable.from_data({"a": ["a", "b"], "b": [1, 2]})
             MyTable(size=2)
             >>> MyTable.from_data([{"a": "a", "b": 1}, {"a": "b", "b": 2}])
             MyTable(size=2)
             >>> MyTable.from_data(a=["a", "b"], b=[1, 2])
             MyTable(size=2)
             >>> import numpy as np
             >>> MyTable.from_data(a=np.array(["a", "b"]), b=np.array([1, 2]))
             MyTable(size=2)
 
+        :param data: The data to populate the table with.
+        :param validate: Whether to validate the data against the table's schema.
+        :param \\**kwargs: More data in keyword argument form. The keys
+          can be column names or attribute names. The values should be
+          arrays, lists, or pyarrow Arrays.
+        :type \\**kwargs: Union[:obj:`AttributeValueType`, :obj:`DataSourceType`]
 
         """
         if data is None:
             instance = cls.from_kwargs(**kwargs)
         else:
             attrib_kwargs = cls._attribute_kwargs_from_kwargs(kwargs)
             if isinstance(data, pa.Table):
@@ -163,26 +191,46 @@
             if not isinstance(v, cls._quivr_attributes[k]._type):
                 raise TypeError(f"Expected {cls._quivr_attributes[k]._type}, got {type(v)} for {k}")
             attrib_kwargs[k] = v
         return attrib_kwargs
 
     @classmethod
     def as_column(
-        cls, nullable: bool = True, metadata: Optional[MetadataDict] = None
-    ) -> SubTableColumn[Self]:
-        return SubTableColumn(cls, nullable=nullable, metadata=metadata)
+        cls, nullable: bool = True, metadata: Optional[columns.MetadataDict] = None
+    ) -> columns.SubTableColumn[Self]:
+        """Embed the Table as a column in another Table.
+
+        This method is the primary way to achieve composition of Tables with quivr.
+
+        :param nullable: Whether the column can contain nulls. Note
+            that this refers to whether an entire row - all columns -
+            can be null, not whether a single value in one column of
+            this table can be null. That is controlled entirely by
+            this Table class's columns.
+
+        :param metadata: Metadata to attach to the column.
+
+        """
+        return columns.SubTableColumn(cls, nullable=nullable, metadata=metadata)
 
     @classmethod
     def from_kwargs(cls, **kwargs: Union[DataSourceType, AttributeValueType]) -> Self:
         """Create a Table instance from keyword arguments.
 
         Each keyword argument corresponds to a column in the Table.
 
-        The keys should correspond to the column names, and the values
-        can be a list, numpy array, pyarrow array, or Table instance.
+        The keys should correspond to column names or attribute names.
+
+        For columns, the values should be arrays, lists, or pyarrow Arrays.
+
+        For attributes, the values should be the appropriate type for that attribute.
+
+        :param \\**kwargs: The data to populate the table with.
+        :type \\**kwargs: Union[:obj:`AttributeValueType`, :obj:`DataSourceType`]
+
         """
         arrays: list[Union[None, pa.Array]] = []
         size = None
 
         # We don't know the size of the table until we've found a
         # field in the schema which corresponds to a kwarg with data.
         # Therefore, we need to keep track of which columns are empty
@@ -239,28 +287,26 @@
             arrays[idx] = pa.nulls(size, type=cls.schema[idx].type)
         attrib_kwargs = cls._attribute_kwargs_from_kwargs(kwargs)
         return cls.from_arrays(arrays, metadata=metadata, **attrib_kwargs)
 
     @classmethod
     def from_arrays(
         cls,
-        arrays: list[pa.array],
+        arrays: list[pa.Array],
         metadata: Optional[dict[bytes, bytes]] = None,
         **kwargs: AttributeValueType,
     ) -> Self:
-        """Create a Table object from a list of arrays.
-
-        Args:
-            arrays: A list of pyarrow.Array objects.
-            metadata: An optional dictionary of metadata to attach to the Table.
-            **kwargs: Additional keyword arguments to pass to the Table's __init__ method.
-
-        Returns:
-            A Table object.
+        """
+        Create a Table object from a list of arrays.
 
+        :param arrays: A list of pyarrow.Array objects.
+        :param metadata: An optional dictionary of metadata to attach to the Table.
+        :param \\**kwargs: Additional keyword arguments for any Table attributes.
+        :type \\**kwargs: :obj:`AttributeValueType`
+        :return: A Table object.
         """
         if metadata is None:
             metadata = {}
         schema = cls.schema.with_metadata(metadata)
         table = pa.Table.from_arrays(arrays, schema=schema)
         return cls(table=table, **kwargs)
 
@@ -272,52 +318,47 @@
         return cls(table=table, **kwargs)
 
     @classmethod
     def from_rows(cls, rows: list[dict[str, Any]], **kwargs: AttributeValueType) -> Self:
         """
         Create a Table object from a list of dictionaries.
 
-        Args:
-            rows: A list of values. Each value corresponds to a row in the table.
-            **kwargs: Additional keyword arguments to pass to the Table's __init__ method.
-
-        Returns:
-            A Table object.
+        :param rows: A list of values. Each value corresponds to a row in the table.
+        :param \\**kwargs: Additional keyword arguments for any Table attributes.
+        :type \\**kwargs: :obj:`AttributeValueType`
+        :returns: A Table object.
 
         Examples:
             >>> import quivr
             >>> class Inner(quivr.Table):
             ...     a = quivr.StringColumn()
             ...
-            >>> class Outer(quivr.TableBase):
+            >>> class Outer(quivr.Table):
             ...     z = quivr.StringColumn()
             ...     i = Inner.as_column()
             ...
             >>> data = [{"z": "v1", "i": {"a": "v1_in"}}, {"z": "v2", "i": {"a": "v2_in"}}]
-            >>> Outer.from_pylist(data)
+            >>> Outer.from_rows(data)
             Outer(size=2)
         """
         table = pa.Table.from_pylist(rows, schema=cls.schema)
         return cls(table=table, **kwargs)
 
     @classmethod
     def from_lists(cls, lists: list[list[Any]], **kwargs: AttributeValueType) -> Self:
         """Create a Table object from a list of lists.
 
         Each inner list corresponds to a column in the Table. They
         should be specified in the same order as the columns in the
         class.
 
-        Args:
-            lists: A list of lists. Each inner list corresponds to a column in the table.
-            **kwargs: Additional keyword arguments to pass to the Table's __init__ method.
-
-
-        Returns:
-            A TableBase object.
+        :param lists: A list of lists. Each inner list corresponds to a column in the table.
+        :param \\**kwargs: Additional keyword arguments for any Table attributes.
+        :type \\**kwargs: :obj:`AttributeValueType`
+        :returns: A Table object.
 
         """
         table = pa.Table.from_arrays(list(map(pa.array, lists)), schema=cls.schema)
         return cls(table=table, **kwargs)
 
     @classmethod
     def from_dataframe(cls, df: pd.DataFrame, **kwargs: AttributeValueType) -> Self:
@@ -327,27 +368,30 @@
         error is raised. If the DataFrame has extra columns, they are
         ignored.
 
         This function cannot load "flattened" dataframes. This only
         matters for nested Tables which contain other Table
         definitions as columns. For that use case, either load an
         unflattened DataFrame, or use from_flat_dataframe.
+
+        :param df: A pandas DataFrame containing the data to load.
+        :param \\**kwargs: Additional keyword arguments for any Table attributes.
+        :type \\**kwargs: :obj:`AttributeValueType`
         """
 
         table = pa.Table.from_pandas(df, schema=cls.schema)
         return cls(table=table, **kwargs)
 
     @classmethod
     def _unflatten_table(cls, table: pa.Table) -> pa.Table:
         """Unflatten a Table.
 
         This is used when loading a flattened CSV into a nested
         Table. It takes a Table with a flat schema, and returns a
         Table with a nested schema.
-
         """
         struct_fields = []
 
         for field in cls.schema:
             if pa.types.is_struct(field.type):
                 struct_fields.append(field)
 
@@ -375,15 +419,21 @@
 
         return pa.Table.from_arrays(child_arrays, schema=cls.schema)
 
     @classmethod
     def from_flat_dataframe(cls, df: pd.DataFrame, **kwargs: AttributeValueType) -> Self:
         """Load a flattened DataFrame into the Table.
 
-        known bug: Doesn't correctly interpret fixed-length lists.
+        .. caution::
+          Known bug: Doesn't correctly interpret fixed-length lists.
+
+        :param df: A pandas DataFrame containing the data to load.
+        :param \\**kwargs: Additional keyword arguments for any Table attributes.
+        :type \\**kwargs: :obj:`AttributeValueType`
+
         """
         struct_fields = []
         for field in cls.schema:
             if pa.types.is_struct(field.type):
                 struct_fields.append(field)
 
         if len(struct_fields) == 0:
@@ -469,36 +519,38 @@
         return table
 
     def select(self, column_name: str, value: Any) -> Self:
         """Select from the table by exact match, returning a new
         Table which only contains rows for which the value in
         column_name equals value.
 
+        :param column_name: The name of the column to select on.
+        :param value: The value to match.
         """
         table = self.table.filter(pc.field(column_name) == value)
         return self.__class__(table)
 
     def sort_by(self, by: Union[str, list[tuple[str, str]]]) -> Self:
         """Sorts the Table by the given column name (or multiple
         columns). This operation requires a copy, and returns a new
         Table using the copied data.
 
         by should be a column name to sort by, or a list of (column,
         order) tuples, where order can be "ascending" or "descending".
 
+        :param by: The column name or list of (column, order) tuples to sort by.
         """
         table = self.table.sort_by(by)
         return self.__class__(table)
 
     def chunk_counts(self) -> dict[str, int]:
         """Returns the number of discrete memory chunks that make up
         each of the Table's underlying arrays. The keys of the
         resulting dictionary are the column names, and the values are
         the number of chunks for that column's data.
-
         """
         result = {}
         for i, field in enumerate(self.schema):
             result[field.name] = self.table.column(i).num_chunks
         return result
 
     def fragmented(self) -> bool:
@@ -510,14 +562,16 @@
         return any(v > 1 for v in self.chunk_counts().values())
 
     def to_structarray(self) -> pa.StructArray:
         """Returns self as a StructArray.
 
         This only works if self is not fragmented. Call table =
         defragment(table) if table.fragmented() is True.
+
+        :raises TableFragmentedError: if the table is fragmented.
         """
         if self.fragmented():
             raise TableFragmentedError(
                 "Tables cannot be converted to StructArrays while fragmented; call defragment(table) first."
             )
         arrays = [chunked_array.chunks[0] for chunked_array in self.table.columns]
         return pa.StructArray.from_arrays(arrays, fields=list(self.schema))
@@ -531,126 +585,236 @@
         columns "foo.a", "foo.b", "foo.c". This is done fully for any
         deeply nested structure, for example "foo.bar.baz.c".
 
         If flatten is false, then that struct will be in a single
         "foo" column, and the values will of the column will be
         dictionaries representing the struct values.
 
+        :param flatten: Whether to flatten the table's structure.
         """
         table = self.table
         if flatten:
             table = self.flattened_table()
         df: pd.DataFrame = table.to_pandas()
         return df
 
     def column(self, column_name: str) -> pa.ChunkedArray:
-        """Returns the column with the given name as a raw pyarrow ChunkedArray."""
+        """
+        Returns the column with the given name as a raw pyarrow ChunkedArray.
+
+        :param column_name: The name of the column to return.
+        """
         return self.table.column(column_name)
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}(size={len(self.table)})"
 
     def __len__(self) -> int:
+        """
+        Returns the number of rows in the Table.
+        """
         return len(self.table)
 
     def with_table(self, table: pa.Table) -> Self:
         return self.__class__(table)
 
     def __getitem__(self, idx: Union[int, slice]) -> Self:
+        """
+        Returns a new Table containing the given row or rows.
+
+        :param idx: The row index or slice to return.
+        """
         if isinstance(idx, int):
             table = self.table[idx : idx + 1]
         else:
             table = self.table[idx]
         return self.with_table(table)
 
     def __iter__(self) -> Iterator[Self]:
+        """
+        Iterates over the rows of the Table, returning a new Table
+        containing each row.
+        """
         for i in range(len(self)):
             yield self[i : i + 1]
 
     def __eq__(self, other: Any) -> bool:
+        """Returns true if the two Tables are equal. They are
+        considered equal if they have the same data in their tables,
+        and identical attributes and attribute values.
+
+        :param other: The other Table to compare to.
+
+        """
         if isinstance(other, Table):
-            return bool(self.table.equals(other.table, check_metadata=True))
+            if not bool(self.table.equals(other.table, check_metadata=False)):
+                return False
+            if not self._attr_equal(other):
+                return False
+            return True
         if isinstance(other, pa.Table):
             return bool(self.table.equals(other, check_metadata=True))
+
         return False
 
+    def _attr_equal(self, other: Self) -> bool:
+        """
+        Check if the attributes of two tables are equal. Recurs into subtables.
+        """
+        if not isinstance(other, self.__class__):
+            return False
+
+        if self.attributes() != other.attributes():
+            return False
+
+        for subtable_name in self._quivr_subtables.keys():
+            self_subtable = getattr(self, subtable_name)
+            other_subtable = getattr(other, subtable_name)
+            if other_subtable is None:
+                return False
+            if not self_subtable._attr_equal(other_subtable):
+                return False
+        return True
+
     def take(self, row_indices: Union[list[int], pa.IntegerArray]) -> Self:
-        """Return a new Table with only the rows at the given indices."""
+        """
+        Return a new Table with only the rows at the given indices.
+
+        :param row_indices: The indices of the rows to return.
+        """
         return self.__class__(self.table.take(row_indices))
 
     def to_parquet(self, path: str, **kwargs: Any) -> None:
-        """Write the table to a Parquet file."""
+        """
+        Write the table to a Parquet file.
+
+        :param path: The path to write the Parquet file to.
+        :param kwargs: Additional arguments to pass to pyarrow.parquet.write_table.
+        """
         pyarrow.parquet.write_table(self.table, path, **kwargs)
 
     @classmethod
     def from_parquet(
         cls,
         path: str,
         memory_map: bool = False,
         pq_buffer_size: int = 0,
         filters: Optional[pc.Expression] = None,
+        column_name_map: Optional[dict[str, str]] = None,
         **kwargs: AttributeValueType,
     ) -> Self:
         """Read a table from a Parquet file.
 
-        Arguments:
-            path: The path to the Parquet file.
-            memory_map: If True, memory-map the file, otherwise read it into memory.
-            pq_buffer_size: If positive, perform read buffering when
-                deserializing individual column chunks. Otherwise, IO
-                calls are unbuffered.
-            filters: An optional filter predicate to apply to the
+        :param path: The path to the Parquet file.
+        :param memory_map: If True, memory-map the file, otherwise read it into memory.
+
+        :param pq_buffer_size: If positive, perform read buffering
+                when deserializing individual column
+                chunks. Otherwise, IO calls are unbuffered.
+        :param filters: An optional filter predicate to apply to the
                 data. Rows which do not match the predicate will be
                 removed from scanned data. For more information, see
                 the PyArrow documentation on
                 pyarrow.parquet.read_table and its filter parameter.
-            **kwargs: Additional keyword arguments to pass to the __init__ method.
-
+        :param column_name_map: An optional dictionary mapping column names in the Parquet file to
+                column names in the resulting Table. This is useful if the Parquet file contains
+                column names that are not valid Python identifiers, or if you want to rename
+                columns for any other reason.
+        :param \\**kwargs: Additional keyword arguments to pass to Self's __init__ method.
 
         """
+        table = cls._load_parquet_table(
+            path=path,
+            memory_map=memory_map,
+            pq_buffer_size=pq_buffer_size,
+            filters=filters,
+            column_name_map=column_name_map,
+        )
+        return cls(table=table, **kwargs)
+
+    @classmethod
+    def _load_parquet_table(
+        cls,
+        path: str,
+        memory_map: bool,
+        pq_buffer_size: int,
+        filters: Optional[pc.Expression],
+        column_name_map: Optional[dict[str, str]],
+    ) -> pa.Table:
+        if column_name_map is not None:
+            inverted_map = {v: k for k, v in column_name_map.items()} if column_name_map else {}
+            column_names = [inverted_map.get(field.name, field.name) for field in cls.schema]
+            schema = pa.schema(
+                [pa.field(inverted_map.get(field.name, field.name), field.type) for field in cls.schema]
+            )
+        else:
+            column_names = [field.name for field in cls.schema]
+            schema = cls.schema
+
         table = pyarrow.parquet.read_table(
             source=path,
-            columns=[field.name for field in cls.schema],
+            columns=column_names,
             memory_map=memory_map,
             buffer_size=pq_buffer_size,
             filters=filters,
+            schema=schema,
         )
-        return cls(table=table, **kwargs)
+        md = pyarrow.parquet.read_metadata(path, memory_map=memory_map)
+        table = table.replace_schema_metadata(md.metadata)
+
+        if column_name_map is not None:
+            table = table.rename_columns([field.name for field in cls.schema])
+
+        return table
 
     def to_feather(self, path: str, **kwargs: Any) -> None:
-        """Write the table to a Feather file."""
+        """
+        Write the table to a Feather file.
+
+        :param path: The path to write the Feather file to.
+        :param kwargs: Additional arguments to pass to pyarrow.feather.write_feather.
+        """
         pyarrow.feather.write_feather(self.table, path, **kwargs)
 
     @classmethod
     def from_feather(cls, path: str, **kwargs: AttributeValueType) -> Self:
-        """Read a table from a Feather file."""
+        """Read a table from a Feather file.
+
+        :param path: The path to the Feather file.
+        :param \\**kwargs: Additional keyword arguments to pass to Self's __init__ method.
+        """
         return cls(table=pyarrow.feather.read_table(path), **kwargs)
 
     def to_csv(self, path: str, attribute_columns: bool = True) -> None:
         """Write the table to a CSV file. Any nested structure is flattened.
 
-        if attribute_columns is True (the default), then any Attributes defined
-        for the table (or its subtable columns) are stored in the CSV as columns;
-        they will have the same value repeated for every row. If it is False,
-        then Attribute data will  not be stored in the CSV, so it cannot be read back out.
+        :param path: The path to write the CSV file to.
+        :param attribute_columns: If True, store any Attributes defined for the table
+            (or its subtable columns) as columns in the CSV file. If False, do not store
+            any Attribute data in the CSV file.
         """
         table = self.flattened_table()
         if attribute_columns:
             for name, val in self._string_attributes().items():
                 table = table.append_column(
                     name,
                     pa.repeat(val, len(table)),
                 )
         pyarrow.csv.write_csv(table, path)
 
     @classmethod
     def from_csv(
         cls, input_file: Union[str, os.PathLike, IOBase], **kwargs: AttributeValueType  # type: ignore
     ) -> Self:
-        """Read a table from a CSV file."""
+        """
+        Read a table from a CSV file.
+
+        :param input_file: The path to the CSV file, or a file-like object.
+        :param \\**kwargs: Additional keyword arguments to set the Table's attributes.
+        """
         flat_table = pyarrow.csv.read_csv(input_file)
 
         # Gather any attributes from the CSV. We do this by looking for specially named
         # columns, and grabbing the value from their first row.
         attributes = {}
         attr_names = cls._attribute_metadata_keys()
         if len(flat_table) > 0:
@@ -684,15 +848,18 @@
             try:
                 validator.validate(self.table.column(name))
             except ValidationError as e:
                 raise ValidationError(f"Column {name} failed validation: {str(e)}", e.failures) from e
 
     @classmethod
     def empty(cls, **kwargs: AttributeValueType) -> Self:
-        """Create an empty instance of the table."""
+        """Create an empty instance of the table.
+
+        :param \\**kwargs: Additional keyword arguments to set the Table's attributes.
+        """
         data = [[] for _ in range(len(cls.schema))]  # type: ignore
         empty_table = pa.table(data, schema=cls.schema)
         return cls(table=empty_table, **kwargs)
 
     def attributes(self) -> dict[str, Any]:
         """Return a dictionary of the table's attributes."""
         return {name: getattr(self, name) for name in self._quivr_attributes}
@@ -753,45 +920,48 @@
                 result.add(f"{column.name}.{attr.name}")
 
             children = column.table_type._attribute_metadata_keys()
             for key in children:
                 result.add(f"{column.name}.{key}")
         return result
 
-    def apply_mask(self, mask: pa.BooleanArray | np.ndarray | list[bool]) -> Self:
-        """Return a new table with rows filtered to match a boolean mask.
+    def apply_mask(self, mask: pa.BooleanArray | np.ndarray[bool, Any] | list[bool]) -> Self:
+        """
+        Return a new table with rows filtered to match a boolean mask.
 
         The mask must have the same length as the table. At each index, if the mask's
         value is True, the row will be included in the new table; if False, it will be
         excluded.
 
         If the mask is a pyarrow BooleanArray, it must not have any null values.
+
+        :param mask: A boolean mask to apply to the table.
         """
         if len(mask) != len(self):
             raise ValueError("mask must be the same length as the table")
         if isinstance(mask, pa.BooleanArray):
             if mask.null_count > 0:
                 raise ValueError("mask must not contain null values")
         return self.__class__(self.table.filter(mask))
 
     def where(self, expr: pc.Expression) -> Self:
-        """Return a new table with rows filtered to match an expression.
+        """
+        Return a new table with rows filtered to match an expression.
 
         The expression must be a pyarrow Expression that evaluates to a boolean array.
 
-        Examples
-        --------
-        >>> from quivr import Table, Int64Column
-        >>> import pyarrow.compute as pc
-        >>> class MyTable(Table):
-        ...     x = Int64Column()
-        ...     y = Int64Column()
-        ...
-        >>> t = MyTable.from_data(x=[1, 2, 3], y=[4, 5, 6])
-        >>> filtered = t.where(pc.field("x") > 1)
-        >>> print(filtered.x.to_pylist())
-        [2, 3]
-        >>> print(filtered.y.to_pylist())
-        [5, 6]
+        :param expr: A pyarrow Expression to apply to the table.
 
+        Examples:
+            >>> from quivr import Table, Int64Column
+            >>> import pyarrow.compute as pc
+            >>> class MyTable(Table):
+            ...     x = Int64Column()
+            ...     y = Int64Column()
+            >>> t = MyTable.from_data(x=[1, 2, 3], y=[4, 5, 6])
+            >>> filtered = t.where(pc.field("x") > 1)
+            >>> print(filtered.x.to_pylist())
+            [2, 3]
+            >>> print(filtered.y.to_pylist())
+            [5, 6]
         """
         return self.__class__(self.table.filter(expr))
```

### Comparing `quivr-0.4.3/quivr/validators.py` & `quivr-0.5.0/quivr/validators.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,39 +3,69 @@
 import pyarrow
 import pyarrow.compute as pc
 
 from .errors import ValidationError
 
 
 class Validator:
+    """A Validator is a tool to validate that data in a
+    :class:`pyarrow.Array` matches a predicate expression.
+
+    :ivar func: The predicate function to use for validation. This
+        must be a scalar or scalar aggregate function.
+    :ivar args: The arguments to pass to the predicate function.
+    :ivar label: A label to use when reporting validation errors.
+    """
+
     def __init__(self, func: pc.Function, args: list[Any], label: str):
+        """
+        :param func: The predicate function to use for validation. This
+            must be a scalar or scalar aggregate function.
+        :param args: The arguments to pass to the predicate function.
+        :param label: A label to use when reporting validation errors.
+        """
         self._check_arity(func, args)
         if func.kind not in {"scalar_aggregate", "scalar"}:
             raise ValueError(f"Invalid function type {func.kind}, must be scalar or scalar_aggregate")
         self.func = func
         self.args = args
         self.label = label
 
     def _check_arity(self, func: pc.Function, args: list[Any]) -> None:
         if not func.arity == (len(args) + 1):
             raise ValueError("Invalid number of arguments")
 
     def evaluate(self, array: pyarrow.Array) -> pyarrow.Array:
+        """
+        Evaluates the predicate function on the given array.
+
+        :param array: The array to evaluate.
+        """
         return self.func.call([array, *self.args])
 
     def valid(self, array: pyarrow.Array) -> bool:
+        """
+        Returns True if the given array is valid, False otherwise.
+
+        :param array: The array to validate.
+        """
         if self.func.kind == "scalar_aggregate":
             return self.evaluate(array).as_py()  # type: ignore
         else:
             results = self.evaluate(array)
             if results.null_count == len(results):
                 return True
             return pc.all(self.evaluate(array)).as_py()  # type: ignore
 
     def validate(self, array: pyarrow.Array) -> None:
+        """
+        Raises a :class:`ValidationError` if the given array is not valid.
+
+        :param array: The array to validate.
+        """
         if not self.valid(array):
             if self.func.kind == "scalar_aggregate":
                 raise ValidationError(f"array did not pass validator '{self.label}'")
             indices, failures = self.failures(array)
             if len(failures) == 1:
                 index = indices[0].as_py()
                 value = failures[0].as_py()
@@ -140,21 +170,24 @@
     Validator that all data in a column is greater than or equal to a given value.
     """
     func = pc.get_function("greater_equal")
     label = f"ge({val})"
     return Validator(func, [val], label)
 
 
-def is_in(val: Any, fail_on_null: bool = False) -> IsInValidator:
+def is_in(val: Any, fail_on_null: bool = False) -> Validator:
     """Validator that all data in a column is in a given set.
 
-    If fail_on_null is true, then nulls always trigger an
-    error. Otherwise, they are matched to the value set, just like
-    regular values.
-
+    :param val: The set of values to check against. This can be a
+        list, tuple, or pyarrow.Array. If it is a list or tuple, it
+        will be converted to a pyarrow.Array.
+
+    :param fail_on_null: If True, then nulls always trigger an
+      error. Otherwise, they are matched to the value set, just like
+      regular values.
     """
     label = f"is_in({val})"
     if not isinstance(val, pyarrow.Array):
         val = pyarrow.array(val)
     val = pc.SetLookupOptions(value_set=val, skip_nulls=fail_on_null)
     return IsInValidator([val], label)
```

### Comparing `quivr-0.4.3/LICENSE` & `quivr-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `quivr-0.4.3/README.md` & `quivr-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `quivr-0.4.3/pyproject.toml` & `quivr-0.5.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -15,14 +15,23 @@
   "pyarrow",
   "numpy",
   "mmh3",
   "typing_extensions>=4.0.0"
 ]
 dynamic = [ "version" ]
 
+[project.optional-dependencies]
+docs = [
+  "sphinx==7.0.1",
+  "sphinx-autodoc-typehints",
+  "sphinx-copybutton",
+  "sphinx-toolbox",
+  "furo",
+]
+
 [project.urls]
 Source = "https://github.com/spenczar/quivr"
 
 [tool.hatch.build.targets.sdist]
 include = [
   "/quivr",
 ]
@@ -61,20 +70,57 @@
 ]
 typecheck = [
   "mypy --strict ./quivr ./examples ./test/typing_tests",
 ]
 test = [
   "pytest --benchmark-disable ./test",
 ]
+doctest = [
+  "pytest --doctest-modules ./quivr"
+]
 benchmark = [
   "pytest --benchmark-only ./test"
 ]
+gauntlet = [
+   "hatch run lint",
+   "hatch run typecheck",
+   "hatch run test",
+   "hatch run doctest",
+]
+
+[tool.hatch.envs.docs]
+dependencies = [
+  "sphinx==7.0.1",
+  "sphinx-autodoc-typehints",
+  "sphinx-copybutton",
+  "sphinx-toolbox",
+  "furo",
+]
+
+[tool.hatch.envs.docs.scripts]
+make-html = [
+  "make -C docs html"
+]
+
+open-docs = [
+  "open docs/build/html/index.html"
+]
+
+clean-html = [
+  "make -C docs clean"
+]
+
+rebuild-html = [
+  "make -C docs clean",
+  "make -C docs html"
+]
 
 [tool.black]
 line-length = 110
 
 [tool.isort]
 profile = "black"
 
 [tool.ruff]
 line-length = 110
 target-version = "py311"
+
```

### Comparing `quivr-0.4.3/PKG-INFO` & `quivr-0.5.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 Metadata-Version: 2.1
 Name: quivr
-Version: 0.4.3
+Version: 0.5.0
 Summary: Container library for working with tabular Arrow data
 Project-URL: Source, https://github.com/spenczar/quivr
 Author-email: Spencer Nelson <spencer@spencerwnelson.com>
 License-File: LICENSE
 Requires-Python: >=3.9
 Requires-Dist: mmh3
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: pyarrow
 Requires-Dist: typing-extensions>=4.0.0
+Provides-Extra: docs
+Requires-Dist: furo; extra == 'docs'
+Requires-Dist: sphinx-autodoc-typehints; extra == 'docs'
+Requires-Dist: sphinx-copybutton; extra == 'docs'
+Requires-Dist: sphinx-toolbox; extra == 'docs'
+Requires-Dist: sphinx==7.0.1; extra == 'docs'
 Description-Content-Type: text/markdown
 
 # quivr
 
 Quivr is a Python library which provides great containers for Arrow data.
 
 Quivr's `Table`s are like DataFrames, but with strict schemas to
```

