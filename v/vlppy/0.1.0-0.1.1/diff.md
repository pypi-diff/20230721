# Comparing `tmp/vlppy-0.1.0.tar.gz` & `tmp/vlppy-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\SoftwareData\VSCode\Python\python_study\pyvlp0.1\dist\.tmp-bmnpw82f\vlppy-0.1.0.tar", last modified: Sun Jun  4 07:34:50 2023, max compression
+gzip compressed data, was "D:\SoftwareData\VSCode\Python\python_study\vlppy0.1\dist\.tmp-th58gco9\vlppy-0.1.1.tar", last modified: Fri Jul 21 08:07:37 2023, max compression
```

## Comparing `vlppy-0.1.0.tar` & `vlppy-0.1.1.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxrwxrwx   0        0        0        0 2023-06-04 07:34:50.684106 vlppy-0.1.0/
--rw-rw-rw-   0        0        0     1091 2022-09-12 09:03:59.000000 vlppy-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      294 2023-06-04 07:31:04.000000 vlppy-0.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2666 2023-06-04 07:34:50.683145 vlppy-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      840 2023-06-04 07:30:42.000000 vlppy-0.1.0/README.md
--rw-rw-rw-   0        0        0      629 2023-06-04 07:30:50.000000 vlppy-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-04 07:34:50.684106 vlppy-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      926 2023-06-04 07:34:26.000000 vlppy-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-04 07:34:50.508937 vlppy-0.1.0/vlppy/
-drwxrwxrwx   0        0        0        0 2023-06-04 07:34:50.528935 vlppy-0.1.0/vlppy/.vscode/
--rw-rw-rw-   0        0        0      478 2022-11-24 08:46:45.000000 vlppy-0.1.0/vlppy/.vscode/settings.json
--rw-rw-rw-   0        0        0     1093 2022-09-23 02:30:35.000000 vlppy-0.1.0/vlppy/LICENSE.txt
--rw-rw-rw-   0        0        0      271 2023-04-18 03:27:13.000000 vlppy-0.1.0/vlppy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-04 07:34:50.546956 vlppy-0.1.0/vlppy/demo/
--rw-rw-rw-   0        0        0      345 2023-06-04 07:33:39.000000 vlppy-0.1.0/vlppy/demo/README.md
--rw-rw-rw-   0        0        0       88 2023-01-09 07:00:52.000000 vlppy-0.1.0/vlppy/demo/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-04 07:34:50.559928 vlppy-0.1.0/vlppy/demo/__pycache__/
--rw-rw-rw-   0        0        0      234 2022-09-15 01:51:51.000000 vlppy-0.1.0/vlppy/demo/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0     1938 2022-09-15 01:51:51.000000 vlppy-0.1.0/vlppy/demo/__pycache__/demo_main.cpython-39.pyc
--rw-rw-rw-   0        0        0     2913 2022-09-15 01:51:51.000000 vlppy-0.1.0/vlppy/demo/__pycache__/vlp_model.cpython-39.pyc
--rw-rw-rw-   0        0        0     1342 2023-04-27 10:40:52.000000 vlppy-0.1.0/vlppy/demo/demo_filter.py
--rw-rw-rw-   0        0        0     2607 2023-04-19 03:46:42.000000 vlppy-0.1.0/vlppy/demo/demo_main.py
--rw-rw-rw-   0        0        0     2950 2023-05-16 06:59:59.000000 vlppy-0.1.0/vlppy/demo/vlp_model.py
-drwxrwxrwx   0        0        0        0 2023-06-04 07:34:50.564961 vlppy-0.1.0/vlppy/error/
--rw-rw-rw-   0        0        0       26 2022-11-08 07:31:14.000000 vlppy-0.1.0/vlppy/error/__init__.py
--rw-rw-rw-   0        0        0     1619 2023-04-20 05:53:48.000000 vlppy-0.1.0/vlppy/error/error.py
--rw-rw-rw-   0        0        0      122 2023-06-04 07:32:48.000000 vlppy-0.1.0/vlppy/info.py
-drwxrwxrwx   0        0        0        0 2023-06-04 07:34:50.572944 vlppy-0.1.0/vlppy/io/
--rw-rw-rw-   0        0        0       26 2022-09-02 10:32:14.000000 vlppy-0.1.0/vlppy/io/__init__.py
--rw-rw-rw-   0        0        0     5346 2023-04-20 06:14:59.000000 vlppy-0.1.0/vlppy/io/io.py
-drwxrwxrwx   0        0        0        0 2023-06-04 07:34:50.584930 vlppy-0.1.0/vlppy/model/
--rw-rw-rw-   0        0        0       66 2022-09-19 01:30:24.000000 vlppy-0.1.0/vlppy/model/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-04 07:34:50.608990 vlppy-0.1.0/vlppy/model/__pycache__/
--rw-rw-rw-   0        0        0      282 2022-09-15 01:51:49.000000 vlppy-0.1.0/vlppy/model/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0    11287 2022-09-15 01:51:49.000000 vlppy-0.1.0/vlppy/model/__pycache__/filter.cpython-39.pyc
--rw-rw-rw-   0        0        0     4494 2022-09-15 01:51:50.000000 vlppy-0.1.0/vlppy/model/__pycache__/led.cpython-39.pyc
--rw-rw-rw-   0        0        0     9730 2022-09-15 01:51:50.000000 vlppy-0.1.0/vlppy/model/__pycache__/pd.cpython-39.pyc
--rw-rw-rw-   0        0        0     9684 2022-09-15 01:51:50.000000 vlppy-0.1.0/vlppy/model/__pycache__/room.cpython-39.pyc
--rw-rw-rw-   0        0        0     6303 2023-05-16 07:19:55.000000 vlppy-0.1.0/vlppy/model/led.py
--rw-rw-rw-   0        0        0    18237 2023-05-22 02:50:09.000000 vlppy-0.1.0/vlppy/model/pd.py
--rw-rw-rw-   0        0        0    17966 2023-06-01 06:04:36.000000 vlppy-0.1.0/vlppy/model/room.py
-drwxrwxrwx   0        0        0        0 2023-06-04 07:34:50.616927 vlppy-0.1.0/vlppy/setting/
--rw-rw-rw-   0        0        0       40 2022-05-31 05:29:34.000000 vlppy-0.1.0/vlppy/setting/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-04 07:34:50.629930 vlppy-0.1.0/vlppy/setting/__pycache__/
--rw-rw-rw-   0        0        0      196 2022-05-31 05:35:37.000000 vlppy-0.1.0/vlppy/setting/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0     2526 2022-09-15 01:51:51.000000 vlppy-0.1.0/vlppy/setting/__pycache__/json_setting.cpython-39.pyc
--rw-rw-rw-   0        0        0     2903 2023-04-20 06:15:26.000000 vlppy-0.1.0/vlppy/setting/json_setting.py
--rw-rw-rw-   0        0        0     2208 2022-12-08 07:54:09.000000 vlppy-0.1.0/vlppy/setting/settings.json
-drwxrwxrwx   0        0        0        0 2023-06-04 07:34:50.661107 vlppy-0.1.0/vlppy/signal/
--rw-rw-rw-   0        0        0       48 2023-01-09 06:55:15.000000 vlppy-0.1.0/vlppy/signal/__init__.py
--rw-rw-rw-   0        0        0    10010 2023-04-20 06:24:52.000000 vlppy-0.1.0/vlppy/signal/filter.py
--rw-rw-rw-   0        0        0     3719 2023-04-27 10:42:14.000000 vlppy-0.1.0/vlppy/signal/plot.py
-drwxrwxrwx   0        0        0        0 2023-06-04 07:34:50.675109 vlppy-0.1.0/vlppy/tools/
--rw-rw-rw-   0        0        0       26 2023-04-18 03:21:34.000000 vlppy-0.1.0/vlppy/tools/__init__.py
--rw-rw-rw-   0        0        0      273 2023-04-18 03:22:02.000000 vlppy-0.1.0/vlppy/tools/decorator.py
-drwxrwxrwx   0        0        0        0 2023-06-04 07:34:50.680108 vlppy-0.1.0/vlppy/vis/
--rw-rw-rw-   0        0        0       26 2022-06-07 05:02:10.000000 vlppy-0.1.0/vlppy/vis/__init__.py
--rw-rw-rw-   0        0        0     3653 2023-04-19 02:52:08.000000 vlppy-0.1.0/vlppy/vis/vis.py
-drwxrwxrwx   0        0        0        0 2023-06-04 07:34:50.525933 vlppy-0.1.0/vlppy.egg-info/
--rw-rw-rw-   0        0        0     2666 2023-06-04 07:34:50.000000 vlppy-0.1.0/vlppy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1266 2023-06-04 07:34:50.000000 vlppy-0.1.0/vlppy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-04 07:34:50.000000 vlppy-0.1.0/vlppy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-06-04 07:34:50.000000 vlppy-0.1.0/vlppy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-04 07:34:50.000000 vlppy-0.1.0/vlppy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-21 08:07:37.297603 vlppy-0.1.1/
+-rw-rw-rw-   0        0        0     1091 2022-09-12 09:03:59.000000 vlppy-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      294 2023-06-04 07:31:04.000000 vlppy-0.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2666 2023-07-21 08:07:37.293445 vlppy-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      840 2023-07-21 08:05:09.000000 vlppy-0.1.1/README.md
+-rw-rw-rw-   0        0        0      629 2023-07-21 08:04:59.000000 vlppy-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-21 08:07:37.298603 vlppy-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      926 2023-07-21 08:05:48.000000 vlppy-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 08:07:37.110365 vlppy-0.1.1/vlppy/
+drwxrwxrwx   0        0        0        0 2023-07-21 08:07:37.128368 vlppy-0.1.1/vlppy/.vscode/
+-rw-rw-rw-   0        0        0      478 2022-11-24 08:46:45.000000 vlppy-0.1.1/vlppy/.vscode/settings.json
+-rw-rw-rw-   0        0        0     1093 2022-09-23 02:30:35.000000 vlppy-0.1.1/vlppy/LICENSE.txt
+-rw-rw-rw-   0        0        0      271 2023-04-18 03:27:13.000000 vlppy-0.1.1/vlppy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 08:07:37.147379 vlppy-0.1.1/vlppy/demo/
+-rw-rw-rw-   0        0        0      345 2023-06-04 07:33:39.000000 vlppy-0.1.1/vlppy/demo/README.md
+-rw-rw-rw-   0        0        0       88 2023-01-09 07:00:52.000000 vlppy-0.1.1/vlppy/demo/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 08:07:37.161376 vlppy-0.1.1/vlppy/demo/__pycache__/
+-rw-rw-rw-   0        0        0      234 2022-09-15 01:51:51.000000 vlppy-0.1.1/vlppy/demo/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1938 2022-09-15 01:51:51.000000 vlppy-0.1.1/vlppy/demo/__pycache__/demo_main.cpython-39.pyc
+-rw-rw-rw-   0        0        0     2913 2022-09-15 01:51:51.000000 vlppy-0.1.1/vlppy/demo/__pycache__/vlp_model.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1342 2023-04-27 10:40:52.000000 vlppy-0.1.1/vlppy/demo/demo_filter.py
+-rw-rw-rw-   0        0        0     2607 2023-04-19 03:46:42.000000 vlppy-0.1.1/vlppy/demo/demo_main.py
+-rw-rw-rw-   0        0        0     2965 2023-07-20 13:25:54.000000 vlppy-0.1.1/vlppy/demo/vlp_model.py
+drwxrwxrwx   0        0        0        0 2023-07-21 08:07:37.170365 vlppy-0.1.1/vlppy/error/
+-rw-rw-rw-   0        0        0       26 2022-11-08 07:31:14.000000 vlppy-0.1.1/vlppy/error/__init__.py
+-rw-rw-rw-   0        0        0     1619 2023-04-20 05:53:48.000000 vlppy-0.1.1/vlppy/error/error.py
+-rw-rw-rw-   0        0        0      120 2023-07-21 08:04:46.000000 vlppy-0.1.1/vlppy/info.py
+drwxrwxrwx   0        0        0        0 2023-07-21 08:07:37.180366 vlppy-0.1.1/vlppy/io/
+-rw-rw-rw-   0        0        0       26 2022-09-02 10:32:14.000000 vlppy-0.1.1/vlppy/io/__init__.py
+-rw-rw-rw-   0        0        0     5346 2023-04-20 06:14:59.000000 vlppy-0.1.1/vlppy/io/io.py
+drwxrwxrwx   0        0        0        0 2023-07-21 08:07:37.199405 vlppy-0.1.1/vlppy/model/
+-rw-rw-rw-   0        0        0       66 2022-09-19 01:30:24.000000 vlppy-0.1.1/vlppy/model/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 08:07:37.220366 vlppy-0.1.1/vlppy/model/__pycache__/
+-rw-rw-rw-   0        0        0      282 2022-09-15 01:51:49.000000 vlppy-0.1.1/vlppy/model/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0    11287 2022-09-15 01:51:49.000000 vlppy-0.1.1/vlppy/model/__pycache__/filter.cpython-39.pyc
+-rw-rw-rw-   0        0        0     4494 2022-09-15 01:51:50.000000 vlppy-0.1.1/vlppy/model/__pycache__/led.cpython-39.pyc
+-rw-rw-rw-   0        0        0     9730 2022-09-15 01:51:50.000000 vlppy-0.1.1/vlppy/model/__pycache__/pd.cpython-39.pyc
+-rw-rw-rw-   0        0        0     9684 2022-09-15 01:51:50.000000 vlppy-0.1.1/vlppy/model/__pycache__/room.cpython-39.pyc
+-rw-rw-rw-   0        0        0     6303 2023-05-16 07:19:55.000000 vlppy-0.1.1/vlppy/model/led.py
+-rw-rw-rw-   0        0        0    18237 2023-05-22 02:50:09.000000 vlppy-0.1.1/vlppy/model/pd.py
+-rw-rw-rw-   0        0        0    18074 2023-07-21 08:00:38.000000 vlppy-0.1.1/vlppy/model/room.py
+drwxrwxrwx   0        0        0        0 2023-07-21 08:07:37.233365 vlppy-0.1.1/vlppy/setting/
+-rw-rw-rw-   0        0        0       40 2022-05-31 05:29:34.000000 vlppy-0.1.1/vlppy/setting/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 08:07:37.244378 vlppy-0.1.1/vlppy/setting/__pycache__/
+-rw-rw-rw-   0        0        0      196 2022-05-31 05:35:37.000000 vlppy-0.1.1/vlppy/setting/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0     2526 2022-09-15 01:51:51.000000 vlppy-0.1.1/vlppy/setting/__pycache__/json_setting.cpython-39.pyc
+-rw-rw-rw-   0        0        0     2903 2023-04-20 06:15:26.000000 vlppy-0.1.1/vlppy/setting/json_setting.py
+-rw-rw-rw-   0        0        0     2208 2022-12-08 07:54:09.000000 vlppy-0.1.1/vlppy/setting/settings.json
+drwxrwxrwx   0        0        0        0 2023-07-21 08:07:37.274363 vlppy-0.1.1/vlppy/signal/
+-rw-rw-rw-   0        0        0       48 2023-01-09 06:55:15.000000 vlppy-0.1.1/vlppy/signal/__init__.py
+-rw-rw-rw-   0        0        0    10010 2023-04-20 06:24:52.000000 vlppy-0.1.1/vlppy/signal/filter.py
+-rw-rw-rw-   0        0        0     3719 2023-04-27 10:42:14.000000 vlppy-0.1.1/vlppy/signal/plot.py
+drwxrwxrwx   0        0        0        0 2023-07-21 08:07:37.280377 vlppy-0.1.1/vlppy/tools/
+-rw-rw-rw-   0        0        0       26 2023-04-18 03:21:34.000000 vlppy-0.1.1/vlppy/tools/__init__.py
+-rw-rw-rw-   0        0        0      273 2023-04-18 03:22:02.000000 vlppy-0.1.1/vlppy/tools/decorator.py
+drwxrwxrwx   0        0        0        0 2023-07-21 08:07:37.291379 vlppy-0.1.1/vlppy/vis/
+-rw-rw-rw-   0        0        0       26 2022-06-07 05:02:10.000000 vlppy-0.1.1/vlppy/vis/__init__.py
+-rw-rw-rw-   0        0        0     3653 2023-04-19 02:52:08.000000 vlppy-0.1.1/vlppy/vis/vis.py
+drwxrwxrwx   0        0        0        0 2023-07-21 08:07:37.125362 vlppy-0.1.1/vlppy.egg-info/
+-rw-rw-rw-   0        0        0     2666 2023-07-21 08:07:36.000000 vlppy-0.1.1/vlppy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1266 2023-07-21 08:07:36.000000 vlppy-0.1.1/vlppy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 08:07:36.000000 vlppy-0.1.1/vlppy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-07-21 08:07:36.000000 vlppy-0.1.1/vlppy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-21 08:07:36.000000 vlppy-0.1.1/vlppy.egg-info/top_level.txt
```

### Comparing `vlppy-0.1.0/LICENSE` & `vlppy-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vlppy-0.1.0/PKG-INFO` & `vlppy-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vlppy
-Version: 0.1.0
+Version: 0.1.1
 Summary: Construction of visible light positioning model
 Home-page: https://gitee.com/yangwuju/vlppy
 Author: yangwuju
 Author-email: yangwuju <1424134319@qq.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -58,12 +58,12 @@
 
 ```
 py -m pip install vlppy
 ```
 
 @updata log
 
