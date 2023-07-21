# Comparing `tmp/pyqtorch-0.3.3.tar.gz` & `tmp/pyqtorch-0.4.0.tar.gz`

## Comparing `pyqtorch-0.3.3.tar` & `pyqtorch-0.4.0.tar`

### file list

```diff
@@ -1,60 +1,64 @@
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/CONTRIBUTING.md
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/README.md
--rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/mkdocs.yml
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/readthedocs.yml
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/setup.py
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/.github/workflows/run-tests-and-mypy.yml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/docs/CODE_OF_CONDUCT.md -> ../CODE_OF_CONDUCT.md
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/docs/CONTRIBUTING.md -> ../CONTRIBUTING.md
--rw-r--r--   0        0        0    57645 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/docs/QAOA.ipynb
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/docs/circuit.md
--rw-r--r--   0        0        0     6493 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/docs/essentials.ipynb
--rw-r--r--   0        0        0   154246 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/docs/fit_function.ipynb
--rw-r--r--   0        0        0     2854 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/docs/gate_composition.ipynb
--rw-r--r--   0        0        0     4634 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/docs/hamevo.md
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/docs/index.md
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/docs/matrices.md
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/docs/parametric.md
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/docs/primitive.md
--rw-r--r--   0        0        0    46162 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/docs/deprecated/QAOA.ipynb
--rw-r--r--   0        0        0    19339 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/docs/deprecated/bench.py
--rw-r--r--   0        0        0    74042 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/docs/deprecated/fit_function.ipynb
--rw-r--r--   0        0        0    74062 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/docs/deprecated/getting_started.ipynb
--rw-r--r--   0        0        0   121176 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/docs/deprecated/ham_evol_comparison.ipynb
--rw-r--r--   0        0        0     6459 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/docs/deprecated/state_evolution.ipynb
--rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/pyqtorch/__init__.py
--rw-r--r--   0        0        0     3544 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/pyqtorch/ansatz.py
--rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/pyqtorch/embedding.py
--rw-r--r--   0        0        0     4939 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/pyqtorch/matrices.py
--rw-r--r--   0        0        0     6255 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/pyqtorch/matrices_sparse.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/pyqtorch/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/pyqtorch/converters/__init__.py
--rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/pyqtorch/converters/store_ops.py
--rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/pyqtorch/converters/to_qiskit.py
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/pyqtorch/core/__init__.py
--rw-r--r--   0        0        0    24532 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/pyqtorch/core/batched_operation.py
--rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/pyqtorch/core/circuit.py
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/pyqtorch/core/measurement.py
--rw-r--r--   0        0        0    23548 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/pyqtorch/core/operation.py
--rw-r--r--   0        0        0     6499 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/pyqtorch/core/utils.py
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/pyqtorch/modules/__init__.py
--rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/pyqtorch/modules/abstract.py
--rw-r--r--   0        0        0     6904 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/pyqtorch/modules/circuit.py
--rw-r--r--   0        0        0    12189 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/pyqtorch/modules/hamevo.py
--rw-r--r--   0        0        0    14141 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/pyqtorch/modules/parametric.py
--rw-r--r--   0        0        0    13235 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/pyqtorch/modules/primitive.py
--rw-r--r--   0        0        0     5393 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/pyqtorch/modules/utils.py
--rw-r--r--   0        0        0     3046 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/tests/conftest.py
--rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/tests/test_batched_operations.py
--rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/tests/test_converters.py
--rw-r--r--   0        0        0     7185 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/tests/test_module_hamevo.py
--rw-r--r--   0        0        0     8719 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/tests/test_modules.py
--rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/tests/test_notebooks.py
--rw-r--r--   0        0        0     6034 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/tests/test_operations.py
--rw-r--r--   0        0        0     6496 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/tests/test_operations_hamevo.py
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/LICENSE
--rw-r--r--   0        0        0     2830 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/README.md
+-rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/mkdocs.yml
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/publish.sh
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/readthedocs.yml
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/setup.py
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/.github/workflows/run-tests-and-mypy.yml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/docs/CODE_OF_CONDUCT.md -> ../CODE_OF_CONDUCT.md
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/docs/CONTRIBUTING.md -> ../CONTRIBUTING.md
+-rw-r--r--   0        0        0    57645 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/docs/QAOA.ipynb
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/docs/circuit.md
+-rw-r--r--   0        0        0     6493 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/docs/essentials.ipynb
+-rw-r--r--   0        0        0   154246 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/docs/fit_function.ipynb
+-rw-r--r--   0        0        0     2854 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/docs/gate_composition.ipynb
+-rw-r--r--   0        0        0     4634 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/docs/hamevo.md
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/docs/index.md
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/docs/matrices.md
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/docs/parametric.md
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/docs/primitive.md
+-rw-r--r--   0        0        0    46162 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/docs/deprecated/QAOA.ipynb
+-rw-r--r--   0        0        0    19339 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/docs/deprecated/bench.py
+-rw-r--r--   0        0        0    74042 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/docs/deprecated/fit_function.ipynb
+-rw-r--r--   0        0        0    74062 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/docs/deprecated/getting_started.ipynb
+-rw-r--r--   0        0        0   121176 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/docs/deprecated/ham_evol_comparison.ipynb
+-rw-r--r--   0        0        0     6459 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/docs/deprecated/state_evolution.ipynb
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/pyqtorch/__init__.py
+-rw-r--r--   0        0        0     3544 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/pyqtorch/ansatz.py
+-rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/pyqtorch/embedding.py
+-rw-r--r--   0        0        0     4939 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/pyqtorch/matrices.py
+-rw-r--r--   0        0        0     6255 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/pyqtorch/matrices_sparse.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/pyqtorch/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/pyqtorch/converters/__init__.py
+-rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/pyqtorch/converters/store_ops.py
+-rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/pyqtorch/converters/to_qiskit.py
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/pyqtorch/core/__init__.py
+-rw-r--r--   0        0        0    24532 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/pyqtorch/core/batched_operation.py
+-rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/pyqtorch/core/circuit.py
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/pyqtorch/core/measurement.py
+-rw-r--r--   0        0        0    23548 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/pyqtorch/core/operation.py
+-rw-r--r--   0        0        0     6499 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/pyqtorch/core/utils.py
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/pyqtorch/modules/__init__.py
+-rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/pyqtorch/modules/abstract.py
+-rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/pyqtorch/modules/apply.py
+-rw-r--r--   0        0        0     6904 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/pyqtorch/modules/circuit.py
+-rw-r--r--   0        0        0    12217 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/pyqtorch/modules/hamevo.py
+-rw-r--r--   0        0        0    14141 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/pyqtorch/modules/parametric.py
+-rw-r--r--   0        0        0    13235 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/pyqtorch/modules/primitive.py
+-rw-r--r--   0        0        0     5393 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/pyqtorch/modules/utils.py
+-rw-r--r--   0        0        0     3046 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/tests/conftest.py
+-rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/tests/test_batched_operations.py
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/tests/test_circ_matrices.py
+-rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/tests/test_converters.py
+-rw-r--r--   0        0        0     8146 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/tests/test_module_hamevo.py
+-rw-r--r--   0        0        0    10001 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/tests/test_modules.py
+-rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/tests/test_notebooks.py
+-rw-r--r--   0        0        0     6034 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/tests/test_operations.py
+-rw-r--r--   0        0        0     6496 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/tests/test_operations_hamevo.py
+-rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/tests/test_sparse_modules.py
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/LICENSE
+-rw-r--r--   0        0        0     2830 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/PKG-INFO
```

