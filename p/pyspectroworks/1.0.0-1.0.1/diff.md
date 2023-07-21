# Comparing `tmp/pyspectroworks-1.0.0.tar.gz` & `tmp/pyspectroworks-1.0.1.tar.gz`

## Comparing `pyspectroworks-1.0.0.tar` & `pyspectroworks-1.0.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    76510 2020-02-02 00:00:00.000000 pyspectroworks-1.0.0/Demo-education.ipynb
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 pyspectroworks-1.0.0/api_test.py
--rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 pyspectroworks-1.0.0/environment.yml
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 pyspectroworks-1.0.0/requirements.txt
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 pyspectroworks-1.0.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 pyspectroworks-1.0.0/src/pyspectroworks/__init__.py
--rw-r--r--   0        0        0    10148 2020-02-02 00:00:00.000000 pyspectroworks-1.0.0/src/pyspectroworks/pyspectroworks.py
--rw-r--r--   0        0        0     2036 2020-02-02 00:00:00.000000 pyspectroworks-1.0.0/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 pyspectroworks-1.0.0/LICENSE
--rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 pyspectroworks-1.0.0/README.md
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 pyspectroworks-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     3641 2020-02-02 00:00:00.000000 pyspectroworks-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    76510 2020-02-02 00:00:00.000000 pyspectroworks-1.0.1/Demo-education.ipynb
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 pyspectroworks-1.0.1/api_test.py
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 pyspectroworks-1.0.1/environment.yml
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 pyspectroworks-1.0.1/requirements.txt
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 pyspectroworks-1.0.1/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 pyspectroworks-1.0.1/src/pyspectroworks/__init__.py
+-rw-r--r--   0        0        0    10148 2020-02-02 00:00:00.000000 pyspectroworks-1.0.1/src/pyspectroworks/pyspectroworks.py
+-rw-r--r--   0        0        0     2036 2020-02-02 00:00:00.000000 pyspectroworks-1.0.1/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 pyspectroworks-1.0.1/LICENSE
+-rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 pyspectroworks-1.0.1/README.md
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 pyspectroworks-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     3641 2020-02-02 00:00:00.000000 pyspectroworks-1.0.1/PKG-INFO
```

### Comparing `pyspectroworks-1.0.0/Demo-education.ipynb` & `pyspectroworks-1.0.1/Demo-education.ipynb`

 * *Files identical despite different names*

### Comparing `pyspectroworks-1.0.0/api_test.py` & `pyspectroworks-1.0.1/api_test.py`

 * *Files identical despite different names*

### Comparing `pyspectroworks-1.0.0/.github/workflows/python-publish.yml` & `pyspectroworks-1.0.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `pyspectroworks-1.0.0/src/pyspectroworks/pyspectroworks.py` & `pyspectroworks-1.0.1/src/pyspectroworks/pyspectroworks.py`

 * *Files identical despite different names*

### Comparing `pyspectroworks-1.0.0/.gitignore` & `pyspectroworks-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pyspectroworks-1.0.0/LICENSE` & `pyspectroworks-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyspectroworks-1.0.0/README.md` & `pyspectroworks-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pyspectroworks-1.0.0/pyproject.toml` & `pyspectroworks-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "pyspectroworks"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="Thomas Sørensen", email="thots@cphnano.com" },
 ]
 description = "pySpectroWorks is a Python module for loading data from SpectroWorks™."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `pyspectroworks-1.0.0/PKG-INFO` & `pyspectroworks-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyspectroworks
-Version: 1.0.0
+Version: 1.0.1
 Summary: pySpectroWorks is a Python module for loading data from SpectroWorks™.
 Project-URL: Homepage, https://github.com/cphnano/pySpectroWorks
 Project-URL: Bug Tracker, https://github.com/cphnano/pySpectroWorks/issues
 Author-email: Thomas Sørensen <thots@cphnano.com>
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