-静态定位（version=0.1.x）；
+静态定位（version=0.1.1）；
 
 将测试平面更新为测试空间区域，可以实现3d定位仿真;
 
 优化部分代码；
```

### Comparing `vlppy-0.1.0/README.md` & `vlppy-0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -23,12 +23,12 @@
 
 ```
 py -m pip install vlppy
 ```
 
 @updata log
 
-静态定位（version=0.1.x）；
+静态定位（version=0.1.1）；
 
 将测试平面更新为测试空间区域，可以实现3d定位仿真;
 
 优化部分代码；
```

### Comparing `vlppy-0.1.0/pyproject.toml` & `vlppy-0.1.1/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "vlppy"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="yangwuju", email="1424134319@qq.com" },
 ]
 description = "Construction of visible light positioning model"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.5"
```

### Comparing `vlppy-0.1.0/setup.py` & `vlppy-0.1.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 path = os.path.join(CUR_PATH, 'build')
 if os.path.isdir(path):
     print('INFO del dir ', path) 
     shutil.rmtree(path)
 
 setup(
     name = 'vlppy', #应用名
-    version = '0.1.0',  #版本号
+    version = '0.1.1',  #版本号
     description = 'Construction of visible light positioning model', 
     packages = find_packages(),  #包括在安装包内的Python包
     include_package_data = True, #启用清单文件MANIFEST.in,包含数据文件
     # exclude_package_data = {'docs':['1.txt']},  #排除文件
     install_requires = [#自动安装依赖
         'numpy>=1.19.0',
         'matplotlib>=3.5.0',
```

### Comparing `vlppy-0.1.0/vlppy/LICENSE.txt` & `vlppy-0.1.1/vlppy/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vlppy-0.1.0/vlppy/demo/__pycache__/demo_main.cpython-39.pyc` & `vlppy-0.1.1/vlppy/demo/__pycache__/demo_main.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `vlppy-0.1.0/vlppy/demo/__pycache__/vlp_model.cpython-39.pyc` & `vlppy-0.1.1/vlppy/demo/__pycache__/vlp_model.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `vlppy-0.1.0/vlppy/demo/demo_filter.py` & `vlppy-0.1.1/vlppy/demo/demo_filter.py`

 * *Files identical despite different names*

### Comparing `vlppy-0.1.0/vlppy/demo/demo_main.py` & `vlppy-0.1.1/vlppy/demo/demo_main.py`

 * *Files identical despite different names*

### Comparing `vlppy-0.1.0/vlppy/demo/vlp_model.py` & `vlppy-0.1.1/vlppy/demo/vlp_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,18 +13,18 @@
         # PD
         pd = kwargs["PD_Info"] 
         pd1 = pd["PD1"]   
         pd2 = pd["PD2"]   
         pd3 = pd["PD3"]   
         pd4 = pd["PD4"]   
         
-        pd1_pos, pd1_Nv = PD.recv_frame_model(l=pd["l"], alpha=pd1["alpha"], beta=pd1["beta"], center_tp_pos=self.room.tp_pos)  # PD位置和倾斜角
-        pd2_pos, pd2_Nv = PD.recv_frame_model(l=pd["l"], alpha=pd2["alpha"], beta=pd2["beta"], center_tp_pos=self.room.tp_pos) 
-        pd3_pos, pd3_Nv = PD.recv_frame_model(l=pd["l"], alpha=pd3["alpha"], beta=pd3["beta"], center_tp_pos=self.room.tp_pos)  
-        pd4_pos, pd4_Nv = PD.recv_frame_model(l=pd["l"], alpha=pd4["alpha"], beta=pd4["beta"], center_tp_pos=self.room.tp_pos) 
+        pd1_pos, pd1_Nv = PD.recv_frame_model(l=pd["l"], alpha=pd1["alpha"], beta=pd1["beta"], center_tp_pos=self.room.tp_pos())  # PD位置和倾斜角
+        pd2_pos, pd2_Nv = PD.recv_frame_model(l=pd["l"], alpha=pd2["alpha"], beta=pd2["beta"], center_tp_pos=self.room.tp_pos()) 
+        pd3_pos, pd3_Nv = PD.recv_frame_model(l=pd["l"], alpha=pd3["alpha"], beta=pd3["beta"], center_tp_pos=self.room.tp_pos())  
+        pd4_pos, pd4_Nv = PD.recv_frame_model(l=pd["l"], alpha=pd4["alpha"], beta=pd4["beta"], center_tp_pos=self.room.tp_pos()) 
         
         self.pd1 = PD(n=pd["n"], fov=pd["fov"], Ar=pd["Ar"], Ts=pd["Ts"], pos=pd1_pos, Nv=pd1_Nv) 
         self.pd2 = PD(n=pd["n"], fov=pd["fov"], Ar=pd["Ar"], Ts=pd["Ts"], pos=pd2_pos, Nv=pd2_Nv)
         self.pd3 = PD(n=pd["n"], fov=pd["fov"], Ar=pd["Ar"], Ts=pd["Ts"], pos=pd3_pos, Nv=pd3_Nv) 
         self.pd4 = PD(n=pd["n"], fov=pd["fov"], Ar=pd["Ar"], Ts=pd["Ts"], pos=pd4_pos, Nv=pd4_Nv) 
         
         # LED
@@ -43,23 +43,23 @@
         # PD接收各LED的信号 (l*w*h)
         P_PD1 = self.pd1.recv_led_signal(led=self.led1, room=self.room) 
         P_PD2 = self.pd2.recv_led_signal(led=self.led1, room=self.room)
         P_PD3 = self.pd3.recv_led_signal(led=self.led1, room=self.room) 
         P_PD4 = self.pd4.recv_led_signal(led=self.led1, room=self.room) 
 
         # 参考点
-        Xr, Yr, Zr = self.room.tp_raw_pos  #（l*w*h）
+        Xr, Yr, Zr = self.room.tp_pos(fmt='c')  #（l*w*h）
         
         return (P_PD1,P_PD2,P_PD3,P_PD4,Xr,Yr,Zr)  
       
     def show(self,z,savepath=...,showfig=True):
         """绘图
         z: 第三维度数据
         """
-        xr, yr, _ = self.room.tp_grid
+        xr, yr, _ = self.room.tp_grid()
         z = np.reshape(z, xr.shape)  
         ax = plt.axes(projection='3d')
         ax.plot_surface(xr, yr, z, cmap='viridis', edgecolor='none')
         ax.set_xlabel('X')
         ax.set_ylabel('Y')
         ax.set_zlabel('Z')
         if savepath != ...:
```

### Comparing `vlppy-0.1.0/vlppy/error/error.py` & `vlppy-0.1.1/vlppy/error/error.py`

 * *Files identical despite different names*

### Comparing `vlppy-0.1.0/vlppy/io/io.py` & `vlppy-0.1.1/vlppy/io/io.py`

 * *Files identical despite different names*

### Comparing `vlppy-0.1.0/vlppy/model/__pycache__/filter.cpython-39.pyc` & `vlppy-0.1.1/vlppy/model/__pycache__/filter.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `vlppy-0.1.0/vlppy/model/__pycache__/led.cpython-39.pyc` & `vlppy-0.1.1/vlppy/model/__pycache__/led.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `vlppy-0.1.0/vlppy/model/__pycache__/pd.cpython-39.pyc` & `vlppy-0.1.1/vlppy/model/__pycache__/pd.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `vlppy-0.1.0/vlppy/model/__pycache__/room.cpython-39.pyc` & `vlppy-0.1.1/vlppy/model/__pycache__/room.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `vlppy-0.1.0/vlppy/model/led.py` & `vlppy-0.1.1/vlppy/model/led.py`

 * *Files identical despite different names*

### Comparing `vlppy-0.1.0/vlppy/model/pd.py` & `vlppy-0.1.1/vlppy/model/pd.py`

 * *Files identical despite different names*

### Comparing `vlppy-0.1.0/vlppy/model/room.py` & `vlppy-0.1.1/vlppy/model/room.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,14 +44,43 @@
         self.rho = rho #墙壁反射率
         
         self.rp_height = [0, height]   # 前后左右反射墙壁高度范围
 
         self.origin = (0,0,0) #原点位置
         self.wall_args_path = f"wall_args.xlsx" # 默认墙壁参数地址
 
+    def get_tp_grid(self):
+        """获取测试点位置的网格矩阵(所有测试点的相对位置)
+        """
+        (xo, yo, zo) = self._origin #原点位置
+
+        gx, gy, gz = self.tp_gap # 测试区域划分网格的间隔
+        tp_h1, tp_h2 = self.tp_height # 测试区域高度
+        x = np.arange(0, self.length+1e-3, gx) # 房间长度等间隔划分的数组
+        y = np.arange(0, self.width+1e-3, gy)  # 房间宽度等间隔划分的数组
+        z = np.arange(tp_h1, tp_h2+1e-3, gz)   # 测试平面高度等间隔划分的数组
+        xr, yr, zr = np.meshgrid(xo+x, yo+y, zo+z, indexing='ij') # 返回二维网格矩阵（测试点的相对位置）
+        return (xr.squeeze(), yr.squeeze(), zr.squeeze()) #（l,w,h）
+
+    def get_tp_pos(self, fmt='r'):
+        """获取测试点位置
+        fmt: 输出测试点坐标格式
+            fmt='r': pos.shape=(n,3)
+            fmt='c': pos.shape=(3,n)
+        """
+        if not fmt in ('r','c'):
+            raise VLPValueError(fmt,'r','c')
+        xr, yr, zr = self.get_tp_grid()
+        xr, yr, zr = xr.flatten(),yr.flatten(),zr.flatten() # (l,w,h) -> (l*w*h)
+        if fmt == 'r':
+            pos = np.stack([xr, yr, zr], axis=-1)  # (l*w*h,3)
+        else:
+            pos = np.reshape([xr,yr,zr], newshape=(3,-1)) # (3,l*w*h)
+        return pos
+
     def _get_reflect_wall_pos(self, gap, wall):
         """得到反射点坐标
         Params
             gap: 墙壁划分网格的间隔
             wall: 第几面墙(0=地板、1-4=前右后左、5=天花板)
         Return
             reflect_pos: 反射点坐标(列表元素个数等于反射单元的个数)
@@ -133,15 +162,15 @@
         xw, yw, zw = xw.flatten(), yw.flatten(), zw.flatten() # 打平操作
         alpha, beta = alpha.flatten(), beta.flatten()
         reflect_pos = np.stack([xw, yw, zw], axis=-1)
         angles = np.stack([alpha, beta], axis=-1)
         return reflect_pos, angles
 
     def set_regular_wall(self):
-        """设置为规制墙壁 (更新墙壁参数)
+        """设置为规则墙壁 (更新墙壁参数)
         """
         # 如果前后左右墙反射单元距离地面最小高度不为0,则无需考虑地面反射
         if self.rp_height[0] > 0 and 0 in self.reflect_wall:
             self.reflect_wall.remove(0)
         # 如果前后左右墙反射单元与天花板最小距离不为0,则无需考虑天花板反射
         if self.rp_height[1] < self.height and 5 in self.reflect_wall:
             self.reflect_wall.remove(5)
@@ -302,45 +331,14 @@
         if not np.all((gap>0) & (gap<self.size)):
             raise VLPValueRangeError(gap, 0, self.size) # The gap setting is not reasonable!
         if gap.size == 1:
             gap = np.full(shape=(3), fill_value=gap) # 填充
         self._tp_gap = gap
 
     @property
-    def tp_grid(self) -> tuple:
-        """获取测试点位置的网格矩阵(所有测试点的相对位置)
-        """
-        (xo, yo, zo) = self._origin #原点位置
-
-        gx, gy, gz = self.tp_gap # 测试区域划分网格的间隔
-        tp_h1, tp_h2 = self.tp_height # 测试区域高度
-        x = np.arange(0, self.length+1e-3, gx) # 房间长度等间隔划分的数组
-        y = np.arange(0, self.width+1e-3, gy)  # 房间宽度等间隔划分的数组
-        z = np.arange(tp_h1, tp_h2+1e-3, gz)   # 测试平面高度等间隔划分的数组
-        xr, yr, zr = np.meshgrid(xo+x, yo+y, zo+z, indexing='ij') # 返回二维网格矩阵（测试点的相对位置）
-        return xr.squeeze(), yr.squeeze(), zr.squeeze() 
-
-    @property
-    def tp_pos(self) -> tuple:
-        """获取测试点位置
-        """
-        xr, yr, zr = self.tp_grid
-        pos = np.stack([xr,yr,zr], axis=-1)
-        return pos
-
-    @property
-    def tp_raw_pos(self) -> tuple:
-        """获取测试点位置
-            shape:(l*w*h)、(l*w*h)、(l*w*h)
-        """
-        xr, yr, zr = self.tp_grid
-        xr, yr, zr = np.reshape(xr,-1), np.reshape(yr,-1), np.reshape(zr,-1)
-        return (xr, yr, zr) 
-
-    @property
     def wall_gap(self):
         """获取墙壁划分网格的间隔 
         """
         return self._wall_gap
     
     @wall_gap.setter
     def wall_gap(self, gap:Union[Number, Sequence]):
```

### Comparing `vlppy-0.1.0/vlppy/setting/__pycache__/json_setting.cpython-39.pyc` & `vlppy-0.1.1/vlppy/setting/__pycache__/json_setting.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `vlppy-0.1.0/vlppy/setting/json_setting.py` & `vlppy-0.1.1/vlppy/setting/json_setting.py`

 * *Files identical despite different names*

### Comparing `vlppy-0.1.0/vlppy/setting/settings.json` & `vlppy-0.1.1/vlppy/setting/settings.json`

 * *Files identical despite different names*

### Comparing `vlppy-0.1.0/vlppy/signal/filter.py` & `vlppy-0.1.1/vlppy/signal/filter.py`

 * *Files identical despite different names*

### Comparing `vlppy-0.1.0/vlppy/signal/plot.py` & `vlppy-0.1.1/vlppy/signal/plot.py`

 * *Files identical despite different names*

### Comparing `vlppy-0.1.0/vlppy/vis/vis.py` & `vlppy-0.1.1/vlppy/vis/vis.py`

 * *Files identical despite different names*

### Comparing `vlppy-0.1.0/vlppy.egg-info/PKG-INFO` & `vlppy-0.1.1/vlppy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vlppy
-Version: 0.1.0
+Version: 0.1.1
 Summary: Construction of visible light positioning model
 Home-page: https://gitee.com/yangwuju/vlppy
 Author: yangwuju
 Author-email: yangwuju <1424134319@qq.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -58,12 +58,12 @@
 
 ```
 py -m pip install vlppy
 ```
 
 @updata log
 
-静态定位（version=0.1.x）；
+静态定位（version=0.1.1）；
 
 将测试平面更新为测试空间区域，可以实现3d定位仿真;
 
 优化部分代码；
```

### Comparing `vlppy-0.1.0/vlppy.egg-info/SOURCES.txt` & `vlppy-0.1.1/vlppy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

