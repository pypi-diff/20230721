# Comparing `tmp/qibojit-0.0.8.tar.gz` & `tmp/qibojit-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qibojit-0.0.8.tar", last modified: Wed Mar 15 11:07:05 2023, max compression
+gzip compressed data, was "qibojit-0.0.9.tar", last modified: Wed Apr 26 19:48:04 2023, max compression
```

## Comparing `qibojit-0.0.8.tar` & `qibojit-0.0.9.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 11:07:05.733648 qibojit-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-15 11:07:01.000000 qibojit-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-03-15 11:07:05.733648 qibojit-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-03-15 11:07:01.000000 qibojit-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-03-15 11:07:01.000000 qibojit-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-15 11:07:05.733648 qibojit-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-03-15 11:07:01.000000 qibojit-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 11:07:05.729648 qibojit-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 11:07:05.729648 qibojit-0.0.8/src/qibojit/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-15 11:07:01.000000 qibojit-0.0.8/src/qibojit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 11:07:05.729648 qibojit-0.0.8/src/qibojit/backends/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-03-15 11:07:01.000000 qibojit-0.0.8/src/qibojit/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12068 2023-03-15 11:07:01.000000 qibojit-0.0.8/src/qibojit/backends/cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)    32248 2023-03-15 11:07:01.000000 qibojit-0.0.8/src/qibojit/backends/gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-03-15 11:07:01.000000 qibojit-0.0.8/src/qibojit/backends/matrices.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 11:07:05.729648 qibojit-0.0.8/src/qibojit/custom_operators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 11:07:01.000000 qibojit-0.0.8/src/qibojit/custom_operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19104 2023-03-15 11:07:01.000000 qibojit-0.0.8/src/qibojit/custom_operators/gates.py
--rw-r--r--   0 runner    (1001) docker     (123)     4922 2023-03-15 11:07:01.000000 qibojit-0.0.8/src/qibojit/custom_operators/ops.py
--rw-r--r--   0 runner    (1001) docker     (123)    15861 2023-03-15 11:07:01.000000 qibojit-0.0.8/src/qibojit/custom_operators/raw_kernels.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 11:07:05.733648 qibojit-0.0.8/src/qibojit/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 11:07:01.000000 qibojit-0.0.8/src/qibojit/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-03-15 11:07:01.000000 qibojit-0.0.8/src/qibojit/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-03-15 11:07:01.000000 qibojit-0.0.8/src/qibojit/tests/test_backends.py
--rw-r--r--   0 runner    (1001) docker     (123)    13187 2023-03-15 11:07:01.000000 qibojit-0.0.8/src/qibojit/tests/test_gates.py
--rw-r--r--   0 runner    (1001) docker     (123)     9077 2023-03-15 11:07:01.000000 qibojit-0.0.8/src/qibojit/tests/test_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-03-15 11:07:01.000000 qibojit-0.0.8/src/qibojit/tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 11:07:05.729648 qibojit-0.0.8/src/qibojit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-03-15 11:07:05.000000 qibojit-0.0.8/src/qibojit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-03-15 11:07:05.000000 qibojit-0.0.8/src/qibojit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-15 11:07:05.000000 qibojit-0.0.8/src/qibojit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-15 11:07:05.000000 qibojit-0.0.8/src/qibojit.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-03-15 11:07:05.000000 qibojit-0.0.8/src/qibojit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-15 11:07:05.000000 qibojit-0.0.8/src/qibojit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:48:04.576860 qibojit-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-26 19:47:58.000000 qibojit-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-04-26 19:48:04.576860 qibojit-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-04-26 19:47:58.000000 qibojit-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-26 19:47:58.000000 qibojit-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 19:48:04.576860 qibojit-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-04-26 19:47:58.000000 qibojit-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:48:04.572860 qibojit-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:48:04.572860 qibojit-0.0.9/src/qibojit/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-26 19:47:58.000000 qibojit-0.0.9/src/qibojit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:48:04.572860 qibojit-0.0.9/src/qibojit/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-26 19:47:58.000000 qibojit-0.0.9/src/qibojit/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12068 2023-04-26 19:47:58.000000 qibojit-0.0.9/src/qibojit/backends/cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32186 2023-04-26 19:47:58.000000 qibojit-0.0.9/src/qibojit/backends/gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-04-26 19:47:58.000000 qibojit-0.0.9/src/qibojit/backends/matrices.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:48:04.572860 qibojit-0.0.9/src/qibojit/custom_operators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 19:47:58.000000 qibojit-0.0.9/src/qibojit/custom_operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19104 2023-04-26 19:47:58.000000 qibojit-0.0.9/src/qibojit/custom_operators/gates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4922 2023-04-26 19:47:58.000000 qibojit-0.0.9/src/qibojit/custom_operators/ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15861 2023-04-26 19:47:58.000000 qibojit-0.0.9/src/qibojit/custom_operators/raw_kernels.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:48:04.576860 qibojit-0.0.9/src/qibojit/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 19:47:58.000000 qibojit-0.0.9/src/qibojit/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-04-26 19:47:58.000000 qibojit-0.0.9/src/qibojit/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-04-26 19:47:58.000000 qibojit-0.0.9/src/qibojit/tests/test_backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13187 2023-04-26 19:47:58.000000 qibojit-0.0.9/src/qibojit/tests/test_gates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9196 2023-04-26 19:47:58.000000 qibojit-0.0.9/src/qibojit/tests/test_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-26 19:47:58.000000 qibojit-0.0.9/src/qibojit/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:48:04.572860 qibojit-0.0.9/src/qibojit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-04-26 19:48:04.000000 qibojit-0.0.9/src/qibojit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-04-26 19:48:04.000000 qibojit-0.0.9/src/qibojit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 19:48:04.000000 qibojit-0.0.9/src/qibojit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 19:48:04.000000 qibojit-0.0.9/src/qibojit.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-26 19:48:04.000000 qibojit-0.0.9/src/qibojit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-26 19:48:04.000000 qibojit-0.0.9/src/qibojit.egg-info/top_level.txt
```

### Comparing `qibojit-0.0.8/LICENSE` & `qibojit-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `qibojit-0.0.8/PKG-INFO` & `qibojit-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qibojit
-Version: 0.0.8
+Version: 0.0.9
 Summary: Simulation tools based on numba and cupy.
 Home-page: https://github.com/qiboteam/qibojit
 Author: The Qibo team
 Author-email: 
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `qibojit-0.0.8/README.md` & `qibojit-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `qibojit-0.0.8/setup.py` & `qibojit-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     package_dir={"": "src"},
     package_data={"": ["*.cc"]},
     zip_safe=False,
     classifiers=[
         "Programming Language :: Python :: 3",
         "Topic :: Scientific/Engineering :: Physics",
     ],
-    install_requires=["numba>=0.51.0", "scipy", "psutil", "qibo>=0.1.11"],
+    install_requires=["numba>=0.51.0", "scipy", "psutil", "qibo>=0.1.13"],
     extras_require={
         "tests": ["pytest"],
     },
     python_requires=">=3.8.0",
     long_description=long_description,
     long_description_content_type="text/markdown",
 )
```

