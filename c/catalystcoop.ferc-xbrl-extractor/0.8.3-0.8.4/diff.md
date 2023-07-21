# Comparing `tmp/catalystcoop.ferc_xbrl_extractor-0.8.3.tar.gz` & `tmp/catalystcoop.ferc_xbrl_extractor-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "catalystcoop.ferc_xbrl_extractor-0.8.3.tar", last modified: Fri Jun 16 16:35:09 2023, max compression
+gzip compressed data, was "catalystcoop.ferc_xbrl_extractor-0.8.4.tar", last modified: Fri Jul 21 17:58:28 2023, max compression
```

## Comparing `catalystcoop.ferc_xbrl_extractor-0.8.3.tar` & `catalystcoop.ferc_xbrl_extractor-0.8.4.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 zane      (1000) staff       (20)        0 2023-06-16 16:35:09.820656 catalystcoop.ferc_xbrl_extractor-0.8.3/
--rw-r--r--   0 zane      (1000) staff       (20)     1077 2022-09-06 23:55:13.000000 catalystcoop.ferc_xbrl_extractor-0.8.3/LICENSE.txt
--rw-r--r--   0 zane      (1000) staff       (20)      160 2023-04-04 18:48:48.000000 catalystcoop.ferc_xbrl_extractor-0.8.3/MANIFEST.in
--rw-r--r--   0 zane      (1000) staff       (20)    11285 2023-06-16 16:35:09.820456 catalystcoop.ferc_xbrl_extractor-0.8.3/PKG-INFO
--rw-r--r--   0 zane      (1000) staff       (20)     8765 2022-12-21 05:42:16.000000 catalystcoop.ferc_xbrl_extractor-0.8.3/README.rst
--rw-r--r--   0 zane      (1000) staff       (20)      269 2023-04-04 18:48:48.000000 catalystcoop.ferc_xbrl_extractor-0.8.3/environment.yml
--rw-r--r--   0 zane      (1000) staff       (20)     3933 2023-06-16 16:28:06.000000 catalystcoop.ferc_xbrl_extractor-0.8.3/pyproject.toml
--rw-r--r--   0 zane      (1000) staff       (20)       38 2023-06-16 16:35:09.820693 catalystcoop.ferc_xbrl_extractor-0.8.3/setup.cfg
-drwxr-xr-x   0 zane      (1000) staff       (20)        0 2023-06-16 16:35:09.807791 catalystcoop.ferc_xbrl_extractor-0.8.3/src/
-drwxr-xr-x   0 zane      (1000) staff       (20)        0 2023-06-16 16:35:09.809422 catalystcoop.ferc_xbrl_extractor-0.8.3/src/catalystcoop.ferc_xbrl_extractor.egg-info/
--rw-r--r--   0 zane      (1000) staff       (20)    11285 2023-06-16 16:35:09.000000 catalystcoop.ferc_xbrl_extractor-0.8.3/src/catalystcoop.ferc_xbrl_extractor.egg-info/PKG-INFO
--rw-r--r--   0 zane      (1000) staff       (20)      952 2023-06-16 16:35:09.000000 catalystcoop.ferc_xbrl_extractor-0.8.3/src/catalystcoop.ferc_xbrl_extractor.egg-info/SOURCES.txt
--rw-r--r--   0 zane      (1000) staff       (20)        1 2023-06-16 16:35:09.000000 catalystcoop.ferc_xbrl_extractor-0.8.3/src/catalystcoop.ferc_xbrl_extractor.egg-info/dependency_links.txt
--rw-r--r--   0 zane      (1000) staff       (20)       62 2023-06-16 16:35:09.000000 catalystcoop.ferc_xbrl_extractor-0.8.3/src/catalystcoop.ferc_xbrl_extractor.egg-info/entry_points.txt
--rw-r--r--   0 zane      (1000) staff       (20)      830 2023-06-16 16:35:09.000000 catalystcoop.ferc_xbrl_extractor-0.8.3/src/catalystcoop.ferc_xbrl_extractor.egg-info/requires.txt
--rw-r--r--   0 zane      (1000) staff       (20)       20 2023-06-16 16:35:09.000000 catalystcoop.ferc_xbrl_extractor-0.8.3/src/catalystcoop.ferc_xbrl_extractor.egg-info/top_level.txt
-drwxr-xr-x   0 zane      (1000) staff       (20)        0 2023-06-16 16:35:09.819261 catalystcoop.ferc_xbrl_extractor-0.8.3/src/ferc_xbrl_extractor/
--rw-r--r--   0 zane      (1000) staff       (20)      117 2022-09-06 23:55:13.000000 catalystcoop.ferc_xbrl_extractor-0.8.3/src/ferc_xbrl_extractor/__init__.py
--rw-r--r--   0 zane      (1000) staff       (20)     5319 2022-12-20 22:44:44.000000 catalystcoop.ferc_xbrl_extractor-0.8.3/src/ferc_xbrl_extractor/arelle_interface.py
--rw-r--r--   0 zane      (1000) staff       (20)     6629 2022-12-09 18:37:59.000000 catalystcoop.ferc_xbrl_extractor-0.8.3/src/ferc_xbrl_extractor/cli.py
--rw-r--r--   0 zane      (1000) staff       (20)    14161 2022-12-09 18:37:59.000000 catalystcoop.ferc_xbrl_extractor-0.8.3/src/ferc_xbrl_extractor/datapackage.py
--rw-r--r--   0 zane      (1000) staff       (20)      911 2022-09-06 23:55:13.000000 catalystcoop.ferc_xbrl_extractor-0.8.3/src/ferc_xbrl_extractor/helpers.py
--rw-r--r--   0 zane      (1000) staff       (20)    12367 2022-12-07 15:37:36.000000 catalystcoop.ferc_xbrl_extractor-0.8.3/src/ferc_xbrl_extractor/instance.py
--rw-r--r--   0 zane      (1000) staff       (20)    10910 2022-12-20 22:44:44.000000 catalystcoop.ferc_xbrl_extractor-0.8.3/src/ferc_xbrl_extractor/taxonomy.py
--rw-r--r--   0 zane      (1000) staff       (20)     7723 2022-12-09 18:37:59.000000 catalystcoop.ferc_xbrl_extractor-0.8.3/src/ferc_xbrl_extractor/xbrl.py
-drwxr-xr-x   0 zane      (1000) staff       (20)        0 2023-06-16 16:35:09.819488 catalystcoop.ferc_xbrl_extractor-0.8.3/tests/
--rw-r--r--   0 zane      (1000) staff       (20)       44 2022-09-06 23:55:13.000000 catalystcoop.ferc_xbrl_extractor-0.8.3/tests/__init__.py
--rw-r--r--   0 zane      (1000) staff       (20)      998 2022-09-06 23:55:13.000000 catalystcoop.ferc_xbrl_extractor-0.8.3/tests/conftest.py
-drwxr-xr-x   0 zane      (1000) staff       (20)        0 2023-06-16 16:35:09.819835 catalystcoop.ferc_xbrl_extractor-0.8.3/tests/integration/
--rw-r--r--   0 zane      (1000) staff       (20)       82 2022-09-06 23:55:13.000000 catalystcoop.ferc_xbrl_extractor-0.8.3/tests/integration/__init__.py
--rw-r--r--   0 zane      (1000) staff       (20)     1477 2022-12-20 22:44:44.000000 catalystcoop.ferc_xbrl_extractor-0.8.3/tests/integration/console_scripts_test.py
--rw-r--r--   0 zane      (1000) staff       (20)      672 2022-09-06 23:55:13.000000 catalystcoop.ferc_xbrl_extractor-0.8.3/tests/integration/datapackage_test.py
-drwxr-xr-x   0 zane      (1000) staff       (20)        0 2023-06-16 16:35:09.820203 catalystcoop.ferc_xbrl_extractor-0.8.3/tests/unit/
--rw-r--r--   0 zane      (1000) staff       (20)       84 2022-09-06 23:55:13.000000 catalystcoop.ferc_xbrl_extractor-0.8.3/tests/unit/__init__.py
--rw-r--r--   0 zane      (1000) staff       (20)     5641 2022-09-06 23:55:13.000000 catalystcoop.ferc_xbrl_extractor-0.8.3/tests/unit/datapackage_test.py
--rw-r--r--   0 zane      (1000) staff       (20)     3761 2022-09-06 23:55:13.000000 catalystcoop.ferc_xbrl_extractor-0.8.3/tests/unit/instance_test.py
--rw-r--r--   0 zane      (1000) staff       (20)     6879 2023-06-16 16:20:47.000000 catalystcoop.ferc_xbrl_extractor-0.8.3/tox.ini
+drwxr-xr-x   0 zane      (1000) staff       (20)        0 2023-07-21 17:58:28.166754 catalystcoop.ferc_xbrl_extractor-0.8.4/
+-rw-r--r--   0 zane      (1000) staff       (20)     1077 2022-09-06 23:55:13.000000 catalystcoop.ferc_xbrl_extractor-0.8.4/LICENSE.txt
+-rw-r--r--   0 zane      (1000) staff       (20)      160 2023-04-04 18:48:48.000000 catalystcoop.ferc_xbrl_extractor-0.8.4/MANIFEST.in
+-rw-r--r--   0 zane      (1000) staff       (20)    11285 2023-07-21 17:58:28.166532 catalystcoop.ferc_xbrl_extractor-0.8.4/PKG-INFO
+-rw-r--r--   0 zane      (1000) staff       (20)     8765 2022-12-21 05:42:16.000000 catalystcoop.ferc_xbrl_extractor-0.8.4/README.rst
+-rw-r--r--   0 zane      (1000) staff       (20)      269 2023-07-21 16:53:33.000000 catalystcoop.ferc_xbrl_extractor-0.8.4/environment.yml
+-rw-r--r--   0 zane      (1000) staff       (20)     3929 2023-07-21 17:16:40.000000 catalystcoop.ferc_xbrl_extractor-0.8.4/pyproject.toml
+-rw-r--r--   0 zane      (1000) staff       (20)       38 2023-07-21 17:58:28.166810 catalystcoop.ferc_xbrl_extractor-0.8.4/setup.cfg
+drwxr-xr-x   0 zane      (1000) staff       (20)        0 2023-07-21 17:58:28.162729 catalystcoop.ferc_xbrl_extractor-0.8.4/src/
+drwxr-xr-x   0 zane      (1000) staff       (20)        0 2023-07-21 17:58:28.164449 catalystcoop.ferc_xbrl_extractor-0.8.4/src/catalystcoop.ferc_xbrl_extractor.egg-info/
+-rw-r--r--   0 zane      (1000) staff       (20)    11285 2023-07-21 17:58:28.000000 catalystcoop.ferc_xbrl_extractor-0.8.4/src/catalystcoop.ferc_xbrl_extractor.egg-info/PKG-INFO
+-rw-r--r--   0 zane      (1000) staff       (20)      952 2023-07-21 17:58:28.000000 catalystcoop.ferc_xbrl_extractor-0.8.4/src/catalystcoop.ferc_xbrl_extractor.egg-info/SOURCES.txt
+-rw-r--r--   0 zane      (1000) staff       (20)        1 2023-07-21 17:58:28.000000 catalystcoop.ferc_xbrl_extractor-0.8.4/src/catalystcoop.ferc_xbrl_extractor.egg-info/dependency_links.txt
+-rw-r--r--   0 zane      (1000) staff       (20)       62 2023-07-21 17:58:28.000000 catalystcoop.ferc_xbrl_extractor-0.8.4/src/catalystcoop.ferc_xbrl_extractor.egg-info/entry_points.txt
+-rw-r--r--   0 zane      (1000) staff       (20)      798 2023-07-21 17:58:28.000000 catalystcoop.ferc_xbrl_extractor-0.8.4/src/catalystcoop.ferc_xbrl_extractor.egg-info/requires.txt
+-rw-r--r--   0 zane      (1000) staff       (20)       20 2023-07-21 17:58:28.000000 catalystcoop.ferc_xbrl_extractor-0.8.4/src/catalystcoop.ferc_xbrl_extractor.egg-info/top_level.txt
+drwxr-xr-x   0 zane      (1000) staff       (20)        0 2023-07-21 17:58:28.165413 catalystcoop.ferc_xbrl_extractor-0.8.4/src/ferc_xbrl_extractor/
+-rw-r--r--   0 zane      (1000) staff       (20)      117 2022-09-06 23:55:13.000000 catalystcoop.ferc_xbrl_extractor-0.8.4/src/ferc_xbrl_extractor/__init__.py
+-rw-r--r--   0 zane      (1000) staff       (20)     5326 2023-07-21 17:04:50.000000 catalystcoop.ferc_xbrl_extractor-0.8.4/src/ferc_xbrl_extractor/arelle_interface.py
+-rw-r--r--   0 zane      (1000) staff       (20)     6629 2022-12-09 18:37:59.000000 catalystcoop.ferc_xbrl_extractor-0.8.4/src/ferc_xbrl_extractor/cli.py
+-rw-r--r--   0 zane      (1000) staff       (20)    14161 2022-12-09 18:37:59.000000 catalystcoop.ferc_xbrl_extractor-0.8.4/src/ferc_xbrl_extractor/datapackage.py
+-rw-r--r--   0 zane      (1000) staff       (20)      911 2022-09-06 23:55:13.000000 catalystcoop.ferc_xbrl_extractor-0.8.4/src/ferc_xbrl_extractor/helpers.py
+-rw-r--r--   0 zane      (1000) staff       (20)    12415 2023-07-21 17:15:26.000000 catalystcoop.ferc_xbrl_extractor-0.8.4/src/ferc_xbrl_extractor/instance.py
+-rw-r--r--   0 zane      (1000) staff       (20)    10917 2023-07-21 17:04:51.000000 catalystcoop.ferc_xbrl_extractor-0.8.4/src/ferc_xbrl_extractor/taxonomy.py
+-rw-r--r--   0 zane      (1000) staff       (20)     7723 2022-12-09 18:37:59.000000 catalystcoop.ferc_xbrl_extractor-0.8.4/src/ferc_xbrl_extractor/xbrl.py
+drwxr-xr-x   0 zane      (1000) staff       (20)        0 2023-07-21 17:58:28.165654 catalystcoop.ferc_xbrl_extractor-0.8.4/tests/
+-rw-r--r--   0 zane      (1000) staff       (20)       44 2022-09-06 23:55:13.000000 catalystcoop.ferc_xbrl_extractor-0.8.4/tests/__init__.py
+-rw-r--r--   0 zane      (1000) staff       (20)      998 2022-09-06 23:55:13.000000 catalystcoop.ferc_xbrl_extractor-0.8.4/tests/conftest.py
+drwxr-xr-x   0 zane      (1000) staff       (20)        0 2023-07-21 17:58:28.166003 catalystcoop.ferc_xbrl_extractor-0.8.4/tests/integration/
+-rw-r--r--   0 zane      (1000) staff       (20)       82 2022-09-06 23:55:13.000000 catalystcoop.ferc_xbrl_extractor-0.8.4/tests/integration/__init__.py
+-rw-r--r--   0 zane      (1000) staff       (20)     1477 2022-12-20 22:44:44.000000 catalystcoop.ferc_xbrl_extractor-0.8.4/tests/integration/console_scripts_test.py
+-rw-r--r--   0 zane      (1000) staff       (20)      672 2022-09-06 23:55:13.000000 catalystcoop.ferc_xbrl_extractor-0.8.4/tests/integration/datapackage_test.py
+drwxr-xr-x   0 zane      (1000) staff       (20)        0 2023-07-21 17:58:28.166331 catalystcoop.ferc_xbrl_extractor-0.8.4/tests/unit/
+-rw-r--r--   0 zane      (1000) staff       (20)       84 2022-09-06 23:55:13.000000 catalystcoop.ferc_xbrl_extractor-0.8.4/tests/unit/__init__.py
+-rw-r--r--   0 zane      (1000) staff       (20)     5641 2022-09-06 23:55:13.000000 catalystcoop.ferc_xbrl_extractor-0.8.4/tests/unit/datapackage_test.py
+-rw-r--r--   0 zane      (1000) staff       (20)     3761 2022-09-06 23:55:13.000000 catalystcoop.ferc_xbrl_extractor-0.8.4/tests/unit/instance_test.py
+-rw-r--r--   0 zane      (1000) staff       (20)     6865 2023-07-21 16:57:12.000000 catalystcoop.ferc_xbrl_extractor-0.8.4/tox.ini
```

### Comparing `catalystcoop.ferc_xbrl_extractor-0.8.3/LICENSE.txt` & `catalystcoop.ferc_xbrl_extractor-0.8.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `catalystcoop.ferc_xbrl_extractor-0.8.3/PKG-INFO` & `catalystcoop.ferc_xbrl_extractor-0.8.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: catalystcoop.ferc_xbrl_extractor
-Version: 0.8.3
+Version: 0.8.4
 Summary: A tool for extracting data from FERC XBRL Filings.
 Author-email: Catalyst Cooperative <pudl@catalyst.coop>, Zach Schira <zach.schira@catalyst.coop>
 License: MIT License
         
         Copyright (c) 2022 Catalyst Cooperative
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `catalystcoop.ferc_xbrl_extractor-0.8.3/README.rst` & `catalystcoop.ferc_xbrl_extractor-0.8.4/README.rst`

 * *Files identical despite different names*

### Comparing `catalystcoop.ferc_xbrl_extractor-0.8.3/pyproject.toml` & `catalystcoop.ferc_xbrl_extractor-0.8.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [build-system]
 build-backend = "setuptools.build_meta"
 requires = [
-    "setuptools>=66,<68",
+    "setuptools>=66,<69",
     "setuptools_scm[toml]>=3.5.0",
     "wheel",
 ]
 
 [project]
 name = "catalystcoop.ferc_xbrl_extractor"
 description = "A tool for extracting data from FERC XBRL Filings."
