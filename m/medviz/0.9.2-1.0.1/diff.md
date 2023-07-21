# Comparing `tmp/medviz-0.9.2.tar.gz` & `tmp/medviz-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medviz-0.9.2.tar", last modified: Sat Jun  3 02:13:53 2023, max compression
+gzip compressed data, was "medviz-1.0.1.tar", last modified: Fri Jul 21 18:42:09 2023, max compression
```

## Comparing `medviz-0.9.2.tar` & `medviz-1.0.1.tar`

### file list

```diff
@@ -1,66 +1,67 @@
-drwxr-xr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-06-03 02:13:53.548121 medviz-0.9.2/
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)    36861 2023-05-31 20:04:32.000000 medviz-0.9.2/LICENSE
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)      180 2023-06-01 05:23:25.000000 medviz-0.9.2/MANIFEST.in
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)     2274 2023-06-03 02:13:53.548121 medviz-0.9.2/PKG-INFO
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)     1803 2023-04-27 15:46:29.000000 medviz-0.9.2/README.rst
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)        5 2023-06-03 02:13:47.000000 medviz-0.9.2/VERSION
-drwxr-xr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-06-03 02:13:53.548121 medviz-0.9.2/medviz/
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)     2043 2023-06-01 05:52:20.000000 medviz-0.9.2/medviz/__init__.py
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)      549 2023-05-31 20:21:50.000000 medviz-0.9.2/medviz/bowel.py
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)      218 2023-05-23 22:19:22.000000 medviz-0.9.2/medviz/bowel2.py
-drwxr-xr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-06-03 02:13:53.548121 medviz-0.9.2/medviz/collage/
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)       41 2023-06-01 02:13:13.000000 medviz-0.9.2/medviz/collage/__init__.py
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)     1982 2023-06-01 02:40:53.000000 medviz-0.9.2/medviz/collage/compute_collage.py
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)    24895 2023-05-31 20:21:55.000000 medviz-0.9.2/medviz/collage/main.py
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)     2122 2023-06-01 02:47:15.000000 medviz-0.9.2/medviz/collage/stats.py
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)      134 2023-05-23 22:19:26.000000 medviz-0.9.2/medviz/example.py
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)     1620 2023-05-15 18:19:57.000000 medviz-0.9.2/medviz/fat_mul.py
-drwxr-xr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-06-03 02:13:53.548121 medviz-0.9.2/medviz/multimodal/
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)       85 2023-05-22 16:27:34.000000 medviz-0.9.2/medviz/multimodal/__init__.py
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)     1065 2023-05-24 22:21:17.000000 medviz-0.9.2/medviz/multimodal/save_dicom_metadata.py
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)      509 2023-05-22 16:27:37.000000 medviz-0.9.2/medviz/multimodal/stats.py
-drwxr-xr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-06-03 02:13:53.548121 medviz-0.9.2/medviz/nifti/
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)     4332 2023-06-03 02:07:25.000000 medviz-0.9.2/medviz/nifti/helper.py
-drwxr-xr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-06-03 02:13:53.548121 medviz-0.9.2/medviz/pkg2/
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)      134 2023-05-23 22:19:26.000000 medviz-0.9.2/medviz/pkg2/example.py
-drwxr-xr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-06-03 02:13:53.548121 medviz-0.9.2/medviz/plots/
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)      123 2023-05-23 23:18:05.000000 medviz-0.9.2/medviz/plots/__init__.py
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)     1552 2023-05-18 02:42:18.000000 medviz-0.9.2/medviz/plots/_plot_image.py
-drwxr-xr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-06-03 02:13:53.548121 medviz-0.9.2/medviz/plots/gif/
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)    10203 2023-05-24 04:19:50.000000 medviz-0.9.2/medviz/plots/gif/gif.py
--rw-rw-r--   0 mohsen    (1000) mohsen    (1000)     2217 2023-05-25 02:41:16.000000 medviz-0.9.2/medviz/plots/helper_plot.py
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)     3682 2023-05-24 04:19:50.000000 medviz-0.9.2/medviz/plots/layered_plot2D.py
-drwxr-xr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-06-03 02:13:53.548121 medviz-0.9.2/medviz/plots/plot2d/
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)      238 2023-05-24 02:22:53.000000 medviz-0.9.2/medviz/plots/plot2d/__init__.py
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)     1890 2023-05-24 05:06:19.000000 medviz-0.9.2/medviz/plots/plot2d/image_mask_annotated.py
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)     1831 2023-05-24 05:06:19.000000 medviz-0.9.2/medviz/plots/plot2d/image_masks.py
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)     1633 2023-05-24 02:54:03.000000 medviz-0.9.2/medviz/plots/plot2d/images.py
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)     1891 2023-05-24 02:59:58.000000 medviz-0.9.2/medviz/plots/plot2d/masks.py
-drwxr-xr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-06-03 02:13:53.548121 medviz-0.9.2/medviz/plots/plot3d/
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)      114 2023-05-25 02:26:37.000000 medviz-0.9.2/medviz/plots/plot3d/__init__.py
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)     1890 2023-05-24 05:06:19.000000 medviz-0.9.2/medviz/plots/plot3d/image_mask_annotated.py
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)     2390 2023-05-24 05:06:19.000000 medviz-0.9.2/medviz/plots/plot3d/images.py
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)     2060 2023-05-31 20:21:55.000000 medviz-0.9.2/medviz/plots/plot3d/layered_plot.py
-drwxr-xr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-06-03 02:13:53.548121 medviz-0.9.2/medviz/preprocess/
--rw-rw-r--   0 mohsen    (1000) mohsen    (1000)       87 2023-06-03 02:09:03.000000 medviz-0.9.2/medviz/preprocess/__init__.py
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)     2071 2023-06-03 02:07:25.000000 medviz-0.9.2/medviz/preprocess/mask.py
--rw-rw-r--   0 mohsen    (1000) mohsen    (1000)     2764 2023-06-03 02:10:07.000000 medviz-0.9.2/medviz/preprocess/match_image_mask.py
-drwxr-xr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-06-03 02:13:53.548121 medviz-0.9.2/medviz/utils/
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)      571 2023-06-03 02:07:23.000000 medviz-0.9.2/medviz/utils/__init__.py
--rw-rw-r--   0 mohsen    (1000) mohsen    (1000)     2175 2023-05-13 17:59:38.000000 medviz-0.9.2/medviz/utils/array_profile.py
--rw-rw-r--   0 mohsen    (1000) mohsen    (1000)      662 2023-05-13 18:05:32.000000 medviz-0.9.2/medviz/utils/array_threshold.py
--rwxr-xr-x   0 mohsen    (1000) mohsen    (1000)      152 2023-05-23 22:19:26.000000 medviz-0.9.2/medviz/utils/custom_type.py
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)     4587 2023-05-23 23:25:32.000000 medviz-0.9.2/medviz/utils/helper_mask.py
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)     2583 2023-06-03 02:07:25.000000 medviz-0.9.2/medviz/utils/helper_path.py
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)      689 2023-01-02 16:26:25.000000 medviz-0.9.2/medviz/utils/log.py
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)      859 2023-05-24 05:07:22.000000 medviz-0.9.2/medviz/utils/reader.py
--rwxr-xr-x   0 mohsen    (1000) mohsen    (1000)       80 2023-05-17 19:24:17.000000 medviz-0.9.2/medviz/utils/utility.py
-drwxr-xr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-06-03 02:13:53.548121 medviz-0.9.2/medviz.egg-info/
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)     2274 2023-06-03 02:13:53.000000 medviz-0.9.2/medviz.egg-info/PKG-INFO
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)     1331 2023-06-03 02:13:53.000000 medviz-0.9.2/medviz.egg-info/SOURCES.txt
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)        1 2023-06-03 02:13:53.000000 medviz-0.9.2/medviz.egg-info/dependency_links.txt
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)      190 2023-06-03 02:13:53.000000 medviz-0.9.2/medviz.egg-info/requires.txt
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)        7 2023-06-03 02:13:53.000000 medviz-0.9.2/medviz.egg-info/top_level.txt
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)     1359 2023-06-01 05:50:19.000000 medviz-0.9.2/pyproject.toml
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)       38 2023-06-03 02:13:53.548121 medviz-0.9.2/setup.cfg
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)      170 2023-04-02 14:20:15.000000 medviz-0.9.2/setup.py
+drwxr-xr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-07-21 18:42:09.764025 medviz-1.0.1/
+-rw-r-----   0 mohsen    (1000) mohsen    (1000)    36861 2023-05-31 20:04:32.000000 medviz-1.0.1/LICENSE
+-rw-r-----   0 mohsen    (1000) mohsen    (1000)      180 2023-06-01 05:23:25.000000 medviz-1.0.1/MANIFEST.in
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)     2274 2023-07-21 18:42:09.764025 medviz-1.0.1/PKG-INFO
+-rw-r-----   0 mohsen    (1000) mohsen    (1000)     1803 2023-04-27 15:46:29.000000 medviz-1.0.1/README.rst
+-rw-r-----   0 mohsen    (1000) mohsen    (1000)        5 2023-07-21 18:33:23.000000 medviz-1.0.1/VERSION
+drwxr-xr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-07-21 18:42:09.760025 medviz-1.0.1/medviz/
+-rw-r-----   0 mohsen    (1000) mohsen    (1000)     2325 2023-07-21 18:33:53.000000 medviz-1.0.1/medviz/__init__.py
+drwxr-xr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-07-21 18:42:09.764025 medviz-1.0.1/medviz/collage/
+-rw-r-----   0 mohsen    (1000) mohsen    (1000)       41 2023-06-01 02:13:13.000000 medviz-1.0.1/medviz/collage/__init__.py
+-rw-r-----   0 mohsen    (1000) mohsen    (1000)     1982 2023-06-01 02:40:53.000000 medviz-1.0.1/medviz/collage/compute_collage.py
+-rw-r-----   0 mohsen    (1000) mohsen    (1000)    24895 2023-05-31 20:21:55.000000 medviz-1.0.1/medviz/collage/main.py
+-rw-r-----   0 mohsen    (1000) mohsen    (1000)     2122 2023-06-01 02:47:15.000000 medviz-1.0.1/medviz/collage/stats.py
+drwxr-xr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-07-21 18:42:09.764025 medviz-1.0.1/medviz/multimodal/
+-rw-r-----   0 mohsen    (1000) mohsen    (1000)       85 2023-05-22 16:27:34.000000 medviz-1.0.1/medviz/multimodal/__init__.py
+-rw-r-----   0 mohsen    (1000) mohsen    (1000)     1065 2023-05-24 22:21:17.000000 medviz-1.0.1/medviz/multimodal/save_dicom_metadata.py
+-rw-r-----   0 mohsen    (1000) mohsen    (1000)      509 2023-05-22 16:27:37.000000 medviz-1.0.1/medviz/multimodal/stats.py
+drwxr-xr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-07-21 18:42:09.764025 medviz-1.0.1/medviz/nifti/
+-rw-r-----   0 mohsen    (1000) mohsen    (1000)     4367 2023-06-08 00:11:51.000000 medviz-1.0.1/medviz/nifti/helper.py
+drwxr-xr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-07-21 18:42:09.764025 medviz-1.0.1/medviz/pkg2_local/
+-rw-r-----   0 mohsen    (1000) mohsen    (1000)      134 2023-05-23 22:19:26.000000 medviz-1.0.1/medviz/pkg2_local/example.py
+drwxr-xr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-07-21 18:42:09.764025 medviz-1.0.1/medviz/plots/
+-rw-r-----   0 mohsen    (1000) mohsen    (1000)      123 2023-05-23 23:18:05.000000 medviz-1.0.1/medviz/plots/__init__.py
+-rw-r-----   0 mohsen    (1000) mohsen    (1000)     1552 2023-05-18 02:42:18.000000 medviz-1.0.1/medviz/plots/_plot_image.py
+drwxr-xr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-07-21 18:42:09.764025 medviz-1.0.1/medviz/plots/gif/
+-rw-r-----   0 mohsen    (1000) mohsen    (1000)    10203 2023-05-24 04:19:50.000000 medviz-1.0.1/medviz/plots/gif/gif.py
+-rw-rw----   0 mohsen    (1000) mohsen    (1000)     2217 2023-05-25 02:41:16.000000 medviz-1.0.1/medviz/plots/helper_plot.py
+-rw-r-----   0 mohsen    (1000) mohsen    (1000)     3682 2023-05-24 04:19:50.000000 medviz-1.0.1/medviz/plots/layered_plot2D.py
+drwxr-xr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-07-21 18:42:09.764025 medviz-1.0.1/medviz/plots/plot2d/
+-rw-r-----   0 mohsen    (1000) mohsen    (1000)      238 2023-05-24 02:22:53.000000 medviz-1.0.1/medviz/plots/plot2d/__init__.py
+-rw-r-----   0 mohsen    (1000) mohsen    (1000)     2139 2023-06-08 02:13:51.000000 medviz-1.0.1/medviz/plots/plot2d/image_mask_annotated.py
+-rw-r-----   0 mohsen    (1000) mohsen    (1000)     2332 2023-06-08 02:13:23.000000 medviz-1.0.1/medviz/plots/plot2d/image_masks.py
+-rw-r-----   0 mohsen    (1000) mohsen    (1000)     2359 2023-06-08 04:45:40.000000 medviz-1.0.1/medviz/plots/plot2d/images.py
+-rw-r-----   0 mohsen    (1000) mohsen    (1000)     2593 2023-06-08 04:46:15.000000 medviz-1.0.1/medviz/plots/plot2d/masks.py
+drwxr-xr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-07-21 18:42:09.764025 medviz-1.0.1/medviz/plots/plot3d/
+-rw-r-----   0 mohsen    (1000) mohsen    (1000)      205 2023-06-08 07:01:03.000000 medviz-1.0.1/medviz/plots/plot3d/__init__.py
+-rw-r-----   0 mohsen    (1000) mohsen    (1000)     1890 2023-06-08 07:01:51.000000 medviz-1.0.1/medviz/plots/plot3d/image_mask_annotated.py
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)     2339 2023-07-18 18:20:40.000000 medviz-1.0.1/medviz/plots/plot3d/image_masks.py
+-rw-r-----   0 mohsen    (1000) mohsen    (1000)     3113 2023-06-08 04:47:31.000000 medviz-1.0.1/medviz/plots/plot3d/images.py
+-rw-r-----   0 mohsen    (1000) mohsen    (1000)     2060 2023-05-31 20:21:55.000000 medviz-1.0.1/medviz/plots/plot3d/layered_plot.py
+-rw-r-----   0 mohsen    (1000) mohsen    (1000)     3577 2023-06-08 06:34:09.000000 medviz-1.0.1/medviz/plots/plot3d/masks.py
+drwxr-xr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-07-21 18:42:09.764025 medviz-1.0.1/medviz/preprocess/
+-rw-rw----   0 mohsen    (1000) mohsen    (1000)      120 2023-07-21 18:32:38.000000 medviz-1.0.1/medviz/preprocess/__init__.py
+-rw-r-----   0 mohsen    (1000) mohsen    (1000)     2071 2023-07-16 03:13:55.000000 medviz-1.0.1/medviz/preprocess/mask.py
+-rw-rw----   0 mohsen    (1000) mohsen    (1000)     2764 2023-06-03 02:10:07.000000 medviz-1.0.1/medviz/preprocess/match_image_mask.py
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)     2086 2023-07-21 17:52:29.000000 medviz-1.0.1/medviz/preprocess/resampling.py
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)     2521 2023-07-18 18:47:42.000000 medviz-1.0.1/medviz/preprocess/resampling_local.py
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)     2996 2023-07-21 17:12:55.000000 medviz-1.0.1/medviz/preprocess/resampling_local_new.py
+drwxr-xr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-07-21 18:42:09.764025 medviz-1.0.1/medviz/utils/
+-rw-r-----   0 mohsen    (1000) mohsen    (1000)      614 2023-06-08 00:57:20.000000 medviz-1.0.1/medviz/utils/__init__.py
+-rw-rw----   0 mohsen    (1000) mohsen    (1000)     2175 2023-05-13 17:59:38.000000 medviz-1.0.1/medviz/utils/array_profile.py
+-rw-rw----   0 mohsen    (1000) mohsen    (1000)      662 2023-05-13 18:05:32.000000 medviz-1.0.1/medviz/utils/array_threshold.py
+-rwxr-x---   0 mohsen    (1000) mohsen    (1000)     1069 2023-06-08 00:57:03.000000 medviz-1.0.1/medviz/utils/custom_type.py
+-rw-r-----   0 mohsen    (1000) mohsen    (1000)     4587 2023-05-23 23:25:32.000000 medviz-1.0.1/medviz/utils/helper_mask.py
+-rw-r-----   0 mohsen    (1000) mohsen    (1000)     2583 2023-07-18 18:20:40.000000 medviz-1.0.1/medviz/utils/helper_path.py
+-rw-r-----   0 mohsen    (1000) mohsen    (1000)      689 2023-01-02 16:26:25.000000 medviz-1.0.1/medviz/utils/log.py
+-rw-r-----   0 mohsen    (1000) mohsen    (1000)      859 2023-05-24 05:07:22.000000 medviz-1.0.1/medviz/utils/reader.py
+-rwxr-x---   0 mohsen    (1000) mohsen    (1000)       80 2023-05-17 19:24:17.000000 medviz-1.0.1/medviz/utils/utility.py
+drwxr-xr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-07-21 18:42:09.764025 medviz-1.0.1/medviz.egg-info/
+-rw-r-----   0 mohsen    (1000) mohsen    (1000)     2274 2023-07-21 18:42:09.000000 medviz-1.0.1/medviz.egg-info/PKG-INFO
+-rw-r-----   0 mohsen    (1000) mohsen    (1000)     1444 2023-07-21 18:42:09.000000 medviz-1.0.1/medviz.egg-info/SOURCES.txt
+-rw-r-----   0 mohsen    (1000) mohsen    (1000)        1 2023-07-21 18:42:09.000000 medviz-1.0.1/medviz.egg-info/dependency_links.txt
+-rw-r-----   0 mohsen    (1000) mohsen    (1000)      190 2023-07-21 18:42:09.000000 medviz-1.0.1/medviz.egg-info/requires.txt
+-rw-r-----   0 mohsen    (1000) mohsen    (1000)        7 2023-07-21 18:42:09.000000 medviz-1.0.1/medviz.egg-info/top_level.txt
+-rw-r-----   0 mohsen    (1000) mohsen    (1000)     1359 2023-06-01 05:50:19.000000 medviz-1.0.1/pyproject.toml
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)       38 2023-07-21 18:42:09.764025 medviz-1.0.1/setup.cfg
+-rw-r-----   0 mohsen    (1000) mohsen    (1000)      170 2023-04-02 14:20:15.000000 medviz-1.0.1/setup.py
```

### Comparing `medviz-0.9.2/LICENSE` & `medviz-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `medviz-0.9.2/PKG-INFO` & `medviz-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medviz
-Version: 0.9.2
+Version: 1.0.1
 Summary: Medical Image Visualization Tool 🐍🚀🎉🦕
 Author-email: Mohsen Hariri <mohsen.hariri@case.eud>
 License: GPL-3.0 License
 Keywords: MRI,CT
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `medviz-0.9.2/README.rst` & `medviz-1.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `medviz-0.9.2/medviz/__init__.py` & `medviz-1.0.1/medviz/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -46,36 +46,48 @@
 )
 
 ### PLOT 3D ###
 
 
 from .plots.plot3d import layered_slider_array, layered_slider_path
 
-# from .plots.plot3d.images import (
-#     images_array as plot3d_images_array,
-#     images_path as plot3d_images_path,
-# )
+from .plots.plot3d.images import (
+    images_array as plot3d_images_array,
+    images_path as plot3d_images_path,
+)
+
+from .plots.plot3d.masks import (
+    masks_array as plot3d_masks_array,
+    masks_path as plot3d_masks_path,
+)
+
+from .plots.plot3d.image_masks import (
+    image_masks_path as plot3d_image_masks_path,
+    image_masks_array as plot3d_image_masks_array,
+)
 
 # from .plots.plot3d.layered_plot import (
 #     layered_plot_data3D as plot3d_layered_data,
 #     layered_plot_path3D as plot3d_layered_path,
 # )
 
 # from .plots.gif import gif, gif_slices, gif_non, gif_reference
 
 
 from .multimodal import save_dicom_metadata, filter_dicom
 
 from .preprocess import *
+from .preprocess import resample
 
 from .collage import compute_stats_collage
 
 from .nifti.helper import nii3d_to_annotated2d, nii_mask3d_to_2d
 
 # def version():
 #     with open("VERSION", "r") as f:
 #         version = f.read().strip()
 #     return version
 
 # __version__ = version()
 
-__version__ = "0.8.8"
+__version__ = "1.0.1"
+
```

