# Comparing `tmp/teapy-0.1.8.tar.gz` & `tmp/teapy-0.1.9.tar.gz`

## Comparing `teapy-0.1.8.tar` & `teapy-0.1.9.tar`

### file list

```diff
@@ -1,90 +1,90 @@
--rw-r--r--   0        0        0     1504 1970-01-01 00:00:00.000000 teapy-0.1.8/Cargo.toml
--rw-r--r--   0     1001      123      540 2023-07-10 03:37:09.000000 teapy-0.1.8/.cargo/config.toml
--rw-r--r--   0     1001      123      763 2023-07-10 03:37:09.000000 teapy-0.1.8/.github/workflows/build.yaml
--rw-r--r--   0     1001      123      975 2023-07-10 03:37:09.000000 teapy-0.1.8/.github/workflows/coverage.yaml
--rw-r--r--   0     1001      123     3561 2023-07-10 03:37:09.000000 teapy-0.1.8/.github/workflows/release_python.yaml
--rw-r--r--   0     1001      123     1303 2023-07-10 03:37:09.000000 teapy-0.1.8/.github/workflows/test_python.yaml
--rw-r--r--   0     1001      123      105 2023-07-10 03:37:09.000000 teapy-0.1.8/.gitignore
--rw-r--r--   0     1001      123       59 2023-07-10 03:37:09.000000 teapy-0.1.8/.vscode/settings.json
--rw-r--r--   0     1001      123     1049 2023-07-10 03:37:09.000000 teapy-0.1.8/LICENSE
--rw-r--r--   0     1001      123     1290 2023-07-10 03:37:09.000000 teapy-0.1.8/Makefile
--rw-r--r--   0     1001      123      520 2023-07-10 03:37:09.000000 teapy-0.1.8/README.md
--rw-r--r--   0     1001      123      214 2023-07-10 03:37:09.000000 teapy-0.1.8/build.requirements.txt
--rw-r--r--   0     1001      123      444 2023-07-10 03:37:09.000000 teapy-0.1.8/pyproject.toml
--rw-r--r--   0     1001      123       99 2023-07-10 03:37:09.000000 teapy-0.1.8/rust-toolchain.toml
--rw-r--r--   0     1001      123    14724 2023-07-10 03:37:09.000000 teapy-0.1.8/src/arr/agg.rs
--rw-r--r--   0     1001      123    33304 2023-07-10 03:37:09.000000 teapy-0.1.8/src/arr/arr_func.rs
--rw-r--r--   0     1001      123     4672 2023-07-10 03:37:09.000000 teapy-0.1.8/src/arr/corr.rs
--rw-r--r--   0     1001      123     8797 2023-07-10 03:37:09.000000 teapy-0.1.8/src/arr/datatype.rs
--rw-r--r--   0     1001      123      535 2023-07-10 03:37:09.000000 teapy-0.1.8/src/arr/export.rs
--rw-r--r--   0     1001      123     9128 2023-07-10 03:37:09.000000 teapy-0.1.8/src/arr/groupby.rs
--rw-r--r--   0     1001      123    15524 2023-07-10 03:37:09.000000 teapy-0.1.8/src/arr/impls/impl_1d_method.rs
--rw-r--r--   0     1001      123    10412 2023-07-10 03:37:09.000000 teapy-0.1.8/src/arr/impls/impl_method.rs
--rw-r--r--   0     1001      123     6606 2023-07-10 03:37:09.000000 teapy-0.1.8/src/arr/impls/impl_numeric.rs
--rw-r--r--   0     1001      123     4100 2023-07-10 03:37:09.000000 teapy-0.1.8/src/arr/impls/impl_traits.rs
--rw-r--r--   0     1001      123      432 2023-07-10 03:37:09.000000 teapy-0.1.8/src/arr/impls/linalg/generate.rs
--rw-r--r--   0     1001      123     7225 2023-07-10 03:37:09.000000 teapy-0.1.8/src/arr/impls/linalg/layout.rs
--rw-r--r--   0     1001      123     7509 2023-07-10 03:37:09.000000 teapy-0.1.8/src/arr/impls/linalg/least_squares.rs
--rw-r--r--   0     1001      123      236 2023-07-10 03:37:09.000000 teapy-0.1.8/src/arr/impls/linalg/mod.rs
--rw-r--r--   0     1001      123     5198 2023-07-10 03:37:09.000000 teapy-0.1.8/src/arr/impls/linalg/svd.rs
--rw-r--r--   0     1001      123      448 2023-07-10 03:37:09.000000 teapy-0.1.8/src/arr/impls/linalg/utils.rs
--rw-r--r--   0     1001      123      218 2023-07-10 03:37:09.000000 teapy-0.1.8/src/arr/impls/mod.rs
--rw-r--r--   0     1001      123    10337 2023-07-10 03:37:09.000000 teapy-0.1.8/src/arr/iterators.rs
--rw-r--r--   0     1001      123     2860 2023-07-10 03:37:09.000000 teapy-0.1.8/src/arr/join.rs
--rw-r--r--   0     1001      123     5002 2023-07-10 03:37:09.000000 teapy-0.1.8/src/arr/lazy/auto_impl_own.rs
--rw-r--r--   0     1001      123     3345 2023-07-10 03:37:09.000000 teapy-0.1.8/src/arr/lazy/expr_view.rs
--rw-r--r--   0     1001      123    14269 2023-07-10 03:37:09.000000 teapy-0.1.8/src/arr/lazy/exprs.rs
--rw-r--r--   0     1001      123     1885 2023-07-10 03:37:09.000000 teapy-0.1.8/src/arr/lazy/impl_cmp.rs
--rw-r--r--   0     1001      123      348 2023-07-10 03:37:09.000000 teapy-0.1.8/src/arr/lazy/impl_mut.rs
--rw-r--r--   0     1001      123     2916 2023-07-10 03:37:09.000000 teapy-0.1.8/src/arr/lazy/impl_ops.rs
--rw-r--r--   0     1001      123    30781 2023-07-10 03:37:09.000000 teapy-0.1.8/src/arr/lazy/impl_own.rs
--rw-r--r--   0     1001      123    11534 2023-07-10 03:37:09.000000 teapy-0.1.8/src/arr/lazy/impl_view.rs
--rw-r--r--   0     1001      123     8596 2023-07-10 03:37:09.000000 teapy-0.1.8/src/arr/lazy/linalg.rs
--rw-r--r--   0     1001      123    41747 2023-07-10 03:37:09.000000 teapy-0.1.8/src/arr/lazy/mod.rs
--rw-r--r--   0     1001      123    11591 2023-07-10 03:37:09.000000 teapy-0.1.8/src/arr/macros.rs
--rw-r--r--   0     1001      123    23495 2023-07-10 03:37:09.000000 teapy-0.1.8/src/arr/mod.rs
--rw-r--r--   0     1001      123      451 2023-07-10 03:37:09.000000 teapy-0.1.8/src/arr/option_datetype.rs
--rw-r--r--   0     1001      123    11274 2023-07-10 03:37:09.000000 teapy-0.1.8/src/arr/time.rs
--rw-r--r--   0     1001      123     1618 2023-07-10 03:37:09.000000 teapy-0.1.8/src/arr/util_trait.rs
--rw-r--r--   0     1001      123     3680 2023-07-10 03:37:09.000000 teapy-0.1.8/src/arr/utils/algos.rs
--rw-r--r--   0     1001      123     1746 2023-07-10 03:37:09.000000 teapy-0.1.8/src/arr/utils/alloc.rs
--rw-r--r--   0     1001      123      195 2023-07-10 03:37:09.000000 teapy-0.1.8/src/arr/utils/default_new.rs
--rw-r--r--   0     1001      123      185 2023-07-10 03:37:09.000000 teapy-0.1.8/src/arr/utils/mod.rs
--rw-r--r--   0     1001      123    13376 2023-07-10 03:37:09.000000 teapy-0.1.8/src/arr/window/compare.rs
--rw-r--r--   0     1001      123     6390 2023-07-10 03:37:09.000000 teapy-0.1.8/src/arr/window/corr.rs
--rw-r--r--   0     1001      123    24023 2023-07-10 03:37:09.000000 teapy-0.1.8/src/arr/window/feature.rs
--rw-r--r--   0     1001      123       75 2023-07-10 03:37:09.000000 teapy-0.1.8/src/arr/window/mod.rs
--rw-r--r--   0     1001      123     9226 2023-07-10 03:37:09.000000 teapy-0.1.8/src/arr/window/norm.rs
--rw-r--r--   0     1001      123    12965 2023-07-10 03:37:09.000000 teapy-0.1.8/src/arr/window/reg.rs
--rw-r--r--   0     1001      123    14796 2023-07-10 03:37:09.000000 teapy-0.1.8/src/equity.rs
--rw-r--r--   0     1001      123     7988 2023-07-10 03:37:09.000000 teapy-0.1.8/src/from_py.rs
--rw-r--r--   0     1001      123     1261 2023-07-10 03:37:09.000000 teapy-0.1.8/src/lib.rs
--rw-r--r--   0     1001      123    41221 2023-07-10 03:37:09.000000 teapy-0.1.8/src/pylazy/datadict.rs
--rw-r--r--   0     1001      123      530 2023-07-10 03:37:09.000000 teapy-0.1.8/src/pylazy/export.rs
--rw-r--r--   0     1001      123     2606 2023-07-10 03:37:09.000000 teapy-0.1.8/src/pylazy/groupby.rs
--rw-r--r--   0     1001      123    87845 2023-07-10 03:37:09.000000 teapy-0.1.8/src/pylazy/impl_pyexpr.rs
--rw-r--r--   0     1001      123     1277 2023-07-10 03:37:09.000000 teapy-0.1.8/src/pylazy/mod.rs
--rw-r--r--   0     1001      123    20439 2023-07-10 03:37:09.000000 teapy-0.1.8/src/pylazy/pyexpr.rs
--rw-r--r--   0     1001      123    16559 2023-07-10 03:37:09.000000 teapy-0.1.8/src/pylazy/pyfunc.rs
--rw-r--r--   0     1001      123      454 2023-07-10 03:37:09.000000 teapy-0.1.8/src/pylazy/time.rs
--rw-r--r--   0     1001      123      414 2023-07-10 03:37:09.000000 teapy-0.1.8/teapy/__init__.py
--rw-r--r--   0     1001      123     4513 2023-07-10 03:37:09.000000 teapy-0.1.8/teapy/array_func.py
--rw-r--r--   0     1001      123     3184 2023-07-10 03:37:09.000000 teapy-0.1.8/teapy/converter.py
--rw-r--r--   0     1001      123     6341 2023-07-10 03:37:09.000000 teapy-0.1.8/teapy/datadict.py
--rw-r--r--   0     1001      123     9221 2023-07-10 03:37:09.000000 teapy-0.1.8/teapy/regression.py
--rw-r--r--   0     1001      123     3440 2023-07-10 03:37:09.000000 teapy-0.1.8/teapy/testing.py
--rw-r--r--   0     1001      123    10814 2023-07-10 03:37:09.000000 teapy-0.1.8/teapy/tests/test_array_func.py
--rw-r--r--   0     1001      123     3406 2023-07-10 03:37:09.000000 teapy-0.1.8/teapy/tests/test_common.py
--rw-r--r--   0     1001      123     4291 2023-07-10 03:37:09.000000 teapy-0.1.8/teapy/tests/test_datadict.py
--rw-r--r--   0     1001      123     2240 2023-07-10 03:37:09.000000 teapy-0.1.8/teapy/tests/test_equity.py
--rw-r--r--   0     1001      123      747 2023-07-10 03:37:09.000000 teapy-0.1.8/teapy/tests/test_expr.py
--rw-r--r--   0     1001      123      245 2023-07-10 03:37:09.000000 teapy-0.1.8/teapy/tests/test_memory.py
--rw-r--r--   0     1001      123     3211 2023-07-10 03:37:09.000000 teapy-0.1.8/teapy/tests/window/test_compare.py
--rw-r--r--   0     1001      123     1418 2023-07-10 03:37:09.000000 teapy-0.1.8/teapy/tests/window/test_corr.py
--rw-r--r--   0     1001      123     5772 2023-07-10 03:37:09.000000 teapy-0.1.8/teapy/tests/window/test_feature.py
--rw-r--r--   0     1001      123     1995 2023-07-10 03:37:09.000000 teapy-0.1.8/teapy/tests/window/test_norm.py
--rw-r--r--   0     1001      123     3165 2023-07-10 03:37:09.000000 teapy-0.1.8/teapy/tests/window/test_reg.py
--rw-r--r--   0     1001      123     3695 2023-07-10 03:37:09.000000 teapy-0.1.8/teapy/window_func.py
--rw-r--r--   0     1001      123     1272 2023-07-10 03:37:09.000000 teapy-0.1.8/teapy/wrapper.py
--rw-r--r--   0     1001      123    54100 2023-07-10 03:37:09.000000 teapy-0.1.8/Cargo.lock
--rw-r--r--   0        0        0      945 1970-01-01 00:00:00.000000 teapy-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1517 1970-01-01 00:00:00.000000 teapy-0.1.9/Cargo.toml
+-rw-r--r--   0     1001      123      540 2023-07-10 10:51:29.000000 teapy-0.1.9/.cargo/config.toml
+-rw-r--r--   0     1001      123      763 2023-07-10 10:51:29.000000 teapy-0.1.9/.github/workflows/build.yaml
+-rw-r--r--   0     1001      123      975 2023-07-10 10:51:29.000000 teapy-0.1.9/.github/workflows/coverage.yaml
+-rw-r--r--   0     1001      123     3561 2023-07-10 10:51:29.000000 teapy-0.1.9/.github/workflows/release_python.yaml
+-rw-r--r--   0     1001      123     1303 2023-07-10 10:51:29.000000 teapy-0.1.9/.github/workflows/test_python.yaml
+-rw-r--r--   0     1001      123      105 2023-07-10 10:51:29.000000 teapy-0.1.9/.gitignore
+-rw-r--r--   0     1001      123       59 2023-07-10 10:51:29.000000 teapy-0.1.9/.vscode/settings.json
+-rw-r--r--   0     1001      123     1049 2023-07-10 10:51:29.000000 teapy-0.1.9/LICENSE
+-rw-r--r--   0     1001      123     1290 2023-07-10 10:51:29.000000 teapy-0.1.9/Makefile
+-rw-r--r--   0     1001      123      520 2023-07-10 10:51:29.000000 teapy-0.1.9/README.md
+-rw-r--r--   0     1001      123      214 2023-07-10 10:51:29.000000 teapy-0.1.9/build.requirements.txt
+-rw-r--r--   0     1001      123      444 2023-07-10 10:51:29.000000 teapy-0.1.9/pyproject.toml
+-rw-r--r--   0     1001      123       99 2023-07-10 10:51:29.000000 teapy-0.1.9/rust-toolchain.toml
+-rw-r--r--   0     1001      123    14724 2023-07-10 10:51:29.000000 teapy-0.1.9/src/arr/agg.rs
+-rw-r--r--   0     1001      123    33304 2023-07-10 10:51:29.000000 teapy-0.1.9/src/arr/arr_func.rs
+-rw-r--r--   0     1001      123     4672 2023-07-10 10:51:29.000000 teapy-0.1.9/src/arr/corr.rs
+-rw-r--r--   0     1001      123     8797 2023-07-10 10:51:29.000000 teapy-0.1.9/src/arr/datatype.rs
+-rw-r--r--   0     1001      123      535 2023-07-10 10:51:29.000000 teapy-0.1.9/src/arr/export.rs
+-rw-r--r--   0     1001      123     9128 2023-07-10 10:51:29.000000 teapy-0.1.9/src/arr/groupby.rs
+-rw-r--r--   0     1001      123    15524 2023-07-10 10:51:29.000000 teapy-0.1.9/src/arr/impls/impl_1d_method.rs
+-rw-r--r--   0     1001      123    10412 2023-07-10 10:51:29.000000 teapy-0.1.9/src/arr/impls/impl_method.rs
+-rw-r--r--   0     1001      123     6606 2023-07-10 10:51:29.000000 teapy-0.1.9/src/arr/impls/impl_numeric.rs
+-rw-r--r--   0     1001      123     4100 2023-07-10 10:51:29.000000 teapy-0.1.9/src/arr/impls/impl_traits.rs
+-rw-r--r--   0     1001      123      432 2023-07-10 10:51:29.000000 teapy-0.1.9/src/arr/impls/linalg/generate.rs
+-rw-r--r--   0     1001      123     7225 2023-07-10 10:51:29.000000 teapy-0.1.9/src/arr/impls/linalg/layout.rs
+-rw-r--r--   0     1001      123     7509 2023-07-10 10:51:29.000000 teapy-0.1.9/src/arr/impls/linalg/least_squares.rs
+-rw-r--r--   0     1001      123      236 2023-07-10 10:51:29.000000 teapy-0.1.9/src/arr/impls/linalg/mod.rs
+-rw-r--r--   0     1001      123     5232 2023-07-10 10:51:29.000000 teapy-0.1.9/src/arr/impls/linalg/svd.rs
+-rw-r--r--   0     1001      123      448 2023-07-10 10:51:29.000000 teapy-0.1.9/src/arr/impls/linalg/utils.rs
+-rw-r--r--   0     1001      123      218 2023-07-10 10:51:29.000000 teapy-0.1.9/src/arr/impls/mod.rs
+-rw-r--r--   0     1001      123    10337 2023-07-10 10:51:29.000000 teapy-0.1.9/src/arr/iterators.rs
+-rw-r--r--   0     1001      123     2860 2023-07-10 10:51:29.000000 teapy-0.1.9/src/arr/join.rs
+-rw-r--r--   0     1001      123     5002 2023-07-10 10:51:29.000000 teapy-0.1.9/src/arr/lazy/auto_impl_own.rs
+-rw-r--r--   0     1001      123     3345 2023-07-10 10:51:29.000000 teapy-0.1.9/src/arr/lazy/expr_view.rs
+-rw-r--r--   0     1001      123    14269 2023-07-10 10:51:29.000000 teapy-0.1.9/src/arr/lazy/exprs.rs
+-rw-r--r--   0     1001      123     1885 2023-07-10 10:51:29.000000 teapy-0.1.9/src/arr/lazy/impl_cmp.rs
+-rw-r--r--   0     1001      123      348 2023-07-10 10:51:29.000000 teapy-0.1.9/src/arr/lazy/impl_mut.rs
+-rw-r--r--   0     1001      123     2916 2023-07-10 10:51:29.000000 teapy-0.1.9/src/arr/lazy/impl_ops.rs
+-rw-r--r--   0     1001      123    30781 2023-07-10 10:51:29.000000 teapy-0.1.9/src/arr/lazy/impl_own.rs
+-rw-r--r--   0     1001      123    11534 2023-07-10 10:51:29.000000 teapy-0.1.9/src/arr/lazy/impl_view.rs
+-rw-r--r--   0     1001      123     8596 2023-07-10 10:51:29.000000 teapy-0.1.9/src/arr/lazy/linalg.rs
+-rw-r--r--   0     1001      123    43625 2023-07-10 10:51:29.000000 teapy-0.1.9/src/arr/lazy/mod.rs
+-rw-r--r--   0     1001      123    11591 2023-07-10 10:51:29.000000 teapy-0.1.9/src/arr/macros.rs
+-rw-r--r--   0     1001      123    23495 2023-07-10 10:51:29.000000 teapy-0.1.9/src/arr/mod.rs
+-rw-r--r--   0     1001      123      451 2023-07-10 10:51:29.000000 teapy-0.1.9/src/arr/option_datetype.rs
+-rw-r--r--   0     1001      123    11274 2023-07-10 10:51:29.000000 teapy-0.1.9/src/arr/time.rs
+-rw-r--r--   0     1001      123     1618 2023-07-10 10:51:29.000000 teapy-0.1.9/src/arr/util_trait.rs
+-rw-r--r--   0     1001      123     3680 2023-07-10 10:51:29.000000 teapy-0.1.9/src/arr/utils/algos.rs
+-rw-r--r--   0     1001      123     1746 2023-07-10 10:51:29.000000 teapy-0.1.9/src/arr/utils/alloc.rs
+-rw-r--r--   0     1001      123      195 2023-07-10 10:51:29.000000 teapy-0.1.9/src/arr/utils/default_new.rs
+-rw-r--r--   0     1001      123      185 2023-07-10 10:51:29.000000 teapy-0.1.9/src/arr/utils/mod.rs
+-rw-r--r--   0     1001      123    13376 2023-07-10 10:51:29.000000 teapy-0.1.9/src/arr/window/compare.rs
+-rw-r--r--   0     1001      123     6390 2023-07-10 10:51:29.000000 teapy-0.1.9/src/arr/window/corr.rs
+-rw-r--r--   0     1001      123    24023 2023-07-10 10:51:29.000000 teapy-0.1.9/src/arr/window/feature.rs
+-rw-r--r--   0     1001      123       75 2023-07-10 10:51:29.000000 teapy-0.1.9/src/arr/window/mod.rs
+-rw-r--r--   0     1001      123     9226 2023-07-10 10:51:29.000000 teapy-0.1.9/src/arr/window/norm.rs
+-rw-r--r--   0     1001      123    12965 2023-07-10 10:51:29.000000 teapy-0.1.9/src/arr/window/reg.rs
+-rw-r--r--   0     1001      123    14796 2023-07-10 10:51:29.000000 teapy-0.1.9/src/equity.rs
+-rw-r--r--   0     1001      123     7988 2023-07-10 10:51:29.000000 teapy-0.1.9/src/from_py.rs
+-rw-r--r--   0     1001      123     1261 2023-07-10 10:51:29.000000 teapy-0.1.9/src/lib.rs
+-rw-r--r--   0     1001      123    41221 2023-07-10 10:51:29.000000 teapy-0.1.9/src/pylazy/datadict.rs
+-rw-r--r--   0     1001      123      530 2023-07-10 10:51:29.000000 teapy-0.1.9/src/pylazy/export.rs
+-rw-r--r--   0     1001      123     2606 2023-07-10 10:51:29.000000 teapy-0.1.9/src/pylazy/groupby.rs
+-rw-r--r--   0     1001      123    88019 2023-07-10 10:51:29.000000 teapy-0.1.9/src/pylazy/impl_pyexpr.rs
+-rw-r--r--   0     1001      123     1277 2023-07-10 10:51:29.000000 teapy-0.1.9/src/pylazy/mod.rs
+-rw-r--r--   0     1001      123    20439 2023-07-10 10:51:29.000000 teapy-0.1.9/src/pylazy/pyexpr.rs
+-rw-r--r--   0     1001      123    16559 2023-07-10 10:51:29.000000 teapy-0.1.9/src/pylazy/pyfunc.rs
+-rw-r--r--   0     1001      123      454 2023-07-10 10:51:29.000000 teapy-0.1.9/src/pylazy/time.rs
+-rw-r--r--   0     1001      123      414 2023-07-10 10:51:29.000000 teapy-0.1.9/teapy/__init__.py
+-rw-r--r--   0     1001      123     4513 2023-07-10 10:51:29.000000 teapy-0.1.9/teapy/array_func.py
+-rw-r--r--   0     1001      123     3184 2023-07-10 10:51:29.000000 teapy-0.1.9/teapy/converter.py
+-rw-r--r--   0     1001      123     6341 2023-07-10 10:51:29.000000 teapy-0.1.9/teapy/datadict.py
+-rw-r--r--   0     1001      123     9221 2023-07-10 10:51:29.000000 teapy-0.1.9/teapy/regression.py
+-rw-r--r--   0     1001      123     3440 2023-07-10 10:51:29.000000 teapy-0.1.9/teapy/testing.py
+-rw-r--r--   0     1001      123    10814 2023-07-10 10:51:29.000000 teapy-0.1.9/teapy/tests/test_array_func.py
+-rw-r--r--   0     1001      123     3406 2023-07-10 10:51:29.000000 teapy-0.1.9/teapy/tests/test_common.py
+-rw-r--r--   0     1001      123     4291 2023-07-10 10:51:29.000000 teapy-0.1.9/teapy/tests/test_datadict.py
+-rw-r--r--   0     1001      123     2240 2023-07-10 10:51:29.000000 teapy-0.1.9/teapy/tests/test_equity.py
+-rw-r--r--   0     1001      123      871 2023-07-10 10:51:29.000000 teapy-0.1.9/teapy/tests/test_expr.py
+-rw-r--r--   0     1001      123      245 2023-07-10 10:51:29.000000 teapy-0.1.9/teapy/tests/test_memory.py
+-rw-r--r--   0     1001      123     3211 2023-07-10 10:51:29.000000 teapy-0.1.9/teapy/tests/window/test_compare.py
+-rw-r--r--   0     1001      123     1418 2023-07-10 10:51:29.000000 teapy-0.1.9/teapy/tests/window/test_corr.py
+-rw-r--r--   0     1001      123     5772 2023-07-10 10:51:29.000000 teapy-0.1.9/teapy/tests/window/test_feature.py
+-rw-r--r--   0     1001      123     1995 2023-07-10 10:51:29.000000 teapy-0.1.9/teapy/tests/window/test_norm.py
+-rw-r--r--   0     1001      123     3165 2023-07-10 10:51:29.000000 teapy-0.1.9/teapy/tests/window/test_reg.py
+-rw-r--r--   0     1001      123     3695 2023-07-10 10:51:29.000000 teapy-0.1.9/teapy/window_func.py
+-rw-r--r--   0     1001      123     1272 2023-07-10 10:51:29.000000 teapy-0.1.9/teapy/wrapper.py
+-rw-r--r--   0     1001      123    54109 2023-07-10 10:51:29.000000 teapy-0.1.9/Cargo.lock
+-rw-r--r--   0        0        0      945 1970-01-01 00:00:00.000000 teapy-0.1.9/PKG-INFO
```

