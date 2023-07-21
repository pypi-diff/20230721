# Comparing `tmp/pytorch-perf-0.0.2.tar.gz` & `tmp/pytorch-perf-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytorch-perf-0.0.2.tar", last modified: Tue Jul 18 05:13:36 2023, max compression
+gzip compressed data, was "pytorch-perf-0.0.3.tar", last modified: Fri Jul 21 20:32:24 2023, max compression
```

## Comparing `pytorch-perf-0.0.2.tar` & `pytorch-perf-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 yren      (1000) yren      (1000)        0 2023-07-18 05:13:36.813395 pytorch-perf-0.0.2/
--rw-rw-r--   0 yren      (1000) yren      (1000)     1488 2023-07-02 21:44:16.000000 pytorch-perf-0.0.2/LICENSE
--rw-rw-r--   0 yren      (1000) yren      (1000)     1764 2023-07-18 05:13:36.813395 pytorch-perf-0.0.2/PKG-INFO
--rw-r--r--   0 yren      (1000) yren      (1000)     1134 2023-07-18 04:45:11.000000 pytorch-perf-0.0.2/README.md
-drwxrwxr-x   0 yren      (1000) yren      (1000)        0 2023-07-18 05:13:36.809395 pytorch-perf-0.0.2/pytorch_perf.egg-info/
--rw-rw-r--   0 yren      (1000) yren      (1000)     1764 2023-07-18 05:13:36.000000 pytorch-perf-0.0.2/pytorch_perf.egg-info/PKG-INFO
--rw-rw-r--   0 yren      (1000) yren      (1000)      347 2023-07-18 05:13:36.000000 pytorch-perf-0.0.2/pytorch_perf.egg-info/SOURCES.txt
--rw-rw-r--   0 yren      (1000) yren      (1000)        1 2023-07-18 05:13:36.000000 pytorch-perf-0.0.2/pytorch_perf.egg-info/dependency_links.txt
--rw-rw-r--   0 yren      (1000) yren      (1000)        6 2023-07-18 05:13:36.000000 pytorch-perf-0.0.2/pytorch_perf.egg-info/requires.txt
--rw-rw-r--   0 yren      (1000) yren      (1000)       10 2023-07-18 05:13:36.000000 pytorch-perf-0.0.2/pytorch_perf.egg-info/top_level.txt
--rw-rw-r--   0 yren      (1000) yren      (1000)       38 2023-07-18 05:13:36.813395 pytorch-perf-0.0.2/setup.cfg
--rw-r--r--   0 yren      (1000) yren      (1000)     1565 2023-07-18 04:48:19.000000 pytorch-perf-0.0.2/setup.py
-drwxrwxr-x   0 yren      (1000) yren      (1000)        0 2023-07-18 05:13:36.809395 pytorch-perf-0.0.2/tests/
--rw-r--r--   0 yren      (1000) yren      (1000)      810 2023-07-18 02:40:40.000000 pytorch-perf-0.0.2/tests/test_basics.py
--rw-r--r--   0 yren      (1000) yren      (1000)      129 2023-07-18 04:27:37.000000 pytorch-perf-0.0.2/tests/test_info.py
--rw-r--r--   0 yren      (1000) yren      (1000)     1137 2023-07-18 04:25:12.000000 pytorch-perf-0.0.2/tests/test_recipe.py
-drwxrwxr-x   0 yren      (1000) yren      (1000)        0 2023-07-18 05:13:36.813395 pytorch-perf-0.0.2/torchperf/
--rw-r--r--   0 yren      (1000) yren      (1000)      160 2023-07-18 04:46:24.000000 pytorch-perf-0.0.2/torchperf/__init__.py
--rw-r--r--   0 yren      (1000) yren      (1000)     1225 2023-07-18 02:30:25.000000 pytorch-perf-0.0.2/torchperf/info.py
--rw-rw-r--   0 yren      (1000) yren      (1000)     1188 2023-07-18 02:39:48.000000 pytorch-perf-0.0.2/torchperf/measure.py
--rw-r--r--   0 yren      (1000) yren      (1000)     2589 2023-07-18 04:30:41.000000 pytorch-perf-0.0.2/torchperf/recipe.py
+drwxrwxr-x   0 yren      (1000) yren      (1000)        0 2023-07-21 20:32:24.702083 pytorch-perf-0.0.3/
+-rw-rw-r--   0 yren      (1000) yren      (1000)     1488 2023-07-02 21:44:16.000000 pytorch-perf-0.0.3/LICENSE
+-rw-rw-r--   0 yren      (1000) yren      (1000)     1864 2023-07-21 20:32:24.702083 pytorch-perf-0.0.3/PKG-INFO
+-rw-r--r--   0 yren      (1000) yren      (1000)     1134 2023-07-18 04:45:11.000000 pytorch-perf-0.0.3/README.md
+drwxrwxr-x   0 yren      (1000) yren      (1000)        0 2023-07-21 20:32:24.702083 pytorch-perf-0.0.3/pytorch_perf.egg-info/
+-rw-rw-r--   0 yren      (1000) yren      (1000)     1864 2023-07-21 20:32:24.000000 pytorch-perf-0.0.3/pytorch_perf.egg-info/PKG-INFO
+-rw-rw-r--   0 yren      (1000) yren      (1000)      347 2023-07-21 20:32:24.000000 pytorch-perf-0.0.3/pytorch_perf.egg-info/SOURCES.txt
+-rw-rw-r--   0 yren      (1000) yren      (1000)        1 2023-07-21 20:32:24.000000 pytorch-perf-0.0.3/pytorch_perf.egg-info/dependency_links.txt
+-rw-rw-r--   0 yren      (1000) yren      (1000)        6 2023-07-21 20:32:24.000000 pytorch-perf-0.0.3/pytorch_perf.egg-info/requires.txt
+-rw-rw-r--   0 yren      (1000) yren      (1000)       10 2023-07-21 20:32:24.000000 pytorch-perf-0.0.3/pytorch_perf.egg-info/top_level.txt
+-rw-rw-r--   0 yren      (1000) yren      (1000)       38 2023-07-21 20:32:24.702083 pytorch-perf-0.0.3/setup.cfg
+-rw-r--r--   0 yren      (1000) yren      (1000)     1671 2023-07-21 20:23:55.000000 pytorch-perf-0.0.3/setup.py
+drwxrwxr-x   0 yren      (1000) yren      (1000)        0 2023-07-21 20:32:24.702083 pytorch-perf-0.0.3/tests/
+-rw-r--r--   0 yren      (1000) yren      (1000)      810 2023-07-18 02:40:40.000000 pytorch-perf-0.0.3/tests/test_basics.py
+-rw-r--r--   0 yren      (1000) yren      (1000)      129 2023-07-18 04:27:37.000000 pytorch-perf-0.0.3/tests/test_info.py
+-rw-r--r--   0 yren      (1000) yren      (1000)     1137 2023-07-18 04:25:12.000000 pytorch-perf-0.0.3/tests/test_recipe.py
+drwxrwxr-x   0 yren      (1000) yren      (1000)        0 2023-07-21 20:32:24.702083 pytorch-perf-0.0.3/torchperf/
+-rw-r--r--   0 yren      (1000) yren      (1000)      160 2023-07-21 20:30:33.000000 pytorch-perf-0.0.3/torchperf/__init__.py
+-rw-r--r--   0 yren      (1000) yren      (1000)     1225 2023-07-18 02:30:25.000000 pytorch-perf-0.0.3/torchperf/info.py
+-rw-rw-r--   0 yren      (1000) yren      (1000)     1188 2023-07-18 02:39:48.000000 pytorch-perf-0.0.3/torchperf/measure.py
+-rw-r--r--   0 yren      (1000) yren      (1000)     2589 2023-07-18 04:30:41.000000 pytorch-perf-0.0.3/torchperf/recipe.py
```

### Comparing `pytorch-perf-0.0.2/LICENSE` & `pytorch-perf-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pytorch-perf-0.0.2/PKG-INFO` & `pytorch-perf-0.0.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: pytorch-perf
-Version: 0.0.2
+Version: 0.0.3
 Summary: A pytorch perf decorator
 Home-page: https://github.com/yhren/torchperf
 Author: Yihui Ren
 Author-email: yren@bnl.gov
 License: BSD-3
 Keywords: decorator cuda performance perf pytorch
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: POSIX :: Linux
-Requires-Python: >=3.9
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PyTorch Perf
 
 <p align="left">
 <a href="https://opensource.org/licenses/BSD-3-Clause"><img alt="License" src="https://img.shields.io/badge/License-BSD_3--Clause-blue.svg"></a>
