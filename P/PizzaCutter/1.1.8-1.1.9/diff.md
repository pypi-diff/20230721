# Comparing `tmp/pizzacutter-1.1.8.tar.gz` & `tmp/pizzacutter-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pizzacutter-1.1.8.tar", last modified: Sat Aug  8 12:53:47 2020, max compression
+gzip compressed data, was "dist/pizzacutter-1.1.9.tar", last modified: Fri Oct  9 16:27:24 2020, max compression
```

## Comparing `pizzacutter-1.1.8.tar` & `pizzacutter-1.1.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-08-08 12:53:47.138567 pizzacutter-1.1.8/
--rw-rw-r--   0 travis    (2000) travis    (2000)      929 2020-08-08 12:53:14.000000 pizzacutter-1.1.8/CHANGES.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      124 2020-08-08 12:53:14.000000 pizzacutter-1.1.8/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)    24562 2020-08-08 12:53:47.138567 pizzacutter-1.1.8/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)    19788 2020-08-08 12:53:46.000000 pizzacutter-1.1.8/README.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-08-08 12:53:47.134567 pizzacutter-1.1.8/pizzacutter/
--rw-rw-r--   0 travis    (2000) travis    (2000)      421 2020-08-08 12:53:14.000000 pizzacutter-1.1.8/pizzacutter/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      503 2020-08-08 12:53:14.000000 pizzacutter-1.1.8/pizzacutter/__init__conf__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    41858 2020-08-08 12:53:14.000000 pizzacutter-1.1.8/pizzacutter/pizzacutter.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4359 2020-08-08 12:53:14.000000 pizzacutter-1.1.8/pizzacutter/pizzacutter_cli.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-08-08 12:53:14.000000 pizzacutter-1.1.8/pizzacutter/py.typed
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-08-08 12:53:47.138567 pizzacutter-1.1.8/pizzacutter/sub/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-08-08 12:53:14.000000 pizzacutter-1.1.8/pizzacutter/sub/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2046 2020-08-08 12:53:14.000000 pizzacutter-1.1.8/pizzacutter/sub/get_config.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4022 2020-08-08 12:53:14.000000 pizzacutter-1.1.8/pizzacutter/sub/helpers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2576 2020-08-08 12:53:14.000000 pizzacutter-1.1.8/pizzacutter/sub/import_module.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10347 2020-08-08 12:53:14.000000 pizzacutter-1.1.8/pizzacutter/sub/pizzacutter_config.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-08-08 12:53:47.138567 pizzacutter-1.1.8/pizzacutter.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)    24562 2020-08-08 12:53:47.000000 pizzacutter-1.1.8/pizzacutter.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      603 2020-08-08 12:53:47.000000 pizzacutter-1.1.8/pizzacutter.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-08-08 12:53:47.000000 pizzacutter-1.1.8/pizzacutter.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       70 2020-08-08 12:53:47.000000 pizzacutter-1.1.8/pizzacutter.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-08-08 12:53:46.000000 pizzacutter-1.1.8/pizzacutter.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)       31 2020-08-08 12:53:47.000000 pizzacutter-1.1.8/pizzacutter.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       12 2020-08-08 12:53:47.000000 pizzacutter-1.1.8/pizzacutter.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      252 2020-08-08 12:53:14.000000 pizzacutter-1.1.8/pyproject.toml
--rw-rw-r--   0 travis    (2000) travis    (2000)      592 2020-08-08 12:53:47.138567 pizzacutter-1.1.8/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     4183 2020-08-08 12:53:14.000000 pizzacutter-1.1.8/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-09 16:27:24.000000 pizzacutter-1.1.9/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4183 2020-10-09 16:26:30.000000 pizzacutter-1.1.9/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-09 16:27:24.000000 pizzacutter-1.1.9/pizzacutter.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-10-09 16:27:23.000000 pizzacutter-1.1.9/pizzacutter.egg-info/not-zip-safe
+-rw-rw-r--   0 travis    (2000) travis    (2000)      603 2020-10-09 16:27:24.000000 pizzacutter-1.1.9/pizzacutter.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       70 2020-10-09 16:27:24.000000 pizzacutter-1.1.9/pizzacutter.egg-info/entry_points.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       12 2020-10-09 16:27:24.000000 pizzacutter-1.1.9/pizzacutter.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-10-09 16:27:24.000000 pizzacutter-1.1.9/pizzacutter.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       31 2020-10-09 16:27:24.000000 pizzacutter-1.1.9/pizzacutter.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)    24902 2020-10-09 16:27:24.000000 pizzacutter-1.1.9/pizzacutter.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20056 2020-10-09 16:26:30.000000 pizzacutter-1.1.9/README.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)    24902 2020-10-09 16:27:24.000000 pizzacutter-1.1.9/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)      124 2020-10-09 16:26:30.000000 pizzacutter-1.1.9/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)      592 2020-10-09 16:27:24.000000 pizzacutter-1.1.9/setup.cfg
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-09 16:27:24.000000 pizzacutter-1.1.9/pizzacutter/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-10-09 16:26:30.000000 pizzacutter-1.1.9/pizzacutter/py.typed
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-09 16:27:24.000000 pizzacutter-1.1.9/pizzacutter/sub/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2046 2020-10-09 16:26:30.000000 pizzacutter-1.1.9/pizzacutter/sub/get_config.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4022 2020-10-09 16:26:30.000000 pizzacutter-1.1.9/pizzacutter/sub/helpers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2576 2020-10-09 16:26:30.000000 pizzacutter-1.1.9/pizzacutter/sub/import_module.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-10-09 16:26:30.000000 pizzacutter-1.1.9/pizzacutter/sub/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10347 2020-10-09 16:26:30.000000 pizzacutter-1.1.9/pizzacutter/sub/pizzacutter_config.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    41086 2020-10-09 16:26:30.000000 pizzacutter-1.1.9/pizzacutter/pizzacutter.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4359 2020-10-09 16:26:30.000000 pizzacutter-1.1.9/pizzacutter/pizzacutter_cli.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      503 2020-10-09 16:26:30.000000 pizzacutter-1.1.9/pizzacutter/__init__conf__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      421 2020-10-09 16:26:30.000000 pizzacutter-1.1.9/pizzacutter/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      252 2020-10-09 16:26:30.000000 pizzacutter-1.1.9/pyproject.toml
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1089 2020-10-09 16:26:30.000000 pizzacutter-1.1.9/CHANGES.rst
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `pizzacutter-1.1.8/CHANGES.rst` & `pizzacutter-1.1.9/CHANGES.rst`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 Changelog
 =========
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v1.1.9
+--------
+2020-10-09: service release
+    - update travis build matrix for linux 3.9-dev
+    - update travis build matrix (paths) for windows 3.9 / 3.10
+
 v1.1.8
 --------
 2020-08-08: service release
     - fix documentation
     - fix travis
     - deprecate pycodestyle
     - implement flake8
