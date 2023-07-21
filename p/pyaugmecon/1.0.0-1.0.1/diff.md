# Comparing `tmp/pyaugmecon-1.0.0.tar.gz` & `tmp/pyaugmecon-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyaugmecon-1.0.0.tar", last modified: Mon Apr 17 13:16:57 2023, max compression
+gzip compressed data, was "pyaugmecon-1.0.1.tar", last modified: Fri Jul 21 11:02:33 2023, max compression
```

## Comparing `pyaugmecon-1.0.0.tar` & `pyaugmecon-1.0.1.tar`

### file list

```diff
@@ -1,23 +1,34 @@
-drwxr-xr-x   0 whbles    (1000) whbles    (1000)        0 2023-04-17 13:16:57.217151 pyaugmecon-1.0.0/
--rw-r--r--   0 whbles    (1000) whbles    (1000)     1164 2021-10-16 20:28:36.000000 pyaugmecon-1.0.0/LICENSE
--rw-r--r--   0 whbles    (1000) whbles    (1000)    28216 2023-04-17 13:16:57.217151 pyaugmecon-1.0.0/PKG-INFO
--rw-r--r--   0 whbles    (1000) whbles    (1000)    26087 2023-04-17 13:10:38.000000 pyaugmecon-1.0.0/README.md
-drwxr-xr-x   0 whbles    (1000) whbles    (1000)        0 2023-04-17 13:16:57.217151 pyaugmecon-1.0.0/pyaugmecon/
--rw-r--r--   0 whbles    (1000) whbles    (1000)       45 2021-10-16 20:28:36.000000 pyaugmecon-1.0.0/pyaugmecon/__init__.py
--rw-r--r--   0 whbles    (1000) whbles    (1000)     1349 2023-04-17 13:10:38.000000 pyaugmecon-1.0.0/pyaugmecon/flag.py
--rw-r--r--   0 whbles    (1000) whbles    (1000)     2483 2023-04-17 13:10:38.000000 pyaugmecon-1.0.0/pyaugmecon/helper.py
--rw-r--r--   0 whbles    (1000) whbles    (1000)     1295 2023-04-17 13:10:38.000000 pyaugmecon-1.0.0/pyaugmecon/logs.py
--rw-r--r--   0 whbles    (1000) whbles    (1000)    11055 2023-04-17 13:10:38.000000 pyaugmecon-1.0.0/pyaugmecon/model.py
--rw-r--r--   0 whbles    (1000) whbles    (1000)     4029 2023-04-17 13:10:38.000000 pyaugmecon-1.0.0/pyaugmecon/options.py
--rw-r--r--   0 whbles    (1000) whbles    (1000)     2616 2023-04-17 13:10:38.000000 pyaugmecon-1.0.0/pyaugmecon/process_handler.py
--rw-r--r--   0 whbles    (1000) whbles    (1000)     9360 2023-04-17 13:10:50.000000 pyaugmecon-1.0.0/pyaugmecon/pyaugmecon.py
--rw-r--r--   0 whbles    (1000) whbles    (1000)     4230 2023-04-17 13:10:38.000000 pyaugmecon-1.0.0/pyaugmecon/queue_handler.py
--rw-r--r--   0 whbles    (1000) whbles    (1000)     6603 2023-04-17 13:10:38.000000 pyaugmecon-1.0.0/pyaugmecon/solver_process.py
-drwxr-xr-x   0 whbles    (1000) whbles    (1000)        0 2023-04-17 13:16:57.217151 pyaugmecon-1.0.0/pyaugmecon.egg-info/
--rw-r--r--   0 whbles    (1000) whbles    (1000)    28216 2023-04-17 13:16:57.000000 pyaugmecon-1.0.0/pyaugmecon.egg-info/PKG-INFO
--rw-r--r--   0 whbles    (1000) whbles    (1000)      431 2023-04-17 13:16:57.000000 pyaugmecon-1.0.0/pyaugmecon.egg-info/SOURCES.txt
--rw-r--r--   0 whbles    (1000) whbles    (1000)        1 2023-04-17 13:16:57.000000 pyaugmecon-1.0.0/pyaugmecon.egg-info/dependency_links.txt
--rw-r--r--   0 whbles    (1000) whbles    (1000)      107 2023-04-17 13:16:57.000000 pyaugmecon-1.0.0/pyaugmecon.egg-info/requires.txt
--rw-r--r--   0 whbles    (1000) whbles    (1000)       11 2023-04-17 13:16:57.000000 pyaugmecon-1.0.0/pyaugmecon.egg-info/top_level.txt
--rw-r--r--   0 whbles    (1000) whbles    (1000)       38 2023-04-17 13:16:57.217151 pyaugmecon-1.0.0/setup.cfg
--rw-r--r--   0 whbles    (1000) whbles    (1000)     1843 2023-04-17 13:13:24.000000 pyaugmecon-1.0.0/setup.py
+drwxr-xr-x   0 whbles    (1000) whbles    (1000)        0 2023-07-21 11:02:33.387499 pyaugmecon-1.0.1/
+-rw-r--r--   0 whbles    (1000) whbles    (1000)     1164 2021-10-16 20:28:36.000000 pyaugmecon-1.0.1/LICENSE
+-rw-r--r--   0 whbles    (1000) whbles    (1000)    28282 2023-07-21 11:02:33.387499 pyaugmecon-1.0.1/PKG-INFO
+-rw-r--r--   0 whbles    (1000) whbles    (1000)    26087 2023-04-17 13:10:38.000000 pyaugmecon-1.0.1/README.md
+drwxr-xr-x   0 whbles    (1000) whbles    (1000)        0 2023-07-21 11:02:33.377498 pyaugmecon-1.0.1/pyaugmecon/
+-rw-r--r--   0 whbles    (1000) whbles    (1000)       45 2021-10-16 20:28:36.000000 pyaugmecon-1.0.1/pyaugmecon/__init__.py
+-rw-r--r--   0 whbles    (1000) whbles    (1000)     1349 2023-04-17 13:10:38.000000 pyaugmecon-1.0.1/pyaugmecon/flag.py
+-rw-r--r--   0 whbles    (1000) whbles    (1000)     2483 2023-04-17 13:10:38.000000 pyaugmecon-1.0.1/pyaugmecon/helper.py
+-rw-r--r--   0 whbles    (1000) whbles    (1000)     1295 2023-04-17 13:10:38.000000 pyaugmecon-1.0.1/pyaugmecon/logs.py
+-rw-r--r--   0 whbles    (1000) whbles    (1000)    11055 2023-04-17 13:10:38.000000 pyaugmecon-1.0.1/pyaugmecon/model.py
+-rw-r--r--   0 whbles    (1000) whbles    (1000)     4029 2023-04-17 13:10:38.000000 pyaugmecon-1.0.1/pyaugmecon/options.py
+-rw-r--r--   0 whbles    (1000) whbles    (1000)     2616 2023-04-17 13:10:38.000000 pyaugmecon-1.0.1/pyaugmecon/process_handler.py
+-rw-r--r--   0 whbles    (1000) whbles    (1000)     9360 2023-04-17 13:10:50.000000 pyaugmecon-1.0.1/pyaugmecon/pyaugmecon.py
+-rw-r--r--   0 whbles    (1000) whbles    (1000)     4275 2023-07-21 10:34:45.000000 pyaugmecon-1.0.1/pyaugmecon/queue_handler.py
+-rw-r--r--   0 whbles    (1000) whbles    (1000)     6603 2023-04-17 13:10:38.000000 pyaugmecon-1.0.1/pyaugmecon/solver_process.py
+drwxr-xr-x   0 whbles    (1000) whbles    (1000)        0 2023-07-21 11:02:33.377498 pyaugmecon-1.0.1/pyaugmecon.egg-info/
+-rw-r--r--   0 whbles    (1000) whbles    (1000)    28282 2023-07-21 11:02:33.000000 pyaugmecon-1.0.1/pyaugmecon.egg-info/PKG-INFO
+-rw-r--r--   0 whbles    (1000) whbles    (1000)      670 2023-07-21 11:02:33.000000 pyaugmecon-1.0.1/pyaugmecon.egg-info/SOURCES.txt
+-rw-r--r--   0 whbles    (1000) whbles    (1000)        1 2023-07-21 11:02:33.000000 pyaugmecon-1.0.1/pyaugmecon.egg-info/dependency_links.txt
+-rw-r--r--   0 whbles    (1000) whbles    (1000)      107 2023-07-21 11:02:33.000000 pyaugmecon-1.0.1/pyaugmecon.egg-info/requires.txt
+-rw-r--r--   0 whbles    (1000) whbles    (1000)       11 2023-07-21 11:02:33.000000 pyaugmecon-1.0.1/pyaugmecon.egg-info/top_level.txt
+-rw-r--r--   0 whbles    (1000) whbles    (1000)       38 2023-07-21 11:02:33.387499 pyaugmecon-1.0.1/setup.cfg
+-rw-r--r--   0 whbles    (1000) whbles    (1000)     1843 2023-07-21 10:38:11.000000 pyaugmecon-1.0.1/setup.py
+drwxr-xr-x   0 whbles    (1000) whbles    (1000)        0 2023-07-21 11:02:33.387499 pyaugmecon-1.0.1/tests/
+-rw-r--r--   0 whbles    (1000) whbles    (1000)      709 2023-04-04 17:14:23.000000 pyaugmecon-1.0.1/tests/test_2kp100.py
+-rw-r--r--   0 whbles    (1000) whbles    (1000)      710 2023-04-04 17:14:23.000000 pyaugmecon-1.0.1/tests/test_2kp250.py
+-rw-r--r--   0 whbles    (1000) whbles    (1000)      708 2023-04-04 17:14:23.000000 pyaugmecon-1.0.1/tests/test_2kp50.py
+-rw-r--r--   0 whbles    (1000) whbles    (1000)      746 2023-04-04 17:14:23.000000 pyaugmecon-1.0.1/tests/test_3kp40.py
+-rw-r--r--   0 whbles    (1000) whbles    (1000)      746 2023-04-04 17:14:23.000000 pyaugmecon-1.0.1/tests/test_3kp50.py
+-rw-r--r--   0 whbles    (1000) whbles    (1000)      747 2023-04-04 17:14:23.000000 pyaugmecon-1.0.1/tests/test_4kp40.py
+-rw-r--r--   0 whbles    (1000) whbles    (1000)      746 2023-04-04 17:14:23.000000 pyaugmecon-1.0.1/tests/test_4kp50.py
+-rw-r--r--   0 whbles    (1000) whbles    (1000)     1314 2023-04-04 17:14:23.000000 pyaugmecon-1.0.1/tests/test_three_objectives.py
+-rw-r--r--   0 whbles    (1000) whbles    (1000)     1351 2023-04-04 17:14:23.000000 pyaugmecon-1.0.1/tests/test_three_objectives_mixed.py
+-rw-r--r--   0 whbles    (1000) whbles    (1000)      881 2023-04-04 17:14:23.000000 pyaugmecon-1.0.1/tests/test_two_objectives.py
```

### Comparing `pyaugmecon-1.0.0/LICENSE` & `pyaugmecon-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyaugmecon-1.0.0/PKG-INFO` & `pyaugmecon-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaugmecon
-Version: 1.0.0
+Version: 1.0.1
 Home-page: https://github.com/wouterbles/pyaugmecon
 Author: Wouter Bles
 Author-email: whbles@gmail.com
 License: MIT
 Project-URL: Changelog, https://github.com/wouterbles/pyaugmecon/blob/main/CHANGELOG.md
 Keywords: python,pyomo,optimization,multi-objective-optimization,augmecon
 Classifier: Development Status :: 3 - Alpha