### Comparing `pyqtorch-0.3.3/.pre-commit-config.yaml` & `pyqtorch-0.4.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.3/CODE_OF_CONDUCT.md` & `pyqtorch-0.4.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.3/CONTRIBUTING.md` & `pyqtorch-0.4.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.3/mkdocs.yml` & `pyqtorch-0.4.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.3/.github/workflows/run-tests-and-mypy.yml` & `pyqtorch-0.4.0/.github/workflows/run-tests-and-mypy.yml`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.3/docs/QAOA.ipynb` & `pyqtorch-0.4.0/docs/QAOA.ipynb`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.3/docs/essentials.ipynb` & `pyqtorch-0.4.0/docs/essentials.ipynb`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.3/docs/fit_function.ipynb` & `pyqtorch-0.4.0/docs/fit_function.ipynb`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.3/docs/gate_composition.ipynb` & `pyqtorch-0.4.0/docs/gate_composition.ipynb`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.3/docs/hamevo.md` & `pyqtorch-0.4.0/docs/hamevo.md`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.3/docs/deprecated/QAOA.ipynb` & `pyqtorch-0.4.0/docs/deprecated/QAOA.ipynb`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.3/docs/deprecated/bench.py` & `pyqtorch-0.4.0/docs/deprecated/bench.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.3/docs/deprecated/fit_function.ipynb` & `pyqtorch-0.4.0/docs/deprecated/fit_function.ipynb`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.3/docs/deprecated/getting_started.ipynb` & `pyqtorch-0.4.0/docs/deprecated/getting_started.ipynb`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.3/docs/deprecated/ham_evol_comparison.ipynb` & `pyqtorch-0.4.0/docs/deprecated/ham_evol_comparison.ipynb`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.3/docs/deprecated/state_evolution.ipynb` & `pyqtorch-0.4.0/docs/deprecated/state_evolution.ipynb`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.3/pyqtorch/__init__.py` & `pyqtorch-0.4.0/pyqtorch/__init__.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.3/pyqtorch/ansatz.py` & `pyqtorch-0.4.0/pyqtorch/ansatz.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.3/pyqtorch/embedding.py` & `pyqtorch-0.4.0/pyqtorch/embedding.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.3/pyqtorch/matrices.py` & `pyqtorch-0.4.0/pyqtorch/matrices.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.3/pyqtorch/matrices_sparse.py` & `pyqtorch-0.4.0/pyqtorch/matrices_sparse.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.3/pyqtorch/converters/store_ops.py` & `pyqtorch-0.4.0/pyqtorch/converters/store_ops.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.3/pyqtorch/converters/to_qiskit.py` & `pyqtorch-0.4.0/pyqtorch/converters/to_qiskit.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.3/pyqtorch/core/__init__.py` & `pyqtorch-0.4.0/pyqtorch/core/__init__.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.3/pyqtorch/core/batched_operation.py` & `pyqtorch-0.4.0/pyqtorch/core/batched_operation.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.3/pyqtorch/core/circuit.py` & `pyqtorch-0.4.0/pyqtorch/core/circuit.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.3/pyqtorch/core/measurement.py` & `pyqtorch-0.4.0/pyqtorch/core/measurement.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.3/pyqtorch/core/operation.py` & `pyqtorch-0.4.0/pyqtorch/core/operation.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.3/pyqtorch/core/utils.py` & `pyqtorch-0.4.0/pyqtorch/core/utils.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.3/pyqtorch/modules/__init__.py` & `pyqtorch-0.4.0/pyqtorch/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.3/pyqtorch/modules/abstract.py` & `pyqtorch-0.4.0/pyqtorch/modules/abstract.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.3/pyqtorch/modules/circuit.py` & `pyqtorch-0.4.0/pyqtorch/modules/circuit.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.3/pyqtorch/modules/hamevo.py` & `pyqtorch-0.4.0/pyqtorch/modules/hamevo.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
     def __init__(
         self, H: torch.Tensor, t: torch.Tensor, qubits: Any, n_qubits: int, n_steps: int = 100
     ):
         super().__init__()
         self.H: torch.Tensor
         self.t: torch.Tensor
