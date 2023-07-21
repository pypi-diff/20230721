# Comparing `tmp/examon_core-1.0.7.tar.gz` & `tmp/examon_core-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "examon_core-1.0.7.tar", max compression
+gzip compressed data, was "examon_core-1.0.8.tar", max compression
```

## Comparing `examon_core-1.0.7.tar` & `examon_core-1.0.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      199 2023-05-28 20:39:21.972747 examon_core-1.0.7/examon_core/__init__.py
--rw-r--r--   0        0        0     1039 2023-07-16 08:19:13.878728 examon_core-1.0.7/examon_core/code_metrics.py
--rwxr-xr-x   0        0        0      574 2023-07-17 15:50:11.694400 examon_core-1.0.7/examon_core/examon_item.py
--rwxr-xr-x   0        0        0     1531 2023-07-18 13:36:47.779723 examon_core-1.0.7/examon_core/examon_item_registry.py
--rwxr-xr-x   0        0        0     1697 2023-07-16 08:20:56.019327 examon_core-1.0.7/examon_core/function_raw_code.py
--rw-r--r--   0        0        0      408 2023-07-16 08:19:13.774401 examon_core-1.0.7/examon_core/multi_choice_factory.py
--rw-r--r--   0        0        0      980 2023-07-16 08:19:13.846489 examon_core-1.0.7/examon_core/print_ext.py
--rwxr-xr-x   0        0        0      620 2023-07-16 08:19:13.933636 examon_core-1.0.7/examon_core/question.py
--rw-r--r--   0        0        0     2850 2023-07-18 20:38:10.761164 examon_core-1.0.7/examon_core/question_factory.py
--rwxr-xr-x   0        0        0      201 2023-07-15 15:48:50.722464 examon_core-1.0.7/examon_core/question_response.py
--rw-r--r--   0        0        0      107 2023-07-17 15:48:04.895960 examon_core-1.0.7/examon_core/todo.md
--rw-r--r--   0        0        0      517 2023-07-18 20:40:27.926998 examon_core-1.0.7/pyproject.toml
--rw-r--r--   0        0        0      461 1970-01-01 00:00:00.000000 examon_core-1.0.7/PKG-INFO
+-rw-r--r--   0        0        0      199 2023-05-28 20:39:21.972747 examon_core-1.0.8/examon_core/__init__.py
+-rw-r--r--   0        0        0     1039 2023-07-16 08:19:13.878728 examon_core-1.0.8/examon_core/code_metrics.py
+-rwxr-xr-x   0        0        0      574 2023-07-17 15:50:11.694400 examon_core-1.0.8/examon_core/examon_item.py
+-rwxr-xr-x   0        0        0     1606 2023-07-21 16:14:24.632842 examon_core-1.0.8/examon_core/examon_item_registry.py
+-rwxr-xr-x   0        0        0     1697 2023-07-16 08:20:56.019327 examon_core-1.0.8/examon_core/function_raw_code.py
+-rw-r--r--   0        0        0      408 2023-07-16 08:19:13.774401 examon_core-1.0.8/examon_core/multi_choice_factory.py
+-rw-r--r--   0        0        0      980 2023-07-16 08:19:13.846489 examon_core-1.0.8/examon_core/print_ext.py
+-rwxr-xr-x   0        0        0      620 2023-07-16 08:19:13.933636 examon_core-1.0.8/examon_core/question.py
+-rw-r--r--   0        0        0     2855 2023-07-20 08:28:48.400131 examon_core-1.0.8/examon_core/question_factory.py
+-rwxr-xr-x   0        0        0      201 2023-07-15 15:48:50.722464 examon_core-1.0.8/examon_core/question_response.py
+-rw-r--r--   0        0        0      107 2023-07-17 15:48:04.895960 examon_core-1.0.8/examon_core/todo.md
+-rw-r--r--   0        0        0      517 2023-07-21 16:16:23.994600 examon_core-1.0.8/pyproject.toml
+-rw-r--r--   0        0        0      461 1970-01-01 00:00:00.000000 examon_core-1.0.8/PKG-INFO
```

### Comparing `examon_core-1.0.7/examon_core/code_metrics.py` & `examon_core-1.0.8/examon_core/code_metrics.py`

 * *Files identical despite different names*

### Comparing `examon_core-1.0.7/examon_core/examon_item.py` & `examon_core-1.0.8/examon_core/examon_item.py`

 * *Files identical despite different names*

### Comparing `examon_core-1.0.7/examon_core/function_raw_code.py` & `examon_core-1.0.8/examon_core/function_raw_code.py`

 * *Files identical despite different names*

### Comparing `examon_core-1.0.7/examon_core/print_ext.py` & `examon_core-1.0.8/examon_core/print_ext.py`

 * *Files identical despite different names*

### Comparing `examon_core-1.0.7/examon_core/question.py` & `examon_core-1.0.8/examon_core/question.py`

 * *Files identical despite different names*

### Comparing `examon_core-1.0.7/examon_core/question_factory.py` & `examon_core-1.0.8/examon_core/question_factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,10 +78,10 @@
             return result
         except Exception as e:
             return repr(e)
 
     @staticmethod
     def run_function_with_param(function, param):
         try:
-            return function(param)
+            return str(function(param))
         except Exception as e:
             return repr(e)
```

### Comparing `examon_core-1.0.7/pyproject.toml` & `examon_core-1.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "examon_core"
-version = "1.0.7"
+version = "1.0.8"
 description = "Examon Core Libs"
 authors = ["Jarrod Folino <jdfolino@icloud.com>"]
 packages = [{include = "examon_core"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 radon = "^6.0.1"
```