```

### Comparing `pizzacutter-1.1.8/PKG-INFO` & `pizzacutter-1.1.9/pizzacutter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: pizzacutter
-Version: 1.1.8
+Version: 1.1.9
 Summary: create and update projects from project templates
 Home-page: https://github.com/bitranox/PizzaCutter
 Author: Robert Nowotny
 Author-email: bitranox@gmail.com
 License: UNKNOWN
 Description: PizzaCutter
         ===========
         
         
-        Version v1.1.8 as of 2020-08-08 see `Changelog`_
+        Version v1.1.9 as of 2020-10-09 see `Changelog`_
         
         |travis_build| |license| |pypi|
         
         |codecov| |better_code| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
         
         
         .. |travis_build| image:: https://img.shields.io/travis/bitranox/PizzaCutter/master.svg
@@ -47,14 +47,17 @@
         .. |cc_coverage| image:: https://img.shields.io/codeclimate/coverage/bitranox/PizzaCutter?label=CC%20coverage
            :target: https://codeclimate.com/github/bitranox/PizzaCutter/test_coverage
            :alt: Code Coverage
         
         .. |snyk| image:: https://img.shields.io/snyk/vulnerabilities/github/bitranox/PizzaCutter
            :target: https://snyk.io/test/github/bitranox/PizzaCutter
         
+        .. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
+           :target: https://github.com/psf/black
+        
         FUNCTION
         ========
         
         A command-line utility that creates and updates software projects in any language from PizzaCutter project templates.
         
         for the impatient, find here the latest PizzaCutter Templates:
             - `PizzaCutter default python template <https://github.com/bitranox/pct_python_default>`_
@@ -87,15 +90,15 @@
            import pizzacutter
            pizzacutter.build(path_conf_file=pathlib.Path('./.../.../path_to_conf_file.py'))
         
         - Directory names and filenames can be templated. For example:
         
         .. code-block:: bash
         
-           {{\PizzaCutter.repo_name}}/{{\PizzaCutter.repo_name}}/{{\PizzaCutter.repo_name}}.py
+           {{PizzaCutter.repo_name}}/{{PizzaCutter.repo_name}}/{{PizzaCutter.repo_name}}.py
         
         - Supports unlimited levels of directory nesting. (beware of possible path length limitations, especially on Travis Windows builds)
         - 100% of templating is done with just (bytes) replace function. No Jinja2.
         
         Why PizzaCutter?
         ================
         
@@ -170,35 +173,35 @@
                     # but can be useful to drop files on the desktop, /etc, and so on
                     self.pizza_cutter_allow_outside_write = False
                     self.pizza_cutter_dry_run = False
                     self.pizza_cutter_quiet = False
         
             # User Section - do whatever You want here
             # Pizza Cutter Configuration, can override by cli options.
