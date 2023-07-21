# Comparing `tmp/brokerage-0.0.7.tar.gz` & `tmp/brokerage-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brokerage-0.0.7.tar", last modified: Fri Aug 26 06:41:22 2022, max compression
+gzip compressed data, was "brokerage-0.0.8.tar", last modified: Fri Jul 21 03:40:54 2023, max compression
```

## Comparing `brokerage-0.0.7.tar` & `brokerage-0.0.8.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxrwxr-x   0 kygoh     (1000) kygoh     (1000)        0 2022-08-26 06:41:22.061156 brokerage-0.0.7/
--rw-rw-r--   0 kygoh     (1000) kygoh     (1000)     1066 2022-06-21 14:16:49.000000 brokerage-0.0.7/LICENSE
--rw-rw-r--   0 kygoh     (1000) kygoh     (1000)      665 2022-08-26 06:41:22.061156 brokerage-0.0.7/PKG-INFO
--rw-rw-r--   0 kygoh     (1000) kygoh     (1000)       47 2022-06-21 14:16:49.000000 brokerage-0.0.7/README.md
-drwxrwxr-x   0 kygoh     (1000) kygoh     (1000)        0 2022-08-26 06:41:22.061156 brokerage-0.0.7/brokerage/
--rw-rw-r--   0 kygoh     (1000) kygoh     (1000)      126 2022-06-24 05:29:32.000000 brokerage-0.0.7/brokerage/__init__.py
--rw-rw-r--   0 kygoh     (1000) kygoh     (1000)      164 2022-08-04 13:11:59.000000 brokerage-0.0.7/brokerage/brokerage.py
--rw-rw-r--   0 kygoh     (1000) kygoh     (1000)     9697 2022-08-26 06:39:40.000000 brokerage-0.0.7/brokerage/make_simulator.py
--rw-rw-r--   0 kygoh     (1000) kygoh     (1000)      488 2022-06-23 06:53:22.000000 brokerage-0.0.7/brokerage/minimal_connect.py
-drwxrwxr-x   0 kygoh     (1000) kygoh     (1000)        0 2022-08-26 06:41:22.061156 brokerage-0.0.7/brokerage.egg-info/
--rw-rw-r--   0 kygoh     (1000) kygoh     (1000)      665 2022-08-26 06:41:22.000000 brokerage-0.0.7/brokerage.egg-info/PKG-INFO
--rw-rw-r--   0 kygoh     (1000) kygoh     (1000)      275 2022-08-26 06:41:22.000000 brokerage-0.0.7/brokerage.egg-info/SOURCES.txt
--rw-rw-r--   0 kygoh     (1000) kygoh     (1000)        1 2022-08-26 06:41:22.000000 brokerage-0.0.7/brokerage.egg-info/dependency_links.txt
--rw-rw-r--   0 kygoh     (1000) kygoh     (1000)       10 2022-08-26 06:41:22.000000 brokerage-0.0.7/brokerage.egg-info/top_level.txt
--rw-rw-r--   0 kygoh     (1000) kygoh     (1000)      588 2022-08-26 06:40:52.000000 brokerage-0.0.7/pyproject.toml
--rw-rw-r--   0 kygoh     (1000) kygoh     (1000)       38 2022-08-26 06:41:22.061156 brokerage-0.0.7/setup.cfg
--rw-rw-r--   0 kygoh     (1000) kygoh     (1000)      735 2022-06-22 01:19:55.000000 brokerage-0.0.7/setup.py
+drwxrwxr-x   0 kygoh     (1000) kygoh     (1000)        0 2023-07-21 03:40:54.987029 brokerage-0.0.8/
+-rw-rw-r--   0 kygoh     (1000) kygoh     (1000)     1066 2022-06-21 14:16:49.000000 brokerage-0.0.8/LICENSE
+-rw-rw-r--   0 kygoh     (1000) kygoh     (1000)      665 2023-07-21 03:40:54.987029 brokerage-0.0.8/PKG-INFO
+-rw-rw-r--   0 kygoh     (1000) kygoh     (1000)       47 2022-06-21 14:16:49.000000 brokerage-0.0.8/README.md
+drwxrwxr-x   0 kygoh     (1000) kygoh     (1000)        0 2023-07-21 03:40:54.987029 brokerage-0.0.8/brokerage/
+-rw-rw-r--   0 kygoh     (1000) kygoh     (1000)      126 2022-06-24 05:29:32.000000 brokerage-0.0.8/brokerage/__init__.py
+-rw-rw-r--   0 kygoh     (1000) kygoh     (1000)      202 2023-07-21 03:13:53.000000 brokerage-0.0.8/brokerage/brokerage.py
+-rw-rw-r--   0 kygoh     (1000) kygoh     (1000)     9763 2023-07-16 15:51:13.000000 brokerage-0.0.8/brokerage/make_simulator.py
+-rw-rw-r--   0 kygoh     (1000) kygoh     (1000)      567 2023-07-14 00:47:22.000000 brokerage-0.0.8/brokerage/minimal_connect.py
+drwxrwxr-x   0 kygoh     (1000) kygoh     (1000)        0 2023-07-21 03:40:54.987029 brokerage-0.0.8/brokerage.egg-info/
+-rw-rw-r--   0 kygoh     (1000) kygoh     (1000)      665 2023-07-21 03:40:54.000000 brokerage-0.0.8/brokerage.egg-info/PKG-INFO
+-rw-rw-r--   0 kygoh     (1000) kygoh     (1000)      293 2023-07-21 03:40:54.000000 brokerage-0.0.8/brokerage.egg-info/SOURCES.txt
+-rw-rw-r--   0 kygoh     (1000) kygoh     (1000)        1 2023-07-21 03:40:54.000000 brokerage-0.0.8/brokerage.egg-info/dependency_links.txt
+-rw-rw-r--   0 kygoh     (1000) kygoh     (1000)       10 2023-07-21 03:40:54.000000 brokerage-0.0.8/brokerage.egg-info/top_level.txt
+-rw-rw-r--   0 kygoh     (1000) kygoh     (1000)      588 2023-07-21 00:50:40.000000 brokerage-0.0.8/pyproject.toml
+-rw-rw-r--   0 kygoh     (1000) kygoh     (1000)       38 2023-07-21 03:40:54.987029 brokerage-0.0.8/setup.cfg
+-rw-rw-r--   0 kygoh     (1000) kygoh     (1000)      735 2023-07-21 03:08:27.000000 brokerage-0.0.8/setup.py
+drwxrwxr-x   0 kygoh     (1000) kygoh     (1000)        0 2023-07-21 03:40:54.987029 brokerage-0.0.8/tests/
+-rw-rw-r--   0 kygoh     (1000) kygoh     (1000)       69 2022-06-22 00:36:54.000000 brokerage-0.0.8/tests/test_foo.py
```

### Comparing `brokerage-0.0.7/LICENSE` & `brokerage-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `brokerage-0.0.7/PKG-INFO` & `brokerage-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brokerage
-Version: 0.0.7
+Version: 0.0.8
 Summary: Simulate data feed from broker
 Home-page: https://github.com/yongkheng/brokerage
 Author: Goh Yong Kheng
 Author-email: Goh Yong Kheng <goh.yongkheng@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/yongkheng/brokerage
 Project-URL: Bug Tracker, https://github.com/yongkheng/brokerage/issues
```

