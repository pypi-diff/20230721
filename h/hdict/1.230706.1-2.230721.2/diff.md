# Comparing `tmp/hdict-1.230706.1.tar.gz` & `tmp/hdict-2.230721.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hdict-1.230706.1.tar", max compression
+gzip compressed data, was "hdict-2.230721.2.tar", max compression
```

## Comparing `hdict-1.230706.1.tar` & `hdict-2.230721.2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0    35149 2022-12-26 01:24:40.000000 hdict-1.230706.1/LICENSE
--rw-r--r--   0        0        0     7696 2023-07-06 23:25:53.275010 hdict-1.230706.1/README.md
--rw-r--r--   0        0        0     1385 2023-07-06 23:26:54.439029 hdict-1.230706.1/pyproject.toml
--rw-r--r--   0        0        0    15595 2023-07-06 23:14:52.886751 hdict-1.230706.1/src/hdict/__init__.py
--rw-r--r--   0        0        0      223 2023-07-06 17:42:16.967118 hdict-1.230706.1/src/hdict/abs/__init__.py
--rw-r--r--   0        0        0        0 2023-07-06 17:42:16.967118 hdict-1.230706.1/src/hdict/content/__init__.py
--rw-r--r--   0        0        0      755 2023-07-06 17:42:16.967118 hdict-1.230706.1/src/hdict/content/argument/__init__.py
--rw-r--r--   0        0        0    14478 2023-07-06 23:19:47.382880 hdict-1.230706.1/src/hdict/content/argument/apply.py
--rw-r--r--   0        0        0     3242 2023-07-06 22:11:28.034640 hdict-1.230706.1/src/hdict/content/argument/aux_apply.py
--rw-r--r--   0        0        0     1483 2023-07-06 17:42:16.967118 hdict-1.230706.1/src/hdict/content/argument/default.py
--rw-r--r--   0        0        0     1318 2023-07-06 17:42:16.967118 hdict-1.230706.1/src/hdict/content/argument/entry.py
--rw-r--r--   0        0        0     2162 2023-07-06 23:15:22.758765 hdict-1.230706.1/src/hdict/content/argument/field.py
--rw-r--r--   0        0        0     2330 2023-07-06 22:17:01.298525 hdict-1.230706.1/src/hdict/content/argument/sample.py
--rw-r--r--   0        0        0     3967 2023-07-06 22:34:49.954302 hdict-1.230706.1/src/hdict/content/aux_value.py
--rw-r--r--   0        0        0     2011 2023-07-06 17:42:16.967118 hdict-1.230706.1/src/hdict/content/entry/__init__.py
--rw-r--r--   0        0        0     1965 2023-07-06 17:42:16.967118 hdict-1.230706.1/src/hdict/content/entry/aux_closure.py
--rw-r--r--   0        0        0     1346 2023-07-06 17:42:16.967118 hdict-1.230706.1/src/hdict/content/entry/cached.py
--rw-r--r--   0        0        0     4378 2023-07-06 17:42:16.967118 hdict-1.230706.1/src/hdict/content/entry/closure.py
--rw-r--r--   0        0        0     2835 2023-07-06 17:42:16.967118 hdict-1.230706.1/src/hdict/content/entry/subvalue.py
--rw-r--r--   0        0        0      541 2023-07-06 17:42:16.967118 hdict-1.230706.1/src/hdict/content/entry/wrapper.py
--rw-r--r--   0        0        0     2254 2023-07-06 22:53:17.646321 hdict-1.230706.1/src/hdict/content/value.py
--rw-r--r--   0        0        0        0 2023-07-06 17:42:16.967118 hdict-1.230706.1/src/hdict/data/__init__.py
--rw-r--r--   0        0        0    10149 2023-07-06 23:16:22.646793 hdict-1.230706.1/src/hdict/data/aux_frozendict.py
--rw-r--r--   0        0        0     2211 2023-07-06 17:42:16.967118 hdict-1.230706.1/src/hdict/data/empty_.py
--rw-r--r--   0        0        0    21144 2023-07-06 23:19:47.554880 hdict-1.230706.1/src/hdict/data/frozenhdict.py
--rw-r--r--   0        0        0    24195 2023-07-06 23:20:34.062898 hdict-1.230706.1/src/hdict/data/hdict_.py
--rw-r--r--   0        0        0        0 2023-07-06 17:42:16.967118 hdict-1.230706.1/src/hdict/dataset/__init__.py
--rw-r--r--   0        0        0     8333 2023-07-06 23:23:02.878954 hdict-1.230706.1/src/hdict/dataset/dataset.py
--rw-r--r--   0        0        0     4465 2023-07-06 23:23:48.782970 hdict-1.230706.1/src/hdict/dataset/pandas_handling.py
--rw-r--r--   0        0        0        0 2023-07-06 17:42:16.967118 hdict-1.230706.1/src/hdict/expression/__init__.py
--rw-r--r--   0        0        0     3543 2023-07-06 17:42:16.967118 hdict-1.230706.1/src/hdict/expression/expr.py
--rw-r--r--   0        0        0        0 2023-07-06 17:42:16.967118 hdict-1.230706.1/src/hdict/expression/step/__init__.py
--rw-r--r--   0        0        0     2280 2023-07-06 23:24:29.266983 hdict-1.230706.1/src/hdict/expression/step/applyout.py
--rw-r--r--   0        0        0     2529 2023-07-06 23:19:24.594871 hdict-1.230706.1/src/hdict/expression/step/cache.py
--rw-r--r--   0        0        0      395 2023-07-06 17:42:16.967118 hdict-1.230706.1/src/hdict/expression/step/edict.py
--rw-r--r--   0        0        0     2198 2023-07-06 17:42:16.967118 hdict-1.230706.1/src/hdict/expression/step/step.py
--rw-r--r--   0        0        0        0 2023-07-06 17:42:16.967118 hdict-1.230706.1/src/hdict/persistence/__init__.py
--rw-r--r--   0        0        0     1223 2023-07-06 17:42:16.967118 hdict-1.230706.1/src/hdict/persistence/stored.py
--rw-r--r--   0        0        0        0 2023-07-06 17:42:16.967118 hdict-1.230706.1/src/hdict/text/__init__.py
--rw-r--r--   0        0        0     7525 2023-07-06 23:19:47.262880 hdict-1.230706.1/src/hdict/text/customjson.py
--rw-r--r--   0        0        0     9232 1970-01-01 00:00:00.000000 hdict-1.230706.1/setup.py
--rw-r--r--   0        0        0     8740 1970-01-01 00:00:00.000000 hdict-1.230706.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-12-26 01:24:40.000000 hdict-2.230721.2/LICENSE
+-rw-r--r--   0        0        0     7754 2023-07-21 03:27:09.441173 hdict-2.230721.2/README.md
+-rw-r--r--   0        0        0     1412 2023-07-21 03:27:16.545177 hdict-2.230721.2/pyproject.toml
+-rw-r--r--   0        0        0    15681 2023-07-21 00:53:01.312195 hdict-2.230721.2/src/hdict/__init__.py
+-rw-r--r--   0        0        0      223 2023-07-06 17:42:16.967118 hdict-2.230721.2/src/hdict/abs/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-06 17:42:16.967118 hdict-2.230721.2/src/hdict/content/__init__.py
+-rw-r--r--   0        0        0      757 2023-07-21 01:08:50.956711 hdict-2.230721.2/src/hdict/content/argument/__init__.py
+-rw-r--r--   0        0        0    14982 2023-07-21 02:13:49.898820 hdict-2.230721.2/src/hdict/content/argument/apply.py
+-rw-r--r--   0        0        0     3323 2023-07-21 02:23:42.487137 hdict-2.230721.2/src/hdict/content/argument/aux_apply.py
+-rw-r--r--   0        0        0     1483 2023-07-06 17:42:16.967118 hdict-2.230721.2/src/hdict/content/argument/default.py
+-rw-r--r--   0        0        0     1318 2023-07-06 17:42:16.967118 hdict-2.230721.2/src/hdict/content/argument/entry.py
+-rw-r--r--   0        0        0     2163 2023-07-21 00:26:28.439317 hdict-2.230721.2/src/hdict/content/argument/field.py
+-rw-r--r--   0        0        0     2330 2023-07-06 22:17:01.298525 hdict-2.230721.2/src/hdict/content/argument/sample.py
+-rw-r--r--   0        0        0     3967 2023-07-06 22:34:49.954302 hdict-2.230721.2/src/hdict/content/aux_value.py
+-rw-r--r--   0        0        0     2037 2023-07-21 02:00:13.958384 hdict-2.230721.2/src/hdict/content/entry/__init__.py
+-rw-r--r--   0        0        0     2033 2023-07-21 02:34:04.199469 hdict-2.230721.2/src/hdict/content/entry/aux_closure.py
+-rw-r--r--   0        0        0     1346 2023-07-06 17:42:16.967118 hdict-2.230721.2/src/hdict/content/entry/cached.py
+-rw-r--r--   0        0        0     4478 2023-07-21 01:48:03.097990 hdict-2.230721.2/src/hdict/content/entry/closure.py
+-rw-r--r--   0        0        0     2835 2023-07-06 17:42:16.967118 hdict-2.230721.2/src/hdict/content/entry/subvalue.py
+-rw-r--r--   0        0        0      541 2023-07-06 17:42:16.967118 hdict-2.230721.2/src/hdict/content/entry/wrapper.py
+-rw-r--r--   0        0        0     2254 2023-07-06 22:53:17.646321 hdict-2.230721.2/src/hdict/content/value.py
+-rw-r--r--   0        0        0        0 2023-07-06 17:42:16.967118 hdict-2.230721.2/src/hdict/data/__init__.py
+-rw-r--r--   0        0        0    10587 2023-07-21 03:21:52.653003 hdict-2.230721.2/src/hdict/data/aux_frozendict.py
+-rw-r--r--   0        0        0     1995 2023-07-21 01:29:06.329372 hdict-2.230721.2/src/hdict/data/empty_.py
+-rw-r--r--   0        0        0    21056 2023-07-21 03:21:52.797003 hdict-2.230721.2/src/hdict/data/frozenhdict.py
+-rw-r--r--   0        0        0    25770 2023-07-21 02:21:05.263053 hdict-2.230721.2/src/hdict/data/hdict_.py
+-rw-r--r--   0        0        0     3432 2023-07-21 02:23:42.415137 hdict-2.230721.2/src/hdict/data/self_.py
+-rw-r--r--   0        0        0        0 2023-07-06 17:42:16.967118 hdict-2.230721.2/src/hdict/dataset/__init__.py
+-rw-r--r--   0        0        0     8333 2023-07-06 23:23:02.878954 hdict-2.230721.2/src/hdict/dataset/dataset.py
+-rw-r--r--   0        0        0     4465 2023-07-06 23:23:48.782970 hdict-2.230721.2/src/hdict/dataset/pandas_handling.py
+-rw-r--r--   0        0        0        0 2023-07-06 17:42:16.967118 hdict-2.230721.2/src/hdict/expression/__init__.py
+-rw-r--r--   0        0        0     3543 2023-07-06 17:42:16.967118 hdict-2.230721.2/src/hdict/expression/expr.py
+-rw-r--r--   0        0        0        0 2023-07-06 17:42:16.967118 hdict-2.230721.2/src/hdict/expression/step/__init__.py
+-rw-r--r--   0        0        0     2280 2023-07-06 23:24:29.266983 hdict-2.230721.2/src/hdict/expression/step/applyout.py
+-rw-r--r--   0        0        0     2529 2023-07-06 23:19:24.594871 hdict-2.230721.2/src/hdict/expression/step/cache.py
+-rw-r--r--   0        0        0      395 2023-07-06 17:42:16.967118 hdict-2.230721.2/src/hdict/expression/step/edict.py
+-rw-r--r--   0        0        0     2198 2023-07-06 17:42:16.967118 hdict-2.230721.2/src/hdict/expression/step/step.py
+-rw-r--r--   0        0        0        0 2023-07-06 17:42:16.967118 hdict-2.230721.2/src/hdict/persistence/__init__.py
+-rw-r--r--   0        0        0     1223 2023-07-06 17:42:16.967118 hdict-2.230721.2/src/hdict/persistence/stored.py
+-rw-r--r--   0        0        0        0 2023-07-06 17:42:16.967118 hdict-2.230721.2/src/hdict/text/__init__.py
+-rw-r--r--   0        0        0     7525 2023-07-06 23:19:47.262880 hdict-2.230721.2/src/hdict/text/customjson.py
+-rw-r--r--   0        0        0     8798 1970-01-01 00:00:00.000000 hdict-2.230721.2/PKG-INFO
```

### Comparing `hdict-1.230706.1/LICENSE` & `hdict-2.230721.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hdict-1.230706.1/README.md` & `hdict-2.230721.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 [![license: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 
 <!--- [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5501845.svg)](https://doi.org/10.5281/zenodo.5501845) --->
 [![arXiv](https://img.shields.io/badge/arXiv-2109.06028-b31b1b.svg?style=flat-square)](https://arxiv.org/abs/2109.06028)
 [![API documentation](https://img.shields.io/badge/API-autogenerated-a030a0.svg)](https://davips.github.io/hdict)
 [![Manual](https://img.shields.io/badge/manual-handcrafted-a030a0.svg)](https://hosh.page)
 [![Downloads](https://static.pepy.tech/badge/hdict)](https://pepy.tech/project/hdict)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/hdict)
 
 # hdict { A _unique_ data structure }
 [Website](https://hosh.page) | 
 [Latest Release](https://pypi.org/project/hdict) |
 [Current Code](https://github.com/davips/hdict) |
 [API Documentation](https://davips.github.io/hdict)
```

#### html2text {}

```diff
@@ -4,21 +4,22 @@
 badge/python-3.10+-blue.svg) [![license: GPL v3](https://img.shields.io/badge/
 License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)  [![arXiv]
 (https://img.shields.io/badge/arXiv-2109.06028-b31b1b.svg?style=flat-square)]
 (https://arxiv.org/abs/2109.06028) [![API documentation](https://
 img.shields.io/badge/API-autogenerated-a030a0.svg)](https://davips.github.io/
 hdict) [![Manual](https://img.shields.io/badge/manual-handcrafted-a030a0.svg)]
 (https://hosh.page) [![Downloads](https://static.pepy.tech/badge/hdict)](https:
-//pepy.tech/project/hdict) # hdict { A _unique_ data structure } [Website]
-(https://hosh.page) | [Latest Release](https://pypi.org/project/hdict) |
-[Current Code](https://github.com/davips/hdict) | [API Documentation](https://
-davips.github.io/hdict) Please see the [website](https://hosh.page) for more
-detailed usage information. ## Overview Shortly, `hdict` is a data structure
-useful for frictionless experiments, distributed data, among others. It can be
-more formally defined as a hoshÂ¹-based cacheable lazy `dict` with predictable/
+//pepy.tech/project/hdict) ![PyPI - Downloads](https://img.shields.io/pypi/dm/
+hdict) # hdict { A _unique_ data structure } [Website](https://hosh.page) |
+[Latest Release](https://pypi.org/project/hdict) | [Current Code](https://
+github.com/davips/hdict) | [API Documentation](https://davips.github.io/hdict)
+Please see the [website](https://hosh.page) for more detailed usage
+information. ## Overview Shortly, `hdict` is a data structure useful for
+frictionless experiments, distributed data, among others. It can be more
+formally defined as a hoshÂ¹-based cacheable lazy `dict` with predictable/
 deterministic universally uniqueÂ² identifiers. This library is stable for the
 most common scenarios. However, we will wait for more use in the wild before
 reaching the major version 1. See the Section Versioning below for more
 information. Â¹ hosh: _Operable HaSH_ Â² unique: _probabilistically guaranteed_
 ### Context * [hosh](https://pypi.org/project/hosh): identification engine at
 the core of `hdict` * previous projects: [hoshmap](https://pypi.org/project/
 hoshmap), [idict](https://pypi.org/project/idict), [ldict](https://pypi.org/
```

### Comparing `hdict-1.230706.1/pyproject.toml` & `hdict-2.230721.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hdict"
-version = "1.230706.1"
+version = "2.230721.2"
 description = "A versatile dictionary based on a novel paradigm useful for computing, caching, experiments, distributed data, among others."
 authors = ["davips <dpsabc@gmail.com>"]
 license = "GPLv3"
 readme = "README.md"
 packages = [
     { include = "hdict", from = "src" }
 ]
@@ -37,11 +37,12 @@
 ipython = "^8.9.0"
 pandas = "^2.0.0"
 shelchemy = "^0.220906.5"
 safeserializer = "^0.230202.1"
 lz4 = "^4.3.2"
 scikit-learn = "^1.2.2"
 liac-arff = "^2.5.0"
+pycrunch-engine = "^1.5.2"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `hdict-1.230706.1/src/hdict/__init__.py` & `hdict-2.230721.2/src/hdict/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 from hdict.content.argument.apply import apply
 from hdict.content.argument.field import field
 from hdict.content.argument.sample import sample
 from hdict.data.empty_ import Empty_
 from hdict.content.value import value
 from hdict.data.frozenhdict import frozenhdict
 from hdict.data.hdict_ import hdict_
+from hdict.data.self_ import Self_
 from hdict.expression.step.cache import cache
 
 __all__ = ["hdict", "_", "Ø", "apply", "field", "sample", "frozenhdict", "value", "cache"]
 
 VT = TypeVar("VT")
 
 
@@ -170,16 +171,16 @@
     >>> d >>= apply(field("f"), field("x"), y=default(3))("w", "v")
     >>> d["w2", "v2"] = apply(field("f"), field("x"), y=default(3))
     >>> d >>= {"z": apply(f, field("x"), y=3), ("w", "v"): apply(g, y=7)}
     >>> d >>= apply(f, field("x"), y=3)("z9") * apply(g, y=7)("w9", "v9")
     >>> pp = apply(f, field("x"), y=3)("z") >> apply(g, y=7)("w", "v")
     >>> d >>= {"x": 3} >> pp >> apply(g, y=7)("w", "v")
     >>> from hdict import _
-    >>> a1 = apply(f, y=_[1, 2, 4, ..., 128])
-    >>> a2 = apply(f, _[0, 3, 6, ..., 9], y=_[0, 3, 6, ..., 9])
+    >>> a1 = apply(f, y=_(1, 2, 4, ..., 128))
+    >>> a2 = apply(f, _(0, 3, 6, ..., 9), y=_(0, 3, 6, ..., 9))
     >>> ppp = hdict() >> a2.sample()("k", "t")
     >>> ppp.show(colored=False)
     {
         k: λ(9 9)→0,
         t: λ(9 9)→1,
         _id: dK-iumb4L5nkFVT9LCkdk3daQtuC.ORk6JwWMhnt,
         _ids: {
@@ -191,15 +192,15 @@
     387420489
     >>> a1("z")
     z=λ(x y=~[1 2 .*. 128])
     >>> a2(w="a", v="b")
     (('w', 'a'), ('v', 'b'))=λ(x=~[0 3 .+. 9] y=~[0 3 .+. 9])
     >>> p = a1("z") >> a2(w="a", v="b")
     >>> h = lambda a, b=4: 5
-    >>> app = apply(h, a=_[0, 3, 6, ..., 9])
+    >>> app = apply(h, a=_(0, 3, 6, ..., 9))
     >>> app
     λ(a=~[0 3 .+. 9] b=default(4))
     >>> app.c
     c=λ(a=~[0 3 .+. 9] b=default(4))
     >>> sampled = app.sample(0).c
     >>> sampled
     c=λ(9 b=default(4))
@@ -226,16 +227,16 @@
     >>> d["w"]
     10
     >>> d >>= p1
     >>> d["z"] = apply(f, 2, y=3)
     >>> d["w", "v"] = apply(f, _.x, y=_.x)
     >>> d["w", "v"] = apply(_.f, _.x, y=default(3))
     >>> d = hdict() >> {"z": apply(f, 7, y=3), ("w", "v"): apply(g, default(6), y=7)}
-    >>> d = hdict(w=6) >> (apply(f, _.w, y=3)(z="z") >> apply(g, x=_[1,2,3,...,5], y=7)("ww", "v")).sample(0)
-    >>> p = apply(f, y=_[1, 2, 4, ..., 128])("z") >> apply(f, y=_[0, 3, 6, ..., 9])(w="a", v="b")
+    >>> d = hdict(w=6) >> (apply(f, _["w"], y=3)(z="z") >> apply(g, x=_(1,2,3,...,5), y=7)("ww", "v")).sample(0)
+    >>> p = apply(f, y=_(1, 2, 4, ..., 128))("z") >> apply(f, y=_(0, 3, 6, ..., 9))(w="a", v="b")
     >>> d.show(colored=False)
     {
         w: 6,
         z: λ(x=w 3)→z,
         ww: λ(4 7)→0,
         v: λ(4 7)→1,
         _id: x4TxaVuAymsh97Yr.15Oc1ekllvlpECk091124RM,
@@ -449,23 +450,28 @@
     """
 
 
 class Empty(Empty_):
     """
     >>> from hdict import _
     >>> d = _ >> {"x": 5} >> dict(y=7)
-    >>> type(_), type(d)
+    >>> type(+_), type(d)
     (<class 'hdict.Empty'>, <class 'hdict.hdict'>)
     >>> d.show(colored=False)
     {
         x: 5,
         y: 7,
         _id: A0G3Y7KNMLihDvpSJ3tB.zxshc6u1CbbiiYjCAAA,
         _ids: {
             x: ecvgo-CBPi7wRWIxNzuo1HgHQCbdvR058xi6zmr2,
             y: eJCW9jGsdZTD6-AD9opKwjPIOWZ4R.T0CG2kdyzf
         }
     }
     """
 
 
-Ø = _ = Empty()
+class Self(Self_):
+    """"""
+
+
+Ø = empty = Empty()
+_ = Self()
```

### Comparing `hdict-1.230706.1/src/hdict/content/argument/__init__.py` & `hdict-2.230721.2/src/hdict/content/argument/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 
 class AbsBaseArgument(AbsArgument):
     """
     Normal function argument provided by the user: `value`*, `field`, `apply`; or from advanced use: `entry`
 
     Exceptionally, 'field' is a subclass that can also be piped through '>>'
-    *value also inherits AbsReadyEntry
+    *value also inherits AbsBaseArgument
     """
 
 
 class AbsMetaArgument(AbsArgument):
     """
     Special temporary argument-like directive provided by the user: `default`, `sample`
     """
```

### Comparing `hdict-1.230706.1/src/hdict/content/argument/apply.py` & `hdict-2.230721.2/src/hdict/content/argument/apply.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,14 +32,27 @@
 from hdict.content.argument import AbsBaseArgument, AbsArgument
 from hdict.content.argument.field import field
 from hdict.text.customjson import truncate
 from hdict.content.aux_value import f2hosh
 
 
 def getattr_(__o: object, name: str, __default=None):
+    """
+    >>> from hdict import _, apply
+    >>> (_ >> {"o": "str"} >> apply(getattr, _.o, "find").r).evaluated.show(colored=False)  # doctest:+ELLIPSIS
+    {
+        o: "str",
+        r: "<built-in method find of str object at 0x...>",
+        _id: zU3QsJ.a9fjr8eeoqwaPKlufC6.AEacZZBWScM39,
+        _ids: {
+            o: PdHGvI1xk.ZG7wt3-2TQm-GjFXidwYNw8xsD3Wpe,
+            r: BKrY9O9ExQh8k0xjgINKKV2-JD6qEEjDOIVR1yyq
+        }
+    }
+    """
     return getattr(__o, name, __default)
 
 
 # todo hide unneeded attrs to avoid poluting namespace for output field
 class apply(AbsBaseArgument):
     """
     Function application
@@ -55,38 +68,38 @@
     >>> g = lambda x, y: x**y
     >>> apply(g, y=value(7777), x=v)
     λ(x=λ(5 7) 7777)
 
     >>> v2 = apply(f, a=v, b=value(7))
     >>> v2
     λ(a=λ(5 7) 7)
-    >>> v.enclosure({}, "j").value
+    >>> v.enclosure({}, "j", None).value
     78125
-    >>> v2.enclosure({}, "j")
+    >>> v2.enclosure({}, "j", None)
     λ(a=λ(5 7) 7)
-    >>> v2.enclosure({}, "j").value
+    >>> v2.enclosure({}, "j", None).value
     17763568394002504646778106689453125
 
     >>> f = lambda a,b, c=1,d=2,e=13: 0
     >>> apply(f).requirements
     {'a': field(a), 'b': field(b), 'c': default(1), 'd': default(2), 'e': default(13)}
     >>> ap = apply(f,3)
     >>> ap.requirements
     {'a': 3, 'b': field(b), 'c': default(1), 'd': default(2), 'e': default(13)}
     >>> ap
     λ(3 b c=default(1) d=default(2) e=default(13))
-    >>> ap.enclosure({"b": value(77)}, "j")
+    >>> ap.enclosure({"b": value(77)}, "j", None)
     λ(3 b c=1 d=2 e=13)
     >>> ap
     λ(3 b c=default(1) d=default(2) e=default(13))
     >>> d = {"f": ap, "b": 5, "d": 1, "e": field("b")}
     >>> d
     {'f': λ(3 b c=default(1) d=default(2) e=default(13)), 'b': 5, 'd': 1, 'e': field(b)}
     >>> from hdict.data.aux_frozendict import handle_items
-    >>> handle_items(d, previous={"b": 5})
+    >>> handle_items(d, previous=frozenhdict({"b": 5}))
     {'b': 5, 'f': λ(3 b c=1 d=2 e=13), 'd': 1, 'e': 5}
     >>> d
     {'f': λ(3 b c=default(1) d=default(2) e=default(13)), 'b': 5, 'd': 1, 'e': field(b)}
     >>> apply(f,3,4).requirements
     {'a': 3, 'b': 4, 'c': default(1), 'd': default(2), 'e': default(13)}
     >>> apply(f,3,4,5).requirements
     {'a': 3, 'b': 4, 'c': 5, 'd': default(2), 'e': default(13)}
@@ -312,18 +325,18 @@
         clone = self.clone(_sampleable=False)
         for k, v in clone.fargs.items():
             clone.fargs[k] = v.sample(rnd)
         for k, v in clone.fkwargs.items():
             clone.fkwargs[k] = v.sample(rnd)
         return clone
 
-    def enclosure(self, data, key):
+    def enclosure(self, data, key, previous):
         from hdict.content.entry.closure import Closure
 
-        return Closure(self, data, [key])
+        return Closure(self, data, [key], previous)
 
     def __call__(self, *out, **kwout):
         from hdict.expression.step.applyout import ApplyOut
 
         if not (out or kwout):  # pragma: no cover
             raise Exception(f"At least one output field must be specified to apply.")
```

### Comparing `hdict-1.230706.1/src/hdict/content/argument/aux_apply.py` & `hdict-2.230721.2/src/hdict/content/argument/aux_apply.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,19 @@
     """
 
     def __repr__(self):
         return repr(dict(self.items()))
 
 
 class Arg(str):
+    """
+    >>> Arg("a") >= Arg("a")
+    True
+    """
+
     def __init__(self, position: int):
         self.position = position
 
     def __hash__(self):
         return hash(self.position)
 
     def __lt__(self, other):
@@ -46,18 +51,19 @@
             fargs[i] = v
             params.append(i)
         for k, v in applied_kwargs.items():
             fkwargs[k] = v
             params.append(k)
     else:
         for par in signature.parameters.values():
-            if str(par).startswith("**"):
+            strpar = str(par)
+            if strpar.startswith("**"):
                 haskwargs = True
                 continue
-            elif str(par).startswith("*"):
+            elif strpar.startswith("*"):
                 hasargs = True
                 continue
             name = par.name
             if (v := par.default) is par.empty:
                 fargs[name] = field(name)
             else:
                 from hdict.content.argument.default import default
```

### Comparing `hdict-1.230706.1/src/hdict/content/argument/default.py` & `hdict-2.230721.2/src/hdict/content/argument/default.py`

 * *Files identical despite different names*

### Comparing `hdict-1.230706.1/src/hdict/content/argument/entry.py` & `hdict-2.230721.2/src/hdict/content/argument/entry.py`

 * *Files identical despite different names*

### Comparing `hdict-1.230706.1/src/hdict/content/argument/field.py` & `hdict-2.230721.2/src/hdict/content/argument/field.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     >>> from hdict import Ø, _, apply
     >>> d = Ø
     >>> d.show(colored=False)
     {
         _id: 0000000000000000000000000000000000000000,
         _ids: {}
     }
-    >>> d = _
+    >>> d = +_
     >>> d.show(colored=False)
     {
         _id: 0000000000000000000000000000000000000000,
         _ids: {}
     }
     >>> d >>= {"x": 3, "y": 5} >> apply(lambda x, y: x + y).z
     >>> d.show(colored=False)
```

### Comparing `hdict-1.230706.1/src/hdict/content/argument/sample.py` & `hdict-2.230721.2/src/hdict/content/argument/sample.py`

 * *Files identical despite different names*

### Comparing `hdict-1.230706.1/src/hdict/content/aux_value.py` & `hdict-2.230721.2/src/hdict/content/aux_value.py`

 * *Files identical despite different names*

### Comparing `hdict-1.230706.1/src/hdict/content/entry/__init__.py` & `hdict-2.230721.2/src/hdict/content/entry/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -50,13 +50,13 @@
 
     def evaluate(self):
         _ = self.value
 
     @property
     def isevaluated(self):
         """
-        >>> from hdict import apply
+        >>> from hdict import apply, frozenhdict
         >>> from hdict.content.entry.closure import Closure
-        >>> Closure(apply(lambda x, y: x + y), {"x": 3, "y": 5}, []).isevaluated
+        >>> Closure(apply(lambda x, y: x + y), {"x": 3, "y": 5}, [], frozenhdict).isevaluated
         False
         """
         return not isinstance(self._value, Unevaluated)
```

### Comparing `hdict-1.230706.1/src/hdict/content/entry/aux_closure.py` & `hdict-2.230721.2/src/hdict/content/entry/aux_closure.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,48 +1,49 @@
 from __future__ import annotations
 
 from hdict.content.argument import AbsBaseArgument
 
 
-def handle_arg(key, val, data, discarded_defaults, out, torepr):
+def handle_arg(key, val, data, discarded_defaults, out, torepr, previous):
     """Return handled arg and value of pseudocircular entry"""
     from hdict.content.argument.default import default
     from hdict.content.value import value
     from hdict.data.aux_frozendict import handle_item
     from hdict import field
     from hdict.data.aux_frozendict import MissingFieldException
 
     from hdict.content.argument.entry import entry
-    from hdict.content.entry.subvalue import SubValue
 
+    if key == "_":
+        return handle_item(str(key), previous, data, previous)
     match val:
         case default(value=v):
             if key in data:
                 arg = data[key]
                 # REMINDER: `discarded_defaults` exists only for __repr__ purposes
                 discarded_defaults.add(key)
             else:
                 arg = value(v)
             if key in out:
                 torepr[key] = arg
                 return arg
         case field(name=name) if name in out:  # Override case of handle_item if pseudocircular reference.
             if name not in data:  # pragma: no cover
                 raise MissingFieldException(f"Missing pseudocircular field `{name}`")
-            arg = handle_item(str(key), data[name], data)  # key passed for no purpose here AFAIR
+            arg = handle_item(str(key), data[name], data, previous)  # key passed for no purpose here AFAIR
             torepr[key] = arg
             return arg
         case entry(name=name):
             from hdict.content.entry.wrapper import Wrapper
 
             if name not in data:  # pragma: no cover
                 raise MissingFieldException(f"Missing pseudocircular field `{name}`")
-            content = handle_item(str(key), data[name], data)
+            content = handle_item(str(key), data[name], data, previous)
             arg = Wrapper(content)
             torepr[f"·{name}"] = arg
             return arg
         case AbsBaseArgument():
-            arg = handle_item(str(key), val, data)
+            arg = handle_item(str(key), val, data, previous)
         case _:  # pragma: no cover
             raise Exception(f"Cannot handle argument of type `{type(val).__name__}`")
     torepr[key] = val
     return arg
```

### Comparing `hdict-1.230706.1/src/hdict/content/entry/cached.py` & `hdict-2.230721.2/src/hdict/content/entry/cached.py`

 * *Files identical despite different names*

### Comparing `hdict-1.230706.1/src/hdict/content/entry/closure.py` & `hdict-2.230721.2/src/hdict/content/entry/closure.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,45 +1,46 @@
 from __future__ import annotations
 
 from itertools import chain
 
+from hdict.data.frozenhdict import frozenhdict
 from hosh import ø
 
 from hdict.content.argument import AbsArgument
 from hdict.content.argument.apply import apply
 from hdict.content.argument.default import default
 from hdict.content.entry import AbsEntry, Unevaluated
 from hdict.content.entry.aux_closure import handle_arg
 from hdict.text.customjson import truncate
 
 
 class Closure(AbsEntry):
-    def __init__(self, application: apply, data: dict[str, AbsEntry], out: list):
+    def __init__(self, application: apply, data: dict[str, AbsEntry], out: list, previous: frozenhdict):
         from hdict.data.aux_frozendict import handle_item
 
         self.application = application
         self.out = out
         self.torepr = {}
         hosh = ø
         arg = None
         fargs, fkwargs, discarded_defaults = application.fargs.copy(), {}, set()  # We copy fargs to keep args order.
         sortable_fargs = zip(map(str, fargs), fargs.items())
         for idx, tup in sorted(chain(sortable_fargs, application.fkwargs.items())):  # We sort by keys for a deterministic hosh.
             if isinstance(tup, tuple):
                 key, val = tup
-                arg = handle_arg(key, val, data, discarded_defaults, out, self.torepr)
+                arg = handle_arg(key, val, data, discarded_defaults, out, self.torepr, previous)
                 fargs[key] = arg
             else:
                 key, val = idx, tup
-                arg = handle_arg(key, val, data, discarded_defaults, out, self.torepr)
+                arg = handle_arg(key, val, data, discarded_defaults, out, self.torepr, previous)
                 fkwargs[key] = arg
             hosh *= arg.hosh
 
         if application.isfield:
-            appliable_entry = handle_item(application.appliable.name, application.appliable, data)
+            appliable_entry = handle_item(application.appliable.name, application.appliable, data, previous)
             hosh *= appliable_entry.hosh.rev
 
             def f():
                 args = (x.value for x in fargs.values())
                 kwargs = {k: v.value for k, v in fkwargs.items()}
                 try:
                     return appliable_entry.value(*args, **kwargs)
```

### Comparing `hdict-1.230706.1/src/hdict/content/entry/subvalue.py` & `hdict-2.230721.2/src/hdict/content/entry/subvalue.py`

 * *Files identical despite different names*

### Comparing `hdict-1.230706.1/src/hdict/content/entry/wrapper.py` & `hdict-2.230721.2/src/hdict/content/entry/wrapper.py`

 * *Files identical despite different names*

### Comparing `hdict-1.230706.1/src/hdict/content/value.py` & `hdict-2.230721.2/src/hdict/content/value.py`

 * *Files identical despite different names*

### Comparing `hdict-1.230706.1/src/hdict/data/aux_frozendict.py` & `hdict-2.230721.2/src/hdict/data/aux_frozendict.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from itertools import chain
 from typing import Dict
 from typing import TypeVar
 
 from hosh import ø
 
-from hdict import hdict, value, frozenhdict
+from hdict import hdict, value, frozenhdict, Self
 from hdict.abs import AbsAny
 from hdict.content.argument.apply import apply
 from hdict.content.argument.field import field
 from hdict.content.argument.sample import sample
 from hdict.content.entry import AbsEntry
 from hdict.content.entry.closure import Closure
 from hdict.dataset.dataset import df2Xy
@@ -17,73 +17,77 @@
 VT = TypeVar("VT")
 
 
 class MissingFieldException(Exception):
     pass
 
 
-def handle_items(*datas: [Dict[str, object]], previous: [Dict[str, AbsEntry]]):
-    result = previous.copy()
+def handle_items(*datas: [Dict[str, object]], previous: frozenhdict):
+    result = {} if previous is None else previous.raw.copy()
     result__mirror_fields = {}
     for key, item in chain(*(data.items() for data in datas)):
-        entry = handle_item(key, item, result)
+        entry = handle_item(key, item, result, previous)
         if isinstance(key, str) and key.endswith("_"):
             if isinstance(entry, value):
                 result__mirror_fields[f"{key[:-1]}"] = value(entry.hdict, entry.hdict.hosh)
             else:
                 raise Exception(f"lazy mirror?")  # todo:
         if isinstance(entry, dict):
             result.update(entry)
         else:
             result[key] = entry
     result.update(result__mirror_fields)
     return result
 
 
-def handle_item(key, item, previous):
+def handle_item(key, item, result, previous):
     from hdict.content.argument.entry import entry
 
     match item:
         case AbsEntry():
             res = item
         case field(name=name):
-            if name not in previous:  # pragma: no cover
+            if name not in result:  # pragma: no cover
                 raise MissingFieldException(f"Missing field `{name}`")
-            res = handle_item(name, previous[name], previous)
+            res = handle_item(name, result[name], result, previous)
         case entry(name=name):
             from hdict.content.entry.wrapper import Wrapper
 
-            if name not in previous:  # pragma: no cover
+            if name not in result:  # pragma: no cover
                 raise MissingFieldException(f"Missing entry `{name}`")
-            res = Wrapper(handle_item(name, previous[name], previous))
+            res = Wrapper(handle_item(name, result[name], result, previous))
         case apply():
-            res = item.enclosure(previous, key)
+            res = item.enclosure(result, key, previous)
         case sample():  # pragma: no cover
             raise Exception(f"Unsampled variable or argument `{key}`")
         case frozenhdict():
             res = value(item, item.hosh)
         case hdict():
             res = value(item.frozen, item.hosh)
         case ApplyOut():  # pragma: no cover
             raise Exception("Cannot assign output through both apply and dict-key: '>> {out: apply(...)(out)}'.")
+        case Self():
+            if previous is None:
+                raise Exception(f"Cannot reference self in a new hdict. `_` is intended to point to a hdict before application.")
+            res = handle_item(key, previous, result, None)
         case AbsAny():  # pragma: no cover
             raise Exception(f"Cannot handle instance of type '{type(item).__name__}'.")
         case _ if str(type(item)) == "<class 'pandas.core.frame.DataFrame'>":
             from hdict.dataset.pandas_handling import explode_df
 
             # todo: check if this is the best default way of handling DFs.
             df = item.copy(deep=False)
             d = explode_df(df)
             df.__dict__["ashdict"] = d
             res = value(df, hosh=d.hosh.rev, hdict=d)
         case _:
             res = value(item)
 
     if isinstance(key, tuple):
-        return handle_multioutput(key, res, previous)
+        return handle_multioutput(key, res, result, previous)
     elif not isinstance(key, str):  # pragma: no cover
         raise Exception(f"Invalid type for input field specification: {type(key).__name__}")
     # elif key.startswith("_"):  # pragma: no cover     # reminder: _* allowed here due to parameter name in getattr(__o)
     #     raise Exception(f"Field names cannot start with '_': {key}")
 
     return res
 
@@ -107,44 +111,44 @@
         #   E.g.: hash(field name X) != hash(string "X")
         #   In this impementation, the difference is always* true because values are always pickled (they are never hashed as strings), while identifiers are just str.encoded().
         #   * → probabilistically
     ids.update(later)
     return hosh, ids
 
 
-def handle_multioutput(field_names: tuple, entry: AbsEntry | apply, previous):
+def handle_multioutput(field_names: tuple, entry: AbsEntry | apply, previous_result, previous):
     """Fields and hoshes are assigned to each output according to the alphabetical order of the original keys.
 
     >>> from hdict import field, value
     >>> d = {"a": field("b"), "b": field("c"), "c": 5}
     >>> d
     {'a': field(b), 'b': field(c), 'c': 5}
-    >>> handle_multioutput(("x","y"), value([0, 1]), d)
+    >>> handle_multioutput(("x","y"), value([0, 1]), d, None)
     {'x': 0, 'y': 1}
-    >>> handle_multioutput(("x","y"), value({1: "a", 0: "b"}), d)
+    >>> handle_multioutput(("x","y"), value({1: "a", 0: "b"}), d, None)
     {'x': 'b', 'y': 'a'}
     """
     from hdict import value
     from hdict.content.entry.subvalue import SubValue
 
     data = {}
     match entry:
         case value(value=list() as lst):
             if len(field_names) != len(lst):  # pragma: no cover
                 raise Exception(f"Number of output fields ('{len(field_names)}') should match number of list elements ('{len(lst)}').")
             for field_name, val in zip(field_names, lst):
-                data[field_name] = handle_item(field_name, val, previous)
+                data[field_name] = handle_item(field_name, val, previous_result, previous)
         case value(value=dict() as dct):
             if len(field_names) != len(dct):  # pragma: no cover
                 raise Exception(f"Number of output fields ('{len(field_names)}') should match number of dict entries ('{len(dct)}').")
             for field_name, (_, val) in zip(field_names, sorted(dct.items())):
-                data[field_name] = handle_item(field_name, val, previous)
+                data[field_name] = handle_item(field_name, val, previous_result, previous)
         case AbsEntry() | apply():
             keys = []  # For repr().
-            parent = Closure(entry, previous, keys) if isinstance(entry, apply) else entry
+            parent = Closure(entry, previous_result, keys, previous) if isinstance(entry, apply) else entry
             n = len(field_names)
             for key, i, source in loop_field_names(field_names):
                 if key is not None:
                     keys.append(key)
                     data[key] = SubValue(parent, i, n, source)
         case _:  # pragma: no cover
             raise Exception(f"Cannot handle multioutput for key '{field_names}' and type '{type(entry).__name__}'.")
@@ -162,27 +166,27 @@
     elif any(isinstance(x, tuple) for x in field_names):  # pragma: no cover
         raise Exception(f"Cannot mix translated and non translated outputs.", field_names)
     else:
         for i, field_name in enumerate(field_names):
             yield field_name, i, None
 
 
-def handle_mirror(k, data, id, kind):  # object | Cached
-    from hdict.content.entry.cached import Cached
-
-    if not isinstance(data[k], (Cached, frozenhdict)):  # pragma: no cover
-        raise Exception(f"Cannot handle fetched object of type `{type(data[k])}`")
-    match kind:
-        case "<class 'pandas.core.frame.DataFrame'>":
-            f = lambda **kwargs: kwargs[k].asdf
-            return apply(f, fhosh=ø, **{k: field(k)}).enclosure(data, k)
-        case None:  # pragma: no cover
-            pass
-        case _:  # pragma: no cover
-            raise Exception(f"Unknown mirror field kind `{kind}`.")
+# def handle_mirror(k, data, id, kind, previous):  # object | Cached
+#     from hdict.content.entry.cached import Cached
+#
+#     if not isinstance(data[k], (Cached, frozenhdict)):  # pragma: no cover
+#         raise Exception(f"Cannot handle fetched object of type `{type(data[k])}`")
+#     match kind:
+#         case "<class 'pandas.core.frame.DataFrame'>":
+#             f = lambda **kwargs: kwargs[k].asdf
+#             return apply(f, fhosh=ø, **{k: field(k)}).enclosure(data, k, previous)
+#         case None:  # pragma: no cover
+#             pass
+#         case _:  # pragma: no cover
+#             raise Exception(f"Unknown mirror field kind `{kind}`.")
 
 
 def handle_format(format, fields, df, name):
     """
     >>> from hdict import hdict
     >>> df = hdict(index=[1,2], X=[3,4], y=[5,6]).asdf
     >>> handle_format("Xy", ["X", "y"], df, True).show(colored=False)
```

### Comparing `hdict-1.230706.1/src/hdict/data/empty_.py` & `hdict-2.230721.2/src/hdict/data/empty_.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,45 +17,37 @@
 #
 #  (*) Removing authorship by any means, e.g. by distribution of derived
 #  works or verbatim, obfuscated, compiled or rewritten versions of any
 #  part of this work is illegal and it is unethical regarding the effort and
 #  time spent here.
 #
 
-from hdict.content.argument.field import field
-from hdict.content.argument.sample import sample
 from hdict.data.frozenhdict import frozenhdict
 
 
 class Empty_(frozenhdict):
     """
-    >>> from hdict import _
-    >>> d = _ >> {"x": 5} >> dict(y=7)
-    >>> type(_), type(d)
+    >>> from hdict import Ø
+    >>> d = Ø >> {"x": 5} >> dict(y=7)
+    >>> type(Ø), type(d)
     (<class 'hdict.Empty'>, <class 'hdict.hdict'>)
     >>> d.show(colored=False)
     {
         x: 5,
         y: 7,
         _id: A0G3Y7KNMLihDvpSJ3tB.zxshc6u1CbbiiYjCAAA,
         _ids: {
             x: ecvgo-CBPi7wRWIxNzuo1HgHQCbdvR058xi6zmr2,
             y: eJCW9jGsdZTD6-AD9opKwjPIOWZ4R.T0CG2kdyzf
         }
     }
-    >>> str(_ * {})
+    >>> str(Ø * {})
     '⦑{} » {}⦒'
     """
 
-    def __getattr__(self, item):
-        return field(item)
-
-    def __getitem__(self, item):
-        return sample(*item)
-
     def __rshift__(self, other):
         res = super().__rshift__(other)
         if res is NotImplemented:  # pragma: no cover
             return res
         if isinstance(res, frozenhdict):
             res = res.unfrozen
         return res
```

### Comparing `hdict-1.230706.1/src/hdict/data/frozenhdict.py` & `hdict-2.230721.2/src/hdict/data/frozenhdict.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,17 +126,14 @@
 
     # noinspection PyMissingConstructor
     def __init__(self, /, _dictionary=None, _previous=None, **kwargs):
         from hdict.content.entry import AbsEntry
         from hdict.data.aux_frozendict import handle_identity
         from hdict.data.aux_frozendict import handle_items
 
-        if _previous is None:
-            _previous = {}
-
         # todo: : check if _dictionary keys is 'str'; regex to check if k is an identifier;
         data = _dictionary or {}
         # REMINDER: Inside data, the only 'dict' entries are "_id" and "_ids", the rest are AbsEntry objects.
         self.data: dict[str, AbsEntry | str | dict[str, str]]
         self.data = handle_items(data, kwargs, previous=_previous)
         self.hosh, self.ids = handle_identity(self.data)
         self.id = self.hosh.id
@@ -190,15 +187,15 @@
         from hdict.content.argument.apply import apply
 
         if isinstance(other, apply):  # pragma: no cover
             raise Exception(f"Cannot apply without specifying output(s).\n" f"Hint: d >> apply(f)('output_field1', 'output_field2')")
         from hdict.content.argument import AbsArgument
 
         if isinstance(other, AbsArgument):  # pragma: no cover
-            raise Exception(f"Cannot pipe {type(other).__name__} without specifying output.\n" f"Hint: d >> {'field name': object}\n" f"Hint: d['field name'] = object")
+            raise Exception(f"Cannot pipe {type(other).__name__} without specifying output.\n" "Hint: d >> {'field name': object}\n" f"Hint: d['field name'] = object")
 
         from hdict.expression.expr import Expr
 
         match other:
             case hdict() | frozenhdict():
                 dct = other.raw
             case ApplyOut(nested, out):
@@ -209,15 +206,15 @@
                 dct = {k: Cached(self.ids[k], storage, self.raw[k]) for k in fields}
             case dict():
                 dct = other
             case Expr():
                 return Expr(self, other).solve()
             case _:  # pragma: no cover
                 return NotImplemented
-        return frozenhdict(dct, _previous=self.data)
+        return frozenhdict(dct, _previous=self)
 
     def __getitem__(self, item):  # pragma: no cover
         return self.data[item].value
 
     def __getattr__(self, item):  # pragma: no cover
         if item in self.data:
             return self.data[item].value
@@ -262,14 +259,15 @@
         if self._evaluated is None:
             for k, val in self.data.items():
                 val.evaluate()
             self._evaluated = self
         return self
 
     def evaluate(self):
+        # todo: add flag to inhibit evaluation (i.e., fetching) of cached values; or other solution, e.g. Cache(write_onapply)
         _ = self.evaluated
 
     @property
     def asdict(self):
         """
         Convert to 'dict', including ids.
 
@@ -424,24 +422,23 @@
             # if not k.startswith("_"):
             yield k, (val.value if evaluate else val)
 
     def save(self, storage: dict):
         """
         Store an entire frozenidict
         """
-        from hdict.content.entry.cached import kindid
         from hdict.persistence.stored import Stored
 
         data = {self.id: self.ids}
         for field, fid in self.ids.items():
             value = self[field]
             if field.endswith("_"):
                 raise Exception(f"Not implemented for mirror fields")
                 # todo:  confirm existence of the counterpart
-                data[kindid(fid)] = str(type(value))
+                # data[kindid(fid)] = str(type(value))
             elif isinstance(value, frozenhdict):
                 value.save(storage)
             else:
                 data[fid] = Stored(value)
         # todo:  check if frozenhdict is being stored by mistake
         # todo:  attribute/method as subfield:
         #       apply(f, _.df.x)            SubField(name="df", attribute="x")
@@ -462,16 +459,14 @@
     def fetch(id: str, storage: dict, lazy=True, ishdict=False) -> Union["frozenhdict", None]:
         """
         Fetch a single entry
 
         When cache is a list, traverse it from the end (right item to the left item).
         """
         from hdict.content.entry.cached import Cached
-        from hdict.content.entry.cached import getkind
-        from hdict.data.aux_frozendict import handle_mirror
         from hdict.persistence.stored import Stored
 
         if id not in storage:
             return None
         obj = storage[id]
         if isinstance(obj, dict):
             ishdict = True  # Set to True, because now we have a nested frozenhdict
@@ -483,28 +478,28 @@
             data = {}
             mirrored = set()
             for field, fid in ids.items():
                 if field.endswith("_"):
                     # TODO:  2023-06-23
                     #  -
                     raise Exception(f"Not implemented for mirror fields")
-                    mirrored.add(field[:-1])
+                    # mirrored.add(field[:-1])
                     continue
                 if lazy:
                     data[field] = Cached(fid, storage)
                 else:
                     obj = frozenhdict.fetch(fid, storage, lazy=False, ishdict=False)
                     if obj is None:  # pragma: no cover
                         print(storage.keys())
                         raise Exception(f"Incomplete hdict: id '{id}' not found in the provided cache.")
                     data[field] = obj
-            for field in mirrored:
-                obj = data[field]
-                kind = obj.kind if isinstance(obj, Cached) else getkind(storage, obj.hosh)
-                data[field + "_"] = handle_mirror(field, data, ids[field], kind)
+            # for field in mirrored:
+            #     obj = data[field]
+            #     kind = obj.kind if isinstance(obj, Cached) else getkind(storage, obj.hosh)
+            #     data[field + "_"] = handle_mirror(field, data, ids[field], kind)
             return frozenhdict.fromdict(data, ids)
 
         return obj.content
 
     @property
     def asdf(self):
         """
@@ -519,15 +514,15 @@
     @staticmethod
     def fromfile(name, fields=None, format="df", named=None, hide_types=True):
         r"""
         Input format is defined by file extension: .arff, .csv
         """
         from hdict.data.aux_frozendict import handle_format
 
-        df, name = file2df(name, hide_types)
+        df, name = file2df(name, hide_types, True)
         return handle_format(format, fields, df, named and name)
 
     @staticmethod
     def fromtext(text: str, fields=None, format="df", named=None):
         r"""
         Input format is defined by file extension: .arff, .csv
         """
```

### Comparing `hdict-1.230706.1/src/hdict/data/hdict_.py` & `hdict-2.230721.2/src/hdict/data/hdict_.py`

 * *Files 6% similar despite different names*

```diff
@@ -62,14 +62,38 @@
         _ids: {
             x: KeU-dCTjUgnSYGRNrrMMr4i.hg64Dkkfb3c14eh3,
             f: p-nM7oHlOFr6iHSF9ZISWXc9zqi017c3zcvcV8Dr
         }
     }
     >>> str({"a": 2} * d)  # doctest:+ELLIPSIS
     '⦑{a: 2} » {x: 4, f: "<function <lambda> at 0x...>"}⦒'
+    >>> (d >> apply(lambda d: d.x, _).X).evaluated.show(colored=False)  # doctest:+ELLIPSIS
+    {
+        x: 4,
+        f: "<function <lambda> at 0x...>",
+        X: 4,
+        _id: KaIR9dqecR44MZVRrXLUzwqnIbCHhbOkQswgCuQl,
+        _ids: {
+            x: KeU-dCTjUgnSYGRNrrMMr4i.hg64Dkkfb3c14eh3,
+            f: p-nM7oHlOFr6iHSF9ZISWXc9zqi017c3zcvcV8Dr,
+            X: M411IcX.kF9pEdsWGIiS-XGn.R45qYTVQS0ewQs2
+        }
+    }
+    >>> (d >> apply(lambda _: _.x).X).evaluated.show(colored=False)  # doctest:+ELLIPSIS
+    {
+        x: 4,
+        f: "<function <lambda> at 0x...>",
+        X: 4,
+        _id: c1ZgriP45q8xEmDTkRcHjYe2v1C7RLyyZK4NgQ0L,
+        _ids: {
+            x: KeU-dCTjUgnSYGRNrrMMr4i.hg64Dkkfb3c14eh3,
+            f: p-nM7oHlOFr6iHSF9ZISWXc9zqi017c3zcvcV8Dr,
+            X: nVVYNVw8RyQ-7Kv0CxAUeLjRIzZwZwE7-8BKaaFr
+        }
+    }
     """
 
     # noinspection PyMissingConstructor
     def __init__(self, /, _dictionary: dict = None, _frozen: frozenhdict = None, **kwargs):
         # Build hdict from frozen or fresh data. Never both.
         self.frozen = _frozen or frozenhdict(_dictionary, **kwargs)
         self.raw = self.frozen.data
@@ -370,23 +394,34 @@
 
         >>> from hdict import hdict, cache
         >>> from testfixtures import TempDirectory
         >>> arff = "@RELATION mini\n@ATTRIBUTE attr1	REAL\n@ATTRIBUTE attr2 	REAL\n@ATTRIBUTE class 	{0,1}\n@DATA\n5.1,3.5,0\n3.1,4.5,1"
         >>> with TempDirectory() as tmp:  # doctest:+ELLIPSIS
         ...    tmp.write("mini.arff", arff.encode())
         ...    d = hdict.fromfile(tmp.path + "/mini.arff", fields=["df"])
+        ...    d2 = hdict.fromfile(tmp.path + "/mini.arff", fields=["df"], named=True)
         '/tmp/.../mini.arff'
         >>> d.show(colored=False)
         {
             df: "‹{'attr1': {0: 5.1, 1: 3.1}, 'attr2': {0: 3.5, 1: 4.5}, 'class': {0: '0', 1: '1'}}›",
             _id: lV4eqST0pTJL.B3GB4Njtv.P1P2aS5EcuQrjnrdX,
             _ids: {
                 df: rq05QYjRDa4F3kJfE4P8USt4ngF.3skHvVOU5aUt
             }
         }
+        >>> d2.show(colored=False)
+        {
+            df: "‹{'attr1': {0: 5.1, 1: 3.1}, 'attr2': {0: 3.5, 1: 4.5}, 'class': {0: '0', 1: '1'}}›",
+            name: " mini",
+            _id: zd8NFU.IBqgF9a2uaPpZ4y3e1xm2ly25f.6btvgN,
+            _ids: {
+                df: rq05QYjRDa4F3kJfE4P8USt4ngF.3skHvVOU5aUt,
+                name: 5nzeWHgeVef.PD8CnIrPcjwGqaYoRCXK0iwH0cKm
+            }
+        }
         >>> storage = {}
         >>> d.save(storage)
         >>> d = hdict.fetch(d.id, storage)
         >>> d.show(colored=False)
         {
             df: ↑↓ cached at `dict`·,
             _id: lV4eqST0pTJL.B3GB4Njtv.P1P2aS5EcuQrjnrdX,
@@ -477,15 +512,15 @@
         Fetch an entire hdict
 
         >>> from hdict import _
         >>> from hdict.persistence.stored import Stored
         >>> fid = "1234567890123456789012345678901234567890"
         >>> did = "0000567890123456789012345678901234567890"
         >>> storage = {did: {"x": fid}, fid: Stored(5)}
-        >>> d = _.load(did, storage)
+        >>> d = (+_).load(did, storage)
         >>> d.show(colored=False)
         {
             x: ↑↓ cached at `dict`·,
             _id: kYzgpPdRgQSYSEpp1qt4EHQLQJXuyb2WDQS-iNPh,
             _ids: {
                 x: 1234567890123456789012345678901234567890
             }
@@ -580,11 +615,16 @@
         b  2  6
         c  3  7
         """
         return self.frozen.asdf
 
     @property
     def hoshes(self):
+        """
+        >>> from hdict import frozenhdict
+        >>> [h.id for h in frozenhdict(x=3, y=2).hoshes.values()]
+        ['KGWjj0iyLAn1RG6RTGtsGE3omZraJM6xO.kvG5pr', 'k3PWYRxIEc0lEvD1f6rbnk.36RAD5AyfROy1aT29']
+        """
         return self.frozen.hoshes
 
     # def __reduce__(self):
     # return self.frozen.__reduce__()
```

### Comparing `hdict-1.230706.1/src/hdict/dataset/dataset.py` & `hdict-2.230721.2/src/hdict/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `hdict-1.230706.1/src/hdict/dataset/pandas_handling.py` & `hdict-2.230721.2/src/hdict/dataset/pandas_handling.py`

 * *Files identical despite different names*

### Comparing `hdict-1.230706.1/src/hdict/expression/expr.py` & `hdict-2.230721.2/src/hdict/expression/expr.py`

 * *Files identical despite different names*

### Comparing `hdict-1.230706.1/src/hdict/expression/step/applyout.py` & `hdict-2.230721.2/src/hdict/expression/step/applyout.py`

 * *Files identical despite different names*

### Comparing `hdict-1.230706.1/src/hdict/expression/step/cache.py` & `hdict-2.230721.2/src/hdict/expression/step/cache.py`

 * *Files identical despite different names*

### Comparing `hdict-1.230706.1/src/hdict/expression/step/step.py` & `hdict-2.230721.2/src/hdict/expression/step/step.py`

 * *Files identical despite different names*

### Comparing `hdict-1.230706.1/src/hdict/persistence/stored.py` & `hdict-2.230721.2/src/hdict/persistence/stored.py`

 * *Files identical despite different names*

### Comparing `hdict-1.230706.1/src/hdict/text/customjson.py` & `hdict-2.230721.2/src/hdict/text/customjson.py`

 * *Files identical despite different names*

### Comparing `hdict-1.230706.1/setup.py` & `hdict-2.230721.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,53 +1,235 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: hdict
+Version: 2.230721.2
+Summary: A versatile dictionary based on a novel paradigm useful for computing, caching, experiments, distributed data, among others.
+License: GPLv3
+Author: davips
+Author-email: dpsabc@gmail.com
+Requires-Python: >=3.10,<4.0
+Classifier: License :: Other/Proprietary License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: full
+Requires-Dist: hosh (>=3.230705.2,<4.0.0)
+Requires-Dist: indexed (>=1.3.0,<2.0.0)
+Requires-Dist: lange (>=1.230203.2,<2.0.0)
+Requires-Dist: liac-arff (>=2.5.0,<3.0.0) ; extra == "full"
+Requires-Dist: lz4 (>=4.3.2,<5.0.0) ; extra == "full"
+Requires-Dist: pandas (>=2.0.0,<3.0.0) ; extra == "full"
+Requires-Dist: safeserializer (>=0.230202.1,<0.230203.0) ; extra == "full"
+Requires-Dist: scikit-learn (>=1.2.2,<2.0.0) ; extra == "full"
+Requires-Dist: shelchemy (>=0.220906.3,<0.220907.0) ; extra == "full"
+Description-Content-Type: text/markdown
+
+![test](https://github.com/davips/hdict/workflows/test/badge.svg)
+[![codecov](https://codecov.io/gh/davips/hdict/branch/main/graph/badge.svg)](https://codecov.io/gh/davips/hdict)
+<a href="https://pypi.org/project/hdict">
+<img src="https://img.shields.io/pypi/v/hdict.svg?label=release&color=blue&style=flat-square" alt="pypi">
+</a>
+![Python version](https://img.shields.io/badge/python-3.10+-blue.svg)
+[![license: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
+
+<!--- [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5501845.svg)](https://doi.org/10.5281/zenodo.5501845) --->
+[![arXiv](https://img.shields.io/badge/arXiv-2109.06028-b31b1b.svg?style=flat-square)](https://arxiv.org/abs/2109.06028)
+[![API documentation](https://img.shields.io/badge/API-autogenerated-a030a0.svg)](https://davips.github.io/hdict)
+[![Manual](https://img.shields.io/badge/manual-handcrafted-a030a0.svg)](https://hosh.page)
+[![Downloads](https://static.pepy.tech/badge/hdict)](https://pepy.tech/project/hdict)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/hdict)
+
+# hdict { A _unique_ data structure }
+[Website](https://hosh.page) | 
+[Latest Release](https://pypi.org/project/hdict) |
+[Current Code](https://github.com/davips/hdict) |
+[API Documentation](https://davips.github.io/hdict)
+
+Please see the [website](https://hosh.page) for more detailed usage information.
+
+## Overview
+Shortly, `hdict` is a data structure useful for frictionless experiments, distributed data, among others.
+It can be more formally defined as a hosh¹-based cacheable lazy `dict` with predictable/deterministic universally unique² identifiers.
+
+This library is stable for the most common scenarios.
+However, we will wait for more use in the wild before reaching the major version 1.
+See the Section Versioning below for more information.
+
+¹ hosh: _Operable HaSH_
+
+² unique: _probabilistically guaranteed_
+
+
+
+### Context
+
+  * [hosh](https://pypi.org/project/hosh): identification engine at the core of `hdict`
+  * previous projects: [hoshmap](https://pypi.org/project/hoshmap), [idict](https://pypi.org/project/idict), [ldict](https://pypi.org/project/ldict), [garoupa](https://pypi.org/project/garoupa)
+
+### The concept
+
+`hdict` is like an ordinary `dict` with `str` keys. 
+Each entry, called _field_, and the `hdict` itself, are identified by 40-digit hashes (see [hosh](https://pypi.org/project/hosh)).
+A `hdict` object (say `d`) provides two extra entries: `_id` (hdict identifier) and `_ids` (field identifiers),
+accessible through square brackets or through the shortcuts `d.id` and `d.ids`.
+
+**`hdict` creation**
+<details>
+<p>
+
+```python3
+from hdict import hdict
+
+# From named arguments.
+d = hdict(x=5, y=7, z=10)
+
+# From a dict object.
+d = hdict({"x": 5, "y": 7, "z": 10})
+
+# From an empty 'hdict' object.
+d = hdict() >> {"x": 5} >> {"y": 7, "z": 10}
+
+# All three options have the same result.
+d.show(colored=False)
+"""
+{
+    x: 5,
+    y: 7,
+    z: 10,
+    _id: BN-3Q3Z.2Q.9nsbIYnOI75HT7xhgjvF6wErwBPTn,
+    _ids: {
+        x: ecvgo-CBPi7wRWIxNzuo1HgHQCbdvR058xi6zmr2,
+        y: eJCW9jGsdZTD6-AD9opKwjPIOWZ4R.T0CG2kdyzf,
+        z: u-Yykj2nDtKaUMGzfqScX5Y14qC7eqJrO7lXrJ1m
+    }
+}
+"""
+```
+
+```python3
 
-package_dir = \
-{'': 'src'}
+from hosh import setup
 
-packages = \
-['hdict',
- 'hdict.abs',
- 'hdict.content',
- 'hdict.content.argument',
- 'hdict.content.entry',
- 'hdict.data',
- 'hdict.dataset',
- 'hdict.expression',
- 'hdict.expression.step',
- 'hdict.persistence',
- 'hdict.text']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['hosh>=3.230705.2,<4.0.0', 'indexed>=1.3.0,<2.0.0', 'lange>=1.230203.2,<2.0.0']
-
-extras_require = \
-{'full': ['pandas>=2.0.0,<3.0.0',
-          'shelchemy>=0.220906.3,<0.220907.0',
-          'safeserializer>=0.230202.1,<0.230203.0',
-          'lz4>=4.3.2,<5.0.0',
-          'scikit-learn>=1.2.2,<2.0.0',
-          'liac-arff>=2.5.0,<3.0.0']}
-
-setup_kwargs = {
-    'name': 'hdict',
-    'version': '1.230706.1',
-    'description': 'A versatile dictionary based on a novel paradigm useful for computing, caching, experiments, distributed data, among others.',
-    'long_description': '![test](https://github.com/davips/hdict/workflows/test/badge.svg)\n[![codecov](https://codecov.io/gh/davips/hdict/branch/main/graph/badge.svg)](https://codecov.io/gh/davips/hdict)\n<a href="https://pypi.org/project/hdict">\n<img src="https://img.shields.io/pypi/v/hdict.svg?label=release&color=blue&style=flat-square" alt="pypi">\n</a>\n![Python version](https://img.shields.io/badge/python-3.10+-blue.svg)\n[![license: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)\n\n<!--- [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5501845.svg)](https://doi.org/10.5281/zenodo.5501845) --->\n[![arXiv](https://img.shields.io/badge/arXiv-2109.06028-b31b1b.svg?style=flat-square)](https://arxiv.org/abs/2109.06028)\n[![API documentation](https://img.shields.io/badge/API-autogenerated-a030a0.svg)](https://davips.github.io/hdict)\n[![Manual](https://img.shields.io/badge/manual-handcrafted-a030a0.svg)](https://hosh.page)\n[![Downloads](https://static.pepy.tech/badge/hdict)](https://pepy.tech/project/hdict)\n\n# hdict { A _unique_ data structure }\n[Website](https://hosh.page) | \n[Latest Release](https://pypi.org/project/hdict) |\n[Current Code](https://github.com/davips/hdict) |\n[API Documentation](https://davips.github.io/hdict)\n\nPlease see the [website](https://hosh.page) for more detailed usage information.\n\n## Overview\nShortly, `hdict` is a data structure useful for frictionless experiments, distributed data, among others.\nIt can be more formally defined as a hosh¹-based cacheable lazy `dict` with predictable/deterministic universally unique² identifiers.\n\nThis library is stable for the most common scenarios.\nHowever, we will wait for more use in the wild before reaching the major version 1.\nSee the Section Versioning below for more information.\n\n¹ hosh: _Operable HaSH_\n\n² unique: _probabilistically guaranteed_\n\n\n\n### Context\n\n  * [hosh](https://pypi.org/project/hosh): identification engine at the core of `hdict`\n  * previous projects: [hoshmap](https://pypi.org/project/hoshmap), [idict](https://pypi.org/project/idict), [ldict](https://pypi.org/project/ldict), [garoupa](https://pypi.org/project/garoupa)\n\n### The concept\n\n`hdict` is like an ordinary `dict` with `str` keys. \nEach entry, called _field_, and the `hdict` itself, are identified by 40-digit hashes (see [hosh](https://pypi.org/project/hosh)).\nA `hdict` object (say `d`) provides two extra entries: `_id` (hdict identifier) and `_ids` (field identifiers),\naccessible through square brackets or through the shortcuts `d.id` and `d.ids`.\n\n**`hdict` creation**\n<details>\n<p>\n\n```python3\nfrom hdict import hdict\n\n# From named arguments.\nd = hdict(x=5, y=7, z=10)\n\n# From a dict object.\nd = hdict({"x": 5, "y": 7, "z": 10})\n\n# From an empty \'hdict\' object.\nd = hdict() >> {"x": 5} >> {"y": 7, "z": 10}\n\n# All three options have the same result.\nd.show(colored=False)\n"""\n{\n    x: 5,\n    y: 7,\n    z: 10,\n    _id: BN-3Q3Z.2Q.9nsbIYnOI75HT7xhgjvF6wErwBPTn,\n    _ids: {\n        x: ecvgo-CBPi7wRWIxNzuo1HgHQCbdvR058xi6zmr2,\n        y: eJCW9jGsdZTD6-AD9opKwjPIOWZ4R.T0CG2kdyzf,\n        z: u-Yykj2nDtKaUMGzfqScX5Y14qC7eqJrO7lXrJ1m\n    }\n}\n"""\n```\n\n```python3\n\nfrom hosh import setup\n\n# For better integration within the documentation, we change the color theme.\nsetup(dark_theme=False)\n\nd.show(colored=False)\n\n"""\n{\n    x: 5,\n    y: 7,\n    z: 10,\n    _id: BN-3Q3Z.2Q.9nsbIYnOI75HT7xhgjvF6wErwBPTn,\n    _ids: {\n        x: ecvgo-CBPi7wRWIxNzuo1HgHQCbdvR058xi6zmr2,\n        y: eJCW9jGsdZTD6-AD9opKwjPIOWZ4R.T0CG2kdyzf,\n        z: u-Yykj2nDtKaUMGzfqScX5Y14qC7eqJrO7lXrJ1m\n    }\n}\n"""\n```\n\n\n</p>\n</details>\n\nA field contains a value or a function application.\nA field pointing to an application is only evaluated on demand, i.e., lazily.\n\n<!-- ------------------------------------------------------------------------ \nValue objects can have custom identifiers as well, if provided whithin the entry `ids`. \nOtherwise, identifiers for functions and values will be calculated through blake3 hashing of their content.\nFor functions, the bytecode is used as content.\nFor this reason, such functions should be simple, with minimal external dependencies or\nwith their import statements inside the function body.\nThis decreases the odds of using two functions with identical local code (and, therefore, identical identifiers)\nperforming different calculations.\n\ntransformation steps done through the operator `>>`, which symbolizes the ordering of the steps.\n* **value insertion** - represented by dict-like objects\n* **function application** - represented by ordinary Python functions\n\nFunctions, `hdict`s, and values have a deterministic UUID\n(called _hosh_ - **o**perable **h**a**sh**). \nIdentifiers (hoshes) for `hdict`s and values are predictable through the\nmagic available [here](https://pypi.org/project/garoupa).\nAn `hdict` is completely defined by its key-value pairs so that\nit can be converted from/to a built-in `dict`.\n\n\n------------------------------------------------------------------------  -->\n\nPlease refer to our [website](https://hosh.page) for more examples.\n\n\n## Installation\n### ...as a standalone lib\n```bash\n# Set up a virtualenv. \npython3 -m venv venv\nsource venv/bin/activate\n\n# Install from PyPI...\npip install --upgrade pip\npip install -U hdict\n\n# use the flag \'full\' for extra functionality (recommended if working with persistence or some special values like DataFrames)\npip install -U hdict[full]\n\n# ...or, install from updated source code.\npip install git+https://github.com/davips/hdict\n```\n\n### ...from source\n```bash\ngit clone https://github.com/davips/hdict\ncd hdict\npoetry install\n\n# use the flag \'full\' for extra functionality (recommended if working with persistence or some special values like DataFrames)  \npoetry install -E full\n```\n\n## Examples\n\nPlease refer to our [website](https://hosh.page) for examples.\n\n\n\n## Development\n### Licensing\nThe initial license choosen is GPL. Please contact the developer for other licensing needs.\n\n### Versioning\nWhile the version scheme has a meaningful calendar component (`minor=yymmdd`), it is still compatible with semantic versioning.\nFor instance, the version `0.230215.1` means `major=0`, `minor=230215`, `micro/patch=1`. Notes:\n * While `major=0`, some compatibility-breaking changes may occur.\n * From `major=1` onwards, compatibility-breaking changes increment it, and update the minor version to reflect the release date.\n * New (non breaking) features update only the minor version to reflect the release date.\n * Bug fixes (including compatibility-breaking ones) increment only the micro version.\n\n### Contributing\n#### Collaboration\nWe have ongoing research applying this tool to machine learning and clinical academic experiments.\nAlthough, the scope of application is broad as it encompasses software development in general.\nFeel free to contact us if you are interested in the project/concept or have a suggestion/interesting problem to be solved.\n\n#### Donation\nCurrently there are no established forms of donation.\nExpenses:\n  * Programming hours\n  * Support\n  * Custom features\n  * Domain name maintenance yearly costs\n\n### Acknowledgement\nThis work was based on a previous research supported by Fapesp under supervision of\nProf. André C. P. L. F. de Carvalho at CEPID-CeMEAI (Grants 2013/07375-0 – 2019/01735-0)\nuntil 2021-03-31.\n\nWe would like to thank the providers of free tools that make this project feasible:\n  * github for hosting the code repository freely\n  * Oracle for hosting the website freely\n  * Developers of Mint, XFCE, and GNU/Linux for the operating system\n  * JetBrains for Intellij IDEA Community Edition\n  * Developers of Python packages listed in our project.toml\n',
-    'author': 'davips',
-    'author_email': 'dpsabc@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'python_requires': '>=3.10,<4.0',
+# For better integration within the documentation, we change the color theme.
+setup(dark_theme=False)
+
+d.show(colored=False)
+
+"""
+{
+    x: 5,
+    y: 7,
+    z: 10,
+    _id: BN-3Q3Z.2Q.9nsbIYnOI75HT7xhgjvF6wErwBPTn,
+    _ids: {
+        x: ecvgo-CBPi7wRWIxNzuo1HgHQCbdvR058xi6zmr2,
+        y: eJCW9jGsdZTD6-AD9opKwjPIOWZ4R.T0CG2kdyzf,
+        z: u-Yykj2nDtKaUMGzfqScX5Y14qC7eqJrO7lXrJ1m
+    }
 }
+"""
+```
+
+
+</p>
+</details>
 
+A field contains a value or a function application.
+A field pointing to an application is only evaluated on demand, i.e., lazily.
+
+<!-- ------------------------------------------------------------------------ 
+Value objects can have custom identifiers as well, if provided whithin the entry `ids`. 
+Otherwise, identifiers for functions and values will be calculated through blake3 hashing of their content.
+For functions, the bytecode is used as content.
+For this reason, such functions should be simple, with minimal external dependencies or
+with their import statements inside the function body.
+This decreases the odds of using two functions with identical local code (and, therefore, identical identifiers)
+performing different calculations.
+
+transformation steps done through the operator `>>`, which symbolizes the ordering of the steps.
+* **value insertion** - represented by dict-like objects
+* **function application** - represented by ordinary Python functions
+
+Functions, `hdict`s, and values have a deterministic UUID
+(called _hosh_ - **o**perable **h**a**sh**). 
+Identifiers (hoshes) for `hdict`s and values are predictable through the
+magic available [here](https://pypi.org/project/garoupa).
+An `hdict` is completely defined by its key-value pairs so that
+it can be converted from/to a built-in `dict`.
+
+
+------------------------------------------------------------------------  -->
+
+Please refer to our [website](https://hosh.page) for more examples.
+
+
+## Installation
+### ...as a standalone lib
+```bash
+# Set up a virtualenv. 
+python3 -m venv venv
+source venv/bin/activate
+
+# Install from PyPI...
+pip install --upgrade pip
+pip install -U hdict
+
+# use the flag 'full' for extra functionality (recommended if working with persistence or some special values like DataFrames)
+pip install -U hdict[full]
+
+# ...or, install from updated source code.
+pip install git+https://github.com/davips/hdict
+```
+
+### ...from source
+```bash
+git clone https://github.com/davips/hdict
+cd hdict
+poetry install
+
+# use the flag 'full' for extra functionality (recommended if working with persistence or some special values like DataFrames)  
+poetry install -E full
+```
+
+## Examples
+
+Please refer to our [website](https://hosh.page) for examples.
+
+
+
+## Development
+### Licensing
+The initial license choosen is GPL. Please contact the developer for other licensing needs.
+
+### Versioning
+While the version scheme has a meaningful calendar component (`minor=yymmdd`), it is still compatible with semantic versioning.
+For instance, the version `0.230215.1` means `major=0`, `minor=230215`, `micro/patch=1`. Notes:
+ * While `major=0`, some compatibility-breaking changes may occur.
+ * From `major=1` onwards, compatibility-breaking changes increment it, and update the minor version to reflect the release date.
+ * New (non breaking) features update only the minor version to reflect the release date.
+ * Bug fixes (including compatibility-breaking ones) increment only the micro version.
+
+### Contributing
+#### Collaboration
+We have ongoing research applying this tool to machine learning and clinical academic experiments.
+Although, the scope of application is broad as it encompasses software development in general.
+Feel free to contact us if you are interested in the project/concept or have a suggestion/interesting problem to be solved.
+
+#### Donation
+Currently there are no established forms of donation.
+Expenses:
+  * Programming hours
+  * Support
+  * Custom features
+  * Domain name maintenance yearly costs
+
+### Acknowledgement
+This work was based on a previous research supported by Fapesp under supervision of
+Prof. André C. P. L. F. de Carvalho at CEPID-CeMEAI (Grants 2013/07375-0 – 2019/01735-0)
+until 2021-03-31.
+
+We would like to thank the providers of free tools that make this project feasible:
+  * github for hosting the code repository freely
+  * Oracle for hosting the website freely
+  * Developers of Mint, XFCE, and GNU/Linux for the operating system
+  * JetBrains for Intellij IDEA Community Edition
+  * Developers of Python packages listed in our project.toml
 
-setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,101 +1,97 @@
-# -*- coding: utf-8 -*- from setuptools import setup package_dir = \ {'':
-'src'} packages = \ ['hdict', 'hdict.abs', 'hdict.content',
-'hdict.content.argument', 'hdict.content.entry', 'hdict.data', 'hdict.dataset',
-'hdict.expression', 'hdict.expression.step', 'hdict.persistence', 'hdict.text']
-package_data = \ {'': ['*']} install_requires = \ ['hosh>=3.230705.2,<4.0.0',
-'indexed>=1.3.0,<2.0.0', 'lange>=1.230203.2,<2.0.0'] extras_require = \
-{'full': ['pandas>=2.0.0,<3.0.0', 'shelchemy>=0.220906.3,<0.220907.0',
-'safeserializer>=0.230202.1,<0.230203.0', 'lz4>=4.3.2,<5.0.0', 'scikit-
-learn>=1.2.2,<2.0.0', 'liac-arff>=2.5.0,<3.0.0']} setup_kwargs = { 'name':
-'hdict', 'version': '1.230706.1', 'description': 'A versatile dictionary based
-on a novel paradigm useful for computing, caching, experiments, distributed
-data, among others.', 'long_description': '![test](https://github.com/davips/
-hdict/workflows/test/badge.svg)\n[![codecov](https://codecov.io/gh/davips/
-hdict/branch/main/graph/badge.svg)](https://codecov.io/gh/davips/hdict)\n\n
-[pypi]\n\n![Python version](https://img.shields.io/badge/python-3.10+-
-blue.svg)\n[![license: GPL v3](https://img.shields.io/badge/License-GPLv3-
-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)\n\n\n[![arXiv](https://
-img.shields.io/badge/arXiv-2109.06028-b31b1b.svg?style=flat-square)](https://
-arxiv.org/abs/2109.06028)\n[![API documentation](https://img.shields.io/badge/
-API-autogenerated-a030a0.svg)](https://davips.github.io/hdict)\n[![Manual]
-(https://img.shields.io/badge/manual-handcrafted-a030a0.svg)](https://
-hosh.page)\n[![Downloads](https://static.pepy.tech/badge/hdict)](https://
-pepy.tech/project/hdict)\n\n# hdict { A _unique_ data structure }\n[Website]
-(https://hosh.page) | \n[Latest Release](https://pypi.org/project/hdict) |\n
-[Current Code](https://github.com/davips/hdict) |\n[API Documentation](https://
-davips.github.io/hdict)\n\nPlease see the [website](https://hosh.page) for more
-detailed usage information.\n\n## Overview\nShortly, `hdict` is a data
-structure useful for frictionless experiments, distributed data, among
-others.\nIt can be more formally defined as a hoshÂ¹-based cacheable lazy
-`dict` with predictable/deterministic universally uniqueÂ² identifiers.\n\nThis
-library is stable for the most common scenarios.\nHowever, we will wait for
-more use in the wild before reaching the major version 1.\nSee the Section
-Versioning below for more information.\n\nÂ¹ hosh: _Operable HaSH_\n\nÂ²
-unique: _probabilistically guaranteed_\n\n\n\n### Context\n\n * [hosh](https://
-pypi.org/project/hosh): identification engine at the core of `hdict`\n *
-previous projects: [hoshmap](https://pypi.org/project/hoshmap), [idict](https:/
-/pypi.org/project/idict), [ldict](https://pypi.org/project/ldict), [garoupa]
-(https://pypi.org/project/garoupa)\n\n### The concept\n\n`hdict` is like an
-ordinary `dict` with `str` keys. \nEach entry, called _field_, and the `hdict`
-itself, are identified by 40-digit hashes (see [hosh](https://pypi.org/project/
-hosh)).\nA `hdict` object (say `d`) provides two extra entries: `_id` (hdict
-identifier) and `_ids` (field identifiers),\naccessible through square brackets
-or through the shortcuts `d.id` and `d.ids`.\n\n**`hdict` creation**\n\n
-\n\n```python3\nfrom hdict import hdict\n\n# From named arguments.\nd = hdict
-(x=5, y=7, z=10)\n\n# From a dict object.\nd = hdict({"x": 5, "y": 7, "z":
-10})\n\n# From an empty \'hdict\' object.\nd = hdict() >> {"x": 5} >> {"y": 7,
-"z": 10}\n\n# All three options have the same result.\nd.show
-(colored=False)\n"""\n{\n x: 5,\n y: 7,\n z: 10,\n _id: BN-
-3Q3Z.2Q.9nsbIYnOI75HT7xhgjvF6wErwBPTn,\n _ids: {\n x: ecvgo-
-CBPi7wRWIxNzuo1HgHQCbdvR058xi6zmr2,\n y: eJCW9jGsdZTD6-
-AD9opKwjPIOWZ4R.T0CG2kdyzf,\n z: u-Yykj2nDtKaUMGzfqScX5Y14qC7eqJrO7lXrJ1m\n
-}\n}\n"""\n```\n\n```python3\n\nfrom hosh import setup\n\n# For better
-integration within the documentation, we change the color theme.\nsetup
-(dark_theme=False)\n\nd.show(colored=False)\n\n"""\n{\n x: 5,\n y: 7,\n z:
-10,\n _id: BN-3Q3Z.2Q.9nsbIYnOI75HT7xhgjvF6wErwBPTn,\n _ids: {\n x: ecvgo-
-CBPi7wRWIxNzuo1HgHQCbdvR058xi6zmr2,\n y: eJCW9jGsdZTD6-
-AD9opKwjPIOWZ4R.T0CG2kdyzf,\n z: u-Yykj2nDtKaUMGzfqScX5Y14qC7eqJrO7lXrJ1m\n
-}\n}\n"""\n```\n\n\n
-\n\n\nA field contains a value or a function application.\nA field pointing to
-an application is only evaluated on demand, i.e., lazily.\n\n\n\nPlease refer
-to our [website](https://hosh.page) for more examples.\n\n\n##
-Installation\n### ...as a standalone lib\n```bash\n# Set up a virtualenv.
-\npython3 -m venv venv\nsource venv/bin/activate\n\n# Install from PyPI...\npip
-install --upgrade pip\npip install -U hdict\n\n# use the flag \'full\' for
-extra functionality (recommended if working with persistence or some special
-values like DataFrames)\npip install -U hdict[full]\n\n# ...or, install from
-updated source code.\npip install git+https://github.com/davips/
-hdict\n```\n\n### ...from source\n```bash\ngit clone https://github.com/davips/
-hdict\ncd hdict\npoetry install\n\n# use the flag \'full\' for extra
+Metadata-Version: 2.1 Name: hdict Version: 2.230721.2 Summary: A versatile
+dictionary based on a novel paradigm useful for computing, caching,
+experiments, distributed data, among others. License: GPLv3 Author: davips
+Author-email: dpsabc@gmail.com Requires-Python: >=3.10,<4.0 Classifier: License
+:: Other/Proprietary License Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Provides-Extra: full Requires-Dist: hosh
+(>=3.230705.2,<4.0.0) Requires-Dist: indexed (>=1.3.0,<2.0.0) Requires-Dist:
+lange (>=1.230203.2,<2.0.0) Requires-Dist: liac-arff (>=2.5.0,<3.0.0) ; extra
+== "full" Requires-Dist: lz4 (>=4.3.2,<5.0.0) ; extra == "full" Requires-Dist:
+pandas (>=2.0.0,<3.0.0) ; extra == "full" Requires-Dist: safeserializer
+(>=0.230202.1,<0.230203.0) ; extra == "full" Requires-Dist: scikit-learn
+(>=1.2.2,<2.0.0) ; extra == "full" Requires-Dist: shelchemy
+(>=0.220906.3,<0.220907.0) ; extra == "full" Description-Content-Type: text/
+markdown ![test](https://github.com/davips/hdict/workflows/test/badge.svg) [!
+[codecov](https://codecov.io/gh/davips/hdict/branch/main/graph/badge.svg)]
+(https://codecov.io/gh/davips/hdict) [pypi] ![Python version](https://
+img.shields.io/badge/python-3.10+-blue.svg) [![license: GPL v3](https://
+img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-
+3.0)  [![arXiv](https://img.shields.io/badge/arXiv-2109.06028-
+b31b1b.svg?style=flat-square)](https://arxiv.org/abs/2109.06028) [![API
+documentation](https://img.shields.io/badge/API-autogenerated-a030a0.svg)]
+(https://davips.github.io/hdict) [![Manual](https://img.shields.io/badge/
+manual-handcrafted-a030a0.svg)](https://hosh.page) [![Downloads](https://
+static.pepy.tech/badge/hdict)](https://pepy.tech/project/hdict) ![PyPI -
+Downloads](https://img.shields.io/pypi/dm/hdict) # hdict { A _unique_ data
+structure } [Website](https://hosh.page) | [Latest Release](https://pypi.org/
+project/hdict) | [Current Code](https://github.com/davips/hdict) | [API
+Documentation](https://davips.github.io/hdict) Please see the [website](https:/
+/hosh.page) for more detailed usage information. ## Overview Shortly, `hdict`
+is a data structure useful for frictionless experiments, distributed data,
+among others. It can be more formally defined as a hoshÂ¹-based cacheable lazy
+`dict` with predictable/deterministic universally uniqueÂ² identifiers. This
+library is stable for the most common scenarios. However, we will wait for more
+use in the wild before reaching the major version 1. See the Section Versioning
+below for more information. Â¹ hosh: _Operable HaSH_ Â² unique:
+_probabilistically guaranteed_ ### Context * [hosh](https://pypi.org/project/
+hosh): identification engine at the core of `hdict` * previous projects:
+[hoshmap](https://pypi.org/project/hoshmap), [idict](https://pypi.org/project/
+idict), [ldict](https://pypi.org/project/ldict), [garoupa](https://pypi.org/
+project/garoupa) ### The concept `hdict` is like an ordinary `dict` with `str`
+keys. Each entry, called _field_, and the `hdict` itself, are identified by 40-
+digit hashes (see [hosh](https://pypi.org/project/hosh)). A `hdict` object (say
+`d`) provides two extra entries: `_id` (hdict identifier) and `_ids` (field
+identifiers), accessible through square brackets or through the shortcuts
+`d.id` and `d.ids`. **`hdict` creation**
+```python3 from hdict import hdict # From named arguments. d = hdict(x=5, y=7,
+z=10) # From a dict object. d = hdict({"x": 5, "y": 7, "z": 10}) # From an
+empty 'hdict' object. d = hdict() >> {"x": 5} >> {"y": 7, "z": 10} # All three
+options have the same result. d.show(colored=False) """ { x: 5, y: 7, z: 10,
+_id: BN-3Q3Z.2Q.9nsbIYnOI75HT7xhgjvF6wErwBPTn, _ids: { x: ecvgo-
+CBPi7wRWIxNzuo1HgHQCbdvR058xi6zmr2, y: eJCW9jGsdZTD6-
+AD9opKwjPIOWZ4R.T0CG2kdyzf, z: u-Yykj2nDtKaUMGzfqScX5Y14qC7eqJrO7lXrJ1m } } """
+``` ```python3 from hosh import setup # For better integration within the
+documentation, we change the color theme. setup(dark_theme=False) d.show
+(colored=False) """ { x: 5, y: 7, z: 10, _id: BN-
+3Q3Z.2Q.9nsbIYnOI75HT7xhgjvF6wErwBPTn, _ids: { x: ecvgo-
+CBPi7wRWIxNzuo1HgHQCbdvR058xi6zmr2, y: eJCW9jGsdZTD6-
+AD9opKwjPIOWZ4R.T0CG2kdyzf, z: u-Yykj2nDtKaUMGzfqScX5Y14qC7eqJrO7lXrJ1m } } """
+```
+ A field contains a value or a function application. A field pointing to an
+application is only evaluated on demand, i.e., lazily.  Please refer to our
+[website](https://hosh.page) for more examples. ## Installation ### ...as a
+standalone lib ```bash # Set up a virtualenv. python3 -m venv venv source venv/
+bin/activate # Install from PyPI... pip install --upgrade pip pip install -
+U hdict # use the flag 'full' for extra functionality (recommended if working
+with persistence or some special values like DataFrames) pip install -U hdict
+[full] # ...or, install from updated source code. pip install git+https://
+github.com/davips/hdict ``` ### ...from source ```bash git clone https://
+github.com/davips/hdict cd hdict poetry install # use the flag 'full' for extra
 functionality (recommended if working with persistence or some special values
-like DataFrames) \npoetry install -E full\n```\n\n## Examples\n\nPlease refer
-to our [website](https://hosh.page) for examples.\n\n\n\n## Development\n###
-Licensing\nThe initial license choosen is GPL. Please contact the developer for
-other licensing needs.\n\n### Versioning\nWhile the version scheme has a
-meaningful calendar component (`minor=yymmdd`), it is still compatible with
-semantic versioning.\nFor instance, the version `0.230215.1` means `major=0`,
-`minor=230215`, `micro/patch=1`. Notes:\n * While `major=0`, some
-compatibility-breaking changes may occur.\n * From `major=1` onwards,
-compatibility-breaking changes increment it, and update the minor version to
-reflect the release date.\n * New (non breaking) features update only the minor
-version to reflect the release date.\n * Bug fixes (including compatibility-
-breaking ones) increment only the micro version.\n\n### Contributing\n####
-Collaboration\nWe have ongoing research applying this tool to machine learning
-and clinical academic experiments.\nAlthough, the scope of application is broad
-as it encompasses software development in general.\nFeel free to contact us if
-you are interested in the project/concept or have a suggestion/interesting
-problem to be solved.\n\n#### Donation\nCurrently there are no established
-forms of donation.\nExpenses:\n * Programming hours\n * Support\n * Custom
-features\n * Domain name maintenance yearly costs\n\n### Acknowledgement\nThis
-work was based on a previous research supported by Fapesp under supervision
-of\nProf. AndrÃ© C. P. L. F. de Carvalho at CEPID-CeMEAI (Grants 2013/07375-
-0 â 2019/01735-0)\nuntil 2021-03-31.\n\nWe would like to thank the providers
-of free tools that make this project feasible:\n * github for hosting the code
-repository freely\n * Oracle for hosting the website freely\n * Developers of
-Mint, XFCE, and GNU/Linux for the operating system\n * JetBrains for Intellij
-IDEA Community Edition\n * Developers of Python packages listed in our
-project.toml\n', 'author': 'davips', 'author_email': 'dpsabc@gmail.com',
-'maintainer': 'None', 'maintainer_email': 'None', 'url': 'None', 'package_dir':
-package_dir, 'packages': packages, 'package_data': package_data,
-'install_requires': install_requires, 'extras_require': extras_require,
-'python_requires': '>=3.10,<4.0', } setup(**setup_kwargs)
+like DataFrames) poetry install -E full ``` ## Examples Please refer to our
+[website](https://hosh.page) for examples. ## Development ### Licensing The
+initial license choosen is GPL. Please contact the developer for other
+licensing needs. ### Versioning While the version scheme has a meaningful
+calendar component (`minor=yymmdd`), it is still compatible with semantic
+versioning. For instance, the version `0.230215.1` means `major=0`,
+`minor=230215`, `micro/patch=1`. Notes: * While `major=0`, some compatibility-
+breaking changes may occur. * From `major=1` onwards, compatibility-breaking
+changes increment it, and update the minor version to reflect the release date.
+* New (non breaking) features update only the minor version to reflect the
+release date. * Bug fixes (including compatibility-breaking ones) increment
+only the micro version. ### Contributing #### Collaboration We have ongoing
+research applying this tool to machine learning and clinical academic
+experiments. Although, the scope of application is broad as it encompasses
+software development in general. Feel free to contact us if you are interested
+in the project/concept or have a suggestion/interesting problem to be solved.
+#### Donation Currently there are no established forms of donation. Expenses: *
+Programming hours * Support * Custom features * Domain name maintenance yearly
+costs ### Acknowledgement This work was based on a previous research supported
+by Fapesp under supervision of Prof. AndrÃ© C. P. L. F. de Carvalho at CEPID-
+CeMEAI (Grants 2013/07375-0 â 2019/01735-0) until 2021-03-31. We would like
+to thank the providers of free tools that make this project feasible: * github
+for hosting the code repository freely * Oracle for hosting the website freely
+* Developers of Mint, XFCE, and GNU/Linux for the operating system * JetBrains
+for Intellij IDEA Community Edition * Developers of Python packages listed in
+our project.toml
```