-            # You might name Your Patterns as You like {{\PizzaCutter. ... }}, {{LemonCutter. ... }}, {{MelonCutter. ... }}
-                    self.pizza_cutter_patterns['{{\PizzaCutter.full_name}}'] = 'Robert Nowotny'
-                    self.pizza_cutter_patterns['{{\PizzaCutter.email}}'] = 'bitranox@gmail.com'
-                    self.pizza_cutter_patterns['{{\PizzaCutter.project.name}}'] = 'Complexity'
-                    self.pizza_cutter_patterns['{{\PizzaCutter.project_short_description}}'] = 'Refreshingly simple static site generator.'
-                    self.pizza_cutter_patterns['{{\PizzaCutter.release_date}}'] = '2013-07-10'
-                    self.pizza_cutter_patterns['{{\PizzaCutter.year}}'] = '2013'
-                    self.pizza_cutter_patterns['{{\PizzaCutter.current_version}}'] = '0.1.1'
+            # You might name Your Patterns as You like {{PizzaCutter. ... }}, {{LemonCutter. ... }}, {{MelonCutter. ... }}
+                    self.pizza_cutter_patterns['{{PizzaCutter.full_name}}'] = 'Robert Nowotny'
+                    self.pizza_cutter_patterns['{{PizzaCutter.email}}'] = 'bitranox@gmail.com'
+                    self.pizza_cutter_patterns['{{PizzaCutter.project.name}}'] = 'Complexity'
+                    self.pizza_cutter_patterns['{{PizzaCutter.project_short_description}}'] = 'Refreshingly simple static site generator.'
+                    self.pizza_cutter_patterns['{{PizzaCutter.release_date}}'] = '2013-07-10'
+                    self.pizza_cutter_patterns['{{PizzaCutter.year}}'] = '2013'
+                    self.pizza_cutter_patterns['{{PizzaCutter.current_version}}'] = '0.1.1'
         
                 self.set_defaults()
                 self.set_patterns()
         
         well - that looks like a cookiecutter configuration, only a bit more complicated, so what is the difference ?
         In .XML Files You just can not program. What, if for instance You want to update the "release_date"
         to the current date automatically, every time You update Your project ?
         
         With Pizzacutter its easy :
         
         .. code-block:: python
         
-                    self.pizza_cutter_patterns['{{\PizzaCutter.release_date}}'] = datetime.datetime.strptime(today, '%Y-%m-%d')
+                    self.pizza_cutter_patterns['{{PizzaCutter.release_date}}'] = datetime.datetime.strptime(today, '%Y-%m-%d')
         
         This is where the flexibility starts - You can dynamically calculate and assign values in the config file.
         
         So easy, so effective, just use python for Your config.
         
         
         PizzaCutter is created and maintained with PizzaCutter !
@@ -249,15 +252,15 @@
         ----
         
         automated tests, Travis Matrix, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
         .com/bitranox/PizzaCutter>`_ (cookiecutter on steroids)
         
         Python version required: 3.6.0 or newer
         
-        tested on linux "bionic" with python 3.6, 3.7, 3.8, 3.8-dev, pypy3 - architectures: amd64, ppc64le, s390x, arm64
+        tested on linux "bionic" with python 3.6, 3.7, 3.8, 3.9-dev, pypy3 - architectures: amd64, ppc64le, s390x, arm64
         
         `100% code coverage <https://codecov.io/gh/bitranox/PizzaCutter>`_, flake8 style checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://travis-ci.org/bitranox/PizzaCutter>`_, automatic daily builds and monitoring
         
         ----
         
         - `Usage`_
         - `Usage from Commandline`_
@@ -466,14 +469,20 @@
         Changelog
         =========
         
         - new MAJOR version for incompatible API changes,
         - new MINOR version for added functionality in a backwards compatible manner
         - new PATCH version for backwards compatible bug fixes
         
+        v1.1.9
+        --------
+        2020-10-09: service release
+            - update travis build matrix for linux 3.9-dev
+            - update travis build matrix (paths) for windows 3.9 / 3.10
+        
         v1.1.8
         --------
         2020-08-08: service release
             - fix documentation
             - fix travis
             - deprecate pycodestyle
             - implement flake8
```

### Comparing `pizzacutter-1.1.8/README.rst` & `pizzacutter-1.1.9/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 PizzaCutter
 ===========
 
 
-Version v1.1.8 as of 2020-08-08 see `Changelog`_
+Version v1.1.9 as of 2020-10-09 see `Changelog`_
 
 |travis_build| |license| |pypi|
 
 |codecov| |better_code| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
 
 
 .. |travis_build| image:: https://img.shields.io/travis/bitranox/PizzaCutter/master.svg
@@ -39,14 +39,17 @@
 .. |cc_coverage| image:: https://img.shields.io/codeclimate/coverage/bitranox/PizzaCutter?label=CC%20coverage
    :target: https://codeclimate.com/github/bitranox/PizzaCutter/test_coverage
    :alt: Code Coverage
 
 .. |snyk| image:: https://img.shields.io/snyk/vulnerabilities/github/bitranox/PizzaCutter
    :target: https://snyk.io/test/github/bitranox/PizzaCutter
 
