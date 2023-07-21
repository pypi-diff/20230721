# Comparing `tmp/pure_interface-7.1.0.tar.gz` & `tmp/pure_interface-7.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\Source\pure_interface\dist\.tmp-_a_hks6u\pure_interface-7.1.0.tar", last modified: Mon May  1 21:58:03 2023, max compression
+gzip compressed data, was "pure_interface-7.3.0.tar", last modified: Fri Jul 21 02:34:49 2023, max compression
```

## Comparing `pure_interface-7.1.0.tar` & `pure_interface-7.3.0.tar`

### file list

```diff
@@ -1,36 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 21:58:03.589988 pure_interface-7.1.0/
--rw-rw-rw-   0        0        0     1070 2021-09-21 22:43:47.000000 pure_interface-7.1.0/LICENSE
--rw-rw-rw-   0        0        0    34895 2023-05-01 21:58:03.589988 pure_interface-7.1.0/PKG-INFO
--rw-rw-rw-   0        0        0    33927 2023-05-01 21:55:51.000000 pure_interface-7.1.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-01 21:58:03.559726 pure_interface-7.1.0/pure_interface/
--rw-rw-rw-   0        0        0      617 2023-05-01 21:55:58.000000 pure_interface-7.1.0/pure_interface/__init__.py
--rw-rw-rw-   0        0        0     7884 2023-03-01 20:08:43.000000 pure_interface-7.1.0/pure_interface/adaption.py
--rw-rw-rw-   0        0        0     2167 2023-03-01 20:08:43.000000 pure_interface-7.1.0/pure_interface/data_classes.py
--rw-rw-rw-   0        0        0     8522 2023-05-01 21:45:26.000000 pure_interface-7.1.0/pure_interface/delegation.py
--rw-rw-rw-   0        0        0      372 2023-03-01 20:08:43.000000 pure_interface-7.1.0/pure_interface/errors.py
--rw-rw-rw-   0        0        0    33634 2023-05-01 21:16:47.000000 pure_interface-7.1.0/pure_interface/interface.py
-drwxrwxrwx   0        0        0        0 2023-05-01 21:58:03.564727 pure_interface-7.1.0/pure_interface.egg-info/
--rw-rw-rw-   0        0        0    34895 2023-05-01 21:58:03.000000 pure_interface-7.1.0/pure_interface.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      821 2023-05-01 21:58:03.000000 pure_interface-7.1.0/pure_interface.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 21:58:03.000000 pure_interface-7.1.0/pure_interface.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-05-01 21:58:03.000000 pure_interface-7.1.0/pure_interface.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       90 2021-09-21 22:43:47.000000 pure_interface-7.1.0/pyproject.toml
--rw-rw-rw-   0        0        0     1088 2023-05-01 21:58:03.591989 pure_interface-7.1.0/setup.cfg
--rw-rw-rw-   0        0        0       43 2021-09-21 22:43:47.000000 pure_interface-7.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-01 21:58:03.588989 pure_interface-7.1.0/tests/
--rw-rw-rw-   0        0        0     3843 2023-04-27 05:33:41.000000 pure_interface-7.1.0/tests/test_adapt_args_anno.py
--rw-rw-rw-   0        0        0     2871 2023-04-27 05:33:41.000000 pure_interface-7.1.0/tests/test_adapt_args_no_anno.py
--rw-rw-rw-   0        0        0    12205 2023-04-27 05:33:41.000000 pure_interface-7.1.0/tests/test_adaption.py
--rw-rw-rw-   0        0        0     1022 2023-04-27 05:33:41.000000 pure_interface-7.1.0/tests/test_dataclass_support.py
--rw-rw-rw-   0        0        0     9280 2023-05-01 21:50:19.000000 pure_interface-7.1.0/tests/test_delegate.py
--rw-rw-rw-   0        0        0     5935 2023-04-27 05:33:41.000000 pure_interface-7.1.0/tests/test_func_sigs3.py
--rw-rw-rw-   0        0        0    11757 2023-04-27 05:33:41.000000 pure_interface-7.1.0/tests/test_function_sigs.py
--rw-rw-rw-   0        0        0     1051 2023-05-01 21:06:52.000000 pure_interface-7.1.0/tests/test_generic_support.py
--rw-rw-rw-   0        0        0    16459 2023-05-01 21:18:53.000000 pure_interface-7.1.0/tests/test_implementation_checks.py
--rw-rw-rw-   0        0        0     2803 2023-04-27 05:33:41.000000 pure_interface-7.1.0/tests/test_inheritance.py
--rw-rw-rw-   0        0        0     4040 2023-04-27 05:33:41.000000 pure_interface-7.1.0/tests/test_isinstance.py
--rw-rw-rw-   0        0        0     2346 2023-03-01 20:08:43.000000 pure_interface-7.1.0/tests/test_meta_classes.py
--rw-rw-rw-   0        0        0     2877 2023-04-27 05:33:41.000000 pure_interface-7.1.0/tests/test_module_funcs.py
--rw-rw-rw-   0        0        0     3364 2023-03-01 20:08:43.000000 pure_interface-7.1.0/tests/test_no_content_checks.py
--rw-rw-rw-   0        0        0     2071 2023-04-27 05:33:41.000000 pure_interface-7.1.0/tests/test_tracker.py
--rw-rw-rw-   0        0        0      514 2023-04-27 05:33:41.000000 pure_interface-7.1.0/tests/test_versions_in_sync.py
+drwxrwxrwx   0        0        0        0 2023-07-21 02:34:49.891073 pure_interface-7.3.0/
+-rw-rw-rw-   0        0        0     1070 2021-09-21 22:43:47.000000 pure_interface-7.3.0/LICENSE
+-rw-rw-rw-   0        0        0    35832 2023-07-21 02:34:49.892074 pure_interface-7.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0    34863 2023-07-21 02:33:09.000000 pure_interface-7.3.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-07-21 02:34:49.816177 pure_interface-7.3.0/pure_interface/
+-rw-rw-rw-   0        0        0      596 2023-07-21 02:33:09.000000 pure_interface-7.3.0/pure_interface/__init__.py
+-rw-rw-rw-   0        0        0     2862 2023-07-21 02:33:09.000000 pure_interface-7.3.0/pure_interface/_sub_interface.py
+-rw-rw-rw-   0        0        0     7929 2023-07-21 02:33:09.000000 pure_interface-7.3.0/pure_interface/adaption.py
+-rw-rw-rw-   0        0        0     2195 2023-05-11 00:43:53.000000 pure_interface-7.3.0/pure_interface/data_classes.py
+-rw-rw-rw-   0        0        0     8709 2023-07-21 02:33:09.000000 pure_interface-7.3.0/pure_interface/delegation.py
+-rw-rw-rw-   0        0        0      374 2023-07-21 02:33:09.000000 pure_interface-7.3.0/pure_interface/errors.py
+-rw-rw-rw-   0        0        0    33969 2023-07-21 02:33:09.000000 pure_interface-7.3.0/pure_interface/interface.py
+-rw-rw-rw-   0        0        0        0 2023-05-11 00:43:53.000000 pure_interface-7.3.0/pure_interface/py.typed
+drwxrwxrwx   0        0        0        0 2023-07-21 02:34:49.832187 pure_interface-7.3.0/pure_interface.egg-info/
+-rw-rw-rw-   0        0        0    35832 2023-07-21 02:34:49.000000 pure_interface-7.3.0/pure_interface.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      907 2023-07-21 02:34:49.000000 pure_interface-7.3.0/pure_interface.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 02:34:49.000000 pure_interface-7.3.0/pure_interface.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-07-21 02:34:49.000000 pure_interface-7.3.0/pure_interface.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       90 2021-09-21 22:43:47.000000 pure_interface-7.3.0/pyproject.toml
+-rw-rw-rw-   0        0        0     1142 2023-07-21 02:34:49.900072 pure_interface-7.3.0/setup.cfg
+-rw-rw-rw-   0        0        0       43 2021-09-21 22:43:47.000000 pure_interface-7.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 02:34:49.889074 pure_interface-7.3.0/tests/
+-rw-rw-rw-   0        0        0     4287 2023-07-21 02:33:09.000000 pure_interface-7.3.0/tests/test_adapt_args_anno.py
+-rw-rw-rw-   0        0        0     2871 2023-04-27 05:33:41.000000 pure_interface-7.3.0/tests/test_adapt_args_no_anno.py
+-rw-rw-rw-   0        0        0    12843 2023-07-21 02:33:09.000000 pure_interface-7.3.0/tests/test_adaption.py
+-rw-rw-rw-   0        0        0     1552 2023-07-21 02:33:09.000000 pure_interface-7.3.0/tests/test_dataclass_support.py
+-rw-rw-rw-   0        0        0     9796 2023-07-21 02:33:09.000000 pure_interface-7.3.0/tests/test_delegate.py
+-rw-rw-rw-   0        0        0     5930 2023-07-21 02:33:09.000000 pure_interface-7.3.0/tests/test_func_sigs3.py
+-rw-rw-rw-   0        0        0    11759 2023-07-21 02:33:09.000000 pure_interface-7.3.0/tests/test_function_sigs.py
+-rw-rw-rw-   0        0        0     1051 2023-05-01 21:06:52.000000 pure_interface-7.3.0/tests/test_generic_support.py
+-rw-rw-rw-   0        0        0    16578 2023-07-21 02:33:09.000000 pure_interface-7.3.0/tests/test_implementation_checks.py
+-rw-rw-rw-   0        0        0     2781 2023-07-21 02:33:09.000000 pure_interface-7.3.0/tests/test_inheritance.py
+-rw-rw-rw-   0        0        0     4034 2023-07-21 02:33:09.000000 pure_interface-7.3.0/tests/test_isinstance.py
+-rw-rw-rw-   0        0        0     2346 2023-03-01 20:08:43.000000 pure_interface-7.3.0/tests/test_meta_classes.py
+-rw-rw-rw-   0        0        0     2877 2023-04-27 05:33:41.000000 pure_interface-7.3.0/tests/test_module_funcs.py
+-rw-rw-rw-   0        0        0     3364 2023-03-01 20:08:43.000000 pure_interface-7.3.0/tests/test_no_content_checks.py
+-rw-rw-rw-   0        0        0     3376 2023-07-21 02:33:09.000000 pure_interface-7.3.0/tests/test_sub_interfaces.py
+-rw-rw-rw-   0        0        0     2714 2023-07-21 02:33:09.000000 pure_interface-7.3.0/tests/test_tracker.py
+-rw-rw-rw-   0        0        0      514 2023-04-27 05:33:41.000000 pure_interface-7.3.0/tests/test_versions_in_sync.py
```

### Comparing `pure_interface-7.1.0/LICENSE` & `pure_interface-7.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pure_interface-7.1.0/PKG-INFO` & `pure_interface-7.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: pure_interface
-Version: 7.1.0
+Version: 7.3.0
 Summary: A Python interface library that disallows function body content on interfaces and supports adaption.
 Home-page: https://github.com/seequent/pure_interface
 Download-URL: https://pypi.org/project/pure-interface/
 Author: Tim Mitchell
 Author-email: tim.mitchell@seequent.com
 License: MIT
 Keywords: abc interface adapt adaption mapper structural typing dataclass
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 pure_interface
 ==============
 
 A Python interface library that disallows function body content on interfaces and supports adaption.
