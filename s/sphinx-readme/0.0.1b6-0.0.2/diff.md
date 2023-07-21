# Comparing `tmp/sphinx-readme-0.0.1b6.tar.gz` & `tmp/sphinx-readme-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx-readme-0.0.1b6.tar", last modified: Mon Jul 10 13:25:29 2023, max compression
+gzip compressed data, was "sphinx-readme-0.0.2.tar", last modified: Fri Jul 21 06:50:31 2023, max compression
```

## Comparing `sphinx-readme-0.0.1b6.tar` & `sphinx-readme-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 13:25:29.443000 sphinx-readme-0.0.1b6/
--rw-rw-rw-   0        0        0     1084 2023-05-09 12:07:43.000000 sphinx-readme-0.0.1b6/LICENSE
--rw-rw-rw-   0        0        0     9372 2023-07-10 13:25:29.443000 sphinx-readme-0.0.1b6/PKG-INFO
--rw-rw-rw-   0        0        0     8581 2023-07-10 13:24:24.000000 sphinx-readme-0.0.1b6/README.rst
--rw-rw-rw-   0        0        0       42 2023-07-10 13:25:29.443000 sphinx-readme-0.0.1b6/setup.cfg
--rw-rw-rw-   0        0        0     1454 2023-07-07 16:12:34.000000 sphinx-readme-0.0.1b6/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-10 13:25:29.396136 sphinx-readme-0.0.1b6/sphinx_readme/
--rw-rw-rw-   0        0        0     1712 2023-07-10 13:12:35.000000 sphinx-readme-0.0.1b6/sphinx_readme/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-10 13:25:29.443000 sphinx-readme-0.0.1b6/sphinx_readme/config/
--rw-rw-rw-   0        0        0       57 2023-07-10 13:08:55.000000 sphinx-readme-0.0.1b6/sphinx_readme/config/__init__.py
--rw-rw-rw-   0        0        0     7156 2023-07-10 13:08:55.000000 sphinx-readme-0.0.1b6/sphinx_readme/config/linkcode.py
--rw-rw-rw-   0        0        0     9080 2023-07-10 13:08:55.000000 sphinx-readme-0.0.1b6/sphinx_readme/config/main.py
--rw-rw-rw-   0        0        0    20713 2023-07-10 13:08:55.000000 sphinx-readme-0.0.1b6/sphinx_readme/parser.py
--rw-rw-rw-   0        0        0     4878 2023-07-07 16:12:34.000000 sphinx-readme-0.0.1b6/sphinx_readme/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-10 13:25:29.427382 sphinx-readme-0.0.1b6/sphinx_readme.egg-info/
--rw-rw-rw-   0        0        0     9372 2023-07-10 13:25:29.000000 sphinx-readme-0.0.1b6/sphinx_readme.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      379 2023-07-10 13:25:29.000000 sphinx-readme-0.0.1b6/sphinx_readme.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 13:25:29.000000 sphinx-readme-0.0.1b6/sphinx_readme.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-07-10 13:25:29.000000 sphinx-readme-0.0.1b6/sphinx_readme.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-10 13:25:29.000000 sphinx-readme-0.0.1b6/sphinx_readme.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-21 06:50:31.481447 sphinx-readme-0.0.2/
+-rw-rw-rw-   0        0        0     1084 2023-05-09 12:07:43.000000 sphinx-readme-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     9259 2023-07-21 06:50:31.481447 sphinx-readme-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     8470 2023-07-21 06:49:17.000000 sphinx-readme-0.0.2/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-21 06:50:31.481447 sphinx-readme-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1454 2023-07-18 11:51:26.000000 sphinx-readme-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 06:50:31.450206 sphinx-readme-0.0.2/sphinx_readme/
+-rw-rw-rw-   0        0        0     1722 2023-07-21 06:42:57.000000 sphinx-readme-0.0.2/sphinx_readme/__init__.py
+-rw-rw-rw-   0        0        0    11766 2023-07-21 06:42:57.000000 sphinx-readme-0.0.2/sphinx_readme/config.py
+-rw-rw-rw-   0        0        0    27686 2023-07-21 06:42:57.000000 sphinx-readme-0.0.2/sphinx_readme/parser.py
+drwxrwxrwx   0        0        0        0 2023-07-21 06:50:31.481447 sphinx-readme-0.0.2/sphinx_readme/utils/
+-rw-rw-rw-   0        0        0        0 2023-07-21 06:42:57.000000 sphinx-readme-0.0.2/sphinx_readme/utils/__init__.py
+-rw-rw-rw-   0        0        0     4643 2023-07-21 06:42:57.000000 sphinx-readme-0.0.2/sphinx_readme/utils/git.py
+-rw-rw-rw-   0        0        0     3727 2023-07-21 06:42:57.000000 sphinx-readme-0.0.2/sphinx_readme/utils/linkcode.py
+-rw-rw-rw-   0        0        0     4252 2023-07-21 06:42:57.000000 sphinx-readme-0.0.2/sphinx_readme/utils/rst.py
+-rw-rw-rw-   0        0        0      810 2023-07-21 06:42:57.000000 sphinx-readme-0.0.2/sphinx_readme/utils/sphinx.py
+drwxrwxrwx   0        0        0        0 2023-07-21 06:50:31.465826 sphinx-readme-0.0.2/sphinx_readme.egg-info/
+-rw-rw-rw-   0        0        0     9259 2023-07-21 06:50:31.000000 sphinx-readme-0.0.2/sphinx_readme.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      433 2023-07-21 06:50:31.000000 sphinx-readme-0.0.2/sphinx_readme.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 06:50:31.000000 sphinx-readme-0.0.2/sphinx_readme.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-07-21 06:50:31.000000 sphinx-readme-0.0.2/sphinx_readme.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-21 06:50:31.000000 sphinx-readme-0.0.2/sphinx_readme.egg-info/top_level.txt
```

### Comparing `sphinx-readme-0.0.1b6/LICENSE` & `sphinx-readme-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinx-readme-0.0.1b6/PKG-INFO` & `sphinx-readme-0.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-readme
-Version: 0.0.1b6
+Version: 0.0.2
 Summary: Generate Beautiful reStructuredText README.rst for GitHub, PyPi, GitLab, BitBucket
 Home-page: https://github.com/tdkorn/sphinx-readme
 Author: Adam Korn
 Author-email: hello@dailykitten.net
 License: MIT License
 Download-URL: https://github.com/TDKorn/sphinx-readme/tarball/main
 Keywords: sphinx,docutils,sphinx-extension,sphinx-contrib,reStructuredText,rst,reST,parser,rst-parser,README.rst,README,autodoc,linkcode
@@ -14,20 +14,20 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/x-rst; charset=UTF-8
 License-File: LICENSE
 
 .. |.`~.sphinx.ext.autodoc`| replace:: ``autodoc``
 .. _.`~.sphinx.ext.autodoc`: https://www.sphinx-doc.org/en/master/usage/extensions/autodoc.html#module-sphinx.ext.autodoc