+.. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
+   :target: https://github.com/psf/black
+
 FUNCTION
 ========
 
 A command-line utility that creates and updates software projects in any language from PizzaCutter project templates.
 
 for the impatient, find here the latest PizzaCutter Templates:
     - `PizzaCutter default python template <https://github.com/bitranox/pct_python_default>`_
@@ -79,15 +82,15 @@
    import pizzacutter
    pizzacutter.build(path_conf_file=pathlib.Path('./.../.../path_to_conf_file.py'))
 
 - Directory names and filenames can be templated. For example:
 
 .. code-block:: bash
 
-   {{\PizzaCutter.repo_name}}/{{\PizzaCutter.repo_name}}/{{\PizzaCutter.repo_name}}.py
+   {{PizzaCutter.repo_name}}/{{PizzaCutter.repo_name}}/{{PizzaCutter.repo_name}}.py
 
 - Supports unlimited levels of directory nesting. (beware of possible path length limitations, especially on Travis Windows builds)
 - 100% of templating is done with just (bytes) replace function. No Jinja2.
 
 Why PizzaCutter?
 ================
 
@@ -162,35 +165,35 @@
             # but can be useful to drop files on the desktop, /etc, and so on
             self.pizza_cutter_allow_outside_write = False
             self.pizza_cutter_dry_run = False
             self.pizza_cutter_quiet = False
 
     # User Section - do whatever You want here
     # Pizza Cutter Configuration, can override by cli options.
-    # You might name Your Patterns as You like {{\PizzaCutter. ... }}, {{LemonCutter. ... }}, {{MelonCutter. ... }}
-            self.pizza_cutter_patterns['{{\PizzaCutter.full_name}}'] = 'Robert Nowotny'
-            self.pizza_cutter_patterns['{{\PizzaCutter.email}}'] = 'bitranox@gmail.com'
-            self.pizza_cutter_patterns['{{\PizzaCutter.project.name}}'] = 'Complexity'
-            self.pizza_cutter_patterns['{{\PizzaCutter.project_short_description}}'] = 'Refreshingly simple static site generator.'
-            self.pizza_cutter_patterns['{{\PizzaCutter.release_date}}'] = '2013-07-10'
-            self.pizza_cutter_patterns['{{\PizzaCutter.year}}'] = '2013'
-            self.pizza_cutter_patterns['{{\PizzaCutter.current_version}}'] = '0.1.1'
+    # You might name Your Patterns as You like {{PizzaCutter. ... }}, {{LemonCutter. ... }}, {{MelonCutter. ... }}
+            self.pizza_cutter_patterns['{{PizzaCutter.full_name}}'] = 'Robert Nowotny'
+            self.pizza_cutter_patterns['{{PizzaCutter.email}}'] = 'bitranox@gmail.com'
+            self.pizza_cutter_patterns['{{PizzaCutter.project.name}}'] = 'Complexity'
+            self.pizza_cutter_patterns['{{PizzaCutter.project_short_description}}'] = 'Refreshingly simple static site generator.'
+            self.pizza_cutter_patterns['{{PizzaCutter.release_date}}'] = '2013-07-10'
+            self.pizza_cutter_patterns['{{PizzaCutter.year}}'] = '2013'
+            self.pizza_cutter_patterns['{{PizzaCutter.current_version}}'] = '0.1.1'
 
         self.set_defaults()
         self.set_patterns()
 
 well - that looks like a cookiecutter configuration, only a bit more complicated, so what is the difference ?
 In .XML Files You just can not program. What, if for instance You want to update the "release_date"
 to the current date automatically, every time You update Your project ?
 
 With Pizzacutter its easy :
 
 .. code-block:: python
 
-            self.pizza_cutter_patterns['{{\PizzaCutter.release_date}}'] = datetime.datetime.strptime(today, '%Y-%m-%d')
+            self.pizza_cutter_patterns['{{PizzaCutter.release_date}}'] = datetime.datetime.strptime(today, '%Y-%m-%d')
 
 This is where the flexibility starts - You can dynamically calculate and assign values in the config file.
 
 So easy, so effective, just use python for Your config.
 
 
 PizzaCutter is created and maintained with PizzaCutter !
@@ -241,15 +244,15 @@
 ----
 
 automated tests, Travis Matrix, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
 .com/bitranox/PizzaCutter>`_ (cookiecutter on steroids)
 
 Python version required: 3.6.0 or newer
 
-tested on linux "bionic" with python 3.6, 3.7, 3.8, 3.8-dev, pypy3 - architectures: amd64, ppc64le, s390x, arm64
+tested on linux "bionic" with python 3.6, 3.7, 3.8, 3.9-dev, pypy3 - architectures: amd64, ppc64le, s390x, arm64
 
 `100% code coverage <https://codecov.io/gh/bitranox/PizzaCutter>`_, flake8 style checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://travis-ci.org/bitranox/PizzaCutter>`_, automatic daily builds and monitoring
 
 ----
 
 - `Usage`_
 - `Usage from Commandline`_