### Comparing `teapy-0.1.8/Cargo.toml` & `teapy-0.1.9/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "teapy"
-version = "0.1.8"
+version = "0.1.9"
 edition = "2021"
 
 [lib]
 name = "teapy"
 crate-type = ["cdylib", "rlib"]
 
 [features]
@@ -30,14 +30,15 @@
 lto = true
 
 
 [dependencies]
 pyo3 = {version = "0.19.0", features = ["extension-module", "abi3-py38", "macros", "serde"]}
 numpy = "0.19"
 num = "0.4"
+libc = "0.2"
 
 rayon = "1.5"
 ahash = "0.8.2"
 regex = "1"
 chrono = {version = "0.4.23", features = ["serde"]}
 serde = { version = "1.0", features = ["derive"] }
 serde_with = {version = "3.0", features = ["chrono"]}
```

### Comparing `teapy-0.1.8/.cargo/config.toml` & `teapy-0.1.9/.cargo/config.toml`

 * *Files identical despite different names*

### Comparing `teapy-0.1.8/.github/workflows/build.yaml` & `teapy-0.1.9/.github/workflows/build.yaml`

 * *Files identical despite different names*

### Comparing `teapy-0.1.8/.github/workflows/coverage.yaml` & `teapy-0.1.9/.github/workflows/coverage.yaml`

 * *Files identical despite different names*

### Comparing `teapy-0.1.8/.github/workflows/release_python.yaml` & `teapy-0.1.9/.github/workflows/release_python.yaml`

 * *Files identical despite different names*

### Comparing `teapy-0.1.8/.github/workflows/test_python.yaml` & `teapy-0.1.9/.github/workflows/test_python.yaml`

 * *Files identical despite different names*

### Comparing `teapy-0.1.8/LICENSE` & `teapy-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `teapy-0.1.8/Makefile` & `teapy-0.1.9/Makefile`

 * *Files identical despite different names*

