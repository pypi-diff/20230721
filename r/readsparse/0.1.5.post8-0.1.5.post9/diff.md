# Comparing `tmp/readsparse-0.1.5.post8.tar.gz` & `tmp/readsparse-0.1.5.post9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "readsparse-0.1.5.post8.tar", last modified: Sat Jul 15 11:14:40 2023, max compression
+gzip compressed data, was "readsparse-0.1.5.post9.tar", last modified: Tue Jul 18 21:17:27 2023, max compression
```

## Comparing `readsparse-0.1.5.post8.tar` & `readsparse-0.1.5.post9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-07-15 11:14:40.636311 readsparse-0.1.5.post8/
--rw-r--r--   0 david     (1000) david     (1000)     1317 2021-01-02 12:50:02.000000 readsparse-0.1.5.post8/LICENSE
--rw-r--r--   0 david     (1000) david     (1000)      371 2021-08-22 23:35:24.000000 readsparse-0.1.5.post8/MANIFEST.in
--rw-r--r--   0 david     (1000) david     (1000)      245 2023-07-15 11:14:40.636311 readsparse-0.1.5.post8/PKG-INFO
--rw-r--r--   0 david     (1000) david     (1000)       86 2021-04-15 16:03:50.000000 readsparse-0.1.5.post8/pyproject.toml
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-07-15 11:14:40.632311 readsparse-0.1.5.post8/readsparse/
--rw-r--r--   0 david     (1000) david     (1000)    26992 2023-07-03 19:01:43.000000 readsparse-0.1.5.post8/readsparse/__init__.py
--rw-r--r--   0 david     (1000) david     (1000)    70879 2021-06-25 15:16:58.000000 readsparse-0.1.5.post8/readsparse/cpp_interface.pxi
--rw-r--r--   0 david     (1000) david     (1000)       83 2021-01-04 13:36:06.000000 readsparse-0.1.5.post8/readsparse/cpp_interface_size_t.pyx
--rw-r--r--   0 david     (1000) david     (1000)      120 2021-01-04 13:31:53.000000 readsparse-0.1.5.post8/readsparse/cpp_interface_uint64_t.pyx
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-07-15 11:14:40.632311 readsparse-0.1.5.post8/readsparse.egg-info/
--rw-r--r--   0 david     (1000) david     (1000)      245 2023-07-15 11:14:40.000000 readsparse-0.1.5.post8/readsparse.egg-info/PKG-INFO
--rw-r--r--   0 david     (1000) david     (1000)      480 2023-07-15 11:14:40.000000 readsparse-0.1.5.post8/readsparse.egg-info/SOURCES.txt
--rw-r--r--   0 david     (1000) david     (1000)        1 2023-07-15 11:14:40.000000 readsparse-0.1.5.post8/readsparse.egg-info/dependency_links.txt
--rw-r--r--   0 david     (1000) david     (1000)       11 2023-07-15 11:14:40.000000 readsparse-0.1.5.post8/readsparse.egg-info/top_level.txt
--rw-r--r--   0 david     (1000) david     (1000)       38 2023-07-15 11:14:40.636311 readsparse-0.1.5.post8/setup.cfg
--rw-r--r--   0 david     (1000) david     (1000)     9648 2023-07-15 11:14:08.000000 readsparse-0.1.5.post8/setup.py
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-07-15 11:14:40.636311 readsparse-0.1.5.post8/src/
--rw-r--r--   0 david     (1000) david     (1000)     5594 2021-07-25 03:01:47.000000 readsparse-0.1.5.post8/src/python_streams.hpp
--rw-r--r--   0 david     (1000) david     (1000)    89722 2021-06-25 15:11:19.000000 readsparse-0.1.5.post8/src/reader.cpp
--rw-r--r--   0 david     (1000) david     (1000)    58520 2022-01-16 21:05:53.000000 readsparse-0.1.5.post8/src/reader.hpp
--rw-r--r--   0 david     (1000) david     (1000)    15446 2021-06-25 15:12:25.000000 readsparse-0.1.5.post8/src/readsparse.hpp
--rw-r--r--   0 david     (1000) david     (1000)    95786 2021-06-25 15:11:19.000000 readsparse-0.1.5.post8/src/readsparse_detemplated.hpp
--rw-r--r--   0 david     (1000) david     (1000)    10285 2022-09-11 18:48:32.000000 readsparse-0.1.5.post8/src/readsparse_internal.hpp
--rw-r--r--   0 david     (1000) david     (1000)     7226 2021-08-25 00:18:42.000000 readsparse-0.1.5.post8/src/utils.hpp
--rw-r--r--   0 david     (1000) david     (1000)    71373 2021-06-25 15:11:19.000000 readsparse-0.1.5.post8/src/writer.cpp
--rw-r--r--   0 david     (1000) david     (1000)    37907 2021-07-14 01:23:59.000000 readsparse-0.1.5.post8/src/writer.hpp
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-07-18 21:17:27.564504 readsparse-0.1.5.post9/
+-rw-r--r--   0 david     (1000) david     (1000)     1317 2021-01-02 12:50:02.000000 readsparse-0.1.5.post9/LICENSE
+-rw-r--r--   0 david     (1000) david     (1000)      371 2021-08-22 23:35:24.000000 readsparse-0.1.5.post9/MANIFEST.in
+-rw-r--r--   0 david     (1000) david     (1000)      245 2023-07-18 21:17:27.564504 readsparse-0.1.5.post9/PKG-INFO
+-rw-r--r--   0 david     (1000) david     (1000)       84 2023-07-18 21:14:55.000000 readsparse-0.1.5.post9/pyproject.toml
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-07-18 21:17:27.560504 readsparse-0.1.5.post9/readsparse/
+-rw-r--r--   0 david     (1000) david     (1000)    26992 2023-07-03 19:01:43.000000 readsparse-0.1.5.post9/readsparse/__init__.py
+-rw-r--r--   0 david     (1000) david     (1000)    70879 2023-07-18 21:14:37.000000 readsparse-0.1.5.post9/readsparse/cpp_interface.pxi
+-rw-r--r--   0 david     (1000) david     (1000)       83 2021-01-04 13:36:06.000000 readsparse-0.1.5.post9/readsparse/cpp_interface_size_t.pyx
+-rw-r--r--   0 david     (1000) david     (1000)      120 2021-01-04 13:31:53.000000 readsparse-0.1.5.post9/readsparse/cpp_interface_uint64_t.pyx
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-07-18 21:17:27.560504 readsparse-0.1.5.post9/readsparse.egg-info/
+-rw-r--r--   0 david     (1000) david     (1000)      245 2023-07-18 21:17:27.000000 readsparse-0.1.5.post9/readsparse.egg-info/PKG-INFO
+-rw-r--r--   0 david     (1000) david     (1000)      480 2023-07-18 21:17:27.000000 readsparse-0.1.5.post9/readsparse.egg-info/SOURCES.txt
+-rw-r--r--   0 david     (1000) david     (1000)        1 2023-07-18 21:17:27.000000 readsparse-0.1.5.post9/readsparse.egg-info/dependency_links.txt
+-rw-r--r--   0 david     (1000) david     (1000)       11 2023-07-18 21:17:27.000000 readsparse-0.1.5.post9/readsparse.egg-info/top_level.txt
+-rw-r--r--   0 david     (1000) david     (1000)       38 2023-07-18 21:17:27.564504 readsparse-0.1.5.post9/setup.cfg
+-rw-r--r--   0 david     (1000) david     (1000)     9734 2023-07-18 21:15:25.000000 readsparse-0.1.5.post9/setup.py
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-07-18 21:17:27.564504 readsparse-0.1.5.post9/src/
+-rw-r--r--   0 david     (1000) david     (1000)     5594 2021-07-25 03:01:47.000000 readsparse-0.1.5.post9/src/python_streams.hpp
+-rw-r--r--   0 david     (1000) david     (1000)    89722 2021-06-25 15:11:19.000000 readsparse-0.1.5.post9/src/reader.cpp
+-rw-r--r--   0 david     (1000) david     (1000)    58520 2022-01-16 21:05:53.000000 readsparse-0.1.5.post9/src/reader.hpp
+-rw-r--r--   0 david     (1000) david     (1000)    15446 2021-06-25 15:12:25.000000 readsparse-0.1.5.post9/src/readsparse.hpp
+-rw-r--r--   0 david     (1000) david     (1000)    95786 2021-06-25 15:11:19.000000 readsparse-0.1.5.post9/src/readsparse_detemplated.hpp
+-rw-r--r--   0 david     (1000) david     (1000)    10285 2022-09-11 18:48:32.000000 readsparse-0.1.5.post9/src/readsparse_internal.hpp
+-rw-r--r--   0 david     (1000) david     (1000)     7226 2021-08-25 00:18:42.000000 readsparse-0.1.5.post9/src/utils.hpp
+-rw-r--r--   0 david     (1000) david     (1000)    71373 2021-06-25 15:11:19.000000 readsparse-0.1.5.post9/src/writer.cpp
+-rw-r--r--   0 david     (1000) david     (1000)    37907 2021-07-14 01:23:59.000000 readsparse-0.1.5.post9/src/writer.hpp
```

### Comparing `readsparse-0.1.5.post8/LICENSE` & `readsparse-0.1.5.post9/LICENSE`

 * *Files identical despite different names*

### Comparing `readsparse-0.1.5.post8/readsparse/__init__.py` & `readsparse-0.1.5.post9/readsparse/__init__.py`

 * *Files identical despite different names*

### Comparing `readsparse-0.1.5.post8/readsparse/cpp_interface.pxi` & `readsparse-0.1.5.post9/readsparse/cpp_interface.pxi`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,15 @@
         size_large &nclasses,
         const size_t limit_nrows,
         const bool_t ignore_zero_valued,
         const bool_t sort_indices,
         const bool_t text_is_base1,
         const bool_t assume_no_qid,
         const bool_t assume_trailing_ws
-    ) nogil except +
+    ) except + nogil
 
     bool_t read_multi_label_template[int_t_, real_t_](
         FILE *input_file,
         vector[int_t_] &indptr,
         vector[int_t_] &indices,
         vector[real_t_] &values,
         vector[int_t_] &indptr_lab,
@@ -103,15 +103,15 @@
         size_large &nclasses,
         const size_t limit_nrows,
         const bool_t ignore_zero_valued,
         const bool_t sort_indices,
         const bool_t text_is_base1,
         const bool_t assume_no_qid,
         const bool_t assume_trailing_ws
-    ) nogil except +
+    ) except + nogil
 
 cdef extern from "writer.hpp":
 
     bool_t write_single_label_template[int_t_, real_t_, label_t_](
         FILE *output_file,
         int_t_ *indptr,
         int_t_ *indices,
@@ -125,15 +125,15 @@
         const size_large ncols,
         const size_large nclasses,
         const bool_t ignore_zero_valued,
         const bool_t sort_indices,
         const bool_t text_is_base1,
         const bool_t add_header,
         const int decimal_places
-    ) nogil except +
+    ) except + nogil
 
     bool_t write_multi_label_template[int_t_, real_t_](
         FILE *output_file,
         int_t_ *indptr,
         int_t_ *indices,
         real_t_ *values,
         int_t_ *indptr_lab,
@@ -145,15 +145,15 @@
         const size_large ncols,
         const size_large nclasses,
         const bool_t ignore_zero_valued,
         const bool_t sort_indices,
         const bool_t text_is_base1,
         const bool_t add_header,
         const int decimal_places
-    ) nogil except +
+    ) except + nogil
 
 
 cdef extern from "python_streams.hpp":
     bool_t read_multi_label_str[int_t_, real_t_](
         string &input_str,
         vector[int_t_] &indptr,
         vector[int_t_] &indices,
@@ -166,15 +166,15 @@
         size_large &nclasses,
         const size_t limit_nrows,
         const bool_t ignore_zero_valued,
         const bool_t sort_indices,
         const bool_t text_is_base1,
         const bool_t assume_no_qid,
         const bool_t assume_trailing_ws
-    ) nogil except +
+    ) except + nogil
 
     string write_multi_label_str[int_t_, real_t_](
         int_t_ *indptr,
         int_t_ *indices,
         real_t_ *values,
         int_t_ *indptr_lab,
         int_t_ *indices_lab,
@@ -185,15 +185,15 @@
         const size_large ncols,
         const size_large nclasses,
         const bool_t ignore_zero_valued,
         const bool_t sort_indices,
         const bool_t text_is_base1,
         const bool_t add_header,
         const int decimal_places
-    ) nogil except +
+    ) except + nogil
 
     bool_t read_single_label_str[int_t_, real_t_, label_t_](
         string &input_str,
         vector[int_t_] &indptr,
         vector[int_t_] &indices,
         vector[real_t_] &values,
         vector[label_t_] &labels,
@@ -203,15 +203,15 @@
         size_large &nclasses,
         const size_t limit_nrows,
         const bool_t ignore_zero_valued,
         const bool_t sort_indices,
         const bool_t text_is_base1,
         const bool_t assume_no_qid,
         const bool_t assume_trailing_ws
-    ) nogil except +
+    ) except + nogil
 
     string write_single_label_str[int_t_, real_t_, label_t_](
         int_t_ *indptr,
         int_t_ *indices,
         real_t_ *values,
         label_t_ *labels,
         int_t_ *qid,
@@ -222,15 +222,15 @@
         const size_large ncols,
         const size_large nclasses,
         const bool_t ignore_zero_valued,
         const bool_t sort_indices,
         const bool_t text_is_base1,
         const bool_t add_header,
         const int decimal_places
-    ) nogil except +
+    ) except + nogil
 
 cdef extern from "utils.hpp":
     void sort_sparse_indices_known_ncol[int_t_, real_t_](
         int_t_ *indptr,
         int_t_ *indices,
         real_t_ *values,
         size_t nrows, size_t ncols
```