@@ -458,14 +461,20 @@
 Changelog
 =========
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v1.1.9
+--------
+2020-10-09: service release
+    - update travis build matrix for linux 3.9-dev
+    - update travis build matrix (paths) for windows 3.9 / 3.10
+
 v1.1.8
 --------
 2020-08-08: service release
     - fix documentation
     - fix travis
     - deprecate pycodestyle
     - implement flake8
```

### Comparing `pizzacutter-1.1.8/pizzacutter/pizzacutter.py` & `pizzacutter-1.1.9/pizzacutter/pizzacutter.py`

 * *Files 5% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         Traceback (most recent call last):
         ...
         FileNotFoundError: the config file ... can not be found
 
         """
 
         if not path_conf_file.is_file():
-            raise FileNotFoundError('the config file "{}" can not be found'.format(path_conf_file))
+            raise FileNotFoundError(f'the config file "{path_conf_file}" can not be found')
 
         self.conf = get_config.PizzaCutterGetConfig(pizza_cutter_path_conf_file=path_conf_file,
                                                     pizza_cutter_path_template_dir=path_template_dir,
                                                     pizza_cutter_path_target_dir=path_target_dir).conf
 
         if path_template_dir is None:
             # we call again pathlib.Path, to be sure it is pathlib3x Type
@@ -139,15 +139,15 @@
         replace all the patterns in the source file
         it is already prepared for the function that You can include the content of other files into one file -
         we dont know if we will ever finish that idea, because we simply can make that replacement in the config file
         """
 
         # this is already preparation when we are able to include the content of other files
         if path_source_file in self.file_stack:                                                                     # pragma: no cover
-            raise RecursionError('Recursion on path includes : \n {}'.format(pprint.pformat(self.file_stack)))      # pragma: no cover
+            raise RecursionError(f'Recursion on path includes : \n {pprint.pformat(self.file_stack)}')              # pragma: no cover
         self.file_stack.append(path_source_file)
 
         # this is in preparation for the function if we can include the content of files into other files
         # because on included files you need to make all replacements before
 
         with open(str(path_source_file), 'rb') as f_source:
             source_line = f_source.readline()
@@ -255,17 +255,16 @@
         for pattern in self.conf.pizza_cutter_patterns.keys():
             replacement = self.conf.pizza_cutter_patterns[pattern]
             if isinstance(replacement, str):
                 self.resolve_str_patterns_recursive(pattern)
 
     def resolve_str_patterns_recursive(self, pattern: str) -> str:
         if pattern in self.pattern_stack:
-            raise RecursionError('"{last_entry}" refers back to "{pattern}"\n\nStack:\n{stack}'.format(stack=pprint.pformat(self.pattern_stack),
-                                                                                                       last_entry=self.pattern_stack[-1],
-                                                                                                       pattern=pattern))
+            raise RecursionError(f'"{self.pattern_stack[-1]}" refers back to "{pattern}"\n\nStack:\n{pprint.pformat(self.pattern_stack)}')
+
         self.pattern_stack.append(pattern)
 
         replacement = str(self.conf.pizza_cutter_patterns[pattern])
         for sub_pattern in self.conf.pizza_cutter_patterns.keys():
             if sub_pattern in replacement:
                 sub_replacement = self.resolve_str_patterns_recursive(sub_pattern)
                 replacement = replacement.replace(sub_pattern, sub_replacement)
@@ -404,18 +403,18 @@
             quiet = self.quiet
 
         if helpers.path_startswith(path_target_object, self.path_target_dir):
             return skip_outside_write
 
         if self.allow_outside_write:
             if self.dry_run:
-                logger.info('object outside project directory: "{}"'.format(path_target_object))
+                logger.info(f'object outside project directory: "{path_target_object}"')
             skip_outside_write = False
         else:
-            msg = 'object outside project directory not allowed: "{}"'.format(path_target_object)
+            msg = f'object outside project directory not allowed: "{path_target_object}"'
             if self.dry_run:
                 logger.info(msg)
             else:
                 if not quiet:
                     logger.warning(msg)
             skip_outside_write = True
 
@@ -426,19 +425,19 @@
 
         if self.conf.pizza_cutter_options['object_no_overwrite'] in str(path_source_object) and path_target_object.exists():
             return True
 
         if path_target_object.exists():
             if self.allow_overwrite:
                 if self.dry_run:
-                    logger.debug('object will be overwritten: "{}"'.format(path_target_object))
+                    logger.debug(f'object will be overwritten: "{path_target_object}"')
                 return False
             else:
                 if self.dry_run:
-                    logger.debug('object overwrite skipped, because allow_overwrite = False: "{}"'.format(path_target_object))
+                    logger.debug(f'object overwrite skipped, because allow_overwrite = False: "{path_target_object}"')
                 return True
         else:
             return False
 
     def log_unfilled_patterns(self) -> None:
 
         path_source_objects = self.get_path_template_objects()
@@ -489,21 +488,21 @@
         # we think a pattern never will be that long
         max_pattern_length = 160
         for pattern_prefix in self.conf.pizzacutter_pattern_prefixes:
             if not self.quiet:
                 for position in helpers.findall(pattern_prefix, str_path):
                     current_slice = str_path[position: position + max_pattern_length]
                     if '}}' not in current_slice:
-                        l_patterns.append('missing closing brackets for "{}"'.format(pattern_prefix))
+                        l_patterns.append(f'missing closing brackets for "{pattern_prefix}"')
                     else:
                         full_pattern = current_slice.split('}}', 1)[0] + '}}'
-                        l_patterns.append('unfilled pattern "{}"'.format(full_pattern))
+                        l_patterns.append(f'unfilled pattern "{full_pattern}"')
                 if l_patterns:
                     patterns = '\n'.join(l_patterns)
-                    logger.warning('unfilled or malformed patterns in filename "{str_path}": \n{patterns}'.format(str_path=str_path, patterns=patterns))
+                    logger.warning(f'unfilled or malformed patterns in filename "{str_path}": \n{patterns}')
         return l_patterns
 
     def log_unfilled_pattern_in_object(self, path_object: pathlib.Path) -> List[str]:
         """
         find unfilled patterns in the file contents.
         we search for bytes, because we dont know the encoding of the file
 
@@ -537,15 +536,15 @@
                         current_slice = b'{{' + current_slice[2:].split(b'{{', 1)[0].split(b'}', 1)[0]
                         l_patterns.append('missing closing brackets for "{}"'.format(current_slice.decode('utf-8')))
                     else:
                         full_pattern_bytes = current_slice.split(b'}}', 1)[0] + b'}}'
                         l_patterns.append('unfilled pattern "{}"'.format(full_pattern_bytes.decode('utf-8')))
             if l_patterns:
                 patterns = '\n'.join(l_patterns)
-                logger.warning('unfilled or malformed patterns in file "{path_object}": \n{patterns}'.format(path_object=path_object, patterns=patterns))
+                logger.warning(f'unfilled or malformed patterns in file "{path_object}": \n{patterns}')
         return l_patterns
 
     def path_remove_cutter_option_patterns(self, path_source_file: pathlib.Path) -> pathlib.Path:
         """
         removes option patterns from the filename - those are already checked and considered earlier
 
         >>> # Setup
@@ -578,15 +577,15 @@
         """
         source_file_parts = path_source_file.parts
         result_file_parts = list()
         for source_file_part in source_file_parts:
             for option_pattern in self.conf.pizza_cutter_options.values():
                 source_file_part = source_file_part.replace(option_pattern, '')
             if not source_file_part:
-                raise RuntimeError('No part of the path must consist ONLY of option patterns: "{}"'.format(path_source_file))
+                raise RuntimeError(f'No part of the path must consist ONLY of option patterns: "{path_source_file}"')
             result_file_parts.append(source_file_part)
         result_path_source_file = pathlib.Path(*result_file_parts)
         return result_path_source_file
 
     def get_path_target_object(self, path_source_object: pathlib.Path) -> pathlib.Path:
         path_source_object = self.path_replace_string_patterns(path_source_object)
         path_source_object = self.path_remove_cutter_option_patterns(path_source_object)
@@ -713,37 +712,35 @@
                 # we need this, because pathlib3x.Path is NOT instance of pathlib.Path,
                 # but the User might use pathlib in his config File !
                 if isinstance(replacement, str):
                     continue
                 if pattern in source_object_part:
                     if source_object_part != pattern:
                         raise RuntimeError(
-                            'pathlib.Path patterns can only be one complete part of a path : Path: "{path_source_file}", Pattern: {pattern}'.format(
-                                path_source_file=path_source_path, pattern=pattern))
+                            f'pathlib.Path patterns can only be one complete part of a path : Path: "{path_source_path}", Pattern: {pattern}'
+                            )
                     else:
                         target_object_part = pathlib.Path(replacement)
                         if target_object_part.is_absolute() and absolute_path_found:
                             logger.warning(
                                 'the resulting path might be unexpected, You have more then one absolute pathlib.Path pattern in the path: '
-                                '"{path_source_file}", Pattern: "{pattern}" points to "{replacement}"'.format(
-                                    path_source_file=path_source_path, pattern=pattern, replacement=replacement))
+                                f'"{path_source_path}", Pattern: "{pattern}" points to "{replacement}"')
 
             if not absolute_path_found:
                 target_parts.append(target_object_part)
                 if not isinstance(target_object_part, str) and pathlib.Path(target_object_part).is_absolute():
                     absolute_path_found = True
 
         target_parts = list(reversed(target_parts))
         path_target_path = pathlib.Path(*target_parts).resolve()
 
         if absolute_path_found:
             if not self.quiet:
                 logger.warning('the resulting path of a template file might be unexpected, You have an absolute pathlib.Path pattern in the path: '
-                               '"{path_source_path}" points to "{path_target_path}"'.format(path_source_path=path_source_path,
-                                                                                            path_target_path=path_target_path))
+                               f'"{path_source_path}" points to "{path_target_path}"')
         else:
             path_target_path = path_target_path.replace_parts(self.path_template_dir.resolve(), self.path_target_dir.resolve())
         return path_target_path
 
     def get_path_template_subdirs_with_pattern(self) -> List[pathlib.Path]:
         """
         get the template sub directories with a valid pattern in it - all other directories are considered not to be part of the template
```

