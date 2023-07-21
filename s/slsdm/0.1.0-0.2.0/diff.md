# Comparing `tmp/slsdm-0.1.0.tar.gz` & `tmp/slsdm-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slsdm-0.1.0.tar", last modified: Tue Jul 18 20:21:20 2023, max compression
+gzip compressed data, was "slsdm-0.2.0.tar", last modified: Fri Jul 21 21:19:43 2023, max compression
```

## Comparing `slsdm-0.1.0.tar` & `slsdm-0.2.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 20:21:20.658925 slsdm-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-07-18 20:21:00.000000 slsdm-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-07-18 20:21:20.658925 slsdm-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-18 20:21:00.000000 slsdm-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-07-18 20:21:00.000000 slsdm-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-18 20:21:20.658925 slsdm-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    15042 2023-07-18 20:21:00.000000 slsdm-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 20:21:20.654924 slsdm-0.1.0/slsdm/
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-18 20:21:00.000000 slsdm-0.1.0/slsdm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-18 20:21:00.000000 slsdm-0.1.0/slsdm/_dist_metrics.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     8976 2023-07-18 20:21:00.000000 slsdm-0.1.0/slsdm/_generate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 20:21:20.654924 slsdm-0.1.0/slsdm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-07-18 20:21:20.000000 slsdm-0.1.0/slsdm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-18 20:21:20.000000 slsdm-0.1.0/slsdm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 20:21:20.000000 slsdm-0.1.0/slsdm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 20:21:19.000000 slsdm-0.1.0/slsdm.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-18 20:21:20.000000 slsdm-0.1.0/slsdm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-18 20:21:20.000000 slsdm-0.1.0/slsdm.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 20:21:20.658925 slsdm-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-07-18 20:21:00.000000 slsdm-0.1.0/tests/test_distancemetrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 21:19:43.609857 slsdm-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-07-21 21:19:18.000000 slsdm-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-07-21 21:19:43.609857 slsdm-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-07-21 21:19:18.000000 slsdm-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-07-21 21:19:18.000000 slsdm-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-21 21:19:43.613857 slsdm-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    15038 2023-07-21 21:19:18.000000 slsdm-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 21:19:43.609857 slsdm-0.2.0/slsdm/
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-21 21:19:18.000000 slsdm-0.2.0/slsdm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-07-21 21:19:18.000000 slsdm-0.2.0/slsdm/_dist_metrics.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     9101 2023-07-21 21:19:18.000000 slsdm-0.2.0/slsdm/_generate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 21:19:43.609857 slsdm-0.2.0/slsdm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-07-21 21:19:43.000000 slsdm-0.2.0/slsdm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-21 21:19:43.000000 slsdm-0.2.0/slsdm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 21:19:43.000000 slsdm-0.2.0/slsdm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 21:19:42.000000 slsdm-0.2.0/slsdm.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-21 21:19:43.000000 slsdm-0.2.0/slsdm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-21 21:19:43.000000 slsdm-0.2.0/slsdm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 21:19:43.609857 slsdm-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-07-21 21:19:18.000000 slsdm-0.2.0/tests/test_distancemetrics.py
```

### Comparing `slsdm-0.1.0/LICENSE` & `slsdm-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `slsdm-0.1.0/pyproject.toml` & `slsdm-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `slsdm-0.1.0/setup.cfg` & `slsdm-0.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `slsdm-0.1.0/setup.py` & `slsdm-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 MAINTAINER = "Meekail Zain"
 MAINTAINER_EMAIL = "zainmeekail@gmail.com"
 LICENSE = "new BSD"
 FEATURE_FLAGS = ""
 
 PYTEST_MIN_VERSION = "5.4.3"
 CYTHON_MIN_VERSION = "0.29.33"
-SKLEARN_MIN_VERSION = "1.3.dev0"
+SKLEARN_MIN_VERSION = "1.3.0"
 
 # TODO: Enable and trim as needed
 # 'build' and 'install' is included to have structured metadata for CI.
 # It will NOT be included in setup's extras_require
 # The values are (version_spec, comma separated tags)
 dependent_packages = {
     "scikit-learn": (SKLEARN_MIN_VERSION, "install"),
@@ -176,15 +176,15 @@
         shutil.rmtree(GENERATED_DIR)
 
     # TODO: Filter to only generate files that are either missing or have had
     # their corresponding *.def files altered.
     # Generate simd compilation targets from *.def files
 
     # TODO: Allow for more nuanced subset generation
-    target_arch = os.environ.get("SLSDM_SIMD_ARCH", "<=sse3")
+    target_arch = os.environ.get("SLSDM_SIMD_ARCH", "<=avx")
     global FEATURE_FLAGS
     FEATURE_FLAGS = generate_code(target_arch)
     srcs = ["_dist_metrics.pyx.tp", "_dist_metrics.pxd"]
     srcs += [
         "/".join(GENERATED_DIR.split("/")[1:]) + os.path.basename(p)
         for p in glob.glob(join(GENERATED_DIR, "*.cpp"))
     ]
```

### Comparing `slsdm-0.1.0/slsdm/__init__.py` & `slsdm-0.2.0/slsdm/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
         from ._dist_metrics import get_distance_metric
 
         return get_distance_metric(X, metric, **metric_kwargs)
     except ModuleNotFoundError:
         return None
 
 
