# Comparing `tmp/nhs_number-1.3.3.tar.gz` & `tmp/nhs_number-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nhs_number-1.3.3.tar", max compression
+gzip compressed data, was "nhs_number-1.3.4.tar", max compression
```

## Comparing `nhs_number-1.3.3.tar` & `nhs_number-1.3.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1097 2023-06-13 13:54:57.104990 nhs_number-1.3.3/LICENSE
--rw-r--r--   0        0        0     1301 2023-06-13 13:54:57.104990 nhs_number-1.3.3/README.md
--rw-r--r--   0        0        0      779 2023-06-13 13:54:57.108990 nhs_number-1.3.3/nhs_number/__init__.py
--rw-r--r--   0        0        0     5081 2023-06-13 13:54:57.108990 nhs_number-1.3.3/nhs_number/constants.py
--rw-r--r--   0        0        0     2701 2023-06-13 13:54:57.108990 nhs_number-1.3.3/nhs_number/details.py
--rw-r--r--   0        0        0     2438 2023-06-13 13:54:57.108990 nhs_number-1.3.3/nhs_number/generate.py
--rw-r--r--   0        0        0     1814 2023-06-13 13:54:57.108990 nhs_number-1.3.3/nhs_number/standardise.py
--rw-r--r--   0        0        0     2733 2023-06-13 13:54:57.108990 nhs_number-1.3.3/nhs_number/validate.py
--rw-r--r--   0        0        0     1585 2023-06-13 13:54:57.108990 nhs_number-1.3.3/pyproject.toml
--rw-r--r--   0        0        0     2606 1970-01-01 00:00:00.000000 nhs_number-1.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1097 2023-07-21 11:21:44.694488 nhs_number-1.3.4/LICENSE
+-rw-r--r--   0        0        0     1301 2023-07-21 11:21:44.694488 nhs_number-1.3.4/README.md
+-rw-r--r--   0        0        0      779 2023-07-21 11:21:44.694488 nhs_number-1.3.4/nhs_number/__init__.py
+-rw-r--r--   0        0        0     5081 2023-07-21 11:21:44.694488 nhs_number-1.3.4/nhs_number/constants.py
+-rw-r--r--   0        0        0     2701 2023-07-21 11:21:44.694488 nhs_number-1.3.4/nhs_number/details.py
+-rw-r--r--   0        0        0     2438 2023-07-21 11:21:44.694488 nhs_number-1.3.4/nhs_number/generate.py
+-rw-r--r--   0        0        0     1814 2023-07-21 11:21:44.694488 nhs_number-1.3.4/nhs_number/standardise.py
+-rw-r--r--   0        0        0     2733 2023-07-21 11:21:44.694488 nhs_number-1.3.4/nhs_number/validate.py
+-rw-r--r--   0        0        0     1585 2023-07-21 11:21:44.694488 nhs_number-1.3.4/pyproject.toml
+-rw-r--r--   0        0        0     2606 1970-01-01 00:00:00.000000 nhs_number-1.3.4/PKG-INFO
```

### Comparing `nhs_number-1.3.3/LICENSE` & `nhs_number-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nhs_number-1.3.3/README.md` & `nhs_number-1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `nhs_number-1.3.3/nhs_number/__init__.py` & `nhs_number-1.3.4/nhs_number/__init__.py`

 * *Files identical despite different names*

### Comparing `nhs_number-1.3.3/nhs_number/constants.py` & `nhs_number-1.3.4/nhs_number/constants.py`

 * *Files identical despite different names*

### Comparing `nhs_number-1.3.3/nhs_number/details.py` & `nhs_number-1.3.4/nhs_number/details.py`

 * *Files identical despite different names*

### Comparing `nhs_number-1.3.3/nhs_number/generate.py` & `nhs_number-1.3.4/nhs_number/generate.py`

 * *Files identical despite different names*

### Comparing `nhs_number-1.3.3/nhs_number/standardise.py` & `nhs_number-1.3.4/nhs_number/standardise.py`

 * *Files identical despite different names*

### Comparing `nhs_number-1.3.3/nhs_number/validate.py` & `nhs_number-1.3.4/nhs_number/validate.py`

 * *Files identical despite different names*

### Comparing `nhs_number-1.3.3/pyproject.toml` & `nhs_number-1.3.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nhs-number"
-version = "1.3.3"
+version = "1.3.4"
 description = "Python package to provide utilities for NHS Numbers, including validity checks, normalisation, and generation."
 authors = [
     "Andy Law <andy.law@roslin.ed.ac.uk>",
     "Marcus Baw <marcusbaw@gmail.com>",
     ]
 license = "MIT"
 readme = "README.md"
```

### Comparing `nhs_number-1.3.3/PKG-INFO` & `nhs_number-1.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nhs-number
-Version: 1.3.3
+Version: 1.3.4
 Summary: Python package to provide utilities for NHS Numbers, including validity checks, normalisation, and generation.
 Home-page: https://nhs-number.uk-fci.tech/
 License: MIT
 Author: Andy Law
 Author-email: andy.law@roslin.ed.ac.uk
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nhs-number Version: 1.3.3 Summary: Python package
+Metadata-Version: 2.1 Name: nhs-number Version: 1.3.4 Summary: Python package
 to provide utilities for NHS Numbers, including validity checks, normalisation,
 and generation. Home-page: https://nhs-number.uk-fci.tech/ License: MIT Author:
 Andy Law Author-email: andy.law@roslin.ed.ac.uk Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: Healthcare Industry
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
```

