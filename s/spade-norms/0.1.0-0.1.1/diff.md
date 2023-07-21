# Comparing `tmp/spade_norms-0.1.0.tar.gz` & `tmp/spade_norms-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spade_norms-0.1.0.tar", last modified: Wed Jul 12 10:55:58 2023, max compression
+gzip compressed data, was "spade_norms-0.1.1.tar", last modified: Fri Jul 21 10:04:05 2023, max compression
```

## Comparing `spade_norms-0.1.0.tar` & `spade_norms-0.1.1.tar`

### file list

```diff
@@ -1,55 +1,68 @@
-drwxr-xr-x   0 jpalanca   (501) staff       (20)        0 2023-07-12 10:55:58.115893 spade_norms-0.1.0/
--rw-r--r--   0 jpalanca   (501) staff       (20)      199 2023-07-12 10:53:47.000000 spade_norms-0.1.0/AUTHORS.rst
--rw-r--r--   0 jpalanca   (501) staff       (20)     3565 2023-05-16 08:35:59.000000 spade_norms-0.1.0/CONTRIBUTING.rst
--rw-r--r--   0 jpalanca   (501) staff       (20)       89 2023-07-12 10:53:58.000000 spade_norms-0.1.0/HISTORY.rst
--rw-r--r--   0 jpalanca   (501) staff       (20)     1071 2023-05-16 08:35:59.000000 spade_norms-0.1.0/LICENSE
--rw-r--r--   0 jpalanca   (501) staff       (20)      262 2023-05-16 08:35:59.000000 spade_norms-0.1.0/MANIFEST.in
--rw-r--r--   0 jpalanca   (501) staff       (20)     2563 2023-07-12 10:55:58.116150 spade_norms-0.1.0/PKG-INFO
--rw-r--r--   0 jpalanca   (501) staff       (20)     1621 2023-07-12 10:53:47.000000 spade_norms-0.1.0/README.rst
-drwxr-xr-x   0 jpalanca   (501) staff       (20)        0 2023-07-12 10:55:58.097824 spade_norms-0.1.0/docs/
--rw-r--r--   0 jpalanca   (501) staff       (20)      612 2023-05-16 08:35:59.000000 spade_norms-0.1.0/docs/Makefile
-drwxr-xr-x   0 jpalanca   (501) staff       (20)        0 2023-07-12 10:55:58.085857 spade_norms-0.1.0/docs/_build/
-drwxr-xr-x   0 jpalanca   (501) staff       (20)        0 2023-07-12 10:55:58.086013 spade_norms-0.1.0/docs/_build/html/
-drwxr-xr-x   0 jpalanca   (501) staff       (20)        0 2023-07-12 10:55:58.105303 spade_norms-0.1.0/docs/_build/html/_static/
--rw-r--r--   0 jpalanca   (501) staff       (20)      673 2023-07-12 10:36:49.000000 spade_norms-0.1.0/docs/_build/html/_static/ajax-loader.gif
--rw-r--r--   0 jpalanca   (501) staff       (20)      756 2023-07-12 10:36:49.000000 spade_norms-0.1.0/docs/_build/html/_static/comment-bright.png
--rw-r--r--   0 jpalanca   (501) staff       (20)      829 2023-07-12 10:36:49.000000 spade_norms-0.1.0/docs/_build/html/_static/comment-close.png
--rw-r--r--   0 jpalanca   (501) staff       (20)      641 2023-07-12 10:36:49.000000 spade_norms-0.1.0/docs/_build/html/_static/comment.png
--rw-r--r--   0 jpalanca   (501) staff       (20)      222 2023-07-12 10:36:49.000000 spade_norms-0.1.0/docs/_build/html/_static/down-pressed.png
--rw-r--r--   0 jpalanca   (501) staff       (20)      202 2023-07-12 10:36:49.000000 spade_norms-0.1.0/docs/_build/html/_static/down.png
--rw-r--r--   0 jpalanca   (501) staff       (20)      286 2023-07-12 10:36:49.000000 spade_norms-0.1.0/docs/_build/html/_static/file.png
--rw-r--r--   0 jpalanca   (501) staff       (20)       90 2023-07-12 10:36:49.000000 spade_norms-0.1.0/docs/_build/html/_static/minus.png
--rw-r--r--   0 jpalanca   (501) staff       (20)       90 2023-07-12 10:36:49.000000 spade_norms-0.1.0/docs/_build/html/_static/plus.png
--rw-r--r--   0 jpalanca   (501) staff       (20)      214 2023-07-12 10:36:49.000000 spade_norms-0.1.0/docs/_build/html/_static/up-pressed.png
--rw-r--r--   0 jpalanca   (501) staff       (20)      203 2023-07-12 10:36:49.000000 spade_norms-0.1.0/docs/_build/html/_static/up.png
--rw-r--r--   0 jpalanca   (501) staff       (20)       28 2023-05-16 08:35:59.000000 spade_norms-0.1.0/docs/authors.rst
--rwxr-xr-x   0 jpalanca   (501) staff       (20)     4837 2023-07-12 10:53:47.000000 spade_norms-0.1.0/docs/conf.py
--rw-r--r--   0 jpalanca   (501) staff       (20)       33 2023-05-16 08:35:59.000000 spade_norms-0.1.0/docs/contributing.rst
--rw-r--r--   0 jpalanca   (501) staff       (20)       28 2023-05-16 08:35:59.000000 spade_norms-0.1.0/docs/history.rst
--rw-r--r--   0 jpalanca   (501) staff       (20)      298 2023-07-12 10:53:47.000000 spade_norms-0.1.0/docs/index.rst
--rw-r--r--   0 jpalanca   (501) staff       (20)     1158 2023-05-16 08:35:59.000000 spade_norms-0.1.0/docs/installation.rst
--rw-r--r--   0 jpalanca   (501) staff       (20)      809 2023-05-16 08:35:59.000000 spade_norms-0.1.0/docs/make.bat
--rw-r--r--   0 jpalanca   (501) staff       (20)       70 2023-07-12 10:40:06.000000 spade_norms-0.1.0/docs/modules.rst
--rw-r--r--   0 jpalanca   (501) staff       (20)       27 2023-05-16 08:35:59.000000 spade_norms-0.1.0/docs/readme.rst
--rw-r--r--   0 jpalanca   (501) staff       (20)      350 2023-07-12 10:40:06.000000 spade_norms-0.1.0/docs/spade_norms.rst
--rw-r--r--   0 jpalanca   (501) staff       (20)     7471 2023-07-12 10:53:47.000000 spade_norms-0.1.0/docs/usage.rst
--rw-r--r--   0 jpalanca   (501) staff       (20)      428 2023-07-12 10:55:58.117382 spade_norms-0.1.0/setup.cfg
--rw-r--r--   0 jpalanca   (501) staff       (20)     1732 2023-05-16 08:41:00.000000 spade_norms-0.1.0/setup.py
-drwxr-xr-x   0 jpalanca   (501) staff       (20)        0 2023-07-12 10:55:58.106634 spade_norms-0.1.0/spade_norms/
--rw-r--r--   0 jpalanca   (501) staff       (20)      235 2023-07-12 10:53:47.000000 spade_norms-0.1.0/spade_norms/__init__.py
--rw-r--r--   0 jpalanca   (501) staff       (20)     4225 2023-07-12 10:53:47.000000 spade_norms-0.1.0/spade_norms/spade_norms.py
-drwxr-xr-x   0 jpalanca   (501) staff       (20)        0 2023-07-12 10:55:58.110564 spade_norms-0.1.0/spade_norms.egg-info/
--rw-r--r--   0 jpalanca   (501) staff       (20)     2563 2023-07-12 10:55:57.000000 spade_norms-0.1.0/spade_norms.egg-info/PKG-INFO
--rw-r--r--   0 jpalanca   (501) staff       (20)     1133 2023-07-12 10:55:58.000000 spade_norms-0.1.0/spade_norms.egg-info/SOURCES.txt
--rw-r--r--   0 jpalanca   (501) staff       (20)        1 2023-07-12 10:55:57.000000 spade_norms-0.1.0/spade_norms.egg-info/dependency_links.txt
--rw-r--r--   0 jpalanca   (501) staff       (20)        1 2023-07-12 10:55:57.000000 spade_norms-0.1.0/spade_norms.egg-info/not-zip-safe
--rw-r--r--   0 jpalanca   (501) staff       (20)      673 2023-07-12 10:55:57.000000 spade_norms-0.1.0/spade_norms.egg-info/requires.txt
--rw-r--r--   0 jpalanca   (501) staff       (20)       12 2023-07-12 10:55:57.000000 spade_norms-0.1.0/spade_norms.egg-info/top_level.txt
-drwxr-xr-x   0 jpalanca   (501) staff       (20)        0 2023-07-12 10:55:58.115339 spade_norms-0.1.0/tests/
--rw-r--r--   0 jpalanca   (501) staff       (20)       41 2023-05-16 08:35:59.000000 spade_norms-0.1.0/tests/__init__.py
--rw-r--r--   0 jpalanca   (501) staff       (20)      140 2023-07-12 10:53:47.000000 spade_norms-0.1.0/tests/conftest.py
--rw-r--r--   0 jpalanca   (501) staff       (20)      391 2023-07-12 10:53:47.000000 spade_norms-0.1.0/tests/factories.py
--rw-r--r--   0 jpalanca   (501) staff       (20)    13786 2023-07-12 10:53:47.000000 spade_norms-0.1.0/tests/test_norm_engine.py
--rw-r--r--   0 jpalanca   (501) staff       (20)     7577 2023-07-12 10:53:47.000000 spade_norms-0.1.0/tests/test_norm_utils.py
--rw-r--r--   0 jpalanca   (501) staff       (20)     6686 2023-07-12 10:53:47.000000 spade_norms-0.1.0/tests/test_normative_response.py
--rw-r--r--   0 jpalanca   (501) staff       (20)      895 2023-07-12 10:53:47.000000 spade_norms-0.1.0/tests/test_spade_norms.py
+drwxr-xr-x   0 jpalanca   (501) staff       (20)        0 2023-07-21 10:04:05.949314 spade_norms-0.1.1/
+-rw-r--r--   0 jpalanca   (501) staff       (20)      199 2023-07-12 10:53:47.000000 spade_norms-0.1.1/AUTHORS.rst
+-rw-r--r--   0 jpalanca   (501) staff       (20)     3565 2023-05-16 08:35:59.000000 spade_norms-0.1.1/CONTRIBUTING.rst
+-rw-r--r--   0 jpalanca   (501) staff       (20)      149 2023-07-21 10:03:26.000000 spade_norms-0.1.1/HISTORY.rst
+-rw-r--r--   0 jpalanca   (501) staff       (20)     1071 2023-05-16 08:35:59.000000 spade_norms-0.1.1/LICENSE
+-rw-r--r--   0 jpalanca   (501) staff       (20)      262 2023-05-16 08:35:59.000000 spade_norms-0.1.1/MANIFEST.in
+-rw-r--r--   0 jpalanca   (501) staff       (20)     2724 2023-07-21 10:04:05.949565 spade_norms-0.1.1/PKG-INFO
+-rw-r--r--   0 jpalanca   (501) staff       (20)     1621 2023-07-12 10:53:47.000000 spade_norms-0.1.1/README.rst
+drwxr-xr-x   0 jpalanca   (501) staff       (20)        0 2023-07-21 10:04:05.919788 spade_norms-0.1.1/docs/
+-rw-r--r--   0 jpalanca   (501) staff       (20)      612 2023-05-16 08:35:59.000000 spade_norms-0.1.1/docs/Makefile
+drwxr-xr-x   0 jpalanca   (501) staff       (20)        0 2023-07-21 10:04:05.905454 spade_norms-0.1.1/docs/_build/
+drwxr-xr-x   0 jpalanca   (501) staff       (20)        0 2023-07-21 10:04:05.905619 spade_norms-0.1.1/docs/_build/html/
+drwxr-xr-x   0 jpalanca   (501) staff       (20)        0 2023-07-21 10:04:05.929718 spade_norms-0.1.1/docs/_build/html/_static/
+-rw-r--r--   0 jpalanca   (501) staff       (20)      673 2023-07-12 10:36:49.000000 spade_norms-0.1.1/docs/_build/html/_static/ajax-loader.gif
+-rw-r--r--   0 jpalanca   (501) staff       (20)      756 2023-07-12 10:36:49.000000 spade_norms-0.1.1/docs/_build/html/_static/comment-bright.png
+-rw-r--r--   0 jpalanca   (501) staff       (20)      829 2023-07-12 10:36:49.000000 spade_norms-0.1.1/docs/_build/html/_static/comment-close.png
+-rw-r--r--   0 jpalanca   (501) staff       (20)      641 2023-07-12 10:36:49.000000 spade_norms-0.1.1/docs/_build/html/_static/comment.png
+-rw-r--r--   0 jpalanca   (501) staff       (20)      222 2023-07-12 10:36:49.000000 spade_norms-0.1.1/docs/_build/html/_static/down-pressed.png
+-rw-r--r--   0 jpalanca   (501) staff       (20)      202 2023-07-12 10:36:49.000000 spade_norms-0.1.1/docs/_build/html/_static/down.png
+-rw-r--r--   0 jpalanca   (501) staff       (20)      286 2023-07-12 10:36:49.000000 spade_norms-0.1.1/docs/_build/html/_static/file.png
+-rw-r--r--   0 jpalanca   (501) staff       (20)       90 2023-07-12 10:36:49.000000 spade_norms-0.1.1/docs/_build/html/_static/minus.png
+-rw-r--r--   0 jpalanca   (501) staff       (20)       90 2023-07-12 10:36:49.000000 spade_norms-0.1.1/docs/_build/html/_static/plus.png
+-rw-r--r--   0 jpalanca   (501) staff       (20)      214 2023-07-12 10:36:49.000000 spade_norms-0.1.1/docs/_build/html/_static/up-pressed.png
+-rw-r--r--   0 jpalanca   (501) staff       (20)      203 2023-07-12 10:36:49.000000 spade_norms-0.1.1/docs/_build/html/_static/up.png
+-rw-r--r--   0 jpalanca   (501) staff       (20)       28 2023-05-16 08:35:59.000000 spade_norms-0.1.1/docs/authors.rst
+-rwxr-xr-x   0 jpalanca   (501) staff       (20)     4837 2023-07-12 10:53:47.000000 spade_norms-0.1.1/docs/conf.py
+-rw-r--r--   0 jpalanca   (501) staff       (20)       33 2023-05-16 08:35:59.000000 spade_norms-0.1.1/docs/contributing.rst
+-rw-r--r--   0 jpalanca   (501) staff       (20)       28 2023-05-16 08:35:59.000000 spade_norms-0.1.1/docs/history.rst
+-rw-r--r--   0 jpalanca   (501) staff       (20)      298 2023-07-12 10:53:47.000000 spade_norms-0.1.1/docs/index.rst
+-rw-r--r--   0 jpalanca   (501) staff       (20)     1158 2023-05-16 08:35:59.000000 spade_norms-0.1.1/docs/installation.rst
+-rw-r--r--   0 jpalanca   (501) staff       (20)      809 2023-05-16 08:35:59.000000 spade_norms-0.1.1/docs/make.bat
+-rw-r--r--   0 jpalanca   (501) staff       (20)       70 2023-07-12 10:40:06.000000 spade_norms-0.1.1/docs/modules.rst
+-rw-r--r--   0 jpalanca   (501) staff       (20)       27 2023-05-16 08:35:59.000000 spade_norms-0.1.1/docs/readme.rst
+-rw-r--r--   0 jpalanca   (501) staff       (20)      350 2023-07-12 10:40:06.000000 spade_norms-0.1.1/docs/spade_norms.rst
+-rw-r--r--   0 jpalanca   (501) staff       (20)     7471 2023-07-12 10:53:47.000000 spade_norms-0.1.1/docs/usage.rst
+-rw-r--r--   0 jpalanca   (501) staff       (20)      428 2023-07-21 10:04:05.950984 spade_norms-0.1.1/setup.cfg
+-rw-r--r--   0 jpalanca   (501) staff       (20)     1831 2023-07-21 10:03:26.000000 spade_norms-0.1.1/setup.py
+drwxr-xr-x   0 jpalanca   (501) staff       (20)        0 2023-07-21 10:04:05.931254 spade_norms-0.1.1/spade_norms/
+-rw-r--r--   0 jpalanca   (501) staff       (20)      243 2023-07-21 10:03:26.000000 spade_norms-0.1.1/spade_norms/__init__.py
+drwxr-xr-x   0 jpalanca   (501) staff       (20)        0 2023-07-21 10:04:05.936847 spade_norms-0.1.1/spade_norms/actions/
+-rw-r--r--   0 jpalanca   (501) staff       (20)        0 2023-07-21 10:03:19.000000 spade_norms-0.1.1/spade_norms/actions/__init__.py
+-rw-r--r--   0 jpalanca   (501) staff       (20)      244 2023-07-12 10:53:47.000000 spade_norms-0.1.1/spade_norms/actions/normative_action.py
+drwxr-xr-x   0 jpalanca   (501) staff       (20)        0 2023-07-21 10:04:05.938737 spade_norms-0.1.1/spade_norms/engines/
+-rw-r--r--   0 jpalanca   (501) staff       (20)        0 2023-07-21 10:03:19.000000 spade_norms-0.1.1/spade_norms/engines/__init__.py
+-rw-r--r--   0 jpalanca   (501) staff       (20)     2808 2023-07-12 10:53:47.000000 spade_norms-0.1.1/spade_norms/engines/norm_engine.py
+-rw-r--r--   0 jpalanca   (501) staff       (20)      812 2023-07-12 10:53:47.000000 spade_norms-0.1.1/spade_norms/engines/reasoning_engine.py
+drwxr-xr-x   0 jpalanca   (501) staff       (20)        0 2023-07-21 10:04:05.943088 spade_norms-0.1.1/spade_norms/norms/
+-rw-r--r--   0 jpalanca   (501) staff       (20)        0 2023-07-21 10:03:19.000000 spade_norms-0.1.1/spade_norms/norms/__init__.py
+-rw-r--r--   0 jpalanca   (501) staff       (20)     1195 2023-07-12 10:53:47.000000 spade_norms-0.1.1/spade_norms/norms/norm.py
+-rw-r--r--   0 jpalanca   (501) staff       (20)      436 2023-07-12 10:53:47.000000 spade_norms-0.1.1/spade_norms/norms/norm_enums.py
+-rw-r--r--   0 jpalanca   (501) staff       (20)     2943 2023-07-12 10:53:47.000000 spade_norms-0.1.1/spade_norms/norms/norm_utils.py
+-rw-r--r--   0 jpalanca   (501) staff       (20)     2372 2023-07-12 10:53:47.000000 spade_norms-0.1.1/spade_norms/norms/normative_response.py
+-rw-r--r--   0 jpalanca   (501) staff       (20)     4225 2023-07-12 10:53:47.000000 spade_norms-0.1.1/spade_norms/spade_norms.py
+drwxr-xr-x   0 jpalanca   (501) staff       (20)        0 2023-07-21 10:04:05.935393 spade_norms-0.1.1/spade_norms.egg-info/
+-rw-r--r--   0 jpalanca   (501) staff       (20)     2724 2023-07-21 10:04:05.000000 spade_norms-0.1.1/spade_norms.egg-info/PKG-INFO
+-rw-r--r--   0 jpalanca   (501) staff       (20)     1472 2023-07-21 10:04:05.000000 spade_norms-0.1.1/spade_norms.egg-info/SOURCES.txt
+-rw-r--r--   0 jpalanca   (501) staff       (20)        1 2023-07-21 10:04:05.000000 spade_norms-0.1.1/spade_norms.egg-info/dependency_links.txt
+-rw-r--r--   0 jpalanca   (501) staff       (20)        1 2023-07-21 10:04:05.000000 spade_norms-0.1.1/spade_norms.egg-info/not-zip-safe
+-rw-r--r--   0 jpalanca   (501) staff       (20)      673 2023-07-21 10:04:05.000000 spade_norms-0.1.1/spade_norms.egg-info/requires.txt
+-rw-r--r--   0 jpalanca   (501) staff       (20)       12 2023-07-21 10:04:05.000000 spade_norms-0.1.1/spade_norms.egg-info/top_level.txt
+drwxr-xr-x   0 jpalanca   (501) staff       (20)        0 2023-07-21 10:04:05.948759 spade_norms-0.1.1/tests/
+-rw-r--r--   0 jpalanca   (501) staff       (20)       41 2023-05-16 08:35:59.000000 spade_norms-0.1.1/tests/__init__.py
+-rw-r--r--   0 jpalanca   (501) staff       (20)      140 2023-07-12 10:53:47.000000 spade_norms-0.1.1/tests/conftest.py
+-rw-r--r--   0 jpalanca   (501) staff       (20)      391 2023-07-12 10:53:47.000000 spade_norms-0.1.1/tests/factories.py
+-rw-r--r--   0 jpalanca   (501) staff       (20)    13786 2023-07-12 10:53:47.000000 spade_norms-0.1.1/tests/test_norm_engine.py
+-rw-r--r--   0 jpalanca   (501) staff       (20)     7577 2023-07-12 10:53:47.000000 spade_norms-0.1.1/tests/test_norm_utils.py
+-rw-r--r--   0 jpalanca   (501) staff       (20)     6686 2023-07-12 10:53:47.000000 spade_norms-0.1.1/tests/test_normative_response.py
+-rw-r--r--   0 jpalanca   (501) staff       (20)      895 2023-07-12 10:53:47.000000 spade_norms-0.1.1/tests/test_spade_norms.py
```

### Comparing `spade_norms-0.1.0/CONTRIBUTING.rst` & `spade_norms-0.1.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `spade_norms-0.1.0/LICENSE` & `spade_norms-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `spade_norms-0.1.0/PKG-INFO` & `spade_norms-0.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: spade_norms
-Version: 0.1.0
+Version: 0.1.1
 Summary: SPADE Normative Plugin
 Home-page: https://github.com/javipalanca/spade_norms
 Author: Javi Palanca
 Author-email: jpalanca@dsic.upv.es
 License: MIT license
 Keywords: spade_norms
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Internet :: XMPP
 Requires-Python: >=3.8
 License-File: LICENSE
