# Comparing `tmp/polyfactory-2.6.2.tar.gz` & `tmp/polyfactory-2.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polyfactory-2.6.2.tar", max compression
+gzip compressed data, was "polyfactory-2.6.3.tar", max compression
```

## Comparing `polyfactory-2.6.2.tar` & `polyfactory-2.6.3.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     1092 2023-07-14 15:44:51.527690 polyfactory-2.6.2/LICENSE
--rw-r--r--   0        0        0    24136 2023-07-14 15:44:51.527690 polyfactory-2.6.2/docs/PYPI_README.md
--rw-r--r--   0        0        0      425 2023-07-14 15:44:51.531690 polyfactory-2.6.2/polyfactory/__init__.py
--rw-r--r--   0        0        0     2525 2023-07-14 15:44:51.531690 polyfactory-2.6.2/polyfactory/collection_extender.py
--rw-r--r--   0        0        0      912 2023-07-14 15:44:51.531690 polyfactory-2.6.2/polyfactory/constants.py
--rw-r--r--   0        0        0     1037 2023-07-14 15:44:51.531690 polyfactory-2.6.2/polyfactory/decorators.py
--rw-r--r--   0        0        0      591 2023-07-14 15:44:51.531690 polyfactory-2.6.2/polyfactory/exceptions.py
--rw-r--r--   0        0        0      257 2023-07-14 15:44:51.531690 polyfactory-2.6.2/polyfactory/factories/__init__.py
--rw-r--r--   0        0        0    33713 2023-07-14 15:44:51.531690 polyfactory-2.6.2/polyfactory/factories/base.py
--rw-r--r--   0        0        0     2758 2023-07-14 15:44:51.531690 polyfactory-2.6.2/polyfactory/factories/beanie_odm_factory.py
--rw-r--r--   0        0        0     1912 2023-07-14 15:44:51.531690 polyfactory-2.6.2/polyfactory/factories/dataclass_factory.py
--rw-r--r--   0        0        0     2751 2023-07-14 15:44:51.531690 polyfactory-2.6.2/polyfactory/factories/msgspec_factory.py
--rw-r--r--   0        0        0     2192 2023-07-14 15:44:51.531690 polyfactory-2.6.2/polyfactory/factories/odmantic_odm_factory.py
--rw-r--r--   0        0        0    13803 2023-07-14 15:44:51.531690 polyfactory-2.6.2/polyfactory/factories/pydantic_factory.py
--rw-r--r--   0        0        0     1699 2023-07-14 15:44:51.531690 polyfactory-2.6.2/polyfactory/factories/typed_dict_factory.py
--rw-r--r--   0        0        0     8246 2023-07-14 15:44:51.531690 polyfactory-2.6.2/polyfactory/field_meta.py
--rw-r--r--   0        0        0     3317 2023-07-14 15:44:51.531690 polyfactory-2.6.2/polyfactory/fields.py
--rw-r--r--   0        0        0     1192 2023-07-14 15:44:51.531690 polyfactory-2.6.2/polyfactory/persistence.py
--rw-r--r--   0        0        0        0 2023-07-14 15:44:51.531690 polyfactory-2.6.2/polyfactory/py.typed
--rw-r--r--   0        0        0     2850 2023-07-14 15:44:51.531690 polyfactory-2.6.2/polyfactory/pytest_plugin.py
--rw-r--r--   0        0        0        0 2023-07-14 15:44:51.531690 polyfactory-2.6.2/polyfactory/utils/__init__.py
--rw-r--r--   0        0        0     3908 2023-07-14 15:44:51.531690 polyfactory-2.6.2/polyfactory/utils/helpers.py
--rw-r--r--   0        0        0     3764 2023-07-14 15:44:51.531690 polyfactory-2.6.2/polyfactory/utils/predicates.py
--rw-r--r--   0        0        0        0 2023-07-14 15:44:51.531690 polyfactory-2.6.2/polyfactory/value_generators/__init__.py
--rw-r--r--   0        0        0     1948 2023-07-14 15:44:51.531690 polyfactory-2.6.2/polyfactory/value_generators/complex_types.py
--rw-r--r--   0        0        0     1885 2023-07-14 15:44:51.531690 polyfactory-2.6.2/polyfactory/value_generators/constrained_collections.py
--rw-r--r--   0        0        0     1125 2023-07-14 15:44:51.531690 polyfactory-2.6.2/polyfactory/value_generators/constrained_dates.py
--rw-r--r--   0        0        0    13429 2023-07-14 15:44:51.531690 polyfactory-2.6.2/polyfactory/value_generators/constrained_numbers.py
--rw-r--r--   0        0        0      433 2023-07-14 15:44:51.531690 polyfactory-2.6.2/polyfactory/value_generators/constrained_path.py
--rw-r--r--   0        0        0     3846 2023-07-14 15:44:51.531690 polyfactory-2.6.2/polyfactory/value_generators/constrained_strings.py
--rw-r--r--   0        0        0      440 2023-07-14 15:44:51.531690 polyfactory-2.6.2/polyfactory/value_generators/constrained_url.py
--rw-r--r--   0        0        0      446 2023-07-14 15:44:51.531690 polyfactory-2.6.2/polyfactory/value_generators/constrained_uuid.py
--rw-r--r--   0        0        0     3635 2023-07-14 15:44:51.531690 polyfactory-2.6.2/polyfactory/value_generators/primitives.py
--rw-r--r--   0        0        0     6172 2023-07-14 15:44:51.531690 polyfactory-2.6.2/polyfactory/value_generators/regex.py
--rw-r--r--   0        0        0     6777 2023-07-14 15:44:51.531690 polyfactory-2.6.2/pyproject.toml
--rw-r--r--   0        0        0    26005 1970-01-01 00:00:00.000000 polyfactory-2.6.2/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-07-21 15:24:49.338390 polyfactory-2.6.3/LICENSE
+-rw-r--r--   0        0        0    24136 2023-07-21 15:24:49.338390 polyfactory-2.6.3/docs/PYPI_README.md
+-rw-r--r--   0        0        0      425 2023-07-21 15:24:49.342390 polyfactory-2.6.3/polyfactory/__init__.py
+-rw-r--r--   0        0        0     2525 2023-07-21 15:24:49.342390 polyfactory-2.6.3/polyfactory/collection_extender.py
+-rw-r--r--   0        0        0      912 2023-07-21 15:24:49.342390 polyfactory-2.6.3/polyfactory/constants.py
+-rw-r--r--   0        0        0     1037 2023-07-21 15:24:49.342390 polyfactory-2.6.3/polyfactory/decorators.py
+-rw-r--r--   0        0        0      591 2023-07-21 15:24:49.342390 polyfactory-2.6.3/polyfactory/exceptions.py
+-rw-r--r--   0        0        0      257 2023-07-21 15:24:49.342390 polyfactory-2.6.3/polyfactory/factories/__init__.py
+-rw-r--r--   0        0        0    33713 2023-07-21 15:24:49.342390 polyfactory-2.6.3/polyfactory/factories/base.py
+-rw-r--r--   0        0        0     2758 2023-07-21 15:24:49.342390 polyfactory-2.6.3/polyfactory/factories/beanie_odm_factory.py
+-rw-r--r--   0        0        0     1912 2023-07-21 15:24:49.342390 polyfactory-2.6.3/polyfactory/factories/dataclass_factory.py
+-rw-r--r--   0        0        0     2751 2023-07-21 15:24:49.342390 polyfactory-2.6.3/polyfactory/factories/msgspec_factory.py
+-rw-r--r--   0        0        0     2192 2023-07-21 15:24:49.342390 polyfactory-2.6.3/polyfactory/factories/odmantic_odm_factory.py
+-rw-r--r--   0        0        0    14047 2023-07-21 15:24:49.342390 polyfactory-2.6.3/polyfactory/factories/pydantic_factory.py
+-rw-r--r--   0        0        0     1699 2023-07-21 15:24:49.342390 polyfactory-2.6.3/polyfactory/factories/typed_dict_factory.py
+-rw-r--r--   0        0        0     8621 2023-07-21 15:24:49.342390 polyfactory-2.6.3/polyfactory/field_meta.py
+-rw-r--r--   0        0        0     3317 2023-07-21 15:24:49.342390 polyfactory-2.6.3/polyfactory/fields.py
+-rw-r--r--   0        0        0     1192 2023-07-21 15:24:49.342390 polyfactory-2.6.3/polyfactory/persistence.py
+-rw-r--r--   0        0        0        0 2023-07-21 15:24:49.342390 polyfactory-2.6.3/polyfactory/py.typed
+-rw-r--r--   0        0        0     2850 2023-07-21 15:24:49.342390 polyfactory-2.6.3/polyfactory/pytest_plugin.py
+-rw-r--r--   0        0        0        0 2023-07-21 15:24:49.342390 polyfactory-2.6.3/polyfactory/utils/__init__.py
+-rw-r--r--   0        0        0     3908 2023-07-21 15:24:49.342390 polyfactory-2.6.3/polyfactory/utils/helpers.py
+-rw-r--r--   0        0        0     3764 2023-07-21 15:24:49.342390 polyfactory-2.6.3/polyfactory/utils/predicates.py
+-rw-r--r--   0        0        0        0 2023-07-21 15:24:49.342390 polyfactory-2.6.3/polyfactory/value_generators/__init__.py
+-rw-r--r--   0        0        0     1948 2023-07-21 15:24:49.342390 polyfactory-2.6.3/polyfactory/value_generators/complex_types.py
+-rw-r--r--   0        0        0     1885 2023-07-21 15:24:49.342390 polyfactory-2.6.3/polyfactory/value_generators/constrained_collections.py
+-rw-r--r--   0        0        0     1125 2023-07-21 15:24:49.342390 polyfactory-2.6.3/polyfactory/value_generators/constrained_dates.py
+-rw-r--r--   0        0        0    13429 2023-07-21 15:24:49.342390 polyfactory-2.6.3/polyfactory/value_generators/constrained_numbers.py
+-rw-r--r--   0        0        0      433 2023-07-21 15:24:49.342390 polyfactory-2.6.3/polyfactory/value_generators/constrained_path.py
+-rw-r--r--   0        0        0     3846 2023-07-21 15:24:49.342390 polyfactory-2.6.3/polyfactory/value_generators/constrained_strings.py
+-rw-r--r--   0        0        0      440 2023-07-21 15:24:49.342390 polyfactory-2.6.3/polyfactory/value_generators/constrained_url.py
+-rw-r--r--   0        0        0      446 2023-07-21 15:24:49.342390 polyfactory-2.6.3/polyfactory/value_generators/constrained_uuid.py
+-rw-r--r--   0        0        0     3635 2023-07-21 15:24:49.342390 polyfactory-2.6.3/polyfactory/value_generators/primitives.py
+-rw-r--r--   0        0        0     6172 2023-07-21 15:24:49.342390 polyfactory-2.6.3/polyfactory/value_generators/regex.py
+-rw-r--r--   0        0        0     6914 2023-07-21 15:24:49.342390 polyfactory-2.6.3/pyproject.toml
+-rw-r--r--   0        0        0    26109 1970-01-01 00:00:00.000000 polyfactory-2.6.3/PKG-INFO
```

### Comparing `polyfactory-2.6.2/LICENSE` & `polyfactory-2.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `polyfactory-2.6.2/docs/PYPI_README.md` & `polyfactory-2.6.3/docs/PYPI_README.md`

 * *Files identical despite different names*

