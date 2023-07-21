# Comparing `tmp/pyftch-1.0.1.tar.gz` & `tmp/pyftch-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyftch-1.0.1.tar", last modified: Fri Jul 21 18:06:35 2023, max compression
+gzip compressed data, was "pyftch-1.0.2.tar", last modified: Fri Jul 21 18:59:45 2023, max compression
```

## Comparing `pyftch-1.0.1.tar` & `pyftch-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 krit      (1000) krit      (1001)        0 2023-07-21 18:06:35.640873 pyftch-1.0.1/
--rw-r--r--   0 krit      (1000) krit      (1001)     1066 2023-07-21 17:43:52.000000 pyftch-1.0.1/LICENSE
--rw-r--r--   0 krit      (1000) krit      (1001)     3634 2023-07-21 18:06:35.639873 pyftch-1.0.1/PKG-INFO
--rw-r--r--   0 krit      (1000) krit      (1001)     1161 2023-07-21 18:04:51.000000 pyftch-1.0.1/README.md
--rw-r--r--   0 krit      (1000) krit      (1001)     1334 2023-07-21 18:06:23.000000 pyftch-1.0.1/pyproject.toml
--rw-r--r--   0 krit      (1000) krit      (1001)       38 2023-07-21 18:06:35.640873 pyftch-1.0.1/setup.cfg
-drwxr-xr-x   0 krit      (1000) krit      (1001)        0 2023-07-21 18:06:35.638873 pyftch-1.0.1/src/
-drwxr-xr-x   0 krit      (1000) krit      (1001)        0 2023-07-21 18:06:35.639873 pyftch-1.0.1/src/pyftch/
--rw-r--r--   0 krit      (1000) krit      (1001)        0 2023-07-21 18:04:51.000000 pyftch-1.0.1/src/pyftch/__init__.py
--rwxr-xr-x   0 krit      (1000) krit      (1001)     7683 2023-07-21 18:04:51.000000 pyftch-1.0.1/src/pyftch/__main__.py
-drwxr-xr-x   0 krit      (1000) krit      (1001)        0 2023-07-21 18:06:35.639873 pyftch-1.0.1/src/pyftch.egg-info/
--rw-r--r--   0 krit      (1000) krit      (1001)     3634 2023-07-21 18:06:35.000000 pyftch-1.0.1/src/pyftch.egg-info/PKG-INFO
--rw-r--r--   0 krit      (1000) krit      (1001)      251 2023-07-21 18:06:35.000000 pyftch-1.0.1/src/pyftch.egg-info/SOURCES.txt
--rw-r--r--   0 krit      (1000) krit      (1001)        1 2023-07-21 18:06:35.000000 pyftch-1.0.1/src/pyftch.egg-info/dependency_links.txt
--rw-r--r--   0 krit      (1000) krit      (1001)       48 2023-07-21 18:06:35.000000 pyftch-1.0.1/src/pyftch.egg-info/entry_points.txt
--rw-r--r--   0 krit      (1000) krit      (1001)        7 2023-07-21 18:06:35.000000 pyftch-1.0.1/src/pyftch.egg-info/top_level.txt
+drwxr-xr-x   0 krit      (1000) krit      (1001)        0 2023-07-21 18:59:45.062005 pyftch-1.0.2/
+-rw-r--r--   0 krit      (1000) krit      (1001)     1066 2023-07-21 17:43:52.000000 pyftch-1.0.2/LICENSE
+-rw-r--r--   0 krit      (1000) krit      (1001)     3761 2023-07-21 18:59:45.062005 pyftch-1.0.2/PKG-INFO
+-rw-r--r--   0 krit      (1000) krit      (1001)     1288 2023-07-21 18:57:20.000000 pyftch-1.0.2/README.md
+-rw-r--r--   0 krit      (1000) krit      (1001)     1334 2023-07-21 18:59:08.000000 pyftch-1.0.2/pyproject.toml
+-rw-r--r--   0 krit      (1000) krit      (1001)       38 2023-07-21 18:59:45.062005 pyftch-1.0.2/setup.cfg
+drwxr-xr-x   0 krit      (1000) krit      (1001)        0 2023-07-21 18:59:45.061005 pyftch-1.0.2/src/
+drwxr-xr-x   0 krit      (1000) krit      (1001)        0 2023-07-21 18:59:45.062005 pyftch-1.0.2/src/pyftch/
+-rw-r--r--   0 krit      (1000) krit      (1001)        0 2023-07-21 18:07:08.000000 pyftch-1.0.2/src/pyftch/__init__.py
+-rwxr-xr-x   0 krit      (1000) krit      (1001)     7683 2023-07-21 18:07:08.000000 pyftch-1.0.2/src/pyftch/__main__.py
+drwxr-xr-x   0 krit      (1000) krit      (1001)        0 2023-07-21 18:59:45.062005 pyftch-1.0.2/src/pyftch.egg-info/
+-rw-r--r--   0 krit      (1000) krit      (1001)     3761 2023-07-21 18:59:45.000000 pyftch-1.0.2/src/pyftch.egg-info/PKG-INFO
+-rw-r--r--   0 krit      (1000) krit      (1001)      251 2023-07-21 18:59:45.000000 pyftch-1.0.2/src/pyftch.egg-info/SOURCES.txt
+-rw-r--r--   0 krit      (1000) krit      (1001)        1 2023-07-21 18:59:45.000000 pyftch-1.0.2/src/pyftch.egg-info/dependency_links.txt
+-rw-r--r--   0 krit      (1000) krit      (1001)       48 2023-07-21 18:59:45.000000 pyftch-1.0.2/src/pyftch.egg-info/entry_points.txt
+-rw-r--r--   0 krit      (1000) krit      (1001)        7 2023-07-21 18:59:45.000000 pyftch-1.0.2/src/pyftch.egg-info/top_level.txt
```

### Comparing `pyftch-1.0.1/LICENSE` & `pyftch-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyftch-1.0.1/PKG-INFO` & `pyftch-1.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyftch
-Version: 1.0.1
+Version: 1.0.2
 Summary: A lightweight and elegant fetch for Linux written in Python with no dependencies.
 Author-email: Krit Dass <dasskrit@gmail.com>
 Maintainer-email: Krit Dass <dasskrit@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Krit Dass
         