### Comparing `teapy-0.1.8/README.md` & `teapy-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `teapy-0.1.8/src/arr/agg.rs` & `teapy-0.1.9/src/arr/agg.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.8/src/arr/arr_func.rs` & `teapy-0.1.9/src/arr/arr_func.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.8/src/arr/corr.rs` & `teapy-0.1.9/src/arr/corr.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.8/src/arr/datatype.rs` & `teapy-0.1.9/src/arr/datatype.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.8/src/arr/export.rs` & `teapy-0.1.9/src/arr/export.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.8/src/arr/groupby.rs` & `teapy-0.1.9/src/arr/groupby.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.8/src/arr/impls/impl_1d_method.rs` & `teapy-0.1.9/src/arr/impls/impl_1d_method.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.8/src/arr/impls/impl_method.rs` & `teapy-0.1.9/src/arr/impls/impl_method.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.8/src/arr/impls/impl_numeric.rs` & `teapy-0.1.9/src/arr/impls/impl_numeric.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.8/src/arr/impls/impl_traits.rs` & `teapy-0.1.9/src/arr/impls/impl_traits.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.8/src/arr/impls/linalg/layout.rs` & `teapy-0.1.9/src/arr/impls/linalg/layout.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.8/src/arr/impls/linalg/least_squares.rs` & `teapy-0.1.9/src/arr/impls/linalg/least_squares.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.8/src/arr/impls/linalg/svd.rs` & `teapy-0.1.9/src/arr/impls/linalg/svd.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 use super::super::super::{
     utils::{vec_uninit, VecAssumeInit},
     Arr1, ArrD,
 };
 use super::{into_matrix, MatrixLayout};
 use lapack_sys::dgesvd_;
