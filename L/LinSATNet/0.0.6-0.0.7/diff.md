# Comparing `tmp/LinSATNet-0.0.6.tar.gz` & `tmp/LinSATNet-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LinSATNet-0.0.6.tar", last modified: Fri Jun 16 13:41:14 2023, max compression
+gzip compressed data, was "LinSATNet-0.0.7.tar", last modified: Fri Jul 21 15:46:18 2023, max compression
```

## Comparing `LinSATNet-0.0.6.tar` & `LinSATNet-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:41:14.551974 LinSATNet-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-16 13:41:05.000000 LinSATNet-0.0.6/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:41:14.551974 LinSATNet-0.0.6/LinSATNet/
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-16 13:41:05.000000 LinSATNet-0.0.6/LinSATNet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11748 2023-06-16 13:41:05.000000 LinSATNet-0.0.6/LinSATNet/linsat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:41:14.551974 LinSATNet-0.0.6/LinSATNet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6903 2023-06-16 13:41:14.000000 LinSATNet-0.0.6/LinSATNet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-16 13:41:14.000000 LinSATNet-0.0.6/LinSATNet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 13:41:14.000000 LinSATNet-0.0.6/LinSATNet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-16 13:41:14.000000 LinSATNet-0.0.6/LinSATNet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-16 13:41:14.000000 LinSATNet-0.0.6/LinSATNet.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6903 2023-06-16 13:41:14.551974 LinSATNet-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18922 2023-06-16 13:41:05.000000 LinSATNet-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 13:41:14.551974 LinSATNet-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-06-16 13:41:05.000000 LinSATNet-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:46:18.897322 LinSATNet-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-21 15:46:05.000000 LinSATNet-0.0.7/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:46:18.893322 LinSATNet-0.0.7/LinSATNet/
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-21 15:46:05.000000 LinSATNet-0.0.7/LinSATNet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11864 2023-07-21 15:46:05.000000 LinSATNet-0.0.7/LinSATNet/linsat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:46:18.893322 LinSATNet-0.0.7/LinSATNet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6984 2023-07-21 15:46:18.000000 LinSATNet-0.0.7/LinSATNet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-21 15:46:18.000000 LinSATNet-0.0.7/LinSATNet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 15:46:18.000000 LinSATNet-0.0.7/LinSATNet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-21 15:46:18.000000 LinSATNet-0.0.7/LinSATNet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-21 15:46:18.000000 LinSATNet-0.0.7/LinSATNet.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6984 2023-07-21 15:46:18.897322 LinSATNet-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18996 2023-07-21 15:46:05.000000 LinSATNet-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 15:46:18.897322 LinSATNet-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-07-21 15:46:05.000000 LinSATNet-0.0.7/setup.py
```

### Comparing `LinSATNet-0.0.6/LICENSE` & `LinSATNet-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `LinSATNet-0.0.6/LinSATNet/linsat.py` & `LinSATNet-0.0.7/LinSATNet/linsat.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,26 +4,28 @@
 #
 # Code author: Runzhong Wang (runzhong.wang@outlook.com)
 
 import torch
 import sys
 
 
-def linsat_layer(x, A=None, b=None, C=None, d=None, E=None, f=None, tau=0.05, max_iter=100, dummy_val=0, mode='v1'):
+def linsat_layer(x, A=None, b=None, C=None, d=None, E=None, f=None, tau=0.05, max_iter=100, dummy_val=0,
+                 mode='v1', no_warning=False):
     """
     Project x with the constraints A x <= b, C x >= d, E x = f.
     All elements in A, b, C, d, E, f must be non-negative.
 
     :param x: (n_v), it can optionally have a batch size (b x n_v)
     :param A, C, E: (n_c x n_v)
     :param b, d, f: (n_c)
     :param tau: parameter to control hard/soft constraint
     :param max_iter: max number of iterations
     :param dummy_val: value of dummy variable
     :param mode: v1 or v2
+    :param no_warning: turn off warning message
     :return: (n_v) or (b x n_v), the projected variables
     """
     if len(x.shape) == 1:
         x = x.unsqueeze(0)
         vector_input = True
     elif len(x.shape) == 2:
         vector_input = False
@@ -158,15 +160,16 @@
         cv_Ef = torch.abs(torch.matmul(ori_E, torch.exp(log_x).t()).t() - ori_f.unsqueeze(0))
 
         if diff <= 1e-3 and \
                 torch.sum(cv_Ab[cv_Ab > 0]) + torch.sum(cv_Cd[cv_Cd > 0]) + torch.sum(cv_Ef[cv_Ef > 0]) < 1e-3:
             break
         last_log_x = log_x
 
-    if torch.sum(cv_Ab[cv_Ab > 0]) + torch.sum(cv_Cd[cv_Cd > 0]) + torch.sum(cv_Ef[cv_Ef > 0]) > 0.1 * batch_size:
+    if not no_warning and \
+            torch.sum(cv_Ab[cv_Ab > 0]) + torch.sum(cv_Cd[cv_Cd > 0]) + torch.sum(cv_Ef[cv_Ef > 0]) > 0.1 * batch_size:
         print('Warning: non-zero constraint violation within max iterations. Add more iterations or infeasible?',
               file=sys.stderr)
 
     return torch.exp(log_x)
 
 
 def linsat_kernel_v2(x, A, b, tau, max_iter, dummy_val,
```