-.. |.`sphinx.ext.autodoc`| replace:: ``sphinx.ext.autodoc``
-.. _.`sphinx.ext.autodoc`: https://www.sphinx-doc.org/en/master/usage/extensions/autodoc.html#module-sphinx.ext.autodoc
 .. |.`sphinx.ext.linkcode`| replace:: ``sphinx.ext.linkcode``
 .. _.`sphinx.ext.linkcode`: https://www.sphinx-doc.org/en/master/usage/extensions/linkcode.html#module-sphinx.ext.linkcode
 .. |.`~.parse_intersphinx_node`| replace:: ``parse_intersphinx_node()``
-.. _.`~.parse_intersphinx_node`: https://github.com/TDKorn/sphinx-readme/blob/v0.0.1b6/sphinx_readme/parser.py#L124-L134
+.. _.`~.parse_intersphinx_node`: https://github.com/TDKorn/sphinx-readme/blob/v0.0.2/sphinx_readme/parser.py#L145-L159
+.. |.`sphinx.ext.autodoc`| replace:: ``sphinx.ext.autodoc``
+.. _.`sphinx.ext.autodoc`: https://www.sphinx-doc.org/en/master/usage/extensions/autodoc.html#module-sphinx.ext.autodoc
 .. |attention| replace:: 🔔️
 .. |caution| replace:: ⚠️
 .. |danger| replace:: ☢️
 .. |error| replace:: ⛔
 .. |hint| replace:: 🧠
 .. |important| replace:: 📢
 .. |note| replace:: 📝
@@ -37,31 +37,31 @@
 .. |about| replace:: 📚
 
 .. meta::
    :author: Adam Korn
    :title: Sphinx README
    :description: Sphinx Extension to Generate Beautiful reStructuredText README.rst for GitHub, PyPi, GitLab, BitBucket
 
-
 Sphinx README - Generate Beautiful ``README.rst`` for GitHub, PyPi, GitLab, BitBucket
 --------------------------------------------------------------------------------------
 
-.. image:: https://raw.githubusercontent.com/TDKorn/sphinx-readme/v0.0.1b6/docs/source/_static/logo_readme.png
+.. image:: https://raw.githubusercontent.com/TDKorn/sphinx-readme/v0.0.2/docs/source/_static/logo_transparent.png
    :alt: Sphinx README: Generate Beautiful reStructuredText README.rst for GitHub, PyPi, GitLab, BitBucket
    :align: center
    :width: 25%
 
-
 A Sphinx extension to generate ``README.rst`` files that render beautifully on GitHub, PyPi, GitLab, BitBucket
 
+
 .. |RTD| replace:: **Explore the docs »**
 .. _RTD: https://sphinx-readme.readthedocs.io/en/latest/
 
 |RTD|_
 
+|
 
 .. image:: https://img.shields.io/pypi/v/sphinx-readme?color=eb5202
    :target: https://pypi.org/project/sphinx-readme
    :alt: PyPI Project for Sphinx README: Generate Beautiful reStructuredText README.rst for GitHub, PyPi, GitLab, BitBucket
 
 .. image:: https://img.shields.io/badge/GitHub-sphinx--readme-4f1abc
    :target: https://github.com/tdkorn/sphinx-readme
@@ -71,15 +71,14 @@
    :target: https://pepy.tech/project/sphinx-readme
    :alt: Downloads for Sphinx README
 
 .. image:: https://readthedocs.org/projects/sphinx-readme/badge/?version=latest
    :target: https://sphinx-readme.readthedocs.io/en/latest/?badge=latest
    :alt: Documentation for Sphinx README: Generate Beautiful reStructuredText README.rst for GitHub, PyPi, GitLab, BitBucket
 
-
 |
 
 About Sphinx README
 ~~~~~~~~~~~~~~~~~~~~~~~
 
 
 .. csv-table::
@@ -87,22 +86,22 @@
 
    "``sphinx_readme`` is a ``reStructuredText`` parser that uses Sphinx
    to generate ``rst`` files that render beautifully on
    GitHub, PyPi, GitLab, and BitBucket."
 
 
 
-With ``sphinx_readme``, there's no need to rewrite your ``README.rst`` as a ``README.md`` file
-==============================================================================================
+**With** ``sphinx_readme`` **, there's no need to rewrite your** ``README.rst`` **as a** ``README.md`` **file**
 
 Files generated by ``sphinx_readme`` have nearly identical appearance and functionality
 as ``html`` builds, including |.`sphinx.ext.autodoc`|_ cross-references!
 
+|
 
-.. image:: https://raw.githubusercontent.com/TDKorn/sphinx-readme/v0.0.1b6/docs/source/_static/demo/demo.gif
+.. image:: https://raw.githubusercontent.com/TDKorn/sphinx-readme/v0.0.2/docs/source/_static/demo/demo.gif
    :alt: Demonstration of how reStructuredText README.rst files generated by Sphinx README render on GitHub, PyPi, GitLab, BitBucket
    :width: 75%
 
 
 Features
 ~~~~~~~~~~
 
@@ -156,25 +155,25 @@
  * At minimum, the username and repository name must be specified
  * Please see `HTML Context Settings <https://docs.readthedocs.io/en/stable/guides/edit-source-links-sphinx.html>`_
    to determine the correct dictionary keys for your hosting platform
 
 .. |html_context| replace:: ``html_context``
 .. _html_context: https://www.sphinx-doc.org/en/master/usage/configuration.html#confval-html_context
 
-...
+|
 
 |html_baseurl|_
  The base URL which points to the root of the HTML documentation
 
   Type: ``str``
 
 .. |html_baseurl| replace:: ``html_baseurl``
 .. _html_baseurl: https://www.sphinx-doc.org/en/master/usage/configuration.html#confval-html_baseurl
 
-...
+|
 
 |readme_src_files|_
  An individual or list of ``rst`` files to parse
 
   Type: ``Union[str, List]``
 
 
@@ -183,15 +182,15 @@
 
    "Filepaths should be specified relative to the source directory"
 
 
 .. |readme_src_files| replace:: ``readme_src_files``
 .. _readme_src_files: https://sphinx-readme.readthedocs.io/en/latest/configuration/configuring.html#confval-readme_src_files
 
-...
+|
 
 |readme_docs_url_type|_
  The documentation source to link to when resolving |.`~.sphinx.ext.autodoc`|_ cross-references
 
   Type: ``str``
 
  Must be either ``"code"`` or ``"html"``
@@ -251,16 +250,16 @@
 .. _readme_raw_directive: https://sphinx-readme.readthedocs.io/en/latest/configuration/configuring.html#confval-readme_raw_directive
 
 
 
 .. csv-table::
    :header: |important| Important
 
-   "If generating a ``README`` for a platform that doesn't support ``raw``
-   directives (PyPi, GitLab, and BitBucket), be sure to disable |readme_raw_directive|_:
+   "For platforms that don't support the ``raw`` directive (PyPi, GitLab, and BitBucket),
+   be sure to disable |readme_raw_directive|_:
 
    .. code-block:: python
 
       readme_raw_directive = False"
