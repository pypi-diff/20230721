# Comparing `tmp/immutabledict-2.2.5.tar.gz` & `tmp/immutabledict-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "immutabledict-2.2.5.tar", max compression
+gzip compressed data, was "immutabledict-3.0.0.tar", max compression
```

## Comparing `immutabledict-2.2.5.tar` & `immutabledict-3.0.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1072 2023-07-04 10:37:42.630829 immutabledict-2.2.5/LICENSE
--rw-r--r--   0        0        0     2180 2023-07-04 10:37:42.630829 immutabledict-2.2.5/README.md
--rw-r--r--   0        0        0     2481 2023-07-04 10:37:42.630829 immutabledict-2.2.5/immutabledict/__init__.py
--rw-r--r--   0        0        0        0 2023-07-04 10:37:42.630829 immutabledict-2.2.5/immutabledict/py.typed
--rw-r--r--   0        0        0     1045 2023-07-04 10:37:42.630829 immutabledict-2.2.5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-04 10:37:42.630829 immutabledict-2.2.5/tests/__init__.py
--rw-r--r--   0        0        0     5392 2023-07-04 10:37:42.630829 immutabledict-2.2.5/tests/test_immutabledict.py
--rw-r--r--   0        0        0     3249 1970-01-01 00:00:00.000000 immutabledict-2.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-07-21 18:13:55.780401 immutabledict-3.0.0/LICENSE
+-rw-r--r--   0        0        0     2116 2023-07-21 18:13:55.780401 immutabledict-3.0.0/README.md
+-rw-r--r--   0        0        0     2324 2023-07-21 18:13:55.780401 immutabledict-3.0.0/immutabledict/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-21 18:13:55.780401 immutabledict-3.0.0/immutabledict/py.typed
+-rw-r--r--   0        0        0     1045 2023-07-21 18:13:55.780401 immutabledict-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-21 18:13:55.780401 immutabledict-3.0.0/tests/__init__.py
+-rw-r--r--   0        0        0     7087 2023-07-21 18:13:55.780401 immutabledict-3.0.0/tests/test_immutabledict.py
+-rw-r--r--   0        0        0     3135 1970-01-01 00:00:00.000000 immutabledict-3.0.0/PKG-INFO
```

### Comparing `immutabledict-2.2.5/LICENSE` & `immutabledict-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `immutabledict-2.2.5/README.md` & `immutabledict-3.0.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -6,31 +6,31 @@
 
 A fork of the original [frozendict](https://github.com/slezica/python-frozendict), an immutable wrapper around dictionaries.
 This library is a pure Python, MIT-licensed alternative to the new LGPL-3.0 licensed [frozendict](https://github.com/Marco-Sulla/python-frozendict).
 
 It implements the complete mapping interface and can be used as a drop-in replacement for dictionaries where immutability is desired.
 The immutabledict constructor mimics dict, and all of the expected interfaces (iter, len, repr, hash, getitem) are provided. Note that an immutabledict does not guarantee the immutability of its values, so the utility of hash method is restricted by usage.
 
-The only difference is that the copy() method of immutable takes variable keyword arguments, which will be present as key/value pairs in the new, immutable copy.
-
 ## Installation
 
-Available as `immutabledict` on :
-- [pypi](https://pypi.org/project/immutabledict/)
-- [conda-forge](https://anaconda.org/conda-forge/immutabledict) (community-maintained, not an official release)
-- alpine as [py3-immutabledict](https://pkgs.alpinelinux.org/packages?name=py3-immutabledict)  (community-maintained, not an official release)
+Official release in [on pypy](https://pypi.org/project/immutabledict/) as `immutabledict`.
+
+**Community-maintained** releases are available:
+- On [conda-forge](https://anaconda.org/conda-forge/immutabledict) as `immutabledict`
+- On [various package repositories](https://repology.org/project/python:immutabledict/versions)
 
 ## Example
 
 ```python
 from immutabledict import immutabledict
 
 my_item = immutabledict({"a": "value", "b": "other_value"})
 print(my_item["a"]) # Print "value"
 ```
 
 ## Differences with the old original frozendict package
 
-- Dropped support of EOL Python versions (version 1.0.0 supports Python 3.5, versions <= 2.2.1 supports Python 3.6)
+- Dropped support of EOL Python versions (older versions of the library may support older Python versions)
 - Fixed `collections.Mapping` deprecation warning
 - Typing
 - [PEP 584 union operators](https://www.python.org/dev/peps/pep-0584/)
+- Keep the same signature for `copy()` as `dict` (starting with immutabledict 3.0.0), don't accept extra keyword arguments.
```

### Comparing `immutabledict-2.2.5/immutabledict/__init__.py` & `immutabledict-3.0.0/immutabledict/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from __future__ import annotations
 
 from collections import OrderedDict
 from typing import Any, Dict, Iterable, Iterator, Mapping, Optional, Type, TypeVar
 
-__version__ = "2.2.5"
+__version__ = "3.0.0"
 
 _K = TypeVar("_K")
-_V = TypeVar("_V")
+_V = TypeVar("_V", covariant=True)
 
 
 class immutabledict(Mapping[_K, _V]):
     """
     An immutable wrapper around dictionaries that implements
     the complete :py:class:`collections.Mapping` interface.
     It can be used as a drop-in replacement for dictionaries
@@ -18,38 +18,38 @@
     """
 
     dict_cls: Type[Dict[Any, Any]] = dict
 
     @classmethod
     def fromkeys(
         cls, seq: Iterable[_K], value: Optional[_V] = None
-    ) -> "immutabledict[_K, _V]":
+    ) -> immutabledict[_K, _V]:
         return cls(cls.dict_cls.fromkeys(seq, value))
 
     def __init__(self, *args: Any, **kwargs: Any) -> None:
         self._dict = self.dict_cls(*args, **kwargs)
         self._hash: Optional[int] = None
 
     def __getitem__(self, key: _K) -> _V:
         return self._dict[key]
 
     def __contains__(self, key: object) -> bool:
         return key in self._dict
 
