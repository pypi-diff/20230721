# Comparing `tmp/pospell-1.2.tar.gz` & `tmp/pospell-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pospell-1.2.tar", last modified: Tue Jul 18 13:06:34 2023, max compression
+gzip compressed data, was "pospell-1.3.tar", last modified: Fri Jul 21 07:08:35 2023, max compression
```

## Comparing `pospell-1.2.tar` & `pospell-1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 mdk       (1000) mdk       (1000)        0 2023-07-18 13:06:34.722670 pospell-1.2/
--rw-r--r--   0 mdk       (1000) mdk       (1000)     2714 2023-07-18 13:06:34.722670 pospell-1.2/PKG-INFO
--rw-r--r--   0 mdk       (1000) mdk       (1000)     2082 2023-04-10 13:30:19.000000 pospell-1.2/README.md
-drwxr-xr-x   0 mdk       (1000) mdk       (1000)        0 2023-07-18 13:06:34.722670 pospell-1.2/pospell.egg-info/
--rw-r--r--   0 mdk       (1000) mdk       (1000)     2714 2023-07-18 13:06:34.000000 pospell-1.2/pospell.egg-info/PKG-INFO
--rw-r--r--   0 mdk       (1000) mdk       (1000)      245 2023-07-18 13:06:34.000000 pospell-1.2/pospell.egg-info/SOURCES.txt
--rw-r--r--   0 mdk       (1000) mdk       (1000)        1 2023-07-18 13:06:34.000000 pospell-1.2/pospell.egg-info/dependency_links.txt
--rw-r--r--   0 mdk       (1000) mdk       (1000)       41 2023-07-18 13:06:34.000000 pospell-1.2/pospell.egg-info/entry_points.txt
--rw-r--r--   0 mdk       (1000) mdk       (1000)       27 2023-07-18 13:06:34.000000 pospell-1.2/pospell.egg-info/requires.txt
--rw-r--r--   0 mdk       (1000) mdk       (1000)        8 2023-07-18 13:06:34.000000 pospell-1.2/pospell.egg-info/top_level.txt
--rw-r--r--   0 mdk       (1000) mdk       (1000)    15975 2023-07-18 13:04:11.000000 pospell-1.2/pospell.py
--rw-r--r--   0 mdk       (1000) mdk       (1000)     1111 2023-07-18 12:38:53.000000 pospell-1.2/pyproject.toml
--rw-r--r--   0 mdk       (1000) mdk       (1000)       38 2023-07-18 13:06:34.722670 pospell-1.2/setup.cfg
-drwxr-xr-x   0 mdk       (1000) mdk       (1000)        0 2023-07-18 13:06:34.722670 pospell-1.2/tests/
--rw-r--r--   0 mdk       (1000) mdk       (1000)     2617 2021-04-09 22:07:43.000000 pospell-1.2/tests/test_pospell.py
+drwxr-xr-x   0 mdk       (1000) mdk       (1000)        0 2023-07-21 07:08:35.263966 pospell-1.3/
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     2714 2023-07-21 07:08:35.263966 pospell-1.3/PKG-INFO
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     2082 2023-04-10 13:30:19.000000 pospell-1.3/README.md
+drwxr-xr-x   0 mdk       (1000) mdk       (1000)        0 2023-07-21 07:08:35.263966 pospell-1.3/pospell.egg-info/
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     2714 2023-07-21 07:08:35.000000 pospell-1.3/pospell.egg-info/PKG-INFO
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      245 2023-07-21 07:08:35.000000 pospell-1.3/pospell.egg-info/SOURCES.txt
+-rw-r--r--   0 mdk       (1000) mdk       (1000)        1 2023-07-21 07:08:35.000000 pospell-1.3/pospell.egg-info/dependency_links.txt
+-rw-r--r--   0 mdk       (1000) mdk       (1000)       41 2023-07-21 07:08:35.000000 pospell-1.3/pospell.egg-info/entry_points.txt
+-rw-r--r--   0 mdk       (1000) mdk       (1000)       46 2023-07-21 07:08:35.000000 pospell-1.3/pospell.egg-info/requires.txt
+-rw-r--r--   0 mdk       (1000) mdk       (1000)        8 2023-07-21 07:08:35.000000 pospell-1.3/pospell.egg-info/top_level.txt
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    15450 2023-07-21 07:08:03.000000 pospell-1.3/pospell.py
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     1150 2023-07-21 07:03:19.000000 pospell-1.3/pyproject.toml
+-rw-r--r--   0 mdk       (1000) mdk       (1000)       38 2023-07-21 07:08:35.263966 pospell-1.3/setup.cfg
+drwxr-xr-x   0 mdk       (1000) mdk       (1000)        0 2023-07-21 07:08:35.263966 pospell-1.3/tests/
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     2617 2021-04-09 22:07:43.000000 pospell-1.3/tests/test_pospell.py
```

### Comparing `pospell-1.2/PKG-INFO` & `pospell-1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pospell
-Version: 1.2
+Version: 1.3
 Summary: Spellcheck .po files containing reStructuredText translations
 Author-email: Julien Palard <julien@palard.fr>
 License: MIT license
 Project-URL: Homepage, https://git.afpy.org/AFPy/pospell
 Keywords: po,spell,gettext,reStructuredText,check,sphinx,translation
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `pospell-1.2/README.md` & `pospell-1.3/README.md`

 * *Files identical despite different names*

