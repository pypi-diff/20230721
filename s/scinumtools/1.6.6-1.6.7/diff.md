# Comparing `tmp/scinumtools-1.6.6.tar.gz` & `tmp/scinumtools-1.6.7.tar.gz`

## Comparing `scinumtools-1.6.6.tar` & `scinumtools-1.6.7.tar`

### file list

```diff
@@ -1,89 +1,89 @@
--rwxr-xr-x   0        0        0      188 2020-02-02 00:00:00.000000 scinumtools-1.6.6/build_doc.sh
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 scinumtools-1.6.6/requirements.txt
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 scinumtools-1.6.6/.github/workflows/pytest.yml
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 scinumtools-1.6.6/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 scinumtools-1.6.6/.github/workflows/static.yml
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 scinumtools-1.6.6/docs/Makefile
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 scinumtools-1.6.6/docs/make.bat
--rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 scinumtools-1.6.6/docs/source/conf.py
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 scinumtools-1.6.6/docs/source/data.rst
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 scinumtools-1.6.6/docs/source/index.rst
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 scinumtools-1.6.6/docs/source/introduction.rst
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 scinumtools-1.6.6/docs/source/math.rst
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 scinumtools-1.6.6/docs/source/phys.rst
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 scinumtools-1.6.6/docs/source/stats.rst
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 scinumtools-1.6.6/docs/source/structs.rst
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 scinumtools-1.6.6/docs/source/api/modules.rst
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 scinumtools-1.6.6/docs/source/api/scinumtools.data.rst
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 scinumtools-1.6.6/docs/source/api/scinumtools.math.rst
--rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 scinumtools-1.6.6/docs/source/api/scinumtools.math.solver.rst
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 scinumtools-1.6.6/docs/source/api/scinumtools.phys.rst
--rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 scinumtools-1.6.6/docs/source/api/scinumtools.phys.units.rst
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 scinumtools-1.6.6/docs/source/api/scinumtools.rst
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 scinumtools-1.6.6/docs/source/api/scinumtools.stats.rst
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 scinumtools-1.6.6/docs/source/api/scinumtools.structs.rst
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 scinumtools-1.6.6/src/scinumtools/__init__.py
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 scinumtools-1.6.6/src/scinumtools/data/CachingClass.py
--rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 scinumtools-1.6.6/src/scinumtools/data/ImageClass.py
--rw-r--r--   0        0        0     6086 2020-02-02 00:00:00.000000 scinumtools-1.6.6/src/scinumtools/data/PlottingClass.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 scinumtools-1.6.6/src/scinumtools/data/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scinumtools-1.6.6/src/scinumtools/math/__init__.py
--rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 scinumtools-1.6.6/src/scinumtools/math/solver/AtomClass.py
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 scinumtools-1.6.6/src/scinumtools/math/solver/ExpressionClass.py
--rw-r--r--   0        0        0     7525 2020-02-02 00:00:00.000000 scinumtools-1.6.6/src/scinumtools/math/solver/OperatorClass.py
--rw-r--r--   0        0        0     3803 2020-02-02 00:00:00.000000 scinumtools-1.6.6/src/scinumtools/math/solver/SolverClass.py
--rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 scinumtools-1.6.6/src/scinumtools/math/solver/TokensClass.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 scinumtools-1.6.6/src/scinumtools/math/solver/__init__.py
--rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 scinumtools-1.6.6/src/scinumtools/phys/ConstantsClass.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 scinumtools-1.6.6/src/scinumtools/phys/__init__.py
--rw-r--r--   0        0        0     2547 2020-02-02 00:00:00.000000 scinumtools-1.6.6/src/scinumtools/phys/units/BaseUnitsClass.py
--rw-r--r--   0        0        0     3332 2020-02-02 00:00:00.000000 scinumtools-1.6.6/src/scinumtools/phys/units/DimensionsClass.py
--rw-r--r--   0        0        0     3403 2020-02-02 00:00:00.000000 scinumtools-1.6.6/src/scinumtools/phys/units/FractionClass.py
--rw-r--r--   0        0        0    13259 2020-02-02 00:00:00.000000 scinumtools-1.6.6/src/scinumtools/phys/units/QuantityClass.py
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 scinumtools-1.6.6/src/scinumtools/phys/units/UnitClass.py
--rw-r--r--   0        0        0     2538 2020-02-02 00:00:00.000000 scinumtools-1.6.6/src/scinumtools/phys/units/UnitConverters.py
--rw-r--r--   0        0        0    10710 2020-02-02 00:00:00.000000 scinumtools-1.6.6/src/scinumtools/phys/units/UnitList.py
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 scinumtools-1.6.6/src/scinumtools/phys/units/__init__.py
--rw-r--r--   0        0        0     2606 2020-02-02 00:00:00.000000 scinumtools-1.6.6/src/scinumtools/stats/StopwatchClass.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 scinumtools-1.6.6/src/scinumtools/stats/__init__.py
--rw-r--r--   0        0        0     5509 2020-02-02 00:00:00.000000 scinumtools-1.6.6/src/scinumtools/structs/CollectorClass.py
--rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 scinumtools-1.6.6/src/scinumtools/structs/ParameterClass.py
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 scinumtools-1.6.6/src/scinumtools/structs/ProgressBar.py
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 scinumtools-1.6.6/src/scinumtools/structs/__init__.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 scinumtools-1.6.6/tests/README.md
--rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 scinumtools-1.6.6/tests/cached_data.npy
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 scinumtools-1.6.6/tests/pyproject.toml
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 scinumtools-1.6.6/tests/requirements.txt
--rw-r--r--   0        0        0     6537 2020-02-02 00:00:00.000000 scinumtools-1.6.6/tests/test_data.py
--rw-r--r--   0        0        0     4225 2020-02-02 00:00:00.000000 scinumtools-1.6.6/tests/test_math.py
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 scinumtools-1.6.6/tests/test_physics.py
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 scinumtools-1.6.6/tests/test_stats.py
--rw-r--r--   0        0        0     4184 2020-02-02 00:00:00.000000 scinumtools-1.6.6/tests/test_struct.py
--rw-r--r--   0        0        0    12551 2020-02-02 00:00:00.000000 scinumtools-1.6.6/tests/test_units.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 scinumtools-1.6.6/tests/src/scinumtools/__init__.py
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 scinumtools-1.6.6/tests/src/scinumtools/data/CachingClass.py
--rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 scinumtools-1.6.6/tests/src/scinumtools/data/ImageClass.py
--rw-r--r--   0        0        0     4741 2020-02-02 00:00:00.000000 scinumtools-1.6.6/tests/src/scinumtools/data/PlottingClass.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 scinumtools-1.6.6/tests/src/scinumtools/data/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scinumtools-1.6.6/tests/src/scinumtools/math/__init__.py
--rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 scinumtools-1.6.6/tests/src/scinumtools/math/solver/AtomClass.py
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 scinumtools-1.6.6/tests/src/scinumtools/math/solver/ExpressionClass.py
--rw-r--r--   0        0        0     7525 2020-02-02 00:00:00.000000 scinumtools-1.6.6/tests/src/scinumtools/math/solver/OperatorClass.py
--rw-r--r--   0        0        0     3803 2020-02-02 00:00:00.000000 scinumtools-1.6.6/tests/src/scinumtools/math/solver/SolverClass.py
--rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 scinumtools-1.6.6/tests/src/scinumtools/math/solver/TokensClass.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 scinumtools-1.6.6/tests/src/scinumtools/math/solver/__init__.py
--rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 scinumtools-1.6.6/tests/src/scinumtools/phys/ConstantsClass.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 scinumtools-1.6.6/tests/src/scinumtools/phys/__init__.py
--rw-r--r--   0        0        0     9181 2020-02-02 00:00:00.000000 scinumtools-1.6.6/tests/src/scinumtools/phys/units/QuantityClass.py
--rw-r--r--   0        0        0     2153 2020-02-02 00:00:00.000000 scinumtools-1.6.6/tests/src/scinumtools/phys/units/UnitConverters.py
--rw-r--r--   0        0        0    10140 2020-02-02 00:00:00.000000 scinumtools-1.6.6/tests/src/scinumtools/phys/units/UnitList.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 scinumtools-1.6.6/tests/src/scinumtools/phys/units/__init__.py
--rw-r--r--   0        0        0     2606 2020-02-02 00:00:00.000000 scinumtools-1.6.6/tests/src/scinumtools/stats/StopwatchClass.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 scinumtools-1.6.6/tests/src/scinumtools/stats/__init__.py
--rw-r--r--   0        0        0     5397 2020-02-02 00:00:00.000000 scinumtools-1.6.6/tests/src/scinumtools/structs/CollectorClass.py
--rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 scinumtools-1.6.6/tests/src/scinumtools/structs/ParameterClass.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 scinumtools-1.6.6/tests/src/scinumtools/structs/__init__.py
--rw-r--r--   0        0        0     3081 2020-02-02 00:00:00.000000 scinumtools-1.6.6/.gitignore
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 scinumtools-1.6.6/README.md
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 scinumtools-1.6.6/pyproject.toml
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 scinumtools-1.6.6/PKG-INFO
+-rwxr-xr-x   0        0        0      188 2020-02-02 00:00:00.000000 scinumtools-1.6.7/build_doc.sh
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 scinumtools-1.6.7/requirements.txt
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 scinumtools-1.6.7/.github/workflows/pytest.yml
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 scinumtools-1.6.7/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 scinumtools-1.6.7/.github/workflows/static.yml
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 scinumtools-1.6.7/docs/Makefile
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 scinumtools-1.6.7/docs/make.bat
+-rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 scinumtools-1.6.7/docs/source/conf.py
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 scinumtools-1.6.7/docs/source/data.rst
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 scinumtools-1.6.7/docs/source/index.rst
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 scinumtools-1.6.7/docs/source/introduction.rst
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 scinumtools-1.6.7/docs/source/math.rst
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 scinumtools-1.6.7/docs/source/phys.rst
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 scinumtools-1.6.7/docs/source/stats.rst
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 scinumtools-1.6.7/docs/source/structs.rst
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 scinumtools-1.6.7/docs/source/api/modules.rst
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 scinumtools-1.6.7/docs/source/api/scinumtools.data.rst
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 scinumtools-1.6.7/docs/source/api/scinumtools.math.rst
+-rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 scinumtools-1.6.7/docs/source/api/scinumtools.math.solver.rst
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 scinumtools-1.6.7/docs/source/api/scinumtools.phys.rst
+-rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 scinumtools-1.6.7/docs/source/api/scinumtools.phys.units.rst
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 scinumtools-1.6.7/docs/source/api/scinumtools.rst
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 scinumtools-1.6.7/docs/source/api/scinumtools.stats.rst
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 scinumtools-1.6.7/docs/source/api/scinumtools.structs.rst
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 scinumtools-1.6.7/src/scinumtools/__init__.py
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 scinumtools-1.6.7/src/scinumtools/data/CachingClass.py
+-rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 scinumtools-1.6.7/src/scinumtools/data/ImageClass.py
+-rw-r--r--   0        0        0     6086 2020-02-02 00:00:00.000000 scinumtools-1.6.7/src/scinumtools/data/PlottingClass.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 scinumtools-1.6.7/src/scinumtools/data/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scinumtools-1.6.7/src/scinumtools/math/__init__.py
+-rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 scinumtools-1.6.7/src/scinumtools/math/solver/AtomClass.py
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 scinumtools-1.6.7/src/scinumtools/math/solver/ExpressionClass.py
+-rw-r--r--   0        0        0     7525 2020-02-02 00:00:00.000000 scinumtools-1.6.7/src/scinumtools/math/solver/OperatorClass.py
+-rw-r--r--   0        0        0     3803 2020-02-02 00:00:00.000000 scinumtools-1.6.7/src/scinumtools/math/solver/SolverClass.py
+-rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 scinumtools-1.6.7/src/scinumtools/math/solver/TokensClass.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 scinumtools-1.6.7/src/scinumtools/math/solver/__init__.py
+-rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 scinumtools-1.6.7/src/scinumtools/phys/ConstantsClass.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 scinumtools-1.6.7/src/scinumtools/phys/__init__.py
+-rw-r--r--   0        0        0     2547 2020-02-02 00:00:00.000000 scinumtools-1.6.7/src/scinumtools/phys/units/BaseUnitsClass.py
+-rw-r--r--   0        0        0     3332 2020-02-02 00:00:00.000000 scinumtools-1.6.7/src/scinumtools/phys/units/DimensionsClass.py
+-rw-r--r--   0        0        0     3403 2020-02-02 00:00:00.000000 scinumtools-1.6.7/src/scinumtools/phys/units/FractionClass.py
+-rw-r--r--   0        0        0    13259 2020-02-02 00:00:00.000000 scinumtools-1.6.7/src/scinumtools/phys/units/QuantityClass.py
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 scinumtools-1.6.7/src/scinumtools/phys/units/UnitClass.py
+-rw-r--r--   0        0        0     2538 2020-02-02 00:00:00.000000 scinumtools-1.6.7/src/scinumtools/phys/units/UnitConverters.py
+-rw-r--r--   0        0        0    10710 2020-02-02 00:00:00.000000 scinumtools-1.6.7/src/scinumtools/phys/units/UnitList.py
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 scinumtools-1.6.7/src/scinumtools/phys/units/__init__.py
+-rw-r--r--   0        0        0     2606 2020-02-02 00:00:00.000000 scinumtools-1.6.7/src/scinumtools/stats/StopwatchClass.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 scinumtools-1.6.7/src/scinumtools/stats/__init__.py
+-rw-r--r--   0        0        0     5509 2020-02-02 00:00:00.000000 scinumtools-1.6.7/src/scinumtools/structs/CollectorClass.py
+-rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 scinumtools-1.6.7/src/scinumtools/structs/ParameterClass.py
+-rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 scinumtools-1.6.7/src/scinumtools/structs/ProgressBar.py
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 scinumtools-1.6.7/src/scinumtools/structs/__init__.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 scinumtools-1.6.7/tests/README.md
+-rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 scinumtools-1.6.7/tests/cached_data.npy
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 scinumtools-1.6.7/tests/pyproject.toml
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 scinumtools-1.6.7/tests/requirements.txt
+-rw-r--r--   0        0        0     6537 2020-02-02 00:00:00.000000 scinumtools-1.6.7/tests/test_data.py
+-rw-r--r--   0        0        0     4225 2020-02-02 00:00:00.000000 scinumtools-1.6.7/tests/test_math.py
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 scinumtools-1.6.7/tests/test_physics.py
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 scinumtools-1.6.7/tests/test_stats.py
+-rw-r--r--   0        0        0     4184 2020-02-02 00:00:00.000000 scinumtools-1.6.7/tests/test_struct.py
+-rw-r--r--   0        0        0    12551 2020-02-02 00:00:00.000000 scinumtools-1.6.7/tests/test_units.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 scinumtools-1.6.7/tests/src/scinumtools/__init__.py
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 scinumtools-1.6.7/tests/src/scinumtools/data/CachingClass.py
+-rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 scinumtools-1.6.7/tests/src/scinumtools/data/ImageClass.py
+-rw-r--r--   0        0        0     4741 2020-02-02 00:00:00.000000 scinumtools-1.6.7/tests/src/scinumtools/data/PlottingClass.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 scinumtools-1.6.7/tests/src/scinumtools/data/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scinumtools-1.6.7/tests/src/scinumtools/math/__init__.py
+-rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 scinumtools-1.6.7/tests/src/scinumtools/math/solver/AtomClass.py
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 scinumtools-1.6.7/tests/src/scinumtools/math/solver/ExpressionClass.py
+-rw-r--r--   0        0        0     7525 2020-02-02 00:00:00.000000 scinumtools-1.6.7/tests/src/scinumtools/math/solver/OperatorClass.py
+-rw-r--r--   0        0        0     3803 2020-02-02 00:00:00.000000 scinumtools-1.6.7/tests/src/scinumtools/math/solver/SolverClass.py
+-rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 scinumtools-1.6.7/tests/src/scinumtools/math/solver/TokensClass.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 scinumtools-1.6.7/tests/src/scinumtools/math/solver/__init__.py
+-rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 scinumtools-1.6.7/tests/src/scinumtools/phys/ConstantsClass.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 scinumtools-1.6.7/tests/src/scinumtools/phys/__init__.py
+-rw-r--r--   0        0        0     9181 2020-02-02 00:00:00.000000 scinumtools-1.6.7/tests/src/scinumtools/phys/units/QuantityClass.py
+-rw-r--r--   0        0        0     2153 2020-02-02 00:00:00.000000 scinumtools-1.6.7/tests/src/scinumtools/phys/units/UnitConverters.py
+-rw-r--r--   0        0        0    10140 2020-02-02 00:00:00.000000 scinumtools-1.6.7/tests/src/scinumtools/phys/units/UnitList.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 scinumtools-1.6.7/tests/src/scinumtools/phys/units/__init__.py
+-rw-r--r--   0        0        0     2606 2020-02-02 00:00:00.000000 scinumtools-1.6.7/tests/src/scinumtools/stats/StopwatchClass.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 scinumtools-1.6.7/tests/src/scinumtools/stats/__init__.py
+-rw-r--r--   0        0        0     5397 2020-02-02 00:00:00.000000 scinumtools-1.6.7/tests/src/scinumtools/structs/CollectorClass.py
+-rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 scinumtools-1.6.7/tests/src/scinumtools/structs/ParameterClass.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 scinumtools-1.6.7/tests/src/scinumtools/structs/__init__.py
+-rw-r--r--   0        0        0     3081 2020-02-02 00:00:00.000000 scinumtools-1.6.7/.gitignore
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 scinumtools-1.6.7/README.md
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 scinumtools-1.6.7/pyproject.toml
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 scinumtools-1.6.7/PKG-INFO
```

