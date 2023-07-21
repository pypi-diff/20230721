# Comparing `tmp/dask-expr-0.1.0.tar.gz` & `tmp/dask-expr-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dask-expr-0.1.0.tar", last modified: Wed Jul 12 18:53:27 2023, max compression
+gzip compressed data, was "dask-expr-0.1.1.tar", last modified: Fri Jul 21 07:51:37 2023, max compression
```

## Comparing `dask-expr-0.1.0.tar` & `dask-expr-0.1.1.tar`

### file list

```diff
@@ -1,35 +1,37 @@
-drwxr-xr-x   0 patrick    (502) staff       (20)        0 2023-07-12 18:53:27.869967 dask-expr-0.1.0/
--rw-r--r--   0 patrick    (502) staff       (20)     1516 2023-07-12 18:00:13.000000 dask-expr-0.1.0/LICENSE.txt
--rw-r--r--   0 patrick    (502) staff       (20)     1963 2023-07-12 18:53:27.870056 dask-expr-0.1.0/PKG-INFO
--rw-r--r--   0 patrick    (502) staff       (20)     1100 2023-07-12 18:52:36.000000 dask-expr-0.1.0/README.md
-drwxr-xr-x   0 patrick    (502) staff       (20)        0 2023-07-12 18:53:27.870477 dask-expr-0.1.0/dask_expr/
--rw-r--r--   0 patrick    (502) staff       (20)      127 2023-07-12 17:51:26.000000 dask-expr-0.1.0/dask_expr/__init__.py
--rw-r--r--   0 patrick    (502) staff       (20)     1434 2023-07-12 17:17:51.000000 dask-expr-0.1.0/dask_expr/_align.py
--rw-r--r--   0 patrick    (502) staff       (20)    34291 2023-07-12 17:17:51.000000 dask-expr-0.1.0/dask_expr/_collection.py
--rw-r--r--   0 patrick    (502) staff       (20)     4982 2023-07-12 17:17:51.000000 dask-expr-0.1.0/dask_expr/_concat.py
--rw-r--r--   0 patrick    (502) staff       (20)    60041 2023-07-12 17:17:51.000000 dask-expr-0.1.0/dask_expr/_expr.py
--rw-r--r--   0 patrick    (502) staff       (20)    15912 2023-07-12 17:17:51.000000 dask-expr-0.1.0/dask_expr/_groupby.py
--rw-r--r--   0 patrick    (502) staff       (20)     9161 2023-07-12 17:17:51.000000 dask-expr-0.1.0/dask_expr/_merge.py
--rw-r--r--   0 patrick    (502) staff       (20)     2169 2023-07-12 17:17:51.000000 dask-expr-0.1.0/dask_expr/_quantiles.py
--rw-r--r--   0 patrick    (502) staff       (20)    16283 2023-07-12 17:17:51.000000 dask-expr-0.1.0/dask_expr/_reductions.py
--rw-r--r--   0 patrick    (502) staff       (20)    11011 2023-07-12 17:17:51.000000 dask-expr-0.1.0/dask_expr/_repartition.py
--rw-r--r--   0 patrick    (502) staff       (20)    27174 2023-07-12 17:17:51.000000 dask-expr-0.1.0/dask_expr/_shuffle.py
--rw-r--r--   0 patrick    (502) staff       (20)      217 2023-06-27 15:57:00.000000 dask-expr-0.1.0/dask_expr/_typing.py
--rw-r--r--   0 patrick    (502) staff       (20)      334 2023-06-29 09:41:00.000000 dask-expr-0.1.0/dask_expr/_util.py
--rw-r--r--   0 patrick    (502) staff       (20)      497 2023-07-12 18:53:27.870516 dask-expr-0.1.0/dask_expr/_version.py
--rw-r--r--   0 patrick    (502) staff       (20)     6228 2023-07-12 17:17:51.000000 dask-expr-0.1.0/dask_expr/datasets.py
-drwxr-xr-x   0 patrick    (502) staff       (20)        0 2023-07-12 18:53:27.869707 dask-expr-0.1.0/dask_expr/io/
--rw-r--r--   0 patrick    (502) staff       (20)       96 2023-05-16 14:29:09.000000 dask-expr-0.1.0/dask_expr/io/__init__.py
--rw-r--r--   0 patrick    (502) staff       (20)      980 2023-06-26 11:37:37.000000 dask-expr-0.1.0/dask_expr/io/csv.py
--rw-r--r--   0 patrick    (502) staff       (20)     3068 2023-07-12 17:17:51.000000 dask-expr-0.1.0/dask_expr/io/io.py
--rw-r--r--   0 patrick    (502) staff       (20)    31853 2023-07-12 17:17:51.000000 dask-expr-0.1.0/dask_expr/io/parquet.py
-drwxr-xr-x   0 patrick    (502) staff       (20)        0 2023-07-12 18:53:27.868968 dask-expr-0.1.0/dask_expr.egg-info/
--rw-r--r--   0 patrick    (502) staff       (20)     1963 2023-07-12 18:53:27.000000 dask-expr-0.1.0/dask_expr.egg-info/PKG-INFO
--rw-r--r--   0 patrick    (502) staff       (20)      651 2023-07-12 18:53:27.000000 dask-expr-0.1.0/dask_expr.egg-info/SOURCES.txt
--rw-r--r--   0 patrick    (502) staff       (20)        1 2023-07-12 18:53:27.000000 dask-expr-0.1.0/dask_expr.egg-info/dependency_links.txt
--rw-r--r--   0 patrick    (502) staff       (20)       32 2023-07-12 18:53:27.000000 dask-expr-0.1.0/dask_expr.egg-info/requires.txt
--rw-r--r--   0 patrick    (502) staff       (20)       10 2023-07-12 18:53:27.000000 dask-expr-0.1.0/dask_expr.egg-info/top_level.txt
--rw-r--r--   0 patrick    (502) staff       (20)     1538 2023-07-12 17:48:33.000000 dask-expr-0.1.0/pyproject.toml
--rw-r--r--   0 patrick    (502) staff       (20)      230 2023-07-12 18:53:27.870339 dask-expr-0.1.0/setup.cfg
--rwxr-xr-x   0 patrick    (502) staff       (20)      194 2023-07-12 17:44:05.000000 dask-expr-0.1.0/setup.py
--rw-r--r--   0 patrick    (502) staff       (20)    86677 2023-07-12 17:47:49.000000 dask-expr-0.1.0/versioneer.py
+drwxr-xr-x   0 patrick    (502) staff       (20)        0 2023-07-21 07:51:37.006375 dask-expr-0.1.1/
+-rw-r--r--   0 patrick    (502) staff       (20)     1516 2023-07-12 18:00:13.000000 dask-expr-0.1.1/LICENSE.txt
+-rw-r--r--   0 patrick    (502) staff       (20)     4456 2023-07-21 07:51:37.006429 dask-expr-0.1.1/PKG-INFO
+-rw-r--r--   0 patrick    (502) staff       (20)     3524 2023-07-21 07:49:20.000000 dask-expr-0.1.1/README.md
+drwxr-xr-x   0 patrick    (502) staff       (20)        0 2023-07-21 07:51:37.006761 dask-expr-0.1.1/dask_expr/
+-rw-r--r--   0 patrick    (502) staff       (20)      127 2023-07-12 17:51:26.000000 dask-expr-0.1.1/dask_expr/__init__.py
+-rw-r--r--   0 patrick    (502) staff       (20)     2603 2023-07-21 07:49:20.000000 dask-expr-0.1.1/dask_expr/_accessor.py
+-rw-r--r--   0 patrick    (502) staff       (20)     1434 2023-07-12 17:17:51.000000 dask-expr-0.1.1/dask_expr/_align.py
+-rw-r--r--   0 patrick    (502) staff       (20)     3683 2023-07-21 07:49:20.000000 dask-expr-0.1.1/dask_expr/_categorical.py
+-rw-r--r--   0 patrick    (502) staff       (20)    35504 2023-07-21 07:49:20.000000 dask-expr-0.1.1/dask_expr/_collection.py
+-rw-r--r--   0 patrick    (502) staff       (20)     4982 2023-07-12 17:17:51.000000 dask-expr-0.1.1/dask_expr/_concat.py
+-rw-r--r--   0 patrick    (502) staff       (20)    66800 2023-07-21 07:49:20.000000 dask-expr-0.1.1/dask_expr/_expr.py
+-rw-r--r--   0 patrick    (502) staff       (20)    15912 2023-07-12 17:17:51.000000 dask-expr-0.1.1/dask_expr/_groupby.py
+-rw-r--r--   0 patrick    (502) staff       (20)     9161 2023-07-12 17:17:51.000000 dask-expr-0.1.1/dask_expr/_merge.py
+-rw-r--r--   0 patrick    (502) staff       (20)     2169 2023-07-12 17:17:51.000000 dask-expr-0.1.1/dask_expr/_quantiles.py
+-rw-r--r--   0 patrick    (502) staff       (20)    18184 2023-07-21 07:49:20.000000 dask-expr-0.1.1/dask_expr/_reductions.py
+-rw-r--r--   0 patrick    (502) staff       (20)    11011 2023-07-12 17:17:51.000000 dask-expr-0.1.1/dask_expr/_repartition.py
+-rw-r--r--   0 patrick    (502) staff       (20)    27547 2023-07-21 07:49:20.000000 dask-expr-0.1.1/dask_expr/_shuffle.py
+-rw-r--r--   0 patrick    (502) staff       (20)      217 2023-06-27 15:57:00.000000 dask-expr-0.1.1/dask_expr/_typing.py
+-rw-r--r--   0 patrick    (502) staff       (20)      732 2023-07-21 07:49:20.000000 dask-expr-0.1.1/dask_expr/_util.py
+-rw-r--r--   0 patrick    (502) staff       (20)      497 2023-07-21 07:51:37.006795 dask-expr-0.1.1/dask_expr/_version.py
+-rw-r--r--   0 patrick    (502) staff       (20)     6228 2023-07-12 17:17:51.000000 dask-expr-0.1.1/dask_expr/datasets.py
+drwxr-xr-x   0 patrick    (502) staff       (20)        0 2023-07-21 07:51:37.006216 dask-expr-0.1.1/dask_expr/io/
+-rw-r--r--   0 patrick    (502) staff       (20)       96 2023-05-16 14:29:09.000000 dask-expr-0.1.1/dask_expr/io/__init__.py
+-rw-r--r--   0 patrick    (502) staff       (20)      980 2023-06-26 11:37:37.000000 dask-expr-0.1.1/dask_expr/io/csv.py
+-rw-r--r--   0 patrick    (502) staff       (20)     3068 2023-07-12 17:17:51.000000 dask-expr-0.1.1/dask_expr/io/io.py
+-rw-r--r--   0 patrick    (502) staff       (20)    33353 2023-07-21 07:49:20.000000 dask-expr-0.1.1/dask_expr/io/parquet.py
+drwxr-xr-x   0 patrick    (502) staff       (20)        0 2023-07-21 07:51:37.005365 dask-expr-0.1.1/dask_expr.egg-info/
+-rw-r--r--   0 patrick    (502) staff       (20)     4456 2023-07-21 07:51:36.000000 dask-expr-0.1.1/dask_expr.egg-info/PKG-INFO
+-rw-r--r--   0 patrick    (502) staff       (20)      700 2023-07-21 07:51:36.000000 dask-expr-0.1.1/dask_expr.egg-info/SOURCES.txt
+-rw-r--r--   0 patrick    (502) staff       (20)        1 2023-07-21 07:51:36.000000 dask-expr-0.1.1/dask_expr.egg-info/dependency_links.txt
+-rw-r--r--   0 patrick    (502) staff       (20)       32 2023-07-21 07:51:36.000000 dask-expr-0.1.1/dask_expr.egg-info/requires.txt
+-rw-r--r--   0 patrick    (502) staff       (20)       10 2023-07-21 07:51:36.000000 dask-expr-0.1.1/dask_expr.egg-info/top_level.txt
+-rw-r--r--   0 patrick    (502) staff       (20)     1615 2023-07-21 07:49:20.000000 dask-expr-0.1.1/pyproject.toml
+-rw-r--r--   0 patrick    (502) staff       (20)      230 2023-07-21 07:51:37.006650 dask-expr-0.1.1/setup.cfg
+-rwxr-xr-x   0 patrick    (502) staff       (20)      194 2023-07-12 17:44:05.000000 dask-expr-0.1.1/setup.py
+-rw-r--r--   0 patrick    (502) staff       (20)    86677 2023-07-12 17:47:49.000000 dask-expr-0.1.1/versioneer.py
```

### Comparing `dask-expr-0.1.0/LICENSE.txt` & `dask-expr-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dask-expr-0.1.0/dask_expr/_align.py` & `dask-expr-0.1.1/dask_expr/_align.py`

 * *Files identical despite different names*

### Comparing `dask-expr-0.1.0/dask_expr/_collection.py` & `dask-expr-0.1.1/dask_expr/_collection.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import warnings
 from collections.abc import Hashable
 from numbers import Number
 
 import numpy as np
 import pandas as pd
 from dask.base import DaskMethodsMixin, is_dask_collection, named_schedulers