### Comparing `pospell-1.2/pospell.egg-info/PKG-INFO` & `pospell-1.3/pospell.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pospell
-Version: 1.2
+Version: 1.3
 Summary: Spellcheck .po files containing reStructuredText translations
 Author-email: Julien Palard <julien@palard.fr>
 License: MIT license
 Project-URL: Homepage, https://git.afpy.org/AFPy/pospell
 Keywords: po,spell,gettext,reStructuredText,check,sphinx,translation
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `pospell-1.2/pospell.py` & `pospell-1.3/pospell.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 """pospell is a spellcheckers for po files containing reStructuedText."""
-import io
-from string import digits
-from unicodedata import category
 import collections
 import functools
+import io
 import logging
 import multiprocessing
 import os
 import subprocess
 import sys
-from typing import List, Tuple
 from contextlib import redirect_stderr
 from itertools import chain
 from pathlib import Path
 from shutil import which
+from string import digits
+from typing import List, Tuple
+from unicodedata import category
 
 import docutils.frontend
 import docutils.nodes
 import docutils.parsers.rst
 import polib
+import regex
 from docutils.parsers.rst import roles
 from docutils.utils import new_document
+from sphinxlint import rst
 
-import regex
-
-__version__ = "1.2"
+__version__ = "1.3"
 
 DEFAULT_DROP_CAPITALIZED = {"fr": True, "fr_FR": True}
 
 
 input_line = collections.namedtuple("input_line", "filename line text")
 
 
@@ -134,38 +134,21 @@
 
 
 def strip_rst(line):
     """Transform reStructuredText to plain text."""
     if line.endswith("::"):
         # Drop :: at the end, it would cause Literal block expected
         line = line[:-2]
+    line = rst.NORMAL_ROLE_RE.sub("", line)
+    settings = docutils.frontend.get_default_settings()
+    settings.pep_references = None
+    settings.rfc_references = None
+    settings.pep_base_url = "http://www.python.org/dev/peps/"
+    settings.pep_file_url_template = "pep-%04d"
     parser = docutils.parsers.rst.Parser()
-    settings = docutils.frontend.Values(
-        {
-            "report_level": 2,
-            "halt_level": 4,
-            "exit_status_level": 5,
-            "debug": None,
-            "warning_stream": None,
-            "error_encoding": "utf-8",
-            "error_encoding_error_handler": "backslashreplace",
-            "language_code": "en",
-            "id_prefix": "",
-            "auto_id_prefix": "id",
-            "pep_references": None,
-            "pep_base_url": "http://www.python.org/dev/peps/",
-            "pep_file_url_template": "pep-%04d",
-            "rfc_references": None,
-            "rfc_base_url": "http://tools.ietf.org/html/",
-            "tab_width": 8,
-            "trim_footnote_reference_space": None,
-            "syntax_highlight": "long",
-            "line_length_limit": 10000,
-        }
-    )
     stderr_stringio = io.StringIO()
     with redirect_stderr(stderr_stringio):
         document = new_document("<rst-doc>", settings=settings)
         parser.parse(line, document)
     stderr = stderr_stringio.getvalue()
     if stderr:
         print(stderr.strip(), "while parsing:", line)
```

### Comparing `pospell-1.2/pyproject.toml` & `pospell-1.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -23,16 +23,17 @@
     "License :: OSI Approved :: MIT License",
     "Natural Language :: English",
     "Programming Language :: Python :: 3",
 ]
 requires-python = ">= 3.6"
 dependencies = [
     "polib",
-    "docutils>=0.16",
+    "docutils>=0.18",
     "regex",
+    "sphinx-lint>=0.6.8",
 ]
 dynamic = [
     "version",
 ]
 
 [project.license]
 text = "MIT license"
@@ -51,7 +52,9 @@
 py-modules = [
     "pospell",
 ]
 include-package-data = false
 
 [tool.setuptools.dynamic.version]
 attr = "pospell.__version__"
+
+[tool.black]
```

### Comparing `pospell-1.2/tests/test_pospell.py` & `pospell-1.3/tests/test_pospell.py`

 * *Files identical despite different names*