### Comparing `LinSATNet-0.0.6/LinSATNet.egg-info/PKG-INFO` & `LinSATNet-0.0.7/LinSATNet.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LinSATNet
-Version: 0.0.6
+Version: 0.0.7
 Summary: LinSATNet offers a neural network layer to enforce the satisfiability of positive linear constraints to the output of neural networks. The gradient through the layer is exactly computed. This package now works with PyTorch.
 Home-page: https://github.com/Thinklab-SJTU/LinSATNet
 Author: Runzhong Wang
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Environment :: GPU :: NVIDIA CUDA
@@ -132,29 +132,30 @@
 ```
 and import the pacakge at the beginning of your code:
 ```python
 from LinSATNet import linsat_layer
 ```
 
 ### The ``linsat_layer`` function
-> **LinSATNet.linsat_layer**(x, A=None, b=None, C=None, d=None, E=None, f=None, tau=0.05, max_iter=100, dummy_val=0, mode='v1') [[source]](https://github.com/Thinklab-SJTU/LinSATNet/blob/main/LinSATNet/linsat.py#L11)
+> **LinSATNet.linsat_layer**(x, A=None, b=None, C=None, d=None, E=None, f=None, tau=0.05, max_iter=100, dummy_val=0, mode='v1', no_warning=False) [[source]](https://github.com/Thinklab-SJTU/LinSATNet/blob/main/LinSATNet/linsat.py#L11)
 
 LinSAT layer enforces positive linear constraints to the input ``x`` and
 projects it with the constraints
 $$\mathbf{A} \mathbf{x} <= \mathbf{b}, \mathbf{C} \mathbf{x} >= \mathbf{d}, \mathbf{E} \mathbf{x} = \mathbf{f}$$
 and all elements in $\mathbf{A}, \mathbf{b}, \mathbf{C}, \mathbf{d}, \mathbf{E}, \mathbf{f}$ must be non-negative.
 
 **Parameters:**
 * ``x``: PyTorch tensor of size ($n_v$), it can optionally have a batch size ($b \times n_v$)
 * ``A``, ``C``, ``E``: PyTorch tensor of size ($n_c \times n_v$), constraint matrix on the left hand side
 * ``b``, ``d``, ``f``: PyTorch tensor of size ($n_c$), constraint vector on the right hand side
 * ``tau``: (``default=0.05``) parameter to control the discreteness of the projection. Smaller value leads to more discrete (harder) results, larger value leads to more continuous (softer) results.
 * ``max_iter``: (``default=100``) max number of iterations
 * ``dummy_val``: (``default=0``) the value of dummy variables appended to the input vector
 * ``mode``: (``default='v1'``) EXPERIMENTAL the mode of LinSAT kernel. ``v2`` is sometimes faster than ``v1``.
+* ``no_warning``: (``default=False``) turn off warning message
 
 **return:** PyTorch tensor of size ($n_v$) or ($b \times n_v$), the projected variables
 
 Notations:
 * $b$ means the batch size.
 * $n_c$ means the number of constraints ($\mathbf{A}$, $\mathbf{C}$, $\mathbf{E}$ may have different $n_c$)
 * $n_v$ means the number of variables
```

