# Comparing `tmp/xdeps-0.2.0.tar.gz` & `tmp/xdeps-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xdeps-0.2.0.tar", last modified: Mon Jun 26 16:13:31 2023, max compression
+gzip compressed data, was "xdeps-0.3.0.tar", last modified: Fri Jul 21 09:06:10 2023, max compression
```

## Comparing `xdeps-0.2.0.tar` & `xdeps-0.3.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 giadarol   (503) staff       (20)        0 2023-06-26 16:13:31.411731 xdeps-0.2.0/
--rw-r--r--   0 giadarol   (503) staff       (20)    11356 2023-03-23 11:04:37.000000 xdeps-0.2.0/LICENSE
--rw-r--r--   0 giadarol   (503) staff       (20)      559 2023-06-26 16:13:31.411519 xdeps-0.2.0/PKG-INFO
--rw-r--r--   0 giadarol   (503) staff       (20)       38 2023-06-26 16:13:31.411786 xdeps-0.2.0/setup.cfg
--rw-r--r--   0 giadarol   (503) staff       (20)     1253 2023-03-23 11:04:37.000000 xdeps-0.2.0/setup.py
-drwxr-xr-x   0 giadarol   (503) staff       (20)        0 2023-06-26 16:13:31.403930 xdeps-0.2.0/xdeps/
--rw-r--r--   0 giadarol   (503) staff       (20)      462 2023-06-26 16:12:34.000000 xdeps-0.2.0/xdeps/__init__.py
--rw-r--r--   0 giadarol   (503) staff       (20)       22 2023-06-26 16:12:56.000000 xdeps-0.2.0/xdeps/_version.py
--rw-r--r--   0 giadarol   (503) staff       (20)      397 2023-06-26 16:12:34.000000 xdeps-0.2.0/xdeps/functions.py
--rw-r--r--   0 giadarol   (503) staff       (20)      160 2023-05-30 19:18:47.000000 xdeps-0.2.0/xdeps/general.py
--rw-r--r--   0 giadarol   (503) staff       (20)     5506 2023-04-05 12:43:31.000000 xdeps-0.2.0/xdeps/madxutils.py
-drwxr-xr-x   0 giadarol   (503) staff       (20)        0 2023-06-26 16:13:31.411055 xdeps-0.2.0/xdeps/optimize/
--rw-r--r--   0 giadarol   (503) staff       (20)      118 2023-05-30 19:18:47.000000 xdeps-0.2.0/xdeps/optimize/__init__.py
--rw-r--r--   0 giadarol   (503) staff       (20)     3511 2023-05-30 19:18:47.000000 xdeps-0.2.0/xdeps/optimize/jacobian.py
--rw-r--r--   0 giadarol   (503) staff       (20)    11173 2023-05-30 19:18:47.000000 xdeps-0.2.0/xdeps/optimize/optimize.py
--rw-r--r--   0 giadarol   (503) staff       (20)    22746 2023-06-26 16:12:34.000000 xdeps-0.2.0/xdeps/refs.py
--rw-r--r--   0 giadarol   (503) staff       (20)     2093 2023-04-05 12:43:31.000000 xdeps-0.2.0/xdeps/sorting.py
--rw-r--r--   0 giadarol   (503) staff       (20)    16572 2023-06-06 14:39:09.000000 xdeps-0.2.0/xdeps/table.py
--rw-r--r--   0 giadarol   (503) staff       (20)    15105 2023-06-26 16:12:34.000000 xdeps-0.2.0/xdeps/tasks.py
--rw-r--r--   0 giadarol   (503) staff       (20)      932 2023-04-05 12:43:31.000000 xdeps-0.2.0/xdeps/utils.py
-drwxr-xr-x   0 giadarol   (503) staff       (20)        0 2023-06-26 16:13:31.407640 xdeps-0.2.0/xdeps.egg-info/
--rw-r--r--   0 giadarol   (503) staff       (20)      559 2023-06-26 16:13:31.000000 xdeps-0.2.0/xdeps.egg-info/PKG-INFO
--rw-r--r--   0 giadarol   (503) staff       (20)      408 2023-06-26 16:13:31.000000 xdeps-0.2.0/xdeps.egg-info/SOURCES.txt
--rw-r--r--   0 giadarol   (503) staff       (20)        1 2023-06-26 16:13:31.000000 xdeps-0.2.0/xdeps.egg-info/dependency_links.txt
--rw-r--r--   0 giadarol   (503) staff       (20)       21 2023-06-26 16:13:31.000000 xdeps-0.2.0/xdeps.egg-info/requires.txt
--rw-r--r--   0 giadarol   (503) staff       (20)        6 2023-06-26 16:13:31.000000 xdeps-0.2.0/xdeps.egg-info/top_level.txt
+drwxr-xr-x   0 giadarol   (503) staff       (20)        0 2023-07-21 09:06:10.734949 xdeps-0.3.0/
+-rw-r--r--   0 giadarol   (503) staff       (20)    11356 2023-03-23 11:04:37.000000 xdeps-0.3.0/LICENSE
+-rw-r--r--   0 giadarol   (503) staff       (20)      559 2023-07-21 09:06:10.734765 xdeps-0.3.0/PKG-INFO
+-rw-r--r--   0 giadarol   (503) staff       (20)       38 2023-07-21 09:06:10.735002 xdeps-0.3.0/setup.cfg
+-rw-r--r--   0 giadarol   (503) staff       (20)     1253 2023-03-23 11:04:37.000000 xdeps-0.3.0/setup.py
+drwxr-xr-x   0 giadarol   (503) staff       (20)        0 2023-07-21 09:06:10.732429 xdeps-0.3.0/xdeps/
+-rw-r--r--   0 giadarol   (503) staff       (20)      462 2023-06-26 16:12:34.000000 xdeps-0.3.0/xdeps/__init__.py
+-rw-r--r--   0 giadarol   (503) staff       (20)       22 2023-07-21 09:05:43.000000 xdeps-0.3.0/xdeps/_version.py
+-rw-r--r--   0 giadarol   (503) staff       (20)      397 2023-06-26 16:12:34.000000 xdeps-0.3.0/xdeps/functions.py
+-rw-r--r--   0 giadarol   (503) staff       (20)      160 2023-05-30 19:18:47.000000 xdeps-0.3.0/xdeps/general.py
+-rw-r--r--   0 giadarol   (503) staff       (20)     5506 2023-04-05 12:43:31.000000 xdeps-0.3.0/xdeps/madxutils.py
+drwxr-xr-x   0 giadarol   (503) staff       (20)        0 2023-07-21 09:06:10.734520 xdeps-0.3.0/xdeps/optimize/
+-rw-r--r--   0 giadarol   (503) staff       (20)      118 2023-05-30 19:18:47.000000 xdeps-0.3.0/xdeps/optimize/__init__.py
+-rw-r--r--   0 giadarol   (503) staff       (20)     5338 2023-07-21 09:05:08.000000 xdeps-0.3.0/xdeps/optimize/jacobian.py
+-rw-r--r--   0 giadarol   (503) staff       (20)    20024 2023-07-21 09:05:08.000000 xdeps-0.3.0/xdeps/optimize/optimize.py
+-rw-r--r--   0 giadarol   (503) staff       (20)    23045 2023-07-21 09:05:08.000000 xdeps-0.3.0/xdeps/refs.py
+-rw-r--r--   0 giadarol   (503) staff       (20)     2093 2023-04-05 12:43:31.000000 xdeps-0.3.0/xdeps/sorting.py
+-rw-r--r--   0 giadarol   (503) staff       (20)    16863 2023-07-21 09:05:08.000000 xdeps-0.3.0/xdeps/table.py
+-rw-r--r--   0 giadarol   (503) staff       (20)    15128 2023-07-21 09:05:08.000000 xdeps-0.3.0/xdeps/tasks.py
+-rw-r--r--   0 giadarol   (503) staff       (20)      932 2023-04-05 12:43:31.000000 xdeps-0.3.0/xdeps/utils.py
+drwxr-xr-x   0 giadarol   (503) staff       (20)        0 2023-07-21 09:06:10.733711 xdeps-0.3.0/xdeps.egg-info/
+-rw-r--r--   0 giadarol   (503) staff       (20)      559 2023-07-21 09:06:10.000000 xdeps-0.3.0/xdeps.egg-info/PKG-INFO
+-rw-r--r--   0 giadarol   (503) staff       (20)      408 2023-07-21 09:06:10.000000 xdeps-0.3.0/xdeps.egg-info/SOURCES.txt
+-rw-r--r--   0 giadarol   (503) staff       (20)        1 2023-07-21 09:06:10.000000 xdeps-0.3.0/xdeps.egg-info/dependency_links.txt
+-rw-r--r--   0 giadarol   (503) staff       (20)       21 2023-07-21 09:06:10.000000 xdeps-0.3.0/xdeps.egg-info/requires.txt
+-rw-r--r--   0 giadarol   (503) staff       (20)        6 2023-07-21 09:06:10.000000 xdeps-0.3.0/xdeps.egg-info/top_level.txt
```

### Comparing `xdeps-0.2.0/LICENSE` & `xdeps-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xdeps-0.2.0/PKG-INFO` & `xdeps-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xdeps
-Version: 0.2.0
+Version: 0.3.0
 Summary: Data dependency manager
 Home-page: https://xsuite.readthedocs.io/
 Download-URL: https://pypi.python.org/pypi/xdeps
 Author: Riccardo De Maria
 Author-email: riccardo.de.maria@cern.ch
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/xsuite/xsuite/issues
```

### Comparing `xdeps-0.2.0/setup.py` & `xdeps-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `xdeps-0.2.0/xdeps/madxutils.py` & `xdeps-0.3.0/xdeps/madxutils.py`

 * *Files identical despite different names*