@@ -33,15 +33,15 @@
 * Ensures that method overrides have compatible signatures
 * Supports interface adaption.
 * Supports optional structural type checking for ``Interface.provided_by(a)`` and ``Interface.adapt(a)``
 * Allows concrete implementations the flexibility to implement abstract properties as instance attributes.
 * ``Interface.adapt()`` can return an implementation wrapper that provides *only* the
   attributes and methods defined by ``Interface``.
 * Warns if ``provided_by`` did a structural type check when inheritance would work.
-* Supports python 3.7+
+* Supports python 3.8+
 
 A note on the name
 ------------------
 The phrase *pure interface* applies only to the first design goal - a class that defines only an interface with no
 implementation is a pure interface [*]_.
 In every other respect the zen of 'practicality beats purity' applies.
 
@@ -230,14 +230,30 @@
     if pure_iterface.missing_method_warnings:
         for warning in pure_iterface.get_missing_method_warnings():
             print(warning)
         exit(1)
 
 Note that missing properties are NOT checked for as they may be provided by instance attributes.
 
+Sub-Interfaces
+==============
+Sometimes your code only uses a small part of a large interface.  It can be useful (eg. for test mocking) to specify
+the sub part of the interface that your code requires.  This can be done with the ``sub_interface_of`` decorator.::
+
+    @sub_interface_of(IAnimal)
+    class IHeight(pure_interface.Interface):
+        height: float
+
+    def my_code(h: IHeight):
+        return "That's tall" if h.height > 100 else "Not so tall"
+
+The ``sub_interface_of`` decorator checks that the attributes and methods of the smaller interface match the larger interface.
+Function signatures must match exactly (not just be compatible).  The decorator will also use ``abc.register`` so that
+``isinstance(Animal(), IHeight)`` returns ``True``.
+
 Adaption
 ========
 
 Registering Adapters
 --------------------
 
 Adapters for an interface are registered with the ``adapts`` decorator or with
@@ -342,14 +358,18 @@
     class IntToB(IB, object):
         def __init__(self, x):
             self.foo = self.bar = x
 
 Then  ``IA.adapt(4)`` will use the ``IntToB`` adapter to adapt ``4`` to ``IA`` (unless there is already an adapter
 from ``int`` to ``IA``)
 
+Further, if an interface is decorated with ``sub_interface_of``, adapters for the larger interface will be used if
+a direct adapter is not found.
+
+
 Structural Type Checking
 ========================
 
 Structural_ type checking checks if an object has the attributes and methods defined by the interface.
 
 As interfaces are inherited, you can usually use ``isinstance(obj, MyInterface)`` to check if an interface is provided.
 An alternative to ``isinstance()`` is the ``Interface.provided_by(obj)`` classmethod which will fall back to structural type
@@ -572,16 +592,16 @@
             self.foo = 3
 
 If you supply more than one delegation rule (e.g. both ``pi_attr_mapping`` and ``pi_attr_fallack``) then
  ``pi_attr_delegates`` delegates are created first and any attributes defined there are now part of the class.
 Then ``pi_attr_mapping`` delegates are created (and become part of the class) and finally ``pi_attr_fallback`` is processed.
 Thus if there are duplicate delegates defined, the one defined first takes precedence.
 
-Composition
------------
+Type Composition
+----------------
 A special case where all delegated attributes are defined in an ``Interface`` is handled by the ``composed_type`` factory function.
 ``composed_type`` takes 2 or more interfaces and returns a new type that inherits from all the interfaces with a
 constructor that takes instances that implement those interfaces (in the same order).  For exmaple::
 
     AT = composed_type(IAnimal, ITalker)
 
     a = Animal(5)
```

### Comparing `pure_interface-7.1.0/README.rst` & `pure_interface-7.3.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 * Ensures that method overrides have compatible signatures
 * Supports interface adaption.
 * Supports optional structural type checking for ``Interface.provided_by(a)`` and ``Interface.adapt(a)``
 * Allows concrete implementations the flexibility to implement abstract properties as instance attributes.
 * ``Interface.adapt()`` can return an implementation wrapper that provides *only* the
   attributes and methods defined by ``Interface``.
 * Warns if ``provided_by`` did a structural type check when inheritance would work.
-* Supports python 3.7+
+* Supports python 3.8+
 
 A note on the name
 ------------------
 The phrase *pure interface* applies only to the first design goal - a class that defines only an interface with no
 implementation is a pure interface [*]_.
 In every other respect the zen of 'practicality beats purity' applies.
 
@@ -208,14 +208,30 @@
     if pure_iterface.missing_method_warnings:
         for warning in pure_iterface.get_missing_method_warnings():
             print(warning)
         exit(1)
 
 Note that missing properties are NOT checked for as they may be provided by instance attributes.
 
+Sub-Interfaces
+==============
+Sometimes your code only uses a small part of a large interface.  It can be useful (eg. for test mocking) to specify
+the sub part of the interface that your code requires.  This can be done with the ``sub_interface_of`` decorator.::
+
+    @sub_interface_of(IAnimal)
+    class IHeight(pure_interface.Interface):
+        height: float
+
+    def my_code(h: IHeight):
+        return "That's tall" if h.height > 100 else "Not so tall"
+
+The ``sub_interface_of`` decorator checks that the attributes and methods of the smaller interface match the larger interface.
+Function signatures must match exactly (not just be compatible).  The decorator will also use ``abc.register`` so that
+``isinstance(Animal(), IHeight)`` returns ``True``.
+
 Adaption
 ========
 
 Registering Adapters
 --------------------
 
 Adapters for an interface are registered with the ``adapts`` decorator or with
@@ -320,14 +336,18 @@
     class IntToB(IB, object):
         def __init__(self, x):
             self.foo = self.bar = x
 
 Then  ``IA.adapt(4)`` will use the ``IntToB`` adapter to adapt ``4`` to ``IA`` (unless there is already an adapter
 from ``int`` to ``IA``)
 
+Further, if an interface is decorated with ``sub_interface_of``, adapters for the larger interface will be used if
+a direct adapter is not found.
+
+
 Structural Type Checking
 ========================
 
 Structural_ type checking checks if an object has the attributes and methods defined by the interface.
 
 As interfaces are inherited, you can usually use ``isinstance(obj, MyInterface)`` to check if an interface is provided.
 An alternative to ``isinstance()`` is the ``Interface.provided_by(obj)`` classmethod which will fall back to structural type
@@ -550,16 +570,16 @@
             self.foo = 3
 
 If you supply more than one delegation rule (e.g. both ``pi_attr_mapping`` and ``pi_attr_fallack``) then
  ``pi_attr_delegates`` delegates are created first and any attributes defined there are now part of the class.
 Then ``pi_attr_mapping`` delegates are created (and become part of the class) and finally ``pi_attr_fallback`` is processed.
 Thus if there are duplicate delegates defined, the one defined first takes precedence.
 
-Composition
------------
+Type Composition
+----------------
 A special case where all delegated attributes are defined in an ``Interface`` is handled by the ``composed_type`` factory function.
 ``composed_type`` takes 2 or more interfaces and returns a new type that inherits from all the interfaces with a
 constructor that takes instances that implement those interfaces (in the same order).  For exmaple::
 
     AT = composed_type(IAnimal, ITalker)
 
     a = Animal(5)
```

### Comparing `pure_interface-7.1.0/pure_interface/adaption.py` & `pure_interface-7.3.0/pure_interface/adaption.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 from __future__ import division, absolute_import, print_function
 
 import functools
 import inspect
 import types
-from typing import Any, Type, Callable
+from typing import Any, Type, Callable, Optional
 import typing
 import warnings
 
 from .errors import InterfaceError, AdaptionError
-from .interface import PI, Interface, InterfaceType
+from .interface import AnInterface, Interface, InterfaceType, AnInterfaceType, type_is_interface
 from .interface import get_type_interfaces, get_pi_attribute
 
 