```

### Comparing `sphinx-readme-0.0.1b6/README.rst` & `sphinx-readme-0.0.2/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 .. |.`~.sphinx.ext.autodoc`| replace:: ``autodoc``
 .. _.`~.sphinx.ext.autodoc`: https://www.sphinx-doc.org/en/master/usage/extensions/autodoc.html#module-sphinx.ext.autodoc
-.. |.`sphinx.ext.autodoc`| replace:: ``sphinx.ext.autodoc``
-.. _.`sphinx.ext.autodoc`: https://www.sphinx-doc.org/en/master/usage/extensions/autodoc.html#module-sphinx.ext.autodoc
 .. |.`sphinx.ext.linkcode`| replace:: ``sphinx.ext.linkcode``
 .. _.`sphinx.ext.linkcode`: https://www.sphinx-doc.org/en/master/usage/extensions/linkcode.html#module-sphinx.ext.linkcode
 .. |.`~.parse_intersphinx_node`| replace:: ``parse_intersphinx_node()``
-.. _.`~.parse_intersphinx_node`: https://github.com/TDKorn/sphinx-readme/blob/v0.0.1b6/sphinx_readme/parser.py#L124-L134
+.. _.`~.parse_intersphinx_node`: https://github.com/TDKorn/sphinx-readme/blob/v0.0.2/sphinx_readme/parser.py#L145-L159
+.. |.`sphinx.ext.autodoc`| replace:: ``sphinx.ext.autodoc``
+.. _.`sphinx.ext.autodoc`: https://www.sphinx-doc.org/en/master/usage/extensions/autodoc.html#module-sphinx.ext.autodoc
 .. |attention| replace:: 🔔️
 .. |caution| replace:: ⚠️
 .. |danger| replace:: ☢️
 .. |error| replace:: ⛔
 .. |hint| replace:: 🧠
 .. |important| replace:: 📢
 .. |note| replace:: 📝
@@ -19,31 +19,31 @@
 .. |about| replace:: 📚
 
 .. meta::
    :author: Adam Korn
    :title: Sphinx README
    :description: Sphinx Extension to Generate Beautiful reStructuredText README.rst for GitHub, PyPi, GitLab, BitBucket
 
-
 Sphinx README - Generate Beautiful ``README.rst`` for GitHub, PyPi, GitLab, BitBucket
 --------------------------------------------------------------------------------------
 
-.. image:: https://raw.githubusercontent.com/TDKorn/sphinx-readme/v0.0.1b6/docs/source/_static/logo_readme.png
+.. image:: https://raw.githubusercontent.com/TDKorn/sphinx-readme/v0.0.2/docs/source/_static/logo_transparent.png
    :alt: Sphinx README: Generate Beautiful reStructuredText README.rst for GitHub, PyPi, GitLab, BitBucket
    :align: center
    :width: 25%
 
-
 A Sphinx extension to generate ``README.rst`` files that render beautifully on GitHub, PyPi, GitLab, BitBucket
 
+
 .. |RTD| replace:: **Explore the docs »**
 .. _RTD: https://sphinx-readme.readthedocs.io/en/latest/
 
 |RTD|_
 
+|
 
 .. image:: https://img.shields.io/pypi/v/sphinx-readme?color=eb5202
    :target: https://pypi.org/project/sphinx-readme
    :alt: PyPI Project for Sphinx README: Generate Beautiful reStructuredText README.rst for GitHub, PyPi, GitLab, BitBucket
 
 .. image:: https://img.shields.io/badge/GitHub-sphinx--readme-4f1abc
    :target: https://github.com/tdkorn/sphinx-readme
@@ -53,15 +53,14 @@
    :target: https://pepy.tech/project/sphinx-readme
    :alt: Downloads for Sphinx README
 
 .. image:: https://readthedocs.org/projects/sphinx-readme/badge/?version=latest
    :target: https://sphinx-readme.readthedocs.io/en/latest/?badge=latest
    :alt: Documentation for Sphinx README: Generate Beautiful reStructuredText README.rst for GitHub, PyPi, GitLab, BitBucket
 
-
 |
 
 About Sphinx README
 ~~~~~~~~~~~~~~~~~~~~~~~
 
 
 .. csv-table::
@@ -69,22 +68,22 @@
 
    "``sphinx_readme`` is a ``reStructuredText`` parser that uses Sphinx
    to generate ``rst`` files that render beautifully on
    GitHub, PyPi, GitLab, and BitBucket."
 
 
 
-With ``sphinx_readme``, there's no need to rewrite your ``README.rst`` as a ``README.md`` file
-==============================================================================================
+**With** ``sphinx_readme`` **, there's no need to rewrite your** ``README.rst`` **as a** ``README.md`` **file**
 
 Files generated by ``sphinx_readme`` have nearly identical appearance and functionality
 as ``html`` builds, including |.`sphinx.ext.autodoc`|_ cross-references!
 
+|
 
-.. image:: https://raw.githubusercontent.com/TDKorn/sphinx-readme/v0.0.1b6/docs/source/_static/demo/demo.gif
+.. image:: https://raw.githubusercontent.com/TDKorn/sphinx-readme/v0.0.2/docs/source/_static/demo/demo.gif
    :alt: Demonstration of how reStructuredText README.rst files generated by Sphinx README render on GitHub, PyPi, GitLab, BitBucket
    :width: 75%
 
 
 Features
 ~~~~~~~~~~
 
@@ -138,25 +137,25 @@
  * At minimum, the username and repository name must be specified
  * Please see `HTML Context Settings <https://docs.readthedocs.io/en/stable/guides/edit-source-links-sphinx.html>`_
    to determine the correct dictionary keys for your hosting platform
 
 .. |html_context| replace:: ``html_context``
 .. _html_context: https://www.sphinx-doc.org/en/master/usage/configuration.html#confval-html_context
 
-...
+|
 
 |html_baseurl|_
  The base URL which points to the root of the HTML documentation
 
   Type: ``str``
 
 .. |html_baseurl| replace:: ``html_baseurl``
 .. _html_baseurl: https://www.sphinx-doc.org/en/master/usage/configuration.html#confval-html_baseurl
 
-...
+|
 
 |readme_src_files|_
  An individual or list of ``rst`` files to parse
 
   Type: ``Union[str, List]``
 
 
@@ -165,15 +164,15 @@
 
    "Filepaths should be specified relative to the source directory"
 
 
 .. |readme_src_files| replace:: ``readme_src_files``
 .. _readme_src_files: https://sphinx-readme.readthedocs.io/en/latest/configuration/configuring.html#confval-readme_src_files
 
-...
+|
 
 |readme_docs_url_type|_
  The documentation source to link to when resolving |.`~.sphinx.ext.autodoc`|_ cross-references
 
   Type: ``str``
 
  Must be either ``"code"`` or ``"html"``
@@ -233,16 +232,16 @@
 .. _readme_raw_directive: https://sphinx-readme.readthedocs.io/en/latest/configuration/configuring.html#confval-readme_raw_directive
 
 
 
 .. csv-table::
    :header: |important| Important
 
