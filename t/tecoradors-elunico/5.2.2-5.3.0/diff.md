# Comparing `tmp/tecoradors-elunico-5.2.2.tar.gz` & `tmp/tecoradors-elunico-5.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tecoradors-elunico-5.2.2.tar", last modified: Tue Jul  4 18:08:18 2023, max compression
+gzip compressed data, was "tecoradors-elunico-5.3.0.tar", last modified: Fri Jul 21 03:56:24 2023, max compression
```

## Comparing `tecoradors-elunico-5.2.2.tar` & `tecoradors-elunico-5.3.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 thomaspovinelli   (501) staff       (20)        0 2023-07-04 18:08:18.447835 tecoradors-elunico-5.2.2/
--rw-r--r--   0 thomaspovinelli   (501) staff       (20)     1073 2023-02-25 18:38:36.000000 tecoradors-elunico-5.2.2/LICENSE
--rw-r--r--   0 thomaspovinelli   (501) staff       (20)      100 2023-02-25 18:38:36.000000 tecoradors-elunico-5.2.2/MANIFEST.in
--rw-r--r--   0 thomaspovinelli   (501) staff       (20)     1180 2023-07-04 18:08:18.447560 tecoradors-elunico-5.2.2/PKG-INFO
--rw-r--r--   0 thomaspovinelli   (501) staff       (20)      716 2023-07-04 17:51:52.000000 tecoradors-elunico-5.2.2/README.md
--rw-r--r--   0 thomaspovinelli   (501) staff       (20)      103 2023-02-25 18:38:36.000000 tecoradors-elunico-5.2.2/pyproject.toml
--rw-r--r--   0 thomaspovinelli   (501) staff       (20)       38 2023-07-04 18:08:18.447932 tecoradors-elunico-5.2.2/setup.cfg
--rw-r--r--   0 thomaspovinelli   (501) staff       (20)      729 2023-07-04 18:08:13.000000 tecoradors-elunico-5.2.2/setup.py
-drwxr-xr-x   0 thomaspovinelli   (501) staff       (20)        0 2023-07-04 18:08:18.444369 tecoradors-elunico-5.2.2/tecoradors/
--rw-r--r--   0 thomaspovinelli   (501) staff       (20)      787 2023-07-04 18:08:13.000000 tecoradors-elunico-5.2.2/tecoradors/__init__.py
--rw-r--r--   0 thomaspovinelli   (501) staff       (20)    40619 2023-07-04 17:53:31.000000 tecoradors-elunico-5.2.2/tecoradors/tecoradors.py
-drwxr-xr-x   0 thomaspovinelli   (501) staff       (20)        0 2023-07-04 18:08:18.446584 tecoradors-elunico-5.2.2/tecoradors_elunico.egg-info/
--rw-r--r--   0 thomaspovinelli   (501) staff       (20)     1180 2023-07-04 18:08:18.000000 tecoradors-elunico-5.2.2/tecoradors_elunico.egg-info/PKG-INFO
--rw-r--r--   0 thomaspovinelli   (501) staff       (20)      282 2023-07-04 18:08:18.000000 tecoradors-elunico-5.2.2/tecoradors_elunico.egg-info/SOURCES.txt
--rw-r--r--   0 thomaspovinelli   (501) staff       (20)        1 2023-07-04 18:08:18.000000 tecoradors-elunico-5.2.2/tecoradors_elunico.egg-info/dependency_links.txt
--rw-r--r--   0 thomaspovinelli   (501) staff       (20)       11 2023-07-04 18:08:18.000000 tecoradors-elunico-5.2.2/tecoradors_elunico.egg-info/top_level.txt
-drwxr-xr-x   0 thomaspovinelli   (501) staff       (20)        0 2023-07-04 18:08:18.446890 tecoradors-elunico-5.2.2/test/
--rw-r--r--   0 thomaspovinelli   (501) staff       (20)      341 2023-04-06 17:24:39.000000 tecoradors-elunico-5.2.2/test/test.py
+drwxr-xr-x   0 thomaspovinelli   (501) staff       (20)        0 2023-07-21 03:56:24.929553 tecoradors-elunico-5.3.0/
+-rw-r--r--   0 thomaspovinelli   (501) staff       (20)     1073 2023-02-25 18:38:36.000000 tecoradors-elunico-5.3.0/LICENSE
+-rw-r--r--   0 thomaspovinelli   (501) staff       (20)      100 2023-02-25 18:38:36.000000 tecoradors-elunico-5.3.0/MANIFEST.in
+-rw-r--r--   0 thomaspovinelli   (501) staff       (20)     1180 2023-07-21 03:56:24.929217 tecoradors-elunico-5.3.0/PKG-INFO
+-rw-r--r--   0 thomaspovinelli   (501) staff       (20)      716 2023-07-04 17:51:52.000000 tecoradors-elunico-5.3.0/README.md
+-rw-r--r--   0 thomaspovinelli   (501) staff       (20)      103 2023-02-25 18:38:36.000000 tecoradors-elunico-5.3.0/pyproject.toml
+-rw-r--r--   0 thomaspovinelli   (501) staff       (20)       38 2023-07-21 03:56:24.929673 tecoradors-elunico-5.3.0/setup.cfg
+-rw-r--r--   0 thomaspovinelli   (501) staff       (20)      729 2023-07-21 03:56:03.000000 tecoradors-elunico-5.3.0/setup.py
+drwxr-xr-x   0 thomaspovinelli   (501) staff       (20)        0 2023-07-21 03:56:24.925780 tecoradors-elunico-5.3.0/tecoradors/
+-rw-r--r--   0 thomaspovinelli   (501) staff       (20)      815 2023-07-21 03:54:39.000000 tecoradors-elunico-5.3.0/tecoradors/__init__.py
+-rw-r--r--   0 thomaspovinelli   (501) staff       (20)    41287 2023-07-21 03:55:32.000000 tecoradors-elunico-5.3.0/tecoradors/tecoradors.py
+drwxr-xr-x   0 thomaspovinelli   (501) staff       (20)        0 2023-07-21 03:56:24.927868 tecoradors-elunico-5.3.0/tecoradors_elunico.egg-info/
+-rw-r--r--   0 thomaspovinelli   (501) staff       (20)     1180 2023-07-21 03:56:24.000000 tecoradors-elunico-5.3.0/tecoradors_elunico.egg-info/PKG-INFO
+-rw-r--r--   0 thomaspovinelli   (501) staff       (20)      282 2023-07-21 03:56:24.000000 tecoradors-elunico-5.3.0/tecoradors_elunico.egg-info/SOURCES.txt
+-rw-r--r--   0 thomaspovinelli   (501) staff       (20)        1 2023-07-21 03:56:24.000000 tecoradors-elunico-5.3.0/tecoradors_elunico.egg-info/dependency_links.txt
+-rw-r--r--   0 thomaspovinelli   (501) staff       (20)       11 2023-07-21 03:56:24.000000 tecoradors-elunico-5.3.0/tecoradors_elunico.egg-info/top_level.txt
+drwxr-xr-x   0 thomaspovinelli   (501) staff       (20)        0 2023-07-21 03:56:24.928300 tecoradors-elunico-5.3.0/test/
+-rw-r--r--   0 thomaspovinelli   (501) staff       (20)      341 2023-04-06 17:24:39.000000 tecoradors-elunico-5.3.0/test/test.py
```

### Comparing `tecoradors-elunico-5.2.2/LICENSE` & `tecoradors-elunico-5.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tecoradors-elunico-5.2.2/PKG-INFO` & `tecoradors-elunico-5.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tecoradors-elunico
-Version: 5.2.2
+Version: 5.3.0
 Summary: A small collection of decorators I like to use often
 Home-page: https://github.com/elunico/tecoradors
 Author: Thomas Povinelli
 Author-email: tompov227@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `tecoradors-elunico-5.2.2/README.md` & `tecoradors-elunico-5.3.0/README.md`

 * *Files identical despite different names*

