# Comparing `tmp/ibl-neuropixel-0.6.2.tar.gz` & `tmp/ibl-neuropixel-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ibl-neuropixel-0.6.2.tar", last modified: Mon Jun 19 11:04:55 2023, max compression
+gzip compressed data, was "ibl-neuropixel-0.7.0.tar", last modified: Fri Jul 21 17:44:27 2023, max compression
```

## Comparing `ibl-neuropixel-0.6.2.tar` & `ibl-neuropixel-0.7.0.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxrwxr-x   0 olivier   (1000) olivier   (1000)        0 2023-06-19 11:04:55.461601 ibl-neuropixel-0.6.2/
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     1087 2022-04-18 09:47:34.000000 ibl-neuropixel-0.6.2/LICENSE
--rw-rw-r--   0 olivier   (1000) olivier   (1000)       25 2022-04-18 12:17:34.000000 ibl-neuropixel-0.6.2/MANIFEST.in
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     1910 2023-06-19 11:04:55.461601 ibl-neuropixel-0.6.2/PKG-INFO
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     1369 2022-06-01 09:21:00.000000 ibl-neuropixel-0.6.2/README.md
--rw-rw-r--   0 olivier   (1000) olivier   (1000)       38 2023-06-19 11:04:55.461601 ibl-neuropixel-0.6.2/setup.cfg
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     1072 2023-06-19 10:31:03.000000 ibl-neuropixel-0.6.2/setup.py
-drwxrwxr-x   0 olivier   (1000) olivier   (1000)        0 2023-06-19 11:04:55.457601 ibl-neuropixel-0.6.2/src/
-drwxrwxr-x   0 olivier   (1000) olivier   (1000)        0 2023-06-19 11:04:55.457601 ibl-neuropixel-0.6.2/src/ibl_neuropixel.egg-info/
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     1910 2023-06-19 11:04:55.000000 ibl-neuropixel-0.6.2/src/ibl_neuropixel.egg-info/PKG-INFO
--rw-rw-r--   0 olivier   (1000) olivier   (1000)      590 2023-06-19 11:04:55.000000 ibl-neuropixel-0.6.2/src/ibl_neuropixel.egg-info/SOURCES.txt
--rw-rw-r--   0 olivier   (1000) olivier   (1000)        1 2023-06-19 11:04:55.000000 ibl-neuropixel-0.6.2/src/ibl_neuropixel.egg-info/dependency_links.txt
--rw-rw-r--   0 olivier   (1000) olivier   (1000)       57 2023-06-19 11:04:55.000000 ibl-neuropixel-0.6.2/src/ibl_neuropixel.egg-info/requires.txt
--rw-rw-r--   0 olivier   (1000) olivier   (1000)       44 2023-06-19 11:04:55.000000 ibl-neuropixel-0.6.2/src/ibl_neuropixel.egg-info/top_level.txt
-drwxrwxr-x   0 olivier   (1000) olivier   (1000)        0 2023-06-19 11:04:55.461601 ibl-neuropixel-0.6.2/src/neurodsp/
--rw-rw-r--   0 olivier   (1000) olivier   (1000)        0 2022-04-18 12:01:15.000000 ibl-neuropixel-0.6.2/src/neurodsp/__init__.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     6071 2023-03-07 11:56:59.000000 ibl-neuropixel-0.6.2/src/neurodsp/cadzow.py
--rw-r--r--   0 olivier   (1000) olivier   (1000)     2371 2022-04-18 10:38:28.000000 ibl-neuropixel-0.6.2/src/neurodsp/cuda_tools.py
--rw-r--r--   0 olivier   (1000) olivier   (1000)     2763 2022-04-20 07:48:28.000000 ibl-neuropixel-0.6.2/src/neurodsp/destripe_gpu.py
--rw-r--r--   0 olivier   (1000) olivier   (1000)     5838 2022-04-18 09:54:14.000000 ibl-neuropixel-0.6.2/src/neurodsp/filter_gpu.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)    10529 2022-04-18 10:39:58.000000 ibl-neuropixel-0.6.2/src/neurodsp/fourier.py
--rw-r--r--   0 olivier   (1000) olivier   (1000)     7947 2022-04-18 14:10:58.000000 ibl-neuropixel-0.6.2/src/neurodsp/smooth.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     8976 2022-09-07 17:44:13.000000 ibl-neuropixel-0.6.2/src/neurodsp/utils.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)    33322 2023-06-05 17:01:59.000000 ibl-neuropixel-0.6.2/src/neurodsp/voltage.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)    20258 2023-06-14 09:51:06.000000 ibl-neuropixel-0.6.2/src/neurodsp/waveforms.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)    35717 2023-06-06 14:06:55.000000 ibl-neuropixel-0.6.2/src/neuropixel.py
-drwxrwxr-x   0 olivier   (1000) olivier   (1000)        0 2023-06-19 11:04:55.461601 ibl-neuropixel-0.6.2/src/neurowaveforms/
--rw-r--r--   0 olivier   (1000) olivier   (1000)        0 2023-06-06 14:06:55.000000 ibl-neuropixel-0.6.2/src/neurowaveforms/__init__.py
--rw-r--r--   0 olivier   (1000) olivier   (1000)     4692 2023-06-06 14:06:55.000000 ibl-neuropixel-0.6.2/src/neurowaveforms/model.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)    33750 2023-06-19 10:26:14.000000 ibl-neuropixel-0.6.2/src/spikeglx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:44:27.153533 ibl-neuropixel-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-21 17:44:20.000000 ibl-neuropixel-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-21 17:44:20.000000 ibl-neuropixel-0.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-07-21 17:44:27.153533 ibl-neuropixel-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-07-21 17:44:20.000000 ibl-neuropixel-0.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 17:44:27.153533 ibl-neuropixel-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-21 17:44:20.000000 ibl-neuropixel-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:44:27.149533 ibl-neuropixel-0.7.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:44:27.149533 ibl-neuropixel-0.7.0/src/ibl_neuropixel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-07-21 17:44:27.000000 ibl-neuropixel-0.7.0/src/ibl_neuropixel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-21 17:44:27.000000 ibl-neuropixel-0.7.0/src/ibl_neuropixel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 17:44:27.000000 ibl-neuropixel-0.7.0/src/ibl_neuropixel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-21 17:44:27.000000 ibl-neuropixel-0.7.0/src/ibl_neuropixel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-21 17:44:27.000000 ibl-neuropixel-0.7.0/src/ibl_neuropixel.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:44:27.153533 ibl-neuropixel-0.7.0/src/neurodsp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 17:44:20.000000 ibl-neuropixel-0.7.0/src/neurodsp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6071 2023-07-21 17:44:20.000000 ibl-neuropixel-0.7.0/src/neurodsp/cadzow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-07-21 17:44:20.000000 ibl-neuropixel-0.7.0/src/neurodsp/cuda_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-07-21 17:44:20.000000 ibl-neuropixel-0.7.0/src/neurodsp/destripe_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5838 2023-07-21 17:44:20.000000 ibl-neuropixel-0.7.0/src/neurodsp/filter_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10529 2023-07-21 17:44:20.000000 ibl-neuropixel-0.7.0/src/neurodsp/fourier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7947 2023-07-21 17:44:20.000000 ibl-neuropixel-0.7.0/src/neurodsp/smooth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4561 2023-07-21 17:44:20.000000 ibl-neuropixel-0.7.0/src/neurodsp/spiketrains.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8976 2023-07-21 17:44:20.000000 ibl-neuropixel-0.7.0/src/neurodsp/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33322 2023-07-21 17:44:20.000000 ibl-neuropixel-0.7.0/src/neurodsp/voltage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20258 2023-07-21 17:44:20.000000 ibl-neuropixel-0.7.0/src/neurodsp/waveforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35717 2023-07-21 17:44:20.000000 ibl-neuropixel-0.7.0/src/neuropixel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:44:27.153533 ibl-neuropixel-0.7.0/src/neurowaveforms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 17:44:20.000000 ibl-neuropixel-0.7.0/src/neurowaveforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4692 2023-07-21 17:44:20.000000 ibl-neuropixel-0.7.0/src/neurowaveforms/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33750 2023-07-21 17:44:20.000000 ibl-neuropixel-0.7.0/src/spikeglx.py
```

### Comparing `ibl-neuropixel-0.6.2/LICENSE` & `ibl-neuropixel-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ibl-neuropixel-0.6.2/PKG-INFO` & `ibl-neuropixel-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibl-neuropixel
-Version: 0.6.2
+Version: 0.7.0
 Summary: Collection of tools for Neuropixel 1.0 and 2.0 probes data
 Home-page: https://github.com/int-brain-lab/ibl-neuropixel
 Author: The International Brain Laboratory
 Project-URL: Bug Tracker, https://github.com/int-brain-lab/ibl-neuropixel/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ibl-neuropixel-0.6.2/README.md` & `ibl-neuropixel-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `ibl-neuropixel-0.6.2/setup.py` & `ibl-neuropixel-0.7.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 with open('requirements.txt') as f:
     require = [x.strip() for x in f.readlines() if not x.startswith('git+')]
 
 setuptools.setup(
     name="ibl-neuropixel",
-    version="0.6.2",
+    version="0.7.0",
     author="The International Brain Laboratory",
     description="Collection of tools for Neuropixel 1.0 and 2.0 probes data",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/int-brain-lab/ibl-neuropixel",
     project_urls={
         "Bug Tracker": "https://github.com/int-brain-lab/ibl-neuropixel/issues",
```

### Comparing `ibl-neuropixel-0.6.2/src/ibl_neuropixel.egg-info/PKG-INFO` & `ibl-neuropixel-0.7.0/src/ibl_neuropixel.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibl-neuropixel
-Version: 0.6.2
+Version: 0.7.0
 Summary: Collection of tools for Neuropixel 1.0 and 2.0 probes data
 Home-page: https://github.com/int-brain-lab/ibl-neuropixel
 Author: The International Brain Laboratory
 Project-URL: Bug Tracker, https://github.com/int-brain-lab/ibl-neuropixel/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ibl-neuropixel-0.6.2/src/ibl_neuropixel.egg-info/SOURCES.txt` & `ibl-neuropixel-0.7.0/src/ibl_neuropixel.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -12,12 +12,13 @@
 src/neurodsp/__init__.py
 src/neurodsp/cadzow.py
 src/neurodsp/cuda_tools.py
 src/neurodsp/destripe_gpu.py
 src/neurodsp/filter_gpu.py
 src/neurodsp/fourier.py
 src/neurodsp/smooth.py
+src/neurodsp/spiketrains.py
 src/neurodsp/utils.py
 src/neurodsp/voltage.py
 src/neurodsp/waveforms.py
 src/neurowaveforms/__init__.py
 src/neurowaveforms/model.py
```

### Comparing `ibl-neuropixel-0.6.2/src/neurodsp/cadzow.py` & `ibl-neuropixel-0.7.0/src/neurodsp/cadzow.py`

 * *Files identical despite different names*

### Comparing `ibl-neuropixel-0.6.2/src/neurodsp/cuda_tools.py` & `ibl-neuropixel-0.7.0/src/neurodsp/cuda_tools.py`

 * *Files identical despite different names*

### Comparing `ibl-neuropixel-0.6.2/src/neurodsp/destripe_gpu.py` & `ibl-neuropixel-0.7.0/src/neurodsp/destripe_gpu.py`

 * *Files identical despite different names*

### Comparing `ibl-neuropixel-0.6.2/src/neurodsp/filter_gpu.py` & `ibl-neuropixel-0.7.0/src/neurodsp/filter_gpu.py`

 * *Files identical despite different names*

### Comparing `ibl-neuropixel-0.6.2/src/neurodsp/fourier.py` & `ibl-neuropixel-0.7.0/src/neurodsp/fourier.py`

 * *Files identical despite different names*

### Comparing `ibl-neuropixel-0.6.2/src/neurodsp/smooth.py` & `ibl-neuropixel-0.7.0/src/neurodsp/smooth.py`

 * *Files identical despite different names*

### Comparing `ibl-neuropixel-0.6.2/src/neurodsp/utils.py` & `ibl-neuropixel-0.7.0/src/neurodsp/utils.py`

 * *Files identical despite different names*

### Comparing `ibl-neuropixel-0.6.2/src/neurodsp/voltage.py` & `ibl-neuropixel-0.7.0/src/neurodsp/voltage.py`

 * *Files identical despite different names*

### Comparing `ibl-neuropixel-0.6.2/src/neurodsp/waveforms.py` & `ibl-neuropixel-0.7.0/src/neurodsp/waveforms.py`

 * *Files identical despite different names*

### Comparing `ibl-neuropixel-0.6.2/src/neuropixel.py` & `ibl-neuropixel-0.7.0/src/neuropixel.py`

 * *Files identical despite different names*

### Comparing `ibl-neuropixel-0.6.2/src/neurowaveforms/model.py` & `ibl-neuropixel-0.7.0/src/neurowaveforms/model.py`

 * *Files identical despite different names*

### Comparing `ibl-neuropixel-0.6.2/src/spikeglx.py` & `ibl-neuropixel-0.7.0/src/spikeglx.py`

 * *Files identical despite different names*