### Comparing `qibojit-0.0.8/src/qibojit/backends/cpu.py` & `qibojit-0.0.9/src/qibojit/backends/cpu.py`

 * *Files identical despite different names*

### Comparing `qibojit-0.0.8/src/qibojit/backends/gpu.py` & `qibojit-0.0.9/src/qibojit/backends/gpu.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,21 +152,20 @@
         n = 1 << nqubits
         kernel = self.gates.get(f"initial_state_kernel_{self.kernel_type}")
         state = self.cp.zeros(n * n, dtype=self.dtype)
         kernel((1,), (1,), [state])
         self.cp.cuda.stream.get_current_stream().synchronize()
         return state.reshape((n, n))
 
-    def identity_density_matrix(self, nqubits):
+    def identity_density_matrix(self, nqubits, normalize: bool = True):
         n = 1 << nqubits
-        kernel = self.gates.get(f"initial_state_kernel_{self.kernel_type}")
         state = self.cp.eye(n, dtype=self.dtype)
-        kernel((1,), (1,), [state])
         self.cp.cuda.stream.get_current_stream().synchronize()
-        state /= 2**nqubits
+        if normalize:
+            state /= 2**nqubits
         return state.reshape((n, n))
 
     def plus_state(self, nqubits):
         state = self.cp.ones(2**nqubits, dtype=self.dtype)
         state /= self.cp.sqrt(2**nqubits)
         return state