### Comparing `scinumtools-1.6.6/.github/workflows/python-publish.yml` & `scinumtools-1.6.7/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `scinumtools-1.6.6/.github/workflows/static.yml` & `scinumtools-1.6.7/.github/workflows/static.yml`

 * *Files identical despite different names*

### Comparing `scinumtools-1.6.6/docs/Makefile` & `scinumtools-1.6.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `scinumtools-1.6.6/docs/make.bat` & `scinumtools-1.6.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `scinumtools-1.6.6/docs/source/conf.py` & `scinumtools-1.6.7/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.6.6/docs/source/index.rst` & `scinumtools-1.6.7/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `scinumtools-1.6.6/docs/source/api/scinumtools.data.rst` & `scinumtools-1.6.7/docs/source/api/scinumtools.data.rst`

 * *Files identical despite different names*

### Comparing `scinumtools-1.6.6/docs/source/api/scinumtools.math.solver.rst` & `scinumtools-1.6.7/docs/source/api/scinumtools.math.solver.rst`

 * *Files identical despite different names*

### Comparing `scinumtools-1.6.6/docs/source/api/scinumtools.phys.units.rst` & `scinumtools-1.6.7/docs/source/api/scinumtools.phys.units.rst`

 * *Files identical despite different names*

### Comparing `scinumtools-1.6.6/docs/source/api/scinumtools.structs.rst` & `scinumtools-1.6.7/docs/source/api/scinumtools.structs.rst`

 * *Files identical despite different names*