+use libc::c_char;
 
 impl ArrD<f64> {
     pub fn svd_into(self, full: bool, calc_uvt: bool) -> (Option<Self>, Self, Option<Self>) {
         let mut arr = self.to_dim2().expect("Array should be dim2 when svd");
         let layout = arr.layout().expect("Array should be contiguous when svd");
         let mut_arr = arr
             .as_slice_memory_order_mut()
@@ -47,16 +48,16 @@
         };
         let mut s = vec_uninit::<f64>(k as usize);
         // eval work size
         let mut info = 0;
         let mut work_size = [0.];
         unsafe {
             dgesvd_(
-                &jobu as *const u8 as *const i8,
-                &jobvt as *const u8 as *const i8,
+                &jobu as *const u8 as *const c_char,
+                &jobvt as *const u8 as *const c_char,
                 &m,
                 &n,
                 std::ptr::null_mut(),       // A
                 &m,                         // lda
                 s.as_mut_ptr() as *mut f64, // S
                 u.as_mut()
                     .map(|x| x.as_mut_ptr())
@@ -75,16 +76,16 @@
             panic!("SVD error: info = {info}");
         }
         let lwork = work_size[0] as i32;
         let mut work = vec_uninit::<f64>(lwork.try_into().unwrap());
         info = 0;
         unsafe {
             dgesvd_(
-                &jobu as *const u8 as *const i8,
-                &jobvt as *const u8 as *const i8,
+                &jobu as *const u8 as *const c_char,
+                &jobvt as *const u8 as *const c_char,
                 &m,
                 &n,
                 mut_arr.as_mut_ptr(),
                 &m,                         // lda
                 s.as_mut_ptr() as *mut f64, // S
                 u.as_mut()
                     .map(|x| x.as_mut_ptr())
```

### Comparing `teapy-0.1.8/src/arr/iterators.rs` & `teapy-0.1.9/src/arr/iterators.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.8/src/arr/join.rs` & `teapy-0.1.9/src/arr/join.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.8/src/arr/lazy/auto_impl_own.rs` & `teapy-0.1.9/src/arr/lazy/auto_impl_own.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.8/src/arr/lazy/expr_view.rs` & `teapy-0.1.9/src/arr/lazy/expr_view.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.8/src/arr/lazy/exprs.rs` & `teapy-0.1.9/src/arr/lazy/exprs.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.8/src/arr/lazy/impl_cmp.rs` & `teapy-0.1.9/src/arr/lazy/impl_cmp.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.8/src/arr/lazy/impl_ops.rs` & `teapy-0.1.9/src/arr/lazy/impl_ops.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.8/src/arr/lazy/impl_own.rs` & `teapy-0.1.9/src/arr/lazy/impl_own.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.8/src/arr/lazy/impl_view.rs` & `teapy-0.1.9/src/arr/lazy/impl_view.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.8/src/arr/lazy/linalg.rs` & `teapy-0.1.9/src/arr/lazy/linalg.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.8/src/arr/lazy/mod.rs` & `teapy-0.1.9/src/arr/lazy/mod.rs`

 * *Files 4% similar despite different names*

```diff
@@ -562,15 +562,15 @@
                                 let mut exprs_lock = exprs.lock().unwrap();
                                 // if exprs_lock.step() != 0 {
                                 exprs_lock.eval_inplace();
                                 // }
                                 // we should not modify the base expression
                                 // safety: the data of the base expression must exist
                                 if ref_count > 1 {
-                                    // panic!("ref_count = {} > 1", ref_count);
+                                    // dbg!("ref_count = {} > 1", ref_count);
                                     let out: ExprOut<'_, T> = exprs_lock.view::<T>().unwrap().into();
                                     return mem::transmute(out)
                                 } else {
                                     mem::drop(exprs_lock);
                                     Expr {e:exprs, _type: PhantomData}.into_out()
                                 }
                             },
@@ -920,24 +920,30 @@
     pub fn update_ref_expr(&mut self) {
         if let ExprBase::Expr(base_expr) = &mut self.base {
             base_expr.lock().unwrap().eval_inplace();
             if let Some(is_owned) = self.owned {
                 if !is_owned {
                     self.ref_expr = Some(vec![base_expr.clone()])
                 }
+                // else if is_owned {
+                //     self.ref_expr = Some(vec![base_expr.clone()])
+                // }
             }
         }
     }
 
     /// Execute the expression inplace
     #[inline]
     pub fn eval_inplace(&mut self) {
         if self.step() != 0 {
             let default_func: FuncChainType<'a, T> = DefaultNew::default_new();
             let func = mem::replace(&mut self.func, default_func);
+            // if let ExprBase::Expr(base_expr) = &mut self.base {
+            //     base_expr.lock().unwrap().eval_inplace();
+            // }
             self.update_ref_expr();
             let base = mem::take(&mut self.base);
             let out = func(base);
             self.set_owned(out.is_owned());
             if self.get_owned().unwrap() {
                 self.ref_expr = None;
             }
@@ -1050,76 +1056,110 @@
         self.into_out().into_arr()
     }
 
     #[inline]
     pub fn into_out(self) -> ExprOut<'a, T> {
         (self.func)(self.base)
     }
+
+    // pub fn add_depend_expr(&mut self, expr: Arc<Mutex<ExprsInner<'a>>>) {
+    //     if matches!(ref_type, RefType::True) {
+    //         // self.ref_expr = Some(vec![base_expr.clone()])
+    //         if let Some(mut ref_expr) = self.ref_expr {
+    //             ref_expr.push(base_expr);
+    //             self.ref_expr = Some(ref_expr);
+    //         } else {
+    //             self.ref_expr = Some(vec![base_expr]);
+    //         }
+    //     }
+    // }
+
     /// chain a new function to current function chain, the function accept
     /// an array of type `ExprOut<'a, T>` and return `ExprOut<'a, T>`
     pub fn chain_f<F, T2>(mut self, f: F, ref_type: RefType) -> ExprInner<'a, T2>
     where
         F: FnOnce(ExprOut<'a, T>) -> ExprOut<'a, T2> + Send + Sync + 'a,
         T2: ExprElement,
     {
-        ExprInner::<'a, T2> {
-            base: self.base,
-            step: self.step + 1,
-            name: self.name.clone(),
-            owned: self.owned,
-            func: Box::new(move |base: ExprBase<'a>| {
-                let expr_out = (self.func)(base);
-                match expr_out {
-                    ExprOut::Arr(arb_array) => {
-                        let last_out = if arb_array.is_owned() {
-                            match ref_type {
-                                RefType::True => {
-                                    let base_expr: ExprsInner =
-                                        ExprInner::<T>::new_with_arr(arb_array, self.name).into();
-                                    let base_expr = Arc::new(Mutex::new(base_expr));
-                                    if let Some(mut ref_expr) = self.ref_expr {
-                                        ref_expr.push(base_expr);
-                                        self.ref_expr = Some(ref_expr);
-                                    } else {
-                                        self.ref_expr = Some(vec![base_expr]);
-                                    }
-                                    if let Some(ref_expr) = &self.ref_expr {
-                                        // this should always be true
-                                        let e = ref_expr.last().unwrap().lock().unwrap();
-                                        let arr_view = e.view::<T>().unwrap().into_arr();
-                                        let arr_view: ArrViewD<'a, T> =
-                                            unsafe { mem::transmute(arr_view) };
-                                        arr_view.into()
-                                    } else {
-                                        unreachable!()
-                                    }
-                                }
-                                _ => arb_array,
-                            }
-                        } else {
-                            arb_array
-                        };
-                        let out = f(ExprOut::Arr(last_out));
-                        if out.is_owned() {
-                            self.ref_expr = None;
-                        }
-                        out
-                    }
-                    _ => {
-                        let out = f(expr_out);
-                        if out.is_owned() {
-                            self.ref_expr = None;
-                        }
-                        out
-                    }
+        if let ExprBase::Expr(base_expr) = &self.base {
+            if matches!(ref_type, RefType::True) {
+                if let Some(mut ref_expr) = self.ref_expr {
+                    ref_expr.push(base_expr.clone());
+                    self.ref_expr = Some(ref_expr);
+                } else {
+                    self.ref_expr = Some(vec![base_expr.clone()]);
                 }
-                // f((self.func)(base).into_arr()).into()
-            }),
-            ref_expr: None,
+            } else {
+                self.ref_expr = None
+            }
         }
+        self.set_step(self.step + 1);
+        let default_func: FuncChainType<'a, T> = DefaultNew::default_new();
+        let ori_func = mem::replace(&mut self.func, default_func);
+        let mut out: ExprInner<'a, T2> = unsafe { mem::transmute(self) };
+        out.set_func(Box::new(|base: ExprBase<'a>| f(ori_func(base))));
+        out
+        // ExprInner::<'a, T2> {
+        //     base: self.base,
+        //     step: self.step + 1,
+        //     name: self.name.clone(),
+        //     owned: self.owned,
+        //     func: Box::new(move |base: ExprBase<'a>| {
+        //         // if matches!(base, ExprBase::Expr(_)) & matches!(ref_type, RefType::False) {
+        //         //     self.ref_expr = None
+        //         // }
+        //         let expr_out = (self.func)(base);
+        //         match expr_out {
+        //             ExprOut::Arr(arb_array) => {
+        //                 let last_out = if arb_array.is_owned() {
+        //                     match ref_type {
+        //                         RefType::True => {
+        //                             let base_expr: ExprsInner =
+        //                                 ExprInner::<T>::new_with_arr(arb_array, self.name).into();
+        //                             let base_expr = Arc::new(Mutex::new(base_expr));
+        //                             if let Some(mut ref_expr) = self.ref_expr {
+        //                                 ref_expr.push(base_expr);
+        //                                 self.ref_expr = Some(ref_expr);
+        //                             } else {
+        //                                 self.ref_expr = Some(vec![base_expr]);
+        //                             }
+        //                             if let Some(ref_expr) = &self.ref_expr {
+        //                                 // this should always be true
+        //                                 let e = ref_expr.last().unwrap().lock().unwrap();
+        //                                 let arr_view = e.view::<T>().unwrap().into_arr();
+        //                                 let arr_view: ArrViewD<'a, T> =
+        //                                     unsafe { mem::transmute(arr_view) };
+        //                                 arr_view.into()
+        //                             } else {
+        //                                 unreachable!()
+        //                             }
+        //                         }
+        //                         _ => arb_array,
+        //                     }
+        //                 } else {
+        //                     arb_array
+        //                 };
+        //                 let out = f(ExprOut::Arr(last_out));
+        //                 if out.is_owned() {
+        //                     self.ref_expr = None;
+        //                 }
+        //                 out
+        //             }
+        //             _ => {
+        //                 let out = f(expr_out);
+        //                 if out.is_owned() {
+        //                     self.ref_expr = None;
+        //                 }
+        //                 out
+        //             }
+        //         }
+        //         // f((self.func)(base).into_arr()).into()
+        //     }),
+        //     ref_expr: None,
+        // }
     }
 
     /// chain a new function to current function chain, the function accept
     /// an array of type `ArbArray<'a, T>` and return `ArbArray<'a, T>`
     pub fn chain_arr_f<F, T2>(self, f: F, ref_type: RefType) -> ExprInner<'a, T2>
     where
         F: FnOnce(ArbArray<'a, T>) -> ArbArray<'a, T2> + Send + Sync + 'a,
```

### Comparing `teapy-0.1.8/src/arr/macros.rs` & `teapy-0.1.9/src/arr/macros.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.8/src/arr/mod.rs` & `teapy-0.1.9/src/arr/mod.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.8/src/arr/time.rs` & `teapy-0.1.9/src/arr/time.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.8/src/arr/util_trait.rs` & `teapy-0.1.9/src/arr/util_trait.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.8/src/arr/utils/algos.rs` & `teapy-0.1.9/src/arr/utils/algos.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.8/src/arr/utils/alloc.rs` & `teapy-0.1.9/src/arr/utils/alloc.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.8/src/arr/window/compare.rs` & `teapy-0.1.9/src/arr/window/compare.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.8/src/arr/window/corr.rs` & `teapy-0.1.9/src/arr/window/corr.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.8/src/arr/window/feature.rs` & `teapy-0.1.9/src/arr/window/feature.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.8/src/arr/window/norm.rs` & `teapy-0.1.9/src/arr/window/norm.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.8/src/arr/window/reg.rs` & `teapy-0.1.9/src/arr/window/reg.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.8/src/equity.rs` & `teapy-0.1.9/src/equity.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.8/src/from_py.rs` & `teapy-0.1.9/src/from_py.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.8/src/lib.rs` & `teapy-0.1.9/src/lib.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.8/src/pylazy/datadict.rs` & `teapy-0.1.9/src/pylazy/datadict.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.8/src/pylazy/export.rs` & `teapy-0.1.9/src/pylazy/export.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.8/src/pylazy/groupby.rs` & `teapy-0.1.9/src/pylazy/groupby.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.8/src/pylazy/impl_pyexpr.rs` & `teapy-0.1.9/src/pylazy/impl_pyexpr.rs`

 * *Files 2% similar despite different names*

```diff
@@ -320,17 +320,23 @@
             Object
         )
     }
 
     #[getter]
     #[allow(unreachable_patterns)]
     pub fn step(&self) -> usize {
-        match_exprs!(&self.inner, expr, { expr.step() })
+        match_exprs!(&self.inner, expr, { expr.step_acc() })
     }
 
+    // #[getter]
+    // #[allow(unreachable_patterns)]
+    // pub fn step_acc(&self) -> usize {
+    //     match_exprs!(&self.inner, expr, { expr.step_acc() })
+    // }
+
     #[getter]
     #[allow(unreachable_patterns)]
     pub fn get_name(&self) -> Option<String> {
         match_exprs!(&self.inner, expr, { expr.name() })
     }
 
     #[setter]
```

### Comparing `teapy-0.1.8/src/pylazy/mod.rs` & `teapy-0.1.9/src/pylazy/mod.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.8/src/pylazy/pyexpr.rs` & `teapy-0.1.9/src/pylazy/pyexpr.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.8/src/pylazy/pyfunc.rs` & `teapy-0.1.9/src/pylazy/pyfunc.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.8/teapy/array_func.py` & `teapy-0.1.9/teapy/array_func.py`

 * *Files identical despite different names*

### Comparing `teapy-0.1.8/teapy/converter.py` & `teapy-0.1.9/teapy/converter.py`

 * *Files identical despite different names*

### Comparing `teapy-0.1.8/teapy/datadict.py` & `teapy-0.1.9/teapy/datadict.py`

 * *Files identical despite different names*

### Comparing `teapy-0.1.8/teapy/regression.py` & `teapy-0.1.9/teapy/regression.py`

 * *Files identical despite different names*

### Comparing `teapy-0.1.8/teapy/testing.py` & `teapy-0.1.9/teapy/testing.py`

 * *Files identical despite different names*

### Comparing `teapy-0.1.8/teapy/tests/test_array_func.py` & `teapy-0.1.9/teapy/tests/test_array_func.py`

 * *Files identical despite different names*

### Comparing `teapy-0.1.8/teapy/tests/test_common.py` & `teapy-0.1.9/teapy/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `teapy-0.1.8/teapy/tests/test_datadict.py` & `teapy-0.1.9/teapy/tests/test_datadict.py`

 * *Files identical despite different names*

### Comparing `teapy-0.1.8/teapy/tests/test_equity.py` & `teapy-0.1.9/teapy/tests/test_equity.py`

 * *Files identical despite different names*

### Comparing `teapy-0.1.8/teapy/tests/test_expr.py` & `teapy-0.1.9/teapy/tests/test_expr.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,20 +2,22 @@
 
 import teapy as tp
 from teapy.testing import assert_allclose
 
 
 def test_slice():
     a = np.random.randn(100, 39)
-    e = tp.Expr(a)
+    e = tp.Expr(a, copy=False)
     assert_allclose(e[:10, :].eview(), a[:10, :])
     assert_allclose(e[-4:9, :].eview(), a[-4:9, :])
     assert_allclose(e[:, -2:-4].eview(), a[:, -2:-4])
     assert_allclose(e[None, :, :].eview(), a[None, :, :])
     assert_allclose(e[[-3, -5], 3:9].eview(), a[[-3, -5], 3:9])
+    e = tp.Expr(a, copy=True)
+    assert_allclose(e.argsort(axis=1)[:, :10].eview(), a.argsort(axis=1)[:, :10])
     # # currentyly the logic is not the same
     # assert_allclose(e[[-3, -5], [3, -2]].eview(), a[[-3, -5], [3, -2]])
 
     a = np.array([1, 2, 3, 4, 5, 6, 7, 8])
     e = tp.Expr(a)
     assert e[-1].eview() == 8
     assert e[-3].eview() == 6
```

### Comparing `teapy-0.1.8/teapy/tests/window/test_compare.py` & `teapy-0.1.9/teapy/tests/window/test_compare.py`

 * *Files identical despite different names*

### Comparing `teapy-0.1.8/teapy/tests/window/test_corr.py` & `teapy-0.1.9/teapy/tests/window/test_corr.py`

 * *Files identical despite different names*

### Comparing `teapy-0.1.8/teapy/tests/window/test_feature.py` & `teapy-0.1.9/teapy/tests/window/test_feature.py`

 * *Files identical despite different names*

### Comparing `teapy-0.1.8/teapy/tests/window/test_norm.py` & `teapy-0.1.9/teapy/tests/window/test_norm.py`

 * *Files identical despite different names*

### Comparing `teapy-0.1.8/teapy/tests/window/test_reg.py` & `teapy-0.1.9/teapy/tests/window/test_reg.py`

 * *Files identical despite different names*

### Comparing `teapy-0.1.8/teapy/window_func.py` & `teapy-0.1.9/teapy/window_func.py`

 * *Files identical despite different names*

### Comparing `teapy-0.1.8/teapy/wrapper.py` & `teapy-0.1.9/teapy/wrapper.py`

 * *Files identical despite different names*

### Comparing `teapy-0.1.8/Cargo.lock` & `teapy-0.1.9/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1632,20 +1632,21 @@
 name = "target-lexicon"
 version = "0.12.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fd1ba337640d60c3e96bc6f0638a939b9c9a7f2c316a1598c279828b3d1dc8c5"
 
 [[package]]
 name = "teapy"
-version = "0.1.8"
+version = "0.1.9"
 dependencies = [
  "ahash",
  "chrono",
  "intel-mkl-src",
  "lapack-sys",
+ "libc",
  "ndarray",
  "ndarray-npy",
  "num",
  "numpy",
  "openblas-src",
  "pyo3",
  "rayon",
```

### Comparing `teapy-0.1.8/PKG-INFO` & `teapy-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: teapy
-Version: 0.1.8
+Version: 0.1.9
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Dist: numpy >=1.16.0
 License-File: LICENSE
 Summary: A blazingly fast datadict library
 Author-email: Teamon <teamon9161@163.com>
```