@@ -14,22 +14,22 @@
     {name = "Catalyst Cooperative", email = "pudl@catalyst.coop"},
     {name = "Zach Schira", email = "zach.schira@catalyst.coop"}
 ]
 requires-python = ">=3.10,<3.12"
 dynamic = ["version"]
 license = {file = "LICENSE.txt"}
 dependencies = [
-    "pydantic>=1.9,<2",
+    "pydantic>=2,<3",
     "coloredlogs>=14.0,<15.1",
-    "arelle-release>=2.3,<2.11",
+    "arelle-release>=2.3,<2.12",
     "frictionless>=4.4,<5",
     "sqlalchemy>=1.4,<3",
     "pandas>=1.5,<2.1",
     "stringcase~=1.2.0",
-    "numpy>=1.16,<1.25",
+    "numpy>=1.16,<2",
     "lxml>=4.9.1,<5",
 ]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Environment :: Console",
     "License :: OSI Approved :: MIT License",
     "Natural Language :: English",
@@ -49,15 +49,15 @@
 "Issue Tracker" = "https://github.com/catalyst-cooperative/ferc-xbrl-extract/issues"
 
 [project.scripts]
 xbrl_extract = "ferc_xbrl_extractor.cli:main"
 
 [project.optional-dependencies]
 dev = [
-    "black>=22.0,<23.4",  # A deterministic code formatter
+    "black>=22.0,<23.8",  # A deterministic code formatter
     "build>=0.10,<0.11",
     "isort>=5.0,<5.13",  # Standardized import sorting
     "tox>=4.0,<4.7",  # Python test environment manager
     "twine>=3.3,<4.1",  # Used to make releases to PyPI
 ]
 docs = [
     "doc8>=1.0,<1.2",  # Ensures clean documentation formatting
@@ -73,22 +73,22 @@
     "flake8>=4.0,<6.1",  # A framework for linting & static analysis
     "flake8-builtins>=1.5,<2.2",  # Avoid shadowing Python built-in names
     "flake8-colors>=0.1,<0.2",  # Produce colorful error / warning output
     "flake8-docstrings>=1.5,<1.8",  # Ensure docstrings are formatted well
     "flake8-rst-docstrings>=0.2,<0.4",  # Allow use of ReST in docstrings
     "flake8-use-fstring>=1.0,<1.5",  # Highlight use of old-style string formatting
     "mccabe>=0.6,<0.8",  # Checks that code isn't overly complicated
-    "mypy>=1.0,<1.4",  # Static type checking
+    "mypy>=1.0,<1.5",  # Static type checking
     "pep8-naming>=0.12,<0.14",  # Require PEP8 compliant variable names
     "pre-commit>=2.9,<3.4",  # Allow us to run pre-commit hooks in testing
     "pydocstyle>=5.1,<6.4",  # Style guidelines for Python documentation
-    "pytest>=6.2,<7.4",  # Our testing framework
+    "pytest>=6.2,<7.5",  # Our testing framework
     "pytest-console-scripts>=1.1,<1.5",  # Allow automatic testing of scripts
     "pytest-cov>=2.10,<4.2",  # Pytest plugin for working with coverage
-    "rstcheck[sphinx]>=5.0,<6.2",  # ReStructuredText linter
+    #"rstcheck[sphinx]>=5.0,<6.2",  # ReStructuredText linter
     "tox>=4.0,<4.7",  # Python test environment manager
 ]
 types = [
     "types-setuptools",
 ]
 
 [tool.setuptools]
