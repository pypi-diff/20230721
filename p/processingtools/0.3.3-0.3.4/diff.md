# Comparing `tmp/processingtools-0.3.3.tar.gz` & `tmp/processingtools-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\processingtools-0.3.3.tar", last modified: Fri Jul 21 14:48:54 2023, max compression
+gzip compressed data, was "dist\processingtools-0.3.4.tar", last modified: Fri Jul 21 16:09:51 2023, max compression
```

## Comparing `processingtools-0.3.3.tar` & `processingtools-0.3.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-21 14:48:54.203144 processingtools-0.3.3/
--rw-rw-rw-   0        0        0     1085 2022-04-02 13:28:58.000000 processingtools-0.3.3/LICENSE
--rw-rw-rw-   0        0        0     2667 2023-07-21 14:48:54.202145 processingtools-0.3.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-21 14:48:54.194143 processingtools-0.3.3/ProcessingTools/
--rw-rw-rw-   0        0        0     8846 2023-07-21 14:46:58.000000 processingtools-0.3.3/ProcessingTools/EnvReco.py
--rw-rw-rw-   0        0        0     4829 2023-07-21 14:46:58.000000 processingtools-0.3.3/ProcessingTools/PrgressBar.py
--rw-rw-rw-   0        0        0      122 2023-06-23 14:29:11.000000 processingtools-0.3.3/ProcessingTools/__init__.py
--rw-rw-rw-   0        0        0     8357 2023-06-14 13:17:42.000000 processingtools-0.3.3/ProcessingTools/functions.py
--rw-rw-rw-   0        0        0    16364 2023-06-23 16:05:03.000000 processingtools-0.3.3/ProcessingTools/torch_tools.py
-drwxrwxrwx   0        0        0        0 2023-07-21 14:48:54.193143 processingtools-0.3.3/ProcessingTools.egg-info/
--rw-rw-rw-   0        0        0     2667 2023-07-21 14:48:53.000000 processingtools-0.3.3/ProcessingTools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      677 2023-07-21 14:48:53.000000 processingtools-0.3.3/ProcessingTools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 14:48:53.000000 processingtools-0.3.3/ProcessingTools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-07-21 14:48:53.000000 processingtools-0.3.3/ProcessingTools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-07-21 14:48:53.000000 processingtools-0.3.3/ProcessingTools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2190 2023-07-03 11:22:43.000000 processingtools-0.3.3/README.md
--rw-rw-rw-   0        0        0       42 2023-07-21 14:48:54.203144 processingtools-0.3.3/setup.cfg
--rw-rw-rw-   0        0        0      860 2023-07-21 14:48:28.000000 processingtools-0.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 16:09:51.845527 processingtools-0.3.4/
+-rw-rw-rw-   0        0        0     1085 2022-04-02 13:28:58.000000 processingtools-0.3.4/LICENSE
+-rw-rw-rw-   0        0        0     2667 2023-07-21 16:09:51.844525 processingtools-0.3.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-21 16:09:51.837526 processingtools-0.3.4/ProcessingTools/
+-rw-rw-rw-   0        0        0     8846 2023-07-21 14:46:58.000000 processingtools-0.3.4/ProcessingTools/EnvReco.py
+-rw-rw-rw-   0        0        0     4903 2023-07-21 16:09:36.000000 processingtools-0.3.4/ProcessingTools/PrgressBar.py
+-rw-rw-rw-   0        0        0      122 2023-06-23 14:29:11.000000 processingtools-0.3.4/ProcessingTools/__init__.py
+-rw-rw-rw-   0        0        0     8357 2023-06-14 13:17:42.000000 processingtools-0.3.4/ProcessingTools/functions.py
+-rw-rw-rw-   0        0        0    16364 2023-06-23 16:05:03.000000 processingtools-0.3.4/ProcessingTools/torch_tools.py
+drwxrwxrwx   0        0        0        0 2023-07-21 16:09:51.835525 processingtools-0.3.4/ProcessingTools.egg-info/
+-rw-rw-rw-   0        0        0     2667 2023-07-21 16:09:51.000000 processingtools-0.3.4/ProcessingTools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      677 2023-07-21 16:09:51.000000 processingtools-0.3.4/ProcessingTools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 16:09:51.000000 processingtools-0.3.4/ProcessingTools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-07-21 16:09:51.000000 processingtools-0.3.4/ProcessingTools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-07-21 16:09:51.000000 processingtools-0.3.4/ProcessingTools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2190 2023-07-03 11:22:43.000000 processingtools-0.3.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-21 16:09:51.845527 processingtools-0.3.4/setup.cfg
+-rw-rw-rw-   0        0        0      860 2023-07-21 16:09:36.000000 processingtools-0.3.4/setup.py
```

### Comparing `processingtools-0.3.3/LICENSE` & `processingtools-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `processingtools-0.3.3/PKG-INFO` & `processingtools-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: processingtools
-Version: 0.3.3
+Version: 0.3.4
 Summary: https://github.com/ysy9997/ProcessingTools.git
 Home-page: https://github.com/ysy9997/ProcessingTools.git
 Author: syy
 Author-email: ysy9997@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `processingtools-0.3.3/ProcessingTools/EnvReco.py` & `processingtools-0.3.4/ProcessingTools/EnvReco.py`

 * *Files identical despite different names*

### Comparing `processingtools-0.3.3/ProcessingTools/PrgressBar.py` & `processingtools-0.3.4/ProcessingTools/PrgressBar.py`

 * *Files 8% similar despite different names*

```diff
@@ -45,14 +45,16 @@
             self.length = max
         else:
             self.it, copy_it = itertools.tee(self.it)
             self.length = 0
             for _ in iter(copy_it): self.length = self.length + 1
 
         self.smoothing = self.length // 100 if smoothing is None else smoothing
+        self.smoothing = 10 if self.smoothing < 10 else self.smoothing
+
         self.take = np.zeros(self.smoothing, float)
         T = time.time()
         for i in range(self.smoothing): self.take[i] = T
 
     def __iter__(self):
         return self
```

### Comparing `processingtools-0.3.3/ProcessingTools/functions.py` & `processingtools-0.3.4/ProcessingTools/functions.py`

 * *Files identical despite different names*

### Comparing `processingtools-0.3.3/ProcessingTools/torch_tools.py` & `processingtools-0.3.4/ProcessingTools/torch_tools.py`

 * *Files identical despite different names*

### Comparing `processingtools-0.3.3/ProcessingTools.egg-info/PKG-INFO` & `processingtools-0.3.4/ProcessingTools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: processingtools
-Version: 0.3.3
+Version: 0.3.4
 Summary: https://github.com/ysy9997/ProcessingTools.git
 Home-page: https://github.com/ysy9997/ProcessingTools.git
 Author: syy
 Author-email: ysy9997@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `processingtools-0.3.3/ProcessingTools.egg-info/SOURCES.txt` & `processingtools-0.3.4/ProcessingTools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `processingtools-0.3.3/README.md` & `processingtools-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `processingtools-0.3.3/setup.py` & `processingtools-0.3.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding='UTF-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="processingtools",
-    version="0.3.3",
+    version="0.3.4",
     install_requires=['opencv-python>=4.5.5.62',
                       'numpy>=1.19.4',
                       'matplotlib>=3.3.3'],
     license='MIT',
     author="syy",
     author_email="ysy9997@gmail.com",
     description="https://github.com/ysy9997/ProcessingTools.git",
```

