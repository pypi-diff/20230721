# Comparing `tmp/nutpie-0.6.0.tar.gz` & `tmp/nutpie-0.7.0.tar.gz`

## Comparing `nutpie-0.6.0.tar` & `nutpie-0.7.0.tar`

### file list

```diff
@@ -1,23 +1,25 @@
--rw-r--r--   0        0        0      988 1970-01-01 00:00:00.000000 nutpie-0.6.0/Cargo.toml
--rw-r--r--   0     1001      123     4882 2023-07-03 17:49:22.000000 nutpie-0.6.0/.github/workflows/ci.yml
--rw-r--r--   0     1001      123      143 2023-07-03 17:49:22.000000 nutpie-0.6.0/.gitignore
--rw-r--r--   0     1001      123     1072 2023-07-03 17:49:22.000000 nutpie-0.6.0/LICENSE
--rw-r--r--   0     1001      123     3583 2023-07-03 17:49:22.000000 nutpie-0.6.0/README.md
--rw-r--r--   0     1001      123     5212 2023-07-03 17:49:22.000000 nutpie-0.6.0/benches/run_tvm_leapfrog.rs_old
--rw-r--r--   0     1001      123       10 2023-07-03 17:49:33.000000 nutpie-0.6.0/dist/nutpie-0.6.0.tar.gz
--rw-r--r--   0     1001      123   251122 2023-07-03 17:49:22.000000 nutpie-0.6.0/notebooks/pytensor_logp.ipynb
--rw-r--r--   0     1001      123     7329 2023-07-03 17:49:22.000000 nutpie-0.6.0/notebooks/pytensor_logp.md
--rw-r--r--   0     1001      123      467 2023-07-03 17:49:22.000000 nutpie-0.6.0/nutpie/__init__.py
--rw-r--r--   0     1001      123    15805 2023-07-03 17:49:22.000000 nutpie-0.6.0/nutpie/compile_pymc.py
--rw-r--r--   0     1001      123     4395 2023-07-03 17:49:22.000000 nutpie-0.6.0/nutpie/compile_stan.py
--rw-r--r--   0     1001      123     8231 2023-07-03 17:49:22.000000 nutpie-0.6.0/nutpie/sample.py
--rw-r--r--   0     1001      123      861 2023-07-03 17:49:22.000000 nutpie-0.6.0/pyproject.toml
--rw-r--r--   0     1001      123       72 2023-07-03 17:49:22.000000 nutpie-0.6.0/src/lib.rs
--rw-r--r--   0     1001      123     7955 2023-07-03 17:49:22.000000 nutpie-0.6.0/src/pymc.rs
--rw-r--r--   0     1001      123     6783 2023-07-03 17:49:22.000000 nutpie-0.6.0/src/sampler.rs
--rw-r--r--   0     1001      123     9041 2023-07-03 17:49:22.000000 nutpie-0.6.0/src/stan.rs
--rw-r--r--   0     1001      123     8472 2023-07-03 17:49:22.000000 nutpie-0.6.0/src/wrapper.rs
--rw-r--r--   0     1001      123     1534 2023-07-03 17:49:22.000000 nutpie-0.6.0/tests/test_pymc.py
--rw-r--r--   0     1001      123      721 2023-07-03 17:49:22.000000 nutpie-0.6.0/tests/test_stan.py
--rw-r--r--   0     1001      123    34350 2023-07-03 17:49:22.000000 nutpie-0.6.0/Cargo.lock
--rw-r--r--   0        0        0     4721 1970-01-01 00:00:00.000000 nutpie-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0      985 1970-01-01 00:00:00.000000 nutpie-0.7.0/Cargo.toml
+-rw-r--r--   0     1001      123     4882 2023-07-21 02:15:54.000000 nutpie-0.7.0/.github/workflows/ci.yml
+-rw-r--r--   0     1001      123      143 2023-07-21 02:15:54.000000 nutpie-0.7.0/.gitignore
+-rw-r--r--   0     1001      123      901 2023-07-21 02:15:54.000000 nutpie-0.7.0/CHANGELOG.md
+-rw-r--r--   0     1001      123     1072 2023-07-21 02:15:54.000000 nutpie-0.7.0/LICENSE
+-rw-r--r--   0     1001      123     3583 2023-07-21 02:15:54.000000 nutpie-0.7.0/README.md
+-rw-r--r--   0     1001      123     5212 2023-07-21 02:15:54.000000 nutpie-0.7.0/benches/run_tvm_leapfrog.rs_old
+-rw-r--r--   0     1001      123     2654 2023-07-21 02:15:54.000000 nutpie-0.7.0/cliff.toml
+-rw-r--r--   0     1001      123       10 2023-07-21 02:16:15.000000 nutpie-0.7.0/dist/nutpie-0.7.0.tar.gz
+-rw-r--r--   0     1001      123   251122 2023-07-21 02:15:54.000000 nutpie-0.7.0/notebooks/pytensor_logp.ipynb
+-rw-r--r--   0     1001      123     7329 2023-07-21 02:15:54.000000 nutpie-0.7.0/notebooks/pytensor_logp.md
+-rw-r--r--   0     1001      123      914 2023-07-21 02:15:54.000000 nutpie-0.7.0/pyproject.toml
+-rw-r--r--   0     1001      123      567 2023-07-21 02:15:54.000000 nutpie-0.7.0/python/nutpie/__init__.py
+-rw-r--r--   0     1001      123    15179 2023-07-21 02:15:54.000000 nutpie-0.7.0/python/nutpie/compile_pymc.py
+-rw-r--r--   0     1001      123     4760 2023-07-21 02:15:54.000000 nutpie-0.7.0/python/nutpie/compile_stan.py
+-rw-r--r--   0     1001      123     8752 2023-07-21 02:15:54.000000 nutpie-0.7.0/python/nutpie/sample.py
+-rw-r--r--   0     1001      123       70 2023-07-21 02:15:54.000000 nutpie-0.7.0/src/lib.rs
+-rw-r--r--   0     1001      123     7955 2023-07-21 02:15:54.000000 nutpie-0.7.0/src/pymc.rs
+-rw-r--r--   0     1001      123     6783 2023-07-21 02:15:54.000000 nutpie-0.7.0/src/sampler.rs
+-rw-r--r--   0     1001      123     9236 2023-07-21 02:15:54.000000 nutpie-0.7.0/src/stan.rs
+-rw-r--r--   0     1001      123     8528 2023-07-21 02:15:54.000000 nutpie-0.7.0/src/wrapper.rs
+-rw-r--r--   0     1001      123     1521 2023-07-21 02:15:54.000000 nutpie-0.7.0/tests/test_pymc.py
+-rw-r--r--   0     1001      123      721 2023-07-21 02:15:54.000000 nutpie-0.7.0/tests/test_stan.py
+-rw-r--r--   0     1001      123    34889 2023-07-21 02:16:13.000000 nutpie-0.7.0/Cargo.lock
+-rw-r--r--   0        0        0     4721 1970-01-01 00:00:00.000000 nutpie-0.7.0/PKG-INFO
```

