# Comparing `tmp/FlashMHA-0.0.5.tar.gz` & `tmp/FlashMHA-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FlashMHA-0.0.5.tar", last modified: Fri Jul 21 14:36:25 2023, max compression
+gzip compressed data, was "FlashMHA-0.6.3.tar", last modified: Tue Jul 11 17:18:16 2023, max compression
```

## Comparing `FlashMHA-0.0.5.tar` & `FlashMHA-0.6.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:36:25.090334 FlashMHA-0.0.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:36:25.086334 FlashMHA-0.0.5/FlashMHA/
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-07-21 14:36:13.000000 FlashMHA-0.0.5/FlashMHA/FlashMHA.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-21 14:36:13.000000 FlashMHA-0.0.5/FlashMHA/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14994 2023-07-21 14:36:13.000000 FlashMHA-0.0.5/FlashMHA/attention.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:36:25.090334 FlashMHA-0.0.5/FlashMHA.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-21 14:36:25.000000 FlashMHA-0.0.5/FlashMHA.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-21 14:36:25.000000 FlashMHA-0.0.5/FlashMHA.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 14:36:25.000000 FlashMHA-0.0.5/FlashMHA.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-21 14:36:25.000000 FlashMHA-0.0.5/FlashMHA.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-21 14:36:25.000000 FlashMHA-0.0.5/FlashMHA.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-21 14:36:13.000000 FlashMHA-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-21 14:36:25.090334 FlashMHA-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4510 2023-07-21 14:36:13.000000 FlashMHA-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 14:36:25.090334 FlashMHA-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-07-21 14:36:13.000000 FlashMHA-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:18:16.171331 FlashMHA-0.6.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:18:16.171331 FlashMHA-0.6.3/FlashMHA/
+-rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-07-11 17:18:06.000000 FlashMHA-0.6.3/FlashMHA/FlashMHA.py
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-11 17:18:06.000000 FlashMHA-0.6.3/FlashMHA/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6169 2023-07-11 17:18:06.000000 FlashMHA-0.6.3/FlashMHA/attention.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:18:16.171331 FlashMHA-0.6.3/FlashMHA.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-11 17:18:16.000000 FlashMHA-0.6.3/FlashMHA.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-11 17:18:16.000000 FlashMHA-0.6.3/FlashMHA.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 17:18:16.000000 FlashMHA-0.6.3/FlashMHA.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-11 17:18:16.000000 FlashMHA-0.6.3/FlashMHA.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-11 17:18:16.000000 FlashMHA-0.6.3/FlashMHA.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-11 17:18:06.000000 FlashMHA-0.6.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-11 17:18:16.171331 FlashMHA-0.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-07-11 17:18:06.000000 FlashMHA-0.6.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 17:18:16.171331 FlashMHA-0.6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-07-11 17:18:06.000000 FlashMHA-0.6.3/setup.py
```

### Comparing `FlashMHA-0.0.5/FlashMHA.egg-info/PKG-INFO` & `FlashMHA-0.6.3/FlashMHA.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlashMHA
-Version: 0.0.5
+Version: 0.6.3
 Summary: FlashMHA - Pytorch
 Home-page: https://github.com/kyegomez/FlashMHA
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `FlashMHA-0.0.5/LICENSE` & `FlashMHA-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `FlashMHA-0.0.5/PKG-INFO` & `FlashMHA-0.6.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlashMHA
-Version: 0.0.5
+Version: 0.6.3
 Summary: FlashMHA - Pytorch
 Home-page: https://github.com/kyegomez/FlashMHA
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `FlashMHA-0.0.5/README.md` & `FlashMHA-0.6.3/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,61 +1,38 @@
 # FlashMHA
 FlashMHA is a PyTorch implementation of the Flash Multi-Head Attention mechanism. It is designed to be efficient and flexible, allowing for both causal and non-causal attention. The implementation also includes support for the Flash Attention mechanism, which is a highly efficient attention mechanism designed for GPUs.
 
 ## Installation
+You can install the FlashMHA library by cloning the GitHub repository and installing the required dependencies using `pip`:
 
-You can install FlashMHA using pip:
-
-```shell
-pip install FlashMHA
+```bash
+git clone https://github.com/kyegomez/FlashMHA.git
+cd FlashMHA
+pip install -r requirements.txt
 ```
 
 ## Usage
-
-After installing FlashMHA, you can import the FlashAttention module for usage in your code:
-
-```python
-from FlashMHA import FlashAttention
-```
-
-or
-
-```python
-from FlashMHA import FlashMHA
-```
-
-Now you can create an instance of the FlashAttention class or the FlashMHA class and use it in your code accordingly.
-
-Example usage:
+Here is a basic example of how to use the FlashMHA module:
 
 ```python
-# Import the necessary module
-from FlashMHA import FlashAttention
-
-# Create an instance of FlashAttention
-flash_attention = FlashAttention(causal=False, dropout=0.0)
+import torch
+from flash_mha import FlashMHA
 
-# Use the FlashAttention instance in your code
-output = flash_attention(query, key, value)
-```
-
-```python
-# Import the necessary module
-from FlashMHA import FlashMHA
+# Initialize the model
+flash_mha = FlashMHA(embed_dim=512, num_heads=8, bias=True, batch_first=True, dropout=0.0, causal=False)
 
-# Create an instance of FlashMHA
-flash_mha_attention = FlashMHA(causal=False, dropout=0.0)
+# Create input tensors
+query = torch.randn(10, 32, 512)
+key = torch.randn(10, 32, 512)
+value = torch.randn(10, 32, 512)
 
-# Use the FlashMHA instance in your code
-output = flash_mha_attention(query, key, value)
+# Forward pass
+output = flash_mha(query, key, value)
 ```
 
-Make sure to replace `query`, `key`, and `value` with your own input tensors.
-
-Now you can utilize the FlashAttention or FlashMHA module in your code by following the provided examples.
 In this example, `query`, `key`, and `value` are input tensors with shape `(batch_size, sequence_length, embed_dim)`. The FlashMHA model applies the multi-head attention mechanism to these inputs and returns the output tensor.
 
 ## Documentation
 
 
 ### `FlashAttention`
```

### Comparing `FlashMHA-0.0.5/setup.py` & `FlashMHA-0.6.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 # 
 
 setup(
   name = 'FlashMHA',
   packages = find_packages(exclude=[]),
-  version = '0.0.5',
+  version = '0.6.3',
   license='MIT',
   description = 'FlashMHA - Pytorch',
   author = 'Kye Gomez',
   author_email = 'kye@apac.ai',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/kyegomez/FlashMHA',
   keywords = [
```

