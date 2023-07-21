# Comparing `tmp/code-annotations-1.3.0.tar.gz` & `tmp/code-annotations-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "code-annotations-1.3.0.tar", last modified: Mon Feb  7 12:35:59 2022, max compression
+gzip compressed data, was "code-annotations-1.5.0.tar", last modified: Fri Jul 21 13:15:03 2023, max compression
```

## Comparing `code-annotations-1.3.0.tar` & `code-annotations-1.5.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 12:35:59.245694 code-annotations-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (121)     3876 2022-02-07 12:35:54.000000 code-annotations-1.3.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (121)    11358 2022-02-07 12:35:54.000000 code-annotations-1.3.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)      228 2022-02-07 12:35:54.000000 code-annotations-1.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      545 2022-02-07 12:35:54.000000 code-annotations-1.3.0/NOTICE.txt
--rw-r--r--   0 runner    (1001) docker     (121)     7935 2022-02-07 12:35:59.245694 code-annotations-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3254 2022-02-07 12:35:54.000000 code-annotations-1.3.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 12:35:59.241694 code-annotations-1.3.0/code_annotations/
--rw-r--r--   0 runner    (1001) docker     (121)       86 2022-02-07 12:35:54.000000 code-annotations-1.3.0/code_annotations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2313 2022-02-07 12:35:54.000000 code-annotations-1.3.0/code_annotations/annotation_errors.py
--rw-r--r--   0 runner    (1001) docker     (121)    23608 2022-02-07 12:35:54.000000 code-annotations-1.3.0/code_annotations/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     7923 2022-02-07 12:35:54.000000 code-annotations-1.3.0/code_annotations/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 12:35:59.241694 code-annotations-1.3.0/code_annotations/contrib/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 12:35:59.245694 code-annotations-1.3.0/code_annotations/contrib/config/
--rw-r--r--   0 runner    (1001) docker     (121)      468 2022-02-07 12:35:54.000000 code-annotations-1.3.0/code_annotations/contrib/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      984 2022-02-07 12:35:54.000000 code-annotations-1.3.0/code_annotations/contrib/config/feature_toggle_annotations.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      279 2022-02-07 12:35:54.000000 code-annotations-1.3.0/code_annotations/contrib/config/setting_annotations.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 12:35:59.241694 code-annotations-1.3.0/code_annotations/contrib/sphinx/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 12:35:59.245694 code-annotations-1.3.0/code_annotations/contrib/sphinx/extensions/
--rw-r--r--   0 runner    (1001) docker     (121)       93 2022-02-07 12:35:54.000000 code-annotations-1.3.0/code_annotations/contrib/sphinx/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1562 2022-02-07 12:35:54.000000 code-annotations-1.3.0/code_annotations/contrib/sphinx/extensions/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     4001 2022-02-07 12:35:54.000000 code-annotations-1.3.0/code_annotations/contrib/sphinx/extensions/featuretoggles.py
--rw-r--r--   0 runner    (1001) docker     (121)     4436 2022-02-07 12:35:54.000000 code-annotations-1.3.0/code_annotations/contrib/sphinx/extensions/settings.py
--rw-r--r--   0 runner    (1001) docker     (121)      173 2022-02-07 12:35:54.000000 code-annotations-1.3.0/code_annotations/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 12:35:59.245694 code-annotations-1.3.0/code_annotations/extensions/
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-02-07 12:35:54.000000 code-annotations-1.3.0/code_annotations/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6629 2022-02-07 12:35:54.000000 code-annotations-1.3.0/code_annotations/extensions/base.py
--rw-r--r--   0 runner    (1001) docker     (121)      495 2022-02-07 12:35:54.000000 code-annotations-1.3.0/code_annotations/extensions/javascript.py
--rw-r--r--   0 runner    (1001) docker     (121)      480 2022-02-07 12:35:54.000000 code-annotations-1.3.0/code_annotations/extensions/python.py
--rw-r--r--   0 runner    (1001) docker     (121)    16689 2022-02-07 12:35:54.000000 code-annotations-1.3.0/code_annotations/find_django.py
--rw-r--r--   0 runner    (1001) docker     (121)     3689 2022-02-07 12:35:54.000000 code-annotations-1.3.0/code_annotations/find_static.py
--rw-r--r--   0 runner    (1001) docker     (121)     5535 2022-02-07 12:35:54.000000 code-annotations-1.3.0/code_annotations/generate_docs.py
--rw-r--r--   0 runner    (1001) docker     (121)     5687 2022-02-07 12:35:54.000000 code-annotations-1.3.0/code_annotations/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 12:35:59.245694 code-annotations-1.3.0/code_annotations.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7935 2022-02-07 12:35:59.000000 code-annotations-1.3.0/code_annotations.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1196 2022-02-07 12:35:59.000000 code-annotations-1.3.0/code_annotations.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-07 12:35:59.000000 code-annotations-1.3.0/code_annotations.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      254 2022-02-07 12:35:59.000000 code-annotations-1.3.0/code_annotations.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-07 12:35:59.000000 code-annotations-1.3.0/code_annotations.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       72 2022-02-07 12:35:59.000000 code-annotations-1.3.0/code_annotations.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-02-07 12:35:59.000000 code-annotations-1.3.0/code_annotations.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 12:35:59.245694 code-annotations-1.3.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (121)      113 2022-02-07 12:35:54.000000 code-annotations-1.3.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (121)      163 2022-02-07 12:35:59.245694 code-annotations-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     3266 2022-02-07 12:35:54.000000 code-annotations-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 13:15:03.524608 code-annotations-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     4226 2023-07-21 13:14:59.000000 code-annotations-1.5.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    11358 2023-07-21 13:14:59.000000 code-annotations-1.5.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      228 2023-07-21 13:14:59.000000 code-annotations-1.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      545 2023-07-21 13:14:59.000000 code-annotations-1.5.0/NOTICE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     8218 2023-07-21 13:15:03.524608 code-annotations-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3146 2023-07-21 13:14:59.000000 code-annotations-1.5.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 13:15:03.524608 code-annotations-1.5.0/code_annotations/
+-rw-r--r--   0 runner    (1001) docker     (122)       86 2023-07-21 13:14:59.000000 code-annotations-1.5.0/code_annotations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2313 2023-07-21 13:14:59.000000 code-annotations-1.5.0/code_annotations/annotation_errors.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23608 2023-07-21 13:14:59.000000 code-annotations-1.5.0/code_annotations/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7923 2023-07-21 13:14:59.000000 code-annotations-1.5.0/code_annotations/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 13:15:03.520608 code-annotations-1.5.0/code_annotations/contrib/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 13:15:03.524608 code-annotations-1.5.0/code_annotations/contrib/config/
+-rw-r--r--   0 runner    (1001) docker     (122)      468 2023-07-21 13:14:59.000000 code-annotations-1.5.0/code_annotations/contrib/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      983 2023-07-21 13:14:59.000000 code-annotations-1.5.0/code_annotations/contrib/config/feature_toggle_annotations.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      279 2023-07-21 13:14:59.000000 code-annotations-1.5.0/code_annotations/contrib/config/setting_annotations.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 13:15:03.520608 code-annotations-1.5.0/code_annotations/contrib/sphinx/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 13:15:03.524608 code-annotations-1.5.0/code_annotations/contrib/sphinx/extensions/
+-rw-r--r--   0 runner    (1001) docker     (122)       93 2023-07-21 13:14:59.000000 code-annotations-1.5.0/code_annotations/contrib/sphinx/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1562 2023-07-21 13:14:59.000000 code-annotations-1.5.0/code_annotations/contrib/sphinx/extensions/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4773 2023-07-21 13:14:59.000000 code-annotations-1.5.0/code_annotations/contrib/sphinx/extensions/featuretoggles.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4764 2023-07-21 13:14:59.000000 code-annotations-1.5.0/code_annotations/contrib/sphinx/extensions/settings.py
+-rw-r--r--   0 runner    (1001) docker     (122)      173 2023-07-21 13:14:59.000000 code-annotations-1.5.0/code_annotations/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 13:15:03.524608 code-annotations-1.5.0/code_annotations/extensions/
+-rw-r--r--   0 runner    (1001) docker     (122)       60 2023-07-21 13:14:59.000000 code-annotations-1.5.0/code_annotations/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6629 2023-07-21 13:14:59.000000 code-annotations-1.5.0/code_annotations/extensions/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)      495 2023-07-21 13:14:59.000000 code-annotations-1.5.0/code_annotations/extensions/javascript.py
+-rw-r--r--   0 runner    (1001) docker     (122)      480 2023-07-21 13:14:59.000000 code-annotations-1.5.0/code_annotations/extensions/python.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16689 2023-07-21 13:14:59.000000 code-annotations-1.5.0/code_annotations/find_django.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3689 2023-07-21 13:14:59.000000 code-annotations-1.5.0/code_annotations/find_static.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5535 2023-07-21 13:14:59.000000 code-annotations-1.5.0/code_annotations/generate_docs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5687 2023-07-21 13:14:59.000000 code-annotations-1.5.0/code_annotations/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 13:15:03.524608 code-annotations-1.5.0/code_annotations.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     8218 2023-07-21 13:15:03.000000 code-annotations-1.5.0/code_annotations.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1196 2023-07-21 13:15:03.000000 code-annotations-1.5.0/code_annotations.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-21 13:15:03.000000 code-annotations-1.5.0/code_annotations.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      254 2023-07-21 13:15:03.000000 code-annotations-1.5.0/code_annotations.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-21 13:15:03.000000 code-annotations-1.5.0/code_annotations.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       72 2023-07-21 13:15:03.000000 code-annotations-1.5.0/code_annotations.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       17 2023-07-21 13:15:03.000000 code-annotations-1.5.0/code_annotations.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 13:15:03.524608 code-annotations-1.5.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      113 2023-07-21 13:14:59.000000 code-annotations-1.5.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      163 2023-07-21 13:15:03.528608 code-annotations-1.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     3318 2023-07-21 13:14:59.000000 code-annotations-1.5.0/setup.py
```

### Comparing `code-annotations-1.3.0/CHANGELOG.rst` & `code-annotations-1.5.0/CHANGELOG.rst`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,27 @@
    This project adheres to Semantic Versioning (http://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
+
+[1.5.0] - 2023-07-21
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+* Switch from ``edx-sphinx-theme`` to ``sphinx-book-theme`` since the former is
+  deprecated
+* Added Support for Django 4.2
+
+[1.4.0] - 2022-05-23
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+* Rename toggle_warnings to toggle_warning for consistency with setting_warning.
+
 [1.3.0] - 2022-02-07
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 * Dropped Django 22, 30 and 31 Support
 * Added Django40 Support in CI
 
 [1.2.0] - 2021-07-26
```