### Comparing `polyfactory-2.6.2/polyfactory/collection_extender.py` & `polyfactory-2.6.3/polyfactory/collection_extender.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.6.2/polyfactory/constants.py` & `polyfactory-2.6.3/polyfactory/constants.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.6.2/polyfactory/decorators.py` & `polyfactory-2.6.3/polyfactory/decorators.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.6.2/polyfactory/exceptions.py` & `polyfactory-2.6.3/polyfactory/exceptions.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.6.2/polyfactory/factories/base.py` & `polyfactory-2.6.3/polyfactory/factories/base.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.6.2/polyfactory/factories/beanie_odm_factory.py` & `polyfactory-2.6.3/polyfactory/factories/beanie_odm_factory.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.6.2/polyfactory/factories/dataclass_factory.py` & `polyfactory-2.6.3/polyfactory/factories/dataclass_factory.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.6.2/polyfactory/factories/msgspec_factory.py` & `polyfactory-2.6.3/polyfactory/factories/msgspec_factory.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.6.2/polyfactory/factories/odmantic_odm_factory.py` & `polyfactory-2.6.3/polyfactory/factories/odmantic_odm_factory.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.6.2/polyfactory/factories/pydantic_factory.py` & `polyfactory-2.6.3/polyfactory/factories/pydantic_factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,14 +65,17 @@
     ) -> PydanticFieldMeta:
         """Create an instance from a pydantic field info.
 
         :param field_name: The name of the field.
         :param field_info: A pydantic FieldInfo instance.
         :param use_alias: Whether to use the field alias.
         :param random: A random.Random instance.
+        :param randomize_collection_length: Whether to randomize collection length.
+        :param min_collection_length: Minimum collection length.
+        :param max_collection_length: Maximum collection length.
 
         :returns: A PydanticFieldMeta instance.
         """
         if callable(field_info.default_factory):
             default_value = field_info.default_factory()
         else:
             default_value = field_info.default if field_info.default is not Undefined else Null