@@ -347,14 +347,18 @@
 
 - Wouter Bles (current version of the package)
 - Nikolaos Paterakis (initial implementation)
 
 
 # Changelog
 
+## 1.0.1
+
+- Make QueueHandler work on MacOS #5, thanks @yvanoers
+
 ## 1.0.0
 
 - Add new methods for solution retrieval
 
 ## 0.2.1
 
 - Add Python 3.10 to supported versions
```

### Comparing `pyaugmecon-1.0.0/README.md` & `pyaugmecon-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pyaugmecon-1.0.0/pyaugmecon/flag.py` & `pyaugmecon-1.0.1/pyaugmecon/flag.py`

 * *Files identical despite different names*

### Comparing `pyaugmecon-1.0.0/pyaugmecon/helper.py` & `pyaugmecon-1.0.1/pyaugmecon/helper.py`

 * *Files identical despite different names*

### Comparing `pyaugmecon-1.0.0/pyaugmecon/logs.py` & `pyaugmecon-1.0.1/pyaugmecon/logs.py`

 * *Files identical despite different names*

### Comparing `pyaugmecon-1.0.0/pyaugmecon/model.py` & `pyaugmecon-1.0.1/pyaugmecon/model.py`

 * *Files identical despite different names*

### Comparing `pyaugmecon-1.0.0/pyaugmecon/options.py` & `pyaugmecon-1.0.1/pyaugmecon/options.py`

 * *Files identical despite different names*

### Comparing `pyaugmecon-1.0.0/pyaugmecon/process_handler.py` & `pyaugmecon-1.0.1/pyaugmecon/process_handler.py`

 * *Files identical despite different names*

### Comparing `pyaugmecon-1.0.0/pyaugmecon/pyaugmecon.py` & `pyaugmecon-1.0.1/pyaugmecon/pyaugmecon.py`

 * *Files identical despite different names*

### Comparing `pyaugmecon-1.0.0/pyaugmecon/queue_handler.py` & `pyaugmecon-1.0.1/pyaugmecon/queue_handler.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
 import queue