### Comparing `code-annotations-1.3.0/LICENSE.txt` & `code-annotations-1.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `code-annotations-1.3.0/NOTICE.txt` & `code-annotations-1.5.0/NOTICE.txt`

 * *Files identical despite different names*

### Comparing `code-annotations-1.3.0/PKG-INFO` & `code-annotations-1.5.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: code-annotations
-Version: 1.3.0
+Version: 1.5.0
 Summary: Extensible tools for parsing annotations in codebases
-Home-page: https://github.com/edx/code-annotations
+Home-page: https://github.com/openedx/code-annotations
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: edx pii code annotations
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
+Description-Content-Type: text/x-rst
 Provides-Extra: django
 License-File: LICENSE.txt
 License-File: NOTICE.txt
 
 code-annotations
 =============================
 
@@ -55,24 +56,21 @@
 Please see ``LICENSE.txt`` for details.
 
 How To Contribute
 -----------------
 
 Contributions are very welcome.
 
-Please read `How To Contribute <https://github.com/edx/edx-platform/blob/master/CONTRIBUTING.rst>`_ for details.
-
-Even though they were written with ``edx-platform`` in mind, the guidelines
-should be followed for Open edX code in general.
+Please read `How To Contribute <https://github.com/openedx/.github/blob/master/CONTRIBUTING.md>`_ for details.
 
 PR description template should be automatically applied if you are sending PR from github interface; otherwise you
