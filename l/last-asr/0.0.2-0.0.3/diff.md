# Comparing `tmp/last-asr-0.0.2.tar.gz` & `tmp/last_asr-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "last-asr-0.0.2.tar", last modified: Fri Apr  7 22:45:35 2023, max compression
+gzip compressed data, was "last_asr-0.0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `last-asr-0.0.2.tar` & `last_asr-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0    11357 2023-04-07 22:44:59.937729 last-asr-0.0.2/LICENSE
--rw-r--r--   0        0        0      682 2023-04-07 22:44:59.937729 last-asr-0.0.2/README.md
--rw-r--r--   0        0        0      514 2023-04-07 22:44:59.937729 last-asr-0.0.2/last/.readthedocs.yaml
--rw-r--r--   0        0        0      850 2023-04-07 22:44:59.937729 last-asr-0.0.2/last/__init__.py
--rw-r--r--   0        0        0    18488 2023-04-07 22:44:59.937729 last-asr-0.0.2/last/alignments.py
--rw-r--r--   0        0        0    12216 2023-04-07 22:44:59.937729 last-asr-0.0.2/last/contexts.py
--rw-r--r--   0        0        0    34907 2023-04-07 22:44:59.937729 last-asr-0.0.2/last/lattices.py
--rw-r--r--   0        0        0     4872 2023-04-07 22:44:59.937729 last-asr-0.0.2/last/scatter_reduce.py
--rw-r--r--   0        0        0    15206 2023-04-07 22:44:59.941729 last-asr-0.0.2/last/semirings.py
--rw-r--r--   0        0        0    11569 2023-04-07 22:44:59.941729 last-asr-0.0.2/last/weight_fns.py
--rw-r--r--   0        0        0     1230 2023-04-07 22:44:59.941729 last-asr-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1632 1970-01-01 00:00:00.000000 last-asr-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-21 14:22:47.480223 last_asr-0.0.3/LICENSE
+-rw-r--r--   0        0        0      682 2023-07-21 14:22:47.480223 last_asr-0.0.3/README.md
+-rw-r--r--   0        0        0      850 2023-07-21 14:22:47.480223 last_asr-0.0.3/last/__init__.py
+-rw-r--r--   0        0        0    18488 2023-07-21 14:22:47.480223 last_asr-0.0.3/last/alignments.py
+-rw-r--r--   0        0        0    12216 2023-07-21 14:22:47.480223 last_asr-0.0.3/last/contexts.py
+-rw-r--r--   0        0        0    34907 2023-07-21 14:22:47.480223 last_asr-0.0.3/last/lattices.py
+-rw-r--r--   0        0        0     4872 2023-07-21 14:22:47.480223 last_asr-0.0.3/last/scatter_reduce.py
+-rw-r--r--   0        0        0    15803 2023-07-21 14:22:47.480223 last_asr-0.0.3/last/semirings.py
+-rw-r--r--   0        0        0    11683 2023-07-21 14:22:47.480223 last_asr-0.0.3/last/weight_fns.py
+-rw-r--r--   0        0        0     1230 2023-07-21 14:22:47.480223 last_asr-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1632 1970-01-01 00:00:00.000000 last_asr-0.0.3/PKG-INFO
```

### Comparing `last-asr-0.0.2/LICENSE` & `last_asr-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `last-asr-0.0.2/README.md` & `last_asr-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `last-asr-0.0.2/last/__init__.py` & `last_asr-0.0.3/last/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,8 +17,8 @@
 from last import alignments
 from last import contexts
 from last import semirings
 from last import weight_fns
 from last.lattices import RecognitionLattice
 
 # A new PyPI release will be pushed everytime `__version__` is increased.
-__version__ = '0.0.2'
+__version__ = '0.0.3'
```

### Comparing `last-asr-0.0.2/last/alignments.py` & `last_asr-0.0.3/last/alignments.py`

 * *Files identical despite different names*

### Comparing `last-asr-0.0.2/last/contexts.py` & `last_asr-0.0.3/last/contexts.py`

 * *Files identical despite different names*

### Comparing `last-asr-0.0.2/last/lattices.py` & `last_asr-0.0.3/last/lattices.py`

 * *Files identical despite different names*

### Comparing `last-asr-0.0.2/last/scatter_reduce.py` & `last_asr-0.0.3/last/scatter_reduce.py`

 * *Files identical despite different names*

### Comparing `last-asr-0.0.2/last/semirings.py` & `last_asr-0.0.3/last/semirings.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,18 +91,26 @@
   of identically shaped ndarrays, with possibly different dtypes. The shape
   and dtypes of a semiring value can be obtained with methods
   `last.semirings.value_shape()` and `last.semirings.value_dtype()`.
 
   Semiring is not an abstract base class because we allow operations to be
   unimplemented (e.g. `prod`, is not commonly used).
 
-  Note: Reductions (prod & sum) can be tricky to implement correctly, here are
-  two important things to watch out for:
-  *   `axis` can be in the range [-rank, rank).
-  *   The input can have 0-sized dimensions.
+  Implementation tips:
+  *   Binary operations (times & plus) should support broadcasting. If a binary
+      operation requires a custom vjp implementation, it may not be straight-
+      forward to write one that handles input broadcasting properly. Instead,
+      write a custom vjp function that requires inputs with identical shapes,
+      then use `jnp.broadcast_arrays()` to preprocess the operands in the
+      implementation of the semiring operations. See `{_Log,_MaxTropical}.plus`
+      for examples.
+  *   Reductions (prod & sum) can be tricky to implement correctly, here are
+      two important things to watch out for:
+      *   `axis` can be in the range [-rank, rank).
+      *   The input can have 0-sized dimensions.
   """
 
   def zeros(self, shape: Sequence[int], dtype: Optional[DType] = None) -> T:
     """Semiring zeros in the given shape and dtype.
 
     Args:
       shape: Desired output shape.
