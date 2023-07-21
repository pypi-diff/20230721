# Comparing `tmp/pso2keras-0.1.4.tar.gz` & `tmp/pso2keras-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pso2keras-0.1.4.tar", last modified: Fri Jul 21 06:21:44 2023, max compression
+gzip compressed data, was "pso2keras-0.1.5.tar", last modified: Fri Jul 21 06:26:52 2023, max compression
```

## Comparing `pso2keras-0.1.4.tar` & `pso2keras-0.1.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 06:21:44.711463 pso2keras-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     8466 2023-07-21 06:21:44.711463 pso2keras-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8127 2023-07-21 06:20:38.000000 pso2keras-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 06:21:44.707463 pso2keras-0.1.4/pso/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-21 06:20:38.000000 pso2keras-0.1.4/pso/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21985 2023-07-21 06:20:38.000000 pso2keras-0.1.4/pso/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9757 2023-07-21 06:20:38.000000 pso2keras-0.1.4/pso/particle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 06:21:44.711463 pso2keras-0.1.4/pso2keras.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8466 2023-07-21 06:21:44.000000 pso2keras-0.1.4/pso2keras.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-21 06:21:44.000000 pso2keras-0.1.4/pso2keras.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 06:21:44.000000 pso2keras-0.1.4/pso2keras.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 06:21:44.000000 pso2keras-0.1.4/pso2keras.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-21 06:21:44.000000 pso2keras-0.1.4/pso2keras.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-21 06:21:44.000000 pso2keras-0.1.4/pso2keras.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 06:21:44.711463 pso2keras-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-07-21 06:20:38.000000 pso2keras-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 06:26:52.801769 pso2keras-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     8466 2023-07-21 06:26:52.801769 pso2keras-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8127 2023-07-21 06:25:49.000000 pso2keras-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 06:26:52.801769 pso2keras-0.1.5/pso/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-21 06:25:49.000000 pso2keras-0.1.5/pso/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21985 2023-07-21 06:25:49.000000 pso2keras-0.1.5/pso/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9757 2023-07-21 06:25:49.000000 pso2keras-0.1.5/pso/particle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 06:26:52.801769 pso2keras-0.1.5/pso2keras.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8466 2023-07-21 06:26:52.000000 pso2keras-0.1.5/pso2keras.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-21 06:26:52.000000 pso2keras-0.1.5/pso2keras.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 06:26:52.000000 pso2keras-0.1.5/pso2keras.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 06:26:52.000000 pso2keras-0.1.5/pso2keras.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-21 06:26:52.000000 pso2keras-0.1.5/pso2keras.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-21 06:26:52.000000 pso2keras-0.1.5/pso2keras.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 06:26:52.801769 pso2keras-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-07-21 06:25:49.000000 pso2keras-0.1.5/setup.py
```

### Comparing `pso2keras-0.1.4/PKG-INFO` & `pso2keras-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: pso2keras
-Version: 0.1.4
+Version: 0.1.5
 Summary: Particle Swarm Optimization to tensorflow package
 Home-page: https://github.com/jung-geun/PSO
 Author: pieroot
 Author-email: jgbong0306@gmail.com
 License: UNKNOWN
 Keywords: pso,tensorflow,keras
 Platform: UNKNOWN
-Requires-Python: ==3.9
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 [![Python Package Index publish](https://github.com/jung-geun/PSO/actions/workflows/pypi.yml/badge.svg?event=push)](https://github.com/jung-geun/PSO/actions/workflows/pypi.yml)
 
 # PSO 알고리즘 구현 및 새로운 시도
 
 pso 알고리즘을 사용하여 새로운 학습 방법을 찾는중 입니다
```

### Comparing `pso2keras-0.1.4/README.md` & `pso2keras-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `pso2keras-0.1.4/pso/optimizer.py` & `pso2keras-0.1.5/pso/optimizer.py`

 * *Files identical despite different names*

### Comparing `pso2keras-0.1.4/pso/particle.py` & `pso2keras-0.1.5/pso/particle.py`

 * *Files identical despite different names*

### Comparing `pso2keras-0.1.4/pso2keras.egg-info/PKG-INFO` & `pso2keras-0.1.5/pso2keras.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: pso2keras
-Version: 0.1.4
+Version: 0.1.5
 Summary: Particle Swarm Optimization to tensorflow package
 Home-page: https://github.com/jung-geun/PSO
 Author: pieroot
 Author-email: jgbong0306@gmail.com
 License: UNKNOWN
 Keywords: pso,tensorflow,keras
 Platform: UNKNOWN
-Requires-Python: ==3.9
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 [![Python Package Index publish](https://github.com/jung-geun/PSO/actions/workflows/pypi.yml/badge.svg?event=push)](https://github.com/jung-geun/PSO/actions/workflows/pypi.yml)
 
 # PSO 알고리즘 구현 및 새로운 시도
 
 pso 알고리즘을 사용하여 새로운 학습 방법을 찾는중 입니다
```

### Comparing `pso2keras-0.1.4/setup.py` & `pso2keras-0.1.5/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -15,13 +15,13 @@
         "tqdm",
         "numpy",
         "pandas",
         "ipython",
     ],
     packages=find_packages(exclude=[]),
     keywords=["pso", "tensorflow", "keras"],
-    python_requires="==3.9",
+    python_requires=">=3.8",
     package_data={},
     zip_safe=False,
     long_description=open("README.md", encoding="UTF8").read(),
     long_description_content_type="text/markdown",
 )
```