-def adapts(from_type, to_interface=None):
-    # type: (Any, Type[PI]) -> Callable[[Any], Any]
+def adapts(from_type: Any, to_interface: Optional[Type[AnInterface]] = None) -> Callable[[Any], Any]:
     """Class or function decorator for declaring an adapter from a type to an interface.
     E.g.
         @adapts(MyClass, MyInterface)
         def interface_factory(obj):
             ....
 
     If decorating a class to_interface may be None to use the first interface in the class's MRO.
@@ -43,16 +42,18 @@
             interface = to_interface
         register_adapter(cls, from_type, interface)
         return cls
 
     return decorator
 
 
-def register_adapter(adapter, from_type, to_interface):
-    # type: (Callable, Any, Type[Interface]) -> None
+def register_adapter(
+        adapter: Callable[[Type], AnInterfaceType],
+        from_type: Type,
+        to_interface: AnInterfaceType) -> None:
     """ Registers adapter to convert instances of from_type to objects that provide to_interface
     for the to_interface.adapt() method.
 
     :param adapter: callable that takes an instance of from_type and returns an object providing to_interface.
     :param from_type: a type to adapt from
     :param to_interface: a (non-concrete) Interface subclass to adapt to.
     """
@@ -75,61 +76,58 @@
     want the overhead of lots of copies.  This class provides adapt() and adapt_or_none() methods that track adaptions.
     Thus if `x is b` is `True` then `adapter.adapt(x, I) is adapter.adapt(b, I)` is `True`.
     """
     def __init__(self, mapping_factory=dict):
         self._factory = mapping_factory
         self._adapters = mapping_factory()
 
-    def adapt(self, obj, interface):
+    def adapt(self, obj: Any, interface: Type[AnInterface]) -> AnInterface:
         """ Adapts `obj` to `interface`"""
         try:
             return self._adapters[interface][obj]
         except KeyError:
             return self._adapt(obj, interface)
 
-    def adapt_or_none(self, obj, interface):
+    def adapt_or_none(self, obj: Any, interface: Type[AnInterface]) -> Optional[AnInterface]:
         """ Adapt obj to interface returning None on failure."""
         try:
             return self.adapt(obj, interface)
         except ValueError:
             return None
 
-    def clear(self):
+    def clear(self) -> None:
         """ Clears the cached adapters."""
         self._adapters = self._factory()
 
-    def _adapt(self, obj, interface):
+    def _adapt(self, obj: Any, interface: Type[AnInterface]) -> AnInterface:
         adapted = interface.adapt(obj)
         try:
             adapters = self._adapters[interface]
         except KeyError:
             adapters = self._adapters[interface] = self._factory()
         adapters[obj] = adapted
         return adapted
 
 
-def _interface_from_anno(annotation):
+def _interface_from_anno(annotation: Any) -> Optional[AnInterfaceType]:
     """ Typically the annotation is the interface,  but if a default value of None is given the annotation is
     a typing.Union[interface, None] a.k.a. Optional[interface]. Lets be nice and support those too.
     """
     try:
         if issubclass(annotation, Interface):
             return annotation
     except TypeError:
         pass
     if hasattr(annotation, '__origin__') and hasattr(annotation, '__args__'):
         # could be a typing.Union
         if annotation.__origin__ is not typing.Union:
             return None
         for arg_type in annotation.__args__:
-            try:
-                if issubclass(arg_type, Interface):
-                    return arg_type
-            except TypeError:
-                pass
+            if type_is_interface(arg_type):
+                return arg_type
 
     return None
 
 
 def adapt_args(*func_arg, **kwarg_types):
     """ adapts arguments to the decorated function to the types given.  For example:
 
@@ -175,27 +173,22 @@
             raise AdaptionError('Only one posititional argument permitted')
         if not isinstance(func_arg[0], types.FunctionType):
             raise AdaptionError('Positional argument must be a function (to decorate)')
         if kwarg_types:
             raise AdaptionError('keyword parameters not permitted with positional argument')
         funcn = func_arg[0]
         annotations = typing.get_type_hints(funcn)
-        if annotations is None:
-            annotations = {}
         if not annotations:
             warnings.warn('No annotations for {}. '
                           'Add annotations or pass explicit argument types to adapt_args'.format(funcn.__name__),
                           stacklevel=2)
         for key, anno in annotations.items():
             i_face = _interface_from_anno(anno)
             if i_face is not None:
                 kwarg_types[key] = i_face
         return decorator(funcn)
 
     for key, i_face in kwarg_types.items():
-        try:
-            can_adapt = issubclass(i_face, Interface)
-        except TypeError:
-            can_adapt = False
+        can_adapt = type_is_interface(i_face)
         if not can_adapt:
             raise AdaptionError('adapt_args parameter values must be subtypes of Interface')
     return decorator
```

### Comparing `pure_interface-7.1.0/pure_interface/data_classes.py` & `pure_interface-7.3.0/pure_interface/data_classes.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     _dataclass_args = ('init', 'repr', 'eq', 'order', 'unsafe_hash', 'frozen',
                        'match_args', 'kw_only', 'slots')
 else:
     _dataclass_args = ('init', 'repr', 'eq', 'order', 'unsafe_hash', 'frozen',
                        'match_args', 'kw_only', 'slots', 'weakref_slot')
 
 
-def dataclass(_cls=None, **kwargs):
+def dataclass(_cls: typing.Union[type, None] = None, **kwargs):
     """Returns the same class as was passed in, with dunder methods
     added based on the fields defined in the class.
     """
     arg_tuple = tuple(kwargs.get(arg_name, _dataclass_defaults[arg_name]) for arg_name in _dataclass_args)
 
     def wrap(cls):
         # dataclasses only operates on annotations in the current class
```

### Comparing `pure_interface-7.1.0/pure_interface/delegation.py` & `pure_interface-7.3.0/pure_interface/delegation.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from __future__ import division, absolute_import, print_function
 
 import operator
+from typing import Dict, Union, Sequence, Type, Set, Tuple, Any
 
-import pure_interface
 from .errors import InterfaceError
-from .interface import get_interface_names, type_is_interface, get_type_interfaces, InterfaceType
+from .interface import get_interface_names, type_is_interface, get_type_interfaces, AnInterfaceType, AnInterface
 
-_composed_types_map = {}
+_composed_types_map: Dict[Tuple[Type, ...], Type] = {}
 _letters = 'abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ'
 
 
 class _Delegated:
-    def __init__(self, dotted_name):
+    def __init__(self, dotted_name: str):
         self._getter = operator.attrgetter(dotted_name)
         self._impl_name, self._attr_name = dotted_name.rsplit('.', 1)
 
     def __get__(self, obj, cls):
         if obj is None:
             return self
         return self._getter(obj)
@@ -107,22 +107,22 @@
 
             def __init__(self, impl):
                 self.impl = impl
                 self.foo = 3
 
     """
     pi_attr_fallback = None
-    pi_attr_delegates = {}
-    pi_attr_mapping = {}
+    pi_attr_delegates: Dict[str, Union[str, type]] = {}
+    pi_attr_mapping: Dict[str, Sequence[str]] = {}
 
     def __init_subclass__(cls, **kwargs):
         # get non-interface base class ignoring abc.ABC and object.
         non_interface_bases = [base for base in cls.mro()[:-2] if not type_is_interface(base)]
 
-        def i_have_attribute(attrib):
+        def i_have_attribute(attrib: str) -> bool:
             for klass in non_interface_bases:
                 if attrib in klass.__dict__:
                     return True
             return False
 
         for delegate, attr_list in cls.__dict__.get('pi_attr_delegates', {}).items():
             if isinstance(attr_list, type):
@@ -145,15 +145,15 @@
                 interface_names = get_interface_names(interface)
                 for attr in interface_names:
                     if not i_have_attribute(attr):
                         dotted_name = f'{fallback}.{attr}'
                         setattr(cls, attr, _Delegated(dotted_name))
 
     @classmethod
-    def provided_by(cls, obj):
+    def provided_by(cls, obj: Any):
         if not hasattr(cls, 'pi_composed_interfaces'):
             raise InterfaceError('provided_by() can only be called on composed types')
         if isinstance(obj, cls):
             return True
         other_mro = [c for c in type(obj).mro() if type_is_interface(c)]
         my_mro = [c for c in cls.mro() if type_is_interface(c)]
         if set(my_mro) <= set(other_mro):
@@ -165,15 +165,15 @@
     for i, impl in enumerate(args):
         attr = '_' + _letters[i]
         if not isinstance(impl, type(self).pi_composed_interfaces[i]):
             raise ValueError(f'Expected {type(self).pi_composed_interfaces[i]} got {type(impl)} instead')
         setattr(self, attr, impl)
 
 
