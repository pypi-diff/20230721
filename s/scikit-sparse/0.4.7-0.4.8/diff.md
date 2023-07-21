# Comparing `tmp/scikit-sparse-0.4.7.tar.gz` & `tmp/scikit-sparse-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/scikit-sparse-0.4.7.tar", last modified: Sat Nov  5 01:45:55 2022, max compression
+gzip compressed data, was "dist/scikit-sparse-0.4.8.tar", last modified: Sun Nov 27 16:55:32 2022, max compression
```

## Comparing `scikit-sparse-0.4.7.tar` & `scikit-sparse-0.4.8.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-05 01:45:55.000000 scikit-sparse-0.4.7/
--rw-r--r--   0 runner    (1001) docker     (121)     1385 2022-11-05 01:45:40.000000 scikit-sparse-0.4.7/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)      170 2022-11-05 01:45:40.000000 scikit-sparse-0.4.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1306 2022-11-05 01:45:55.000000 scikit-sparse-0.4.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5387 2022-11-05 01:45:40.000000 scikit-sparse-0.4.7/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      680 2022-11-05 01:45:40.000000 scikit-sparse-0.4.7/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-05 01:45:55.000000 scikit-sparse-0.4.7/scikit_sparse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1306 2022-11-05 01:45:55.000000 scikit-sparse-0.4.7/scikit_sparse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      647 2022-11-05 01:45:55.000000 scikit-sparse-0.4.7/scikit_sparse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-05 01:45:55.000000 scikit-sparse-0.4.7/scikit_sparse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-11-05 01:45:55.000000 scikit-sparse-0.4.7/scikit_sparse.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-11-05 01:45:55.000000 scikit-sparse-0.4.7/scikit_sparse.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-05 01:45:55.000000 scikit-sparse-0.4.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     3284 2022-11-05 01:45:40.000000 scikit-sparse-0.4.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-05 01:45:55.000000 scikit-sparse-0.4.7/sksparse/
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-11-05 01:45:40.000000 scikit-sparse-0.4.7/sksparse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    48134 2022-11-05 01:45:40.000000 scikit-sparse-0.4.7/sksparse/cholmod.pyx
--rw-r--r--   0 runner    (1001) docker     (121)      633 2022-11-05 01:45:40.000000 scikit-sparse-0.4.7/sksparse/cholmod_backward_compatible.h
--rw-r--r--   0 runner    (1001) docker     (121)    11388 2022-11-05 01:45:40.000000 scikit-sparse-0.4.7/sksparse/test_cholmod.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-05 01:45:55.000000 scikit-sparse-0.4.7/sksparse/test_data/
--rw-r--r--   0 runner    (1001) docker     (121)    27031 2022-11-05 01:45:40.000000 scikit-sparse-0.4.7/sksparse/test_data/illc1033.mtx.gz
--rw-r--r--   0 runner    (1001) docker     (121)     6644 2022-11-05 01:45:40.000000 scikit-sparse-0.4.7/sksparse/test_data/illc1033_rhs1.mtx.gz
--rw-r--r--   0 runner    (1001) docker     (121)    51499 2022-11-05 01:45:40.000000 scikit-sparse-0.4.7/sksparse/test_data/illc1850.mtx.gz
--rw-r--r--   0 runner    (1001) docker     (121)    11906 2022-11-05 01:45:40.000000 scikit-sparse-0.4.7/sksparse/test_data/illc1850_rhs1.mtx.gz
--rw-r--r--   0 runner    (1001) docker     (121)    28620 2022-11-05 01:45:40.000000 scikit-sparse-0.4.7/sksparse/test_data/well1033.mtx.gz
--rw-r--r--   0 runner    (1001) docker     (121)     6645 2022-11-05 01:45:40.000000 scikit-sparse-0.4.7/sksparse/test_data/well1033_rhs1.mtx.gz
--rw-r--r--   0 runner    (1001) docker     (121)    53817 2022-11-05 01:45:40.000000 scikit-sparse-0.4.7/sksparse/test_data/well1850.mtx.gz
--rw-r--r--   0 runner    (1001) docker     (121)    11906 2022-11-05 01:45:40.000000 scikit-sparse-0.4.7/sksparse/test_data/well1850_rhs1.mtx.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-27 16:55:32.000000 scikit-sparse-0.4.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2022-11-27 16:55:16.000000 scikit-sparse-0.4.8/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2022-11-27 16:55:16.000000 scikit-sparse-0.4.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2022-11-27 16:55:32.000000 scikit-sparse-0.4.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5387 2022-11-27 16:55:16.000000 scikit-sparse-0.4.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2022-11-27 16:55:16.000000 scikit-sparse-0.4.8/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-27 16:55:31.000000 scikit-sparse-0.4.8/scikit_sparse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2022-11-27 16:55:31.000000 scikit-sparse-0.4.8/scikit_sparse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2022-11-27 16:55:31.000000 scikit-sparse-0.4.8/scikit_sparse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-11-27 16:55:31.000000 scikit-sparse-0.4.8/scikit_sparse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2022-11-27 16:55:31.000000 scikit-sparse-0.4.8/scikit_sparse.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2022-11-27 16:55:31.000000 scikit-sparse-0.4.8/scikit_sparse.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2022-11-27 16:55:32.000000 scikit-sparse-0.4.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3284 2022-11-27 16:55:16.000000 scikit-sparse-0.4.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-27 16:55:32.000000 scikit-sparse-0.4.8/sksparse/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2022-11-27 16:55:16.000000 scikit-sparse-0.4.8/sksparse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48134 2022-11-27 16:55:16.000000 scikit-sparse-0.4.8/sksparse/cholmod.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2022-11-27 16:55:16.000000 scikit-sparse-0.4.8/sksparse/cholmod_backward_compatible.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11388 2022-11-27 16:55:16.000000 scikit-sparse-0.4.8/sksparse/test_cholmod.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-27 16:55:32.000000 scikit-sparse-0.4.8/sksparse/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    27031 2022-11-27 16:55:16.000000 scikit-sparse-0.4.8/sksparse/test_data/illc1033.mtx.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     6644 2022-11-27 16:55:16.000000 scikit-sparse-0.4.8/sksparse/test_data/illc1033_rhs1.mtx.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    51499 2022-11-27 16:55:16.000000 scikit-sparse-0.4.8/sksparse/test_data/illc1850.mtx.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    11906 2022-11-27 16:55:16.000000 scikit-sparse-0.4.8/sksparse/test_data/illc1850_rhs1.mtx.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    28620 2022-11-27 16:55:16.000000 scikit-sparse-0.4.8/sksparse/test_data/well1033.mtx.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     6645 2022-11-27 16:55:16.000000 scikit-sparse-0.4.8/sksparse/test_data/well1033_rhs1.mtx.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    53817 2022-11-27 16:55:16.000000 scikit-sparse-0.4.8/sksparse/test_data/well1850.mtx.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    11906 2022-11-27 16:55:16.000000 scikit-sparse-0.4.8/sksparse/test_data/well1850_rhs1.mtx.gz
```

### Comparing `scikit-sparse-0.4.7/LICENSE.txt` & `scikit-sparse-0.4.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `scikit-sparse-0.4.7/PKG-INFO` & `scikit-sparse-0.4.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scikit-sparse
-Version: 0.4.7
+Version: 0.4.8
 Summary: Scikit sparse matrix package
 Home-page: https://github.com/scikit-sparse/scikit-sparse
 Maintainer: Justin Ellis
 Maintainer-email: justin.ellis18@gmail.com
 License: BSD
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `scikit-sparse-0.4.7/README.md` & `scikit-sparse-0.4.8/README.md`

 * *Files identical despite different names*

### Comparing `scikit-sparse-0.4.7/pyproject.toml` & `scikit-sparse-0.4.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `scikit-sparse-0.4.7/scikit_sparse.egg-info/PKG-INFO` & `scikit-sparse-0.4.8/scikit_sparse.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scikit-sparse
-Version: 0.4.7
+Version: 0.4.8
 Summary: Scikit sparse matrix package
 Home-page: https://github.com/scikit-sparse/scikit-sparse
 Maintainer: Justin Ellis
 Maintainer-email: justin.ellis18@gmail.com
 License: BSD
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `scikit-sparse-0.4.7/scikit_sparse.egg-info/SOURCES.txt` & `scikit-sparse-0.4.8/scikit_sparse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scikit-sparse-0.4.7/setup.py` & `scikit-sparse-0.4.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
     install_requires=["numpy>=1.13.3", "scipy>=0.19"],
     python_requires=">=3.6, <3.11",
     packages=find_packages(),
     package_data={
         "": ["test_data/*.mtx.gz"],
     },
     name=DISTNAME,
