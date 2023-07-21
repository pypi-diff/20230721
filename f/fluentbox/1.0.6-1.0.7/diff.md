# Comparing `tmp/fluentbox-1.0.6.tar.gz` & `tmp/fluentbox-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fluentbox-1.0.6.tar", last modified: Mon Jul 10 10:02:32 2023, max compression
+gzip compressed data, was "fluentbox-1.0.7.tar", last modified: Fri Jul 21 09:45:52 2023, max compression
```

## Comparing `fluentbox-1.0.6.tar` & `fluentbox-1.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-10 10:02:32.756944 fluentbox-1.0.6/
--rw-rw-r--   0 alex      (1000) alex      (1000)       53 2023-07-10 10:02:32.756944 fluentbox-1.0.6/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)       90 2023-03-23 19:38:01.000000 fluentbox-1.0.6/pyproject.toml
--rw-rw-r--   0 alex      (1000) alex      (1000)      212 2023-07-10 10:02:32.756944 fluentbox-1.0.6/setup.cfg
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-10 10:02:32.756944 fluentbox-1.0.6/src/
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-10 10:02:32.756944 fluentbox-1.0.6/src/fluentbox/
--rw-rw-r--   0 alex      (1000) alex      (1000)      239 2023-01-27 09:52:59.000000 fluentbox-1.0.6/src/fluentbox/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    14836 2023-07-10 09:59:12.000000 fluentbox-1.0.6/src/fluentbox/fluentbox.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-10 10:02:32.756944 fluentbox-1.0.6/src/fluentbox.egg-info/
--rw-rw-r--   0 alex      (1000) alex      (1000)       53 2023-07-10 10:02:32.000000 fluentbox-1.0.6/src/fluentbox.egg-info/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)      249 2023-07-10 10:02:32.000000 fluentbox-1.0.6/src/fluentbox.egg-info/SOURCES.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-07-10 10:02:32.000000 fluentbox-1.0.6/src/fluentbox.egg-info/dependency_links.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       10 2023-07-10 10:02:32.000000 fluentbox-1.0.6/src/fluentbox.egg-info/top_level.txt
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-10 10:02:32.756944 fluentbox-1.0.6/tests/
--rw-rw-r--   0 alex      (1000) alex      (1000)    14996 2023-01-30 16:45:01.000000 fluentbox-1.0.6/tests/test_fluentbox.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-21 09:45:52.589906 fluentbox-1.0.7/
+-rw-rw-r--   0 alex      (1000) alex      (1000)       53 2023-07-21 09:45:52.589906 fluentbox-1.0.7/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)       90 2023-03-23 19:38:01.000000 fluentbox-1.0.7/pyproject.toml
+-rw-rw-r--   0 alex      (1000) alex      (1000)      212 2023-07-21 09:45:52.589906 fluentbox-1.0.7/setup.cfg
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-21 09:45:52.589906 fluentbox-1.0.7/src/
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-21 09:45:52.589906 fluentbox-1.0.7/src/fluentbox/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      239 2023-01-27 09:52:59.000000 fluentbox-1.0.7/src/fluentbox/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    15183 2023-07-21 09:36:29.000000 fluentbox-1.0.7/src/fluentbox/fluentbox.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-21 09:45:52.589906 fluentbox-1.0.7/src/fluentbox.egg-info/
+-rw-rw-r--   0 alex      (1000) alex      (1000)       53 2023-07-21 09:45:52.000000 fluentbox-1.0.7/src/fluentbox.egg-info/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)      249 2023-07-21 09:45:52.000000 fluentbox-1.0.7/src/fluentbox.egg-info/SOURCES.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-07-21 09:45:52.000000 fluentbox-1.0.7/src/fluentbox.egg-info/dependency_links.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       10 2023-07-21 09:45:52.000000 fluentbox-1.0.7/src/fluentbox.egg-info/top_level.txt
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-21 09:45:52.589906 fluentbox-1.0.7/tests/
+-rw-rw-r--   0 alex      (1000) alex      (1000)    14996 2023-01-30 16:45:01.000000 fluentbox-1.0.7/tests/test_fluentbox.py
```

### Comparing `fluentbox-1.0.6/src/fluentbox/fluentbox.py` & `fluentbox-1.0.7/src/fluentbox/fluentbox.py`

 * *Files 2% similar despite different names*

```diff
@@ -368,14 +368,22 @@
     def only(self, keys: abc.Iterable[abc.Hashable]) -> MappingBox:
         # noinspection PyUnusedLocal
         def callback(key: abc.Hashable, value: Any) -> bool:
             return key in keys
 
         return self.filter(callback)
 
+    def map_with_keys(self, callback: abc.Callable[[abc.Hashable, Any], tuple[abc.Hashable, Any]]) -> MutableMappingBox:
+        result = {}
+        for key, value in self.items():
+            result_key, result_value = callback(key, value)
+            result[result_key] = result_value
+
+        return cast(MutableMappingBox, self._new(result))
+
 
 class MutableMappingBox(MappingBox, abc.MutableMapping):
     _items: abc.MutableMapping
 
     def __setitem__(self, key: abc.Hashable, value: Any) -> None:
         self._items[key] = value
```

### Comparing `fluentbox-1.0.6/tests/test_fluentbox.py` & `fluentbox-1.0.7/tests/test_fluentbox.py`

 * *Files identical despite different names*