-        self.qubits = qubits
+        self.qubits = [n_qubits - i - 1 for i in qubits]
         self.n_qubits = n_qubits
         self.n_steps = n_steps
         if H.ndim == 2:
             H = H.unsqueeze(2)
         if H.size(-1) == t.size(0) or t.size(0) == 1:
             self.register_buffer("H", H)
             self.register_buffer("t", t)
```

### Comparing `pyqtorch-0.3.3/pyqtorch/modules/parametric.py` & `pyqtorch-0.4.0/pyqtorch/modules/parametric.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.3/pyqtorch/modules/primitive.py` & `pyqtorch-0.4.0/pyqtorch/modules/primitive.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.3/pyqtorch/modules/utils.py` & `pyqtorch-0.4.0/pyqtorch/modules/utils.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.3/tests/conftest.py` & `pyqtorch-0.4.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.3/tests/test_batched_operations.py` & `pyqtorch-0.4.0/tests/test_batched_operations.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.3/tests/test_converters.py` & `pyqtorch-0.4.0/tests/test_converters.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.3/tests/test_module_hamevo.py` & `pyqtorch-0.4.0/tests/test_module_hamevo.py`

 * *Files 13% similar despite different names*

```diff
@@ -122,15 +122,14 @@
     H = Hamiltonian(batch_size)
     t_evo = torch.tensor([torch.pi / 4], dtype=torch.cdouble)
 
     hamevo = ham_evo(H, t_evo, range(n_qubits), n_qubits)
     psi = pyq.uniform_state(n_qubits, batch_size)
     psi_star = hamevo.forward(psi)
     result = overlap(psi_star, psi)