-    version="0.4.7",  # remember to update __init__.py
+    version="0.4.8",  # remember to update __init__.py
     maintainer=MAINTAINER,
     maintainer_email=MAINTAINER_EMAIL,
     description=DESCRIPTION,
     license=LICENSE,
     url=URL,
     long_description=LONG_DESCRIPTION,
     classifiers=[
```

### Comparing `scikit-sparse-0.4.7/sksparse/cholmod.pyx` & `scikit-sparse-0.4.8/sksparse/cholmod.pyx`

 * *Files identical despite different names*

### Comparing `scikit-sparse-0.4.7/sksparse/cholmod_backward_compatible.h` & `scikit-sparse-0.4.8/sksparse/cholmod_backward_compatible.h`

 * *Files identical despite different names*

### Comparing `scikit-sparse-0.4.7/sksparse/test_cholmod.py` & `scikit-sparse-0.4.8/sksparse/test_cholmod.py`

 * *Files identical despite different names*

### Comparing `scikit-sparse-0.4.7/sksparse/test_data/illc1033.mtx.gz` & `scikit-sparse-0.4.8/sksparse/test_data/illc1033.mtx.gz`

 * *Files identical despite different names*

### Comparing `scikit-sparse-0.4.7/sksparse/test_data/illc1033_rhs1.mtx.gz` & `scikit-sparse-0.4.8/sksparse/test_data/illc1033_rhs1.mtx.gz`

 * *Files identical despite different names*

### Comparing `scikit-sparse-0.4.7/sksparse/test_data/illc1850.mtx.gz` & `scikit-sparse-0.4.8/sksparse/test_data/illc1850.mtx.gz`

 * *Files identical despite different names*

### Comparing `scikit-sparse-0.4.7/sksparse/test_data/illc1850_rhs1.mtx.gz` & `scikit-sparse-0.4.8/sksparse/test_data/illc1850_rhs1.mtx.gz`

 * *Files identical despite different names*

### Comparing `scikit-sparse-0.4.7/sksparse/test_data/well1033.mtx.gz` & `scikit-sparse-0.4.8/sksparse/test_data/well1033.mtx.gz`

 * *Files identical despite different names*

### Comparing `scikit-sparse-0.4.7/sksparse/test_data/well1033_rhs1.mtx.gz` & `scikit-sparse-0.4.8/sksparse/test_data/well1033_rhs1.mtx.gz`

 * *Files identical despite different names*

### Comparing `scikit-sparse-0.4.7/sksparse/test_data/well1850.mtx.gz` & `scikit-sparse-0.4.8/sksparse/test_data/well1850.mtx.gz`

 * *Files identical despite different names*

### Comparing `scikit-sparse-0.4.7/sksparse/test_data/well1850_rhs1.mtx.gz` & `scikit-sparse-0.4.8/sksparse/test_data/well1850_rhs1.mtx.gz`

 * *Files identical despite different names*

