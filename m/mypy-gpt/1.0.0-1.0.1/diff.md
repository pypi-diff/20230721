# Comparing `tmp/mypy-gpt-1.0.0.tar.gz` & `tmp/mypy-gpt-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-gpt-1.0.0.tar", last modified: Fri Jul 21 18:57:36 2023, max compression
+gzip compressed data, was "mypy-gpt-1.0.1.tar", last modified: Fri Jul 21 19:02:12 2023, max compression
```

## Comparing `mypy-gpt-1.0.0.tar` & `mypy-gpt-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-21 18:57:36.859271 mypy-gpt-1.0.0/
--rw-rw-rw-   0        0        0    35184 2023-07-21 03:02:01.000000 mypy-gpt-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      253 2023-07-21 18:57:36.858745 mypy-gpt-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     2181 2023-07-21 18:29:39.000000 mypy-gpt-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-21 18:57:36.849588 mypy-gpt-1.0.0/mypy_gpt/
--rw-rw-rw-   0        0        0        0 2023-07-21 18:55:16.000000 mypy-gpt-1.0.0/mypy_gpt/__init__.py
--rw-rw-rw-   0        0        0       33 2023-07-21 18:55:16.000000 mypy-gpt-1.0.0/mypy_gpt/__main__.py
--rw-rw-rw-   0        0        0     9926 2023-07-21 18:55:16.000000 mypy-gpt-1.0.0/mypy_gpt/mypygpt.py
-drwxrwxrwx   0        0        0        0 2023-07-21 18:57:36.857123 mypy-gpt-1.0.0/mypy_gpt.egg-info/
--rw-rw-rw-   0        0        0      253 2023-07-21 18:57:36.000000 mypy-gpt-1.0.0/mypy_gpt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      247 2023-07-21 18:57:36.000000 mypy-gpt-1.0.0/mypy_gpt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 18:57:36.000000 mypy-gpt-1.0.0/mypy_gpt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2023-07-21 18:57:36.000000 mypy-gpt-1.0.0/mypy_gpt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-21 18:57:36.000000 mypy-gpt-1.0.0/mypy_gpt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-21 18:57:36.859271 mypy-gpt-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      709 2023-07-21 18:55:16.000000 mypy-gpt-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 19:02:12.579358 mypy-gpt-1.0.1/
+-rw-rw-rw-   0        0        0    35184 2023-07-21 03:02:01.000000 mypy-gpt-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0      313 2023-07-21 19:02:12.578358 mypy-gpt-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2181 2023-07-21 18:29:39.000000 mypy-gpt-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-21 19:02:12.557356 mypy-gpt-1.0.1/mypy_gpt/
+-rw-rw-rw-   0        0        0        0 2023-07-21 18:55:16.000000 mypy-gpt-1.0.1/mypy_gpt/__init__.py
+-rw-rw-rw-   0        0        0       33 2023-07-21 18:55:16.000000 mypy-gpt-1.0.1/mypy_gpt/__main__.py
+-rw-rw-rw-   0        0        0     9926 2023-07-21 18:55:16.000000 mypy-gpt-1.0.1/mypy_gpt/mypygpt.py
+drwxrwxrwx   0        0        0        0 2023-07-21 19:02:12.577358 mypy-gpt-1.0.1/mypy_gpt.egg-info/
+-rw-rw-rw-   0        0        0      313 2023-07-21 19:02:12.000000 mypy-gpt-1.0.1/mypy_gpt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      247 2023-07-21 19:02:12.000000 mypy-gpt-1.0.1/mypy_gpt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 19:02:12.000000 mypy-gpt-1.0.1/mypy_gpt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2023-07-21 19:02:12.000000 mypy-gpt-1.0.1/mypy_gpt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-21 19:02:12.000000 mypy-gpt-1.0.1/mypy_gpt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-21 19:02:12.579358 mypy-gpt-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      748 2023-07-21 19:02:07.000000 mypy-gpt-1.0.1/setup.py
```

### Comparing `mypy-gpt-1.0.0/LICENSE` & `mypy-gpt-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-gpt-1.0.0/README.md` & `mypy-gpt-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `mypy-gpt-1.0.0/mypy_gpt/mypygpt.py` & `mypy-gpt-1.0.1/mypy_gpt/mypygpt.py`

 * *Files identical despite different names*

### Comparing `mypy-gpt-1.0.0/setup.py` & `mypy-gpt-1.0.1/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from setuptools import setup
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 import pkg_resources
 import setuptools
 import pathlib
-
+desc = 'Python minor issue resolver (mypy) using gpt by openai! '
 with pathlib.Path('requirements.txt').open() as requirements_txt:
     install_requires = [
         str(requirement)
         for requirement
         in pkg_resources.parse_requirements(requirements_txt)
     ]
 
 setup(
     name='mypy-gpt',
-    version='1.0.0',
+    version='1.0.1',
     packages=['mypy_gpt'],
     url='https://github.com/eyalk11/mypy-gpt',
     license=' AGPL-3.0 license',
     author='ekarni',
     author_email='',
-    description='Python minor issue resolver (mypy) using gpt by openai! ',
+    description=desc,
+    long_description=desc,
     install_requires=install_requires
 )
```

