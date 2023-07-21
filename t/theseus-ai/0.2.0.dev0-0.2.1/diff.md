# Comparing `tmp/theseus-ai-0.2.0.dev0.tar.gz` & `tmp/theseus-ai-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "theseus-ai-0.2.0.dev0.tar", last modified: Fri Jun 16 22:24:47 2023, max compression
+gzip compressed data, was "theseus-ai-0.2.1.tar", last modified: Fri Jul 21 04:31:40 2023, max compression
```

## Comparing `theseus-ai-0.2.0.dev0.tar` & `theseus-ai-0.2.1.tar`

### file list

```diff
@@ -1,149 +1,140 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 22:24:47.675665 theseus-ai-0.2.0.dev0/
--rw-r--r--   0 root         (0) root         (0)     1088 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       91 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    11635 2023-06-16 22:24:47.675665 theseus-ai-0.2.0.dev0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    11035 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 22:24:47.655664 theseus-ai-0.2.0.dev0/requirements/
--rw-r--r--   0 root         (0) root         (0)      192 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/requirements/dev.txt
--rw-r--r--   0 root         (0) root         (0)      174 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/requirements/docs.txt
--rw-r--r--   0 root         (0) root         (0)      111 2023-06-16 22:24:40.000000 theseus-ai-0.2.0.dev0/requirements/main.txt
--rw-r--r--   0 root         (0) root         (0)      482 2023-06-16 22:24:47.675665 theseus-ai-0.2.0.dev0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     6333 2023-06-16 22:24:40.000000 theseus-ai-0.2.0.dev0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 22:24:47.655664 theseus-ai-0.2.0.dev0/theseus/
--rw-r--r--   0 root         (0) root         (0)     2133 2023-06-16 22:24:41.000000 theseus-ai-0.2.0.dev0/theseus/__init__.py
--rw-r--r--   0 root         (0) root         (0)      334 2023-06-16 22:24:41.000000 theseus-ai-0.2.0.dev0/theseus/_version.py
--rw-r--r--   0 root         (0) root         (0)      627 2023-06-16 22:24:41.000000 theseus-ai-0.2.0.dev0/theseus/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 22:24:47.655664 theseus-ai-0.2.0.dev0/theseus/core/
--rw-r--r--   0 root         (0) root         (0)      624 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16303 2023-06-16 22:24:41.000000 theseus-ai-0.2.0.dev0/theseus/core/cost_function.py
--rw-r--r--   0 root         (0) root         (0)     4984 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/core/cost_weight.py
--rw-r--r--   0 root         (0) root         (0)    30933 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/core/objective.py
--rw-r--r--   0 root         (0) root         (0)     7188 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/core/robust_cost_function.py
--rw-r--r--   0 root         (0) root         (0)     1606 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/core/robust_loss.py
--rw-r--r--   0 root         (0) root         (0)     6417 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/core/theseus_function.py
--rw-r--r--   0 root         (0) root         (0)     4800 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/core/variable.py
--rw-r--r--   0 root         (0) root         (0)    20320 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/core/vectorizer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 22:24:47.655664 theseus-ai-0.2.0.dev0/theseus/embodied/
--rw-r--r--   0 root         (0) root         (0)      581 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/embodied/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 22:24:47.659664 theseus-ai-0.2.0.dev0/theseus/embodied/collision/
--rw-r--r--   0 root         (0) root         (0)      329 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/embodied/collision/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3616 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/embodied/collision/collision.py
--rw-r--r--   0 root         (0) root         (0)     4906 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/embodied/collision/eff_obj_contact.py
--rw-r--r--   0 root         (0) root         (0)     9043 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/embodied/collision/signed_distance_field.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 22:24:47.659664 theseus-ai-0.2.0.dev0/theseus/embodied/kinematics/
--rw-r--r--   0 root         (0) root         (0)      257 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/embodied/kinematics/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3894 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/embodied/kinematics/kinematics_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 22:24:47.659664 theseus-ai-0.2.0.dev0/theseus/embodied/measurements/
--rw-r--r--   0 root         (0) root         (0)      301 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/embodied/measurements/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1818 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/embodied/measurements/between.py
--rw-r--r--   0 root         (0) root         (0)     2730 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/embodied/measurements/moving_frame_between.py
--rw-r--r--   0 root         (0) root         (0)     4090 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/embodied/measurements/reprojection.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 22:24:47.659664 theseus-ai-0.2.0.dev0/theseus/embodied/misc/
--rw-r--r--   0 root         (0) root         (0)      213 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/embodied/misc/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1564 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/embodied/misc/local_cost_fn.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 22:24:47.659664 theseus-ai-0.2.0.dev0/theseus/embodied/motionmodel/
--rw-r--r--   0 root         (0) root         (0)      365 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/embodied/motionmodel/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7715 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/embodied/motionmodel/double_integrator.py
--rw-r--r--   0 root         (0) root         (0)     6957 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/embodied/motionmodel/misc.py
--rw-r--r--   0 root         (0) root         (0)    11526 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/embodied/motionmodel/quasi_static_pushing_planar.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 22:24:47.663664 theseus-ai-0.2.0.dev0/theseus/extlib/
--rw-r--r--   0 root         (0) root         (0)      179 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/extlib/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14114 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/extlib/baspacho_solver.cpp
--rw-r--r--   0 root         (0) root         (0)     3751 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/extlib/baspacho_solver.h
--rw-r--r--   0 root         (0) root         (0)    12381 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/extlib/baspacho_solver_cuda.cu
--rw-r--r--   0 root         (0) root         (0)    16013 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/extlib/cusolver_lu_solver.cpp
--rw-r--r--   0 root         (0) root         (0)     3140 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/extlib/cusolver_sp_defs.cpp
--rw-r--r--   0 root         (0) root         (0)      744 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/extlib/cusolver_sp_defs.h
--rw-r--r--   0 root         (0) root         (0)    14555 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/extlib/mat_mult.cu
--rw-r--r--   0 root         (0) root         (0)     1186 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/extlib/utils.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 22:24:47.663664 theseus-ai-0.2.0.dev0/theseus/geometry/
--rw-r--r--   0 root         (0) root         (0)      911 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/geometry/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7224 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/geometry/lie_group.py
--rw-r--r--   0 root         (0) root         (0)     2094 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/geometry/lie_group_check.py
--rw-r--r--   0 root         (0) root         (0)     5689 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/geometry/manifold.py
--rw-r--r--   0 root         (0) root         (0)     7322 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/geometry/point_types.py
--rw-r--r--   0 root         (0) root         (0)    16493 2023-06-16 22:24:41.000000 theseus-ai-0.2.0.dev0/theseus/geometry/se2.py
--rw-r--r--   0 root         (0) root         (0)    10894 2023-06-16 22:24:41.000000 theseus-ai-0.2.0.dev0/theseus/geometry/se3.py
--rw-r--r--   0 root         (0) root         (0)    11454 2023-06-16 22:24:41.000000 theseus-ai-0.2.0.dev0/theseus/geometry/so2.py
--rw-r--r--   0 root         (0) root         (0)    11324 2023-06-16 22:24:41.000000 theseus-ai-0.2.0.dev0/theseus/geometry/so3.py
--rw-r--r--   0 root         (0) root         (0)     2683 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/geometry/utils.py
--rw-r--r--   0 root         (0) root         (0)     9405 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/geometry/vector.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 22:24:47.663664 theseus-ai-0.2.0.dev0/theseus/labs/
--rw-r--r--   0 root         (0) root         (0)      179 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/labs/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 22:24:47.663664 theseus-ai-0.2.0.dev0/theseus/labs/embodied/
--rw-r--r--   0 root         (0) root         (0)      179 2023-06-16 22:24:41.000000 theseus-ai-0.2.0.dev0/theseus/labs/embodied/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 22:24:47.663664 theseus-ai-0.2.0.dev0/theseus/labs/embodied/robot/
--rw-r--r--   0 root         (0) root         (0)      179 2023-06-16 22:24:41.000000 theseus-ai-0.2.0.dev0/theseus/labs/embodied/robot/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4922 2023-06-16 22:24:41.000000 theseus-ai-0.2.0.dev0/theseus/labs/embodied/robot/forward_kinematics.py
--rw-r--r--   0 root         (0) root         (0)    15442 2023-06-16 22:24:41.000000 theseus-ai-0.2.0.dev0/theseus/labs/embodied/robot/joint.py
--rw-r--r--   0 root         (0) root         (0)     8668 2023-06-16 22:24:41.000000 theseus-ai-0.2.0.dev0/theseus/labs/embodied/robot/robot.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 22:24:47.667664 theseus-ai-0.2.0.dev0/theseus/optimizer/
--rw-r--r--   0 root         (0) root         (0)      505 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/optimizer/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 22:24:47.667664 theseus-ai-0.2.0.dev0/theseus/optimizer/autograd/
--rw-r--r--   0 root         (0) root         (0)      454 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/optimizer/autograd/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5948 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/optimizer/autograd/baspacho_sparse_autograd.py
--rw-r--r--   0 root         (0) root         (0)     5365 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/optimizer/autograd/cholmod_sparse_autograd.py
--rw-r--r--   0 root         (0) root         (0)     1710 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/optimizer/autograd/common.py
--rw-r--r--   0 root         (0) root         (0)     7572 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/optimizer/autograd/lu_cuda_sparse_autograd.py
--rw-r--r--   0 root         (0) root         (0)     2691 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/optimizer/dense_linearization.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 22:24:47.667664 theseus-ai-0.2.0.dev0/theseus/optimizer/linear/
--rw-r--r--   0 root         (0) root         (0)      520 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/optimizer/linear/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5161 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/optimizer/linear/baspacho_sparse_solver.py
--rw-r--r--   0 root         (0) root         (0)     2648 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/optimizer/linear/cholmod_sparse_solver.py
--rw-r--r--   0 root         (0) root         (0)     5681 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/optimizer/linear/dense_solver.py
--rw-r--r--   0 root         (0) root         (0)     2630 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/optimizer/linear/linear_optimizer.py
--rw-r--r--   0 root         (0) root         (0)     1107 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/optimizer/linear/linear_solver.py
--rw-r--r--   0 root         (0) root         (0)     6892 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/optimizer/linear/lu_cuda_sparse_solver.py
--rw-r--r--   0 root         (0) root         (0)     1221 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/optimizer/linear/utils.py
--rw-r--r--   0 root         (0) root         (0)     1346 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/optimizer/linear_system.py
--rw-r--r--   0 root         (0) root         (0)     2437 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/optimizer/linearization.py
--rw-r--r--   0 root         (0) root         (0)     6184 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/optimizer/manifold_gaussian.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 22:24:47.671664 theseus-ai-0.2.0.dev0/theseus/optimizer/nonlinear/
--rw-r--r--   0 root         (0) root         (0)      584 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/optimizer/nonlinear/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8421 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/optimizer/nonlinear/dcem.py
--rw-r--r--   0 root         (0) root         (0)     4354 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/optimizer/nonlinear/dogleg.py
--rw-r--r--   0 root         (0) root         (0)     1591 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/optimizer/nonlinear/gauss_newton.py
--rw-r--r--   0 root         (0) root         (0)     7009 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/optimizer/nonlinear/levenberg_marquardt.py
--rw-r--r--   0 root         (0) root         (0)    16237 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/optimizer/nonlinear/nonlinear_least_squares.py
--rw-r--r--   0 root         (0) root         (0)    10821 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/optimizer/nonlinear/nonlinear_optimizer.py
--rw-r--r--   0 root         (0) root         (0)     5696 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/optimizer/nonlinear/trust_region.py
--rw-r--r--   0 root         (0) root         (0)     1740 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/optimizer/optimizer.py
--rw-r--r--   0 root         (0) root         (0)     8226 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/optimizer/sparse_linearization.py
--rw-r--r--   0 root         (0) root         (0)     2068 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/optimizer/variable_ordering.py
--rw-r--r--   0 root         (0) root         (0)     2331 2023-06-16 22:24:41.000000 theseus-ai-0.2.0.dev0/theseus/options.py
--rw-r--r--   0 root         (0) root         (0)    12958 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/theseus_layer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 22:24:47.671664 theseus-ai-0.2.0.dev0/theseus/third_party/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/third_party/__init__.py
--rw-r--r--   0 root         (0) root         (0)    28031 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/third_party/easyaug.py
--rwxr-xr-x   0 root         (0) root         (0)     6703 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/third_party/lml.py
--rw-r--r--   0 root         (0) root         (0)     2040 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/third_party/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 22:24:47.671664 theseus-ai-0.2.0.dev0/theseus/utils/
--rw-r--r--   0 root         (0) root         (0)      499 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/utils/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 22:24:47.671664 theseus-ai-0.2.0.dev0/theseus/utils/examples/
--rw-r--r--   0 root         (0) root         (0)     1526 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/utils/examples/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 22:24:47.671664 theseus-ai-0.2.0.dev0/theseus/utils/examples/bundle_adjustment/
--rw-r--r--   0 root         (0) root         (0)      244 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/utils/examples/bundle_adjustment/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12392 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/utils/examples/bundle_adjustment/data.py
--rw-r--r--   0 root         (0) root         (0)     2220 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/utils/examples/bundle_adjustment/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 22:24:47.675665 theseus-ai-0.2.0.dev0/theseus/utils/examples/motion_planning/
--rw-r--r--   0 root         (0) root         (0)      435 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/utils/examples/motion_planning/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9168 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/utils/examples/motion_planning/misc.py
--rw-r--r--   0 root         (0) root         (0)     9771 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/utils/examples/motion_planning/models.py
--rw-r--r--   0 root         (0) root         (0)    19745 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/utils/examples/motion_planning/motion_planner.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 22:24:47.675665 theseus-ai-0.2.0.dev0/theseus/utils/examples/pose_graph/
--rw-r--r--   0 root         (0) root         (0)      308 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/utils/examples/pose_graph/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16407 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/utils/examples/pose_graph/dataset.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 22:24:47.675665 theseus-ai-0.2.0.dev0/theseus/utils/examples/tactile_pose_estimation/
--rw-r--r--   0 root         (0) root         (0)      510 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/utils/examples/tactile_pose_estimation/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10221 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/utils/examples/tactile_pose_estimation/misc.py
--rw-r--r--   0 root         (0) root         (0)    10050 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/utils/examples/tactile_pose_estimation/models.py
--rw-r--r--   0 root         (0) root         (0)     9304 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/utils/examples/tactile_pose_estimation/pose_estimator.py
--rw-r--r--   0 root         (0) root         (0)    12465 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/utils/examples/tactile_pose_estimation/trainer.py
--rw-r--r--   0 root         (0) root         (0)     8649 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/utils/sparse_matrix_utils.py
--rw-r--r--   0 root         (0) root         (0)     8089 2023-06-16 22:24:38.000000 theseus-ai-0.2.0.dev0/theseus/utils/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 22:24:47.675665 theseus-ai-0.2.0.dev0/theseus_ai.egg-info/
--rw-r--r--   0 root         (0) root         (0)    11635 2023-06-16 22:24:47.000000 theseus-ai-0.2.0.dev0/theseus_ai.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4424 2023-06-16 22:24:47.000000 theseus-ai-0.2.0.dev0/theseus_ai.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-16 22:24:47.000000 theseus-ai-0.2.0.dev0/theseus_ai.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      424 2023-06-16 22:24:47.000000 theseus-ai-0.2.0.dev0/theseus_ai.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-16 22:24:47.000000 theseus-ai-0.2.0.dev0/theseus_ai.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 04:31:40.299487 theseus-ai-0.2.1/
+-rw-r--r--   0 root         (0) root         (0)     1088 2023-07-21 04:31:31.000000 theseus-ai-0.2.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       91 2023-07-21 04:31:31.000000 theseus-ai-0.2.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    11980 2023-07-21 04:31:40.299487 theseus-ai-0.2.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    11385 2023-07-21 04:31:31.000000 theseus-ai-0.2.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 04:31:40.279486 theseus-ai-0.2.1/requirements/
+-rw-r--r--   0 root         (0) root         (0)      193 2023-07-21 04:31:31.000000 theseus-ai-0.2.1/requirements/dev.txt
+-rw-r--r--   0 root         (0) root         (0)      174 2023-07-21 04:31:31.000000 theseus-ai-0.2.1/requirements/docs.txt
+-rw-r--r--   0 root         (0) root         (0)      121 2023-07-21 04:31:34.000000 theseus-ai-0.2.1/requirements/main.txt
+-rw-r--r--   0 root         (0) root         (0)      672 2023-07-21 04:31:40.299487 theseus-ai-0.2.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     6355 2023-07-21 04:31:34.000000 theseus-ai-0.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 04:31:40.279486 theseus-ai-0.2.1/theseus/
+-rw-r--r--   0 root         (0) root         (0)     2193 2023-07-21 04:31:31.000000 theseus-ai-0.2.1/theseus/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1119 2023-07-21 04:31:31.000000 theseus-ai-0.2.1/theseus/_version.py
+-rw-r--r--   0 root         (0) root         (0)      627 2023-07-21 04:31:31.000000 theseus-ai-0.2.1/theseus/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 04:31:40.283486 theseus-ai-0.2.1/theseus/core/
+-rw-r--r--   0 root         (0) root         (0)      624 2023-07-21 04:31:31.000000 theseus-ai-0.2.1/theseus/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16372 2023-07-21 04:31:31.000000 theseus-ai-0.2.1/theseus/core/cost_function.py
+-rw-r--r--   0 root         (0) root         (0)     4984 2023-07-21 04:31:31.000000 theseus-ai-0.2.1/theseus/core/cost_weight.py
+-rw-r--r--   0 root         (0) root         (0)    41201 2023-07-21 04:31:31.000000 theseus-ai-0.2.1/theseus/core/objective.py
+-rw-r--r--   0 root         (0) root         (0)     7188 2023-07-21 04:31:31.000000 theseus-ai-0.2.1/theseus/core/robust_cost_function.py
+-rw-r--r--   0 root         (0) root         (0)     1606 2023-07-21 04:31:31.000000 theseus-ai-0.2.1/theseus/core/robust_loss.py
+-rw-r--r--   0 root         (0) root         (0)     6417 2023-07-21 04:31:31.000000 theseus-ai-0.2.1/theseus/core/theseus_function.py
+-rw-r--r--   0 root         (0) root         (0)     4801 2023-07-21 04:31:31.000000 theseus-ai-0.2.1/theseus/core/variable.py
+-rw-r--r--   0 root         (0) root         (0)    20320 2023-07-21 04:31:31.000000 theseus-ai-0.2.1/theseus/core/vectorizer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 04:31:40.283486 theseus-ai-0.2.1/theseus/embodied/
+-rw-r--r--   0 root         (0) root         (0)      581 2023-07-21 04:31:31.000000 theseus-ai-0.2.1/theseus/embodied/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 04:31:40.283486 theseus-ai-0.2.1/theseus/embodied/collision/
+-rw-r--r--   0 root         (0) root         (0)      329 2023-07-21 04:31:31.000000 theseus-ai-0.2.1/theseus/embodied/collision/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3616 2023-07-21 04:31:31.000000 theseus-ai-0.2.1/theseus/embodied/collision/collision.py
+-rw-r--r--   0 root         (0) root         (0)     4906 2023-07-21 04:31:31.000000 theseus-ai-0.2.1/theseus/embodied/collision/eff_obj_contact.py
+-rw-r--r--   0 root         (0) root         (0)     9043 2023-07-21 04:31:31.000000 theseus-ai-0.2.1/theseus/embodied/collision/signed_distance_field.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 04:31:40.283486 theseus-ai-0.2.1/theseus/embodied/kinematics/
+-rw-r--r--   0 root         (0) root         (0)      257 2023-07-21 04:31:31.000000 theseus-ai-0.2.1/theseus/embodied/kinematics/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4631 2023-07-21 04:31:31.000000 theseus-ai-0.2.1/theseus/embodied/kinematics/kinematics_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 04:31:40.283486 theseus-ai-0.2.1/theseus/embodied/measurements/
+-rw-r--r--   0 root         (0) root         (0)      301 2023-07-21 04:31:31.000000 theseus-ai-0.2.1/theseus/embodied/measurements/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1818 2023-07-21 04:31:31.000000 theseus-ai-0.2.1/theseus/embodied/measurements/between.py
+-rw-r--r--   0 root         (0) root         (0)     2730 2023-07-21 04:31:31.000000 theseus-ai-0.2.1/theseus/embodied/measurements/moving_frame_between.py
+-rw-r--r--   0 root         (0) root         (0)     4090 2023-07-21 04:31:31.000000 theseus-ai-0.2.1/theseus/embodied/measurements/reprojection.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 04:31:40.283486 theseus-ai-0.2.1/theseus/embodied/misc/
+-rw-r--r--   0 root         (0) root         (0)      213 2023-07-21 04:31:31.000000 theseus-ai-0.2.1/theseus/embodied/misc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1564 2023-07-21 04:31:31.000000 theseus-ai-0.2.1/theseus/embodied/misc/local_cost_fn.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 04:31:40.283486 theseus-ai-0.2.1/theseus/embodied/motionmodel/
+-rw-r--r--   0 root         (0) root         (0)      365 2023-07-21 04:31:31.000000 theseus-ai-0.2.1/theseus/embodied/motionmodel/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7715 2023-07-21 04:31:31.000000 theseus-ai-0.2.1/theseus/embodied/motionmodel/double_integrator.py
+-rw-r--r--   0 root         (0) root         (0)     6957 2023-07-21 04:31:31.000000 theseus-ai-0.2.1/theseus/embodied/motionmodel/misc.py
+-rw-r--r--   0 root         (0) root         (0)    11526 2023-07-21 04:31:31.000000 theseus-ai-0.2.1/theseus/embodied/motionmodel/quasi_static_pushing_planar.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 04:31:40.287486 theseus-ai-0.2.1/theseus/extlib/
+-rw-r--r--   0 root         (0) root         (0)      179 2023-07-21 04:31:31.000000 theseus-ai-0.2.1/theseus/extlib/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14114 2023-07-21 04:31:31.000000 theseus-ai-0.2.1/theseus/extlib/baspacho_solver.cpp
+-rw-r--r--   0 root         (0) root         (0)     3751 2023-07-21 04:31:31.000000 theseus-ai-0.2.1/theseus/extlib/baspacho_solver.h
+-rw-r--r--   0 root         (0) root         (0)    12381 2023-07-21 04:31:31.000000 theseus-ai-0.2.1/theseus/extlib/baspacho_solver_cuda.cu
+-rw-r--r--   0 root         (0) root         (0)    16013 2023-07-21 04:31:31.000000 theseus-ai-0.2.1/theseus/extlib/cusolver_lu_solver.cpp
+-rw-r--r--   0 root         (0) root         (0)     3140 2023-07-21 04:31:31.000000 theseus-ai-0.2.1/theseus/extlib/cusolver_sp_defs.cpp
+-rw-r--r--   0 root         (0) root         (0)      744 2023-07-21 04:31:31.000000 theseus-ai-0.2.1/theseus/extlib/cusolver_sp_defs.h
+-rw-r--r--   0 root         (0) root         (0)    14555 2023-07-21 04:31:31.000000 theseus-ai-0.2.1/theseus/extlib/mat_mult.cu
+-rw-r--r--   0 root         (0) root         (0)     1186 2023-07-21 04:31:31.000000 theseus-ai-0.2.1/theseus/extlib/utils.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 04:31:40.287486 theseus-ai-0.2.1/theseus/geometry/
+-rw-r--r--   0 root         (0) root         (0)      911 2023-07-21 04:31:31.000000 theseus-ai-0.2.1/theseus/geometry/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7397 2023-07-21 04:31:31.000000 theseus-ai-0.2.1/theseus/geometry/lie_group.py
+-rw-r--r--   0 root         (0) root         (0)     2094 2023-07-21 04:31:31.000000 theseus-ai-0.2.1/theseus/geometry/lie_group_check.py
+-rw-r--r--   0 root         (0) root         (0)     5856 2023-07-21 04:31:31.000000 theseus-ai-0.2.1/theseus/geometry/manifold.py
+-rw-r--r--   0 root         (0) root         (0)     7323 2023-07-21 04:31:31.000000 theseus-ai-0.2.1/theseus/geometry/point_types.py
+-rw-r--r--   0 root         (0) root         (0)    16843 2023-07-21 04:31:31.000000 theseus-ai-0.2.1/theseus/geometry/se2.py
+-rw-r--r--   0 root         (0) root         (0)    10331 2023-07-21 04:31:31.000000 theseus-ai-0.2.1/theseus/geometry/se3.py
+-rw-r--r--   0 root         (0) root         (0)    11632 2023-07-21 04:31:31.000000 theseus-ai-0.2.1/theseus/geometry/so2.py
+-rw-r--r--   0 root         (0) root         (0)    11165 2023-07-21 04:31:31.000000 theseus-ai-0.2.1/theseus/geometry/so3.py
+-rw-r--r--   0 root         (0) root         (0)     2683 2023-07-21 04:31:31.000000 theseus-ai-0.2.1/theseus/geometry/utils.py
+-rw-r--r--   0 root         (0) root         (0)     9405 2023-07-21 04:31:31.000000 theseus-ai-0.2.1/theseus/geometry/vector.py
+-rw-r--r--   0 root         (0) root         (0)     2477 2023-07-21 04:31:31.000000 theseus-ai-0.2.1/theseus/global_params.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 04:31:40.291487 theseus-ai-0.2.1/theseus/optimizer/
+-rw-r--r--   0 root         (0) root         (0)      505 2023-07-21 04:31:31.000000 theseus-ai-0.2.1/theseus/optimizer/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 04:31:40.291487 theseus-ai-0.2.1/theseus/optimizer/autograd/
+-rw-r--r--   0 root         (0) root         (0)      454 2023-07-21 04:31:31.000000 theseus-ai-0.2.1/theseus/optimizer/autograd/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5950 2023-07-21 04:31:31.000000 theseus-ai-0.2.1/theseus/optimizer/autograd/baspacho_sparse_autograd.py
+-rw-r--r--   0 root         (0) root         (0)     5365 2023-07-21 04:31:31.000000 theseus-ai-0.2.1/theseus/optimizer/autograd/cholmod_sparse_autograd.py
+-rw-r--r--   0 root         (0) root         (0)     1710 2023-07-21 04:31:31.000000 theseus-ai-0.2.1/theseus/optimizer/autograd/common.py
+-rw-r--r--   0 root         (0) root         (0)     7573 2023-07-21 04:31:31.000000 theseus-ai-0.2.1/theseus/optimizer/autograd/lu_cuda_sparse_autograd.py
+-rw-r--r--   0 root         (0) root         (0)     2691 2023-07-21 04:31:31.000000 theseus-ai-0.2.1/theseus/optimizer/dense_linearization.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 04:31:40.291487 theseus-ai-0.2.1/theseus/optimizer/linear/
+-rw-r--r--   0 root         (0) root         (0)      520 2023-07-21 04:31:31.000000 theseus-ai-0.2.1/theseus/optimizer/linear/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5161 2023-07-21 04:31:31.000000 theseus-ai-0.2.1/theseus/optimizer/linear/baspacho_sparse_solver.py
+-rw-r--r--   0 root         (0) root         (0)     2648 2023-07-21 04:31:31.000000 theseus-ai-0.2.1/theseus/optimizer/linear/cholmod_sparse_solver.py
+-rw-r--r--   0 root         (0) root         (0)     5681 2023-07-21 04:31:31.000000 theseus-ai-0.2.1/theseus/optimizer/linear/dense_solver.py
+-rw-r--r--   0 root         (0) root         (0)     2630 2023-07-21 04:31:31.000000 theseus-ai-0.2.1/theseus/optimizer/linear/linear_optimizer.py
+-rw-r--r--   0 root         (0) root         (0)     1107 2023-07-21 04:31:31.000000 theseus-ai-0.2.1/theseus/optimizer/linear/linear_solver.py
+-rw-r--r--   0 root         (0) root         (0)     6892 2023-07-21 04:31:31.000000 theseus-ai-0.2.1/theseus/optimizer/linear/lu_cuda_sparse_solver.py
+-rw-r--r--   0 root         (0) root         (0)     1223 2023-07-21 04:31:31.000000 theseus-ai-0.2.1/theseus/optimizer/linear/utils.py
+-rw-r--r--   0 root         (0) root         (0)     1346 2023-07-21 04:31:31.000000 theseus-ai-0.2.1/theseus/optimizer/linear_system.py
+-rw-r--r--   0 root         (0) root         (0)     2437 2023-07-21 04:31:31.000000 theseus-ai-0.2.1/theseus/optimizer/linearization.py
+-rw-r--r--   0 root         (0) root         (0)     6184 2023-07-21 04:31:31.000000 theseus-ai-0.2.1/theseus/optimizer/manifold_gaussian.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 04:31:40.295487 theseus-ai-0.2.1/theseus/optimizer/nonlinear/
+-rw-r--r--   0 root         (0) root         (0)      584 2023-07-21 04:31:31.000000 theseus-ai-0.2.1/theseus/optimizer/nonlinear/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8421 2023-07-21 04:31:31.000000 theseus-ai-0.2.1/theseus/optimizer/nonlinear/dcem.py
+-rw-r--r--   0 root         (0) root         (0)     4354 2023-07-21 04:31:31.000000 theseus-ai-0.2.1/theseus/optimizer/nonlinear/dogleg.py
+-rw-r--r--   0 root         (0) root         (0)     1591 2023-07-21 04:31:31.000000 theseus-ai-0.2.1/theseus/optimizer/nonlinear/gauss_newton.py
+-rw-r--r--   0 root         (0) root         (0)     7009 2023-07-21 04:31:31.000000 theseus-ai-0.2.1/theseus/optimizer/nonlinear/levenberg_marquardt.py
+-rw-r--r--   0 root         (0) root         (0)    16544 2023-07-21 04:31:31.000000 theseus-ai-0.2.1/theseus/optimizer/nonlinear/nonlinear_least_squares.py
+-rw-r--r--   0 root         (0) root         (0)    10821 2023-07-21 04:31:31.000000 theseus-ai-0.2.1/theseus/optimizer/nonlinear/nonlinear_optimizer.py
+-rw-r--r--   0 root         (0) root         (0)     5695 2023-07-21 04:31:31.000000 theseus-ai-0.2.1/theseus/optimizer/nonlinear/trust_region.py
+-rw-r--r--   0 root         (0) root         (0)     1740 2023-07-21 04:31:31.000000 theseus-ai-0.2.1/theseus/optimizer/optimizer.py
+-rw-r--r--   0 root         (0) root         (0)     8226 2023-07-21 04:31:31.000000 theseus-ai-0.2.1/theseus/optimizer/sparse_linearization.py
+-rw-r--r--   0 root         (0) root         (0)     2068 2023-07-21 04:31:31.000000 theseus-ai-0.2.1/theseus/optimizer/variable_ordering.py
+-rw-r--r--   0 root         (0) root         (0)    12958 2023-07-21 04:31:31.000000 theseus-ai-0.2.1/theseus/theseus_layer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 04:31:40.295487 theseus-ai-0.2.1/theseus/third_party/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 04:31:31.000000 theseus-ai-0.2.1/theseus/third_party/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    28031 2023-07-21 04:31:31.000000 theseus-ai-0.2.1/theseus/third_party/easyaug.py
+-rwxr-xr-x   0 root         (0) root         (0)     6655 2023-07-21 04:31:31.000000 theseus-ai-0.2.1/theseus/third_party/lml.py
+-rw-r--r--   0 root         (0) root         (0)     2040 2023-07-21 04:31:31.000000 theseus-ai-0.2.1/theseus/third_party/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 04:31:40.295487 theseus-ai-0.2.1/theseus/utils/
+-rw-r--r--   0 root         (0) root         (0)      513 2023-07-21 04:31:31.000000 theseus-ai-0.2.1/theseus/utils/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 04:31:40.295487 theseus-ai-0.2.1/theseus/utils/examples/
+-rw-r--r--   0 root         (0) root         (0)     1526 2023-07-21 04:31:31.000000 theseus-ai-0.2.1/theseus/utils/examples/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 04:31:40.295487 theseus-ai-0.2.1/theseus/utils/examples/bundle_adjustment/
+-rw-r--r--   0 root         (0) root         (0)      244 2023-07-21 04:31:31.000000 theseus-ai-0.2.1/theseus/utils/examples/bundle_adjustment/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12392 2023-07-21 04:31:31.000000 theseus-ai-0.2.1/theseus/utils/examples/bundle_adjustment/data.py
+-rw-r--r--   0 root         (0) root         (0)     2220 2023-07-21 04:31:31.000000 theseus-ai-0.2.1/theseus/utils/examples/bundle_adjustment/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 04:31:40.295487 theseus-ai-0.2.1/theseus/utils/examples/motion_planning/
+-rw-r--r--   0 root         (0) root         (0)      435 2023-07-21 04:31:31.000000 theseus-ai-0.2.1/theseus/utils/examples/motion_planning/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9168 2023-07-21 04:31:31.000000 theseus-ai-0.2.1/theseus/utils/examples/motion_planning/misc.py
+-rw-r--r--   0 root         (0) root         (0)     9771 2023-07-21 04:31:31.000000 theseus-ai-0.2.1/theseus/utils/examples/motion_planning/models.py
+-rw-r--r--   0 root         (0) root         (0)    19745 2023-07-21 04:31:31.000000 theseus-ai-0.2.1/theseus/utils/examples/motion_planning/motion_planner.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 04:31:40.299487 theseus-ai-0.2.1/theseus/utils/examples/pose_graph/
+-rw-r--r--   0 root         (0) root         (0)      308 2023-07-21 04:31:31.000000 theseus-ai-0.2.1/theseus/utils/examples/pose_graph/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16473 2023-07-21 04:31:31.000000 theseus-ai-0.2.1/theseus/utils/examples/pose_graph/dataset.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 04:31:40.299487 theseus-ai-0.2.1/theseus/utils/examples/tactile_pose_estimation/
+-rw-r--r--   0 root         (0) root         (0)      689 2023-07-21 04:31:31.000000 theseus-ai-0.2.1/theseus/utils/examples/tactile_pose_estimation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10400 2023-07-21 04:31:31.000000 theseus-ai-0.2.1/theseus/utils/examples/tactile_pose_estimation/misc.py
+-rw-r--r--   0 root         (0) root         (0)    10229 2023-07-21 04:31:31.000000 theseus-ai-0.2.1/theseus/utils/examples/tactile_pose_estimation/models.py
+-rw-r--r--   0 root         (0) root         (0)     9483 2023-07-21 04:31:31.000000 theseus-ai-0.2.1/theseus/utils/examples/tactile_pose_estimation/pose_estimator.py
+-rw-r--r--   0 root         (0) root         (0)    12465 2023-07-21 04:31:31.000000 theseus-ai-0.2.1/theseus/utils/examples/tactile_pose_estimation/trainer.py
+-rw-r--r--   0 root         (0) root         (0)     8649 2023-07-21 04:31:31.000000 theseus-ai-0.2.1/theseus/utils/sparse_matrix_utils.py
+-rw-r--r--   0 root         (0) root         (0)     8771 2023-07-21 04:31:31.000000 theseus-ai-0.2.1/theseus/utils/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 04:31:40.299487 theseus-ai-0.2.1/theseus_ai.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    11980 2023-07-21 04:31:40.000000 theseus-ai-0.2.1/theseus_ai.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4335 2023-07-21 04:31:40.000000 theseus-ai-0.2.1/theseus_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 04:31:40.000000 theseus-ai-0.2.1/theseus_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-21 04:31:40.000000 theseus-ai-0.2.1/theseus_ai.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-21 04:31:40.000000 theseus-ai-0.2.1/theseus_ai.egg-info/top_level.txt
```

### Comparing `theseus-ai-0.2.0.dev0/LICENSE` & `theseus-ai-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `theseus-ai-0.2.0.dev0/PKG-INFO` & `theseus-ai-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: theseus-ai
-Version: 0.2.0.dev0
+Version: 0.2.1
 Summary: A library for differentiable nonlinear optimization.
 Home-page: https://github.com/facebookresearch/theseus
 Author: Meta Research
 Keywords: differentiable optimization,nonlinear least squares,factor graphs
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Science/Research
@@ -72,20 +72,22 @@
 -----
 
 ## Current Features
 
 ### Application agnostic interface
 Our implementation provides an easy to use interface to build custom optimization layers and plug them into any neural architecture. Following differentiable features are currently available:
 - [Second-order nonlinear optimizers](https://github.com/facebookresearch/theseus/tree/main/theseus/optimizer/nonlinear)
-    - Gauss-Newton, Levenberg–Marquardt
+    - Gauss-Newton (GN), Levenberg–Marquardt (LM), Trust Region, Dogleg
+- [Other nonlinear optimizers](https://github.com/facebookresearch/theseus/tree/main/theseus/optimizer/nonlinear)
+    - Cross Entropy Method (CEM)
 - [Linear solvers](https://github.com/facebookresearch/theseus/tree/main/theseus/optimizer/linear)
     - Dense: Cholesky, LU; Sparse: CHOLMOD, LU (GPU-only), [BaSpaCho](https://github.com/facebookresearch/baspacho)
 - [Commonly used costs](https://github.com/facebookresearch/theseus/tree/main/theseus/embodied), [AutoDiffCostFunction](https://github.com/facebookresearch/theseus/blob/main/theseus/core/cost_function.py), [RobustCostFunction](https://github.com/facebookresearch/theseus/blob/main/theseus/core/robust_cost_function.py)
-- [Lie groups](https://github.com/facebookresearch/theseus/tree/main/theseus/geometry)
-- [Robot kinematics](https://github.com/facebookresearch/theseus/blob/main/theseus/embodied/kinematics/kinematics_model.py)
+- [Lie groups](https://github.com/facebookresearch/theseus/tree/main/theseus/geometry) based on [torchlie](https://github.com/facebookresearch/theseus/tree/main/torchlie)
+- [Robot kinematics](https://github.com/facebookresearch/theseus/blob/main/theseus/embodied/kinematics) based on [torchkin](https://github.com/facebookresearch/theseus/tree/main/torchkin)
 
 ### Efficiency based design
 We support several features that improve computation times and memory consumption:
 - [Sparse linear solvers](https://github.com/facebookresearch/theseus/tree/main/theseus/optimizer/linear)
 - Batching and GPU acceleration
 - [Automatic vectorization](https://github.com/facebookresearch/theseus/blob/main/theseus/core/vectorizer.py)
 - [Backward modes](https://github.com/facebookresearch/theseus/blob/main/theseus/optimizer/nonlinear/nonlinear_optimizer.py)
@@ -120,14 +122,15 @@
     ```bash
     git clone https://github.com/facebookresearch/theseus.git && cd theseus
     pip install -e .
     ```
     If you are interested in contributing to Theseus, instead install
     ```bash
     pip install -e ".[dev]"
