# Comparing `tmp/scheduling_utils-0.1.1.tar.gz` & `tmp/scheduling_utils-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scheduling_utils-0.1.1.tar", last modified: Tue May  2 07:08:48 2023, max compression
+gzip compressed data, was "scheduling_utils-0.1.2.tar", last modified: Fri Jul 21 17:47:04 2023, max compression
```

## Comparing `scheduling_utils-0.1.1.tar` & `scheduling_utils-0.1.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 dserez    (1001) dserez    (1001)        0 2023-05-02 07:08:48.048241 scheduling_utils-0.1.1/
--rw-rw-r--   0 dserez    (1001) dserez    (1001)     1063 2023-01-24 12:20:04.000000 scheduling_utils-0.1.1/LICENSE
--rw-rw-r--   0 dserez    (1001) dserez    (1001)       38 2023-02-03 09:13:57.000000 scheduling_utils-0.1.1/MANIFEST.in
--rw-rw-r--   0 dserez    (1001) dserez    (1001)     1060 2023-05-02 07:08:48.048241 scheduling_utils-0.1.1/PKG-INFO
--rw-rw-r--   0 dserez    (1001) dserez    (1001)      801 2023-05-02 07:05:00.000000 scheduling_utils-0.1.1/README.md
-drwxrwxr-x   0 dserez    (1001) dserez    (1001)        0 2023-05-02 07:08:48.048241 scheduling_utils-0.1.1/images/
--rw-rw-r--   0 dserez    (1001) dserez    (1001)    15837 2023-02-03 08:45:24.000000 scheduling_utils-0.1.1/images/cosine_decay.png
--rw-rw-r--   0 dserez    (1001) dserez    (1001)    15046 2023-02-03 08:47:14.000000 scheduling_utils-0.1.1/images/cosine_ramp.png
--rw-rw-r--   0 dserez    (1001) dserez    (1001)    22196 2023-05-02 06:58:05.000000 scheduling_utils-0.1.1/images/linear_cosine.png
--rw-rw-r--   0 dserez    (1001) dserez    (1001)    16089 2023-02-03 08:45:56.000000 scheduling_utils-0.1.1/images/linear_decay.png
--rw-rw-r--   0 dserez    (1001) dserez    (1001)    14761 2023-02-03 08:47:45.000000 scheduling_utils-0.1.1/images/linear_ramp.png
-drwxrwxr-x   0 dserez    (1001) dserez    (1001)        0 2023-05-02 07:08:48.048241 scheduling_utils-0.1.1/scheduling_utils/
--rw-rw-r--   0 dserez    (1001) dserez    (1001)        0 2023-01-09 07:27:26.000000 scheduling_utils-0.1.1/scheduling_utils/__init__.py
--rw-rw-r--   0 dserez    (1001) dserez    (1001)     3190 2023-05-02 06:56:13.000000 scheduling_utils-0.1.1/scheduling_utils/schedulers.py
--rw-rw-r--   0 dserez    (1001) dserez    (1001)     1922 2023-05-02 07:05:10.000000 scheduling_utils-0.1.1/scheduling_utils/test.py
-drwxrwxr-x   0 dserez    (1001) dserez    (1001)        0 2023-05-02 07:08:48.048241 scheduling_utils-0.1.1/scheduling_utils.egg-info/
--rw-rw-r--   0 dserez    (1001) dserez    (1001)     1060 2023-05-02 07:08:48.000000 scheduling_utils-0.1.1/scheduling_utils.egg-info/PKG-INFO
--rw-rw-r--   0 dserez    (1001) dserez    (1001)      441 2023-05-02 07:08:48.000000 scheduling_utils-0.1.1/scheduling_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 dserez    (1001) dserez    (1001)        1 2023-05-02 07:08:48.000000 scheduling_utils-0.1.1/scheduling_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 dserez    (1001) dserez    (1001)        1 2023-02-03 09:24:34.000000 scheduling_utils-0.1.1/scheduling_utils.egg-info/not-zip-safe
--rw-rw-r--   0 dserez    (1001) dserez    (1001)       17 2023-05-02 07:08:48.000000 scheduling_utils-0.1.1/scheduling_utils.egg-info/top_level.txt
--rw-rw-r--   0 dserez    (1001) dserez    (1001)       38 2023-05-02 07:08:48.048241 scheduling_utils-0.1.1/setup.cfg
--rw-rw-r--   0 dserez    (1001) dserez    (1001)      574 2023-05-02 07:08:46.000000 scheduling_utils-0.1.1/setup.py
+drwxrwxr-x   0 dserez    (1001) dserez    (1001)        0 2023-07-21 17:47:04.006075 scheduling_utils-0.1.2/
+-rw-rw-r--   0 dserez    (1001) dserez    (1001)     1063 2023-01-24 12:20:04.000000 scheduling_utils-0.1.2/LICENSE
+-rw-rw-r--   0 dserez    (1001) dserez    (1001)       38 2023-02-03 09:13:57.000000 scheduling_utils-0.1.2/MANIFEST.in
+-rw-rw-r--   0 dserez    (1001) dserez    (1001)     1060 2023-07-21 17:47:04.006075 scheduling_utils-0.1.2/PKG-INFO
+-rw-rw-r--   0 dserez    (1001) dserez    (1001)      801 2023-05-02 07:05:00.000000 scheduling_utils-0.1.2/README.md
+drwxrwxr-x   0 dserez    (1001) dserez    (1001)        0 2023-07-21 17:47:04.002075 scheduling_utils-0.1.2/images/
+-rw-rw-r--   0 dserez    (1001) dserez    (1001)    18198 2023-07-21 14:49:59.000000 scheduling_utils-0.1.2/images/cosine_decay.png
+-rw-rw-r--   0 dserez    (1001) dserez    (1001)    14689 2023-07-21 14:50:21.000000 scheduling_utils-0.1.2/images/cosine_ramp.png
+-rw-rw-r--   0 dserez    (1001) dserez    (1001)    22922 2023-07-21 17:43:23.000000 scheduling_utils-0.1.2/images/linear_cosine.png
+-rw-rw-r--   0 dserez    (1001) dserez    (1001)    16089 2023-02-03 08:45:56.000000 scheduling_utils-0.1.2/images/linear_decay.png
+-rw-rw-r--   0 dserez    (1001) dserez    (1001)    14761 2023-02-03 08:47:45.000000 scheduling_utils-0.1.2/images/linear_ramp.png
+drwxrwxr-x   0 dserez    (1001) dserez    (1001)        0 2023-07-21 17:47:04.002075 scheduling_utils-0.1.2/scheduling_utils/
+-rw-rw-r--   0 dserez    (1001) dserez    (1001)        0 2023-01-09 07:27:26.000000 scheduling_utils-0.1.2/scheduling_utils/__init__.py
+-rw-rw-r--   0 dserez    (1001) dserez    (1001)     3405 2023-07-21 17:41:52.000000 scheduling_utils-0.1.2/scheduling_utils/schedulers.py
+-rw-rw-r--   0 dserez    (1001) dserez    (1001)     1922 2023-07-21 17:42:18.000000 scheduling_utils-0.1.2/scheduling_utils/test.py
+drwxrwxr-x   0 dserez    (1001) dserez    (1001)        0 2023-07-21 17:47:04.006075 scheduling_utils-0.1.2/scheduling_utils.egg-info/
+-rw-rw-r--   0 dserez    (1001) dserez    (1001)     1060 2023-07-21 17:47:03.000000 scheduling_utils-0.1.2/scheduling_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 dserez    (1001) dserez    (1001)      441 2023-07-21 17:47:03.000000 scheduling_utils-0.1.2/scheduling_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 dserez    (1001) dserez    (1001)        1 2023-07-21 17:47:03.000000 scheduling_utils-0.1.2/scheduling_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 dserez    (1001) dserez    (1001)        1 2023-07-21 17:47:03.000000 scheduling_utils-0.1.2/scheduling_utils.egg-info/not-zip-safe
+-rw-rw-r--   0 dserez    (1001) dserez    (1001)       17 2023-07-21 17:47:03.000000 scheduling_utils-0.1.2/scheduling_utils.egg-info/top_level.txt
+-rw-rw-r--   0 dserez    (1001) dserez    (1001)       38 2023-07-21 17:47:04.006075 scheduling_utils-0.1.2/setup.cfg
+-rw-rw-r--   0 dserez    (1001) dserez    (1001)      574 2023-07-21 17:44:56.000000 scheduling_utils-0.1.2/setup.py
```

### Comparing `scheduling_utils-0.1.1/LICENSE` & `scheduling_utils-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `scheduling_utils-0.1.1/PKG-INFO` & `scheduling_utils-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scheduling_utils
-Version: 0.1.1
+Version: 0.1.2
 Summary: implementation of scheduling function utils
 Home-page: https://github.com/SerezD/scheduling_utils
 Author: DSerez
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `scheduling_utils-0.1.1/README.md` & `scheduling_utils-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `scheduling_utils-0.1.1/images/linear_decay.png` & `scheduling_utils-0.1.2/images/linear_decay.png`

 * *Files identical despite different names*