-can find it it at `PULL_REQUEST_TEMPLATE.md <https://github.com/edx/code-annotations/blob/master/.github/PULL_REQUEST_TEMPLATE.md>`_
+can find it it at `PULL_REQUEST_TEMPLATE.md <https://github.com/openedx/code-annotations/blob/master/.github/PULL_REQUEST_TEMPLATE.md>`_
 
 Issue report template should be automatically applied if you are sending it from github UI as well; otherwise you
-can find it at `ISSUE_TEMPLATE.md <https://github.com/edx/code-annotations/blob/master/.github/ISSUE_TEMPLATE.md>`_
+can find it at `ISSUE_TEMPLATE.md <https://github.com/openedx/code-annotations/blob/master/.github/ISSUE_TEMPLATE.md>`_
 
 Reporting Security Issues
 -------------------------
 
 Please do not report security issues in public. Please email security@edx.org.
 
 Getting Help
@@ -84,16 +82,16 @@
 .. _list of resources: https://open.edx.org/getting-help
 
 
 .. |pypi-badge| image:: https://img.shields.io/pypi/v/code-annotations.svg
     :target: https://pypi.python.org/pypi/code-annotations/
     :alt: PyPI
 
-.. |CI| image:: https://github.com/edx/code-annotations/workflows/Python%20CI/badge.svg?branch=master
-    :target: https://github.com/edx/code-annotations/actions?query=workflow%3A%22Python+CI%22
+.. |CI| image:: https://github.com/openedx/code-annotations/workflows/Python%20CI/badge.svg?branch=master
+    :target: https://github.com/openedx/code-annotations/actions?query=workflow%3A%22Python+CI%22
     :alt: CI
 
 .. |codecov-badge| image:: http://codecov.io/github/edx/code-annotations/coverage.svg?branch=master
     :target: http://codecov.io/github/edx/code-annotations?branch=master
     :alt: Codecov
 
 .. |doc-badge| image:: https://readthedocs.org/projects/code-annotations/badge/?version=latest
