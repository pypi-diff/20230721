# Comparing `tmp/assert_element-0.3.0.tar.gz` & `tmp/assert_element-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "assert_element-0.3.0.tar", last modified: Fri Sep 16 21:35:56 2022, max compression
+gzip compressed data, was "assert_element-0.4.0.tar", last modified: Fri Jul 21 16:34:55 2023, max compression
```

## Comparing `assert_element-0.3.0.tar` & `assert_element-0.4.0.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2022-09-16 21:35:56.178823 assert_element-0.3.0/
--rw-rw-r--   0 petr      (1000) petr      (1000)      146 2022-09-16 21:35:55.000000 assert_element-0.3.0/.coveragerc
--rw-rw-r--   0 petr      (1000) petr      (1000)      331 2022-09-16 21:35:55.000000 assert_element-0.3.0/.editorconfig
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2022-09-16 21:35:56.178823 assert_element-0.3.0/.github/
--rw-rw-r--   0 petr      (1000) petr      (1000)      350 2022-09-16 21:35:55.000000 assert_element-0.3.0/.github/ISSUE_TEMPLATE.md
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2022-09-16 21:35:56.178823 assert_element-0.3.0/.github/workflows/
--rw-rw-r--   0 petr      (1000) petr      (1000)     1992 2022-09-16 21:35:55.000000 assert_element-0.3.0/.github/workflows/main.yml
--rw-rw-r--   0 petr      (1000) petr      (1000)      419 2022-09-16 21:35:55.000000 assert_element-0.3.0/.gitignore
--rw-rw-r--   0 petr      (1000) petr      (1000)      158 2022-09-16 21:35:55.000000 assert_element-0.3.0/AUTHORS.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     3274 2022-09-16 21:35:55.000000 assert_element-0.3.0/CONTRIBUTING.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)      272 2022-09-16 21:35:55.000000 assert_element-0.3.0/HISTORY.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     1075 2022-09-16 21:35:55.000000 assert_element-0.3.0/LICENSE
--rw-rw-r--   0 petr      (1000) petr      (1000)      182 2022-09-16 21:35:55.000000 assert_element-0.3.0/MANIFEST.in
--rw-rw-r--   0 petr      (1000) petr      (1000)     4461 2022-09-16 21:35:56.178823 assert_element-0.3.0/PKG-INFO
--rw-rw-r--   0 petr      (1000) petr      (1000)     2430 2022-09-16 21:35:55.000000 assert_element-0.3.0/README.rst
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2022-09-16 21:35:56.178823 assert_element-0.3.0/assert_element/
--rw-rw-r--   0 petr      (1000) petr      (1000)       77 2022-09-16 21:35:55.000000 assert_element-0.3.0/assert_element/__init__.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      905 2022-09-16 21:35:55.000000 assert_element-0.3.0/assert_element/assert_element.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2022-09-16 21:35:56.178823 assert_element-0.3.0/assert_element.egg-info/
--rw-rw-r--   0 petr      (1000) petr      (1000)     4461 2022-09-16 21:35:56.000000 assert_element-0.3.0/assert_element.egg-info/PKG-INFO
--rw-rw-r--   0 petr      (1000) petr      (1000)      863 2022-09-16 21:35:56.000000 assert_element-0.3.0/assert_element.egg-info/SOURCES.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)        1 2022-09-16 21:35:56.000000 assert_element-0.3.0/assert_element.egg-info/dependency_links.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)        1 2022-09-16 21:35:56.000000 assert_element-0.3.0/assert_element.egg-info/not-zip-safe
--rw-rw-r--   0 petr      (1000) petr      (1000)       15 2022-09-16 21:35:56.000000 assert_element-0.3.0/assert_element.egg-info/requires.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)       15 2022-09-16 21:35:56.000000 assert_element-0.3.0/assert_element.egg-info/top_level.txt
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2022-09-16 21:35:56.178823 assert_element-0.3.0/docs/
--rw-rw-r--   0 petr      (1000) petr      (1000)     6778 2022-09-16 21:35:55.000000 assert_element-0.3.0/docs/Makefile
--rw-rw-r--   0 petr      (1000) petr      (1000)       28 2022-09-16 21:35:55.000000 assert_element-0.3.0/docs/authors.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     8450 2022-09-16 21:35:55.000000 assert_element-0.3.0/docs/conf.py
--rw-rw-r--   0 petr      (1000) petr      (1000)       33 2022-09-16 21:35:55.000000 assert_element-0.3.0/docs/contributing.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)       28 2022-09-16 21:35:55.000000 assert_element-0.3.0/docs/history.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)      452 2022-09-16 21:35:55.000000 assert_element-0.3.0/docs/index.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)      212 2022-09-16 21:35:55.000000 assert_element-0.3.0/docs/installation.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     6709 2022-09-16 21:35:55.000000 assert_element-0.3.0/docs/make.bat
--rw-rw-r--   0 petr      (1000) petr      (1000)       27 2022-09-16 21:35:55.000000 assert_element-0.3.0/docs/readme.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)      452 2022-09-16 21:35:55.000000 assert_element-0.3.0/docs/usage.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)      330 2022-09-16 21:35:55.000000 assert_element-0.3.0/manage.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      190 2022-09-16 21:35:55.000000 assert_element-0.3.0/mypy.ini
--rw-rw-r--   0 petr      (1000) petr      (1000)       50 2022-09-16 21:35:55.000000 assert_element-0.3.0/requirements.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)       34 2022-09-16 21:35:55.000000 assert_element-0.3.0/requirements_dev.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)      159 2022-09-16 21:35:55.000000 assert_element-0.3.0/requirements_test.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)      547 2022-09-16 21:35:55.000000 assert_element-0.3.0/runtests.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      487 2022-09-16 21:35:56.178823 assert_element-0.3.0/setup.cfg
--rwxrwxr-x   0 petr      (1000) petr      (1000)     2415 2022-09-16 21:35:55.000000 assert_element-0.3.0/setup.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     2265 2022-09-16 21:35:55.000000 assert_element-0.3.0/tasks.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2022-09-16 21:35:56.178823 assert_element-0.3.0/tests/
--rw-rw-r--   0 petr      (1000) petr      (1000)      652 2022-09-16 21:35:55.000000 assert_element-0.3.0/tests/README.md
--rw-rw-r--   0 petr      (1000) petr      (1000)        0 2022-09-16 21:35:55.000000 assert_element-0.3.0/tests/__init__.py
--rw-rw-r--   0 petr      (1000) petr      (1000)       90 2022-09-16 21:35:55.000000 assert_element-0.3.0/tests/requirements.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)     3062 2022-09-16 21:35:55.000000 assert_element-0.3.0/tests/settings.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     1685 2022-09-16 21:35:55.000000 assert_element-0.3.0/tests/test_models.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      200 2022-09-16 21:35:55.000000 assert_element-0.3.0/tests/urls.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      390 2022-09-16 21:35:55.000000 assert_element-0.3.0/tests/wsgi.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      369 2022-09-16 21:35:55.000000 assert_element-0.3.0/tox.ini
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-07-21 16:34:55.926930 assert_element-0.4.0/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      146 2023-07-21 16:34:55.000000 assert_element-0.4.0/.coveragerc
+-rw-rw-r--   0 petr      (1000) petr      (1000)      331 2023-07-21 16:34:55.000000 assert_element-0.4.0/.editorconfig
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-07-21 16:34:55.922930 assert_element-0.4.0/.github/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      350 2023-07-21 16:34:55.000000 assert_element-0.4.0/.github/ISSUE_TEMPLATE.md
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-07-21 16:34:55.922930 assert_element-0.4.0/.github/workflows/
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1992 2023-07-21 16:34:55.000000 assert_element-0.4.0/.github/workflows/main.yml
+-rw-rw-r--   0 petr      (1000) petr      (1000)      419 2023-07-21 16:34:55.000000 assert_element-0.4.0/.gitignore
+-rw-rw-r--   0 petr      (1000) petr      (1000)      158 2023-07-21 16:34:55.000000 assert_element-0.4.0/AUTHORS.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     3274 2023-07-21 16:34:55.000000 assert_element-0.4.0/CONTRIBUTING.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)      356 2023-07-21 16:34:55.000000 assert_element-0.4.0/HISTORY.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1075 2023-07-21 16:34:55.000000 assert_element-0.4.0/LICENSE
+-rw-rw-r--   0 petr      (1000) petr      (1000)      182 2023-07-21 16:34:55.000000 assert_element-0.4.0/MANIFEST.in
+-rw-rw-r--   0 petr      (1000) petr      (1000)     3658 2023-07-21 16:34:55.926930 assert_element-0.4.0/PKG-INFO
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2430 2023-07-21 16:34:55.000000 assert_element-0.4.0/README.rst
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-07-21 16:34:55.922930 assert_element-0.4.0/assert_element/
+-rw-rw-r--   0 petr      (1000) petr      (1000)       77 2023-07-21 16:34:55.000000 assert_element-0.4.0/assert_element/__init__.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1695 2023-07-21 16:34:55.000000 assert_element-0.4.0/assert_element/assert_element.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-07-21 16:34:55.926930 assert_element-0.4.0/assert_element.egg-info/
+-rw-rw-r--   0 petr      (1000) petr      (1000)     3658 2023-07-21 16:34:55.000000 assert_element-0.4.0/assert_element.egg-info/PKG-INFO
+-rw-rw-r--   0 petr      (1000) petr      (1000)      863 2023-07-21 16:34:55.000000 assert_element-0.4.0/assert_element.egg-info/SOURCES.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)        1 2023-07-21 16:34:55.000000 assert_element-0.4.0/assert_element.egg-info/dependency_links.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)        1 2023-07-21 16:34:55.000000 assert_element-0.4.0/assert_element.egg-info/not-zip-safe
+-rw-rw-r--   0 petr      (1000) petr      (1000)       15 2023-07-21 16:34:55.000000 assert_element-0.4.0/assert_element.egg-info/requires.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)       15 2023-07-21 16:34:55.000000 assert_element-0.4.0/assert_element.egg-info/top_level.txt
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-07-21 16:34:55.926930 assert_element-0.4.0/docs/
+-rw-rw-r--   0 petr      (1000) petr      (1000)     6778 2023-07-21 16:34:55.000000 assert_element-0.4.0/docs/Makefile
+-rw-rw-r--   0 petr      (1000) petr      (1000)       28 2023-07-21 16:34:55.000000 assert_element-0.4.0/docs/authors.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     8450 2023-07-21 16:34:55.000000 assert_element-0.4.0/docs/conf.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)       33 2023-07-21 16:34:55.000000 assert_element-0.4.0/docs/contributing.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)       28 2023-07-21 16:34:55.000000 assert_element-0.4.0/docs/history.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)      452 2023-07-21 16:34:55.000000 assert_element-0.4.0/docs/index.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)      212 2023-07-21 16:34:55.000000 assert_element-0.4.0/docs/installation.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     6709 2023-07-21 16:34:55.000000 assert_element-0.4.0/docs/make.bat
+-rw-rw-r--   0 petr      (1000) petr      (1000)       27 2023-07-21 16:34:55.000000 assert_element-0.4.0/docs/readme.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)      452 2023-07-21 16:34:55.000000 assert_element-0.4.0/docs/usage.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)      330 2023-07-21 16:34:55.000000 assert_element-0.4.0/manage.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      190 2023-07-21 16:34:55.000000 assert_element-0.4.0/mypy.ini
+-rw-rw-r--   0 petr      (1000) petr      (1000)       50 2023-07-21 16:34:55.000000 assert_element-0.4.0/requirements.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)       34 2023-07-21 16:34:55.000000 assert_element-0.4.0/requirements_dev.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)      159 2023-07-21 16:34:55.000000 assert_element-0.4.0/requirements_test.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)      547 2023-07-21 16:34:55.000000 assert_element-0.4.0/runtests.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      412 2023-07-21 16:34:55.926930 assert_element-0.4.0/setup.cfg
+-rwxrwxr-x   0 petr      (1000) petr      (1000)     2415 2023-07-21 16:34:55.000000 assert_element-0.4.0/setup.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2265 2023-07-21 16:34:55.000000 assert_element-0.4.0/tasks.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-07-21 16:34:55.926930 assert_element-0.4.0/tests/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      652 2023-07-21 16:34:55.000000 assert_element-0.4.0/tests/README.md
+-rw-rw-r--   0 petr      (1000) petr      (1000)        0 2023-07-21 16:34:55.000000 assert_element-0.4.0/tests/__init__.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)       90 2023-07-21 16:34:55.000000 assert_element-0.4.0/tests/requirements.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)     3062 2023-07-21 16:34:55.000000 assert_element-0.4.0/tests/settings.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1685 2023-07-21 16:34:55.000000 assert_element-0.4.0/tests/test_models.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      200 2023-07-21 16:34:55.000000 assert_element-0.4.0/tests/urls.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      390 2023-07-21 16:34:55.000000 assert_element-0.4.0/tests/wsgi.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      369 2023-07-21 16:34:55.000000 assert_element-0.4.0/tox.ini
```

### Comparing `assert_element-0.3.0/.github/workflows/main.yml` & `assert_element-0.4.0/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `assert_element-0.3.0/CONTRIBUTING.rst` & `assert_element-0.4.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `assert_element-0.3.0/LICENSE` & `assert_element-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `assert_element-0.3.0/PKG-INFO` & `assert_element-0.4.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,135 +1,141 @@
 Metadata-Version: 2.1
 Name: assert_element
-Version: 0.3.0
+Version: 0.4.0
 Summary: Simple TestCase assertion that finds element based on it's path and check if it equals with given content.
 Home-page: https://github.com/PetrDlouhy/django-assert-element
 Author: Petr Dlouhý
 Author-email: petr.dlouhy@email.cz
 License: MIT
-Description: =============================
-        Django assert element
-        =============================
-        
-        .. image:: https://badge.fury.io/py/assert_element.svg
-            :target: https://badge.fury.io/py/assert_element
-        
-        .. image:: https://codecov.io/gh/PetrDlouhy/assert_element/branch/master/graph/badge.svg
-            :target: https://codecov.io/gh/PetrDlouhy/assert_element
-        
-        .. image:: https://github.com/PetrDlouhy/django-assert-element/actions/workflows/main.yml/badge.svg?event=registry_package
-            :target: https://github.com/PetrDlouhy/django-assert-element/actions/workflows/main.yml
-        
-        Simple TestCase assertion that finds element based on it's path and check if it equals with given content.
-        
-        This is more useful than the default Django AssertContains
-        because it will find the element and show differences if something changed.
-        The test also tries to ignore differences in whitespaces as much as possible.
-        
-        Other similar projects
-        ----------------------
-        
-        I released this package just to realize after few days, that there are some other very similar projects:
-        
-        * https://pypi.org/project/django_html_assertions/
-        * https://django-with-asserts.readthedocs.io/en/latest/
-        * https://github.com/robjohncox/python-html-assert
-        
-        Documentation
-        -------------
-        
-        The full documentation is at https://assert_element.readthedocs.io.
-        
-        Quickstart
-        ----------
-        
-        Install by:
-        
-        .. code-block:: bash
-            
-            pip install assert-element
-        
-        Usage in tests:
-        
-        .. code-block:: python
-        
-            from assert_element import AssertElementMixin
-        
-            class MyTestCase(AssertElementMixin, TestCase):
-                def test_something(self):
-                    response = self.client.get(address)
-                    self.assertElementContains(
-                        response,
-                        'div[id="my-div"]',
-                        '<div id="my-div">My div</div>',
-                    )
-        
-        The first attribute can be response or content itself.
-        Second attribute is the path to the element.
-        Third attribute is the expected content.
-        
-        Running Tests
-        -------------
-        
-        Does the code actually work?
-        
-        ::
-        
-            source <YOURVIRTUALENV>/bin/activate
-            (myenv) $ pip install tox
-            (myenv) $ tox
-        
-        
-        Development commands
-        ---------------------
-        
-        ::
-        
-            pip install -r requirements_dev.txt
-            invoke -l
-        
-        
-        Credits
-        -------
-        
-        Tools used in rendering this package:
-        
-        *  Cookiecutter_
-        *  `cookiecutter-djangopackage`_
-        
-        .. _Cookiecutter: https://github.com/audreyr/cookiecutter
-        .. _`cookiecutter-djangopackage`: https://github.com/pydanny/cookiecutter-djangopackage
-        
-        
-        
-        
-        History
-        -------
-        
-        0.3.0 (2022-09-16)
-        ++++++++++++++++++
-        
-        * more tolerance in whitespace differences
-        
-        0.2.0 (2022-09-01)
-        ++++++++++++++++++
-        
-        * first attribute can be response or content itself
-        
-        0.1.0 (2022-08-21)
-        ++++++++++++++++++
-        
-        * First release on PyPI.
-        
 Keywords: assert_element
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django :: 1.11
 Classifier: Framework :: Django :: 2.1
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
+License-File: LICENSE
+License-File: AUTHORS.rst
+
+=============================
+Django assert element
+=============================
+
+.. image:: https://badge.fury.io/py/assert_element.svg
+    :target: https://badge.fury.io/py/assert_element
+
+.. image:: https://codecov.io/gh/PetrDlouhy/assert_element/branch/master/graph/badge.svg
+    :target: https://codecov.io/gh/PetrDlouhy/assert_element
+
+.. image:: https://github.com/PetrDlouhy/django-assert-element/actions/workflows/main.yml/badge.svg?event=registry_package
+    :target: https://github.com/PetrDlouhy/django-assert-element/actions/workflows/main.yml
+
+Simple TestCase assertion that finds element based on it's path and check if it equals with given content.
+
+This is more useful than the default Django AssertContains
+because it will find the element and show differences if something changed.
+The test also tries to ignore differences in whitespaces as much as possible.
+
+Other similar projects
+----------------------
+
+I released this package just to realize after few days, that there are some other very similar projects:
+
+* https://pypi.org/project/django_html_assertions/
+* https://django-with-asserts.readthedocs.io/en/latest/
+* https://github.com/robjohncox/python-html-assert
+
+Documentation
+-------------
+
+The full documentation is at https://assert_element.readthedocs.io.
+
+Quickstart
+----------
+
+Install by:
+
+.. code-block:: bash
+    
+    pip install assert-element
+
+Usage in tests:
+
+.. code-block:: python
+
+    from assert_element import AssertElementMixin
+
+    class MyTestCase(AssertElementMixin, TestCase):
+        def test_something(self):
+            response = self.client.get(address)
+            self.assertElementContains(
+                response,
+                'div[id="my-div"]',
+                '<div id="my-div">My div</div>',
+            )
+
+The first attribute can be response or content itself.
+Second attribute is the path to the element.
+Third attribute is the expected content.
+
+Running Tests
+-------------
+
+Does the code actually work?
+
+::
+
+    source <YOURVIRTUALENV>/bin/activate
+    (myenv) $ pip install tox
+    (myenv) $ tox
+
+
+Development commands
+---------------------
+
+::
+
+    pip install -r requirements_dev.txt
+    invoke -l
+
+
+Credits
+-------
+
+Tools used in rendering this package:
+
+*  Cookiecutter_
+*  `cookiecutter-djangopackage`_
+
+.. _Cookiecutter: https://github.com/audreyr/cookiecutter
+.. _`cookiecutter-djangopackage`: https://github.com/pydanny/cookiecutter-djangopackage
+
+
+
+
+History
+-------
+
+0.4.0 (2023-07-21)
+++++++++++++++++++
+
+* more readable output when assertion fails
+
+0.3.0 (2022-09-16)
+++++++++++++++++++
+
+* more tolerance in whitespace differences
+
+0.2.0 (2022-09-01)
+++++++++++++++++++
+
+* first attribute can be response or content itself
+
+0.1.0 (2022-08-21)
+++++++++++++++++++
+
+* First release on PyPI.
```

