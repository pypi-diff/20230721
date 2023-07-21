# Comparing `tmp/fileformats_extras-0.1.1.tar.gz` & `tmp/fileformats_extras-0.2.0.tar.gz`

## Comparing `fileformats_extras-0.1.1.tar` & `fileformats_extras-0.2.0.tar`

### file list

```diff
@@ -1,24 +1,25 @@
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 fileformats_extras-0.1.1/.codespell-ignorewords
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 fileformats_extras-0.1.1/.flake8
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 fileformats_extras-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 fileformats_extras-0.1.1/conftest.py
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 fileformats_extras-0.1.1/pytest.ini
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 fileformats_extras-0.1.1/.github/workflows/publish.yml
--rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 fileformats_extras-0.1.1/.github/workflows/tests.yml
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 fileformats_extras-0.1.1/fileformats/extras/archive/__init__.py
--rw-r--r--   0        0        0     8869 2020-02-02 00:00:00.000000 fileformats_extras-0.1.1/fileformats/extras/archive/converters.py
--rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 fileformats_extras-0.1.1/fileformats/extras/archive/tests/test_archive_converters.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 fileformats_extras-0.1.1/fileformats/extras/core/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 fileformats_extras-0.1.1/fileformats/extras/core/_version.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 fileformats_extras-0.1.1/fileformats/extras/image/__init__.py
--rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 fileformats_extras-0.1.1/fileformats/extras/image/converters.py
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 fileformats_extras-0.1.1/fileformats/extras/image/readwrite.py
--rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 fileformats_extras-0.1.1/fileformats/extras/image/tests/test_image_converters.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 fileformats_extras-0.1.1/fileformats/extras/serialization/__init__.py
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 fileformats_extras-0.1.1/fileformats/extras/serialization/converters.py
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 fileformats_extras-0.1.1/fileformats/extras/serialization/tests/test_serialization_converters.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 fileformats_extras-0.1.1/.gitignore
--rw-r--r--   0        0        0    14222 2020-02-02 00:00:00.000000 fileformats_extras-0.1.1/LICENSE
--rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 fileformats_extras-0.1.1/README.rst
--rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 fileformats_extras-0.1.1/pyproject.toml
--rw-r--r--   0        0        0    18214 2020-02-02 00:00:00.000000 fileformats_extras-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 fileformats_extras-0.2.0/.codespell-ignorewords
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 fileformats_extras-0.2.0/.flake8
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 fileformats_extras-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 fileformats_extras-0.2.0/conftest.py
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 fileformats_extras-0.2.0/pytest.ini
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 fileformats_extras-0.2.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 fileformats_extras-0.2.0/.github/workflows/tests.yml
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 fileformats_extras-0.2.0/fileformats/extras/archive/__init__.py
+-rw-r--r--   0        0        0     8869 2020-02-02 00:00:00.000000 fileformats_extras-0.2.0/fileformats/extras/archive/converters.py
+-rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 fileformats_extras-0.2.0/fileformats/extras/archive/tests/test_archive_converters.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 fileformats_extras-0.2.0/fileformats/extras/core/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 fileformats_extras-0.2.0/fileformats/extras/core/_version.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 fileformats_extras-0.2.0/fileformats/extras/image/__init__.py
+-rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 fileformats_extras-0.2.0/fileformats/extras/image/converters.py
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 fileformats_extras-0.2.0/fileformats/extras/image/readwrite.py
+-rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 fileformats_extras-0.2.0/fileformats/extras/image/tests/test_image_converters.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 fileformats_extras-0.2.0/fileformats/extras/serialization/__init__.py
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 fileformats_extras-0.2.0/fileformats/extras/serialization/converters.py
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 fileformats_extras-0.2.0/fileformats/extras/serialization/yaml.py
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 fileformats_extras-0.2.0/fileformats/extras/serialization/tests/test_serialization_converters.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 fileformats_extras-0.2.0/.gitignore
+-rw-r--r--   0        0        0    14222 2020-02-02 00:00:00.000000 fileformats_extras-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 fileformats_extras-0.2.0/README.rst
+-rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 fileformats_extras-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0    18191 2020-02-02 00:00:00.000000 fileformats_extras-0.2.0/PKG-INFO
```

### Comparing `fileformats_extras-0.1.1/.pre-commit-config.yaml` & `fileformats_extras-0.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `fileformats_extras-0.1.1/conftest.py` & `fileformats_extras-0.2.0/conftest.py`

 * *Files identical despite different names*

### Comparing `fileformats_extras-0.1.1/.github/workflows/publish.yml` & `fileformats_extras-0.2.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `fileformats_extras-0.1.1/.github/workflows/tests.yml` & `fileformats_extras-0.2.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `fileformats_extras-0.1.1/fileformats/extras/archive/converters.py` & `fileformats_extras-0.2.0/fileformats/extras/archive/converters.py`

 * *Files identical despite different names*