-    def copy(self, **add_or_replace: _V) -> immutabledict[_K, _V]:
-        return self.__class__(self, **add_or_replace)
+    def copy(self) -> immutabledict[_K, _V]:
+        return self.__class__(self)
 
     def __iter__(self) -> Iterator[_K]:
         return iter(self._dict)
 
     def __len__(self) -> int:
         return len(self._dict)
 
     def __repr__(self) -> str:
-        return "%s(%r)" % (self.__class__.__name__, self._dict)
+        return "{}({!r})".format(self.__class__.__name__, self._dict)
 
     def __hash__(self) -> int:
         if self._hash is None:
             h = 0
             for key, value in self.items():
                 h ^= hash((key, value))
             self._hash = h
@@ -70,16 +70,13 @@
         new.update(self)
         return new
 
     def __ior__(self, other: Any) -> immutabledict[_K, _V]:
         raise TypeError(f"'{self.__class__.__name__}' object is not mutable")
 
 
-class ImmutableOrderedDict(immutabledict):
+class ImmutableOrderedDict(immutabledict[_K, _V]):
     """
     An immutabledict subclass that maintains key order.
-
-    Not necessary anymore as for Python >= 3.7 order is guaranteed with the normal
-    immutabledict class, but kept for compatibility purpose.
     """
 
     dict_cls = OrderedDict
```

### Comparing `immutabledict-2.2.5/pyproject.toml` & `immutabledict-3.0.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "immutabledict"
-version = "2.2.5"
+version = "3.0.0"
 description = "Immutable wrapper around dictionaries (a fork of frozendict)"
 authors = ["Corentin Garcia <corenting@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/corenting/immutabledict"
 keywords = ["immutable", "dictionary"]
 classifiers = [
@@ -16,15 +16,15 @@
 ]
 
 [tool.poetry.urls]
 "Changelog" = "https://github.com/corenting/immutabledict/blob/master/CHANGELOG.md"
 "Bug Tracker" = "https://github.com/corenting/immutabledict/issues"
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.8"
 
 [tool.poetry.dev-dependencies]
 black = "*"
 coverage = "*"
 mypy = "*"
 pdbpp = "*"
 pytest = "*"
```

### Comparing `immutabledict-2.2.5/PKG-INFO` & `immutabledict-3.0.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: immutabledict
-Version: 2.2.5
+Version: 3.0.0
 Summary: Immutable wrapper around dictionaries (a fork of frozendict)
 Home-page: https://github.com/corenting/immutabledict
 License: MIT
 Keywords: immutable,dictionary
 Author: Corentin Garcia
 Author-email: corenting@gmail.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Project-URL: Bug Tracker, https://github.com/corenting/immutabledict/issues
 Project-URL: Changelog, https://github.com/corenting/immutabledict/blob/master/CHANGELOG.md
@@ -30,32 +29,32 @@
 
 A fork of the original [frozendict](https://github.com/slezica/python-frozendict), an immutable wrapper around dictionaries.
 This library is a pure Python, MIT-licensed alternative to the new LGPL-3.0 licensed [frozendict](https://github.com/Marco-Sulla/python-frozendict).
 
 It implements the complete mapping interface and can be used as a drop-in replacement for dictionaries where immutability is desired.
 The immutabledict constructor mimics dict, and all of the expected interfaces (iter, len, repr, hash, getitem) are provided. Note that an immutabledict does not guarantee the immutability of its values, so the utility of hash method is restricted by usage.
 
-The only difference is that the copy() method of immutable takes variable keyword arguments, which will be present as key/value pairs in the new, immutable copy.
-
 ## Installation
 
-Available as `immutabledict` on :
-- [pypi](https://pypi.org/project/immutabledict/)
-- [conda-forge](https://anaconda.org/conda-forge/immutabledict) (community-maintained, not an official release)
-- alpine as [py3-immutabledict](https://pkgs.alpinelinux.org/packages?name=py3-immutabledict)  (community-maintained, not an official release)
+Official release in [on pypy](https://pypi.org/project/immutabledict/) as `immutabledict`.
+
+**Community-maintained** releases are available:
+- On [conda-forge](https://anaconda.org/conda-forge/immutabledict) as `immutabledict`
+- On [various package repositories](https://repology.org/project/python:immutabledict/versions)
 
 ## Example
 
 ```python
 from immutabledict import immutabledict
 
 my_item = immutabledict({"a": "value", "b": "other_value"})
 print(my_item["a"]) # Print "value"
 ```
 
 ## Differences with the old original frozendict package
 
-- Dropped support of EOL Python versions (version 1.0.0 supports Python 3.5, versions <= 2.2.1 supports Python 3.6)
+- Dropped support of EOL Python versions (older versions of the library may support older Python versions)
 - Fixed `collections.Mapping` deprecation warning
 - Typing
 - [PEP 584 union operators](https://www.python.org/dev/peps/pep-0584/)
+- Keep the same signature for `copy()` as `dict` (starting with immutabledict 3.0.0), don't accept extra keyword arguments.
```