-   "If generating a ``README`` for a platform that doesn't support ``raw``
-   directives (PyPi, GitLab, and BitBucket), be sure to disable |readme_raw_directive|_:
+   "For platforms that don't support the ``raw`` directive (PyPi, GitLab, and BitBucket),
+   be sure to disable |readme_raw_directive|_:
 
    .. code-block:: python
 
       readme_raw_directive = False"
```

### Comparing `sphinx-readme-0.0.1b6/setup.py` & `sphinx-readme-0.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `sphinx-readme-0.0.1b6/sphinx_readme/__init__.py` & `sphinx-readme-0.0.2/sphinx_readme/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import os
 import sphinx
 from typing import Dict, Any
 from docutils.nodes import document
 from sphinx.application import Sphinx
 from sphinx.environment import BuildEnvironment
-from sphinx_readme.utils import get_conf_val, set_conf_val
-from sphinx_readme.config import get_repo_dir
+
+from sphinx_readme.utils.sphinx import get_conf_val, set_conf_val
+from sphinx_readme.utils.git import get_repo_dir
 from sphinx_readme.parser import READMEParser
 
 
-__version__ = "v0.0.1b6"
+__version__ = "v0.0.2"
 
 
 def setup(app: Sphinx) -> Dict[str, Any]:
     # Avoid setting up extension if building on ReadTheDocs
     if os.environ.get("READTHEDOCS") == "True":
         return {}
```

### Comparing `sphinx-readme-0.0.1b6/sphinx_readme/parser.py` & `sphinx-readme-0.0.2/sphinx_readme/parser.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,58 +1,71 @@
 import re
-from copy import copy
+import copy
 from pathlib import Path
 from collections import defaultdict
-from typing import Dict, List, Tuple, Set
+from typing import Dict, List, Tuple, Set, Union
 
 from docutils import nodes
-from docutils.nodes import Node, document
+from docutils.nodes import document
 
 from sphinx import addnodes
 from sphinx.application import Sphinx
 from sphinx.testing import restructuredtext
 from sphinx.transforms import SphinxTransformer
 from sphinx.environment import BuildEnvironment
 
 from sphinx_readme.config import READMEConfig
-from sphinx_readme.utils import get_all_variants, escape_rst, format_rst
+from sphinx_readme.utils.rst import get_all_xref_variants, escape_rst, format_rst
 
 
 class READMEParser:
 
+    REFERENCE_MAP = {
+        "ref": [],
+        "doc": []
+    }
+
     def __init__(self, app: Sphinx):
-        self.config = READMEConfig(app)
+        #: The :class:`~.READMEConfig` for the parser
+        self.config: READMEConfig = READMEConfig(app)
         self.logger = self.config.logger
-        self.ref_map = self.config.ref_map
-        self.sources = self.config.source_files
-        self.toctrees = defaultdict(list)
-        self.admonitions = {}
-        self.titles = {}
+        #: Mapping of info for standard and :mod:`sphinx.ext.autodoc` cross-references
+        self.ref_map: Dict[str, Union[List, Dict]] = copy.deepcopy(self.REFERENCE_MAP)
+        #: Mapping of source files to their content
+        self.sources: Dict[str, str] = self.config.sources
+        #: Mapping of source files to their toctree data
+        self.toctrees: Dict[str, List[Dict]] = defaultdict(list)
+        # Mapping of source files to their admonition data
+        self.admonitions: Dict[str, Dict[str, List[Dict]]] = {}
+        # Mapping of docnames to their parsed titles
+        self.titles: Dict[str, str] = {}
 
-    def parse(self, app: Sphinx, doctree: document, docname: str):
+    def parse(self, app: Sphinx, doctree: document, docname: str) -> None:
+        """Parses cross-reference, admonition, and toctree data from a resolved doctree"""
         # If a source has ``only`` directives, its doctree will have missing/extra content
-        # Replace the ``only`` directives, then generate a new doctree if needed
+        # Replace the ``only`` directives, then generate a new doctree to parse if needed
         doctree = self.get_doctree(app, doctree, docname)
 
         inline_nodes = list(doctree.findall(nodes.inline))
         literal_nodes = list(doctree.findall(nodes.literal))
 
         self.parse_autodoc_nodes(literal_nodes, docname)
 
         if self.config.docs_url_type == "code":
             self.parse_linkcode_nodes(inline_nodes)
 
-        for node in list(doctree.findall(addnodes.toctree)):
-            self.parse_toctree(node, doctree)
-
         if doctree.get('source') in self.sources:
             self.parse_xref_nodes(inline_nodes)
             self.parse_admonitions(doctree)
+            self.parse_toctrees(doctree)
 
     def get_doctree(self, app: Sphinx, doctree: document, docname: str) -> document:
+        """Generates and resolves a new doctree for :attr:`~.src_files`
+        that contain :rst:dir:`only` directives
+        """
         # Return original doctree if file is not a readme source
         if (src := doctree.get('source')) not in self.sources:
             return doctree
 
         # Parse ``only`` directives to get true source rst of README version
         parsed_rst = self.config.read_rst(src, replace_only=True)
         raw_rst = self.sources[src]
@@ -67,45 +80,53 @@
         docname = docname + "_readme"
 
         # Generate new doctree from parsed rst using Sphinx application
         doctree = restructuredtext.parse(app, parsed_rst, docname)
 
         # Resolve references in the doctree
         try:
-            backup = copy(app.env.temp_data)
+            backup = copy.deepcopy(app.env.temp_data)
             app.env.temp_data['docname'] = docname
 
             transformer = SphinxTransformer(doctree)
             transformer.set_environment(app.env)
             transformer.add_transforms(app.registry.get_post_transforms())
             transformer.apply_transforms()
 
         finally:
             app.env.temp_data = backup
 
         # Replace temp source with actual source
         doctree['source'] = src
         return doctree
 
-    def parse_xref_nodes(self, inline_nodes: List[nodes.inline]):
+    def parse_xref_nodes(self, inline_nodes: List[nodes.inline]) -> None:
+        """Adds node data from :rst:role:`doc` or :rst:role:`ref` cross-references to the :attr:`~ref_map`
+
+        :param inline_nodes: the inline nodes from the document being parsed
+        """
         for node in inline_nodes:
             if 'doc' in node['classes']:
                 self.ref_map['doc'].append(self._parse_xref(node))
 
             elif 'std-ref' in node['classes']:
                 self.ref_map['ref'].append(self._parse_xref(node))
 
-    def _parse_xref(self, node: nodes.inline) -> Dict:
+    def _parse_xref(self, node: nodes.inline) -> Dict[str, str]:
         """Helper function to parse target info of a ``:ref:`` or ``:doc:`` xref"""
         return {
             'text': node.children[0].astext(),
             "refuri": self.config.html_baseurl + "/" + node.parent.get('refuri', '')
         }
 
-    def parse_autodoc_nodes(self, literal_nodes: List[nodes.literal], docname: str):
+    def parse_autodoc_nodes(self, literal_nodes: List[nodes.literal], docname: str) -> None:
+        """Parses node data from :mod:`sphinx.ext.autodoc` cross-references
+
+        :param literal_nodes: the literal nodes from the document being parsed
+        """
         for node in literal_nodes:
             if 'py' not in node['classes']:
                 continue
 
             if not isinstance(node.parent, nodes.reference):
                 continue
 