```

### Comparing `pytorch-perf-0.0.2/README.md` & `pytorch-perf-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pytorch-perf-0.0.2/pytorch_perf.egg-info/PKG-INFO` & `pytorch-perf-0.0.3/pytorch_perf.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: pytorch-perf
-Version: 0.0.2
+Version: 0.0.3
 Summary: A pytorch perf decorator
 Home-page: https://github.com/yhren/torchperf
 Author: Yihui Ren
 Author-email: yren@bnl.gov
 License: BSD-3
 Keywords: decorator cuda performance perf pytorch
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: POSIX :: Linux
-Requires-Python: >=3.9
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PyTorch Perf
 
 <p align="left">
 <a href="https://opensource.org/licenses/BSD-3-Clause"><img alt="License" src="https://img.shields.io/badge/License-BSD_3--Clause-blue.svg"></a>
```

### Comparing `pytorch-perf-0.0.2/setup.py` & `pytorch-perf-0.0.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,18 +24,20 @@
         license="BSD-3",
         long_description=LONG_DESC,
         long_description_content_type="text/markdown",
         url="https://github.com/yhren/torchperf",
         keywords="decorator cuda performance perf pytorch",
         packages=find_namespace_packages(include=["torchperf", "torchperf.*"]),
         include_package_data=True,
-        python_requires=">=3.9",
+        python_requires=">=3.7",
         classifiers=[
             "License :: OSI Approved :: BSD License",
             "Development Status :: 2 - Pre-Alpha",
+            "Programming Language :: Python :: 3.7",
+            "Programming Language :: Python :: 3.8",
             "Programming Language :: Python :: 3.9",
             "Programming Language :: Python :: 3.10",
             "Programming Language :: Python :: 3.11",
             "Operating System :: POSIX :: Linux",
         ],
         install_requires=["numpy"],
         # Install development dependencies with
```

### Comparing `pytorch-perf-0.0.2/tests/test_basics.py` & `pytorch-perf-0.0.3/tests/test_basics.py`

 * *Files identical despite different names*

### Comparing `pytorch-perf-0.0.2/tests/test_recipe.py` & `pytorch-perf-0.0.3/tests/test_recipe.py`

 * *Files identical despite different names*

### Comparing `pytorch-perf-0.0.2/torchperf/info.py` & `pytorch-perf-0.0.3/torchperf/info.py`

 * *Files identical despite different names*

### Comparing `pytorch-perf-0.0.2/torchperf/measure.py` & `pytorch-perf-0.0.3/torchperf/measure.py`

 * *Files identical despite different names*

### Comparing `pytorch-perf-0.0.2/torchperf/recipe.py` & `pytorch-perf-0.0.3/torchperf/recipe.py`

 * *Files identical despite different names*

