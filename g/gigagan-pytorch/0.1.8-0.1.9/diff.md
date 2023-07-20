# Comparing `tmp/gigagan-pytorch-0.1.8.tar.gz` & `tmp/gigagan-pytorch-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gigagan-pytorch-0.1.8.tar", last modified: Thu Jul 20 19:21:33 2023, max compression
+gzip compressed data, was "gigagan-pytorch-0.1.9.tar", last modified: Thu Jul 20 19:30:08 2023, max compression
```

## Comparing `gigagan-pytorch-0.1.8.tar` & `gigagan-pytorch-0.1.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:21:33.149839 gigagan-pytorch-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-20 19:21:21.000000 gigagan-pytorch-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-20 19:21:33.149839 gigagan-pytorch-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8704 2023-07-20 19:21:21.000000 gigagan-pytorch-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:21:33.149839 gigagan-pytorch-0.1.8/gigagan_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-20 19:21:21.000000 gigagan-pytorch-0.1.8/gigagan_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-07-20 19:21:21.000000 gigagan-pytorch-0.1.8/gigagan_pytorch/attend.py
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-07-20 19:21:21.000000 gigagan-pytorch-0.1.8/gigagan_pytorch/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    71724 2023-07-20 19:21:21.000000 gigagan-pytorch-0.1.8/gigagan_pytorch/gigagan_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4585 2023-07-20 19:21:21.000000 gigagan-pytorch-0.1.8/gigagan_pytorch/open_clip.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-20 19:21:21.000000 gigagan-pytorch-0.1.8/gigagan_pytorch/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    17727 2023-07-20 19:21:21.000000 gigagan-pytorch-0.1.8/gigagan_pytorch/unet_upsampler.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-20 19:21:21.000000 gigagan-pytorch-0.1.8/gigagan_pytorch/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:21:33.149839 gigagan-pytorch-0.1.8/gigagan_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-20 19:21:33.000000 gigagan-pytorch-0.1.8/gigagan_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-20 19:21:33.000000 gigagan-pytorch-0.1.8/gigagan_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 19:21:33.000000 gigagan-pytorch-0.1.8/gigagan_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-20 19:21:33.000000 gigagan-pytorch-0.1.8/gigagan_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-20 19:21:33.000000 gigagan-pytorch-0.1.8/gigagan_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-20 19:21:21.000000 gigagan-pytorch-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 19:21:33.149839 gigagan-pytorch-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-20 19:21:21.000000 gigagan-pytorch-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:30:08.250156 gigagan-pytorch-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-20 19:29:58.000000 gigagan-pytorch-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-20 19:30:08.250156 gigagan-pytorch-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8704 2023-07-20 19:29:58.000000 gigagan-pytorch-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:30:08.246156 gigagan-pytorch-0.1.9/gigagan_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-20 19:29:58.000000 gigagan-pytorch-0.1.9/gigagan_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-07-20 19:29:58.000000 gigagan-pytorch-0.1.9/gigagan_pytorch/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-07-20 19:29:58.000000 gigagan-pytorch-0.1.9/gigagan_pytorch/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71723 2023-07-20 19:29:58.000000 gigagan-pytorch-0.1.9/gigagan_pytorch/gigagan_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4585 2023-07-20 19:29:58.000000 gigagan-pytorch-0.1.9/gigagan_pytorch/open_clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-20 19:29:58.000000 gigagan-pytorch-0.1.9/gigagan_pytorch/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17727 2023-07-20 19:29:58.000000 gigagan-pytorch-0.1.9/gigagan_pytorch/unet_upsampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-20 19:29:58.000000 gigagan-pytorch-0.1.9/gigagan_pytorch/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:30:08.250156 gigagan-pytorch-0.1.9/gigagan_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-20 19:30:08.000000 gigagan-pytorch-0.1.9/gigagan_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-20 19:30:08.000000 gigagan-pytorch-0.1.9/gigagan_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 19:30:08.000000 gigagan-pytorch-0.1.9/gigagan_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-20 19:30:08.000000 gigagan-pytorch-0.1.9/gigagan_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-20 19:30:08.000000 gigagan-pytorch-0.1.9/gigagan_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-20 19:29:58.000000 gigagan-pytorch-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 19:30:08.250156 gigagan-pytorch-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-20 19:29:58.000000 gigagan-pytorch-0.1.9/setup.py
```

### Comparing `gigagan-pytorch-0.1.8/LICENSE` & `gigagan-pytorch-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `gigagan-pytorch-0.1.8/PKG-INFO` & `gigagan-pytorch-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gigagan-pytorch
-Version: 0.1.8
+Version: 0.1.9
 Summary: GigaGAN - Pytorch
 Home-page: https://github.com/lucidrains/ETSformer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,generative adversarial networks
 Classifier: Development Status :: 4 - Beta
```

### Comparing `gigagan-pytorch-0.1.8/README.md` & `gigagan-pytorch-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `gigagan-pytorch-0.1.8/gigagan_pytorch/__init__.py` & `gigagan-pytorch-0.1.9/gigagan_pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `gigagan-pytorch-0.1.8/gigagan_pytorch/attend.py` & `gigagan-pytorch-0.1.9/gigagan_pytorch/attend.py`

 * *Files identical despite different names*

### Comparing `gigagan-pytorch-0.1.8/gigagan_pytorch/data.py` & `gigagan-pytorch-0.1.9/gigagan_pytorch/data.py`

 * *Files identical despite different names*

### Comparing `gigagan-pytorch-0.1.8/gigagan_pytorch/gigagan_pytorch.py` & `gigagan-pytorch-0.1.9/gigagan_pytorch/gigagan_pytorch.py`

 * *Files 0% similar despite different names*

```diff
@@ -1664,15 +1664,15 @@
         early_save_and_sample_every = 100,
         num_samples = 25,
         model_folder = './gigagan-models',
         results_folder = './gigagan-results',
         sample_upsampler_dl: Optional[DataLoader] = None,
         accelerator: Optional[Accelerator] = None,
         accelerate_kwargs: dict = {},
-        find_unused_parameters = False,
+        find_unused_parameters = True,
         amp = False,
         mixed_precision_type = 'fp16'
     ):
         super().__init__()
 
         # create accelerator
```

### Comparing `gigagan-pytorch-0.1.8/gigagan_pytorch/open_clip.py` & `gigagan-pytorch-0.1.9/gigagan_pytorch/open_clip.py`

 * *Files identical despite different names*

### Comparing `gigagan-pytorch-0.1.8/gigagan_pytorch/optimizer.py` & `gigagan-pytorch-0.1.9/gigagan_pytorch/optimizer.py`

 * *Files identical despite different names*

### Comparing `gigagan-pytorch-0.1.8/gigagan_pytorch/unet_upsampler.py` & `gigagan-pytorch-0.1.9/gigagan_pytorch/unet_upsampler.py`

 * *Files identical despite different names*

### Comparing `gigagan-pytorch-0.1.8/gigagan_pytorch.egg-info/PKG-INFO` & `gigagan-pytorch-0.1.9/gigagan_pytorch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gigagan-pytorch
-Version: 0.1.8
+Version: 0.1.9
 Summary: GigaGAN - Pytorch
 Home-page: https://github.com/lucidrains/ETSformer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,generative adversarial networks
 Classifier: Development Status :: 4 - Beta
```

### Comparing `gigagan-pytorch-0.1.8/setup.py` & `gigagan-pytorch-0.1.9/setup.py`

 * *Files identical despite different names*