### Comparing `fileformats_extras-0.1.1/fileformats/extras/archive/tests/test_archive_converters.py` & `fileformats_extras-0.2.0/fileformats/extras/archive/tests/test_archive_converters.py`

 * *Files identical despite different names*

### Comparing `fileformats_extras-0.1.1/fileformats/extras/image/converters.py` & `fileformats_extras-0.2.0/fileformats/extras/image/converters.py`

 * *Files identical despite different names*

### Comparing `fileformats_extras-0.1.1/fileformats/extras/image/tests/test_image_converters.py` & `fileformats_extras-0.2.0/fileformats/extras/image/tests/test_image_converters.py`

 * *Files identical despite different names*

### Comparing `fileformats_extras-0.1.1/fileformats/extras/serialization/converters.py` & `fileformats_extras-0.2.0/fileformats/extras/serialization/converters.py`

 * *Files identical despite different names*

### Comparing `fileformats_extras-0.1.1/fileformats/extras/serialization/tests/test_serialization_converters.py` & `fileformats_extras-0.2.0/fileformats/extras/serialization/tests/test_serialization_converters.py`

 * *Files identical despite different names*

### Comparing `fileformats_extras-0.1.1/LICENSE` & `fileformats_extras-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fileformats_extras-0.1.1/README.rst` & `fileformats_extras-0.2.0/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 FileFormats Extras
 ==================
 .. image:: https://github.com/arcanaframework/fileformats-extras/actions/workflows/tests.yml/badge.svg
     :target: https://github.com/arcanaframework/fileformats-extras/actions/workflows/tests.yml
 .. image:: https://codecov.io/gh/arcanaframework/fileformats-extras/branch/main/graph/badge.svg?token=UIS0OGPST7
     :target: https://codecov.io/gh/arcanaframework/fileformats-extras
-.. image:: https://img.shields.io/github/stars/ArcanaFramework/fileformats-extras.svg
-    :alt: GitHub stars
-    :target: https://github.com/ArcanaFramework/fileformats-extras
+.. image:: https://img.shields.io/pypi/v/fileformats-extras.svg
+   :target: https://pypi.python.org/pypi/fileformats-extras/
+   :alt: Latest Version    
 .. image:: https://img.shields.io/badge/docs-latest-brightgreen.svg?style=flat
     :target: https://arcanaframework.github.io/fileformats/
     :alt: Documentation Status
 
 
 This is a extras module for the
 `fileformats <https://github.com/ArcanaFramework/fileformats>`__ package, which provides
```

### Comparing `fileformats_extras-0.1.1/pyproject.toml` & `fileformats_extras-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fileformats_extras-0.1.1/PKG-INFO` & `fileformats_extras-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fileformats-extras
-Version: 0.1.1
+Version: 0.2.0
 Summary: Classes for representing different file formats in Python classes for use in type hinting in data workflows
 Project-URL: repository, https://github.com/ArcanaFramework/fileformats-extras
 Author-email: "Thomas G. Close" <tom.g.close@gmail.com>
 Maintainer-email: "Thomas G. Close" <tom.g.close@gmail.com>
 License: Creative Commons Attribution 4.0 International Public License
         By exercising the Licensed Rights (defined below), You accept and agree to be bound by the terms and conditions of this Creative Commons Attribution 4.0 International Public License ("Public License"). To the extent this Public License may be interpreted as a contract, You are granted the Licensed Rights in consideration of Your acceptance of these terms and conditions, and the Licensor grants You such rights in consideration of benefits the Licensor receives from making the Licensed Material available under these terms and conditions.
         
@@ -131,17 +131,17 @@
 
 FileFormats Extras
 ==================
 .. image:: https://github.com/arcanaframework/fileformats-extras/actions/workflows/tests.yml/badge.svg
     :target: https://github.com/arcanaframework/fileformats-extras/actions/workflows/tests.yml
 .. image:: https://codecov.io/gh/arcanaframework/fileformats-extras/branch/main/graph/badge.svg?token=UIS0OGPST7
     :target: https://codecov.io/gh/arcanaframework/fileformats-extras
-.. image:: https://img.shields.io/github/stars/ArcanaFramework/fileformats-extras.svg
-    :alt: GitHub stars
-    :target: https://github.com/ArcanaFramework/fileformats-extras
+.. image:: https://img.shields.io/pypi/v/fileformats-extras.svg
+   :target: https://pypi.python.org/pypi/fileformats-extras/
+   :alt: Latest Version    
 .. image:: https://img.shields.io/badge/docs-latest-brightgreen.svg?style=flat
     :target: https://arcanaframework.github.io/fileformats/
     :alt: Documentation Status
 
 
 This is a extras module for the
 `fileformats <https://github.com/ArcanaFramework/fileformats>`__ package, which provides
```

