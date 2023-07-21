# Comparing `tmp/attr_utils-0.7.0.tar.gz` & `tmp/attr_utils-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "attr_utils-0.7.0.tar", last modified: Sun Jan 16 07:29:19 2022, max compression
+gzip compressed data, was "attr_utils-0.8.0.tar", last modified: Fri Jul 21 08:56:11 2023, max compression
```

## Comparing `attr_utils-0.7.0.tar` & `attr_utils-0.8.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0 runner    (1001) docker     (121)      128 2022-01-16 07:29:19.295309 attr_utils-0.7.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4926 2022-01-16 07:29:19.291309 attr_utils-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     5323 2022-01-16 07:29:19.295309 attr_utils-0.7.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)     7246 2022-01-16 07:29:19.379310 attr_utils-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1064 2022-01-16 07:29:19.287310 attr_utils-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     8224 2022-01-16 07:28:46.703354 attr_utils-0.7.0/attr_utils/mypy_plugin.py
--rw-r--r--   0 runner    (1001) docker     (121)     4165 2022-01-16 07:28:46.703354 attr_utils-0.7.0/attr_utils/docstrings.py
--rw-r--r--   0 runner    (1001) docker     (121)     1440 2022-01-16 07:28:46.703354 attr_utils-0.7.0/attr_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6609 2022-01-16 07:28:46.703354 attr_utils-0.7.0/attr_utils/serialise.py
--rw-r--r--   0 runner    (1001) docker     (121)    11993 2022-01-16 07:28:46.703354 attr_utils-0.7.0/attr_utils/autoattrs.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-16 07:28:46.703354 attr_utils-0.7.0/attr_utils/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)     1587 2022-01-16 07:28:46.703354 attr_utils-0.7.0/attr_utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     6047 2022-01-16 07:28:46.703354 attr_utils-0.7.0/attr_utils/pprinter.py
--rw-r--r--   0 runner    (1001) docker     (121)     8767 2022-01-16 07:28:46.703354 attr_utils-0.7.0/attr_utils/annotations.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1064 2023-07-21 08:56:11.723672 attr_utils-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      128 2023-07-21 08:56:11.731672 attr_utils-0.8.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     5325 2023-07-21 08:56:11.731672 attr_utils-0.8.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     7299 2023-07-21 08:56:11.735672 attr_utils-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5000 2023-07-21 08:56:11.731672 attr_utils-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)     4206 2023-07-21 08:55:30.167565 attr_utils-0.8.0/attr_utils/docstrings.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6609 2023-07-21 08:55:30.167565 attr_utils-0.8.0/attr_utils/serialise.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1440 2023-07-21 08:55:30.167565 attr_utils-0.8.0/attr_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8224 2023-07-21 08:55:30.167565 attr_utils-0.8.0/attr_utils/mypy_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8713 2023-07-21 08:55:30.167565 attr_utils-0.8.0/attr_utils/annotations.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-21 08:55:30.167565 attr_utils-0.8.0/attr_utils/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)     6047 2023-07-21 08:55:30.167565 attr_utils-0.8.0/attr_utils/pprinter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1707 2023-07-21 08:55:30.167565 attr_utils-0.8.0/attr_utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12298 2023-07-21 08:55:30.167565 attr_utils-0.8.0/attr_utils/autoattrs.py
```

### Comparing `attr_utils-0.7.0/pyproject.toml` & `attr_utils-0.8.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "whey",]
 build-backend = "whey"
 
 [project]
 name = "attr_utils"