-from multiprocessing import Queue
+from multiprocessing import Queue, Manager
 
 import numpy as np
 
 from pyaugmecon.options import Options
 
 
 class QueueHandler:
@@ -117,14 +117,15 @@
         """
         block_size = self.opts.gp  # Get the block size from the options
         blocks = [
             self.work[i : i + block_size] for i in range(0, len(self.work), block_size)
         ]  # Divide the work into blocks
         blocks = np.array_split(np.array(blocks), self.opts.cpu_count)  # Divide the blocks into sub-blocks
         blocks = [x for x in blocks if x.size > 0]  # Remove empty sub-blocks
+        manager = Manager()
         self.proc_count = len(blocks)  # Set the number of processes to be used
-        self.job_qs = [Queue() for _ in range(self.proc_count)]  # Create a job queue for each process
+        self.job_qs = [manager.Queue() for _ in range(self.proc_count)]  # Create a job queue for each process
         self.logger.info(f"Dividing grid over {self.proc_count} process(es)")  # Log the number of processes
 
         for i, block in enumerate(blocks):
             items = [tuple(item) for sublist in block.tolist() for item in sublist]  # Flatten the sub-blocks
             self.job_qs[i].put(items)  # Put the flattened items in the job queue for the process
```

### Comparing `pyaugmecon-1.0.0/pyaugmecon/solver_process.py` & `pyaugmecon-1.0.1/pyaugmecon/solver_process.py`

 * *Files identical despite different names*

### Comparing `pyaugmecon-1.0.0/pyaugmecon.egg-info/PKG-INFO` & `pyaugmecon-1.0.1/pyaugmecon.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaugmecon
-Version: 1.0.0
+Version: 1.0.1
 Home-page: https://github.com/wouterbles/pyaugmecon
 Author: Wouter Bles
 Author-email: whbles@gmail.com
 License: MIT
 Project-URL: Changelog, https://github.com/wouterbles/pyaugmecon/blob/main/CHANGELOG.md
 Keywords: python,pyomo,optimization,multi-objective-optimization,augmecon
 Classifier: Development Status :: 3 - Alpha
@@ -347,14 +347,18 @@
 
 - Wouter Bles (current version of the package)
 - Nikolaos Paterakis (initial implementation)
 
 
 # Changelog
 
+## 1.0.1
+
+- Make QueueHandler work on MacOS #5, thanks @yvanoers
+
 ## 1.0.0
 
 - Add new methods for solution retrieval
 
 ## 0.2.1
 
 - Add Python 3.10 to supported versions
```

### Comparing `pyaugmecon-1.0.0/setup.py` & `pyaugmecon-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         + "\n\n"
         + (CURRENT_DIR / "CHANGELOG.md").read_text(encoding="utf8")
     )
 
 
 setup(
     name="pyaugmecon",
-    version="1.0.0",
+    version="1.0.1",
     author="Wouter Bles",
     author_email="whbles@gmail.com",
     long_description=get_long_description(),
     long_description_content_type="text/markdown",
     keywords="python, pyomo, optimization, multi-objective-optimization, augmecon",
     url="https://github.com/wouterbles/pyaugmecon",
     project_urls={"Changelog": "https://github.com/wouterbles/pyaugmecon/blob/main/CHANGELOG.md"},
```