+    pre-commit install
     ```
     and follow the more detailed instructions in [CONTRIBUTING](https://github.com/facebookresearch/theseus/blob/main/CONTRIBUTING.md).
 
 - **Installing BaSpaCho extensions from source**
 
     By default, installing from source doesn't include our BaSpaCho sparse solver extension. For this, follow these steps:
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: theseus-ai Version: 0.2.0.dev0 Summary: A library
-for differentiable nonlinear optimization. Home-page: https://github.com/
+Metadata-Version: 2.1 Name: theseus-ai Version: 0.2.1 Summary: A library for
+differentiable nonlinear optimization. Home-page: https://github.com/
 facebookresearch/theseus Author: Meta Research Keywords: differentiable
 optimization,nonlinear least squares,factor graphs Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Science/Research Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Requires-Python: >=3.8
 Description-Content-Type: text/markdown Provides-Extra: dev License-File:
 LICENSE ![](https://raw.githubusercontent.com/facebookresearch/theseus/main/
@@ -23,28 +23,32 @@
 by differentiating through the optimizer which allows neural models to train on
 the final task loss, while also taking advantage of priors captured by the
 optimizer. ----- ## Current Features ### Application agnostic interface Our
 implementation provides an easy to use interface to build custom optimization
 layers and plug them into any neural architecture. Following differentiable
 features are currently available: - [Second-order nonlinear optimizers](https:/
 /github.com/facebookresearch/theseus/tree/main/theseus/optimizer/nonlinear) -
-Gauss-Newton, LevenbergâMarquardt - [Linear solvers](https://github.com/
-facebookresearch/theseus/tree/main/theseus/optimizer/linear) - Dense: Cholesky,
-LU; Sparse: CHOLMOD, LU (GPU-only), [BaSpaCho](https://github.com/
-facebookresearch/baspacho) - [Commonly used costs](https://github.com/
-facebookresearch/theseus/tree/main/theseus/embodied), [AutoDiffCostFunction]
-(https://github.com/facebookresearch/theseus/blob/main/theseus/core/
-cost_function.py), [RobustCostFunction](https://github.com/facebookresearch/
-theseus/blob/main/theseus/core/robust_cost_function.py) - [Lie groups](https://
-github.com/facebookresearch/theseus/tree/main/theseus/geometry) - [Robot
-kinematics](https://github.com/facebookresearch/theseus/blob/main/theseus/
-embodied/kinematics/kinematics_model.py) ### Efficiency based design We support
-several features that improve computation times and memory consumption: -
-[Sparse linear solvers](https://github.com/facebookresearch/theseus/tree/main/
-theseus/optimizer/linear) - Batching and GPU acceleration - [Automatic
+Gauss-Newton (GN), LevenbergâMarquardt (LM), Trust Region, Dogleg - [Other
+nonlinear optimizers](https://github.com/facebookresearch/theseus/tree/main/
+theseus/optimizer/nonlinear) - Cross Entropy Method (CEM) - [Linear solvers]
+(https://github.com/facebookresearch/theseus/tree/main/theseus/optimizer/
+linear) - Dense: Cholesky, LU; Sparse: CHOLMOD, LU (GPU-only), [BaSpaCho]
+(https://github.com/facebookresearch/baspacho) - [Commonly used costs](https://
+github.com/facebookresearch/theseus/tree/main/theseus/embodied),
+[AutoDiffCostFunction](https://github.com/facebookresearch/theseus/blob/main/
+theseus/core/cost_function.py), [RobustCostFunction](https://github.com/
+facebookresearch/theseus/blob/main/theseus/core/robust_cost_function.py) - [Lie
+groups](https://github.com/facebookresearch/theseus/tree/main/theseus/geometry)
+based on [torchlie](https://github.com/facebookresearch/theseus/tree/main/
+torchlie) - [Robot kinematics](https://github.com/facebookresearch/theseus/
+blob/main/theseus/embodied/kinematics) based on [torchkin](https://github.com/
+facebookresearch/theseus/tree/main/torchkin) ### Efficiency based design We
+support several features that improve computation times and memory consumption:
+- [Sparse linear solvers](https://github.com/facebookresearch/theseus/tree/
+main/theseus/optimizer/linear) - Batching and GPU acceleration - [Automatic
 vectorization](https://github.com/facebookresearch/theseus/blob/main/theseus/
 core/vectorizer.py) - [Backward modes](https://github.com/facebookresearch/
 theseus/blob/main/theseus/optimizer/nonlinear/nonlinear_optimizer.py) -
 Implicit, Truncated, Direct Loss Minimization ([DLM](https://github.com/
 facebookresearch/theseus/blob/main/theseus/theseus_layer.py)), Sampling ([LEO]
 (https://github.com/facebookresearch/theseus/blob/main/examples/
 state_estimation_2d.py)) ## Getting Started ### Prerequisites - We *strongly*
@@ -65,23 +69,23 @@
 theseus/blob/main/build_scripts/build_wheel.sh). Note that `pypi` installation
 doesn't include our experimental [Theseus Labs](https://github.com/
 facebookresearch/theseus/tree/main/theseus/labs). For this, please install from
 source. - #### **From source** The simplest way to install Theseus from source
 is by running the following (see further below to also include BaSpaCho)
 ```bash git clone https://github.com/facebookresearch/theseus.git && cd theseus
 pip install -e . ``` If you are interested in contributing to Theseus, instead
-install ```bash pip install -e ".[dev]" ``` and follow the more detailed
-instructions in [CONTRIBUTING](https://github.com/facebookresearch/theseus/
-blob/main/CONTRIBUTING.md). - **Installing BaSpaCho extensions from source** By
-default, installing from source doesn't include our BaSpaCho sparse solver
-extension. For this, follow these steps: 1. Compile BaSpaCho from source
-following instructions [here](https://github.com/facebookresearch/baspacho). We
-recommend using flags `-DBLA_STATIC=ON -DBUILD_SHARED_LIBS=OFF`. 2. Run ```bash
-git clone https://github.com/facebookresearch/theseus.git && cd theseus
-BASPACHO_ROOT_DIR=
+install ```bash pip install -e ".[dev]" pre-commit install ``` and follow the
+more detailed instructions in [CONTRIBUTING](https://github.com/
+facebookresearch/theseus/blob/main/CONTRIBUTING.md). - **Installing BaSpaCho
+extensions from source** By default, installing from source doesn't include our
+BaSpaCho sparse solver extension. For this, follow these steps: 1. Compile
+BaSpaCho from source following instructions [here](https://github.com/
+facebookresearch/baspacho). We recommend using flags `-DBLA_STATIC=ON -
+DBUILD_SHARED_LIBS=OFF`. 2. Run ```bash git clone https://github.com/
+facebookresearch/theseus.git && cd theseus BASPACHO_ROOT_DIR=
 o/root/baspacho/dir> pip install -e . ``` where the BaSpaCho root dir must have
 the binaries in the subdirectory `build`. ### Running unit tests (requires
 `dev` installation) ```bash python -m pytest tests ``` By default, unit tests
 include tests for our CUDA extensions. You can add the option `-m "not
 cudaext"` to skip them when installing without CUDA support. Additionally, the
 tests for sparse solver BaSpaCho are automatically skipped when its extlib is
 not compiled. ## Examples [Simple example](https://github.com/facebookresearch/