@@ -117,83 +138,118 @@
                 # Parse :mod: xrefs regardless of docs_url_type
                 self.parse_module_node(node, docname)
 
             elif self.config.docs_url_type == "html":
                 # Only parse remaining py xrefs if linking to html
                 self.parse_autodoc_node(node, docname)
 
-    def parse_intersphinx_node(self, node: nodes.literal):
+    def parse_intersphinx_node(self, node: nodes.literal) -> None:
+        """Adds node data from a :mod:`sphinx.ext.intersphinx` cross-reference to the :attr:`~ref_map`
+
+        :param node: the literal node of an external :mod:`~sphinx.ext.autodoc` reference
+        """
         pattern = r":(mod|class|meth|func|attr):`~?\.?[.\w]+`"
         match = re.match(pattern, node.rawsource)
         target = node.parent.get('refuri')
 
         if not all((match, target)):
             return
 
         is_callable = match.group(1) in ("meth", "func")
         qualified_name = target.split("#")[-1].split("-")[-1]
         self.add_variants(qualified_name, target, is_callable)
 
-    def parse_module_node(self, node: Node, docname: str):
+    def parse_module_node(self, node: nodes.literal, docname: str) -> None:
+        """Adds node data from a ``:mod:`` cross-reference to the :attr:`ref_map`
+
+        :param node: a literal node with the ``"py-mod"`` class
+        :param docname: the name of the document containing the node
+        """
         qualified_name = node.parent.get("reftitle", "")
 
         if self.config.docs_url_type == 'code':
             # Ex. sphinx_readme.parser -> sphinx_readme/parser.py
             refuri = qualified_name.replace('.', '/') + '.py'
         else:
             refuri = self._parse_refuri(node, docname)
 
         if not all((qualified_name, refuri)):
             return
 
         target = f"{self.config.docs_url}/{refuri}"
         self.add_variants(qualified_name, target)
 
-    def parse_autodoc_node(self, node: nodes.literal, docname: str):
+    def parse_autodoc_node(self, node: nodes.literal, docname: str) -> None:
+        """Adds node data from any :mod:`sphinx.ext.autodoc` cross-reference except ``:mod:`` to the :attr:`ref_map`
+
+        :param node: a literal node with the ``"py-{class|func|meth|attr}"`` class
+        :param docname: the name of the document containing the node
+        """
         qualified_name = node.parent.get("reftitle")
         refuri = self._parse_refuri(node, docname)
 
         if not all((refuri, qualified_name)):
             return
 
         is_callable = bool(re.match(r":(meth|func):", node.rawsource))
         target = f"{self.config.docs_url}/{refuri}"
         self.add_variants(qualified_name, target, is_callable)
 
-    def _parse_refuri(self, node: Node, docname: str):
+    def _parse_refuri(self, node: nodes.literal, docname: str) -> str:
+        """Helper function to parse the target of a :mod:`sphinx.ext.autodoc` cross-reference"""
         if 'refuri' in node.parent:
             # Ex. ../parser.html#sphinx_readme.parser.READMEParser
             return node.parent["refuri"].lstrip("./")
 
         elif 'refid' in node.parent:
             # Ex. sphinx_readme.parser.READMEParser
             return f"{docname}.html#{node.parent['refid']}"
 
-    def parse_linkcode_nodes(self, inline_nodes: List[nodes.inline]):
+    def parse_linkcode_nodes(self, inline_nodes: List[nodes.inline]) -> None:
+        """Parses data from nodes added by :mod:`sphinx.ext.linkcode`
+
+        :param inline_nodes: the inline nodes from the document being parsed
+        """
         for node in inline_nodes:
             if 'viewcode-link' in node['classes'] or 'linkcode-link' in node['classes']:
                 if node.parent.get('internal') is False:
                     # Only parse links to external source code
                     self.parse_linkcode_node(node)
 
-    def parse_linkcode_node(self, node: nodes.inline):
+    def parse_linkcode_node(self, node: nodes.inline) -> None:
+        """Adds node data from a :mod:`~sphinx.ext.linkcode` node to the :attr:`ref_map`
+
+        :param node: an inline node added by :mod:`sphinx.ext.linkcode`
+        """
         grandparent = node.parent.parent
         is_callable = grandparent.get("_toc_name", "").endswith("()")
 
         try:
             qualified_name = grandparent.get("ids")[0]
         except IndexError:
             qualified_name = grandparent.get("module", "") + grandparent.get("fullname", "")
 
         target = node.parent.get("refuri")
         self.add_variants(qualified_name, target, is_callable)
 
-    def add_variants(self, qualified_name, target, is_callable: bool = False):
+    def add_variants(self, qualified_name: str, target: str, is_callable: bool = False):
+        """Adds substitution information for an object to the :attr:`ref_map`
+
+        This data is used to replace any :mod:`~sphinx.ext.autodoc` cross-reference to
+        the object with a substitution, hyperlinked to the corresponding
+        source code or documentation entry
+
+        .. tip:: See :func:`~.get_all_xref_variants` and :meth:`replace_autodoc_refs`
+
+        :param qualified_name: the fully qualified name of an object (ex. ``"sphinx_readme.parser.add_variants"``)
+        :param target: the refuri of the object's corresponding source code or documentation entry
+        :param is_callable: specifies if the object is a method or function
+        """
         short_ref = qualified_name.split('.')[-1]
-        variants = get_all_variants(qualified_name)
+        variants = get_all_xref_variants(qualified_name)
 
         for variant in variants:
             if variant in self.ref_map:
                 continue
 
             if variant.startswith("~"):
                 replace = short_ref
@@ -202,46 +258,58 @@
 
             if is_callable:
                 replace += "()"
 
             if self.config.inline_markup:
                 replace = f"``{replace}``"
 
-            self.ref_map[variant].update({
-                'target': target,
-                'replace': replace
-            })
+            self.ref_map[variant] = {
+                'replace': replace,
+                'target': target
+            }
 
-    def parse_titles(self, env: BuildEnvironment):
-        for fname, title_node in env.titles.items():
+    def parse_titles(self, env: BuildEnvironment) -> None:
+        """Parses document titles from the :class:`~.BuildEnvironment`"""
+        for docname, title_node in env.titles.items():
             parts = []
 
             for child in title_node.children:
                 text = child.astext()
                 if isinstance(child, nodes.literal):
                     parts.append(f"``{text}``")
                 else:
                     parts.append(text)
 
-            self.titles[fname] = ' '.join(parts)
+            self.titles[docname] = ' '.join(parts)
 