@@ -269,15 +272,15 @@
 
         """
         if "_fields_metadata" not in cls.__dict__:
             if VERSION.startswith("1"):
                 cls._fields_metadata = [
                     PydanticFieldMeta.from_model_field(
                         field,
-                        use_alias=not cls.__model__.__config__.allow_population_by_field_name,
+                        use_alias=not cls.__model__.__config__.allow_population_by_field_name,  # type: ignore[attr-defined]
                         random=cls.__random__,
                         randomize_collection_length=cls.__randomize_collection_length__,
                         min_collection_length=cls.__min_collection_length__,
                         max_collection_length=cls.__max_collection_length__,
                     )
                     for field in cls.__model__.__fields__.values()  # type: ignore[attr-defined]
                 ]
```

### Comparing `polyfactory-2.6.2/polyfactory/factories/typed_dict_factory.py` & `polyfactory-2.6.3/polyfactory/factories/typed_dict_factory.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.6.2/polyfactory/field_meta.py` & `polyfactory-2.6.3/polyfactory/field_meta.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from __future__ import annotations
 
 from dataclasses import asdict, is_dataclass
 from typing import TYPE_CHECKING, Any, Literal, Pattern, TypedDict, cast
 
+from typing_extensions import get_args, get_origin
+
 from polyfactory.collection_extender import CollectionExtender
 from polyfactory.constants import (
     DEFAULT_RANDOM,
     MAX_COLLECTION_LENGTH,
     MIN_COLLECTION_LENGTH,
     RANDOMIZE_COLLECTION_LENGTH,
     TYPE_MAPPING,
@@ -127,22 +129,29 @@
         """
         field_type = normalize_annotation(annotation, random=random)
 
         if not constraints and is_annotated(annotation):
             _, metadata = unwrap_annotated(annotation, random=random)
             constraints = cls.parse_constraints(metadata)
 