@@ -202,14 +210,15 @@
 
   @staticmethod
   def times(a: jnp.ndarray, b: jnp.ndarray) -> jnp.ndarray:
     return a + b
 
   @staticmethod
   def plus(a: jnp.ndarray, b: jnp.ndarray) -> jnp.ndarray:
+    a, b = jnp.broadcast_arrays(a, b)
     return _logaddexp(a, b)
 
   @staticmethod
   def prod(a: jnp.ndarray, axis: int) -> jnp.ndarray:
     return jnp.sum(a, axis=axis)
 
   @classmethod
@@ -323,14 +332,15 @@
 
   @staticmethod
   def times(a: jnp.ndarray, b: jnp.ndarray) -> jnp.ndarray:
     return a + b
 
   @staticmethod
   def plus(a: jnp.ndarray, b: jnp.ndarray) -> jnp.ndarray:
+    a, b = jnp.broadcast_arrays(a, b)
     return _maximum(a, b)
 
   @staticmethod
   def prod(a: jnp.ndarray, axis: int) -> jnp.ndarray:
     return jnp.sum(a, axis=axis)
 
   @classmethod
```

### Comparing `last-asr-0.0.2/last/weight_fns.py` & `last_asr-0.0.3/last/weight_fns.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 """Weight functions."""
 
 import abc
 from typing import Callable, Generic, Optional, TypeVar
 
 import einops
 from flax import linen as nn
-import flax.struct
 import jax
 import jax.numpy as jnp
 
 # Weight functions are the only components in GNAT with trainable parameters. We
 # implement weight functions in two parts: WeightFn and WeightFnCacher.
 #
 # A WeightFn is a neural network that computes the arc weights for a given
@@ -237,37 +236,45 @@
   embedding table can be used with JointWeightFn.
   """
   vocab_size: int
   context_size: int
   rnn_size: int
   rnn_embedding_size: int
   # TODO(wuke): Use LSTM with layer norm.
-  rnn_cell: nn.recurrent.RNNCellBase = flax.struct.field(
-      default_factory=nn.OptimizedLSTMCell)
+  rnn_cell: Optional[nn.RNNCellBase] = None
 
   @nn.compact
   def __call__(self) -> jnp.ndarray:
+    if self.rnn_cell is None:
+      rnn_cell = nn.OptimizedLSTMCell(self.rnn_size, name='rnn_cell')
+    else:
+      rnn_cell = self.rnn_cell
 
     def tile_rnn_state(state):
       return einops.repeat(state, 'n ... -> (n v) ...', v=self.vocab_size)
 
     # Label 0 is an extra label for seeding the start state.
     # Labels [1, vocab_size] are the actual lexical labels.
     embed = nn.Embed(self.vocab_size + 1, self.rnn_embedding_size)
     # TODO(wuke): Proper rng handling.
     dummy_rng = jax.random.PRNGKey(0)
-    rnn_states, start_embedding = self.rnn_cell(
-        self.rnn_cell.initialize_carry(dummy_rng, (1,), self.rnn_size),
-        embed(jnp.array([0])))
+    rnn_states, start_embedding = rnn_cell(
+        rnn_cell.initialize_carry(dummy_rng, (1, self.rnn_size)),
+        embed(jnp.array([0])),
+    )
     parts = [start_embedding]
-    inputs = embed(jnp.arange(1, self.vocab_size + 1))
-    for _ in range(self.context_size):
-      rnn_states, embeddings = self.rnn_cell(
-          jax.tree_util.tree_map(tile_rnn_state, rnn_states), inputs)
-      inputs = einops.repeat(inputs, 'n ... -> (v n) ...', v=self.vocab_size)
+    inputs = None
+    for i in range(self.context_size):
+      if i == 0:
+        inputs = embed(jnp.arange(1, self.vocab_size + 1))
+      else:
+        inputs = einops.repeat(inputs, 'n ... -> (v n) ...', v=self.vocab_size)
+      rnn_states, embeddings = rnn_cell(
+          jax.tree_util.tree_map(tile_rnn_state, rnn_states), inputs
+      )
       parts.append(embeddings)
     return jnp.concatenate(parts, axis=0)
 
 
 class NullCacher(WeightFnCacher[type(None)]):
   """A cacher that simply returns None.
```

### Comparing `last-asr-0.0.2/pyproject.toml` & `last_asr-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     "Intended Audience :: Science/Research",
 ]
 keywords = ["speech", "jax"]
 
 # pip dependencies of the project
 dependencies = [
   "einops>=0.5.0",
-  "flax>=0.6.1",
+  "flax>=0.7.0",
   "jax>=0.3.21",
 ]
 
 # This is set automatically by flit using `last.__version__`
 dynamic = ["version"]
 
 [project.urls]
```

### Comparing `last-asr-0.0.2/PKG-INFO` & `last_asr-0.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: last-asr
-Version: 0.0.2
+Version: 0.0.3
 Summary: The LAttice-based Speech Transducer (LAST) library
 Keywords: speech,jax
 Author: LAST authors
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Science/Research
 Requires-Dist: einops>=0.5.0
-Requires-Dist: flax>=0.6.1
+Requires-Dist: flax>=0.7.0
 Requires-Dist: jax>=0.3.21
 Requires-Dist: absl-py ; extra == "dev"
 Requires-Dist: numpy ; extra == "dev"
 Requires-Dist: optax ; extra == "dev"
 Requires-Dist: pytest ; extra == "dev"
 Requires-Dist: pytest-xdist ; extra == "dev"
 Requires-Dist: pylint>=2.6.0 ; extra == "dev"
```