```

### Comparing `qibojit-0.0.8/src/qibojit/backends/matrices.py` & `qibojit-0.0.9/src/qibojit/backends/matrices.py`

 * *Files identical despite different names*

### Comparing `qibojit-0.0.8/src/qibojit/custom_operators/gates.py` & `qibojit-0.0.9/src/qibojit/custom_operators/gates.py`

 * *Files identical despite different names*

### Comparing `qibojit-0.0.8/src/qibojit/custom_operators/ops.py` & `qibojit-0.0.9/src/qibojit/custom_operators/ops.py`

 * *Files identical despite different names*

### Comparing `qibojit-0.0.8/src/qibojit/custom_operators/raw_kernels.py` & `qibojit-0.0.9/src/qibojit/custom_operators/raw_kernels.py`

 * *Files identical despite different names*

### Comparing `qibojit-0.0.8/src/qibojit/tests/conftest.py` & `qibojit-0.0.9/src/qibojit/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `qibojit-0.0.8/src/qibojit/tests/test_backends.py` & `qibojit-0.0.9/src/qibojit/tests/test_backends.py`

 * *Files identical despite different names*

### Comparing `qibojit-0.0.8/src/qibojit/tests/test_gates.py` & `qibojit-0.0.9/src/qibojit/tests/test_gates.py`

 * *Files identical despite different names*

### Comparing `qibojit-0.0.8/src/qibojit/tests/test_ops.py` & `qibojit-0.0.9/src/qibojit/tests/test_ops.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,18 +16,20 @@
         target_state = np.reshape(target_state, (16, 16))
     else:
         final_state = backend.zero_state(4)
         target_state = np.array([1] + [0] * 15, dtype=dtype)
     backend.assert_allclose(final_state, target_state)
 
 
-def test_identity_density_matrix(backend, dtype):
+@pytest.mark.parametrize("normalize", [False, True])
+def test_identity_density_matrix(backend, dtype, normalize):
     set_precision(dtype, backend)
-    final_state = backend.identity_density_matrix(4)
-    target_state = np.eye(16, 16, dtype=dtype) / 16
+    norm = 16 if normalize else 1.0
+    final_state = backend.identity_density_matrix(4, normalize=normalize)
+    target_state = np.eye(16, dtype=dtype) / norm
     backend.assert_allclose(final_state, target_state)
 
 
 @pytest.mark.parametrize("is_matrix", [False, True])
 def test_plus_state(backend, dtype, is_matrix):
     set_precision(dtype, backend)
     if is_matrix:
```

### Comparing `qibojit-0.0.8/src/qibojit/tests/utils.py` & `qibojit-0.0.9/src/qibojit/tests/utils.py`

 * *Files identical despite different names*

### Comparing `qibojit-0.0.8/src/qibojit.egg-info/PKG-INFO` & `qibojit-0.0.9/src/qibojit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qibojit
-Version: 0.0.8
+Version: 0.0.9
 Summary: Simulation tools based on numba and cupy.
 Home-page: https://github.com/qiboteam/qibojit
 Author: The Qibo team
 Author-email: 
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `qibojit-0.0.8/src/qibojit.egg-info/SOURCES.txt` & `qibojit-0.0.9/src/qibojit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