### Comparing `brokerage-0.0.7/brokerage/make_simulator.py` & `brokerage-0.0.8/brokerage/make_simulator.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,14 +86,15 @@
         significant = max([item[::-1].find(".") for item in quote])
         o, h, l, c = [float(item) for item in quote]
         if n_ticks == 4:
             hl = [h, l]
             np.random.shuffle(hl)
             return [o, *hl, c]
         sigma = (h - l) / n_ticks
+        sigma = np.sqrt(2*abs(np.log(c/o)))
         dB = np.random.randn(n_ticks) / np.sqrt(n_ticks - 1)
         dB[0] = 0
         B = dB.cumsum()
         ticks = o * np.exp(-(sigma ** 2) / 2 + sigma * B)
         if ticks.max() > ticks.min():
             ticks = (ticks - ticks.min()) * (h - l) / (ticks.max() - ticks.min()) + l
         ticks = np.round(ticks, significant)
@@ -102,14 +103,15 @@
         ticks[ticks[1:-1].argmax() + 1] = h
         ticks[ticks[1:-1].argmin() + 1] = l
         cond = ticks[0] == o, ticks.max() == h, ticks.min() == l, ticks[-1] == c
         if not all(cond):
             print(
                 f"\033[35mWARNING:: [{o}, {h}, {l}, {c}] not equal [{ticks[0]}, {ticks.max()}, {ticks.min()}, {ticks[-1]}]\033[0m"
             )
+        #breakpoint()
         return ticks
 
     def _set_fake_data(self, samples):
         import datetime as dt
         import numpy as np
 
         np.random.seed(self.seed)
```

### Comparing `brokerage-0.0.7/brokerage.egg-info/PKG-INFO` & `brokerage-0.0.8/brokerage.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brokerage
-Version: 0.0.7
+Version: 0.0.8
 Summary: Simulate data feed from broker
 Home-page: https://github.com/yongkheng/brokerage
 Author: Goh Yong Kheng
 Author-email: Goh Yong Kheng <goh.yongkheng@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/yongkheng/brokerage
 Project-URL: Bug Tracker, https://github.com/yongkheng/brokerage/issues
```

### Comparing `brokerage-0.0.7/pyproject.toml` & `brokerage-0.0.8/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "brokerage"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="Goh Yong Kheng", email="goh.yongkheng@gmail.com" },
 ]
 description = "Simulate data feed from broker"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `brokerage-0.0.7/setup.py` & `brokerage-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 def readme():
     with open("README.md") as f:
         return f.read()
 
 setup(
     name="brokerage",
-    version="0.0.1",
+    version="0.0.8",
     description="Simulate data feed from brokerage",
     long_description=readme(),
     logn_description_content_type="text/markdown",
     classifiers=[
         "Development Status :: Unstable",
         "License :: MIT License",
         "Programming Language :: Python 3.10",
```

