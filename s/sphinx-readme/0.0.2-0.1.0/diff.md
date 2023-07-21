# Comparing `tmp/sphinx-readme-0.0.2.tar.gz` & `tmp/sphinx-readme-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx-readme-0.0.2.tar", last modified: Fri Jul 21 06:50:31 2023, max compression
+gzip compressed data, was "sphinx-readme-0.1.0.tar", last modified: Fri Jul 21 07:31:33 2023, max compression
```

## Comparing `sphinx-readme-0.0.2.tar` & `sphinx-readme-0.1.0.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-21 06:50:31.481447 sphinx-readme-0.0.2/
--rw-rw-rw-   0        0        0     1084 2023-05-09 12:07:43.000000 sphinx-readme-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     9259 2023-07-21 06:50:31.481447 sphinx-readme-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     8470 2023-07-21 06:49:17.000000 sphinx-readme-0.0.2/README.rst
--rw-rw-rw-   0        0        0       42 2023-07-21 06:50:31.481447 sphinx-readme-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1454 2023-07-18 11:51:26.000000 sphinx-readme-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-21 06:50:31.450206 sphinx-readme-0.0.2/sphinx_readme/
--rw-rw-rw-   0        0        0     1722 2023-07-21 06:42:57.000000 sphinx-readme-0.0.2/sphinx_readme/__init__.py
--rw-rw-rw-   0        0        0    11766 2023-07-21 06:42:57.000000 sphinx-readme-0.0.2/sphinx_readme/config.py
--rw-rw-rw-   0        0        0    27686 2023-07-21 06:42:57.000000 sphinx-readme-0.0.2/sphinx_readme/parser.py
-drwxrwxrwx   0        0        0        0 2023-07-21 06:50:31.481447 sphinx-readme-0.0.2/sphinx_readme/utils/
--rw-rw-rw-   0        0        0        0 2023-07-21 06:42:57.000000 sphinx-readme-0.0.2/sphinx_readme/utils/__init__.py
--rw-rw-rw-   0        0        0     4643 2023-07-21 06:42:57.000000 sphinx-readme-0.0.2/sphinx_readme/utils/git.py
--rw-rw-rw-   0        0        0     3727 2023-07-21 06:42:57.000000 sphinx-readme-0.0.2/sphinx_readme/utils/linkcode.py
--rw-rw-rw-   0        0        0     4252 2023-07-21 06:42:57.000000 sphinx-readme-0.0.2/sphinx_readme/utils/rst.py
--rw-rw-rw-   0        0        0      810 2023-07-21 06:42:57.000000 sphinx-readme-0.0.2/sphinx_readme/utils/sphinx.py
-drwxrwxrwx   0        0        0        0 2023-07-21 06:50:31.465826 sphinx-readme-0.0.2/sphinx_readme.egg-info/
--rw-rw-rw-   0        0        0     9259 2023-07-21 06:50:31.000000 sphinx-readme-0.0.2/sphinx_readme.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      433 2023-07-21 06:50:31.000000 sphinx-readme-0.0.2/sphinx_readme.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 06:50:31.000000 sphinx-readme-0.0.2/sphinx_readme.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-07-21 06:50:31.000000 sphinx-readme-0.0.2/sphinx_readme.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-21 06:50:31.000000 sphinx-readme-0.0.2/sphinx_readme.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-21 07:31:33.748779 sphinx-readme-0.1.0/
+-rw-rw-rw-   0        0        0     1084 2023-05-09 12:07:43.000000 sphinx-readme-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0     9734 2023-07-21 07:31:33.733156 sphinx-readme-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     8945 2023-07-21 07:31:07.000000 sphinx-readme-0.1.0/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-21 07:31:33.748779 sphinx-readme-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1454 2023-07-18 11:51:26.000000 sphinx-readme-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 07:31:33.696196 sphinx-readme-0.1.0/sphinx_readme/
+-rw-rw-rw-   0        0        0     1703 2023-07-21 07:28:05.000000 sphinx-readme-0.1.0/sphinx_readme/__init__.py
+-rw-rw-rw-   0        0        0    11533 2023-07-21 07:23:43.000000 sphinx-readme-0.1.0/sphinx_readme/config.py
+-rw-rw-rw-   0        0        0    24336 2023-07-21 07:23:43.000000 sphinx-readme-0.1.0/sphinx_readme/parser.py
+drwxrwxrwx   0        0        0        0 2023-07-21 07:31:33.733156 sphinx-readme-0.1.0/sphinx_readme/utils/
+-rw-rw-rw-   0        0        0        0 2023-07-21 06:42:57.000000 sphinx-readme-0.1.0/sphinx_readme/utils/__init__.py
+-rw-rw-rw-   0        0        0      603 2023-07-21 07:23:43.000000 sphinx-readme-0.1.0/sphinx_readme/utils/docutils.py
+-rw-rw-rw-   0        0        0     4643 2023-07-21 06:42:57.000000 sphinx-readme-0.1.0/sphinx_readme/utils/git.py
+-rw-rw-rw-   0        0        0     3727 2023-07-21 06:42:57.000000 sphinx-readme-0.1.0/sphinx_readme/utils/linkcode.py
+-rw-rw-rw-   0        0        0     6453 2023-07-21 07:23:43.000000 sphinx-readme-0.1.0/sphinx_readme/utils/rst.py
+-rw-rw-rw-   0        0        0      810 2023-07-21 06:42:57.000000 sphinx-readme-0.1.0/sphinx_readme/utils/sphinx.py
+drwxrwxrwx   0        0        0        0 2023-07-21 07:31:33.732097 sphinx-readme-0.1.0/sphinx_readme.egg-info/
+-rw-rw-rw-   0        0        0     9734 2023-07-21 07:31:33.000000 sphinx-readme-0.1.0/sphinx_readme.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      465 2023-07-21 07:31:33.000000 sphinx-readme-0.1.0/sphinx_readme.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 07:31:33.000000 sphinx-readme-0.1.0/sphinx_readme.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-07-21 07:31:33.000000 sphinx-readme-0.1.0/sphinx_readme.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-21 07:31:33.000000 sphinx-readme-0.1.0/sphinx_readme.egg-info/top_level.txt
```

### Comparing `sphinx-readme-0.0.2/LICENSE` & `sphinx-readme-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinx-readme-0.0.2/PKG-INFO` & `sphinx-readme-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-readme
-Version: 0.0.2
+Version: 0.1.0
 Summary: Generate Beautiful reStructuredText README.rst for GitHub, PyPi, GitLab, BitBucket
 Home-page: https://github.com/tdkorn/sphinx-readme
 Author: Adam Korn
 Author-email: hello@dailykitten.net
 License: MIT License
 Download-URL: https://github.com/TDKorn/sphinx-readme/tarball/main
 Keywords: sphinx,docutils,sphinx-extension,sphinx-contrib,reStructuredText,rst,reST,parser,rst-parser,README.rst,README,autodoc,linkcode
@@ -12,43 +12,58 @@
 Classifier: Framework :: Sphinx :: Extension
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/x-rst; charset=UTF-8
 License-File: LICENSE
 
-.. |.`~.sphinx.ext.autodoc`| replace:: ``autodoc``
-.. _.`~.sphinx.ext.autodoc`: https://www.sphinx-doc.org/en/master/usage/extensions/autodoc.html#module-sphinx.ext.autodoc
+.. |.`~.parse_intersphinx_nodes`| replace:: ``parse_intersphinx_nodes()``
+.. _.`~.parse_intersphinx_nodes`: https://github.com/TDKorn/sphinx-readme/blob/v0.1.0/sphinx_readme/parser.py#L208-L232
 .. |.`sphinx.ext.linkcode`| replace:: ``sphinx.ext.linkcode``
 .. _.`sphinx.ext.linkcode`: https://www.sphinx-doc.org/en/master/usage/extensions/linkcode.html#module-sphinx.ext.linkcode
-.. |.`~.parse_intersphinx_node`| replace:: ``parse_intersphinx_node()``
-.. _.`~.parse_intersphinx_node`: https://github.com/TDKorn/sphinx-readme/blob/v0.0.2/sphinx_readme/parser.py#L145-L159
+.. |.`~.sphinx.ext.autodoc`| replace:: ``autodoc``
+.. _.`~.sphinx.ext.autodoc`: https://www.sphinx-doc.org/en/master/usage/extensions/autodoc.html#module-sphinx.ext.autodoc
 .. |.`sphinx.ext.autodoc`| replace:: ``sphinx.ext.autodoc``
 .. _.`sphinx.ext.autodoc`: https://www.sphinx-doc.org/en/master/usage/extensions/autodoc.html#module-sphinx.ext.autodoc
 .. |attention| replace:: 🔔️
 .. |caution| replace:: ⚠️
 .. |danger| replace:: ☢️
 .. |error| replace:: ⛔
 .. |hint| replace:: 🧠
 .. |important| replace:: 📢
 .. |note| replace:: 📝
 .. |tip| replace:: 💡
 .. |warning| replace:: 🚩
 .. |default| replace:: 📄
 .. |about| replace:: 📚
 