### Comparing `nutpie-0.6.0/Cargo.toml` & `nutpie-0.7.0/Cargo.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "nutpie"
-version = "0.6.0"
+version = "0.7.0"
 authors = [
     "Adrian Seyboldt <adrian.seyboldt@gmail.com>",
     "PyMC Developers <pymc.devs@gmail.com>"
 ]
 edition = "2021"
 license = "MIT"
 repository = "https://github.com/pymc-devs/nutpie"
@@ -13,32 +13,32 @@
 
 [features]
 extension-module = ["pyo3/extension-module"]
 default = ["extension-module"]
 simd_support = ["nuts-rs/simd_support"]
 
 [lib]
-name = "nutpie"
+name = "_lib"
 crate-type = ["cdylib"]
 
 [dependencies]
-nuts-rs = "0.5.0"
+nuts-rs = "0.6.0"
 numpy = "0.19.0"
 ndarray = "0.15.6"
 rand = "0.8.5"
-thiserror = "1.0.40"
+thiserror = "1.0.43"
 rand_chacha = "0.3.1"
 rayon = "1.7.0"
-arrow2 = "0.17.2"
-anyhow = "1.0.71"
+arrow2 = "0.17.3"
+anyhow = "1.0.72"
 itertools = "0.11.0"
-bridgestan = "=2.1.1"
+bridgestan = "2.1.2"
 
 [dependencies.pyo3]
-version = "0.19.0"
+version = "0.19.1"
 features = ["extension-module", "anyhow"]
 
 [dev-dependencies]
 criterion = "0.5.1"
 
 [profile.release]
 debug = true
```

### Comparing `nutpie-0.6.0/.github/workflows/ci.yml` & `nutpie-0.7.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `nutpie-0.6.0/LICENSE` & `nutpie-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nutpie-0.6.0/README.md` & `nutpie-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `nutpie-0.6.0/benches/run_tvm_leapfrog.rs_old` & `nutpie-0.7.0/benches/run_tvm_leapfrog.rs_old`

 * *Files identical despite different names*

### Comparing `nutpie-0.6.0/notebooks/pytensor_logp.ipynb` & `nutpie-0.7.0/notebooks/pytensor_logp.ipynb`

 * *Files identical despite different names*

### Comparing `nutpie-0.6.0/notebooks/pytensor_logp.md` & `nutpie-0.7.0/notebooks/pytensor_logp.md`

 * *Files identical despite different names*

### Comparing `nutpie-0.6.0/nutpie/compile_pymc.py` & `nutpie-0.7.0/python/nutpie/compile_pymc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import dataclasses
-import functools
 import itertools
 from dataclasses import dataclass
 from math import prod
 from typing import Any, Dict, Optional, Tuple
 
 import numba
 import numba.core.ccallback
@@ -13,16 +12,16 @@
 import pytensor
 import pytensor.link.numba.dispatch
 import pytensor.tensor as pt
 from numba import literal_unroll
 from numba.cpython.unsafe.tuple import alloca_once, tuple_setitem
 from numpy.typing import NDArray
 
-from . import lib
-from .sample import CompiledModel
+from nutpie import _lib
+from nutpie.sample import CompiledModel
 
 
 @numba.extending.intrinsic
 def address_as_void_pointer(typingctx, src):
     """returns a void pointer from a given memory address"""
     from numba.core import cgutils, types
 
@@ -80,34 +79,34 @@
             self,
             shared_data=shared_data,
             user_data=user_data,
         )
 
     def _make_sampler(self, settings, init_mean, chains, cores, seed):
         model = self._make_model(init_mean)
-        return lib.PySampler.from_pymc(settings, chains, cores, model, seed)
+        return _lib.PySampler.from_pymc(settings, chains, cores, model, seed)
 
     def _make_model(self, init_mean):
