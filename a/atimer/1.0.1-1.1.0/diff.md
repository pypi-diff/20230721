# Comparing `tmp/atimer-1.0.1.tar.gz` & `tmp/atimer-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atimer-1.0.1.tar", last modified: Tue Jan 18 22:00:55 2022, max compression
+gzip compressed data, was "atimer-1.1.0.tar", last modified: Fri Jul 21 19:09:28 2023, max compression
```

## Comparing `atimer-1.0.1.tar` & `atimer-1.1.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 wrobell   (1000) wrobell   (1000)        0 2022-01-18 22:00:55.793594 atimer-1.0.1/
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)    35147 2021-04-13 21:40:50.000000 atimer-1.0.1/COPYING
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1289 2022-01-18 22:00:55.793594 atimer-1.0.1/PKG-INFO
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)      586 2021-04-13 21:40:50.000000 atimer-1.0.1/README
-drwxr-xr-x   0 wrobell   (1000) wrobell   (1000)        0 2022-01-18 22:00:55.790261 atimer-1.0.1/atimer/
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1340 2021-05-27 21:32:39.000000 atimer-1.0.1/atimer/__init__.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)   217220 2022-01-18 22:00:55.000000 atimer-1.0.1/atimer/_atimer.c
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     2833 2021-04-13 21:40:50.000000 atimer-1.0.1/atimer/_atimer.pyx
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     3129 2021-12-23 19:33:20.000000 atimer-1.0.1/atimer/glue.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)        0 2021-04-13 21:40:50.000000 atimer-1.0.1/atimer/py.typed
-drwxr-xr-x   0 wrobell   (1000) wrobell   (1000)        0 2022-01-18 22:00:55.793594 atimer-1.0.1/atimer/tests/
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)      766 2021-04-13 21:40:50.000000 atimer-1.0.1/atimer/tests/__init__.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1794 2021-12-23 19:33:59.000000 atimer-1.0.1/atimer/tests/test_atimer.py
-drwxr-xr-x   0 wrobell   (1000) wrobell   (1000)        0 2022-01-18 22:00:55.793594 atimer-1.0.1/atimer.egg-info/
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1289 2022-01-18 22:00:55.000000 atimer-1.0.1/atimer.egg-info/PKG-INFO
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)      336 2022-01-18 22:00:55.000000 atimer-1.0.1/atimer.egg-info/SOURCES.txt
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)        1 2022-01-18 22:00:55.000000 atimer-1.0.1/atimer.egg-info/dependency_links.txt
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)       89 2022-01-18 22:00:55.000000 atimer-1.0.1/atimer.egg-info/requires.txt
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)        7 2022-01-18 22:00:55.000000 atimer-1.0.1/atimer.egg-info/top_level.txt
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)      115 2021-06-29 22:55:21.000000 atimer-1.0.1/pyproject.toml
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1041 2022-01-18 22:00:55.793594 atimer-1.0.1/setup.cfg
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)      969 2021-06-29 22:55:05.000000 atimer-1.0.1/setup.py
+drwxr-xr-x   0 wrobell   (1000) wrobell   (1000)        0 2023-07-21 19:09:28.931893 atimer-1.1.0/
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)    35147 2023-07-20 22:19:44.000000 atimer-1.1.0/COPYING
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1318 2023-07-21 19:09:28.931893 atimer-1.1.0/PKG-INFO
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)      634 2023-07-20 23:00:35.000000 atimer-1.1.0/README
+drwxr-xr-x   0 wrobell   (1000) wrobell   (1000)        0 2023-07-21 19:09:28.931893 atimer-1.1.0/atimer/
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1329 2023-07-20 22:19:44.000000 atimer-1.1.0/atimer/__init__.py
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)   334714 2023-07-20 22:45:16.000000 atimer-1.1.0/atimer/_atimer.c
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     2835 2023-07-20 22:19:44.000000 atimer-1.1.0/atimer/_atimer.pyx
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     3231 2023-07-20 23:06:05.000000 atimer-1.1.0/atimer/glue.py
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)        0 2023-07-20 22:19:44.000000 atimer-1.1.0/atimer/py.typed
+drwxr-xr-x   0 wrobell   (1000) wrobell   (1000)        0 2023-07-21 19:09:28.931893 atimer-1.1.0/atimer/tests/
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)      768 2023-07-20 22:19:44.000000 atimer-1.1.0/atimer/tests/__init__.py
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1796 2023-07-20 22:19:44.000000 atimer-1.1.0/atimer/tests/test_atimer.py
+drwxr-xr-x   0 wrobell   (1000) wrobell   (1000)        0 2023-07-21 19:09:28.931893 atimer-1.1.0/atimer.egg-info/
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1318 2023-07-21 19:09:28.000000 atimer-1.1.0/atimer.egg-info/PKG-INFO
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)      336 2023-07-21 19:09:28.000000 atimer-1.1.0/atimer.egg-info/SOURCES.txt
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)        1 2023-07-21 19:09:28.000000 atimer-1.1.0/atimer.egg-info/dependency_links.txt
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)       69 2023-07-21 19:09:28.000000 atimer-1.1.0/atimer.egg-info/requires.txt
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)        7 2023-07-21 19:09:28.000000 atimer-1.1.0/atimer.egg-info/top_level.txt
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)      124 2023-07-20 22:19:44.000000 atimer-1.1.0/pyproject.toml
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1021 2023-07-21 19:09:28.931893 atimer-1.1.0/setup.cfg
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)      971 2023-07-20 22:19:44.000000 atimer-1.1.0/setup.py
```

### Comparing `atimer-1.0.1/COPYING` & `atimer-1.1.0/COPYING`

 * *Files identical despite different names*

### Comparing `atimer-1.0.1/PKG-INFO` & `atimer-1.1.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,33 @@
 Metadata-Version: 2.1
 Name: atimer
-Version: 1.0.1
+Version: 1.1.0
 Summary: atimer - timer library for asyncio
 Home-page: https://wrobell.dcmod.org/atimer/
 Author: Artur Wroblewski
 Author-email: wrobell@riseup.net
 License: GPLv3+
 Project-URL: Source Code, https://gitlab.com/n23/atimer
 Project-URL: Bug tracker, https://gitlab.com/n23/atimer/issues
-Platform: UNKNOWN
 Classifier: Topic :: Software Development :: Libraries
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
-Requires-Python: >=3.8
+Requires-Python: >=3.11
 Description-Content-Type: text/x-rst
 Provides-Extra: tests
 License-File: COPYING
 
 `atimer` library implements asynchronous timer Python coroutine based on
 POSIX timers. The coroutine can be used with Python `asyncio
 <https://docs.python.org/3/library/asyncio.html>`_ module API.
 
-The main features are
+The main features of the timer implemented by the library are
 
-- timer expires at regular intervals
-- track number of expirations if a long running task causes overrun
-- start synchronized with system clock at the edge of an interval
-- measure time while system is suspended
+- expires at regular intervals
+- allows to track number of expirations if a long running task causes
+  overrun
+- starts synchronized with system clock at the edge of an interval
+- measures time while system is suspended
 
 The `atimer` library is licensed under terms of GPL license, version 3, see
 `COPYING <https://www.gnu.org/licenses/gpl-3.0.en.html>`_ file for details.
-
-
```

### Comparing `atimer-1.0.1/README` & `atimer-1.1.0/README`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 `atimer` library implements asynchronous timer Python coroutine based on
 POSIX timers. The coroutine can be used with Python `asyncio
 <https://docs.python.org/3/library/asyncio.html>`_ module API.
 
-The main features are
+The main features of the timer implemented by the library are
 
-- timer expires at regular intervals
-- track number of expirations if a long running task causes overrun
-- start synchronized with system clock at the edge of an interval
-- measure time while system is suspended
+- expires at regular intervals
+- allows to track number of expirations if a long running task causes
+  overrun
+- starts synchronized with system clock at the edge of an interval
+- measures time while system is suspended
 
 The `atimer` library is licensed under terms of GPL license, version 3, see
 `COPYING <https://www.gnu.org/licenses/gpl-3.0.en.html>`_ file for details.
```

### Comparing `atimer-1.0.1/atimer/__init__.py` & `atimer-1.1.0/atimer/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # atimer - timer library for asyncio
 # 
-# Copyright (C) 2016-2021 by Artur Wroblewski <wrobell@riseup.net>
+# Copyright (C) 2016 - 2023 by Artur Wroblewski <wrobell@riseup.net>
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -26,16 +26,16 @@
 
 - timer expires at regular intervals
 - track number of expirations if a long running task causes overrun
 - start synchronized with system clock at the edge of an interval
 - measure time while system is suspended
 """
 
-import pkg_resources
+from importlib.metadata import version
 
 from .glue import Timer
 
-__version__ = pkg_resources.get_distribution('atimer').version
+__version__ = version('atimer')
 
 __all__ = ['Timer']
 
 # vim: sw=4:et:ai
```

### Comparing `atimer-1.0.1/atimer/_atimer.c` & `atimer-1.1.0/atimer/_atimer.c`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.26 */
+/* Generated by Cython 3.0.0 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [],
         "name": "atimer._atimer",
         "sources": [
@@ -12,28 +12,40 @@
     "module_name": "atimer._atimer"
 }
 END: Cython Metadata */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
+#if defined(CYTHON_LIMITED_API) && 0
+  #ifndef Py_LIMITED_API
+    #if CYTHON_LIMITED_API+0 > 0x03030000
+      #define Py_LIMITED_API CYTHON_LIMITED_API
+    #else
+      #define Py_LIMITED_API 0x03030000
+    #endif
+  #endif
+#endif
+
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
-#elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
-    #error Cython requires Python 2.6+ or Python 3.3+.
+#elif PY_VERSION_HEX < 0x02070000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
+    #error Cython requires Python 2.7+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_26"
-#define CYTHON_HEX_VERSION 0x001D1AF0
+#define CYTHON_ABI "3_0_0"
+#define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
+#define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
+#define CYTHON_HEX_VERSION 0x030000F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
-#if !defined(WIN32) && !defined(MS_WINDOWS)
+#if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
     #define __stdcall
   #endif
   #ifndef __cdecl
     #define __cdecl
   #endif
   #ifndef __fastcall
@@ -44,30 +56,34 @@
   #define DL_IMPORT(t) t
 #endif
 #ifndef DL_EXPORT
   #define DL_EXPORT(t) t
 #endif
 #define __PYX_COMMA ,
 #ifndef HAVE_LONG_LONG
-  #if PY_VERSION_HEX >= 0x02070000
-    #define HAVE_LONG_LONG
-  #endif
+  #define HAVE_LONG_LONG
 #endif
 #ifndef PY_LONG_LONG
   #define PY_LONG_LONG LONG_LONG
 #endif
 #ifndef Py_HUGE_VAL
   #define Py_HUGE_VAL HUGE_VAL
 #endif
-#ifdef PYPY_VERSION
-  #define CYTHON_COMPILING_IN_PYPY 1
-  #define CYTHON_COMPILING_IN_PYSTON 0
+#if defined(GRAALVM_PYTHON)
+  /* For very preliminary testing purposes. Most variables are set the same as PyPy.
+     The existence of this section does not imply that anything works or is even tested */
+  #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_LIMITED_API 0
+  #define CYTHON_COMPILING_IN_GRAAL 1
+  #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
   #define CYTHON_USE_TYPE_SLOTS 0
+  #undef CYTHON_USE_TYPE_SPECS
+  #define CYTHON_USE_TYPE_SPECS 0
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #if PY_VERSION_HEX < 0x03050000
     #undef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 0
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
@@ -84,35 +100,167 @@
   #define CYTHON_AVOID_BORROWED_REFS 1
   #undef CYTHON_ASSUME_SAFE_MACROS
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #undef CYTHON_METH_FASTCALL
+  #define CYTHON_METH_FASTCALL 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS (PY_MAJOR_VERSION >= 3)
+  #endif
   #undef CYTHON_PEP489_MULTI_PHASE_INIT
-  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #undef CYTHON_USE_MODULE_STATE
+  #define CYTHON_USE_MODULE_STATE 0
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
-#elif defined(PYSTON_VERSION)
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
+  #endif
+#elif defined(PYPY_VERSION)
+  #define CYTHON_COMPILING_IN_PYPY 1
+  #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_LIMITED_API 0
+  #define CYTHON_COMPILING_IN_GRAAL 0
+  #define CYTHON_COMPILING_IN_NOGIL 0
+  #undef CYTHON_USE_TYPE_SLOTS
+  #define CYTHON_USE_TYPE_SLOTS 0
+  #undef CYTHON_USE_TYPE_SPECS
+  #define CYTHON_USE_TYPE_SPECS 0
+  #undef CYTHON_USE_PYTYPE_LOOKUP
+  #define CYTHON_USE_PYTYPE_LOOKUP 0
+  #if PY_VERSION_HEX < 0x03050000
+    #undef CYTHON_USE_ASYNC_SLOTS
+    #define CYTHON_USE_ASYNC_SLOTS 0
+  #elif !defined(CYTHON_USE_ASYNC_SLOTS)
+    #define CYTHON_USE_ASYNC_SLOTS 1
+  #endif
+  #undef CYTHON_USE_PYLIST_INTERNALS
+  #define CYTHON_USE_PYLIST_INTERNALS 0
+  #undef CYTHON_USE_UNICODE_INTERNALS
+  #define CYTHON_USE_UNICODE_INTERNALS 0
+  #undef CYTHON_USE_UNICODE_WRITER
+  #define CYTHON_USE_UNICODE_WRITER 0
+  #undef CYTHON_USE_PYLONG_INTERNALS
+  #define CYTHON_USE_PYLONG_INTERNALS 0
+  #undef CYTHON_AVOID_BORROWED_REFS
+  #define CYTHON_AVOID_BORROWED_REFS 1
+  #undef CYTHON_ASSUME_SAFE_MACROS
+  #define CYTHON_ASSUME_SAFE_MACROS 0
+  #undef CYTHON_UNPACK_METHODS
+  #define CYTHON_UNPACK_METHODS 0
+  #undef CYTHON_FAST_THREAD_STATE
+  #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #undef CYTHON_METH_FASTCALL
+  #define CYTHON_METH_FASTCALL 0
+  #undef CYTHON_FAST_PYCALL
+  #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS (PY_MAJOR_VERSION >= 3)
+  #endif
+  #if PY_VERSION_HEX < 0x03090000
+    #undef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
+  #undef CYTHON_USE_MODULE_STATE
+  #define CYTHON_USE_MODULE_STATE 0
+  #undef CYTHON_USE_TP_FINALIZE
+  #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1 && PYPY_VERSION_NUM >= 0x07030C00)
+  #undef CYTHON_USE_DICT_VERSIONS
+  #define CYTHON_USE_DICT_VERSIONS 0
+  #undef CYTHON_USE_EXC_INFO_STACK
+  #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
+  #endif
+#elif defined(CYTHON_LIMITED_API)
+  #define CYTHON_COMPILING_IN_PYPY 0
+  #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_LIMITED_API 1
+  #define CYTHON_COMPILING_IN_GRAAL 0
+  #define CYTHON_COMPILING_IN_NOGIL 0
+  #undef CYTHON_CLINE_IN_TRACEBACK
+  #define CYTHON_CLINE_IN_TRACEBACK 0
+  #undef CYTHON_USE_TYPE_SLOTS
+  #define CYTHON_USE_TYPE_SLOTS 0
+  #undef CYTHON_USE_TYPE_SPECS
+  #define CYTHON_USE_TYPE_SPECS 1
+  #undef CYTHON_USE_PYTYPE_LOOKUP
+  #define CYTHON_USE_PYTYPE_LOOKUP 0
+  #undef CYTHON_USE_ASYNC_SLOTS
+  #define CYTHON_USE_ASYNC_SLOTS 0
+  #undef CYTHON_USE_PYLIST_INTERNALS
+  #define CYTHON_USE_PYLIST_INTERNALS 0
+  #undef CYTHON_USE_UNICODE_INTERNALS
+  #define CYTHON_USE_UNICODE_INTERNALS 0
+  #ifndef CYTHON_USE_UNICODE_WRITER
+    #define CYTHON_USE_UNICODE_WRITER 0
+  #endif
+  #undef CYTHON_USE_PYLONG_INTERNALS
+  #define CYTHON_USE_PYLONG_INTERNALS 0
+  #ifndef CYTHON_AVOID_BORROWED_REFS
+    #define CYTHON_AVOID_BORROWED_REFS 0
+  #endif
+  #undef CYTHON_ASSUME_SAFE_MACROS
+  #define CYTHON_ASSUME_SAFE_MACROS 0
+  #undef CYTHON_UNPACK_METHODS
+  #define CYTHON_UNPACK_METHODS 0
+  #undef CYTHON_FAST_THREAD_STATE
+  #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #undef CYTHON_METH_FASTCALL
+  #define CYTHON_METH_FASTCALL 0
+  #undef CYTHON_FAST_PYCALL
+  #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS 1
+  #endif
+  #undef CYTHON_PEP489_MULTI_PHASE_INIT
+  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #undef CYTHON_USE_MODULE_STATE
+  #define CYTHON_USE_MODULE_STATE 1
+  #ifndef CYTHON_USE_TP_FINALIZE
+    #define CYTHON_USE_TP_FINALIZE 1
+  #endif
+  #undef CYTHON_USE_DICT_VERSIONS
+  #define CYTHON_USE_DICT_VERSIONS 0
+  #undef CYTHON_USE_EXC_INFO_STACK
+  #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
+  #endif
+#elif defined(PY_NOGIL)
   #define CYTHON_COMPILING_IN_PYPY 0
-  #define CYTHON_COMPILING_IN_PYSTON 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_LIMITED_API 0
+  #define CYTHON_COMPILING_IN_GRAAL 0
+  #define CYTHON_COMPILING_IN_NOGIL 1
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
-  #undef CYTHON_USE_ASYNC_SLOTS
-  #define CYTHON_USE_ASYNC_SLOTS 0
+  #ifndef CYTHON_USE_ASYNC_SLOTS
+    #define CYTHON_USE_ASYNC_SLOTS 1
+  #endif
   #undef CYTHON_USE_PYLIST_INTERNALS
   #define CYTHON_USE_PYLIST_INTERNALS 0
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
   #undef CYTHON_USE_UNICODE_WRITER
   #define CYTHON_USE_UNICODE_WRITER 0
@@ -127,45 +275,46 @@
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
-  #undef CYTHON_PEP489_MULTI_PHASE_INIT
-  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
-  #undef CYTHON_USE_TP_FINALIZE
-  #define CYTHON_USE_TP_FINALIZE 0
+  #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
+  #ifndef CYTHON_USE_TP_FINALIZE
+    #define CYTHON_USE_TP_FINALIZE 1
+  #endif
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
-  #define CYTHON_COMPILING_IN_PYSTON 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
+  #define CYTHON_COMPILING_IN_LIMITED_API 0
+  #define CYTHON_COMPILING_IN_GRAAL 0
+  #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
-  #if PY_VERSION_HEX < 0x02070000
-    #undef CYTHON_USE_PYTYPE_LOOKUP
-    #define CYTHON_USE_PYTYPE_LOOKUP 0
-  #elif !defined(CYTHON_USE_PYTYPE_LOOKUP)
+  #ifndef CYTHON_USE_TYPE_SPECS
+    #define CYTHON_USE_TYPE_SPECS 0
+  #endif
+  #ifndef CYTHON_USE_PYTYPE_LOOKUP
     #define CYTHON_USE_PYTYPE_LOOKUP 1
   #endif
   #if PY_MAJOR_VERSION < 3
     #undef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 0
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
-  #if PY_VERSION_HEX < 0x02070000
-    #undef CYTHON_USE_PYLONG_INTERNALS
-    #define CYTHON_USE_PYLONG_INTERNALS 0
-  #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
+  #ifndef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
@@ -184,33 +333,64 @@
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
   #ifndef CYTHON_FAST_THREAD_STATE
     #define CYTHON_FAST_THREAD_STATE 1
   #endif
-  #ifndef CYTHON_FAST_PYCALL
-    #define CYTHON_FAST_PYCALL (PY_VERSION_HEX < 0x030B00A1)
+  #ifndef CYTHON_FAST_GIL
+    #define CYTHON_FAST_GIL (PY_MAJOR_VERSION < 3 || PY_VERSION_HEX >= 0x03060000 && PY_VERSION_HEX < 0x030C00A6)
   #endif
-  #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
-    #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
+  #ifndef CYTHON_METH_FASTCALL
+    #define CYTHON_METH_FASTCALL (PY_VERSION_HEX >= 0x030700A1)
   #endif
-  #ifndef CYTHON_USE_TP_FINALIZE
-    #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
+  #ifndef CYTHON_FAST_PYCALL
+    #define CYTHON_FAST_PYCALL 1
   #endif
-  #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS 1
   #endif
-  #ifndef CYTHON_USE_EXC_INFO_STACK
-    #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
+  #if PY_VERSION_HEX < 0x03050000
+    #undef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
+  #ifndef CYTHON_USE_MODULE_STATE
+    #define CYTHON_USE_MODULE_STATE 0
+  #endif
+  #if PY_VERSION_HEX < 0x030400a1
+    #undef CYTHON_USE_TP_FINALIZE
+    #define CYTHON_USE_TP_FINALIZE 0
+  #elif !defined(CYTHON_USE_TP_FINALIZE)
+    #define CYTHON_USE_TP_FINALIZE 1
+  #endif
+  #if PY_VERSION_HEX < 0x030600B1
+    #undef CYTHON_USE_DICT_VERSIONS
+    #define CYTHON_USE_DICT_VERSIONS 0
+  #elif !defined(CYTHON_USE_DICT_VERSIONS)
+    #define CYTHON_USE_DICT_VERSIONS  (PY_VERSION_HEX < 0x030C00A5)
+  #endif
+  #if PY_VERSION_HEX < 0x030700A3
+    #undef CYTHON_USE_EXC_INFO_STACK
+    #define CYTHON_USE_EXC_INFO_STACK 0
+  #elif !defined(CYTHON_USE_EXC_INFO_STACK)
+    #define CYTHON_USE_EXC_INFO_STACK 1
+  #endif
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
   #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
+#if !defined(CYTHON_VECTORCALL)
+#define CYTHON_VECTORCALL  (CYTHON_FAST_PYCCALL && PY_VERSION_HEX >= 0x030800B1)
+#endif
+#define CYTHON_BACKPORT_VECTORCALL (CYTHON_METH_FASTCALL && PY_VERSION_HEX < 0x030800B1)
 #if CYTHON_USE_PYLONG_INTERNALS
   #if PY_MAJOR_VERSION < 3
     #include "longintrepr.h"
   #endif
   #undef SHIFT
   #undef BASE
   #undef MASK
@@ -232,78 +412,128 @@
   #elif defined (__STDC_VERSION__) && __STDC_VERSION__ >= 199901L
     #define CYTHON_RESTRICT restrict
   #else
     #define CYTHON_RESTRICT
   #endif
 #endif
 #ifndef CYTHON_UNUSED
+  #if defined(__cplusplus)
+    /* for clang __has_cpp_attribute(maybe_unused) is true even before C++17
+     * but leads to warnings with -pedantic, since it is a C++17 feature */
+    #if ((defined(_MSVC_LANG) && _MSVC_LANG >= 201703L) || __cplusplus >= 201703L)
+      #if __has_cpp_attribute(maybe_unused)
+        #define CYTHON_UNUSED [[maybe_unused]]
+      #endif
+    #endif
+  #endif
+#endif
+#ifndef CYTHON_UNUSED
 # if defined(__GNUC__)
 #   if !(defined(__cplusplus)) || (__GNUC__ > 3 || (__GNUC__ == 3 && __GNUC_MINOR__ >= 4))
 #     define CYTHON_UNUSED __attribute__ ((__unused__))
 #   else
 #     define CYTHON_UNUSED
 #   endif
 # elif defined(__ICC) || (defined(__INTEL_COMPILER) && !defined(_MSC_VER))
 #   define CYTHON_UNUSED __attribute__ ((__unused__))
 # else
 #   define CYTHON_UNUSED
 # endif
 #endif
-#ifndef CYTHON_MAYBE_UNUSED_VAR
+#ifndef CYTHON_UNUSED_VAR
 #  if defined(__cplusplus)
-     template<class T> void CYTHON_MAYBE_UNUSED_VAR( const T& ) { }
+     template<class T> void CYTHON_UNUSED_VAR( const T& ) { }
 #  else
-#    define CYTHON_MAYBE_UNUSED_VAR(x) (void)(x)
+#    define CYTHON_UNUSED_VAR(x) (void)(x)
 #  endif
 #endif
+#ifndef CYTHON_MAYBE_UNUSED_VAR
+  #define CYTHON_MAYBE_UNUSED_VAR(x) CYTHON_UNUSED_VAR(x)
+#endif
 #ifndef CYTHON_NCP_UNUSED
 # if CYTHON_COMPILING_IN_CPYTHON
 #  define CYTHON_NCP_UNUSED
 # else
 #  define CYTHON_NCP_UNUSED CYTHON_UNUSED
 # endif
 #endif
 #define __Pyx_void_to_None(void_result) ((void)(void_result), Py_INCREF(Py_None), Py_None)
 #ifdef _MSC_VER
     #ifndef _MSC_STDINT_H_
         #if _MSC_VER < 1300
-           typedef unsigned char     uint8_t;
-           typedef unsigned int      uint32_t;
+            typedef unsigned char     uint8_t;
+            typedef unsigned short    uint16_t;
+            typedef unsigned int      uint32_t;
+        #else
+            typedef unsigned __int8   uint8_t;
+            typedef unsigned __int16  uint16_t;
+            typedef unsigned __int32  uint32_t;
+        #endif
+    #endif
+    #if _MSC_VER < 1300
+        #ifdef _WIN64
+            typedef unsigned long long  __pyx_uintptr_t;
+        #else
+            typedef unsigned int        __pyx_uintptr_t;
+        #endif
+    #else
+        #ifdef _WIN64
+            typedef unsigned __int64    __pyx_uintptr_t;
         #else
-           typedef unsigned __int8   uint8_t;
-           typedef unsigned __int32  uint32_t;
+            typedef unsigned __int32    __pyx_uintptr_t;
         #endif
     #endif
 #else
-   #include <stdint.h>
+    #include <stdint.h>
+    typedef uintptr_t  __pyx_uintptr_t;
 #endif
 #ifndef CYTHON_FALLTHROUGH
-  #if defined(__cplusplus) && __cplusplus >= 201103L
-    #if __has_cpp_attribute(fallthrough)
-      #define CYTHON_FALLTHROUGH [[fallthrough]]
-    #elif __has_cpp_attribute(clang::fallthrough)
-      #define CYTHON_FALLTHROUGH [[clang::fallthrough]]
-    #elif __has_cpp_attribute(gnu::fallthrough)
-      #define CYTHON_FALLTHROUGH [[gnu::fallthrough]]
+  #if defined(__cplusplus)
+    /* for clang __has_cpp_attribute(fallthrough) is true even before C++17
+     * but leads to warnings with -pedantic, since it is a C++17 feature */
+    #if ((defined(_MSVC_LANG) && _MSVC_LANG >= 201703L) || __cplusplus >= 201703L)
+      #if __has_cpp_attribute(fallthrough)
+        #define CYTHON_FALLTHROUGH [[fallthrough]]
+      #endif
+    #endif
+    #ifndef CYTHON_FALLTHROUGH
+      #if __has_cpp_attribute(clang::fallthrough)
+        #define CYTHON_FALLTHROUGH [[clang::fallthrough]]
+      #elif __has_cpp_attribute(gnu::fallthrough)
+        #define CYTHON_FALLTHROUGH [[gnu::fallthrough]]
+      #endif
     #endif
   #endif
   #ifndef CYTHON_FALLTHROUGH
     #if __has_attribute(fallthrough)
       #define CYTHON_FALLTHROUGH __attribute__((fallthrough))
     #else
       #define CYTHON_FALLTHROUGH
     #endif
   #endif
-  #if defined(__clang__ ) && defined(__apple_build_version__)
+  #if defined(__clang__) && defined(__apple_build_version__)
     #if __apple_build_version__ < 7000000
       #undef  CYTHON_FALLTHROUGH
       #define CYTHON_FALLTHROUGH
     #endif
   #endif
 #endif
+#ifdef __cplusplus
+  template <typename T>
+  struct __PYX_IS_UNSIGNED_IMPL {static const bool value = T(0) < T(-1);};
+  #define __PYX_IS_UNSIGNED(type) (__PYX_IS_UNSIGNED_IMPL<type>::value)
+#else
+  #define __PYX_IS_UNSIGNED(type) (((type)-1) > 0)
+#endif
+#if CYTHON_COMPILING_IN_PYPY == 1
+  #define __PYX_NEED_TP_PRINT_SLOT  (PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x030A0000)
+#else
+  #define __PYX_NEED_TP_PRINT_SLOT  (PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000)
+#endif
+#define __PYX_REINTERPRET_FUNCION(func_pointer, other_pointer) ((func_pointer)(void(*)(void))(other_pointer))
 
 #ifndef CYTHON_INLINE
   #if defined(__clang__)
     #define CYTHON_INLINE __inline__ __attribute__ ((__unused__))
   #elif defined(__GNUC__)
     #define CYTHON_INLINE __inline__
   #elif defined(_MSC_VER)
@@ -311,43 +541,40 @@
   #elif defined (__STDC_VERSION__) && __STDC_VERSION__ >= 199901L
     #define CYTHON_INLINE inline
   #else
     #define CYTHON_INLINE
   #endif
 #endif
 
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
-  #define Py_OptimizeFlag 0
-#endif
 #define __PYX_BUILD_PY_SSIZE_T "n"
 #define CYTHON_FORMAT_SSIZE_T "z"
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
-  #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
-          PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
   #define __Pyx_DefaultClassType PyClass_Type
+  #define __Pyx_PyCode_New(a, p, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
+          PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #else
   #define __Pyx_BUILTIN_MODULE_NAME "builtins"
   #define __Pyx_DefaultClassType PyType_Type
 #if PY_VERSION_HEX >= 0x030B00A1
-    static CYTHON_INLINE PyCodeObject* __Pyx_PyCode_New(int a, int k, int l, int s, int f,
+    static CYTHON_INLINE PyCodeObject* __Pyx_PyCode_New(int a, int p, int k, int l, int s, int f,
                                                     PyObject *code, PyObject *c, PyObject* n, PyObject *v,
                                                     PyObject *fv, PyObject *cell, PyObject* fn,
                                                     PyObject *name, int fline, PyObject *lnos) {
         PyObject *kwds=NULL, *argcount=NULL, *posonlyargcount=NULL, *kwonlyargcount=NULL;
-        PyObject *nlocals=NULL, *stacksize=NULL, *flags=NULL, *replace=NULL, *call_result=NULL, *empty=NULL;
+        PyObject *nlocals=NULL, *stacksize=NULL, *flags=NULL, *replace=NULL, *empty=NULL;
         const char *fn_cstr=NULL;
         const char *name_cstr=NULL;
-        PyCodeObject* co=NULL;
+        PyCodeObject *co=NULL, *result=NULL;
         PyObject *type, *value, *traceback;
         PyErr_Fetch(&type, &value, &traceback);
         if (!(kwds=PyDict_New())) goto end;
         if (!(argcount=PyLong_FromLong(a))) goto end;
         if (PyDict_SetItemString(kwds, "co_argcount", argcount) != 0) goto end;
-        if (!(posonlyargcount=PyLong_FromLong(0))) goto end;
+        if (!(posonlyargcount=PyLong_FromLong(p))) goto end;
         if (PyDict_SetItemString(kwds, "co_posonlyargcount", posonlyargcount) != 0) goto end;
         if (!(kwonlyargcount=PyLong_FromLong(k))) goto end;
         if (PyDict_SetItemString(kwds, "co_kwonlyargcount", kwonlyargcount) != 0) goto end;
         if (!(nlocals=PyLong_FromLong(l))) goto end;
         if (PyDict_SetItemString(kwds, "co_nlocals", nlocals) != 0) goto end;
         if (!(stacksize=PyLong_FromLong(s))) goto end;
         if (PyDict_SetItemString(kwds, "co_stacksize", stacksize) != 0) goto end;
@@ -359,104 +586,180 @@
         if (PyDict_SetItemString(kwds, "co_varnames", v) != 0) goto end;
         if (PyDict_SetItemString(kwds, "co_freevars", fv) != 0) goto end;
         if (PyDict_SetItemString(kwds, "co_cellvars", cell) != 0) goto end;
         if (PyDict_SetItemString(kwds, "co_linetable", lnos) != 0) goto end;
         if (!(fn_cstr=PyUnicode_AsUTF8AndSize(fn, NULL))) goto end;
         if (!(name_cstr=PyUnicode_AsUTF8AndSize(name, NULL))) goto end;
         if (!(co = PyCode_NewEmpty(fn_cstr, name_cstr, fline))) goto end;
-        if (!(replace = PyObject_GetAttrString((PyObject*)co, "replace"))) goto cleanup_code_too;
-        if (!(empty = PyTuple_New(0))) goto cleanup_code_too; // unfortunately __pyx_empty_tuple isn't available here
-        if (!(call_result = PyObject_Call(replace, empty, kwds))) goto cleanup_code_too;
-        Py_XDECREF((PyObject*)co);
-        co = (PyCodeObject*)call_result;
-        call_result = NULL;
-        if (0) {
-            cleanup_code_too:
-            Py_XDECREF((PyObject*)co);
-            co = NULL;
-        }
-        end:
+        if (!(replace = PyObject_GetAttrString((PyObject*)co, "replace"))) goto end;
+        if (!(empty = PyTuple_New(0))) goto end;
+        result = (PyCodeObject*) PyObject_Call(replace, empty, kwds);
+    end:
+        Py_XDECREF((PyObject*) co);
         Py_XDECREF(kwds);
         Py_XDECREF(argcount);
         Py_XDECREF(posonlyargcount);
         Py_XDECREF(kwonlyargcount);
         Py_XDECREF(nlocals);
         Py_XDECREF(stacksize);
         Py_XDECREF(replace);
-        Py_XDECREF(call_result);
         Py_XDECREF(empty);
         if (type) {
             PyErr_Restore(type, value, traceback);
         }
-        return co;
+        return result;
     }
+#elif PY_VERSION_HEX >= 0x030800B2 && !CYTHON_COMPILING_IN_PYPY
+  #define __Pyx_PyCode_New(a, p, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
+          PyCode_NewWithPosOnlyArgs(a, p, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #else
-  #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
+  #define __Pyx_PyCode_New(a, p, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #endif
-  #define __Pyx_DefaultClassType PyType_Type
+#endif
+#if PY_VERSION_HEX >= 0x030900A4 || defined(Py_IS_TYPE)
+  #define __Pyx_IS_TYPE(ob, type) Py_IS_TYPE(ob, type)
+#else
+  #define __Pyx_IS_TYPE(ob, type) (((const PyObject*)ob)->ob_type == (type))
+#endif
+#if PY_VERSION_HEX >= 0x030A00B1 || defined(Py_Is)
+  #define __Pyx_Py_Is(x, y)  Py_Is(x, y)
+#else
+  #define __Pyx_Py_Is(x, y) ((x) == (y))
+#endif
+#if PY_VERSION_HEX >= 0x030A00B1 || defined(Py_IsNone)
+  #define __Pyx_Py_IsNone(ob) Py_IsNone(ob)
+#else
+  #define __Pyx_Py_IsNone(ob) __Pyx_Py_Is((ob), Py_None)
+#endif
+#if PY_VERSION_HEX >= 0x030A00B1 || defined(Py_IsTrue)
+  #define __Pyx_Py_IsTrue(ob) Py_IsTrue(ob)
+#else
+  #define __Pyx_Py_IsTrue(ob) __Pyx_Py_Is((ob), Py_True)
+#endif
+#if PY_VERSION_HEX >= 0x030A00B1 || defined(Py_IsFalse)
+  #define __Pyx_Py_IsFalse(ob) Py_IsFalse(ob)
+#else
+  #define __Pyx_Py_IsFalse(ob) __Pyx_Py_Is((ob), Py_False)
+#endif
+#define __Pyx_NoneAsNull(obj)  (__Pyx_Py_IsNone(obj) ? NULL : (obj))
+#if PY_VERSION_HEX >= 0x030900F0 && !CYTHON_COMPILING_IN_PYPY
+  #define __Pyx_PyObject_GC_IsFinalized(o) PyObject_GC_IsFinalized(o)
+#else
+  #define __Pyx_PyObject_GC_IsFinalized(o) _PyGC_FINALIZED(o)
+#endif
+#ifndef CO_COROUTINE
+  #define CO_COROUTINE 0x80
+#endif
+#ifndef CO_ASYNC_GENERATOR
+  #define CO_ASYNC_GENERATOR 0x200
 #endif
 #ifndef Py_TPFLAGS_CHECKTYPES
   #define Py_TPFLAGS_CHECKTYPES 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_INDEX
   #define Py_TPFLAGS_HAVE_INDEX 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_NEWBUFFER
   #define Py_TPFLAGS_HAVE_NEWBUFFER 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_FINALIZE
   #define Py_TPFLAGS_HAVE_FINALIZE 0
 #endif
+#ifndef Py_TPFLAGS_SEQUENCE
+  #define Py_TPFLAGS_SEQUENCE 0
+#endif
+#ifndef Py_TPFLAGS_MAPPING
+  #define Py_TPFLAGS_MAPPING 0
+#endif
 #ifndef METH_STACKLESS
   #define METH_STACKLESS 0
 #endif
 #if PY_VERSION_HEX <= 0x030700A3 || !defined(METH_FASTCALL)
   #ifndef METH_FASTCALL
      #define METH_FASTCALL 0x80
   #endif
   typedef PyObject *(*__Pyx_PyCFunctionFast) (PyObject *self, PyObject *const *args, Py_ssize_t nargs);
   typedef PyObject *(*__Pyx_PyCFunctionFastWithKeywords) (PyObject *self, PyObject *const *args,
                                                           Py_ssize_t nargs, PyObject *kwnames);
 #else
   #define __Pyx_PyCFunctionFast _PyCFunctionFast
   #define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
 #endif
-#if CYTHON_FAST_PYCCALL
-#define __Pyx_PyFastCFunction_Check(func)\
-    ((PyCFunction_Check(func) && (METH_FASTCALL == (PyCFunction_GET_FLAGS(func) & ~(METH_CLASS | METH_STATIC | METH_COEXIST | METH_KEYWORDS | METH_STACKLESS)))))
+#if CYTHON_METH_FASTCALL
+  #define __Pyx_METH_FASTCALL METH_FASTCALL
+  #define __Pyx_PyCFunction_FastCall __Pyx_PyCFunctionFast
+  #define __Pyx_PyCFunction_FastCallWithKeywords __Pyx_PyCFunctionFastWithKeywords
+#else
+  #define __Pyx_METH_FASTCALL METH_VARARGS
+  #define __Pyx_PyCFunction_FastCall PyCFunction
+  #define __Pyx_PyCFunction_FastCallWithKeywords PyCFunctionWithKeywords
+#endif
+#if CYTHON_VECTORCALL
+  #define __pyx_vectorcallfunc vectorcallfunc
+  #define __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET  PY_VECTORCALL_ARGUMENTS_OFFSET
+  #define __Pyx_PyVectorcall_NARGS(n)  PyVectorcall_NARGS((size_t)(n))
+#elif CYTHON_BACKPORT_VECTORCALL
+  typedef PyObject *(*__pyx_vectorcallfunc)(PyObject *callable, PyObject *const *args,
+                                            size_t nargsf, PyObject *kwnames);
+  #define __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET  ((size_t)1 << (8 * sizeof(size_t) - 1))
+  #define __Pyx_PyVectorcall_NARGS(n)  ((Py_ssize_t)(((size_t)(n)) & ~__Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET))
+#else
+  #define __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET  0
+  #define __Pyx_PyVectorcall_NARGS(n)  ((Py_ssize_t)(n))
+#endif
+#if PY_VERSION_HEX < 0x030900B1
+  #define __Pyx_PyType_FromModuleAndSpec(m, s, b)  ((void)m, PyType_FromSpecWithBases(s, b))
+  typedef PyObject *(*__Pyx_PyCMethod)(PyObject *, PyTypeObject *, PyObject *const *, size_t, PyObject *);
 #else
-#define __Pyx_PyFastCFunction_Check(func) 0
+  #define __Pyx_PyType_FromModuleAndSpec(m, s, b)  PyType_FromModuleAndSpec(m, s, b)
+  #define __Pyx_PyCMethod  PyCMethod
+#endif
+#ifndef METH_METHOD
+  #define METH_METHOD 0x200
 #endif
 #if CYTHON_COMPILING_IN_PYPY && !defined(PyObject_Malloc)
   #define PyObject_Malloc(s)   PyMem_Malloc(s)
   #define PyObject_Free(p)     PyMem_Free(p)
   #define PyObject_Realloc(p)  PyMem_Realloc(p)
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030400A1
-  #define PyMem_RawMalloc(n)           PyMem_Malloc(n)
-  #define PyMem_RawRealloc(p, n)       PyMem_Realloc(p, n)
-  #define PyMem_RawFree(p)             PyMem_Free(p)
-#endif
-#if CYTHON_COMPILING_IN_PYSTON
-  #define __Pyx_PyCode_HasFreeVars(co)  PyCode_HasFreeVars(co)
-  #define __Pyx_PyFrame_SetLineNumber(frame, lineno) PyFrame_SetLineNumber(frame, lineno)
+#if CYTHON_COMPILING_IN_LIMITED_API
+  #define __Pyx_PyCode_HasFreeVars(co)  (PyCode_GetNumFree(co) > 0)
+  #define __Pyx_PyFrame_SetLineNumber(frame, lineno)
 #else
   #define __Pyx_PyCode_HasFreeVars(co)  (PyCode_GetNumFree(co) > 0)
   #define __Pyx_PyFrame_SetLineNumber(frame, lineno)  (frame)->f_lineno = (lineno)
 #endif
-#if !CYTHON_FAST_THREAD_STATE || PY_VERSION_HEX < 0x02070000
+#if CYTHON_COMPILING_IN_LIMITED_API
+  #define __Pyx_PyThreadState_Current PyThreadState_Get()
+#elif !CYTHON_FAST_THREAD_STATE
   #define __Pyx_PyThreadState_Current PyThreadState_GET()
 #elif PY_VERSION_HEX >= 0x03060000
   #define __Pyx_PyThreadState_Current _PyThreadState_UncheckedGet()
 #elif PY_VERSION_HEX >= 0x03000000
   #define __Pyx_PyThreadState_Current PyThreadState_GET()
 #else
   #define __Pyx_PyThreadState_Current _PyThreadState_Current
 #endif
+#if CYTHON_COMPILING_IN_LIMITED_API
+static CYTHON_INLINE void *__Pyx_PyModule_GetState(PyObject *op)
+{
+    void *result;
+    result = PyModule_GetState(op);
+    if (!result)
+        Py_FatalError("Couldn't find the module state");
+    return result;
+}
+#endif
+#define __Pyx_PyObject_GetSlot(obj, name, func_ctype)  __Pyx_PyType_GetSlot(Py_TYPE(obj), name, func_ctype)
+#if CYTHON_COMPILING_IN_LIMITED_API
+  #define __Pyx_PyType_GetSlot(type, name, func_ctype)  ((func_ctype) PyType_GetSlot((type), Py_##name))
+#else
+  #define __Pyx_PyType_GetSlot(type, name, func_ctype)  ((type)->name)
+#endif
 #if PY_VERSION_HEX < 0x030700A2 && !defined(PyThread_tss_create) && !defined(Py_tss_NEEDS_INIT)
 #include "pythread.h"
 #define Py_tss_NEEDS_INIT 0
 typedef int Py_tss_t;
 static CYTHON_INLINE int PyThread_tss_create(Py_tss_t *key) {
   *key = PyThread_create_key();
   return 0;
@@ -479,86 +782,166 @@
 static CYTHON_INLINE int PyThread_tss_set(Py_tss_t *key, void *value) {
   return PyThread_set_key_value(*key, value);
 }
 static CYTHON_INLINE void * PyThread_tss_get(Py_tss_t *key) {
   return PyThread_get_key_value(*key);
 }
 #endif
+#if PY_MAJOR_VERSION < 3
+    #if CYTHON_COMPILING_IN_PYPY
+        #if PYPY_VERSION_NUM < 0x07030600
+            #if defined(__cplusplus) && __cplusplus >= 201402L
+                [[deprecated("`with nogil:` inside a nogil function will not release the GIL in PyPy2 < 7.3.6")]]
+            #elif defined(__GNUC__) || defined(__clang__)
+                __attribute__ ((__deprecated__("`with nogil:` inside a nogil function will not release the GIL in PyPy2 < 7.3.6")))
+            #elif defined(_MSC_VER)
+                __declspec(deprecated("`with nogil:` inside a nogil function will not release the GIL in PyPy2 < 7.3.6"))
+            #endif
+            static CYTHON_INLINE int PyGILState_Check(void) {
+                return 0;
+            }
+        #else  // PYPY_VERSION_NUM < 0x07030600
+        #endif  // PYPY_VERSION_NUM < 0x07030600
+    #else
+        static CYTHON_INLINE int PyGILState_Check(void) {
+            PyThreadState * tstate = _PyThreadState_Current;
+            return tstate && (tstate == PyGILState_GetThisThreadState());
+        }
+    #endif
+#endif
 #if CYTHON_COMPILING_IN_CPYTHON || defined(_PyDict_NewPresized)
 #define __Pyx_PyDict_NewPresized(n)  ((n <= 8) ? PyDict_New() : _PyDict_NewPresized(n))
 #else
 #define __Pyx_PyDict_NewPresized(n)  PyDict_New()
 #endif
 #if PY_MAJOR_VERSION >= 3 || CYTHON_FUTURE_DIVISION
   #define __Pyx_PyNumber_Divide(x,y)         PyNumber_TrueDivide(x,y)
   #define __Pyx_PyNumber_InPlaceDivide(x,y)  PyNumber_InPlaceTrueDivide(x,y)
 #else
   #define __Pyx_PyNumber_Divide(x,y)         PyNumber_Divide(x,y)
   #define __Pyx_PyNumber_InPlaceDivide(x,y)  PyNumber_InPlaceDivide(x,y)
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1 && CYTHON_USE_UNICODE_INTERNALS
-#define __Pyx_PyDict_GetItemStr(dict, name)  _PyDict_GetItem_KnownHash(dict, name, ((PyASCIIObject *) name)->hash)
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX > 0x030600B4 && CYTHON_USE_UNICODE_INTERNALS
+#define __Pyx_PyDict_GetItemStrWithError(dict, name)  _PyDict_GetItem_KnownHash(dict, name, ((PyASCIIObject *) name)->hash)
+static CYTHON_INLINE PyObject * __Pyx_PyDict_GetItemStr(PyObject *dict, PyObject *name) {
+    PyObject *res = __Pyx_PyDict_GetItemStrWithError(dict, name);
+    if (res == NULL) PyErr_Clear();
+    return res;
+}
+#elif PY_MAJOR_VERSION >= 3 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07020000)
+#define __Pyx_PyDict_GetItemStrWithError  PyDict_GetItemWithError
+#define __Pyx_PyDict_GetItemStr           PyDict_GetItem
+#else
+static CYTHON_INLINE PyObject * __Pyx_PyDict_GetItemStrWithError(PyObject *dict, PyObject *name) {
+#if CYTHON_COMPILING_IN_PYPY
+    return PyDict_GetItem(dict, name);
 #else
-#define __Pyx_PyDict_GetItemStr(dict, name)  PyDict_GetItem(dict, name)
+    PyDictEntry *ep;
+    PyDictObject *mp = (PyDictObject*) dict;
+    long hash = ((PyStringObject *) name)->ob_shash;
+    assert(hash != -1);
+    ep = (mp->ma_lookup)(mp, name, hash);
+    if (ep == NULL) {
+        return NULL;
+    }
+    return ep->me_value;
+#endif
+}
+#define __Pyx_PyDict_GetItemStr           PyDict_GetItem
 #endif
-#if PY_VERSION_HEX > 0x03030000 && defined(PyUnicode_KIND)
+#if CYTHON_USE_TYPE_SLOTS
+  #define __Pyx_PyType_GetFlags(tp)   (((PyTypeObject *)tp)->tp_flags)
+  #define __Pyx_PyType_HasFeature(type, feature)  ((__Pyx_PyType_GetFlags(type) & (feature)) != 0)
+  #define __Pyx_PyObject_GetIterNextFunc(obj)  (Py_TYPE(obj)->tp_iternext)
+#else
+  #define __Pyx_PyType_GetFlags(tp)   (PyType_GetFlags((PyTypeObject *)tp))
+  #define __Pyx_PyType_HasFeature(type, feature)  PyType_HasFeature(type, feature)
+  #define __Pyx_PyObject_GetIterNextFunc(obj)  PyIter_Next
+#endif
+#if CYTHON_USE_TYPE_SPECS && PY_VERSION_HEX >= 0x03080000
+#define __Pyx_PyHeapTypeObject_GC_Del(obj)  {\
+    PyTypeObject *type = Py_TYPE(obj);\
+    assert(__Pyx_PyType_HasFeature(type, Py_TPFLAGS_HEAPTYPE));\
+    PyObject_GC_Del(obj);\
+    Py_DECREF(type);\
+}
+#else
+#define __Pyx_PyHeapTypeObject_GC_Del(obj)  PyObject_GC_Del(obj)
+#endif
+#if CYTHON_COMPILING_IN_LIMITED_API
   #define CYTHON_PEP393_ENABLED 1
-  #if defined(PyUnicode_IS_READY)
-  #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
-                                              0 : _PyUnicode_Ready((PyObject *)(op)))
-  #else
   #define __Pyx_PyUnicode_READY(op)       (0)
+  #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GetLength(u)
+  #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_ReadChar(u, i)
+  #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   ((void)u, 1114111U)
+  #define __Pyx_PyUnicode_KIND(u)         ((void)u, (0))
+  #define __Pyx_PyUnicode_DATA(u)         ((void*)u)
+  #define __Pyx_PyUnicode_READ(k, d, i)   ((void)k, PyUnicode_ReadChar((PyObject*)(d), i))
+  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GetLength(u))
+#elif PY_VERSION_HEX > 0x03030000 && defined(PyUnicode_KIND)
+  #define CYTHON_PEP393_ENABLED 1
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_READY(op)       (0)
+  #else
+    #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
+                                                0 : _PyUnicode_Ready((PyObject *)(op)))
   #endif
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_LENGTH(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_READ_CHAR(u, i)
   #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   PyUnicode_MAX_CHAR_VALUE(u)
-  #define __Pyx_PyUnicode_KIND(u)         PyUnicode_KIND(u)
+  #define __Pyx_PyUnicode_KIND(u)         ((int)PyUnicode_KIND(u))
   #define __Pyx_PyUnicode_DATA(u)         PyUnicode_DATA(u)
   #define __Pyx_PyUnicode_READ(k, d, i)   PyUnicode_READ(k, d, i)
-  #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, ch)
-  #if defined(PyUnicode_IS_READY) && defined(PyUnicode_GET_SIZE)
-  #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
-  #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
-  #endif
+  #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, (Py_UCS4) ch)
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
   #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
+    #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
+    #else
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
+    #endif
   #endif
 #else
   #define CYTHON_PEP393_ENABLED 0
   #define PyUnicode_1BYTE_KIND  1
   #define PyUnicode_2BYTE_KIND  2
   #define PyUnicode_4BYTE_KIND  4
   #define __Pyx_PyUnicode_READY(op)       (0)
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_SIZE(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) ((Py_UCS4)(PyUnicode_AS_UNICODE(u)[i]))
-  #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   ((sizeof(Py_UNICODE) == 2) ? 65535 : 1114111)
-  #define __Pyx_PyUnicode_KIND(u)         (sizeof(Py_UNICODE))
+  #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   ((sizeof(Py_UNICODE) == 2) ? 65535U : 1114111U)
+  #define __Pyx_PyUnicode_KIND(u)         ((int)sizeof(Py_UNICODE))
   #define __Pyx_PyUnicode_DATA(u)         ((void*)PyUnicode_AS_UNICODE(u))
   #define __Pyx_PyUnicode_READ(k, d, i)   ((void)(k), (Py_UCS4)(((Py_UNICODE*)d)[i]))
-  #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  (((void)(k)), ((Py_UNICODE*)d)[i] = ch)
+  #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  (((void)(k)), ((Py_UNICODE*)d)[i] = (Py_UNICODE) ch)
   #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_SIZE(u))
 #endif
 #if CYTHON_COMPILING_IN_PYPY
   #define __Pyx_PyUnicode_Concat(a, b)      PyNumber_Add(a, b)
   #define __Pyx_PyUnicode_ConcatSafe(a, b)  PyNumber_Add(a, b)
 #else
   #define __Pyx_PyUnicode_Concat(a, b)      PyUnicode_Concat(a, b)
   #define __Pyx_PyUnicode_ConcatSafe(a, b)  ((unlikely((a) == Py_None) || unlikely((b) == Py_None)) ?\
       PyNumber_Add(a, b) : __Pyx_PyUnicode_Concat(a, b))
 #endif
-#if CYTHON_COMPILING_IN_PYPY && !defined(PyUnicode_Contains)
-  #define PyUnicode_Contains(u, s)  PySequence_Contains(u, s)
-#endif
-#if CYTHON_COMPILING_IN_PYPY && !defined(PyByteArray_Check)
-  #define PyByteArray_Check(obj)  PyObject_TypeCheck(obj, &PyByteArray_Type)
-#endif
-#if CYTHON_COMPILING_IN_PYPY && !defined(PyObject_Format)
-  #define PyObject_Format(obj, fmt)  PyObject_CallMethod(obj, "__format__", "O", fmt)
+#if CYTHON_COMPILING_IN_PYPY
+  #if !defined(PyUnicode_DecodeUnicodeEscape)
+    #define PyUnicode_DecodeUnicodeEscape(s, size, errors)  PyUnicode_Decode(s, size, "unicode_escape", errors)
+  #endif
+  #if !defined(PyUnicode_Contains) || (PY_MAJOR_VERSION == 2 && PYPY_VERSION_NUM < 0x07030500)
+    #undef PyUnicode_Contains
+    #define PyUnicode_Contains(u, s)  PySequence_Contains(u, s)
+  #endif
+  #if !defined(PyByteArray_Check)
+    #define PyByteArray_Check(obj)  PyObject_TypeCheck(obj, &PyByteArray_Type)
+  #endif
+  #if !defined(PyObject_Format)
+    #define PyObject_Format(obj, fmt)  PyObject_CallMethod(obj, "__format__", "O", fmt)
+  #endif
 #endif
 #define __Pyx_PyString_FormatSafe(a, b)   ((unlikely((a) == Py_None || (PyString_Check(b) && !PyString_CheckExact(b)))) ? PyNumber_Remainder(a, b) : __Pyx_PyString_Format(a, b))
 #define __Pyx_PyUnicode_FormatSafe(a, b)  ((unlikely((a) == Py_None || (PyUnicode_Check(b) && !PyUnicode_CheckExact(b)))) ? PyNumber_Remainder(a, b) : PyUnicode_Format(a, b))
 #if PY_MAJOR_VERSION >= 3
   #define __Pyx_PyString_Format(a, b)  PyUnicode_Format(a, b)
 #else
   #define __Pyx_PyString_Format(a, b)  PyString_Format(a, b)
@@ -579,16 +962,22 @@
 #if PY_MAJOR_VERSION >= 3
   #define __Pyx_PyBaseString_Check(obj) PyUnicode_Check(obj)
   #define __Pyx_PyBaseString_CheckExact(obj) PyUnicode_CheckExact(obj)
 #else
   #define __Pyx_PyBaseString_Check(obj) (PyString_Check(obj) || PyUnicode_Check(obj))
   #define __Pyx_PyBaseString_CheckExact(obj) (PyString_CheckExact(obj) || PyUnicode_CheckExact(obj))
 #endif
+#if CYTHON_COMPILING_IN_CPYTHON
+  #define __Pyx_PySequence_ListKeepNew(obj)\
+    (likely(PyList_CheckExact(obj) && Py_REFCNT(obj) == 1) ? __Pyx_NewRef(obj) : PySequence_List(obj))
+#else
+  #define __Pyx_PySequence_ListKeepNew(obj)  PySequence_List(obj)
+#endif
 #ifndef PySet_CheckExact
-  #define PySet_CheckExact(obj)        (Py_TYPE(obj) == &PySet_Type)
+  #define PySet_CheckExact(obj)        __Pyx_IS_TYPE(obj, &PySet_Type)
 #endif
 #if PY_VERSION_HEX >= 0x030900A4
   #define __Pyx_SET_REFCNT(obj, refcnt) Py_SET_REFCNT(obj, refcnt)
   #define __Pyx_SET_SIZE(obj, size) Py_SET_SIZE(obj, size)
 #else
   #define __Pyx_SET_REFCNT(obj, refcnt) Py_REFCNT(obj) = (refcnt)
   #define __Pyx_SET_SIZE(obj, size) Py_SIZE(obj) = (size)
@@ -599,25 +988,30 @@
   #define __Pyx_PySequence_SIZE(seq)  PySequence_Size(seq)
 #endif
 #if PY_MAJOR_VERSION >= 3
   #define PyIntObject                  PyLongObject
   #define PyInt_Type                   PyLong_Type
   #define PyInt_Check(op)              PyLong_Check(op)
   #define PyInt_CheckExact(op)         PyLong_CheckExact(op)
+  #define __Pyx_Py3Int_Check(op)       PyLong_Check(op)
+  #define __Pyx_Py3Int_CheckExact(op)  PyLong_CheckExact(op)
   #define PyInt_FromString             PyLong_FromString
   #define PyInt_FromUnicode            PyLong_FromUnicode
   #define PyInt_FromLong               PyLong_FromLong
   #define PyInt_FromSize_t             PyLong_FromSize_t
   #define PyInt_FromSsize_t            PyLong_FromSsize_t
   #define PyInt_AsLong                 PyLong_AsLong
   #define PyInt_AS_LONG                PyLong_AS_LONG
   #define PyInt_AsSsize_t              PyLong_AsSsize_t
   #define PyInt_AsUnsignedLongMask     PyLong_AsUnsignedLongMask
   #define PyInt_AsUnsignedLongLongMask PyLong_AsUnsignedLongLongMask
   #define PyNumber_Int                 PyNumber_Long
+#else
+  #define __Pyx_Py3Int_Check(op)       (PyLong_Check(op) || PyInt_Check(op))
+  #define __Pyx_Py3Int_CheckExact(op)  (PyLong_CheckExact(op) || PyInt_CheckExact(op))
 #endif
 #if PY_MAJOR_VERSION >= 3
   #define PyBoolObject                 PyLongObject
 #endif
 #if PY_MAJOR_VERSION >= 3 && CYTHON_COMPILING_IN_PYPY
   #ifndef PyUnicode_InternFromString
     #define PyUnicode_InternFromString(s) PyUnicode_FromString(s)
@@ -627,19 +1021,14 @@
   typedef long Py_hash_t;
   #define __Pyx_PyInt_FromHash_t PyInt_FromLong
   #define __Pyx_PyInt_AsHash_t   __Pyx_PyIndex_AsHash_t
 #else
   #define __Pyx_PyInt_FromHash_t PyInt_FromSsize_t
   #define __Pyx_PyInt_AsHash_t   __Pyx_PyIndex_AsSsize_t
 #endif
-#if PY_MAJOR_VERSION >= 3
-  #define __Pyx_PyMethod_New(func, self, klass) ((self) ? ((void)(klass), PyMethod_New(func, self)) : __Pyx_NewRef(func))
-#else
-  #define __Pyx_PyMethod_New(func, self, klass) PyMethod_New(func, self, klass)
-#endif
 #if CYTHON_USE_ASYNC_SLOTS
   #if PY_VERSION_HEX >= 0x030500B1
     #define __Pyx_PyAsyncMethodsStruct PyAsyncMethods
     #define __Pyx_PyType_AsAsync(obj) (Py_TYPE(obj)->tp_as_async)
   #else
     #define __Pyx_PyType_AsAsync(obj) ((__Pyx_PyAsyncMethodsStruct*) (Py_TYPE(obj)->tp_reserved))
   #endif
@@ -650,16 +1039,18 @@
     typedef struct {
         unaryfunc am_await;
         unaryfunc am_aiter;
         unaryfunc am_anext;
     } __Pyx_PyAsyncMethodsStruct;
 #endif
 
-#if defined(WIN32) || defined(MS_WINDOWS)
-  #define _USE_MATH_DEFINES
+#if defined(_WIN32) || defined(WIN32) || defined(MS_WINDOWS)
+  #if !defined(_USE_MATH_DEFINES)
+    #define _USE_MATH_DEFINES
+  #endif
 #endif
 #include <math.h>
 #ifdef NAN
 #define __PYX_NAN() ((float) NAN)
 #else
 static CYTHON_INLINE float __PYX_NAN() {
   float value;
@@ -674,15 +1065,24 @@
 #endif
 
 #define __PYX_MARK_ERR_POS(f_index, lineno) \
     { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__; (void)__pyx_clineno; }
 #define __PYX_ERR(f_index, lineno, Ln_error) \
     { __PYX_MARK_ERR_POS(f_index, lineno) goto Ln_error; }
 
-#ifndef __PYX_EXTERN_C
+#ifdef CYTHON_EXTERN_C
+    #undef __PYX_EXTERN_C
+    #define __PYX_EXTERN_C CYTHON_EXTERN_C
+#elif defined(__PYX_EXTERN_C)
+    #ifdef _MSC_VER
+    #pragma message ("Please do not define the '__PYX_EXTERN_C' macro externally. Use 'CYTHON_EXTERN_C' instead.")
+    #else
+    #warning Please do not define the '__PYX_EXTERN_C' macro externally. Use 'CYTHON_EXTERN_C' instead.
+    #endif
+#else
   #ifdef __cplusplus
     #define __PYX_EXTERN_C extern "C"
   #else
     #define __PYX_EXTERN_C extern
   #endif
 #endif
 
@@ -760,29 +1160,40 @@
 #endif
 #define __Pyx_PyBytes_AsWritableString(s)     ((char*) PyBytes_AS_STRING(s))
 #define __Pyx_PyBytes_AsWritableSString(s)    ((signed char*) PyBytes_AS_STRING(s))
 #define __Pyx_PyBytes_AsWritableUString(s)    ((unsigned char*) PyBytes_AS_STRING(s))
 #define __Pyx_PyBytes_AsString(s)     ((const char*) PyBytes_AS_STRING(s))
 #define __Pyx_PyBytes_AsSString(s)    ((const signed char*) PyBytes_AS_STRING(s))
 #define __Pyx_PyBytes_AsUString(s)    ((const unsigned char*) PyBytes_AS_STRING(s))
-#define __Pyx_PyObject_AsWritableString(s)    ((char*) __Pyx_PyObject_AsString(s))
-#define __Pyx_PyObject_AsWritableSString(s)    ((signed char*) __Pyx_PyObject_AsString(s))
-#define __Pyx_PyObject_AsWritableUString(s)    ((unsigned char*) __Pyx_PyObject_AsString(s))
+#define __Pyx_PyObject_AsWritableString(s)    ((char*)(__pyx_uintptr_t) __Pyx_PyObject_AsString(s))
+#define __Pyx_PyObject_AsWritableSString(s)    ((signed char*)(__pyx_uintptr_t) __Pyx_PyObject_AsString(s))
+#define __Pyx_PyObject_AsWritableUString(s)    ((unsigned char*)(__pyx_uintptr_t) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_AsSString(s)    ((const signed char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_AsUString(s)    ((const unsigned char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_FromCString(s)  __Pyx_PyObject_FromString((const char*)s)
 #define __Pyx_PyBytes_FromCString(s)   __Pyx_PyBytes_FromString((const char*)s)
 #define __Pyx_PyByteArray_FromCString(s)   __Pyx_PyByteArray_FromString((const char*)s)
 #define __Pyx_PyStr_FromCString(s)     __Pyx_PyStr_FromString((const char*)s)
 #define __Pyx_PyUnicode_FromCString(s) __Pyx_PyUnicode_FromString((const char*)s)
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const Py_UNICODE *u) {
+#if CYTHON_COMPILING_IN_LIMITED_API
+static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const wchar_t *u)
+{
+    const wchar_t *u_end = u;
+    while (*u_end++) ;
+    return (size_t)(u_end - u - 1);
+}
+#else
+static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const Py_UNICODE *u)
+{
     const Py_UNICODE *u_end = u;
     while (*u_end++) ;
     return (size_t)(u_end - u - 1);
 }
+#endif
+#define __Pyx_PyUnicode_FromOrdinal(o)       PyUnicode_FromOrdinal((int)o)
 #define __Pyx_PyUnicode_FromUnicode(u)       PyUnicode_FromUnicode(u, __Pyx_Py_UNICODE_strlen(u))
 #define __Pyx_PyUnicode_FromUnicodeAndLength PyUnicode_FromUnicode
 #define __Pyx_PyUnicode_AsUnicode            PyUnicode_AsUnicode
 #define __Pyx_NewRef(obj) (Py_INCREF(obj), obj)
 #define __Pyx_Owned_Py_None(b) __Pyx_NewRef(Py_None)
 static CYTHON_INLINE PyObject * __Pyx_PyBool_FromLong(long b);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrue(PyObject*);
@@ -800,15 +1211,60 @@
 #endif
 #define __pyx_PyFloat_AsFloat(x) ((float) __pyx_PyFloat_AsDouble(x))
 #if PY_MAJOR_VERSION >= 3
 #define __Pyx_PyNumber_Int(x) (PyLong_CheckExact(x) ? __Pyx_NewRef(x) : PyNumber_Long(x))
 #else
 #define __Pyx_PyNumber_Int(x) (PyInt_CheckExact(x) ? __Pyx_NewRef(x) : PyNumber_Int(x))
 #endif
-#define __Pyx_PyNumber_Float(x) (PyFloat_CheckExact(x) ? __Pyx_NewRef(x) : PyNumber_Float(x))
+#if CYTHON_USE_PYLONG_INTERNALS
+  #if PY_VERSION_HEX >= 0x030C00A7
+  #ifndef _PyLong_SIGN_MASK
+    #define _PyLong_SIGN_MASK 3
+  #endif
+  #ifndef _PyLong_NON_SIZE_BITS
+    #define _PyLong_NON_SIZE_BITS 3
+  #endif
+  #define __Pyx_PyLong_Sign(x)  (((PyLongObject*)x)->long_value.lv_tag & _PyLong_SIGN_MASK)
+  #define __Pyx_PyLong_IsNeg(x)  ((__Pyx_PyLong_Sign(x) & 2) != 0)
+  #define __Pyx_PyLong_IsNonNeg(x)  (!__Pyx_PyLong_IsNeg(x))
+  #define __Pyx_PyLong_IsZero(x)  (__Pyx_PyLong_Sign(x) & 1)
+  #define __Pyx_PyLong_IsPos(x)  (__Pyx_PyLong_Sign(x) == 0)
+  #define __Pyx_PyLong_CompactValueUnsigned(x)  (__Pyx_PyLong_Digits(x)[0])
+  #define __Pyx_PyLong_DigitCount(x)  ((Py_ssize_t) (((PyLongObject*)x)->long_value.lv_tag >> _PyLong_NON_SIZE_BITS))
+  #define __Pyx_PyLong_SignedDigitCount(x)\
+        ((1 - (Py_ssize_t) __Pyx_PyLong_Sign(x)) * __Pyx_PyLong_DigitCount(x))
+  #if defined(PyUnstable_Long_IsCompact) && defined(PyUnstable_Long_CompactValue)
+    #define __Pyx_PyLong_IsCompact(x)     PyUnstable_Long_IsCompact((PyLongObject*) x)
+    #define __Pyx_PyLong_CompactValue(x)  PyUnstable_Long_CompactValue((PyLongObject*) x)
+  #else
+    #define __Pyx_PyLong_IsCompact(x)     (((PyLongObject*)x)->long_value.lv_tag < (2 << _PyLong_NON_SIZE_BITS))
+    #define __Pyx_PyLong_CompactValue(x)  ((1 - (Py_ssize_t) __Pyx_PyLong_Sign(x)) * (Py_ssize_t) __Pyx_PyLong_Digits(x)[0])
+  #endif
+  typedef Py_ssize_t  __Pyx_compact_pylong;
+  typedef size_t  __Pyx_compact_upylong;
+  #else  // Py < 3.12
+  #define __Pyx_PyLong_IsNeg(x)  (Py_SIZE(x) < 0)
+  #define __Pyx_PyLong_IsNonNeg(x)  (Py_SIZE(x) >= 0)
+  #define __Pyx_PyLong_IsZero(x)  (Py_SIZE(x) == 0)
+  #define __Pyx_PyLong_IsPos(x)  (Py_SIZE(x) > 0)
+  #define __Pyx_PyLong_CompactValueUnsigned(x)  ((Py_SIZE(x) == 0) ? 0 : __Pyx_PyLong_Digits(x)[0])
+  #define __Pyx_PyLong_DigitCount(x)  __Pyx_sst_abs(Py_SIZE(x))
+  #define __Pyx_PyLong_SignedDigitCount(x)  Py_SIZE(x)
+  #define __Pyx_PyLong_IsCompact(x)  (Py_SIZE(x) == 0 || Py_SIZE(x) == 1 || Py_SIZE(x) == -1)
+  #define __Pyx_PyLong_CompactValue(x)\
+        ((Py_SIZE(x) == 0) ? (sdigit) 0 : ((Py_SIZE(x) < 0) ? -(sdigit)__Pyx_PyLong_Digits(x)[0] : (sdigit)__Pyx_PyLong_Digits(x)[0]))
+  typedef sdigit  __Pyx_compact_pylong;
+  typedef digit  __Pyx_compact_upylong;
+  #endif
+  #if PY_VERSION_HEX >= 0x030C00A5
+  #define __Pyx_PyLong_Digits(x)  (((PyLongObject*)x)->long_value.ob_digit)
+  #else
+  #define __Pyx_PyLong_Digits(x)  (((PyLongObject*)x)->ob_digit)
+  #endif
+#endif
 #if PY_MAJOR_VERSION < 3 && __PYX_DEFAULT_STRING_ENCODING_IS_ASCII
 static int __Pyx_sys_getdefaultencoding_not_ascii;
 static int __Pyx_init_sys_getdefaultencoding_params(void) {
     PyObject* sys;
     PyObject* default_encoding = NULL;
     PyObject* ascii_chars_u = NULL;
     PyObject* ascii_chars_b = NULL;
@@ -822,15 +1278,15 @@
     if (!default_encoding_c) goto bad;
     if (strcmp(default_encoding_c, "ascii") == 0) {
         __Pyx_sys_getdefaultencoding_not_ascii = 0;
     } else {
         char ascii_chars[128];
         int c;
         for (c = 0; c < 128; c++) {
-            ascii_chars[c] = c;
+            ascii_chars[c] = (char) c;
         }
         __Pyx_sys_getdefaultencoding_not_ascii = 1;
         ascii_chars_u = PyUnicode_DecodeASCII(ascii_chars, 128, NULL);
         if (!ascii_chars_u) goto bad;
         ascii_chars_b = PyUnicode_AsEncodedString(ascii_chars_u, default_encoding_c, NULL);
         if (!ascii_chars_b || !PyBytes_Check(ascii_chars_b) || memcmp(ascii_chars, PyBytes_AS_STRING(ascii_chars_b), 128) != 0) {
             PyErr_Format(
@@ -887,120 +1343,280 @@
   #define unlikely(x) __builtin_expect(!!(x), 0)
 #else /* !__GNUC__ or GCC < 2.95 */
   #define likely(x)   (x)
   #define unlikely(x) (x)
 #endif /* __GNUC__ */
 static CYTHON_INLINE void __Pyx_pretend_to_initialize(void* ptr) { (void)ptr; }
 
+#if !CYTHON_USE_MODULE_STATE
 static PyObject *__pyx_m = NULL;
-static PyObject *__pyx_d;
-static PyObject *__pyx_b;
-static PyObject *__pyx_cython_runtime = NULL;
-static PyObject *__pyx_empty_tuple;
-static PyObject *__pyx_empty_bytes;
-static PyObject *__pyx_empty_unicode;
+#endif
 static int __pyx_lineno;
 static int __pyx_clineno = 0;
-static const char * __pyx_cfilenm= __FILE__;
+static const char * __pyx_cfilenm = __FILE__;
 static const char *__pyx_filename;
 
+/* #### Code section: filename_table ### */
 
 static const char *__pyx_f[] = {
   "atimer/_atimer.pyx",
-  "stringsource",
+  "<stringsource>",
 };
+/* #### Code section: utility_code_proto_before_types ### */
+/* #### Code section: numeric_typedefs ### */
+/* #### Code section: complex_type_declarations ### */
+/* #### Code section: type_declarations ### */
 
 /*--- Type declarations ---*/
+/* #### Code section: utility_code_proto ### */
 
 /* --- Runtime support code (head) --- */
 /* Refnanny.proto */
 #ifndef CYTHON_REFNANNY
   #define CYTHON_REFNANNY 0
 #endif
 #if CYTHON_REFNANNY
   typedef struct {
-    void (*INCREF)(void*, PyObject*, int);
-    void (*DECREF)(void*, PyObject*, int);
-    void (*GOTREF)(void*, PyObject*, int);
-    void (*GIVEREF)(void*, PyObject*, int);
-    void* (*SetupContext)(const char*, int, const char*);
+    void (*INCREF)(void*, PyObject*, Py_ssize_t);
+    void (*DECREF)(void*, PyObject*, Py_ssize_t);
+    void (*GOTREF)(void*, PyObject*, Py_ssize_t);
+    void (*GIVEREF)(void*, PyObject*, Py_ssize_t);
+    void* (*SetupContext)(const char*, Py_ssize_t, const char*);
     void (*FinishContext)(void**);
   } __Pyx_RefNannyAPIStruct;
   static __Pyx_RefNannyAPIStruct *__Pyx_RefNanny = NULL;
   static __Pyx_RefNannyAPIStruct *__Pyx_RefNannyImportAPI(const char *modname);
   #define __Pyx_RefNannyDeclarations void *__pyx_refnanny = NULL;
 #ifdef WITH_THREAD
   #define __Pyx_RefNannySetupContext(name, acquire_gil)\
           if (acquire_gil) {\
               PyGILState_STATE __pyx_gilstate_save = PyGILState_Ensure();\
-              __pyx_refnanny = __Pyx_RefNanny->SetupContext((name), __LINE__, __FILE__);\
+              __pyx_refnanny = __Pyx_RefNanny->SetupContext((name), (__LINE__), (__FILE__));\
               PyGILState_Release(__pyx_gilstate_save);\
           } else {\
-              __pyx_refnanny = __Pyx_RefNanny->SetupContext((name), __LINE__, __FILE__);\
+              __pyx_refnanny = __Pyx_RefNanny->SetupContext((name), (__LINE__), (__FILE__));\
+          }
+  #define __Pyx_RefNannyFinishContextNogil() {\
+              PyGILState_STATE __pyx_gilstate_save = PyGILState_Ensure();\
+              __Pyx_RefNannyFinishContext();\
+              PyGILState_Release(__pyx_gilstate_save);\
           }
 #else
   #define __Pyx_RefNannySetupContext(name, acquire_gil)\
-          __pyx_refnanny = __Pyx_RefNanny->SetupContext((name), __LINE__, __FILE__)
+          __pyx_refnanny = __Pyx_RefNanny->SetupContext((name), (__LINE__), (__FILE__))
+  #define __Pyx_RefNannyFinishContextNogil() __Pyx_RefNannyFinishContext()
 #endif
+  #define __Pyx_RefNannyFinishContextNogil() {\
+              PyGILState_STATE __pyx_gilstate_save = PyGILState_Ensure();\
+              __Pyx_RefNannyFinishContext();\
+              PyGILState_Release(__pyx_gilstate_save);\
+          }
   #define __Pyx_RefNannyFinishContext()\
           __Pyx_RefNanny->FinishContext(&__pyx_refnanny)
-  #define __Pyx_INCREF(r)  __Pyx_RefNanny->INCREF(__pyx_refnanny, (PyObject *)(r), __LINE__)
-  #define __Pyx_DECREF(r)  __Pyx_RefNanny->DECREF(__pyx_refnanny, (PyObject *)(r), __LINE__)
-  #define __Pyx_GOTREF(r)  __Pyx_RefNanny->GOTREF(__pyx_refnanny, (PyObject *)(r), __LINE__)
-  #define __Pyx_GIVEREF(r) __Pyx_RefNanny->GIVEREF(__pyx_refnanny, (PyObject *)(r), __LINE__)
-  #define __Pyx_XINCREF(r)  do { if((r) != NULL) {__Pyx_INCREF(r); }} while(0)
-  #define __Pyx_XDECREF(r)  do { if((r) != NULL) {__Pyx_DECREF(r); }} while(0)
-  #define __Pyx_XGOTREF(r)  do { if((r) != NULL) {__Pyx_GOTREF(r); }} while(0)
-  #define __Pyx_XGIVEREF(r) do { if((r) != NULL) {__Pyx_GIVEREF(r);}} while(0)
+  #define __Pyx_INCREF(r)  __Pyx_RefNanny->INCREF(__pyx_refnanny, (PyObject *)(r), (__LINE__))
+  #define __Pyx_DECREF(r)  __Pyx_RefNanny->DECREF(__pyx_refnanny, (PyObject *)(r), (__LINE__))
+  #define __Pyx_GOTREF(r)  __Pyx_RefNanny->GOTREF(__pyx_refnanny, (PyObject *)(r), (__LINE__))
+  #define __Pyx_GIVEREF(r) __Pyx_RefNanny->GIVEREF(__pyx_refnanny, (PyObject *)(r), (__LINE__))
+  #define __Pyx_XINCREF(r)  do { if((r) == NULL); else {__Pyx_INCREF(r); }} while(0)
+  #define __Pyx_XDECREF(r)  do { if((r) == NULL); else {__Pyx_DECREF(r); }} while(0)
+  #define __Pyx_XGOTREF(r)  do { if((r) == NULL); else {__Pyx_GOTREF(r); }} while(0)
+  #define __Pyx_XGIVEREF(r) do { if((r) == NULL); else {__Pyx_GIVEREF(r);}} while(0)
 #else
   #define __Pyx_RefNannyDeclarations
   #define __Pyx_RefNannySetupContext(name, acquire_gil)
+  #define __Pyx_RefNannyFinishContextNogil()
   #define __Pyx_RefNannyFinishContext()
   #define __Pyx_INCREF(r) Py_INCREF(r)
   #define __Pyx_DECREF(r) Py_DECREF(r)
   #define __Pyx_GOTREF(r)
   #define __Pyx_GIVEREF(r)
   #define __Pyx_XINCREF(r) Py_XINCREF(r)
   #define __Pyx_XDECREF(r) Py_XDECREF(r)
   #define __Pyx_XGOTREF(r)
   #define __Pyx_XGIVEREF(r)
 #endif
+#define __Pyx_Py_XDECREF_SET(r, v) do {\
+        PyObject *tmp = (PyObject *) r;\
+        r = v; Py_XDECREF(tmp);\
+    } while (0)
 #define __Pyx_XDECREF_SET(r, v) do {\
         PyObject *tmp = (PyObject *) r;\
         r = v; __Pyx_XDECREF(tmp);\
     } while (0)
 #define __Pyx_DECREF_SET(r, v) do {\
         PyObject *tmp = (PyObject *) r;\
         r = v; __Pyx_DECREF(tmp);\
     } while (0)
 #define __Pyx_CLEAR(r)    do { PyObject* tmp = ((PyObject*)(r)); r = NULL; __Pyx_DECREF(tmp);} while(0)
 #define __Pyx_XCLEAR(r)   do { if((r) != NULL) {PyObject* tmp = ((PyObject*)(r)); r = NULL; __Pyx_DECREF(tmp);}} while(0)
 
-/* RaiseArgTupleInvalid.proto */
-static void __Pyx_RaiseArgtupleInvalid(const char* func_name, int exact,
-    Py_ssize_t num_min, Py_ssize_t num_max, Py_ssize_t num_found);
+/* PyErrExceptionMatches.proto */
+#if CYTHON_FAST_THREAD_STATE
+#define __Pyx_PyErr_ExceptionMatches(err) __Pyx_PyErr_ExceptionMatchesInState(__pyx_tstate, err)
+static CYTHON_INLINE int __Pyx_PyErr_ExceptionMatchesInState(PyThreadState* tstate, PyObject* err);
+#else
+#define __Pyx_PyErr_ExceptionMatches(err)  PyErr_ExceptionMatches(err)
+#endif
 
-/* RaiseDoubleKeywords.proto */
-static void __Pyx_RaiseDoubleKeywordsError(const char* func_name, PyObject* kw_name);
+/* PyThreadStateGet.proto */
+#if CYTHON_FAST_THREAD_STATE
+#define __Pyx_PyThreadState_declare  PyThreadState *__pyx_tstate;
+#define __Pyx_PyThreadState_assign  __pyx_tstate = __Pyx_PyThreadState_Current;
+#if PY_VERSION_HEX >= 0x030C00A6
+#define __Pyx_PyErr_Occurred()  (__pyx_tstate->current_exception != NULL)
+#define __Pyx_PyErr_CurrentExceptionType()  (__pyx_tstate->current_exception ? (PyObject*) Py_TYPE(__pyx_tstate->current_exception) : (PyObject*) NULL)
+#else
+#define __Pyx_PyErr_Occurred()  (__pyx_tstate->curexc_type != NULL)
+#define __Pyx_PyErr_CurrentExceptionType()  (__pyx_tstate->curexc_type)
+#endif
+#else
+#define __Pyx_PyThreadState_declare
+#define __Pyx_PyThreadState_assign
+#define __Pyx_PyErr_Occurred()  (PyErr_Occurred() != NULL)
+#define __Pyx_PyErr_CurrentExceptionType()  PyErr_Occurred()
+#endif
 
-/* ParseKeywords.proto */
-static int __Pyx_ParseOptionalKeywords(PyObject *kwds, PyObject **argnames[],\
-    PyObject *kwds2, PyObject *values[], Py_ssize_t num_pos_args,\
-    const char* function_name);
+/* PyErrFetchRestore.proto */
+#if CYTHON_FAST_THREAD_STATE
+#define __Pyx_PyErr_Clear() __Pyx_ErrRestore(NULL, NULL, NULL)
+#define __Pyx_ErrRestoreWithState(type, value, tb)  __Pyx_ErrRestoreInState(PyThreadState_GET(), type, value, tb)
+#define __Pyx_ErrFetchWithState(type, value, tb)    __Pyx_ErrFetchInState(PyThreadState_GET(), type, value, tb)
+#define __Pyx_ErrRestore(type, value, tb)  __Pyx_ErrRestoreInState(__pyx_tstate, type, value, tb)
+#define __Pyx_ErrFetch(type, value, tb)    __Pyx_ErrFetchInState(__pyx_tstate, type, value, tb)
+static CYTHON_INLINE void __Pyx_ErrRestoreInState(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb);
+static CYTHON_INLINE void __Pyx_ErrFetchInState(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A6
+#define __Pyx_PyErr_SetNone(exc) (Py_INCREF(exc), __Pyx_ErrRestore((exc), NULL, NULL))
+#else
+#define __Pyx_PyErr_SetNone(exc) PyErr_SetNone(exc)
+#endif
+#else
+#define __Pyx_PyErr_Clear() PyErr_Clear()
+#define __Pyx_PyErr_SetNone(exc) PyErr_SetNone(exc)
+#define __Pyx_ErrRestoreWithState(type, value, tb)  PyErr_Restore(type, value, tb)
+#define __Pyx_ErrFetchWithState(type, value, tb)  PyErr_Fetch(type, value, tb)
+#define __Pyx_ErrRestoreInState(tstate, type, value, tb)  PyErr_Restore(type, value, tb)
+#define __Pyx_ErrFetchInState(tstate, type, value, tb)  PyErr_Fetch(type, value, tb)
+#define __Pyx_ErrRestore(type, value, tb)  PyErr_Restore(type, value, tb)
+#define __Pyx_ErrFetch(type, value, tb)  PyErr_Fetch(type, value, tb)
+#endif
 
 /* PyObjectGetAttrStr.proto */
 #if CYTHON_USE_TYPE_SLOTS
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStr(PyObject* obj, PyObject* attr_name);
 #else
 #define __Pyx_PyObject_GetAttrStr(o,n) PyObject_GetAttr(o,n)
 #endif
 
+/* PyObjectGetAttrStrNoError.proto */
+static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name);
+
 /* GetBuiltinName.proto */
 static PyObject *__Pyx_GetBuiltinName(PyObject *name);
 
+/* DictGetItem.proto */
+#if PY_MAJOR_VERSION >= 3 && !CYTHON_COMPILING_IN_PYPY
+static PyObject *__Pyx_PyDict_GetItem(PyObject *d, PyObject* key);
+#define __Pyx_PyObject_Dict_GetItem(obj, name)\
+    (likely(PyDict_CheckExact(obj)) ?\
+     __Pyx_PyDict_GetItem(obj, name) : PyObject_GetItem(obj, name))
+#else
+#define __Pyx_PyDict_GetItem(d, key) PyObject_GetItem(d, key)
+#define __Pyx_PyObject_Dict_GetItem(obj, name)  PyObject_GetItem(obj, name)
+#endif
+
+/* GetTopmostException.proto */
+#if CYTHON_USE_EXC_INFO_STACK && CYTHON_FAST_THREAD_STATE
+static _PyErr_StackItem * __Pyx_PyErr_GetTopmostException(PyThreadState *tstate);
+#endif
+
+/* SaveResetException.proto */
+#if CYTHON_FAST_THREAD_STATE
+#define __Pyx_ExceptionSave(type, value, tb)  __Pyx__ExceptionSave(__pyx_tstate, type, value, tb)
+static CYTHON_INLINE void __Pyx__ExceptionSave(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
+#define __Pyx_ExceptionReset(type, value, tb)  __Pyx__ExceptionReset(__pyx_tstate, type, value, tb)
+static CYTHON_INLINE void __Pyx__ExceptionReset(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb);
+#else
+#define __Pyx_ExceptionSave(type, value, tb)   PyErr_GetExcInfo(type, value, tb)
+#define __Pyx_ExceptionReset(type, value, tb)  PyErr_SetExcInfo(type, value, tb)
+#endif
+
+/* GetException.proto */
+#if CYTHON_FAST_THREAD_STATE
+#define __Pyx_GetException(type, value, tb)  __Pyx__GetException(__pyx_tstate, type, value, tb)
+static int __Pyx__GetException(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
+#else
+static int __Pyx_GetException(PyObject **type, PyObject **value, PyObject **tb);
+#endif
+
+/* PyObjectCall.proto */
+#if CYTHON_COMPILING_IN_CPYTHON
+static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw);
+#else
+#define __Pyx_PyObject_Call(func, arg, kw) PyObject_Call(func, arg, kw)
+#endif
+
+/* RaiseException.proto */
+static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause);
+
+/* TupleAndListFromArray.proto */
+#if CYTHON_COMPILING_IN_CPYTHON
+static CYTHON_INLINE PyObject* __Pyx_PyList_FromArray(PyObject *const *src, Py_ssize_t n);
+static CYTHON_INLINE PyObject* __Pyx_PyTuple_FromArray(PyObject *const *src, Py_ssize_t n);
+#endif
+
+/* IncludeStringH.proto */
+#include <string.h>
+
+/* BytesEquals.proto */
+static CYTHON_INLINE int __Pyx_PyBytes_Equals(PyObject* s1, PyObject* s2, int equals);
+
+/* UnicodeEquals.proto */
+static CYTHON_INLINE int __Pyx_PyUnicode_Equals(PyObject* s1, PyObject* s2, int equals);
+
+/* fastcall.proto */
+#define __Pyx_Arg_VARARGS(args, i) PyTuple_GET_ITEM(args, i)
+#define __Pyx_NumKwargs_VARARGS(kwds) PyDict_Size(kwds)
+#define __Pyx_KwValues_VARARGS(args, nargs) NULL
+#define __Pyx_GetKwValue_VARARGS(kw, kwvalues, s) __Pyx_PyDict_GetItemStrWithError(kw, s)
+#define __Pyx_KwargsAsDict_VARARGS(kw, kwvalues) PyDict_Copy(kw)
+#if CYTHON_METH_FASTCALL
+    #define __Pyx_Arg_FASTCALL(args, i) args[i]
+    #define __Pyx_NumKwargs_FASTCALL(kwds) PyTuple_GET_SIZE(kwds)
+    #define __Pyx_KwValues_FASTCALL(args, nargs) ((args) + (nargs))
+    static CYTHON_INLINE PyObject * __Pyx_GetKwValue_FASTCALL(PyObject *kwnames, PyObject *const *kwvalues, PyObject *s);
+    #define __Pyx_KwargsAsDict_FASTCALL(kw, kwvalues) _PyStack_AsDict(kwvalues, kw)
+#else
+    #define __Pyx_Arg_FASTCALL __Pyx_Arg_VARARGS
+    #define __Pyx_NumKwargs_FASTCALL __Pyx_NumKwargs_VARARGS
+    #define __Pyx_KwValues_FASTCALL __Pyx_KwValues_VARARGS
+    #define __Pyx_GetKwValue_FASTCALL __Pyx_GetKwValue_VARARGS
+    #define __Pyx_KwargsAsDict_FASTCALL __Pyx_KwargsAsDict_VARARGS
+#endif
+#if CYTHON_COMPILING_IN_CPYTHON
+#define __Pyx_ArgsSlice_VARARGS(args, start, stop) __Pyx_PyTuple_FromArray(&__Pyx_Arg_VARARGS(args, start), stop - start)
+#define __Pyx_ArgsSlice_FASTCALL(args, start, stop) __Pyx_PyTuple_FromArray(&__Pyx_Arg_FASTCALL(args, start), stop - start)
+#else
+#define __Pyx_ArgsSlice_VARARGS(args, start, stop) PyTuple_GetSlice(args, start, stop)
+#define __Pyx_ArgsSlice_FASTCALL(args, start, stop) PyTuple_GetSlice(args, start, stop)
+#endif
+
+/* RaiseArgTupleInvalid.proto */
+static void __Pyx_RaiseArgtupleInvalid(const char* func_name, int exact,
+    Py_ssize_t num_min, Py_ssize_t num_max, Py_ssize_t num_found);
+
+/* RaiseDoubleKeywords.proto */
+static void __Pyx_RaiseDoubleKeywordsError(const char* func_name, PyObject* kw_name);
+
+/* ParseKeywords.proto */
+static int __Pyx_ParseOptionalKeywords(PyObject *kwds, PyObject *const *kwvalues,
+    PyObject **argnames[],
+    PyObject *kwds2, PyObject *values[], Py_ssize_t num_pos_args,
+    const char* function_name);
+
 /* PyDictVersioning.proto */
 #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_TYPE_SLOTS
 #define __PYX_DICT_VERSION_INIT  ((PY_UINT64_T) -1)
 #define __PYX_GET_DICT_VERSION(dict)  (((PyDictObject*)(dict))->ma_version_tag)
 #define __PYX_UPDATE_DICT_CACHE(dict, value, cache_var, version_var)\
     (version_var) = __PYX_GET_DICT_VERSION(dict);\
     (cache_var) = (value);
@@ -1021,218 +1637,277 @@
 #define __PYX_GET_DICT_VERSION(dict)  (0)
 #define __PYX_UPDATE_DICT_CACHE(dict, value, cache_var, version_var)
 #define __PYX_PY_DICT_LOOKUP_IF_MODIFIED(VAR, DICT, LOOKUP)  (VAR) = (LOOKUP);
 #endif
 
 /* GetModuleGlobalName.proto */
 #if CYTHON_USE_DICT_VERSIONS
-#define __Pyx_GetModuleGlobalName(var, name)  {\
+#define __Pyx_GetModuleGlobalName(var, name)  do {\
     static PY_UINT64_T __pyx_dict_version = 0;\
     static PyObject *__pyx_dict_cached_value = NULL;\
     (var) = (likely(__pyx_dict_version == __PYX_GET_DICT_VERSION(__pyx_d))) ?\
         (likely(__pyx_dict_cached_value) ? __Pyx_NewRef(__pyx_dict_cached_value) : __Pyx_GetBuiltinName(name)) :\
         __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
-#define __Pyx_GetModuleGlobalNameUncached(var, name)  {\
+} while(0)
+#define __Pyx_GetModuleGlobalNameUncached(var, name)  do {\
     PY_UINT64_T __pyx_dict_version;\
     PyObject *__pyx_dict_cached_value;\
     (var) = __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
+} while(0)
 static PyObject *__Pyx__GetModuleGlobalName(PyObject *name, PY_UINT64_T *dict_version, PyObject **dict_cached_value);
 #else
 #define __Pyx_GetModuleGlobalName(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 #define __Pyx_GetModuleGlobalNameUncached(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name);
 #endif
 
-/* PyCFunctionFastCall.proto */
-#if CYTHON_FAST_PYCCALL
-static CYTHON_INLINE PyObject *__Pyx_PyCFunction_FastCall(PyObject *func, PyObject **args, Py_ssize_t nargs);
-#else
-#define __Pyx_PyCFunction_FastCall(func, args, nargs)  (assert(0), NULL)
-#endif
-
 /* PyFunctionFastCall.proto */
 #if CYTHON_FAST_PYCALL
+#if !CYTHON_VECTORCALL
 #define __Pyx_PyFunction_FastCall(func, args, nargs)\
     __Pyx_PyFunction_FastCallDict((func), (args), (nargs), NULL)
-#if 1 || PY_VERSION_HEX < 0x030600B1
 static PyObject *__Pyx_PyFunction_FastCallDict(PyObject *func, PyObject **args, Py_ssize_t nargs, PyObject *kwargs);
-#else
-#define __Pyx_PyFunction_FastCallDict(func, args, nargs, kwargs) _PyFunction_FastCallDict(func, args, nargs, kwargs)
 #endif
 #define __Pyx_BUILD_ASSERT_EXPR(cond)\
     (sizeof(char [1 - 2*!(cond)]) - 1)
 #ifndef Py_MEMBER_SIZE
 #define Py_MEMBER_SIZE(type, member) sizeof(((type *)0)->member)
 #endif
-#if CYTHON_FAST_PYCALL
+#if !CYTHON_VECTORCALL
+#if PY_VERSION_HEX >= 0x03080000
+  #include "frameobject.h"
+#if PY_VERSION_HEX >= 0x030b00a6
+  #ifndef Py_BUILD_CORE
+    #define Py_BUILD_CORE 1
+  #endif
+  #include "internal/pycore_frame.h"
+#endif
+  #define __Pxy_PyFrame_Initialize_Offsets()
+  #define __Pyx_PyFrame_GetLocalsplus(frame)  ((frame)->f_localsplus)
+#else
   static size_t __pyx_pyframe_localsplus_offset = 0;
   #include "frameobject.h"
   #define __Pxy_PyFrame_Initialize_Offsets()\
     ((void)__Pyx_BUILD_ASSERT_EXPR(sizeof(PyFrameObject) == offsetof(PyFrameObject, f_localsplus) + Py_MEMBER_SIZE(PyFrameObject, f_localsplus)),\
      (void)(__pyx_pyframe_localsplus_offset = ((size_t)PyFrame_Type.tp_basicsize) - Py_MEMBER_SIZE(PyFrameObject, f_localsplus)))
   #define __Pyx_PyFrame_GetLocalsplus(frame)\
     (assert(__pyx_pyframe_localsplus_offset), (PyObject **)(((char *)(frame)) + __pyx_pyframe_localsplus_offset))
-#endif // CYTHON_FAST_PYCALL
 #endif
-
-/* PyObjectCall.proto */
-#if CYTHON_COMPILING_IN_CPYTHON
-static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw);
-#else
-#define __Pyx_PyObject_Call(func, arg, kw) PyObject_Call(func, arg, kw)
 #endif
-
-/* PyObjectCall2Args.proto */
-static CYTHON_UNUSED PyObject* __Pyx_PyObject_Call2Args(PyObject* function, PyObject* arg1, PyObject* arg2);
+#endif
 
 /* PyObjectCallMethO.proto */
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallMethO(PyObject *func, PyObject *arg);
 #endif
 
-/* PyObjectCallOneArg.proto */
-static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg);
+/* PyObjectFastCall.proto */
+#define __Pyx_PyObject_FastCall(func, args, nargs)  __Pyx_PyObject_FastCallDict(func, args, (size_t)(nargs), NULL)
+static CYTHON_INLINE PyObject* __Pyx_PyObject_FastCallDict(PyObject *func, PyObject **args, size_t nargs, PyObject *kwargs);
 
 /* RaiseTooManyValuesToUnpack.proto */
 static CYTHON_INLINE void __Pyx_RaiseTooManyValuesError(Py_ssize_t expected);
 
 /* RaiseNeedMoreValuesToUnpack.proto */
 static CYTHON_INLINE void __Pyx_RaiseNeedMoreValuesError(Py_ssize_t index);
 
 /* IterFinish.proto */
 static CYTHON_INLINE int __Pyx_IterFinish(void);
 
 /* UnpackItemEndCheck.proto */
 static int __Pyx_IternextUnpackEndCheck(PyObject *retval, Py_ssize_t expected);
 
-/* PyObjectCallNoArg.proto */
-#if CYTHON_COMPILING_IN_CPYTHON
-static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func);
+/* AssertionsEnabled.proto */
+#define __Pyx_init_assertions_enabled()
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
+  #define __pyx_assertions_enabled() (1)
+#elif PY_VERSION_HEX < 0x03080000  ||  CYTHON_COMPILING_IN_PYPY  ||  defined(Py_LIMITED_API)
+  #define __pyx_assertions_enabled() (!Py_OptimizeFlag)
+#elif CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030900A6
+  static int __pyx_assertions_enabled_flag;
+  #define __pyx_assertions_enabled() (__pyx_assertions_enabled_flag)
+  #undef __Pyx_init_assertions_enabled
+  static void __Pyx_init_assertions_enabled(void) {
+    __pyx_assertions_enabled_flag = ! _PyInterpreterState_GetConfig(__Pyx_PyThreadState_Current->interp)->optimization_level;
+  }
 #else
-#define __Pyx_PyObject_CallNoArg(func) __Pyx_PyObject_Call(func, __pyx_empty_tuple, NULL)
+  #define __pyx_assertions_enabled() (!Py_OptimizeFlag)
 #endif
 
-/* DictGetItem.proto */
-#if PY_MAJOR_VERSION >= 3 && !CYTHON_COMPILING_IN_PYPY
-static PyObject *__Pyx_PyDict_GetItem(PyObject *d, PyObject* key);
-#define __Pyx_PyObject_Dict_GetItem(obj, name)\
-    (likely(PyDict_CheckExact(obj)) ?\
-     __Pyx_PyDict_GetItem(obj, name) : PyObject_GetItem(obj, name))
-#else
-#define __Pyx_PyDict_GetItem(d, key) PyObject_GetItem(d, key)
-#define __Pyx_PyObject_Dict_GetItem(obj, name)  PyObject_GetItem(obj, name)
-#endif
+/* Import.proto */
+static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
 
-/* GetTopmostException.proto */
-#if CYTHON_USE_EXC_INFO_STACK
-static _PyErr_StackItem * __Pyx_PyErr_GetTopmostException(PyThreadState *tstate);
+/* ImportDottedModule.proto */
+static PyObject *__Pyx_ImportDottedModule(PyObject *name, PyObject *parts_tuple);
+#if PY_MAJOR_VERSION >= 3
+static PyObject *__Pyx_ImportDottedModule_WalkParts(PyObject *module, PyObject *name, PyObject *parts_tuple);
 #endif
 
-/* PyThreadStateGet.proto */
-#if CYTHON_FAST_THREAD_STATE
-#define __Pyx_PyThreadState_declare  PyThreadState *__pyx_tstate;
-#define __Pyx_PyThreadState_assign  __pyx_tstate = __Pyx_PyThreadState_Current;
-#define __Pyx_PyErr_Occurred()  __pyx_tstate->curexc_type
-#else
-#define __Pyx_PyThreadState_declare
-#define __Pyx_PyThreadState_assign
-#define __Pyx_PyErr_Occurred()  PyErr_Occurred()
-#endif
+/* IncludeStructmemberH.proto */
+#include <structmember.h>
 
-/* SaveResetException.proto */
-#if CYTHON_FAST_THREAD_STATE
-#define __Pyx_ExceptionSave(type, value, tb)  __Pyx__ExceptionSave(__pyx_tstate, type, value, tb)
-static CYTHON_INLINE void __Pyx__ExceptionSave(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
-#define __Pyx_ExceptionReset(type, value, tb)  __Pyx__ExceptionReset(__pyx_tstate, type, value, tb)
-static CYTHON_INLINE void __Pyx__ExceptionReset(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb);
-#else
-#define __Pyx_ExceptionSave(type, value, tb)   PyErr_GetExcInfo(type, value, tb)
-#define __Pyx_ExceptionReset(type, value, tb)  PyErr_SetExcInfo(type, value, tb)
+/* FixUpExtensionType.proto */
+#if CYTHON_USE_TYPE_SPECS
+static int __Pyx_fix_up_extension_type_from_spec(PyType_Spec *spec, PyTypeObject *type);
 #endif
 
-/* PyErrExceptionMatches.proto */
-#if CYTHON_FAST_THREAD_STATE
-#define __Pyx_PyErr_ExceptionMatches(err) __Pyx_PyErr_ExceptionMatchesInState(__pyx_tstate, err)
-static CYTHON_INLINE int __Pyx_PyErr_ExceptionMatchesInState(PyThreadState* tstate, PyObject* err);
-#else
-#define __Pyx_PyErr_ExceptionMatches(err)  PyErr_ExceptionMatches(err)
-#endif
+/* FetchSharedCythonModule.proto */
+static PyObject *__Pyx_FetchSharedCythonABIModule(void);
 
-/* GetException.proto */
-#if CYTHON_FAST_THREAD_STATE
-#define __Pyx_GetException(type, value, tb)  __Pyx__GetException(__pyx_tstate, type, value, tb)
-static int __Pyx__GetException(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
+/* FetchCommonType.proto */
+#if !CYTHON_USE_TYPE_SPECS
+static PyTypeObject* __Pyx_FetchCommonType(PyTypeObject* type);
 #else
-static int __Pyx_GetException(PyObject **type, PyObject **value, PyObject **tb);
+static PyTypeObject* __Pyx_FetchCommonTypeFromSpec(PyObject *module, PyType_Spec *spec, PyObject *bases);
 #endif
 
-/* PyErrFetchRestore.proto */
-#if CYTHON_FAST_THREAD_STATE
-#define __Pyx_PyErr_Clear() __Pyx_ErrRestore(NULL, NULL, NULL)
-#define __Pyx_ErrRestoreWithState(type, value, tb)  __Pyx_ErrRestoreInState(PyThreadState_GET(), type, value, tb)
-#define __Pyx_ErrFetchWithState(type, value, tb)    __Pyx_ErrFetchInState(PyThreadState_GET(), type, value, tb)
-#define __Pyx_ErrRestore(type, value, tb)  __Pyx_ErrRestoreInState(__pyx_tstate, type, value, tb)
-#define __Pyx_ErrFetch(type, value, tb)    __Pyx_ErrFetchInState(__pyx_tstate, type, value, tb)
-static CYTHON_INLINE void __Pyx_ErrRestoreInState(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb);
-static CYTHON_INLINE void __Pyx_ErrFetchInState(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
-#if CYTHON_COMPILING_IN_CPYTHON
-#define __Pyx_PyErr_SetNone(exc) (Py_INCREF(exc), __Pyx_ErrRestore((exc), NULL, NULL))
+/* PyMethodNew.proto */
+#if PY_MAJOR_VERSION >= 3
+static PyObject *__Pyx_PyMethod_New(PyObject *func, PyObject *self, PyObject *typ) {
+    CYTHON_UNUSED_VAR(typ);
+    if (!self)
+        return __Pyx_NewRef(func);
+    return PyMethod_New(func, self);
+}
+#else
+    #define __Pyx_PyMethod_New PyMethod_New
+#endif
+
+/* PyVectorcallFastCallDict.proto */
+#if CYTHON_METH_FASTCALL
+static CYTHON_INLINE PyObject *__Pyx_PyVectorcall_FastCallDict(PyObject *func, __pyx_vectorcallfunc vc, PyObject *const *args, size_t nargs, PyObject *kw);
+#endif
+
+/* CythonFunctionShared.proto */
+#define __Pyx_CyFunction_USED
+#define __Pyx_CYFUNCTION_STATICMETHOD  0x01
+#define __Pyx_CYFUNCTION_CLASSMETHOD   0x02
+#define __Pyx_CYFUNCTION_CCLASS        0x04
+#define __Pyx_CYFUNCTION_COROUTINE     0x08
+#define __Pyx_CyFunction_GetClosure(f)\
+    (((__pyx_CyFunctionObject *) (f))->func_closure)
+#if PY_VERSION_HEX < 0x030900B1
+  #define __Pyx_CyFunction_GetClassObj(f)\
+      (((__pyx_CyFunctionObject *) (f))->func_classobj)
+#else
+  #define __Pyx_CyFunction_GetClassObj(f)\
+      ((PyObject*) ((PyCMethodObject *) (f))->mm_class)
+#endif
+#define __Pyx_CyFunction_SetClassObj(f, classobj)\
+    __Pyx__CyFunction_SetClassObj((__pyx_CyFunctionObject *) (f), (classobj))
+#define __Pyx_CyFunction_Defaults(type, f)\
+    ((type *)(((__pyx_CyFunctionObject *) (f))->defaults))
+#define __Pyx_CyFunction_SetDefaultsGetter(f, g)\
+    ((__pyx_CyFunctionObject *) (f))->defaults_getter = (g)
+typedef struct {
+#if PY_VERSION_HEX < 0x030900B1
+    PyCFunctionObject func;
 #else
-#define __Pyx_PyErr_SetNone(exc) PyErr_SetNone(exc)
+    PyCMethodObject func;
 #endif
-#else
-#define __Pyx_PyErr_Clear() PyErr_Clear()
-#define __Pyx_PyErr_SetNone(exc) PyErr_SetNone(exc)
-#define __Pyx_ErrRestoreWithState(type, value, tb)  PyErr_Restore(type, value, tb)
-#define __Pyx_ErrFetchWithState(type, value, tb)  PyErr_Fetch(type, value, tb)
-#define __Pyx_ErrRestoreInState(tstate, type, value, tb)  PyErr_Restore(type, value, tb)
-#define __Pyx_ErrFetchInState(tstate, type, value, tb)  PyErr_Fetch(type, value, tb)
-#define __Pyx_ErrRestore(type, value, tb)  PyErr_Restore(type, value, tb)
-#define __Pyx_ErrFetch(type, value, tb)  PyErr_Fetch(type, value, tb)
+#if CYTHON_BACKPORT_VECTORCALL
+    __pyx_vectorcallfunc func_vectorcall;
 #endif
-
-/* RaiseException.proto */
-static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause);
-
-/* Import.proto */
-static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
+#if PY_VERSION_HEX < 0x030500A0
+    PyObject *func_weakreflist;
+#endif
+    PyObject *func_dict;
+    PyObject *func_name;
+    PyObject *func_qualname;
+    PyObject *func_doc;
+    PyObject *func_globals;
+    PyObject *func_code;
+    PyObject *func_closure;
+#if PY_VERSION_HEX < 0x030900B1
+    PyObject *func_classobj;
+#endif
+    void *defaults;
+    int defaults_pyobjects;
+    size_t defaults_size;  // used by FusedFunction for copying defaults
+    int flags;
+    PyObject *defaults_tuple;
+    PyObject *defaults_kwdict;
+    PyObject *(*defaults_getter)(PyObject *);
+    PyObject *func_annotations;
+    PyObject *func_is_coroutine;
+} __pyx_CyFunctionObject;
+#define __Pyx_CyFunction_Check(obj)  __Pyx_TypeCheck(obj, __pyx_CyFunctionType)
+#define __Pyx_IsCyOrPyCFunction(obj)  __Pyx_TypeCheck2(obj, __pyx_CyFunctionType, &PyCFunction_Type)
+#define __Pyx_CyFunction_CheckExact(obj)  __Pyx_IS_TYPE(obj, __pyx_CyFunctionType)
+static PyObject *__Pyx_CyFunction_Init(__pyx_CyFunctionObject* op, PyMethodDef *ml,
+                                      int flags, PyObject* qualname,
+                                      PyObject *closure,
+                                      PyObject *module, PyObject *globals,
+                                      PyObject* code);
+static CYTHON_INLINE void __Pyx__CyFunction_SetClassObj(__pyx_CyFunctionObject* f, PyObject* classobj);
+static CYTHON_INLINE void *__Pyx_CyFunction_InitDefaults(PyObject *m,
+                                                         size_t size,
+                                                         int pyobjects);
+static CYTHON_INLINE void __Pyx_CyFunction_SetDefaultsTuple(PyObject *m,
+                                                            PyObject *tuple);
+static CYTHON_INLINE void __Pyx_CyFunction_SetDefaultsKwDict(PyObject *m,
+                                                             PyObject *dict);
+static CYTHON_INLINE void __Pyx_CyFunction_SetAnnotationsDict(PyObject *m,
+                                                              PyObject *dict);
+static int __pyx_CyFunction_init(PyObject *module);
+#if CYTHON_METH_FASTCALL
+static PyObject * __Pyx_CyFunction_Vectorcall_NOARGS(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames);
+static PyObject * __Pyx_CyFunction_Vectorcall_O(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames);
+static PyObject * __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames);
+static PyObject * __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS_METHOD(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames);
+#if CYTHON_BACKPORT_VECTORCALL
+#define __Pyx_CyFunction_func_vectorcall(f) (((__pyx_CyFunctionObject*)f)->func_vectorcall)
+#else
+#define __Pyx_CyFunction_func_vectorcall(f) (((PyCFunctionObject*)f)->vectorcall)
+#endif
+#endif
+
+/* CythonFunction.proto */
+static PyObject *__Pyx_CyFunction_New(PyMethodDef *ml,
+                                      int flags, PyObject* qualname,
+                                      PyObject *closure,
+                                      PyObject *module, PyObject *globals,
+                                      PyObject* code);
 
 /* CLineInTraceback.proto */
 #ifdef CYTHON_CLINE_IN_TRACEBACK
 #define __Pyx_CLineForTraceback(tstate, c_line)  (((CYTHON_CLINE_IN_TRACEBACK)) ? c_line : 0)
 #else
 static int __Pyx_CLineForTraceback(PyThreadState *tstate, int c_line);
 #endif
 
 /* CodeObjectCache.proto */
+#if !CYTHON_COMPILING_IN_LIMITED_API
 typedef struct {
     PyCodeObject* code_object;
     int code_line;
 } __Pyx_CodeObjectCacheEntry;
 struct __Pyx_CodeObjectCache {
     int count;
     int max_count;
     __Pyx_CodeObjectCacheEntry* entries;
 };
 static struct __Pyx_CodeObjectCache __pyx_code_cache = {0,0,NULL};
 static int __pyx_bisect_code_objects(__Pyx_CodeObjectCacheEntry* entries, int count, int code_line);
 static PyCodeObject *__pyx_find_code_object(int code_line);
 static void __pyx_insert_code_object(int code_line, PyCodeObject* code_object);
+#endif
 
 /* AddTraceback.proto */
 static void __Pyx_AddTraceback(const char *funcname, int c_line,
                                int py_line, const char *filename);
 
 /* GCCDiagnostics.proto */
-#if defined(__GNUC__) && (__GNUC__ > 4 || (__GNUC__ == 4 && __GNUC_MINOR__ >= 6))
+#if !defined(__INTEL_COMPILER) && defined(__GNUC__) && (__GNUC__ > 4 || (__GNUC__ == 4 && __GNUC_MINOR__ >= 6))
 #define __Pyx_HAS_GCC_DIAGNOSTIC
 #endif
 
+/* RaiseUnexpectedTypeError.proto */
+static int __Pyx_RaiseUnexpectedTypeError(const char *expected, PyObject *obj);
+
 static PyObject* __pyx_convert__to_py_struct__timespec(struct timespec s);
 /* CIntFromPy.proto */
 static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *);
 
 /* CIntFromPy.proto */
 static CYTHON_INLINE time_t __Pyx_PyInt_As_time_t(PyObject *);
 
@@ -1244,149 +1919,767 @@
 
 /* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_time_t(time_t value);
 
 /* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value);
 
+/* FormatTypeName.proto */
+#if CYTHON_COMPILING_IN_LIMITED_API
+typedef PyObject *__Pyx_TypeName;
+#define __Pyx_FMT_TYPENAME "%U"
+static __Pyx_TypeName __Pyx_PyType_GetName(PyTypeObject* tp);
+#define __Pyx_DECREF_TypeName(obj) Py_XDECREF(obj)
+#else
+typedef const char *__Pyx_TypeName;
+#define __Pyx_FMT_TYPENAME "%.200s"
+#define __Pyx_PyType_GetName(tp) ((tp)->tp_name)
+#define __Pyx_DECREF_TypeName(obj)
+#endif
+
 /* FastTypeChecks.proto */
 #if CYTHON_COMPILING_IN_CPYTHON
 #define __Pyx_TypeCheck(obj, type) __Pyx_IsSubtype(Py_TYPE(obj), (PyTypeObject *)type)
+#define __Pyx_TypeCheck2(obj, type1, type2) __Pyx_IsAnySubtype2(Py_TYPE(obj), (PyTypeObject *)type1, (PyTypeObject *)type2)
 static CYTHON_INLINE int __Pyx_IsSubtype(PyTypeObject *a, PyTypeObject *b);
+static CYTHON_INLINE int __Pyx_IsAnySubtype2(PyTypeObject *cls, PyTypeObject *a, PyTypeObject *b);
 static CYTHON_INLINE int __Pyx_PyErr_GivenExceptionMatches(PyObject *err, PyObject *type);
 static CYTHON_INLINE int __Pyx_PyErr_GivenExceptionMatches2(PyObject *err, PyObject *type1, PyObject *type2);
 #else
 #define __Pyx_TypeCheck(obj, type) PyObject_TypeCheck(obj, (PyTypeObject *)type)
+#define __Pyx_TypeCheck2(obj, type1, type2) (PyObject_TypeCheck(obj, (PyTypeObject *)type1) || PyObject_TypeCheck(obj, (PyTypeObject *)type2))
 #define __Pyx_PyErr_GivenExceptionMatches(err, type) PyErr_GivenExceptionMatches(err, type)
 #define __Pyx_PyErr_GivenExceptionMatches2(err, type1, type2) (PyErr_GivenExceptionMatches(err, type1) || PyErr_GivenExceptionMatches(err, type2))
 #endif
+#define __Pyx_PyErr_ExceptionMatches2(err1, err2)  __Pyx_PyErr_GivenExceptionMatches2(__Pyx_PyErr_CurrentExceptionType(), err1, err2)
 #define __Pyx_PyException_Check(obj) __Pyx_TypeCheck(obj, PyExc_Exception)
 
 /* CheckBinaryVersion.proto */
 static int __Pyx_check_binary_version(void);
 
 /* InitStrings.proto */
 static int __Pyx_InitStrings(__Pyx_StringTabEntry *t);
 
+/* #### Code section: module_declarations ### */
 
-/* Module declarations from 'posix.types' */
+/* Module declarations from "posix.types" */
 
-/* Module declarations from 'posix.unistd' */
+/* Module declarations from "posix.unistd" */
 
-/* Module declarations from 'posix.signal' */
+/* Module declarations from "posix.signal" */
 
-/* Module declarations from 'posix.time' */
+/* Module declarations from "posix.time" */
 
-/* Module declarations from 'libc.stddef' */
+/* Module declarations from "libc.stddef" */
 
-/* Module declarations from 'libc.time' */
+/* Module declarations from "libc.time" */
 
-/* Module declarations from 'atimer._atimer' */
+/* Module declarations from "atimer._atimer" */
 static struct timespec __pyx_convert__from_py_struct__timespec(PyObject *); /*proto*/
+/* #### Code section: typeinfo ### */
+/* #### Code section: before_global_var ### */
 #define __Pyx_MODULE_NAME "atimer._atimer"
 extern int __pyx_module_is_main_atimer___atimer;
 int __pyx_module_is_main_atimer___atimer = 0;
 
-/* Implementation of 'atimer._atimer' */
-static PyObject *__pyx_builtin_TypeError;
+/* Implementation of "atimer._atimer" */
+/* #### Code section: global_var ### */
+static PyObject *__pyx_builtin_AssertionError;
 static PyObject *__pyx_builtin_KeyError;
 static PyObject *__pyx_builtin_ValueError;
+/* #### Code section: string_decls ### */
 static const char __pyx_k_r[] = "r";
+static const char __pyx_k__3[] = "*";
 static const char __pyx_k_fd[] = "fd";
 static const char __pyx_k_ts[] = "ts";
+static const char __pyx_k__13[] = "?";
 static const char __pyx_k_now[] = "now";
 static const char __pyx_k_sec[] = "sec";
 static const char __pyx_k_main[] = "__main__";
 static const char __pyx_k_name[] = "__name__";
 static const char __pyx_k_nsec[] = "nsec";
+static const char __pyx_k_spec[] = "__spec__";
 static const char __pyx_k_test[] = "__test__";
 static const char __pyx_k_time[] = "time";
 static const char __pyx_k_d_sec[] = "d_sec";
 static const char __pyx_k_value[] = "value";
 static const char __pyx_k_d_nsec[] = "d_nsec";
 static const char __pyx_k_import[] = "__import__";
 static const char __pyx_k_tv_sec[] = "tv_sec";
 static const char __pyx_k_NANOSEC[] = "NANOSEC";
 static const char __pyx_k_tv_nsec[] = "tv_nsec";
 static const char __pyx_k_KeyError[] = "KeyError";
 static const char __pyx_k_interval[] = "interval";
-static const char __pyx_k_TypeError[] = "TypeError";
 static const char __pyx_k_ValueError[] = "ValueError";
 static const char __pyx_k_atimer_init[] = "atimer_init";
 static const char __pyx_k_to_timespec[] = "to_timespec";
 static const char __pyx_k_atimer_close[] = "atimer_close";
 static const char __pyx_k_atimer_start[] = "atimer_start";
+static const char __pyx_k_initializing[] = "_initializing";
+static const char __pyx_k_is_coroutine[] = "_is_coroutine";
 static const char __pyx_k_timespec_add[] = "timespec_add";
+static const char __pyx_k_AssertionError[] = "AssertionError";
 static const char __pyx_k_atimer__atimer[] = "atimer._atimer";
+static const char __pyx_k_asyncio_coroutines[] = "asyncio.coroutines";
 static const char __pyx_k_atimer__atimer_pyx[] = "atimer/_atimer.pyx";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
 static const char __pyx_k_No_value_specified_for_struct_at[] = "No value specified for struct attribute 'tv_sec'";
 static const char __pyx_k_No_value_specified_for_struct_at_2[] = "No value specified for struct attribute 'tv_nsec'";
-static PyObject *__pyx_n_s_KeyError;
-static PyObject *__pyx_n_s_NANOSEC;
-static PyObject *__pyx_kp_s_No_value_specified_for_struct_at;
-static PyObject *__pyx_kp_s_No_value_specified_for_struct_at_2;
-static PyObject *__pyx_n_s_TypeError;
-static PyObject *__pyx_n_s_ValueError;
-static PyObject *__pyx_n_s_atimer__atimer;
-static PyObject *__pyx_kp_s_atimer__atimer_pyx;
-static PyObject *__pyx_n_s_atimer_close;
-static PyObject *__pyx_n_s_atimer_init;
-static PyObject *__pyx_n_s_atimer_start;
-static PyObject *__pyx_n_s_cline_in_traceback;
-static PyObject *__pyx_n_s_d_nsec;
-static PyObject *__pyx_n_s_d_sec;
-static PyObject *__pyx_n_s_fd;
-static PyObject *__pyx_n_s_import;
-static PyObject *__pyx_n_s_interval;
-static PyObject *__pyx_n_s_main;
-static PyObject *__pyx_n_s_name;
-static PyObject *__pyx_n_s_now;
-static PyObject *__pyx_n_s_nsec;
-static PyObject *__pyx_n_s_r;
-static PyObject *__pyx_n_s_sec;
-static PyObject *__pyx_n_s_test;
-static PyObject *__pyx_n_s_time;
-static PyObject *__pyx_n_s_timespec_add;
-static PyObject *__pyx_n_s_to_timespec;
-static PyObject *__pyx_n_s_ts;
-static PyObject *__pyx_n_s_tv_nsec;
-static PyObject *__pyx_n_s_tv_sec;
-static PyObject *__pyx_n_s_value;
+/* #### Code section: decls ### */
 static PyObject *__pyx_pf_6atimer_7_atimer_atimer_init(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
 static PyObject *__pyx_pf_6atimer_7_atimer_2atimer_start(CYTHON_UNUSED PyObject *__pyx_self, int __pyx_v_fd, double __pyx_v_interval); /* proto */
 static PyObject *__pyx_pf_6atimer_7_atimer_4atimer_close(CYTHON_UNUSED PyObject *__pyx_self, int __pyx_v_fd); /* proto */
 static PyObject *__pyx_pf_6atimer_7_atimer_6to_timespec(CYTHON_UNUSED PyObject *__pyx_self, double __pyx_v_value); /* proto */
 static PyObject *__pyx_pf_6atimer_7_atimer_8timespec_add(CYTHON_UNUSED PyObject *__pyx_self, struct timespec __pyx_v_now, time_t __pyx_v_sec, long __pyx_v_nsec); /* proto */
-static PyObject *__pyx_float_1e9;
-static PyObject *__pyx_tuple_;
-static PyObject *__pyx_tuple__2;
-static PyObject *__pyx_tuple__4;
-static PyObject *__pyx_tuple__6;
-static PyObject *__pyx_tuple__8;
-static PyObject *__pyx_tuple__10;
-static PyObject *__pyx_codeobj__3;
-static PyObject *__pyx_codeobj__5;
-static PyObject *__pyx_codeobj__7;
-static PyObject *__pyx_codeobj__9;
-static PyObject *__pyx_codeobj__11;
-/* Late includes */
+/* #### Code section: late_includes ### */
+/* #### Code section: module_state ### */
+typedef struct {
+  PyObject *__pyx_d;
+  PyObject *__pyx_b;
+  PyObject *__pyx_cython_runtime;
+  PyObject *__pyx_empty_tuple;
+  PyObject *__pyx_empty_bytes;
+  PyObject *__pyx_empty_unicode;
+  #ifdef __Pyx_CyFunction_USED
+  PyTypeObject *__pyx_CyFunctionType;
+  #endif
+  #ifdef __Pyx_FusedFunction_USED
+  PyTypeObject *__pyx_FusedFunctionType;
+  #endif
+  #ifdef __Pyx_Generator_USED
+  PyTypeObject *__pyx_GeneratorType;
+  #endif
+  #ifdef __Pyx_IterableCoroutine_USED
+  PyTypeObject *__pyx_IterableCoroutineType;
+  #endif
+  #ifdef __Pyx_Coroutine_USED
+  PyTypeObject *__pyx_CoroutineAwaitType;
+  #endif
+  #ifdef __Pyx_Coroutine_USED
+  PyTypeObject *__pyx_CoroutineType;
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  PyObject *__pyx_n_s_AssertionError;
+  PyObject *__pyx_n_s_KeyError;
+  PyObject *__pyx_n_s_NANOSEC;
+  PyObject *__pyx_kp_s_No_value_specified_for_struct_at;
+  PyObject *__pyx_kp_s_No_value_specified_for_struct_at_2;
+  PyObject *__pyx_n_s_ValueError;
+  PyObject *__pyx_n_s__13;
+  PyObject *__pyx_n_s__3;
+  PyObject *__pyx_n_s_asyncio_coroutines;
+  PyObject *__pyx_n_s_atimer__atimer;
+  PyObject *__pyx_kp_s_atimer__atimer_pyx;
+  PyObject *__pyx_n_s_atimer_close;
+  PyObject *__pyx_n_s_atimer_init;
+  PyObject *__pyx_n_s_atimer_start;
+  PyObject *__pyx_n_s_cline_in_traceback;
+  PyObject *__pyx_n_s_d_nsec;
+  PyObject *__pyx_n_s_d_sec;
+  PyObject *__pyx_n_s_fd;
+  PyObject *__pyx_n_s_import;
+  PyObject *__pyx_n_s_initializing;
+  PyObject *__pyx_n_s_interval;
+  PyObject *__pyx_n_s_is_coroutine;
+  PyObject *__pyx_n_s_main;
+  PyObject *__pyx_n_s_name;
+  PyObject *__pyx_n_s_now;
+  PyObject *__pyx_n_s_nsec;
+  PyObject *__pyx_n_s_r;
+  PyObject *__pyx_n_s_sec;
+  PyObject *__pyx_n_s_spec;
+  PyObject *__pyx_n_s_test;
+  PyObject *__pyx_n_s_time;
+  PyObject *__pyx_n_s_timespec_add;
+  PyObject *__pyx_n_s_to_timespec;
+  PyObject *__pyx_n_s_ts;
+  PyObject *__pyx_n_s_tv_nsec;
+  PyObject *__pyx_n_s_tv_sec;
+  PyObject *__pyx_n_s_value;
+  PyObject *__pyx_float_1e9;
+  PyObject *__pyx_tuple_;
+  PyObject *__pyx_tuple__2;
+  PyObject *__pyx_tuple__5;
+  PyObject *__pyx_tuple__7;
+  PyObject *__pyx_tuple__9;
+  PyObject *__pyx_tuple__11;
+  PyObject *__pyx_codeobj__4;
+  PyObject *__pyx_codeobj__6;
+  PyObject *__pyx_codeobj__8;
+  PyObject *__pyx_codeobj__10;
+  PyObject *__pyx_codeobj__12;
+} __pyx_mstate;
+
+#if CYTHON_USE_MODULE_STATE
+#ifdef __cplusplus
+namespace {
+  extern struct PyModuleDef __pyx_moduledef;
+} /* anonymous namespace */
+#else
+static struct PyModuleDef __pyx_moduledef;
+#endif
+
+#define __pyx_mstate(o) ((__pyx_mstate *)__Pyx_PyModule_GetState(o))
+
+#define __pyx_mstate_global (__pyx_mstate(PyState_FindModule(&__pyx_moduledef)))
+
+#define __pyx_m (PyState_FindModule(&__pyx_moduledef))
+#else
+static __pyx_mstate __pyx_mstate_global_static =
+#ifdef __cplusplus
+    {};
+#else
+    {0};
+#endif
+static __pyx_mstate *__pyx_mstate_global = &__pyx_mstate_global_static;
+#endif
+/* #### Code section: module_state_clear ### */
+#if CYTHON_USE_MODULE_STATE
+static int __pyx_m_clear(PyObject *m) {
+  __pyx_mstate *clear_module_state = __pyx_mstate(m);
+  if (!clear_module_state) return 0;
+  Py_CLEAR(clear_module_state->__pyx_d);
+  Py_CLEAR(clear_module_state->__pyx_b);
+  Py_CLEAR(clear_module_state->__pyx_cython_runtime);
+  Py_CLEAR(clear_module_state->__pyx_empty_tuple);
+  Py_CLEAR(clear_module_state->__pyx_empty_bytes);
+  Py_CLEAR(clear_module_state->__pyx_empty_unicode);
+  #ifdef __Pyx_CyFunction_USED
+  Py_CLEAR(clear_module_state->__pyx_CyFunctionType);
+  #endif
+  #ifdef __Pyx_FusedFunction_USED
+  Py_CLEAR(clear_module_state->__pyx_FusedFunctionType);
+  #endif
+  Py_CLEAR(clear_module_state->__pyx_n_s_AssertionError);
+  Py_CLEAR(clear_module_state->__pyx_n_s_KeyError);
+  Py_CLEAR(clear_module_state->__pyx_n_s_NANOSEC);
+  Py_CLEAR(clear_module_state->__pyx_kp_s_No_value_specified_for_struct_at);
+  Py_CLEAR(clear_module_state->__pyx_kp_s_No_value_specified_for_struct_at_2);
+  Py_CLEAR(clear_module_state->__pyx_n_s_ValueError);
+  Py_CLEAR(clear_module_state->__pyx_n_s__13);
+  Py_CLEAR(clear_module_state->__pyx_n_s__3);
+  Py_CLEAR(clear_module_state->__pyx_n_s_asyncio_coroutines);
+  Py_CLEAR(clear_module_state->__pyx_n_s_atimer__atimer);
+  Py_CLEAR(clear_module_state->__pyx_kp_s_atimer__atimer_pyx);
+  Py_CLEAR(clear_module_state->__pyx_n_s_atimer_close);
+  Py_CLEAR(clear_module_state->__pyx_n_s_atimer_init);
+  Py_CLEAR(clear_module_state->__pyx_n_s_atimer_start);
+  Py_CLEAR(clear_module_state->__pyx_n_s_cline_in_traceback);
+  Py_CLEAR(clear_module_state->__pyx_n_s_d_nsec);
+  Py_CLEAR(clear_module_state->__pyx_n_s_d_sec);
+  Py_CLEAR(clear_module_state->__pyx_n_s_fd);
+  Py_CLEAR(clear_module_state->__pyx_n_s_import);
+  Py_CLEAR(clear_module_state->__pyx_n_s_initializing);
+  Py_CLEAR(clear_module_state->__pyx_n_s_interval);
+  Py_CLEAR(clear_module_state->__pyx_n_s_is_coroutine);
+  Py_CLEAR(clear_module_state->__pyx_n_s_main);
+  Py_CLEAR(clear_module_state->__pyx_n_s_name);
+  Py_CLEAR(clear_module_state->__pyx_n_s_now);
+  Py_CLEAR(clear_module_state->__pyx_n_s_nsec);
+  Py_CLEAR(clear_module_state->__pyx_n_s_r);
+  Py_CLEAR(clear_module_state->__pyx_n_s_sec);
+  Py_CLEAR(clear_module_state->__pyx_n_s_spec);
+  Py_CLEAR(clear_module_state->__pyx_n_s_test);
+  Py_CLEAR(clear_module_state->__pyx_n_s_time);
+  Py_CLEAR(clear_module_state->__pyx_n_s_timespec_add);
+  Py_CLEAR(clear_module_state->__pyx_n_s_to_timespec);
+  Py_CLEAR(clear_module_state->__pyx_n_s_ts);
+  Py_CLEAR(clear_module_state->__pyx_n_s_tv_nsec);
+  Py_CLEAR(clear_module_state->__pyx_n_s_tv_sec);
+  Py_CLEAR(clear_module_state->__pyx_n_s_value);
+  Py_CLEAR(clear_module_state->__pyx_float_1e9);
+  Py_CLEAR(clear_module_state->__pyx_tuple_);
+  Py_CLEAR(clear_module_state->__pyx_tuple__2);
+  Py_CLEAR(clear_module_state->__pyx_tuple__5);
+  Py_CLEAR(clear_module_state->__pyx_tuple__7);
+  Py_CLEAR(clear_module_state->__pyx_tuple__9);
+  Py_CLEAR(clear_module_state->__pyx_tuple__11);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__4);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__6);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__8);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__10);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__12);
+  return 0;
+}
+#endif
+/* #### Code section: module_state_traverse ### */
+#if CYTHON_USE_MODULE_STATE
+static int __pyx_m_traverse(PyObject *m, visitproc visit, void *arg) {
+  __pyx_mstate *traverse_module_state = __pyx_mstate(m);
+  if (!traverse_module_state) return 0;
+  Py_VISIT(traverse_module_state->__pyx_d);
+  Py_VISIT(traverse_module_state->__pyx_b);
+  Py_VISIT(traverse_module_state->__pyx_cython_runtime);
+  Py_VISIT(traverse_module_state->__pyx_empty_tuple);
+  Py_VISIT(traverse_module_state->__pyx_empty_bytes);
+  Py_VISIT(traverse_module_state->__pyx_empty_unicode);
+  #ifdef __Pyx_CyFunction_USED
+  Py_VISIT(traverse_module_state->__pyx_CyFunctionType);
+  #endif
+  #ifdef __Pyx_FusedFunction_USED
+  Py_VISIT(traverse_module_state->__pyx_FusedFunctionType);
+  #endif
+  Py_VISIT(traverse_module_state->__pyx_n_s_AssertionError);
+  Py_VISIT(traverse_module_state->__pyx_n_s_KeyError);
+  Py_VISIT(traverse_module_state->__pyx_n_s_NANOSEC);
+  Py_VISIT(traverse_module_state->__pyx_kp_s_No_value_specified_for_struct_at);
+  Py_VISIT(traverse_module_state->__pyx_kp_s_No_value_specified_for_struct_at_2);
+  Py_VISIT(traverse_module_state->__pyx_n_s_ValueError);
+  Py_VISIT(traverse_module_state->__pyx_n_s__13);
+  Py_VISIT(traverse_module_state->__pyx_n_s__3);
+  Py_VISIT(traverse_module_state->__pyx_n_s_asyncio_coroutines);
+  Py_VISIT(traverse_module_state->__pyx_n_s_atimer__atimer);
+  Py_VISIT(traverse_module_state->__pyx_kp_s_atimer__atimer_pyx);
+  Py_VISIT(traverse_module_state->__pyx_n_s_atimer_close);
+  Py_VISIT(traverse_module_state->__pyx_n_s_atimer_init);
+  Py_VISIT(traverse_module_state->__pyx_n_s_atimer_start);
+  Py_VISIT(traverse_module_state->__pyx_n_s_cline_in_traceback);
+  Py_VISIT(traverse_module_state->__pyx_n_s_d_nsec);
+  Py_VISIT(traverse_module_state->__pyx_n_s_d_sec);
+  Py_VISIT(traverse_module_state->__pyx_n_s_fd);
+  Py_VISIT(traverse_module_state->__pyx_n_s_import);
+  Py_VISIT(traverse_module_state->__pyx_n_s_initializing);
+  Py_VISIT(traverse_module_state->__pyx_n_s_interval);
+  Py_VISIT(traverse_module_state->__pyx_n_s_is_coroutine);
+  Py_VISIT(traverse_module_state->__pyx_n_s_main);
+  Py_VISIT(traverse_module_state->__pyx_n_s_name);
+  Py_VISIT(traverse_module_state->__pyx_n_s_now);
+  Py_VISIT(traverse_module_state->__pyx_n_s_nsec);
+  Py_VISIT(traverse_module_state->__pyx_n_s_r);
+  Py_VISIT(traverse_module_state->__pyx_n_s_sec);
+  Py_VISIT(traverse_module_state->__pyx_n_s_spec);
+  Py_VISIT(traverse_module_state->__pyx_n_s_test);
+  Py_VISIT(traverse_module_state->__pyx_n_s_time);
+  Py_VISIT(traverse_module_state->__pyx_n_s_timespec_add);
+  Py_VISIT(traverse_module_state->__pyx_n_s_to_timespec);
+  Py_VISIT(traverse_module_state->__pyx_n_s_ts);
+  Py_VISIT(traverse_module_state->__pyx_n_s_tv_nsec);
+  Py_VISIT(traverse_module_state->__pyx_n_s_tv_sec);
+  Py_VISIT(traverse_module_state->__pyx_n_s_value);
+  Py_VISIT(traverse_module_state->__pyx_float_1e9);
+  Py_VISIT(traverse_module_state->__pyx_tuple_);
+  Py_VISIT(traverse_module_state->__pyx_tuple__2);
+  Py_VISIT(traverse_module_state->__pyx_tuple__5);
+  Py_VISIT(traverse_module_state->__pyx_tuple__7);
+  Py_VISIT(traverse_module_state->__pyx_tuple__9);
+  Py_VISIT(traverse_module_state->__pyx_tuple__11);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__4);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__6);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__8);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__10);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__12);
+  return 0;
+}
+#endif
+/* #### Code section: module_state_defines ### */
+#define __pyx_d __pyx_mstate_global->__pyx_d
+#define __pyx_b __pyx_mstate_global->__pyx_b
+#define __pyx_cython_runtime __pyx_mstate_global->__pyx_cython_runtime
+#define __pyx_empty_tuple __pyx_mstate_global->__pyx_empty_tuple
+#define __pyx_empty_bytes __pyx_mstate_global->__pyx_empty_bytes
+#define __pyx_empty_unicode __pyx_mstate_global->__pyx_empty_unicode
+#ifdef __Pyx_CyFunction_USED
+#define __pyx_CyFunctionType __pyx_mstate_global->__pyx_CyFunctionType
+#endif
+#ifdef __Pyx_FusedFunction_USED
+#define __pyx_FusedFunctionType __pyx_mstate_global->__pyx_FusedFunctionType
+#endif
+#ifdef __Pyx_Generator_USED
+#define __pyx_GeneratorType __pyx_mstate_global->__pyx_GeneratorType
+#endif
+#ifdef __Pyx_IterableCoroutine_USED
+#define __pyx_IterableCoroutineType __pyx_mstate_global->__pyx_IterableCoroutineType
+#endif
+#ifdef __Pyx_Coroutine_USED
+#define __pyx_CoroutineAwaitType __pyx_mstate_global->__pyx_CoroutineAwaitType
+#endif
+#ifdef __Pyx_Coroutine_USED
+#define __pyx_CoroutineType __pyx_mstate_global->__pyx_CoroutineType
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#define __pyx_n_s_AssertionError __pyx_mstate_global->__pyx_n_s_AssertionError
+#define __pyx_n_s_KeyError __pyx_mstate_global->__pyx_n_s_KeyError
+#define __pyx_n_s_NANOSEC __pyx_mstate_global->__pyx_n_s_NANOSEC
+#define __pyx_kp_s_No_value_specified_for_struct_at __pyx_mstate_global->__pyx_kp_s_No_value_specified_for_struct_at
+#define __pyx_kp_s_No_value_specified_for_struct_at_2 __pyx_mstate_global->__pyx_kp_s_No_value_specified_for_struct_at_2
+#define __pyx_n_s_ValueError __pyx_mstate_global->__pyx_n_s_ValueError
+#define __pyx_n_s__13 __pyx_mstate_global->__pyx_n_s__13
+#define __pyx_n_s__3 __pyx_mstate_global->__pyx_n_s__3
+#define __pyx_n_s_asyncio_coroutines __pyx_mstate_global->__pyx_n_s_asyncio_coroutines
+#define __pyx_n_s_atimer__atimer __pyx_mstate_global->__pyx_n_s_atimer__atimer
+#define __pyx_kp_s_atimer__atimer_pyx __pyx_mstate_global->__pyx_kp_s_atimer__atimer_pyx
+#define __pyx_n_s_atimer_close __pyx_mstate_global->__pyx_n_s_atimer_close
+#define __pyx_n_s_atimer_init __pyx_mstate_global->__pyx_n_s_atimer_init
+#define __pyx_n_s_atimer_start __pyx_mstate_global->__pyx_n_s_atimer_start
+#define __pyx_n_s_cline_in_traceback __pyx_mstate_global->__pyx_n_s_cline_in_traceback
+#define __pyx_n_s_d_nsec __pyx_mstate_global->__pyx_n_s_d_nsec
+#define __pyx_n_s_d_sec __pyx_mstate_global->__pyx_n_s_d_sec
+#define __pyx_n_s_fd __pyx_mstate_global->__pyx_n_s_fd
+#define __pyx_n_s_import __pyx_mstate_global->__pyx_n_s_import
+#define __pyx_n_s_initializing __pyx_mstate_global->__pyx_n_s_initializing
+#define __pyx_n_s_interval __pyx_mstate_global->__pyx_n_s_interval
+#define __pyx_n_s_is_coroutine __pyx_mstate_global->__pyx_n_s_is_coroutine
+#define __pyx_n_s_main __pyx_mstate_global->__pyx_n_s_main
+#define __pyx_n_s_name __pyx_mstate_global->__pyx_n_s_name
+#define __pyx_n_s_now __pyx_mstate_global->__pyx_n_s_now
+#define __pyx_n_s_nsec __pyx_mstate_global->__pyx_n_s_nsec
+#define __pyx_n_s_r __pyx_mstate_global->__pyx_n_s_r
+#define __pyx_n_s_sec __pyx_mstate_global->__pyx_n_s_sec
+#define __pyx_n_s_spec __pyx_mstate_global->__pyx_n_s_spec
+#define __pyx_n_s_test __pyx_mstate_global->__pyx_n_s_test
+#define __pyx_n_s_time __pyx_mstate_global->__pyx_n_s_time
+#define __pyx_n_s_timespec_add __pyx_mstate_global->__pyx_n_s_timespec_add
+#define __pyx_n_s_to_timespec __pyx_mstate_global->__pyx_n_s_to_timespec
+#define __pyx_n_s_ts __pyx_mstate_global->__pyx_n_s_ts
+#define __pyx_n_s_tv_nsec __pyx_mstate_global->__pyx_n_s_tv_nsec
+#define __pyx_n_s_tv_sec __pyx_mstate_global->__pyx_n_s_tv_sec
+#define __pyx_n_s_value __pyx_mstate_global->__pyx_n_s_value
+#define __pyx_float_1e9 __pyx_mstate_global->__pyx_float_1e9
+#define __pyx_tuple_ __pyx_mstate_global->__pyx_tuple_
+#define __pyx_tuple__2 __pyx_mstate_global->__pyx_tuple__2
+#define __pyx_tuple__5 __pyx_mstate_global->__pyx_tuple__5
+#define __pyx_tuple__7 __pyx_mstate_global->__pyx_tuple__7
+#define __pyx_tuple__9 __pyx_mstate_global->__pyx_tuple__9
+#define __pyx_tuple__11 __pyx_mstate_global->__pyx_tuple__11
+#define __pyx_codeobj__4 __pyx_mstate_global->__pyx_codeobj__4
+#define __pyx_codeobj__6 __pyx_mstate_global->__pyx_codeobj__6
+#define __pyx_codeobj__8 __pyx_mstate_global->__pyx_codeobj__8
+#define __pyx_codeobj__10 __pyx_mstate_global->__pyx_codeobj__10
+#define __pyx_codeobj__12 __pyx_mstate_global->__pyx_codeobj__12
+/* #### Code section: module_code ### */
+
+/* "FromPyStructUtility":12
+ * 
+ * @cname("__pyx_convert__from_py_struct__timespec")
+ * cdef struct_type __pyx_convert__from_py_struct__timespec(obj) except *:             # <<<<<<<<<<<<<<
+ *     cdef struct_type result
+ *     if not PyMapping_Check(obj):
+ */
+
+static struct timespec __pyx_convert__from_py_struct__timespec(PyObject *__pyx_v_obj) {
+  struct timespec __pyx_v_result;
+  PyObject *__pyx_v_value = NULL;
+  struct timespec __pyx_r;
+  __Pyx_RefNannyDeclarations
+  int __pyx_t_1;
+  int __pyx_t_2;
+  PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_4 = NULL;
+  PyObject *__pyx_t_5 = NULL;
+  PyObject *__pyx_t_6 = NULL;
+  PyObject *__pyx_t_7 = NULL;
+  PyObject *__pyx_t_8 = NULL;
+  PyObject *__pyx_t_9 = NULL;
+  time_t __pyx_t_10;
+  long __pyx_t_11;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__pyx_convert__from_py_struct__timespec", 0);
+
+  /* "FromPyStructUtility":14
+ * cdef struct_type __pyx_convert__from_py_struct__timespec(obj) except *:
+ *     cdef struct_type result
+ *     if not PyMapping_Check(obj):             # <<<<<<<<<<<<<<
+ *         __Pyx_RaiseUnexpectedTypeError(b"a mapping", obj)
+ * 
+ */
+  __pyx_t_1 = (!PyMapping_Check(__pyx_v_obj));
+  if (__pyx_t_1) {
+
+    /* "FromPyStructUtility":15
+ *     cdef struct_type result
+ *     if not PyMapping_Check(obj):
+ *         __Pyx_RaiseUnexpectedTypeError(b"a mapping", obj)             # <<<<<<<<<<<<<<
+ * 
+ *     try:
+ */
+    __pyx_t_2 = __Pyx_RaiseUnexpectedTypeError(((char const *)"a mapping"), __pyx_v_obj); if (unlikely(__pyx_t_2 == ((int)0))) __PYX_ERR(1, 15, __pyx_L1_error)
+
+    /* "FromPyStructUtility":14
+ * cdef struct_type __pyx_convert__from_py_struct__timespec(obj) except *:
+ *     cdef struct_type result
+ *     if not PyMapping_Check(obj):             # <<<<<<<<<<<<<<
+ *         __Pyx_RaiseUnexpectedTypeError(b"a mapping", obj)
+ * 
+ */
+  }
+
+  /* "FromPyStructUtility":17
+ *         __Pyx_RaiseUnexpectedTypeError(b"a mapping", obj)
+ * 
+ *     try:             # <<<<<<<<<<<<<<
+ *         value = obj['tv_sec']
+ *     except KeyError:
+ */
+  {
+    __Pyx_PyThreadState_declare
+    __Pyx_PyThreadState_assign
+    __Pyx_ExceptionSave(&__pyx_t_3, &__pyx_t_4, &__pyx_t_5);
+    __Pyx_XGOTREF(__pyx_t_3);
+    __Pyx_XGOTREF(__pyx_t_4);
+    __Pyx_XGOTREF(__pyx_t_5);
+    /*try:*/ {
+
+      /* "FromPyStructUtility":18
+ * 
+ *     try:
+ *         value = obj['tv_sec']             # <<<<<<<<<<<<<<
+ *     except KeyError:
+ *         raise ValueError("No value specified for struct attribute 'tv_sec'")
+ */
+      __pyx_t_6 = __Pyx_PyObject_Dict_GetItem(__pyx_v_obj, __pyx_n_s_tv_sec); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 18, __pyx_L4_error)
+      __Pyx_GOTREF(__pyx_t_6);
+      __pyx_v_value = __pyx_t_6;
+      __pyx_t_6 = 0;
+
+      /* "FromPyStructUtility":17
+ *         __Pyx_RaiseUnexpectedTypeError(b"a mapping", obj)
+ * 
+ *     try:             # <<<<<<<<<<<<<<
+ *         value = obj['tv_sec']
+ *     except KeyError:
+ */
+    }
+    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+    goto __pyx_L9_try_end;
+    __pyx_L4_error:;
+    __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+
+    /* "FromPyStructUtility":19
+ *     try:
+ *         value = obj['tv_sec']
+ *     except KeyError:             # <<<<<<<<<<<<<<
+ *         raise ValueError("No value specified for struct attribute 'tv_sec'")
+ *     result.tv_sec = value
+ */
+    __pyx_t_2 = __Pyx_PyErr_ExceptionMatches(__pyx_builtin_KeyError);
+    if (__pyx_t_2) {
+      __Pyx_AddTraceback("FromPyStructUtility.__pyx_convert__from_py_struct__timespec", __pyx_clineno, __pyx_lineno, __pyx_filename);
+      if (__Pyx_GetException(&__pyx_t_6, &__pyx_t_7, &__pyx_t_8) < 0) __PYX_ERR(1, 19, __pyx_L6_except_error)
+      __Pyx_XGOTREF(__pyx_t_6);
+      __Pyx_XGOTREF(__pyx_t_7);
+      __Pyx_XGOTREF(__pyx_t_8);
+
+      /* "FromPyStructUtility":20
+ *         value = obj['tv_sec']
+ *     except KeyError:
+ *         raise ValueError("No value specified for struct attribute 'tv_sec'")             # <<<<<<<<<<<<<<
+ *     result.tv_sec = value
+ *     try:
+ */
+      __pyx_t_9 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 20, __pyx_L6_except_error)
+      __Pyx_GOTREF(__pyx_t_9);
+      __Pyx_Raise(__pyx_t_9, 0, 0, 0);
+      __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+      __PYX_ERR(1, 20, __pyx_L6_except_error)
+    }
+    goto __pyx_L6_except_error;
+
+    /* "FromPyStructUtility":17
+ *         __Pyx_RaiseUnexpectedTypeError(b"a mapping", obj)
+ * 
+ *     try:             # <<<<<<<<<<<<<<
+ *         value = obj['tv_sec']
+ *     except KeyError:
+ */
+    __pyx_L6_except_error:;
+    __Pyx_XGIVEREF(__pyx_t_3);
+    __Pyx_XGIVEREF(__pyx_t_4);
+    __Pyx_XGIVEREF(__pyx_t_5);
+    __Pyx_ExceptionReset(__pyx_t_3, __pyx_t_4, __pyx_t_5);
+    goto __pyx_L1_error;
+    __pyx_L9_try_end:;
+  }
+
+  /* "FromPyStructUtility":21
+ *     except KeyError:
+ *         raise ValueError("No value specified for struct attribute 'tv_sec'")
+ *     result.tv_sec = value             # <<<<<<<<<<<<<<
+ *     try:
+ *         value = obj['tv_nsec']
+ */
+  __pyx_t_10 = __Pyx_PyInt_As_time_t(__pyx_v_value); if (unlikely((__pyx_t_10 == ((time_t)-1)) && PyErr_Occurred())) __PYX_ERR(1, 21, __pyx_L1_error)
+  __pyx_v_result.tv_sec = __pyx_t_10;
+
+  /* "FromPyStructUtility":22
+ *         raise ValueError("No value specified for struct attribute 'tv_sec'")
+ *     result.tv_sec = value
+ *     try:             # <<<<<<<<<<<<<<
+ *         value = obj['tv_nsec']
+ *     except KeyError:
+ */
+  {
+    __Pyx_PyThreadState_declare
+    __Pyx_PyThreadState_assign
+    __Pyx_ExceptionSave(&__pyx_t_5, &__pyx_t_4, &__pyx_t_3);
+    __Pyx_XGOTREF(__pyx_t_5);
+    __Pyx_XGOTREF(__pyx_t_4);
+    __Pyx_XGOTREF(__pyx_t_3);
+    /*try:*/ {
+
+      /* "FromPyStructUtility":23
+ *     result.tv_sec = value
+ *     try:
+ *         value = obj['tv_nsec']             # <<<<<<<<<<<<<<
+ *     except KeyError:
+ *         raise ValueError("No value specified for struct attribute 'tv_nsec'")
+ */
+      __pyx_t_8 = __Pyx_PyObject_Dict_GetItem(__pyx_v_obj, __pyx_n_s_tv_nsec); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 23, __pyx_L12_error)
+      __Pyx_GOTREF(__pyx_t_8);
+      __Pyx_DECREF_SET(__pyx_v_value, __pyx_t_8);
+      __pyx_t_8 = 0;
+
+      /* "FromPyStructUtility":22
+ *         raise ValueError("No value specified for struct attribute 'tv_sec'")
+ *     result.tv_sec = value
+ *     try:             # <<<<<<<<<<<<<<
+ *         value = obj['tv_nsec']
+ *     except KeyError:
+ */
+    }
+    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+    goto __pyx_L17_try_end;
+    __pyx_L12_error:;
+    __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
+    __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
+    __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
+
+    /* "FromPyStructUtility":24
+ *     try:
+ *         value = obj['tv_nsec']
+ *     except KeyError:             # <<<<<<<<<<<<<<
+ *         raise ValueError("No value specified for struct attribute 'tv_nsec'")
+ *     result.tv_nsec = value
+ */
+    __pyx_t_2 = __Pyx_PyErr_ExceptionMatches(__pyx_builtin_KeyError);
+    if (__pyx_t_2) {
+      __Pyx_AddTraceback("FromPyStructUtility.__pyx_convert__from_py_struct__timespec", __pyx_clineno, __pyx_lineno, __pyx_filename);
+      if (__Pyx_GetException(&__pyx_t_8, &__pyx_t_7, &__pyx_t_6) < 0) __PYX_ERR(1, 24, __pyx_L14_except_error)
+      __Pyx_XGOTREF(__pyx_t_8);
+      __Pyx_XGOTREF(__pyx_t_7);
+      __Pyx_XGOTREF(__pyx_t_6);
+
+      /* "FromPyStructUtility":25
+ *         value = obj['tv_nsec']
+ *     except KeyError:
+ *         raise ValueError("No value specified for struct attribute 'tv_nsec'")             # <<<<<<<<<<<<<<
+ *     result.tv_nsec = value
+ *     return result
+ */
+      __pyx_t_9 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 25, __pyx_L14_except_error)
+      __Pyx_GOTREF(__pyx_t_9);
+      __Pyx_Raise(__pyx_t_9, 0, 0, 0);
+      __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+      __PYX_ERR(1, 25, __pyx_L14_except_error)
+    }
+    goto __pyx_L14_except_error;
+
+    /* "FromPyStructUtility":22
+ *         raise ValueError("No value specified for struct attribute 'tv_sec'")
+ *     result.tv_sec = value
+ *     try:             # <<<<<<<<<<<<<<
+ *         value = obj['tv_nsec']
+ *     except KeyError:
+ */
+    __pyx_L14_except_error:;
+    __Pyx_XGIVEREF(__pyx_t_5);
+    __Pyx_XGIVEREF(__pyx_t_4);
+    __Pyx_XGIVEREF(__pyx_t_3);
+    __Pyx_ExceptionReset(__pyx_t_5, __pyx_t_4, __pyx_t_3);
+    goto __pyx_L1_error;
+    __pyx_L17_try_end:;
+  }
+
+  /* "FromPyStructUtility":26
+ *     except KeyError:
+ *         raise ValueError("No value specified for struct attribute 'tv_nsec'")
+ *     result.tv_nsec = value             # <<<<<<<<<<<<<<
+ *     return result
+ * 
+ */
+  __pyx_t_11 = __Pyx_PyInt_As_long(__pyx_v_value); if (unlikely((__pyx_t_11 == (long)-1) && PyErr_Occurred())) __PYX_ERR(1, 26, __pyx_L1_error)
+  __pyx_v_result.tv_nsec = __pyx_t_11;
+
+  /* "FromPyStructUtility":27
+ *         raise ValueError("No value specified for struct attribute 'tv_nsec'")
+ *     result.tv_nsec = value
+ *     return result             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_r = __pyx_v_result;
+  goto __pyx_L0;
+
+  /* "FromPyStructUtility":12
+ * 
+ * @cname("__pyx_convert__from_py_struct__timespec")
+ * cdef struct_type __pyx_convert__from_py_struct__timespec(obj) except *:             # <<<<<<<<<<<<<<
+ *     cdef struct_type result
+ *     if not PyMapping_Check(obj):
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_6);
+  __Pyx_XDECREF(__pyx_t_7);
+  __Pyx_XDECREF(__pyx_t_8);
+  __Pyx_XDECREF(__pyx_t_9);
+  __Pyx_AddTraceback("FromPyStructUtility.__pyx_convert__from_py_struct__timespec", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_pretend_to_initialize(&__pyx_r);
+  __pyx_L0:;
+  __Pyx_XDECREF(__pyx_v_value);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
 
 /* "atimer/_atimer.pyx":39
  *     int timerfd_gettime(int, itimerspec*)
  * 
  * def atimer_init():             # <<<<<<<<<<<<<<
  *     # CLOCK_BOOTIME: count number of expirations when running machine is
  *     # suspended
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_6atimer_7_atimer_1atimer_init(PyObject *__pyx_self, CYTHON_UNUSED PyObject *unused); /*proto*/
 static PyMethodDef __pyx_mdef_6atimer_7_atimer_1atimer_init = {"atimer_init", (PyCFunction)__pyx_pw_6atimer_7_atimer_1atimer_init, METH_NOARGS, 0};
 static PyObject *__pyx_pw_6atimer_7_atimer_1atimer_init(PyObject *__pyx_self, CYTHON_UNUSED PyObject *unused) {
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("atimer_init (wrapper)", 0);
   __pyx_r = __pyx_pf_6atimer_7_atimer_atimer_init(__pyx_self);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
@@ -1440,66 +2733,84 @@
  * 
  * def atimer_start(int fd, double interval):             # <<<<<<<<<<<<<<
  *     cdef itimerspec ts
  *     cdef timespec now
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_6atimer_7_atimer_3atimer_start(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyMethodDef __pyx_mdef_6atimer_7_atimer_3atimer_start = {"atimer_start", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_6atimer_7_atimer_3atimer_start, METH_VARARGS|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_6atimer_7_atimer_3atimer_start(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_6atimer_7_atimer_3atimer_start(PyObject *__pyx_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+); /*proto*/
+static PyMethodDef __pyx_mdef_6atimer_7_atimer_3atimer_start = {"atimer_start", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_6atimer_7_atimer_3atimer_start, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_6atimer_7_atimer_3atimer_start(PyObject *__pyx_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+) {
   int __pyx_v_fd;
   double __pyx_v_interval;
+  #if !CYTHON_METH_FASTCALL
+  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #endif
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("atimer_start (wrapper)", 0);
   {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_fd,&__pyx_n_s_interval,0};
+    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_fd,&__pyx_n_s_interval,0};
     PyObject* values[2] = {0,0};
-    if (unlikely(__pyx_kwds)) {
+    if (__pyx_kwds) {
       Py_ssize_t kw_args;
-      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
-      switch (pos_args) {
-        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+      switch (__pyx_nargs) {
+        case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
-        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
-      kw_args = PyDict_Size(__pyx_kwds);
-      switch (pos_args) {
+      kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
+      switch (__pyx_nargs) {
         case  0:
-        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_fd)) != 0)) kw_args--;
+        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_fd)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 46, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
-        if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_interval)) != 0)) kw_args--;
+        if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_interval)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 46, __pyx_L3_error)
         else {
           __Pyx_RaiseArgtupleInvalid("atimer_start", 1, 2, 2, 1); __PYX_ERR(0, 46, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "atimer_start") < 0)) __PYX_ERR(0, 46, __pyx_L3_error)
+        const Py_ssize_t kwd_pos_args = __pyx_nargs;
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "atimer_start") < 0)) __PYX_ERR(0, 46, __pyx_L3_error)
       }
-    } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
+    } else if (unlikely(__pyx_nargs != 2)) {
       goto __pyx_L5_argtuple_error;
     } else {
-      values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
-      values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+      values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+      values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
     }
     __pyx_v_fd = __Pyx_PyInt_As_int(values[0]); if (unlikely((__pyx_v_fd == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 46, __pyx_L3_error)
     __pyx_v_interval = __pyx_PyFloat_AsDouble(values[1]); if (unlikely((__pyx_v_interval == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 46, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("atimer_start", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 46, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("atimer_start", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 46, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("atimer._atimer.atimer_start", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6atimer_7_atimer_2atimer_start(__pyx_self, __pyx_v_fd, __pyx_v_interval);
 
@@ -1517,22 +2828,21 @@
   long __pyx_v_d_nsec;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
-  PyObject *(*__pyx_t_5)(PyObject *);
-  time_t __pyx_t_6;
-  long __pyx_t_7;
-  PyObject *__pyx_t_8 = NULL;
+  int __pyx_t_5;
+  PyObject *(*__pyx_t_6)(PyObject *);
+  time_t __pyx_t_7;
+  long __pyx_t_8;
   PyObject *__pyx_t_9 = NULL;
-  int __pyx_t_10;
-  PyObject *__pyx_t_11 = NULL;
-  struct timespec __pyx_t_12;
+  PyObject *__pyx_t_10 = NULL;
+  struct timespec __pyx_t_11;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("atimer_start", 0);
 
   /* "atimer/_atimer.pyx":52
  *     cdef long nsec, d_nsec
@@ -1542,29 +2852,34 @@
  *     # sync monotonic clock to the edge of realtime clock, then use
  */
   __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_to_timespec); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 52, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = PyFloat_FromDouble(__pyx_v_interval); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 52, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = NULL;
+  __pyx_t_5 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
+      __pyx_t_5 = 1;
     }
   }
-  __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_t_3) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3);
-  __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 52, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  {
+    PyObject *__pyx_callargs[2] = {__pyx_t_4, __pyx_t_3};
+    __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
+    __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 52, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  }
   if ((likely(PyTuple_CheckExact(__pyx_t_1))) || (PyList_CheckExact(__pyx_t_1))) {
     PyObject* sequence = __pyx_t_1;
     Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
     if (unlikely(size != 2)) {
       if (size > 2) __Pyx_RaiseTooManyValuesError(2);
       else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
       __PYX_ERR(0, 52, __pyx_L1_error)
@@ -1587,36 +2902,36 @@
     #endif
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   } else {
     Py_ssize_t index = -1;
     __pyx_t_4 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 52, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_5 = Py_TYPE(__pyx_t_4)->tp_iternext;
-    index = 0; __pyx_t_2 = __pyx_t_5(__pyx_t_4); if (unlikely(!__pyx_t_2)) goto __pyx_L3_unpacking_failed;
+    __pyx_t_6 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_4);
+    index = 0; __pyx_t_2 = __pyx_t_6(__pyx_t_4); if (unlikely(!__pyx_t_2)) goto __pyx_L3_unpacking_failed;
     __Pyx_GOTREF(__pyx_t_2);
-    index = 1; __pyx_t_3 = __pyx_t_5(__pyx_t_4); if (unlikely(!__pyx_t_3)) goto __pyx_L3_unpacking_failed;
+    index = 1; __pyx_t_3 = __pyx_t_6(__pyx_t_4); if (unlikely(!__pyx_t_3)) goto __pyx_L3_unpacking_failed;
     __Pyx_GOTREF(__pyx_t_3);
-    if (__Pyx_IternextUnpackEndCheck(__pyx_t_5(__pyx_t_4), 2) < 0) __PYX_ERR(0, 52, __pyx_L1_error)
-    __pyx_t_5 = NULL;
+    if (__Pyx_IternextUnpackEndCheck(__pyx_t_6(__pyx_t_4), 2) < 0) __PYX_ERR(0, 52, __pyx_L1_error)
+    __pyx_t_6 = NULL;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     goto __pyx_L4_unpacking_done;
     __pyx_L3_unpacking_failed:;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_5 = NULL;
+    __pyx_t_6 = NULL;
     if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
     __PYX_ERR(0, 52, __pyx_L1_error)
     __pyx_L4_unpacking_done:;
   }
-  __pyx_t_6 = __Pyx_PyInt_As_time_t(__pyx_t_2); if (unlikely((__pyx_t_6 == ((time_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 52, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyInt_As_time_t(__pyx_t_2); if (unlikely((__pyx_t_7 == ((time_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 52, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_7 = __Pyx_PyInt_As_long(__pyx_t_3); if (unlikely((__pyx_t_7 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 52, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyInt_As_long(__pyx_t_3); if (unlikely((__pyx_t_8 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 52, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_v_sec = __pyx_t_6;
-  __pyx_v_nsec = __pyx_t_7;
+  __pyx_v_sec = __pyx_t_7;
+  __pyx_v_nsec = __pyx_t_8;
 
   /* "atimer/_atimer.pyx":56
  *     # sync monotonic clock to the edge of realtime clock, then use
  *     # TFD_TIMER_ABSTIME to achieve first expiration at synchronized time
  *     clock_gettime(CLOCK_BOOTTIME, &now)             # <<<<<<<<<<<<<<
  *     d_sec, d_nsec = to_timespec(-time.time() % interval)
  *     ts.it_value = timespec_add(now, d_sec, d_nsec)
@@ -1630,57 +2945,67 @@
  *     ts.it_value = timespec_add(now, d_sec, d_nsec)
  * 
  */
   __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_to_timespec); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 57, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_time); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 57, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_time); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 57, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_8);
+  __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_time); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 57, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_9);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_t_4 = NULL;
-  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_8))) {
-    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_8);
+  __pyx_t_5 = 0;
+  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_9))) {
+    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_9);
     if (likely(__pyx_t_4)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_8);
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_9);
       __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_8, function);
+      __Pyx_DECREF_SET(__pyx_t_9, function);
+      __pyx_t_5 = 1;
     }
   }
-  __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_8, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_8);
-  __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 57, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  __pyx_t_8 = PyNumber_Negative(__pyx_t_2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 57, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_8);
+  {
+    PyObject *__pyx_callargs[1] = {__pyx_t_4, };
+    __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_9, __pyx_callargs+1-__pyx_t_5, 0+__pyx_t_5);
+    __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 57, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+  }
+  __pyx_t_9 = PyNumber_Negative(__pyx_t_2); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 57, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_9);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = PyFloat_FromDouble(__pyx_v_interval); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 57, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = PyNumber_Remainder(__pyx_t_8, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 57, __pyx_L1_error)
+  __pyx_t_4 = PyNumber_Remainder(__pyx_t_9, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 57, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+  __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = NULL;
+  __pyx_t_5 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_2)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_2);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
+      __pyx_t_5 = 1;
     }
   }
-  __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_2, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4);
-  __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 57, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  {
+    PyObject *__pyx_callargs[2] = {__pyx_t_2, __pyx_t_4};
+    __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
+    __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 57, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  }
   if ((likely(PyTuple_CheckExact(__pyx_t_1))) || (PyList_CheckExact(__pyx_t_1))) {
     PyObject* sequence = __pyx_t_1;
     Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
     if (unlikely(size != 2)) {
       if (size > 2) __Pyx_RaiseTooManyValuesError(2);
       else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
       __PYX_ERR(0, 57, __pyx_L1_error)
@@ -1703,109 +3028,78 @@
     #endif
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   } else {
     Py_ssize_t index = -1;
     __pyx_t_2 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 57, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_5 = Py_TYPE(__pyx_t_2)->tp_iternext;
-    index = 0; __pyx_t_3 = __pyx_t_5(__pyx_t_2); if (unlikely(!__pyx_t_3)) goto __pyx_L5_unpacking_failed;
+    __pyx_t_6 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_2);
+    index = 0; __pyx_t_3 = __pyx_t_6(__pyx_t_2); if (unlikely(!__pyx_t_3)) goto __pyx_L5_unpacking_failed;
     __Pyx_GOTREF(__pyx_t_3);
-    index = 1; __pyx_t_4 = __pyx_t_5(__pyx_t_2); if (unlikely(!__pyx_t_4)) goto __pyx_L5_unpacking_failed;
+    index = 1; __pyx_t_4 = __pyx_t_6(__pyx_t_2); if (unlikely(!__pyx_t_4)) goto __pyx_L5_unpacking_failed;
     __Pyx_GOTREF(__pyx_t_4);
-    if (__Pyx_IternextUnpackEndCheck(__pyx_t_5(__pyx_t_2), 2) < 0) __PYX_ERR(0, 57, __pyx_L1_error)
-    __pyx_t_5 = NULL;
+    if (__Pyx_IternextUnpackEndCheck(__pyx_t_6(__pyx_t_2), 2) < 0) __PYX_ERR(0, 57, __pyx_L1_error)
+    __pyx_t_6 = NULL;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     goto __pyx_L6_unpacking_done;
     __pyx_L5_unpacking_failed:;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_5 = NULL;
+    __pyx_t_6 = NULL;
     if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
     __PYX_ERR(0, 57, __pyx_L1_error)
     __pyx_L6_unpacking_done:;
   }
-  __pyx_t_6 = __Pyx_PyInt_As_time_t(__pyx_t_3); if (unlikely((__pyx_t_6 == ((time_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 57, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyInt_As_time_t(__pyx_t_3); if (unlikely((__pyx_t_7 == ((time_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 57, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_7 = __Pyx_PyInt_As_long(__pyx_t_4); if (unlikely((__pyx_t_7 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 57, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyInt_As_long(__pyx_t_4); if (unlikely((__pyx_t_8 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 57, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_v_d_sec = __pyx_t_6;
-  __pyx_v_d_nsec = __pyx_t_7;
+  __pyx_v_d_sec = __pyx_t_7;
+  __pyx_v_d_nsec = __pyx_t_8;
 
   /* "atimer/_atimer.pyx":58
  *     clock_gettime(CLOCK_BOOTTIME, &now)
  *     d_sec, d_nsec = to_timespec(-time.time() % interval)
  *     ts.it_value = timespec_add(now, d_sec, d_nsec)             # <<<<<<<<<<<<<<
  * 
  *     ts.it_interval.tv_sec = sec
  */
   __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_timespec_add); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 58, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_3 = __pyx_convert__to_py_struct__timespec(__pyx_v_now); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 58, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_2 = __Pyx_PyInt_From_time_t(__pyx_v_d_sec); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 58, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_8 = __Pyx_PyInt_From_long(__pyx_v_d_nsec); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 58, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_8);
-  __pyx_t_9 = NULL;
-  __pyx_t_10 = 0;
+  __pyx_t_9 = __Pyx_PyInt_From_long(__pyx_v_d_nsec); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 58, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_9);
+  __pyx_t_10 = NULL;
+  __pyx_t_5 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
-    __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_4);
-    if (likely(__pyx_t_9)) {
+    __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_4);
+    if (likely(__pyx_t_10)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
-      __Pyx_INCREF(__pyx_t_9);
+      __Pyx_INCREF(__pyx_t_10);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_4, function);
-      __pyx_t_10 = 1;
+      __pyx_t_5 = 1;
     }
   }
-  #if CYTHON_FAST_PYCALL
-  if (PyFunction_Check(__pyx_t_4)) {
-    PyObject *__pyx_temp[4] = {__pyx_t_9, __pyx_t_3, __pyx_t_2, __pyx_t_8};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_10, 3+__pyx_t_10); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 58, __pyx_L1_error)
-    __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
-    __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  } else
-  #endif
-  #if CYTHON_FAST_PYCCALL
-  if (__Pyx_PyFastCFunction_Check(__pyx_t_4)) {
-    PyObject *__pyx_temp[4] = {__pyx_t_9, __pyx_t_3, __pyx_t_2, __pyx_t_8};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_10, 3+__pyx_t_10); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 58, __pyx_L1_error)
-    __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
-    __Pyx_GOTREF(__pyx_t_1);
+  {
+    PyObject *__pyx_callargs[4] = {__pyx_t_10, __pyx_t_3, __pyx_t_2, __pyx_t_9};
+    __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_5, 3+__pyx_t_5);
+    __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  } else
-  #endif
-  {
-    __pyx_t_11 = PyTuple_New(3+__pyx_t_10); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 58, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_11);
-    if (__pyx_t_9) {
-      __Pyx_GIVEREF(__pyx_t_9); PyTuple_SET_ITEM(__pyx_t_11, 0, __pyx_t_9); __pyx_t_9 = NULL;
-    }
-    __Pyx_GIVEREF(__pyx_t_3);
-    PyTuple_SET_ITEM(__pyx_t_11, 0+__pyx_t_10, __pyx_t_3);
-    __Pyx_GIVEREF(__pyx_t_2);
-    PyTuple_SET_ITEM(__pyx_t_11, 1+__pyx_t_10, __pyx_t_2);
-    __Pyx_GIVEREF(__pyx_t_8);
-    PyTuple_SET_ITEM(__pyx_t_11, 2+__pyx_t_10, __pyx_t_8);
-    __pyx_t_3 = 0;
-    __pyx_t_2 = 0;
-    __pyx_t_8 = 0;
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_11, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 58, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 58, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   }
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_12 = __pyx_convert__from_py_struct__timespec(__pyx_t_1); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 58, __pyx_L1_error)
+  __pyx_t_11 = __pyx_convert__from_py_struct__timespec(__pyx_t_1); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 58, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_v_ts.it_value = __pyx_t_12;
+  __pyx_v_ts.it_value = __pyx_t_11;
 
   /* "atimer/_atimer.pyx":60
  *     ts.it_value = timespec_add(now, d_sec, d_nsec)
  * 
  *     ts.it_interval.tv_sec = sec             # <<<<<<<<<<<<<<
  *     ts.it_interval.tv_nsec = nsec
  * 
@@ -1845,17 +3139,16 @@
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
-  __Pyx_XDECREF(__pyx_t_8);
   __Pyx_XDECREF(__pyx_t_9);
-  __Pyx_XDECREF(__pyx_t_11);
+  __Pyx_XDECREF(__pyx_t_10);
   __Pyx_AddTraceback("atimer._atimer.atimer_start", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
@@ -1865,34 +3158,78 @@
  * 
  * def atimer_close(int fd):             # <<<<<<<<<<<<<<
  *     cdef int r
  *     cdef itimerspec ts
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_6atimer_7_atimer_5atimer_close(PyObject *__pyx_self, PyObject *__pyx_arg_fd); /*proto*/
-static PyMethodDef __pyx_mdef_6atimer_7_atimer_5atimer_close = {"atimer_close", (PyCFunction)__pyx_pw_6atimer_7_atimer_5atimer_close, METH_O, 0};
-static PyObject *__pyx_pw_6atimer_7_atimer_5atimer_close(PyObject *__pyx_self, PyObject *__pyx_arg_fd) {
+static PyObject *__pyx_pw_6atimer_7_atimer_5atimer_close(PyObject *__pyx_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+); /*proto*/
+static PyMethodDef __pyx_mdef_6atimer_7_atimer_5atimer_close = {"atimer_close", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_6atimer_7_atimer_5atimer_close, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_6atimer_7_atimer_5atimer_close(PyObject *__pyx_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+) {
   int __pyx_v_fd;
+  #if !CYTHON_METH_FASTCALL
+  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #endif
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("atimer_close (wrapper)", 0);
-  assert(__pyx_arg_fd); {
-    __pyx_v_fd = __Pyx_PyInt_As_int(__pyx_arg_fd); if (unlikely((__pyx_v_fd == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 65, __pyx_L3_error)
+  {
+    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_fd,0};
+    PyObject* values[1] = {0};
+    if (__pyx_kwds) {
+      Py_ssize_t kw_args;
+      switch (__pyx_nargs) {
+        case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+        CYTHON_FALLTHROUGH;
+        case  0: break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+      kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
+      switch (__pyx_nargs) {
+        case  0:
+        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_fd)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 65, __pyx_L3_error)
+        else goto __pyx_L5_argtuple_error;
+      }
+      if (unlikely(kw_args > 0)) {
+        const Py_ssize_t kwd_pos_args = __pyx_nargs;
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "atimer_close") < 0)) __PYX_ERR(0, 65, __pyx_L3_error)
+      }
+    } else if (unlikely(__pyx_nargs != 1)) {
+      goto __pyx_L5_argtuple_error;
+    } else {
+      values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+    }
+    __pyx_v_fd = __Pyx_PyInt_As_int(values[0]); if (unlikely((__pyx_v_fd == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 65, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
+  __pyx_L5_argtuple_error:;
+  __Pyx_RaiseArgtupleInvalid("atimer_close", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 65, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("atimer._atimer.atimer_close", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_6atimer_7_atimer_4atimer_close(__pyx_self, ((int)__pyx_v_fd));
+  __pyx_r = __pyx_pf_6atimer_7_atimer_4atimer_close(__pyx_self, __pyx_v_fd);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_6atimer_7_atimer_4atimer_close(CYTHON_UNUSED PyObject *__pyx_self, int __pyx_v_fd) {
@@ -1998,50 +3335,95 @@
  * 
  * def to_timespec(double value):             # <<<<<<<<<<<<<<
  *     """
  *     Convert float number to `timespec` value.
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_6atimer_7_atimer_7to_timespec(PyObject *__pyx_self, PyObject *__pyx_arg_value); /*proto*/
-static char __pyx_doc_6atimer_7_atimer_6to_timespec[] = "\n    Convert float number to `timespec` value.\n\n    Tuple is returned\n\n    - number of seconds\n    - number of nanoseconds\n    ";
-static PyMethodDef __pyx_mdef_6atimer_7_atimer_7to_timespec = {"to_timespec", (PyCFunction)__pyx_pw_6atimer_7_atimer_7to_timespec, METH_O, __pyx_doc_6atimer_7_atimer_6to_timespec};
-static PyObject *__pyx_pw_6atimer_7_atimer_7to_timespec(PyObject *__pyx_self, PyObject *__pyx_arg_value) {
+static PyObject *__pyx_pw_6atimer_7_atimer_7to_timespec(PyObject *__pyx_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+); /*proto*/
+PyDoc_STRVAR(__pyx_doc_6atimer_7_atimer_6to_timespec, "\n    Convert float number to `timespec` value.\n\n    Tuple is returned\n\n    - number of seconds\n    - number of nanoseconds\n    ");
+static PyMethodDef __pyx_mdef_6atimer_7_atimer_7to_timespec = {"to_timespec", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_6atimer_7_atimer_7to_timespec, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_6atimer_7_atimer_6to_timespec};
+static PyObject *__pyx_pw_6atimer_7_atimer_7to_timespec(PyObject *__pyx_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+) {
   double __pyx_v_value;
+  #if !CYTHON_METH_FASTCALL
+  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #endif
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("to_timespec (wrapper)", 0);
-  assert(__pyx_arg_value); {
-    __pyx_v_value = __pyx_PyFloat_AsDouble(__pyx_arg_value); if (unlikely((__pyx_v_value == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 79, __pyx_L3_error)
+  {
+    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_value,0};
+    PyObject* values[1] = {0};
+    if (__pyx_kwds) {
+      Py_ssize_t kw_args;
+      switch (__pyx_nargs) {
+        case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+        CYTHON_FALLTHROUGH;
+        case  0: break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+      kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
+      switch (__pyx_nargs) {
+        case  0:
+        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_value)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 79, __pyx_L3_error)
+        else goto __pyx_L5_argtuple_error;
+      }
+      if (unlikely(kw_args > 0)) {
+        const Py_ssize_t kwd_pos_args = __pyx_nargs;
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "to_timespec") < 0)) __PYX_ERR(0, 79, __pyx_L3_error)
+      }
+    } else if (unlikely(__pyx_nargs != 1)) {
+      goto __pyx_L5_argtuple_error;
+    } else {
+      values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+    }
+    __pyx_v_value = __pyx_PyFloat_AsDouble(values[0]); if (unlikely((__pyx_v_value == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 79, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
+  __pyx_L5_argtuple_error:;
+  __Pyx_RaiseArgtupleInvalid("to_timespec", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 79, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("atimer._atimer.to_timespec", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_6atimer_7_atimer_6to_timespec(__pyx_self, ((double)__pyx_v_value));
+  __pyx_r = __pyx_pf_6atimer_7_atimer_6to_timespec(__pyx_self, __pyx_v_value);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_6atimer_7_atimer_6to_timespec(CYTHON_UNUSED PyObject *__pyx_self, double __pyx_v_value) {
   time_t __pyx_v_sec;
   long __pyx_v_nsec;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
+  int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
-  long __pyx_t_4;
+  PyObject *__pyx_t_4 = NULL;
+  long __pyx_t_5;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("to_timespec", 0);
 
   /* "atimer/_atimer.pyx":91
  *     cdef long nsec
@@ -2056,78 +3438,81 @@
  *     sec = <int> value
  * 
  *     assert sec <= value             # <<<<<<<<<<<<<<
  *     nsec = (value - sec) * NANOSEC
  * 
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
-  if (unlikely(!Py_OptimizeFlag)) {
-    if (unlikely(!((__pyx_v_sec <= __pyx_v_value) != 0))) {
-      PyErr_SetNone(PyExc_AssertionError);
+  if (unlikely(__pyx_assertions_enabled())) {
+    __pyx_t_1 = (__pyx_v_sec <= __pyx_v_value);
+    if (unlikely(!__pyx_t_1)) {
+      __Pyx_Raise(__pyx_builtin_AssertionError, 0, 0, 0);
       __PYX_ERR(0, 93, __pyx_L1_error)
     }
   }
+  #else
+  if ((1)); else __PYX_ERR(0, 93, __pyx_L1_error)
   #endif
 
   /* "atimer/_atimer.pyx":94
  * 
  *     assert sec <= value
  *     nsec = (value - sec) * NANOSEC             # <<<<<<<<<<<<<<
  * 
  *     return sec, nsec
  */
-  __pyx_t_1 = PyFloat_FromDouble((__pyx_v_value - __pyx_v_sec)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 94, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_NANOSEC); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 94, __pyx_L1_error)
+  __pyx_t_2 = PyFloat_FromDouble((__pyx_v_value - __pyx_v_sec)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 94, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = PyNumber_Multiply(__pyx_t_1, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 94, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_NANOSEC); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 94, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_4 = PyNumber_Multiply(__pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 94, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_4 = __Pyx_PyInt_As_long(__pyx_t_3); if (unlikely((__pyx_t_4 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 94, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_v_nsec = __pyx_t_4;
+  __pyx_t_5 = __Pyx_PyInt_As_long(__pyx_t_4); if (unlikely((__pyx_t_5 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 94, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_v_nsec = __pyx_t_5;
 
   /* "atimer/_atimer.pyx":96
  *     nsec = (value - sec) * NANOSEC
  * 
  *     return sec, nsec             # <<<<<<<<<<<<<<
  * 
  * def timespec_add(timespec now, time_t sec, long nsec):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_3 = __Pyx_PyInt_From_time_t(__pyx_v_sec); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 96, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_From_time_t(__pyx_v_sec); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 96, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_t_3 = __Pyx_PyInt_From_long(__pyx_v_nsec); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 96, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = __Pyx_PyInt_From_long(__pyx_v_nsec); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 96, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 96, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 96, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_GIVEREF(__pyx_t_4);
+  PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_3);
-  PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_3);
-  __Pyx_GIVEREF(__pyx_t_2);
-  PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_2);
+  PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_t_3);
+  __pyx_t_4 = 0;
   __pyx_t_3 = 0;
+  __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
-  __pyx_r = __pyx_t_1;
-  __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* "atimer/_atimer.pyx":79
  *     return r
  * 
  * def to_timespec(double value):             # <<<<<<<<<<<<<<
  *     """
  *     Convert float number to `timespec` value.
  */
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_4);
   __Pyx_AddTraceback("atimer._atimer.to_timespec", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
@@ -2137,77 +3522,96 @@
  * 
  * def timespec_add(timespec now, time_t sec, long nsec):             # <<<<<<<<<<<<<<
  *     now.tv_sec += sec + (now.tv_nsec + nsec) / NANOSEC
  *     now.tv_nsec = (now.tv_nsec + nsec) % NANOSEC
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_6atimer_7_atimer_9timespec_add(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyMethodDef __pyx_mdef_6atimer_7_atimer_9timespec_add = {"timespec_add", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_6atimer_7_atimer_9timespec_add, METH_VARARGS|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_6atimer_7_atimer_9timespec_add(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_6atimer_7_atimer_9timespec_add(PyObject *__pyx_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+); /*proto*/
+static PyMethodDef __pyx_mdef_6atimer_7_atimer_9timespec_add = {"timespec_add", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_6atimer_7_atimer_9timespec_add, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_6atimer_7_atimer_9timespec_add(PyObject *__pyx_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+) {
   struct timespec __pyx_v_now;
   time_t __pyx_v_sec;
   long __pyx_v_nsec;
+  #if !CYTHON_METH_FASTCALL
+  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #endif
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("timespec_add (wrapper)", 0);
   {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_now,&__pyx_n_s_sec,&__pyx_n_s_nsec,0};
+    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_now,&__pyx_n_s_sec,&__pyx_n_s_nsec,0};
     PyObject* values[3] = {0,0,0};
-    if (unlikely(__pyx_kwds)) {
+    if (__pyx_kwds) {
       Py_ssize_t kw_args;
-      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
-      switch (pos_args) {
-        case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
+      switch (__pyx_nargs) {
+        case  3: values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
-        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+        case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
-        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
-      kw_args = PyDict_Size(__pyx_kwds);
-      switch (pos_args) {
+      kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
+      switch (__pyx_nargs) {
         case  0:
-        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_now)) != 0)) kw_args--;
+        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_now)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 98, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
-        if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_sec)) != 0)) kw_args--;
+        if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_sec)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 98, __pyx_L3_error)
         else {
           __Pyx_RaiseArgtupleInvalid("timespec_add", 1, 3, 3, 1); __PYX_ERR(0, 98, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
-        if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_nsec)) != 0)) kw_args--;
+        if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_nsec)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 98, __pyx_L3_error)
         else {
           __Pyx_RaiseArgtupleInvalid("timespec_add", 1, 3, 3, 2); __PYX_ERR(0, 98, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "timespec_add") < 0)) __PYX_ERR(0, 98, __pyx_L3_error)
+        const Py_ssize_t kwd_pos_args = __pyx_nargs;
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "timespec_add") < 0)) __PYX_ERR(0, 98, __pyx_L3_error)
       }
-    } else if (PyTuple_GET_SIZE(__pyx_args) != 3) {
+    } else if (unlikely(__pyx_nargs != 3)) {
       goto __pyx_L5_argtuple_error;
     } else {
-      values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
-      values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
-      values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
+      values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+      values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
+      values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
     }
     __pyx_v_now = __pyx_convert__from_py_struct__timespec(values[0]); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 98, __pyx_L3_error)
     __pyx_v_sec = __Pyx_PyInt_As_time_t(values[1]); if (unlikely((__pyx_v_sec == ((time_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 98, __pyx_L3_error)
     __pyx_v_nsec = __Pyx_PyInt_As_long(values[2]); if (unlikely((__pyx_v_nsec == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 98, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("timespec_add", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 98, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("timespec_add", 1, 3, 3, __pyx_nargs); __PYX_ERR(0, 98, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("atimer._atimer.timespec_add", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6atimer_7_atimer_8timespec_add(__pyx_self, __pyx_v_now, __pyx_v_sec, __pyx_v_nsec);
 
@@ -2314,490 +3718,192 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "FromPyStructUtility":11
- * 
- * @cname("__pyx_convert__from_py_struct__timespec")
- * cdef struct_type __pyx_convert__from_py_struct__timespec(obj) except *:             # <<<<<<<<<<<<<<
- *     cdef struct_type result
- *     if not PyMapping_Check(obj):
- */
-
-static struct timespec __pyx_convert__from_py_struct__timespec(PyObject *__pyx_v_obj) {
-  struct timespec __pyx_v_result;
-  PyObject *__pyx_v_value = NULL;
-  struct timespec __pyx_r;
-  __Pyx_RefNannyDeclarations
-  int __pyx_t_1;
-  PyObject *__pyx_t_2 = NULL;
-  PyObject *__pyx_t_3 = NULL;
-  PyObject *__pyx_t_4 = NULL;
-  PyObject *__pyx_t_5 = NULL;
-  int __pyx_t_6;
-  PyObject *__pyx_t_7 = NULL;
-  PyObject *__pyx_t_8 = NULL;
-  PyObject *__pyx_t_9 = NULL;
-  time_t __pyx_t_10;
-  long __pyx_t_11;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__pyx_convert__from_py_struct__timespec", 0);
-
-  /* "FromPyStructUtility":13
- * cdef struct_type __pyx_convert__from_py_struct__timespec(obj) except *:
- *     cdef struct_type result
- *     if not PyMapping_Check(obj):             # <<<<<<<<<<<<<<
- *         PyErr_Format(TypeError, b"Expected %.16s, got %.200s", b"a mapping", Py_TYPE(obj).tp_name)
- * 
- */
-  __pyx_t_1 = ((!(PyMapping_Check(__pyx_v_obj) != 0)) != 0);
-  if (__pyx_t_1) {
-
-    /* "FromPyStructUtility":14
- *     cdef struct_type result
- *     if not PyMapping_Check(obj):
- *         PyErr_Format(TypeError, b"Expected %.16s, got %.200s", b"a mapping", Py_TYPE(obj).tp_name)             # <<<<<<<<<<<<<<
- * 
- *     try:
- */
-    __pyx_t_2 = PyErr_Format(__pyx_builtin_TypeError, ((char const *)"Expected %.16s, got %.200s"), ((char *)"a mapping"), Py_TYPE(__pyx_v_obj)->tp_name); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 14, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-
-    /* "FromPyStructUtility":13
- * cdef struct_type __pyx_convert__from_py_struct__timespec(obj) except *:
- *     cdef struct_type result
- *     if not PyMapping_Check(obj):             # <<<<<<<<<<<<<<
- *         PyErr_Format(TypeError, b"Expected %.16s, got %.200s", b"a mapping", Py_TYPE(obj).tp_name)
- * 
- */
-  }
-
-  /* "FromPyStructUtility":16
- *         PyErr_Format(TypeError, b"Expected %.16s, got %.200s", b"a mapping", Py_TYPE(obj).tp_name)
- * 
- *     try:             # <<<<<<<<<<<<<<
- *         value = obj['tv_sec']
- *     except KeyError:
- */
-  {
-    __Pyx_PyThreadState_declare
-    __Pyx_PyThreadState_assign
-    __Pyx_ExceptionSave(&__pyx_t_3, &__pyx_t_4, &__pyx_t_5);
-    __Pyx_XGOTREF(__pyx_t_3);
-    __Pyx_XGOTREF(__pyx_t_4);
-    __Pyx_XGOTREF(__pyx_t_5);
-    /*try:*/ {
-
-      /* "FromPyStructUtility":17
- * 
- *     try:
- *         value = obj['tv_sec']             # <<<<<<<<<<<<<<
- *     except KeyError:
- *         raise ValueError("No value specified for struct attribute 'tv_sec'")
- */
-      __pyx_t_2 = __Pyx_PyObject_Dict_GetItem(__pyx_v_obj, __pyx_n_s_tv_sec); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 17, __pyx_L4_error)
-      __Pyx_GOTREF(__pyx_t_2);
-      __pyx_v_value = __pyx_t_2;
-      __pyx_t_2 = 0;
-
-      /* "FromPyStructUtility":16
- *         PyErr_Format(TypeError, b"Expected %.16s, got %.200s", b"a mapping", Py_TYPE(obj).tp_name)
- * 
- *     try:             # <<<<<<<<<<<<<<
- *         value = obj['tv_sec']
- *     except KeyError:
- */
-    }
-    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-    goto __pyx_L9_try_end;
-    __pyx_L4_error:;
-    __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-
-    /* "FromPyStructUtility":18
- *     try:
- *         value = obj['tv_sec']
- *     except KeyError:             # <<<<<<<<<<<<<<
- *         raise ValueError("No value specified for struct attribute 'tv_sec'")
- *     result.tv_sec = value
- */
-    __pyx_t_6 = __Pyx_PyErr_ExceptionMatches(__pyx_builtin_KeyError);
-    if (__pyx_t_6) {
-      __Pyx_AddTraceback("FromPyStructUtility.__pyx_convert__from_py_struct__timespec", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_2, &__pyx_t_7, &__pyx_t_8) < 0) __PYX_ERR(1, 18, __pyx_L6_except_error)
-      __Pyx_GOTREF(__pyx_t_2);
-      __Pyx_GOTREF(__pyx_t_7);
-      __Pyx_GOTREF(__pyx_t_8);
-
-      /* "FromPyStructUtility":19
- *         value = obj['tv_sec']
- *     except KeyError:
- *         raise ValueError("No value specified for struct attribute 'tv_sec'")             # <<<<<<<<<<<<<<
- *     result.tv_sec = value
- *     try:
- */
-      __pyx_t_9 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 19, __pyx_L6_except_error)
-      __Pyx_GOTREF(__pyx_t_9);
-      __Pyx_Raise(__pyx_t_9, 0, 0, 0);
-      __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-      __PYX_ERR(1, 19, __pyx_L6_except_error)
-    }
-    goto __pyx_L6_except_error;
-    __pyx_L6_except_error:;
-
-    /* "FromPyStructUtility":16
- *         PyErr_Format(TypeError, b"Expected %.16s, got %.200s", b"a mapping", Py_TYPE(obj).tp_name)
- * 
- *     try:             # <<<<<<<<<<<<<<
- *         value = obj['tv_sec']
- *     except KeyError:
- */
-    __Pyx_XGIVEREF(__pyx_t_3);
-    __Pyx_XGIVEREF(__pyx_t_4);
-    __Pyx_XGIVEREF(__pyx_t_5);
-    __Pyx_ExceptionReset(__pyx_t_3, __pyx_t_4, __pyx_t_5);
-    goto __pyx_L1_error;
-    __pyx_L9_try_end:;
-  }
-
-  /* "FromPyStructUtility":20
- *     except KeyError:
- *         raise ValueError("No value specified for struct attribute 'tv_sec'")
- *     result.tv_sec = value             # <<<<<<<<<<<<<<
- *     try:
- *         value = obj['tv_nsec']
- */
-  __pyx_t_10 = __Pyx_PyInt_As_time_t(__pyx_v_value); if (unlikely((__pyx_t_10 == ((time_t)-1)) && PyErr_Occurred())) __PYX_ERR(1, 20, __pyx_L1_error)
-  __pyx_v_result.tv_sec = __pyx_t_10;
-
-  /* "FromPyStructUtility":21
- *         raise ValueError("No value specified for struct attribute 'tv_sec'")
- *     result.tv_sec = value
- *     try:             # <<<<<<<<<<<<<<
- *         value = obj['tv_nsec']
- *     except KeyError:
- */
-  {
-    __Pyx_PyThreadState_declare
-    __Pyx_PyThreadState_assign
-    __Pyx_ExceptionSave(&__pyx_t_5, &__pyx_t_4, &__pyx_t_3);
-    __Pyx_XGOTREF(__pyx_t_5);
-    __Pyx_XGOTREF(__pyx_t_4);
-    __Pyx_XGOTREF(__pyx_t_3);
-    /*try:*/ {
-
-      /* "FromPyStructUtility":22
- *     result.tv_sec = value
- *     try:
- *         value = obj['tv_nsec']             # <<<<<<<<<<<<<<
- *     except KeyError:
- *         raise ValueError("No value specified for struct attribute 'tv_nsec'")
- */
-      __pyx_t_8 = __Pyx_PyObject_Dict_GetItem(__pyx_v_obj, __pyx_n_s_tv_nsec); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 22, __pyx_L12_error)
-      __Pyx_GOTREF(__pyx_t_8);
-      __Pyx_DECREF_SET(__pyx_v_value, __pyx_t_8);
-      __pyx_t_8 = 0;
-
-      /* "FromPyStructUtility":21
- *         raise ValueError("No value specified for struct attribute 'tv_sec'")
- *     result.tv_sec = value
- *     try:             # <<<<<<<<<<<<<<
- *         value = obj['tv_nsec']
- *     except KeyError:
- */
-    }
-    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    goto __pyx_L17_try_end;
-    __pyx_L12_error:;
-    __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-    __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
-    __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
-
-    /* "FromPyStructUtility":23
- *     try:
- *         value = obj['tv_nsec']
- *     except KeyError:             # <<<<<<<<<<<<<<
- *         raise ValueError("No value specified for struct attribute 'tv_nsec'")
- *     result.tv_nsec = value
- */
-    __pyx_t_6 = __Pyx_PyErr_ExceptionMatches(__pyx_builtin_KeyError);
-    if (__pyx_t_6) {
-      __Pyx_AddTraceback("FromPyStructUtility.__pyx_convert__from_py_struct__timespec", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_8, &__pyx_t_7, &__pyx_t_2) < 0) __PYX_ERR(1, 23, __pyx_L14_except_error)
-      __Pyx_GOTREF(__pyx_t_8);
-      __Pyx_GOTREF(__pyx_t_7);
-      __Pyx_GOTREF(__pyx_t_2);
-
-      /* "FromPyStructUtility":24
- *         value = obj['tv_nsec']
- *     except KeyError:
- *         raise ValueError("No value specified for struct attribute 'tv_nsec'")             # <<<<<<<<<<<<<<
- *     result.tv_nsec = value
- *     return result
- */
-      __pyx_t_9 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 24, __pyx_L14_except_error)
-      __Pyx_GOTREF(__pyx_t_9);
-      __Pyx_Raise(__pyx_t_9, 0, 0, 0);
-      __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-      __PYX_ERR(1, 24, __pyx_L14_except_error)
-    }
-    goto __pyx_L14_except_error;
-    __pyx_L14_except_error:;
-
-    /* "FromPyStructUtility":21
- *         raise ValueError("No value specified for struct attribute 'tv_sec'")
- *     result.tv_sec = value
- *     try:             # <<<<<<<<<<<<<<
- *         value = obj['tv_nsec']
- *     except KeyError:
- */
-    __Pyx_XGIVEREF(__pyx_t_5);
-    __Pyx_XGIVEREF(__pyx_t_4);
-    __Pyx_XGIVEREF(__pyx_t_3);
-    __Pyx_ExceptionReset(__pyx_t_5, __pyx_t_4, __pyx_t_3);
-    goto __pyx_L1_error;
-    __pyx_L17_try_end:;
-  }
-
-  /* "FromPyStructUtility":25
- *     except KeyError:
- *         raise ValueError("No value specified for struct attribute 'tv_nsec'")
- *     result.tv_nsec = value             # <<<<<<<<<<<<<<
- *     return result
- * 
- */
-  __pyx_t_11 = __Pyx_PyInt_As_long(__pyx_v_value); if (unlikely((__pyx_t_11 == (long)-1) && PyErr_Occurred())) __PYX_ERR(1, 25, __pyx_L1_error)
-  __pyx_v_result.tv_nsec = __pyx_t_11;
-
-  /* "FromPyStructUtility":26
- *         raise ValueError("No value specified for struct attribute 'tv_nsec'")
- *     result.tv_nsec = value
- *     return result             # <<<<<<<<<<<<<<
- * 
- * 
- */
-  __pyx_r = __pyx_v_result;
-  goto __pyx_L0;
-
-  /* "FromPyStructUtility":11
- * 
- * @cname("__pyx_convert__from_py_struct__timespec")
- * cdef struct_type __pyx_convert__from_py_struct__timespec(obj) except *:             # <<<<<<<<<<<<<<
- *     cdef struct_type result
- *     if not PyMapping_Check(obj):
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_7);
-  __Pyx_XDECREF(__pyx_t_8);
-  __Pyx_XDECREF(__pyx_t_9);
-  __Pyx_AddTraceback("FromPyStructUtility.__pyx_convert__from_py_struct__timespec", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_pretend_to_initialize(&__pyx_r);
-  __pyx_L0:;
-  __Pyx_XDECREF(__pyx_v_value);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
 static PyMethodDef __pyx_methods[] = {
   {0, 0, 0, 0}
 };
-
-#if PY_MAJOR_VERSION >= 3
-#if CYTHON_PEP489_MULTI_PHASE_INIT
-static PyObject* __pyx_pymod_create(PyObject *spec, PyModuleDef *def); /*proto*/
-static int __pyx_pymod_exec__atimer(PyObject* module); /*proto*/
-static PyModuleDef_Slot __pyx_moduledef_slots[] = {
-  {Py_mod_create, (void*)__pyx_pymod_create},
-  {Py_mod_exec, (void*)__pyx_pymod_exec__atimer},
-  {0, NULL}
-};
-#endif
-
-static struct PyModuleDef __pyx_moduledef = {
-    PyModuleDef_HEAD_INIT,
-    "_atimer",
-    0, /* m_doc */
-  #if CYTHON_PEP489_MULTI_PHASE_INIT
-    0, /* m_size */
-  #else
-    -1, /* m_size */
-  #endif
-    __pyx_methods /* m_methods */,
-  #if CYTHON_PEP489_MULTI_PHASE_INIT
-    __pyx_moduledef_slots, /* m_slots */
-  #else
-    NULL, /* m_reload */
-  #endif
-    NULL, /* m_traverse */
-    NULL, /* m_clear */
-    NULL /* m_free */
-};
-#endif
 #ifndef CYTHON_SMALL_CODE
 #if defined(__clang__)
     #define CYTHON_SMALL_CODE
 #elif defined(__GNUC__) && (__GNUC__ > 4 || (__GNUC__ == 4 && __GNUC_MINOR__ >= 3))
     #define CYTHON_SMALL_CODE __attribute__((cold))
 #else
     #define CYTHON_SMALL_CODE
 #endif
 #endif
+/* #### Code section: pystring_table ### */
 
-static __Pyx_StringTabEntry __pyx_string_tab[] = {
-  {&__pyx_n_s_KeyError, __pyx_k_KeyError, sizeof(__pyx_k_KeyError), 0, 0, 1, 1},
-  {&__pyx_n_s_NANOSEC, __pyx_k_NANOSEC, sizeof(__pyx_k_NANOSEC), 0, 0, 1, 1},
-  {&__pyx_kp_s_No_value_specified_for_struct_at, __pyx_k_No_value_specified_for_struct_at, sizeof(__pyx_k_No_value_specified_for_struct_at), 0, 0, 1, 0},
-  {&__pyx_kp_s_No_value_specified_for_struct_at_2, __pyx_k_No_value_specified_for_struct_at_2, sizeof(__pyx_k_No_value_specified_for_struct_at_2), 0, 0, 1, 0},
-  {&__pyx_n_s_TypeError, __pyx_k_TypeError, sizeof(__pyx_k_TypeError), 0, 0, 1, 1},
-  {&__pyx_n_s_ValueError, __pyx_k_ValueError, sizeof(__pyx_k_ValueError), 0, 0, 1, 1},
-  {&__pyx_n_s_atimer__atimer, __pyx_k_atimer__atimer, sizeof(__pyx_k_atimer__atimer), 0, 0, 1, 1},
-  {&__pyx_kp_s_atimer__atimer_pyx, __pyx_k_atimer__atimer_pyx, sizeof(__pyx_k_atimer__atimer_pyx), 0, 0, 1, 0},
-  {&__pyx_n_s_atimer_close, __pyx_k_atimer_close, sizeof(__pyx_k_atimer_close), 0, 0, 1, 1},
-  {&__pyx_n_s_atimer_init, __pyx_k_atimer_init, sizeof(__pyx_k_atimer_init), 0, 0, 1, 1},
-  {&__pyx_n_s_atimer_start, __pyx_k_atimer_start, sizeof(__pyx_k_atimer_start), 0, 0, 1, 1},
-  {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
-  {&__pyx_n_s_d_nsec, __pyx_k_d_nsec, sizeof(__pyx_k_d_nsec), 0, 0, 1, 1},
-  {&__pyx_n_s_d_sec, __pyx_k_d_sec, sizeof(__pyx_k_d_sec), 0, 0, 1, 1},
-  {&__pyx_n_s_fd, __pyx_k_fd, sizeof(__pyx_k_fd), 0, 0, 1, 1},
-  {&__pyx_n_s_import, __pyx_k_import, sizeof(__pyx_k_import), 0, 0, 1, 1},
-  {&__pyx_n_s_interval, __pyx_k_interval, sizeof(__pyx_k_interval), 0, 0, 1, 1},
-  {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
-  {&__pyx_n_s_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
-  {&__pyx_n_s_now, __pyx_k_now, sizeof(__pyx_k_now), 0, 0, 1, 1},
-  {&__pyx_n_s_nsec, __pyx_k_nsec, sizeof(__pyx_k_nsec), 0, 0, 1, 1},
-  {&__pyx_n_s_r, __pyx_k_r, sizeof(__pyx_k_r), 0, 0, 1, 1},
-  {&__pyx_n_s_sec, __pyx_k_sec, sizeof(__pyx_k_sec), 0, 0, 1, 1},
-  {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
-  {&__pyx_n_s_time, __pyx_k_time, sizeof(__pyx_k_time), 0, 0, 1, 1},
-  {&__pyx_n_s_timespec_add, __pyx_k_timespec_add, sizeof(__pyx_k_timespec_add), 0, 0, 1, 1},
-  {&__pyx_n_s_to_timespec, __pyx_k_to_timespec, sizeof(__pyx_k_to_timespec), 0, 0, 1, 1},
-  {&__pyx_n_s_ts, __pyx_k_ts, sizeof(__pyx_k_ts), 0, 0, 1, 1},
-  {&__pyx_n_s_tv_nsec, __pyx_k_tv_nsec, sizeof(__pyx_k_tv_nsec), 0, 0, 1, 1},
-  {&__pyx_n_s_tv_sec, __pyx_k_tv_sec, sizeof(__pyx_k_tv_sec), 0, 0, 1, 1},
-  {&__pyx_n_s_value, __pyx_k_value, sizeof(__pyx_k_value), 0, 0, 1, 1},
-  {0, 0, 0, 0, 0, 0, 0}
-};
+static int __Pyx_CreateStringTabAndInitStrings(void) {
+  __Pyx_StringTabEntry __pyx_string_tab[] = {
+    {&__pyx_n_s_AssertionError, __pyx_k_AssertionError, sizeof(__pyx_k_AssertionError), 0, 0, 1, 1},
+    {&__pyx_n_s_KeyError, __pyx_k_KeyError, sizeof(__pyx_k_KeyError), 0, 0, 1, 1},
+    {&__pyx_n_s_NANOSEC, __pyx_k_NANOSEC, sizeof(__pyx_k_NANOSEC), 0, 0, 1, 1},
+    {&__pyx_kp_s_No_value_specified_for_struct_at, __pyx_k_No_value_specified_for_struct_at, sizeof(__pyx_k_No_value_specified_for_struct_at), 0, 0, 1, 0},
+    {&__pyx_kp_s_No_value_specified_for_struct_at_2, __pyx_k_No_value_specified_for_struct_at_2, sizeof(__pyx_k_No_value_specified_for_struct_at_2), 0, 0, 1, 0},
+    {&__pyx_n_s_ValueError, __pyx_k_ValueError, sizeof(__pyx_k_ValueError), 0, 0, 1, 1},
+    {&__pyx_n_s__13, __pyx_k__13, sizeof(__pyx_k__13), 0, 0, 1, 1},
+    {&__pyx_n_s__3, __pyx_k__3, sizeof(__pyx_k__3), 0, 0, 1, 1},
+    {&__pyx_n_s_asyncio_coroutines, __pyx_k_asyncio_coroutines, sizeof(__pyx_k_asyncio_coroutines), 0, 0, 1, 1},
+    {&__pyx_n_s_atimer__atimer, __pyx_k_atimer__atimer, sizeof(__pyx_k_atimer__atimer), 0, 0, 1, 1},
+    {&__pyx_kp_s_atimer__atimer_pyx, __pyx_k_atimer__atimer_pyx, sizeof(__pyx_k_atimer__atimer_pyx), 0, 0, 1, 0},
+    {&__pyx_n_s_atimer_close, __pyx_k_atimer_close, sizeof(__pyx_k_atimer_close), 0, 0, 1, 1},
+    {&__pyx_n_s_atimer_init, __pyx_k_atimer_init, sizeof(__pyx_k_atimer_init), 0, 0, 1, 1},
+    {&__pyx_n_s_atimer_start, __pyx_k_atimer_start, sizeof(__pyx_k_atimer_start), 0, 0, 1, 1},
+    {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
+    {&__pyx_n_s_d_nsec, __pyx_k_d_nsec, sizeof(__pyx_k_d_nsec), 0, 0, 1, 1},
+    {&__pyx_n_s_d_sec, __pyx_k_d_sec, sizeof(__pyx_k_d_sec), 0, 0, 1, 1},
+    {&__pyx_n_s_fd, __pyx_k_fd, sizeof(__pyx_k_fd), 0, 0, 1, 1},
+    {&__pyx_n_s_import, __pyx_k_import, sizeof(__pyx_k_import), 0, 0, 1, 1},
+    {&__pyx_n_s_initializing, __pyx_k_initializing, sizeof(__pyx_k_initializing), 0, 0, 1, 1},
+    {&__pyx_n_s_interval, __pyx_k_interval, sizeof(__pyx_k_interval), 0, 0, 1, 1},
+    {&__pyx_n_s_is_coroutine, __pyx_k_is_coroutine, sizeof(__pyx_k_is_coroutine), 0, 0, 1, 1},
+    {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
+    {&__pyx_n_s_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
+    {&__pyx_n_s_now, __pyx_k_now, sizeof(__pyx_k_now), 0, 0, 1, 1},
+    {&__pyx_n_s_nsec, __pyx_k_nsec, sizeof(__pyx_k_nsec), 0, 0, 1, 1},
+    {&__pyx_n_s_r, __pyx_k_r, sizeof(__pyx_k_r), 0, 0, 1, 1},
+    {&__pyx_n_s_sec, __pyx_k_sec, sizeof(__pyx_k_sec), 0, 0, 1, 1},
+    {&__pyx_n_s_spec, __pyx_k_spec, sizeof(__pyx_k_spec), 0, 0, 1, 1},
+    {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
+    {&__pyx_n_s_time, __pyx_k_time, sizeof(__pyx_k_time), 0, 0, 1, 1},
+    {&__pyx_n_s_timespec_add, __pyx_k_timespec_add, sizeof(__pyx_k_timespec_add), 0, 0, 1, 1},
+    {&__pyx_n_s_to_timespec, __pyx_k_to_timespec, sizeof(__pyx_k_to_timespec), 0, 0, 1, 1},
+    {&__pyx_n_s_ts, __pyx_k_ts, sizeof(__pyx_k_ts), 0, 0, 1, 1},
+    {&__pyx_n_s_tv_nsec, __pyx_k_tv_nsec, sizeof(__pyx_k_tv_nsec), 0, 0, 1, 1},
+    {&__pyx_n_s_tv_sec, __pyx_k_tv_sec, sizeof(__pyx_k_tv_sec), 0, 0, 1, 1},
+    {&__pyx_n_s_value, __pyx_k_value, sizeof(__pyx_k_value), 0, 0, 1, 1},
+    {0, 0, 0, 0, 0, 0, 0}
+  };
+  return __Pyx_InitStrings(__pyx_string_tab);
+}
+/* #### Code section: cached_builtins ### */
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
-  __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(1, 14, __pyx_L1_error)
-  __pyx_builtin_KeyError = __Pyx_GetBuiltinName(__pyx_n_s_KeyError); if (!__pyx_builtin_KeyError) __PYX_ERR(1, 18, __pyx_L1_error)
-  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(1, 19, __pyx_L1_error)
+  __pyx_builtin_AssertionError = __Pyx_GetBuiltinName(__pyx_n_s_AssertionError); if (!__pyx_builtin_AssertionError) __PYX_ERR(0, 93, __pyx_L1_error)
+  __pyx_builtin_KeyError = __Pyx_GetBuiltinName(__pyx_n_s_KeyError); if (!__pyx_builtin_KeyError) __PYX_ERR(1, 19, __pyx_L1_error)
+  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(1, 20, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
+/* #### Code section: cached_constants ### */
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "FromPyStructUtility":19
+  /* "FromPyStructUtility":20
  *         value = obj['tv_sec']
  *     except KeyError:
  *         raise ValueError("No value specified for struct attribute 'tv_sec'")             # <<<<<<<<<<<<<<
  *     result.tv_sec = value
  *     try:
  */
-  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_s_No_value_specified_for_struct_at); if (unlikely(!__pyx_tuple_)) __PYX_ERR(1, 19, __pyx_L1_error)
+  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_s_No_value_specified_for_struct_at); if (unlikely(!__pyx_tuple_)) __PYX_ERR(1, 20, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
 
-  /* "FromPyStructUtility":24
+  /* "FromPyStructUtility":25
  *         value = obj['tv_nsec']
  *     except KeyError:
  *         raise ValueError("No value specified for struct attribute 'tv_nsec'")             # <<<<<<<<<<<<<<
  *     result.tv_nsec = value
  *     return result
  */
-  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_s_No_value_specified_for_struct_at_2); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 24, __pyx_L1_error)
+  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_s_No_value_specified_for_struct_at_2); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 25, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__2);
   __Pyx_GIVEREF(__pyx_tuple__2);
 
   /* "atimer/_atimer.pyx":39
  *     int timerfd_gettime(int, itimerspec*)
  * 
  * def atimer_init():             # <<<<<<<<<<<<<<
  *     # CLOCK_BOOTIME: count number of expirations when running machine is
  *     # suspended
  */
-  __pyx_codeobj__3 = (PyObject*)__Pyx_PyCode_New(0, 0, 0, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_atimer__atimer_pyx, __pyx_n_s_atimer_init, 39, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__3)) __PYX_ERR(0, 39, __pyx_L1_error)
+  __pyx_codeobj__4 = (PyObject*)__Pyx_PyCode_New(0, 0, 0, 0, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_atimer__atimer_pyx, __pyx_n_s_atimer_init, 39, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__4)) __PYX_ERR(0, 39, __pyx_L1_error)
 
   /* "atimer/_atimer.pyx":46
  *     return timerfd_create(CLOCK_BOOTTIME, TFD_NONBLOCK)
  * 
  * def atimer_start(int fd, double interval):             # <<<<<<<<<<<<<<
  *     cdef itimerspec ts
  *     cdef timespec now
  */
-  __pyx_tuple__4 = PyTuple_Pack(8, __pyx_n_s_fd, __pyx_n_s_interval, __pyx_n_s_ts, __pyx_n_s_now, __pyx_n_s_sec, __pyx_n_s_d_sec, __pyx_n_s_nsec, __pyx_n_s_d_nsec); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(0, 46, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__4);
-  __Pyx_GIVEREF(__pyx_tuple__4);
-  __pyx_codeobj__5 = (PyObject*)__Pyx_PyCode_New(2, 0, 8, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__4, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_atimer__atimer_pyx, __pyx_n_s_atimer_start, 46, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__5)) __PYX_ERR(0, 46, __pyx_L1_error)
+  __pyx_tuple__5 = PyTuple_Pack(8, __pyx_n_s_fd, __pyx_n_s_interval, __pyx_n_s_ts, __pyx_n_s_now, __pyx_n_s_sec, __pyx_n_s_d_sec, __pyx_n_s_nsec, __pyx_n_s_d_nsec); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(0, 46, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__5);
+  __Pyx_GIVEREF(__pyx_tuple__5);
+  __pyx_codeobj__6 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 8, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__5, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_atimer__atimer_pyx, __pyx_n_s_atimer_start, 46, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__6)) __PYX_ERR(0, 46, __pyx_L1_error)
 
   /* "atimer/_atimer.pyx":65
  *     return timerfd_settime(fd, TFD_TIMER_ABSTIME, &ts, NULL)
  * 
  * def atimer_close(int fd):             # <<<<<<<<<<<<<<
  *     cdef int r
  *     cdef itimerspec ts
  */
-  __pyx_tuple__6 = PyTuple_Pack(4, __pyx_n_s_fd, __pyx_n_s_fd, __pyx_n_s_r, __pyx_n_s_ts); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(0, 65, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__6);
-  __Pyx_GIVEREF(__pyx_tuple__6);
-  __pyx_codeobj__7 = (PyObject*)__Pyx_PyCode_New(1, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__6, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_atimer__atimer_pyx, __pyx_n_s_atimer_close, 65, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__7)) __PYX_ERR(0, 65, __pyx_L1_error)
+  __pyx_tuple__7 = PyTuple_Pack(3, __pyx_n_s_fd, __pyx_n_s_r, __pyx_n_s_ts); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(0, 65, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__7);
+  __Pyx_GIVEREF(__pyx_tuple__7);
+  __pyx_codeobj__8 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__7, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_atimer__atimer_pyx, __pyx_n_s_atimer_close, 65, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__8)) __PYX_ERR(0, 65, __pyx_L1_error)
 
   /* "atimer/_atimer.pyx":79
  *     return r
  * 
  * def to_timespec(double value):             # <<<<<<<<<<<<<<
  *     """
  *     Convert float number to `timespec` value.
  */
-  __pyx_tuple__8 = PyTuple_Pack(4, __pyx_n_s_value, __pyx_n_s_value, __pyx_n_s_sec, __pyx_n_s_nsec); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(0, 79, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__8);
-  __Pyx_GIVEREF(__pyx_tuple__8);
-  __pyx_codeobj__9 = (PyObject*)__Pyx_PyCode_New(1, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__8, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_atimer__atimer_pyx, __pyx_n_s_to_timespec, 79, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__9)) __PYX_ERR(0, 79, __pyx_L1_error)
+  __pyx_tuple__9 = PyTuple_Pack(3, __pyx_n_s_value, __pyx_n_s_sec, __pyx_n_s_nsec); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(0, 79, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__9);
+  __Pyx_GIVEREF(__pyx_tuple__9);
+  __pyx_codeobj__10 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__9, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_atimer__atimer_pyx, __pyx_n_s_to_timespec, 79, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__10)) __PYX_ERR(0, 79, __pyx_L1_error)
 
   /* "atimer/_atimer.pyx":98
  *     return sec, nsec
  * 
  * def timespec_add(timespec now, time_t sec, long nsec):             # <<<<<<<<<<<<<<
  *     now.tv_sec += sec + (now.tv_nsec + nsec) / NANOSEC
  *     now.tv_nsec = (now.tv_nsec + nsec) % NANOSEC
  */
-  __pyx_tuple__10 = PyTuple_Pack(3, __pyx_n_s_now, __pyx_n_s_sec, __pyx_n_s_nsec); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(0, 98, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__10);
-  __Pyx_GIVEREF(__pyx_tuple__10);
-  __pyx_codeobj__11 = (PyObject*)__Pyx_PyCode_New(3, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__10, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_atimer__atimer_pyx, __pyx_n_s_timespec_add, 98, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__11)) __PYX_ERR(0, 98, __pyx_L1_error)
+  __pyx_tuple__11 = PyTuple_Pack(3, __pyx_n_s_now, __pyx_n_s_sec, __pyx_n_s_nsec); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(0, 98, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__11);
+  __Pyx_GIVEREF(__pyx_tuple__11);
+  __pyx_codeobj__12 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__11, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_atimer__atimer_pyx, __pyx_n_s_timespec_add, 98, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__12)) __PYX_ERR(0, 98, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
+/* #### Code section: init_constants ### */
 
-static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
-  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+static CYTHON_SMALL_CODE int __Pyx_InitConstants(void) {
+  if (__Pyx_CreateStringTabAndInitStrings() < 0) __PYX_ERR(0, 1, __pyx_L1_error);
   __pyx_float_1e9 = PyFloat_FromDouble(1e9); if (unlikely(!__pyx_float_1e9)) __PYX_ERR(0, 1, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
+/* #### Code section: init_globals ### */
+
+static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
+  /* AssertionsEnabled.init */
+  __Pyx_init_assertions_enabled();
+
+if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1, __pyx_L1_error)
+
+  return 0;
+  __pyx_L1_error:;
+  return -1;
+}
+/* #### Code section: init_module ### */
 
 static CYTHON_SMALL_CODE int __Pyx_modinit_global_init_code(void); /*proto*/
 static CYTHON_SMALL_CODE int __Pyx_modinit_variable_export_code(void); /*proto*/
 static CYTHON_SMALL_CODE int __Pyx_modinit_function_export_code(void); /*proto*/
 static CYTHON_SMALL_CODE int __Pyx_modinit_type_init_code(void); /*proto*/
 static CYTHON_SMALL_CODE int __Pyx_modinit_type_import_code(void); /*proto*/
 static CYTHON_SMALL_CODE int __Pyx_modinit_variable_import_code(void); /*proto*/
@@ -2856,14 +3962,63 @@
   __Pyx_RefNannySetupContext("__Pyx_modinit_function_import_code", 0);
   /*--- Function import code ---*/
   __Pyx_RefNannyFinishContext();
   return 0;
 }
 
 
+#if PY_MAJOR_VERSION >= 3
+#if CYTHON_PEP489_MULTI_PHASE_INIT
+static PyObject* __pyx_pymod_create(PyObject *spec, PyModuleDef *def); /*proto*/
+static int __pyx_pymod_exec__atimer(PyObject* module); /*proto*/
+static PyModuleDef_Slot __pyx_moduledef_slots[] = {
+  {Py_mod_create, (void*)__pyx_pymod_create},
+  {Py_mod_exec, (void*)__pyx_pymod_exec__atimer},
+  {0, NULL}
+};
+#endif
+
+#ifdef __cplusplus
+namespace {
+  struct PyModuleDef __pyx_moduledef =
+  #else
+  static struct PyModuleDef __pyx_moduledef =
+  #endif
+  {
+      PyModuleDef_HEAD_INIT,
+      "_atimer",
+      0, /* m_doc */
+    #if CYTHON_PEP489_MULTI_PHASE_INIT
+      0, /* m_size */
+    #elif CYTHON_USE_MODULE_STATE
+      sizeof(__pyx_mstate), /* m_size */
+    #else
+      -1, /* m_size */
+    #endif
+      __pyx_methods /* m_methods */,
+    #if CYTHON_PEP489_MULTI_PHASE_INIT
+      __pyx_moduledef_slots, /* m_slots */
+    #else
+      NULL, /* m_reload */
+    #endif
+    #if CYTHON_USE_MODULE_STATE
+      __pyx_m_traverse, /* m_traverse */
+      __pyx_m_clear, /* m_clear */
+      NULL /* m_free */
+    #else
+      NULL, /* m_traverse */
+      NULL, /* m_clear */
+      NULL /* m_free */
+    #endif
+  };
+  #ifdef __cplusplus
+} /* anonymous namespace */
+#endif
+#endif
+
 #ifndef CYTHON_NO_PYINIT_EXPORT
 #define __Pyx_PyMODINIT_FUNC PyMODINIT_FUNC
 #elif PY_MAJOR_VERSION < 3
 #ifdef __cplusplus
 #define __Pyx_PyMODINIT_FUNC extern "C" void
 #else
 #define __Pyx_PyMODINIT_FUNC void
@@ -2906,42 +4061,56 @@
         PyErr_SetString(
             PyExc_ImportError,
             "Interpreter change detected - this module can only be loaded into one interpreter per process.");
         return -1;
     }
     return 0;
 }
-static CYTHON_SMALL_CODE int __Pyx_copy_spec_to_module(PyObject *spec, PyObject *moddict, const char* from_name, const char* to_name, int allow_none) {
+#if CYTHON_COMPILING_IN_LIMITED_API
+static CYTHON_SMALL_CODE int __Pyx_copy_spec_to_module(PyObject *spec, PyObject *module, const char* from_name, const char* to_name, int allow_none)
+#else
+static CYTHON_SMALL_CODE int __Pyx_copy_spec_to_module(PyObject *spec, PyObject *moddict, const char* from_name, const char* to_name, int allow_none)
+#endif
+{
     PyObject *value = PyObject_GetAttrString(spec, from_name);
     int result = 0;
     if (likely(value)) {
         if (allow_none || value != Py_None) {
+#if CYTHON_COMPILING_IN_LIMITED_API
+            result = PyModule_AddObject(module, to_name, value);
+#else
             result = PyDict_SetItemString(moddict, to_name, value);
+#endif
         }
         Py_DECREF(value);
     } else if (PyErr_ExceptionMatches(PyExc_AttributeError)) {
         PyErr_Clear();
     } else {
         result = -1;
     }
     return result;
 }
-static CYTHON_SMALL_CODE PyObject* __pyx_pymod_create(PyObject *spec, CYTHON_UNUSED PyModuleDef *def) {
+static CYTHON_SMALL_CODE PyObject* __pyx_pymod_create(PyObject *spec, PyModuleDef *def) {
     PyObject *module = NULL, *moddict, *modname;
+    CYTHON_UNUSED_VAR(def);
     if (__Pyx_check_single_interpreter())
         return NULL;
     if (__pyx_m)
         return __Pyx_NewRef(__pyx_m);
     modname = PyObject_GetAttrString(spec, "name");
     if (unlikely(!modname)) goto bad;
     module = PyModule_NewObject(modname);
     Py_DECREF(modname);
     if (unlikely(!module)) goto bad;
+#if CYTHON_COMPILING_IN_LIMITED_API
+    moddict = module;
+#else
     moddict = PyModule_GetDict(module);
     if (unlikely(!moddict)) goto bad;
+#endif
     if (unlikely(__Pyx_copy_spec_to_module(spec, moddict, "loader", "__loader__", 1) < 0)) goto bad;
     if (unlikely(__Pyx_copy_spec_to_module(spec, moddict, "origin", "__file__", 1) < 0)) goto bad;
     if (unlikely(__Pyx_copy_spec_to_module(spec, moddict, "parent", "__package__", 1) < 0)) goto bad;
     if (unlikely(__Pyx_copy_spec_to_module(spec, moddict, "submodule_search_locations", "__path__", 0) < 0)) goto bad;
     return module;
 bad:
     Py_XDECREF(module);
@@ -2949,28 +4118,62 @@
 }
 
 
 static CYTHON_SMALL_CODE int __pyx_pymod_exec__atimer(PyObject *__pyx_pyinit_module)
 #endif
 #endif
 {
+  int stringtab_initialized = 0;
+  #if CYTHON_USE_MODULE_STATE
+  int pystate_addmodule_run = 0;
+  #endif
   PyObject *__pyx_t_1 = NULL;
+  PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannyDeclarations
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   if (__pyx_m) {
     if (__pyx_m == __pyx_pyinit_module) return 0;
     PyErr_SetString(PyExc_RuntimeError, "Module '_atimer' has already been imported. Re-initialisation is not supported.");
     return -1;
   }
   #elif PY_MAJOR_VERSION >= 3
   if (__pyx_m) return __Pyx_NewRef(__pyx_m);
   #endif
+  /*--- Module creation code ---*/
+  #if CYTHON_PEP489_MULTI_PHASE_INIT
+  __pyx_m = __pyx_pyinit_module;
+  Py_INCREF(__pyx_m);
+  #else
+  #if PY_MAJOR_VERSION < 3
+  __pyx_m = Py_InitModule4("_atimer", __pyx_methods, 0, 0, PYTHON_API_VERSION); Py_XINCREF(__pyx_m);
+  if (unlikely(!__pyx_m)) __PYX_ERR(0, 1, __pyx_L1_error)
+  #elif CYTHON_USE_MODULE_STATE
+  __pyx_t_1 = PyModule_Create(&__pyx_moduledef); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
+  {
+    int add_module_result = PyState_AddModule(__pyx_t_1, &__pyx_moduledef);
+    __pyx_t_1 = 0; /* transfer ownership from __pyx_t_1 to _atimer pseudovariable */
+    if (unlikely((add_module_result < 0))) __PYX_ERR(0, 1, __pyx_L1_error)
+    pystate_addmodule_run = 1;
+  }
+  #else
+  __pyx_m = PyModule_Create(&__pyx_moduledef);
+  if (unlikely(!__pyx_m)) __PYX_ERR(0, 1, __pyx_L1_error)
+  #endif
+  #endif
+  CYTHON_UNUSED_VAR(__pyx_t_1);
+  __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(0, 1, __pyx_L1_error)
+  Py_INCREF(__pyx_d);
+  __pyx_b = PyImport_AddModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(0, 1, __pyx_L1_error)
+  Py_INCREF(__pyx_b);
+  __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(0, 1, __pyx_L1_error)
+  Py_INCREF(__pyx_cython_runtime);
+  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #if CYTHON_REFNANNY
 __Pyx_RefNanny = __Pyx_RefNannyImportAPI("refnanny");
 if (!__Pyx_RefNanny) {
   PyErr_Clear();
   __Pyx_RefNanny = __Pyx_RefNannyImportAPI("Cython.Runtime.refnanny");
   if (!__Pyx_RefNanny)
       Py_FatalError("failed to import 'refnanny' module");
@@ -2981,68 +4184,51 @@
   #ifdef __Pxy_PyFrame_Initialize_Offsets
   __Pxy_PyFrame_Initialize_Offsets();
   #endif
   __pyx_empty_tuple = PyTuple_New(0); if (unlikely(!__pyx_empty_tuple)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_empty_bytes = PyBytes_FromStringAndSize("", 0); if (unlikely(!__pyx_empty_bytes)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_empty_unicode = PyUnicode_FromStringAndSize("", 0); if (unlikely(!__pyx_empty_unicode)) __PYX_ERR(0, 1, __pyx_L1_error)
   #ifdef __Pyx_CyFunction_USED
-  if (__pyx_CyFunction_init() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__pyx_CyFunction_init(__pyx_m) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   #ifdef __Pyx_FusedFunction_USED
-  if (__pyx_FusedFunction_init() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__pyx_FusedFunction_init(__pyx_m) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   #ifdef __Pyx_Coroutine_USED
-  if (__pyx_Coroutine_init() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__pyx_Coroutine_init(__pyx_m) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   #ifdef __Pyx_Generator_USED
-  if (__pyx_Generator_init() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__pyx_Generator_init(__pyx_m) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   #ifdef __Pyx_AsyncGen_USED
-  if (__pyx_AsyncGen_init() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__pyx_AsyncGen_init(__pyx_m) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   #ifdef __Pyx_StopAsyncIteration_USED
-  if (__pyx_StopAsyncIteration_init() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__pyx_StopAsyncIteration_init(__pyx_m) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   /*--- Library function declarations ---*/
   /*--- Threads initialization code ---*/
   #if defined(WITH_THREAD) && PY_VERSION_HEX < 0x030700F0 && defined(__PYX_FORCE_INIT_THREADS) && __PYX_FORCE_INIT_THREADS
   PyEval_InitThreads();
   #endif
-  /*--- Module creation code ---*/
-  #if CYTHON_PEP489_MULTI_PHASE_INIT
-  __pyx_m = __pyx_pyinit_module;
-  Py_INCREF(__pyx_m);
-  #else
-  #if PY_MAJOR_VERSION < 3
-  __pyx_m = Py_InitModule4("_atimer", __pyx_methods, 0, 0, PYTHON_API_VERSION); Py_XINCREF(__pyx_m);
-  #else
-  __pyx_m = PyModule_Create(&__pyx_moduledef);
-  #endif
-  if (unlikely(!__pyx_m)) __PYX_ERR(0, 1, __pyx_L1_error)
-  #endif
-  __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(0, 1, __pyx_L1_error)
-  Py_INCREF(__pyx_d);
-  __pyx_b = PyImport_AddModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(0, 1, __pyx_L1_error)
-  Py_INCREF(__pyx_b);
-  __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(0, 1, __pyx_L1_error)
-  Py_INCREF(__pyx_cython_runtime);
-  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
   /*--- Initialize various global constants etc. ---*/
+  if (__Pyx_InitConstants() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  stringtab_initialized = 1;
   if (__Pyx_InitGlobals() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #if PY_MAJOR_VERSION < 3 && (__PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT)
   if (__Pyx_init_sys_getdefaultencoding_params() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   if (__pyx_module_is_main_atimer___atimer) {
     if (PyObject_SetAttr(__pyx_m, __pyx_n_s_name, __pyx_n_s_main) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   }
   #if PY_MAJOR_VERSION >= 3
   {
     PyObject *modules = PyImport_GetModuleDict(); if (unlikely(!modules)) __PYX_ERR(0, 1, __pyx_L1_error)
     if (!PyDict_GetItemString(modules, "atimer._atimer")) {
-      if (unlikely(PyDict_SetItemString(modules, "atimer._atimer", __pyx_m) < 0)) __PYX_ERR(0, 1, __pyx_L1_error)
+      if (unlikely((PyDict_SetItemString(modules, "atimer._atimer", __pyx_m) < 0))) __PYX_ERR(0, 1, __pyx_L1_error)
     }
   }
   #endif
   /*--- Builtin init code ---*/
   if (__Pyx_InitCachedBuiltins() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Constants init code ---*/
   if (__Pyx_InitCachedConstants() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -3062,132 +4248,150 @@
   /* "atimer/_atimer.pyx":22
  * #
  * 
  * import time             # <<<<<<<<<<<<<<
  * 
  * from posix.unistd cimport close
  */
-  __pyx_t_1 = __Pyx_Import(__pyx_n_s_time, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 22, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_time, __pyx_t_1) < 0) __PYX_ERR(0, 22, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_2 = __Pyx_ImportDottedModule(__pyx_n_s_time, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 22, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_time, __pyx_t_2) < 0) __PYX_ERR(0, 22, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "atimer/_atimer.pyx":28
  * from libc.time cimport time_t
  * 
  * NANOSEC = int(1e9)             # <<<<<<<<<<<<<<
  * 
  * cdef extern from "<sys/timerfd.h>":
  */
-  __pyx_t_1 = __Pyx_PyNumber_Int(__pyx_float_1e9); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 28, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_NANOSEC, __pyx_t_1) < 0) __PYX_ERR(0, 28, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_2 = __Pyx_PyNumber_Int(__pyx_float_1e9); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 28, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_NANOSEC, __pyx_t_2) < 0) __PYX_ERR(0, 28, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "atimer/_atimer.pyx":39
  *     int timerfd_gettime(int, itimerspec*)
  * 
  * def atimer_init():             # <<<<<<<<<<<<<<
  *     # CLOCK_BOOTIME: count number of expirations when running machine is
  *     # suspended
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_6atimer_7_atimer_1atimer_init, NULL, __pyx_n_s_atimer__atimer); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 39, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_atimer_init, __pyx_t_1) < 0) __PYX_ERR(0, 39, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_6atimer_7_atimer_1atimer_init, 0, __pyx_n_s_atimer_init, NULL, __pyx_n_s_atimer__atimer, __pyx_d, ((PyObject *)__pyx_codeobj__4)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 39, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_atimer_init, __pyx_t_2) < 0) __PYX_ERR(0, 39, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "atimer/_atimer.pyx":46
  *     return timerfd_create(CLOCK_BOOTTIME, TFD_NONBLOCK)
  * 
  * def atimer_start(int fd, double interval):             # <<<<<<<<<<<<<<
  *     cdef itimerspec ts
  *     cdef timespec now
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_6atimer_7_atimer_3atimer_start, NULL, __pyx_n_s_atimer__atimer); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 46, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_atimer_start, __pyx_t_1) < 0) __PYX_ERR(0, 46, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_6atimer_7_atimer_3atimer_start, 0, __pyx_n_s_atimer_start, NULL, __pyx_n_s_atimer__atimer, __pyx_d, ((PyObject *)__pyx_codeobj__6)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 46, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_atimer_start, __pyx_t_2) < 0) __PYX_ERR(0, 46, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "atimer/_atimer.pyx":65
  *     return timerfd_settime(fd, TFD_TIMER_ABSTIME, &ts, NULL)
  * 
  * def atimer_close(int fd):             # <<<<<<<<<<<<<<
  *     cdef int r
  *     cdef itimerspec ts
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_6atimer_7_atimer_5atimer_close, NULL, __pyx_n_s_atimer__atimer); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 65, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_atimer_close, __pyx_t_1) < 0) __PYX_ERR(0, 65, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_6atimer_7_atimer_5atimer_close, 0, __pyx_n_s_atimer_close, NULL, __pyx_n_s_atimer__atimer, __pyx_d, ((PyObject *)__pyx_codeobj__8)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 65, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_atimer_close, __pyx_t_2) < 0) __PYX_ERR(0, 65, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "atimer/_atimer.pyx":79
  *     return r
  * 
  * def to_timespec(double value):             # <<<<<<<<<<<<<<
  *     """
  *     Convert float number to `timespec` value.
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_6atimer_7_atimer_7to_timespec, NULL, __pyx_n_s_atimer__atimer); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 79, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_to_timespec, __pyx_t_1) < 0) __PYX_ERR(0, 79, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_6atimer_7_atimer_7to_timespec, 0, __pyx_n_s_to_timespec, NULL, __pyx_n_s_atimer__atimer, __pyx_d, ((PyObject *)__pyx_codeobj__10)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 79, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_to_timespec, __pyx_t_2) < 0) __PYX_ERR(0, 79, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "atimer/_atimer.pyx":98
  *     return sec, nsec
  * 
  * def timespec_add(timespec now, time_t sec, long nsec):             # <<<<<<<<<<<<<<
  *     now.tv_sec += sec + (now.tv_nsec + nsec) / NANOSEC
  *     now.tv_nsec = (now.tv_nsec + nsec) % NANOSEC
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_6atimer_7_atimer_9timespec_add, NULL, __pyx_n_s_atimer__atimer); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 98, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_timespec_add, __pyx_t_1) < 0) __PYX_ERR(0, 98, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_6atimer_7_atimer_9timespec_add, 0, __pyx_n_s_timespec_add, NULL, __pyx_n_s_atimer__atimer, __pyx_d, ((PyObject *)__pyx_codeobj__12)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 98, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_timespec_add, __pyx_t_2) < 0) __PYX_ERR(0, 98, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "atimer/_atimer.pyx":1
  * #             # <<<<<<<<<<<<<<
  * # atimer - timer library for asyncio
  * #
  */
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_1) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-
-  /* "FromPyStructUtility":11
- * 
- * @cname("__pyx_convert__from_py_struct__timespec")
- * cdef struct_type __pyx_convert__from_py_struct__timespec(obj) except *:             # <<<<<<<<<<<<<<
- *     cdef struct_type result
- *     if not PyMapping_Check(obj):
- */
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_2) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /*--- Wrapped vars code ---*/
 
   goto __pyx_L0;
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_2);
   if (__pyx_m) {
-    if (__pyx_d) {
+    if (__pyx_d && stringtab_initialized) {
       __Pyx_AddTraceback("init atimer._atimer", __pyx_clineno, __pyx_lineno, __pyx_filename);
     }
+    #if !CYTHON_USE_MODULE_STATE
     Py_CLEAR(__pyx_m);
+    #else
+    Py_DECREF(__pyx_m);
+    if (pystate_addmodule_run) {
+      PyObject *tp, *value, *tb;
+      PyErr_Fetch(&tp, &value, &tb);
+      PyState_RemoveModule(&__pyx_moduledef);
+      PyErr_Restore(tp, value, tb);
+    }
+    #endif
   } else if (!PyErr_Occurred()) {
     PyErr_SetString(PyExc_ImportError, "init atimer._atimer");
   }
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   return (__pyx_m != NULL) ? 0 : -1;
   #elif PY_MAJOR_VERSION >= 3
   return __pyx_m;
   #else
   return;
   #endif
 }
+/* #### Code section: cleanup_globals ### */
+/* #### Code section: cleanup_module ### */
+/* #### Code section: main_method ### */
+/* #### Code section: utility_code_pragmas ### */
+#ifdef _MSC_VER
+#pragma warning( push )
+/* Warning 4127: conditional expression is constant
+ * Cython uses constant conditional expressions to allow in inline functions to be optimized at
+ * compile-time, so this warning is not useful
+ */
+#pragma warning( disable : 4127 )
+#endif
+
+
+
+/* #### Code section: utility_code_def ### */
 
 /* --- Runtime support code --- */
 /* Refnanny */
 #if CYTHON_REFNANNY
 static __Pyx_RefNannyAPIStruct *__Pyx_RefNannyImportAPI(const char *modname) {
     PyObject *m = NULL, *p = NULL;
     void *r = NULL;
@@ -3199,14 +4403,753 @@
 end:
     Py_XDECREF(p);
     Py_XDECREF(m);
     return (__Pyx_RefNannyAPIStruct *)r;
 }
 #endif
 
+/* PyErrExceptionMatches */
+#if CYTHON_FAST_THREAD_STATE
+static int __Pyx_PyErr_ExceptionMatchesTuple(PyObject *exc_type, PyObject *tuple) {
+    Py_ssize_t i, n;
+    n = PyTuple_GET_SIZE(tuple);
+#if PY_MAJOR_VERSION >= 3
+    for (i=0; i<n; i++) {
+        if (exc_type == PyTuple_GET_ITEM(tuple, i)) return 1;
+    }
+#endif
+    for (i=0; i<n; i++) {
+        if (__Pyx_PyErr_GivenExceptionMatches(exc_type, PyTuple_GET_ITEM(tuple, i))) return 1;
+    }
+    return 0;
+}
+static CYTHON_INLINE int __Pyx_PyErr_ExceptionMatchesInState(PyThreadState* tstate, PyObject* err) {
+    int result;
+    PyObject *exc_type;
+#if PY_VERSION_HEX >= 0x030C00A6
+    PyObject *current_exception = tstate->current_exception;
+    if (unlikely(!current_exception)) return 0;
+    exc_type = (PyObject*) Py_TYPE(current_exception);
+    if (exc_type == err) return 1;
+#else
+    exc_type = tstate->curexc_type;
+    if (exc_type == err) return 1;
+    if (unlikely(!exc_type)) return 0;
+#endif
+    #if CYTHON_AVOID_BORROWED_REFS
+    Py_INCREF(exc_type);
+    #endif
+    if (unlikely(PyTuple_Check(err))) {
+        result = __Pyx_PyErr_ExceptionMatchesTuple(exc_type, err);
+    } else {
+        result = __Pyx_PyErr_GivenExceptionMatches(exc_type, err);
+    }
+    #if CYTHON_AVOID_BORROWED_REFS
+    Py_DECREF(exc_type);
+    #endif
+    return result;
+}
+#endif
+
+/* PyErrFetchRestore */
+#if CYTHON_FAST_THREAD_STATE
+static CYTHON_INLINE void __Pyx_ErrRestoreInState(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb) {
+#if PY_VERSION_HEX >= 0x030C00A6
+    PyObject *tmp_value;
+    assert(type == NULL || (value != NULL && type == (PyObject*) Py_TYPE(value)));
+    if (value) {
+        #if CYTHON_COMPILING_IN_CPYTHON
+        if (unlikely(((PyBaseExceptionObject*) value)->traceback != tb))
+        #endif
+            PyException_SetTraceback(value, tb);
+    }
+    tmp_value = tstate->current_exception;
+    tstate->current_exception = value;
+    Py_XDECREF(tmp_value);
+#else
+    PyObject *tmp_type, *tmp_value, *tmp_tb;
+    tmp_type = tstate->curexc_type;
+    tmp_value = tstate->curexc_value;
+    tmp_tb = tstate->curexc_traceback;
+    tstate->curexc_type = type;
+    tstate->curexc_value = value;
+    tstate->curexc_traceback = tb;
+    Py_XDECREF(tmp_type);
+    Py_XDECREF(tmp_value);
+    Py_XDECREF(tmp_tb);
+#endif
+}
+static CYTHON_INLINE void __Pyx_ErrFetchInState(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb) {
+#if PY_VERSION_HEX >= 0x030C00A6
+    PyObject* exc_value;
+    exc_value = tstate->current_exception;
+    tstate->current_exception = 0;
+    *value = exc_value;
+    *type = NULL;
+    *tb = NULL;
+    if (exc_value) {
+        *type = (PyObject*) Py_TYPE(exc_value);
+        Py_INCREF(*type);
+        #if CYTHON_COMPILING_IN_CPYTHON
+        *tb = ((PyBaseExceptionObject*) exc_value)->traceback;
+        Py_XINCREF(*tb);
+        #else
+        *tb = PyException_GetTraceback(exc_value);
+        #endif
+    }
+#else
+    *type = tstate->curexc_type;
+    *value = tstate->curexc_value;
+    *tb = tstate->curexc_traceback;
+    tstate->curexc_type = 0;
+    tstate->curexc_value = 0;
+    tstate->curexc_traceback = 0;
+#endif
+}
+#endif
+
+/* PyObjectGetAttrStr */
+#if CYTHON_USE_TYPE_SLOTS
+static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStr(PyObject* obj, PyObject* attr_name) {
+    PyTypeObject* tp = Py_TYPE(obj);
+    if (likely(tp->tp_getattro))
+        return tp->tp_getattro(obj, attr_name);
+#if PY_MAJOR_VERSION < 3
+    if (likely(tp->tp_getattr))
+        return tp->tp_getattr(obj, PyString_AS_STRING(attr_name));
+#endif
+    return PyObject_GetAttr(obj, attr_name);
+}
+#endif
+
+/* PyObjectGetAttrStrNoError */
+static void __Pyx_PyObject_GetAttrStr_ClearAttributeError(void) {
+    __Pyx_PyThreadState_declare
+    __Pyx_PyThreadState_assign
+    if (likely(__Pyx_PyErr_ExceptionMatches(PyExc_AttributeError)))
+        __Pyx_PyErr_Clear();
+}
+static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name) {
+    PyObject *result;
+#if CYTHON_COMPILING_IN_CPYTHON && CYTHON_USE_TYPE_SLOTS && PY_VERSION_HEX >= 0x030700B1
+    PyTypeObject* tp = Py_TYPE(obj);
+    if (likely(tp->tp_getattro == PyObject_GenericGetAttr)) {
+        return _PyObject_GenericGetAttrWithDict(obj, attr_name, NULL, 1);
+    }
+#endif
+    result = __Pyx_PyObject_GetAttrStr(obj, attr_name);
+    if (unlikely(!result)) {
+        __Pyx_PyObject_GetAttrStr_ClearAttributeError();
+    }
+    return result;
+}
+
+/* GetBuiltinName */
+static PyObject *__Pyx_GetBuiltinName(PyObject *name) {
+    PyObject* result = __Pyx_PyObject_GetAttrStrNoError(__pyx_b, name);
+    if (unlikely(!result) && !PyErr_Occurred()) {
+        PyErr_Format(PyExc_NameError,
+#if PY_MAJOR_VERSION >= 3
+            "name '%U' is not defined", name);
+#else
+            "name '%.200s' is not defined", PyString_AS_STRING(name));
+#endif
+    }
+    return result;
+}
+
+/* DictGetItem */
+#if PY_MAJOR_VERSION >= 3 && !CYTHON_COMPILING_IN_PYPY
+static PyObject *__Pyx_PyDict_GetItem(PyObject *d, PyObject* key) {
+    PyObject *value;
+    value = PyDict_GetItemWithError(d, key);
+    if (unlikely(!value)) {
+        if (!PyErr_Occurred()) {
+            if (unlikely(PyTuple_Check(key))) {
+                PyObject* args = PyTuple_Pack(1, key);
+                if (likely(args)) {
+                    PyErr_SetObject(PyExc_KeyError, args);
+                    Py_DECREF(args);
+                }
+            } else {
+                PyErr_SetObject(PyExc_KeyError, key);
+            }
+        }
+        return NULL;
+    }
+    Py_INCREF(value);
+    return value;
+}
+#endif
+
+/* GetTopmostException */
+#if CYTHON_USE_EXC_INFO_STACK && CYTHON_FAST_THREAD_STATE
+static _PyErr_StackItem *
+__Pyx_PyErr_GetTopmostException(PyThreadState *tstate)
+{
+    _PyErr_StackItem *exc_info = tstate->exc_info;
+    while ((exc_info->exc_value == NULL || exc_info->exc_value == Py_None) &&
+           exc_info->previous_item != NULL)
+    {
+        exc_info = exc_info->previous_item;
+    }
+    return exc_info;
+}
+#endif
+
+/* SaveResetException */
+#if CYTHON_FAST_THREAD_STATE
+static CYTHON_INLINE void __Pyx__ExceptionSave(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb) {
+  #if CYTHON_USE_EXC_INFO_STACK && PY_VERSION_HEX >= 0x030B00a4
+    _PyErr_StackItem *exc_info = __Pyx_PyErr_GetTopmostException(tstate);
+    PyObject *exc_value = exc_info->exc_value;
+    if (exc_value == NULL || exc_value == Py_None) {
+        *value = NULL;
+        *type = NULL;
+        *tb = NULL;
+    } else {
+        *value = exc_value;
+        Py_INCREF(*value);
+        *type = (PyObject*) Py_TYPE(exc_value);
+        Py_INCREF(*type);
+        *tb = PyException_GetTraceback(exc_value);
+    }
+  #elif CYTHON_USE_EXC_INFO_STACK
+    _PyErr_StackItem *exc_info = __Pyx_PyErr_GetTopmostException(tstate);
+    *type = exc_info->exc_type;
+    *value = exc_info->exc_value;
+    *tb = exc_info->exc_traceback;
+    Py_XINCREF(*type);
+    Py_XINCREF(*value);
+    Py_XINCREF(*tb);
+  #else
+    *type = tstate->exc_type;
+    *value = tstate->exc_value;
+    *tb = tstate->exc_traceback;
+    Py_XINCREF(*type);
+    Py_XINCREF(*value);
+    Py_XINCREF(*tb);
+  #endif
+}
+static CYTHON_INLINE void __Pyx__ExceptionReset(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb) {
+  #if CYTHON_USE_EXC_INFO_STACK && PY_VERSION_HEX >= 0x030B00a4
+    _PyErr_StackItem *exc_info = tstate->exc_info;
+    PyObject *tmp_value = exc_info->exc_value;
+    exc_info->exc_value = value;
+    Py_XDECREF(tmp_value);
+    Py_XDECREF(type);
+    Py_XDECREF(tb);
+  #else
+    PyObject *tmp_type, *tmp_value, *tmp_tb;
+    #if CYTHON_USE_EXC_INFO_STACK
+    _PyErr_StackItem *exc_info = tstate->exc_info;
+    tmp_type = exc_info->exc_type;
+    tmp_value = exc_info->exc_value;
+    tmp_tb = exc_info->exc_traceback;
+    exc_info->exc_type = type;
+    exc_info->exc_value = value;
+    exc_info->exc_traceback = tb;
+    #else
+    tmp_type = tstate->exc_type;
+    tmp_value = tstate->exc_value;
+    tmp_tb = tstate->exc_traceback;
+    tstate->exc_type = type;
+    tstate->exc_value = value;
+    tstate->exc_traceback = tb;
+    #endif
+    Py_XDECREF(tmp_type);
+    Py_XDECREF(tmp_value);
+    Py_XDECREF(tmp_tb);
+  #endif
+}
+#endif
+
+/* GetException */
+#if CYTHON_FAST_THREAD_STATE
+static int __Pyx__GetException(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb)
+#else
+static int __Pyx_GetException(PyObject **type, PyObject **value, PyObject **tb)
+#endif
+{
+    PyObject *local_type = NULL, *local_value, *local_tb = NULL;
+#if CYTHON_FAST_THREAD_STATE
+    PyObject *tmp_type, *tmp_value, *tmp_tb;
+  #if PY_VERSION_HEX >= 0x030C00A6
+    local_value = tstate->current_exception;
+    tstate->current_exception = 0;
+    if (likely(local_value)) {
+        local_type = (PyObject*) Py_TYPE(local_value);
+        Py_INCREF(local_type);
+        local_tb = PyException_GetTraceback(local_value);
+    }
+  #else
+    local_type = tstate->curexc_type;
+    local_value = tstate->curexc_value;
+    local_tb = tstate->curexc_traceback;
+    tstate->curexc_type = 0;
+    tstate->curexc_value = 0;
+    tstate->curexc_traceback = 0;
+  #endif
+#else
+    PyErr_Fetch(&local_type, &local_value, &local_tb);
+#endif
+    PyErr_NormalizeException(&local_type, &local_value, &local_tb);
+#if CYTHON_FAST_THREAD_STATE && PY_VERSION_HEX >= 0x030C00A6
+    if (unlikely(tstate->current_exception))
+#elif CYTHON_FAST_THREAD_STATE
+    if (unlikely(tstate->curexc_type))
+#else
+    if (unlikely(PyErr_Occurred()))
+#endif
+        goto bad;
+    #if PY_MAJOR_VERSION >= 3
+    if (local_tb) {
+        if (unlikely(PyException_SetTraceback(local_value, local_tb) < 0))
+            goto bad;
+    }
+    #endif
+    Py_XINCREF(local_tb);
+    Py_XINCREF(local_type);
+    Py_XINCREF(local_value);
+    *type = local_type;
+    *value = local_value;
+    *tb = local_tb;
+#if CYTHON_FAST_THREAD_STATE
+    #if CYTHON_USE_EXC_INFO_STACK
+    {
+        _PyErr_StackItem *exc_info = tstate->exc_info;
+      #if PY_VERSION_HEX >= 0x030B00a4
+        tmp_value = exc_info->exc_value;
+        exc_info->exc_value = local_value;
+        tmp_type = NULL;
+        tmp_tb = NULL;
+        Py_XDECREF(local_type);
+        Py_XDECREF(local_tb);
+      #else
+        tmp_type = exc_info->exc_type;
+        tmp_value = exc_info->exc_value;
+        tmp_tb = exc_info->exc_traceback;
+        exc_info->exc_type = local_type;
+        exc_info->exc_value = local_value;
+        exc_info->exc_traceback = local_tb;
+      #endif
+    }
+    #else
+    tmp_type = tstate->exc_type;
+    tmp_value = tstate->exc_value;
+    tmp_tb = tstate->exc_traceback;
+    tstate->exc_type = local_type;
+    tstate->exc_value = local_value;
+    tstate->exc_traceback = local_tb;
+    #endif
+    Py_XDECREF(tmp_type);
+    Py_XDECREF(tmp_value);
+    Py_XDECREF(tmp_tb);
+#else
+    PyErr_SetExcInfo(local_type, local_value, local_tb);
+#endif
+    return 0;
+bad:
+    *type = 0;
+    *value = 0;
+    *tb = 0;
+    Py_XDECREF(local_type);
+    Py_XDECREF(local_value);
+    Py_XDECREF(local_tb);
+    return -1;
+}
+
+/* PyObjectCall */
+#if CYTHON_COMPILING_IN_CPYTHON
+static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw) {
+    PyObject *result;
+    ternaryfunc call = Py_TYPE(func)->tp_call;
+    if (unlikely(!call))
+        return PyObject_Call(func, arg, kw);
+    if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object")))
+        return NULL;
+    result = (*call)(func, arg, kw);
+    Py_LeaveRecursiveCall();
+    if (unlikely(!result) && unlikely(!PyErr_Occurred())) {
+        PyErr_SetString(
+            PyExc_SystemError,
+            "NULL result without error in PyObject_Call");
+    }
+    return result;
+}
+#endif
+
+/* RaiseException */
+#if PY_MAJOR_VERSION < 3
+static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause) {
+    __Pyx_PyThreadState_declare
+    CYTHON_UNUSED_VAR(cause);
+    Py_XINCREF(type);
+    if (!value || value == Py_None)
+        value = NULL;
+    else
+        Py_INCREF(value);
+    if (!tb || tb == Py_None)
+        tb = NULL;
+    else {
+        Py_INCREF(tb);
+        if (!PyTraceBack_Check(tb)) {
+            PyErr_SetString(PyExc_TypeError,
+                "raise: arg 3 must be a traceback or None");
+            goto raise_error;
+        }
+    }
+    if (PyType_Check(type)) {
+#if CYTHON_COMPILING_IN_PYPY
+        if (!value) {
+            Py_INCREF(Py_None);
+            value = Py_None;
+        }
+#endif
+        PyErr_NormalizeException(&type, &value, &tb);
+    } else {
+        if (value) {
+            PyErr_SetString(PyExc_TypeError,
+                "instance exception may not have a separate value");
+            goto raise_error;
+        }
+        value = type;
+        type = (PyObject*) Py_TYPE(type);
+        Py_INCREF(type);
+        if (!PyType_IsSubtype((PyTypeObject *)type, (PyTypeObject *)PyExc_BaseException)) {
+            PyErr_SetString(PyExc_TypeError,
+                "raise: exception class must be a subclass of BaseException");
+            goto raise_error;
+        }
+    }
+    __Pyx_PyThreadState_assign
+    __Pyx_ErrRestore(type, value, tb);
+    return;
+raise_error:
+    Py_XDECREF(value);
+    Py_XDECREF(type);
+    Py_XDECREF(tb);
+    return;
+}
+#else
+static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause) {
+    PyObject* owned_instance = NULL;
+    if (tb == Py_None) {
+        tb = 0;
+    } else if (tb && !PyTraceBack_Check(tb)) {
+        PyErr_SetString(PyExc_TypeError,
+            "raise: arg 3 must be a traceback or None");
+        goto bad;
+    }
+    if (value == Py_None)
+        value = 0;
+    if (PyExceptionInstance_Check(type)) {
+        if (value) {
+            PyErr_SetString(PyExc_TypeError,
+                "instance exception may not have a separate value");
+            goto bad;
+        }
+        value = type;
+        type = (PyObject*) Py_TYPE(value);
+    } else if (PyExceptionClass_Check(type)) {
+        PyObject *instance_class = NULL;
+        if (value && PyExceptionInstance_Check(value)) {
+            instance_class = (PyObject*) Py_TYPE(value);
+            if (instance_class != type) {
+                int is_subclass = PyObject_IsSubclass(instance_class, type);
+                if (!is_subclass) {
+                    instance_class = NULL;
+                } else if (unlikely(is_subclass == -1)) {
+                    goto bad;
+                } else {
+                    type = instance_class;
+                }
+            }
+        }
+        if (!instance_class) {
+            PyObject *args;
+            if (!value)
+                args = PyTuple_New(0);
+            else if (PyTuple_Check(value)) {
+                Py_INCREF(value);
+                args = value;
+            } else
+                args = PyTuple_Pack(1, value);
+            if (!args)
+                goto bad;
+            owned_instance = PyObject_Call(type, args, NULL);
+            Py_DECREF(args);
+            if (!owned_instance)
+                goto bad;
+            value = owned_instance;
+            if (!PyExceptionInstance_Check(value)) {
+                PyErr_Format(PyExc_TypeError,
+                             "calling %R should have returned an instance of "
+                             "BaseException, not %R",
+                             type, Py_TYPE(value));
+                goto bad;
+            }
+        }
+    } else {
+        PyErr_SetString(PyExc_TypeError,
+            "raise: exception class must be a subclass of BaseException");
+        goto bad;
+    }
+    if (cause) {
+        PyObject *fixed_cause;
+        if (cause == Py_None) {
+            fixed_cause = NULL;
+        } else if (PyExceptionClass_Check(cause)) {
+            fixed_cause = PyObject_CallObject(cause, NULL);
+            if (fixed_cause == NULL)
+                goto bad;
+        } else if (PyExceptionInstance_Check(cause)) {
+            fixed_cause = cause;
+            Py_INCREF(fixed_cause);
+        } else {
+            PyErr_SetString(PyExc_TypeError,
+                            "exception causes must derive from "
+                            "BaseException");
+            goto bad;
+        }
+        PyException_SetCause(value, fixed_cause);
+    }
+    PyErr_SetObject(type, value);
+    if (tb) {
+      #if PY_VERSION_HEX >= 0x030C00A6
+        PyException_SetTraceback(value, tb);
+      #elif CYTHON_FAST_THREAD_STATE
+        PyThreadState *tstate = __Pyx_PyThreadState_Current;
+        PyObject* tmp_tb = tstate->curexc_traceback;
+        if (tb != tmp_tb) {
+            Py_INCREF(tb);
+            tstate->curexc_traceback = tb;
+            Py_XDECREF(tmp_tb);
+        }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
+#endif
+    }
+bad:
+    Py_XDECREF(owned_instance);
+    return;
+}
+#endif
+
+/* TupleAndListFromArray */
+#if CYTHON_COMPILING_IN_CPYTHON
+static CYTHON_INLINE void __Pyx_copy_object_array(PyObject *const *CYTHON_RESTRICT src, PyObject** CYTHON_RESTRICT dest, Py_ssize_t length) {
+    PyObject *v;
+    Py_ssize_t i;
+    for (i = 0; i < length; i++) {
+        v = dest[i] = src[i];
+        Py_INCREF(v);
+    }
+}
+static CYTHON_INLINE PyObject *
+__Pyx_PyTuple_FromArray(PyObject *const *src, Py_ssize_t n)
+{
+    PyObject *res;
+    if (n <= 0) {
+        Py_INCREF(__pyx_empty_tuple);
+        return __pyx_empty_tuple;
+    }
+    res = PyTuple_New(n);
+    if (unlikely(res == NULL)) return NULL;
+    __Pyx_copy_object_array(src, ((PyTupleObject*)res)->ob_item, n);
+    return res;
+}
+static CYTHON_INLINE PyObject *
+__Pyx_PyList_FromArray(PyObject *const *src, Py_ssize_t n)
+{
+    PyObject *res;
+    if (n <= 0) {
+        return PyList_New(0);
+    }
+    res = PyList_New(n);
+    if (unlikely(res == NULL)) return NULL;
+    __Pyx_copy_object_array(src, ((PyListObject*)res)->ob_item, n);
+    return res;
+}
+#endif
+
+/* BytesEquals */
+static CYTHON_INLINE int __Pyx_PyBytes_Equals(PyObject* s1, PyObject* s2, int equals) {
+#if CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API
+    return PyObject_RichCompareBool(s1, s2, equals);
+#else
+    if (s1 == s2) {
+        return (equals == Py_EQ);
+    } else if (PyBytes_CheckExact(s1) & PyBytes_CheckExact(s2)) {
+        const char *ps1, *ps2;
+        Py_ssize_t length = PyBytes_GET_SIZE(s1);
+        if (length != PyBytes_GET_SIZE(s2))
+            return (equals == Py_NE);
+        ps1 = PyBytes_AS_STRING(s1);
+        ps2 = PyBytes_AS_STRING(s2);
+        if (ps1[0] != ps2[0]) {
+            return (equals == Py_NE);
+        } else if (length == 1) {
+            return (equals == Py_EQ);
+        } else {
+            int result;
+#if CYTHON_USE_UNICODE_INTERNALS && (PY_VERSION_HEX < 0x030B0000)
+            Py_hash_t hash1, hash2;
+            hash1 = ((PyBytesObject*)s1)->ob_shash;
+            hash2 = ((PyBytesObject*)s2)->ob_shash;
+            if (hash1 != hash2 && hash1 != -1 && hash2 != -1) {
+                return (equals == Py_NE);
+            }
+#endif
+            result = memcmp(ps1, ps2, (size_t)length);
+            return (equals == Py_EQ) ? (result == 0) : (result != 0);
+        }
+    } else if ((s1 == Py_None) & PyBytes_CheckExact(s2)) {
+        return (equals == Py_NE);
+    } else if ((s2 == Py_None) & PyBytes_CheckExact(s1)) {
+        return (equals == Py_NE);
+    } else {
+        int result;
+        PyObject* py_result = PyObject_RichCompare(s1, s2, equals);
+        if (!py_result)
+            return -1;
+        result = __Pyx_PyObject_IsTrue(py_result);
+        Py_DECREF(py_result);
+        return result;
+    }
+#endif
+}
+
+/* UnicodeEquals */
+static CYTHON_INLINE int __Pyx_PyUnicode_Equals(PyObject* s1, PyObject* s2, int equals) {
+#if CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API
+    return PyObject_RichCompareBool(s1, s2, equals);
+#else
+#if PY_MAJOR_VERSION < 3
+    PyObject* owned_ref = NULL;
+#endif
+    int s1_is_unicode, s2_is_unicode;
+    if (s1 == s2) {
+        goto return_eq;
+    }
+    s1_is_unicode = PyUnicode_CheckExact(s1);
+    s2_is_unicode = PyUnicode_CheckExact(s2);
+#if PY_MAJOR_VERSION < 3
+    if ((s1_is_unicode & (!s2_is_unicode)) && PyString_CheckExact(s2)) {
+        owned_ref = PyUnicode_FromObject(s2);
+        if (unlikely(!owned_ref))
+            return -1;
+        s2 = owned_ref;
+        s2_is_unicode = 1;
+    } else if ((s2_is_unicode & (!s1_is_unicode)) && PyString_CheckExact(s1)) {
+        owned_ref = PyUnicode_FromObject(s1);
+        if (unlikely(!owned_ref))
+            return -1;
+        s1 = owned_ref;
+        s1_is_unicode = 1;
+    } else if (((!s2_is_unicode) & (!s1_is_unicode))) {
+        return __Pyx_PyBytes_Equals(s1, s2, equals);
+    }
+#endif
+    if (s1_is_unicode & s2_is_unicode) {
+        Py_ssize_t length;
+        int kind;
+        void *data1, *data2;
+        if (unlikely(__Pyx_PyUnicode_READY(s1) < 0) || unlikely(__Pyx_PyUnicode_READY(s2) < 0))
+            return -1;
+        length = __Pyx_PyUnicode_GET_LENGTH(s1);
+        if (length != __Pyx_PyUnicode_GET_LENGTH(s2)) {
+            goto return_ne;
+        }
+#if CYTHON_USE_UNICODE_INTERNALS
+        {
+            Py_hash_t hash1, hash2;
+        #if CYTHON_PEP393_ENABLED
+            hash1 = ((PyASCIIObject*)s1)->hash;
+            hash2 = ((PyASCIIObject*)s2)->hash;
+        #else
+            hash1 = ((PyUnicodeObject*)s1)->hash;
+            hash2 = ((PyUnicodeObject*)s2)->hash;
+        #endif
+            if (hash1 != hash2 && hash1 != -1 && hash2 != -1) {
+                goto return_ne;
+            }
+        }
+#endif
+        kind = __Pyx_PyUnicode_KIND(s1);
+        if (kind != __Pyx_PyUnicode_KIND(s2)) {
+            goto return_ne;
+        }
+        data1 = __Pyx_PyUnicode_DATA(s1);
+        data2 = __Pyx_PyUnicode_DATA(s2);
+        if (__Pyx_PyUnicode_READ(kind, data1, 0) != __Pyx_PyUnicode_READ(kind, data2, 0)) {
+            goto return_ne;
+        } else if (length == 1) {
+            goto return_eq;
+        } else {
+            int result = memcmp(data1, data2, (size_t)(length * kind));
+            #if PY_MAJOR_VERSION < 3
+            Py_XDECREF(owned_ref);
+            #endif
+            return (equals == Py_EQ) ? (result == 0) : (result != 0);
+        }
+    } else if ((s1 == Py_None) & s2_is_unicode) {
+        goto return_ne;
+    } else if ((s2 == Py_None) & s1_is_unicode) {
+        goto return_ne;
+    } else {
+        int result;
+        PyObject* py_result = PyObject_RichCompare(s1, s2, equals);
+        #if PY_MAJOR_VERSION < 3
+        Py_XDECREF(owned_ref);
+        #endif
+        if (!py_result)
+            return -1;
+        result = __Pyx_PyObject_IsTrue(py_result);
+        Py_DECREF(py_result);
+        return result;
+    }
+return_eq:
+    #if PY_MAJOR_VERSION < 3
+    Py_XDECREF(owned_ref);
+    #endif
+    return (equals == Py_EQ);
+return_ne:
+    #if PY_MAJOR_VERSION < 3
+    Py_XDECREF(owned_ref);
+    #endif
+    return (equals == Py_NE);
+#endif
+}
+
+/* fastcall */
+#if CYTHON_METH_FASTCALL
+static CYTHON_INLINE PyObject * __Pyx_GetKwValue_FASTCALL(PyObject *kwnames, PyObject *const *kwvalues, PyObject *s)
+{
+    Py_ssize_t i, n = PyTuple_GET_SIZE(kwnames);
+    for (i = 0; i < n; i++)
+    {
+        if (s == PyTuple_GET_ITEM(kwnames, i)) return kwvalues[i];
+    }
+    for (i = 0; i < n; i++)
+    {
+        int eq = __Pyx_PyUnicode_Equals(s, PyTuple_GET_ITEM(kwnames, i), Py_EQ);
+        if (unlikely(eq != 0)) {
+            if (unlikely(eq < 0)) return NULL;  // error
+            return kwvalues[i];
+        }
+    }
+    return NULL;  // not found (no exception set)
+}
+#endif
+
 /* RaiseArgTupleInvalid */
 static void __Pyx_RaiseArgtupleInvalid(
     const char* func_name,
     int exact,
     Py_ssize_t num_min,
     Py_ssize_t num_max,
     Py_ssize_t num_found)
@@ -3242,25 +5185,37 @@
         PyString_AsString(kw_name));
         #endif
 }
 
 /* ParseKeywords */
 static int __Pyx_ParseOptionalKeywords(
     PyObject *kwds,
+    PyObject *const *kwvalues,
     PyObject **argnames[],
     PyObject *kwds2,
     PyObject *values[],
     Py_ssize_t num_pos_args,
     const char* function_name)
 {
     PyObject *key = 0, *value = 0;
     Py_ssize_t pos = 0;
     PyObject*** name;
     PyObject*** first_kw_arg = argnames + num_pos_args;
-    while (PyDict_Next(kwds, &pos, &key, &value)) {
+    int kwds_is_tuple = CYTHON_METH_FASTCALL && likely(PyTuple_Check(kwds));
+    while (1) {
+        if (kwds_is_tuple) {
+            if (pos >= PyTuple_GET_SIZE(kwds)) break;
+            key = PyTuple_GET_ITEM(kwds, pos);
+            value = kwvalues[pos];
+            pos++;
+        }
+        else
+        {
+            if (!PyDict_Next(kwds, &pos, &key, &value)) break;
+        }
         name = first_kw_arg;
         while (*name && (**name != key)) name++;
         if (*name) {
             values[name-argnames] = value;
             continue;
         }
         name = first_kw_arg;
@@ -3286,19 +5241,20 @@
                     argname++;
                 }
             }
         } else
         #endif
         if (likely(PyUnicode_Check(key))) {
             while (*name) {
-                int cmp = (**name == key) ? 0 :
+                int cmp = (
                 #if !CYTHON_COMPILING_IN_PYPY && PY_MAJOR_VERSION >= 3
                     (__Pyx_PyUnicode_GET_LENGTH(**name) != __Pyx_PyUnicode_GET_LENGTH(key)) ? 1 :
                 #endif
-                    PyUnicode_Compare(**name, key);
+                    PyUnicode_Compare(**name, key)
+                );
                 if (cmp < 0 && unlikely(PyErr_Occurred())) goto bad;
                 if (cmp == 0) {
                     values[name-argnames] = value;
                     break;
                 }
                 name++;
             }
@@ -3329,54 +5285,27 @@
     __Pyx_RaiseDoubleKeywordsError(function_name, key);
     goto bad;
 invalid_keyword_type:
     PyErr_Format(PyExc_TypeError,
         "%.200s() keywords must be strings", function_name);
     goto bad;
 invalid_keyword:
-    PyErr_Format(PyExc_TypeError,
     #if PY_MAJOR_VERSION < 3
+    PyErr_Format(PyExc_TypeError,
         "%.200s() got an unexpected keyword argument '%.200s'",
         function_name, PyString_AsString(key));
     #else
+    PyErr_Format(PyExc_TypeError,
         "%s() got an unexpected keyword argument '%U'",
         function_name, key);
     #endif
 bad:
     return -1;
 }
 
-/* PyObjectGetAttrStr */
-#if CYTHON_USE_TYPE_SLOTS
-static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStr(PyObject* obj, PyObject* attr_name) {
-    PyTypeObject* tp = Py_TYPE(obj);
-    if (likely(tp->tp_getattro))
-        return tp->tp_getattro(obj, attr_name);
-#if PY_MAJOR_VERSION < 3
-    if (likely(tp->tp_getattr))
-        return tp->tp_getattr(obj, PyString_AS_STRING(attr_name));
-#endif
-    return PyObject_GetAttr(obj, attr_name);
-}
-#endif
-
-/* GetBuiltinName */
-static PyObject *__Pyx_GetBuiltinName(PyObject *name) {
-    PyObject* result = __Pyx_PyObject_GetAttrStr(__pyx_b, name);
-    if (unlikely(!result)) {
-        PyErr_Format(PyExc_NameError,
-#if PY_MAJOR_VERSION >= 3
-            "name '%U' is not defined", name);
-#else
-            "name '%.200s' is not defined", PyString_AS_STRING(name));
-#endif
-    }
-    return result;
-}
-
 /* PyDictVersioning */
 #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_TYPE_SLOTS
 static CYTHON_INLINE PY_UINT64_T __Pyx_get_tp_dict_version(PyObject *obj) {
     PyObject *dict = Py_TYPE(obj)->tp_dict;
     return likely(dict) ? __PYX_GET_DICT_VERSION(dict) : 0;
 }
 static CYTHON_INLINE PY_UINT64_T __Pyx_get_object_dict_version(PyObject *obj) {
@@ -3412,14 +5341,22 @@
     result = _PyDict_GetItem_KnownHash(__pyx_d, name, ((PyASCIIObject *) name)->hash);
     __PYX_UPDATE_DICT_CACHE(__pyx_d, result, *dict_cached_value, *dict_version)
     if (likely(result)) {
         return __Pyx_NewRef(result);
     } else if (unlikely(PyErr_Occurred())) {
         return NULL;
     }
+#elif CYTHON_COMPILING_IN_LIMITED_API
+    if (unlikely(!__pyx_m)) {
+        return NULL;
+    }
+    result = PyObject_GetAttr(__pyx_m, name);
+    if (likely(result)) {
+        return result;
+    }
 #else
     result = PyDict_GetItem(__pyx_d, name);
     __PYX_UPDATE_DICT_CACHE(__pyx_d, result, *dict_cached_value, *dict_version)
     if (likely(result)) {
         return __Pyx_NewRef(result);
     }
 #endif
@@ -3430,39 +5367,16 @@
         return __Pyx_NewRef(result);
     }
     PyErr_Clear();
 #endif
     return __Pyx_GetBuiltinName(name);
 }
 
-/* PyCFunctionFastCall */
-#if CYTHON_FAST_PYCCALL
-static CYTHON_INLINE PyObject * __Pyx_PyCFunction_FastCall(PyObject *func_obj, PyObject **args, Py_ssize_t nargs) {
-    PyCFunctionObject *func = (PyCFunctionObject*)func_obj;
-    PyCFunction meth = PyCFunction_GET_FUNCTION(func);
-    PyObject *self = PyCFunction_GET_SELF(func);
-    int flags = PyCFunction_GET_FLAGS(func);
-    assert(PyCFunction_Check(func));
-    assert(METH_FASTCALL == (flags & ~(METH_CLASS | METH_STATIC | METH_COEXIST | METH_KEYWORDS | METH_STACKLESS)));
-    assert(nargs >= 0);
-    assert(nargs == 0 || args != NULL);
-    /* _PyCFunction_FastCallDict() must not be called with an exception set,
-       because it may clear it (directly or indirectly) and so the
-       caller loses its exception */
-    assert(!PyErr_Occurred());
-    if ((PY_VERSION_HEX < 0x030700A0) || unlikely(flags & METH_KEYWORDS)) {
-        return (*((__Pyx_PyCFunctionFastWithKeywords)(void*)meth)) (self, args, nargs, NULL);
-    } else {
-        return (*((__Pyx_PyCFunctionFast)(void*)meth)) (self, args, nargs);
-    }
-}
-#endif
-
 /* PyFunctionFastCall */
-#if CYTHON_FAST_PYCALL
+#if CYTHON_FAST_PYCALL && !CYTHON_VECTORCALL
 static PyObject* __Pyx_PyFunction_FastCallNoKw(PyCodeObject *co, PyObject **args, Py_ssize_t na,
                                                PyObject *globals) {
     PyFrameObject *f;
     PyThreadState *tstate = __Pyx_PyThreadState_Current;
     PyObject **fastlocals;
     Py_ssize_t i;
     PyObject *result;
@@ -3483,15 +5397,14 @@
     }
     result = PyEval_EvalFrameEx(f,0);
     ++tstate->recursion_depth;
     Py_DECREF(f);
     --tstate->recursion_depth;
     return result;
 }
-#if 1 || PY_VERSION_HEX < 0x030600B1
 static PyObject *__Pyx_PyFunction_FastCallDict(PyObject *func, PyObject **args, Py_ssize_t nargs, PyObject *kwargs) {
     PyCodeObject *co = (PyCodeObject *)PyFunction_GET_CODE(func);
     PyObject *globals = PyFunction_GET_GLOBALS(func);
     PyObject *argdefs = PyFunction_GET_DEFAULTS(func);
     PyObject *closure;
 #if PY_MAJOR_VERSION >= 3
     PyObject *kwdefs;
@@ -3499,15 +5412,15 @@
     PyObject *kwtuple, **k;
     PyObject **d;
     Py_ssize_t nd;
     Py_ssize_t nk;
     PyObject *result;
     assert(kwargs == NULL || PyDict_Check(kwargs));
     nk = kwargs ? PyDict_Size(kwargs) : 0;
-    if (Py_EnterRecursiveCall((char*)" while calling a Python object")) {
+    if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object"))) {
         return NULL;
     }
     if (
 #if PY_MAJOR_VERSION >= 3
             co->co_kwonlyargcount == 0 &&
 #endif
             likely(kwargs == NULL || nk == 0) &&
@@ -3570,64 +5483,14 @@
 #endif
     Py_XDECREF(kwtuple);
 done:
     Py_LeaveRecursiveCall();
     return result;
 }
 #endif
-#endif
-
-/* PyObjectCall */
-#if CYTHON_COMPILING_IN_CPYTHON
-static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw) {
-    PyObject *result;
-    ternaryfunc call = Py_TYPE(func)->tp_call;
-    if (unlikely(!call))
-        return PyObject_Call(func, arg, kw);
-    if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object")))
-        return NULL;
-    result = (*call)(func, arg, kw);
-    Py_LeaveRecursiveCall();
-    if (unlikely(!result) && unlikely(!PyErr_Occurred())) {
-        PyErr_SetString(
-            PyExc_SystemError,
-            "NULL result without error in PyObject_Call");
-    }
-    return result;
-}
-#endif
-
-/* PyObjectCall2Args */
-static CYTHON_UNUSED PyObject* __Pyx_PyObject_Call2Args(PyObject* function, PyObject* arg1, PyObject* arg2) {
-    PyObject *args, *result = NULL;
-    #if CYTHON_FAST_PYCALL
-    if (PyFunction_Check(function)) {
-        PyObject *args[2] = {arg1, arg2};
-        return __Pyx_PyFunction_FastCall(function, args, 2);
-    }
-    #endif
-    #if CYTHON_FAST_PYCCALL
-    if (__Pyx_PyFastCFunction_Check(function)) {
-        PyObject *args[2] = {arg1, arg2};
-        return __Pyx_PyCFunction_FastCall(function, args, 2);
-    }
-    #endif
-    args = PyTuple_New(2);
-    if (unlikely(!args)) goto done;
-    Py_INCREF(arg1);
-    PyTuple_SET_ITEM(args, 0, arg1);
-    Py_INCREF(arg2);
-    PyTuple_SET_ITEM(args, 1, arg2);
-    Py_INCREF(function);
-    result = __Pyx_PyObject_Call(function, args, NULL);
-    Py_DECREF(args);
-    Py_DECREF(function);
-done:
-    return result;
-}
 
 /* PyObjectCallMethO */
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallMethO(PyObject *func, PyObject *arg) {
     PyObject *self, *result;
     PyCFunction cfunc;
     cfunc = PyCFunction_GET_FUNCTION(func);
@@ -3641,53 +5504,90 @@
             PyExc_SystemError,
             "NULL result without error in PyObject_Call");
     }
     return result;
 }
 #endif
 
-/* PyObjectCallOneArg */
-#if CYTHON_COMPILING_IN_CPYTHON
-static PyObject* __Pyx__PyObject_CallOneArg(PyObject *func, PyObject *arg) {
+/* PyObjectFastCall */
+static PyObject* __Pyx_PyObject_FastCall_fallback(PyObject *func, PyObject **args, size_t nargs, PyObject *kwargs) {
+    PyObject *argstuple;
     PyObject *result;
-    PyObject *args = PyTuple_New(1);
-    if (unlikely(!args)) return NULL;
-    Py_INCREF(arg);
-    PyTuple_SET_ITEM(args, 0, arg);
-    result = __Pyx_PyObject_Call(func, args, NULL);
-    Py_DECREF(args);
+    size_t i;
+    argstuple = PyTuple_New((Py_ssize_t)nargs);
+    if (unlikely(!argstuple)) return NULL;
+    for (i = 0; i < nargs; i++) {
+        Py_INCREF(args[i]);
+        PyTuple_SET_ITEM(argstuple, (Py_ssize_t)i, args[i]);
+    }
+    result = __Pyx_PyObject_Call(func, argstuple, kwargs);
+    Py_DECREF(argstuple);
     return result;
 }
-static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg) {
-#if CYTHON_FAST_PYCALL
-    if (PyFunction_Check(func)) {
-        return __Pyx_PyFunction_FastCall(func, &arg, 1);
-    }
+static CYTHON_INLINE PyObject* __Pyx_PyObject_FastCallDict(PyObject *func, PyObject **args, size_t _nargs, PyObject *kwargs) {
+    Py_ssize_t nargs = __Pyx_PyVectorcall_NARGS(_nargs);
+#if CYTHON_COMPILING_IN_CPYTHON
+    if (nargs == 0 && kwargs == NULL) {
+#if defined(__Pyx_CyFunction_USED) && defined(NDEBUG)
+        if (__Pyx_IsCyOrPyCFunction(func))
+#else
+        if (PyCFunction_Check(func))
 #endif
-    if (likely(PyCFunction_Check(func))) {
-        if (likely(PyCFunction_GET_FLAGS(func) & METH_O)) {
-            return __Pyx_PyObject_CallMethO(func, arg);
-#if CYTHON_FAST_PYCCALL
-        } else if (__Pyx_PyFastCFunction_Check(func)) {
-            return __Pyx_PyCFunction_FastCall(func, &arg, 1);
+        {
+            if (likely(PyCFunction_GET_FLAGS(func) & METH_NOARGS)) {
+                return __Pyx_PyObject_CallMethO(func, NULL);
+            }
+        }
+    }
+    else if (nargs == 1 && kwargs == NULL) {
+        if (PyCFunction_Check(func))
+        {
+            if (likely(PyCFunction_GET_FLAGS(func) & METH_O)) {
+                return __Pyx_PyObject_CallMethO(func, args[0]);
+            }
+        }
+    }
 #endif
+    #if PY_VERSION_HEX < 0x030800B1
+    #if CYTHON_FAST_PYCCALL
+    if (PyCFunction_Check(func)) {
+        if (kwargs) {
+            return _PyCFunction_FastCallDict(func, args, nargs, kwargs);
+        } else {
+            return _PyCFunction_FastCallKeywords(func, args, nargs, NULL);
         }
     }
-    return __Pyx__PyObject_CallOneArg(func, arg);
-}
-#else
-static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg) {
-    PyObject *result;
-    PyObject *args = PyTuple_Pack(1, arg);
-    if (unlikely(!args)) return NULL;
-    result = __Pyx_PyObject_Call(func, args, NULL);
-    Py_DECREF(args);
-    return result;
+    #if PY_VERSION_HEX >= 0x030700A1
+    if (!kwargs && __Pyx_IS_TYPE(func, &PyMethodDescr_Type)) {
+        return _PyMethodDescr_FastCallKeywords(func, args, nargs, NULL);
+    }
+    #endif
+    #endif
+    #if CYTHON_FAST_PYCALL
+    if (PyFunction_Check(func)) {
+        return __Pyx_PyFunction_FastCallDict(func, args, nargs, kwargs);
+    }
+    #endif
+    #endif
+    #if CYTHON_VECTORCALL
+    vectorcallfunc f = _PyVectorcall_Function(func);
+    if (f) {
+        return f(func, args, (size_t)nargs, kwargs);
+    }
+    #elif defined(__Pyx_CyFunction_USED) && CYTHON_BACKPORT_VECTORCALL
+    if (__Pyx_CyFunction_CheckExact(func)) {
+        __pyx_vectorcallfunc f = __Pyx_CyFunction_func_vectorcall(func);
+        if (f) return f(func, args, (size_t)nargs, kwargs);
+    }
+    #endif
+    if (nargs == 0) {
+        return __Pyx_PyObject_Call(func, __pyx_empty_tuple, kwargs);
+    }
+    return __Pyx_PyObject_FastCall_fallback(func, args, (size_t)nargs, kwargs);
 }
-#endif
 
 /* RaiseTooManyValuesToUnpack */
 static CYTHON_INLINE void __Pyx_RaiseTooManyValuesError(Py_ssize_t expected) {
     PyErr_Format(PyExc_ValueError,
                  "too many values to unpack (expected %" CYTHON_FORMAT_SSIZE_T "d)", expected);
 }
 
@@ -3696,530 +5596,1377 @@
     PyErr_Format(PyExc_ValueError,
                  "need more than %" CYTHON_FORMAT_SSIZE_T "d value%.1s to unpack",
                  index, (index == 1) ? "" : "s");
 }
 
 /* IterFinish */
 static CYTHON_INLINE int __Pyx_IterFinish(void) {
-#if CYTHON_FAST_THREAD_STATE
-    PyThreadState *tstate = __Pyx_PyThreadState_Current;
-    PyObject* exc_type = tstate->curexc_type;
+    __Pyx_PyThreadState_declare
+    __Pyx_PyThreadState_assign
+    PyObject* exc_type = __Pyx_PyErr_CurrentExceptionType();
     if (unlikely(exc_type)) {
-        if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) {
-            PyObject *exc_value, *exc_tb;
-            exc_value = tstate->curexc_value;
-            exc_tb = tstate->curexc_traceback;
-            tstate->curexc_type = 0;
-            tstate->curexc_value = 0;
-            tstate->curexc_traceback = 0;
-            Py_DECREF(exc_type);
-            Py_XDECREF(exc_value);
-            Py_XDECREF(exc_tb);
-            return 0;
-        } else {
-            return -1;
-        }
-    }
-    return 0;
-#else
-    if (unlikely(PyErr_Occurred())) {
-        if (likely(PyErr_ExceptionMatches(PyExc_StopIteration))) {
-            PyErr_Clear();
-            return 0;
-        } else {
+        if (unlikely(!__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration)))
             return -1;
-        }
+        __Pyx_PyErr_Clear();
+        return 0;
     }
     return 0;
-#endif
 }
 
 /* UnpackItemEndCheck */
 static int __Pyx_IternextUnpackEndCheck(PyObject *retval, Py_ssize_t expected) {
     if (unlikely(retval)) {
         Py_DECREF(retval);
         __Pyx_RaiseTooManyValuesError(expected);
         return -1;
-    } else {
-        return __Pyx_IterFinish();
     }
-    return 0;
+    return __Pyx_IterFinish();
 }
 
-/* PyObjectCallNoArg */
-#if CYTHON_COMPILING_IN_CPYTHON
-static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func) {
-#if CYTHON_FAST_PYCALL
-    if (PyFunction_Check(func)) {
-        return __Pyx_PyFunction_FastCall(func, NULL, 0);
+/* Import */
+static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level) {
+    PyObject *module = 0;
+    PyObject *empty_dict = 0;
+    PyObject *empty_list = 0;
+    #if PY_MAJOR_VERSION < 3
+    PyObject *py_import;
+    py_import = __Pyx_PyObject_GetAttrStr(__pyx_b, __pyx_n_s_import);
+    if (unlikely(!py_import))
+        goto bad;
+    if (!from_list) {
+        empty_list = PyList_New(0);
+        if (unlikely(!empty_list))
+            goto bad;
+        from_list = empty_list;
     }
+    #endif
+    empty_dict = PyDict_New();
+    if (unlikely(!empty_dict))
+        goto bad;
+    {
+        #if PY_MAJOR_VERSION >= 3
+        if (level == -1) {
+            if ((1) && (strchr(__Pyx_MODULE_NAME, '.'))) {
+                #if CYTHON_COMPILING_IN_LIMITED_API
+                module = PyImport_ImportModuleLevelObject(
+                    name, empty_dict, empty_dict, from_list, 1);
+                #else
+                module = PyImport_ImportModuleLevelObject(
+                    name, __pyx_d, empty_dict, from_list, 1);
+                #endif
+                if (unlikely(!module)) {
+                    if (unlikely(!PyErr_ExceptionMatches(PyExc_ImportError)))
+                        goto bad;
+                    PyErr_Clear();
+                }
+            }
+            level = 0;
+        }
+        #endif
+        if (!module) {
+            #if PY_MAJOR_VERSION < 3
+            PyObject *py_level = PyInt_FromLong(level);
+            if (unlikely(!py_level))
+                goto bad;
+            module = PyObject_CallFunctionObjArgs(py_import,
+                name, __pyx_d, empty_dict, from_list, py_level, (PyObject *)NULL);
+            Py_DECREF(py_level);
+            #else
+            #if CYTHON_COMPILING_IN_LIMITED_API
+            module = PyImport_ImportModuleLevelObject(
+                name, empty_dict, empty_dict, from_list, level);
+            #else
+            module = PyImport_ImportModuleLevelObject(
+                name, __pyx_d, empty_dict, from_list, level);
+            #endif
+            #endif
+        }
+    }
+bad:
+    Py_XDECREF(empty_dict);
+    Py_XDECREF(empty_list);
+    #if PY_MAJOR_VERSION < 3
+    Py_XDECREF(py_import);
+    #endif
+    return module;
+}
+
+/* ImportDottedModule */
+#if PY_MAJOR_VERSION >= 3
+static PyObject *__Pyx__ImportDottedModule_Error(PyObject *name, PyObject *parts_tuple, Py_ssize_t count) {
+    PyObject *partial_name = NULL, *slice = NULL, *sep = NULL;
+    if (unlikely(PyErr_Occurred())) {
+        PyErr_Clear();
+    }
+    if (likely(PyTuple_GET_SIZE(parts_tuple) == count)) {
+        partial_name = name;
+    } else {
+        slice = PySequence_GetSlice(parts_tuple, 0, count);
+        if (unlikely(!slice))
+            goto bad;
+        sep = PyUnicode_FromStringAndSize(".", 1);
+        if (unlikely(!sep))
+            goto bad;
+        partial_name = PyUnicode_Join(sep, slice);
+    }
+    PyErr_Format(
+#if PY_MAJOR_VERSION < 3
+        PyExc_ImportError,
+        "No module named '%s'", PyString_AS_STRING(partial_name));
+#else
+#if PY_VERSION_HEX >= 0x030600B1
+        PyExc_ModuleNotFoundError,
+#else
+        PyExc_ImportError,
 #endif
-#ifdef __Pyx_CyFunction_USED
-    if (likely(PyCFunction_Check(func) || __Pyx_CyFunction_Check(func)))
+        "No module named '%U'", partial_name);
+#endif
+bad:
+    Py_XDECREF(sep);
+    Py_XDECREF(slice);
+    Py_XDECREF(partial_name);
+    return NULL;
+}
+#endif
+#if PY_MAJOR_VERSION >= 3
+static PyObject *__Pyx__ImportDottedModule_Lookup(PyObject *name) {
+    PyObject *imported_module;
+#if PY_VERSION_HEX < 0x030700A1 || (CYTHON_COMPILING_IN_PYPY && PYPY_VERSION_NUM  < 0x07030400)
+    PyObject *modules = PyImport_GetModuleDict();
+    if (unlikely(!modules))
+        return NULL;
+    imported_module = __Pyx_PyDict_GetItemStr(modules, name);
+    Py_XINCREF(imported_module);
 #else
-    if (likely(PyCFunction_Check(func)))
+    imported_module = PyImport_GetModule(name);
 #endif
-    {
-        if (likely(PyCFunction_GET_FLAGS(func) & METH_NOARGS)) {
-            return __Pyx_PyObject_CallMethO(func, NULL);
-        }
+    return imported_module;
+}
+#endif
+#if PY_MAJOR_VERSION >= 3
+static PyObject *__Pyx_ImportDottedModule_WalkParts(PyObject *module, PyObject *name, PyObject *parts_tuple) {
+    Py_ssize_t i, nparts;
+    nparts = PyTuple_GET_SIZE(parts_tuple);
+    for (i=1; i < nparts && module; i++) {
+        PyObject *part, *submodule;
+#if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+        part = PyTuple_GET_ITEM(parts_tuple, i);
+#else
+        part = PySequence_ITEM(parts_tuple, i);
+#endif
+        submodule = __Pyx_PyObject_GetAttrStrNoError(module, part);
+#if !(CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS)
+        Py_DECREF(part);
+#endif
+        Py_DECREF(module);
+        module = submodule;
     }
-    return __Pyx_PyObject_Call(func, __pyx_empty_tuple, NULL);
+    if (unlikely(!module)) {
+        return __Pyx__ImportDottedModule_Error(name, parts_tuple, i);
+    }
+    return module;
 }
 #endif
-
-/* DictGetItem */
-#if PY_MAJOR_VERSION >= 3 && !CYTHON_COMPILING_IN_PYPY
-static PyObject *__Pyx_PyDict_GetItem(PyObject *d, PyObject* key) {
-    PyObject *value;
-    value = PyDict_GetItemWithError(d, key);
-    if (unlikely(!value)) {
-        if (!PyErr_Occurred()) {
-            if (unlikely(PyTuple_Check(key))) {
-                PyObject* args = PyTuple_Pack(1, key);
-                if (likely(args)) {
-                    PyErr_SetObject(PyExc_KeyError, args);
-                    Py_DECREF(args);
-                }
-            } else {
-                PyErr_SetObject(PyExc_KeyError, key);
-            }
-        }
+static PyObject *__Pyx__ImportDottedModule(PyObject *name, PyObject *parts_tuple) {
+#if PY_MAJOR_VERSION < 3
+    PyObject *module, *from_list, *star = __pyx_n_s__3;
+    CYTHON_UNUSED_VAR(parts_tuple);
+    from_list = PyList_New(1);
+    if (unlikely(!from_list))
         return NULL;
+    Py_INCREF(star);
+    PyList_SET_ITEM(from_list, 0, star);
+    module = __Pyx_Import(name, from_list, 0);
+    Py_DECREF(from_list);
+    return module;
+#else
+    PyObject *imported_module;
+    PyObject *module = __Pyx_Import(name, NULL, 0);
+    if (!parts_tuple || unlikely(!module))
+        return module;
+    imported_module = __Pyx__ImportDottedModule_Lookup(name);
+    if (likely(imported_module)) {
+        Py_DECREF(module);
+        return imported_module;
     }
-    Py_INCREF(value);
-    return value;
+    PyErr_Clear();
+    return __Pyx_ImportDottedModule_WalkParts(module, name, parts_tuple);
+#endif
 }
+static PyObject *__Pyx_ImportDottedModule(PyObject *name, PyObject *parts_tuple) {
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030400B1
+    PyObject *module = __Pyx__ImportDottedModule_Lookup(name);
+    if (likely(module)) {
+        PyObject *spec = __Pyx_PyObject_GetAttrStrNoError(module, __pyx_n_s_spec);
+        if (likely(spec)) {
+            PyObject *unsafe = __Pyx_PyObject_GetAttrStrNoError(spec, __pyx_n_s_initializing);
+            if (likely(!unsafe || !__Pyx_PyObject_IsTrue(unsafe))) {
+                Py_DECREF(spec);
+                spec = NULL;
+            }
+            Py_XDECREF(unsafe);
+        }
+        if (likely(!spec)) {
+            PyErr_Clear();
+            return module;
+        }
+        Py_DECREF(spec);
+        Py_DECREF(module);
+    } else if (PyErr_Occurred()) {
+        PyErr_Clear();
+    }
 #endif
+    return __Pyx__ImportDottedModule(name, parts_tuple);
+}
 
-/* GetTopmostException */
-#if CYTHON_USE_EXC_INFO_STACK
-static _PyErr_StackItem *
-__Pyx_PyErr_GetTopmostException(PyThreadState *tstate)
-{
-    _PyErr_StackItem *exc_info = tstate->exc_info;
-    while ((exc_info->exc_type == NULL || exc_info->exc_type == Py_None) &&
-           exc_info->previous_item != NULL)
-    {
-        exc_info = exc_info->previous_item;
+/* FixUpExtensionType */
+#if CYTHON_USE_TYPE_SPECS
+static int __Pyx_fix_up_extension_type_from_spec(PyType_Spec *spec, PyTypeObject *type) {
+#if PY_VERSION_HEX > 0x030900B1 || CYTHON_COMPILING_IN_LIMITED_API
+    CYTHON_UNUSED_VAR(spec);
+    CYTHON_UNUSED_VAR(type);
+#else
+    const PyType_Slot *slot = spec->slots;
+    while (slot && slot->slot && slot->slot != Py_tp_members)
+        slot++;
+    if (slot && slot->slot == Py_tp_members) {
+        int changed = 0;
+#if !(PY_VERSION_HEX <= 0x030900b1 && CYTHON_COMPILING_IN_CPYTHON)
+        const
+#endif
+            PyMemberDef *memb = (PyMemberDef*) slot->pfunc;
+        while (memb && memb->name) {
+            if (memb->name[0] == '_' && memb->name[1] == '_') {
+#if PY_VERSION_HEX < 0x030900b1
+                if (strcmp(memb->name, "__weaklistoffset__") == 0) {
+                    assert(memb->type == T_PYSSIZET);
+                    assert(memb->flags == READONLY);
+                    type->tp_weaklistoffset = memb->offset;
+                    changed = 1;
+                }
+                else if (strcmp(memb->name, "__dictoffset__") == 0) {
+                    assert(memb->type == T_PYSSIZET);
+                    assert(memb->flags == READONLY);
+                    type->tp_dictoffset = memb->offset;
+                    changed = 1;
+                }
+#if CYTHON_METH_FASTCALL
+                else if (strcmp(memb->name, "__vectorcalloffset__") == 0) {
+                    assert(memb->type == T_PYSSIZET);
+                    assert(memb->flags == READONLY);
+#if PY_VERSION_HEX >= 0x030800b4
+                    type->tp_vectorcall_offset = memb->offset;
+#else
+                    type->tp_print = (printfunc) memb->offset;
+#endif
+                    changed = 1;
+                }
+#endif
+#else
+                if ((0));
+#endif
+#if PY_VERSION_HEX <= 0x030900b1 && CYTHON_COMPILING_IN_CPYTHON
+                else if (strcmp(memb->name, "__module__") == 0) {
+                    PyObject *descr;
+                    assert(memb->type == T_OBJECT);
+                    assert(memb->flags == 0 || memb->flags == READONLY);
+                    descr = PyDescr_NewMember(type, memb);
+                    if (unlikely(!descr))
+                        return -1;
+                    if (unlikely(PyDict_SetItem(type->tp_dict, PyDescr_NAME(descr), descr) < 0)) {
+                        Py_DECREF(descr);
+                        return -1;
+                    }
+                    Py_DECREF(descr);
+                    changed = 1;
+                }
+#endif
+            }
+            memb++;
+        }
+        if (changed)
+            PyType_Modified(type);
     }
-    return exc_info;
+#endif
+    return 0;
 }
 #endif
 
-/* SaveResetException */
-#if CYTHON_FAST_THREAD_STATE
-static CYTHON_INLINE void __Pyx__ExceptionSave(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb) {
-    #if CYTHON_USE_EXC_INFO_STACK
-    _PyErr_StackItem *exc_info = __Pyx_PyErr_GetTopmostException(tstate);
-    *type = exc_info->exc_type;
-    *value = exc_info->exc_value;
-    *tb = exc_info->exc_traceback;
-    #else
-    *type = tstate->exc_type;
-    *value = tstate->exc_value;
-    *tb = tstate->exc_traceback;
-    #endif
-    Py_XINCREF(*type);
-    Py_XINCREF(*value);
-    Py_XINCREF(*tb);
+/* FetchSharedCythonModule */
+static PyObject *__Pyx_FetchSharedCythonABIModule(void) {
+    PyObject *abi_module = PyImport_AddModule((char*) __PYX_ABI_MODULE_NAME);
+    if (unlikely(!abi_module)) return NULL;
+    Py_INCREF(abi_module);
+    return abi_module;
+}
+
+/* FetchCommonType */
+static int __Pyx_VerifyCachedType(PyObject *cached_type,
+                               const char *name,
+                               Py_ssize_t basicsize,
+                               Py_ssize_t expected_basicsize) {
+    if (!PyType_Check(cached_type)) {
+        PyErr_Format(PyExc_TypeError,
+            "Shared Cython type %.200s is not a type object", name);
+        return -1;
+    }
+    if (basicsize != expected_basicsize) {
+        PyErr_Format(PyExc_TypeError,
+            "Shared Cython type %.200s has the wrong size, try recompiling",
+            name);
+        return -1;
+    }
+    return 0;
 }
-static CYTHON_INLINE void __Pyx__ExceptionReset(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb) {
-    PyObject *tmp_type, *tmp_value, *tmp_tb;
-    #if CYTHON_USE_EXC_INFO_STACK
-    _PyErr_StackItem *exc_info = tstate->exc_info;
-    tmp_type = exc_info->exc_type;
-    tmp_value = exc_info->exc_value;
-    tmp_tb = exc_info->exc_traceback;
-    exc_info->exc_type = type;
-    exc_info->exc_value = value;
-    exc_info->exc_traceback = tb;
-    #else
-    tmp_type = tstate->exc_type;
-    tmp_value = tstate->exc_value;
-    tmp_tb = tstate->exc_traceback;
-    tstate->exc_type = type;
-    tstate->exc_value = value;
-    tstate->exc_traceback = tb;
-    #endif
-    Py_XDECREF(tmp_type);
-    Py_XDECREF(tmp_value);
-    Py_XDECREF(tmp_tb);
+#if !CYTHON_USE_TYPE_SPECS
+static PyTypeObject* __Pyx_FetchCommonType(PyTypeObject* type) {
+    PyObject* abi_module;
+    const char* object_name;
+    PyTypeObject *cached_type = NULL;
+    abi_module = __Pyx_FetchSharedCythonABIModule();
+    if (!abi_module) return NULL;
+    object_name = strrchr(type->tp_name, '.');
+    object_name = object_name ? object_name+1 : type->tp_name;
+    cached_type = (PyTypeObject*) PyObject_GetAttrString(abi_module, object_name);
+    if (cached_type) {
+        if (__Pyx_VerifyCachedType(
+              (PyObject *)cached_type,
+              object_name,
+              cached_type->tp_basicsize,
+              type->tp_basicsize) < 0) {
+            goto bad;
+        }
+        goto done;
+    }
+    if (!PyErr_ExceptionMatches(PyExc_AttributeError)) goto bad;
+    PyErr_Clear();
+    if (PyType_Ready(type) < 0) goto bad;
+    if (PyObject_SetAttrString(abi_module, object_name, (PyObject *)type) < 0)
+        goto bad;
+    Py_INCREF(type);
+    cached_type = type;
+done:
+    Py_DECREF(abi_module);
+    return cached_type;
+bad:
+    Py_XDECREF(cached_type);
+    cached_type = NULL;
+    goto done;
+}
+#else
+static PyTypeObject *__Pyx_FetchCommonTypeFromSpec(PyObject *module, PyType_Spec *spec, PyObject *bases) {
+    PyObject *abi_module, *cached_type = NULL;
+    const char* object_name = strrchr(spec->name, '.');
+    object_name = object_name ? object_name+1 : spec->name;
+    abi_module = __Pyx_FetchSharedCythonABIModule();
+    if (!abi_module) return NULL;
+    cached_type = PyObject_GetAttrString(abi_module, object_name);
+    if (cached_type) {
+        Py_ssize_t basicsize;
+#if CYTHON_COMPILING_IN_LIMITED_API
+        PyObject *py_basicsize;
+        py_basicsize = PyObject_GetAttrString(cached_type, "__basicsize__");
+        if (unlikely(!py_basicsize)) goto bad;
+        basicsize = PyLong_AsSsize_t(py_basicsize);
+        Py_DECREF(py_basicsize);
+        py_basicsize = 0;
+        if (unlikely(basicsize == (Py_ssize_t)-1) && PyErr_Occurred()) goto bad;
+#else
+        basicsize = likely(PyType_Check(cached_type)) ? ((PyTypeObject*) cached_type)->tp_basicsize : -1;
+#endif
+        if (__Pyx_VerifyCachedType(
+              cached_type,
+              object_name,
+              basicsize,
+              spec->basicsize) < 0) {
+            goto bad;
+        }
+        goto done;
+    }
+    if (!PyErr_ExceptionMatches(PyExc_AttributeError)) goto bad;
+    PyErr_Clear();
+    CYTHON_UNUSED_VAR(module);
+    cached_type = __Pyx_PyType_FromModuleAndSpec(abi_module, spec, bases);
+    if (unlikely(!cached_type)) goto bad;
+    if (unlikely(__Pyx_fix_up_extension_type_from_spec(spec, (PyTypeObject *) cached_type) < 0)) goto bad;
+    if (PyObject_SetAttrString(abi_module, object_name, cached_type) < 0) goto bad;
+done:
+    Py_DECREF(abi_module);
+    assert(cached_type == NULL || PyType_Check(cached_type));
+    return (PyTypeObject *) cached_type;
+bad:
+    Py_XDECREF(cached_type);
+    cached_type = NULL;
+    goto done;
 }
 #endif
 
-/* PyErrExceptionMatches */
-#if CYTHON_FAST_THREAD_STATE
-static int __Pyx_PyErr_ExceptionMatchesTuple(PyObject *exc_type, PyObject *tuple) {
-    Py_ssize_t i, n;
-    n = PyTuple_GET_SIZE(tuple);
-#if PY_MAJOR_VERSION >= 3
-    for (i=0; i<n; i++) {
-        if (exc_type == PyTuple_GET_ITEM(tuple, i)) return 1;
+/* PyVectorcallFastCallDict */
+#if CYTHON_METH_FASTCALL
+static PyObject *__Pyx_PyVectorcall_FastCallDict_kw(PyObject *func, __pyx_vectorcallfunc vc, PyObject *const *args, size_t nargs, PyObject *kw)
+{
+    PyObject *res = NULL;
+    PyObject *kwnames;
+    PyObject **newargs;
+    PyObject **kwvalues;
+    Py_ssize_t i, pos;
+    size_t j;
+    PyObject *key, *value;
+    unsigned long keys_are_strings;
+    Py_ssize_t nkw = PyDict_GET_SIZE(kw);
+    newargs = (PyObject **)PyMem_Malloc((nargs + (size_t)nkw) * sizeof(args[0]));
+    if (unlikely(newargs == NULL)) {
+        PyErr_NoMemory();
+        return NULL;
     }
-#endif
-    for (i=0; i<n; i++) {
-        if (__Pyx_PyErr_GivenExceptionMatches(exc_type, PyTuple_GET_ITEM(tuple, i))) return 1;
+    for (j = 0; j < nargs; j++) newargs[j] = args[j];
+    kwnames = PyTuple_New(nkw);
+    if (unlikely(kwnames == NULL)) {
+        PyMem_Free(newargs);
+        return NULL;
     }
-    return 0;
+    kwvalues = newargs + nargs;
+    pos = i = 0;
+    keys_are_strings = Py_TPFLAGS_UNICODE_SUBCLASS;
+    while (PyDict_Next(kw, &pos, &key, &value)) {
+        keys_are_strings &= Py_TYPE(key)->tp_flags;
+        Py_INCREF(key);
+        Py_INCREF(value);
+        PyTuple_SET_ITEM(kwnames, i, key);
+        kwvalues[i] = value;
+        i++;
+    }
+    if (unlikely(!keys_are_strings)) {
+        PyErr_SetString(PyExc_TypeError, "keywords must be strings");
+        goto cleanup;
+    }
+    res = vc(func, newargs, nargs, kwnames);
+cleanup:
+    Py_DECREF(kwnames);
+    for (i = 0; i < nkw; i++)
+        Py_DECREF(kwvalues[i]);
+    PyMem_Free(newargs);
+    return res;
 }
-static CYTHON_INLINE int __Pyx_PyErr_ExceptionMatchesInState(PyThreadState* tstate, PyObject* err) {
-    PyObject *exc_type = tstate->curexc_type;
-    if (exc_type == err) return 1;
-    if (unlikely(!exc_type)) return 0;
-    if (unlikely(PyTuple_Check(err)))
-        return __Pyx_PyErr_ExceptionMatchesTuple(exc_type, err);
-    return __Pyx_PyErr_GivenExceptionMatches(exc_type, err);
+static CYTHON_INLINE PyObject *__Pyx_PyVectorcall_FastCallDict(PyObject *func, __pyx_vectorcallfunc vc, PyObject *const *args, size_t nargs, PyObject *kw)
+{
+    if (likely(kw == NULL) || PyDict_GET_SIZE(kw) == 0) {
+        return vc(func, args, nargs, NULL);
+    }
+    return __Pyx_PyVectorcall_FastCallDict_kw(func, vc, args, nargs, kw);
 }
 #endif
 
-/* GetException */
-#if CYTHON_FAST_THREAD_STATE
-static int __Pyx__GetException(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb)
+/* CythonFunctionShared */
+static CYTHON_INLINE void __Pyx__CyFunction_SetClassObj(__pyx_CyFunctionObject* f, PyObject* classobj) {
+#if PY_VERSION_HEX < 0x030900B1
+    __Pyx_Py_XDECREF_SET(
+        __Pyx_CyFunction_GetClassObj(f),
+            ((classobj) ? __Pyx_NewRef(classobj) : NULL));
 #else
-static int __Pyx_GetException(PyObject **type, PyObject **value, PyObject **tb)
+    __Pyx_Py_XDECREF_SET(
+        ((PyCMethodObject *) (f))->mm_class,
+        (PyTypeObject*)((classobj) ? __Pyx_NewRef(classobj) : NULL));
 #endif
+}
+static PyObject *
+__Pyx_CyFunction_get_doc(__pyx_CyFunctionObject *op, void *closure)
 {
-    PyObject *local_type, *local_value, *local_tb;
-#if CYTHON_FAST_THREAD_STATE
-    PyObject *tmp_type, *tmp_value, *tmp_tb;
-    local_type = tstate->curexc_type;
-    local_value = tstate->curexc_value;
-    local_tb = tstate->curexc_traceback;
-    tstate->curexc_type = 0;
-    tstate->curexc_value = 0;
-    tstate->curexc_traceback = 0;
+    CYTHON_UNUSED_VAR(closure);
+    if (unlikely(op->func_doc == NULL)) {
+        if (((PyCFunctionObject*)op)->m_ml->ml_doc) {
+#if PY_MAJOR_VERSION >= 3
+            op->func_doc = PyUnicode_FromString(((PyCFunctionObject*)op)->m_ml->ml_doc);
 #else
-    PyErr_Fetch(&local_type, &local_value, &local_tb);
+            op->func_doc = PyString_FromString(((PyCFunctionObject*)op)->m_ml->ml_doc);
 #endif
-    PyErr_NormalizeException(&local_type, &local_value, &local_tb);
-#if CYTHON_FAST_THREAD_STATE
-    if (unlikely(tstate->curexc_type))
+            if (unlikely(op->func_doc == NULL))
+                return NULL;
+        } else {
+            Py_INCREF(Py_None);
+            return Py_None;
+        }
+    }
+    Py_INCREF(op->func_doc);
+    return op->func_doc;
+}
+static int
+__Pyx_CyFunction_set_doc(__pyx_CyFunctionObject *op, PyObject *value, void *context)
+{
+    CYTHON_UNUSED_VAR(context);
+    if (value == NULL) {
+        value = Py_None;
+    }
+    Py_INCREF(value);
+    __Pyx_Py_XDECREF_SET(op->func_doc, value);
+    return 0;
+}
+static PyObject *
+__Pyx_CyFunction_get_name(__pyx_CyFunctionObject *op, void *context)
+{
+    CYTHON_UNUSED_VAR(context);
+    if (unlikely(op->func_name == NULL)) {
+#if PY_MAJOR_VERSION >= 3
+        op->func_name = PyUnicode_InternFromString(((PyCFunctionObject*)op)->m_ml->ml_name);
 #else
-    if (unlikely(PyErr_Occurred()))
+        op->func_name = PyString_InternFromString(((PyCFunctionObject*)op)->m_ml->ml_name);
 #endif
-        goto bad;
-    #if PY_MAJOR_VERSION >= 3
-    if (local_tb) {
-        if (unlikely(PyException_SetTraceback(local_value, local_tb) < 0))
-            goto bad;
+        if (unlikely(op->func_name == NULL))
+            return NULL;
     }
-    #endif
-    Py_XINCREF(local_tb);
-    Py_XINCREF(local_type);
-    Py_XINCREF(local_value);
-    *type = local_type;
-    *value = local_value;
-    *tb = local_tb;
-#if CYTHON_FAST_THREAD_STATE
-    #if CYTHON_USE_EXC_INFO_STACK
+    Py_INCREF(op->func_name);
+    return op->func_name;
+}
+static int
+__Pyx_CyFunction_set_name(__pyx_CyFunctionObject *op, PyObject *value, void *context)
+{
+    CYTHON_UNUSED_VAR(context);
+#if PY_MAJOR_VERSION >= 3
+    if (unlikely(value == NULL || !PyUnicode_Check(value)))
+#else
+    if (unlikely(value == NULL || !PyString_Check(value)))
+#endif
     {
-        _PyErr_StackItem *exc_info = tstate->exc_info;
-        tmp_type = exc_info->exc_type;
-        tmp_value = exc_info->exc_value;
-        tmp_tb = exc_info->exc_traceback;
-        exc_info->exc_type = local_type;
-        exc_info->exc_value = local_value;
-        exc_info->exc_traceback = local_tb;
+        PyErr_SetString(PyExc_TypeError,
+                        "__name__ must be set to a string object");
+        return -1;
     }
-    #else
-    tmp_type = tstate->exc_type;
-    tmp_value = tstate->exc_value;
-    tmp_tb = tstate->exc_traceback;
-    tstate->exc_type = local_type;
-    tstate->exc_value = local_value;
-    tstate->exc_traceback = local_tb;
-    #endif
-    Py_XDECREF(tmp_type);
-    Py_XDECREF(tmp_value);
-    Py_XDECREF(tmp_tb);
+    Py_INCREF(value);
+    __Pyx_Py_XDECREF_SET(op->func_name, value);
+    return 0;
+}
+static PyObject *
+__Pyx_CyFunction_get_qualname(__pyx_CyFunctionObject *op, void *context)
+{
+    CYTHON_UNUSED_VAR(context);
+    Py_INCREF(op->func_qualname);
+    return op->func_qualname;
+}
+static int
+__Pyx_CyFunction_set_qualname(__pyx_CyFunctionObject *op, PyObject *value, void *context)
+{
+    CYTHON_UNUSED_VAR(context);
+#if PY_MAJOR_VERSION >= 3
+    if (unlikely(value == NULL || !PyUnicode_Check(value)))
 #else
-    PyErr_SetExcInfo(local_type, local_value, local_tb);
+    if (unlikely(value == NULL || !PyString_Check(value)))
 #endif
+    {
+        PyErr_SetString(PyExc_TypeError,
+                        "__qualname__ must be set to a string object");
+        return -1;
+    }
+    Py_INCREF(value);
+    __Pyx_Py_XDECREF_SET(op->func_qualname, value);
     return 0;
-bad:
-    *type = 0;
-    *value = 0;
-    *tb = 0;
-    Py_XDECREF(local_type);
-    Py_XDECREF(local_value);
-    Py_XDECREF(local_tb);
-    return -1;
 }
-
-/* PyErrFetchRestore */
-#if CYTHON_FAST_THREAD_STATE
-static CYTHON_INLINE void __Pyx_ErrRestoreInState(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb) {
-    PyObject *tmp_type, *tmp_value, *tmp_tb;
-    tmp_type = tstate->curexc_type;
-    tmp_value = tstate->curexc_value;
-    tmp_tb = tstate->curexc_traceback;
-    tstate->curexc_type = type;
-    tstate->curexc_value = value;
-    tstate->curexc_traceback = tb;
-    Py_XDECREF(tmp_type);
-    Py_XDECREF(tmp_value);
-    Py_XDECREF(tmp_tb);
+static PyObject *
+__Pyx_CyFunction_get_dict(__pyx_CyFunctionObject *op, void *context)
+{
+    CYTHON_UNUSED_VAR(context);
+    if (unlikely(op->func_dict == NULL)) {
+        op->func_dict = PyDict_New();
+        if (unlikely(op->func_dict == NULL))
+            return NULL;
+    }
+    Py_INCREF(op->func_dict);
+    return op->func_dict;
 }
-static CYTHON_INLINE void __Pyx_ErrFetchInState(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb) {
-    *type = tstate->curexc_type;
-    *value = tstate->curexc_value;
-    *tb = tstate->curexc_traceback;
-    tstate->curexc_type = 0;
-    tstate->curexc_value = 0;
-    tstate->curexc_traceback = 0;
+static int
+__Pyx_CyFunction_set_dict(__pyx_CyFunctionObject *op, PyObject *value, void *context)
+{
+    CYTHON_UNUSED_VAR(context);
+    if (unlikely(value == NULL)) {
+        PyErr_SetString(PyExc_TypeError,
+               "function's dictionary may not be deleted");
+        return -1;
+    }
+    if (unlikely(!PyDict_Check(value))) {
+        PyErr_SetString(PyExc_TypeError,
+               "setting function's dictionary to a non-dict");
+        return -1;
+    }
+    Py_INCREF(value);
+    __Pyx_Py_XDECREF_SET(op->func_dict, value);
+    return 0;
 }
-#endif
-
-/* RaiseException */
-#if PY_MAJOR_VERSION < 3
-static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb,
-                        CYTHON_UNUSED PyObject *cause) {
-    __Pyx_PyThreadState_declare
-    Py_XINCREF(type);
-    if (!value || value == Py_None)
-        value = NULL;
-    else
-        Py_INCREF(value);
-    if (!tb || tb == Py_None)
-        tb = NULL;
+static PyObject *
+__Pyx_CyFunction_get_globals(__pyx_CyFunctionObject *op, void *context)
+{
+    CYTHON_UNUSED_VAR(context);
+    Py_INCREF(op->func_globals);
+    return op->func_globals;
+}
+static PyObject *
+__Pyx_CyFunction_get_closure(__pyx_CyFunctionObject *op, void *context)
+{
+    CYTHON_UNUSED_VAR(op);
+    CYTHON_UNUSED_VAR(context);
+    Py_INCREF(Py_None);
+    return Py_None;
+}
+static PyObject *
+__Pyx_CyFunction_get_code(__pyx_CyFunctionObject *op, void *context)
+{
+    PyObject* result = (op->func_code) ? op->func_code : Py_None;
+    CYTHON_UNUSED_VAR(context);
+    Py_INCREF(result);
+    return result;
+}
+static int
+__Pyx_CyFunction_init_defaults(__pyx_CyFunctionObject *op) {
+    int result = 0;
+    PyObject *res = op->defaults_getter((PyObject *) op);
+    if (unlikely(!res))
+        return -1;
+    #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+    op->defaults_tuple = PyTuple_GET_ITEM(res, 0);
+    Py_INCREF(op->defaults_tuple);
+    op->defaults_kwdict = PyTuple_GET_ITEM(res, 1);
+    Py_INCREF(op->defaults_kwdict);
+    #else
+    op->defaults_tuple = PySequence_ITEM(res, 0);
+    if (unlikely(!op->defaults_tuple)) result = -1;
     else {
-        Py_INCREF(tb);
-        if (!PyTraceBack_Check(tb)) {
-            PyErr_SetString(PyExc_TypeError,
-                "raise: arg 3 must be a traceback or None");
-            goto raise_error;
-        }
+        op->defaults_kwdict = PySequence_ITEM(res, 1);
+        if (unlikely(!op->defaults_kwdict)) result = -1;
     }
-    if (PyType_Check(type)) {
-#if CYTHON_COMPILING_IN_PYPY
-        if (!value) {
-            Py_INCREF(Py_None);
-            value = Py_None;
-        }
-#endif
-        PyErr_NormalizeException(&type, &value, &tb);
-    } else {
-        if (value) {
-            PyErr_SetString(PyExc_TypeError,
-                "instance exception may not have a separate value");
-            goto raise_error;
-        }
-        value = type;
-        type = (PyObject*) Py_TYPE(type);
-        Py_INCREF(type);
-        if (!PyType_IsSubtype((PyTypeObject *)type, (PyTypeObject *)PyExc_BaseException)) {
-            PyErr_SetString(PyExc_TypeError,
-                "raise: exception class must be a subclass of BaseException");
-            goto raise_error;
+    #endif
+    Py_DECREF(res);
+    return result;
+}
+static int
+__Pyx_CyFunction_set_defaults(__pyx_CyFunctionObject *op, PyObject* value, void *context) {
+    CYTHON_UNUSED_VAR(context);
+    if (!value) {
+        value = Py_None;
+    } else if (unlikely(value != Py_None && !PyTuple_Check(value))) {
+        PyErr_SetString(PyExc_TypeError,
+                        "__defaults__ must be set to a tuple object");
+        return -1;
+    }
+    PyErr_WarnEx(PyExc_RuntimeWarning, "changes to cyfunction.__defaults__ will not "
+                 "currently affect the values used in function calls", 1);
+    Py_INCREF(value);
+    __Pyx_Py_XDECREF_SET(op->defaults_tuple, value);
+    return 0;
+}
+static PyObject *
+__Pyx_CyFunction_get_defaults(__pyx_CyFunctionObject *op, void *context) {
+    PyObject* result = op->defaults_tuple;
+    CYTHON_UNUSED_VAR(context);
+    if (unlikely(!result)) {
+        if (op->defaults_getter) {
+            if (unlikely(__Pyx_CyFunction_init_defaults(op) < 0)) return NULL;
+            result = op->defaults_tuple;
+        } else {
+            result = Py_None;
         }
     }
-    __Pyx_PyThreadState_assign
-    __Pyx_ErrRestore(type, value, tb);
-    return;
-raise_error:
-    Py_XDECREF(value);
-    Py_XDECREF(type);
-    Py_XDECREF(tb);
-    return;
+    Py_INCREF(result);
+    return result;
 }
-#else
-static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause) {
-    PyObject* owned_instance = NULL;
-    if (tb == Py_None) {
-        tb = 0;
-    } else if (tb && !PyTraceBack_Check(tb)) {
+static int
+__Pyx_CyFunction_set_kwdefaults(__pyx_CyFunctionObject *op, PyObject* value, void *context) {
+    CYTHON_UNUSED_VAR(context);
+    if (!value) {
+        value = Py_None;
+    } else if (unlikely(value != Py_None && !PyDict_Check(value))) {
         PyErr_SetString(PyExc_TypeError,
-            "raise: arg 3 must be a traceback or None");
-        goto bad;
+                        "__kwdefaults__ must be set to a dict object");
+        return -1;
     }
-    if (value == Py_None)
-        value = 0;
-    if (PyExceptionInstance_Check(type)) {
-        if (value) {
-            PyErr_SetString(PyExc_TypeError,
-                "instance exception may not have a separate value");
-            goto bad;
-        }
-        value = type;
-        type = (PyObject*) Py_TYPE(value);
-    } else if (PyExceptionClass_Check(type)) {
-        PyObject *instance_class = NULL;
-        if (value && PyExceptionInstance_Check(value)) {
-            instance_class = (PyObject*) Py_TYPE(value);
-            if (instance_class != type) {
-                int is_subclass = PyObject_IsSubclass(instance_class, type);
-                if (!is_subclass) {
-                    instance_class = NULL;
-                } else if (unlikely(is_subclass == -1)) {
-                    goto bad;
-                } else {
-                    type = instance_class;
-                }
-            }
-        }
-        if (!instance_class) {
-            PyObject *args;
-            if (!value)
-                args = PyTuple_New(0);
-            else if (PyTuple_Check(value)) {
-                Py_INCREF(value);
-                args = value;
-            } else
-                args = PyTuple_Pack(1, value);
-            if (!args)
-                goto bad;
-            owned_instance = PyObject_Call(type, args, NULL);
-            Py_DECREF(args);
-            if (!owned_instance)
-                goto bad;
-            value = owned_instance;
-            if (!PyExceptionInstance_Check(value)) {
-                PyErr_Format(PyExc_TypeError,
-                             "calling %R should have returned an instance of "
-                             "BaseException, not %R",
-                             type, Py_TYPE(value));
-                goto bad;
-            }
+    PyErr_WarnEx(PyExc_RuntimeWarning, "changes to cyfunction.__kwdefaults__ will not "
+                 "currently affect the values used in function calls", 1);
+    Py_INCREF(value);
+    __Pyx_Py_XDECREF_SET(op->defaults_kwdict, value);
+    return 0;
+}
+static PyObject *
+__Pyx_CyFunction_get_kwdefaults(__pyx_CyFunctionObject *op, void *context) {
+    PyObject* result = op->defaults_kwdict;
+    CYTHON_UNUSED_VAR(context);
+    if (unlikely(!result)) {
+        if (op->defaults_getter) {
+            if (unlikely(__Pyx_CyFunction_init_defaults(op) < 0)) return NULL;
+            result = op->defaults_kwdict;
+        } else {
+            result = Py_None;
         }
-    } else {
+    }
+    Py_INCREF(result);
+    return result;
+}
+static int
+__Pyx_CyFunction_set_annotations(__pyx_CyFunctionObject *op, PyObject* value, void *context) {
+    CYTHON_UNUSED_VAR(context);
+    if (!value || value == Py_None) {
+        value = NULL;
+    } else if (unlikely(!PyDict_Check(value))) {
         PyErr_SetString(PyExc_TypeError,
-            "raise: exception class must be a subclass of BaseException");
-        goto bad;
+                        "__annotations__ must be set to a dict object");
+        return -1;
     }
-    if (cause) {
-        PyObject *fixed_cause;
-        if (cause == Py_None) {
-            fixed_cause = NULL;
-        } else if (PyExceptionClass_Check(cause)) {
-            fixed_cause = PyObject_CallObject(cause, NULL);
-            if (fixed_cause == NULL)
-                goto bad;
-        } else if (PyExceptionInstance_Check(cause)) {
-            fixed_cause = cause;
-            Py_INCREF(fixed_cause);
-        } else {
-            PyErr_SetString(PyExc_TypeError,
-                            "exception causes must derive from "
-                            "BaseException");
-            goto bad;
+    Py_XINCREF(value);
+    __Pyx_Py_XDECREF_SET(op->func_annotations, value);
+    return 0;
+}
+static PyObject *
+__Pyx_CyFunction_get_annotations(__pyx_CyFunctionObject *op, void *context) {
+    PyObject* result = op->func_annotations;
+    CYTHON_UNUSED_VAR(context);
+    if (unlikely(!result)) {
+        result = PyDict_New();
+        if (unlikely(!result)) return NULL;
+        op->func_annotations = result;
+    }
+    Py_INCREF(result);
+    return result;
+}
+static PyObject *
+__Pyx_CyFunction_get_is_coroutine(__pyx_CyFunctionObject *op, void *context) {
+    int is_coroutine;
+    CYTHON_UNUSED_VAR(context);
+    if (op->func_is_coroutine) {
+        return __Pyx_NewRef(op->func_is_coroutine);
+    }
+    is_coroutine = op->flags & __Pyx_CYFUNCTION_COROUTINE;
+#if PY_VERSION_HEX >= 0x03050000
+    if (is_coroutine) {
+        PyObject *module, *fromlist, *marker = __pyx_n_s_is_coroutine;
+        fromlist = PyList_New(1);
+        if (unlikely(!fromlist)) return NULL;
+        Py_INCREF(marker);
+        PyList_SET_ITEM(fromlist, 0, marker);
+        module = PyImport_ImportModuleLevelObject(__pyx_n_s_asyncio_coroutines, NULL, NULL, fromlist, 0);
+        Py_DECREF(fromlist);
+        if (unlikely(!module)) goto ignore;
+        op->func_is_coroutine = __Pyx_PyObject_GetAttrStr(module, marker);
+        Py_DECREF(module);
+        if (likely(op->func_is_coroutine)) {
+            return __Pyx_NewRef(op->func_is_coroutine);
         }
-        PyException_SetCause(value, fixed_cause);
+ignore:
+        PyErr_Clear();
     }
-    PyErr_SetObject(type, value);
-    if (tb) {
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
+#endif
+    op->func_is_coroutine = __Pyx_PyBool_FromLong(is_coroutine);
+    return __Pyx_NewRef(op->func_is_coroutine);
+}
+static PyGetSetDef __pyx_CyFunction_getsets[] = {
+    {(char *) "func_doc", (getter)__Pyx_CyFunction_get_doc, (setter)__Pyx_CyFunction_set_doc, 0, 0},
+    {(char *) "__doc__",  (getter)__Pyx_CyFunction_get_doc, (setter)__Pyx_CyFunction_set_doc, 0, 0},
+    {(char *) "func_name", (getter)__Pyx_CyFunction_get_name, (setter)__Pyx_CyFunction_set_name, 0, 0},
+    {(char *) "__name__", (getter)__Pyx_CyFunction_get_name, (setter)__Pyx_CyFunction_set_name, 0, 0},
+    {(char *) "__qualname__", (getter)__Pyx_CyFunction_get_qualname, (setter)__Pyx_CyFunction_set_qualname, 0, 0},
+    {(char *) "func_dict", (getter)__Pyx_CyFunction_get_dict, (setter)__Pyx_CyFunction_set_dict, 0, 0},
+    {(char *) "__dict__", (getter)__Pyx_CyFunction_get_dict, (setter)__Pyx_CyFunction_set_dict, 0, 0},
+    {(char *) "func_globals", (getter)__Pyx_CyFunction_get_globals, 0, 0, 0},
+    {(char *) "__globals__", (getter)__Pyx_CyFunction_get_globals, 0, 0, 0},
+    {(char *) "func_closure", (getter)__Pyx_CyFunction_get_closure, 0, 0, 0},
+    {(char *) "__closure__", (getter)__Pyx_CyFunction_get_closure, 0, 0, 0},
+    {(char *) "func_code", (getter)__Pyx_CyFunction_get_code, 0, 0, 0},
+    {(char *) "__code__", (getter)__Pyx_CyFunction_get_code, 0, 0, 0},
+    {(char *) "func_defaults", (getter)__Pyx_CyFunction_get_defaults, (setter)__Pyx_CyFunction_set_defaults, 0, 0},
+    {(char *) "__defaults__", (getter)__Pyx_CyFunction_get_defaults, (setter)__Pyx_CyFunction_set_defaults, 0, 0},
+    {(char *) "__kwdefaults__", (getter)__Pyx_CyFunction_get_kwdefaults, (setter)__Pyx_CyFunction_set_kwdefaults, 0, 0},
+    {(char *) "__annotations__", (getter)__Pyx_CyFunction_get_annotations, (setter)__Pyx_CyFunction_set_annotations, 0, 0},
+    {(char *) "_is_coroutine", (getter)__Pyx_CyFunction_get_is_coroutine, 0, 0, 0},
+    {0, 0, 0, 0, 0}
+};
+static PyMemberDef __pyx_CyFunction_members[] = {
+    {(char *) "__module__", T_OBJECT, offsetof(PyCFunctionObject, m_module), 0, 0},
+#if CYTHON_USE_TYPE_SPECS
+    {(char *) "__dictoffset__", T_PYSSIZET, offsetof(__pyx_CyFunctionObject, func_dict), READONLY, 0},
+#if CYTHON_METH_FASTCALL
+#if CYTHON_BACKPORT_VECTORCALL
+    {(char *) "__vectorcalloffset__", T_PYSSIZET, offsetof(__pyx_CyFunctionObject, func_vectorcall), READONLY, 0},
 #else
-        PyThreadState *tstate = __Pyx_PyThreadState_Current;
-        PyObject* tmp_tb = tstate->curexc_traceback;
-        if (tb != tmp_tb) {
-            Py_INCREF(tb);
-            tstate->curexc_traceback = tb;
-            Py_XDECREF(tmp_tb);
-        }
+    {(char *) "__vectorcalloffset__", T_PYSSIZET, offsetof(PyCFunctionObject, vectorcall), READONLY, 0},
+#endif
+#endif
+#if PY_VERSION_HEX < 0x030500A0
+    {(char *) "__weaklistoffset__", T_PYSSIZET, offsetof(__pyx_CyFunctionObject, func_weakreflist), READONLY, 0},
+#else
+    {(char *) "__weaklistoffset__", T_PYSSIZET, offsetof(PyCFunctionObject, m_weakreflist), READONLY, 0},
+#endif
+#endif
+    {0, 0, 0,  0, 0}
+};
+static PyObject *
+__Pyx_CyFunction_reduce(__pyx_CyFunctionObject *m, PyObject *args)
+{
+    CYTHON_UNUSED_VAR(args);
+#if PY_MAJOR_VERSION >= 3
+    Py_INCREF(m->func_qualname);
+    return m->func_qualname;
+#else
+    return PyString_FromString(((PyCFunctionObject*)m)->m_ml->ml_name);
 #endif
-    }
-bad:
-    Py_XDECREF(owned_instance);
-    return;
 }
+static PyMethodDef __pyx_CyFunction_methods[] = {
+    {"__reduce__", (PyCFunction)__Pyx_CyFunction_reduce, METH_VARARGS, 0},
+    {0, 0, 0, 0}
+};
+#if PY_VERSION_HEX < 0x030500A0
+#define __Pyx_CyFunction_weakreflist(cyfunc) ((cyfunc)->func_weakreflist)
+#else
+#define __Pyx_CyFunction_weakreflist(cyfunc) (((PyCFunctionObject*)cyfunc)->m_weakreflist)
 #endif
-
-/* Import */
-static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level) {
-    PyObject *empty_list = 0;
-    PyObject *module = 0;
-    PyObject *global_dict = 0;
-    PyObject *empty_dict = 0;
-    PyObject *list;
-    #if PY_MAJOR_VERSION < 3
-    PyObject *py_import;
-    py_import = __Pyx_PyObject_GetAttrStr(__pyx_b, __pyx_n_s_import);
-    if (!py_import)
-        goto bad;
-    #endif
-    if (from_list)
-        list = from_list;
-    else {
-        empty_list = PyList_New(0);
-        if (!empty_list)
-            goto bad;
-        list = empty_list;
+static PyObject *__Pyx_CyFunction_Init(__pyx_CyFunctionObject *op, PyMethodDef *ml, int flags, PyObject* qualname,
+                                       PyObject *closure, PyObject *module, PyObject* globals, PyObject* code) {
+    PyCFunctionObject *cf = (PyCFunctionObject*) op;
+    if (unlikely(op == NULL))
+        return NULL;
+    op->flags = flags;
+    __Pyx_CyFunction_weakreflist(op) = NULL;
+    cf->m_ml = ml;
+    cf->m_self = (PyObject *) op;
+    Py_XINCREF(closure);
+    op->func_closure = closure;
+    Py_XINCREF(module);
+    cf->m_module = module;
+    op->func_dict = NULL;
+    op->func_name = NULL;
+    Py_INCREF(qualname);
+    op->func_qualname = qualname;
+    op->func_doc = NULL;
+#if PY_VERSION_HEX < 0x030900B1
+    op->func_classobj = NULL;
+#else
+    ((PyCMethodObject*)op)->mm_class = NULL;
+#endif
+    op->func_globals = globals;
+    Py_INCREF(op->func_globals);
+    Py_XINCREF(code);
+    op->func_code = code;
+    op->defaults_pyobjects = 0;
+    op->defaults_size = 0;
+    op->defaults = NULL;
+    op->defaults_tuple = NULL;
+    op->defaults_kwdict = NULL;
+    op->defaults_getter = NULL;
+    op->func_annotations = NULL;
+    op->func_is_coroutine = NULL;
+#if CYTHON_METH_FASTCALL
+    switch (ml->ml_flags & (METH_VARARGS | METH_FASTCALL | METH_NOARGS | METH_O | METH_KEYWORDS | METH_METHOD)) {
+    case METH_NOARGS:
+        __Pyx_CyFunction_func_vectorcall(op) = __Pyx_CyFunction_Vectorcall_NOARGS;
+        break;
+    case METH_O:
+        __Pyx_CyFunction_func_vectorcall(op) = __Pyx_CyFunction_Vectorcall_O;
+        break;
+    case METH_METHOD | METH_FASTCALL | METH_KEYWORDS:
+        __Pyx_CyFunction_func_vectorcall(op) = __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS_METHOD;
+        break;
+    case METH_FASTCALL | METH_KEYWORDS:
+        __Pyx_CyFunction_func_vectorcall(op) = __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS;
+        break;
+    case METH_VARARGS | METH_KEYWORDS:
+        __Pyx_CyFunction_func_vectorcall(op) = NULL;
+        break;
+    default:
+        PyErr_SetString(PyExc_SystemError, "Bad call flags for CyFunction");
+        Py_DECREF(op);
+        return NULL;
     }
-    global_dict = PyModule_GetDict(__pyx_m);
-    if (!global_dict)
-        goto bad;
-    empty_dict = PyDict_New();
-    if (!empty_dict)
-        goto bad;
+#endif
+    return (PyObject *) op;
+}
+static int
+__Pyx_CyFunction_clear(__pyx_CyFunctionObject *m)
+{
+    Py_CLEAR(m->func_closure);
+    Py_CLEAR(((PyCFunctionObject*)m)->m_module);
+    Py_CLEAR(m->func_dict);
+    Py_CLEAR(m->func_name);
+    Py_CLEAR(m->func_qualname);
+    Py_CLEAR(m->func_doc);
+    Py_CLEAR(m->func_globals);
+    Py_CLEAR(m->func_code);
+#if PY_VERSION_HEX < 0x030900B1
+    Py_CLEAR(__Pyx_CyFunction_GetClassObj(m));
+#else
     {
-        #if PY_MAJOR_VERSION >= 3
-        if (level == -1) {
-            if ((1) && (strchr(__Pyx_MODULE_NAME, '.'))) {
-                module = PyImport_ImportModuleLevelObject(
-                    name, global_dict, empty_dict, list, 1);
-                if (!module) {
-                    if (!PyErr_ExceptionMatches(PyExc_ImportError))
-                        goto bad;
-                    PyErr_Clear();
-                }
+        PyObject *cls = (PyObject*) ((PyCMethodObject *) (m))->mm_class;
+        ((PyCMethodObject *) (m))->mm_class = NULL;
+        Py_XDECREF(cls);
+    }
+#endif
+    Py_CLEAR(m->defaults_tuple);
+    Py_CLEAR(m->defaults_kwdict);
+    Py_CLEAR(m->func_annotations);
+    Py_CLEAR(m->func_is_coroutine);
+    if (m->defaults) {
+        PyObject **pydefaults = __Pyx_CyFunction_Defaults(PyObject *, m);
+        int i;
+        for (i = 0; i < m->defaults_pyobjects; i++)
+            Py_XDECREF(pydefaults[i]);
+        PyObject_Free(m->defaults);
+        m->defaults = NULL;
+    }
+    return 0;
+}
+static void __Pyx__CyFunction_dealloc(__pyx_CyFunctionObject *m)
+{
+    if (__Pyx_CyFunction_weakreflist(m) != NULL)
+        PyObject_ClearWeakRefs((PyObject *) m);
+    __Pyx_CyFunction_clear(m);
+    __Pyx_PyHeapTypeObject_GC_Del(m);
+}
+static void __Pyx_CyFunction_dealloc(__pyx_CyFunctionObject *m)
+{
+    PyObject_GC_UnTrack(m);
+    __Pyx__CyFunction_dealloc(m);
+}
+static int __Pyx_CyFunction_traverse(__pyx_CyFunctionObject *m, visitproc visit, void *arg)
+{
+    Py_VISIT(m->func_closure);
+    Py_VISIT(((PyCFunctionObject*)m)->m_module);
+    Py_VISIT(m->func_dict);
+    Py_VISIT(m->func_name);
+    Py_VISIT(m->func_qualname);
+    Py_VISIT(m->func_doc);
+    Py_VISIT(m->func_globals);
+    Py_VISIT(m->func_code);
+    Py_VISIT(__Pyx_CyFunction_GetClassObj(m));
+    Py_VISIT(m->defaults_tuple);
+    Py_VISIT(m->defaults_kwdict);
+    Py_VISIT(m->func_is_coroutine);
+    if (m->defaults) {
+        PyObject **pydefaults = __Pyx_CyFunction_Defaults(PyObject *, m);
+        int i;
+        for (i = 0; i < m->defaults_pyobjects; i++)
+            Py_VISIT(pydefaults[i]);
+    }
+    return 0;
+}
+static PyObject*
+__Pyx_CyFunction_repr(__pyx_CyFunctionObject *op)
+{
+#if PY_MAJOR_VERSION >= 3
+    return PyUnicode_FromFormat("<cyfunction %U at %p>",
+                                op->func_qualname, (void *)op);
+#else
+    return PyString_FromFormat("<cyfunction %s at %p>",
+                               PyString_AsString(op->func_qualname), (void *)op);
+#endif
+}
+static PyObject * __Pyx_CyFunction_CallMethod(PyObject *func, PyObject *self, PyObject *arg, PyObject *kw) {
+    PyCFunctionObject* f = (PyCFunctionObject*)func;
+    PyCFunction meth = f->m_ml->ml_meth;
+    Py_ssize_t size;
+    switch (f->m_ml->ml_flags & (METH_VARARGS | METH_KEYWORDS | METH_NOARGS | METH_O)) {
+    case METH_VARARGS:
+        if (likely(kw == NULL || PyDict_Size(kw) == 0))
+            return (*meth)(self, arg);
+        break;
+    case METH_VARARGS | METH_KEYWORDS:
+        return (*(PyCFunctionWithKeywords)(void*)meth)(self, arg, kw);
+    case METH_NOARGS:
+        if (likely(kw == NULL || PyDict_Size(kw) == 0)) {
+            size = PyTuple_GET_SIZE(arg);
+            if (likely(size == 0))
+                return (*meth)(self, NULL);
+            PyErr_Format(PyExc_TypeError,
+                "%.200s() takes no arguments (%" CYTHON_FORMAT_SSIZE_T "d given)",
+                f->m_ml->ml_name, size);
+            return NULL;
+        }
+        break;
+    case METH_O:
+        if (likely(kw == NULL || PyDict_Size(kw) == 0)) {
+            size = PyTuple_GET_SIZE(arg);
+            if (likely(size == 1)) {
+                PyObject *result, *arg0;
+                #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+                arg0 = PyTuple_GET_ITEM(arg, 0);
+                #else
+                arg0 = PySequence_ITEM(arg, 0); if (unlikely(!arg0)) return NULL;
+                #endif
+                result = (*meth)(self, arg0);
+                #if !(CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS)
+                Py_DECREF(arg0);
+                #endif
+                return result;
             }
-            level = 0;
+            PyErr_Format(PyExc_TypeError,
+                "%.200s() takes exactly one argument (%" CYTHON_FORMAT_SSIZE_T "d given)",
+                f->m_ml->ml_name, size);
+            return NULL;
         }
-        #endif
-        if (!module) {
-            #if PY_MAJOR_VERSION < 3
-            PyObject *py_level = PyInt_FromLong(level);
-            if (!py_level)
-                goto bad;
-            module = PyObject_CallFunctionObjArgs(py_import,
-                name, global_dict, empty_dict, list, py_level, (PyObject *)NULL);
-            Py_DECREF(py_level);
-            #else
-            module = PyImport_ImportModuleLevelObject(
-                name, global_dict, empty_dict, list, level);
-            #endif
+        break;
+    default:
+        PyErr_SetString(PyExc_SystemError, "Bad call flags for CyFunction");
+        return NULL;
+    }
+    PyErr_Format(PyExc_TypeError, "%.200s() takes no keyword arguments",
+                 f->m_ml->ml_name);
+    return NULL;
+}
+static CYTHON_INLINE PyObject *__Pyx_CyFunction_Call(PyObject *func, PyObject *arg, PyObject *kw) {
+    return __Pyx_CyFunction_CallMethod(func, ((PyCFunctionObject*)func)->m_self, arg, kw);
+}
+static PyObject *__Pyx_CyFunction_CallAsMethod(PyObject *func, PyObject *args, PyObject *kw) {
+    PyObject *result;
+    __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *) func;
+#if CYTHON_METH_FASTCALL
+     __pyx_vectorcallfunc vc = __Pyx_CyFunction_func_vectorcall(cyfunc);
+    if (vc) {
+#if CYTHON_ASSUME_SAFE_MACROS
+        return __Pyx_PyVectorcall_FastCallDict(func, vc, &PyTuple_GET_ITEM(args, 0), (size_t)PyTuple_GET_SIZE(args), kw);
+#else
+        (void) &__Pyx_PyVectorcall_FastCallDict;
+        return PyVectorcall_Call(func, args, kw);
+#endif
+    }
+#endif
+    if ((cyfunc->flags & __Pyx_CYFUNCTION_CCLASS) && !(cyfunc->flags & __Pyx_CYFUNCTION_STATICMETHOD)) {
+        Py_ssize_t argc;
+        PyObject *new_args;
+        PyObject *self;
+        argc = PyTuple_GET_SIZE(args);
+        new_args = PyTuple_GetSlice(args, 1, argc);
+        if (unlikely(!new_args))
+            return NULL;
+        self = PyTuple_GetItem(args, 0);
+        if (unlikely(!self)) {
+            Py_DECREF(new_args);
+#if PY_MAJOR_VERSION > 2
+            PyErr_Format(PyExc_TypeError,
+                         "unbound method %.200S() needs an argument",
+                         cyfunc->func_qualname);
+#else
+            PyErr_SetString(PyExc_TypeError,
+                            "unbound method needs an argument");
+#endif
+            return NULL;
         }
+        result = __Pyx_CyFunction_CallMethod(func, self, new_args, kw);
+        Py_DECREF(new_args);
+    } else {
+        result = __Pyx_CyFunction_Call(func, args, kw);
     }
-bad:
-    #if PY_MAJOR_VERSION < 3
-    Py_XDECREF(py_import);
-    #endif
-    Py_XDECREF(empty_list);
-    Py_XDECREF(empty_dict);
-    return module;
+    return result;
+}
+#if CYTHON_METH_FASTCALL
+static CYTHON_INLINE int __Pyx_CyFunction_Vectorcall_CheckArgs(__pyx_CyFunctionObject *cyfunc, Py_ssize_t nargs, PyObject *kwnames)
+{
+    int ret = 0;
+    if ((cyfunc->flags & __Pyx_CYFUNCTION_CCLASS) && !(cyfunc->flags & __Pyx_CYFUNCTION_STATICMETHOD)) {
+        if (unlikely(nargs < 1)) {
+            PyErr_Format(PyExc_TypeError, "%.200s() needs an argument",
+                         ((PyCFunctionObject*)cyfunc)->m_ml->ml_name);
+            return -1;
+        }
+        ret = 1;
+    }
+    if (unlikely(kwnames) && unlikely(PyTuple_GET_SIZE(kwnames))) {
+        PyErr_Format(PyExc_TypeError,
+                     "%.200s() takes no keyword arguments", ((PyCFunctionObject*)cyfunc)->m_ml->ml_name);
+        return -1;
+    }
+    return ret;
+}
+static PyObject * __Pyx_CyFunction_Vectorcall_NOARGS(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames)
+{
+    __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *)func;
+    PyMethodDef* def = ((PyCFunctionObject*)cyfunc)->m_ml;
+#if CYTHON_BACKPORT_VECTORCALL
+    Py_ssize_t nargs = (Py_ssize_t)nargsf;
+#else
+    Py_ssize_t nargs = PyVectorcall_NARGS(nargsf);
+#endif
+    PyObject *self;
+    switch (__Pyx_CyFunction_Vectorcall_CheckArgs(cyfunc, nargs, kwnames)) {
+    case 1:
+        self = args[0];
+        args += 1;
+        nargs -= 1;
+        break;
+    case 0:
+        self = ((PyCFunctionObject*)cyfunc)->m_self;
+        break;
+    default:
+        return NULL;
+    }
+    if (unlikely(nargs != 0)) {
+        PyErr_Format(PyExc_TypeError,
+            "%.200s() takes no arguments (%" CYTHON_FORMAT_SSIZE_T "d given)",
+            def->ml_name, nargs);
+        return NULL;
+    }
+    return def->ml_meth(self, NULL);
+}
+static PyObject * __Pyx_CyFunction_Vectorcall_O(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames)
+{
+    __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *)func;
+    PyMethodDef* def = ((PyCFunctionObject*)cyfunc)->m_ml;
+#if CYTHON_BACKPORT_VECTORCALL
+    Py_ssize_t nargs = (Py_ssize_t)nargsf;
+#else
+    Py_ssize_t nargs = PyVectorcall_NARGS(nargsf);
+#endif
+    PyObject *self;
+    switch (__Pyx_CyFunction_Vectorcall_CheckArgs(cyfunc, nargs, kwnames)) {
+    case 1:
+        self = args[0];
+        args += 1;
+        nargs -= 1;
+        break;
+    case 0:
+        self = ((PyCFunctionObject*)cyfunc)->m_self;
+        break;
+    default:
+        return NULL;
+    }
+    if (unlikely(nargs != 1)) {
+        PyErr_Format(PyExc_TypeError,
+            "%.200s() takes exactly one argument (%" CYTHON_FORMAT_SSIZE_T "d given)",
+            def->ml_name, nargs);
+        return NULL;
+    }
+    return def->ml_meth(self, args[0]);
+}
+static PyObject * __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames)
+{
+    __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *)func;
+    PyMethodDef* def = ((PyCFunctionObject*)cyfunc)->m_ml;
+#if CYTHON_BACKPORT_VECTORCALL
+    Py_ssize_t nargs = (Py_ssize_t)nargsf;
+#else
+    Py_ssize_t nargs = PyVectorcall_NARGS(nargsf);
+#endif
+    PyObject *self;
+    switch (__Pyx_CyFunction_Vectorcall_CheckArgs(cyfunc, nargs, NULL)) {
+    case 1:
+        self = args[0];
+        args += 1;
+        nargs -= 1;
+        break;
+    case 0:
+        self = ((PyCFunctionObject*)cyfunc)->m_self;
+        break;
+    default:
+        return NULL;
+    }
+    return ((_PyCFunctionFastWithKeywords)(void(*)(void))def->ml_meth)(self, args, nargs, kwnames);
+}
+static PyObject * __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS_METHOD(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames)
+{
+    __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *)func;
+    PyMethodDef* def = ((PyCFunctionObject*)cyfunc)->m_ml;
+    PyTypeObject *cls = (PyTypeObject *) __Pyx_CyFunction_GetClassObj(cyfunc);
+#if CYTHON_BACKPORT_VECTORCALL
+    Py_ssize_t nargs = (Py_ssize_t)nargsf;
+#else
+    Py_ssize_t nargs = PyVectorcall_NARGS(nargsf);
+#endif
+    PyObject *self;
+    switch (__Pyx_CyFunction_Vectorcall_CheckArgs(cyfunc, nargs, NULL)) {
+    case 1:
+        self = args[0];
+        args += 1;
+        nargs -= 1;
+        break;
+    case 0:
+        self = ((PyCFunctionObject*)cyfunc)->m_self;
+        break;
+    default:
+        return NULL;
+    }
+    return ((__Pyx_PyCMethod)(void(*)(void))def->ml_meth)(self, cls, args, (size_t)nargs, kwnames);
+}
+#endif
+#if CYTHON_USE_TYPE_SPECS
+static PyType_Slot __pyx_CyFunctionType_slots[] = {
+    {Py_tp_dealloc, (void *)__Pyx_CyFunction_dealloc},
+    {Py_tp_repr, (void *)__Pyx_CyFunction_repr},
+    {Py_tp_call, (void *)__Pyx_CyFunction_CallAsMethod},
+    {Py_tp_traverse, (void *)__Pyx_CyFunction_traverse},
+    {Py_tp_clear, (void *)__Pyx_CyFunction_clear},
+    {Py_tp_methods, (void *)__pyx_CyFunction_methods},
+    {Py_tp_members, (void *)__pyx_CyFunction_members},
+    {Py_tp_getset, (void *)__pyx_CyFunction_getsets},
+    {Py_tp_descr_get, (void *)__Pyx_PyMethod_New},
+    {0, 0},
+};
+static PyType_Spec __pyx_CyFunctionType_spec = {
+    __PYX_TYPE_MODULE_PREFIX "cython_function_or_method",
+    sizeof(__pyx_CyFunctionObject),
+    0,
+#ifdef Py_TPFLAGS_METHOD_DESCRIPTOR
+    Py_TPFLAGS_METHOD_DESCRIPTOR |
+#endif
+#if (defined(_Py_TPFLAGS_HAVE_VECTORCALL) && CYTHON_METH_FASTCALL)
+    _Py_TPFLAGS_HAVE_VECTORCALL |
+#endif
+    Py_TPFLAGS_DEFAULT | Py_TPFLAGS_HAVE_GC | Py_TPFLAGS_BASETYPE,
+    __pyx_CyFunctionType_slots
+};
+#else
+static PyTypeObject __pyx_CyFunctionType_type = {
+    PyVarObject_HEAD_INIT(0, 0)
+    __PYX_TYPE_MODULE_PREFIX "cython_function_or_method",
+    sizeof(__pyx_CyFunctionObject),
+    0,
+    (destructor) __Pyx_CyFunction_dealloc,
+#if !CYTHON_METH_FASTCALL
+    0,
+#elif CYTHON_BACKPORT_VECTORCALL
+    (printfunc)offsetof(__pyx_CyFunctionObject, func_vectorcall),
+#else
+    offsetof(PyCFunctionObject, vectorcall),
+#endif
+    0,
+    0,
+#if PY_MAJOR_VERSION < 3
+    0,
+#else
+    0,
+#endif
+    (reprfunc) __Pyx_CyFunction_repr,
+    0,
+    0,
+    0,
+    0,
+    __Pyx_CyFunction_CallAsMethod,
+    0,
+    0,
+    0,
+    0,
+#ifdef Py_TPFLAGS_METHOD_DESCRIPTOR
+    Py_TPFLAGS_METHOD_DESCRIPTOR |
+#endif
+#ifdef _Py_TPFLAGS_HAVE_VECTORCALL
+    _Py_TPFLAGS_HAVE_VECTORCALL |
+#endif
+    Py_TPFLAGS_DEFAULT | Py_TPFLAGS_HAVE_GC | Py_TPFLAGS_BASETYPE,
+    0,
+    (traverseproc) __Pyx_CyFunction_traverse,
+    (inquiry) __Pyx_CyFunction_clear,
+    0,
+#if PY_VERSION_HEX < 0x030500A0
+    offsetof(__pyx_CyFunctionObject, func_weakreflist),
+#else
+    offsetof(PyCFunctionObject, m_weakreflist),
+#endif
+    0,
+    0,
+    __pyx_CyFunction_methods,
+    __pyx_CyFunction_members,
+    __pyx_CyFunction_getsets,
+    0,
+    0,
+    __Pyx_PyMethod_New,
+    0,
+    offsetof(__pyx_CyFunctionObject, func_dict),
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+#if PY_VERSION_HEX >= 0x030400a1
+    0,
+#endif
+#if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
+    0,
+#endif
+#if __PYX_NEED_TP_PRINT_SLOT
+    0,
+#endif
+#if PY_VERSION_HEX >= 0x030C0000
+    0,
+#endif
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+    0,
+#endif
+};
+#endif
+static int __pyx_CyFunction_init(PyObject *module) {
+#if CYTHON_USE_TYPE_SPECS
+    __pyx_CyFunctionType = __Pyx_FetchCommonTypeFromSpec(module, &__pyx_CyFunctionType_spec, NULL);
+#else
+    CYTHON_UNUSED_VAR(module);
+    __pyx_CyFunctionType = __Pyx_FetchCommonType(&__pyx_CyFunctionType_type);
+#endif
+    if (unlikely(__pyx_CyFunctionType == NULL)) {
+        return -1;
+    }
+    return 0;
+}
+static CYTHON_INLINE void *__Pyx_CyFunction_InitDefaults(PyObject *func, size_t size, int pyobjects) {
+    __pyx_CyFunctionObject *m = (__pyx_CyFunctionObject *) func;
+    m->defaults = PyObject_Malloc(size);
+    if (unlikely(!m->defaults))
+        return PyErr_NoMemory();
+    memset(m->defaults, 0, size);
+    m->defaults_pyobjects = pyobjects;
+    m->defaults_size = size;
+    return m->defaults;
+}
+static CYTHON_INLINE void __Pyx_CyFunction_SetDefaultsTuple(PyObject *func, PyObject *tuple) {
+    __pyx_CyFunctionObject *m = (__pyx_CyFunctionObject *) func;
+    m->defaults_tuple = tuple;
+    Py_INCREF(tuple);
+}
+static CYTHON_INLINE void __Pyx_CyFunction_SetDefaultsKwDict(PyObject *func, PyObject *dict) {
+    __pyx_CyFunctionObject *m = (__pyx_CyFunctionObject *) func;
+    m->defaults_kwdict = dict;
+    Py_INCREF(dict);
+}
+static CYTHON_INLINE void __Pyx_CyFunction_SetAnnotationsDict(PyObject *func, PyObject *dict) {
+    __pyx_CyFunctionObject *m = (__pyx_CyFunctionObject *) func;
+    m->func_annotations = dict;
+    Py_INCREF(dict);
+}
+
+/* CythonFunction */
+static PyObject *__Pyx_CyFunction_New(PyMethodDef *ml, int flags, PyObject* qualname,
+                                      PyObject *closure, PyObject *module, PyObject* globals, PyObject* code) {
+    PyObject *op = __Pyx_CyFunction_Init(
+        PyObject_GC_New(__pyx_CyFunctionObject, __pyx_CyFunctionType),
+        ml, flags, qualname, closure, module, globals, code
+    );
+    if (likely(op)) {
+        PyObject_GC_Track(op);
+    }
+    return op;
 }
 
 /* CLineInTraceback */
 #ifndef CYTHON_CLINE_IN_TRACEBACK
-static int __Pyx_CLineForTraceback(CYTHON_NCP_UNUSED PyThreadState *tstate, int c_line) {
+static int __Pyx_CLineForTraceback(PyThreadState *tstate, int c_line) {
     PyObject *use_cline;
     PyObject *ptype, *pvalue, *ptraceback;
 #if CYTHON_COMPILING_IN_CPYTHON
     PyObject **cython_runtime_dict;
 #endif
+    CYTHON_MAYBE_UNUSED_VAR(tstate);
     if (unlikely(!__pyx_cython_runtime)) {
         return c_line;
     }
     __Pyx_ErrFetchInState(tstate, &ptype, &pvalue, &ptraceback);
 #if CYTHON_COMPILING_IN_CPYTHON
     cython_runtime_dict = _PyObject_GetDictPtr(__pyx_cython_runtime);
     if (likely(cython_runtime_dict)) {
         __PYX_PY_DICT_LOOKUP_IF_MODIFIED(
             use_cline, *cython_runtime_dict,
             __Pyx_PyDict_GetItemStr(*cython_runtime_dict, __pyx_n_s_cline_in_traceback))
     } else
 #endif
     {
-      PyObject *use_cline_obj = __Pyx_PyObject_GetAttrStr(__pyx_cython_runtime, __pyx_n_s_cline_in_traceback);
+      PyObject *use_cline_obj = __Pyx_PyObject_GetAttrStrNoError(__pyx_cython_runtime, __pyx_n_s_cline_in_traceback);
       if (use_cline_obj) {
         use_cline = PyObject_Not(use_cline_obj) ? Py_False : Py_True;
         Py_DECREF(use_cline_obj);
       } else {
         PyErr_Clear();
         use_cline = NULL;
       }
@@ -4233,14 +6980,15 @@
     }
     __Pyx_ErrRestoreInState(tstate, ptype, pvalue, ptraceback);
     return c_line;
 }
 #endif
 
 /* CodeObjectCache */
+#if !CYTHON_COMPILING_IN_LIMITED_API
 static int __pyx_bisect_code_objects(__Pyx_CodeObjectCacheEntry* entries, int count, int code_line) {
     int start = 0, mid = 0, end = count - 1;
     if (end >= 0 && code_line > entries[end].code_line) {
         return count;
     }
     while (start < end) {
         mid = start + (end - start) / 2;
@@ -4311,19 +7059,36 @@
         entries[i] = entries[i-1];
     }
     entries[pos].code_line = code_line;
     entries[pos].code_object = code_object;
     __pyx_code_cache.count++;
     Py_INCREF(code_object);
 }
+#endif
 
 /* AddTraceback */
 #include "compile.h"
 #include "frameobject.h"
 #include "traceback.h"
+#if PY_VERSION_HEX >= 0x030b00a6
+  #ifndef Py_BUILD_CORE
+    #define Py_BUILD_CORE 1
+  #endif
+  #include "internal/pycore_frame.h"
+#endif
+#if CYTHON_COMPILING_IN_LIMITED_API
+static void __Pyx_AddTraceback(const char *funcname, int c_line,
+                               int py_line, const char *filename) {
+    if (c_line) {
+        (void) __pyx_cfilenm;
+        (void) __Pyx_CLineForTraceback(__Pyx_PyThreadState_Current, c_line);
+    }
+    _PyTraceback_Add(funcname, filename, py_line);
+}
+#else
 static PyCodeObject* __Pyx_CreateCodeObjectForTraceback(
             const char *funcname, int c_line,
             int py_line, const char *filename) {
     PyCodeObject *py_code = NULL;
     PyObject *py_funcname = NULL;
     #if PY_MAJOR_VERSION < 3
     PyObject *py_srcfile = NULL;
@@ -4350,14 +7115,15 @@
     #if PY_MAJOR_VERSION < 3
     py_code = __Pyx_PyCode_New(
         0,
         0,
         0,
         0,
         0,
+        0,
         __pyx_empty_bytes, /*PyObject *code,*/
         __pyx_empty_tuple, /*PyObject *consts,*/
         __pyx_empty_tuple, /*PyObject *names,*/
         __pyx_empty_tuple, /*PyObject *varnames,*/
         __pyx_empty_tuple, /*PyObject *freevars,*/
         __pyx_empty_tuple, /*PyObject *cellvars,*/
         py_srcfile,   /*PyObject *filename,*/
@@ -4379,22 +7145,32 @@
     return NULL;
 }
 static void __Pyx_AddTraceback(const char *funcname, int c_line,
                                int py_line, const char *filename) {
     PyCodeObject *py_code = 0;
     PyFrameObject *py_frame = 0;
     PyThreadState *tstate = __Pyx_PyThreadState_Current;
+    PyObject *ptype, *pvalue, *ptraceback;
     if (c_line) {
         c_line = __Pyx_CLineForTraceback(tstate, c_line);
     }
     py_code = __pyx_find_code_object(c_line ? -c_line : py_line);
     if (!py_code) {
+        __Pyx_ErrFetchInState(tstate, &ptype, &pvalue, &ptraceback);
         py_code = __Pyx_CreateCodeObjectForTraceback(
             funcname, c_line, py_line, filename);
-        if (!py_code) goto bad;
+        if (!py_code) {
+            /* If the code object creation fails, then we should clear the
+               fetched exception references and propagate the new exception */
+            Py_XDECREF(ptype);
+            Py_XDECREF(pvalue);
+            Py_XDECREF(ptraceback);
+            goto bad;
+        }
+        __Pyx_ErrRestoreInState(tstate, ptype, pvalue, ptraceback);
         __pyx_insert_code_object(c_line ? -c_line : py_line, py_code);
     }
     py_frame = PyFrame_New(
         tstate,            /*PyThreadState *tstate,*/
         py_code,           /*PyCodeObject *code,*/
         __pyx_d,    /*PyObject *globals,*/
         0                  /*PyObject *locals*/
@@ -4402,14 +7178,15 @@
     if (!py_frame) goto bad;
     __Pyx_PyFrame_SetLineNumber(py_frame, py_line);
     PyTraceBack_Here(py_frame);
 bad:
     Py_XDECREF(py_code);
     Py_XDECREF(py_frame);
 }
+#endif
 
 /* CIntFromPyVerify */
 #define __PYX_VERIFY_RETURN_INT(target_type, func_type, func_value)\
     __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, 0)
 #define __PYX_VERIFY_RETURN_INT_EXC(target_type, func_type, func_value)\
     __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, 1)
 #define __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, exc)\
@@ -4425,14 +7202,25 @@
                 else\
                     goto raise_overflow;\
             }\
         }\
         return (target_type) value;\
     }
 
+/* RaiseUnexpectedTypeError */
+static int
+__Pyx_RaiseUnexpectedTypeError(const char *expected, PyObject *obj)
+{
+    __Pyx_TypeName obj_type_name = __Pyx_PyType_GetName(Py_TYPE(obj));
+    PyErr_Format(PyExc_TypeError, "Expected %s, got " __Pyx_FMT_TYPENAME,
+                 expected, obj_type_name);
+    __Pyx_DECREF_TypeName(obj_type_name);
+    return 0;
+}
+
 static PyObject* __pyx_convert__to_py_struct__timespec(struct timespec s) {
   PyObject* res;
   PyObject* member;
   res = __Pyx_PyDict_NewPresized(2); if (unlikely(!res)) return NULL;
   member = __Pyx_PyInt_From_time_t(s.tv_sec); if (unlikely(!member)) goto bad;
   if (unlikely(PyDict_SetItem(res, __pyx_n_s_tv_sec, member) < 0)) goto bad;
   Py_DECREF(member);
@@ -4454,177 +7242,254 @@
     const int neg_one = (int) -1, const_zero = (int) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
 #endif
     const int is_unsigned = neg_one > const_zero;
 #if PY_MAJOR_VERSION < 3
     if (likely(PyInt_Check(x))) {
-        if (sizeof(int) < sizeof(long)) {
+        if ((sizeof(int) < sizeof(long))) {
             __PYX_VERIFY_RETURN_INT(int, long, PyInt_AS_LONG(x))
         } else {
             long val = PyInt_AS_LONG(x);
             if (is_unsigned && unlikely(val < 0)) {
                 goto raise_neg_overflow;
             }
             return (int) val;
         }
     } else
 #endif
     if (likely(PyLong_Check(x))) {
         if (is_unsigned) {
 #if CYTHON_USE_PYLONG_INTERNALS
-            const digit* digits = ((PyLongObject*)x)->ob_digit;
-            switch (Py_SIZE(x)) {
-                case  0: return (int) 0;
-                case  1: __PYX_VERIFY_RETURN_INT(int, digit, digits[0])
-                case 2:
-                    if (8 * sizeof(int) > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) >= 2 * PyLong_SHIFT) {
-                            return (int) (((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
+            if (unlikely(__Pyx_PyLong_IsNeg(x))) {
+                goto raise_neg_overflow;
+            } else if (__Pyx_PyLong_IsCompact(x)) {
+                __PYX_VERIFY_RETURN_INT(int, __Pyx_compact_upylong, __Pyx_PyLong_CompactValueUnsigned(x))
+            } else {
+                const digit* digits = __Pyx_PyLong_Digits(x);
+                assert(__Pyx_PyLong_DigitCount(x) > 1);
+                switch (__Pyx_PyLong_DigitCount(x)) {
+                    case 2:
+                        if ((8 * sizeof(int) > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) >= 2 * PyLong_SHIFT)) {
+                                return (int) (((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
+                            }
                         }
-                    }
-                    break;
-                case 3:
-                    if (8 * sizeof(int) > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) >= 3 * PyLong_SHIFT) {
-                            return (int) (((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
+                        break;
+                    case 3:
+                        if ((8 * sizeof(int) > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) >= 3 * PyLong_SHIFT)) {
+                                return (int) (((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
+                            }
                         }
-                    }
-                    break;
-                case 4:
-                    if (8 * sizeof(int) > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
-                            return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
+                        break;
+                    case 4:
+                        if ((8 * sizeof(int) > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) >= 4 * PyLong_SHIFT)) {
+                                return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
+                            }
                         }
-                    }
-                    break;
+                        break;
+                }
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
                     return (int) -1;
                 if (unlikely(result == 1))
                     goto raise_neg_overflow;
             }
 #endif
-            if (sizeof(int) <= sizeof(unsigned long)) {
+            if ((sizeof(int) <= sizeof(unsigned long))) {
                 __PYX_VERIFY_RETURN_INT_EXC(int, unsigned long, PyLong_AsUnsignedLong(x))
 #ifdef HAVE_LONG_LONG
-            } else if (sizeof(int) <= sizeof(unsigned PY_LONG_LONG)) {
+            } else if ((sizeof(int) <= sizeof(unsigned PY_LONG_LONG))) {
                 __PYX_VERIFY_RETURN_INT_EXC(int, unsigned PY_LONG_LONG, PyLong_AsUnsignedLongLong(x))
 #endif
             }
         } else {
 #if CYTHON_USE_PYLONG_INTERNALS
-            const digit* digits = ((PyLongObject*)x)->ob_digit;
-            switch (Py_SIZE(x)) {
-                case  0: return (int) 0;
-                case -1: __PYX_VERIFY_RETURN_INT(int, sdigit, (sdigit) (-(sdigit)digits[0]))
-                case  1: __PYX_VERIFY_RETURN_INT(int,  digit, +digits[0])
-                case -2:
-                    if (8 * sizeof(int) - 1 > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) - 1 > 2 * PyLong_SHIFT) {
-                            return (int) (((int)-1)*(((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+            if (__Pyx_PyLong_IsCompact(x)) {
+                __PYX_VERIFY_RETURN_INT(int, __Pyx_compact_pylong, __Pyx_PyLong_CompactValue(x))
+            } else {
+                const digit* digits = __Pyx_PyLong_Digits(x);
+                assert(__Pyx_PyLong_DigitCount(x) > 1);
+                switch (__Pyx_PyLong_SignedDigitCount(x)) {
+                    case -2:
+                        if ((8 * sizeof(int) - 1 > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) - 1 > 2 * PyLong_SHIFT)) {
+                                return (int) (((int)-1)*(((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case 2:
-                    if (8 * sizeof(int) > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) - 1 > 2 * PyLong_SHIFT) {
-                            return (int) ((((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                        break;
+                    case 2:
+                        if ((8 * sizeof(int) > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) - 1 > 2 * PyLong_SHIFT)) {
+                                return (int) ((((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case -3:
-                    if (8 * sizeof(int) - 1 > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) - 1 > 3 * PyLong_SHIFT) {
-                            return (int) (((int)-1)*(((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                        break;
+                    case -3:
+                        if ((8 * sizeof(int) - 1 > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) - 1 > 3 * PyLong_SHIFT)) {
+                                return (int) (((int)-1)*(((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case 3:
-                    if (8 * sizeof(int) > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) - 1 > 3 * PyLong_SHIFT) {
-                            return (int) ((((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                        break;
+                    case 3:
+                        if ((8 * sizeof(int) > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) - 1 > 3 * PyLong_SHIFT)) {
+                                return (int) ((((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case -4:
-                    if (8 * sizeof(int) - 1 > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) - 1 > 4 * PyLong_SHIFT) {
-                            return (int) (((int)-1)*(((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                        break;
+                    case -4:
+                        if ((8 * sizeof(int) - 1 > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) - 1 > 4 * PyLong_SHIFT)) {
+                                return (int) (((int)-1)*(((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case 4:
-                    if (8 * sizeof(int) > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) - 1 > 4 * PyLong_SHIFT) {
-                            return (int) ((((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                        break;
+                    case 4:
+                        if ((8 * sizeof(int) > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) - 1 > 4 * PyLong_SHIFT)) {
+                                return (int) ((((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                            }
                         }
-                    }
-                    break;
+                        break;
+                }
             }
 #endif
-            if (sizeof(int) <= sizeof(long)) {
+            if ((sizeof(int) <= sizeof(long))) {
                 __PYX_VERIFY_RETURN_INT_EXC(int, long, PyLong_AsLong(x))
 #ifdef HAVE_LONG_LONG
-            } else if (sizeof(int) <= sizeof(PY_LONG_LONG)) {
+            } else if ((sizeof(int) <= sizeof(PY_LONG_LONG))) {
                 __PYX_VERIFY_RETURN_INT_EXC(int, PY_LONG_LONG, PyLong_AsLongLong(x))
 #endif
             }
         }
         {
-#if CYTHON_COMPILING_IN_PYPY && !defined(_PyLong_AsByteArray)
-            PyErr_SetString(PyExc_RuntimeError,
-                            "_PyLong_AsByteArray() not available in PyPy, cannot convert large numbers");
-#else
             int val;
             PyObject *v = __Pyx_PyNumber_IntOrLong(x);
- #if PY_MAJOR_VERSION < 3
+#if PY_MAJOR_VERSION < 3
             if (likely(v) && !PyLong_Check(v)) {
                 PyObject *tmp = v;
                 v = PyNumber_Long(tmp);
                 Py_DECREF(tmp);
             }
- #endif
+#endif
             if (likely(v)) {
+                int ret = -1;
+#if !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
                 int one = 1; int is_little = (int)*(unsigned char *)&one;
                 unsigned char *bytes = (unsigned char *)&val;
-                int ret = _PyLong_AsByteArray((PyLongObject *)v,
-                                              bytes, sizeof(val),
-                                              is_little, !is_unsigned);
+                ret = _PyLong_AsByteArray((PyLongObject *)v,
+                                           bytes, sizeof(val),
+                                           is_little, !is_unsigned);
+#else
+                PyObject *stepval = NULL, *mask = NULL, *shift = NULL;
+                int bits, remaining_bits, is_negative = 0;
+                long idigit;
+                int chunk_size = (sizeof(long) < 8) ? 30 : 62;
+                if (unlikely(!PyLong_CheckExact(v))) {
+                    PyObject *tmp = v;
+                    v = PyNumber_Long(v);
+                    assert(PyLong_CheckExact(v));
+                    Py_DECREF(tmp);
+                    if (unlikely(!v)) return (int) -1;
+                }
+#if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+                if (Py_SIZE(x) == 0)
+                    return (int) 0;
+                is_negative = Py_SIZE(x) < 0;
+#else
+                {
+                    int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
+                    if (unlikely(result < 0))
+                        return (int) -1;
+                    is_negative = result == 1;
+                }
+#endif
+                if (is_unsigned && unlikely(is_negative)) {
+                    goto raise_neg_overflow;
+                } else if (is_negative) {
+                    stepval = PyNumber_Invert(v);
+                    if (unlikely(!stepval))
+                        return (int) -1;
+                } else {
+                    stepval = __Pyx_NewRef(v);
+                }
+                val = (int) 0;
+                mask = PyLong_FromLong((1L << chunk_size) - 1); if (unlikely(!mask)) goto done;
+                shift = PyLong_FromLong(chunk_size); if (unlikely(!shift)) goto done;
+                for (bits = 0; bits < (int) sizeof(int) * 8 - chunk_size; bits += chunk_size) {
+                    PyObject *tmp, *digit;
+                    digit = PyNumber_And(stepval, mask);
+                    if (unlikely(!digit)) goto done;
+                    idigit = PyLong_AsLong(digit);
+                    Py_DECREF(digit);
+                    if (unlikely(idigit < 0)) goto done;
+                    tmp = PyNumber_Rshift(stepval, shift);
+                    if (unlikely(!tmp)) goto done;
+                    Py_DECREF(stepval); stepval = tmp;
+                    val |= ((int) idigit) << bits;
+                    #if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+                    if (Py_SIZE(stepval) == 0)
+                        goto unpacking_done;
+                    #endif
+                }
+                idigit = PyLong_AsLong(stepval);
+                if (unlikely(idigit < 0)) goto done;
+                remaining_bits = ((int) sizeof(int) * 8) - bits - (is_unsigned ? 0 : 1);
+                if (unlikely(idigit >= (1L << remaining_bits)))
+                    goto raise_overflow;
+                val |= ((int) idigit) << bits;
+            #if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+            unpacking_done:
+            #endif
+                if (!is_unsigned) {
+                    if (unlikely(val & (((int) 1) << (sizeof(int) * 8 - 1))))
+                        goto raise_overflow;
+                    if (is_negative)
+                        val = ~val;
+                }
+                ret = 0;
+            done:
+                Py_XDECREF(shift);
+                Py_XDECREF(mask);
+                Py_XDECREF(stepval);
+#endif
                 Py_DECREF(v);
                 if (likely(!ret))
                     return val;
             }
-#endif
             return (int) -1;
         }
     } else {
         int val;
         PyObject *tmp = __Pyx_PyNumber_IntOrLong(x);
         if (!tmp) return (int) -1;
         val = __Pyx_PyInt_As_int(tmp);
@@ -4650,177 +7515,254 @@
     const time_t neg_one = (time_t) -1, const_zero = (time_t) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
 #endif
     const int is_unsigned = neg_one > const_zero;
 #if PY_MAJOR_VERSION < 3
     if (likely(PyInt_Check(x))) {
-        if (sizeof(time_t) < sizeof(long)) {
+        if ((sizeof(time_t) < sizeof(long))) {
             __PYX_VERIFY_RETURN_INT(time_t, long, PyInt_AS_LONG(x))
         } else {
             long val = PyInt_AS_LONG(x);
             if (is_unsigned && unlikely(val < 0)) {
                 goto raise_neg_overflow;
             }
             return (time_t) val;
         }
     } else
 #endif
     if (likely(PyLong_Check(x))) {
         if (is_unsigned) {
 #if CYTHON_USE_PYLONG_INTERNALS
-            const digit* digits = ((PyLongObject*)x)->ob_digit;
-            switch (Py_SIZE(x)) {
-                case  0: return (time_t) 0;
-                case  1: __PYX_VERIFY_RETURN_INT(time_t, digit, digits[0])
-                case 2:
-                    if (8 * sizeof(time_t) > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(time_t, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(time_t) >= 2 * PyLong_SHIFT) {
-                            return (time_t) (((((time_t)digits[1]) << PyLong_SHIFT) | (time_t)digits[0]));
+            if (unlikely(__Pyx_PyLong_IsNeg(x))) {
+                goto raise_neg_overflow;
+            } else if (__Pyx_PyLong_IsCompact(x)) {
+                __PYX_VERIFY_RETURN_INT(time_t, __Pyx_compact_upylong, __Pyx_PyLong_CompactValueUnsigned(x))
+            } else {
+                const digit* digits = __Pyx_PyLong_Digits(x);
+                assert(__Pyx_PyLong_DigitCount(x) > 1);
+                switch (__Pyx_PyLong_DigitCount(x)) {
+                    case 2:
+                        if ((8 * sizeof(time_t) > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(time_t, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(time_t) >= 2 * PyLong_SHIFT)) {
+                                return (time_t) (((((time_t)digits[1]) << PyLong_SHIFT) | (time_t)digits[0]));
+                            }
                         }
-                    }
-                    break;
-                case 3:
-                    if (8 * sizeof(time_t) > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(time_t, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(time_t) >= 3 * PyLong_SHIFT) {
-                            return (time_t) (((((((time_t)digits[2]) << PyLong_SHIFT) | (time_t)digits[1]) << PyLong_SHIFT) | (time_t)digits[0]));
+                        break;
+                    case 3:
+                        if ((8 * sizeof(time_t) > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(time_t, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(time_t) >= 3 * PyLong_SHIFT)) {
+                                return (time_t) (((((((time_t)digits[2]) << PyLong_SHIFT) | (time_t)digits[1]) << PyLong_SHIFT) | (time_t)digits[0]));
+                            }
                         }
-                    }
-                    break;
-                case 4:
-                    if (8 * sizeof(time_t) > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(time_t, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(time_t) >= 4 * PyLong_SHIFT) {
-                            return (time_t) (((((((((time_t)digits[3]) << PyLong_SHIFT) | (time_t)digits[2]) << PyLong_SHIFT) | (time_t)digits[1]) << PyLong_SHIFT) | (time_t)digits[0]));
+                        break;
+                    case 4:
+                        if ((8 * sizeof(time_t) > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(time_t, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(time_t) >= 4 * PyLong_SHIFT)) {
+                                return (time_t) (((((((((time_t)digits[3]) << PyLong_SHIFT) | (time_t)digits[2]) << PyLong_SHIFT) | (time_t)digits[1]) << PyLong_SHIFT) | (time_t)digits[0]));
+                            }
                         }
-                    }
-                    break;
+                        break;
+                }
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
                     return (time_t) -1;
                 if (unlikely(result == 1))
                     goto raise_neg_overflow;
             }
 #endif
-            if (sizeof(time_t) <= sizeof(unsigned long)) {
+            if ((sizeof(time_t) <= sizeof(unsigned long))) {
                 __PYX_VERIFY_RETURN_INT_EXC(time_t, unsigned long, PyLong_AsUnsignedLong(x))
 #ifdef HAVE_LONG_LONG
-            } else if (sizeof(time_t) <= sizeof(unsigned PY_LONG_LONG)) {
+            } else if ((sizeof(time_t) <= sizeof(unsigned PY_LONG_LONG))) {
                 __PYX_VERIFY_RETURN_INT_EXC(time_t, unsigned PY_LONG_LONG, PyLong_AsUnsignedLongLong(x))
 #endif
             }
         } else {
 #if CYTHON_USE_PYLONG_INTERNALS
-            const digit* digits = ((PyLongObject*)x)->ob_digit;
-            switch (Py_SIZE(x)) {
-                case  0: return (time_t) 0;
-                case -1: __PYX_VERIFY_RETURN_INT(time_t, sdigit, (sdigit) (-(sdigit)digits[0]))
-                case  1: __PYX_VERIFY_RETURN_INT(time_t,  digit, +digits[0])
-                case -2:
-                    if (8 * sizeof(time_t) - 1 > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(time_t, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(time_t) - 1 > 2 * PyLong_SHIFT) {
-                            return (time_t) (((time_t)-1)*(((((time_t)digits[1]) << PyLong_SHIFT) | (time_t)digits[0])));
+            if (__Pyx_PyLong_IsCompact(x)) {
+                __PYX_VERIFY_RETURN_INT(time_t, __Pyx_compact_pylong, __Pyx_PyLong_CompactValue(x))
+            } else {
+                const digit* digits = __Pyx_PyLong_Digits(x);
+                assert(__Pyx_PyLong_DigitCount(x) > 1);
+                switch (__Pyx_PyLong_SignedDigitCount(x)) {
+                    case -2:
+                        if ((8 * sizeof(time_t) - 1 > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(time_t, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(time_t) - 1 > 2 * PyLong_SHIFT)) {
+                                return (time_t) (((time_t)-1)*(((((time_t)digits[1]) << PyLong_SHIFT) | (time_t)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case 2:
-                    if (8 * sizeof(time_t) > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(time_t, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(time_t) - 1 > 2 * PyLong_SHIFT) {
-                            return (time_t) ((((((time_t)digits[1]) << PyLong_SHIFT) | (time_t)digits[0])));
+                        break;
+                    case 2:
+                        if ((8 * sizeof(time_t) > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(time_t, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(time_t) - 1 > 2 * PyLong_SHIFT)) {
+                                return (time_t) ((((((time_t)digits[1]) << PyLong_SHIFT) | (time_t)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case -3:
-                    if (8 * sizeof(time_t) - 1 > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(time_t, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(time_t) - 1 > 3 * PyLong_SHIFT) {
-                            return (time_t) (((time_t)-1)*(((((((time_t)digits[2]) << PyLong_SHIFT) | (time_t)digits[1]) << PyLong_SHIFT) | (time_t)digits[0])));
+                        break;
+                    case -3:
+                        if ((8 * sizeof(time_t) - 1 > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(time_t, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(time_t) - 1 > 3 * PyLong_SHIFT)) {
+                                return (time_t) (((time_t)-1)*(((((((time_t)digits[2]) << PyLong_SHIFT) | (time_t)digits[1]) << PyLong_SHIFT) | (time_t)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case 3:
-                    if (8 * sizeof(time_t) > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(time_t, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(time_t) - 1 > 3 * PyLong_SHIFT) {
-                            return (time_t) ((((((((time_t)digits[2]) << PyLong_SHIFT) | (time_t)digits[1]) << PyLong_SHIFT) | (time_t)digits[0])));
+                        break;
+                    case 3:
+                        if ((8 * sizeof(time_t) > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(time_t, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(time_t) - 1 > 3 * PyLong_SHIFT)) {
+                                return (time_t) ((((((((time_t)digits[2]) << PyLong_SHIFT) | (time_t)digits[1]) << PyLong_SHIFT) | (time_t)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case -4:
-                    if (8 * sizeof(time_t) - 1 > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(time_t, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(time_t) - 1 > 4 * PyLong_SHIFT) {
-                            return (time_t) (((time_t)-1)*(((((((((time_t)digits[3]) << PyLong_SHIFT) | (time_t)digits[2]) << PyLong_SHIFT) | (time_t)digits[1]) << PyLong_SHIFT) | (time_t)digits[0])));
+                        break;
+                    case -4:
+                        if ((8 * sizeof(time_t) - 1 > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(time_t, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(time_t) - 1 > 4 * PyLong_SHIFT)) {
+                                return (time_t) (((time_t)-1)*(((((((((time_t)digits[3]) << PyLong_SHIFT) | (time_t)digits[2]) << PyLong_SHIFT) | (time_t)digits[1]) << PyLong_SHIFT) | (time_t)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case 4:
-                    if (8 * sizeof(time_t) > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(time_t, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(time_t) - 1 > 4 * PyLong_SHIFT) {
-                            return (time_t) ((((((((((time_t)digits[3]) << PyLong_SHIFT) | (time_t)digits[2]) << PyLong_SHIFT) | (time_t)digits[1]) << PyLong_SHIFT) | (time_t)digits[0])));
+                        break;
+                    case 4:
+                        if ((8 * sizeof(time_t) > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(time_t, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(time_t) - 1 > 4 * PyLong_SHIFT)) {
+                                return (time_t) ((((((((((time_t)digits[3]) << PyLong_SHIFT) | (time_t)digits[2]) << PyLong_SHIFT) | (time_t)digits[1]) << PyLong_SHIFT) | (time_t)digits[0])));
+                            }
                         }
-                    }
-                    break;
+                        break;
+                }
             }
 #endif
-            if (sizeof(time_t) <= sizeof(long)) {
+            if ((sizeof(time_t) <= sizeof(long))) {
                 __PYX_VERIFY_RETURN_INT_EXC(time_t, long, PyLong_AsLong(x))
 #ifdef HAVE_LONG_LONG
-            } else if (sizeof(time_t) <= sizeof(PY_LONG_LONG)) {
+            } else if ((sizeof(time_t) <= sizeof(PY_LONG_LONG))) {
                 __PYX_VERIFY_RETURN_INT_EXC(time_t, PY_LONG_LONG, PyLong_AsLongLong(x))
 #endif
             }
         }
         {
-#if CYTHON_COMPILING_IN_PYPY && !defined(_PyLong_AsByteArray)
-            PyErr_SetString(PyExc_RuntimeError,
-                            "_PyLong_AsByteArray() not available in PyPy, cannot convert large numbers");
-#else
             time_t val;
             PyObject *v = __Pyx_PyNumber_IntOrLong(x);
- #if PY_MAJOR_VERSION < 3
+#if PY_MAJOR_VERSION < 3
             if (likely(v) && !PyLong_Check(v)) {
                 PyObject *tmp = v;
                 v = PyNumber_Long(tmp);
                 Py_DECREF(tmp);
             }
- #endif
+#endif
             if (likely(v)) {
+                int ret = -1;
+#if !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
                 int one = 1; int is_little = (int)*(unsigned char *)&one;
                 unsigned char *bytes = (unsigned char *)&val;
-                int ret = _PyLong_AsByteArray((PyLongObject *)v,
-                                              bytes, sizeof(val),
-                                              is_little, !is_unsigned);
+                ret = _PyLong_AsByteArray((PyLongObject *)v,
+                                           bytes, sizeof(val),
+                                           is_little, !is_unsigned);
+#else
+                PyObject *stepval = NULL, *mask = NULL, *shift = NULL;
+                int bits, remaining_bits, is_negative = 0;
+                long idigit;
+                int chunk_size = (sizeof(long) < 8) ? 30 : 62;
+                if (unlikely(!PyLong_CheckExact(v))) {
+                    PyObject *tmp = v;
+                    v = PyNumber_Long(v);
+                    assert(PyLong_CheckExact(v));
+                    Py_DECREF(tmp);
+                    if (unlikely(!v)) return (time_t) -1;
+                }
+#if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+                if (Py_SIZE(x) == 0)
+                    return (time_t) 0;
+                is_negative = Py_SIZE(x) < 0;
+#else
+                {
+                    int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
+                    if (unlikely(result < 0))
+                        return (time_t) -1;
+                    is_negative = result == 1;
+                }
+#endif
+                if (is_unsigned && unlikely(is_negative)) {
+                    goto raise_neg_overflow;
+                } else if (is_negative) {
+                    stepval = PyNumber_Invert(v);
+                    if (unlikely(!stepval))
+                        return (time_t) -1;
+                } else {
+                    stepval = __Pyx_NewRef(v);
+                }
+                val = (time_t) 0;
+                mask = PyLong_FromLong((1L << chunk_size) - 1); if (unlikely(!mask)) goto done;
+                shift = PyLong_FromLong(chunk_size); if (unlikely(!shift)) goto done;
+                for (bits = 0; bits < (int) sizeof(time_t) * 8 - chunk_size; bits += chunk_size) {
+                    PyObject *tmp, *digit;
+                    digit = PyNumber_And(stepval, mask);
+                    if (unlikely(!digit)) goto done;
+                    idigit = PyLong_AsLong(digit);
+                    Py_DECREF(digit);
+                    if (unlikely(idigit < 0)) goto done;
+                    tmp = PyNumber_Rshift(stepval, shift);
+                    if (unlikely(!tmp)) goto done;
+                    Py_DECREF(stepval); stepval = tmp;
+                    val |= ((time_t) idigit) << bits;
+                    #if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+                    if (Py_SIZE(stepval) == 0)
+                        goto unpacking_done;
+                    #endif
+                }
+                idigit = PyLong_AsLong(stepval);
+                if (unlikely(idigit < 0)) goto done;
+                remaining_bits = ((int) sizeof(time_t) * 8) - bits - (is_unsigned ? 0 : 1);
+                if (unlikely(idigit >= (1L << remaining_bits)))
+                    goto raise_overflow;
+                val |= ((time_t) idigit) << bits;
+            #if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+            unpacking_done:
+            #endif
+                if (!is_unsigned) {
+                    if (unlikely(val & (((time_t) 1) << (sizeof(time_t) * 8 - 1))))
+                        goto raise_overflow;
+                    if (is_negative)
+                        val = ~val;
+                }
+                ret = 0;
+            done:
+                Py_XDECREF(shift);
+                Py_XDECREF(mask);
+                Py_XDECREF(stepval);
+#endif
                 Py_DECREF(v);
                 if (likely(!ret))
                     return val;
             }
-#endif
             return (time_t) -1;
         }
     } else {
         time_t val;
         PyObject *tmp = __Pyx_PyNumber_IntOrLong(x);
         if (!tmp) return (time_t) -1;
         val = __Pyx_PyInt_As_time_t(tmp);
@@ -4846,177 +7788,254 @@
     const long neg_one = (long) -1, const_zero = (long) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
 #endif
     const int is_unsigned = neg_one > const_zero;
 #if PY_MAJOR_VERSION < 3
     if (likely(PyInt_Check(x))) {
-        if (sizeof(long) < sizeof(long)) {
+        if ((sizeof(long) < sizeof(long))) {
             __PYX_VERIFY_RETURN_INT(long, long, PyInt_AS_LONG(x))
         } else {
             long val = PyInt_AS_LONG(x);
             if (is_unsigned && unlikely(val < 0)) {
                 goto raise_neg_overflow;
             }
             return (long) val;
         }
     } else
 #endif
     if (likely(PyLong_Check(x))) {
         if (is_unsigned) {
 #if CYTHON_USE_PYLONG_INTERNALS
-            const digit* digits = ((PyLongObject*)x)->ob_digit;
-            switch (Py_SIZE(x)) {
-                case  0: return (long) 0;
-                case  1: __PYX_VERIFY_RETURN_INT(long, digit, digits[0])
-                case 2:
-                    if (8 * sizeof(long) > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(long) >= 2 * PyLong_SHIFT) {
-                            return (long) (((((long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
+            if (unlikely(__Pyx_PyLong_IsNeg(x))) {
+                goto raise_neg_overflow;
+            } else if (__Pyx_PyLong_IsCompact(x)) {
+                __PYX_VERIFY_RETURN_INT(long, __Pyx_compact_upylong, __Pyx_PyLong_CompactValueUnsigned(x))
+            } else {
+                const digit* digits = __Pyx_PyLong_Digits(x);
+                assert(__Pyx_PyLong_DigitCount(x) > 1);
+                switch (__Pyx_PyLong_DigitCount(x)) {
+                    case 2:
+                        if ((8 * sizeof(long) > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) >= 2 * PyLong_SHIFT)) {
+                                return (long) (((((long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
+                            }
                         }
-                    }
-                    break;
-                case 3:
-                    if (8 * sizeof(long) > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(long) >= 3 * PyLong_SHIFT) {
-                            return (long) (((((((long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
+                        break;
+                    case 3:
+                        if ((8 * sizeof(long) > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) >= 3 * PyLong_SHIFT)) {
+                                return (long) (((((((long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
+                            }
                         }
-                    }
-                    break;
-                case 4:
-                    if (8 * sizeof(long) > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
-                            return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
+                        break;
+                    case 4:
+                        if ((8 * sizeof(long) > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) >= 4 * PyLong_SHIFT)) {
+                                return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
+                            }
                         }
-                    }
-                    break;
+                        break;
+                }
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
                     return (long) -1;
                 if (unlikely(result == 1))
                     goto raise_neg_overflow;
             }
 #endif
-            if (sizeof(long) <= sizeof(unsigned long)) {
+            if ((sizeof(long) <= sizeof(unsigned long))) {
                 __PYX_VERIFY_RETURN_INT_EXC(long, unsigned long, PyLong_AsUnsignedLong(x))
 #ifdef HAVE_LONG_LONG
-            } else if (sizeof(long) <= sizeof(unsigned PY_LONG_LONG)) {
+            } else if ((sizeof(long) <= sizeof(unsigned PY_LONG_LONG))) {
                 __PYX_VERIFY_RETURN_INT_EXC(long, unsigned PY_LONG_LONG, PyLong_AsUnsignedLongLong(x))
 #endif
             }
         } else {
 #if CYTHON_USE_PYLONG_INTERNALS
-            const digit* digits = ((PyLongObject*)x)->ob_digit;
-            switch (Py_SIZE(x)) {
-                case  0: return (long) 0;
-                case -1: __PYX_VERIFY_RETURN_INT(long, sdigit, (sdigit) (-(sdigit)digits[0]))
-                case  1: __PYX_VERIFY_RETURN_INT(long,  digit, +digits[0])
-                case -2:
-                    if (8 * sizeof(long) - 1 > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(long, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(long) - 1 > 2 * PyLong_SHIFT) {
-                            return (long) (((long)-1)*(((((long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+            if (__Pyx_PyLong_IsCompact(x)) {
+                __PYX_VERIFY_RETURN_INT(long, __Pyx_compact_pylong, __Pyx_PyLong_CompactValue(x))
+            } else {
+                const digit* digits = __Pyx_PyLong_Digits(x);
+                assert(__Pyx_PyLong_DigitCount(x) > 1);
+                switch (__Pyx_PyLong_SignedDigitCount(x)) {
+                    case -2:
+                        if ((8 * sizeof(long) - 1 > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(long, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) - 1 > 2 * PyLong_SHIFT)) {
+                                return (long) (((long)-1)*(((((long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case 2:
-                    if (8 * sizeof(long) > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(long) - 1 > 2 * PyLong_SHIFT) {
-                            return (long) ((((((long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                        break;
+                    case 2:
+                        if ((8 * sizeof(long) > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) - 1 > 2 * PyLong_SHIFT)) {
+                                return (long) ((((((long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case -3:
-                    if (8 * sizeof(long) - 1 > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(long, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(long) - 1 > 3 * PyLong_SHIFT) {
-                            return (long) (((long)-1)*(((((((long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                        break;
+                    case -3:
+                        if ((8 * sizeof(long) - 1 > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(long, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) - 1 > 3 * PyLong_SHIFT)) {
+                                return (long) (((long)-1)*(((((((long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case 3:
-                    if (8 * sizeof(long) > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(long) - 1 > 3 * PyLong_SHIFT) {
-                            return (long) ((((((((long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                        break;
+                    case 3:
+                        if ((8 * sizeof(long) > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) - 1 > 3 * PyLong_SHIFT)) {
+                                return (long) ((((((((long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case -4:
-                    if (8 * sizeof(long) - 1 > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(long, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(long) - 1 > 4 * PyLong_SHIFT) {
-                            return (long) (((long)-1)*(((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                        break;
+                    case -4:
+                        if ((8 * sizeof(long) - 1 > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(long, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) - 1 > 4 * PyLong_SHIFT)) {
+                                return (long) (((long)-1)*(((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case 4:
-                    if (8 * sizeof(long) > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(long) - 1 > 4 * PyLong_SHIFT) {
-                            return (long) ((((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                        break;
+                    case 4:
+                        if ((8 * sizeof(long) > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) - 1 > 4 * PyLong_SHIFT)) {
+                                return (long) ((((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                            }
                         }
-                    }
-                    break;
+                        break;
+                }
             }
 #endif
-            if (sizeof(long) <= sizeof(long)) {
+            if ((sizeof(long) <= sizeof(long))) {
                 __PYX_VERIFY_RETURN_INT_EXC(long, long, PyLong_AsLong(x))
 #ifdef HAVE_LONG_LONG
-            } else if (sizeof(long) <= sizeof(PY_LONG_LONG)) {
+            } else if ((sizeof(long) <= sizeof(PY_LONG_LONG))) {
                 __PYX_VERIFY_RETURN_INT_EXC(long, PY_LONG_LONG, PyLong_AsLongLong(x))
 #endif
             }
         }
         {
-#if CYTHON_COMPILING_IN_PYPY && !defined(_PyLong_AsByteArray)
-            PyErr_SetString(PyExc_RuntimeError,
-                            "_PyLong_AsByteArray() not available in PyPy, cannot convert large numbers");
-#else
             long val;
             PyObject *v = __Pyx_PyNumber_IntOrLong(x);
- #if PY_MAJOR_VERSION < 3
+#if PY_MAJOR_VERSION < 3
             if (likely(v) && !PyLong_Check(v)) {
                 PyObject *tmp = v;
                 v = PyNumber_Long(tmp);
                 Py_DECREF(tmp);
             }
- #endif
+#endif
             if (likely(v)) {
+                int ret = -1;
+#if !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
                 int one = 1; int is_little = (int)*(unsigned char *)&one;
                 unsigned char *bytes = (unsigned char *)&val;
-                int ret = _PyLong_AsByteArray((PyLongObject *)v,
-                                              bytes, sizeof(val),
-                                              is_little, !is_unsigned);
+                ret = _PyLong_AsByteArray((PyLongObject *)v,
+                                           bytes, sizeof(val),
+                                           is_little, !is_unsigned);
+#else
+                PyObject *stepval = NULL, *mask = NULL, *shift = NULL;
+                int bits, remaining_bits, is_negative = 0;
+                long idigit;
+                int chunk_size = (sizeof(long) < 8) ? 30 : 62;
+                if (unlikely(!PyLong_CheckExact(v))) {
+                    PyObject *tmp = v;
+                    v = PyNumber_Long(v);
+                    assert(PyLong_CheckExact(v));
+                    Py_DECREF(tmp);
+                    if (unlikely(!v)) return (long) -1;
+                }
+#if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+                if (Py_SIZE(x) == 0)
+                    return (long) 0;
+                is_negative = Py_SIZE(x) < 0;
+#else
+                {
+                    int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
+                    if (unlikely(result < 0))
+                        return (long) -1;
+                    is_negative = result == 1;
+                }
+#endif
+                if (is_unsigned && unlikely(is_negative)) {
+                    goto raise_neg_overflow;
+                } else if (is_negative) {
+                    stepval = PyNumber_Invert(v);
+                    if (unlikely(!stepval))
+                        return (long) -1;
+                } else {
+                    stepval = __Pyx_NewRef(v);
+                }
+                val = (long) 0;
+                mask = PyLong_FromLong((1L << chunk_size) - 1); if (unlikely(!mask)) goto done;
+                shift = PyLong_FromLong(chunk_size); if (unlikely(!shift)) goto done;
+                for (bits = 0; bits < (int) sizeof(long) * 8 - chunk_size; bits += chunk_size) {
+                    PyObject *tmp, *digit;
+                    digit = PyNumber_And(stepval, mask);
+                    if (unlikely(!digit)) goto done;
+                    idigit = PyLong_AsLong(digit);
+                    Py_DECREF(digit);
+                    if (unlikely(idigit < 0)) goto done;
+                    tmp = PyNumber_Rshift(stepval, shift);
+                    if (unlikely(!tmp)) goto done;
+                    Py_DECREF(stepval); stepval = tmp;
+                    val |= ((long) idigit) << bits;
+                    #if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+                    if (Py_SIZE(stepval) == 0)
+                        goto unpacking_done;
+                    #endif
+                }
+                idigit = PyLong_AsLong(stepval);
+                if (unlikely(idigit < 0)) goto done;
+                remaining_bits = ((int) sizeof(long) * 8) - bits - (is_unsigned ? 0 : 1);
+                if (unlikely(idigit >= (1L << remaining_bits)))
+                    goto raise_overflow;
+                val |= ((long) idigit) << bits;
+            #if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+            unpacking_done:
+            #endif
+                if (!is_unsigned) {
+                    if (unlikely(val & (((long) 1) << (sizeof(long) * 8 - 1))))
+                        goto raise_overflow;
+                    if (is_negative)
+                        val = ~val;
+                }
+                ret = 0;
+            done:
+                Py_XDECREF(shift);
+                Py_XDECREF(mask);
+                Py_XDECREF(stepval);
+#endif
                 Py_DECREF(v);
                 if (likely(!ret))
                     return val;
             }
-#endif
             return (long) -1;
         }
     } else {
         long val;
         PyObject *tmp = __Pyx_PyNumber_IntOrLong(x);
         if (!tmp) return (long) -1;
         val = __Pyx_PyInt_As_long(tmp);
@@ -5143,19 +8162,34 @@
         int one = 1; int little = (int)*(unsigned char *)&one;
         unsigned char *bytes = (unsigned char *)&value;
         return _PyLong_FromByteArray(bytes, sizeof(long),
                                      little, !is_unsigned);
     }
 }
 
+/* FormatTypeName */
+#if CYTHON_COMPILING_IN_LIMITED_API
+static __Pyx_TypeName
+__Pyx_PyType_GetName(PyTypeObject* tp)
+{
+    PyObject *name = __Pyx_PyObject_GetAttrStr((PyObject *)tp,
+                                               __pyx_n_s_name);
+    if (unlikely(name == NULL) || unlikely(!PyUnicode_Check(name))) {
+        PyErr_Clear();
+        Py_XSETREF(name, __Pyx_NewRef(__pyx_n_s__13));
+    }
+    return name;
+}
+#endif
+
 /* FastTypeChecks */
 #if CYTHON_COMPILING_IN_CPYTHON
 static int __Pyx_InBases(PyTypeObject *a, PyTypeObject *b) {
     while (a) {
-        a = a->tp_base;
+        a = __Pyx_PyType_GetSlot(a, tp_base, PyTypeObject*);
         if (a == b)
             return 1;
     }
     return b == &PyBaseObject_Type;
 }
 static CYTHON_INLINE int __Pyx_IsSubtype(PyTypeObject *a, PyTypeObject *b) {
     PyObject *mro;
@@ -5168,14 +8202,30 @@
             if (PyTuple_GET_ITEM(mro, i) == (PyObject *)b)
                 return 1;
         }
         return 0;
     }
     return __Pyx_InBases(a, b);
 }
+static CYTHON_INLINE int __Pyx_IsAnySubtype2(PyTypeObject *cls, PyTypeObject *a, PyTypeObject *b) {
+    PyObject *mro;
+    if (cls == a || cls == b) return 1;
+    mro = cls->tp_mro;
+    if (likely(mro)) {
+        Py_ssize_t i, n;
+        n = PyTuple_GET_SIZE(mro);
+        for (i = 0; i < n; i++) {
+            PyObject *base = PyTuple_GET_ITEM(mro, i);
+            if (base == (PyObject *)a || base == (PyObject *)b)
+                return 1;
+        }
+        return 0;
+    }
+    return __Pyx_InBases(cls, a) || __Pyx_InBases(cls, b);
+}
 #if PY_MAJOR_VERSION == 2
 static int __Pyx_inner_PyErr_GivenExceptionMatches2(PyObject *err, PyObject* exc_type1, PyObject* exc_type2) {
     PyObject *exception, *value, *tb;
     int res;
     __Pyx_PyThreadState_declare
     __Pyx_PyThreadState_assign
     __Pyx_ErrFetch(&exception, &value, &tb);
@@ -5192,19 +8242,19 @@
         }
     }
     __Pyx_ErrRestore(exception, value, tb);
     return res;
 }
 #else
 static CYTHON_INLINE int __Pyx_inner_PyErr_GivenExceptionMatches2(PyObject *err, PyObject* exc_type1, PyObject *exc_type2) {
-    int res = exc_type1 ? __Pyx_IsSubtype((PyTypeObject*)err, (PyTypeObject*)exc_type1) : 0;
-    if (!res) {
-        res = __Pyx_IsSubtype((PyTypeObject*)err, (PyTypeObject*)exc_type2);
+    if (exc_type1) {
+        return __Pyx_IsAnySubtype2((PyTypeObject*)err, (PyTypeObject*)exc_type1, (PyTypeObject*)exc_type2);
+    } else {
+        return __Pyx_IsSubtype((PyTypeObject*)err, (PyTypeObject*)exc_type2);
     }
-    return res;
 }
 #endif
 static int __Pyx_PyErr_GivenExceptionMatchesTuple(PyObject *exc_type, PyObject *tuple) {
     Py_ssize_t i, n;
     assert(PyExceptionClass_Check(exc_type));
     n = PyTuple_GET_SIZE(tuple);
 #if PY_MAJOR_VERSION >= 3
@@ -5245,56 +8295,88 @@
     }
     return (PyErr_GivenExceptionMatches(err, exc_type1) || PyErr_GivenExceptionMatches(err, exc_type2));
 }
 #endif
 
 /* CheckBinaryVersion */
 static int __Pyx_check_binary_version(void) {
-    char ctversion[4], rtversion[4];
-    PyOS_snprintf(ctversion, 4, "%d.%d", PY_MAJOR_VERSION, PY_MINOR_VERSION);
-    PyOS_snprintf(rtversion, 4, "%s", Py_GetVersion());
-    if (ctversion[0] != rtversion[0] || ctversion[2] != rtversion[2]) {
+    char ctversion[5];
+    int same=1, i, found_dot;
+    const char* rt_from_call = Py_GetVersion();
+    PyOS_snprintf(ctversion, 5, "%d.%d", PY_MAJOR_VERSION, PY_MINOR_VERSION);
+    found_dot = 0;
+    for (i = 0; i < 4; i++) {
+        if (!ctversion[i]) {
+            same = (rt_from_call[i] < '0' || rt_from_call[i] > '9');
+            break;
+        }
+        if (rt_from_call[i] != ctversion[i]) {
+            same = 0;
+            break;
+        }
+    }
+    if (!same) {
+        char rtversion[5] = {'\0'};
         char message[200];
+        for (i=0; i<4; ++i) {
+            if (rt_from_call[i] == '.') {
+                if (found_dot) break;
+                found_dot = 1;
+            } else if (rt_from_call[i] < '0' || rt_from_call[i] > '9') {
+                break;
+            }
+            rtversion[i] = rt_from_call[i];
+        }
         PyOS_snprintf(message, sizeof(message),
-                      "compiletime version %s of module '%.100s' "
+                      "compile time version %s of module '%.100s' "
                       "does not match runtime version %s",
                       ctversion, __Pyx_MODULE_NAME, rtversion);
         return PyErr_WarnEx(NULL, message, 1);
     }
     return 0;
 }
 
 /* InitStrings */
+#if PY_MAJOR_VERSION >= 3
+static int __Pyx_InitString(__Pyx_StringTabEntry t, PyObject **str) {
+    if (t.is_unicode | t.is_str) {
+        if (t.intern) {
+            *str = PyUnicode_InternFromString(t.s);
+        } else if (t.encoding) {
+            *str = PyUnicode_Decode(t.s, t.n - 1, t.encoding, NULL);
+        } else {
+            *str = PyUnicode_FromStringAndSize(t.s, t.n - 1);
+        }
+    } else {
+        *str = PyBytes_FromStringAndSize(t.s, t.n - 1);
+    }
+    if (!*str)
+        return -1;
+    if (PyObject_Hash(*str) == -1)
+        return -1;
+    return 0;
+}
+#endif
 static int __Pyx_InitStrings(__Pyx_StringTabEntry *t) {
     while (t->p) {
-        #if PY_MAJOR_VERSION < 3
+        #if PY_MAJOR_VERSION >= 3
+        __Pyx_InitString(*t, t->p);
+        #else
         if (t->is_unicode) {
             *t->p = PyUnicode_DecodeUTF8(t->s, t->n - 1, NULL);
         } else if (t->intern) {
             *t->p = PyString_InternFromString(t->s);
         } else {
             *t->p = PyString_FromStringAndSize(t->s, t->n - 1);
         }
-        #else
-        if (t->is_unicode | t->is_str) {
-            if (t->intern) {
-                *t->p = PyUnicode_InternFromString(t->s);
-            } else if (t->encoding) {
-                *t->p = PyUnicode_Decode(t->s, t->n - 1, t->encoding, NULL);
-            } else {
-                *t->p = PyUnicode_FromStringAndSize(t->s, t->n - 1);
-            }
-        } else {
-            *t->p = PyBytes_FromStringAndSize(t->s, t->n - 1);
-        }
-        #endif
         if (!*t->p)
             return -1;
         if (PyObject_Hash(*t->p) == -1)
             return -1;
+        #endif
         ++t;
     }
     return 0;
 }
 
 static CYTHON_INLINE PyObject* __Pyx_PyUnicode_FromString(const char* c_str) {
     return __Pyx_PyUnicode_FromStringAndSize(c_str, (Py_ssize_t)strlen(c_str));
@@ -5348,15 +8430,15 @@
 #if PY_MAJOR_VERSION < 3 && __PYX_DEFAULT_STRING_ENCODING_IS_ASCII
             __Pyx_sys_getdefaultencoding_not_ascii &&
 #endif
             PyUnicode_Check(o)) {
         return __Pyx_PyUnicode_AsStringAndSize(o, length);
     } else
 #endif
-#if (!CYTHON_COMPILING_IN_PYPY) || (defined(PyByteArray_AS_STRING) && defined(PyByteArray_GET_SIZE))
+#if (!CYTHON_COMPILING_IN_PYPY && !CYTHON_COMPILING_IN_LIMITED_API) || (defined(PyByteArray_AS_STRING) && defined(PyByteArray_GET_SIZE))
     if (PyByteArray_Check(o)) {
         *length = PyByteArray_GET_SIZE(o);
         return PyByteArray_AS_STRING(o);
     } else
 #endif
     {
         char* result;
@@ -5377,30 +8459,34 @@
     int retval;
     if (unlikely(!x)) return -1;
     retval = __Pyx_PyObject_IsTrue(x);
     Py_DECREF(x);
     return retval;
 }
 static PyObject* __Pyx_PyNumber_IntOrLongWrongResultType(PyObject* result, const char* type_name) {
+    __Pyx_TypeName result_type_name = __Pyx_PyType_GetName(Py_TYPE(result));
 #if PY_MAJOR_VERSION >= 3
     if (PyLong_Check(result)) {
         if (PyErr_WarnFormat(PyExc_DeprecationWarning, 1,
-                "__int__ returned non-int (type %.200s).  "
-                "The ability to return an instance of a strict subclass of int "
-                "is deprecated, and may be removed in a future version of Python.",
-                Py_TYPE(result)->tp_name)) {
+                "__int__ returned non-int (type " __Pyx_FMT_TYPENAME ").  "
+                "The ability to return an instance of a strict subclass of int is deprecated, "
+                "and may be removed in a future version of Python.",
+                result_type_name)) {
+            __Pyx_DECREF_TypeName(result_type_name);
             Py_DECREF(result);
             return NULL;
         }
+        __Pyx_DECREF_TypeName(result_type_name);
         return result;
     }
 #endif
     PyErr_Format(PyExc_TypeError,
-                 "__%.4s__ returned non-%.4s (type %.200s)",
-                 type_name, type_name, Py_TYPE(result)->tp_name);
+                 "__%.4s__ returned non-%.4s (type " __Pyx_FMT_TYPENAME ")",
+                 type_name, type_name, result_type_name);
+    __Pyx_DECREF_TypeName(result_type_name);
     Py_DECREF(result);
     return NULL;
 }
 static CYTHON_INLINE PyObject* __Pyx_PyNumber_IntOrLong(PyObject* x) {
 #if CYTHON_USE_TYPE_SLOTS
   PyNumberMethods *m;
 #endif
@@ -5458,21 +8544,19 @@
         return PyInt_AS_LONG(b);
     else
         return PyInt_AsSsize_t(b);
   }
 #endif
   if (likely(PyLong_CheckExact(b))) {
     #if CYTHON_USE_PYLONG_INTERNALS
-    const digit* digits = ((PyLongObject*)b)->ob_digit;
-    const Py_ssize_t size = Py_SIZE(b);
-    if (likely(__Pyx_sst_abs(size) <= 1)) {
-        ival = likely(size) ? digits[0] : 0;
-        if (size == -1) ival = -ival;
-        return ival;
+    if (likely(__Pyx_PyLong_IsCompact(b))) {
+        return __Pyx_PyLong_CompactValue(b);
     } else {
+      const digit* digits = __Pyx_PyLong_Digits(b);
+      const Py_ssize_t size = __Pyx_PyLong_SignedDigitCount(b);
       switch (size) {
          case 2:
            if (8 * sizeof(Py_ssize_t) > 2 * PyLong_SHIFT) {
              return (Py_ssize_t) (((((size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0]));
            }
            break;
          case -2:
@@ -5532,8 +8616,16 @@
   return b ? __Pyx_NewRef(Py_True) : __Pyx_NewRef(Py_False);
 }
 static CYTHON_INLINE PyObject * __Pyx_PyInt_FromSize_t(size_t ival) {
     return PyInt_FromSize_t(ival);
 }
 
 
+/* #### Code section: utility_code_pragmas_end ### */
+#ifdef _MSC_VER
+#pragma warning( pop )
+#endif
+
+
+
+/* #### Code section: end ### */
 #endif /* Py_PYTHON_H */
```

### Comparing `atimer-1.0.1/atimer/_atimer.pyx` & `atimer-1.1.0/atimer/_atimer.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # atimer - timer library for asyncio
 #
-# Copyright (C) 2016-2021 by Artur Wroblewski <wrobell@riseup.net>
+# Copyright (C) 2016 - 2023 by Artur Wroblewski <wrobell@riseup.net>
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
```

### Comparing `atimer-1.0.1/atimer/glue.py` & `atimer-1.1.0/atimer/glue.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # atimer - timer library for asyncio
 #
-# Copyright (C) 2016-2021 by Artur Wroblewski <wrobell@riseup.net>
+# Copyright (C) 2016 - 2023 by Artur Wroblewski <wrobell@riseup.net>
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -31,44 +31,45 @@
 from ._atimer import atimer_init, atimer_start, atimer_close  # type: ignore
 
 logger = logging.getLogger(__name__)
 
 class Timer(Awaitable[int]):
     """
     Timer based on Linux `timerfd` interface.
+
+    Timer object is a Python asynchronous coroutine. It waits for timer
+    expiration. An awaited coroutine returns number of timer expirations.
+
+    The number of expirations is usually `1` until timer overrun happens.
+    Refer to POSIX documentation for definition of the timer overrun.
+
+    :param interval: Interval, in seconds, at which the timer expires.
     """
     def __init__(self, interval: float):
         """
         Create timer object.
 
         :param interval: Interval, in seconds, at which the timer expires.
         """
         self._fd = atimer_init()
         self._interval = interval
-        self._task: tp.Optional[asyncio.Future[int]] = None
-        self._loop: tp.Optional[asyncio.AbstractEventLoop] = None
+        self._task: asyncio.Future[int] | None = None
+        self._loop: asyncio.AbstractEventLoop | None = None
 
     def start(self) -> None:
         """
         Arm the timer.
         """
         self._loop = asyncio.get_running_loop()
         self._loop.add_reader(self._fd, self._timer_expired)
         atimer_start(self._fd, self._interval)
         if __debug__:
             logger.debug('timer armed')
 
     def __await__(self) -> tp.Generator[tp.Any, None, int]:
-        """
-        Wait for timer expiration.
-
-        Return number of timer expirations. The number of expirations is
-        usually `1` until timer overrun happens. Refer to POSIX
-        documentation for definition of timer overrun.
-        """
         assert self._loop is not None
         self._task = self._loop.create_future()
         return (yield from self._task)
 
     def close(self) -> None:
         """
         Stop and disarm the timer.
```

### Comparing `atimer-1.0.1/atimer/tests/__init__.py` & `atimer-1.1.0/atimer/tests/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # atimer - timer library for asyncio
 # 
-# Copyright (C) 2016-2021 by Artur Wroblewski <wrobell@riseup.net>
+# Copyright (C) 2016 - 2023 by Artur Wroblewski <wrobell@riseup.net>
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
```

### Comparing `atimer-1.0.1/atimer/tests/test_atimer.py` & `atimer-1.1.0/atimer/tests/test_atimer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # atimer - timer library for asyncio
 # 
-# Copyright (C) 2016-2021 by Artur Wroblewski <wrobell@riseup.net>
+# Copyright (C) 2016 - 2023 by Artur Wroblewski <wrobell@riseup.net>
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
```

### Comparing `atimer-1.0.1/atimer.egg-info/PKG-INFO` & `atimer-1.1.0/atimer.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,33 @@
 Metadata-Version: 2.1
 Name: atimer
-Version: 1.0.1
+Version: 1.1.0
 Summary: atimer - timer library for asyncio
 Home-page: https://wrobell.dcmod.org/atimer/
 Author: Artur Wroblewski
 Author-email: wrobell@riseup.net
 License: GPLv3+
 Project-URL: Source Code, https://gitlab.com/n23/atimer
 Project-URL: Bug tracker, https://gitlab.com/n23/atimer/issues
-Platform: UNKNOWN
 Classifier: Topic :: Software Development :: Libraries
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
-Requires-Python: >=3.8
+Requires-Python: >=3.11
 Description-Content-Type: text/x-rst
 Provides-Extra: tests
 License-File: COPYING
 
 `atimer` library implements asynchronous timer Python coroutine based on
 POSIX timers. The coroutine can be used with Python `asyncio
 <https://docs.python.org/3/library/asyncio.html>`_ module API.
 
-The main features are
+The main features of the timer implemented by the library are
 
-- timer expires at regular intervals
-- track number of expirations if a long running task causes overrun
-- start synchronized with system clock at the edge of an interval
-- measure time while system is suspended
+- expires at regular intervals
+- allows to track number of expirations if a long running task causes
+  overrun
+- starts synchronized with system clock at the edge of an interval
+- measures time while system is suspended
 
 The `atimer` library is licensed under terms of GPL license, version 3, see
 `COPYING <https://www.gnu.org/licenses/gpl-3.0.en.html>`_ file for details.
-
-
```

### Comparing `atimer-1.0.1/setup.cfg` & `atimer-1.1.0/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = atimer
-version = 1.0.1
+version = 1.1.0
 author = Artur Wroblewski
 author_email = wrobell@riseup.net
 license = GPLv3+
 description = atimer - timer library for asyncio
 long_description = file: README
 long_description_content_type = text/x-rst
 url = https://wrobell.dcmod.org/atimer/
@@ -15,32 +15,31 @@
 	Topic :: Software Development :: Libraries
 	License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 	Programming Language :: Python :: 3
 	Development Status :: 5 - Production/Stable
 
 [options]
 packages = find:
-python_requires = >= 3.8
+python_requires = >= 3.11
 include_package_data = True
 
 [options.package_data]
 * = 
 	py.typed
 	*.pyx
 	*.pyi
 	*.pxd
 
 [options.extras_require]
 tests = 
-	mypy >= 0.931
+	mypy == 1.4.1
 	pytest-cov
 	pytest-timeout
 	pytest-asyncio
 	uvloop
-	types-pkg-resources
 
 [tool:pytest]
 addopts = --cov atimer --cov-report=term-missing
 
 [tool:coverage:report]
 show_missing = 1
 partial_branches = 1
```

### Comparing `atimer-1.0.1/setup.py` & `atimer-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 #
 # atimer - timer library for asyncio
 #
-# Copyright (C) 2016-2021 by Artur Wroblewski <wrobell@riseup.net>
+# Copyright (C) 2016 - 2023 by Artur Wroblewski <wrobell@riseup.net>
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
```