+.. |html_context| replace:: ``html_context``
+.. _html_context: https://sphinx-readme.readthedocs.io/en/latest/configuration/configuring.html#confval-html_context
+.. |html_baseurl| replace:: ``html_baseurl``
+.. _html_baseurl: https://sphinx-readme.readthedocs.io/en/latest/configuration/configuring.html#confval-html_baseurl
+.. |readme_src_files| replace:: ``readme_src_files``
+.. _readme_src_files: https://sphinx-readme.readthedocs.io/en/latest/configuration/configuring.html#confval-readme_src_files
+.. |readme_docs_url_type| replace:: ``readme_docs_url_type``
+.. _readme_docs_url_type: https://sphinx-readme.readthedocs.io/en/latest/configuration/configuring.html#confval-readme_docs_url_type
+.. |readme_replace_attrs| replace:: ``readme_replace_attrs``
+.. _readme_replace_attrs: https://sphinx-readme.readthedocs.io/en/latest/configuration/configuring.html#confval-readme_replace_attrs
+.. |readme_inline_markup| replace:: ``readme_inline_markup``
+.. _readme_inline_markup: https://sphinx-readme.readthedocs.io/en/latest/configuration/configuring.html#confval-readme_inline_markup
+.. |readme_raw_directive| replace:: ``readme_raw_directive``
+.. _readme_raw_directive: https://sphinx-readme.readthedocs.io/en/latest/configuration/configuring.html#confval-readme_raw_directive
+
 .. meta::
    :author: Adam Korn
    :title: Sphinx README
    :description: Sphinx Extension to Generate Beautiful reStructuredText README.rst for GitHub, PyPi, GitLab, BitBucket
 
 Sphinx README - Generate Beautiful ``README.rst`` for GitHub, PyPi, GitLab, BitBucket
 --------------------------------------------------------------------------------------
 
-.. image:: https://raw.githubusercontent.com/TDKorn/sphinx-readme/v0.0.2/docs/source/_static/logo_transparent.png
+.. image:: https://raw.githubusercontent.com/TDKorn/sphinx-readme/v0.1.0/docs/source/_static/logo_transparent.png
    :alt: Sphinx README: Generate Beautiful reStructuredText README.rst for GitHub, PyPi, GitLab, BitBucket
    :align: center
    :width: 25%
 
 A Sphinx extension to generate ``README.rst`` files that render beautifully on GitHub, PyPi, GitLab, BitBucket
 
 
@@ -93,35 +108,35 @@
 **With** ``sphinx_readme`` **, there's no need to rewrite your** ``README.rst`` **as a** ``README.md`` **file**
 
 Files generated by ``sphinx_readme`` have nearly identical appearance and functionality
 as ``html`` builds, including |.`sphinx.ext.autodoc`|_ cross-references!
 
 |
 
-.. image:: https://raw.githubusercontent.com/TDKorn/sphinx-readme/v0.0.2/docs/source/_static/demo/demo.gif
+.. image:: https://raw.githubusercontent.com/TDKorn/sphinx-readme/v0.1.0/docs/source/_static/demo/demo.gif
    :alt: Demonstration of how reStructuredText README.rst files generated by Sphinx README render on GitHub, PyPi, GitLab, BitBucket
    :width: 75%
 
 
-Features
-~~~~~~~~~~
+📋 Features
+~~~~~~~~~~~~
 
 ``sphinx_readme`` adds support for the following ``sphinx`` and ``docutils`` directives and features:
 
 * |.`sphinx.ext.autodoc`|_ cross-references (``:mod:``, ``:class:``, ``:meth:``, ``:func:``, and ``:attr:``)
 * Standard cross-reference roles (``:doc:`` and ``:ref:``)
 * Generic and Specific Admonitions
 * Only directives
 * Toctrees
 * Rubrics
 * Images
 
 
-Installation
-~~~~~~~~~~~~~
+⚙ Installation
+~~~~~~~~~~~~~~~~
 
 Install using pip::
 
    pip install sphinx-readme
 
 
 Add the extension to your ``conf.py``:
@@ -130,48 +145,49 @@
 
    extensions = [
       'sphinx_readme',
    ]
 
 
 
-Configuration
-~~~~~~~~~~~~~~~
+🔧 Configuration
+~~~~~~~~~~~~~~~~~
 
+.. |linkcode| replace:: |.`sphinx.ext.linkcode`|_
 
 
 
 
 Please see `Extension Configuration <https://sphinx-readme.readthedocs.io/en/latest/configuration/configuring.html>`_ for full documentation on configuration variables
 
 
 Mandatory ``conf.py`` Values
 ==================================
 
 |html_context|_
- A dictionary containing info about your repository
+ A dictionary containing info about your repository (|sphinx_html_context|_)
 
   Type: ``dict``
 
  * At minimum, the username and repository name must be specified
  * Please see `HTML Context Settings <https://docs.readthedocs.io/en/stable/guides/edit-source-links-sphinx.html>`_
    to determine the correct dictionary keys for your hosting platform
 
-.. |html_context| replace:: ``html_context``
-.. _html_context: https://www.sphinx-doc.org/en/master/usage/configuration.html#confval-html_context
+.. |sphinx_html_context| replace:: ``html_context``
+.. _sphinx_html_context: https://www.sphinx-doc.org/en/master/usage/configuration.html#confval-html_context
 
 |
 
 |html_baseurl|_
- The base URL which points to the root of the HTML documentation
+ The base URL which points to the root of the HTML documentation (|sphinx_html_baseurl|_)
 
   Type: ``str``
 
-.. |html_baseurl| replace:: ``html_baseurl``
-.. _html_baseurl: https://www.sphinx-doc.org/en/master/usage/configuration.html#confval-html_baseurl
+.. |sphinx_html_baseurl| replace:: ``html_baseurl``
+.. _sphinx_html_baseurl: https://www.sphinx-doc.org/en/master/usage/configuration.html#confval-html_baseurl
 
 |
 
 |readme_src_files|_
  An individual or list of ``rst`` files to parse
 
   Type: ``Union[str, List]``
@@ -179,53 +195,45 @@
 
 .. csv-table::
    :header: |important| Important
 
    "Filepaths should be specified relative to the source directory"
 
 
-.. |readme_src_files| replace:: ``readme_src_files``
-.. _readme_src_files: https://sphinx-readme.readthedocs.io/en/latest/configuration/configuring.html#confval-readme_src_files
-
 |
 
 |readme_docs_url_type|_
  The documentation source to link to when resolving |.`~.sphinx.ext.autodoc`|_ cross-references
 
   Type: ``str``
 
  Must be either ``"code"`` or ``"html"``
 
- * ``"code"``: uses |.`sphinx.ext.linkcode`|_ to replace references with links to highlighted source code
+ * ``"code"``: uses |linkcode| to replace references with links to highlighted source code
 
-   **Example**: |.`~.parse_intersphinx_node`|_
+   **Example**: |.`~.parse_intersphinx_nodes`|_
 
 
  * ``"html"``: replaces references with links to HTML documentation entries
 
-   **Example**: |parse_intersphinx_node_html|_
+   **Example**: |parse_intersphinx_nodes_html|_
 
 
 .. csv-table::
    :header: |note| Note
 
    "If set to ``code``, then :code:`:attr:` cross-references will not be replaced with links
 
    * Instead, they'll be replaced with ``inline literals`` or left as is
    * Please see |readme_replace_attrs|_ and |readme_inline_markup|_"
 
 
-.. |readme_docs_url_type| replace:: ``readme_docs_url_type``
-.. _readme_docs_url_type: https://sphinx-readme.readthedocs.io/en/latest/configuration/configuring.html#confval-readme_docs_url_type
-.. |parse_intersphinx_node_html| replace:: ``parse_intersphinx_node()``
-.. _parse_intersphinx_node_html: http://sphinx-readme.readthedocs.io/en/latest/parser.html#sphinx_readme.parser.READMEParser.parse_intersphinx_node
-.. |readme_replace_attrs| replace:: ``readme_replace_attrs``
-.. _readme_replace_attrs: https://sphinx-readme.readthedocs.io/en/latest/configuration/configuring.html#confval-readme_replace_attrs
-.. |readme_inline_markup| replace:: ``readme_inline_markup``
-.. _readme_inline_markup: https://sphinx-readme.readthedocs.io/en/latest/configuration/configuring.html#confval-readme_inline_markup
+
+.. |parse_intersphinx_nodes_html| replace:: ``parse_intersphinx_nodes()``
+.. _parse_intersphinx_nodes_html: http://sphinx-readme.readthedocs.io/en/latest/parser.html#sphinx_readme.parser.READMEParser.parse_intersphinx_nodes
 
 
 Sample ``conf.py``
 ~~~~~~~~~~~~~~~~~~~
 
 .. code-block:: python
 
@@ -242,17 +250,14 @@
    html_baseurl = "https://sphinx-readme.readthedocs.io/en/latest"
 
    readme_src_files = "README.rst"
 
    readme_docs_url_type = "code"
 
 
-.. |readme_raw_directive| replace:: ``readme_raw_directive``
-.. _readme_raw_directive: https://sphinx-readme.readthedocs.io/en/latest/configuration/configuring.html#confval-readme_raw_directive
-
 
 
 .. csv-table::
    :header: |important| Important
 
    "For platforms that don't support the ``raw`` directive (PyPi, GitLab, and BitBucket),
    be sure to disable |readme_raw_directive|_:
@@ -260,16 +265,15 @@
    .. code-block:: python
 
       readme_raw_directive = False"
 
 
 
 
-
-Documentation
+📚 Documentation
 ~~~~~~~~~~~~~~~~
 
 Full documentation can be found on |docs|_
 
 
 .. |docs| replace:: ``ReadTheDocs``
 .. _docs: https://sphinx-readme.readthedocs.io/en/latest
```

### Comparing `sphinx-readme-0.0.2/README.rst` & `sphinx-readme-0.1.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,51 @@
-.. |.`~.sphinx.ext.autodoc`| replace:: ``autodoc``
-.. _.`~.sphinx.ext.autodoc`: https://www.sphinx-doc.org/en/master/usage/extensions/autodoc.html#module-sphinx.ext.autodoc
+.. |.`~.parse_intersphinx_nodes`| replace:: ``parse_intersphinx_nodes()``
+.. _.`~.parse_intersphinx_nodes`: https://github.com/TDKorn/sphinx-readme/blob/v0.1.0/sphinx_readme/parser.py#L208-L232
 .. |.`sphinx.ext.linkcode`| replace:: ``sphinx.ext.linkcode``
 .. _.`sphinx.ext.linkcode`: https://www.sphinx-doc.org/en/master/usage/extensions/linkcode.html#module-sphinx.ext.linkcode
