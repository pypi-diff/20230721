# Comparing `tmp/nvidia-dali-tf-plugin-nightly-cuda120-1.29.0.dev20230720.tar.gz` & `tmp/nvidia-dali-tf-plugin-nightly-cuda120-1.29.0.dev20230721.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nvidia-dali-tf-plugin-nightly-cuda120-1.29.0.dev20230720.tar", last modified: Fri Jul 21 12:44:05 2023, max compression
+gzip compressed data, was "nvidia-dali-tf-plugin-nightly-cuda120-1.29.0.dev20230721.tar", last modified: Fri Jul 21 14:23:34 2023, max compression
```

## Comparing `nvidia-dali-tf-plugin-nightly-cuda120-1.29.0.dev20230720.tar` & `nvidia-dali-tf-plugin-nightly-cuda120-1.29.0.dev20230721.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-07-21 12:44:04.998797 nvidia-dali-tf-plugin-nightly-cuda120-1.29.0.dev20230720/
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      469 2023-07-21 12:44:04.000000 nvidia-dali-tf-plugin-nightly-cuda120-1.29.0.dev20230720/ERROR.txt
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)    11336 2023-07-06 05:01:19.000000 nvidia-dali-tf-plugin-nightly-cuda120-1.29.0.dev20230720/LICENSE.md
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       37 2023-07-21 12:44:04.000000 nvidia-dali-tf-plugin-nightly-cuda120-1.29.0.dev20230720/PACKAGE_NAME
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1708 2023-07-21 12:44:04.998797 nvidia-dali-tf-plugin-nightly-cuda120-1.29.0.dev20230720/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      316 2023-07-21 12:44:04.000000 nvidia-dali-tf-plugin-nightly-cuda120-1.29.0.dev20230720/README.rst
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-07-21 12:44:04.998797 nvidia-dali-tf-plugin-nightly-cuda120-1.29.0.dev20230720/nvidia_dali_tf_plugin_nightly_cuda120.egg-info/
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1708 2023-07-21 12:44:04.000000 nvidia-dali-tf-plugin-nightly-cuda120-1.29.0.dev20230720/nvidia_dali_tf_plugin_nightly_cuda120.egg-info/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      297 2023-07-21 12:44:04.000000 nvidia-dali-tf-plugin-nightly-cuda120-1.29.0.dev20230720/nvidia_dali_tf_plugin_nightly_cuda120.egg-info/SOURCES.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-07-21 12:44:04.000000 nvidia-dali-tf-plugin-nightly-cuda120-1.29.0.dev20230720/nvidia_dali_tf_plugin_nightly_cuda120.egg-info/dependency_links.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       22 2023-07-21 12:44:04.000000 nvidia-dali-tf-plugin-nightly-cuda120-1.29.0.dev20230720/nvidia_dali_tf_plugin_nightly_cuda120.egg-info/top_level.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       38 2023-07-21 12:44:04.998797 nvidia-dali-tf-plugin-nightly-cuda120-1.29.0.dev20230720/setup.cfg
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     4560 2023-07-06 05:01:19.000000 nvidia-dali-tf-plugin-nightly-cuda120-1.29.0.dev20230720/setup.py
+drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-07-21 14:23:34.313176 nvidia-dali-tf-plugin-nightly-cuda120-1.29.0.dev20230721/
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      469 2023-07-21 14:23:34.000000 nvidia-dali-tf-plugin-nightly-cuda120-1.29.0.dev20230721/ERROR.txt
+-rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)    11336 2023-07-06 05:01:19.000000 nvidia-dali-tf-plugin-nightly-cuda120-1.29.0.dev20230721/LICENSE.md
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       37 2023-07-21 14:23:34.000000 nvidia-dali-tf-plugin-nightly-cuda120-1.29.0.dev20230721/PACKAGE_NAME
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1708 2023-07-21 14:23:34.309176 nvidia-dali-tf-plugin-nightly-cuda120-1.29.0.dev20230721/PKG-INFO
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      316 2023-07-21 14:23:34.000000 nvidia-dali-tf-plugin-nightly-cuda120-1.29.0.dev20230721/README.rst
+drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-07-21 14:23:34.309176 nvidia-dali-tf-plugin-nightly-cuda120-1.29.0.dev20230721/nvidia_dali_tf_plugin_nightly_cuda120.egg-info/
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1708 2023-07-21 14:23:34.000000 nvidia-dali-tf-plugin-nightly-cuda120-1.29.0.dev20230721/nvidia_dali_tf_plugin_nightly_cuda120.egg-info/PKG-INFO
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      297 2023-07-21 14:23:34.000000 nvidia-dali-tf-plugin-nightly-cuda120-1.29.0.dev20230721/nvidia_dali_tf_plugin_nightly_cuda120.egg-info/SOURCES.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-07-21 14:23:34.000000 nvidia-dali-tf-plugin-nightly-cuda120-1.29.0.dev20230721/nvidia_dali_tf_plugin_nightly_cuda120.egg-info/dependency_links.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       22 2023-07-21 14:23:34.000000 nvidia-dali-tf-plugin-nightly-cuda120-1.29.0.dev20230721/nvidia_dali_tf_plugin_nightly_cuda120.egg-info/top_level.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       38 2023-07-21 14:23:34.313176 nvidia-dali-tf-plugin-nightly-cuda120-1.29.0.dev20230721/setup.cfg
+-rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     4560 2023-07-06 05:01:19.000000 nvidia-dali-tf-plugin-nightly-cuda120-1.29.0.dev20230721/setup.py
```

### Comparing `nvidia-dali-tf-plugin-nightly-cuda120-1.29.0.dev20230720/LICENSE.md` & `nvidia-dali-tf-plugin-nightly-cuda120-1.29.0.dev20230721/LICENSE.md`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-nightly-cuda120-1.29.0.dev20230720/PKG-INFO` & `nvidia-dali-tf-plugin-nightly-cuda120-1.29.0.dev20230721/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nvidia-dali-tf-plugin-nightly-cuda120
-Version: 1.29.0.dev20230720
+Version: 1.29.0.dev20230721
 Summary: A fake package to warn the user they are not installing the correct package.
 Home-page: https://github.com/NVIDIA
 Download-URL: https://github.com/NVIDIA
 Author: Kitmaker
 Author-email: kitmaker@nvidia.com
 Maintainer: Kitmaker
 Maintainer-email: kitmaker@nvidia.com
```

### Comparing `nvidia-dali-tf-plugin-nightly-cuda120-1.29.0.dev20230720/nvidia_dali_tf_plugin_nightly_cuda120.egg-info/PKG-INFO` & `nvidia-dali-tf-plugin-nightly-cuda120-1.29.0.dev20230721/nvidia_dali_tf_plugin_nightly_cuda120.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nvidia-dali-tf-plugin-nightly-cuda120
-Version: 1.29.0.dev20230720
+Version: 1.29.0.dev20230721
 Summary: A fake package to warn the user they are not installing the correct package.
 Home-page: https://github.com/NVIDIA
 Download-URL: https://github.com/NVIDIA
 Author: Kitmaker
 Author-email: kitmaker@nvidia.com
 Maintainer: Kitmaker
 Maintainer-email: kitmaker@nvidia.com
```

### Comparing `nvidia-dali-tf-plugin-nightly-cuda120-1.29.0.dev20230720/setup.py` & `nvidia-dali-tf-plugin-nightly-cuda120-1.29.0.dev20230721/setup.py`

 * *Files identical despite different names*

