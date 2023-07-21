# Comparing `tmp/mypy-boto3-1.28.8.tar.gz` & `tmp/mypy-boto3-1.28.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-1.28.8.tar", last modified: Thu Jul 20 19:47:56 2023, max compression
+gzip compressed data, was "mypy-boto3-1.28.9.tar", last modified: Fri Jul 21 20:32:58 2023, max compression
```

## Comparing `mypy-boto3-1.28.8.tar` & `mypy-boto3-1.28.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:47:56.000775 mypy-boto3-1.28.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-20 19:46:33.000000 mypy-boto3-1.28.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-07-20 19:47:55.996775 mypy-boto3-1.28.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-07-20 19:46:33.000000 mypy-boto3-1.28.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:47:55.992775 mypy-boto3-1.28.8/mypy_boto3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 19:46:35.000000 mypy-boto3-1.28.8/mypy_boto3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-20 19:46:35.000000 mypy-boto3-1.28.8/mypy_boto3/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-20 19:46:33.000000 mypy-boto3-1.28.8/mypy_boto3/boto3_init.py
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-20 19:46:33.000000 mypy-boto3-1.28.8/mypy_boto3/boto3_init_stub.py
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-20 19:46:35.000000 mypy-boto3-1.28.8/mypy_boto3/boto3_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-07-20 19:46:33.000000 mypy-boto3-1.28.8/mypy_boto3/boto3_session_stub.py
--rw-r--r--   0 runner    (1001) docker     (123)    14083 2023-07-20 19:46:35.000000 mypy-boto3-1.28.8/mypy_boto3/main.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 19:46:33.000000 mypy-boto3-1.28.8/mypy_boto3/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   106280 2023-07-20 19:46:35.000000 mypy-boto3-1.28.8/mypy_boto3/submodules.py
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-20 19:46:33.000000 mypy-boto3-1.28.8/mypy_boto3/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:47:55.996775 mypy-boto3-1.28.8/mypy_boto3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-07-20 19:47:55.000000 mypy-boto3-1.28.8/mypy_boto3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-20 19:47:55.000000 mypy-boto3-1.28.8/mypy_boto3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 19:47:55.000000 mypy-boto3-1.28.8/mypy_boto3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 19:47:55.000000 mypy-boto3-1.28.8/mypy_boto3.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-20 19:47:55.000000 mypy-boto3-1.28.8/mypy_boto3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-20 19:47:55.000000 mypy-boto3-1.28.8/mypy_boto3.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 19:47:56.000775 mypy-boto3-1.28.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-07-20 19:46:33.000000 mypy-boto3-1.28.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:32:58.251903 mypy-boto3-1.28.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-21 20:31:55.000000 mypy-boto3-1.28.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-07-21 20:32:58.251903 mypy-boto3-1.28.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-07-21 20:31:55.000000 mypy-boto3-1.28.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:32:58.231903 mypy-boto3-1.28.9/mypy_boto3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 20:31:57.000000 mypy-boto3-1.28.9/mypy_boto3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-21 20:31:57.000000 mypy-boto3-1.28.9/mypy_boto3/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-21 20:31:55.000000 mypy-boto3-1.28.9/mypy_boto3/boto3_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-21 20:31:55.000000 mypy-boto3-1.28.9/mypy_boto3/boto3_init_stub.py
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-21 20:31:57.000000 mypy-boto3-1.28.9/mypy_boto3/boto3_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-07-21 20:31:55.000000 mypy-boto3-1.28.9/mypy_boto3/boto3_session_stub.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14083 2023-07-21 20:31:57.000000 mypy-boto3-1.28.9/mypy_boto3/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 20:31:55.000000 mypy-boto3-1.28.9/mypy_boto3/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   106280 2023-07-21 20:31:57.000000 mypy-boto3-1.28.9/mypy_boto3/submodules.py
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-21 20:31:55.000000 mypy-boto3-1.28.9/mypy_boto3/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:32:58.251903 mypy-boto3-1.28.9/mypy_boto3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-07-21 20:32:58.000000 mypy-boto3-1.28.9/mypy_boto3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-21 20:32:58.000000 mypy-boto3-1.28.9/mypy_boto3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 20:32:58.000000 mypy-boto3-1.28.9/mypy_boto3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 20:32:58.000000 mypy-boto3-1.28.9/mypy_boto3.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-21 20:32:58.000000 mypy-boto3-1.28.9/mypy_boto3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-21 20:32:58.000000 mypy-boto3-1.28.9/mypy_boto3.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 20:32:58.251903 mypy-boto3-1.28.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-07-21 20:31:55.000000 mypy-boto3-1.28.9/setup.py
```

### Comparing `mypy-boto3-1.28.8/LICENSE` & `mypy-boto3-1.28.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-1.28.8/PKG-INFO` & `mypy-boto3-1.28.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3
-Version: 1.28.8
-Summary: Type annotations for boto3 1.28.8 master module generated with mypy-boto3-builder 7.15.1
+Version: 1.28.9
+Summary: Type annotations for boto3 1.28.9 master module generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3.svg?color=blue)](https://pypi.org/project/mypy-boto3)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3?color=blue)](https://pypistats.org/packages/mypy-boto3)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Dynamic
-[boto3 1.28.8](https://boto3.amazonaws.com/v1/documentation/api/1.28.8/index.html)
+[boto3 1.28.9](https://boto3.amazonaws.com/v1/documentation/api/1.28.9/index.html)
 type annotations builder for
 [boto3-stubs](https://pypi.org/project/boto3-stubs/).
 
 Generated by
 [mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
```

### Comparing `mypy-boto3-1.28.8/README.md` & `mypy-boto3-1.28.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3.svg?color=blue)](https://pypi.org/project/mypy-boto3)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3?color=blue)](https://pypistats.org/packages/mypy-boto3)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Dynamic
-[boto3 1.28.8](https://boto3.amazonaws.com/v1/documentation/api/1.28.8/index.html)
+[boto3 1.28.9](https://boto3.amazonaws.com/v1/documentation/api/1.28.9/index.html)
 type annotations builder for
 [boto3-stubs](https://pypi.org/project/boto3-stubs/).
 
 Generated by
 [mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
```

### Comparing `mypy-boto3-1.28.8/mypy_boto3/boto3_init_stub.py` & `mypy-boto3-1.28.9/mypy_boto3/boto3_init_stub.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-1.28.8/mypy_boto3/boto3_session_stub.py` & `mypy-boto3-1.28.9/mypy_boto3/boto3_session_stub.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-1.28.8/mypy_boto3/main.py` & `mypy-boto3-1.28.9/mypy_boto3/main.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-1.28.8/mypy_boto3/submodules.py` & `mypy-boto3-1.28.9/mypy_boto3/submodules.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-1.28.8/mypy_boto3.egg-info/PKG-INFO` & `mypy-boto3-1.28.9/mypy_boto3.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3
-Version: 1.28.8
-Summary: Type annotations for boto3 1.28.8 master module generated with mypy-boto3-builder 7.15.1
+Version: 1.28.9
+Summary: Type annotations for boto3 1.28.9 master module generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3.svg?color=blue)](https://pypi.org/project/mypy-boto3)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3?color=blue)](https://pypistats.org/packages/mypy-boto3)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Dynamic
-[boto3 1.28.8](https://boto3.amazonaws.com/v1/documentation/api/1.28.8/index.html)
+[boto3 1.28.9](https://boto3.amazonaws.com/v1/documentation/api/1.28.9/index.html)
 type annotations builder for
 [boto3-stubs](https://pypi.org/project/boto3-stubs/).
 
 Generated by
 [mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
```

### Comparing `mypy-boto3-1.28.8/setup.py` & `mypy-boto3-1.28.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3",
-    version="1.28.8",
+    version="1.28.9",
     packages=[
         "mypy_boto3",
     ],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3 1.28.8 master module generated with mypy-boto3-builder 7.15.1"
+        "Type annotations for boto3 1.28.9 master module generated with mypy-boto3-builder 7.15.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