-version = "0.7.0"
+version = "0.8.0"
 description = "Utilities to augment attrs."
 readme = "README.rst"
 keywords = [ "attrs", "documentation", "serde", "sphinx",]
 dynamic = []
 dependencies = [
     "attrs>=19.3.0",
     "domdf-python-tools>=2.9.0",
@@ -19,14 +19,15 @@
 classifiers = [
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
     "Topic :: Software Development :: Libraries :: Python Modules",
@@ -42,20 +43,20 @@
 [project.license]
 file = "LICENSE"
 
 [project.urls]
 Homepage = "https://github.com/domdfcoding/attr_utils"
 "Issue Tracker" = "https://github.com/domdfcoding/attr_utils/issues"
 "Source Code" = "https://github.com/domdfcoding/attr_utils"
-Documentation = "https://attr_utils.readthedocs.io/en/latest"
+Documentation = "https://attr-utils.readthedocs.io/en/latest"
 
 [project.optional-dependencies]
 pprint = [ "prettyprinter==0.18.0",]
-sphinx = [ "sphinx<3.4.0,>=3.2.0", "sphinx-toolbox>=2.12.1",]
-all = [ "prettyprinter==0.18.0", "sphinx<3.4.0,>=3.2.0", "sphinx-toolbox>=2.12.1",]
+sphinx = [ "sphinx<3.4.0,>=3.2.0", "sphinx-toolbox>=2.16.0",]
+all = [ "prettyprinter==0.18.0", "sphinx<3.4.0,>=3.2.0", "sphinx-toolbox>=2.16.0",]
 
 [tool.mkrecipe]
 conda-channels = [ "conda-forge", "domdfcoding",]
 extras = "all"
 license-key = "MIT"
 
 [tool.sphinx-pyproject]
@@ -68,25 +69,25 @@
 package_root = "attr_utils"
 extensions = [
     "sphinx_toolbox",
     "sphinx_toolbox.more_autodoc",
     "sphinx_toolbox.more_autosummary",
     "sphinx_toolbox.documentation_summary",
     "sphinx_toolbox.tweaks.param_dash",
+    "sphinxcontrib.toctree_plus",
     "sphinx_toolbox.tweaks.latex_layout",
     "sphinx_toolbox.tweaks.latex_toc",
     "sphinx.ext.intersphinx",
     "sphinx.ext.mathjax",
     "sphinxcontrib.extras_require",
     "sphinx.ext.todo",
     "sphinxemoji.sphinxemoji",
     "notfound.extension",
     "sphinx_copybutton",
     "sphinxcontrib.default_values",
-    "sphinxcontrib.toctree_plus",
     "sphinx_debuginfo",
     "sphinx_licenseinfo",
     "seed_intersphinx_mapping",
     "html_section",
     "attr_utils.annotations",
     "attr_utils.autoattrs",
     "sphinx_toolbox_experimental.autosummary_widths",
@@ -145,27 +146,28 @@
 
 [tool.whey]
 base-classifiers = [
     "Intended Audience :: Developers",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Typing :: Typed",
 ]
-python-versions = [ "3.6", "3.7", "3.8", "3.9", "3.10",]
+python-versions = [ "3.6", "3.7", "3.8", "3.9", "3.10", "3.11",]
 python-implementations = [ "CPython", "PyPy",]
 platforms = [ "Windows", "macOS", "Linux",]
 license-key = "MIT"
 
 [tool.mypy]
-python_version = "3.6"
+python_version = "3.7"
 namespace_packages = true
 check_untyped_defs = true
 warn_unused_ignores = true
 no_implicit_optional = true
 show_error_codes = true
 plugins = [ "attr_utils.mypy_plugin",]
+incremental = false
 
 [tool.snippet-fmt]
 directives = [ "code-block",]
 
 [tool.dep_checker.name_mapping]
 attrs = "attr"
```

### Comparing `attr_utils-0.7.0/README.rst` & `attr_utils-0.8.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -26,16 +26,16 @@
 	* - Activity
 	  - |commits-latest| |commits-since| |maintained| |pypi-downloads|
 	* - QA
 	  - |codefactor| |actions_flake8| |actions_mypy|
 	* - Other
 	  - |license| |language| |requires|
 
-.. |docs| image:: https://img.shields.io/readthedocs/attr_utils/latest?logo=read-the-docs
-	:target: https://attr_utils.readthedocs.io/en/latest
+.. |docs| image:: https://img.shields.io/readthedocs/attr-utils/latest?logo=read-the-docs
+	:target: https://attr-utils.readthedocs.io/en/latest
 	:alt: Documentation Build Status
 
 .. |docs_check| image:: https://github.com/domdfcoding/attr_utils/workflows/Docs%20Check/badge.svg
 	:target: https://github.com/domdfcoding/attr_utils/actions?query=workflow%3A%22Docs+Check%22
 	:alt: Docs Check Status
 
 .. |actions_linux| image:: https://github.com/domdfcoding/attr_utils/workflows/Linux/badge.svg
@@ -54,16 +54,16 @@
 	:target: https://github.com/domdfcoding/attr_utils/actions?query=workflow%3A%22Flake8%22
 	:alt: Flake8 Status
 
 .. |actions_mypy| image:: https://github.com/domdfcoding/attr_utils/workflows/mypy/badge.svg
 	:target: https://github.com/domdfcoding/attr_utils/actions?query=workflow%3A%22mypy%22
 	:alt: mypy status
 
-.. |requires| image:: https://dependency-dash.herokuapp.com/github/domdfcoding/attr_utils/badge.svg
-	:target: https://dependency-dash.herokuapp.com/github/domdfcoding/attr_utils/
+.. |requires| image:: https://dependency-dash.repo-helper.uk/github/domdfcoding/attr_utils/badge.svg
+	:target: https://dependency-dash.repo-helper.uk/github/domdfcoding/attr_utils/
 	:alt: Requirements Status
 
 .. |coveralls| image:: https://img.shields.io/coveralls/github/domdfcoding/attr_utils/master?logo=coveralls
 	:target: https://coveralls.io/github/domdfcoding/attr_utils?branch=master
 	:alt: Coverage
 
 .. |codefactor| image:: https://img.shields.io/codefactor/grade/github/domdfcoding/attr_utils?logo=codefactor
@@ -97,23 +97,23 @@
 .. |license| image:: https://img.shields.io/github/license/domdfcoding/attr_utils
 	:target: https://github.com/domdfcoding/attr_utils/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/domdfcoding/attr_utils
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/attr_utils/v0.7.0
+.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/attr_utils/v0.8.0
 	:target: https://github.com/domdfcoding/attr_utils/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/domdfcoding/attr_utils
 	:target: https://github.com/domdfcoding/attr_utils/commit/master
 	:alt: GitHub last commit
 
-.. |maintained| image:: https://img.shields.io/maintenance/yes/2022
+.. |maintained| image:: https://img.shields.io/maintenance/yes/2023
 	:alt: Maintenance
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/attr_utils
 	:target: https://pypi.org/project/attr_utils/
 	:alt: PyPI - Downloads
 
 .. end shields
```

### Comparing `attr_utils-0.7.0/PKG-INFO` & `attr_utils-0.8.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,50 +1,51 @@
 Metadata-Version: 2.1
 Name: attr-utils
-Version: 0.7.0
+Version: 0.8.0
 Summary: Utilities to augment attrs.
 Author-email: Dominic Davis-Foster <dominic@davis-foster.co.uk>
 License: MIT
 Keywords: attrs,documentation,serde,sphinx
 Home-page: https://github.com/domdfcoding/attr_utils
 Project-URL: Issue Tracker, https://github.com/domdfcoding/attr_utils/issues
 Project-URL: Source Code, https://github.com/domdfcoding/attr_utils
-Project-URL: Documentation, https://attr_utils.readthedocs.io/en/latest
+Project-URL: Documentation, https://attr-utils.readthedocs.io/en/latest
 Platform: Windows
 Platform: macOS
 Platform: Linux
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
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
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Python: >=3.6
 Requires-Dist: attrs>=19.3.0
 Requires-Dist: domdf-python-tools>=2.9.0
 Requires-Dist: toolz>=0.11.1
 Requires-Dist: typing-extensions>=3.7.4.3
 Requires-Dist: typing-inspect>=0.6.0; python_version == "3.6"
-Provides-Extra: pprint
 Requires-Dist: prettyprinter==0.18.0; extra == 'pprint'
-Provides-Extra: sphinx
 Requires-Dist: sphinx<3.4.0,>=3.2.0; extra == 'sphinx'
-Requires-Dist: sphinx-toolbox>=2.12.1; extra == 'sphinx'
-Provides-Extra: all
+Requires-Dist: sphinx-toolbox>=2.16.0; extra == 'sphinx'
 Requires-Dist: prettyprinter==0.18.0; extra == 'all'
 Requires-Dist: sphinx<3.4.0,>=3.2.0; extra == 'all'
-Requires-Dist: sphinx-toolbox>=2.12.1; extra == 'all'
+Requires-Dist: sphinx-toolbox>=2.16.0; extra == 'all'
+Provides-Extra: pprint
+Provides-Extra: sphinx
+Provides-Extra: all
 Description-Content-Type: text/x-rst
 
 
 ###########
 attr_utils
 ###########
 
@@ -72,16 +73,16 @@
 	* - Activity
 	  - |commits-latest| |commits-since| |maintained| |pypi-downloads|
 	* - QA
 	  - |codefactor| |actions_flake8| |actions_mypy|
 	* - Other
 	  - |license| |language| |requires|
 
-.. |docs| image:: https://img.shields.io/readthedocs/attr_utils/latest?logo=read-the-docs
-	:target: https://attr_utils.readthedocs.io/en/latest
+.. |docs| image:: https://img.shields.io/readthedocs/attr-utils/latest?logo=read-the-docs
+	:target: https://attr-utils.readthedocs.io/en/latest
 	:alt: Documentation Build Status
 
 .. |docs_check| image:: https://github.com/domdfcoding/attr_utils/workflows/Docs%20Check/badge.svg
 	:target: https://github.com/domdfcoding/attr_utils/actions?query=workflow%3A%22Docs+Check%22
 	:alt: Docs Check Status
 
 .. |actions_linux| image:: https://github.com/domdfcoding/attr_utils/workflows/Linux/badge.svg
@@ -100,16 +101,16 @@
 	:target: https://github.com/domdfcoding/attr_utils/actions?query=workflow%3A%22Flake8%22
 	:alt: Flake8 Status
 
 .. |actions_mypy| image:: https://github.com/domdfcoding/attr_utils/workflows/mypy/badge.svg
 	:target: https://github.com/domdfcoding/attr_utils/actions?query=workflow%3A%22mypy%22
 	:alt: mypy status
 
-.. |requires| image:: https://dependency-dash.herokuapp.com/github/domdfcoding/attr_utils/badge.svg
-	:target: https://dependency-dash.herokuapp.com/github/domdfcoding/attr_utils/
+.. |requires| image:: https://dependency-dash.repo-helper.uk/github/domdfcoding/attr_utils/badge.svg
+	:target: https://dependency-dash.repo-helper.uk/github/domdfcoding/attr_utils/
 	:alt: Requirements Status
 
 .. |coveralls| image:: https://img.shields.io/coveralls/github/domdfcoding/attr_utils/master?logo=coveralls
 	:target: https://coveralls.io/github/domdfcoding/attr_utils?branch=master
 	:alt: Coverage
 
 .. |codefactor| image:: https://img.shields.io/codefactor/grade/github/domdfcoding/attr_utils?logo=codefactor
@@ -143,23 +144,23 @@
 .. |license| image:: https://img.shields.io/github/license/domdfcoding/attr_utils
 	:target: https://github.com/domdfcoding/attr_utils/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/domdfcoding/attr_utils
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/attr_utils/v0.7.0
+.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/attr_utils/v0.8.0
 	:target: https://github.com/domdfcoding/attr_utils/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/domdfcoding/attr_utils
 	:target: https://github.com/domdfcoding/attr_utils/commit/master
 	:alt: GitHub last commit
 
-.. |maintained| image:: https://img.shields.io/maintenance/yes/2022
+.. |maintained| image:: https://img.shields.io/maintenance/yes/2023
 	:alt: Maintenance
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/attr_utils
 	:target: https://pypi.org/project/attr_utils/
 	:alt: PyPI - Downloads
 
 .. end shields
```

### Comparing `attr_utils-0.7.0/LICENSE` & `attr_utils-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `attr_utils-0.7.0/attr_utils/mypy_plugin.py` & `attr_utils-0.8.0/attr_utils/mypy_plugin.py`

 * *Files identical despite different names*

### Comparing `attr_utils-0.7.0/attr_utils/docstrings.py` & `attr_utils-0.8.0/attr_utils/docstrings.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 #  DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR
 #  OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE
 #  OR OTHER DEALINGS IN THE SOFTWARE.
 #
 
 # stdlib
 import re
+import sys
 from types import MethodType
 from typing import Optional, Pattern, Type, TypeVar
 
 # 3rd party
 from domdf_python_tools.compat import PYPY, PYPY37
 from domdf_python_tools.doctools import base_new_docstrings, prettify_docstrings
 from domdf_python_tools.typing import MethodDescriptorType, MethodWrapperType, WrapperDescriptorType
@@ -88,15 +89,15 @@
 		if not PYPY and isinstance(
 				attribute,
 				(WrapperDescriptorType, MethodDescriptorType, MethodWrapperType, MethodType),
 				):
 			continue  # pragma: no cover (!PyPy)
 		elif PYPY and isinstance(attribute, MethodType):
 			continue  # pragma: no cover
-		elif PYPY37:  # pragma: no cover (not (PyPy and py37))
+		elif PYPY and sys.version_info >= (3, 7):  # pragma: no cover (not (PyPy and py37+))
 			if attribute is getattr(object, attr_name, None):
 				continue
 			elif attribute is getattr(float, attr_name, None):
 				continue
 			elif attribute is getattr(str, attr_name, None):
 				continue
```

### Comparing `attr_utils-0.7.0/attr_utils/__init__.py` & `attr_utils-0.8.0/attr_utils/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,11 +25,11 @@
 #  OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE
 #  OR OTHER DEALINGS IN THE SOFTWARE.
 #
 
 __author__: str = "Dominic Davis-Foster"
 __copyright__: str = "2020 Dominic Davis-Foster"
 __license__: str = "MIT License"
-__version__: str = "0.7.0"
+__version__: str = "0.8.0"
 __email__: str = "dominic@davis-foster.co.uk"
 
 _docs = False
```

### Comparing `attr_utils-0.7.0/attr_utils/serialise.py` & `attr_utils-0.8.0/attr_utils/serialise.py`

 * *Files identical despite different names*

### Comparing `attr_utils-0.7.0/attr_utils/autoattrs.py` & `attr_utils-0.8.0/attr_utils/autoattrs.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,20 +93,22 @@
 #  |  DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY
 #  |  THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 #  |  (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 #  |  OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 #
 
 # stdlib
+import warnings
 from textwrap import dedent
 from typing import Any, Dict, List, MutableMapping, Optional, Tuple, Type
 
 # 3rd party
 import attr
 from sphinx.application import Sphinx  # nodep
+from sphinx.deprecation import RemovedInSphinx50Warning  # nodep
 from sphinx.ext.autodoc import ClassDocumenter, Documenter  # nodep
 from sphinx.pycode import ModuleAnalyzer  # nodep
 from sphinx_toolbox import __version__  # nodep
 from sphinx_toolbox.more_autosummary import PatchedAutoSummClassDocumenter  # nodep
 from sphinx_toolbox.utils import Param, SphinxExtMetadata, flag, parse_parameters, unknown_module_warning  # nodep
 
 # this package
@@ -162,25 +164,28 @@
 		"""
 		Add extra content (from docstrings, attribute docs etc.), but not the class docstring.
 
 		:param more_content:
 		:param no_docstring:
 		"""
 
-		Documenter.add_content(self, more_content, True)
+		with warnings.catch_warnings():
+			# TODO: work out what to do about this
+			warnings.simplefilter("ignore", RemovedInSphinx50Warning)
+			Documenter.add_content(self, more_content, True)
 
 		# set sourcename and add content from attribute documentation
-		sourcename = self.get_sourcename()
+		# sourcename = self.get_sourcename()
 
-		params, pre_output, post_output = self._get_docstring()
+		# params, pre_output, post_output = self._get_docstring()
 
-		self.add_line('', sourcename)
-		for line in list(self.process_doc([pre_output])):
-			self.add_line(line, sourcename)
-		self.add_line('', sourcename)
+		# self.add_line('', sourcename)
+		# for line in list(self.process_doc([pre_output])):
+		# 	self.add_line(line, sourcename)
+		# self.add_line('', sourcename)
 
 	def _get_docstring(self) -> Tuple[Dict[str, Param], List[str], List[str]]:
 		"""
 		Returns params, pre_output, post_output.
 		"""
 
 		# Size varies depending on docutils config
@@ -256,29 +261,30 @@
 				doc = member_docstrings[field]
 
 			field_entry = [f":param {field}:", *doc]
 			parameter_docs.append(' '.join(field_entry))
 			all_docs[field] = ''.join(doc).strip()
 
 		self.add_line('', sourcename)
-		for line in list(self.process_doc([[*parameter_docs, '', '', *post_output]])):
+
+		for line in list(self.process_doc([[*pre_output, *parameter_docs, '', '', *post_output]])):
 			self.add_line(line, sourcename)
 		self.add_line('', sourcename)
 
 		self._docstring_processed = True
 
 		if hasattr(self.object, "__slots__"):
 			slots_dict: MutableMapping[str, Optional[str]] = {}
-			for item in self.object.__slots__:
+			for item in self.object.__slots__:  # type: ignore[attr-defined]
 				if item in all_docs:
 					slots_dict[item] = all_docs[item]
 				else:
 					slots_dict[item] = None
 
-			self.object.__slots__ = slots_dict
+			self.object.__slots__ = slots_dict  # type: ignore[attr-defined]
 
 		if hasattr(self, "add_autosummary"):
 			self.add_autosummary()
 
 		# import functools
 		#
 		# for documenter in documenters:
```

### Comparing `attr_utils-0.7.0/attr_utils/utils.py` & `attr_utils-0.8.0/attr_utils/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,26 +23,31 @@
 #  IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,
 #  DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR
 #  OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE
 #  OR OTHER DEALINGS IN THE SOFTWARE.
 #
 
 # stdlib
-from typing import Tuple
+from typing import TYPE_CHECKING, Tuple
 
 # 3rd party
 from attr import Attribute
-from typing_extensions import Protocol, runtime_checkable
 
 __all__ = ["AttrsClass"]
 
+if TYPE_CHECKING:
+	# 3rd party
+	from attr import AttrsInstance as AttrsClass
+else:
+	# 3rd party
+	from typing_extensions import Protocol, runtime_checkable
+
+	@runtime_checkable
+	class AttrsClass(Protocol):
+		"""
+		:class:`~typing.Protocol` for attrs classes.
+		"""
 
-@runtime_checkable
-class AttrsClass(Protocol):
-	"""
-	:class:`~typing.Protocol` for attrs classes.
-	"""
+		#: Special attribute used internally by attrs.
+		__attrs_attrs__: Tuple[Attribute, ...]
 
-	#: Special attribute used internally by attrs.
-	__attrs_attrs__: Tuple[Attribute, ...]
-
-	__name__: str
+		__name__: str
```

### Comparing `attr_utils-0.7.0/attr_utils/pprinter.py` & `attr_utils-0.8.0/attr_utils/pprinter.py`

 * *Files identical despite different names*

### Comparing `attr_utils-0.7.0/attr_utils/annotations.py` & `attr_utils-0.8.0/attr_utils/annotations.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,15 +154,15 @@
 	"""
 
 	if not attr.has(obj):  # type: ignore
 		return obj
 
 	annotations: Dict[str, Optional[Type]] = {"return": None}
 
-	attrs = attr.fields(obj)  # type: ignore
+	attrs = attr.fields(obj)
 
 	for a in attrs:
 		arg_name = a.name.lstrip('_')
 
 		if a.init is True and a.type is not None:
 			if a.converter is None:
 				annotations[arg_name] = a.type
@@ -181,20 +181,20 @@
 					signature = inspect.signature(a.converter)
 					arg_type = next(iter(signature.parameters.items()))[1].annotation
 					if arg_type is inspect.Signature.empty:
 						annotations[arg_name] = a.type
 					else:
 						annotations[arg_name] = arg_type
 
-	if hasattr(obj.__init__, "__annotations__"):  # type: ignore
-		obj.__init__.__annotations__.update(annotations)  # type: ignore
+	if hasattr(obj.__init__, "__annotations__"):
+		obj.__init__.__annotations__.update(annotations)
 	else:  # pragma: no cover
-		obj.__init__.__annotations__ = annotations  # type: ignore
+		obj.__init__.__annotations__ = annotations
 
-	return obj
+	return cast(_C, obj)
 
 
 def attrib(
 		default=attr.NOTHING,
 		validator=None,
 		repr: bool = True,  # noqa: A002  # pylint: disable=redefined-builtin
 		hash=None,  # noqa: A002  # pylint: disable=redefined-builtin
```