-.. |.`~.parse_intersphinx_node`| replace:: ``parse_intersphinx_node()``
-.. _.`~.parse_intersphinx_node`: https://github.com/TDKorn/sphinx-readme/blob/v0.0.2/sphinx_readme/parser.py#L145-L159
+.. |.`~.sphinx.ext.autodoc`| replace:: ``autodoc``
+.. _.`~.sphinx.ext.autodoc`: https://www.sphinx-doc.org/en/master/usage/extensions/autodoc.html#module-sphinx.ext.autodoc
 .. |.`sphinx.ext.autodoc`| replace:: ``sphinx.ext.autodoc``
 .. _.`sphinx.ext.autodoc`: https://www.sphinx-doc.org/en/master/usage/extensions/autodoc.html#module-sphinx.ext.autodoc
 .. |attention| replace:: 🔔️
 .. |caution| replace:: ⚠️
 .. |danger| replace:: ☢️
 .. |error| replace:: ⛔
 .. |hint| replace:: 🧠
 .. |important| replace:: 📢
 .. |note| replace:: 📝
 .. |tip| replace:: 💡
 .. |warning| replace:: 🚩
 .. |default| replace:: 📄
 .. |about| replace:: 📚
 
+.. |html_context| replace:: ``html_context``
+.. _html_context: https://sphinx-readme.readthedocs.io/en/latest/configuration/configuring.html#confval-html_context
+.. |html_baseurl| replace:: ``html_baseurl``
+.. _html_baseurl: https://sphinx-readme.readthedocs.io/en/latest/configuration/configuring.html#confval-html_baseurl
+.. |readme_src_files| replace:: ``readme_src_files``
+.. _readme_src_files: https://sphinx-readme.readthedocs.io/en/latest/configuration/configuring.html#confval-readme_src_files
+.. |readme_docs_url_type| replace:: ``readme_docs_url_type``
+.. _readme_docs_url_type: https://sphinx-readme.readthedocs.io/en/latest/configuration/configuring.html#confval-readme_docs_url_type
+.. |readme_replace_attrs| replace:: ``readme_replace_attrs``
+.. _readme_replace_attrs: https://sphinx-readme.readthedocs.io/en/latest/configuration/configuring.html#confval-readme_replace_attrs
+.. |readme_inline_markup| replace:: ``readme_inline_markup``
+.. _readme_inline_markup: https://sphinx-readme.readthedocs.io/en/latest/configuration/configuring.html#confval-readme_inline_markup
+.. |readme_raw_directive| replace:: ``readme_raw_directive``
+.. _readme_raw_directive: https://sphinx-readme.readthedocs.io/en/latest/configuration/configuring.html#confval-readme_raw_directive
+
 .. meta::
    :author: Adam Korn
    :title: Sphinx README
    :description: Sphinx Extension to Generate Beautiful reStructuredText README.rst for GitHub, PyPi, GitLab, BitBucket
 
 Sphinx README - Generate Beautiful ``README.rst`` for GitHub, PyPi, GitLab, BitBucket
 --------------------------------------------------------------------------------------
 
-.. image:: https://raw.githubusercontent.com/TDKorn/sphinx-readme/v0.0.2/docs/source/_static/logo_transparent.png
+.. image:: https://raw.githubusercontent.com/TDKorn/sphinx-readme/v0.1.0/docs/source/_static/logo_transparent.png
    :alt: Sphinx README: Generate Beautiful reStructuredText README.rst for GitHub, PyPi, GitLab, BitBucket
    :align: center
    :width: 25%
 
 A Sphinx extension to generate ``README.rst`` files that render beautifully on GitHub, PyPi, GitLab, BitBucket
 
 
@@ -75,35 +90,35 @@
 **With** ``sphinx_readme`` **, there's no need to rewrite your** ``README.rst`` **as a** ``README.md`` **file**
 
 Files generated by ``sphinx_readme`` have nearly identical appearance and functionality
 as ``html`` builds, including |.`sphinx.ext.autodoc`|_ cross-references!
 
 |
 
-.. image:: https://raw.githubusercontent.com/TDKorn/sphinx-readme/v0.0.2/docs/source/_static/demo/demo.gif
+.. image:: https://raw.githubusercontent.com/TDKorn/sphinx-readme/v0.1.0/docs/source/_static/demo/demo.gif
    :alt: Demonstration of how reStructuredText README.rst files generated by Sphinx README render on GitHub, PyPi, GitLab, BitBucket
    :width: 75%
 
 
-Features
-~~~~~~~~~~
+📋 Features
+~~~~~~~~~~~~
 
 ``sphinx_readme`` adds support for the following ``sphinx`` and ``docutils`` directives and features:
 
 * |.`sphinx.ext.autodoc`|_ cross-references (``:mod:``, ``:class:``, ``:meth:``, ``:func:``, and ``:attr:``)
 * Standard cross-reference roles (``:doc:`` and ``:ref:``)
 * Generic and Specific Admonitions
 * Only directives
 * Toctrees
 * Rubrics
 * Images
 
 
-Installation
-~~~~~~~~~~~~~
+⚙ Installation
+~~~~~~~~~~~~~~~~
 
 Install using pip::
 
    pip install sphinx-readme
 
 
 Add the extension to your ``conf.py``:
@@ -112,48 +127,49 @@
 
    extensions = [
       'sphinx_readme',
    ]
 
 
 
-Configuration
-~~~~~~~~~~~~~~~
+🔧 Configuration
+~~~~~~~~~~~~~~~~~
 
+.. |linkcode| replace:: |.`sphinx.ext.linkcode`|_
 
 
 
 
 Please see `Extension Configuration <https://sphinx-readme.readthedocs.io/en/latest/configuration/configuring.html>`_ for full documentation on configuration variables
 
 
 Mandatory ``conf.py`` Values
 ==================================
 
 |html_context|_
- A dictionary containing info about your repository
+ A dictionary containing info about your repository (|sphinx_html_context|_)
 
   Type: ``dict``
 
  * At minimum, the username and repository name must be specified
  * Please see `HTML Context Settings <https://docs.readthedocs.io/en/stable/guides/edit-source-links-sphinx.html>`_
    to determine the correct dictionary keys for your hosting platform
 
-.. |html_context| replace:: ``html_context``
-.. _html_context: https://www.sphinx-doc.org/en/master/usage/configuration.html#confval-html_context
+.. |sphinx_html_context| replace:: ``html_context``
+.. _sphinx_html_context: https://www.sphinx-doc.org/en/master/usage/configuration.html#confval-html_context
 
 |
 
 |html_baseurl|_
- The base URL which points to the root of the HTML documentation
+ The base URL which points to the root of the HTML documentation (|sphinx_html_baseurl|_)
 
   Type: ``str``
 
-.. |html_baseurl| replace:: ``html_baseurl``
-.. _html_baseurl: https://www.sphinx-doc.org/en/master/usage/configuration.html#confval-html_baseurl
+.. |sphinx_html_baseurl| replace:: ``html_baseurl``
+.. _sphinx_html_baseurl: https://www.sphinx-doc.org/en/master/usage/configuration.html#confval-html_baseurl
 
 |
 
 |readme_src_files|_
  An individual or list of ``rst`` files to parse
 
   Type: ``Union[str, List]``
@@ -161,53 +177,45 @@
 
 .. csv-table::
    :header: |important| Important
 
    "Filepaths should be specified relative to the source directory"
 
 
-.. |readme_src_files| replace:: ``readme_src_files``
-.. _readme_src_files: https://sphinx-readme.readthedocs.io/en/latest/configuration/configuring.html#confval-readme_src_files
-
 |
 
 |readme_docs_url_type|_
  The documentation source to link to when resolving |.`~.sphinx.ext.autodoc`|_ cross-references
 
   Type: ``str``
 
  Must be either ``"code"`` or ``"html"``
 
- * ``"code"``: uses |.`sphinx.ext.linkcode`|_ to replace references with links to highlighted source code
+ * ``"code"``: uses |linkcode| to replace references with links to highlighted source code
 
-   **Example**: |.`~.parse_intersphinx_node`|_
+   **Example**: |.`~.parse_intersphinx_nodes`|_
 
 
  * ``"html"``: replaces references with links to HTML documentation entries
 
-   **Example**: |parse_intersphinx_node_html|_
+   **Example**: |parse_intersphinx_nodes_html|_
 
 
 .. csv-table::
    :header: |note| Note
 
    "If set to ``code``, then :code:`:attr:` cross-references will not be replaced with links
 
    * Instead, they'll be replaced with ``inline literals`` or left as is
    * Please see |readme_replace_attrs|_ and |readme_inline_markup|_"
 
 
-.. |readme_docs_url_type| replace:: ``readme_docs_url_type``
-.. _readme_docs_url_type: https://sphinx-readme.readthedocs.io/en/latest/configuration/configuring.html#confval-readme_docs_url_type
-.. |parse_intersphinx_node_html| replace:: ``parse_intersphinx_node()``
-.. _parse_intersphinx_node_html: http://sphinx-readme.readthedocs.io/en/latest/parser.html#sphinx_readme.parser.READMEParser.parse_intersphinx_node
-.. |readme_replace_attrs| replace:: ``readme_replace_attrs``
-.. _readme_replace_attrs: https://sphinx-readme.readthedocs.io/en/latest/configuration/configuring.html#confval-readme_replace_attrs
-.. |readme_inline_markup| replace:: ``readme_inline_markup``
-.. _readme_inline_markup: https://sphinx-readme.readthedocs.io/en/latest/configuration/configuring.html#confval-readme_inline_markup
+
+.. |parse_intersphinx_nodes_html| replace:: ``parse_intersphinx_nodes()``
+.. _parse_intersphinx_nodes_html: http://sphinx-readme.readthedocs.io/en/latest/parser.html#sphinx_readme.parser.READMEParser.parse_intersphinx_nodes
 
 
 Sample ``conf.py``
 ~~~~~~~~~~~~~~~~~~~
 
 .. code-block:: python
 