### Comparing `medviz-0.9.2/medviz/collage/compute_collage.py` & `medviz-1.0.1/medviz/collage/compute_collage.py`

 * *Files identical despite different names*

### Comparing `medviz-0.9.2/medviz/collage/main.py` & `medviz-1.0.1/medviz/collage/main.py`

 * *Files identical despite different names*

### Comparing `medviz-0.9.2/medviz/collage/stats.py` & `medviz-1.0.1/medviz/collage/stats.py`

 * *Files identical despite different names*

### Comparing `medviz-0.9.2/medviz/multimodal/save_dicom_metadata.py` & `medviz-1.0.1/medviz/multimodal/save_dicom_metadata.py`

 * *Files identical despite different names*

### Comparing `medviz-0.9.2/medviz/nifti/helper.py` & `medviz-1.0.1/medviz/nifti/helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from pathlib import Path
 
 import nibabel as nib
 import numpy as np
 
-from medviz.utils.helper_mask import significant_slice_idx_data
+from ..utils import path_in, save_path_dir, significant_slice_idx
 
-from ..utils import save_path_dir, significant_slice_idx
 
-
-def nifti_to_hu(file_path: str or Path):
+# add save_path to save the image (Optional)
+def to_hu(file_path: str or Path):
     """
     read the image and convert it to hu image
     :param file_path: file path
     :return: hu image
     """