-    def parse_toctree(self, toctree: Node, doctree: addnodes.document):
-        src = doctree.get('source')
-        toc = {
-            'caption': toctree.get('caption'),
-            'entries': []
-        }
-        for _, entry in toctree.get('entries', []):
-            toc['entries'].append({
-                'entry': entry,
-                'title': self.titles.get(entry),
-            })
-        self.toctrees[src].append(toc)
+    def parse_toctrees(self, doctree: addnodes.document) -> None:
+        """Parses the caption and entry data from :class:`~.sphinx.addnodes.toctree` nodes
 
-    def parse_admonitions(self, doctree: Node):
+        .. caution:: Toctrees are currently parsed as if the directive has the ``:titlesonly:`` option
+
+        :param doctree: the doctree from one of the :attr:`~.src_files`
+        """
+        source = doctree.get('source')
+        for toctree in list(doctree.findall(addnodes.toctree)):
+            toc = {
+                'caption': toctree.get('caption'),
+                'entries': []
+            }
+            for _, entry in toctree.get('entries', []):
+                toc['entries'].append({
+                    'entry': entry,
+                    'title': self.titles.get(entry),
+                })
+            self.toctrees[source].append(toc)
+
+    def parse_admonitions(self, doctree: nodes.document) -> None:
+        """Parses data from generic and specific admonitions
+
+        :param doctree: the doctree from one of the :attr:`~.src_files`
+        """
         admonitions = {'generic': [], 'specific': []}
         src = doctree.get('source')
 
         for admonition in list(doctree.findall(nodes.Admonition)):
             info = {
                 'body': admonition.rawsource
             }
@@ -258,24 +326,28 @@
                     'class': admonition.tagname,
                     'title': admonition.tagname.title(),
                 })
                 admonitions['specific'].append(info)
 
         self.admonitions[src] = admonitions
 
-    def resolve(self):
+    def resolve(self) -> None:
+        """Uses the data from :meth:`parse` to replace cross-references and directives in the :attr:`~.src_files`
+
+        Once resolved, files are written to the :attr:`~.out_dir`.
+        """
         for src, rst in self.sources.items():
             # Replace everything using data from ``parse()``
             rst = self.replace_admonitions(src, rst)
             rst = self.replace_rst_images(src, rst)
             rst = self.replace_toctrees(src, rst)
             rst = self.replace_rst_rubrics(rst)
 
             for role in ('ref', 'doc'):
-                rst = self.replace_cross_refs(rst, role)
+                rst = self.replace_cross_refs(role, rst)
 
             # Use ref_map to generate autodoc substitution definitions
             rst, autodoc_refs = self.replace_autodoc_refs(rst)
             header_vals = self.get_header_vals(autodoc_refs)
 
             # Write the final output
             rst_out = Path(self.config.out_dir, Path(src).name)
@@ -283,14 +355,27 @@
             with open(rst_out, 'w', encoding='utf-8') as f:
                 f.write(
                     "\n".join(header_vals) + "\n\n" + rst)
             print(
                 f'``sphinx_readme``: saved generated .rst file to {rst_out}')
 
     def replace_admonitions(self, rst_src: str, rst: str) -> str:
+        """Replaces generic and specific admonition directives with HTML tables or :rst:dir:`csv-table`
+        directives, depending on the value of :confval:`readme_raw_directive`
+
+        .. admonition:: Customizing Admonitions
+           :class: about
+
+           The :attr:`~.icon_map` can be overriden to use custom admonition icons/classes
+
+           * See :confval:`readme_admonition_icons` and :confval:`readme_default_admonition_icon`
+
+        :param rst_src: absolute path of the source file
+        :param rst: content of the source file
+        """
         admonitions = self.admonitions[rst_src]
 
         for _type in ('generic', 'specific'):
             for admonition in admonitions[_type]:
                 if pattern := self.get_admonition_regex(admonition, _type):
                     icon = self.get_admonition_icon(admonition)
                     if not self.config.raw_directive:
@@ -309,32 +394,35 @@
                                 text=admonition['body'],
                                 icon=icon),
                             string=rst
                         )
         return rst
 
     def replace_toctrees(self, rst_src: str, rst: str) -> str:
-        if self.config.docs_url_type == 'html':
-            base_url = self.config.docs_url
-        else:
-            base_url = self.config.html_baseurl
+        """Replaces :rst:dir:`toctree` directives with hyperlinked bullet lists
+
+        .. note:: Entries will link to HTML documentation regardless of the
+           value of :confval:`readme_docs_url_type`
 
+        :param rst_src: absolute path of the source file
+        :param rst: content of the source file
+        """
         pattern = r".. toctree::\n+?(?:\s+:\w+:\s*?\w*?\n\s+)*?(?:\s+\w+\n)+?(?=\n+\S+?)"
         toctrees = re.findall(pattern, rst)
 
         for toctree, info in zip(toctrees, self.toctrees[rst_src]):
             substitutions = []
             repl = ""
 
             if info['caption']:
                 repl += f"**{info['caption']}**\n\n"
 
             for entry in info['entries']:
                 # Replace each entry with a link to html docs
