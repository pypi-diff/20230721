# Comparing `tmp/default_values-0.5.2.tar.gz` & `tmp/default_values-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "default_values-0.5.2.tar", last modified: Fri Apr 14 12:27:14 2023, max compression
+gzip compressed data, was "default_values-0.5.3.tar", last modified: Fri Jul 21 08:16:20 2023, max compression
```

## Comparing `default_values-0.5.2.tar` & `default_values-0.5.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0 runner    (1001) docker     (122)     7492 2023-04-14 12:27:14.699399 default_values-0.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4926 2023-04-14 12:27:14.699399 default_values-0.5.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)     1093 2023-04-14 12:27:14.691399 default_values-0.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     5855 2023-04-14 12:27:14.699399 default_values-0.5.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)       64 2023-04-14 12:27:14.699399 default_values-0.5.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)    10171 2023-04-14 12:26:43.915115 default_values-0.5.2/sphinxcontrib/default_values/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1254 2023-04-14 12:26:43.915115 default_values-0.5.2/sphinxcontrib/default_values/demo.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-14 12:26:43.915115 default_values-0.5.2/sphinxcontrib/default_values/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)     1093 2023-07-21 08:16:20.298898 default_values-0.5.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       60 2023-07-21 08:16:20.302899 default_values-0.5.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     5855 2023-07-21 08:16:20.306898 default_values-0.5.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     7539 2023-07-21 08:16:20.306898 default_values-0.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4976 2023-07-21 08:16:20.302899 default_values-0.5.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)     1254 2023-07-21 08:15:45.742954 default_values-0.5.3/sphinxcontrib/default_values/demo.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10298 2023-07-21 08:15:45.742954 default_values-0.5.3/sphinxcontrib/default_values/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-21 08:15:45.742954 default_values-0.5.3/sphinxcontrib/default_values/py.typed
```

### Comparing `default_values-0.5.2/PKG-INFO` & `default_values-0.5.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: default-values
-Version: 0.5.2
+Version: 0.5.3
 Summary: Sphinx extension to show default values in documentation.
 Author-email: Dominic Davis-Foster <dominic@davis-foster.co.uk>
 License: MIT
 Keywords: documentation,sphinx
 Home-page: https://github.com/sphinx-toolbox/default_values
 Project-URL: Issue Tracker, https://github.com/sphinx-toolbox/default_values/issues
 Project-URL: Source Code, https://github.com/sphinx-toolbox/default_values
@@ -20,23 +20,24 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Documentation
 Classifier: Topic :: Documentation :: Sphinx
 Classifier: Topic :: Software Development :: Documentation
 Classifier: Typing :: Typed
 Requires-Python: >=3.6
 Requires-Dist: docutils==0.16
-Requires-Dist: sphinx<3.6.0,>=3.2.0
+Requires-Dist: sphinx<6,>=3.2.0
 Requires-Dist: sphinx-jinja2-compat>=0.1.0
 Description-Content-Type: text/x-rst
 
 
 ###############
 default_values
 ###############
@@ -152,15 +153,15 @@
 .. |license| image:: https://img.shields.io/github/license/sphinx-toolbox/default_values
 	:target: https://github.com/sphinx-toolbox/default_values/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/sphinx-toolbox/default_values
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/sphinx-toolbox/default_values/v0.5.2
+.. |commits-since| image:: https://img.shields.io/github/commits-since/sphinx-toolbox/default_values/v0.5.3
 	:target: https://github.com/sphinx-toolbox/default_values/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/sphinx-toolbox/default_values
 	:target: https://github.com/sphinx-toolbox/default_values/commit/master
 	:alt: GitHub last commit
```

### Comparing `default_values-0.5.2/pyproject.toml` & `default_values-0.5.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 [build-system]
 requires = [ "whey",]
 build-backend = "whey"
 
 [project]
 name = "default_values"
-version = "0.5.2"
+version = "0.5.3"
 description = "Sphinx extension to show default values in documentation."
 readme = "README.rst"
 keywords = [ "documentation", "sphinx",]
 dynamic = []
-dependencies = [ "docutils==0.16", "sphinx<3.6.0,>=3.2.0", "sphinx-jinja2-compat>=0.1.0",]
+dependencies = [ "docutils==0.16", "sphinx<6,>=3.2.0", "sphinx-jinja2-compat>=0.1.0",]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Framework :: Sphinx :: Extension",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.6",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
     "Topic :: Documentation",
@@ -52,15 +53,15 @@
     "Framework :: Sphinx :: Extension",
     "Intended Audience :: Developers",
     "Topic :: Documentation",
     "Topic :: Documentation :: Sphinx",
     "Topic :: Software Development :: Documentation",
     "Typing :: Typed",
 ]
