# Comparing `tmp/zrouter-0.3.6.tar.gz` & `tmp/zrouter-0.3.7.tar.gz`

## Comparing `zrouter-0.3.6.tar` & `zrouter-0.3.7.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     2375 2020-02-02 00:00:00.000000 zrouter-0.3.6/src/zrouter/__init__.py
--rw-r--r--   0        0        0     2407 2020-02-02 00:00:00.000000 zrouter-0.3.6/src/zrouter/decorator.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 zrouter-0.3.6/src/zrouter/exception.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 zrouter-0.3.6/LICENSE
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 zrouter-0.3.6/README.md
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 zrouter-0.3.6/pyproject.toml
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 zrouter-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0     2539 2020-02-02 00:00:00.000000 zrouter-0.3.7/src/zrouter/__init__.py
+-rw-r--r--   0        0        0     2407 2020-02-02 00:00:00.000000 zrouter-0.3.7/src/zrouter/decorator.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 zrouter-0.3.7/src/zrouter/exception.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 zrouter-0.3.7/LICENSE
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 zrouter-0.3.7/README.md
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 zrouter-0.3.7/pyproject.toml
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 zrouter-0.3.7/PKG-INFO
```

### Comparing `zrouter-0.3.6/src/zrouter/__init__.py` & `zrouter-0.3.7/src/zrouter/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from flask import Blueprint, request
 from zrouter.exception import MessagePrompt
 from inspirare import json as json_
 from json import JSONDecodeError
+from jsonschema.exceptions import ValidationError
 from functools import wraps
 
 
 class RouterUtility:
     @staticmethod
     def get_params():
         """ 获取路由参数"""
@@ -45,17 +46,19 @@
             def func_wrapper(func):
                 @wraps(func)
                 def wrapper(*args, **kwargs):
                     params = self.clean_params(self.get_params())
                     if not self.authorized and not open:
                         return {'code': 401, 'msg': '用户无权限'}
                     try:
-                        data = func(params)
+                        data = func(**params)
                     except MessagePrompt as e:
                         return {'code': 500, 'msg': str(e)}
+                    except ValidationError as e:
+                        return {'code': 400, 'msg': str(e)}
                     if direct:
                         return data
                     if isinstance(data, dict):
                         data = json_.iter_camel(data)
                     elif isinstance(data, list):
                         data = [json_.iter_camel(item) for item in data]
                     return {'code': 200, 'msg': '操作成功', 'data': data}
```

### Comparing `zrouter-0.3.6/src/zrouter/decorator.py` & `zrouter-0.3.7/src/zrouter/decorator.py`

 * *Files identical despite different names*

### Comparing `zrouter-0.3.6/LICENSE` & `zrouter-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `zrouter-0.3.6/pyproject.toml` & `zrouter-0.3.7/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "zrouter"
-version = "0.3.6"
+version = "0.3.7"
 authors = [
   { name="inspirare6", email="inspirare6@163.com" },
 ]
 description = "zen router library"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
   "flask==2.2.2",
-  "jsonschema==4.17.3",
   "inspirare",
+  "jsonschema"
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `zrouter-0.3.6/PKG-INFO` & `zrouter-0.3.7/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: zrouter
-Version: 0.3.6
+Version: 0.3.7
 Summary: zen router library
 Project-URL: Homepage, https://github.com/inspirare6/zrouter
 Project-URL: Bug Tracker, https://github.com/inspirare6/zrouter/issues
 Author-email: inspirare6 <inspirare6@163.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Requires-Dist: flask==2.2.2
 Requires-Dist: inspirare
-Requires-Dist: jsonschema==4.17.3
+Requires-Dist: jsonschema
 Description-Content-Type: text/markdown
 
 # ztime
 
 Zen time library.
```

