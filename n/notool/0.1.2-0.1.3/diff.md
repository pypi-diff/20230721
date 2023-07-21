# Comparing `tmp/notool-0.1.2-py3-none-any.whl.zip` & `tmp/notool-0.1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 35850 bytes, number of entries: 11
--rw-rw-rw-  2.0 fat      671 b- defN 23-Mar-03 08:42 notool/__init__.py
--rw-rw-rw-  2.0 fat   110415 b- defN 23-Mar-03 08:42 notool/data_container.py
--rw-rw-rw-  2.0 fat     5710 b- defN 23-Mar-03 08:42 notool/dataclass_ex.py
--rw-rw-rw-  2.0 fat     8506 b- defN 23-Mar-03 08:42 notool/enum_ex.py
--rw-rw-rw-  2.0 fat     1722 b- defN 23-Mar-03 08:42 notool/helpers.py
--rw-rw-rw-  2.0 fat      796 b- defN 23-Mar-03 08:42 notool/utils.py
--rw-rw-rw-  2.0 fat     1096 b- defN 23-Mar-03 08:42 notool-0.1.2.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      832 b- defN 23-Mar-03 08:42 notool-0.1.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Mar-03 08:42 notool-0.1.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        7 b- defN 23-Mar-03 08:42 notool-0.1.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      834 b- defN 23-Mar-03 08:42 notool-0.1.2.dist-info/RECORD
-11 files, 130681 bytes uncompressed, 34458 bytes compressed:  73.6%
+Zip file size: 35751 bytes, number of entries: 11
+-rw-rw-rw-  2.0 fat      671 b- defN 23-Jul-21 08:03 notool/__init__.py
+-rw-rw-rw-  2.0 fat   110415 b- defN 23-Jul-21 08:03 notool/data_container.py
+-rw-rw-rw-  2.0 fat     5284 b- defN 23-Jul-21 08:03 notool/dataclass_ex.py
+-rw-rw-rw-  2.0 fat     8506 b- defN 23-Jul-21 08:03 notool/enum_ex.py
+-rw-rw-rw-  2.0 fat     1722 b- defN 23-Jul-21 08:03 notool/helpers.py
+-rw-rw-rw-  2.0 fat      800 b- defN 23-Jul-21 08:03 notool/utils.py
+-rw-rw-rw-  2.0 fat     1096 b- defN 23-Jul-21 08:03 notool-0.1.3.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      832 b- defN 23-Jul-21 08:03 notool-0.1.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-21 08:03 notool-0.1.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        7 b- defN 23-Jul-21 08:03 notool-0.1.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      834 b- defN 23-Jul-21 08:03 notool-0.1.3.dist-info/RECORD
+11 files, 130259 bytes uncompressed, 34359 bytes compressed:  73.6%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: notool/helpers.py
 Comment: 
 
 Filename: notool/utils.py
 Comment: 
 
-Filename: notool-0.1.2.dist-info/LICENSE
+Filename: notool-0.1.3.dist-info/LICENSE
 Comment: 
 
-Filename: notool-0.1.2.dist-info/METADATA
+Filename: notool-0.1.3.dist-info/METADATA
 Comment: 
 
-Filename: notool-0.1.2.dist-info/WHEEL
+Filename: notool-0.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: notool-0.1.2.dist-info/top_level.txt
+Filename: notool-0.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: notool-0.1.2.dist-info/RECORD
+Filename: notool-0.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## notool/__init__.py

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.1.2'
+__version__ = '0.1.3'
 
 from .utils import (
     get_var_name,
     wraps_hint,
     start_generator,
     functools_cache
 )
```

## notool/dataclass_ex.py

```diff
@@ -1,62 +1,51 @@
 import datetime
 import functools
+import time
 from dataclasses import dataclass
 import typing as t
 from enum import EnumMeta
 
 import orjson
-from dacite import from_dict, core, UnionMatchError, Config
+from dacite import from_dict, core, Config
+from dacite.exceptions import DaciteFieldError
 
 _T = t.TypeVar("_T")
 
 