### Comparing `pizzacutter-1.1.8/pizzacutter/pizzacutter_cli.py` & `pizzacutter-1.1.9/pizzacutter/pizzacutter_cli.py`

 * *Files identical despite different names*

### Comparing `pizzacutter-1.1.8/pizzacutter/sub/get_config.py` & `pizzacutter-1.1.9/pizzacutter/sub/get_config.py`

 * *Files identical despite different names*

### Comparing `pizzacutter-1.1.8/pizzacutter/sub/helpers.py` & `pizzacutter-1.1.9/pizzacutter/sub/helpers.py`

 * *Files identical despite different names*

### Comparing `pizzacutter-1.1.8/pizzacutter/sub/import_module.py` & `pizzacutter-1.1.9/pizzacutter/sub/import_module.py`

 * *Files identical despite different names*

### Comparing `pizzacutter-1.1.8/pizzacutter/sub/pizzacutter_config.py` & `pizzacutter-1.1.9/pizzacutter/sub/pizzacutter_config.py`

 * *Files identical despite different names*

### Comparing `pizzacutter-1.1.8/pizzacutter.egg-info/PKG-INFO` & `pizzacutter-1.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: pizzacutter
-Version: 1.1.8
+Version: 1.1.9
 Summary: create and update projects from project templates
 Home-page: https://github.com/bitranox/PizzaCutter
 Author: Robert Nowotny
 Author-email: bitranox@gmail.com
 License: UNKNOWN
 Description: PizzaCutter
         ===========
         
         