@@ -76,11 +78,16 @@
 Installation and debug of plugin: https://stackoverflow.com/a/19048754
 
 
 =======
 History
 =======
 
+0.1.1 (2023-07-21)
+------------------
+
+* Fixed import bug.
+
 0.1.0 (2023-07-12)
 ------------------
 
 * First release on PyPI.
```

### Comparing `spade_norms-0.1.0/README.rst` & `spade_norms-0.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `spade_norms-0.1.0/docs/Makefile` & `spade_norms-0.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `spade_norms-0.1.0/docs/_build/html/_static/ajax-loader.gif` & `spade_norms-0.1.1/docs/_build/html/_static/ajax-loader.gif`

 * *Files identical despite different names*

### Comparing `spade_norms-0.1.0/docs/_build/html/_static/comment-bright.png` & `spade_norms-0.1.1/docs/_build/html/_static/comment-bright.png`

 * *Files identical despite different names*

### Comparing `spade_norms-0.1.0/docs/_build/html/_static/comment-close.png` & `spade_norms-0.1.1/docs/_build/html/_static/comment-close.png`

 * *Files identical despite different names*

### Comparing `spade_norms-0.1.0/docs/_build/html/_static/comment.png` & `spade_norms-0.1.1/docs/_build/html/_static/comment.png`

 * *Files identical despite different names*

### Comparing `spade_norms-0.1.0/docs/conf.py` & `spade_norms-0.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `spade_norms-0.1.0/docs/installation.rst` & `spade_norms-0.1.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `spade_norms-0.1.0/docs/make.bat` & `spade_norms-0.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `spade_norms-0.1.0/docs/usage.rst` & `spade_norms-0.1.1/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `spade_norms-0.1.0/setup.py` & `spade_norms-0.1.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -29,14 +29,16 @@
     classifiers=[
         'Development Status :: 2 - Pre-Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Natural Language :: English',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
         'Operating System :: MacOS :: MacOS X',
         'Operating System :: POSIX :: Linux',
         'Operating System :: Microsoft :: Windows',
         'Topic :: Scientific/Engineering :: Artificial Intelligence',
         'Topic :: Internet :: XMPP',
     ],
     description="SPADE Normative Plugin",