@@ -224,17 +232,14 @@
    html_baseurl = "https://sphinx-readme.readthedocs.io/en/latest"
 
    readme_src_files = "README.rst"
 
    readme_docs_url_type = "code"
 
 
-.. |readme_raw_directive| replace:: ``readme_raw_directive``
-.. _readme_raw_directive: https://sphinx-readme.readthedocs.io/en/latest/configuration/configuring.html#confval-readme_raw_directive
-
 
 
 .. csv-table::
    :header: |important| Important
 
    "For platforms that don't support the ``raw`` directive (PyPi, GitLab, and BitBucket),
    be sure to disable |readme_raw_directive|_:
@@ -242,16 +247,15 @@
    .. code-block:: python
 
       readme_raw_directive = False"
 
 
 
 
-
-Documentation
+📚 Documentation
 ~~~~~~~~~~~~~~~~
 
 Full documentation can be found on |docs|_
 
 
 .. |docs| replace:: ``ReadTheDocs``
 .. _docs: https://sphinx-readme.readthedocs.io/en/latest
```

### Comparing `sphinx-readme-0.0.2/setup.py` & `sphinx-readme-0.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `sphinx-readme-0.0.2/sphinx_readme/__init__.py` & `sphinx-readme-0.1.0/sphinx_readme/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,44 +6,45 @@
 from sphinx.environment import BuildEnvironment
 
 from sphinx_readme.utils.sphinx import get_conf_val, set_conf_val
 from sphinx_readme.utils.git import get_repo_dir
 from sphinx_readme.parser import READMEParser
 
 
-__version__ = "v0.0.2"
+__version__ = "v0.1.0"
 
 
 def setup(app: Sphinx) -> Dict[str, Any]:
     # Avoid setting up extension if building on ReadTheDocs
     if os.environ.get("READTHEDOCS") == "True":
         return {}
 
-    app.connect('env-check-consistency', parse_titles)
-    app.connect('doctree-resolved', parse_references)
-    app.connect('build-finished', resolve_readme)
+    app.connect('env-check-consistency', parse_env)
+    app.connect('doctree-resolved', parse_doctree)
+    app.connect('build-finished', resolve)
 
     app.add_config_value("readme_inline_markup", True, True)
     app.add_config_value("readme_raw_directive", True, True)
     app.add_config_value("readme_include_directive", True, True)
     app.add_config_value("readme_replace_attrs", True, True)
     app.add_config_value("readme_out_dir", get_repo_dir(), True)
     app.add_config_value("readme_blob", 'head', True)
     app.add_config_value("readme_default_admonition_icon", "📄", True)
 
     set_conf_val(app, 'READMEParser', READMEParser(app))
 
     return {'version': sphinx.__display_version__, 'parallel_read_safe': True}
 
-def parse_titles(app: Sphinx, env: BuildEnvironment):
-    readme = get_conf_val(app, 'READMEParser')
-    readme.parse_titles(env)
 
+def parse_env(app: Sphinx, env: BuildEnvironment):
+    parser = get_conf_val(app, 'READMEParser')
+    parser.parse_env(env)
 
-def parse_references(app: Sphinx, doctree: document, docname: str):
-    readme = get_conf_val(app, 'READMEParser')
-    readme.parse(app, doctree, docname)
 
+def parse_doctree(app: Sphinx, doctree: document, docname: str):
+    parser = get_conf_val(app, 'READMEParser')
+    parser.parse_doctree(app, doctree, docname)
 
-def resolve_readme(app: Sphinx, exception):
-    readme = get_conf_val(app, 'READMEParser')
-    readme.resolve()
+
+def resolve(app: Sphinx, exception):
+    parser = get_conf_val(app, 'READMEParser')
+    parser.resolve()
```

### Comparing `sphinx-readme-0.0.2/sphinx_readme/config.py` & `sphinx-readme-0.1.0/sphinx_readme/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import re
 from pathlib import Path
-from typing import Union, List, Dict
+from typing import Union, List, Dict, Callable
 from functools import cached_property
 
 from sphinx.application import Sphinx
 from sphinx.errors import ExtensionError
 
 from sphinx_readme.utils.git import get_repo_url, get_blob_url, get_repo_host, get_repo_dir
 from sphinx_readme.utils.rst import replace_only_directives, remove_raw_directives
@@ -79,37 +79,31 @@
                 )
         else:  # ``docs_url_type`` is "code"
             docs_url = self.blob_url
 
         return docs_url.rstrip("/")
 
     def setup_linkcode_resolve(self, app: Sphinx) -> None:
-        """Retrieves or defines a ``linkcode_resolve()`` function for your package
-        and enables the :mod:`sphinx.ext.linkcode` extension
-
-        .. tip:: The linkcode extension is only used if
-           :confval:`readme_docs_url_type` is ``"code"``
-        """
+        """Retrieves or defines a ``linkcode_resolve()`` function for your package"""
         linkcode_func = get_conf_val(app, "linkcode_resolve")
 
         if not callable(linkcode_func):
             self.logger.debug(
                 "``sphinx_readme:`` using default ``linkcode_resolve``"
             )
             # Get the template for linking to source code
             linkcode_url = get_linkcode_url(self.blob_url)
             linkcode_func = get_linkcode_resolve(linkcode_url)
 
         set_conf_val(app, 'linkcode_resolve', linkcode_func)
-        app.setup_extension("sphinx.ext.linkcode")
 
-    def read_rst(self, rst_file: Union[str, Path], replace_only: bool = False) -> str:
+    def read_rst(self, rst_file: Union[str, Path], replace_only: bool = True) -> str:
         """Reads and partially parses an ``rst`` file
 
-        .. hint::
+        .. tip::
 
            Files are parsed as follows:
 
            1. If ``replace_only`` is ``True``, only directives are replaced via
               :func:`~.replace_only_directives`
 
            2. If :confval:`readme_include_directive` is ``True``, include directives are
```

### Comparing `sphinx-readme-0.0.2/sphinx_readme/parser.py` & `sphinx-readme-0.1.0/sphinx_readme/parser.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,241 +1,139 @@
 import re
-import copy
 from pathlib import Path
 from collections import defaultdict
-from typing import Dict, List, Tuple, Set, Union
+from functools import cached_property
+from typing import Dict, List, Set, Union, Callable, Optional
 
 from docutils import nodes
-from docutils.nodes import document
-
 from sphinx import addnodes
-from sphinx.application import Sphinx
-from sphinx.testing import restructuredtext
-from sphinx.transforms import SphinxTransformer
-from sphinx.environment import BuildEnvironment
+from sphinx.domains.python import ObjectEntry
+from sphinx.application import Sphinx, BuildEnvironment
 
 from sphinx_readme.config import READMEConfig
-from sphinx_readme.utils.rst import get_all_xref_variants, escape_rst, format_rst
+from sphinx_readme.utils.sphinx import get_conf_val
+from sphinx_readme.utils.docutils import get_doctree
+from sphinx_readme.utils.rst import get_all_xref_variants, escape_rst, format_rst, replace_attrs, format_hyperlink
 
 
 class READMEParser:
 
-    REFERENCE_MAP = {
-        "ref": [],
-        "doc": []
-    }
-
     def __init__(self, app: Sphinx):
         #: The :class:`~.READMEConfig` for the parser
         self.config: READMEConfig = READMEConfig(app)
         self.logger = self.config.logger
         #: Mapping of info for standard and :mod:`sphinx.ext.autodoc` cross-references
-        self.ref_map: Dict[str, Union[List, Dict]] = copy.deepcopy(self.REFERENCE_MAP)
+        self.ref_map: Dict[str, Union[List, Dict]] = {}
         #: Mapping of source files to their content
         self.sources: Dict[str, str] = self.config.sources
         #: Mapping of source files to their toctree data
         self.toctrees: Dict[str, List[Dict]] = defaultdict(list)
-        # Mapping of source files to their admonition data
+        #: Mapping of source files to their admonition data
         self.admonitions: Dict[str, Dict[str, List[Dict]]] = {}
-        # Mapping of docnames to their parsed titles
+        #: Mapping of docnames to their parsed titles
         self.titles: Dict[str, str] = {}
+        #: Standard cross-reference roles
+        self.roles: Set[str] = {"doc", "ref"}
 
-    def parse(self, app: Sphinx, doctree: document, docname: str) -> None:
-        """Parses cross-reference, admonition, and toctree data from a resolved doctree"""
-        # If a source has ``only`` directives, its doctree will have missing/extra content
-        # Replace the ``only`` directives, then generate a new doctree to parse if needed
-        doctree = self.get_doctree(app, doctree, docname)
-
-        inline_nodes = list(doctree.findall(nodes.inline))
-        literal_nodes = list(doctree.findall(nodes.literal))
-
-        self.parse_autodoc_nodes(literal_nodes, docname)
-
-        if self.config.docs_url_type == "code":
-            self.parse_linkcode_nodes(inline_nodes)
-
-        if doctree.get('source') in self.sources:
-            self.parse_xref_nodes(inline_nodes)
-            self.parse_admonitions(doctree)
-            self.parse_toctrees(doctree)
-
-    def get_doctree(self, app: Sphinx, doctree: document, docname: str) -> document:
-        """Generates and resolves a new doctree for :attr:`~.src_files`
-        that contain :rst:dir:`only` directives
-        """
-        # Return original doctree if file is not a readme source
-        if (src := doctree.get('source')) not in self.sources:
-            return doctree
-
-        # Parse ``only`` directives to get true source rst of README version
-        parsed_rst = self.config.read_rst(src, replace_only=True)
-        raw_rst = self.sources[src]
-
-        # Return original doctree if file had no ``only`` directives
-        if parsed_rst == raw_rst:
-            return doctree
-
-        self.sources[src] = parsed_rst
-
-        # Use temp docname to avoid duplicate warnings
-        docname = docname + "_readme"
-
-        # Generate new doctree from parsed rst using Sphinx application
-        doctree = restructuredtext.parse(app, parsed_rst, docname)
-
-        # Resolve references in the doctree
-        try:
-            backup = copy.deepcopy(app.env.temp_data)
-            app.env.temp_data['docname'] = docname
-
-            transformer = SphinxTransformer(doctree)
-            transformer.set_environment(app.env)
-            transformer.add_transforms(app.registry.get_post_transforms())
-            transformer.apply_transforms()
-
-        finally:
-            app.env.temp_data = backup
+    def parse_env(self, env: BuildEnvironment) -> None:
+        """Parses domain data and document titles from the |env|"""
+        self.parse_titles(env)
+        self.parse_py_domain(env)
+        self.parse_std_domain(env)
 
-        # Replace temp source with actual source
-        doctree['source'] = src
-        return doctree
-
-    def parse_xref_nodes(self, inline_nodes: List[nodes.inline]) -> None:
-        """Adds node data from :rst:role:`doc` or :rst:role:`ref` cross-references to the :attr:`~ref_map`
-
-        :param inline_nodes: the inline nodes from the document being parsed
-        """
-        for node in inline_nodes:
-            if 'doc' in node['classes']:
-                self.ref_map['doc'].append(self._parse_xref(node))
+    def parse_titles(self, env: BuildEnvironment) -> None:
+        """Parses document titles from the |env|"""
+        for docname, title_node in env.titles.items():
+            parts = []
 
-            elif 'std-ref' in node['classes']:
-                self.ref_map['ref'].append(self._parse_xref(node))
+            for child in title_node.children:
+                text = child.astext()
+                if isinstance(child, nodes.literal):
+                    parts.append(f"``{text}``")
+                else:
+                    parts.append(text)
 
-    def _parse_xref(self, node: nodes.inline) -> Dict[str, str]:
-        """Helper function to parse target info of a ``:ref:`` or ``:doc:`` xref"""
-        return {
-            'text': node.children[0].astext(),
-            "refuri": self.config.html_baseurl + "/" + node.parent.get('refuri', '')
-        }
+            self.titles[docname] = ' '.join(parts)
 
-    def parse_autodoc_nodes(self, literal_nodes: List[nodes.literal], docname: str) -> None:
-        """Parses node data from :mod:`sphinx.ext.autodoc` cross-references
+    def parse_std_domain(self, env: BuildEnvironment) -> None:
+        """Parses cross-reference data from the |std_domain|
 
-        :param literal_nodes: the literal nodes from the document being parsed
+        :param env: the |env|
         """