### Comparing `scinumtools-1.6.6/src/scinumtools/data/CachingClass.py` & `scinumtools-1.6.7/src/scinumtools/data/CachingClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.6.6/src/scinumtools/data/ImageClass.py` & `scinumtools-1.6.7/src/scinumtools/data/ImageClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.6.6/src/scinumtools/data/PlottingClass.py` & `scinumtools-1.6.7/src/scinumtools/data/PlottingClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.6.6/src/scinumtools/math/solver/AtomClass.py` & `scinumtools-1.6.7/src/scinumtools/math/solver/AtomClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.6.6/src/scinumtools/math/solver/ExpressionClass.py` & `scinumtools-1.6.7/src/scinumtools/math/solver/ExpressionClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.6.6/src/scinumtools/math/solver/OperatorClass.py` & `scinumtools-1.6.7/src/scinumtools/math/solver/OperatorClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.6.6/src/scinumtools/math/solver/SolverClass.py` & `scinumtools-1.6.7/src/scinumtools/math/solver/SolverClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.6.6/src/scinumtools/math/solver/TokensClass.py` & `scinumtools-1.6.7/src/scinumtools/math/solver/TokensClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.6.6/src/scinumtools/phys/ConstantsClass.py` & `scinumtools-1.6.7/src/scinumtools/phys/ConstantsClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.6.6/src/scinumtools/phys/units/BaseUnitsClass.py` & `scinumtools-1.6.7/src/scinumtools/phys/units/BaseUnitsClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.6.6/src/scinumtools/phys/units/DimensionsClass.py` & `scinumtools-1.6.7/src/scinumtools/phys/units/DimensionsClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.6.6/src/scinumtools/phys/units/FractionClass.py` & `scinumtools-1.6.7/src/scinumtools/phys/units/FractionClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.6.6/src/scinumtools/phys/units/QuantityClass.py` & `scinumtools-1.6.7/src/scinumtools/phys/units/QuantityClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.6.6/src/scinumtools/phys/units/UnitClass.py` & `scinumtools-1.6.7/src/scinumtools/phys/units/UnitClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.6.6/src/scinumtools/phys/units/UnitConverters.py` & `scinumtools-1.6.7/src/scinumtools/phys/units/UnitConverters.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.6.6/src/scinumtools/phys/units/UnitList.py` & `scinumtools-1.6.7/src/scinumtools/phys/units/UnitList.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.6.6/src/scinumtools/stats/StopwatchClass.py` & `scinumtools-1.6.7/src/scinumtools/stats/StopwatchClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.6.6/src/scinumtools/structs/CollectorClass.py` & `scinumtools-1.6.7/src/scinumtools/structs/CollectorClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.6.6/src/scinumtools/structs/ParameterClass.py` & `scinumtools-1.6.7/src/scinumtools/structs/ParameterClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.6.6/tests/cached_data.npy` & `scinumtools-1.6.7/tests/cached_data.npy`

 * *Files identical despite different names*