+from dask.dataframe.accessor import CachedAccessor
 from dask.dataframe.core import (
     _concat,
     _Frame,
     check_divisions,
     is_dataframe_like,
     is_index_like,
     is_series_like,
@@ -20,14 +21,15 @@
 from dask.dataframe.dispatch import meta_nonempty
 from dask.utils import IndexCallable, random_state_data, typename
 from fsspec.utils import stringify_path
 from tlz import first
 
 from dask_expr import _expr as expr
 from dask_expr._align import AlignPartitions
+from dask_expr._categorical import CategoricalAccessor
 from dask_expr._concat import Concat
 from dask_expr._expr import Eval, no_default
 from dask_expr._merge import JoinRecursive, Merge
 from dask_expr._quantiles import RepartitionQuantiles
 from dask_expr._reductions import (
     DropDuplicates,
     Len,
@@ -143,16 +145,18 @@
 
     def simplify(self):
         return new_collection(self.expr.simplify())
 
     def lower_once(self):
         return new_collection(self.expr.lower_once())
 
-    def optimize(self, fuse: bool = True):
-        return new_collection(self.expr.optimize(fuse=fuse))
+    def optimize(self, combine_similar: bool = True, fuse: bool = True):
+        return new_collection(
+            self.expr.optimize(combine_similar=combine_similar, fuse=fuse)
+        )
 
     @property
     def dask(self):
         return self.__dask_graph__()
 
     def __dask_postcompute__(self):
         state = self.optimize(fuse=False)
@@ -430,14 +434,20 @@
 
     def sum(self, skipna=True, numeric_only=False, min_count=0):
         return new_collection(self.expr.sum(skipna, numeric_only, min_count))
 
     def prod(self, skipna=True, numeric_only=False, min_count=0):
         return new_collection(self.expr.prod(skipna, numeric_only, min_count))
 
+    def var(self, axis=0, skipna=True, ddof=1, numeric_only=False):
+        return new_collection(self.expr.var(axis, skipna, ddof, numeric_only))
+
+    def std(self, axis=0, skipna=True, ddof=1, numeric_only=False):
+        return new_collection(self.expr.std(axis, skipna, ddof, numeric_only))
+
     def mean(self, skipna=True, numeric_only=False, min_count=0):
         return new_collection(self.expr.mean(skipna, numeric_only))
 
     def max(self, skipna=True, numeric_only=False, min_count=0):
         return new_collection(self.expr.max(skipna, numeric_only, min_count))
 
     def any(self, skipna=True):
@@ -806,34 +816,56 @@
     def select_dtypes(self, include=None, exclude=None):
         columns = self._meta.select_dtypes(include=include, exclude=exclude).columns
         return new_collection(self.expr[columns])
 
     def eval(self, expr, **kwargs):
         return new_collection(Eval(self.expr, _expr=expr, expr_kwargs=kwargs))
 
-    def set_index(self, other, drop=True, sorted=False, divisions=None):
+    def set_index(
+        self,
+        other,
+        drop=True,
+        sorted=False,
+        npartitions: int | None = None,
+        divisions=None,
+        sort: bool = True,
+    ):
         if isinstance(other, DataFrame):
             raise TypeError("other can't be of type DataFrame")
         if isinstance(other, Series):
             if other._name == self.index._name:
                 return self
         elif other == self.index.name:
             return self
 
         if divisions is not None:
             check_divisions(divisions)
         other = other.expr if isinstance(other, Series) else other
 
+        if (sorted or not sort) and npartitions is not None:
+            raise ValueError(
+                "Specifying npartitions with sort=False or sorted=True is not "
+                "supported. Call `repartition` afterwards."
+            )
+
         if sorted:
             return new_collection(
                 SetIndexBlockwise(self.expr, other, drop, new_divisions=divisions)
             )
+        elif not sort:
+            return new_collection(SetIndexBlockwise(self.expr, other, drop, None))
 
         return new_collection(
-            SetIndex(self.expr, other, drop, user_divisions=divisions)
+            SetIndex(
+                self.expr,
+                other,
+                drop,
+                user_divisions=divisions,
+                npartitions=npartitions,
+            )
         )
 
 
 class Series(FrameBase):
     """Series-like Expr Collection"""
 
     def __dir__(self):
@@ -886,14 +918,16 @@
         return new_collection(
             expr.Between(self.expr, left=left, right=right, inclusive=inclusive)
         )
 
     def explode(self):
         return new_collection(expr.ExplodeSeries(self.expr))
 
+    cat = CachedAccessor("cat", CategoricalAccessor)
+
     def _repartition_quantiles(self, npartitions, upsample=1.0, random_state=None):
         return new_collection(
             RepartitionQuantiles(self.expr, npartitions, upsample, random_state)
         )
 
 
 class Index(Series):
@@ -967,18 +1001,20 @@
     """
     graph = ddf.dask
     if optimize:
         graph = ddf.__dask_optimize__(graph, ddf.__dask_keys__())
     return from_graph(graph, ddf._meta, ddf.divisions, ddf._name)
 
 
-def read_csv(*args, **kwargs):
+def read_csv(path, *args, **kwargs):
     from dask_expr.io.csv import ReadCSV
 
-    return new_collection(ReadCSV(*args, **kwargs))
+    if not isinstance(path, str):
+        path = stringify_path(path)
+    return new_collection(ReadCSV(path, *args, **kwargs))
 
 
 def read_parquet(
     path=None,
     columns=None,
     filters=None,
     categories=None,
@@ -993,15 +1029,15 @@
     aggregate_files=None,
     parquet_file_extension=(".parq", ".parquet", ".pq"),
     filesystem="fsspec",
     **kwargs,
 ):
     from dask_expr.io.parquet import ReadParquet
 
-    if hasattr(path, "name"):
+    if not isinstance(path, str):
         path = stringify_path(path)
 
     kwargs["dtype_backend"] = dtype_backend
 
     return new_collection(
         ReadParquet(
             path,
```

### Comparing `dask-expr-0.1.0/dask_expr/_concat.py` & `dask-expr-0.1.1/dask_expr/_concat.py`

 * *Files identical despite different names*

### Comparing `dask-expr-0.1.0/dask_expr/_expr.py` & `dask-expr-0.1.1/dask_expr/_expr.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,17 +4,18 @@
 import numbers
 import operator
 import os
 from collections import defaultdict
 from collections.abc import Generator, Mapping
 
 import dask
+import numpy as np
 import pandas as pd
 import toolz
-from dask.base import normalize_token, tokenize
+from dask.base import normalize_token
 from dask.core import flatten, ishashable
 from dask.dataframe import methods
 from dask.dataframe.core import (
     _get_divisions_map_partitions,
     _get_meta_map_partitions,
     apply_and_enforce,
     is_dataframe_like,
@@ -23,14 +24,16 @@
     make_meta,
 )
 from dask.dataframe.dispatch import meta_nonempty
 from dask.dataframe.utils import clear_known_categories, drop_by_shallow_copy
 from dask.utils import M, apply, funcname, import_required, is_arraylike
 from tlz import merge_sorted, unique
 
+from dask_expr._util import _tokenize_deterministic
+
 replacement_rules = []
 
 no_default = "__no_default__"
 
 
 class Expr:
     """Primary class for all Expressions
@@ -141,15 +144,21 @@
             # by existing methods/properties
             _parameters = type(self)._parameters
             if key in _parameters:
                 idx = _parameters.index(key)
                 return self.operands[idx]
             if is_dataframe_like(self._meta) and key in self._meta.columns:
                 return self[key]
-            raise err
+
+            link = "https://github.com/dask-contrib/dask-expr/blob/main/README.md#api-coverage"
+            raise AttributeError(
+                f"{err}\n\n"
+                "This often means that you are attempting to use an unsupported "
+                f"API function. Current API coverage is documented here: {link}."
+            )
 
     def operand(self, key):
         # Access an operand unambiguously
         # (e.g. if the key is reserved by a method/property)
         return self.operands[type(self)._parameters.index(key)]
 
     def dependencies(self):
@@ -303,14 +312,93 @@
             out = type(out)(*new_operands)
 
         return out
 
     def _lower(self):
         return
 
+    def combine_similar(
+        self, root: Expr | None = None, _cache: dict | None = None
+    ) -> Expr:
+        """Combine similar expression nodes using global information
+
+        This leverages the ``._combine_similar`` method defined
+        on each class. The global expression-tree traversal will
+        change IO leaves first, and finish with the root expression.
+        The primary purpose of this method is to allow column
+        projections to be "pushed back up" the expression graph
+        in the case that simlar IO & Blockwise operations can
+        be captured by the same operations.
+
+        Parameters
+        ----------
+        root:
+            The root node of the global expression graph. If not
+            specified, the root is assumed to be ``self``.
+        _cache:
+            Optional dictionary to use for caching.
+
+        Returns
+        -------
+        expr:
+            output expression
+        """
+        expr = self
+        update_root = root is None
+        root = root or self
+
+        if _cache is None:
+            _cache = {}
+        elif (self._name, root._name) in _cache:
+            return _cache[(self._name, root._name)]
+
+        while True:
+            changed = False
+
+            # Call combine_similar on each dependency
+            new_operands = []
+            changed_dependency = False
+            for operand in expr.operands:
+                if isinstance(operand, Expr):
+                    new = operand.combine_similar(root=root, _cache=_cache)
+                    if new._name != operand._name:
+                        changed_dependency = True
+                else:
+                    new = operand
+                new_operands.append(new)
+
+            if changed_dependency:
+                expr = type(expr)(*new_operands)
+                changed = True
+                if update_root:
+                    root = expr
+                continue
+
+            # Execute "_combine_similar" on expr
+            out = expr._combine_similar(root)
+            if out is None:
+                out = expr
+            if not isinstance(out, Expr):
+                _cache[(self._name, root._name)] = out
+                return out
+            if out._name != expr._name:
+                changed = True
+                expr = out
+                if update_root:
+                    root = expr
+
+            if not changed:
+                break
+
+        _cache[(self._name, root._name)] = expr
+        return expr
+
+    def _combine_similar(self, root: Expr):
+        return
+
     def optimize(self, **kwargs):
         return optimize(self, **kwargs)
 
     @property
     def index(self):
         return Index(self)
 
@@ -411,14 +499,25 @@
 
     def sum(self, skipna=True, numeric_only=False, min_count=0):
         return Sum(self, skipna, numeric_only, min_count)
 
     def prod(self, skipna=True, numeric_only=False, min_count=0):
         return Prod(self, skipna, numeric_only, min_count)
 
+    def var(self, axis=0, skipna=True, ddof=1, numeric_only=False):
+        if axis == 0:
+            return Var(self, skipna, ddof, numeric_only)
+        elif axis == 1:
+            return VarColumns(self, skipna, ddof, numeric_only)
+        else:
+            raise ValueError(f"axis={axis} not supported. Please specify 0 or 1")
+
+    def std(self, axis=0, skipna=True, ddof=1, numeric_only=False):
+        return Sqrt(self.var(axis, skipna, ddof, numeric_only))
+
     def mean(self, skipna=True, numeric_only=False, min_count=0):
         return Mean(self, skipna=skipna, numeric_only=numeric_only)
 
     def max(self, skipna=True, numeric_only=False, min_count=0):
         return Max(self, skipna, numeric_only, min_count)
 
     def any(self, skipna=True):
@@ -526,15 +625,17 @@
             idx = self._parameters.index("npartitions")
             return self.operands[idx]
         else:
             return len(self.divisions) - 1
 
     @functools.cached_property
     def _name(self):
-        return funcname(type(self)).lower() + "-" + tokenize(*self.operands)
+        return (
+            funcname(type(self)).lower() + "-" + _tokenize_deterministic(*self.operands)
+        )
 
     @property
     def columns(self) -> list:
         try:
             return list(self._meta.columns)
         except AttributeError:
             return []
@@ -608,14 +709,64 @@
             else:
                 new.append(operand)
 
         if update:  # Only recreate if something changed
             return type(self)(*new)
         return self
 
+    def substitute_parameters(self, substitutions: dict) -> Expr:
+        """Substitute specific `Expr` parameters
+
+        Parameters
+        ----------
+        substitutions:
+            Mapping of parameter keys to new values. Keys that
+            are not found in ``self._parameters`` will be ignored.
+        """
+        if not substitutions:
+            return self
+
+        changed = False
+        new_operands = []
+        for i, operand in enumerate(self.operands):
+            if i < len(self._parameters) and self._parameters[i] in substitutions:
+                new_operands.append(substitutions[self._parameters[i]])
+                changed = True
+            else:
+                new_operands.append(operand)
+        if changed:
+            return type(self)(*new_operands)
+        return self
+
+    def _find_similar_operations(self, root: Expr, ignore: list | None = None):
+        # Find operations with the same type and operands.
+        # Parameter keys specified by `ignore` will not be
+        # included in the operand comparison
+        alike = [
+            op for op in root.find_operations(type(self)) if op._name != self._name
+        ]
+        if not alike:
+            # No other operations of the same type. Early return
+            return []
+
+        def _tokenize(rp):
+            # Helper function to "tokenize" the operands
+            # that are not in the `ignore` list
+            return _tokenize_deterministic(
+                *[
+                    op
+                    for i, op in enumerate(rp.operands)
+                    if i >= len(rp._parameters) or rp._parameters[i] not in ignore
+                ]
+            )
+
+        # Return subset of `alike` with the same "token"
+        token = _tokenize(self)
+        return [item for item in alike if _tokenize(item) == token]
+
     def _node_label_args(self):
         """Operands to include in the node label by `visualize`"""
         return self.dependencies()
 
     def _to_graphviz(
         self,
         rankdir="BT",
@@ -832,15 +983,15 @@
 
     @functools.cached_property
     def _name(self):
         if self.operation:
             head = funcname(self.operation)
         else:
             head = funcname(type(self)).lower()
-        return head + "-" + tokenize(*self.operands)
+        return head + "-" + _tokenize_deterministic(*self.operands)
 
     def _blockwise_arg(self, arg, i):
         """Return a Blockwise-task argument"""
         if isinstance(arg, Expr):
             # Make key for Expr-based argument
             if self._broadcast_dep(arg):
                 return (arg._name, 0)
@@ -868,14 +1019,34 @@
         else:
             return (self.operation,) + tuple(args)
 
     def _simplify_up(self, parent):
         if self._projection_passthrough and isinstance(parent, Projection):
             return type(self)(self.frame[parent.operand("columns")], *self.operands[1:])
 
+    def _combine_similar(self, root: Expr):
+        # Push projections back up through `_projection_passthrough`
+        # operations if it reduces the number of unique expression nodes.
+        if self._projection_passthrough and isinstance(self.frame, Projection):
+            common = type(self)(self.frame.frame, *self.operands[1:])
+            projection = self.frame.operand("columns")
+            push_up_projection = False
+            for op in self._find_similar_operations(root, ignore=self._parameters):
+                if (
+                    isinstance(op.frame, Projection)
+                    and (
+                        common._name == type(op)(op.frame.frame, *op.operands[1:])._name
+                    )
+                ) or common._name == op._name:
+                    push_up_projection = True
+
+            if push_up_projection:
+                return common[projection]
+        return None
+
 
 class MapPartitions(Blockwise):
     _parameters = [
         "frame",
         "func",
         "meta",
         "enforce_metadata",
@@ -1064,14 +1235,30 @@
 class ToFrameIndex(Blockwise):
     _parameters = ["frame", "index", "name"]
     _defaults = {"name": no_default, "index": True}
     _keyword_only = ["name", "index"]
     operation = M.to_frame
 
 
+class VarColumns(Blockwise):
+    _parameters = ["frame", "skipna", "ddof", "numeric_only"]
+    _defaults = {"skipna": True, "ddof": 1, "numeric_only": False}
+    _keyword_only = ["skipna", "ddof", "numeric_only"]
+    operation = M.var
+
+    @functools.cached_property
+    def _kwargs(self) -> dict:
+        return {"axis": 1, **super()._kwargs}
+
+
+class Sqrt(Blockwise):
+    _parameters = ["frame"]
+    operation = np.sqrt
+
+
 class Elemwise(Blockwise):
     """
     This doesn't really do anything, but we anticipate that future
     optimizations, like `len` will care about which operations preserve length
     """
 
     pass
@@ -1720,19 +1907,15 @@
         elif isinstance(self.frame, PartitionsFiltered):
             if self.frame._partitions:
                 partitions = [self.frame._partitions[p] for p in self.partitions]
             else:
                 partitions = self.partitions
             # We assume that expressions defining a special "_partitions"
             # parameter can internally capture the same logic as `Partitions`
-            operands = [
-                partitions if self.frame._parameters[i] == "_partitions" else op
-                for i, op in enumerate(self.frame.operands)
-            ]
-            return type(self.frame)(*operands)
+            return self.frame.substitute_parameters({"_partitions": partitions})
 
     def _node_label_args(self):
         return [self.frame, self.partitions]
 
 
 class PartitionsFiltered(Expr):
     """Mixin class for partition filtering
@@ -1790,42 +1973,50 @@
 
 
 @normalize_token.register(Expr)
 def normalize_expression(expr):
     return expr._name
 
 
-def optimize(expr: Expr, fuse: bool = True) -> Expr:
+def optimize(expr: Expr, combine_similar: bool = True, fuse: bool = True) -> Expr:
     """High level query optimization
 
     This leverages three optimization passes:
 
     1.  Class based simplification using the ``_simplify`` function and methods
-    2.  Blockwise fusion
+    2.  Combine similar operations
+    3.  Blockwise fusion
 
     Parameters
     ----------
     expr:
         Input expression to optimize
+    combine_similar:
+        whether or not to combine similar operations
+        (like `ReadParquet`) to aggregate redundant work.
     fuse:
         whether or not to turn on blockwise fusion
 
     See Also
     --------
     simplify
+    combine_similar
     optimize_blockwise_fusion
     """
 
     result = expr
     while True:
         out = result.simplify().lower_once()
         if out._name == result._name:
             break
         result = out
 
+    if combine_similar:
+        result = result.combine_similar()
+
     if fuse:
         result = optimize_blockwise_fusion(result)
 
     return result
 
 
 def is_broadcastable(s):
@@ -2021,15 +2212,15 @@
         if len(names) > 3:
             names = [names[0], f"{len(names) - 2}", names[-1]]
         descr = "-".join(names)
         return f"Fused-{descr}"
 
     @functools.cached_property
     def _name(self):
-        return f"{str(self)}-{tokenize(self.exprs)}"
+        return f"{str(self)}-{_tokenize_deterministic(self.exprs)}"
 
     def _divisions(self):
         return self.exprs[0]._divisions()
 
     def _broadcast_dep(self, dep: Expr):
         # Always broadcast single-partition dependencies in Fused
         return dep.npartitions == 1
@@ -2071,9 +2262,10 @@
     Min,
     Mode,
     NBytes,
     NuniqueApprox,
     Prod,
     Size,
     Sum,
+    Var,
 )
 from dask_expr.io import IO, BlockwiseIO
```

### Comparing `dask-expr-0.1.0/dask_expr/_groupby.py` & `dask-expr-0.1.1/dask_expr/_groupby.py`

 * *Files identical despite different names*

### Comparing `dask-expr-0.1.0/dask_expr/_merge.py` & `dask-expr-0.1.1/dask_expr/_merge.py`

 * *Files identical despite different names*

### Comparing `dask-expr-0.1.0/dask_expr/_quantiles.py` & `dask-expr-0.1.1/dask_expr/_quantiles.py`

 * *Files identical despite different names*

### Comparing `dask-expr-0.1.0/dask_expr/_reductions.py` & `dask-expr-0.1.1/dask_expr/_reductions.py`

 * *Files 6% similar despite different names*

```diff
@@ -384,14 +384,75 @@
 
 class NBytes(Reduction):
     # Only supported for Series objects
     reduction_chunk = lambda ser: ser.nbytes
     reduction_aggregate = sum
 
 
+class Var(Reduction):
+    # Uses the parallel version of Welford's online algorithm (Chan 79')
+    # (http://i.stanford.edu/pub/cstr/reports/cs/tr/79/773/CS-TR-79-773.pdf)
+    _parameters = ["frame", "skipna", "ddof", "numeric_only"]
+    _defaults = {"skipna": True, "ddof": 1, "numeric_only": False}
+
+    @property
+    def _meta(self):
+        return make_meta(
+            meta_nonempty(self.frame._meta).var(
+                skipna=self.skipna, numeric_only=self.numeric_only
+            )
+        )
+
+    @property
+    def chunk_kwargs(self):
+        return dict(skipna=self.skipna, numeric_only=self.numeric_only)
+
+    @property
+    def combine_kwargs(self):
+        return {}
+
+    @property
+    def aggregate_kwargs(self):
+        return dict(ddof=self.ddof)
+
+    @classmethod
+    def reduction_chunk(cls, x, skipna=True, numeric_only=False):
+        kwargs = {"numeric_only": numeric_only} if is_dataframe_like(x) else {}
+        if skipna:
+            n = x.count(**kwargs)
+            kwargs["skipna"] = skipna
+            avg = x.mean(**kwargs)
+        else:
+            # Not skipping nulls, so might as well
+            # avoid the full `count` operation
+            n = len(x)
+            kwargs["skipna"] = skipna
+            avg = x.sum(**kwargs) / n
+        m2 = ((x - avg) ** 2).sum(**kwargs)
+        return n, avg, m2
+
+    @classmethod
+    def reduction_combine(cls, parts):
+        n, avg, m2 = parts[0]
+        for i in range(1, len(parts)):
+            n_a, avg_a, m2_a = n, avg, m2
+            n_b, avg_b, m2_b = parts[i]
+            n = n_a + n_b
+            avg = (n_a * avg_a + n_b * avg_b) / n
+            delta = avg_b - avg_a
+            m2 = m2_a + m2_b + delta**2 * n_a * n_b / n
+        return n, avg, m2
+
+    @classmethod
+    def reduction_aggregate(cls, vals, ddof=1):
+        vals = cls.reduction_combine(vals)
+        n, _, m2 = vals
+        return m2 / (n - ddof)
+
+
 class Mean(Reduction):
     _parameters = ["frame", "skipna", "numeric_only"]
     _defaults = {"skipna": True, "numeric_only": False}
 
     @property
     def _meta(self):
         return (
```

### Comparing `dask-expr-0.1.0/dask_expr/_repartition.py` & `dask-expr-0.1.1/dask_expr/_repartition.py`

 * *Files identical despite different names*

### Comparing `dask-expr-0.1.0/dask_expr/_shuffle.py` & `dask-expr-0.1.1/dask_expr/_shuffle.py`

 * *Files 1% similar despite different names*

```diff
@@ -641,33 +641,41 @@
     _parameters = [
         "frame",
         "_other",
         "drop",
         "user_divisions",
         "partition_size",
         "ascending",
+        "npartitions",
     ]
     _defaults = {
         "drop": True,
         "user_divisions": None,
         "partition_size": 128e6,
         "ascending": True,
+        "npartitions": None,
     }
 
     def _divisions(self):
         if self.user_divisions is not None:
             return self.user_divisions
         divisions, mins, maxes, presorted = _calculate_divisions(
-            self.frame, self.other, self.ascending
+            self.frame, self.other, self.npartitions, self.ascending
         )
         if presorted:
             divisions = mins.copy() + [maxes[-1]]
         return divisions
 
     @property
+    def npartitions(self):
+        if self.operand("npartitions") is not None:
+            return self.operand("npartitions")
+        return self.frame.npartitions
+
+    @property
     def _meta(self):
         if isinstance(self._other, Expr):
             other = self._other._meta
         else:
             other = self._other
         return self.frame._meta.set_index(other, drop=self.drop)
 
@@ -676,17 +684,19 @@
         if isinstance(self._other, Expr):
             return self._other
         return self.frame[self._other]
 
     def _lower(self):
         if self.user_divisions is None:
             divisions = self._divisions()
-            presorted = _calculate_divisions(self.frame, self.other, self.ascending)[3]
+            presorted = _calculate_divisions(
+                self.frame, self.other, self.npartitions, self.ascending
+            )[3]
 
-            if presorted:
+            if presorted and self.npartitions == self.frame.npartitions:
                 index_set = SetIndexBlockwise(
                     self.frame, self._other, self.drop, divisions
                 )
                 return SortIndexBlockwise(index_set)
 
         else:
             divisions = self.user_divisions
@@ -802,20 +812,24 @@
                 type(self)(self.frame[columns], *self.operands[1:]),
                 parent.operand("columns"),
             )
 
 
 @functools.lru_cache  # noqa: B019
 def _calculate_divisions(
-    frame, other, ascending: bool = True, partition_size: float = 128e6
+    frame,
+    other,
+    npartitions: int,
+    ascending: bool = True,
+    partition_size: float = 128e6,
 ):
     from dask_expr import RepartitionQuantiles, new_collection
 
     divisions, mins, maxes = compute(
-        new_collection(RepartitionQuantiles(other, frame.npartitions)),
+        new_collection(RepartitionQuantiles(other, npartitions)),
         new_collection(other).map_partitions(M.min),
         new_collection(other).map_partitions(M.max),
     )
     sizes = []
 
     empty_dataframe_detected = pd.isna(divisions).all()
     if empty_dataframe_detected:
```

### Comparing `dask-expr-0.1.0/dask_expr/datasets.py` & `dask-expr-0.1.1/dask_expr/datasets.py`

 * *Files identical despite different names*

### Comparing `dask-expr-0.1.0/dask_expr/io/csv.py` & `dask-expr-0.1.1/dask_expr/io/csv.py`

 * *Files identical despite different names*

### Comparing `dask-expr-0.1.0/dask_expr/io/io.py` & `dask-expr-0.1.1/dask_expr/io/io.py`

 * *Files identical despite different names*

### Comparing `dask-expr-0.1.0/dask_expr/io/parquet.py` & `dask-expr-0.1.1/dask_expr/io/parquet.py`

 * *Files 3% similar despite different names*

```diff
@@ -423,31 +423,65 @@
     def columns(self):
         columns_operand = self.operand("columns")
         if columns_operand is None:
             return list(self._meta.columns)
         else:
             return _convert_to_list(columns_operand)
 
+    def _combine_similar(self, root: Expr):
+        # For ReadParquet, we can avoid redundant file-system
+        # access by aggregating multiple operations with different
+        # column projections into the same operation.
+        alike = self._find_similar_operations(root, ignore=["columns", "_series"])
+        if alike:
+            # We have other ReadParquet operations in the expression
+            # graph that can be combined with this one.
+
+            # Find the column-projection union needed to combine
+            # the qualified ReadParquet operations
+            columns = set()
+            rps = [self] + alike
+            for rp in rps:
+                if rp.operand("columns"):
+                    columns |= set(rp.operand("columns"))
+            columns = sorted(columns)
+
+            # Can bail if we are not changing columns or the "_series" operand
+            columns_operand = self.operand("columns")
+            if columns_operand == columns and (len(columns) > 1 or not self._series):
+                return
+
+            # Check if we have the operation we want elsewhere in the graph
+            for rp in rps:
+                if rp.operand("columns") == columns and not rp.operand("_series"):
+                    return (
+                        rp[columns_operand[0]] if self._series else rp[columns_operand]
+                    )
+
+            # Create the "combined" ReadParquet operation
+            subs = {"columns": columns}
+            if self._series:
+                subs["_series"] = False
+            new = self.substitute_parameters(subs)
+            return new[columns_operand[0]] if self._series else new[columns_operand]
+
+        return
+
     def _simplify_up(self, parent):
         if isinstance(parent, Index):
             # Column projection
-            operands = list(self.operands)
-            operands[self._parameters.index("columns")] = []
-            operands[self._parameters.index("_series")] = False
-            return ReadParquet(*operands)
+            return self.substitute_parameters({"columns": [], "_series": False})
 
         if isinstance(parent, Projection):
             # Column projection
-            operands = list(self.operands)
-            operands[self._parameters.index("columns")] = _convert_to_list(
-                parent.operand("columns")
-            )
-            if isinstance(parent.operand("columns"), (str, int)):
-                operands[self._parameters.index("_series")] = True
-            return ReadParquet(*operands)
+            parent_columns = parent.operand("columns")
+            substitutions = {"columns": _convert_to_list(parent_columns)}
+            if isinstance(parent_columns, (str, int)):
+                substitutions["_series"] = True
+            return self.substitute_parameters(substitutions)
 
         if isinstance(parent, Filter) and isinstance(
             parent.predicate, (LE, GE, LT, GT, EQ, NE, And, Or)
         ):
             # Predicate pushdown
             filters = _DNF.extract_pq_filters(self, parent.predicate)
             if filters:
```

### Comparing `dask-expr-0.1.0/dask_expr.egg-info/SOURCES.txt` & `dask-expr-0.1.1/dask_expr.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 LICENSE.txt
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 versioneer.py
 dask_expr/__init__.py
+dask_expr/_accessor.py
 dask_expr/_align.py
+dask_expr/_categorical.py
 dask_expr/_collection.py
 dask_expr/_concat.py
 dask_expr/_expr.py
 dask_expr/_groupby.py
 dask_expr/_merge.py
 dask_expr/_quantiles.py
 dask_expr/_reductions.py
```

### Comparing `dask-expr-0.1.0/pyproject.toml` & `dask-expr-0.1.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -28,14 +28,17 @@
     "dask >= 2023.07",
     "pyarrow",
     "pandas >= 2",
 ]
 
 dynamic = ["version"]
 
+[project.urls]
+"Source code" = "https://github.com/dask-contrib/dask-expr/"
+
 [tool.setuptools.packages.find]
 exclude = ["*tests*"]
 namespaces = false
 
 [tool.coverage.run]
 omit = [
     "*/test_*.py",
```

### Comparing `dask-expr-0.1.0/versioneer.py` & `dask-expr-0.1.1/versioneer.py`

 * *Files identical despite different names*