-    print(result)
 
     assert map(isclose, zip(result, [0.5, 0.5]))  # type: ignore [arg-type]
 
 
 @pytest.mark.parametrize("get_hamiltonians", [Hamiltonian_general, Hamiltonian_diag])
 def test_hamevo_consistency(get_hamiltonians: Callable) -> None:
     n_qubits = 4
@@ -218,7 +217,36 @@
     assert isinstance(ham_evo_instance, ham_evo_class)
 
     psi = pyq.uniform_state(n_qubits)
     psi_star = hamevo(H, t_evo, psi)
     result = overlap(psi_star, psi)
     assert result.size() == (batch_size,)
     assert torch.allclose(result, target)
+
+
+def test_hamevo_endianness() -> None:
+    t = torch.ones(1)
+    h = torch.tensor(
+        [
+            [0.9701, 0.0000, 0.7078, 0.0000],
+            [0.0000, 0.9701, 0.0000, 0.7078],
+            [0.4594, 0.0000, 0.9207, 0.0000],
+            [0.0000, 0.4594, 0.0000, 0.9207],
+        ]
+    )
+    iszero = torch.tensor([False, True, False, True])
+    op = pyq.HamEvoExp(h, t, qubits=[0, 1], n_qubits=2)
+    st = op(pyq.zero_state(2)).flatten()
+    assert torch.allclose(st[iszero], torch.zeros(1, dtype=torch.cdouble))
+
+    h = torch.tensor(
+        [
+            [0.9701, 0.7078, 0.0000, 0.0000],
+            [0.4594, 0.9207, 0.0000, 0.0000],
+            [0.0000, 0.0000, 0.9701, 0.7078],
+            [0.0000, 0.0000, 0.4594, 0.9207],
+        ]
+    )
+    iszero = torch.tensor([False, False, True, True])
+    op = pyq.HamEvoExp(h, t, qubits=[0, 1], n_qubits=2)
+    st = op(pyq.zero_state(2)).flatten()
+    assert torch.allclose(st[iszero], torch.zeros(1, dtype=torch.cdouble))
```

### Comparing `pyqtorch-0.3.3/tests/test_modules.py` & `pyqtorch-0.4.0/tests/test_modules.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,118 +5,132 @@
 import pytest
 import torch
 
 import pyqtorch.core as func_pyq
 import pyqtorch.modules as pyq
 from pyqtorch.modules.abstract import AbstractGate
 
-state_000 = pyq.zero_state(3, device="cpu", dtype=torch.cdouble)
+DEVICE = "cuda" if torch.cuda.is_available() else "cpu"
+DTYPE = torch.cdouble
+
+state_000 = pyq.zero_state(3, device=DEVICE, dtype=DTYPE)
 state_001 = pyq.X(qubits=[2], n_qubits=3)(state_000)
 state_100 = pyq.X(qubits=[0], n_qubits=3)(state_000)
 state_101 = pyq.X(qubits=[2], n_qubits=3)(pyq.X(qubits=[0], n_qubits=3)(state_000))
 state_110 = pyq.X(qubits=[1], n_qubits=3)(pyq.X(qubits=[0], n_qubits=3)(state_000))
 
 