@@ -46,10 +48,10 @@
     include_package_data=True,
     keywords='spade_norms',
     name='spade_norms',
     packages=find_packages(include=['spade_norms', 'spade_norms.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/javipalanca/spade_norms',
-    version='0.1.0',
+    version='0.1.1',
     zip_safe=False,
 )
```

### Comparing `spade_norms-0.1.0/spade_norms/spade_norms.py` & `spade_norms-0.1.1/spade_norms/spade_norms.py`

 * *Files identical despite different names*

### Comparing `spade_norms-0.1.0/spade_norms.egg-info/PKG-INFO` & `spade_norms-0.1.1/spade_norms.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: spade-norms
-Version: 0.1.0
+Version: 0.1.1
 Summary: SPADE Normative Plugin
 Home-page: https://github.com/javipalanca/spade_norms
 Author: Javi Palanca
 Author-email: jpalanca@dsic.upv.es
 License: MIT license
 Keywords: spade_norms
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Internet :: XMPP
 Requires-Python: >=3.8
 License-File: LICENSE
@@ -76,11 +78,16 @@
 Installation and debug of plugin: https://stackoverflow.com/a/19048754
 
 
 =======
 History
 =======
 
+0.1.1 (2023-07-21)
+------------------
+
+* Fixed import bug.
+
 0.1.0 (2023-07-12)
 ------------------
 
 * First release on PyPI.
```

### Comparing `spade_norms-0.1.0/spade_norms.egg-info/SOURCES.txt` & `spade_norms-0.1.1/spade_norms.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -33,14 +33,24 @@
 spade_norms/spade_norms.py
 spade_norms.egg-info/PKG-INFO
 spade_norms.egg-info/SOURCES.txt
 spade_norms.egg-info/dependency_links.txt
 spade_norms.egg-info/not-zip-safe
 spade_norms.egg-info/requires.txt
 spade_norms.egg-info/top_level.txt
+spade_norms/actions/__init__.py
+spade_norms/actions/normative_action.py
+spade_norms/engines/__init__.py
+spade_norms/engines/norm_engine.py
+spade_norms/engines/reasoning_engine.py
+spade_norms/norms/__init__.py
+spade_norms/norms/norm.py
+spade_norms/norms/norm_enums.py
+spade_norms/norms/norm_utils.py
+spade_norms/norms/normative_response.py
 tests/__init__.py
 tests/conftest.py
 tests/factories.py
 tests/test_norm_engine.py
 tests/test_norm_utils.py
 tests/test_normative_response.py
 tests/test_spade_norms.py
```

### Comparing `spade_norms-0.1.0/spade_norms.egg-info/requires.txt` & `spade_norms-0.1.1/spade_norms.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `spade_norms-0.1.0/tests/test_norm_engine.py` & `spade_norms-0.1.1/tests/test_norm_engine.py`

 * *Files identical despite different names*

### Comparing `spade_norms-0.1.0/tests/test_norm_utils.py` & `spade_norms-0.1.1/tests/test_norm_utils.py`

 * *Files identical despite different names*

### Comparing `spade_norms-0.1.0/tests/test_normative_response.py` & `spade_norms-0.1.1/tests/test_normative_response.py`

 * *Files identical despite different names*

### Comparing `spade_norms-0.1.0/tests/test_spade_norms.py` & `spade_norms-0.1.1/tests/test_spade_norms.py`

 * *Files identical despite different names*