### Comparing `xdeps-0.2.0/xdeps/refs.py` & `xdeps-0.3.0/xdeps/refs.py`

 * *Files 1% similar despite different names*

```diff
@@ -333,14 +333,15 @@
     def _expr(self):
         if self in self._manager.tasks:
             task = self._manager.tasks[self]
             if hasattr(task, "expr"):
                 return task.expr
 
     def _info(self, limit=10):
+
         print(f"#  {self}._get_value()")
         try:
             value = self._get_value()
             print(f"   {self} = {value}")
         except:
             print(f"#  {self} has no value")
         print()
@@ -353,24 +354,25 @@
             if hasattr(task, "info"):
                 task.info()
         else:
             print(f"#  {self}._expr is None")
             print()
 
         refs = self._manager.find_deps([self])[1:]
+        limit = (limit or len(refs))
         if len(refs) == 0:
             print(f"#  {self} does not influence any target")
             print()
         else:
             print(f"#  {self}._find_dependant_targets()")
             for tt in refs[:limit]:
                 if tt._expr is not None:
                     print(f"   {tt}")
             if len(refs) > limit:
-                print(f"   ... set _info(limit={len(refs)}) to get all lines")
+                print(f"   ... set _info(limit=None) to get all lines")
             print()
 
     def __iadd__(self, other):
         newexpr = self._expr
         if newexpr:
             return newexpr + other
         else:
@@ -655,15 +657,19 @@
     # def __setstate__(self, state):
     #     object.__setattr__(self, "_a", state[0])
     #     object.__setattr__(self, "_b", state[1])
 
     def _get_value(self):
         a = ARef._mk_value(self._a)
         b = ARef._mk_value(self._b)
-        return self._op(a, b)
+        try:
+            ret = self._op(a, b)
+        except ZeroDivisionError:
+            ret = float("nan")
+        return ret
 
     def _get_dependencies(self, out=None):
         a = self._a
         b = self._b
         if out is None:
             out = set()
         if isinstance(a, ARef):
@@ -777,25 +783,25 @@
         if isinstance(self._func, ARef):
             fname = repr(self._func)
         else:
             fname = self._func.__name__
         return f"{fname}({args})"
 
 
-class RefList:
+class RefContainer:
     """
     A list implementation that does not use __eq__ for comparisons. It is used
     for storing tasks, which need to be compared by their hash, as the usual
     == operator yields an expression, which is always True.
     """
     def __init__(self, *args, **kwargs):
-        self.list = list(*args, **kwargs)
+        self.list = set(list(*args, **kwargs))
 
     def __repr__(self):
-        return f"RefList({self.list})"
+        return f"RefContainer({self.list})"
 
     def __contains__(self, item):
         try:
             self.index(item)
             return True
         except ValueError:
             return False
@@ -805,30 +811,36 @@
 
     def __delitem__(self, index):
         self.list.pop(index)
 
     def __iter__(self):
         return iter(self.list)
 
+    def __len__(self):
+        return len(self.list)
+
     def index(self, item):
         for ii, x in enumerate(self.list):
             if hash(item) == hash(x):
                 return ii
         raise ValueError(f'{item} is not in list')
 
     def extend(self, other):
-        if isinstance(other, RefList):
+        if isinstance(other, RefContainer):
             other = other.list
-        self.list.extend(other)
+        #self.list.extend(other)
+        self.list.update(other)
 
     def append(self, item):
-        self.list.append(item)
+        #self.list.append(item)
+        self.list.add(item)
 
     def remove(self, item):
-        del self[self.index(item)]
+        #del self[self.index(item)]
+        self.list.remove(item)
 
 
 gbl = globals()
 for st, op in _binops.items():
     fn = op.__name__.replace("_", "")
     cn = f"{fn.capitalize()}Ref"
     mn = f"__{fn}__"
```

