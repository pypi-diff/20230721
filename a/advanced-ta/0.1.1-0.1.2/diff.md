# Comparing `tmp/advanced-ta-0.1.1.tar.gz` & `tmp/advanced-ta-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "advanced-ta-0.1.1.tar", max compression
+gzip compressed data, was "advanced-ta-0.1.2.tar", max compression
```

## Comparing `advanced-ta-0.1.1.tar` & `advanced-ta-0.1.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      562 2023-07-20 18:32:34.878723 advanced-ta-0.1.1/README.md
--rw-r--r--   0        0        0    26037 2023-07-20 19:33:10.956673 advanced-ta-0.1.1/advanced_ta/LorentzianClassification/Classifier.py
--rw-r--r--   0        0        0     2689 2023-07-20 17:14:25.348338 advanced-ta-0.1.1/advanced_ta/LorentzianClassification/KernelFunctions.py
--rw-r--r--   0        0        0     7252 2023-07-20 17:16:02.641151 advanced-ta-0.1.1/advanced_ta/LorentzianClassification/MLExtensions.py
--rw-r--r--   0        0        0     1891 2023-07-20 15:20:39.939402 advanced-ta-0.1.1/advanced_ta/LorentzianClassification/Types.py
--rw-r--r--   0        0        0       73 2023-07-20 15:29:10.313143 advanced-ta-0.1.1/advanced_ta/__init__.py
--rw-r--r--   0        0        0      581 2023-07-20 19:33:50.072998 advanced-ta-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1451 2023-07-20 19:34:16.618661 advanced-ta-0.1.1/setup.py
--rw-r--r--   0        0        0     1299 2023-07-20 19:34:16.618857 advanced-ta-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     2234 2023-07-20 22:06:54.818226 advanced-ta-0.1.2/README.md
+-rw-r--r--   0        0        0    26037 2023-07-20 21:47:44.968749 advanced-ta-0.1.2/advanced_ta/LorentzianClassification/Classifier.py
+-rw-r--r--   0        0        0     2689 2023-07-20 17:14:25.348338 advanced-ta-0.1.2/advanced_ta/LorentzianClassification/KernelFunctions.py
+-rw-r--r--   0        0        0     7252 2023-07-20 17:16:02.641151 advanced-ta-0.1.2/advanced_ta/LorentzianClassification/MLExtensions.py
+-rw-r--r--   0        0        0     1891 2023-07-20 15:20:39.939402 advanced-ta-0.1.2/advanced_ta/LorentzianClassification/Types.py
+-rw-r--r--   0        0        0       73 2023-07-20 15:29:10.313143 advanced-ta-0.1.2/advanced_ta/__init__.py
+-rw-r--r--   0        0        0      581 2023-07-20 22:11:02.592268 advanced-ta-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3215 2023-07-20 22:11:27.006567 advanced-ta-0.1.2/setup.py
+-rw-r--r--   0        0        0     2971 2023-07-20 22:11:27.006803 advanced-ta-0.1.2/PKG-INFO
```

### Comparing `advanced-ta-0.1.1/advanced_ta/LorentzianClassification/Classifier.py` & `advanced-ta-0.1.2/advanced_ta/LorentzianClassification/Classifier.py`

 * *Files identical despite different names*

### Comparing `advanced-ta-0.1.1/advanced_ta/LorentzianClassification/KernelFunctions.py` & `advanced-ta-0.1.2/advanced_ta/LorentzianClassification/KernelFunctions.py`

 * *Files identical despite different names*

### Comparing `advanced-ta-0.1.1/advanced_ta/LorentzianClassification/MLExtensions.py` & `advanced-ta-0.1.2/advanced_ta/LorentzianClassification/MLExtensions.py`

 * *Files identical despite different names*

### Comparing `advanced-ta-0.1.1/advanced_ta/LorentzianClassification/Types.py` & `advanced-ta-0.1.2/advanced_ta/LorentzianClassification/Types.py`

 * *Files identical despite different names*

### Comparing `advanced-ta-0.1.1/pyproject.toml` & `advanced-ta-0.1.2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "advanced-ta"
-version = "0.1.1"
+version = "0.1.2"
 description = "Python implementation of Lorentzian Classification algorithm."
 authors = ["Loki Arya <loki.arya+osdev@gmail.com>"]
 readme = "README.md"
 repository = "https://bitbucket.org/lokiarya/advanced-ta"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