### Comparing `scheduling_utils-0.1.1/images/linear_ramp.png` & `scheduling_utils-0.1.2/images/linear_ramp.png`

 * *Files identical despite different names*

### Comparing `scheduling_utils-0.1.1/scheduling_utils/schedulers.py` & `scheduling_utils-0.1.2/scheduling_utils/schedulers.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,19 +26,20 @@
 
     @abstractmethod
     def warp_func(self, perc_step: float):
         pass
 
     def _get_perc_step(self, step: int):
 
-        # step normalized in 0_1 range
+        # get step normalized in 0_1 range
         return max(0, min(1, (step - self._start_step) / (self._stop_step - self._start_step)))
 
     def _get_value(self, perc_step: float):
-        return perc_step * self._stop_value + (1 - perc_step) * self._start_value
+        # get value at perc_step
+        return self._start_value + (self._stop_value - self._start_value) * perc_step
 
     def step(self, step: int):
 
         # step normalized in 0_1 range
         perc_step = self._get_perc_step(step)
 
         # warp perc according to scheduler type
@@ -51,15 +52,18 @@
 
     def __init__(self, start_step: int, stop_step: int, start_value: float, stop_value: float):
         super().__init__(start_step, stop_step, start_value, stop_value)
 
     def warp_func(self, perc_step: float):
 
         # warp with cosine