-        for node in literal_nodes:
-            if 'py' not in node['classes']:
-                continue
-
-            if not isinstance(node.parent, nodes.reference):
-                continue
+        domain = env.get_domain("std")
+        self.roles.update(set(domain.object_types))
 
-            if node.parent.get('internal') is False:
-                # External links are xrefs from intersphinx
-                self.parse_intersphinx_node(node)
+        for ref_id, text, role, docname, anchor, _ in domain.get_objects():
+            replace = self.titles.get(ref_id) or text
+            target = f"{self.config.html_baseurl}/{docname}.html"
 
-            elif 'py-mod' in node['classes']:
-                # Parse :mod: xrefs regardless of docs_url_type
-                self.parse_module_node(node, docname)
+            if anchor:
+                target += f"#{anchor}"
 
-            elif self.config.docs_url_type == "html":
-                # Only parse remaining py xrefs if linking to html
-                self.parse_autodoc_node(node, docname)
-
-    def parse_intersphinx_node(self, node: nodes.literal) -> None:
-        """Adds node data from a :mod:`sphinx.ext.intersphinx` cross-reference to the :attr:`~ref_map`
-
-        :param node: the literal node of an external :mod:`~sphinx.ext.autodoc` reference
-        """
-        pattern = r":(mod|class|meth|func|attr):`~?\.?[.\w]+`"
-        match = re.match(pattern, node.rawsource)
-        target = node.parent.get('refuri')
+            if role == "confval" and self.config.inline_markup:
+                replace = f"``{replace}``"
 
-        if not all((match, target)):
-            return
+            elif role == "label":
+                role = "ref"
 
-        is_callable = match.group(1) in ("meth", "func")
-        qualified_name = target.split("#")[-1].split("-")[-1]
-        self.add_variants(qualified_name, target, is_callable)
+            self.ref_map.setdefault(role, {})[ref_id] = {
+                "replace": replace,
+                "target": target
+            }
 
-    def parse_module_node(self, node: nodes.literal, docname: str) -> None:
-        """Adds node data from a ``:mod:`` cross-reference to the :attr:`ref_map`
+    def parse_py_domain(self, env: BuildEnvironment) -> None:
+        """Parses cross-reference data for |py_domain| objects
 
-        :param node: a literal node with the ``"py-mod"`` class
-        :param docname: the name of the document containing the node
+        :param env: the |env|
         """
-        qualified_name = node.parent.get("reftitle", "")
+        py_objects = env.domaindata.get('py', {}).get("objects", {})
+        linkcode_resolve = get_conf_val(env, "linkcode_resolve")
 
-        if self.config.docs_url_type == 'code':
-            # Ex. sphinx_readme.parser -> sphinx_readme/parser.py
-            refuri = qualified_name.replace('.', '/') + '.py'
-        else:
-            refuri = self._parse_refuri(node, docname)
-
-        if not all((qualified_name, refuri)):
-            return
-
-        target = f"{self.config.docs_url}/{refuri}"
-        self.add_variants(qualified_name, target)
+        for qualname, entry in py_objects.items():
+            if target := self.get_py_target(entry, linkcode_resolve):
+                self.add_variants(
+                    qualified_name=qualname,
+                    target=target,
+                    is_callable=entry.objtype in ("method", "function"))
 
-    def parse_autodoc_node(self, node: nodes.literal, docname: str) -> None:
-        """Adds node data from any :mod:`sphinx.ext.autodoc` cross-reference except ``:mod:`` to the :attr:`ref_map`
+    def get_py_target(self, entry: ObjectEntry, linkcode_resolve: Optional[Callable] = None) -> Optional[str]:
+        """Resolves the target for a cross-reference to an object in the |py_domain|
 
-        :param node: a literal node with the ``"py-{class|func|meth|attr}"`` class
-        :param docname: the name of the document containing the node
+        :param entry: the ``ObjectEntry`` for the object
+        :param linkcode_resolve: function to resolve targets when linking to source code
+        :return: the link to the object's corresponding documentation entry or highlighted source code
         """
-        qualified_name = node.parent.get("reftitle")
-        refuri = self._parse_refuri(node, docname)
+        if self.config.docs_url_type == "html":
+            # All links to html documentation follow the same format
+            return f"{self.config.html_baseurl}/{entry.docname}.html#{entry.node_id}"
 
-        if not all((refuri, qualified_name)):
-            return
+        # Links to source code depend on the object type
+        if entry.objtype in ("property", "attribute", "data", "decorator"):
+            return None  # Cannot link to source code
 
-        is_callable = bool(re.match(r":(meth|func):", node.rawsource))
-        target = f"{self.config.docs_url}/{refuri}"
-        self.add_variants(qualified_name, target, is_callable)
+        if entry.objtype == "module":  # Link to the file in the repository
+            filepath = entry.node_id.removeprefix("module-").replace(".", "/")
+            return f"{self.config.blob_url}/{filepath}.py"
 
-    def _parse_refuri(self, node: nodes.literal, docname: str) -> str:
-        """Helper function to parse the target of a :mod:`sphinx.ext.autodoc` cross-reference"""
-        if 'refuri' in node.parent:
-            # Ex. ../parser.html#sphinx_readme.parser.READMEParser
-            return node.parent["refuri"].lstrip("./")
+        # For class/meth/func, use linkcode_resolve
+        info = dict.fromkeys(("module", "fullname"))
+        parts = entry.node_id.split('.')
 
-        elif 'refid' in node.parent:
-            # Ex. sphinx_readme.parser.READMEParser
-            return f"{docname}.html#{node.parent['refid']}"
+        # TODO: look into autoexception and autodecorator
+        if entry.objtype in ("class", "function"):
+            info["module"] = '.'.join(parts[:-1])
+            info['fullname'] = parts[-1]
 
-    def parse_linkcode_nodes(self, inline_nodes: List[nodes.inline]) -> None:
-        """Parses data from nodes added by :mod:`sphinx.ext.linkcode`
-
-        :param inline_nodes: the inline nodes from the document being parsed
-        """
-        for node in inline_nodes:
-            if 'viewcode-link' in node['classes'] or 'linkcode-link' in node['classes']:
-                if node.parent.get('internal') is False:
-                    # Only parse links to external source code
-                    self.parse_linkcode_node(node)
+        elif entry.objtype == "method":
+            info["module"] = '.'.join(parts[:-2])
+            info['fullname'] = '.'.join(parts[-2:])
 
