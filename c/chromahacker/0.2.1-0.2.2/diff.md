# Comparing `tmp/chromahacker-0.2.1.tar.gz` & `tmp/chromahacker-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chromahacker-0.2.1.tar", max compression
+gzip compressed data, was "chromahacker-0.2.2.tar", max compression
```

## Comparing `chromahacker-0.2.1.tar` & `chromahacker-0.2.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        0 2023-06-06 19:05:27.092423 chromahacker-0.2.1/README.md
--rw-r--r--   0        0        0     6148 2023-06-06 20:17:27.539807 chromahacker-0.2.1/chromahacker/.DS_Store
--rw-r--r--   0        0        0       89 2023-06-08 16:47:40.434230 chromahacker-0.2.1/chromahacker/__init__.py
--rw-r--r--   0        0        0     6621 2023-06-09 00:51:51.371973 chromahacker-0.2.1/chromahacker/color_input.py
--rw-r--r--   0        0        0      419 2023-06-14 21:19:09.134682 chromahacker-0.2.1/chromahacker/palettize.py
--rw-r--r--   0        0        0      266 2023-06-09 00:21:03.357804 chromahacker-0.2.1/chromahacker/process_image.py
--rw-r--r--   0        0        0      424 2023-06-08 17:20:05.944611 chromahacker-0.2.1/chromahacker/spline.py
--rw-r--r--   0        0        0      337 2023-06-14 21:19:50.220847 chromahacker-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      473 1970-01-01 00:00:00.000000 chromahacker-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-06 19:05:27.000000 chromahacker-0.2.2/README.md
+-rw-r--r--   0        0        0     6148 2023-06-06 20:17:27.000000 chromahacker-0.2.2/chromahacker/.DS_Store
+-rw-r--r--   0        0        0       89 2023-06-08 16:47:40.000000 chromahacker-0.2.2/chromahacker/__init__.py
+-rw-r--r--   0        0        0     6621 2023-06-09 00:51:51.000000 chromahacker-0.2.2/chromahacker/color_input.py
+-rw-r--r--   0        0        0      554 2023-07-21 16:55:54.955424 chromahacker-0.2.2/chromahacker/palettize.py
+-rw-r--r--   0        0        0      266 2023-06-09 00:21:03.000000 chromahacker-0.2.2/chromahacker/process_image.py
+-rw-r--r--   0        0        0      469 2023-07-21 16:56:05.933097 chromahacker-0.2.2/chromahacker/spline.py
+-rw-r--r--   0        0        0      337 2023-07-21 17:09:51.067125 chromahacker-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      473 1970-01-01 00:00:00.000000 chromahacker-0.2.2/PKG-INFO
```

### Comparing `chromahacker-0.2.1/chromahacker/.DS_Store` & `chromahacker-0.2.2/chromahacker/.DS_Store`

 * *Files identical despite different names*

### Comparing `chromahacker-0.2.1/chromahacker/color_input.py` & `chromahacker-0.2.2/chromahacker/color_input.py`

 * *Files identical despite different names*