-                target = f"{base_url}/{entry['entry']}.html"
+                target = f"{self.config.html_baseurl}/{entry['entry']}.html"
 
                 if "`" in entry['title']:
                     # Inline markup in links must be inserted with substitutions
                     sub = entry['title'].replace('`', '')
                     substitutions.extend([
                         f".. |{sub}| replace:: {entry['title']}",
                         f".. _{sub}: {target}"
@@ -352,26 +440,27 @@
             rst = rst.replace(toctree, repl)
 
         return rst
 
     def replace_rst_images(self, rst_src: str, rst: str) -> str:
         """Replaces filepaths in ``image`` directives with repository links
 
-        :Example:
-            :rst:`.. image:: /_static/logo.png`
+        **Example:**
+
+            :rst:`.. image:: /_static/logo_readme.png`
 
             would be replaced with
 
-            :rst:`.. image:: https://github.com/tdkorn/sphinx-readme/blob/main/docs/source/_static/logo.png?raw=True`
+            :rst:`.. image:: https://raw.githubusercontent.com/tdkorn/sphinx-readme/main/docs/source/_static/logo_readme.png`
 
         .. note:: Your repository will be used as the image source regardless of the
            value of :confval:`readme_docs_url_type`
 
-        :param rst_src: absolute path of the rst file being parsed
-        :param rst: the content of the rst file being parsed
+        :param rst_src: absolute path of the source file
+        :param rst: content of the source file
         """
         src_dir = self.config.src_dir
         repo_dir = self.config.repo_dir
         rst_src_dir = Path(rst_src).parent
         relpath_to_src_dir = src_dir.relative_to(repo_dir)
 
         # Find the targets of all image directives
@@ -394,15 +483,39 @@
             rst = re.sub(
                 pattern=rf"\.\. image:: {img_path}",
                 repl=fr".. image:: {self.config.image_baseurl}/{path_to_img}",
                 string=rst
             )
         return rst
 
-    def replace_rst_rubrics(self, rst: str):
+    def replace_rst_rubrics(self, rst: str) -> str:
+        """Replaces :rst:dir:`rubric` directives with the section heading
+        character specified by :confval:`readme_rubric_heading`
+
+        If :confval:`readme_rubric_heading` is not specified, the rubric
+        will be replaced with bold text instead
+
+        ...
+
+        **Example:**
+
+        Consider a source file that contains
+        :rst:`.. rubric:: This is a \`\`rubric\`\` directive`
+
+        * Replacement without specifying ``readme_rubric_heading``::
+
+              **This is a** ``rubric`` **directive**
+
+        * Replacement if :code:`readme_rubric_heading = "^"`::
+
+              This is a ``rubric`` directive
+              ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+        :param rst: content of the source file
+        """
         heading_chars = '!"#$%&\'()*+,-./:;<=>?@[\\]^_`{|}~'
         rubric_pattern = r'\.\. rubric:: (.+?)(?=\n)'
 
         if heading := self.config.rubric_heading:
             if heading in heading_chars:
                 return re.sub(
                     pattern=rubric_pattern,
@@ -411,15 +524,20 @@
                 )
         return re.sub(
             pattern=rubric_pattern,
             repl=lambda m: format_rst("bold", m.group(1)),
             string=rst
         )
 
-    def replace_cross_refs(self, rst: str, ref_role: str) -> str:
+    def replace_cross_refs(self, ref_role: str, rst: str) -> str:
+        """Replaces cross-references using the :rst:role:`doc` or :rst:role:`ref` role
+
+        :param ref_role: the name of the cross-reference role
+        :param rst: content of the source file
+        """
         # Find all :ref_role:`ref_id` cross-refs
         cross_refs = re.findall(
             pattern=fr"(?:\s*?):{ref_role}:`([^`]+)`(?=\s*?)",
             string=rst
         )
         # Match these ids up with target data in the ref_map
         cross_ref_map = dict(zip(cross_refs, self.ref_map[ref_role]))
@@ -430,17 +548,25 @@
                 pattern=rf":{ref_role}:`{ref_id}`",
                 repl=rf"`{target['text']} <{target['refuri']}>`_",
                 string=rst
             )
         return rst
 
     def replace_autodoc_refs(self, rst: str) -> Tuple[str, Set]:
-        """
-        :param rst:
-        :return:
+        """Replace :mod:`~sphinx.ext.autodoc` cross-references with substitutions
+
+        These substitutions will be hyperlinked to the corresponding source code
+        or HTML documentation entry, depending on the value of
+        :confval:`readme_docs_url_type`
+
+        .. note: Attributes will only be hyperlinked
+           if linking to HTML documentation
+
+        :param rst: content of the source file
+        :returns: subbed rst and all autodoc xref targets found within it
         """
         # :role:`{~.}{module|class}{.}target` where {} is optional
         pattern = r":(?:mod|class|meth|func):`([~\.\w]+)`"
 
         if self.config.replace_attrs:
             if self.config.docs_url_type == 'html':
                 # If linking to HTML docs, we can generate cross-refs for attributes
@@ -452,42 +578,55 @@
         # To render on GitHub/PyPi/etc., we use Sphinx substitutions instead of cross-refs
         # Syntax is |.{ref}|_ or |.`{ref}`|_
         if self.config.inline_markup:
             repl = r"|.`\1`|_"
         else:
             repl = r"|.\1|_"
 
-        # Get a list of all autodoc cross-refs
+        # Get a set of all autodoc cross-refs
         autodoc_refs = set(re.findall(pattern, rst))
 
         # Replace cross-refs with substitutions
         rst = re.sub(pattern, repl, rst)
 
         # Use autodoc_refs and ref_map to generate substitution definitions
         return rst, autodoc_refs
 
     def replace_autodoc_attrs(self, rst: str) -> str:
+        """Replaces ``:attr:`` cross-references with ``inline literals``
+
+        .. hint::
+
+           This method is only called if both
+
+           1. :confval:`readme_docs_url_type` is ``"code"``
+           2. :confval:`readme_replace_attrs` is ``True``
+        """
         # Ex. ~.Class.meth => ``meth``
         short_ref = r" :attr:`~\.?(\w+)`"
         # Ex. .Class.meth => ``Class.meth``
         long_ref = r" :attr:`\.?([\.\w]+)`"
         repl = r" ``\1``"
 
         rst = re.sub(short_ref, repl, rst)
         rst = re.sub(long_ref, repl, rst)
         return rst
 
     def get_header_vals(self, autodoc_refs: Set) -> List[str]:
+        """Returns a list of substitution definitions and hyperlink references to prepend to the file
+
+        :param autodoc_refs: :mod:`sphinx.ext.autodoc` targets to define substitutions for
+        """
         header = []
 
         for ref in autodoc_refs:
-            info = self.ref_map[ref]
+            info = self.ref_map.get(ref)
 
-            # Check for empty REFERENCE_MAPPING
-            if not any(info.values()):
+            # Check for invalid ref
+            if info is None:
                 continue
 
             if self.config.inline_markup:
                 ref = f"`{ref}`"
 
             header.extend([
                 f".. |.{ref}| replace:: {info['replace']}",
@@ -496,15 +635,20 @@
 
         if not self.config.raw_directive:
             for _type, icon in self.config.icon_map.items():
                 header.append(f'.. |{_type}| replace:: {icon}')
 
         return header
 
-    def get_admonition_regex(self, admonition, admonition_type):
+    def get_admonition_regex(self, admonition: Dict[str, str], admonition_type: str) -> str:
+        """Returns the regex to match a specific admonition directive
+
+        :param admonition: a dict containing admonition data
+        :param admonition_type: ``"generic"`` or ``"specific"``
+        """
         body = escape_rst(admonition['body'])
         title = escape_rst(admonition['title'])
 
         # Account for arbitrary whitespace before each line of directive content
         lines = (line.replace('\n', '\n\s+') for line in body.split('\n\n'))
         body = '\n\n\s+'.join(lines)
 
@@ -529,14 +673,18 @@
             # raw html template body uses string formatting
             pattern += rf"{body}"
 
         pattern += r"(?=[\n\S]+?)"
         return pattern
 
     def get_admonition_icon(self, admonition: dict):
+        """Returns the icon to use for an admonition
+
+        :param admonition: a dict of admonition data
+        """
         icon = self.config.icon_map.get(admonition['class'])
 
         # Raw directive allows for using icon directly
         if self.config.raw_directive:
             return icon if icon else self.config.default_admonition_icon
 
         if icon:  # Without raw directive, must use substitution
```

### Comparing `sphinx-readme-0.0.1b6/sphinx_readme.egg-info/PKG-INFO` & `sphinx-readme-0.0.2/sphinx_readme.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-readme
-Version: 0.0.1b6
+Version: 0.0.2
 Summary: Generate Beautiful reStructuredText README.rst for GitHub, PyPi, GitLab, BitBucket
 Home-page: https://github.com/tdkorn/sphinx-readme
 Author: Adam Korn
 Author-email: hello@dailykitten.net
 License: MIT License
 Download-URL: https://github.com/TDKorn/sphinx-readme/tarball/main
 Keywords: sphinx,docutils,sphinx-extension,sphinx-contrib,reStructuredText,rst,reST,parser,rst-parser,README.rst,README,autodoc,linkcode
@@ -14,20 +14,20 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/x-rst; charset=UTF-8
 License-File: LICENSE
 
 .. |.`~.sphinx.ext.autodoc`| replace:: ``autodoc``
 .. _.`~.sphinx.ext.autodoc`: https://www.sphinx-doc.org/en/master/usage/extensions/autodoc.html#module-sphinx.ext.autodoc
-.. |.`sphinx.ext.autodoc`| replace:: ``sphinx.ext.autodoc``
-.. _.`sphinx.ext.autodoc`: https://www.sphinx-doc.org/en/master/usage/extensions/autodoc.html#module-sphinx.ext.autodoc
 .. |.`sphinx.ext.linkcode`| replace:: ``sphinx.ext.linkcode``
 .. _.`sphinx.ext.linkcode`: https://www.sphinx-doc.org/en/master/usage/extensions/linkcode.html#module-sphinx.ext.linkcode
 .. |.`~.parse_intersphinx_node`| replace:: ``parse_intersphinx_node()``
-.. _.`~.parse_intersphinx_node`: https://github.com/TDKorn/sphinx-readme/blob/v0.0.1b6/sphinx_readme/parser.py#L124-L134
+.. _.`~.parse_intersphinx_node`: https://github.com/TDKorn/sphinx-readme/blob/v0.0.2/sphinx_readme/parser.py#L145-L159
+.. |.`sphinx.ext.autodoc`| replace:: ``sphinx.ext.autodoc``
+.. _.`sphinx.ext.autodoc`: https://www.sphinx-doc.org/en/master/usage/extensions/autodoc.html#module-sphinx.ext.autodoc
 .. |attention| replace:: 🔔️
 .. |caution| replace:: ⚠️
 .. |danger| replace:: ☢️
 .. |error| replace:: ⛔
 .. |hint| replace:: 🧠
 .. |important| replace:: 📢
 .. |note| replace:: 📝
@@ -37,31 +37,31 @@
 .. |about| replace:: 📚
 
 .. meta::
    :author: Adam Korn
    :title: Sphinx README
    :description: Sphinx Extension to Generate Beautiful reStructuredText README.rst for GitHub, PyPi, GitLab, BitBucket
 
-
 Sphinx README - Generate Beautiful ``README.rst`` for GitHub, PyPi, GitLab, BitBucket
 --------------------------------------------------------------------------------------
 
-.. image:: https://raw.githubusercontent.com/TDKorn/sphinx-readme/v0.0.1b6/docs/source/_static/logo_readme.png
+.. image:: https://raw.githubusercontent.com/TDKorn/sphinx-readme/v0.0.2/docs/source/_static/logo_transparent.png
    :alt: Sphinx README: Generate Beautiful reStructuredText README.rst for GitHub, PyPi, GitLab, BitBucket
    :align: center
    :width: 25%
 
-
 A Sphinx extension to generate ``README.rst`` files that render beautifully on GitHub, PyPi, GitLab, BitBucket
 
+
 .. |RTD| replace:: **Explore the docs »**
 .. _RTD: https://sphinx-readme.readthedocs.io/en/latest/
 
 |RTD|_
 
+|
 
 .. image:: https://img.shields.io/pypi/v/sphinx-readme?color=eb5202
    :target: https://pypi.org/project/sphinx-readme
    :alt: PyPI Project for Sphinx README: Generate Beautiful reStructuredText README.rst for GitHub, PyPi, GitLab, BitBucket
 
 .. image:: https://img.shields.io/badge/GitHub-sphinx--readme-4f1abc
    :target: https://github.com/tdkorn/sphinx-readme
@@ -71,15 +71,14 @@
    :target: https://pepy.tech/project/sphinx-readme
    :alt: Downloads for Sphinx README
 
 .. image:: https://readthedocs.org/projects/sphinx-readme/badge/?version=latest
    :target: https://sphinx-readme.readthedocs.io/en/latest/?badge=latest
    :alt: Documentation for Sphinx README: Generate Beautiful reStructuredText README.rst for GitHub, PyPi, GitLab, BitBucket
 
-
 |
 
 About Sphinx README
 ~~~~~~~~~~~~~~~~~~~~~~~
 
 
 .. csv-table::
@@ -87,22 +86,22 @@
 
    "``sphinx_readme`` is a ``reStructuredText`` parser that uses Sphinx
    to generate ``rst`` files that render beautifully on
    GitHub, PyPi, GitLab, and BitBucket."
 
 
 
-With ``sphinx_readme``, there's no need to rewrite your ``README.rst`` as a ``README.md`` file
-==============================================================================================
+**With** ``sphinx_readme`` **, there's no need to rewrite your** ``README.rst`` **as a** ``README.md`` **file**
 
 Files generated by ``sphinx_readme`` have nearly identical appearance and functionality
 as ``html`` builds, including |.`sphinx.ext.autodoc`|_ cross-references!
 
+|
 
-.. image:: https://raw.githubusercontent.com/TDKorn/sphinx-readme/v0.0.1b6/docs/source/_static/demo/demo.gif
+.. image:: https://raw.githubusercontent.com/TDKorn/sphinx-readme/v0.0.2/docs/source/_static/demo/demo.gif
    :alt: Demonstration of how reStructuredText README.rst files generated by Sphinx README render on GitHub, PyPi, GitLab, BitBucket
    :width: 75%
 
 
 Features
 ~~~~~~~~~~
 
@@ -156,25 +155,25 @@
  * At minimum, the username and repository name must be specified
  * Please see `HTML Context Settings <https://docs.readthedocs.io/en/stable/guides/edit-source-links-sphinx.html>`_
    to determine the correct dictionary keys for your hosting platform
 
 .. |html_context| replace:: ``html_context``
 .. _html_context: https://www.sphinx-doc.org/en/master/usage/configuration.html#confval-html_context
 
-...
+|
 
 |html_baseurl|_
  The base URL which points to the root of the HTML documentation
 
   Type: ``str``
 
 .. |html_baseurl| replace:: ``html_baseurl``
 .. _html_baseurl: https://www.sphinx-doc.org/en/master/usage/configuration.html#confval-html_baseurl
 
-...
+|
 
 |readme_src_files|_
  An individual or list of ``rst`` files to parse
 
   Type: ``Union[str, List]``
 
 
@@ -183,15 +182,15 @@
 
    "Filepaths should be specified relative to the source directory"
 
 
 .. |readme_src_files| replace:: ``readme_src_files``
 .. _readme_src_files: https://sphinx-readme.readthedocs.io/en/latest/configuration/configuring.html#confval-readme_src_files
 
-...
+|
 
 |readme_docs_url_type|_
  The documentation source to link to when resolving |.`~.sphinx.ext.autodoc`|_ cross-references
 
   Type: ``str``
 
  Must be either ``"code"`` or ``"html"``
@@ -251,16 +250,16 @@
 .. _readme_raw_directive: https://sphinx-readme.readthedocs.io/en/latest/configuration/configuring.html#confval-readme_raw_directive
 
 
 
 .. csv-table::
    :header: |important| Important
 
-   "If generating a ``README`` for a platform that doesn't support ``raw``
-   directives (PyPi, GitLab, and BitBucket), be sure to disable |readme_raw_directive|_:
+   "For platforms that don't support the ``raw`` directive (PyPi, GitLab, and BitBucket),
+   be sure to disable |readme_raw_directive|_:
 
    .. code-block:: python
 
       readme_raw_directive = False"
```