+@pytest.mark.parametrize("batch_size", [i for i in range(1, 2, 10)])
+@pytest.mark.parametrize("n_qubits", [i for i in range(1, 6)])
 @pytest.mark.parametrize("gate", ["X", "Y", "Z", "H", "I", "S", "T", "Sdagger"])
-def test_constant_gates(gate: str) -> None:
+def test_constant_gates(batch_size: int, n_qubits: int, gate: str) -> None:
     dtype = torch.cdouble
-    device = "cpu"
-    batch_size = 100
-    qubits = [0]
-    n_qubits = 2
-
-    state = pyq.zero_state(n_qubits, batch_size=batch_size, device=device, dtype=dtype)
-    phi = torch.rand(batch_size, device=device, dtype=dtype)
+    qubits = [torch.randint(low=0, high=n_qubits, size=(1,)).item()]
 
+    state = pyq.random_state(n_qubits, batch_size=batch_size, device=DEVICE, dtype=DTYPE)
     Op = getattr(pyq, gate)
     FuncOp = getattr(func_pyq.operation, gate)
 
     func_out = FuncOp(state, qubits, n_qubits)
-    op = Op(qubits, n_qubits).to(device=device, dtype=dtype)
+    op = Op(qubits, n_qubits).to(device=DEVICE, dtype=dtype)
     mod_out = op(state)
 
     assert torch.allclose(func_out, mod_out)
 
 
+@pytest.mark.parametrize("batch_size", [i for i in range(1, 2, 10)])
+@pytest.mark.parametrize("n_qubits", [i for i in range(1, 6)])
 @pytest.mark.parametrize("gate", ["RX", "RY", "RZ"])
-def test_parametrized_gates(gate: str) -> None:
-    dtype = torch.cdouble
-    device = "cpu"
-    batch_size = 100
-    qubits = [0]
-    n_qubits = 2
+def test_parametrized_gates(batch_size: int, n_qubits: int, gate: str) -> None:
+    qubits = [torch.randint(low=0, high=n_qubits, size=(1,)).item()]
 
-    state = pyq.zero_state(n_qubits, batch_size=batch_size, device=device, dtype=dtype)
-    phi = torch.rand(batch_size, device=device, dtype=dtype)
+    state = pyq.random_state(n_qubits, batch_size=batch_size, device=DEVICE, dtype=DTYPE)
+    phi = torch.rand(batch_size, device=DEVICE, dtype=DTYPE)
 
     Op = getattr(pyq, gate)
     FuncOp = getattr(func_pyq.batched_operation, f"batched{gate}")
 
     func_out = FuncOp(phi, state, qubits, n_qubits)
-    op = Op(qubits, n_qubits).to(device=device, dtype=dtype)
+    op = Op(qubits, n_qubits).to(device=DEVICE, dtype=DTYPE)
     mod_out = op(state, phi)
 
     assert torch.allclose(func_out, mod_out)
 
 
-@pytest.mark.parametrize("batch_size", [1, 2, 4, 6])
-def test_circuit(batch_size: int) -> None:
-    n_qubits = 2
-    device = "cuda" if torch.cuda.is_available() else "cpu"
-    dtype = torch.cdouble
+@pytest.mark.parametrize("batch_size", [i for i in range(1, 2, 10)])
+@pytest.mark.parametrize("n_qubits", [i for i in range(2, 6)])
+@pytest.mark.parametrize("gate", ["CRX", "CRY", "CRZ"])
+def test_controlled_parametrized_gates(batch_size: int, n_qubits: int, gate: str) -> None:
+    qubits = torch.randint(low=0, high=n_qubits, size=(2,))
+
+    while qubits[0] == qubits[1]:
+        qubits[1] = torch.randint(low=0, high=n_qubits, size=(1,))
 