-    def parse_linkcode_node(self, node: nodes.inline) -> None:
-        """Adds node data from a :mod:`~sphinx.ext.linkcode` node to the :attr:`ref_map`
+        return linkcode_resolve("py", info)
 
-        :param node: an inline node added by :mod:`sphinx.ext.linkcode`
-        """
-        grandparent = node.parent.parent
-        is_callable = grandparent.get("_toc_name", "").endswith("()")
-
-        try:
-            qualified_name = grandparent.get("ids")[0]
-        except IndexError:
-            qualified_name = grandparent.get("module", "") + grandparent.get("fullname", "")
-
-        target = node.parent.get("refuri")
-        self.add_variants(qualified_name, target, is_callable)
-
-    def add_variants(self, qualified_name: str, target: str, is_callable: bool = False):
+    def add_variants(self, qualified_name: str, target: str, is_callable: bool = False) -> None:
         """Adds substitution information for an object to the :attr:`ref_map`
 
         This data is used to replace any :mod:`~sphinx.ext.autodoc` cross-reference to
         the object with a substitution, hyperlinked to the corresponding
         source code or documentation entry
 
         .. tip:: See :func:`~.get_all_xref_variants` and :meth:`replace_autodoc_refs`
@@ -263,55 +161,32 @@
                 replace = f"``{replace}``"
 
             self.ref_map[variant] = {
                 'replace': replace,
                 'target': target
             }
 
-    def parse_titles(self, env: BuildEnvironment) -> None:
-        """Parses document titles from the :class:`~.BuildEnvironment`"""
-        for docname, title_node in env.titles.items():
-            parts = []
-
-            for child in title_node.children:
-                text = child.astext()
-                if isinstance(child, nodes.literal):
-                    parts.append(f"``{text}``")
-                else:
-                    parts.append(text)
-
-            self.titles[docname] = ' '.join(parts)
-
-    def parse_toctrees(self, doctree: addnodes.document) -> None:
-        """Parses the caption and entry data from :class:`~.sphinx.addnodes.toctree` nodes
-
-        .. caution:: Toctrees are currently parsed as if the directive has the ``:titlesonly:`` option
-
-        :param doctree: the doctree from one of the :attr:`~.src_files`
-        """
-        source = doctree.get('source')
-        for toctree in list(doctree.findall(addnodes.toctree)):
-            toc = {
-                'caption': toctree.get('caption'),
-                'entries': []
-            }
-            for _, entry in toctree.get('entries', []):
-                toc['entries'].append({
-                    'entry': entry,
-                    'title': self.titles.get(entry),
-                })
-            self.toctrees[source].append(toc)
+    def parse_doctree(self, app: Sphinx, doctree: nodes.document, docname: str) -> None:
+        """Parses cross-reference, admonition, and toctree data from a resolved doctree"""
+        if doctree.get('source') in self.sources:
+            self.parse_admonitions(app, doctree, docname)
+            self.parse_intersphinx_nodes(doctree)
+            self.parse_toctrees(doctree)
 
-    def parse_admonitions(self, doctree: nodes.document) -> None:
+    def parse_admonitions(self, app: Sphinx, doctree: nodes.document, docname: str) -> None:
         """Parses data from generic and specific admonitions
 
         :param doctree: the doctree from one of the :attr:`~.src_files`
         """
         admonitions = {'generic': [], 'specific': []}
         src = doctree.get('source')
+        rst = self.sources[src]
+
+        # Generate new doctree to account for only directives
+        doctree = get_doctree(app, rst, docname)
 
         for admonition in list(doctree.findall(nodes.Admonition)):
             info = {
                 'body': admonition.rawsource
             }
             if isinstance(admonition, nodes.admonition):
                 # Generic Admonition (using admonition directive)
@@ -326,32 +201,78 @@
                     'class': admonition.tagname,
                     'title': admonition.tagname.title(),
                 })
                 admonitions['specific'].append(info)
 
         self.admonitions[src] = admonitions
 
+    def parse_intersphinx_nodes(self, doctree: nodes.document) -> None:
+        """Parses :mod:`sphinx.ext.autodoc` cross-references that utilize :mod:`sphinx.ext.intersphinx`
+
+        :param doctree: the doctree from one of the :attr:`~.src_files`
+        """
+        for node in doctree.findall(nodes.literal):
+            if not isinstance(node.parent, nodes.reference):
+                continue
+
+            if node.parent.get('internal') is True:
+                continue
+
+            if 'py' not in node['classes']:
+                continue
+
+            pattern = r":(mod|class|meth|func|attr):`~?\.?[.\w]+`"
+            match = re.match(pattern, node.rawsource)
+            target = node.parent.get('refuri')
+
+            if not all((match, target)):
+                continue
+
+            is_callable = match.group(1) in ("meth", "func")
+            qualified_name = target.split("#")[-1].split("-")[-1]
+            self.add_variants(qualified_name, target, is_callable)
+
+    def parse_toctrees(self, doctree: nodes.document) -> None:
+        """Parses the caption and entry data from :class:`~.sphinx.addnodes.toctree` nodes
+
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
     def resolve(self) -> None:
-        """Uses the data from :meth:`parse` to replace cross-references and directives in the :attr:`~.src_files`
+        """Uses parsed data from to replace cross-references and directives in the :attr:`~.src_files`
 
         Once resolved, files are written to the :attr:`~.out_dir`.
         """
         for src, rst in self.sources.items():
-            # Replace everything using data from ``parse()``
+            # Replace everything using parsed data
             rst = self.replace_admonitions(src, rst)
             rst = self.replace_rst_images(src, rst)
             rst = self.replace_toctrees(src, rst)
             rst = self.replace_rst_rubrics(rst)
+            rst = self.replace_py_xrefs(rst)
 
-            for role in ('ref', 'doc'):
-                rst = self.replace_cross_refs(role, rst)
+            for role in self.roles:
+                rst = self.replace_std_xrefs(role, rst)
 
             # Use ref_map to generate autodoc substitution definitions
-            rst, autodoc_refs = self.replace_autodoc_refs(rst)
-            header_vals = self.get_header_vals(autodoc_refs)
+            header_vals = self.get_header_vals()
 
             # Write the final output
             rst_out = Path(self.config.out_dir, Path(src).name)
 
             with open(rst_out, 'w', encoding='utf-8') as f:
                 f.write(
                     "\n".join(header_vals) + "\n\n" + rst)
@@ -402,43 +323,34 @@
 
         .. note:: Entries will link to HTML documentation regardless of the
            value of :confval:`readme_docs_url_type`
 
         :param rst_src: absolute path of the source file
         :param rst: content of the source file
         """
-        pattern = r".. toctree::\n+?(?:\s+:\w+:\s*?\w*?\n\s+)*?(?:\s+\w+\n)+?(?=\n+\S+?)"
-        toctrees = re.findall(pattern, rst)
+        pattern = r"\.\. toctree::\s*?\n+?(?:^[ ]+.+?$|^\s*$)+?(?=\n*\S+|\Z)"
+        toctrees = re.findall(pattern, rst, re.M | re.DOTALL)
 
         for toctree, info in zip(toctrees, self.toctrees[rst_src]):
             substitutions = []
             repl = ""
 
             if info['caption']:
                 repl += f"**{info['caption']}**\n\n"
 
             for entry in info['entries']:
                 # Replace each entry with a link to html docs
                 target = f"{self.config.html_baseurl}/{entry['entry']}.html"
-
-                if "`" in entry['title']:
-                    # Inline markup in links must be inserted with substitutions
-                    sub = entry['title'].replace('`', '')
-                    substitutions.extend([
-                        f".. |{sub}| replace:: {entry['title']}",
-                        f".. _{sub}: {target}"
-                    ])
-                    repl += f"* |{sub}|_\n"
-
-                else:
-                    # Replace with a normal link otherwise
-                    repl += f"* `{entry['title']} <{target}>`_\n"
+                link, subs = format_hyperlink(target, text=entry['title'])
+                substitutions.extend(subs)
+                repl += f"* {link}\n"
 
             if substitutions:
-                repl += '\n\n' + '\n'.join(substitutions) + '\n\n'
+                # Inline literals in links must use substitutions
+                repl += '\n' + '\n'.join(substitutions) + '\n'
 
             # Replace toctree directive with links and substitution defs
             rst = rst.replace(toctree, repl)
 
         return rst
 
     def replace_rst_images(self, rst_src: str, rst: str) -> str:
@@ -524,105 +436,92 @@
                 )
         return re.sub(
             pattern=rubric_pattern,
             repl=lambda m: format_rst("bold", m.group(1)),
             string=rst
         )
 