### Comparing `LinSATNet-0.0.6/PKG-INFO` & `LinSATNet-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LinSATNet
-Version: 0.0.6
+Version: 0.0.7
 Summary: LinSATNet offers a neural network layer to enforce the satisfiability of positive linear constraints to the output of neural networks. The gradient through the layer is exactly computed. This package now works with PyTorch.
 Home-page: https://github.com/Thinklab-SJTU/LinSATNet
 Author: Runzhong Wang
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Environment :: GPU :: NVIDIA CUDA
@@ -132,29 +132,30 @@
 ```
 and import the pacakge at the beginning of your code:
 ```python
 from LinSATNet import linsat_layer
 ```
 
 ### The ``linsat_layer`` function
-> **LinSATNet.linsat_layer**(x, A=None, b=None, C=None, d=None, E=None, f=None, tau=0.05, max_iter=100, dummy_val=0, mode='v1') [[source]](https://github.com/Thinklab-SJTU/LinSATNet/blob/main/LinSATNet/linsat.py#L11)
+> **LinSATNet.linsat_layer**(x, A=None, b=None, C=None, d=None, E=None, f=None, tau=0.05, max_iter=100, dummy_val=0, mode='v1', no_warning=False) [[source]](https://github.com/Thinklab-SJTU/LinSATNet/blob/main/LinSATNet/linsat.py#L11)
 
 LinSAT layer enforces positive linear constraints to the input ``x`` and
 projects it with the constraints
 $$\mathbf{A} \mathbf{x} <= \mathbf{b}, \mathbf{C} \mathbf{x} >= \mathbf{d}, \mathbf{E} \mathbf{x} = \mathbf{f}$$
 and all elements in $\mathbf{A}, \mathbf{b}, \mathbf{C}, \mathbf{d}, \mathbf{E}, \mathbf{f}$ must be non-negative.
 
 **Parameters:**
 * ``x``: PyTorch tensor of size ($n_v$), it can optionally have a batch size ($b \times n_v$)
 * ``A``, ``C``, ``E``: PyTorch tensor of size ($n_c \times n_v$), constraint matrix on the left hand side
 * ``b``, ``d``, ``f``: PyTorch tensor of size ($n_c$), constraint vector on the right hand side
 * ``tau``: (``default=0.05``) parameter to control the discreteness of the projection. Smaller value leads to more discrete (harder) results, larger value leads to more continuous (softer) results.
 * ``max_iter``: (``default=100``) max number of iterations
 * ``dummy_val``: (``default=0``) the value of dummy variables appended to the input vector
 * ``mode``: (``default='v1'``) EXPERIMENTAL the mode of LinSAT kernel. ``v2`` is sometimes faster than ``v1``.
+* ``no_warning``: (``default=False``) turn off warning message
 
 **return:** PyTorch tensor of size ($n_v$) or ($b \times n_v$), the projected variables
 
 Notations:
 * $b$ means the batch size.
 * $n_c$ means the number of constraints ($\mathbf{A}$, $\mathbf{C}$, $\mathbf{E}$ may have different $n_c$)
 * $n_v$ means the number of variables
```