-def _transform_value(type_hooks, cast, target_type, value):
-    args = t.get_args(target_type)
-    target_type = t.get_origin(target_type) or target_type
-    try:
-        if target_type is dict and args and (key_type := args[0]):
-            # key_type_args = t.get_args(key_type)
-            # key_type = t.get_origin(key_type) or key_type
-            if key_type is str:
-                pass
-            # TODO orjson not supported tuple as dict keys
-            # elif key_type is tuple and key_type_args:
-            #     if len(key_type_args) > 1 or \
-            #             (key_type_args := key_type_args[0]) not in (int, float, str):
-            #         raise NotImplementedError
-            #     return {tuple(map(key_type_args, key[1:-1].split(','))): val
-            #             for key, val in value.items()}
-            elif key_type in (int, float):
-                return {key_type(key): val for key, val in value.items()}
-            else:
-                raise NotImplementedError
-        elif target_type in (bytes, bytearray, memoryview) and isinstance(value, str):
-            return str.encode(value, 'charmap')
-        elif hasattr(target_type, '_asdict'):  # for namedtuple
-            return target_type(**value)
-        elif target_type in (int, float) or isinstance(target_type, EnumMeta) or target_type is tuple:
-            return target_type(value if value is not None else '')
-        elif target_type is datetime.datetime:
-            return datetime.datetime.fromisoformat(value)
-    except ValueError:
-        raise KeyError
-
-    return super_transform_value(type_hooks, cast, target_type, value)
-
-
 def _build_value(type_, data, config):
+    origin_type = t.get_origin(type_) or type_
     try:
+        if origin_type is dict:
+            args = t.get_args(type_)
+            if args and (key_type := args[0]):
+                if key_type is str:
+                    pass
+                elif key_type in (int, float):
+                    data = {key_type(key): val for key, val in data.items()}
+                else:
+                    # TODO orjson not supported tuple as dict keys
+                    raise NotImplementedError
+        elif origin_type is type(data):
+            ...
+        elif origin_type in (bytes, bytearray, memoryview) and isinstance(data, str):
+            data = str.encode(data, 'charmap')
+        elif hasattr(origin_type, '_asdict'):  # for namedtuple
+            data = origin_type(**data)
+        elif origin_type in (int, float) or isinstance(origin_type, EnumMeta) or origin_type is tuple:
+            data = origin_type(data if data is not None else '')
+        elif origin_type is datetime.datetime:
+            data = datetime.datetime.fromisoformat(data)
+
         return super_build_value(type_, data, config)
-    except UnionMatchError:
-        raise KeyError
+
+    except ValueError:
+        raise DaciteFieldError
 
 
-super_transform_value = getattr(core, 'transform_value')
-setattr(core, 'transform_value', _transform_value)
 super_build_value = getattr(core, '_build_value')
 setattr(core, '_build_value', _build_value)
 
 
 def _orjson_default(obj):
     if hasattr(obj, '_asdict'):
         return obj._asdict()
@@ -127,26 +116,34 @@
         @dataclass
         class TestData(Serializable):
             field0: bytes = b'default\n'
             field1: Data._T = Data1.data1a
             field2: float = 2.0
             field3: dict = field(default_factory=lambda: {'test_field': 2})
             field4: list[TestForList] = field(default_factory=list)
+            field5: t.Optional[datetime.datetime] = None
 
         list_ = []
         for i in range(10):
             dict_ = {}
             for j in range(10):
                 test_for_dict = TestForDict(EbcParams(i, i, i), j)
                 dict_.update({j: test_for_dict})
             a = bool(i % 2)
             tuple_ = EbcParams(i, i, i) if a else (str(i), i)
             list_.append(TestForList(Data1.data1a, (i, i), a, tuple_, dict_))
 
         for test_data in (TestData(b'default\n', Data2.data2a, 14.2, {'test_field2': 22}),
-                          TestData(b'default\n', Data2.data2a, 14.2, {'test_field2': 22}, list_)):
-            test_data_loads = orjson.loads(orjson.dumps(test_data, default=_orjson_default, option=orjson.OPT_NON_STR_KEYS))
-            test_data_dacite = from_dict(TestData, test_data_loads, )  # Config(cast=[Data], check_types=True))
-            assert test_data == test_data_dacite
-            assert test_data == TestData.loads(test_data.dumps())
+                          TestData(b'default\n', Data2.data2a, 14.2, {'test_field2': 22},
+                                   list_, datetime.datetime.now())):
+            test_data_loads = orjson.loads(
+                orjson.dumps(test_data, default=_orjson_default, option=orjson.OPT_NON_STR_KEYS))
+            assert (test_data
+                    == from_dict(TestData, test_data_loads)
+                    == TestData.loads(test_data.dumps()))
+        else:
+            start = time.monotonic()
+            for _ in range(1000):
+                TestData.loads(test_data_loads)
+            print(time.monotonic() - start)
 
     _tests()