-    def replace_cross_refs(self, ref_role: str, rst: str) -> str:
-        """Replaces cross-references using the :rst:role:`doc` or :rst:role:`ref` role
+    def replace_std_xrefs(self, ref_role: str, rst: str) -> str:
+        """Replaces cross-references from the |std_domain|
+
+        .. hint::
+
+           This includes cross-references using the :rst:role:`doc`
+           or :rst:role:`ref` role, as well as any custom objects added by
+           :meth:`Sphinx.add_object_type() <sphinx.application.Sphinx.add_object_type>`
 
         :param ref_role: the name of the cross-reference role
         :param rst: content of the source file
         """
-        # Find all :ref_role:`ref_id` cross-refs
-        cross_refs = re.findall(
-            pattern=fr"(?:\s*?):{ref_role}:`([^`]+)`(?=\s*?)",
+        # Find all :ref_role:`ref_id` or :ref_role:`title <ref_id>` cross-refs
+        xrefs = re.findall(
+            pattern=fr"(?:\s*?):{ref_role}:`(([^`]+?)(?:\s<([\w./]+?)>)?)`(?=\s*?)",
             string=rst
         )
-        # Match these ids up with target data in the ref_map
-        cross_ref_map = dict(zip(cross_refs, self.ref_map[ref_role]))
+        substitutions = []
+
+        for xref in xrefs:
+            if not all(xref):  # :ref_role:`ref_id` ->  ('ref_id', 'ref_id', '')
+                ref, ref_id, title = xref
+
+            else:  # :ref_role:`title <ref_id>` -> ('title <ref_id>', 'title', 'ref_id')
+                ref, title, ref_id = xref
+
+            # Match these ids up with target data in the ref_map
+            if info := self.ref_map.get(ref_role, {}).get(ref_id, {}):
+                # Replace cross-refs with `text <link>`_ or substitutions
+                link, subs = format_hyperlink(
+                    target=info['target'],
+                    text=title or info['replace']
+                )
+                substitutions.extend(subs)
+                rst = re.sub(
+                    pattern=rf":{ref_role}:`{escape_rst(ref)}`",
+                    repl=link,
+                    string=rst
+                )
+        if substitutions:
+            # Substitutions are used for inline literals
+            rst = "\n".join(substitutions) + "\n\n" + rst
 
-        # Replace cross-refs with `text <link>`_ format
-        for ref_id, target in cross_ref_map.items():
-            rst = re.sub(
-                pattern=rf":{ref_role}:`{ref_id}`",
-                repl=rf"`{target['text']} <{target['refuri']}>`_",
-                string=rst
-            )
         return rst
 
-    def replace_autodoc_refs(self, rst: str) -> Tuple[str, Set]:
+    def replace_py_xrefs(self, rst: str) -> str:
         """Replace :mod:`~sphinx.ext.autodoc` cross-references with substitutions
 
         These substitutions will be hyperlinked to the corresponding source code
         or HTML documentation entry, depending on the value of
         :confval:`readme_docs_url_type`
 
         .. note: Attributes will only be hyperlinked
            if linking to HTML documentation
 
         :param rst: content of the source file
-        :returns: subbed rst and all autodoc xref targets found within it
         """
-        # :role:`{~.}{module|class}{.}target` where {} is optional
-        pattern = r":(?:mod|class|meth|func):`([~\.\w]+)`"
-
-        if self.config.replace_attrs:
-            if self.config.docs_url_type == 'html':
-                # If linking to HTML docs, we can generate cross-refs for attributes
-                pattern = r":(?:mod|class|meth|func|attr):`([~\.\w]+)`"
-            else:
-                # If linking to source code, just replace :attr:`~.attribute` with ``attribute``
-                rst = self.replace_autodoc_attrs(rst)
-
         # To render on GitHub/PyPi/etc., we use Sphinx substitutions instead of cross-refs
         # Syntax is |.{ref}|_ or |.`{ref}`|_
         if self.config.inline_markup:
             repl = r"|.`\1`|_"
         else:
             repl = r"|.\1|_"
 
-        # Get a set of all autodoc cross-refs
-        autodoc_refs = set(re.findall(pattern, rst))
-
         # Replace cross-refs with substitutions
-        rst = re.sub(pattern, repl, rst)
-
-        # Use autodoc_refs and ref_map to generate substitution definitions
-        return rst, autodoc_refs
-
-    def replace_autodoc_attrs(self, rst: str) -> str:
-        """Replaces ``:attr:`` cross-references with ``inline literals``
+        rst = re.sub(self.py_xref_regex, repl, rst)
 
-        .. hint::
-
-           This method is only called if both
+        # If linking to source code, replace :attr:`~.attribute` with ``attribute``
+        if self.config.docs_url_type == "code" and self.config.replace_attrs:
+            rst = replace_attrs(rst)
 