### Comparing `tecoradors-elunico-5.2.2/setup.py` & `tecoradors-elunico-5.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="tecoradors-elunico",
-    version="5.2.2",
+    version="5.3.0",
     author="Thomas Povinelli",
     author_email="tompov227@gmail.com",
     description="A small collection of decorators I like to use often",
     long_description=long_description,
     long_description_content_type="text/markdown",
     include_package_data=True,
     url="https://github.com/elunico/tecoradors",
```

### Comparing `tecoradors-elunico-5.2.2/tecoradors/__init__.py` & `tecoradors-elunico-5.3.0/tecoradors/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from tecoradors.tecoradors import (
     accepts, dataclass, deprecated, equatable, final, freeze, FrozenClassError, hashable, json_serializable, log, Self,
     spread, squash, stringable, synchronized, timed, count_calls, returns, interruptable, lazy, precompute, PrecomputeStorage, NoSuchValue,
-    builder, tattle, TattleOptions
+    builder, tattle, TattleOptions, orderable
 )
 
 __all__ = [
     "accepts",
     "json_serializable",
     "spread",
     'builder',
     'tattle',
     'TattleOptions',
     "timed",
     "squash",
     "stringable",
     "equatable",
     "hashable",
+    "orderable",
     "dataclass",
     "Self",
     "final",
     "deprecated",
     "freeze",
     "FrozenClassError",
     "log",
```

### Comparing `tecoradors-elunico-5.2.2/tecoradors/tecoradors.py` & `tecoradors-elunico-5.3.0/tecoradors/tecoradors.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,33 @@
 import enum
 import functools
 import inspect
 import sys
 import typing
 
 
+def chained(obj, *fields):
+    for field in fields:
+        obj = getattr(obj, field)
+    return obj
+
+
+def apply(fns, *arguments, **kwarguments):
+    return tuple(fn(*arguments, **kwarguments) for fn in fns)
+
 # taken from https://stackoverflow.com/questions/3589311/get-defining-class-of-unbound-method-object-in-python-3
+
+
 def _get_class_that_defined_method(meth):
     if isinstance(meth, functools.partial):
         return _get_class_that_defined_method(meth.func)
     if inspect.ismethod(meth) or (
             inspect.isbuiltin(meth) and getattr(meth, '__self__', None) is not None and getattr(meth.__self__,
                                                                                                 '__class__', None)):
-        for cls in inspect.getmro(meth.__self__.__class__):
+        for cls in meth.__self__.__class__.__mro__:
             if meth.__name__ in cls.__dict__:
                 return cls
         meth = getattr(meth, '__func__', meth)  # fallback to __qualname__ parsing
     if inspect.isfunction(meth):
         cls = getattr(inspect.getmodule(meth), meth.__qualname__.split('.<locals>', 1)[0].rsplit('.', 1)[0], None)
         if isinstance(cls, type):
             return cls
@@ -459,15 +470,14 @@
                 if options.onexit is not None:
                     options.onexit(result, *args, **kwargs)
                 return result
         return wrapper
     return interior
 
 
-
 def timed(fn):
     """
     Wraps a function using time.time() in order to time the execution of the function
 
     Returns the a tuple of original function result and the time elapsed in
     seconds
     """
@@ -706,15 +716,29 @@
                 raise TypeError(str_format)
         return super_hasher(cls, self) ^ functools.reduce(hasher, self.__dict__.values(), 0)
 
     setattr(cls, '__hash__', __hash__)
     return cls
 
 
+def orderable(cls):
+    """
+    Modifies a class to be orderable. Provides a __eq__ and __hash__ method using @hashable.
+    Requires an implementation of one of the 6 magic comparison methods.
+    Uses @functools.total_ordering to accomplish the ordering.
+
+    See the descriptions of @hashable and @functools.total_ordering for the
+    caveats around using this decorator
+    """
+    cls = hashable(cls)
+    return functools.total_ordering(cls)
+
 # decorator function
+
+
 def dataclass(cls, **kwargs):
     """
     Wraps the built-in dataclass.dataclass annotation in order to also give the
     class a __str__ method. All options provided in kwargs are forwarded to the
     dataclasses.dataclass decorator. After that the stringable decorator is used
     to give the class a __str__ method
 
@@ -971,15 +995,15 @@
 
 T = typing.TypeVar('T')
 R = typing.TypeVar('R')
 
 
 class Descriptor(typing.Protocol):
     def __get__(this, self: typing.Optional[R], owner: typing.Optional[typing.Any] = None, *args, **kwargs) -> \
-    typing.Union[T, typing.Self]:
+            typing.Union[T, typing.Self]:
         ...
 
 
 def lazy(method: typing.Callable[[typing.Any], T]) -> Descriptor:
     '''
     Similar to the `@property` decorator, lazy allows you to access the value computed by a method
     call as if it were a simple attribute on an instance. The main difference between `@property`
@@ -992,15 +1016,15 @@
     in a function, and only evaluating the function when accessed. It also elimited the overhead of
     other similar solutions like `@functools.cache` by re-writing the attribute after first access,
     removing the descriptor and obviating the need for an `if arg in cache` check
     '''
 
     class descriptor(Descriptor):
         def __get__(self, receiver: typing.Optional[R], owner: typing.Optional[typing.Any] = None, *args, **kwargs) -> \
-        typing.Union[T, typing.Self]:
+                typing.Union[T, typing.Self]:
             if receiver is None:
                 return self
             value = method(receiver, *args, **kwargs)
             setattr(receiver, method.__name__, value)
             return value
 
     return descriptor()
```

### Comparing `tecoradors-elunico-5.2.2/tecoradors_elunico.egg-info/PKG-INFO` & `tecoradors-elunico-5.3.0/tecoradors_elunico.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tecoradors-elunico
-Version: 5.2.2
+Version: 5.3.0
 Summary: A small collection of decorators I like to use often
 Home-page: https://github.com/elunico/tecoradors
 Author: Thomas Povinelli
 Author-email: tompov227@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