-        Version v1.1.8 as of 2020-08-08 see `Changelog`_
+        Version v1.1.9 as of 2020-10-09 see `Changelog`_
         
         |travis_build| |license| |pypi|
         
         |codecov| |better_code| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
         
         
         .. |travis_build| image:: https://img.shields.io/travis/bitranox/PizzaCutter/master.svg
@@ -47,14 +47,17 @@
         .. |cc_coverage| image:: https://img.shields.io/codeclimate/coverage/bitranox/PizzaCutter?label=CC%20coverage
            :target: https://codeclimate.com/github/bitranox/PizzaCutter/test_coverage
            :alt: Code Coverage
         
         .. |snyk| image:: https://img.shields.io/snyk/vulnerabilities/github/bitranox/PizzaCutter
            :target: https://snyk.io/test/github/bitranox/PizzaCutter
         
+        .. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
+           :target: https://github.com/psf/black
+        
         FUNCTION
         ========
         
         A command-line utility that creates and updates software projects in any language from PizzaCutter project templates.
         
         for the impatient, find here the latest PizzaCutter Templates:
             - `PizzaCutter default python template <https://github.com/bitranox/pct_python_default>`_
@@ -87,15 +90,15 @@
            import pizzacutter
            pizzacutter.build(path_conf_file=pathlib.Path('./.../.../path_to_conf_file.py'))
         
         - Directory names and filenames can be templated. For example:
         
         .. code-block:: bash
         
-           {{\PizzaCutter.repo_name}}/{{\PizzaCutter.repo_name}}/{{\PizzaCutter.repo_name}}.py
+           {{PizzaCutter.repo_name}}/{{PizzaCutter.repo_name}}/{{PizzaCutter.repo_name}}.py
         
         - Supports unlimited levels of directory nesting. (beware of possible path length limitations, especially on Travis Windows builds)
         - 100% of templating is done with just (bytes) replace function. No Jinja2.
         
         Why PizzaCutter?
         ================
         
@@ -170,35 +173,35 @@
                     # but can be useful to drop files on the desktop, /etc, and so on
                     self.pizza_cutter_allow_outside_write = False
                     self.pizza_cutter_dry_run = False
                     self.pizza_cutter_quiet = False
         
             # User Section - do whatever You want here
             # Pizza Cutter Configuration, can override by cli options.