-           1. :confval:`readme_docs_url_type` is ``"code"``
-           2. :confval:`readme_replace_attrs` is ``True``
-        """
-        # Ex. ~.Class.meth => ``meth``
-        short_ref = r" :attr:`~\.?(\w+)`"
-        # Ex. .Class.meth => ``Class.meth``
-        long_ref = r" :attr:`\.?([\.\w]+)`"
-        repl = r" ``\1``"
-
-        rst = re.sub(short_ref, repl, rst)
-        rst = re.sub(long_ref, repl, rst)
         return rst
 
-    def get_header_vals(self, autodoc_refs: Set) -> List[str]:
-        """Returns a list of substitution definitions and hyperlink references to prepend to the file
-
-        :param autodoc_refs: :mod:`sphinx.ext.autodoc` targets to define substitutions for
-        """
+    def get_header_vals(self) -> List[str]:
+        """Returns a list of substitution definitions and hyperlink references to prepend to the file"""
         header = []
 
-        for ref in autodoc_refs:
+        for ref in self.py_xrefs:
             info = self.ref_map.get(ref)
 
             # Check for invalid ref
             if info is None:
                 continue
 
             if self.config.inline_markup:
@@ -635,14 +534,34 @@
 
         if not self.config.raw_directive:
             for _type, icon in self.config.icon_map.items():
                 header.append(f'.. |{_type}| replace:: {icon}')
 
         return header
 
+    @cached_property
+    def py_xrefs(self) -> Set[str]:
+        """Python domain cross-reference targets found within source files"""
+        xrefs = set()
+        for src, rst in self.sources.items():
+            xrefs.update(
+                set(re.findall(self.py_xref_regex, rst)))
+        return xrefs
+
+    @cached_property
+    def py_xref_regex(self) -> str:
+        """The regular expression to match Python domain cross-references"""
+        roles = r"mod|class|meth|func"
+        # If linking to HTML docs, we can generate cross-refs for attributes
+        if self.config.docs_url_type == "html":
+            if self.config.replace_attrs:
+                roles += "|attr"
+
+        return rf":(?:{roles}):`(~?\.?[.\w]+)`"
+
     def get_admonition_regex(self, admonition: Dict[str, str], admonition_type: str) -> str:
         """Returns the regex to match a specific admonition directive
 
         :param admonition: a dict containing admonition data
         :param admonition_type: ``"generic"`` or ``"specific"``
         """
         body = escape_rst(admonition['body'])
@@ -672,15 +591,15 @@
         else:
             # raw html template body uses string formatting
             pattern += rf"{body}"
 
         pattern += r"(?=[\n\S]+?)"
         return pattern
 
-    def get_admonition_icon(self, admonition: dict):
+    def get_admonition_icon(self, admonition: dict) -> str:
         """Returns the icon to use for an admonition
 
         :param admonition: a dict of admonition data
         """
         icon = self.config.icon_map.get(admonition['class'])
 
         # Raw directive allows for using icon directly
```

### Comparing `sphinx-readme-0.0.2/sphinx_readme/utils/git.py` & `sphinx-readme-0.1.0/sphinx_readme/utils/git.py`

 * *Files identical despite different names*

### Comparing `sphinx-readme-0.0.2/sphinx_readme/utils/linkcode.py` & `sphinx-readme-0.1.0/sphinx_readme/utils/linkcode.py`

 * *Files identical despite different names*

### Comparing `sphinx-readme-0.0.2/sphinx_readme/utils/sphinx.py` & `sphinx-readme-0.1.0/sphinx_readme/utils/sphinx.py`

 * *Files identical despite different names*

### Comparing `sphinx-readme-0.0.2/sphinx_readme.egg-info/PKG-INFO` & `sphinx-readme-0.1.0/sphinx_readme.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-readme
-Version: 0.0.2
+Version: 0.1.0
 Summary: Generate Beautiful reStructuredText README.rst for GitHub, PyPi, GitLab, BitBucket
 Home-page: https://github.com/tdkorn/sphinx-readme
 Author: Adam Korn
 Author-email: hello@dailykitten.net
 License: MIT License
 Download-URL: https://github.com/TDKorn/sphinx-readme/tarball/main
 Keywords: sphinx,docutils,sphinx-extension,sphinx-contrib,reStructuredText,rst,reST,parser,rst-parser,README.rst,README,autodoc,linkcode
@@ -12,43 +12,58 @@
 Classifier: Framework :: Sphinx :: Extension
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/x-rst; charset=UTF-8
 License-File: LICENSE
 
-.. |.`~.sphinx.ext.autodoc`| replace:: ``autodoc``
-.. _.`~.sphinx.ext.autodoc`: https://www.sphinx-doc.org/en/master/usage/extensions/autodoc.html#module-sphinx.ext.autodoc
+.. |.`~.parse_intersphinx_nodes`| replace:: ``parse_intersphinx_nodes()``
+.. _.`~.parse_intersphinx_nodes`: https://github.com/TDKorn/sphinx-readme/blob/v0.1.0/sphinx_readme/parser.py#L208-L232
 .. |.`sphinx.ext.linkcode`| replace:: ``sphinx.ext.linkcode``
 .. _.`sphinx.ext.linkcode`: https://www.sphinx-doc.org/en/master/usage/extensions/linkcode.html#module-sphinx.ext.linkcode
-.. |.`~.parse_intersphinx_node`| replace:: ``parse_intersphinx_node()``
-.. _.`~.parse_intersphinx_node`: https://github.com/TDKorn/sphinx-readme/blob/v0.0.2/sphinx_readme/parser.py#L145-L159
+.. |.`~.sphinx.ext.autodoc`| replace:: ``autodoc``
+.. _.`~.sphinx.ext.autodoc`: https://www.sphinx-doc.org/en/master/usage/extensions/autodoc.html#module-sphinx.ext.autodoc
 .. |.`sphinx.ext.autodoc`| replace:: ``sphinx.ext.autodoc``
 .. _.`sphinx.ext.autodoc`: https://www.sphinx-doc.org/en/master/usage/extensions/autodoc.html#module-sphinx.ext.autodoc
 .. |attention| replace:: 🔔️
 .. |caution| replace:: ⚠️
 .. |danger| replace:: ☢️
 .. |error| replace:: ⛔
 .. |hint| replace:: 🧠
 .. |important| replace:: 📢
 .. |note| replace:: 📝
 .. |tip| replace:: 💡
 .. |warning| replace:: 🚩
 .. |default| replace:: 📄
 .. |about| replace:: 📚
 
+.. |html_context| replace:: ``html_context``
+.. _html_context: https://sphinx-readme.readthedocs.io/en/latest/configuration/configuring.html#confval-html_context
+.. |html_baseurl| replace:: ``html_baseurl``
+.. _html_baseurl: https://sphinx-readme.readthedocs.io/en/latest/configuration/configuring.html#confval-html_baseurl
+.. |readme_src_files| replace:: ``readme_src_files``
+.. _readme_src_files: https://sphinx-readme.readthedocs.io/en/latest/configuration/configuring.html#confval-readme_src_files
+.. |readme_docs_url_type| replace:: ``readme_docs_url_type``
+.. _readme_docs_url_type: https://sphinx-readme.readthedocs.io/en/latest/configuration/configuring.html#confval-readme_docs_url_type
+.. |readme_replace_attrs| replace:: ``readme_replace_attrs``
+.. _readme_replace_attrs: https://sphinx-readme.readthedocs.io/en/latest/configuration/configuring.html#confval-readme_replace_attrs
+.. |readme_inline_markup| replace:: ``readme_inline_markup``
+.. _readme_inline_markup: https://sphinx-readme.readthedocs.io/en/latest/configuration/configuring.html#confval-readme_inline_markup
+.. |readme_raw_directive| replace:: ``readme_raw_directive``
+.. _readme_raw_directive: https://sphinx-readme.readthedocs.io/en/latest/configuration/configuring.html#confval-readme_raw_directive
+
 .. meta::
    :author: Adam Korn
    :title: Sphinx README
    :description: Sphinx Extension to Generate Beautiful reStructuredText README.rst for GitHub, PyPi, GitLab, BitBucket
 
 Sphinx README - Generate Beautiful ``README.rst`` for GitHub, PyPi, GitLab, BitBucket
 --------------------------------------------------------------------------------------
 
-.. image:: https://raw.githubusercontent.com/TDKorn/sphinx-readme/v0.0.2/docs/source/_static/logo_transparent.png
+.. image:: https://raw.githubusercontent.com/TDKorn/sphinx-readme/v0.1.0/docs/source/_static/logo_transparent.png
    :alt: Sphinx README: Generate Beautiful reStructuredText README.rst for GitHub, PyPi, GitLab, BitBucket
    :align: center
    :width: 25%
 
 A Sphinx extension to generate ``README.rst`` files that render beautifully on GitHub, PyPi, GitLab, BitBucket
 
 
@@ -93,35 +108,35 @@
 **With** ``sphinx_readme`` **, there's no need to rewrite your** ``README.rst`` **as a** ``README.md`` **file**
 
 Files generated by ``sphinx_readme`` have nearly identical appearance and functionality
 as ``html`` builds, including |.`sphinx.ext.autodoc`|_ cross-references!
 
 |
 
-.. image:: https://raw.githubusercontent.com/TDKorn/sphinx-readme/v0.0.2/docs/source/_static/demo/demo.gif
+.. image:: https://raw.githubusercontent.com/TDKorn/sphinx-readme/v0.1.0/docs/source/_static/demo/demo.gif
    :alt: Demonstration of how reStructuredText README.rst files generated by Sphinx README render on GitHub, PyPi, GitLab, BitBucket
    :width: 75%
 
 
-Features
-~~~~~~~~~~
+📋 Features
+~~~~~~~~~~~~
 
 ``sphinx_readme`` adds support for the following ``sphinx`` and ``docutils`` directives and features:
 
 * |.`sphinx.ext.autodoc`|_ cross-references (``:mod:``, ``:class:``, ``:meth:``, ``:func:``, and ``:attr:``)
 * Standard cross-reference roles (``:doc:`` and ``:ref:``)
 * Generic and Specific Admonitions
 * Only directives
 * Toctrees
 * Rubrics
 * Images
 
 
-Installation
-~~~~~~~~~~~~~
+⚙ Installation
+~~~~~~~~~~~~~~~~
 
 Install using pip::
 
    pip install sphinx-readme
 
 
 Add the extension to your ``conf.py``:
@@ -130,48 +145,49 @@
 
    extensions = [
       'sphinx_readme',
    ]
 
 
 
-Configuration
-~~~~~~~~~~~~~~~
+🔧 Configuration
+~~~~~~~~~~~~~~~~~
 
+.. |linkcode| replace:: |.`sphinx.ext.linkcode`|_
 
 
 
 
 Please see `Extension Configuration <https://sphinx-readme.readthedocs.io/en/latest/configuration/configuring.html>`_ for full documentation on configuration variables
 
 
 Mandatory ``conf.py`` Values
 ==================================
 
 |html_context|_
- A dictionary containing info about your repository
+ A dictionary containing info about your repository (|sphinx_html_context|_)
 
   Type: ``dict``
 
  * At minimum, the username and repository name must be specified
  * Please see `HTML Context Settings <https://docs.readthedocs.io/en/stable/guides/edit-source-links-sphinx.html>`_
    to determine the correct dictionary keys for your hosting platform
 
-.. |html_context| replace:: ``html_context``
-.. _html_context: https://www.sphinx-doc.org/en/master/usage/configuration.html#confval-html_context
+.. |sphinx_html_context| replace:: ``html_context``
+.. _sphinx_html_context: https://www.sphinx-doc.org/en/master/usage/configuration.html#confval-html_context
 
 |
 
 |html_baseurl|_
- The base URL which points to the root of the HTML documentation
+ The base URL which points to the root of the HTML documentation (|sphinx_html_baseurl|_)
 
   Type: ``str``
 
-.. |html_baseurl| replace:: ``html_baseurl``
-.. _html_baseurl: https://www.sphinx-doc.org/en/master/usage/configuration.html#confval-html_baseurl
+.. |sphinx_html_baseurl| replace:: ``html_baseurl``
+.. _sphinx_html_baseurl: https://www.sphinx-doc.org/en/master/usage/configuration.html#confval-html_baseurl
 
 |
 
 |readme_src_files|_
  An individual or list of ``rst`` files to parse
 
   Type: ``Union[str, List]``
@@ -179,53 +195,45 @@
 
 .. csv-table::
    :header: |important| Important
 
    "Filepaths should be specified relative to the source directory"
 
 
-.. |readme_src_files| replace:: ``readme_src_files``
-.. _readme_src_files: https://sphinx-readme.readthedocs.io/en/latest/configuration/configuring.html#confval-readme_src_files
-
 |
 
 |readme_docs_url_type|_
  The documentation source to link to when resolving |.`~.sphinx.ext.autodoc`|_ cross-references
 
   Type: ``str``
 
  Must be either ``"code"`` or ``"html"``
 
- * ``"code"``: uses |.`sphinx.ext.linkcode`|_ to replace references with links to highlighted source code
+ * ``"code"``: uses |linkcode| to replace references with links to highlighted source code
 
-   **Example**: |.`~.parse_intersphinx_node`|_
+   **Example**: |.`~.parse_intersphinx_nodes`|_
 
 
  * ``"html"``: replaces references with links to HTML documentation entries
 
-   **Example**: |parse_intersphinx_node_html|_
+   **Example**: |parse_intersphinx_nodes_html|_
 
 
 .. csv-table::
    :header: |note| Note
 
    "If set to ``code``, then :code:`:attr:` cross-references will not be replaced with links
 
    * Instead, they'll be replaced with ``inline literals`` or left as is
    * Please see |readme_replace_attrs|_ and |readme_inline_markup|_"
 
 
-.. |readme_docs_url_type| replace:: ``readme_docs_url_type``
-.. _readme_docs_url_type: https://sphinx-readme.readthedocs.io/en/latest/configuration/configuring.html#confval-readme_docs_url_type
-.. |parse_intersphinx_node_html| replace:: ``parse_intersphinx_node()``
-.. _parse_intersphinx_node_html: http://sphinx-readme.readthedocs.io/en/latest/parser.html#sphinx_readme.parser.READMEParser.parse_intersphinx_node
-.. |readme_replace_attrs| replace:: ``readme_replace_attrs``
-.. _readme_replace_attrs: https://sphinx-readme.readthedocs.io/en/latest/configuration/configuring.html#confval-readme_replace_attrs
-.. |readme_inline_markup| replace:: ``readme_inline_markup``
-.. _readme_inline_markup: https://sphinx-readme.readthedocs.io/en/latest/configuration/configuring.html#confval-readme_inline_markup
+
+.. |parse_intersphinx_nodes_html| replace:: ``parse_intersphinx_nodes()``
+.. _parse_intersphinx_nodes_html: http://sphinx-readme.readthedocs.io/en/latest/parser.html#sphinx_readme.parser.READMEParser.parse_intersphinx_nodes
 
 
 Sample ``conf.py``
 ~~~~~~~~~~~~~~~~~~~
 
 .. code-block:: python
 
@@ -242,17 +250,14 @@
    html_baseurl = "https://sphinx-readme.readthedocs.io/en/latest"
 
    readme_src_files = "README.rst"
 
    readme_docs_url_type = "code"
 
 
-.. |readme_raw_directive| replace:: ``readme_raw_directive``
-.. _readme_raw_directive: https://sphinx-readme.readthedocs.io/en/latest/configuration/configuring.html#confval-readme_raw_directive
-
 
 
 .. csv-table::
    :header: |important| Important
 
    "For platforms that don't support the ``raw`` directive (PyPi, GitLab, and BitBucket),
    be sure to disable |readme_raw_directive|_:
@@ -260,16 +265,15 @@
    .. code-block:: python
 
       readme_raw_directive = False"
 
 
 
 
-
-Documentation
+📚 Documentation
 ~~~~~~~~~~~~~~~~
 
 Full documentation can be found on |docs|_
 
 
 .. |docs| replace:: ``ReadTheDocs``
 .. _docs: https://sphinx-readme.readthedocs.io/en/latest
```