```

### Comparing `catalystcoop.ferc_xbrl_extractor-0.8.3/src/catalystcoop.ferc_xbrl_extractor.egg-info/PKG-INFO` & `catalystcoop.ferc_xbrl_extractor-0.8.4/src/catalystcoop.ferc_xbrl_extractor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: catalystcoop.ferc-xbrl-extractor
-Version: 0.8.3
+Version: 0.8.4
 Summary: A tool for extracting data from FERC XBRL Filings.
 Author-email: Catalyst Cooperative <pudl@catalyst.coop>, Zach Schira <zach.schira@catalyst.coop>
 License: MIT License
         
         Copyright (c) 2022 Catalyst Cooperative
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `catalystcoop.ferc_xbrl_extractor-0.8.3/src/catalystcoop.ferc_xbrl_extractor.egg-info/SOURCES.txt` & `catalystcoop.ferc_xbrl_extractor-0.8.4/src/catalystcoop.ferc_xbrl_extractor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `catalystcoop.ferc_xbrl_extractor-0.8.3/src/catalystcoop.ferc_xbrl_extractor.egg-info/requires.txt` & `catalystcoop.ferc_xbrl_extractor-0.8.4/src/catalystcoop.ferc_xbrl_extractor.egg-info/requires.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-pydantic<2,>=1.9
+pydantic<3,>=2
 coloredlogs<15.1,>=14.0