-def composed_type(*interface_types: InterfaceType) -> type:
+def composed_type(*interface_types: AnInterfaceType) -> Type[Delegate]:
     """Returns a new class which implements all the passed interfaces.
     If the interfaces have duplicate attribute or method names, the first enountered implementation is used.
     Instances of the returned type are passed implementations of the given interfaces in the same order.
     e.g.
     class IA(Interface):
         foo: int
     class IB(Interface):
@@ -196,15 +196,15 @@
     if len(interface_types) > len(_letters):
         raise ValueError(f'Too many interfaces.  Use {len(_letters)} or fewer.')
     interface_types = tuple(interface_types)
     c_type = _composed_types_map.get(interface_types)
     if c_type is not None:
         return c_type
     delegates = {}
-    all_names = set()
+    all_names: Set[str] = set()
     for i, interface in enumerate(interface_types):
         if not type_is_interface(interface):
             raise ValueError('all arguments to composed_type must be Interface classes')
         attr = '_' + _letters[i]
         int_names = get_interface_names(interface)
         delegates[attr] = [name for name in int_names if name not in all_names]
         all_names.update(int_names)
```

### Comparing `pure_interface-7.1.0/pure_interface/interface.py` & `pure_interface-7.3.0/pure_interface/interface.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,103 +6,111 @@
 import abc
 from abc import abstractmethod, abstractclassmethod, abstractstaticmethod
 import collections
 import dis
 import inspect
 from inspect import signature, Signature, Parameter
 import types
-from typing import Any, Callable, List, Optional, Iterable, FrozenSet, Type, TypeVar, Generic
+from typing import Any, Callable, List, Optional, Iterable, FrozenSet, Type, TypeVar, Generic, Dict, Set, Tuple, cast, \
+    Union
 import sys
 import warnings
 import weakref
 
 from .errors import InterfaceError, AdaptionError
 
 is_development = not hasattr(sys, 'frozen')
-missing_method_warnings = []
+missing_method_warnings: List[str] = []
 
+_T = TypeVar('_T')
 
-def set_is_development(is_dev):
+
+def set_is_development(is_dev: bool) -> None:
     global is_development
     is_development = is_dev
 
 
-def get_is_development():
+def get_is_development() -> bool:
     return is_development
 
 
-def get_missing_method_warnings():
+def get_missing_method_warnings() -> List[str]:
     return missing_method_warnings
 
 
-def no_adaption(obj):
+def no_adaption(obj: _T) -> _T:
     return obj
 
 
-PI = TypeVar('PI', bound='Interface')
+AnInterface = TypeVar('AnInterface', bound='Interface')
+AnInterfaceType = TypeVar('AnInterfaceType', bound=Type['Interface'])
 
 
 class _PIAttributes(object):
     """ rather than clutter the class namespace with lots of _pi_XXX attributes, collect them all here"""
 
-    def __init__(self, type_is_interface, abstract_properties, interface_method_signatures, interface_attribute_names):
-        self.type_is_interface = type_is_interface
+    def __init__(self, type_is_interface: bool,
+                 abstract_properties: Set[str],
+                 interface_method_signatures: Dict[str, Signature],
+                 interface_attribute_names: Set[str]):
+        self.type_is_interface: bool = type_is_interface
         # abstractproperties are checked for at instantiation.
         # When concrete classes use a @property then they are removed from this set
         self.abstractproperties = frozenset(abstract_properties)
-        self.interface_method_names = frozenset(interface_method_signatures.keys())  # type: FrozenSet[str]
-        self.interface_attribute_names = frozenset(interface_attribute_names)  # type: FrozenSet[str]
+        self.interface_method_names = frozenset(interface_method_signatures.keys())
+        self.interface_attribute_names = frozenset(interface_attribute_names)
         self.interface_method_signatures = interface_method_signatures
-        self.adapters = weakref.WeakKeyDictionary()
-        self.structural_subclasses = set()
-        self.impl_wrapper_type = None
+        self.adapters = weakref.WeakKeyDictionary()  # type: ignore
+        self.registered_types = weakref.WeakSet()  # type: ignore
+        self.structural_subclasses: Set[type] = set()
+        self.impl_wrapper_type: Optional[type] = None
 
     @property
-    def interface_names(self):
+    def interface_names(self) -> FrozenSet[str]:
         return self.interface_method_names.union(self.interface_attribute_names)
 
 
 class _ImplementationWrapper(object):
-    def __init__(self, implementation, interface):
+    def __init__(self, implementation: Any, interface: AnInterfaceType):
         object.__setattr__(self, '_ImplementationWrapper__impl', implementation)
         object.__setattr__(self, '_ImplementationWrapper__interface', interface)
         object.__setattr__(self, '_ImplementationWrapper__interface_attrs', interface._pi.interface_names)
         object.__setattr__(self, '_ImplementationWrapper__interface_name', interface.__name__)
 
-    def __getattr__(self, attr):
+    def __getattr__(self, attr: str) -> Any:
         impl = self.__impl
         if attr in self.__interface_attrs:
             return getattr(impl, attr)
         else:
             raise AttributeError("'{}' interface has no attribute '{}'".format(self.__interface_name, attr))
 
-    def __setattr__(self, key, value):
+    def __setattr__(self, key: str, value: Any) -> None:
         if key in self.__interface_attrs:
             setattr(self.__impl, key, value)
         else:
             raise AttributeError("'{}' interface has no attribute '{}'".format(self.__interface_name, key))
 
 
-def _builtin_attrs(name):
+def _builtin_attrs(name: str) -> bool:
     """ These attributes are ignored when checking ABC types for emptyness.
     """
     return name in ('__doc__', '__module__', '__qualname__', '__abstractmethods__', '__dict__',
                     '__metaclass__', '__weakref__', '__subclasshook__', '__orig_bases__',
                     '_abc_cache', '_abc_impl', '_abc_registry', '_abc_negative_cache_version', '_abc_negative_cache',
                     '_pi', '_pi_unwrap_decorators')
 
 
-def get_pi_attribute(cls, attr_name, default=None):
+def get_pi_attribute(cls: Type, attr_name: str, default: Any = None) -> Any:
     if hasattr(cls, '_pi'):
         return getattr(cls._pi, attr_name)
     else:
         return default
 
 
-def _type_is_interface(cls):
+def _type_is_interface(cls: type) -> bool:
     """ Return True if cls is a pure interface or an empty ABC class"""
     if cls is object:
         return False
     if hasattr(cls, '_pi'):
         return cls._pi.type_is_interface
     if cls is Generic:
         return True  # this class is just for type hinting
@@ -118,17 +126,17 @@
                     if func is not None and not _is_empty_function(func):
                         return False
         return True
 
     return False
 
 
-def _get_abc_interface_props_and_funcs(cls):
-    properties = set()
-    function_sigs = {}
+def _get_abc_interface_props_and_funcs(cls: Type[abc.ABC]) -> Tuple[Set[str], Dict[str, Signature]]:
+    properties: Set[str] = set()
+    function_sigs: Dict[str, Signature] = {}
     if not hasattr(cls, '__abstractmethods__'):
         return properties, function_sigs
     for name in cls.__abstractmethods__:
         if _builtin_attrs(name):
             pass  # shortcut
         value = getattr(cls, name)
         if isinstance(value, (staticmethod, classmethod, types.MethodType)):
@@ -138,23 +146,23 @@
             function_sigs[name] = signature(value)
         elif isinstance(value, property):
             properties.add(name)
 
     return properties, function_sigs
 
 
-def _unwrap_function(func):
+def _unwrap_function(func: Any) -> Any:
     """ Look for decorated functions and return the wrapped function.
     """
     while hasattr(func, '__wrapped__'):
         func = func.__wrapped__
     return func
 
 
-def _is_empty_function(func, unwrap=False):
+def _is_empty_function(func: Any, unwrap: bool = False) -> bool:
     """ Return True if func is considered empty.
      All functions with no return statement have an implicit return None - this is explicit in the code object.
     """
     if isinstance(func, (staticmethod, classmethod, types.MethodType)):
         func = func.__func__
     if isinstance(func, property):
         func = property.fget
@@ -182,120 +190,88 @@
         byte_code = byte_code[2:]  # remove RESUME opcode added in 3.11
     if byte_code.startswith(b'\t\x00'):
         byte_code = byte_code[2:]  # remove NOP opcode
     if byte_code in (b'd\x00\x00S', b'd\x00S\x00') and code_obj.co_consts[0] is None:
         return True
     if byte_code in (b'd\x01\x00S', b'd\x01S\x00') and code_obj.co_consts[1] is None:
         return True
+    if byte_code == b'y\x00' and code_obj.co_consts[0] is None:  # RETURN_CONST in 3.12+
+        return True
     # convert bytes to instructions
-    instructions = _get_instructions(code_obj)
+    instructions = list(dis.get_instructions(code_obj))
     if len(instructions) < 2:
         return True  # this never happens
     if instructions[0].opname == 'GEN_START':
         instructions.pop(0)
     if instructions[0].opname == 'RESUME':
         instructions.pop(0)
     if instructions[0].opname == 'NOP':
         instructions.pop(0)
     if instructions[0].opname == 'RETURN_GENERATOR':
         instructions.pop(0)
         if instructions[0].opname == 'POP_TOP':
             instructions.pop(0)
+        # All generator functions end with these 2 opcodes in 3.12+
+        if (len(instructions) > 2 and
+                instructions[-2].opname == 'CALL_INTRINSIC_1' and
+                instructions[-1].opname == 'RERAISE'):
+            instructions = instructions[:-2]  # remove last 2 instructions
     if instructions[0].opname == 'RESUME':
         instructions.pop(0)
     if instructions[0].opname == 'NOP':
         instructions.pop(0)
     if instructions[-1].opname == 'RETURN_VALUE':  # returns TOS (top of stack)
         instruction = instructions[-2]
         if not (instruction.opname == 'LOAD_CONST' and code_obj.co_consts[instruction.arg] is None):  # TOS is None
             return False  # return is not None
         instructions = instructions[:-2]
+    if len(instructions) > 0 and instructions[-1].opname == 'RETURN_CONST' and instructions[-1].argval is None:  # returns constant
+        instructions.pop(-1)
     if len(instructions) == 0:
         return True
     # look for raise NotImplementedError
     if instructions[-1].opname == 'RAISE_VARARGS':
         # the thing we are raising should be the result of __call__  (instantiating exception object)
         if instructions[-2].opname in ('CALL_FUNCTION', 'CALL'):
             for instr in instructions[-3::-1]:
                 if instr.opname == 'LOAD_GLOBAL':
-                    return instr.argval == 'NotImplementedError'
+                    return bool(instr.argval == 'NotImplementedError')
 
     return False
 
 
-_Instruction = collections.namedtuple('_Instruction', ('opcode', 'opname', 'arg', 'argval'))
-
-
-def _get_instructions(code_obj):
-    if hasattr(dis, 'get_instructions'):
-        return list(dis.get_instructions(code_obj))
-
-    instructions = []
-    instruction = None
-    for byte in code_obj.co_code:
-        if instruction is None:
-            instruction = [byte]
-        else:
-            instruction.append(byte)
-        if instruction[0] < dis.HAVE_ARGUMENT or len(instruction) == 3:
-            op_code = instruction[0]
-            op_name = dis.opname[op_code]
-            if instruction[0] < dis.HAVE_ARGUMENT:
-                instructions.append(_Instruction(op_code, op_name, None, None))
-            else:
-                arg = instruction[1]
-                instructions.append(_Instruction(op_code, op_name, arg, arg))
-            instruction = None
-    return instructions
-
-
-def _is_descriptor(obj):  # in our context we only care about __get__
+def _is_descriptor(obj: Any) -> bool:  # in our context we only care about __get__
     return hasattr(obj, '__get__')
 
 
 class _ParamTypes(object):
-    def __init__(self, pos_only, pos_or_kw, vararg, kw_only, varkw):
+    def __init__(self, pos_only: List[Parameter], pos_or_kw: List[Parameter],
+                 vararg: List[Parameter], kw_only: List[Parameter], varkw: List[Parameter]):
         self.pos_only = pos_only
         self.pos_or_kw = pos_or_kw
         self.vararg = vararg
         self.kw_only = kw_only
         self.varkw = varkw
         self.positional = pos_only + pos_or_kw
         self.keyword = pos_or_kw + kw_only
 
 
-def _signature_info(arg_spec):
-    # type: (List[Parameter]) -> _ParamTypes
+def _signature_info(arg_spec: Iterable[Parameter]) -> _ParamTypes:
     param_types = collections.defaultdict(list)
     for param in arg_spec:
         param_types[param.kind].append(param)
 
     return _ParamTypes(param_types[Parameter.POSITIONAL_ONLY],
                        param_types[Parameter.POSITIONAL_OR_KEYWORD],
                        param_types[Parameter.VAR_POSITIONAL],
                        param_types[Parameter.KEYWORD_ONLY],
                        param_types[Parameter.VAR_KEYWORD]
                        )
 
 
-def _required_params(param_list):
-    """ return params without a default"""
-    # params with defaults come last
-    for i, p in enumerate(param_list):
-        if p.default is not Parameter.empty:
-            return param_list[:i]
-    # no defaults
-    return param_list
-
-
-def _kw_names_match(func, base):
-    func_names = set(p.name for p in func)
-    return all(p.name in func_names for p in base)
-
-
 def _positional_args_match(func_list, base_list, vararg, base_kwo):
     # arguments are positional - so name doesn't matter
     # func may not have fewer parameters
     if len(base_list) > len(func_list):
         if not vararg:  # unless it has varargs
             return False
     # extra parameters must be have defaults (be optional)
@@ -342,16 +318,15 @@
         func_args = {p.name: p for p in func_list}
         for bp in base_list:
             if bp.name not in func_args:
                 return False
     return True
 
 
-def _signatures_are_consistent(func_sig, base_sig):
-    # type: (Signature, Signature) -> bool
+def _signatures_are_consistent(func_sig: Signature, base_sig: Signature) -> bool:
     """
     :param func_sig: Signature of overriding function
     :param base_sig: Signature of base class function
     :return: True if signature of func is Liskov substitutable for base.
     """
     base = _signature_info(base_sig.parameters.values())
     func = _signature_info(func_sig.parameters.values())
@@ -494,20 +469,20 @@
         warnings.warn('Class {module}.{sub_name} implements {cls_name}.\n'
                       'Consider inheriting {cls_name} or using {cls_name}.register({sub_name})'
                       .format(cls_name=cls.__name__, sub_name=subclass.__name__, module=subclass.__module__),
                       stacklevel=stacklevel)
     return True
 
 
-def _get_adapter(cls, obj_type):
-    # type: (Type[PI], Type[Any]) -> Optional[Callable]
+def _get_adapter(cls: AnInterfaceType, obj_type: Type) -> Optional[Callable]:
     """ Returns a callable that adapts objects of type obj_type to this interface or None if no adapter exists.
     """
-    adapters = {}
-    candidate_interfaces = [cls] + cls.__subclasses__()
+    adapters = {}  # type: ignore
+    # registered interfaces can come from cls.register(AnotherInterface) or @sub_interface_of(AnotherInterface)(cls)
+    candidate_interfaces = [cls] + cls.__subclasses__() + list(cls._pi.registered_types)
     candidate_interfaces.reverse()  # prefer this class over sub-class adapters
     for subcls in candidate_interfaces:
         if type_is_interface(subcls):
             adapters.update(subcls._pi.adapters)
     if not adapters:
         return None
 
@@ -696,123 +671,117 @@
             yield f
 
     def optional_adapt(cls, obj, allow_implicit=False, interface_only=None):
         if obj is None:
             return None
         return InterfaceType.adapt(cls, obj, allow_implicit=allow_implicit, interface_only=interface_only)
 
+    def register(cls, subclass: Type[_T]) -> Type[_T]:
+        if type_is_interface(cls):
+            cls._pi.registered_types.add(subclass)  # type: ignore[attr-defined]
+        return super().register(subclass)
+
 
 class Interface(abc.ABC, metaclass=InterfaceType):
     # These methods don't need to be here, as they would resolve to the meta-class methods anyway.
-    # However including them here means we can add type hints that would otherwise be ambiguous on the meta-class.
+    # However, including them here means we can add type hints that would otherwise be ambiguous on the meta-class.
+    _pi: _PIAttributes
 
     @classmethod
-    def provided_by(cls, obj, allow_implicit=True):
-        # type: (Any, bool) -> bool
+    def provided_by(cls, obj, allow_implicit: bool = True) -> bool:
         """ Returns True if obj provides this interface.
         provided_by(cls, obj) is equivalent to isinstance(obj, cls) unless allow_implicit is True
         If allow_implicit is True then returns True if interface duck-type check passes.
         Returns False otherwise.
         """
         return InterfaceType.provided_by(cls, obj, allow_implicit=allow_implicit)
 
     @classmethod
-    def interface_only(cls, implementation):
-        # type: (Type[PI], PI) -> PI
+    def interface_only(cls: Type[AnInterface], implementation: AnInterface) -> AnInterface:
         """ Returns a wrapper around implementation that provides ONLY this interface. """
         return InterfaceType.interface_only(cls, implementation)
 
     @classmethod
-    def adapt(cls, obj, allow_implicit=False, interface_only=None):
-        # type: (Type[PI], Any, bool, Optional[bool]) -> PI
+    def adapt(cls: Type[AnInterface], obj: Any,
+              allow_implicit: bool = False, interface_only: Optional[bool] = None) -> AnInterface:
         """ Adapts obj to interface, returning obj if to_interface.provided_by(obj, allow_implicit) is True
         and raising ValueError if no adapter is found
         If interface_only is True, or interface_only is None and is_development is True then the
         returned object is wrapped by an object that only provides the methods and properties defined by to_interface.
         """
         return InterfaceType.adapt(cls, obj, allow_implicit=allow_implicit, interface_only=interface_only)
 
     @classmethod
-    def adapt_or_none(cls, obj, allow_implicit=False, interface_only=None):
-        # type: (Type[PI], Any, bool, Optional[bool]) -> Optional[PI]
+    def adapt_or_none(cls: Type[AnInterface], obj,
+                      allow_implicit: bool = False, interface_only: Optional[bool] = None) -> Optional[AnInterface]:
         """ Adapt obj to to_interface or return None if adaption fails """
         return InterfaceType.adapt_or_none(cls, obj, allow_implicit=allow_implicit, interface_only=interface_only)
 
     @classmethod
-    def can_adapt(cls, obj, allow_implicit=False):
-        # type: (Any, bool) -> bool
+    def can_adapt(cls, obj, allow_implicit: bool = False) -> bool:
         """ Returns True if adapt(obj, allow_implicit) will succeed."""
         return InterfaceType.can_adapt(cls, obj, allow_implicit=allow_implicit)
 
     @classmethod
-    def filter_adapt(cls, objects, allow_implicit=False, interface_only=None):
-        # type: (Type[PI], Iterable[Any], bool, Optional[bool]) -> Iterable[PI]
+    def filter_adapt(cls: Type[AnInterface], objects: Iterable,
+                     allow_implicit: bool = False, interface_only: Optional[bool] = None) -> Iterable[AnInterface]:
         """ Generates adaptions of the given objects to this interface.
         Objects that cannot be adapted to this interface are silently skipped.
         """
         return InterfaceType.filter_adapt(cls, objects, allow_implicit=allow_implicit,
                                           interface_only=interface_only)
 
     @classmethod
-    def optional_adapt(cls, obj, allow_implicit=False, interface_only=None):
-        # type: (Type[PI], Any, bool, Optional[bool]) -> Optional[PI]
+    def optional_adapt(cls: Type[AnInterface], obj,
+                       allow_implicit: bool = False, interface_only: Optional[bool] = None) -> Optional[AnInterface]:
         """ Adapt obj to to_interface or return None if adaption fails """
         return InterfaceType.optional_adapt(cls, obj, allow_implicit=allow_implicit, interface_only=interface_only)
 
 
-def type_is_interface(cls):
-    # type: (Type[Any]) -> bool
+def type_is_interface(cls: Type) -> bool:  # -> TypeGuard[AnInterfaceType]
     """ Return True if cls is a pure interface"""
     try:
         if not issubclass(cls, Interface):
             return False
     except TypeError:  # handle non-classes
         return False
     return get_pi_attribute(cls, 'type_is_interface', False)
 
 
-def type_is_pure_interface(cls):
-    warnings.warn('type_is_pure_interface has been renamed to type_is_interface.')
-    return type_is_pure_interface(cls)
-
-
-def get_type_interfaces(cls):
-    # type: (Type[Any]) -> List[Type[Interface]]
+def get_type_interfaces(cls: Type) -> List[AnInterfaceType]:
     """ Returns all interfaces in the cls mro including cls itself if it is an interface """
     try:
         bases = cls.mro()
     except AttributeError:  # handle non-classes
         return []
-    return [base for base in bases if type_is_interface(base) and base is not Interface]
+    # type_is_interface ensures returned types are Interface subclasses by mypy doesn't know this
+    return [base for base in bases if type_is_interface(base) and base is not Interface]  # type: ignore [misc]
 
 
-def get_interface_names(interface):
-    # type: (Type[Interface]) -> FrozenSet[str]
+def get_interface_names(interface: Type) -> FrozenSet[str]:
     """ returns a frozen set of names (methods and attributes) defined by the interface.
     if interface is not a Interface subtype then an empty set is returned.
     """
     if type_is_interface(interface):
         return get_pi_attribute(interface, 'interface_names')
     else:
         return frozenset()
 
 
-def get_interface_method_names(interface):
-    # type: (Type[Interface]) -> FrozenSet[str]
+def get_interface_method_names(interface: Type) -> FrozenSet[str]:
     """ returns a frozen set of names of methods defined by the interface.
     if interface is not a Interface subtype then an empty set is returned
     """
     if type_is_interface(interface):
         return get_pi_attribute(interface, 'interface_method_names')
     else:
         return frozenset()
 
 
-def get_interface_attribute_names(interface):
-    # type: (Type[Interface]) -> FrozenSet[str]
+def get_interface_attribute_names(interface: Type) -> FrozenSet[str]:
     """ returns a frozen set of names of attributes defined by the interface
     if interface is not a Interface subtype then an empty set is returned
     """
     if type_is_interface(interface):
         return get_pi_attribute(interface, 'interface_attribute_names')
     else:
         return frozenset()
```

### Comparing `pure_interface-7.1.0/pure_interface.egg-info/PKG-INFO` & `pure_interface-7.3.0/pure_interface.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: pure-interface
-Version: 7.1.0
+Version: 7.3.0
 Summary: A Python interface library that disallows function body content on interfaces and supports adaption.
 Home-page: https://github.com/seequent/pure_interface
 Download-URL: https://pypi.org/project/pure-interface/
 Author: Tim Mitchell
 Author-email: tim.mitchell@seequent.com
 License: MIT
 Keywords: abc interface adapt adaption mapper structural typing dataclass
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 pure_interface
 ==============
 
 A Python interface library that disallows function body content on interfaces and supports adaption.
@@ -33,15 +33,15 @@
 * Ensures that method overrides have compatible signatures
 * Supports interface adaption.
 * Supports optional structural type checking for ``Interface.provided_by(a)`` and ``Interface.adapt(a)``
 * Allows concrete implementations the flexibility to implement abstract properties as instance attributes.
 * ``Interface.adapt()`` can return an implementation wrapper that provides *only* the
   attributes and methods defined by ``Interface``.
 * Warns if ``provided_by`` did a structural type check when inheritance would work.
-* Supports python 3.7+
+* Supports python 3.8+
 
 A note on the name
 ------------------
 The phrase *pure interface* applies only to the first design goal - a class that defines only an interface with no
 implementation is a pure interface [*]_.
 In every other respect the zen of 'practicality beats purity' applies.
 
@@ -230,14 +230,30 @@
     if pure_iterface.missing_method_warnings:
         for warning in pure_iterface.get_missing_method_warnings():
             print(warning)
         exit(1)
 
 Note that missing properties are NOT checked for as they may be provided by instance attributes.
 
+Sub-Interfaces
+==============
+Sometimes your code only uses a small part of a large interface.  It can be useful (eg. for test mocking) to specify
+the sub part of the interface that your code requires.  This can be done with the ``sub_interface_of`` decorator.::
+
+    @sub_interface_of(IAnimal)
+    class IHeight(pure_interface.Interface):
+        height: float
+
+    def my_code(h: IHeight):
+        return "That's tall" if h.height > 100 else "Not so tall"
+
+The ``sub_interface_of`` decorator checks that the attributes and methods of the smaller interface match the larger interface.
+Function signatures must match exactly (not just be compatible).  The decorator will also use ``abc.register`` so that
+``isinstance(Animal(), IHeight)`` returns ``True``.
+
 Adaption
 ========
 
 Registering Adapters
 --------------------
 
 Adapters for an interface are registered with the ``adapts`` decorator or with
@@ -342,14 +358,18 @@
     class IntToB(IB, object):
         def __init__(self, x):
             self.foo = self.bar = x
 
 Then  ``IA.adapt(4)`` will use the ``IntToB`` adapter to adapt ``4`` to ``IA`` (unless there is already an adapter
 from ``int`` to ``IA``)
 
+Further, if an interface is decorated with ``sub_interface_of``, adapters for the larger interface will be used if
+a direct adapter is not found.
+
+
 Structural Type Checking
 ========================
 
 Structural_ type checking checks if an object has the attributes and methods defined by the interface.
 
 As interfaces are inherited, you can usually use ``isinstance(obj, MyInterface)`` to check if an interface is provided.
 An alternative to ``isinstance()`` is the ``Interface.provided_by(obj)`` classmethod which will fall back to structural type
@@ -572,16 +592,16 @@
             self.foo = 3
 
 If you supply more than one delegation rule (e.g. both ``pi_attr_mapping`` and ``pi_attr_fallack``) then
  ``pi_attr_delegates`` delegates are created first and any attributes defined there are now part of the class.
 Then ``pi_attr_mapping`` delegates are created (and become part of the class) and finally ``pi_attr_fallback`` is processed.
 Thus if there are duplicate delegates defined, the one defined first takes precedence.
 
-Composition
------------
+Type Composition
+----------------
 A special case where all delegated attributes are defined in an ``Interface`` is handled by the ``composed_type`` factory function.
 ``composed_type`` takes 2 or more interfaces and returns a new type that inherits from all the interfaces with a
 constructor that takes instances that implement those interfaces (in the same order).  For exmaple::
 
     AT = composed_type(IAnimal, ITalker)
 
     a = Animal(5)
```

### Comparing `pure_interface-7.1.0/pure_interface.egg-info/SOURCES.txt` & `pure_interface-7.3.0/pure_interface.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 LICENSE
 README.rst
 pyproject.toml
 setup.cfg
 setup.py
 pure_interface/__init__.py
+pure_interface/_sub_interface.py
 pure_interface/adaption.py
 pure_interface/data_classes.py
 pure_interface/delegation.py
 pure_interface/errors.py
 pure_interface/interface.py
+pure_interface/py.typed
 pure_interface.egg-info/PKG-INFO
 pure_interface.egg-info/SOURCES.txt
 pure_interface.egg-info/dependency_links.txt
 pure_interface.egg-info/top_level.txt
 tests/test_adapt_args_anno.py
 tests/test_adapt_args_no_anno.py
 tests/test_adaption.py
@@ -23,9 +25,10 @@
 tests/test_generic_support.py
 tests/test_implementation_checks.py
 tests/test_inheritance.py
 tests/test_isinstance.py
 tests/test_meta_classes.py
 tests/test_module_funcs.py
 tests/test_no_content_checks.py
+tests/test_sub_interfaces.py
 tests/test_tracker.py
 tests/test_versions_in_sync.py
```

### Comparing `pure_interface-7.1.0/setup.cfg` & `pure_interface-7.3.0/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 7572 655f 696e 7465 7266 6163   = pure_interfac
-00000020: 650d 0a76 6572 7369 6f6e 203d 2037 2e31  e..version = 7.1
+00000020: 650d 0a76 6572 7369 6f6e 203d 2037 2e33  e..version = 7.3
 00000030: 2e30 0d0a 6465 7363 7269 7074 696f 6e20  .0..description 
 00000040: 3d20 4120 5079 7468 6f6e 2069 6e74 6572  = A Python inter
 00000050: 6661 6365 206c 6962 7261 7279 2074 6861  face library tha
 00000060: 7420 6469 7361 6c6c 6f77 7320 6675 6e63  t disallows func
 00000070: 7469 6f6e 2062 6f64 7920 636f 6e74 656e  tion body conten
 00000080: 7420 6f6e 2069 6e74 6572 6661 6365 7320  t on interfaces 
 00000090: 616e 6420 7375 7070 6f72 7473 2061 6461  and supports ada
@@ -40,29 +40,33 @@
 00000270: 7069 6320 3a3a 2053 6f66 7477 6172 6520  pic :: Software 
 00000280: 4465 7665 6c6f 706d 656e 7420 3a3a 204c  Development :: L
 00000290: 6962 7261 7269 6573 0d0a 094c 6963 656e  ibraries...Licen
 000002a0: 7365 203a 3a20 4f53 4920 4170 7072 6f76  se :: OSI Approv
 000002b0: 6564 203a 3a20 4d49 5420 4c69 6365 6e73  ed :: MIT Licens
 000002c0: 650d 0a09 5072 6f67 7261 6d6d 696e 6720  e...Programming 
 000002d0: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
-000002e0: 6f6e 203a 3a20 332e 370d 0a09 5072 6f67  on :: 3.7...Prog
+000002e0: 6f6e 203a 3a20 332e 380d 0a09 5072 6f67  on :: 3.8...Prog
 000002f0: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
 00000300: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
-00000310: 380d 0a09 5072 6f67 7261 6d6d 696e 6720  8...Programming 
+00000310: 390d 0a09 5072 6f67 7261 6d6d 696e 6720  9...Programming 
 00000320: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
-00000330: 6f6e 203a 3a20 332e 390d 0a09 5072 6f67  on :: 3.9...Prog
-00000340: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
-00000350: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
-00000360: 3130 0d0a 0950 726f 6772 616d 6d69 6e67  10...Programming
-00000370: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
-00000380: 686f 6e20 3a3a 2033 2e31 310d 0a6c 6963  hon :: 3.11..lic
-00000390: 656e 7365 203d 204d 4954 0d0a 6c69 6365  ense = MIT..lice
-000003a0: 6e73 655f 6669 6c65 7320 3d20 4c49 4345  nse_files = LICE
-000003b0: 4e53 450d 0a0d 0a5b 6f70 7469 6f6e 735d  NSE....[options]
-000003c0: 0d0a 7061 636b 6167 6573 203d 2066 696e  ..packages = fin
-000003d0: 643a 0d0a 0d0a 5b6f 7074 696f 6e73 2e70  d:....[options.p
-000003e0: 6163 6b61 6765 732e 6669 6e64 5d0d 0a77  ackages.find]..w
-000003f0: 6865 7265 203d 202e 0d0a 696e 636c 7564  here = ...includ
-00000400: 6520 3d20 7075 7265 5f69 6e74 6572 6661  e = pure_interfa
-00000410: 6365 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d  ce....[egg_info]
-00000420: 0d0a 7461 675f 6275 696c 6420 3d20 0d0a  ..tag_build = ..
-00000430: 7461 675f 6461 7465 203d 2030 0d0a 0d0a  tag_date = 0....
+00000330: 6f6e 203a 3a20 332e 3130 0d0a 0950 726f  on :: 3.10...Pro
+00000340: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
+00000350: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
+00000360: 2e31 310d 0a09 5072 6f67 7261 6d6d 696e  .11...Programmin
+00000370: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+00000380: 7468 6f6e 203a 3a20 332e 3132 0d0a 6c69  thon :: 3.12..li
+00000390: 6365 6e73 6520 3d20 4d49 540d 0a6c 6963  cense = MIT..lic
+000003a0: 656e 7365 5f66 696c 6573 203d 204c 4943  ense_files = LIC
+000003b0: 454e 5345 0d0a 0d0a 5b6f 7074 696f 6e73  ENSE....[options
+000003c0: 5d0d 0a70 6163 6b61 6765 7320 3d20 6669  ]..packages = fi
+000003d0: 6e64 3a0d 0a0d 0a5b 6f70 7469 6f6e 732e  nd:....[options.
+000003e0: 7061 636b 6167 6573 2e66 696e 645d 0d0a  packages.find]..
+000003f0: 7768 6572 6520 3d20 2e0d 0a69 6e63 6c75  where = ...inclu
+00000400: 6465 203d 2070 7572 655f 696e 7465 7266  de = pure_interf
+00000410: 6163 650d 0a0d 0a5b 6f70 7469 6f6e 732e  ace....[options.
+00000420: 7061 636b 6167 655f 6461 7461 5d0d 0a70  package_data]..p
+00000430: 7572 655f 696e 7465 7266 6163 6520 3d20  ure_interface = 
+00000440: 7079 2e74 7970 6564 0d0a 0d0a 5b65 6767  py.typed....[egg
+00000450: 5f69 6e66 6f5d 0d0a 7461 675f 6275 696c  _info]..tag_buil
+00000460: 6420 3d20 0d0a 7461 675f 6461 7465 203d  d = ..tag_date =
+00000470: 2030 0d0a 0d0a                            0....
```

### Comparing `pure_interface-7.1.0/tests/test_adapt_args_anno.py` & `pure_interface-7.3.0/tests/test_adapt_args_anno.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 try:
     from unittest import mock
 except ImportError:
     import mock
 
 from pure_interface import adapt_args, AdaptionError
 import pure_interface
-from typing import Optional
+from typing import Optional, List
 
 
 class I1(pure_interface.Interface):
     foo: str
 
     def bar(self):
         pass
@@ -108,35 +108,47 @@
         with mock.patch('warnings.warn') as warn:
             @adapt_args
             def no_anno(x, y):
                 pass
 
             self.assertEqual(1, warn.call_count)
 
-    def test_type_error_raised_if_arg_not_subclass(self):
+    def test_adaption_error_raised_if_arg_not_subclass(self):
         with self.assertRaises(AdaptionError):
             @adapt_args(x=int)
             def some_func(x):
                 pass
 
-    def test_type_error_raised_if_positional_arg_not_func(self):
+    def test_adaption_error_raised_if_positional_arg_not_func(self):
         with self.assertRaises(AdaptionError):
             @adapt_args(I2)
             def some_func(x):
                 pass
 
-    def test_type_error_raised_if_multiple_positional_args(self):
+    def test_adaption_error_raised_if_multiple_positional_args(self):
         with self.assertRaises(AdaptionError):
             @adapt_args(I1, I2)
             def some_func(x):
                 pass
 
-    def test_type_error_raised_if_mixed_args(self):
+    def test_adaption_error_raised_if_mixed_args(self):
         with self.assertRaises(AdaptionError):
             @adapt_args(I1, y=I2)
             def some_func(x, y):
                 pass
 
-    def test_wrong_args_type_raises(self):
+    def test_wrong_args_type_raises_adaption_error(self):
         thing2 = Thing2()
         with self.assertRaises(ValueError):
             some_func(3, thing2)
+
+    def test_mixed_args_type_raises_adaption_error(self):
+        with self.assertRaises(AdaptionError):
+            adapt_args(some_func, x=3)
+
+    def test_unsupported_generic_annotations_are_skipped(self):
+        try:
+            @adapt_args
+            def some_func(x: List[int], y: I2):
+                pass
+        except Exception:
+            self.fail('Failed to ignore unsupported annotation')
```

### Comparing `pure_interface-7.1.0/tests/test_adapt_args_no_anno.py` & `pure_interface-7.3.0/tests/test_adapt_args_no_anno.py`

 * *Files identical despite different names*

### Comparing `pure_interface-7.1.0/tests/test_adaption.py` & `pure_interface-7.3.0/tests/test_adaption.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,15 +126,15 @@
     def __len__(self):
         return 5
 
 
 class TestAdaption(unittest.TestCase):
     @classmethod
     def setUpClass(cls):
-        interface.is_development = True
+        pure_interface.set_is_development(True)
 
     def test_adaption_passes(self):
         talker = Talker()
         s = ISpeaker.adapt(talker, interface_only=False)
 
         self.assertTrue(ISpeaker.provided_by(s, allow_implicit=False))
         self.assertEqual(s.speak(5), 'talk')
@@ -229,19 +229,32 @@
         self.assertEqual(len(output), 3)
         self.assertIsInstance(output[0], Speaker)
         speaker = output[1]
         self.assertIs(output[2], a_speaker)
         self.assertIsInstance(speaker, TalkerToSpeaker)
         self.assertIs(speaker._talker, a_talker)
 
+    def test_fail_if_no_to_interface_for_func(self):
+        with self.assertRaises(interface.InterfaceError):
+            @pure_interface.adapts(int)
+            def foo(arg):
+                return None
+
+    def test_manual_interface_only(self):
+        topic_speaker = TopicSpeaker('Python')
+        s = ITopicSpeaker.interface_only(topic_speaker)
+
+        self.assertIsInstance(s, interface._ImplementationWrapper)
+        self.assertIsInstance(s, ITopicSpeaker)
+
 
 class TestAdaptionToInterfaceOnly(unittest.TestCase):
     @classmethod
     def setUpClass(cls):
-        interface.is_development = True
+        pure_interface.set_is_development(True)
 
     def test_wrapping_works(self):
         topic_speaker = TopicSpeaker('Python')
         s = ITopicSpeaker.adapt(topic_speaker)
         topic_speaker2 = TopicSpeaker('Interfaces')
         t = ITopicSpeaker.adapt(topic_speaker2)
 
@@ -376,7 +389,11 @@
         except TypeError:
             self.fail('calling interface only failed')
 
         try:
             len(dunder)
         except:
             self.fail('len() interface only failed')
+
+    def test_can_adapt(self):
+        self.assertFalse(ITalker.can_adapt('hello'))
+        self.assertTrue(ITalker.can_adapt(Talker()))
```

### Comparing `pure_interface-7.1.0/tests/test_dataclass_support.py` & `pure_interface-7.3.0/tests/test_dataclass_support.py`

 * *Files 12% similar despite different names*

```diff
@@ -34,7 +34,24 @@
                 f = Foo(2, 'two', 34.0)
                 self.assertEqual(2, f.a)
                 self.assertEqual('two', f.b)
                 self.assertEqual(34.0, f.c)
                 self.assertEqual('a=2, b=two, c=34.0', f.foo())
             except Exception as exc:
                 self.fail(str(exc))
+
+        def test_data_class_with_args(self):
+            try:
+                @dataclass(frozen=True)
+                class FrozenFoo(IFoo, object):
+                    c: float = 12.0
+
+                    def foo(self):
+                        return 'a={}, b={}, c={}'.format(self.a, self.b, self.c)
+
+            except Exception as exc:
+                self.fail(str(exc))
+
+            f = Foo(a=1, b='two')
+            self.assertEqual(1, f.a)
+            self.assertEqual('two', f.b)
+            self.assertEqual(12.0, f.c)
```

### Comparing `pure_interface-7.1.0/tests/test_delegate.py` & `pure_interface-7.3.0/tests/test_delegate.py`

 * *Files 2% similar despite different names*

```diff
@@ -297,14 +297,18 @@
             DSubFallback(Talker())  # no implementation of chat
 
     def test_delegate_subclass_fallback2(self):
         """Check subclass fallbacks are used for missing attributes."""
         d = DSubFallback2(Talker())
         self.assertEqual('chat', d.chat())
 
+    def test_delegate_provides_fails(self):
+        with self.assertRaises(pure_interface.InterfaceError):
+            DFallback.provided_by(ITalker)
+
 
 class CompositionTest(unittest.TestCase):
 
     def test_type_composition(self):
         a = Point(1, 2)
         b = Talker()
 
@@ -372,7 +376,16 @@
                 def __init__(self):
                     self.a = Talker()
 
             x = UnusedFallbackDelegate()
 
         except Exception as exc:
             self.fail(str(exc))
+
+    def test_fail_on_unsupported_type(self):
+        with self.assertRaises(ValueError):
+            delegation.composed_type(str, int)
+
+    def test_too_many_interfaces(self):
+        with mock.patch('pure_interface.delegation._letters', 'a'):
+            with self.assertRaises(ValueError):
+                delegation.composed_type(ITalker, IPoint)
```

### Comparing `pure_interface-7.1.0/tests/test_func_sigs3.py` & `pure_interface-7.3.0/tests/test_func_sigs3.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,16 +88,15 @@
         return False
     kwargs = ba.arguments.get('kwargs', {})
     if not all(k == v for k, v in kwargs.items()):
         return False
     return True
 
 
-def test_call(spec_func, impl_func):
-    # type: (types.FunctionType, types.FunctionType) -> bool
+def test_call(spec_func: types.FunctionType, impl_func: types.FunctionType) -> bool:
     """ call the function with parameters as indicated by the parameter list
     """
     spec_sig = pure_interface.interface.signature(spec_func)
     impl_sig = pure_interface.interface.signature(impl_func)
 
     pos_only = [p for p in spec_sig.parameters.values() if p.kind == p.POSITIONAL_ONLY]
     num_po = len(pos_only)
@@ -154,15 +153,15 @@
         kwargs = {x: x for x in kwo_args[:i]}
         yield kwargs
 
 
 class TestFunctionSigsPy3(unittest.TestCase):
     @classmethod
     def setUpClass(cls):
-        interface.is_development = True
+        pure_interface.set_is_development(True)
 
     def check_signatures(self, int_func, impl_func, expected_result):
         interface_sig = pure_interface.interface.signature(int_func)
         concrete_sig = pure_interface.interface.signature(impl_func)
         reality = test_call(int_func, impl_func)
         self.assertEqual(expected_result, reality,
                          '{}, {}. Reality does not match expectations'.format(int_func.__name__, impl_func.__name__))
```

### Comparing `pure_interface-7.1.0/tests/test_function_sigs.py` & `pure_interface-7.3.0/tests/test_function_sigs.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,16 +79,15 @@
         return False
     kwargs = ba.arguments.get('kwargs', {})
     if not all(k == v for k, v in kwargs.items()):
         return False
     return True
 
 
-def test_call(spec_func, impl_func):
-    # type: (types.FunctionType, types.FunctionType) -> bool
+def test_call(spec_func: types.FunctionType, impl_func: types.FunctionType) -> bool:
     """ call the function with parameters as indicated by the parameter list
     """
     spec_sig = pure_interface.interface.signature(spec_func)
     impl_sig = pure_interface.interface.signature(impl_func)
     pos_or_kw = [p for p in spec_sig.parameters.values() if p.kind == p.POSITIONAL_OR_KEYWORD]
     pok_args = [p.name for p in pos_or_kw]
     pok_def = {p.name: p.name for p in pos_or_kw if p.default is not p.empty}
@@ -121,15 +120,15 @@
             return False
     return True
 
 
 class TestFunctionSignatureChecks(unittest.TestCase):
     @classmethod
     def setUpClass(cls):
-        interface.is_development = True
+        pure_interface.set_is_development(True)
 
     def check_signatures(self, int_func, impl_func, expected_result):
         interface_sig = pure_interface.interface.signature(int_func)
         concrete_sig = pure_interface.interface.signature(impl_func)
         reality = test_call(int_func, impl_func)
         self.assertEqual(expected_result, reality,
                          '{}, {}. Reality does not match expectations'.format(int_func.__name__, impl_func.__name__))
@@ -332,15 +331,15 @@
                 def grow(self, height):
                     pass
 
 
 class TestDisableFunctionSignatureChecks(unittest.TestCase):
     @classmethod
     def setUpClass(cls):
-        interface.is_development = False
+        pure_interface.set_is_development(False)
 
     def test_too_many_passes(self):
         try:
             class Animal(IAnimal, object):
                 def speak(self, volume, msg):
                     pass
             a = Animal()
```

### Comparing `pure_interface-7.1.0/tests/test_generic_support.py` & `pure_interface-7.3.0/tests/test_generic_support.py`

 * *Files identical despite different names*

### Comparing `pure_interface-7.1.0/tests/test_implementation_checks.py` & `pure_interface-7.3.0/tests/test_implementation_checks.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 import abc
 import unittest
 import warnings
 
 from pure_interface import *
 from pure_interface import interface
 
-try:
-    from unittest import mock
-except ImportError:
-    import mock
+from unittest import mock
+
 
 class ADescriptor(object):
     def __init__(self, value):
         self._value = value
 
     def __get__(self, instance, owner):
         return self._value
@@ -219,15 +217,15 @@
         except:
             self.fail('Overriding function with descriptor failed')
         s = Simple()
         self.assertEqual(s.foo(), 1)
 
     def test_missing_methods_warning(self):
         # assemble
-        interface.is_development = True
+        set_is_development(True)
         interface.missing_method_warnings = []
         # act
 
         with warnings.catch_warnings():
             warnings.simplefilter('ignore')
 
             class SimpleSimon(ISimple, object):
@@ -275,14 +273,19 @@
             height = ADescriptor('really tall')
 
         class Test(HeightDescr, IPlant):
             pass
 
         self.assertEqual(frozenset([]), Test._pi.abstractproperties)
 
+    def test_set_development(self):
+        for value in True, False:
+            set_is_development(value)
+            self.assertEqual(value, get_is_development())
+
 
 class TestPropertyImplementations(unittest.TestCase):
     def test_abstract_property_override_passes(self):
         class Animal(IGrowingAnimal, object):
             def get_height(self):
                 return 10
```

### Comparing `pure_interface-7.1.0/tests/test_inheritance.py` & `pure_interface-7.3.0/tests/test_inheritance.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import unittest
 
 import pure_interface
-from pure_interface import interface
 
 
 class IGrowingThing(pure_interface.Interface):
     def get_height(self):
         return None
 
     def set_height(self, height):
@@ -62,22 +61,22 @@
 
 class Y(object):
     pass
 
 
 class TestInheritance(unittest.TestCase):
     def test_bad_mixin_class_is_checked(self):
-        interface.is_development = True
+        pure_interface.set_is_development(True)
 
         with self.assertRaises(pure_interface.InterfaceError):
             class Growing(BadGrowingMixin, IGrowingThing):
                 pass
 
     def test_ok_mixin_class_passes(self):
-        interface.is_development = True
+        pure_interface.set_is_development(True)
 
         class Growing(GrowingMixin, IGrowingThing):
             pass
 
         g = Growing()
         self.assertEqual(g.get_height(), 10)
```

### Comparing `pure_interface-7.1.0/tests/test_isinstance.py` & `pure_interface-7.3.0/tests/test_isinstance.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import io
 import unittest
 from unittest import mock
 import warnings
 
 import pure_interface
-from pure_interface import interface
 from tests.interface_module import IAnimal
 
 
 class TestIsInstanceChecks(unittest.TestCase):
     def test_abc_register(self):
         class Animal(object):
             pass
@@ -57,15 +56,15 @@
                 return True
 
         c = Cat()
         with self.assertRaises(pure_interface.InterfaceError):
             Cat.provided_by(c, allow_implicit=False)
 
     def test_warning_issued_once(self):
-        interface.is_development = True
+        pure_interface.set_is_development(True)
 
         class Cat2(object):
             def speak(self, volume):
                 print('meow')
 
             @property
             def height(self):
@@ -75,15 +74,15 @@
         with mock.patch('warnings.warn', warn):
             IAnimal.provided_by(Cat2(), allow_implicit=True)
             IAnimal.provided_by(Cat2(), allow_implicit=True)
 
         self.assertEqual(warn.call_count, 1)
 
     def test_warning_not_issued(self):
-        interface.is_development = False
+        pure_interface.set_is_development(False)
 
         class Cat3(object):
             def speak(self, volume):
                 print('meow')
 
             @property
             def height(self):
@@ -92,15 +91,15 @@
         warn = mock.MagicMock()
         with mock.patch('warnings.warn', warn):
             IAnimal.provided_by(Cat3(), allow_implicit=True)
 
         warn.assert_not_called()
 
     def test_warning_contents(self):
-        interface.is_development = True
+        pure_interface.set_is_development(True)
 
         class Cat4(object):
             def speak(self, volume):
                 print('meow')
 
             @property
             def height(self):
@@ -113,15 +112,15 @@
         msg = s.getvalue()
         self.assertIn('Cat4', msg)
         self.assertIn(Cat4.__module__, msg)
         self.assertNotIn('pure_interface', msg.split('\n')[0])
         self.assertIn('IAnimal', msg)
 
     def test_warning_contents_adapt(self):
-        interface.is_development = True
+        pure_interface.set_is_development(True)
 
         class Cat5(object):
             def speak(self, volume):
                 print('meow')
 
             @property
             def height(self):
```

### Comparing `pure_interface-7.1.0/tests/test_meta_classes.py` & `pure_interface-7.3.0/tests/test_meta_classes.py`

 * *Files identical despite different names*

### Comparing `pure_interface-7.1.0/tests/test_module_funcs.py` & `pure_interface-7.3.0/tests/test_module_funcs.py`

 * *Files identical despite different names*

### Comparing `pure_interface-7.1.0/tests/test_no_content_checks.py` & `pure_interface-7.3.0/tests/test_no_content_checks.py`

 * *Files identical despite different names*

### Comparing `pure_interface-7.1.0/tests/test_tracker.py` & `pure_interface-7.3.0/tests/test_tracker.py`

 * *Files 8% similar despite different names*

```diff
@@ -78,7 +78,33 @@
             return mocks[-1]
 
         tracker = AdapterTracker(mapping_factory=factory)
         t = Talker('hello')
 
         tracker.adapt(t, ISpeaker)
         self.assertTrue(len(mocks) > 1)
+
+    def test_adapt_or_none_works(self):
+        tracker = AdapterTracker()
+        t = Talker()
+
+        speaker = tracker.adapt_or_none(t, ISpeaker)
+
+        self.assertIsInstance(speaker, ISpeaker)
+
+    def test_adapt_or_none_returns_none(self):
+        tracker = AdapterTracker()
+
+        speaker = tracker.adapt_or_none('hello', ISpeaker)
+
+        self.assertIsNone(speaker)
+
+    def test_clear(self):
+        tracker = AdapterTracker()
+        t = Talker()
+        speaker1 = tracker.adapt_or_none(t, ISpeaker)
+
+        tracker.clear()
+
+        speaker2 = tracker.adapt_or_none(t, ISpeaker)
+        self.assertIsNot(speaker1, speaker2)
+
```

### Comparing `pure_interface-7.1.0/tests/test_versions_in_sync.py` & `pure_interface-7.3.0/tests/test_versions_in_sync.py`

 * *Files identical despite different names*