### Comparing `LinSATNet-0.0.6/README.md` & `LinSATNet-0.0.7/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -22,23 +22,23 @@
 ```
 
 ### Table of contents
 
 - [LinSATNet](#linsatnet)
   * [A Quick Example](#a-quick-example)
   * [API Reference](#api-reference)
-    + [The ``linsat_layer`` function](#the---linsat-layer---function)
+    + [The ``linsat_layer`` function](#the-linsat_layer-function)
     + [Some practical notes](#some-practical-notes)
   * [How it works?](#how-it-works-)
     + [Classic Sinkhorn with single-set marginals](#classic-sinkhorn-with-single-set-marginals)
     + [Extended Sinkhorn with multi-set marginals](#extended-sinkhorn-with-multi-set-marginals)
     + [Transforming positive linear constraints into marginals](#transforming-positive-linear-constraints-into-marginals)
-      - [Encoding neural network's output](#encoding-neural-network-s-output)
+      - [Encoding neural network's output](#encoding-neural-networks-output)
       - [From linear constraints to marginals](#from-linear-constraints-to-marginals)
-  * [More Complicated Use Cases (appeared in our paper)](#more-complicated-use-cases--appeared-in-our-paper-)
+  * [More Complicated Use Cases (appeared in our paper)](#more-complicated-use-cases-appeared-in-our-paper)
     + [I. Neural Solver for Traveling Salesman Problem with Extra Constraints](#i-neural-solver-for-traveling-salesman-problem-with-extra-constraints)
     + [II. Partial Graph Matching with Outliers on Both Sides](#ii-partial-graph-matching-with-outliers-on-both-sides)
     + [III. Portfolio Allocation](#iii-portfolio-allocation)
   * [Citation](#citation)
 
 ## A Quick Example
 
@@ -134,29 +134,30 @@
 ```
 and import the pacakge at the beginning of your code:
 ```python
 from LinSATNet import linsat_layer
 ```
 
 ### The ``linsat_layer`` function
-> **LinSATNet.linsat_layer**(x, A=None, b=None, C=None, d=None, E=None, f=None, tau=0.05, max_iter=100, dummy_val=0, mode='v1') [[source]](https://github.com/Thinklab-SJTU/LinSATNet/blob/main/LinSATNet/linsat.py#L11)
+> **LinSATNet.linsat_layer**(x, A=None, b=None, C=None, d=None, E=None, f=None, tau=0.05, max_iter=100, dummy_val=0, mode='v1', no_warning=False) [[source]](https://github.com/Thinklab-SJTU/LinSATNet/blob/main/LinSATNet/linsat.py#L11)
 
 LinSAT layer enforces positive linear constraints to the input ``x`` and
 projects it with the constraints
 $$\mathbf{A} \mathbf{x} <= \mathbf{b}, \mathbf{C} \mathbf{x} >= \mathbf{d}, \mathbf{E} \mathbf{x} = \mathbf{f}$$
 and all elements in $\mathbf{A}, \mathbf{b}, \mathbf{C}, \mathbf{d}, \mathbf{E}, \mathbf{f}$ must be non-negative.
 
 **Parameters:**
 * ``x``: PyTorch tensor of size ($n_v$), it can optionally have a batch size ($b \times n_v$)
 * ``A``, ``C``, ``E``: PyTorch tensor of size ($n_c \times n_v$), constraint matrix on the left hand side
 * ``b``, ``d``, ``f``: PyTorch tensor of size ($n_c$), constraint vector on the right hand side
 * ``tau``: (``default=0.05``) parameter to control the discreteness of the projection. Smaller value leads to more discrete (harder) results, larger value leads to more continuous (softer) results.
 * ``max_iter``: (``default=100``) max number of iterations
 * ``dummy_val``: (``default=0``) the value of dummy variables appended to the input vector
 * ``mode``: (``default='v1'``) EXPERIMENTAL the mode of LinSAT kernel. ``v2`` is sometimes faster than ``v1``.
+* ``no_warning``: (``default=False``) turn off warning message
 
 **return:** PyTorch tensor of size ($n_v$) or ($b \times n_v$), the projected variables
 
 Notations:
 * $b$ means the batch size.
 * $n_c$ means the number of constraints ($\mathbf{A}$, $\mathbf{C}$, $\mathbf{E}$ may have different $n_c$)
 * $n_v$ means the number of variables
```

### Comparing `LinSATNet-0.0.6/setup.py` & `LinSATNet-0.0.7/setup.py`

 * *Files identical despite different names*

