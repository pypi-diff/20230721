# Comparing `tmp/attr_utils-0.8.0.tar.gz` & `tmp/attr_utils-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "attr_utils-0.8.0.tar", last modified: Fri Jul 21 08:56:11 2023, max compression
+gzip compressed data, was "attr_utils-0.8.1.tar", last modified: Fri Jul 21 12:59:20 2023, max compression
```

## Comparing `attr_utils-0.8.0.tar` & `attr_utils-0.8.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0 runner    (1001) docker     (122)     1064 2023-07-21 08:56:11.723672 attr_utils-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      128 2023-07-21 08:56:11.731672 attr_utils-0.8.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)     5325 2023-07-21 08:56:11.731672 attr_utils-0.8.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)     7299 2023-07-21 08:56:11.735672 attr_utils-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     5000 2023-07-21 08:56:11.731672 attr_utils-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)     4206 2023-07-21 08:55:30.167565 attr_utils-0.8.0/attr_utils/docstrings.py
--rw-r--r--   0 runner    (1001) docker     (122)     6609 2023-07-21 08:55:30.167565 attr_utils-0.8.0/attr_utils/serialise.py
--rw-r--r--   0 runner    (1001) docker     (122)     1440 2023-07-21 08:55:30.167565 attr_utils-0.8.0/attr_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8224 2023-07-21 08:55:30.167565 attr_utils-0.8.0/attr_utils/mypy_plugin.py
--rw-r--r--   0 runner    (1001) docker     (122)     8713 2023-07-21 08:55:30.167565 attr_utils-0.8.0/attr_utils/annotations.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-21 08:55:30.167565 attr_utils-0.8.0/attr_utils/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)     6047 2023-07-21 08:55:30.167565 attr_utils-0.8.0/attr_utils/pprinter.py
--rw-r--r--   0 runner    (1001) docker     (122)     1707 2023-07-21 08:55:30.167565 attr_utils-0.8.0/attr_utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    12298 2023-07-21 08:55:30.167565 attr_utils-0.8.0/attr_utils/autoattrs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1064 2023-07-21 12:59:20.013534 attr_utils-0.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      128 2023-07-21 12:59:20.021534 attr_utils-0.8.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     5325 2023-07-21 12:59:20.021534 attr_utils-0.8.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     7299 2023-07-21 12:59:20.025534 attr_utils-0.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5000 2023-07-21 12:59:20.021534 attr_utils-0.8.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)     4206 2023-07-21 12:58:43.940897 attr_utils-0.8.1/attr_utils/docstrings.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6609 2023-07-21 12:58:43.940897 attr_utils-0.8.1/attr_utils/serialise.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1440 2023-07-21 12:58:43.940897 attr_utils-0.8.1/attr_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8224 2023-07-21 12:58:43.940897 attr_utils-0.8.1/attr_utils/mypy_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8713 2023-07-21 12:58:43.940897 attr_utils-0.8.1/attr_utils/annotations.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-21 12:58:43.940897 attr_utils-0.8.1/attr_utils/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)     6047 2023-07-21 12:58:43.940897 attr_utils-0.8.1/attr_utils/pprinter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1707 2023-07-21 12:58:43.940897 attr_utils-0.8.1/attr_utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12328 2023-07-21 12:58:43.940897 attr_utils-0.8.1/attr_utils/autoattrs.py
```

### Comparing `attr_utils-0.8.0/LICENSE` & `attr_utils-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `attr_utils-0.8.0/README.rst` & `attr_utils-0.8.1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -97,15 +97,15 @@
 .. |license| image:: https://img.shields.io/github/license/domdfcoding/attr_utils
 	:target: https://github.com/domdfcoding/attr_utils/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/domdfcoding/attr_utils
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/attr_utils/v0.8.0
+.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/attr_utils/v0.8.1
 	:target: https://github.com/domdfcoding/attr_utils/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/domdfcoding/attr_utils
 	:target: https://github.com/domdfcoding/attr_utils/commit/master
 	:alt: GitHub last commit
```

### Comparing `attr_utils-0.8.0/PKG-INFO` & `attr_utils-0.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: attr-utils
-Version: 0.8.0
+Version: 0.8.1
 Summary: Utilities to augment attrs.
 Author-email: Dominic Davis-Foster <dominic@davis-foster.co.uk>
 License: MIT
 Keywords: attrs,documentation,serde,sphinx
 Home-page: https://github.com/domdfcoding/attr_utils
 Project-URL: Issue Tracker, https://github.com/domdfcoding/attr_utils/issues
 Project-URL: Source Code, https://github.com/domdfcoding/attr_utils
