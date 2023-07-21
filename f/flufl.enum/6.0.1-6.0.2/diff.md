# Comparing `tmp/flufl_enum-6.0.1.tar.gz` & `tmp/flufl_enum-6.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flufl_enum-6.0.1.tar", last modified: Mon Jun 26 16:46:16 2023, max compression
+gzip compressed data, was "flufl_enum-6.0.2.tar", last modified: Fri Jul 21 20:01:32 2023, max compression
```

## Comparing `flufl_enum-6.0.1.tar` & `flufl_enum-6.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      558 2023-06-26 16:45:49.345758 flufl_enum-6.0.1/LICENSE
--rw-r--r--   0        0        0     1165 2023-06-26 16:45:49.345758 flufl_enum-6.0.1/README.rst
--rw-r--r--   0        0        0     1377 2023-06-26 16:45:49.345758 flufl_enum-6.0.1/conftest.py
--rw-r--r--   0        0        0     6667 2023-06-26 16:45:49.345758 flufl_enum-6.0.1/docs/NEWS.rst
--rw-r--r--   0        0        0        0 2023-06-26 16:45:49.369758 flufl_enum-6.0.1/docs/__init__.py
--rw-r--r--   0        0        0      221 2023-06-26 16:45:49.345758 flufl_enum-6.0.1/docs/apiref.rst
--rw-r--r--   0        0        0     7203 2023-06-26 16:45:49.345758 flufl_enum-6.0.1/docs/conf.py
--rw-r--r--   0        0        0     2456 2023-06-26 16:45:49.345758 flufl_enum-6.0.1/docs/index.rst
--rw-r--r--   0        0        0    14725 2023-06-26 16:45:49.345758 flufl_enum-6.0.1/docs/using.rst
--rw-r--r--   0        0        0     3013 2023-06-26 16:46:16.595063 flufl_enum-6.0.1/pyproject.toml
--rw-r--r--   0        0        0      223 2023-06-26 16:45:49.346758 flufl_enum-6.0.1/src/flufl/enum/__init__.py
--rw-r--r--   0        0        0     9048 2023-06-26 16:45:49.346758 flufl_enum-6.0.1/src/flufl/enum/_enum.py
--rw-r--r--   0        0        0        0 2023-06-26 16:45:49.369758 flufl_enum-6.0.1/test/__init__.py
--rw-r--r--   0        0        0       92 2023-06-26 16:45:49.346758 flufl_enum-6.0.1/test/fruit.py
--rw-r--r--   0        0        0    10088 2023-06-26 16:45:49.346758 flufl_enum-6.0.1/test/test_enum.py
--rw-r--r--   0        0        0      772 2023-06-26 16:45:49.346758 flufl_enum-6.0.1/tox.ini
--rw-r--r--   0        0        0     2245 1970-01-01 00:00:00.000000 flufl_enum-6.0.1/PKG-INFO
+-rw-r--r--   0        0        0      558 2023-07-21 20:01:04.601018 flufl_enum-6.0.2/LICENSE
+-rw-r--r--   0        0        0     1165 2023-07-21 20:01:04.601018 flufl_enum-6.0.2/README.rst
+-rw-r--r--   0        0        0     1377 2023-07-21 20:01:04.601018 flufl_enum-6.0.2/conftest.py
+-rw-r--r--   0        0        0     6760 2023-07-21 20:01:04.601018 flufl_enum-6.0.2/docs/NEWS.rst
+-rw-r--r--   0        0        0        0 2023-07-21 20:01:04.625018 flufl_enum-6.0.2/docs/__init__.py
+-rw-r--r--   0        0        0      221 2023-07-21 20:01:04.601018 flufl_enum-6.0.2/docs/apiref.rst
+-rw-r--r--   0        0        0     7205 2023-07-21 20:01:04.601018 flufl_enum-6.0.2/docs/conf.py
+-rw-r--r--   0        0        0     2451 2023-07-21 20:01:04.602018 flufl_enum-6.0.2/docs/index.rst
+-rw-r--r--   0        0        0    14616 2023-07-21 20:01:04.602018 flufl_enum-6.0.2/docs/using.rst
+-rw-r--r--   0        0        0     3013 2023-07-21 20:01:32.536778 flufl_enum-6.0.2/pyproject.toml
+-rw-r--r--   0        0        0      223 2023-07-21 20:01:04.602018 flufl_enum-6.0.2/src/flufl/enum/__init__.py
+-rw-r--r--   0        0        0     9048 2023-07-21 20:01:04.603018 flufl_enum-6.0.2/src/flufl/enum/_enum.py
+-rw-r--r--   0        0        0        0 2023-07-21 20:01:04.626018 flufl_enum-6.0.2/test/__init__.py
+-rw-r--r--   0        0        0       92 2023-07-21 20:01:04.603018 flufl_enum-6.0.2/test/fruit.py
+-rw-r--r--   0        0        0    10088 2023-07-21 20:01:04.603018 flufl_enum-6.0.2/test/test_enum.py
+-rw-r--r--   0        0        0      772 2023-07-21 20:01:04.603018 flufl_enum-6.0.2/tox.ini
+-rw-r--r--   0        0        0     2245 1970-01-01 00:00:00.000000 flufl_enum-6.0.2/PKG-INFO
```

### Comparing `flufl_enum-6.0.1/LICENSE` & `flufl_enum-6.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `flufl_enum-6.0.1/README.rst` & `flufl_enum-6.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `flufl_enum-6.0.1/conftest.py` & `flufl_enum-6.0.2/conftest.py`

 * *Files identical despite different names*

### Comparing `flufl_enum-6.0.1/docs/NEWS.rst` & `flufl_enum-6.0.2/docs/NEWS.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 =====================
 flufl.enum change log
 =====================
 