```

### Comparing `theseus-ai-0.2.0.dev0/README.md` & `theseus-ai-0.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -56,20 +56,22 @@
 -----
 
 ## Current Features
 
 ### Application agnostic interface
 Our implementation provides an easy to use interface to build custom optimization layers and plug them into any neural architecture. Following differentiable features are currently available:
 - [Second-order nonlinear optimizers](https://github.com/facebookresearch/theseus/tree/main/theseus/optimizer/nonlinear)
-    - Gauss-Newton, Levenberg–Marquardt
+    - Gauss-Newton (GN), Levenberg–Marquardt (LM), Trust Region, Dogleg
+- [Other nonlinear optimizers](https://github.com/facebookresearch/theseus/tree/main/theseus/optimizer/nonlinear)
+    - Cross Entropy Method (CEM)
 - [Linear solvers](https://github.com/facebookresearch/theseus/tree/main/theseus/optimizer/linear)
     - Dense: Cholesky, LU; Sparse: CHOLMOD, LU (GPU-only), [BaSpaCho](https://github.com/facebookresearch/baspacho)
 - [Commonly used costs](https://github.com/facebookresearch/theseus/tree/main/theseus/embodied), [AutoDiffCostFunction](https://github.com/facebookresearch/theseus/blob/main/theseus/core/cost_function.py), [RobustCostFunction](https://github.com/facebookresearch/theseus/blob/main/theseus/core/robust_cost_function.py)
-- [Lie groups](https://github.com/facebookresearch/theseus/tree/main/theseus/geometry)
-- [Robot kinematics](https://github.com/facebookresearch/theseus/blob/main/theseus/embodied/kinematics/kinematics_model.py)
+- [Lie groups](https://github.com/facebookresearch/theseus/tree/main/theseus/geometry) based on [torchlie](https://github.com/facebookresearch/theseus/tree/main/torchlie)
+- [Robot kinematics](https://github.com/facebookresearch/theseus/blob/main/theseus/embodied/kinematics) based on [torchkin](https://github.com/facebookresearch/theseus/tree/main/torchkin)
 
 ### Efficiency based design
 We support several features that improve computation times and memory consumption:
 - [Sparse linear solvers](https://github.com/facebookresearch/theseus/tree/main/theseus/optimizer/linear)
 - Batching and GPU acceleration
 - [Automatic vectorization](https://github.com/facebookresearch/theseus/blob/main/theseus/core/vectorizer.py)
 - [Backward modes](https://github.com/facebookresearch/theseus/blob/main/theseus/optimizer/nonlinear/nonlinear_optimizer.py)
@@ -104,14 +106,15 @@
     ```bash
     git clone https://github.com/facebookresearch/theseus.git && cd theseus
     pip install -e .
     ```
     If you are interested in contributing to Theseus, instead install
     ```bash
     pip install -e ".[dev]"
+    pre-commit install
     ```
     and follow the more detailed instructions in [CONTRIBUTING](https://github.com/facebookresearch/theseus/blob/main/CONTRIBUTING.md).
 
 - **Installing BaSpaCho extensions from source**
 
     By default, installing from source doesn't include our BaSpaCho sparse solver extension. For this, follow these steps:
```

#### html2text {}

```diff
@@ -15,28 +15,32 @@
 by differentiating through the optimizer which allows neural models to train on
 the final task loss, while also taking advantage of priors captured by the
 optimizer. ----- ## Current Features ### Application agnostic interface Our
 implementation provides an easy to use interface to build custom optimization
 layers and plug them into any neural architecture. Following differentiable
 features are currently available: - [Second-order nonlinear optimizers](https:/
 /github.com/facebookresearch/theseus/tree/main/theseus/optimizer/nonlinear) -
-Gauss-Newton, LevenbergâMarquardt - [Linear solvers](https://github.com/
-facebookresearch/theseus/tree/main/theseus/optimizer/linear) - Dense: Cholesky,
-LU; Sparse: CHOLMOD, LU (GPU-only), [BaSpaCho](https://github.com/
-facebookresearch/baspacho) - [Commonly used costs](https://github.com/
-facebookresearch/theseus/tree/main/theseus/embodied), [AutoDiffCostFunction]
-(https://github.com/facebookresearch/theseus/blob/main/theseus/core/
-cost_function.py), [RobustCostFunction](https://github.com/facebookresearch/
-theseus/blob/main/theseus/core/robust_cost_function.py) - [Lie groups](https://
-github.com/facebookresearch/theseus/tree/main/theseus/geometry) - [Robot
-kinematics](https://github.com/facebookresearch/theseus/blob/main/theseus/
-embodied/kinematics/kinematics_model.py) ### Efficiency based design We support
-several features that improve computation times and memory consumption: -
-[Sparse linear solvers](https://github.com/facebookresearch/theseus/tree/main/
-theseus/optimizer/linear) - Batching and GPU acceleration - [Automatic
+Gauss-Newton (GN), LevenbergâMarquardt (LM), Trust Region, Dogleg - [Other
+nonlinear optimizers](https://github.com/facebookresearch/theseus/tree/main/
+theseus/optimizer/nonlinear) - Cross Entropy Method (CEM) - [Linear solvers]
+(https://github.com/facebookresearch/theseus/tree/main/theseus/optimizer/
+linear) - Dense: Cholesky, LU; Sparse: CHOLMOD, LU (GPU-only), [BaSpaCho]
+(https://github.com/facebookresearch/baspacho) - [Commonly used costs](https://
+github.com/facebookresearch/theseus/tree/main/theseus/embodied),
+[AutoDiffCostFunction](https://github.com/facebookresearch/theseus/blob/main/
+theseus/core/cost_function.py), [RobustCostFunction](https://github.com/
+facebookresearch/theseus/blob/main/theseus/core/robust_cost_function.py) - [Lie
+groups](https://github.com/facebookresearch/theseus/tree/main/theseus/geometry)
+based on [torchlie](https://github.com/facebookresearch/theseus/tree/main/
+torchlie) - [Robot kinematics](https://github.com/facebookresearch/theseus/
+blob/main/theseus/embodied/kinematics) based on [torchkin](https://github.com/
+facebookresearch/theseus/tree/main/torchkin) ### Efficiency based design We
+support several features that improve computation times and memory consumption:
+- [Sparse linear solvers](https://github.com/facebookresearch/theseus/tree/
+main/theseus/optimizer/linear) - Batching and GPU acceleration - [Automatic
 vectorization](https://github.com/facebookresearch/theseus/blob/main/theseus/
 core/vectorizer.py) - [Backward modes](https://github.com/facebookresearch/
 theseus/blob/main/theseus/optimizer/nonlinear/nonlinear_optimizer.py) -
 Implicit, Truncated, Direct Loss Minimization ([DLM](https://github.com/
 facebookresearch/theseus/blob/main/theseus/theseus_layer.py)), Sampling ([LEO]
 (https://github.com/facebookresearch/theseus/blob/main/examples/
 state_estimation_2d.py)) ## Getting Started ### Prerequisites - We *strongly*
@@ -57,23 +61,23 @@
 theseus/blob/main/build_scripts/build_wheel.sh). Note that `pypi` installation
 doesn't include our experimental [Theseus Labs](https://github.com/
 facebookresearch/theseus/tree/main/theseus/labs). For this, please install from
 source. - #### **From source** The simplest way to install Theseus from source
 is by running the following (see further below to also include BaSpaCho)
 ```bash git clone https://github.com/facebookresearch/theseus.git && cd theseus
 pip install -e . ``` If you are interested in contributing to Theseus, instead
-install ```bash pip install -e ".[dev]" ``` and follow the more detailed
-instructions in [CONTRIBUTING](https://github.com/facebookresearch/theseus/
-blob/main/CONTRIBUTING.md). - **Installing BaSpaCho extensions from source** By
-default, installing from source doesn't include our BaSpaCho sparse solver
-extension. For this, follow these steps: 1. Compile BaSpaCho from source
-following instructions [here](https://github.com/facebookresearch/baspacho). We
-recommend using flags `-DBLA_STATIC=ON -DBUILD_SHARED_LIBS=OFF`. 2. Run ```bash
-git clone https://github.com/facebookresearch/theseus.git && cd theseus
-BASPACHO_ROOT_DIR=
+install ```bash pip install -e ".[dev]" pre-commit install ``` and follow the
+more detailed instructions in [CONTRIBUTING](https://github.com/
+facebookresearch/theseus/blob/main/CONTRIBUTING.md). - **Installing BaSpaCho
+extensions from source** By default, installing from source doesn't include our
+BaSpaCho sparse solver extension. For this, follow these steps: 1. Compile
+BaSpaCho from source following instructions [here](https://github.com/
+facebookresearch/baspacho). We recommend using flags `-DBLA_STATIC=ON -
+DBUILD_SHARED_LIBS=OFF`. 2. Run ```bash git clone https://github.com/
+facebookresearch/theseus.git && cd theseus BASPACHO_ROOT_DIR=
 o/root/baspacho/dir> pip install -e . ``` where the BaSpaCho root dir must have
 the binaries in the subdirectory `build`. ### Running unit tests (requires
 `dev` installation) ```bash python -m pytest tests ``` By default, unit tests
 include tests for our CUDA extensions. You can add the option `-m "not
 cudaext"` to skip them when installing without CUDA support. Additionally, the
 tests for sparse solver BaSpaCho are automatically skipped when its extlib is
 not compiled. ## Examples [Simple example](https://github.com/facebookresearch/
```

### Comparing `theseus-ai-0.2.0.dev0/setup.py` & `theseus-ai-0.2.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -140,25 +140,25 @@
         torch_cpp_ext.CUDAExtension(
             name="theseus.extlib.cusolver_lu_solver",
             sources=[
                 str(root_dir / "theseus" / "extlib" / "cusolver_lu_solver.cpp"),
                 str(root_dir / "theseus" / "extlib" / "cusolver_sp_defs.cpp"),
             ],
             include_dirs=[str(root_dir)],
-            libraries=["cusolver"],
+            libraries=["cusolver", "cusparse"],
         ),
     ]
 else:
     print("No CUDA support found. CUDA extensions won't be installed.")
     ext_modules = []
 baspacho_extension = maybe_create_baspacho_extension(compile_cuda_support)
 if baspacho_extension is not None:
     ext_modules.append(baspacho_extension)
 
-excluded_packages = ["lie", "lie.*", "tests*", "tests", "examples"]
+excluded_packages = ["torchlie", "torchlie.*", "tests*", "tests", "examples"]
 package_name = "theseus-ai-nightly" if is_nightly else "theseus-ai"
 if not os.environ.get("INCLUDE_THESEUS_LABS") and not is_nightly:
     excluded_packages.append("theseus.labs*")
     print("Excluding theseus.labs")
 setuptools.setup(
     name=package_name,
     version=version,
```

### Comparing `theseus-ai-0.2.0.dev0/theseus/__init__.py` & `theseus-ai-0.2.1/theseus/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 from ._version import __version__
 
 from .constants import DeviceType as DeviceType
+from .global_params import set_global_params  # usort: skip
 
 from .core import (  # usort: skip
     AutoDiffCostFunction,
     AutogradMode,
     CostFunction,
     CostWeight,
     DiagonalCostWeight,
```

### Comparing `theseus-ai-0.2.0.dev0/theseus/constants.py` & `theseus-ai-0.2.1/theseus/constants.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
-from typing import Optional, Union
 import math
+from typing import Optional, Union
 
 import torch
 
 TEST_EPS = 5e-7
 EPS = 1e-10
 PI = math.pi
```

### Comparing `theseus-ai-0.2.0.dev0/theseus/core/__init__.py` & `theseus-ai-0.2.1/theseus/core/__init__.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-0.2.0.dev0/theseus/core/cost_function.py` & `theseus-ai-0.2.1/theseus/core/cost_function.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,14 +58,16 @@
 # A cost function is defined by the variables interacting in it,
 # and a cost weight for weighting errors and jacobians
 # This is an abstract class for cost functions of different types.
 # Each concrete function must implement an error method and the
 # jacobian of the error, by implementing abstract methods
 # `error` and `jacobians`, respectively.
 class CostFunction(TheseusFunction, abc.ABC):
+    """A cost function in a differentiable optimization problem."""
+
     def __init__(
         self,
         cost_weight: CostWeight,
         name: Optional[str] = None,
     ):
         super().__init__(name=name)
         self._weight = cost_weight
```

### Comparing `theseus-ai-0.2.0.dev0/theseus/core/cost_weight.py` & `theseus-ai-0.2.1/theseus/core/cost_weight.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-0.2.0.dev0/theseus/core/objective.py` & `theseus-ai-0.2.1/theseus/core/objective.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     Callable,
     Dict,
     Iterable,
     List,
     Optional,
     Protocol,
     Sequence,
+    Tuple,
     Union,
 )
 
 import torch
 
 from theseus.constants import DeviceType
 from theseus.core.theseus_function import TheseusFunction
@@ -35,15 +36,36 @@
 
 def error_squared_norm_fn(error_vector: torch.Tensor) -> torch.Tensor:
     return (error_vector**2).sum(dim=1) / 2
 
 
 # If dtype is None, uses torch.get_default_dtype()
 class Objective:
-    """An objective function to optimize."""
+    """An objective function to optimize.
+
+    Defines the structure of an optimization problem in Theseus by aggregating
+    :class:`cost functions <theseus.CostFunction>` into a single objective.
+    The cost functions that comprise the final
+    objective function are specified via the :meth:`add() <theseus.Objective.add>`
+    method. Cost functions are responsible for registering their optimization and
+    auxiliary variables, which are automatically added to the objective's list of
+    variables when a cost function is added.
+    Importantly, optimization variables must be instances of :class:`Manifold`
+    subclasses, while auxiliary variables can be instances of
+    any :class:`Variable` class.
+
+    Args:
+        dtype (optional[torch.dtype]): the data type to use for all variables. If
+            ``None`` is passed, then uses ``torch.get_default_dtype()``.
+        error_metric_fn (optional[callable]): a reference to a Python function used to
+            aggregate cost functions into a single objective. Defaults to using the
+            sum of squared costs. If given, it must receive a single tensor as input.
+            The objective will use it to pass the batched concatenated error vector,
+            will all cost function errors concatenated.
+    """
 
     def __init__(
         self,
         dtype: Optional[torch.dtype] = None,
         error_metric_fn: Optional[ErrorMetric] = None,
         __allow_mixed_optim_aux_vars__: bool = False,  # experimental
     ):
@@ -179,26 +201,42 @@
 
             if self._allow_mixed_optim_aux_vars and variable not in self_var_to_fn_map:
                 self_var_to_fn_map[variable] = []
 
             # add to list of functions connected to this variable
             self_var_to_fn_map[variable].append(function)
 
-    # Adds a cost function to the objective
-    # Also adds its optimization variables if they haven't been previously added
-    # Throws an error if a new variable has the same name of a previously added
-    # variable that is not the same object.
-    # Does the same for the cost function's auxiliary variables
-    # Then does the same with the cost weight's auxiliary variables
-    #
-    # For now, cost weight "optimization variables" are **NOT** added to the
-    # set of objective's variables, they are kept in a separate container.
-    # Update method will check if any of these are not registered as
-    # cost function variables, and throw a warning.
     def add(self, cost_function: CostFunction):
+        """Adds a cost function to the objective.
+
+        When a cost function is added, this method goes over its list of registered
+        optimization and auxiliary variables, and adds any of them to the objective's
+        list of variables, as long as a variable with th4 same name hasn't been added
+        before. If any of the cost function's variables has the same as that of
+        a variable previously added to the objective, the method
+        checks that they are referring to the same :class:`theseus.Variable`. If this
+        is not the case, an error will be triggered. In other words, the objective
+        expects to have a unique mapping between variable names and objects.
+
+        The same procedure is followed for the cost function's weight.
+
+        Args:
+            cost_function (:class:`theseus.CostFunction`): the cost function to be
+                added to the objective.
+
+        .. warning::
+
+            If a cost weight registers optimization variables that are not used in any
+            :class:`theseus.CostFunction <CostFunction>` objects, these will **NOT**
+            be added to the set of the objective's optimization variables; they will be
+            kept in a separate container. The :meth:`update` method will check for this,
+            and throw a warning whenever this happens. Also note that Theseus
+            always considers cost weights as constants, even if their value depends on
+            variables declared as optimization variables.
+        """
         # adds the cost function if not already present
         if cost_function.name in self.cost_functions:
             if cost_function is not self.cost_functions[cost_function.name]:
                 raise ValueError(
                     f"Two different cost function objects with the "
                     f"same name ({cost_function.name}) are not allowed "
                     "in the same objective."
@@ -265,36 +303,86 @@
             for optim_name in optim_vars_names:
                 if self.has_aux_var(optim_name):
                     raise ValueError(dual_var_err_msg)
             for aux_name in aux_vars_names:
                 if self.has_optim_var(aux_name):
                     raise ValueError(dual_var_err_msg)
 
-    # returns a reference to the cost function with the given name
     def get_cost_function(self, name: str) -> CostFunction:
+        """Returns a reference to the cost function with the given name.
+
+        Args:
+            name (str): the name of the cost function to retrieve.
+
+        Returns:
+            CostFunction: the :class:`theseus.CostFunction` with the given name, if
+            present. Otherwise ``None``.
+        """
         return self.cost_functions.get(name, None)
 
-    # checks if the cost function with the given name is in the objective
     def has_cost_function(self, name: str) -> bool:
+        """Checks if a cost function with the given name is in the objective.
+
+        Args:
+            name (str): the name of the cost function.
+
+        Returns:
+            bool: ``True`` if a function exists with the given name,
+                ``False`` otherwise.
+        """
         return name in self.cost_functions
 
-    # checks if the optimization variable with the given name is in the objective
     def has_optim_var(self, name: str) -> bool:
+        """Checks if an optimization variable is used in the objective.
+
+        Args:
+            name (str): the name of the optimization variable.
+
+        Returns:
+            bool: ``True`` if an optimization variable with the given name exists in the
+                objective (i.e., it's currently associated to at least one cost
+                function in the objective). ``False`` otherwise.
+        """
         return name in self.optim_vars
 
-    # returns a reference to the optimization variable with the given name
     def get_optim_var(self, name: str) -> Manifold:
+        """Returns a reference to the optimization variable with the given name.
+
+        Args:
+            name (str): the name of the optimization variable to retrieve.
+
+        Returns:
+            Manifold: the :class:`theseus.Manifold` with the given name, if
+            present. Otherwise ``None``.
+        """
         return self.optim_vars.get(name, None)
 
-    # checks if the aux. variable with the given name is in the objective
     def has_aux_var(self, name: str) -> bool:
+        """Checks if an auxiliary variable is used in the objective.
+
+        Args:
+            name (str): the name of the auxiliary variable.
+
+        Returns:
+            bool: ``True`` if an auxiliary variable with the given name exists in the
+                objective (i.e., it's currently associated to at least one cost
+                function or cost weight in the objective). ``False`` otherwise.
+        """
         return name in self.aux_vars
 
-    # returns a reference to the aux. variable with the given name
     def get_aux_var(self, name: str) -> Variable:
+        """Returns a reference to the auxiliary variable with the given name.
+
+        Args:
+            name (str): the name of the auxiliary variable to retrieve.
+
+        Returns:
+            Variable: the :class:`theseus.Variable` with the given name, if
+            present. Otherwise ``None``.
+        """
         return self.aux_vars.get(name, None)
 
     @property
     def batch_size(self) -> int:
         return self._batch_size
 
     def _erase_function_variables(
@@ -319,20 +407,25 @@
             # remove function from the variable's list of connected cost functions
             del self_var_to_fn_map[variable][cost_fn_idx]
             # if the variable has no other functions, remove it also
             if not self_var_to_fn_map[variable]:
                 del self_var_to_fn_map[variable]
                 del self_vars_of_this_type[variable.name]
 
-    # Removes a cost function from the objective given its name
-    # Also removes any of its variables that are no longer associated to other
-    # functions (either cost functions, or cost weights).
-    # Does the same for the cost weight, but only if the weight is not associated to
-    # any other cost function
     def erase(self, name: str):
+        """Removes a cost function from the objective given its name
+
+        Also removes any of its variables that are no longer associated to other
+        functions (either cost functions, or cost weights).
+        Does the same for the cost weight variables, but only if the weight is
+        not associated to any other cost function.
+
+        Args:
+            name (str): the name of the cost function to erase.
+        """
         self.current_version += 1
         if name in self.cost_functions:
             cost_function = self.cost_functions[name]
             # erase variables associated to this cost function (if needed)
             self._erase_function_variables(cost_function, optim_vars=True)
             self._erase_function_variables(cost_function, optim_vars=False)
 
@@ -357,21 +450,14 @@
             # finally, delete the cost function
             del self.cost_functions[name]
         else:
             warnings.warn(
                 "This cost function is not in the objective, nothing to be done."
             )
 
-    # gets the name associated with a cost function object (or None if not present)
-    def get_cost_function_name(self, cost_function: CostFunction) -> Optional[str]:
-        for name in self.cost_functions:
-            if id(cost_function) == id(cost_function):
-                return name
-        return None
-
     @staticmethod
     def _get_functions_connected_to_var(
         variable: Union[str, Variable],
         objectives_var_container_dict: "OrderedDict[str, Variable]",
         var_to_cost_fn_map: Dict[Variable, List[TheseusFunction]],
         variable_type: str,
     ) -> List[TheseusFunction]:
@@ -386,56 +472,119 @@
                 f"{variable_type} {variable.name} is not in the objective."
             )
         return var_to_cost_fn_map[variable]
 
     def get_functions_connected_to_optim_var(
         self, variable: Union[Manifold, str]
     ) -> List[TheseusFunction]:
+        """Gets a list of functions that depend on a given optimization variable.
+
+        Args:
+            variable (Union[Manifold, str]): the variable to query for. Can be an
+                instance of :class:`theseus.Manifold` or a string, specifying the name.
+
+        Returns:
+            List[TheseusFunction]: all cost functions that depend on the optimization
+                variable.
+        """
         return Objective._get_functions_connected_to_var(
             variable,
             self.optim_vars,  # type: ignore
             self.functions_for_optim_vars,  # type: ignore
             "Optimization Variable",
         )
 
     def get_functions_connected_to_aux_var(
         self, aux_var: Union[Variable, str]
     ) -> List[TheseusFunction]:
+        """Gets a list of functions that depend on a given auxiliary variable.
+
+        Args:
+            variable (Union[Variable, str]): the variable to query for. Can be an
+                instance of :class:`theseus.Variable` or a string, specifying the name.
+
+        Returns:
+            List[TheseusFunction]: all cost functions that depend on the auxiliary
+                variable.
+        """
         return Objective._get_functions_connected_to_var(
             aux_var, self.aux_vars, self.functions_for_aux_vars, "Auxiliary Variable"
         )
 
-    # sum of cost function dimensions
     def dim(self) -> int:
+        """Returns the dimension of the error vector.
+
+        The dimension is equal to the sum of all cost functions' error dimensions.
+
+        Returns:
+            int: the error dimension.
+        """
         err_dim = 0
         for cost_function in self.cost_functions.values():
             err_dim += cost_function.dim()
         return err_dim
 
-    # number of (cost functions, variables)
-    def size(self) -> tuple:
+    def size(self) -> Tuple[int, int]:
+        """Returns the number of cost functions and variables in the objective.
+
+        Returns:
+            tuple[int, int]: the number of cost functions and optimization variables
+                in the objective, in that order.
+        """
         return len(self.cost_functions), len(self.optim_vars)
 
-    # number of cost functions
     def size_cost_functions(self) -> int:
+        """Returns the number of cost functions in the objective.
+
+        Returns:
+            int: the number of cost functions in the objective.
+        """
         return len(self.cost_functions)
 
-    # number of variables
     def size_variables(self) -> int:
+        """Returns the number of optimization variables in the objective.
+
+        Returns:
+            int: the number of optimization variables in the objective.
+        """
         return len(self.optim_vars)
 
-    # number of auxiliary variables
     def size_aux_vars(self) -> int:
+        """Returns the number of auxiliary variables in the objective.
+
+        Returns:
+            int: the number of auxiliary variables in the objective.
+        """
         return len(self.aux_vars)
 
     def error(
         self,
         input_tensors: Optional[Dict[str, torch.Tensor]] = None,
         also_update: bool = False,
     ) -> torch.Tensor:
+        """Evaluates the error vector.
+
+        Args:
+            input_tensors (Dict[str, torch.Tensor], optional): if given, it must be a
+                dictionary mapping variable names to tensors; if a variable with the
+                given name is registered in the objective, its tensor will be replaced
+                with the one in the dictionary (possibly permanently, depending on the
+                value of ``also_update``). Defaults to ``None``, in which case the error
+                is evaluated using the current tensors stored in all registered
+                variables.
+            also_update (bool, optional): if ``True``, and ``input_tensors`` is given,
+                the modified variables are permanently updated with the given tensors.
+                Defaults to ``False``, in which case the variables are reverted to the
+                previous tensors after the error is evaluated.
+
+        Returns:
+            torch.Tensor: a tensor of shape (batch_size x error_dim), with the
+                concatenation of all cost functions error vectors. The order corresponds
+                to the order in which cost functions were added to the objective.
+        """
         old_tensors = {}
         if input_tensors is not None:
             if not also_update:
                 for var in self.optim_vars:
                     old_tensors[var] = self.optim_vars[var].tensor
             # Update vectorization only if the input tensors will be used for a
             # persistent update.
@@ -461,33 +610,48 @@
         return error_vector
 
     def error_metric(
         self,
         input_tensors: Optional[Dict[str, torch.Tensor]] = None,
         also_update: bool = False,
     ) -> torch.Tensor:
+        """Aggregates all cost function errors into a (batched) scalar objective.
+
+        Args:
+            input_tensors (Dict[str, torch.Tensor], optional): if given, it must be a
+                dictionary mapping variable names to tensors; if a variable with the
+                given name is registered in the objective, its tensor will be replaced
+                with the one in the dictionary (possibly permanently, depending on the
+                value of ``also_update``). Defaults to ``None``, in which case the error
+                is evaluated using the current tensors stored in all registered
+                variables.
+            also_update (bool, optional): if ``True``, and ``input_tensors`` is given,
+                the modified variables are permanently updated with the given tensors.
+                Defaults to ``False``, in which case the variables are reverted to the
+                previous tensors after the error is evaluated.
+
+        Returns:
+            torch.Tensor: a tensor of shape (batch_size,) with the scalar value of
+                the objective function.
+        """
         return self._error_metric_fn(
             self.error(input_tensors=input_tensors, also_update=also_update)
         )
 
-    def error_squared_norm(
-        self,
-        input_tensors: Optional[Dict[str, torch.Tensor]] = None,
-        also_update: bool = False,
-    ) -> torch.Tensor:
-        warnings.warn(
-            "Objective.error_squared_norm() is deprecated "
-            "and will be removed in future versions. "
-            "Please use Objective.error_metric() instead.",
-            DeprecationWarning,
-        )
-        return self.error_metric(input_tensors=input_tensors, also_update=also_update)
-
     def copy(self) -> "Objective":
-        new_objective = Objective(dtype=self.dtype)
+        """Creates a new copy of this objective.
+
+        Returns:
+            Objective: another instance of :class:`theseus.Objective` with copies
+                of all cost functions, weights, and variables, the same
+                connectivity structure, and error metric.
+        """
+        new_objective = Objective(
+            dtype=self.dtype, error_metric_fn=self._error_metric_fn
+        )
 
         # First copy all individual cost weights
         old_to_new_cost_weight_map: Dict[CostWeight, CostWeight] = {}
         for cost_weight in self.cost_functions_for_weights:
             new_cost_weight = cost_weight.copy(
                 new_name=cost_weight.name, keep_variable_names=True
             )
@@ -561,22 +725,63 @@
     # batch size.
     def update(
         self,
         input_tensors: Optional[Dict[str, torch.Tensor]] = None,
         batch_ignore_mask: Optional[torch.Tensor] = None,
         _update_vectorization: bool = True,
     ):
+        """Updates all variables with the given input tensor dictionary.
+
+        The behavior of this method can be summarized by the following pseudocode:
+
+        .. code-block::
+
+            for name, tensor in input_tensors.items():
+                var = self.get_var_with_name(name).update(tensor)
+            check_batch_size_consistency(self.all_variables)
+
+        Any variables not included in the input tensors dictionary will retain their
+        current tensors.
+
+        After updating, the objective will modify its batch size
+        property according to the resulting tensors. Therefore, all variable tensors
+        must have a consistent batch size (either 1 or the same value as the others),
+        after the update is completed. Note that this includes variables not referenced
+        in the ``input_tensors`` dictionary.
+
+        Args:
+            input_tensors (Dict[str, torch.Tensor], optional): if given, it must be a
+                dictionary mapping variable names to tensors; if a variable with the
+                given name is registered in the objective, its tensor will be replaced
+                with the one in the dictionary (possibly permanently, depending on the
+                value of ``also_update``). Defaults to ``None``, in which case nothing
+                will be updated. In both cases, the objective will resolve the
+                batch size with whatever tensors are stored after updating.
+            batch_ignore_mask (torch.Tensor, optional): an optional tensor of shape
+                (batch_size,) of boolean type. Any ``True`` values indicate that
+                this batch index should remain unchanged in all variables.
+                Defaults to ``None``.
+
+        Raises:
+            ValueError: if tensors with inconsistent batch dimension are given.
+        """
         input_tensors = input_tensors or {}
         for var_name, tensor in input_tensors.items():
             if tensor.ndim < 2:
                 raise ValueError(
                     f"Input tensors must have a batch dimension and "
                     f"one ore more data dimensions, but tensor.ndim={tensor.ndim} for "
                     f"tensor with name {var_name}."
                 )
+            if tensor.device != self.device or tensor.dtype != self.dtype:
+                raise ValueError(
+                    f"Attempted to update variable {var_name} with a "
+                    f"({tensor.device},{tensor.dtype}) tensor, which is inconsistent "
+                    f"with objective's expected ({self.device},{self.dtype})."
+                )
             if var_name in self.optim_vars:
                 self.optim_vars[var_name].update(
                     tensor, batch_ignore_mask=batch_ignore_mask
                 )
             elif var_name in self.aux_vars:
                 self.aux_vars[var_name].update(
                     tensor, batch_ignore_mask=batch_ignore_mask
@@ -631,16 +836,16 @@
     def _get_jacobians_iter(self) -> Iterable:
         self.update_vectorization_if_needed()
         if self.vectorized:
             return iter(cf for cf in self._vectorized_jacobians_iter)
         # No vectorization is used, just serve from cost functions
         return iter(cf for cf in self.cost_functions.values())
 
-    # Applies to() with given args to all tensors in the objective
     def to(self, *args, **kwargs):
+        """Applies torch.Tensor.to() to all cost functions in the objective."""
         for cost_function in self.cost_functions.values():
             cost_function.to(*args, **kwargs)
         device, dtype, *_ = torch._C._nn._parse_to(*args, **kwargs)
         self.device = device or self.device
         self.dtype = dtype or self.dtype
         if self._vectorization_to is not None:
             self._vectorization_to(*args, **kwargs)
@@ -657,27 +862,48 @@
             new_var = var.retract(delta[:, var_idx : var_idx + var.dof()])
             if ignore_mask is None or force_update:
                 var.update(new_var.tensor)
             else:
                 var.update(new_var.tensor, batch_ignore_mask=ignore_mask)
             var_idx += var.dof()
 
-    # Retracts an ordered sequence of variables according to the
-    # corresponding `delta` tangent vectors.
-    # This function assumes that delta is constructed as follows:
-    #    For ordering = [v1 v2 ... vn]
-    #    delta = torch.cat([delta_v1, delta_v2, ..., delta_vn], dim=-1)
-    # where delta_vi.shape = (batch_size, vi.dof)
     def retract_vars_sequence(
         self,
         delta: torch.Tensor,
         ordering: Iterable[Manifold],
         ignore_mask: Optional[torch.Tensor] = None,
         force_update: bool = False,
     ):
+        """Retracts an ordered sequence of variables.
+
+        The behavior of this method can be summarized by the following pseudocode:
+
+        .. code-block::
+
+            for var in ordering:
+                var.retract(delta[var_idx])
+
+        This function assumes that ``delta`` is constructed as follows:
+
+        .. code-block::
+
+            delta = torch.cat([delta_v1, delta_v2, ..., delta_vn], dim=-1)
+
+        For an ordering ``[v1 v2 ... vn]``, and where
+        ``delta_vi.shape = (batch_size, vi.dof())``
+
+        Args:
+            delta (torch.Tensor): the tensor to use for retract operation.
+            ordering (Iterable[Manifold]): an ordered iterator of variables to retract.
+                The order must be consistent with ``delta`` as explained above.
+            ignore_mask (torch.Tensor, optional): An ignore mask for batch indices as
+                in :meth:`update() <theseus.Objective.update>`. Defaults to ``None``.
+            force_update (bool, optional): if ``True``, disregards the ``ignore_mask``.
+                Defaults to ``False``.
+        """
         self._retract_method(
             delta, ordering, ignore_mask=ignore_mask, force_update=force_update
         )
         # Updating immediately is useful, since it will keep grad history if
         # needed. Otherwise, with lazy waitng we can be in a situation where
         # vectorization is updated with torch.no_grad() (e.g., for error logging),
         # and then it has to be run again later when grad is back on.
```

### Comparing `theseus-ai-0.2.0.dev0/theseus/core/robust_cost_function.py` & `theseus-ai-0.2.1/theseus/core/robust_cost_function.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-0.2.0.dev0/theseus/core/robust_loss.py` & `theseus-ai-0.2.1/theseus/core/robust_loss.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-0.2.0.dev0/theseus/core/theseus_function.py` & `theseus-ai-0.2.1/theseus/core/theseus_function.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-0.2.0.dev0/theseus/core/variable.py` & `theseus-ai-0.2.1/theseus/core/variable.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
 from itertools import count
 from typing import Any, List, Optional, Sequence, Union
 
 import torch
+
 from theseus.constants import DeviceType
 
 
 class Variable:
     """A variable in a differentiable optimization problem."""
 
     _ids = count(0)
```

### Comparing `theseus-ai-0.2.0.dev0/theseus/core/vectorizer.py` & `theseus-ai-0.2.1/theseus/core/vectorizer.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-0.2.0.dev0/theseus/embodied/__init__.py` & `theseus-ai-0.2.1/theseus/embodied/__init__.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-0.2.0.dev0/theseus/embodied/collision/collision.py` & `theseus-ai-0.2.1/theseus/embodied/collision/collision.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-0.2.0.dev0/theseus/embodied/collision/eff_obj_contact.py` & `theseus-ai-0.2.1/theseus/embodied/collision/eff_obj_contact.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-0.2.0.dev0/theseus/embodied/collision/signed_distance_field.py` & `theseus-ai-0.2.1/theseus/embodied/collision/signed_distance_field.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-0.2.0.dev0/theseus/embodied/measurements/between.py` & `theseus-ai-0.2.1/theseus/embodied/measurements/between.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-0.2.0.dev0/theseus/embodied/measurements/moving_frame_between.py` & `theseus-ai-0.2.1/theseus/embodied/measurements/moving_frame_between.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-0.2.0.dev0/theseus/embodied/measurements/reprojection.py` & `theseus-ai-0.2.1/theseus/embodied/measurements/reprojection.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-0.2.0.dev0/theseus/embodied/misc/local_cost_fn.py` & `theseus-ai-0.2.1/theseus/embodied/misc/local_cost_fn.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-0.2.0.dev0/theseus/embodied/motionmodel/double_integrator.py` & `theseus-ai-0.2.1/theseus/embodied/motionmodel/double_integrator.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-0.2.0.dev0/theseus/embodied/motionmodel/misc.py` & `theseus-ai-0.2.1/theseus/embodied/motionmodel/misc.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-0.2.0.dev0/theseus/embodied/motionmodel/quasi_static_pushing_planar.py` & `theseus-ai-0.2.1/theseus/embodied/motionmodel/quasi_static_pushing_planar.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-0.2.0.dev0/theseus/extlib/baspacho_solver.cpp` & `theseus-ai-0.2.1/theseus/extlib/baspacho_solver.cpp`

 * *Files identical despite different names*

### Comparing `theseus-ai-0.2.0.dev0/theseus/extlib/baspacho_solver.h` & `theseus-ai-0.2.1/theseus/extlib/baspacho_solver.h`

 * *Files identical despite different names*

### Comparing `theseus-ai-0.2.0.dev0/theseus/extlib/baspacho_solver_cuda.cu` & `theseus-ai-0.2.1/theseus/extlib/baspacho_solver_cuda.cu`

 * *Files identical despite different names*

### Comparing `theseus-ai-0.2.0.dev0/theseus/extlib/cusolver_lu_solver.cpp` & `theseus-ai-0.2.1/theseus/extlib/cusolver_lu_solver.cpp`

 * *Files identical despite different names*

### Comparing `theseus-ai-0.2.0.dev0/theseus/extlib/cusolver_sp_defs.cpp` & `theseus-ai-0.2.1/theseus/extlib/cusolver_sp_defs.cpp`

 * *Files identical despite different names*

### Comparing `theseus-ai-0.2.0.dev0/theseus/extlib/cusolver_sp_defs.h` & `theseus-ai-0.2.1/theseus/extlib/cusolver_sp_defs.h`

 * *Files identical despite different names*

### Comparing `theseus-ai-0.2.0.dev0/theseus/extlib/mat_mult.cu` & `theseus-ai-0.2.1/theseus/extlib/mat_mult.cu`

 * *Files identical despite different names*

### Comparing `theseus-ai-0.2.0.dev0/theseus/extlib/utils.h` & `theseus-ai-0.2.1/theseus/extlib/utils.h`

 * *Files identical despite different names*

### Comparing `theseus-ai-0.2.0.dev0/theseus/geometry/__init__.py` & `theseus-ai-0.2.1/theseus/geometry/__init__.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-0.2.0.dev0/theseus/geometry/lie_group.py` & `theseus-ai-0.2.1/theseus/geometry/lie_group.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,17 +24,25 @@
 class LieGroup(Manifold):
     def __init__(
         self,
         *args: Any,
         tensor: Optional[torch.Tensor] = None,
         name: Optional[str] = None,
         dtype: torch.dtype = torch.float,
-        strict: bool = False,
+        strict_checks: bool = False,
+        disable_checks: bool = False,
     ):
-        super().__init__(*args, tensor=tensor, name=name, dtype=dtype, strict=strict)
+        super().__init__(
+            *args,
+            tensor=tensor,
+            name=name,
+            dtype=dtype,
+            strict_checks=strict_checks,
+            disable_checks=disable_checks,
+        )
 
     @staticmethod
     def _check_jacobians_list(jacobians: List[torch.Tensor]):
         if len(jacobians) != 0:
             raise ValueError("jacobians list to be populated must be empty.")
 
     @staticmethod
```

### Comparing `theseus-ai-0.2.0.dev0/theseus/geometry/lie_group_check.py` & `theseus-ai-0.2.1/theseus/geometry/lie_group_check.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-0.2.0.dev0/theseus/geometry/manifold.py` & `theseus-ai-0.2.1/theseus/geometry/manifold.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,24 +31,28 @@
 class Manifold(Variable, abc.ABC):
     def __init__(
         self,
         *args: Any,
         tensor: Optional[torch.Tensor] = None,
         name: Optional[str] = None,
         dtype: Optional[torch.dtype] = None,
-        strict: bool = False,
+        strict_checks: bool = False,
+        disable_checks: bool = False,
     ):
         # If nothing specified, use torch's default dtype
         # else tensor.dtype takes precedence
         if tensor is None and dtype is None:
             dtype = torch.get_default_dtype()
         if tensor is not None:
-            checks_enabled, silent_unchecks = _LieGroupCheckContext.get_context()
+            if disable_checks:
+                checks_enabled, silent_unchecks = False, True
+            else:
+                checks_enabled, silent_unchecks = _LieGroupCheckContext.get_context()
             if checks_enabled:
-                tensor = self._check_tensor(tensor, strict)
+                tensor = self._check_tensor(tensor, strict_checks)
             elif not silent_unchecks:
                 warnings.warn(
                     f"Manifold consistency checks are disabled "
                     f"for {self.__class__.__name__}.",
                     RuntimeWarning,
                 )
             if dtype is not None and tensor.dtype != dtype:
```

### Comparing `theseus-ai-0.2.0.dev0/theseus/geometry/point_types.py` & `theseus-ai-0.2.1/theseus/geometry/point_types.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 # LICENSE file in the root directory of this source tree.
 
 from typing import List, Optional, Tuple, Union, cast
 
 import torch
 
 from theseus.constants import DeviceType
+
 from .vector import Vector
 
 
 def _prepare_dof_and_tensor(
     expected_dof: int, tensor: Optional[torch.Tensor]
 ) -> Tuple[Optional[int], Optional[torch.Tensor]]:
     dof = None
```

### Comparing `theseus-ai-0.2.0.dev0/theseus/geometry/se2.py` & `theseus-ai-0.2.1/theseus/geometry/se2.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from typing import List, Optional, Union, cast
 
 import torch
 
 import theseus.constants
 from theseus.geometry.lie_group_check import no_lie_group_check
-from theseus.options import _THESEUS_GLOBAL_OPTIONS
+from theseus.global_params import _THESEUS_GLOBAL_PARAMS
 
 from .lie_group import LieGroup
 from .point_types import Point2
 from .so2 import SO2
 
 
 # If tensor is passed, must be x, y, cos, sin
@@ -21,21 +21,28 @@
 class SE2(LieGroup):
     def __init__(
         self,
         x_y_theta: Optional[torch.Tensor] = None,
         tensor: Optional[torch.Tensor] = None,
         name: Optional[str] = None,
         dtype: Optional[torch.dtype] = None,
-        strict: bool = False,
+        strict_checks: bool = False,
+        disable_checks: bool = False,
     ):
         if x_y_theta is not None and tensor is not None:
             raise ValueError("Please provide only one of x_y_theta or tensor.")
         if x_y_theta is not None:
             dtype = x_y_theta.dtype
-        super().__init__(tensor=tensor, name=name, dtype=dtype, strict=strict)
+        super().__init__(
+            tensor=tensor,
+            name=name,
+            dtype=dtype,
+            strict_checks=strict_checks,
+            disable_checks=disable_checks,
+        )
         if x_y_theta is not None:
             self.update_from_x_y_theta(x_y_theta)
 
     @staticmethod
     def rand(
         *size: int,
         generator: Optional[torch.Generator] = None,
@@ -159,15 +166,15 @@
         self, jacobians: Optional[List[torch.Tensor]] = None
     ) -> torch.Tensor:
         rotation = self.rotation
         theta = rotation.log_map().view(-1)
         cosine, sine = rotation.to_cos_sin()
 
         # Compute the approximations when theta is near to 0
-        small_theta = theta.abs() < _THESEUS_GLOBAL_OPTIONS.get_eps(
+        small_theta = theta.abs() < _THESEUS_GLOBAL_PARAMS.get_eps(
             "se2", "near_zero", theta.dtype
         )
         non_zero = torch.ones(1, dtype=self.dtype, device=self.device)
         sine_nz = torch.where(small_theta, non_zero, sine)
         half_theta_by_tan_half_theta = (
             0.5
             * (1 + cosine)
@@ -186,26 +193,31 @@
                 3,
                 3,
             )
 
             theta2 = theta**2
             theta3 = theta * theta2
 
-            theta_nz = torch.where(small_theta, non_zero, theta)
-            one_minus_cosine_nz = torch.where(small_theta, non_zero, 1 - cosine)
+            d_small_theta = theta.abs() < _THESEUS_GLOBAL_PARAMS.get_eps(
+                "se2", "d_near_zero", theta.dtype
+            )
+            theta_nz = torch.where(d_small_theta, non_zero, theta)
+            one_minus_cosine_nz = torch.where(d_small_theta, non_zero, 1 - cosine)
 
             half_theta_sine_by_one_minus_cosine = torch.where(
-                small_theta, 1 - theta2 / 12.0, half_theta * sine / one_minus_cosine_nz
+                d_small_theta,
+                1 - theta2 / 12.0,
+                half_theta * sine / one_minus_cosine_nz,
             )
             jac[:, [0, 1], [0, 1]] = half_theta_sine_by_one_minus_cosine.view(-1, 1)
             jac[:, 0, 1] = -half_theta
             jac[:, 1, 0] = half_theta
 
             coeff = torch.where(
-                small_theta,
+                d_small_theta,
                 theta / 12.0 + theta3 / 720.0,
                 1.0 / theta_nz - 0.5 * sine / one_minus_cosine_nz,
             )
 
             jac[:, 0, 2] = coeff * ux + 0.5 * uy
             jac[:, 1, 2] = coeff * uy - 0.5 * ux
 
@@ -230,15 +242,15 @@
         u = tangent_vector[:, :2]
         theta = tangent_vector[:, 2]
         rotation = SO2(theta=theta)
 
         cosine, sine = rotation.to_cos_sin()
 
         # Compute the approximations when theta is near to 0
-        small_theta = theta.abs() < _THESEUS_GLOBAL_OPTIONS.get_eps(
+        small_theta = theta.abs() < _THESEUS_GLOBAL_PARAMS.get_eps(
             "se2", "near_zero", tangent_vector.dtype
         )
         non_zero = torch.ones(
             1, dtype=tangent_vector.dtype, device=tangent_vector.device
         )
         theta2 = theta**2
         theta3 = theta**3
@@ -312,15 +324,15 @@
         new_rotation = rotation_1.compose(rotation_2)
         new_translation = cast(
             Point2,
             translation_1.compose(rotation_1.rotate(translation_2)),
         )
         return SE2(
             tensor=torch.cat([new_translation.tensor, new_rotation.tensor], dim=1),
-            strict=False,
+            disable_checks=True,
         )
 
     def _inverse_impl(self) -> "SE2":
         inverse_rotation = self.rotation._inverse_impl()
         inverse_translation = inverse_rotation.rotate(cast(Point2, -self.translation))
         se2_inverse = SE2(dtype=self.dtype)
         se2_inverse.update_from_rot_and_trans(inverse_rotation, inverse_translation)
```

### Comparing `theseus-ai-0.2.0.dev0/theseus/geometry/se3.py` & `theseus-ai-0.2.1/theseus/geometry/so3.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,303 +3,302 @@
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
 import warnings
 from typing import List, Optional, Union, cast
 
 import torch
-from lie.functional import SE3 as SE3_base
 
 import theseus.constants
+from theseus.global_params import _THESEUS_GLOBAL_PARAMS
+from torchlie.functional import SO3 as SO3_base
 
 from .lie_group import LieGroup
-from .lie_group_check import _LieGroupCheckContext, no_lie_group_check
+from .lie_group_check import _LieGroupCheckContext
 from .point_types import Point3
-from .so3 import SO3
 
 
-class SE3(LieGroup):
+class SO3(LieGroup):
     def __init__(
         self,
-        x_y_z_quaternion: Optional[torch.Tensor] = None,
+        quaternion: Optional[torch.Tensor] = None,
         tensor: Optional[torch.Tensor] = None,
         name: Optional[str] = None,
         dtype: Optional[torch.dtype] = None,
-        strict: bool = False,
+        strict_checks: bool = False,
+        disable_checks: bool = False,
     ):
-        if x_y_z_quaternion is not None and tensor is not None:
-            raise ValueError("Please provide only one of x_y_z_quaternion or tensor.")
-        if x_y_z_quaternion is not None:
-            dtype = x_y_z_quaternion.dtype
-        super().__init__(tensor=tensor, name=name, dtype=dtype, strict=strict)
-        if x_y_z_quaternion is not None:
-            self.update_from_x_y_z_quaternion(x_y_z_quaternion=x_y_z_quaternion)
+        if quaternion is not None and tensor is not None:
+            raise ValueError("Please provide only one of quaternion or tensor.")
+        if quaternion is not None:
+            dtype = quaternion.dtype
+        super().__init__(
+            tensor=tensor,
+            name=name,
+            dtype=dtype,
+            strict_checks=strict_checks,
+            disable_checks=disable_checks,
+        )
+        if quaternion is not None:
+            self.update_from_unit_quaternion(quaternion)
 
     @staticmethod
     def rand(
         *size: int,
         generator: Optional[torch.Generator] = None,
         dtype: Optional[torch.dtype] = None,
         device: theseus.constants.DeviceType = None,
         requires_grad: bool = False,
-    ) -> "SE3":
+    ) -> "SO3":
         if len(size) != 1:
             raise ValueError("The size should be 1D.")
-        tensor = SE3_base.rand(
+        tensor = SO3_base.rand(
             *size,
             generator=generator,
             dtype=dtype,
             device=device,
             requires_grad=requires_grad,
         )
-        return SE3(tensor=tensor)
+        return SO3(tensor=tensor, disable_checks=True)
 
     @staticmethod
     def randn(
         *size: int,
         generator: Optional[torch.Generator] = None,
         dtype: Optional[torch.dtype] = None,
         device: theseus.constants.DeviceType = None,
         requires_grad: bool = False,
-    ) -> "SE3":
+    ) -> "SO3":
         if len(size) != 1:
             raise ValueError("The size should be 1D.")
-        tensor = SE3_base.randn(
+        tensor = SO3_base.randn(
             *size,
             generator=generator,
             dtype=dtype,
             device=device,
             requires_grad=requires_grad,
         )
-        return SE3(tensor=tensor)
+        return SO3(tensor=tensor, disable_checks=True)
 
     @staticmethod
     def _init_tensor() -> torch.Tensor:  # type: ignore
-        return torch.eye(3, 4).view(1, 3, 4)
+        return torch.eye(3, 3).view(1, 3, 3)
+
+    def update_from_unit_quaternion(self, quaternion: torch.Tensor):
+        self.update(self.unit_quaternion_to_SO3(quaternion))
 
     def dof(self) -> int:
-        return 6
+        return 3
 
     def __repr__(self) -> str:
-        return f"SE3(tensor={self.tensor}, name={self.name})"
+        return f"SO3(tensor={self.tensor}, name={self.name})"
 
     def __str__(self) -> str:
         with torch.no_grad():
-            return f"SE3(matrix={self.tensor}), name={self.name})"
+            return f"SO3(matrix={self.tensor}), name={self.name})"
 
     def _adjoint_impl(self) -> torch.Tensor:
-        return SE3_base.adj(self.tensor)
+        return self.tensor.clone()
 
     def _project_impl(
         self, euclidean_grad: torch.Tensor, is_sparse: bool = False
     ) -> torch.Tensor:
         self._project_check(euclidean_grad, is_sparse)
         if is_sparse:
-            return SE3_base.left_project(self.tensor, euclidean_grad)
+            return SO3_base.left_project(self.tensor, euclidean_grad)
         else:
-            ret = self.tensor.new_zeros(euclidean_grad.shape[:-2] + torch.Size([6]))
-            temp = torch.einsum(
-                "...jk,...ji->...ik", euclidean_grad, self.tensor[:, :, :3]
-            )
-            ret[..., :3] = temp[..., 3]
-            ret[..., 3] = temp[..., 2, 1] - temp[..., 1, 2]
-            ret[..., 4] = temp[..., 0, 2] - temp[..., 2, 0]
-            ret[..., 5] = temp[..., 1, 0] - temp[..., 0, 1]
-
+            ret = self.tensor.new_zeros(euclidean_grad.shape[:-1])
+            temp = torch.einsum("...jk,...ji->...ik", euclidean_grad, self.tensor)
+            ret[..., 0] = temp[..., 2, 1] - temp[..., 1, 2]
+            ret[..., 1] = temp[..., 0, 2] - temp[..., 2, 0]
+            ret[..., 2] = temp[..., 1, 0] - temp[..., 0, 1]
             return ret
 
     @staticmethod
     def _check_tensor_impl(tensor: torch.Tensor) -> bool:
-        if tensor.ndim != 3 or tensor.shape[1:] != (3, 4):
-            raise ValueError("SE3 data tensors can only be 3x4 matrices.")
-        try:
-            SE3_base.check_group_tensor(tensor)
-        except ValueError:
-            return False
+        with torch.no_grad():
+            if tensor.ndim != 3 or tensor.shape[1:] != (3, 3):
+                raise ValueError("SO3 data tensors can only be 3x3 matrices.")
+            try:
+                SO3_base.check_group_tensor(tensor)
+            except ValueError:
+                return False
         return True
 
     @staticmethod
-    def x_y_z_unit_quaternion_to_SE3(x_y_z_quaternion: torch.Tensor) -> "SE3":
-        if x_y_z_quaternion.ndim == 1:
-            x_y_z_quaternion = x_y_z_quaternion.unsqueeze(0)
-
-        if x_y_z_quaternion.ndim != 2 and x_y_z_quaternion.shape[1] != 7:
-            raise ValueError("x_y_z_quaternion can only be 7-D vectors.")
-
-        ret = SE3()
-
-        batch_size = x_y_z_quaternion.shape[0]
-        ret.tensor = torch.empty(batch_size, 3, 4).to(
-            device=x_y_z_quaternion.device, dtype=x_y_z_quaternion.dtype
-        )
-        ret[:, :, :3] = SO3.unit_quaternion_to_SO3(x_y_z_quaternion[:, 3:]).tensor
-        ret[:, :, 3] = x_y_z_quaternion[:, :3]
+    def _unit_quaternion_check(quaternion: torch.Tensor):
+        if quaternion.ndim != 2 or quaternion.shape[1] != 4:
+            raise ValueError("Quaternions can only be 4-D vectors.")
 
-        return ret
+        checks_enabled, silent_unchecks = _LieGroupCheckContext.get_context()
+        if checks_enabled:
+            SO3_base.check_unit_quaternion(quaternion)
+        elif not silent_unchecks:
+            warnings.warn(
+                "Lie group checks are disabled, so the validness of unit quaternions is not "
+                "checked for SO3.",
+                RuntimeWarning,
+            )
 
     @staticmethod
     def _hat_matrix_check(matrix: torch.Tensor):
-        if matrix.ndim != 3 or matrix.shape[1:] != (4, 4):
-            raise ValueError("Hat matrices of SE3 can only be 4x4 matrices")
+        if matrix.ndim != 3 or matrix.shape[1:] != (3, 3):
+            raise ValueError("Hat matrices of SO(3) can only be 3x3 matrices")
 
         checks_enabled, silent_unchecks = _LieGroupCheckContext.get_context()
         if checks_enabled:
-            return SE3_base.check_hat_tensor(matrix)
+            SO3_base.check_hat_tensor(matrix)
         elif not silent_unchecks:
             warnings.warn(
                 "Lie group checks are disabled, so the skew-symmetry of hat matrices is "
-                "not checked for SE3.",
+                "not checked for SO3.",
                 RuntimeWarning,
             )
 
     @staticmethod
     def exp_map(
         tangent_vector: torch.Tensor, jacobians: Optional[List[torch.Tensor]] = None
-    ) -> "SE3":
-        if tangent_vector.ndim != 2 or tangent_vector.shape[1] != 6:
-            raise ValueError("Tangent vectors of SE3 can only be 6D vectors.")
-        return SE3(tensor=SE3_base.exp(tangent_vector, jacobians=jacobians))
+    ) -> "SO3":
+        if tangent_vector.ndim != 2 or tangent_vector.shape[1] != 3:
+            raise ValueError("Tangent vectors of SO3 should be batched 3-D vectors.")
+        return SO3(
+            tensor=SO3_base.exp(tangent_vector, jacobians=jacobians),
+            disable_checks=True,
+        )
 
     @staticmethod
     def normalize(tensor: torch.Tensor) -> torch.Tensor:
-        if tensor.ndim != 3 or tensor.shape[1:] != (3, 4):
-            raise ValueError("SE3 data tensors can only be 3x4 matrices.")
-        return SE3_base.normalize(tensor)
+        if tensor.ndim != 3 or tensor.shape[1:] != (3, 3):
+            raise ValueError("SO3 data tensors can only be batched 3x3 matrices.")
+        return SO3_base.normalize(tensor)
 
     def _log_map_impl(
         self, jacobians: Optional[List[torch.Tensor]] = None
     ) -> torch.Tensor:
-        return SE3_base.log(self.tensor, jacobians=jacobians)
+        return SO3_base.log(self.tensor, jacobians=jacobians)
 
-    def _compose_impl(self, se3_2: LieGroup) -> "SE3":
-        return SE3(tensor=SE3_base.compose(self.tensor, se3_2.tensor))
+    def _compose_impl(self, so3_2: LieGroup) -> "SO3":
+        return SO3(
+            tensor=SO3_base.compose(self.tensor, so3_2.tensor), strict_checks=False
+        )
 
-    def _inverse_impl(self, get_jacobian: bool = False) -> "SE3":
-        return SE3(tensor=SE3_base.inv(self.tensor))
+    def _inverse_impl(self, get_jacobian: bool = False) -> "SO3":
+        # if self.tensor is a valid SO(3), then self.tensor.transpose(1, 2)
+        # must be valid as well
+        return SO3(tensor=self.tensor.transpose(1, 2).clone(), disable_checks=True)
 
     def to_matrix(self) -> torch.Tensor:
-        ret = self.tensor.new_zeros(self.shape[0], 4, 4)
-        ret[:, :3] = self.tensor
-        ret[:, 3, 3] = 1
-        return ret
+        return self.tensor.clone()
 
     # The quaternion takes the [w x y z] convention
-    def update_from_x_y_z_quaternion(self, x_y_z_quaternion: torch.Tensor):
-        self.update(SE3.x_y_z_unit_quaternion_to_SE3(x_y_z_quaternion))
-
-    def update_from_rot_and_trans(self, rotation: SO3, translation: Point3):
-        if rotation.shape[0] != translation.shape[0]:
-            raise ValueError("rotation and translation must have the same batch size.")
-
-        if rotation.dtype != translation.dtype:
-            raise ValueError("rotation and translation must be of the same type.")
-
-        if rotation.device != translation.device:
-            raise ValueError("rotation and translation must be on the same device.")
-
-        self.tensor = torch.cat(
-            (rotation.tensor, translation.tensor.unsqueeze(2)), dim=2
+    def to_quaternion(self) -> torch.Tensor:
+        sine_axis = self.tensor.new_zeros(self.shape[0], 3)
+        sine_axis[:, 0] = 0.5 * (self[:, 2, 1] - self[:, 1, 2])
+        sine_axis[:, 1] = 0.5 * (self[:, 0, 2] - self[:, 2, 0])
+        sine_axis[:, 2] = 0.5 * (self[:, 1, 0] - self[:, 0, 1])
+        w = 0.5 * (1 + self[:, 0, 0] + self[:, 1, 1] + self[:, 2, 2]).clamp(0, 4).sqrt()
+
+        near_zero = w > 1 - _THESEUS_GLOBAL_PARAMS.get_eps("so3", "near_zero", w.dtype)
+        near_pi = w <= _THESEUS_GLOBAL_PARAMS.get_eps("so3", "near_pi", w.dtype)
+        non_zero = self.tensor.new_ones([1])
+
+        ret = self.tensor.new_zeros(self.shape[0], 4)
+        # theta != pi
+        ret[:, 0] = w
+        ret[:, 1:] = 0.5 * sine_axis / torch.where(near_pi, non_zero, w).view(-1, 1)
+
+        # theta ~ pi
+        ddiag = torch.diagonal(self.tensor, dim1=1, dim2=2)
+        # Find the index of major coloumns and diagonals
+        major = torch.logical_and(
+            ddiag[:, 1] > ddiag[:, 0], ddiag[:, 1] > ddiag[:, 2]
+        ) + 2 * torch.logical_and(ddiag[:, 2] > ddiag[:, 0], ddiag[:, 2] > ddiag[:, 1])
+        aux = torch.ones(self.shape[0], dtype=torch.bool)
+        sel_rows = 0.5 * (self[aux, major] + self[aux, :, major])
+        cosine_near_pi = 0.5 * (self[:, 0, 0] + self[:, 1, 1] + self[:, 2, 2] - 1)
+        sel_rows[aux, major] -= cosine_near_pi
+        axis = (
+            sel_rows
+            / torch.where(
+                near_zero.view(-1, 1),
+                non_zero.view(-1, 1),
+                sel_rows.norm(dim=1, keepdim=True),
+            )
+            * torch.where(sine_axis[aux, major].view(-1, 1) >= 0, non_zero, -non_zero)
         )
+        sine_half_theta = (0.5 * (1 - cosine_near_pi)).clamp(0, 1).sqrt().view(-1, 1)
+        ret[:, 1:] = torch.where(
+            near_pi.view(-1, 1), axis * sine_half_theta, ret[:, 1:]
+        )
+
+        return ret
 
     @staticmethod
     def hat(tangent_vector: torch.Tensor) -> torch.Tensor:
-        return SE3_base.hat(tangent_vector)
+        return SO3_base.hat(tangent_vector)
 
     @staticmethod
     def vee(matrix: torch.Tensor) -> torch.Tensor:
-        return SE3_base.vee(matrix)
+        SO3._hat_matrix_check(matrix)
+        return SO3_base.vee(matrix)
 
-    def _copy_impl(self, new_name: Optional[str] = None) -> "SE3":
-        # if self.tensor is a valid SE3, so is the copy
-        return SE3(tensor=self.tensor.clone(), name=new_name, strict=False)
-
-    # only added to avoid casting downstream
-    def copy(self, new_name: Optional[str] = None) -> "SE3":
-        return cast(SE3, super().copy(new_name=new_name))
-
-    def _transform_shape_check(self, point: Union[Point3, torch.Tensor]):
+    def _rotate_shape_check(self, point: Union[Point3, torch.Tensor]):
         err_msg = (
-            f"SE3 can only transform vectors of shape [{self.shape[0]}, 3] or [1, 3], "
-            f"but the input has shape {point.shape}."
+            f"Point tensor to rotate must have final dimensions of shape (3,) "
+            f"or (3, 1), and be broadcastable with SO3, but received a tensor with "
+            f"shape {point.shape}, while SO3 shape is {self.shape}."
         )
-
         if isinstance(point, torch.Tensor):
-            if not point.ndim == 2 or point.shape[1] != 3:
+            if (
+                point.ndim not in [2, 3]
+                or point.shape[1] != 3
+                or (point.ndim == 3 and point.shape[-1] != 1)
+            ):
                 raise ValueError(err_msg)
+
         elif point.dof() != 3:
             raise ValueError(err_msg)
         if (
             point.shape[0] != self.shape[0]
             and point.shape[0] != 1
             and self.shape[0] != 1
         ):
             raise ValueError(err_msg)
 
-    def transform_from(
+    # The quaternion takes the [w x y z] convention
+    @staticmethod
+    def unit_quaternion_to_SO3(quaternion: torch.Tensor) -> "SO3":
+        if quaternion.ndim == 1:
+            quaternion = quaternion.unsqueeze(0)
+        return SO3(
+            tensor=SO3_base.quaternion_to_rotation(quaternion), disable_checks=True
+        )
+
+    def _copy_impl(self, new_name: Optional[str] = None) -> "SO3":
+        # if self.tensor is a valid SO(3), so is the copy
+        return SO3(tensor=self.tensor.clone(), name=new_name, disable_checks=True)
+
+    # only added to avoid casting downstream
+    def copy(self, new_name: Optional[str] = None) -> "SO3":
+        return cast(SO3, super().copy(new_name=new_name))
+
+    def rotate(
         self,
         point: Union[Point3, torch.Tensor],
         jacobians: Optional[List[torch.Tensor]] = None,
     ) -> Point3:
-        self._transform_shape_check(point)
+        self._rotate_shape_check(point)
         p = point if isinstance(point, torch.Tensor) else point.tensor
-        return Point3(SE3_base.transform_from(self.tensor, p, jacobians=jacobians))
+        return Point3(tensor=SO3_base.transform(self.tensor, p, jacobians=jacobians))
 
-    def transform_to(
+    def unrotate(
         self,
         point: Union[Point3, torch.Tensor],
         jacobians: Optional[List[torch.Tensor]] = None,
     ) -> Point3:
-        self._transform_shape_check(point)
-        batch_size = max(self.shape[0], point.shape[0])
-        if isinstance(point, torch.Tensor):
-            p = point.view(-1, 3, 1)
-        else:
-            p = point.tensor.view(-1, 3, 1)
-
-        temp = p - self[:, :, 3:]
-        ret = Point3(tensor=(self[:, :, :3].transpose(1, 2) @ temp).view(-1, 3))
-
-        if jacobians is not None:
-            self._check_jacobians_list(jacobians)
-            # Right jacobians for SE3 are computed
-            Jg = torch.zeros(batch_size, 3, 6, dtype=self.dtype, device=self.device)
-            Jg[:, 0, 0] = -1
-            Jg[:, 1, 1] = -1
-            Jg[:, 2, 2] = -1
-            Jg[:, 0, 4] = -ret[:, 2]
-            Jg[:, 1, 3] = ret[:, 2]
-            Jg[:, 0, 5] = ret[:, 1]
-            Jg[:, 2, 3] = -ret[:, 1]
-            Jg[:, 1, 5] = -ret[:, 0]
-            Jg[:, 2, 4] = ret[:, 0]
-            # Jacobians for point
-            Jpnt = self[:, :, :3].transpose(1, 2).expand(batch_size, 3, 3)
-
-            jacobians.extend([Jg, Jpnt])
-
-        return ret
-
-    # The returned tensor will have 7 elements, [x, y, z, qw, qx, qy, qz] where
-    # [x y z] corresponds to the translation and [qw qx qy qz] to the quaternion
-    # using the [w x y z] convention
-    def to_x_y_z_quaternion(self) -> torch.Tensor:
-        ret = self.tensor.new_zeros(self.shape[0], 7)
-        ret[:, :3] = self.tensor[:, :, 3]
-        with no_lie_group_check(silent=True):
-            ret[:, 3:] = SO3(tensor=self.tensor[:, :, :3]).to_quaternion()
-        return ret
-
-    def rotation(self) -> SO3:
-        with no_lie_group_check(silent=True):
-            return SO3(tensor=self.tensor[:, :, :3])
-
-    def translation(self) -> Point3:
-        with no_lie_group_check(silent=True):
-            return Point3(tensor=self.tensor[:, :, 3].view(-1, 3))
-
-    # calls to() on the internal tensors
-    def to(self, *args, **kwargs):
-        super().to(*args, **kwargs)
+        self._rotate_shape_check(point)
+        p = point if isinstance(point, torch.Tensor) else point.tensor
+        return Point3(tensor=SO3_base.untransform(self.tensor, p, jacobians=jacobians))
 
 
-rand_se3 = SE3.rand
-randn_se3 = SE3.randn
+rand_so3 = SO3.rand
+randn_so3 = SO3.randn
```

### Comparing `theseus-ai-0.2.0.dev0/theseus/geometry/so2.py` & `theseus-ai-0.2.1/theseus/geometry/so2.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,35 +5,42 @@
 
 import warnings
 from typing import List, Optional, Tuple, Union, cast
 
 import torch
 
 import theseus.constants
-from theseus.options import _THESEUS_GLOBAL_OPTIONS
+from theseus.global_params import _THESEUS_GLOBAL_PARAMS
 
 from .lie_group import LieGroup
 from .lie_group_check import _LieGroupCheckContext
 from .point_types import Point2
 
 
 class SO2(LieGroup):
     def __init__(
         self,
         theta: Optional[torch.Tensor] = None,
         tensor: Optional[torch.Tensor] = None,
         name: Optional[str] = None,
         dtype: Optional[torch.dtype] = None,
-        strict: bool = False,
+        strict_checks: bool = False,
+        disable_checks: bool = False,
     ):
         if theta is not None and tensor is not None:
             raise ValueError("Please provide only one of theta or tensor.")
         if theta is not None:
             dtype = theta.dtype
-        super().__init__(tensor=tensor, name=name, dtype=dtype, strict=strict)
+        super().__init__(
+            tensor=tensor,
+            name=name,
+            dtype=dtype,
+            strict_checks=strict_checks,
+            disable_checks=disable_checks,
+        )
         if theta is not None:
             if theta.ndim == 1:
                 theta = theta.unsqueeze(1)
             if theta.ndim != 2 or theta.shape[1] != 1:
                 raise ValueError(
                     "Argument theta must be have ndim = 1, or ndim=2 and shape[1] = 1."
                 )
@@ -123,15 +130,15 @@
 
     @staticmethod
     def _check_tensor_impl(tensor: torch.Tensor) -> bool:
         with torch.no_grad():
             if tensor.ndim != 2 or tensor.shape[1] != 2:
                 raise ValueError("SO2 data tensors can only be 2D vectors.")
 
-            MATRIX_EPS = _THESEUS_GLOBAL_OPTIONS.get_eps("so2", "matrix", tensor.dtype)
+            MATRIX_EPS = _THESEUS_GLOBAL_PARAMS.get_eps("so2", "matrix", tensor.dtype)
             if tensor.dtype != torch.float64:
                 tensor = tensor.double()
 
             _check = (
                 torch.linalg.norm(tensor, dim=1) - 1
             ).abs().max().item() <= MATRIX_EPS
 
@@ -179,15 +186,15 @@
 
     @staticmethod
     def normalize(tensor: torch.Tensor) -> torch.Tensor:
         if tensor.ndim != 2 or tensor.shape[1] != 2:
             raise ValueError("SO2 data tensors can only be 2D vectors.")
 
         data_norm = torch.norm(tensor, dim=1, keepdim=True)
-        near_zero = data_norm < _THESEUS_GLOBAL_OPTIONS.get_eps(
+        near_zero = data_norm < _THESEUS_GLOBAL_PARAMS.get_eps(
             "so2", "norm", tensor.dtype
         )
         data_norm_nz = torch.where(
             near_zero,
             torch.tensor(1.0, dtype=tensor.dtype, device=tensor.device),
             data_norm,
         )
@@ -216,19 +223,19 @@
 
     def _compose_impl(self, so2_2: LieGroup) -> "SO2":
         so2_2 = cast(SO2, so2_2)
         cos_1, sin_1 = self.to_cos_sin()
         cos_2, sin_2 = so2_2.to_cos_sin()
         new_cos = cos_1 * cos_2 - sin_1 * sin_2
         new_sin = sin_1 * cos_2 + cos_1 * sin_2
-        return SO2(tensor=torch.stack([new_cos, new_sin], dim=1), strict=False)
+        return SO2(tensor=torch.stack([new_cos, new_sin], dim=1), disable_checks=True)
 
     def _inverse_impl(self, get_jacobian: bool = False) -> "SO2":
         cosine, sine = self.to_cos_sin()
-        return SO2(tensor=torch.stack([cosine, -sine], dim=1), strict=False)
+        return SO2(tensor=torch.stack([cosine, -sine], dim=1), disable_checks=True)
 
     def _rotate_shape_check(self, point: Union[Point2, torch.Tensor]):
         err_msg = (
             f"SO2 can only transform vectors of shape [{self.shape[0]}, 2] or [1, 2], "
             f"but the input has shape {point.shape}."
         )
```

### Comparing `theseus-ai-0.2.0.dev0/theseus/geometry/so3.py` & `theseus-ai-0.2.1/theseus/geometry/se3.py`

 * *Files 27% similar despite different names*

```diff
@@ -3,304 +3,289 @@
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
 import warnings
 from typing import List, Optional, Union, cast
 
 import torch
-from lie.functional import SO3 as SO3_base
 
 import theseus.constants
-from theseus.options import _THESEUS_GLOBAL_OPTIONS
+from torchlie.functional import SE3 as SE3_base
+
 from .lie_group import LieGroup
-from .lie_group_check import _LieGroupCheckContext
+from .lie_group_check import _LieGroupCheckContext, no_lie_group_check
 from .point_types import Point3
+from .so3 import SO3
 
 
-class SO3(LieGroup):
+class SE3(LieGroup):
     def __init__(
         self,
-        quaternion: Optional[torch.Tensor] = None,
+        x_y_z_quaternion: Optional[torch.Tensor] = None,
         tensor: Optional[torch.Tensor] = None,
         name: Optional[str] = None,
         dtype: Optional[torch.dtype] = None,
-        strict: bool = False,
+        strict_checks: bool = False,
+        disable_checks: bool = False,
     ):
-        if quaternion is not None and tensor is not None:
-            raise ValueError("Please provide only one of quaternion or tensor.")
-        if quaternion is not None:
-            dtype = quaternion.dtype
-        super().__init__(tensor=tensor, name=name, dtype=dtype, strict=strict)
-        if quaternion is not None:
-            self.update_from_unit_quaternion(quaternion)
+        if x_y_z_quaternion is not None and tensor is not None:
+            raise ValueError("Please provide only one of x_y_z_quaternion or tensor.")
+        if x_y_z_quaternion is not None:
+            dtype = x_y_z_quaternion.dtype
+        super().__init__(
+            tensor=tensor,
+            name=name,
+            dtype=dtype,
+            strict_checks=strict_checks,
+            disable_checks=disable_checks,
+        )
+        if x_y_z_quaternion is not None:
+            self.update_from_x_y_z_quaternion(x_y_z_quaternion=x_y_z_quaternion)
 
     @staticmethod
     def rand(
         *size: int,
         generator: Optional[torch.Generator] = None,
         dtype: Optional[torch.dtype] = None,
         device: theseus.constants.DeviceType = None,
         requires_grad: bool = False,
-    ) -> "SO3":
+    ) -> "SE3":
         if len(size) != 1:
             raise ValueError("The size should be 1D.")
-        tensor = SO3_base.rand(
+        tensor = SE3_base.rand(
             *size,
             generator=generator,
             dtype=dtype,
             device=device,
             requires_grad=requires_grad,
         )
-        return SO3(tensor=tensor)
+        return SE3(tensor=tensor, disable_checks=True)
 
     @staticmethod
     def randn(
         *size: int,
         generator: Optional[torch.Generator] = None,
         dtype: Optional[torch.dtype] = None,
         device: theseus.constants.DeviceType = None,
         requires_grad: bool = False,
-    ) -> "SO3":
+    ) -> "SE3":
         if len(size) != 1:
             raise ValueError("The size should be 1D.")
-        tensor = SO3_base.randn(
+        tensor = SE3_base.randn(
             *size,
             generator=generator,
             dtype=dtype,
             device=device,
             requires_grad=requires_grad,
         )
-        return SO3(tensor=tensor)
+        return SE3(tensor=tensor, disable_checks=True)
 
     @staticmethod
     def _init_tensor() -> torch.Tensor:  # type: ignore
-        return torch.eye(3, 3).view(1, 3, 3)
-
-    def update_from_unit_quaternion(self, quaternion: torch.Tensor):
-        self.update(self.unit_quaternion_to_SO3(quaternion))
+        return torch.eye(3, 4).view(1, 3, 4)
 
     def dof(self) -> int:
-        return 3
+        return 6
 
     def __repr__(self) -> str:
-        return f"SO3(tensor={self.tensor}, name={self.name})"
+        return f"SE3(tensor={self.tensor}, name={self.name})"
 
     def __str__(self) -> str:
         with torch.no_grad():
-            return f"SO3(matrix={self.tensor}), name={self.name})"
+            return f"SE3(matrix={self.tensor}), name={self.name})"
 
     def _adjoint_impl(self) -> torch.Tensor:
-        return self.tensor.clone()
+        return SE3_base.adj(self.tensor)
 
     def _project_impl(
         self, euclidean_grad: torch.Tensor, is_sparse: bool = False
     ) -> torch.Tensor:
         self._project_check(euclidean_grad, is_sparse)
         if is_sparse:
-            return SO3_base.left_project(self.tensor, euclidean_grad)
+            return SE3_base.left_project(self.tensor, euclidean_grad)
         else:
-            ret = self.tensor.new_zeros(euclidean_grad.shape[:-1])
-            temp = torch.einsum("...jk,...ji->...ik", euclidean_grad, self.tensor)
-            ret[..., 0] = temp[..., 2, 1] - temp[..., 1, 2]
-            ret[..., 1] = temp[..., 0, 2] - temp[..., 2, 0]
-            ret[..., 2] = temp[..., 1, 0] - temp[..., 0, 1]
+            ret = self.tensor.new_zeros(euclidean_grad.shape[:-2] + torch.Size([6]))
+            temp = torch.einsum(
+                "...jk,...ji->...ik", euclidean_grad, self.tensor[:, :, :3]
+            )
+            ret[..., :3] = temp[..., 3]
+            ret[..., 3] = temp[..., 2, 1] - temp[..., 1, 2]
+            ret[..., 4] = temp[..., 0, 2] - temp[..., 2, 0]
+            ret[..., 5] = temp[..., 1, 0] - temp[..., 0, 1]
+
             return ret
 
     @staticmethod
     def _check_tensor_impl(tensor: torch.Tensor) -> bool:
-        with torch.no_grad():
-            if tensor.ndim != 3 or tensor.shape[1:] != (3, 3):
-                raise ValueError("SO3 data tensors can only be 3x3 matrices.")
-            try:
-                SO3_base.check_group_tensor(tensor)
-            except ValueError:
-                return False
+        if tensor.ndim != 3 or tensor.shape[1:] != (3, 4):
+            raise ValueError("SE3 data tensors can only be 3x4 matrices.")
+        try:
+            SE3_base.check_group_tensor(tensor)
+        except ValueError:
+            return False
         return True
 
     @staticmethod
-    def _unit_quaternion_check(quaternion: torch.Tensor):
-        if quaternion.ndim != 2 or quaternion.shape[1] != 4:
-            raise ValueError("Quaternions can only be 4-D vectors.")
+    def x_y_z_unit_quaternion_to_SE3(x_y_z_quaternion: torch.Tensor) -> "SE3":
+        if x_y_z_quaternion.ndim == 1:
+            x_y_z_quaternion = x_y_z_quaternion.unsqueeze(0)
+
+        if x_y_z_quaternion.ndim != 2 and x_y_z_quaternion.shape[1] != 7:
+            raise ValueError("x_y_z_quaternion can only be 7-D vectors.")
+
+        ret = SE3()
+
+        batch_size = x_y_z_quaternion.shape[0]
+        ret.tensor = torch.empty(batch_size, 3, 4).to(
+            device=x_y_z_quaternion.device, dtype=x_y_z_quaternion.dtype
+        )
+        ret[:, :, :3] = SO3.unit_quaternion_to_SO3(x_y_z_quaternion[:, 3:]).tensor
+        ret[:, :, 3] = x_y_z_quaternion[:, :3]
 
-        checks_enabled, silent_unchecks = _LieGroupCheckContext.get_context()
-        if checks_enabled:
-            SO3_base.check_unit_quaternion(quaternion)
-        elif not silent_unchecks:
-            warnings.warn(
-                "Lie group checks are disabled, so the validness of unit quaternions is not "
-                "checked for SO3.",
-                RuntimeWarning,
-            )
+        return ret
 
     @staticmethod
     def _hat_matrix_check(matrix: torch.Tensor):
-        if matrix.ndim != 3 or matrix.shape[1:] != (3, 3):
-            raise ValueError("Hat matrices of SO(3) can only be 3x3 matrices")
+        if matrix.ndim != 3 or matrix.shape[1:] != (4, 4):
+            raise ValueError("Hat matrices of SE3 can only be 4x4 matrices")
 
         checks_enabled, silent_unchecks = _LieGroupCheckContext.get_context()
         if checks_enabled:
-            SO3_base.check_hat_tensor(matrix)
+            return SE3_base.check_hat_tensor(matrix)
         elif not silent_unchecks:
             warnings.warn(
                 "Lie group checks are disabled, so the skew-symmetry of hat matrices is "
-                "not checked for SO3.",
+                "not checked for SE3.",
                 RuntimeWarning,
             )
 
     @staticmethod
     def exp_map(
         tangent_vector: torch.Tensor, jacobians: Optional[List[torch.Tensor]] = None
-    ) -> "SO3":
-        if tangent_vector.ndim != 2 or tangent_vector.shape[1] != 3:
-            raise ValueError("Tangent vectors of SO3 should be batched 3-D vectors.")
-        return SO3(tensor=SO3_base.exp(tangent_vector, jacobians=jacobians))
+    ) -> "SE3":
+        if tangent_vector.ndim != 2 or tangent_vector.shape[1] != 6:
+            raise ValueError("Tangent vectors of SE3 can only be 6D vectors.")
+        return SE3(
+            tensor=SE3_base.exp(tangent_vector, jacobians=jacobians),
+            disable_checks=True,
+        )
 
     @staticmethod
     def normalize(tensor: torch.Tensor) -> torch.Tensor:
-        if tensor.ndim != 3 or tensor.shape[1:] != (3, 3):
-            raise ValueError("SO3 data tensors can only be batched 3x3 matrices.")
-        return SO3_base.normalize(tensor)
+        if tensor.ndim != 3 or tensor.shape[1:] != (3, 4):
+            raise ValueError("SE3 data tensors can only be 3x4 matrices.")
+        return SE3_base.normalize(tensor)
 
     def _log_map_impl(
         self, jacobians: Optional[List[torch.Tensor]] = None
     ) -> torch.Tensor:
-        return SO3_base.log(self.tensor, jacobians=jacobians)
+        return SE3_base.log(self.tensor, jacobians=jacobians)
 
-    def _compose_impl(self, so3_2: LieGroup) -> "SO3":
-        return SO3(tensor=SO3_base.compose(self.tensor, so3_2.tensor))
+    def _compose_impl(self, se3_2: LieGroup) -> "SE3":
+        return SE3(
+            tensor=SE3_base.compose(self.tensor, se3_2.tensor), strict_checks=False
+        )
 
-    def _inverse_impl(self, get_jacobian: bool = False) -> "SO3":
-        # if self.tensor is a valid SO(3), then self.tensor.transpose(1, 2)
-        # must be valid as well
-        return SO3(tensor=self.tensor.transpose(1, 2).clone(), strict=False)
+    def _inverse_impl(self, get_jacobian: bool = False) -> "SE3":
+        return SE3(tensor=SE3_base.inv(self.tensor), disable_checks=True)
 
     def to_matrix(self) -> torch.Tensor:
-        return self.tensor.clone()
+        ret = self.tensor.new_zeros(self.shape[0], 4, 4)
+        ret[:, :3] = self.tensor
+        ret[:, 3, 3] = 1
+        return ret
 
     # The quaternion takes the [w x y z] convention
-    def to_quaternion(self) -> torch.Tensor:
-        sine_axis = self.tensor.new_zeros(self.shape[0], 3)
-        sine_axis[:, 0] = 0.5 * (self[:, 2, 1] - self[:, 1, 2])
-        sine_axis[:, 1] = 0.5 * (self[:, 0, 2] - self[:, 2, 0])
-        sine_axis[:, 2] = 0.5 * (self[:, 1, 0] - self[:, 0, 1])
-        w = 0.5 * (1 + self[:, 0, 0] + self[:, 1, 1] + self[:, 2, 2]).clamp(0, 4).sqrt()
-
-        near_zero = w > 1 - _THESEUS_GLOBAL_OPTIONS.get_eps("so3", "near_zero", w.dtype)
-        near_pi = w <= _THESEUS_GLOBAL_OPTIONS.get_eps("so3", "near_pi", w.dtype)
-        non_zero = self.tensor.new_ones([1])
-
-        ret = self.tensor.new_zeros(self.shape[0], 4)
-        # theta != pi
-        ret[:, 0] = w
-        ret[:, 1:] = 0.5 * sine_axis / torch.where(near_pi, non_zero, w).view(-1, 1)
-
-        # theta ~ pi
-        ddiag = torch.diagonal(self.tensor, dim1=1, dim2=2)
-        # Find the index of major coloumns and diagonals
-        major = torch.logical_and(
-            ddiag[:, 1] > ddiag[:, 0], ddiag[:, 1] > ddiag[:, 2]
-        ) + 2 * torch.logical_and(ddiag[:, 2] > ddiag[:, 0], ddiag[:, 2] > ddiag[:, 1])
-        aux = torch.ones(self.shape[0], dtype=torch.bool)
-        sel_rows = 0.5 * (self[aux, major] + self[aux, :, major])
-        cosine_near_pi = 0.5 * (self[:, 0, 0] + self[:, 1, 1] + self[:, 2, 2] - 1)
-        sel_rows[aux, major] -= cosine_near_pi
-        axis = (
-            sel_rows
-            / torch.where(
-                near_zero.view(-1, 1),
-                non_zero.view(-1, 1),
-                sel_rows.norm(dim=1, keepdim=True),
-            )
-            * torch.where(sine_axis[aux, major].view(-1, 1) >= 0, non_zero, -non_zero)
-        )
-        sine_half_theta = (0.5 * (1 - cosine_near_pi)).clamp(0, 1).sqrt().view(-1, 1)
-        ret[:, 1:] = torch.where(
-            near_pi.view(-1, 1), axis * sine_half_theta, ret[:, 1:]
-        )
+    def update_from_x_y_z_quaternion(self, x_y_z_quaternion: torch.Tensor):
+        self.update(SE3.x_y_z_unit_quaternion_to_SE3(x_y_z_quaternion))
 
-        return ret
+    def update_from_rot_and_trans(self, rotation: SO3, translation: Point3):
+        if rotation.shape[0] != translation.shape[0]:
+            raise ValueError("rotation and translation must have the same batch size.")
+
+        if rotation.dtype != translation.dtype:
+            raise ValueError("rotation and translation must be of the same type.")
+
+        if rotation.device != translation.device:
+            raise ValueError("rotation and translation must be on the same device.")
+
+        self.tensor = torch.cat(
+            (rotation.tensor, translation.tensor.unsqueeze(2)), dim=2
+        )
 
     @staticmethod
     def hat(tangent_vector: torch.Tensor) -> torch.Tensor:
-        return SO3_base.hat(tangent_vector)
+        return SE3_base.hat(tangent_vector)
 
     @staticmethod
     def vee(matrix: torch.Tensor) -> torch.Tensor:
-        SO3._hat_matrix_check(matrix)
-        return SO3_base.vee(matrix)
+        return SE3_base.vee(matrix)
+
+    def _copy_impl(self, new_name: Optional[str] = None) -> "SE3":
+        # if self.tensor is a valid SE3, so is the copy
+        return SE3(tensor=self.tensor.clone(), name=new_name, disable_checks=True)
 
-    def _rotate_shape_check(self, point: Union[Point3, torch.Tensor]):
+    # only added to avoid casting downstream
+    def copy(self, new_name: Optional[str] = None) -> "SE3":
+        return cast(SE3, super().copy(new_name=new_name))
+
+    def _transform_shape_check(self, point: Union[Point3, torch.Tensor]):
         err_msg = (
-            f"SO3 can only rotate vectors of shape [{self.shape[0]}, 3] or [1, 3], "
+            f"SE3 can only transform vectors of shape [{self.shape[0]}, 3] or [1, 3], "
             f"but the input has shape {point.shape}."
         )
+
         if isinstance(point, torch.Tensor):
             if not point.ndim == 2 or point.shape[1] != 3:
                 raise ValueError(err_msg)
         elif point.dof() != 3:
             raise ValueError(err_msg)
         if (
             point.shape[0] != self.shape[0]
             and point.shape[0] != 1
             and self.shape[0] != 1
         ):
             raise ValueError(err_msg)
 
-    # The quaternion takes the [w x y z] convention
-    @staticmethod
-    def unit_quaternion_to_SO3(quaternion: torch.Tensor) -> "SO3":
-        if quaternion.ndim == 1:
-            quaternion = quaternion.unsqueeze(0)
-        return SO3(tensor=SO3_base.quaternion_to_rotation(quaternion))
-
-    def _copy_impl(self, new_name: Optional[str] = None) -> "SO3":
-        # if self.tensor is a valid SO(3), so is the copy
-        return SO3(tensor=self.tensor.clone(), name=new_name, strict=False)
-
-    # only added to avoid casting downstream
-    def copy(self, new_name: Optional[str] = None) -> "SO3":
-        return cast(SO3, super().copy(new_name=new_name))
-
-    def rotate(
+    def transform_from(
         self,
         point: Union[Point3, torch.Tensor],
         jacobians: Optional[List[torch.Tensor]] = None,
     ) -> Point3:
-        self._rotate_shape_check(point)
+        self._transform_shape_check(point)
         p = point if isinstance(point, torch.Tensor) else point.tensor
-        return Point3(
-            tensor=SO3_base.transform_from(self.tensor, p, jacobians=jacobians)
-        )
+        return Point3(SE3_base.transform(self.tensor, p, jacobians=jacobians))
 
-    def unrotate(
+    def transform_to(
         self,
         point: Union[Point3, torch.Tensor],
         jacobians: Optional[List[torch.Tensor]] = None,
     ) -> Point3:
-        self._rotate_shape_check(point)
-        batch_size = max(self.shape[0], point.shape[0])
-        if isinstance(point, torch.Tensor):
-            p = point.view(-1, 3, 1)
-        else:
-            p = point.tensor.view(-1, 3, 1)
+        self._transform_shape_check(point)
+        p = point if isinstance(point, torch.Tensor) else point.tensor
+        return Point3(SE3_base.untransform(self.tensor, p, jacobians=jacobians))
 
-        ret = Point3(tensor=(self.tensor.transpose(1, 2) @ p).view(-1, 3))
-        if jacobians is not None:
-            self._check_jacobians_list(jacobians)
-            # Left jacobians for SO3 are computed
-            Jrot = self.tensor.new_zeros(batch_size, 3, 3)
-            Jrot[:, 0, 1] = -ret[:, 2]
-            Jrot[:, 1, 0] = ret[:, 2]
-            Jrot[:, 0, 2] = ret[:, 1]
-            Jrot[:, 2, 0] = -ret[:, 1]
-            Jrot[:, 1, 2] = -ret[:, 0]
-            Jrot[:, 2, 1] = ret[:, 0]
-            # Jacobians for point
-            Jpnt = self.to_matrix().transpose(1, 2).expand(batch_size, 3, 3)
+    # The returned tensor will have 7 elements, [x, y, z, qw, qx, qy, qz] where
+    # [x y z] corresponds to the translation and [qw qx qy qz] to the quaternion
+    # using the [w x y z] convention
+    def to_x_y_z_quaternion(self) -> torch.Tensor:
+        ret = self.tensor.new_zeros(self.shape[0], 7)
+        ret[:, :3] = self.tensor[:, :, 3]
+        ret[:, 3:] = SO3(
+            tensor=self.tensor[:, :, :3], disable_checks=True
+        ).to_quaternion()
+        return ret
 
-            jacobians.extend([Jrot, Jpnt])
+    def rotation(self) -> SO3:
+        return SO3(tensor=self.tensor[:, :, :3], disable_checks=True)
 
-        return ret
+    def translation(self) -> Point3:
+        with no_lie_group_check(silent=True):
+            return Point3(tensor=self.tensor[:, :, 3].view(-1, 3))
+
+    # calls to() on the internal tensors
+    def to(self, *args, **kwargs):
+        super().to(*args, **kwargs)
 
 
-rand_so3 = SO3.rand
-randn_so3 = SO3.randn
+rand_se3 = SE3.rand
+randn_se3 = SE3.randn
```

### Comparing `theseus-ai-0.2.0.dev0/theseus/geometry/utils.py` & `theseus-ai-0.2.1/theseus/geometry/utils.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-0.2.0.dev0/theseus/geometry/vector.py` & `theseus-ai-0.2.1/theseus/geometry/vector.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-0.2.0.dev0/theseus/optimizer/autograd/baspacho_sparse_autograd.py` & `theseus-ai-0.2.1/theseus/optimizer/autograd/baspacho_sparse_autograd.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
-from typing import Any, Tuple, Optional
+from typing import Any, Optional, Tuple
+
 import torch
 
-from .common import compute_A_grad
-from ..linear_system import SparseStructure
 from theseus.utils.sparse_matrix_utils import mat_vec, tmat_vec
 
+from ..linear_system import SparseStructure
+from .common import compute_A_grad
+
 _BaspachoSolveFunctionBwdReturnType = Tuple[
     torch.Tensor, torch.Tensor, None, None, None, None, None, None, None
 ]
 
 
 class BaspachoSolveFunction(torch.autograd.Function):
     @staticmethod
```

### Comparing `theseus-ai-0.2.0.dev0/theseus/optimizer/autograd/cholmod_sparse_autograd.py` & `theseus-ai-0.2.1/theseus/optimizer/autograd/cholmod_sparse_autograd.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 from typing import Any, Tuple
 
 import torch
 from sksparse.cholmod import Factor as CholeskyDecomposition
 
-from .common import compute_A_grad
 from ..linear_system import SparseStructure
+from .common import compute_A_grad
 
 _CholmodSolveFunctionBwdReturnType = Tuple[
     torch.Tensor, torch.Tensor, None, None, None, None
 ]
 
 
 class CholmodSolveFunction(torch.autograd.Function):
```

### Comparing `theseus-ai-0.2.0.dev0/theseus/optimizer/autograd/common.py` & `theseus-ai-0.2.1/theseus/optimizer/autograd/common.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-0.2.0.dev0/theseus/optimizer/autograd/lu_cuda_sparse_autograd.py` & `theseus-ai-0.2.1/theseus/optimizer/autograd/lu_cuda_sparse_autograd.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 from typing import Any, Optional, Tuple
+
 import torch
 
 from ..linear_system import SparseStructure
 from .common import compute_A_grad
 
 _LUCudaSolveFunctionBwdReturnType = Tuple[
     torch.Tensor, torch.Tensor, None, None, None, None, None, None, None
```

### Comparing `theseus-ai-0.2.0.dev0/theseus/optimizer/dense_linearization.py` & `theseus-ai-0.2.1/theseus/optimizer/dense_linearization.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-0.2.0.dev0/theseus/optimizer/linear/__init__.py` & `theseus-ai-0.2.1/theseus/optimizer/linear/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
 import torch
 
+from .baspacho_sparse_solver import BaspachoSparseSolver
+from .cholmod_sparse_solver import CholmodSparseSolver
 from .dense_solver import CholeskyDenseSolver, DenseSolver, LUDenseSolver
 from .linear_optimizer import LinearOptimizer
 from .linear_solver import LinearSolver
-from .baspacho_sparse_solver import BaspachoSparseSolver
 from .lu_cuda_sparse_solver import LUCudaSparseSolver
-from .cholmod_sparse_solver import CholmodSparseSolver
```

### Comparing `theseus-ai-0.2.0.dev0/theseus/optimizer/linear/baspacho_sparse_solver.py` & `theseus-ai-0.2.1/theseus/optimizer/linear/baspacho_sparse_solver.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
 from typing import Any, Dict, Optional, Type, Union
 
+import numpy as np
 import torch
+from scipy.sparse import csr_matrix
 
 from theseus.constants import DeviceType
 from theseus.core import Objective
 from theseus.optimizer import Linearization, SparseLinearization
 from theseus.optimizer.autograd import BaspachoSolveFunction
 
 from .linear_solver import LinearSolver
 from .utils import convert_to_alpha_beta_damping_tensors
-from scipy.sparse import csr_matrix
-import numpy as np
 
 # assuming the want to use cuda if supported and available
 DEFAULT_DEVICE = "cuda" if torch.cuda.is_available() else "cpu"
 
 
 class BaspachoSparseSolver(LinearSolver):
     def __init__(
```

### Comparing `theseus-ai-0.2.0.dev0/theseus/optimizer/linear/cholmod_sparse_solver.py` & `theseus-ai-0.2.1/theseus/optimizer/linear/cholmod_sparse_solver.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-0.2.0.dev0/theseus/optimizer/linear/dense_solver.py` & `theseus-ai-0.2.1/theseus/optimizer/linear/dense_solver.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-0.2.0.dev0/theseus/optimizer/linear/linear_optimizer.py` & `theseus-ai-0.2.1/theseus/optimizer/linear/linear_optimizer.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-0.2.0.dev0/theseus/optimizer/linear/linear_solver.py` & `theseus-ai-0.2.1/theseus/optimizer/linear/linear_solver.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-0.2.0.dev0/theseus/optimizer/linear/lu_cuda_sparse_solver.py` & `theseus-ai-0.2.1/theseus/optimizer/linear/lu_cuda_sparse_solver.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-0.2.0.dev0/theseus/optimizer/linear/utils.py` & `theseus-ai-0.2.1/theseus/optimizer/linear/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 from typing import Tuple, Union
+
 import torch
+
 from theseus.constants import DeviceType
 
 
 # See Nocedal and Wright, Numerical Optimization, pp. 260 and 261
 # https://www.csie.ntu.edu.tw/~r97002/temp/num_optimization.pdf
 def convert_to_alpha_beta_damping_tensors(
     damping: Union[float, torch.Tensor],
```

### Comparing `theseus-ai-0.2.0.dev0/theseus/optimizer/linear_system.py` & `theseus-ai-0.2.1/theseus/optimizer/linear_system.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-0.2.0.dev0/theseus/optimizer/linearization.py` & `theseus-ai-0.2.1/theseus/optimizer/linearization.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-0.2.0.dev0/theseus/optimizer/manifold_gaussian.py` & `theseus-ai-0.2.1/theseus/optimizer/manifold_gaussian.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-0.2.0.dev0/theseus/optimizer/nonlinear/__init__.py` & `theseus-ai-0.2.1/theseus/optimizer/nonlinear/__init__.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-0.2.0.dev0/theseus/optimizer/nonlinear/dcem.py` & `theseus-ai-0.2.1/theseus/optimizer/nonlinear/dcem.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
-from typing import Optional, Union, List, Dict
+from typing import Dict, List, Optional, Union
 
 import numpy as np
 import torch
 from torch.distributions import Normal
 
-from theseus.third_party.lml import LML
 from theseus.core.objective import Objective
 from theseus.optimizer import OptimizerInfo
 from theseus.optimizer.variable_ordering import VariableOrdering
+from theseus.third_party.lml import LML
 
 from .nonlinear_optimizer import (
-    NonlinearOptimizer,
     BackwardMode,
+    EndIterCallbackType,
+    NonlinearOptimizer,
     NonlinearOptimizerInfo,
     NonlinearOptimizerStatus,
-    EndIterCallbackType,
 )
 
 
 class DCEM(NonlinearOptimizer):
     """
     DCEM optimizer for nonlinear optimization using sampling based techniques.
     The optimizer can be really sensitive to hypermeter tuning. Here are few tuning
```

### Comparing `theseus-ai-0.2.0.dev0/theseus/optimizer/nonlinear/dogleg.py` & `theseus-ai-0.2.1/theseus/optimizer/nonlinear/dogleg.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-0.2.0.dev0/theseus/optimizer/nonlinear/gauss_newton.py` & `theseus-ai-0.2.1/theseus/optimizer/nonlinear/gauss_newton.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-0.2.0.dev0/theseus/optimizer/nonlinear/levenberg_marquardt.py` & `theseus-ai-0.2.1/theseus/optimizer/nonlinear/levenberg_marquardt.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-0.2.0.dev0/theseus/optimizer/nonlinear/nonlinear_least_squares.py` & `theseus-ai-0.2.1/theseus/optimizer/nonlinear/nonlinear_least_squares.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,24 +9,25 @@
 
 import torch
 
 from theseus.core import Objective
 from theseus.core.objective import error_squared_norm_fn
 from theseus.optimizer import Linearization, OptimizerInfo
 from theseus.optimizer.linear import (
-    LinearSolver,
     CholeskyDenseSolver,
+    LinearSolver,
     LUCudaSparseSolver,
 )
+
 from .nonlinear_optimizer import (
     BackwardMode,
+    EndIterCallbackType,
     NonlinearOptimizer,
     NonlinearOptimizerInfo,
     NonlinearOptimizerStatus,
-    EndIterCallbackType,
 )
 
 
 # Base class for all optimizers for NLLS problems,
 # providing the skeleton of the
 # optimization loop. Subclasses need to implement the following method:
 #
@@ -119,18 +120,23 @@
             try:
                 if _last_implicit_diff_step:
                     # The derivation for implicit differentiation states that
                     # the autograd-enabled loop must be done using Gauss-Newton steps.
                     # Well, technically full Newton, this is hard to implement and GN
                     # is working well so far.
                     #
-                    # We also need to detach the hessian when computing
+                    # As shown above, we also need to detach the hessian when computing
                     # linearization above, as higher order terms introduce errors
                     # in the derivative if the fixed point is not accurate enough.
-                    delta = self.linear_solver.solve()
+                    try:
+                        delta = self.linear_solver.solve()
+                    except RuntimeError as e:  # fallback to regular step if GN fails
+                        if kwargs.get("__strict_implicit_final_gn__", False):
+                            raise e
+                        delta = self.compute_delta(**kwargs)
                 else:
                     delta = self.compute_delta(**kwargs)
             except RuntimeError as run_err:
                 msg = (
                     f"There was an error while running the linear optimizer. "
                     f"Original error message: {run_err}."
                 )
```

### Comparing `theseus-ai-0.2.0.dev0/theseus/optimizer/nonlinear/nonlinear_optimizer.py` & `theseus-ai-0.2.1/theseus/optimizer/nonlinear/nonlinear_optimizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # LICENSE file in the root directory of this source tree.
 
 import abc
 import math
 import warnings
 from dataclasses import dataclass
 from enum import Enum
-from typing import Dict, Optional, Tuple, Union, Callable, NoReturn
+from typing import Callable, Dict, NoReturn, Optional, Tuple, Union
 
 import numpy as np
 import torch
 
 from theseus.core import Objective
 from theseus.optimizer import Optimizer, OptimizerInfo
```

### Comparing `theseus-ai-0.2.0.dev0/theseus/optimizer/nonlinear/trust_region.py` & `theseus-ai-0.2.1/theseus/optimizer/nonlinear/trust_region.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 
 from theseus.core import Objective
 from theseus.optimizer import Linearization
 from theseus.optimizer.linear import LinearSolver
 
 from .nonlinear_least_squares import NonlinearLeastSquares
 
-
 # See Nocedal and Wright, Numerical Optimization, Chapter 4
 # https://www.csie.ntu.edu.tw/~r97002/temp/num_optimization.pdf
 
 
 # This optimizer optimize() receives the following keywords (see p. 69):
 #       - trust_region_init (default 1.0)
 #       - accept_threshold (default 0.25)
```

### Comparing `theseus-ai-0.2.0.dev0/theseus/optimizer/optimizer.py` & `theseus-ai-0.2.1/theseus/optimizer/optimizer.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-0.2.0.dev0/theseus/optimizer/sparse_linearization.py` & `theseus-ai-0.2.1/theseus/optimizer/sparse_linearization.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from typing import List, Optional
 
 import numpy as np
 import torch
 
 from theseus.core import Objective
-from theseus.utils.sparse_matrix_utils import sparse_mv, sparse_mtv
+from theseus.utils.sparse_matrix_utils import sparse_mtv, sparse_mv
 
 from .linear_system import SparseStructure
 from .linearization import Linearization
 from .variable_ordering import VariableOrdering
 
 
 class SparseLinearization(Linearization):
```

### Comparing `theseus-ai-0.2.0.dev0/theseus/optimizer/variable_ordering.py` & `theseus-ai-0.2.1/theseus/optimizer/variable_ordering.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-0.2.0.dev0/theseus/theseus_layer.py` & `theseus-ai-0.2.1/theseus/theseus_layer.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from typing import Any, Dict, List, Optional, Tuple
 
 import numpy as np
 import torch
 import torch.nn as nn
 from torch.autograd.function import once_differentiable
 
+from theseus.constants import __FROM_THESEUS_LAYER_TOKEN__, DeviceType
 from theseus.core import (
     CostFunction,
     CostWeight,
     Objective,
     ScaleCostWeight,
     Variable,
     Vectorize,
 )
-from theseus.constants import __FROM_THESEUS_LAYER_TOKEN__, DeviceType
 from theseus.geometry import LieGroup, Manifold
 from theseus.optimizer import Optimizer, OptimizerInfo
 from theseus.optimizer.linear import LinearSolver
 from theseus.optimizer.nonlinear import BackwardMode, GaussNewton
 from theseus.utils import check_jacobians
```

### Comparing `theseus-ai-0.2.0.dev0/theseus/third_party/easyaug.py` & `theseus-ai-0.2.1/theseus/third_party/easyaug.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-0.2.0.dev0/theseus/third_party/lml.py` & `theseus-ai-0.2.1/theseus/third_party/lml.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,26 +16,23 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
 # EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
 # MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
 # NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE
 # LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
 # OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION
 # WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-
+import numpy as np
+import numpy.random as npr
 import torch
 from torch.autograd import Function, Variable, grad
 from torch.nn import Module
 
-import numpy as np
-import numpy.random as npr
-
-from semantic_version import Version
+from theseus._version import lt_version
 
-version = Version(".".join(torch.__version__.split(".")[:3]))
-old_torch = version < Version("0.4.0")
+old_torch = lt_version(torch.__version__, "0.4.0")
 
 
 def bdot(x, y):
     return torch.bmm(x.unsqueeze(1), y.unsqueeze(2)).squeeze()
 
 
 class LML(Module):
@@ -178,14 +175,15 @@
 
         grads = tuple([dx] + [None] * 5)
         return grads
 
 
 if __name__ == "__main__":
     import sys
+
     from IPython.core import ultratb
 
     sys.excepthook = ultratb.FormattedTB(
         mode="Verbose", color_scheme="Linux", call_pdb=1
     )
 
     m = 10
```

### Comparing `theseus-ai-0.2.0.dev0/theseus/third_party/utils.py` & `theseus-ai-0.2.1/theseus/third_party/utils.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-0.2.0.dev0/theseus/utils/examples/__init__.py` & `theseus-ai-0.2.1/theseus/utils/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-0.2.0.dev0/theseus/utils/examples/bundle_adjustment/data.py` & `theseus-ai-0.2.1/theseus/utils/examples/bundle_adjustment/data.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-0.2.0.dev0/theseus/utils/examples/bundle_adjustment/util.py` & `theseus-ai-0.2.1/theseus/utils/examples/bundle_adjustment/util.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-0.2.0.dev0/theseus/utils/examples/motion_planning/misc.py` & `theseus-ai-0.2.1/theseus/utils/examples/motion_planning/misc.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-0.2.0.dev0/theseus/utils/examples/motion_planning/models.py` & `theseus-ai-0.2.1/theseus/utils/examples/motion_planning/models.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-0.2.0.dev0/theseus/utils/examples/motion_planning/motion_planner.py` & `theseus-ai-0.2.1/theseus/utils/examples/motion_planning/motion_planner.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-0.2.0.dev0/theseus/utils/examples/pose_graph/dataset.py` & `theseus-ai-0.2.1/theseus/utils/examples/pose_graph/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -233,16 +233,16 @@
             barlen = round(bi * 80 / max_buckets)
             hist_str += f"{label}: {'#' * barlen} {bi}\n"
         return hist_str
 
     @staticmethod
     def generate_synthetic_3D(
         num_poses: int,
-        rotation_noise: float = 0.05,
-        translation_noise: float = 0.1,
+        translation_noise: float = 0.05,
+        rotation_noise: float = 0.1,
         loop_closure_ratio: float = 0.2,
         loop_closure_outlier_ratio: float = 0.05,
         max_num_loop_closures: int = 10,
         dataset_size: int = 1,
         batch_size: int = 1,
         generator: Optional[torch.Generator] = None,
         dtype: Optional[torch.dtype] = None,
@@ -278,18 +278,18 @@
                     ],
                     dim=1,
                 )
             )
             noise_relative_pose = th.SE3.exp_map(
                 torch.cat(
                     [
-                        rotation_noise
-                        * (2 * torch.rand(dataset_size, 3, dtype=dtype) - 1),
                         translation_noise
                         * (2.0 * torch.rand(dataset_size, 3, dtype=dtype) - 1),
+                        rotation_noise
+                        * (2.0 * torch.rand(dataset_size, 3, dtype=dtype) - 1),
                     ],
                     dim=1,
                 )
             )
             relative_pose = cast(th.SE3, gt_relative_pose.compose(noise_relative_pose))
             relative_pose.name = "EDGE_SE3__{}_{}".format(n - 1, n)
             weight = th.DiagonalCostWeight(
@@ -318,18 +318,18 @@
                     gt_relative_pose = cast(
                         th.SE3, gt_poses[i].inverse().compose(gt_poses[j])
                     )
                     if np.random.rand(1) > loop_closure_outlier_ratio:
                         noise_relative_pose = th.SE3.exp_map(
                             torch.cat(
                                 [
-                                    rotation_noise
-                                    * (2 * torch.rand(1, 3, dtype=dtype) - 1),
                                     translation_noise
                                     * (2.0 * torch.rand(1, 3, dtype=dtype) - 1),
+                                    rotation_noise
+                                    * (2.0 * torch.rand(1, 3, dtype=dtype) - 1),
                                 ],
                                 dim=1,
                             )
                         )
                         inliers.append(True)
                     else:
                         noise_relative_pose = th.SE3.rand(
@@ -350,31 +350,31 @@
                         PoseGraphEdge(i, j, relative_pose=relative_pose, weight=weight)
                     )
 
         for i in range(len(poses)):
             noise_pose = th.SE3.exp_map(
                 torch.cat(
                     [
-                        rotation_noise * (2 * torch.rand(1, 3, dtype=dtype) - 1),
                         translation_noise * (2.0 * torch.rand(1, 3, dtype=dtype) - 1),
+                        rotation_noise * (2.0 * torch.rand(1, 3, dtype=dtype) - 1),
                     ],
                     dim=1,
                 )
             )
             poses[i].tensor = gt_poses[i].compose(noise_pose).tensor
 
         return PoseGraphDataset(poses, edges, gt_poses, batch_size=batch_size), inliers
 
     def write_3D_g2o(self, filename: str):
         for n in range(self.dataset_size):
             with open(filename + f"_{n}.g2o", "w") as file:
                 for edge in self.edges:
                     measurement = edge.relative_pose.tensor[n : n + 1]
                     quat = th.SO3(
-                        tensor=measurement[:, :, :3], strict=False
+                        tensor=measurement[:, :, :3], strict_checks=False
                     ).to_quaternion()
                     tran = measurement[:, :, 3]
                     measurement = torch.cat([tran, quat], dim=1).view(-1).numpy()
                     weight = edge.weight.diagonal.tensor**2
                     line = (
                         f"EDGE_SE3:QUAT {edge.i} {edge.j} {measurement[0]} {measurement[1]} "
                         f"{measurement[2]} "
@@ -382,15 +382,17 @@
                         f"{measurement[6]} {measurement[3]} "
                         f"{weight[0,0]} 0 0 0 0 0 {weight[0,1]} 0 0 0 0 {weight[0,2]} 0 0 0 "
                         f"{weight[0,3]} 0 0 {weight[0,4]} 0 {weight[0,5]}\n"
                     )
                     file.write(line)
                 for i, pose in enumerate(self.poses):
                     pose_n = pose[n : n + 1]
-                    quat = th.SO3(tensor=pose_n[:, :, :3], strict=False).to_quaternion()
+                    quat = th.SO3(
+                        tensor=pose_n[:, :, :3], strict_checks=False
+                    ).to_quaternion()
                     tran = pose_n[:, :, 3]
                     pose_data = torch.cat([tran, quat], dim=1).view(-1).numpy()
                     line = (
                         f"VERTEX_SE3:QUAT {i} {pose_data[0]} {pose_data[1]} {pose_data[2]} "
                         f"{pose_data[4]} {pose_data[5]} {pose_data[6]} {pose_data[3]}\n"
                     )
                     file.write(line)
```

### Comparing `theseus-ai-0.2.0.dev0/theseus/utils/examples/tactile_pose_estimation/misc.py` & `theseus-ai-0.2.1/theseus/utils/examples/tactile_pose_estimation/misc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# Copyright (c) Meta Platforms, Inc. and affiliates.
+#
+# This source code is licensed under the MIT license found in the
+# LICENSE file in the root directory of this source tree.
 from typing import Dict, List, Optional, Tuple
 
 import matplotlib.patches as mpatches
 import matplotlib.pyplot as plt
 import numpy as np
 import torch
```

### Comparing `theseus-ai-0.2.0.dev0/theseus/utils/examples/tactile_pose_estimation/models.py` & `theseus-ai-0.2.1/theseus/utils/examples/tactile_pose_estimation/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# Copyright (c) Meta Platforms, Inc. and affiliates.
+#
+# This source code is licensed under the MIT license found in the
+# LICENSE file in the root directory of this source tree.
 import collections
 import pathlib
 from typing import Dict, List, Optional, Tuple, cast
 
 import numpy as np
 import omegaconf
 import torch
```

### Comparing `theseus-ai-0.2.0.dev0/theseus/utils/examples/tactile_pose_estimation/pose_estimator.py` & `theseus-ai-0.2.1/theseus/utils/examples/tactile_pose_estimation/pose_estimator.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# Copyright (c) Meta Platforms, Inc. and affiliates.
+#
+# This source code is licensed under the MIT license found in the
+# LICENSE file in the root directory of this source tree.
 from typing import Dict, List, Optional, Tuple, Type
 
 import numpy as np
 import torch
 
 import theseus as th
 from theseus.optimizer.nonlinear.levenberg_marquardt import LevenbergMarquardt
```

### Comparing `theseus-ai-0.2.0.dev0/theseus/utils/examples/tactile_pose_estimation/trainer.py` & `theseus-ai-0.2.1/theseus/utils/examples/tactile_pose_estimation/trainer.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-0.2.0.dev0/theseus/utils/sparse_matrix_utils.py` & `theseus-ai-0.2.1/theseus/utils/sparse_matrix_utils.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-0.2.0.dev0/theseus/utils/utils.py` & `theseus-ai-0.2.1/theseus/utils/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
+import cProfile
+import io
+import pstats
 import time
 from typing import Any, Callable, List, Optional, Type
 
 import numpy as np
 import torch
 import torch.nn as nn
 
@@ -214,7 +217,30 @@
     def __exit__(self, exc_type: Any, exc_value: Any, traceback: Any) -> None:
         if self.device.type == "cuda":
             self._end_event.record()
             torch.cuda.synchronize()
             self.elapsed_time = self._start_event.elapsed_time(self._end_event) / 1e3
         else:
             self.elapsed_time = (time.perf_counter_ns() - self._start_time) / 1e9
+
+
+# Wrapper for cProfile.Profile for easily make optional, turn on/off and printing
+class Profiler:
+    def __init__(self, active: bool):
+        self.c_profiler = cProfile.Profile()
+        self.active = active
+
+    def enable(self):
+        if self.active:
+            self.c_profiler.enable()
+
+    def disable(self):
+        if self.active:
+            self.c_profiler.disable()
+
+    def print(self):
+        if self.active:
+            s = io.StringIO()
+            sortby = pstats.SortKey.CUMULATIVE
+            ps = pstats.Stats(self.c_profiler, stream=s).sort_stats(sortby)
+            ps.print_stats()
+            print(s.getvalue())
```

### Comparing `theseus-ai-0.2.0.dev0/theseus_ai.egg-info/PKG-INFO` & `theseus-ai-0.2.1/theseus_ai.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: theseus-ai
-Version: 0.2.0.dev0
+Version: 0.2.1
 Summary: A library for differentiable nonlinear optimization.
 Home-page: https://github.com/facebookresearch/theseus
 Author: Meta Research
 Keywords: differentiable optimization,nonlinear least squares,factor graphs
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Science/Research
@@ -72,20 +72,22 @@
 -----
 
 ## Current Features
 
 ### Application agnostic interface
 Our implementation provides an easy to use interface to build custom optimization layers and plug them into any neural architecture. Following differentiable features are currently available:
 - [Second-order nonlinear optimizers](https://github.com/facebookresearch/theseus/tree/main/theseus/optimizer/nonlinear)
-    - Gauss-Newton, Levenberg–Marquardt
+    - Gauss-Newton (GN), Levenberg–Marquardt (LM), Trust Region, Dogleg
+- [Other nonlinear optimizers](https://github.com/facebookresearch/theseus/tree/main/theseus/optimizer/nonlinear)
+    - Cross Entropy Method (CEM)
 - [Linear solvers](https://github.com/facebookresearch/theseus/tree/main/theseus/optimizer/linear)
     - Dense: Cholesky, LU; Sparse: CHOLMOD, LU (GPU-only), [BaSpaCho](https://github.com/facebookresearch/baspacho)
 - [Commonly used costs](https://github.com/facebookresearch/theseus/tree/main/theseus/embodied), [AutoDiffCostFunction](https://github.com/facebookresearch/theseus/blob/main/theseus/core/cost_function.py), [RobustCostFunction](https://github.com/facebookresearch/theseus/blob/main/theseus/core/robust_cost_function.py)
-- [Lie groups](https://github.com/facebookresearch/theseus/tree/main/theseus/geometry)
-- [Robot kinematics](https://github.com/facebookresearch/theseus/blob/main/theseus/embodied/kinematics/kinematics_model.py)
+- [Lie groups](https://github.com/facebookresearch/theseus/tree/main/theseus/geometry) based on [torchlie](https://github.com/facebookresearch/theseus/tree/main/torchlie)
+- [Robot kinematics](https://github.com/facebookresearch/theseus/blob/main/theseus/embodied/kinematics) based on [torchkin](https://github.com/facebookresearch/theseus/tree/main/torchkin)
 
 ### Efficiency based design
 We support several features that improve computation times and memory consumption:
 - [Sparse linear solvers](https://github.com/facebookresearch/theseus/tree/main/theseus/optimizer/linear)
 - Batching and GPU acceleration
 - [Automatic vectorization](https://github.com/facebookresearch/theseus/blob/main/theseus/core/vectorizer.py)
 - [Backward modes](https://github.com/facebookresearch/theseus/blob/main/theseus/optimizer/nonlinear/nonlinear_optimizer.py)
@@ -120,14 +122,15 @@
     ```bash
     git clone https://github.com/facebookresearch/theseus.git && cd theseus
     pip install -e .
     ```
     If you are interested in contributing to Theseus, instead install
     ```bash
     pip install -e ".[dev]"
+    pre-commit install
     ```
     and follow the more detailed instructions in [CONTRIBUTING](https://github.com/facebookresearch/theseus/blob/main/CONTRIBUTING.md).
 
 - **Installing BaSpaCho extensions from source**
 
     By default, installing from source doesn't include our BaSpaCho sparse solver extension. For this, follow these steps:
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: theseus-ai Version: 0.2.0.dev0 Summary: A library
-for differentiable nonlinear optimization. Home-page: https://github.com/
+Metadata-Version: 2.1 Name: theseus-ai Version: 0.2.1 Summary: A library for
+differentiable nonlinear optimization. Home-page: https://github.com/
 facebookresearch/theseus Author: Meta Research Keywords: differentiable
 optimization,nonlinear least squares,factor graphs Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Science/Research Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Requires-Python: >=3.8
 Description-Content-Type: text/markdown Provides-Extra: dev License-File:
 LICENSE ![](https://raw.githubusercontent.com/facebookresearch/theseus/main/
@@ -23,28 +23,32 @@
 by differentiating through the optimizer which allows neural models to train on
 the final task loss, while also taking advantage of priors captured by the
 optimizer. ----- ## Current Features ### Application agnostic interface Our
 implementation provides an easy to use interface to build custom optimization
 layers and plug them into any neural architecture. Following differentiable
 features are currently available: - [Second-order nonlinear optimizers](https:/
 /github.com/facebookresearch/theseus/tree/main/theseus/optimizer/nonlinear) -
-Gauss-Newton, LevenbergâMarquardt - [Linear solvers](https://github.com/
-facebookresearch/theseus/tree/main/theseus/optimizer/linear) - Dense: Cholesky,
-LU; Sparse: CHOLMOD, LU (GPU-only), [BaSpaCho](https://github.com/
-facebookresearch/baspacho) - [Commonly used costs](https://github.com/
-facebookresearch/theseus/tree/main/theseus/embodied), [AutoDiffCostFunction]
-(https://github.com/facebookresearch/theseus/blob/main/theseus/core/
-cost_function.py), [RobustCostFunction](https://github.com/facebookresearch/
-theseus/blob/main/theseus/core/robust_cost_function.py) - [Lie groups](https://
-github.com/facebookresearch/theseus/tree/main/theseus/geometry) - [Robot
-kinematics](https://github.com/facebookresearch/theseus/blob/main/theseus/
-embodied/kinematics/kinematics_model.py) ### Efficiency based design We support
-several features that improve computation times and memory consumption: -
-[Sparse linear solvers](https://github.com/facebookresearch/theseus/tree/main/
-theseus/optimizer/linear) - Batching and GPU acceleration - [Automatic
+Gauss-Newton (GN), LevenbergâMarquardt (LM), Trust Region, Dogleg - [Other
+nonlinear optimizers](https://github.com/facebookresearch/theseus/tree/main/
+theseus/optimizer/nonlinear) - Cross Entropy Method (CEM) - [Linear solvers]
+(https://github.com/facebookresearch/theseus/tree/main/theseus/optimizer/
+linear) - Dense: Cholesky, LU; Sparse: CHOLMOD, LU (GPU-only), [BaSpaCho]
+(https://github.com/facebookresearch/baspacho) - [Commonly used costs](https://
+github.com/facebookresearch/theseus/tree/main/theseus/embodied),
+[AutoDiffCostFunction](https://github.com/facebookresearch/theseus/blob/main/
+theseus/core/cost_function.py), [RobustCostFunction](https://github.com/
+facebookresearch/theseus/blob/main/theseus/core/robust_cost_function.py) - [Lie
+groups](https://github.com/facebookresearch/theseus/tree/main/theseus/geometry)
+based on [torchlie](https://github.com/facebookresearch/theseus/tree/main/
+torchlie) - [Robot kinematics](https://github.com/facebookresearch/theseus/
+blob/main/theseus/embodied/kinematics) based on [torchkin](https://github.com/
+facebookresearch/theseus/tree/main/torchkin) ### Efficiency based design We
+support several features that improve computation times and memory consumption:
+- [Sparse linear solvers](https://github.com/facebookresearch/theseus/tree/
+main/theseus/optimizer/linear) - Batching and GPU acceleration - [Automatic
 vectorization](https://github.com/facebookresearch/theseus/blob/main/theseus/
 core/vectorizer.py) - [Backward modes](https://github.com/facebookresearch/
 theseus/blob/main/theseus/optimizer/nonlinear/nonlinear_optimizer.py) -
 Implicit, Truncated, Direct Loss Minimization ([DLM](https://github.com/
 facebookresearch/theseus/blob/main/theseus/theseus_layer.py)), Sampling ([LEO]
 (https://github.com/facebookresearch/theseus/blob/main/examples/
 state_estimation_2d.py)) ## Getting Started ### Prerequisites - We *strongly*
@@ -65,23 +69,23 @@
 theseus/blob/main/build_scripts/build_wheel.sh). Note that `pypi` installation
 doesn't include our experimental [Theseus Labs](https://github.com/
 facebookresearch/theseus/tree/main/theseus/labs). For this, please install from
 source. - #### **From source** The simplest way to install Theseus from source
 is by running the following (see further below to also include BaSpaCho)
 ```bash git clone https://github.com/facebookresearch/theseus.git && cd theseus
 pip install -e . ``` If you are interested in contributing to Theseus, instead
-install ```bash pip install -e ".[dev]" ``` and follow the more detailed
-instructions in [CONTRIBUTING](https://github.com/facebookresearch/theseus/
-blob/main/CONTRIBUTING.md). - **Installing BaSpaCho extensions from source** By
-default, installing from source doesn't include our BaSpaCho sparse solver
-extension. For this, follow these steps: 1. Compile BaSpaCho from source
-following instructions [here](https://github.com/facebookresearch/baspacho). We
-recommend using flags `-DBLA_STATIC=ON -DBUILD_SHARED_LIBS=OFF`. 2. Run ```bash
-git clone https://github.com/facebookresearch/theseus.git && cd theseus
-BASPACHO_ROOT_DIR=
+install ```bash pip install -e ".[dev]" pre-commit install ``` and follow the
+more detailed instructions in [CONTRIBUTING](https://github.com/
+facebookresearch/theseus/blob/main/CONTRIBUTING.md). - **Installing BaSpaCho
+extensions from source** By default, installing from source doesn't include our
+BaSpaCho sparse solver extension. For this, follow these steps: 1. Compile
+BaSpaCho from source following instructions [here](https://github.com/
+facebookresearch/baspacho). We recommend using flags `-DBLA_STATIC=ON -
+DBUILD_SHARED_LIBS=OFF`. 2. Run ```bash git clone https://github.com/
+facebookresearch/theseus.git && cd theseus BASPACHO_ROOT_DIR=
 o/root/baspacho/dir> pip install -e . ``` where the BaSpaCho root dir must have
 the binaries in the subdirectory `build`. ### Running unit tests (requires
 `dev` installation) ```bash python -m pytest tests ``` By default, unit tests
 include tests for our CUDA extensions. You can add the option `-m "not
 cudaext"` to skip them when installing without CUDA support. Additionally, the
 tests for sparse solver BaSpaCho are automatically skipped when its extlib is
 not compiled. ## Examples [Simple example](https://github.com/facebookresearch/
```

### Comparing `theseus-ai-0.2.0.dev0/theseus_ai.egg-info/SOURCES.txt` & `theseus-ai-0.2.1/theseus_ai.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
+/theseus/theseus/extlib/cusolver_lu_solver.cpp
+/theseus/theseus/extlib/cusolver_sp_defs.cpp
+/theseus/theseus/extlib/mat_mult.cu
 requirements/dev.txt
 requirements/docs.txt
 requirements/main.txt
 theseus/__init__.py
 theseus/_version.py
 theseus/constants.py
-theseus/options.py
+theseus/global_params.py
 theseus/theseus_layer.py
 theseus/core/__init__.py
 theseus/core/cost_function.py
 theseus/core/cost_weight.py
 theseus/core/objective.py
 theseus/core/robust_cost_function.py
 theseus/core/robust_loss.py
@@ -53,20 +56,14 @@
 theseus/geometry/point_types.py
 theseus/geometry/se2.py
 theseus/geometry/se3.py
 theseus/geometry/so2.py
 theseus/geometry/so3.py
 theseus/geometry/utils.py
 theseus/geometry/vector.py
-theseus/labs/__init__.py
-theseus/labs/embodied/__init__.py
-theseus/labs/embodied/robot/__init__.py
-theseus/labs/embodied/robot/forward_kinematics.py
-theseus/labs/embodied/robot/joint.py
-theseus/labs/embodied/robot/robot.py
 theseus/optimizer/__init__.py
 theseus/optimizer/dense_linearization.py
 theseus/optimizer/linear_system.py
 theseus/optimizer/linearization.py
 theseus/optimizer/manifold_gaussian.py
 theseus/optimizer/optimizer.py
 theseus/optimizer/sparse_linearization.py
```