+        if not any(is_annotated(arg) for arg in get_args(annotation)):
+            annotation = TYPE_MAPPING[field_type] if field_type in TYPE_MAPPING else field_type
+        elif (origin := get_origin(annotation)) and origin in TYPE_MAPPING:  # pragma: no cover
+            container = TYPE_MAPPING[origin]
+            annotation = container[get_args(annotation)]  # type: ignore
+
         field = cls(
-            annotation=TYPE_MAPPING[field_type] if field_type in TYPE_MAPPING else field_type,
+            annotation=annotation,
             random=random,
             name=name,
             default=default,
             children=None,
             constraints=constraints,
         )
+
         if field.type_args:
             if randomize_collection_length:
                 number_of_args = random.randint(min_collection_length, max_collection_length)
             else:
                 number_of_args = 1
 
             extended_type_args = CollectionExtender.extend_type_args(field.annotation, field.type_args, number_of_args)
```

### Comparing `polyfactory-2.6.2/polyfactory/fields.py` & `polyfactory-2.6.3/polyfactory/fields.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.6.2/polyfactory/persistence.py` & `polyfactory-2.6.3/polyfactory/persistence.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.6.2/polyfactory/pytest_plugin.py` & `polyfactory-2.6.3/polyfactory/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.6.2/polyfactory/utils/helpers.py` & `polyfactory-2.6.3/polyfactory/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.6.2/polyfactory/utils/predicates.py` & `polyfactory-2.6.3/polyfactory/utils/predicates.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.6.2/polyfactory/value_generators/complex_types.py` & `polyfactory-2.6.3/polyfactory/value_generators/complex_types.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.6.2/polyfactory/value_generators/constrained_collections.py` & `polyfactory-2.6.3/polyfactory/value_generators/constrained_collections.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.6.2/polyfactory/value_generators/constrained_dates.py` & `polyfactory-2.6.3/polyfactory/value_generators/constrained_dates.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.6.2/polyfactory/value_generators/constrained_numbers.py` & `polyfactory-2.6.3/polyfactory/value_generators/constrained_numbers.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.6.2/polyfactory/value_generators/constrained_strings.py` & `polyfactory-2.6.3/polyfactory/value_generators/constrained_strings.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.6.2/polyfactory/value_generators/primitives.py` & `polyfactory-2.6.3/polyfactory/value_generators/primitives.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.6.2/polyfactory/value_generators/regex.py` & `polyfactory-2.6.3/polyfactory/value_generators/regex.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.6.2/pyproject.toml` & `polyfactory-2.6.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "polyfactory"
-version = "2.6.2"
+version = "2.6.3"
 description = "Mock data generation factories"
 authors = [
     "Na'aman Hirschfeld <nhirschfeld@gmail.com>",
     "Cody Fincher <cody.fincher@gmail.com>",
     "Janek Nouvertné <provinzkraut@posteo.de>",
     "Jacob Coffee <jacob@z7x.org>",
 ]
