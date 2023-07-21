# Comparing `tmp/LinSATNet-0.0.7.tar.gz` & `tmp/LinSATNet-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LinSATNet-0.0.7.tar", last modified: Fri Jul 21 15:46:18 2023, max compression
+gzip compressed data, was "LinSATNet-0.0.8.tar", last modified: Fri Jul 21 16:00:05 2023, max compression
```

## Comparing `LinSATNet-0.0.7.tar` & `LinSATNet-0.0.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:46:18.897322 LinSATNet-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-21 15:46:05.000000 LinSATNet-0.0.7/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:46:18.893322 LinSATNet-0.0.7/LinSATNet/
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-21 15:46:05.000000 LinSATNet-0.0.7/LinSATNet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11864 2023-07-21 15:46:05.000000 LinSATNet-0.0.7/LinSATNet/linsat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:46:18.893322 LinSATNet-0.0.7/LinSATNet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6984 2023-07-21 15:46:18.000000 LinSATNet-0.0.7/LinSATNet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-21 15:46:18.000000 LinSATNet-0.0.7/LinSATNet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 15:46:18.000000 LinSATNet-0.0.7/LinSATNet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-21 15:46:18.000000 LinSATNet-0.0.7/LinSATNet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-21 15:46:18.000000 LinSATNet-0.0.7/LinSATNet.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6984 2023-07-21 15:46:18.897322 LinSATNet-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18996 2023-07-21 15:46:05.000000 LinSATNet-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 15:46:18.897322 LinSATNet-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-07-21 15:46:05.000000 LinSATNet-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:00:05.778843 LinSATNet-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-21 15:59:53.000000 LinSATNet-0.0.8/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:00:05.778843 LinSATNet-0.0.8/LinSATNet/
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-21 15:59:53.000000 LinSATNet-0.0.8/LinSATNet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11994 2023-07-21 15:59:53.000000 LinSATNet-0.0.8/LinSATNet/linsat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:00:05.778843 LinSATNet-0.0.8/LinSATNet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6984 2023-07-21 16:00:05.000000 LinSATNet-0.0.8/LinSATNet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-21 16:00:05.000000 LinSATNet-0.0.8/LinSATNet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 16:00:05.000000 LinSATNet-0.0.8/LinSATNet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-21 16:00:05.000000 LinSATNet-0.0.8/LinSATNet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-21 16:00:05.000000 LinSATNet-0.0.8/LinSATNet.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6984 2023-07-21 16:00:05.778843 LinSATNet-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18996 2023-07-21 15:59:53.000000 LinSATNet-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 16:00:05.778843 LinSATNet-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-07-21 15:59:53.000000 LinSATNet-0.0.8/setup.py
```

### Comparing `LinSATNet-0.0.7/LICENSE` & `LinSATNet-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `LinSATNet-0.0.7/LinSATNet/linsat.py` & `LinSATNet-0.0.8/LinSATNet/linsat.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,23 +92,25 @@
         kernel = linsat_kernel_v1
     elif mode == 'v2':
         kernel = linsat_kernel_v2
     else:
         raise ValueError(f'Unknown mode {mode}')
 
     x = kernel(x, A, b, tau, max_iter, dummy_val,
-               batch_size, num_var, num_constr, ori_A, ori_b, ori_C, ori_d, ori_E, ori_f)
+               batch_size, num_var, num_constr, ori_A, ori_b, ori_C, ori_d, ori_E, ori_f,
+               no_warning)
 
     if vector_input:
         x.squeeze_(0)
     return x
 
 
 def linsat_kernel_v1(x, A, b, tau, max_iter, dummy_val,
-                     batch_size, num_var, num_constr, ori_A, ori_b, ori_C, ori_d, ori_E, ori_f):
+                     batch_size, num_var, num_constr, ori_A, ori_b, ori_C, ori_d, ori_E, ori_f,
+                     no_warning):
     # add dummy variables
     dum_x1 = []
     dum_x2 = []
     for j in range(num_constr):
         dum_x1.append(torch.full((batch_size, 1), dummy_val, dtype=x.dtype, device=x.device))
         dum_x2.append(torch.full((batch_size, torch.sum(A[j] != 0)), dummy_val, dtype=x.dtype, device=x.device))
 
@@ -169,15 +171,16 @@
         print('Warning: non-zero constraint violation within max iterations. Add more iterations or infeasible?',
               file=sys.stderr)
 
     return torch.exp(log_x)
 
 
 def linsat_kernel_v2(x, A, b, tau, max_iter, dummy_val,
-                     batch_size, num_var, num_constr, ori_A, ori_b, ori_C, ori_d, ori_E, ori_f):
+                     batch_size, num_var, num_constr, ori_A, ori_b, ori_C, ori_d, ori_E, ori_f,
+                     no_warning):
     # add dummy variables
     dum_x1 = []
     for j in range(num_constr):
         dum_x1.append(torch.full((batch_size, 2, 1), dummy_val, dtype=x.dtype, device=x.device))
     dum_x2 = torch.full((batch_size, num_var), dummy_val, dtype=x.dtype, device=x.device)
 
     # operations are performed on log scale
@@ -231,15 +234,16 @@
 
     x = torch.exp(log_x[:, 0, :]) # remove dummy row & transform from log scale
 
     with torch.no_grad():
         cv_Ab = torch.matmul(ori_A, x.t()).t() - ori_b.unsqueeze(0)
         cv_Cd = -torch.matmul(ori_C, x.t()).t() + ori_d.unsqueeze(0)
         cv_Ef = torch.abs(torch.matmul(ori_E, x.t()).t() - ori_f.unsqueeze(0))
-        if torch.sum(cv_Ab[cv_Ab > 0]) + torch.sum(cv_Cd[cv_Cd > 0]) + torch.sum(cv_Ef[cv_Ef > 0]) > 0.1 * batch_size:
+        if not no_warning and \
+                torch.sum(cv_Ab[cv_Ab > 0]) + torch.sum(cv_Cd[cv_Cd > 0]) + torch.sum(cv_Ef[cv_Ef > 0]) > 0.1 * batch_size:
             print('Warning: non-zero constraint violation within max iterations. Add more iterations or infeasible?',
                   file=sys.stderr)
 
     return x
 
 
 if __name__ == '__main__':
```

### Comparing `LinSATNet-0.0.7/LinSATNet.egg-info/PKG-INFO` & `LinSATNet-0.0.8/LinSATNet.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LinSATNet
-Version: 0.0.7
+Version: 0.0.8
 Summary: LinSATNet offers a neural network layer to enforce the satisfiability of positive linear constraints to the output of neural networks. The gradient through the layer is exactly computed. This package now works with PyTorch.
 Home-page: https://github.com/Thinklab-SJTU/LinSATNet
 Author: Runzhong Wang
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Environment :: GPU :: NVIDIA CUDA
```

### Comparing `LinSATNet-0.0.7/PKG-INFO` & `LinSATNet-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LinSATNet
-Version: 0.0.7
+Version: 0.0.8
 Summary: LinSATNet offers a neural network layer to enforce the satisfiability of positive linear constraints to the output of neural networks. The gradient through the layer is exactly computed. This package now works with PyTorch.
 Home-page: https://github.com/Thinklab-SJTU/LinSATNet
 Author: Runzhong Wang
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Environment :: GPU :: NVIDIA CUDA
```

### Comparing `LinSATNet-0.0.7/README.md` & `LinSATNet-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `LinSATNet-0.0.7/setup.py` & `LinSATNet-0.0.8/setup.py`

 * *Files identical despite different names*