@@ -144,15 +144,15 @@
 .. |license| image:: https://img.shields.io/github/license/domdfcoding/attr_utils
 	:target: https://github.com/domdfcoding/attr_utils/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/domdfcoding/attr_utils
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/attr_utils/v0.8.0
+.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/attr_utils/v0.8.1
 	:target: https://github.com/domdfcoding/attr_utils/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/domdfcoding/attr_utils
 	:target: https://github.com/domdfcoding/attr_utils/commit/master
 	:alt: GitHub last commit
```

### Comparing `attr_utils-0.8.0/pyproject.toml` & `attr_utils-0.8.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "whey",]
 build-backend = "whey"
 
 [project]
 name = "attr_utils"
-version = "0.8.0"
+version = "0.8.1"
 description = "Utilities to augment attrs."
 readme = "README.rst"
 keywords = [ "attrs", "documentation", "serde", "sphinx",]
 dynamic = []
 dependencies = [
     "attrs>=19.3.0",
     "domdf-python-tools>=2.9.0",
```

### Comparing `attr_utils-0.8.0/attr_utils/docstrings.py` & `attr_utils-0.8.1/attr_utils/docstrings.py`

 * *Files identical despite different names*

### Comparing `attr_utils-0.8.0/attr_utils/serialise.py` & `attr_utils-0.8.1/attr_utils/serialise.py`

 * *Files identical despite different names*

### Comparing `attr_utils-0.8.0/attr_utils/__init__.py` & `attr_utils-0.8.1/attr_utils/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,11 +25,11 @@
 #  OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE
 #  OR OTHER DEALINGS IN THE SOFTWARE.
 #
 
 __author__: str = "Dominic Davis-Foster"
 __copyright__: str = "2020 Dominic Davis-Foster"
 __license__: str = "MIT License"
-__version__: str = "0.8.0"
+__version__: str = "0.8.1"
 __email__: str = "dominic@davis-foster.co.uk"
 
 _docs = False
```

### Comparing `attr_utils-0.8.0/attr_utils/mypy_plugin.py` & `attr_utils-0.8.1/attr_utils/mypy_plugin.py`

 * *Files identical despite different names*

### Comparing `attr_utils-0.8.0/attr_utils/annotations.py` & `attr_utils-0.8.1/attr_utils/annotations.py`

 * *Files identical despite different names*

### Comparing `attr_utils-0.8.0/attr_utils/pprinter.py` & `attr_utils-0.8.1/attr_utils/pprinter.py`

 * *Files identical despite different names*

### Comparing `attr_utils-0.8.0/attr_utils/utils.py` & `attr_utils-0.8.1/attr_utils/utils.py`

 * *Files identical despite different names*

### Comparing `attr_utils-0.8.0/attr_utils/autoattrs.py` & `attr_utils-0.8.1/attr_utils/autoattrs.py`

 * *Files 0% similar despite different names*

```diff
@@ -170,22 +170,22 @@
 
 		with warnings.catch_warnings():
 			# TODO: work out what to do about this
 			warnings.simplefilter("ignore", RemovedInSphinx50Warning)
 			Documenter.add_content(self, more_content, True)
 
 		# set sourcename and add content from attribute documentation
-		# sourcename = self.get_sourcename()
+		sourcename = self.get_sourcename()
 
-		# params, pre_output, post_output = self._get_docstring()
+		params, pre_output, post_output = self._get_docstring()
 
-		# self.add_line('', sourcename)
-		# for line in list(self.process_doc([pre_output])):
-		# 	self.add_line(line, sourcename)
-		# self.add_line('', sourcename)
+		self.add_line('', sourcename)
+		for line in list(self.process_doc([pre_output])):
+			self.add_line(line, sourcename)
+		self.add_line('', sourcename)
 
 	def _get_docstring(self) -> Tuple[Dict[str, Param], List[str], List[str]]:
 		"""
 		Returns params, pre_output, post_output.
 		"""
 
 		# Size varies depending on docutils config
@@ -262,15 +262,17 @@
 
 			field_entry = [f":param {field}:", *doc]
 			parameter_docs.append(' '.join(field_entry))
 			all_docs[field] = ''.join(doc).strip()
 
 		self.add_line('', sourcename)
 
-		for line in list(self.process_doc([[*pre_output, *parameter_docs, '', '', *post_output]])):
+		for line in self.process_doc([[*pre_output, *parameter_docs, '', '', *post_output]]):
+			if line and line in pre_output:
+				continue
 			self.add_line(line, sourcename)
 		self.add_line('', sourcename)
 
 		self._docstring_processed = True
 
 		if hasattr(self.object, "__slots__"):
 			slots_dict: MutableMapping[str, Optional[str]] = {}
```