### Comparing `scinumtools-1.6.6/tests/pyproject.toml` & `scinumtools-1.6.7/tests/pyproject.toml`

 * *Files identical despite different names*

### Comparing `scinumtools-1.6.6/tests/test_data.py` & `scinumtools-1.6.7/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.6.6/tests/test_math.py` & `scinumtools-1.6.7/tests/test_math.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.6.6/tests/test_stats.py` & `scinumtools-1.6.7/tests/test_stats.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.6.6/tests/test_struct.py` & `scinumtools-1.6.7/tests/test_struct.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.6.6/tests/test_units.py` & `scinumtools-1.6.7/tests/test_units.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.6.6/tests/src/scinumtools/data/ImageClass.py` & `scinumtools-1.6.7/tests/src/scinumtools/data/ImageClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.6.6/tests/src/scinumtools/data/PlottingClass.py` & `scinumtools-1.6.7/tests/src/scinumtools/data/PlottingClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.6.6/tests/src/scinumtools/math/solver/AtomClass.py` & `scinumtools-1.6.7/tests/src/scinumtools/math/solver/AtomClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.6.6/tests/src/scinumtools/math/solver/ExpressionClass.py` & `scinumtools-1.6.7/tests/src/scinumtools/math/solver/ExpressionClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.6.6/tests/src/scinumtools/math/solver/OperatorClass.py` & `scinumtools-1.6.7/tests/src/scinumtools/math/solver/OperatorClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.6.6/tests/src/scinumtools/math/solver/SolverClass.py` & `scinumtools-1.6.7/tests/src/scinumtools/math/solver/SolverClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.6.6/tests/src/scinumtools/math/solver/TokensClass.py` & `scinumtools-1.6.7/tests/src/scinumtools/math/solver/TokensClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.6.6/tests/src/scinumtools/phys/ConstantsClass.py` & `scinumtools-1.6.7/tests/src/scinumtools/phys/ConstantsClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.6.6/tests/src/scinumtools/phys/units/QuantityClass.py` & `scinumtools-1.6.7/tests/src/scinumtools/phys/units/QuantityClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.6.6/tests/src/scinumtools/phys/units/UnitConverters.py` & `scinumtools-1.6.7/tests/src/scinumtools/phys/units/UnitConverters.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.6.6/tests/src/scinumtools/phys/units/UnitList.py` & `scinumtools-1.6.7/tests/src/scinumtools/phys/units/UnitList.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.6.6/tests/src/scinumtools/stats/StopwatchClass.py` & `scinumtools-1.6.7/tests/src/scinumtools/stats/StopwatchClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.6.6/tests/src/scinumtools/structs/CollectorClass.py` & `scinumtools-1.6.7/tests/src/scinumtools/structs/CollectorClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.6.6/tests/src/scinumtools/structs/ParameterClass.py` & `scinumtools-1.6.7/tests/src/scinumtools/structs/ParameterClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.6.6/.gitignore` & `scinumtools-1.6.7/.gitignore`

 * *Files identical despite different names*

### Comparing `scinumtools-1.6.6/pyproject.toml` & `scinumtools-1.6.7/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "scinumtools"
-version = "1.6.6"
+version = "1.6.7"
 authors = [
   { name="Ondrej Pego Jaura", email="vrtulka23@pm.me" },
 ]
 description = "Set of most frequently used tools for a rapid numerical code development in Python."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `scinumtools-1.6.6/PKG-INFO` & `scinumtools-1.6.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scinumtools
-Version: 1.6.6
+Version: 1.6.7
 Summary: Set of most frequently used tools for a rapid numerical code development in Python.
 Project-URL: Homepage, https://github.com/vrtulka23/scinumtools
 Project-URL: Bug Tracker, https://github.com/vrtulka23/scinumtools/issues
 Author-email: Ondrej Pego Jaura <vrtulka23@pm.me>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