-arelle-release<2.11,>=2.3
+arelle-release<2.12,>=2.3
 frictionless<5,>=4.4
 sqlalchemy<3,>=1.4
 pandas<2.1,>=1.5
 stringcase~=1.2.0
-numpy<1.25,>=1.16
+numpy<2,>=1.16
 lxml<5,>=4.9.1
 
 [dev]
-black<23.4,>=22.0
+black<23.8,>=22.0
 build<0.11,>=0.10
 isort<5.13,>=5.0
 tox<4.7,>=4.0
 twine<4.1,>=3.3
 
 [docs]
 doc8<1.2,>=1.0
@@ -29,19 +29,18 @@
 flake8<6.1,>=4.0
 flake8-builtins<2.2,>=1.5
 flake8-colors<0.2,>=0.1
 flake8-docstrings<1.8,>=1.5
 flake8-rst-docstrings<0.4,>=0.2
 flake8-use-fstring<1.5,>=1.0
 mccabe<0.8,>=0.6
-mypy<1.4,>=1.0
+mypy<1.5,>=1.0
 pep8-naming<0.14,>=0.12
 pre-commit<3.4,>=2.9
 pydocstyle<6.4,>=5.1
-pytest<7.4,>=6.2
+pytest<7.5,>=6.2
 pytest-console-scripts<1.5,>=1.1
 pytest-cov<4.2,>=2.10