-        expand_fn = lib.ExpandFunc(
+        expand_fn = _lib.ExpandFunc(
             self.n_dim,
             self.n_expanded,
             self.compiled_expand_func.address,
             self.user_data.ctypes.data,
             self,
         )
-        logp_fn = lib.LogpFunc(
+        logp_fn = _lib.LogpFunc(
             self.n_dim,
             self.compiled_logp_func.address,
             self.user_data.ctypes.data,
             self,
         )
 
         var_sizes = [prod(shape) for shape in self.shape_info[2]]
 
-        return lib.PyMcModel(
+        return _lib.PyMcModel(
             self.n_dim,
             logp_fn,
             expand_fn,
             var_sizes,
             self.shape_info[0],
             init_mean,
         )
@@ -196,21 +195,21 @@
     for base, _, shape in zip(*shape_info):
         if base not in [var.name for var in model.value_vars]:
             continue
         for idx in itertools.product(*[range(length) for length in shape]):
             if len(idx) == 0:
                 names.append(base)
             else:
-                names.append(f"{base}_{'_'.join(str(i) for i in idx)}")
+                names.append(f"{base}_{'.'.join(str(i) for i in idx)}")
     coords["unconstrained_parameter"] = pd.Index(names)
 
     return CompiledPyMCModel(
         _n_dim=n_dim,
         dims=model.named_vars_to_dims,
-        _coords=model.coords,
+        _coords=coords,
         _shapes={name: tuple(shape) for name, _, shape in zip(*shape_info)},
         compiled_logp_func=logp_numba,
         compiled_expand_func=expand_numba,
         shared_data=shared_data,
         user_data=user_data,
         n_expanded=n_expanded,
         shape_info=shape_info,
@@ -303,31 +302,23 @@
             model.free_RVs,
             joined_shapes,
             variables,
         )
     }
 
     (logp, grad) = pytensor.graph_replace([logp, grad], replacements)
-    # (logp, grad) = pytensor.graph.rewrite_graph(logp, include=["canonicalize", "stabilize"])
-    # grad = pytensor.gradient.grad(logp, joined)
 
     # We should avoid compiling the function, and optimize only
     logp_fn_pt = pytensor.compile.function.function(
         (joined,), (logp, grad), mode=pytensor.compile.NUMBA
     )
 
     logp_fn = logp_fn_pt.vm.jit_fn
 
     # Make function that computes remaining variables for the trace
-    trace_vars = {
-        name: var
-        for (name, var) in model.named_vars.items()
-        if var not in model.observed_RVs + model.potentials
-    }
-    remaining_names = [name for name in trace_vars if name not in joined_names]
     remaining_rvs = [
         var for var in model.unobserved_value_vars if var.name not in joined_names
     ]
 
     all_names = joined_names + remaining_rvs
 
     all_names = joined_names.copy()
@@ -348,17 +339,14 @@
     expand_fn_pt = pytensor.compile.function.function(
         (joined,),
         (allvars,),
         givens=list(replacements.items()),
         mode=pytensor.compile.NUMBA,
     )
     expand_fn = expand_fn_pt.vm.jit_fn
-    # expand_fn = numba.njit(expand_fn, fastmath=True, error_model="numpy")
-    # Trigger a compile
-    # expand_fn(np.zeros(num_free_vars), *[var.get_value() for var in expand_fn_pt.get_shared()])
 
     return (
         num_free_vars,
         num_expanded,
         logp_fn_pt,
         logp_fn,
         expand_fn_pt,
@@ -424,16 +412,14 @@
         if not isinstance(index, numba.types.Literal):
             return
 
         index = index.literal_value
 
         name, ndim, base_shape, dtype = shared_metadata[index]
 
-        ndim_range = tuple(range(ndim))
-
         def impl(user_data, index):
             data_ptr = address_as_void_pointer(user_data["data"][name][()])
             data = numba.carray(data_ptr, int(user_data["size"][name][()]), dtype)
 
             shape = user_data["shape"][name]
 
             assert len(shape) == len(base_shape)
```

### Comparing `nutpie-0.6.0/nutpie/compile_stan.py` & `nutpie-0.7.0/python/nutpie/compile_stan.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import json
 import pathlib
 import tempfile
 from dataclasses import dataclass, replace
-from typing import Any, Dict, Optional
+from typing import Any, Dict, List, Optional
 
 import numpy as np
 import pandas as pd
 from numpy.typing import NDArray
 
-from nutpie import lib
+from nutpie import _lib
 from nutpie.sample import CompiledModel
 
 
 class _NumpyArrayEncoder(json.JSONEncoder):
     def default(self, obj):
         if isinstance(obj, np.ndarray):
             return obj.tolist()
@@ -37,15 +37,15 @@
         data.update(updates)
 
         if data is not None:
             data_json = json.dumps(data, cls=_NumpyArrayEncoder)
         else:
             data_json = None
 
-        model = lib.StanModel(self.library, seed, data_json)
+        model = _lib.StanModel(self.library, seed, data_json)
         coords = self._coords
         if coords is None:
             coords = {}
         else:
             coords = coords.copy()
         coords["unconstrained_parameter"] = pd.Index(model.param_unc_names())
 
@@ -77,15 +77,15 @@
     def _make_model(self, init_mean):
         if self.model is None:
             return self.with_data().model
         return self.model
 
     def _make_sampler(self, settings, init_mean, chains, cores, seed):
         model = self._make_model(init_mean)
-        return lib.PySampler.from_stan(settings, chains, cores, model, seed)
+        return _lib.PySampler.from_stan(settings, chains, cores, model, seed)
 
     @property
     def n_dim(self):
         if self.model is None:
             return self.with_data().n_dim
         return self.model.ndim()
 
@@ -100,22 +100,23 @@
         if self.model is None:
             return self.with_data().coords
         return self._coords
 
 
 def compile_stan_model(
     *,
-    code=None,
-    filename=None,
-    extra_compile_args=None,
-    dims=None,
-    coords=None,
-    model_name=None,
-    cleanup=True,
-):
+    code: Optional[str] = None,
+    filename: Optional[str] = None,
+    extra_compile_args: Optional[List[str]] = None,
+    extra_stanc_args: Optional[List[str]] = None,
+    dims: Optional[Dict[str, int]] = None,
+    coords: Optional[Dict[str, Any]] = None,
+    model_name: Optional[str] = None,
+    cleanup: bool = True,
+) -> CompiledStanModel:
     import bridgestan
 
     if dims is None:
         dims = {}
     if coords is None:
         coords = {}
 
@@ -138,18 +139,23 @@
             .with_name(model_name)  # This verifies that it is a valid filename
             .with_suffix(".stan")
         )
         model_path.write_text(code)
         make_args = ["STAN_THREADS=true"]
         if extra_compile_args:
             make_args.extend(extra_compile_args)
-        so_path = bridgestan.compile_model(model_path, make_args=make_args)
+        stanc_args = []
+        if extra_stanc_args:
+            stanc_args.extend(extra_stanc_args)
+        so_path = bridgestan.compile_model(
+            model_path, make_args=make_args, stanc_args=stanc_args
+        )
         # Set necessary library loading paths
         bridgestan.compile.windows_dll_path_setup()
-        library = lib.StanLibrary(so_path)
+        library = _lib.StanLibrary(so_path)
     finally:
         try:
             if cleanup:
                 basedir.cleanup()
         except Exception:
             pass
```

### Comparing `nutpie-0.6.0/nutpie/sample.py` & `nutpie-0.7.0/python/nutpie/sample.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,17 +2,16 @@
 from typing import Dict, Optional, Tuple
 
 import arviz
 import fastprogress
 import numpy as np
 import pandas as pd
 import pyarrow
-import xarray as xr
 
-from . import lib
+from nutpie import _lib
 
 
 @dataclass(frozen=True)
 class CompiledModel:
     dims: Optional[Dict[str, Tuple[str, ...]]]
 
     @property
@@ -42,19 +41,22 @@
         times = []
         if isinstance(cores, int):
             cores = [cores]
         for num_cores in cores:
             if num_cores == 0:
                 continue
             flat = model.benchmark_logp(point, num_cores, num_evals)
+            data = pd.DataFrame(flat)
+            data.index = pd.MultiIndex.from_product(
+                [range(num_cores), [num_cores]],
+                names=["thread", "concurrent_cores"]
+            )
             data = (
-                pd.DataFrame(flat)
-                .rename_axis(index="concurrent_cores", columns="evaluation")
-                .unstack()
-                .rename("seconds")
+                data
+                .rename_axis(columns="evaluation")
             )
             times.append(data)
         return pd.concat(times)
 
 
 def _trace_to_arviz(traces, n_tune, shapes, **kwargs):
     n_chains = len(traces)
@@ -87,15 +89,15 @@
                 (len(chunk),) + shapes[name]
             )
 
         data_dict[name] = data[:, n_tune:]
         data_dict_tune[name] = data[:, :n_tune]
 
     for name, col in zip(table_stats.column_names, table_stats.columns):
