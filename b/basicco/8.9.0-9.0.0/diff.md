# Comparing `tmp/basicco-8.9.0.tar.gz` & `tmp/basicco-9.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "basicco-8.9.0.tar", last modified: Tue Oct 25 07:15:56 2022, max compression
+gzip compressed data, was "basicco-9.0.0.tar", last modified: Thu Jan 19 00:22:01 2023, max compression
```

## Comparing `basicco-8.9.0.tar` & `basicco-9.0.0.tar`

### file list

```diff
@@ -1,124 +1,127 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 07:15:56.478307 basicco-8.9.0/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 07:15:56.462307 basicco-8.9.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 07:15:56.462307 basicco-8.9.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      578 2022-10-25 07:15:43.000000 basicco-8.9.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (121)      623 2022-10-25 07:15:43.000000 basicco-8.9.0/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (121)      617 2022-10-25 07:15:43.000000 basicco-8.9.0/.github/workflows/mypy.yml
--rw-r--r--   0 runner    (1001) docker     (121)      602 2022-10-25 07:15:43.000000 basicco-8.9.0/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (121)      643 2022-10-25 07:15:43.000000 basicco-8.9.0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1068 2022-10-25 07:15:43.000000 basicco-8.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      406 2022-10-25 07:15:43.000000 basicco-8.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    21189 2022-10-25 07:15:56.478307 basicco-8.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    20772 2022-10-25 07:15:43.000000 basicco-8.9.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 07:15:56.466307 basicco-8.9.0/basicco/
--rw-r--r--   0 runner    (1001) docker     (121)      614 2022-10-25 07:15:43.000000 basicco-8.9.0/basicco/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2356 2022-10-25 07:15:43.000000 basicco-8.9.0/basicco/_bases.py
--rw-r--r--   0 runner    (1001) docker     (121)     5616 2022-10-25 07:15:43.000000 basicco-8.9.0/basicco/abstract_class.py
--rw-r--r--   0 runner    (1001) docker     (121)     5170 2022-10-25 07:15:43.000000 basicco-8.9.0/basicco/basic_data.py
--rw-r--r--   0 runner    (1001) docker     (121)      656 2022-10-25 07:15:43.000000 basicco-8.9.0/basicco/caller_module.py
--rw-r--r--   0 runner    (1001) docker     (121)     8038 2022-10-25 07:15:43.000000 basicco-8.9.0/basicco/context_vars.py
--rw-r--r--   0 runner    (1001) docker     (121)     3065 2022-10-25 07:15:43.000000 basicco-8.9.0/basicco/custom_repr.py
--rw-r--r--   0 runner    (1001) docker     (121)     1848 2022-10-25 07:15:43.000000 basicco-8.9.0/basicco/default_dir.py
--rw-r--r--   0 runner    (1001) docker     (121)     2663 2022-10-25 07:15:43.000000 basicco-8.9.0/basicco/dynamic_code.py
--rw-r--r--   0 runner    (1001) docker     (121)     1133 2022-10-25 07:15:43.000000 basicco-8.9.0/basicco/explicit_hash.py
--rw-r--r--   0 runner    (1001) docker     (121)     3168 2022-10-25 07:15:43.000000 basicco-8.9.0/basicco/fabricate_value.py
--rw-r--r--   0 runner    (1001) docker     (121)     2695 2022-10-25 07:15:43.000000 basicco-8.9.0/basicco/get_mro.py
--rw-r--r--   0 runner    (1001) docker     (121)      452 2022-10-25 07:15:43.000000 basicco-8.9.0/basicco/hash_cache_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (121)      807 2022-10-25 07:15:43.000000 basicco-8.9.0/basicco/implicit_hash.py
--rw-r--r--   0 runner    (1001) docker     (121)     9933 2022-10-25 07:15:43.000000 basicco-8.9.0/basicco/import_path.py
--rw-r--r--   0 runner    (1001) docker     (121)     3867 2022-10-25 07:15:43.000000 basicco-8.9.0/basicco/init_subclass.py
--rw-r--r--   0 runner    (1001) docker     (121)     3102 2022-10-25 07:15:43.000000 basicco-8.9.0/basicco/locked_class.py
--rw-r--r--   0 runner    (1001) docker     (121)     1369 2022-10-25 07:15:43.000000 basicco-8.9.0/basicco/mangling.py
--rw-r--r--   0 runner    (1001) docker     (121)     1036 2022-10-25 07:15:43.000000 basicco-8.9.0/basicco/mapping_proxy.py
--rw-r--r--   0 runner    (1001) docker     (121)     1690 2022-10-25 07:15:43.000000 basicco-8.9.0/basicco/named_tuple.py
--rw-r--r--   0 runner    (1001) docker     (121)     4961 2022-10-25 07:15:43.000000 basicco-8.9.0/basicco/namespace.py
--rw-r--r--   0 runner    (1001) docker     (121)     4858 2022-10-25 07:15:43.000000 basicco-8.9.0/basicco/obj_state.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-25 07:15:43.000000 basicco-8.9.0/basicco/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)     9357 2022-10-25 07:15:43.000000 basicco-8.9.0/basicco/qualname.py
--rw-r--r--   0 runner    (1001) docker     (121)     2596 2022-10-25 07:15:43.000000 basicco-8.9.0/basicco/recursive_repr.py
--rw-r--r--   0 runner    (1001) docker     (121)     4229 2022-10-25 07:15:43.000000 basicco-8.9.0/basicco/runtime_final.py
--rw-r--r--   0 runner    (1001) docker     (121)     1509 2022-10-25 07:15:43.000000 basicco-8.9.0/basicco/safe_not_equals.py
--rw-r--r--   0 runner    (1001) docker     (121)     2129 2022-10-25 07:15:43.000000 basicco-8.9.0/basicco/safe_repr.py
--rw-r--r--   0 runner    (1001) docker     (121)      867 2022-10-25 07:15:43.000000 basicco-8.9.0/basicco/set_name.py
--rw-r--r--   0 runner    (1001) docker     (121)    17403 2022-10-25 07:15:43.000000 basicco-8.9.0/basicco/type_checking.py
--rw-r--r--   0 runner    (1001) docker     (121)      456 2022-10-25 07:15:43.000000 basicco-8.9.0/basicco/unique_iterator.py
--rw-r--r--   0 runner    (1001) docker     (121)     3742 2022-10-25 07:15:43.000000 basicco-8.9.0/basicco/weak_reference.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 07:15:56.466307 basicco-8.9.0/basicco.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    21189 2022-10-25 07:15:56.000000 basicco-8.9.0/basicco.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3228 2022-10-25 07:15:56.000000 basicco-8.9.0/basicco.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-25 07:15:56.000000 basicco-8.9.0/basicco.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      112 2022-10-25 07:15:56.000000 basicco-8.9.0/basicco.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-10-25 07:15:56.000000 basicco-8.9.0/basicco.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 07:15:56.462307 basicco-8.9.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 07:15:56.470307 basicco-8.9.0/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 07:15:56.470307 basicco-8.9.0/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     6282 2022-10-25 07:15:43.000000 basicco-8.9.0/docs/source/_static/basicco.svg
--rw-r--r--   0 runner    (1001) docker     (121)     6337 2022-10-25 07:15:43.000000 basicco-8.9.0/docs/source/_static/basicco_white.svg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 07:15:56.470307 basicco-8.9.0/docs/source/api/
--rw-r--r--   0 runner    (1001) docker     (121)      156 2022-10-25 07:15:43.000000 basicco-8.9.0/docs/source/api/basicco.abstract_class.rst
--rw-r--r--   0 runner    (1001) docker     (121)      144 2022-10-25 07:15:43.000000 basicco-8.9.0/docs/source/api/basicco.basic_data.rst
--rw-r--r--   0 runner    (1001) docker     (121)      153 2022-10-25 07:15:43.000000 basicco-8.9.0/docs/source/api/basicco.caller_module.rst
--rw-r--r--   0 runner    (1001) docker     (121)      150 2022-10-25 07:15:43.000000 basicco-8.9.0/docs/source/api/basicco.context_vars.rst
--rw-r--r--   0 runner    (1001) docker     (121)      147 2022-10-25 07:15:43.000000 basicco-8.9.0/docs/source/api/basicco.custom_repr.rst
--rw-r--r--   0 runner    (1001) docker     (121)      147 2022-10-25 07:15:43.000000 basicco-8.9.0/docs/source/api/basicco.default_dir.rst
--rw-r--r--   0 runner    (1001) docker     (121)      150 2022-10-25 07:15:43.000000 basicco-8.9.0/docs/source/api/basicco.dynamic_code.rst
--rw-r--r--   0 runner    (1001) docker     (121)      153 2022-10-25 07:15:43.000000 basicco-8.9.0/docs/source/api/basicco.explicit_hash.rst
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-10-25 07:15:43.000000 basicco-8.9.0/docs/source/api/basicco.fabricate_value.rst
--rw-r--r--   0 runner    (1001) docker     (121)      135 2022-10-25 07:15:43.000000 basicco-8.9.0/docs/source/api/basicco.get_mro.rst
--rw-r--r--   0 runner    (1001) docker     (121)      170 2022-10-25 07:15:43.000000 basicco-8.9.0/docs/source/api/basicco.hash_cache_wrapper.rst
--rw-r--r--   0 runner    (1001) docker     (121)      153 2022-10-25 07:15:43.000000 basicco-8.9.0/docs/source/api/basicco.implicit_hash.rst
--rw-r--r--   0 runner    (1001) docker     (121)      147 2022-10-25 07:15:43.000000 basicco-8.9.0/docs/source/api/basicco.import_path.rst
--rw-r--r--   0 runner    (1001) docker     (121)      153 2022-10-25 07:15:43.000000 basicco-8.9.0/docs/source/api/basicco.init_subclass.rst
--rw-r--r--   0 runner    (1001) docker     (121)      150 2022-10-25 07:15:43.000000 basicco-8.9.0/docs/source/api/basicco.locked_class.rst
--rw-r--r--   0 runner    (1001) docker     (121)      136 2022-10-25 07:15:43.000000 basicco-8.9.0/docs/source/api/basicco.mangling.rst
--rw-r--r--   0 runner    (1001) docker     (121)      153 2022-10-25 07:15:43.000000 basicco-8.9.0/docs/source/api/basicco.mapping_proxy.rst
--rw-r--r--   0 runner    (1001) docker     (121)      147 2022-10-25 07:15:43.000000 basicco-8.9.0/docs/source/api/basicco.named_tuple.rst
--rw-r--r--   0 runner    (1001) docker     (121)      139 2022-10-25 07:15:43.000000 basicco-8.9.0/docs/source/api/basicco.namespace.rst
--rw-r--r--   0 runner    (1001) docker     (121)      141 2022-10-25 07:15:43.000000 basicco-8.9.0/docs/source/api/basicco.obj_state.rst
--rw-r--r--   0 runner    (1001) docker     (121)      136 2022-10-25 07:15:43.000000 basicco-8.9.0/docs/source/api/basicco.qualname.rst
--rw-r--r--   0 runner    (1001) docker     (121)      156 2022-10-25 07:15:43.000000 basicco-8.9.0/docs/source/api/basicco.recursive_repr.rst
--rw-r--r--   0 runner    (1001) docker     (121)      857 2022-10-25 07:15:43.000000 basicco-8.9.0/docs/source/api/basicco.rst
--rw-r--r--   0 runner    (1001) docker     (121)      153 2022-10-25 07:15:43.000000 basicco-8.9.0/docs/source/api/basicco.runtime_final.rst
--rw-r--r--   0 runner    (1001) docker     (121)      161 2022-10-25 07:15:43.000000 basicco-8.9.0/docs/source/api/basicco.safe_not_equals.rst
--rw-r--r--   0 runner    (1001) docker     (121)      141 2022-10-25 07:15:43.000000 basicco-8.9.0/docs/source/api/basicco.safe_repr.rst
--rw-r--r--   0 runner    (1001) docker     (121)      138 2022-10-25 07:15:43.000000 basicco-8.9.0/docs/source/api/basicco.set_name.rst
--rw-r--r--   0 runner    (1001) docker     (121)      153 2022-10-25 07:15:43.000000 basicco-8.9.0/docs/source/api/basicco.type_checking.rst
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-10-25 07:15:43.000000 basicco-8.9.0/docs/source/api/basicco.unique_iterator.rst
--rw-r--r--   0 runner    (1001) docker     (121)      156 2022-10-25 07:15:43.000000 basicco-8.9.0/docs/source/api/basicco.weak_reference.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1694 2022-10-25 07:15:43.000000 basicco-8.9.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      242 2022-10-25 07:15:43.000000 basicco-8.9.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-10-25 07:15:43.000000 basicco-8.9.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       75 2022-10-25 07:15:43.000000 basicco-8.9.0/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (121)      133 2022-10-25 07:15:56.478307 basicco-8.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1787 2022-10-25 07:15:43.000000 basicco-8.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 07:15:56.478307 basicco-8.9.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     2512 2022-10-25 07:15:43.000000 basicco-8.9.0/tests/test_abstract_class.py
--rw-r--r--   0 runner    (1001) docker     (121)      521 2022-10-25 07:15:43.000000 basicco-8.9.0/tests/test_bases.py
--rw-r--r--   0 runner    (1001) docker     (121)     1808 2022-10-25 07:15:43.000000 basicco-8.9.0/tests/test_basic_data.py
--rw-r--r--   0 runner    (1001) docker     (121)      224 2022-10-25 07:15:43.000000 basicco-8.9.0/tests/test_caller_module.py
--rw-r--r--   0 runner    (1001) docker     (121)     9253 2022-10-25 07:15:43.000000 basicco-8.9.0/tests/test_context_vars.py
--rw-r--r--   0 runner    (1001) docker     (121)     1605 2022-10-25 07:15:43.000000 basicco-8.9.0/tests/test_custom_repr.py
--rw-r--r--   0 runner    (1001) docker     (121)     1293 2022-10-25 07:15:43.000000 basicco-8.9.0/tests/test_default_dir.py
--rw-r--r--   0 runner    (1001) docker     (121)     1148 2022-10-25 07:15:43.000000 basicco-8.9.0/tests/test_dynamic_code.py
--rw-r--r--   0 runner    (1001) docker     (121)     1042 2022-10-25 07:15:43.000000 basicco-8.9.0/tests/test_explicit_hash.py
--rw-r--r--   0 runner    (1001) docker     (121)      668 2022-10-25 07:15:43.000000 basicco-8.9.0/tests/test_fabricate_value.py
--rw-r--r--   0 runner    (1001) docker     (121)     1137 2022-10-25 07:15:43.000000 basicco-8.9.0/tests/test_get_mro.py
--rw-r--r--   0 runner    (1001) docker     (121)      536 2022-10-25 07:15:43.000000 basicco-8.9.0/tests/test_hash_cache_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (121)     1920 2022-10-25 07:15:43.000000 basicco-8.9.0/tests/test_import_path.py
--rw-r--r--   0 runner    (1001) docker     (121)     2571 2022-10-25 07:15:43.000000 basicco-8.9.0/tests/test_init_subclass.py
--rw-r--r--   0 runner    (1001) docker     (121)     1755 2022-10-25 07:15:43.000000 basicco-8.9.0/tests/test_locked_class.py
--rw-r--r--   0 runner    (1001) docker     (121)     1079 2022-10-25 07:15:43.000000 basicco-8.9.0/tests/test_mangling.py
--rw-r--r--   0 runner    (1001) docker     (121)      572 2022-10-25 07:15:43.000000 basicco-8.9.0/tests/test_mapping_proxy.py
--rw-r--r--   0 runner    (1001) docker     (121)      754 2022-10-25 07:15:43.000000 basicco-8.9.0/tests/test_named_tuple.py
--rw-r--r--   0 runner    (1001) docker     (121)     3274 2022-10-25 07:15:43.000000 basicco-8.9.0/tests/test_namespace.py
--rw-r--r--   0 runner    (1001) docker     (121)     3621 2022-10-25 07:15:43.000000 basicco-8.9.0/tests/test_obj_state.py
--rw-r--r--   0 runner    (1001) docker     (121)     3314 2022-10-25 07:15:43.000000 basicco-8.9.0/tests/test_qualname.py
--rw-r--r--   0 runner    (1001) docker     (121)      334 2022-10-25 07:15:43.000000 basicco-8.9.0/tests/test_recursive_repr.py
--rw-r--r--   0 runner    (1001) docker     (121)     2790 2022-10-25 07:15:43.000000 basicco-8.9.0/tests/test_runtime_final.py
--rw-r--r--   0 runner    (1001) docker     (121)      443 2022-10-25 07:15:43.000000 basicco-8.9.0/tests/test_safe_not_equals.py
--rw-r--r--   0 runner    (1001) docker     (121)      397 2022-10-25 07:15:43.000000 basicco-8.9.0/tests/test_safe_repr.py
--rw-r--r--   0 runner    (1001) docker     (121)     1517 2022-10-25 07:15:43.000000 basicco-8.9.0/tests/test_set_name.py
--rw-r--r--   0 runner    (1001) docker     (121)    10804 2022-10-25 07:15:43.000000 basicco-8.9.0/tests/test_type_checking.py
--rw-r--r--   0 runner    (1001) docker     (121)      227 2022-10-25 07:15:43.000000 basicco-8.9.0/tests/test_unique_iterator.py
--rw-r--r--   0 runner    (1001) docker     (121)     2757 2022-10-25 07:15:43.000000 basicco-8.9.0/tests/test_weak_reference.py
--rw-r--r--   0 runner    (1001) docker     (121)      351 2022-10-25 07:15:43.000000 basicco-8.9.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 00:22:01.889637 basicco-9.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 00:22:01.877637 basicco-9.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 00:22:01.877637 basicco-9.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-01-19 00:21:43.000000 basicco-9.0.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-01-19 00:21:43.000000 basicco-9.0.0/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-01-19 00:21:43.000000 basicco-9.0.0/.github/workflows/mypy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-01-19 00:21:43.000000 basicco-9.0.0/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-01-19 00:21:43.000000 basicco-9.0.0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-01-19 00:21:43.000000 basicco-9.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-01-19 00:21:43.000000 basicco-9.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    21355 2023-01-19 00:22:01.889637 basicco-9.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20886 2023-01-19 00:21:43.000000 basicco-9.0.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 00:22:01.881637 basicco-9.0.0/basicco/
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-01-19 00:21:43.000000 basicco-9.0.0/basicco/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-01-19 00:21:43.000000 basicco-9.0.0/basicco/_bases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5643 2023-01-19 00:21:43.000000 basicco-9.0.0/basicco/abstract_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-01-19 00:21:43.000000 basicco-9.0.0/basicco/caller_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7965 2023-01-19 00:21:43.000000 basicco-9.0.0/basicco/context_vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-01-19 00:21:43.000000 basicco-9.0.0/basicco/custom_repr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36064 2023-01-19 00:21:43.000000 basicco-9.0.0/basicco/data_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-01-19 00:21:43.000000 basicco-9.0.0/basicco/default_dir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-01-19 00:21:43.000000 basicco-9.0.0/basicco/dynamic_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-01-19 00:21:43.000000 basicco-9.0.0/basicco/dynamic_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-01-19 00:21:43.000000 basicco-9.0.0/basicco/explicit_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-01-19 00:21:43.000000 basicco-9.0.0/basicco/fabricate_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-01-19 00:21:43.000000 basicco-9.0.0/basicco/get_mro.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-01-19 00:21:43.000000 basicco-9.0.0/basicco/hash_cache_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-01-19 00:21:43.000000 basicco-9.0.0/basicco/implicit_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9933 2023-01-19 00:21:43.000000 basicco-9.0.0/basicco/import_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-01-19 00:21:43.000000 basicco-9.0.0/basicco/init_subclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-01-19 00:21:43.000000 basicco-9.0.0/basicco/locked_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-01-19 00:21:43.000000 basicco-9.0.0/basicco/mangling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-01-19 00:21:43.000000 basicco-9.0.0/basicco/mapping_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-01-19 00:21:43.000000 basicco-9.0.0/basicco/named_tuple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4961 2023-01-19 00:21:43.000000 basicco-9.0.0/basicco/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4858 2023-01-19 00:21:43.000000 basicco-9.0.0/basicco/obj_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-19 00:21:43.000000 basicco-9.0.0/basicco/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     9357 2023-01-19 00:21:43.000000 basicco-9.0.0/basicco/qualname.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-01-19 00:21:43.000000 basicco-9.0.0/basicco/recursive_repr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4256 2023-01-19 00:21:43.000000 basicco-9.0.0/basicco/runtime_final.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-01-19 00:21:43.000000 basicco-9.0.0/basicco/safe_not_equals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-01-19 00:21:43.000000 basicco-9.0.0/basicco/safe_repr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-01-19 00:21:43.000000 basicco-9.0.0/basicco/set_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17386 2023-01-19 00:21:43.000000 basicco-9.0.0/basicco/type_checking.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-01-19 00:21:43.000000 basicco-9.0.0/basicco/unique_iterator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-01-19 00:21:43.000000 basicco-9.0.0/basicco/weak_reference.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 00:22:01.881637 basicco-9.0.0/basicco.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21355 2023-01-19 00:22:01.000000 basicco-9.0.0/basicco.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-01-19 00:22:01.000000 basicco-9.0.0/basicco.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-19 00:22:01.000000 basicco-9.0.0/basicco.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-01-19 00:22:01.000000 basicco-9.0.0/basicco.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-01-19 00:22:01.000000 basicco-9.0.0/basicco.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 00:22:01.877637 basicco-9.0.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 00:22:01.881637 basicco-9.0.0/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 00:22:01.881637 basicco-9.0.0/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     6282 2023-01-19 00:21:43.000000 basicco-9.0.0/docs/source/_static/basicco.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6337 2023-01-19 00:21:43.000000 basicco-9.0.0/docs/source/_static/basicco_white.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 00:22:01.885637 basicco-9.0.0/docs/source/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-01-19 00:21:43.000000 basicco-9.0.0/docs/source/api/basicco.abstract_class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-01-19 00:21:43.000000 basicco-9.0.0/docs/source/api/basicco.caller_module.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-01-19 00:21:43.000000 basicco-9.0.0/docs/source/api/basicco.context_vars.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-01-19 00:21:43.000000 basicco-9.0.0/docs/source/api/basicco.custom_repr.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-01-19 00:21:43.000000 basicco-9.0.0/docs/source/api/basicco.data_class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-01-19 00:21:43.000000 basicco-9.0.0/docs/source/api/basicco.default_dir.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-01-19 00:21:43.000000 basicco-9.0.0/docs/source/api/basicco.dynamic_class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-01-19 00:21:43.000000 basicco-9.0.0/docs/source/api/basicco.dynamic_code.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-01-19 00:21:43.000000 basicco-9.0.0/docs/source/api/basicco.explicit_hash.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-01-19 00:21:43.000000 basicco-9.0.0/docs/source/api/basicco.fabricate_value.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-01-19 00:21:43.000000 basicco-9.0.0/docs/source/api/basicco.get_mro.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-01-19 00:21:43.000000 basicco-9.0.0/docs/source/api/basicco.hash_cache_wrapper.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-01-19 00:21:43.000000 basicco-9.0.0/docs/source/api/basicco.implicit_hash.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-01-19 00:21:43.000000 basicco-9.0.0/docs/source/api/basicco.import_path.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-01-19 00:21:43.000000 basicco-9.0.0/docs/source/api/basicco.init_subclass.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-01-19 00:21:43.000000 basicco-9.0.0/docs/source/api/basicco.locked_class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-01-19 00:21:43.000000 basicco-9.0.0/docs/source/api/basicco.mangling.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-01-19 00:21:43.000000 basicco-9.0.0/docs/source/api/basicco.mapping_proxy.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-01-19 00:21:43.000000 basicco-9.0.0/docs/source/api/basicco.named_tuple.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-01-19 00:21:43.000000 basicco-9.0.0/docs/source/api/basicco.namespace.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-01-19 00:21:43.000000 basicco-9.0.0/docs/source/api/basicco.obj_state.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-01-19 00:21:43.000000 basicco-9.0.0/docs/source/api/basicco.qualname.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-01-19 00:21:43.000000 basicco-9.0.0/docs/source/api/basicco.recursive_repr.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-01-19 00:21:43.000000 basicco-9.0.0/docs/source/api/basicco.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-01-19 00:21:43.000000 basicco-9.0.0/docs/source/api/basicco.runtime_final.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-01-19 00:21:43.000000 basicco-9.0.0/docs/source/api/basicco.safe_not_equals.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-01-19 00:21:43.000000 basicco-9.0.0/docs/source/api/basicco.safe_repr.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-01-19 00:21:43.000000 basicco-9.0.0/docs/source/api/basicco.set_name.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-01-19 00:21:43.000000 basicco-9.0.0/docs/source/api/basicco.type_checking.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-01-19 00:21:43.000000 basicco-9.0.0/docs/source/api/basicco.unique_iterator.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-01-19 00:21:43.000000 basicco-9.0.0/docs/source/api/basicco.weak_reference.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-01-19 00:21:43.000000 basicco-9.0.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-01-19 00:21:43.000000 basicco-9.0.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-01-19 00:21:43.000000 basicco-9.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-01-19 00:21:43.000000 basicco-9.0.0/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-01-19 00:22:01.889637 basicco-9.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-01-19 00:21:43.000000 basicco-9.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 00:22:01.889637 basicco-9.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-01-19 00:21:43.000000 basicco-9.0.0/tests/test_abstract_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-01-19 00:21:43.000000 basicco-9.0.0/tests/test_bases.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-01-19 00:21:43.000000 basicco-9.0.0/tests/test_caller_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9253 2023-01-19 00:21:43.000000 basicco-9.0.0/tests/test_context_vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-01-19 00:21:43.000000 basicco-9.0.0/tests/test_custom_repr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-01-19 00:21:43.000000 basicco-9.0.0/tests/test_data_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-01-19 00:21:43.000000 basicco-9.0.0/tests/test_default_dir.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-01-19 00:21:43.000000 basicco-9.0.0/tests/test_dynamic_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-01-19 00:21:43.000000 basicco-9.0.0/tests/test_dynamic_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-01-19 00:21:43.000000 basicco-9.0.0/tests/test_explicit_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-01-19 00:21:43.000000 basicco-9.0.0/tests/test_fabricate_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-01-19 00:21:43.000000 basicco-9.0.0/tests/test_get_mro.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-01-19 00:21:43.000000 basicco-9.0.0/tests/test_hash_cache_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-01-19 00:21:43.000000 basicco-9.0.0/tests/test_import_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-01-19 00:21:43.000000 basicco-9.0.0/tests/test_init_subclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-01-19 00:21:43.000000 basicco-9.0.0/tests/test_locked_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-01-19 00:21:43.000000 basicco-9.0.0/tests/test_mangling.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-01-19 00:21:43.000000 basicco-9.0.0/tests/test_mapping_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-01-19 00:21:43.000000 basicco-9.0.0/tests/test_named_tuple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-01-19 00:21:43.000000 basicco-9.0.0/tests/test_namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-01-19 00:21:43.000000 basicco-9.0.0/tests/test_obj_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-01-19 00:21:43.000000 basicco-9.0.0/tests/test_qualname.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-01-19 00:21:43.000000 basicco-9.0.0/tests/test_recursive_repr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-01-19 00:21:43.000000 basicco-9.0.0/tests/test_runtime_final.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-01-19 00:21:43.000000 basicco-9.0.0/tests/test_safe_not_equals.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-01-19 00:21:43.000000 basicco-9.0.0/tests/test_safe_repr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-01-19 00:21:43.000000 basicco-9.0.0/tests/test_set_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10804 2023-01-19 00:21:43.000000 basicco-9.0.0/tests/test_type_checking.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-01-19 00:21:43.000000 basicco-9.0.0/tests/test_unique_iterator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-01-19 00:21:43.000000 basicco-9.0.0/tests/test_weak_reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-01-19 00:21:43.000000 basicco-9.0.0/tox.ini
```

### Comparing `basicco-8.9.0/.github/workflows/docs.yml` & `basicco-9.0.0/.github/workflows/docs.yml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 jobs:
   build:
 
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: ["3.10"]
+        python-version: ["3.11"]
 
     steps:
     - uses: actions/checkout@v2
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v2
       with:
         python-version: ${{ matrix.python-version }}
```

### Comparing `basicco-8.9.0/.github/workflows/lint.yml` & `basicco-9.0.0/.github/workflows/lint.yml`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 jobs:
   build:
 
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: ["3.10"]
+        python-version: ["3.11"]
 
     steps:
     - uses: actions/checkout@v2
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v2
       with:
         python-version: ${{ matrix.python-version }}
```

### Comparing `basicco-8.9.0/.github/workflows/mypy.yml` & `basicco-9.0.0/.github/workflows/tests.yml`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-name: MyPy
+name: Tests
 
 on:
   push:
     branches: [ main ]
   pull_request:
     branches: [ main ]
 
 jobs:
   build:
 
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: ["3.10"]
+        python-version: ["3.7", "3.8", "3.9", "3.10", "3.11"]
 
     steps:
     - uses: actions/checkout@v2
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v2
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
+        pip install invoke pytest
         pip install -r requirements.txt
-        pip install -r requirements_dev.txt
-    - name: Mypy check
+    - name: Test with pytest
       run: |
-        inv mypy
+        inv tests
```

### Comparing `basicco-8.9.0/.github/workflows/pypi.yml` & `basicco-9.0.0/.github/workflows/pypi.yml`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     runs-on: ubuntu-latest
 
     steps:
     - uses: actions/checkout@v2
     - name: Set up Python
       uses: actions/setup-python@v2
       with:
-        python-version: "3.10"
+        python-version: "3.11"
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install build setuptools wheel twine
     - name: Build and publish
       env:
         TWINE_USERNAME: ${{ secrets.PYPI_USERNAME }}
```

### Comparing `basicco-8.9.0/.github/workflows/tests.yml` & `basicco-9.0.0/.github/workflows/mypy.yml`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-name: Tests
+name: MyPy
 
 on:
   push:
     branches: [ main ]
   pull_request:
     branches: [ main ]
 
 jobs:
   build:
 
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: ["2.7", "3.7", "3.8", "3.9", "3.10"]
+        python-version: ["3.11"]
 
     steps:
     - uses: actions/checkout@v2
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v2
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
-        pip install invoke pytest
         pip install -r requirements.txt
-    - name: Test with pytest
+        pip install -r requirements_dev.txt
+    - name: Mypy check
       run: |
-        inv tests
+        inv mypy
```

### Comparing `basicco-8.9.0/LICENSE` & `basicco-9.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `basicco-8.9.0/PKG-INFO` & `basicco-9.0.0/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,1325 +1,1306 @@
-00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
-00000010: 3a20 322e 310a 4e61 6d65 3a20 6261 7369  : 2.1.Name: basi
-00000020: 6363 6f0a 5665 7273 696f 6e3a 2038 2e39  cco.Version: 8.9
-00000030: 2e30 0a53 756d 6d61 7279 3a20 436f 6c6c  .0.Summary: Coll
-00000040: 6563 7469 6f6e 206f 6620 6c6f 7765 722d  ection of lower-
-00000050: 6c65 7665 6c20 7574 696c 6974 6965 7320  level utilities 
-00000060: 7468 6174 2065 6e68 616e 6365 2063 6f64  that enhance cod
-00000070: 6520 636f 6d70 6174 6962 696c 6974 7920  e compatibility 
-00000080: 616e 6420 7661 6c69 6461 7469 6f6e 2e0a  and validation..
-00000090: 486f 6d65 2d70 6167 653a 2068 7474 7073  Home-page: https
-000000a0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6272  ://github.com/br
-000000b0: 756e 6f6e 6963 6b6f 2f62 6173 6963 636f  unonicko/basicco
-000000c0: 0a41 7574 686f 723a 2042 7275 6e6f 204e  .Author: Bruno N
-000000d0: 6963 6b6f 0a41 7574 686f 722d 656d 6169  icko.Author-emai
-000000e0: 6c3a 2062 7275 6e6f 6e69 636b 6f40 676d  l: brunonicko@gm
-000000f0: 6169 6c2e 636f 6d0a 436c 6173 7369 6669  ail.com.Classifi
-00000100: 6572 3a20 496e 7465 6e64 6564 2041 7564  er: Intended Aud
-00000110: 6965 6e63 6520 3a3a 2044 6576 656c 6f70  ience :: Develop
-00000120: 6572 730a 436c 6173 7369 6669 6572 3a20  ers.Classifier: 
-00000130: 4c69 6365 6e73 6520 3a3a 204f 5349 2041  License :: OSI A
-00000140: 7070 726f 7665 6420 3a3a 204d 4954 204c  pproved :: MIT L
-00000150: 6963 656e 7365 0a43 6c61 7373 6966 6965  icense.Classifie
-00000160: 723a 204f 7065 7261 7469 6e67 2053 7973  r: Operating Sys
-00000170: 7465 6d20 3a3a 204f 5320 496e 6465 7065  tem :: OS Indepe
-00000180: 6e64 656e 740a 436c 6173 7369 6669 6572  ndent.Classifier
-00000190: 3a20 5072 6f67 7261 6d6d 696e 6720 4c61  : Programming La
-000001a0: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-000001b0: 203a 3a20 322e 370a 436c 6173 7369 6669   :: 2.7.Classifi
-000001c0: 6572 3a20 5072 6f67 7261 6d6d 696e 6720  er: Programming 
-000001d0: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
-000001e0: 6f6e 203a 3a20 332e 370a 436c 6173 7369  on :: 3.7.Classi
-000001f0: 6669 6572 3a20 5072 6f67 7261 6d6d 696e  fier: Programmin
-00000200: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-00000210: 7468 6f6e 203a 3a20 332e 380a 436c 6173  thon :: 3.8.Clas
-00000220: 7369 6669 6572 3a20 5072 6f67 7261 6d6d  sifier: Programm
-00000230: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
-00000240: 5079 7468 6f6e 203a 3a20 332e 390a 436c  Python :: 3.9.Cl
-00000250: 6173 7369 6669 6572 3a20 5072 6f67 7261  assifier: Progra
-00000260: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-00000270: 3a20 5079 7468 6f6e 203a 3a20 332e 3130  : Python :: 3.10
-00000280: 0a43 6c61 7373 6966 6965 723a 2050 726f  .Classifier: Pro
-00000290: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
-000002a0: 6520 3a3a 2050 7974 686f 6e20 3a3a 2049  e :: Python :: I
-000002b0: 6d70 6c65 6d65 6e74 6174 696f 6e20 3a3a  mplementation ::
-000002c0: 2050 7950 790a 5265 7175 6972 6573 2d50   PyPy.Requires-P
-000002d0: 7974 686f 6e3a 203e 3d20 322e 372c 2021  ython: >= 2.7, !
-000002e0: 3d20 332e 302e 2a2c 2021 3d20 332e 312e  = 3.0.*, != 3.1.
-000002f0: 2a2c 2021 3d20 332e 322e 2a2c 2021 3d20  *, != 3.2.*, != 
-00000300: 332e 332e 2a2c 2021 3d20 332e 342e 2a2c  3.3.*, != 3.4.*,
-00000310: 2021 3d20 332e 352e 2a2c 2021 3d20 332e   != 3.5.*, != 3.
-00000320: 362e 2a0a 4465 7363 7269 7074 696f 6e2d  6.*.Description-
-00000330: 436f 6e74 656e 742d 5479 7065 3a20 7465  Content-Type: te
-00000340: 7874 2f78 2d72 7374 0a4c 6963 656e 7365  xt/x-rst.License
-00000350: 2d46 696c 653a 204c 4943 454e 5345 0a0a  -File: LICENSE..
-00000360: 4261 7369 6363 6f0a 3d3d 3d3d 3d3d 3d0a  Basicco.=======.
-00000370: 0a2e 2e20 696d 6167 653a 3a20 6874 7470  ... image:: http
-00000380: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f62  s://github.com/b
-00000390: 7275 6e6f 6e69 636b 6f2f 6261 7369 6363  runonicko/basicc
-000003a0: 6f2f 776f 726b 666c 6f77 732f 4d79 5079  o/workflows/MyPy
-000003b0: 2f62 6164 6765 2e73 7667 0a20 2020 3a74  /badge.svg.   :t
-000003c0: 6172 6765 743a 2068 7474 7073 3a2f 2f67  arget: https://g
-000003d0: 6974 6875 622e 636f 6d2f 6272 756e 6f6e  ithub.com/brunon
-000003e0: 6963 6b6f 2f62 6173 6963 636f 2f61 6374  icko/basicco/act
-000003f0: 696f 6e73 3f71 7565 7279 3d77 6f72 6b66  ions?query=workf
-00000400: 6c6f 7725 3341 4d79 5079 0a0a 2e2e 2069  low%3AMyPy.... i
-00000410: 6d61 6765 3a3a 2068 7474 7073 3a2f 2f67  mage:: https://g
-00000420: 6974 6875 622e 636f 6d2f 6272 756e 6f6e  ithub.com/brunon
-00000430: 6963 6b6f 2f62 6173 6963 636f 2f77 6f72  icko/basicco/wor
-00000440: 6b66 6c6f 7773 2f4c 696e 742f 6261 6467  kflows/Lint/badg
-00000450: 652e 7376 670a 2020 203a 7461 7267 6574  e.svg.   :target
-00000460: 3a20 6874 7470 733a 2f2f 6769 7468 7562  : https://github
-00000470: 2e63 6f6d 2f62 7275 6e6f 6e69 636b 6f2f  .com/brunonicko/
-00000480: 6261 7369 6363 6f2f 6163 7469 6f6e 733f  basicco/actions?
-00000490: 7175 6572 793d 776f 726b 666c 6f77 2533  query=workflow%3
-000004a0: 414c 696e 740a 0a2e 2e20 696d 6167 653a  ALint.... image:
-000004b0: 3a20 6874 7470 733a 2f2f 6769 7468 7562  : https://github
-000004c0: 2e63 6f6d 2f62 7275 6e6f 6e69 636b 6f2f  .com/brunonicko/
-000004d0: 6261 7369 6363 6f2f 776f 726b 666c 6f77  basicco/workflow
-000004e0: 732f 5465 7374 732f 6261 6467 652e 7376  s/Tests/badge.sv
-000004f0: 670a 2020 203a 7461 7267 6574 3a20 6874  g.   :target: ht
-00000500: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000510: 2f62 7275 6e6f 6e69 636b 6f2f 6261 7369  /brunonicko/basi
-00000520: 6363 6f2f 6163 7469 6f6e 733f 7175 6572  cco/actions?quer
-00000530: 793d 776f 726b 666c 6f77 2533 4154 6573  y=workflow%3ATes
-00000540: 7473 0a0a 2e2e 2069 6d61 6765 3a3a 2068  ts.... image:: h
-00000550: 7474 7073 3a2f 2f72 6561 6474 6865 646f  ttps://readthedo
-00000560: 6373 2e6f 7267 2f70 726f 6a65 6374 732f  cs.org/projects/
-00000570: 6261 7369 6363 6f2f 6261 6467 652f 3f76  basicco/badge/?v
-00000580: 6572 7369 6f6e 3d73 7461 626c 650a 2020  ersion=stable.  
-00000590: 203a 7461 7267 6574 3a20 6874 7470 733a   :target: https:
-000005a0: 2f2f 6261 7369 6363 6f2e 7265 6164 7468  //basicco.readth
-000005b0: 6564 6f63 732e 696f 2f65 6e2f 7374 6162  edocs.io/en/stab
-000005c0: 6c65 2f0a 0a2e 2e20 696d 6167 653a 3a20  le/.... image:: 
-000005d0: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
-000005e0: 6c64 732e 696f 2f67 6974 6875 622f 6c69  lds.io/github/li
-000005f0: 6365 6e73 652f 6272 756e 6f6e 6963 6b6f  cense/brunonicko
-00000600: 2f62 6173 6963 636f 3f63 6f6c 6f72 3d6c  /basicco?color=l
-00000610: 6967 6874 2d67 7265 656e 0a20 2020 3a74  ight-green.   :t
-00000620: 6172 6765 743a 2068 7474 7073 3a2f 2f67  arget: https://g
-00000630: 6974 6875 622e 636f 6d2f 6272 756e 6f6e  ithub.com/brunon
-00000640: 6963 6b6f 2f62 6173 6963 636f 2f62 6c6f  icko/basicco/blo
-00000650: 622f 6d61 7374 6572 2f4c 4943 454e 5345  b/master/LICENSE
-00000660: 0a0a 2e2e 2069 6d61 6765 3a3a 2068 7474  .... image:: htt
-00000670: 7073 3a2f 2f73 7461 7469 632e 7065 7079  ps://static.pepy
-00000680: 2e74 6563 682f 7065 7273 6f6e 616c 697a  .tech/personaliz
-00000690: 6564 2d62 6164 6765 2f62 6173 6963 636f  ed-badge/basicco
-000006a0: 3f70 6572 696f 643d 746f 7461 6c26 756e  ?period=total&un
-000006b0: 6974 733d 696e 7465 726e 6174 696f 6e61  its=internationa
-000006c0: 6c5f 7379 7374 656d 266c 6566 745f 636f  l_system&left_co
-000006d0: 6c6f 723d 6772 6579 2672 6967 6874 5f63  lor=grey&right_c
-000006e0: 6f6c 6f72 3d62 7269 6768 7467 7265 656e  olor=brightgreen
-000006f0: 266c 6566 745f 7465 7874 3d44 6f77 6e6c  &left_text=Downl
-00000700: 6f61 6473 0a20 2020 3a74 6172 6765 743a  oads.   :target:
-00000710: 2068 7474 7073 3a2f 2f70 6570 792e 7465   https://pepy.te
-00000720: 6368 2f70 726f 6a65 6374 2f62 6173 6963  ch/project/basic
-00000730: 636f 0a0a 2e2e 2069 6d61 6765 3a3a 2068  co.... image:: h
-00000740: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
-00000750: 6473 2e69 6f2f 7079 7069 2f70 7976 6572  ds.io/pypi/pyver
-00000760: 7369 6f6e 732f 6261 7369 6363 6f3f 636f  sions/basicco?co
-00000770: 6c6f 723d 6c69 6768 742d 6772 6565 6e26  lor=light-green&
-00000780: 7374 796c 653d 666c 6174 0a20 2020 3a74  style=flat.   :t
-00000790: 6172 6765 743a 2068 7474 7073 3a2f 2f70  arget: https://p
-000007a0: 7970 692e 6f72 672f 7072 6f6a 6563 742f  ypi.org/project/
-000007b0: 6261 7369 6363 6f2f 0a0a 4f76 6572 7669  basicco/..Overvi
-000007c0: 6577 0a2d 2d2d 2d2d 2d2d 2d0a 6062 6173  ew.--------.`bas
-000007d0: 6963 636f 6020 6973 2061 2050 7974 686f  icco` is a Pytho
-000007e0: 6e20 7061 636b 6167 6520 7468 6174 2070  n package that p
-000007f0: 726f 7669 6465 7320 6c6f 772d 6c65 7665  rovides low-leve
-00000800: 6c20 6042 6173 6520 436c 6173 7365 7360  l `Base Classes`
-00000810: 5f20 616e 6420 6055 7469 6c69 7469 6573  _ and `Utilities
-00000820: 605f 2074 6f20 656e 6861 6e63 6520 636f  `_ to enhance co
-00000830: 6465 2063 6f6d 7061 7469 6269 6c69 7479  de compatibility
-00000840: 2c0a 6665 6174 7572 6573 2061 6e64 2076  ,.features and v
-00000850: 616c 6964 6174 696f 6e2e 0a0a 4d6f 7469  alidation...Moti
-00000860: 7661 7469 6f6e 0a2d 2d2d 2d2d 2d2d 2d2d  vation.---------
-00000870: 2d0a 5768 696c 6520 6465 7665 6c6f 7069  -.While developi
-00000880: 6e67 2050 7974 686f 6e20 736f 6674 7761  ng Python softwa
-00000890: 7265 2066 6f72 2056 6973 7561 6c20 4566  re for Visual Ef
-000008a0: 6665 6374 7320 7069 7065 6c69 6e65 732c  fects pipelines,
-000008b0: 2049 2066 6f75 6e64 206d 7973 656c 6620   I found myself 
-000008c0: 6861 7669 6e67 2074 6f20 7772 6974 6520  having to write 
-000008d0: 7468 6520 7361 6d65 2062 6f69 6c65 722d  the same boiler-
-000008e0: 706c 6174 650a 636f 6465 206f 7665 7220  plate.code over 
-000008f0: 616e 6420 6f76 6572 2061 6761 696e 2c20  and over again, 
-00000900: 6173 2077 656c 6c20 6173 2073 7472 7567  as well as strug
-00000910: 676c 696e 6720 7769 7468 2063 6f6d 7061  gling with compa
-00000920: 7469 6269 6c69 7479 2069 7373 7565 7320  tibility issues 
-00000930: 616e 6420 6665 6174 7572 6520 6761 7073  and feature gaps
-00000940: 2062 6574 7765 656e 2050 7974 686f 6e20   between Python 
-00000950: 322e 3720 616e 640a 5079 7468 6f6e 2033  2.7 and.Python 3
-00000960: 2e37 2b2e 0a0a 536f 2049 2064 6563 6964  .7+...So I decid
-00000970: 6564 2074 6f20 696d 706c 656d 656e 7420  ed to implement 
-00000980: 736f 6c75 7469 6f6e 7320 666f 7220 7468  solutions for th
-00000990: 6f73 6520 6973 7375 6573 2061 7420 7468  ose issues at th
-000009a0: 6520 6042 6173 6560 5f2c 2061 6e64 2060  e `Base`_, and `
-000009b0: 6261 7369 6363 6f60 2077 6173 2062 6f72  basicco` was bor
-000009c0: 6e2e 0a0a 4261 7365 2043 6c61 7373 6573  n...Base Classes
-000009d0: 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 0a43  .------------..C
-000009e0: 6f6d 7061 7442 6173 650a 5e5e 5e5e 5e5e  ompatBase.^^^^^^
-000009f0: 5e5e 5e5e 0a54 6865 2067 6f61 6c20 7769  ^^^^.The goal wi
-00000a00: 7468 2074 6865 2060 436f 6d70 6174 4261  th the `CompatBa
-00000a10: 7365 4d65 7461 6020 6d65 7461 636c 6173  seMeta` metaclas
-00000a20: 7320 616e 6420 7468 6520 6043 6f6d 7061  s and the `Compa
-00000a30: 7442 6173 6560 2063 6c61 7373 2069 7320  tBase` class is 
-00000a40: 746f 2062 7269 6467 6520 736f 6d65 206f  to bridge some o
-00000a50: 6620 7468 6520 6665 6174 7572 6520 6761  f the feature ga
-00000a60: 7073 2062 6574 7765 656e 0a50 7974 686f  ps between.Pytho
-00000a70: 6e20 322e 3720 616e 6420 5079 7468 6f6e  n 2.7 and Python
-00000a80: 2033 2e37 2b2e 0a0a 5468 6973 2069 6e63   3.7+...This inc
-00000a90: 6c75 6465 7320 6164 6469 6e67 2050 7974  ludes adding Pyt
-00000aa0: 686f 6e20 322e 3720 776f 726b 6172 6f75  hon 2.7 workarou
-00000ab0: 6e64 7320 666f 723a 0a20 202d 2060 4162  nds for:.  - `Ab
-00000ac0: 7374 7261 6374 2070 726f 7065 7274 6965  stract propertie
-00000ad0: 7320 3c68 7474 7073 3a2f 2f64 6f63 732e  s <https://docs.
-00000ae0: 7079 7468 6f6e 2e6f 7267 2f33 2f6c 6962  python.org/3/lib
-00000af0: 7261 7279 2f61 6263 2e68 746d 6c23 6162  rary/abc.html#ab
-00000b00: 632e 6162 7374 7261 6374 7072 6f70 6572  c.abstractproper
-00000b10: 7479 3e60 5f3a 2042 6574 7465 7220 6061  ty>`_: Better `a
-00000b20: 6273 7472 6163 746d 6574 686f 6460 0a20  bstractmethod`. 
-00000b30: 2020 2064 6563 6f72 6174 6f72 2073 7570     decorator sup
-00000b40: 706f 7274 2066 6f72 2070 726f 7065 7274  port for propert
-00000b50: 792d 6c69 6b65 2064 6573 6372 6970 746f  y-like descripto
-00000b60: 7273 2e20 5365 6520 616c 736f 2060 6162  rs. See also `ab
-00000b70: 7374 7261 6374 5f63 6c61 7373 605f 2e0a  stract_class`_..
-00000b80: 2020 2d20 6050 4550 2034 3837 203c 6874    - `PEP 487 <ht
-00000b90: 7470 733a 2f2f 7065 7073 2e70 7974 686f  tps://peps.pytho
-00000ba0: 6e2e 6f72 672f 7065 702d 3034 3837 2f3e  n.org/pep-0487/>
-00000bb0: 605f 3a20 5375 7070 6f72 7420 666f 7220  `_: Support for 
-00000bc0: 605f 5f69 6e69 745f 7375 6263 6c61 7373  `__init_subclass
-00000bd0: 5f5f 6020 616e 6420 605f 5f73 6574 5f6e  __` and `__set_n
-00000be0: 616d 655f 5f60 2e0a 2020 2020 5365 6520  ame__`..    See 
-00000bf0: 616c 736f 2060 696e 6974 5f73 7562 636c  also `init_subcl
-00000c00: 6173 7360 5f20 616e 6420 6073 6574 5f6e  ass`_ and `set_n
-00000c10: 616d 6560 5f2e 0a20 202d 2060 6f62 6a65  ame`_..  - `obje
-00000c20: 6374 2e5f 5f64 6972 5f5f 203c 6874 7470  ct.__dir__ <http
-00000c30: 733a 2f2f 646f 6373 2e70 7974 686f 6e2e  s://docs.python.
-00000c40: 6f72 672f 332f 7265 6665 7265 6e63 652f  org/3/reference/
-00000c50: 6461 7461 6d6f 6465 6c2e 6874 6d6c 236f  datamodel.html#o
-00000c60: 626a 6563 742e 5f5f 6469 725f 5f3e 605f  bject.__dir__>`_
-00000c70: 3a20 4261 7365 2060 5f5f 6469 725f 5f60  : Base `__dir__`
-00000c80: 206d 6574 686f 642e 0a20 2020 2053 6565   method..    See
-00000c90: 2061 6c73 6f20 6064 6566 6175 6c74 5f64   also `default_d
-00000ca0: 6972 605f 2e0a 2020 2d20 605f 5f65 715f  ir`_..  - `__eq_
-00000cb0: 5f20 6f76 6572 7269 6465 203c 6874 7470  _ override <http
-00000cc0: 733a 2f2f 646f 6373 2e70 7974 686f 6e2e  s://docs.python.
-00000cd0: 6f72 672f 332f 7265 6665 7265 6e63 652f  org/3/reference/
-00000ce0: 6461 7461 6d6f 6465 6c2e 6874 6d6c 236f  datamodel.html#o
-00000cf0: 626a 6563 742e 5f5f 6861 7368 5f5f 3e60  bject.__hash__>`
-00000d00: 5f3a 204f 7665 7272 6964 696e 6720 605f  _: Overriding `_
-00000d10: 5f65 715f 5f60 2077 696c 6c0a 2020 2020  _eq__` will.    
-00000d20: 7365 7420 605f 5f68 6173 685f 5f60 2074  set `__hash__` t
-00000d30: 6f20 4e6f 6e65 2e20 5365 6520 616c 736f  o None. See also
-00000d40: 2060 696d 706c 6963 6974 5f68 6173 6860   `implicit_hash`
-00000d50: 5f2e 0a20 202d 2060 5045 5020 3330 3720  _..  - `PEP 307 
-00000d60: 3c68 7474 7073 3a2f 2f70 6570 732e 7079  <https://peps.py
-00000d70: 7468 6f6e 2e6f 7267 2f70 6570 2d30 3330  thon.org/pep-030
-00000d80: 372f 3e60 5f3a 2053 7570 706f 7274 2066  7/>`_: Support f
-00000d90: 6f72 2070 6963 6b6c 696e 6720 6f62 6a65  or pickling obje
-00000da0: 6374 7320 7769 7468 2060 5f5f 736c 6f74  cts with `__slot
-00000db0: 735f 5f60 2e0a 2020 2020 5365 6520 616c  s__`..    See al
-00000dc0: 736f 2060 6f62 6a5f 7374 6174 6560 5f2e  so `obj_state`_.
-00000dd0: 0a20 202d 2060 5045 5020 3331 3535 203c  .  - `PEP 3155 <
-00000de0: 6874 7470 733a 2f2f 7065 7073 2e70 7974  https://peps.pyt
-00000df0: 686f 6e2e 6f72 672f 7065 702d 3033 3135  hon.org/pep-0315
-00000e00: 352f 3e60 5f3a 2051 7561 6c69 6669 6564  5/>`_: Qualified
-00000e10: 206e 616d 6520 605f 5f71 7561 6c6e 616d   name `__qualnam
-00000e20: 655f 5f60 2066 6f72 206e 6573 7465 6420  e__` for nested 
-00000e30: 636c 6173 7365 732e 0a20 2020 2053 6565  classes..    See
-00000e40: 2061 6c73 6f20 6071 7561 6c6e 616d 6560   also `qualname`
-00000e50: 5f2e 0a20 202d 2060 5f5f 6e65 5f5f 2062  _..  - `__ne__ b
-00000e60: 6568 6176 696f 7220 3c68 7474 7073 3a2f  ehavior <https:/
-00000e70: 2f64 6f63 732e 7079 7468 6f6e 2e6f 7267  /docs.python.org
-00000e80: 2f33 2e30 2f77 6861 7473 6e65 772f 332e  /3.0/whatsnew/3.
-00000e90: 302e 6874 6d6c 236f 7065 7261 746f 7273  0.html#operators
-00000ea0: 2d61 6e64 2d73 7065 6369 616c 2d6d 6574  -and-special-met
-00000eb0: 686f 6473 3e60 5f3a 2042 7920 6465 6661  hods>`_: By defa
-00000ec0: 756c 742c 0a20 2020 2060 5f5f 6e65 5f5f  ult,.    `__ne__
-00000ed0: 6020 7368 6f75 6c64 206e 6567 6174 6520  ` should negate 
-00000ee0: 7468 6520 7265 7375 6c74 206f 6620 605f  the result of `_
-00000ef0: 5f65 715f 5f60 2e0a 2020 2020 5365 6520  _eq__`..    See 
-00000f00: 616c 736f 2060 7361 6665 5f6e 6f74 5f65  also `safe_not_e
-00000f10: 7175 616c 7360 5f0a 2020 2d20 6050 4550  quals`_.  - `PEP
-00000f20: 2030 3536 3020 3c68 7474 7073 3a2f 2f70   0560 <https://p
-00000f30: 6570 732e 7079 7468 6f6e 2e6f 7267 2f70  eps.python.org/p
-00000f40: 6570 2d30 3536 302f 3e60 5f3a 2042 6574  ep-0560/>`_: Bet
-00000f50: 7465 7220 6861 6e64 6c69 6e67 206f 6620  ter handling of 
-00000f60: 4765 6e65 7269 6320 636c 6173 7365 732e  Generic classes.
-00000f70: 0a20 2020 2053 6565 2061 6c73 6f20 6074  .    See also `t
-00000f80: 6970 706f 203c 6874 7470 733a 2f2f 6769  ippo <https://gi
-00000f90: 7468 7562 2e63 6f6d 2f62 7275 6e6f 6e69  thub.com/brunoni
-00000fa0: 636b 6f2f 7469 7070 6f23 6765 6e65 7269  cko/tippo#generi
-00000fb0: 632d 6669 7865 733e 605f 2e0a 0a42 6173  c-fixes>`_...Bas
-00000fc0: 650a 5e5e 5e5e 0a49 6e20 6164 6469 7469  e.^^^^.In additi
-00000fd0: 6f6e 2074 6f20 7468 6520 636f 6d70 6174  on to the compat
-00000fe0: 6962 696c 6974 7920 736f 6c75 7469 6f6e  ibility solution
-00000ff0: 732c 2074 6865 2067 6f61 6c20 7769 7468  s, the goal with
-00001000: 2074 6865 2060 4261 7365 4d65 7461 6020   the `BaseMeta` 
-00001010: 6d65 7461 636c 6173 7320 616e 6420 7468  metaclass and th
-00001020: 6520 6042 6173 6560 2063 6c61 7373 2069  e `Base` class i
-00001030: 7320 746f 2061 6464 0a75 7365 6675 6c20  s to add.useful 
-00001040: 6c6f 772d 6c65 7665 6c20 6665 6174 7572  low-level featur
-00001050: 6573 2074 6861 7420 686f 7065 6675 6c6c  es that hopefull
-00001060: 7920 7969 656c 6420 6265 7474 6572 2063  y yield better c
-00001070: 6f64 6520 7265 6164 6162 696c 6974 7920  ode readability 
-00001080: 616e 6420 7661 6c69 6461 7469 6f6e 2e0a  and validation..
-00001090: 0a54 6869 7320 696e 636c 7564 6573 3a0a  .This includes:.
-000010a0: 2020 2d20 605f 5f77 6561 6b72 6566 5f5f    - `__weakref__
-000010b0: 6020 736c 6f74 3a20 4164 6465 6420 6279  ` slot: Added by
-000010c0: 2064 6566 6175 6c74 2e0a 2020 2d20 606c   default..  - `l
-000010d0: 6f63 6b65 645f 636c 6173 7360 5f3a 2050  ocked_class`_: P
-000010e0: 7562 6c69 6320 636c 6173 7320 6174 7472  ublic class attr
-000010f0: 6962 7574 6573 2061 7265 2072 6561 642d  ibutes are read-
-00001100: 6f6e 6c79 2062 7920 6465 6661 756c 742e  only by default.
-00001110: 0a20 202d 2060 6578 706c 6963 6974 5f68  .  - `explicit_h
-00001120: 6173 6860 5f3a 204f 7665 7272 6964 696e  ash`_: Overridin
-00001130: 6720 605f 5f65 715f 5f60 2077 6974 686f  g `__eq__` witho
-00001140: 7574 206f 7665 7272 6964 696e 6720 605f  ut overriding `_
-00001150: 5f68 6173 685f 5f60 2077 696c 6c20 7261  _hash__` will ra
-00001160: 6973 6520 616e 2065 7272 6f72 2e0a 2020  ise an error..  
-00001170: 2d20 606e 616d 6573 7061 6365 605f 3a20  - `namespace`_: 
-00001180: 4164 6473 2061 2070 726f 7465 6374 6564  Adds a protected
-00001190: 2060 5f5f 6e61 6d65 7370 6163 6560 2075   `__namespace` u
-000011a0: 6e69 7175 6520 746f 2065 6163 6820 636c  nique to each cl
-000011b0: 6173 732e 0a20 202d 2060 7275 6e74 696d  ass..  - `runtim
-000011c0: 655f 6669 6e61 6c60 5f3a 2052 756e 7469  e_final`_: Runti
-000011d0: 6d65 2063 6865 636b 696e 6720 666f 7220  me checking for 
-000011e0: 636c 6173 7365 7320 616e 6420 6d65 7468  classes and meth
-000011f0: 6f64 7320 6465 636f 7261 7465 6420 7769  ods decorated wi
-00001200: 7468 2060 6669 6e61 6c60 2e0a 0a53 6c6f  th `final`...Slo
-00001210: 7474 6564 4261 7365 0a5e 5e5e 5e5e 5e5e  ttedBase.^^^^^^^
-00001220: 5e5e 5e5e 0a54 6865 2060 536c 6f74 7465  ^^^^.The `Slotte
-00001230: 6442 6173 6560 2063 6c61 7373 2061 6e64  dBase` class and
-00001240: 2074 6865 2060 536c 6f74 7465 6442 6173   the `SlottedBas
-00001250: 654d 6574 6160 206d 6574 6163 6c61 7373  eMeta` metaclass
-00001260: 206f 6666 6572 2061 6c6c 2066 6561 7475   offer all featu
-00001270: 7265 7320 6672 6f6d 2060 4261 7365 6020  res from `Base` 
-00001280: 616e 6420 6042 6173 654d 6574 6160 2070  and `BaseMeta` p
-00001290: 6c75 7320 696d 706c 6963 6974 0a60 5f5f  lus implicit.`__
-000012a0: 736c 6f74 735f 5f60 2064 6563 6c61 7261  slots__` declara
-000012b0: 7469 6f6e 2e20 5365 6520 6073 6c6f 7474  tion. See `slott
-000012c0: 6564 203c 6874 7470 733a 2f2f 6769 7468  ed <https://gith
-000012d0: 7562 2e63 6f6d 2f62 7275 6e6f 6e69 636b  ub.com/brunonick
-000012e0: 6f2f 736c 6f74 7465 643e 605f 2066 6f72  o/slotted>`_ for
-000012f0: 206d 6f72 6520 696e 666f 726d 6174 696f   more informatio
-00001300: 6e2e 0a0a 5574 696c 6974 6965 730a 2d2d  n...Utilities.--
-00001310: 2d2d 2d2d 2d2d 2d0a 4170 6172 7420 6672  -------.Apart fr
-00001320: 6f6d 2074 6865 2066 6561 7475 7265 7320  om the features 
-00001330: 696e 7465 6772 6174 6564 2069 6e74 6f20  integrated into 
-00001340: 7468 6520 6261 7365 2063 6c61 7373 6573  the base classes
-00001350: 2c20 6062 6173 6963 636f 6020 7072 6f76  , `basicco` prov
-00001360: 6964 6573 2061 2076 6172 6965 7479 206f  ides a variety o
-00001370: 6620 6765 6e65 7261 6c20 7574 696c 6974  f general utilit
-00001380: 6965 732e 0a54 686f 7365 2063 616e 2062  ies..Those can b
-00001390: 6520 696d 706f 7274 6564 2066 726f 6d20  e imported from 
-000013a0: 7468 6520 7375 622d 6d6f 6475 6c65 7320  the sub-modules 
-000013b0: 6465 7363 7269 6265 6420 6265 6c6f 772e  described below.
-000013c0: 0a0a 6162 7374 7261 6374 5f63 6c61 7373  ..abstract_class
-000013d0: 0a5e 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e 5e0a  .^^^^^^^^^^^^^^.
-000013e0: 4265 7474 6572 2060 6162 7374 7261 6374  Better `abstract
-000013f0: 2063 6c61 7373 6573 203c 6874 7470 733a   classes <https:
-00001400: 2f2f 646f 6373 2e70 7974 686f 6e2e 6f72  //docs.python.or
-00001410: 672f 332f 6c69 6272 6172 792f 6162 632e  g/3/library/abc.
-00001420: 6874 6d6c 2361 6263 2e61 6273 7472 6163  html#abc.abstrac
-00001430: 746d 6574 686f 643e 605f 2073 7570 706f  tmethod>`_ suppo
-00001440: 7274 2e0a 0a50 726f 7669 6465 7320 6162  rt...Provides ab
-00001450: 7374 7261 6374 2064 6563 6f72 6174 6f72  stract decorator
-00001460: 7320 7468 6174 2063 616e 2062 6520 7573  s that can be us
-00001470: 6564 2064 6972 6563 746c 7920 6f6e 206d  ed directly on m
-00001480: 6574 686f 6473 2062 7574 2061 6c73 6f20  ethods but also 
-00001490: 6f6e 2063 6c61 7373 6573 2c20 7072 6f70  on classes, prop
-000014a0: 6572 7469 6573 2c20 636c 6173 736d 6574  erties, classmet
-000014b0: 686f 6473 2c20 616e 640a 7374 6174 6963  hods, and.static
-000014c0: 6d65 7468 6f64 7320 2865 7665 6e20 696e  methods (even in
-000014d0: 2050 7974 686f 6e20 322e 3729 2e0a 0a2e   Python 2.7)....
-000014e0: 2e20 636f 6465 3a3a 2070 7974 686f 6e0a  . code:: python.
-000014f0: 0a20 2020 203e 3e3e 2066 726f 6d20 7369  .    >>> from si
-00001500: 7820 696d 706f 7274 2077 6974 685f 6d65  x import with_me
-00001510: 7461 636c 6173 730a 2020 2020 3e3e 3e20  taclass.    >>> 
-00001520: 6672 6f6d 2062 6173 6963 636f 2e61 6273  from basicco.abs
-00001530: 7472 6163 745f 636c 6173 7320 696d 706f  tract_class impo
-00001540: 7274 2041 6273 7472 6163 744d 6574 612c  rt AbstractMeta,
-00001550: 2061 6273 7472 6163 740a 2020 2020 3e3e   abstract.    >>
-00001560: 3e20 636c 6173 7320 4173 7365 7428 7769  > class Asset(wi
-00001570: 7468 5f6d 6574 6163 6c61 7373 2841 6273  th_metaclass(Abs
-00001580: 7472 6163 744d 6574 612c 206f 626a 6563  tractMeta, objec
-00001590: 7429 293a 0a20 2020 202e 2e2e 2020 2020  t)):.    ...    
-000015a0: 2040 6162 7374 7261 6374 0a20 2020 202e   @abstract.    .
-000015b0: 2e2e 2020 2020 2064 6566 206d 6574 686f  ..     def metho
-000015c0: 6428 7365 6c66 293a 0a20 2020 202e 2e2e  d(self):.    ...
-000015d0: 2020 2020 2020 2020 2070 6173 730a 2020           pass.  
-000015e0: 2020 2e2e 2e0a 2020 2020 2e2e 2e20 2020    ....    ...   
-000015f0: 2020 4070 726f 7065 7274 790a 2020 2020    @property.    
-00001600: 2e2e 2e20 2020 2020 4061 6273 7472 6163  ...     @abstrac
-00001610: 740a 2020 2020 2e2e 2e20 2020 2020 6465  t.    ...     de
-00001620: 6620 7072 6f70 2873 656c 6629 3a0a 2020  f prop(self):.  
-00001630: 2020 2e2e 2e20 2020 2020 2020 2020 7265    ...         re
-00001640: 7475 726e 204e 6f6e 650a 2020 2020 2e2e  turn None.    ..
-00001650: 2e0a 2020 2020 3e3e 3e20 4173 7365 7428  ..    >>> Asset(
-00001660: 290a 2020 2020 5472 6163 6562 6163 6b20  ).    Traceback 
-00001670: 286d 6f73 7420 7265 6365 6e74 2063 616c  (most recent cal
-00001680: 6c20 6c61 7374 293a 0a20 2020 2054 7970  l last):.    Typ
-00001690: 6545 7272 6f72 3a20 4361 6e27 7420 696e  eError: Can't in
-000016a0: 7374 616e 7469 6174 6520 6162 7374 7261  stantiate abstra
-000016b0: 6374 2063 6c61 7373 2041 7373 6574 2077  ct class Asset w
-000016c0: 6974 6820 6162 7374 7261 6374 206d 6574  ith abstract met
-000016d0: 686f 6473 206d 6574 686f 642c 2070 726f  hods method, pro
-000016e0: 700a 0a2e 2e20 636f 6465 3a3a 2070 7974  p.... code:: pyt
-000016f0: 686f 6e0a 0a20 2020 203e 3e3e 2066 726f  hon..    >>> fro
-00001700: 6d20 6261 7369 6363 6f2e 6162 7374 7261  m basicco.abstra
-00001710: 6374 5f63 6c61 7373 2069 6d70 6f72 7420  ct_class import 
-00001720: 4162 7374 7261 6374 4d65 7461 2c20 6162  AbstractMeta, ab
-00001730: 7374 7261 6374 0a20 2020 203e 3e3e 2040  stract.    >>> @
-00001740: 6162 7374 7261 6374 0a20 2020 202e 2e2e  abstract.    ...
-00001750: 2063 6c61 7373 2041 7373 6574 2877 6974   class Asset(wit
-00001760: 685f 6d65 7461 636c 6173 7328 4162 7374  h_metaclass(Abst
-00001770: 7261 6374 4d65 7461 2c20 6f62 6a65 6374  ractMeta, object
-00001780: 2929 3a0a 2020 2020 2e2e 2e20 2020 2020  )):.    ...     
-00001790: 7061 7373 0a20 2020 202e 2e2e 0a20 2020  pass.    ....   
-000017a0: 203e 3e3e 2041 7373 6574 2829 0a20 2020   >>> Asset().   
-000017b0: 2054 7261 6365 6261 636b 2028 6d6f 7374   Traceback (most
-000017c0: 2072 6563 656e 7420 6361 6c6c 206c 6173   recent call las
-000017d0: 7429 3a0a 2020 2020 5479 7065 4572 726f  t):.    TypeErro
-000017e0: 723a 2063 616e 2774 2069 6e73 7461 6e74  r: can't instant
-000017f0: 6961 7465 2061 6273 7472 6163 7420 636c  iate abstract cl
-00001800: 6173 7320 2741 7373 6574 270a 0a62 6173  ass 'Asset'..bas
-00001810: 6963 5f64 6174 610a 5e5e 5e5e 5e5e 5e5e  ic_data.^^^^^^^^
-00001820: 5e5e 0a45 6173 6573 2074 6865 2074 6173  ^^.Eases the tas
-00001830: 6b20 6f66 2063 7265 6174 696e 6720 7369  k of creating si
-00001840: 6d70 6c65 2064 6174 6120 636f 6e74 6169  mple data contai
-00001850: 6e65 7220 636c 6173 7365 7320 7468 6174  ner classes that
-00001860: 2073 7570 706f 7274 2065 7175 616c 6974   support equalit
-00001870: 7920 636f 6d70 6172 6973 6f6e 732c 2068  y comparisons, h
-00001880: 6173 6869 6e67 2c20 7374 7269 6e67 0a72  ashing, string.r
-00001890: 6570 7265 7365 6e74 6174 696f 6e2c 2063  epresentation, c
-000018a0: 6f6e 7665 7273 696f 6e20 746f 2064 6963  onversion to dic
-000018b0: 7469 6f6e 6172 792c 2065 7463 2e0a 0a2e  tionary, etc....
-000018c0: 2e20 636f 6465 3a3a 2070 7974 686f 6e0a  . code:: python.
-000018d0: 0a20 2020 203e 3e3e 2066 726f 6d20 6d61  .    >>> from ma
-000018e0: 7468 2069 6d70 6f72 7420 7371 7274 0a20  th import sqrt. 
-000018f0: 2020 203e 3e3e 2066 726f 6d20 6261 7369     >>> from basi
-00001900: 6363 6f2e 6261 7369 635f 6461 7461 2069  cco.basic_data i
-00001910: 6d70 6f72 7420 4974 656d 5573 6563 6173  mport ItemUsecas
-00001920: 652c 2042 6173 6963 4461 7461 0a20 2020  e, BasicData.   
-00001930: 203e 3e3e 2063 6c61 7373 2056 6563 746f   >>> class Vecto
-00001940: 7228 4261 7369 6344 6174 6129 3a0a 2020  r(BasicData):.  
-00001950: 2020 2e2e 2e20 2020 2020 5f5f 736c 6f74    ...     __slot
-00001960: 735f 5f20 3d20 2822 7822 2c20 2279 2229  s__ = ("x", "y")
-00001970: 0a20 2020 202e 2e2e 2020 2020 2064 6566  .    ...     def
-00001980: 205f 5f69 6e69 745f 5f28 7365 6c66 2c20   __init__(self, 
-00001990: 782c 2079 293a 0a20 2020 202e 2e2e 2020  x, y):.    ...  
-000019a0: 2020 2020 2020 2073 656c 662e 7820 3d20         self.x = 
-000019b0: 780a 2020 2020 2e2e 2e20 2020 2020 2020  x.    ...       
-000019c0: 2020 7365 6c66 2e79 203d 2079 0a20 2020    self.y = y.   
-000019d0: 202e 2e2e 2020 2020 2064 6566 2074 6f5f   ...     def to_
-000019e0: 6974 656d 7328 7365 6c66 2c20 7573 6563  items(self, usec
-000019f0: 6173 653d 4e6f 6e65 293a 0a20 2020 202e  ase=None):.    .
-00001a00: 2e2e 2020 2020 2020 2020 2069 7465 6d73  ..         items
-00001a10: 203d 205b 2822 7822 2c20 7365 6c66 2e78   = [("x", self.x
-00001a20: 292c 2028 2279 222c 2073 656c 662e 7929  ), ("y", self.y)
-00001a30: 5d0a 2020 2020 2e2e 2e20 2020 2020 2020  ].    ...       
-00001a40: 2020 6966 2075 7365 6361 7365 2069 7320    if usecase is 
-00001a50: 4974 656d 5573 6563 6173 652e 5245 5052  ItemUsecase.REPR
-00001a60: 3a0a 2020 2020 2e2e 2e20 2020 2020 2020  :.    ...       
-00001a70: 2020 2020 2020 6974 656d 732e 6170 7065        items.appe
-00001a80: 6e64 2828 226d 6167 222c 2073 656c 662e  nd(("mag", self.
-00001a90: 6d61 6729 290a 2020 2020 2e2e 2e20 2020  mag)).    ...   
-00001aa0: 2020 2020 2020 7265 7475 726e 2069 7465        return ite
-00001ab0: 6d73 0a20 2020 202e 2e2e 2020 2020 2040  ms.    ...     @
-00001ac0: 7072 6f70 6572 7479 0a20 2020 202e 2e2e  property.    ...
-00001ad0: 2020 2020 2064 6566 206d 6167 2873 656c       def mag(sel
-00001ae0: 6629 3a0a 2020 2020 2e2e 2e20 2020 2020  f):.    ...     
-00001af0: 2020 2020 7265 7475 726e 2073 7172 7428      return sqrt(
-00001b00: 7365 6c66 2e78 2a2a 3220 2b20 7365 6c66  self.x**2 + self
-00001b10: 2e79 2a2a 3229 0a20 2020 202e 2e2e 0a20  .y**2).    .... 
-00001b20: 2020 203e 3e3e 2056 6563 746f 7228 332e     >>> Vector(3.
-00001b30: 302c 2034 2e30 290a 2020 2020 5665 6374  0, 4.0).    Vect
-00001b40: 6f72 2878 3d33 2e30 2c20 793d 342e 302c  or(x=3.0, y=4.0,
-00001b50: 203c 6d61 673d 352e 303e 290a 0a63 616c   <mag=5.0>)..cal
-00001b60: 6c65 725f 6d6f 6475 6c65 0a5e 5e5e 5e5e  ler_module.^^^^^
-00001b70: 5e5e 5e5e 5e5e 5e5e 0a52 6574 7269 6576  ^^^^^^^^.Retriev
-00001b80: 6520 7468 6520 6361 6c6c 6572 2773 206d  e the caller's m
-00001b90: 6f64 756c 6520 6e61 6d65 2e0a 0a2e 2e20  odule name..... 
-00001ba0: 636f 6465 3a3a 2070 7974 686f 6e0a 0a20  code:: python.. 
-00001bb0: 2020 203e 3e3e 2066 726f 6d20 6261 7369     >>> from basi
-00001bc0: 6363 6f2e 6361 6c6c 6572 5f6d 6f64 756c  cco.caller_modul
-00001bd0: 6520 696d 706f 7274 2063 616c 6c65 725f  e import caller_
-00001be0: 6d6f 6475 6c65 0a20 2020 203e 3e3e 2064  module.    >>> d
-00001bf0: 6566 2064 6f5f 736f 6d65 7468 696e 6728  ef do_something(
-00001c00: 293a 0a20 2020 202e 2e2e 2020 2020 2072  ):.    ...     r
-00001c10: 6574 7572 6e20 2249 2077 6173 2063 616c  eturn "I was cal
-00001c20: 6c65 6420 6279 207b 7d22 2e66 6f72 6d61  led by {}".forma
-00001c30: 7428 6361 6c6c 6572 5f6d 6f64 756c 6528  t(caller_module(
-00001c40: 2929 0a20 2020 202e 2e2e 0a20 2020 203e  )).    ....    >
-00001c50: 3e3e 2064 6f5f 736f 6d65 7468 696e 6728  >> do_something(
-00001c60: 290a 2020 2020 2749 2077 6173 2063 616c  ).    'I was cal
-00001c70: 6c65 6420 6279 205f 5f6d 6169 6e5f 5f27  led by __main__'
-00001c80: 0a0a 636f 6e74 6578 745f 7661 7273 0a5e  ..context_vars.^
-00001c90: 5e5e 5e5e 5e5e 5e5e 5e5e 5e0a 4261 636b  ^^^^^^^^^^^.Back
-00001ca0: 706f 7274 206f 6620 7468 6520 6063 6f6e  port of the `con
-00001cb0: 7465 7874 7661 7273 6020 6d6f 6475 6c65  textvars` module
-00001cc0: 2066 6f72 2050 7974 686f 6e20 322e 372c   for Python 2.7,
-00001cd0: 2062 6173 6564 206f 6e0a 604d 6167 6963   based on.`Magic
-00001ce0: 5374 6163 6b2f 636f 6e74 6578 7476 6172  Stack/contextvar
-00001cf0: 7320 3c68 7474 7073 3a2f 2f67 6974 6875  s <https://githu
-00001d00: 622e 636f 6d2f 4d61 6769 6353 7461 636b  b.com/MagicStack
-00001d10: 2f63 6f6e 7465 7874 7661 7273 3e60 5f2e  /contextvars>`_.
-00001d20: 0a0a 5768 656e 2069 6d70 6f72 7465 6420  ..When imported 
-00001d30: 6672 6f6d 2050 7974 686f 6e20 332c 2069  from Python 3, i
-00001d40: 7420 7265 6469 7265 6374 7320 7468 6520  t redirects the 
-00001d50: 636f 6e74 656e 7473 2074 6f20 7468 6520  contents to the 
-00001d60: 6e61 7469 7665 0a60 636f 6e74 6578 7476  native.`contextv
-00001d70: 6172 7320 3c68 7474 7073 3a2f 2f64 6f63  ars <https://doc
-00001d80: 732e 7079 7468 6f6e 2e6f 7267 2f33 2f6c  s.python.org/3/l
-00001d90: 6962 7261 7279 2f63 6f6e 7465 7874 7661  ibrary/contextva
-00001da0: 7273 2e68 746d 6c3e 605f 206d 6f64 756c  rs.html>`_ modul
-00001db0: 652e 0a0a 2e2e 2063 6f64 653a 3a20 7079  e..... code:: py
-00001dc0: 7468 6f6e 0a0a 2020 2020 3e3e 3e20 6672  thon..    >>> fr
-00001dd0: 6f6d 2062 6173 6963 636f 2e63 6f6e 7465  om basicco.conte
-00001de0: 7874 5f76 6172 7320 696d 706f 7274 2043  xt_vars import C
-00001df0: 6f6e 7465 7874 5661 720a 2020 2020 3e3e  ontextVar.    >>
-00001e00: 3e20 6d79 5f76 6172 203d 2043 6f6e 7465  > my_var = Conte
-00001e10: 7874 5661 7228 226d 795f 7661 7222 2c20  xtVar("my_var", 
-00001e20: 6465 6661 756c 743d 2262 6172 2229 0a20  default="bar"). 
-00001e30: 2020 203e 3e3e 2074 6f6b 656e 203d 206d     >>> token = m
-00001e40: 795f 7661 722e 7365 7428 2266 6f6f 2229  y_var.set("foo")
-00001e50: 0a20 2020 203e 3e3e 206d 795f 7661 722e  .    >>> my_var.
-00001e60: 6765 7428 290a 2020 2020 2766 6f6f 270a  get().    'foo'.
-00001e70: 2020 2020 3e3e 3e20 6d79 5f76 6172 2e72      >>> my_var.r
-00001e80: 6573 6574 2874 6f6b 656e 290a 2020 2020  eset(token).    
-00001e90: 3e3e 3e20 6d79 5f76 6172 2e67 6574 2829  >>> my_var.get()
-00001ea0: 0a20 2020 2027 6261 7227 0a0a 6375 7374  .    'bar'..cust
-00001eb0: 6f6d 5f72 6570 720a 5e5e 5e5e 5e5e 5e5e  om_repr.^^^^^^^^
-00001ec0: 5e5e 5e0a 4375 7374 6f6d 2072 6570 7265  ^^^.Custom repre
-00001ed0: 7365 6e74 6174 696f 6e20 6675 6e63 7469  sentation functi
-00001ee0: 6f6e 7320 666f 7220 6d61 7070 696e 6773  ons for mappings
-00001ef0: 2c20 6974 656d 732c 2061 6e64 2069 7465  , items, and ite
-00001f00: 7261 626c 6573 2e0a 0a2e 2e20 636f 6465  rables..... code
-00001f10: 3a3a 2070 7974 686f 6e0a 0a20 2020 203e  :: python..    >
-00001f20: 3e3e 2066 726f 6d20 6261 7369 6363 6f2e  >> from basicco.
-00001f30: 6375 7374 6f6d 5f72 6570 7220 696d 706f  custom_repr impo
-00001f40: 7274 206d 6170 7069 6e67 5f72 6570 720a  rt mapping_repr.
-00001f50: 2020 2020 3e3e 3e20 6463 7420 3d20 7b22      >>> dct = {"
-00001f60: 6122 3a20 312c 2022 6222 3a20 327d 0a20  a": 1, "b": 2}. 
-00001f70: 2020 203e 3e3e 206d 6170 7069 6e67 5f72     >>> mapping_r
-00001f80: 6570 7228 6463 742c 2070 7265 6669 783d  epr(dct, prefix=
-00001f90: 223c 222c 2073 7566 6669 783d 223e 222c  "<", suffix=">",
-00001fa0: 2074 656d 706c 6174 653d 227b 6b65 797d   template="{key}
-00001fb0: 3d7b 7661 6c75 657d 222c 2073 6f72 7469  ={value}", sorti
-00001fc0: 6e67 3d54 7275 6529 0a20 2020 2022 3c27  ng=True).    "<'
-00001fd0: 6127 3d31 2c20 2762 273d 323e 220a 0a2e  a'=1, 'b'=2>"...
-00001fe0: 2e20 636f 6465 3a3a 2070 7974 686f 6e0a  . code:: python.
-00001ff0: 0a20 2020 203e 3e3e 2066 726f 6d20 6261  .    >>> from ba
-00002000: 7369 6363 6f2e 6375 7374 6f6d 5f72 6570  sicco.custom_rep
-00002010: 7220 696d 706f 7274 206d 6170 7069 6e67  r import mapping
-00002020: 5f72 6570 720a 2020 2020 3e3e 3e20 6974  _repr.    >>> it
-00002030: 656d 7320 3d20 5b28 2261 222c 2031 292c  ems = [("a", 1),
-00002040: 2028 2262 222c 2032 295d 0a20 2020 203e   ("b", 2)].    >
-00002050: 3e3e 206d 6170 7069 6e67 5f72 6570 7228  >> mapping_repr(
-00002060: 6974 656d 732c 2070 7265 6669 783d 225b  items, prefix="[
-00002070: 222c 2073 7566 6669 783d 225d 222c 2074  ", suffix="]", t
-00002080: 656d 706c 6174 653d 6c61 6d62 6461 2069  emplate=lambda i
-00002090: 2c20 6b65 792c 2076 616c 7565 3a20 6b65  , key, value: ke
-000020a0: 7920 2b20 2220 2d3e 2022 202b 2076 616c  y + " -> " + val
-000020b0: 7565 290a 2020 2020 225b 2761 2720 2d3e  ue).    "['a' ->
-000020c0: 2031 2c20 2762 2720 2d3e 2032 5d22 0a0a   1, 'b' -> 2]"..
-000020d0: 2e2e 2063 6f64 653a 3a20 7079 7468 6f6e  .. code:: python
-000020e0: 0a0a 2020 2020 3e3e 3e20 6672 6f6d 2062  ..    >>> from b
-000020f0: 6173 6963 636f 2e63 7573 746f 6d5f 7265  asicco.custom_re
-00002100: 7072 2069 6d70 6f72 7420 6974 6572 6162  pr import iterab
-00002110: 6c65 5f72 6570 720a 2020 2020 3e3e 3e20  le_repr.    >>> 
-00002120: 7475 7020 3d20 2822 6122 2c20 2262 222c  tup = ("a", "b",
-00002130: 2022 6322 2c20 312c 2032 2c20 3329 0a20   "c", 1, 2, 3). 
-00002140: 2020 203e 3e3e 2069 7465 7261 626c 655f     >>> iterable_
-00002150: 7265 7072 2874 7570 2c20 7072 6566 6978  repr(tup, prefix
-00002160: 3d22 3c22 2c20 7375 6666 6978 3d22 3e22  ="<", suffix=">"
-00002170: 2c20 7661 6c75 655f 7265 7072 3d73 7472  , value_repr=str
-00002180: 290a 2020 2020 273c 612c 2062 2c20 632c  ).    '<a, b, c,
-00002190: 2031 2c20 322c 2033 3e27 0a0a 6465 6661   1, 2, 3>'..defa
-000021a0: 756c 745f 6469 720a 5e5e 5e5e 5e5e 5e5e  ult_dir.^^^^^^^^
-000021b0: 5e5e 5e0a 4261 636b 706f 7274 206f 6620  ^^^.Backport of 
-000021c0: 5079 7468 6f6e 2033 2773 2069 6d70 6c65  Python 3's imple
-000021d0: 6d65 6e74 6174 696f 6e20 6f66 0a60 6f62  mentation of.`ob
-000021e0: 6a65 6374 2e5f 5f64 6972 5f5f 203c 6874  ject.__dir__ <ht
-000021f0: 7470 733a 2f2f 646f 6373 2e70 7974 686f  tps://docs.pytho
-00002200: 6e2e 6f72 672f 332f 7265 6665 7265 6e63  n.org/3/referenc
-00002210: 652f 6461 7461 6d6f 6465 6c2e 6874 6d6c  e/datamodel.html
-00002220: 236f 626a 6563 742e 5f5f 6469 725f 5f3e  #object.__dir__>
-00002230: 605f 2066 6f72 2050 7974 686f 6e20 322e  `_ for Python 2.
-00002240: 372e 0a0a 5468 6973 2061 6c6c 6f77 7320  7...This allows 
-00002250: 666f 7220 6361 6c6c 696e 6720 6073 7570  for calling `sup
-00002260: 6572 2829 2e5f 5f64 6972 5f5f 2829 6020  er().__dir__()` 
-00002270: 6672 6f6d 2061 2073 7562 636c 6173 7320  from a subclass 
-00002280: 746f 206c 6576 6572 6167 6520 7468 6520  to leverage the 
-00002290: 6465 6661 756c 7420 696d 706c 656d 656e  default implemen
-000022a0: 7461 7469 6f6e 2e0a 0a2e 2e20 636f 6465  tation..... code
-000022b0: 3a3a 2070 7974 686f 6e0a 0a20 2020 203e  :: python..    >
-000022c0: 3e3e 2066 726f 6d20 7369 7820 696d 706f  >> from six impo
-000022d0: 7274 2077 6974 685f 6d65 7461 636c 6173  rt with_metaclas
-000022e0: 730a 2020 2020 3e3e 3e20 6672 6f6d 2062  s.    >>> from b
-000022f0: 6173 6963 636f 2e64 6566 6175 6c74 5f64  asicco.default_d
-00002300: 6972 2069 6d70 6f72 7420 4465 6661 756c  ir import Defaul
-00002310: 7444 6972 0a20 2020 203e 3e3e 2063 6c61  tDir.    >>> cla
-00002320: 7373 2043 6c61 7373 2844 6566 6175 6c74  ss Class(Default
-00002330: 4469 7229 3a0a 2020 2020 2e2e 2e20 2020  Dir):.    ...   
-00002340: 2020 6465 6620 5f5f 6469 725f 5f28 7365    def __dir__(se
-00002350: 6c66 293a 0a20 2020 202e 2e2e 2020 2020  lf):.    ...    
-00002360: 2020 2020 2072 6574 7572 6e20 7375 7065       return supe
-00002370: 7228 436c 6173 732c 2073 656c 6629 2e5f  r(Class, self)._
-00002380: 5f64 6972 5f5f 2829 0a20 2020 202e 2e2e  _dir__().    ...
-00002390: 0a20 2020 203e 3e3e 206f 626a 203d 2043  .    >>> obj = C
-000023a0: 6c61 7373 2829 0a20 2020 203e 3e3e 2064  lass().    >>> d
-000023b0: 6972 286f 626a 290a 2020 2020 5b2e 2e2e  ir(obj).    [...
-000023c0: 5d0a 0a64 796e 616d 6963 5f63 6f64 650a  ]..dynamic_code.
-000023d0: 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e 0a47 656e  ^^^^^^^^^^^^.Gen
-000023e0: 6572 6174 6520 6465 6275 6767 6162 6c65  erate debuggable
-000023f0: 2063 6f64 6520 6f6e 2074 6865 2066 6c79   code on the fly
-00002400: 2074 6861 7420 7375 7070 6f72 7473 206c   that supports l
-00002410: 696e 6520 6e75 6d62 6572 7320 6f6e 2074  ine numbers on t
-00002420: 7261 6365 6261 636b 732e 0a0a 2e2e 2063  racebacks..... c
-00002430: 6f64 653a 3a20 7079 7468 6f6e 0a0a 2020  ode:: python..  
-00002440: 2020 3e3e 3e20 6672 6f6d 2062 6173 6963    >>> from basic
-00002450: 636f 2e64 796e 616d 6963 5f63 6f64 6520  co.dynamic_code 
-00002460: 696d 706f 7274 206d 616b 655f 6675 6e63  import make_func
-00002470: 7469 6f6e 2c20 6765 6e65 7261 7465 5f75  tion, generate_u
-00002480: 6e69 7175 655f 6669 6c65 6e61 6d65 0a20  nique_filename. 
-00002490: 2020 203e 3e3e 2063 6c61 7373 204d 7943     >>> class MyC
-000024a0: 6c61 7373 286f 626a 6563 7429 3a0a 2020  lass(object):.  
-000024b0: 2020 2e2e 2e20 2020 2020 7061 7373 0a20    ...     pass. 
-000024c0: 2020 202e 2e2e 0a20 2020 203e 3e3e 2062     ....    >>> b
-000024d0: 6172 203d 2027 6261 7227 0a20 2020 203e  ar = 'bar'.    >
-000024e0: 3e3e 2023 2050 7265 7061 7265 2074 6865  >> # Prepare the
-000024f0: 2073 6372 6970 7420 616e 6420 6e65 6365   script and nece
-00002500: 7373 6172 7920 6461 7461 2e0a 2020 2020  ssary data..    
-00002510: 3e3e 3e20 7363 7269 7074 203d 2022 5c6e  >>> script = "\n
-00002520: 222e 6a6f 696e 280a 2020 2020 2e2e 2e20  ".join(.    ... 
-00002530: 2020 2020 280a 2020 2020 2e2e 2e20 2020      (.    ...   
-00002540: 2020 2020 2020 2264 6566 205f 5f69 6e69        "def __ini
-00002550: 745f 5f28 7365 6c66 293a 222c 0a20 2020  t__(self):",.   
-00002560: 202e 2e2e 2020 2020 2020 2020 2022 2020   ...         "  
-00002570: 2020 7365 6c66 2e66 6f6f 203d 2027 6261    self.foo = 'ba
-00002580: 7227 222c 0a20 2020 202e 2e2e 2020 2020  r'",.    ...    
-00002590: 2029 0a20 2020 202e 2e2e 2029 0a20 2020   ).    ... ).   
-000025a0: 203e 3e3e 2023 2047 6174 6865 7220 696e   >>> # Gather in
-000025b0: 666f 726d 6174 696f 6e2e 0a20 2020 203e  formation..    >
-000025c0: 3e3e 206e 616d 6520 3d20 225f 5f69 6e69  >> name = "__ini
-000025d0: 745f 5f22 0a20 2020 203e 3e3e 206f 776e  t__".    >>> own
-000025e0: 6572 5f6e 616d 6520 3d20 4d79 436c 6173  er_name = MyClas
-000025f0: 732e 5f5f 6e61 6d65 5f5f 0a20 2020 203e  s.__name__.    >
-00002600: 3e3e 206d 6f64 756c 6520 3d20 4d79 436c  >> module = MyCl
-00002610: 6173 732e 5f5f 6d6f 6475 6c65 5f5f 0a20  ass.__module__. 
-00002620: 2020 203e 3e3e 2066 696c 656e 616d 6520     >>> filename 
-00002630: 3d20 6765 6e65 7261 7465 5f75 6e69 7175  = generate_uniqu
-00002640: 655f 6669 6c65 6e61 6d65 286e 616d 652c  e_filename(name,
-00002650: 206d 6f64 756c 652c 206f 776e 6572 5f6e   module, owner_n
-00002660: 616d 6529 0a20 2020 203e 3e3e 2067 6c6f  ame).    >>> glo
-00002670: 6273 203d 207b 2262 6172 223a 2062 6172  bs = {"bar": bar
-00002680: 7d0a 2020 2020 3e3e 3e20 2320 4d61 6b65  }.    >>> # Make
-00002690: 2066 756e 6374 696f 6e20 616e 6420 6174   function and at
-000026a0: 7461 6368 2069 7420 6173 2061 206d 6574  tach it as a met
-000026b0: 686f 642e 0a20 2020 203e 3e3e 204d 7943  hod..    >>> MyC
-000026c0: 6c61 7373 2e5f 5f69 6e69 745f 5f20 3d20  lass.__init__ = 
-000026d0: 6d61 6b65 5f66 756e 6374 696f 6e28 6e61  make_function(na
-000026e0: 6d65 2c20 7363 7269 7074 2c20 676c 6f62  me, script, glob
-000026f0: 732c 2066 696c 656e 616d 652c 206d 6f64  s, filename, mod
-00002700: 756c 6529 0a20 2020 203e 3e3e 206f 626a  ule).    >>> obj
-00002710: 203d 204d 7943 6c61 7373 2829 0a20 2020   = MyClass().   
-00002720: 203e 3e3e 206f 626a 2e66 6f6f 0a20 2020   >>> obj.foo.   
-00002730: 2027 6261 7227 0a0a 6578 706c 6963 6974   'bar'..explicit
-00002740: 5f68 6173 680a 5e5e 5e5e 5e5e 5e5e 5e5e  _hash.^^^^^^^^^^
-00002750: 5e5e 5e0a 4d65 7461 636c 6173 7320 7468  ^^^.Metaclass th
-00002760: 6174 2066 6f72 6365 7320 605f 5f68 6173  at forces `__has
-00002770: 685f 5f60 2074 6f20 6265 2064 6563 6c61  h__` to be decla
-00002780: 7265 6420 7768 656e 6576 6572 2060 5f5f  red whenever `__
-00002790: 6571 5f5f 6020 6973 2064 6563 6c61 7265  eq__` is declare
-000027a0: 642e 0a0a 2e2e 2063 6f64 653a 3a20 7079  d..... code:: py
-000027b0: 7468 6f6e 0a0a 2020 2020 3e3e 3e20 6672  thon..    >>> fr
-000027c0: 6f6d 2073 6978 2069 6d70 6f72 7420 7769  om six import wi
-000027d0: 7468 5f6d 6574 6163 6c61 7373 0a20 2020  th_metaclass.   
-000027e0: 203e 3e3e 2066 726f 6d20 6261 7369 6363   >>> from basicc
-000027f0: 6f2e 6578 706c 6963 6974 5f68 6173 6820  o.explicit_hash 
-00002800: 696d 706f 7274 2045 7870 6c69 6369 7448  import ExplicitH
-00002810: 6173 684d 6574 610a 2020 2020 3e3e 3e20  ashMeta.    >>> 
-00002820: 636c 6173 7320 4173 7365 7428 7769 7468  class Asset(with
-00002830: 5f6d 6574 6163 6c61 7373 2845 7870 6c69  _metaclass(Expli
-00002840: 6369 7448 6173 684d 6574 612c 206f 626a  citHashMeta, obj
-00002850: 6563 7429 293a 0a20 2020 202e 2e2e 2020  ect)):.    ...  
-00002860: 2020 2064 6566 205f 5f65 715f 5f28 7365     def __eq__(se
-00002870: 6c66 2c20 6f74 6865 7229 3a0a 2020 2020  lf, other):.    
-00002880: 2e2e 2e20 2020 2020 2020 2020 7061 7373  ...         pass
-00002890: 0a20 2020 202e 2e2e 0a20 2020 2054 7261  .    ....    Tra
-000028a0: 6365 6261 636b 2028 6d6f 7374 2072 6563  ceback (most rec
-000028b0: 656e 7420 6361 6c6c 206c 6173 7429 3a0a  ent call last):.
-000028c0: 2020 2020 5479 7065 4572 726f 723a 2064      TypeError: d
-000028d0: 6563 6c61 7265 6420 275f 5f65 715f 5f27  eclared '__eq__'
-000028e0: 2069 6e20 2741 7373 6574 2720 6275 7420   in 'Asset' but 
-000028f0: 6469 646e 2774 2064 6563 6c61 7265 2027  didn't declare '
-00002900: 5f5f 6861 7368 5f5f 270a 0a66 6162 7269  __hash__'..fabri
-00002910: 6361 7465 5f76 616c 7565 0a5e 5e5e 5e5e  cate_value.^^^^^
-00002920: 5e5e 5e5e 5e5e 5e5e 5e5e 0a52 756e 2061  ^^^^^^^^^^.Run a
-00002930: 2076 616c 7565 2074 6872 6f75 6768 2061   value through a
-00002940: 2063 616c 6c61 626c 6520 6661 6374 6f72   callable factor
-00002950: 7920 286f 7220 4e6f 6e65 292e 0a0a 2e2e  y (or None).....
-00002960: 2063 6f64 653a 3a20 7079 7468 6f6e 0a0a   code:: python..
-00002970: 2020 2020 3e3e 3e20 6672 6f6d 2062 6173      >>> from bas
-00002980: 6963 636f 2e66 6162 7269 6361 7465 5f76  icco.fabricate_v
-00002990: 616c 7565 2069 6d70 6f72 7420 6661 6272  alue import fabr
-000029a0: 6963 6174 655f 7661 6c75 650a 2020 2020  icate_value.    
-000029b0: 3e3e 3e20 6661 6272 6963 6174 655f 7661  >>> fabricate_va
-000029c0: 6c75 6528 4e6f 6e65 2c20 3329 2020 2320  lue(None, 3)  # 
-000029d0: 6e6f 2066 6163 746f 7279 2c20 7661 6c75  no factory, valu
-000029e0: 6520 7061 7373 7468 726f 7567 680a 2020  e passthrough.  
-000029f0: 2020 330a 2020 2020 3e3e 3e20 6661 6272    3.    >>> fabr
-00002a00: 6963 6174 655f 7661 6c75 6528 7374 722c  icate_value(str,
-00002a10: 2033 2920 2023 2063 616c 6c61 626c 6520   3)  # callable 
-00002a20: 6661 6374 6f72 790a 2020 2020 2733 270a  factory.    '3'.
-00002a30: 2020 2020 3e3e 3e20 6661 6272 6963 6174      >>> fabricat
-00002a40: 655f 7661 6c75 6528 2273 7472 222c 2033  e_value("str", 3
-00002a50: 2920 2023 2075 7365 2061 6e20 696d 706f  )  # use an impo
-00002a60: 7274 2070 6174 680a 2020 2020 2733 270a  rt path.    '3'.
-00002a70: 2020 2020 3e3e 3e20 6661 6272 6963 6174      >>> fabricat
-00002a80: 655f 7661 6c75 6528 696e 7429 2020 2320  e_value(int)  # 
-00002a90: 6e6f 2069 6e70 7574 2076 616c 7565 2c20  no input value, 
-00002aa0: 6a75 7374 2074 6865 2066 6163 746f 7279  just the factory
-00002ab0: 2069 7473 656c 660a 2020 2020 300a 0a67   itself.    0..g
-00002ac0: 6574 5f6d 726f 0a5e 5e5e 5e5e 5e5e 0a47  et_mro.^^^^^^^.G
-00002ad0: 6574 2063 6f6e 7369 7374 656e 7420 4d52  et consistent MR
-00002ae0: 4f20 616d 6f6e 6773 7420 6469 6666 6572  O amongst differ
-00002af0: 656e 7420 7079 7468 6f6e 2076 6572 7369  ent python versi
-00002b00: 6f6e 732e 2054 6869 7320 776f 726b 7320  ons. This works 
-00002b10: 6576 656e 2077 6974 6820 6765 6e65 7269  even with generi
-00002b20: 6320 636c 6173 7365 7320 696e 2050 7974  c classes in Pyt
-00002b30: 686f 6e20 322e 372e 0a0a 2e2e 2063 6f64  hon 2.7..... cod
-00002b40: 653a 3a20 7079 7468 6f6e 0a0a 2020 2020  e:: python..    
-00002b50: 3e3e 3e20 6672 6f6d 2073 6978 2069 6d70  >>> from six imp
-00002b60: 6f72 7420 7769 7468 5f6d 6574 6163 6c61  ort with_metacla
-00002b70: 7373 0a20 2020 203e 3e3e 2066 726f 6d20  ss.    >>> from 
-00002b80: 7469 7070 6f20 696d 706f 7274 2047 656e  tippo import Gen
-00002b90: 6572 6963 2c20 5479 7065 5661 720a 2020  eric, TypeVar.  
-00002ba0: 2020 3e3e 3e20 6672 6f6d 2062 6173 6963    >>> from basic
-00002bb0: 636f 2e67 6574 5f6d 726f 2069 6d70 6f72  co.get_mro impor
-00002bc0: 7420 6765 745f 6d72 6f0a 2020 2020 3e3e  t get_mro.    >>
-00002bd0: 3e20 5420 3d20 5479 7065 5661 7228 2254  > T = TypeVar("T
-00002be0: 2229 0a20 2020 203e 3e3e 2063 6c61 7373  ").    >>> class
-00002bf0: 204d 7947 656e 6572 6963 2847 656e 6572   MyGeneric(Gener
-00002c00: 6963 5b54 5d29 3a0a 2020 2020 2e2e 2e20  ic[T]):.    ... 
-00002c10: 2020 2020 7061 7373 0a20 2020 202e 2e2e      pass.    ...
-00002c20: 0a20 2020 203e 3e3e 2063 6c61 7373 2053  .    >>> class S
-00002c30: 7562 436c 6173 7328 4d79 4765 6e65 7269  ubClass(MyGeneri
-00002c40: 635b 545d 293a 0a20 2020 202e 2e2e 2020  c[T]):.    ...  
-00002c50: 2020 2070 6173 730a 2020 2020 2e2e 2e0a     pass.    ....
-00002c60: 2020 2020 3e3e 3e20 636c 6173 7320 4d69      >>> class Mi
-00002c70: 7865 6428 5375 6243 6c61 7373 5b54 5d2c  xed(SubClass[T],
-00002c80: 204d 7947 656e 6572 6963 5b54 5d29 3a0a   MyGeneric[T]):.
-00002c90: 2020 2020 2e2e 2e20 2020 2020 7061 7373      ...     pass
-00002ca0: 0a20 2020 202e 2e2e 0a20 2020 203e 3e3e  .    ....    >>>
-00002cb0: 205b 632e 5f5f 6e61 6d65 5f5f 2066 6f72   [c.__name__ for
-00002cc0: 2063 2069 6e20 6765 745f 6d72 6f28 4d69   c in get_mro(Mi
-00002cd0: 7865 6429 5d0a 2020 2020 5b27 4d69 7865  xed)].    ['Mixe
-00002ce0: 6427 2c20 2753 7562 436c 6173 7327 2c20  d', 'SubClass', 
-00002cf0: 274d 7947 656e 6572 6963 272c 2027 4765  'MyGeneric', 'Ge
-00002d00: 6e65 7269 6327 2c20 276f 626a 6563 7427  neric', 'object'
-00002d10: 5d0a 0a68 6173 685f 6361 6368 655f 7772  ]..hash_cache_wr
-00002d20: 6170 7065 720a 5e5e 5e5e 5e5e 5e5e 5e5e  apper.^^^^^^^^^^
-00002d30: 5e5e 5e5e 5e5e 5e5e 0a41 6e20 696e 7465  ^^^^^^^^.An inte
-00002d40: 6765 7220 7375 6263 6c61 7373 2074 6861  ger subclass tha
-00002d50: 7420 7069 636b 6c65 732f 636f 7069 6573  t pickles/copies
-00002d60: 2061 7320 4e6f 6e65 2e20 5468 6973 2063   as None. This c
-00002d70: 616e 2062 6520 7573 6564 2074 6f20 6176  an be used to av
-00002d80: 6f69 6420 7365 7269 616c 697a 696e 6720  oid serializing 
-00002d90: 6120 6361 6368 6564 2068 6173 6820 7661  a cached hash va
-00002da0: 6c75 652e 0a0a 2e2e 2063 6f64 653a 3a20  lue..... code:: 
+00000000: 2e2e 206c 6f67 6f5f 7374 6172 740a 2e2e  .. logo_start...
+00000010: 2072 6177 3a3a 2068 746d 6c0a 0a20 2020   raw:: html..   
+00000020: 3c70 2061 6c69 676e 3d22 6365 6e74 6572  <p align="center
+00000030: 223e 0a20 2020 2020 3c61 2068 7265 663d  ">.     <a href=
+00000040: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
+00000050: 636f 6d2f 6272 756e 6f6e 6963 6b6f 2f62  com/brunonicko/b
+00000060: 6173 6963 636f 223e 0a20 2020 2020 2020  asicco">.       
+00000070: 2020 3c70 6963 7475 7265 3e0a 2020 2020    <picture>.    
+00000080: 2020 2020 2020 2020 3c6f 626a 6563 7420          <object 
+00000090: 6461 7461 3d22 2e2f 5f73 7461 7469 632f  data="./_static/
+000000a0: 6261 7369 6363 6f2e 7376 6722 2074 7970  basicco.svg" typ
+000000b0: 653d 2269 6d61 6765 2f70 6e67 223e 0a20  e="image/png">. 
+000000c0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+000000d0: 736f 7572 6365 2073 7263 7365 743d 222e  source srcset=".
+000000e0: 2f64 6f63 732f 736f 7572 6365 2f5f 7374  /docs/source/_st
+000000f0: 6174 6963 2f62 6173 6963 636f 5f77 6869  atic/basicco_whi
+00000100: 7465 2e73 7667 2220 6d65 6469 613d 2228  te.svg" media="(
+00000110: 7072 6566 6572 732d 636f 6c6f 722d 7363  prefers-color-sc
+00000120: 6865 6d65 3a20 6461 726b 2922 3e0a 2020  heme: dark)">.  
+00000130: 2020 2020 2020 2020 2020 2020 2020 3c69                <i
+00000140: 6d67 2073 7263 3d22 2e2f 646f 6373 2f73  mg src="./docs/s
+00000150: 6f75 7263 652f 5f73 7461 7469 632f 6261  ource/_static/ba
+00000160: 7369 6363 6f2e 7376 6722 2077 6964 7468  sicco.svg" width
+00000170: 3d22 3630 2522 2061 6c74 3d22 6261 7369  ="60%" alt="basi
+00000180: 6363 6f22 202f 3e0a 2020 2020 2020 2020  cco" />.        
+00000190: 2020 2020 3c2f 6f62 6a65 6374 3e0a 2020      </object>.  
+000001a0: 2020 2020 2020 203c 2f70 6963 7475 7265         </picture
+000001b0: 3e0a 2020 2020 203c 2f61 3e0a 2020 203c  >.     </a>.   <
+000001c0: 2f70 3e0a 2e2e 206c 6f67 6f5f 656e 640a  /p>... logo_end.
+000001d0: 0a2e 2e20 696d 6167 653a 3a20 6874 7470  ... image:: http
+000001e0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f62  s://github.com/b
+000001f0: 7275 6e6f 6e69 636b 6f2f 6261 7369 6363  runonicko/basicc
+00000200: 6f2f 776f 726b 666c 6f77 732f 4d79 5079  o/workflows/MyPy
+00000210: 2f62 6164 6765 2e73 7667 0a20 2020 3a74  /badge.svg.   :t
+00000220: 6172 6765 743a 2068 7474 7073 3a2f 2f67  arget: https://g
+00000230: 6974 6875 622e 636f 6d2f 6272 756e 6f6e  ithub.com/brunon
+00000240: 6963 6b6f 2f62 6173 6963 636f 2f61 6374  icko/basicco/act
+00000250: 696f 6e73 3f71 7565 7279 3d77 6f72 6b66  ions?query=workf
+00000260: 6c6f 7725 3341 4d79 5079 0a0a 2e2e 2069  low%3AMyPy.... i
+00000270: 6d61 6765 3a3a 2068 7474 7073 3a2f 2f67  mage:: https://g
+00000280: 6974 6875 622e 636f 6d2f 6272 756e 6f6e  ithub.com/brunon
+00000290: 6963 6b6f 2f62 6173 6963 636f 2f77 6f72  icko/basicco/wor
+000002a0: 6b66 6c6f 7773 2f4c 696e 742f 6261 6467  kflows/Lint/badg
+000002b0: 652e 7376 670a 2020 203a 7461 7267 6574  e.svg.   :target
+000002c0: 3a20 6874 7470 733a 2f2f 6769 7468 7562  : https://github
+000002d0: 2e63 6f6d 2f62 7275 6e6f 6e69 636b 6f2f  .com/brunonicko/
+000002e0: 6261 7369 6363 6f2f 6163 7469 6f6e 733f  basicco/actions?
+000002f0: 7175 6572 793d 776f 726b 666c 6f77 2533  query=workflow%3
+00000300: 414c 696e 740a 0a2e 2e20 696d 6167 653a  ALint.... image:
+00000310: 3a20 6874 7470 733a 2f2f 6769 7468 7562  : https://github
+00000320: 2e63 6f6d 2f62 7275 6e6f 6e69 636b 6f2f  .com/brunonicko/
+00000330: 6261 7369 6363 6f2f 776f 726b 666c 6f77  basicco/workflow
+00000340: 732f 5465 7374 732f 6261 6467 652e 7376  s/Tests/badge.sv
+00000350: 670a 2020 203a 7461 7267 6574 3a20 6874  g.   :target: ht
+00000360: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000370: 2f62 7275 6e6f 6e69 636b 6f2f 6261 7369  /brunonicko/basi
+00000380: 6363 6f2f 6163 7469 6f6e 733f 7175 6572  cco/actions?quer
+00000390: 793d 776f 726b 666c 6f77 2533 4154 6573  y=workflow%3ATes
+000003a0: 7473 0a0a 2e2e 2069 6d61 6765 3a3a 2068  ts.... image:: h
+000003b0: 7474 7073 3a2f 2f72 6561 6474 6865 646f  ttps://readthedo
+000003c0: 6373 2e6f 7267 2f70 726f 6a65 6374 732f  cs.org/projects/
+000003d0: 6261 7369 6363 6f2f 6261 6467 652f 3f76  basicco/badge/?v
+000003e0: 6572 7369 6f6e 3d73 7461 626c 650a 2020  ersion=stable.  
+000003f0: 203a 7461 7267 6574 3a20 6874 7470 733a   :target: https:
+00000400: 2f2f 6261 7369 6363 6f2e 7265 6164 7468  //basicco.readth
+00000410: 6564 6f63 732e 696f 2f65 6e2f 7374 6162  edocs.io/en/stab
+00000420: 6c65 2f0a 0a2e 2e20 696d 6167 653a 3a20  le/.... image:: 
+00000430: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
+00000440: 6c64 732e 696f 2f67 6974 6875 622f 6c69  lds.io/github/li
+00000450: 6365 6e73 652f 6272 756e 6f6e 6963 6b6f  cense/brunonicko
+00000460: 2f62 6173 6963 636f 3f63 6f6c 6f72 3d6c  /basicco?color=l
+00000470: 6967 6874 2d67 7265 656e 0a20 2020 3a74  ight-green.   :t
+00000480: 6172 6765 743a 2068 7474 7073 3a2f 2f67  arget: https://g
+00000490: 6974 6875 622e 636f 6d2f 6272 756e 6f6e  ithub.com/brunon
+000004a0: 6963 6b6f 2f62 6173 6963 636f 2f62 6c6f  icko/basicco/blo
+000004b0: 622f 6d61 7374 6572 2f4c 4943 454e 5345  b/master/LICENSE
+000004c0: 0a0a 2e2e 2069 6d61 6765 3a3a 2068 7474  .... image:: htt
+000004d0: 7073 3a2f 2f73 7461 7469 632e 7065 7079  ps://static.pepy
+000004e0: 2e74 6563 682f 7065 7273 6f6e 616c 697a  .tech/personaliz
+000004f0: 6564 2d62 6164 6765 2f62 6173 6963 636f  ed-badge/basicco
+00000500: 3f70 6572 696f 643d 746f 7461 6c26 756e  ?period=total&un
+00000510: 6974 733d 696e 7465 726e 6174 696f 6e61  its=internationa
+00000520: 6c5f 7379 7374 656d 266c 6566 745f 636f  l_system&left_co
+00000530: 6c6f 723d 6772 6579 2672 6967 6874 5f63  lor=grey&right_c
+00000540: 6f6c 6f72 3d62 7269 6768 7467 7265 656e  olor=brightgreen
+00000550: 266c 6566 745f 7465 7874 3d44 6f77 6e6c  &left_text=Downl
+00000560: 6f61 6473 0a20 2020 3a74 6172 6765 743a  oads.   :target:
+00000570: 2068 7474 7073 3a2f 2f70 6570 792e 7465   https://pepy.te
+00000580: 6368 2f70 726f 6a65 6374 2f62 6173 6963  ch/project/basic
+00000590: 636f 0a0a 2e2e 2069 6d61 6765 3a3a 2068  co.... image:: h
+000005a0: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
+000005b0: 6473 2e69 6f2f 7079 7069 2f70 7976 6572  ds.io/pypi/pyver
+000005c0: 7369 6f6e 732f 6261 7369 6363 6f3f 636f  sions/basicco?co
+000005d0: 6c6f 723d 6c69 6768 742d 6772 6565 6e26  lor=light-green&
+000005e0: 7374 796c 653d 666c 6174 0a20 2020 3a74  style=flat.   :t
+000005f0: 6172 6765 743a 2068 7474 7073 3a2f 2f70  arget: https://p
+00000600: 7970 692e 6f72 672f 7072 6f6a 6563 742f  ypi.org/project/
+00000610: 6261 7369 6363 6f2f 0a0a 4f76 6572 7669  basicco/..Overvi
+00000620: 6577 0a2d 2d2d 2d2d 2d2d 2d0a 6042 6173  ew.--------.`Bas
+00000630: 6520 436c 6173 7365 7360 5f20 616e 6420  e Classes`_ and 
+00000640: 6055 7469 6c69 7469 6573 605f 2074 6861  `Utilities`_ tha
+00000650: 7420 656e 6861 6e63 6520 636f 6465 2063  t enhance code c
+00000660: 6f6d 7061 7469 6269 6c69 7479 2c20 6665  ompatibility, fe
+00000670: 6174 7572 6573 2061 6e64 2076 616c 6964  atures and valid
+00000680: 6174 696f 6e2e 0a0a 4d6f 7469 7661 7469  ation...Motivati
+00000690: 6f6e 0a2d 2d2d 2d2d 2d2d 2d2d 2d0a 5768  on.----------.Wh
+000006a0: 696c 6520 6465 7665 6c6f 7069 6e67 2050  ile developing P
+000006b0: 7974 686f 6e20 736f 6674 7761 7265 2066  ython software f
+000006c0: 6f72 2056 6973 7561 6c20 4566 6665 6374  or Visual Effect
+000006d0: 7320 7069 7065 6c69 6e65 732c 2049 2066  s pipelines, I f
+000006e0: 6f75 6e64 206d 7973 656c 6620 6861 7669  ound myself havi
+000006f0: 6e67 2074 6f20 7772 6974 6520 7468 6520  ng to write the 
+00000700: 7361 6d65 2062 6f69 6c65 722d 706c 6174  same boiler-plat
+00000710: 650a 636f 6465 206f 7665 7220 616e 6420  e.code over and 
+00000720: 6f76 6572 2061 6761 696e 2c20 6173 2077  over again, as w
+00000730: 656c 6c20 6173 2073 7472 7567 676c 696e  ell as strugglin
+00000740: 6720 7769 7468 2063 6f6d 7061 7469 6269  g with compatibi
+00000750: 6c69 7479 2069 7373 7565 7320 616e 6420  lity issues and 
+00000760: 6665 6174 7572 6520 6761 7073 2062 6574  feature gaps bet
+00000770: 7765 656e 2050 7974 686f 6e20 322e 3720  ween Python 2.7 
+00000780: 616e 640a 5079 7468 6f6e 2033 2e37 2b2e  and.Python 3.7+.
+00000790: 0a0a 536f 2049 2064 6563 6964 6564 2074  ..So I decided t
+000007a0: 6f20 696d 706c 656d 656e 7420 736f 6c75  o implement solu
+000007b0: 7469 6f6e 7320 666f 7220 7468 6f73 6520  tions for those 
+000007c0: 6973 7375 6573 2061 7420 7468 6520 6042  issues at the `B
+000007d0: 6173 6560 5f2c 2061 6e64 2060 6261 7369  ase`_, and `basi
+000007e0: 6363 6f60 2077 6173 2062 6f72 6e2e 0a0a  cco` was born...
+000007f0: 4261 7365 2043 6c61 7373 6573 0a2d 2d2d  Base Classes.---
+00000800: 2d2d 2d2d 2d2d 2d2d 2d0a 0a43 6f6d 7061  ---------..Compa
+00000810: 7442 6173 650a 5e5e 5e5e 5e5e 5e5e 5e5e  tBase.^^^^^^^^^^
+00000820: 0a54 6865 2067 6f61 6c20 7769 7468 2074  .The goal with t
+00000830: 6865 2060 436f 6d70 6174 4261 7365 4d65  he `CompatBaseMe
+00000840: 7461 6020 6d65 7461 636c 6173 7320 616e  ta` metaclass an
+00000850: 6420 7468 6520 6043 6f6d 7061 7442 6173  d the `CompatBas
+00000860: 6560 2063 6c61 7373 2069 7320 746f 2062  e` class is to b
+00000870: 7269 6467 6520 736f 6d65 206f 6620 7468  ridge some of th
+00000880: 6520 6665 6174 7572 6520 6761 7073 2062  e feature gaps b
+00000890: 6574 7765 656e 0a50 7974 686f 6e20 322e  etween.Python 2.
+000008a0: 3720 616e 6420 5079 7468 6f6e 2033 2e37  7 and Python 3.7
+000008b0: 2b2e 0a0a 5468 6973 2069 6e63 6c75 6465  +...This include
+000008c0: 7320 6164 6469 6e67 2050 7974 686f 6e20  s adding Python 
+000008d0: 322e 3720 776f 726b 6172 6f75 6e64 7320  2.7 workarounds 
+000008e0: 666f 723a 0a20 202d 2060 4162 7374 7261  for:.  - `Abstra
+000008f0: 6374 2070 726f 7065 7274 6965 7320 3c68  ct properties <h
+00000900: 7474 7073 3a2f 2f64 6f63 732e 7079 7468  ttps://docs.pyth
+00000910: 6f6e 2e6f 7267 2f33 2f6c 6962 7261 7279  on.org/3/library
+00000920: 2f61 6263 2e68 746d 6c23 6162 632e 6162  /abc.html#abc.ab
+00000930: 7374 7261 6374 7072 6f70 6572 7479 3e60  stractproperty>`
+00000940: 5f3a 2042 6574 7465 7220 6061 6273 7472  _: Better `abstr
+00000950: 6163 746d 6574 686f 6460 0a20 2020 2064  actmethod`.    d
+00000960: 6563 6f72 6174 6f72 2073 7570 706f 7274  ecorator support
+00000970: 2066 6f72 2070 726f 7065 7274 792d 6c69   for property-li
+00000980: 6b65 2064 6573 6372 6970 746f 7273 2e20  ke descriptors. 
+00000990: 5365 6520 616c 736f 2060 6162 7374 7261  See also `abstra
+000009a0: 6374 5f63 6c61 7373 605f 2e0a 2020 2d20  ct_class`_..  - 
+000009b0: 6050 4550 2034 3837 203c 6874 7470 733a  `PEP 487 <https:
+000009c0: 2f2f 7065 7073 2e70 7974 686f 6e2e 6f72  //peps.python.or
+000009d0: 672f 7065 702d 3034 3837 2f3e 605f 3a20  g/pep-0487/>`_: 
+000009e0: 5375 7070 6f72 7420 666f 7220 605f 5f69  Support for `__i
+000009f0: 6e69 745f 7375 6263 6c61 7373 5f5f 6020  nit_subclass__` 
+00000a00: 616e 6420 605f 5f73 6574 5f6e 616d 655f  and `__set_name_
+00000a10: 5f60 2e0a 2020 2020 5365 6520 616c 736f  _`..    See also
+00000a20: 2060 696e 6974 5f73 7562 636c 6173 7360   `init_subclass`
+00000a30: 5f20 616e 6420 6073 6574 5f6e 616d 6560  _ and `set_name`
+00000a40: 5f2e 0a20 202d 2060 6f62 6a65 6374 2e5f  _..  - `object._
+00000a50: 5f64 6972 5f5f 203c 6874 7470 733a 2f2f  _dir__ <https://
+00000a60: 646f 6373 2e70 7974 686f 6e2e 6f72 672f  docs.python.org/
+00000a70: 332f 7265 6665 7265 6e63 652f 6461 7461  3/reference/data
+00000a80: 6d6f 6465 6c2e 6874 6d6c 236f 626a 6563  model.html#objec
+00000a90: 742e 5f5f 6469 725f 5f3e 605f 3a20 4261  t.__dir__>`_: Ba
+00000aa0: 7365 2060 5f5f 6469 725f 5f60 206d 6574  se `__dir__` met
+00000ab0: 686f 642e 0a20 2020 2053 6565 2061 6c73  hod..    See als
+00000ac0: 6f20 6064 6566 6175 6c74 5f64 6972 605f  o `default_dir`_
+00000ad0: 2e0a 2020 2d20 605f 5f65 715f 5f20 6f76  ..  - `__eq__ ov
+00000ae0: 6572 7269 6465 203c 6874 7470 733a 2f2f  erride <https://
+00000af0: 646f 6373 2e70 7974 686f 6e2e 6f72 672f  docs.python.org/
+00000b00: 332f 7265 6665 7265 6e63 652f 6461 7461  3/reference/data
+00000b10: 6d6f 6465 6c2e 6874 6d6c 236f 626a 6563  model.html#objec
+00000b20: 742e 5f5f 6861 7368 5f5f 3e60 5f3a 204f  t.__hash__>`_: O
+00000b30: 7665 7272 6964 696e 6720 605f 5f65 715f  verriding `__eq_
+00000b40: 5f60 2077 696c 6c0a 2020 2020 7365 7420  _` will.    set 
+00000b50: 605f 5f68 6173 685f 5f60 2074 6f20 4e6f  `__hash__` to No
+00000b60: 6e65 2e20 5365 6520 616c 736f 2060 696d  ne. See also `im
+00000b70: 706c 6963 6974 5f68 6173 6860 5f2e 0a20  plicit_hash`_.. 
+00000b80: 202d 2060 5045 5020 3330 3720 3c68 7474   - `PEP 307 <htt
+00000b90: 7073 3a2f 2f70 6570 732e 7079 7468 6f6e  ps://peps.python
+00000ba0: 2e6f 7267 2f70 6570 2d30 3330 372f 3e60  .org/pep-0307/>`
+00000bb0: 5f3a 2053 7570 706f 7274 2066 6f72 2070  _: Support for p
+00000bc0: 6963 6b6c 696e 6720 6f62 6a65 6374 7320  ickling objects 
+00000bd0: 7769 7468 2060 5f5f 736c 6f74 735f 5f60  with `__slots__`
+00000be0: 2e0a 2020 2020 5365 6520 616c 736f 2060  ..    See also `
+00000bf0: 6f62 6a5f 7374 6174 6560 5f2e 0a20 202d  obj_state`_..  -
+00000c00: 2060 5045 5020 3331 3535 203c 6874 7470   `PEP 3155 <http
+00000c10: 733a 2f2f 7065 7073 2e70 7974 686f 6e2e  s://peps.python.
+00000c20: 6f72 672f 7065 702d 3033 3135 352f 3e60  org/pep-03155/>`
+00000c30: 5f3a 2051 7561 6c69 6669 6564 206e 616d  _: Qualified nam
+00000c40: 6520 605f 5f71 7561 6c6e 616d 655f 5f60  e `__qualname__`
+00000c50: 2066 6f72 206e 6573 7465 6420 636c 6173   for nested clas
+00000c60: 7365 732e 0a20 2020 2053 6565 2061 6c73  ses..    See als
+00000c70: 6f20 6071 7561 6c6e 616d 6560 5f2e 0a20  o `qualname`_.. 
+00000c80: 202d 2060 5f5f 6e65 5f5f 2062 6568 6176   - `__ne__ behav
+00000c90: 696f 7220 3c68 7474 7073 3a2f 2f64 6f63  ior <https://doc
+00000ca0: 732e 7079 7468 6f6e 2e6f 7267 2f33 2e30  s.python.org/3.0
+00000cb0: 2f77 6861 7473 6e65 772f 332e 302e 6874  /whatsnew/3.0.ht
+00000cc0: 6d6c 236f 7065 7261 746f 7273 2d61 6e64  ml#operators-and
+00000cd0: 2d73 7065 6369 616c 2d6d 6574 686f 6473  -special-methods
+00000ce0: 3e60 5f3a 2042 7920 6465 6661 756c 742c  >`_: By default,
+00000cf0: 0a20 2020 2060 5f5f 6e65 5f5f 6020 7368  .    `__ne__` sh
+00000d00: 6f75 6c64 206e 6567 6174 6520 7468 6520  ould negate the 
+00000d10: 7265 7375 6c74 206f 6620 605f 5f65 715f  result of `__eq_
+00000d20: 5f60 2e0a 2020 2020 5365 6520 616c 736f  _`..    See also
+00000d30: 2060 7361 6665 5f6e 6f74 5f65 7175 616c   `safe_not_equal
+00000d40: 7360 5f0a 2020 2d20 6050 4550 2030 3536  s`_.  - `PEP 056
+00000d50: 3020 3c68 7474 7073 3a2f 2f70 6570 732e  0 <https://peps.
+00000d60: 7079 7468 6f6e 2e6f 7267 2f70 6570 2d30  python.org/pep-0
+00000d70: 3536 302f 3e60 5f3a 2042 6574 7465 7220  560/>`_: Better 
+00000d80: 6861 6e64 6c69 6e67 206f 6620 4765 6e65  handling of Gene
+00000d90: 7269 6320 636c 6173 7365 732e 0a20 2020  ric classes..   
+00000da0: 2053 6565 2061 6c73 6f20 6074 6970 706f   See also `tippo
+00000db0: 203c 6874 7470 733a 2f2f 6769 7468 7562   <https://github
+00000dc0: 2e63 6f6d 2f62 7275 6e6f 6e69 636b 6f2f  .com/brunonicko/
+00000dd0: 7469 7070 6f23 6765 6e65 7269 632d 6669  tippo#generic-fi
+00000de0: 7865 733e 605f 2e0a 0a42 6173 650a 5e5e  xes>`_...Base.^^
+00000df0: 5e5e 0a49 6e20 6164 6469 7469 6f6e 2074  ^^.In addition t
+00000e00: 6f20 7468 6520 636f 6d70 6174 6962 696c  o the compatibil
+00000e10: 6974 7920 736f 6c75 7469 6f6e 732c 2074  ity solutions, t
+00000e20: 6865 2067 6f61 6c20 7769 7468 2074 6865  he goal with the
+00000e30: 2060 4261 7365 4d65 7461 6020 6d65 7461   `BaseMeta` meta
+00000e40: 636c 6173 7320 616e 6420 7468 6520 6042  class and the `B
+00000e50: 6173 6560 2063 6c61 7373 2069 7320 746f  ase` class is to
+00000e60: 2061 6464 0a75 7365 6675 6c20 6c6f 772d   add.useful low-
+00000e70: 6c65 7665 6c20 6665 6174 7572 6573 2074  level features t
+00000e80: 6861 7420 686f 7065 6675 6c6c 7920 7969  hat hopefully yi
+00000e90: 656c 6420 6265 7474 6572 2063 6f64 6520  eld better code 
+00000ea0: 7265 6164 6162 696c 6974 7920 616e 6420  readability and 
+00000eb0: 7661 6c69 6461 7469 6f6e 2e0a 0a54 6869  validation...Thi
+00000ec0: 7320 696e 636c 7564 6573 3a0a 2020 2d20  s includes:.  - 
+00000ed0: 605f 5f77 6561 6b72 6566 5f5f 6020 736c  `__weakref__` sl
+00000ee0: 6f74 3a20 4164 6465 6420 6279 2064 6566  ot: Added by def
+00000ef0: 6175 6c74 2e0a 2020 2d20 606c 6f63 6b65  ault..  - `locke
+00000f00: 645f 636c 6173 7360 5f3a 2050 7562 6c69  d_class`_: Publi
+00000f10: 6320 636c 6173 7320 6174 7472 6962 7574  c class attribut
+00000f20: 6573 2061 7265 2072 6561 642d 6f6e 6c79  es are read-only
+00000f30: 2062 7920 6465 6661 756c 742e 0a20 202d   by default..  -
+00000f40: 2060 6578 706c 6963 6974 5f68 6173 6860   `explicit_hash`
+00000f50: 5f3a 204f 7665 7272 6964 696e 6720 605f  _: Overriding `_
+00000f60: 5f65 715f 5f60 2077 6974 686f 7574 206f  _eq__` without o
+00000f70: 7665 7272 6964 696e 6720 605f 5f68 6173  verriding `__has
+00000f80: 685f 5f60 2077 696c 6c20 7261 6973 6520  h__` will raise 
+00000f90: 616e 2065 7272 6f72 2e0a 2020 2d20 606e  an error..  - `n
+00000fa0: 616d 6573 7061 6365 605f 3a20 4164 6473  amespace`_: Adds
+00000fb0: 2061 2070 726f 7465 6374 6564 2060 5f5f   a protected `__
+00000fc0: 6e61 6d65 7370 6163 6560 2075 6e69 7175  namespace` uniqu
+00000fd0: 6520 746f 2065 6163 6820 636c 6173 732e  e to each class.
+00000fe0: 0a20 202d 2060 7275 6e74 696d 655f 6669  .  - `runtime_fi
+00000ff0: 6e61 6c60 5f3a 2052 756e 7469 6d65 2063  nal`_: Runtime c
+00001000: 6865 636b 696e 6720 666f 7220 636c 6173  hecking for clas
+00001010: 7365 7320 616e 6420 6d65 7468 6f64 7320  ses and methods 
+00001020: 6465 636f 7261 7465 6420 7769 7468 2060  decorated with `
+00001030: 6669 6e61 6c60 2e0a 0a53 6c6f 7474 6564  final`...Slotted
+00001040: 4261 7365 0a5e 5e5e 5e5e 5e5e 5e5e 5e5e  Base.^^^^^^^^^^^
+00001050: 0a54 6865 2060 536c 6f74 7465 6442 6173  .The `SlottedBas
+00001060: 6560 2063 6c61 7373 2061 6e64 2074 6865  e` class and the
+00001070: 2060 536c 6f74 7465 6442 6173 654d 6574   `SlottedBaseMet
+00001080: 6160 206d 6574 6163 6c61 7373 206f 6666  a` metaclass off
+00001090: 6572 2061 6c6c 2066 6561 7475 7265 7320  er all features 
+000010a0: 6672 6f6d 2060 4261 7365 6020 616e 6420  from `Base` and 
+000010b0: 6042 6173 654d 6574 6160 2070 6c75 7320  `BaseMeta` plus 
+000010c0: 696d 706c 6963 6974 0a60 5f5f 736c 6f74  implicit.`__slot
+000010d0: 735f 5f60 2064 6563 6c61 7261 7469 6f6e  s__` declaration
+000010e0: 2e20 5365 6520 6073 6c6f 7474 6564 203c  . See `slotted <
+000010f0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00001100: 6f6d 2f62 7275 6e6f 6e69 636b 6f2f 736c  om/brunonicko/sl
+00001110: 6f74 7465 643e 605f 2066 6f72 206d 6f72  otted>`_ for mor
+00001120: 6520 696e 666f 726d 6174 696f 6e2e 0a0a  e information...
+00001130: 5574 696c 6974 6965 730a 2d2d 2d2d 2d2d  Utilities.------
+00001140: 2d2d 2d0a 4170 6172 7420 6672 6f6d 2074  ---.Apart from t
+00001150: 6865 2066 6561 7475 7265 7320 696e 7465  he features inte
+00001160: 6772 6174 6564 2069 6e74 6f20 7468 6520  grated into the 
+00001170: 6261 7365 2063 6c61 7373 6573 2c20 6062  base classes, `b
+00001180: 6173 6963 636f 6020 7072 6f76 6964 6573  asicco` provides
+00001190: 206d 616e 7920 6765 6e65 7261 6c20 7574   many general ut
+000011a0: 696c 6974 7920 6d6f 6475 6c65 732e 0a0a  ility modules...
+000011b0: 6162 7374 7261 6374 5f63 6c61 7373 0a5e  abstract_class.^
+000011c0: 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e 5e0a 4265  ^^^^^^^^^^^^^.Be
+000011d0: 7474 6572 2060 6162 7374 7261 6374 2063  tter `abstract c
+000011e0: 6c61 7373 6573 203c 6874 7470 733a 2f2f  lasses <https://
+000011f0: 646f 6373 2e70 7974 686f 6e2e 6f72 672f  docs.python.org/
+00001200: 332f 6c69 6272 6172 792f 6162 632e 6874  3/library/abc.ht
+00001210: 6d6c 2361 6263 2e61 6273 7472 6163 746d  ml#abc.abstractm
+00001220: 6574 686f 643e 605f 2073 7570 706f 7274  ethod>`_ support
+00001230: 2e0a 0a50 726f 7669 6465 7320 6162 7374  ...Provides abst
+00001240: 7261 6374 2064 6563 6f72 6174 6f72 7320  ract decorators 
+00001250: 7468 6174 2063 616e 2062 6520 7573 6564  that can be used
+00001260: 2064 6972 6563 746c 7920 6f6e 206d 6574   directly on met
+00001270: 686f 6473 2062 7574 2061 6c73 6f20 6f6e  hods but also on
+00001280: 2063 6c61 7373 6573 2c20 7072 6f70 6572   classes, proper
+00001290: 7469 6573 2c20 636c 6173 736d 6574 686f  ties, classmetho
+000012a0: 6473 2c20 616e 640a 7374 6174 6963 6d65  ds, and.staticme
+000012b0: 7468 6f64 7320 2865 7665 6e20 696e 2050  thods (even in P
+000012c0: 7974 686f 6e20 322e 3729 2e0a 0a2e 2e20  ython 2.7)..... 
+000012d0: 636f 6465 3a3a 2070 7974 686f 6e0a 0a20  code:: python.. 
+000012e0: 2020 203e 3e3e 2066 726f 6d20 7369 7820     >>> from six 
+000012f0: 696d 706f 7274 2077 6974 685f 6d65 7461  import with_meta
+00001300: 636c 6173 730a 2020 2020 3e3e 3e20 6672  class.    >>> fr
+00001310: 6f6d 2062 6173 6963 636f 2e61 6273 7472  om basicco.abstr
+00001320: 6163 745f 636c 6173 7320 696d 706f 7274  act_class import
+00001330: 2041 6273 7472 6163 744d 6574 612c 2061   AbstractMeta, a
+00001340: 6273 7472 6163 740a 2020 2020 3e3e 3e20  bstract.    >>> 
+00001350: 636c 6173 7320 4173 7365 7428 7769 7468  class Asset(with
+00001360: 5f6d 6574 6163 6c61 7373 2841 6273 7472  _metaclass(Abstr
+00001370: 6163 744d 6574 612c 206f 626a 6563 7429  actMeta, object)
+00001380: 293a 0a20 2020 202e 2e2e 2020 2020 2040  ):.    ...     @
+00001390: 6162 7374 7261 6374 0a20 2020 202e 2e2e  abstract.    ...
+000013a0: 2020 2020 2064 6566 206d 6574 686f 6428       def method(
+000013b0: 7365 6c66 293a 0a20 2020 202e 2e2e 2020  self):.    ...  
+000013c0: 2020 2020 2020 2070 6173 730a 2020 2020         pass.    
+000013d0: 2e2e 2e0a 2020 2020 2e2e 2e20 2020 2020  ....    ...     
+000013e0: 4070 726f 7065 7274 790a 2020 2020 2e2e  @property.    ..
+000013f0: 2e20 2020 2020 4061 6273 7472 6163 740a  .     @abstract.
+00001400: 2020 2020 2e2e 2e20 2020 2020 6465 6620      ...     def 
+00001410: 7072 6f70 2873 656c 6629 3a0a 2020 2020  prop(self):.    
+00001420: 2e2e 2e20 2020 2020 2020 2020 7265 7475  ...         retu
+00001430: 726e 204e 6f6e 650a 2020 2020 2e2e 2e0a  rn None.    ....
+00001440: 2020 2020 3e3e 3e20 4173 7365 7428 290a      >>> Asset().
+00001450: 2020 2020 5472 6163 6562 6163 6b20 286d      Traceback (m
+00001460: 6f73 7420 7265 6365 6e74 2063 616c 6c20  ost recent call 
+00001470: 6c61 7374 293a 0a20 2020 2054 7970 6545  last):.    TypeE
+00001480: 7272 6f72 3a20 4361 6e27 7420 696e 7374  rror: Can't inst
+00001490: 616e 7469 6174 6520 6162 7374 7261 6374  antiate abstract
+000014a0: 2063 6c61 7373 2041 7373 6574 2077 6974   class Asset wit
+000014b0: 6820 6162 7374 7261 6374 206d 6574 686f  h abstract metho
+000014c0: 6473 206d 6574 686f 642c 2070 726f 700a  ds method, prop.
+000014d0: 0a2e 2e20 636f 6465 3a3a 2070 7974 686f  ... code:: pytho
+000014e0: 6e0a 0a20 2020 203e 3e3e 2066 726f 6d20  n..    >>> from 
+000014f0: 6261 7369 6363 6f2e 6162 7374 7261 6374  basicco.abstract
+00001500: 5f63 6c61 7373 2069 6d70 6f72 7420 4162  _class import Ab
+00001510: 7374 7261 6374 4d65 7461 2c20 6162 7374  stractMeta, abst
+00001520: 7261 6374 0a20 2020 203e 3e3e 2040 6162  ract.    >>> @ab
+00001530: 7374 7261 6374 0a20 2020 202e 2e2e 2063  stract.    ... c
+00001540: 6c61 7373 2041 7373 6574 2877 6974 685f  lass Asset(with_
+00001550: 6d65 7461 636c 6173 7328 4162 7374 7261  metaclass(Abstra
+00001560: 6374 4d65 7461 2c20 6f62 6a65 6374 2929  ctMeta, object))
+00001570: 3a0a 2020 2020 2e2e 2e20 2020 2020 7061  :.    ...     pa
+00001580: 7373 0a20 2020 202e 2e2e 0a20 2020 203e  ss.    ....    >
+00001590: 3e3e 2041 7373 6574 2829 0a20 2020 2054  >> Asset().    T
+000015a0: 7261 6365 6261 636b 2028 6d6f 7374 2072  raceback (most r
+000015b0: 6563 656e 7420 6361 6c6c 206c 6173 7429  ecent call last)
+000015c0: 3a0a 2020 2020 5479 7065 4572 726f 723a  :.    TypeError:
+000015d0: 2063 616e 2774 2069 6e73 7461 6e74 6961   can't instantia
+000015e0: 7465 2061 6273 7472 6163 7420 636c 6173  te abstract clas
+000015f0: 7320 2741 7373 6574 270a 0a63 616c 6c65  s 'Asset'..calle
+00001600: 725f 6d6f 6475 6c65 0a5e 5e5e 5e5e 5e5e  r_module.^^^^^^^
+00001610: 5e5e 5e5e 5e5e 0a52 6574 7269 6576 6520  ^^^^^^.Retrieve 
+00001620: 7468 6520 6361 6c6c 6572 2773 206d 6f64  the caller's mod
+00001630: 756c 6520 6e61 6d65 2e0a 0a2e 2e20 636f  ule name..... co
+00001640: 6465 3a3a 2070 7974 686f 6e0a 0a20 2020  de:: python..   
+00001650: 203e 3e3e 2066 726f 6d20 6261 7369 6363   >>> from basicc
+00001660: 6f2e 6361 6c6c 6572 5f6d 6f64 756c 6520  o.caller_module 
+00001670: 696d 706f 7274 2063 616c 6c65 725f 6d6f  import caller_mo
+00001680: 6475 6c65 0a20 2020 203e 3e3e 2064 6566  dule.    >>> def
+00001690: 2064 6f5f 736f 6d65 7468 696e 6728 293a   do_something():
+000016a0: 0a20 2020 202e 2e2e 2020 2020 2072 6574  .    ...     ret
+000016b0: 7572 6e20 2249 2077 6173 2063 616c 6c65  urn "I was calle
+000016c0: 6420 6279 207b 7d22 2e66 6f72 6d61 7428  d by {}".format(
+000016d0: 6361 6c6c 6572 5f6d 6f64 756c 6528 2929  caller_module())
+000016e0: 0a20 2020 202e 2e2e 0a20 2020 203e 3e3e  .    ....    >>>
+000016f0: 2064 6f5f 736f 6d65 7468 696e 6728 290a   do_something().
+00001700: 2020 2020 2749 2077 6173 2063 616c 6c65      'I was calle
+00001710: 6420 6279 205f 5f6d 6169 6e5f 5f27 0a0a  d by __main__'..
+00001720: 636f 6e74 6578 745f 7661 7273 0a5e 5e5e  context_vars.^^^
+00001730: 5e5e 5e5e 5e5e 5e5e 5e0a 4261 636b 706f  ^^^^^^^^^.Backpo
+00001740: 7274 206f 6620 7468 6520 6063 6f6e 7465  rt of the `conte
+00001750: 7874 7661 7273 6020 6d6f 6475 6c65 2066  xtvars` module f
+00001760: 6f72 2050 7974 686f 6e20 322e 372c 2062  or Python 2.7, b
+00001770: 6173 6564 206f 6e0a 604d 6167 6963 5374  ased on.`MagicSt
+00001780: 6163 6b2f 636f 6e74 6578 7476 6172 7320  ack/contextvars 
+00001790: 3c68 7474 7073 3a2f 2f67 6974 6875 622e  <https://github.
+000017a0: 636f 6d2f 4d61 6769 6353 7461 636b 2f63  com/MagicStack/c
+000017b0: 6f6e 7465 7874 7661 7273 3e60 5f2e 0a0a  ontextvars>`_...
+000017c0: 5768 656e 2069 6d70 6f72 7465 6420 6672  When imported fr
+000017d0: 6f6d 2050 7974 686f 6e20 332c 2069 7420  om Python 3, it 
+000017e0: 7369 6d70 6c79 2072 6564 6972 6563 7473  simply redirects
+000017f0: 2074 6f20 7468 6520 6e61 7469 7665 0a60   to the native.`
+00001800: 636f 6e74 6578 7476 6172 7320 3c68 7474  contextvars <htt
+00001810: 7073 3a2f 2f64 6f63 732e 7079 7468 6f6e  ps://docs.python
+00001820: 2e6f 7267 2f33 2f6c 6962 7261 7279 2f63  .org/3/library/c
+00001830: 6f6e 7465 7874 7661 7273 2e68 746d 6c3e  ontextvars.html>
+00001840: 605f 206d 6f64 756c 652e 0a0a 2e2e 2063  `_ module..... c
+00001850: 6f64 653a 3a20 7079 7468 6f6e 0a0a 2020  ode:: python..  
+00001860: 2020 3e3e 3e20 6672 6f6d 2062 6173 6963    >>> from basic
+00001870: 636f 2e63 6f6e 7465 7874 5f76 6172 7320  co.context_vars 
+00001880: 696d 706f 7274 2043 6f6e 7465 7874 5661  import ContextVa
+00001890: 720a 2020 2020 3e3e 3e20 6d79 5f76 6172  r.    >>> my_var
+000018a0: 203d 2043 6f6e 7465 7874 5661 7228 226d   = ContextVar("m
+000018b0: 795f 7661 7222 2c20 6465 6661 756c 743d  y_var", default=
+000018c0: 2262 6172 2229 0a20 2020 203e 3e3e 2074  "bar").    >>> t
+000018d0: 6f6b 656e 203d 206d 795f 7661 722e 7365  oken = my_var.se
+000018e0: 7428 2266 6f6f 2229 0a20 2020 203e 3e3e  t("foo").    >>>
+000018f0: 206d 795f 7661 722e 6765 7428 290a 2020   my_var.get().  
+00001900: 2020 2766 6f6f 270a 2020 2020 3e3e 3e20    'foo'.    >>> 
+00001910: 6d79 5f76 6172 2e72 6573 6574 2874 6f6b  my_var.reset(tok
+00001920: 656e 290a 2020 2020 3e3e 3e20 6d79 5f76  en).    >>> my_v
+00001930: 6172 2e67 6574 2829 0a20 2020 2027 6261  ar.get().    'ba
+00001940: 7227 0a0a 6375 7374 6f6d 5f72 6570 720a  r'..custom_repr.
+00001950: 5e5e 5e5e 5e5e 5e5e 5e5e 5e0a 4375 7374  ^^^^^^^^^^^.Cust
+00001960: 6f6d 2072 6570 7265 7365 6e74 6174 696f  om representatio
+00001970: 6e20 6675 6e63 7469 6f6e 7320 666f 7220  n functions for 
+00001980: 6d61 7070 696e 6773 2c20 6974 656d 732c  mappings, items,
+00001990: 2061 6e64 2069 7465 7261 626c 6573 2e0a   and iterables..
+000019a0: 0a2e 2e20 636f 6465 3a3a 2070 7974 686f  ... code:: pytho
+000019b0: 6e0a 0a20 2020 203e 3e3e 2066 726f 6d20  n..    >>> from 
+000019c0: 6261 7369 6363 6f2e 6375 7374 6f6d 5f72  basicco.custom_r
+000019d0: 6570 7220 696d 706f 7274 206d 6170 7069  epr import mappi
+000019e0: 6e67 5f72 6570 720a 2020 2020 3e3e 3e20  ng_repr.    >>> 
+000019f0: 6463 7420 3d20 7b22 6122 3a20 312c 2022  dct = {"a": 1, "
+00001a00: 6222 3a20 327d 0a20 2020 203e 3e3e 206d  b": 2}.    >>> m
+00001a10: 6170 7069 6e67 5f72 6570 7228 6463 742c  apping_repr(dct,
+00001a20: 2070 7265 6669 783d 223c 222c 2073 7566   prefix="<", suf
+00001a30: 6669 783d 223e 222c 2074 656d 706c 6174  fix=">", templat
+00001a40: 653d 227b 6b65 797d 3d7b 7661 6c75 657d  e="{key}={value}
+00001a50: 222c 2073 6f72 7469 6e67 3d54 7275 6529  ", sorting=True)
+00001a60: 0a20 2020 2022 3c27 6127 3d31 2c20 2762  .    "<'a'=1, 'b
+00001a70: 273d 323e 220a 0a2e 2e20 636f 6465 3a3a  '=2>".... code::
+00001a80: 2070 7974 686f 6e0a 0a20 2020 203e 3e3e   python..    >>>
+00001a90: 2066 726f 6d20 6261 7369 6363 6f2e 6375   from basicco.cu
+00001aa0: 7374 6f6d 5f72 6570 7220 696d 706f 7274  stom_repr import
+00001ab0: 206d 6170 7069 6e67 5f72 6570 720a 2020   mapping_repr.  
+00001ac0: 2020 3e3e 3e20 6974 656d 7320 3d20 5b28    >>> items = [(
+00001ad0: 2261 222c 2031 292c 2028 2262 222c 2032  "a", 1), ("b", 2
+00001ae0: 295d 0a20 2020 203e 3e3e 206d 6170 7069  )].    >>> mappi
+00001af0: 6e67 5f72 6570 7228 6974 656d 732c 2070  ng_repr(items, p
+00001b00: 7265 6669 783d 225b 222c 2073 7566 6669  refix="[", suffi
+00001b10: 783d 225d 222c 2074 656d 706c 6174 653d  x="]", template=
+00001b20: 6c61 6d62 6461 2069 2c20 6b65 792c 2076  lambda i, key, v
+00001b30: 616c 7565 3a20 6b65 7920 2b20 2220 2d3e  alue: key + " ->
+00001b40: 2022 202b 2076 616c 7565 290a 2020 2020   " + value).    
+00001b50: 225b 2761 2720 2d3e 2031 2c20 2762 2720  "['a' -> 1, 'b' 
+00001b60: 2d3e 2032 5d22 0a0a 2e2e 2063 6f64 653a  -> 2]".... code:
+00001b70: 3a20 7079 7468 6f6e 0a0a 2020 2020 3e3e  : python..    >>
+00001b80: 3e20 6672 6f6d 2062 6173 6963 636f 2e63  > from basicco.c
+00001b90: 7573 746f 6d5f 7265 7072 2069 6d70 6f72  ustom_repr impor
+00001ba0: 7420 6974 6572 6162 6c65 5f72 6570 720a  t iterable_repr.
+00001bb0: 2020 2020 3e3e 3e20 7475 7020 3d20 2822      >>> tup = ("
+00001bc0: 6122 2c20 2262 222c 2022 6322 2c20 312c  a", "b", "c", 1,
+00001bd0: 2032 2c20 3329 0a20 2020 203e 3e3e 2069   2, 3).    >>> i
+00001be0: 7465 7261 626c 655f 7265 7072 2874 7570  terable_repr(tup
+00001bf0: 2c20 7072 6566 6978 3d22 3c22 2c20 7375  , prefix="<", su
+00001c00: 6666 6978 3d22 3e22 2c20 7661 6c75 655f  ffix=">", value_
+00001c10: 7265 7072 3d73 7472 290a 2020 2020 273c  repr=str).    '<
+00001c20: 612c 2062 2c20 632c 2031 2c20 322c 2033  a, b, c, 1, 2, 3
+00001c30: 3e27 0a0a 6461 7461 5f63 6c61 7373 0a5e  >'..data_class.^
+00001c40: 5e5e 5e5e 5e5e 5e5e 5e0a 5079 7468 6f6e  ^^^^^^^^^.Python
+00001c50: 2032 2e37 2063 6f6d 7061 7469 626c 6520   2.7 compatible 
+00001c60: 6461 7461 636c 6173 732d 6c69 6b65 2073  dataclass-like s
+00001c70: 7472 7563 7475 7265 732e 0a0a 2e2e 2063  tructures..... c
+00001c80: 6f64 653a 3a20 7079 7468 6f6e 0a0a 2020  ode:: python..  
+00001c90: 2020 3e3e 3e20 6672 6f6d 206d 6174 6820    >>> from math 
+00001ca0: 696d 706f 7274 2073 7172 740a 2020 2020  import sqrt.    
+00001cb0: 3e3e 3e20 6672 6f6d 2062 6173 6963 636f  >>> from basicco
+00001cc0: 2e64 6174 615f 636c 6173 7320 696d 706f  .data_class impo
+00001cd0: 7274 2044 6174 6143 6c61 7373 2c20 6669  rt DataClass, fi
+00001ce0: 656c 640a 2020 2020 3e3e 3e20 636c 6173  eld.    >>> clas
+00001cf0: 7320 5665 6374 6f72 2844 6174 6143 6c61  s Vector(DataCla
+00001d00: 7373 293a 0a20 2020 202e 2e2e 2020 2020  ss):.    ...    
+00001d10: 2078 203d 2066 6965 6c64 2829 2020 2320   x = field()  # 
+00001d20: 7479 7065 3a20 666c 6f61 740a 2020 2020  type: float.    
+00001d30: 2e2e 2e20 2020 2020 7920 3d20 6669 656c  ...     y = fiel
+00001d40: 6428 2920 2023 2074 7970 653a 2066 6c6f  d()  # type: flo
+00001d50: 6174 0a20 2020 202e 2e2e 2020 2020 2040  at.    ...     @
+00001d60: 7072 6f70 6572 7479 0a20 2020 202e 2e2e  property.    ...
+00001d70: 2020 2020 2040 6669 656c 640a 2020 2020       @field.    
+00001d80: 2e2e 2e20 2020 2020 6465 6620 6d61 6728  ...     def mag(
+00001d90: 7365 6c66 293a 0a20 2020 202e 2e2e 2020  self):.    ...  
+00001da0: 2020 2020 2020 2072 6574 7572 6e20 7371         return sq
+00001db0: 7274 2873 656c 662e 782a 2a32 202b 2073  rt(self.x**2 + s
+00001dc0: 656c 662e 792a 2a32 290a 2020 2020 2e2e  elf.y**2).    ..
+00001dd0: 2e0a 2020 2020 3e3e 3e20 5665 6374 6f72  ..    >>> Vector
+00001de0: 2833 2e30 2c20 342e 3029 0a20 2020 2056  (3.0, 4.0).    V
+00001df0: 6563 746f 7228 332e 302c 2034 2e30 2c20  ector(3.0, 4.0, 
+00001e00: 6d61 673d 352e 3029 0a0a 6465 6661 756c  mag=5.0)..defaul
+00001e10: 745f 6469 720a 5e5e 5e5e 5e5e 5e5e 5e5e  t_dir.^^^^^^^^^^
+00001e20: 5e0a 4261 636b 706f 7274 206f 6620 5079  ^.Backport of Py
+00001e30: 7468 6f6e 2033 2773 2069 6d70 6c65 6d65  thon 3's impleme
+00001e40: 6e74 6174 696f 6e20 6f66 0a60 6f62 6a65  ntation of.`obje
+00001e50: 6374 2e5f 5f64 6972 5f5f 203c 6874 7470  ct.__dir__ <http
+00001e60: 733a 2f2f 646f 6373 2e70 7974 686f 6e2e  s://docs.python.
+00001e70: 6f72 672f 332f 7265 6665 7265 6e63 652f  org/3/reference/
+00001e80: 6461 7461 6d6f 6465 6c2e 6874 6d6c 236f  datamodel.html#o
+00001e90: 626a 6563 742e 5f5f 6469 725f 5f3e 605f  bject.__dir__>`_
+00001ea0: 2066 6f72 2050 7974 686f 6e20 322e 372e   for Python 2.7.
+00001eb0: 0a0a 5468 6973 2061 6c6c 6f77 7320 666f  ..This allows fo
+00001ec0: 7220 6361 6c6c 696e 6720 6073 7570 6572  r calling `super
+00001ed0: 2829 2e5f 5f64 6972 5f5f 2829 6020 6672  ().__dir__()` fr
+00001ee0: 6f6d 2061 2073 7562 636c 6173 7320 746f  om a subclass to
+00001ef0: 206c 6576 6572 6167 6520 7468 6520 6465   leverage the de
+00001f00: 6661 756c 7420 696d 706c 656d 656e 7461  fault implementa
+00001f10: 7469 6f6e 2e0a 0a2e 2e20 636f 6465 3a3a  tion..... code::
+00001f20: 2070 7974 686f 6e0a 0a20 2020 203e 3e3e   python..    >>>
+00001f30: 2066 726f 6d20 7369 7820 696d 706f 7274   from six import
+00001f40: 2077 6974 685f 6d65 7461 636c 6173 730a   with_metaclass.
+00001f50: 2020 2020 3e3e 3e20 6672 6f6d 2062 6173      >>> from bas
+00001f60: 6963 636f 2e64 6566 6175 6c74 5f64 6972  icco.default_dir
+00001f70: 2069 6d70 6f72 7420 4465 6661 756c 7444   import DefaultD
+00001f80: 6972 0a20 2020 203e 3e3e 2063 6c61 7373  ir.    >>> class
+00001f90: 2043 6c61 7373 2844 6566 6175 6c74 4469   Class(DefaultDi
+00001fa0: 7229 3a0a 2020 2020 2e2e 2e20 2020 2020  r):.    ...     
+00001fb0: 6465 6620 5f5f 6469 725f 5f28 7365 6c66  def __dir__(self
+00001fc0: 293a 0a20 2020 202e 2e2e 2020 2020 2020  ):.    ...      
+00001fd0: 2020 2072 6574 7572 6e20 7375 7065 7228     return super(
+00001fe0: 436c 6173 732c 2073 656c 6629 2e5f 5f64  Class, self).__d
+00001ff0: 6972 5f5f 2829 0a20 2020 202e 2e2e 0a20  ir__().    .... 
+00002000: 2020 203e 3e3e 206f 626a 203d 2043 6c61     >>> obj = Cla
+00002010: 7373 2829 0a20 2020 203e 3e3e 2064 6972  ss().    >>> dir
+00002020: 286f 626a 290a 2020 2020 5b2e 2e2e 5d0a  (obj).    [...].
+00002030: 0a64 796e 616d 6963 5f63 6c61 7373 0a5e  .dynamic_class.^
+00002040: 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e 0a45 6173  ^^^^^^^^^^^^.Eas
+00002050: 696c 7920 6765 6e65 7261 7465 2063 6c61  ily generate cla
+00002060: 7373 6573 206f 6e20 7468 6520 666c 792e  sses on the fly.
+00002070: 2054 6869 7320 776f 726b 7320 6265 7374   This works best
+00002080: 2077 6974 6820 6120 6042 6173 6560 5f20   with a `Base`_ 
+00002090: 636c 6173 732e 0a49 6620 7072 6f76 6964  class..If provid
+000020a0: 6564 2061 2076 616c 6964 2071 7561 6c69  ed a valid quali
+000020b0: 6669 6564 206e 616d 6520 616e 6420 6d6f  fied name and mo
+000020c0: 6475 6c65 2028 7573 6573 2060 6361 6c6c  dule (uses `call
+000020d0: 6572 5f6d 6f64 756c 6560 5f20 6279 2064  er_module`_ by d
+000020e0: 6566 6175 6c74 292c 2074 6865 2063 6c61  efault), the cla
+000020f0: 7373 2077 696c 6c20 6265 2070 6963 6b61  ss will be picka
+00002100: 626c 652f 696d 706f 7274 6162 6c65 2e0a  ble/importable..
+00002110: 0a2e 2e20 636f 6465 3a3a 2070 7974 686f  ... code:: pytho
+00002120: 6e0a 0a20 2020 203e 3e3e 2066 726f 6d20  n..    >>> from 
+00002130: 6261 7369 6363 6f20 696d 706f 7274 2042  basicco import B
+00002140: 6173 650a 2020 2020 3e3e 3e20 6672 6f6d  ase.    >>> from
+00002150: 2062 6173 6963 636f 2e64 796e 616d 6963   basicco.dynamic
+00002160: 5f63 6c61 7373 2069 6d70 6f72 7420 6d61  _class import ma
+00002170: 6b65 5f63 6c73 0a20 2020 203e 3e3e 2063  ke_cls.    >>> c
+00002180: 6c61 7373 204d 7943 6c61 7373 286f 626a  lass MyClass(obj
+00002190: 6563 7429 3a0a 2020 2020 2e2e 2e20 2020  ect):.    ...   
+000021a0: 2020 4479 6e43 6c61 7373 203d 206d 616b    DynClass = mak
+000021b0: 655f 636c 7328 224d 7943 6c61 7373 2e44  e_cls("MyClass.D
+000021c0: 796e 436c 6173 7322 2c20 6261 7365 733d  ynClass", bases=
+000021d0: 2842 6173 652c 292c 2064 6374 3d7b 2266  (Base,), dct={"f
+000021e0: 6f6f 223a 2022 6261 7222 7d29 0a20 2020  oo": "bar"}).   
+000021f0: 202e 2e2e 0a20 2020 203e 3e3e 2072 6570   ....    >>> rep
+00002200: 7228 4d79 436c 6173 732e 4479 6e43 6c61  r(MyClass.DynCla
+00002210: 7373 290a 2020 2020 223c 636c 6173 7320  ss).    "<class 
+00002220: 275f 5f6d 6169 6e5f 5f2e 4d79 436c 6173  '__main__.MyClas
+00002230: 732e 4479 6e43 6c61 7373 273e 220a 0a64  s.DynClass'>"..d
+00002240: 796e 616d 6963 5f63 6f64 650a 5e5e 5e5e  ynamic_code.^^^^
+00002250: 5e5e 5e5e 5e5e 5e5e 0a47 656e 6572 6174  ^^^^^^^^.Generat
+00002260: 6520 6465 6275 6767 6162 6c65 2063 6f64  e debuggable cod
+00002270: 6520 6f6e 2074 6865 2066 6c79 2074 6861  e on the fly tha
+00002280: 7420 7375 7070 6f72 7473 206c 696e 6520  t supports line 
+00002290: 6e75 6d62 6572 7320 6f6e 2074 7261 6365  numbers on trace
+000022a0: 6261 636b 732e 0a0a 2e2e 2063 6f64 653a  backs..... code:
+000022b0: 3a20 7079 7468 6f6e 0a0a 2020 2020 3e3e  : python..    >>
+000022c0: 3e20 6672 6f6d 2062 6173 6963 636f 2e64  > from basicco.d
+000022d0: 796e 616d 6963 5f63 6f64 6520 696d 706f  ynamic_code impo
+000022e0: 7274 206d 616b 655f 6675 6e63 7469 6f6e  rt make_function
+000022f0: 2c20 6765 6e65 7261 7465 5f75 6e69 7175  , generate_uniqu
+00002300: 655f 6669 6c65 6e61 6d65 0a20 2020 203e  e_filename.    >
+00002310: 3e3e 2063 6c61 7373 204d 7943 6c61 7373  >> class MyClass
+00002320: 286f 626a 6563 7429 3a0a 2020 2020 2e2e  (object):.    ..
+00002330: 2e20 2020 2020 7061 7373 0a20 2020 202e  .     pass.    .
+00002340: 2e2e 0a20 2020 203e 3e3e 2062 6172 203d  ...    >>> bar =
+00002350: 2027 6261 7227 0a20 2020 203e 3e3e 2023   'bar'.    >>> #
+00002360: 2050 7265 7061 7265 2074 6865 2073 6372   Prepare the scr
+00002370: 6970 7420 616e 6420 6e65 6365 7373 6172  ipt and necessar
+00002380: 7920 6461 7461 2e0a 2020 2020 3e3e 3e20  y data..    >>> 
+00002390: 7363 7269 7074 203d 2022 5c6e 222e 6a6f  script = "\n".jo
+000023a0: 696e 280a 2020 2020 2e2e 2e20 2020 2020  in(.    ...     
+000023b0: 280a 2020 2020 2e2e 2e20 2020 2020 2020  (.    ...       
+000023c0: 2020 2264 6566 205f 5f69 6e69 745f 5f28    "def __init__(
+000023d0: 7365 6c66 293a 222c 0a20 2020 202e 2e2e  self):",.    ...
+000023e0: 2020 2020 2020 2020 2022 2020 2020 7365           "    se
+000023f0: 6c66 2e66 6f6f 203d 2027 6261 7227 222c  lf.foo = 'bar'",
+00002400: 0a20 2020 202e 2e2e 2020 2020 2029 0a20  .    ...     ). 
+00002410: 2020 202e 2e2e 2029 0a20 2020 203e 3e3e     ... ).    >>>
+00002420: 2023 2047 6174 6865 7220 696e 666f 726d   # Gather inform
+00002430: 6174 696f 6e2e 0a20 2020 203e 3e3e 206e  ation..    >>> n
+00002440: 616d 6520 3d20 225f 5f69 6e69 745f 5f22  ame = "__init__"
+00002450: 0a20 2020 203e 3e3e 206f 776e 6572 5f6e  .    >>> owner_n
+00002460: 616d 6520 3d20 4d79 436c 6173 732e 5f5f  ame = MyClass.__
+00002470: 6e61 6d65 5f5f 0a20 2020 203e 3e3e 206d  name__.    >>> m
+00002480: 6f64 756c 6520 3d20 4d79 436c 6173 732e  odule = MyClass.
+00002490: 5f5f 6d6f 6475 6c65 5f5f 0a20 2020 203e  __module__.    >
+000024a0: 3e3e 2066 696c 656e 616d 6520 3d20 6765  >> filename = ge
+000024b0: 6e65 7261 7465 5f75 6e69 7175 655f 6669  nerate_unique_fi
+000024c0: 6c65 6e61 6d65 286e 616d 652c 206d 6f64  lename(name, mod
+000024d0: 756c 652c 206f 776e 6572 5f6e 616d 6529  ule, owner_name)
+000024e0: 0a20 2020 203e 3e3e 2067 6c6f 6273 203d  .    >>> globs =
+000024f0: 207b 2262 6172 223a 2062 6172 7d0a 2020   {"bar": bar}.  
+00002500: 2020 3e3e 3e20 2320 4d61 6b65 2066 756e    >>> # Make fun
+00002510: 6374 696f 6e20 616e 6420 6174 7461 6368  ction and attach
+00002520: 2069 7420 6173 2061 206d 6574 686f 642e   it as a method.
+00002530: 0a20 2020 203e 3e3e 204d 7943 6c61 7373  .    >>> MyClass
+00002540: 2e5f 5f69 6e69 745f 5f20 3d20 6d61 6b65  .__init__ = make
+00002550: 5f66 756e 6374 696f 6e28 6e61 6d65 2c20  _function(name, 
+00002560: 7363 7269 7074 2c20 676c 6f62 732c 2066  script, globs, f
+00002570: 696c 656e 616d 652c 206d 6f64 756c 6529  ilename, module)
+00002580: 0a20 2020 203e 3e3e 206f 626a 203d 204d  .    >>> obj = M
+00002590: 7943 6c61 7373 2829 0a20 2020 203e 3e3e  yClass().    >>>
+000025a0: 206f 626a 2e66 6f6f 0a20 2020 2027 6261   obj.foo.    'ba
+000025b0: 7227 0a0a 6578 706c 6963 6974 5f68 6173  r'..explicit_has
+000025c0: 680a 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e 5e0a  h.^^^^^^^^^^^^^.
+000025d0: 4d65 7461 636c 6173 7320 7468 6174 2066  Metaclass that f
+000025e0: 6f72 6365 7320 605f 5f68 6173 685f 5f60  orces `__hash__`
+000025f0: 2074 6f20 6265 2064 6563 6c61 7265 6420   to be declared 
+00002600: 7768 656e 6576 6572 2060 5f5f 6571 5f5f  whenever `__eq__
+00002610: 6020 6973 2064 6563 6c61 7265 642e 0a0a  ` is declared...
+00002620: 2e2e 2063 6f64 653a 3a20 7079 7468 6f6e  .. code:: python
+00002630: 0a0a 2020 2020 3e3e 3e20 6672 6f6d 2073  ..    >>> from s
+00002640: 6978 2069 6d70 6f72 7420 7769 7468 5f6d  ix import with_m
+00002650: 6574 6163 6c61 7373 0a20 2020 203e 3e3e  etaclass.    >>>
+00002660: 2066 726f 6d20 6261 7369 6363 6f2e 6578   from basicco.ex
+00002670: 706c 6963 6974 5f68 6173 6820 696d 706f  plicit_hash impo
+00002680: 7274 2045 7870 6c69 6369 7448 6173 684d  rt ExplicitHashM
+00002690: 6574 610a 2020 2020 3e3e 3e20 636c 6173  eta.    >>> clas
+000026a0: 7320 4173 7365 7428 7769 7468 5f6d 6574  s Asset(with_met
+000026b0: 6163 6c61 7373 2845 7870 6c69 6369 7448  aclass(ExplicitH
+000026c0: 6173 684d 6574 612c 206f 626a 6563 7429  ashMeta, object)
+000026d0: 293a 0a20 2020 202e 2e2e 2020 2020 2064  ):.    ...     d
+000026e0: 6566 205f 5f65 715f 5f28 7365 6c66 2c20  ef __eq__(self, 
+000026f0: 6f74 6865 7229 3a0a 2020 2020 2e2e 2e20  other):.    ... 
+00002700: 2020 2020 2020 2020 7061 7373 0a20 2020          pass.   
+00002710: 202e 2e2e 0a20 2020 2054 7261 6365 6261   ....    Traceba
+00002720: 636b 2028 6d6f 7374 2072 6563 656e 7420  ck (most recent 
+00002730: 6361 6c6c 206c 6173 7429 3a0a 2020 2020  call last):.    
+00002740: 5479 7065 4572 726f 723a 2064 6563 6c61  TypeError: decla
+00002750: 7265 6420 275f 5f65 715f 5f27 2069 6e20  red '__eq__' in 
+00002760: 2741 7373 6574 2720 6275 7420 6469 646e  'Asset' but didn
+00002770: 2774 2064 6563 6c61 7265 2027 5f5f 6861  't declare '__ha
+00002780: 7368 5f5f 270a 0a66 6162 7269 6361 7465  sh__'..fabricate
+00002790: 5f76 616c 7565 0a5e 5e5e 5e5e 5e5e 5e5e  _value.^^^^^^^^^
+000027a0: 5e5e 5e5e 5e5e 0a52 756e 2061 2076 616c  ^^^^^^.Run a val
+000027b0: 7565 2074 6872 6f75 6768 2061 2063 616c  ue through a cal
+000027c0: 6c61 626c 6520 6661 6374 6f72 7920 286f  lable factory (o
+000027d0: 7220 4e6f 6e65 292e 0a0a 2e2e 2063 6f64  r None)..... cod
+000027e0: 653a 3a20 7079 7468 6f6e 0a0a 2020 2020  e:: python..    
+000027f0: 3e3e 3e20 6672 6f6d 2062 6173 6963 636f  >>> from basicco
+00002800: 2e66 6162 7269 6361 7465 5f76 616c 7565  .fabricate_value
+00002810: 2069 6d70 6f72 7420 6661 6272 6963 6174   import fabricat
+00002820: 655f 7661 6c75 650a 2020 2020 3e3e 3e20  e_value.    >>> 
+00002830: 6661 6272 6963 6174 655f 7661 6c75 6528  fabricate_value(
+00002840: 4e6f 6e65 2c20 3329 2020 2320 6e6f 2066  None, 3)  # no f
+00002850: 6163 746f 7279 2c20 7661 6c75 6520 7061  actory, value pa
+00002860: 7373 7468 726f 7567 680a 2020 2020 330a  ssthrough.    3.
+00002870: 2020 2020 3e3e 3e20 6661 6272 6963 6174      >>> fabricat
+00002880: 655f 7661 6c75 6528 7374 722c 2033 2920  e_value(str, 3) 
+00002890: 2023 2063 616c 6c61 626c 6520 6661 6374   # callable fact
+000028a0: 6f72 790a 2020 2020 2733 270a 2020 2020  ory.    '3'.    
+000028b0: 3e3e 3e20 6661 6272 6963 6174 655f 7661  >>> fabricate_va
+000028c0: 6c75 6528 2273 7472 222c 2033 2920 2023  lue("str", 3)  #
+000028d0: 2075 7365 2061 6e20 696d 706f 7274 2070   use an import p
+000028e0: 6174 680a 2020 2020 2733 270a 2020 2020  ath.    '3'.    
+000028f0: 3e3e 3e20 6661 6272 6963 6174 655f 7661  >>> fabricate_va
+00002900: 6c75 6528 696e 7429 2020 2320 6e6f 2069  lue(int)  # no i
+00002910: 6e70 7574 2076 616c 7565 2c20 6a75 7374  nput value, just
+00002920: 2074 6865 2066 6163 746f 7279 2069 7473   the factory its
+00002930: 656c 660a 2020 2020 300a 0a67 6574 5f6d  elf.    0..get_m
+00002940: 726f 0a5e 5e5e 5e5e 5e5e 0a47 6574 2063  ro.^^^^^^^.Get c
+00002950: 6f6e 7369 7374 656e 7420 4d52 4f20 616d  onsistent MRO am
+00002960: 6f6e 6773 7420 6469 6666 6572 656e 7420  ongst different 
+00002970: 7079 7468 6f6e 2076 6572 7369 6f6e 732e  python versions.
+00002980: 2054 6869 7320 776f 726b 7320 6576 656e   This works even
+00002990: 2077 6974 6820 6765 6e65 7269 6320 636c   with generic cl
+000029a0: 6173 7365 7320 696e 2050 7974 686f 6e20  asses in Python 
+000029b0: 322e 372e 0a0a 2e2e 2063 6f64 653a 3a20  2.7..... code:: 
+000029c0: 7079 7468 6f6e 0a0a 2020 2020 3e3e 3e20  python..    >>> 
+000029d0: 6672 6f6d 2073 6978 2069 6d70 6f72 7420  from six import 
+000029e0: 7769 7468 5f6d 6574 6163 6c61 7373 0a20  with_metaclass. 
+000029f0: 2020 203e 3e3e 2066 726f 6d20 7469 7070     >>> from tipp
+00002a00: 6f20 696d 706f 7274 2047 656e 6572 6963  o import Generic
+00002a10: 2c20 5479 7065 5661 720a 2020 2020 3e3e  , TypeVar.    >>
+00002a20: 3e20 6672 6f6d 2062 6173 6963 636f 2e67  > from basicco.g
+00002a30: 6574 5f6d 726f 2069 6d70 6f72 7420 6765  et_mro import ge
+00002a40: 745f 6d72 6f0a 2020 2020 3e3e 3e20 5420  t_mro.    >>> T 
+00002a50: 3d20 5479 7065 5661 7228 2254 2229 0a20  = TypeVar("T"). 
+00002a60: 2020 203e 3e3e 2063 6c61 7373 204d 7947     >>> class MyG
+00002a70: 656e 6572 6963 2847 656e 6572 6963 5b54  eneric(Generic[T
+00002a80: 5d29 3a0a 2020 2020 2e2e 2e20 2020 2020  ]):.    ...     
+00002a90: 7061 7373 0a20 2020 202e 2e2e 0a20 2020  pass.    ....   
+00002aa0: 203e 3e3e 2063 6c61 7373 2053 7562 436c   >>> class SubCl
+00002ab0: 6173 7328 4d79 4765 6e65 7269 635b 545d  ass(MyGeneric[T]
+00002ac0: 293a 0a20 2020 202e 2e2e 2020 2020 2070  ):.    ...     p
+00002ad0: 6173 730a 2020 2020 2e2e 2e0a 2020 2020  ass.    ....    
+00002ae0: 3e3e 3e20 636c 6173 7320 4d69 7865 6428  >>> class Mixed(
+00002af0: 5375 6243 6c61 7373 5b54 5d2c 204d 7947  SubClass[T], MyG
+00002b00: 656e 6572 6963 5b54 5d29 3a0a 2020 2020  eneric[T]):.    
+00002b10: 2e2e 2e20 2020 2020 7061 7373 0a20 2020  ...     pass.   
+00002b20: 202e 2e2e 0a20 2020 203e 3e3e 205b 632e   ....    >>> [c.
+00002b30: 5f5f 6e61 6d65 5f5f 2066 6f72 2063 2069  __name__ for c i
+00002b40: 6e20 6765 745f 6d72 6f28 4d69 7865 6429  n get_mro(Mixed)
+00002b50: 5d0a 2020 2020 5b27 4d69 7865 6427 2c20  ].    ['Mixed', 
+00002b60: 2753 7562 436c 6173 7327 2c20 274d 7947  'SubClass', 'MyG
+00002b70: 656e 6572 6963 272c 2027 4765 6e65 7269  eneric', 'Generi
+00002b80: 6327 2c20 276f 626a 6563 7427 5d0a 0a68  c', 'object']..h
+00002b90: 6173 685f 6361 6368 655f 7772 6170 7065  ash_cache_wrappe
+00002ba0: 720a 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e  r.^^^^^^^^^^^^^^
+00002bb0: 5e5e 5e5e 0a41 6e20 696e 7465 6765 7220  ^^^^.An integer 
+00002bc0: 7375 6263 6c61 7373 2074 6861 7420 7069  subclass that pi
+00002bd0: 636b 6c65 732f 636f 7069 6573 2061 7320  ckles/copies as 
+00002be0: 4e6f 6e65 2e20 5468 6973 2063 616e 2062  None. This can b
+00002bf0: 6520 7573 6564 2074 6f20 6176 6f69 6420  e used to avoid 
+00002c00: 7365 7269 616c 697a 696e 6720 6120 6361  serializing a ca
+00002c10: 6368 6564 2068 6173 6820 7661 6c75 652e  ched hash value.
+00002c20: 0a0a 2e2e 2063 6f64 653a 3a20 7079 7468  .... code:: pyth
+00002c30: 6f6e 0a0a 2020 2020 3e3e 3e20 6672 6f6d  on..    >>> from
+00002c40: 2063 6f70 7920 696d 706f 7274 2063 6f70   copy import cop
+00002c50: 790a 2020 2020 3e3e 3e20 6672 6f6d 2062  y.    >>> from b
+00002c60: 6173 6963 636f 2e68 6173 685f 6361 6368  asicco.hash_cach
+00002c70: 655f 7772 6170 7065 7220 696d 706f 7274  e_wrapper import
+00002c80: 2048 6173 6843 6163 6865 5772 6170 7065   HashCacheWrappe
+00002c90: 720a 2020 2020 3e3e 3e20 6861 7368 5f63  r.    >>> hash_c
+00002ca0: 6163 6865 203d 2048 6173 6843 6163 6865  ache = HashCache
+00002cb0: 5772 6170 7065 7228 3132 3334 3529 0a20  Wrapper(12345). 
+00002cc0: 2020 203e 3e3e 2070 7269 6e74 2868 6173     >>> print(has
+00002cd0: 685f 6361 6368 6529 0a20 2020 2031 3233  h_cache).    123
+00002ce0: 3435 0a20 2020 203e 3e3e 2070 7269 6e74  45.    >>> print
+00002cf0: 2863 6f70 7928 6861 7368 5f63 6163 6865  (copy(hash_cache
+00002d00: 2929 0a20 2020 204e 6f6e 650a 0a69 6d70  )).    None..imp
+00002d10: 6c69 6369 745f 6861 7368 0a5e 5e5e 5e5e  licit_hash.^^^^^
+00002d20: 5e5e 5e5e 5e5e 5e5e 0a4d 6574 6163 6c61  ^^^^^^^^.Metacla
+00002d30: 7373 2074 6861 7420 666f 7263 6573 2060  ss that forces `
+00002d40: 5f5f 6861 7368 5f5f 6020 746f 204e 6f6e  __hash__` to Non
+00002d50: 6520 7768 656e 2060 5f5f 6571 5f5f 6020  e when `__eq__` 
+00002d60: 6973 2064 6563 6c61 7265 642e 0a54 6869  is declared..Thi
+00002d70: 7320 6973 2061 2062 6163 6b70 6f72 7420  s is a backport 
+00002d80: 6f66 2074 6865 2064 6566 6175 6c74 2062  of the default b
+00002d90: 6568 6176 696f 7220 696e 2050 7974 686f  ehavior in Pytho
+00002da0: 6e20 332e 0a0a 2e2e 2063 6f64 653a 3a20  n 3..... code:: 
 00002db0: 7079 7468 6f6e 0a0a 2020 2020 3e3e 3e20  python..    >>> 
-00002dc0: 6672 6f6d 2063 6f70 7920 696d 706f 7274  from copy import
-00002dd0: 2063 6f70 790a 2020 2020 3e3e 3e20 6672   copy.    >>> fr
-00002de0: 6f6d 2062 6173 6963 636f 2e68 6173 685f  om basicco.hash_
-00002df0: 6361 6368 655f 7772 6170 7065 7220 696d  cache_wrapper im
-00002e00: 706f 7274 2048 6173 6843 6163 6865 5772  port HashCacheWr
-00002e10: 6170 7065 720a 2020 2020 3e3e 3e20 6861  apper.    >>> ha
-00002e20: 7368 5f63 6163 6865 203d 2048 6173 6843  sh_cache = HashC
-00002e30: 6163 6865 5772 6170 7065 7228 3132 3334  acheWrapper(1234
-00002e40: 3529 0a20 2020 203e 3e3e 2070 7269 6e74  5).    >>> print
-00002e50: 2868 6173 685f 6361 6368 6529 0a20 2020  (hash_cache).   
-00002e60: 2031 3233 3435 0a20 2020 203e 3e3e 2070   12345.    >>> p
-00002e70: 7269 6e74 2863 6f70 7928 6861 7368 5f63  rint(copy(hash_c
-00002e80: 6163 6865 2929 0a20 2020 204e 6f6e 650a  ache)).    None.
-00002e90: 0a69 6d70 6c69 6369 745f 6861 7368 0a5e  .implicit_hash.^
-00002ea0: 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e 0a4d 6574  ^^^^^^^^^^^^.Met
-00002eb0: 6163 6c61 7373 2074 6861 7420 666f 7263  aclass that forc
-00002ec0: 6573 2060 5f5f 6861 7368 5f5f 6020 746f  es `__hash__` to
-00002ed0: 204e 6f6e 6520 7768 656e 2060 5f5f 6571   None when `__eq
-00002ee0: 5f5f 6020 6973 2064 6563 6c61 7265 642e  __` is declared.
-00002ef0: 0a54 6869 7320 6973 2061 2062 6163 6b70  .This is a backp
-00002f00: 6f72 7420 6f66 2074 6865 2064 6566 6175  ort of the defau
-00002f10: 6c74 2062 6568 6176 696f 7220 696e 2050  lt behavior in P
-00002f20: 7974 686f 6e20 332e 0a0a 2e2e 2063 6f64  ython 3..... cod
-00002f30: 653a 3a20 7079 7468 6f6e 0a0a 2020 2020  e:: python..    
-00002f40: 3e3e 3e20 6672 6f6d 2073 6978 2069 6d70  >>> from six imp
-00002f50: 6f72 7420 7769 7468 5f6d 6574 6163 6c61  ort with_metacla
-00002f60: 7373 0a20 2020 203e 3e3e 2066 726f 6d20  ss.    >>> from 
-00002f70: 6261 7369 6363 6f2e 696d 706c 6963 6974  basicco.implicit
-00002f80: 5f68 6173 6820 696d 706f 7274 2049 6d70  _hash import Imp
-00002f90: 6c69 6369 7448 6173 684d 6574 610a 2020  licitHashMeta.  
-00002fa0: 2020 3e3e 3e20 636c 6173 7320 4173 7365    >>> class Asse
-00002fb0: 7428 7769 7468 5f6d 6574 6163 6c61 7373  t(with_metaclass
-00002fc0: 2849 6d70 6c69 6369 7448 6173 684d 6574  (ImplicitHashMet
-00002fd0: 612c 206f 626a 6563 7429 293a 0a20 2020  a, object)):.   
-00002fe0: 202e 2e2e 2020 2020 2064 6566 205f 5f65   ...     def __e
-00002ff0: 715f 5f28 7365 6c66 2c20 6f74 6865 7229  q__(self, other)
-00003000: 3a0a 2020 2020 2e2e 2e20 2020 2020 2020  :.    ...       
-00003010: 2020 7061 7373 0a20 2020 202e 2e2e 0a20    pass.    .... 
-00003020: 2020 203e 3e3e 2041 7373 6574 2e5f 5f68     >>> Asset.__h
-00003030: 6173 685f 5f20 6973 204e 6f6e 650a 2020  ash__ is None.  
-00003040: 2020 5472 7565 0a0a 696d 706f 7274 5f70    True..import_p
-00003050: 6174 680a 5e5e 5e5e 5e5e 5e5e 5e5e 5e0a  ath.^^^^^^^^^^^.
-00003060: 4765 6e65 7261 7465 2069 6d70 6f72 7461  Generate importa
-00003070: 626c 6520 646f 7420 7061 7468 7320 616e  ble dot paths an
-00003080: 6420 696d 706f 7274 2066 726f 6d20 7468  d import from th
-00003090: 656d 2e0a 0a2e 2e20 636f 6465 3a3a 2070  em..... code:: p
-000030a0: 7974 686f 6e0a 0a20 2020 203e 3e3e 2069  ython..    >>> i
-000030b0: 6d70 6f72 7420 6974 6572 746f 6f6c 730a  mport itertools.
-000030c0: 2020 2020 3e3e 3e20 6672 6f6d 2062 6173      >>> from bas
-000030d0: 6963 636f 2e69 6d70 6f72 745f 7061 7468  icco.import_path
-000030e0: 2069 6d70 6f72 7420 6765 745f 7061 7468   import get_path
-000030f0: 2c20 696d 706f 7274 5f70 6174 680a 2020  , import_path.  
-00003100: 2020 3e3e 3e20 6765 745f 7061 7468 2869    >>> get_path(i
-00003110: 7465 7274 6f6f 6c73 2e63 6861 696e 290a  tertools.chain).
-00003120: 2020 2020 2769 7465 7274 6f6f 6c73 2e63      'itertools.c
-00003130: 6861 696e 270a 2020 2020 3e3e 3e20 696d  hain'.    >>> im
-00003140: 706f 7274 5f70 6174 6828 2269 7465 7274  port_path("itert
-00003150: 6f6f 6c73 2e63 6861 696e 2229 0a20 2020  ools.chain").   
-00003160: 203c 2e2e 2e20 2769 7465 7274 6f6f 6c73   <... 'itertools
-00003170: 2e63 6861 696e 273e 0a0a 2e2e 2063 6f64  .chain'>.... cod
-00003180: 653a 3a20 7079 7468 6f6e 0a0a 2020 2020  e:: python..    
-00003190: 3e3e 3e20 6672 6f6d 2062 6173 6963 636f  >>> from basicco
-000031a0: 2e69 6d70 6f72 745f 7061 7468 2069 6d70  .import_path imp
-000031b0: 6f72 7420 6578 7472 6163 745f 6765 6e65  ort extract_gene
-000031c0: 7269 635f 7061 7468 730a 2020 2020 3e3e  ric_paths.    >>
-000031d0: 3e20 6578 7472 6163 745f 6765 6e65 7269  > extract_generi
-000031e0: 635f 7061 7468 7328 2254 7570 6c65 5b69  c_paths("Tuple[i
-000031f0: 6e74 2c20 7374 725d 2229 0a20 2020 2028  nt, str]").    (
-00003200: 2754 7570 6c65 272c 2028 2769 6e74 272c  'Tuple', ('int',
-00003210: 2027 7374 7227 2929 0a0a 696e 6974 5f73   'str'))..init_s
-00003220: 7562 636c 6173 730a 5e5e 5e5e 5e5e 5e5e  ubclass.^^^^^^^^
-00003230: 5e5e 5e5e 5e0a 4261 636b 706f 7274 206f  ^^^^^.Backport o
-00003240: 6620 7468 6520 6675 6e63 7469 6f6e 616c  f the functional
-00003250: 6974 7920 6f66 2060 5f5f 696e 6974 5f73  ity of `__init_s
-00003260: 7562 636c 6173 735f 5f60 2066 726f 6d20  ubclass__` from 
-00003270: 5045 5020 3438 3720 746f 2050 7974 686f  PEP 487 to Pytho
-00003280: 6e20 322e 372e 0a54 6869 7320 776f 726b  n 2.7..This work
-00003290: 7320 666f 7220 626f 7468 2050 7974 686f  s for both Pytho
-000032a0: 6e20 3220 2875 7369 6e67 2060 5f5f 6b77  n 2 (using `__kw
-000032b0: 6172 6773 5f5f 6029 2061 6e64 2033 2028  args__`) and 3 (
-000032c0: 7573 696e 6720 7468 6520 6e65 7720 636c  using the new cl
-000032d0: 6173 7320 7061 7261 6d65 7465 7273 292e  ass parameters).
-000032e0: 0a0a 2e2e 2063 6f64 653a 3a20 7079 7468  .... code:: pyth
-000032f0: 6f6e 0a0a 2020 2020 3e3e 3e20 6672 6f6d  on..    >>> from
-00003300: 2062 6173 6963 636f 2e69 6e69 745f 7375   basicco.init_su
-00003310: 6263 6c61 7373 2069 6d70 6f72 7420 496e  bclass import In
-00003320: 6974 5375 6263 6c61 7373 0a20 2020 203e  itSubclass.    >
-00003330: 3e3e 2063 6c61 7373 2046 6f6f 2849 6e69  >> class Foo(Ini
-00003340: 7453 7562 636c 6173 7329 3a0a 2020 2020  tSubclass):.    
-00003350: 2e2e 2e20 2020 2020 6465 6620 5f5f 696e  ...     def __in
-00003360: 6974 5f73 7562 636c 6173 735f 5f28 636c  it_subclass__(cl
-00003370: 732c 2066 6f6f 3d4e 6f6e 652c 202a 2a6b  s, foo=None, **k
-00003380: 7761 7267 7329 3a0a 2020 2020 2e2e 2e20  wargs):.    ... 
-00003390: 2020 2020 2020 2020 636c 732e 666f 6f20          cls.foo 
-000033a0: 3d20 666f 6f0a 2020 2020 2e2e 2e0a 2020  = foo.    ....  
-000033b0: 2020 3e3e 3e20 636c 6173 7320 4261 7228    >>> class Bar(
-000033c0: 466f 6f29 3a0a 2020 2020 2e2e 2e20 2020  Foo):.    ...   
-000033d0: 2020 5f5f 6b77 6172 6773 5f5f 203d 207b    __kwargs__ = {
-000033e0: 2266 6f6f 223a 2022 6261 7222 7d20 2023  "foo": "bar"}  #
-000033f0: 2079 6f75 2063 616e 2073 7065 6369 6679   you can specify
-00003400: 2063 6c73 206b 7761 7267 7320 6f6e 2070   cls kwargs on p
-00003410: 7932 206c 696b 6520 7468 6973 0a20 2020  y2 like this.   
-00003420: 202e 2e2e 0a20 2020 203e 3e3e 2042 6172   ....    >>> Bar
-00003430: 2e66 6f6f 0a20 2020 2027 6261 7227 0a0a  .foo.    'bar'..
-00003440: 6c6f 636b 6564 5f63 6c61 7373 0a5e 5e5e  locked_class.^^^
-00003450: 5e5e 5e5e 5e5e 5e5e 5e5e 0a50 7265 7665  ^^^^^^^^^^.Preve
-00003460: 6e74 7320 6368 616e 6769 6e67 2070 7562  nts changing pub
-00003470: 6c69 6320 636c 6173 7320 6174 7472 6962  lic class attrib
-00003480: 7574 6573 2e0a 0a2e 2e20 636f 6465 3a3a  utes..... code::
-00003490: 2070 7974 686f 6e0a 0a20 2020 203e 3e3e   python..    >>>
-000034a0: 2066 726f 6d20 7369 7820 696d 706f 7274   from six import
-000034b0: 2077 6974 685f 6d65 7461 636c 6173 730a   with_metaclass.
-000034c0: 2020 2020 3e3e 3e20 6672 6f6d 2062 6173      >>> from bas
-000034d0: 6963 636f 2e6c 6f63 6b65 645f 636c 6173  icco.locked_clas
-000034e0: 7320 696d 706f 7274 204c 6f63 6b65 6443  s import LockedC
-000034f0: 6c61 7373 4d65 7461 0a20 2020 203e 3e3e  lassMeta.    >>>
-00003500: 2063 6c61 7373 2046 6f6f 2877 6974 685f   class Foo(with_
-00003510: 6d65 7461 636c 6173 7328 4c6f 636b 6564  metaclass(Locked
-00003520: 436c 6173 734d 6574 612c 206f 626a 6563  ClassMeta, objec
-00003530: 7429 293a 0a20 2020 202e 2e2e 2020 2020  t)):.    ...    
-00003540: 2070 6173 730a 2020 2020 2e2e 2e0a 2020   pass.    ....  
-00003550: 2020 3e3e 3e20 466f 6f2e 6261 7220 3d20    >>> Foo.bar = 
-00003560: 2262 6172 220a 2020 2020 5472 6163 6562  "bar".    Traceb
-00003570: 6163 6b20 286d 6f73 7420 7265 6365 6e74  ack (most recent
-00003580: 2063 616c 6c20 6c61 7374 293a 0a20 2020   call last):.   
-00003590: 2041 7474 7269 6275 7465 4572 726f 723a   AttributeError:
-000035a0: 2063 616e 2774 2073 6574 2072 6561 642d   can't set read-
-000035b0: 6f6e 6c79 2063 6c61 7373 2061 7474 7269  only class attri
-000035c0: 6275 7465 2027 6261 7227 0a0a 6d61 6e67  bute 'bar'..mang
-000035d0: 6c69 6e67 0a5e 5e5e 5e5e 5e5e 5e0a 4675  ling.^^^^^^^^.Fu
-000035e0: 6e63 7469 6f6e 7320 746f 206d 616e 676c  nctions to mangl
-000035f0: 652f 756e 6d61 6e67 6c65 2f65 7874 7261  e/unmangle/extra
-00003600: 6374 2070 7269 7661 7465 206e 616d 6573  ct private names
-00003610: 2e0a 0a2e 2e20 636f 6465 3a3a 2070 7974  ..... code:: pyt
-00003620: 686f 6e0a 0a20 2020 203e 3e3e 2066 726f  hon..    >>> fro
-00003630: 6d20 6261 7369 6363 6f2e 6d61 6e67 6c69  m basicco.mangli
-00003640: 6e67 2069 6d70 6f72 7420 6d61 6e67 6c65  ng import mangle
-00003650: 2c20 756e 6d61 6e67 6c65 2c20 6578 7472  , unmangle, extr
-00003660: 6163 740a 2020 2020 3e3e 3e20 6d61 6e67  act.    >>> mang
-00003670: 6c65 2822 5f5f 6d65 6d62 6572 222c 2022  le("__member", "
-00003680: 466f 6f22 290a 2020 2020 275f 466f 6f5f  Foo").    '_Foo_
-00003690: 5f6d 656d 6265 7227 0a20 2020 203e 3e3e  _member'.    >>>
-000036a0: 2075 6e6d 616e 676c 6528 225f 466f 6f5f   unmangle("_Foo_
-000036b0: 5f6d 656d 6265 7222 2c20 2246 6f6f 2229  _member", "Foo")
-000036c0: 0a20 2020 2027 5f5f 6d65 6d62 6572 270a  .    '__member'.
-000036d0: 2020 2020 3e3e 3e20 6578 7472 6163 7428      >>> extract(
-000036e0: 225f 466f 6f5f 5f6d 656d 6265 7222 290a  "_Foo__member").
-000036f0: 2020 2020 2827 5f5f 6d65 6d62 6572 272c      ('__member',
-00003700: 2027 466f 6f27 290a 0a6d 6170 7069 6e67   'Foo')..mapping
-00003710: 5f70 726f 7879 0a5e 5e5e 5e5e 5e5e 5e5e  _proxy.^^^^^^^^^
-00003720: 5e5e 5e5e 0a4d 6170 7069 6e67 2050 726f  ^^^^.Mapping Pro
-00003730: 7879 2074 7970 6520 2872 6561 642d 6f6e  xy type (read-on
-00003740: 6c79 2920 666f 7220 6f6c 6465 7220 5079  ly) for older Py
-00003750: 7468 6f6e 2076 6572 7369 6f6e 732e 0a0a  thon versions...
-00003760: 2e2e 2063 6f64 653a 3a20 7079 7468 6f6e  .. code:: python
-00003770: 0a0a 2020 2020 3e3e 3e20 6672 6f6d 2062  ..    >>> from b
-00003780: 6173 6963 636f 2e6d 6170 7069 6e67 5f70  asicco.mapping_p
-00003790: 726f 7879 2069 6d70 6f72 7420 4d61 7070  roxy import Mapp
-000037a0: 696e 6750 726f 7879 5479 7065 0a20 2020  ingProxyType.   
-000037b0: 203e 3e3e 2069 6e74 6572 6e61 6c5f 6469   >>> internal_di
-000037c0: 6374 203d 207b 2266 6f6f 223a 2022 6261  ct = {"foo": "ba
-000037d0: 7222 7d0a 2020 2020 3e3e 3e20 7072 6f78  r"}.    >>> prox
-000037e0: 795f 6469 6374 203d 204d 6170 7069 6e67  y_dict = Mapping
-000037f0: 5072 6f78 7954 7970 6528 696e 7465 726e  ProxyType(intern
-00003800: 616c 5f64 6963 7429 0a20 2020 203e 3e3e  al_dict).    >>>
-00003810: 2070 726f 7879 5f64 6963 745b 2266 6f6f   proxy_dict["foo
-00003820: 225d 0a20 2020 2027 6261 7227 0a0a 6e61  "].    'bar'..na
-00003830: 6d65 645f 7475 706c 650a 5e5e 5e5e 5e5e  med_tuple.^^^^^^
-00003840: 5e5e 5e5e 5e0a 4e61 6d65 6420 5475 706c  ^^^^^.Named Tupl
-00003850: 6520 7574 696c 6974 6965 732e 0a0a 4578  e utilities...Ex
-00003860: 616d 706c 6520 6f66 2060 6465 6661 756c  ample of `defaul
-00003870: 7473 6020 6465 636f 7261 746f 722f 6675  ts` decorator/fu
-00003880: 6e63 7469 6f6e 2074 6f20 7365 7420 6120  nction to set a 
-00003890: 4e61 6d65 6420 5475 706c 6527 7320 6465  Named Tuple's de
-000038a0: 6661 756c 7420 7661 6c75 6573 3a0a 0a2e  fault values:...
-000038b0: 2e20 636f 6465 3a3a 2070 7974 686f 6e0a  . code:: python.
-000038c0: 0a20 2020 203e 3e3e 2066 726f 6d20 636f  .    >>> from co
-000038d0: 6c6c 6563 7469 6f6e 7320 696d 706f 7274  llections import
-000038e0: 206e 616d 6564 7475 706c 650a 2020 2020   namedtuple.    
-000038f0: 3e3e 3e20 6672 6f6d 2062 6173 6963 636f  >>> from basicco
-00003900: 2e6e 616d 6564 5f74 7570 6c65 2069 6d70  .named_tuple imp
-00003910: 6f72 7420 6465 6661 756c 7473 0a20 2020  ort defaults.   
-00003920: 203e 3e3e 2050 6f69 6e74 203d 2064 6566   >>> Point = def
-00003930: 6175 6c74 7328 6e61 6d65 3d22 666f 6f22  aults(name="foo"
-00003940: 2928 6e61 6d65 6474 7570 6c65 2822 506f  )(namedtuple("Po
-00003950: 696e 7422 2c20 2822 7822 2c20 2279 222c  int", ("x", "y",
-00003960: 2022 6e61 6d65 2229 2929 0a20 2020 203e   "name"))).    >
-00003970: 3e3e 2050 6f69 6e74 2831 2c20 3229 0a20  >> Point(1, 2). 
-00003980: 2020 2050 6f69 6e74 2878 3d31 2c20 793d     Point(x=1, y=
-00003990: 322c 206e 616d 653d 2766 6f6f 2729 0a0a  2, name='foo')..
-000039a0: 6e61 6d65 7370 6163 650a 5e5e 5e5e 5e5e  namespace.^^^^^^
-000039b0: 5e5e 5e0a 5772 6170 7320 6120 6469 6374  ^^^.Wraps a dict
-000039c0: 696f 6e61 7279 2f6d 6170 7069 6e67 2061  ionary/mapping a
-000039d0: 6e64 2070 726f 7669 6465 7320 6174 7472  nd provides attr
-000039e0: 6962 7574 652d 7374 796c 6520 6163 6365  ibute-style acce
-000039f0: 7373 2074 6f20 6974 2e0a 0a2e 2e20 636f  ss to it..... co
-00003a00: 6465 3a3a 2070 7974 686f 6e0a 0a20 2020  de:: python..   
-00003a10: 203e 3e3e 2066 726f 6d20 6261 7369 6363   >>> from basicc
-00003a20: 6f2e 6e61 6d65 7370 6163 6520 696d 706f  o.namespace impo
-00003a30: 7274 204e 616d 6573 7061 6365 0a20 2020  rt Namespace.   
-00003a40: 203e 3e3e 206e 7320 3d20 4e61 6d65 7370   >>> ns = Namesp
-00003a50: 6163 6528 7b22 6261 7222 3a20 2266 6f6f  ace({"bar": "foo
-00003a60: 227d 290a 2020 2020 3e3e 3e20 6e73 2e62  "}).    >>> ns.b
-00003a70: 6172 0a20 2020 2027 666f 6f27 0a0a 2e2e  ar.    'foo'....
-00003a80: 2063 6f64 653a 3a20 7079 7468 6f6e 0a0a   code:: python..
-00003a90: 2020 2020 3e3e 3e20 6672 6f6d 2062 6173      >>> from bas
-00003aa0: 6963 636f 2e6e 616d 6573 7061 6365 2069  icco.namespace i
-00003ab0: 6d70 6f72 7420 4d75 7461 626c 654e 616d  mport MutableNam
-00003ac0: 6573 7061 6365 0a20 2020 203e 3e3e 206e  espace.    >>> n
-00003ad0: 7320 3d20 4d75 7461 626c 654e 616d 6573  s = MutableNames
-00003ae0: 7061 6365 287b 2262 6172 223a 2022 666f  pace({"bar": "fo
-00003af0: 6f22 7d29 0a20 2020 203e 3e3e 206e 732e  o"}).    >>> ns.
-00003b00: 666f 6f20 3d20 2262 6172 220a 2020 2020  foo = "bar".    
-00003b10: 3e3e 3e20 6e73 2e66 6f6f 0a20 2020 2027  >>> ns.foo.    '
-00003b20: 6261 7227 0a20 2020 203e 3e3e 206e 732e  bar'.    >>> ns.
-00003b30: 6261 720a 2020 2020 2766 6f6f 270a 0a41  bar.    'foo'..A
-00003b40: 6c73 6f20 7072 6f76 6964 6573 2061 2060  lso provides a `
-00003b50: 4e61 6d65 7370 6163 6564 4d65 7461 6020  NamespacedMeta` 
-00003b60: 6d65 7461 636c 6173 7320 7468 6174 2061  metaclass that a
-00003b70: 6464 7320 6120 605f 5f6e 616d 6573 7061  dds a `__namespa
-00003b80: 6365 6020 7072 6f74 6563 7465 6420 636c  ce` protected cl
-00003b90: 6173 7320 6174 7472 6962 7574 6520 7468  ass attribute th
-00003ba0: 6174 2069 7320 756e 6971 7565 2074 6f20  at is unique to 
-00003bb0: 6561 6368 0a63 6c61 7373 2e0a 0a2e 2e20  each.class..... 
-00003bc0: 636f 6465 3a3a 2070 7974 686f 6e0a 0a20  code:: python.. 
-00003bd0: 2020 203e 3e3e 2066 726f 6d20 7369 7820     >>> from six 
-00003be0: 696d 706f 7274 2077 6974 685f 6d65 7461  import with_meta
-00003bf0: 636c 6173 730a 2020 2020 3e3e 3e20 6672  class.    >>> fr
-00003c00: 6f6d 2062 6173 6963 636f 2e6e 616d 6573  om basicco.names
-00003c10: 7061 6365 2069 6d70 6f72 7420 4e61 6d65  pace import Name
-00003c20: 7370 6163 6564 4d65 7461 0a20 2020 203e  spacedMeta.    >
-00003c30: 3e3e 2063 6c61 7373 2041 7373 6574 2877  >> class Asset(w
-00003c40: 6974 685f 6d65 7461 636c 6173 7328 4e61  ith_metaclass(Na
-00003c50: 6d65 7370 6163 6564 4d65 7461 2c20 6f62  mespacedMeta, ob
-00003c60: 6a65 6374 2929 3a0a 2020 2020 2e2e 2e20  ject)):.    ... 
-00003c70: 2020 2020 4063 6c61 7373 6d65 7468 6f64      @classmethod
-00003c80: 0a20 2020 202e 2e2e 2020 2020 2064 6566  .    ...     def
-00003c90: 2073 6574 5f63 6c61 7373 5f76 616c 7565   set_class_value
-00003ca0: 2863 6c73 2c20 7661 6c75 6529 3a0a 2020  (cls, value):.  
-00003cb0: 2020 2e2e 2e20 2020 2020 2020 2020 636c    ...         cl
-00003cc0: 732e 5f5f 6e61 6d65 7370 6163 652e 7661  s.__namespace.va
-00003cd0: 6c75 6520 3d20 7661 6c75 650a 2020 2020  lue = value.    
-00003ce0: 2e2e 2e0a 2020 2020 2e2e 2e20 2020 2020  ....    ...     
-00003cf0: 4063 6c61 7373 6d65 7468 6f64 0a20 2020  @classmethod.   
-00003d00: 202e 2e2e 2020 2020 2064 6566 2067 6574   ...     def get
-00003d10: 5f63 6c61 7373 5f76 616c 7565 2863 6c73  _class_value(cls
-00003d20: 293a 0a20 2020 202e 2e2e 2020 2020 2020  ):.    ...      
-00003d30: 2020 2072 6574 7572 6e20 636c 732e 5f5f     return cls.__
-00003d40: 6e61 6d65 7370 6163 652e 7661 6c75 650a  namespace.value.
-00003d50: 2020 2020 2e2e 2e0a 2020 2020 3e3e 3e20      ....    >>> 
-00003d60: 4173 7365 742e 7365 745f 636c 6173 735f  Asset.set_class_
-00003d70: 7661 6c75 6528 2266 6f6f 6261 7222 290a  value("foobar").
-00003d80: 2020 2020 3e3e 3e20 4173 7365 742e 6765      >>> Asset.ge
-00003d90: 745f 636c 6173 735f 7661 6c75 6528 290a  t_class_value().
-00003da0: 2020 2020 2766 6f6f 6261 7227 0a0a 6f62      'foobar'..ob
-00003db0: 6a5f 7374 6174 650a 5e5e 5e5e 5e5e 5e5e  j_state.^^^^^^^^
-00003dc0: 5e0a 4765 742f 7570 6461 7465 2074 6865  ^.Get/update the
-00003dd0: 2073 7461 7465 206f 6620 616e 206f 626a   state of an obj
-00003de0: 6563 742c 2073 6c6f 7474 6564 206f 7220  ect, slotted or 
-00003df0: 6e6f 7420 2877 6f72 6b73 2065 7665 6e20  not (works even 
-00003e00: 696e 2050 7974 686f 6e20 322e 3729 2e0a  in Python 2.7)..
-00003e10: 0a2e 2e20 636f 6465 3a3a 2070 7974 686f  ... code:: pytho
-00003e20: 6e0a 0a20 2020 203e 3e3e 2066 726f 6d20  n..    >>> from 
-00003e30: 6261 7369 6363 6f2e 6f62 6a5f 7374 6174  basicco.obj_stat
-00003e40: 6520 696d 706f 7274 2067 6574 5f73 7461  e import get_sta
-00003e50: 7465 0a20 2020 203e 3e3e 2063 6c61 7373  te.    >>> class
-00003e60: 2053 6c6f 7474 6564 286f 626a 6563 7429   Slotted(object)
-00003e70: 3a0a 2020 2020 2e2e 2e20 2020 2020 5f5f  :.    ...     __
-00003e80: 736c 6f74 735f 5f20 3d20 2822 666f 6f22  slots__ = ("foo"
-00003e90: 2c20 2262 6172 2229 0a20 2020 202e 2e2e  , "bar").    ...
-00003ea0: 2020 2020 2064 6566 205f 5f69 6e69 745f       def __init_
-00003eb0: 5f28 7365 6c66 2c20 666f 6f2c 2062 6172  _(self, foo, bar
-00003ec0: 293a 0a20 2020 202e 2e2e 2020 2020 2020  ):.    ...      
-00003ed0: 2020 2073 656c 662e 666f 6f20 3d20 666f     self.foo = fo
-00003ee0: 6f0a 2020 2020 2e2e 2e20 2020 2020 2020  o.    ...       
-00003ef0: 2020 7365 6c66 2e62 6172 203d 2062 6172    self.bar = bar
-00003f00: 0a20 2020 202e 2e2e 0a20 2020 203e 3e3e  .    ....    >>>
-00003f10: 2073 6c6f 7474 6564 203d 2053 6c6f 7474   slotted = Slott
-00003f20: 6564 2822 6122 2c20 2262 2229 0a20 2020  ed("a", "b").   
-00003f30: 203e 3e3e 2073 6f72 7465 6428 6765 745f   >>> sorted(get_
-00003f40: 7374 6174 6528 736c 6f74 7465 6429 2e69  state(slotted).i
-00003f50: 7465 6d73 2829 290a 2020 2020 5b28 2762  tems()).    [('b
-00003f60: 6172 272c 2027 6227 292c 2028 2766 6f6f  ar', 'b'), ('foo
-00003f70: 272c 2027 6127 295d 0a0a 416c 736f 2070  ', 'a')]..Also p
-00003f80: 726f 7669 6465 7320 6120 6052 6564 7563  rovides a `Reduc
-00003f90: 6962 6c65 4d65 7461 6020 6d65 7461 636c  ibleMeta` metacl
-00003fa0: 6173 7320 7468 6174 2061 6c6c 6f77 7320  ass that allows 
-00003fb0: 666f 7220 7069 636b 6c69 6e67 2069 6e73  for pickling ins
-00003fc0: 7461 6e63 6573 206f 6620 736c 6f74 7465  tances of slotte
-00003fd0: 6420 636c 6173 7365 7320 696e 2050 7974  d classes in Pyt
-00003fe0: 686f 6e20 322e 372e 0a0a 7175 616c 6e61  hon 2.7...qualna
-00003ff0: 6d65 0a5e 5e5e 5e5e 5e5e 5e0a 5079 7468  me.^^^^^^^^.Pyth
-00004000: 6f6e 2032 2e37 2063 6f6d 7061 7469 626c  on 2.7 compatibl
-00004010: 6520 7761 7920 6f66 2067 6574 7469 6e67  e way of getting
-00004020: 2074 6865 2071 7561 6c69 6669 6564 206e   the qualified n
-00004030: 616d 652e 2042 6173 6564 206f 6e0a 6077  ame. Based on.`w
-00004040: 626f 6c73 7465 722f 7175 616c 6e61 6d65  bolster/qualname
-00004050: 203c 6874 7470 733a 2f2f 6769 7468 7562   <https://github
-00004060: 2e63 6f6d 2f77 626f 6c73 7465 722f 7175  .com/wbolster/qu
-00004070: 616c 6e61 6d65 3e60 5f2e 0a41 6c73 6f20  alname>`_..Also 
-00004080: 7072 6f76 6964 6573 2061 2060 5175 616c  provides a `Qual
-00004090: 6e61 6d65 644d 6574 6160 206d 6574 6163  namedMeta` metac
-000040a0: 6c61 7373 2077 6974 6820 6120 605f 5f71  lass with a `__q
-000040b0: 7561 6c6e 616d 655f 5f60 2063 6c61 7373  ualname__` class
-000040c0: 2070 726f 7065 7274 7920 666f 7220 5079   property for Py
-000040d0: 7468 6f6e 2032 2e37 2e0a 0a72 6563 7572  thon 2.7...recur
-000040e0: 7369 7665 5f72 6570 720a 5e5e 5e5e 5e5e  sive_repr.^^^^^^
-000040f0: 5e5e 5e5e 5e5e 5e5e 0a44 6563 6f72 6174  ^^^^^^^^.Decorat
-00004100: 6f72 2074 6861 7420 7072 6576 656e 7473  or that prevents
-00004110: 2069 6e66 696e 6974 6520 7265 6375 7273   infinite recurs
-00004120: 696f 6e20 666f 7220 605f 5f72 6570 725f  ion for `__repr_
-00004130: 5f60 206d 6574 686f 6473 2e0a 0a2e 2e20  _` methods..... 
-00004140: 636f 6465 3a3a 2070 7974 686f 6e0a 0a20  code:: python.. 
-00004150: 2020 203e 3e3e 2066 726f 6d20 6261 7369     >>> from basi
-00004160: 6363 6f2e 7265 6375 7273 6976 655f 7265  cco.recursive_re
-00004170: 7072 2069 6d70 6f72 7420 7265 6375 7273  pr import recurs
-00004180: 6976 655f 7265 7072 0a20 2020 203e 3e3e  ive_repr.    >>>
-00004190: 2063 6c61 7373 204d 7943 6c61 7373 286f   class MyClass(o
-000041a0: 626a 6563 7429 3a0a 2020 2020 2e2e 2e0a  bject):.    ....
-000041b0: 2020 2020 2e2e 2e20 2020 2020 4072 6563      ...     @rec
-000041c0: 7572 7369 7665 5f72 6570 720a 2020 2020  ursive_repr.    
-000041d0: 2e2e 2e20 2020 2020 6465 6620 5f5f 7265  ...     def __re
-000041e0: 7072 5f5f 2873 656c 6629 3a0a 2020 2020  pr__(self):.    
-000041f0: 2e2e 2e20 2020 2020 2020 2020 7265 7475  ...         retu
-00004200: 726e 2022 4d79 436c 6173 733c 7b21 727d  rn "MyClass<{!r}
-00004210: 3e22 2e66 6f72 6d61 7428 7365 6c66 290a  >".format(self).
-00004220: 2020 2020 2e2e 2e0a 2020 2020 3e3e 3e20      ....    >>> 
-00004230: 6d79 5f6f 626a 203d 204d 7943 6c61 7373  my_obj = MyClass
-00004240: 2829 0a20 2020 203e 3e3e 2072 6570 7228  ().    >>> repr(
-00004250: 6d79 5f6f 626a 290a 2020 2020 274d 7943  my_obj).    'MyC
-00004260: 6c61 7373 3c2e 2e2e 3e27 0a0a 7275 6e74  lass<...>'..runt
-00004270: 696d 655f 6669 6e61 6c0a 5e5e 5e5e 5e5e  ime_final.^^^^^^
-00004280: 5e5e 5e5e 5e5e 5e0a 5275 6e74 696d 652d  ^^^^^^^.Runtime-
-00004290: 6368 6563 6b65 6420 7665 7273 696f 6e20  checked version 
-000042a0: 6f66 2074 6865 2060 7479 7069 6e67 2e66  of the `typing.f
-000042b0: 696e 616c 203c 6874 7470 733a 2f2f 646f  inal <https://do
-000042c0: 6373 2e70 7974 686f 6e2e 6f72 672f 332f  cs.python.org/3/
-000042d0: 6c69 6272 6172 792f 7479 7069 6e67 2e68  library/typing.h
-000042e0: 746d 6c23 7479 7069 6e67 2e66 696e 616c  tml#typing.final
-000042f0: 3e60 5f20 6465 636f 7261 746f 722e 0a0a  >`_ decorator...
-00004300: 4361 6e20 6265 2075 7365 6420 6f6e 206d  Can be used on m
-00004310: 6574 686f 6473 2c20 7072 6f70 6572 7469  ethods, properti
-00004320: 6573 2c20 636c 6173 736d 6574 686f 6473  es, classmethods
-00004330: 2c20 7374 6174 6963 6d65 7468 6f64 732c  , staticmethods,
-00004340: 2061 6e64 2063 6c61 7373 6573 2074 6861   and classes tha
-00004350: 7420 6861 7665 2060 5275 6e74 696d 6546  t have `RuntimeF
-00004360: 696e 616c 4d65 7461 6020 6173 2061 206d  inalMeta` as a m
-00004370: 6574 6163 6c61 7373 2e0a 4974 2069 7320  etaclass..It is 
-00004380: 616c 736f 2072 6563 6f67 6e69 7a65 6420  also recognized 
-00004390: 6279 2073 7461 7469 6320 7479 7065 2063  by static type c
-000043a0: 6865 636b 6572 7320 616e 6420 7072 6576  heckers and prev
-000043b0: 656e 7473 2073 7562 636c 6173 7369 6e67  ents subclassing
-000043c0: 2061 6e64 2f6f 7220 6d65 6d62 6572 206f   and/or member o
-000043d0: 7665 7272 6964 696e 6720 6475 7269 6e67  verriding during
-000043e0: 2072 756e 7469 6d65 3a0a 0a2e 2e20 636f   runtime:.... co
-000043f0: 6465 3a3a 2070 7974 686f 6e0a 0a20 2020  de:: python..   
-00004400: 203e 3e3e 2066 726f 6d20 7369 7820 696d   >>> from six im
-00004410: 706f 7274 2077 6974 685f 6d65 7461 636c  port with_metacl
-00004420: 6173 730a 2020 2020 3e3e 3e20 6672 6f6d  ass.    >>> from
-00004430: 2062 6173 6963 636f 2e72 756e 7469 6d65   basicco.runtime
-00004440: 5f66 696e 616c 2069 6d70 6f72 7420 5275  _final import Ru
-00004450: 6e74 696d 6546 696e 616c 4d65 7461 2c20  ntimeFinalMeta, 
-00004460: 6669 6e61 6c0a 2020 2020 3e3e 3e20 4066  final.    >>> @f
-00004470: 696e 616c 0a20 2020 202e 2e2e 2063 6c61  inal.    ... cla
-00004480: 7373 2041 7373 6574 2877 6974 685f 6d65  ss Asset(with_me
-00004490: 7461 636c 6173 7328 5275 6e74 696d 6546  taclass(RuntimeF
-000044a0: 696e 616c 4d65 7461 2c20 6f62 6a65 6374  inalMeta, object
-000044b0: 2929 3a0a 2020 2020 2e2e 2e20 2020 2020  )):.    ...     
-000044c0: 7061 7373 0a20 2020 202e 2e2e 0a20 2020  pass.    ....   
-000044d0: 203e 3e3e 2063 6c61 7373 2053 7562 4173   >>> class SubAs
-000044e0: 7365 7428 4173 7365 7429 3a0a 2020 2020  set(Asset):.    
-000044f0: 2e2e 2e20 2020 2020 7061 7373 0a20 2020  ...     pass.   
-00004500: 202e 2e2e 0a20 2020 2054 7261 6365 6261   ....    Traceba
-00004510: 636b 2028 6d6f 7374 2072 6563 656e 7420  ck (most recent 
-00004520: 6361 6c6c 206c 6173 7429 3a0a 2020 2020  call last):.    
-00004530: 5479 7065 4572 726f 723a 2063 616e 2774  TypeError: can't
-00004540: 2073 7562 636c 6173 7320 6669 6e61 6c20   subclass final 
-00004550: 636c 6173 7320 2741 7373 6574 270a 0a2e  class 'Asset'...
-00004560: 2e20 636f 6465 3a3a 2070 7974 686f 6e0a  . code:: python.
-00004570: 0a20 2020 203e 3e3e 2066 726f 6d20 7369  .    >>> from si
-00004580: 7820 696d 706f 7274 2077 6974 685f 6d65  x import with_me
-00004590: 7461 636c 6173 730a 2020 2020 3e3e 3e20  taclass.    >>> 
-000045a0: 6672 6f6d 2062 6173 6963 636f 2e72 756e  from basicco.run
-000045b0: 7469 6d65 5f66 696e 616c 2069 6d70 6f72  time_final impor
-000045c0: 7420 5275 6e74 696d 6546 696e 616c 4d65  t RuntimeFinalMe
-000045d0: 7461 2c20 6669 6e61 6c0a 2020 2020 3e3e  ta, final.    >>
-000045e0: 3e20 636c 6173 7320 4173 7365 7428 7769  > class Asset(wi
-000045f0: 7468 5f6d 6574 6163 6c61 7373 2852 756e  th_metaclass(Run
-00004600: 7469 6d65 4669 6e61 6c4d 6574 612c 206f  timeFinalMeta, o
-00004610: 626a 6563 7429 293a 0a20 2020 202e 2e2e  bject)):.    ...
-00004620: 2020 2020 2040 6669 6e61 6c0a 2020 2020       @final.    
-00004630: 2e2e 2e20 2020 2020 6465 6620 6d65 7468  ...     def meth
-00004640: 6f64 2873 656c 6629 3a0a 2020 2020 2e2e  od(self):.    ..
-00004650: 2e20 2020 2020 2020 2020 7061 7373 0a20  .         pass. 
-00004660: 2020 202e 2e2e 0a20 2020 203e 3e3e 2063     ....    >>> c
-00004670: 6c61 7373 2053 7562 4173 7365 7428 4173  lass SubAsset(As
-00004680: 7365 7429 3a0a 2020 2020 2e2e 2e20 2020  set):.    ...   
-00004690: 2020 6465 6620 6d65 7468 6f64 2873 656c    def method(sel
-000046a0: 6629 3a0a 2020 2020 2e2e 2e20 2020 2020  f):.    ...     
-000046b0: 2020 2020 7061 7373 0a20 2020 2054 7261      pass.    Tra
-000046c0: 6365 6261 636b 2028 6d6f 7374 2072 6563  ceback (most rec
-000046d0: 656e 7420 6361 6c6c 206c 6173 7429 3a0a  ent call last):.
-000046e0: 2020 2020 5479 7065 4572 726f 723a 2027      TypeError: '
-000046f0: 5375 6241 7373 6574 2720 6f76 6572 7269  SubAsset' overri
-00004700: 6465 7320 6669 6e61 6c20 6d65 6d62 6572  des final member
-00004710: 2027 6d65 7468 6f64 2720 6465 6669 6e65   'method' define
-00004720: 6420 6279 2027 4173 7365 7427 0a0a 2e2e  d by 'Asset'....
-00004730: 2063 6f64 653a 3a20 7079 7468 6f6e 0a0a   code:: python..
-00004740: 2020 2020 3e3e 3e20 6672 6f6d 2073 6978      >>> from six
-00004750: 2069 6d70 6f72 7420 7769 7468 5f6d 6574   import with_met
-00004760: 6163 6c61 7373 0a20 2020 203e 3e3e 2066  aclass.    >>> f
-00004770: 726f 6d20 6261 7369 6363 6f2e 7275 6e74  rom basicco.runt
-00004780: 696d 655f 6669 6e61 6c20 696d 706f 7274  ime_final import
-00004790: 2052 756e 7469 6d65 4669 6e61 6c4d 6574   RuntimeFinalMet
-000047a0: 612c 2066 696e 616c 0a20 2020 203e 3e3e  a, final.    >>>
-000047b0: 2063 6c61 7373 2041 7373 6574 2877 6974   class Asset(wit
-000047c0: 685f 6d65 7461 636c 6173 7328 5275 6e74  h_metaclass(Runt
-000047d0: 696d 6546 696e 616c 4d65 7461 2c20 6f62  imeFinalMeta, ob
-000047e0: 6a65 6374 2929 3a0a 2020 2020 2e2e 2e20  ject)):.    ... 
-000047f0: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
-00004800: 2020 2e2e 2e20 2020 2020 4066 696e 616c    ...     @final
-00004810: 0a20 2020 202e 2e2e 2020 2020 2064 6566  .    ...     def
-00004820: 2070 726f 7028 7365 6c66 293a 0a20 2020   prop(self):.   
-00004830: 202e 2e2e 2020 2020 2020 2020 2070 6173   ...         pas
-00004840: 730a 2020 2020 2e2e 2e0a 2020 2020 3e3e  s.    ....    >>
-00004850: 3e20 636c 6173 7320 5375 6241 7373 6574  > class SubAsset
-00004860: 2841 7373 6574 293a 0a20 2020 202e 2e2e  (Asset):.    ...
-00004870: 2020 2020 2040 7072 6f70 6572 7479 0a20       @property. 
-00004880: 2020 202e 2e2e 2020 2020 2064 6566 2070     ...     def p
-00004890: 726f 7028 7365 6c66 293a 0a20 2020 202e  rop(self):.    .
-000048a0: 2e2e 2020 2020 2020 2020 2070 6173 730a  ..         pass.
-000048b0: 2020 2020 5472 6163 6562 6163 6b20 286d      Traceback (m
-000048c0: 6f73 7420 7265 6365 6e74 2063 616c 6c20  ost recent call 
-000048d0: 6c61 7374 293a 0a20 2020 2054 7970 6545  last):.    TypeE
-000048e0: 7272 6f72 3a20 2753 7562 4173 7365 7427  rror: 'SubAsset'
-000048f0: 206f 7665 7272 6964 6573 2066 696e 616c   overrides final
-00004900: 206d 656d 6265 7220 2770 726f 7027 2064   member 'prop' d
-00004910: 6566 696e 6564 2062 7920 2741 7373 6574  efined by 'Asset
-00004920: 270a 0a73 6166 655f 6e6f 745f 6571 7561  '..safe_not_equa
-00004930: 6c73 0a5e 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e  ls.^^^^^^^^^^^^^
-00004940: 5e5e 0a42 6163 6b70 6f72 7420 6f66 2074  ^^.Backport of t
-00004950: 6865 2064 6566 6175 6c74 2050 7974 686f  he default Pytho
-00004960: 6e20 3320 6265 6861 7669 6f72 206f 6620  n 3 behavior of 
-00004970: 605f 5f6e 655f 5f60 2062 6568 6176 696f  `__ne__` behavio
-00004980: 7220 666f 7220 5079 7468 6f6e 2032 2e37  r for Python 2.7
-00004990: 2e0a 0a2e 2e20 636f 6465 3a3a 2070 7974  ..... code:: pyt
-000049a0: 686f 6e0a 0a20 2020 203e 3e3e 2066 726f  hon..    >>> fro
-000049b0: 6d20 7369 7820 696d 706f 7274 2077 6974  m six import wit
-000049c0: 685f 6d65 7461 636c 6173 730a 2020 2020  h_metaclass.    
-000049d0: 3e3e 3e20 6672 6f6d 2062 6173 6963 636f  >>> from basicco
-000049e0: 2e73 6166 655f 6e6f 745f 6571 7561 6c73  .safe_not_equals
-000049f0: 2069 6d70 6f72 7420 5361 6665 4e6f 7445   import SafeNotE
-00004a00: 7175 616c 734d 6574 610a 2020 2020 3e3e  qualsMeta.    >>
-00004a10: 3e20 636c 6173 7320 436c 6173 7328 7769  > class Class(wi
-00004a20: 7468 5f6d 6574 6163 6c61 7373 2853 6166  th_metaclass(Saf
-00004a30: 654e 6f74 4571 7561 6c73 4d65 7461 2c20  eNotEqualsMeta, 
-00004a40: 6f62 6a65 6374 2929 3a0a 2020 2020 2e2e  object)):.    ..
-00004a50: 2e20 2020 2020 7061 7373 0a20 2020 202e  .     pass.    .
-00004a60: 2e2e 0a20 2020 203e 3e3e 206f 626a 5f61  ...    >>> obj_a
-00004a70: 203d 2043 6c61 7373 2829 0a20 2020 203e   = Class().    >
-00004a80: 3e3e 206f 626a 5f62 203d 2043 6c61 7373  >> obj_b = Class
-00004a90: 2829 0a20 2020 203e 3e3e 2061 7373 6572  ().    >>> asser
-00004aa0: 7420 286f 626a 5f61 203d 3d20 6f62 6a5f  t (obj_a == obj_
-00004ab0: 6129 2069 7320 6e6f 7420 286f 626a 5f61  a) is not (obj_a
-00004ac0: 2021 3d20 6f62 6a5f 6129 0a20 2020 203e   != obj_a).    >
-00004ad0: 3e3e 2061 7373 6572 7420 286f 626a 5f62  >> assert (obj_b
-00004ae0: 203d 3d20 6f62 6a5f 6229 2069 7320 6e6f   == obj_b) is no
-00004af0: 7420 286f 626a 5f62 2021 3d20 6f62 6a5f  t (obj_b != obj_
-00004b00: 6229 0a20 2020 203e 3e3e 2061 7373 6572  b).    >>> asser
-00004b10: 7420 286f 626a 5f61 203d 3d20 6f62 6a5f  t (obj_a == obj_
-00004b20: 6229 2069 7320 6e6f 7420 286f 626a 5f61  b) is not (obj_a
-00004b30: 2021 3d20 6f62 6a5f 6229 0a0a 7361 6665   != obj_b)..safe
-00004b40: 5f72 6570 720a 5e5e 5e5e 5e5e 5e5e 5e0a  _repr.^^^^^^^^^.
-00004b50: 4465 636f 7261 746f 7220 7468 6174 2070  Decorator that p
-00004b60: 7265 7665 6e74 7320 605f 5f72 6570 725f  revents `__repr_
-00004b70: 5f60 206d 6574 686f 6473 2066 726f 6d20  _` methods from 
-00004b80: 7261 6973 696e 6720 6578 6365 7074 696f  raising exceptio
-00004b90: 6e73 2061 6e64 2072 6574 7572 6e20 6120  ns and return a 
-00004ba0: 6465 6661 756c 7420 7265 7072 6573 656e  default represen
-00004bb0: 7461 7469 6f6e 2069 6e73 7465 6164 2e0a  tation instead..
-00004bc0: 0a2e 2e20 636f 6465 3a3a 2070 7974 686f  ... code:: pytho
-00004bd0: 6e0a 0a20 2020 203e 3e3e 2066 726f 6d20  n..    >>> from 
-00004be0: 6261 7369 6363 6f2e 7361 6665 5f72 6570  basicco.safe_rep
-00004bf0: 7220 696d 706f 7274 2073 6166 655f 7265  r import safe_re
-00004c00: 7072 0a20 2020 203e 3e3e 2063 6c61 7373  pr.    >>> class
-00004c10: 2043 6c61 7373 286f 626a 6563 7429 3a0a   Class(object):.
-00004c20: 2020 2020 2e2e 2e20 2020 2020 4073 6166      ...     @saf
-00004c30: 655f 7265 7072 0a20 2020 202e 2e2e 2020  e_repr.    ...  
-00004c40: 2020 2064 6566 205f 5f72 6570 725f 5f28     def __repr__(
-00004c50: 7365 6c66 293a 0a20 2020 202e 2e2e 2020  self):.    ...  
-00004c60: 2020 2020 2020 2072 6169 7365 2052 756e         raise Run
-00004c70: 7469 6d65 4572 726f 7228 226f 6820 6f68  timeError("oh oh
-00004c80: 2229 0a20 2020 202e 2e2e 0a20 2020 203e  ").    ....    >
-00004c90: 3e3e 206f 626a 203d 2043 6c61 7373 2829  >> obj = Class()
-00004ca0: 0a20 2020 203e 3e3e 2072 6570 7228 6f62  .    >>> repr(ob
-00004cb0: 6a29 0a20 2020 2022 3c5f 5f6d 6169 6e5f  j).    "<__main_
-00004cc0: 5f2e 436c 6173 7320 6f62 6a65 6374 2061  _.Class object a
-00004cd0: 7420 2e2e 2e3b 2072 6570 7220 6661 696c  t ...; repr fail
-00004ce0: 6564 2064 7565 2074 6f20 2752 756e 7469  ed due to 'Runti
-00004cf0: 6d65 4572 726f 723a 206f 6820 6f68 273e  meError: oh oh'>
-00004d00: 220a 0a73 6574 5f6e 616d 650a 5e5e 5e5e  "..set_name.^^^^
-00004d10: 5e5e 5e5e 0a42 6163 6b70 6f72 7420 6f66  ^^^^.Backport of
-00004d20: 2074 6865 2066 756e 6374 696f 6e61 6c69   the functionali
-00004d30: 7479 206f 6620 605f 5f73 6574 5f6e 616d  ty of `__set_nam
-00004d40: 655f 5f60 2066 726f 6d20 5045 5020 3438  e__` from PEP 48
-00004d50: 3720 746f 2050 7974 686f 6e20 322e 372e  7 to Python 2.7.
-00004d60: 0a0a 2e2e 2063 6f64 653a 3a20 7079 7468  .... code:: pyth
-00004d70: 6f6e 0a0a 2020 2020 3e3e 3e20 6672 6f6d  on..    >>> from
-00004d80: 2062 6173 6963 636f 2e73 6574 5f6e 616d   basicco.set_nam
-00004d90: 6520 696d 706f 7274 2053 6574 4e61 6d65  e import SetName
-00004da0: 0a20 2020 203e 3e3e 2063 6c61 7373 2041  .    >>> class A
-00004db0: 7474 7269 6275 7465 286f 626a 6563 7429  ttribute(object)
-00004dc0: 3a0a 2020 2020 2e2e 2e20 2020 2020 6465  :.    ...     de
-00004dd0: 6620 5f5f 7365 745f 6e61 6d65 5f5f 2873  f __set_name__(s
-00004de0: 656c 662c 206f 776e 6572 2c20 6e61 6d65  elf, owner, name
-00004df0: 293a 0a20 2020 202e 2e2e 2020 2020 2020  ):.    ...      
-00004e00: 2020 2073 656c 662e 6f77 6e65 7220 3d20     self.owner = 
-00004e10: 6f77 6e65 720a 2020 2020 2e2e 2e20 2020  owner.    ...   
-00004e20: 2020 2020 2020 7365 6c66 2e6e 616d 6520        self.name 
-00004e30: 3d20 6e61 6d65 0a20 2020 202e 2e2e 0a20  = name.    .... 
-00004e40: 2020 203e 3e3e 2063 6c61 7373 2043 6f6c     >>> class Col
-00004e50: 6c65 6374 696f 6e28 5365 744e 616d 6529  lection(SetName)
-00004e60: 3a0a 2020 2020 2e2e 2e20 2020 2020 666f  :.    ...     fo
-00004e70: 6f20 3d20 4174 7472 6962 7574 6528 290a  o = Attribute().
-00004e80: 2020 2020 2e2e 2e0a 2020 2020 3e3e 3e20      ....    >>> 
-00004e90: 436f 6c6c 6563 7469 6f6e 2e66 6f6f 2e6f  Collection.foo.o
-00004ea0: 776e 6572 2069 7320 436f 6c6c 6563 7469  wner is Collecti
-00004eb0: 6f6e 0a20 2020 2054 7275 650a 2020 2020  on.    True.    
-00004ec0: 3e3e 3e20 436f 6c6c 6563 7469 6f6e 2e66  >>> Collection.f
-00004ed0: 6f6f 2e6e 616d 650a 2020 2020 2766 6f6f  oo.name.    'foo
-00004ee0: 270a 0a74 7970 655f 6368 6563 6b69 6e67  '..type_checking
-00004ef0: 0a5e 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e 0a52  .^^^^^^^^^^^^^.R
-00004f00: 756e 7469 6d65 2074 7970 6520 6368 6563  untime type chec
-00004f10: 6b69 6e67 2077 6974 6820 7375 7070 6f72  king with suppor
-00004f20: 7420 666f 7220 696d 706f 7274 2070 6174  t for import pat
-00004f30: 6873 2061 6e64 2074 7970 6520 6869 6e74  hs and type hint
-00004f40: 732e 0a0a 2e2e 2063 6f64 653a 3a20 7079  s..... code:: py
-00004f50: 7468 6f6e 0a0a 2020 2020 3e3e 3e20 6672  thon..    >>> fr
-00004f60: 6f6d 2074 6970 706f 2069 6d70 6f72 7420  om tippo import 
-00004f70: 4d61 7070 696e 670a 2020 2020 3e3e 3e20  Mapping.    >>> 
-00004f80: 6672 6f6d 2069 7465 7274 6f6f 6c73 2069  from itertools i
-00004f90: 6d70 6f72 7420 6368 6169 6e0a 2020 2020  mport chain.    
-00004fa0: 3e3e 3e20 6672 6f6d 2062 6173 6963 636f  >>> from basicco
-00004fb0: 2e74 7970 655f 6368 6563 6b69 6e67 2069  .type_checking i
-00004fc0: 6d70 6f72 7420 6973 5f69 6e73 7461 6e63  mport is_instanc
-00004fd0: 650a 2020 2020 3e3e 3e20 636c 6173 7320  e.    >>> class 
-00004fe0: 5375 6243 6861 696e 2863 6861 696e 293a  SubChain(chain):
-00004ff0: 0a20 2020 202e 2e2e 2020 2020 2070 6173  .    ...     pas
-00005000: 730a 2020 2020 2e2e 2e0a 2020 2020 3e3e  s.    ....    >>
-00005010: 3e20 6973 5f69 6e73 7461 6e63 6528 332c  > is_instance(3,
-00005020: 2069 6e74 290a 2020 2020 5472 7565 0a20   int).    True. 
-00005030: 2020 203e 3e3e 2069 735f 696e 7374 616e     >>> is_instan
-00005040: 6365 2833 2c20 2863 6861 696e 2c20 696e  ce(3, (chain, in
-00005050: 7429 290a 2020 2020 5472 7565 0a20 2020  t)).    True.   
-00005060: 203e 3e3e 2069 735f 696e 7374 616e 6365   >>> is_instance
-00005070: 2833 2c20 2829 290a 2020 2020 4661 6c73  (3, ()).    Fals
-00005080: 650a 2020 2020 3e3e 3e20 6973 5f69 6e73  e.    >>> is_ins
-00005090: 7461 6e63 6528 5375 6243 6861 696e 2829  tance(SubChain()
-000050a0: 2c20 2269 7465 7274 6f6f 6c73 2e63 6861  , "itertools.cha
-000050b0: 696e 2229 0a20 2020 2054 7275 650a 2020  in").    True.  
-000050c0: 2020 3e3e 3e20 6973 5f69 6e73 7461 6e63    >>> is_instanc
-000050d0: 6528 6368 6169 6e28 292c 2022 6974 6572  e(chain(), "iter
-000050e0: 746f 6f6c 732e 6368 6169 6e22 2c20 7375  tools.chain", su
-000050f0: 6274 7970 6573 3d46 616c 7365 290a 2020  btypes=False).  
-00005100: 2020 5472 7565 0a20 2020 203e 3e3e 2069    True.    >>> i
-00005110: 735f 696e 7374 616e 6365 2853 7562 4368  s_instance(SubCh
-00005120: 6169 6e28 292c 2022 6974 6572 746f 6f6c  ain(), "itertool
-00005130: 732e 6368 6169 6e22 2c20 7375 6274 7970  s.chain", subtyp
-00005140: 6573 3d46 616c 7365 290a 2020 2020 4661  es=False).    Fa
-00005150: 6c73 650a 2020 2020 3e3e 3e20 6973 5f69  lse.    >>> is_i
-00005160: 6e73 7461 6e63 6528 7b22 6122 3a20 312c  nstance({"a": 1,
-00005170: 2022 6222 3a20 327d 2c20 4d61 7070 696e   "b": 2}, Mappin
-00005180: 675b 7374 722c 2069 6e74 5d29 0a20 2020  g[str, int]).   
-00005190: 2054 7275 650a 0a75 6e69 7175 655f 6974   True..unique_it
-000051a0: 6572 6174 6f72 0a5e 5e5e 5e5e 5e5e 5e5e  erator.^^^^^^^^^
-000051b0: 5e5e 5e5e 5e5e 0a49 7465 7261 746f 7220  ^^^^^^.Iterator 
-000051c0: 7468 6174 2079 6965 6c64 7320 756e 6971  that yields uniq
-000051d0: 7565 2076 616c 7565 732e 0a0a 2e2e 2063  ue values..... c
-000051e0: 6f64 653a 3a20 7079 7468 6f6e 0a0a 2020  ode:: python..  
-000051f0: 2020 3e3e 3e20 6672 6f6d 2062 6173 6963    >>> from basic
-00005200: 636f 2e75 6e69 7175 655f 6974 6572 6174  co.unique_iterat
-00005210: 6f72 2069 6d70 6f72 7420 756e 6971 7565  or import unique
-00005220: 5f69 7465 7261 746f 720a 2020 2020 3e3e  _iterator.    >>
-00005230: 3e20 6c69 7374 2875 6e69 7175 655f 6974  > list(unique_it
-00005240: 6572 6174 6f72 285b 312c 2032 2c20 332c  erator([1, 2, 3,
-00005250: 2033 2c20 342c 2034 2c20 355d 2929 0a20   3, 4, 4, 5])). 
-00005260: 2020 205b 312c 2032 2c20 332c 2034 2c20     [1, 2, 3, 4, 
-00005270: 355d 0a0a 7765 616b 5f72 6566 6572 656e  5]..weak_referen
-00005280: 6365 0a5e 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e  ce.^^^^^^^^^^^^^
-00005290: 5e0a 5765 616b 2052 6566 6572 656e 6365  ^.Weak Reference
-000052a0: 2d6c 696b 6520 6f62 6a65 6374 2074 6861  -like object tha
-000052b0: 7420 7375 7070 6f72 7473 2070 6963 6b6c  t supports pickl
-000052c0: 696e 672e 0a                             ing..
+00002dc0: 6672 6f6d 2073 6978 2069 6d70 6f72 7420  from six import 
+00002dd0: 7769 7468 5f6d 6574 6163 6c61 7373 0a20  with_metaclass. 
+00002de0: 2020 203e 3e3e 2066 726f 6d20 6261 7369     >>> from basi
+00002df0: 6363 6f2e 696d 706c 6963 6974 5f68 6173  cco.implicit_has
+00002e00: 6820 696d 706f 7274 2049 6d70 6c69 6369  h import Implici
+00002e10: 7448 6173 684d 6574 610a 2020 2020 3e3e  tHashMeta.    >>
+00002e20: 3e20 636c 6173 7320 4173 7365 7428 7769  > class Asset(wi
+00002e30: 7468 5f6d 6574 6163 6c61 7373 2849 6d70  th_metaclass(Imp
+00002e40: 6c69 6369 7448 6173 684d 6574 612c 206f  licitHashMeta, o
+00002e50: 626a 6563 7429 293a 0a20 2020 202e 2e2e  bject)):.    ...
+00002e60: 2020 2020 2064 6566 205f 5f65 715f 5f28       def __eq__(
+00002e70: 7365 6c66 2c20 6f74 6865 7229 3a0a 2020  self, other):.  
+00002e80: 2020 2e2e 2e20 2020 2020 2020 2020 7061    ...         pa
+00002e90: 7373 0a20 2020 202e 2e2e 0a20 2020 203e  ss.    ....    >
+00002ea0: 3e3e 2041 7373 6574 2e5f 5f68 6173 685f  >> Asset.__hash_
+00002eb0: 5f20 6973 204e 6f6e 650a 2020 2020 5472  _ is None.    Tr
+00002ec0: 7565 0a0a 696d 706f 7274 5f70 6174 680a  ue..import_path.
+00002ed0: 5e5e 5e5e 5e5e 5e5e 5e5e 5e0a 4765 6e65  ^^^^^^^^^^^.Gene
+00002ee0: 7261 7465 2069 6d70 6f72 7461 626c 6520  rate importable 
+00002ef0: 646f 7420 7061 7468 7320 616e 6420 696d  dot paths and im
+00002f00: 706f 7274 2066 726f 6d20 7468 656d 2e0a  port from them..
+00002f10: 0a2e 2e20 636f 6465 3a3a 2070 7974 686f  ... code:: pytho
+00002f20: 6e0a 0a20 2020 203e 3e3e 2069 6d70 6f72  n..    >>> impor
+00002f30: 7420 6974 6572 746f 6f6c 730a 2020 2020  t itertools.    
+00002f40: 3e3e 3e20 6672 6f6d 2062 6173 6963 636f  >>> from basicco
+00002f50: 2e69 6d70 6f72 745f 7061 7468 2069 6d70  .import_path imp
+00002f60: 6f72 7420 6765 745f 7061 7468 2c20 696d  ort get_path, im
+00002f70: 706f 7274 5f70 6174 680a 2020 2020 3e3e  port_path.    >>
+00002f80: 3e20 6765 745f 7061 7468 2869 7465 7274  > get_path(itert
+00002f90: 6f6f 6c73 2e63 6861 696e 290a 2020 2020  ools.chain).    
+00002fa0: 2769 7465 7274 6f6f 6c73 2e63 6861 696e  'itertools.chain
+00002fb0: 270a 2020 2020 3e3e 3e20 696d 706f 7274  '.    >>> import
+00002fc0: 5f70 6174 6828 2269 7465 7274 6f6f 6c73  _path("itertools
+00002fd0: 2e63 6861 696e 2229 0a20 2020 203c 2e2e  .chain").    <..
+00002fe0: 2e20 2769 7465 7274 6f6f 6c73 2e63 6861  . 'itertools.cha
+00002ff0: 696e 273e 0a0a 2e2e 2063 6f64 653a 3a20  in'>.... code:: 
+00003000: 7079 7468 6f6e 0a0a 2020 2020 3e3e 3e20  python..    >>> 
+00003010: 6672 6f6d 2062 6173 6963 636f 2e69 6d70  from basicco.imp
+00003020: 6f72 745f 7061 7468 2069 6d70 6f72 7420  ort_path import 
+00003030: 6578 7472 6163 745f 6765 6e65 7269 635f  extract_generic_
+00003040: 7061 7468 730a 2020 2020 3e3e 3e20 6578  paths.    >>> ex
+00003050: 7472 6163 745f 6765 6e65 7269 635f 7061  tract_generic_pa
+00003060: 7468 7328 2254 7570 6c65 5b69 6e74 2c20  ths("Tuple[int, 
+00003070: 7374 725d 2229 0a20 2020 2028 2754 7570  str]").    ('Tup
+00003080: 6c65 272c 2028 2769 6e74 272c 2027 7374  le', ('int', 'st
+00003090: 7227 2929 0a0a 696e 6974 5f73 7562 636c  r'))..init_subcl
+000030a0: 6173 730a 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e  ass.^^^^^^^^^^^^
+000030b0: 5e0a 4261 636b 706f 7274 206f 6620 7468  ^.Backport of th
+000030c0: 6520 6675 6e63 7469 6f6e 616c 6974 7920  e functionality 
+000030d0: 6f66 2060 5f5f 696e 6974 5f73 7562 636c  of `__init_subcl
+000030e0: 6173 735f 5f60 2066 726f 6d20 5045 5020  ass__` from PEP 
+000030f0: 3438 3720 746f 2050 7974 686f 6e20 322e  487 to Python 2.
+00003100: 372e 0a54 6869 7320 776f 726b 7320 666f  7..This works fo
+00003110: 7220 626f 7468 2050 7974 686f 6e20 3220  r both Python 2 
+00003120: 2875 7369 6e67 2060 5f5f 6b77 6172 6773  (using `__kwargs
+00003130: 5f5f 6029 2061 6e64 2033 2028 7573 696e  __`) and 3 (usin
+00003140: 6720 7468 6520 6e65 7720 636c 6173 7320  g the new class 
+00003150: 7061 7261 6d65 7465 7273 292e 0a0a 2e2e  parameters).....
+00003160: 2063 6f64 653a 3a20 7079 7468 6f6e 0a0a   code:: python..
+00003170: 2020 2020 3e3e 3e20 6672 6f6d 2062 6173      >>> from bas
+00003180: 6963 636f 2e69 6e69 745f 7375 6263 6c61  icco.init_subcla
+00003190: 7373 2069 6d70 6f72 7420 496e 6974 5375  ss import InitSu
+000031a0: 6263 6c61 7373 0a20 2020 203e 3e3e 2063  bclass.    >>> c
+000031b0: 6c61 7373 2046 6f6f 2849 6e69 7453 7562  lass Foo(InitSub
+000031c0: 636c 6173 7329 3a0a 2020 2020 2e2e 2e20  class):.    ... 
+000031d0: 2020 2020 6465 6620 5f5f 696e 6974 5f73      def __init_s
+000031e0: 7562 636c 6173 735f 5f28 636c 732c 2066  ubclass__(cls, f
+000031f0: 6f6f 3d4e 6f6e 652c 202a 2a6b 7761 7267  oo=None, **kwarg
+00003200: 7329 3a0a 2020 2020 2e2e 2e20 2020 2020  s):.    ...     
+00003210: 2020 2020 636c 732e 666f 6f20 3d20 666f      cls.foo = fo
+00003220: 6f0a 2020 2020 2e2e 2e0a 2020 2020 3e3e  o.    ....    >>
+00003230: 3e20 636c 6173 7320 4261 7228 466f 6f29  > class Bar(Foo)
+00003240: 3a0a 2020 2020 2e2e 2e20 2020 2020 5f5f  :.    ...     __
+00003250: 6b77 6172 6773 5f5f 203d 207b 2266 6f6f  kwargs__ = {"foo
+00003260: 223a 2022 6261 7222 7d20 2023 2079 6f75  ": "bar"}  # you
+00003270: 2063 616e 2073 7065 6369 6679 2063 6c73   can specify cls
+00003280: 206b 7761 7267 7320 6f6e 2070 7932 206c   kwargs on py2 l
+00003290: 696b 6520 7468 6973 0a20 2020 202e 2e2e  ike this.    ...
+000032a0: 0a20 2020 203e 3e3e 2042 6172 2e66 6f6f  .    >>> Bar.foo
+000032b0: 0a20 2020 2027 6261 7227 0a0a 6c6f 636b  .    'bar'..lock
+000032c0: 6564 5f63 6c61 7373 0a5e 5e5e 5e5e 5e5e  ed_class.^^^^^^^
+000032d0: 5e5e 5e5e 5e0a 5072 6576 656e 7473 2063  ^^^^^.Prevents c
+000032e0: 6861 6e67 696e 6720 7075 626c 6963 2063  hanging public c
+000032f0: 6c61 7373 2061 7474 7269 6275 7465 732e  lass attributes.
+00003300: 0a0a 2e2e 2063 6f64 653a 3a20 7079 7468  .... code:: pyth
+00003310: 6f6e 0a0a 2020 2020 3e3e 3e20 6672 6f6d  on..    >>> from
+00003320: 2073 6978 2069 6d70 6f72 7420 7769 7468   six import with
+00003330: 5f6d 6574 6163 6c61 7373 0a20 2020 203e  _metaclass.    >
+00003340: 3e3e 2066 726f 6d20 6261 7369 6363 6f2e  >> from basicco.
+00003350: 6c6f 636b 6564 5f63 6c61 7373 2069 6d70  locked_class imp
+00003360: 6f72 7420 4c6f 636b 6564 436c 6173 734d  ort LockedClassM
+00003370: 6574 610a 2020 2020 3e3e 3e20 636c 6173  eta.    >>> clas
+00003380: 7320 466f 6f28 7769 7468 5f6d 6574 6163  s Foo(with_metac
+00003390: 6c61 7373 284c 6f63 6b65 6443 6c61 7373  lass(LockedClass
+000033a0: 4d65 7461 2c20 6f62 6a65 6374 2929 3a0a  Meta, object)):.
+000033b0: 2020 2020 2e2e 2e20 2020 2020 6261 7220      ...     bar 
+000033c0: 3d20 2266 6f6f 220a 2020 2020 2e2e 2e0a  = "foo".    ....
+000033d0: 2020 2020 3e3e 3e20 466f 6f2e 6261 7220      >>> Foo.bar 
+000033e0: 3d20 2262 6172 220a 2020 2020 5472 6163  = "bar".    Trac
+000033f0: 6562 6163 6b20 286d 6f73 7420 7265 6365  eback (most rece
+00003400: 6e74 2063 616c 6c20 6c61 7374 293a 0a20  nt call last):. 
+00003410: 2020 2041 7474 7269 6275 7465 4572 726f     AttributeErro
+00003420: 723a 2063 616e 2774 2073 6574 2072 6561  r: can't set rea
+00003430: 642d 6f6e 6c79 2063 6c61 7373 2061 7474  d-only class att
+00003440: 7269 6275 7465 2027 6261 7227 0a0a 6d61  ribute 'bar'..ma
+00003450: 6e67 6c69 6e67 0a5e 5e5e 5e5e 5e5e 5e0a  ngling.^^^^^^^^.
+00003460: 4675 6e63 7469 6f6e 7320 746f 206d 616e  Functions to man
+00003470: 676c 652f 756e 6d61 6e67 6c65 2f65 7874  gle/unmangle/ext
+00003480: 7261 6374 2070 7269 7661 7465 206e 616d  ract private nam
+00003490: 6573 2e0a 0a2e 2e20 636f 6465 3a3a 2070  es..... code:: p
+000034a0: 7974 686f 6e0a 0a20 2020 203e 3e3e 2066  ython..    >>> f
+000034b0: 726f 6d20 6261 7369 6363 6f2e 6d61 6e67  rom basicco.mang
+000034c0: 6c69 6e67 2069 6d70 6f72 7420 6d61 6e67  ling import mang
+000034d0: 6c65 2c20 756e 6d61 6e67 6c65 2c20 6578  le, unmangle, ex
+000034e0: 7472 6163 740a 2020 2020 3e3e 3e20 6d61  tract.    >>> ma
+000034f0: 6e67 6c65 2822 5f5f 6d65 6d62 6572 222c  ngle("__member",
+00003500: 2022 466f 6f22 290a 2020 2020 275f 466f   "Foo").    '_Fo
+00003510: 6f5f 5f6d 656d 6265 7227 0a20 2020 203e  o__member'.    >
+00003520: 3e3e 2075 6e6d 616e 676c 6528 225f 466f  >> unmangle("_Fo
+00003530: 6f5f 5f6d 656d 6265 7222 2c20 2246 6f6f  o__member", "Foo
+00003540: 2229 0a20 2020 2027 5f5f 6d65 6d62 6572  ").    '__member
+00003550: 270a 2020 2020 3e3e 3e20 6578 7472 6163  '.    >>> extrac
+00003560: 7428 225f 466f 6f5f 5f6d 656d 6265 7222  t("_Foo__member"
+00003570: 290a 2020 2020 2827 5f5f 6d65 6d62 6572  ).    ('__member
+00003580: 272c 2027 466f 6f27 290a 0a6d 6170 7069  ', 'Foo')..mappi
+00003590: 6e67 5f70 726f 7879 0a5e 5e5e 5e5e 5e5e  ng_proxy.^^^^^^^
+000035a0: 5e5e 5e5e 5e5e 0a4d 6170 7069 6e67 2050  ^^^^^^.Mapping P
+000035b0: 726f 7879 2074 7970 6520 2872 6561 642d  roxy type (read-
+000035c0: 6f6e 6c79 2064 6963 7469 6f6e 6172 7929  only dictionary)
+000035d0: 2066 6f72 206f 6c64 6572 2050 7974 686f   for older Pytho
+000035e0: 6e20 7665 7273 696f 6e73 2e0a 0a2e 2e20  n versions..... 
+000035f0: 636f 6465 3a3a 2070 7974 686f 6e0a 0a20  code:: python.. 
+00003600: 2020 203e 3e3e 2066 726f 6d20 6261 7369     >>> from basi
+00003610: 6363 6f2e 6d61 7070 696e 675f 7072 6f78  cco.mapping_prox
+00003620: 7920 696d 706f 7274 204d 6170 7069 6e67  y import Mapping
+00003630: 5072 6f78 7954 7970 650a 2020 2020 3e3e  ProxyType.    >>
+00003640: 3e20 696e 7465 726e 616c 5f64 6963 7420  > internal_dict 
+00003650: 3d20 7b22 666f 6f22 3a20 2262 6172 227d  = {"foo": "bar"}
+00003660: 0a20 2020 203e 3e3e 2070 726f 7879 5f64  .    >>> proxy_d
+00003670: 6963 7420 3d20 4d61 7070 696e 6750 726f  ict = MappingPro
+00003680: 7879 5479 7065 2869 6e74 6572 6e61 6c5f  xyType(internal_
+00003690: 6469 6374 290a 2020 2020 3e3e 3e20 7072  dict).    >>> pr
+000036a0: 6f78 795f 6469 6374 5b22 666f 6f22 5d0a  oxy_dict["foo"].
+000036b0: 2020 2020 2762 6172 270a 0a6e 616d 6564      'bar'..named
+000036c0: 5f74 7570 6c65 0a5e 5e5e 5e5e 5e5e 5e5e  _tuple.^^^^^^^^^
+000036d0: 5e5e 0a4e 616d 6564 2054 7570 6c65 2075  ^^.Named Tuple u
+000036e0: 7469 6c69 7469 6573 2e0a 0a45 7861 6d70  tilities...Examp
+000036f0: 6c65 206f 6620 6064 6566 6175 6c74 7360  le of `defaults`
+00003700: 2064 6563 6f72 6174 6f72 2f66 756e 6374   decorator/funct
+00003710: 696f 6e20 746f 2073 6574 2061 204e 616d  ion to set a Nam
+00003720: 6564 2054 7570 6c65 2773 2064 6566 6175  ed Tuple's defau
+00003730: 6c74 2076 616c 7565 733a 0a0a 2e2e 2063  lt values:.... c
+00003740: 6f64 653a 3a20 7079 7468 6f6e 0a0a 2020  ode:: python..  
+00003750: 2020 3e3e 3e20 6672 6f6d 2063 6f6c 6c65    >>> from colle
+00003760: 6374 696f 6e73 2069 6d70 6f72 7420 6e61  ctions import na
+00003770: 6d65 6474 7570 6c65 0a20 2020 203e 3e3e  medtuple.    >>>
+00003780: 2066 726f 6d20 6261 7369 6363 6f2e 6e61   from basicco.na
+00003790: 6d65 645f 7475 706c 6520 696d 706f 7274  med_tuple import
+000037a0: 2064 6566 6175 6c74 730a 2020 2020 3e3e   defaults.    >>
+000037b0: 3e20 506f 696e 7420 3d20 6465 6661 756c  > Point = defaul
+000037c0: 7473 286e 616d 653d 2266 6f6f 2229 286e  ts(name="foo")(n
+000037d0: 616d 6564 7475 706c 6528 2250 6f69 6e74  amedtuple("Point
+000037e0: 222c 2028 2278 222c 2022 7922 2c20 226e  ", ("x", "y", "n
+000037f0: 616d 6522 2929 290a 2020 2020 3e3e 3e20  ame"))).    >>> 
+00003800: 506f 696e 7428 312c 2032 290a 2020 2020  Point(1, 2).    
+00003810: 506f 696e 7428 783d 312c 2079 3d32 2c20  Point(x=1, y=2, 
+00003820: 6e61 6d65 3d27 666f 6f27 290a 0a6e 616d  name='foo')..nam
+00003830: 6573 7061 6365 0a5e 5e5e 5e5e 5e5e 5e5e  espace.^^^^^^^^^
+00003840: 0a57 7261 7073 2061 2064 6963 7469 6f6e  .Wraps a diction
+00003850: 6172 792f 6d61 7070 696e 6720 616e 6420  ary/mapping and 
+00003860: 7072 6f76 6964 6573 2061 7474 7269 6275  provides attribu
+00003870: 7465 2d73 7479 6c65 2061 6363 6573 7320  te-style access 
+00003880: 746f 2069 742e 0a0a 2e2e 2063 6f64 653a  to it..... code:
+00003890: 3a20 7079 7468 6f6e 0a0a 2020 2020 3e3e  : python..    >>
+000038a0: 3e20 6672 6f6d 2062 6173 6963 636f 2e6e  > from basicco.n
+000038b0: 616d 6573 7061 6365 2069 6d70 6f72 7420  amespace import 
+000038c0: 4e61 6d65 7370 6163 650a 2020 2020 3e3e  Namespace.    >>
+000038d0: 3e20 6e73 203d 204e 616d 6573 7061 6365  > ns = Namespace
+000038e0: 287b 2262 6172 223a 2022 666f 6f22 7d29  ({"bar": "foo"})
+000038f0: 0a20 2020 203e 3e3e 206e 732e 6261 720a  .    >>> ns.bar.
+00003900: 2020 2020 2766 6f6f 270a 0a2e 2e20 636f      'foo'.... co
+00003910: 6465 3a3a 2070 7974 686f 6e0a 0a20 2020  de:: python..   
+00003920: 203e 3e3e 2066 726f 6d20 6261 7369 6363   >>> from basicc
+00003930: 6f2e 6e61 6d65 7370 6163 6520 696d 706f  o.namespace impo
+00003940: 7274 204d 7574 6162 6c65 4e61 6d65 7370  rt MutableNamesp
+00003950: 6163 650a 2020 2020 3e3e 3e20 6e73 203d  ace.    >>> ns =
+00003960: 204d 7574 6162 6c65 4e61 6d65 7370 6163   MutableNamespac
+00003970: 6528 7b22 6261 7222 3a20 2266 6f6f 227d  e({"bar": "foo"}
+00003980: 290a 2020 2020 3e3e 3e20 6e73 2e66 6f6f  ).    >>> ns.foo
+00003990: 203d 2022 6261 7222 0a20 2020 203e 3e3e   = "bar".    >>>
+000039a0: 206e 732e 666f 6f0a 2020 2020 2762 6172   ns.foo.    'bar
+000039b0: 270a 2020 2020 3e3e 3e20 6e73 2e62 6172  '.    >>> ns.bar
+000039c0: 0a20 2020 2027 666f 6f27 0a0a 416c 736f  .    'foo'..Also
+000039d0: 2070 726f 7669 6465 7320 6120 604e 616d   provides a `Nam
+000039e0: 6573 7061 6365 644d 6574 6160 206d 6574  espacedMeta` met
+000039f0: 6163 6c61 7373 2074 6861 7420 6164 6473  aclass that adds
+00003a00: 2061 2060 5f5f 6e61 6d65 7370 6163 6560   a `__namespace`
+00003a10: 2070 726f 7465 6374 6564 2063 6c61 7373   protected class
+00003a20: 2061 7474 7269 6275 7465 2074 6861 7420   attribute that 
+00003a30: 6973 2075 6e69 7175 6520 746f 2065 6163  is unique to eac
+00003a40: 680a 636c 6173 732e 0a0a 2e2e 2063 6f64  h.class..... cod
+00003a50: 653a 3a20 7079 7468 6f6e 0a0a 2020 2020  e:: python..    
+00003a60: 3e3e 3e20 6672 6f6d 2073 6978 2069 6d70  >>> from six imp
+00003a70: 6f72 7420 7769 7468 5f6d 6574 6163 6c61  ort with_metacla
+00003a80: 7373 0a20 2020 203e 3e3e 2066 726f 6d20  ss.    >>> from 
+00003a90: 6261 7369 6363 6f2e 6e61 6d65 7370 6163  basicco.namespac
+00003aa0: 6520 696d 706f 7274 204e 616d 6573 7061  e import Namespa
+00003ab0: 6365 644d 6574 610a 2020 2020 3e3e 3e20  cedMeta.    >>> 
+00003ac0: 636c 6173 7320 4173 7365 7428 7769 7468  class Asset(with
+00003ad0: 5f6d 6574 6163 6c61 7373 284e 616d 6573  _metaclass(Names
+00003ae0: 7061 6365 644d 6574 612c 206f 626a 6563  pacedMeta, objec
+00003af0: 7429 293a 0a20 2020 202e 2e2e 2020 2020  t)):.    ...    
+00003b00: 2040 636c 6173 736d 6574 686f 640a 2020   @classmethod.  
+00003b10: 2020 2e2e 2e20 2020 2020 6465 6620 7365    ...     def se
+00003b20: 745f 636c 6173 735f 7661 6c75 6528 636c  t_class_value(cl
+00003b30: 732c 2076 616c 7565 293a 0a20 2020 202e  s, value):.    .
+00003b40: 2e2e 2020 2020 2020 2020 2063 6c73 2e5f  ..         cls._
+00003b50: 5f6e 616d 6573 7061 6365 2e76 616c 7565  _namespace.value
+00003b60: 203d 2076 616c 7565 0a20 2020 202e 2e2e   = value.    ...
+00003b70: 0a20 2020 202e 2e2e 2020 2020 2040 636c  .    ...     @cl
+00003b80: 6173 736d 6574 686f 640a 2020 2020 2e2e  assmethod.    ..
+00003b90: 2e20 2020 2020 6465 6620 6765 745f 636c  .     def get_cl
+00003ba0: 6173 735f 7661 6c75 6528 636c 7329 3a0a  ass_value(cls):.
+00003bb0: 2020 2020 2e2e 2e20 2020 2020 2020 2020      ...         
+00003bc0: 7265 7475 726e 2063 6c73 2e5f 5f6e 616d  return cls.__nam
+00003bd0: 6573 7061 6365 2e76 616c 7565 0a20 2020  espace.value.   
+00003be0: 202e 2e2e 0a20 2020 203e 3e3e 2041 7373   ....    >>> Ass
+00003bf0: 6574 2e73 6574 5f63 6c61 7373 5f76 616c  et.set_class_val
+00003c00: 7565 2822 666f 6f62 6172 2229 0a20 2020  ue("foobar").   
+00003c10: 203e 3e3e 2041 7373 6574 2e67 6574 5f63   >>> Asset.get_c
+00003c20: 6c61 7373 5f76 616c 7565 2829 0a20 2020  lass_value().   
+00003c30: 2027 666f 6f62 6172 270a 0a6f 626a 5f73   'foobar'..obj_s
+00003c40: 7461 7465 0a5e 5e5e 5e5e 5e5e 5e5e 0a47  tate.^^^^^^^^^.G
+00003c50: 6574 2f75 7064 6174 6520 7468 6520 7374  et/update the st
+00003c60: 6174 6520 6f66 2061 6e20 6f62 6a65 6374  ate of an object
+00003c70: 2c20 736c 6f74 7465 6420 6f72 206e 6f74  , slotted or not
+00003c80: 2028 776f 726b 7320 6576 656e 2069 6e20   (works even in 
+00003c90: 5079 7468 6f6e 2032 2e37 292e 0a0a 2e2e  Python 2.7).....
+00003ca0: 2063 6f64 653a 3a20 7079 7468 6f6e 0a0a   code:: python..
+00003cb0: 2020 2020 3e3e 3e20 6672 6f6d 2062 6173      >>> from bas
+00003cc0: 6963 636f 2e6f 626a 5f73 7461 7465 2069  icco.obj_state i
+00003cd0: 6d70 6f72 7420 6765 745f 7374 6174 650a  mport get_state.
+00003ce0: 2020 2020 3e3e 3e20 636c 6173 7320 536c      >>> class Sl
+00003cf0: 6f74 7465 6428 6f62 6a65 6374 293a 0a20  otted(object):. 
+00003d00: 2020 202e 2e2e 2020 2020 205f 5f73 6c6f     ...     __slo
+00003d10: 7473 5f5f 203d 2028 2266 6f6f 222c 2022  ts__ = ("foo", "
+00003d20: 6261 7222 290a 2020 2020 2e2e 2e20 2020  bar").    ...   
+00003d30: 2020 6465 6620 5f5f 696e 6974 5f5f 2873    def __init__(s
+00003d40: 656c 662c 2066 6f6f 2c20 6261 7229 3a0a  elf, foo, bar):.
+00003d50: 2020 2020 2e2e 2e20 2020 2020 2020 2020      ...         
+00003d60: 7365 6c66 2e66 6f6f 203d 2066 6f6f 0a20  self.foo = foo. 
+00003d70: 2020 202e 2e2e 2020 2020 2020 2020 2073     ...         s
+00003d80: 656c 662e 6261 7220 3d20 6261 720a 2020  elf.bar = bar.  
+00003d90: 2020 2e2e 2e0a 2020 2020 3e3e 3e20 736c    ....    >>> sl
+00003da0: 6f74 7465 6420 3d20 536c 6f74 7465 6428  otted = Slotted(
+00003db0: 2261 222c 2022 6222 290a 2020 2020 3e3e  "a", "b").    >>
+00003dc0: 3e20 736f 7274 6564 2867 6574 5f73 7461  > sorted(get_sta
+00003dd0: 7465 2873 6c6f 7474 6564 292e 6974 656d  te(slotted).item
+00003de0: 7328 2929 0a20 2020 205b 2827 6261 7227  s()).    [('bar'
+00003df0: 2c20 2762 2729 2c20 2827 666f 6f27 2c20  , 'b'), ('foo', 
+00003e00: 2761 2729 5d0a 0a41 6c73 6f20 7072 6f76  'a')]..Also prov
+00003e10: 6964 6573 2061 2060 5265 6475 6369 626c  ides a `Reducibl
+00003e20: 654d 6574 6160 206d 6574 6163 6c61 7373  eMeta` metaclass
+00003e30: 2074 6861 7420 616c 6c6f 7773 2066 6f72   that allows for
+00003e40: 2070 6963 6b6c 696e 6720 696e 7374 616e   pickling instan
+00003e50: 6365 7320 6f66 2073 6c6f 7474 6564 2063  ces of slotted c
+00003e60: 6c61 7373 6573 2069 6e20 5079 7468 6f6e  lasses in Python
+00003e70: 2032 2e37 2e0a 0a71 7561 6c6e 616d 650a   2.7...qualname.
+00003e80: 5e5e 5e5e 5e5e 5e5e 0a50 7974 686f 6e20  ^^^^^^^^.Python 
+00003e90: 322e 3720 636f 6d70 6174 6962 6c65 2077  2.7 compatible w
+00003ea0: 6179 206f 6620 6765 7474 696e 6720 7468  ay of getting th
+00003eb0: 6520 7175 616c 6966 6965 6420 6e61 6d65  e qualified name
+00003ec0: 2e20 4261 7365 6420 6f6e 0a60 7762 6f6c  . Based on.`wbol
+00003ed0: 7374 6572 2f71 7561 6c6e 616d 6520 3c68  ster/qualname <h
+00003ee0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00003ef0: 6d2f 7762 6f6c 7374 6572 2f71 7561 6c6e  m/wbolster/qualn
+00003f00: 616d 653e 605f 2e0a 416c 736f 2070 726f  ame>`_..Also pro
+00003f10: 7669 6465 7320 6120 6051 7561 6c6e 616d  vides a `Qualnam
+00003f20: 6564 4d65 7461 6020 6d65 7461 636c 6173  edMeta` metaclas
+00003f30: 7320 7769 7468 2061 2060 5f5f 7175 616c  s with a `__qual
+00003f40: 6e61 6d65 5f5f 6020 636c 6173 7320 7072  name__` class pr
+00003f50: 6f70 6572 7479 2066 6f72 2050 7974 686f  operty for Pytho
+00003f60: 6e20 322e 372e 0a0a 7265 6375 7273 6976  n 2.7...recursiv
+00003f70: 655f 7265 7072 0a5e 5e5e 5e5e 5e5e 5e5e  e_repr.^^^^^^^^^
+00003f80: 5e5e 5e5e 5e0a 4465 636f 7261 746f 7220  ^^^^^.Decorator 
+00003f90: 7468 6174 2070 7265 7665 6e74 7320 696e  that prevents in
+00003fa0: 6669 6e69 7465 2072 6563 7572 7369 6f6e  finite recursion
+00003fb0: 2066 6f72 2060 5f5f 7265 7072 5f5f 6020   for `__repr__` 
+00003fc0: 6d65 7468 6f64 732e 0a0a 2e2e 2063 6f64  methods..... cod
+00003fd0: 653a 3a20 7079 7468 6f6e 0a0a 2020 2020  e:: python..    
+00003fe0: 3e3e 3e20 6672 6f6d 2062 6173 6963 636f  >>> from basicco
+00003ff0: 2e72 6563 7572 7369 7665 5f72 6570 7220  .recursive_repr 
+00004000: 696d 706f 7274 2072 6563 7572 7369 7665  import recursive
+00004010: 5f72 6570 720a 2020 2020 3e3e 3e20 636c  _repr.    >>> cl
+00004020: 6173 7320 4d79 436c 6173 7328 6f62 6a65  ass MyClass(obje
+00004030: 6374 293a 0a20 2020 202e 2e2e 0a20 2020  ct):.    ....   
+00004040: 202e 2e2e 2020 2020 2040 7265 6375 7273   ...     @recurs
+00004050: 6976 655f 7265 7072 0a20 2020 202e 2e2e  ive_repr.    ...
+00004060: 2020 2020 2064 6566 205f 5f72 6570 725f       def __repr_
+00004070: 5f28 7365 6c66 293a 0a20 2020 202e 2e2e  _(self):.    ...
+00004080: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00004090: 224d 7943 6c61 7373 3c7b 2172 7d3e 222e  "MyClass<{!r}>".
+000040a0: 666f 726d 6174 2873 656c 6629 0a20 2020  format(self).   
+000040b0: 202e 2e2e 0a20 2020 203e 3e3e 206d 795f   ....    >>> my_
+000040c0: 6f62 6a20 3d20 4d79 436c 6173 7328 290a  obj = MyClass().
+000040d0: 2020 2020 3e3e 3e20 7265 7072 286d 795f      >>> repr(my_
+000040e0: 6f62 6a29 0a20 2020 2027 4d79 436c 6173  obj).    'MyClas
+000040f0: 733c 2e2e 2e3e 270a 0a72 756e 7469 6d65  s<...>'..runtime
+00004100: 5f66 696e 616c 0a5e 5e5e 5e5e 5e5e 5e5e  _final.^^^^^^^^^
+00004110: 5e5e 5e5e 0a52 756e 7469 6d65 2d63 6865  ^^^^.Runtime-che
+00004120: 636b 6564 2076 6572 7369 6f6e 206f 6620  cked version of 
+00004130: 7468 6520 6074 7970 696e 672e 6669 6e61  the `typing.fina
+00004140: 6c20 3c68 7474 7073 3a2f 2f64 6f63 732e  l <https://docs.
+00004150: 7079 7468 6f6e 2e6f 7267 2f33 2f6c 6962  python.org/3/lib
+00004160: 7261 7279 2f74 7970 696e 672e 6874 6d6c  rary/typing.html
+00004170: 2374 7970 696e 672e 6669 6e61 6c3e 605f  #typing.final>`_
+00004180: 2064 6563 6f72 6174 6f72 2e0a 0a43 616e   decorator...Can
+00004190: 2062 6520 7573 6564 206f 6e20 6d65 7468   be used on meth
+000041a0: 6f64 732c 2070 726f 7065 7274 6965 732c  ods, properties,
+000041b0: 2063 6c61 7373 6d65 7468 6f64 732c 2073   classmethods, s
+000041c0: 7461 7469 636d 6574 686f 6473 2c20 616e  taticmethods, an
+000041d0: 6420 636c 6173 7365 7320 7468 6174 2068  d classes that h
+000041e0: 6176 6520 6052 756e 7469 6d65 4669 6e61  ave `RuntimeFina
+000041f0: 6c4d 6574 6160 2061 7320 6120 6d65 7461  lMeta` as a meta
+00004200: 636c 6173 732e 0a49 7420 6973 2061 6c73  class..It is als
+00004210: 6f20 7265 636f 676e 697a 6564 2062 7920  o recognized by 
+00004220: 7374 6174 6963 2074 7970 6520 6368 6563  static type chec
+00004230: 6b65 7273 2061 6e64 2070 7265 7665 6e74  kers and prevent
+00004240: 7320 7375 6263 6c61 7373 696e 6720 616e  s subclassing an
+00004250: 642f 6f72 206d 656d 6265 7220 6f76 6572  d/or member over
+00004260: 7269 6469 6e67 2064 7572 696e 6720 7275  riding during ru
+00004270: 6e74 696d 653a 0a0a 2e2e 2063 6f64 653a  ntime:.... code:
+00004280: 3a20 7079 7468 6f6e 0a0a 2020 2020 3e3e  : python..    >>
+00004290: 3e20 6672 6f6d 2073 6978 2069 6d70 6f72  > from six impor
+000042a0: 7420 7769 7468 5f6d 6574 6163 6c61 7373  t with_metaclass
+000042b0: 0a20 2020 203e 3e3e 2066 726f 6d20 6261  .    >>> from ba
+000042c0: 7369 6363 6f2e 7275 6e74 696d 655f 6669  sicco.runtime_fi
+000042d0: 6e61 6c20 696d 706f 7274 2052 756e 7469  nal import Runti
+000042e0: 6d65 4669 6e61 6c4d 6574 612c 2066 696e  meFinalMeta, fin
+000042f0: 616c 0a20 2020 203e 3e3e 2040 6669 6e61  al.    >>> @fina
+00004300: 6c0a 2020 2020 2e2e 2e20 636c 6173 7320  l.    ... class 
+00004310: 4173 7365 7428 7769 7468 5f6d 6574 6163  Asset(with_metac
+00004320: 6c61 7373 2852 756e 7469 6d65 4669 6e61  lass(RuntimeFina
+00004330: 6c4d 6574 612c 206f 626a 6563 7429 293a  lMeta, object)):
+00004340: 0a20 2020 202e 2e2e 2020 2020 2070 6173  .    ...     pas
+00004350: 730a 2020 2020 2e2e 2e0a 2020 2020 3e3e  s.    ....    >>
+00004360: 3e20 636c 6173 7320 5375 6241 7373 6574  > class SubAsset
+00004370: 2841 7373 6574 293a 0a20 2020 202e 2e2e  (Asset):.    ...
+00004380: 2020 2020 2070 6173 730a 2020 2020 2e2e       pass.    ..
+00004390: 2e0a 2020 2020 5472 6163 6562 6163 6b20  ..    Traceback 
+000043a0: 286d 6f73 7420 7265 6365 6e74 2063 616c  (most recent cal
+000043b0: 6c20 6c61 7374 293a 0a20 2020 2054 7970  l last):.    Typ
+000043c0: 6545 7272 6f72 3a20 6361 6e27 7420 7375  eError: can't su
+000043d0: 6263 6c61 7373 2066 696e 616c 2063 6c61  bclass final cla
+000043e0: 7373 2027 4173 7365 7427 0a0a 2e2e 2063  ss 'Asset'.... c
+000043f0: 6f64 653a 3a20 7079 7468 6f6e 0a0a 2020  ode:: python..  
+00004400: 2020 3e3e 3e20 6672 6f6d 2073 6978 2069    >>> from six i
+00004410: 6d70 6f72 7420 7769 7468 5f6d 6574 6163  mport with_metac
+00004420: 6c61 7373 0a20 2020 203e 3e3e 2066 726f  lass.    >>> fro
+00004430: 6d20 6261 7369 6363 6f2e 7275 6e74 696d  m basicco.runtim
+00004440: 655f 6669 6e61 6c20 696d 706f 7274 2052  e_final import R
+00004450: 756e 7469 6d65 4669 6e61 6c4d 6574 612c  untimeFinalMeta,
+00004460: 2066 696e 616c 0a20 2020 203e 3e3e 2063   final.    >>> c
+00004470: 6c61 7373 2041 7373 6574 2877 6974 685f  lass Asset(with_
+00004480: 6d65 7461 636c 6173 7328 5275 6e74 696d  metaclass(Runtim
+00004490: 6546 696e 616c 4d65 7461 2c20 6f62 6a65  eFinalMeta, obje
+000044a0: 6374 2929 3a0a 2020 2020 2e2e 2e20 2020  ct)):.    ...   
+000044b0: 2020 4066 696e 616c 0a20 2020 202e 2e2e    @final.    ...
+000044c0: 2020 2020 2064 6566 206d 6574 686f 6428       def method(
+000044d0: 7365 6c66 293a 0a20 2020 202e 2e2e 2020  self):.    ...  
+000044e0: 2020 2020 2020 2070 6173 730a 2020 2020         pass.    
+000044f0: 2e2e 2e0a 2020 2020 3e3e 3e20 636c 6173  ....    >>> clas
+00004500: 7320 5375 6241 7373 6574 2841 7373 6574  s SubAsset(Asset
+00004510: 293a 0a20 2020 202e 2e2e 2020 2020 2064  ):.    ...     d
+00004520: 6566 206d 6574 686f 6428 7365 6c66 293a  ef method(self):
+00004530: 0a20 2020 202e 2e2e 2020 2020 2020 2020  .    ...        
+00004540: 2070 6173 730a 2020 2020 5472 6163 6562   pass.    Traceb
+00004550: 6163 6b20 286d 6f73 7420 7265 6365 6e74  ack (most recent
+00004560: 2063 616c 6c20 6c61 7374 293a 0a20 2020   call last):.   
+00004570: 2054 7970 6545 7272 6f72 3a20 2753 7562   TypeError: 'Sub
+00004580: 4173 7365 7427 206f 7665 7272 6964 6573  Asset' overrides
+00004590: 2066 696e 616c 206d 656d 6265 7220 276d   final member 'm
+000045a0: 6574 686f 6427 2064 6566 696e 6564 2062  ethod' defined b
+000045b0: 7920 2741 7373 6574 270a 0a2e 2e20 636f  y 'Asset'.... co
+000045c0: 6465 3a3a 2070 7974 686f 6e0a 0a20 2020  de:: python..   
+000045d0: 203e 3e3e 2066 726f 6d20 7369 7820 696d   >>> from six im
+000045e0: 706f 7274 2077 6974 685f 6d65 7461 636c  port with_metacl
+000045f0: 6173 730a 2020 2020 3e3e 3e20 6672 6f6d  ass.    >>> from
+00004600: 2062 6173 6963 636f 2e72 756e 7469 6d65   basicco.runtime
+00004610: 5f66 696e 616c 2069 6d70 6f72 7420 5275  _final import Ru
+00004620: 6e74 696d 6546 696e 616c 4d65 7461 2c20  ntimeFinalMeta, 
+00004630: 6669 6e61 6c0a 2020 2020 3e3e 3e20 636c  final.    >>> cl
+00004640: 6173 7320 4173 7365 7428 7769 7468 5f6d  ass Asset(with_m
+00004650: 6574 6163 6c61 7373 2852 756e 7469 6d65  etaclass(Runtime
+00004660: 4669 6e61 6c4d 6574 612c 206f 626a 6563  FinalMeta, objec
+00004670: 7429 293a 0a20 2020 202e 2e2e 2020 2020  t)):.    ...    
+00004680: 2040 7072 6f70 6572 7479 0a20 2020 202e   @property.    .
+00004690: 2e2e 2020 2020 2040 6669 6e61 6c0a 2020  ..     @final.  
+000046a0: 2020 2e2e 2e20 2020 2020 6465 6620 7072    ...     def pr
+000046b0: 6f70 2873 656c 6629 3a0a 2020 2020 2e2e  op(self):.    ..
+000046c0: 2e20 2020 2020 2020 2020 7061 7373 0a20  .         pass. 
+000046d0: 2020 202e 2e2e 0a20 2020 203e 3e3e 2063     ....    >>> c
+000046e0: 6c61 7373 2053 7562 4173 7365 7428 4173  lass SubAsset(As
+000046f0: 7365 7429 3a0a 2020 2020 2e2e 2e20 2020  set):.    ...   
+00004700: 2020 4070 726f 7065 7274 790a 2020 2020    @property.    
+00004710: 2e2e 2e20 2020 2020 6465 6620 7072 6f70  ...     def prop
+00004720: 2873 656c 6629 3a0a 2020 2020 2e2e 2e20  (self):.    ... 
+00004730: 2020 2020 2020 2020 7061 7373 0a20 2020          pass.   
+00004740: 2054 7261 6365 6261 636b 2028 6d6f 7374   Traceback (most
+00004750: 2072 6563 656e 7420 6361 6c6c 206c 6173   recent call las
+00004760: 7429 3a0a 2020 2020 5479 7065 4572 726f  t):.    TypeErro
+00004770: 723a 2027 5375 6241 7373 6574 2720 6f76  r: 'SubAsset' ov
+00004780: 6572 7269 6465 7320 6669 6e61 6c20 6d65  errides final me
+00004790: 6d62 6572 2027 7072 6f70 2720 6465 6669  mber 'prop' defi
+000047a0: 6e65 6420 6279 2027 4173 7365 7427 0a0a  ned by 'Asset'..
+000047b0: 7361 6665 5f6e 6f74 5f65 7175 616c 730a  safe_not_equals.
+000047c0: 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e 5e0a  ^^^^^^^^^^^^^^^.
+000047d0: 4261 636b 706f 7274 206f 6620 7468 6520  Backport of the 
+000047e0: 6465 6661 756c 7420 5079 7468 6f6e 2033  default Python 3
+000047f0: 2062 6568 6176 696f 7220 6f66 2060 5f5f   behavior of `__
+00004800: 6e65 5f5f 6020 6265 6861 7669 6f72 2066  ne__` behavior f
+00004810: 6f72 2050 7974 686f 6e20 322e 372e 0a0a  or Python 2.7...
+00004820: 2e2e 2063 6f64 653a 3a20 7079 7468 6f6e  .. code:: python
+00004830: 0a0a 2020 2020 3e3e 3e20 6672 6f6d 2073  ..    >>> from s
+00004840: 6978 2069 6d70 6f72 7420 7769 7468 5f6d  ix import with_m
+00004850: 6574 6163 6c61 7373 0a20 2020 203e 3e3e  etaclass.    >>>
+00004860: 2066 726f 6d20 6261 7369 6363 6f2e 7361   from basicco.sa
+00004870: 6665 5f6e 6f74 5f65 7175 616c 7320 696d  fe_not_equals im
+00004880: 706f 7274 2053 6166 654e 6f74 4571 7561  port SafeNotEqua
+00004890: 6c73 4d65 7461 0a20 2020 203e 3e3e 2063  lsMeta.    >>> c
+000048a0: 6c61 7373 2043 6c61 7373 2877 6974 685f  lass Class(with_
+000048b0: 6d65 7461 636c 6173 7328 5361 6665 4e6f  metaclass(SafeNo
+000048c0: 7445 7175 616c 734d 6574 612c 206f 626a  tEqualsMeta, obj
+000048d0: 6563 7429 293a 0a20 2020 202e 2e2e 2020  ect)):.    ...  
+000048e0: 2020 2070 6173 730a 2020 2020 2e2e 2e0a     pass.    ....
+000048f0: 2020 2020 3e3e 3e20 6f62 6a5f 6120 3d20      >>> obj_a = 
+00004900: 436c 6173 7328 290a 2020 2020 3e3e 3e20  Class().    >>> 
+00004910: 6f62 6a5f 6220 3d20 436c 6173 7328 290a  obj_b = Class().
+00004920: 2020 2020 3e3e 3e20 6173 7365 7274 2028      >>> assert (
+00004930: 6f62 6a5f 6120 3d3d 206f 626a 5f61 2920  obj_a == obj_a) 
+00004940: 6973 206e 6f74 2028 6f62 6a5f 6120 213d  is not (obj_a !=
+00004950: 206f 626a 5f61 290a 2020 2020 3e3e 3e20   obj_a).    >>> 
+00004960: 6173 7365 7274 2028 6f62 6a5f 6220 3d3d  assert (obj_b ==
+00004970: 206f 626a 5f62 2920 6973 206e 6f74 2028   obj_b) is not (
+00004980: 6f62 6a5f 6220 213d 206f 626a 5f62 290a  obj_b != obj_b).
+00004990: 2020 2020 3e3e 3e20 6173 7365 7274 2028      >>> assert (
+000049a0: 6f62 6a5f 6120 3d3d 206f 626a 5f62 2920  obj_a == obj_b) 
+000049b0: 6973 206e 6f74 2028 6f62 6a5f 6120 213d  is not (obj_a !=
+000049c0: 206f 626a 5f62 290a 0a73 6166 655f 7265   obj_b)..safe_re
+000049d0: 7072 0a5e 5e5e 5e5e 5e5e 5e5e 0a44 6563  pr.^^^^^^^^^.Dec
+000049e0: 6f72 6174 6f72 2074 6861 7420 7072 6576  orator that prev
+000049f0: 656e 7473 2060 5f5f 7265 7072 5f5f 6020  ents `__repr__` 
+00004a00: 6d65 7468 6f64 7320 6672 6f6d 2072 6169  methods from rai
+00004a10: 7369 6e67 2065 7863 6570 7469 6f6e 7320  sing exceptions 
+00004a20: 616e 6420 7265 7475 726e 2061 2064 6566  and return a def
+00004a30: 6175 6c74 2072 6570 7265 7365 6e74 6174  ault representat
+00004a40: 696f 6e20 696e 7374 6561 642e 0a0a 2e2e  ion instead.....
+00004a50: 2063 6f64 653a 3a20 7079 7468 6f6e 0a0a   code:: python..
+00004a60: 2020 2020 3e3e 3e20 6672 6f6d 2062 6173      >>> from bas
+00004a70: 6963 636f 2e73 6166 655f 7265 7072 2069  icco.safe_repr i
+00004a80: 6d70 6f72 7420 7361 6665 5f72 6570 720a  mport safe_repr.
+00004a90: 2020 2020 3e3e 3e20 636c 6173 7320 436c      >>> class Cl
+00004aa0: 6173 7328 6f62 6a65 6374 293a 0a20 2020  ass(object):.   
+00004ab0: 202e 2e2e 2020 2020 2040 7361 6665 5f72   ...     @safe_r
+00004ac0: 6570 720a 2020 2020 2e2e 2e20 2020 2020  epr.    ...     
+00004ad0: 6465 6620 5f5f 7265 7072 5f5f 2873 656c  def __repr__(sel
+00004ae0: 6629 3a0a 2020 2020 2e2e 2e20 2020 2020  f):.    ...     
+00004af0: 2020 2020 7261 6973 6520 5275 6e74 696d      raise Runtim
+00004b00: 6545 7272 6f72 2822 6f68 206f 6822 290a  eError("oh oh").
+00004b10: 2020 2020 2e2e 2e0a 2020 2020 3e3e 3e20      ....    >>> 
+00004b20: 6f62 6a20 3d20 436c 6173 7328 290a 2020  obj = Class().  
+00004b30: 2020 3e3e 3e20 7265 7072 286f 626a 290a    >>> repr(obj).
+00004b40: 2020 2020 223c 5f5f 6d61 696e 5f5f 2e43      "<__main__.C
+00004b50: 6c61 7373 206f 626a 6563 7420 6174 202e  lass object at .
+00004b60: 2e2e 3b20 7265 7072 2066 6169 6c65 6420  ..; repr failed 
+00004b70: 6475 6520 746f 2027 5275 6e74 696d 6545  due to 'RuntimeE
+00004b80: 7272 6f72 3a20 6f68 206f 6827 3e22 0a0a  rror: oh oh'>"..
+00004b90: 7365 745f 6e61 6d65 0a5e 5e5e 5e5e 5e5e  set_name.^^^^^^^
+00004ba0: 5e0a 4261 636b 706f 7274 206f 6620 7468  ^.Backport of th
+00004bb0: 6520 6675 6e63 7469 6f6e 616c 6974 7920  e functionality 
+00004bc0: 6f66 2060 5f5f 7365 745f 6e61 6d65 5f5f  of `__set_name__
+00004bd0: 6020 6672 6f6d 2050 4550 2034 3837 2074  ` from PEP 487 t
+00004be0: 6f20 5079 7468 6f6e 2032 2e37 2e0a 0a2e  o Python 2.7....
+00004bf0: 2e20 636f 6465 3a3a 2070 7974 686f 6e0a  . code:: python.
+00004c00: 0a20 2020 203e 3e3e 2066 726f 6d20 6261  .    >>> from ba
+00004c10: 7369 6363 6f2e 7365 745f 6e61 6d65 2069  sicco.set_name i
+00004c20: 6d70 6f72 7420 5365 744e 616d 650a 2020  mport SetName.  
+00004c30: 2020 3e3e 3e20 636c 6173 7320 4174 7472    >>> class Attr
+00004c40: 6962 7574 6528 6f62 6a65 6374 293a 0a20  ibute(object):. 
+00004c50: 2020 202e 2e2e 2020 2020 2064 6566 205f     ...     def _
+00004c60: 5f73 6574 5f6e 616d 655f 5f28 7365 6c66  _set_name__(self
+00004c70: 2c20 6f77 6e65 722c 206e 616d 6529 3a0a  , owner, name):.
+00004c80: 2020 2020 2e2e 2e20 2020 2020 2020 2020      ...         
+00004c90: 7365 6c66 2e6f 776e 6572 203d 206f 776e  self.owner = own
+00004ca0: 6572 0a20 2020 202e 2e2e 2020 2020 2020  er.    ...      
+00004cb0: 2020 2073 656c 662e 6e61 6d65 203d 206e     self.name = n
+00004cc0: 616d 650a 2020 2020 2e2e 2e0a 2020 2020  ame.    ....    
+00004cd0: 3e3e 3e20 636c 6173 7320 436f 6c6c 6563  >>> class Collec
+00004ce0: 7469 6f6e 2853 6574 4e61 6d65 293a 0a20  tion(SetName):. 
+00004cf0: 2020 202e 2e2e 2020 2020 2066 6f6f 203d     ...     foo =
+00004d00: 2041 7474 7269 6275 7465 2829 0a20 2020   Attribute().   
+00004d10: 202e 2e2e 0a20 2020 203e 3e3e 2043 6f6c   ....    >>> Col
+00004d20: 6c65 6374 696f 6e2e 666f 6f2e 6f77 6e65  lection.foo.owne
+00004d30: 7220 6973 2043 6f6c 6c65 6374 696f 6e0a  r is Collection.
+00004d40: 2020 2020 5472 7565 0a20 2020 203e 3e3e      True.    >>>
+00004d50: 2043 6f6c 6c65 6374 696f 6e2e 666f 6f2e   Collection.foo.
+00004d60: 6e61 6d65 0a20 2020 2027 666f 6f27 0a0a  name.    'foo'..
+00004d70: 7479 7065 5f63 6865 636b 696e 670a 5e5e  type_checking.^^
+00004d80: 5e5e 5e5e 5e5e 5e5e 5e5e 5e0a 5275 6e74  ^^^^^^^^^^^.Runt
+00004d90: 696d 6520 7479 7065 2063 6865 636b 696e  ime type checkin
+00004da0: 6720 7769 7468 2073 7570 706f 7274 2066  g with support f
+00004db0: 6f72 2069 6d70 6f72 7420 7061 7468 7320  or import paths 
+00004dc0: 616e 6420 7479 7065 2068 696e 7473 2e0a  and type hints..
+00004dd0: 0a2e 2e20 636f 6465 3a3a 2070 7974 686f  ... code:: pytho
+00004de0: 6e0a 0a20 2020 203e 3e3e 2066 726f 6d20  n..    >>> from 
+00004df0: 7469 7070 6f20 696d 706f 7274 204d 6170  tippo import Map
+00004e00: 7069 6e67 2c20 4c69 7465 7261 6c0a 2020  ping, Literal.  
+00004e10: 2020 3e3e 3e20 6672 6f6d 2069 7465 7274    >>> from itert
+00004e20: 6f6f 6c73 2069 6d70 6f72 7420 6368 6169  ools import chai
+00004e30: 6e0a 2020 2020 3e3e 3e20 6672 6f6d 2062  n.    >>> from b
+00004e40: 6173 6963 636f 2e74 7970 655f 6368 6563  asicco.type_chec
+00004e50: 6b69 6e67 2069 6d70 6f72 7420 6973 5f69  king import is_i
+00004e60: 6e73 7461 6e63 650a 2020 2020 3e3e 3e20  nstance.    >>> 
+00004e70: 636c 6173 7320 5375 6243 6861 696e 2863  class SubChain(c
+00004e80: 6861 696e 293a 0a20 2020 202e 2e2e 2020  hain):.    ...  
+00004e90: 2020 2070 6173 730a 2020 2020 2e2e 2e0a     pass.    ....
+00004ea0: 2020 2020 3e3e 3e20 6973 5f69 6e73 7461      >>> is_insta
+00004eb0: 6e63 6528 332c 2069 6e74 290a 2020 2020  nce(3, int).    
+00004ec0: 5472 7565 0a20 2020 203e 3e3e 2069 735f  True.    >>> is_
+00004ed0: 696e 7374 616e 6365 2833 2c20 2863 6861  instance(3, (cha
+00004ee0: 696e 2c20 696e 7429 290a 2020 2020 5472  in, int)).    Tr
+00004ef0: 7565 0a20 2020 203e 3e3e 2069 735f 696e  ue.    >>> is_in
+00004f00: 7374 616e 6365 2833 2c20 2829 290a 2020  stance(3, ()).  
+00004f10: 2020 4661 6c73 650a 2020 2020 3e3e 3e20    False.    >>> 
+00004f20: 6973 5f69 6e73 7461 6e63 6528 5375 6243  is_instance(SubC
+00004f30: 6861 696e 2829 2c20 2269 7465 7274 6f6f  hain(), "itertoo
+00004f40: 6c73 2e63 6861 696e 2229 0a20 2020 2054  ls.chain").    T
+00004f50: 7275 650a 2020 2020 3e3e 3e20 6973 5f69  rue.    >>> is_i
+00004f60: 6e73 7461 6e63 6528 6368 6169 6e28 292c  nstance(chain(),
+00004f70: 2022 6974 6572 746f 6f6c 732e 6368 6169   "itertools.chai
+00004f80: 6e22 2c20 7375 6274 7970 6573 3d46 616c  n", subtypes=Fal
+00004f90: 7365 290a 2020 2020 5472 7565 0a20 2020  se).    True.   
+00004fa0: 203e 3e3e 2069 735f 696e 7374 616e 6365   >>> is_instance
+00004fb0: 2853 7562 4368 6169 6e28 292c 2022 6974  (SubChain(), "it
+00004fc0: 6572 746f 6f6c 732e 6368 6169 6e22 2c20  ertools.chain", 
+00004fd0: 7375 6274 7970 6573 3d46 616c 7365 290a  subtypes=False).
+00004fe0: 2020 2020 4661 6c73 650a 2020 2020 3e3e      False.    >>
+00004ff0: 3e20 6973 5f69 6e73 7461 6e63 6528 7b22  > is_instance({"
+00005000: 6122 3a20 312c 2022 6222 3a20 327d 2c20  a": 1, "b": 2}, 
+00005010: 4d61 7070 696e 675b 7374 722c 2069 6e74  Mapping[str, int
+00005020: 5d29 0a20 2020 2054 7275 650a 2020 2020  ]).    True.    
+00005030: 3e3e 3e20 6973 5f69 6e73 7461 6e63 6528  >>> is_instance(
+00005040: 2250 5245 222c 204c 6974 6572 616c 5b22  "PRE", Literal["
+00005050: 5052 4522 2c20 2250 4f53 5422 5d29 0a20  PRE", "POST"]). 
+00005060: 2020 2054 7275 650a 0a75 6e69 7175 655f     True..unique_
+00005070: 6974 6572 6174 6f72 0a5e 5e5e 5e5e 5e5e  iterator.^^^^^^^
+00005080: 5e5e 5e5e 5e5e 5e5e 0a49 7465 7261 746f  ^^^^^^^^.Iterato
+00005090: 7220 7468 6174 2079 6965 6c64 7320 756e  r that yields un
+000050a0: 6971 7565 2076 616c 7565 732e 0a0a 2e2e  ique values.....
+000050b0: 2063 6f64 653a 3a20 7079 7468 6f6e 0a0a   code:: python..
+000050c0: 2020 2020 3e3e 3e20 6672 6f6d 2062 6173      >>> from bas
+000050d0: 6963 636f 2e75 6e69 7175 655f 6974 6572  icco.unique_iter
+000050e0: 6174 6f72 2069 6d70 6f72 7420 756e 6971  ator import uniq
+000050f0: 7565 5f69 7465 7261 746f 720a 2020 2020  ue_iterator.    
+00005100: 3e3e 3e20 6c69 7374 2875 6e69 7175 655f  >>> list(unique_
+00005110: 6974 6572 6174 6f72 285b 312c 2032 2c20  iterator([1, 2, 
+00005120: 332c 2033 2c20 342c 2034 2c20 355d 2929  3, 3, 4, 4, 5]))
+00005130: 0a20 2020 205b 312c 2032 2c20 332c 2034  .    [1, 2, 3, 4
+00005140: 2c20 355d 0a0a 7765 616b 5f72 6566 6572  , 5]..weak_refer
+00005150: 656e 6365 0a5e 5e5e 5e5e 5e5e 5e5e 5e5e  ence.^^^^^^^^^^^
+00005160: 5e5e 5e0a 5765 616b 2052 6566 6572 656e  ^^^.Weak Referen
+00005170: 6365 2d6c 696b 6520 6f62 6a65 6374 2074  ce-like object t
+00005180: 6861 7420 7375 7070 6f72 7473 2070 6963  hat supports pic
+00005190: 6b6c 696e 672e                           kling.
```

### Comparing `basicco-8.9.0/README.rst` & `basicco-9.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,1299 +1,1335 @@
-00000000: 2e2e 206c 6f67 6f5f 7374 6172 740a 2e2e  .. logo_start...
-00000010: 2072 6177 3a3a 2068 746d 6c0a 0a20 2020   raw:: html..   
-00000020: 3c70 2061 6c69 676e 3d22 6365 6e74 6572  <p align="center
-00000030: 223e 0a20 2020 2020 3c61 2068 7265 663d  ">.     <a href=
-00000040: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
-00000050: 636f 6d2f 6272 756e 6f6e 6963 6b6f 2f62  com/brunonicko/b
-00000060: 6173 6963 636f 223e 0a20 2020 2020 2020  asicco">.       
-00000070: 2020 3c70 6963 7475 7265 3e0a 2020 2020    <picture>.    
-00000080: 2020 2020 2020 2020 3c6f 626a 6563 7420          <object 
-00000090: 6461 7461 3d22 2e2f 5f73 7461 7469 632f  data="./_static/
-000000a0: 6261 7369 6363 6f2e 7376 6722 2074 7970  basicco.svg" typ
-000000b0: 653d 2269 6d61 6765 2f70 6e67 223e 0a20  e="image/png">. 
-000000c0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-000000d0: 736f 7572 6365 2073 7263 7365 743d 222e  source srcset=".
-000000e0: 2f64 6f63 732f 736f 7572 6365 2f5f 7374  /docs/source/_st
-000000f0: 6174 6963 2f62 6173 6963 636f 5f77 6869  atic/basicco_whi
-00000100: 7465 2e73 7667 2220 6d65 6469 613d 2228  te.svg" media="(
-00000110: 7072 6566 6572 732d 636f 6c6f 722d 7363  prefers-color-sc
-00000120: 6865 6d65 3a20 6461 726b 2922 3e0a 2020  heme: dark)">.  
-00000130: 2020 2020 2020 2020 2020 2020 2020 3c69                <i
-00000140: 6d67 2073 7263 3d22 2e2f 646f 6373 2f73  mg src="./docs/s
-00000150: 6f75 7263 652f 5f73 7461 7469 632f 6261  ource/_static/ba
-00000160: 7369 6363 6f2e 7376 6722 2077 6964 7468  sicco.svg" width
-00000170: 3d22 3630 2522 2061 6c74 3d22 6261 7369  ="60%" alt="basi
-00000180: 6363 6f22 202f 3e0a 2020 2020 2020 2020  cco" />.        
-00000190: 2020 2020 3c2f 6f62 6a65 6374 3e0a 2020      </object>.  
-000001a0: 2020 2020 2020 203c 2f70 6963 7475 7265         </picture
-000001b0: 3e0a 2020 2020 203c 2f61 3e0a 2020 203c  >.     </a>.   <
-000001c0: 2f70 3e0a 2e2e 206c 6f67 6f5f 656e 640a  /p>... logo_end.
-000001d0: 0a2e 2e20 696d 6167 653a 3a20 6874 7470  ... image:: http
-000001e0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f62  s://github.com/b
-000001f0: 7275 6e6f 6e69 636b 6f2f 6261 7369 6363  runonicko/basicc
-00000200: 6f2f 776f 726b 666c 6f77 732f 4d79 5079  o/workflows/MyPy
-00000210: 2f62 6164 6765 2e73 7667 0a20 2020 3a74  /badge.svg.   :t
-00000220: 6172 6765 743a 2068 7474 7073 3a2f 2f67  arget: https://g
-00000230: 6974 6875 622e 636f 6d2f 6272 756e 6f6e  ithub.com/brunon
-00000240: 6963 6b6f 2f62 6173 6963 636f 2f61 6374  icko/basicco/act
-00000250: 696f 6e73 3f71 7565 7279 3d77 6f72 6b66  ions?query=workf
-00000260: 6c6f 7725 3341 4d79 5079 0a0a 2e2e 2069  low%3AMyPy.... i
-00000270: 6d61 6765 3a3a 2068 7474 7073 3a2f 2f67  mage:: https://g
-00000280: 6974 6875 622e 636f 6d2f 6272 756e 6f6e  ithub.com/brunon
-00000290: 6963 6b6f 2f62 6173 6963 636f 2f77 6f72  icko/basicco/wor
-000002a0: 6b66 6c6f 7773 2f4c 696e 742f 6261 6467  kflows/Lint/badg
-000002b0: 652e 7376 670a 2020 203a 7461 7267 6574  e.svg.   :target
-000002c0: 3a20 6874 7470 733a 2f2f 6769 7468 7562  : https://github
-000002d0: 2e63 6f6d 2f62 7275 6e6f 6e69 636b 6f2f  .com/brunonicko/
-000002e0: 6261 7369 6363 6f2f 6163 7469 6f6e 733f  basicco/actions?
-000002f0: 7175 6572 793d 776f 726b 666c 6f77 2533  query=workflow%3
-00000300: 414c 696e 740a 0a2e 2e20 696d 6167 653a  ALint.... image:
-00000310: 3a20 6874 7470 733a 2f2f 6769 7468 7562  : https://github
-00000320: 2e63 6f6d 2f62 7275 6e6f 6e69 636b 6f2f  .com/brunonicko/
-00000330: 6261 7369 6363 6f2f 776f 726b 666c 6f77  basicco/workflow
-00000340: 732f 5465 7374 732f 6261 6467 652e 7376  s/Tests/badge.sv
-00000350: 670a 2020 203a 7461 7267 6574 3a20 6874  g.   :target: ht
-00000360: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000370: 2f62 7275 6e6f 6e69 636b 6f2f 6261 7369  /brunonicko/basi
-00000380: 6363 6f2f 6163 7469 6f6e 733f 7175 6572  cco/actions?quer
-00000390: 793d 776f 726b 666c 6f77 2533 4154 6573  y=workflow%3ATes
-000003a0: 7473 0a0a 2e2e 2069 6d61 6765 3a3a 2068  ts.... image:: h
-000003b0: 7474 7073 3a2f 2f72 6561 6474 6865 646f  ttps://readthedo
-000003c0: 6373 2e6f 7267 2f70 726f 6a65 6374 732f  cs.org/projects/
-000003d0: 6261 7369 6363 6f2f 6261 6467 652f 3f76  basicco/badge/?v
-000003e0: 6572 7369 6f6e 3d73 7461 626c 650a 2020  ersion=stable.  
-000003f0: 203a 7461 7267 6574 3a20 6874 7470 733a   :target: https:
-00000400: 2f2f 6261 7369 6363 6f2e 7265 6164 7468  //basicco.readth
-00000410: 6564 6f63 732e 696f 2f65 6e2f 7374 6162  edocs.io/en/stab
-00000420: 6c65 2f0a 0a2e 2e20 696d 6167 653a 3a20  le/.... image:: 
-00000430: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
-00000440: 6c64 732e 696f 2f67 6974 6875 622f 6c69  lds.io/github/li
-00000450: 6365 6e73 652f 6272 756e 6f6e 6963 6b6f  cense/brunonicko
-00000460: 2f62 6173 6963 636f 3f63 6f6c 6f72 3d6c  /basicco?color=l
-00000470: 6967 6874 2d67 7265 656e 0a20 2020 3a74  ight-green.   :t
-00000480: 6172 6765 743a 2068 7474 7073 3a2f 2f67  arget: https://g
-00000490: 6974 6875 622e 636f 6d2f 6272 756e 6f6e  ithub.com/brunon
-000004a0: 6963 6b6f 2f62 6173 6963 636f 2f62 6c6f  icko/basicco/blo
-000004b0: 622f 6d61 7374 6572 2f4c 4943 454e 5345  b/master/LICENSE
-000004c0: 0a0a 2e2e 2069 6d61 6765 3a3a 2068 7474  .... image:: htt
-000004d0: 7073 3a2f 2f73 7461 7469 632e 7065 7079  ps://static.pepy
-000004e0: 2e74 6563 682f 7065 7273 6f6e 616c 697a  .tech/personaliz
-000004f0: 6564 2d62 6164 6765 2f62 6173 6963 636f  ed-badge/basicco
-00000500: 3f70 6572 696f 643d 746f 7461 6c26 756e  ?period=total&un
-00000510: 6974 733d 696e 7465 726e 6174 696f 6e61  its=internationa
-00000520: 6c5f 7379 7374 656d 266c 6566 745f 636f  l_system&left_co
-00000530: 6c6f 723d 6772 6579 2672 6967 6874 5f63  lor=grey&right_c
-00000540: 6f6c 6f72 3d62 7269 6768 7467 7265 656e  olor=brightgreen
-00000550: 266c 6566 745f 7465 7874 3d44 6f77 6e6c  &left_text=Downl
-00000560: 6f61 6473 0a20 2020 3a74 6172 6765 743a  oads.   :target:
-00000570: 2068 7474 7073 3a2f 2f70 6570 792e 7465   https://pepy.te
-00000580: 6368 2f70 726f 6a65 6374 2f62 6173 6963  ch/project/basic
-00000590: 636f 0a0a 2e2e 2069 6d61 6765 3a3a 2068  co.... image:: h
-000005a0: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
-000005b0: 6473 2e69 6f2f 7079 7069 2f70 7976 6572  ds.io/pypi/pyver
-000005c0: 7369 6f6e 732f 6261 7369 6363 6f3f 636f  sions/basicco?co
-000005d0: 6c6f 723d 6c69 6768 742d 6772 6565 6e26  lor=light-green&
-000005e0: 7374 796c 653d 666c 6174 0a20 2020 3a74  style=flat.   :t
-000005f0: 6172 6765 743a 2068 7474 7073 3a2f 2f70  arget: https://p
-00000600: 7970 692e 6f72 672f 7072 6f6a 6563 742f  ypi.org/project/
-00000610: 6261 7369 6363 6f2f 0a0a 4f76 6572 7669  basicco/..Overvi
-00000620: 6577 0a2d 2d2d 2d2d 2d2d 2d0a 6062 6173  ew.--------.`bas
-00000630: 6963 636f 6020 6973 2061 2050 7974 686f  icco` is a Pytho
-00000640: 6e20 7061 636b 6167 6520 7468 6174 2070  n package that p
-00000650: 726f 7669 6465 7320 6c6f 772d 6c65 7665  rovides low-leve
-00000660: 6c20 6042 6173 6520 436c 6173 7365 7360  l `Base Classes`
-00000670: 5f20 616e 6420 6055 7469 6c69 7469 6573  _ and `Utilities
-00000680: 605f 2074 6f20 656e 6861 6e63 6520 636f  `_ to enhance co
-00000690: 6465 2063 6f6d 7061 7469 6269 6c69 7479  de compatibility
-000006a0: 2c0a 6665 6174 7572 6573 2061 6e64 2076  ,.features and v
-000006b0: 616c 6964 6174 696f 6e2e 0a0a 4d6f 7469  alidation...Moti
-000006c0: 7661 7469 6f6e 0a2d 2d2d 2d2d 2d2d 2d2d  vation.---------
-000006d0: 2d0a 5768 696c 6520 6465 7665 6c6f 7069  -.While developi
-000006e0: 6e67 2050 7974 686f 6e20 736f 6674 7761  ng Python softwa
-000006f0: 7265 2066 6f72 2056 6973 7561 6c20 4566  re for Visual Ef
-00000700: 6665 6374 7320 7069 7065 6c69 6e65 732c  fects pipelines,
-00000710: 2049 2066 6f75 6e64 206d 7973 656c 6620   I found myself 
-00000720: 6861 7669 6e67 2074 6f20 7772 6974 6520  having to write 
-00000730: 7468 6520 7361 6d65 2062 6f69 6c65 722d  the same boiler-
-00000740: 706c 6174 650a 636f 6465 206f 7665 7220  plate.code over 
-00000750: 616e 6420 6f76 6572 2061 6761 696e 2c20  and over again, 
-00000760: 6173 2077 656c 6c20 6173 2073 7472 7567  as well as strug
-00000770: 676c 696e 6720 7769 7468 2063 6f6d 7061  gling with compa
-00000780: 7469 6269 6c69 7479 2069 7373 7565 7320  tibility issues 
-00000790: 616e 6420 6665 6174 7572 6520 6761 7073  and feature gaps
-000007a0: 2062 6574 7765 656e 2050 7974 686f 6e20   between Python 
-000007b0: 322e 3720 616e 640a 5079 7468 6f6e 2033  2.7 and.Python 3
-000007c0: 2e37 2b2e 0a0a 536f 2049 2064 6563 6964  .7+...So I decid
-000007d0: 6564 2074 6f20 696d 706c 656d 656e 7420  ed to implement 
-000007e0: 736f 6c75 7469 6f6e 7320 666f 7220 7468  solutions for th
-000007f0: 6f73 6520 6973 7375 6573 2061 7420 7468  ose issues at th
-00000800: 6520 6042 6173 6560 5f2c 2061 6e64 2060  e `Base`_, and `
-00000810: 6261 7369 6363 6f60 2077 6173 2062 6f72  basicco` was bor
-00000820: 6e2e 0a0a 4261 7365 2043 6c61 7373 6573  n...Base Classes
-00000830: 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 0a43  .------------..C
-00000840: 6f6d 7061 7442 6173 650a 5e5e 5e5e 5e5e  ompatBase.^^^^^^
-00000850: 5e5e 5e5e 0a54 6865 2067 6f61 6c20 7769  ^^^^.The goal wi
-00000860: 7468 2074 6865 2060 436f 6d70 6174 4261  th the `CompatBa
-00000870: 7365 4d65 7461 6020 6d65 7461 636c 6173  seMeta` metaclas
-00000880: 7320 616e 6420 7468 6520 6043 6f6d 7061  s and the `Compa
-00000890: 7442 6173 6560 2063 6c61 7373 2069 7320  tBase` class is 
-000008a0: 746f 2062 7269 6467 6520 736f 6d65 206f  to bridge some o
-000008b0: 6620 7468 6520 6665 6174 7572 6520 6761  f the feature ga
-000008c0: 7073 2062 6574 7765 656e 0a50 7974 686f  ps between.Pytho
-000008d0: 6e20 322e 3720 616e 6420 5079 7468 6f6e  n 2.7 and Python
-000008e0: 2033 2e37 2b2e 0a0a 5468 6973 2069 6e63   3.7+...This inc
-000008f0: 6c75 6465 7320 6164 6469 6e67 2050 7974  ludes adding Pyt
-00000900: 686f 6e20 322e 3720 776f 726b 6172 6f75  hon 2.7 workarou
-00000910: 6e64 7320 666f 723a 0a20 202d 2060 4162  nds for:.  - `Ab
-00000920: 7374 7261 6374 2070 726f 7065 7274 6965  stract propertie
-00000930: 7320 3c68 7474 7073 3a2f 2f64 6f63 732e  s <https://docs.
-00000940: 7079 7468 6f6e 2e6f 7267 2f33 2f6c 6962  python.org/3/lib
-00000950: 7261 7279 2f61 6263 2e68 746d 6c23 6162  rary/abc.html#ab
-00000960: 632e 6162 7374 7261 6374 7072 6f70 6572  c.abstractproper
-00000970: 7479 3e60 5f3a 2042 6574 7465 7220 6061  ty>`_: Better `a
-00000980: 6273 7472 6163 746d 6574 686f 6460 0a20  bstractmethod`. 
-00000990: 2020 2064 6563 6f72 6174 6f72 2073 7570     decorator sup
-000009a0: 706f 7274 2066 6f72 2070 726f 7065 7274  port for propert
-000009b0: 792d 6c69 6b65 2064 6573 6372 6970 746f  y-like descripto
-000009c0: 7273 2e20 5365 6520 616c 736f 2060 6162  rs. See also `ab
-000009d0: 7374 7261 6374 5f63 6c61 7373 605f 2e0a  stract_class`_..
-000009e0: 2020 2d20 6050 4550 2034 3837 203c 6874    - `PEP 487 <ht
-000009f0: 7470 733a 2f2f 7065 7073 2e70 7974 686f  tps://peps.pytho
-00000a00: 6e2e 6f72 672f 7065 702d 3034 3837 2f3e  n.org/pep-0487/>
-00000a10: 605f 3a20 5375 7070 6f72 7420 666f 7220  `_: Support for 
-00000a20: 605f 5f69 6e69 745f 7375 6263 6c61 7373  `__init_subclass
-00000a30: 5f5f 6020 616e 6420 605f 5f73 6574 5f6e  __` and `__set_n
-00000a40: 616d 655f 5f60 2e0a 2020 2020 5365 6520  ame__`..    See 
-00000a50: 616c 736f 2060 696e 6974 5f73 7562 636c  also `init_subcl
-00000a60: 6173 7360 5f20 616e 6420 6073 6574 5f6e  ass`_ and `set_n
-00000a70: 616d 6560 5f2e 0a20 202d 2060 6f62 6a65  ame`_..  - `obje
-00000a80: 6374 2e5f 5f64 6972 5f5f 203c 6874 7470  ct.__dir__ <http
-00000a90: 733a 2f2f 646f 6373 2e70 7974 686f 6e2e  s://docs.python.
-00000aa0: 6f72 672f 332f 7265 6665 7265 6e63 652f  org/3/reference/
-00000ab0: 6461 7461 6d6f 6465 6c2e 6874 6d6c 236f  datamodel.html#o
-00000ac0: 626a 6563 742e 5f5f 6469 725f 5f3e 605f  bject.__dir__>`_
-00000ad0: 3a20 4261 7365 2060 5f5f 6469 725f 5f60  : Base `__dir__`
-00000ae0: 206d 6574 686f 642e 0a20 2020 2053 6565   method..    See
-00000af0: 2061 6c73 6f20 6064 6566 6175 6c74 5f64   also `default_d
-00000b00: 6972 605f 2e0a 2020 2d20 605f 5f65 715f  ir`_..  - `__eq_
-00000b10: 5f20 6f76 6572 7269 6465 203c 6874 7470  _ override <http
-00000b20: 733a 2f2f 646f 6373 2e70 7974 686f 6e2e  s://docs.python.
-00000b30: 6f72 672f 332f 7265 6665 7265 6e63 652f  org/3/reference/
-00000b40: 6461 7461 6d6f 6465 6c2e 6874 6d6c 236f  datamodel.html#o
-00000b50: 626a 6563 742e 5f5f 6861 7368 5f5f 3e60  bject.__hash__>`
-00000b60: 5f3a 204f 7665 7272 6964 696e 6720 605f  _: Overriding `_
-00000b70: 5f65 715f 5f60 2077 696c 6c0a 2020 2020  _eq__` will.    
-00000b80: 7365 7420 605f 5f68 6173 685f 5f60 2074  set `__hash__` t
-00000b90: 6f20 4e6f 6e65 2e20 5365 6520 616c 736f  o None. See also
-00000ba0: 2060 696d 706c 6963 6974 5f68 6173 6860   `implicit_hash`
-00000bb0: 5f2e 0a20 202d 2060 5045 5020 3330 3720  _..  - `PEP 307 
-00000bc0: 3c68 7474 7073 3a2f 2f70 6570 732e 7079  <https://peps.py
-00000bd0: 7468 6f6e 2e6f 7267 2f70 6570 2d30 3330  thon.org/pep-030
-00000be0: 372f 3e60 5f3a 2053 7570 706f 7274 2066  7/>`_: Support f
-00000bf0: 6f72 2070 6963 6b6c 696e 6720 6f62 6a65  or pickling obje
-00000c00: 6374 7320 7769 7468 2060 5f5f 736c 6f74  cts with `__slot
-00000c10: 735f 5f60 2e0a 2020 2020 5365 6520 616c  s__`..    See al
-00000c20: 736f 2060 6f62 6a5f 7374 6174 6560 5f2e  so `obj_state`_.
-00000c30: 0a20 202d 2060 5045 5020 3331 3535 203c  .  - `PEP 3155 <
-00000c40: 6874 7470 733a 2f2f 7065 7073 2e70 7974  https://peps.pyt
-00000c50: 686f 6e2e 6f72 672f 7065 702d 3033 3135  hon.org/pep-0315
-00000c60: 352f 3e60 5f3a 2051 7561 6c69 6669 6564  5/>`_: Qualified
-00000c70: 206e 616d 6520 605f 5f71 7561 6c6e 616d   name `__qualnam
-00000c80: 655f 5f60 2066 6f72 206e 6573 7465 6420  e__` for nested 
-00000c90: 636c 6173 7365 732e 0a20 2020 2053 6565  classes..    See
-00000ca0: 2061 6c73 6f20 6071 7561 6c6e 616d 6560   also `qualname`
-00000cb0: 5f2e 0a20 202d 2060 5f5f 6e65 5f5f 2062  _..  - `__ne__ b
-00000cc0: 6568 6176 696f 7220 3c68 7474 7073 3a2f  ehavior <https:/
-00000cd0: 2f64 6f63 732e 7079 7468 6f6e 2e6f 7267  /docs.python.org
-00000ce0: 2f33 2e30 2f77 6861 7473 6e65 772f 332e  /3.0/whatsnew/3.
-00000cf0: 302e 6874 6d6c 236f 7065 7261 746f 7273  0.html#operators
-00000d00: 2d61 6e64 2d73 7065 6369 616c 2d6d 6574  -and-special-met
-00000d10: 686f 6473 3e60 5f3a 2042 7920 6465 6661  hods>`_: By defa
-00000d20: 756c 742c 0a20 2020 2060 5f5f 6e65 5f5f  ult,.    `__ne__
-00000d30: 6020 7368 6f75 6c64 206e 6567 6174 6520  ` should negate 
-00000d40: 7468 6520 7265 7375 6c74 206f 6620 605f  the result of `_
-00000d50: 5f65 715f 5f60 2e0a 2020 2020 5365 6520  _eq__`..    See 
-00000d60: 616c 736f 2060 7361 6665 5f6e 6f74 5f65  also `safe_not_e
-00000d70: 7175 616c 7360 5f0a 2020 2d20 6050 4550  quals`_.  - `PEP
-00000d80: 2030 3536 3020 3c68 7474 7073 3a2f 2f70   0560 <https://p
-00000d90: 6570 732e 7079 7468 6f6e 2e6f 7267 2f70  eps.python.org/p
-00000da0: 6570 2d30 3536 302f 3e60 5f3a 2042 6574  ep-0560/>`_: Bet
-00000db0: 7465 7220 6861 6e64 6c69 6e67 206f 6620  ter handling of 
-00000dc0: 4765 6e65 7269 6320 636c 6173 7365 732e  Generic classes.
-00000dd0: 0a20 2020 2053 6565 2061 6c73 6f20 6074  .    See also `t
-00000de0: 6970 706f 203c 6874 7470 733a 2f2f 6769  ippo <https://gi
-00000df0: 7468 7562 2e63 6f6d 2f62 7275 6e6f 6e69  thub.com/brunoni
-00000e00: 636b 6f2f 7469 7070 6f23 6765 6e65 7269  cko/tippo#generi
-00000e10: 632d 6669 7865 733e 605f 2e0a 0a42 6173  c-fixes>`_...Bas
-00000e20: 650a 5e5e 5e5e 0a49 6e20 6164 6469 7469  e.^^^^.In additi
-00000e30: 6f6e 2074 6f20 7468 6520 636f 6d70 6174  on to the compat
-00000e40: 6962 696c 6974 7920 736f 6c75 7469 6f6e  ibility solution
-00000e50: 732c 2074 6865 2067 6f61 6c20 7769 7468  s, the goal with
-00000e60: 2074 6865 2060 4261 7365 4d65 7461 6020   the `BaseMeta` 
-00000e70: 6d65 7461 636c 6173 7320 616e 6420 7468  metaclass and th
-00000e80: 6520 6042 6173 6560 2063 6c61 7373 2069  e `Base` class i
-00000e90: 7320 746f 2061 6464 0a75 7365 6675 6c20  s to add.useful 
-00000ea0: 6c6f 772d 6c65 7665 6c20 6665 6174 7572  low-level featur
-00000eb0: 6573 2074 6861 7420 686f 7065 6675 6c6c  es that hopefull
-00000ec0: 7920 7969 656c 6420 6265 7474 6572 2063  y yield better c
-00000ed0: 6f64 6520 7265 6164 6162 696c 6974 7920  ode readability 
-00000ee0: 616e 6420 7661 6c69 6461 7469 6f6e 2e0a  and validation..
-00000ef0: 0a54 6869 7320 696e 636c 7564 6573 3a0a  .This includes:.
-00000f00: 2020 2d20 605f 5f77 6561 6b72 6566 5f5f    - `__weakref__
-00000f10: 6020 736c 6f74 3a20 4164 6465 6420 6279  ` slot: Added by
-00000f20: 2064 6566 6175 6c74 2e0a 2020 2d20 606c   default..  - `l
-00000f30: 6f63 6b65 645f 636c 6173 7360 5f3a 2050  ocked_class`_: P
-00000f40: 7562 6c69 6320 636c 6173 7320 6174 7472  ublic class attr
-00000f50: 6962 7574 6573 2061 7265 2072 6561 642d  ibutes are read-
-00000f60: 6f6e 6c79 2062 7920 6465 6661 756c 742e  only by default.
-00000f70: 0a20 202d 2060 6578 706c 6963 6974 5f68  .  - `explicit_h
-00000f80: 6173 6860 5f3a 204f 7665 7272 6964 696e  ash`_: Overridin
-00000f90: 6720 605f 5f65 715f 5f60 2077 6974 686f  g `__eq__` witho
-00000fa0: 7574 206f 7665 7272 6964 696e 6720 605f  ut overriding `_
-00000fb0: 5f68 6173 685f 5f60 2077 696c 6c20 7261  _hash__` will ra
-00000fc0: 6973 6520 616e 2065 7272 6f72 2e0a 2020  ise an error..  
-00000fd0: 2d20 606e 616d 6573 7061 6365 605f 3a20  - `namespace`_: 
-00000fe0: 4164 6473 2061 2070 726f 7465 6374 6564  Adds a protected
-00000ff0: 2060 5f5f 6e61 6d65 7370 6163 6560 2075   `__namespace` u
-00001000: 6e69 7175 6520 746f 2065 6163 6820 636c  nique to each cl
-00001010: 6173 732e 0a20 202d 2060 7275 6e74 696d  ass..  - `runtim
-00001020: 655f 6669 6e61 6c60 5f3a 2052 756e 7469  e_final`_: Runti
-00001030: 6d65 2063 6865 636b 696e 6720 666f 7220  me checking for 
-00001040: 636c 6173 7365 7320 616e 6420 6d65 7468  classes and meth
-00001050: 6f64 7320 6465 636f 7261 7465 6420 7769  ods decorated wi
-00001060: 7468 2060 6669 6e61 6c60 2e0a 0a53 6c6f  th `final`...Slo
-00001070: 7474 6564 4261 7365 0a5e 5e5e 5e5e 5e5e  ttedBase.^^^^^^^
-00001080: 5e5e 5e5e 0a54 6865 2060 536c 6f74 7465  ^^^^.The `Slotte
-00001090: 6442 6173 6560 2063 6c61 7373 2061 6e64  dBase` class and
-000010a0: 2074 6865 2060 536c 6f74 7465 6442 6173   the `SlottedBas
-000010b0: 654d 6574 6160 206d 6574 6163 6c61 7373  eMeta` metaclass
-000010c0: 206f 6666 6572 2061 6c6c 2066 6561 7475   offer all featu
-000010d0: 7265 7320 6672 6f6d 2060 4261 7365 6020  res from `Base` 
-000010e0: 616e 6420 6042 6173 654d 6574 6160 2070  and `BaseMeta` p
-000010f0: 6c75 7320 696d 706c 6963 6974 0a60 5f5f  lus implicit.`__
-00001100: 736c 6f74 735f 5f60 2064 6563 6c61 7261  slots__` declara
-00001110: 7469 6f6e 2e20 5365 6520 6073 6c6f 7474  tion. See `slott
-00001120: 6564 203c 6874 7470 733a 2f2f 6769 7468  ed <https://gith
-00001130: 7562 2e63 6f6d 2f62 7275 6e6f 6e69 636b  ub.com/brunonick
-00001140: 6f2f 736c 6f74 7465 643e 605f 2066 6f72  o/slotted>`_ for
-00001150: 206d 6f72 6520 696e 666f 726d 6174 696f   more informatio
-00001160: 6e2e 0a0a 5574 696c 6974 6965 730a 2d2d  n...Utilities.--
-00001170: 2d2d 2d2d 2d2d 2d0a 4170 6172 7420 6672  -------.Apart fr
-00001180: 6f6d 2074 6865 2066 6561 7475 7265 7320  om the features 
-00001190: 696e 7465 6772 6174 6564 2069 6e74 6f20  integrated into 
-000011a0: 7468 6520 6261 7365 2063 6c61 7373 6573  the base classes
-000011b0: 2c20 6062 6173 6963 636f 6020 7072 6f76  , `basicco` prov
-000011c0: 6964 6573 2061 2076 6172 6965 7479 206f  ides a variety o
-000011d0: 6620 6765 6e65 7261 6c20 7574 696c 6974  f general utilit
-000011e0: 6965 732e 0a54 686f 7365 2063 616e 2062  ies..Those can b
-000011f0: 6520 696d 706f 7274 6564 2066 726f 6d20  e imported from 
-00001200: 7468 6520 7375 622d 6d6f 6475 6c65 7320  the sub-modules 
-00001210: 6465 7363 7269 6265 6420 6265 6c6f 772e  described below.
-00001220: 0a0a 6162 7374 7261 6374 5f63 6c61 7373  ..abstract_class
-00001230: 0a5e 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e 5e0a  .^^^^^^^^^^^^^^.
-00001240: 4265 7474 6572 2060 6162 7374 7261 6374  Better `abstract
-00001250: 2063 6c61 7373 6573 203c 6874 7470 733a   classes <https:
-00001260: 2f2f 646f 6373 2e70 7974 686f 6e2e 6f72  //docs.python.or
-00001270: 672f 332f 6c69 6272 6172 792f 6162 632e  g/3/library/abc.
-00001280: 6874 6d6c 2361 6263 2e61 6273 7472 6163  html#abc.abstrac
-00001290: 746d 6574 686f 643e 605f 2073 7570 706f  tmethod>`_ suppo
-000012a0: 7274 2e0a 0a50 726f 7669 6465 7320 6162  rt...Provides ab
-000012b0: 7374 7261 6374 2064 6563 6f72 6174 6f72  stract decorator
-000012c0: 7320 7468 6174 2063 616e 2062 6520 7573  s that can be us
-000012d0: 6564 2064 6972 6563 746c 7920 6f6e 206d  ed directly on m
-000012e0: 6574 686f 6473 2062 7574 2061 6c73 6f20  ethods but also 
-000012f0: 6f6e 2063 6c61 7373 6573 2c20 7072 6f70  on classes, prop
-00001300: 6572 7469 6573 2c20 636c 6173 736d 6574  erties, classmet
-00001310: 686f 6473 2c20 616e 640a 7374 6174 6963  hods, and.static
-00001320: 6d65 7468 6f64 7320 2865 7665 6e20 696e  methods (even in
-00001330: 2050 7974 686f 6e20 322e 3729 2e0a 0a2e   Python 2.7)....
-00001340: 2e20 636f 6465 3a3a 2070 7974 686f 6e0a  . code:: python.
-00001350: 0a20 2020 203e 3e3e 2066 726f 6d20 7369  .    >>> from si
-00001360: 7820 696d 706f 7274 2077 6974 685f 6d65  x import with_me
-00001370: 7461 636c 6173 730a 2020 2020 3e3e 3e20  taclass.    >>> 
-00001380: 6672 6f6d 2062 6173 6963 636f 2e61 6273  from basicco.abs
-00001390: 7472 6163 745f 636c 6173 7320 696d 706f  tract_class impo
-000013a0: 7274 2041 6273 7472 6163 744d 6574 612c  rt AbstractMeta,
-000013b0: 2061 6273 7472 6163 740a 2020 2020 3e3e   abstract.    >>
-000013c0: 3e20 636c 6173 7320 4173 7365 7428 7769  > class Asset(wi
-000013d0: 7468 5f6d 6574 6163 6c61 7373 2841 6273  th_metaclass(Abs
-000013e0: 7472 6163 744d 6574 612c 206f 626a 6563  tractMeta, objec
-000013f0: 7429 293a 0a20 2020 202e 2e2e 2020 2020  t)):.    ...    
-00001400: 2040 6162 7374 7261 6374 0a20 2020 202e   @abstract.    .
-00001410: 2e2e 2020 2020 2064 6566 206d 6574 686f  ..     def metho
-00001420: 6428 7365 6c66 293a 0a20 2020 202e 2e2e  d(self):.    ...
-00001430: 2020 2020 2020 2020 2070 6173 730a 2020           pass.  
-00001440: 2020 2e2e 2e0a 2020 2020 2e2e 2e20 2020    ....    ...   
-00001450: 2020 4070 726f 7065 7274 790a 2020 2020    @property.    
-00001460: 2e2e 2e20 2020 2020 4061 6273 7472 6163  ...     @abstrac
-00001470: 740a 2020 2020 2e2e 2e20 2020 2020 6465  t.    ...     de
-00001480: 6620 7072 6f70 2873 656c 6629 3a0a 2020  f prop(self):.  
-00001490: 2020 2e2e 2e20 2020 2020 2020 2020 7265    ...         re
-000014a0: 7475 726e 204e 6f6e 650a 2020 2020 2e2e  turn None.    ..
-000014b0: 2e0a 2020 2020 3e3e 3e20 4173 7365 7428  ..    >>> Asset(
-000014c0: 290a 2020 2020 5472 6163 6562 6163 6b20  ).    Traceback 
-000014d0: 286d 6f73 7420 7265 6365 6e74 2063 616c  (most recent cal
-000014e0: 6c20 6c61 7374 293a 0a20 2020 2054 7970  l last):.    Typ
-000014f0: 6545 7272 6f72 3a20 4361 6e27 7420 696e  eError: Can't in
-00001500: 7374 616e 7469 6174 6520 6162 7374 7261  stantiate abstra
-00001510: 6374 2063 6c61 7373 2041 7373 6574 2077  ct class Asset w
-00001520: 6974 6820 6162 7374 7261 6374 206d 6574  ith abstract met
-00001530: 686f 6473 206d 6574 686f 642c 2070 726f  hods method, pro
-00001540: 700a 0a2e 2e20 636f 6465 3a3a 2070 7974  p.... code:: pyt
-00001550: 686f 6e0a 0a20 2020 203e 3e3e 2066 726f  hon..    >>> fro
-00001560: 6d20 6261 7369 6363 6f2e 6162 7374 7261  m basicco.abstra
-00001570: 6374 5f63 6c61 7373 2069 6d70 6f72 7420  ct_class import 
-00001580: 4162 7374 7261 6374 4d65 7461 2c20 6162  AbstractMeta, ab
-00001590: 7374 7261 6374 0a20 2020 203e 3e3e 2040  stract.    >>> @
-000015a0: 6162 7374 7261 6374 0a20 2020 202e 2e2e  abstract.    ...
-000015b0: 2063 6c61 7373 2041 7373 6574 2877 6974   class Asset(wit
-000015c0: 685f 6d65 7461 636c 6173 7328 4162 7374  h_metaclass(Abst
-000015d0: 7261 6374 4d65 7461 2c20 6f62 6a65 6374  ractMeta, object
-000015e0: 2929 3a0a 2020 2020 2e2e 2e20 2020 2020  )):.    ...     
-000015f0: 7061 7373 0a20 2020 202e 2e2e 0a20 2020  pass.    ....   
-00001600: 203e 3e3e 2041 7373 6574 2829 0a20 2020   >>> Asset().   
-00001610: 2054 7261 6365 6261 636b 2028 6d6f 7374   Traceback (most
-00001620: 2072 6563 656e 7420 6361 6c6c 206c 6173   recent call las
-00001630: 7429 3a0a 2020 2020 5479 7065 4572 726f  t):.    TypeErro
-00001640: 723a 2063 616e 2774 2069 6e73 7461 6e74  r: can't instant
-00001650: 6961 7465 2061 6273 7472 6163 7420 636c  iate abstract cl
-00001660: 6173 7320 2741 7373 6574 270a 0a62 6173  ass 'Asset'..bas
-00001670: 6963 5f64 6174 610a 5e5e 5e5e 5e5e 5e5e  ic_data.^^^^^^^^
-00001680: 5e5e 0a45 6173 6573 2074 6865 2074 6173  ^^.Eases the tas
-00001690: 6b20 6f66 2063 7265 6174 696e 6720 7369  k of creating si
-000016a0: 6d70 6c65 2064 6174 6120 636f 6e74 6169  mple data contai
-000016b0: 6e65 7220 636c 6173 7365 7320 7468 6174  ner classes that
-000016c0: 2073 7570 706f 7274 2065 7175 616c 6974   support equalit
-000016d0: 7920 636f 6d70 6172 6973 6f6e 732c 2068  y comparisons, h
-000016e0: 6173 6869 6e67 2c20 7374 7269 6e67 0a72  ashing, string.r
-000016f0: 6570 7265 7365 6e74 6174 696f 6e2c 2063  epresentation, c
-00001700: 6f6e 7665 7273 696f 6e20 746f 2064 6963  onversion to dic
-00001710: 7469 6f6e 6172 792c 2065 7463 2e0a 0a2e  tionary, etc....
-00001720: 2e20 636f 6465 3a3a 2070 7974 686f 6e0a  . code:: python.
-00001730: 0a20 2020 203e 3e3e 2066 726f 6d20 6d61  .    >>> from ma
-00001740: 7468 2069 6d70 6f72 7420 7371 7274 0a20  th import sqrt. 
-00001750: 2020 203e 3e3e 2066 726f 6d20 6261 7369     >>> from basi
-00001760: 6363 6f2e 6261 7369 635f 6461 7461 2069  cco.basic_data i
-00001770: 6d70 6f72 7420 4974 656d 5573 6563 6173  mport ItemUsecas
-00001780: 652c 2042 6173 6963 4461 7461 0a20 2020  e, BasicData.   
-00001790: 203e 3e3e 2063 6c61 7373 2056 6563 746f   >>> class Vecto
-000017a0: 7228 4261 7369 6344 6174 6129 3a0a 2020  r(BasicData):.  
-000017b0: 2020 2e2e 2e20 2020 2020 5f5f 736c 6f74    ...     __slot
-000017c0: 735f 5f20 3d20 2822 7822 2c20 2279 2229  s__ = ("x", "y")
-000017d0: 0a20 2020 202e 2e2e 2020 2020 2064 6566  .    ...     def
-000017e0: 205f 5f69 6e69 745f 5f28 7365 6c66 2c20   __init__(self, 
-000017f0: 782c 2079 293a 0a20 2020 202e 2e2e 2020  x, y):.    ...  
-00001800: 2020 2020 2020 2073 656c 662e 7820 3d20         self.x = 
-00001810: 780a 2020 2020 2e2e 2e20 2020 2020 2020  x.    ...       
-00001820: 2020 7365 6c66 2e79 203d 2079 0a20 2020    self.y = y.   
-00001830: 202e 2e2e 2020 2020 2064 6566 2074 6f5f   ...     def to_
-00001840: 6974 656d 7328 7365 6c66 2c20 7573 6563  items(self, usec
-00001850: 6173 653d 4e6f 6e65 293a 0a20 2020 202e  ase=None):.    .
-00001860: 2e2e 2020 2020 2020 2020 2069 7465 6d73  ..         items
-00001870: 203d 205b 2822 7822 2c20 7365 6c66 2e78   = [("x", self.x
-00001880: 292c 2028 2279 222c 2073 656c 662e 7929  ), ("y", self.y)
-00001890: 5d0a 2020 2020 2e2e 2e20 2020 2020 2020  ].    ...       
-000018a0: 2020 6966 2075 7365 6361 7365 2069 7320    if usecase is 
-000018b0: 4974 656d 5573 6563 6173 652e 5245 5052  ItemUsecase.REPR
-000018c0: 3a0a 2020 2020 2e2e 2e20 2020 2020 2020  :.    ...       
-000018d0: 2020 2020 2020 6974 656d 732e 6170 7065        items.appe
-000018e0: 6e64 2828 226d 6167 222c 2073 656c 662e  nd(("mag", self.
-000018f0: 6d61 6729 290a 2020 2020 2e2e 2e20 2020  mag)).    ...   
-00001900: 2020 2020 2020 7265 7475 726e 2069 7465        return ite
-00001910: 6d73 0a20 2020 202e 2e2e 2020 2020 2040  ms.    ...     @
-00001920: 7072 6f70 6572 7479 0a20 2020 202e 2e2e  property.    ...
-00001930: 2020 2020 2064 6566 206d 6167 2873 656c       def mag(sel
-00001940: 6629 3a0a 2020 2020 2e2e 2e20 2020 2020  f):.    ...     
-00001950: 2020 2020 7265 7475 726e 2073 7172 7428      return sqrt(
-00001960: 7365 6c66 2e78 2a2a 3220 2b20 7365 6c66  self.x**2 + self
-00001970: 2e79 2a2a 3229 0a20 2020 202e 2e2e 0a20  .y**2).    .... 
-00001980: 2020 203e 3e3e 2056 6563 746f 7228 332e     >>> Vector(3.
-00001990: 302c 2034 2e30 290a 2020 2020 5665 6374  0, 4.0).    Vect
-000019a0: 6f72 2878 3d33 2e30 2c20 793d 342e 302c  or(x=3.0, y=4.0,
-000019b0: 203c 6d61 673d 352e 303e 290a 0a63 616c   <mag=5.0>)..cal
-000019c0: 6c65 725f 6d6f 6475 6c65 0a5e 5e5e 5e5e  ler_module.^^^^^
-000019d0: 5e5e 5e5e 5e5e 5e5e 0a52 6574 7269 6576  ^^^^^^^^.Retriev
-000019e0: 6520 7468 6520 6361 6c6c 6572 2773 206d  e the caller's m
-000019f0: 6f64 756c 6520 6e61 6d65 2e0a 0a2e 2e20  odule name..... 
-00001a00: 636f 6465 3a3a 2070 7974 686f 6e0a 0a20  code:: python.. 
-00001a10: 2020 203e 3e3e 2066 726f 6d20 6261 7369     >>> from basi
-00001a20: 6363 6f2e 6361 6c6c 6572 5f6d 6f64 756c  cco.caller_modul
-00001a30: 6520 696d 706f 7274 2063 616c 6c65 725f  e import caller_
-00001a40: 6d6f 6475 6c65 0a20 2020 203e 3e3e 2064  module.    >>> d
-00001a50: 6566 2064 6f5f 736f 6d65 7468 696e 6728  ef do_something(
-00001a60: 293a 0a20 2020 202e 2e2e 2020 2020 2072  ):.    ...     r
-00001a70: 6574 7572 6e20 2249 2077 6173 2063 616c  eturn "I was cal
-00001a80: 6c65 6420 6279 207b 7d22 2e66 6f72 6d61  led by {}".forma
-00001a90: 7428 6361 6c6c 6572 5f6d 6f64 756c 6528  t(caller_module(
-00001aa0: 2929 0a20 2020 202e 2e2e 0a20 2020 203e  )).    ....    >
-00001ab0: 3e3e 2064 6f5f 736f 6d65 7468 696e 6728  >> do_something(
-00001ac0: 290a 2020 2020 2749 2077 6173 2063 616c  ).    'I was cal
-00001ad0: 6c65 6420 6279 205f 5f6d 6169 6e5f 5f27  led by __main__'
-00001ae0: 0a0a 636f 6e74 6578 745f 7661 7273 0a5e  ..context_vars.^
-00001af0: 5e5e 5e5e 5e5e 5e5e 5e5e 5e0a 4261 636b  ^^^^^^^^^^^.Back
-00001b00: 706f 7274 206f 6620 7468 6520 6063 6f6e  port of the `con
-00001b10: 7465 7874 7661 7273 6020 6d6f 6475 6c65  textvars` module
-00001b20: 2066 6f72 2050 7974 686f 6e20 322e 372c   for Python 2.7,
-00001b30: 2062 6173 6564 206f 6e0a 604d 6167 6963   based on.`Magic
-00001b40: 5374 6163 6b2f 636f 6e74 6578 7476 6172  Stack/contextvar
-00001b50: 7320 3c68 7474 7073 3a2f 2f67 6974 6875  s <https://githu
-00001b60: 622e 636f 6d2f 4d61 6769 6353 7461 636b  b.com/MagicStack
-00001b70: 2f63 6f6e 7465 7874 7661 7273 3e60 5f2e  /contextvars>`_.
-00001b80: 0a0a 5768 656e 2069 6d70 6f72 7465 6420  ..When imported 
-00001b90: 6672 6f6d 2050 7974 686f 6e20 332c 2069  from Python 3, i
-00001ba0: 7420 7265 6469 7265 6374 7320 7468 6520  t redirects the 
-00001bb0: 636f 6e74 656e 7473 2074 6f20 7468 6520  contents to the 
-00001bc0: 6e61 7469 7665 0a60 636f 6e74 6578 7476  native.`contextv
-00001bd0: 6172 7320 3c68 7474 7073 3a2f 2f64 6f63  ars <https://doc
-00001be0: 732e 7079 7468 6f6e 2e6f 7267 2f33 2f6c  s.python.org/3/l
-00001bf0: 6962 7261 7279 2f63 6f6e 7465 7874 7661  ibrary/contextva
-00001c00: 7273 2e68 746d 6c3e 605f 206d 6f64 756c  rs.html>`_ modul
-00001c10: 652e 0a0a 2e2e 2063 6f64 653a 3a20 7079  e..... code:: py
-00001c20: 7468 6f6e 0a0a 2020 2020 3e3e 3e20 6672  thon..    >>> fr
-00001c30: 6f6d 2062 6173 6963 636f 2e63 6f6e 7465  om basicco.conte
-00001c40: 7874 5f76 6172 7320 696d 706f 7274 2043  xt_vars import C
-00001c50: 6f6e 7465 7874 5661 720a 2020 2020 3e3e  ontextVar.    >>
-00001c60: 3e20 6d79 5f76 6172 203d 2043 6f6e 7465  > my_var = Conte
-00001c70: 7874 5661 7228 226d 795f 7661 7222 2c20  xtVar("my_var", 
-00001c80: 6465 6661 756c 743d 2262 6172 2229 0a20  default="bar"). 
-00001c90: 2020 203e 3e3e 2074 6f6b 656e 203d 206d     >>> token = m
-00001ca0: 795f 7661 722e 7365 7428 2266 6f6f 2229  y_var.set("foo")
-00001cb0: 0a20 2020 203e 3e3e 206d 795f 7661 722e  .    >>> my_var.
-00001cc0: 6765 7428 290a 2020 2020 2766 6f6f 270a  get().    'foo'.
-00001cd0: 2020 2020 3e3e 3e20 6d79 5f76 6172 2e72      >>> my_var.r
-00001ce0: 6573 6574 2874 6f6b 656e 290a 2020 2020  eset(token).    
-00001cf0: 3e3e 3e20 6d79 5f76 6172 2e67 6574 2829  >>> my_var.get()
-00001d00: 0a20 2020 2027 6261 7227 0a0a 6375 7374  .    'bar'..cust
-00001d10: 6f6d 5f72 6570 720a 5e5e 5e5e 5e5e 5e5e  om_repr.^^^^^^^^
-00001d20: 5e5e 5e0a 4375 7374 6f6d 2072 6570 7265  ^^^.Custom repre
-00001d30: 7365 6e74 6174 696f 6e20 6675 6e63 7469  sentation functi
-00001d40: 6f6e 7320 666f 7220 6d61 7070 696e 6773  ons for mappings
-00001d50: 2c20 6974 656d 732c 2061 6e64 2069 7465  , items, and ite
-00001d60: 7261 626c 6573 2e0a 0a2e 2e20 636f 6465  rables..... code
-00001d70: 3a3a 2070 7974 686f 6e0a 0a20 2020 203e  :: python..    >
-00001d80: 3e3e 2066 726f 6d20 6261 7369 6363 6f2e  >> from basicco.
-00001d90: 6375 7374 6f6d 5f72 6570 7220 696d 706f  custom_repr impo
-00001da0: 7274 206d 6170 7069 6e67 5f72 6570 720a  rt mapping_repr.
-00001db0: 2020 2020 3e3e 3e20 6463 7420 3d20 7b22      >>> dct = {"
-00001dc0: 6122 3a20 312c 2022 6222 3a20 327d 0a20  a": 1, "b": 2}. 
-00001dd0: 2020 203e 3e3e 206d 6170 7069 6e67 5f72     >>> mapping_r
-00001de0: 6570 7228 6463 742c 2070 7265 6669 783d  epr(dct, prefix=
-00001df0: 223c 222c 2073 7566 6669 783d 223e 222c  "<", suffix=">",
-00001e00: 2074 656d 706c 6174 653d 227b 6b65 797d   template="{key}
-00001e10: 3d7b 7661 6c75 657d 222c 2073 6f72 7469  ={value}", sorti
-00001e20: 6e67 3d54 7275 6529 0a20 2020 2022 3c27  ng=True).    "<'
-00001e30: 6127 3d31 2c20 2762 273d 323e 220a 0a2e  a'=1, 'b'=2>"...
-00001e40: 2e20 636f 6465 3a3a 2070 7974 686f 6e0a  . code:: python.
-00001e50: 0a20 2020 203e 3e3e 2066 726f 6d20 6261  .    >>> from ba
-00001e60: 7369 6363 6f2e 6375 7374 6f6d 5f72 6570  sicco.custom_rep
-00001e70: 7220 696d 706f 7274 206d 6170 7069 6e67  r import mapping
-00001e80: 5f72 6570 720a 2020 2020 3e3e 3e20 6974  _repr.    >>> it
-00001e90: 656d 7320 3d20 5b28 2261 222c 2031 292c  ems = [("a", 1),
-00001ea0: 2028 2262 222c 2032 295d 0a20 2020 203e   ("b", 2)].    >
-00001eb0: 3e3e 206d 6170 7069 6e67 5f72 6570 7228  >> mapping_repr(
-00001ec0: 6974 656d 732c 2070 7265 6669 783d 225b  items, prefix="[
-00001ed0: 222c 2073 7566 6669 783d 225d 222c 2074  ", suffix="]", t
-00001ee0: 656d 706c 6174 653d 6c61 6d62 6461 2069  emplate=lambda i
-00001ef0: 2c20 6b65 792c 2076 616c 7565 3a20 6b65  , key, value: ke
-00001f00: 7920 2b20 2220 2d3e 2022 202b 2076 616c  y + " -> " + val
-00001f10: 7565 290a 2020 2020 225b 2761 2720 2d3e  ue).    "['a' ->
-00001f20: 2031 2c20 2762 2720 2d3e 2032 5d22 0a0a   1, 'b' -> 2]"..
-00001f30: 2e2e 2063 6f64 653a 3a20 7079 7468 6f6e  .. code:: python
-00001f40: 0a0a 2020 2020 3e3e 3e20 6672 6f6d 2062  ..    >>> from b
-00001f50: 6173 6963 636f 2e63 7573 746f 6d5f 7265  asicco.custom_re
-00001f60: 7072 2069 6d70 6f72 7420 6974 6572 6162  pr import iterab
-00001f70: 6c65 5f72 6570 720a 2020 2020 3e3e 3e20  le_repr.    >>> 
-00001f80: 7475 7020 3d20 2822 6122 2c20 2262 222c  tup = ("a", "b",
-00001f90: 2022 6322 2c20 312c 2032 2c20 3329 0a20   "c", 1, 2, 3). 
-00001fa0: 2020 203e 3e3e 2069 7465 7261 626c 655f     >>> iterable_
-00001fb0: 7265 7072 2874 7570 2c20 7072 6566 6978  repr(tup, prefix
-00001fc0: 3d22 3c22 2c20 7375 6666 6978 3d22 3e22  ="<", suffix=">"
-00001fd0: 2c20 7661 6c75 655f 7265 7072 3d73 7472  , value_repr=str
-00001fe0: 290a 2020 2020 273c 612c 2062 2c20 632c  ).    '<a, b, c,
-00001ff0: 2031 2c20 322c 2033 3e27 0a0a 6465 6661   1, 2, 3>'..defa
-00002000: 756c 745f 6469 720a 5e5e 5e5e 5e5e 5e5e  ult_dir.^^^^^^^^
-00002010: 5e5e 5e0a 4261 636b 706f 7274 206f 6620  ^^^.Backport of 
-00002020: 5079 7468 6f6e 2033 2773 2069 6d70 6c65  Python 3's imple
-00002030: 6d65 6e74 6174 696f 6e20 6f66 0a60 6f62  mentation of.`ob
-00002040: 6a65 6374 2e5f 5f64 6972 5f5f 203c 6874  ject.__dir__ <ht
-00002050: 7470 733a 2f2f 646f 6373 2e70 7974 686f  tps://docs.pytho
-00002060: 6e2e 6f72 672f 332f 7265 6665 7265 6e63  n.org/3/referenc
-00002070: 652f 6461 7461 6d6f 6465 6c2e 6874 6d6c  e/datamodel.html
-00002080: 236f 626a 6563 742e 5f5f 6469 725f 5f3e  #object.__dir__>
-00002090: 605f 2066 6f72 2050 7974 686f 6e20 322e  `_ for Python 2.
-000020a0: 372e 0a0a 5468 6973 2061 6c6c 6f77 7320  7...This allows 
-000020b0: 666f 7220 6361 6c6c 696e 6720 6073 7570  for calling `sup
-000020c0: 6572 2829 2e5f 5f64 6972 5f5f 2829 6020  er().__dir__()` 
-000020d0: 6672 6f6d 2061 2073 7562 636c 6173 7320  from a subclass 
-000020e0: 746f 206c 6576 6572 6167 6520 7468 6520  to leverage the 
-000020f0: 6465 6661 756c 7420 696d 706c 656d 656e  default implemen
-00002100: 7461 7469 6f6e 2e0a 0a2e 2e20 636f 6465  tation..... code
-00002110: 3a3a 2070 7974 686f 6e0a 0a20 2020 203e  :: python..    >
-00002120: 3e3e 2066 726f 6d20 7369 7820 696d 706f  >> from six impo
-00002130: 7274 2077 6974 685f 6d65 7461 636c 6173  rt with_metaclas
-00002140: 730a 2020 2020 3e3e 3e20 6672 6f6d 2062  s.    >>> from b
-00002150: 6173 6963 636f 2e64 6566 6175 6c74 5f64  asicco.default_d
-00002160: 6972 2069 6d70 6f72 7420 4465 6661 756c  ir import Defaul
-00002170: 7444 6972 0a20 2020 203e 3e3e 2063 6c61  tDir.    >>> cla
-00002180: 7373 2043 6c61 7373 2844 6566 6175 6c74  ss Class(Default
-00002190: 4469 7229 3a0a 2020 2020 2e2e 2e20 2020  Dir):.    ...   
-000021a0: 2020 6465 6620 5f5f 6469 725f 5f28 7365    def __dir__(se
-000021b0: 6c66 293a 0a20 2020 202e 2e2e 2020 2020  lf):.    ...    
-000021c0: 2020 2020 2072 6574 7572 6e20 7375 7065       return supe
-000021d0: 7228 436c 6173 732c 2073 656c 6629 2e5f  r(Class, self)._
-000021e0: 5f64 6972 5f5f 2829 0a20 2020 202e 2e2e  _dir__().    ...
-000021f0: 0a20 2020 203e 3e3e 206f 626a 203d 2043  .    >>> obj = C
-00002200: 6c61 7373 2829 0a20 2020 203e 3e3e 2064  lass().    >>> d
-00002210: 6972 286f 626a 290a 2020 2020 5b2e 2e2e  ir(obj).    [...
-00002220: 5d0a 0a64 796e 616d 6963 5f63 6f64 650a  ]..dynamic_code.
-00002230: 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e 0a47 656e  ^^^^^^^^^^^^.Gen
-00002240: 6572 6174 6520 6465 6275 6767 6162 6c65  erate debuggable
-00002250: 2063 6f64 6520 6f6e 2074 6865 2066 6c79   code on the fly
-00002260: 2074 6861 7420 7375 7070 6f72 7473 206c   that supports l
-00002270: 696e 6520 6e75 6d62 6572 7320 6f6e 2074  ine numbers on t
-00002280: 7261 6365 6261 636b 732e 0a0a 2e2e 2063  racebacks..... c
-00002290: 6f64 653a 3a20 7079 7468 6f6e 0a0a 2020  ode:: python..  
-000022a0: 2020 3e3e 3e20 6672 6f6d 2062 6173 6963    >>> from basic
-000022b0: 636f 2e64 796e 616d 6963 5f63 6f64 6520  co.dynamic_code 
-000022c0: 696d 706f 7274 206d 616b 655f 6675 6e63  import make_func
-000022d0: 7469 6f6e 2c20 6765 6e65 7261 7465 5f75  tion, generate_u
-000022e0: 6e69 7175 655f 6669 6c65 6e61 6d65 0a20  nique_filename. 
-000022f0: 2020 203e 3e3e 2063 6c61 7373 204d 7943     >>> class MyC
-00002300: 6c61 7373 286f 626a 6563 7429 3a0a 2020  lass(object):.  
-00002310: 2020 2e2e 2e20 2020 2020 7061 7373 0a20    ...     pass. 
-00002320: 2020 202e 2e2e 0a20 2020 203e 3e3e 2062     ....    >>> b
-00002330: 6172 203d 2027 6261 7227 0a20 2020 203e  ar = 'bar'.    >
-00002340: 3e3e 2023 2050 7265 7061 7265 2074 6865  >> # Prepare the
-00002350: 2073 6372 6970 7420 616e 6420 6e65 6365   script and nece
-00002360: 7373 6172 7920 6461 7461 2e0a 2020 2020  ssary data..    
-00002370: 3e3e 3e20 7363 7269 7074 203d 2022 5c6e  >>> script = "\n
-00002380: 222e 6a6f 696e 280a 2020 2020 2e2e 2e20  ".join(.    ... 
-00002390: 2020 2020 280a 2020 2020 2e2e 2e20 2020      (.    ...   
-000023a0: 2020 2020 2020 2264 6566 205f 5f69 6e69        "def __ini
-000023b0: 745f 5f28 7365 6c66 293a 222c 0a20 2020  t__(self):",.   
-000023c0: 202e 2e2e 2020 2020 2020 2020 2022 2020   ...         "  
-000023d0: 2020 7365 6c66 2e66 6f6f 203d 2027 6261    self.foo = 'ba
-000023e0: 7227 222c 0a20 2020 202e 2e2e 2020 2020  r'",.    ...    
-000023f0: 2029 0a20 2020 202e 2e2e 2029 0a20 2020   ).    ... ).   
-00002400: 203e 3e3e 2023 2047 6174 6865 7220 696e   >>> # Gather in
-00002410: 666f 726d 6174 696f 6e2e 0a20 2020 203e  formation..    >
-00002420: 3e3e 206e 616d 6520 3d20 225f 5f69 6e69  >> name = "__ini
-00002430: 745f 5f22 0a20 2020 203e 3e3e 206f 776e  t__".    >>> own
-00002440: 6572 5f6e 616d 6520 3d20 4d79 436c 6173  er_name = MyClas
-00002450: 732e 5f5f 6e61 6d65 5f5f 0a20 2020 203e  s.__name__.    >
-00002460: 3e3e 206d 6f64 756c 6520 3d20 4d79 436c  >> module = MyCl
-00002470: 6173 732e 5f5f 6d6f 6475 6c65 5f5f 0a20  ass.__module__. 
-00002480: 2020 203e 3e3e 2066 696c 656e 616d 6520     >>> filename 
-00002490: 3d20 6765 6e65 7261 7465 5f75 6e69 7175  = generate_uniqu
-000024a0: 655f 6669 6c65 6e61 6d65 286e 616d 652c  e_filename(name,
-000024b0: 206d 6f64 756c 652c 206f 776e 6572 5f6e   module, owner_n
-000024c0: 616d 6529 0a20 2020 203e 3e3e 2067 6c6f  ame).    >>> glo
-000024d0: 6273 203d 207b 2262 6172 223a 2062 6172  bs = {"bar": bar
-000024e0: 7d0a 2020 2020 3e3e 3e20 2320 4d61 6b65  }.    >>> # Make
-000024f0: 2066 756e 6374 696f 6e20 616e 6420 6174   function and at
-00002500: 7461 6368 2069 7420 6173 2061 206d 6574  tach it as a met
-00002510: 686f 642e 0a20 2020 203e 3e3e 204d 7943  hod..    >>> MyC
-00002520: 6c61 7373 2e5f 5f69 6e69 745f 5f20 3d20  lass.__init__ = 
-00002530: 6d61 6b65 5f66 756e 6374 696f 6e28 6e61  make_function(na
-00002540: 6d65 2c20 7363 7269 7074 2c20 676c 6f62  me, script, glob
-00002550: 732c 2066 696c 656e 616d 652c 206d 6f64  s, filename, mod
-00002560: 756c 6529 0a20 2020 203e 3e3e 206f 626a  ule).    >>> obj
-00002570: 203d 204d 7943 6c61 7373 2829 0a20 2020   = MyClass().   
-00002580: 203e 3e3e 206f 626a 2e66 6f6f 0a20 2020   >>> obj.foo.   
-00002590: 2027 6261 7227 0a0a 6578 706c 6963 6974   'bar'..explicit
-000025a0: 5f68 6173 680a 5e5e 5e5e 5e5e 5e5e 5e5e  _hash.^^^^^^^^^^
-000025b0: 5e5e 5e0a 4d65 7461 636c 6173 7320 7468  ^^^.Metaclass th
-000025c0: 6174 2066 6f72 6365 7320 605f 5f68 6173  at forces `__has
-000025d0: 685f 5f60 2074 6f20 6265 2064 6563 6c61  h__` to be decla
-000025e0: 7265 6420 7768 656e 6576 6572 2060 5f5f  red whenever `__
-000025f0: 6571 5f5f 6020 6973 2064 6563 6c61 7265  eq__` is declare
-00002600: 642e 0a0a 2e2e 2063 6f64 653a 3a20 7079  d..... code:: py
-00002610: 7468 6f6e 0a0a 2020 2020 3e3e 3e20 6672  thon..    >>> fr
-00002620: 6f6d 2073 6978 2069 6d70 6f72 7420 7769  om six import wi
-00002630: 7468 5f6d 6574 6163 6c61 7373 0a20 2020  th_metaclass.   
-00002640: 203e 3e3e 2066 726f 6d20 6261 7369 6363   >>> from basicc
-00002650: 6f2e 6578 706c 6963 6974 5f68 6173 6820  o.explicit_hash 
-00002660: 696d 706f 7274 2045 7870 6c69 6369 7448  import ExplicitH
-00002670: 6173 684d 6574 610a 2020 2020 3e3e 3e20  ashMeta.    >>> 
-00002680: 636c 6173 7320 4173 7365 7428 7769 7468  class Asset(with
-00002690: 5f6d 6574 6163 6c61 7373 2845 7870 6c69  _metaclass(Expli
-000026a0: 6369 7448 6173 684d 6574 612c 206f 626a  citHashMeta, obj
-000026b0: 6563 7429 293a 0a20 2020 202e 2e2e 2020  ect)):.    ...  
-000026c0: 2020 2064 6566 205f 5f65 715f 5f28 7365     def __eq__(se
-000026d0: 6c66 2c20 6f74 6865 7229 3a0a 2020 2020  lf, other):.    
-000026e0: 2e2e 2e20 2020 2020 2020 2020 7061 7373  ...         pass
-000026f0: 0a20 2020 202e 2e2e 0a20 2020 2054 7261  .    ....    Tra
-00002700: 6365 6261 636b 2028 6d6f 7374 2072 6563  ceback (most rec
-00002710: 656e 7420 6361 6c6c 206c 6173 7429 3a0a  ent call last):.
-00002720: 2020 2020 5479 7065 4572 726f 723a 2064      TypeError: d
-00002730: 6563 6c61 7265 6420 275f 5f65 715f 5f27  eclared '__eq__'
-00002740: 2069 6e20 2741 7373 6574 2720 6275 7420   in 'Asset' but 
-00002750: 6469 646e 2774 2064 6563 6c61 7265 2027  didn't declare '
-00002760: 5f5f 6861 7368 5f5f 270a 0a66 6162 7269  __hash__'..fabri
-00002770: 6361 7465 5f76 616c 7565 0a5e 5e5e 5e5e  cate_value.^^^^^
-00002780: 5e5e 5e5e 5e5e 5e5e 5e5e 0a52 756e 2061  ^^^^^^^^^^.Run a
-00002790: 2076 616c 7565 2074 6872 6f75 6768 2061   value through a
-000027a0: 2063 616c 6c61 626c 6520 6661 6374 6f72   callable factor
-000027b0: 7920 286f 7220 4e6f 6e65 292e 0a0a 2e2e  y (or None).....
-000027c0: 2063 6f64 653a 3a20 7079 7468 6f6e 0a0a   code:: python..
-000027d0: 2020 2020 3e3e 3e20 6672 6f6d 2062 6173      >>> from bas
-000027e0: 6963 636f 2e66 6162 7269 6361 7465 5f76  icco.fabricate_v
-000027f0: 616c 7565 2069 6d70 6f72 7420 6661 6272  alue import fabr
-00002800: 6963 6174 655f 7661 6c75 650a 2020 2020  icate_value.    
-00002810: 3e3e 3e20 6661 6272 6963 6174 655f 7661  >>> fabricate_va
-00002820: 6c75 6528 4e6f 6e65 2c20 3329 2020 2320  lue(None, 3)  # 
-00002830: 6e6f 2066 6163 746f 7279 2c20 7661 6c75  no factory, valu
-00002840: 6520 7061 7373 7468 726f 7567 680a 2020  e passthrough.  
-00002850: 2020 330a 2020 2020 3e3e 3e20 6661 6272    3.    >>> fabr
-00002860: 6963 6174 655f 7661 6c75 6528 7374 722c  icate_value(str,
-00002870: 2033 2920 2023 2063 616c 6c61 626c 6520   3)  # callable 
-00002880: 6661 6374 6f72 790a 2020 2020 2733 270a  factory.    '3'.
-00002890: 2020 2020 3e3e 3e20 6661 6272 6963 6174      >>> fabricat
-000028a0: 655f 7661 6c75 6528 2273 7472 222c 2033  e_value("str", 3
-000028b0: 2920 2023 2075 7365 2061 6e20 696d 706f  )  # use an impo
-000028c0: 7274 2070 6174 680a 2020 2020 2733 270a  rt path.    '3'.
-000028d0: 2020 2020 3e3e 3e20 6661 6272 6963 6174      >>> fabricat
-000028e0: 655f 7661 6c75 6528 696e 7429 2020 2320  e_value(int)  # 
-000028f0: 6e6f 2069 6e70 7574 2076 616c 7565 2c20  no input value, 
-00002900: 6a75 7374 2074 6865 2066 6163 746f 7279  just the factory
-00002910: 2069 7473 656c 660a 2020 2020 300a 0a67   itself.    0..g
-00002920: 6574 5f6d 726f 0a5e 5e5e 5e5e 5e5e 0a47  et_mro.^^^^^^^.G
-00002930: 6574 2063 6f6e 7369 7374 656e 7420 4d52  et consistent MR
-00002940: 4f20 616d 6f6e 6773 7420 6469 6666 6572  O amongst differ
-00002950: 656e 7420 7079 7468 6f6e 2076 6572 7369  ent python versi
-00002960: 6f6e 732e 2054 6869 7320 776f 726b 7320  ons. This works 
-00002970: 6576 656e 2077 6974 6820 6765 6e65 7269  even with generi
-00002980: 6320 636c 6173 7365 7320 696e 2050 7974  c classes in Pyt
-00002990: 686f 6e20 322e 372e 0a0a 2e2e 2063 6f64  hon 2.7..... cod
-000029a0: 653a 3a20 7079 7468 6f6e 0a0a 2020 2020  e:: python..    
-000029b0: 3e3e 3e20 6672 6f6d 2073 6978 2069 6d70  >>> from six imp
-000029c0: 6f72 7420 7769 7468 5f6d 6574 6163 6c61  ort with_metacla
-000029d0: 7373 0a20 2020 203e 3e3e 2066 726f 6d20  ss.    >>> from 
-000029e0: 7469 7070 6f20 696d 706f 7274 2047 656e  tippo import Gen
-000029f0: 6572 6963 2c20 5479 7065 5661 720a 2020  eric, TypeVar.  
-00002a00: 2020 3e3e 3e20 6672 6f6d 2062 6173 6963    >>> from basic
-00002a10: 636f 2e67 6574 5f6d 726f 2069 6d70 6f72  co.get_mro impor
-00002a20: 7420 6765 745f 6d72 6f0a 2020 2020 3e3e  t get_mro.    >>
-00002a30: 3e20 5420 3d20 5479 7065 5661 7228 2254  > T = TypeVar("T
-00002a40: 2229 0a20 2020 203e 3e3e 2063 6c61 7373  ").    >>> class
-00002a50: 204d 7947 656e 6572 6963 2847 656e 6572   MyGeneric(Gener
-00002a60: 6963 5b54 5d29 3a0a 2020 2020 2e2e 2e20  ic[T]):.    ... 
-00002a70: 2020 2020 7061 7373 0a20 2020 202e 2e2e      pass.    ...
-00002a80: 0a20 2020 203e 3e3e 2063 6c61 7373 2053  .    >>> class S
-00002a90: 7562 436c 6173 7328 4d79 4765 6e65 7269  ubClass(MyGeneri
-00002aa0: 635b 545d 293a 0a20 2020 202e 2e2e 2020  c[T]):.    ...  
-00002ab0: 2020 2070 6173 730a 2020 2020 2e2e 2e0a     pass.    ....
-00002ac0: 2020 2020 3e3e 3e20 636c 6173 7320 4d69      >>> class Mi
-00002ad0: 7865 6428 5375 6243 6c61 7373 5b54 5d2c  xed(SubClass[T],
-00002ae0: 204d 7947 656e 6572 6963 5b54 5d29 3a0a   MyGeneric[T]):.
-00002af0: 2020 2020 2e2e 2e20 2020 2020 7061 7373      ...     pass
-00002b00: 0a20 2020 202e 2e2e 0a20 2020 203e 3e3e  .    ....    >>>
-00002b10: 205b 632e 5f5f 6e61 6d65 5f5f 2066 6f72   [c.__name__ for
-00002b20: 2063 2069 6e20 6765 745f 6d72 6f28 4d69   c in get_mro(Mi
-00002b30: 7865 6429 5d0a 2020 2020 5b27 4d69 7865  xed)].    ['Mixe
-00002b40: 6427 2c20 2753 7562 436c 6173 7327 2c20  d', 'SubClass', 
-00002b50: 274d 7947 656e 6572 6963 272c 2027 4765  'MyGeneric', 'Ge
-00002b60: 6e65 7269 6327 2c20 276f 626a 6563 7427  neric', 'object'
-00002b70: 5d0a 0a68 6173 685f 6361 6368 655f 7772  ]..hash_cache_wr
-00002b80: 6170 7065 720a 5e5e 5e5e 5e5e 5e5e 5e5e  apper.^^^^^^^^^^
-00002b90: 5e5e 5e5e 5e5e 5e5e 0a41 6e20 696e 7465  ^^^^^^^^.An inte
-00002ba0: 6765 7220 7375 6263 6c61 7373 2074 6861  ger subclass tha
-00002bb0: 7420 7069 636b 6c65 732f 636f 7069 6573  t pickles/copies
-00002bc0: 2061 7320 4e6f 6e65 2e20 5468 6973 2063   as None. This c
-00002bd0: 616e 2062 6520 7573 6564 2074 6f20 6176  an be used to av
-00002be0: 6f69 6420 7365 7269 616c 697a 696e 6720  oid serializing 
-00002bf0: 6120 6361 6368 6564 2068 6173 6820 7661  a cached hash va
-00002c00: 6c75 652e 0a0a 2e2e 2063 6f64 653a 3a20  lue..... code:: 
-00002c10: 7079 7468 6f6e 0a0a 2020 2020 3e3e 3e20  python..    >>> 
-00002c20: 6672 6f6d 2063 6f70 7920 696d 706f 7274  from copy import
-00002c30: 2063 6f70 790a 2020 2020 3e3e 3e20 6672   copy.    >>> fr
-00002c40: 6f6d 2062 6173 6963 636f 2e68 6173 685f  om basicco.hash_
-00002c50: 6361 6368 655f 7772 6170 7065 7220 696d  cache_wrapper im
-00002c60: 706f 7274 2048 6173 6843 6163 6865 5772  port HashCacheWr
-00002c70: 6170 7065 720a 2020 2020 3e3e 3e20 6861  apper.    >>> ha
-00002c80: 7368 5f63 6163 6865 203d 2048 6173 6843  sh_cache = HashC
-00002c90: 6163 6865 5772 6170 7065 7228 3132 3334  acheWrapper(1234
-00002ca0: 3529 0a20 2020 203e 3e3e 2070 7269 6e74  5).    >>> print
-00002cb0: 2868 6173 685f 6361 6368 6529 0a20 2020  (hash_cache).   
-00002cc0: 2031 3233 3435 0a20 2020 203e 3e3e 2070   12345.    >>> p
-00002cd0: 7269 6e74 2863 6f70 7928 6861 7368 5f63  rint(copy(hash_c
-00002ce0: 6163 6865 2929 0a20 2020 204e 6f6e 650a  ache)).    None.
-00002cf0: 0a69 6d70 6c69 6369 745f 6861 7368 0a5e  .implicit_hash.^
-00002d00: 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e 0a4d 6574  ^^^^^^^^^^^^.Met
-00002d10: 6163 6c61 7373 2074 6861 7420 666f 7263  aclass that forc
-00002d20: 6573 2060 5f5f 6861 7368 5f5f 6020 746f  es `__hash__` to
-00002d30: 204e 6f6e 6520 7768 656e 2060 5f5f 6571   None when `__eq
-00002d40: 5f5f 6020 6973 2064 6563 6c61 7265 642e  __` is declared.
-00002d50: 0a54 6869 7320 6973 2061 2062 6163 6b70  .This is a backp
-00002d60: 6f72 7420 6f66 2074 6865 2064 6566 6175  ort of the defau
-00002d70: 6c74 2062 6568 6176 696f 7220 696e 2050  lt behavior in P
-00002d80: 7974 686f 6e20 332e 0a0a 2e2e 2063 6f64  ython 3..... cod
-00002d90: 653a 3a20 7079 7468 6f6e 0a0a 2020 2020  e:: python..    
-00002da0: 3e3e 3e20 6672 6f6d 2073 6978 2069 6d70  >>> from six imp
-00002db0: 6f72 7420 7769 7468 5f6d 6574 6163 6c61  ort with_metacla
-00002dc0: 7373 0a20 2020 203e 3e3e 2066 726f 6d20  ss.    >>> from 
-00002dd0: 6261 7369 6363 6f2e 696d 706c 6963 6974  basicco.implicit
-00002de0: 5f68 6173 6820 696d 706f 7274 2049 6d70  _hash import Imp
-00002df0: 6c69 6369 7448 6173 684d 6574 610a 2020  licitHashMeta.  
-00002e00: 2020 3e3e 3e20 636c 6173 7320 4173 7365    >>> class Asse
-00002e10: 7428 7769 7468 5f6d 6574 6163 6c61 7373  t(with_metaclass
-00002e20: 2849 6d70 6c69 6369 7448 6173 684d 6574  (ImplicitHashMet
-00002e30: 612c 206f 626a 6563 7429 293a 0a20 2020  a, object)):.   
-00002e40: 202e 2e2e 2020 2020 2064 6566 205f 5f65   ...     def __e
-00002e50: 715f 5f28 7365 6c66 2c20 6f74 6865 7229  q__(self, other)
-00002e60: 3a0a 2020 2020 2e2e 2e20 2020 2020 2020  :.    ...       
-00002e70: 2020 7061 7373 0a20 2020 202e 2e2e 0a20    pass.    .... 
-00002e80: 2020 203e 3e3e 2041 7373 6574 2e5f 5f68     >>> Asset.__h
-00002e90: 6173 685f 5f20 6973 204e 6f6e 650a 2020  ash__ is None.  
-00002ea0: 2020 5472 7565 0a0a 696d 706f 7274 5f70    True..import_p
-00002eb0: 6174 680a 5e5e 5e5e 5e5e 5e5e 5e5e 5e0a  ath.^^^^^^^^^^^.
-00002ec0: 4765 6e65 7261 7465 2069 6d70 6f72 7461  Generate importa
-00002ed0: 626c 6520 646f 7420 7061 7468 7320 616e  ble dot paths an
-00002ee0: 6420 696d 706f 7274 2066 726f 6d20 7468  d import from th
-00002ef0: 656d 2e0a 0a2e 2e20 636f 6465 3a3a 2070  em..... code:: p
-00002f00: 7974 686f 6e0a 0a20 2020 203e 3e3e 2069  ython..    >>> i
-00002f10: 6d70 6f72 7420 6974 6572 746f 6f6c 730a  mport itertools.
-00002f20: 2020 2020 3e3e 3e20 6672 6f6d 2062 6173      >>> from bas
-00002f30: 6963 636f 2e69 6d70 6f72 745f 7061 7468  icco.import_path
-00002f40: 2069 6d70 6f72 7420 6765 745f 7061 7468   import get_path
-00002f50: 2c20 696d 706f 7274 5f70 6174 680a 2020  , import_path.  
-00002f60: 2020 3e3e 3e20 6765 745f 7061 7468 2869    >>> get_path(i
-00002f70: 7465 7274 6f6f 6c73 2e63 6861 696e 290a  tertools.chain).
-00002f80: 2020 2020 2769 7465 7274 6f6f 6c73 2e63      'itertools.c
-00002f90: 6861 696e 270a 2020 2020 3e3e 3e20 696d  hain'.    >>> im
-00002fa0: 706f 7274 5f70 6174 6828 2269 7465 7274  port_path("itert
-00002fb0: 6f6f 6c73 2e63 6861 696e 2229 0a20 2020  ools.chain").   
-00002fc0: 203c 2e2e 2e20 2769 7465 7274 6f6f 6c73   <... 'itertools
-00002fd0: 2e63 6861 696e 273e 0a0a 2e2e 2063 6f64  .chain'>.... cod
-00002fe0: 653a 3a20 7079 7468 6f6e 0a0a 2020 2020  e:: python..    
-00002ff0: 3e3e 3e20 6672 6f6d 2062 6173 6963 636f  >>> from basicco
-00003000: 2e69 6d70 6f72 745f 7061 7468 2069 6d70  .import_path imp
-00003010: 6f72 7420 6578 7472 6163 745f 6765 6e65  ort extract_gene
-00003020: 7269 635f 7061 7468 730a 2020 2020 3e3e  ric_paths.    >>
-00003030: 3e20 6578 7472 6163 745f 6765 6e65 7269  > extract_generi
-00003040: 635f 7061 7468 7328 2254 7570 6c65 5b69  c_paths("Tuple[i
-00003050: 6e74 2c20 7374 725d 2229 0a20 2020 2028  nt, str]").    (
-00003060: 2754 7570 6c65 272c 2028 2769 6e74 272c  'Tuple', ('int',
-00003070: 2027 7374 7227 2929 0a0a 696e 6974 5f73   'str'))..init_s
-00003080: 7562 636c 6173 730a 5e5e 5e5e 5e5e 5e5e  ubclass.^^^^^^^^
-00003090: 5e5e 5e5e 5e0a 4261 636b 706f 7274 206f  ^^^^^.Backport o
-000030a0: 6620 7468 6520 6675 6e63 7469 6f6e 616c  f the functional
-000030b0: 6974 7920 6f66 2060 5f5f 696e 6974 5f73  ity of `__init_s
-000030c0: 7562 636c 6173 735f 5f60 2066 726f 6d20  ubclass__` from 
-000030d0: 5045 5020 3438 3720 746f 2050 7974 686f  PEP 487 to Pytho
-000030e0: 6e20 322e 372e 0a54 6869 7320 776f 726b  n 2.7..This work
-000030f0: 7320 666f 7220 626f 7468 2050 7974 686f  s for both Pytho
-00003100: 6e20 3220 2875 7369 6e67 2060 5f5f 6b77  n 2 (using `__kw
-00003110: 6172 6773 5f5f 6029 2061 6e64 2033 2028  args__`) and 3 (
-00003120: 7573 696e 6720 7468 6520 6e65 7720 636c  using the new cl
-00003130: 6173 7320 7061 7261 6d65 7465 7273 292e  ass parameters).
-00003140: 0a0a 2e2e 2063 6f64 653a 3a20 7079 7468  .... code:: pyth
-00003150: 6f6e 0a0a 2020 2020 3e3e 3e20 6672 6f6d  on..    >>> from
-00003160: 2062 6173 6963 636f 2e69 6e69 745f 7375   basicco.init_su
-00003170: 6263 6c61 7373 2069 6d70 6f72 7420 496e  bclass import In
-00003180: 6974 5375 6263 6c61 7373 0a20 2020 203e  itSubclass.    >
-00003190: 3e3e 2063 6c61 7373 2046 6f6f 2849 6e69  >> class Foo(Ini
-000031a0: 7453 7562 636c 6173 7329 3a0a 2020 2020  tSubclass):.    
-000031b0: 2e2e 2e20 2020 2020 6465 6620 5f5f 696e  ...     def __in
-000031c0: 6974 5f73 7562 636c 6173 735f 5f28 636c  it_subclass__(cl
-000031d0: 732c 2066 6f6f 3d4e 6f6e 652c 202a 2a6b  s, foo=None, **k
-000031e0: 7761 7267 7329 3a0a 2020 2020 2e2e 2e20  wargs):.    ... 
-000031f0: 2020 2020 2020 2020 636c 732e 666f 6f20          cls.foo 
-00003200: 3d20 666f 6f0a 2020 2020 2e2e 2e0a 2020  = foo.    ....  
-00003210: 2020 3e3e 3e20 636c 6173 7320 4261 7228    >>> class Bar(
-00003220: 466f 6f29 3a0a 2020 2020 2e2e 2e20 2020  Foo):.    ...   
-00003230: 2020 5f5f 6b77 6172 6773 5f5f 203d 207b    __kwargs__ = {
-00003240: 2266 6f6f 223a 2022 6261 7222 7d20 2023  "foo": "bar"}  #
-00003250: 2079 6f75 2063 616e 2073 7065 6369 6679   you can specify
-00003260: 2063 6c73 206b 7761 7267 7320 6f6e 2070   cls kwargs on p
-00003270: 7932 206c 696b 6520 7468 6973 0a20 2020  y2 like this.   
-00003280: 202e 2e2e 0a20 2020 203e 3e3e 2042 6172   ....    >>> Bar
-00003290: 2e66 6f6f 0a20 2020 2027 6261 7227 0a0a  .foo.    'bar'..
-000032a0: 6c6f 636b 6564 5f63 6c61 7373 0a5e 5e5e  locked_class.^^^
-000032b0: 5e5e 5e5e 5e5e 5e5e 5e5e 0a50 7265 7665  ^^^^^^^^^^.Preve
-000032c0: 6e74 7320 6368 616e 6769 6e67 2070 7562  nts changing pub
-000032d0: 6c69 6320 636c 6173 7320 6174 7472 6962  lic class attrib
-000032e0: 7574 6573 2e0a 0a2e 2e20 636f 6465 3a3a  utes..... code::
-000032f0: 2070 7974 686f 6e0a 0a20 2020 203e 3e3e   python..    >>>
-00003300: 2066 726f 6d20 7369 7820 696d 706f 7274   from six import
-00003310: 2077 6974 685f 6d65 7461 636c 6173 730a   with_metaclass.
-00003320: 2020 2020 3e3e 3e20 6672 6f6d 2062 6173      >>> from bas
-00003330: 6963 636f 2e6c 6f63 6b65 645f 636c 6173  icco.locked_clas
-00003340: 7320 696d 706f 7274 204c 6f63 6b65 6443  s import LockedC
-00003350: 6c61 7373 4d65 7461 0a20 2020 203e 3e3e  lassMeta.    >>>
-00003360: 2063 6c61 7373 2046 6f6f 2877 6974 685f   class Foo(with_
-00003370: 6d65 7461 636c 6173 7328 4c6f 636b 6564  metaclass(Locked
-00003380: 436c 6173 734d 6574 612c 206f 626a 6563  ClassMeta, objec
-00003390: 7429 293a 0a20 2020 202e 2e2e 2020 2020  t)):.    ...    
-000033a0: 2070 6173 730a 2020 2020 2e2e 2e0a 2020   pass.    ....  
-000033b0: 2020 3e3e 3e20 466f 6f2e 6261 7220 3d20    >>> Foo.bar = 
-000033c0: 2262 6172 220a 2020 2020 5472 6163 6562  "bar".    Traceb
-000033d0: 6163 6b20 286d 6f73 7420 7265 6365 6e74  ack (most recent
-000033e0: 2063 616c 6c20 6c61 7374 293a 0a20 2020   call last):.   
-000033f0: 2041 7474 7269 6275 7465 4572 726f 723a   AttributeError:
-00003400: 2063 616e 2774 2073 6574 2072 6561 642d   can't set read-
-00003410: 6f6e 6c79 2063 6c61 7373 2061 7474 7269  only class attri
-00003420: 6275 7465 2027 6261 7227 0a0a 6d61 6e67  bute 'bar'..mang
-00003430: 6c69 6e67 0a5e 5e5e 5e5e 5e5e 5e0a 4675  ling.^^^^^^^^.Fu
-00003440: 6e63 7469 6f6e 7320 746f 206d 616e 676c  nctions to mangl
-00003450: 652f 756e 6d61 6e67 6c65 2f65 7874 7261  e/unmangle/extra
-00003460: 6374 2070 7269 7661 7465 206e 616d 6573  ct private names
-00003470: 2e0a 0a2e 2e20 636f 6465 3a3a 2070 7974  ..... code:: pyt
-00003480: 686f 6e0a 0a20 2020 203e 3e3e 2066 726f  hon..    >>> fro
-00003490: 6d20 6261 7369 6363 6f2e 6d61 6e67 6c69  m basicco.mangli
-000034a0: 6e67 2069 6d70 6f72 7420 6d61 6e67 6c65  ng import mangle
-000034b0: 2c20 756e 6d61 6e67 6c65 2c20 6578 7472  , unmangle, extr
-000034c0: 6163 740a 2020 2020 3e3e 3e20 6d61 6e67  act.    >>> mang
-000034d0: 6c65 2822 5f5f 6d65 6d62 6572 222c 2022  le("__member", "
-000034e0: 466f 6f22 290a 2020 2020 275f 466f 6f5f  Foo").    '_Foo_
-000034f0: 5f6d 656d 6265 7227 0a20 2020 203e 3e3e  _member'.    >>>
-00003500: 2075 6e6d 616e 676c 6528 225f 466f 6f5f   unmangle("_Foo_
-00003510: 5f6d 656d 6265 7222 2c20 2246 6f6f 2229  _member", "Foo")
-00003520: 0a20 2020 2027 5f5f 6d65 6d62 6572 270a  .    '__member'.
-00003530: 2020 2020 3e3e 3e20 6578 7472 6163 7428      >>> extract(
-00003540: 225f 466f 6f5f 5f6d 656d 6265 7222 290a  "_Foo__member").
-00003550: 2020 2020 2827 5f5f 6d65 6d62 6572 272c      ('__member',
-00003560: 2027 466f 6f27 290a 0a6d 6170 7069 6e67   'Foo')..mapping
-00003570: 5f70 726f 7879 0a5e 5e5e 5e5e 5e5e 5e5e  _proxy.^^^^^^^^^
-00003580: 5e5e 5e5e 0a4d 6170 7069 6e67 2050 726f  ^^^^.Mapping Pro
-00003590: 7879 2074 7970 6520 2872 6561 642d 6f6e  xy type (read-on
-000035a0: 6c79 2920 666f 7220 6f6c 6465 7220 5079  ly) for older Py
-000035b0: 7468 6f6e 2076 6572 7369 6f6e 732e 0a0a  thon versions...
-000035c0: 2e2e 2063 6f64 653a 3a20 7079 7468 6f6e  .. code:: python
-000035d0: 0a0a 2020 2020 3e3e 3e20 6672 6f6d 2062  ..    >>> from b
-000035e0: 6173 6963 636f 2e6d 6170 7069 6e67 5f70  asicco.mapping_p
-000035f0: 726f 7879 2069 6d70 6f72 7420 4d61 7070  roxy import Mapp
-00003600: 696e 6750 726f 7879 5479 7065 0a20 2020  ingProxyType.   
-00003610: 203e 3e3e 2069 6e74 6572 6e61 6c5f 6469   >>> internal_di
-00003620: 6374 203d 207b 2266 6f6f 223a 2022 6261  ct = {"foo": "ba
-00003630: 7222 7d0a 2020 2020 3e3e 3e20 7072 6f78  r"}.    >>> prox
-00003640: 795f 6469 6374 203d 204d 6170 7069 6e67  y_dict = Mapping
-00003650: 5072 6f78 7954 7970 6528 696e 7465 726e  ProxyType(intern
-00003660: 616c 5f64 6963 7429 0a20 2020 203e 3e3e  al_dict).    >>>
-00003670: 2070 726f 7879 5f64 6963 745b 2266 6f6f   proxy_dict["foo
-00003680: 225d 0a20 2020 2027 6261 7227 0a0a 6e61  "].    'bar'..na
-00003690: 6d65 645f 7475 706c 650a 5e5e 5e5e 5e5e  med_tuple.^^^^^^
-000036a0: 5e5e 5e5e 5e0a 4e61 6d65 6420 5475 706c  ^^^^^.Named Tupl
-000036b0: 6520 7574 696c 6974 6965 732e 0a0a 4578  e utilities...Ex
-000036c0: 616d 706c 6520 6f66 2060 6465 6661 756c  ample of `defaul
-000036d0: 7473 6020 6465 636f 7261 746f 722f 6675  ts` decorator/fu
-000036e0: 6e63 7469 6f6e 2074 6f20 7365 7420 6120  nction to set a 
-000036f0: 4e61 6d65 6420 5475 706c 6527 7320 6465  Named Tuple's de
-00003700: 6661 756c 7420 7661 6c75 6573 3a0a 0a2e  fault values:...
-00003710: 2e20 636f 6465 3a3a 2070 7974 686f 6e0a  . code:: python.
-00003720: 0a20 2020 203e 3e3e 2066 726f 6d20 636f  .    >>> from co
-00003730: 6c6c 6563 7469 6f6e 7320 696d 706f 7274  llections import
-00003740: 206e 616d 6564 7475 706c 650a 2020 2020   namedtuple.    
-00003750: 3e3e 3e20 6672 6f6d 2062 6173 6963 636f  >>> from basicco
-00003760: 2e6e 616d 6564 5f74 7570 6c65 2069 6d70  .named_tuple imp
-00003770: 6f72 7420 6465 6661 756c 7473 0a20 2020  ort defaults.   
-00003780: 203e 3e3e 2050 6f69 6e74 203d 2064 6566   >>> Point = def
-00003790: 6175 6c74 7328 6e61 6d65 3d22 666f 6f22  aults(name="foo"
-000037a0: 2928 6e61 6d65 6474 7570 6c65 2822 506f  )(namedtuple("Po
-000037b0: 696e 7422 2c20 2822 7822 2c20 2279 222c  int", ("x", "y",
-000037c0: 2022 6e61 6d65 2229 2929 0a20 2020 203e   "name"))).    >
-000037d0: 3e3e 2050 6f69 6e74 2831 2c20 3229 0a20  >> Point(1, 2). 
-000037e0: 2020 2050 6f69 6e74 2878 3d31 2c20 793d     Point(x=1, y=
-000037f0: 322c 206e 616d 653d 2766 6f6f 2729 0a0a  2, name='foo')..
-00003800: 6e61 6d65 7370 6163 650a 5e5e 5e5e 5e5e  namespace.^^^^^^
-00003810: 5e5e 5e0a 5772 6170 7320 6120 6469 6374  ^^^.Wraps a dict
-00003820: 696f 6e61 7279 2f6d 6170 7069 6e67 2061  ionary/mapping a
-00003830: 6e64 2070 726f 7669 6465 7320 6174 7472  nd provides attr
-00003840: 6962 7574 652d 7374 796c 6520 6163 6365  ibute-style acce
-00003850: 7373 2074 6f20 6974 2e0a 0a2e 2e20 636f  ss to it..... co
-00003860: 6465 3a3a 2070 7974 686f 6e0a 0a20 2020  de:: python..   
-00003870: 203e 3e3e 2066 726f 6d20 6261 7369 6363   >>> from basicc
-00003880: 6f2e 6e61 6d65 7370 6163 6520 696d 706f  o.namespace impo
-00003890: 7274 204e 616d 6573 7061 6365 0a20 2020  rt Namespace.   
-000038a0: 203e 3e3e 206e 7320 3d20 4e61 6d65 7370   >>> ns = Namesp
-000038b0: 6163 6528 7b22 6261 7222 3a20 2266 6f6f  ace({"bar": "foo
-000038c0: 227d 290a 2020 2020 3e3e 3e20 6e73 2e62  "}).    >>> ns.b
-000038d0: 6172 0a20 2020 2027 666f 6f27 0a0a 2e2e  ar.    'foo'....
-000038e0: 2063 6f64 653a 3a20 7079 7468 6f6e 0a0a   code:: python..
-000038f0: 2020 2020 3e3e 3e20 6672 6f6d 2062 6173      >>> from bas
-00003900: 6963 636f 2e6e 616d 6573 7061 6365 2069  icco.namespace i
-00003910: 6d70 6f72 7420 4d75 7461 626c 654e 616d  mport MutableNam
-00003920: 6573 7061 6365 0a20 2020 203e 3e3e 206e  espace.    >>> n
-00003930: 7320 3d20 4d75 7461 626c 654e 616d 6573  s = MutableNames
-00003940: 7061 6365 287b 2262 6172 223a 2022 666f  pace({"bar": "fo
-00003950: 6f22 7d29 0a20 2020 203e 3e3e 206e 732e  o"}).    >>> ns.
-00003960: 666f 6f20 3d20 2262 6172 220a 2020 2020  foo = "bar".    
-00003970: 3e3e 3e20 6e73 2e66 6f6f 0a20 2020 2027  >>> ns.foo.    '
-00003980: 6261 7227 0a20 2020 203e 3e3e 206e 732e  bar'.    >>> ns.
-00003990: 6261 720a 2020 2020 2766 6f6f 270a 0a41  bar.    'foo'..A
-000039a0: 6c73 6f20 7072 6f76 6964 6573 2061 2060  lso provides a `
-000039b0: 4e61 6d65 7370 6163 6564 4d65 7461 6020  NamespacedMeta` 
-000039c0: 6d65 7461 636c 6173 7320 7468 6174 2061  metaclass that a
-000039d0: 6464 7320 6120 605f 5f6e 616d 6573 7061  dds a `__namespa
-000039e0: 6365 6020 7072 6f74 6563 7465 6420 636c  ce` protected cl
-000039f0: 6173 7320 6174 7472 6962 7574 6520 7468  ass attribute th
-00003a00: 6174 2069 7320 756e 6971 7565 2074 6f20  at is unique to 
-00003a10: 6561 6368 0a63 6c61 7373 2e0a 0a2e 2e20  each.class..... 
-00003a20: 636f 6465 3a3a 2070 7974 686f 6e0a 0a20  code:: python.. 
-00003a30: 2020 203e 3e3e 2066 726f 6d20 7369 7820     >>> from six 
-00003a40: 696d 706f 7274 2077 6974 685f 6d65 7461  import with_meta
-00003a50: 636c 6173 730a 2020 2020 3e3e 3e20 6672  class.    >>> fr
-00003a60: 6f6d 2062 6173 6963 636f 2e6e 616d 6573  om basicco.names
-00003a70: 7061 6365 2069 6d70 6f72 7420 4e61 6d65  pace import Name
-00003a80: 7370 6163 6564 4d65 7461 0a20 2020 203e  spacedMeta.    >
-00003a90: 3e3e 2063 6c61 7373 2041 7373 6574 2877  >> class Asset(w
-00003aa0: 6974 685f 6d65 7461 636c 6173 7328 4e61  ith_metaclass(Na
-00003ab0: 6d65 7370 6163 6564 4d65 7461 2c20 6f62  mespacedMeta, ob
-00003ac0: 6a65 6374 2929 3a0a 2020 2020 2e2e 2e20  ject)):.    ... 
-00003ad0: 2020 2020 4063 6c61 7373 6d65 7468 6f64      @classmethod
-00003ae0: 0a20 2020 202e 2e2e 2020 2020 2064 6566  .    ...     def
-00003af0: 2073 6574 5f63 6c61 7373 5f76 616c 7565   set_class_value
-00003b00: 2863 6c73 2c20 7661 6c75 6529 3a0a 2020  (cls, value):.  
-00003b10: 2020 2e2e 2e20 2020 2020 2020 2020 636c    ...         cl
-00003b20: 732e 5f5f 6e61 6d65 7370 6163 652e 7661  s.__namespace.va
-00003b30: 6c75 6520 3d20 7661 6c75 650a 2020 2020  lue = value.    
-00003b40: 2e2e 2e0a 2020 2020 2e2e 2e20 2020 2020  ....    ...     
-00003b50: 4063 6c61 7373 6d65 7468 6f64 0a20 2020  @classmethod.   
-00003b60: 202e 2e2e 2020 2020 2064 6566 2067 6574   ...     def get
-00003b70: 5f63 6c61 7373 5f76 616c 7565 2863 6c73  _class_value(cls
-00003b80: 293a 0a20 2020 202e 2e2e 2020 2020 2020  ):.    ...      
-00003b90: 2020 2072 6574 7572 6e20 636c 732e 5f5f     return cls.__
-00003ba0: 6e61 6d65 7370 6163 652e 7661 6c75 650a  namespace.value.
-00003bb0: 2020 2020 2e2e 2e0a 2020 2020 3e3e 3e20      ....    >>> 
-00003bc0: 4173 7365 742e 7365 745f 636c 6173 735f  Asset.set_class_
-00003bd0: 7661 6c75 6528 2266 6f6f 6261 7222 290a  value("foobar").
-00003be0: 2020 2020 3e3e 3e20 4173 7365 742e 6765      >>> Asset.ge
-00003bf0: 745f 636c 6173 735f 7661 6c75 6528 290a  t_class_value().
-00003c00: 2020 2020 2766 6f6f 6261 7227 0a0a 6f62      'foobar'..ob
-00003c10: 6a5f 7374 6174 650a 5e5e 5e5e 5e5e 5e5e  j_state.^^^^^^^^
-00003c20: 5e0a 4765 742f 7570 6461 7465 2074 6865  ^.Get/update the
-00003c30: 2073 7461 7465 206f 6620 616e 206f 626a   state of an obj
-00003c40: 6563 742c 2073 6c6f 7474 6564 206f 7220  ect, slotted or 
-00003c50: 6e6f 7420 2877 6f72 6b73 2065 7665 6e20  not (works even 
-00003c60: 696e 2050 7974 686f 6e20 322e 3729 2e0a  in Python 2.7)..
-00003c70: 0a2e 2e20 636f 6465 3a3a 2070 7974 686f  ... code:: pytho
-00003c80: 6e0a 0a20 2020 203e 3e3e 2066 726f 6d20  n..    >>> from 
-00003c90: 6261 7369 6363 6f2e 6f62 6a5f 7374 6174  basicco.obj_stat
-00003ca0: 6520 696d 706f 7274 2067 6574 5f73 7461  e import get_sta
-00003cb0: 7465 0a20 2020 203e 3e3e 2063 6c61 7373  te.    >>> class
-00003cc0: 2053 6c6f 7474 6564 286f 626a 6563 7429   Slotted(object)
-00003cd0: 3a0a 2020 2020 2e2e 2e20 2020 2020 5f5f  :.    ...     __
-00003ce0: 736c 6f74 735f 5f20 3d20 2822 666f 6f22  slots__ = ("foo"
-00003cf0: 2c20 2262 6172 2229 0a20 2020 202e 2e2e  , "bar").    ...
-00003d00: 2020 2020 2064 6566 205f 5f69 6e69 745f       def __init_
-00003d10: 5f28 7365 6c66 2c20 666f 6f2c 2062 6172  _(self, foo, bar
-00003d20: 293a 0a20 2020 202e 2e2e 2020 2020 2020  ):.    ...      
-00003d30: 2020 2073 656c 662e 666f 6f20 3d20 666f     self.foo = fo
-00003d40: 6f0a 2020 2020 2e2e 2e20 2020 2020 2020  o.    ...       
-00003d50: 2020 7365 6c66 2e62 6172 203d 2062 6172    self.bar = bar
-00003d60: 0a20 2020 202e 2e2e 0a20 2020 203e 3e3e  .    ....    >>>
-00003d70: 2073 6c6f 7474 6564 203d 2053 6c6f 7474   slotted = Slott
-00003d80: 6564 2822 6122 2c20 2262 2229 0a20 2020  ed("a", "b").   
-00003d90: 203e 3e3e 2073 6f72 7465 6428 6765 745f   >>> sorted(get_
-00003da0: 7374 6174 6528 736c 6f74 7465 6429 2e69  state(slotted).i
-00003db0: 7465 6d73 2829 290a 2020 2020 5b28 2762  tems()).    [('b
-00003dc0: 6172 272c 2027 6227 292c 2028 2766 6f6f  ar', 'b'), ('foo
-00003dd0: 272c 2027 6127 295d 0a0a 416c 736f 2070  ', 'a')]..Also p
-00003de0: 726f 7669 6465 7320 6120 6052 6564 7563  rovides a `Reduc
-00003df0: 6962 6c65 4d65 7461 6020 6d65 7461 636c  ibleMeta` metacl
-00003e00: 6173 7320 7468 6174 2061 6c6c 6f77 7320  ass that allows 
-00003e10: 666f 7220 7069 636b 6c69 6e67 2069 6e73  for pickling ins
-00003e20: 7461 6e63 6573 206f 6620 736c 6f74 7465  tances of slotte
-00003e30: 6420 636c 6173 7365 7320 696e 2050 7974  d classes in Pyt
-00003e40: 686f 6e20 322e 372e 0a0a 7175 616c 6e61  hon 2.7...qualna
-00003e50: 6d65 0a5e 5e5e 5e5e 5e5e 5e0a 5079 7468  me.^^^^^^^^.Pyth
-00003e60: 6f6e 2032 2e37 2063 6f6d 7061 7469 626c  on 2.7 compatibl
-00003e70: 6520 7761 7920 6f66 2067 6574 7469 6e67  e way of getting
-00003e80: 2074 6865 2071 7561 6c69 6669 6564 206e   the qualified n
-00003e90: 616d 652e 2042 6173 6564 206f 6e0a 6077  ame. Based on.`w
-00003ea0: 626f 6c73 7465 722f 7175 616c 6e61 6d65  bolster/qualname
-00003eb0: 203c 6874 7470 733a 2f2f 6769 7468 7562   <https://github
-00003ec0: 2e63 6f6d 2f77 626f 6c73 7465 722f 7175  .com/wbolster/qu
-00003ed0: 616c 6e61 6d65 3e60 5f2e 0a41 6c73 6f20  alname>`_..Also 
-00003ee0: 7072 6f76 6964 6573 2061 2060 5175 616c  provides a `Qual
-00003ef0: 6e61 6d65 644d 6574 6160 206d 6574 6163  namedMeta` metac
-00003f00: 6c61 7373 2077 6974 6820 6120 605f 5f71  lass with a `__q
-00003f10: 7561 6c6e 616d 655f 5f60 2063 6c61 7373  ualname__` class
-00003f20: 2070 726f 7065 7274 7920 666f 7220 5079   property for Py
-00003f30: 7468 6f6e 2032 2e37 2e0a 0a72 6563 7572  thon 2.7...recur
-00003f40: 7369 7665 5f72 6570 720a 5e5e 5e5e 5e5e  sive_repr.^^^^^^
-00003f50: 5e5e 5e5e 5e5e 5e5e 0a44 6563 6f72 6174  ^^^^^^^^.Decorat
-00003f60: 6f72 2074 6861 7420 7072 6576 656e 7473  or that prevents
-00003f70: 2069 6e66 696e 6974 6520 7265 6375 7273   infinite recurs
-00003f80: 696f 6e20 666f 7220 605f 5f72 6570 725f  ion for `__repr_
-00003f90: 5f60 206d 6574 686f 6473 2e0a 0a2e 2e20  _` methods..... 
-00003fa0: 636f 6465 3a3a 2070 7974 686f 6e0a 0a20  code:: python.. 
-00003fb0: 2020 203e 3e3e 2066 726f 6d20 6261 7369     >>> from basi
-00003fc0: 6363 6f2e 7265 6375 7273 6976 655f 7265  cco.recursive_re
-00003fd0: 7072 2069 6d70 6f72 7420 7265 6375 7273  pr import recurs
-00003fe0: 6976 655f 7265 7072 0a20 2020 203e 3e3e  ive_repr.    >>>
-00003ff0: 2063 6c61 7373 204d 7943 6c61 7373 286f   class MyClass(o
-00004000: 626a 6563 7429 3a0a 2020 2020 2e2e 2e0a  bject):.    ....
-00004010: 2020 2020 2e2e 2e20 2020 2020 4072 6563      ...     @rec
-00004020: 7572 7369 7665 5f72 6570 720a 2020 2020  ursive_repr.    
-00004030: 2e2e 2e20 2020 2020 6465 6620 5f5f 7265  ...     def __re
-00004040: 7072 5f5f 2873 656c 6629 3a0a 2020 2020  pr__(self):.    
-00004050: 2e2e 2e20 2020 2020 2020 2020 7265 7475  ...         retu
-00004060: 726e 2022 4d79 436c 6173 733c 7b21 727d  rn "MyClass<{!r}
-00004070: 3e22 2e66 6f72 6d61 7428 7365 6c66 290a  >".format(self).
-00004080: 2020 2020 2e2e 2e0a 2020 2020 3e3e 3e20      ....    >>> 
-00004090: 6d79 5f6f 626a 203d 204d 7943 6c61 7373  my_obj = MyClass
-000040a0: 2829 0a20 2020 203e 3e3e 2072 6570 7228  ().    >>> repr(
-000040b0: 6d79 5f6f 626a 290a 2020 2020 274d 7943  my_obj).    'MyC
-000040c0: 6c61 7373 3c2e 2e2e 3e27 0a0a 7275 6e74  lass<...>'..runt
-000040d0: 696d 655f 6669 6e61 6c0a 5e5e 5e5e 5e5e  ime_final.^^^^^^
-000040e0: 5e5e 5e5e 5e5e 5e0a 5275 6e74 696d 652d  ^^^^^^^.Runtime-
-000040f0: 6368 6563 6b65 6420 7665 7273 696f 6e20  checked version 
-00004100: 6f66 2074 6865 2060 7479 7069 6e67 2e66  of the `typing.f
-00004110: 696e 616c 203c 6874 7470 733a 2f2f 646f  inal <https://do
-00004120: 6373 2e70 7974 686f 6e2e 6f72 672f 332f  cs.python.org/3/
-00004130: 6c69 6272 6172 792f 7479 7069 6e67 2e68  library/typing.h
-00004140: 746d 6c23 7479 7069 6e67 2e66 696e 616c  tml#typing.final
-00004150: 3e60 5f20 6465 636f 7261 746f 722e 0a0a  >`_ decorator...
-00004160: 4361 6e20 6265 2075 7365 6420 6f6e 206d  Can be used on m
-00004170: 6574 686f 6473 2c20 7072 6f70 6572 7469  ethods, properti
-00004180: 6573 2c20 636c 6173 736d 6574 686f 6473  es, classmethods
-00004190: 2c20 7374 6174 6963 6d65 7468 6f64 732c  , staticmethods,
-000041a0: 2061 6e64 2063 6c61 7373 6573 2074 6861   and classes tha
-000041b0: 7420 6861 7665 2060 5275 6e74 696d 6546  t have `RuntimeF
-000041c0: 696e 616c 4d65 7461 6020 6173 2061 206d  inalMeta` as a m
-000041d0: 6574 6163 6c61 7373 2e0a 4974 2069 7320  etaclass..It is 
-000041e0: 616c 736f 2072 6563 6f67 6e69 7a65 6420  also recognized 
-000041f0: 6279 2073 7461 7469 6320 7479 7065 2063  by static type c
-00004200: 6865 636b 6572 7320 616e 6420 7072 6576  heckers and prev
-00004210: 656e 7473 2073 7562 636c 6173 7369 6e67  ents subclassing
-00004220: 2061 6e64 2f6f 7220 6d65 6d62 6572 206f   and/or member o
-00004230: 7665 7272 6964 696e 6720 6475 7269 6e67  verriding during
-00004240: 2072 756e 7469 6d65 3a0a 0a2e 2e20 636f   runtime:.... co
-00004250: 6465 3a3a 2070 7974 686f 6e0a 0a20 2020  de:: python..   
-00004260: 203e 3e3e 2066 726f 6d20 7369 7820 696d   >>> from six im
-00004270: 706f 7274 2077 6974 685f 6d65 7461 636c  port with_metacl
-00004280: 6173 730a 2020 2020 3e3e 3e20 6672 6f6d  ass.    >>> from
-00004290: 2062 6173 6963 636f 2e72 756e 7469 6d65   basicco.runtime
-000042a0: 5f66 696e 616c 2069 6d70 6f72 7420 5275  _final import Ru
-000042b0: 6e74 696d 6546 696e 616c 4d65 7461 2c20  ntimeFinalMeta, 
-000042c0: 6669 6e61 6c0a 2020 2020 3e3e 3e20 4066  final.    >>> @f
-000042d0: 696e 616c 0a20 2020 202e 2e2e 2063 6c61  inal.    ... cla
-000042e0: 7373 2041 7373 6574 2877 6974 685f 6d65  ss Asset(with_me
-000042f0: 7461 636c 6173 7328 5275 6e74 696d 6546  taclass(RuntimeF
-00004300: 696e 616c 4d65 7461 2c20 6f62 6a65 6374  inalMeta, object
-00004310: 2929 3a0a 2020 2020 2e2e 2e20 2020 2020  )):.    ...     
-00004320: 7061 7373 0a20 2020 202e 2e2e 0a20 2020  pass.    ....   
-00004330: 203e 3e3e 2063 6c61 7373 2053 7562 4173   >>> class SubAs
-00004340: 7365 7428 4173 7365 7429 3a0a 2020 2020  set(Asset):.    
-00004350: 2e2e 2e20 2020 2020 7061 7373 0a20 2020  ...     pass.   
-00004360: 202e 2e2e 0a20 2020 2054 7261 6365 6261   ....    Traceba
-00004370: 636b 2028 6d6f 7374 2072 6563 656e 7420  ck (most recent 
-00004380: 6361 6c6c 206c 6173 7429 3a0a 2020 2020  call last):.    
-00004390: 5479 7065 4572 726f 723a 2063 616e 2774  TypeError: can't
-000043a0: 2073 7562 636c 6173 7320 6669 6e61 6c20   subclass final 
-000043b0: 636c 6173 7320 2741 7373 6574 270a 0a2e  class 'Asset'...
-000043c0: 2e20 636f 6465 3a3a 2070 7974 686f 6e0a  . code:: python.
-000043d0: 0a20 2020 203e 3e3e 2066 726f 6d20 7369  .    >>> from si
-000043e0: 7820 696d 706f 7274 2077 6974 685f 6d65  x import with_me
-000043f0: 7461 636c 6173 730a 2020 2020 3e3e 3e20  taclass.    >>> 
-00004400: 6672 6f6d 2062 6173 6963 636f 2e72 756e  from basicco.run
-00004410: 7469 6d65 5f66 696e 616c 2069 6d70 6f72  time_final impor
-00004420: 7420 5275 6e74 696d 6546 696e 616c 4d65  t RuntimeFinalMe
-00004430: 7461 2c20 6669 6e61 6c0a 2020 2020 3e3e  ta, final.    >>
-00004440: 3e20 636c 6173 7320 4173 7365 7428 7769  > class Asset(wi
-00004450: 7468 5f6d 6574 6163 6c61 7373 2852 756e  th_metaclass(Run
-00004460: 7469 6d65 4669 6e61 6c4d 6574 612c 206f  timeFinalMeta, o
-00004470: 626a 6563 7429 293a 0a20 2020 202e 2e2e  bject)):.    ...
-00004480: 2020 2020 2040 6669 6e61 6c0a 2020 2020       @final.    
-00004490: 2e2e 2e20 2020 2020 6465 6620 6d65 7468  ...     def meth
-000044a0: 6f64 2873 656c 6629 3a0a 2020 2020 2e2e  od(self):.    ..
-000044b0: 2e20 2020 2020 2020 2020 7061 7373 0a20  .         pass. 
-000044c0: 2020 202e 2e2e 0a20 2020 203e 3e3e 2063     ....    >>> c
-000044d0: 6c61 7373 2053 7562 4173 7365 7428 4173  lass SubAsset(As
-000044e0: 7365 7429 3a0a 2020 2020 2e2e 2e20 2020  set):.    ...   
-000044f0: 2020 6465 6620 6d65 7468 6f64 2873 656c    def method(sel
-00004500: 6629 3a0a 2020 2020 2e2e 2e20 2020 2020  f):.    ...     
-00004510: 2020 2020 7061 7373 0a20 2020 2054 7261      pass.    Tra
-00004520: 6365 6261 636b 2028 6d6f 7374 2072 6563  ceback (most rec
-00004530: 656e 7420 6361 6c6c 206c 6173 7429 3a0a  ent call last):.
-00004540: 2020 2020 5479 7065 4572 726f 723a 2027      TypeError: '
-00004550: 5375 6241 7373 6574 2720 6f76 6572 7269  SubAsset' overri
-00004560: 6465 7320 6669 6e61 6c20 6d65 6d62 6572  des final member
-00004570: 2027 6d65 7468 6f64 2720 6465 6669 6e65   'method' define
-00004580: 6420 6279 2027 4173 7365 7427 0a0a 2e2e  d by 'Asset'....
-00004590: 2063 6f64 653a 3a20 7079 7468 6f6e 0a0a   code:: python..
-000045a0: 2020 2020 3e3e 3e20 6672 6f6d 2073 6978      >>> from six
-000045b0: 2069 6d70 6f72 7420 7769 7468 5f6d 6574   import with_met
-000045c0: 6163 6c61 7373 0a20 2020 203e 3e3e 2066  aclass.    >>> f
-000045d0: 726f 6d20 6261 7369 6363 6f2e 7275 6e74  rom basicco.runt
-000045e0: 696d 655f 6669 6e61 6c20 696d 706f 7274  ime_final import
-000045f0: 2052 756e 7469 6d65 4669 6e61 6c4d 6574   RuntimeFinalMet
-00004600: 612c 2066 696e 616c 0a20 2020 203e 3e3e  a, final.    >>>
-00004610: 2063 6c61 7373 2041 7373 6574 2877 6974   class Asset(wit
-00004620: 685f 6d65 7461 636c 6173 7328 5275 6e74  h_metaclass(Runt
-00004630: 696d 6546 696e 616c 4d65 7461 2c20 6f62  imeFinalMeta, ob
-00004640: 6a65 6374 2929 3a0a 2020 2020 2e2e 2e20  ject)):.    ... 
-00004650: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
-00004660: 2020 2e2e 2e20 2020 2020 4066 696e 616c    ...     @final
-00004670: 0a20 2020 202e 2e2e 2020 2020 2064 6566  .    ...     def
-00004680: 2070 726f 7028 7365 6c66 293a 0a20 2020   prop(self):.   
-00004690: 202e 2e2e 2020 2020 2020 2020 2070 6173   ...         pas
-000046a0: 730a 2020 2020 2e2e 2e0a 2020 2020 3e3e  s.    ....    >>
-000046b0: 3e20 636c 6173 7320 5375 6241 7373 6574  > class SubAsset
-000046c0: 2841 7373 6574 293a 0a20 2020 202e 2e2e  (Asset):.    ...
-000046d0: 2020 2020 2040 7072 6f70 6572 7479 0a20       @property. 
-000046e0: 2020 202e 2e2e 2020 2020 2064 6566 2070     ...     def p
-000046f0: 726f 7028 7365 6c66 293a 0a20 2020 202e  rop(self):.    .
-00004700: 2e2e 2020 2020 2020 2020 2070 6173 730a  ..         pass.
-00004710: 2020 2020 5472 6163 6562 6163 6b20 286d      Traceback (m
-00004720: 6f73 7420 7265 6365 6e74 2063 616c 6c20  ost recent call 
-00004730: 6c61 7374 293a 0a20 2020 2054 7970 6545  last):.    TypeE
-00004740: 7272 6f72 3a20 2753 7562 4173 7365 7427  rror: 'SubAsset'
-00004750: 206f 7665 7272 6964 6573 2066 696e 616c   overrides final
-00004760: 206d 656d 6265 7220 2770 726f 7027 2064   member 'prop' d
-00004770: 6566 696e 6564 2062 7920 2741 7373 6574  efined by 'Asset
-00004780: 270a 0a73 6166 655f 6e6f 745f 6571 7561  '..safe_not_equa
-00004790: 6c73 0a5e 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e  ls.^^^^^^^^^^^^^
-000047a0: 5e5e 0a42 6163 6b70 6f72 7420 6f66 2074  ^^.Backport of t
-000047b0: 6865 2064 6566 6175 6c74 2050 7974 686f  he default Pytho
-000047c0: 6e20 3320 6265 6861 7669 6f72 206f 6620  n 3 behavior of 
-000047d0: 605f 5f6e 655f 5f60 2062 6568 6176 696f  `__ne__` behavio
-000047e0: 7220 666f 7220 5079 7468 6f6e 2032 2e37  r for Python 2.7
-000047f0: 2e0a 0a2e 2e20 636f 6465 3a3a 2070 7974  ..... code:: pyt
-00004800: 686f 6e0a 0a20 2020 203e 3e3e 2066 726f  hon..    >>> fro
-00004810: 6d20 7369 7820 696d 706f 7274 2077 6974  m six import wit
-00004820: 685f 6d65 7461 636c 6173 730a 2020 2020  h_metaclass.    
-00004830: 3e3e 3e20 6672 6f6d 2062 6173 6963 636f  >>> from basicco
-00004840: 2e73 6166 655f 6e6f 745f 6571 7561 6c73  .safe_not_equals
-00004850: 2069 6d70 6f72 7420 5361 6665 4e6f 7445   import SafeNotE
-00004860: 7175 616c 734d 6574 610a 2020 2020 3e3e  qualsMeta.    >>
-00004870: 3e20 636c 6173 7320 436c 6173 7328 7769  > class Class(wi
-00004880: 7468 5f6d 6574 6163 6c61 7373 2853 6166  th_metaclass(Saf
-00004890: 654e 6f74 4571 7561 6c73 4d65 7461 2c20  eNotEqualsMeta, 
-000048a0: 6f62 6a65 6374 2929 3a0a 2020 2020 2e2e  object)):.    ..
-000048b0: 2e20 2020 2020 7061 7373 0a20 2020 202e  .     pass.    .
-000048c0: 2e2e 0a20 2020 203e 3e3e 206f 626a 5f61  ...    >>> obj_a
-000048d0: 203d 2043 6c61 7373 2829 0a20 2020 203e   = Class().    >
-000048e0: 3e3e 206f 626a 5f62 203d 2043 6c61 7373  >> obj_b = Class
-000048f0: 2829 0a20 2020 203e 3e3e 2061 7373 6572  ().    >>> asser
-00004900: 7420 286f 626a 5f61 203d 3d20 6f62 6a5f  t (obj_a == obj_
-00004910: 6129 2069 7320 6e6f 7420 286f 626a 5f61  a) is not (obj_a
-00004920: 2021 3d20 6f62 6a5f 6129 0a20 2020 203e   != obj_a).    >
-00004930: 3e3e 2061 7373 6572 7420 286f 626a 5f62  >> assert (obj_b
-00004940: 203d 3d20 6f62 6a5f 6229 2069 7320 6e6f   == obj_b) is no
-00004950: 7420 286f 626a 5f62 2021 3d20 6f62 6a5f  t (obj_b != obj_
-00004960: 6229 0a20 2020 203e 3e3e 2061 7373 6572  b).    >>> asser
-00004970: 7420 286f 626a 5f61 203d 3d20 6f62 6a5f  t (obj_a == obj_
-00004980: 6229 2069 7320 6e6f 7420 286f 626a 5f61  b) is not (obj_a
-00004990: 2021 3d20 6f62 6a5f 6229 0a0a 7361 6665   != obj_b)..safe
-000049a0: 5f72 6570 720a 5e5e 5e5e 5e5e 5e5e 5e0a  _repr.^^^^^^^^^.
-000049b0: 4465 636f 7261 746f 7220 7468 6174 2070  Decorator that p
-000049c0: 7265 7665 6e74 7320 605f 5f72 6570 725f  revents `__repr_
-000049d0: 5f60 206d 6574 686f 6473 2066 726f 6d20  _` methods from 
-000049e0: 7261 6973 696e 6720 6578 6365 7074 696f  raising exceptio
-000049f0: 6e73 2061 6e64 2072 6574 7572 6e20 6120  ns and return a 
-00004a00: 6465 6661 756c 7420 7265 7072 6573 656e  default represen
-00004a10: 7461 7469 6f6e 2069 6e73 7465 6164 2e0a  tation instead..
-00004a20: 0a2e 2e20 636f 6465 3a3a 2070 7974 686f  ... code:: pytho
-00004a30: 6e0a 0a20 2020 203e 3e3e 2066 726f 6d20  n..    >>> from 
-00004a40: 6261 7369 6363 6f2e 7361 6665 5f72 6570  basicco.safe_rep
-00004a50: 7220 696d 706f 7274 2073 6166 655f 7265  r import safe_re
-00004a60: 7072 0a20 2020 203e 3e3e 2063 6c61 7373  pr.    >>> class
-00004a70: 2043 6c61 7373 286f 626a 6563 7429 3a0a   Class(object):.
-00004a80: 2020 2020 2e2e 2e20 2020 2020 4073 6166      ...     @saf
-00004a90: 655f 7265 7072 0a20 2020 202e 2e2e 2020  e_repr.    ...  
-00004aa0: 2020 2064 6566 205f 5f72 6570 725f 5f28     def __repr__(
-00004ab0: 7365 6c66 293a 0a20 2020 202e 2e2e 2020  self):.    ...  
-00004ac0: 2020 2020 2020 2072 6169 7365 2052 756e         raise Run
-00004ad0: 7469 6d65 4572 726f 7228 226f 6820 6f68  timeError("oh oh
-00004ae0: 2229 0a20 2020 202e 2e2e 0a20 2020 203e  ").    ....    >
-00004af0: 3e3e 206f 626a 203d 2043 6c61 7373 2829  >> obj = Class()
-00004b00: 0a20 2020 203e 3e3e 2072 6570 7228 6f62  .    >>> repr(ob
-00004b10: 6a29 0a20 2020 2022 3c5f 5f6d 6169 6e5f  j).    "<__main_
-00004b20: 5f2e 436c 6173 7320 6f62 6a65 6374 2061  _.Class object a
-00004b30: 7420 2e2e 2e3b 2072 6570 7220 6661 696c  t ...; repr fail
-00004b40: 6564 2064 7565 2074 6f20 2752 756e 7469  ed due to 'Runti
-00004b50: 6d65 4572 726f 723a 206f 6820 6f68 273e  meError: oh oh'>
-00004b60: 220a 0a73 6574 5f6e 616d 650a 5e5e 5e5e  "..set_name.^^^^
-00004b70: 5e5e 5e5e 0a42 6163 6b70 6f72 7420 6f66  ^^^^.Backport of
-00004b80: 2074 6865 2066 756e 6374 696f 6e61 6c69   the functionali
-00004b90: 7479 206f 6620 605f 5f73 6574 5f6e 616d  ty of `__set_nam
-00004ba0: 655f 5f60 2066 726f 6d20 5045 5020 3438  e__` from PEP 48
-00004bb0: 3720 746f 2050 7974 686f 6e20 322e 372e  7 to Python 2.7.
-00004bc0: 0a0a 2e2e 2063 6f64 653a 3a20 7079 7468  .... code:: pyth
-00004bd0: 6f6e 0a0a 2020 2020 3e3e 3e20 6672 6f6d  on..    >>> from
-00004be0: 2062 6173 6963 636f 2e73 6574 5f6e 616d   basicco.set_nam
-00004bf0: 6520 696d 706f 7274 2053 6574 4e61 6d65  e import SetName
-00004c00: 0a20 2020 203e 3e3e 2063 6c61 7373 2041  .    >>> class A
-00004c10: 7474 7269 6275 7465 286f 626a 6563 7429  ttribute(object)
-00004c20: 3a0a 2020 2020 2e2e 2e20 2020 2020 6465  :.    ...     de
-00004c30: 6620 5f5f 7365 745f 6e61 6d65 5f5f 2873  f __set_name__(s
-00004c40: 656c 662c 206f 776e 6572 2c20 6e61 6d65  elf, owner, name
-00004c50: 293a 0a20 2020 202e 2e2e 2020 2020 2020  ):.    ...      
-00004c60: 2020 2073 656c 662e 6f77 6e65 7220 3d20     self.owner = 
-00004c70: 6f77 6e65 720a 2020 2020 2e2e 2e20 2020  owner.    ...   
-00004c80: 2020 2020 2020 7365 6c66 2e6e 616d 6520        self.name 
-00004c90: 3d20 6e61 6d65 0a20 2020 202e 2e2e 0a20  = name.    .... 
-00004ca0: 2020 203e 3e3e 2063 6c61 7373 2043 6f6c     >>> class Col
-00004cb0: 6c65 6374 696f 6e28 5365 744e 616d 6529  lection(SetName)
-00004cc0: 3a0a 2020 2020 2e2e 2e20 2020 2020 666f  :.    ...     fo
-00004cd0: 6f20 3d20 4174 7472 6962 7574 6528 290a  o = Attribute().
-00004ce0: 2020 2020 2e2e 2e0a 2020 2020 3e3e 3e20      ....    >>> 
-00004cf0: 436f 6c6c 6563 7469 6f6e 2e66 6f6f 2e6f  Collection.foo.o
-00004d00: 776e 6572 2069 7320 436f 6c6c 6563 7469  wner is Collecti
-00004d10: 6f6e 0a20 2020 2054 7275 650a 2020 2020  on.    True.    
-00004d20: 3e3e 3e20 436f 6c6c 6563 7469 6f6e 2e66  >>> Collection.f
-00004d30: 6f6f 2e6e 616d 650a 2020 2020 2766 6f6f  oo.name.    'foo
-00004d40: 270a 0a74 7970 655f 6368 6563 6b69 6e67  '..type_checking
-00004d50: 0a5e 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e 0a52  .^^^^^^^^^^^^^.R
-00004d60: 756e 7469 6d65 2074 7970 6520 6368 6563  untime type chec
-00004d70: 6b69 6e67 2077 6974 6820 7375 7070 6f72  king with suppor
-00004d80: 7420 666f 7220 696d 706f 7274 2070 6174  t for import pat
-00004d90: 6873 2061 6e64 2074 7970 6520 6869 6e74  hs and type hint
-00004da0: 732e 0a0a 2e2e 2063 6f64 653a 3a20 7079  s..... code:: py
-00004db0: 7468 6f6e 0a0a 2020 2020 3e3e 3e20 6672  thon..    >>> fr
-00004dc0: 6f6d 2074 6970 706f 2069 6d70 6f72 7420  om tippo import 
-00004dd0: 4d61 7070 696e 670a 2020 2020 3e3e 3e20  Mapping.    >>> 
-00004de0: 6672 6f6d 2069 7465 7274 6f6f 6c73 2069  from itertools i
-00004df0: 6d70 6f72 7420 6368 6169 6e0a 2020 2020  mport chain.    
-00004e00: 3e3e 3e20 6672 6f6d 2062 6173 6963 636f  >>> from basicco
-00004e10: 2e74 7970 655f 6368 6563 6b69 6e67 2069  .type_checking i
-00004e20: 6d70 6f72 7420 6973 5f69 6e73 7461 6e63  mport is_instanc
-00004e30: 650a 2020 2020 3e3e 3e20 636c 6173 7320  e.    >>> class 
-00004e40: 5375 6243 6861 696e 2863 6861 696e 293a  SubChain(chain):
-00004e50: 0a20 2020 202e 2e2e 2020 2020 2070 6173  .    ...     pas
-00004e60: 730a 2020 2020 2e2e 2e0a 2020 2020 3e3e  s.    ....    >>
-00004e70: 3e20 6973 5f69 6e73 7461 6e63 6528 332c  > is_instance(3,
-00004e80: 2069 6e74 290a 2020 2020 5472 7565 0a20   int).    True. 
-00004e90: 2020 203e 3e3e 2069 735f 696e 7374 616e     >>> is_instan
-00004ea0: 6365 2833 2c20 2863 6861 696e 2c20 696e  ce(3, (chain, in
-00004eb0: 7429 290a 2020 2020 5472 7565 0a20 2020  t)).    True.   
-00004ec0: 203e 3e3e 2069 735f 696e 7374 616e 6365   >>> is_instance
-00004ed0: 2833 2c20 2829 290a 2020 2020 4661 6c73  (3, ()).    Fals
-00004ee0: 650a 2020 2020 3e3e 3e20 6973 5f69 6e73  e.    >>> is_ins
-00004ef0: 7461 6e63 6528 5375 6243 6861 696e 2829  tance(SubChain()
-00004f00: 2c20 2269 7465 7274 6f6f 6c73 2e63 6861  , "itertools.cha
-00004f10: 696e 2229 0a20 2020 2054 7275 650a 2020  in").    True.  
-00004f20: 2020 3e3e 3e20 6973 5f69 6e73 7461 6e63    >>> is_instanc
-00004f30: 6528 6368 6169 6e28 292c 2022 6974 6572  e(chain(), "iter
-00004f40: 746f 6f6c 732e 6368 6169 6e22 2c20 7375  tools.chain", su
-00004f50: 6274 7970 6573 3d46 616c 7365 290a 2020  btypes=False).  
-00004f60: 2020 5472 7565 0a20 2020 203e 3e3e 2069    True.    >>> i
-00004f70: 735f 696e 7374 616e 6365 2853 7562 4368  s_instance(SubCh
-00004f80: 6169 6e28 292c 2022 6974 6572 746f 6f6c  ain(), "itertool
-00004f90: 732e 6368 6169 6e22 2c20 7375 6274 7970  s.chain", subtyp
-00004fa0: 6573 3d46 616c 7365 290a 2020 2020 4661  es=False).    Fa
-00004fb0: 6c73 650a 2020 2020 3e3e 3e20 6973 5f69  lse.    >>> is_i
-00004fc0: 6e73 7461 6e63 6528 7b22 6122 3a20 312c  nstance({"a": 1,
-00004fd0: 2022 6222 3a20 327d 2c20 4d61 7070 696e   "b": 2}, Mappin
-00004fe0: 675b 7374 722c 2069 6e74 5d29 0a20 2020  g[str, int]).   
-00004ff0: 2054 7275 650a 0a75 6e69 7175 655f 6974   True..unique_it
-00005000: 6572 6174 6f72 0a5e 5e5e 5e5e 5e5e 5e5e  erator.^^^^^^^^^
-00005010: 5e5e 5e5e 5e5e 0a49 7465 7261 746f 7220  ^^^^^^.Iterator 
-00005020: 7468 6174 2079 6965 6c64 7320 756e 6971  that yields uniq
-00005030: 7565 2076 616c 7565 732e 0a0a 2e2e 2063  ue values..... c
-00005040: 6f64 653a 3a20 7079 7468 6f6e 0a0a 2020  ode:: python..  
-00005050: 2020 3e3e 3e20 6672 6f6d 2062 6173 6963    >>> from basic
-00005060: 636f 2e75 6e69 7175 655f 6974 6572 6174  co.unique_iterat
-00005070: 6f72 2069 6d70 6f72 7420 756e 6971 7565  or import unique
-00005080: 5f69 7465 7261 746f 720a 2020 2020 3e3e  _iterator.    >>
-00005090: 3e20 6c69 7374 2875 6e69 7175 655f 6974  > list(unique_it
-000050a0: 6572 6174 6f72 285b 312c 2032 2c20 332c  erator([1, 2, 3,
-000050b0: 2033 2c20 342c 2034 2c20 355d 2929 0a20   3, 4, 4, 5])). 
-000050c0: 2020 205b 312c 2032 2c20 332c 2034 2c20     [1, 2, 3, 4, 
-000050d0: 355d 0a0a 7765 616b 5f72 6566 6572 656e  5]..weak_referen
-000050e0: 6365 0a5e 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e  ce.^^^^^^^^^^^^^
-000050f0: 5e0a 5765 616b 2052 6566 6572 656e 6365  ^.Weak Reference
-00005100: 2d6c 696b 6520 6f62 6a65 6374 2074 6861  -like object tha
-00005110: 7420 7375 7070 6f72 7473 2070 6963 6b6c  t supports pickl
-00005120: 696e 672e                                ing.
+00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
+00000010: 3a20 322e 310a 4e61 6d65 3a20 6261 7369  : 2.1.Name: basi
+00000020: 6363 6f0a 5665 7273 696f 6e3a 2039 2e30  cco.Version: 9.0
+00000030: 2e30 0a53 756d 6d61 7279 3a20 4261 7365  .0.Summary: Base
+00000040: 2063 6c61 7373 6573 2061 6e64 2075 7469   classes and uti
+00000050: 6c69 7469 6573 2074 6861 7420 656e 6861  lities that enha
+00000060: 6e63 6520 636f 6465 2063 6f6d 7061 7469  nce code compati
+00000070: 6269 6c69 7479 2c20 6665 6174 7572 6573  bility, features
+00000080: 2061 6e64 2076 616c 6964 6174 696f 6e2e   and validation.
+00000090: 0a48 6f6d 652d 7061 6765 3a20 6874 7470  .Home-page: http
+000000a0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f62  s://github.com/b
+000000b0: 7275 6e6f 6e69 636b 6f2f 6261 7369 6363  runonicko/basicc
+000000c0: 6f0a 4175 7468 6f72 3a20 4272 756e 6f20  o.Author: Bruno 
+000000d0: 4e69 636b 6f0a 4175 7468 6f72 2d65 6d61  Nicko.Author-ema
+000000e0: 696c 3a20 6272 756e 6f6e 6963 6b6f 4067  il: brunonicko@g
+000000f0: 6d61 696c 2e63 6f6d 0a43 6c61 7373 6966  mail.com.Classif
+00000100: 6965 723a 2049 6e74 656e 6465 6420 4175  ier: Intended Au
+00000110: 6469 656e 6365 203a 3a20 4465 7665 6c6f  dience :: Develo
+00000120: 7065 7273 0a43 6c61 7373 6966 6965 723a  pers.Classifier:
+00000130: 204c 6963 656e 7365 203a 3a20 4f53 4920   License :: OSI 
+00000140: 4170 7072 6f76 6564 203a 3a20 4d49 5420  Approved :: MIT 
+00000150: 4c69 6365 6e73 650a 436c 6173 7369 6669  License.Classifi
+00000160: 6572 3a20 4f70 6572 6174 696e 6720 5379  er: Operating Sy
+00000170: 7374 656d 203a 3a20 4f53 2049 6e64 6570  stem :: OS Indep
+00000180: 656e 6465 6e74 0a43 6c61 7373 6966 6965  endent.Classifie
+00000190: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
+000001a0: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
+000001b0: 6e20 3a3a 2032 2e37 0a43 6c61 7373 6966  n :: 2.7.Classif
+000001c0: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
+000001d0: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
+000001e0: 686f 6e20 3a3a 2033 2e37 0a43 6c61 7373  hon :: 3.7.Class
+000001f0: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
+00000200: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+00000210: 7974 686f 6e20 3a3a 2033 2e38 0a43 6c61  ython :: 3.8.Cla
+00000220: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
+00000230: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
+00000240: 2050 7974 686f 6e20 3a3a 2033 2e39 0a43   Python :: 3.9.C
+00000250: 6c61 7373 6966 6965 723a 2050 726f 6772  lassifier: Progr
+00000260: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
+00000270: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e31  :: Python :: 3.1
+00000280: 300a 436c 6173 7369 6669 6572 3a20 5072  0.Classifier: Pr
+00000290: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
+000002a0: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
+000002b0: 332e 3131 0a43 6c61 7373 6966 6965 723a  3.11.Classifier:
+000002c0: 2050 726f 6772 616d 6d69 6e67 204c 616e   Programming Lan
+000002d0: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
+000002e0: 3a3a 2049 6d70 6c65 6d65 6e74 6174 696f  :: Implementatio
+000002f0: 6e20 3a3a 2050 7950 790a 5265 7175 6972  n :: PyPy.Requir
+00000300: 6573 2d50 7974 686f 6e3a 203e 3d20 322e  es-Python: >= 2.
+00000310: 372c 2021 3d20 332e 302e 2a2c 2021 3d20  7, != 3.0.*, != 
+00000320: 332e 312e 2a2c 2021 3d20 332e 322e 2a2c  3.1.*, != 3.2.*,
+00000330: 2021 3d20 332e 332e 2a2c 2021 3d20 332e   != 3.3.*, != 3.
+00000340: 342e 2a2c 2021 3d20 332e 352e 2a2c 2021  4.*, != 3.5.*, !
+00000350: 3d20 332e 362e 2a0a 4465 7363 7269 7074  = 3.6.*.Descript
+00000360: 696f 6e2d 436f 6e74 656e 742d 5479 7065  ion-Content-Type
+00000370: 3a20 7465 7874 2f78 2d72 7374 0a4c 6963  : text/x-rst.Lic
+00000380: 656e 7365 2d46 696c 653a 204c 4943 454e  ense-File: LICEN
+00000390: 5345 0a0a 4261 7369 6363 6f0a 3d3d 3d3d  SE..Basicco.====
+000003a0: 3d3d 3d0a 0a2e 2e20 696d 6167 653a 3a20  ===.... image:: 
+000003b0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+000003c0: 6f6d 2f62 7275 6e6f 6e69 636b 6f2f 6261  om/brunonicko/ba
+000003d0: 7369 6363 6f2f 776f 726b 666c 6f77 732f  sicco/workflows/
+000003e0: 4d79 5079 2f62 6164 6765 2e73 7667 0a20  MyPy/badge.svg. 
+000003f0: 2020 3a74 6172 6765 743a 2068 7474 7073    :target: https
+00000400: 3a2f 2f67 6974 6875 622e 636f 6d2f 6272  ://github.com/br
+00000410: 756e 6f6e 6963 6b6f 2f62 6173 6963 636f  unonicko/basicco
+00000420: 2f61 6374 696f 6e73 3f71 7565 7279 3d77  /actions?query=w
+00000430: 6f72 6b66 6c6f 7725 3341 4d79 5079 0a0a  orkflow%3AMyPy..
+00000440: 2e2e 2069 6d61 6765 3a3a 2068 7474 7073  .. image:: https
+00000450: 3a2f 2f67 6974 6875 622e 636f 6d2f 6272  ://github.com/br
+00000460: 756e 6f6e 6963 6b6f 2f62 6173 6963 636f  unonicko/basicco
+00000470: 2f77 6f72 6b66 6c6f 7773 2f4c 696e 742f  /workflows/Lint/
+00000480: 6261 6467 652e 7376 670a 2020 203a 7461  badge.svg.   :ta
+00000490: 7267 6574 3a20 6874 7470 733a 2f2f 6769  rget: https://gi
+000004a0: 7468 7562 2e63 6f6d 2f62 7275 6e6f 6e69  thub.com/brunoni
+000004b0: 636b 6f2f 6261 7369 6363 6f2f 6163 7469  cko/basicco/acti
+000004c0: 6f6e 733f 7175 6572 793d 776f 726b 666c  ons?query=workfl
+000004d0: 6f77 2533 414c 696e 740a 0a2e 2e20 696d  ow%3ALint.... im
+000004e0: 6167 653a 3a20 6874 7470 733a 2f2f 6769  age:: https://gi
+000004f0: 7468 7562 2e63 6f6d 2f62 7275 6e6f 6e69  thub.com/brunoni
+00000500: 636b 6f2f 6261 7369 6363 6f2f 776f 726b  cko/basicco/work
+00000510: 666c 6f77 732f 5465 7374 732f 6261 6467  flows/Tests/badg
+00000520: 652e 7376 670a 2020 203a 7461 7267 6574  e.svg.   :target
+00000530: 3a20 6874 7470 733a 2f2f 6769 7468 7562  : https://github
+00000540: 2e63 6f6d 2f62 7275 6e6f 6e69 636b 6f2f  .com/brunonicko/
+00000550: 6261 7369 6363 6f2f 6163 7469 6f6e 733f  basicco/actions?
+00000560: 7175 6572 793d 776f 726b 666c 6f77 2533  query=workflow%3
+00000570: 4154 6573 7473 0a0a 2e2e 2069 6d61 6765  ATests.... image
+00000580: 3a3a 2068 7474 7073 3a2f 2f72 6561 6474  :: https://readt
+00000590: 6865 646f 6373 2e6f 7267 2f70 726f 6a65  hedocs.org/proje
+000005a0: 6374 732f 6261 7369 6363 6f2f 6261 6467  cts/basicco/badg
+000005b0: 652f 3f76 6572 7369 6f6e 3d73 7461 626c  e/?version=stabl
+000005c0: 650a 2020 203a 7461 7267 6574 3a20 6874  e.   :target: ht
+000005d0: 7470 733a 2f2f 6261 7369 6363 6f2e 7265  tps://basicco.re
+000005e0: 6164 7468 6564 6f63 732e 696f 2f65 6e2f  adthedocs.io/en/
+000005f0: 7374 6162 6c65 2f0a 0a2e 2e20 696d 6167  stable/.... imag
+00000600: 653a 3a20 6874 7470 733a 2f2f 696d 672e  e:: https://img.
+00000610: 7368 6965 6c64 732e 696f 2f67 6974 6875  shields.io/githu
+00000620: 622f 6c69 6365 6e73 652f 6272 756e 6f6e  b/license/brunon
+00000630: 6963 6b6f 2f62 6173 6963 636f 3f63 6f6c  icko/basicco?col
+00000640: 6f72 3d6c 6967 6874 2d67 7265 656e 0a20  or=light-green. 
+00000650: 2020 3a74 6172 6765 743a 2068 7474 7073    :target: https
+00000660: 3a2f 2f67 6974 6875 622e 636f 6d2f 6272  ://github.com/br
+00000670: 756e 6f6e 6963 6b6f 2f62 6173 6963 636f  unonicko/basicco
+00000680: 2f62 6c6f 622f 6d61 7374 6572 2f4c 4943  /blob/master/LIC
+00000690: 454e 5345 0a0a 2e2e 2069 6d61 6765 3a3a  ENSE.... image::
+000006a0: 2068 7474 7073 3a2f 2f73 7461 7469 632e   https://static.
+000006b0: 7065 7079 2e74 6563 682f 7065 7273 6f6e  pepy.tech/person
+000006c0: 616c 697a 6564 2d62 6164 6765 2f62 6173  alized-badge/bas
+000006d0: 6963 636f 3f70 6572 696f 643d 746f 7461  icco?period=tota
+000006e0: 6c26 756e 6974 733d 696e 7465 726e 6174  l&units=internat
+000006f0: 696f 6e61 6c5f 7379 7374 656d 266c 6566  ional_system&lef
+00000700: 745f 636f 6c6f 723d 6772 6579 2672 6967  t_color=grey&rig
+00000710: 6874 5f63 6f6c 6f72 3d62 7269 6768 7467  ht_color=brightg
+00000720: 7265 656e 266c 6566 745f 7465 7874 3d44  reen&left_text=D
+00000730: 6f77 6e6c 6f61 6473 0a20 2020 3a74 6172  ownloads.   :tar
+00000740: 6765 743a 2068 7474 7073 3a2f 2f70 6570  get: https://pep
+00000750: 792e 7465 6368 2f70 726f 6a65 6374 2f62  y.tech/project/b
+00000760: 6173 6963 636f 0a0a 2e2e 2069 6d61 6765  asicco.... image
+00000770: 3a3a 2068 7474 7073 3a2f 2f69 6d67 2e73  :: https://img.s
+00000780: 6869 656c 6473 2e69 6f2f 7079 7069 2f70  hields.io/pypi/p
+00000790: 7976 6572 7369 6f6e 732f 6261 7369 6363  yversions/basicc
+000007a0: 6f3f 636f 6c6f 723d 6c69 6768 742d 6772  o?color=light-gr
+000007b0: 6565 6e26 7374 796c 653d 666c 6174 0a20  een&style=flat. 
+000007c0: 2020 3a74 6172 6765 743a 2068 7474 7073    :target: https
+000007d0: 3a2f 2f70 7970 692e 6f72 672f 7072 6f6a  ://pypi.org/proj
+000007e0: 6563 742f 6261 7369 6363 6f2f 0a0a 4f76  ect/basicco/..Ov
+000007f0: 6572 7669 6577 0a2d 2d2d 2d2d 2d2d 2d0a  erview.--------.
+00000800: 6042 6173 6520 436c 6173 7365 7360 5f20  `Base Classes`_ 
+00000810: 616e 6420 6055 7469 6c69 7469 6573 605f  and `Utilities`_
+00000820: 2074 6861 7420 656e 6861 6e63 6520 636f   that enhance co
+00000830: 6465 2063 6f6d 7061 7469 6269 6c69 7479  de compatibility
+00000840: 2c20 6665 6174 7572 6573 2061 6e64 2076  , features and v
+00000850: 616c 6964 6174 696f 6e2e 0a0a 4d6f 7469  alidation...Moti
+00000860: 7661 7469 6f6e 0a2d 2d2d 2d2d 2d2d 2d2d  vation.---------
+00000870: 2d0a 5768 696c 6520 6465 7665 6c6f 7069  -.While developi
+00000880: 6e67 2050 7974 686f 6e20 736f 6674 7761  ng Python softwa
+00000890: 7265 2066 6f72 2056 6973 7561 6c20 4566  re for Visual Ef
+000008a0: 6665 6374 7320 7069 7065 6c69 6e65 732c  fects pipelines,
+000008b0: 2049 2066 6f75 6e64 206d 7973 656c 6620   I found myself 
+000008c0: 6861 7669 6e67 2074 6f20 7772 6974 6520  having to write 
+000008d0: 7468 6520 7361 6d65 2062 6f69 6c65 722d  the same boiler-
+000008e0: 706c 6174 650a 636f 6465 206f 7665 7220  plate.code over 
+000008f0: 616e 6420 6f76 6572 2061 6761 696e 2c20  and over again, 
+00000900: 6173 2077 656c 6c20 6173 2073 7472 7567  as well as strug
+00000910: 676c 696e 6720 7769 7468 2063 6f6d 7061  gling with compa
+00000920: 7469 6269 6c69 7479 2069 7373 7565 7320  tibility issues 
+00000930: 616e 6420 6665 6174 7572 6520 6761 7073  and feature gaps
+00000940: 2062 6574 7765 656e 2050 7974 686f 6e20   between Python 
+00000950: 322e 3720 616e 640a 5079 7468 6f6e 2033  2.7 and.Python 3
+00000960: 2e37 2b2e 0a0a 536f 2049 2064 6563 6964  .7+...So I decid
+00000970: 6564 2074 6f20 696d 706c 656d 656e 7420  ed to implement 
+00000980: 736f 6c75 7469 6f6e 7320 666f 7220 7468  solutions for th
+00000990: 6f73 6520 6973 7375 6573 2061 7420 7468  ose issues at th
+000009a0: 6520 6042 6173 6560 5f2c 2061 6e64 2060  e `Base`_, and `
+000009b0: 6261 7369 6363 6f60 2077 6173 2062 6f72  basicco` was bor
+000009c0: 6e2e 0a0a 4261 7365 2043 6c61 7373 6573  n...Base Classes
+000009d0: 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 0a43  .------------..C
+000009e0: 6f6d 7061 7442 6173 650a 5e5e 5e5e 5e5e  ompatBase.^^^^^^
+000009f0: 5e5e 5e5e 0a54 6865 2067 6f61 6c20 7769  ^^^^.The goal wi
+00000a00: 7468 2074 6865 2060 436f 6d70 6174 4261  th the `CompatBa
+00000a10: 7365 4d65 7461 6020 6d65 7461 636c 6173  seMeta` metaclas
+00000a20: 7320 616e 6420 7468 6520 6043 6f6d 7061  s and the `Compa
+00000a30: 7442 6173 6560 2063 6c61 7373 2069 7320  tBase` class is 
+00000a40: 746f 2062 7269 6467 6520 736f 6d65 206f  to bridge some o
+00000a50: 6620 7468 6520 6665 6174 7572 6520 6761  f the feature ga
+00000a60: 7073 2062 6574 7765 656e 0a50 7974 686f  ps between.Pytho
+00000a70: 6e20 322e 3720 616e 6420 5079 7468 6f6e  n 2.7 and Python
+00000a80: 2033 2e37 2b2e 0a0a 5468 6973 2069 6e63   3.7+...This inc
+00000a90: 6c75 6465 7320 6164 6469 6e67 2050 7974  ludes adding Pyt
+00000aa0: 686f 6e20 322e 3720 776f 726b 6172 6f75  hon 2.7 workarou
+00000ab0: 6e64 7320 666f 723a 0a20 202d 2060 4162  nds for:.  - `Ab
+00000ac0: 7374 7261 6374 2070 726f 7065 7274 6965  stract propertie
+00000ad0: 7320 3c68 7474 7073 3a2f 2f64 6f63 732e  s <https://docs.
+00000ae0: 7079 7468 6f6e 2e6f 7267 2f33 2f6c 6962  python.org/3/lib
+00000af0: 7261 7279 2f61 6263 2e68 746d 6c23 6162  rary/abc.html#ab
+00000b00: 632e 6162 7374 7261 6374 7072 6f70 6572  c.abstractproper
+00000b10: 7479 3e60 5f3a 2042 6574 7465 7220 6061  ty>`_: Better `a
+00000b20: 6273 7472 6163 746d 6574 686f 6460 0a20  bstractmethod`. 
+00000b30: 2020 2064 6563 6f72 6174 6f72 2073 7570     decorator sup
+00000b40: 706f 7274 2066 6f72 2070 726f 7065 7274  port for propert
+00000b50: 792d 6c69 6b65 2064 6573 6372 6970 746f  y-like descripto
+00000b60: 7273 2e20 5365 6520 616c 736f 2060 6162  rs. See also `ab
+00000b70: 7374 7261 6374 5f63 6c61 7373 605f 2e0a  stract_class`_..
+00000b80: 2020 2d20 6050 4550 2034 3837 203c 6874    - `PEP 487 <ht
+00000b90: 7470 733a 2f2f 7065 7073 2e70 7974 686f  tps://peps.pytho
+00000ba0: 6e2e 6f72 672f 7065 702d 3034 3837 2f3e  n.org/pep-0487/>
+00000bb0: 605f 3a20 5375 7070 6f72 7420 666f 7220  `_: Support for 
+00000bc0: 605f 5f69 6e69 745f 7375 6263 6c61 7373  `__init_subclass
+00000bd0: 5f5f 6020 616e 6420 605f 5f73 6574 5f6e  __` and `__set_n
+00000be0: 616d 655f 5f60 2e0a 2020 2020 5365 6520  ame__`..    See 
+00000bf0: 616c 736f 2060 696e 6974 5f73 7562 636c  also `init_subcl
+00000c00: 6173 7360 5f20 616e 6420 6073 6574 5f6e  ass`_ and `set_n
+00000c10: 616d 6560 5f2e 0a20 202d 2060 6f62 6a65  ame`_..  - `obje
+00000c20: 6374 2e5f 5f64 6972 5f5f 203c 6874 7470  ct.__dir__ <http
+00000c30: 733a 2f2f 646f 6373 2e70 7974 686f 6e2e  s://docs.python.
+00000c40: 6f72 672f 332f 7265 6665 7265 6e63 652f  org/3/reference/
+00000c50: 6461 7461 6d6f 6465 6c2e 6874 6d6c 236f  datamodel.html#o
+00000c60: 626a 6563 742e 5f5f 6469 725f 5f3e 605f  bject.__dir__>`_
+00000c70: 3a20 4261 7365 2060 5f5f 6469 725f 5f60  : Base `__dir__`
+00000c80: 206d 6574 686f 642e 0a20 2020 2053 6565   method..    See
+00000c90: 2061 6c73 6f20 6064 6566 6175 6c74 5f64   also `default_d
+00000ca0: 6972 605f 2e0a 2020 2d20 605f 5f65 715f  ir`_..  - `__eq_
+00000cb0: 5f20 6f76 6572 7269 6465 203c 6874 7470  _ override <http
+00000cc0: 733a 2f2f 646f 6373 2e70 7974 686f 6e2e  s://docs.python.
+00000cd0: 6f72 672f 332f 7265 6665 7265 6e63 652f  org/3/reference/
+00000ce0: 6461 7461 6d6f 6465 6c2e 6874 6d6c 236f  datamodel.html#o
+00000cf0: 626a 6563 742e 5f5f 6861 7368 5f5f 3e60  bject.__hash__>`
+00000d00: 5f3a 204f 7665 7272 6964 696e 6720 605f  _: Overriding `_
+00000d10: 5f65 715f 5f60 2077 696c 6c0a 2020 2020  _eq__` will.    
+00000d20: 7365 7420 605f 5f68 6173 685f 5f60 2074  set `__hash__` t
+00000d30: 6f20 4e6f 6e65 2e20 5365 6520 616c 736f  o None. See also
+00000d40: 2060 696d 706c 6963 6974 5f68 6173 6860   `implicit_hash`
+00000d50: 5f2e 0a20 202d 2060 5045 5020 3330 3720  _..  - `PEP 307 
+00000d60: 3c68 7474 7073 3a2f 2f70 6570 732e 7079  <https://peps.py
+00000d70: 7468 6f6e 2e6f 7267 2f70 6570 2d30 3330  thon.org/pep-030
+00000d80: 372f 3e60 5f3a 2053 7570 706f 7274 2066  7/>`_: Support f
+00000d90: 6f72 2070 6963 6b6c 696e 6720 6f62 6a65  or pickling obje
+00000da0: 6374 7320 7769 7468 2060 5f5f 736c 6f74  cts with `__slot
+00000db0: 735f 5f60 2e0a 2020 2020 5365 6520 616c  s__`..    See al
+00000dc0: 736f 2060 6f62 6a5f 7374 6174 6560 5f2e  so `obj_state`_.
+00000dd0: 0a20 202d 2060 5045 5020 3331 3535 203c  .  - `PEP 3155 <
+00000de0: 6874 7470 733a 2f2f 7065 7073 2e70 7974  https://peps.pyt
+00000df0: 686f 6e2e 6f72 672f 7065 702d 3033 3135  hon.org/pep-0315
+00000e00: 352f 3e60 5f3a 2051 7561 6c69 6669 6564  5/>`_: Qualified
+00000e10: 206e 616d 6520 605f 5f71 7561 6c6e 616d   name `__qualnam
+00000e20: 655f 5f60 2066 6f72 206e 6573 7465 6420  e__` for nested 
+00000e30: 636c 6173 7365 732e 0a20 2020 2053 6565  classes..    See
+00000e40: 2061 6c73 6f20 6071 7561 6c6e 616d 6560   also `qualname`
+00000e50: 5f2e 0a20 202d 2060 5f5f 6e65 5f5f 2062  _..  - `__ne__ b
+00000e60: 6568 6176 696f 7220 3c68 7474 7073 3a2f  ehavior <https:/
+00000e70: 2f64 6f63 732e 7079 7468 6f6e 2e6f 7267  /docs.python.org
+00000e80: 2f33 2e30 2f77 6861 7473 6e65 772f 332e  /3.0/whatsnew/3.
+00000e90: 302e 6874 6d6c 236f 7065 7261 746f 7273  0.html#operators
+00000ea0: 2d61 6e64 2d73 7065 6369 616c 2d6d 6574  -and-special-met
+00000eb0: 686f 6473 3e60 5f3a 2042 7920 6465 6661  hods>`_: By defa
+00000ec0: 756c 742c 0a20 2020 2060 5f5f 6e65 5f5f  ult,.    `__ne__
+00000ed0: 6020 7368 6f75 6c64 206e 6567 6174 6520  ` should negate 
+00000ee0: 7468 6520 7265 7375 6c74 206f 6620 605f  the result of `_
+00000ef0: 5f65 715f 5f60 2e0a 2020 2020 5365 6520  _eq__`..    See 
+00000f00: 616c 736f 2060 7361 6665 5f6e 6f74 5f65  also `safe_not_e
+00000f10: 7175 616c 7360 5f0a 2020 2d20 6050 4550  quals`_.  - `PEP
+00000f20: 2030 3536 3020 3c68 7474 7073 3a2f 2f70   0560 <https://p
+00000f30: 6570 732e 7079 7468 6f6e 2e6f 7267 2f70  eps.python.org/p
+00000f40: 6570 2d30 3536 302f 3e60 5f3a 2042 6574  ep-0560/>`_: Bet
+00000f50: 7465 7220 6861 6e64 6c69 6e67 206f 6620  ter handling of 
+00000f60: 4765 6e65 7269 6320 636c 6173 7365 732e  Generic classes.
+00000f70: 0a20 2020 2053 6565 2061 6c73 6f20 6074  .    See also `t
+00000f80: 6970 706f 203c 6874 7470 733a 2f2f 6769  ippo <https://gi
+00000f90: 7468 7562 2e63 6f6d 2f62 7275 6e6f 6e69  thub.com/brunoni
+00000fa0: 636b 6f2f 7469 7070 6f23 6765 6e65 7269  cko/tippo#generi
+00000fb0: 632d 6669 7865 733e 605f 2e0a 0a42 6173  c-fixes>`_...Bas
+00000fc0: 650a 5e5e 5e5e 0a49 6e20 6164 6469 7469  e.^^^^.In additi
+00000fd0: 6f6e 2074 6f20 7468 6520 636f 6d70 6174  on to the compat
+00000fe0: 6962 696c 6974 7920 736f 6c75 7469 6f6e  ibility solution
+00000ff0: 732c 2074 6865 2067 6f61 6c20 7769 7468  s, the goal with
+00001000: 2074 6865 2060 4261 7365 4d65 7461 6020   the `BaseMeta` 
+00001010: 6d65 7461 636c 6173 7320 616e 6420 7468  metaclass and th
+00001020: 6520 6042 6173 6560 2063 6c61 7373 2069  e `Base` class i
+00001030: 7320 746f 2061 6464 0a75 7365 6675 6c20  s to add.useful 
+00001040: 6c6f 772d 6c65 7665 6c20 6665 6174 7572  low-level featur
+00001050: 6573 2074 6861 7420 686f 7065 6675 6c6c  es that hopefull
+00001060: 7920 7969 656c 6420 6265 7474 6572 2063  y yield better c
+00001070: 6f64 6520 7265 6164 6162 696c 6974 7920  ode readability 
+00001080: 616e 6420 7661 6c69 6461 7469 6f6e 2e0a  and validation..
+00001090: 0a54 6869 7320 696e 636c 7564 6573 3a0a  .This includes:.
+000010a0: 2020 2d20 605f 5f77 6561 6b72 6566 5f5f    - `__weakref__
+000010b0: 6020 736c 6f74 3a20 4164 6465 6420 6279  ` slot: Added by
+000010c0: 2064 6566 6175 6c74 2e0a 2020 2d20 606c   default..  - `l
+000010d0: 6f63 6b65 645f 636c 6173 7360 5f3a 2050  ocked_class`_: P
+000010e0: 7562 6c69 6320 636c 6173 7320 6174 7472  ublic class attr
+000010f0: 6962 7574 6573 2061 7265 2072 6561 642d  ibutes are read-
+00001100: 6f6e 6c79 2062 7920 6465 6661 756c 742e  only by default.
+00001110: 0a20 202d 2060 6578 706c 6963 6974 5f68  .  - `explicit_h
+00001120: 6173 6860 5f3a 204f 7665 7272 6964 696e  ash`_: Overridin
+00001130: 6720 605f 5f65 715f 5f60 2077 6974 686f  g `__eq__` witho
+00001140: 7574 206f 7665 7272 6964 696e 6720 605f  ut overriding `_
+00001150: 5f68 6173 685f 5f60 2077 696c 6c20 7261  _hash__` will ra
+00001160: 6973 6520 616e 2065 7272 6f72 2e0a 2020  ise an error..  
+00001170: 2d20 606e 616d 6573 7061 6365 605f 3a20  - `namespace`_: 
+00001180: 4164 6473 2061 2070 726f 7465 6374 6564  Adds a protected
+00001190: 2060 5f5f 6e61 6d65 7370 6163 6560 2075   `__namespace` u
+000011a0: 6e69 7175 6520 746f 2065 6163 6820 636c  nique to each cl
+000011b0: 6173 732e 0a20 202d 2060 7275 6e74 696d  ass..  - `runtim
+000011c0: 655f 6669 6e61 6c60 5f3a 2052 756e 7469  e_final`_: Runti
+000011d0: 6d65 2063 6865 636b 696e 6720 666f 7220  me checking for 
+000011e0: 636c 6173 7365 7320 616e 6420 6d65 7468  classes and meth
+000011f0: 6f64 7320 6465 636f 7261 7465 6420 7769  ods decorated wi
+00001200: 7468 2060 6669 6e61 6c60 2e0a 0a53 6c6f  th `final`...Slo
+00001210: 7474 6564 4261 7365 0a5e 5e5e 5e5e 5e5e  ttedBase.^^^^^^^
+00001220: 5e5e 5e5e 0a54 6865 2060 536c 6f74 7465  ^^^^.The `Slotte
+00001230: 6442 6173 6560 2063 6c61 7373 2061 6e64  dBase` class and
+00001240: 2074 6865 2060 536c 6f74 7465 6442 6173   the `SlottedBas
+00001250: 654d 6574 6160 206d 6574 6163 6c61 7373  eMeta` metaclass
+00001260: 206f 6666 6572 2061 6c6c 2066 6561 7475   offer all featu
+00001270: 7265 7320 6672 6f6d 2060 4261 7365 6020  res from `Base` 
+00001280: 616e 6420 6042 6173 654d 6574 6160 2070  and `BaseMeta` p
+00001290: 6c75 7320 696d 706c 6963 6974 0a60 5f5f  lus implicit.`__
+000012a0: 736c 6f74 735f 5f60 2064 6563 6c61 7261  slots__` declara
+000012b0: 7469 6f6e 2e20 5365 6520 6073 6c6f 7474  tion. See `slott
+000012c0: 6564 203c 6874 7470 733a 2f2f 6769 7468  ed <https://gith
+000012d0: 7562 2e63 6f6d 2f62 7275 6e6f 6e69 636b  ub.com/brunonick
+000012e0: 6f2f 736c 6f74 7465 643e 605f 2066 6f72  o/slotted>`_ for
+000012f0: 206d 6f72 6520 696e 666f 726d 6174 696f   more informatio
+00001300: 6e2e 0a0a 5574 696c 6974 6965 730a 2d2d  n...Utilities.--
+00001310: 2d2d 2d2d 2d2d 2d0a 4170 6172 7420 6672  -------.Apart fr
+00001320: 6f6d 2074 6865 2066 6561 7475 7265 7320  om the features 
+00001330: 696e 7465 6772 6174 6564 2069 6e74 6f20  integrated into 
+00001340: 7468 6520 6261 7365 2063 6c61 7373 6573  the base classes
+00001350: 2c20 6062 6173 6963 636f 6020 7072 6f76  , `basicco` prov
+00001360: 6964 6573 206d 616e 7920 6765 6e65 7261  ides many genera
+00001370: 6c20 7574 696c 6974 7920 6d6f 6475 6c65  l utility module
+00001380: 732e 0a0a 6162 7374 7261 6374 5f63 6c61  s...abstract_cla
+00001390: 7373 0a5e 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e  ss.^^^^^^^^^^^^^
+000013a0: 5e0a 4265 7474 6572 2060 6162 7374 7261  ^.Better `abstra
+000013b0: 6374 2063 6c61 7373 6573 203c 6874 7470  ct classes <http
+000013c0: 733a 2f2f 646f 6373 2e70 7974 686f 6e2e  s://docs.python.
+000013d0: 6f72 672f 332f 6c69 6272 6172 792f 6162  org/3/library/ab
+000013e0: 632e 6874 6d6c 2361 6263 2e61 6273 7472  c.html#abc.abstr
+000013f0: 6163 746d 6574 686f 643e 605f 2073 7570  actmethod>`_ sup
+00001400: 706f 7274 2e0a 0a50 726f 7669 6465 7320  port...Provides 
+00001410: 6162 7374 7261 6374 2064 6563 6f72 6174  abstract decorat
+00001420: 6f72 7320 7468 6174 2063 616e 2062 6520  ors that can be 
+00001430: 7573 6564 2064 6972 6563 746c 7920 6f6e  used directly on
+00001440: 206d 6574 686f 6473 2062 7574 2061 6c73   methods but als
+00001450: 6f20 6f6e 2063 6c61 7373 6573 2c20 7072  o on classes, pr
+00001460: 6f70 6572 7469 6573 2c20 636c 6173 736d  operties, classm
+00001470: 6574 686f 6473 2c20 616e 640a 7374 6174  ethods, and.stat
+00001480: 6963 6d65 7468 6f64 7320 2865 7665 6e20  icmethods (even 
+00001490: 696e 2050 7974 686f 6e20 322e 3729 2e0a  in Python 2.7)..
+000014a0: 0a2e 2e20 636f 6465 3a3a 2070 7974 686f  ... code:: pytho
+000014b0: 6e0a 0a20 2020 203e 3e3e 2066 726f 6d20  n..    >>> from 
+000014c0: 7369 7820 696d 706f 7274 2077 6974 685f  six import with_
+000014d0: 6d65 7461 636c 6173 730a 2020 2020 3e3e  metaclass.    >>
+000014e0: 3e20 6672 6f6d 2062 6173 6963 636f 2e61  > from basicco.a
+000014f0: 6273 7472 6163 745f 636c 6173 7320 696d  bstract_class im
+00001500: 706f 7274 2041 6273 7472 6163 744d 6574  port AbstractMet
+00001510: 612c 2061 6273 7472 6163 740a 2020 2020  a, abstract.    
+00001520: 3e3e 3e20 636c 6173 7320 4173 7365 7428  >>> class Asset(
+00001530: 7769 7468 5f6d 6574 6163 6c61 7373 2841  with_metaclass(A
+00001540: 6273 7472 6163 744d 6574 612c 206f 626a  bstractMeta, obj
+00001550: 6563 7429 293a 0a20 2020 202e 2e2e 2020  ect)):.    ...  
+00001560: 2020 2040 6162 7374 7261 6374 0a20 2020     @abstract.   
+00001570: 202e 2e2e 2020 2020 2064 6566 206d 6574   ...     def met
+00001580: 686f 6428 7365 6c66 293a 0a20 2020 202e  hod(self):.    .
+00001590: 2e2e 2020 2020 2020 2020 2070 6173 730a  ..         pass.
+000015a0: 2020 2020 2e2e 2e0a 2020 2020 2e2e 2e20      ....    ... 
+000015b0: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
+000015c0: 2020 2e2e 2e20 2020 2020 4061 6273 7472    ...     @abstr
+000015d0: 6163 740a 2020 2020 2e2e 2e20 2020 2020  act.    ...     
+000015e0: 6465 6620 7072 6f70 2873 656c 6629 3a0a  def prop(self):.
+000015f0: 2020 2020 2e2e 2e20 2020 2020 2020 2020      ...         
+00001600: 7265 7475 726e 204e 6f6e 650a 2020 2020  return None.    
+00001610: 2e2e 2e0a 2020 2020 3e3e 3e20 4173 7365  ....    >>> Asse
+00001620: 7428 290a 2020 2020 5472 6163 6562 6163  t().    Tracebac
+00001630: 6b20 286d 6f73 7420 7265 6365 6e74 2063  k (most recent c
+00001640: 616c 6c20 6c61 7374 293a 0a20 2020 2054  all last):.    T
+00001650: 7970 6545 7272 6f72 3a20 4361 6e27 7420  ypeError: Can't 
+00001660: 696e 7374 616e 7469 6174 6520 6162 7374  instantiate abst
+00001670: 7261 6374 2063 6c61 7373 2041 7373 6574  ract class Asset
+00001680: 2077 6974 6820 6162 7374 7261 6374 206d   with abstract m
+00001690: 6574 686f 6473 206d 6574 686f 642c 2070  ethods method, p
+000016a0: 726f 700a 0a2e 2e20 636f 6465 3a3a 2070  rop.... code:: p
+000016b0: 7974 686f 6e0a 0a20 2020 203e 3e3e 2066  ython..    >>> f
+000016c0: 726f 6d20 6261 7369 6363 6f2e 6162 7374  rom basicco.abst
+000016d0: 7261 6374 5f63 6c61 7373 2069 6d70 6f72  ract_class impor
+000016e0: 7420 4162 7374 7261 6374 4d65 7461 2c20  t AbstractMeta, 
+000016f0: 6162 7374 7261 6374 0a20 2020 203e 3e3e  abstract.    >>>
+00001700: 2040 6162 7374 7261 6374 0a20 2020 202e   @abstract.    .
+00001710: 2e2e 2063 6c61 7373 2041 7373 6574 2877  .. class Asset(w
+00001720: 6974 685f 6d65 7461 636c 6173 7328 4162  ith_metaclass(Ab
+00001730: 7374 7261 6374 4d65 7461 2c20 6f62 6a65  stractMeta, obje
+00001740: 6374 2929 3a0a 2020 2020 2e2e 2e20 2020  ct)):.    ...   
+00001750: 2020 7061 7373 0a20 2020 202e 2e2e 0a20    pass.    .... 
+00001760: 2020 203e 3e3e 2041 7373 6574 2829 0a20     >>> Asset(). 
+00001770: 2020 2054 7261 6365 6261 636b 2028 6d6f     Traceback (mo
+00001780: 7374 2072 6563 656e 7420 6361 6c6c 206c  st recent call l
+00001790: 6173 7429 3a0a 2020 2020 5479 7065 4572  ast):.    TypeEr
+000017a0: 726f 723a 2063 616e 2774 2069 6e73 7461  ror: can't insta
+000017b0: 6e74 6961 7465 2061 6273 7472 6163 7420  ntiate abstract 
+000017c0: 636c 6173 7320 2741 7373 6574 270a 0a63  class 'Asset'..c
+000017d0: 616c 6c65 725f 6d6f 6475 6c65 0a5e 5e5e  aller_module.^^^
+000017e0: 5e5e 5e5e 5e5e 5e5e 5e5e 0a52 6574 7269  ^^^^^^^^^^.Retri
+000017f0: 6576 6520 7468 6520 6361 6c6c 6572 2773  eve the caller's
+00001800: 206d 6f64 756c 6520 6e61 6d65 2e0a 0a2e   module name....
+00001810: 2e20 636f 6465 3a3a 2070 7974 686f 6e0a  . code:: python.
+00001820: 0a20 2020 203e 3e3e 2066 726f 6d20 6261  .    >>> from ba
+00001830: 7369 6363 6f2e 6361 6c6c 6572 5f6d 6f64  sicco.caller_mod
+00001840: 756c 6520 696d 706f 7274 2063 616c 6c65  ule import calle
+00001850: 725f 6d6f 6475 6c65 0a20 2020 203e 3e3e  r_module.    >>>
+00001860: 2064 6566 2064 6f5f 736f 6d65 7468 696e   def do_somethin
+00001870: 6728 293a 0a20 2020 202e 2e2e 2020 2020  g():.    ...    
+00001880: 2072 6574 7572 6e20 2249 2077 6173 2063   return "I was c
+00001890: 616c 6c65 6420 6279 207b 7d22 2e66 6f72  alled by {}".for
+000018a0: 6d61 7428 6361 6c6c 6572 5f6d 6f64 756c  mat(caller_modul
+000018b0: 6528 2929 0a20 2020 202e 2e2e 0a20 2020  e()).    ....   
+000018c0: 203e 3e3e 2064 6f5f 736f 6d65 7468 696e   >>> do_somethin
+000018d0: 6728 290a 2020 2020 2749 2077 6173 2063  g().    'I was c
+000018e0: 616c 6c65 6420 6279 205f 5f6d 6169 6e5f  alled by __main_
+000018f0: 5f27 0a0a 636f 6e74 6578 745f 7661 7273  _'..context_vars
+00001900: 0a5e 5e5e 5e5e 5e5e 5e5e 5e5e 5e0a 4261  .^^^^^^^^^^^^.Ba
+00001910: 636b 706f 7274 206f 6620 7468 6520 6063  ckport of the `c
+00001920: 6f6e 7465 7874 7661 7273 6020 6d6f 6475  ontextvars` modu
+00001930: 6c65 2066 6f72 2050 7974 686f 6e20 322e  le for Python 2.
+00001940: 372c 2062 6173 6564 206f 6e0a 604d 6167  7, based on.`Mag
+00001950: 6963 5374 6163 6b2f 636f 6e74 6578 7476  icStack/contextv
+00001960: 6172 7320 3c68 7474 7073 3a2f 2f67 6974  ars <https://git
+00001970: 6875 622e 636f 6d2f 4d61 6769 6353 7461  hub.com/MagicSta
+00001980: 636b 2f63 6f6e 7465 7874 7661 7273 3e60  ck/contextvars>`
+00001990: 5f2e 0a0a 5768 656e 2069 6d70 6f72 7465  _...When importe
+000019a0: 6420 6672 6f6d 2050 7974 686f 6e20 332c  d from Python 3,
+000019b0: 2069 7420 7369 6d70 6c79 2072 6564 6972   it simply redir
+000019c0: 6563 7473 2074 6f20 7468 6520 6e61 7469  ects to the nati
+000019d0: 7665 0a60 636f 6e74 6578 7476 6172 7320  ve.`contextvars 
+000019e0: 3c68 7474 7073 3a2f 2f64 6f63 732e 7079  <https://docs.py
+000019f0: 7468 6f6e 2e6f 7267 2f33 2f6c 6962 7261  thon.org/3/libra
+00001a00: 7279 2f63 6f6e 7465 7874 7661 7273 2e68  ry/contextvars.h
+00001a10: 746d 6c3e 605f 206d 6f64 756c 652e 0a0a  tml>`_ module...
+00001a20: 2e2e 2063 6f64 653a 3a20 7079 7468 6f6e  .. code:: python
+00001a30: 0a0a 2020 2020 3e3e 3e20 6672 6f6d 2062  ..    >>> from b
+00001a40: 6173 6963 636f 2e63 6f6e 7465 7874 5f76  asicco.context_v
+00001a50: 6172 7320 696d 706f 7274 2043 6f6e 7465  ars import Conte
+00001a60: 7874 5661 720a 2020 2020 3e3e 3e20 6d79  xtVar.    >>> my
+00001a70: 5f76 6172 203d 2043 6f6e 7465 7874 5661  _var = ContextVa
+00001a80: 7228 226d 795f 7661 7222 2c20 6465 6661  r("my_var", defa
+00001a90: 756c 743d 2262 6172 2229 0a20 2020 203e  ult="bar").    >
+00001aa0: 3e3e 2074 6f6b 656e 203d 206d 795f 7661  >> token = my_va
+00001ab0: 722e 7365 7428 2266 6f6f 2229 0a20 2020  r.set("foo").   
+00001ac0: 203e 3e3e 206d 795f 7661 722e 6765 7428   >>> my_var.get(
+00001ad0: 290a 2020 2020 2766 6f6f 270a 2020 2020  ).    'foo'.    
+00001ae0: 3e3e 3e20 6d79 5f76 6172 2e72 6573 6574  >>> my_var.reset
+00001af0: 2874 6f6b 656e 290a 2020 2020 3e3e 3e20  (token).    >>> 
+00001b00: 6d79 5f76 6172 2e67 6574 2829 0a20 2020  my_var.get().   
+00001b10: 2027 6261 7227 0a0a 6375 7374 6f6d 5f72   'bar'..custom_r
+00001b20: 6570 720a 5e5e 5e5e 5e5e 5e5e 5e5e 5e0a  epr.^^^^^^^^^^^.
+00001b30: 4375 7374 6f6d 2072 6570 7265 7365 6e74  Custom represent
+00001b40: 6174 696f 6e20 6675 6e63 7469 6f6e 7320  ation functions 
+00001b50: 666f 7220 6d61 7070 696e 6773 2c20 6974  for mappings, it
+00001b60: 656d 732c 2061 6e64 2069 7465 7261 626c  ems, and iterabl
+00001b70: 6573 2e0a 0a2e 2e20 636f 6465 3a3a 2070  es..... code:: p
+00001b80: 7974 686f 6e0a 0a20 2020 203e 3e3e 2066  ython..    >>> f
+00001b90: 726f 6d20 6261 7369 6363 6f2e 6375 7374  rom basicco.cust
+00001ba0: 6f6d 5f72 6570 7220 696d 706f 7274 206d  om_repr import m
+00001bb0: 6170 7069 6e67 5f72 6570 720a 2020 2020  apping_repr.    
+00001bc0: 3e3e 3e20 6463 7420 3d20 7b22 6122 3a20  >>> dct = {"a": 
+00001bd0: 312c 2022 6222 3a20 327d 0a20 2020 203e  1, "b": 2}.    >
+00001be0: 3e3e 206d 6170 7069 6e67 5f72 6570 7228  >> mapping_repr(
+00001bf0: 6463 742c 2070 7265 6669 783d 223c 222c  dct, prefix="<",
+00001c00: 2073 7566 6669 783d 223e 222c 2074 656d   suffix=">", tem
+00001c10: 706c 6174 653d 227b 6b65 797d 3d7b 7661  plate="{key}={va
+00001c20: 6c75 657d 222c 2073 6f72 7469 6e67 3d54  lue}", sorting=T
+00001c30: 7275 6529 0a20 2020 2022 3c27 6127 3d31  rue).    "<'a'=1
+00001c40: 2c20 2762 273d 323e 220a 0a2e 2e20 636f  , 'b'=2>".... co
+00001c50: 6465 3a3a 2070 7974 686f 6e0a 0a20 2020  de:: python..   
+00001c60: 203e 3e3e 2066 726f 6d20 6261 7369 6363   >>> from basicc
+00001c70: 6f2e 6375 7374 6f6d 5f72 6570 7220 696d  o.custom_repr im
+00001c80: 706f 7274 206d 6170 7069 6e67 5f72 6570  port mapping_rep
+00001c90: 720a 2020 2020 3e3e 3e20 6974 656d 7320  r.    >>> items 
+00001ca0: 3d20 5b28 2261 222c 2031 292c 2028 2262  = [("a", 1), ("b
+00001cb0: 222c 2032 295d 0a20 2020 203e 3e3e 206d  ", 2)].    >>> m
+00001cc0: 6170 7069 6e67 5f72 6570 7228 6974 656d  apping_repr(item
+00001cd0: 732c 2070 7265 6669 783d 225b 222c 2073  s, prefix="[", s
+00001ce0: 7566 6669 783d 225d 222c 2074 656d 706c  uffix="]", templ
+00001cf0: 6174 653d 6c61 6d62 6461 2069 2c20 6b65  ate=lambda i, ke
+00001d00: 792c 2076 616c 7565 3a20 6b65 7920 2b20  y, value: key + 
+00001d10: 2220 2d3e 2022 202b 2076 616c 7565 290a  " -> " + value).
+00001d20: 2020 2020 225b 2761 2720 2d3e 2031 2c20      "['a' -> 1, 
+00001d30: 2762 2720 2d3e 2032 5d22 0a0a 2e2e 2063  'b' -> 2]".... c
+00001d40: 6f64 653a 3a20 7079 7468 6f6e 0a0a 2020  ode:: python..  
+00001d50: 2020 3e3e 3e20 6672 6f6d 2062 6173 6963    >>> from basic
+00001d60: 636f 2e63 7573 746f 6d5f 7265 7072 2069  co.custom_repr i
+00001d70: 6d70 6f72 7420 6974 6572 6162 6c65 5f72  mport iterable_r
+00001d80: 6570 720a 2020 2020 3e3e 3e20 7475 7020  epr.    >>> tup 
+00001d90: 3d20 2822 6122 2c20 2262 222c 2022 6322  = ("a", "b", "c"
+00001da0: 2c20 312c 2032 2c20 3329 0a20 2020 203e  , 1, 2, 3).    >
+00001db0: 3e3e 2069 7465 7261 626c 655f 7265 7072  >> iterable_repr
+00001dc0: 2874 7570 2c20 7072 6566 6978 3d22 3c22  (tup, prefix="<"
+00001dd0: 2c20 7375 6666 6978 3d22 3e22 2c20 7661  , suffix=">", va
+00001de0: 6c75 655f 7265 7072 3d73 7472 290a 2020  lue_repr=str).  
+00001df0: 2020 273c 612c 2062 2c20 632c 2031 2c20    '<a, b, c, 1, 
+00001e00: 322c 2033 3e27 0a0a 6461 7461 5f63 6c61  2, 3>'..data_cla
+00001e10: 7373 0a5e 5e5e 5e5e 5e5e 5e5e 5e0a 5079  ss.^^^^^^^^^^.Py
+00001e20: 7468 6f6e 2032 2e37 2063 6f6d 7061 7469  thon 2.7 compati
+00001e30: 626c 6520 6461 7461 636c 6173 732d 6c69  ble dataclass-li
+00001e40: 6b65 2073 7472 7563 7475 7265 732e 0a0a  ke structures...
+00001e50: 2e2e 2063 6f64 653a 3a20 7079 7468 6f6e  .. code:: python
+00001e60: 0a0a 2020 2020 3e3e 3e20 6672 6f6d 206d  ..    >>> from m
+00001e70: 6174 6820 696d 706f 7274 2073 7172 740a  ath import sqrt.
+00001e80: 2020 2020 3e3e 3e20 6672 6f6d 2062 6173      >>> from bas
+00001e90: 6963 636f 2e64 6174 615f 636c 6173 7320  icco.data_class 
+00001ea0: 696d 706f 7274 2044 6174 6143 6c61 7373  import DataClass
+00001eb0: 2c20 6669 656c 640a 2020 2020 3e3e 3e20  , field.    >>> 
+00001ec0: 636c 6173 7320 5665 6374 6f72 2844 6174  class Vector(Dat
+00001ed0: 6143 6c61 7373 293a 0a20 2020 202e 2e2e  aClass):.    ...
+00001ee0: 2020 2020 2078 203d 2066 6965 6c64 2829       x = field()
+00001ef0: 2020 2320 7479 7065 3a20 666c 6f61 740a    # type: float.
+00001f00: 2020 2020 2e2e 2e20 2020 2020 7920 3d20      ...     y = 
+00001f10: 6669 656c 6428 2920 2023 2074 7970 653a  field()  # type:
+00001f20: 2066 6c6f 6174 0a20 2020 202e 2e2e 2020   float.    ...  
+00001f30: 2020 2040 7072 6f70 6572 7479 0a20 2020     @property.   
+00001f40: 202e 2e2e 2020 2020 2040 6669 656c 640a   ...     @field.
+00001f50: 2020 2020 2e2e 2e20 2020 2020 6465 6620      ...     def 
+00001f60: 6d61 6728 7365 6c66 293a 0a20 2020 202e  mag(self):.    .
+00001f70: 2e2e 2020 2020 2020 2020 2072 6574 7572  ..         retur
+00001f80: 6e20 7371 7274 2873 656c 662e 782a 2a32  n sqrt(self.x**2
+00001f90: 202b 2073 656c 662e 792a 2a32 290a 2020   + self.y**2).  
+00001fa0: 2020 2e2e 2e0a 2020 2020 3e3e 3e20 5665    ....    >>> Ve
+00001fb0: 6374 6f72 2833 2e30 2c20 342e 3029 0a20  ctor(3.0, 4.0). 
+00001fc0: 2020 2056 6563 746f 7228 332e 302c 2034     Vector(3.0, 4
+00001fd0: 2e30 2c20 6d61 673d 352e 3029 0a0a 6465  .0, mag=5.0)..de
+00001fe0: 6661 756c 745f 6469 720a 5e5e 5e5e 5e5e  fault_dir.^^^^^^
+00001ff0: 5e5e 5e5e 5e0a 4261 636b 706f 7274 206f  ^^^^^.Backport o
+00002000: 6620 5079 7468 6f6e 2033 2773 2069 6d70  f Python 3's imp
+00002010: 6c65 6d65 6e74 6174 696f 6e20 6f66 0a60  lementation of.`
+00002020: 6f62 6a65 6374 2e5f 5f64 6972 5f5f 203c  object.__dir__ <
+00002030: 6874 7470 733a 2f2f 646f 6373 2e70 7974  https://docs.pyt
+00002040: 686f 6e2e 6f72 672f 332f 7265 6665 7265  hon.org/3/refere
+00002050: 6e63 652f 6461 7461 6d6f 6465 6c2e 6874  nce/datamodel.ht
+00002060: 6d6c 236f 626a 6563 742e 5f5f 6469 725f  ml#object.__dir_
+00002070: 5f3e 605f 2066 6f72 2050 7974 686f 6e20  _>`_ for Python 
+00002080: 322e 372e 0a0a 5468 6973 2061 6c6c 6f77  2.7...This allow
+00002090: 7320 666f 7220 6361 6c6c 696e 6720 6073  s for calling `s
+000020a0: 7570 6572 2829 2e5f 5f64 6972 5f5f 2829  uper().__dir__()
+000020b0: 6020 6672 6f6d 2061 2073 7562 636c 6173  ` from a subclas
+000020c0: 7320 746f 206c 6576 6572 6167 6520 7468  s to leverage th
+000020d0: 6520 6465 6661 756c 7420 696d 706c 656d  e default implem
+000020e0: 656e 7461 7469 6f6e 2e0a 0a2e 2e20 636f  entation..... co
+000020f0: 6465 3a3a 2070 7974 686f 6e0a 0a20 2020  de:: python..   
+00002100: 203e 3e3e 2066 726f 6d20 7369 7820 696d   >>> from six im
+00002110: 706f 7274 2077 6974 685f 6d65 7461 636c  port with_metacl
+00002120: 6173 730a 2020 2020 3e3e 3e20 6672 6f6d  ass.    >>> from
+00002130: 2062 6173 6963 636f 2e64 6566 6175 6c74   basicco.default
+00002140: 5f64 6972 2069 6d70 6f72 7420 4465 6661  _dir import Defa
+00002150: 756c 7444 6972 0a20 2020 203e 3e3e 2063  ultDir.    >>> c
+00002160: 6c61 7373 2043 6c61 7373 2844 6566 6175  lass Class(Defau
+00002170: 6c74 4469 7229 3a0a 2020 2020 2e2e 2e20  ltDir):.    ... 
+00002180: 2020 2020 6465 6620 5f5f 6469 725f 5f28      def __dir__(
+00002190: 7365 6c66 293a 0a20 2020 202e 2e2e 2020  self):.    ...  
+000021a0: 2020 2020 2020 2072 6574 7572 6e20 7375         return su
+000021b0: 7065 7228 436c 6173 732c 2073 656c 6629  per(Class, self)
+000021c0: 2e5f 5f64 6972 5f5f 2829 0a20 2020 202e  .__dir__().    .
+000021d0: 2e2e 0a20 2020 203e 3e3e 206f 626a 203d  ...    >>> obj =
+000021e0: 2043 6c61 7373 2829 0a20 2020 203e 3e3e   Class().    >>>
+000021f0: 2064 6972 286f 626a 290a 2020 2020 5b2e   dir(obj).    [.
+00002200: 2e2e 5d0a 0a64 796e 616d 6963 5f63 6c61  ..]..dynamic_cla
+00002210: 7373 0a5e 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e  ss.^^^^^^^^^^^^^
+00002220: 0a45 6173 696c 7920 6765 6e65 7261 7465  .Easily generate
+00002230: 2063 6c61 7373 6573 206f 6e20 7468 6520   classes on the 
+00002240: 666c 792e 2054 6869 7320 776f 726b 7320  fly. This works 
+00002250: 6265 7374 2077 6974 6820 6120 6042 6173  best with a `Bas
+00002260: 6560 5f20 636c 6173 732e 0a49 6620 7072  e`_ class..If pr
+00002270: 6f76 6964 6564 2061 2076 616c 6964 2071  ovided a valid q
+00002280: 7561 6c69 6669 6564 206e 616d 6520 616e  ualified name an
+00002290: 6420 6d6f 6475 6c65 2028 7573 6573 2060  d module (uses `
+000022a0: 6361 6c6c 6572 5f6d 6f64 756c 6560 5f20  caller_module`_ 
+000022b0: 6279 2064 6566 6175 6c74 292c 2074 6865  by default), the
+000022c0: 2063 6c61 7373 2077 696c 6c20 6265 2070   class will be p
+000022d0: 6963 6b61 626c 652f 696d 706f 7274 6162  ickable/importab
+000022e0: 6c65 2e0a 0a2e 2e20 636f 6465 3a3a 2070  le..... code:: p
+000022f0: 7974 686f 6e0a 0a20 2020 203e 3e3e 2066  ython..    >>> f
+00002300: 726f 6d20 6261 7369 6363 6f20 696d 706f  rom basicco impo
+00002310: 7274 2042 6173 650a 2020 2020 3e3e 3e20  rt Base.    >>> 
+00002320: 6672 6f6d 2062 6173 6963 636f 2e64 796e  from basicco.dyn
+00002330: 616d 6963 5f63 6c61 7373 2069 6d70 6f72  amic_class impor
+00002340: 7420 6d61 6b65 5f63 6c73 0a20 2020 203e  t make_cls.    >
+00002350: 3e3e 2063 6c61 7373 204d 7943 6c61 7373  >> class MyClass
+00002360: 286f 626a 6563 7429 3a0a 2020 2020 2e2e  (object):.    ..
+00002370: 2e20 2020 2020 4479 6e43 6c61 7373 203d  .     DynClass =
+00002380: 206d 616b 655f 636c 7328 224d 7943 6c61   make_cls("MyCla
+00002390: 7373 2e44 796e 436c 6173 7322 2c20 6261  ss.DynClass", ba
+000023a0: 7365 733d 2842 6173 652c 292c 2064 6374  ses=(Base,), dct
+000023b0: 3d7b 2266 6f6f 223a 2022 6261 7222 7d29  ={"foo": "bar"})
+000023c0: 0a20 2020 202e 2e2e 0a20 2020 203e 3e3e  .    ....    >>>
+000023d0: 2072 6570 7228 4d79 436c 6173 732e 4479   repr(MyClass.Dy
+000023e0: 6e43 6c61 7373 290a 2020 2020 223c 636c  nClass).    "<cl
+000023f0: 6173 7320 275f 5f6d 6169 6e5f 5f2e 4d79  ass '__main__.My
+00002400: 436c 6173 732e 4479 6e43 6c61 7373 273e  Class.DynClass'>
+00002410: 220a 0a64 796e 616d 6963 5f63 6f64 650a  "..dynamic_code.
+00002420: 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e 0a47 656e  ^^^^^^^^^^^^.Gen
+00002430: 6572 6174 6520 6465 6275 6767 6162 6c65  erate debuggable
+00002440: 2063 6f64 6520 6f6e 2074 6865 2066 6c79   code on the fly
+00002450: 2074 6861 7420 7375 7070 6f72 7473 206c   that supports l
+00002460: 696e 6520 6e75 6d62 6572 7320 6f6e 2074  ine numbers on t
+00002470: 7261 6365 6261 636b 732e 0a0a 2e2e 2063  racebacks..... c
+00002480: 6f64 653a 3a20 7079 7468 6f6e 0a0a 2020  ode:: python..  
+00002490: 2020 3e3e 3e20 6672 6f6d 2062 6173 6963    >>> from basic
+000024a0: 636f 2e64 796e 616d 6963 5f63 6f64 6520  co.dynamic_code 
+000024b0: 696d 706f 7274 206d 616b 655f 6675 6e63  import make_func
+000024c0: 7469 6f6e 2c20 6765 6e65 7261 7465 5f75  tion, generate_u
+000024d0: 6e69 7175 655f 6669 6c65 6e61 6d65 0a20  nique_filename. 
+000024e0: 2020 203e 3e3e 2063 6c61 7373 204d 7943     >>> class MyC
+000024f0: 6c61 7373 286f 626a 6563 7429 3a0a 2020  lass(object):.  
+00002500: 2020 2e2e 2e20 2020 2020 7061 7373 0a20    ...     pass. 
+00002510: 2020 202e 2e2e 0a20 2020 203e 3e3e 2062     ....    >>> b
+00002520: 6172 203d 2027 6261 7227 0a20 2020 203e  ar = 'bar'.    >
+00002530: 3e3e 2023 2050 7265 7061 7265 2074 6865  >> # Prepare the
+00002540: 2073 6372 6970 7420 616e 6420 6e65 6365   script and nece
+00002550: 7373 6172 7920 6461 7461 2e0a 2020 2020  ssary data..    
+00002560: 3e3e 3e20 7363 7269 7074 203d 2022 5c6e  >>> script = "\n
+00002570: 222e 6a6f 696e 280a 2020 2020 2e2e 2e20  ".join(.    ... 
+00002580: 2020 2020 280a 2020 2020 2e2e 2e20 2020      (.    ...   
+00002590: 2020 2020 2020 2264 6566 205f 5f69 6e69        "def __ini
+000025a0: 745f 5f28 7365 6c66 293a 222c 0a20 2020  t__(self):",.   
+000025b0: 202e 2e2e 2020 2020 2020 2020 2022 2020   ...         "  
+000025c0: 2020 7365 6c66 2e66 6f6f 203d 2027 6261    self.foo = 'ba
+000025d0: 7227 222c 0a20 2020 202e 2e2e 2020 2020  r'",.    ...    
+000025e0: 2029 0a20 2020 202e 2e2e 2029 0a20 2020   ).    ... ).   
+000025f0: 203e 3e3e 2023 2047 6174 6865 7220 696e   >>> # Gather in
+00002600: 666f 726d 6174 696f 6e2e 0a20 2020 203e  formation..    >
+00002610: 3e3e 206e 616d 6520 3d20 225f 5f69 6e69  >> name = "__ini
+00002620: 745f 5f22 0a20 2020 203e 3e3e 206f 776e  t__".    >>> own
+00002630: 6572 5f6e 616d 6520 3d20 4d79 436c 6173  er_name = MyClas
+00002640: 732e 5f5f 6e61 6d65 5f5f 0a20 2020 203e  s.__name__.    >
+00002650: 3e3e 206d 6f64 756c 6520 3d20 4d79 436c  >> module = MyCl
+00002660: 6173 732e 5f5f 6d6f 6475 6c65 5f5f 0a20  ass.__module__. 
+00002670: 2020 203e 3e3e 2066 696c 656e 616d 6520     >>> filename 
+00002680: 3d20 6765 6e65 7261 7465 5f75 6e69 7175  = generate_uniqu
+00002690: 655f 6669 6c65 6e61 6d65 286e 616d 652c  e_filename(name,
+000026a0: 206d 6f64 756c 652c 206f 776e 6572 5f6e   module, owner_n
+000026b0: 616d 6529 0a20 2020 203e 3e3e 2067 6c6f  ame).    >>> glo
+000026c0: 6273 203d 207b 2262 6172 223a 2062 6172  bs = {"bar": bar
+000026d0: 7d0a 2020 2020 3e3e 3e20 2320 4d61 6b65  }.    >>> # Make
+000026e0: 2066 756e 6374 696f 6e20 616e 6420 6174   function and at
+000026f0: 7461 6368 2069 7420 6173 2061 206d 6574  tach it as a met
+00002700: 686f 642e 0a20 2020 203e 3e3e 204d 7943  hod..    >>> MyC
+00002710: 6c61 7373 2e5f 5f69 6e69 745f 5f20 3d20  lass.__init__ = 
+00002720: 6d61 6b65 5f66 756e 6374 696f 6e28 6e61  make_function(na
+00002730: 6d65 2c20 7363 7269 7074 2c20 676c 6f62  me, script, glob
+00002740: 732c 2066 696c 656e 616d 652c 206d 6f64  s, filename, mod
+00002750: 756c 6529 0a20 2020 203e 3e3e 206f 626a  ule).    >>> obj
+00002760: 203d 204d 7943 6c61 7373 2829 0a20 2020   = MyClass().   
+00002770: 203e 3e3e 206f 626a 2e66 6f6f 0a20 2020   >>> obj.foo.   
+00002780: 2027 6261 7227 0a0a 6578 706c 6963 6974   'bar'..explicit
+00002790: 5f68 6173 680a 5e5e 5e5e 5e5e 5e5e 5e5e  _hash.^^^^^^^^^^
+000027a0: 5e5e 5e0a 4d65 7461 636c 6173 7320 7468  ^^^.Metaclass th
+000027b0: 6174 2066 6f72 6365 7320 605f 5f68 6173  at forces `__has
+000027c0: 685f 5f60 2074 6f20 6265 2064 6563 6c61  h__` to be decla
+000027d0: 7265 6420 7768 656e 6576 6572 2060 5f5f  red whenever `__
+000027e0: 6571 5f5f 6020 6973 2064 6563 6c61 7265  eq__` is declare
+000027f0: 642e 0a0a 2e2e 2063 6f64 653a 3a20 7079  d..... code:: py
+00002800: 7468 6f6e 0a0a 2020 2020 3e3e 3e20 6672  thon..    >>> fr
+00002810: 6f6d 2073 6978 2069 6d70 6f72 7420 7769  om six import wi
+00002820: 7468 5f6d 6574 6163 6c61 7373 0a20 2020  th_metaclass.   
+00002830: 203e 3e3e 2066 726f 6d20 6261 7369 6363   >>> from basicc
+00002840: 6f2e 6578 706c 6963 6974 5f68 6173 6820  o.explicit_hash 
+00002850: 696d 706f 7274 2045 7870 6c69 6369 7448  import ExplicitH
+00002860: 6173 684d 6574 610a 2020 2020 3e3e 3e20  ashMeta.    >>> 
+00002870: 636c 6173 7320 4173 7365 7428 7769 7468  class Asset(with
+00002880: 5f6d 6574 6163 6c61 7373 2845 7870 6c69  _metaclass(Expli
+00002890: 6369 7448 6173 684d 6574 612c 206f 626a  citHashMeta, obj
+000028a0: 6563 7429 293a 0a20 2020 202e 2e2e 2020  ect)):.    ...  
+000028b0: 2020 2064 6566 205f 5f65 715f 5f28 7365     def __eq__(se
+000028c0: 6c66 2c20 6f74 6865 7229 3a0a 2020 2020  lf, other):.    
+000028d0: 2e2e 2e20 2020 2020 2020 2020 7061 7373  ...         pass
+000028e0: 0a20 2020 202e 2e2e 0a20 2020 2054 7261  .    ....    Tra
+000028f0: 6365 6261 636b 2028 6d6f 7374 2072 6563  ceback (most rec
+00002900: 656e 7420 6361 6c6c 206c 6173 7429 3a0a  ent call last):.
+00002910: 2020 2020 5479 7065 4572 726f 723a 2064      TypeError: d
+00002920: 6563 6c61 7265 6420 275f 5f65 715f 5f27  eclared '__eq__'
+00002930: 2069 6e20 2741 7373 6574 2720 6275 7420   in 'Asset' but 
+00002940: 6469 646e 2774 2064 6563 6c61 7265 2027  didn't declare '
+00002950: 5f5f 6861 7368 5f5f 270a 0a66 6162 7269  __hash__'..fabri
+00002960: 6361 7465 5f76 616c 7565 0a5e 5e5e 5e5e  cate_value.^^^^^
+00002970: 5e5e 5e5e 5e5e 5e5e 5e5e 0a52 756e 2061  ^^^^^^^^^^.Run a
+00002980: 2076 616c 7565 2074 6872 6f75 6768 2061   value through a
+00002990: 2063 616c 6c61 626c 6520 6661 6374 6f72   callable factor
+000029a0: 7920 286f 7220 4e6f 6e65 292e 0a0a 2e2e  y (or None).....
+000029b0: 2063 6f64 653a 3a20 7079 7468 6f6e 0a0a   code:: python..
+000029c0: 2020 2020 3e3e 3e20 6672 6f6d 2062 6173      >>> from bas
+000029d0: 6963 636f 2e66 6162 7269 6361 7465 5f76  icco.fabricate_v
+000029e0: 616c 7565 2069 6d70 6f72 7420 6661 6272  alue import fabr
+000029f0: 6963 6174 655f 7661 6c75 650a 2020 2020  icate_value.    
+00002a00: 3e3e 3e20 6661 6272 6963 6174 655f 7661  >>> fabricate_va
+00002a10: 6c75 6528 4e6f 6e65 2c20 3329 2020 2320  lue(None, 3)  # 
+00002a20: 6e6f 2066 6163 746f 7279 2c20 7661 6c75  no factory, valu
+00002a30: 6520 7061 7373 7468 726f 7567 680a 2020  e passthrough.  
+00002a40: 2020 330a 2020 2020 3e3e 3e20 6661 6272    3.    >>> fabr
+00002a50: 6963 6174 655f 7661 6c75 6528 7374 722c  icate_value(str,
+00002a60: 2033 2920 2023 2063 616c 6c61 626c 6520   3)  # callable 
+00002a70: 6661 6374 6f72 790a 2020 2020 2733 270a  factory.    '3'.
+00002a80: 2020 2020 3e3e 3e20 6661 6272 6963 6174      >>> fabricat
+00002a90: 655f 7661 6c75 6528 2273 7472 222c 2033  e_value("str", 3
+00002aa0: 2920 2023 2075 7365 2061 6e20 696d 706f  )  # use an impo
+00002ab0: 7274 2070 6174 680a 2020 2020 2733 270a  rt path.    '3'.
+00002ac0: 2020 2020 3e3e 3e20 6661 6272 6963 6174      >>> fabricat
+00002ad0: 655f 7661 6c75 6528 696e 7429 2020 2320  e_value(int)  # 
+00002ae0: 6e6f 2069 6e70 7574 2076 616c 7565 2c20  no input value, 
+00002af0: 6a75 7374 2074 6865 2066 6163 746f 7279  just the factory
+00002b00: 2069 7473 656c 660a 2020 2020 300a 0a67   itself.    0..g
+00002b10: 6574 5f6d 726f 0a5e 5e5e 5e5e 5e5e 0a47  et_mro.^^^^^^^.G
+00002b20: 6574 2063 6f6e 7369 7374 656e 7420 4d52  et consistent MR
+00002b30: 4f20 616d 6f6e 6773 7420 6469 6666 6572  O amongst differ
+00002b40: 656e 7420 7079 7468 6f6e 2076 6572 7369  ent python versi
+00002b50: 6f6e 732e 2054 6869 7320 776f 726b 7320  ons. This works 
+00002b60: 6576 656e 2077 6974 6820 6765 6e65 7269  even with generi
+00002b70: 6320 636c 6173 7365 7320 696e 2050 7974  c classes in Pyt
+00002b80: 686f 6e20 322e 372e 0a0a 2e2e 2063 6f64  hon 2.7..... cod
+00002b90: 653a 3a20 7079 7468 6f6e 0a0a 2020 2020  e:: python..    
+00002ba0: 3e3e 3e20 6672 6f6d 2073 6978 2069 6d70  >>> from six imp
+00002bb0: 6f72 7420 7769 7468 5f6d 6574 6163 6c61  ort with_metacla
+00002bc0: 7373 0a20 2020 203e 3e3e 2066 726f 6d20  ss.    >>> from 
+00002bd0: 7469 7070 6f20 696d 706f 7274 2047 656e  tippo import Gen
+00002be0: 6572 6963 2c20 5479 7065 5661 720a 2020  eric, TypeVar.  
+00002bf0: 2020 3e3e 3e20 6672 6f6d 2062 6173 6963    >>> from basic
+00002c00: 636f 2e67 6574 5f6d 726f 2069 6d70 6f72  co.get_mro impor
+00002c10: 7420 6765 745f 6d72 6f0a 2020 2020 3e3e  t get_mro.    >>
+00002c20: 3e20 5420 3d20 5479 7065 5661 7228 2254  > T = TypeVar("T
+00002c30: 2229 0a20 2020 203e 3e3e 2063 6c61 7373  ").    >>> class
+00002c40: 204d 7947 656e 6572 6963 2847 656e 6572   MyGeneric(Gener
+00002c50: 6963 5b54 5d29 3a0a 2020 2020 2e2e 2e20  ic[T]):.    ... 
+00002c60: 2020 2020 7061 7373 0a20 2020 202e 2e2e      pass.    ...
+00002c70: 0a20 2020 203e 3e3e 2063 6c61 7373 2053  .    >>> class S
+00002c80: 7562 436c 6173 7328 4d79 4765 6e65 7269  ubClass(MyGeneri
+00002c90: 635b 545d 293a 0a20 2020 202e 2e2e 2020  c[T]):.    ...  
+00002ca0: 2020 2070 6173 730a 2020 2020 2e2e 2e0a     pass.    ....
+00002cb0: 2020 2020 3e3e 3e20 636c 6173 7320 4d69      >>> class Mi
+00002cc0: 7865 6428 5375 6243 6c61 7373 5b54 5d2c  xed(SubClass[T],
+00002cd0: 204d 7947 656e 6572 6963 5b54 5d29 3a0a   MyGeneric[T]):.
+00002ce0: 2020 2020 2e2e 2e20 2020 2020 7061 7373      ...     pass
+00002cf0: 0a20 2020 202e 2e2e 0a20 2020 203e 3e3e  .    ....    >>>
+00002d00: 205b 632e 5f5f 6e61 6d65 5f5f 2066 6f72   [c.__name__ for
+00002d10: 2063 2069 6e20 6765 745f 6d72 6f28 4d69   c in get_mro(Mi
+00002d20: 7865 6429 5d0a 2020 2020 5b27 4d69 7865  xed)].    ['Mixe
+00002d30: 6427 2c20 2753 7562 436c 6173 7327 2c20  d', 'SubClass', 
+00002d40: 274d 7947 656e 6572 6963 272c 2027 4765  'MyGeneric', 'Ge
+00002d50: 6e65 7269 6327 2c20 276f 626a 6563 7427  neric', 'object'
+00002d60: 5d0a 0a68 6173 685f 6361 6368 655f 7772  ]..hash_cache_wr
+00002d70: 6170 7065 720a 5e5e 5e5e 5e5e 5e5e 5e5e  apper.^^^^^^^^^^
+00002d80: 5e5e 5e5e 5e5e 5e5e 0a41 6e20 696e 7465  ^^^^^^^^.An inte
+00002d90: 6765 7220 7375 6263 6c61 7373 2074 6861  ger subclass tha
+00002da0: 7420 7069 636b 6c65 732f 636f 7069 6573  t pickles/copies
+00002db0: 2061 7320 4e6f 6e65 2e20 5468 6973 2063   as None. This c
+00002dc0: 616e 2062 6520 7573 6564 2074 6f20 6176  an be used to av
+00002dd0: 6f69 6420 7365 7269 616c 697a 696e 6720  oid serializing 
+00002de0: 6120 6361 6368 6564 2068 6173 6820 7661  a cached hash va
+00002df0: 6c75 652e 0a0a 2e2e 2063 6f64 653a 3a20  lue..... code:: 
+00002e00: 7079 7468 6f6e 0a0a 2020 2020 3e3e 3e20  python..    >>> 
+00002e10: 6672 6f6d 2063 6f70 7920 696d 706f 7274  from copy import
+00002e20: 2063 6f70 790a 2020 2020 3e3e 3e20 6672   copy.    >>> fr
+00002e30: 6f6d 2062 6173 6963 636f 2e68 6173 685f  om basicco.hash_
+00002e40: 6361 6368 655f 7772 6170 7065 7220 696d  cache_wrapper im
+00002e50: 706f 7274 2048 6173 6843 6163 6865 5772  port HashCacheWr
+00002e60: 6170 7065 720a 2020 2020 3e3e 3e20 6861  apper.    >>> ha
+00002e70: 7368 5f63 6163 6865 203d 2048 6173 6843  sh_cache = HashC
+00002e80: 6163 6865 5772 6170 7065 7228 3132 3334  acheWrapper(1234
+00002e90: 3529 0a20 2020 203e 3e3e 2070 7269 6e74  5).    >>> print
+00002ea0: 2868 6173 685f 6361 6368 6529 0a20 2020  (hash_cache).   
+00002eb0: 2031 3233 3435 0a20 2020 203e 3e3e 2070   12345.    >>> p
+00002ec0: 7269 6e74 2863 6f70 7928 6861 7368 5f63  rint(copy(hash_c
+00002ed0: 6163 6865 2929 0a20 2020 204e 6f6e 650a  ache)).    None.
+00002ee0: 0a69 6d70 6c69 6369 745f 6861 7368 0a5e  .implicit_hash.^
+00002ef0: 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e 0a4d 6574  ^^^^^^^^^^^^.Met
+00002f00: 6163 6c61 7373 2074 6861 7420 666f 7263  aclass that forc
+00002f10: 6573 2060 5f5f 6861 7368 5f5f 6020 746f  es `__hash__` to
+00002f20: 204e 6f6e 6520 7768 656e 2060 5f5f 6571   None when `__eq
+00002f30: 5f5f 6020 6973 2064 6563 6c61 7265 642e  __` is declared.
+00002f40: 0a54 6869 7320 6973 2061 2062 6163 6b70  .This is a backp
+00002f50: 6f72 7420 6f66 2074 6865 2064 6566 6175  ort of the defau
+00002f60: 6c74 2062 6568 6176 696f 7220 696e 2050  lt behavior in P
+00002f70: 7974 686f 6e20 332e 0a0a 2e2e 2063 6f64  ython 3..... cod
+00002f80: 653a 3a20 7079 7468 6f6e 0a0a 2020 2020  e:: python..    
+00002f90: 3e3e 3e20 6672 6f6d 2073 6978 2069 6d70  >>> from six imp
+00002fa0: 6f72 7420 7769 7468 5f6d 6574 6163 6c61  ort with_metacla
+00002fb0: 7373 0a20 2020 203e 3e3e 2066 726f 6d20  ss.    >>> from 
+00002fc0: 6261 7369 6363 6f2e 696d 706c 6963 6974  basicco.implicit
+00002fd0: 5f68 6173 6820 696d 706f 7274 2049 6d70  _hash import Imp
+00002fe0: 6c69 6369 7448 6173 684d 6574 610a 2020  licitHashMeta.  
+00002ff0: 2020 3e3e 3e20 636c 6173 7320 4173 7365    >>> class Asse
+00003000: 7428 7769 7468 5f6d 6574 6163 6c61 7373  t(with_metaclass
+00003010: 2849 6d70 6c69 6369 7448 6173 684d 6574  (ImplicitHashMet
+00003020: 612c 206f 626a 6563 7429 293a 0a20 2020  a, object)):.   
+00003030: 202e 2e2e 2020 2020 2064 6566 205f 5f65   ...     def __e
+00003040: 715f 5f28 7365 6c66 2c20 6f74 6865 7229  q__(self, other)
+00003050: 3a0a 2020 2020 2e2e 2e20 2020 2020 2020  :.    ...       
+00003060: 2020 7061 7373 0a20 2020 202e 2e2e 0a20    pass.    .... 
+00003070: 2020 203e 3e3e 2041 7373 6574 2e5f 5f68     >>> Asset.__h
+00003080: 6173 685f 5f20 6973 204e 6f6e 650a 2020  ash__ is None.  
+00003090: 2020 5472 7565 0a0a 696d 706f 7274 5f70    True..import_p
+000030a0: 6174 680a 5e5e 5e5e 5e5e 5e5e 5e5e 5e0a  ath.^^^^^^^^^^^.
+000030b0: 4765 6e65 7261 7465 2069 6d70 6f72 7461  Generate importa
+000030c0: 626c 6520 646f 7420 7061 7468 7320 616e  ble dot paths an
+000030d0: 6420 696d 706f 7274 2066 726f 6d20 7468  d import from th
+000030e0: 656d 2e0a 0a2e 2e20 636f 6465 3a3a 2070  em..... code:: p
+000030f0: 7974 686f 6e0a 0a20 2020 203e 3e3e 2069  ython..    >>> i
+00003100: 6d70 6f72 7420 6974 6572 746f 6f6c 730a  mport itertools.
+00003110: 2020 2020 3e3e 3e20 6672 6f6d 2062 6173      >>> from bas
+00003120: 6963 636f 2e69 6d70 6f72 745f 7061 7468  icco.import_path
+00003130: 2069 6d70 6f72 7420 6765 745f 7061 7468   import get_path
+00003140: 2c20 696d 706f 7274 5f70 6174 680a 2020  , import_path.  
+00003150: 2020 3e3e 3e20 6765 745f 7061 7468 2869    >>> get_path(i
+00003160: 7465 7274 6f6f 6c73 2e63 6861 696e 290a  tertools.chain).
+00003170: 2020 2020 2769 7465 7274 6f6f 6c73 2e63      'itertools.c
+00003180: 6861 696e 270a 2020 2020 3e3e 3e20 696d  hain'.    >>> im
+00003190: 706f 7274 5f70 6174 6828 2269 7465 7274  port_path("itert
+000031a0: 6f6f 6c73 2e63 6861 696e 2229 0a20 2020  ools.chain").   
+000031b0: 203c 2e2e 2e20 2769 7465 7274 6f6f 6c73   <... 'itertools
+000031c0: 2e63 6861 696e 273e 0a0a 2e2e 2063 6f64  .chain'>.... cod
+000031d0: 653a 3a20 7079 7468 6f6e 0a0a 2020 2020  e:: python..    
+000031e0: 3e3e 3e20 6672 6f6d 2062 6173 6963 636f  >>> from basicco
+000031f0: 2e69 6d70 6f72 745f 7061 7468 2069 6d70  .import_path imp
+00003200: 6f72 7420 6578 7472 6163 745f 6765 6e65  ort extract_gene
+00003210: 7269 635f 7061 7468 730a 2020 2020 3e3e  ric_paths.    >>
+00003220: 3e20 6578 7472 6163 745f 6765 6e65 7269  > extract_generi
+00003230: 635f 7061 7468 7328 2254 7570 6c65 5b69  c_paths("Tuple[i
+00003240: 6e74 2c20 7374 725d 2229 0a20 2020 2028  nt, str]").    (
+00003250: 2754 7570 6c65 272c 2028 2769 6e74 272c  'Tuple', ('int',
+00003260: 2027 7374 7227 2929 0a0a 696e 6974 5f73   'str'))..init_s
+00003270: 7562 636c 6173 730a 5e5e 5e5e 5e5e 5e5e  ubclass.^^^^^^^^
+00003280: 5e5e 5e5e 5e0a 4261 636b 706f 7274 206f  ^^^^^.Backport o
+00003290: 6620 7468 6520 6675 6e63 7469 6f6e 616c  f the functional
+000032a0: 6974 7920 6f66 2060 5f5f 696e 6974 5f73  ity of `__init_s
+000032b0: 7562 636c 6173 735f 5f60 2066 726f 6d20  ubclass__` from 
+000032c0: 5045 5020 3438 3720 746f 2050 7974 686f  PEP 487 to Pytho
+000032d0: 6e20 322e 372e 0a54 6869 7320 776f 726b  n 2.7..This work
+000032e0: 7320 666f 7220 626f 7468 2050 7974 686f  s for both Pytho
+000032f0: 6e20 3220 2875 7369 6e67 2060 5f5f 6b77  n 2 (using `__kw
+00003300: 6172 6773 5f5f 6029 2061 6e64 2033 2028  args__`) and 3 (
+00003310: 7573 696e 6720 7468 6520 6e65 7720 636c  using the new cl
+00003320: 6173 7320 7061 7261 6d65 7465 7273 292e  ass parameters).
+00003330: 0a0a 2e2e 2063 6f64 653a 3a20 7079 7468  .... code:: pyth
+00003340: 6f6e 0a0a 2020 2020 3e3e 3e20 6672 6f6d  on..    >>> from
+00003350: 2062 6173 6963 636f 2e69 6e69 745f 7375   basicco.init_su
+00003360: 6263 6c61 7373 2069 6d70 6f72 7420 496e  bclass import In
+00003370: 6974 5375 6263 6c61 7373 0a20 2020 203e  itSubclass.    >
+00003380: 3e3e 2063 6c61 7373 2046 6f6f 2849 6e69  >> class Foo(Ini
+00003390: 7453 7562 636c 6173 7329 3a0a 2020 2020  tSubclass):.    
+000033a0: 2e2e 2e20 2020 2020 6465 6620 5f5f 696e  ...     def __in
+000033b0: 6974 5f73 7562 636c 6173 735f 5f28 636c  it_subclass__(cl
+000033c0: 732c 2066 6f6f 3d4e 6f6e 652c 202a 2a6b  s, foo=None, **k
+000033d0: 7761 7267 7329 3a0a 2020 2020 2e2e 2e20  wargs):.    ... 
+000033e0: 2020 2020 2020 2020 636c 732e 666f 6f20          cls.foo 
+000033f0: 3d20 666f 6f0a 2020 2020 2e2e 2e0a 2020  = foo.    ....  
+00003400: 2020 3e3e 3e20 636c 6173 7320 4261 7228    >>> class Bar(
+00003410: 466f 6f29 3a0a 2020 2020 2e2e 2e20 2020  Foo):.    ...   
+00003420: 2020 5f5f 6b77 6172 6773 5f5f 203d 207b    __kwargs__ = {
+00003430: 2266 6f6f 223a 2022 6261 7222 7d20 2023  "foo": "bar"}  #
+00003440: 2079 6f75 2063 616e 2073 7065 6369 6679   you can specify
+00003450: 2063 6c73 206b 7761 7267 7320 6f6e 2070   cls kwargs on p
+00003460: 7932 206c 696b 6520 7468 6973 0a20 2020  y2 like this.   
+00003470: 202e 2e2e 0a20 2020 203e 3e3e 2042 6172   ....    >>> Bar
+00003480: 2e66 6f6f 0a20 2020 2027 6261 7227 0a0a  .foo.    'bar'..
+00003490: 6c6f 636b 6564 5f63 6c61 7373 0a5e 5e5e  locked_class.^^^
+000034a0: 5e5e 5e5e 5e5e 5e5e 5e0a 5072 6576 656e  ^^^^^^^^^.Preven
+000034b0: 7473 2063 6861 6e67 696e 6720 7075 626c  ts changing publ
+000034c0: 6963 2063 6c61 7373 2061 7474 7269 6275  ic class attribu
+000034d0: 7465 732e 0a0a 2e2e 2063 6f64 653a 3a20  tes..... code:: 
+000034e0: 7079 7468 6f6e 0a0a 2020 2020 3e3e 3e20  python..    >>> 
+000034f0: 6672 6f6d 2073 6978 2069 6d70 6f72 7420  from six import 
+00003500: 7769 7468 5f6d 6574 6163 6c61 7373 0a20  with_metaclass. 
+00003510: 2020 203e 3e3e 2066 726f 6d20 6261 7369     >>> from basi
+00003520: 6363 6f2e 6c6f 636b 6564 5f63 6c61 7373  cco.locked_class
+00003530: 2069 6d70 6f72 7420 4c6f 636b 6564 436c   import LockedCl
+00003540: 6173 734d 6574 610a 2020 2020 3e3e 3e20  assMeta.    >>> 
+00003550: 636c 6173 7320 466f 6f28 7769 7468 5f6d  class Foo(with_m
+00003560: 6574 6163 6c61 7373 284c 6f63 6b65 6443  etaclass(LockedC
+00003570: 6c61 7373 4d65 7461 2c20 6f62 6a65 6374  lassMeta, object
+00003580: 2929 3a0a 2020 2020 2e2e 2e20 2020 2020  )):.    ...     
+00003590: 6261 7220 3d20 2266 6f6f 220a 2020 2020  bar = "foo".    
+000035a0: 2e2e 2e0a 2020 2020 3e3e 3e20 466f 6f2e  ....    >>> Foo.
+000035b0: 6261 7220 3d20 2262 6172 220a 2020 2020  bar = "bar".    
+000035c0: 5472 6163 6562 6163 6b20 286d 6f73 7420  Traceback (most 
+000035d0: 7265 6365 6e74 2063 616c 6c20 6c61 7374  recent call last
+000035e0: 293a 0a20 2020 2041 7474 7269 6275 7465  ):.    Attribute
+000035f0: 4572 726f 723a 2063 616e 2774 2073 6574  Error: can't set
+00003600: 2072 6561 642d 6f6e 6c79 2063 6c61 7373   read-only class
+00003610: 2061 7474 7269 6275 7465 2027 6261 7227   attribute 'bar'
+00003620: 0a0a 6d61 6e67 6c69 6e67 0a5e 5e5e 5e5e  ..mangling.^^^^^
+00003630: 5e5e 5e0a 4675 6e63 7469 6f6e 7320 746f  ^^^.Functions to
+00003640: 206d 616e 676c 652f 756e 6d61 6e67 6c65   mangle/unmangle
+00003650: 2f65 7874 7261 6374 2070 7269 7661 7465  /extract private
+00003660: 206e 616d 6573 2e0a 0a2e 2e20 636f 6465   names..... code
+00003670: 3a3a 2070 7974 686f 6e0a 0a20 2020 203e  :: python..    >
+00003680: 3e3e 2066 726f 6d20 6261 7369 6363 6f2e  >> from basicco.
+00003690: 6d61 6e67 6c69 6e67 2069 6d70 6f72 7420  mangling import 
+000036a0: 6d61 6e67 6c65 2c20 756e 6d61 6e67 6c65  mangle, unmangle
+000036b0: 2c20 6578 7472 6163 740a 2020 2020 3e3e  , extract.    >>
+000036c0: 3e20 6d61 6e67 6c65 2822 5f5f 6d65 6d62  > mangle("__memb
+000036d0: 6572 222c 2022 466f 6f22 290a 2020 2020  er", "Foo").    
+000036e0: 275f 466f 6f5f 5f6d 656d 6265 7227 0a20  '_Foo__member'. 
+000036f0: 2020 203e 3e3e 2075 6e6d 616e 676c 6528     >>> unmangle(
+00003700: 225f 466f 6f5f 5f6d 656d 6265 7222 2c20  "_Foo__member", 
+00003710: 2246 6f6f 2229 0a20 2020 2027 5f5f 6d65  "Foo").    '__me
+00003720: 6d62 6572 270a 2020 2020 3e3e 3e20 6578  mber'.    >>> ex
+00003730: 7472 6163 7428 225f 466f 6f5f 5f6d 656d  tract("_Foo__mem
+00003740: 6265 7222 290a 2020 2020 2827 5f5f 6d65  ber").    ('__me
+00003750: 6d62 6572 272c 2027 466f 6f27 290a 0a6d  mber', 'Foo')..m
+00003760: 6170 7069 6e67 5f70 726f 7879 0a5e 5e5e  apping_proxy.^^^
+00003770: 5e5e 5e5e 5e5e 5e5e 5e5e 0a4d 6170 7069  ^^^^^^^^^^.Mappi
+00003780: 6e67 2050 726f 7879 2074 7970 6520 2872  ng Proxy type (r
+00003790: 6561 642d 6f6e 6c79 2064 6963 7469 6f6e  ead-only diction
+000037a0: 6172 7929 2066 6f72 206f 6c64 6572 2050  ary) for older P
+000037b0: 7974 686f 6e20 7665 7273 696f 6e73 2e0a  ython versions..
+000037c0: 0a2e 2e20 636f 6465 3a3a 2070 7974 686f  ... code:: pytho
+000037d0: 6e0a 0a20 2020 203e 3e3e 2066 726f 6d20  n..    >>> from 
+000037e0: 6261 7369 6363 6f2e 6d61 7070 696e 675f  basicco.mapping_
+000037f0: 7072 6f78 7920 696d 706f 7274 204d 6170  proxy import Map
+00003800: 7069 6e67 5072 6f78 7954 7970 650a 2020  pingProxyType.  
+00003810: 2020 3e3e 3e20 696e 7465 726e 616c 5f64    >>> internal_d
+00003820: 6963 7420 3d20 7b22 666f 6f22 3a20 2262  ict = {"foo": "b
+00003830: 6172 227d 0a20 2020 203e 3e3e 2070 726f  ar"}.    >>> pro
+00003840: 7879 5f64 6963 7420 3d20 4d61 7070 696e  xy_dict = Mappin
+00003850: 6750 726f 7879 5479 7065 2869 6e74 6572  gProxyType(inter
+00003860: 6e61 6c5f 6469 6374 290a 2020 2020 3e3e  nal_dict).    >>
+00003870: 3e20 7072 6f78 795f 6469 6374 5b22 666f  > proxy_dict["fo
+00003880: 6f22 5d0a 2020 2020 2762 6172 270a 0a6e  o"].    'bar'..n
+00003890: 616d 6564 5f74 7570 6c65 0a5e 5e5e 5e5e  amed_tuple.^^^^^
+000038a0: 5e5e 5e5e 5e5e 0a4e 616d 6564 2054 7570  ^^^^^^.Named Tup
+000038b0: 6c65 2075 7469 6c69 7469 6573 2e0a 0a45  le utilities...E
+000038c0: 7861 6d70 6c65 206f 6620 6064 6566 6175  xample of `defau
+000038d0: 6c74 7360 2064 6563 6f72 6174 6f72 2f66  lts` decorator/f
+000038e0: 756e 6374 696f 6e20 746f 2073 6574 2061  unction to set a
+000038f0: 204e 616d 6564 2054 7570 6c65 2773 2064   Named Tuple's d
+00003900: 6566 6175 6c74 2076 616c 7565 733a 0a0a  efault values:..
+00003910: 2e2e 2063 6f64 653a 3a20 7079 7468 6f6e  .. code:: python
+00003920: 0a0a 2020 2020 3e3e 3e20 6672 6f6d 2063  ..    >>> from c
+00003930: 6f6c 6c65 6374 696f 6e73 2069 6d70 6f72  ollections impor
+00003940: 7420 6e61 6d65 6474 7570 6c65 0a20 2020  t namedtuple.   
+00003950: 203e 3e3e 2066 726f 6d20 6261 7369 6363   >>> from basicc
+00003960: 6f2e 6e61 6d65 645f 7475 706c 6520 696d  o.named_tuple im
+00003970: 706f 7274 2064 6566 6175 6c74 730a 2020  port defaults.  
+00003980: 2020 3e3e 3e20 506f 696e 7420 3d20 6465    >>> Point = de
+00003990: 6661 756c 7473 286e 616d 653d 2266 6f6f  faults(name="foo
+000039a0: 2229 286e 616d 6564 7475 706c 6528 2250  ")(namedtuple("P
+000039b0: 6f69 6e74 222c 2028 2278 222c 2022 7922  oint", ("x", "y"
+000039c0: 2c20 226e 616d 6522 2929 290a 2020 2020  , "name"))).    
+000039d0: 3e3e 3e20 506f 696e 7428 312c 2032 290a  >>> Point(1, 2).
+000039e0: 2020 2020 506f 696e 7428 783d 312c 2079      Point(x=1, y
+000039f0: 3d32 2c20 6e61 6d65 3d27 666f 6f27 290a  =2, name='foo').
+00003a00: 0a6e 616d 6573 7061 6365 0a5e 5e5e 5e5e  .namespace.^^^^^
+00003a10: 5e5e 5e5e 0a57 7261 7073 2061 2064 6963  ^^^^.Wraps a dic
+00003a20: 7469 6f6e 6172 792f 6d61 7070 696e 6720  tionary/mapping 
+00003a30: 616e 6420 7072 6f76 6964 6573 2061 7474  and provides att
+00003a40: 7269 6275 7465 2d73 7479 6c65 2061 6363  ribute-style acc
+00003a50: 6573 7320 746f 2069 742e 0a0a 2e2e 2063  ess to it..... c
+00003a60: 6f64 653a 3a20 7079 7468 6f6e 0a0a 2020  ode:: python..  
+00003a70: 2020 3e3e 3e20 6672 6f6d 2062 6173 6963    >>> from basic
+00003a80: 636f 2e6e 616d 6573 7061 6365 2069 6d70  co.namespace imp
+00003a90: 6f72 7420 4e61 6d65 7370 6163 650a 2020  ort Namespace.  
+00003aa0: 2020 3e3e 3e20 6e73 203d 204e 616d 6573    >>> ns = Names
+00003ab0: 7061 6365 287b 2262 6172 223a 2022 666f  pace({"bar": "fo
+00003ac0: 6f22 7d29 0a20 2020 203e 3e3e 206e 732e  o"}).    >>> ns.
+00003ad0: 6261 720a 2020 2020 2766 6f6f 270a 0a2e  bar.    'foo'...
+00003ae0: 2e20 636f 6465 3a3a 2070 7974 686f 6e0a  . code:: python.
+00003af0: 0a20 2020 203e 3e3e 2066 726f 6d20 6261  .    >>> from ba
+00003b00: 7369 6363 6f2e 6e61 6d65 7370 6163 6520  sicco.namespace 
+00003b10: 696d 706f 7274 204d 7574 6162 6c65 4e61  import MutableNa
+00003b20: 6d65 7370 6163 650a 2020 2020 3e3e 3e20  mespace.    >>> 
+00003b30: 6e73 203d 204d 7574 6162 6c65 4e61 6d65  ns = MutableName
+00003b40: 7370 6163 6528 7b22 6261 7222 3a20 2266  space({"bar": "f
+00003b50: 6f6f 227d 290a 2020 2020 3e3e 3e20 6e73  oo"}).    >>> ns
+00003b60: 2e66 6f6f 203d 2022 6261 7222 0a20 2020  .foo = "bar".   
+00003b70: 203e 3e3e 206e 732e 666f 6f0a 2020 2020   >>> ns.foo.    
+00003b80: 2762 6172 270a 2020 2020 3e3e 3e20 6e73  'bar'.    >>> ns
+00003b90: 2e62 6172 0a20 2020 2027 666f 6f27 0a0a  .bar.    'foo'..
+00003ba0: 416c 736f 2070 726f 7669 6465 7320 6120  Also provides a 
+00003bb0: 604e 616d 6573 7061 6365 644d 6574 6160  `NamespacedMeta`
+00003bc0: 206d 6574 6163 6c61 7373 2074 6861 7420   metaclass that 
+00003bd0: 6164 6473 2061 2060 5f5f 6e61 6d65 7370  adds a `__namesp
+00003be0: 6163 6560 2070 726f 7465 6374 6564 2063  ace` protected c
+00003bf0: 6c61 7373 2061 7474 7269 6275 7465 2074  lass attribute t
+00003c00: 6861 7420 6973 2075 6e69 7175 6520 746f  hat is unique to
+00003c10: 2065 6163 680a 636c 6173 732e 0a0a 2e2e   each.class.....
+00003c20: 2063 6f64 653a 3a20 7079 7468 6f6e 0a0a   code:: python..
+00003c30: 2020 2020 3e3e 3e20 6672 6f6d 2073 6978      >>> from six
+00003c40: 2069 6d70 6f72 7420 7769 7468 5f6d 6574   import with_met
+00003c50: 6163 6c61 7373 0a20 2020 203e 3e3e 2066  aclass.    >>> f
+00003c60: 726f 6d20 6261 7369 6363 6f2e 6e61 6d65  rom basicco.name
+00003c70: 7370 6163 6520 696d 706f 7274 204e 616d  space import Nam
+00003c80: 6573 7061 6365 644d 6574 610a 2020 2020  espacedMeta.    
+00003c90: 3e3e 3e20 636c 6173 7320 4173 7365 7428  >>> class Asset(
+00003ca0: 7769 7468 5f6d 6574 6163 6c61 7373 284e  with_metaclass(N
+00003cb0: 616d 6573 7061 6365 644d 6574 612c 206f  amespacedMeta, o
+00003cc0: 626a 6563 7429 293a 0a20 2020 202e 2e2e  bject)):.    ...
+00003cd0: 2020 2020 2040 636c 6173 736d 6574 686f       @classmetho
+00003ce0: 640a 2020 2020 2e2e 2e20 2020 2020 6465  d.    ...     de
+00003cf0: 6620 7365 745f 636c 6173 735f 7661 6c75  f set_class_valu
+00003d00: 6528 636c 732c 2076 616c 7565 293a 0a20  e(cls, value):. 
+00003d10: 2020 202e 2e2e 2020 2020 2020 2020 2063     ...         c
+00003d20: 6c73 2e5f 5f6e 616d 6573 7061 6365 2e76  ls.__namespace.v
+00003d30: 616c 7565 203d 2076 616c 7565 0a20 2020  alue = value.   
+00003d40: 202e 2e2e 0a20 2020 202e 2e2e 2020 2020   ....    ...    
+00003d50: 2040 636c 6173 736d 6574 686f 640a 2020   @classmethod.  
+00003d60: 2020 2e2e 2e20 2020 2020 6465 6620 6765    ...     def ge
+00003d70: 745f 636c 6173 735f 7661 6c75 6528 636c  t_class_value(cl
+00003d80: 7329 3a0a 2020 2020 2e2e 2e20 2020 2020  s):.    ...     
+00003d90: 2020 2020 7265 7475 726e 2063 6c73 2e5f      return cls._
+00003da0: 5f6e 616d 6573 7061 6365 2e76 616c 7565  _namespace.value
+00003db0: 0a20 2020 202e 2e2e 0a20 2020 203e 3e3e  .    ....    >>>
+00003dc0: 2041 7373 6574 2e73 6574 5f63 6c61 7373   Asset.set_class
+00003dd0: 5f76 616c 7565 2822 666f 6f62 6172 2229  _value("foobar")
+00003de0: 0a20 2020 203e 3e3e 2041 7373 6574 2e67  .    >>> Asset.g
+00003df0: 6574 5f63 6c61 7373 5f76 616c 7565 2829  et_class_value()
+00003e00: 0a20 2020 2027 666f 6f62 6172 270a 0a6f  .    'foobar'..o
+00003e10: 626a 5f73 7461 7465 0a5e 5e5e 5e5e 5e5e  bj_state.^^^^^^^
+00003e20: 5e5e 0a47 6574 2f75 7064 6174 6520 7468  ^^.Get/update th
+00003e30: 6520 7374 6174 6520 6f66 2061 6e20 6f62  e state of an ob
+00003e40: 6a65 6374 2c20 736c 6f74 7465 6420 6f72  ject, slotted or
+00003e50: 206e 6f74 2028 776f 726b 7320 6576 656e   not (works even
+00003e60: 2069 6e20 5079 7468 6f6e 2032 2e37 292e   in Python 2.7).
+00003e70: 0a0a 2e2e 2063 6f64 653a 3a20 7079 7468  .... code:: pyth
+00003e80: 6f6e 0a0a 2020 2020 3e3e 3e20 6672 6f6d  on..    >>> from
+00003e90: 2062 6173 6963 636f 2e6f 626a 5f73 7461   basicco.obj_sta
+00003ea0: 7465 2069 6d70 6f72 7420 6765 745f 7374  te import get_st
+00003eb0: 6174 650a 2020 2020 3e3e 3e20 636c 6173  ate.    >>> clas
+00003ec0: 7320 536c 6f74 7465 6428 6f62 6a65 6374  s Slotted(object
+00003ed0: 293a 0a20 2020 202e 2e2e 2020 2020 205f  ):.    ...     _
+00003ee0: 5f73 6c6f 7473 5f5f 203d 2028 2266 6f6f  _slots__ = ("foo
+00003ef0: 222c 2022 6261 7222 290a 2020 2020 2e2e  ", "bar").    ..
+00003f00: 2e20 2020 2020 6465 6620 5f5f 696e 6974  .     def __init
+00003f10: 5f5f 2873 656c 662c 2066 6f6f 2c20 6261  __(self, foo, ba
+00003f20: 7229 3a0a 2020 2020 2e2e 2e20 2020 2020  r):.    ...     
+00003f30: 2020 2020 7365 6c66 2e66 6f6f 203d 2066      self.foo = f
+00003f40: 6f6f 0a20 2020 202e 2e2e 2020 2020 2020  oo.    ...      
+00003f50: 2020 2073 656c 662e 6261 7220 3d20 6261     self.bar = ba
+00003f60: 720a 2020 2020 2e2e 2e0a 2020 2020 3e3e  r.    ....    >>
+00003f70: 3e20 736c 6f74 7465 6420 3d20 536c 6f74  > slotted = Slot
+00003f80: 7465 6428 2261 222c 2022 6222 290a 2020  ted("a", "b").  
+00003f90: 2020 3e3e 3e20 736f 7274 6564 2867 6574    >>> sorted(get
+00003fa0: 5f73 7461 7465 2873 6c6f 7474 6564 292e  _state(slotted).
+00003fb0: 6974 656d 7328 2929 0a20 2020 205b 2827  items()).    [('
+00003fc0: 6261 7227 2c20 2762 2729 2c20 2827 666f  bar', 'b'), ('fo
+00003fd0: 6f27 2c20 2761 2729 5d0a 0a41 6c73 6f20  o', 'a')]..Also 
+00003fe0: 7072 6f76 6964 6573 2061 2060 5265 6475  provides a `Redu
+00003ff0: 6369 626c 654d 6574 6160 206d 6574 6163  cibleMeta` metac
+00004000: 6c61 7373 2074 6861 7420 616c 6c6f 7773  lass that allows
+00004010: 2066 6f72 2070 6963 6b6c 696e 6720 696e   for pickling in
+00004020: 7374 616e 6365 7320 6f66 2073 6c6f 7474  stances of slott
+00004030: 6564 2063 6c61 7373 6573 2069 6e20 5079  ed classes in Py
+00004040: 7468 6f6e 2032 2e37 2e0a 0a71 7561 6c6e  thon 2.7...qualn
+00004050: 616d 650a 5e5e 5e5e 5e5e 5e5e 0a50 7974  ame.^^^^^^^^.Pyt
+00004060: 686f 6e20 322e 3720 636f 6d70 6174 6962  hon 2.7 compatib
+00004070: 6c65 2077 6179 206f 6620 6765 7474 696e  le way of gettin
+00004080: 6720 7468 6520 7175 616c 6966 6965 6420  g the qualified 
+00004090: 6e61 6d65 2e20 4261 7365 6420 6f6e 0a60  name. Based on.`
+000040a0: 7762 6f6c 7374 6572 2f71 7561 6c6e 616d  wbolster/qualnam
+000040b0: 6520 3c68 7474 7073 3a2f 2f67 6974 6875  e <https://githu
+000040c0: 622e 636f 6d2f 7762 6f6c 7374 6572 2f71  b.com/wbolster/q
+000040d0: 7561 6c6e 616d 653e 605f 2e0a 416c 736f  ualname>`_..Also
+000040e0: 2070 726f 7669 6465 7320 6120 6051 7561   provides a `Qua
+000040f0: 6c6e 616d 6564 4d65 7461 6020 6d65 7461  lnamedMeta` meta
+00004100: 636c 6173 7320 7769 7468 2061 2060 5f5f  class with a `__
+00004110: 7175 616c 6e61 6d65 5f5f 6020 636c 6173  qualname__` clas
+00004120: 7320 7072 6f70 6572 7479 2066 6f72 2050  s property for P
+00004130: 7974 686f 6e20 322e 372e 0a0a 7265 6375  ython 2.7...recu
+00004140: 7273 6976 655f 7265 7072 0a5e 5e5e 5e5e  rsive_repr.^^^^^
+00004150: 5e5e 5e5e 5e5e 5e5e 5e0a 4465 636f 7261  ^^^^^^^^^.Decora
+00004160: 746f 7220 7468 6174 2070 7265 7665 6e74  tor that prevent
+00004170: 7320 696e 6669 6e69 7465 2072 6563 7572  s infinite recur
+00004180: 7369 6f6e 2066 6f72 2060 5f5f 7265 7072  sion for `__repr
+00004190: 5f5f 6020 6d65 7468 6f64 732e 0a0a 2e2e  __` methods.....
+000041a0: 2063 6f64 653a 3a20 7079 7468 6f6e 0a0a   code:: python..
+000041b0: 2020 2020 3e3e 3e20 6672 6f6d 2062 6173      >>> from bas
+000041c0: 6963 636f 2e72 6563 7572 7369 7665 5f72  icco.recursive_r
+000041d0: 6570 7220 696d 706f 7274 2072 6563 7572  epr import recur
+000041e0: 7369 7665 5f72 6570 720a 2020 2020 3e3e  sive_repr.    >>
+000041f0: 3e20 636c 6173 7320 4d79 436c 6173 7328  > class MyClass(
+00004200: 6f62 6a65 6374 293a 0a20 2020 202e 2e2e  object):.    ...
+00004210: 0a20 2020 202e 2e2e 2020 2020 2040 7265  .    ...     @re
+00004220: 6375 7273 6976 655f 7265 7072 0a20 2020  cursive_repr.   
+00004230: 202e 2e2e 2020 2020 2064 6566 205f 5f72   ...     def __r
+00004240: 6570 725f 5f28 7365 6c66 293a 0a20 2020  epr__(self):.   
+00004250: 202e 2e2e 2020 2020 2020 2020 2072 6574   ...         ret
+00004260: 7572 6e20 224d 7943 6c61 7373 3c7b 2172  urn "MyClass<{!r
+00004270: 7d3e 222e 666f 726d 6174 2873 656c 6629  }>".format(self)
+00004280: 0a20 2020 202e 2e2e 0a20 2020 203e 3e3e  .    ....    >>>
+00004290: 206d 795f 6f62 6a20 3d20 4d79 436c 6173   my_obj = MyClas
+000042a0: 7328 290a 2020 2020 3e3e 3e20 7265 7072  s().    >>> repr
+000042b0: 286d 795f 6f62 6a29 0a20 2020 2027 4d79  (my_obj).    'My
+000042c0: 436c 6173 733c 2e2e 2e3e 270a 0a72 756e  Class<...>'..run
+000042d0: 7469 6d65 5f66 696e 616c 0a5e 5e5e 5e5e  time_final.^^^^^
+000042e0: 5e5e 5e5e 5e5e 5e5e 0a52 756e 7469 6d65  ^^^^^^^^.Runtime
+000042f0: 2d63 6865 636b 6564 2076 6572 7369 6f6e  -checked version
+00004300: 206f 6620 7468 6520 6074 7970 696e 672e   of the `typing.
+00004310: 6669 6e61 6c20 3c68 7474 7073 3a2f 2f64  final <https://d
+00004320: 6f63 732e 7079 7468 6f6e 2e6f 7267 2f33  ocs.python.org/3
+00004330: 2f6c 6962 7261 7279 2f74 7970 696e 672e  /library/typing.
+00004340: 6874 6d6c 2374 7970 696e 672e 6669 6e61  html#typing.fina
+00004350: 6c3e 605f 2064 6563 6f72 6174 6f72 2e0a  l>`_ decorator..
+00004360: 0a43 616e 2062 6520 7573 6564 206f 6e20  .Can be used on 
+00004370: 6d65 7468 6f64 732c 2070 726f 7065 7274  methods, propert
+00004380: 6965 732c 2063 6c61 7373 6d65 7468 6f64  ies, classmethod
+00004390: 732c 2073 7461 7469 636d 6574 686f 6473  s, staticmethods
+000043a0: 2c20 616e 6420 636c 6173 7365 7320 7468  , and classes th
+000043b0: 6174 2068 6176 6520 6052 756e 7469 6d65  at have `Runtime
+000043c0: 4669 6e61 6c4d 6574 6160 2061 7320 6120  FinalMeta` as a 
+000043d0: 6d65 7461 636c 6173 732e 0a49 7420 6973  metaclass..It is
+000043e0: 2061 6c73 6f20 7265 636f 676e 697a 6564   also recognized
+000043f0: 2062 7920 7374 6174 6963 2074 7970 6520   by static type 
+00004400: 6368 6563 6b65 7273 2061 6e64 2070 7265  checkers and pre
+00004410: 7665 6e74 7320 7375 6263 6c61 7373 696e  vents subclassin
+00004420: 6720 616e 642f 6f72 206d 656d 6265 7220  g and/or member 
+00004430: 6f76 6572 7269 6469 6e67 2064 7572 696e  overriding durin
+00004440: 6720 7275 6e74 696d 653a 0a0a 2e2e 2063  g runtime:.... c
+00004450: 6f64 653a 3a20 7079 7468 6f6e 0a0a 2020  ode:: python..  
+00004460: 2020 3e3e 3e20 6672 6f6d 2073 6978 2069    >>> from six i
+00004470: 6d70 6f72 7420 7769 7468 5f6d 6574 6163  mport with_metac
+00004480: 6c61 7373 0a20 2020 203e 3e3e 2066 726f  lass.    >>> fro
+00004490: 6d20 6261 7369 6363 6f2e 7275 6e74 696d  m basicco.runtim
+000044a0: 655f 6669 6e61 6c20 696d 706f 7274 2052  e_final import R
+000044b0: 756e 7469 6d65 4669 6e61 6c4d 6574 612c  untimeFinalMeta,
+000044c0: 2066 696e 616c 0a20 2020 203e 3e3e 2040   final.    >>> @
+000044d0: 6669 6e61 6c0a 2020 2020 2e2e 2e20 636c  final.    ... cl
+000044e0: 6173 7320 4173 7365 7428 7769 7468 5f6d  ass Asset(with_m
+000044f0: 6574 6163 6c61 7373 2852 756e 7469 6d65  etaclass(Runtime
+00004500: 4669 6e61 6c4d 6574 612c 206f 626a 6563  FinalMeta, objec
+00004510: 7429 293a 0a20 2020 202e 2e2e 2020 2020  t)):.    ...    
+00004520: 2070 6173 730a 2020 2020 2e2e 2e0a 2020   pass.    ....  
+00004530: 2020 3e3e 3e20 636c 6173 7320 5375 6241    >>> class SubA
+00004540: 7373 6574 2841 7373 6574 293a 0a20 2020  sset(Asset):.   
+00004550: 202e 2e2e 2020 2020 2070 6173 730a 2020   ...     pass.  
+00004560: 2020 2e2e 2e0a 2020 2020 5472 6163 6562    ....    Traceb
+00004570: 6163 6b20 286d 6f73 7420 7265 6365 6e74  ack (most recent
+00004580: 2063 616c 6c20 6c61 7374 293a 0a20 2020   call last):.   
+00004590: 2054 7970 6545 7272 6f72 3a20 6361 6e27   TypeError: can'
+000045a0: 7420 7375 6263 6c61 7373 2066 696e 616c  t subclass final
+000045b0: 2063 6c61 7373 2027 4173 7365 7427 0a0a   class 'Asset'..
+000045c0: 2e2e 2063 6f64 653a 3a20 7079 7468 6f6e  .. code:: python
+000045d0: 0a0a 2020 2020 3e3e 3e20 6672 6f6d 2073  ..    >>> from s
+000045e0: 6978 2069 6d70 6f72 7420 7769 7468 5f6d  ix import with_m
+000045f0: 6574 6163 6c61 7373 0a20 2020 203e 3e3e  etaclass.    >>>
+00004600: 2066 726f 6d20 6261 7369 6363 6f2e 7275   from basicco.ru
+00004610: 6e74 696d 655f 6669 6e61 6c20 696d 706f  ntime_final impo
+00004620: 7274 2052 756e 7469 6d65 4669 6e61 6c4d  rt RuntimeFinalM
+00004630: 6574 612c 2066 696e 616c 0a20 2020 203e  eta, final.    >
+00004640: 3e3e 2063 6c61 7373 2041 7373 6574 2877  >> class Asset(w
+00004650: 6974 685f 6d65 7461 636c 6173 7328 5275  ith_metaclass(Ru
+00004660: 6e74 696d 6546 696e 616c 4d65 7461 2c20  ntimeFinalMeta, 
+00004670: 6f62 6a65 6374 2929 3a0a 2020 2020 2e2e  object)):.    ..
+00004680: 2e20 2020 2020 4066 696e 616c 0a20 2020  .     @final.   
+00004690: 202e 2e2e 2020 2020 2064 6566 206d 6574   ...     def met
+000046a0: 686f 6428 7365 6c66 293a 0a20 2020 202e  hod(self):.    .
+000046b0: 2e2e 2020 2020 2020 2020 2070 6173 730a  ..         pass.
+000046c0: 2020 2020 2e2e 2e0a 2020 2020 3e3e 3e20      ....    >>> 
+000046d0: 636c 6173 7320 5375 6241 7373 6574 2841  class SubAsset(A
+000046e0: 7373 6574 293a 0a20 2020 202e 2e2e 2020  sset):.    ...  
+000046f0: 2020 2064 6566 206d 6574 686f 6428 7365     def method(se
+00004700: 6c66 293a 0a20 2020 202e 2e2e 2020 2020  lf):.    ...    
+00004710: 2020 2020 2070 6173 730a 2020 2020 5472       pass.    Tr
+00004720: 6163 6562 6163 6b20 286d 6f73 7420 7265  aceback (most re
+00004730: 6365 6e74 2063 616c 6c20 6c61 7374 293a  cent call last):
+00004740: 0a20 2020 2054 7970 6545 7272 6f72 3a20  .    TypeError: 
+00004750: 2753 7562 4173 7365 7427 206f 7665 7272  'SubAsset' overr
+00004760: 6964 6573 2066 696e 616c 206d 656d 6265  ides final membe
+00004770: 7220 276d 6574 686f 6427 2064 6566 696e  r 'method' defin
+00004780: 6564 2062 7920 2741 7373 6574 270a 0a2e  ed by 'Asset'...
+00004790: 2e20 636f 6465 3a3a 2070 7974 686f 6e0a  . code:: python.
+000047a0: 0a20 2020 203e 3e3e 2066 726f 6d20 7369  .    >>> from si
+000047b0: 7820 696d 706f 7274 2077 6974 685f 6d65  x import with_me
+000047c0: 7461 636c 6173 730a 2020 2020 3e3e 3e20  taclass.    >>> 
+000047d0: 6672 6f6d 2062 6173 6963 636f 2e72 756e  from basicco.run
+000047e0: 7469 6d65 5f66 696e 616c 2069 6d70 6f72  time_final impor
+000047f0: 7420 5275 6e74 696d 6546 696e 616c 4d65  t RuntimeFinalMe
+00004800: 7461 2c20 6669 6e61 6c0a 2020 2020 3e3e  ta, final.    >>
+00004810: 3e20 636c 6173 7320 4173 7365 7428 7769  > class Asset(wi
+00004820: 7468 5f6d 6574 6163 6c61 7373 2852 756e  th_metaclass(Run
+00004830: 7469 6d65 4669 6e61 6c4d 6574 612c 206f  timeFinalMeta, o
+00004840: 626a 6563 7429 293a 0a20 2020 202e 2e2e  bject)):.    ...
+00004850: 2020 2020 2040 7072 6f70 6572 7479 0a20       @property. 
+00004860: 2020 202e 2e2e 2020 2020 2040 6669 6e61     ...     @fina
+00004870: 6c0a 2020 2020 2e2e 2e20 2020 2020 6465  l.    ...     de
+00004880: 6620 7072 6f70 2873 656c 6629 3a0a 2020  f prop(self):.  
+00004890: 2020 2e2e 2e20 2020 2020 2020 2020 7061    ...         pa
+000048a0: 7373 0a20 2020 202e 2e2e 0a20 2020 203e  ss.    ....    >
+000048b0: 3e3e 2063 6c61 7373 2053 7562 4173 7365  >> class SubAsse
+000048c0: 7428 4173 7365 7429 3a0a 2020 2020 2e2e  t(Asset):.    ..
+000048d0: 2e20 2020 2020 4070 726f 7065 7274 790a  .     @property.
+000048e0: 2020 2020 2e2e 2e20 2020 2020 6465 6620      ...     def 
+000048f0: 7072 6f70 2873 656c 6629 3a0a 2020 2020  prop(self):.    
+00004900: 2e2e 2e20 2020 2020 2020 2020 7061 7373  ...         pass
+00004910: 0a20 2020 2054 7261 6365 6261 636b 2028  .    Traceback (
+00004920: 6d6f 7374 2072 6563 656e 7420 6361 6c6c  most recent call
+00004930: 206c 6173 7429 3a0a 2020 2020 5479 7065   last):.    Type
+00004940: 4572 726f 723a 2027 5375 6241 7373 6574  Error: 'SubAsset
+00004950: 2720 6f76 6572 7269 6465 7320 6669 6e61  ' overrides fina
+00004960: 6c20 6d65 6d62 6572 2027 7072 6f70 2720  l member 'prop' 
+00004970: 6465 6669 6e65 6420 6279 2027 4173 7365  defined by 'Asse
+00004980: 7427 0a0a 7361 6665 5f6e 6f74 5f65 7175  t'..safe_not_equ
+00004990: 616c 730a 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e  als.^^^^^^^^^^^^
+000049a0: 5e5e 5e0a 4261 636b 706f 7274 206f 6620  ^^^.Backport of 
+000049b0: 7468 6520 6465 6661 756c 7420 5079 7468  the default Pyth
+000049c0: 6f6e 2033 2062 6568 6176 696f 7220 6f66  on 3 behavior of
+000049d0: 2060 5f5f 6e65 5f5f 6020 6265 6861 7669   `__ne__` behavi
+000049e0: 6f72 2066 6f72 2050 7974 686f 6e20 322e  or for Python 2.
+000049f0: 372e 0a0a 2e2e 2063 6f64 653a 3a20 7079  7..... code:: py
+00004a00: 7468 6f6e 0a0a 2020 2020 3e3e 3e20 6672  thon..    >>> fr
+00004a10: 6f6d 2073 6978 2069 6d70 6f72 7420 7769  om six import wi
+00004a20: 7468 5f6d 6574 6163 6c61 7373 0a20 2020  th_metaclass.   
+00004a30: 203e 3e3e 2066 726f 6d20 6261 7369 6363   >>> from basicc
+00004a40: 6f2e 7361 6665 5f6e 6f74 5f65 7175 616c  o.safe_not_equal
+00004a50: 7320 696d 706f 7274 2053 6166 654e 6f74  s import SafeNot
+00004a60: 4571 7561 6c73 4d65 7461 0a20 2020 203e  EqualsMeta.    >
+00004a70: 3e3e 2063 6c61 7373 2043 6c61 7373 2877  >> class Class(w
+00004a80: 6974 685f 6d65 7461 636c 6173 7328 5361  ith_metaclass(Sa
+00004a90: 6665 4e6f 7445 7175 616c 734d 6574 612c  feNotEqualsMeta,
+00004aa0: 206f 626a 6563 7429 293a 0a20 2020 202e   object)):.    .
+00004ab0: 2e2e 2020 2020 2070 6173 730a 2020 2020  ..     pass.    
+00004ac0: 2e2e 2e0a 2020 2020 3e3e 3e20 6f62 6a5f  ....    >>> obj_
+00004ad0: 6120 3d20 436c 6173 7328 290a 2020 2020  a = Class().    
+00004ae0: 3e3e 3e20 6f62 6a5f 6220 3d20 436c 6173  >>> obj_b = Clas
+00004af0: 7328 290a 2020 2020 3e3e 3e20 6173 7365  s().    >>> asse
+00004b00: 7274 2028 6f62 6a5f 6120 3d3d 206f 626a  rt (obj_a == obj
+00004b10: 5f61 2920 6973 206e 6f74 2028 6f62 6a5f  _a) is not (obj_
+00004b20: 6120 213d 206f 626a 5f61 290a 2020 2020  a != obj_a).    
+00004b30: 3e3e 3e20 6173 7365 7274 2028 6f62 6a5f  >>> assert (obj_
+00004b40: 6220 3d3d 206f 626a 5f62 2920 6973 206e  b == obj_b) is n
+00004b50: 6f74 2028 6f62 6a5f 6220 213d 206f 626a  ot (obj_b != obj
+00004b60: 5f62 290a 2020 2020 3e3e 3e20 6173 7365  _b).    >>> asse
+00004b70: 7274 2028 6f62 6a5f 6120 3d3d 206f 626a  rt (obj_a == obj
+00004b80: 5f62 2920 6973 206e 6f74 2028 6f62 6a5f  _b) is not (obj_
+00004b90: 6120 213d 206f 626a 5f62 290a 0a73 6166  a != obj_b)..saf
+00004ba0: 655f 7265 7072 0a5e 5e5e 5e5e 5e5e 5e5e  e_repr.^^^^^^^^^
+00004bb0: 0a44 6563 6f72 6174 6f72 2074 6861 7420  .Decorator that 
+00004bc0: 7072 6576 656e 7473 2060 5f5f 7265 7072  prevents `__repr
+00004bd0: 5f5f 6020 6d65 7468 6f64 7320 6672 6f6d  __` methods from
+00004be0: 2072 6169 7369 6e67 2065 7863 6570 7469   raising excepti
+00004bf0: 6f6e 7320 616e 6420 7265 7475 726e 2061  ons and return a
+00004c00: 2064 6566 6175 6c74 2072 6570 7265 7365   default represe
+00004c10: 6e74 6174 696f 6e20 696e 7374 6561 642e  ntation instead.
+00004c20: 0a0a 2e2e 2063 6f64 653a 3a20 7079 7468  .... code:: pyth
+00004c30: 6f6e 0a0a 2020 2020 3e3e 3e20 6672 6f6d  on..    >>> from
+00004c40: 2062 6173 6963 636f 2e73 6166 655f 7265   basicco.safe_re
+00004c50: 7072 2069 6d70 6f72 7420 7361 6665 5f72  pr import safe_r
+00004c60: 6570 720a 2020 2020 3e3e 3e20 636c 6173  epr.    >>> clas
+00004c70: 7320 436c 6173 7328 6f62 6a65 6374 293a  s Class(object):
+00004c80: 0a20 2020 202e 2e2e 2020 2020 2040 7361  .    ...     @sa
+00004c90: 6665 5f72 6570 720a 2020 2020 2e2e 2e20  fe_repr.    ... 
+00004ca0: 2020 2020 6465 6620 5f5f 7265 7072 5f5f      def __repr__
+00004cb0: 2873 656c 6629 3a0a 2020 2020 2e2e 2e20  (self):.    ... 
+00004cc0: 2020 2020 2020 2020 7261 6973 6520 5275          raise Ru
+00004cd0: 6e74 696d 6545 7272 6f72 2822 6f68 206f  ntimeError("oh o
+00004ce0: 6822 290a 2020 2020 2e2e 2e0a 2020 2020  h").    ....    
+00004cf0: 3e3e 3e20 6f62 6a20 3d20 436c 6173 7328  >>> obj = Class(
+00004d00: 290a 2020 2020 3e3e 3e20 7265 7072 286f  ).    >>> repr(o
+00004d10: 626a 290a 2020 2020 223c 5f5f 6d61 696e  bj).    "<__main
+00004d20: 5f5f 2e43 6c61 7373 206f 626a 6563 7420  __.Class object 
+00004d30: 6174 202e 2e2e 3b20 7265 7072 2066 6169  at ...; repr fai
+00004d40: 6c65 6420 6475 6520 746f 2027 5275 6e74  led due to 'Runt
+00004d50: 696d 6545 7272 6f72 3a20 6f68 206f 6827  imeError: oh oh'
+00004d60: 3e22 0a0a 7365 745f 6e61 6d65 0a5e 5e5e  >"..set_name.^^^
+00004d70: 5e5e 5e5e 5e0a 4261 636b 706f 7274 206f  ^^^^^.Backport o
+00004d80: 6620 7468 6520 6675 6e63 7469 6f6e 616c  f the functional
+00004d90: 6974 7920 6f66 2060 5f5f 7365 745f 6e61  ity of `__set_na
+00004da0: 6d65 5f5f 6020 6672 6f6d 2050 4550 2034  me__` from PEP 4
+00004db0: 3837 2074 6f20 5079 7468 6f6e 2032 2e37  87 to Python 2.7
+00004dc0: 2e0a 0a2e 2e20 636f 6465 3a3a 2070 7974  ..... code:: pyt
+00004dd0: 686f 6e0a 0a20 2020 203e 3e3e 2066 726f  hon..    >>> fro
+00004de0: 6d20 6261 7369 6363 6f2e 7365 745f 6e61  m basicco.set_na
+00004df0: 6d65 2069 6d70 6f72 7420 5365 744e 616d  me import SetNam
+00004e00: 650a 2020 2020 3e3e 3e20 636c 6173 7320  e.    >>> class 
+00004e10: 4174 7472 6962 7574 6528 6f62 6a65 6374  Attribute(object
+00004e20: 293a 0a20 2020 202e 2e2e 2020 2020 2064  ):.    ...     d
+00004e30: 6566 205f 5f73 6574 5f6e 616d 655f 5f28  ef __set_name__(
+00004e40: 7365 6c66 2c20 6f77 6e65 722c 206e 616d  self, owner, nam
+00004e50: 6529 3a0a 2020 2020 2e2e 2e20 2020 2020  e):.    ...     
+00004e60: 2020 2020 7365 6c66 2e6f 776e 6572 203d      self.owner =
+00004e70: 206f 776e 6572 0a20 2020 202e 2e2e 2020   owner.    ...  
+00004e80: 2020 2020 2020 2073 656c 662e 6e61 6d65         self.name
+00004e90: 203d 206e 616d 650a 2020 2020 2e2e 2e0a   = name.    ....
+00004ea0: 2020 2020 3e3e 3e20 636c 6173 7320 436f      >>> class Co
+00004eb0: 6c6c 6563 7469 6f6e 2853 6574 4e61 6d65  llection(SetName
+00004ec0: 293a 0a20 2020 202e 2e2e 2020 2020 2066  ):.    ...     f
+00004ed0: 6f6f 203d 2041 7474 7269 6275 7465 2829  oo = Attribute()
+00004ee0: 0a20 2020 202e 2e2e 0a20 2020 203e 3e3e  .    ....    >>>
+00004ef0: 2043 6f6c 6c65 6374 696f 6e2e 666f 6f2e   Collection.foo.
+00004f00: 6f77 6e65 7220 6973 2043 6f6c 6c65 6374  owner is Collect
+00004f10: 696f 6e0a 2020 2020 5472 7565 0a20 2020  ion.    True.   
+00004f20: 203e 3e3e 2043 6f6c 6c65 6374 696f 6e2e   >>> Collection.
+00004f30: 666f 6f2e 6e61 6d65 0a20 2020 2027 666f  foo.name.    'fo
+00004f40: 6f27 0a0a 7479 7065 5f63 6865 636b 696e  o'..type_checkin
+00004f50: 670a 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e 5e0a  g.^^^^^^^^^^^^^.
+00004f60: 5275 6e74 696d 6520 7479 7065 2063 6865  Runtime type che
+00004f70: 636b 696e 6720 7769 7468 2073 7570 706f  cking with suppo
+00004f80: 7274 2066 6f72 2069 6d70 6f72 7420 7061  rt for import pa
+00004f90: 7468 7320 616e 6420 7479 7065 2068 696e  ths and type hin
+00004fa0: 7473 2e0a 0a2e 2e20 636f 6465 3a3a 2070  ts..... code:: p
+00004fb0: 7974 686f 6e0a 0a20 2020 203e 3e3e 2066  ython..    >>> f
+00004fc0: 726f 6d20 7469 7070 6f20 696d 706f 7274  rom tippo import
+00004fd0: 204d 6170 7069 6e67 2c20 4c69 7465 7261   Mapping, Litera
+00004fe0: 6c0a 2020 2020 3e3e 3e20 6672 6f6d 2069  l.    >>> from i
+00004ff0: 7465 7274 6f6f 6c73 2069 6d70 6f72 7420  tertools import 
+00005000: 6368 6169 6e0a 2020 2020 3e3e 3e20 6672  chain.    >>> fr
+00005010: 6f6d 2062 6173 6963 636f 2e74 7970 655f  om basicco.type_
+00005020: 6368 6563 6b69 6e67 2069 6d70 6f72 7420  checking import 
+00005030: 6973 5f69 6e73 7461 6e63 650a 2020 2020  is_instance.    
+00005040: 3e3e 3e20 636c 6173 7320 5375 6243 6861  >>> class SubCha
+00005050: 696e 2863 6861 696e 293a 0a20 2020 202e  in(chain):.    .
+00005060: 2e2e 2020 2020 2070 6173 730a 2020 2020  ..     pass.    
+00005070: 2e2e 2e0a 2020 2020 3e3e 3e20 6973 5f69  ....    >>> is_i
+00005080: 6e73 7461 6e63 6528 332c 2069 6e74 290a  nstance(3, int).
+00005090: 2020 2020 5472 7565 0a20 2020 203e 3e3e      True.    >>>
+000050a0: 2069 735f 696e 7374 616e 6365 2833 2c20   is_instance(3, 
+000050b0: 2863 6861 696e 2c20 696e 7429 290a 2020  (chain, int)).  
+000050c0: 2020 5472 7565 0a20 2020 203e 3e3e 2069    True.    >>> i
+000050d0: 735f 696e 7374 616e 6365 2833 2c20 2829  s_instance(3, ()
+000050e0: 290a 2020 2020 4661 6c73 650a 2020 2020  ).    False.    
+000050f0: 3e3e 3e20 6973 5f69 6e73 7461 6e63 6528  >>> is_instance(
+00005100: 5375 6243 6861 696e 2829 2c20 2269 7465  SubChain(), "ite
+00005110: 7274 6f6f 6c73 2e63 6861 696e 2229 0a20  rtools.chain"). 
+00005120: 2020 2054 7275 650a 2020 2020 3e3e 3e20     True.    >>> 
+00005130: 6973 5f69 6e73 7461 6e63 6528 6368 6169  is_instance(chai
+00005140: 6e28 292c 2022 6974 6572 746f 6f6c 732e  n(), "itertools.
+00005150: 6368 6169 6e22 2c20 7375 6274 7970 6573  chain", subtypes
+00005160: 3d46 616c 7365 290a 2020 2020 5472 7565  =False).    True
+00005170: 0a20 2020 203e 3e3e 2069 735f 696e 7374  .    >>> is_inst
+00005180: 616e 6365 2853 7562 4368 6169 6e28 292c  ance(SubChain(),
+00005190: 2022 6974 6572 746f 6f6c 732e 6368 6169   "itertools.chai
+000051a0: 6e22 2c20 7375 6274 7970 6573 3d46 616c  n", subtypes=Fal
+000051b0: 7365 290a 2020 2020 4661 6c73 650a 2020  se).    False.  
+000051c0: 2020 3e3e 3e20 6973 5f69 6e73 7461 6e63    >>> is_instanc
+000051d0: 6528 7b22 6122 3a20 312c 2022 6222 3a20  e({"a": 1, "b": 
+000051e0: 327d 2c20 4d61 7070 696e 675b 7374 722c  2}, Mapping[str,
+000051f0: 2069 6e74 5d29 0a20 2020 2054 7275 650a   int]).    True.
+00005200: 2020 2020 3e3e 3e20 6973 5f69 6e73 7461      >>> is_insta
+00005210: 6e63 6528 2250 5245 222c 204c 6974 6572  nce("PRE", Liter
+00005220: 616c 5b22 5052 4522 2c20 2250 4f53 5422  al["PRE", "POST"
+00005230: 5d29 0a20 2020 2054 7275 650a 0a75 6e69  ]).    True..uni
+00005240: 7175 655f 6974 6572 6174 6f72 0a5e 5e5e  que_iterator.^^^
+00005250: 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e 0a49 7465  ^^^^^^^^^^^^.Ite
+00005260: 7261 746f 7220 7468 6174 2079 6965 6c64  rator that yield
+00005270: 7320 756e 6971 7565 2076 616c 7565 732e  s unique values.
+00005280: 0a0a 2e2e 2063 6f64 653a 3a20 7079 7468  .... code:: pyth
+00005290: 6f6e 0a0a 2020 2020 3e3e 3e20 6672 6f6d  on..    >>> from
+000052a0: 2062 6173 6963 636f 2e75 6e69 7175 655f   basicco.unique_
+000052b0: 6974 6572 6174 6f72 2069 6d70 6f72 7420  iterator import 
+000052c0: 756e 6971 7565 5f69 7465 7261 746f 720a  unique_iterator.
+000052d0: 2020 2020 3e3e 3e20 6c69 7374 2875 6e69      >>> list(uni
+000052e0: 7175 655f 6974 6572 6174 6f72 285b 312c  que_iterator([1,
+000052f0: 2032 2c20 332c 2033 2c20 342c 2034 2c20   2, 3, 3, 4, 4, 
+00005300: 355d 2929 0a20 2020 205b 312c 2032 2c20  5])).    [1, 2, 
+00005310: 332c 2034 2c20 355d 0a0a 7765 616b 5f72  3, 4, 5]..weak_r
+00005320: 6566 6572 656e 6365 0a5e 5e5e 5e5e 5e5e  eference.^^^^^^^
+00005330: 5e5e 5e5e 5e5e 5e0a 5765 616b 2052 6566  ^^^^^^^.Weak Ref
+00005340: 6572 656e 6365 2d6c 696b 6520 6f62 6a65  erence-like obje
+00005350: 6374 2074 6861 7420 7375 7070 6f72 7473  ct that supports
+00005360: 2070 6963 6b6c 696e 672e 0a               pickling..
```

### Comparing `basicco-8.9.0/basicco/__init__.py` & `basicco-9.0.0/basicco/__init__.py`

 * *Files identical despite different names*

### Comparing `basicco-8.9.0/basicco/_bases.py` & `basicco-9.0.0/basicco/_bases.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,23 +3,17 @@
 from tippo import GenericMeta
 
 from .abstract_class import Abstract, AbstractMeta, abstract, is_abstract
 from .default_dir import DefaultDir, DefaultDirMeta
 from .explicit_hash import ExplicitHash, ExplicitHashMeta
 from .implicit_hash import ImplicitHash, ImplicitHashMeta
 from .init_subclass import InitSubclass, InitSubclassMeta
-from .locked_class import (
-    LockedClass,
-    LockedClassMeta,
-    is_locked,
-    set_locked,
-    unlocked_context,
-)
+from .locked_class import LockedClass, LockedClassMeta, is_locked, set_locked, unlocked_context
 from .namespace import Namespaced, NamespacedMeta
-from .obj_state import Reducible, ReducibleMeta
+from .obj_state import Reducible, ReducibleMeta, get_state, update_state
 from .qualname import Qualnamed, QualnamedMeta
 from .runtime_final import RuntimeFinal, RuntimeFinalMeta, final
 from .safe_not_equals import SafeNotEquals, SafeNotEqualsMeta
 from .set_name import SetName, SetNameMeta
 
 __all__ = [
     "CompatBaseMeta",
@@ -89,14 +83,20 @@
         CompatBase,
     )
 ):
     """Base class that adds extra features to the basic `object`."""
 
     __slots__ = ("__weakref__",)
 
+    def __copy__(self):
+        cls = type(self)
+        new_self = cls.__new__(cls)
+        update_state(new_self, get_state(self))
+        return new_self
+
 
 class SlottedBaseMeta(BaseMeta, slotted.SlottedABCGenericMeta):
     """Slotted base metaclass."""
 
 
 class SlottedBase(six.with_metaclass(SlottedBaseMeta, Base, slotted.SlottedABC)):
     """Slotted base class."""
```

### Comparing `basicco-8.9.0/basicco/abstract_class.py` & `basicco-9.0.0/basicco/abstract_class.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,14 +133,15 @@
     """Metaclass that finds abstract members in properties and descriptors for both Python 2.7 and 3.7+."""
 
     def __init__(cls, name, bases, dct, **kwargs):
         super(AbstractMeta, cls).__init__(name, bases, dct, **kwargs)  # noqa
         cls.__gather_abstract_members()
 
     def __gather_abstract_members(cls):
+        # type: () -> None
 
         # Iterate over MRO of the class.
         abstract_method_names = set()  # type: Set[str]
         for base in reversed(get_mro(cls)):
 
             # Find abstract members.
             for member_name, member in six.iteritems(base.__dict__):
```

### Comparing `basicco-8.9.0/basicco/context_vars.py` & `basicco-9.0.0/basicco/context_vars.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,24 +12,15 @@
 except ImportError:
     import enum
     import threading
 
     import pyrsistent
     import six
     from pyrsistent.typing import PMap
-    from tippo import (
-        Any,
-        Callable,
-        Generic,
-        GenericMeta,
-        Iterator,
-        Mapping,
-        TypeVar,
-        overload,
-    )
+    from tippo import Any, Callable, Generic, GenericMeta, Iterator, Mapping, TypeVar, overload
 
     class _NoDefaultType(enum.Enum):
         NO_DEFAULT = "NO_DEFAULT"
 
     _NO_DEFAULT = _NoDefaultType.NO_DEFAULT
     _MODULE = __name__
```

### Comparing `basicco-8.9.0/basicco/custom_repr.py` & `basicco-9.0.0/basicco/custom_repr.py`

 * *Files identical despite different names*

### Comparing `basicco-8.9.0/basicco/default_dir.py` & `basicco-9.0.0/basicco/default_dir.py`

 * *Files identical despite different names*

### Comparing `basicco-8.9.0/basicco/dynamic_code.py` & `basicco-9.0.0/basicco/dynamic_code.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from tippo import Any, Callable
 
 __all__ = ["compile_and_eval", "generate_unique_filename", "make_function"]
 
 
 def compile_and_eval(script, globs=None, locs=None, filename=""):
-    # type: (str, dict[str, Any], dict[str, Any] | None, str) -> None
+    # type: (str, dict[str, Any] | None, dict[str, Any] | None, str) -> None
     """
     Evaluate the script with the given globals and locals.
 
     :param script: Script.
     :param globs: Globals.
     :param locs: Locals.
     :param filename: Filename.
@@ -39,38 +39,38 @@
     elif module is not None:
         return "<generated {}.{}>".format(module, obj_name)
     else:
         return "<generated {}>".format(obj_name)
 
 
 def make_function(name, script, globs=None, filename=None, module=None):
-    # type: (str, str, dict[str, Any], str | None, str | None) -> Callable
+    # type: (str, str, dict[str, Any] | None, str | None, str | None) -> Callable
     """
     Create a function with the given script.
 
     :param name: Function name.
     :param script: Script.
     :param filename: Filename.
     :param globs: Globals.
     :param module: Module name.
     :return: Function object.
     """
 
-    # Add a fake linecache entry for debuggers.
+    # Add a fake linecache entry for debuggers.  # FIXME: infinite looping here when dup function is generated
     if filename:
         count = 1
         base_filename = complete_filename = filename  # type: str
         while True:
             linecache_tuple = (
                 len(script),
                 None,
                 script.splitlines(True),
                 complete_filename,
             )  # type: tuple[int, float | None, list[str], str]
-            old_val = linecache.cache.setdefault(filename, linecache_tuple)
+            old_val = linecache.cache.setdefault(complete_filename, linecache_tuple)
             if old_val == linecache_tuple:
                 break
             else:
                 complete_filename = "{}-{}>".format(base_filename[:-1], count)
                 count += 1
     else:
         complete_filename = ""
```

### Comparing `basicco-8.9.0/basicco/explicit_hash.py` & `basicco-9.0.0/basicco/explicit_hash.py`

 * *Files identical despite different names*

### Comparing `basicco-8.9.0/basicco/fabricate_value.py` & `basicco-9.0.0/basicco/fabricate_value.py`

 * *Files identical despite different names*

### Comparing `basicco-8.9.0/basicco/get_mro.py` & `basicco-9.0.0/basicco/get_mro.py`

 * *Files identical despite different names*

### Comparing `basicco-8.9.0/basicco/implicit_hash.py` & `basicco-9.0.0/basicco/implicit_hash.py`

 * *Files identical despite different names*

### Comparing `basicco-8.9.0/basicco/import_path.py` & `basicco-9.0.0/basicco/import_path.py`

 * *Files identical despite different names*

### Comparing `basicco-8.9.0/basicco/init_subclass.py` & `basicco-9.0.0/basicco/init_subclass.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,14 +63,15 @@
                 method = base.__dict__.get("__init_subclass__")
                 if method is not None:
                     method_owner = base
                     break
 
             # Found a method.
             if method is not None:
+                assert method_owner is not None
 
                 # Invalid base.
                 if not isinstance(method_owner, InitSubclassMeta):
                     error = "base {!r} defines '__init_subclass__' but does not utilize {!r} as a metaclass".format(
                         method_owner.__name__, InitSubclassMeta.__name__
                     )
                     raise TypeError(error)
```

### Comparing `basicco-8.9.0/basicco/locked_class.py` & `basicco-9.0.0/basicco/locked_class.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,34 +19,36 @@
     :param cls: Class.
     :return: True if locked.
     """
     locked_attr = mangle("__locked", cls.__name__)
     try:
         locked = getattr(cls, locked_attr)
     except AttributeError:
-        pass
+        assert_is_instance(cls, LockedClassMeta)
+        return True
     else:
         return locked
-    assert_is_instance(cls, LockedClassMeta)
-    raise
 
 
 def set_locked(cls, locked):
     # type: (Type[LockedClass] | LockedClassMeta, bool) -> None
     """
     Set class locked state.
 
     :param cls: Class.
     :param locked: Locked state.
     :raise TypeCheckError: Invalid class type.
     """
     locked_attr = mangle("__locked", cls.__name__)
     if not hasattr(cls, locked_attr):
         assert_is_instance(cls, LockedClassMeta)
-    type.__setattr__(cls, locked_attr, locked)
+    elif not locked:
+        type.__setattr__(cls, locked_attr, False)
+    else:
+        type.__delattr__(cls, locked_attr)
 
 
 @contextlib.contextmanager
 def unlocked_context(cls):
     # type: (Type[LockedClass] | LockedClassMeta) -> Iterator
     """
     Unlocked class context manager.
@@ -63,25 +65,28 @@
         if before:
             set_locked(cls, True)
 
 
 class LockedClassMeta(type):
     """Metaclass that prevents changing public class attributes."""
 
+    def __new__(mcs, name, bases, dct, **kwargs):
+        dct = dict(dct)
+        dct[mangle("__locked", name)] = False
+        return super(LockedClassMeta, mcs).__new__(mcs, name, bases, dct, **kwargs)
+
     def __init__(cls, name, bases, dct, **kwargs):
         super(LockedClassMeta, cls).__init__(name, bases, dct, **kwargs)
         if not is_locked(cls):
             set_locked(cls, True)
 
     def __getattr__(cls, name):
         # type: (str) -> Any
-        locked_attr = mangle("__locked", cls.__name__)
-        if name == locked_attr:
-            type.__setattr__(cls, locked_attr, False)
-            return False
+        if name == mangle("__locked", cls.__name__):
+            return True
         try:
             return super(LockedClassMeta, cls).__getattr__(name)  # type: ignore  # noqa
         except AttributeError:
             pass
         error = "class {!r} has no attribute {!r}".format(cls.__name__, name)
         raise AttributeError(error)
```

### Comparing `basicco-8.9.0/basicco/mangling.py` & `basicco-9.0.0/basicco/mangling.py`

 * *Files identical despite different names*

### Comparing `basicco-8.9.0/basicco/mapping_proxy.py` & `basicco-9.0.0/basicco/mapping_proxy.py`

 * *Files identical despite different names*

### Comparing `basicco-8.9.0/basicco/named_tuple.py` & `basicco-9.0.0/basicco/named_tuple.py`

 * *Files identical despite different names*

### Comparing `basicco-8.9.0/basicco/namespace.py` & `basicco-9.0.0/basicco/namespace.py`

 * *Files identical despite different names*

### Comparing `basicco-8.9.0/basicco/obj_state.py` & `basicco-9.0.0/basicco/obj_state.py`

 * *Files identical despite different names*

### Comparing `basicco-8.9.0/basicco/qualname.py` & `basicco-9.0.0/basicco/qualname.py`

 * *Files identical despite different names*

### Comparing `basicco-8.9.0/basicco/recursive_repr.py` & `basicco-9.0.0/basicco/recursive_repr.py`

 * *Files identical despite different names*

### Comparing `basicco-8.9.0/basicco/runtime_final.py` & `basicco-9.0.0/basicco/runtime_final.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,14 +75,15 @@
     """Metaclass that enables runtime-checking for `final` decorator."""
 
     def __init__(cls, name, bases, dct, **kwargs):
         super(RuntimeFinalMeta, cls).__init__(name, bases, dct, **kwargs)
         cls.__gather_final_members()
 
     def __gather_final_members(cls):
+        # type: () -> None
 
         # Iterate over MRO of the class.
         final_cls = None  # type: Type | None
         final_member_names = {}  # type: dict[str, Type]
         mro = get_mro(cls)
         for base in reversed(mro):
             if base is object:
```

### Comparing `basicco-8.9.0/basicco/safe_not_equals.py` & `basicco-9.0.0/basicco/safe_not_equals.py`

 * *Files identical despite different names*

### Comparing `basicco-8.9.0/basicco/safe_repr.py` & `basicco-9.0.0/basicco/safe_repr.py`

 * *Files identical despite different names*

### Comparing `basicco-8.9.0/basicco/set_name.py` & `basicco-9.0.0/basicco/set_name.py`

 * *Files identical despite different names*

### Comparing `basicco-8.9.0/basicco/type_checking.py` & `basicco-9.0.0/basicco/type_checking.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,14 @@
 """Runtime type checking with support for import paths and type hints."""
 
 import itertools
 
 import six
 import typing_inspect  # type: ignore
-from tippo import (
-    Any,
-    Callable,
-    ForwardRef,
-    Iterable,
-    Mapping,
-    Type,
-    TypeVar,
-    cast,
-    get_args,
-    get_origin,
-    get_typing,
-)
+from tippo import Any, Callable, ForwardRef, Iterable, Mapping, Type, TypeVar, cast, get_args, get_origin, get_typing
 
 from .import_path import get_name, import_path
 
 __all__ = [
     "TEXT_TYPES",
     "TypeCheckError",
     "type_names",
@@ -92,15 +80,15 @@
 
 
 def _check_mapping(obj, mapping, type_depth, instance, typing, *args):
     origin = get_origin(mapping)
     if type_depth or not instance:
         return _check(obj, origin, type_depth, instance, False, *args)
 
-    if not isinstance(obj, origin):
+    if not isinstance(obj, origin):  # type: ignore
         return False
 
     mapping_args = get_args(mapping)
     if not mapping_args:
         return True
 
     assert len(mapping_args) == 2
@@ -115,15 +103,15 @@
 
 
 def _check_iterable(obj, iterable, type_depth, instance, typing, *args):
     origin = get_origin(iterable)
     if type_depth or not instance:
         return _check(obj, origin, type_depth, instance, False, *args)
 
-    if not isinstance(obj, origin):
+    if not isinstance(obj, origin):  # type: ignore
         return False
 
     iterable_args = get_args(iterable)
     if not iterable_args:
         return True
 
     assert len(iterable_args) == 1
```

### Comparing `basicco-8.9.0/basicco/weak_reference.py` & `basicco-9.0.0/basicco/weak_reference.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 class WeakReference(Generic[_T]):
     """Weak Reference-like object that supports pickling."""
 
     __slots__ = ("__weakref__", "__ref")
 
     @staticmethod
     def __new__(cls, obj=None):
-        # type: (Type[WeakReference[_T]], _T) -> WeakReference[_T]
+        # type: (Type[WeakReference[_T]], _T | None) -> WeakReference[_T]
         with _lock:
             cache = _cache.setdefault(cls, weakref.WeakValueDictionary())
             if obj is None:
                 obj_ref = _DEAD_REF
             else:
                 obj_ref = weakref.ref(obj)
```

### Comparing `basicco-8.9.0/basicco.egg-info/PKG-INFO` & `basicco-9.0.0/basicco.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: basicco
-Version: 8.9.0
-Summary: Collection of lower-level utilities that enhance code compatibility and validation.
+Version: 9.0.0
+Summary: Base classes and utilities that enhance code compatibility, features and validation.
 Home-page: https://github.com/brunonicko/basicco
 Author: Bruno Nicko
 Author-email: brunonicko@gmail.com
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >= 2.7, != 3.0.*, != 3.1.*, != 3.2.*, != 3.3.*, != 3.4.*, != 3.5.*, != 3.6.*
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 Basicco
 =======
@@ -40,16 +41,15 @@
    :target: https://pepy.tech/project/basicco
 
 .. image:: https://img.shields.io/pypi/pyversions/basicco?color=light-green&style=flat
    :target: https://pypi.org/project/basicco/
 
 Overview
 --------
-`basicco` is a Python package that provides low-level `Base Classes`_ and `Utilities`_ to enhance code compatibility,
-features and validation.
+`Base Classes`_ and `Utilities`_ that enhance code compatibility, features and validation.
 
 Motivation
 ----------
 While developing Python software for Visual Effects pipelines, I found myself having to write the same boiler-plate
 code over and over again, as well as struggling with compatibility issues and feature gaps between Python 2.7 and
 Python 3.7+.
 
@@ -97,16 +97,15 @@
 SlottedBase
 ^^^^^^^^^^^
 The `SlottedBase` class and the `SlottedBaseMeta` metaclass offer all features from `Base` and `BaseMeta` plus implicit
 `__slots__` declaration. See `slotted <https://github.com/brunonicko/slotted>`_ for more information.
 
 Utilities
 ---------
-Apart from the features integrated into the base classes, `basicco` provides a variety of general utilities.
-Those can be imported from the sub-modules described below.
+Apart from the features integrated into the base classes, `basicco` provides many general utility modules.
 
 abstract_class
 ^^^^^^^^^^^^^^
 Better `abstract classes <https://docs.python.org/3/library/abc.html#abc.abstractmethod>`_ support.
 
 Provides abstract decorators that can be used directly on methods but also on classes, properties, classmethods, and
 staticmethods (even in Python 2.7).
@@ -136,40 +135,14 @@
     ... class Asset(with_metaclass(AbstractMeta, object)):
     ...     pass
     ...
     >>> Asset()
     Traceback (most recent call last):
     TypeError: can't instantiate abstract class 'Asset'
 
-basic_data
-^^^^^^^^^^
-Eases the task of creating simple data container classes that support equality comparisons, hashing, string
-representation, conversion to dictionary, etc.
-
-.. code:: python
-
-    >>> from math import sqrt
-    >>> from basicco.basic_data import ItemUsecase, BasicData
-    >>> class Vector(BasicData):
-    ...     __slots__ = ("x", "y")
-    ...     def __init__(self, x, y):
-    ...         self.x = x
-    ...         self.y = y
-    ...     def to_items(self, usecase=None):
-    ...         items = [("x", self.x), ("y", self.y)]
-    ...         if usecase is ItemUsecase.REPR:
-    ...             items.append(("mag", self.mag))
-    ...         return items
-    ...     @property
-    ...     def mag(self):
-    ...         return sqrt(self.x**2 + self.y**2)
-    ...
-    >>> Vector(3.0, 4.0)
-    Vector(x=3.0, y=4.0, <mag=5.0>)
-
 caller_module
 ^^^^^^^^^^^^^
 Retrieve the caller's module name.
 
 .. code:: python
 
     >>> from basicco.caller_module import caller_module
@@ -180,15 +153,15 @@
     'I was called by __main__'
 
 context_vars
 ^^^^^^^^^^^^
 Backport of the `contextvars` module for Python 2.7, based on
 `MagicStack/contextvars <https://github.com/MagicStack/contextvars>`_.
 
-When imported from Python 3, it redirects the contents to the native
+When imported from Python 3, it simply redirects to the native
 `contextvars <https://docs.python.org/3/library/contextvars.html>`_ module.
 
 .. code:: python
 
     >>> from basicco.context_vars import ContextVar
     >>> my_var = ContextVar("my_var", default="bar")
     >>> token = my_var.set("foo")
@@ -219,14 +192,33 @@
 .. code:: python
 
     >>> from basicco.custom_repr import iterable_repr
     >>> tup = ("a", "b", "c", 1, 2, 3)
     >>> iterable_repr(tup, prefix="<", suffix=">", value_repr=str)
     '<a, b, c, 1, 2, 3>'
 
+data_class
+^^^^^^^^^^
+Python 2.7 compatible dataclass-like structures.
+
+.. code:: python
+
+    >>> from math import sqrt
+    >>> from basicco.data_class import DataClass, field
+    >>> class Vector(DataClass):
+    ...     x = field()  # type: float
+    ...     y = field()  # type: float
+    ...     @property
+    ...     @field
+    ...     def mag(self):
+    ...         return sqrt(self.x**2 + self.y**2)
+    ...
+    >>> Vector(3.0, 4.0)
+    Vector(3.0, 4.0, mag=5.0)
+
 default_dir
 ^^^^^^^^^^^
 Backport of Python 3's implementation of
 `object.__dir__ <https://docs.python.org/3/reference/datamodel.html#object.__dir__>`_ for Python 2.7.
 
 This allows for calling `super().__dir__()` from a subclass to leverage the default implementation.
 
@@ -238,14 +230,29 @@
     ...     def __dir__(self):
     ...         return super(Class, self).__dir__()
     ...
     >>> obj = Class()
     >>> dir(obj)
     [...]
 
+dynamic_class
+^^^^^^^^^^^^^
+Easily generate classes on the fly. This works best with a `Base`_ class.
+If provided a valid qualified name and module (uses `caller_module`_ by default), the class will be pickable/importable.
+
+.. code:: python
+
+    >>> from basicco import Base
+    >>> from basicco.dynamic_class import make_cls
+    >>> class MyClass(object):
+    ...     DynClass = make_cls("MyClass.DynClass", bases=(Base,), dct={"foo": "bar"})
+    ...
+    >>> repr(MyClass.DynClass)
+    "<class '__main__.MyClass.DynClass'>"
+
 dynamic_code
 ^^^^^^^^^^^^
 Generate debuggable code on the fly that supports line numbers on tracebacks.
 
 .. code:: python
 
     >>> from basicco.dynamic_code import make_function, generate_unique_filename
@@ -389,23 +396,23 @@
     >>> class Bar(Foo):
     ...     __kwargs__ = {"foo": "bar"}  # you can specify cls kwargs on py2 like this
     ...
     >>> Bar.foo
     'bar'
 
 locked_class
-^^^^^^^^^^^^^
+^^^^^^^^^^^^
 Prevents changing public class attributes.
 
 .. code:: python
 
     >>> from six import with_metaclass
     >>> from basicco.locked_class import LockedClassMeta
     >>> class Foo(with_metaclass(LockedClassMeta, object)):
-    ...     pass
+    ...     bar = "foo"
     ...
     >>> Foo.bar = "bar"
     Traceback (most recent call last):
     AttributeError: can't set read-only class attribute 'bar'
 
 mangling
 ^^^^^^^^
@@ -419,15 +426,15 @@
     >>> unmangle("_Foo__member", "Foo")
     '__member'
     >>> extract("_Foo__member")
     ('__member', 'Foo')
 
 mapping_proxy
 ^^^^^^^^^^^^^
-Mapping Proxy type (read-only) for older Python versions.
+Mapping Proxy type (read-only dictionary) for older Python versions.
 
 .. code:: python
 
     >>> from basicco.mapping_proxy import MappingProxyType
     >>> internal_dict = {"foo": "bar"}
     >>> proxy_dict = MappingProxyType(internal_dict)
     >>> proxy_dict["foo"]
@@ -638,15 +645,15 @@
 
 type_checking
 ^^^^^^^^^^^^^
 Runtime type checking with support for import paths and type hints.
 
 .. code:: python
 
-    >>> from tippo import Mapping
+    >>> from tippo import Mapping, Literal
     >>> from itertools import chain
     >>> from basicco.type_checking import is_instance
     >>> class SubChain(chain):
     ...     pass
     ...
     >>> is_instance(3, int)
     True
@@ -658,14 +665,16 @@
     True
     >>> is_instance(chain(), "itertools.chain", subtypes=False)
     True
     >>> is_instance(SubChain(), "itertools.chain", subtypes=False)
     False
     >>> is_instance({"a": 1, "b": 2}, Mapping[str, int])
     True
+    >>> is_instance("PRE", Literal["PRE", "POST"])
+    True
 
 unique_iterator
 ^^^^^^^^^^^^^^^
 Iterator that yields unique values.
 
 .. code:: python
```

### Comparing `basicco-8.9.0/basicco.egg-info/SOURCES.txt` & `basicco-9.0.0/basicco.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -10,19 +10,20 @@
 .github/workflows/lint.yml
 .github/workflows/mypy.yml
 .github/workflows/pypi.yml
 .github/workflows/tests.yml
 basicco/__init__.py
 basicco/_bases.py
 basicco/abstract_class.py
-basicco/basic_data.py
 basicco/caller_module.py
 basicco/context_vars.py
 basicco/custom_repr.py
+basicco/data_class.py
 basicco/default_dir.py
+basicco/dynamic_class.py
 basicco/dynamic_code.py
 basicco/explicit_hash.py
 basicco/fabricate_value.py
 basicco/get_mro.py
 basicco/hash_cache_wrapper.py
 basicco/implicit_hash.py
 basicco/import_path.py
@@ -49,19 +50,20 @@
 basicco.egg-info/requires.txt
 basicco.egg-info/top_level.txt
 docs/source/conf.py
 docs/source/index.rst
 docs/source/_static/basicco.svg
 docs/source/_static/basicco_white.svg
 docs/source/api/basicco.abstract_class.rst
-docs/source/api/basicco.basic_data.rst
 docs/source/api/basicco.caller_module.rst
 docs/source/api/basicco.context_vars.rst
 docs/source/api/basicco.custom_repr.rst
+docs/source/api/basicco.data_class.rst
 docs/source/api/basicco.default_dir.rst
+docs/source/api/basicco.dynamic_class.rst
 docs/source/api/basicco.dynamic_code.rst
 docs/source/api/basicco.explicit_hash.rst
 docs/source/api/basicco.fabricate_value.rst
 docs/source/api/basicco.get_mro.rst
 docs/source/api/basicco.hash_cache_wrapper.rst
 docs/source/api/basicco.implicit_hash.rst
 docs/source/api/basicco.import_path.rst
@@ -80,19 +82,20 @@
 docs/source/api/basicco.safe_repr.rst
 docs/source/api/basicco.set_name.rst
 docs/source/api/basicco.type_checking.rst
 docs/source/api/basicco.unique_iterator.rst
 docs/source/api/basicco.weak_reference.rst
 tests/test_abstract_class.py
 tests/test_bases.py
-tests/test_basic_data.py
 tests/test_caller_module.py
 tests/test_context_vars.py
 tests/test_custom_repr.py
+tests/test_data_class.py
 tests/test_default_dir.py
+tests/test_dynamic_class.py
 tests/test_dynamic_code.py
 tests/test_explicit_hash.py
 tests/test_fabricate_value.py
 tests/test_get_mro.py
 tests/test_hash_cache_wrapper.py
 tests/test_import_path.py
 tests/test_init_subclass.py
```

### Comparing `basicco-8.9.0/docs/source/_static/basicco.svg` & `basicco-9.0.0/docs/source/_static/basicco.svg`

 * *Files identical despite different names*

### Comparing `basicco-8.9.0/docs/source/_static/basicco_white.svg` & `basicco-9.0.0/docs/source/_static/basicco_white.svg`

 * *Files identical despite different names*

### Comparing `basicco-8.9.0/docs/source/api/basicco.rst` & `basicco-9.0.0/docs/source/api/basicco.rst`

 * *Files 20% similar despite different names*

```diff
@@ -9,19 +9,20 @@
 Submodules
 ----------
 
 .. toctree::
    :maxdepth: 4
 
    basicco.abstract_class
-   basicco.basic_data
    basicco.caller_module
    basicco.context_vars
    basicco.custom_repr
+   basicco.data_class
    basicco.default_dir
+   basicco.dynamic_class
    basicco.dynamic_code
    basicco.explicit_hash
    basicco.fabricate_value
    basicco.get_mro
    basicco.hash_cache_wrapper
    basicco.implicit_hash
    basicco.import_path
```

### Comparing `basicco-8.9.0/docs/source/conf.py` & `basicco-9.0.0/docs/source/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     "sphinx.ext.autodoc",
     "sphinx_rtd_theme",
 ]
 
 # Intersphinx configuration.
 intersphinx_mapping = {
     "pyrsistent": ("https://pyrsistent.readthedocs.io/en/stable/", None),
-    "python": ("https://docs.python.org/3.10", None),
+    "python": ("https://docs.python.org/3.11", None),
     "six": ("https://six.readthedocs.io/", None),
     "slotted": ("https://slotted.readthedocs.io/en/stable/", None),
     "sphinx": ("https://www.sphinx-doc.org/en/master/", None),
     "tippo": ("https://tippo.readthedocs.io/en/stable/", None),
 }
 
 # Autodoc configuration.
```

### Comparing `basicco-8.9.0/setup.py` & `basicco-9.0.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,18 +20,18 @@
 
 with open("requirements.txt", "r") as fh:
     install_requires = [line.strip(os.linesep) for line in fh.readlines()]
 
 
 setuptools.setup(
     name="basicco",
-    version="8.9.0",
+    version="9.0.0",
     author="Bruno Nicko",
     author_email="brunonicko@gmail.com",
-    description="Collection of lower-level utilities that enhance code compatibility and validation.",
+    description="Base classes and utilities that enhance code compatibility, features and validation.",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/brunonicko/basicco",
     packages=setuptools.find_packages(exclude=["tests", "tests.*"]),
     package_data={"basicco": ["py.typed"]},
     install_requires=install_requires,
     classifiers=[
@@ -39,12 +39,13 @@
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 2.7",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: Implementation :: PyPy",
     ],
     python_requires=">= 2.7, != 3.0.*, != 3.1.*, != 3.2.*, != 3.3.*, != 3.4.*, != 3.5.*, != 3.6.*",
     tests_require=["pytest"],
 )
```

### Comparing `basicco-8.9.0/tests/test_abstract_class.py` & `basicco-9.0.0/tests/test_abstract_class.py`

 * *Files identical despite different names*

### Comparing `basicco-8.9.0/tests/test_bases.py` & `basicco-9.0.0/tests/test_bases.py`

 * *Files identical despite different names*

### Comparing `basicco-8.9.0/tests/test_context_vars.py` & `basicco-9.0.0/tests/test_context_vars.py`

 * *Files identical despite different names*

### Comparing `basicco-8.9.0/tests/test_custom_repr.py` & `basicco-9.0.0/tests/test_custom_repr.py`

 * *Files identical despite different names*

### Comparing `basicco-8.9.0/tests/test_default_dir.py` & `basicco-9.0.0/tests/test_default_dir.py`

 * *Files identical despite different names*

### Comparing `basicco-8.9.0/tests/test_dynamic_code.py` & `basicco-9.0.0/tests/test_dynamic_code.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 import pytest  # noqa
+from tippo import Any
 
-from basicco.dynamic_code import (
-    compile_and_eval,
-    generate_unique_filename,
-    make_function,
-)
+from basicco.dynamic_code import compile_and_eval, generate_unique_filename, make_function
 
 
 def test_generate_unique_filename():
     assert generate_unique_filename("my_func") == "<generated my_func>"
     assert generate_unique_filename("my_func", "module") == "<generated module.my_func>"
     assert generate_unique_filename("my_method", "module", "Class") == "<generated module.Class.my_method>"
 
 
 def test_compile_and_eval():
-    globs = {}
+    globs = {}  # type: dict[str, Any]
     compile_and_eval("foo = 40", globs)
     compile_and_eval("bar = 2", globs)
     compile_and_eval("foobar = foo + bar", globs)
     assert globs["foo"] == 40
     assert globs["bar"] == 2
     assert globs["foobar"] == 42
```

### Comparing `basicco-8.9.0/tests/test_explicit_hash.py` & `basicco-9.0.0/tests/test_explicit_hash.py`

 * *Files identical despite different names*

### Comparing `basicco-8.9.0/tests/test_fabricate_value.py` & `basicco-9.0.0/tests/test_fabricate_value.py`

 * *Files identical despite different names*

### Comparing `basicco-8.9.0/tests/test_get_mro.py` & `basicco-9.0.0/tests/test_get_mro.py`

 * *Files identical despite different names*

### Comparing `basicco-8.9.0/tests/test_hash_cache_wrapper.py` & `basicco-9.0.0/tests/test_hash_cache_wrapper.py`

 * *Files identical despite different names*

### Comparing `basicco-8.9.0/tests/test_import_path.py` & `basicco-9.0.0/tests/test_import_path.py`

 * *Files identical despite different names*

### Comparing `basicco-8.9.0/tests/test_init_subclass.py` & `basicco-9.0.0/tests/test_init_subclass.py`

 * *Files identical despite different names*

### Comparing `basicco-8.9.0/tests/test_locked_class.py` & `basicco-9.0.0/tests/test_locked_class.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,11 @@
 import pytest  # noqa
 import six
 
-from basicco.locked_class import (
-    LockedClass,
-    LockedClassMeta,
-    is_locked,
-    set_locked,
-    unlocked_context,
-)
+from basicco.locked_class import LockedClass, LockedClassMeta, is_locked, set_locked, unlocked_context
 
 
 def test_class():
     assert isinstance(LockedClass, LockedClassMeta)
 
 
 def test_metaclass():
```

### Comparing `basicco-8.9.0/tests/test_mangling.py` & `basicco-9.0.0/tests/test_mangling.py`

 * *Files identical despite different names*

### Comparing `basicco-8.9.0/tests/test_mapping_proxy.py` & `basicco-9.0.0/tests/test_mapping_proxy.py`

 * *Files identical despite different names*

### Comparing `basicco-8.9.0/tests/test_named_tuple.py` & `basicco-9.0.0/tests/test_named_tuple.py`

 * *Files identical despite different names*

### Comparing `basicco-8.9.0/tests/test_namespace.py` & `basicco-9.0.0/tests/test_namespace.py`

 * *Files identical despite different names*

### Comparing `basicco-8.9.0/tests/test_obj_state.py` & `basicco-9.0.0/tests/test_obj_state.py`

 * *Files identical despite different names*

### Comparing `basicco-8.9.0/tests/test_qualname.py` & `basicco-9.0.0/tests/test_qualname.py`

 * *Files identical despite different names*

### Comparing `basicco-8.9.0/tests/test_runtime_final.py` & `basicco-9.0.0/tests/test_runtime_final.py`

 * *Files identical despite different names*

### Comparing `basicco-8.9.0/tests/test_set_name.py` & `basicco-9.0.0/tests/test_set_name.py`

 * *Files identical despite different names*

### Comparing `basicco-8.9.0/tests/test_type_checking.py` & `basicco-9.0.0/tests/test_type_checking.py`

 * *Files identical despite different names*

### Comparing `basicco-8.9.0/tests/test_weak_reference.py` & `basicco-9.0.0/tests/test_weak_reference.py`

 * *Files identical despite different names*