-rstcheck[sphinx]<6.2,>=5.0
 tox<4.7,>=4.0
 
 [types]
 types-setuptools
```

### Comparing `catalystcoop.ferc_xbrl_extractor-0.8.3/src/ferc_xbrl_extractor/arelle_interface.py` & `catalystcoop.ferc_xbrl_extractor-0.8.4/src/ferc_xbrl_extractor/arelle_interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,15 @@
     Taxonomies contain various metedata which are useful for interpreting XBRL filings.
     The metadata fields being extracted here include references, calculations, and balances.
     """
 
     name: str
     references: References
     calculations: list[Calculation]
-    balance: Literal["credit", "debit"] | None
+    balance: Literal["credit", "debit"] | None = None
 
     @classmethod
     def from_concept(cls, concept: ModelConcept) -> "Metadata":
         """Get metadata for a single XBRL Concept.
 
         This function will create a Metadata object with metadata extracted for
         a single Concept.
```

### Comparing `catalystcoop.ferc_xbrl_extractor-0.8.3/src/ferc_xbrl_extractor/cli.py` & `catalystcoop.ferc_xbrl_extractor-0.8.4/src/ferc_xbrl_extractor/cli.py`

 * *Files identical despite different names*

### Comparing `catalystcoop.ferc_xbrl_extractor-0.8.3/src/ferc_xbrl_extractor/datapackage.py` & `catalystcoop.ferc_xbrl_extractor-0.8.4/src/ferc_xbrl_extractor/datapackage.py`

 * *Files identical despite different names*

### Comparing `catalystcoop.ferc_xbrl_extractor-0.8.3/src/ferc_xbrl_extractor/helpers.py` & `catalystcoop.ferc_xbrl_extractor-0.8.4/src/ferc_xbrl_extractor/helpers.py`

 * *Files identical despite different names*

### Comparing `catalystcoop.ferc_xbrl_extractor-0.8.3/src/ferc_xbrl_extractor/instance.py` & `catalystcoop.ferc_xbrl_extractor-0.8.4/src/ferc_xbrl_extractor/instance.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,29 +2,29 @@
 import io
 from enum import Enum, auto
 from typing import BinaryIO
 
 import stringcase
 from lxml import etree  # nosec: B410
 from lxml.etree import _Element as Element  # nosec: B410
