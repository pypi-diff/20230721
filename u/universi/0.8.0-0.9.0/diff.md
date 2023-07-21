# Comparing `tmp/universi-0.8.0.tar.gz` & `tmp/universi-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "universi-0.8.0.tar", max compression
+gzip compressed data, was "universi-0.9.0.tar", max compression
```

## Comparing `universi-0.8.0.tar` & `universi-0.9.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1072 2023-06-12 19:09:15.569998 universi-0.8.0/LICENSE
--rw-r--r--   0        0        0    10813 2023-07-16 21:30:00.123318 universi-0.8.0/README.md
--rw-r--r--   0        0        0     4072 2023-07-18 06:54:59.346664 universi-0.8.0/pyproject.toml
--rw-r--r--   0        0        0      453 2023-07-12 22:40:12.864421 universi-0.8.0/universi/__init__.py
--rw-r--r--   0        0        0     2821 2023-07-14 12:35:15.746665 universi-0.8.0/universi/_utils.py
--rw-r--r--   0        0        0    22420 2023-07-18 06:54:15.303331 universi-0.8.0/universi/codegen.py
--rw-r--r--   0        0        0      324 2023-07-10 23:48:56.035792 universi-0.8.0/universi/exceptions.py
--rw-r--r--   0        0        0     2841 2023-07-08 14:21:11.688092 universi-0.8.0/universi/fields.py
--rw-r--r--   0        0        0      903 2023-07-06 22:52:01.148105 universi-0.8.0/universi/header.py
--rw-r--r--   0        0        0        0 2023-07-13 08:09:29.390618 universi-0.8.0/universi/py.typed
--rw-r--r--   0        0        0    12077 2023-07-16 13:58:23.713333 universi-0.8.0/universi/routing.py
--rw-r--r--   0        0        0      426 2023-07-16 13:09:25.456661 universi-0.8.0/universi/structure/__init__.py
--rw-r--r--   0        0        0      265 2023-07-08 11:43:06.913473 universi-0.8.0/universi/structure/common.py
--rw-r--r--   0        0        0     4936 2023-07-10 10:22:38.358870 universi-0.8.0/universi/structure/endpoints.py
--rw-r--r--   0        0        0      944 2023-07-08 11:43:06.913473 universi-0.8.0/universi/structure/enums.py
--rw-r--r--   0        0        0     1270 2023-07-14 12:35:15.266665 universi-0.8.0/universi/structure/responses.py
--rw-r--r--   0        0        0     6058 2023-07-16 13:58:29.106666 universi-0.8.0/universi/structure/schemas.py
--rw-r--r--   0        0        0     9545 2023-07-16 13:09:26.053328 universi-0.8.0/universi/structure/versions.py
--rw-r--r--   0        0        0    11713 1970-01-01 00:00:00.000000 universi-0.8.0/setup.py
--rw-r--r--   0        0        0    11400 1970-01-01 00:00:00.000000 universi-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-06-12 19:09:15.569998 universi-0.9.0/LICENSE
+-rw-r--r--   0        0        0    21640 2023-07-21 21:25:34.939997 universi-0.9.0/README.md
+-rw-r--r--   0        0        0     4072 2023-07-21 18:16:55.923321 universi-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      453 2023-07-12 22:40:12.864421 universi-0.9.0/universi/__init__.py
+-rw-r--r--   0        0        0     2821 2023-07-14 12:35:15.746665 universi-0.9.0/universi/_utils.py
+-rw-r--r--   0        0        0    22420 2023-07-18 06:54:15.303331 universi-0.9.0/universi/codegen.py
+-rw-r--r--   0        0        0      324 2023-07-10 23:48:56.035792 universi-0.9.0/universi/exceptions.py
+-rw-r--r--   0        0        0     2841 2023-07-08 14:21:11.688092 universi-0.9.0/universi/fields.py
+-rw-r--r--   0        0        0      903 2023-07-06 22:52:01.148105 universi-0.9.0/universi/header.py
+-rw-r--r--   0        0        0        0 2023-07-13 08:09:29.390618 universi-0.9.0/universi/py.typed
+-rw-r--r--   0        0        0    12077 2023-07-16 13:58:23.713333 universi-0.9.0/universi/routing.py
+-rw-r--r--   0        0        0      426 2023-07-16 13:09:25.456661 universi-0.9.0/universi/structure/__init__.py
+-rw-r--r--   0        0        0      265 2023-07-08 11:43:06.913473 universi-0.9.0/universi/structure/common.py
+-rw-r--r--   0        0        0     4936 2023-07-10 10:22:38.358870 universi-0.9.0/universi/structure/endpoints.py
+-rw-r--r--   0        0        0      944 2023-07-08 11:43:06.913473 universi-0.9.0/universi/structure/enums.py
+-rw-r--r--   0        0        0     1270 2023-07-14 12:35:15.266665 universi-0.9.0/universi/structure/responses.py
+-rw-r--r--   0        0        0     6058 2023-07-16 13:58:29.106666 universi-0.9.0/universi/structure/schemas.py
+-rw-r--r--   0        0        0     9907 2023-07-21 21:10:28.899997 universi-0.9.0/universi/structure/versions.py
+-rw-r--r--   0        0        0    22824 1970-01-01 00:00:00.000000 universi-0.9.0/setup.py
+-rw-r--r--   0        0        0    22227 1970-01-01 00:00:00.000000 universi-0.9.0/PKG-INFO
```

### Comparing `universi-0.8.0/LICENSE` & `universi-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `universi-0.8.0/pyproject.toml` & `universi-0.9.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "universi"
-version = "0.8.0"
+version = "0.9.0"
 description = ""
 authors = ["Stanislav Zmiev <szmiev2000@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/ovsyanka83/universi"
 
 [tool.poetry.dependencies]
```