### Comparing `xdeps-0.2.0/xdeps/sorting.py` & `xdeps-0.3.0/xdeps/sorting.py`

 * *Files identical despite different names*

### Comparing `xdeps-0.2.0/xdeps/table.py` & `xdeps-0.3.0/xdeps/table.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 import pathlib
 import re
 import numpy as np
 
 gblmath = {"np": np}
 for k, fu in np.__dict__.items():
     if type(fu) is np.ufunc:
@@ -278,15 +279,15 @@
     def __getattr__(self, key):
         if key in self._data:
             return self._data[key]
         else:
             raise AttributeError(f"Cannot find `{key}` in table")
 
     def __len__(self):
-        return len(self._data)
+        return len(self._data[self._index])
 
     def keys(self, exclude_columns=False):
         if exclude_columns:
             return [kk for kk in self._data.keys() if kk not in self._col_names]
         return self._data.keys()
 
     def values(self):
@@ -435,15 +436,15 @@
             )  # table
 
     def show(
         self,
         rows=None,
         cols=None,
         maxrows=20,
-        maxwidth=80,
+        maxwidth='auto',
         output=None,
         digits=6,
         fixed="g",
         header=True,
     ):
         view, col_list = self._get_view_col_list(rows, cols)
 
@@ -453,14 +454,22 @@
         col_list.insert(0, self._index)
 
         cut = -1
         viewrows = len(view)
         if maxrows is not None and output is None and viewrows > maxrows:
             cut = maxrows // 2
 