-            # You might name Your Patterns as You like {{\PizzaCutter. ... }}, {{LemonCutter. ... }}, {{MelonCutter. ... }}
-                    self.pizza_cutter_patterns['{{\PizzaCutter.full_name}}'] = 'Robert Nowotny'
-                    self.pizza_cutter_patterns['{{\PizzaCutter.email}}'] = 'bitranox@gmail.com'
-                    self.pizza_cutter_patterns['{{\PizzaCutter.project.name}}'] = 'Complexity'
-                    self.pizza_cutter_patterns['{{\PizzaCutter.project_short_description}}'] = 'Refreshingly simple static site generator.'
-                    self.pizza_cutter_patterns['{{\PizzaCutter.release_date}}'] = '2013-07-10'
-                    self.pizza_cutter_patterns['{{\PizzaCutter.year}}'] = '2013'
-                    self.pizza_cutter_patterns['{{\PizzaCutter.current_version}}'] = '0.1.1'
+            # You might name Your Patterns as You like {{PizzaCutter. ... }}, {{LemonCutter. ... }}, {{MelonCutter. ... }}
+                    self.pizza_cutter_patterns['{{PizzaCutter.full_name}}'] = 'Robert Nowotny'
+                    self.pizza_cutter_patterns['{{PizzaCutter.email}}'] = 'bitranox@gmail.com'
+                    self.pizza_cutter_patterns['{{PizzaCutter.project.name}}'] = 'Complexity'
+                    self.pizza_cutter_patterns['{{PizzaCutter.project_short_description}}'] = 'Refreshingly simple static site generator.'
+                    self.pizza_cutter_patterns['{{PizzaCutter.release_date}}'] = '2013-07-10'
+                    self.pizza_cutter_patterns['{{PizzaCutter.year}}'] = '2013'
+                    self.pizza_cutter_patterns['{{PizzaCutter.current_version}}'] = '0.1.1'
         
                 self.set_defaults()
                 self.set_patterns()
         
         well - that looks like a cookiecutter configuration, only a bit more complicated, so what is the difference ?
         In .XML Files You just can not program. What, if for instance You want to update the "release_date"
         to the current date automatically, every time You update Your project ?
         
         With Pizzacutter its easy :
         
         .. code-block:: python
         
-                    self.pizza_cutter_patterns['{{\PizzaCutter.release_date}}'] = datetime.datetime.strptime(today, '%Y-%m-%d')
+                    self.pizza_cutter_patterns['{{PizzaCutter.release_date}}'] = datetime.datetime.strptime(today, '%Y-%m-%d')
         
         This is where the flexibility starts - You can dynamically calculate and assign values in the config file.
         
         So easy, so effective, just use python for Your config.
         
         
         PizzaCutter is created and maintained with PizzaCutter !
@@ -249,15 +252,15 @@
         ----
         
         automated tests, Travis Matrix, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
         .com/bitranox/PizzaCutter>`_ (cookiecutter on steroids)
         
         Python version required: 3.6.0 or newer
         
-        tested on linux "bionic" with python 3.6, 3.7, 3.8, 3.8-dev, pypy3 - architectures: amd64, ppc64le, s390x, arm64
+        tested on linux "bionic" with python 3.6, 3.7, 3.8, 3.9-dev, pypy3 - architectures: amd64, ppc64le, s390x, arm64
         
         `100% code coverage <https://codecov.io/gh/bitranox/PizzaCutter>`_, flake8 style checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://travis-ci.org/bitranox/PizzaCutter>`_, automatic daily builds and monitoring
         
         ----
         
         - `Usage`_
         - `Usage from Commandline`_
@@ -466,14 +469,20 @@
         Changelog
         =========
         
         - new MAJOR version for incompatible API changes,
         - new MINOR version for added functionality in a backwards compatible manner
         - new PATCH version for backwards compatible bug fixes
         
+        v1.1.9
+        --------
+        2020-10-09: service release
+            - update travis build matrix for linux 3.9-dev
+            - update travis build matrix (paths) for windows 3.9 / 3.10
+        
         v1.1.8
         --------
         2020-08-08: service release
             - fix documentation
             - fix travis
             - deprecate pycodestyle
             - implement flake8
```

### Comparing `pizzacutter-1.1.8/pizzacutter.egg-info/SOURCES.txt` & `pizzacutter-1.1.9/pizzacutter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pizzacutter-1.1.8/setup.cfg` & `pizzacutter-1.1.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `pizzacutter-1.1.8/setup.py` & `pizzacutter-1.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 if is_travis_deploy() and is_tagged_commit():
     setup_requires = strip_links_from_required(setup_requires)
     tests_require = strip_links_from_required(tests_require)
     install_requires = strip_links_from_required(install_requires)
 
 setup_kwargs: Dict[str, Any] = dict()
 setup_kwargs["name"] = "pizzacutter"
-setup_kwargs["version"] = "v1.1.8"
+setup_kwargs["version"] = "v1.1.9"
 setup_kwargs["url"] = "https://github.com/bitranox/PizzaCutter"
 setup_kwargs["packages"] = find_packages()
 setup_kwargs["package_data"] = {"pizzacutter": ["py.typed", "*.pyi", "__init__.pyi"]}
 setup_kwargs["description"] = "create and update projects from project templates"
 setup_kwargs["long_description"] = long_description
 setup_kwargs["long_description_content_type"] = "text/x-rst"
 setup_kwargs["author"] = "Robert Nowotny"
```

