# Comparing `tmp/funi-0.0.0.tar.gz` & `tmp/funi-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funi-0.0.0.tar", last modified: Mon Jun 26 21:36:23 2023, max compression
+gzip compressed data, was "funi-0.0.1.tar", last modified: Fri Jul 21 15:30:13 2023, max compression
```

## Comparing `funi-0.0.0.tar` & `funi-0.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:36:23.440440 funi-0.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-26 21:36:12.000000 funi-0.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-06-26 21:36:23.440440 funi-0.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-06-26 21:36:12.000000 funi-0.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:36:23.440440 funi-0.0.0/funi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-06-26 21:36:23.000000 funi-0.0.0/funi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-26 21:36:23.000000 funi-0.0.0/funi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 21:36:23.000000 funi-0.0.0/funi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 21:36:23.000000 funi-0.0.0/funi.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-26 21:36:23.000000 funi-0.0.0/funi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-26 21:36:23.000000 funi-0.0.0/funi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-26 21:36:12.000000 funi-0.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 21:36:23.440440 funi-0.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-06-26 21:36:12.000000 funi-0.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:36:23.440440 funi-0.0.0/src/
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-26 21:36:12.000000 funi-0.0.0/src/pyfuni.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:36:23.440440 funi-0.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-06-26 21:36:12.000000 funi-0.0.0/tests/test_funi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:30:13.364379 funi-0.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-21 15:30:05.000000 funi-0.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-07-21 15:30:13.364379 funi-0.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-21 15:30:05.000000 funi-0.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:30:13.364379 funi-0.0.1/funi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-07-21 15:30:13.000000 funi-0.0.1/funi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-21 15:30:13.000000 funi-0.0.1/funi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 15:30:13.000000 funi-0.0.1/funi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 15:30:13.000000 funi-0.0.1/funi.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-21 15:30:13.000000 funi-0.0.1/funi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-21 15:30:13.000000 funi-0.0.1/funi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-21 15:30:05.000000 funi-0.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 15:30:13.364379 funi-0.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-07-21 15:30:05.000000 funi-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:30:13.364379 funi-0.0.1/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-21 15:30:05.000000 funi-0.0.1/src/pyfuni.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:30:13.364379 funi-0.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-07-21 15:30:05.000000 funi-0.0.1/tests/test_funi.py
```

### Comparing `funi-0.0.0/LICENSE` & `funi-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `funi-0.0.0/PKG-INFO` & `funi-0.0.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funi
-Version: 0.0.0
+Version: 0.0.1
 Summary: Find unique float arrays
 Home-page: https://github.com/tataratat/funi
 Author: Jaewook Lee
 Author-email: jaewooklee042@gmail.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
@@ -19,16 +19,19 @@
 Classifier: Topic :: Scientific/Engineering
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # funi
 Find UNIque float array rows.
 [numpy.unique](https://numpy.org/doc/stable/reference/generated/numpy.unique.html) is an awesome function that alleviates headaches, fast.
-Haven you wished that it'd be applicable for 2D float arrays?
+Haven't you wished that it'd be applicable for 2D float arrays?
 `funi` is here to help!
+There are two available methods: `axis` and `lexicographic`.
+`axis` will first project each array to an axis to sort, where as
+`lexicographic` sorts given array in lexicographical manner.
 
 ## Install
 ```bash
 pip install funi
 ```
 
 ## Quick Start
@@ -37,26 +40,20 @@
 import numpy as np
 
 # create a random array with duplicating entries
 arr = np.random.random((10000, 3))
 arr = np.vstack((arr, arr, arr))
 np.random.shuffle(arr)
 
-# specify tolerance and
-# tolerance is used to compare entries in column-wise.
-# consider it as bounding-box edge length for duplicate identification
-# with stable_sort + sorted_index unique_id will start from 0
+# specify tolerance and if you want your unique ids to be stable sorted.
 unique_data, unique_ids, inverse = funi.unique_rows(
     arr,
     tolerance=1e-11,
-    return_unique=True,
-    return_index=True,
     sorted_index=True,
-    return_inverse=True,
-    stable_sort=True,
+    method="axis",
 )
 
 # use ids to extract unique_data from the original array
 assert np.allclose(unique_data, arr[unique_ids])
 
 # use inverse to map unique_data back to the original array
 assert np.allclose(arr, unique_data[inverse])
```

