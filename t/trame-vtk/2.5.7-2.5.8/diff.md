# Comparing `tmp/trame-vtk-2.5.7.tar.gz` & `tmp/trame-vtk-2.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trame-vtk-2.5.7.tar", last modified: Thu Jul 20 03:21:41 2023, max compression
+gzip compressed data, was "trame-vtk-2.5.8.tar", last modified: Thu Jul 20 23:41:23 2023, max compression
```

## Comparing `trame-vtk-2.5.7.tar` & `trame-vtk-2.5.8.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 03:21:41.934354 trame-vtk-2.5.7/
--rw-r--r--   0 root         (0) root         (0)     1504 2023-07-20 03:21:37.000000 trame-vtk-2.5.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)      106 2023-07-20 03:21:37.000000 trame-vtk-2.5.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    12927 2023-07-20 03:21:41.934354 trame-vtk-2.5.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    12192 2023-07-20 03:21:37.000000 trame-vtk-2.5.7/README.rst
--rw-r--r--   0 root         (0) root         (0)      878 2023-07-20 03:21:41.934354 trame-vtk-2.5.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-20 03:21:37.000000 trame-vtk-2.5.7/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 03:21:41.922354 trame-vtk-2.5.7/trame/
--rw-r--r--   0 root         (0) root         (0)       65 2023-07-20 03:21:37.000000 trame-vtk-2.5.7/trame/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 03:21:41.926354 trame-vtk-2.5.7/trame/modules/
--rw-r--r--   0 root         (0) root         (0)       65 2023-07-20 03:21:37.000000 trame-vtk-2.5.7/trame/modules/__init__.py
--rw-r--r--   0 root         (0) root         (0)       39 2023-07-20 03:21:37.000000 trame-vtk-2.5.7/trame/modules/paraview.py
--rw-r--r--   0 root         (0) root         (0)       39 2023-07-20 03:21:37.000000 trame-vtk-2.5.7/trame/modules/vtk.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 03:21:41.926354 trame-vtk-2.5.7/trame/tools/
--rw-r--r--   0 root         (0) root         (0)       65 2023-07-20 03:21:37.000000 trame-vtk-2.5.7/trame/tools/__init__.py
--rw-r--r--   0 root         (0) root         (0)       83 2023-07-20 03:21:37.000000 trame-vtk-2.5.7/trame/tools/vtksz2html.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 03:21:41.926354 trame-vtk-2.5.7/trame/widgets/
--rw-r--r--   0 root         (0) root         (0)       65 2023-07-20 03:21:37.000000 trame-vtk-2.5.7/trame/widgets/__init__.py
--rw-r--r--   0 root         (0) root         (0)      182 2023-07-20 03:21:37.000000 trame-vtk-2.5.7/trame/widgets/paraview.py
--rw-r--r--   0 root         (0) root         (0)      172 2023-07-20 03:21:37.000000 trame-vtk-2.5.7/trame/widgets/vtk.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 03:21:41.926354 trame-vtk-2.5.7/trame_vtk/
--rw-r--r--   0 root         (0) root         (0)     1504 2023-07-20 03:21:37.000000 trame-vtk-2.5.7/trame_vtk/LICENSE
--rw-r--r--   0 root         (0) root         (0)       91 2023-07-20 03:21:37.000000 trame-vtk-2.5.7/trame_vtk/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 03:21:41.926354 trame-vtk-2.5.7/trame_vtk/modules/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-20 03:21:37.000000 trame-vtk-2.5.7/trame_vtk/modules/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 03:21:41.926354 trame-vtk-2.5.7/trame_vtk/modules/common/
--rw-r--r--   0 root         (0) root         (0)      354 2023-07-20 03:21:37.000000 trame-vtk-2.5.7/trame_vtk/modules/common/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 03:21:41.926354 trame-vtk-2.5.7/trame_vtk/modules/common/serve/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 03:21:37.000000 trame-vtk-2.5.7/trame_vtk/modules/common/serve/.gitignore
--rw-r--r--   0 root         (0) root         (0)  1693968 2023-07-20 03:21:38.000000 trame-vtk-2.5.7/trame_vtk/modules/common/serve/trame-vtk.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 03:21:41.930354 trame-vtk-2.5.7/trame_vtk/modules/paraview/
--rw-r--r--   0 root         (0) root         (0)     7896 2023-07-20 03:21:37.000000 trame-vtk-2.5.7/trame_vtk/modules/paraview/__init__.py
--rw-r--r--   0 root         (0) root         (0)      627 2023-07-20 03:21:37.000000 trame-vtk-2.5.7/trame_vtk/modules/paraview/core.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 03:21:41.930354 trame-vtk-2.5.7/trame_vtk/modules/paraview/protocols/
--rw-r--r--   0 root         (0) root         (0)      363 2023-07-20 03:21:37.000000 trame-vtk-2.5.7/trame_vtk/modules/paraview/protocols/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5356 2023-07-20 03:21:37.000000 trame-vtk-2.5.7/trame_vtk/modules/paraview/protocols/local_rendering.py
--rw-r--r--   0 root         (0) root         (0)     2233 2023-07-20 03:21:37.000000 trame-vtk-2.5.7/trame_vtk/modules/paraview/protocols/mouse_handler.py
--rw-r--r--   0 root         (0) root         (0)    23952 2023-07-20 03:21:37.000000 trame-vtk-2.5.7/trame_vtk/modules/paraview/protocols/publish_image_delivery.py
--rw-r--r--   0 root         (0) root         (0)     3565 2023-07-20 03:21:37.000000 trame-vtk-2.5.7/trame_vtk/modules/paraview/protocols/view_port.py
--rw-r--r--   0 root         (0) root         (0)     4170 2023-07-20 03:21:37.000000 trame-vtk-2.5.7/trame_vtk/modules/paraview/protocols/web_protocol.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 03:21:41.930354 trame-vtk-2.5.7/trame_vtk/modules/vtk/
--rw-r--r--   0 root         (0) root         (0)     7639 2023-07-20 03:21:37.000000 trame-vtk-2.5.7/trame_vtk/modules/vtk/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2738 2023-07-20 03:21:37.000000 trame-vtk-2.5.7/trame_vtk/modules/vtk/core.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 03:21:41.930354 trame-vtk-2.5.7/trame_vtk/modules/vtk/protocols/
--rw-r--r--   0 root         (0) root         (0)      322 2023-07-20 03:21:37.000000 trame-vtk-2.5.7/trame_vtk/modules/vtk/protocols/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5574 2023-07-20 03:21:37.000000 trame-vtk-2.5.7/trame_vtk/modules/vtk/protocols/local_rendering.py
--rw-r--r--   0 root         (0) root         (0)     3981 2023-07-20 03:21:37.000000 trame-vtk-2.5.7/trame_vtk/modules/vtk/protocols/mouse_handler.py
--rw-r--r--   0 root         (0) root         (0)    12797 2023-07-20 03:21:37.000000 trame-vtk-2.5.7/trame_vtk/modules/vtk/protocols/publish_image_delivery.py
--rw-r--r--   0 root         (0) root         (0)     1973 2023-07-20 03:21:37.000000 trame-vtk-2.5.7/trame_vtk/modules/vtk/protocols/view_port.py
--rw-r--r--   0 root         (0) root         (0)     1787 2023-07-20 03:21:37.000000 trame-vtk-2.5.7/trame_vtk/modules/vtk/protocols/web_protocol.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 03:21:41.934354 trame-vtk-2.5.7/trame_vtk/modules/vtk/serializers/
--rw-r--r--   0 root         (0) root         (0)      726 2023-07-20 03:21:37.000000 trame-vtk-2.5.7/trame_vtk/modules/vtk/serializers/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12646 2023-07-20 03:21:37.000000 trame-vtk-2.5.7/trame_vtk/modules/vtk/serializers/actors.py
--rw-r--r--   0 root         (0) root         (0)      463 2023-07-20 03:21:37.000000 trame-vtk-2.5.7/trame_vtk/modules/vtk/serializers/cache.py
--rw-r--r--   0 root         (0) root         (0)     6188 2023-07-20 03:21:37.000000 trame-vtk-2.5.7/trame_vtk/modules/vtk/serializers/data.py
--rw-r--r--   0 root         (0) root         (0)      926 2023-07-20 03:21:37.000000 trame-vtk-2.5.7/trame_vtk/modules/vtk/serializers/export.py
--rw-r--r--   0 root         (0) root         (0)     5785 2023-07-20 03:21:37.000000 trame-vtk-2.5.7/trame_vtk/modules/vtk/serializers/helpers.py
--rw-r--r--   0 root         (0) root         (0)     4772 2023-07-20 03:21:37.000000 trame-vtk-2.5.7/trame_vtk/modules/vtk/serializers/initialize.py
--rw-r--r--   0 root         (0) root         (0)     1528 2023-07-20 03:21:37.000000 trame-vtk-2.5.7/trame_vtk/modules/vtk/serializers/lights.py
--rw-r--r--   0 root         (0) root         (0)     6059 2023-07-20 03:21:37.000000 trame-vtk-2.5.7/trame_vtk/modules/vtk/serializers/lookup_tables.py
--rw-r--r--   0 root         (0) root         (0)     5431 2023-07-20 03:21:37.000000 trame-vtk-2.5.7/trame_vtk/modules/vtk/serializers/mappers.py
--rw-r--r--   0 root         (0) root         (0)     6041 2023-07-20 03:21:37.000000 trame-vtk-2.5.7/trame_vtk/modules/vtk/serializers/mesh.py
--rw-r--r--   0 root         (0) root         (0)     3471 2023-07-20 03:21:37.000000 trame-vtk-2.5.7/trame_vtk/modules/vtk/serializers/properties.py
--rw-r--r--   0 root         (0) root         (0)      378 2023-07-20 03:21:37.000000 trame-vtk-2.5.7/trame_vtk/modules/vtk/serializers/registry.py
--rw-r--r--   0 root         (0) root         (0)     4978 2023-07-20 03:21:37.000000 trame-vtk-2.5.7/trame_vtk/modules/vtk/serializers/render_windows.py
--rw-r--r--   0 root         (0) root         (0)      914 2023-07-20 03:21:37.000000 trame-vtk-2.5.7/trame_vtk/modules/vtk/serializers/serialize.py
--rw-r--r--   0 root         (0) root         (0)     3541 2023-07-20 03:21:37.000000 trame-vtk-2.5.7/trame_vtk/modules/vtk/serializers/synchronization_context.py
--rw-r--r--   0 root         (0) root         (0)     1337 2023-07-20 03:21:37.000000 trame-vtk-2.5.7/trame_vtk/modules/vtk/serializers/textures.py
--rw-r--r--   0 root         (0) root         (0)     1946 2023-07-20 03:21:37.000000 trame-vtk-2.5.7/trame_vtk/modules/vtk/serializers/utils.py
--rw-r--r--   0 root         (0) root         (0)     1595 2023-07-20 03:21:37.000000 trame-vtk-2.5.7/trame_vtk/modules/vtk/serializers/widgets.py
--rw-r--r--   0 root         (0) root         (0)     4551 2023-07-20 03:21:37.000000 trame-vtk-2.5.7/trame_vtk/modules/vtk/widget.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 03:21:41.934354 trame-vtk-2.5.7/trame_vtk/tools/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-20 03:21:37.000000 trame-vtk-2.5.7/trame_vtk/tools/__init__.py
--rw-r--r--   0 root         (0) root         (0)   970597 2023-07-20 03:21:38.000000 trame-vtk-2.5.7/trame_vtk/tools/static_viewer.html
--rw-r--r--   0 root         (0) root         (0)     1713 2023-07-20 03:21:37.000000 trame-vtk-2.5.7/trame_vtk/tools/vtksz2html.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 03:21:41.934354 trame-vtk-2.5.7/trame_vtk/widgets/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-20 03:21:37.000000 trame-vtk-2.5.7/trame_vtk/widgets/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 03:21:41.934354 trame-vtk-2.5.7/trame_vtk/widgets/vtk/
--rw-r--r--   0 root         (0) root         (0)      645 2023-07-20 03:21:37.000000 trame-vtk-2.5.7/trame_vtk/widgets/vtk/__init__.py
--rw-r--r--   0 root         (0) root         (0)    33204 2023-07-20 03:21:37.000000 trame-vtk-2.5.7/trame_vtk/widgets/vtk/common.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 03:21:41.926354 trame-vtk-2.5.7/trame_vtk.egg-info/
--rw-r--r--   0 root         (0) root         (0)    12927 2023-07-20 03:21:41.000000 trame-vtk-2.5.7/trame_vtk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2481 2023-07-20 03:21:41.000000 trame-vtk-2.5.7/trame_vtk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 03:21:41.000000 trame-vtk-2.5.7/trame_vtk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-20 03:21:41.000000 trame-vtk-2.5.7/trame_vtk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-07-20 03:21:41.000000 trame-vtk-2.5.7/trame_vtk.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 23:41:23.161276 trame-vtk-2.5.8/
+-rw-r--r--   0 root         (0) root         (0)     1504 2023-07-20 23:41:19.000000 trame-vtk-2.5.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      106 2023-07-20 23:41:19.000000 trame-vtk-2.5.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    12927 2023-07-20 23:41:23.161276 trame-vtk-2.5.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    12192 2023-07-20 23:41:19.000000 trame-vtk-2.5.8/README.rst
+-rw-r--r--   0 root         (0) root         (0)      878 2023-07-20 23:41:23.165276 trame-vtk-2.5.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-20 23:41:19.000000 trame-vtk-2.5.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 23:41:23.149276 trame-vtk-2.5.8/trame/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-07-20 23:41:19.000000 trame-vtk-2.5.8/trame/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 23:41:23.149276 trame-vtk-2.5.8/trame/modules/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-07-20 23:41:19.000000 trame-vtk-2.5.8/trame/modules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       39 2023-07-20 23:41:19.000000 trame-vtk-2.5.8/trame/modules/paraview.py
+-rw-r--r--   0 root         (0) root         (0)       39 2023-07-20 23:41:19.000000 trame-vtk-2.5.8/trame/modules/vtk.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 23:41:23.149276 trame-vtk-2.5.8/trame/tools/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-07-20 23:41:19.000000 trame-vtk-2.5.8/trame/tools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       83 2023-07-20 23:41:19.000000 trame-vtk-2.5.8/trame/tools/vtksz2html.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 23:41:23.153276 trame-vtk-2.5.8/trame/widgets/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-07-20 23:41:19.000000 trame-vtk-2.5.8/trame/widgets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      182 2023-07-20 23:41:19.000000 trame-vtk-2.5.8/trame/widgets/paraview.py
+-rw-r--r--   0 root         (0) root         (0)      172 2023-07-20 23:41:19.000000 trame-vtk-2.5.8/trame/widgets/vtk.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 23:41:23.153276 trame-vtk-2.5.8/trame_vtk/
+-rw-r--r--   0 root         (0) root         (0)     1504 2023-07-20 23:41:19.000000 trame-vtk-2.5.8/trame_vtk/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       91 2023-07-20 23:41:19.000000 trame-vtk-2.5.8/trame_vtk/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 23:41:23.153276 trame-vtk-2.5.8/trame_vtk/modules/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-20 23:41:19.000000 trame-vtk-2.5.8/trame_vtk/modules/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 23:41:23.153276 trame-vtk-2.5.8/trame_vtk/modules/common/
+-rw-r--r--   0 root         (0) root         (0)      354 2023-07-20 23:41:19.000000 trame-vtk-2.5.8/trame_vtk/modules/common/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 23:41:23.153276 trame-vtk-2.5.8/trame_vtk/modules/common/serve/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 23:41:19.000000 trame-vtk-2.5.8/trame_vtk/modules/common/serve/.gitignore
+-rw-r--r--   0 root         (0) root         (0)  1693968 2023-07-20 23:41:19.000000 trame-vtk-2.5.8/trame_vtk/modules/common/serve/trame-vtk.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 23:41:23.157276 trame-vtk-2.5.8/trame_vtk/modules/paraview/
+-rw-r--r--   0 root         (0) root         (0)     7896 2023-07-20 23:41:19.000000 trame-vtk-2.5.8/trame_vtk/modules/paraview/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      627 2023-07-20 23:41:19.000000 trame-vtk-2.5.8/trame_vtk/modules/paraview/core.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 23:41:23.157276 trame-vtk-2.5.8/trame_vtk/modules/paraview/protocols/
+-rw-r--r--   0 root         (0) root         (0)      363 2023-07-20 23:41:19.000000 trame-vtk-2.5.8/trame_vtk/modules/paraview/protocols/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5356 2023-07-20 23:41:19.000000 trame-vtk-2.5.8/trame_vtk/modules/paraview/protocols/local_rendering.py
+-rw-r--r--   0 root         (0) root         (0)     2233 2023-07-20 23:41:19.000000 trame-vtk-2.5.8/trame_vtk/modules/paraview/protocols/mouse_handler.py
+-rw-r--r--   0 root         (0) root         (0)    23952 2023-07-20 23:41:19.000000 trame-vtk-2.5.8/trame_vtk/modules/paraview/protocols/publish_image_delivery.py
+-rw-r--r--   0 root         (0) root         (0)     3565 2023-07-20 23:41:19.000000 trame-vtk-2.5.8/trame_vtk/modules/paraview/protocols/view_port.py
+-rw-r--r--   0 root         (0) root         (0)     4170 2023-07-20 23:41:19.000000 trame-vtk-2.5.8/trame_vtk/modules/paraview/protocols/web_protocol.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 23:41:23.157276 trame-vtk-2.5.8/trame_vtk/modules/vtk/
+-rw-r--r--   0 root         (0) root         (0)     7639 2023-07-20 23:41:19.000000 trame-vtk-2.5.8/trame_vtk/modules/vtk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2738 2023-07-20 23:41:19.000000 trame-vtk-2.5.8/trame_vtk/modules/vtk/core.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 23:41:23.157276 trame-vtk-2.5.8/trame_vtk/modules/vtk/protocols/
+-rw-r--r--   0 root         (0) root         (0)      322 2023-07-20 23:41:19.000000 trame-vtk-2.5.8/trame_vtk/modules/vtk/protocols/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5574 2023-07-20 23:41:19.000000 trame-vtk-2.5.8/trame_vtk/modules/vtk/protocols/local_rendering.py
+-rw-r--r--   0 root         (0) root         (0)     3981 2023-07-20 23:41:19.000000 trame-vtk-2.5.8/trame_vtk/modules/vtk/protocols/mouse_handler.py
+-rw-r--r--   0 root         (0) root         (0)    12797 2023-07-20 23:41:19.000000 trame-vtk-2.5.8/trame_vtk/modules/vtk/protocols/publish_image_delivery.py
+-rw-r--r--   0 root         (0) root         (0)     1973 2023-07-20 23:41:19.000000 trame-vtk-2.5.8/trame_vtk/modules/vtk/protocols/view_port.py
+-rw-r--r--   0 root         (0) root         (0)     1787 2023-07-20 23:41:19.000000 trame-vtk-2.5.8/trame_vtk/modules/vtk/protocols/web_protocol.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 23:41:23.161276 trame-vtk-2.5.8/trame_vtk/modules/vtk/serializers/
+-rw-r--r--   0 root         (0) root         (0)      726 2023-07-20 23:41:19.000000 trame-vtk-2.5.8/trame_vtk/modules/vtk/serializers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12646 2023-07-20 23:41:19.000000 trame-vtk-2.5.8/trame_vtk/modules/vtk/serializers/actors.py
+-rw-r--r--   0 root         (0) root         (0)      463 2023-07-20 23:41:19.000000 trame-vtk-2.5.8/trame_vtk/modules/vtk/serializers/cache.py
+-rw-r--r--   0 root         (0) root         (0)     6188 2023-07-20 23:41:19.000000 trame-vtk-2.5.8/trame_vtk/modules/vtk/serializers/data.py
+-rw-r--r--   0 root         (0) root         (0)      926 2023-07-20 23:41:19.000000 trame-vtk-2.5.8/trame_vtk/modules/vtk/serializers/export.py
+-rw-r--r--   0 root         (0) root         (0)     5785 2023-07-20 23:41:19.000000 trame-vtk-2.5.8/trame_vtk/modules/vtk/serializers/helpers.py
+-rw-r--r--   0 root         (0) root         (0)     4772 2023-07-20 23:41:19.000000 trame-vtk-2.5.8/trame_vtk/modules/vtk/serializers/initialize.py
+-rw-r--r--   0 root         (0) root         (0)     1528 2023-07-20 23:41:19.000000 trame-vtk-2.5.8/trame_vtk/modules/vtk/serializers/lights.py
+-rw-r--r--   0 root         (0) root         (0)     6059 2023-07-20 23:41:19.000000 trame-vtk-2.5.8/trame_vtk/modules/vtk/serializers/lookup_tables.py
+-rw-r--r--   0 root         (0) root         (0)     5436 2023-07-20 23:41:19.000000 trame-vtk-2.5.8/trame_vtk/modules/vtk/serializers/mappers.py
+-rw-r--r--   0 root         (0) root         (0)     6041 2023-07-20 23:41:19.000000 trame-vtk-2.5.8/trame_vtk/modules/vtk/serializers/mesh.py
+-rw-r--r--   0 root         (0) root         (0)     3471 2023-07-20 23:41:19.000000 trame-vtk-2.5.8/trame_vtk/modules/vtk/serializers/properties.py
+-rw-r--r--   0 root         (0) root         (0)      378 2023-07-20 23:41:19.000000 trame-vtk-2.5.8/trame_vtk/modules/vtk/serializers/registry.py
+-rw-r--r--   0 root         (0) root         (0)     4978 2023-07-20 23:41:19.000000 trame-vtk-2.5.8/trame_vtk/modules/vtk/serializers/render_windows.py
+-rw-r--r--   0 root         (0) root         (0)      914 2023-07-20 23:41:19.000000 trame-vtk-2.5.8/trame_vtk/modules/vtk/serializers/serialize.py
+-rw-r--r--   0 root         (0) root         (0)     3541 2023-07-20 23:41:19.000000 trame-vtk-2.5.8/trame_vtk/modules/vtk/serializers/synchronization_context.py
+-rw-r--r--   0 root         (0) root         (0)     1337 2023-07-20 23:41:19.000000 trame-vtk-2.5.8/trame_vtk/modules/vtk/serializers/textures.py
+-rw-r--r--   0 root         (0) root         (0)     1946 2023-07-20 23:41:19.000000 trame-vtk-2.5.8/trame_vtk/modules/vtk/serializers/utils.py
+-rw-r--r--   0 root         (0) root         (0)     1595 2023-07-20 23:41:19.000000 trame-vtk-2.5.8/trame_vtk/modules/vtk/serializers/widgets.py
+-rw-r--r--   0 root         (0) root         (0)     4551 2023-07-20 23:41:19.000000 trame-vtk-2.5.8/trame_vtk/modules/vtk/widget.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 23:41:23.161276 trame-vtk-2.5.8/trame_vtk/tools/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-20 23:41:19.000000 trame-vtk-2.5.8/trame_vtk/tools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   970597 2023-07-20 23:41:19.000000 trame-vtk-2.5.8/trame_vtk/tools/static_viewer.html
+-rw-r--r--   0 root         (0) root         (0)     1713 2023-07-20 23:41:19.000000 trame-vtk-2.5.8/trame_vtk/tools/vtksz2html.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 23:41:23.161276 trame-vtk-2.5.8/trame_vtk/widgets/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-20 23:41:19.000000 trame-vtk-2.5.8/trame_vtk/widgets/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 23:41:23.161276 trame-vtk-2.5.8/trame_vtk/widgets/vtk/
+-rw-r--r--   0 root         (0) root         (0)      645 2023-07-20 23:41:19.000000 trame-vtk-2.5.8/trame_vtk/widgets/vtk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    33204 2023-07-20 23:41:19.000000 trame-vtk-2.5.8/trame_vtk/widgets/vtk/common.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 23:41:23.153276 trame-vtk-2.5.8/trame_vtk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    12927 2023-07-20 23:41:23.000000 trame-vtk-2.5.8/trame_vtk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2481 2023-07-20 23:41:23.000000 trame-vtk-2.5.8/trame_vtk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 23:41:23.000000 trame-vtk-2.5.8/trame_vtk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-20 23:41:23.000000 trame-vtk-2.5.8/trame_vtk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-07-20 23:41:23.000000 trame-vtk-2.5.8/trame_vtk.egg-info/top_level.txt
```

### Comparing `trame-vtk-2.5.7/LICENSE` & `trame-vtk-2.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.5.7/PKG-INFO` & `trame-vtk-2.5.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trame-vtk
-Version: 2.5.7
+Version: 2.5.8
 Summary: VTK widgets for trame
 Author: Kitware Inc.
 License: BSD License
 Keywords: Python,Interactive,Web,Application,Framework
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `trame-vtk-2.5.7/README.rst` & `trame-vtk-2.5.8/README.rst`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.5.7/setup.cfg` & `trame-vtk-2.5.8/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = trame-vtk
-version = 2.5.7
+version = 2.5.8
 description = VTK widgets for trame
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 author = Kitware Inc.
 license = BSD License
 classifiers = 
 	Development Status :: 5 - Production/Stable