@@ -101,15 +99,15 @@
     :alt: Documentation
 
 .. |pyversions-badge| image:: https://img.shields.io/pypi/pyversions/code-annotations.svg
     :target: https://pypi.python.org/pypi/code-annotations/
     :alt: Supported Python versions
 
 .. |license-badge| image:: https://img.shields.io/github/license/edx/code-annotations.svg
-    :target: https://github.com/edx/code-annotations/blob/master/LICENSE.txt
+    :target: https://github.com/openedx/code-annotations/blob/master/LICENSE.txt
     :alt: License
 
 
 Change Log
 ----------
 
 ..
@@ -121,14 +119,27 @@
    This project adheres to Semantic Versioning (http://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
+
+[1.5.0] - 2023-07-21
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+* Switch from ``edx-sphinx-theme`` to ``sphinx-book-theme`` since the former is
+  deprecated
+* Added Support for Django 4.2
+
+[1.4.0] - 2022-05-23
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+* Rename toggle_warnings to toggle_warning for consistency with setting_warning.
+
 [1.3.0] - 2022-02-07
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 * Dropped Django 22, 30 and 31 Support
 * Added Django40 Support in CI
 
 [1.2.0] - 2021-07-26
```

### Comparing `code-annotations-1.3.0/README.rst` & `code-annotations-1.5.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -31,24 +31,21 @@
 Please see ``LICENSE.txt`` for details.
 
 How To Contribute
 -----------------
 
 Contributions are very welcome.
 
-Please read `How To Contribute <https://github.com/edx/edx-platform/blob/master/CONTRIBUTING.rst>`_ for details.
-
-Even though they were written with ``edx-platform`` in mind, the guidelines
-should be followed for Open edX code in general.
+Please read `How To Contribute <https://github.com/openedx/.github/blob/master/CONTRIBUTING.md>`_ for details.
 
 PR description template should be automatically applied if you are sending PR from github interface; otherwise you
-can find it it at `PULL_REQUEST_TEMPLATE.md <https://github.com/edx/code-annotations/blob/master/.github/PULL_REQUEST_TEMPLATE.md>`_
+can find it it at `PULL_REQUEST_TEMPLATE.md <https://github.com/openedx/code-annotations/blob/master/.github/PULL_REQUEST_TEMPLATE.md>`_
 
 Issue report template should be automatically applied if you are sending it from github UI as well; otherwise you
-can find it at `ISSUE_TEMPLATE.md <https://github.com/edx/code-annotations/blob/master/.github/ISSUE_TEMPLATE.md>`_
+can find it at `ISSUE_TEMPLATE.md <https://github.com/openedx/code-annotations/blob/master/.github/ISSUE_TEMPLATE.md>`_
 
 Reporting Security Issues
 -------------------------
 
 Please do not report security issues in public. Please email security@edx.org.
 
 Getting Help
@@ -60,16 +57,16 @@
 .. _list of resources: https://open.edx.org/getting-help
 
 
 .. |pypi-badge| image:: https://img.shields.io/pypi/v/code-annotations.svg
     :target: https://pypi.python.org/pypi/code-annotations/
     :alt: PyPI
 
-.. |CI| image:: https://github.com/edx/code-annotations/workflows/Python%20CI/badge.svg?branch=master
-    :target: https://github.com/edx/code-annotations/actions?query=workflow%3A%22Python+CI%22
+.. |CI| image:: https://github.com/openedx/code-annotations/workflows/Python%20CI/badge.svg?branch=master
+    :target: https://github.com/openedx/code-annotations/actions?query=workflow%3A%22Python+CI%22
     :alt: CI
 
 .. |codecov-badge| image:: http://codecov.io/github/edx/code-annotations/coverage.svg?branch=master
     :target: http://codecov.io/github/edx/code-annotations?branch=master
     :alt: Codecov
 
 .. |doc-badge| image:: https://readthedocs.org/projects/code-annotations/badge/?version=latest
@@ -77,9 +74,9 @@
     :alt: Documentation
 
 .. |pyversions-badge| image:: https://img.shields.io/pypi/pyversions/code-annotations.svg
     :target: https://pypi.python.org/pypi/code-annotations/
     :alt: Supported Python versions
 
 .. |license-badge| image:: https://img.shields.io/github/license/edx/code-annotations.svg
-    :target: https://github.com/edx/code-annotations/blob/master/LICENSE.txt
+    :target: https://github.com/openedx/code-annotations/blob/master/LICENSE.txt
     :alt: License
```

### Comparing `code-annotations-1.3.0/code_annotations/annotation_errors.py` & `code-annotations-1.5.0/code_annotations/annotation_errors.py`

 * *Files identical despite different names*

### Comparing `code-annotations-1.3.0/code_annotations/base.py` & `code-annotations-1.5.0/code_annotations/base.py`

 * *Files identical despite different names*

### Comparing `code-annotations-1.3.0/code_annotations/cli.py` & `code-annotations-1.5.0/code_annotations/cli.py`

 * *Files identical despite different names*

### Comparing `code-annotations-1.3.0/code_annotations/contrib/config/feature_toggle_annotations.yaml` & `code-annotations-1.5.0/code_annotations/contrib/config/feature_toggle_annotations.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     - ".. toggle_default:":
     - ".. toggle_description:":
     - ".. toggle_use_cases:":
         choices: [temporary, circuit_breaker, vip, opt_out, opt_in, open_edx]
     - ".. toggle_creation_date:":
     - ".. toggle_target_removal_date:":
         optional: true
-    - ".. toggle_warnings:":
+    - ".. toggle_warning:":
         optional: true
     - ".. toggle_tickets:":
         optional: true
 extensions:
     python:
         - py
 rst_template: doc.rst.j2
```

### Comparing `code-annotations-1.3.0/code_annotations/contrib/sphinx/extensions/base.py` & `code-annotations-1.5.0/code_annotations/contrib/sphinx/extensions/base.py`

 * *Files identical despite different names*

### Comparing `code-annotations-1.3.0/code_annotations/contrib/sphinx/extensions/featuretoggles.py` & `code-annotations-1.5.0/code_annotations/contrib/sphinx/extensions/featuretoggles.py`

 * *Files 21% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
     - ``featuretoggles_source_path``: absolute path to the repository file tree. E.g:
 
         featuretoggles_source_path = os.path.join(os.path.dirname(__file__), "..", "..")
 
     - ``featuretoggles_repo_url``: Github repository where the code is hosted. E.g:
 
-        featuretoggles_repo_url = "https://github.com/edx/myrepo"
+        featuretoggles_repo_url = "https://github.com/openedx/myrepo"
 
     - ``featuretoggles_repo_version``: current version of the git repository. E.g:
 
         import git
         try:
             repo = git.Repo(search_parent_directories=True)
             featuretoggles_repo_version = repo.head.object.hexsha
@@ -70,38 +70,54 @@
         """
         toggles = find_feature_toggles(self.env.config.featuretoggles_source_path)
         for toggle_name in sorted(toggles):
             toggle = toggles[toggle_name]
             toggle_default_value = toggle.get(".. toggle_default:", "Not defined")
             toggle_default_node = nodes.literal(text=quote_value(toggle_default_value))
             toggle_section = nodes.section("", ids=[f"featuretoggle-{toggle_name}"])
-            toggle_section += nodes.title(text=toggle_name)
-            toggle_section += nodes.paragraph("", "Default: ", toggle_default_node)
+            toggle_section += nodes.title(text=toggle_name, ids=[f"name-{toggle_name}"])
+            toggle_section += nodes.paragraph(
+                "", "Default: ", toggle_default_node, ids=[f"default-{toggle_name}"]
+            )
             toggle_section += nodes.paragraph(
                 "",
                 "Source: ",
                 nodes.reference(
                     text="{} (line {})".format(
                         toggle["filename"], toggle["line_number"]
                     ),
                     refuri="{}/blob/{}/{}#L{}".format(
                         self.env.config.featuretoggles_repo_url,
                         self.env.config.featuretoggles_repo_version,
                         toggle["filename"],
                         toggle["line_number"],
                     ),
                 ),
+                ids=[f"source-{toggle_name}"],
             )
             toggle_section += nodes.paragraph(
-                text=toggle.get(".. toggle_description:", "")
+                text=f'Desc: {toggle.get(".. toggle_description:", "NaN")}',
+                ids=[f"description-{toggle_name}"],
             )
-            if toggle.get(".. toggle_warnings:") not in (None, "None", "n/a", "N/A"):
+            if toggle.get(".. toggle_warning:") not in (None, "None", "n/a", "N/A"):
                 toggle_section += nodes.warning(
-                    "", nodes.paragraph("", toggle[".. toggle_warnings:"])
+                    "", nodes.paragraph("", toggle[".. toggle_warning:"]), ids=[f"warning-{toggle_name}"]
                 )
+            optional_attrs = [
+                "creation_date",
+                "target_removal_date",
+                "implementation",
+                "use_cases",
+            ]
+            for opt in optional_attrs:
+                if toggle.get(f".. toggle_{opt}:") not in (None, "None", "n/a", "N/A"):
+                    toggle_section += nodes.paragraph(
+                        text=f'{opt.title().replace("_"," ")}: {toggle[f".. toggle_{opt}:"]}',
+                        ids=[f"{opt}-{toggle_name}"],
+                    )
             yield toggle_section
 
 
 def setup(app):
     """
     Declare the Sphinx extension.
     """
```

### Comparing `code-annotations-1.3.0/code_annotations/contrib/sphinx/extensions/settings.py` & `code-annotations-1.5.0/code_annotations/contrib/sphinx/extensions/settings.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,15 +15,17 @@
 def find_settings(source_path):
     """
     Find the Django settings as defined in the configuration file.
 
     Return:
         settings (dict): Django settings indexed by name.
     """
-    return find_annotations(source_path, SETTING_ANNOTATIONS_CONFIG_PATH, ".. setting_name:")
+    return find_annotations(
+        source_path, SETTING_ANNOTATIONS_CONFIG_PATH, ".. setting_name:"
+    )
 
 
 class Settings(SphinxDirective):
     """
     Sphinx directive to document Django settings in a single documentation page.
 
     Use this directive as follows::
@@ -35,15 +37,15 @@
 
     - ``settings_source_path``: absolute path to the repository file tree. E.g:
 
         settings_source_path = os.path.join(os.path.dirname(__file__), "..", "..")
 
     - ``settings_repo_url``: Github repository where the code is hosted. E.g:
 
-        settings_repo_url = "https://github.com/edx/myrepo"
+        settings_repo_url = "https://github.com/openedx/myrepo"
 
     - ``settings_repo_version``: current version of the git repository. E.g:
 
         import git
         try:
             repo = git.Repo(search_parent_directories=True)
             settings_repo_version = repo.head.object.hexsha
@@ -68,57 +70,67 @@
         """
         Iterate on the docutils nodes generated by this directive.
         """
         folder_path = self.options.get("folder_path", "")
         source_path = os.path.join(self.env.config.settings_source_path, folder_path)
         settings = find_settings(source_path)
         # folder_path can point to a file or directory
-        root_folder = folder_path if os.path.isdir(source_path) else os.path.dirname(folder_path)
+        root_folder = (
+            folder_path if os.path.isdir(source_path) else os.path.dirname(folder_path)
+        )
         for setting_name in sorted(settings):
             setting = settings[setting_name]
             # setting["filename"] is relative to the root_path
             setting_filename = os.path.join(root_folder, setting["filename"])
             setting_default_value = setting.get(".. setting_default:", "Not defined")
             setting_default_node = nodes.literal(
                 text=quote_value(setting_default_value)
             )
             setting_section = nodes.section("", ids=[f"setting-{setting_name}"])
-            setting_section += nodes.title(text=setting_name)
-            setting_section += nodes.paragraph("", "Default: ", setting_default_node)
+            setting_section += nodes.title(text=setting_name, ids=[f"title-{setting_name}"])
+            setting_section += nodes.paragraph(
+                "", "Default: ", setting_default_node, ids=[f"default-{setting_name}"]
+            )
             setting_section += nodes.paragraph(
                 "",
                 "Source: ",
                 nodes.reference(
                     text="{} (line {})".format(
                         setting["filename"], setting["line_number"]
                     ),
                     refuri="{}/blob/{}/{}#L{}".format(
                         self.env.config.settings_repo_url,
                         self.env.config.settings_repo_version,
                         setting_filename,
                         setting["line_number"],
                     ),
                 ),
+                ids=[f"source-{setting_name}"],
             )
             setting_section += nodes.paragraph(
-                text=setting.get(".. setting_description:", "")
+                text=setting.get(".. setting_description:", ""),
+                ids=[f"description-{setting_name}"],
             )
             if setting.get(".. setting_warning:") not in (None, "None", "n/a", "N/A"):
                 setting_section += nodes.warning(
-                    "", nodes.paragraph("", setting[".. setting_warning:"])
+                    "",
+                    nodes.paragraph("", setting[".. setting_warning:"]),
+                    ids=[f"warning-{setting_name}"],
                 )
             yield setting_section
 
 
 def setup(app):
     """
     Declare the Sphinx extension.
     """
     app.add_config_value(
-        "settings_source_path", os.path.abspath(".."), "env",
+        "settings_source_path",
+        os.path.abspath(".."),
+        "env",
     )
     app.add_config_value("settings_repo_url", "", "env")
     app.add_config_value("settings_repo_version", "master", "env")
     app.add_directive("settings", Settings)
 
     return {
         "version": "0.1",
```

### Comparing `code-annotations-1.3.0/code_annotations/extensions/base.py` & `code-annotations-1.5.0/code_annotations/extensions/base.py`

 * *Files identical despite different names*

### Comparing `code-annotations-1.3.0/code_annotations/find_django.py` & `code-annotations-1.5.0/code_annotations/find_django.py`

 * *Files identical despite different names*

### Comparing `code-annotations-1.3.0/code_annotations/find_static.py` & `code-annotations-1.5.0/code_annotations/find_static.py`

 * *Files identical despite different names*

### Comparing `code-annotations-1.3.0/code_annotations/generate_docs.py` & `code-annotations-1.5.0/code_annotations/generate_docs.py`

 * *Files identical despite different names*

### Comparing `code-annotations-1.3.0/code_annotations/helpers.py` & `code-annotations-1.5.0/code_annotations/helpers.py`

 * *Files identical despite different names*

### Comparing `code-annotations-1.3.0/code_annotations.egg-info/PKG-INFO` & `code-annotations-1.5.0/code_annotations.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: code-annotations
-Version: 1.3.0
+Version: 1.5.0
 Summary: Extensible tools for parsing annotations in codebases
-Home-page: https://github.com/edx/code-annotations
+Home-page: https://github.com/openedx/code-annotations
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: edx pii code annotations
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
+Description-Content-Type: text/x-rst
 Provides-Extra: django
 License-File: LICENSE.txt
 License-File: NOTICE.txt
 
 code-annotations
 =============================
 
@@ -55,24 +56,21 @@
 Please see ``LICENSE.txt`` for details.
 
 How To Contribute
 -----------------
 
 Contributions are very welcome.
 
-Please read `How To Contribute <https://github.com/edx/edx-platform/blob/master/CONTRIBUTING.rst>`_ for details.
-
-Even though they were written with ``edx-platform`` in mind, the guidelines
-should be followed for Open edX code in general.
+Please read `How To Contribute <https://github.com/openedx/.github/blob/master/CONTRIBUTING.md>`_ for details.
 
 PR description template should be automatically applied if you are sending PR from github interface; otherwise you
-can find it it at `PULL_REQUEST_TEMPLATE.md <https://github.com/edx/code-annotations/blob/master/.github/PULL_REQUEST_TEMPLATE.md>`_
+can find it it at `PULL_REQUEST_TEMPLATE.md <https://github.com/openedx/code-annotations/blob/master/.github/PULL_REQUEST_TEMPLATE.md>`_
 
 Issue report template should be automatically applied if you are sending it from github UI as well; otherwise you
-can find it at `ISSUE_TEMPLATE.md <https://github.com/edx/code-annotations/blob/master/.github/ISSUE_TEMPLATE.md>`_
+can find it at `ISSUE_TEMPLATE.md <https://github.com/openedx/code-annotations/blob/master/.github/ISSUE_TEMPLATE.md>`_
 
 Reporting Security Issues
 -------------------------
 
 Please do not report security issues in public. Please email security@edx.org.
 
 Getting Help
@@ -84,16 +82,16 @@
 .. _list of resources: https://open.edx.org/getting-help
 
 
 .. |pypi-badge| image:: https://img.shields.io/pypi/v/code-annotations.svg
     :target: https://pypi.python.org/pypi/code-annotations/
     :alt: PyPI
 
-.. |CI| image:: https://github.com/edx/code-annotations/workflows/Python%20CI/badge.svg?branch=master
-    :target: https://github.com/edx/code-annotations/actions?query=workflow%3A%22Python+CI%22
+.. |CI| image:: https://github.com/openedx/code-annotations/workflows/Python%20CI/badge.svg?branch=master
+    :target: https://github.com/openedx/code-annotations/actions?query=workflow%3A%22Python+CI%22
     :alt: CI
 
 .. |codecov-badge| image:: http://codecov.io/github/edx/code-annotations/coverage.svg?branch=master
     :target: http://codecov.io/github/edx/code-annotations?branch=master
     :alt: Codecov
 
 .. |doc-badge| image:: https://readthedocs.org/projects/code-annotations/badge/?version=latest
@@ -101,15 +99,15 @@
     :alt: Documentation
 
 .. |pyversions-badge| image:: https://img.shields.io/pypi/pyversions/code-annotations.svg
     :target: https://pypi.python.org/pypi/code-annotations/
     :alt: Supported Python versions
 
 .. |license-badge| image:: https://img.shields.io/github/license/edx/code-annotations.svg
-    :target: https://github.com/edx/code-annotations/blob/master/LICENSE.txt
+    :target: https://github.com/openedx/code-annotations/blob/master/LICENSE.txt
     :alt: License
 
 
 Change Log
 ----------
 
 ..
@@ -121,14 +119,27 @@
    This project adheres to Semantic Versioning (http://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
+
+[1.5.0] - 2023-07-21
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+* Switch from ``edx-sphinx-theme`` to ``sphinx-book-theme`` since the former is
+  deprecated
+* Added Support for Django 4.2
+
+[1.4.0] - 2022-05-23
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+* Rename toggle_warnings to toggle_warning for consistency with setting_warning.
+
 [1.3.0] - 2022-02-07
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 * Dropped Django 22, 30 and 31 Support
 * Added Django40 Support in CI
 
 [1.2.0] - 2021-07-26
```

### Comparing `code-annotations-1.3.0/code_annotations.egg-info/SOURCES.txt` & `code-annotations-1.5.0/code_annotations.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `code-annotations-1.3.0/setup.py` & `code-annotations-1.5.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -68,17 +68,18 @@
 CHANGELOG = open(os.path.join(os.path.dirname(__file__), 'CHANGELOG.rst')).read()
 
 setup(
     name='code-annotations',
     version=VERSION,
     description="""Extensible tools for parsing annotations in codebases""",
     long_description=README + '\n\n' + CHANGELOG,
+    long_description_content_type='text/x-rst',
     author='edX',
     author_email='oscm@edx.org',
-    url='https://github.com/edx/code-annotations',
+    url='https://github.com/openedx/code-annotations',
     packages=[
         'code_annotations',
     ],
     entry_points={
         'console_scripts': [
             'code_annotations = code_annotations.cli:entry_point',
         ],
@@ -93,15 +94,15 @@
     license="AGPL 3.0",
     zip_safe=False,
     keywords='edx pii code annotations',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Framework :: Django',
         'Framework :: Django :: 3.2',
-        'Framework :: Django :: 4.0',
+        'Framework :: Django :: 4.2',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: Apache Software License',
         'Natural Language :: English',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.8',
     ],
```

