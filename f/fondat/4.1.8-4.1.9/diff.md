# Comparing `tmp/fondat-4.1.8.tar.gz` & `tmp/fondat-4.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fondat-4.1.8.tar", max compression
+gzip compressed data, was "fondat-4.1.9.tar", max compression
```

## Comparing `fondat-4.1.8.tar` & `fondat-4.1.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1054 2023-02-01 22:27:57.731621 fondat-4.1.8/LICENSE
--rw-r--r--   0        0        0      817 2022-06-01 04:36:45.561693 fondat-4.1.8/README.md
--rw-r--r--   0        0        0     1477 2022-05-31 23:18:30.030138 fondat-4.1.8/fondat/annotation.py
--rw-r--r--   0        0        0     5213 2023-05-07 17:30:10.420228 fondat-4.1.8/fondat/asgi.py
--rw-r--r--   0        0        0      923 2023-02-01 23:37:21.447708 fondat-4.1.8/fondat/cache.py
--rw-r--r--   0        0        0    47875 2023-07-16 23:51:26.184751 fondat-4.1.8/fondat/codec.py
--rw-r--r--   0        0        0     5810 2023-05-05 04:34:02.260758 fondat-4.1.8/fondat/context.py
--rw-r--r--   0        0        0    10842 2023-05-27 21:01:55.538544 fondat-4.1.8/fondat/csv.py
--rw-r--r--   0        0        0     9119 2023-02-01 23:37:21.447708 fondat-4.1.8/fondat/data.py
--rw-r--r--   0        0        0     2444 2023-07-11 20:44:25.310120 fondat-4.1.8/fondat/error.py
--rw-r--r--   0        0        0     6552 2023-05-27 21:04:21.481983 fondat-4.1.8/fondat/file.py
--rw-r--r--   0        0        0    19284 2023-02-01 23:37:21.447708 fondat-4.1.8/fondat/http.py
--rw-r--r--   0        0        0     4501 2022-10-20 06:46:29.449990 fondat-4.1.8/fondat/lazy.py
--rw-r--r--   0        0        0     4155 2023-01-03 22:30:55.181857 fondat-4.1.8/fondat/memory.py
--rw-r--r--   0        0        0     4438 2022-10-17 21:06:57.865002 fondat-4.1.8/fondat/monitor.py
--rw-r--r--   0        0        0      521 2023-06-21 21:23:41.913723 fondat-4.1.8/fondat/oauth.py
--rw-r--r--   0        0        0    31467 2022-10-21 02:52:32.452813 fondat-4.1.8/fondat/openapi.py
--rw-r--r--   0        0        0     2584 2023-06-15 06:32:27.349190 fondat-4.1.8/fondat/pagination.py
--rw-r--r--   0        0        0     2130 2022-10-17 03:49:58.147449 fondat-4.1.8/fondat/patch.py
--rw-r--r--   0        0        0    11552 2023-07-11 21:43:50.415822 fondat-4.1.8/fondat/resource.py
--rw-r--r--   0        0        0     1828 2022-05-30 16:49:00.995761 fondat-4.1.8/fondat/security.py
--rw-r--r--   0        0        0    28028 2023-06-21 21:23:42.117056 fondat-4.1.8/fondat/sql.py
--rw-r--r--   0        0        0    10965 2023-06-21 21:11:33.842694 fondat-4.1.8/fondat/sqlite.py
--rw-r--r--   0        0        0     6541 2023-05-27 21:03:43.828608 fondat-4.1.8/fondat/stream.py
--rw-r--r--   0        0        0     2293 2022-10-17 18:55:29.684237 fondat-4.1.8/fondat/string.py
--rw-r--r--   0        0        0     6393 2022-12-05 21:33:22.805679 fondat-4.1.8/fondat/types.py
--rw-r--r--   0        0        0    13873 2023-07-17 00:04:51.967963 fondat-4.1.8/fondat/validation.py
--rw-r--r--   0        0        0     1171 2023-07-17 00:05:42.774849 fondat-4.1.8/pyproject.toml
--rw-r--r--   0        0        0     1684 1970-01-01 00:00:00.000000 fondat-4.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1054 2023-02-01 22:27:57.731621 fondat-4.1.9/LICENSE
+-rw-r--r--   0        0        0      817 2022-06-01 04:36:45.561693 fondat-4.1.9/README.md
+-rw-r--r--   0        0        0     1477 2022-05-31 23:18:30.030138 fondat-4.1.9/fondat/annotation.py
+-rw-r--r--   0        0        0     5213 2023-05-07 17:30:10.420228 fondat-4.1.9/fondat/asgi.py
+-rw-r--r--   0        0        0      923 2023-02-01 23:37:21.447708 fondat-4.1.9/fondat/cache.py
+-rw-r--r--   0        0        0    47875 2023-07-16 23:51:26.184751 fondat-4.1.9/fondat/codec.py
+-rw-r--r--   0        0        0     5810 2023-05-05 04:34:02.260758 fondat-4.1.9/fondat/context.py
+-rw-r--r--   0        0        0    10842 2023-05-27 21:01:55.538544 fondat-4.1.9/fondat/csv.py
+-rw-r--r--   0        0        0     9119 2023-02-01 23:37:21.447708 fondat-4.1.9/fondat/data.py
+-rw-r--r--   0        0        0     2444 2023-07-11 20:44:25.310120 fondat-4.1.9/fondat/error.py
+-rw-r--r--   0        0        0     6552 2023-05-27 21:04:21.481983 fondat-4.1.9/fondat/file.py
+-rw-r--r--   0        0        0    19284 2023-02-01 23:37:21.447708 fondat-4.1.9/fondat/http.py
+-rw-r--r--   0        0        0     4501 2022-10-20 06:46:29.449990 fondat-4.1.9/fondat/lazy.py
+-rw-r--r--   0        0        0     4155 2023-01-03 22:30:55.181857 fondat-4.1.9/fondat/memory.py
+-rw-r--r--   0        0        0     4438 2022-10-17 21:06:57.865002 fondat-4.1.9/fondat/monitor.py
+-rw-r--r--   0        0        0      521 2023-06-21 21:23:41.913723 fondat-4.1.9/fondat/oauth.py
+-rw-r--r--   0        0        0    31467 2022-10-21 02:52:32.452813 fondat-4.1.9/fondat/openapi.py
+-rw-r--r--   0        0        0     2584 2023-06-15 06:32:27.349190 fondat-4.1.9/fondat/pagination.py
+-rw-r--r--   0        0        0     2130 2022-10-17 03:49:58.147449 fondat-4.1.9/fondat/patch.py
+-rw-r--r--   0        0        0    11552 2023-07-11 21:43:50.415822 fondat-4.1.9/fondat/resource.py
+-rw-r--r--   0        0        0     1828 2022-05-30 16:49:00.995761 fondat-4.1.9/fondat/security.py
+-rw-r--r--   0        0        0    28028 2023-06-21 21:23:42.117056 fondat-4.1.9/fondat/sql.py
+-rw-r--r--   0        0        0    10965 2023-06-21 21:11:33.842694 fondat-4.1.9/fondat/sqlite.py
+-rw-r--r--   0        0        0     6541 2023-05-27 21:03:43.828608 fondat-4.1.9/fondat/stream.py
+-rw-r--r--   0        0        0     2270 2023-07-20 23:12:32.911542 fondat-4.1.9/fondat/string.py
+-rw-r--r--   0        0        0     6393 2022-12-05 21:33:22.805679 fondat-4.1.9/fondat/types.py
+-rw-r--r--   0        0        0    13857 2023-07-17 16:44:25.817139 fondat-4.1.9/fondat/validation.py
+-rw-r--r--   0        0        0     1171 2023-07-20 23:28:09.376052 fondat-4.1.9/pyproject.toml
+-rw-r--r--   0        0        0     1684 1970-01-01 00:00:00.000000 fondat-4.1.9/PKG-INFO
```

### Comparing `fondat-4.1.8/LICENSE` & `fondat-4.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `fondat-4.1.8/README.md` & `fondat-4.1.9/README.md`

 * *Files identical despite different names*

