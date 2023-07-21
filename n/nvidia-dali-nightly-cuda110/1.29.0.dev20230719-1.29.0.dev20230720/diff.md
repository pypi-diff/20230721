# Comparing `tmp/nvidia-dali-nightly-cuda110-1.29.0.dev20230719.tar.gz` & `tmp/nvidia-dali-nightly-cuda110-1.29.0.dev20230720.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nvidia-dali-nightly-cuda110-1.29.0.dev20230719.tar", last modified: Thu Jul 20 07:44:52 2023, max compression
+gzip compressed data, was "nvidia-dali-nightly-cuda110-1.29.0.dev20230720.tar", last modified: Thu Jul 20 20:06:23 2023, max compression
```

## Comparing `nvidia-dali-nightly-cuda110-1.29.0.dev20230719.tar` & `nvidia-dali-nightly-cuda110-1.29.0.dev20230720.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-07-20 07:44:52.072308 nvidia-dali-nightly-cuda110-1.29.0.dev20230719/
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      459 2023-07-20 07:44:52.000000 nvidia-dali-nightly-cuda110-1.29.0.dev20230719/ERROR.txt
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)    11336 2023-07-06 05:01:19.000000 nvidia-dali-nightly-cuda110-1.29.0.dev20230719/LICENSE.md
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       27 2023-07-20 07:44:52.000000 nvidia-dali-nightly-cuda110-1.29.0.dev20230719/PACKAGE_NAME
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1668 2023-07-20 07:44:52.072308 nvidia-dali-nightly-cuda110-1.29.0.dev20230719/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      286 2023-07-20 07:44:52.000000 nvidia-dali-nightly-cuda110-1.29.0.dev20230719/README.rst
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-07-20 07:44:52.068308 nvidia-dali-nightly-cuda110-1.29.0.dev20230719/nvidia_dali_nightly_cuda110.egg-info/
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1668 2023-07-20 07:44:52.000000 nvidia-dali-nightly-cuda110-1.29.0.dev20230719/nvidia_dali_nightly_cuda110.egg-info/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      257 2023-07-20 07:44:52.000000 nvidia-dali-nightly-cuda110-1.29.0.dev20230719/nvidia_dali_nightly_cuda110.egg-info/SOURCES.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-07-20 07:44:52.000000 nvidia-dali-nightly-cuda110-1.29.0.dev20230719/nvidia_dali_nightly_cuda110.egg-info/dependency_links.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       22 2023-07-20 07:44:52.000000 nvidia-dali-nightly-cuda110-1.29.0.dev20230719/nvidia_dali_nightly_cuda110.egg-info/top_level.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       38 2023-07-20 07:44:52.072308 nvidia-dali-nightly-cuda110-1.29.0.dev20230719/setup.cfg
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     4560 2023-07-06 05:01:19.000000 nvidia-dali-nightly-cuda110-1.29.0.dev20230719/setup.py
+drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-07-20 20:06:23.676023 nvidia-dali-nightly-cuda110-1.29.0.dev20230720/
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      459 2023-07-20 20:06:23.000000 nvidia-dali-nightly-cuda110-1.29.0.dev20230720/ERROR.txt
+-rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)    11336 2023-07-06 05:01:19.000000 nvidia-dali-nightly-cuda110-1.29.0.dev20230720/LICENSE.md
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       27 2023-07-20 20:06:23.000000 nvidia-dali-nightly-cuda110-1.29.0.dev20230720/PACKAGE_NAME
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1668 2023-07-20 20:06:23.676023 nvidia-dali-nightly-cuda110-1.29.0.dev20230720/PKG-INFO
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      286 2023-07-20 20:06:23.000000 nvidia-dali-nightly-cuda110-1.29.0.dev20230720/README.rst
+drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-07-20 20:06:23.676023 nvidia-dali-nightly-cuda110-1.29.0.dev20230720/nvidia_dali_nightly_cuda110.egg-info/
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1668 2023-07-20 20:06:23.000000 nvidia-dali-nightly-cuda110-1.29.0.dev20230720/nvidia_dali_nightly_cuda110.egg-info/PKG-INFO
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      257 2023-07-20 20:06:23.000000 nvidia-dali-nightly-cuda110-1.29.0.dev20230720/nvidia_dali_nightly_cuda110.egg-info/SOURCES.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-07-20 20:06:23.000000 nvidia-dali-nightly-cuda110-1.29.0.dev20230720/nvidia_dali_nightly_cuda110.egg-info/dependency_links.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       22 2023-07-20 20:06:23.000000 nvidia-dali-nightly-cuda110-1.29.0.dev20230720/nvidia_dali_nightly_cuda110.egg-info/top_level.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       38 2023-07-20 20:06:23.676023 nvidia-dali-nightly-cuda110-1.29.0.dev20230720/setup.cfg
+-rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     4560 2023-07-06 05:01:19.000000 nvidia-dali-nightly-cuda110-1.29.0.dev20230720/setup.py
```

### Comparing `nvidia-dali-nightly-cuda110-1.29.0.dev20230719/LICENSE.md` & `nvidia-dali-nightly-cuda110-1.29.0.dev20230720/LICENSE.md`

 * *Files identical despite different names*

### Comparing `nvidia-dali-nightly-cuda110-1.29.0.dev20230719/PKG-INFO` & `nvidia-dali-nightly-cuda110-1.29.0.dev20230720/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nvidia-dali-nightly-cuda110
-Version: 1.29.0.dev20230719
+Version: 1.29.0.dev20230720
 Summary: A fake package to warn the user they are not installing the correct package.
 Home-page: https://github.com/NVIDIA
 Download-URL: https://github.com/NVIDIA
 Author: Kitmaker
 Author-email: kitmaker@nvidia.com
 Maintainer: Kitmaker
 Maintainer-email: kitmaker@nvidia.com
```

### Comparing `nvidia-dali-nightly-cuda110-1.29.0.dev20230719/nvidia_dali_nightly_cuda110.egg-info/PKG-INFO` & `nvidia-dali-nightly-cuda110-1.29.0.dev20230720/nvidia_dali_nightly_cuda110.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nvidia-dali-nightly-cuda110
-Version: 1.29.0.dev20230719
+Version: 1.29.0.dev20230720
 Summary: A fake package to warn the user they are not installing the correct package.
 Home-page: https://github.com/NVIDIA
 Download-URL: https://github.com/NVIDIA
 Author: Kitmaker
 Author-email: kitmaker@nvidia.com
 Maintainer: Kitmaker
 Maintainer-email: kitmaker@nvidia.com
```

### Comparing `nvidia-dali-nightly-cuda110-1.29.0.dev20230719/setup.py` & `nvidia-dali-nightly-cuda110-1.29.0.dev20230720/setup.py`

 * *Files identical despite different names*