+    file_path = path_in(file_path)
     image = nib.load(file_path)
     image_data = image.get_fdata()
 
     slope = image.dataobj.slope
     intercept = image.dataobj.inter
 
     is_hu_format = (slope == 1) and (intercept <= 0)
@@ -43,15 +43,15 @@
 #     mask_data = np.zeros(mask_data_bool.shape, dtype=np.int16)
 #     mask_data[mask_data_bool] = 1
 #     mask_img = nib.Nifti1Image(mask_data, affine)
 #     nib.save(mask_img, output_path)
 #     print("Mask saved at", output_path)
 
 
-def mask(mask_data_bool: np.ndarray, affine: np.ndarray, output_path: str):
+def boolean_mask_to_nifti(mask_data_bool: np.ndarray, affine: np.ndarray, output_path: str):
     """
     Save mask as nii.gz file
     :param mask_data_bool: mask data as boolean numpy array
     :param affine: affine matrix
     :param output_path: output path
     :return: None
     """
```

### Comparing `medviz-0.9.2/medviz/plots/_plot_image.py` & `medviz-1.0.1/medviz/plots/_plot_image.py`

 * *Files identical despite different names*

### Comparing `medviz-0.9.2/medviz/plots/gif/gif.py` & `medviz-1.0.1/medviz/plots/gif/gif.py`

 * *Files identical despite different names*

### Comparing `medviz-0.9.2/medviz/plots/helper_plot.py` & `medviz-1.0.1/medviz/plots/helper_plot.py`

 * *Files identical despite different names*

### Comparing `medviz-0.9.2/medviz/plots/layered_plot2D.py` & `medviz-1.0.1/medviz/plots/layered_plot2D.py`

 * *Files identical despite different names*

### Comparing `medviz-0.9.2/medviz/plots/plot2d/image_mask_annotated.py` & `medviz-1.0.1/medviz/plots/plot3d/image_mask_annotated.py`

 * *Files identical despite different names*

### Comparing `medviz-0.9.2/medviz/plots/plot2d/image_masks.py` & `medviz-1.0.1/medviz/plots/plot2d/image_masks.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,39 @@
 from ...plots import (
     assert_shape,
     generate_mask_colors,
     plot_contour,
     plot_image,
     save_image,
 )