+    qubits = [qubits[0].item(), qubits[1].item()]
+
+    state = pyq.random_state(n_qubits, batch_size=batch_size, device=DEVICE, dtype=DTYPE)
+    phi = torch.rand(batch_size, device=DEVICE, dtype=DTYPE)
+
+    Op = getattr(pyq, gate)
+    BatchedOP = getattr(func_pyq.batched_operation, f"batched{gate}")
+
+    func_out = BatchedOP(phi, state, qubits, n_qubits)
+    op = Op(qubits, n_qubits).to(device=DEVICE, dtype=DTYPE)
+    mod_out = op(state, phi)
+
+    assert torch.allclose(func_out, mod_out)
+
+
+@pytest.mark.parametrize("batch_size", [i for i in range(1, 2, 10)])
+@pytest.mark.parametrize("n_qubits", [i for i in range(2, 6)])
+def test_circuit(batch_size: int, n_qubits: int) -> None:
     ops = [
         pyq.X([0], n_qubits),
         pyq.X([1], n_qubits),
         pyq.RX([1], n_qubits),
         pyq.CNOT([0, 1], n_qubits),
     ]
-    circ = pyq.QuantumCircuit(n_qubits, ops).to(device=device, dtype=dtype)
+    circ = pyq.QuantumCircuit(n_qubits, ops).to(device=DEVICE, dtype=DTYPE)
 
-    state = circ.init_state(batch_size)
-    phi = torch.rand(batch_size, device=device, dtype=dtype, requires_grad=True)
+    state = pyq.random_state(n_qubits, batch_size)
+    phi = torch.rand(batch_size, device=DEVICE, dtype=DTYPE, requires_grad=True)
 
-    assert circ(state, phi).size() == (2, 2, batch_size)
+    assert circ(state, phi).size() == tuple(2 for _ in range(n_qubits)) + (batch_size,)
 
-    state = pyq.zero_state(n_qubits, batch_size=batch_size, device=device, dtype=dtype)
+    state = pyq.random_state(n_qubits, batch_size=batch_size, device=DEVICE, dtype=DTYPE)
 
     res = circ(state, phi)
     assert not torch.all(torch.isnan(res))
-
-    # g = torch.autograd.grad(circ, thetas)
     dres_theta = torch.autograd.grad(res, phi, torch.ones_like(res), create_graph=True)[0]
     assert not torch.all(torch.isnan(dres_theta))
 
 
 @pytest.mark.parametrize("batch_size", [1, 2, 4, 6])
 def test_empty_circuit(batch_size: int) -> None:
     n_qubits = 2
-    device = "cuda" if torch.cuda.is_available() else "cpu"
-    dtype = torch.cdouble
-
     ops: list = []
-    circ = pyq.QuantumCircuit(n_qubits, ops).to(device=device, dtype=dtype)
+    circ = pyq.QuantumCircuit(n_qubits, ops).to(device=DEVICE, dtype=DTYPE)
 
     state = circ.init_state(batch_size)
-    phi = torch.rand(batch_size, device=device, dtype=dtype, requires_grad=True)
+    phi = torch.rand(batch_size, device=DEVICE, dtype=DTYPE, requires_grad=True)
 
     assert circ(state, phi).size() == (2, 2, batch_size)
 
-    state = pyq.zero_state(n_qubits, batch_size=batch_size, device=device, dtype=dtype)
+    state = pyq.random_state(n_qubits, batch_size=batch_size, device=DEVICE, dtype=DTYPE)
 
     res = circ(state, phi)
     assert not torch.all(torch.isnan(res))
 
 
 @pytest.mark.parametrize("batch_size", [1, 2, 4, 6])
 def test_U_gate(batch_size: int) -> None:
     n_qubits = 1
     u = pyq.U([0], n_qubits)
     x = torch.rand(3, batch_size)