+6.0.2 (2023-07-16)
+==================
+* Update dependencies.
+* Minor documentation updates.
+
 6.0.1 (2023-06-26)
 ==================
 * Update dependencies.
 * This release also utilizes a newer ``pdm-backend`` which fixes the project
   metadata.
 
 6.0 (2023-06-05)
```

### Comparing `flufl_enum-6.0.1/docs/conf.py` & `flufl_enum-6.0.2/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 # coming with Sphinx (named 'sphinx.ext.*') or your custom ones.
 extensions = [
     'sphinx.ext.autodoc',
     'sphinx.ext.intersphinx',
     ]
 
 intersphinx_mapping = {
-    'python': ('https://docs.python.org/', None),
+    'python': ('https://docs.python.org/3/', None),
     }
 
 #autodoc_typehints = 'both'
 autoclass_content = 'both'
 
 # We don't want to document the EnumValue.__init__() arguments because user
 # code will never call it directly.
```

### Comparing `flufl_enum-6.0.1/docs/index.rst` & `flufl_enum-6.0.2/docs/index.rst`

 * *Files 5% similar despite different names*

```diff
@@ -34,21 +34,21 @@
 ===============
 
  * Project home: https://gitlab.com/warsaw/flufl.enum
  * Report bugs at: https://gitlab.com/warsaw/flufl.enum/issues
  * Code hosting: https://gitlab.com/warsaw/flufl.enum.git
  * Documentation: http://fluflenum.readthedocs.org/
 
-You can install it with `pip`::
+You can install it with ``pip``::
 
     % pip install flufl.enum
 
-You can grab the latest development copy of the code using git.  The master
-repository is hosted on GitLab.  If you have git installed, you can grab
-your own branch of the code like this::
+You can grab the latest development copy of the code using git.  The
+repository is hosted on GitLab.  If you have git installed, you can grab your
+own branch of the code like this::
 
     $ git clone https://gitlab.com/warsaw/flufl.enum.git
 
 You may contact the author via barry@python.org.
 
 
 Copyright
```

### Comparing `flufl_enum-6.0.1/docs/using.rst` & `flufl_enum-6.0.2/docs/using.rst`

 * *Files 2% similar despite different names*

```diff
@@ -504,14 +504,12 @@
 has been modified and extended by Barry Warsaw for use in the `GNU Mailman`_
 project.  Ben Finney is the author of the earlier enumeration PEP 354.  Eli
 Bendersky is the co-author of PEP 435.  Numerous people on the `python-ideas`_
 and `python-dev`_ mailing lists have provided valuable feedback.
 
 
 .. _`PEP 435`: http://www.python.org/dev/peps/pep-0435/
-.. _`Python 3.4`: http://www.python.org/dev/peps/pep-0429/
 .. _`PEP 354`: http://www.python.org/dev/peps/pep-0354/
-.. _enum: http://cheeseshop.python.org/pypi/enum/
 .. _`GNU Mailman`: http://www.list.org
 .. _`python-ideas`: http://mail.python.org/mailman/listinfo/python-ideas
 .. _`python-dev`: http://mail.python.org/mailman/listinfo/python-dev
 .. _`Barry Warsaw`: http://barry.warsaw.us
```

### Comparing `flufl_enum-6.0.1/pyproject.toml` & `flufl_enum-6.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     "Topic :: Software Development :: Libraries",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 dependencies = [
     "atpublic",
 ]
 dynamic = []
-version = "6.0.1"
+version = "6.0.2"
 
 [project.license]
 text = "Apache-2.0"
 
 [project.urls]
 "Home Page" = "https://fluflenum.readthedocs.io"
 Documentation = "https://fluflenum.readthedocs.io"
```

### Comparing `flufl_enum-6.0.1/src/flufl/enum/_enum.py` & `flufl_enum-6.0.2/src/flufl/enum/_enum.py`

 * *Files identical despite different names*

### Comparing `flufl_enum-6.0.1/test/test_enum.py` & `flufl_enum-6.0.2/test/test_enum.py`

 * *Files identical despite different names*

### Comparing `flufl_enum-6.0.1/tox.ini` & `flufl_enum-6.0.2/tox.ini`

 * *Files identical despite different names*

### Comparing `flufl_enum-6.0.1/PKG-INFO` & `flufl_enum-6.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flufl.enum
-Version: 6.0.1
+Version: 6.0.2
 Summary: A Python enumeration package
 Keywords: enum
 Author-Email: Barry Warsaw <barry@python.org>
 License: Apache-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Development Status :: 6 - Mature
 Classifier: Intended Audience :: Developers
```