```

### Comparing `trame-vtk-2.5.7/trame_vtk/LICENSE` & `trame-vtk-2.5.8/trame_vtk/LICENSE`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.5.7/trame_vtk/modules/common/serve/trame-vtk.js` & `trame-vtk-2.5.8/trame_vtk/modules/common/serve/trame-vtk.js`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.5.7/trame_vtk/modules/paraview/__init__.py` & `trame-vtk-2.5.8/trame_vtk/modules/paraview/__init__.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.5.7/trame_vtk/modules/paraview/core.py` & `trame-vtk-2.5.8/trame_vtk/modules/paraview/core.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.5.7/trame_vtk/modules/paraview/protocols/local_rendering.py` & `trame-vtk-2.5.8/trame_vtk/modules/paraview/protocols/local_rendering.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.5.7/trame_vtk/modules/paraview/protocols/mouse_handler.py` & `trame-vtk-2.5.8/trame_vtk/modules/paraview/protocols/mouse_handler.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.5.7/trame_vtk/modules/paraview/protocols/publish_image_delivery.py` & `trame-vtk-2.5.8/trame_vtk/modules/paraview/protocols/publish_image_delivery.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.5.7/trame_vtk/modules/paraview/protocols/view_port.py` & `trame-vtk-2.5.8/trame_vtk/modules/paraview/protocols/view_port.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.5.7/trame_vtk/modules/paraview/protocols/web_protocol.py` & `trame-vtk-2.5.8/trame_vtk/modules/paraview/protocols/web_protocol.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.5.7/trame_vtk/modules/vtk/__init__.py` & `trame-vtk-2.5.8/trame_vtk/modules/vtk/__init__.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.5.7/trame_vtk/modules/vtk/core.py` & `trame-vtk-2.5.8/trame_vtk/modules/vtk/core.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.5.7/trame_vtk/modules/vtk/protocols/local_rendering.py` & `trame-vtk-2.5.8/trame_vtk/modules/vtk/protocols/local_rendering.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.5.7/trame_vtk/modules/vtk/protocols/mouse_handler.py` & `trame-vtk-2.5.8/trame_vtk/modules/vtk/protocols/mouse_handler.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.5.7/trame_vtk/modules/vtk/protocols/publish_image_delivery.py` & `trame-vtk-2.5.8/trame_vtk/modules/vtk/protocols/publish_image_delivery.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.5.7/trame_vtk/modules/vtk/protocols/view_port.py` & `trame-vtk-2.5.8/trame_vtk/modules/vtk/protocols/view_port.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.5.7/trame_vtk/modules/vtk/protocols/web_protocol.py` & `trame-vtk-2.5.8/trame_vtk/modules/vtk/protocols/web_protocol.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.5.7/trame_vtk/modules/vtk/serializers/__init__.py` & `trame-vtk-2.5.8/trame_vtk/modules/vtk/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.5.7/trame_vtk/modules/vtk/serializers/actors.py` & `trame-vtk-2.5.8/trame_vtk/modules/vtk/serializers/actors.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.5.7/trame_vtk/modules/vtk/serializers/data.py` & `trame-vtk-2.5.8/trame_vtk/modules/vtk/serializers/data.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.5.7/trame_vtk/modules/vtk/serializers/export.py` & `trame-vtk-2.5.8/trame_vtk/modules/vtk/serializers/export.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.5.7/trame_vtk/modules/vtk/serializers/helpers.py` & `trame-vtk-2.5.8/trame_vtk/modules/vtk/serializers/helpers.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.5.7/trame_vtk/modules/vtk/serializers/initialize.py` & `trame-vtk-2.5.8/trame_vtk/modules/vtk/serializers/initialize.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.5.7/trame_vtk/modules/vtk/serializers/lights.py` & `trame-vtk-2.5.8/trame_vtk/modules/vtk/serializers/lights.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.5.7/trame_vtk/modules/vtk/serializers/lookup_tables.py` & `trame-vtk-2.5.8/trame_vtk/modules/vtk/serializers/lookup_tables.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.5.7/trame_vtk/modules/vtk/serializers/mappers.py` & `trame-vtk-2.5.8/trame_vtk/modules/vtk/serializers/mappers.py`

 * *Files 0% similar despite different names*

```diff
@@ -134,15 +134,15 @@
             "id": mapper_id,
             "type": class_name(mapper),
             "properties": cache_properties(
                 mapper_id,
                 context,
                 {
                     # VolumeMapper
-                    "sampleDistance": mapper.GetSampleDistance(),
+                    "sampleDistance": abs(mapper.GetSampleDistance()),
                     "imageSampleDistance": image_sample_distance,
                     # "maximumSamplesPerRay": mapper.GetMaximumSamplesPerRay(),
                     "autoAdjustSampleDistances": mapper.GetAutoAdjustSampleDistances(),
                     "blendMode": mapper.GetBlendMode(),
                     # "ipScalarRange": mapper.GetIpScalarRange(),
                     # "filterMode": mapper.GetFilterMode(),
                     # "preferSizeOverAccuracy": mapper.Get(),
```

### Comparing `trame-vtk-2.5.7/trame_vtk/modules/vtk/serializers/mesh.py` & `trame-vtk-2.5.8/trame_vtk/modules/vtk/serializers/mesh.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.5.7/trame_vtk/modules/vtk/serializers/properties.py` & `trame-vtk-2.5.8/trame_vtk/modules/vtk/serializers/properties.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.5.7/trame_vtk/modules/vtk/serializers/render_windows.py` & `trame-vtk-2.5.8/trame_vtk/modules/vtk/serializers/render_windows.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.5.7/trame_vtk/modules/vtk/serializers/serialize.py` & `trame-vtk-2.5.8/trame_vtk/modules/vtk/serializers/serialize.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.5.7/trame_vtk/modules/vtk/serializers/synchronization_context.py` & `trame-vtk-2.5.8/trame_vtk/modules/vtk/serializers/synchronization_context.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.5.7/trame_vtk/modules/vtk/serializers/textures.py` & `trame-vtk-2.5.8/trame_vtk/modules/vtk/serializers/textures.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.5.7/trame_vtk/modules/vtk/serializers/utils.py` & `trame-vtk-2.5.8/trame_vtk/modules/vtk/serializers/utils.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.5.7/trame_vtk/modules/vtk/serializers/widgets.py` & `trame-vtk-2.5.8/trame_vtk/modules/vtk/serializers/widgets.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.5.7/trame_vtk/modules/vtk/widget.py` & `trame-vtk-2.5.8/trame_vtk/modules/vtk/widget.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.5.7/trame_vtk/tools/static_viewer.html` & `trame-vtk-2.5.8/trame_vtk/tools/static_viewer.html`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.5.7/trame_vtk/tools/vtksz2html.py` & `trame-vtk-2.5.8/trame_vtk/tools/vtksz2html.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.5.7/trame_vtk/widgets/vtk/__init__.py` & `trame-vtk-2.5.8/trame_vtk/widgets/vtk/__init__.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.5.7/trame_vtk/widgets/vtk/common.py` & `trame-vtk-2.5.8/trame_vtk/widgets/vtk/common.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.5.7/trame_vtk.egg-info/PKG-INFO` & `trame-vtk-2.5.8/trame_vtk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trame-vtk
-Version: 2.5.7
+Version: 2.5.8
 Summary: VTK widgets for trame
 Author: Kitware Inc.
 License: BSD License
 Keywords: Python,Interactive,Web,Application,Framework
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `trame-vtk-2.5.7/trame_vtk.egg-info/SOURCES.txt` & `trame-vtk-2.5.8/trame_vtk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