@@ -59,8 +59,8 @@
 Pyftch is a small and efficient fetch script inspired by [nitch](https://github.com/ssleert/nitch) and [pfetch](https://github.com/dylanaraps/pfetch). It has a relatively fast execution time of ~20ms and is tested on Python versions 3.7 or newer and PyPy (it will probably work on earlier versions but has not been tested as such). It is configured by editing its source code, though the Python used is relatively simple and readable. Rest assured, if you do not understand something, open up an issue and I will be happy to explain it to you. At its current state, Pyftch only supports a few popular Linux distributions (see [this function](https://github.com/kritdass/pyftch/blob/873ffd62d048b7b27da0153ab21e70eb92f7efe5/src/pyftch/__main__.py#L426) for a list though most are not tested). If support is lacking for your distribution, please open up an issue and I will add support for your distribution. Pull requests are welcome and encouraged, please do not hesitate.
 
 ## Installation
 
 ```
   $ pip install pyftch
 ```
-
+You will need a [Nerd Font](https://www.nerdfonts.com/) to see the icons. I use [JetFlow](https://github.com/kritdass/JetFlow).
```

### Comparing `pyftch-1.0.1/README.md` & `pyftch-1.0.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 Pyftch is a small and efficient fetch script inspired by [nitch](https://github.com/ssleert/nitch) and [pfetch](https://github.com/dylanaraps/pfetch). It has a relatively fast execution time of ~20ms and is tested on Python versions 3.7 or newer and PyPy (it will probably work on earlier versions but has not been tested as such). It is configured by editing its source code, though the Python used is relatively simple and readable. Rest assured, if you do not understand something, open up an issue and I will be happy to explain it to you. At its current state, Pyftch only supports a few popular Linux distributions (see [this function](https://github.com/kritdass/pyftch/blob/873ffd62d048b7b27da0153ab21e70eb92f7efe5/src/pyftch/__main__.py#L426) for a list though most are not tested). If support is lacking for your distribution, please open up an issue and I will add support for your distribution. Pull requests are welcome and encouraged, please do not hesitate.
 
 ## Installation
 
 ```
   $ pip install pyftch
 ```
-
+You will need a [Nerd Font](https://www.nerdfonts.com/) to see the icons. I use [JetFlow](https://github.com/kritdass/JetFlow).
```

### Comparing `pyftch-1.0.1/pyproject.toml` & `pyftch-1.0.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyftch"
-version = "1.0.1"
+version = "1.0.2"
 description = "A lightweight and elegant fetch for Linux written in Python with no dependencies."
 readme = "README.md"
 authors = [{ name = "Krit Dass", email = "dasskrit@gmail.com" }]
 maintainers = [{ name = "Krit Dass", email = "dasskrit@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
   "Development Status :: 1 - Planning",
```

### Comparing `pyftch-1.0.1/src/pyftch/__main__.py` & `pyftch-1.0.2/src/pyftch/__main__.py`

 * *Files identical despite different names*

### Comparing `pyftch-1.0.1/src/pyftch.egg-info/PKG-INFO` & `pyftch-1.0.2/src/pyftch.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyftch
-Version: 1.0.1
+Version: 1.0.2
 Summary: A lightweight and elegant fetch for Linux written in Python with no dependencies.
 Author-email: Krit Dass <dasskrit@gmail.com>
 Maintainer-email: Krit Dass <dasskrit@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Krit Dass
         
@@ -59,8 +59,8 @@
 Pyftch is a small and efficient fetch script inspired by [nitch](https://github.com/ssleert/nitch) and [pfetch](https://github.com/dylanaraps/pfetch). It has a relatively fast execution time of ~20ms and is tested on Python versions 3.7 or newer and PyPy (it will probably work on earlier versions but has not been tested as such). It is configured by editing its source code, though the Python used is relatively simple and readable. Rest assured, if you do not understand something, open up an issue and I will be happy to explain it to you. At its current state, Pyftch only supports a few popular Linux distributions (see [this function](https://github.com/kritdass/pyftch/blob/873ffd62d048b7b27da0153ab21e70eb92f7efe5/src/pyftch/__main__.py#L426) for a list though most are not tested). If support is lacking for your distribution, please open up an issue and I will add support for your distribution. Pull requests are welcome and encouraged, please do not hesitate.
 
 ## Installation
 
 ```
   $ pip install pyftch
 ```
-
+You will need a [Nerd Font](https://www.nerdfonts.com/) to see the icons. I use [JetFlow](https://github.com/kritdass/JetFlow).
```