-from pydantic import BaseModel, validator
+from pydantic import BaseModel, field_validator
 
 XBRL_INSTANCE = "http://www.xbrl.org/2003/instance"
 
 
 class Period(BaseModel):
     """Pydantic model that defines an XBRL period.
 
     A period can be instantaneous or a duration of time. Instantaneous periods will
     only have the end_date field, while duration periods will have start_date, and
     end_date.
     """
 
     instant: bool
-    start_date: str | None
+    start_date: str | None = None
     end_date: str
 
     @classmethod
     def from_xml(cls, elem: Element) -> "Period":
         """Construct Period from XML element."""
         instant = elem.find(f"{{{XBRL_INSTANCE}}}instant")
         if instant is not None:
@@ -57,15 +57,16 @@
     belong to.
     """
 
     name: str
     value: str = ""
     dimension_type: DimensionType
 
-    @validator("name", pre=True)  # type: ignore
+    @field_validator("name", mode="before")  # type: ignore
+    @classmethod
     def strip_prefix(cls, name: str):  # noqa: N805
         """Strip XML prefix from name."""
         return name.split(":")[1] if ":" in name else name
 
     @classmethod
     def from_xml(cls, elem: Element) -> "Axis":
         """Construct Axis from XML element."""
@@ -188,15 +189,15 @@
 
     A fact is a single "data point", which contains a name, value, and a Context to
     give background information.
     """
 
     name: str
     c_id: str