-python-versions = [ "3.6", "3.7", "3.8", "3.9", "3.10",]
+python-versions = [ "3.6", "3.7", "3.8", "3.9", "3.10", "3.11",]
 python-implementations = [ "CPython", "PyPy",]
 platforms = [ "Windows", "macOS", "Linux",]
 license-key = "MIT"
 package = "sphinxcontrib"
 
 [tool.mkrecipe]
 conda-channels = [ "conda-forge", "domdfcoding",]
```

### Comparing `default_values-0.5.2/LICENSE` & `default_values-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `default_values-0.5.2/README.rst` & `default_values-0.5.3/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -113,15 +113,15 @@
 .. |license| image:: https://img.shields.io/github/license/sphinx-toolbox/default_values
 	:target: https://github.com/sphinx-toolbox/default_values/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/sphinx-toolbox/default_values
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/sphinx-toolbox/default_values/v0.5.2
+.. |commits-since| image:: https://img.shields.io/github/commits-since/sphinx-toolbox/default_values/v0.5.3
 	:target: https://github.com/sphinx-toolbox/default_values/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/sphinx-toolbox/default_values
 	:target: https://github.com/sphinx-toolbox/default_values/commit/master
 	:alt: GitHub last commit
```

### Comparing `default_values-0.5.2/sphinxcontrib/default_values/__init__.py` & `default_values-0.5.3/sphinxcontrib/default_values/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 	# attrs is used in a way that it is only required in situations
 	# where it is available to import, so its fine to do this.
 	pass
 
 __author__: str = "Dominic Davis-Foster"
 __copyright__: str = "2020 Dominic Davis-Foster"
 __license__: str = "MIT"
-__version__: str = "0.5.2"
+__version__: str = "0.5.3"
 __email__: str = "dominic@davis-foster.co.uk"
 
 __all__ = [
 		"process_docstring",
 		"process_default_format",
 		"setup",
 		"get_class_defaults",
@@ -70,22 +70,22 @@
 		"format_default_value",
 		]
 
 default_regex: Pattern = re.compile("^:(?i:default) ")
 """
 Regular expression to match default values declared in docstrings.
 
-.. versionchanged:: 0.5.2  Change to be case insensitive.
+.. versionchanged:: 0.5.3  Change to be case insensitive.
 """
 
 no_default_regex: Pattern = re.compile("^:(?i:no[-_]default) ")
 """
 Regular expression to match fields in docstrings to suppress default values.
 
-.. versionchanged:: 0.5.2  Change to be case insensitive.
+.. versionchanged:: 0.5.3  Change to be case insensitive.
 """
 
 # ref: sphinx.domains.python.PyObject.doc_field_types
 _fields = '|'.join([
 		"param",
 		"parameter",
 		"arg",
@@ -108,15 +108,15 @@
 	return string
 
 
 def format_default_value(value: Any) -> Optional[str]:
 	"""
 	Format the value as a string.
 
-	.. versionadded:: 0.5.2
+	.. versionadded:: 0.5.3
 
 	:param value:
 	"""
 
 	if value is not inspect.Signature.empty and value is not Ellipsis:
 
 		if isinstance(value, ModuleType):
@@ -221,27 +221,32 @@
 							# Ensure the previous line has a fullstop at the end.
 							line_content = ':'.join(lines[insert_index + idx].split(':')[2:]).strip()
 							if line_content and line_content[-1] not in ".,;:":
 								lines[insert_index + idx] += '.'
 
 							lines.insert(
 									insert_index + 1 + idx,
-									f"{a_tab}{default_description_format % formatted_annotation}."
+									f"{a_tab}{default_description_format % formatted_annotation}".rstrip('.') + '.'
 									)
 							break
 
+		indices_to_remove = set()
+
 		# Remove all remaining :default *: lines
 		for i, line in enumerate(lines):
 			if default_regex.match(line):
-				lines.remove(line)
+				indices_to_remove.add(i)
 
 		# Remove all remaining :no-default *: lines
 		for i, line in enumerate(lines):
 			if no_default_regex.match(line):
-				lines.remove(line)
+				indices_to_remove.add(i)
+
+		for i in sorted(indices_to_remove, reverse=True):
+			del lines[i]
 
 	return None
 
 
 _defaults = Iterator[Tuple[str, Any]]
```

### Comparing `default_values-0.5.2/sphinxcontrib/default_values/demo.py` & `default_values-0.5.3/sphinxcontrib/default_values/demo.py`

 * *Files identical despite different names*