### Comparing `fondat-4.1.8/fondat/annotation.py` & `fondat-4.1.9/fondat/annotation.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.8/fondat/asgi.py` & `fondat-4.1.9/fondat/asgi.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.8/fondat/cache.py` & `fondat-4.1.9/fondat/cache.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.8/fondat/codec.py` & `fondat-4.1.9/fondat/codec.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.8/fondat/context.py` & `fondat-4.1.9/fondat/context.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.8/fondat/csv.py` & `fondat-4.1.9/fondat/csv.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.8/fondat/data.py` & `fondat-4.1.9/fondat/data.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.8/fondat/error.py` & `fondat-4.1.9/fondat/error.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.8/fondat/file.py` & `fondat-4.1.9/fondat/file.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.8/fondat/http.py` & `fondat-4.1.9/fondat/http.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.8/fondat/lazy.py` & `fondat-4.1.9/fondat/lazy.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.8/fondat/memory.py` & `fondat-4.1.9/fondat/memory.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.8/fondat/monitor.py` & `fondat-4.1.9/fondat/monitor.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.8/fondat/oauth.py` & `fondat-4.1.9/fondat/oauth.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.8/fondat/openapi.py` & `fondat-4.1.9/fondat/openapi.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.8/fondat/pagination.py` & `fondat-4.1.9/fondat/pagination.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.8/fondat/patch.py` & `fondat-4.1.9/fondat/patch.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.8/fondat/resource.py` & `fondat-4.1.9/fondat/resource.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.8/fondat/security.py` & `fondat-4.1.9/fondat/security.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.8/fondat/sql.py` & `fondat-4.1.9/fondat/sql.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.8/fondat/sqlite.py` & `fondat-4.1.9/fondat/sqlite.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.8/fondat/stream.py` & `fondat-4.1.9/fondat/stream.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.8/fondat/string.py` & `fondat-4.1.9/fondat/string.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,36 +15,36 @@
 
     A substition expression in the template takes the form "${...}". For example, if a
     template contains "${foo}" substitution expression, then "foo" is the value that is passed
     to a resolver coroutine to be resolved. A subsitution expression cannot span lines
     within the template string.
     """
 
-    _pattern = re.compile(r"\$\{(.*?)}")
+    _pattern = re.compile(r"\${(.*)}")
 
     def __init__(self, template: str):
         self.template = template
 
     async def _resolve(
         self, template: str, resolver: Callable[[str], Coroutine[Any, Any, str | None]]
     ) -> str:
         segments = []
         for line in template.splitlines(keepends=True):
             index = 0
             while match := self._pattern.search(line[index:]):
                 group = match.group(1)
                 resolved = None
-                if resolved := await resolver(group):
-                    span = match.span()
-                    segments.append(line[index : span[0]])
-                    segments.append(await self._resolve(resolved, resolver))
-                    index = span[1]
-                    break
-                if not resolved:
+                resolved = await resolver(group)
+                if resolved is None:
                     raise ValueError(f"could not resolve ${{{group}}} in template")
+                span = match.span()
+                segments.append(line[index : span[0]])
+                segments.append(await self._resolve(resolved, resolver))
+                index = span[1]
+                break
             segments.append(line[index:])
         return "".join(segments)
 
     async def resolve(self, resolver: Callable[[str], Coroutine[Any, Any, str | None]]) -> str:
         """
         Return a new string with resolved template substitutions.