-from ...utils import image_path_to_data_ax, mask_path_to_data_ax, save_path_file
+from ...utils import (
+    image_path_to_data_ax,
+    mask_path_to_data_ax,
+    path_in,
+    save_path_file,
+)
 
 
 def image_masks_path(
     image_path,
     masks_path,
     mask_colors=None,
     titles=[],
     title_image="Image",
     cmap="gray",
     origin="upper",
     save_path=None,
 ):
+    if len(masks_path) == 0:
+        raise ValueError("masks_path must be a list of paths")
+
+    image_path = path_in(image_path)
     image_data = image_path_to_data_ax(image_path)
+
+    masks_path = [path_in(path) for path in masks_path]
     masks_data = [mask_path_to_data_ax(path) for path in masks_path]
 
     image_masks_array(
         image_data=image_data,
         masks_data=masks_data,
         mask_colors=mask_colors,
         titles=titles,
@@ -43,16 +54,26 @@
     mask_colors=None,
     titles=[],
     title_image="Image",
     cmap="gray",
     origin="upper",
     save_path=None,
 ):
+    if len(masks_data) == 0:
+        raise ValueError("masks_data must be a list of arrays")
+
     print("Loading images...")
 
+    if image_data.ndim != 2:
+        raise ValueError("Image must be 2D")
+
+    for mask_data in masks_data:
+        if mask_data.ndim != 2:
+            raise ValueError("Masks must be 2D")
+
     num_masks = len(masks_data)
 
     # assert_shape(image_data + masks_data)
 
     mask_colors = generate_mask_colors(num_masks, mask_colors)
 
     _, ax = plt.subplots()