```

## notool/utils.py

```diff
@@ -6,18 +6,20 @@
 
 C = t.TypeVar('C')
 
 
 def wraps_hint(decorator: C) -> C:
     return decorator
 
+
 @wraps_hint
 def functools_cache(func):
     return functools.cache(func)
 
+
 @wraps_hint
 def start_generator(func):
     @functools.wraps(func)
     def wrapper(*args, **kwargs):
         generator = func(*args, **kwargs)
         next(generator)
         return generator
```

## Comparing `notool-0.1.2.dist-info/LICENSE` & `notool-0.1.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `notool-0.1.2.dist-info/METADATA` & `notool-0.1.3.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notool
-Version: 0.1.2
+Version: 0.1.3
 Summary: Different handies
 Home-page: https://github.com/means0nothing/Notool
 Author: Pavel Shevcov
 Author-email: means0nothing@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -14,11 +14,11 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy (>=1.23.1)
 Requires-Dist: rdp (==0.8)
-Requires-Dist: dacite (==1.6.0)
+Requires-Dist: dacite (==1.8.1)
 Requires-Dist: orjson (==3.8.1)
 
 Different handies
```

## Comparing `notool-0.1.2.dist-info/RECORD` & `notool-0.1.3.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-notool/__init__.py,sha256=-cLF3F1VfdIVvGDGn7Beua2w_LhlW1H012ESVnF_KAw,671
+notool/__init__.py,sha256=60vwqNpj3kO-Fzvkj4ry2eFZqPsATo_gvpT8Uf24SVY,671
 notool/data_container.py,sha256=E1A-gF3M_3WjVoMFJayOmIj1ZibDc8vLujZL8VoIkmc,110415
-notool/dataclass_ex.py,sha256=kXjNZtTBMJbbbjFW4CDy3R03tdEvPdAZWpU2coArtvs,5710
+notool/dataclass_ex.py,sha256=hiGpaE1VQ-1lRYD_Eyk1QUymCAVFFef5u3uCYXyuwr4,5284
 notool/enum_ex.py,sha256=uBud9wgqrEDkdDFPowgGevmsdBAxsSXfbT1o0X1EjqQ,8506
 notool/helpers.py,sha256=en6i3OZCXVZ_3qaH4keHUCWRmE7fSn073ldgq9o2qBQ,1722
-notool/utils.py,sha256=Y_Or3EVfEuVkSabAoav0iqMpRLcaJgQIwAPZYRE8-Rw,796
-notool-0.1.2.dist-info/LICENSE,sha256=KOI2v5c_M5MQQkVqxM4BBqmkZnNAh6PYV-3Q9pTInWE,1096
-notool-0.1.2.dist-info/METADATA,sha256=SWxqATCMC3BCq3kdMCR42Bt1VEuIjsNbW8azv6tvMfE,832
-notool-0.1.2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-notool-0.1.2.dist-info/top_level.txt,sha256=6Hb7XWnIGyAyQUL6dnjSZwjShKUC_EXtzG3KMqQ4ZZ4,7
-notool-0.1.2.dist-info/RECORD,,
+notool/utils.py,sha256=EEPD-HPq1_WU3VYDqTqaMN-hPeHTbxI4rePu0WdKY00,800
+notool-0.1.3.dist-info/LICENSE,sha256=KOI2v5c_M5MQQkVqxM4BBqmkZnNAh6PYV-3Q9pTInWE,1096
+notool-0.1.3.dist-info/METADATA,sha256=tLdPEqX8za0iiyCV8gP4aQXqXWPZA-yOPp746XBB4qQ,832
+notool-0.1.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+notool-0.1.3.dist-info/top_level.txt,sha256=6Hb7XWnIGyAyQUL6dnjSZwjShKUC_EXtzG3KMqQ4ZZ4,7
+notool-0.1.3.dist-info/RECORD,,
```