-        if name in ["chain", "draw"]:
+        if name in ["chain", "draw", "divergence_message"]:
             continue
         col_type = col.type
         if hasattr(col_type, "list_size"):
             last_shape = (col_type.list_size,)
             dtype = col_type.field(0).type.to_pandas_dtype()
         else:
             dtype = col_type.to_pandas_dtype()
@@ -160,15 +162,18 @@
         Fail if we can't find a valid initializion point after
         this many tries.
     save_warmup: bool
         Wether to save the tuning (warmup) statistics and
         posterior draws in the output dataset.
     store_divergences: bool
         If true, store the exact locations where diverging
-        transitions happend in the sampler stats.
+        transitions happend in the sampler stats. This is currently
+        experimental, as the implementation is very wastefull
+        with memory, and a better interface will need breaking
+        changes.
     progress_bar: bool
         If true, display the progress bar (default)
     init_mean: ndarray
         Initialize the chains using jittered values around this
         point on the transformed parameter space. Defaults to
         zeros.
     store_unconstrained: bool
@@ -189,22 +194,22 @@
         The maximum depth of the tree for each draw. The maximum
         number of gradient evaluations for each draw will
         be 2 ^ maxdepth.
     return_raw_trace: bool, default=False
         Return the raw trace object (an apache arrow structure)
         instead of converting to arviz.
     **kwargs