-    value: str | None
+    value: str | None = None
 
     @classmethod
     def from_xml(cls, elem: Element) -> "Fact":
         """Construct Fact from XML element."""
         # Get prefix from namespace map to strip from fact name
         prefix = f"{{{elem.nsmap[elem.prefix]}}}"
         return cls(
```

### Comparing `catalystcoop.ferc_xbrl_extractor-0.8.3/src/ferc_xbrl_extractor/taxonomy.py` & `catalystcoop.ferc_xbrl_extractor-0.8.4/src/ferc_xbrl_extractor/taxonomy.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 
     name: str
     standard_label: str
     documentation: str
     type_: XBRLType = pydantic.Field(alias="type")
     period_type: Literal["duration", "instant"]
     child_concepts: "list[Concept]"
-    metadata: Metadata | None
+    metadata: Metadata | None = None
 
     @classmethod
     def from_list(cls, concept_list: list, concept_dict: ConceptDict) -> "Concept":
         """Construct a Concept from a list.
 
         The way Arelle represents the structure of the of a taxonomy is a
         bit unintuitive. Each concept is represented as a list with
```

### Comparing `catalystcoop.ferc_xbrl_extractor-0.8.3/src/ferc_xbrl_extractor/xbrl.py` & `catalystcoop.ferc_xbrl_extractor-0.8.4/src/ferc_xbrl_extractor/xbrl.py`

 * *Files identical despite different names*

### Comparing `catalystcoop.ferc_xbrl_extractor-0.8.3/tests/conftest.py` & `catalystcoop.ferc_xbrl_extractor-0.8.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `catalystcoop.ferc_xbrl_extractor-0.8.3/tests/integration/console_scripts_test.py` & `catalystcoop.ferc_xbrl_extractor-0.8.4/tests/integration/console_scripts_test.py`

 * *Files identical despite different names*

### Comparing `catalystcoop.ferc_xbrl_extractor-0.8.3/tests/integration/datapackage_test.py` & `catalystcoop.ferc_xbrl_extractor-0.8.4/tests/integration/datapackage_test.py`

 * *Files identical despite different names*

### Comparing `catalystcoop.ferc_xbrl_extractor-0.8.3/tests/unit/datapackage_test.py` & `catalystcoop.ferc_xbrl_extractor-0.8.4/tests/unit/datapackage_test.py`

 * *Files identical despite different names*

### Comparing `catalystcoop.ferc_xbrl_extractor-0.8.3/tests/unit/instance_test.py` & `catalystcoop.ferc_xbrl_extractor-0.8.4/tests/unit/instance_test.py`

 * *Files identical despite different names*

### Comparing `catalystcoop.ferc_xbrl_extractor-0.8.3/tox.ini` & `catalystcoop.ferc_xbrl_extractor-0.8.4/tox.ini`

 * *Files 1% similar despite different names*

```diff
@@ -63,20 +63,20 @@
 
 [testenv:linters]
 description = Run the pre-commit, flake8 and bandit linters.
 skip_install = false
 extras =
     {[testenv:pre_commit]extras}
     {[testenv:bandit]extras}
-    {[testenv:rstcheck]extras}
+#   {[testenv:rstcheck]extras}
     {[testenv:flake8]extras}
 commands =
     {[testenv:pre_commit]commands}
     {[testenv:bandit]commands}
-    {[testenv:rstcheck]commands}
+#   {[testenv:rstcheck]commands}
     {[testenv:flake8]commands}
 
 #######################################################################################
 # Lint and Build the Docs
 #######################################################################################
 [testenv:doc8]
 description = Check the documentation input files for syntactical correctness.
@@ -87,19 +87,19 @@
     doc8 docs/ README.rst
 
 [testenv:docs]
 description = Build the HTML docs from scratch using Sphinx.
 skip_install = false
 extras =
     {[testenv:doc8]extras}
-    {[testenv:rstcheck]extras}
+#   {[testenv:rstcheck]extras}
 commands =
     bash -c 'rm -rf docs/_build'
     {[testenv:doc8]commands}
-    {[testenv:rstcheck]commands}
+#   {[testenv:rstcheck]commands}
     sphinx-build -W -b html docs docs/_build/html
 
 #######################################################################################
 # Test the code
 #######################################################################################
 [testenv:unit]
 description = Run all the software unit tests.
@@ -152,26 +152,26 @@
 basepython = python3
 skip_install = false
 extras =
     dev
 commands =
     {[testenv:build]commands}
     twine check dist/*
-    twine upload --sign --verbose --repository testpypi --skip-existing dist/*
+    twine upload --verbose --repository testpypi --skip-existing dist/*
 
 [testenv:release]
 description = Release the package to the production PyPI server.
 basepython = python3
 skip_install = false
 extras =
     dev
 commands =
     {[testenv:build]commands}
     twine check dist/*
-    twine upload --sign --verbose --skip-existing dist/*
+    twine upload --verbose --skip-existing dist/*
 
 #######################################################################################
 # Configuration for various tools.
 #######################################################################################
 [pytest]
 testpaths = .
 addopts = --verbose
```