-    state = pyq.zero_state(n_qubits, batch_size=batch_size, device="cpu", dtype=torch.cdouble)
+    state = pyq.random_state(n_qubits, batch_size=batch_size, device=DEVICE, dtype=DTYPE)
     assert not torch.all(torch.isnan(u(state, x)))
 
 
 @pytest.mark.parametrize(
     "a,b,val",
     [
         (pyq.X([0], 1), pyq.X([0], 1), True),
@@ -229,29 +243,29 @@
     assert torch.allclose(cswap(state_110), state_101)
 
 
 @pytest.mark.parametrize("state_fn", [pyq.random_state, pyq.zero_state, pyq.uniform_state])
 @pytest.mark.parametrize("n_qubits", [i for i in range(1, 8)])
 @pytest.mark.parametrize("batch_size", [i for i in range(1, 8)])
 def test_isnormalized_states(state_fn: Callable, n_qubits: int, batch_size: int) -> None:
-    state = state_fn(n_qubits, batch_size)
+    state = state_fn(n_qubits, batch_size, device=DEVICE, dtype=DTYPE)
     assert pyq.is_normalized(state)
 
 
 @pytest.mark.parametrize("n_qubits", [i for i in range(1, 8)])
 @pytest.mark.parametrize("batch_size", [i for i in range(1, 8)])
 def test_state_shapes(n_qubits: int, batch_size: int) -> None:
-    zero = pyq.zero_state(n_qubits, batch_size)
-    uni = pyq.uniform_state(n_qubits, batch_size)
-    rand = pyq.random_state(n_qubits, batch_size)
+    zero = pyq.zero_state(n_qubits, batch_size, device=DEVICE, dtype=DTYPE)
+    uni = pyq.uniform_state(n_qubits, batch_size, device=DEVICE, dtype=DTYPE)
+    rand = pyq.random_state(n_qubits, batch_size, device=DEVICE, dtype=DTYPE)
     assert zero.shape == rand.shape and uni.shape == rand.shape
 
 
 @pytest.mark.parametrize("state_fn", [pyq.random_state, pyq.zero_state, pyq.uniform_state])
 @pytest.mark.parametrize("n_qubits", [i for i in range(1, 8)])
 @pytest.mark.parametrize("batch_size", [i for i in range(1, 8)])
 def test_overlap_states_batch_nqubits(state_fn: Callable, n_qubits: int, batch_size: int) -> None:
-    state = state_fn(n_qubits, batch_size)
+    state = state_fn(n_qubits, batch_size, device=DEVICE, dtype=DTYPE)
     assert torch.allclose(
         pyq.overlap(state, state),
         torch.ones(batch_size),
     )
```

### Comparing `pyqtorch-0.3.3/tests/test_notebooks.py` & `pyqtorch-0.4.0/tests/test_notebooks.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.3/tests/test_operations.py` & `pyqtorch-0.4.0/tests/test_operations.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.3/tests/test_operations_hamevo.py` & `pyqtorch-0.4.0/tests/test_operations_hamevo.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.3/.gitignore` & `pyqtorch-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.3/LICENSE` & `pyqtorch-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.3/pyproject.toml` & `pyqtorch-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     { name = "Aleksander Wennersteen", email = "aleksander.wennersteen@pasqal.com" },
     { name = "Mario Dagrada", email = "mario.dagrada@pasqal.com" },
     { name = "Dominik Seitz", email = "dominik.seitz@pasqal.com" },
     { name = "Niklas Heim", email = "niklas.heim@pasqal.com" },
 ]
 requires-python = ">=3.8,<3.12"
 license = {text = "Proprietary"}
-version = "0.3.3"
+version = "0.4.0"
 classifiers=[
     "License :: Other/Proprietary License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
```

### Comparing `pyqtorch-0.3.3/PKG-INFO` & `pyqtorch-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyqtorch
-Version: 0.3.3
+Version: 0.4.0
 Summary: An efficient, large-scale emulator designed for quantum machine learning, seamlessly integrated with a PyTorch backend. Please refer to https://pyqtorch.readthedocs.io/en/latest/ for setup and usage info, along with the full documentation.
 Author-email: Slimane Thabet <slimane.thabet@pasqal.com>, Aleksander Wennersteen <aleksander.wennersteen@pasqal.com>, Mario Dagrada <mario.dagrada@pasqal.com>, Dominik Seitz <dominik.seitz@pasqal.com>, Niklas Heim <niklas.heim@pasqal.com>
 License: Proprietary
 License-File: LICENSE
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