```

### Comparing `medviz-0.9.2/medviz/plots/plot2d/images.py` & `medviz-1.0.1/medviz/plots/plot2d/images.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,67 +1,92 @@
 import math
 
 import matplotlib.pyplot as plt
 import numpy as np
 
 from ...plots import plot_image, save_image
-from ...utils import image_path_to_data_ax, save_path_file
+from ...utils import (
+    NumLst,
+    PathType,
+    PathTypeLst,
+    StrLst,
+    image_path_to_data_ax,
+    path_in,
+    save_path_file,
+)
 
 
 def images_path(
-    paths,
-    rows=None,
-    columns=None,
-    titles=[],
-    cmap="gray",
-    origin="upper",
-    save_path=None,
+    paths: PathTypeLst,
+    rows: int or None = None,
+    columns: int or None = None,
+    titles: StrLst = [],
+    cmap: str or None = "gray",
+    origin: str or None = "upper",
+    save_path: PathType or None = None,
 ):
+    if len(paths) == 0:
+        raise ValueError("paths must be a list of paths")
+
+    paths = [path_in(path) for path in paths]
+
     images_data = [image_path_to_data_ax(path) for path in paths]
 
     images_array(
         images_data=images_data,
         rows=rows,
         columns=columns,
         titles=titles,
         cmap=cmap,
         origin=origin,
         save_path=save_path,
     )
 
 
 def images_array(
-    images_data,
+    images_data: NumLst,
     rows=None,
     columns=None,
     titles=[],
     cmap="gray",
     origin="upper",
     save_path=None,
 ):
     print("Loading images...")
 
