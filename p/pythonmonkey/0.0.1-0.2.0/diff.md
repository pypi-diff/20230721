# Comparing `tmp/pythonmonkey-0.0.1.tar.gz` & `tmp/pythonmonkey-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythonmonkey-0.0.1.tar", last modified: Wed Apr 12 14:34:44 2023, max compression
+gzip compressed data, was "pythonmonkey-0.2.0.tar", max compression
```

## Comparing `pythonmonkey-0.0.1.tar` & `pythonmonkey-0.2.0.tar`

### file list

```diff
@@ -1,12 +1,136 @@
-drwxrwxr-x   0 xmader    (1000) xmader    (1000)        0 2023-04-12 14:34:44.030356 pythonmonkey-0.0.1/
--rw-rw-r--   0 xmader    (1000) xmader    (1000)      387 2023-04-12 14:34:44.030356 pythonmonkey-0.0.1/PKG-INFO
--rw-rw-r--   0 xmader    (1000) xmader    (1000)      387 2023-04-12 14:28:50.000000 pythonmonkey-0.0.1/pyproject.toml
--rw-rw-r--   0 xmader    (1000) xmader    (1000)       38 2023-04-12 14:34:44.030356 pythonmonkey-0.0.1/setup.cfg
-drwxrwxr-x   0 xmader    (1000) xmader    (1000)        0 2023-04-12 14:34:44.026355 pythonmonkey-0.0.1/src/
-drwxrwxr-x   0 xmader    (1000) xmader    (1000)        0 2023-04-12 14:34:44.026355 pythonmonkey-0.0.1/src/pythonmonkey/
--rw-rw-r--   0 xmader    (1000) xmader    (1000)       28 2023-04-12 14:27:45.000000 pythonmonkey-0.0.1/src/pythonmonkey/__init__.py
-drwxrwxr-x   0 xmader    (1000) xmader    (1000)        0 2023-04-12 14:34:44.030356 pythonmonkey-0.0.1/src/pythonmonkey.egg-info/
--rw-rw-r--   0 xmader    (1000) xmader    (1000)      387 2023-04-12 14:34:44.000000 pythonmonkey-0.0.1/src/pythonmonkey.egg-info/PKG-INFO
--rw-rw-r--   0 xmader    (1000) xmader    (1000)      203 2023-04-12 14:34:44.000000 pythonmonkey-0.0.1/src/pythonmonkey.egg-info/SOURCES.txt
--rw-rw-r--   0 xmader    (1000) xmader    (1000)        1 2023-04-12 14:34:44.000000 pythonmonkey-0.0.1/src/pythonmonkey.egg-info/dependency_links.txt
--rw-rw-r--   0 xmader    (1000) xmader    (1000)       13 2023-04-12 14:34:44.000000 pythonmonkey-0.0.1/src/pythonmonkey.egg-info/top_level.txt
+-rw-r--r--   0        0        0     3284 2023-07-21 13:59:26.607132 pythonmonkey-0.2.0/CMakeLists.txt
+-rw-r--r--   0        0        0     1075 2023-07-21 13:59:26.607132 pythonmonkey-0.2.0/LICENSE
+-rw-r--r--   0        0        0    14866 2023-07-21 13:59:26.607132 pythonmonkey-0.2.0/README.md
+-rw-r--r--   0        0        0     2157 2023-07-21 13:59:26.607132 pythonmonkey-0.2.0/build.py
+-rw-r--r--   0        0        0      921 2023-07-21 13:59:26.607132 pythonmonkey-0.2.0/cmake/docs/CMakeLists.txt
+-rw-r--r--   0        0        0      243 2023-07-21 13:59:26.607132 pythonmonkey-0.2.0/cmake/docs/Doxyfile.in
+-rw-r--r--   0        0        0        0 2023-07-21 13:59:26.607132 pythonmonkey-0.2.0/cmake/docs/mainpage.md
+-rw-r--r--   0        0        0      957 2023-07-21 13:59:26.607132 pythonmonkey-0.2.0/cmake/externals/autopep8/CMakeLists.txt
+-rw-r--r--   0        0        0     1498 2023-07-21 13:59:26.607132 pythonmonkey-0.2.0/cmake/externals/uncrustify/CMakeLists.txt
+-rw-r--r--   0        0        0     3571 2023-07-21 13:59:26.607132 pythonmonkey-0.2.0/cmake/format/CMakeLists.txt
+-rw-r--r--   0        0        0     4714 2023-07-21 13:59:26.607132 pythonmonkey-0.2.0/cmake/format/uncrustify.cfg
+-rw-r--r--   0        0        0     4957 2023-07-21 13:59:26.607132 pythonmonkey-0.2.0/cmake/modules/FindSpiderMonkey.cmake
+-rw-r--r--   0        0        0      643 2023-07-21 13:59:26.607132 pythonmonkey-0.2.0/include/BoolType.hh
+-rw-r--r--   0        0        0     2350 2023-07-21 13:59:26.607132 pythonmonkey-0.2.0/include/BufferType.hh
+-rw-r--r--   0        0        0      951 2023-07-21 13:59:26.607132 pythonmonkey-0.2.0/include/DateType.hh
+-rw-r--r--   0        0        0     1392 2023-07-21 13:59:26.607132 pythonmonkey-0.2.0/include/DictType.hh
+-rw-r--r--   0        0        0     1136 2023-07-21 13:59:26.607132 pythonmonkey-0.2.0/include/ExceptionType.hh
+-rw-r--r--   0        0        0      679 2023-07-21 13:59:26.607132 pythonmonkey-0.2.0/include/FloatType.hh
+-rw-r--r--   0        0        0      643 2023-07-21 13:59:26.607132 pythonmonkey-0.2.0/include/FuncType.hh
+-rw-r--r--   0        0        0     1071 2023-07-21 13:59:26.607132 pythonmonkey-0.2.0/include/IntType.hh
+-rw-r--r--   0        0        0     5828 2023-07-21 13:59:26.607132 pythonmonkey-0.2.0/include/JSObjectProxy.hh
+-rw-r--r--   0        0        0     3771 2023-07-21 13:59:26.607132 pythonmonkey-0.2.0/include/JobQueue.hh
+-rw-r--r--   0        0        0     1220 2023-07-21 13:59:26.607132 pythonmonkey-0.2.0/include/ListType.hh
+-rw-r--r--   0        0        0      506 2023-07-21 13:59:26.607132 pythonmonkey-0.2.0/include/NoneType.hh
+-rw-r--r--   0        0        0      600 2023-07-21 13:59:26.607132 pythonmonkey-0.2.0/include/NullType.hh
+-rw-r--r--   0        0        0     2001 2023-07-21 13:59:26.607132 pythonmonkey-0.2.0/include/PromiseType.hh
+-rw-r--r--   0        0        0     6866 2023-07-21 13:59:26.607132 pythonmonkey-0.2.0/include/PyEventLoop.hh
+-rw-r--r--   0        0        0     7110 2023-07-21 13:59:26.607132 pythonmonkey-0.2.0/include/PyProxyHandler.hh
+-rw-r--r--   0        0        0      655 2023-07-21 13:59:26.607132 pythonmonkey-0.2.0/include/PyType.hh
+-rw-r--r--   0        0        0     1736 2023-07-21 13:59:26.607132 pythonmonkey-0.2.0/include/StrType.hh
+-rw-r--r--   0        0        0      839 2023-07-21 13:59:26.607132 pythonmonkey-0.2.0/include/TupleType.hh
+-rw-r--r--   0        0        0      554 2023-07-21 13:59:26.607132 pythonmonkey-0.2.0/include/TypeEnum.hh
+-rw-r--r--   0        0        0      572 2023-07-21 13:59:26.607132 pythonmonkey-0.2.0/include/internalBinding.hh
+-rw-r--r--   0        0        0     1852 2023-07-21 13:59:26.607132 pythonmonkey-0.2.0/include/jsTypeFactory.hh
+-rw-r--r--   0        0        0     3591 2023-07-21 13:59:26.607132 pythonmonkey-0.2.0/include/modules/pythonmonkey/pythonmonkey.hh
+-rw-r--r--   0        0        0     2112 2023-07-21 13:59:26.607132 pythonmonkey-0.2.0/include/pyTypeFactory.hh
+-rw-r--r--   0        0        0      981 2023-07-21 13:59:26.607132 pythonmonkey-0.2.0/include/setSpiderMonkeyException.hh
+-rw-r--r--   0        0        0     1896 2023-07-21 13:59:50.491216 pythonmonkey-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      908 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/python/pythonmonkey/__init__.py
+-rw-r--r--   0        0        0      617 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/python/pythonmonkey/builtin_modules/base64.d.ts
+-rw-r--r--   0        0        0      633 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/python/pythonmonkey/builtin_modules/base64.py
+-rw-r--r--   0        0        0     2571 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/python/pythonmonkey/builtin_modules/console.js
+-rw-r--r--   0        0        0     1177 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/python/pythonmonkey/builtin_modules/internal-binding.d.ts
+-rw-r--r--   0        0        0      176 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/python/pythonmonkey/builtin_modules/internal-binding.py
+-rw-r--r--   0        0        0    28025 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/python/pythonmonkey/builtin_modules/util.js
+-rw-r--r--   0        0        0        0 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/python/pythonmonkey/cli/__init__.py
+-rwxr-xr-x   0        0        0    13319 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/python/pythonmonkey/cli/pmjs.py
+-rw-r--r--   0        0        0     2157 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/python/pythonmonkey/global.d.ts
+-rw-r--r--   0        0        0     1743 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/python/pythonmonkey/lib/pmjs/global-init.js
+-rw-r--r--   0        0        0     1383 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/python/pythonmonkey/pythonmonkey.pyi
+-rw-r--r--   0        0        0    13456 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/python/pythonmonkey/require.py
+-rw-r--r--   0        0        0      422 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/python/pythonmonkey/tsconfig.json
+-rwxr-xr-x   0        0        0     3181 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/setup.sh
+-rw-r--r--   0        0        0      302 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/src/BoolType.cc
+-rw-r--r--   0        0        0     8782 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/src/BufferType.cc
+-rw-r--r--   0        0        0     1386 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/src/CMakeLists.txt
+-rw-r--r--   0        0        0     1988 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/src/DateType.cc
+-rw-r--r--   0        0        0     1032 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/src/DictType.cc
+-rw-r--r--   0        0        0     2137 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/src/ExceptionType.cc
+-rw-r--r--   0        0        0      391 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/src/FloatType.cc
+-rw-r--r--   0        0        0      256 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/src/FuncType.cc
+-rw-r--r--   0        0        0     7990 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/src/IntType.cc
+-rw-r--r--   0        0        0     8984 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/src/JSObjectProxy.cc
+-rw-r--r--   0        0        0     3679 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/src/JobQueue.cc
+-rw-r--r--   0        0        0      688 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/src/ListType.cc
+-rw-r--r--   0        0        0      331 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/src/NoneType.cc
+-rw-r--r--   0        0        0      419 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/src/NullType.cc
+-rw-r--r--   0        0        0     7205 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/src/PromiseType.cc
+-rw-r--r--   0        0        0     6866 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/src/PyEventLoop.cc
+-rw-r--r--   0        0        0     7947 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/src/PyProxyHandler.cc
+-rw-r--r--   0        0        0      286 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/src/PyType.cc
+-rw-r--r--   0        0        0     6252 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/src/StrType.cc
+-rw-r--r--   0        0        0      577 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/src/TupleType.cc
+-rw-r--r--   0        0        0     3990 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/src/internalBinding/utils.cc
+-rw-r--r--   0        0        0     2404 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/src/internalBinding.cc
+-rw-r--r--   0        0        0    10785 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/src/jsTypeFactory.cc
+-rw-r--r--   0        0        0    18299 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/src/modules/pythonmonkey/pythonmonkey.cc
+-rw-r--r--   0        0        0     7365 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/src/pyTypeFactory.cc
+-rw-r--r--   0        0        0     3502 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/src/setSpiderMonkeyException.cc
+-rwxr-xr-x   0        0        0     1249 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/tests/js/commonjs-modules.bash
+-rw-r--r--   0        0        0      602 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/tests/js/console-smoke.simple
+-rwxr-xr-x   0        0        0      935 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/tests/js/console-stdio.bash
+-rw-r--r--   0        0        0     1008 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/tests/js/console-this.simple
+-rw-r--r--   0        0        0      532 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/tests/js/is-compilable-unit.simple
+-rw-r--r--   0        0        0      962 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/tests/js/js2py/array-change-index.simple
+-rw-r--r--   0        0        0      873 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/tests/js/js2py/arraybuffer.simple
+-rw-r--r--   0        0        0      787 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/tests/js/js2py/bigint.simple
+-rw-r--r--   0        0        0      866 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/tests/js/js2py/boolean.simple
+-rw-r--r--   0        0        0     1175 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/tests/js/js2py/datetime.simple
+-rw-r--r--   0        0        0     2003 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/tests/js/js2py/datetime2.simple
+-rw-r--r--   0        0        0      810 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/tests/js/js2py/function-curry.simple
+-rw-r--r--   0        0        0      733 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/tests/js/js2py/higher-order-function.simple
+-rw-r--r--   0        0        0      846 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/tests/js/js2py/promise-await-in-python.simple.failing
+-rw-r--r--   0        0        0      718 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/tests/js/js2py/promise.simple.failing
+-rw-r--r--   0        0        0      699 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/tests/js/js2py/string.simple
+-rw-r--r--   0        0        0      519 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/tests/js/js2py/trivial-function.simple
+-rw-r--r--   0        0        0      278 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/tests/js/load-cjs-module.simple
+-rw-r--r--   0        0        0      368 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/tests/js/load-cjs-python-module.simple
+-rw-r--r--   0        0        0      268 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/tests/js/modules/cjs-module.js
+-rw-r--r--   0        0        0       67 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/tests/js/modules/print-load.js
+-rw-r--r--   0        0        0      246 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/tests/js/modules/python-cjs-module.py
+-rw-r--r--   0        0        0      371 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/tests/js/modules/vm-tools.py
+-rw-r--r--   0        0        0      447 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/tests/js/not-strict-mode.simple
+-rwxr-xr-x   0        0        0      750 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/tests/js/pmjs-eopt.bash
+-rwxr-xr-x   0        0        0     1211 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/tests/js/pmjs-global-arguments.bash
+-rwxr-xr-x   0        0        0     1289 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/tests/js/pmjs-interactive-smoke.bash
+-rwxr-xr-x   0        0        0      747 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/tests/js/pmjs-popt.bash
+-rwxr-xr-x   0        0        0     1089 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/tests/js/pmjs-require-cache.bash
+-rwxr-xr-x   0        0        0      753 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/tests/js/pmjs-ropt.bash
+-rw-r--r--   0        0        0     1169 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/tests/js/program-module.simple
+-rwxr-xr-x   0        0        0      635 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/tests/js/program.js
+-rw-r--r--   0        0        0      639 2023-07-21 13:59:26.615132 pythonmonkey-0.2.0/tests/js/py2js/array-change-index.simple
+-rw-r--r--   0        0        0      681 2023-07-21 13:59:26.615132 pythonmonkey-0.2.0/tests/js/py2js/arraybuffer.simple
+-rw-r--r--   0        0        0     1026 2023-07-21 13:59:26.615132 pythonmonkey-0.2.0/tests/js/py2js/boolean.simple
+-rw-r--r--   0        0        0     1515 2023-07-21 13:59:26.615132 pythonmonkey-0.2.0/tests/js/py2js/datetime.simple
+-rw-r--r--   0        0        0      903 2023-07-21 13:59:26.615132 pythonmonkey-0.2.0/tests/js/py2js/function-curry.simple.failing
+-rw-r--r--   0        0        0      666 2023-07-21 13:59:26.615132 pythonmonkey-0.2.0/tests/js/py2js/higher-order-function.simple
+-rw-r--r--   0        0        0      591 2023-07-21 13:59:26.615132 pythonmonkey-0.2.0/tests/js/py2js/integer.simple
+-rw-r--r--   0        0        0      669 2023-07-21 13:59:26.615132 pythonmonkey-0.2.0/tests/js/py2js/promise.simple.failing
+-rw-r--r--   0        0        0      538 2023-07-21 13:59:26.615132 pythonmonkey-0.2.0/tests/js/py2js/string.simple
+-rw-r--r--   0        0        0      471 2023-07-21 13:59:26.615132 pythonmonkey-0.2.0/tests/js/py2js/trivial-function.simple
+-rwxr-xr-x   0        0        0      796 2023-07-21 13:59:26.615132 pythonmonkey-0.2.0/tests/js/require-module-stack.bash.failing
+-rw-r--r--   0        0        0     1672 2023-07-21 13:59:26.615132 pythonmonkey-0.2.0/tests/js/test-atob-btoa.simple
+-rw-r--r--   0        0        0      330 2023-07-21 13:59:26.615132 pythonmonkey-0.2.0/tests/js/throw-filename.js
+-rwxr-xr-x   0        0        0     1208 2023-07-21 13:59:26.615132 pythonmonkey-0.2.0/tests/js/typeofs-segfaults.simple.failing
+-rwxr-xr-x   0        0        0     1667 2023-07-21 13:59:26.615132 pythonmonkey-0.2.0/tests/js/typeofs.simple
+-rw-r--r--   0        0        0      432 2023-07-21 13:59:26.615132 pythonmonkey-0.2.0/tests/js/use-strict.simple
+-rw-r--r--   0        0        0      356 2023-07-21 13:59:26.615132 pythonmonkey-0.2.0/tests/python/conftest.py
+-rw-r--r--   0        0        0     6491 2023-07-21 13:59:26.615132 pythonmonkey-0.2.0/tests/python/test_bigints.py
+-rw-r--r--   0        0        0    11020 2023-07-21 13:59:26.615132 pythonmonkey-0.2.0/tests/python/test_buffer_typed_array.py
+-rw-r--r--   0        0        0     4135 2023-07-21 13:59:26.615132 pythonmonkey-0.2.0/tests/python/test_dicts_lists.py
+-rw-r--r--   0        0        0    14294 2023-07-21 13:59:26.615132 pythonmonkey-0.2.0/tests/python/test_event_loop.py
+-rw-r--r--   0        0        0    10622 2023-07-21 13:59:26.615132 pythonmonkey-0.2.0/tests/python/test_pythonmonkey_eval.py
+-rw-r--r--   0        0        0      576 2023-07-21 13:59:26.615132 pythonmonkey-0.2.0/tests/python/test_reentrance_smoke.py
+-rw-r--r--   0        0        0     9095 2023-07-21 13:59:26.615132 pythonmonkey-0.2.0/tests/python/test_strings.py
+-rw-r--r--   0        0        0    15380 1970-01-01 00:00:00.000000 pythonmonkey-0.2.0/PKG-INFO
```

