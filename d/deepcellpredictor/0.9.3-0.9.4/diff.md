# Comparing `tmp/deepcellpredictor-0.9.3.tar.gz` & `tmp/deepcellpredictor-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepcellpredictor-0.9.3.tar", last modified: Thu Jul 20 22:51:59 2023, max compression
+gzip compressed data, was "deepcellpredictor-0.9.4.tar", last modified: Thu Jul 20 22:53:59 2023, max compression
```

## Comparing `deepcellpredictor-0.9.3.tar` & `deepcellpredictor-0.9.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 gaurav    (1001) gaurav    (1001)        0 2023-07-20 22:51:59.082783 deepcellpredictor-0.9.3/
-drwxrwxr-x   0 gaurav    (1001) gaurav    (1001)        0 2023-07-20 22:51:59.082783 deepcellpredictor-0.9.3/DCP/
--rw-rw-r--   0 gaurav    (1001) gaurav    (1001)     1245 2023-07-20 15:52:22.000000 deepcellpredictor-0.9.3/DCP/ModelPlanner.py
--rw-rw-r--   0 gaurav    (1001) gaurav    (1001)     8298 2023-07-20 22:39:47.000000 deepcellpredictor-0.9.3/DCP/VAEtorch.py
--rw-rw-r--   0 gaurav    (1001) gaurav    (1001)      474 2023-07-20 20:33:00.000000 deepcellpredictor-0.9.3/DCP/__init__.py
--rw-rw-r--   0 gaurav    (1001) gaurav    (1001)    11734 2023-07-20 22:35:17.000000 deepcellpredictor-0.9.3/DCP/deep_predictor.py
--rw-rw-r--   0 gaurav    (1001) gaurav    (1001)     4056 2023-07-20 15:52:22.000000 deepcellpredictor-0.9.3/DCP/flow.py
--rw-rw-r--   0 gaurav    (1001) gaurav    (1001)      679 2023-07-20 15:52:22.000000 deepcellpredictor-0.9.3/DCP/utils.py
--rw-rw-r--   0 gaurav    (1001) gaurav    (1001)     1063 2023-07-20 20:33:00.000000 deepcellpredictor-0.9.3/LICENSE
--rw-rw-r--   0 gaurav    (1001) gaurav    (1001)      444 2023-07-20 22:51:59.082783 deepcellpredictor-0.9.3/PKG-INFO
--rw-rw-r--   0 gaurav    (1001) gaurav    (1001)      182 2023-07-20 15:52:22.000000 deepcellpredictor-0.9.3/README.md
-drwxrwxr-x   0 gaurav    (1001) gaurav    (1001)        0 2023-07-20 22:51:59.082783 deepcellpredictor-0.9.3/deepcellpredictor.egg-info/
--rw-rw-r--   0 gaurav    (1001) gaurav    (1001)      444 2023-07-20 22:51:58.000000 deepcellpredictor-0.9.3/deepcellpredictor.egg-info/PKG-INFO
--rw-rw-r--   0 gaurav    (1001) gaurav    (1001)      329 2023-07-20 22:51:59.000000 deepcellpredictor-0.9.3/deepcellpredictor.egg-info/SOURCES.txt
--rw-rw-r--   0 gaurav    (1001) gaurav    (1001)        1 2023-07-20 22:51:58.000000 deepcellpredictor-0.9.3/deepcellpredictor.egg-info/dependency_links.txt
--rw-rw-r--   0 gaurav    (1001) gaurav    (1001)       92 2023-07-20 22:51:58.000000 deepcellpredictor-0.9.3/deepcellpredictor.egg-info/requires.txt
--rw-rw-r--   0 gaurav    (1001) gaurav    (1001)        4 2023-07-20 22:51:58.000000 deepcellpredictor-0.9.3/deepcellpredictor.egg-info/top_level.txt
--rw-rw-r--   0 gaurav    (1001) gaurav    (1001)       38 2023-07-20 22:51:59.082783 deepcellpredictor-0.9.3/setup.cfg
--rw-rw-r--   0 gaurav    (1001) gaurav    (1001)      800 2023-07-20 22:51:39.000000 deepcellpredictor-0.9.3/setup.py
+drwxrwxr-x   0 gaurav    (1001) gaurav    (1001)        0 2023-07-20 22:53:59.387201 deepcellpredictor-0.9.4/
+drwxrwxr-x   0 gaurav    (1001) gaurav    (1001)        0 2023-07-20 22:53:59.387201 deepcellpredictor-0.9.4/DCP/
+-rw-rw-r--   0 gaurav    (1001) gaurav    (1001)     1245 2023-07-20 15:52:22.000000 deepcellpredictor-0.9.4/DCP/ModelPlanner.py
+-rw-rw-r--   0 gaurav    (1001) gaurav    (1001)     8298 2023-07-20 22:39:47.000000 deepcellpredictor-0.9.4/DCP/VAEtorch.py
+-rw-rw-r--   0 gaurav    (1001) gaurav    (1001)      474 2023-07-20 20:33:00.000000 deepcellpredictor-0.9.4/DCP/__init__.py
+-rw-rw-r--   0 gaurav    (1001) gaurav    (1001)    11734 2023-07-20 22:35:17.000000 deepcellpredictor-0.9.4/DCP/deep_predictor.py
+-rw-rw-r--   0 gaurav    (1001) gaurav    (1001)     4056 2023-07-20 15:52:22.000000 deepcellpredictor-0.9.4/DCP/flow.py
+-rw-rw-r--   0 gaurav    (1001) gaurav    (1001)      679 2023-07-20 15:52:22.000000 deepcellpredictor-0.9.4/DCP/utils.py
+-rw-rw-r--   0 gaurav    (1001) gaurav    (1001)     1063 2023-07-20 20:33:00.000000 deepcellpredictor-0.9.4/LICENSE
+-rw-rw-r--   0 gaurav    (1001) gaurav    (1001)      444 2023-07-20 22:53:59.387201 deepcellpredictor-0.9.4/PKG-INFO
+-rw-rw-r--   0 gaurav    (1001) gaurav    (1001)      182 2023-07-20 15:52:22.000000 deepcellpredictor-0.9.4/README.md
+drwxrwxr-x   0 gaurav    (1001) gaurav    (1001)        0 2023-07-20 22:53:59.387201 deepcellpredictor-0.9.4/deepcellpredictor.egg-info/
+-rw-rw-r--   0 gaurav    (1001) gaurav    (1001)      444 2023-07-20 22:53:58.000000 deepcellpredictor-0.9.4/deepcellpredictor.egg-info/PKG-INFO
+-rw-rw-r--   0 gaurav    (1001) gaurav    (1001)      329 2023-07-20 22:53:59.000000 deepcellpredictor-0.9.4/deepcellpredictor.egg-info/SOURCES.txt
+-rw-rw-r--   0 gaurav    (1001) gaurav    (1001)        1 2023-07-20 22:53:58.000000 deepcellpredictor-0.9.4/deepcellpredictor.egg-info/dependency_links.txt
+-rw-rw-r--   0 gaurav    (1001) gaurav    (1001)       90 2023-07-20 22:53:59.000000 deepcellpredictor-0.9.4/deepcellpredictor.egg-info/requires.txt
+-rw-rw-r--   0 gaurav    (1001) gaurav    (1001)        4 2023-07-20 22:53:59.000000 deepcellpredictor-0.9.4/deepcellpredictor.egg-info/top_level.txt
+-rw-rw-r--   0 gaurav    (1001) gaurav    (1001)       38 2023-07-20 22:53:59.387201 deepcellpredictor-0.9.4/setup.cfg
+-rw-rw-r--   0 gaurav    (1001) gaurav    (1001)      798 2023-07-20 22:53:41.000000 deepcellpredictor-0.9.4/setup.py
```

### Comparing `deepcellpredictor-0.9.3/DCP/ModelPlanner.py` & `deepcellpredictor-0.9.4/DCP/ModelPlanner.py`

 * *Files identical despite different names*

### Comparing `deepcellpredictor-0.9.3/DCP/VAEtorch.py` & `deepcellpredictor-0.9.4/DCP/VAEtorch.py`

 * *Files identical despite different names*

### Comparing `deepcellpredictor-0.9.3/DCP/deep_predictor.py` & `deepcellpredictor-0.9.4/DCP/deep_predictor.py`

 * *Files identical despite different names*

### Comparing `deepcellpredictor-0.9.3/DCP/flow.py` & `deepcellpredictor-0.9.4/DCP/flow.py`

 * *Files identical despite different names*

### Comparing `deepcellpredictor-0.9.3/DCP/utils.py` & `deepcellpredictor-0.9.4/DCP/utils.py`

 * *Files identical despite different names*

### Comparing `deepcellpredictor-0.9.3/LICENSE` & `deepcellpredictor-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `deepcellpredictor-0.9.3/setup.py` & `deepcellpredictor-0.9.4/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from setuptools import setup, find_packages
 import os
 
-VERSION = '0.9.3'
+VERSION = '0.9.4'
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
-        'scvi==0.19.0'
+        'scvi-tools'
     ],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
     ],
     python_requires=">=3.6",
```