-    try:
-        assert len(images_data[0].shape) == 2
-    except AssertionError:
-        raise ValueError("Images must be 2D")
+    if len(images_data) == 0:
+        raise ValueError("images_data must be a list of arrays")
+
+    for image_data in images_data:
+        if image_data.ndim != 2:
+            raise ValueError("Images must be 2D")
 
     num_images = len(images_data)  # Number of images
-    rows = math.ceil(math.sqrt(num_images))  # Number of rows in the grid
-    columns = math.ceil(num_images / rows)  # Number of columns in the grid
+
+    if rows is None and columns is None:
+        rows = math.ceil(math.sqrt(num_images))  # Number of rows in the grid
+        columns = math.ceil(num_images / rows)  # Number of columns in the grid
+    elif rows is None:
+        rows = math.ceil(num_images / columns)
+    elif columns is None:
+        columns = math.ceil(num_images / rows)
+
+    if num_images > rows * columns:
+        raise ValueError("rows * columns must be greater than or equal to num_images")
 
     _, axs = plt.subplots(rows, columns)
     if num_images == 1:
         axs = np.array([axs])
 
     for i, ax in enumerate(axs.flat):
         if i < num_images:
             title = titles[i] if titles else f"Image {i}"
             plot_image(ax, images_data[i], cmap=cmap, title=title, origin=origin)
             ax.axis("off")
+
         else:
             ax.axis("off")
 
     plt.tight_layout()
 
     if save_path:
         save_path = save_path_file(save_path, suffix=".png")
```

### Comparing `medviz-0.9.2/medviz/plots/plot2d/masks.py` & `medviz-1.0.1/medviz/plots/plot2d/image_mask_annotated.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,76 +1,82 @@
+"""
+INPUT: 3D image, 3D mask
+Finds slices with the most values 
+
+OUTPU: 2D images
+"""
+
 import math
 
 import matplotlib.pyplot as plt
 import numpy as np
 