### Comparing `universi-0.8.0/universi/_utils.py` & `universi-0.9.0/universi/_utils.py`

 * *Files identical despite different names*

### Comparing `universi-0.8.0/universi/codegen.py` & `universi-0.9.0/universi/codegen.py`

 * *Files identical despite different names*

### Comparing `universi-0.8.0/universi/fields.py` & `universi-0.9.0/universi/fields.py`

 * *Files identical despite different names*

### Comparing `universi-0.8.0/universi/header.py` & `universi-0.9.0/universi/header.py`

 * *Files identical despite different names*

### Comparing `universi-0.8.0/universi/routing.py` & `universi-0.9.0/universi/routing.py`

 * *Files identical despite different names*

### Comparing `universi-0.8.0/universi/structure/endpoints.py` & `universi-0.9.0/universi/structure/endpoints.py`

 * *Files identical despite different names*

### Comparing `universi-0.8.0/universi/structure/enums.py` & `universi-0.9.0/universi/structure/enums.py`

 * *Files identical despite different names*

### Comparing `universi-0.8.0/universi/structure/responses.py` & `universi-0.9.0/universi/structure/responses.py`

 * *Files identical despite different names*

### Comparing `universi-0.8.0/universi/structure/schemas.py` & `universi-0.9.0/universi/structure/schemas.py`

 * *Files identical despite different names*

### Comparing `universi-0.8.0/universi/structure/versions.py` & `universi-0.9.0/universi/structure/versions.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,32 +17,24 @@
 from .common import Endpoint, VersionedModel
 from .responses import AlterResponseInstruction
 from .schemas import AlterSchemaSubInstruction, SchemaPropertyDefinitionInstruction
 
 _P = ParamSpec("_P")
 _R = TypeVar("_R")
 VersionDate: TypeAlias = datetime.date
-PossibleInstructions: TypeAlias = (
-    AlterSchemaSubInstruction | AlterEndpointSubInstruction | AlterEnumSubInstruction
-)
+PossibleInstructions: TypeAlias = AlterSchemaSubInstruction | AlterEndpointSubInstruction | AlterEnumSubInstruction
 
 
 class VersionChange:
     description: ClassVar[str] = Sentinel
-    instructions_to_migrate_to_previous_version: ClassVar[
-        Sequence[PossibleInstructions]
-    ] = Sentinel
+    instructions_to_migrate_to_previous_version: ClassVar[Sequence[PossibleInstructions]] = Sentinel
     alter_schema_instructions: ClassVar[Sequence[AlterSchemaSubInstruction]] = Sentinel
     alter_enum_instructions: ClassVar[Sequence[AlterEnumSubInstruction]] = Sentinel
-    alter_endpoint_instructions: ClassVar[
-        Sequence[AlterEndpointSubInstruction]
-    ] = Sentinel
-    alter_response_instructions: ClassVar[
-        dict[Endpoint, AlterResponseInstruction]
-    ] = Sentinel
+    alter_endpoint_instructions: ClassVar[Sequence[AlterEndpointSubInstruction]] = Sentinel
+    alter_response_instructions: ClassVar[dict[Endpoint, AlterResponseInstruction]] = Sentinel
 
     def __init_subclass__(cls, _abstract: bool = False) -> None:
         if _abstract:
             return
         if cls.description is Sentinel:
             raise UniversiStructureError(
                 f"Version change description is not set on '{cls.__name__}' but is required.",
@@ -155,16 +147,15 @@
             raise ValueError(
                 "Versions are not sorted correctly. Please sort them in descending order.",
             )
 
     @functools.cached_property
     def versioned_schemas(self) -> dict[str, type[VersionedModel]]:
         return {
-            instruction.schema.__module__
-            + instruction.schema.__name__: instruction.schema
+            instruction.schema.__module__ + instruction.schema.__name__: instruction.schema
             for version in self.versions
             for version_change in version.version_changes
             for instruction in version_change.alter_schema_instructions
         }
 
     @functools.cached_property
     def versioned_enums(self) -> dict[str, type[Enum]]:
@@ -175,27 +166,34 @@
             for instruction in version_change.alter_enum_instructions
         }
 
     @functools.cached_property
     def _version_changes_to_version_mapping(
         self,
     ) -> dict[type[VersionChange], VersionDate]:
-        return {
-            version_change: version.date
-            for version in self.versions
-            for version_change in version.version_changes
-        }
+        return {version_change: version.date for version in self.versions for version_change in version.version_changes}
 
     # TODO: It might need caching for iteration to speed it up
     def data_to_version(
         self,
         endpoint: Endpoint,
         data: dict[str, Any],
         version: VersionDate,
     ) -> dict[str, Any]:
+        """Convert the data to a specific version by applying all version changes in reverse order.
+
+        Args:
+            endpoint: the function which usually returns this data. Data migrations marked with this endpoint will
+            be applied to the passed data
+            data: data to be migrated. Will be mutated during the call
+            version: the version to which the data should be converted
+
+        Returns:
+            Modified data
+        """
         for v in self.versions:
             if v.date <= version:
                 break
             for version_change in v.version_changes:
                 if endpoint in version_change.alter_response_instructions:
                     version_change.alter_response_instructions[endpoint](data)
         return data
```

