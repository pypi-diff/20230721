# Comparing `tmp/brain-isotopic-distribution-1.5.8.tar.gz` & `tmp/brain-isotopic-distribution-1.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brain-isotopic-distribution-1.5.8.tar", last modified: Sat Nov  6 02:29:30 2021, max compression
+gzip compressed data, was "brain-isotopic-distribution-1.5.9.tar", last modified: Sat Nov  6 19:11:41 2021, max compression
```

## Comparing `brain-isotopic-distribution-1.5.8.tar` & `brain-isotopic-distribution-1.5.9.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 02:29:30.633018 brain-isotopic-distribution-1.5.8/
--rw-r--r--   0 runner    (1001) docker     (121)    11358 2021-11-06 02:28:47.000000 brain-isotopic-distribution-1.5.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      124 2021-11-06 02:28:47.000000 brain-isotopic-distribution-1.5.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2985 2021-11-06 02:29:30.633018 brain-isotopic-distribution-1.5.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3292 2021-11-06 02:28:47.000000 brain-isotopic-distribution-1.5.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 02:29:30.625017 brain-isotopic-distribution-1.5.8/brain_isotopic_distribution.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2985 2021-11-06 02:29:12.000000 brain-isotopic-distribution-1.5.8/brain_isotopic_distribution.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      950 2021-11-06 02:29:12.000000 brain-isotopic-distribution-1.5.8/brain_isotopic_distribution.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-06 02:29:12.000000 brain-isotopic-distribution-1.5.8/brain_isotopic_distribution.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2021-11-06 02:29:12.000000 brain-isotopic-distribution-1.5.8/brain_isotopic_distribution.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 02:29:30.629017 brain-isotopic-distribution-1.5.8/brainpy/
--rw-r--r--   0 runner    (1001) docker     (121)     1839 2021-11-06 02:28:47.000000 brain-isotopic-distribution-1.5.8/brainpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 02:29:30.633018 brain-isotopic-distribution-1.5.8/brainpy/_c/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-06 02:28:47.000000 brain-isotopic-distribution-1.5.8/brainpy/_c/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3685 2021-11-06 02:28:47.000000 brain-isotopic-distribution-1.5.8/brainpy/_c/compat.h
--rw-r--r--   0 runner    (1001) docker     (121)      406 2021-11-06 02:28:47.000000 brain-isotopic-distribution-1.5.8/brainpy/_c/compat.pxd
--rw-r--r--   0 runner    (1001) docker     (121)   938767 2021-11-06 02:29:10.000000 brain-isotopic-distribution-1.5.8/brainpy/_c/composition.c
--rw-r--r--   0 runner    (1001) docker     (121)     5426 2021-11-06 02:28:47.000000 brain-isotopic-distribution-1.5.8/brainpy/_c/composition.pxd
--rw-r--r--   0 runner    (1001) docker     (121)    47727 2021-11-06 02:28:47.000000 brain-isotopic-distribution-1.5.8/brainpy/_c/composition.pyx
--rw-r--r--   0 runner    (1001) docker     (121)   139529 2021-11-06 02:29:10.000000 brain-isotopic-distribution-1.5.8/brainpy/_c/double_vector.c
--rw-r--r--   0 runner    (1001) docker     (121)      582 2021-11-06 02:28:47.000000 brain-isotopic-distribution-1.5.8/brainpy/_c/double_vector.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     2232 2021-11-06 02:28:47.000000 brain-isotopic-distribution-1.5.8/brainpy/_c/double_vector.pyx
--rw-r--r--   0 runner    (1001) docker     (121)   246621 2021-11-06 02:29:11.000000 brain-isotopic-distribution-1.5.8/brainpy/_c/isotopic_constants.c
--rw-r--r--   0 runner    (1001) docker     (121)     2402 2021-11-06 02:28:47.000000 brain-isotopic-distribution-1.5.8/brainpy/_c/isotopic_constants.pxd
--rw-r--r--   0 runner    (1001) docker     (121)    11905 2021-11-06 02:28:47.000000 brain-isotopic-distribution-1.5.8/brainpy/_c/isotopic_constants.pyx
--rw-r--r--   0 runner    (1001) docker     (121)   527711 2021-11-06 02:29:11.000000 brain-isotopic-distribution-1.5.8/brainpy/_c/isotopic_distribution.c
--rw-r--r--   0 runner    (1001) docker     (121)     2752 2021-11-06 02:28:47.000000 brain-isotopic-distribution-1.5.8/brainpy/_c/isotopic_distribution.pxd
--rw-r--r--   0 runner    (1001) docker     (121)    30260 2021-11-06 02:28:47.000000 brain-isotopic-distribution-1.5.8/brainpy/_c/isotopic_distribution.pyx
--rw-r--r--   0 runner    (1001) docker     (121)  1102282 2021-11-06 02:29:12.000000 brain-isotopic-distribution-1.5.8/brainpy/_speedup.c
--rw-r--r--   0 runner    (1001) docker     (121)      777 2021-11-06 02:28:47.000000 brain-isotopic-distribution-1.5.8/brainpy/_speedup.pxd
--rw-r--r--   0 runner    (1001) docker     (121)    22980 2021-11-06 02:28:47.000000 brain-isotopic-distribution-1.5.8/brainpy/_speedup.pyx
--rw-r--r--   0 runner    (1001) docker     (121)    22755 2021-11-06 02:28:47.000000 brain-isotopic-distribution-1.5.8/brainpy/brainpy.py
--rw-r--r--   0 runner    (1001) docker     (121)     4130 2021-11-06 02:28:47.000000 brain-isotopic-distribution-1.5.8/brainpy/composition.py
--rw-r--r--   0 runner    (1001) docker     (121)   110632 2021-11-06 02:28:47.000000 brain-isotopic-distribution-1.5.8/brainpy/mass_dict.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 02:29:30.633018 brain-isotopic-distribution-1.5.8/brainpy/test/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-06 02:28:47.000000 brain-isotopic-distribution-1.5.8/brainpy/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2682 2021-11-06 02:28:47.000000 brain-isotopic-distribution-1.5.8/brainpy/test/test_composition.py
--rw-r--r--   0 runner    (1001) docker     (121)     1550 2021-11-06 02:28:47.000000 brain-isotopic-distribution-1.5.8/brainpy/test/test_isotopic_distribution.py
--rw-r--r--   0 runner    (1001) docker     (121)       83 2021-11-06 02:28:47.000000 brain-isotopic-distribution-1.5.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      158 2021-11-06 02:29:30.633018 brain-isotopic-distribution-1.5.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     7247 2021-11-06 02:28:47.000000 brain-isotopic-distribution-1.5.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 19:11:41.347998 brain-isotopic-distribution-1.5.9/
+-rw-r--r--   0 runner    (1001) docker     (121)    11358 2021-11-06 19:11:04.000000 brain-isotopic-distribution-1.5.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      124 2021-11-06 19:11:04.000000 brain-isotopic-distribution-1.5.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     2985 2021-11-06 19:11:41.347998 brain-isotopic-distribution-1.5.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3292 2021-11-06 19:11:04.000000 brain-isotopic-distribution-1.5.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 19:11:41.339998 brain-isotopic-distribution-1.5.9/brain_isotopic_distribution.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     2985 2021-11-06 19:11:26.000000 brain-isotopic-distribution-1.5.9/brain_isotopic_distribution.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      950 2021-11-06 19:11:26.000000 brain-isotopic-distribution-1.5.9/brain_isotopic_distribution.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-06 19:11:26.000000 brain-isotopic-distribution-1.5.9/brain_isotopic_distribution.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        8 2021-11-06 19:11:26.000000 brain-isotopic-distribution-1.5.9/brain_isotopic_distribution.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 19:11:41.343999 brain-isotopic-distribution-1.5.9/brainpy/
+-rw-r--r--   0 runner    (1001) docker     (121)     1839 2021-11-06 19:11:04.000000 brain-isotopic-distribution-1.5.9/brainpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 19:11:41.347998 brain-isotopic-distribution-1.5.9/brainpy/_c/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-06 19:11:04.000000 brain-isotopic-distribution-1.5.9/brainpy/_c/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3685 2021-11-06 19:11:04.000000 brain-isotopic-distribution-1.5.9/brainpy/_c/compat.h
+-rw-r--r--   0 runner    (1001) docker     (121)      406 2021-11-06 19:11:04.000000 brain-isotopic-distribution-1.5.9/brainpy/_c/compat.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)   938767 2021-11-06 19:11:25.000000 brain-isotopic-distribution-1.5.9/brainpy/_c/composition.c
+-rw-r--r--   0 runner    (1001) docker     (121)     5426 2021-11-06 19:11:04.000000 brain-isotopic-distribution-1.5.9/brainpy/_c/composition.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)    47727 2021-11-06 19:11:04.000000 brain-isotopic-distribution-1.5.9/brainpy/_c/composition.pyx
+-rw-r--r--   0 runner    (1001) docker     (121)   139529 2021-11-06 19:11:25.000000 brain-isotopic-distribution-1.5.9/brainpy/_c/double_vector.c
+-rw-r--r--   0 runner    (1001) docker     (121)      582 2021-11-06 19:11:04.000000 brain-isotopic-distribution-1.5.9/brainpy/_c/double_vector.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     2232 2021-11-06 19:11:04.000000 brain-isotopic-distribution-1.5.9/brainpy/_c/double_vector.pyx
+-rw-r--r--   0 runner    (1001) docker     (121)   246621 2021-11-06 19:11:25.000000 brain-isotopic-distribution-1.5.9/brainpy/_c/isotopic_constants.c
+-rw-r--r--   0 runner    (1001) docker     (121)     2402 2021-11-06 19:11:04.000000 brain-isotopic-distribution-1.5.9/brainpy/_c/isotopic_constants.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)    11905 2021-11-06 19:11:04.000000 brain-isotopic-distribution-1.5.9/brainpy/_c/isotopic_constants.pyx
+-rw-r--r--   0 runner    (1001) docker     (121)   527719 2021-11-06 19:11:26.000000 brain-isotopic-distribution-1.5.9/brainpy/_c/isotopic_distribution.c
+-rw-r--r--   0 runner    (1001) docker     (121)     2752 2021-11-06 19:11:04.000000 brain-isotopic-distribution-1.5.9/brainpy/_c/isotopic_distribution.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)    30539 2021-11-06 19:11:04.000000 brain-isotopic-distribution-1.5.9/brainpy/_c/isotopic_distribution.pyx
+-rw-r--r--   0 runner    (1001) docker     (121)  1102282 2021-11-06 19:11:26.000000 brain-isotopic-distribution-1.5.9/brainpy/_speedup.c
+-rw-r--r--   0 runner    (1001) docker     (121)      777 2021-11-06 19:11:04.000000 brain-isotopic-distribution-1.5.9/brainpy/_speedup.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)    22980 2021-11-06 19:11:04.000000 brain-isotopic-distribution-1.5.9/brainpy/_speedup.pyx
+-rw-r--r--   0 runner    (1001) docker     (121)    22755 2021-11-06 19:11:04.000000 brain-isotopic-distribution-1.5.9/brainpy/brainpy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4130 2021-11-06 19:11:04.000000 brain-isotopic-distribution-1.5.9/brainpy/composition.py
+-rw-r--r--   0 runner    (1001) docker     (121)   110632 2021-11-06 19:11:04.000000 brain-isotopic-distribution-1.5.9/brainpy/mass_dict.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 19:11:41.347998 brain-isotopic-distribution-1.5.9/brainpy/test/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-06 19:11:04.000000 brain-isotopic-distribution-1.5.9/brainpy/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2682 2021-11-06 19:11:04.000000 brain-isotopic-distribution-1.5.9/brainpy/test/test_composition.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1550 2021-11-06 19:11:04.000000 brain-isotopic-distribution-1.5.9/brainpy/test/test_isotopic_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (121)       83 2021-11-06 19:11:04.000000 brain-isotopic-distribution-1.5.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      158 2021-11-06 19:11:41.347998 brain-isotopic-distribution-1.5.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     7247 2021-11-06 19:11:04.000000 brain-isotopic-distribution-1.5.9/setup.py
```

### Comparing `brain-isotopic-distribution-1.5.8/LICENSE` & `brain-isotopic-distribution-1.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `brain-isotopic-distribution-1.5.8/PKG-INFO` & `brain-isotopic-distribution-1.5.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brain-isotopic-distribution
-Version: 1.5.8
+Version: 1.5.9
 Summary: Fast and efficient theoretical isotopic profile generation
 Home-page: https://github.com/mobiusklein/brainpy
 Author: Joshua Klein, Han Hu
 Author-email: jaklein@bu.edu
 Maintainer: Joshua Klein
 Maintainer-email: jaklein@bu.edu
 License: UNKNOWN
```

### Comparing `brain-isotopic-distribution-1.5.8/README.md` & `brain-isotopic-distribution-1.5.9/README.md`

 * *Files identical despite different names*

### Comparing `brain-isotopic-distribution-1.5.8/brain_isotopic_distribution.egg-info/PKG-INFO` & `brain-isotopic-distribution-1.5.9/brain_isotopic_distribution.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brain-isotopic-distribution
-Version: 1.5.8
+Version: 1.5.9
 Summary: Fast and efficient theoretical isotopic profile generation
 Home-page: https://github.com/mobiusklein/brainpy
 Author: Joshua Klein, Han Hu
 Author-email: jaklein@bu.edu
 Maintainer: Joshua Klein
 Maintainer-email: jaklein@bu.edu
 License: UNKNOWN
```

### Comparing `brain-isotopic-distribution-1.5.8/brain_isotopic_distribution.egg-info/SOURCES.txt` & `brain-isotopic-distribution-1.5.9/brain_isotopic_distribution.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `brain-isotopic-distribution-1.5.8/brainpy/__init__.py` & `brain-isotopic-distribution-1.5.9/brainpy/__init__.py`

 * *Files identical despite different names*

### Comparing `brain-isotopic-distribution-1.5.8/brainpy/_c/compat.h` & `brain-isotopic-distribution-1.5.9/brainpy/_c/compat.h`

 * *Files identical despite different names*

### Comparing `brain-isotopic-distribution-1.5.8/brainpy/_c/composition.c` & `brain-isotopic-distribution-1.5.9/brainpy/_c/composition.c`

 * *Files identical despite different names*

### Comparing `brain-isotopic-distribution-1.5.8/brainpy/_c/composition.pxd` & `brain-isotopic-distribution-1.5.9/brainpy/_c/composition.pxd`

 * *Files identical despite different names*

### Comparing `brain-isotopic-distribution-1.5.8/brainpy/_c/composition.pyx` & `brain-isotopic-distribution-1.5.9/brainpy/_c/composition.pyx`

 * *Files identical despite different names*

### Comparing `brain-isotopic-distribution-1.5.8/brainpy/_c/double_vector.c` & `brain-isotopic-distribution-1.5.9/brainpy/_c/double_vector.c`

 * *Files identical despite different names*

### Comparing `brain-isotopic-distribution-1.5.8/brainpy/_c/double_vector.pxd` & `brain-isotopic-distribution-1.5.9/brainpy/_c/double_vector.pxd`

 * *Files identical despite different names*

### Comparing `brain-isotopic-distribution-1.5.8/brainpy/_c/double_vector.pyx` & `brain-isotopic-distribution-1.5.9/brainpy/_c/double_vector.pyx`

 * *Files identical despite different names*

### Comparing `brain-isotopic-distribution-1.5.8/brainpy/_c/isotopic_constants.c` & `brain-isotopic-distribution-1.5.9/brainpy/_c/isotopic_constants.c`

 * *Files identical despite different names*

### Comparing `brain-isotopic-distribution-1.5.8/brainpy/_c/isotopic_constants.pxd` & `brain-isotopic-distribution-1.5.9/brainpy/_c/isotopic_constants.pxd`

 * *Files identical despite different names*

### Comparing `brain-isotopic-distribution-1.5.8/brainpy/_c/isotopic_constants.pyx` & `brain-isotopic-distribution-1.5.9/brainpy/_c/isotopic_constants.pyx`

 * *Files identical despite different names*

### Comparing `brain-isotopic-distribution-1.5.8/brainpy/_c/isotopic_distribution.c` & `brain-isotopic-distribution-1.5.9/brainpy/_c/isotopic_distribution.c`

 * *Files 0% similar despite different names*

```diff
@@ -1207,15 +1207,15 @@
  * 
  * ctypedef DoubleVector dvec             # <<<<<<<<<<<<<<
  * 
  * 
  */
 typedef struct __pyx_t_7brainpy_2_c_13double_vector_DoubleVector __pyx_t_7brainpy_2_c_21isotopic_distribution_dvec;
 
-/* "brainpy/_c/isotopic_distribution.pyx":50
+/* "brainpy/_c/isotopic_distribution.pyx":62
  * # ElementPolynomialMap Declaration and Methods
  * 
  * cdef struct ElementPolynomialMap:             # <<<<<<<<<<<<<<
  *     char** elements
  *     dvec** polynomials
  */
 struct __pyx_t_7brainpy_2_c_21isotopic_distribution_ElementPolynomialMap {
@@ -1285,15 +1285,15 @@
   void (*add_from)(struct __pyx_obj_7brainpy_2_c_11composition_PyComposition *, struct __pyx_obj_7brainpy_2_c_11composition_PyComposition *);
   void (*subtract_from)(struct __pyx_obj_7brainpy_2_c_11composition_PyComposition *, struct __pyx_obj_7brainpy_2_c_11composition_PyComposition *);
   void (*scale_by)(struct __pyx_obj_7brainpy_2_c_11composition_PyComposition *, long);
 };
 static struct __pyx_vtabstruct_7brainpy_2_c_11composition_PyComposition *__pyx_vtabptr_7brainpy_2_c_11composition_PyComposition;
 
 
-/* "brainpy/_c/isotopic_distribution.pyx":788
+/* "brainpy/_c/isotopic_distribution.pyx":800
  * 
  * @cython.freelist(1000000)
  * cdef class TheoreticalPeak(object):             # <<<<<<<<<<<<<<
  *     def __init__(self, mz, intensity, charge):
  *         self.mz = mz
  */
 
@@ -1957,925 +1957,925 @@
 static PyObject *__pyx_tuple__11;
 static PyObject *__pyx_codeobj__6;
 static PyObject *__pyx_codeobj__8;
 static PyObject *__pyx_codeobj__10;
 static PyObject *__pyx_codeobj__12;
 /* Late includes */
 
-/* "brainpy/_c/isotopic_distribution.pyx":56
+/* "brainpy/_c/isotopic_distribution.pyx":68
  *     size_t size
  * 
  * cdef ElementPolynomialMap* make_element_polynomial_map(size_t sizehint) nogil:             # <<<<<<<<<<<<<<
  *     cdef ElementPolynomialMap* result
  *     result = <ElementPolynomialMap*>malloc(sizeof(ElementPolynomialMap))
  */
 
 static struct __pyx_t_7brainpy_2_c_21isotopic_distribution_ElementPolynomialMap *__pyx_f_7brainpy_2_c_21isotopic_distribution_make_element_polynomial_map(size_t __pyx_v_sizehint) {
   struct __pyx_t_7brainpy_2_c_21isotopic_distribution_ElementPolynomialMap *__pyx_v_result;
   struct __pyx_t_7brainpy_2_c_21isotopic_distribution_ElementPolynomialMap *__pyx_r;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":58
+  /* "brainpy/_c/isotopic_distribution.pyx":70
  * cdef ElementPolynomialMap* make_element_polynomial_map(size_t sizehint) nogil:
  *     cdef ElementPolynomialMap* result
  *     result = <ElementPolynomialMap*>malloc(sizeof(ElementPolynomialMap))             # <<<<<<<<<<<<<<
  *     result.elements = <char**>malloc(sizeof(char*) * sizehint)
  *     result.polynomials = <dvec**>malloc(sizeof(dvec*) * sizehint)
  */
   __pyx_v_result = ((struct __pyx_t_7brainpy_2_c_21isotopic_distribution_ElementPolynomialMap *)malloc((sizeof(struct __pyx_t_7brainpy_2_c_21isotopic_distribution_ElementPolynomialMap))));
 
-  /* "brainpy/_c/isotopic_distribution.pyx":59
+  /* "brainpy/_c/isotopic_distribution.pyx":71
  *     cdef ElementPolynomialMap* result
  *     result = <ElementPolynomialMap*>malloc(sizeof(ElementPolynomialMap))
  *     result.elements = <char**>malloc(sizeof(char*) * sizehint)             # <<<<<<<<<<<<<<
  *     result.polynomials = <dvec**>malloc(sizeof(dvec*) * sizehint)
  *     result.size = sizehint
  */
   __pyx_v_result->elements = ((char **)malloc(((sizeof(char *)) * __pyx_v_sizehint)));
 
-  /* "brainpy/_c/isotopic_distribution.pyx":60
+  /* "brainpy/_c/isotopic_distribution.pyx":72
  *     result = <ElementPolynomialMap*>malloc(sizeof(ElementPolynomialMap))
  *     result.elements = <char**>malloc(sizeof(char*) * sizehint)
  *     result.polynomials = <dvec**>malloc(sizeof(dvec*) * sizehint)             # <<<<<<<<<<<<<<
  *     result.size = sizehint
  *     result.used = 0
  */
   __pyx_v_result->polynomials = ((__pyx_t_7brainpy_2_c_21isotopic_distribution_dvec **)malloc(((sizeof(__pyx_t_7brainpy_2_c_21isotopic_distribution_dvec *)) * __pyx_v_sizehint)));
 
-  /* "brainpy/_c/isotopic_distribution.pyx":61
+  /* "brainpy/_c/isotopic_distribution.pyx":73
  *     result.elements = <char**>malloc(sizeof(char*) * sizehint)
  *     result.polynomials = <dvec**>malloc(sizeof(dvec*) * sizehint)
  *     result.size = sizehint             # <<<<<<<<<<<<<<
  *     result.used = 0
  * 
  */
   __pyx_v_result->size = __pyx_v_sizehint;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":62
+  /* "brainpy/_c/isotopic_distribution.pyx":74
  *     result.polynomials = <dvec**>malloc(sizeof(dvec*) * sizehint)
  *     result.size = sizehint
  *     result.used = 0             # <<<<<<<<<<<<<<
  * 
  *     return result
  */
   __pyx_v_result->used = 0;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":64
+  /* "brainpy/_c/isotopic_distribution.pyx":76
  *     result.used = 0
  * 
  *     return result             # <<<<<<<<<<<<<<
  * 
  * cdef int element_polynomial_map_set(ElementPolynomialMap* ep_map, char* element, dvec* polynomial) nogil:
  */
   __pyx_r = __pyx_v_result;
   goto __pyx_L0;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":56
+  /* "brainpy/_c/isotopic_distribution.pyx":68
  *     size_t size
  * 
  * cdef ElementPolynomialMap* make_element_polynomial_map(size_t sizehint) nogil:             # <<<<<<<<<<<<<<
  *     cdef ElementPolynomialMap* result
  *     result = <ElementPolynomialMap*>malloc(sizeof(ElementPolynomialMap))
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "brainpy/_c/isotopic_distribution.pyx":66
+/* "brainpy/_c/isotopic_distribution.pyx":78
  *     return result
  * 
  * cdef int element_polynomial_map_set(ElementPolynomialMap* ep_map, char* element, dvec* polynomial) nogil:             # <<<<<<<<<<<<<<
  *     cdef:
  *         size_t i
  */
 
 static int __pyx_f_7brainpy_2_c_21isotopic_distribution_element_polynomial_map_set(struct __pyx_t_7brainpy_2_c_21isotopic_distribution_ElementPolynomialMap *__pyx_v_ep_map, char *__pyx_v_element, __pyx_t_7brainpy_2_c_21isotopic_distribution_dvec *__pyx_v_polynomial) {
   size_t __pyx_v_i;
   int __pyx_v_done;
   int __pyx_r;
   int __pyx_t_1;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":72
+  /* "brainpy/_c/isotopic_distribution.pyx":84
  *         bint done
  * 
  *     done = False             # <<<<<<<<<<<<<<
  *     i = 0
  *     while (i < ep_map.used):
  */
   __pyx_v_done = 0;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":73
+  /* "brainpy/_c/isotopic_distribution.pyx":85
  * 
  *     done = False
  *     i = 0             # <<<<<<<<<<<<<<
  *     while (i < ep_map.used):
  *         if strcmp(element, ep_map.elements[i]) == 0:
  */
   __pyx_v_i = 0;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":74
+  /* "brainpy/_c/isotopic_distribution.pyx":86
  *     done = False
  *     i = 0
  *     while (i < ep_map.used):             # <<<<<<<<<<<<<<
  *         if strcmp(element, ep_map.elements[i]) == 0:
  *             done = True
  */
   while (1) {
     __pyx_t_1 = ((__pyx_v_i < __pyx_v_ep_map->used) != 0);
     if (!__pyx_t_1) break;
 
-    /* "brainpy/_c/isotopic_distribution.pyx":75
+    /* "brainpy/_c/isotopic_distribution.pyx":87
  *     i = 0
  *     while (i < ep_map.used):
  *         if strcmp(element, ep_map.elements[i]) == 0:             # <<<<<<<<<<<<<<
  *             done = True
  *             ep_map.polynomials[i] = polynomial
  */
     __pyx_t_1 = ((strcmp(__pyx_v_element, (__pyx_v_ep_map->elements[__pyx_v_i])) == 0) != 0);
     if (__pyx_t_1) {
 
-      /* "brainpy/_c/isotopic_distribution.pyx":76
+      /* "brainpy/_c/isotopic_distribution.pyx":88
  *     while (i < ep_map.used):
  *         if strcmp(element, ep_map.elements[i]) == 0:
  *             done = True             # <<<<<<<<<<<<<<
  *             ep_map.polynomials[i] = polynomial
  *             return 0
  */
       __pyx_v_done = 1;
 
-      /* "brainpy/_c/isotopic_distribution.pyx":77
+      /* "brainpy/_c/isotopic_distribution.pyx":89
  *         if strcmp(element, ep_map.elements[i]) == 0:
  *             done = True
  *             ep_map.polynomials[i] = polynomial             # <<<<<<<<<<<<<<
  *             return 0
  *         i += 1
  */
       (__pyx_v_ep_map->polynomials[__pyx_v_i]) = __pyx_v_polynomial;
 
-      /* "brainpy/_c/isotopic_distribution.pyx":78
+      /* "brainpy/_c/isotopic_distribution.pyx":90
  *             done = True
  *             ep_map.polynomials[i] = polynomial
  *             return 0             # <<<<<<<<<<<<<<
  *         i += 1
  *     if not done:
  */
       __pyx_r = 0;
       goto __pyx_L0;
 
-      /* "brainpy/_c/isotopic_distribution.pyx":75
+      /* "brainpy/_c/isotopic_distribution.pyx":87
  *     i = 0
  *     while (i < ep_map.used):
  *         if strcmp(element, ep_map.elements[i]) == 0:             # <<<<<<<<<<<<<<
  *             done = True
  *             ep_map.polynomials[i] = polynomial
  */
     }
 
-    /* "brainpy/_c/isotopic_distribution.pyx":79
+    /* "brainpy/_c/isotopic_distribution.pyx":91
  *             ep_map.polynomials[i] = polynomial
  *             return 0
  *         i += 1             # <<<<<<<<<<<<<<
  *     if not done:
  *         ep_map.used += 1
  */
     __pyx_v_i = (__pyx_v_i + 1);
   }
 
-  /* "brainpy/_c/isotopic_distribution.pyx":80
+  /* "brainpy/_c/isotopic_distribution.pyx":92
  *             return 0
  *         i += 1
  *     if not done:             # <<<<<<<<<<<<<<
  *         ep_map.used += 1
  *         if ep_map.used >= ep_map.size:
  */
   __pyx_t_1 = ((!(__pyx_v_done != 0)) != 0);
   if (__pyx_t_1) {
 
-    /* "brainpy/_c/isotopic_distribution.pyx":81
+    /* "brainpy/_c/isotopic_distribution.pyx":93
  *         i += 1
  *     if not done:
  *         ep_map.used += 1             # <<<<<<<<<<<<<<
  *         if ep_map.used >= ep_map.size:
  *             printf("Overloaded ElementPolynomialMap\n %d, %d\n", i, ep_map.size)
  */
     __pyx_v_ep_map->used = (__pyx_v_ep_map->used + 1);
 
-    /* "brainpy/_c/isotopic_distribution.pyx":82
+    /* "brainpy/_c/isotopic_distribution.pyx":94
  *     if not done:
  *         ep_map.used += 1
  *         if ep_map.used >= ep_map.size:             # <<<<<<<<<<<<<<
  *             printf("Overloaded ElementPolynomialMap\n %d, %d\n", i, ep_map.size)
  *             return -1
  */
     __pyx_t_1 = ((__pyx_v_ep_map->used >= __pyx_v_ep_map->size) != 0);
     if (__pyx_t_1) {
 
-      /* "brainpy/_c/isotopic_distribution.pyx":83
+      /* "brainpy/_c/isotopic_distribution.pyx":95
  *         ep_map.used += 1
  *         if ep_map.used >= ep_map.size:
  *             printf("Overloaded ElementPolynomialMap\n %d, %d\n", i, ep_map.size)             # <<<<<<<<<<<<<<
  *             return -1
  *         ep_map.elements[i] = element
  */
       (void)(printf(((char const *)"Overloaded ElementPolynomialMap\n %d, %d\n"), __pyx_v_i, __pyx_v_ep_map->size));
 
-      /* "brainpy/_c/isotopic_distribution.pyx":84
+      /* "brainpy/_c/isotopic_distribution.pyx":96
  *         if ep_map.used >= ep_map.size:
  *             printf("Overloaded ElementPolynomialMap\n %d, %d\n", i, ep_map.size)
  *             return -1             # <<<<<<<<<<<<<<
  *         ep_map.elements[i] = element
  *         ep_map.polynomials[i] = polynomial
  */
       __pyx_r = -1;
       goto __pyx_L0;
 
-      /* "brainpy/_c/isotopic_distribution.pyx":82
+      /* "brainpy/_c/isotopic_distribution.pyx":94
  *     if not done:
  *         ep_map.used += 1
  *         if ep_map.used >= ep_map.size:             # <<<<<<<<<<<<<<
  *             printf("Overloaded ElementPolynomialMap\n %d, %d\n", i, ep_map.size)
  *             return -1
  */
     }
 
-    /* "brainpy/_c/isotopic_distribution.pyx":85
+    /* "brainpy/_c/isotopic_distribution.pyx":97
  *             printf("Overloaded ElementPolynomialMap\n %d, %d\n", i, ep_map.size)
  *             return -1
  *         ep_map.elements[i] = element             # <<<<<<<<<<<<<<
  *         ep_map.polynomials[i] = polynomial
  *         return 0
  */
     (__pyx_v_ep_map->elements[__pyx_v_i]) = __pyx_v_element;
 
-    /* "brainpy/_c/isotopic_distribution.pyx":86
+    /* "brainpy/_c/isotopic_distribution.pyx":98
  *             return -1
  *         ep_map.elements[i] = element
  *         ep_map.polynomials[i] = polynomial             # <<<<<<<<<<<<<<
  *         return 0
  *     return 1
  */
     (__pyx_v_ep_map->polynomials[__pyx_v_i]) = __pyx_v_polynomial;
 
-    /* "brainpy/_c/isotopic_distribution.pyx":87
+    /* "brainpy/_c/isotopic_distribution.pyx":99
  *         ep_map.elements[i] = element
  *         ep_map.polynomials[i] = polynomial
  *         return 0             # <<<<<<<<<<<<<<
  *     return 1
  * 
  */
     __pyx_r = 0;
     goto __pyx_L0;
 
-    /* "brainpy/_c/isotopic_distribution.pyx":80
+    /* "brainpy/_c/isotopic_distribution.pyx":92
  *             return 0
  *         i += 1
  *     if not done:             # <<<<<<<<<<<<<<
  *         ep_map.used += 1
  *         if ep_map.used >= ep_map.size:
  */
   }
 
-  /* "brainpy/_c/isotopic_distribution.pyx":88
+  /* "brainpy/_c/isotopic_distribution.pyx":100
  *         ep_map.polynomials[i] = polynomial
  *         return 0
  *     return 1             # <<<<<<<<<<<<<<
  * 
  * cdef int element_polynomial_map_get(ElementPolynomialMap* ep_map, char* element, dvec** polynomial) nogil:
  */
   __pyx_r = 1;
   goto __pyx_L0;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":66
+  /* "brainpy/_c/isotopic_distribution.pyx":78
  *     return result
  * 
  * cdef int element_polynomial_map_set(ElementPolynomialMap* ep_map, char* element, dvec* polynomial) nogil:             # <<<<<<<<<<<<<<
  *     cdef:
  *         size_t i
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "brainpy/_c/isotopic_distribution.pyx":90
+/* "brainpy/_c/isotopic_distribution.pyx":102
  *     return 1
  * 
  * cdef int element_polynomial_map_get(ElementPolynomialMap* ep_map, char* element, dvec** polynomial) nogil:             # <<<<<<<<<<<<<<
  *     cdef:
  *         size_t i
  */
 
 static int __pyx_f_7brainpy_2_c_21isotopic_distribution_element_polynomial_map_get(struct __pyx_t_7brainpy_2_c_21isotopic_distribution_ElementPolynomialMap *__pyx_v_ep_map, char *__pyx_v_element, __pyx_t_7brainpy_2_c_21isotopic_distribution_dvec **__pyx_v_polynomial) {
   size_t __pyx_v_i;
   CYTHON_UNUSED int __pyx_v_done;
   int __pyx_r;
   int __pyx_t_1;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":96
+  /* "brainpy/_c/isotopic_distribution.pyx":108
  *         bint done
  * 
  *     done = False             # <<<<<<<<<<<<<<
  *     i = 0
  *     while i < ep_map.used:
  */
   __pyx_v_done = 0;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":97
+  /* "brainpy/_c/isotopic_distribution.pyx":109
  * 
  *     done = False
  *     i = 0             # <<<<<<<<<<<<<<
  *     while i < ep_map.used:
  *         if strcmp(ep_map.elements[i], element) == 0:
  */
   __pyx_v_i = 0;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":98
+  /* "brainpy/_c/isotopic_distribution.pyx":110
  *     done = False
  *     i = 0
  *     while i < ep_map.used:             # <<<<<<<<<<<<<<
  *         if strcmp(ep_map.elements[i], element) == 0:
  *             polynomial[0] = ep_map.polynomials[i]
  */
   while (1) {
     __pyx_t_1 = ((__pyx_v_i < __pyx_v_ep_map->used) != 0);
     if (!__pyx_t_1) break;
 
-    /* "brainpy/_c/isotopic_distribution.pyx":99
+    /* "brainpy/_c/isotopic_distribution.pyx":111
  *     i = 0
  *     while i < ep_map.used:
  *         if strcmp(ep_map.elements[i], element) == 0:             # <<<<<<<<<<<<<<
  *             polynomial[0] = ep_map.polynomials[i]
  *             return 0
  */
     __pyx_t_1 = ((strcmp((__pyx_v_ep_map->elements[__pyx_v_i]), __pyx_v_element) == 0) != 0);
     if (__pyx_t_1) {
 
-      /* "brainpy/_c/isotopic_distribution.pyx":100
+      /* "brainpy/_c/isotopic_distribution.pyx":112
  *     while i < ep_map.used:
  *         if strcmp(ep_map.elements[i], element) == 0:
  *             polynomial[0] = ep_map.polynomials[i]             # <<<<<<<<<<<<<<
  *             return 0
  *         i += 1
  */
       (__pyx_v_polynomial[0]) = (__pyx_v_ep_map->polynomials[__pyx_v_i]);
 
-      /* "brainpy/_c/isotopic_distribution.pyx":101
+      /* "brainpy/_c/isotopic_distribution.pyx":113
  *         if strcmp(ep_map.elements[i], element) == 0:
  *             polynomial[0] = ep_map.polynomials[i]
  *             return 0             # <<<<<<<<<<<<<<
  *         i += 1
  *     return 1
  */
       __pyx_r = 0;
       goto __pyx_L0;
 
-      /* "brainpy/_c/isotopic_distribution.pyx":99
+      /* "brainpy/_c/isotopic_distribution.pyx":111
  *     i = 0
  *     while i < ep_map.used:
  *         if strcmp(ep_map.elements[i], element) == 0:             # <<<<<<<<<<<<<<
  *             polynomial[0] = ep_map.polynomials[i]
  *             return 0
  */
     }
 
-    /* "brainpy/_c/isotopic_distribution.pyx":102
+    /* "brainpy/_c/isotopic_distribution.pyx":114
  *             polynomial[0] = ep_map.polynomials[i]
  *             return 0
  *         i += 1             # <<<<<<<<<<<<<<
  *     return 1
  * 
  */
     __pyx_v_i = (__pyx_v_i + 1);
   }
 
-  /* "brainpy/_c/isotopic_distribution.pyx":103
+  /* "brainpy/_c/isotopic_distribution.pyx":115
  *             return 0
  *         i += 1
  *     return 1             # <<<<<<<<<<<<<<
  * 
  * cdef void free_element_polynomial_map(ElementPolynomialMap* ep_map) nogil:
  */
   __pyx_r = 1;
   goto __pyx_L0;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":90
+  /* "brainpy/_c/isotopic_distribution.pyx":102
  *     return 1
  * 
  * cdef int element_polynomial_map_get(ElementPolynomialMap* ep_map, char* element, dvec** polynomial) nogil:             # <<<<<<<<<<<<<<
  *     cdef:
  *         size_t i
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "brainpy/_c/isotopic_distribution.pyx":105
+/* "brainpy/_c/isotopic_distribution.pyx":117
  *     return 1
  * 
  * cdef void free_element_polynomial_map(ElementPolynomialMap* ep_map) nogil:             # <<<<<<<<<<<<<<
  *     cdef:
  *         size_t i
  */
 
 static void __pyx_f_7brainpy_2_c_21isotopic_distribution_free_element_polynomial_map(struct __pyx_t_7brainpy_2_c_21isotopic_distribution_ElementPolynomialMap *__pyx_v_ep_map) {
   size_t __pyx_v_i;
   int __pyx_t_1;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":108
+  /* "brainpy/_c/isotopic_distribution.pyx":120
  *     cdef:
  *         size_t i
  *     i = 0             # <<<<<<<<<<<<<<
  *     while i < ep_map.used:
  *         free_double_vector(ep_map.polynomials[i])
  */
   __pyx_v_i = 0;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":109
+  /* "brainpy/_c/isotopic_distribution.pyx":121
  *         size_t i
  *     i = 0
  *     while i < ep_map.used:             # <<<<<<<<<<<<<<
  *         free_double_vector(ep_map.polynomials[i])
  *         i += 1
  */
   while (1) {
     __pyx_t_1 = ((__pyx_v_i < __pyx_v_ep_map->used) != 0);
     if (!__pyx_t_1) break;
 
-    /* "brainpy/_c/isotopic_distribution.pyx":110
+    /* "brainpy/_c/isotopic_distribution.pyx":122
  *     i = 0
  *     while i < ep_map.used:
  *         free_double_vector(ep_map.polynomials[i])             # <<<<<<<<<<<<<<
  *         i += 1
  *     free(ep_map.elements)
  */
     __pyx_f_7brainpy_2_c_13double_vector_free_double_vector((__pyx_v_ep_map->polynomials[__pyx_v_i]));
 
-    /* "brainpy/_c/isotopic_distribution.pyx":111
+    /* "brainpy/_c/isotopic_distribution.pyx":123
  *     while i < ep_map.used:
  *         free_double_vector(ep_map.polynomials[i])
  *         i += 1             # <<<<<<<<<<<<<<
  *     free(ep_map.elements)
  *     free(ep_map.polynomials)
  */
     __pyx_v_i = (__pyx_v_i + 1);
   }
 
-  /* "brainpy/_c/isotopic_distribution.pyx":112
+  /* "brainpy/_c/isotopic_distribution.pyx":124
  *         free_double_vector(ep_map.polynomials[i])
  *         i += 1
  *     free(ep_map.elements)             # <<<<<<<<<<<<<<
  *     free(ep_map.polynomials)
  *     free(ep_map)
  */
   free(__pyx_v_ep_map->elements);
 
-  /* "brainpy/_c/isotopic_distribution.pyx":113
+  /* "brainpy/_c/isotopic_distribution.pyx":125
  *         i += 1
  *     free(ep_map.elements)
  *     free(ep_map.polynomials)             # <<<<<<<<<<<<<<
  *     free(ep_map)
  * 
  */
   free(__pyx_v_ep_map->polynomials);
 
-  /* "brainpy/_c/isotopic_distribution.pyx":114
+  /* "brainpy/_c/isotopic_distribution.pyx":126
  *     free(ep_map.elements)
  *     free(ep_map.polynomials)
  *     free(ep_map)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   free(__pyx_v_ep_map);
 
-  /* "brainpy/_c/isotopic_distribution.pyx":105
+  /* "brainpy/_c/isotopic_distribution.pyx":117
  *     return 1
  * 
  * cdef void free_element_polynomial_map(ElementPolynomialMap* ep_map) nogil:             # <<<<<<<<<<<<<<
  *     cdef:
  *         size_t i
  */
 
   /* function exit code */
 }
 
-/* "brainpy/_c/isotopic_distribution.pyx":120
+/* "brainpy/_c/isotopic_distribution.pyx":132
  * # Peak Methods
  * 
  * cdef void print_peak(Peak* peak) nogil:             # <<<<<<<<<<<<<<
  *     printf("Peak: %f, %f, %d\n", peak.mz, peak.intensity, peak.charge)
  * 
  */
 
 static void __pyx_f_7brainpy_2_c_21isotopic_distribution_print_peak(struct __pyx_t_7brainpy_2_c_21isotopic_distribution_Peak *__pyx_v_peak) {
 
-  /* "brainpy/_c/isotopic_distribution.pyx":121
+  /* "brainpy/_c/isotopic_distribution.pyx":133
  * 
  * cdef void print_peak(Peak* peak) nogil:
  *     printf("Peak: %f, %f, %d\n", peak.mz, peak.intensity, peak.charge)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   (void)(printf(((char const *)"Peak: %f, %f, %d\n"), __pyx_v_peak->mz, __pyx_v_peak->intensity, __pyx_v_peak->charge));
 
-  /* "brainpy/_c/isotopic_distribution.pyx":120
+  /* "brainpy/_c/isotopic_distribution.pyx":132
  * # Peak Methods
  * 
  * cdef void print_peak(Peak* peak) nogil:             # <<<<<<<<<<<<<<
  *     printf("Peak: %f, %f, %d\n", peak.mz, peak.intensity, peak.charge)
  * 
  */
 
   /* function exit code */
 }
 
-/* "brainpy/_c/isotopic_distribution.pyx":124
+/* "brainpy/_c/isotopic_distribution.pyx":136
  * 
  * 
  * cdef Peak* make_peak(double mz, double intensity, int charge) nogil:             # <<<<<<<<<<<<<<
  *     cdef Peak* peak
  *     peak = <Peak*>malloc(sizeof(Peak))
  */
 
 static struct __pyx_t_7brainpy_2_c_21isotopic_distribution_Peak *__pyx_f_7brainpy_2_c_21isotopic_distribution_make_peak(double __pyx_v_mz, double __pyx_v_intensity, int __pyx_v_charge) {
   struct __pyx_t_7brainpy_2_c_21isotopic_distribution_Peak *__pyx_v_peak;
   struct __pyx_t_7brainpy_2_c_21isotopic_distribution_Peak *__pyx_r;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":126
+  /* "brainpy/_c/isotopic_distribution.pyx":138
  * cdef Peak* make_peak(double mz, double intensity, int charge) nogil:
  *     cdef Peak* peak
  *     peak = <Peak*>malloc(sizeof(Peak))             # <<<<<<<<<<<<<<
  *     peak.mz = mz
  *     peak.intensity = intensity
  */
   __pyx_v_peak = ((struct __pyx_t_7brainpy_2_c_21isotopic_distribution_Peak *)malloc((sizeof(struct __pyx_t_7brainpy_2_c_21isotopic_distribution_Peak))));
 
-  /* "brainpy/_c/isotopic_distribution.pyx":127
+  /* "brainpy/_c/isotopic_distribution.pyx":139
  *     cdef Peak* peak
  *     peak = <Peak*>malloc(sizeof(Peak))
  *     peak.mz = mz             # <<<<<<<<<<<<<<
  *     peak.intensity = intensity
  *     peak.charge = charge
  */
   __pyx_v_peak->mz = __pyx_v_mz;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":128
+  /* "brainpy/_c/isotopic_distribution.pyx":140
  *     peak = <Peak*>malloc(sizeof(Peak))
  *     peak.mz = mz
  *     peak.intensity = intensity             # <<<<<<<<<<<<<<
  *     peak.charge = charge
  *     return peak
  */
   __pyx_v_peak->intensity = __pyx_v_intensity;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":129
+  /* "brainpy/_c/isotopic_distribution.pyx":141
  *     peak.mz = mz
  *     peak.intensity = intensity
  *     peak.charge = charge             # <<<<<<<<<<<<<<
  *     return peak
  * 
  */
   __pyx_v_peak->charge = __pyx_v_charge;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":130
+  /* "brainpy/_c/isotopic_distribution.pyx":142
  *     peak.intensity = intensity
  *     peak.charge = charge
  *     return peak             # <<<<<<<<<<<<<<
  * 
  * # -----------------------------------------------------------------------------
  */
   __pyx_r = __pyx_v_peak;
   goto __pyx_L0;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":124
+  /* "brainpy/_c/isotopic_distribution.pyx":136
  * 
  * 
  * cdef Peak* make_peak(double mz, double intensity, int charge) nogil:             # <<<<<<<<<<<<<<
  *     cdef Peak* peak
  *     peak = <Peak*>malloc(sizeof(Peak))
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "brainpy/_c/isotopic_distribution.pyx":135
+/* "brainpy/_c/isotopic_distribution.pyx":147
  * # PeakList Methods
  * 
  * cdef PeakList* make_peak_list() nogil:             # <<<<<<<<<<<<<<
  *     cdef PeakList* result
  * 
  */
 
 static struct __pyx_t_7brainpy_2_c_21isotopic_distribution_PeakList *__pyx_f_7brainpy_2_c_21isotopic_distribution_make_peak_list(void) {
   struct __pyx_t_7brainpy_2_c_21isotopic_distribution_PeakList *__pyx_v_result;
   struct __pyx_t_7brainpy_2_c_21isotopic_distribution_PeakList *__pyx_r;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":138
+  /* "brainpy/_c/isotopic_distribution.pyx":150
  *     cdef PeakList* result
  * 
  *     result = <PeakList*>malloc(sizeof(PeakList))             # <<<<<<<<<<<<<<
  *     result.peaks = <Peak*>malloc(sizeof(Peak) * 10)
  *     result.size = 10
  */
   __pyx_v_result = ((struct __pyx_t_7brainpy_2_c_21isotopic_distribution_PeakList *)malloc((sizeof(struct __pyx_t_7brainpy_2_c_21isotopic_distribution_PeakList))));
 
-  /* "brainpy/_c/isotopic_distribution.pyx":139
+  /* "brainpy/_c/isotopic_distribution.pyx":151
  * 
  *     result = <PeakList*>malloc(sizeof(PeakList))
  *     result.peaks = <Peak*>malloc(sizeof(Peak) * 10)             # <<<<<<<<<<<<<<
  *     result.size = 10
  *     result.used = 0
  */
   __pyx_v_result->peaks = ((struct __pyx_t_7brainpy_2_c_21isotopic_distribution_Peak *)malloc(((sizeof(struct __pyx_t_7brainpy_2_c_21isotopic_distribution_Peak)) * 10)));
 
-  /* "brainpy/_c/isotopic_distribution.pyx":140
+  /* "brainpy/_c/isotopic_distribution.pyx":152
  *     result = <PeakList*>malloc(sizeof(PeakList))
  *     result.peaks = <Peak*>malloc(sizeof(Peak) * 10)
  *     result.size = 10             # <<<<<<<<<<<<<<
  *     result.used = 0
  * 
  */
   __pyx_v_result->size = 10;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":141
+  /* "brainpy/_c/isotopic_distribution.pyx":153
  *     result.peaks = <Peak*>malloc(sizeof(Peak) * 10)
  *     result.size = 10
  *     result.used = 0             # <<<<<<<<<<<<<<
  * 
  *     return result
  */
   __pyx_v_result->used = 0;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":143
+  /* "brainpy/_c/isotopic_distribution.pyx":155
  *     result.used = 0
  * 
  *     return result             # <<<<<<<<<<<<<<
  * 
  * cdef void free_peak_list(PeakList* peaklist) nogil:
  */
   __pyx_r = __pyx_v_result;
   goto __pyx_L0;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":135
+  /* "brainpy/_c/isotopic_distribution.pyx":147
  * # PeakList Methods
  * 
  * cdef PeakList* make_peak_list() nogil:             # <<<<<<<<<<<<<<
  *     cdef PeakList* result
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "brainpy/_c/isotopic_distribution.pyx":145
+/* "brainpy/_c/isotopic_distribution.pyx":157
  *     return result
  * 
  * cdef void free_peak_list(PeakList* peaklist) nogil:             # <<<<<<<<<<<<<<
  *     free(peaklist.peaks)
  *     free(peaklist)
  */
 
 static void __pyx_f_7brainpy_2_c_21isotopic_distribution_free_peak_list(struct __pyx_t_7brainpy_2_c_21isotopic_distribution_PeakList *__pyx_v_peaklist) {
 
-  /* "brainpy/_c/isotopic_distribution.pyx":146
+  /* "brainpy/_c/isotopic_distribution.pyx":158
  * 
  * cdef void free_peak_list(PeakList* peaklist) nogil:
  *     free(peaklist.peaks)             # <<<<<<<<<<<<<<
  *     free(peaklist)
  * 
  */
   free(__pyx_v_peaklist->peaks);
 
-  /* "brainpy/_c/isotopic_distribution.pyx":147
+  /* "brainpy/_c/isotopic_distribution.pyx":159
  * cdef void free_peak_list(PeakList* peaklist) nogil:
  *     free(peaklist.peaks)
  *     free(peaklist)             # <<<<<<<<<<<<<<
  * 
  * cdef int resize_peak_list(PeakList* peaklist) nogil:
  */
   free(__pyx_v_peaklist);
 
-  /* "brainpy/_c/isotopic_distribution.pyx":145
+  /* "brainpy/_c/isotopic_distribution.pyx":157
  *     return result
  * 
  * cdef void free_peak_list(PeakList* peaklist) nogil:             # <<<<<<<<<<<<<<
  *     free(peaklist.peaks)
  *     free(peaklist)
  */
 
   /* function exit code */
 }
 
-/* "brainpy/_c/isotopic_distribution.pyx":149
+/* "brainpy/_c/isotopic_distribution.pyx":161
  *     free(peaklist)
  * 
  * cdef int resize_peak_list(PeakList* peaklist) nogil:             # <<<<<<<<<<<<<<
  *     cdef:
  *         Peak* peaks
  */
 
 static int __pyx_f_7brainpy_2_c_21isotopic_distribution_resize_peak_list(struct __pyx_t_7brainpy_2_c_21isotopic_distribution_PeakList *__pyx_v_peaklist) {
   struct __pyx_t_7brainpy_2_c_21isotopic_distribution_Peak *__pyx_v_peaks;
   int __pyx_r;
   int __pyx_t_1;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":152
+  /* "brainpy/_c/isotopic_distribution.pyx":164
  *     cdef:
  *         Peak* peaks
  *     peaks = <Peak*>realloc(peaklist.peaks, sizeof(Peak) * peaklist.size * 2)             # <<<<<<<<<<<<<<
  *     if peaks == NULL:
  *         printf("realloc peaklist returned NULL\n")
  */
   __pyx_v_peaks = ((struct __pyx_t_7brainpy_2_c_21isotopic_distribution_Peak *)realloc(__pyx_v_peaklist->peaks, (((sizeof(struct __pyx_t_7brainpy_2_c_21isotopic_distribution_Peak)) * __pyx_v_peaklist->size) * 2)));
 
-  /* "brainpy/_c/isotopic_distribution.pyx":153
+  /* "brainpy/_c/isotopic_distribution.pyx":165
  *         Peak* peaks
  *     peaks = <Peak*>realloc(peaklist.peaks, sizeof(Peak) * peaklist.size * 2)
  *     if peaks == NULL:             # <<<<<<<<<<<<<<
  *         printf("realloc peaklist returned NULL\n")
  *         return -1
  */
   __pyx_t_1 = ((__pyx_v_peaks == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "brainpy/_c/isotopic_distribution.pyx":154
+    /* "brainpy/_c/isotopic_distribution.pyx":166
  *     peaks = <Peak*>realloc(peaklist.peaks, sizeof(Peak) * peaklist.size * 2)
  *     if peaks == NULL:
  *         printf("realloc peaklist returned NULL\n")             # <<<<<<<<<<<<<<
  *         return -1
  *     peaklist.peaks = peaks
  */
     (void)(printf(((char const *)"realloc peaklist returned NULL\n")));
 
-    /* "brainpy/_c/isotopic_distribution.pyx":155
+    /* "brainpy/_c/isotopic_distribution.pyx":167
  *     if peaks == NULL:
  *         printf("realloc peaklist returned NULL\n")
  *         return -1             # <<<<<<<<<<<<<<
  *     peaklist.peaks = peaks
  *     peaklist.size *= 2
  */
     __pyx_r = -1;
     goto __pyx_L0;
 
-    /* "brainpy/_c/isotopic_distribution.pyx":153
+    /* "brainpy/_c/isotopic_distribution.pyx":165
  *         Peak* peaks
  *     peaks = <Peak*>realloc(peaklist.peaks, sizeof(Peak) * peaklist.size * 2)
  *     if peaks == NULL:             # <<<<<<<<<<<<<<
  *         printf("realloc peaklist returned NULL\n")
  *         return -1
  */
   }
 
-  /* "brainpy/_c/isotopic_distribution.pyx":156
+  /* "brainpy/_c/isotopic_distribution.pyx":168
  *         printf("realloc peaklist returned NULL\n")
  *         return -1
  *     peaklist.peaks = peaks             # <<<<<<<<<<<<<<
  *     peaklist.size *= 2
  *     return 0
  */
   __pyx_v_peaklist->peaks = __pyx_v_peaks;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":157
+  /* "brainpy/_c/isotopic_distribution.pyx":169
  *         return -1
  *     peaklist.peaks = peaks
  *     peaklist.size *= 2             # <<<<<<<<<<<<<<
  *     return 0
  * 
  */
   __pyx_v_peaklist->size = (__pyx_v_peaklist->size * 2);
 
-  /* "brainpy/_c/isotopic_distribution.pyx":158
+  /* "brainpy/_c/isotopic_distribution.pyx":170
  *     peaklist.peaks = peaks
  *     peaklist.size *= 2
  *     return 0             # <<<<<<<<<<<<<<
  * 
  * cdef void peak_list_append(PeakList* peaklist, Peak* peak) nogil:
  */
   __pyx_r = 0;
   goto __pyx_L0;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":149
+  /* "brainpy/_c/isotopic_distribution.pyx":161
  *     free(peaklist)
  * 
  * cdef int resize_peak_list(PeakList* peaklist) nogil:             # <<<<<<<<<<<<<<
  *     cdef:
  *         Peak* peaks
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "brainpy/_c/isotopic_distribution.pyx":160
+/* "brainpy/_c/isotopic_distribution.pyx":172
  *     return 0
  * 
  * cdef void peak_list_append(PeakList* peaklist, Peak* peak) nogil:             # <<<<<<<<<<<<<<
  *     if peaklist.used == peaklist.size:
  *         resize_peak_list(peaklist)
  */
 
 static void __pyx_f_7brainpy_2_c_21isotopic_distribution_peak_list_append(struct __pyx_t_7brainpy_2_c_21isotopic_distribution_PeakList *__pyx_v_peaklist, struct __pyx_t_7brainpy_2_c_21isotopic_distribution_Peak *__pyx_v_peak) {
   int __pyx_t_1;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":161
+  /* "brainpy/_c/isotopic_distribution.pyx":173
  * 
  * cdef void peak_list_append(PeakList* peaklist, Peak* peak) nogil:
  *     if peaklist.used == peaklist.size:             # <<<<<<<<<<<<<<
  *         resize_peak_list(peaklist)
  *     peaklist.peaks[peaklist.used] = peak[0]
  */
   __pyx_t_1 = ((__pyx_v_peaklist->used == __pyx_v_peaklist->size) != 0);
   if (__pyx_t_1) {
 
-    /* "brainpy/_c/isotopic_distribution.pyx":162
+    /* "brainpy/_c/isotopic_distribution.pyx":174
  * cdef void peak_list_append(PeakList* peaklist, Peak* peak) nogil:
  *     if peaklist.used == peaklist.size:
  *         resize_peak_list(peaklist)             # <<<<<<<<<<<<<<
  *     peaklist.peaks[peaklist.used] = peak[0]
  *     peaklist.used += 1
  */
     (void)(__pyx_f_7brainpy_2_c_21isotopic_distribution_resize_peak_list(__pyx_v_peaklist));
 
-    /* "brainpy/_c/isotopic_distribution.pyx":161
+    /* "brainpy/_c/isotopic_distribution.pyx":173
  * 
  * cdef void peak_list_append(PeakList* peaklist, Peak* peak) nogil:
  *     if peaklist.used == peaklist.size:             # <<<<<<<<<<<<<<
  *         resize_peak_list(peaklist)
  *     peaklist.peaks[peaklist.used] = peak[0]
  */
   }
 
-  /* "brainpy/_c/isotopic_distribution.pyx":163
+  /* "brainpy/_c/isotopic_distribution.pyx":175
  *     if peaklist.used == peaklist.size:
  *         resize_peak_list(peaklist)
  *     peaklist.peaks[peaklist.used] = peak[0]             # <<<<<<<<<<<<<<
  *     peaklist.used += 1
  * 
  */
   (__pyx_v_peaklist->peaks[__pyx_v_peaklist->used]) = (__pyx_v_peak[0]);
 
-  /* "brainpy/_c/isotopic_distribution.pyx":164
+  /* "brainpy/_c/isotopic_distribution.pyx":176
  *         resize_peak_list(peaklist)
  *     peaklist.peaks[peaklist.used] = peak[0]
  *     peaklist.used += 1             # <<<<<<<<<<<<<<
  * 
  * cdef void peak_list_reset(PeakList* peaklist) nogil:
  */
   __pyx_v_peaklist->used = (__pyx_v_peaklist->used + 1);
 
-  /* "brainpy/_c/isotopic_distribution.pyx":160
+  /* "brainpy/_c/isotopic_distribution.pyx":172
  *     return 0
  * 
  * cdef void peak_list_append(PeakList* peaklist, Peak* peak) nogil:             # <<<<<<<<<<<<<<
  *     if peaklist.used == peaklist.size:
  *         resize_peak_list(peaklist)
  */
 
   /* function exit code */
 }
 
-/* "brainpy/_c/isotopic_distribution.pyx":166
+/* "brainpy/_c/isotopic_distribution.pyx":178
  *     peaklist.used += 1
  * 
  * cdef void peak_list_reset(PeakList* peaklist) nogil:             # <<<<<<<<<<<<<<
  *     peaklist.used = 0
  * 
  */
 
 static void __pyx_f_7brainpy_2_c_21isotopic_distribution_peak_list_reset(struct __pyx_t_7brainpy_2_c_21isotopic_distribution_PeakList *__pyx_v_peaklist) {
 
-  /* "brainpy/_c/isotopic_distribution.pyx":167
+  /* "brainpy/_c/isotopic_distribution.pyx":179
  * 
  * cdef void peak_list_reset(PeakList* peaklist) nogil:
  *     peaklist.used = 0             # <<<<<<<<<<<<<<
  * 
  * @cython.cdivision
  */
   __pyx_v_peaklist->used = 0;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":166
+  /* "brainpy/_c/isotopic_distribution.pyx":178
  *     peaklist.used += 1
  * 
  * cdef void peak_list_reset(PeakList* peaklist) nogil:             # <<<<<<<<<<<<<<
  *     peaklist.used = 0
  * 
  */
 
   /* function exit code */
 }
 
-/* "brainpy/_c/isotopic_distribution.pyx":170
+/* "brainpy/_c/isotopic_distribution.pyx":182
  * 
  * @cython.cdivision
  * cdef PeakList* peak_list_ignore_below(PeakList* peaklist, double ignore_below, PeakList* result) nogil:             # <<<<<<<<<<<<<<
  *     cdef:
  *         double total
  */
 
@@ -2888,83 +2888,83 @@
   size_t __pyx_t_1;
   int __pyx_t_2;
   size_t __pyx_t_3;
   size_t __pyx_t_4;
   int __pyx_t_5;
   size_t __pyx_t_6;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":177
+  /* "brainpy/_c/isotopic_distribution.pyx":189
  *         Peak p
  * 
  *     total = 0             # <<<<<<<<<<<<<<
  *     n = peaklist.used
  * 
  */
   __pyx_v_total = 0.0;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":178
+  /* "brainpy/_c/isotopic_distribution.pyx":190
  * 
  *     total = 0
  *     n = peaklist.used             # <<<<<<<<<<<<<<
  * 
  *     if result == NULL:
  */
   __pyx_t_1 = __pyx_v_peaklist->used;
   __pyx_v_n = __pyx_t_1;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":180
+  /* "brainpy/_c/isotopic_distribution.pyx":192
  *     n = peaklist.used
  * 
  *     if result == NULL:             # <<<<<<<<<<<<<<
  *         result = make_peak_list()
  * 
  */
   __pyx_t_2 = ((__pyx_v_result == NULL) != 0);
   if (__pyx_t_2) {
 
-    /* "brainpy/_c/isotopic_distribution.pyx":181
+    /* "brainpy/_c/isotopic_distribution.pyx":193
  * 
  *     if result == NULL:
  *         result = make_peak_list()             # <<<<<<<<<<<<<<
  * 
  *     for i in range(n):
  */
     __pyx_v_result = __pyx_f_7brainpy_2_c_21isotopic_distribution_make_peak_list();
 
-    /* "brainpy/_c/isotopic_distribution.pyx":180
+    /* "brainpy/_c/isotopic_distribution.pyx":192
  *     n = peaklist.used
  * 
  *     if result == NULL:             # <<<<<<<<<<<<<<
  *         result = make_peak_list()
  * 
  */
   }
 
-  /* "brainpy/_c/isotopic_distribution.pyx":183
+  /* "brainpy/_c/isotopic_distribution.pyx":195
  *         result = make_peak_list()
  * 
  *     for i in range(n):             # <<<<<<<<<<<<<<
  *         p = result.peaks[i]
  *         if (p.intensity < ignore_below) and (i > 1):
  */
   __pyx_t_1 = __pyx_v_n;
   __pyx_t_3 = __pyx_t_1;
   for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
     __pyx_v_i = __pyx_t_4;
 
-    /* "brainpy/_c/isotopic_distribution.pyx":184
+    /* "brainpy/_c/isotopic_distribution.pyx":196
  * 
  *     for i in range(n):
  *         p = result.peaks[i]             # <<<<<<<<<<<<<<
  *         if (p.intensity < ignore_below) and (i > 1):
  *             continue
  */
     __pyx_v_p = (__pyx_v_result->peaks[__pyx_v_i]);
 
-    /* "brainpy/_c/isotopic_distribution.pyx":185
+    /* "brainpy/_c/isotopic_distribution.pyx":197
  *     for i in range(n):
  *         p = result.peaks[i]
  *         if (p.intensity < ignore_below) and (i > 1):             # <<<<<<<<<<<<<<
  *             continue
  *         else:
  */
     __pyx_t_5 = ((__pyx_v_p.intensity < __pyx_v_ignore_below) != 0);
@@ -2974,111 +2974,111 @@
       goto __pyx_L7_bool_binop_done;
     }
     __pyx_t_5 = ((__pyx_v_i > 1) != 0);
     __pyx_t_2 = __pyx_t_5;
     __pyx_L7_bool_binop_done:;
     if (__pyx_t_2) {
 
-      /* "brainpy/_c/isotopic_distribution.pyx":186
+      /* "brainpy/_c/isotopic_distribution.pyx":198
  *         p = result.peaks[i]
  *         if (p.intensity < ignore_below) and (i > 1):
  *             continue             # <<<<<<<<<<<<<<
  *         else:
  *             total += p.intensity
  */
       goto __pyx_L4_continue;
 
-      /* "brainpy/_c/isotopic_distribution.pyx":185
+      /* "brainpy/_c/isotopic_distribution.pyx":197
  *     for i in range(n):
  *         p = result.peaks[i]
  *         if (p.intensity < ignore_below) and (i > 1):             # <<<<<<<<<<<<<<
  *             continue
  *         else:
  */
     }
 
-    /* "brainpy/_c/isotopic_distribution.pyx":188
+    /* "brainpy/_c/isotopic_distribution.pyx":200
  *             continue
  *         else:
  *             total += p.intensity             # <<<<<<<<<<<<<<
  *         peak_list_append(result, &p)
  *     n = result.used
  */
     /*else*/ {
       __pyx_v_total = (__pyx_v_total + __pyx_v_p.intensity);
     }
 
-    /* "brainpy/_c/isotopic_distribution.pyx":189
+    /* "brainpy/_c/isotopic_distribution.pyx":201
  *         else:
  *             total += p.intensity
  *         peak_list_append(result, &p)             # <<<<<<<<<<<<<<
  *     n = result.used
  *     for i in range(n):
  */
     __pyx_f_7brainpy_2_c_21isotopic_distribution_peak_list_append(__pyx_v_result, (&__pyx_v_p));
     __pyx_L4_continue:;
   }
 
-  /* "brainpy/_c/isotopic_distribution.pyx":190
+  /* "brainpy/_c/isotopic_distribution.pyx":202
  *             total += p.intensity
  *         peak_list_append(result, &p)
  *     n = result.used             # <<<<<<<<<<<<<<
  *     for i in range(n):
  *         result.peaks[i].intensity /= total
  */
   __pyx_t_1 = __pyx_v_result->used;
   __pyx_v_n = __pyx_t_1;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":191
+  /* "brainpy/_c/isotopic_distribution.pyx":203
  *         peak_list_append(result, &p)
  *     n = result.used
  *     for i in range(n):             # <<<<<<<<<<<<<<
  *         result.peaks[i].intensity /= total
  *     return result
  */
   __pyx_t_1 = __pyx_v_n;
   __pyx_t_3 = __pyx_t_1;
   for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
     __pyx_v_i = __pyx_t_4;
 
-    /* "brainpy/_c/isotopic_distribution.pyx":192
+    /* "brainpy/_c/isotopic_distribution.pyx":204
  *     n = result.used
  *     for i in range(n):
  *         result.peaks[i].intensity /= total             # <<<<<<<<<<<<<<
  *     return result
  * 
  */
     __pyx_t_6 = __pyx_v_i;
     (__pyx_v_result->peaks[__pyx_t_6]).intensity = ((__pyx_v_result->peaks[__pyx_t_6]).intensity / __pyx_v_total);
   }
 
-  /* "brainpy/_c/isotopic_distribution.pyx":193
+  /* "brainpy/_c/isotopic_distribution.pyx":205
  *     for i in range(n):
  *         result.peaks[i].intensity /= total
  *     return result             # <<<<<<<<<<<<<<
  * 
  * @cython.cdivision
  */
   __pyx_r = __pyx_v_result;
   goto __pyx_L0;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":170
+  /* "brainpy/_c/isotopic_distribution.pyx":182
  * 
  * @cython.cdivision
  * cdef PeakList* peak_list_ignore_below(PeakList* peaklist, double ignore_below, PeakList* result) nogil:             # <<<<<<<<<<<<<<
  *     cdef:
  *         double total
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "brainpy/_c/isotopic_distribution.pyx":196
+/* "brainpy/_c/isotopic_distribution.pyx":208
  * 
  * @cython.cdivision
  * cdef PeakList* peak_list_truncate_after(PeakList* peaklist, double truncate_after, PeakList* result) nogil:             # <<<<<<<<<<<<<<
  *     cdef:
  *         double cumsum
  */
 
@@ -3090,187 +3090,187 @@
   struct __pyx_t_7brainpy_2_c_21isotopic_distribution_PeakList *__pyx_r;
   size_t __pyx_t_1;
   int __pyx_t_2;
   size_t __pyx_t_3;
   size_t __pyx_t_4;
   size_t __pyx_t_5;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":202
+  /* "brainpy/_c/isotopic_distribution.pyx":214
  *         size_t i, n
  * 
  *     cumsum = 0             # <<<<<<<<<<<<<<
  *     n = peaklist.used
  *     if result == NULL:
  */
   __pyx_v_cumsum = 0.0;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":203
+  /* "brainpy/_c/isotopic_distribution.pyx":215
  * 
  *     cumsum = 0
  *     n = peaklist.used             # <<<<<<<<<<<<<<
  *     if result == NULL:
  *         result = make_peak_list()
  */
   __pyx_t_1 = __pyx_v_peaklist->used;
   __pyx_v_n = __pyx_t_1;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":204
+  /* "brainpy/_c/isotopic_distribution.pyx":216
  *     cumsum = 0
  *     n = peaklist.used
  *     if result == NULL:             # <<<<<<<<<<<<<<
  *         result = make_peak_list()
  * 
  */
   __pyx_t_2 = ((__pyx_v_result == NULL) != 0);
   if (__pyx_t_2) {
 
-    /* "brainpy/_c/isotopic_distribution.pyx":205
+    /* "brainpy/_c/isotopic_distribution.pyx":217
  *     n = peaklist.used
  *     if result == NULL:
  *         result = make_peak_list()             # <<<<<<<<<<<<<<
  * 
  *     for i in range(n):
  */
     __pyx_v_result = __pyx_f_7brainpy_2_c_21isotopic_distribution_make_peak_list();
 
-    /* "brainpy/_c/isotopic_distribution.pyx":204
+    /* "brainpy/_c/isotopic_distribution.pyx":216
  *     cumsum = 0
  *     n = peaklist.used
  *     if result == NULL:             # <<<<<<<<<<<<<<
  *         result = make_peak_list()
  * 
  */
   }
 
-  /* "brainpy/_c/isotopic_distribution.pyx":207
+  /* "brainpy/_c/isotopic_distribution.pyx":219
  *         result = make_peak_list()
  * 
  *     for i in range(n):             # <<<<<<<<<<<<<<
  *         peak = peaklist.peaks[i]
  *         cumsum += peak.intensity
  */
   __pyx_t_1 = __pyx_v_n;
   __pyx_t_3 = __pyx_t_1;
   for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
     __pyx_v_i = __pyx_t_4;
 
-    /* "brainpy/_c/isotopic_distribution.pyx":208
+    /* "brainpy/_c/isotopic_distribution.pyx":220
  * 
  *     for i in range(n):
  *         peak = peaklist.peaks[i]             # <<<<<<<<<<<<<<
  *         cumsum += peak.intensity
  *         peak_list_append(result, &peak)
  */
     __pyx_v_peak = (__pyx_v_peaklist->peaks[__pyx_v_i]);
 
-    /* "brainpy/_c/isotopic_distribution.pyx":209
+    /* "brainpy/_c/isotopic_distribution.pyx":221
  *     for i in range(n):
  *         peak = peaklist.peaks[i]
  *         cumsum += peak.intensity             # <<<<<<<<<<<<<<
  *         peak_list_append(result, &peak)
  *         if cumsum >= truncate_after:
  */
     __pyx_v_cumsum = (__pyx_v_cumsum + __pyx_v_peak.intensity);
 
-    /* "brainpy/_c/isotopic_distribution.pyx":210
+    /* "brainpy/_c/isotopic_distribution.pyx":222
  *         peak = peaklist.peaks[i]
  *         cumsum += peak.intensity
  *         peak_list_append(result, &peak)             # <<<<<<<<<<<<<<
  *         if cumsum >= truncate_after:
  *             break
  */
     __pyx_f_7brainpy_2_c_21isotopic_distribution_peak_list_append(__pyx_v_result, (&__pyx_v_peak));
 
-    /* "brainpy/_c/isotopic_distribution.pyx":211
+    /* "brainpy/_c/isotopic_distribution.pyx":223
  *         cumsum += peak.intensity
  *         peak_list_append(result, &peak)
  *         if cumsum >= truncate_after:             # <<<<<<<<<<<<<<
  *             break
  * 
  */
     __pyx_t_2 = ((__pyx_v_cumsum >= __pyx_v_truncate_after) != 0);
     if (__pyx_t_2) {
 
-      /* "brainpy/_c/isotopic_distribution.pyx":212
+      /* "brainpy/_c/isotopic_distribution.pyx":224
  *         peak_list_append(result, &peak)
  *         if cumsum >= truncate_after:
  *             break             # <<<<<<<<<<<<<<
  * 
  *     n = result.used
  */
       goto __pyx_L5_break;
 
-      /* "brainpy/_c/isotopic_distribution.pyx":211
+      /* "brainpy/_c/isotopic_distribution.pyx":223
  *         cumsum += peak.intensity
  *         peak_list_append(result, &peak)
  *         if cumsum >= truncate_after:             # <<<<<<<<<<<<<<
  *             break
  * 
  */
     }
   }
   __pyx_L5_break:;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":214
+  /* "brainpy/_c/isotopic_distribution.pyx":226
  *             break
  * 
  *     n = result.used             # <<<<<<<<<<<<<<
  *     for i in range(n):
  *         result.peaks[i].intensity /= cumsum
  */
   __pyx_t_1 = __pyx_v_result->used;
   __pyx_v_n = __pyx_t_1;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":215
+  /* "brainpy/_c/isotopic_distribution.pyx":227
  * 
  *     n = result.used
  *     for i in range(n):             # <<<<<<<<<<<<<<
  *         result.peaks[i].intensity /= cumsum
  *     return result
  */
   __pyx_t_1 = __pyx_v_n;
   __pyx_t_3 = __pyx_t_1;
   for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
     __pyx_v_i = __pyx_t_4;
 
-    /* "brainpy/_c/isotopic_distribution.pyx":216
+    /* "brainpy/_c/isotopic_distribution.pyx":228
  *     n = result.used
  *     for i in range(n):
  *         result.peaks[i].intensity /= cumsum             # <<<<<<<<<<<<<<
  *     return result
  * 
  */
     __pyx_t_5 = __pyx_v_i;
     (__pyx_v_result->peaks[__pyx_t_5]).intensity = ((__pyx_v_result->peaks[__pyx_t_5]).intensity / __pyx_v_cumsum);
   }
 
-  /* "brainpy/_c/isotopic_distribution.pyx":217
+  /* "brainpy/_c/isotopic_distribution.pyx":229
  *     for i in range(n):
  *         result.peaks[i].intensity /= cumsum
  *     return result             # <<<<<<<<<<<<<<
  * 
  * cdef void peak_list_shift(PeakList* peaklist, double shift) nogil:
  */
   __pyx_r = __pyx_v_result;
   goto __pyx_L0;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":196
+  /* "brainpy/_c/isotopic_distribution.pyx":208
  * 
  * @cython.cdivision
  * cdef PeakList* peak_list_truncate_after(PeakList* peaklist, double truncate_after, PeakList* result) nogil:             # <<<<<<<<<<<<<<
  *     cdef:
  *         double cumsum
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "brainpy/_c/isotopic_distribution.pyx":219
+/* "brainpy/_c/isotopic_distribution.pyx":231
  *     return result
  * 
  * cdef void peak_list_shift(PeakList* peaklist, double shift) nogil:             # <<<<<<<<<<<<<<
  *     cdef:
  *         size_t i, n
  */
 
@@ -3280,408 +3280,408 @@
   double __pyx_v_delta;
   size_t __pyx_t_1;
   int __pyx_t_2;
   size_t __pyx_t_3;
   size_t __pyx_t_4;
   size_t __pyx_t_5;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":224
+  /* "brainpy/_c/isotopic_distribution.pyx":236
  *         double delta
  * 
  *     n = peaklist.used             # <<<<<<<<<<<<<<
  *     if n == 0:
  *         return
  */
   __pyx_t_1 = __pyx_v_peaklist->used;
   __pyx_v_n = __pyx_t_1;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":225
+  /* "brainpy/_c/isotopic_distribution.pyx":237
  * 
  *     n = peaklist.used
  *     if n == 0:             # <<<<<<<<<<<<<<
  *         return
  *     delta = shift - peaklist.peaks[0].mz
  */
   __pyx_t_2 = ((__pyx_v_n == 0) != 0);
   if (__pyx_t_2) {
 
-    /* "brainpy/_c/isotopic_distribution.pyx":226
+    /* "brainpy/_c/isotopic_distribution.pyx":238
  *     n = peaklist.used
  *     if n == 0:
  *         return             # <<<<<<<<<<<<<<
  *     delta = shift - peaklist.peaks[0].mz
  *     for i in range(n):
  */
     goto __pyx_L0;
 
-    /* "brainpy/_c/isotopic_distribution.pyx":225
+    /* "brainpy/_c/isotopic_distribution.pyx":237
  * 
  *     n = peaklist.used
  *     if n == 0:             # <<<<<<<<<<<<<<
  *         return
  *     delta = shift - peaklist.peaks[0].mz
  */
   }
 
-  /* "brainpy/_c/isotopic_distribution.pyx":227
+  /* "brainpy/_c/isotopic_distribution.pyx":239
  *     if n == 0:
  *         return
  *     delta = shift - peaklist.peaks[0].mz             # <<<<<<<<<<<<<<
  *     for i in range(n):
  *         peaklist.peaks[i].mz += delta
  */
   __pyx_v_delta = (__pyx_v_shift - (__pyx_v_peaklist->peaks[0]).mz);
 
-  /* "brainpy/_c/isotopic_distribution.pyx":228
+  /* "brainpy/_c/isotopic_distribution.pyx":240
  *         return
  *     delta = shift - peaklist.peaks[0].mz
  *     for i in range(n):             # <<<<<<<<<<<<<<
  *         peaklist.peaks[i].mz += delta
  * 
  */
   __pyx_t_1 = __pyx_v_n;
   __pyx_t_3 = __pyx_t_1;
   for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
     __pyx_v_i = __pyx_t_4;
 
-    /* "brainpy/_c/isotopic_distribution.pyx":229
+    /* "brainpy/_c/isotopic_distribution.pyx":241
  *     delta = shift - peaklist.peaks[0].mz
  *     for i in range(n):
  *         peaklist.peaks[i].mz += delta             # <<<<<<<<<<<<<<
  * 
  * # -----------------------------------------------------------------------------
  */
     __pyx_t_5 = __pyx_v_i;
     (__pyx_v_peaklist->peaks[__pyx_t_5]).mz = ((__pyx_v_peaklist->peaks[__pyx_t_5]).mz + __pyx_v_delta);
   }
 
-  /* "brainpy/_c/isotopic_distribution.pyx":219
+  /* "brainpy/_c/isotopic_distribution.pyx":231
  *     return result
  * 
  * cdef void peak_list_shift(PeakList* peaklist, double shift) nogil:             # <<<<<<<<<<<<<<
  *     cdef:
  *         size_t i, n
  */
 
   /* function exit code */
   __pyx_L0:;
 }
 
-/* "brainpy/_c/isotopic_distribution.pyx":234
+/* "brainpy/_c/isotopic_distribution.pyx":246
  * # ElementCache Methods
  * 
  * cdef ElementCache* make_element_cache(ElementHashTable* source) nogil:             # <<<<<<<<<<<<<<
  *     cdef:
  *         ElementCache* cache
  */
 
 static struct __pyx_t_7brainpy_2_c_21isotopic_distribution_ElementCache *__pyx_f_7brainpy_2_c_21isotopic_distribution_make_element_cache(struct __pyx_t_7brainpy_2_c_11composition_ElementHashTable *__pyx_v_source) {
   struct __pyx_t_7brainpy_2_c_21isotopic_distribution_ElementCache *__pyx_v_cache;
   struct __pyx_t_7brainpy_2_c_21isotopic_distribution_ElementCache *__pyx_r;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":237
+  /* "brainpy/_c/isotopic_distribution.pyx":249
  *     cdef:
  *         ElementCache* cache
  *     cache = <ElementCache*>malloc(sizeof(ElementCache))             # <<<<<<<<<<<<<<
  *     cache.source = source
  *     cache.elements = <Element**>malloc(sizeof(Element*) * 10)
  */
   __pyx_v_cache = ((struct __pyx_t_7brainpy_2_c_21isotopic_distribution_ElementCache *)malloc((sizeof(struct __pyx_t_7brainpy_2_c_21isotopic_distribution_ElementCache))));
 
-  /* "brainpy/_c/isotopic_distribution.pyx":238
+  /* "brainpy/_c/isotopic_distribution.pyx":250
  *         ElementCache* cache
  *     cache = <ElementCache*>malloc(sizeof(ElementCache))
  *     cache.source = source             # <<<<<<<<<<<<<<
  *     cache.elements = <Element**>malloc(sizeof(Element*) * 10)
  *     cache.used = 0
  */
   __pyx_v_cache->source = __pyx_v_source;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":239
+  /* "brainpy/_c/isotopic_distribution.pyx":251
  *     cache = <ElementCache*>malloc(sizeof(ElementCache))
  *     cache.source = source
  *     cache.elements = <Element**>malloc(sizeof(Element*) * 10)             # <<<<<<<<<<<<<<
  *     cache.used = 0
  *     cache.size = 10
  */
   __pyx_v_cache->elements = ((struct __pyx_t_7brainpy_2_c_11composition_Element **)malloc(((sizeof(struct __pyx_t_7brainpy_2_c_11composition_Element *)) * 10)));
 
-  /* "brainpy/_c/isotopic_distribution.pyx":240
+  /* "brainpy/_c/isotopic_distribution.pyx":252
  *     cache.source = source
  *     cache.elements = <Element**>malloc(sizeof(Element*) * 10)
  *     cache.used = 0             # <<<<<<<<<<<<<<
  *     cache.size = 10
  *     return cache
  */
   __pyx_v_cache->used = 0;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":241
+  /* "brainpy/_c/isotopic_distribution.pyx":253
  *     cache.elements = <Element**>malloc(sizeof(Element*) * 10)
  *     cache.used = 0
  *     cache.size = 10             # <<<<<<<<<<<<<<
  *     return cache
  * 
  */
   __pyx_v_cache->size = 10;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":242
+  /* "brainpy/_c/isotopic_distribution.pyx":254
  *     cache.used = 0
  *     cache.size = 10
  *     return cache             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = __pyx_v_cache;
   goto __pyx_L0;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":234
+  /* "brainpy/_c/isotopic_distribution.pyx":246
  * # ElementCache Methods
  * 
  * cdef ElementCache* make_element_cache(ElementHashTable* source) nogil:             # <<<<<<<<<<<<<<
  *     cdef:
  *         ElementCache* cache
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "brainpy/_c/isotopic_distribution.pyx":245
+/* "brainpy/_c/isotopic_distribution.pyx":257
  * 
  * 
  * cdef void free_element_cache(ElementCache* cache) nogil:             # <<<<<<<<<<<<<<
  *     free(cache.elements)
  *     free(cache)
  */
 
 static void __pyx_f_7brainpy_2_c_21isotopic_distribution_free_element_cache(struct __pyx_t_7brainpy_2_c_21isotopic_distribution_ElementCache *__pyx_v_cache) {
 
-  /* "brainpy/_c/isotopic_distribution.pyx":246
+  /* "brainpy/_c/isotopic_distribution.pyx":258
  * 
  * cdef void free_element_cache(ElementCache* cache) nogil:
  *     free(cache.elements)             # <<<<<<<<<<<<<<
  *     free(cache)
  * 
  */
   free(__pyx_v_cache->elements);
 
-  /* "brainpy/_c/isotopic_distribution.pyx":247
+  /* "brainpy/_c/isotopic_distribution.pyx":259
  * cdef void free_element_cache(ElementCache* cache) nogil:
  *     free(cache.elements)
  *     free(cache)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   free(__pyx_v_cache);
 
-  /* "brainpy/_c/isotopic_distribution.pyx":245
+  /* "brainpy/_c/isotopic_distribution.pyx":257
  * 
  * 
  * cdef void free_element_cache(ElementCache* cache) nogil:             # <<<<<<<<<<<<<<
  *     free(cache.elements)
  *     free(cache)
  */
 
   /* function exit code */
 }
 
-/* "brainpy/_c/isotopic_distribution.pyx":250
+/* "brainpy/_c/isotopic_distribution.pyx":262
  * 
  * 
  * cdef int resize_element_cache(ElementCache* cache) nogil:             # <<<<<<<<<<<<<<
  *     cdef:
  *         Element** values
  */
 
 static int __pyx_f_7brainpy_2_c_21isotopic_distribution_resize_element_cache(struct __pyx_t_7brainpy_2_c_21isotopic_distribution_ElementCache *__pyx_v_cache) {
   struct __pyx_t_7brainpy_2_c_11composition_Element **__pyx_v_values;
   size_t __pyx_v_new_size;
   int __pyx_r;
   int __pyx_t_1;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":254
+  /* "brainpy/_c/isotopic_distribution.pyx":266
  *         Element** values
  *         size_t new_size
  *     new_size = cache.size * 10             # <<<<<<<<<<<<<<
  *     values = <Element**>realloc(cache.elements, sizeof(Element*) * new_size)
  *     if values == NULL:
  */
   __pyx_v_new_size = (__pyx_v_cache->size * 10);
 
-  /* "brainpy/_c/isotopic_distribution.pyx":255
+  /* "brainpy/_c/isotopic_distribution.pyx":267
  *         size_t new_size
  *     new_size = cache.size * 10
  *     values = <Element**>realloc(cache.elements, sizeof(Element*) * new_size)             # <<<<<<<<<<<<<<
  *     if values == NULL:
  *         printf("resize_element_cache returned -1\n")
  */
   __pyx_v_values = ((struct __pyx_t_7brainpy_2_c_11composition_Element **)realloc(__pyx_v_cache->elements, ((sizeof(struct __pyx_t_7brainpy_2_c_11composition_Element *)) * __pyx_v_new_size)));
 
-  /* "brainpy/_c/isotopic_distribution.pyx":256
+  /* "brainpy/_c/isotopic_distribution.pyx":268
  *     new_size = cache.size * 10
  *     values = <Element**>realloc(cache.elements, sizeof(Element*) * new_size)
  *     if values == NULL:             # <<<<<<<<<<<<<<
  *         printf("resize_element_cache returned -1\n")
  *         return -1
  */
   __pyx_t_1 = ((__pyx_v_values == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "brainpy/_c/isotopic_distribution.pyx":257
+    /* "brainpy/_c/isotopic_distribution.pyx":269
  *     values = <Element**>realloc(cache.elements, sizeof(Element*) * new_size)
  *     if values == NULL:
  *         printf("resize_element_cache returned -1\n")             # <<<<<<<<<<<<<<
  *         return -1
  *     cache.elements = values
  */
     (void)(printf(((char const *)"resize_element_cache returned -1\n")));
 
-    /* "brainpy/_c/isotopic_distribution.pyx":258
+    /* "brainpy/_c/isotopic_distribution.pyx":270
  *     if values == NULL:
  *         printf("resize_element_cache returned -1\n")
  *         return -1             # <<<<<<<<<<<<<<
  *     cache.elements = values
  *     cache.size = new_size
  */
     __pyx_r = -1;
     goto __pyx_L0;
 
-    /* "brainpy/_c/isotopic_distribution.pyx":256
+    /* "brainpy/_c/isotopic_distribution.pyx":268
  *     new_size = cache.size * 10
  *     values = <Element**>realloc(cache.elements, sizeof(Element*) * new_size)
  *     if values == NULL:             # <<<<<<<<<<<<<<
  *         printf("resize_element_cache returned -1\n")
  *         return -1
  */
   }
 
-  /* "brainpy/_c/isotopic_distribution.pyx":259
+  /* "brainpy/_c/isotopic_distribution.pyx":271
  *         printf("resize_element_cache returned -1\n")
  *         return -1
  *     cache.elements = values             # <<<<<<<<<<<<<<
  *     cache.size = new_size
  *     return 0
  */
   __pyx_v_cache->elements = __pyx_v_values;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":260
+  /* "brainpy/_c/isotopic_distribution.pyx":272
  *         return -1
  *     cache.elements = values
  *     cache.size = new_size             # <<<<<<<<<<<<<<
  *     return 0
  * 
  */
   __pyx_v_cache->size = __pyx_v_new_size;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":261
+  /* "brainpy/_c/isotopic_distribution.pyx":273
  *     cache.elements = values
  *     cache.size = new_size
  *     return 0             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = 0;
   goto __pyx_L0;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":250
+  /* "brainpy/_c/isotopic_distribution.pyx":262
  * 
  * 
  * cdef int resize_element_cache(ElementCache* cache) nogil:             # <<<<<<<<<<<<<<
  *     cdef:
  *         Element** values
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "brainpy/_c/isotopic_distribution.pyx":264
+/* "brainpy/_c/isotopic_distribution.pyx":276
  * 
  * 
  * cdef int element_cache_put(ElementCache* cache, Element** element) nogil:             # <<<<<<<<<<<<<<
  *     cdef:
  *         size_t i
  */
 
 static int __pyx_f_7brainpy_2_c_21isotopic_distribution_element_cache_put(struct __pyx_t_7brainpy_2_c_21isotopic_distribution_ElementCache *__pyx_v_cache, struct __pyx_t_7brainpy_2_c_11composition_Element **__pyx_v_element) {
   int __pyx_r;
   int __pyx_t_1;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":267
+  /* "brainpy/_c/isotopic_distribution.pyx":279
  *     cdef:
  *         size_t i
  *     if (cache.used + 1) == cache.size:             # <<<<<<<<<<<<<<
  *         resize_element_cache(cache)
  *     cache.elements[cache.used] = element[0]
  */
   __pyx_t_1 = (((__pyx_v_cache->used + 1) == __pyx_v_cache->size) != 0);
   if (__pyx_t_1) {
 
-    /* "brainpy/_c/isotopic_distribution.pyx":268
+    /* "brainpy/_c/isotopic_distribution.pyx":280
  *         size_t i
  *     if (cache.used + 1) == cache.size:
  *         resize_element_cache(cache)             # <<<<<<<<<<<<<<
  *     cache.elements[cache.used] = element[0]
  *     cache.used += 1
  */
     (void)(__pyx_f_7brainpy_2_c_21isotopic_distribution_resize_element_cache(__pyx_v_cache));
 
-    /* "brainpy/_c/isotopic_distribution.pyx":267
+    /* "brainpy/_c/isotopic_distribution.pyx":279
  *     cdef:
  *         size_t i
  *     if (cache.used + 1) == cache.size:             # <<<<<<<<<<<<<<
  *         resize_element_cache(cache)
  *     cache.elements[cache.used] = element[0]
  */
   }
 
-  /* "brainpy/_c/isotopic_distribution.pyx":269
+  /* "brainpy/_c/isotopic_distribution.pyx":281
  *     if (cache.used + 1) == cache.size:
  *         resize_element_cache(cache)
  *     cache.elements[cache.used] = element[0]             # <<<<<<<<<<<<<<
  *     cache.used += 1
  *     return 0
  */
   (__pyx_v_cache->elements[__pyx_v_cache->used]) = (__pyx_v_element[0]);
 
-  /* "brainpy/_c/isotopic_distribution.pyx":270
+  /* "brainpy/_c/isotopic_distribution.pyx":282
  *         resize_element_cache(cache)
  *     cache.elements[cache.used] = element[0]
  *     cache.used += 1             # <<<<<<<<<<<<<<
  *     return 0
  * 
  */
   __pyx_v_cache->used = (__pyx_v_cache->used + 1);
 
-  /* "brainpy/_c/isotopic_distribution.pyx":271
+  /* "brainpy/_c/isotopic_distribution.pyx":283
  *     cache.elements[cache.used] = element[0]
  *     cache.used += 1
  *     return 0             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = 0;
   goto __pyx_L0;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":264
+  /* "brainpy/_c/isotopic_distribution.pyx":276
  * 
  * 
  * cdef int element_cache_put(ElementCache* cache, Element** element) nogil:             # <<<<<<<<<<<<<<
  *     cdef:
  *         size_t i
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "brainpy/_c/isotopic_distribution.pyx":274
+/* "brainpy/_c/isotopic_distribution.pyx":286
  * 
  * 
  * cdef int element_cache_get(ElementCache* cache, char* symbol, Element** out) nogil:             # <<<<<<<<<<<<<<
  *     cdef:
  *         size_t i
  */
 
@@ -3690,145 +3690,145 @@
   struct __pyx_t_7brainpy_2_c_11composition_Element *__pyx_v_element;
   int __pyx_r;
   int __pyx_t_1;
   size_t __pyx_t_2;
   size_t __pyx_t_3;
   size_t __pyx_t_4;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":279
+  /* "brainpy/_c/isotopic_distribution.pyx":291
  *         Element* element
  * 
  *     if cache == NULL:             # <<<<<<<<<<<<<<
  *         return element_hash_table_get(_ElementTable, symbol, out)
  * 
  */
   __pyx_t_1 = ((__pyx_v_cache == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "brainpy/_c/isotopic_distribution.pyx":280
+    /* "brainpy/_c/isotopic_distribution.pyx":292
  * 
  *     if cache == NULL:
  *         return element_hash_table_get(_ElementTable, symbol, out)             # <<<<<<<<<<<<<<
  * 
  *     for i in range(cache.used):
  */
     __pyx_r = __pyx_f_7brainpy_2_c_11composition_element_hash_table_get(__pyx_v_7brainpy_2_c_11composition__ElementTable, __pyx_v_symbol, __pyx_v_out);
     goto __pyx_L0;
 
-    /* "brainpy/_c/isotopic_distribution.pyx":279
+    /* "brainpy/_c/isotopic_distribution.pyx":291
  *         Element* element
  * 
  *     if cache == NULL:             # <<<<<<<<<<<<<<
  *         return element_hash_table_get(_ElementTable, symbol, out)
  * 
  */
   }
 
-  /* "brainpy/_c/isotopic_distribution.pyx":282
+  /* "brainpy/_c/isotopic_distribution.pyx":294
  *         return element_hash_table_get(_ElementTable, symbol, out)
  * 
  *     for i in range(cache.used):             # <<<<<<<<<<<<<<
  *         element = cache.elements[i]
  *         if strcmp(element.symbol, symbol) == 0:
  */
   __pyx_t_2 = __pyx_v_cache->used;
   __pyx_t_3 = __pyx_t_2;
   for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
     __pyx_v_i = __pyx_t_4;
 
-    /* "brainpy/_c/isotopic_distribution.pyx":283
+    /* "brainpy/_c/isotopic_distribution.pyx":295
  * 
  *     for i in range(cache.used):
  *         element = cache.elements[i]             # <<<<<<<<<<<<<<
  *         if strcmp(element.symbol, symbol) == 0:
  *             out[0] = element
  */
     __pyx_v_element = (__pyx_v_cache->elements[__pyx_v_i]);
 
-    /* "brainpy/_c/isotopic_distribution.pyx":284
+    /* "brainpy/_c/isotopic_distribution.pyx":296
  *     for i in range(cache.used):
  *         element = cache.elements[i]
  *         if strcmp(element.symbol, symbol) == 0:             # <<<<<<<<<<<<<<
  *             out[0] = element
  *             return 0
  */
     __pyx_t_1 = ((strcmp(__pyx_v_element->symbol, __pyx_v_symbol) == 0) != 0);
     if (__pyx_t_1) {
 
-      /* "brainpy/_c/isotopic_distribution.pyx":285
+      /* "brainpy/_c/isotopic_distribution.pyx":297
  *         element = cache.elements[i]
  *         if strcmp(element.symbol, symbol) == 0:
  *             out[0] = element             # <<<<<<<<<<<<<<
  *             return 0
  *     element_hash_table_get(cache.source, symbol, out)
  */
       (__pyx_v_out[0]) = __pyx_v_element;
 
-      /* "brainpy/_c/isotopic_distribution.pyx":286
+      /* "brainpy/_c/isotopic_distribution.pyx":298
  *         if strcmp(element.symbol, symbol) == 0:
  *             out[0] = element
  *             return 0             # <<<<<<<<<<<<<<
  *     element_hash_table_get(cache.source, symbol, out)
  *     element_cache_put(cache, out)
  */
       __pyx_r = 0;
       goto __pyx_L0;
 
-      /* "brainpy/_c/isotopic_distribution.pyx":284
+      /* "brainpy/_c/isotopic_distribution.pyx":296
  *     for i in range(cache.used):
  *         element = cache.elements[i]
  *         if strcmp(element.symbol, symbol) == 0:             # <<<<<<<<<<<<<<
  *             out[0] = element
  *             return 0
  */
     }
   }
 
-  /* "brainpy/_c/isotopic_distribution.pyx":287
+  /* "brainpy/_c/isotopic_distribution.pyx":299
  *             out[0] = element
  *             return 0
  *     element_hash_table_get(cache.source, symbol, out)             # <<<<<<<<<<<<<<
  *     element_cache_put(cache, out)
  *     return 1
  */
   (void)(__pyx_f_7brainpy_2_c_11composition_element_hash_table_get(__pyx_v_cache->source, __pyx_v_symbol, __pyx_v_out));
 
-  /* "brainpy/_c/isotopic_distribution.pyx":288
+  /* "brainpy/_c/isotopic_distribution.pyx":300
  *             return 0
  *     element_hash_table_get(cache.source, symbol, out)
  *     element_cache_put(cache, out)             # <<<<<<<<<<<<<<
  *     return 1
  * 
  */
   (void)(__pyx_f_7brainpy_2_c_21isotopic_distribution_element_cache_put(__pyx_v_cache, __pyx_v_out));
 
-  /* "brainpy/_c/isotopic_distribution.pyx":289
+  /* "brainpy/_c/isotopic_distribution.pyx":301
  *     element_hash_table_get(cache.source, symbol, out)
  *     element_cache_put(cache, out)
  *     return 1             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = 1;
   goto __pyx_L0;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":274
+  /* "brainpy/_c/isotopic_distribution.pyx":286
  * 
  * 
  * cdef int element_cache_get(ElementCache* cache, char* symbol, Element** out) nogil:             # <<<<<<<<<<<<<<
  *     cdef:
  *         size_t i
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "brainpy/_c/isotopic_distribution.pyx":295
+/* "brainpy/_c/isotopic_distribution.pyx":307
  * # Support Functions
  * 
  * cdef int max_variants(Composition* composition, ElementCache* cache) nogil:             # <<<<<<<<<<<<<<
  *     cdef:
  *         size_t i
  */
 
@@ -3840,166 +3840,166 @@
   struct __pyx_t_7brainpy_2_c_11composition_Element *__pyx_v_element;
   int __pyx_r;
   int __pyx_t_1;
   size_t __pyx_t_2;
   size_t __pyx_t_3;
   size_t __pyx_t_4;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":303
+  /* "brainpy/_c/isotopic_distribution.pyx":315
  *         Element* element
  * 
  *     if composition.max_variants != 0:             # <<<<<<<<<<<<<<
  *         return composition.max_variants
  * 
  */
   __pyx_t_1 = ((__pyx_v_composition->max_variants != 0) != 0);
   if (__pyx_t_1) {
 
-    /* "brainpy/_c/isotopic_distribution.pyx":304
+    /* "brainpy/_c/isotopic_distribution.pyx":316
  * 
  *     if composition.max_variants != 0:
  *         return composition.max_variants             # <<<<<<<<<<<<<<
  * 
  *     max_variants = 0
  */
     __pyx_r = __pyx_v_composition->max_variants;
     goto __pyx_L0;
 
-    /* "brainpy/_c/isotopic_distribution.pyx":303
+    /* "brainpy/_c/isotopic_distribution.pyx":315
  *         Element* element
  * 
  *     if composition.max_variants != 0:             # <<<<<<<<<<<<<<
  *         return composition.max_variants
  * 
  */
   }
 
-  /* "brainpy/_c/isotopic_distribution.pyx":306
+  /* "brainpy/_c/isotopic_distribution.pyx":318
  *         return composition.max_variants
  * 
  *     max_variants = 0             # <<<<<<<<<<<<<<
  *     for i in range(composition.used):
  *         symbol = composition.elements[i]
  */
   __pyx_v_max_variants = 0;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":307
+  /* "brainpy/_c/isotopic_distribution.pyx":319
  * 
  *     max_variants = 0
  *     for i in range(composition.used):             # <<<<<<<<<<<<<<
  *         symbol = composition.elements[i]
  *         count = composition.counts[i]
  */
   __pyx_t_2 = __pyx_v_composition->used;
   __pyx_t_3 = __pyx_t_2;
   for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
     __pyx_v_i = __pyx_t_4;
 
-    /* "brainpy/_c/isotopic_distribution.pyx":308
+    /* "brainpy/_c/isotopic_distribution.pyx":320
  *     max_variants = 0
  *     for i in range(composition.used):
  *         symbol = composition.elements[i]             # <<<<<<<<<<<<<<
  *         count = composition.counts[i]
  *         if cache == NULL:
  */
     __pyx_v_symbol = (__pyx_v_composition->elements[__pyx_v_i]);
 
-    /* "brainpy/_c/isotopic_distribution.pyx":309
+    /* "brainpy/_c/isotopic_distribution.pyx":321
  *     for i in range(composition.used):
  *         symbol = composition.elements[i]
  *         count = composition.counts[i]             # <<<<<<<<<<<<<<
  *         if cache == NULL:
  *             element_hash_table_get(_ElementTable, symbol, &element)
  */
     __pyx_v_count = (__pyx_v_composition->counts[__pyx_v_i]);
 
-    /* "brainpy/_c/isotopic_distribution.pyx":310
+    /* "brainpy/_c/isotopic_distribution.pyx":322
  *         symbol = composition.elements[i]
  *         count = composition.counts[i]
  *         if cache == NULL:             # <<<<<<<<<<<<<<
  *             element_hash_table_get(_ElementTable, symbol, &element)
  *         else:
  */
     __pyx_t_1 = ((__pyx_v_cache == NULL) != 0);
     if (__pyx_t_1) {
 
-      /* "brainpy/_c/isotopic_distribution.pyx":311
+      /* "brainpy/_c/isotopic_distribution.pyx":323
  *         count = composition.counts[i]
  *         if cache == NULL:
  *             element_hash_table_get(_ElementTable, symbol, &element)             # <<<<<<<<<<<<<<
  *         else:
  *             element_cache_get(cache, symbol, &element)
  */
       (void)(__pyx_f_7brainpy_2_c_11composition_element_hash_table_get(__pyx_v_7brainpy_2_c_11composition__ElementTable, __pyx_v_symbol, (&__pyx_v_element)));
 
-      /* "brainpy/_c/isotopic_distribution.pyx":310
+      /* "brainpy/_c/isotopic_distribution.pyx":322
  *         symbol = composition.elements[i]
  *         count = composition.counts[i]
  *         if cache == NULL:             # <<<<<<<<<<<<<<
  *             element_hash_table_get(_ElementTable, symbol, &element)
  *         else:
  */
       goto __pyx_L6;
     }
 
-    /* "brainpy/_c/isotopic_distribution.pyx":313
+    /* "brainpy/_c/isotopic_distribution.pyx":325
  *             element_hash_table_get(_ElementTable, symbol, &element)
  *         else:
  *             element_cache_get(cache, symbol, &element)             # <<<<<<<<<<<<<<
  *         max_variants += <int>(count) * element_max_neutron_shift(element)
  *     composition.max_variants = max_variants
  */
     /*else*/ {
       (void)(__pyx_f_7brainpy_2_c_21isotopic_distribution_element_cache_get(__pyx_v_cache, __pyx_v_symbol, (&__pyx_v_element)));
     }
     __pyx_L6:;
 
-    /* "brainpy/_c/isotopic_distribution.pyx":314
+    /* "brainpy/_c/isotopic_distribution.pyx":326
  *         else:
  *             element_cache_get(cache, symbol, &element)
  *         max_variants += <int>(count) * element_max_neutron_shift(element)             # <<<<<<<<<<<<<<
  *     composition.max_variants = max_variants
  *     return max_variants
  */
     __pyx_v_max_variants = (__pyx_v_max_variants + (((int)__pyx_v_count) * __pyx_f_7brainpy_2_c_11composition_element_max_neutron_shift(__pyx_v_element)));
   }
 
-  /* "brainpy/_c/isotopic_distribution.pyx":315
+  /* "brainpy/_c/isotopic_distribution.pyx":327
  *             element_cache_get(cache, symbol, &element)
  *         max_variants += <int>(count) * element_max_neutron_shift(element)
  *     composition.max_variants = max_variants             # <<<<<<<<<<<<<<
  *     return max_variants
  * 
  */
   __pyx_v_composition->max_variants = __pyx_v_max_variants;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":316
+  /* "brainpy/_c/isotopic_distribution.pyx":328
  *         max_variants += <int>(count) * element_max_neutron_shift(element)
  *     composition.max_variants = max_variants
  *     return max_variants             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = __pyx_v_max_variants;
   goto __pyx_L0;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":295
+  /* "brainpy/_c/isotopic_distribution.pyx":307
  * # Support Functions
  * 
  * cdef int max_variants(Composition* composition, ElementCache* cache) nogil:             # <<<<<<<<<<<<<<
  *     cdef:
  *         size_t i
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "brainpy/_c/isotopic_distribution.pyx":319
+/* "brainpy/_c/isotopic_distribution.pyx":331
  * 
  * 
  * cdef int validate_composition(Composition* composition) nogil:             # <<<<<<<<<<<<<<
  *     cdef:
  *         size_t i
  */
 
@@ -4013,230 +4013,230 @@
   int __pyx_v_retcode;
   int __pyx_r;
   size_t __pyx_t_1;
   size_t __pyx_t_2;
   size_t __pyx_t_3;
   int __pyx_t_4;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":328
+  /* "brainpy/_c/isotopic_distribution.pyx":340
  *         int retcode
  * 
  *     retcode = 0             # <<<<<<<<<<<<<<
  *     for i in range(composition.used):
  *         element_symbol = composition.elements[i]
  */
   __pyx_v_retcode = 0;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":329
+  /* "brainpy/_c/isotopic_distribution.pyx":341
  * 
  *     retcode = 0
  *     for i in range(composition.used):             # <<<<<<<<<<<<<<
  *         element_symbol = composition.elements[i]
  *         status = element_hash_table_get(_ElementTable, element_symbol, &element)
  */
   __pyx_t_1 = __pyx_v_composition->used;
   __pyx_t_2 = __pyx_t_1;
   for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
     __pyx_v_i = __pyx_t_3;
 
-    /* "brainpy/_c/isotopic_distribution.pyx":330
+    /* "brainpy/_c/isotopic_distribution.pyx":342
  *     retcode = 0
  *     for i in range(composition.used):
  *         element_symbol = composition.elements[i]             # <<<<<<<<<<<<<<
  *         status = element_hash_table_get(_ElementTable, element_symbol, &element)
  *         # printf("Element %s, Status %d\n", element_symbol, status)
  */
     __pyx_v_element_symbol = (__pyx_v_composition->elements[__pyx_v_i]);
 
-    /* "brainpy/_c/isotopic_distribution.pyx":331
+    /* "brainpy/_c/isotopic_distribution.pyx":343
  *     for i in range(composition.used):
  *         element_symbol = composition.elements[i]
  *         status = element_hash_table_get(_ElementTable, element_symbol, &element)             # <<<<<<<<<<<<<<
  *         # printf("Element %s, Status %d\n", element_symbol, status)
  *         if status == -1:
  */
     __pyx_v_status = __pyx_f_7brainpy_2_c_11composition_element_hash_table_get(__pyx_v_7brainpy_2_c_11composition__ElementTable, __pyx_v_element_symbol, (&__pyx_v_element));
 
-    /* "brainpy/_c/isotopic_distribution.pyx":333
+    /* "brainpy/_c/isotopic_distribution.pyx":345
  *         status = element_hash_table_get(_ElementTable, element_symbol, &element)
  *         # printf("Element %s, Status %d\n", element_symbol, status)
  *         if status == -1:             # <<<<<<<<<<<<<<
  *             element_buffer = <char*>malloc(sizeof(char) * 10)
  *             # printf("Could not resolve element %s, attempting to generate fixed isotope\n", element_symbol)
  */
     __pyx_t_4 = ((__pyx_v_status == -1L) != 0);
     if (__pyx_t_4) {
 
-      /* "brainpy/_c/isotopic_distribution.pyx":334
+      /* "brainpy/_c/isotopic_distribution.pyx":346
  *         # printf("Element %s, Status %d\n", element_symbol, status)
  *         if status == -1:
  *             element_buffer = <char*>malloc(sizeof(char) * 10)             # <<<<<<<<<<<<<<
  *             # printf("Could not resolve element %s, attempting to generate fixed isotope\n", element_symbol)
  *             _parse_isotope_string(element_symbol, &isotope_number, element_buffer)
  */
       __pyx_v_element_buffer = ((char *)malloc(((sizeof(char)) * 10)));
 
-      /* "brainpy/_c/isotopic_distribution.pyx":336
+      /* "brainpy/_c/isotopic_distribution.pyx":348
  *             element_buffer = <char*>malloc(sizeof(char) * 10)
  *             # printf("Could not resolve element %s, attempting to generate fixed isotope\n", element_symbol)
  *             _parse_isotope_string(element_symbol, &isotope_number, element_buffer)             # <<<<<<<<<<<<<<
  *             # printf("Element: %s, Isotope: %d\n", element_buffer, isotope_number)
  *             if isotope_number != 0:
  */
       (void)(__pyx_f_7brainpy_2_c_11composition__parse_isotope_string(__pyx_v_element_symbol, (&__pyx_v_isotope_number), __pyx_v_element_buffer));
 
-      /* "brainpy/_c/isotopic_distribution.pyx":338
+      /* "brainpy/_c/isotopic_distribution.pyx":350
  *             _parse_isotope_string(element_symbol, &isotope_number, element_buffer)
  *             # printf("Element: %s, Isotope: %d\n", element_buffer, isotope_number)
  *             if isotope_number != 0:             # <<<<<<<<<<<<<<
  *                 status = element_hash_table_get(_ElementTable, element_buffer, &element)
  *                 # printf("Retreived Base Element: %s. Status: %d\n", element_buffer, status)
  */
       __pyx_t_4 = ((__pyx_v_isotope_number != 0) != 0);
       if (__pyx_t_4) {
 
-        /* "brainpy/_c/isotopic_distribution.pyx":339
+        /* "brainpy/_c/isotopic_distribution.pyx":351
  *             # printf("Element: %s, Isotope: %d\n", element_buffer, isotope_number)
  *             if isotope_number != 0:
  *                 status = element_hash_table_get(_ElementTable, element_buffer, &element)             # <<<<<<<<<<<<<<
  *                 # printf("Retreived Base Element: %s. Status: %d\n", element_buffer, status)
  *                 element = make_fixed_isotope_element(element, isotope_number)
  */
         __pyx_v_status = __pyx_f_7brainpy_2_c_11composition_element_hash_table_get(__pyx_v_7brainpy_2_c_11composition__ElementTable, __pyx_v_element_buffer, (&__pyx_v_element));
 
-        /* "brainpy/_c/isotopic_distribution.pyx":341
+        /* "brainpy/_c/isotopic_distribution.pyx":353
  *                 status = element_hash_table_get(_ElementTable, element_buffer, &element)
  *                 # printf("Retreived Base Element: %s. Status: %d\n", element_buffer, status)
  *                 element = make_fixed_isotope_element(element, isotope_number)             # <<<<<<<<<<<<<<
  *                 if element == NULL:
  *                     retcode = 1
  */
         __pyx_v_element = __pyx_f_7brainpy_2_c_11composition_make_fixed_isotope_element(__pyx_v_element, __pyx_v_isotope_number);
 
-        /* "brainpy/_c/isotopic_distribution.pyx":342
+        /* "brainpy/_c/isotopic_distribution.pyx":354
  *                 # printf("Retreived Base Element: %s. Status: %d\n", element_buffer, status)
  *                 element = make_fixed_isotope_element(element, isotope_number)
  *                 if element == NULL:             # <<<<<<<<<<<<<<
  *                     retcode = 1
  *                     free(element_buffer)
  */
         __pyx_t_4 = ((__pyx_v_element == NULL) != 0);
         if (__pyx_t_4) {
 
-          /* "brainpy/_c/isotopic_distribution.pyx":343
+          /* "brainpy/_c/isotopic_distribution.pyx":355
  *                 element = make_fixed_isotope_element(element, isotope_number)
  *                 if element == NULL:
  *                     retcode = 1             # <<<<<<<<<<<<<<
  *                     free(element_buffer)
  *                     return retcode
  */
           __pyx_v_retcode = 1;
 
-          /* "brainpy/_c/isotopic_distribution.pyx":344
+          /* "brainpy/_c/isotopic_distribution.pyx":356
  *                 if element == NULL:
  *                     retcode = 1
  *                     free(element_buffer)             # <<<<<<<<<<<<<<
  *                     return retcode
  *                 element_hash_table_put(_ElementTable, element)
  */
           free(__pyx_v_element_buffer);
 
-          /* "brainpy/_c/isotopic_distribution.pyx":345
+          /* "brainpy/_c/isotopic_distribution.pyx":357
  *                     retcode = 1
  *                     free(element_buffer)
  *                     return retcode             # <<<<<<<<<<<<<<
  *                 element_hash_table_put(_ElementTable, element)
  *                 free(element_buffer)
  */
           __pyx_r = __pyx_v_retcode;
           goto __pyx_L0;
 
-          /* "brainpy/_c/isotopic_distribution.pyx":342
+          /* "brainpy/_c/isotopic_distribution.pyx":354
  *                 # printf("Retreived Base Element: %s. Status: %d\n", element_buffer, status)
  *                 element = make_fixed_isotope_element(element, isotope_number)
  *                 if element == NULL:             # <<<<<<<<<<<<<<
  *                     retcode = 1
  *                     free(element_buffer)
  */
         }
 
-        /* "brainpy/_c/isotopic_distribution.pyx":346
+        /* "brainpy/_c/isotopic_distribution.pyx":358
  *                     free(element_buffer)
  *                     return retcode
  *                 element_hash_table_put(_ElementTable, element)             # <<<<<<<<<<<<<<
  *                 free(element_buffer)
  *             else:
  */
         (void)(__pyx_f_7brainpy_2_c_11composition_element_hash_table_put(__pyx_v_7brainpy_2_c_11composition__ElementTable, __pyx_v_element));
 
-        /* "brainpy/_c/isotopic_distribution.pyx":347
+        /* "brainpy/_c/isotopic_distribution.pyx":359
  *                     return retcode
  *                 element_hash_table_put(_ElementTable, element)
  *                 free(element_buffer)             # <<<<<<<<<<<<<<
  *             else:
  *                 # printf("Could not resolve element %s\n", element_symbol)
  */
         free(__pyx_v_element_buffer);
 
-        /* "brainpy/_c/isotopic_distribution.pyx":338
+        /* "brainpy/_c/isotopic_distribution.pyx":350
  *             _parse_isotope_string(element_symbol, &isotope_number, element_buffer)
  *             # printf("Element: %s, Isotope: %d\n", element_buffer, isotope_number)
  *             if isotope_number != 0:             # <<<<<<<<<<<<<<
  *                 status = element_hash_table_get(_ElementTable, element_buffer, &element)
  *                 # printf("Retreived Base Element: %s. Status: %d\n", element_buffer, status)
  */
         goto __pyx_L6;
       }
 
-      /* "brainpy/_c/isotopic_distribution.pyx":350
+      /* "brainpy/_c/isotopic_distribution.pyx":362
  *             else:
  *                 # printf("Could not resolve element %s\n", element_symbol)
  *                 free(element_buffer)             # <<<<<<<<<<<<<<
  *     return retcode
  * 
  */
       /*else*/ {
         free(__pyx_v_element_buffer);
       }
       __pyx_L6:;
 
-      /* "brainpy/_c/isotopic_distribution.pyx":333
+      /* "brainpy/_c/isotopic_distribution.pyx":345
  *         status = element_hash_table_get(_ElementTable, element_symbol, &element)
  *         # printf("Element %s, Status %d\n", element_symbol, status)
  *         if status == -1:             # <<<<<<<<<<<<<<
  *             element_buffer = <char*>malloc(sizeof(char) * 10)
  *             # printf("Could not resolve element %s, attempting to generate fixed isotope\n", element_symbol)
  */
     }
   }
 
-  /* "brainpy/_c/isotopic_distribution.pyx":351
+  /* "brainpy/_c/isotopic_distribution.pyx":363
  *                 # printf("Could not resolve element %s\n", element_symbol)
  *                 free(element_buffer)
  *     return retcode             # <<<<<<<<<<<<<<
  * 
  * # -----------------------------------------------------------------------------
  */
   __pyx_r = __pyx_v_retcode;
   goto __pyx_L0;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":319
+  /* "brainpy/_c/isotopic_distribution.pyx":331
  * 
  * 
  * cdef int validate_composition(Composition* composition) nogil:             # <<<<<<<<<<<<<<
  *     cdef:
  *         size_t i
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "brainpy/_c/isotopic_distribution.pyx":356
+/* "brainpy/_c/isotopic_distribution.pyx":368
  * # IsotopicDistribution Methods
  * 
  * cdef void isotopic_distribution_update_isotopic_constants(IsotopicDistribution* distribution) nogil:             # <<<<<<<<<<<<<<
  *     cdef:
  *         size_t i
  */
 
@@ -4248,149 +4248,149 @@
   struct __pyx_t_7brainpy_2_c_11composition_Composition *__pyx_t_1;
   struct __pyx_t_7brainpy_2_c_18isotopic_constants_IsotopicConstants *__pyx_t_2;
   size_t __pyx_t_3;
   size_t __pyx_t_4;
   size_t __pyx_t_5;
   int __pyx_t_6;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":363
+  /* "brainpy/_c/isotopic_distribution.pyx":375
  *         char* symbol
  * 
  *     composition = distribution.composition             # <<<<<<<<<<<<<<
  *     isotopes = distribution._isotopic_constants
  * 
  */
   __pyx_t_1 = __pyx_v_distribution->composition;
   __pyx_v_composition = __pyx_t_1;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":364
+  /* "brainpy/_c/isotopic_distribution.pyx":376
  * 
  *     composition = distribution.composition
  *     isotopes = distribution._isotopic_constants             # <<<<<<<<<<<<<<
  * 
  *     for i in range(composition.used):
  */
   __pyx_t_2 = __pyx_v_distribution->_isotopic_constants;
   __pyx_v_isotopes = __pyx_t_2;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":366
+  /* "brainpy/_c/isotopic_distribution.pyx":378
  *     isotopes = distribution._isotopic_constants
  * 
  *     for i in range(composition.used):             # <<<<<<<<<<<<<<
  *         symbol = composition.elements[i]
  *         isotopic_constants_add_element(isotopes, symbol)
  */
   __pyx_t_3 = __pyx_v_composition->used;
   __pyx_t_4 = __pyx_t_3;
   for (__pyx_t_5 = 0; __pyx_t_5 < __pyx_t_4; __pyx_t_5+=1) {
     __pyx_v_i = __pyx_t_5;
 
-    /* "brainpy/_c/isotopic_distribution.pyx":367
+    /* "brainpy/_c/isotopic_distribution.pyx":379
  * 
  *     for i in range(composition.used):
  *         symbol = composition.elements[i]             # <<<<<<<<<<<<<<
  *         isotopic_constants_add_element(isotopes, symbol)
  *     isotopes.order = distribution.order
  */
     __pyx_v_symbol = (__pyx_v_composition->elements[__pyx_v_i]);
 
-    /* "brainpy/_c/isotopic_distribution.pyx":368
+    /* "brainpy/_c/isotopic_distribution.pyx":380
  *     for i in range(composition.used):
  *         symbol = composition.elements[i]
  *         isotopic_constants_add_element(isotopes, symbol)             # <<<<<<<<<<<<<<
  *     isotopes.order = distribution.order
  *     isotopic_constants_update_coefficients(isotopes)
  */
     __pyx_f_7brainpy_2_c_18isotopic_constants_isotopic_constants_add_element(__pyx_v_isotopes, __pyx_v_symbol);
   }
 
-  /* "brainpy/_c/isotopic_distribution.pyx":369
+  /* "brainpy/_c/isotopic_distribution.pyx":381
  *         symbol = composition.elements[i]
  *         isotopic_constants_add_element(isotopes, symbol)
  *     isotopes.order = distribution.order             # <<<<<<<<<<<<<<
  *     isotopic_constants_update_coefficients(isotopes)
  * 
  */
   __pyx_t_6 = __pyx_v_distribution->order;
   __pyx_v_isotopes->order = __pyx_t_6;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":370
+  /* "brainpy/_c/isotopic_distribution.pyx":382
  *         isotopic_constants_add_element(isotopes, symbol)
  *     isotopes.order = distribution.order
  *     isotopic_constants_update_coefficients(isotopes)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_f_7brainpy_2_c_18isotopic_constants_isotopic_constants_update_coefficients(__pyx_v_isotopes);
 
-  /* "brainpy/_c/isotopic_distribution.pyx":356
+  /* "brainpy/_c/isotopic_distribution.pyx":368
  * # IsotopicDistribution Methods
  * 
  * cdef void isotopic_distribution_update_isotopic_constants(IsotopicDistribution* distribution) nogil:             # <<<<<<<<<<<<<<
  *     cdef:
  *         size_t i
  */
 
   /* function exit code */
 }
 
-/* "brainpy/_c/isotopic_distribution.pyx":373
+/* "brainpy/_c/isotopic_distribution.pyx":385
  * 
  * 
  * cdef void isotopic_distribution_update_order(IsotopicDistribution* distribution, int order) nogil:             # <<<<<<<<<<<<<<
  *     cdef:
  *         int possible_variants
  */
 
 static void __pyx_f_7brainpy_2_c_21isotopic_distribution_isotopic_distribution_update_order(struct __pyx_t_7brainpy_2_c_21isotopic_distribution_IsotopicDistribution *__pyx_v_distribution, int __pyx_v_order) {
   int __pyx_v_possible_variants;
   int __pyx_t_1;
   int __pyx_t_2;
   int __pyx_t_3;
   int __pyx_t_4;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":377
+  /* "brainpy/_c/isotopic_distribution.pyx":389
  *         int possible_variants
  * 
  *     possible_variants = max_variants(distribution.composition, NULL)             # <<<<<<<<<<<<<<
  *     if order == -1:
  *         distribution.order = possible_variants
  */
   __pyx_v_possible_variants = __pyx_f_7brainpy_2_c_21isotopic_distribution_max_variants(__pyx_v_distribution->composition, NULL);
 
-  /* "brainpy/_c/isotopic_distribution.pyx":378
+  /* "brainpy/_c/isotopic_distribution.pyx":390
  * 
  *     possible_variants = max_variants(distribution.composition, NULL)
  *     if order == -1:             # <<<<<<<<<<<<<<
  *         distribution.order = possible_variants
  *     else:
  */
   __pyx_t_1 = ((__pyx_v_order == -1L) != 0);
   if (__pyx_t_1) {
 
-    /* "brainpy/_c/isotopic_distribution.pyx":379
+    /* "brainpy/_c/isotopic_distribution.pyx":391
  *     possible_variants = max_variants(distribution.composition, NULL)
  *     if order == -1:
  *         distribution.order = possible_variants             # <<<<<<<<<<<<<<
  *     else:
  *         distribution.order = min(order, possible_variants)
  */
     __pyx_v_distribution->order = __pyx_v_possible_variants;
 
-    /* "brainpy/_c/isotopic_distribution.pyx":378
+    /* "brainpy/_c/isotopic_distribution.pyx":390
  * 
  *     possible_variants = max_variants(distribution.composition, NULL)
  *     if order == -1:             # <<<<<<<<<<<<<<
  *         distribution.order = possible_variants
  *     else:
  */
     goto __pyx_L3;
   }
 
-  /* "brainpy/_c/isotopic_distribution.pyx":381
+  /* "brainpy/_c/isotopic_distribution.pyx":393
  *         distribution.order = possible_variants
  *     else:
  *         distribution.order = min(order, possible_variants)             # <<<<<<<<<<<<<<
  * 
  *     isotopic_distribution_update_isotopic_constants(distribution)
  */
   /*else*/ {
@@ -4401,35 +4401,35 @@
     } else {
       __pyx_t_4 = __pyx_t_3;
     }
     __pyx_v_distribution->order = __pyx_t_4;
   }
   __pyx_L3:;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":383
+  /* "brainpy/_c/isotopic_distribution.pyx":395
  *         distribution.order = min(order, possible_variants)
  * 
  *     isotopic_distribution_update_isotopic_constants(distribution)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_f_7brainpy_2_c_21isotopic_distribution_isotopic_distribution_update_isotopic_constants(__pyx_v_distribution);
 
-  /* "brainpy/_c/isotopic_distribution.pyx":373
+  /* "brainpy/_c/isotopic_distribution.pyx":385
  * 
  * 
  * cdef void isotopic_distribution_update_order(IsotopicDistribution* distribution, int order) nogil:             # <<<<<<<<<<<<<<
  *     cdef:
  *         int possible_variants
  */
 
   /* function exit code */
 }
 
-/* "brainpy/_c/isotopic_distribution.pyx":386
+/* "brainpy/_c/isotopic_distribution.pyx":398
  * 
  * 
  * cdef Peak* isotopic_distribution_make_monoisotopic_peak(IsotopicDistribution* distribution) nogil:             # <<<<<<<<<<<<<<
  *     cdef:
  *         Peak* peak
  */
 
@@ -4440,123 +4440,123 @@
   CYTHON_UNUSED int __pyx_v_status;
   double __pyx_v_intensity;
   struct __pyx_t_7brainpy_2_c_21isotopic_distribution_Peak *__pyx_r;
   size_t __pyx_t_1;
   size_t __pyx_t_2;
   size_t __pyx_t_3;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":394
+  /* "brainpy/_c/isotopic_distribution.pyx":406
  *         double intensity
  * 
  *     peak = <Peak*>malloc(sizeof(Peak))             # <<<<<<<<<<<<<<
  *     peak.mz = composition_mass(distribution.composition)
  * 
  */
   __pyx_v_peak = ((struct __pyx_t_7brainpy_2_c_21isotopic_distribution_Peak *)malloc((sizeof(struct __pyx_t_7brainpy_2_c_21isotopic_distribution_Peak))));
 
-  /* "brainpy/_c/isotopic_distribution.pyx":395
+  /* "brainpy/_c/isotopic_distribution.pyx":407
  * 
  *     peak = <Peak*>malloc(sizeof(Peak))
  *     peak.mz = composition_mass(distribution.composition)             # <<<<<<<<<<<<<<
  * 
  *     intensity = 0
  */
   __pyx_v_peak->mz = __pyx_f_7brainpy_2_c_11composition_composition_mass(__pyx_v_distribution->composition);
 
-  /* "brainpy/_c/isotopic_distribution.pyx":397
+  /* "brainpy/_c/isotopic_distribution.pyx":409
  *     peak.mz = composition_mass(distribution.composition)
  * 
  *     intensity = 0             # <<<<<<<<<<<<<<
  *     for i in range(distribution.composition.used):
  *         status = element_cache_get(distribution.cache, distribution.composition.elements[i], &element)
  */
   __pyx_v_intensity = 0.0;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":398
+  /* "brainpy/_c/isotopic_distribution.pyx":410
  * 
  *     intensity = 0
  *     for i in range(distribution.composition.used):             # <<<<<<<<<<<<<<
  *         status = element_cache_get(distribution.cache, distribution.composition.elements[i], &element)
  *         intensity += log(get_isotope_by_neutron_shift(element.isotopes, 0).abundance)
  */
   __pyx_t_1 = __pyx_v_distribution->composition->used;
   __pyx_t_2 = __pyx_t_1;
   for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
     __pyx_v_i = __pyx_t_3;
 
-    /* "brainpy/_c/isotopic_distribution.pyx":399
+    /* "brainpy/_c/isotopic_distribution.pyx":411
  *     intensity = 0
  *     for i in range(distribution.composition.used):
  *         status = element_cache_get(distribution.cache, distribution.composition.elements[i], &element)             # <<<<<<<<<<<<<<
  *         intensity += log(get_isotope_by_neutron_shift(element.isotopes, 0).abundance)
  *     intensity = exp(intensity)
  */
     __pyx_v_status = __pyx_f_7brainpy_2_c_21isotopic_distribution_element_cache_get(__pyx_v_distribution->cache, (__pyx_v_distribution->composition->elements[__pyx_v_i]), (&__pyx_v_element));
 
-    /* "brainpy/_c/isotopic_distribution.pyx":400
+    /* "brainpy/_c/isotopic_distribution.pyx":412
  *     for i in range(distribution.composition.used):
  *         status = element_cache_get(distribution.cache, distribution.composition.elements[i], &element)
  *         intensity += log(get_isotope_by_neutron_shift(element.isotopes, 0).abundance)             # <<<<<<<<<<<<<<
  *     intensity = exp(intensity)
  *     peak.intensity = intensity
  */
     __pyx_v_intensity = (__pyx_v_intensity + log(__pyx_f_7brainpy_2_c_11composition_get_isotope_by_neutron_shift(__pyx_v_element->isotopes, 0)->abundance));
   }
 
-  /* "brainpy/_c/isotopic_distribution.pyx":401
+  /* "brainpy/_c/isotopic_distribution.pyx":413
  *         status = element_cache_get(distribution.cache, distribution.composition.elements[i], &element)
  *         intensity += log(get_isotope_by_neutron_shift(element.isotopes, 0).abundance)
  *     intensity = exp(intensity)             # <<<<<<<<<<<<<<
  *     peak.intensity = intensity
  *     peak.charge = 0
  */
   __pyx_v_intensity = exp(__pyx_v_intensity);
 
-  /* "brainpy/_c/isotopic_distribution.pyx":402
+  /* "brainpy/_c/isotopic_distribution.pyx":414
  *         intensity += log(get_isotope_by_neutron_shift(element.isotopes, 0).abundance)
  *     intensity = exp(intensity)
  *     peak.intensity = intensity             # <<<<<<<<<<<<<<
  *     peak.charge = 0
  *     return peak
  */
   __pyx_v_peak->intensity = __pyx_v_intensity;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":403
+  /* "brainpy/_c/isotopic_distribution.pyx":415
  *     intensity = exp(intensity)
  *     peak.intensity = intensity
  *     peak.charge = 0             # <<<<<<<<<<<<<<
  *     return peak
  * 
  */
   __pyx_v_peak->charge = 0;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":404
+  /* "brainpy/_c/isotopic_distribution.pyx":416
  *     peak.intensity = intensity
  *     peak.charge = 0
  *     return peak             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = __pyx_v_peak;
   goto __pyx_L0;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":386
+  /* "brainpy/_c/isotopic_distribution.pyx":398
  * 
  * 
  * cdef Peak* isotopic_distribution_make_monoisotopic_peak(IsotopicDistribution* distribution) nogil:             # <<<<<<<<<<<<<<
  *     cdef:
  *         Peak* peak
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "brainpy/_c/isotopic_distribution.pyx":407
+/* "brainpy/_c/isotopic_distribution.pyx":419
  * 
  * 
  * cdef IsotopicDistribution* make_isotopic_distribution(Composition* composition, int order, ElementCache* cache=NULL) nogil:             # <<<<<<<<<<<<<<
  *     cdef:
  *         IsotopicDistribution* result
  */
 
@@ -4567,215 +4567,215 @@
   int __pyx_t_1;
   if (__pyx_optional_args) {
     if (__pyx_optional_args->__pyx_n > 0) {
       __pyx_v_cache = __pyx_optional_args->cache;
     }
   }
 
-  /* "brainpy/_c/isotopic_distribution.pyx":410
+  /* "brainpy/_c/isotopic_distribution.pyx":422
  *     cdef:
  *         IsotopicDistribution* result
  *     if cache == NULL:             # <<<<<<<<<<<<<<
  *         cache = make_element_cache(_ElementTable)
  *     result = <IsotopicDistribution*>malloc(sizeof(IsotopicDistribution))
  */
   __pyx_t_1 = ((__pyx_v_cache == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "brainpy/_c/isotopic_distribution.pyx":411
+    /* "brainpy/_c/isotopic_distribution.pyx":423
  *         IsotopicDistribution* result
  *     if cache == NULL:
  *         cache = make_element_cache(_ElementTable)             # <<<<<<<<<<<<<<
  *     result = <IsotopicDistribution*>malloc(sizeof(IsotopicDistribution))
  *     result.composition = composition
  */
     __pyx_v_cache = __pyx_f_7brainpy_2_c_21isotopic_distribution_make_element_cache(__pyx_v_7brainpy_2_c_11composition__ElementTable);
 
-    /* "brainpy/_c/isotopic_distribution.pyx":410
+    /* "brainpy/_c/isotopic_distribution.pyx":422
  *     cdef:
  *         IsotopicDistribution* result
  *     if cache == NULL:             # <<<<<<<<<<<<<<
  *         cache = make_element_cache(_ElementTable)
  *     result = <IsotopicDistribution*>malloc(sizeof(IsotopicDistribution))
  */
   }
 
-  /* "brainpy/_c/isotopic_distribution.pyx":412
+  /* "brainpy/_c/isotopic_distribution.pyx":424
  *     if cache == NULL:
  *         cache = make_element_cache(_ElementTable)
  *     result = <IsotopicDistribution*>malloc(sizeof(IsotopicDistribution))             # <<<<<<<<<<<<<<
  *     result.composition = composition
  *     result.cache = cache
  */
   __pyx_v_result = ((struct __pyx_t_7brainpy_2_c_21isotopic_distribution_IsotopicDistribution *)malloc((sizeof(struct __pyx_t_7brainpy_2_c_21isotopic_distribution_IsotopicDistribution))));
 
-  /* "brainpy/_c/isotopic_distribution.pyx":413
+  /* "brainpy/_c/isotopic_distribution.pyx":425
  *         cache = make_element_cache(_ElementTable)
  *     result = <IsotopicDistribution*>malloc(sizeof(IsotopicDistribution))
  *     result.composition = composition             # <<<<<<<<<<<<<<
  *     result.cache = cache
  *     result.order = 0
  */
   __pyx_v_result->composition = __pyx_v_composition;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":414
+  /* "brainpy/_c/isotopic_distribution.pyx":426
  *     result = <IsotopicDistribution*>malloc(sizeof(IsotopicDistribution))
  *     result.composition = composition
  *     result.cache = cache             # <<<<<<<<<<<<<<
  *     result.order = 0
  *     result._isotopic_constants = make_isotopic_constants()
  */
   __pyx_v_result->cache = __pyx_v_cache;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":415
+  /* "brainpy/_c/isotopic_distribution.pyx":427
  *     result.composition = composition
  *     result.cache = cache
  *     result.order = 0             # <<<<<<<<<<<<<<
  *     result._isotopic_constants = make_isotopic_constants()
  *     isotopic_distribution_update_order(result, order)
  */
   __pyx_v_result->order = 0;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":416
+  /* "brainpy/_c/isotopic_distribution.pyx":428
  *     result.cache = cache
  *     result.order = 0
  *     result._isotopic_constants = make_isotopic_constants()             # <<<<<<<<<<<<<<
  *     isotopic_distribution_update_order(result, order)
  *     result.average_mass = 0
  */
   __pyx_v_result->_isotopic_constants = __pyx_f_7brainpy_2_c_18isotopic_constants_make_isotopic_constants();
 
-  /* "brainpy/_c/isotopic_distribution.pyx":417
+  /* "brainpy/_c/isotopic_distribution.pyx":429
  *     result.order = 0
  *     result._isotopic_constants = make_isotopic_constants()
  *     isotopic_distribution_update_order(result, order)             # <<<<<<<<<<<<<<
  *     result.average_mass = 0
  *     result.monoisotopic_peak = isotopic_distribution_make_monoisotopic_peak(result)
  */
   __pyx_f_7brainpy_2_c_21isotopic_distribution_isotopic_distribution_update_order(__pyx_v_result, __pyx_v_order);
 
-  /* "brainpy/_c/isotopic_distribution.pyx":418
+  /* "brainpy/_c/isotopic_distribution.pyx":430
  *     result._isotopic_constants = make_isotopic_constants()
  *     isotopic_distribution_update_order(result, order)
  *     result.average_mass = 0             # <<<<<<<<<<<<<<
  *     result.monoisotopic_peak = isotopic_distribution_make_monoisotopic_peak(result)
  *     return result
  */
   __pyx_v_result->average_mass = 0.0;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":419
+  /* "brainpy/_c/isotopic_distribution.pyx":431
  *     isotopic_distribution_update_order(result, order)
  *     result.average_mass = 0
  *     result.monoisotopic_peak = isotopic_distribution_make_monoisotopic_peak(result)             # <<<<<<<<<<<<<<
  *     return result
  * 
  */
   __pyx_v_result->monoisotopic_peak = __pyx_f_7brainpy_2_c_21isotopic_distribution_isotopic_distribution_make_monoisotopic_peak(__pyx_v_result);
 
-  /* "brainpy/_c/isotopic_distribution.pyx":420
+  /* "brainpy/_c/isotopic_distribution.pyx":432
  *     result.average_mass = 0
  *     result.monoisotopic_peak = isotopic_distribution_make_monoisotopic_peak(result)
  *     return result             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = __pyx_v_result;
   goto __pyx_L0;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":407
+  /* "brainpy/_c/isotopic_distribution.pyx":419
  * 
  * 
  * cdef IsotopicDistribution* make_isotopic_distribution(Composition* composition, int order, ElementCache* cache=NULL) nogil:             # <<<<<<<<<<<<<<
  *     cdef:
  *         IsotopicDistribution* result
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "brainpy/_c/isotopic_distribution.pyx":423
+/* "brainpy/_c/isotopic_distribution.pyx":435
  * 
  * 
  * cdef void free_isotopic_distribution(IsotopicDistribution* distribution)  nogil:             # <<<<<<<<<<<<<<
  *     free(distribution.monoisotopic_peak)
  *     free_isotopic_constants(distribution._isotopic_constants)
  */
 
 static void __pyx_f_7brainpy_2_c_21isotopic_distribution_free_isotopic_distribution(struct __pyx_t_7brainpy_2_c_21isotopic_distribution_IsotopicDistribution *__pyx_v_distribution) {
   int __pyx_t_1;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":424
+  /* "brainpy/_c/isotopic_distribution.pyx":436
  * 
  * cdef void free_isotopic_distribution(IsotopicDistribution* distribution)  nogil:
  *     free(distribution.monoisotopic_peak)             # <<<<<<<<<<<<<<
  *     free_isotopic_constants(distribution._isotopic_constants)
  *     if distribution.cache != NULL:
  */
   free(__pyx_v_distribution->monoisotopic_peak);
 
-  /* "brainpy/_c/isotopic_distribution.pyx":425
+  /* "brainpy/_c/isotopic_distribution.pyx":437
  * cdef void free_isotopic_distribution(IsotopicDistribution* distribution)  nogil:
  *     free(distribution.monoisotopic_peak)
  *     free_isotopic_constants(distribution._isotopic_constants)             # <<<<<<<<<<<<<<
  *     if distribution.cache != NULL:
  *         free_element_cache(distribution.cache)
  */
   __pyx_f_7brainpy_2_c_18isotopic_constants_free_isotopic_constants(__pyx_v_distribution->_isotopic_constants);
 
-  /* "brainpy/_c/isotopic_distribution.pyx":426
+  /* "brainpy/_c/isotopic_distribution.pyx":438
  *     free(distribution.monoisotopic_peak)
  *     free_isotopic_constants(distribution._isotopic_constants)
  *     if distribution.cache != NULL:             # <<<<<<<<<<<<<<
  *         free_element_cache(distribution.cache)
  *     free(distribution)
  */
   __pyx_t_1 = ((__pyx_v_distribution->cache != NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "brainpy/_c/isotopic_distribution.pyx":427
+    /* "brainpy/_c/isotopic_distribution.pyx":439
  *     free_isotopic_constants(distribution._isotopic_constants)
  *     if distribution.cache != NULL:
  *         free_element_cache(distribution.cache)             # <<<<<<<<<<<<<<
  *     free(distribution)
  * 
  */
     __pyx_f_7brainpy_2_c_21isotopic_distribution_free_element_cache(__pyx_v_distribution->cache);
 
-    /* "brainpy/_c/isotopic_distribution.pyx":426
+    /* "brainpy/_c/isotopic_distribution.pyx":438
  *     free(distribution.monoisotopic_peak)
  *     free_isotopic_constants(distribution._isotopic_constants)
  *     if distribution.cache != NULL:             # <<<<<<<<<<<<<<
  *         free_element_cache(distribution.cache)
  *     free(distribution)
  */
   }
 
-  /* "brainpy/_c/isotopic_distribution.pyx":428
+  /* "brainpy/_c/isotopic_distribution.pyx":440
  *     if distribution.cache != NULL:
  *         free_element_cache(distribution.cache)
  *     free(distribution)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   free(__pyx_v_distribution);
 
-  /* "brainpy/_c/isotopic_distribution.pyx":423
+  /* "brainpy/_c/isotopic_distribution.pyx":435
  * 
  * 
  * cdef void free_isotopic_distribution(IsotopicDistribution* distribution)  nogil:             # <<<<<<<<<<<<<<
  *     free(distribution.monoisotopic_peak)
  *     free_isotopic_constants(distribution._isotopic_constants)
  */
 
   /* function exit code */
 }
 
-/* "brainpy/_c/isotopic_distribution.pyx":431
+/* "brainpy/_c/isotopic_distribution.pyx":443
  * 
  * 
  * cdef dvec* id_phi_values(IsotopicDistribution* distribution) nogil:             # <<<<<<<<<<<<<<
  *     cdef:
  *         dvec* power_sum
  */
 
@@ -4783,78 +4783,78 @@
   __pyx_t_7brainpy_2_c_21isotopic_distribution_dvec *__pyx_v_power_sum;
   size_t __pyx_v_i;
   __pyx_t_7brainpy_2_c_21isotopic_distribution_dvec *__pyx_r;
   long __pyx_t_1;
   long __pyx_t_2;
   size_t __pyx_t_3;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":435
+  /* "brainpy/_c/isotopic_distribution.pyx":447
  *         dvec* power_sum
  *         size_t i
  *     power_sum = make_double_vector_with_size(distribution.order)             # <<<<<<<<<<<<<<
  *     double_vector_append(power_sum, 0.)
  *     for i in range(1, distribution.order + 1):
  */
   __pyx_v_power_sum = __pyx_f_7brainpy_2_c_13double_vector_make_double_vector_with_size(__pyx_v_distribution->order);
 
-  /* "brainpy/_c/isotopic_distribution.pyx":436
+  /* "brainpy/_c/isotopic_distribution.pyx":448
  *         size_t i
  *     power_sum = make_double_vector_with_size(distribution.order)
  *     double_vector_append(power_sum, 0.)             # <<<<<<<<<<<<<<
  *     for i in range(1, distribution.order + 1):
  *         double_vector_append(power_sum, _id_phi_value(distribution, i))
  */
   (void)(__pyx_f_7brainpy_2_c_13double_vector_double_vector_append(__pyx_v_power_sum, 0.));
 
-  /* "brainpy/_c/isotopic_distribution.pyx":437
+  /* "brainpy/_c/isotopic_distribution.pyx":449
  *     power_sum = make_double_vector_with_size(distribution.order)
  *     double_vector_append(power_sum, 0.)
  *     for i in range(1, distribution.order + 1):             # <<<<<<<<<<<<<<
  *         double_vector_append(power_sum, _id_phi_value(distribution, i))
  *     return power_sum
  */
   __pyx_t_1 = (__pyx_v_distribution->order + 1);
   __pyx_t_2 = __pyx_t_1;
   for (__pyx_t_3 = 1; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
     __pyx_v_i = __pyx_t_3;
 
-    /* "brainpy/_c/isotopic_distribution.pyx":438
+    /* "brainpy/_c/isotopic_distribution.pyx":450
  *     double_vector_append(power_sum, 0.)
  *     for i in range(1, distribution.order + 1):
  *         double_vector_append(power_sum, _id_phi_value(distribution, i))             # <<<<<<<<<<<<<<
  *     return power_sum
  * 
  */
     (void)(__pyx_f_7brainpy_2_c_13double_vector_double_vector_append(__pyx_v_power_sum, __pyx_f_7brainpy_2_c_21isotopic_distribution__id_phi_value(__pyx_v_distribution, __pyx_v_i)));
   }
 
-  /* "brainpy/_c/isotopic_distribution.pyx":439
+  /* "brainpy/_c/isotopic_distribution.pyx":451
  *     for i in range(1, distribution.order + 1):
  *         double_vector_append(power_sum, _id_phi_value(distribution, i))
  *     return power_sum             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = __pyx_v_power_sum;
   goto __pyx_L0;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":431
+  /* "brainpy/_c/isotopic_distribution.pyx":443
  * 
  * 
  * cdef dvec* id_phi_values(IsotopicDistribution* distribution) nogil:             # <<<<<<<<<<<<<<
  *     cdef:
  *         dvec* power_sum
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "brainpy/_c/isotopic_distribution.pyx":442
+/* "brainpy/_c/isotopic_distribution.pyx":454
  * 
  * 
  * cdef double _id_phi_value(IsotopicDistribution* distribution, int order) nogil:             # <<<<<<<<<<<<<<
  *     cdef:
  *         double phi
  */
 
@@ -4862,173 +4862,173 @@
   double __pyx_v_phi;
   char *__pyx_v_element;
   double __pyx_v_count;
   size_t __pyx_v_i;
   double __pyx_r;
   int __pyx_t_1;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":449
+  /* "brainpy/_c/isotopic_distribution.pyx":461
  *         size_t i
  * 
  *     phi = 0             # <<<<<<<<<<<<<<
  *     i = 0
  *     while i < distribution.composition.used:
  */
   __pyx_v_phi = 0.0;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":450
+  /* "brainpy/_c/isotopic_distribution.pyx":462
  * 
  *     phi = 0
  *     i = 0             # <<<<<<<<<<<<<<
  *     while i < distribution.composition.used:
  *         element = distribution.composition.elements[i]
  */
   __pyx_v_i = 0;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":451
+  /* "brainpy/_c/isotopic_distribution.pyx":463
  *     phi = 0
  *     i = 0
  *     while i < distribution.composition.used:             # <<<<<<<<<<<<<<
  *         element = distribution.composition.elements[i]
  *         count = distribution.composition.counts[i]
  */
   while (1) {
     __pyx_t_1 = ((__pyx_v_i < __pyx_v_distribution->composition->used) != 0);
     if (!__pyx_t_1) break;
 
-    /* "brainpy/_c/isotopic_distribution.pyx":452
+    /* "brainpy/_c/isotopic_distribution.pyx":464
  *     i = 0
  *     while i < distribution.composition.used:
  *         element = distribution.composition.elements[i]             # <<<<<<<<<<<<<<
  *         count = distribution.composition.counts[i]
  *         phi += isotopic_constants_nth_element_power_sum(
  */
     __pyx_v_element = (__pyx_v_distribution->composition->elements[__pyx_v_i]);
 
-    /* "brainpy/_c/isotopic_distribution.pyx":453
+    /* "brainpy/_c/isotopic_distribution.pyx":465
  *     while i < distribution.composition.used:
  *         element = distribution.composition.elements[i]
  *         count = distribution.composition.counts[i]             # <<<<<<<<<<<<<<
  *         phi += isotopic_constants_nth_element_power_sum(
  *             distribution._isotopic_constants, element, order) * count
  */
     __pyx_v_count = (__pyx_v_distribution->composition->counts[__pyx_v_i]);
 
-    /* "brainpy/_c/isotopic_distribution.pyx":454
+    /* "brainpy/_c/isotopic_distribution.pyx":466
  *         element = distribution.composition.elements[i]
  *         count = distribution.composition.counts[i]
  *         phi += isotopic_constants_nth_element_power_sum(             # <<<<<<<<<<<<<<
  *             distribution._isotopic_constants, element, order) * count
  *         i += 1
  */
     __pyx_v_phi = (__pyx_v_phi + (__pyx_f_7brainpy_2_c_18isotopic_constants_isotopic_constants_nth_element_power_sum(__pyx_v_distribution->_isotopic_constants, __pyx_v_element, __pyx_v_order) * __pyx_v_count));
 
-    /* "brainpy/_c/isotopic_distribution.pyx":456
+    /* "brainpy/_c/isotopic_distribution.pyx":468
  *         phi += isotopic_constants_nth_element_power_sum(
  *             distribution._isotopic_constants, element, order) * count
  *         i += 1             # <<<<<<<<<<<<<<
  *     return phi
  * 
  */
     __pyx_v_i = (__pyx_v_i + 1);
   }
 
-  /* "brainpy/_c/isotopic_distribution.pyx":457
+  /* "brainpy/_c/isotopic_distribution.pyx":469
  *             distribution._isotopic_constants, element, order) * count
  *         i += 1
  *     return phi             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = __pyx_v_phi;
   goto __pyx_L0;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":442
+  /* "brainpy/_c/isotopic_distribution.pyx":454
  * 
  * 
  * cdef double _id_phi_value(IsotopicDistribution* distribution, int order) nogil:             # <<<<<<<<<<<<<<
  *     cdef:
  *         double phi
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "brainpy/_c/isotopic_distribution.pyx":460
+/* "brainpy/_c/isotopic_distribution.pyx":472
  * 
  * 
  * cdef dvec* id_modified_phi_values(IsotopicDistribution* distribution, char* element, dvec* power_sum) nogil:             # <<<<<<<<<<<<<<
  *     cdef:
  *         size_t i
  */
 
 static __pyx_t_7brainpy_2_c_21isotopic_distribution_dvec *__pyx_f_7brainpy_2_c_21isotopic_distribution_id_modified_phi_values(struct __pyx_t_7brainpy_2_c_21isotopic_distribution_IsotopicDistribution *__pyx_v_distribution, char *__pyx_v_element, __pyx_t_7brainpy_2_c_21isotopic_distribution_dvec *__pyx_v_power_sum) {
   size_t __pyx_v_i;
   __pyx_t_7brainpy_2_c_21isotopic_distribution_dvec *__pyx_r;
   long __pyx_t_1;
   long __pyx_t_2;
   size_t __pyx_t_3;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":464
+  /* "brainpy/_c/isotopic_distribution.pyx":476
  *         size_t i
  * 
  *     double_vector_append(power_sum, 0.)             # <<<<<<<<<<<<<<
  *     for i in range(1, distribution.order + 1):
  *         double_vector_append(power_sum,
  */
   (void)(__pyx_f_7brainpy_2_c_13double_vector_double_vector_append(__pyx_v_power_sum, 0.));
 
-  /* "brainpy/_c/isotopic_distribution.pyx":465
+  /* "brainpy/_c/isotopic_distribution.pyx":477
  * 
  *     double_vector_append(power_sum, 0.)
  *     for i in range(1, distribution.order + 1):             # <<<<<<<<<<<<<<
  *         double_vector_append(power_sum,
  *                              _id_modified_phi_value(distribution, element, i))
  */
   __pyx_t_1 = (__pyx_v_distribution->order + 1);
   __pyx_t_2 = __pyx_t_1;
   for (__pyx_t_3 = 1; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
     __pyx_v_i = __pyx_t_3;
 
-    /* "brainpy/_c/isotopic_distribution.pyx":466
+    /* "brainpy/_c/isotopic_distribution.pyx":478
  *     double_vector_append(power_sum, 0.)
  *     for i in range(1, distribution.order + 1):
  *         double_vector_append(power_sum,             # <<<<<<<<<<<<<<
  *                              _id_modified_phi_value(distribution, element, i))
  *     return power_sum
  */
     (void)(__pyx_f_7brainpy_2_c_13double_vector_double_vector_append(__pyx_v_power_sum, __pyx_f_7brainpy_2_c_21isotopic_distribution__id_modified_phi_value(__pyx_v_distribution, __pyx_v_element, __pyx_v_i)));
   }
 
-  /* "brainpy/_c/isotopic_distribution.pyx":468
+  /* "brainpy/_c/isotopic_distribution.pyx":480
  *         double_vector_append(power_sum,
  *                              _id_modified_phi_value(distribution, element, i))
  *     return power_sum             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = __pyx_v_power_sum;
   goto __pyx_L0;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":460
+  /* "brainpy/_c/isotopic_distribution.pyx":472
  * 
  * 
  * cdef dvec* id_modified_phi_values(IsotopicDistribution* distribution, char* element, dvec* power_sum) nogil:             # <<<<<<<<<<<<<<
  *     cdef:
  *         size_t i
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "brainpy/_c/isotopic_distribution.pyx":471
+/* "brainpy/_c/isotopic_distribution.pyx":483
  * 
  * 
  * cdef double _id_modified_phi_value(IsotopicDistribution* distribution, char* symbol, int order) nogil:             # <<<<<<<<<<<<<<
  *     cdef:
  *         double phi
  */
 
@@ -5037,154 +5037,154 @@
   char *__pyx_v_element;
   double __pyx_v_count;
   size_t __pyx_v_i;
   double __pyx_v_coef;
   double __pyx_r;
   int __pyx_t_1;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":479
+  /* "brainpy/_c/isotopic_distribution.pyx":491
  *         double coef
  * 
  *     phi = 0             # <<<<<<<<<<<<<<
  *     i = 0
  *     while i < distribution.composition.used:
  */
   __pyx_v_phi = 0.0;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":480
+  /* "brainpy/_c/isotopic_distribution.pyx":492
  * 
  *     phi = 0
  *     i = 0             # <<<<<<<<<<<<<<
  *     while i < distribution.composition.used:
  *         element = distribution.composition.elements[i]
  */
   __pyx_v_i = 0;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":481
+  /* "brainpy/_c/isotopic_distribution.pyx":493
  *     phi = 0
  *     i = 0
  *     while i < distribution.composition.used:             # <<<<<<<<<<<<<<
  *         element = distribution.composition.elements[i]
  *         count = distribution.composition.counts[i]
  */
   while (1) {
     __pyx_t_1 = ((__pyx_v_i < __pyx_v_distribution->composition->used) != 0);
     if (!__pyx_t_1) break;
 
-    /* "brainpy/_c/isotopic_distribution.pyx":482
+    /* "brainpy/_c/isotopic_distribution.pyx":494
  *     i = 0
  *     while i < distribution.composition.used:
  *         element = distribution.composition.elements[i]             # <<<<<<<<<<<<<<
  *         count = distribution.composition.counts[i]
  * 
  */
     __pyx_v_element = (__pyx_v_distribution->composition->elements[__pyx_v_i]);
 
-    /* "brainpy/_c/isotopic_distribution.pyx":483
+    /* "brainpy/_c/isotopic_distribution.pyx":495
  *     while i < distribution.composition.used:
  *         element = distribution.composition.elements[i]
  *         count = distribution.composition.counts[i]             # <<<<<<<<<<<<<<
  * 
  *         if strcmp(element, symbol) == 0:
  */
     __pyx_v_count = (__pyx_v_distribution->composition->counts[__pyx_v_i]);
 
-    /* "brainpy/_c/isotopic_distribution.pyx":485
+    /* "brainpy/_c/isotopic_distribution.pyx":497
  *         count = distribution.composition.counts[i]
  * 
  *         if strcmp(element, symbol) == 0:             # <<<<<<<<<<<<<<
  *             coef = count - 1
  *         else:
  */
     __pyx_t_1 = ((strcmp(__pyx_v_element, __pyx_v_symbol) == 0) != 0);
     if (__pyx_t_1) {
 
-      /* "brainpy/_c/isotopic_distribution.pyx":486
+      /* "brainpy/_c/isotopic_distribution.pyx":498
  * 
  *         if strcmp(element, symbol) == 0:
  *             coef = count - 1             # <<<<<<<<<<<<<<
  *         else:
  *             coef = count
  */
       __pyx_v_coef = (__pyx_v_count - 1.0);
 
-      /* "brainpy/_c/isotopic_distribution.pyx":485
+      /* "brainpy/_c/isotopic_distribution.pyx":497
  *         count = distribution.composition.counts[i]
  * 
  *         if strcmp(element, symbol) == 0:             # <<<<<<<<<<<<<<
  *             coef = count - 1
  *         else:
  */
       goto __pyx_L5;
     }
 
-    /* "brainpy/_c/isotopic_distribution.pyx":488
+    /* "brainpy/_c/isotopic_distribution.pyx":500
  *             coef = count - 1
  *         else:
  *             coef = count             # <<<<<<<<<<<<<<
  * 
  *         phi += isotopic_constants_nth_element_power_sum(
  */
     /*else*/ {
       __pyx_v_coef = __pyx_v_count;
     }
     __pyx_L5:;
 
-    /* "brainpy/_c/isotopic_distribution.pyx":490
+    /* "brainpy/_c/isotopic_distribution.pyx":502
  *             coef = count
  * 
  *         phi += isotopic_constants_nth_element_power_sum(             # <<<<<<<<<<<<<<
  *             distribution._isotopic_constants, element, order) * coef
  *         i += 1
  */
     __pyx_v_phi = (__pyx_v_phi + (__pyx_f_7brainpy_2_c_18isotopic_constants_isotopic_constants_nth_element_power_sum(__pyx_v_distribution->_isotopic_constants, __pyx_v_element, __pyx_v_order) * __pyx_v_coef));
 
-    /* "brainpy/_c/isotopic_distribution.pyx":492
+    /* "brainpy/_c/isotopic_distribution.pyx":504
  *         phi += isotopic_constants_nth_element_power_sum(
  *             distribution._isotopic_constants, element, order) * coef
  *         i += 1             # <<<<<<<<<<<<<<
  * 
  *     phi += isotopic_constants_nth_modified_element_power_sum(
  */
     __pyx_v_i = (__pyx_v_i + 1);
   }
 
-  /* "brainpy/_c/isotopic_distribution.pyx":494
+  /* "brainpy/_c/isotopic_distribution.pyx":506
  *         i += 1
  * 
  *     phi += isotopic_constants_nth_modified_element_power_sum(             # <<<<<<<<<<<<<<
  *         distribution._isotopic_constants, symbol, order)
  * 
  */
   __pyx_v_phi = (__pyx_v_phi + __pyx_f_7brainpy_2_c_18isotopic_constants_isotopic_constants_nth_modified_element_power_sum(__pyx_v_distribution->_isotopic_constants, __pyx_v_symbol, __pyx_v_order));
 
-  /* "brainpy/_c/isotopic_distribution.pyx":497
+  /* "brainpy/_c/isotopic_distribution.pyx":509
  *         distribution._isotopic_constants, symbol, order)
  * 
  *     return phi             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = __pyx_v_phi;
   goto __pyx_L0;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":471
+  /* "brainpy/_c/isotopic_distribution.pyx":483
  * 
  * 
  * cdef double _id_modified_phi_value(IsotopicDistribution* distribution, char* symbol, int order) nogil:             # <<<<<<<<<<<<<<
  *     cdef:
  *         double phi
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "brainpy/_c/isotopic_distribution.pyx":500
+/* "brainpy/_c/isotopic_distribution.pyx":512
  * 
  * 
  * cdef dvec* id_probability_vector(IsotopicDistribution* distribution) nogil:             # <<<<<<<<<<<<<<
  *     cdef:
  *         dvec* phi_values
  */
 
@@ -5197,120 +5197,120 @@
   __pyx_t_7brainpy_2_c_21isotopic_distribution_dvec *__pyx_r;
   size_t __pyx_t_1;
   size_t __pyx_t_2;
   size_t __pyx_t_3;
   int __pyx_t_4;
   size_t __pyx_t_5;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":508
+  /* "brainpy/_c/isotopic_distribution.pyx":520
  *         int sign
  * 
  *     phi_values = id_phi_values(distribution)             # <<<<<<<<<<<<<<
  *     probability_vector = make_double_vector_with_size(phi_values.size)
  *     max_variant_count = distribution.order + 1
  */
   __pyx_v_phi_values = __pyx_f_7brainpy_2_c_21isotopic_distribution_id_phi_values(__pyx_v_distribution);
 
-  /* "brainpy/_c/isotopic_distribution.pyx":509
+  /* "brainpy/_c/isotopic_distribution.pyx":521
  * 
  *     phi_values = id_phi_values(distribution)
  *     probability_vector = make_double_vector_with_size(phi_values.size)             # <<<<<<<<<<<<<<
  *     max_variant_count = distribution.order + 1
  * 
  */
   __pyx_v_probability_vector = __pyx_f_7brainpy_2_c_13double_vector_make_double_vector_with_size(__pyx_v_phi_values->size);
 
-  /* "brainpy/_c/isotopic_distribution.pyx":510
+  /* "brainpy/_c/isotopic_distribution.pyx":522
  *     phi_values = id_phi_values(distribution)
  *     probability_vector = make_double_vector_with_size(phi_values.size)
  *     max_variant_count = distribution.order + 1             # <<<<<<<<<<<<<<
  * 
  *     newton(phi_values, probability_vector, max_variant_count)
  */
   __pyx_v_max_variant_count = (__pyx_v_distribution->order + 1);
 
-  /* "brainpy/_c/isotopic_distribution.pyx":512
+  /* "brainpy/_c/isotopic_distribution.pyx":524
  *     max_variant_count = distribution.order + 1
  * 
  *     newton(phi_values, probability_vector, max_variant_count)             # <<<<<<<<<<<<<<
  * 
  *     for i in range(0, probability_vector.used):
  */
   __pyx_f_7brainpy_2_c_18isotopic_constants_newton(__pyx_v_phi_values, __pyx_v_probability_vector, __pyx_v_max_variant_count);
 
-  /* "brainpy/_c/isotopic_distribution.pyx":514
+  /* "brainpy/_c/isotopic_distribution.pyx":526
  *     newton(phi_values, probability_vector, max_variant_count)
  * 
  *     for i in range(0, probability_vector.used):             # <<<<<<<<<<<<<<
  *         sign = 1 if i % 2 == 0 else -1
  *         probability_vector.v[i] *= distribution.monoisotopic_peak.intensity * sign
  */
   __pyx_t_1 = __pyx_v_probability_vector->used;
   __pyx_t_2 = __pyx_t_1;
   for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
     __pyx_v_i = __pyx_t_3;
 
-    /* "brainpy/_c/isotopic_distribution.pyx":515
+    /* "brainpy/_c/isotopic_distribution.pyx":527
  * 
  *     for i in range(0, probability_vector.used):
  *         sign = 1 if i % 2 == 0 else -1             # <<<<<<<<<<<<<<
  *         probability_vector.v[i] *= distribution.monoisotopic_peak.intensity * sign
  * 
  */
     if ((((__pyx_v_i % 2) == 0) != 0)) {
       __pyx_t_4 = 1;
     } else {
       __pyx_t_4 = -1;
     }
     __pyx_v_sign = __pyx_t_4;
 
-    /* "brainpy/_c/isotopic_distribution.pyx":516
+    /* "brainpy/_c/isotopic_distribution.pyx":528
  *     for i in range(0, probability_vector.used):
  *         sign = 1 if i % 2 == 0 else -1
  *         probability_vector.v[i] *= distribution.monoisotopic_peak.intensity * sign             # <<<<<<<<<<<<<<
  * 
  *     free_double_vector(phi_values)
  */
     __pyx_t_5 = __pyx_v_i;
     (__pyx_v_probability_vector->v[__pyx_t_5]) = ((__pyx_v_probability_vector->v[__pyx_t_5]) * (__pyx_v_distribution->monoisotopic_peak->intensity * __pyx_v_sign));
   }
 
-  /* "brainpy/_c/isotopic_distribution.pyx":518
+  /* "brainpy/_c/isotopic_distribution.pyx":530
  *         probability_vector.v[i] *= distribution.monoisotopic_peak.intensity * sign
  * 
  *     free_double_vector(phi_values)             # <<<<<<<<<<<<<<
  *     return probability_vector
  * 
  */
   __pyx_f_7brainpy_2_c_13double_vector_free_double_vector(__pyx_v_phi_values);
 
-  /* "brainpy/_c/isotopic_distribution.pyx":519
+  /* "brainpy/_c/isotopic_distribution.pyx":531
  * 
  *     free_double_vector(phi_values)
  *     return probability_vector             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = __pyx_v_probability_vector;
   goto __pyx_L0;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":500
+  /* "brainpy/_c/isotopic_distribution.pyx":512
  * 
  * 
  * cdef dvec* id_probability_vector(IsotopicDistribution* distribution) nogil:             # <<<<<<<<<<<<<<
  *     cdef:
  *         dvec* phi_values
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "brainpy/_c/isotopic_distribution.pyx":523
+/* "brainpy/_c/isotopic_distribution.pyx":535
  * 
  * @cython.cdivision
  * cdef dvec* id_center_mass_vector(IsotopicDistribution* distribution, dvec* probability_vector) nogil:             # <<<<<<<<<<<<<<
  *     cdef:
  *         dvec* mass_vector
  */
 
@@ -5336,392 +5336,392 @@
   double __pyx_t_1;
   int __pyx_t_2;
   long __pyx_t_3;
   long __pyx_t_4;
   size_t __pyx_t_5;
   int __pyx_t_6;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":537
+  /* "brainpy/_c/isotopic_distribution.pyx":549
  *         ElementPolynomialMap* ep_map
  * 
  *     mass_vector = make_double_vector_with_size(probability_vector.size + 3)             # <<<<<<<<<<<<<<
  *     power_sum = make_double_vector()
  *     max_variant_count = distribution.order + 1
  */
   __pyx_v_mass_vector = __pyx_f_7brainpy_2_c_13double_vector_make_double_vector_with_size((__pyx_v_probability_vector->size + 3));
 
-  /* "brainpy/_c/isotopic_distribution.pyx":538
+  /* "brainpy/_c/isotopic_distribution.pyx":550
  * 
  *     mass_vector = make_double_vector_with_size(probability_vector.size + 3)
  *     power_sum = make_double_vector()             # <<<<<<<<<<<<<<
  *     max_variant_count = distribution.order + 1
  *     base_intensity = distribution.monoisotopic_peak.intensity
  */
   __pyx_v_power_sum = __pyx_f_7brainpy_2_c_13double_vector_make_double_vector();
 
-  /* "brainpy/_c/isotopic_distribution.pyx":539
+  /* "brainpy/_c/isotopic_distribution.pyx":551
  *     mass_vector = make_double_vector_with_size(probability_vector.size + 3)
  *     power_sum = make_double_vector()
  *     max_variant_count = distribution.order + 1             # <<<<<<<<<<<<<<
  *     base_intensity = distribution.monoisotopic_peak.intensity
  *     ep_map = make_element_polynomial_map(distribution.composition.size)
  */
   __pyx_v_max_variant_count = (__pyx_v_distribution->order + 1);
 
-  /* "brainpy/_c/isotopic_distribution.pyx":540
+  /* "brainpy/_c/isotopic_distribution.pyx":552
  *     power_sum = make_double_vector()
  *     max_variant_count = distribution.order + 1
  *     base_intensity = distribution.monoisotopic_peak.intensity             # <<<<<<<<<<<<<<
  *     ep_map = make_element_polynomial_map(distribution.composition.size)
  * 
  */
   __pyx_t_1 = __pyx_v_distribution->monoisotopic_peak->intensity;
   __pyx_v_base_intensity = __pyx_t_1;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":541
+  /* "brainpy/_c/isotopic_distribution.pyx":553
  *     max_variant_count = distribution.order + 1
  *     base_intensity = distribution.monoisotopic_peak.intensity
  *     ep_map = make_element_polynomial_map(distribution.composition.size)             # <<<<<<<<<<<<<<
  * 
  *     j = 0
  */
   __pyx_v_ep_map = __pyx_f_7brainpy_2_c_21isotopic_distribution_make_element_polynomial_map(__pyx_v_distribution->composition->size);
 
-  /* "brainpy/_c/isotopic_distribution.pyx":543
+  /* "brainpy/_c/isotopic_distribution.pyx":555
  *     ep_map = make_element_polynomial_map(distribution.composition.size)
  * 
  *     j = 0             # <<<<<<<<<<<<<<
  *     while j < distribution.composition.used:
  *         element = distribution.composition.elements[j]
  */
   __pyx_v_j = 0;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":544
+  /* "brainpy/_c/isotopic_distribution.pyx":556
  * 
  *     j = 0
  *     while j < distribution.composition.used:             # <<<<<<<<<<<<<<
  *         element = distribution.composition.elements[j]
  *         reset_double_vector(power_sum)
  */
   while (1) {
     __pyx_t_2 = ((__pyx_v_j < __pyx_v_distribution->composition->used) != 0);
     if (!__pyx_t_2) break;
 
-    /* "brainpy/_c/isotopic_distribution.pyx":545
+    /* "brainpy/_c/isotopic_distribution.pyx":557
  *     j = 0
  *     while j < distribution.composition.used:
  *         element = distribution.composition.elements[j]             # <<<<<<<<<<<<<<
  *         reset_double_vector(power_sum)
  *         power_sum = id_modified_phi_values(distribution, element, power_sum)
  */
     __pyx_v_element = (__pyx_v_distribution->composition->elements[__pyx_v_j]);
 
-    /* "brainpy/_c/isotopic_distribution.pyx":546
+    /* "brainpy/_c/isotopic_distribution.pyx":558
  *     while j < distribution.composition.used:
  *         element = distribution.composition.elements[j]
  *         reset_double_vector(power_sum)             # <<<<<<<<<<<<<<
  *         power_sum = id_modified_phi_values(distribution, element, power_sum)
  *         ele_sym_poly = make_double_vector()
  */
     __pyx_f_7brainpy_2_c_13double_vector_reset_double_vector(__pyx_v_power_sum);
 
-    /* "brainpy/_c/isotopic_distribution.pyx":547
+    /* "brainpy/_c/isotopic_distribution.pyx":559
  *         element = distribution.composition.elements[j]
  *         reset_double_vector(power_sum)
  *         power_sum = id_modified_phi_values(distribution, element, power_sum)             # <<<<<<<<<<<<<<
  *         ele_sym_poly = make_double_vector()
  *         newton(power_sum, ele_sym_poly, max_variant_count)
  */
     __pyx_v_power_sum = __pyx_f_7brainpy_2_c_21isotopic_distribution_id_modified_phi_values(__pyx_v_distribution, __pyx_v_element, __pyx_v_power_sum);
 
-    /* "brainpy/_c/isotopic_distribution.pyx":548
+    /* "brainpy/_c/isotopic_distribution.pyx":560
  *         reset_double_vector(power_sum)
  *         power_sum = id_modified_phi_values(distribution, element, power_sum)
  *         ele_sym_poly = make_double_vector()             # <<<<<<<<<<<<<<
  *         newton(power_sum, ele_sym_poly, max_variant_count)
  *         element_polynomial_map_set(ep_map, element, ele_sym_poly)
  */
     __pyx_v_ele_sym_poly = __pyx_f_7brainpy_2_c_13double_vector_make_double_vector();
 
-    /* "brainpy/_c/isotopic_distribution.pyx":549
+    /* "brainpy/_c/isotopic_distribution.pyx":561
  *         power_sum = id_modified_phi_values(distribution, element, power_sum)
  *         ele_sym_poly = make_double_vector()
  *         newton(power_sum, ele_sym_poly, max_variant_count)             # <<<<<<<<<<<<<<
  *         element_polynomial_map_set(ep_map, element, ele_sym_poly)
  *         j += 1
  */
     __pyx_f_7brainpy_2_c_18isotopic_constants_newton(__pyx_v_power_sum, __pyx_v_ele_sym_poly, __pyx_v_max_variant_count);
 
-    /* "brainpy/_c/isotopic_distribution.pyx":550
+    /* "brainpy/_c/isotopic_distribution.pyx":562
  *         ele_sym_poly = make_double_vector()
  *         newton(power_sum, ele_sym_poly, max_variant_count)
  *         element_polynomial_map_set(ep_map, element, ele_sym_poly)             # <<<<<<<<<<<<<<
  *         j += 1
  *     free_double_vector(power_sum)
  */
     (void)(__pyx_f_7brainpy_2_c_21isotopic_distribution_element_polynomial_map_set(__pyx_v_ep_map, __pyx_v_element, __pyx_v_ele_sym_poly));
 
-    /* "brainpy/_c/isotopic_distribution.pyx":551
+    /* "brainpy/_c/isotopic_distribution.pyx":563
  *         newton(power_sum, ele_sym_poly, max_variant_count)
  *         element_polynomial_map_set(ep_map, element, ele_sym_poly)
  *         j += 1             # <<<<<<<<<<<<<<
  *     free_double_vector(power_sum)
  *     i = 0
  */
     __pyx_v_j = (__pyx_v_j + 1);
   }
 
-  /* "brainpy/_c/isotopic_distribution.pyx":552
+  /* "brainpy/_c/isotopic_distribution.pyx":564
  *         element_polynomial_map_set(ep_map, element, ele_sym_poly)
  *         j += 1
  *     free_double_vector(power_sum)             # <<<<<<<<<<<<<<
  *     i = 0
  *     for i in range(distribution.order + 1):
  */
   __pyx_f_7brainpy_2_c_13double_vector_free_double_vector(__pyx_v_power_sum);
 
-  /* "brainpy/_c/isotopic_distribution.pyx":553
+  /* "brainpy/_c/isotopic_distribution.pyx":565
  *         j += 1
  *     free_double_vector(power_sum)
  *     i = 0             # <<<<<<<<<<<<<<
  *     for i in range(distribution.order + 1):
  *         sign = 1 if i % 2 == 0 else -1
  */
   __pyx_v_i = 0;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":554
+  /* "brainpy/_c/isotopic_distribution.pyx":566
  *     free_double_vector(power_sum)
  *     i = 0
  *     for i in range(distribution.order + 1):             # <<<<<<<<<<<<<<
  *         sign = 1 if i % 2 == 0 else -1
  *         center = 0.0
  */
   __pyx_t_3 = (__pyx_v_distribution->order + 1);
   __pyx_t_4 = __pyx_t_3;
   for (__pyx_t_5 = 0; __pyx_t_5 < __pyx_t_4; __pyx_t_5+=1) {
     __pyx_v_i = __pyx_t_5;
 
-    /* "brainpy/_c/isotopic_distribution.pyx":555
+    /* "brainpy/_c/isotopic_distribution.pyx":567
  *     i = 0
  *     for i in range(distribution.order + 1):
  *         sign = 1 if i % 2 == 0 else -1             # <<<<<<<<<<<<<<
  *         center = 0.0
  *         k = 0
  */
     if ((((__pyx_v_i % 2) == 0) != 0)) {
       __pyx_t_6 = 1;
     } else {
       __pyx_t_6 = -1;
     }
     __pyx_v_sign = __pyx_t_6;
 
-    /* "brainpy/_c/isotopic_distribution.pyx":556
+    /* "brainpy/_c/isotopic_distribution.pyx":568
  *     for i in range(distribution.order + 1):
  *         sign = 1 if i % 2 == 0 else -1
  *         center = 0.0             # <<<<<<<<<<<<<<
  *         k = 0
  *         while k < ep_map.used:
  */
     __pyx_v_center = 0.0;
 
-    /* "brainpy/_c/isotopic_distribution.pyx":557
+    /* "brainpy/_c/isotopic_distribution.pyx":569
  *         sign = 1 if i % 2 == 0 else -1
  *         center = 0.0
  *         k = 0             # <<<<<<<<<<<<<<
  *         while k < ep_map.used:
  *             element = ep_map.elements[k]
  */
     __pyx_v_k = 0;
 
-    /* "brainpy/_c/isotopic_distribution.pyx":558
+    /* "brainpy/_c/isotopic_distribution.pyx":570
  *         center = 0.0
  *         k = 0
  *         while k < ep_map.used:             # <<<<<<<<<<<<<<
  *             element = ep_map.elements[k]
  *             element_polynomial_map_get(ep_map, element, &ele_sym_poly)
  */
     while (1) {
       __pyx_t_2 = ((__pyx_v_k < __pyx_v_ep_map->used) != 0);
       if (!__pyx_t_2) break;
 
-      /* "brainpy/_c/isotopic_distribution.pyx":559
+      /* "brainpy/_c/isotopic_distribution.pyx":571
  *         k = 0
  *         while k < ep_map.used:
  *             element = ep_map.elements[k]             # <<<<<<<<<<<<<<
  *             element_polynomial_map_get(ep_map, element, &ele_sym_poly)
  * 
  */
       __pyx_v_element = (__pyx_v_ep_map->elements[__pyx_v_k]);
 
-      /* "brainpy/_c/isotopic_distribution.pyx":560
+      /* "brainpy/_c/isotopic_distribution.pyx":572
  *         while k < ep_map.used:
  *             element = ep_map.elements[k]
  *             element_polynomial_map_get(ep_map, element, &ele_sym_poly)             # <<<<<<<<<<<<<<
  * 
  *             composition_get_element_count(distribution.composition, element, &_element_count)
  */
       (void)(__pyx_f_7brainpy_2_c_21isotopic_distribution_element_polynomial_map_get(__pyx_v_ep_map, __pyx_v_element, (&__pyx_v_ele_sym_poly)));
 
-      /* "brainpy/_c/isotopic_distribution.pyx":562
+      /* "brainpy/_c/isotopic_distribution.pyx":574
  *             element_polynomial_map_get(ep_map, element, &ele_sym_poly)
  * 
  *             composition_get_element_count(distribution.composition, element, &_element_count)             # <<<<<<<<<<<<<<
  *             element_cache_get(distribution.cache, element, &element_struct)
  * 
  */
       (void)(__pyx_f_7brainpy_2_c_11composition_composition_get_element_count(__pyx_v_distribution->composition, __pyx_v_element, (&__pyx_v__element_count)));
 
-      /* "brainpy/_c/isotopic_distribution.pyx":563
+      /* "brainpy/_c/isotopic_distribution.pyx":575
  * 
  *             composition_get_element_count(distribution.composition, element, &_element_count)
  *             element_cache_get(distribution.cache, element, &element_struct)             # <<<<<<<<<<<<<<
  * 
  *             _monoisotopic_mass = element_monoisotopic_mass(element_struct)
  */
       (void)(__pyx_f_7brainpy_2_c_21isotopic_distribution_element_cache_get(__pyx_v_distribution->cache, __pyx_v_element, (&__pyx_v_element_struct)));
 
-      /* "brainpy/_c/isotopic_distribution.pyx":565
+      /* "brainpy/_c/isotopic_distribution.pyx":577
  *             element_cache_get(distribution.cache, element, &element_struct)
  * 
  *             _monoisotopic_mass = element_monoisotopic_mass(element_struct)             # <<<<<<<<<<<<<<
  * 
  *             polynomial_term = ele_sym_poly.v[i]
  */
       __pyx_v__monoisotopic_mass = __pyx_f_7brainpy_2_c_11composition_element_monoisotopic_mass(__pyx_v_element_struct);
 
-      /* "brainpy/_c/isotopic_distribution.pyx":567
+      /* "brainpy/_c/isotopic_distribution.pyx":579
  *             _monoisotopic_mass = element_monoisotopic_mass(element_struct)
  * 
  *             polynomial_term = ele_sym_poly.v[i]             # <<<<<<<<<<<<<<
  *             temp = _element_count
  *             temp *= sign * polynomial_term
  */
       __pyx_v_polynomial_term = (__pyx_v_ele_sym_poly->v[__pyx_v_i]);
 
-      /* "brainpy/_c/isotopic_distribution.pyx":568
+      /* "brainpy/_c/isotopic_distribution.pyx":580
  * 
  *             polynomial_term = ele_sym_poly.v[i]
  *             temp = _element_count             # <<<<<<<<<<<<<<
  *             temp *= sign * polynomial_term
  *             temp *= base_intensity * _monoisotopic_mass
  */
       __pyx_v_temp = __pyx_v__element_count;
 
-      /* "brainpy/_c/isotopic_distribution.pyx":569
+      /* "brainpy/_c/isotopic_distribution.pyx":581
  *             polynomial_term = ele_sym_poly.v[i]
  *             temp = _element_count
  *             temp *= sign * polynomial_term             # <<<<<<<<<<<<<<
  *             temp *= base_intensity * _monoisotopic_mass
  *             center += temp
  */
       __pyx_v_temp = (__pyx_v_temp * (__pyx_v_sign * __pyx_v_polynomial_term));
 
-      /* "brainpy/_c/isotopic_distribution.pyx":570
+      /* "brainpy/_c/isotopic_distribution.pyx":582
  *             temp = _element_count
  *             temp *= sign * polynomial_term
  *             temp *= base_intensity * _monoisotopic_mass             # <<<<<<<<<<<<<<
  *             center += temp
  *             k += 1
  */
       __pyx_v_temp = (__pyx_v_temp * (__pyx_v_base_intensity * __pyx_v__monoisotopic_mass));
 
-      /* "brainpy/_c/isotopic_distribution.pyx":571
+      /* "brainpy/_c/isotopic_distribution.pyx":583
  *             temp *= sign * polynomial_term
  *             temp *= base_intensity * _monoisotopic_mass
  *             center += temp             # <<<<<<<<<<<<<<
  *             k += 1
  *         if probability_vector.v[i] == 0:
  */
       __pyx_v_center = (__pyx_v_center + __pyx_v_temp);
 
-      /* "brainpy/_c/isotopic_distribution.pyx":572
+      /* "brainpy/_c/isotopic_distribution.pyx":584
  *             temp *= base_intensity * _monoisotopic_mass
  *             center += temp
  *             k += 1             # <<<<<<<<<<<<<<
  *         if probability_vector.v[i] == 0:
  *             double_vector_append(mass_vector, 0)
  */
       __pyx_v_k = (__pyx_v_k + 1);
     }
 
-    /* "brainpy/_c/isotopic_distribution.pyx":573
+    /* "brainpy/_c/isotopic_distribution.pyx":585
  *             center += temp
  *             k += 1
  *         if probability_vector.v[i] == 0:             # <<<<<<<<<<<<<<
  *             double_vector_append(mass_vector, 0)
  *         else:
  */
     __pyx_t_2 = (((__pyx_v_probability_vector->v[__pyx_v_i]) == 0.0) != 0);
     if (__pyx_t_2) {
 
-      /* "brainpy/_c/isotopic_distribution.pyx":574
+      /* "brainpy/_c/isotopic_distribution.pyx":586
  *             k += 1
  *         if probability_vector.v[i] == 0:
  *             double_vector_append(mass_vector, 0)             # <<<<<<<<<<<<<<
  *         else:
  *             double_vector_append(mass_vector, center / probability_vector.v[i])
  */
       (void)(__pyx_f_7brainpy_2_c_13double_vector_double_vector_append(__pyx_v_mass_vector, 0.0));
 
-      /* "brainpy/_c/isotopic_distribution.pyx":573
+      /* "brainpy/_c/isotopic_distribution.pyx":585
  *             center += temp
  *             k += 1
  *         if probability_vector.v[i] == 0:             # <<<<<<<<<<<<<<
  *             double_vector_append(mass_vector, 0)
  *         else:
  */
       goto __pyx_L9;
     }
 
-    /* "brainpy/_c/isotopic_distribution.pyx":576
+    /* "brainpy/_c/isotopic_distribution.pyx":588
  *             double_vector_append(mass_vector, 0)
  *         else:
  *             double_vector_append(mass_vector, center / probability_vector.v[i])             # <<<<<<<<<<<<<<
  * 
  *     free_element_polynomial_map(ep_map)
  */
     /*else*/ {
       (void)(__pyx_f_7brainpy_2_c_13double_vector_double_vector_append(__pyx_v_mass_vector, (__pyx_v_center / (__pyx_v_probability_vector->v[__pyx_v_i]))));
     }
     __pyx_L9:;
   }
 
-  /* "brainpy/_c/isotopic_distribution.pyx":578
+  /* "brainpy/_c/isotopic_distribution.pyx":590
  *             double_vector_append(mass_vector, center / probability_vector.v[i])
  * 
  *     free_element_polynomial_map(ep_map)             # <<<<<<<<<<<<<<
  * 
  *     return mass_vector
  */
   __pyx_f_7brainpy_2_c_21isotopic_distribution_free_element_polynomial_map(__pyx_v_ep_map);
 
-  /* "brainpy/_c/isotopic_distribution.pyx":580
+  /* "brainpy/_c/isotopic_distribution.pyx":592
  *     free_element_polynomial_map(ep_map)
  * 
  *     return mass_vector             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = __pyx_v_mass_vector;
   goto __pyx_L0;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":523
+  /* "brainpy/_c/isotopic_distribution.pyx":535
  * 
  * @cython.cdivision
  * cdef dvec* id_center_mass_vector(IsotopicDistribution* distribution, dvec* probability_vector) nogil:             # <<<<<<<<<<<<<<
  *     cdef:
  *         dvec* mass_vector
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "brainpy/_c/isotopic_distribution.pyx":584
+/* "brainpy/_c/isotopic_distribution.pyx":596
  * 
  * @cython.cdivision
  * cdef PeakList* id_aggregated_isotopic_variants(IsotopicDistribution* distribution, int charge, double charge_carrier) nogil:             # <<<<<<<<<<<<<<
  *     cdef:
  *         dvec* probability_vector
  */
 
@@ -5742,442 +5742,442 @@
   size_t __pyx_t_3;
   long __pyx_t_4;
   long __pyx_t_5;
   int __pyx_t_6;
   double __pyx_t_7;
   struct __pyx_opt_args_7brainpy_2_c_11composition_mass_charge_ratio __pyx_t_8;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":595
+  /* "brainpy/_c/isotopic_distribution.pyx":607
  *         double center_mass_i, intensity_i
  * 
  *     probability_vector = id_probability_vector(distribution)             # <<<<<<<<<<<<<<
  *     center_mass_vector = id_center_mass_vector(distribution, probability_vector)
  * 
  */
   __pyx_v_probability_vector = __pyx_f_7brainpy_2_c_21isotopic_distribution_id_probability_vector(__pyx_v_distribution);
 
-  /* "brainpy/_c/isotopic_distribution.pyx":596
+  /* "brainpy/_c/isotopic_distribution.pyx":608
  * 
  *     probability_vector = id_probability_vector(distribution)
  *     center_mass_vector = id_center_mass_vector(distribution, probability_vector)             # <<<<<<<<<<<<<<
  * 
  *     peak_set = make_peak_list()
  */
   __pyx_v_center_mass_vector = __pyx_f_7brainpy_2_c_21isotopic_distribution_id_center_mass_vector(__pyx_v_distribution, __pyx_v_probability_vector);
 
-  /* "brainpy/_c/isotopic_distribution.pyx":598
+  /* "brainpy/_c/isotopic_distribution.pyx":610
  *     center_mass_vector = id_center_mass_vector(distribution, probability_vector)
  * 
  *     peak_set = make_peak_list()             # <<<<<<<<<<<<<<
  * 
  *     average_mass = 0
  */
   __pyx_v_peak_set = __pyx_f_7brainpy_2_c_21isotopic_distribution_make_peak_list();
 
-  /* "brainpy/_c/isotopic_distribution.pyx":600
+  /* "brainpy/_c/isotopic_distribution.pyx":612
  *     peak_set = make_peak_list()
  * 
  *     average_mass = 0             # <<<<<<<<<<<<<<
  *     total = 0
  * 
  */
   __pyx_v_average_mass = 0.0;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":601
+  /* "brainpy/_c/isotopic_distribution.pyx":613
  * 
  *     average_mass = 0
  *     total = 0             # <<<<<<<<<<<<<<
  * 
  *     for i in range(probability_vector.used):
  */
   __pyx_v_total = 0.0;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":603
+  /* "brainpy/_c/isotopic_distribution.pyx":615
  *     total = 0
  * 
  *     for i in range(probability_vector.used):             # <<<<<<<<<<<<<<
  *         total += probability_vector.v[i]
  * 
  */
   __pyx_t_1 = __pyx_v_probability_vector->used;
   __pyx_t_2 = __pyx_t_1;
   for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
     __pyx_v_i = __pyx_t_3;
 
-    /* "brainpy/_c/isotopic_distribution.pyx":604
+    /* "brainpy/_c/isotopic_distribution.pyx":616
  * 
  *     for i in range(probability_vector.used):
  *         total += probability_vector.v[i]             # <<<<<<<<<<<<<<
  * 
  *     for i in range(distribution.order + 1):
  */
     __pyx_v_total = (__pyx_v_total + (__pyx_v_probability_vector->v[__pyx_v_i]));
   }
 
-  /* "brainpy/_c/isotopic_distribution.pyx":606
+  /* "brainpy/_c/isotopic_distribution.pyx":618
  *         total += probability_vector.v[i]
  * 
  *     for i in range(distribution.order + 1):             # <<<<<<<<<<<<<<
  *         center_mass_i = center_mass_vector.v[i]
  *         intensity_i = probability_vector.v[i]
  */
   __pyx_t_4 = (__pyx_v_distribution->order + 1);
   __pyx_t_5 = __pyx_t_4;
   for (__pyx_t_1 = 0; __pyx_t_1 < __pyx_t_5; __pyx_t_1+=1) {
     __pyx_v_i = __pyx_t_1;
 
-    /* "brainpy/_c/isotopic_distribution.pyx":607
+    /* "brainpy/_c/isotopic_distribution.pyx":619
  * 
  *     for i in range(distribution.order + 1):
  *         center_mass_i = center_mass_vector.v[i]             # <<<<<<<<<<<<<<
  *         intensity_i = probability_vector.v[i]
  * 
  */
     __pyx_v_center_mass_i = (__pyx_v_center_mass_vector->v[__pyx_v_i]);
 
-    /* "brainpy/_c/isotopic_distribution.pyx":608
+    /* "brainpy/_c/isotopic_distribution.pyx":620
  *     for i in range(distribution.order + 1):
  *         center_mass_i = center_mass_vector.v[i]
  *         intensity_i = probability_vector.v[i]             # <<<<<<<<<<<<<<
  * 
  * 
  */
     __pyx_v_intensity_i = (__pyx_v_probability_vector->v[__pyx_v_i]);
 
-    /* "brainpy/_c/isotopic_distribution.pyx":611
+    /* "brainpy/_c/isotopic_distribution.pyx":623
  * 
  * 
  *         if charge != 0:             # <<<<<<<<<<<<<<
  *             adjusted_mz = mass_charge_ratio(center_mass_i, charge, charge_carrier)
  *         else:
  */
     __pyx_t_6 = ((__pyx_v_charge != 0) != 0);
     if (__pyx_t_6) {
 
-      /* "brainpy/_c/isotopic_distribution.pyx":612
+      /* "brainpy/_c/isotopic_distribution.pyx":624
  * 
  *         if charge != 0:
  *             adjusted_mz = mass_charge_ratio(center_mass_i, charge, charge_carrier)             # <<<<<<<<<<<<<<
  *         else:
  *             adjusted_mz = center_mass_i
  */
       __pyx_t_8.__pyx_n = 1;
       __pyx_t_8.charge_carrier = __pyx_v_charge_carrier;
       __pyx_t_7 = __pyx_f_7brainpy_2_c_11composition_mass_charge_ratio(__pyx_v_center_mass_i, __pyx_v_charge, &__pyx_t_8); 
       __pyx_v_adjusted_mz = __pyx_t_7;
 
-      /* "brainpy/_c/isotopic_distribution.pyx":611
+      /* "brainpy/_c/isotopic_distribution.pyx":623
  * 
  * 
  *         if charge != 0:             # <<<<<<<<<<<<<<
  *             adjusted_mz = mass_charge_ratio(center_mass_i, charge, charge_carrier)
  *         else:
  */
       goto __pyx_L7;
     }
 
-    /* "brainpy/_c/isotopic_distribution.pyx":614
+    /* "brainpy/_c/isotopic_distribution.pyx":626
  *             adjusted_mz = mass_charge_ratio(center_mass_i, charge, charge_carrier)
  *         else:
  *             adjusted_mz = center_mass_i             # <<<<<<<<<<<<<<
  * 
  * 
  */
     /*else*/ {
       __pyx_v_adjusted_mz = __pyx_v_center_mass_i;
     }
     __pyx_L7:;
 
-    /* "brainpy/_c/isotopic_distribution.pyx":617
+    /* "brainpy/_c/isotopic_distribution.pyx":629
  * 
  * 
  *         peak.mz = adjusted_mz             # <<<<<<<<<<<<<<
  *         peak.intensity = intensity_i / total
  *         peak.charge = charge
  */
     __pyx_v_peak.mz = __pyx_v_adjusted_mz;
 
-    /* "brainpy/_c/isotopic_distribution.pyx":618
+    /* "brainpy/_c/isotopic_distribution.pyx":630
  * 
  *         peak.mz = adjusted_mz
  *         peak.intensity = intensity_i / total             # <<<<<<<<<<<<<<
  *         peak.charge = charge
  * 
  */
     __pyx_v_peak.intensity = (__pyx_v_intensity_i / __pyx_v_total);
 
-    /* "brainpy/_c/isotopic_distribution.pyx":619
+    /* "brainpy/_c/isotopic_distribution.pyx":631
  *         peak.mz = adjusted_mz
  *         peak.intensity = intensity_i / total
  *         peak.charge = charge             # <<<<<<<<<<<<<<
  * 
  *         if peak.intensity < 1e-10:
  */
     __pyx_v_peak.charge = __pyx_v_charge;
 
-    /* "brainpy/_c/isotopic_distribution.pyx":621
+    /* "brainpy/_c/isotopic_distribution.pyx":633
  *         peak.charge = charge
  * 
  *         if peak.intensity < 1e-10:             # <<<<<<<<<<<<<<
  *             continue
  * 
  */
     __pyx_t_6 = ((__pyx_v_peak.intensity < 1e-10) != 0);
     if (__pyx_t_6) {
 
-      /* "brainpy/_c/isotopic_distribution.pyx":622
+      /* "brainpy/_c/isotopic_distribution.pyx":634
  * 
  *         if peak.intensity < 1e-10:
  *             continue             # <<<<<<<<<<<<<<
  * 
  *         peak_list_append(peak_set, &peak)
  */
       goto __pyx_L5_continue;
 
-      /* "brainpy/_c/isotopic_distribution.pyx":621
+      /* "brainpy/_c/isotopic_distribution.pyx":633
  *         peak.charge = charge
  * 
  *         if peak.intensity < 1e-10:             # <<<<<<<<<<<<<<
  *             continue
  * 
  */
     }
 
-    /* "brainpy/_c/isotopic_distribution.pyx":624
+    /* "brainpy/_c/isotopic_distribution.pyx":636
  *             continue
  * 
  *         peak_list_append(peak_set, &peak)             # <<<<<<<<<<<<<<
  * 
  *         average_mass += adjusted_mz * intensity_i
  */
     __pyx_f_7brainpy_2_c_21isotopic_distribution_peak_list_append(__pyx_v_peak_set, (&__pyx_v_peak));
 
-    /* "brainpy/_c/isotopic_distribution.pyx":626
+    /* "brainpy/_c/isotopic_distribution.pyx":638
  *         peak_list_append(peak_set, &peak)
  * 
  *         average_mass += adjusted_mz * intensity_i             # <<<<<<<<<<<<<<
  * 
  *     average_mass /= total
  */
     __pyx_v_average_mass = (__pyx_v_average_mass + (__pyx_v_adjusted_mz * __pyx_v_intensity_i));
     __pyx_L5_continue:;
   }
 
-  /* "brainpy/_c/isotopic_distribution.pyx":628
+  /* "brainpy/_c/isotopic_distribution.pyx":640
  *         average_mass += adjusted_mz * intensity_i
  * 
  *     average_mass /= total             # <<<<<<<<<<<<<<
  * 
  *     free_double_vector(probability_vector)
  */
   __pyx_v_average_mass = (__pyx_v_average_mass / __pyx_v_total);
 
-  /* "brainpy/_c/isotopic_distribution.pyx":630
+  /* "brainpy/_c/isotopic_distribution.pyx":642
  *     average_mass /= total
  * 
  *     free_double_vector(probability_vector)             # <<<<<<<<<<<<<<
  *     free_double_vector(center_mass_vector)
  * 
  */
   __pyx_f_7brainpy_2_c_13double_vector_free_double_vector(__pyx_v_probability_vector);
 
-  /* "brainpy/_c/isotopic_distribution.pyx":631
+  /* "brainpy/_c/isotopic_distribution.pyx":643
  * 
  *     free_double_vector(probability_vector)
  *     free_double_vector(center_mass_vector)             # <<<<<<<<<<<<<<
  * 
  *     distribution.average_mass = average_mass
  */
   __pyx_f_7brainpy_2_c_13double_vector_free_double_vector(__pyx_v_center_mass_vector);
 
-  /* "brainpy/_c/isotopic_distribution.pyx":633
+  /* "brainpy/_c/isotopic_distribution.pyx":645
  *     free_double_vector(center_mass_vector)
  * 
  *     distribution.average_mass = average_mass             # <<<<<<<<<<<<<<
  * 
  *     sort_by_mz(peak_set)
  */
   __pyx_v_distribution->average_mass = __pyx_v_average_mass;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":635
+  /* "brainpy/_c/isotopic_distribution.pyx":647
  *     distribution.average_mass = average_mass
  * 
  *     sort_by_mz(peak_set)             # <<<<<<<<<<<<<<
  *     return peak_set
  * 
  */
   __pyx_f_7brainpy_2_c_21isotopic_distribution_sort_by_mz(__pyx_v_peak_set);
 
-  /* "brainpy/_c/isotopic_distribution.pyx":636
+  /* "brainpy/_c/isotopic_distribution.pyx":648
  * 
  *     sort_by_mz(peak_set)
  *     return peak_set             # <<<<<<<<<<<<<<
  * 
  * cdef void sort_by_mz(PeakList* peaklist) nogil:
  */
   __pyx_r = __pyx_v_peak_set;
   goto __pyx_L0;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":584
+  /* "brainpy/_c/isotopic_distribution.pyx":596
  * 
  * @cython.cdivision
  * cdef PeakList* id_aggregated_isotopic_variants(IsotopicDistribution* distribution, int charge, double charge_carrier) nogil:             # <<<<<<<<<<<<<<
  *     cdef:
  *         dvec* probability_vector
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "brainpy/_c/isotopic_distribution.pyx":638
+/* "brainpy/_c/isotopic_distribution.pyx":650
  *     return peak_set
  * 
  * cdef void sort_by_mz(PeakList* peaklist) nogil:             # <<<<<<<<<<<<<<
  *     qsort(peaklist.peaks, peaklist.used, sizeof(Peak), compare_by_mz)
  * 
  */
 
 static void __pyx_f_7brainpy_2_c_21isotopic_distribution_sort_by_mz(struct __pyx_t_7brainpy_2_c_21isotopic_distribution_PeakList *__pyx_v_peaklist) {
 
-  /* "brainpy/_c/isotopic_distribution.pyx":639
+  /* "brainpy/_c/isotopic_distribution.pyx":651
  * 
  * cdef void sort_by_mz(PeakList* peaklist) nogil:
  *     qsort(peaklist.peaks, peaklist.used, sizeof(Peak), compare_by_mz)             # <<<<<<<<<<<<<<
  * 
  * cdef int compare_by_mz(const void * a, const void * b) nogil:
  */
   qsort(__pyx_v_peaklist->peaks, __pyx_v_peaklist->used, (sizeof(struct __pyx_t_7brainpy_2_c_21isotopic_distribution_Peak)), __pyx_f_7brainpy_2_c_21isotopic_distribution_compare_by_mz);
 
-  /* "brainpy/_c/isotopic_distribution.pyx":638
+  /* "brainpy/_c/isotopic_distribution.pyx":650
  *     return peak_set
  * 
  * cdef void sort_by_mz(PeakList* peaklist) nogil:             # <<<<<<<<<<<<<<
  *     qsort(peaklist.peaks, peaklist.used, sizeof(Peak), compare_by_mz)
  * 
  */
 
   /* function exit code */
 }
 
-/* "brainpy/_c/isotopic_distribution.pyx":641
+/* "brainpy/_c/isotopic_distribution.pyx":653
  *     qsort(peaklist.peaks, peaklist.used, sizeof(Peak), compare_by_mz)
  * 
  * cdef int compare_by_mz(const void * a, const void * b) nogil:             # <<<<<<<<<<<<<<
  *     if (<Peak*>a).mz < (<Peak*>b).mz:
  *         return -1
  */
 
 static int __pyx_f_7brainpy_2_c_21isotopic_distribution_compare_by_mz(void const *__pyx_v_a, void const *__pyx_v_b) {
   int __pyx_r;
   int __pyx_t_1;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":642
+  /* "brainpy/_c/isotopic_distribution.pyx":654
  * 
  * cdef int compare_by_mz(const void * a, const void * b) nogil:
  *     if (<Peak*>a).mz < (<Peak*>b).mz:             # <<<<<<<<<<<<<<
  *         return -1
  *     elif (<Peak*>a).mz == (<Peak*>b).mz:
  */
   __pyx_t_1 = ((((struct __pyx_t_7brainpy_2_c_21isotopic_distribution_Peak *)__pyx_v_a)->mz < ((struct __pyx_t_7brainpy_2_c_21isotopic_distribution_Peak *)__pyx_v_b)->mz) != 0);
   if (__pyx_t_1) {
 
-    /* "brainpy/_c/isotopic_distribution.pyx":643
+    /* "brainpy/_c/isotopic_distribution.pyx":655
  * cdef int compare_by_mz(const void * a, const void * b) nogil:
  *     if (<Peak*>a).mz < (<Peak*>b).mz:
  *         return -1             # <<<<<<<<<<<<<<
  *     elif (<Peak*>a).mz == (<Peak*>b).mz:
  *         return 0
  */
     __pyx_r = -1;
     goto __pyx_L0;
 
-    /* "brainpy/_c/isotopic_distribution.pyx":642
+    /* "brainpy/_c/isotopic_distribution.pyx":654
  * 
  * cdef int compare_by_mz(const void * a, const void * b) nogil:
  *     if (<Peak*>a).mz < (<Peak*>b).mz:             # <<<<<<<<<<<<<<
  *         return -1
  *     elif (<Peak*>a).mz == (<Peak*>b).mz:
  */
   }
 
-  /* "brainpy/_c/isotopic_distribution.pyx":644
+  /* "brainpy/_c/isotopic_distribution.pyx":656
  *     if (<Peak*>a).mz < (<Peak*>b).mz:
  *         return -1
  *     elif (<Peak*>a).mz == (<Peak*>b).mz:             # <<<<<<<<<<<<<<
  *         return 0
  *     elif (<Peak*>a).mz > (<Peak*>b).mz:
  */
   __pyx_t_1 = ((((struct __pyx_t_7brainpy_2_c_21isotopic_distribution_Peak *)__pyx_v_a)->mz == ((struct __pyx_t_7brainpy_2_c_21isotopic_distribution_Peak *)__pyx_v_b)->mz) != 0);
   if (__pyx_t_1) {
 
-    /* "brainpy/_c/isotopic_distribution.pyx":645
+    /* "brainpy/_c/isotopic_distribution.pyx":657
  *         return -1
  *     elif (<Peak*>a).mz == (<Peak*>b).mz:
  *         return 0             # <<<<<<<<<<<<<<
  *     elif (<Peak*>a).mz > (<Peak*>b).mz:
  *         return 1
  */
     __pyx_r = 0;
     goto __pyx_L0;
 
-    /* "brainpy/_c/isotopic_distribution.pyx":644
+    /* "brainpy/_c/isotopic_distribution.pyx":656
  *     if (<Peak*>a).mz < (<Peak*>b).mz:
  *         return -1
  *     elif (<Peak*>a).mz == (<Peak*>b).mz:             # <<<<<<<<<<<<<<
  *         return 0
  *     elif (<Peak*>a).mz > (<Peak*>b).mz:
  */
   }
 
-  /* "brainpy/_c/isotopic_distribution.pyx":646
+  /* "brainpy/_c/isotopic_distribution.pyx":658
  *     elif (<Peak*>a).mz == (<Peak*>b).mz:
  *         return 0
  *     elif (<Peak*>a).mz > (<Peak*>b).mz:             # <<<<<<<<<<<<<<
  *         return 1
  * 
  */
   __pyx_t_1 = ((((struct __pyx_t_7brainpy_2_c_21isotopic_distribution_Peak *)__pyx_v_a)->mz > ((struct __pyx_t_7brainpy_2_c_21isotopic_distribution_Peak *)__pyx_v_b)->mz) != 0);
   if (__pyx_t_1) {
 
-    /* "brainpy/_c/isotopic_distribution.pyx":647
+    /* "brainpy/_c/isotopic_distribution.pyx":659
  *         return 0
  *     elif (<Peak*>a).mz > (<Peak*>b).mz:
  *         return 1             # <<<<<<<<<<<<<<
  * 
  * 
  */
     __pyx_r = 1;
     goto __pyx_L0;
 
-    /* "brainpy/_c/isotopic_distribution.pyx":646
+    /* "brainpy/_c/isotopic_distribution.pyx":658
  *     elif (<Peak*>a).mz == (<Peak*>b).mz:
  *         return 0
  *     elif (<Peak*>a).mz > (<Peak*>b).mz:             # <<<<<<<<<<<<<<
  *         return 1
  * 
  */
   }
 
-  /* "brainpy/_c/isotopic_distribution.pyx":641
+  /* "brainpy/_c/isotopic_distribution.pyx":653
  *     qsort(peaklist.peaks, peaklist.used, sizeof(Peak), compare_by_mz)
  * 
  * cdef int compare_by_mz(const void * a, const void * b) nogil:             # <<<<<<<<<<<<<<
  *     if (<Peak*>a).mz < (<Peak*>b).mz:
  *         return -1
  */
 
   /* function exit code */
   __pyx_r = 0;
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "brainpy/_c/isotopic_distribution.pyx":650
+/* "brainpy/_c/isotopic_distribution.pyx":662
  * 
  * 
  * cpdef bint check_composition_non_negative(dict composition):             # <<<<<<<<<<<<<<
  *     cdef:
  *         bint negative_element
  */
 
@@ -6198,189 +6198,189 @@
   PyObject *(*__pyx_t_8)(PyObject *);
   int __pyx_t_9;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("check_composition_non_negative", 0);
 
-  /* "brainpy/_c/isotopic_distribution.pyx":656
+  /* "brainpy/_c/isotopic_distribution.pyx":668
  *         object v
  * 
  *     negative_element = False             # <<<<<<<<<<<<<<
  *     for k, v in composition.items():
  *         if v < 0:
  */
   __pyx_v_negative_element = 0;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":657
+  /* "brainpy/_c/isotopic_distribution.pyx":669
  * 
  *     negative_element = False
  *     for k, v in composition.items():             # <<<<<<<<<<<<<<
  *         if v < 0:
  *             negative_element = True
  */
   if (unlikely(__pyx_v_composition == Py_None)) {
     PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "items");
-    __PYX_ERR(0, 657, __pyx_L1_error)
+    __PYX_ERR(0, 669, __pyx_L1_error)
   }
-  __pyx_t_1 = __Pyx_PyDict_Items(__pyx_v_composition); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 657, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_Items(__pyx_v_composition); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 669, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (likely(PyList_CheckExact(__pyx_t_1)) || PyTuple_CheckExact(__pyx_t_1)) {
     __pyx_t_2 = __pyx_t_1; __Pyx_INCREF(__pyx_t_2); __pyx_t_3 = 0;
     __pyx_t_4 = NULL;
   } else {
-    __pyx_t_3 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 657, __pyx_L1_error)
+    __pyx_t_3 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 669, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = Py_TYPE(__pyx_t_2)->tp_iternext; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 657, __pyx_L1_error)
+    __pyx_t_4 = Py_TYPE(__pyx_t_2)->tp_iternext; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 669, __pyx_L1_error)
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   for (;;) {
     if (likely(!__pyx_t_4)) {
       if (likely(PyList_CheckExact(__pyx_t_2))) {
         if (__pyx_t_3 >= PyList_GET_SIZE(__pyx_t_2)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_1 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_1); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(0, 657, __pyx_L1_error)
+        __pyx_t_1 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_1); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(0, 669, __pyx_L1_error)
         #else
-        __pyx_t_1 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 657, __pyx_L1_error)
+        __pyx_t_1 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 669, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         #endif
       } else {
         if (__pyx_t_3 >= PyTuple_GET_SIZE(__pyx_t_2)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_1 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_1); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(0, 657, __pyx_L1_error)
+        __pyx_t_1 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_1); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(0, 669, __pyx_L1_error)
         #else
-        __pyx_t_1 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 657, __pyx_L1_error)
+        __pyx_t_1 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 669, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         #endif
       }
     } else {
       __pyx_t_1 = __pyx_t_4(__pyx_t_2);
       if (unlikely(!__pyx_t_1)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(0, 657, __pyx_L1_error)
+          else __PYX_ERR(0, 669, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_1);
     }
     if ((likely(PyTuple_CheckExact(__pyx_t_1))) || (PyList_CheckExact(__pyx_t_1))) {
       PyObject* sequence = __pyx_t_1;
       Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
       if (unlikely(size != 2)) {
         if (size > 2) __Pyx_RaiseTooManyValuesError(2);
         else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-        __PYX_ERR(0, 657, __pyx_L1_error)
+        __PYX_ERR(0, 669, __pyx_L1_error)
       }
       #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
       if (likely(PyTuple_CheckExact(sequence))) {
         __pyx_t_5 = PyTuple_GET_ITEM(sequence, 0); 
         __pyx_t_6 = PyTuple_GET_ITEM(sequence, 1); 
       } else {
         __pyx_t_5 = PyList_GET_ITEM(sequence, 0); 
         __pyx_t_6 = PyList_GET_ITEM(sequence, 1); 
       }
       __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(__pyx_t_6);
       #else
-      __pyx_t_5 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 657, __pyx_L1_error)
+      __pyx_t_5 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 669, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
-      __pyx_t_6 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 657, __pyx_L1_error)
+      __pyx_t_6 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 669, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     } else {
       Py_ssize_t index = -1;
-      __pyx_t_7 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 657, __pyx_L1_error)
+      __pyx_t_7 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 669, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __pyx_t_8 = Py_TYPE(__pyx_t_7)->tp_iternext;
       index = 0; __pyx_t_5 = __pyx_t_8(__pyx_t_7); if (unlikely(!__pyx_t_5)) goto __pyx_L5_unpacking_failed;
       __Pyx_GOTREF(__pyx_t_5);
       index = 1; __pyx_t_6 = __pyx_t_8(__pyx_t_7); if (unlikely(!__pyx_t_6)) goto __pyx_L5_unpacking_failed;
       __Pyx_GOTREF(__pyx_t_6);
-      if (__Pyx_IternextUnpackEndCheck(__pyx_t_8(__pyx_t_7), 2) < 0) __PYX_ERR(0, 657, __pyx_L1_error)
+      if (__Pyx_IternextUnpackEndCheck(__pyx_t_8(__pyx_t_7), 2) < 0) __PYX_ERR(0, 669, __pyx_L1_error)
       __pyx_t_8 = NULL;
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
       goto __pyx_L6_unpacking_done;
       __pyx_L5_unpacking_failed:;
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
       __pyx_t_8 = NULL;
       if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-      __PYX_ERR(0, 657, __pyx_L1_error)
+      __PYX_ERR(0, 669, __pyx_L1_error)
       __pyx_L6_unpacking_done:;
     }
-    if (!(likely(PyString_CheckExact(__pyx_t_5))||((__pyx_t_5) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "str", Py_TYPE(__pyx_t_5)->tp_name), 0))) __PYX_ERR(0, 657, __pyx_L1_error)
+    if (!(likely(PyString_CheckExact(__pyx_t_5))||((__pyx_t_5) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "str", Py_TYPE(__pyx_t_5)->tp_name), 0))) __PYX_ERR(0, 669, __pyx_L1_error)
     __Pyx_XDECREF_SET(__pyx_v_k, ((PyObject*)__pyx_t_5));
     __pyx_t_5 = 0;
     __Pyx_XDECREF_SET(__pyx_v_v, __pyx_t_6);
     __pyx_t_6 = 0;
 
-    /* "brainpy/_c/isotopic_distribution.pyx":658
+    /* "brainpy/_c/isotopic_distribution.pyx":670
  *     negative_element = False
  *     for k, v in composition.items():
  *         if v < 0:             # <<<<<<<<<<<<<<
  *             negative_element = True
  *             break
  */
-    __pyx_t_1 = PyObject_RichCompare(__pyx_v_v, __pyx_int_0, Py_LT); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 658, __pyx_L1_error)
-    __pyx_t_9 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_9 < 0)) __PYX_ERR(0, 658, __pyx_L1_error)
+    __pyx_t_1 = PyObject_RichCompare(__pyx_v_v, __pyx_int_0, Py_LT); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 670, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_9 < 0)) __PYX_ERR(0, 670, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     if (__pyx_t_9) {
 
-      /* "brainpy/_c/isotopic_distribution.pyx":659
+      /* "brainpy/_c/isotopic_distribution.pyx":671
  *     for k, v in composition.items():
  *         if v < 0:
  *             negative_element = True             # <<<<<<<<<<<<<<
  *             break
  *     return negative_element
  */
       __pyx_v_negative_element = 1;
 
-      /* "brainpy/_c/isotopic_distribution.pyx":660
+      /* "brainpy/_c/isotopic_distribution.pyx":672
  *         if v < 0:
  *             negative_element = True
  *             break             # <<<<<<<<<<<<<<
  *     return negative_element
  * 
  */
       goto __pyx_L4_break;
 
-      /* "brainpy/_c/isotopic_distribution.pyx":658
+      /* "brainpy/_c/isotopic_distribution.pyx":670
  *     negative_element = False
  *     for k, v in composition.items():
  *         if v < 0:             # <<<<<<<<<<<<<<
  *             negative_element = True
  *             break
  */
     }
 
-    /* "brainpy/_c/isotopic_distribution.pyx":657
+    /* "brainpy/_c/isotopic_distribution.pyx":669
  * 
  *     negative_element = False
  *     for k, v in composition.items():             # <<<<<<<<<<<<<<
  *         if v < 0:
  *             negative_element = True
  */
   }
   __pyx_L4_break:;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":661
+  /* "brainpy/_c/isotopic_distribution.pyx":673
  *             negative_element = True
  *             break
  *     return negative_element             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = __pyx_v_negative_element;
   goto __pyx_L0;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":650
+  /* "brainpy/_c/isotopic_distribution.pyx":662
  * 
  * 
  * cpdef bint check_composition_non_negative(dict composition):             # <<<<<<<<<<<<<<
  *     cdef:
  *         bint negative_element
  */
 
@@ -6406,15 +6406,15 @@
 static PyObject *__pyx_pw_7brainpy_2_c_21isotopic_distribution_1check_composition_non_negative(PyObject *__pyx_self, PyObject *__pyx_v_composition) {
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("check_composition_non_negative (wrapper)", 0);
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_composition), (&PyDict_Type), 1, "composition", 1))) __PYX_ERR(0, 650, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_composition), (&PyDict_Type), 1, "composition", 1))) __PYX_ERR(0, 662, __pyx_L1_error)
   __pyx_r = __pyx_pf_7brainpy_2_c_21isotopic_distribution_check_composition_non_negative(__pyx_self, ((PyObject*)__pyx_v_composition));
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -6427,15 +6427,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("check_composition_non_negative", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyBool_FromLong(__pyx_f_7brainpy_2_c_21isotopic_distribution_check_composition_non_negative(__pyx_v_composition, 0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 650, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyBool_FromLong(__pyx_f_7brainpy_2_c_21isotopic_distribution_check_composition_non_negative(__pyx_v_composition, 0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 662, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -6444,15 +6444,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "brainpy/_c/isotopic_distribution.pyx":664
+/* "brainpy/_c/isotopic_distribution.pyx":676
  * 
  * 
  * cdef int guess_npeaks(Composition* composition_struct, size_t max_npeaks, ElementCache* cache=NULL) nogil:             # <<<<<<<<<<<<<<
  *     cdef:
  *         int max_n_variants, npeaks
  */
 
@@ -6468,33 +6468,33 @@
   size_t __pyx_t_5;
   if (__pyx_optional_args) {
     if (__pyx_optional_args->__pyx_n > 0) {
       __pyx_v_cache = __pyx_optional_args->cache;
     }
   }
 
-  /* "brainpy/_c/isotopic_distribution.pyx":667
+  /* "brainpy/_c/isotopic_distribution.pyx":679
  *     cdef:
  *         int max_n_variants, npeaks
  *     max_n_variants = max_variants(composition_struct, cache)             # <<<<<<<<<<<<<<
  *     npeaks = <int>sqrt(max_n_variants) - 2
  *     npeaks = min(max(npeaks, 3), max_npeaks)
  */
   __pyx_v_max_n_variants = __pyx_f_7brainpy_2_c_21isotopic_distribution_max_variants(__pyx_v_composition_struct, __pyx_v_cache);
 
-  /* "brainpy/_c/isotopic_distribution.pyx":668
+  /* "brainpy/_c/isotopic_distribution.pyx":680
  *         int max_n_variants, npeaks
  *     max_n_variants = max_variants(composition_struct, cache)
  *     npeaks = <int>sqrt(max_n_variants) - 2             # <<<<<<<<<<<<<<
  *     npeaks = min(max(npeaks, 3), max_npeaks)
  *     return npeaks
  */
   __pyx_v_npeaks = (((int)sqrt(__pyx_v_max_n_variants)) - 2);
 
-  /* "brainpy/_c/isotopic_distribution.pyx":669
+  /* "brainpy/_c/isotopic_distribution.pyx":681
  *     max_n_variants = max_variants(composition_struct, cache)
  *     npeaks = <int>sqrt(max_n_variants) - 2
  *     npeaks = min(max(npeaks, 3), max_npeaks)             # <<<<<<<<<<<<<<
  *     return npeaks
  * 
  */
   __pyx_t_1 = __pyx_v_max_npeaks;
@@ -6509,38 +6509,38 @@
   if (((__pyx_t_1 < __pyx_t_2) != 0)) {
     __pyx_t_5 = __pyx_t_1;
   } else {
     __pyx_t_5 = __pyx_t_2;
   }
   __pyx_v_npeaks = __pyx_t_5;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":670
+  /* "brainpy/_c/isotopic_distribution.pyx":682
  *     npeaks = <int>sqrt(max_n_variants) - 2
  *     npeaks = min(max(npeaks, 3), max_npeaks)
  *     return npeaks             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = __pyx_v_npeaks;
   goto __pyx_L0;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":664
+  /* "brainpy/_c/isotopic_distribution.pyx":676
  * 
  * 
  * cdef int guess_npeaks(Composition* composition_struct, size_t max_npeaks, ElementCache* cache=NULL) nogil:             # <<<<<<<<<<<<<<
  *     cdef:
  *         int max_n_variants, npeaks
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "brainpy/_c/isotopic_distribution.pyx":673
+/* "brainpy/_c/isotopic_distribution.pyx":685
  * 
  * 
  * def pyisotopic_variants(object composition not None, object npeaks=None, int charge=0,             # <<<<<<<<<<<<<<
  *                         double charge_carrier=PROTON):
  *     '''
  */
 
@@ -6599,15 +6599,15 @@
         case  3:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_charge_carrier);
           if (value) { values[3] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "pyisotopic_variants") < 0)) __PYX_ERR(0, 673, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "pyisotopic_variants") < 0)) __PYX_ERR(0, 685, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
         CYTHON_FALLTHROUGH;
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
@@ -6617,34 +6617,34 @@
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_composition = values[0];
     __pyx_v_npeaks = values[1];
     if (values[2]) {
-      __pyx_v_charge = __Pyx_PyInt_As_int(values[2]); if (unlikely((__pyx_v_charge == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 673, __pyx_L3_error)
+      __pyx_v_charge = __Pyx_PyInt_As_int(values[2]); if (unlikely((__pyx_v_charge == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 685, __pyx_L3_error)
     } else {
       __pyx_v_charge = ((int)0);
     }
     if (values[3]) {
-      __pyx_v_charge_carrier = __pyx_PyFloat_AsDouble(values[3]); if (unlikely((__pyx_v_charge_carrier == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 674, __pyx_L3_error)
+      __pyx_v_charge_carrier = __pyx_PyFloat_AsDouble(values[3]); if (unlikely((__pyx_v_charge_carrier == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 686, __pyx_L3_error)
     } else {
       __pyx_v_charge_carrier = __pyx_k_;
     }
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("pyisotopic_variants", 0, 1, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 673, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("pyisotopic_variants", 0, 1, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 685, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("brainpy._c.isotopic_distribution.pyisotopic_variants", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   if (unlikely(((PyObject *)__pyx_v_composition) == Py_None)) {
-    PyErr_Format(PyExc_TypeError, "Argument '%.200s' must not be None", "composition"); __PYX_ERR(0, 673, __pyx_L1_error)
+    PyErr_Format(PyExc_TypeError, "Argument '%.200s' must not be None", "composition"); __PYX_ERR(0, 685, __pyx_L1_error)
   }
   __pyx_r = __pyx_pf_7brainpy_2_c_21isotopic_distribution_2pyisotopic_variants(__pyx_self, __pyx_v_composition, __pyx_v_npeaks, __pyx_v_charge, __pyx_v_charge_carrier);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
@@ -6659,33 +6659,33 @@
   PyObject *__pyx_t_1 = NULL;
   struct __pyx_opt_args_7brainpy_2_c_21isotopic_distribution__isotopic_variants __pyx_t_2;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("pyisotopic_variants", 0);
 
-  /* "brainpy/_c/isotopic_distribution.pyx":697
+  /* "brainpy/_c/isotopic_distribution.pyx":709
  *     list of TheoreticalPeak
  *     '''
  *     return _isotopic_variants(composition, npeaks, charge, charge_carrier)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_2.__pyx_n = 3;
   __pyx_t_2.npeaks = __pyx_v_npeaks;
   __pyx_t_2.charge = __pyx_v_charge;
   __pyx_t_2.charge_carrier = __pyx_v_charge_carrier;
-  __pyx_t_1 = __pyx_f_7brainpy_2_c_21isotopic_distribution__isotopic_variants(__pyx_v_composition, 0, &__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 697, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_7brainpy_2_c_21isotopic_distribution__isotopic_variants(__pyx_v_composition, 0, &__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 709, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":673
+  /* "brainpy/_c/isotopic_distribution.pyx":685
  * 
  * 
  * def pyisotopic_variants(object composition not None, object npeaks=None, int charge=0,             # <<<<<<<<<<<<<<
  *                         double charge_carrier=PROTON):
  *     '''
  */
 
@@ -6696,15 +6696,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "brainpy/_c/isotopic_distribution.pyx":700
+/* "brainpy/_c/isotopic_distribution.pyx":712
  * 
  * 
  * cpdef list _isotopic_variants(object composition, object npeaks=None, int charge=0, double charge_carrier=PROTON):             # <<<<<<<<<<<<<<
  *     '''
  *     Compute a peak list representing the theoretical isotopic cluster for `composition`.
  */
 
@@ -6736,148 +6736,148 @@
         if (__pyx_optional_args->__pyx_n > 2) {
           __pyx_v_charge_carrier = __pyx_optional_args->charge_carrier;
         }
       }
     }
   }
 
-  /* "brainpy/_c/isotopic_distribution.pyx":730
+  /* "brainpy/_c/isotopic_distribution.pyx":742
  *         int _npeaks, max_n_variants
  * 
  *     composition_struct = dict_to_composition(dict(composition))             # <<<<<<<<<<<<<<
  *     if validate_composition(composition_struct) != 0:
  *         free_composition(composition_struct)
  */
-  __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyDict_Type)), __pyx_v_composition); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 730, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyDict_Type)), __pyx_v_composition); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 742, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_composition_struct = __pyx_f_7brainpy_2_c_11composition_dict_to_composition(((PyObject*)__pyx_t_1));
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":731
+  /* "brainpy/_c/isotopic_distribution.pyx":743
  * 
  *     composition_struct = dict_to_composition(dict(composition))
  *     if validate_composition(composition_struct) != 0:             # <<<<<<<<<<<<<<
  *         free_composition(composition_struct)
  *         raise KeyError("Unrecognized Isotope")
  */
   __pyx_t_2 = ((__pyx_f_7brainpy_2_c_21isotopic_distribution_validate_composition(__pyx_v_composition_struct) != 0) != 0);
   if (unlikely(__pyx_t_2)) {
 
-    /* "brainpy/_c/isotopic_distribution.pyx":732
+    /* "brainpy/_c/isotopic_distribution.pyx":744
  *     composition_struct = dict_to_composition(dict(composition))
  *     if validate_composition(composition_struct) != 0:
  *         free_composition(composition_struct)             # <<<<<<<<<<<<<<
  *         raise KeyError("Unrecognized Isotope")
  * 
  */
     __pyx_f_7brainpy_2_c_11composition_free_composition(__pyx_v_composition_struct);
 
-    /* "brainpy/_c/isotopic_distribution.pyx":733
+    /* "brainpy/_c/isotopic_distribution.pyx":745
  *     if validate_composition(composition_struct) != 0:
  *         free_composition(composition_struct)
  *         raise KeyError("Unrecognized Isotope")             # <<<<<<<<<<<<<<
  * 
  *     if npeaks is None:
  */
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_KeyError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 733, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_KeyError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 745, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_Raise(__pyx_t_1, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __PYX_ERR(0, 733, __pyx_L1_error)
+    __PYX_ERR(0, 745, __pyx_L1_error)
 
-    /* "brainpy/_c/isotopic_distribution.pyx":731
+    /* "brainpy/_c/isotopic_distribution.pyx":743
  * 
  *     composition_struct = dict_to_composition(dict(composition))
  *     if validate_composition(composition_struct) != 0:             # <<<<<<<<<<<<<<
  *         free_composition(composition_struct)
  *         raise KeyError("Unrecognized Isotope")
  */
   }
 
-  /* "brainpy/_c/isotopic_distribution.pyx":735
+  /* "brainpy/_c/isotopic_distribution.pyx":747
  *         raise KeyError("Unrecognized Isotope")
  * 
  *     if npeaks is None:             # <<<<<<<<<<<<<<
  *         _npeaks = guess_npeaks(composition_struct, 300)
  *     else:
  */
   __pyx_t_2 = (__pyx_v_npeaks == Py_None);
   __pyx_t_3 = (__pyx_t_2 != 0);
   if (__pyx_t_3) {
 
-    /* "brainpy/_c/isotopic_distribution.pyx":736
+    /* "brainpy/_c/isotopic_distribution.pyx":748
  * 
  *     if npeaks is None:
  *         _npeaks = guess_npeaks(composition_struct, 300)             # <<<<<<<<<<<<<<
  *     else:
  *         # The npeaks variable is left as a Python-level variable to
  */
     __pyx_v__npeaks = __pyx_f_7brainpy_2_c_21isotopic_distribution_guess_npeaks(__pyx_v_composition_struct, 0x12C, NULL);
 
-    /* "brainpy/_c/isotopic_distribution.pyx":735
+    /* "brainpy/_c/isotopic_distribution.pyx":747
  *         raise KeyError("Unrecognized Isotope")
  * 
  *     if npeaks is None:             # <<<<<<<<<<<<<<
  *         _npeaks = guess_npeaks(composition_struct, 300)
  *     else:
  */
     goto __pyx_L4;
   }
 
-  /* "brainpy/_c/isotopic_distribution.pyx":740
+  /* "brainpy/_c/isotopic_distribution.pyx":752
  *         # The npeaks variable is left as a Python-level variable to
  *         # allow it to be any Python numeric type
  *         _npeaks = npeaks - 1             # <<<<<<<<<<<<<<
  * 
  *     with nogil:
  */
   /*else*/ {
-    __pyx_t_1 = __Pyx_PyInt_SubtractObjC(__pyx_v_npeaks, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 740, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyInt_SubtractObjC(__pyx_v_npeaks, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 752, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_4 = __Pyx_PyInt_As_int(__pyx_t_1); if (unlikely((__pyx_t_4 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 740, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_As_int(__pyx_t_1); if (unlikely((__pyx_t_4 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 752, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_v__npeaks = __pyx_t_4;
   }
   __pyx_L4:;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":742
+  /* "brainpy/_c/isotopic_distribution.pyx":754
  *         _npeaks = npeaks - 1
  * 
  *     with nogil:             # <<<<<<<<<<<<<<
  *         dist = make_isotopic_distribution(composition_struct, _npeaks)
  *         peak_set = id_aggregated_isotopic_variants(dist, charge, charge_carrier)
  */
   {
       #ifdef WITH_THREAD
       PyThreadState *_save;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "brainpy/_c/isotopic_distribution.pyx":743
+        /* "brainpy/_c/isotopic_distribution.pyx":755
  * 
  *     with nogil:
  *         dist = make_isotopic_distribution(composition_struct, _npeaks)             # <<<<<<<<<<<<<<
  *         peak_set = id_aggregated_isotopic_variants(dist, charge, charge_carrier)
  * 
  */
         __pyx_v_dist = __pyx_f_7brainpy_2_c_21isotopic_distribution_make_isotopic_distribution(__pyx_v_composition_struct, __pyx_v__npeaks, NULL);
 
-        /* "brainpy/_c/isotopic_distribution.pyx":744
+        /* "brainpy/_c/isotopic_distribution.pyx":756
  *     with nogil:
  *         dist = make_isotopic_distribution(composition_struct, _npeaks)
  *         peak_set = id_aggregated_isotopic_variants(dist, charge, charge_carrier)             # <<<<<<<<<<<<<<
  * 
  *     peaklist = peaklist_to_list(peak_set)
  */
         __pyx_v_peak_set = __pyx_f_7brainpy_2_c_21isotopic_distribution_id_aggregated_isotopic_variants(__pyx_v_dist, __pyx_v_charge, __pyx_v_charge_carrier);
       }
 
-      /* "brainpy/_c/isotopic_distribution.pyx":742
+      /* "brainpy/_c/isotopic_distribution.pyx":754
  *         _npeaks = npeaks - 1
  * 
  *     with nogil:             # <<<<<<<<<<<<<<
  *         dist = make_isotopic_distribution(composition_struct, _npeaks)
  *         peak_set = id_aggregated_isotopic_variants(dist, charge, charge_carrier)
  */
       /*finally:*/ {
@@ -6888,66 +6888,66 @@
           #endif
           goto __pyx_L7;
         }
         __pyx_L7:;
       }
   }
 
-  /* "brainpy/_c/isotopic_distribution.pyx":746
+  /* "brainpy/_c/isotopic_distribution.pyx":758
  *         peak_set = id_aggregated_isotopic_variants(dist, charge, charge_carrier)
  * 
  *     peaklist = peaklist_to_list(peak_set)             # <<<<<<<<<<<<<<
  * 
  *     free_peak_list(peak_set)
  */
-  __pyx_t_1 = __pyx_f_7brainpy_2_c_21isotopic_distribution_peaklist_to_list(__pyx_v_peak_set); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 746, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_7brainpy_2_c_21isotopic_distribution_peaklist_to_list(__pyx_v_peak_set); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 758, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_peaklist = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":748
+  /* "brainpy/_c/isotopic_distribution.pyx":760
  *     peaklist = peaklist_to_list(peak_set)
  * 
  *     free_peak_list(peak_set)             # <<<<<<<<<<<<<<
  *     free_isotopic_distribution(dist)
  *     free_composition(composition_struct)
  */
   __pyx_f_7brainpy_2_c_21isotopic_distribution_free_peak_list(__pyx_v_peak_set);
 
-  /* "brainpy/_c/isotopic_distribution.pyx":749
+  /* "brainpy/_c/isotopic_distribution.pyx":761
  * 
  *     free_peak_list(peak_set)
  *     free_isotopic_distribution(dist)             # <<<<<<<<<<<<<<
  *     free_composition(composition_struct)
  *     return peaklist
  */
   __pyx_f_7brainpy_2_c_21isotopic_distribution_free_isotopic_distribution(__pyx_v_dist);
 
-  /* "brainpy/_c/isotopic_distribution.pyx":750
+  /* "brainpy/_c/isotopic_distribution.pyx":762
  *     free_peak_list(peak_set)
  *     free_isotopic_distribution(dist)
  *     free_composition(composition_struct)             # <<<<<<<<<<<<<<
  *     return peaklist
  * 
  */
   __pyx_f_7brainpy_2_c_11composition_free_composition(__pyx_v_composition_struct);
 
-  /* "brainpy/_c/isotopic_distribution.pyx":751
+  /* "brainpy/_c/isotopic_distribution.pyx":763
  *     free_isotopic_distribution(dist)
  *     free_composition(composition_struct)
  *     return peaklist             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_peaklist);
   __pyx_r = __pyx_v_peaklist;
   goto __pyx_L0;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":700
+  /* "brainpy/_c/isotopic_distribution.pyx":712
  * 
  * 
  * cpdef list _isotopic_variants(object composition, object npeaks=None, int charge=0, double charge_carrier=PROTON):             # <<<<<<<<<<<<<<
  *     '''
  *     Compute a peak list representing the theoretical isotopic cluster for `composition`.
  */
 
@@ -7017,15 +7017,15 @@
         case  3:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_charge_carrier);
           if (value) { values[3] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "_isotopic_variants") < 0)) __PYX_ERR(0, 700, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "_isotopic_variants") < 0)) __PYX_ERR(0, 712, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
         CYTHON_FALLTHROUGH;
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
@@ -7035,27 +7035,27 @@
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_composition = values[0];
     __pyx_v_npeaks = values[1];
     if (values[2]) {
-      __pyx_v_charge = __Pyx_PyInt_As_int(values[2]); if (unlikely((__pyx_v_charge == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 700, __pyx_L3_error)
+      __pyx_v_charge = __Pyx_PyInt_As_int(values[2]); if (unlikely((__pyx_v_charge == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 712, __pyx_L3_error)
     } else {
       __pyx_v_charge = ((int)0);
     }
     if (values[3]) {
-      __pyx_v_charge_carrier = __pyx_PyFloat_AsDouble(values[3]); if (unlikely((__pyx_v_charge_carrier == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 700, __pyx_L3_error)
+      __pyx_v_charge_carrier = __pyx_PyFloat_AsDouble(values[3]); if (unlikely((__pyx_v_charge_carrier == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 712, __pyx_L3_error)
     } else {
       __pyx_v_charge_carrier = __pyx_k__2;
     }
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("_isotopic_variants", 0, 1, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 700, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("_isotopic_variants", 0, 1, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 712, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("brainpy._c.isotopic_distribution._isotopic_variants", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_7brainpy_2_c_21isotopic_distribution_4_isotopic_variants(__pyx_self, __pyx_v_composition, __pyx_v_npeaks, __pyx_v_charge, __pyx_v_charge_carrier);
 
@@ -7074,15 +7074,15 @@
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_isotopic_variants", 0);
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_2.__pyx_n = 3;
   __pyx_t_2.npeaks = __pyx_v_npeaks;
   __pyx_t_2.charge = __pyx_v_charge;
   __pyx_t_2.charge_carrier = __pyx_v_charge_carrier;
-  __pyx_t_1 = __pyx_f_7brainpy_2_c_21isotopic_distribution__isotopic_variants(__pyx_v_composition, 0, &__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 700, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_7brainpy_2_c_21isotopic_distribution__isotopic_variants(__pyx_v_composition, 0, &__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 712, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -7091,15 +7091,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "brainpy/_c/isotopic_distribution.pyx":754
+/* "brainpy/_c/isotopic_distribution.pyx":766
  * 
  * 
  * cdef PeakList* isotopic_variants(Composition* composition, int npeaks, int charge=0, double charge_carrier=PROTON) nogil:             # <<<<<<<<<<<<<<
  *     cdef:
  *         IsotopicDistribution* dist
  */
 
@@ -7115,144 +7115,144 @@
       __pyx_v_charge = __pyx_optional_args->charge;
       if (__pyx_optional_args->__pyx_n > 1) {
         __pyx_v_charge_carrier = __pyx_optional_args->charge_carrier;
       }
     }
   }
 
-  /* "brainpy/_c/isotopic_distribution.pyx":760
+  /* "brainpy/_c/isotopic_distribution.pyx":772
  *         int max_n_variants
  * 
  *     if validate_composition(composition) != 0:             # <<<<<<<<<<<<<<
  *         printf("Malformed composition\n")
  *         return NULL
  */
   __pyx_t_1 = ((__pyx_f_7brainpy_2_c_21isotopic_distribution_validate_composition(__pyx_v_composition) != 0) != 0);
   if (__pyx_t_1) {
 
-    /* "brainpy/_c/isotopic_distribution.pyx":761
+    /* "brainpy/_c/isotopic_distribution.pyx":773
  * 
  *     if validate_composition(composition) != 0:
  *         printf("Malformed composition\n")             # <<<<<<<<<<<<<<
  *         return NULL
  * 
  */
     (void)(printf(((char const *)"Malformed composition\n")));
 
-    /* "brainpy/_c/isotopic_distribution.pyx":762
+    /* "brainpy/_c/isotopic_distribution.pyx":774
  *     if validate_composition(composition) != 0:
  *         printf("Malformed composition\n")
  *         return NULL             # <<<<<<<<<<<<<<
  * 
  *     if npeaks == 0:
  */
     __pyx_r = NULL;
     goto __pyx_L0;
 
-    /* "brainpy/_c/isotopic_distribution.pyx":760
+    /* "brainpy/_c/isotopic_distribution.pyx":772
  *         int max_n_variants
  * 
  *     if validate_composition(composition) != 0:             # <<<<<<<<<<<<<<
  *         printf("Malformed composition\n")
  *         return NULL
  */
   }
 
-  /* "brainpy/_c/isotopic_distribution.pyx":764
+  /* "brainpy/_c/isotopic_distribution.pyx":776
  *         return NULL
  * 
  *     if npeaks == 0:             # <<<<<<<<<<<<<<
  *         npeaks = guess_npeaks(composition, 300)
  *     else:
  */
   __pyx_t_1 = ((__pyx_v_npeaks == 0) != 0);
   if (__pyx_t_1) {
 
-    /* "brainpy/_c/isotopic_distribution.pyx":765
+    /* "brainpy/_c/isotopic_distribution.pyx":777
  * 
  *     if npeaks == 0:
  *         npeaks = guess_npeaks(composition, 300)             # <<<<<<<<<<<<<<
  *     else:
  *         npeaks = npeaks - 1
  */
     __pyx_v_npeaks = __pyx_f_7brainpy_2_c_21isotopic_distribution_guess_npeaks(__pyx_v_composition, 0x12C, NULL);
 
-    /* "brainpy/_c/isotopic_distribution.pyx":764
+    /* "brainpy/_c/isotopic_distribution.pyx":776
  *         return NULL
  * 
  *     if npeaks == 0:             # <<<<<<<<<<<<<<
  *         npeaks = guess_npeaks(composition, 300)
  *     else:
  */
     goto __pyx_L4;
   }
 
-  /* "brainpy/_c/isotopic_distribution.pyx":767
+  /* "brainpy/_c/isotopic_distribution.pyx":779
  *         npeaks = guess_npeaks(composition, 300)
  *     else:
  *         npeaks = npeaks - 1             # <<<<<<<<<<<<<<
  * 
  *     dist = make_isotopic_distribution(composition, npeaks)
  */
   /*else*/ {
     __pyx_v_npeaks = (__pyx_v_npeaks - 1);
   }
   __pyx_L4:;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":769
+  /* "brainpy/_c/isotopic_distribution.pyx":781
  *         npeaks = npeaks - 1
  * 
  *     dist = make_isotopic_distribution(composition, npeaks)             # <<<<<<<<<<<<<<
  *     peaklist = id_aggregated_isotopic_variants(dist, charge, charge_carrier)
  *     free_isotopic_distribution(dist)
  */
   __pyx_v_dist = __pyx_f_7brainpy_2_c_21isotopic_distribution_make_isotopic_distribution(__pyx_v_composition, __pyx_v_npeaks, NULL);
 
-  /* "brainpy/_c/isotopic_distribution.pyx":770
+  /* "brainpy/_c/isotopic_distribution.pyx":782
  * 
  *     dist = make_isotopic_distribution(composition, npeaks)
  *     peaklist = id_aggregated_isotopic_variants(dist, charge, charge_carrier)             # <<<<<<<<<<<<<<
  *     free_isotopic_distribution(dist)
  * 
  */
   __pyx_v_peaklist = __pyx_f_7brainpy_2_c_21isotopic_distribution_id_aggregated_isotopic_variants(__pyx_v_dist, __pyx_v_charge, __pyx_v_charge_carrier);
 
-  /* "brainpy/_c/isotopic_distribution.pyx":771
+  /* "brainpy/_c/isotopic_distribution.pyx":783
  *     dist = make_isotopic_distribution(composition, npeaks)
  *     peaklist = id_aggregated_isotopic_variants(dist, charge, charge_carrier)
  *     free_isotopic_distribution(dist)             # <<<<<<<<<<<<<<
  * 
  *     return peaklist
  */
   __pyx_f_7brainpy_2_c_21isotopic_distribution_free_isotopic_distribution(__pyx_v_dist);
 
-  /* "brainpy/_c/isotopic_distribution.pyx":773
+  /* "brainpy/_c/isotopic_distribution.pyx":785
  *     free_isotopic_distribution(dist)
  * 
  *     return peaklist             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = __pyx_v_peaklist;
   goto __pyx_L0;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":754
+  /* "brainpy/_c/isotopic_distribution.pyx":766
  * 
  * 
  * cdef PeakList* isotopic_variants(Composition* composition, int npeaks, int charge=0, double charge_carrier=PROTON) nogil:             # <<<<<<<<<<<<<<
  *     cdef:
  *         IsotopicDistribution* dist
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "brainpy/_c/isotopic_distribution.pyx":776
+/* "brainpy/_c/isotopic_distribution.pyx":788
  * 
  * 
  * cdef list peaklist_to_list(PeakList* peaklist):             # <<<<<<<<<<<<<<
  *     cdef:
  *         list pypeaklist
  */
 
@@ -7267,64 +7267,64 @@
   size_t __pyx_t_4;
   int __pyx_t_5;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("peaklist_to_list", 0);
 
-  /* "brainpy/_c/isotopic_distribution.pyx":780
+  /* "brainpy/_c/isotopic_distribution.pyx":792
  *         list pypeaklist
  *         size_t i
  *     pypeaklist = []             # <<<<<<<<<<<<<<
  *     for i in range(peaklist.used):
  *         pypeaklist.append(TheoreticalPeak._create(
  */
-  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 780, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 792, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_pypeaklist = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":781
+  /* "brainpy/_c/isotopic_distribution.pyx":793
  *         size_t i
  *     pypeaklist = []
  *     for i in range(peaklist.used):             # <<<<<<<<<<<<<<
  *         pypeaklist.append(TheoreticalPeak._create(
  *             peaklist.peaks[i].mz, peaklist.peaks[i].intensity, peaklist.peaks[i].charge))
  */
   __pyx_t_2 = __pyx_v_peaklist->used;
   __pyx_t_3 = __pyx_t_2;
   for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
     __pyx_v_i = __pyx_t_4;
 
-    /* "brainpy/_c/isotopic_distribution.pyx":782
+    /* "brainpy/_c/isotopic_distribution.pyx":794
  *     pypeaklist = []
  *     for i in range(peaklist.used):
  *         pypeaklist.append(TheoreticalPeak._create(             # <<<<<<<<<<<<<<
  *             peaklist.peaks[i].mz, peaklist.peaks[i].intensity, peaklist.peaks[i].charge))
  *     return pypeaklist
  */
-    __pyx_t_1 = ((PyObject *)__pyx_f_7brainpy_2_c_21isotopic_distribution_15TheoreticalPeak__create((__pyx_v_peaklist->peaks[__pyx_v_i]).mz, (__pyx_v_peaklist->peaks[__pyx_v_i]).intensity, (__pyx_v_peaklist->peaks[__pyx_v_i]).charge)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 782, __pyx_L1_error)
+    __pyx_t_1 = ((PyObject *)__pyx_f_7brainpy_2_c_21isotopic_distribution_15TheoreticalPeak__create((__pyx_v_peaklist->peaks[__pyx_v_i]).mz, (__pyx_v_peaklist->peaks[__pyx_v_i]).intensity, (__pyx_v_peaklist->peaks[__pyx_v_i]).charge)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 794, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_5 = __Pyx_PyList_Append(__pyx_v_pypeaklist, __pyx_t_1); if (unlikely(__pyx_t_5 == ((int)-1))) __PYX_ERR(0, 782, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyList_Append(__pyx_v_pypeaklist, __pyx_t_1); if (unlikely(__pyx_t_5 == ((int)-1))) __PYX_ERR(0, 794, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   }
 
-  /* "brainpy/_c/isotopic_distribution.pyx":784
+  /* "brainpy/_c/isotopic_distribution.pyx":796
  *         pypeaklist.append(TheoreticalPeak._create(
  *             peaklist.peaks[i].mz, peaklist.peaks[i].intensity, peaklist.peaks[i].charge))
  *     return pypeaklist             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_pypeaklist);
   __pyx_r = __pyx_v_pypeaklist;
   goto __pyx_L0;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":776
+  /* "brainpy/_c/isotopic_distribution.pyx":788
  * 
  * 
  * cdef list peaklist_to_list(PeakList* peaklist):             # <<<<<<<<<<<<<<
  *     cdef:
  *         list pypeaklist
  */
 
@@ -7336,15 +7336,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_pypeaklist);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "brainpy/_c/isotopic_distribution.pyx":789
+/* "brainpy/_c/isotopic_distribution.pyx":801
  * @cython.freelist(1000000)
  * cdef class TheoreticalPeak(object):
  *     def __init__(self, mz, intensity, charge):             # <<<<<<<<<<<<<<
  *         self.mz = mz
  *         self.intensity = intensity
  */
 
@@ -7381,40 +7381,40 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_mz)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_intensity)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__init__", 1, 3, 3, 1); __PYX_ERR(0, 789, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__init__", 1, 3, 3, 1); __PYX_ERR(0, 801, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_charge)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__init__", 1, 3, 3, 2); __PYX_ERR(0, 789, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__init__", 1, 3, 3, 2); __PYX_ERR(0, 801, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 789, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 801, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 3) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
     }
     __pyx_v_mz = values[0];
     __pyx_v_intensity = values[1];
     __pyx_v_charge = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__init__", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 789, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__init__", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 801, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("brainpy._c.isotopic_distribution.TheoreticalPeak.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_7brainpy_2_c_21isotopic_distribution_15TheoreticalPeak___init__(((struct __pyx_obj_7brainpy_2_c_21isotopic_distribution_TheoreticalPeak *)__pyx_v_self), __pyx_v_mz, __pyx_v_intensity, __pyx_v_charge);
 
@@ -7429,45 +7429,45 @@
   double __pyx_t_1;
   int __pyx_t_2;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 0);
 
-  /* "brainpy/_c/isotopic_distribution.pyx":790
+  /* "brainpy/_c/isotopic_distribution.pyx":802
  * cdef class TheoreticalPeak(object):
  *     def __init__(self, mz, intensity, charge):
  *         self.mz = mz             # <<<<<<<<<<<<<<
  *         self.intensity = intensity
  *         self.charge = charge
  */
-  __pyx_t_1 = __pyx_PyFloat_AsDouble(__pyx_v_mz); if (unlikely((__pyx_t_1 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 790, __pyx_L1_error)
+  __pyx_t_1 = __pyx_PyFloat_AsDouble(__pyx_v_mz); if (unlikely((__pyx_t_1 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 802, __pyx_L1_error)
   __pyx_v_self->mz = __pyx_t_1;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":791
+  /* "brainpy/_c/isotopic_distribution.pyx":803
  *     def __init__(self, mz, intensity, charge):
  *         self.mz = mz
  *         self.intensity = intensity             # <<<<<<<<<<<<<<
  *         self.charge = charge
  * 
  */
-  __pyx_t_1 = __pyx_PyFloat_AsDouble(__pyx_v_intensity); if (unlikely((__pyx_t_1 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 791, __pyx_L1_error)
+  __pyx_t_1 = __pyx_PyFloat_AsDouble(__pyx_v_intensity); if (unlikely((__pyx_t_1 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 803, __pyx_L1_error)
   __pyx_v_self->intensity = __pyx_t_1;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":792
+  /* "brainpy/_c/isotopic_distribution.pyx":804
  *         self.mz = mz
  *         self.intensity = intensity
  *         self.charge = charge             # <<<<<<<<<<<<<<
  * 
  *     def __repr__(self):
  */
-  __pyx_t_2 = __Pyx_PyInt_As_int(__pyx_v_charge); if (unlikely((__pyx_t_2 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 792, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_As_int(__pyx_v_charge); if (unlikely((__pyx_t_2 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 804, __pyx_L1_error)
   __pyx_v_self->charge = __pyx_t_2;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":789
+  /* "brainpy/_c/isotopic_distribution.pyx":801
  * @cython.freelist(1000000)
  * cdef class TheoreticalPeak(object):
  *     def __init__(self, mz, intensity, charge):             # <<<<<<<<<<<<<<
  *         self.mz = mz
  *         self.intensity = intensity
  */
 
@@ -7478,15 +7478,15 @@
   __Pyx_AddTraceback("brainpy._c.isotopic_distribution.TheoreticalPeak.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "brainpy/_c/isotopic_distribution.pyx":794
+/* "brainpy/_c/isotopic_distribution.pyx":806
  *         self.charge = charge
  * 
  *     def __repr__(self):             # <<<<<<<<<<<<<<
  *         return "Peak(mz=%f, intensity=%f, charge=%d)" % (self.mz, self.intensity, self.charge)
  * 
  */
 
@@ -7511,47 +7511,47 @@
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__repr__", 0);
 
-  /* "brainpy/_c/isotopic_distribution.pyx":795
+  /* "brainpy/_c/isotopic_distribution.pyx":807
  * 
  *     def __repr__(self):
  *         return "Peak(mz=%f, intensity=%f, charge=%d)" % (self.mz, self.intensity, self.charge)             # <<<<<<<<<<<<<<
  * 
  *     cpdef bint _eq(self, TheoreticalPeak other):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyFloat_FromDouble(__pyx_v_self->mz); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 795, __pyx_L1_error)
+  __pyx_t_1 = PyFloat_FromDouble(__pyx_v_self->mz); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 807, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyFloat_FromDouble(__pyx_v_self->intensity); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 795, __pyx_L1_error)
+  __pyx_t_2 = PyFloat_FromDouble(__pyx_v_self->intensity); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 807, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_self->charge); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 795, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_self->charge); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 807, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = PyTuple_New(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 795, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 807, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_4, 2, __pyx_t_3);
   __pyx_t_1 = 0;
   __pyx_t_2 = 0;
   __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyString_Format(__pyx_kp_s_Peak_mz_f_intensity_f_charge_d, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 795, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyString_Format(__pyx_kp_s_Peak_mz_f_intensity_f_charge_d, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 807, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_r = __pyx_t_3;
   __pyx_t_3 = 0;
   goto __pyx_L0;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":794
+  /* "brainpy/_c/isotopic_distribution.pyx":806
  *         self.charge = charge
  * 
  *     def __repr__(self):             # <<<<<<<<<<<<<<
  *         return "Peak(mz=%f, intensity=%f, charge=%d)" % (self.mz, self.intensity, self.charge)
  * 
  */
 
@@ -7565,15 +7565,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "brainpy/_c/isotopic_distribution.pyx":797
+/* "brainpy/_c/isotopic_distribution.pyx":809
  *         return "Peak(mz=%f, intensity=%f, charge=%d)" % (self.mz, self.intensity, self.charge)
  * 
  *     cpdef bint _eq(self, TheoreticalPeak other):             # <<<<<<<<<<<<<<
  *         cdef bint val
  *         val = (abs(self.mz - other.mz) < 1e-10 and\
  */
 
@@ -7597,15 +7597,15 @@
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_type_dict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_eq); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 797, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_eq); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 809, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_7brainpy_2_c_21isotopic_distribution_15TheoreticalPeak_5_eq)) {
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_3 = __pyx_t_1; __pyx_t_4 = NULL;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
           __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
           if (likely(__pyx_t_4)) {
@@ -7613,18 +7613,18 @@
             __Pyx_INCREF(__pyx_t_4);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_3, function);
           }
         }
         __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, ((PyObject *)__pyx_v_other)) : __Pyx_PyObject_CallOneArg(__pyx_t_3, ((PyObject *)__pyx_v_other));
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 797, __pyx_L1_error)
+        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 809, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-        __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely((__pyx_t_5 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 797, __pyx_L1_error)
+        __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely((__pyx_t_5 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 809, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __pyx_r = __pyx_t_5;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
       __pyx_tp_dict_version = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
@@ -7635,65 +7635,65 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "brainpy/_c/isotopic_distribution.pyx":799
+  /* "brainpy/_c/isotopic_distribution.pyx":811
  *     cpdef bint _eq(self, TheoreticalPeak other):
  *         cdef bint val
  *         val = (abs(self.mz - other.mz) < 1e-10 and\             # <<<<<<<<<<<<<<
  *                abs(self.intensity - other.intensity) < 1e-10 and\
  *                self.charge == other.charge)
  */
   __pyx_t_6 = ((fabs((__pyx_v_self->mz - __pyx_v_other->mz)) < 1e-10) != 0);
   if (__pyx_t_6) {
   } else {
     __pyx_t_5 = __pyx_t_6;
     goto __pyx_L3_bool_binop_done;
   }
 
-  /* "brainpy/_c/isotopic_distribution.pyx":800
+  /* "brainpy/_c/isotopic_distribution.pyx":812
  *         cdef bint val
  *         val = (abs(self.mz - other.mz) < 1e-10 and\
  *                abs(self.intensity - other.intensity) < 1e-10 and\             # <<<<<<<<<<<<<<
  *                self.charge == other.charge)
  *         return val
  */
   __pyx_t_6 = ((fabs((__pyx_v_self->intensity - __pyx_v_other->intensity)) < 1e-10) != 0);
   if (__pyx_t_6) {
   } else {
     __pyx_t_5 = __pyx_t_6;
     goto __pyx_L3_bool_binop_done;
   }
 
-  /* "brainpy/_c/isotopic_distribution.pyx":801
+  /* "brainpy/_c/isotopic_distribution.pyx":813
  *         val = (abs(self.mz - other.mz) < 1e-10 and\
  *                abs(self.intensity - other.intensity) < 1e-10 and\
  *                self.charge == other.charge)             # <<<<<<<<<<<<<<
  *         return val
  * 
  */
   __pyx_t_6 = ((__pyx_v_self->charge == __pyx_v_other->charge) != 0);
   __pyx_t_5 = __pyx_t_6;
   __pyx_L3_bool_binop_done:;
   __pyx_v_val = __pyx_t_5;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":802
+  /* "brainpy/_c/isotopic_distribution.pyx":814
  *                abs(self.intensity - other.intensity) < 1e-10 and\
  *                self.charge == other.charge)
  *         return val             # <<<<<<<<<<<<<<
  * 
  *     def __hash__(self):
  */
   __pyx_r = __pyx_v_val;
   goto __pyx_L0;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":797
+  /* "brainpy/_c/isotopic_distribution.pyx":809
  *         return "Peak(mz=%f, intensity=%f, charge=%d)" % (self.mz, self.intensity, self.charge)
  * 
  *     cpdef bint _eq(self, TheoreticalPeak other):             # <<<<<<<<<<<<<<
  *         cdef bint val
  *         val = (abs(self.mz - other.mz) < 1e-10 and\
  */
 
@@ -7716,15 +7716,15 @@
 static PyObject *__pyx_pw_7brainpy_2_c_21isotopic_distribution_15TheoreticalPeak_5_eq(PyObject *__pyx_v_self, PyObject *__pyx_v_other) {
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("_eq (wrapper)", 0);
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_other), __pyx_ptype_7brainpy_2_c_21isotopic_distribution_TheoreticalPeak, 1, "other", 0))) __PYX_ERR(0, 797, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_other), __pyx_ptype_7brainpy_2_c_21isotopic_distribution_TheoreticalPeak, 1, "other", 0))) __PYX_ERR(0, 809, __pyx_L1_error)
   __pyx_r = __pyx_pf_7brainpy_2_c_21isotopic_distribution_15TheoreticalPeak_4_eq(((struct __pyx_obj_7brainpy_2_c_21isotopic_distribution_TheoreticalPeak *)__pyx_v_self), ((struct __pyx_obj_7brainpy_2_c_21isotopic_distribution_TheoreticalPeak *)__pyx_v_other));
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -7737,15 +7737,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_eq", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyBool_FromLong(__pyx_f_7brainpy_2_c_21isotopic_distribution_15TheoreticalPeak__eq(__pyx_v_self, __pyx_v_other, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 797, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyBool_FromLong(__pyx_f_7brainpy_2_c_21isotopic_distribution_15TheoreticalPeak__eq(__pyx_v_self, __pyx_v_other, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 809, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -7754,15 +7754,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "brainpy/_c/isotopic_distribution.pyx":804
+/* "brainpy/_c/isotopic_distribution.pyx":816
  *         return val
  * 
  *     def __hash__(self):             # <<<<<<<<<<<<<<
  *         return hash((self.mz, self.intensity, self.charge))
  * 
  */
 
@@ -7788,44 +7788,44 @@
   PyObject *__pyx_t_4 = NULL;
   Py_hash_t __pyx_t_5;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__hash__", 0);
 
-  /* "brainpy/_c/isotopic_distribution.pyx":805
+  /* "brainpy/_c/isotopic_distribution.pyx":817
  * 
  *     def __hash__(self):
  *         return hash((self.mz, self.intensity, self.charge))             # <<<<<<<<<<<<<<
  * 
  *     def __richcmp__(self, other, int code):
  */
-  __pyx_t_1 = PyFloat_FromDouble(__pyx_v_self->mz); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 805, __pyx_L1_error)
+  __pyx_t_1 = PyFloat_FromDouble(__pyx_v_self->mz); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 817, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyFloat_FromDouble(__pyx_v_self->intensity); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 805, __pyx_L1_error)
+  __pyx_t_2 = PyFloat_FromDouble(__pyx_v_self->intensity); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 817, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_self->charge); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 805, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_self->charge); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 817, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = PyTuple_New(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 805, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 817, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_4, 2, __pyx_t_3);
   __pyx_t_1 = 0;
   __pyx_t_2 = 0;
   __pyx_t_3 = 0;
-  __pyx_t_5 = PyObject_Hash(__pyx_t_4); if (unlikely(__pyx_t_5 == ((Py_hash_t)-1))) __PYX_ERR(0, 805, __pyx_L1_error)
+  __pyx_t_5 = PyObject_Hash(__pyx_t_4); if (unlikely(__pyx_t_5 == ((Py_hash_t)-1))) __PYX_ERR(0, 817, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_r = __pyx_t_5;
   goto __pyx_L0;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":804
+  /* "brainpy/_c/isotopic_distribution.pyx":816
  *         return val
  * 
  *     def __hash__(self):             # <<<<<<<<<<<<<<
  *         return hash((self.mz, self.intensity, self.charge))
  * 
  */
 
@@ -7839,15 +7839,15 @@
   __pyx_r = -1;
   __pyx_L0:;
   if (unlikely(__pyx_r == -1) && !PyErr_Occurred()) __pyx_r = -2;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "brainpy/_c/isotopic_distribution.pyx":807
+/* "brainpy/_c/isotopic_distribution.pyx":819
  *         return hash((self.mz, self.intensity, self.charge))
  * 
  *     def __richcmp__(self, other, int code):             # <<<<<<<<<<<<<<
  *         if code == 2:
  *             return self._eq(other)
  */
 
@@ -7869,76 +7869,76 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__richcmp__", 0);
 
-  /* "brainpy/_c/isotopic_distribution.pyx":808
+  /* "brainpy/_c/isotopic_distribution.pyx":820
  * 
  *     def __richcmp__(self, other, int code):
  *         if code == 2:             # <<<<<<<<<<<<<<
  *             return self._eq(other)
  *         elif code == 3:
  */
   switch (__pyx_v_code) {
     case 2:
 
-    /* "brainpy/_c/isotopic_distribution.pyx":809
+    /* "brainpy/_c/isotopic_distribution.pyx":821
  *     def __richcmp__(self, other, int code):
  *         if code == 2:
  *             return self._eq(other)             # <<<<<<<<<<<<<<
  *         elif code == 3:
  *             return not self._eq(other)
  */
     __Pyx_XDECREF(__pyx_r);
-    if (!(likely(((__pyx_v_other) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_other, __pyx_ptype_7brainpy_2_c_21isotopic_distribution_TheoreticalPeak))))) __PYX_ERR(0, 809, __pyx_L1_error)
-    __pyx_t_1 = __Pyx_PyBool_FromLong(((struct __pyx_vtabstruct_7brainpy_2_c_21isotopic_distribution_TheoreticalPeak *)__pyx_v_self->__pyx_vtab)->_eq(__pyx_v_self, ((struct __pyx_obj_7brainpy_2_c_21isotopic_distribution_TheoreticalPeak *)__pyx_v_other), 0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 809, __pyx_L1_error)
+    if (!(likely(((__pyx_v_other) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_other, __pyx_ptype_7brainpy_2_c_21isotopic_distribution_TheoreticalPeak))))) __PYX_ERR(0, 821, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyBool_FromLong(((struct __pyx_vtabstruct_7brainpy_2_c_21isotopic_distribution_TheoreticalPeak *)__pyx_v_self->__pyx_vtab)->_eq(__pyx_v_self, ((struct __pyx_obj_7brainpy_2_c_21isotopic_distribution_TheoreticalPeak *)__pyx_v_other), 0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 821, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_r = __pyx_t_1;
     __pyx_t_1 = 0;
     goto __pyx_L0;
 
-    /* "brainpy/_c/isotopic_distribution.pyx":808
+    /* "brainpy/_c/isotopic_distribution.pyx":820
  * 
  *     def __richcmp__(self, other, int code):
  *         if code == 2:             # <<<<<<<<<<<<<<
  *             return self._eq(other)
  *         elif code == 3:
  */
     break;
     case 3:
 
-    /* "brainpy/_c/isotopic_distribution.pyx":811
+    /* "brainpy/_c/isotopic_distribution.pyx":823
  *             return self._eq(other)
  *         elif code == 3:
  *             return not self._eq(other)             # <<<<<<<<<<<<<<
  * 
  *     def __reduce__(self):
  */
     __Pyx_XDECREF(__pyx_r);
-    if (!(likely(((__pyx_v_other) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_other, __pyx_ptype_7brainpy_2_c_21isotopic_distribution_TheoreticalPeak))))) __PYX_ERR(0, 811, __pyx_L1_error)
-    __pyx_t_1 = __Pyx_PyBool_FromLong((!(((struct __pyx_vtabstruct_7brainpy_2_c_21isotopic_distribution_TheoreticalPeak *)__pyx_v_self->__pyx_vtab)->_eq(__pyx_v_self, ((struct __pyx_obj_7brainpy_2_c_21isotopic_distribution_TheoreticalPeak *)__pyx_v_other), 0) != 0))); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 811, __pyx_L1_error)
+    if (!(likely(((__pyx_v_other) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_other, __pyx_ptype_7brainpy_2_c_21isotopic_distribution_TheoreticalPeak))))) __PYX_ERR(0, 823, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyBool_FromLong((!(((struct __pyx_vtabstruct_7brainpy_2_c_21isotopic_distribution_TheoreticalPeak *)__pyx_v_self->__pyx_vtab)->_eq(__pyx_v_self, ((struct __pyx_obj_7brainpy_2_c_21isotopic_distribution_TheoreticalPeak *)__pyx_v_other), 0) != 0))); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 823, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_r = __pyx_t_1;
     __pyx_t_1 = 0;
     goto __pyx_L0;
 
-    /* "brainpy/_c/isotopic_distribution.pyx":810
+    /* "brainpy/_c/isotopic_distribution.pyx":822
  *         if code == 2:
  *             return self._eq(other)
  *         elif code == 3:             # <<<<<<<<<<<<<<
  *             return not self._eq(other)
  * 
  */
     break;
     default: break;
   }
 
-  /* "brainpy/_c/isotopic_distribution.pyx":807
+  /* "brainpy/_c/isotopic_distribution.pyx":819
  *         return hash((self.mz, self.intensity, self.charge))
  * 
  *     def __richcmp__(self, other, int code):             # <<<<<<<<<<<<<<
  *         if code == 2:
  *             return self._eq(other)
  */
 
@@ -7951,15 +7951,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "brainpy/_c/isotopic_distribution.pyx":813
+/* "brainpy/_c/isotopic_distribution.pyx":825
  *             return not self._eq(other)
  * 
  *     def __reduce__(self):             # <<<<<<<<<<<<<<
  *         return TheoreticalPeak, (self.mz, self.intensity, self.charge)
  * 
  */
 
@@ -7985,52 +7985,52 @@
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__reduce__", 0);
 
-  /* "brainpy/_c/isotopic_distribution.pyx":814
+  /* "brainpy/_c/isotopic_distribution.pyx":826
  * 
  *     def __reduce__(self):
  *         return TheoreticalPeak, (self.mz, self.intensity, self.charge)             # <<<<<<<<<<<<<<
  * 
  *     cpdef TheoreticalPeak clone(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyFloat_FromDouble(__pyx_v_self->mz); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 814, __pyx_L1_error)
+  __pyx_t_1 = PyFloat_FromDouble(__pyx_v_self->mz); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 826, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyFloat_FromDouble(__pyx_v_self->intensity); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 814, __pyx_L1_error)
+  __pyx_t_2 = PyFloat_FromDouble(__pyx_v_self->intensity); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 826, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_self->charge); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 814, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_self->charge); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 826, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = PyTuple_New(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 814, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 826, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_4, 2, __pyx_t_3);
   __pyx_t_1 = 0;
   __pyx_t_2 = 0;
   __pyx_t_3 = 0;
-  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 814, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 826, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_INCREF(((PyObject *)__pyx_ptype_7brainpy_2_c_21isotopic_distribution_TheoreticalPeak));
   __Pyx_GIVEREF(((PyObject *)__pyx_ptype_7brainpy_2_c_21isotopic_distribution_TheoreticalPeak));
   PyTuple_SET_ITEM(__pyx_t_3, 0, ((PyObject *)__pyx_ptype_7brainpy_2_c_21isotopic_distribution_TheoreticalPeak));
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_4);
   __pyx_t_4 = 0;
   __pyx_r = __pyx_t_3;
   __pyx_t_3 = 0;
   goto __pyx_L0;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":813
+  /* "brainpy/_c/isotopic_distribution.pyx":825
  *             return not self._eq(other)
  * 
  *     def __reduce__(self):             # <<<<<<<<<<<<<<
  *         return TheoreticalPeak, (self.mz, self.intensity, self.charge)
  * 
  */
 
@@ -8044,15 +8044,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "brainpy/_c/isotopic_distribution.pyx":816
+/* "brainpy/_c/isotopic_distribution.pyx":828
  *         return TheoreticalPeak, (self.mz, self.intensity, self.charge)
  * 
  *     cpdef TheoreticalPeak clone(self):             # <<<<<<<<<<<<<<
  *         return TheoreticalPeak._create(self.mz, self.intensity, self.charge)
  * 
  */
 
@@ -8073,15 +8073,15 @@
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_type_dict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_clone); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 816, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_clone); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 828, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_7brainpy_2_c_21isotopic_distribution_15TheoreticalPeak_13clone)) {
         __Pyx_XDECREF(((PyObject *)__pyx_r));
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_3 = __pyx_t_1; __pyx_t_4 = NULL;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
           __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
@@ -8090,18 +8090,18 @@
             __Pyx_INCREF(__pyx_t_4);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_3, function);
           }
         }
         __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 816, __pyx_L1_error)
+        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 828, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-        if (!(likely(((__pyx_t_2) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_2, __pyx_ptype_7brainpy_2_c_21isotopic_distribution_TheoreticalPeak))))) __PYX_ERR(0, 816, __pyx_L1_error)
+        if (!(likely(((__pyx_t_2) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_2, __pyx_ptype_7brainpy_2_c_21isotopic_distribution_TheoreticalPeak))))) __PYX_ERR(0, 828, __pyx_L1_error)
         __pyx_r = ((struct __pyx_obj_7brainpy_2_c_21isotopic_distribution_TheoreticalPeak *)__pyx_t_2);
         __pyx_t_2 = 0;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
       __pyx_tp_dict_version = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
@@ -8112,29 +8112,29 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "brainpy/_c/isotopic_distribution.pyx":817
+  /* "brainpy/_c/isotopic_distribution.pyx":829
  * 
  *     cpdef TheoreticalPeak clone(self):
  *         return TheoreticalPeak._create(self.mz, self.intensity, self.charge)             # <<<<<<<<<<<<<<
  * 
  *     @staticmethod
  */
   __Pyx_XDECREF(((PyObject *)__pyx_r));
-  __pyx_t_1 = ((PyObject *)__pyx_f_7brainpy_2_c_21isotopic_distribution_15TheoreticalPeak__create(__pyx_v_self->mz, __pyx_v_self->intensity, __pyx_v_self->charge)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 817, __pyx_L1_error)
+  __pyx_t_1 = ((PyObject *)__pyx_f_7brainpy_2_c_21isotopic_distribution_15TheoreticalPeak__create(__pyx_v_self->mz, __pyx_v_self->intensity, __pyx_v_self->charge)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 829, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = ((struct __pyx_obj_7brainpy_2_c_21isotopic_distribution_TheoreticalPeak *)__pyx_t_1);
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":816
+  /* "brainpy/_c/isotopic_distribution.pyx":828
  *         return TheoreticalPeak, (self.mz, self.intensity, self.charge)
  * 
  *     cpdef TheoreticalPeak clone(self):             # <<<<<<<<<<<<<<
  *         return TheoreticalPeak._create(self.mz, self.intensity, self.charge)
  * 
  */
 
@@ -8171,15 +8171,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("clone", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = ((PyObject *)__pyx_f_7brainpy_2_c_21isotopic_distribution_15TheoreticalPeak_clone(__pyx_v_self, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 816, __pyx_L1_error)
+  __pyx_t_1 = ((PyObject *)__pyx_f_7brainpy_2_c_21isotopic_distribution_15TheoreticalPeak_clone(__pyx_v_self, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 828, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -8188,15 +8188,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "brainpy/_c/isotopic_distribution.pyx":820
+/* "brainpy/_c/isotopic_distribution.pyx":832
  * 
  *     @staticmethod
  *     cdef TheoreticalPeak _create(double mz, double intensity, int charge):             # <<<<<<<<<<<<<<
  *         cdef:
  *             TheoreticalPeak inst
  */
 
@@ -8206,66 +8206,66 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_create", 0);
 
-  /* "brainpy/_c/isotopic_distribution.pyx":823
+  /* "brainpy/_c/isotopic_distribution.pyx":835
  *         cdef:
  *             TheoreticalPeak inst
  *         inst = TheoreticalPeak.__new__(TheoreticalPeak)             # <<<<<<<<<<<<<<
  *         inst.mz = mz
  *         inst.intensity = intensity
  */
-  __pyx_t_1 = ((PyObject *)__pyx_tp_new_7brainpy_2_c_21isotopic_distribution_TheoreticalPeak(((PyTypeObject *)__pyx_ptype_7brainpy_2_c_21isotopic_distribution_TheoreticalPeak), __pyx_empty_tuple, NULL)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 823, __pyx_L1_error)
+  __pyx_t_1 = ((PyObject *)__pyx_tp_new_7brainpy_2_c_21isotopic_distribution_TheoreticalPeak(((PyTypeObject *)__pyx_ptype_7brainpy_2_c_21isotopic_distribution_TheoreticalPeak), __pyx_empty_tuple, NULL)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 835, __pyx_L1_error)
   __Pyx_GOTREF(((PyObject *)__pyx_t_1));
   __pyx_v_inst = ((struct __pyx_obj_7brainpy_2_c_21isotopic_distribution_TheoreticalPeak *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":824
+  /* "brainpy/_c/isotopic_distribution.pyx":836
  *             TheoreticalPeak inst
  *         inst = TheoreticalPeak.__new__(TheoreticalPeak)
  *         inst.mz = mz             # <<<<<<<<<<<<<<
  *         inst.intensity = intensity
  *         inst.charge = charge
  */
   __pyx_v_inst->mz = __pyx_v_mz;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":825
+  /* "brainpy/_c/isotopic_distribution.pyx":837
  *         inst = TheoreticalPeak.__new__(TheoreticalPeak)
  *         inst.mz = mz
  *         inst.intensity = intensity             # <<<<<<<<<<<<<<
  *         inst.charge = charge
  *         return inst
  */
   __pyx_v_inst->intensity = __pyx_v_intensity;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":826
+  /* "brainpy/_c/isotopic_distribution.pyx":838
  *         inst.mz = mz
  *         inst.intensity = intensity
  *         inst.charge = charge             # <<<<<<<<<<<<<<
  *         return inst
  * 
  */
   __pyx_v_inst->charge = __pyx_v_charge;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":827
+  /* "brainpy/_c/isotopic_distribution.pyx":839
  *         inst.intensity = intensity
  *         inst.charge = charge
  *         return inst             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(((PyObject *)__pyx_r));
   __Pyx_INCREF(((PyObject *)__pyx_v_inst));
   __pyx_r = __pyx_v_inst;
   goto __pyx_L0;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":820
+  /* "brainpy/_c/isotopic_distribution.pyx":832
  * 
  *     @staticmethod
  *     cdef TheoreticalPeak _create(double mz, double intensity, int charge):             # <<<<<<<<<<<<<<
  *         cdef:
  *             TheoreticalPeak inst
  */
 
@@ -8523,15 +8523,15 @@
   __Pyx_AddTraceback("brainpy._c.isotopic_distribution.TheoreticalPeak.charge.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "brainpy/_c/isotopic_distribution.pyx":830
+/* "brainpy/_c/isotopic_distribution.pyx":842
  * 
  * 
  * def main():             # <<<<<<<<<<<<<<
  *     cdef:
  *         dict comp_dict
  */
 
@@ -8559,191 +8559,191 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("main", 0);
 
-  /* "brainpy/_c/isotopic_distribution.pyx":837
+  /* "brainpy/_c/isotopic_distribution.pyx":849
  *         IsotopicDistribution* distribution2
  * 
  *     comp_dict = dict(H=2, O=1)             # <<<<<<<<<<<<<<
  *     print comp_dict
  *     composition = dict_to_composition(comp_dict)
  */
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 837, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 849, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_H, __pyx_int_2) < 0) __PYX_ERR(0, 837, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_O, __pyx_int_1) < 0) __PYX_ERR(0, 837, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_H, __pyx_int_2) < 0) __PYX_ERR(0, 849, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_O, __pyx_int_1) < 0) __PYX_ERR(0, 849, __pyx_L1_error)
   __pyx_v_comp_dict = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":838
+  /* "brainpy/_c/isotopic_distribution.pyx":850
  * 
  *     comp_dict = dict(H=2, O=1)
  *     print comp_dict             # <<<<<<<<<<<<<<
  *     composition = dict_to_composition(comp_dict)
  *     print_composition(composition)
  */
-  if (__Pyx_PrintOne(0, __pyx_v_comp_dict) < 0) __PYX_ERR(0, 838, __pyx_L1_error)
+  if (__Pyx_PrintOne(0, __pyx_v_comp_dict) < 0) __PYX_ERR(0, 850, __pyx_L1_error)
 
-  /* "brainpy/_c/isotopic_distribution.pyx":839
+  /* "brainpy/_c/isotopic_distribution.pyx":851
  *     comp_dict = dict(H=2, O=1)
  *     print comp_dict
  *     composition = dict_to_composition(comp_dict)             # <<<<<<<<<<<<<<
  *     print_composition(composition)
  *     distribution = make_isotopic_distribution(composition, 4)
  */
   __pyx_v_composition = __pyx_f_7brainpy_2_c_11composition_dict_to_composition(__pyx_v_comp_dict);
 
-  /* "brainpy/_c/isotopic_distribution.pyx":840
+  /* "brainpy/_c/isotopic_distribution.pyx":852
  *     print comp_dict
  *     composition = dict_to_composition(comp_dict)
  *     print_composition(composition)             # <<<<<<<<<<<<<<
  *     distribution = make_isotopic_distribution(composition, 4)
  *     print "Going to print constants"
  */
   __pyx_f_7brainpy_2_c_11composition_print_composition(__pyx_v_composition);
 
-  /* "brainpy/_c/isotopic_distribution.pyx":841
+  /* "brainpy/_c/isotopic_distribution.pyx":853
  *     composition = dict_to_composition(comp_dict)
  *     print_composition(composition)
  *     distribution = make_isotopic_distribution(composition, 4)             # <<<<<<<<<<<<<<
  *     print "Going to print constants"
  *     print_isotopic_constants(distribution._isotopic_constants)
  */
   __pyx_v_distribution = __pyx_f_7brainpy_2_c_21isotopic_distribution_make_isotopic_distribution(__pyx_v_composition, 4, NULL);
 
-  /* "brainpy/_c/isotopic_distribution.pyx":842
+  /* "brainpy/_c/isotopic_distribution.pyx":854
  *     print_composition(composition)
  *     distribution = make_isotopic_distribution(composition, 4)
  *     print "Going to print constants"             # <<<<<<<<<<<<<<
  *     print_isotopic_constants(distribution._isotopic_constants)
  *     print "Done"
  */
-  if (__Pyx_PrintOne(0, __pyx_kp_s_Going_to_print_constants) < 0) __PYX_ERR(0, 842, __pyx_L1_error)
+  if (__Pyx_PrintOne(0, __pyx_kp_s_Going_to_print_constants) < 0) __PYX_ERR(0, 854, __pyx_L1_error)
 
-  /* "brainpy/_c/isotopic_distribution.pyx":843
+  /* "brainpy/_c/isotopic_distribution.pyx":855
  *     distribution = make_isotopic_distribution(composition, 4)
  *     print "Going to print constants"
  *     print_isotopic_constants(distribution._isotopic_constants)             # <<<<<<<<<<<<<<
  *     print "Done"
  * 
  */
   __pyx_f_7brainpy_2_c_18isotopic_constants_print_isotopic_constants(__pyx_v_distribution->_isotopic_constants);
 
-  /* "brainpy/_c/isotopic_distribution.pyx":844
+  /* "brainpy/_c/isotopic_distribution.pyx":856
  *     print "Going to print constants"
  *     print_isotopic_constants(distribution._isotopic_constants)
  *     print "Done"             # <<<<<<<<<<<<<<
  * 
  *     print "Trying to free"
  */
-  if (__Pyx_PrintOne(0, __pyx_n_s_Done) < 0) __PYX_ERR(0, 844, __pyx_L1_error)
+  if (__Pyx_PrintOne(0, __pyx_n_s_Done) < 0) __PYX_ERR(0, 856, __pyx_L1_error)
 
-  /* "brainpy/_c/isotopic_distribution.pyx":846
+  /* "brainpy/_c/isotopic_distribution.pyx":858
  *     print "Done"
  * 
  *     print "Trying to free"             # <<<<<<<<<<<<<<
  *     free_isotopic_distribution(distribution)
  *     print "Free Done"
  */
-  if (__Pyx_PrintOne(0, __pyx_kp_s_Trying_to_free) < 0) __PYX_ERR(0, 846, __pyx_L1_error)
+  if (__Pyx_PrintOne(0, __pyx_kp_s_Trying_to_free) < 0) __PYX_ERR(0, 858, __pyx_L1_error)
 
-  /* "brainpy/_c/isotopic_distribution.pyx":847
+  /* "brainpy/_c/isotopic_distribution.pyx":859
  * 
  *     print "Trying to free"
  *     free_isotopic_distribution(distribution)             # <<<<<<<<<<<<<<
  *     print "Free Done"
  * 
  */
   __pyx_f_7brainpy_2_c_21isotopic_distribution_free_isotopic_distribution(__pyx_v_distribution);
 
-  /* "brainpy/_c/isotopic_distribution.pyx":848
+  /* "brainpy/_c/isotopic_distribution.pyx":860
  *     print "Trying to free"
  *     free_isotopic_distribution(distribution)
  *     print "Free Done"             # <<<<<<<<<<<<<<
  * 
  *     distribution2 = make_isotopic_distribution(composition, 4)
  */
-  if (__Pyx_PrintOne(0, __pyx_kp_s_Free_Done) < 0) __PYX_ERR(0, 848, __pyx_L1_error)
+  if (__Pyx_PrintOne(0, __pyx_kp_s_Free_Done) < 0) __PYX_ERR(0, 860, __pyx_L1_error)
 
-  /* "brainpy/_c/isotopic_distribution.pyx":850
+  /* "brainpy/_c/isotopic_distribution.pyx":862
  *     print "Free Done"
  * 
  *     distribution2 = make_isotopic_distribution(composition, 4)             # <<<<<<<<<<<<<<
  *     print "Seconc construction"
  *     print_isotopic_constants(distribution2._isotopic_constants)
  */
   __pyx_v_distribution2 = __pyx_f_7brainpy_2_c_21isotopic_distribution_make_isotopic_distribution(__pyx_v_composition, 4, NULL);
 
-  /* "brainpy/_c/isotopic_distribution.pyx":851
+  /* "brainpy/_c/isotopic_distribution.pyx":863
  * 
  *     distribution2 = make_isotopic_distribution(composition, 4)
  *     print "Seconc construction"             # <<<<<<<<<<<<<<
  *     print_isotopic_constants(distribution2._isotopic_constants)
  *     print "Second Free"
  */
-  if (__Pyx_PrintOne(0, __pyx_kp_s_Seconc_construction) < 0) __PYX_ERR(0, 851, __pyx_L1_error)
+  if (__Pyx_PrintOne(0, __pyx_kp_s_Seconc_construction) < 0) __PYX_ERR(0, 863, __pyx_L1_error)
 
-  /* "brainpy/_c/isotopic_distribution.pyx":852
+  /* "brainpy/_c/isotopic_distribution.pyx":864
  *     distribution2 = make_isotopic_distribution(composition, 4)
  *     print "Seconc construction"
  *     print_isotopic_constants(distribution2._isotopic_constants)             # <<<<<<<<<<<<<<
  *     print "Second Free"
  *     free_isotopic_distribution(distribution2)
  */
   __pyx_f_7brainpy_2_c_18isotopic_constants_print_isotopic_constants(__pyx_v_distribution2->_isotopic_constants);
 
-  /* "brainpy/_c/isotopic_distribution.pyx":853
+  /* "brainpy/_c/isotopic_distribution.pyx":865
  *     print "Seconc construction"
  *     print_isotopic_constants(distribution2._isotopic_constants)
  *     print "Second Free"             # <<<<<<<<<<<<<<
  *     free_isotopic_distribution(distribution2)
  *     print comp_dict
  */
-  if (__Pyx_PrintOne(0, __pyx_kp_s_Second_Free) < 0) __PYX_ERR(0, 853, __pyx_L1_error)
+  if (__Pyx_PrintOne(0, __pyx_kp_s_Second_Free) < 0) __PYX_ERR(0, 865, __pyx_L1_error)
 
-  /* "brainpy/_c/isotopic_distribution.pyx":854
+  /* "brainpy/_c/isotopic_distribution.pyx":866
  *     print_isotopic_constants(distribution2._isotopic_constants)
  *     print "Second Free"
  *     free_isotopic_distribution(distribution2)             # <<<<<<<<<<<<<<
  *     print comp_dict
  *     free_composition(composition)
  */
   __pyx_f_7brainpy_2_c_21isotopic_distribution_free_isotopic_distribution(__pyx_v_distribution2);
 
-  /* "brainpy/_c/isotopic_distribution.pyx":855
+  /* "brainpy/_c/isotopic_distribution.pyx":867
  *     print "Second Free"
  *     free_isotopic_distribution(distribution2)
  *     print comp_dict             # <<<<<<<<<<<<<<
  *     free_composition(composition)
  *     print "Really done"
  */
-  if (__Pyx_PrintOne(0, __pyx_v_comp_dict) < 0) __PYX_ERR(0, 855, __pyx_L1_error)
+  if (__Pyx_PrintOne(0, __pyx_v_comp_dict) < 0) __PYX_ERR(0, 867, __pyx_L1_error)
 
-  /* "brainpy/_c/isotopic_distribution.pyx":856
+  /* "brainpy/_c/isotopic_distribution.pyx":868
  *     free_isotopic_distribution(distribution2)
  *     print comp_dict
  *     free_composition(composition)             # <<<<<<<<<<<<<<
  *     print "Really done"
  * 
  */
   __pyx_f_7brainpy_2_c_11composition_free_composition(__pyx_v_composition);
 
-  /* "brainpy/_c/isotopic_distribution.pyx":857
+  /* "brainpy/_c/isotopic_distribution.pyx":869
  *     print comp_dict
  *     free_composition(composition)
  *     print "Really done"             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  if (__Pyx_PrintOne(0, __pyx_kp_s_Really_done) < 0) __PYX_ERR(0, 857, __pyx_L1_error)
+  if (__Pyx_PrintOne(0, __pyx_kp_s_Really_done) < 0) __PYX_ERR(0, 869, __pyx_L1_error)
 
-  /* "brainpy/_c/isotopic_distribution.pyx":830
+  /* "brainpy/_c/isotopic_distribution.pyx":842
  * 
  * 
  * def main():             # <<<<<<<<<<<<<<
  *     cdef:
  *         dict comp_dict
  */
 
@@ -8757,15 +8757,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_comp_dict);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "brainpy/_c/isotopic_distribution.pyx":860
+/* "brainpy/_c/isotopic_distribution.pyx":872
  * 
  * 
  * def test(object composition, int max_npeaks=300):             # <<<<<<<<<<<<<<
  *     cdef:
  *         Composition* composition_struct
  */
 
@@ -8805,35 +8805,35 @@
         case  1:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_max_npeaks);
           if (value) { values[1] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "test") < 0)) __PYX_ERR(0, 860, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "test") < 0)) __PYX_ERR(0, 872, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_composition = values[0];
     if (values[1]) {
-      __pyx_v_max_npeaks = __Pyx_PyInt_As_int(values[1]); if (unlikely((__pyx_v_max_npeaks == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 860, __pyx_L3_error)
+      __pyx_v_max_npeaks = __Pyx_PyInt_As_int(values[1]); if (unlikely((__pyx_v_max_npeaks == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 872, __pyx_L3_error)
     } else {
       __pyx_v_max_npeaks = ((int)0x12C);
     }
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("test", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 860, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("test", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 872, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("brainpy._c.isotopic_distribution.test", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_7brainpy_2_c_21isotopic_distribution_8test(__pyx_self, __pyx_v_composition, __pyx_v_max_npeaks);
 
@@ -8854,179 +8854,179 @@
   PyObject *__pyx_t_2 = NULL;
   Py_ssize_t __pyx_t_3;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("test", 0);
 
-  /* "brainpy/_c/isotopic_distribution.pyx":866
+  /* "brainpy/_c/isotopic_distribution.pyx":878
  *         int npeaks, max_n_variants
  * 
  *     composition_struct = dict_to_composition(dict(composition))             # <<<<<<<<<<<<<<
  *     validate_composition(composition_struct)
  * 
  */
-  __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyDict_Type)), __pyx_v_composition); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 866, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyDict_Type)), __pyx_v_composition); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 878, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_composition_struct = __pyx_f_7brainpy_2_c_11composition_dict_to_composition(((PyObject*)__pyx_t_1));
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":867
+  /* "brainpy/_c/isotopic_distribution.pyx":879
  * 
  *     composition_struct = dict_to_composition(dict(composition))
  *     validate_composition(composition_struct)             # <<<<<<<<<<<<<<
  * 
  *     npeaks = guess_npeaks(composition_struct, max_npeaks)
  */
   (void)(__pyx_f_7brainpy_2_c_21isotopic_distribution_validate_composition(__pyx_v_composition_struct));
 
-  /* "brainpy/_c/isotopic_distribution.pyx":869
+  /* "brainpy/_c/isotopic_distribution.pyx":881
  *     validate_composition(composition_struct)
  * 
  *     npeaks = guess_npeaks(composition_struct, max_npeaks)             # <<<<<<<<<<<<<<
  *     print("Guessed # of Peaks: ", npeaks)
  * 
  */
   __pyx_v_npeaks = __pyx_f_7brainpy_2_c_21isotopic_distribution_guess_npeaks(__pyx_v_composition_struct, __pyx_v_max_npeaks, NULL);
 
-  /* "brainpy/_c/isotopic_distribution.pyx":870
+  /* "brainpy/_c/isotopic_distribution.pyx":882
  * 
  *     npeaks = guess_npeaks(composition_struct, max_npeaks)
  *     print("Guessed # of Peaks: ", npeaks)             # <<<<<<<<<<<<<<
  * 
  *     dist = make_isotopic_distribution(composition_struct, npeaks)
  */
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_npeaks); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 870, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_npeaks); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 882, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 870, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 882, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_kp_s_Guessed_of_Peaks);
   __Pyx_GIVEREF(__pyx_kp_s_Guessed_of_Peaks);
   PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_kp_s_Guessed_of_Peaks);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_t_1);
   __pyx_t_1 = 0;
-  if (__Pyx_PrintOne(0, __pyx_t_2) < 0) __PYX_ERR(0, 870, __pyx_L1_error)
+  if (__Pyx_PrintOne(0, __pyx_t_2) < 0) __PYX_ERR(0, 882, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":872
+  /* "brainpy/_c/isotopic_distribution.pyx":884
  *     print("Guessed # of Peaks: ", npeaks)
  * 
  *     dist = make_isotopic_distribution(composition_struct, npeaks)             # <<<<<<<<<<<<<<
  * 
  *     print("Size of probability vector:", id_probability_vector(dist).used)
  */
   __pyx_v_dist = __pyx_f_7brainpy_2_c_21isotopic_distribution_make_isotopic_distribution(__pyx_v_composition_struct, __pyx_v_npeaks, NULL);
 
-  /* "brainpy/_c/isotopic_distribution.pyx":874
+  /* "brainpy/_c/isotopic_distribution.pyx":886
  *     dist = make_isotopic_distribution(composition_struct, npeaks)
  * 
  *     print("Size of probability vector:", id_probability_vector(dist).used)             # <<<<<<<<<<<<<<
  * 
  *     peak_set = id_aggregated_isotopic_variants(dist, 1, PROTON)
  */
-  __pyx_t_2 = __Pyx_PyInt_FromSize_t(__pyx_f_7brainpy_2_c_21isotopic_distribution_id_probability_vector(__pyx_v_dist)->used); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 874, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_FromSize_t(__pyx_f_7brainpy_2_c_21isotopic_distribution_id_probability_vector(__pyx_v_dist)->used); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 886, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 874, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 886, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_kp_s_Size_of_probability_vector);
   __Pyx_GIVEREF(__pyx_kp_s_Size_of_probability_vector);
   PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_kp_s_Size_of_probability_vector);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_2);
   __pyx_t_2 = 0;
-  if (__Pyx_PrintOne(0, __pyx_t_1) < 0) __PYX_ERR(0, 874, __pyx_L1_error)
+  if (__Pyx_PrintOne(0, __pyx_t_1) < 0) __PYX_ERR(0, 886, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":876
+  /* "brainpy/_c/isotopic_distribution.pyx":888
  *     print("Size of probability vector:", id_probability_vector(dist).used)
  * 
  *     peak_set = id_aggregated_isotopic_variants(dist, 1, PROTON)             # <<<<<<<<<<<<<<
  * 
  *     peaklist = peaklist_to_list(peak_set)
  */
   __pyx_v_peak_set = __pyx_f_7brainpy_2_c_21isotopic_distribution_id_aggregated_isotopic_variants(__pyx_v_dist, 1, __pyx_v_7brainpy_2_c_11composition_PROTON);
 
-  /* "brainpy/_c/isotopic_distribution.pyx":878
+  /* "brainpy/_c/isotopic_distribution.pyx":890
  *     peak_set = id_aggregated_isotopic_variants(dist, 1, PROTON)
  * 
  *     peaklist = peaklist_to_list(peak_set)             # <<<<<<<<<<<<<<
  * 
  *     print("Actual # of Peaks Returned:", len(peaklist))
  */
-  __pyx_t_1 = __pyx_f_7brainpy_2_c_21isotopic_distribution_peaklist_to_list(__pyx_v_peak_set); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 878, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_7brainpy_2_c_21isotopic_distribution_peaklist_to_list(__pyx_v_peak_set); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 890, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_peaklist = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":880
+  /* "brainpy/_c/isotopic_distribution.pyx":892
  *     peaklist = peaklist_to_list(peak_set)
  * 
  *     print("Actual # of Peaks Returned:", len(peaklist))             # <<<<<<<<<<<<<<
  * 
  *     free_peak_list(peak_set)
  */
   if (unlikely(__pyx_v_peaklist == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-    __PYX_ERR(0, 880, __pyx_L1_error)
+    __PYX_ERR(0, 892, __pyx_L1_error)
   }
-  __pyx_t_3 = PyList_GET_SIZE(__pyx_v_peaklist); if (unlikely(__pyx_t_3 == ((Py_ssize_t)-1))) __PYX_ERR(0, 880, __pyx_L1_error)
-  __pyx_t_1 = PyInt_FromSsize_t(__pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 880, __pyx_L1_error)
+  __pyx_t_3 = PyList_GET_SIZE(__pyx_v_peaklist); if (unlikely(__pyx_t_3 == ((Py_ssize_t)-1))) __PYX_ERR(0, 892, __pyx_L1_error)
+  __pyx_t_1 = PyInt_FromSsize_t(__pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 892, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 880, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 892, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_kp_s_Actual_of_Peaks_Returned);
   __Pyx_GIVEREF(__pyx_kp_s_Actual_of_Peaks_Returned);
   PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_kp_s_Actual_of_Peaks_Returned);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_t_1);
   __pyx_t_1 = 0;
-  if (__Pyx_PrintOne(0, __pyx_t_2) < 0) __PYX_ERR(0, 880, __pyx_L1_error)
+  if (__Pyx_PrintOne(0, __pyx_t_2) < 0) __PYX_ERR(0, 892, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":882
+  /* "brainpy/_c/isotopic_distribution.pyx":894
  *     print("Actual # of Peaks Returned:", len(peaklist))
  * 
  *     free_peak_list(peak_set)             # <<<<<<<<<<<<<<
  *     free_isotopic_distribution(dist)
  *     free_composition(composition_struct)
  */
   __pyx_f_7brainpy_2_c_21isotopic_distribution_free_peak_list(__pyx_v_peak_set);
 
-  /* "brainpy/_c/isotopic_distribution.pyx":883
+  /* "brainpy/_c/isotopic_distribution.pyx":895
  * 
  *     free_peak_list(peak_set)
  *     free_isotopic_distribution(dist)             # <<<<<<<<<<<<<<
  *     free_composition(composition_struct)
  *     return peaklist
  */
   __pyx_f_7brainpy_2_c_21isotopic_distribution_free_isotopic_distribution(__pyx_v_dist);
 
-  /* "brainpy/_c/isotopic_distribution.pyx":884
+  /* "brainpy/_c/isotopic_distribution.pyx":896
  *     free_peak_list(peak_set)
  *     free_isotopic_distribution(dist)
  *     free_composition(composition_struct)             # <<<<<<<<<<<<<<
  *     return peaklist
  * 
  */
   __pyx_f_7brainpy_2_c_11composition_free_composition(__pyx_v_composition_struct);
 
-  /* "brainpy/_c/isotopic_distribution.pyx":885
+  /* "brainpy/_c/isotopic_distribution.pyx":897
  *     free_isotopic_distribution(dist)
  *     free_composition(composition_struct)
  *     return peaklist             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_peaklist);
   __pyx_r = __pyx_v_peaklist;
   goto __pyx_L0;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":860
+  /* "brainpy/_c/isotopic_distribution.pyx":872
  * 
  * 
  * def test(object composition, int max_npeaks=300):             # <<<<<<<<<<<<<<
  *     cdef:
  *         Composition* composition_struct
  */
 
@@ -9039,15 +9039,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_peaklist);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "brainpy/_c/isotopic_distribution.pyx":888
+/* "brainpy/_c/isotopic_distribution.pyx":900
  * 
  * 
  * cdef size_t max_variants_approx(double mass, double lambda_factor=1800.0, size_t maxiter=255,             # <<<<<<<<<<<<<<
  *                                 double threshold=0.9999) nogil:
  *     '''Approximate the maximum number of isotopic peaks to include in an isotopic distribution
  */
 
@@ -9077,207 +9077,207 @@
         if (__pyx_optional_args->__pyx_n > 2) {
           __pyx_v_threshold = __pyx_optional_args->threshold;
         }
       }
     }
   }
 
-  /* "brainpy/_c/isotopic_distribution.pyx":923
+  /* "brainpy/_c/isotopic_distribution.pyx":935
  *     '''
  *     cdef:
  *         double lmbda = mass / lambda_factor             # <<<<<<<<<<<<<<
  *         double p_i = 1.0
  *         double factorial_acc = 1.0
  */
   if (unlikely(__pyx_v_lambda_factor == 0)) {
     #ifdef WITH_THREAD
     PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
     #endif
     PyErr_SetString(PyExc_ZeroDivisionError, "float division");
     #ifdef WITH_THREAD
     __Pyx_PyGILState_Release(__pyx_gilstate_save);
     #endif
-    __PYX_ERR(0, 923, __pyx_L1_error)
+    __PYX_ERR(0, 935, __pyx_L1_error)
   }
   __pyx_v_lmbda = (__pyx_v_mass / __pyx_v_lambda_factor);
 
-  /* "brainpy/_c/isotopic_distribution.pyx":924
+  /* "brainpy/_c/isotopic_distribution.pyx":936
  *     cdef:
  *         double lmbda = mass / lambda_factor
  *         double p_i = 1.0             # <<<<<<<<<<<<<<
  *         double factorial_acc = 1.0
  *         double acc = 1.0
  */
   __pyx_v_p_i = 1.0;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":925
+  /* "brainpy/_c/isotopic_distribution.pyx":937
  *         double lmbda = mass / lambda_factor
  *         double p_i = 1.0
  *         double factorial_acc = 1.0             # <<<<<<<<<<<<<<
  *         double acc = 1.0
  *         double cur_intensity
  */
   __pyx_v_factorial_acc = 1.0;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":926
+  /* "brainpy/_c/isotopic_distribution.pyx":938
  *         double p_i = 1.0
  *         double factorial_acc = 1.0
  *         double acc = 1.0             # <<<<<<<<<<<<<<
  *         double cur_intensity
  *         size_t i
  */
   __pyx_v_acc = 1.0;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":930
+  /* "brainpy/_c/isotopic_distribution.pyx":942
  *         size_t i
  * 
  *     threshold = 1.0 - threshold             # <<<<<<<<<<<<<<
  *     for i in range(1, maxiter):
  *         p_i *= lmbda
  */
   __pyx_v_threshold = (1.0 - __pyx_v_threshold);
 
-  /* "brainpy/_c/isotopic_distribution.pyx":931
+  /* "brainpy/_c/isotopic_distribution.pyx":943
  * 
  *     threshold = 1.0 - threshold
  *     for i in range(1, maxiter):             # <<<<<<<<<<<<<<
  *         p_i *= lmbda
  *         factorial_acc *= i
  */
   __pyx_t_1 = __pyx_v_maxiter;
   __pyx_t_2 = __pyx_t_1;
   for (__pyx_t_3 = 1; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
     __pyx_v_i = __pyx_t_3;
 
-    /* "brainpy/_c/isotopic_distribution.pyx":932
+    /* "brainpy/_c/isotopic_distribution.pyx":944
  *     threshold = 1.0 - threshold
  *     for i in range(1, maxiter):
  *         p_i *= lmbda             # <<<<<<<<<<<<<<
  *         factorial_acc *= i
  *         cur_intensity = p_i / factorial_acc
  */
     __pyx_v_p_i = (__pyx_v_p_i * __pyx_v_lmbda);
 
-    /* "brainpy/_c/isotopic_distribution.pyx":933
+    /* "brainpy/_c/isotopic_distribution.pyx":945
  *     for i in range(1, maxiter):
  *         p_i *= lmbda
  *         factorial_acc *= i             # <<<<<<<<<<<<<<
  *         cur_intensity = p_i / factorial_acc
  *         if isinf(cur_intensity):
  */
     __pyx_v_factorial_acc = (__pyx_v_factorial_acc * __pyx_v_i);
 
-    /* "brainpy/_c/isotopic_distribution.pyx":934
+    /* "brainpy/_c/isotopic_distribution.pyx":946
  *         p_i *= lmbda
  *         factorial_acc *= i
  *         cur_intensity = p_i / factorial_acc             # <<<<<<<<<<<<<<
  *         if isinf(cur_intensity):
  *             return i
  */
     if (unlikely(__pyx_v_factorial_acc == 0)) {
       #ifdef WITH_THREAD
       PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
       #endif
       PyErr_SetString(PyExc_ZeroDivisionError, "float division");
       #ifdef WITH_THREAD
       __Pyx_PyGILState_Release(__pyx_gilstate_save);
       #endif
-      __PYX_ERR(0, 934, __pyx_L1_error)
+      __PYX_ERR(0, 946, __pyx_L1_error)
     }
     __pyx_v_cur_intensity = (__pyx_v_p_i / __pyx_v_factorial_acc);
 
-    /* "brainpy/_c/isotopic_distribution.pyx":935
+    /* "brainpy/_c/isotopic_distribution.pyx":947
  *         factorial_acc *= i
  *         cur_intensity = p_i / factorial_acc
  *         if isinf(cur_intensity):             # <<<<<<<<<<<<<<
  *             return i
  *         acc += cur_intensity
  */
     __pyx_t_4 = (isinf(__pyx_v_cur_intensity) != 0);
     if (__pyx_t_4) {
 
-      /* "brainpy/_c/isotopic_distribution.pyx":936
+      /* "brainpy/_c/isotopic_distribution.pyx":948
  *         cur_intensity = p_i / factorial_acc
  *         if isinf(cur_intensity):
  *             return i             # <<<<<<<<<<<<<<
  *         acc += cur_intensity
  *         if cur_intensity / acc < threshold:
  */
       __pyx_r = __pyx_v_i;
       goto __pyx_L0;
 
-      /* "brainpy/_c/isotopic_distribution.pyx":935
+      /* "brainpy/_c/isotopic_distribution.pyx":947
  *         factorial_acc *= i
  *         cur_intensity = p_i / factorial_acc
  *         if isinf(cur_intensity):             # <<<<<<<<<<<<<<
  *             return i
  *         acc += cur_intensity
  */
     }
 
-    /* "brainpy/_c/isotopic_distribution.pyx":937
+    /* "brainpy/_c/isotopic_distribution.pyx":949
  *         if isinf(cur_intensity):
  *             return i
  *         acc += cur_intensity             # <<<<<<<<<<<<<<
  *         if cur_intensity / acc < threshold:
  *             return i
  */
     __pyx_v_acc = (__pyx_v_acc + __pyx_v_cur_intensity);
 
-    /* "brainpy/_c/isotopic_distribution.pyx":938
+    /* "brainpy/_c/isotopic_distribution.pyx":950
  *             return i
  *         acc += cur_intensity
  *         if cur_intensity / acc < threshold:             # <<<<<<<<<<<<<<
  *             return i
  *     return 0
  */
     if (unlikely(__pyx_v_acc == 0)) {
       #ifdef WITH_THREAD
       PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
       #endif
       PyErr_SetString(PyExc_ZeroDivisionError, "float division");
       #ifdef WITH_THREAD
       __Pyx_PyGILState_Release(__pyx_gilstate_save);
       #endif
-      __PYX_ERR(0, 938, __pyx_L1_error)
+      __PYX_ERR(0, 950, __pyx_L1_error)
     }
     __pyx_t_4 = (((__pyx_v_cur_intensity / __pyx_v_acc) < __pyx_v_threshold) != 0);
     if (__pyx_t_4) {
 
-      /* "brainpy/_c/isotopic_distribution.pyx":939
+      /* "brainpy/_c/isotopic_distribution.pyx":951
  *         acc += cur_intensity
  *         if cur_intensity / acc < threshold:
  *             return i             # <<<<<<<<<<<<<<
  *     return 0
  * 
  */
       __pyx_r = __pyx_v_i;
       goto __pyx_L0;
 
-      /* "brainpy/_c/isotopic_distribution.pyx":938
+      /* "brainpy/_c/isotopic_distribution.pyx":950
  *             return i
  *         acc += cur_intensity
  *         if cur_intensity / acc < threshold:             # <<<<<<<<<<<<<<
  *             return i
  *     return 0
  */
     }
   }
 
-  /* "brainpy/_c/isotopic_distribution.pyx":940
+  /* "brainpy/_c/isotopic_distribution.pyx":952
  *         if cur_intensity / acc < threshold:
  *             return i
  *     return 0             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = 0;
   goto __pyx_L0;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":888
+  /* "brainpy/_c/isotopic_distribution.pyx":900
  * 
  * 
  * cdef size_t max_variants_approx(double mass, double lambda_factor=1800.0, size_t maxiter=255,             # <<<<<<<<<<<<<<
  *                                 double threshold=0.9999) nogil:
  *     '''Approximate the maximum number of isotopic peaks to include in an isotopic distribution
  */
 
@@ -9285,15 +9285,15 @@
   __pyx_L1_error:;
   __Pyx_WriteUnraisable("brainpy._c.isotopic_distribution.max_variants_approx", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 1);
   __pyx_r = 0;
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "brainpy/_c/isotopic_distribution.pyx":943
+/* "brainpy/_c/isotopic_distribution.pyx":955
  * 
  * 
  * def py_max_variants_approx(double mass, double lambda_factor=1800.0, size_t maxiter=255,             # <<<<<<<<<<<<<<
  *                            double threshold=0.9999):
  *     with nogil:
  */
 
@@ -9351,49 +9351,49 @@
         case  3:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_threshold);
           if (value) { values[3] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "py_max_variants_approx") < 0)) __PYX_ERR(0, 943, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "py_max_variants_approx") < 0)) __PYX_ERR(0, 955, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
         CYTHON_FALLTHROUGH;
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
-    __pyx_v_mass = __pyx_PyFloat_AsDouble(values[0]); if (unlikely((__pyx_v_mass == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 943, __pyx_L3_error)
+    __pyx_v_mass = __pyx_PyFloat_AsDouble(values[0]); if (unlikely((__pyx_v_mass == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 955, __pyx_L3_error)
     if (values[1]) {
-      __pyx_v_lambda_factor = __pyx_PyFloat_AsDouble(values[1]); if (unlikely((__pyx_v_lambda_factor == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 943, __pyx_L3_error)
+      __pyx_v_lambda_factor = __pyx_PyFloat_AsDouble(values[1]); if (unlikely((__pyx_v_lambda_factor == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 955, __pyx_L3_error)
     } else {
       __pyx_v_lambda_factor = ((double)1800.0);
     }
     if (values[2]) {
-      __pyx_v_maxiter = __Pyx_PyInt_As_size_t(values[2]); if (unlikely((__pyx_v_maxiter == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 943, __pyx_L3_error)
+      __pyx_v_maxiter = __Pyx_PyInt_As_size_t(values[2]); if (unlikely((__pyx_v_maxiter == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 955, __pyx_L3_error)
     } else {
       __pyx_v_maxiter = ((size_t)0xFF);
     }
     if (values[3]) {
-      __pyx_v_threshold = __pyx_PyFloat_AsDouble(values[3]); if (unlikely((__pyx_v_threshold == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 944, __pyx_L3_error)
+      __pyx_v_threshold = __pyx_PyFloat_AsDouble(values[3]); if (unlikely((__pyx_v_threshold == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 956, __pyx_L3_error)
     } else {
       __pyx_v_threshold = ((double)0.9999);
     }
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("py_max_variants_approx", 0, 1, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 943, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("py_max_variants_approx", 0, 1, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 955, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("brainpy._c.isotopic_distribution.py_max_variants_approx", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_7brainpy_2_c_21isotopic_distribution_10py_max_variants_approx(__pyx_self, __pyx_v_mass, __pyx_v_lambda_factor, __pyx_v_maxiter, __pyx_v_threshold);
 
@@ -9410,44 +9410,44 @@
   struct __pyx_opt_args_7brainpy_2_c_21isotopic_distribution_max_variants_approx __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("py_max_variants_approx", 0);
 
-  /* "brainpy/_c/isotopic_distribution.pyx":945
+  /* "brainpy/_c/isotopic_distribution.pyx":957
  * def py_max_variants_approx(double mass, double lambda_factor=1800.0, size_t maxiter=255,
  *                            double threshold=0.9999):
  *     with nogil:             # <<<<<<<<<<<<<<
  *         val = max_variants_approx(mass, lambda_factor, maxiter, threshold)
  *     return val
  */
   {
       #ifdef WITH_THREAD
       PyThreadState *_save;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "brainpy/_c/isotopic_distribution.pyx":946
+        /* "brainpy/_c/isotopic_distribution.pyx":958
  *                            double threshold=0.9999):
  *     with nogil:
  *         val = max_variants_approx(mass, lambda_factor, maxiter, threshold)             # <<<<<<<<<<<<<<
  *     return val
  */
         __pyx_t_2.__pyx_n = 3;
         __pyx_t_2.lambda_factor = __pyx_v_lambda_factor;
         __pyx_t_2.maxiter = __pyx_v_maxiter;
         __pyx_t_2.threshold = __pyx_v_threshold;
         __pyx_t_1 = __pyx_f_7brainpy_2_c_21isotopic_distribution_max_variants_approx(__pyx_v_mass, &__pyx_t_2); 
         __pyx_v_val = __pyx_t_1;
       }
 
-      /* "brainpy/_c/isotopic_distribution.pyx":945
+      /* "brainpy/_c/isotopic_distribution.pyx":957
  * def py_max_variants_approx(double mass, double lambda_factor=1800.0, size_t maxiter=255,
  *                            double threshold=0.9999):
  *     with nogil:             # <<<<<<<<<<<<<<
  *         val = max_variants_approx(mass, lambda_factor, maxiter, threshold)
  *     return val
  */
       /*finally:*/ {
@@ -9458,27 +9458,27 @@
           #endif
           goto __pyx_L5;
         }
         __pyx_L5:;
       }
   }
 
-  /* "brainpy/_c/isotopic_distribution.pyx":947
+  /* "brainpy/_c/isotopic_distribution.pyx":959
  *     with nogil:
  *         val = max_variants_approx(mass, lambda_factor, maxiter, threshold)
  *     return val             # <<<<<<<<<<<<<<
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_3 = __Pyx_PyInt_FromSize_t(__pyx_v_val); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 947, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_FromSize_t(__pyx_v_val); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 959, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_r = __pyx_t_3;
   __pyx_t_3 = 0;
   goto __pyx_L0;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":943
+  /* "brainpy/_c/isotopic_distribution.pyx":955
  * 
  * 
  * def py_max_variants_approx(double mass, double lambda_factor=1800.0, size_t maxiter=255,             # <<<<<<<<<<<<<<
  *                            double threshold=0.9999):
  *     with nogil:
  */
 
@@ -9756,83 +9756,83 @@
   {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
   {&__pyx_n_s_test_2, __pyx_k_test_2, sizeof(__pyx_k_test_2), 0, 0, 1, 1},
   {&__pyx_n_s_threshold, __pyx_k_threshold, sizeof(__pyx_k_threshold), 0, 0, 1, 1},
   {&__pyx_n_s_val, __pyx_k_val, sizeof(__pyx_k_val), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
-  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 183, __pyx_L1_error)
-  __pyx_builtin_KeyError = __Pyx_GetBuiltinName(__pyx_n_s_KeyError); if (!__pyx_builtin_KeyError) __PYX_ERR(0, 733, __pyx_L1_error)
+  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 195, __pyx_L1_error)
+  __pyx_builtin_KeyError = __Pyx_GetBuiltinName(__pyx_n_s_KeyError); if (!__pyx_builtin_KeyError) __PYX_ERR(0, 745, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "brainpy/_c/isotopic_distribution.pyx":733
+  /* "brainpy/_c/isotopic_distribution.pyx":745
  *     if validate_composition(composition_struct) != 0:
  *         free_composition(composition_struct)
  *         raise KeyError("Unrecognized Isotope")             # <<<<<<<<<<<<<<
  * 
  *     if npeaks is None:
  */
-  __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_s_Unrecognized_Isotope); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 733, __pyx_L1_error)
+  __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_s_Unrecognized_Isotope); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 745, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__3);
   __Pyx_GIVEREF(__pyx_tuple__3);
 
-  /* "brainpy/_c/isotopic_distribution.pyx":673
+  /* "brainpy/_c/isotopic_distribution.pyx":685
  * 
  * 
  * def pyisotopic_variants(object composition not None, object npeaks=None, int charge=0,             # <<<<<<<<<<<<<<
  *                         double charge_carrier=PROTON):
  *     '''
  */
-  __pyx_tuple__5 = PyTuple_Pack(4, __pyx_n_s_composition, __pyx_n_s_npeaks, __pyx_n_s_charge, __pyx_n_s_charge_carrier); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(0, 673, __pyx_L1_error)
+  __pyx_tuple__5 = PyTuple_Pack(4, __pyx_n_s_composition, __pyx_n_s_npeaks, __pyx_n_s_charge, __pyx_n_s_charge_carrier); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(0, 685, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__5);
   __Pyx_GIVEREF(__pyx_tuple__5);
-  __pyx_codeobj__6 = (PyObject*)__Pyx_PyCode_New(4, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__5, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_brainpy__c_isotopic_distribution, __pyx_n_s_pyisotopic_variants, 673, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__6)) __PYX_ERR(0, 673, __pyx_L1_error)
+  __pyx_codeobj__6 = (PyObject*)__Pyx_PyCode_New(4, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__5, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_brainpy__c_isotopic_distribution, __pyx_n_s_pyisotopic_variants, 685, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__6)) __PYX_ERR(0, 685, __pyx_L1_error)
 
-  /* "brainpy/_c/isotopic_distribution.pyx":830
+  /* "brainpy/_c/isotopic_distribution.pyx":842
  * 
  * 
  * def main():             # <<<<<<<<<<<<<<
  *     cdef:
  *         dict comp_dict
  */
-  __pyx_tuple__7 = PyTuple_Pack(4, __pyx_n_s_comp_dict, __pyx_n_s_composition, __pyx_n_s_distribution, __pyx_n_s_distribution2); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(0, 830, __pyx_L1_error)
+  __pyx_tuple__7 = PyTuple_Pack(4, __pyx_n_s_comp_dict, __pyx_n_s_composition, __pyx_n_s_distribution, __pyx_n_s_distribution2); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(0, 842, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__7);
   __Pyx_GIVEREF(__pyx_tuple__7);
-  __pyx_codeobj__8 = (PyObject*)__Pyx_PyCode_New(0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__7, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_brainpy__c_isotopic_distribution, __pyx_n_s_main_2, 830, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__8)) __PYX_ERR(0, 830, __pyx_L1_error)
+  __pyx_codeobj__8 = (PyObject*)__Pyx_PyCode_New(0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__7, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_brainpy__c_isotopic_distribution, __pyx_n_s_main_2, 842, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__8)) __PYX_ERR(0, 842, __pyx_L1_error)
 
-  /* "brainpy/_c/isotopic_distribution.pyx":860
+  /* "brainpy/_c/isotopic_distribution.pyx":872
  * 
  * 
  * def test(object composition, int max_npeaks=300):             # <<<<<<<<<<<<<<
  *     cdef:
  *         Composition* composition_struct
  */
-  __pyx_tuple__9 = PyTuple_Pack(9, __pyx_n_s_composition, __pyx_n_s_max_npeaks, __pyx_n_s_composition_struct, __pyx_n_s_distribution, __pyx_n_s_npeaks, __pyx_n_s_max_n_variants, __pyx_n_s_dist, __pyx_n_s_peak_set, __pyx_n_s_peaklist); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(0, 860, __pyx_L1_error)
+  __pyx_tuple__9 = PyTuple_Pack(9, __pyx_n_s_composition, __pyx_n_s_max_npeaks, __pyx_n_s_composition_struct, __pyx_n_s_distribution, __pyx_n_s_npeaks, __pyx_n_s_max_n_variants, __pyx_n_s_dist, __pyx_n_s_peak_set, __pyx_n_s_peaklist); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(0, 872, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__9);
   __Pyx_GIVEREF(__pyx_tuple__9);
-  __pyx_codeobj__10 = (PyObject*)__Pyx_PyCode_New(2, 0, 9, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__9, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_brainpy__c_isotopic_distribution, __pyx_n_s_test, 860, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__10)) __PYX_ERR(0, 860, __pyx_L1_error)
+  __pyx_codeobj__10 = (PyObject*)__Pyx_PyCode_New(2, 0, 9, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__9, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_brainpy__c_isotopic_distribution, __pyx_n_s_test, 872, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__10)) __PYX_ERR(0, 872, __pyx_L1_error)
 
-  /* "brainpy/_c/isotopic_distribution.pyx":943
+  /* "brainpy/_c/isotopic_distribution.pyx":955
  * 
  * 
  * def py_max_variants_approx(double mass, double lambda_factor=1800.0, size_t maxiter=255,             # <<<<<<<<<<<<<<
  *                            double threshold=0.9999):
  *     with nogil:
  */
-  __pyx_tuple__11 = PyTuple_Pack(5, __pyx_n_s_mass, __pyx_n_s_lambda_factor, __pyx_n_s_maxiter, __pyx_n_s_threshold, __pyx_n_s_val); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(0, 943, __pyx_L1_error)
+  __pyx_tuple__11 = PyTuple_Pack(5, __pyx_n_s_mass, __pyx_n_s_lambda_factor, __pyx_n_s_maxiter, __pyx_n_s_threshold, __pyx_n_s_val); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(0, 955, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__11);
   __Pyx_GIVEREF(__pyx_tuple__11);
-  __pyx_codeobj__12 = (PyObject*)__Pyx_PyCode_New(4, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__11, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_brainpy__c_isotopic_distribution, __pyx_n_s_py_max_variants_approx, 943, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__12)) __PYX_ERR(0, 943, __pyx_L1_error)
+  __pyx_codeobj__12 = (PyObject*)__Pyx_PyCode_New(4, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__11, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_brainpy__c_isotopic_distribution, __pyx_n_s_py_max_variants_approx, 955, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__12)) __PYX_ERR(0, 955, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
@@ -9915,23 +9915,23 @@
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_init_code", 0);
   /*--- Type init code ---*/
   __pyx_vtabptr_7brainpy_2_c_21isotopic_distribution_TheoreticalPeak = &__pyx_vtable_7brainpy_2_c_21isotopic_distribution_TheoreticalPeak;
   __pyx_vtable_7brainpy_2_c_21isotopic_distribution_TheoreticalPeak._create = (struct __pyx_obj_7brainpy_2_c_21isotopic_distribution_TheoreticalPeak *(*)(double, double, int))__pyx_f_7brainpy_2_c_21isotopic_distribution_15TheoreticalPeak__create;
   __pyx_vtable_7brainpy_2_c_21isotopic_distribution_TheoreticalPeak._eq = (int (*)(struct __pyx_obj_7brainpy_2_c_21isotopic_distribution_TheoreticalPeak *, struct __pyx_obj_7brainpy_2_c_21isotopic_distribution_TheoreticalPeak *, int __pyx_skip_dispatch))__pyx_f_7brainpy_2_c_21isotopic_distribution_15TheoreticalPeak__eq;
   __pyx_vtable_7brainpy_2_c_21isotopic_distribution_TheoreticalPeak.clone = (struct __pyx_obj_7brainpy_2_c_21isotopic_distribution_TheoreticalPeak *(*)(struct __pyx_obj_7brainpy_2_c_21isotopic_distribution_TheoreticalPeak *, int __pyx_skip_dispatch))__pyx_f_7brainpy_2_c_21isotopic_distribution_15TheoreticalPeak_clone;
-  if (PyType_Ready(&__pyx_type_7brainpy_2_c_21isotopic_distribution_TheoreticalPeak) < 0) __PYX_ERR(0, 788, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_7brainpy_2_c_21isotopic_distribution_TheoreticalPeak) < 0) __PYX_ERR(0, 800, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_7brainpy_2_c_21isotopic_distribution_TheoreticalPeak.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_7brainpy_2_c_21isotopic_distribution_TheoreticalPeak.tp_dictoffset && __pyx_type_7brainpy_2_c_21isotopic_distribution_TheoreticalPeak.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_7brainpy_2_c_21isotopic_distribution_TheoreticalPeak.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (__Pyx_SetVtable(__pyx_type_7brainpy_2_c_21isotopic_distribution_TheoreticalPeak.tp_dict, __pyx_vtabptr_7brainpy_2_c_21isotopic_distribution_TheoreticalPeak) < 0) __PYX_ERR(0, 788, __pyx_L1_error)
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_TheoreticalPeak, (PyObject *)&__pyx_type_7brainpy_2_c_21isotopic_distribution_TheoreticalPeak) < 0) __PYX_ERR(0, 788, __pyx_L1_error)
+  if (__Pyx_SetVtable(__pyx_type_7brainpy_2_c_21isotopic_distribution_TheoreticalPeak.tp_dict, __pyx_vtabptr_7brainpy_2_c_21isotopic_distribution_TheoreticalPeak) < 0) __PYX_ERR(0, 800, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_TheoreticalPeak, (PyObject *)&__pyx_type_7brainpy_2_c_21isotopic_distribution_TheoreticalPeak) < 0) __PYX_ERR(0, 800, __pyx_L1_error)
   __pyx_ptype_7brainpy_2_c_21isotopic_distribution_TheoreticalPeak = &__pyx_type_7brainpy_2_c_21isotopic_distribution_TheoreticalPeak;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
@@ -10237,88 +10237,88 @@
   if (unlikely(__Pyx_modinit_variable_import_code() < 0)) __PYX_ERR(0, 1, __pyx_L1_error)
   if (unlikely(__Pyx_modinit_function_import_code() < 0)) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Execution code ---*/
   #if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
   if (__Pyx_patch_abc() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
 
-  /* "brainpy/_c/isotopic_distribution.pyx":674
+  /* "brainpy/_c/isotopic_distribution.pyx":686
  * 
  * def pyisotopic_variants(object composition not None, object npeaks=None, int charge=0,
  *                         double charge_carrier=PROTON):             # <<<<<<<<<<<<<<
  *     '''
  *     Compute a peak list representing the theoretical isotopic cluster for `composition`.
  */
   __pyx_k_ = __pyx_v_7brainpy_2_c_11composition_PROTON;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":673
+  /* "brainpy/_c/isotopic_distribution.pyx":685
  * 
  * 
  * def pyisotopic_variants(object composition not None, object npeaks=None, int charge=0,             # <<<<<<<<<<<<<<
  *                         double charge_carrier=PROTON):
  *     '''
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_7brainpy_2_c_21isotopic_distribution_3pyisotopic_variants, NULL, __pyx_n_s_brainpy__c_isotopic_distribution_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 673, __pyx_L1_error)
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_7brainpy_2_c_21isotopic_distribution_3pyisotopic_variants, NULL, __pyx_n_s_brainpy__c_isotopic_distribution_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 685, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_pyisotopic_variants, __pyx_t_1) < 0) __PYX_ERR(0, 673, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_pyisotopic_variants, __pyx_t_1) < 0) __PYX_ERR(0, 685, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":700
+  /* "brainpy/_c/isotopic_distribution.pyx":712
  * 
  * 
  * cpdef list _isotopic_variants(object composition, object npeaks=None, int charge=0, double charge_carrier=PROTON):             # <<<<<<<<<<<<<<
  *     '''
  *     Compute a peak list representing the theoretical isotopic cluster for `composition`.
  */
   __pyx_k__2 = __pyx_v_7brainpy_2_c_11composition_PROTON;
   __pyx_k__2 = __pyx_v_7brainpy_2_c_11composition_PROTON;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":754
+  /* "brainpy/_c/isotopic_distribution.pyx":766
  * 
  * 
  * cdef PeakList* isotopic_variants(Composition* composition, int npeaks, int charge=0, double charge_carrier=PROTON) nogil:             # <<<<<<<<<<<<<<
  *     cdef:
  *         IsotopicDistribution* dist
  */
   __pyx_k__4 = __pyx_v_7brainpy_2_c_11composition_PROTON;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":830
+  /* "brainpy/_c/isotopic_distribution.pyx":842
  * 
  * 
  * def main():             # <<<<<<<<<<<<<<
  *     cdef:
  *         dict comp_dict
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_7brainpy_2_c_21isotopic_distribution_7main, NULL, __pyx_n_s_brainpy__c_isotopic_distribution_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 830, __pyx_L1_error)
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_7brainpy_2_c_21isotopic_distribution_7main, NULL, __pyx_n_s_brainpy__c_isotopic_distribution_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 842, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_main_2, __pyx_t_1) < 0) __PYX_ERR(0, 830, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_main_2, __pyx_t_1) < 0) __PYX_ERR(0, 842, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":860
+  /* "brainpy/_c/isotopic_distribution.pyx":872
  * 
  * 
  * def test(object composition, int max_npeaks=300):             # <<<<<<<<<<<<<<
  *     cdef:
  *         Composition* composition_struct
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_7brainpy_2_c_21isotopic_distribution_9test, NULL, __pyx_n_s_brainpy__c_isotopic_distribution_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 860, __pyx_L1_error)
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_7brainpy_2_c_21isotopic_distribution_9test, NULL, __pyx_n_s_brainpy__c_isotopic_distribution_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 872, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_1) < 0) __PYX_ERR(0, 860, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_1) < 0) __PYX_ERR(0, 872, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "brainpy/_c/isotopic_distribution.pyx":943
+  /* "brainpy/_c/isotopic_distribution.pyx":955
  * 
  * 
  * def py_max_variants_approx(double mass, double lambda_factor=1800.0, size_t maxiter=255,             # <<<<<<<<<<<<<<
  *                            double threshold=0.9999):
  *     with nogil:
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_7brainpy_2_c_21isotopic_distribution_11py_max_variants_approx, NULL, __pyx_n_s_brainpy__c_isotopic_distribution_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 943, __pyx_L1_error)
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_7brainpy_2_c_21isotopic_distribution_11py_max_variants_approx, NULL, __pyx_n_s_brainpy__c_isotopic_distribution_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 955, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_py_max_variants_approx, __pyx_t_1) < 0) __PYX_ERR(0, 943, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_py_max_variants_approx, __pyx_t_1) < 0) __PYX_ERR(0, 955, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "brainpy/_c/isotopic_distribution.pyx":1
  * # cython: embedsignature=True             # <<<<<<<<<<<<<<
  * # -*- coding: utf-8 -*-
  * cimport cython
  */
```

### Comparing `brain-isotopic-distribution-1.5.8/brainpy/_c/isotopic_distribution.pxd` & `brain-isotopic-distribution-1.5.9/brainpy/_c/isotopic_distribution.pxd`

 * *Files identical despite different names*

### Comparing `brain-isotopic-distribution-1.5.8/brainpy/_c/isotopic_distribution.pyx` & `brain-isotopic-distribution-1.5.9/brainpy/_c/isotopic_distribution.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from brainpy._c.double_vector cimport(
     DoubleVector, make_double_vector, double_vector_append,
     make_double_vector_with_size,
     free_double_vector, print_double_vector, reset_double_vector)
 
 from libc.stdlib cimport malloc, free, realloc
 from libc.string cimport strcmp
-from libc.math cimport log, exp, sqrt, isinf
+from libc.math cimport log, exp, sqrt, fabs
 from libc cimport *
 
 from brainpy._c.isotopic_constants cimport (
     IsotopicConstants, isotopic_constants_get, make_isotopic_constants,
     isotopic_constants_resize, free_isotopic_constants, isotopic_constants_add_element,
     isotopic_constants_update_coefficients,
     isotopic_constants_nth_element_power_sum, print_isotopic_constants,
@@ -40,14 +40,26 @@
 
 
 cdef extern from * nogil:
     int printf (const char *template, ...)
     void qsort (void *base, unsigned short n, unsigned short w, int (*cmp_func)(void*, void*))
 
 
+IF int == long:
+    DEF PY_VERSION = 3
+ELSE:
+    DEF PY_VERSION = 2
+IF UNAME_SYSNAME == "Windows" and PY_VERSION == 2:
+    cdef double INFINITY = float('inf')
+
+    cdef int isinf(double x) nogil:
+        return fabs(x) == INFINITY
+ELSE:
+    from libc.math cimport isinf as isinf
+
 # -----------------------------------------------------------------------------
 # ElementPolynomialMap Declaration and Methods
 
 cdef struct ElementPolynomialMap:
     char** elements
     dvec** polynomials
     size_t used
```

### Comparing `brain-isotopic-distribution-1.5.8/brainpy/_speedup.c` & `brain-isotopic-distribution-1.5.9/brainpy/_speedup.c`

 * *Files identical despite different names*

### Comparing `brain-isotopic-distribution-1.5.8/brainpy/_speedup.pxd` & `brain-isotopic-distribution-1.5.9/brainpy/_speedup.pxd`

 * *Files identical despite different names*

### Comparing `brain-isotopic-distribution-1.5.8/brainpy/_speedup.pyx` & `brain-isotopic-distribution-1.5.9/brainpy/_speedup.pyx`

 * *Files identical despite different names*

### Comparing `brain-isotopic-distribution-1.5.8/brainpy/brainpy.py` & `brain-isotopic-distribution-1.5.9/brainpy/brainpy.py`

 * *Files identical despite different names*

### Comparing `brain-isotopic-distribution-1.5.8/brainpy/composition.py` & `brain-isotopic-distribution-1.5.9/brainpy/composition.py`

 * *Files identical despite different names*

### Comparing `brain-isotopic-distribution-1.5.8/brainpy/mass_dict.py` & `brain-isotopic-distribution-1.5.9/brainpy/mass_dict.py`

 * *Files identical despite different names*

### Comparing `brain-isotopic-distribution-1.5.8/brainpy/test/test_composition.py` & `brain-isotopic-distribution-1.5.9/brainpy/test/test_composition.py`

 * *Files identical despite different names*

### Comparing `brain-isotopic-distribution-1.5.8/brainpy/test/test_isotopic_distribution.py` & `brain-isotopic-distribution-1.5.9/brainpy/test/test_isotopic_distribution.py`

 * *Files identical despite different names*

### Comparing `brain-isotopic-distribution-1.5.8/setup.py` & `brain-isotopic-distribution-1.5.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,15 +115,15 @@
         print(msg)
     print('*' * 75)
 
 
 def run_setup(include_cext=True):
     setup(
         name='brain-isotopic-distribution',
-        version='1.5.8',
+        version='1.5.9',
         packages=find_packages(),
         description="Fast and efficient theoretical isotopic profile generation",
         long_description='''
 :mod:`brainpy` is a small Python library implementing the *B* afflingly *R* ecursive
 *A* lgorithm for *I* sotopic Patter *N* generation [Dittwald2014]_. It includes three implementations,
 a pure-Python object oriented implementation, a :title-reference:`Cython` accelerated
 version of the object oriented implementation, and a pure :title-reference:`C` implementation,
```