### Comparing `funi-0.0.0/README.md` & `funi-0.0.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 # funi
 Find UNIque float array rows.
 [numpy.unique](https://numpy.org/doc/stable/reference/generated/numpy.unique.html) is an awesome function that alleviates headaches, fast.
-Haven you wished that it'd be applicable for 2D float arrays?
+Haven't you wished that it'd be applicable for 2D float arrays?
 `funi` is here to help!
+There are two available methods: `axis` and `lexicographic`.
+`axis` will first project each array to an axis to sort, where as
+`lexicographic` sorts given array in lexicographical manner.
 
 ## Install
 ```bash
 pip install funi
 ```
 
 ## Quick Start
@@ -15,26 +18,20 @@
 import numpy as np
 
 # create a random array with duplicating entries
 arr = np.random.random((10000, 3))
 arr = np.vstack((arr, arr, arr))
 np.random.shuffle(arr)
 
-# specify tolerance and
-# tolerance is used to compare entries in column-wise.
-# consider it as bounding-box edge length for duplicate identification
-# with stable_sort + sorted_index unique_id will start from 0
+# specify tolerance and if you want your unique ids to be stable sorted.
 unique_data, unique_ids, inverse = funi.unique_rows(
     arr,
     tolerance=1e-11,
-    return_unique=True,
-    return_index=True,
     sorted_index=True,
-    return_inverse=True,
-    stable_sort=True,
+    method="axis",
 )
 
 # use ids to extract unique_data from the original array
 assert np.allclose(unique_data, arr[unique_ids])
 
 # use inverse to map unique_data back to the original array
 assert np.allclose(arr, unique_data[inverse])
```

### Comparing `funi-0.0.0/funi.egg-info/PKG-INFO` & `funi-0.0.1/funi.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funi
-Version: 0.0.0
+Version: 0.0.1
 Summary: Find unique float arrays
 Home-page: https://github.com/tataratat/funi
 Author: Jaewook Lee
 Author-email: jaewooklee042@gmail.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
@@ -19,16 +19,19 @@
 Classifier: Topic :: Scientific/Engineering
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # funi
 Find UNIque float array rows.
 [numpy.unique](https://numpy.org/doc/stable/reference/generated/numpy.unique.html) is an awesome function that alleviates headaches, fast.
-Haven you wished that it'd be applicable for 2D float arrays?
+Haven't you wished that it'd be applicable for 2D float arrays?
 `funi` is here to help!
+There are two available methods: `axis` and `lexicographic`.
+`axis` will first project each array to an axis to sort, where as
+`lexicographic` sorts given array in lexicographical manner.
 
 ## Install
 ```bash
 pip install funi
 ```
 
 ## Quick Start
@@ -37,26 +40,20 @@
 import numpy as np
 
 # create a random array with duplicating entries
 arr = np.random.random((10000, 3))
 arr = np.vstack((arr, arr, arr))
 np.random.shuffle(arr)
 
-# specify tolerance and
-# tolerance is used to compare entries in column-wise.
-# consider it as bounding-box edge length for duplicate identification
-# with stable_sort + sorted_index unique_id will start from 0
+# specify tolerance and if you want your unique ids to be stable sorted.
 unique_data, unique_ids, inverse = funi.unique_rows(
     arr,
     tolerance=1e-11,
-    return_unique=True,
-    return_index=True,
     sorted_index=True,
-    return_inverse=True,
-    stable_sort=True,
+    method="axis",
 )
 
 # use ids to extract unique_data from the original array
 assert np.allclose(unique_data, arr[unique_ids])
 
 # use inverse to map unique_data back to the original array
 assert np.allclose(arr, unique_data[inverse])
```

### Comparing `funi-0.0.0/setup.py` & `funi-0.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from pybind11.setup_helpers import Pybind11Extension, build_ext
 from setuptools import setup
 
 with open("README.md") as f:
     readme = f.read()
 
-__version__ = "0.0.0"
+__version__ = "0.0.1"
 
 ext_modules = [
     Pybind11Extension(
         "funi",
         ["src/pyfuni.cpp"],
         include_dirs=["src"],
         extra_compile_args=["-O3"],
```

### Comparing `funi-0.0.0/tests/test_funi.py` & `funi-0.0.1/tests/test_funi.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,69 +12,46 @@
         self.q = np.vstack((q, q, q))
         np.random.shuffle(self.q)
 
     def test_all_return(self):
         tol = 1e-10
 
         # sorted indices
-        unique_s, ids_s, inv_s = funi.unique_float64(
-            self.q, tol, True, True, True, True, True
-        )
+        unique_s, ids_s, inv_s = funi.unique_rows(self.q, tol, True, "l")
 
         # mapping check
         assert np.allclose(self.q[ids_s], unique_s)
         assert np.allclose(self.q, unique_s[inv_s])
 
         # sortedness check
         assert ~np.all(np.diff(ids_s) < 0)
 
         # not sorted
         # sorted indices
-        unique_ns, ids_ns, inv_ns = funi.unique_float64(
-            self.q, tol, True, True, False, True, True
-        )
+        unique_ns, ids_ns, inv_ns = funi.unique_rows(self.q, tol, False, "l")
 
         # mapping check
         assert np.allclose(self.q[ids_ns], unique_ns)
         assert np.allclose(self.q, unique_ns[inv_ns])
 
-        # no unique return - sorted
-        unique, ids, inv = funi.unique_float64(
-            self.q, tol, False, True, True, True, True
-        )
-
-        assert unique.size == 0
-        assert np.allclose(self.q, self.q[ids][inv])
-        assert np.allclose(ids, ids_s)
-        assert np.allclose(inv, inv_s)
-
-        # no unique return - not sorted
-        unique, ids, inv = funi.unique_float64(
-            self.q, tol, False, True, False, True, True
-        )
-
-        assert unique.size == 0
-        assert np.allclose(self.q, self.q[ids][inv])
-        assert np.allclose(ids, ids_ns)
-        assert np.allclose(inv, inv_ns)
-
-        # no inverse - sorted
-        unique, ids, inv = funi.unique_float64(
-            self.q, tol, True, True, True, False, True
-        )
-
-        assert inv.size == 0
-        assert np.allclose(unique, self.q[ids])
-        assert np.allclose(ids, ids_s)
-
-        # no invese - not sorted
-        unique, ids, inv = funi.unique_float64(
-            self.q, tol, True, True, False, False, True
-        )
-
-        assert inv.size == 0
-        assert np.allclose(unique, self.q[ids])
-        assert np.allclose(ids, ids_ns)
+        # now for axis based
+        # sorted indices
+        unique_s, ids_s, inv_s = funi.unique_rows(self.q, tol, True, "a")
+
+        # mapping check
+        assert np.allclose(self.q[ids_s], unique_s)
+        assert np.allclose(self.q, unique_s[inv_s])
+
+        # sortedness check
+        assert ~np.all(np.diff(ids_s) < 0)
+
+        # not sorted
+        # sorted indices
+        unique_ns, ids_ns, inv_ns = funi.unique_rows(self.q, tol, False, "a")
+
+        # mapping check
+        assert np.allclose(self.q[ids_ns], unique_ns)
+        assert np.allclose(self.q, unique_ns[inv_ns])
 
 
 if __name__ == "__main__":
     unittest.main()
```

