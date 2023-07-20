# Comparing `tmp/deepcellpredictor-0.9.2.tar.gz` & `tmp/deepcellpredictor-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepcellpredictor-0.9.2.tar", last modified: Thu Jul 20 22:41:19 2023, max compression
+gzip compressed data, was "deepcellpredictor-0.9.3.tar", last modified: Thu Jul 20 22:51:59 2023, max compression
```

## Comparing `deepcellpredictor-0.9.2.tar` & `deepcellpredictor-0.9.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 gaurav    (1001) gaurav    (1001)        0 2023-07-20 22:41:19.160624 deepcellpredictor-0.9.2/
-drwxrwxr-x   0 gaurav    (1001) gaurav    (1001)        0 2023-07-20 22:41:19.160624 deepcellpredictor-0.9.2/DCP/
--rw-rw-r--   0 gaurav    (1001) gaurav    (1001)     1245 2023-07-20 15:52:22.000000 deepcellpredictor-0.9.2/DCP/ModelPlanner.py
--rw-rw-r--   0 gaurav    (1001) gaurav    (1001)     8298 2023-07-20 22:39:47.000000 deepcellpredictor-0.9.2/DCP/VAEtorch.py
--rw-rw-r--   0 gaurav    (1001) gaurav    (1001)      474 2023-07-20 20:33:00.000000 deepcellpredictor-0.9.2/DCP/__init__.py
--rw-rw-r--   0 gaurav    (1001) gaurav    (1001)    11734 2023-07-20 22:35:17.000000 deepcellpredictor-0.9.2/DCP/deep_predictor.py
--rw-rw-r--   0 gaurav    (1001) gaurav    (1001)     4056 2023-07-20 15:52:22.000000 deepcellpredictor-0.9.2/DCP/flow.py
--rw-rw-r--   0 gaurav    (1001) gaurav    (1001)      679 2023-07-20 15:52:22.000000 deepcellpredictor-0.9.2/DCP/utils.py
--rw-rw-r--   0 gaurav    (1001) gaurav    (1001)     1063 2023-07-20 20:33:00.000000 deepcellpredictor-0.9.2/LICENSE
--rw-rw-r--   0 gaurav    (1001) gaurav    (1001)      444 2023-07-20 22:41:19.160624 deepcellpredictor-0.9.2/PKG-INFO
--rw-rw-r--   0 gaurav    (1001) gaurav    (1001)      182 2023-07-20 15:52:22.000000 deepcellpredictor-0.9.2/README.md
-drwxrwxr-x   0 gaurav    (1001) gaurav    (1001)        0 2023-07-20 22:41:19.160624 deepcellpredictor-0.9.2/deepcellpredictor.egg-info/
--rw-rw-r--   0 gaurav    (1001) gaurav    (1001)      444 2023-07-20 22:41:18.000000 deepcellpredictor-0.9.2/deepcellpredictor.egg-info/PKG-INFO
--rw-rw-r--   0 gaurav    (1001) gaurav    (1001)      329 2023-07-20 22:41:19.000000 deepcellpredictor-0.9.2/deepcellpredictor.egg-info/SOURCES.txt
--rw-rw-r--   0 gaurav    (1001) gaurav    (1001)        1 2023-07-20 22:41:18.000000 deepcellpredictor-0.9.2/deepcellpredictor.egg-info/dependency_links.txt
--rw-rw-r--   0 gaurav    (1001) gaurav    (1001)       84 2023-07-20 22:41:19.000000 deepcellpredictor-0.9.2/deepcellpredictor.egg-info/requires.txt
--rw-rw-r--   0 gaurav    (1001) gaurav    (1001)        4 2023-07-20 22:41:19.000000 deepcellpredictor-0.9.2/deepcellpredictor.egg-info/top_level.txt
--rw-rw-r--   0 gaurav    (1001) gaurav    (1001)       38 2023-07-20 22:41:19.160624 deepcellpredictor-0.9.2/setup.cfg
--rw-rw-r--   0 gaurav    (1001) gaurav    (1001)      792 2023-07-20 22:41:09.000000 deepcellpredictor-0.9.2/setup.py
+drwxrwxr-x   0 gaurav    (1001) gaurav    (1001)        0 2023-07-20 22:51:59.082783 deepcellpredictor-0.9.3/
+drwxrwxr-x   0 gaurav    (1001) gaurav    (1001)        0 2023-07-20 22:51:59.082783 deepcellpredictor-0.9.3/DCP/
+-rw-rw-r--   0 gaurav    (1001) gaurav    (1001)     1245 2023-07-20 15:52:22.000000 deepcellpredictor-0.9.3/DCP/ModelPlanner.py
+-rw-rw-r--   0 gaurav    (1001) gaurav    (1001)     8298 2023-07-20 22:39:47.000000 deepcellpredictor-0.9.3/DCP/VAEtorch.py
+-rw-rw-r--   0 gaurav    (1001) gaurav    (1001)      474 2023-07-20 20:33:00.000000 deepcellpredictor-0.9.3/DCP/__init__.py
+-rw-rw-r--   0 gaurav    (1001) gaurav    (1001)    11734 2023-07-20 22:35:17.000000 deepcellpredictor-0.9.3/DCP/deep_predictor.py
+-rw-rw-r--   0 gaurav    (1001) gaurav    (1001)     4056 2023-07-20 15:52:22.000000 deepcellpredictor-0.9.3/DCP/flow.py
+-rw-rw-r--   0 gaurav    (1001) gaurav    (1001)      679 2023-07-20 15:52:22.000000 deepcellpredictor-0.9.3/DCP/utils.py
+-rw-rw-r--   0 gaurav    (1001) gaurav    (1001)     1063 2023-07-20 20:33:00.000000 deepcellpredictor-0.9.3/LICENSE
+-rw-rw-r--   0 gaurav    (1001) gaurav    (1001)      444 2023-07-20 22:51:59.082783 deepcellpredictor-0.9.3/PKG-INFO
+-rw-rw-r--   0 gaurav    (1001) gaurav    (1001)      182 2023-07-20 15:52:22.000000 deepcellpredictor-0.9.3/README.md
+drwxrwxr-x   0 gaurav    (1001) gaurav    (1001)        0 2023-07-20 22:51:59.082783 deepcellpredictor-0.9.3/deepcellpredictor.egg-info/
+-rw-rw-r--   0 gaurav    (1001) gaurav    (1001)      444 2023-07-20 22:51:58.000000 deepcellpredictor-0.9.3/deepcellpredictor.egg-info/PKG-INFO
+-rw-rw-r--   0 gaurav    (1001) gaurav    (1001)      329 2023-07-20 22:51:59.000000 deepcellpredictor-0.9.3/deepcellpredictor.egg-info/SOURCES.txt
+-rw-rw-r--   0 gaurav    (1001) gaurav    (1001)        1 2023-07-20 22:51:58.000000 deepcellpredictor-0.9.3/deepcellpredictor.egg-info/dependency_links.txt
+-rw-rw-r--   0 gaurav    (1001) gaurav    (1001)       92 2023-07-20 22:51:58.000000 deepcellpredictor-0.9.3/deepcellpredictor.egg-info/requires.txt
+-rw-rw-r--   0 gaurav    (1001) gaurav    (1001)        4 2023-07-20 22:51:58.000000 deepcellpredictor-0.9.3/deepcellpredictor.egg-info/top_level.txt
+-rw-rw-r--   0 gaurav    (1001) gaurav    (1001)       38 2023-07-20 22:51:59.082783 deepcellpredictor-0.9.3/setup.cfg
+-rw-rw-r--   0 gaurav    (1001) gaurav    (1001)      800 2023-07-20 22:51:39.000000 deepcellpredictor-0.9.3/setup.py
```

### Comparing `deepcellpredictor-0.9.2/DCP/ModelPlanner.py` & `deepcellpredictor-0.9.3/DCP/ModelPlanner.py`

 * *Files identical despite different names*

### Comparing `deepcellpredictor-0.9.2/DCP/VAEtorch.py` & `deepcellpredictor-0.9.3/DCP/VAEtorch.py`

 * *Files identical despite different names*

### Comparing `deepcellpredictor-0.9.2/DCP/deep_predictor.py` & `deepcellpredictor-0.9.3/DCP/deep_predictor.py`

 * *Files identical despite different names*

### Comparing `deepcellpredictor-0.9.2/DCP/flow.py` & `deepcellpredictor-0.9.3/DCP/flow.py`

 * *Files identical despite different names*

### Comparing `deepcellpredictor-0.9.2/DCP/utils.py` & `deepcellpredictor-0.9.3/DCP/utils.py`

 * *Files identical despite different names*

### Comparing `deepcellpredictor-0.9.2/LICENSE` & `deepcellpredictor-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `deepcellpredictor-0.9.2/setup.py` & `deepcellpredictor-0.9.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from setuptools import setup, find_packages
 import os
 
-VERSION = '0.9.2'
+VERSION = '0.9.3'
 DESCRIPTION = "a transfer learning approach that explicitly models changes in transcriptional variance using a combination of variational autoencoders and normalizing flows"
 
 setup(
     name='deepcellpredictor',
     version=VERSION,
     description='transfer learning approach',
     long_description=DESCRIPTION,
     packages=find_packages(),
     install_requires=[
         'torch==1.11.0',
         'anndata==0.8.0',
         'pytorch_lightning==1.7.7',
         'scanpy==1.9.1',
         'scipy==1.6',
-        'scvi'
+        'scvi==0.19.0'
     ],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
     ],
     python_requires=">=3.6",
```