-        return 1.0 - math.cos(perc_step * math.pi / 2)
+        # math.cos(math.pi * perc_step) goes from 1 to -1
+        # sum 1 and mul 0.5 to normalize
+        # then reverse since you still want a perc step as output
+        return 1 - (0.5 * (1. + math.cos(math.pi * perc_step)))
 
 
 class LinearScheduler(Scheduler):
 
     def __init__(self, start_step: int, stop_step: int, start_value: float, stop_value: float):
         super().__init__(start_step, stop_step, start_value, stop_value)
```

### Comparing `scheduling_utils-0.1.1/scheduling_utils/test.py` & `scheduling_utils-0.1.2/scheduling_utils/test.py`

 * *Files identical despite different names*

### Comparing `scheduling_utils-0.1.1/scheduling_utils.egg-info/PKG-INFO` & `scheduling_utils-0.1.2/scheduling_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scheduling-utils
-Version: 0.1.1
+Version: 0.1.2
 Summary: implementation of scheduling function utils
 Home-page: https://github.com/SerezD/scheduling_utils
 Author: DSerez
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `scheduling_utils-0.1.1/setup.py` & `scheduling_utils-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 
 setup(name='scheduling_utils',
-      version='0.1.1',
+      version='0.1.2',
       description='implementation of scheduling function utils',
       long_description=long_description,
       long_description_content_type='text/markdown',
       url='https://github.com/SerezD/scheduling_utils',
       author='DSerez',
       license='MIT',
       packages=find_packages(),
```