-        Pass additional arguments to nutpie.lib.PySamplerArgs
+        Pass additional arguments to nutpie._lib.PySamplerArgs
 
     Returns
     -------
     trace : arviz.InferenceData
         An ArviZ ``InferenceData`` object that contains the samples.
     """
-    settings = lib.PySamplerArgs()
+    settings = _lib.PySamplerArgs()
     settings.num_tune = tune
     settings.num_draws = draws
 
     for name, val in kwargs.items():
         setattr(settings, name, val)
 
     if init_mean is None:
@@ -234,14 +239,18 @@
     finally:
         results = sampler.finalize()
 
     dims = {name: list(dim) for name, dim in compiled_model.dims.items()}
     dims["mass_matrix_inv"] = ["unconstrained_parameter"]
     dims["gradient"] = ["unconstrained_parameter"]
     dims["unconstrained_draw"] = ["unconstrained_parameter"]
+    dims["divergence_start"] = ["unconstrained_parameter"]
+    dims["divergence_start_gradient"] = ["unconstrained_parameter"]
+    dims["divergence_end"] = ["unconstrained_parameter"]
+    dims["divergence_momentum"] = ["unconstrained_parameter"]
 
     if return_raw_trace:
         return results
     else:
         return _trace_to_arviz(
             results,
             tune,
```

### Comparing `nutpie-0.6.0/src/pymc.rs` & `nutpie-0.7.0/src/pymc.rs`

 * *Files identical despite different names*

### Comparing `nutpie-0.6.0/src/sampler.rs` & `nutpie-0.7.0/src/sampler.rs`

 * *Files identical despite different names*

### Comparing `nutpie-0.6.0/src/stan.rs` & `nutpie-0.7.0/src/stan.rs`

 * *Files 2% similar despite different names*

```diff
@@ -192,28 +192,36 @@
         Ok(out)
     }
 }
 
 pub struct StanDensity<'model>(&'model InnerModel);
 
 #[derive(Debug, Error)]
-#[error("Error during logp evaluation: {0}")]
-pub struct StanLogpError(#[from] bridgestan::BridgeStanError);
+pub enum StanLogpError {
+    #[error("Error during logp evaluation: {0}")]
+    BridgeStan(#[from] bridgestan::BridgeStanError),
+    #[error("Bad logp value: {0}")]
+    BadLogp(f64),
+}
 
 impl LogpError for StanLogpError {
     fn is_recoverable(&self) -> bool {
         true
     }
 }
 
 impl<'model> CpuLogpFunc for StanDensity<'model> {
     type Err = StanLogpError;
 
     fn logp(&mut self, position: &[f64], grad: &mut [f64]) -> Result<f64, Self::Err> {
-        Ok(self.0.log_density_gradient(position, true, true, grad)?)
+        let logp = self.0.log_density_gradient(position, true, true, grad)?;
+        if !logp.is_finite() {
+            return Err(StanLogpError::BadLogp(logp));
+        }
+        Ok(logp)
     }
 
     fn dim(&self) -> usize {
         self.0.param_unc_num()
     }
 }
```

### Comparing `nutpie-0.6.0/src/wrapper.rs` & `nutpie-0.7.0/src/wrapper.rs`

 * *Files 1% similar despite different names*

```diff
@@ -170,15 +170,15 @@
     }
 
     #[getter]
     fn max_energy_error(&self) -> f64 {
         self.inner.max_energy_error
     }
 
-    #[setter(energy_error)]
+    #[setter(max_energy_error)]
     fn set_max_energy_error(&mut self, val: f64) {
         self.inner.max_energy_error = val
     }
 
     #[setter(target_accept)]
     fn set_target_accept(&mut self, val: f64) {
         self.inner
@@ -323,18 +323,19 @@
         ),
     )?;
     Ok(data.into_py(py))
 }
 
 /// A Python module implemented in Rust.
 #[pymodule]
-pub fn nutpie(_py: Python, m: &PyModule) -> PyResult<()> {
+pub fn _lib(_py: Python, m: &PyModule) -> PyResult<()> {
     m.add_class::<PySamplerArgs>()?;
     m.add_class::<PySampleStats>()?;
     m.add_class::<PySampler>()?;
     m.add_class::<PyMcModel>()?;
     m.add_class::<LogpFunc>()?;
     m.add_class::<ExpandFunc>()?;
     m.add_class::<StanLibrary>()?;
     m.add_class::<StanModel>()?;
+    m.add("__version__", env!("CARGO_PKG_VERSION"))?;
     Ok(())
 }
```

### Comparing `nutpie-0.6.0/tests/test_pymc.py` & `nutpie-0.7.0/tests/test_pymc.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     trace = nutpie.sample(compiled, chains=1)
     trace.posterior.a
 
 
 def test_det():
     with pm.Model() as model:
         a = pm.Uniform("a", shape=2)
-        b = pm.Deterministic("b", 2 * a)
+        pm.Deterministic("b", 2 * a)
 
     compiled = nutpie.compile_pymc_model(model)
     trace = nutpie.sample(compiled, chains=1)
     assert trace.posterior.a.shape[-1] == 2
     assert trace.posterior.b.shape[-1] == 2
 
 
@@ -47,8 +47,8 @@
 
     compiled2 = compiled.with_data(mu=10.0, sigma=3 * np.ones(3))
     trace2 = nutpie.sample(compiled2, chains=1, seed=1)
     np.testing.assert_allclose(trace2.posterior.a.mean().values, 10.0, atol=0.5)
 
     compiled3 = compiled.with_data(mu=0.5, sigma=3 * np.ones(4))
     with pytest.raises(ValueError):
-        trace3 = nutpie.sample(compiled3, chains=1)
+        nutpie.sample(compiled3, chains=1)
```

### Comparing `nutpie-0.6.0/tests/test_stan.py` & `nutpie-0.7.0/tests/test_stan.py`

 * *Files identical despite different names*

### Comparing `nutpie-0.6.0/Cargo.lock` & `nutpie-0.7.0/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,23 @@
  "cfg-if",
  "getrandom",
  "once_cell",
  "version_check",
 ]
 
 [[package]]
+name = "aho-corasick"
+version = "1.0.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "43f6cb1bf222025340178f382c426f13757b2960e89779dfcb319c32542a5a41"
+dependencies = [
+ "memchr",
+]
+
+[[package]]
 name = "android-tzdata"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e999941b234f3131b00bc13c22d06e8c5ff726d1b6318ac7eb276997bbb4fef0"
 
 [[package]]
 name = "anes"
@@ -30,23 +39,23 @@
 name = "anstyle"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3a30da5c5f2d5e72842e00bcb57657162cdabef0931f40e2deb9b4140440cecd"
 
 [[package]]
 name = "anyhow"
-version = "1.0.71"
+version = "1.0.72"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9c7d0618f0e0b7e8ff11427422b64564d5fb0be1940354bfe2e0529b18a9d9b8"
+checksum = "3b13c32d80ecc7ab747b80c3784bce54ee8a7a0cc4fbda9bf4cda2cf6fe90854"
 
 [[package]]
 name = "arrow2"
-version = "0.17.2"
+version = "0.17.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "15ae0428d69ab31d7b2adad22a752d6f11fef2e901d2262d0cad4f5cb08b7093"
+checksum = "e44f27e89e3edd8738a07c5e2c881efaa25e69be97a816d2df051685d460670c"
 dependencies = [
  "ahash",
  "bytemuck",
  "chrono",
  "dyn-clone",
  "either",
  "ethnum",
@@ -79,15 +88,15 @@
  "peeking_take_while",
  "prettyplease",
  "proc-macro2",
  "quote",
  "regex",
  "rustc-hash",
  "shlex",
- "syn 2.0.23",
+ "syn 2.0.26",
  "which",
 ]
 
 [[package]]
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -97,17 +106,17 @@
 name = "bitflags"
 version = "2.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "630be753d4e58660abd17930c71b647fe46c27ea6b63cc59e1e3851406972e42"
 
 [[package]]
 name = "bridgestan"
-version = "2.1.1"
+version = "2.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "40be108ab686fe2710a841b5e9473de9d5823c436200b9eb0b25e5a3a36afe90"
+checksum = "b1077a38022365223d0543a3d78666b8680d754542f340a26ab6c79952fa065c"
 dependencies = [
  "bindgen",
  "libloading 0.8.0",
  "thiserror",
 ]
 
 [[package]]
@@ -129,15 +138,15 @@
 name = "bytemuck_derive"
 version = "1.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fdde5c9cd29ebd706ce1b35600920a33550e402fc998a2e53ad3b42c3c47a192"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.23",
+ "syn 2.0.26",
 ]
 
 [[package]]
 name = "cast"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "37b2a672a2cb129a2e41c10b1224bb368f9f37a2b16b612598138befd7b37eb5"
@@ -209,26 +218,26 @@
  "glob",
  "libc",
  "libloading 0.7.4",
 ]
 
 [[package]]
 name = "clap"
-version = "4.3.10"
+version = "4.3.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "384e169cc618c613d5e3ca6404dda77a8685a63e08660dcc64abaf7da7cb0c7a"
+checksum = "5b0827b011f6f8ab38590295339817b0d26f344aa4932c3ced71b45b0c54b4a9"
 dependencies = [
  "clap_builder",
 ]
 
 [[package]]
 name = "clap_builder"
-version = "4.3.10"
+version = "4.3.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ef137bbe35aab78bdb468ccfba75a5f4d8321ae011d34063770780545176af2d"
+checksum = "9441b403be87be858db6a23edb493e7f694761acdc3343d5a0fcaafd304cbc9e"
 dependencies = [
  "anstyle",
  "clap_lex",
 ]
 
 [[package]]
 name = "clap_lex"
@@ -337,17 +346,17 @@
 checksum = "5a22b2d63d4d1dc0b7f1b6b2747dd0088008a9be28b6ddf0b1e7d335e3037294"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
 name = "dyn-clone"
-version = "1.0.11"
+version = "1.0.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "68b0cf012f1230e43cd00ebb729c6bb58707ecfa8ad08b52ef3a4ccd2697fc30"
+checksum = "304e6508efa593091e97a9abbc10f90aa7ca635b6d2784feff3c89d41dd12272"
 
 [[package]]
 name = "either"
 version = "1.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7fcaabb2fef8c910e7f4c7ce9f67a1283a1715879a7c230ca9d6d1ae31f16d91"
 
@@ -413,29 +422,29 @@
 name = "hash_hasher"
 version = "2.0.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "74721d007512d0cb3338cd20f0654ac913920061a4c4d0d8708edb3f2a698c0c"
 
 [[package]]
 name = "hermit-abi"
-version = "0.3.1"
+version = "0.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fed44880c466736ef9a5c5b5facefb5ed0785676d0c02d612db14e54f0d84286"
+checksum = "443144c8cdadd93ebf52ddb4056d257f5b52c04d3c804e657d19eb73fc33668b"
 
 [[package]]
 name = "indoc"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
 name = "is-terminal"
-version = "0.4.8"
+version = "0.4.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "24fddda5af7e54bf7da53067d6e802dbcc381d0a8eef629df528e3ebf68755cb"
+checksum = "cb0889898416213fab133e1d33a0e5858a48177452750691bde3666d0fdbaf8b"
 dependencies = [
  "hermit-abi",
  "rustix",
  "windows-sys",
 ]
 
 [[package]]
@@ -454,17 +463,17 @@
 checksum = "b1c173a5686ce8bfa551b3563d0c2170bf24ca44da99c7ca4bfdab5418c3fe57"
 dependencies = [
  "either",
 ]
 
 [[package]]
 name = "itoa"
-version = "1.0.7"
+version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c0aa48fab2893d8a49caa94082ae8488f4e1050d73b367881dcd2198f4199fd8"
+checksum = "af150ab688ff2122fcef229be89cb50dd66af9e01a4ff320cc137eecc9bacc38"
 
 [[package]]
 name = "js-sys"
 version = "0.3.64"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c5f195fe497f702db0f318b07fdd68edb16955aed830df8363d837542f8f935a"
 dependencies = [
@@ -630,17 +639,17 @@
 dependencies = [
  "autocfg",
  "num-traits",
 ]
 
 [[package]]
 name = "num-traits"
-version = "0.2.15"
+version = "0.2.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "578ede34cf02f8924ab9447f50c28075b4d3e5b269972345e7e0372b38c6cdcd"
+checksum = "f30b0abd723be7e2ffca1272140fac1a2f084c77ec3e123c192b66af1ee9e6c2"
 dependencies = [
  "autocfg",
  "libm",
 ]
 
 [[package]]
 name = "num_cpus"
@@ -665,15 +674,15 @@
  "num-traits",
  "pyo3",
  "rustc-hash",
 ]
 
 [[package]]
 name = "nutpie"
-version = "0.6.0"
+version = "0.7.0"
 dependencies = [
  "anyhow",
  "arrow2",
  "bridgestan",
  "criterion",
  "itertools 0.11.0",
  "ndarray",
@@ -684,17 +693,17 @@
  "rand_chacha",
  "rayon",
  "thiserror",
 ]
 
 [[package]]
 name = "nuts-rs"
-version = "0.5.1"
+version = "0.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "aa23fb9109210d6afebc5b9f4c06827c2d6985838a911b8ff75cd4f75aa7c79f"
+checksum = "d85453ab1ad7a07a4a6963b00e84b258113d4e8d2c79d6ec306418d05be7eaa5"
 dependencies = [
  "anyhow",
  "arrow2",
  "crossbeam",
  "itertools 0.11.0",
  "multiversion",
  "rand",
@@ -777,27 +786,27 @@
 name = "ppv-lite86"
 version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
 
 [[package]]
 name = "prettyplease"
-version = "0.2.9"
+version = "0.2.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9825a04601d60621feed79c4e6b56d65db77cdca55cef43b46b0de1096d1c282"
+checksum = "aea97f0167426c9ca51bc27fcf5ba6130b36012263316a1db75e5f38daf0d1e5"
 dependencies = [
  "proc-macro2",
- "syn 2.0.23",
+ "syn 2.0.26",
 ]
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.63"
+version = "1.0.66"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7b368fba921b0dce7e60f5e04ec15e565b3303972b42bcfde1d0713b881959eb"
+checksum = "18fb31db3f9bddb2ea821cde30a9f70117e3f119938b5ee630b7403aa6e2ead9"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
 version = "0.19.1"
@@ -857,17 +866,17 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.29"
+version = "1.0.31"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "573015e8ab27661678357f27dc26460738fd2b6c86e46f386fde94cb5d913105"
+checksum = "5fe8a65d69dd0808184ebb5f836ab526bb259db23c657efa38711b1072ee47f0"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "rand"
 version = "0.8.5"
@@ -943,26 +952,40 @@
 checksum = "567664f262709473930a4bf9e51bf2ebf3348f2e748ccc50dea20646858f8f29"
 dependencies = [
  "bitflags 1.3.2",
 ]
 
 [[package]]
 name = "regex"
-version = "1.8.4"
+version = "1.9.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b2eae68fc220f7cf2532e4494aded17545fce192d59cd996e0fe7887f4ceb575"
+dependencies = [
+ "aho-corasick",
+ "memchr",
+ "regex-automata",
+ "regex-syntax",
+]
+
+[[package]]
+name = "regex-automata"
+version = "0.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d0ab3ca65655bb1e41f2a8c8cd662eb4fb035e67c3f78da1d61dffe89d07300f"
+checksum = "39354c10dd07468c2e73926b23bb9c2caca74c5501e38a35da70406f1d923310"
 dependencies = [
+ "aho-corasick",
+ "memchr",
  "regex-syntax",
 ]
 
 [[package]]
 name = "regex-syntax"
-version = "0.7.2"
+version = "0.7.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "436b050e76ed2903236f032a59761c1eb99e1b0aead2c257922771dab1fc8c78"
+checksum = "e5ea92a5b6195c6ef2a0295ea818b312502c6fc94dde986c5553242e18fd4ce2"
 
 [[package]]
 name = "rustc-hash"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "08d43f7aa6b08d49f382cde6a7982047c3426db949b1424bc4b7ec9ae12c6ce2"
 
@@ -973,77 +996,77 @@
 checksum = "bfa0f585226d2e68097d4f95d113b15b83a82e819ab25717ec0590d9584ef366"
 dependencies = [
  "semver",
 ]
 
 [[package]]
 name = "rustix"
-version = "0.38.2"
+version = "0.38.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "aabcb0461ebd01d6b79945797c27f8529082226cb630a9865a71870ff63532a4"
+checksum = "0a962918ea88d644592894bc6dc55acc6c0956488adcebbfb6e273506b7fd6e5"
 dependencies = [
  "bitflags 2.3.3",
  "errno",
  "libc",
  "linux-raw-sys",
  "windows-sys",
 ]
 
 [[package]]
 name = "ryu"
-version = "1.0.13"
+version = "1.0.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f91339c0467de62360649f8d3e185ca8de4224ff281f66000de5eb2a77a79041"
+checksum = "1ad4cc8da4ef723ed60bced201181d83791ad433213d8c24efffda1eec85d741"
 
 [[package]]
 name = "same-file"
 version = "1.0.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "93fc1dc3aaa9bfed95e02e6eadabb4baf7e3078b0bd1b4d7b6b0b68378900502"
 dependencies = [
  "winapi-util",
 ]
 
 [[package]]
 name = "scopeguard"
-version = "1.1.0"
+version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
+checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
 
 [[package]]
 name = "semver"
-version = "1.0.17"
+version = "1.0.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bebd363326d05ec3e2f532ab7660680f3b02130d780c299bca73469d521bc0ed"
+checksum = "b0293b4b29daaf487284529cc2f5675b8e57c61f70167ba415a463651fd6a918"
 
 [[package]]
 name = "serde"
-version = "1.0.165"
+version = "1.0.173"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c939f902bb7d0ccc5bce4f03297e161543c2dcb30914faf032c2bd0b7a0d48fc"
+checksum = "e91f70896d6720bc714a4a57d22fc91f1db634680e65c8efe13323f1fa38d53f"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.165"
+version = "1.0.173"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6eaae920e25fffe4019b75ff65e7660e72091e59dd204cb5849bbd6a3fd343d7"
+checksum = "a6250dde8342e0232232be9ca3db7aa40aceb5a3e5dd9bddbc00d99a007cde49"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.23",
+ "syn 2.0.26",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.99"
+version = "1.0.103"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "46266871c240a00b8f503b877622fe33430b3c7d963bdc0f2adc511e54a1eae3"
+checksum = "d03b412469450d4404fe8499a268edd7f8b79fecb074b0d812ad64ca21f4031b"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
@@ -1056,87 +1079,87 @@
 name = "simdutf8"
 version = "0.1.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f27f6278552951f1f2b8cf9da965d10969b2efdea95a6ec47987ab46edfe263a"
 
 [[package]]
 name = "smallvec"
-version = "1.10.0"
+version = "1.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a507befe795404456341dfab10cef66ead4c041f62b8b11bbb92bffe5d0953e0"
+checksum = "62bb4feee49fdd9f707ef802e22365a35de4b7b299de4763d44bfea899442ff9"
 
 [[package]]
 name = "syn"
 version = "1.0.109"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "72b64191b275b66ffe2469e8af2c1cfe3bafa67b529ead792a6d0160888b4237"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.23"
+version = "2.0.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "59fb7d6d8281a51045d62b8eb3a7d1ce347b76f312af50cd3dc0af39c87c1737"
+checksum = "45c3457aacde3c65315de5031ec191ce46604304d2446e803d71ade03308d970"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "target-features"
 version = "0.1.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "06f6b473c37f9add4cf1df5b4d66a8ef58ab6c895f1a3b3f949cf3e21230140e"
 
 [[package]]
 name = "target-lexicon"
-version = "0.12.8"
+version = "0.12.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1b1c7f239eb94671427157bd93b3694320f3668d4e1eff08c7285366fd777fac"
+checksum = "1d2faeef5759ab89935255b1a4cd98e0baf99d1085e37d36599c625dac49ae8e"
 
 [[package]]
 name = "thiserror"
-version = "1.0.40"
+version = "1.0.43"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "978c9a314bd8dc99be594bc3c175faaa9794be04a5a5e153caba6915336cebac"
+checksum = "a35fc5b8971143ca348fa6df4f024d4d55264f3468c71ad1c2f365b0a4d58c42"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.40"
+version = "1.0.43"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f9456a42c5b0d803c8cd86e73dd7cc9edd429499f37a3550d286d5e86720569f"
+checksum = "463fe12d7993d3b327787537ce8dd4dfa058de32fc2b195ef3cde03dc4771e8f"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.23",
+ "syn 2.0.26",
 ]
 
 [[package]]
 name = "tinytemplate"
 version = "1.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "be4d6b5f19ff7664e8c98d03e2139cb510db9b0a60b55f8e8709b689d939b6bc"
 dependencies = [
  "serde",
  "serde_json",
 ]
 
 [[package]]
 name = "unicode-ident"
-version = "1.0.9"
+version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b15811caf2415fb889178633e7724bad2509101cde276048e013b9def5e51fa0"
+checksum = "301abaae475aa91687eb82514b328ab47a211a533026cb25fc3e519b86adfc3c"
 
 [[package]]
 name = "unindent"
 version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
 
@@ -1179,15 +1202,15 @@
 checksum = "5ef2b6d3c510e9625e5fe6f509ab07d66a760f0885d858736483c32ed7809abd"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 2.0.23",
+ "syn 2.0.26",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro"
 version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -1201,15 +1224,15 @@
 name = "wasm-bindgen-macro-support"
 version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "54681b18a46765f095758388f2d0cf16eb8d4169b639ab575a8f5693af210c7b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.23",
+ "syn 2.0.26",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
 version = "0.2.87"
```

### Comparing `nutpie-0.6.0/PKG-INFO` & `nutpie-0.7.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: nutpie
-Version: 0.6.0
+Version: 0.7.0
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: pyarrow >=12.0.0
 Requires-Dist: pandas >=2.0
 Requires-Dist: xarray >=2023.6.0
 Requires-Dist: arviz >=0.15.0
 Requires-Dist: fastprogress >=1.0.3
-Requires-Dist: bridgestan ==2.1.1 ; extra == 'stan'
+Requires-Dist: bridgestan >=2.1.2 ; extra == 'stan'
 Requires-Dist: pymc >=5.5.0 ; extra == 'pymc'
 Requires-Dist: numba >=0.57.1 ; extra == 'pymc'
-Requires-Dist: bridgestan ==2.1.1 ; extra == 'all'
+Requires-Dist: bridgestan >=2.1.2 ; extra == 'all'
 Requires-Dist: pymc >=5.5.0 ; extra == 'all'
 Requires-Dist: numba >=0.57.1 ; extra == 'all'
 Provides-Extra: stan
 Provides-Extra: pymc
 Provides-Extra: all
 License-File: LICENSE
 Summary: Sample Stan or PyMC models
```