-__version__ = "0.1.0"
+__version__ = "0.2.0"
 
 
 def get_best_arch():
     try:
         from ._dist_metrics import get_best_arch
 
         return get_best_arch()
```

### Comparing `slsdm-0.1.0/slsdm/_dist_metrics.pxd` & `slsdm-0.2.0/slsdm/_dist_metrics.pxd`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from sklearn.utils._typedefs cimport float64_t, float32_t, int32_t, intp_t
 
 cdef extern from "src/generated/_dist_optim.cpp":
-    cdef bint HAS_SIMD
     cdef Type xsimd_manhattan_dist[Type](Type * x, Type * y, intp_t size) nogil
     cdef Type xsimd_euclidean_rdist[Type](Type * x, Type * y, intp_t size) nogil
     cdef Type xsimd_seuclidean_rdist[Type](Type * x, Type * y, intp_t size, const Type * v) nogil
     cdef Type xsimd_chebyshev_dist[Type](Type * x, Type * y, intp_t size) nogil
     cdef Type xsimd_minkowski_rdist[Type](Type * x, Type * y, intp_t size, const double p) nogil
     cdef Type xsimd_minkowski_w_rdist[Type](Type * x, Type * y, intp_t size, const Type * w, const double p) nogil
```

### Comparing `slsdm-0.1.0/slsdm/_generate.py` & `slsdm-0.2.0/slsdm/_generate.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,90 +5,91 @@
 import io
 
 PY_TAB = "    "
 GENERATED_DIR = "slsdm/src/generated/"
 DEFINITIONS_DIR = "slsdm/definitions/"
 VECTOR_UNROLL_FACTOR = 4
 
-# XXX: Is there a nicer, more user-friendly approach towards
-# FMA{3, 4} instructions?
 # TODO: Add documentation regarding instruction priorities/ordering
 # All SIMD instructions supported by xsimd
 _x86 = [
     "avx512bw",
     "avx512dq",
     "avx512cd",
     "avx512f",
     "fma4",
-    "fma3<xs::avx2>",
     "avx2",
-    "fma3<xs::avx>",
     "avx",
-    "fma3<xs::sse4_2>",
     "sse4_2",
     "sse4_1",
     "ssse3",
     "sse3",
     "sse2",
 ]
 
 
 def _parse_arch_flag(arch):
     if "fma3" in arch:
         return "fma"
-    if "fma4" in arch:
-        return "fma4"
     return arch.replace("_", ".")
 
 
 def _get_arch_id(target_arch):
     try:
         target_arch_idx = _x86.index(target_arch)
     except ValueError:
         raise ValueError(
             f"Unknown target architecture '{target_arch}' provided; please choose from"
             f" {_x86} for x86 systems. Note we do not currently support ARM systems."
         )
     return target_arch_idx
 
 
-def _parse_spec(spec, arch):
+def _parse_spec(spec, arch, cur_archs):
     target_arch_idx = _get_arch_id(arch)
-    # We use a dict with empty values to preserve uniqueness and order of keys
-    out = {}
-
     if "<" in spec:
         fma_version = arch[3] if (len(arch) > 3 and arch[:3] == "fma") else -1
         for a in _x86[target_arch_idx:]:
             # Ensure unsupported/mutually-exclusive FMA features are not enabled
             if "fma" not in a or a[3] == fma_version:
-                out[a] = None
-    if "<=" in spec or not spec:
-        out[_x86[target_arch_idx]] = None
-    if "!" in spec:
-        out.pop(_x86[target_arch_idx], None)
-    return out
+                cur_archs[a] = None
+    if spec == "<=" or not spec:
+        cur_archs[_x86[target_arch_idx]] = None
+    if spec == "~":
+        cur_archs.pop(_x86[target_arch_idx], None)
+    return cur_archs
 
 
 def _make_architectures(target_archs):
-    SPECIFIERS = ["<=", "<", "!"]
-    out = {}
+    SPECIFIERS = ["<=", "<", "~"]
+    cur_archs = {}
+    has_fma3 = False
     for config in target_archs.split(","):
         config = config.strip()
         spec = ""
         arch = config
         for mark in SPECIFIERS:
             # Guard against incorrectly parsing fma3<...>
             if mark in config[:2]:
                 spec = mark
                 arch = arch[len(spec) :]
                 break
+        if arch == "fma3":
+            has_fma3 = True
+        else:
+            _parse_spec(spec, arch, cur_archs)
+    cur_archs = list(cur_archs)
+
+    # Second pass to enable any compatible fma3 sets
+    if has_fma3:
+        for fma_compatible_arch in ("sse4_2", "avx", "avx2"):
+            if fma_compatible_arch in cur_archs:
+                cur_archs.append(f"fma3<xs::{fma_compatible_arch}>")
 
-        out.update(_parse_spec(spec, arch))
-    return list(out)
+    return cur_archs
 
 
 def _pprint_config(config):
     for key in config:
         print(f"For function {key}:\n")
         spec = config[key]
         for section in spec:
```

### Comparing `slsdm-0.1.0/tests/test_distancemetrics.py` & `slsdm-0.2.0/tests/test_distancemetrics.py`

 * *Files identical despite different names*