### Comparing `assert_element-0.3.0/README.rst` & `assert_element-0.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `assert_element-0.3.0/assert_element.egg-info/PKG-INFO` & `assert_element-0.4.0/assert_element.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,135 +1,141 @@
 Metadata-Version: 2.1
 Name: assert-element
-Version: 0.3.0
+Version: 0.4.0
 Summary: Simple TestCase assertion that finds element based on it's path and check if it equals with given content.
 Home-page: https://github.com/PetrDlouhy/django-assert-element
 Author: Petr Dlouhý
 Author-email: petr.dlouhy@email.cz
 License: MIT
-Description: =============================
-        Django assert element
-        =============================
-        
-        .. image:: https://badge.fury.io/py/assert_element.svg
-            :target: https://badge.fury.io/py/assert_element
-        
-        .. image:: https://codecov.io/gh/PetrDlouhy/assert_element/branch/master/graph/badge.svg
-            :target: https://codecov.io/gh/PetrDlouhy/assert_element
-        
-        .. image:: https://github.com/PetrDlouhy/django-assert-element/actions/workflows/main.yml/badge.svg?event=registry_package
-            :target: https://github.com/PetrDlouhy/django-assert-element/actions/workflows/main.yml
-        
-        Simple TestCase assertion that finds element based on it's path and check if it equals with given content.
-        
-        This is more useful than the default Django AssertContains
-        because it will find the element and show differences if something changed.
-        The test also tries to ignore differences in whitespaces as much as possible.
-        
-        Other similar projects
-        ----------------------
-        
-        I released this package just to realize after few days, that there are some other very similar projects:
-        
-        * https://pypi.org/project/django_html_assertions/
-        * https://django-with-asserts.readthedocs.io/en/latest/
-        * https://github.com/robjohncox/python-html-assert
-        
-        Documentation
-        -------------
-        
-        The full documentation is at https://assert_element.readthedocs.io.
-        
-        Quickstart
-        ----------
-        
-        Install by:
-        
-        .. code-block:: bash
-            
-            pip install assert-element
-        
-        Usage in tests:
-        
-        .. code-block:: python
-        
-            from assert_element import AssertElementMixin
-        
-            class MyTestCase(AssertElementMixin, TestCase):
-                def test_something(self):
-                    response = self.client.get(address)
-                    self.assertElementContains(
-                        response,
-                        'div[id="my-div"]',
-                        '<div id="my-div">My div</div>',
-                    )
-        
-        The first attribute can be response or content itself.
-        Second attribute is the path to the element.
-        Third attribute is the expected content.
-        
-        Running Tests
-        -------------
-        
-        Does the code actually work?
-        
-        ::
-        
-            source <YOURVIRTUALENV>/bin/activate
-            (myenv) $ pip install tox
-            (myenv) $ tox
-        
-        
-        Development commands
-        ---------------------
-        
-        ::
-        
-            pip install -r requirements_dev.txt
-            invoke -l
-        
-        
-        Credits
-        -------
-        
-        Tools used in rendering this package:
-        
-        *  Cookiecutter_
-        *  `cookiecutter-djangopackage`_
-        
-        .. _Cookiecutter: https://github.com/audreyr/cookiecutter
-        .. _`cookiecutter-djangopackage`: https://github.com/pydanny/cookiecutter-djangopackage
-        
-        
-        
-        
-        History
-        -------
-        
-        0.3.0 (2022-09-16)
-        ++++++++++++++++++
-        
-        * more tolerance in whitespace differences
-        
-        0.2.0 (2022-09-01)
-        ++++++++++++++++++
-        
-        * first attribute can be response or content itself
-        
-        0.1.0 (2022-08-21)
-        ++++++++++++++++++
-        
-        * First release on PyPI.
-        
 Keywords: assert_element
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django :: 1.11
 Classifier: Framework :: Django :: 2.1
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
+License-File: LICENSE
+License-File: AUTHORS.rst
+
+=============================
+Django assert element
+=============================
+
+.. image:: https://badge.fury.io/py/assert_element.svg
+    :target: https://badge.fury.io/py/assert_element
+
+.. image:: https://codecov.io/gh/PetrDlouhy/assert_element/branch/master/graph/badge.svg
+    :target: https://codecov.io/gh/PetrDlouhy/assert_element
+
+.. image:: https://github.com/PetrDlouhy/django-assert-element/actions/workflows/main.yml/badge.svg?event=registry_package
+    :target: https://github.com/PetrDlouhy/django-assert-element/actions/workflows/main.yml
+
+Simple TestCase assertion that finds element based on it's path and check if it equals with given content.
+
+This is more useful than the default Django AssertContains
+because it will find the element and show differences if something changed.
+The test also tries to ignore differences in whitespaces as much as possible.
+
+Other similar projects
+----------------------
+
+I released this package just to realize after few days, that there are some other very similar projects:
+
+* https://pypi.org/project/django_html_assertions/
+* https://django-with-asserts.readthedocs.io/en/latest/
+* https://github.com/robjohncox/python-html-assert
+
+Documentation
+-------------
+
+The full documentation is at https://assert_element.readthedocs.io.
+
+Quickstart
+----------
+
+Install by:
+
+.. code-block:: bash
+    
+    pip install assert-element
+
+Usage in tests:
+
+.. code-block:: python
+
+    from assert_element import AssertElementMixin
+
+    class MyTestCase(AssertElementMixin, TestCase):
+        def test_something(self):
+            response = self.client.get(address)
+            self.assertElementContains(
+                response,
+                'div[id="my-div"]',
+                '<div id="my-div">My div</div>',
+            )
+
+The first attribute can be response or content itself.
+Second attribute is the path to the element.
+Third attribute is the expected content.
+
+Running Tests
+-------------
+
+Does the code actually work?
+
+::
+
+    source <YOURVIRTUALENV>/bin/activate
+    (myenv) $ pip install tox
+    (myenv) $ tox
+
+
+Development commands
+---------------------
+
+::
+
+    pip install -r requirements_dev.txt
+    invoke -l
+
+
+Credits
+-------
+
+Tools used in rendering this package:
+
+*  Cookiecutter_
+*  `cookiecutter-djangopackage`_
+
+.. _Cookiecutter: https://github.com/audreyr/cookiecutter
+.. _`cookiecutter-djangopackage`: https://github.com/pydanny/cookiecutter-djangopackage
+
+
+
+
+History
+-------
+
+0.4.0 (2023-07-21)
+++++++++++++++++++
+
+* more readable output when assertion fails
+
+0.3.0 (2022-09-16)
+++++++++++++++++++
+
+* more tolerance in whitespace differences
+
+0.2.0 (2022-09-01)
+++++++++++++++++++
+
+* first attribute can be response or content itself
+
+0.1.0 (2022-08-21)
+++++++++++++++++++
+
+* First release on PyPI.
```

### Comparing `assert_element-0.3.0/assert_element.egg-info/SOURCES.txt` & `assert_element-0.4.0/assert_element.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `assert_element-0.3.0/docs/Makefile` & `assert_element-0.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `assert_element-0.3.0/docs/conf.py` & `assert_element-0.4.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `assert_element-0.3.0/docs/make.bat` & `assert_element-0.4.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `assert_element-0.3.0/runtests.py` & `assert_element-0.4.0/runtests.py`

 * *Files identical despite different names*

### Comparing `assert_element-0.3.0/setup.py` & `assert_element-0.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `assert_element-0.3.0/tasks.py` & `assert_element-0.4.0/tasks.py`

 * *Files identical despite different names*

### Comparing `assert_element-0.3.0/tests/README.md` & `assert_element-0.4.0/tests/README.md`

 * *Files identical despite different names*

### Comparing `assert_element-0.3.0/tests/settings.py` & `assert_element-0.4.0/tests/settings.py`

 * *Files identical despite different names*

### Comparing `assert_element-0.3.0/tests/test_models.py` & `assert_element-0.4.0/tests/test_models.py`

 * *Files identical despite different names*