### Comparing `readsparse-0.1.5.post8/setup.py` & `readsparse-0.1.5.post9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -204,15 +204,15 @@
     platform_is_32 = True
 
 is_windows = sys.platform[:3] == "win"
 
 setup(
     name  = "readsparse",
     packages = ["readsparse"],
-    version = '0.1.5-8',
+    version = '0.1.5-9',
     description = 'Read and Write Sparse Matrices in Text Format',
     author = 'David Cortes',
     url = 'https://github.com/david-cortes/readsparse',
     keywords = ['sparse', 'svmlight', 'libsvm'],
     cmdclass = {'build_ext': build_ext_subclass},
     ext_modules = [Extension(
                                 "readsparse._cpp_interface",
@@ -222,12 +222,13 @@
                                          "src/reader.cpp", "src/writer.cpp"
                                          ],
                                 include_dirs=[np.get_include(), "./src", "./readsparse"],
                                 language="c++",
                                 install_requires=["numpy", "cython", "scipy"],
                                 define_macros=[
                                     ("_FOR_PYTHON", None),
-                                    ("NDEBUG", None)
+                                    ("NDEBUG", None),
+                                    ("NPY_NO_DEPRECATED_API", "NPY_1_7_API_VERSION")
                                 ],
                                 compiler_directives={'language_level' : "3"}
                             )]
     )