```

### Comparing `fondat-4.1.8/fondat/types.py` & `fondat-4.1.9/fondat/types.py`

 * *Files identical despite different names*

### Comparing `fondat-4.1.8/fondat/validation.py` & `fondat-4.1.9/fondat/validation.py`

 * *Files 1% similar despite different names*

```diff
@@ -450,13 +450,12 @@
 
     Parameters:
     • errors: object to add error to
     • message: human-readable error message
     • path: path to the attribute that is the subject of the validation error
     • code: machine-readable error code
     """
-    if condition:  # validation passed
-        return
-    error = ValidationError(message=message, path=path, code=code)
-    if errors is None:
-        raise error
-    errors.add(error)
+    if not condition:
+        error = ValidationError(message=message, path=path, code=code)
+        if errors is None:
+            raise error
+        errors.add(error)
```

### Comparing `fondat-4.1.8/pyproject.toml` & `fondat-4.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.black]
 line-length = 96
 target-version = ['py310']
 
 [tool.poetry]
 name = "fondat"
-version = "4.1.8"
+version = "4.1.9"
 description = "A foundation for resource-oriented backend applications."
 readme = "README.md"
 authors = ["fondat authors"]
 homepage = "https://github.com/fondat/fondat/"
 documentation = "https://github.com/fondat/fondat/tree/main/docs"
 license = "MIT"
 keywords = ["asgi", "foundation", "resource", "openapi"]
```

### Comparing `fondat-4.1.8/PKG-INFO` & `fondat-4.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fondat
-Version: 4.1.8
+Version: 4.1.9
 Summary: A foundation for resource-oriented backend applications.
 Home-page: https://github.com/fondat/fondat/
 License: MIT
 Keywords: asgi,foundation,resource,openapi
 Author: fondat authors
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

