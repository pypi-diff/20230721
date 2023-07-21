# Comparing `tmp/nvidia-dali-tf-plugin-nightly-cuda110-1.29.0.dev20230719.tar.gz` & `tmp/nvidia-dali-tf-plugin-nightly-cuda110-1.29.0.dev20230720.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nvidia-dali-tf-plugin-nightly-cuda110-1.29.0.dev20230719.tar", last modified: Thu Jul 20 07:43:35 2023, max compression
+gzip compressed data, was "nvidia-dali-tf-plugin-nightly-cuda110-1.29.0.dev20230720.tar", last modified: Thu Jul 20 20:03:40 2023, max compression
```

## Comparing `nvidia-dali-tf-plugin-nightly-cuda110-1.29.0.dev20230719.tar` & `nvidia-dali-tf-plugin-nightly-cuda110-1.29.0.dev20230720.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-07-20 07:43:35.721082 nvidia-dali-tf-plugin-nightly-cuda110-1.29.0.dev20230719/
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      469 2023-07-20 07:43:35.000000 nvidia-dali-tf-plugin-nightly-cuda110-1.29.0.dev20230719/ERROR.txt
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)    11336 2023-07-06 05:01:19.000000 nvidia-dali-tf-plugin-nightly-cuda110-1.29.0.dev20230719/LICENSE.md
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       37 2023-07-20 07:43:35.000000 nvidia-dali-tf-plugin-nightly-cuda110-1.29.0.dev20230719/PACKAGE_NAME
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1708 2023-07-20 07:43:35.721082 nvidia-dali-tf-plugin-nightly-cuda110-1.29.0.dev20230719/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      316 2023-07-20 07:43:35.000000 nvidia-dali-tf-plugin-nightly-cuda110-1.29.0.dev20230719/README.rst
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-07-20 07:43:35.721082 nvidia-dali-tf-plugin-nightly-cuda110-1.29.0.dev20230719/nvidia_dali_tf_plugin_nightly_cuda110.egg-info/
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1708 2023-07-20 07:43:35.000000 nvidia-dali-tf-plugin-nightly-cuda110-1.29.0.dev20230719/nvidia_dali_tf_plugin_nightly_cuda110.egg-info/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      297 2023-07-20 07:43:35.000000 nvidia-dali-tf-plugin-nightly-cuda110-1.29.0.dev20230719/nvidia_dali_tf_plugin_nightly_cuda110.egg-info/SOURCES.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-07-20 07:43:35.000000 nvidia-dali-tf-plugin-nightly-cuda110-1.29.0.dev20230719/nvidia_dali_tf_plugin_nightly_cuda110.egg-info/dependency_links.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       22 2023-07-20 07:43:35.000000 nvidia-dali-tf-plugin-nightly-cuda110-1.29.0.dev20230719/nvidia_dali_tf_plugin_nightly_cuda110.egg-info/top_level.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       38 2023-07-20 07:43:35.721082 nvidia-dali-tf-plugin-nightly-cuda110-1.29.0.dev20230719/setup.cfg
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     4560 2023-07-06 05:01:19.000000 nvidia-dali-tf-plugin-nightly-cuda110-1.29.0.dev20230719/setup.py
+drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-07-20 20:03:40.329404 nvidia-dali-tf-plugin-nightly-cuda110-1.29.0.dev20230720/
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      469 2023-07-20 20:03:40.000000 nvidia-dali-tf-plugin-nightly-cuda110-1.29.0.dev20230720/ERROR.txt
+-rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)    11336 2023-07-06 05:01:19.000000 nvidia-dali-tf-plugin-nightly-cuda110-1.29.0.dev20230720/LICENSE.md
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       37 2023-07-20 20:03:40.000000 nvidia-dali-tf-plugin-nightly-cuda110-1.29.0.dev20230720/PACKAGE_NAME
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1708 2023-07-20 20:03:40.329404 nvidia-dali-tf-plugin-nightly-cuda110-1.29.0.dev20230720/PKG-INFO
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      316 2023-07-20 20:03:40.000000 nvidia-dali-tf-plugin-nightly-cuda110-1.29.0.dev20230720/README.rst
+drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-07-20 20:03:40.329404 nvidia-dali-tf-plugin-nightly-cuda110-1.29.0.dev20230720/nvidia_dali_tf_plugin_nightly_cuda110.egg-info/
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1708 2023-07-20 20:03:40.000000 nvidia-dali-tf-plugin-nightly-cuda110-1.29.0.dev20230720/nvidia_dali_tf_plugin_nightly_cuda110.egg-info/PKG-INFO
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      297 2023-07-20 20:03:40.000000 nvidia-dali-tf-plugin-nightly-cuda110-1.29.0.dev20230720/nvidia_dali_tf_plugin_nightly_cuda110.egg-info/SOURCES.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-07-20 20:03:40.000000 nvidia-dali-tf-plugin-nightly-cuda110-1.29.0.dev20230720/nvidia_dali_tf_plugin_nightly_cuda110.egg-info/dependency_links.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       22 2023-07-20 20:03:40.000000 nvidia-dali-tf-plugin-nightly-cuda110-1.29.0.dev20230720/nvidia_dali_tf_plugin_nightly_cuda110.egg-info/top_level.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       38 2023-07-20 20:03:40.329404 nvidia-dali-tf-plugin-nightly-cuda110-1.29.0.dev20230720/setup.cfg
+-rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     4560 2023-07-06 05:01:19.000000 nvidia-dali-tf-plugin-nightly-cuda110-1.29.0.dev20230720/setup.py
```

### Comparing `nvidia-dali-tf-plugin-nightly-cuda110-1.29.0.dev20230719/LICENSE.md` & `nvidia-dali-tf-plugin-nightly-cuda110-1.29.0.dev20230720/LICENSE.md`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-nightly-cuda110-1.29.0.dev20230719/PKG-INFO` & `nvidia-dali-tf-plugin-nightly-cuda110-1.29.0.dev20230720/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nvidia-dali-tf-plugin-nightly-cuda110
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

### Comparing `nvidia-dali-tf-plugin-nightly-cuda110-1.29.0.dev20230719/nvidia_dali_tf_plugin_nightly_cuda110.egg-info/PKG-INFO` & `nvidia-dali-tf-plugin-nightly-cuda110-1.29.0.dev20230720/nvidia_dali_tf_plugin_nightly_cuda110.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nvidia-dali-tf-plugin-nightly-cuda110
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

### Comparing `nvidia-dali-tf-plugin-nightly-cuda110-1.29.0.dev20230719/setup.py` & `nvidia-dali-tf-plugin-nightly-cuda110-1.29.0.dev20230720/setup.py`

 * *Files identical despite different names*

