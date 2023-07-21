# Comparing `tmp/edx-api-doc-tools-1.6.0.tar.gz` & `tmp/edx-api-doc-tools-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edx-api-doc-tools-1.6.0.tar", last modified: Wed Feb 16 09:31:11 2022, max compression
+gzip compressed data, was "edx-api-doc-tools-1.7.0.tar", last modified: Fri Jul 21 12:22:44 2023, max compression
```

## Comparing `edx-api-doc-tools-1.6.0.tar` & `edx-api-doc-tools-1.7.0.tar`

### file list

```diff
@@ -1,26 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-16 09:31:11.191878 edx-api-doc-tools-1.6.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1837 2022-02-16 09:31:03.000000 edx-api-doc-tools-1.6.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (121)    10177 2022-02-16 09:31:03.000000 edx-api-doc-tools-1.6.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)      127 2022-02-16 09:31:03.000000 edx-api-doc-tools-1.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     6216 2022-02-16 09:31:11.191878 edx-api-doc-tools-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3610 2022-02-16 09:31:03.000000 edx-api-doc-tools-1.6.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-16 09:31:11.191878 edx-api-doc-tools-1.6.0/edx_api_doc_tools/
--rw-r--r--   0 runner    (1001) docker     (121)     1321 2022-02-16 09:31:03.000000 edx-api-doc-tools-1.6.0/edx_api_doc_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1197 2022-02-16 09:31:03.000000 edx-api-doc-tools-1.6.0/edx_api_doc_tools/apps.py
--rw-r--r--   0 runner    (1001) docker     (121)     6030 2022-02-16 09:31:03.000000 edx-api-doc-tools-1.6.0/edx_api_doc_tools/conf_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     2417 2022-02-16 09:31:03.000000 edx-api-doc-tools-1.6.0/edx_api_doc_tools/data.py
--rw-r--r--   0 runner    (1001) docker     (121)     1032 2022-02-16 09:31:03.000000 edx-api-doc-tools-1.6.0/edx_api_doc_tools/internal_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      212 2022-02-16 09:31:03.000000 edx-api-doc-tools-1.6.0/edx_api_doc_tools/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)     5993 2022-02-16 09:31:03.000000 edx-api-doc-tools-1.6.0/edx_api_doc_tools/view_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-16 09:31:11.191878 edx-api-doc-tools-1.6.0/edx_api_doc_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6216 2022-02-16 09:31:11.000000 edx-api-doc-tools-1.6.0/edx_api_doc_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      569 2022-02-16 09:31:11.000000 edx-api-doc-tools-1.6.0/edx_api_doc_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-16 09:31:11.000000 edx-api-doc-tools-1.6.0/edx_api_doc_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-16 09:31:11.000000 edx-api-doc-tools-1.6.0/edx_api_doc_tools.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       43 2022-02-16 09:31:11.000000 edx-api-doc-tools-1.6.0/edx_api_doc_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-02-16 09:31:11.000000 edx-api-doc-tools-1.6.0/edx_api_doc_tools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-16 09:31:11.191878 edx-api-doc-tools-1.6.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (121)      110 2022-02-16 09:31:03.000000 edx-api-doc-tools-1.6.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (121)      573 2022-02-16 09:31:03.000000 edx-api-doc-tools-1.6.0/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (121)      413 2022-02-16 09:31:11.191878 edx-api-doc-tools-1.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     5372 2022-02-16 09:31:03.000000 edx-api-doc-tools-1.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 12:22:44.297615 edx-api-doc-tools-1.7.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     2003 2023-07-21 12:22:34.000000 edx-api-doc-tools-1.7.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    10177 2023-07-21 12:22:34.000000 edx-api-doc-tools-1.7.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      127 2023-07-21 12:22:34.000000 edx-api-doc-tools-1.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     6393 2023-07-21 12:22:44.297615 edx-api-doc-tools-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3620 2023-07-21 12:22:34.000000 edx-api-doc-tools-1.7.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 12:22:44.297615 edx-api-doc-tools-1.7.0/edx_api_doc_tools/
+-rw-r--r--   0 runner    (1001) docker     (122)     1253 2023-07-21 12:22:34.000000 edx-api-doc-tools-1.7.0/edx_api_doc_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1197 2023-07-21 12:22:34.000000 edx-api-doc-tools-1.7.0/edx_api_doc_tools/apps.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6034 2023-07-21 12:22:34.000000 edx-api-doc-tools-1.7.0/edx_api_doc_tools/conf_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2417 2023-07-21 12:22:34.000000 edx-api-doc-tools-1.7.0/edx_api_doc_tools/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1032 2023-07-21 12:22:34.000000 edx-api-doc-tools-1.7.0/edx_api_doc_tools/internal_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      212 2023-07-21 12:22:34.000000 edx-api-doc-tools-1.7.0/edx_api_doc_tools/urls.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5993 2023-07-21 12:22:34.000000 edx-api-doc-tools-1.7.0/edx_api_doc_tools/view_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 12:22:44.297615 edx-api-doc-tools-1.7.0/edx_api_doc_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     6393 2023-07-21 12:22:44.000000 edx-api-doc-tools-1.7.0/edx_api_doc_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      615 2023-07-21 12:22:44.000000 edx-api-doc-tools-1.7.0/edx_api_doc_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-21 12:22:44.000000 edx-api-doc-tools-1.7.0/edx_api_doc_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-21 12:22:44.000000 edx-api-doc-tools-1.7.0/edx_api_doc_tools.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       43 2023-07-21 12:22:44.000000 edx-api-doc-tools-1.7.0/edx_api_doc_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-07-21 12:22:44.000000 edx-api-doc-tools-1.7.0/edx_api_doc_tools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 12:22:44.297615 edx-api-doc-tools-1.7.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      110 2023-07-21 12:22:34.000000 edx-api-doc-tools-1.7.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      573 2023-07-21 12:22:34.000000 edx-api-doc-tools-1.7.0/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      413 2023-07-21 12:22:44.297615 edx-api-doc-tools-1.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     5393 2023-07-21 12:22:34.000000 edx-api-doc-tools-1.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 12:22:44.297615 edx-api-doc-tools-1.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     6905 2023-07-21 12:22:34.000000 edx-api-doc-tools-1.7.0/tests/test_doc_tools.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2663 2023-07-21 12:22:34.000000 edx-api-doc-tools-1.7.0/tests/test_example.py
```

### Comparing `edx-api-doc-tools-1.6.0/CHANGELOG.rst` & `edx-api-doc-tools-1.7.0/CHANGELOG.rst`

 * *Files 8% similar despite different names*

```diff
@@ -10,14 +10,21 @@
    This project adheres to Semantic Versioning (http://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ----------
 
+1.7.0 --- 2023-07-23
+--------------------
+
+* Switch from ``edx-sphinx-theme`` to ``sphinx-book-theme`` since the former is
+  deprecated
+* Add support for Django 4.2
+
 1.6.0 --- 2022-02-11
 --------------------
 
 * Dropped support for django 2.2, 3.0, 3.1
 * Added support for Django 4.0
 
 1.5.0 --- 2021-07-19
```

### Comparing `edx-api-doc-tools-1.6.0/LICENSE.txt` & `edx-api-doc-tools-1.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edx-api-doc-tools-1.6.0/PKG-INFO` & `edx-api-doc-tools-1.7.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: edx-api-doc-tools
-Version: 1.6.0
+Version: 1.7.0
 Summary: Tools for writing and generating API documentation for edX REST APIs
-Home-page: https://github.com/edx/api-doc-tools
-Author: edX
-Author-email: oscm@edx.org
+Home-page: https://github.com/openedx/api-doc-tools
+Author: Open edX Project
+Author-email: oscm@openedx.org
 License: Apache Software License 2.0
 Keywords: Django edx
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
@@ -71,15 +70,15 @@
 How To Contribute
 -----------------
 
 Contributions are very welcome.  Please read `How To Contribute`__ for details.
 Even though they were written with `edx-platform` in mind, the guidelines
 should be followed for all Open edX projects.
 
-__ https://github.com/edx/edx-platform/blob/master/CONTRIBUTING.rst
+__ https://github.com/openedx/.github/blob/master/CONTRIBUTING.md
 
 The pull request description template should be automatically applied if you
 are creating a pull request from GitHub. Otherwise you can find it at
 `PULL_REQUEST_TEMPLATE.md`_.
 
 The issue report template should be automatically applied if you are creating
 an issue on GitHub as well. Otherwise you can find it at `ISSUE_TEMPLATE.md`_.
@@ -98,28 +97,28 @@
 Have a question about this repository, or about the Open edX project in general?  Please refer to this `list of resources <https://open.edx.org/getting-help>`_ if you need any assistance.
 
 
 
 .. |pypi| image:: https://img.shields.io/pypi/v/edx-api-doc-tools.svg
     :target: https://pypi.python.org/pypi/edx-api-doc-tools/
     :alt: PyPI
-.. |CI| image:: https://github.com/edx/api-doc-tools/workflows/Python%20CI/badge.svg?branch=master
-    :target: https://github.com/edx/api-doc-tools/actions?query=workflow%3A%22Python+CI%22
+.. |CI| image:: https://github.com/openedx/api-doc-tools/workflows/Python%20CI/badge.svg?branch=master
+    :target: https://github.com/openedx/api-doc-tools/actions?query=workflow%3A%22Python+CI%22
     :alt: CI
 .. |codecov| image:: http://codecov.io/github/edx/api-doc-tools/coverage.svg?branch=master
     :target: http://codecov.io/github/edx/api-doc-tools?branch=master
     :alt: Codecov
 .. |readthedocs| image:: https://readthedocs.org/projects/edx-api-doc-tools/badge/?version=latest
     :target: http://edx-api-doc-tools.readthedocs.io/en/latest/
     :alt: Documentation
 .. |pyversions| image:: https://img.shields.io/pypi/pyversions/edx-api-doc-tools.svg
     :target: https://pypi.python.org/pypi/edx-api-doc-tools/
     :alt: Supported
 .. |license| image:: https://img.shields.io/github/license/edx/api-doc-tools.svg
-    :target: https://github.com/edx/api-doc-tools/blob/master/LICENSE.txt
+    :target: https://github.com/openedx/api-doc-tools/blob/master/LICENSE.txt
     :alt: License
 
 
 Change Log
 ==========
 
 ..
@@ -131,14 +130,21 @@
    This project adheres to Semantic Versioning (http://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ----------
 
+1.7.0 --- 2023-07-23
+--------------------
+
+* Switch from ``edx-sphinx-theme`` to ``sphinx-book-theme`` since the former is
+  deprecated
+* Add support for Django 4.2
+
 1.6.0 --- 2022-02-11
 --------------------
 
 * Dropped support for django 2.2, 3.0, 3.1
 * Added support for Django 4.0
 
 1.5.0 --- 2021-07-19
@@ -203,9 +209,7 @@
 * Added documentation.
 
 
 1.0.2 --- 2020-01-17
 --------------------
 
 * First release on PyPI.
-
-
```

### Comparing `edx-api-doc-tools-1.6.0/README.rst` & `edx-api-doc-tools-1.7.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 How To Contribute
 -----------------
 
 Contributions are very welcome.  Please read `How To Contribute`__ for details.
 Even though they were written with `edx-platform` in mind, the guidelines
 should be followed for all Open edX projects.
 
-__ https://github.com/edx/edx-platform/blob/master/CONTRIBUTING.rst
+__ https://github.com/openedx/.github/blob/master/CONTRIBUTING.md
 
 The pull request description template should be automatically applied if you
 are creating a pull request from GitHub. Otherwise you can find it at
 `PULL_REQUEST_TEMPLATE.md`_.
 
 The issue report template should be automatically applied if you are creating
 an issue on GitHub as well. Otherwise you can find it at `ISSUE_TEMPLATE.md`_.
@@ -76,22 +76,22 @@
 Have a question about this repository, or about the Open edX project in general?  Please refer to this `list of resources <https://open.edx.org/getting-help>`_ if you need any assistance.
 
 
 
 .. |pypi| image:: https://img.shields.io/pypi/v/edx-api-doc-tools.svg
     :target: https://pypi.python.org/pypi/edx-api-doc-tools/
     :alt: PyPI
-.. |CI| image:: https://github.com/edx/api-doc-tools/workflows/Python%20CI/badge.svg?branch=master
-    :target: https://github.com/edx/api-doc-tools/actions?query=workflow%3A%22Python+CI%22
+.. |CI| image:: https://github.com/openedx/api-doc-tools/workflows/Python%20CI/badge.svg?branch=master
+    :target: https://github.com/openedx/api-doc-tools/actions?query=workflow%3A%22Python+CI%22
     :alt: CI
 .. |codecov| image:: http://codecov.io/github/edx/api-doc-tools/coverage.svg?branch=master
     :target: http://codecov.io/github/edx/api-doc-tools?branch=master
     :alt: Codecov
 .. |readthedocs| image:: https://readthedocs.org/projects/edx-api-doc-tools/badge/?version=latest
     :target: http://edx-api-doc-tools.readthedocs.io/en/latest/
     :alt: Documentation
 .. |pyversions| image:: https://img.shields.io/pypi/pyversions/edx-api-doc-tools.svg
     :target: https://pypi.python.org/pypi/edx-api-doc-tools/
     :alt: Supported
 .. |license| image:: https://img.shields.io/github/license/edx/api-doc-tools.svg
-    :target: https://github.com/edx/api-doc-tools/blob/master/LICENSE.txt
+    :target: https://github.com/openedx/api-doc-tools/blob/master/LICENSE.txt
     :alt: License
```

### Comparing `edx-api-doc-tools-1.6.0/edx_api_doc_tools/__init__.py` & `edx-api-doc-tools-1.7.0/edx_api_doc_tools/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -42,10 +42,8 @@
     exclude_schema_for_all,
     is_schema_request,
     schema,
     schema_for,
 )
 
 
-__version__ = '1.6.0'
-
-default_app_config = 'edx_api_doc_tools.apps.EdxApiDocToolsConfig'
+__version__ = '1.7.0'
```

### Comparing `edx-api-doc-tools-1.6.0/edx_api_doc_tools/apps.py` & `edx-api-doc-tools-1.7.0/edx_api_doc_tools/apps.py`

 * *Files identical despite different names*

### Comparing `edx-api-doc-tools-1.6.0/edx_api_doc_tools/conf_utils.py` & `edx-api-doc-tools-1.7.0/edx_api_doc_tools/conf_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         docs_ui_view=make_docs_ui_view(api_info, api_url_patterns),
     )
 
 
 def make_api_info(
         title="Open edX APIs",
         version="v1",
-        email="oscm@edx.org",
+        email="oscm@openedx.org",
         description="APIs for access to Open edX information",
 ):
     """
     Build an API info object.
 
     Arguments:
         title (str): The title of the API.
```

### Comparing `edx-api-doc-tools-1.6.0/edx_api_doc_tools/data.py` & `edx-api-doc-tools-1.7.0/edx_api_doc_tools/data.py`

 * *Files identical despite different names*

### Comparing `edx-api-doc-tools-1.6.0/edx_api_doc_tools/internal_utils.py` & `edx-api-doc-tools-1.7.0/edx_api_doc_tools/internal_utils.py`

 * *Files identical despite different names*

### Comparing `edx-api-doc-tools-1.6.0/edx_api_doc_tools/view_utils.py` & `edx-api-doc-tools-1.7.0/edx_api_doc_tools/view_utils.py`

 * *Files identical despite different names*

### Comparing `edx-api-doc-tools-1.6.0/edx_api_doc_tools.egg-info/PKG-INFO` & `edx-api-doc-tools-1.7.0/edx_api_doc_tools.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: edx-api-doc-tools
-Version: 1.6.0
+Version: 1.7.0
 Summary: Tools for writing and generating API documentation for edX REST APIs
-Home-page: https://github.com/edx/api-doc-tools
-Author: edX
-Author-email: oscm@edx.org
+Home-page: https://github.com/openedx/api-doc-tools
+Author: Open edX Project
+Author-email: oscm@openedx.org
 License: Apache Software License 2.0
 Keywords: Django edx
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
@@ -71,15 +70,15 @@
 How To Contribute
 -----------------
 
 Contributions are very welcome.  Please read `How To Contribute`__ for details.
 Even though they were written with `edx-platform` in mind, the guidelines
 should be followed for all Open edX projects.
 
-__ https://github.com/edx/edx-platform/blob/master/CONTRIBUTING.rst
+__ https://github.com/openedx/.github/blob/master/CONTRIBUTING.md
 
 The pull request description template should be automatically applied if you
 are creating a pull request from GitHub. Otherwise you can find it at
 `PULL_REQUEST_TEMPLATE.md`_.
 
 The issue report template should be automatically applied if you are creating
 an issue on GitHub as well. Otherwise you can find it at `ISSUE_TEMPLATE.md`_.
@@ -98,28 +97,28 @@
 Have a question about this repository, or about the Open edX project in general?  Please refer to this `list of resources <https://open.edx.org/getting-help>`_ if you need any assistance.
 
 
 
 .. |pypi| image:: https://img.shields.io/pypi/v/edx-api-doc-tools.svg
     :target: https://pypi.python.org/pypi/edx-api-doc-tools/
     :alt: PyPI
-.. |CI| image:: https://github.com/edx/api-doc-tools/workflows/Python%20CI/badge.svg?branch=master
-    :target: https://github.com/edx/api-doc-tools/actions?query=workflow%3A%22Python+CI%22
+.. |CI| image:: https://github.com/openedx/api-doc-tools/workflows/Python%20CI/badge.svg?branch=master
+    :target: https://github.com/openedx/api-doc-tools/actions?query=workflow%3A%22Python+CI%22
     :alt: CI
 .. |codecov| image:: http://codecov.io/github/edx/api-doc-tools/coverage.svg?branch=master
     :target: http://codecov.io/github/edx/api-doc-tools?branch=master
     :alt: Codecov
 .. |readthedocs| image:: https://readthedocs.org/projects/edx-api-doc-tools/badge/?version=latest
     :target: http://edx-api-doc-tools.readthedocs.io/en/latest/
     :alt: Documentation
 .. |pyversions| image:: https://img.shields.io/pypi/pyversions/edx-api-doc-tools.svg
     :target: https://pypi.python.org/pypi/edx-api-doc-tools/
     :alt: Supported
 .. |license| image:: https://img.shields.io/github/license/edx/api-doc-tools.svg
-    :target: https://github.com/edx/api-doc-tools/blob/master/LICENSE.txt
+    :target: https://github.com/openedx/api-doc-tools/blob/master/LICENSE.txt
     :alt: License
 
 
 Change Log
 ==========
 
 ..
@@ -131,14 +130,21 @@
    This project adheres to Semantic Versioning (http://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ----------
 
+1.7.0 --- 2023-07-23
+--------------------
+
+* Switch from ``edx-sphinx-theme`` to ``sphinx-book-theme`` since the former is
+  deprecated
+* Add support for Django 4.2
+
 1.6.0 --- 2022-02-11
 --------------------
 
 * Dropped support for django 2.2, 3.0, 3.1
 * Added support for Django 4.0
 
 1.5.0 --- 2021-07-19
@@ -203,9 +209,7 @@
 * Added documentation.
 
 
 1.0.2 --- 2020-01-17
 --------------------
 
 * First release on PyPI.
-
-
```

### Comparing `edx-api-doc-tools-1.6.0/edx_api_doc_tools.egg-info/SOURCES.txt` & `edx-api-doc-tools-1.7.0/edx_api_doc_tools.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -14,8 +14,10 @@
 edx_api_doc_tools.egg-info/PKG-INFO
 edx_api_doc_tools.egg-info/SOURCES.txt
 edx_api_doc_tools.egg-info/dependency_links.txt
 edx_api_doc_tools.egg-info/not-zip-safe
 edx_api_doc_tools.egg-info/requires.txt
 edx_api_doc_tools.egg-info/top_level.txt
 requirements/base.in
-requirements/constraints.txt
+requirements/constraints.txt
+tests/test_doc_tools.py
+tests/test_example.py
```

### Comparing `edx-api-doc-tools-1.6.0/requirements/constraints.txt` & `edx-api-doc-tools-1.7.0/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `edx-api-doc-tools-1.6.0/setup.py` & `edx-api-doc-tools-1.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,30 +106,30 @@
 
 setup(
     name='edx-api-doc-tools',
     version=VERSION,
     description="Tools for writing and generating API documentation for edX REST APIs",
     long_description=README + '\n\n' + CHANGELOG,
     long_description_content_type="text/x-rst",
-    author='edX',
-    author_email='oscm@edx.org',
-    url='https://github.com/edx/api-doc-tools',
+    author='Open edX Project',
+    author_email='oscm@openedx.org',
+    url='https://github.com/openedx/api-doc-tools',
     packages=[
         'edx_api_doc_tools',
     ],
     include_package_data=True,
     install_requires=load_requirements('requirements/base.in'),
     license="Apache Software License 2.0",
     zip_safe=False,
     keywords='Django edx',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Framework :: Django',
         'Framework :: Django :: 3.2',
-        'Framework :: Django :: 4.0',
+        'Framework :: Django :: 4.2',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: Apache Software License',
         'Natural Language :: English',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.8',
     ],
 )
```