@@ -58,46 +58,56 @@
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
 beanie = { version = "*", optional = true }
 faker = "*"
 msgspec = { version = "*", optional = true }
 odmantic = { version = "*", optional = true }
-pydantic = { version = "*", optional = true }
+pydantic = { version = "*", optional = true, extras = ["email"] }
 typing-extensions = "*"
 
 [tool.poetry.group.dev.dependencies]
-annotated-types = "*"
-beanie = "*"
-email-validator = "*"
 hypothesis = "*"
 mongomock-motor = "*"
-msgspec = "*"
-odmantic = "*"
-pre-commit = "*"
-pydantic = ">=2"
 pytest = "*"
 pytest-asyncio = "*"
 pytest-cov = "*"
-sourcery = "*"
 
 [tool.poetry.group.docs.dependencies]
 auto-pytabs = "*"
 blacken-docs = "*"
 litestar-sphinx-theme = { git = "https://github.com/litestar-org/litestar-sphinx-theme.git" }
 sphinx = "*"
 sphinx-autobuild = "*"
 sphinx-copybutton = "*"
 sphinxcontrib-mermaid = "*"
 
+[tool.poetry.group.lint]
+optional = true
+
+[tool.poetry.group.lint.dependencies]
+black = "*"
+blacken-docs = "*"
+mypy = "*"
+pre-commit = "*"
+pyright = "*"
+ruff = '*'
+sourcery = "*"
+
 [tool.poetry.extras]
 pydantic = ["pydantic"]
 msgspec = ["msgspec"]
 odmantic = ["odmantic", "pydantic"]
 beanie = ["beanie", "pydantic"]
+full = [
+    "pydantic",
+    "odmantic",
+    "msgspec",
+    "beanie",
+]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 120
```

### Comparing `polyfactory-2.6.2/PKG-INFO` & `polyfactory-2.6.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polyfactory
-Version: 2.6.2
+Version: 2.6.3
 Summary: Mock data generation factories
 Home-page: https://github.com/litestar-org/polyfactory
 License: MIT
 Keywords: beanie,dataclasses,factory,faker,litestar,mock,msgspec,odmantic,pydantic,pytest,tdd,testing,typeddict
 Author: Na'aman Hirschfeld
 Author-email: nhirschfeld@gmail.com
 Maintainer: Na'aman Hirschfeld
@@ -26,22 +26,23 @@
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Software Development :: Testing :: Unit
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Provides-Extra: beanie
+Provides-Extra: full
 Provides-Extra: msgspec
 Provides-Extra: odmantic
 Provides-Extra: pydantic
-Requires-Dist: beanie ; extra == "beanie"
+Requires-Dist: beanie ; extra == "beanie" or extra == "full"
 Requires-Dist: faker
-Requires-Dist: msgspec ; extra == "msgspec"
-Requires-Dist: odmantic ; extra == "odmantic"
-Requires-Dist: pydantic ; extra == "pydantic" or extra == "odmantic" or extra == "beanie"
+Requires-Dist: msgspec ; extra == "msgspec" or extra == "full"
+Requires-Dist: odmantic ; extra == "odmantic" or extra == "full"
+Requires-Dist: pydantic[email] ; extra == "pydantic" or extra == "odmantic" or extra == "beanie" or extra == "full"
 Requires-Dist: typing-extensions
 Project-URL: Documentation, https://github.com/litestar-org/polyfactory
 Project-URL: Repository, https://github.com/litestar-org/polyfactory
 Description-Content-Type: text/markdown
 
 <!-- markdownlint-disable -->
 <p align="center">
```