-from ...plots import generate_mask_colors, plot_contour, save_image
-from ...utils import mask_path_to_data_ax, save_path_file
+from ...plots import generate_mask_colors, plot_contour, plot_image, save_image
+from ...utils import (
+    PathType,
+    image_path_to_data_ax,
+    mask_path_to_data_ax,
+    path_in,
+    save_path_file,
+    significant_slice_idx_data,
+)
 
 
-def masks_path(
-    paths,
-    rows=None,
-    columns=None,
-    mask_colors=None,
-    titles=[],
-    origin="upper",
+def image_mask_annotated_path(
+    image_path: PathType,
+    mask_path: PathType,
+    cmap="gray",
     save_path=None,
+    limit: int = 10,
 ):
-    masks_data = [mask_path_to_data_ax(path) for path in paths]  # just for nifti files
+    image_path = path_in(image_path)
+    mask_path = path_in(mask_path)
+
+    image_data = image_path_to_data_ax(image_path)
+    mask_data = mask_path_to_data_ax(mask_path)
 
-    masks_array(
-        masks_data=masks_data,
-        rows=rows,
-        columns=columns,
-        titles=titles,
-        origin=origin,
-        mask_colors=mask_colors,
+    image_mask_annotated_array(
+        image_data=image_data,
+        mask_data=mask_data,
+        cmap=cmap,
         save_path=save_path,
+        limit=limit,
     )
 
 
-def masks_array(
-    masks_data,
-    rows=None,
-    columns=None,
-    titles=[],
-    mask_colors=None,
-    origin="upper",
+def image_mask_annotated_array(
+    image_data,
+    mask_data,
+    cmap="gray",
     save_path=None,
+    limit: int = 10,
 ):
     print("Loading images...")
 
-    try:
-        assert len(masks_data[0].shape) == 2
-    except AssertionError:
-        raise ValueError("Masks must be 2D")
+    most_value_nonzero_slices, num_nonzero_slices = significant_slice_idx_data(mask_data)
+    num_masks = min(num_nonzero_slices, limit)
 
-    num_masks = len(masks_data)  # Number of images
     rows = math.ceil(math.sqrt(num_masks))  # Number of rows in the grid
     columns = math.ceil(num_masks / rows)  # Number of columns in the grid
 
-    mask_colors = generate_mask_colors(num_masks, mask_colors)
+    mask_colors = generate_mask_colors(num_masks)
 
     _, axs = plt.subplots(rows, columns)
+
     if num_masks == 1:
         axs = np.array([axs])
 
     for i, ax in enumerate(axs.flat):
         if i < num_masks:
-            title = titles[i] if titles else f"Mask {i}"
-
+            # title = titles[i] if titles else f"Image {i}"
+            plot_image(ax, image_data[:, :, most_value_nonzero_slices[i]], cmap=cmap)
             plot_contour(
-                ax,
-                masks_data[i],
-                color=mask_colors[i],
-                title=title,
-                origin=origin,
-                levels=[0.5],
+                ax, mask_data[:, :, most_value_nonzero_slices[i]], color=mask_colors[i], levels=[0.5]
             )
+            ax.set_title(f"Slice {most_value_nonzero_slices[i]}")
             # ax.axis("off")
         else:
             ax.axis("off")
 
     plt.tight_layout()
 
     if save_path:
```

### Comparing `medviz-0.9.2/medviz/plots/plot3d/images.py` & `medviz-1.0.1/medviz/plots/plot3d/images.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,50 +1,84 @@
 import math
 
 import matplotlib.pyplot as plt
 import numpy as np
 from matplotlib.widgets import Slider
 
-from ...plots import plot_image, save_image
-from ...utils import image_path_to_data_ax
+from ...plots import plot_image
+from ...utils import NumLst, PathTypeLst, StrLst, image_path_to_data_ax, path_in
 
 
-def images_path(paths, rows=None, columns=None, titles=[], cmap="gray"):
+def images_path(
+    paths: PathTypeLst,
+    rows: int or None = None,
+    columns: int or None = None,
+    titles: StrLst = [],
+    cmap: str or None = "gray",
+):
+    if len(paths) == 0:
+        raise ValueError("paths must be a list of paths")
+
+    paths = [path_in(path) for path in paths]
+
     images_data = [image_path_to_data_ax(path) for path in paths]
 
     images_array(
         images_data=images_data,
         rows=rows,
         columns=columns,
         titles=titles,
         cmap=cmap,
     )
 
 
-def images_array(images_data, rows=None, columns=None, titles=[], cmap="gray"):
+def images_array(
+    images_data: NumLst,
+    rows=None,
+    columns=None,
+    titles=[],
+    cmap="gray",
+):
     print("Loading images...")
 
-    d = images_data[0].shape[2]
-    init_slice, last_slice = d // 2, d - 1
+    if len(images_data) == 0:
+        raise ValueError("images_data must be a list of arrays")
+
+    for image_data in images_data:
+        if image_data.ndim != 3:
+            raise ValueError("images_data must be a list of 3D arrays")
 
     num_images = len(images_data)  # Number of images
-    rows = math.ceil(math.sqrt(num_images))  # Number of rows in the grid
-    columns = math.ceil(num_images / rows)  # Number of columns in the grid
+
+    if rows is None and columns is None:
+        rows = math.ceil(math.sqrt(num_images))  # Number of rows in the grid
+        columns = math.ceil(num_images / rows)  # Number of columns in the grid
+    elif rows is None:
+        rows = math.ceil(num_images / columns)
+    elif columns is None:
+        columns = math.ceil(num_images / rows)
+
+    if num_images > rows * columns:
+        raise ValueError("rows * columns must be greater than or equal to num_images")
+
+    depth = [image_data.shape[2] for image_data in images_data]
+
+    init_slice, last_slice = int(np.mean(depth) // 2), np.max(depth) - 2
 
     _, axs = plt.subplots(rows, columns)
     if num_images == 1:
         axs = np.array([axs])
 
     plt.subplots_adjust(bottom=0.25)
 
     for i, ax in enumerate(axs.flat):
         if i < num_images:
             title = titles[i] if titles else f"Image {i}"
             plot_image(ax, images_data[i][:, :, init_slice], cmap=cmap, title=title)
-            ax.axis("off")
+            # ax.axis("off")
             ax.set_xlabel(f"Slice Number: {init_slice}")
 
         else:
             ax.axis("off")
 
     slider_ax = plt.axes([0.2, 0.1, 0.6, 0.03])
 
@@ -62,30 +96,21 @@
 
         for i, ax in enumerate(axs.flat):
             ax.clear()
 
             if i < num_images:
                 title = titles[i] if titles else f"Image {i}"
 
+                if images_data[i].shape[2] <= slice_num:
+                    slice_num = images_data[i].shape[2] - 1
                 plot_image(ax, images_data[i][:, :, slice_num], cmap=cmap, title=title)
                 ax.set_xlabel(f"Slice Number: {slice_num}")
-                ax.axis("off")
+                # ax.axis("off")
             else:
                 ax.axis("off")
-
+                pass
         # ax.set_title(title)
 
     slider.on_changed(update)
 
     plt.tight_layout()
     plt.show()
-
-
-# import nibabel as nib
-
-# if __name__ == "__main__":
-#     ct_image = nib.load("dataset/1-1.nii")
-#     ct_data = ct_image.get_fdata()
-#     print(ct_data.shape)
-#     ct_data = image_path_to_data("dataset/1-1.nii")
-#     # ct_data = ct_data[:, :, 100]
-#     plot_multi_data([ct_data, ct_data], title="Image")
```

### Comparing `medviz-0.9.2/medviz/plots/plot3d/layered_plot.py` & `medviz-1.0.1/medviz/plots/plot3d/layered_plot.py`

 * *Files identical despite different names*

### Comparing `medviz-0.9.2/medviz/preprocess/mask.py` & `medviz-1.0.1/medviz/preprocess/mask.py`

 * *Files identical despite different names*

### Comparing `medviz-0.9.2/medviz/preprocess/match_image_mask.py` & `medviz-1.0.1/medviz/preprocess/match_image_mask.py`

 * *Files identical despite different names*

### Comparing `medviz-0.9.2/medviz/utils/__init__.py` & `medviz-1.0.1/medviz/utils/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from .custom_type import PathType
+from .custom_type import PathType, PathTypeLst, PathTypeIter, StrLst, NumLst
 from .utility import now
 from .array_profile import profile
 from .array_threshold import compute_thresholds
 
 # from .helper_path import path_in, save_path_file, save_path_dir
 
 from .helper_mask import (
```

### Comparing `medviz-0.9.2/medviz/utils/array_profile.py` & `medviz-1.0.1/medviz/utils/array_profile.py`

 * *Files identical despite different names*

### Comparing `medviz-0.9.2/medviz/utils/array_threshold.py` & `medviz-1.0.1/medviz/utils/array_threshold.py`

 * *Files identical despite different names*

### Comparing `medviz-0.9.2/medviz/utils/helper_mask.py` & `medviz-1.0.1/medviz/utils/helper_mask.py`

 * *Files identical despite different names*

### Comparing `medviz-0.9.2/medviz/utils/helper_path.py` & `medviz-1.0.1/medviz/utils/helper_path.py`

 * *Files identical despite different names*

### Comparing `medviz-0.9.2/medviz/utils/log.py` & `medviz-1.0.1/medviz/utils/log.py`

 * *Files identical despite different names*

### Comparing `medviz-0.9.2/medviz/utils/reader.py` & `medviz-1.0.1/medviz/utils/reader.py`

 * *Files identical despite different names*

### Comparing `medviz-0.9.2/medviz.egg-info/PKG-INFO` & `medviz-1.0.1/medviz.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medviz
-Version: 0.9.2
+Version: 1.0.1
 Summary: Medical Image Visualization Tool 🐍🚀🎉🦕
 Author-email: Mohsen Hariri <mohsen.hariri@case.eud>
 License: GPL-3.0 License
 Keywords: MRI,CT
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `medviz-0.9.2/medviz.egg-info/SOURCES.txt` & `medviz-1.0.1/medviz.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,49 +1,50 @@
 LICENSE
 MANIFEST.in
 README.rst
 VERSION
 pyproject.toml
 setup.py
 medviz/__init__.py
-medviz/bowel.py
-medviz/bowel2.py
-medviz/example.py
-medviz/fat_mul.py
 medviz.egg-info/PKG-INFO
 medviz.egg-info/SOURCES.txt
 medviz.egg-info/dependency_links.txt
 medviz.egg-info/requires.txt
 medviz.egg-info/top_level.txt
 medviz/collage/__init__.py
 medviz/collage/compute_collage.py
 medviz/collage/main.py
 medviz/collage/stats.py
 medviz/multimodal/__init__.py
 medviz/multimodal/save_dicom_metadata.py
 medviz/multimodal/stats.py
 medviz/nifti/helper.py
-medviz/pkg2/example.py
+medviz/pkg2_local/example.py
 medviz/plots/__init__.py
 medviz/plots/_plot_image.py
 medviz/plots/helper_plot.py
 medviz/plots/layered_plot2D.py
 medviz/plots/gif/gif.py
 medviz/plots/plot2d/__init__.py
 medviz/plots/plot2d/image_mask_annotated.py
 medviz/plots/plot2d/image_masks.py
 medviz/plots/plot2d/images.py
 medviz/plots/plot2d/masks.py
 medviz/plots/plot3d/__init__.py
 medviz/plots/plot3d/image_mask_annotated.py
+medviz/plots/plot3d/image_masks.py
 medviz/plots/plot3d/images.py
 medviz/plots/plot3d/layered_plot.py
+medviz/plots/plot3d/masks.py
 medviz/preprocess/__init__.py
 medviz/preprocess/mask.py
 medviz/preprocess/match_image_mask.py
+medviz/preprocess/resampling.py
+medviz/preprocess/resampling_local.py
+medviz/preprocess/resampling_local_new.py
 medviz/utils/__init__.py
 medviz/utils/array_profile.py
 medviz/utils/array_threshold.py
 medviz/utils/custom_type.py
 medviz/utils/helper_mask.py
 medviz/utils/helper_path.py
 medviz/utils/log.py
```

### Comparing `medviz-0.9.2/pyproject.toml` & `medviz-1.0.1/pyproject.toml`

 * *Files identical despite different names*