+        if maxwidth == "auto":
+            try:
+                maxwidth = os.get_terminal_size().columns - 5
+                if maxwidth < 10 or maxwidth > 10000:
+                    raise Exception()
+            except Exception:
+                maxwidth = 100
+
         data = []
         width = 0
         # maxwidth=10000000 if maxwidth is None else maxwidth
         fmt = []
         header_line = []
         for cc in col_list:
             if cc in view:
```

### Comparing `xdeps-0.2.0/xdeps/tasks.py` & `xdeps-0.3.0/xdeps/tasks.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # ######################################### #
 
 from dataclasses import dataclass, field
 from collections import defaultdict
 import logging
 from copy import deepcopy
 
-from .refs import ARef, CallRef, Ref, ObjectAttrRef, RefList
+from .refs import ARef, CallRef, Ref, ObjectAttrRef, RefContainer
 from .utils import os_display_png, mpl_display_png, ipy_display_png
 from .utils import AttrDict
 from .sorting import toposort
 
 logger = logging.getLogger(__name__)
 
 
@@ -133,18 +133,18 @@
     tartasks: ref -> all tasks that has ref as target
     containers: label -> controlled container
     """
 
     def __init__(self):
         self.tasks = {}
         self.containers = {}
-        self.rdeps = defaultdict(RefList)
-        self.rtasks = defaultdict(RefList)
-        self.deptasks = defaultdict(RefList)
-        self.tartasks = defaultdict(RefList)
+        self.rdeps = defaultdict(RefContainer)
+        self.rtasks = defaultdict(RefContainer)
+        self.deptasks = defaultdict(RefContainer)
+        self.tartasks = defaultdict(RefContainer)
         self._tree_frozen = False
 
     def ref(self, container=None, label="_"):
         """Return a ref to an instance (or dict) associated to a label.
 
         Label must be unique.
         """
@@ -441,8 +441,8 @@
             odct = getattr(other, dct)
             sdct = getattr(self, dct)
             for kk, ss in list(sdct.items()):
                 if set(ss) != set(odct[kk]):
                     print(f"{dct}[{kk}] not consistent")
                     print(f"{dct}[{kk}] self - check:", set(ss) - set(odct[kk]))
                     print(f"{dct}[{kk}] check - self:", set(odct[kk]) - set(ss))
-                    # raise (ValueError(f"{self} is not consistent in {dct}[{kk}]"))
+                    raise (ValueError(f"{self} is not consistent in {dct}[{kk}]"))
```

### Comparing `xdeps-0.2.0/xdeps/utils.py` & `xdeps-0.3.0/xdeps/utils.py`

 * *Files identical despite different names*

### Comparing `xdeps-0.2.0/xdeps.egg-info/PKG-INFO` & `xdeps-0.3.0/xdeps.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xdeps
-Version: 0.2.0
+Version: 0.3.0
 Summary: Data dependency manager
 Home-page: https://xsuite.readthedocs.io/
 Download-URL: https://pypi.python.org/pypi/xdeps
 Author: Riccardo De Maria
 Author-email: riccardo.de.maria@cern.ch
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/xsuite/xsuite/issues
```