```

### Comparing `readsparse-0.1.5.post8/src/python_streams.hpp` & `readsparse-0.1.5.post9/src/python_streams.hpp`

 * *Files identical despite different names*

### Comparing `readsparse-0.1.5.post8/src/reader.cpp` & `readsparse-0.1.5.post9/src/reader.cpp`

 * *Files identical despite different names*

### Comparing `readsparse-0.1.5.post8/src/reader.hpp` & `readsparse-0.1.5.post9/src/reader.hpp`

 * *Files identical despite different names*

### Comparing `readsparse-0.1.5.post8/src/readsparse.hpp` & `readsparse-0.1.5.post9/src/readsparse.hpp`

 * *Files identical despite different names*

### Comparing `readsparse-0.1.5.post8/src/readsparse_detemplated.hpp` & `readsparse-0.1.5.post9/src/readsparse_detemplated.hpp`

 * *Files identical despite different names*

### Comparing `readsparse-0.1.5.post8/src/readsparse_internal.hpp` & `readsparse-0.1.5.post9/src/readsparse_internal.hpp`

 * *Files identical despite different names*

### Comparing `readsparse-0.1.5.post8/src/utils.hpp` & `readsparse-0.1.5.post9/src/utils.hpp`

 * *Files identical despite different names*

### Comparing `readsparse-0.1.5.post8/src/writer.cpp` & `readsparse-0.1.5.post9/src/writer.cpp`

 * *Files identical despite different names*

### Comparing `readsparse-0.1.5.post8/src/writer.hpp` & `readsparse-0.1.5.post9/src/writer.hpp`

 * *Files identical despite different names*

