# Comparing `tmp/ndtorch-0.1.5.tar.gz` & `tmp/ndtorch-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ndtorch-0.1.5.tar", last modified: Thu Jun 29 07:12:19 2023, max compression
+gzip compressed data, was "ndtorch-0.1.6.tar", last modified: Fri Jul 21 09:19:37 2023, max compression
```

## Comparing `ndtorch-0.1.5.tar` & `ndtorch-0.1.6.tar`

### file list

```diff
@@ -1,64 +1,72 @@
-drwxrwxr-x   0 imorozov  (1000) imorozov  (1000)        0 2023-06-29 07:12:19.975473 ndtorch-0.1.5/
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     1822 2023-06-01 15:51:48.000000 ndtorch-0.1.5/.gitignore
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)      152 2023-05-23 16:04:29.000000 ndtorch-0.1.5/.readthedocs.yml
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     1069 2023-05-23 16:04:29.000000 ndtorch-0.1.5/LICENSE
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     2601 2023-06-29 07:12:19.971473 ndtorch-0.1.5/PKG-INFO
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     2115 2023-06-11 14:21:22.000000 ndtorch-0.1.5/README.MD
-drwxrwxr-x   0 imorozov  (1000) imorozov  (1000)        0 2023-06-29 07:12:19.879475 ndtorch-0.1.5/docs/
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)      638 2023-05-23 16:04:29.000000 ndtorch-0.1.5/docs/Makefile
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)      804 2023-05-23 16:04:29.000000 ndtorch-0.1.5/docs/make.bat
-drwxrwxr-x   0 imorozov  (1000) imorozov  (1000)        0 2023-06-29 07:12:19.911474 ndtorch-0.1.5/docs/pics/
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)  1376301 2023-05-25 16:59:32.000000 ndtorch-0.1.5/docs/pics/change.gif
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)  1239706 2023-05-24 09:08:54.000000 ndtorch-0.1.5/docs/pics/collision.gif
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)    92012 2023-05-25 15:47:52.000000 ndtorch-0.1.5/docs/pics/logo.svg
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)  2852797 2023-05-25 15:55:45.000000 ndtorch-0.1.5/docs/pics/manifold.gif
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       43 2023-06-27 06:09:15.000000 ndtorch-0.1.5/docs/requirements.txt
-drwxrwxr-x   0 imorozov  (1000) imorozov  (1000)        0 2023-06-29 07:12:19.939474 ndtorch-0.1.5/docs/source/
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     2195 2023-05-25 16:17:36.000000 ndtorch-0.1.5/docs/source/conf.py
-drwxrwxr-x   0 imorozov  (1000) imorozov  (1000)        0 2023-06-29 07:12:19.939474 ndtorch-0.1.5/docs/source/examples/
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)  2104809 2023-06-29 07:07:45.000000 ndtorch-0.1.5/docs/source/examples/ndtorch.ipynb
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     1101 2023-06-29 07:10:23.000000 ndtorch-0.1.5/docs/source/index.rst
-drwxrwxr-x   0 imorozov  (1000) imorozov  (1000)        0 2023-06-29 07:12:19.967473 ndtorch-0.1.5/docs/source/modules/
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       45 2023-06-10 05:03:33.000000 ndtorch-0.1.5/docs/source/modules/bracket.rst
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       48 2023-05-23 16:04:29.000000 ndtorch-0.1.5/docs/source/modules/derivative.rst
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       46 2023-05-23 16:04:29.000000 ndtorch-0.1.5/docs/source/modules/evaluate.rst
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       43 2023-05-23 16:04:29.000000 ndtorch-0.1.5/docs/source/modules/index.rst
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       47 2023-06-15 05:00:31.000000 ndtorch-0.1.5/docs/source/modules/invariant.rst
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       46 2023-06-28 11:54:29.000000 ndtorch-0.1.5/docs/source/modules/inverse.rst
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       41 2023-05-23 16:04:29.000000 ndtorch-0.1.5/docs/source/modules/jet.rst
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       45 2023-06-18 09:03:15.000000 ndtorch-0.1.5/docs/source/modules/matrix.rst
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       46 2023-06-29 07:09:51.000000 ndtorch-0.1.5/docs/source/modules/momenta.rst
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       41 2023-05-23 16:04:29.000000 ndtorch-0.1.5/docs/source/modules/pfp.rst
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       47 2023-05-23 16:04:29.000000 ndtorch-0.1.5/docs/source/modules/propagate.rst
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       44 2023-05-23 16:04:29.000000 ndtorch-0.1.5/docs/source/modules/series.rst
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       47 2023-05-23 16:04:29.000000 ndtorch-0.1.5/docs/source/modules/signature.rst
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       44 2023-06-10 05:03:41.000000 ndtorch-0.1.5/docs/source/modules/taylor.rst
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       42 2023-05-23 16:04:29.000000 ndtorch-0.1.5/docs/source/modules/util.rst
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       46 2023-06-13 06:47:51.000000 ndtorch-0.1.5/docs/source/modules/yoshida.rst
-drwxrwxr-x   0 imorozov  (1000) imorozov  (1000)        0 2023-06-29 07:12:19.971473 ndtorch-0.1.5/ndtorch/
--rwxrwxr-x   0 imorozov  (1000) imorozov  (1000)     8386 2023-06-03 15:36:07.000000 ndtorch-0.1.5/ndtorch/__init__.py
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     5471 2023-06-11 13:21:51.000000 ndtorch-0.1.5/ndtorch/bracket.py
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     6864 2023-06-04 06:09:17.000000 ndtorch-0.1.5/ndtorch/derivative.py
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     7561 2023-06-11 10:21:16.000000 ndtorch-0.1.5/ndtorch/evaluate.py
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)    13530 2023-06-22 08:11:21.000000 ndtorch-0.1.5/ndtorch/index.py
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)    11066 2023-06-28 05:43:18.000000 ndtorch-0.1.5/ndtorch/invariant.py
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     5352 2023-06-28 12:02:11.000000 ndtorch-0.1.5/ndtorch/inverse.py
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)    22836 2023-06-04 06:10:00.000000 ndtorch-0.1.5/ndtorch/jet.py
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)      655 2023-06-18 09:02:20.000000 ndtorch-0.1.5/ndtorch/matrix.py
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     7597 2023-06-29 07:07:53.000000 ndtorch-0.1.5/ndtorch/momenta.py
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)    17135 2023-06-22 08:39:42.000000 ndtorch-0.1.5/ndtorch/pfp.py
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)    10182 2023-06-27 07:55:00.000000 ndtorch-0.1.5/ndtorch/propagate.py
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)    11455 2023-06-22 08:12:53.000000 ndtorch-0.1.5/ndtorch/series.py
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     9333 2023-06-16 14:18:00.000000 ndtorch-0.1.5/ndtorch/signature.py
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     2875 2023-06-15 14:15:13.000000 ndtorch-0.1.5/ndtorch/taylor.py
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     7023 2023-06-22 08:02:24.000000 ndtorch-0.1.5/ndtorch/util.py
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)    11084 2023-06-15 05:20:19.000000 ndtorch-0.1.5/ndtorch/yoshida.py
-drwxrwxr-x   0 imorozov  (1000) imorozov  (1000)        0 2023-06-29 07:12:19.971473 ndtorch-0.1.5/ndtorch.egg-info/
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     2601 2023-06-29 07:12:19.000000 ndtorch-0.1.5/ndtorch.egg-info/PKG-INFO
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     1266 2023-06-29 07:12:19.000000 ndtorch-0.1.5/ndtorch.egg-info/SOURCES.txt
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)        1 2023-06-29 07:12:19.000000 ndtorch-0.1.5/ndtorch.egg-info/dependency_links.txt
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)      143 2023-06-29 07:12:19.000000 ndtorch-0.1.5/ndtorch.egg-info/requires.txt
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)        8 2023-06-29 07:12:19.000000 ndtorch-0.1.5/ndtorch.egg-info/top_level.txt
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)  2104809 2023-06-29 07:07:45.000000 ndtorch-0.1.5/ndtorch.ipynb
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)      745 2023-06-29 07:11:32.000000 ndtorch-0.1.5/pyproject.toml
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       38 2023-06-29 07:12:19.975473 ndtorch-0.1.5/setup.cfg
+drwxrwxr-x   0 imorozov  (1000) imorozov  (1000)        0 2023-07-21 09:19:37.495003 ndtorch-0.1.6/
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     1822 2023-06-01 15:51:48.000000 ndtorch-0.1.6/.gitignore
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)      152 2023-05-23 16:04:29.000000 ndtorch-0.1.6/.readthedocs.yml
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     1069 2023-05-23 16:04:29.000000 ndtorch-0.1.6/LICENSE
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     3952 2023-07-21 09:19:37.495003 ndtorch-0.1.6/PKG-INFO
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     3466 2023-07-21 09:15:04.000000 ndtorch-0.1.6/README.MD
+drwxrwxr-x   0 imorozov  (1000) imorozov  (1000)        0 2023-07-21 09:19:37.391003 ndtorch-0.1.6/docs/
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)      638 2023-05-23 16:04:29.000000 ndtorch-0.1.6/docs/Makefile
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)      804 2023-05-23 16:04:29.000000 ndtorch-0.1.6/docs/make.bat
+drwxrwxr-x   0 imorozov  (1000) imorozov  (1000)        0 2023-07-21 09:19:37.427003 ndtorch-0.1.6/docs/pics/
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)  1376301 2023-05-25 16:59:32.000000 ndtorch-0.1.6/docs/pics/change.gif
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)  1239706 2023-05-24 09:08:54.000000 ndtorch-0.1.6/docs/pics/collision.gif
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)    92012 2023-05-25 15:47:52.000000 ndtorch-0.1.6/docs/pics/logo.svg
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)  2852797 2023-05-25 15:55:45.000000 ndtorch-0.1.6/docs/pics/manifold.gif
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       43 2023-06-27 06:09:15.000000 ndtorch-0.1.6/docs/requirements.txt
+drwxrwxr-x   0 imorozov  (1000) imorozov  (1000)        0 2023-07-21 09:19:37.447003 ndtorch-0.1.6/docs/source/
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     2195 2023-05-25 16:17:36.000000 ndtorch-0.1.6/docs/source/conf.py
+drwxrwxr-x   0 imorozov  (1000) imorozov  (1000)        0 2023-07-21 09:19:37.447003 ndtorch-0.1.6/docs/source/examples/
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)  2228362 2023-07-04 12:27:49.000000 ndtorch-0.1.6/docs/source/examples/ndtorch.ipynb
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     1177 2023-07-21 09:16:52.000000 ndtorch-0.1.6/docs/source/index.rst
+drwxrwxr-x   0 imorozov  (1000) imorozov  (1000)        0 2023-07-21 09:19:37.475003 ndtorch-0.1.6/docs/source/modules/
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       45 2023-06-10 05:03:33.000000 ndtorch-0.1.6/docs/source/modules/bracket.rst
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       46 2023-07-03 16:31:26.000000 ndtorch-0.1.6/docs/source/modules/complex.rst
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       48 2023-05-23 16:04:29.000000 ndtorch-0.1.6/docs/source/modules/derivative.rst
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       46 2023-05-23 16:04:29.000000 ndtorch-0.1.6/docs/source/modules/evaluate.rst
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       52 2023-06-30 15:31:47.000000 ndtorch-0.1.6/docs/source/modules/factorization.rst
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       47 2023-07-21 09:16:09.000000 ndtorch-0.1.6/docs/source/modules/gradient.rst
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       43 2023-05-23 16:04:29.000000 ndtorch-0.1.6/docs/source/modules/index.rst
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       47 2023-06-15 05:00:31.000000 ndtorch-0.1.6/docs/source/modules/invariant.rst
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       46 2023-06-28 11:54:29.000000 ndtorch-0.1.6/docs/source/modules/inverse.rst
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       41 2023-05-23 16:04:29.000000 ndtorch-0.1.6/docs/source/modules/jet.rst
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       45 2023-06-18 09:03:15.000000 ndtorch-0.1.6/docs/source/modules/matrix.rst
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       46 2023-06-29 07:09:51.000000 ndtorch-0.1.6/docs/source/modules/momenta.rst
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       41 2023-05-23 16:04:29.000000 ndtorch-0.1.6/docs/source/modules/pfp.rst
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       47 2023-05-23 16:04:29.000000 ndtorch-0.1.6/docs/source/modules/propagate.rst
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       44 2023-05-23 16:04:29.000000 ndtorch-0.1.6/docs/source/modules/series.rst
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       47 2023-05-23 16:04:29.000000 ndtorch-0.1.6/docs/source/modules/signature.rst
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       44 2023-06-10 05:03:41.000000 ndtorch-0.1.6/docs/source/modules/taylor.rst
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       42 2023-05-23 16:04:29.000000 ndtorch-0.1.6/docs/source/modules/util.rst
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       46 2023-06-13 06:47:51.000000 ndtorch-0.1.6/docs/source/modules/yoshida.rst
+drwxrwxr-x   0 imorozov  (1000) imorozov  (1000)        0 2023-07-21 09:19:37.495003 ndtorch-0.1.6/ndtorch/
+-rwxrwxr-x   0 imorozov  (1000) imorozov  (1000)     8386 2023-06-03 15:36:07.000000 ndtorch-0.1.6/ndtorch/__init__.py
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     5471 2023-06-11 13:21:51.000000 ndtorch-0.1.6/ndtorch/bracket.py
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       60 2023-07-03 16:30:44.000000 ndtorch-0.1.6/ndtorch/complex.py
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     6864 2023-06-04 06:09:17.000000 ndtorch-0.1.6/ndtorch/derivative.py
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     6912 2023-07-07 13:27:14.000000 ndtorch-0.1.6/ndtorch/evaluate.py
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       31 2023-06-29 08:14:51.000000 ndtorch-0.1.6/ndtorch/expression.py
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)    24474 2023-07-04 12:27:41.000000 ndtorch-0.1.6/ndtorch/factorization.py
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)    19511 2023-07-21 09:09:48.000000 ndtorch-0.1.6/ndtorch/gradient.py
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)    13530 2023-06-22 08:11:21.000000 ndtorch-0.1.6/ndtorch/index.py
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     5929 2023-07-02 01:11:33.000000 ndtorch-0.1.6/ndtorch/invariant.py
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     5245 2023-07-02 01:33:50.000000 ndtorch-0.1.6/ndtorch/inverse.py
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)    22836 2023-06-04 06:10:00.000000 ndtorch-0.1.6/ndtorch/jet.py
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)      655 2023-06-18 09:02:20.000000 ndtorch-0.1.6/ndtorch/matrix.py
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     7597 2023-06-29 07:07:53.000000 ndtorch-0.1.6/ndtorch/momenta.py
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)    17135 2023-06-22 08:39:42.000000 ndtorch-0.1.6/ndtorch/pfp.py
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)    10182 2023-06-27 07:55:00.000000 ndtorch-0.1.6/ndtorch/propagate.py
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)    11455 2023-06-22 08:12:53.000000 ndtorch-0.1.6/ndtorch/series.py
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)    11146 2023-07-04 12:46:34.000000 ndtorch-0.1.6/ndtorch/signature.py
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       33 2023-06-29 08:07:59.000000 ndtorch-0.1.6/ndtorch/symplectify.py
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     2875 2023-06-15 14:15:13.000000 ndtorch-0.1.6/ndtorch/taylor.py
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     7023 2023-06-22 08:02:24.000000 ndtorch-0.1.6/ndtorch/util.py
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)    11084 2023-06-15 05:20:19.000000 ndtorch-0.1.6/ndtorch/yoshida.py
+drwxrwxr-x   0 imorozov  (1000) imorozov  (1000)        0 2023-07-21 09:19:37.495003 ndtorch-0.1.6/ndtorch.egg-info/
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     3952 2023-07-21 09:19:37.000000 ndtorch-0.1.6/ndtorch.egg-info/PKG-INFO
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     1478 2023-07-21 09:19:37.000000 ndtorch-0.1.6/ndtorch.egg-info/SOURCES.txt
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)        1 2023-07-21 09:19:37.000000 ndtorch-0.1.6/ndtorch.egg-info/dependency_links.txt
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)      143 2023-07-21 09:19:37.000000 ndtorch-0.1.6/ndtorch.egg-info/requires.txt
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)        8 2023-07-21 09:19:37.000000 ndtorch-0.1.6/ndtorch.egg-info/top_level.txt
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)  2228362 2023-07-04 12:27:49.000000 ndtorch-0.1.6/ndtorch.ipynb
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)      745 2023-07-21 09:17:32.000000 ndtorch-0.1.6/pyproject.toml
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       38 2023-07-21 09:19:37.495003 ndtorch-0.1.6/setup.cfg
```

### Comparing `ndtorch-0.1.5/.gitignore` & `ndtorch-0.1.6/.gitignore`

 * *Files identical despite different names*

### Comparing `ndtorch-0.1.5/LICENSE` & `ndtorch-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ndtorch-0.1.5/README.MD` & `ndtorch-0.1.6/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: ndtorch
+Version: 0.1.6
+Summary: Higher order partial derivatives computation with respect to one or several tensor-like variables, application to nonlinear dynamics
+Author-email: Ivan Morozov <i.a.morozov@inp.nsk.su>
+License: MIT
+Keywords: torch,derivative
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+Provides-Extra: examples
+Provides-Extra: test
+Provides-Extra: all
+License-File: LICENSE
+
 [![Documentation Status](https://readthedocs.org/projects/ndtorch/badge/?version=latest)](https://ndtorch.readthedocs.io/en/latest/?badge=latest)
 
 # ndtorch, 2022-2023
 ## i.a.morozov@inp.nsk.su
 
 <p align="center">
   <img width="100" height="100" src="docs/pics/logo.svg">
@@ -16,15 +31,15 @@
 ```
 $ git clone https://github.com/i-a-morozov/ndtorch.git
 $ cd ndtorch
 $ python -m pip install .
 
 ```
 
-# Derivative
+# Derivative (composable jacobian)
 
 Compute higher order function (partial) derivatives.
 
 ```python
 >>> from ndtorch.derivative import derivative
 >>> def fn(x):
 ...     return 1 + x + x**2 + x**3 + x**4 + x**5
@@ -59,14 +74,72 @@
 >>> y = torch.tensor(0.0)
 >>> derivative((2, 1), fn, x, y)
 [[tensor(0.), tensor(0.)], [tensor([0., 0.]), tensor([0., 0.])], [tensor([[2., 0.],
         [0., 2.]]), tensor([[ 2.,  0.],
         [ 0., -2.]])]]
 ```
 
+# Derivative (gradient)
+
+Compute higher order function (partial) derivatives.
+
+```python
+>>> from ndtorch.gradient import series
+>>> def fn(x):
+...     return 1 + x + x**2 + x**3 + x**4 + x**5
+... 
+>>> import torch
+>>> x = torch.tensor([0.0])
+>>> series((5, ), fn, x, retain=False, series=False)
+{(0,): tensor([1.]),
+ (1,): tensor([1.]),
+ (2,): tensor([2.]),
+ (3,): tensor([6.]),
+ (4,): tensor([24.]),
+ (5,): tensor([120.])}
+```
+
+```python
+>>> from ndtorch.gradient import series
+>>> def fn(x):
+...     x1, x2 = x
+...     return x1**2 + x1*x2 + x2**2
+...
+>>> import torch
+>>> x = torch.tensor([0.0, 0.0])
+>>> series((2, ), fn, x, intermediate=False, retain=False, series=False)
+{(2, 0): tensor(2.), (1, 1): tensor(1.), (0, 2): tensor(2.)}
+
+```
+
+```python
+>>> from ndtorch.gradient import series
+>>> def fn(x, y):
+...     x1, x2 = x
+...     y1, = y
+...     return x1**2*(1 + y1) + x2**2*(1 - y1)
+...
+>>> import torch
+>>> x = torch.tensor([0.0, 0.0])
+>>> y = torch.tensor([0.0])
+>>> series((2, 1), fn, x, y, retain=False, series=False)
+{(0, 0, 0): tensor(0.),
+ (0, 0, 1): tensor(0.),
+ (1, 0, 0): tensor(0.),
+ (0, 1, 0): tensor(0.),
+ (1, 0, 1): tensor(0.),
+ (0, 1, 1): tensor(-0.),
+ (2, 0, 0): tensor(2.),
+ (1, 1, 0): tensor(0.),
+ (0, 2, 0): tensor(2.),
+ (2, 0, 1): tensor(2.),
+ (1, 1, 1): tensor(0.),
+ (0, 2, 1): tensor(-2.)}
+```
+
 # Desription
 
 ```python
 >>> import ndtorch
 >>> ndtorch.__about__
 ```
```

### Comparing `ndtorch-0.1.5/docs/Makefile` & `ndtorch-0.1.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ndtorch-0.1.5/docs/make.bat` & `ndtorch-0.1.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ndtorch-0.1.5/docs/pics/change.gif` & `ndtorch-0.1.6/docs/pics/change.gif`

 * *Files identical despite different names*

### Comparing `ndtorch-0.1.5/docs/pics/collision.gif` & `ndtorch-0.1.6/docs/pics/collision.gif`

 * *Files identical despite different names*

### Comparing `ndtorch-0.1.5/docs/pics/logo.svg` & `ndtorch-0.1.6/docs/pics/logo.svg`

 * *Files identical despite different names*

### Comparing `ndtorch-0.1.5/docs/pics/manifold.gif` & `ndtorch-0.1.6/docs/pics/manifold.gif`

 * *Files identical despite different names*

### Comparing `ndtorch-0.1.5/docs/source/conf.py` & `ndtorch-0.1.6/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `ndtorch-0.1.5/docs/source/examples/ndtorch.ipynb` & `ndtorch-0.1.6/docs/source/examples/ndtorch.ipynb`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9868812378770304%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(4, '# Derivatives are computed by nesting torch jacobian "*

 * *            "functions\\n'), (5, '# For higher order derivatives, nesting results in exponentially "*

 * *            "growing redundant computations\\n'), (6, '# Note, forward mode is more memory "*

 * *            "efficient in this case\\n'), (9, '# This representation can be evaluated near given "*

 * *            'evaluation point (at a given deviation) if the input function returns a scalar or a '*

 * *            "vector\\n […]*

```diff
@@ -17,20 +17,21 @@
             },
             "outputs": [],
             "source": [
                 "# Given an input function, its higher order (partial) derivatives with respect to one or sevaral tensor arguments can be computed using forward or reverse mode automatic differentiation\n",
                 "# Derivative orders can be different for each tensor argument\n",
                 "# Input function is expected to return a tensor or a (nested) list of tensors\n",
                 "\n",
-                "# Derivatives are computed by nesting torch.func jacobian functions\n",
-                "# For higher order derivatives, this results in growing redundant computations, forward mode is more efficient in this case\n",
+                "# Derivatives are computed by nesting torch jacobian functions\n",
+                "# For higher order derivatives, nesting results in exponentially growing redundant computations\n",
+                "# Note, forward mode is more memory efficient in this case\n",
                 "\n",
                 "# If the input function returns a tensor, the output is referred as derivative table representation\n",
-                "# This representation can be evaluated near given evaluation point if the input function returns a scalar or a vector\n",
-                "# Table representation is a (nested) list of tensors, it can be used as a (redundant) function representation near given evaluation point\n",
+                "# This representation can be evaluated near given evaluation point (at a given deviation) if the input function returns a scalar or a vector\n",
+                "# Table representation is a (nested) list of tensors, it can be used as a redundant function representation near given evaluation point (taylor series)\n",
                 "# Table structure for f(x), f(x, y) and f(x, y, z) is shown bellow (similar structure holds for a function with more aruments)\n",
                 "\n",
                 "# f(x)\n",
                 "# t(f, x)\n",
                 "# [f, Dx f, Dxx f, ...]\n",
                 "\n",
                 "# f(x, y)\n",
@@ -125,23 +126,23 @@
             "source": [
                 "# Basic derivative interface\n",
                 "\n",
                 "# derivative(\n",
                 "#     order:int,                             # derivative order\n",
                 "#     function:Callable,                     # input function\n",
                 "#     *args,                                 # function(*args) = function(x:Tensor, ...)\n",
-                "#     intermediate:bool = True,              # flag to return intermediate derivatives\n",
+                "#     intermediate:bool = True,              # flag to return all intermediate derivatives\n",
                 "#     jacobian:Callable = torch.func.jacfwd  # torch.func.jacfwd or torch.func.jacfrev\n",
                 "# )\n",
                 "\n",
                 "# derivative(\n",
                 "#     order:tuple[int, ...],                 # derivative orders\n",
                 "#     function:Callable,                     # input function\n",
                 "#     *args,                                 # function(*args) = function(x:Tensor, y:Tensor, z:Tensor, ...)\n",
-                "#     intermediate:bool = True,              # flag to return intermediate derivatives\n",
+                "#     intermediate:bool = True,              # flag to return all intermediate derivatives\n",
                 "#     jacobian:Callable = torch.func.jacfwd  # torch.func.jacfwd or torch.func.jacfrev\n",
                 "# )"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 5,
@@ -164,14 +165,15 @@
             "source": [
                 "# Derivative\n",
                 "\n",
                 "# Input:  scalar\n",
                 "# Output: scalar\n",
                 "\n",
                 "# Set test function\n",
+                "\n",
                 "# Note, the first function argument is a scalar tensor\n",
                 "# Input function can have other additional arguments\n",
                 "# Other arguments are not used in computation of derivatives\n",
                 "\n",
                 "def fn(x, a, b, c, d, e, f):\n",
                 "    return a + b*x + c*x**2 + d*x**3 + e*x**4 + f*x**5\n",
                 "\n",
@@ -189,15 +191,16 @@
                 "\n",
                 "# Compute n'th derivative\n",
                 "\n",
                 "value = derivative(n, fn, x, a, b, c, d, e, f, intermediate=False, jacobian=torch.func.jacfwd)\n",
                 "print(value.cpu().numpy().tolist())\n",
                 "\n",
                 "# Compute all derivatives upto given order\n",
-                "# Note, function value itself is referred as zeros order derivative\n",
+                "\n",
+                "# Note, function value itself is referred as zero order derivative\n",
                 "# Since function returns a tensor, output is a list of tensors\n",
                 "\n",
                 "values = derivative(n, fn, x, a, b, c, d, e, f, intermediate=True, jacobian=torch.func.jacfwd)\n",
                 "print(*[value.cpu().numpy().tolist() for value in values], sep=', ')\n",
                 "\n",
                 "# Note, intermediate flag (default=True) can be used to return all derivatives\n",
                 "# For jacobian parameter, torch.func.jacfwd or torch.func.jacrev functions can be passed\n",
@@ -234,14 +237,15 @@
             "source": [
                 "# Derivative\n",
                 "\n",
                 "# Input:  vector\n",
                 "# Output: scalar\n",
                 "\n",
                 "# Set test function\n",
+                "\n",
                 "# Note, the first function argument is a vector tensor\n",
                 "# Input function can have other additional arguments\n",
                 "# Other arguments are not used in computation of derivatives\n",
                 "\n",
                 "def fn(x, a, b, c):\n",
                 "    x1, x2 = x\n",
                 "    return a + b*(x1 - 1)**2 + c*(x2 + 1)**2\n",
@@ -255,27 +259,29 @@
                 "x = torch.tensor([0.0, 0.0], dtype=dtype, device=device)\n",
                 "\n",
                 "# Set fixed parameters\n",
                 "\n",
                 "a, b, c = torch.tensor([1.0, 1.0, 1.0], dtype=dtype, device=device)\n",
                 "\n",
                 "# Compute only n'th derivative\n",
-                "# Note, for given input & output the result is hessian\n",
+                "\n",
+                "# Note, for given input & output the result is a hessian\n",
                 "\n",
                 "value = derivative(n, fn, x, a, b, c, intermediate=False, jacobian=torch.func.jacfwd)\n",
                 "print(value.cpu().numpy().tolist())\n",
                 "\n",
                 "# Compute all derivatives upto given order\n",
-                "# Note, fuction value itself is referred as zeros order derivative\n",
+                "\n",
+                "# Note, fuction value itself is referred as zero order derivative\n",
                 "# Output is a list of tensors (value, jacobian, hessian, ...)\n",
                 "\n",
                 "values = derivative(n, fn, x, a, b, c, intermediate=True, jacobian=torch.func.jacfwd)\n",
                 "print(*[value.cpu().numpy().tolist() for value in values], sep=', ')\n",
                 "\n",
-                "# Compute jacobian and hessian with torch.func\n",
+                "# Compute jacobian and hessian with torch\n",
                 "\n",
                 "print(fn(x, a, b, c).cpu().numpy().tolist(), \n",
                 "      torch.func.jacfwd(lambda x: fn(x, a, b, c))(x).cpu().numpy().tolist(), \n",
                 "      torch.func.hessian(lambda x: fn(x, a, b, c))(x).cpu().numpy().tolist(), \n",
                 "      sep=', ')\n",
                 "\n",
                 "# Evaluate derivative table representation for a given deviation from the evaluation point\n",
@@ -285,14 +291,15 @@
                 "print(fn(x + dx, a, b, c).cpu().numpy())\n",
                 "\n",
                 "# Evaluate can be mapped over a set of deviation values\n",
                 "\n",
                 "print(torch.func.vmap(lambda x: evaluate(values, [x]))(torch.stack(5*[dx])).cpu().numpy().tolist())\n",
                 "\n",
                 "# Derivative can be mapped over a set of evaluation points\n",
+                "\n",
                 "# Note, the inputt function is expeted to return a tensor\n",
                 "\n",
                 "print(torch.func.vmap(lambda x: derivative(1, fn, x, a, b, c, intermediate=False))(torch.stack(5*[x])).cpu().numpy().tolist())"
             ]
         },
         {
             "cell_type": "code",
@@ -316,14 +323,15 @@
             "source": [
                 "# Derivative\n",
                 "\n",
                 "# Input:  vector\n",
                 "# Output: vector\n",
                 "\n",
                 "# Set test function\n",
+                "\n",
                 "# Note, the first function argument is a vector tensor\n",
                 "# Input function can have other additional arguments\n",
                 "# Other arguments (if any) are not used in computation of derivatives\n",
                 "\n",
                 "def fn(x):\n",
                 "    x1, x2 = x\n",
                 "    X1 = 1.0*x1 + 2.0*x2\n",
@@ -392,20 +400,22 @@
                 "n = 3\n",
                 "\n",
                 "# Set evaluation point\n",
                 "\n",
                 "x = torch.zeros((1, 2, 3), dtype=dtype, device=device)\n",
                 "\n",
                 "# Compute derivatives\n",
+                "\n",
                 "# Note, output is a list of tensors\n",
                 "\n",
                 "values = derivative(n, fn, x)\n",
                 "print(*[list(value.shape) for value in values], sep='\\n')\n",
                 "\n",
                 "# Evaluate derivative table representation for a given deviation from the evaluation point\n",
+                "\n",
                 "# Note, evaluate function works with scalar or vector tensor input\n",
                 "# One should compute derivatives of a wrapped function and reshape the result of evaluate\n",
                 "\n",
                 "# Set wrapped function\n",
                 "\n",
                 "def gn(x, shape):\n",
                 "    return fn(x.reshape(shape)).flatten()\n",
@@ -8866,16 +8876,16 @@
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "# Compute nonlinear invariants\n",
                 "# Note, computation is not optimized and requires a lot of memory\n",
                 "\n",
-                "tx, _ = invariant((4, ), x, [], ix, lambda x: evaluate(t, [x]), jacobian=torch.func.jacfwd, threshold=1.0E-3)\n",
-                "ty, _ = invariant((4, ), x, [], iy, lambda x: evaluate(t, [x]), jacobian=torch.func.jacfwd, threshold=1.0E-3)"
+                "tx, _ = invariant((4, ), x, [], ix, t, jacobian=torch.func.jacfwd, threshold=1.0E-3)\n",
+                "ty, _ = invariant((4, ), x, [], iy, t, jacobian=torch.func.jacfwd, threshold=1.0E-3)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 13,
             "id": "89508b00-d209-4268-9493-4181cf94325a",
             "metadata": {
@@ -9389,15 +9399,15 @@
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "# 1st invariant\n",
                 "\n",
-                "tx, _ = invariant((nx, nw, nk), x, [w, k], ix, t, jacobian=torch.func.jacrev, threshold=0.01, limit=1)\n",
+                "tx, _ = invariant((nx, nw, nk), x, [w, k], ix, t, jacobian=torch.func.jacrev, threshold=0.01)\n",
                 "_"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 15,
             "id": "1aba49aa-9193-4888-8a0c-c83222f00e84",
@@ -9413,17 +9423,17 @@
                     },
                     "execution_count": 15,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "# 2st invariant\n",
+                "# 2nd invariant\n",
                 "\n",
-                "ty, _ = invariant((nx, nw, nk), x, [w, k], iy, t, jacobian=torch.func.jacrev, threshold=0.01, limit=1)\n",
+                "ty, _ = invariant((nx, nw, nk), x, [w, k], iy, t, jacobian=torch.func.jacrev, threshold=0.01)\n",
                 "_"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 16,
             "id": "9744a927-cdbd-477c-ad0a-4f7363285d26",
@@ -9441,16 +9451,16 @@
                 }
             ],
             "source": [
                 "# Test conservation\n",
                 "\n",
                 "# Note, here propagate is used as composition\n",
                 "\n",
-                "print(compare(tx, propagate((4, 1, 3), (nx-1, nw, nk), t, [w, k], tx)))\n",
-                "print(compare(ty, propagate((4, 1, 3), (nx-1, nw, nk), t, [w, k], ty)))"
+                "print(compare(propagate((4, 1, 3), (nx-1, nw, nk), t, [w, k], tx), tx))\n",
+                "print(compare(propagate((4, 1, 3), (nx-1, nw, nk), t, [w, k], ty), ty))"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 17,
             "id": "a5e75ebb-22b4-4f55-9c14-5e21e97d6427",
             "metadata": {
@@ -10192,22 +10202,20 @@
             "id": "b6d8a68a-5c71-4812-a8fe-9952ae2c863f",
             "metadata": {
                 "tags": []
             },
             "outputs": [
                 {
                     "data": {
-                        "image/png": "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\n",
+                        "image/png": "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9mu1WnTt2hVFRUV315SDU/N9vnXrVpw/fx46nQ4AsGTJEqSmpmLNmjWIi4uzSn+OyBaZN0Zj7nUcFZ+AEQDA29sbfn5+Db5cXV1hMplQUVGBnJwcZWxaWhrMZjOCgoLqPXZgYCBcXFywY8cOZVthYSGKiopgMpkAACaTCQcOHLC4GU1NTYVOp4O/vz90Oh0OHDiAvLw85RUdHY2ePXsiLy/vln+3I3P0zOts2LABEyZMwIYNGxAaGmrtGByCq6srAgMDLfIym83YsWOHkteNTCaTRT3wX3519b6+vjAajRY1lZWVyMzMtLgGTb22zYVamQP/PfkaPHiw8lRAo2kZXwrVynzhwoXYv3+/8tldt9T0pk2bMHfuXKv26GjUyjwwMBBarRaFhYVKTU1NDU6cOIEHHnjAav05IrUyv3TpEgDc9Hmi0WiUJ5LNlS0yb4zG3Os4LJUXAaF70LBhw6RPnz6SmZkpv//+u3Tv3t1i2ezi4mLp2bOnZGZmKtuio6OlS5cukpaWJtnZ2WIymcRkMin765ZEDwkJkby8PNm+fbt4e3vXuwx9nZayCqKIepmvW7dOnJ2dZfHixXL69GnlVVFRYZ/G7Wjjxo2i1Wpl9erVcujQIZk0aZLo9Xpllcjx48dLXFycUp+eni7Ozs7y0UcfyeHDhyUhIaHeZYv1er388MMP8ueff8rIkSPrXYa+oWvbnKmReXFxsXTr1k2GDBkixcXFFu/rlkCt9/n1brWiWXOlVuavv/663H///ZKSkiIFBQUSGRkpBoNBysvL7de8StTI/OzZs+Ll5SWjR4+WvLw8KSwslLfeektcXFwkLy/PvgGowBaZnzt3TnJzcyUpKUkAyMaNGyU3N9fi8/p29zqOihMwarJz587JuHHjpE2bNqLT6WTChAlSVVWl7K/74rpz505l2+XLl2Xq1Kni6ekp7u7u8vzzz990w3PixAkZPny4uLm5Sfv27SU2NlZqampueR4taQKmVuaDBg0SADe9Xn31VVu3rIpFixZJly5dxNXVVR5//HHZs2ePsm/QoEE39b1582bp0aOHuLq6ysMPPyxJSUkW+81ms7z33nvi4+MjWq1WhgwZIoWFhRY1t7u2zZ29M1+1alW97+mW9P1INd7n12tpEzARdTKvrq6W2NhYMRgM0rZtWwkODpaDBw/arEdHo0bme/fulZCQEGnXrp20bdtW+vfvL8nJyTbr0dFYO/NbfV4nJCQoNY2513FETiIidn3kRkRERERE1EK1jB98JyIiIiIicgCcgBEREREREdkJJ2BERERERER2wgkYERERERGRnXACRkREREREZCecgBEREREREdkJJ2BERERERER2wgkYERERERGRnXACRkREREREZCecgBEREREREdkJJ2BERERERER28n947CN6rmYMbQAAAABJRU5ErkJggg==",
                         "text/plain": [
-                            "<Figure size 720x720 with 1 Axes>"
+                            "<Figure size 1000x1000 with 1 Axes>"
                         ]
                     },
-                    "metadata": {
-                        "needs_background": "light"
-                    },
+                    "metadata": {},
                     "output_type": "display_data"
                 }
             ],
             "source": [
                 "# Compare phase space trajectories\n",
                 "\n",
                 "plt.figure(figsize=(10, 10))\n",
@@ -10460,133 +10468,34 @@
             "execution_count": 8,
             "id": "e7f286aa-dc5d-48c0-9827-d0aa560362bd",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "[tensor([0., 0., 0., 0.], dtype=torch.float64),\n",
+                            "[[],\n",
                             " tensor([[1.000000000000e+00, 0.000000000000e+00, 0.000000000000e+00, 0.000000000000e+00],\n",
                             "         [0.000000000000e+00, 1.000000000000e+00, 0.000000000000e+00, 0.000000000000e+00],\n",
                             "         [0.000000000000e+00, 0.000000000000e+00, 1.000000000000e+00, 0.000000000000e+00],\n",
                             "         [0.000000000000e+00, 0.000000000000e+00, 0.000000000000e+00, 1.000000000000e+00]],\n",
                             "        dtype=torch.float64),\n",
-                            " tensor([[[0., 0., 0., 0.],\n",
-                            "          [0., 0., 0., 0.],\n",
-                            "          [0., 0., 0., 0.],\n",
-                            "          [0., 0., 0., 0.]],\n",
-                            " \n",
-                            "         [[0., 0., 0., 0.],\n",
-                            "          [0., 0., 0., 0.],\n",
-                            "          [0., 0., 0., 0.],\n",
-                            "          [0., 0., 0., 0.]],\n",
-                            " \n",
-                            "         [[0., 0., 0., 0.],\n",
-                            "          [0., 0., 0., 0.],\n",
-                            "          [0., 0., 0., 0.],\n",
-                            "          [0., 0., 0., 0.]],\n",
-                            " \n",
-                            "         [[0., 0., 0., 0.],\n",
-                            "          [0., 0., 0., 0.],\n",
-                            "          [0., 0., 0., 0.],\n",
-                            "          [0., 0., 0., 0.]]], dtype=torch.float64),\n",
-                            " tensor([[[[0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.]],\n",
-                            " \n",
-                            "          [[0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.]],\n",
-                            " \n",
-                            "          [[0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.]],\n",
-                            " \n",
-                            "          [[0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.]]],\n",
-                            " \n",
-                            " \n",
-                            "         [[[0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.]],\n",
-                            " \n",
-                            "          [[0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.]],\n",
-                            " \n",
-                            "          [[0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.]],\n",
-                            " \n",
-                            "          [[0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.]]],\n",
-                            " \n",
-                            " \n",
-                            "         [[[0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.]],\n",
-                            " \n",
-                            "          [[0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.]],\n",
-                            " \n",
-                            "          [[0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.]],\n",
-                            " \n",
-                            "          [[0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.]]],\n",
-                            " \n",
-                            " \n",
-                            "         [[[0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.]],\n",
-                            " \n",
-                            "          [[0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.]],\n",
-                            " \n",
-                            "          [[0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.]],\n",
-                            " \n",
-                            "          [[0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.]]]], dtype=torch.float64)]"
+                            " [],\n",
+                            " []]"
                         ]
                     },
                     "execution_count": 8,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "# Check\n",
                 "\n",
                 "out = propagate((4, ), (n, ), t_inv, [], t)\n",
-                "chop(out)\n",
+                "chop(out, replace=True)\n",
                 "out"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "fd37bbff-419e-48cd-af75-7026011537df",
             "metadata": {},
@@ -10823,26 +10732,15 @@
             "metadata": {
                 "tags": []
             },
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "[[tensor([0., 0., 0., 0.], dtype=torch.float64),\n",
-                            "  tensor([[0.],\n",
-                            "          [0.],\n",
-                            "          [0.],\n",
-                            "          [0.]], dtype=torch.float64),\n",
-                            "  tensor([[[0.]],\n",
-                            "  \n",
-                            "          [[0.]],\n",
-                            "  \n",
-                            "          [[0.]],\n",
-                            "  \n",
-                            "          [[0.]]], dtype=torch.float64)]]"
+                            "[[[], [], []]]"
                         ]
                     },
                     "execution_count": 9,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -10852,15 +10750,15 @@
                 "# Note, this transformation map zero (parametric) state to zero (upto given order)\n",
                 "# This is true by construction\n",
                 "\n",
                 "def fn_01_02(x, w):\n",
                 "    return map_01_02(x + evaluate(first(pfp), [w]), w) - evaluate(first(pfp), [w])\n",
                 "\n",
                 "out = propagate((4, 1), (0, nw), identity((0, nw), [x, w]), [w], fn_01_02)\n",
-                "chop(out)\n",
+                "chop(out, replace=True)\n",
                 "out"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 10,
             "id": "cb80f040-10d2-4f0a-b2f9-654c71ac62f6",
@@ -10892,417 +10790,75 @@
             "execution_count": 12,
             "id": "15165c76-6665-4098-86b3-9a6d06b198ee",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "[[tensor([0., 0., 0., 0.], dtype=torch.float64),\n",
-                            "  tensor([[0.],\n",
-                            "          [0.],\n",
-                            "          [0.],\n",
-                            "          [0.]], dtype=torch.float64),\n",
-                            "  tensor([[[0.]],\n",
-                            "  \n",
-                            "          [[0.]],\n",
-                            "  \n",
-                            "          [[0.]],\n",
-                            "  \n",
-                            "          [[0.]]], dtype=torch.float64)],\n",
+                            "[[[], [], []],\n",
                             " [tensor([[1.000000000000e+00, 0.000000000000e+00, 0.000000000000e+00, 0.000000000000e+00],\n",
                             "          [0.000000000000e+00, 1.000000000000e+00, 0.000000000000e+00, 0.000000000000e+00],\n",
                             "          [0.000000000000e+00, 0.000000000000e+00, 1.000000000000e+00, 0.000000000000e+00],\n",
                             "          [0.000000000000e+00, 0.000000000000e+00, 0.000000000000e+00, 1.000000000000e+00]],\n",
                             "         dtype=torch.float64),\n",
-                            "  tensor([[[0., 0., 0., 0.]],\n",
-                            "  \n",
-                            "          [[0., 0., 0., 0.]],\n",
-                            "  \n",
-                            "          [[0., 0., 0., 0.]],\n",
-                            "  \n",
-                            "          [[0., 0., 0., 0.]]], dtype=torch.float64),\n",
-                            "  tensor([[[[0., 0., 0., 0.]]],\n",
-                            "  \n",
-                            "  \n",
-                            "          [[[0., 0., 0., 0.]]],\n",
-                            "  \n",
-                            "  \n",
-                            "          [[[0., 0., 0., 0.]]],\n",
-                            "  \n",
-                            "  \n",
-                            "          [[[0., 0., 0., 0.]]]], dtype=torch.float64)],\n",
-                            " [tensor([[[0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.]],\n",
-                            "  \n",
-                            "          [[0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.]],\n",
-                            "  \n",
-                            "          [[0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.]],\n",
-                            "  \n",
-                            "          [[0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.]]], dtype=torch.float64),\n",
-                            "  tensor([[[[0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.]]],\n",
-                            "  \n",
-                            "  \n",
-                            "          [[[0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.]]],\n",
-                            "  \n",
-                            "  \n",
-                            "          [[[0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.]]],\n",
-                            "  \n",
-                            "  \n",
-                            "          [[[0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.]]]], dtype=torch.float64),\n",
-                            "  tensor([[[[[0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.]]]],\n",
-                            "  \n",
-                            "  \n",
-                            "  \n",
-                            "          [[[[0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.]]]],\n",
-                            "  \n",
-                            "  \n",
-                            "  \n",
-                            "          [[[[0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.]]]],\n",
-                            "  \n",
-                            "  \n",
-                            "  \n",
-                            "          [[[[0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.]]]]], dtype=torch.float64)],\n",
-                            " [tensor([[[[0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.]],\n",
-                            "  \n",
-                            "           [[0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.]],\n",
-                            "  \n",
-                            "           [[0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.]],\n",
-                            "  \n",
-                            "           [[0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.]]],\n",
-                            "  \n",
-                            "  \n",
-                            "          [[[0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.]],\n",
-                            "  \n",
-                            "           [[0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.]],\n",
-                            "  \n",
-                            "           [[0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.]],\n",
-                            "  \n",
-                            "           [[0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.]]],\n",
-                            "  \n",
-                            "  \n",
-                            "          [[[0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.]],\n",
-                            "  \n",
-                            "           [[0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.]],\n",
-                            "  \n",
-                            "           [[0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.]],\n",
-                            "  \n",
-                            "           [[0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.]]],\n",
-                            "  \n",
-                            "  \n",
-                            "          [[[0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.]],\n",
-                            "  \n",
-                            "           [[0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.]],\n",
-                            "  \n",
-                            "           [[0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.]],\n",
-                            "  \n",
-                            "           [[0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.]]]], dtype=torch.float64),\n",
-                            "  tensor([[[[[0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.]],\n",
-                            "  \n",
-                            "            [[0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.]],\n",
-                            "  \n",
-                            "            [[0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.]],\n",
-                            "  \n",
-                            "            [[0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.]]]],\n",
-                            "  \n",
-                            "  \n",
-                            "  \n",
-                            "          [[[[0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.]],\n",
-                            "  \n",
-                            "            [[0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.]],\n",
-                            "  \n",
-                            "            [[0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.]],\n",
-                            "  \n",
-                            "            [[0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.]]]],\n",
-                            "  \n",
-                            "  \n",
-                            "  \n",
-                            "          [[[[0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.]],\n",
-                            "  \n",
-                            "            [[0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.]],\n",
-                            "  \n",
-                            "            [[0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.]],\n",
-                            "  \n",
-                            "            [[0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.]]]],\n",
-                            "  \n",
-                            "  \n",
-                            "  \n",
-                            "          [[[[0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.]],\n",
-                            "  \n",
-                            "            [[0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.]],\n",
-                            "  \n",
-                            "            [[0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.]],\n",
-                            "  \n",
-                            "            [[0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.]]]]], dtype=torch.float64),\n",
-                            "  tensor([[[[[[0., 0., 0., 0.],\n",
-                            "              [0., 0., 0., 0.],\n",
-                            "              [0., 0., 0., 0.],\n",
-                            "              [0., 0., 0., 0.]],\n",
-                            "  \n",
-                            "             [[0., 0., 0., 0.],\n",
-                            "              [0., 0., 0., 0.],\n",
-                            "              [0., 0., 0., 0.],\n",
-                            "              [0., 0., 0., 0.]],\n",
-                            "  \n",
-                            "             [[0., 0., 0., 0.],\n",
-                            "              [0., 0., 0., 0.],\n",
-                            "              [0., 0., 0., 0.],\n",
-                            "              [0., 0., 0., 0.]],\n",
-                            "  \n",
-                            "             [[0., 0., 0., 0.],\n",
-                            "              [0., 0., 0., 0.],\n",
-                            "              [0., 0., 0., 0.],\n",
-                            "              [0., 0., 0., 0.]]]]],\n",
-                            "  \n",
-                            "  \n",
-                            "  \n",
-                            "  \n",
-                            "          [[[[[0., 0., 0., 0.],\n",
-                            "              [0., 0., 0., 0.],\n",
-                            "              [0., 0., 0., 0.],\n",
-                            "              [0., 0., 0., 0.]],\n",
-                            "  \n",
-                            "             [[0., 0., 0., 0.],\n",
-                            "              [0., 0., 0., 0.],\n",
-                            "              [0., 0., 0., 0.],\n",
-                            "              [0., 0., 0., 0.]],\n",
-                            "  \n",
-                            "             [[0., 0., 0., 0.],\n",
-                            "              [0., 0., 0., 0.],\n",
-                            "              [0., 0., 0., 0.],\n",
-                            "              [0., 0., 0., 0.]],\n",
-                            "  \n",
-                            "             [[0., 0., 0., 0.],\n",
-                            "              [0., 0., 0., 0.],\n",
-                            "              [0., 0., 0., 0.],\n",
-                            "              [0., 0., 0., 0.]]]]],\n",
-                            "  \n",
-                            "  \n",
-                            "  \n",
-                            "  \n",
-                            "          [[[[[0., 0., 0., 0.],\n",
-                            "              [0., 0., 0., 0.],\n",
-                            "              [0., 0., 0., 0.],\n",
-                            "              [0., 0., 0., 0.]],\n",
-                            "  \n",
-                            "             [[0., 0., 0., 0.],\n",
-                            "              [0., 0., 0., 0.],\n",
-                            "              [0., 0., 0., 0.],\n",
-                            "              [0., 0., 0., 0.]],\n",
-                            "  \n",
-                            "             [[0., 0., 0., 0.],\n",
-                            "              [0., 0., 0., 0.],\n",
-                            "              [0., 0., 0., 0.],\n",
-                            "              [0., 0., 0., 0.]],\n",
-                            "  \n",
-                            "             [[0., 0., 0., 0.],\n",
-                            "              [0., 0., 0., 0.],\n",
-                            "              [0., 0., 0., 0.],\n",
-                            "              [0., 0., 0., 0.]]]]],\n",
-                            "  \n",
-                            "  \n",
-                            "  \n",
-                            "  \n",
-                            "          [[[[[0., 0., 0., 0.],\n",
-                            "              [0., 0., 0., 0.],\n",
-                            "              [0., 0., 0., 0.],\n",
-                            "              [0., 0., 0., 0.]],\n",
-                            "  \n",
-                            "             [[0., 0., 0., 0.],\n",
-                            "              [0., 0., 0., 0.],\n",
-                            "              [0., 0., 0., 0.],\n",
-                            "              [0., 0., 0., 0.]],\n",
-                            "  \n",
-                            "             [[0., 0., 0., 0.],\n",
-                            "              [0., 0., 0., 0.],\n",
-                            "              [0., 0., 0., 0.],\n",
-                            "              [0., 0., 0., 0.]],\n",
-                            "  \n",
-                            "             [[0., 0., 0., 0.],\n",
-                            "              [0., 0., 0., 0.],\n",
-                            "              [0., 0., 0., 0.],\n",
-                            "              [0., 0., 0., 0.]]]]]], dtype=torch.float64)]]"
+                            "  [],\n",
+                            "  []],\n",
+                            " [[], [], []],\n",
+                            " [[], [], []]]"
                         ]
                     },
                     "execution_count": 12,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "# Check\n",
                 "\n",
                 "out = propagate((4, 1), (nx, nw), t_inv, [w], t)\n",
-                "chop(out)\n",
+                "chop(out, replace=True)\n",
                 "out"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "1a64f7bd-e716-4653-95f6-ddc3ed0108d3",
             "metadata": {},
             "source": [
-                "# Example-29: Momenta"
+                "# Example-29: Momenta generator"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 1,
             "id": "fd671059-7f65-4e37-a093-63e5b90b6c35",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
-                "# In this example initial and final monemta are computed from given initial and final coordinates"
+                "# In this example initial and final monemta are computed from given initial and final coordinates\n",
+                "# Given an origing preserving mapping, its table representation can be computed upto some order\n",
+                "# This representation can be considered as exact\n",
+                "# Next, given initial and final coordinates, corresponding momenta can be computed using momenta generator"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 18,
+            "execution_count": 2,
             "id": "a8cfbb8f-8e87-4e6e-9e5d-b30fe8d87318",
             "metadata": {
                 "tags": []
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "False\n"
+                        "True\n"
                     ]
                 }
             ],
             "source": [
                 "# Import\n",
                 "\n",
                 "import numpy\n",
@@ -11324,30 +10880,30 @@
                 "\n",
                 "import warnings\n",
                 "warnings.filterwarnings(\"ignore\")"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 19,
+            "execution_count": 3,
             "id": "701fc087-f666-43e0-a90a-8b0580102a7f",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "# Set data type and device\n",
                 "\n",
                 "dtype = torch.float64\n",
                 "device = torch.device('cpu')"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 20,
+            "execution_count": 4,
             "id": "3094551a-2a92-464e-9121-d37f190864a4",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "# Set elements\n",
@@ -11572,25 +11128,25 @@
             "execution_count": 12,
             "id": "287c366c-dbe7-4675-8f79-209e7c9e1f78",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
-                "# Compute monemta generator\n",
+                "# Compute momenta generator\n",
                 "\n",
                 "# Note, computation order can be different from that of the input table\n",
                 "# Accuracy is strongly related to computation order and magnitude of initial coordinates\n",
                 "\n",
                 "m = momenta((nx, nw), x, [w], t)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 27,
+            "execution_count": 13,
             "id": "fa9a6e65-5a23-4d45-a76b-756da0491388",
             "metadata": {
                 "tags": []
             },
             "outputs": [
                 {
                     "name": "stdout",
@@ -11613,16 +11169,16 @@
                 }
             ],
             "source": [
                 "# Recover momenta from coordinates\n",
                 "\n",
                 "# Set deviations\n",
                 "\n",
-                "xi = torch.tensor([0.0005, 0.0001, -0.0005, -0.0001], dtype=dtype)\n",
-                "dw = torch.tensor(1*[0.0001], dtype=torch.float64)\n",
+                "xi = torch.tensor([0.0005, 0.0001, -0.0005, -0.0001], dtype=dtype, device=device)\n",
+                "dw = torch.tensor(1*[0.0001], dtype=dtype, device=device)\n",
                 "\n",
                 "# Evaluate final state using table representation\n",
                 "\n",
                 "xf = evaluate(t, [xi, dw])\n",
                 "\n",
                 "print(xf)\n",
                 "print()\n",
@@ -11646,14 +11202,987 @@
                 "print()\n",
                 "\n",
                 "# Evaluate generator using coordinates\n",
                 "\n",
                 "print(evaluate(m, [qs, 0*dw]))\n",
                 "print(evaluate(m, [qs, 1*dw]))"
             ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "9dcdb26f-f41a-428b-b3f1-0de458403dc3",
+            "metadata": {},
+            "source": [
+                "# Example-30: Factorization (kick)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 1,
+            "id": "5c9c3ebf-1980-4108-b5b0-58ffe61cb8fe",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "# Given a derivative table representation (taylor series) of an origin preserving mapping\n",
+                "# It is possible to factorize it into composition of linear and nonlinear table representations\n",
+                "# If original mapping represents a single turn, linear part can be brought to its normal form\n",
+                "# This can be done using linear theory\n",
+                "# The nonlinear part is a near identity transformation, it can be represented with Lie transformation\n",
+                "# t = tl o tn and tn = exp(-[h])\n",
+                "# In this example (generator) h is computed for a single kick\n",
+                "# It can be used to construct nonlinear normal forms or as a redundancy free representation"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 2,
+            "id": "186b19c2-a6a4-4eb7-b239-e9e0695cd7e4",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "True\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Import\n",
+                "\n",
+                "import torch\n",
+                "\n",
+                "from ndtorch.derivative import derivative\n",
+                "from ndtorch.signature import chop\n",
+                "from ndtorch.evaluate import evaluate\n",
+                "from ndtorch.propagate import identity\n",
+                "from ndtorch.propagate import propagate\n",
+                "from ndtorch.series import series\n",
+                "from ndtorch.series import clean\n",
+                "from ndtorch.taylor import taylor\n",
+                "from ndtorch.inverse import inverse\n",
+                "from ndtorch.factorization import hamiltonian\n",
+                "\n",
+                "torch.set_printoptions(precision=12, sci_mode=True)\n",
+                "print(torch.cuda.is_available())\n",
+                "\n",
+                "import warnings\n",
+                "warnings.filterwarnings(\"ignore\")"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 3,
+            "id": "56cd3c16-afee-4687-b711-9a248e9c9f0d",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "# Set data type and device\n",
+                "\n",
+                "dtype = torch.float64\n",
+                "device = torch.device('cpu')"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 4,
+            "id": "46182ddc-f0a7-47f0-873a-57c2eb80da81",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "tensor([0., 0., 0., 0.], dtype=torch.float64)\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Set transformation\n",
+                "\n",
+                "# Note, this transformation can be exactly represented with a taylor series (i.e. polynomial)\n",
+                "\n",
+                "def mapping(x, k, l):\n",
+                "    (qx, px, qy, py), (k, ), l = x, k, l/2\n",
+                "    qx, qy = qx + l*px, qy + l*py\n",
+                "    px, py = px - 1.0*l*k*(qx**2 - qy**2), py + 2.0*l*k*qx*qy\n",
+                "    qx, qy = qx + l*px, qy + l*py\n",
+                "    return torch.stack([qx, px, qy, py])\n",
+                "\n",
+                "# Test origin propagation\n",
+                "\n",
+                "x = torch.tensor(4*[0.0], dtype=dtype, device=device)\n",
+                "k = torch.tensor(1*[0.0], dtype=dtype, device=device)\n",
+                "\n",
+                "print(mapping(x, k, 0.1))"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 5,
+            "id": "281e3c38-c941-4622-8a3b-5f0619409511",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "# Compute table representation\n",
+                "\n",
+                "t = identity((2, 1), [x, k])\n",
+                "t = propagate((4, 1), (2, 1), t, [k], mapping, 0.1)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 6,
+            "id": "63a04154-d5da-4968-aa34-e6bcbbcf0576",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "tensor([1.009811250000e-01, 9.622500000000e-03, 5.102537625000e-02, 1.050752500000e-02],\n",
+                        "       dtype=torch.float64)\n",
+                        "tensor([1.009811250000e-01, 9.622500000000e-03, 5.102537625000e-02, 1.050752500000e-02],\n",
+                        "       dtype=torch.float64)\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Compare for some deviation\n",
+                "\n",
+                "dx = torch.tensor([0.1, 0.01, 0.05, 0.01], dtype=dtype, device=device)\n",
+                "dk = torch.tensor([1.0],dtype=dtype, device=device)\n",
+                "\n",
+                "print(mapping(x + dx, k + dk, 0.1))\n",
+                "print(evaluate(t, [dx, dk]))"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 7,
+            "id": "52aff165-c437-4e34-9d62-78dd396522d5",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "tensor([[1.000000000000e+00, 1.000000000000e-01, 0.000000000000e+00, 0.000000000000e+00],\n",
+                        "        [0.000000000000e+00, 1.000000000000e+00, 0.000000000000e+00, 0.000000000000e+00],\n",
+                        "        [0.000000000000e+00, 0.000000000000e+00, 1.000000000000e+00, 1.000000000000e-01],\n",
+                        "        [0.000000000000e+00, 0.000000000000e+00, 0.000000000000e+00, 1.000000000000e+00]],\n",
+                        "       dtype=torch.float64)\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Linear part is not near identity\n",
+                "\n",
+                "print(derivative(1, lambda x, k: evaluate(t, [x, k]), x, k, intermediate=False))"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 8,
+            "id": "1b25e630-6870-4be2-86d3-8d8dce231b3b",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "# Set linear part and compose with its inverse\n",
+                "\n",
+                "l = derivative(1, lambda x, k: evaluate(t, [x, k]), x, k)\n",
+                "t = propagate((4, 1), (2, 1), inverse(1, x, [k], l), [k], t)\n",
+                "chop(t)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 9,
+            "id": "c631a032-59f2-40b7-ace1-00b9e1243b25",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "tensor([[1.000000000000e+00, 0.000000000000e+00, 0.000000000000e+00, 0.000000000000e+00],\n",
+                        "        [0.000000000000e+00, 1.000000000000e+00, 0.000000000000e+00, 0.000000000000e+00],\n",
+                        "        [0.000000000000e+00, 0.000000000000e+00, 1.000000000000e+00, 0.000000000000e+00],\n",
+                        "        [0.000000000000e+00, 0.000000000000e+00, 0.000000000000e+00, 1.000000000000e+00]],\n",
+                        "       dtype=torch.float64)\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Now table represents a near identity transformation\n",
+                "\n",
+                "print(derivative(1, lambda x, k: evaluate(t, [x, k]), x, k, intermediate=False))"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 10,
+            "id": "6852653d-0193-4d28-8454-05530ab38812",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "(3, 0, 0, 0, 1) tensor(1.666666666667e-02, dtype=torch.float64)\n",
+                        "(2, 1, 0, 0, 1) tensor(-2.500000000000e-03, dtype=torch.float64)\n",
+                        "(1, 2, 0, 0, 1) tensor(1.250000000000e-04, dtype=torch.float64)\n",
+                        "(1, 0, 2, 0, 1) tensor(-5.000000000000e-02, dtype=torch.float64)\n",
+                        "(1, 0, 1, 1, 1) tensor(5.000000000000e-03, dtype=torch.float64)\n",
+                        "(1, 0, 0, 2, 1) tensor(-1.250000000000e-04, dtype=torch.float64)\n",
+                        "(0, 3, 0, 0, 1) tensor(-2.083333333333e-06, dtype=torch.float64)\n",
+                        "(0, 1, 2, 0, 1) tensor(2.500000000000e-03, dtype=torch.float64)\n",
+                        "(0, 1, 1, 1, 1) tensor(-2.500000000000e-04, dtype=torch.float64)\n",
+                        "(0, 1, 0, 2, 1) tensor(6.250000000000e-06, dtype=torch.float64)\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Compute single exponent generator\n",
+                "\n",
+                "h = hamiltonian((2, 1), x, [k], t)\n",
+                "chop(h)\n",
+                "\n",
+                "# Compute series representation\n",
+                "\n",
+                "# Note, each coefficient is proportional to strength\n",
+                "\n",
+                "s = clean(series((4, 1), (3, 1), h))\n",
+                "for index, value in s.items():\n",
+                "    print(index, value.squeeze())"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 11,
+            "id": "0bd97ea3-8875-4b60-904a-59e29890b8ce",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "tensor([1.009811250000e-01, 9.622500000000e-03, 5.102537625000e-02, 1.050752500000e-02],\n",
+                        "       dtype=torch.float64)\n",
+                        "tensor([1.009811250000e-01, 9.622500000000e-03, 5.102537625000e-02, 1.050752500000e-02],\n",
+                        "       dtype=torch.float64)\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# In this example, this hamiltonian generates exact solution with taylor intergator\n",
+                "\n",
+                "print(mapping(x + dx, k + dk, 0.1))\n",
+                "print(taylor(1, 1.0, lambda x, k: evaluate(h, [x, k]), evaluate(l, [dx, dk]), dk))"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "4168324a-1472-4574-9087-e60922704759",
+            "metadata": {},
+            "source": [
+                "# Example-31: Factorization (fodo)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 1,
+            "id": "d50ae1b9-9c66-4f96-b57c-3b6d9be7dae6",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "True\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Import\n",
+                "\n",
+                "import torch\n",
+                "\n",
+                "from ndtorch.derivative import derivative\n",
+                "from ndtorch.signature import chop\n",
+                "from ndtorch.evaluate import evaluate\n",
+                "from ndtorch.evaluate import compare\n",
+                "from ndtorch.propagate import identity\n",
+                "from ndtorch.propagate import propagate\n",
+                "from ndtorch.series import series\n",
+                "from ndtorch.series import clean\n",
+                "from ndtorch.taylor import taylor\n",
+                "from ndtorch.inverse import inverse\n",
+                "from ndtorch.factorization import hamiltonian\n",
+                "from ndtorch.factorization import solution\n",
+                "\n",
+                "torch.set_printoptions(precision=12, sci_mode=True)\n",
+                "print(torch.cuda.is_available())\n",
+                "\n",
+                "import warnings\n",
+                "warnings.filterwarnings(\"ignore\")"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 2,
+            "id": "d1824145-7e9f-45c8-8473-294bb7db7cf5",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [],
+            "source": [
+                "# Set data type and device\n",
+                "\n",
+                "dtype = torch.float64\n",
+                "device = torch.device('cpu')"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 3,
+            "id": "48d3e9e8-cde9-43f6-a74d-6caa49e5d233",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [],
+            "source": [
+                "# Set elements\n",
+                "\n",
+                "def drif(x, w, l):\n",
+                "    (qx, px, qy, py), (w, ), l = x, w, l\n",
+                "    return torch.stack([qx + l*px/(1 + w), px, qy + l*py/(1 + w), py])\n",
+                "\n",
+                "def quad(x, w, kq, l, n=5):\n",
+                "    (qx, px, qy, py), (w, ), kq, l = x, w, kq, l/(2.0*n)\n",
+                "    for _ in range(n):\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "        px, py = px - 2.0*l*kq*qx, py + 2.0*l*kq*qy\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "    return torch.stack([qx, px, qy, py])\n",
+                "\n",
+                "def sext(x, w, ks, l, n=1):\n",
+                "    (qx, px, qy, py), (w, ), ks, l = x, w, ks, l/(2.0*n)\n",
+                "    for _ in range(n):\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "        px, py = px - 1.0*l*ks*(qx**2 - qy**2), py + 2.0*l*ks*qx*qy\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "    return torch.stack([qx, px, qy, py])\n",
+                "\n",
+                "def bend(x, w, r, kq, ks, l, n=10):\n",
+                "    (qx, px, qy, py), (w, ), r, kq, ks, l = x, w, r, kq, ks, l/(2.0*n)\n",
+                "    for _ in range(n):\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "        px, py = px - 2.0*l*kq*qx - 1.0*l*ks*(qx**2 - qy**2) + 2.0*l/r**2*(w*r - qx), py + 2.0*l*kq*qy + 2.0*l*ks*qx*qy\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "    return torch.stack([qx, px, qy, py]) \n",
+                "\n",
+                "def kick(x, cx, cy):\n",
+                "    (qx, px, qy, py) = x\n",
+                "    return torch.stack([qx, px + cx, qy, py + cy])    \n",
+                "\n",
+                "def slip(x, dx, dy):\n",
+                "    (qx, px, qy, py) = x\n",
+                "    return torch.stack([qx + dx, px, qy + dy, py])"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 4,
+            "id": "a877a9b8-31a2-4329-8053-386b10f72dde",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [],
+            "source": [
+                "# Set fodo\n",
+                "\n",
+                "def fodo(x):\n",
+                "    x = quad(x, [0.0], 0.19, 0.50)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = sext(x, [0.0], 0.1, +0.5)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = bend(x, [0.0], 22.92, 0.015, 0.25, 3.0)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = sext(x, [0.0], 0.1, -0.5)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = quad(x, [0.0], -0.21, 0.50)\n",
+                "    x = quad(x, [0.0], -0.21, 0.50)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = sext(x, [0.0], 0.1, -0.5)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = bend(x, [0.0], 22.92, 0.015, 0.25, 3.0)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = sext(x, [0.0], 0.1, +0.5)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = quad(x, [0.0], 0.19, 0.50)\n",
+                "    return x"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 5,
+            "id": "62358986-4d24-49f8-9e60-5facf10c0104",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "tensor([0., 0., 0., 0.], dtype=torch.float64)"
+                        ]
+                    },
+                    "execution_count": 5,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "# Set computation order & evaluation point\n",
+                "\n",
+                "n = 4\n",
+                "x = torch.tensor([0.0, 0.0, 0.0, 0.0], dtype=dtype, device=device)\n",
+                "\n",
+                "# Note, origin is preserved\n",
+                "\n",
+                "fodo(x)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 6,
+            "id": "b43b5788-9b64-414a-99ca-296fc0a1b0b9",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [],
+            "source": [
+                "# Compute derivative table\n",
+                "\n",
+                "t = identity((n, ), [x])\n",
+                "t = propagate((4, ), (n, ), t, [], lambda x: fodo(x))"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 7,
+            "id": "7d23b3ce-06ab-482a-939e-1a798c735974",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "[tensor([0., 0., 0., 0.], dtype=torch.float64),\n",
+                            " tensor([[8.259928915375e-02, 1.470387298165e+01, 0.000000000000e+00, 0.000000000000e+00],\n",
+                            "         [-6.754528950779e-02, 8.259928915375e-02, 0.000000000000e+00, 0.000000000000e+00],\n",
+                            "         [0.000000000000e+00, 0.000000000000e+00, 8.239443265215e-01, 6.857644998910e+00],\n",
+                            "         [0.000000000000e+00, 0.000000000000e+00, -4.682595072274e-02, 8.239443265215e-01]],\n",
+                            "        dtype=torch.float64)]"
+                        ]
+                    },
+                    "execution_count": 7,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "# Set linear part\n",
+                "\n",
+                "l = derivative(1, lambda x: evaluate(t, [x]), x)\n",
+                "l"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 8,
+            "id": "ac3be7e9-12ad-4bf8-986c-3dc318dd5b96",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "[tensor([0., 0., 0., 0.], dtype=torch.float64),\n",
+                            " tensor([[1.000000000000e+00, 0.000000000000e+00, 0.000000000000e+00, 0.000000000000e+00],\n",
+                            "         [0.000000000000e+00, 1.000000000000e+00, 0.000000000000e+00, 0.000000000000e+00],\n",
+                            "         [0.000000000000e+00, 0.000000000000e+00, 1.000000000000e+00, 0.000000000000e+00],\n",
+                            "         [0.000000000000e+00, 0.000000000000e+00, 0.000000000000e+00, 1.000000000000e+00]],\n",
+                            "        dtype=torch.float64)]"
+                        ]
+                    },
+                    "execution_count": 8,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "# Set nonlinear part\n",
+                "\n",
+                "u = propagate((4, ), (n, ), inverse(1, x, [], l), [], t)\n",
+                "chop(u)\n",
+                "derivative(1, lambda x: evaluate(u, [x]), x)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 9,
+            "id": "e614b69d-6596-4ea3-9a69-1eafc23c4994",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [],
+            "source": [
+                "# Compute hamiltonian\n",
+                "\n",
+                "h = hamiltonian((n, ), x, [], u)\n",
+                "chop(h)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 10,
+            "id": "d2a22f41-7484-4fb9-a743-dff32cf7c6d5",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "(3, 0, 0, 0) tensor(5.024988945080e-02, dtype=torch.float64)\n",
+                        "(2, 1, 0, 0) tensor(-8.027849817894e-01, dtype=torch.float64)\n",
+                        "(1, 2, 0, 0) tensor(1.242554019904e+01, dtype=torch.float64)\n",
+                        "(1, 0, 2, 0) tensor(-5.976214487541e-01, dtype=torch.float64)\n",
+                        "(1, 0, 1, 1) tensor(3.719621673904e+00, dtype=torch.float64)\n",
+                        "(1, 0, 0, 2) tensor(-6.659517059512e+00, dtype=torch.float64)\n",
+                        "(0, 3, 0, 0) tensor(-1.465736828313e+02, dtype=torch.float64)\n",
+                        "(0, 1, 2, 0) tensor(7.616595688746e+00, dtype=torch.float64)\n",
+                        "(0, 1, 1, 1) tensor(-6.812652464723e+01, dtype=torch.float64)\n",
+                        "(0, 1, 0, 2) tensor(1.637189795764e+02, dtype=torch.float64)\n",
+                        "(4, 0, 0, 0) tensor(-2.670453079972e-02, dtype=torch.float64)\n",
+                        "(3, 1, 0, 0) tensor(1.592046859279e+00, dtype=torch.float64)\n",
+                        "(2, 2, 0, 0) tensor(-4.015290100155e+01, dtype=torch.float64)\n",
+                        "(2, 0, 2, 0) tensor(1.098921583040e-02, dtype=torch.float64)\n",
+                        "(2, 0, 1, 1) tensor(-1.150214563563e+00, dtype=torch.float64)\n",
+                        "(2, 0, 0, 2) tensor(5.596016324538e+00, dtype=torch.float64)\n",
+                        "(1, 3, 0, 0) tensor(2.720415502394e+02, dtype=torch.float64)\n",
+                        "(1, 1, 2, 0) tensor(9.092563694884e+00, dtype=torch.float64)\n",
+                        "(1, 1, 1, 1) tensor(-7.311435065924e+01, dtype=torch.float64)\n",
+                        "(1, 1, 0, 2) tensor(1.043406910282e+02, dtype=torch.float64)\n",
+                        "(0, 4, 0, 0) tensor(-8.872464473277e+02, dtype=torch.float64)\n",
+                        "(0, 2, 2, 0) tensor(2.515413272498e+01, dtype=torch.float64)\n",
+                        "(0, 2, 1, 1) tensor(6.993401944277e+01, dtype=torch.float64)\n",
+                        "(0, 2, 0, 2) tensor(-3.593047920669e+02, dtype=torch.float64)\n",
+                        "(0, 0, 4, 0) tensor(-1.258999636146e+00, dtype=torch.float64)\n",
+                        "(0, 0, 3, 1) tensor(1.898846058062e+01, dtype=torch.float64)\n",
+                        "(0, 0, 2, 2) tensor(-1.062500223737e+02, dtype=torch.float64)\n",
+                        "(0, 0, 1, 3) tensor(2.608144282259e+02, dtype=torch.float64)\n",
+                        "(0, 0, 0, 4) tensor(-2.419706859670e+02, dtype=torch.float64)\n",
+                        "(5, 0, 0, 0) tensor(3.720153703396e-02, dtype=torch.float64)\n",
+                        "(4, 1, 0, 0) tensor(-2.470046738149e+00, dtype=torch.float64)\n",
+                        "(3, 2, 0, 0) tensor(5.465213020046e+01, dtype=torch.float64)\n",
+                        "(3, 0, 2, 0) tensor(6.994399435987e-02, dtype=torch.float64)\n",
+                        "(3, 0, 1, 1) tensor(-9.734770779462e-01, dtype=torch.float64)\n",
+                        "(3, 0, 0, 2) tensor(5.509140066922e-01, dtype=torch.float64)\n",
+                        "(2, 3, 0, 0) tensor(-7.728896235979e+02, dtype=torch.float64)\n",
+                        "(2, 1, 2, 0) tensor(1.614402519455e+01, dtype=torch.float64)\n",
+                        "(2, 1, 1, 1) tensor(-1.014114400601e+02, dtype=torch.float64)\n",
+                        "(2, 1, 0, 2) tensor(2.099498728183e+02, dtype=torch.float64)\n",
+                        "(1, 4, 0, 0) tensor(6.599464974629e+03, dtype=torch.float64)\n",
+                        "(1, 2, 2, 0) tensor(-1.831472433171e+02, dtype=torch.float64)\n",
+                        "(1, 2, 1, 1) tensor(1.658609587412e+03, dtype=torch.float64)\n",
+                        "(1, 2, 0, 2) tensor(-4.455648121228e+03, dtype=torch.float64)\n",
+                        "(1, 0, 4, 0) tensor(-2.372154036991e+00, dtype=torch.float64)\n",
+                        "(1, 0, 3, 1) tensor(3.120364861986e+01, dtype=torch.float64)\n",
+                        "(1, 0, 2, 2) tensor(-1.392873544053e+02, dtype=torch.float64)\n",
+                        "(1, 0, 1, 3) tensor(2.280297561995e+02, dtype=torch.float64)\n",
+                        "(1, 0, 0, 4) tensor(-5.830536198793e+01, dtype=torch.float64)\n",
+                        "(0, 5, 0, 0) tensor(-1.712807218852e+04, dtype=torch.float64)\n",
+                        "(0, 3, 2, 0) tensor(-5.278629070820e+02, dtype=torch.float64)\n",
+                        "(0, 3, 1, 1) tensor(3.474912442117e+03, dtype=torch.float64)\n",
+                        "(0, 3, 0, 2) tensor(1.999757814650e+02, dtype=torch.float64)\n",
+                        "(0, 1, 4, 0) tensor(2.874466602579e+01, dtype=torch.float64)\n",
+                        "(0, 1, 3, 1) tensor(-5.199961828427e+02, dtype=torch.float64)\n",
+                        "(0, 1, 2, 2) tensor(3.267795295152e+03, dtype=torch.float64)\n",
+                        "(0, 1, 1, 3) tensor(-8.677457594504e+03, dtype=torch.float64)\n",
+                        "(0, 1, 0, 4) tensor(8.128231575922e+03, dtype=torch.float64)\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Compute series representation\n",
+                "\n",
+                "s = clean(series((4, ), (n + 1, ), h), epsilon=1.0E-9)\n",
+                "for index, value in s.items():\n",
+                "    print(index, value.squeeze())"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 11,
+            "id": "f5bfe2b0-5796-45f5-8785-f30ed8a32cd6",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "True\n",
+                        "True\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Restore mapping table nonlinear part from hamiltonian\n",
+                "\n",
+                "print(compare(u, solution((n, ), x, [], h)))\n",
+                "print(compare(t, propagate((4, ), (n, ), l, [], solution((n, ), x, [], h))))"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "b6d8236a-9e84-47e0-ab5f-003cc8fd7f92",
+            "metadata": {},
+            "source": [
+                "# Example-32: Factorization (factorize)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 1,
+            "id": "ba8720f6-ac3f-447d-b74a-5f2a7cc5ed65",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "True\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Import\n",
+                "\n",
+                "import torch\n",
+                "from ndtorch.derivative import derivative\n",
+                "from ndtorch.signature import chop\n",
+                "from ndtorch.evaluate import evaluate\n",
+                "from ndtorch.evaluate import compare\n",
+                "from ndtorch.series import series\n",
+                "from ndtorch.series import clean\n",
+                "from ndtorch.series import split\n",
+                "from ndtorch.propagate import identity\n",
+                "from ndtorch.propagate import propagate\n",
+                "from ndtorch.bracket import bracket\n",
+                "from ndtorch.factorization import hamiltonian\n",
+                "from ndtorch.factorization import solution\n",
+                "from ndtorch.factorization import factorize\n",
+                "\n",
+                "torch.set_printoptions(precision=12, sci_mode=True)\n",
+                "print(torch.cuda.is_available())\n",
+                "\n",
+                "import warnings\n",
+                "warnings.filterwarnings(\"ignore\")"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 2,
+            "id": "f459d7a8-0c87-45a8-be50-3c6e0eaf4815",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [],
+            "source": [
+                "# Set data type and device\n",
+                "\n",
+                "dtype = torch.float64\n",
+                "device = torch.device('cpu')"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 3,
+            "id": "017b340b-4d9c-42ba-ad8b-c6a410514e10",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "{(3, 0, 0, 0): tensor(1.000000000000e+00, dtype=torch.float64),\n",
+                            " (2, 1, 0, 0): tensor(1.000000000000e+00, dtype=torch.float64),\n",
+                            " (1, 2, 0, 0): tensor(1.000000000000e+00, dtype=torch.float64),\n",
+                            " (0, 3, 0, 0): tensor(1.000000000000e+00, dtype=torch.float64),\n",
+                            " (3, 0, 1, 0): tensor(1.000000000000e+00, dtype=torch.float64),\n",
+                            " (3, 0, 2, 0): tensor(1.000000000000e+00, dtype=torch.float64),\n",
+                            " (4, 0, 0, 0): tensor(1.000000000000e+00, dtype=torch.float64),\n",
+                            " (3, 1, 0, 0): tensor(1.000000000000e+00, dtype=torch.float64),\n",
+                            " (2, 2, 0, 0): tensor(1.000000000000e+00, dtype=torch.float64),\n",
+                            " (1, 3, 0, 0): tensor(1.000000000000e+00, dtype=torch.float64),\n",
+                            " (0, 4, 0, 0): tensor(1.000000000000e+00, dtype=torch.float64),\n",
+                            " (4, 0, 0, 1): tensor(1.000000000000e+00, dtype=torch.float64),\n",
+                            " (5, 0, 0, 0): tensor(1.000000000000e+00, dtype=torch.float64),\n",
+                            " (4, 1, 0, 0): tensor(1.000000000000e+00, dtype=torch.float64),\n",
+                            " (3, 2, 0, 0): tensor(1.000000000000e+00, dtype=torch.float64),\n",
+                            " (2, 3, 0, 0): tensor(1.000000000000e+00, dtype=torch.float64),\n",
+                            " (1, 4, 0, 0): tensor(1.000000000000e+00, dtype=torch.float64),\n",
+                            " (0, 5, 0, 0): tensor(1.000000000000e+00, dtype=torch.float64)}"
+                        ]
+                    },
+                    "execution_count": 3,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "# Set test hamiltonian function and compute corresponding table representation\n",
+                "\n",
+                "# Note, test hamiltonian is near identity\n",
+                "\n",
+                "def h(x, u, v):\n",
+                "    q, p = x\n",
+                "    u, = u\n",
+                "    v, = v\n",
+                "    h1 = (1 + u + u**2)*q**3 + q**2*p + q*p**2 + p**3\n",
+                "    h2 = (1 + v)*q**4 + q**3*p + q**2*p**2 + q*p**3 + p**4\n",
+                "    h3 = q**5 + q**4*p + q**3*p**2 + q**2*p**3 + q*p**4 + p**5\n",
+                "    return h1 + h2 + h3\n",
+                "\n",
+                "x = torch.tensor([0.0, 0.0], dtype=dtype, device=device)\n",
+                "u = torch.tensor([0.0], dtype=dtype, device=device)\n",
+                "v = torch.tensor([0.0], dtype=dtype, device=device)\n",
+                "\n",
+                "h = derivative((5, 2, 1), h, x, u, v)\n",
+                "chop(h, replace=True)\n",
+                "\n",
+                "s, *_ = split(clean(series((2, 1, 1), (5, 2, 1), h)))\n",
+                "s"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 4,
+            "id": "1fcb9c0c-4136-49b9-9639-9532c15155b8",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [],
+            "source": [
+                "# Compute solution\n",
+                "\n",
+                "t = solution((4, 2, 1), x, [u, v], h)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 5,
+            "id": "c30313c7-b21d-4a38-9a1b-36651a60691e",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "True"
+                        ]
+                    },
+                    "execution_count": 5,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "# Compute hamiltonian from solution and compare\n",
+                "\n",
+                "compare(h, hamiltonian((4, 2, 1), x, [u, v], t))"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 6,
+            "id": "c7e423a0-73e0-4c22-8d83-6648b670f1f7",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [],
+            "source": [
+                "# Perform factorization\n",
+                "\n",
+                "h1, h2, h3, *_ = factorize((4, 2, 1), x, [u, v], t)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 7,
+            "id": "9a14155f-01b8-4224-a93f-55610417aa9a",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "{(3, 0, 0, 0): tensor(1.000000000000e+00, dtype=torch.float64),\n",
+                            " (2, 1, 0, 0): tensor(1.000000000000e+00, dtype=torch.float64),\n",
+                            " (1, 2, 0, 0): tensor(1.000000000000e+00, dtype=torch.float64),\n",
+                            " (0, 3, 0, 0): tensor(1.000000000000e+00, dtype=torch.float64),\n",
+                            " (3, 0, 1, 0): tensor(1.000000000000e+00, dtype=torch.float64)}"
+                        ]
+                    },
+                    "execution_count": 7,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "# Examine series representation\n",
+                "\n",
+                "s, *_ = split(clean(series((2, 1, 1), (5, 1), h1)))\n",
+                "s"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 8,
+            "id": "4c099717-836f-48b6-9dbb-84a3b9ce5455",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "{(4, 0, 0, 0): tensor(1.000000000000e+00, dtype=torch.float64),\n",
+                            " (3, 1, 0, 0): tensor(1.000000000000e+00, dtype=torch.float64),\n",
+                            " (2, 2, 0, 0): tensor(1.000000000000e+00, dtype=torch.float64),\n",
+                            " (1, 3, 0, 0): tensor(1.000000000000e+00, dtype=torch.float64),\n",
+                            " (0, 4, 0, 0): tensor(1.000000000000e+00, dtype=torch.float64),\n",
+                            " (4, 0, 0, 1): tensor(1.000000000000e+00, dtype=torch.float64)}"
+                        ]
+                    },
+                    "execution_count": 8,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "# Examine series representation\n",
+                "\n",
+                "s, *_ = split(clean(series((2, 1, 1), (5, 1), h2)))\n",
+                "s"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 9,
+            "id": "1f97e5ac-3cdb-4b24-a8bf-0e8c15d8a17f",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "{(5, 0, 0, 0): tensor(5.000000000000e-01, dtype=torch.float64),\n",
+                            " (4, 1, 0, 0): tensor(-5.000000000000e-01, dtype=torch.float64),\n",
+                            " (3, 2, 0, 0): tensor(-2.000000000000e+00, dtype=torch.float64),\n",
+                            " (2, 3, 0, 0): tensor(4.000000000000e+00, dtype=torch.float64),\n",
+                            " (1, 4, 0, 0): tensor(2.500000000000e+00, dtype=torch.float64),\n",
+                            " (0, 5, 0, 0): tensor(1.500000000000e+00, dtype=torch.float64),\n",
+                            " (5, 0, 0, 1): tensor(-2.000000000000e+00, dtype=torch.float64),\n",
+                            " (4, 1, 0, 1): tensor(-4.000000000000e+00, dtype=torch.float64),\n",
+                            " (3, 2, 0, 1): tensor(-6.000000000000e+00, dtype=torch.float64),\n",
+                            " (5, 0, 1, 0): tensor(1.500000000000e+00, dtype=torch.float64),\n",
+                            " (4, 1, 1, 0): tensor(3.000000000000e+00, dtype=torch.float64),\n",
+                            " (3, 2, 1, 0): tensor(4.500000000000e+00, dtype=torch.float64),\n",
+                            " (2, 3, 1, 0): tensor(6.000000000000e+00, dtype=torch.float64)}"
+                        ]
+                    },
+                    "execution_count": 9,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "# Examine series representation\n",
+                "\n",
+                "s, *_ = split(clean(series((2, 1, 1), (5, 1), h3)))\n",
+                "s"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 10,
+            "id": "fef41af0-cc19-4eaf-bc96-def01749691d",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [],
+            "source": [
+                "# Compute solutions\n",
+                "\n",
+                "t1 = solution((4, 2, 1), x, [u, v], h1)\n",
+                "t2 = solution((4, 2, 1), x, [u, v], h2)\n",
+                "t3 = solution((4, 2, 1) ,x, [u, v], h3)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 11,
+            "id": "5d3545d6-d9d4-40ee-bb5f-6b97bb268509",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "True"
+                        ]
+                    },
+                    "execution_count": 11,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "# Compose individual solutions and compare with initial solution\n",
+                "\n",
+                "T = identity((4, 2, 1), [x, u, v])\n",
+                "T = propagate((2, 1, 1), (4, 2, 1), T, [u, v], t1)\n",
+                "T = propagate((2, 1, 1), (4, 2, 1), T, [u, v], t2)\n",
+                "T = propagate((2, 1, 1), (4, 2, 1), T, [u, v], t3)\n",
+                "compare(t, T)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "bae67b59-1584-4879-9255-8096c603f900",
+            "metadata": {},
+            "outputs": [],
+            "source": []
         }
     ],
     "metadata": {
         "colab": {
             "collapsed_sections": [
                 "myt0_gMIOq7b",
                 "5d97819c"
@@ -11672,15 +12201,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.10"
+            "version": "3.11.2"
         },
         "latex_envs": {
             "LaTeX_envs_menu_present": true,
             "autoclose": false,
             "autocomplete": true,
             "bibliofile": "biblio.bib",
             "cite_by": "apalike",
```

### Comparing `ndtorch-0.1.5/docs/source/index.rst` & `ndtorch-0.1.6/docs/source/index.rst`

 * *Files 3% similar despite different names*

```diff
@@ -18,26 +18,29 @@
 
 .. toctree::
    :caption: API:
    :maxdepth: 1
 
    modules/util.rst
    modules/derivative.rst
+   modules/gradient.rst
+   modules/complex.rst
    modules/signature.rst
    modules/index.rst
    modules/series.rst
    modules/evaluate.rst
    modules/propagate.rst
    modules/pfp.rst
    modules/bracket.rst
    modules/taylor.rst
    modules/yoshida.rst
    modules/invariant.rst
    modules/inverse.rst
    modules/momenta.rst
+   modules/factorization.rst
    modeles/matrix.rst
    modules/jet.rst
 
 Indices and tables
 ==================
 
 * :ref:`genindex`
```

### Comparing `ndtorch-0.1.5/ndtorch/__init__.py` & `ndtorch-0.1.6/ndtorch/__init__.py`

 * *Files identical despite different names*

### Comparing `ndtorch-0.1.5/ndtorch/bracket.py` & `ndtorch-0.1.6/ndtorch/bracket.py`

 * *Files identical despite different names*

### Comparing `ndtorch-0.1.5/ndtorch/derivative.py` & `ndtorch-0.1.6/ndtorch/derivative.py`

 * *Files identical despite different names*

### Comparing `ndtorch-0.1.5/ndtorch/evaluate.py` & `ndtorch-0.1.6/ndtorch/evaluate.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 from multimethod import multimethod
 
 import torch
 from torch import Tensor
 
 from .util import flatten
 from .derivative import derivative
+from .signature import signature
+from .signature import get
 
 
 State       : TypeAlias = Tensor
 Knobs       : TypeAlias = list[Tensor]
 Point       : TypeAlias = list[Tensor]
 Delta       : TypeAlias = list[Tensor]
 Table       : TypeAlias = list
@@ -135,15 +137,15 @@
     >>> dy = 1.0E-3*torch.ones_like(x)
     >>> torch.allclose(fn(x + dx, y + dy), evaluate(s, [dx, dy]))
 
     """
     state = torch.cat(delta)
 
     if epsilon is not None:
-        state = epsilon + state
+        state = state + 0*(epsilon + torch.sin(state.sum()))
         index = torch.tensor([*series.keys()], dtype=torch.int64, device=state.device)
         value = torch.stack([*series.values()])
         return (value.T*(state**index).prod(-1)).sum(-1)
 
     total, *_ = series.values()
     total = torch.zeros_like(total)
     for key, value in series.items():
@@ -210,15 +212,14 @@
 
     value, *_ = series.values()
     delta = [torch.zeros(i, dtype=value.dtype, device=value.device) for i in dimension]
 
     return derivative(order, function, delta, intermediate=True, jacobian=jacobian)
 
 
-@multimethod
 def compare(probe:Table, other:Table) -> bool:
     """
     Compare tables
 
     Parameters
     ----------
     probe, other: Table
@@ -239,48 +240,14 @@
     >>> x = torch.tensor([0.0, 0.0])
     >>> y = torch.zeros_like(x)
     >>> t = derivative((2, 1), fn, x, y)
     >>> compare(t, t)
     True
 
     """
-    for x, y in zip(*map(lambda array: flatten(array, target=list), [probe, other])):
-        if not torch.allclose(x, y):
-            return False
-    return True
-
-
-@multimethod
-def compare(probe:Series, other:Series) -> bool:
-    """
-    Compare series
-
-    Parameters
-    ----------
-    probe, other: Series
-        series to compare
-
-    Returns
-    -------
-    bool
-
-    Examples
-    --------
-    >>> import torch
-    >>> from ndtorch.derivative import derivative
-    >>> from ndtorch.series import series
-    >>> def fn(x, y):
-    ...    x1, x2 = x
-    ...    y1, y2 = y
-    ...    return torch.stack([x1*(1 + y1), x2*(1 + y2)])
-    >>> x = torch.tensor([0.0, 0.0])
-    >>> y = torch.zeros_like(x)
-    >>> t = derivative((2, 1), fn, x, y)
-    >>> s = series((2, 2), (2, 1), t)
-    >>> compare(s, s)
-    True
-
-    """
-    for x, y in zip(probe.values(), other.values()):
-        if not torch.allclose(x, y):
-            return False
+    for i in signature(probe):
+        x = get(probe, i)
+        y = get(other, i)
+        if isinstance(x, Tensor) and isinstance(y, Tensor):
+            if not torch.allclose(x, y):
+                return False
     return True
```

### Comparing `ndtorch-0.1.5/ndtorch/index.py` & `ndtorch-0.1.6/ndtorch/index.py`

 * *Files identical despite different names*

### Comparing `ndtorch-0.1.5/ndtorch/inverse.py` & `ndtorch-0.1.6/ndtorch/inverse.py`

 * *Files 12% similar despite different names*

```diff
@@ -67,59 +67,63 @@
     Table
 
     Examples
     --------
     >>> import torch
     >>> from ndtorch.derivative import derivative
     >>> from ndtorch.propagate import propagate
-    >>> def fn(x, k):
+    >>> def fn(x):
     ...     q, p = x
-    ...     a, b = k
-    ...     return torch.stack([q, p + (1 + a)*q + (1 + b)*q**2])
+    ...     return torch.stack([q, p + q + q**2])
     >>> x = torch.tensor([0.0, 0.0], dtype=torch.float64)
     >>> t = derivative((2, ), fn, x)
     >>> inverse((2, ), x, [], t)
-    [tensor([0., 0.], dtype=torch.float64),
+    [[],
     tensor([[ 1.,  0.],
             [-1.,  1.]], dtype=torch.float64),
     tensor([[[ 0.,  0.],
             [ 0.,  0.]],
+    
             [[-2.,  0.],
             [ 0.,  0.]]], dtype=torch.float64)]
 
     >>> import torch
     >>> from ndtorch.derivative import derivative
     >>> from ndtorch.propagate import propagate
     >>> def fn(x, k):
     ...     q, p = x
     ...     a, b = k
     ...     return torch.stack([q, p + (1 + a)*q + (1 + b)*q**2])
     >>> x = torch.tensor([0.0, 0.0], dtype=torch.float64)
     >>> k = torch.tensor([0.0, 0.0], dtype=torch.float64)
     >>> t = derivative((2, 1), fn, x, k)
     >>> inverse((2, 1), x, [k], t)
-    [[tensor([0., 0.], dtype=torch.float64),
-    tensor([[0., 0.],
-            [0., 0.]], dtype=torch.float64)],
+    [[[], []],
     [tensor([[ 1.,  0.],
             [-1.,  1.]], dtype=torch.float64),
     tensor([[[ 0.,  0.],
             [ 0.,  0.]],
+    
             [[-1.,  0.],
             [ 0.,  0.]]], dtype=torch.float64)],
     [tensor([[[ 0.,  0.],
             [ 0.,  0.]],
+    
             [[-2.,  0.],
             [ 0.,  0.]]], dtype=torch.float64),
     tensor([[[[ 0.,  0.],
                 [ 0.,  0.]],
+    
             [[ 0.,  0.],
                 [ 0.,  0.]]],
+    
+    
             [[[ 0.,  0.],
                 [ 0.,  0.]],
+    
             [[-2.,  0.],
                 [ 0.,  0.]]]], dtype=torch.float64)]]
 
     """
     if solve is None:
         def solve(matrix, vector):
             return torch.linalg.lstsq(matrix, vector.unsqueeze(1)).solution.squeeze()
@@ -153,14 +157,15 @@
         *_, local = reduce(dimension, index, local)
         return torch.stack([*local.values()]).flatten()
 
     array = signature(data)
 
     for i in array:
         if not first(i):
+            set(result, i, [])
             continue
         guess = get(result, i)
         sequence, shape, unique = reduce(dimension, i, guess)
         guess = torch.stack([*unique.values()]).flatten()
         values = newton(objective,
                         guess,
                         i,
```

### Comparing `ndtorch-0.1.5/ndtorch/jet.py` & `ndtorch-0.1.6/ndtorch/jet.py`

 * *Files identical despite different names*

### Comparing `ndtorch-0.1.5/ndtorch/matrix.py` & `ndtorch-0.1.6/ndtorch/matrix.py`

 * *Files identical despite different names*

### Comparing `ndtorch-0.1.5/ndtorch/momenta.py` & `ndtorch-0.1.6/ndtorch/momenta.py`

 * *Files identical despite different names*

### Comparing `ndtorch-0.1.5/ndtorch/pfp.py` & `ndtorch-0.1.6/ndtorch/pfp.py`

 * *Files identical despite different names*

### Comparing `ndtorch-0.1.5/ndtorch/propagate.py` & `ndtorch-0.1.6/ndtorch/propagate.py`

 * *Files identical despite different names*

### Comparing `ndtorch-0.1.5/ndtorch/series.py` & `ndtorch-0.1.6/ndtorch/series.py`

 * *Files identical despite different names*

### Comparing `ndtorch-0.1.5/ndtorch/signature.py` & `ndtorch-0.1.6/ndtorch/signature.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 from typing import TypeAlias
 from typing import Callable
 from typing import Union
 
 from multimethod import multimethod
 
+import torch
 from torch import Tensor
 
 from .util import flatten
 
 
 State       : TypeAlias = Tensor
 Knobs       : TypeAlias = list[Tensor]
@@ -27,14 +28,77 @@
 Signature   : TypeAlias = Union[list[tuple[int, ...]], list[tuple[tuple[int, ...], float]]]
 Mapping     : TypeAlias = Callable
 Observable  : TypeAlias = Callable
 Hamiltonian : TypeAlias = Callable
 
 
 @multimethod
+def signature(order:tuple[int, ...], *,
+              factor:bool=False) -> Signature:
+    """
+    Compute derivative table bottom elements signatures from given orders
+
+    Parameters
+    ----------
+    order: tuple[int, ...]
+        table order
+    fator: bool, default=True
+        flag to return elements multipliation factors
+
+    Returns
+    -------
+    Signature
+        bottom table elements signatures
+
+    Examples
+    --------
+    >>> import torch
+    >>> from ndtorch.derivative import derivative
+    >>> def fn(x, y):
+    ...    x1, x2 = x
+    ...    y1, y2 = y
+    ...    return (x1 + x2 + x1**2 + x1*x2 + x2**2)*(1 + y1 + y2)
+    >>> x = torch.tensor([0.0, 0.0])
+    >>> y = torch.zeros_like(x)
+    >>> signature((2, 1))
+    [(0, 0), (0, 1), (1, 0), (1, 1), (2, 0), (2, 1)]
+    >>> signature((2, 1), factor=True)
+    [((0, 0), 1.0),
+     ((0, 1), 1.0),
+     ((1, 0), 1.0),
+     ((1, 1), 1.0),
+     ((2, 0), 0.5),
+     ((2, 1), 0.5)]
+    
+    """
+    length = len(order)
+
+    def generate(order, local, indices):
+        if length == len(local):
+            indices.append(tuple(local))
+        else:
+            for i in range(order[len(local)] + 1):
+                generate(order, local + [i], indices)
+
+    indices = []
+    generate(order, [], indices)
+
+    if not factor:
+        return indices
+
+    result = []
+    for index in indices:
+        value = 1.0
+        for count in index:
+            value *= 1.0/factorial(count)
+        result.append((index, value))
+
+    return result
+
+@multimethod
 def signature(table:Table, *,
               factor:bool=False) -> Signature:
     """
     Compute derivative table bottom elements signatures
 
     Note, signature elements corresponds to the bottom elements of a flattened derivative table
     Bottom element signature is a tuple integers, derivative orders with respect to each tensor
@@ -94,15 +158,16 @@
     """ (auxiliary) """
     value = 1.0
     for count in index:
         value *= 1.0/factorial(count)
     return tuple(index) if not factor else (tuple(index), value)
 
 
-def get(table:Table, index:tuple[int, ...]) -> Union[Tensor, Table]:
+def get(table:Table,
+        index:tuple[int, ...]) -> Union[Tensor, Table]:
     """
     Get derivative table element at a given (bottom) element signature
 
     Note, index can correspond to a bottom element or a subtable
 
     Parameters
     ----------
@@ -137,15 +202,17 @@
 
     *ns, n = index
     for i in ns:
         table = table[i]
     return table[n]
 
 
-def set(table:Table, index:tuple[int, ...], value:Union[Tensor, Table]) -> None:
+def set(table:Table,
+        index:tuple[int, ...],
+        value:Union[Tensor, Table]) -> None:
     """
     Set derivative table element at a given (bottom) element signature
 
     Note, index can correspond to a bottom element or a subtable
 
     Parameters
     ----------
@@ -184,15 +251,17 @@
     *ns, n = index
     for i in ns:
         table = table[i]
     table[n] = value
 
 
 @multimethod
-def apply(table:Table, index:tuple[int, ...], function:Callable) -> None:
+def apply(table:Table,
+          index:tuple[int, ...],
+          function:Callable) -> None:
     """
     Apply function (modifies element at index)
 
     Note, index can correspond to a bottom element or a subtable
 
     Parameters
     ----------
@@ -225,15 +294,17 @@
 
     """
     value = get(table, index)
     set(table, index, function(value))
 
 
 @multimethod
-def apply(table:Table, index:list[tuple[int, ...]], function:Callable) -> None:
+def apply(table:Table,
+          index:list[tuple[int, ...]],
+          function:Callable) -> None:
     """
     Apply function (modifies element at list of indices)
 
     Parameters
     ----------
     table: Table
         input derivative table representation
@@ -260,19 +331,21 @@
     >>> apply(t, [(1, 0), (1, 1)], torch.log)
     >>> get(t, [(1)])
     [tensor([0., 0.]),
     tensor([[0., 0.],
             [0., 0.]])]
 
     """
-    [*map(lambda index: apply(table, index, function), index)]
+    for i in index:
+        apply(table, i, function)
 
 
 @multimethod
-def apply(table:Table, function:Callable) -> None:
+def apply(table:Table,
+          function:Callable) -> None:
     """
     Apply function to all bottom elements
 
     Parameters
     ----------
     table: Table
         input derivative table representation
@@ -300,26 +373,31 @@
      [tensor(1.4142), tensor(2.)],
      [tensor(3.1623), tensor(4.4721)]]
 
     """
     apply(table, signature(table), function)
 
 
-def chop(table:Table, threshold:float=1.0E-9, value:float=0.0) -> None:
+def chop(table:Table, *,
+         threshold:float=1.0E-9,
+         value:float=0.0,
+         replace:bool=False) -> None:
     """
     Chop tensor elements in a table below a given threshold
 
     Parameters
     ----------
     table: Table
         input derivative table representation
     threshold: float, default=1.0E-9
         threshold value
     value: float, default=0.0
         set value
+    replace: bool, default=False
+        flag to replace zero tensors
 
     Returns
     -------
     None
 
     Examples
     --------
@@ -337,14 +415,16 @@
     >>> t
     [[tensor(0.), tensor([0., 0.])]]
 
     """
     def inner(tensor):
         tensor = tensor.clone()
         tensor[tensor.abs() < threshold] = value
+        if replace and torch.allclose(tensor, torch.zeros_like(tensor)):
+            tensor = []
         return tensor
     apply(table, inner)
 
 
 def to(table:Table,
        *args:tuple,
        **kwargs:dict) -> None:
```

### Comparing `ndtorch-0.1.5/ndtorch/taylor.py` & `ndtorch-0.1.6/ndtorch/taylor.py`

 * *Files identical despite different names*

### Comparing `ndtorch-0.1.5/ndtorch/util.py` & `ndtorch-0.1.6/ndtorch/util.py`

 * *Files identical despite different names*

### Comparing `ndtorch-0.1.5/ndtorch/yoshida.py` & `ndtorch-0.1.6/ndtorch/yoshida.py`

 * *Files identical despite different names*

### Comparing `ndtorch-0.1.5/ndtorch.egg-info/SOURCES.txt` & `ndtorch-0.1.6/ndtorch.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -11,16 +11,19 @@
 docs/pics/collision.gif
 docs/pics/logo.svg
 docs/pics/manifold.gif
 docs/source/conf.py
 docs/source/index.rst
 docs/source/examples/ndtorch.ipynb
 docs/source/modules/bracket.rst
+docs/source/modules/complex.rst
 docs/source/modules/derivative.rst
 docs/source/modules/evaluate.rst
+docs/source/modules/factorization.rst
+docs/source/modules/gradient.rst
 docs/source/modules/index.rst
 docs/source/modules/invariant.rst
 docs/source/modules/inverse.rst
 docs/source/modules/jet.rst
 docs/source/modules/matrix.rst
 docs/source/modules/momenta.rst
 docs/source/modules/pfp.rst
@@ -28,26 +31,31 @@
 docs/source/modules/series.rst
 docs/source/modules/signature.rst
 docs/source/modules/taylor.rst
 docs/source/modules/util.rst
 docs/source/modules/yoshida.rst
 ndtorch/__init__.py
 ndtorch/bracket.py
+ndtorch/complex.py
 ndtorch/derivative.py
 ndtorch/evaluate.py
+ndtorch/expression.py
+ndtorch/factorization.py
+ndtorch/gradient.py
 ndtorch/index.py
 ndtorch/invariant.py
 ndtorch/inverse.py
 ndtorch/jet.py
 ndtorch/matrix.py
 ndtorch/momenta.py
 ndtorch/pfp.py
 ndtorch/propagate.py
 ndtorch/series.py
 ndtorch/signature.py
+ndtorch/symplectify.py
 ndtorch/taylor.py
 ndtorch/util.py
 ndtorch/yoshida.py
 ndtorch.egg-info/PKG-INFO
 ndtorch.egg-info/SOURCES.txt
 ndtorch.egg-info/dependency_links.txt
 ndtorch.egg-info/requires.txt
```

### Comparing `ndtorch-0.1.5/ndtorch.ipynb` & `ndtorch-0.1.6/ndtorch.ipynb`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9868812378770304%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(4, '# Derivatives are computed by nesting torch jacobian "*

 * *            "functions\\n'), (5, '# For higher order derivatives, nesting results in exponentially "*

 * *            "growing redundant computations\\n'), (6, '# Note, forward mode is more memory "*

 * *            "efficient in this case\\n'), (9, '# This representation can be evaluated near given "*

 * *            'evaluation point (at a given deviation) if the input function returns a scalar or a '*

 * *            "vector\\n […]*

```diff
@@ -17,20 +17,21 @@
             },
             "outputs": [],
             "source": [
                 "# Given an input function, its higher order (partial) derivatives with respect to one or sevaral tensor arguments can be computed using forward or reverse mode automatic differentiation\n",
                 "# Derivative orders can be different for each tensor argument\n",
                 "# Input function is expected to return a tensor or a (nested) list of tensors\n",
                 "\n",
-                "# Derivatives are computed by nesting torch.func jacobian functions\n",
-                "# For higher order derivatives, this results in growing redundant computations, forward mode is more efficient in this case\n",
+                "# Derivatives are computed by nesting torch jacobian functions\n",
+                "# For higher order derivatives, nesting results in exponentially growing redundant computations\n",
+                "# Note, forward mode is more memory efficient in this case\n",
                 "\n",
                 "# If the input function returns a tensor, the output is referred as derivative table representation\n",
-                "# This representation can be evaluated near given evaluation point if the input function returns a scalar or a vector\n",
-                "# Table representation is a (nested) list of tensors, it can be used as a (redundant) function representation near given evaluation point\n",
+                "# This representation can be evaluated near given evaluation point (at a given deviation) if the input function returns a scalar or a vector\n",
+                "# Table representation is a (nested) list of tensors, it can be used as a redundant function representation near given evaluation point (taylor series)\n",
                 "# Table structure for f(x), f(x, y) and f(x, y, z) is shown bellow (similar structure holds for a function with more aruments)\n",
                 "\n",
                 "# f(x)\n",
                 "# t(f, x)\n",
                 "# [f, Dx f, Dxx f, ...]\n",
                 "\n",
                 "# f(x, y)\n",
@@ -125,23 +126,23 @@
             "source": [
                 "# Basic derivative interface\n",
                 "\n",
                 "# derivative(\n",
                 "#     order:int,                             # derivative order\n",
                 "#     function:Callable,                     # input function\n",
                 "#     *args,                                 # function(*args) = function(x:Tensor, ...)\n",
-                "#     intermediate:bool = True,              # flag to return intermediate derivatives\n",
+                "#     intermediate:bool = True,              # flag to return all intermediate derivatives\n",
                 "#     jacobian:Callable = torch.func.jacfwd  # torch.func.jacfwd or torch.func.jacfrev\n",
                 "# )\n",
                 "\n",
                 "# derivative(\n",
                 "#     order:tuple[int, ...],                 # derivative orders\n",
                 "#     function:Callable,                     # input function\n",
                 "#     *args,                                 # function(*args) = function(x:Tensor, y:Tensor, z:Tensor, ...)\n",
-                "#     intermediate:bool = True,              # flag to return intermediate derivatives\n",
+                "#     intermediate:bool = True,              # flag to return all intermediate derivatives\n",
                 "#     jacobian:Callable = torch.func.jacfwd  # torch.func.jacfwd or torch.func.jacfrev\n",
                 "# )"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 5,
@@ -164,14 +165,15 @@
             "source": [
                 "# Derivative\n",
                 "\n",
                 "# Input:  scalar\n",
                 "# Output: scalar\n",
                 "\n",
                 "# Set test function\n",
+                "\n",
                 "# Note, the first function argument is a scalar tensor\n",
                 "# Input function can have other additional arguments\n",
                 "# Other arguments are not used in computation of derivatives\n",
                 "\n",
                 "def fn(x, a, b, c, d, e, f):\n",
                 "    return a + b*x + c*x**2 + d*x**3 + e*x**4 + f*x**5\n",
                 "\n",
@@ -189,15 +191,16 @@
                 "\n",
                 "# Compute n'th derivative\n",
                 "\n",
                 "value = derivative(n, fn, x, a, b, c, d, e, f, intermediate=False, jacobian=torch.func.jacfwd)\n",
                 "print(value.cpu().numpy().tolist())\n",
                 "\n",
                 "# Compute all derivatives upto given order\n",
-                "# Note, function value itself is referred as zeros order derivative\n",
+                "\n",
+                "# Note, function value itself is referred as zero order derivative\n",
                 "# Since function returns a tensor, output is a list of tensors\n",
                 "\n",
                 "values = derivative(n, fn, x, a, b, c, d, e, f, intermediate=True, jacobian=torch.func.jacfwd)\n",
                 "print(*[value.cpu().numpy().tolist() for value in values], sep=', ')\n",
                 "\n",
                 "# Note, intermediate flag (default=True) can be used to return all derivatives\n",
                 "# For jacobian parameter, torch.func.jacfwd or torch.func.jacrev functions can be passed\n",
@@ -234,14 +237,15 @@
             "source": [
                 "# Derivative\n",
                 "\n",
                 "# Input:  vector\n",
                 "# Output: scalar\n",
                 "\n",
                 "# Set test function\n",
+                "\n",
                 "# Note, the first function argument is a vector tensor\n",
                 "# Input function can have other additional arguments\n",
                 "# Other arguments are not used in computation of derivatives\n",
                 "\n",
                 "def fn(x, a, b, c):\n",
                 "    x1, x2 = x\n",
                 "    return a + b*(x1 - 1)**2 + c*(x2 + 1)**2\n",
@@ -255,27 +259,29 @@
                 "x = torch.tensor([0.0, 0.0], dtype=dtype, device=device)\n",
                 "\n",
                 "# Set fixed parameters\n",
                 "\n",
                 "a, b, c = torch.tensor([1.0, 1.0, 1.0], dtype=dtype, device=device)\n",
                 "\n",
                 "# Compute only n'th derivative\n",
-                "# Note, for given input & output the result is hessian\n",
+                "\n",
+                "# Note, for given input & output the result is a hessian\n",
                 "\n",
                 "value = derivative(n, fn, x, a, b, c, intermediate=False, jacobian=torch.func.jacfwd)\n",
                 "print(value.cpu().numpy().tolist())\n",
                 "\n",
                 "# Compute all derivatives upto given order\n",
-                "# Note, fuction value itself is referred as zeros order derivative\n",
+                "\n",
+                "# Note, fuction value itself is referred as zero order derivative\n",
                 "# Output is a list of tensors (value, jacobian, hessian, ...)\n",
                 "\n",
                 "values = derivative(n, fn, x, a, b, c, intermediate=True, jacobian=torch.func.jacfwd)\n",
                 "print(*[value.cpu().numpy().tolist() for value in values], sep=', ')\n",
                 "\n",
-                "# Compute jacobian and hessian with torch.func\n",
+                "# Compute jacobian and hessian with torch\n",
                 "\n",
                 "print(fn(x, a, b, c).cpu().numpy().tolist(), \n",
                 "      torch.func.jacfwd(lambda x: fn(x, a, b, c))(x).cpu().numpy().tolist(), \n",
                 "      torch.func.hessian(lambda x: fn(x, a, b, c))(x).cpu().numpy().tolist(), \n",
                 "      sep=', ')\n",
                 "\n",
                 "# Evaluate derivative table representation for a given deviation from the evaluation point\n",
@@ -285,14 +291,15 @@
                 "print(fn(x + dx, a, b, c).cpu().numpy())\n",
                 "\n",
                 "# Evaluate can be mapped over a set of deviation values\n",
                 "\n",
                 "print(torch.func.vmap(lambda x: evaluate(values, [x]))(torch.stack(5*[dx])).cpu().numpy().tolist())\n",
                 "\n",
                 "# Derivative can be mapped over a set of evaluation points\n",
+                "\n",
                 "# Note, the inputt function is expeted to return a tensor\n",
                 "\n",
                 "print(torch.func.vmap(lambda x: derivative(1, fn, x, a, b, c, intermediate=False))(torch.stack(5*[x])).cpu().numpy().tolist())"
             ]
         },
         {
             "cell_type": "code",
@@ -316,14 +323,15 @@
             "source": [
                 "# Derivative\n",
                 "\n",
                 "# Input:  vector\n",
                 "# Output: vector\n",
                 "\n",
                 "# Set test function\n",
+                "\n",
                 "# Note, the first function argument is a vector tensor\n",
                 "# Input function can have other additional arguments\n",
                 "# Other arguments (if any) are not used in computation of derivatives\n",
                 "\n",
                 "def fn(x):\n",
                 "    x1, x2 = x\n",
                 "    X1 = 1.0*x1 + 2.0*x2\n",
@@ -392,20 +400,22 @@
                 "n = 3\n",
                 "\n",
                 "# Set evaluation point\n",
                 "\n",
                 "x = torch.zeros((1, 2, 3), dtype=dtype, device=device)\n",
                 "\n",
                 "# Compute derivatives\n",
+                "\n",
                 "# Note, output is a list of tensors\n",
                 "\n",
                 "values = derivative(n, fn, x)\n",
                 "print(*[list(value.shape) for value in values], sep='\\n')\n",
                 "\n",
                 "# Evaluate derivative table representation for a given deviation from the evaluation point\n",
+                "\n",
                 "# Note, evaluate function works with scalar or vector tensor input\n",
                 "# One should compute derivatives of a wrapped function and reshape the result of evaluate\n",
                 "\n",
                 "# Set wrapped function\n",
                 "\n",
                 "def gn(x, shape):\n",
                 "    return fn(x.reshape(shape)).flatten()\n",
@@ -8866,16 +8876,16 @@
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "# Compute nonlinear invariants\n",
                 "# Note, computation is not optimized and requires a lot of memory\n",
                 "\n",
-                "tx, _ = invariant((4, ), x, [], ix, lambda x: evaluate(t, [x]), jacobian=torch.func.jacfwd, threshold=1.0E-3)\n",
-                "ty, _ = invariant((4, ), x, [], iy, lambda x: evaluate(t, [x]), jacobian=torch.func.jacfwd, threshold=1.0E-3)"
+                "tx, _ = invariant((4, ), x, [], ix, t, jacobian=torch.func.jacfwd, threshold=1.0E-3)\n",
+                "ty, _ = invariant((4, ), x, [], iy, t, jacobian=torch.func.jacfwd, threshold=1.0E-3)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 13,
             "id": "89508b00-d209-4268-9493-4181cf94325a",
             "metadata": {
@@ -9389,15 +9399,15 @@
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "# 1st invariant\n",
                 "\n",
-                "tx, _ = invariant((nx, nw, nk), x, [w, k], ix, t, jacobian=torch.func.jacrev, threshold=0.01, limit=1)\n",
+                "tx, _ = invariant((nx, nw, nk), x, [w, k], ix, t, jacobian=torch.func.jacrev, threshold=0.01)\n",
                 "_"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 15,
             "id": "1aba49aa-9193-4888-8a0c-c83222f00e84",
@@ -9413,17 +9423,17 @@
                     },
                     "execution_count": 15,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "# 2st invariant\n",
+                "# 2nd invariant\n",
                 "\n",
-                "ty, _ = invariant((nx, nw, nk), x, [w, k], iy, t, jacobian=torch.func.jacrev, threshold=0.01, limit=1)\n",
+                "ty, _ = invariant((nx, nw, nk), x, [w, k], iy, t, jacobian=torch.func.jacrev, threshold=0.01)\n",
                 "_"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 16,
             "id": "9744a927-cdbd-477c-ad0a-4f7363285d26",
@@ -9441,16 +9451,16 @@
                 }
             ],
             "source": [
                 "# Test conservation\n",
                 "\n",
                 "# Note, here propagate is used as composition\n",
                 "\n",
-                "print(compare(tx, propagate((4, 1, 3), (nx-1, nw, nk), t, [w, k], tx)))\n",
-                "print(compare(ty, propagate((4, 1, 3), (nx-1, nw, nk), t, [w, k], ty)))"
+                "print(compare(propagate((4, 1, 3), (nx-1, nw, nk), t, [w, k], tx), tx))\n",
+                "print(compare(propagate((4, 1, 3), (nx-1, nw, nk), t, [w, k], ty), ty))"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 17,
             "id": "a5e75ebb-22b4-4f55-9c14-5e21e97d6427",
             "metadata": {
@@ -10192,22 +10202,20 @@
             "id": "b6d8a68a-5c71-4812-a8fe-9952ae2c863f",
             "metadata": {
                 "tags": []
             },
             "outputs": [
                 {
                     "data": {
-                        "image/png": "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\n",
+                        "image/png": "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9mu1WnTt2hVFRUV315SDU/N9vnXrVpw/fx46nQ4AsGTJEqSmpmLNmjWIi4uzSn+OyBaZN0Zj7nUcFZ+AEQDA29sbfn5+Db5cXV1hMplQUVGBnJwcZWxaWhrMZjOCgoLqPXZgYCBcXFywY8cOZVthYSGKiopgMpkAACaTCQcOHLC4GU1NTYVOp4O/vz90Oh0OHDiAvLw85RUdHY2ePXsiLy/vln+3I3P0zOts2LABEyZMwIYNGxAaGmrtGByCq6srAgMDLfIym83YsWOHkteNTCaTRT3wX3519b6+vjAajRY1lZWVyMzMtLgGTb22zYVamQP/PfkaPHiw8lRAo2kZXwrVynzhwoXYv3+/8tldt9T0pk2bMHfuXKv26GjUyjwwMBBarRaFhYVKTU1NDU6cOIEHHnjAav05IrUyv3TpEgDc9Hmi0WiUJ5LNlS0yb4zG3Os4LJUXAaF70LBhw6RPnz6SmZkpv//+u3Tv3t1i2ezi4mLp2bOnZGZmKtuio6OlS5cukpaWJtnZ2WIymcRkMin765ZEDwkJkby8PNm+fbt4e3vXuwx9nZayCqKIepmvW7dOnJ2dZfHixXL69GnlVVFRYZ/G7Wjjxo2i1Wpl9erVcujQIZk0aZLo9Xpllcjx48dLXFycUp+eni7Ozs7y0UcfyeHDhyUhIaHeZYv1er388MMP8ueff8rIkSPrXYa+oWvbnKmReXFxsXTr1k2GDBkixcXFFu/rlkCt9/n1brWiWXOlVuavv/663H///ZKSkiIFBQUSGRkpBoNBysvL7de8StTI/OzZs+Ll5SWjR4+WvLw8KSwslLfeektcXFwkLy/PvgGowBaZnzt3TnJzcyUpKUkAyMaNGyU3N9fi8/p29zqOihMwarJz587JuHHjpE2bNqLT6WTChAlSVVWl7K/74rpz505l2+XLl2Xq1Kni6ekp7u7u8vzzz990w3PixAkZPny4uLm5Sfv27SU2NlZqampueR4taQKmVuaDBg0SADe9Xn31VVu3rIpFixZJly5dxNXVVR5//HHZs2ePsm/QoEE39b1582bp0aOHuLq6ysMPPyxJSUkW+81ms7z33nvi4+MjWq1WhgwZIoWFhRY1t7u2zZ29M1+1alW97+mW9P1INd7n12tpEzARdTKvrq6W2NhYMRgM0rZtWwkODpaDBw/arEdHo0bme/fulZCQEGnXrp20bdtW+vfvL8nJyTbr0dFYO/NbfV4nJCQoNY2513FETiIidn3kRkRERERE1EK1jB98JyIiIiIicgCcgBEREREREdkJJ2BERERERER2wgkYERERERGRnXACRkREREREZCecgBEREREREdkJJ2BERERERER2wgkYERERERGRnXACRkREREREZCecgBEREREREdkJJ2BERERERER28n947CN6rmYMbQAAAABJRU5ErkJggg==",
                         "text/plain": [
-                            "<Figure size 720x720 with 1 Axes>"
+                            "<Figure size 1000x1000 with 1 Axes>"
                         ]
                     },
-                    "metadata": {
-                        "needs_background": "light"
-                    },
+                    "metadata": {},
                     "output_type": "display_data"
                 }
             ],
             "source": [
                 "# Compare phase space trajectories\n",
                 "\n",
                 "plt.figure(figsize=(10, 10))\n",
@@ -10460,133 +10468,34 @@
             "execution_count": 8,
             "id": "e7f286aa-dc5d-48c0-9827-d0aa560362bd",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "[tensor([0., 0., 0., 0.], dtype=torch.float64),\n",
+                            "[[],\n",
                             " tensor([[1.000000000000e+00, 0.000000000000e+00, 0.000000000000e+00, 0.000000000000e+00],\n",
                             "         [0.000000000000e+00, 1.000000000000e+00, 0.000000000000e+00, 0.000000000000e+00],\n",
                             "         [0.000000000000e+00, 0.000000000000e+00, 1.000000000000e+00, 0.000000000000e+00],\n",
                             "         [0.000000000000e+00, 0.000000000000e+00, 0.000000000000e+00, 1.000000000000e+00]],\n",
                             "        dtype=torch.float64),\n",
-                            " tensor([[[0., 0., 0., 0.],\n",
-                            "          [0., 0., 0., 0.],\n",
-                            "          [0., 0., 0., 0.],\n",
-                            "          [0., 0., 0., 0.]],\n",
-                            " \n",
-                            "         [[0., 0., 0., 0.],\n",
-                            "          [0., 0., 0., 0.],\n",
-                            "          [0., 0., 0., 0.],\n",
-                            "          [0., 0., 0., 0.]],\n",
-                            " \n",
-                            "         [[0., 0., 0., 0.],\n",
-                            "          [0., 0., 0., 0.],\n",
-                            "          [0., 0., 0., 0.],\n",
-                            "          [0., 0., 0., 0.]],\n",
-                            " \n",
-                            "         [[0., 0., 0., 0.],\n",
-                            "          [0., 0., 0., 0.],\n",
-                            "          [0., 0., 0., 0.],\n",
-                            "          [0., 0., 0., 0.]]], dtype=torch.float64),\n",
-                            " tensor([[[[0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.]],\n",
-                            " \n",
-                            "          [[0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.]],\n",
-                            " \n",
-                            "          [[0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.]],\n",
-                            " \n",
-                            "          [[0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.]]],\n",
-                            " \n",
-                            " \n",
-                            "         [[[0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.]],\n",
-                            " \n",
-                            "          [[0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.]],\n",
-                            " \n",
-                            "          [[0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.]],\n",
-                            " \n",
-                            "          [[0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.]]],\n",
-                            " \n",
-                            " \n",
-                            "         [[[0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.]],\n",
-                            " \n",
-                            "          [[0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.]],\n",
-                            " \n",
-                            "          [[0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.]],\n",
-                            " \n",
-                            "          [[0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.]]],\n",
-                            " \n",
-                            " \n",
-                            "         [[[0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.]],\n",
-                            " \n",
-                            "          [[0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.]],\n",
-                            " \n",
-                            "          [[0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.]],\n",
-                            " \n",
-                            "          [[0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.]]]], dtype=torch.float64)]"
+                            " [],\n",
+                            " []]"
                         ]
                     },
                     "execution_count": 8,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "# Check\n",
                 "\n",
                 "out = propagate((4, ), (n, ), t_inv, [], t)\n",
-                "chop(out)\n",
+                "chop(out, replace=True)\n",
                 "out"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "fd37bbff-419e-48cd-af75-7026011537df",
             "metadata": {},
@@ -10823,26 +10732,15 @@
             "metadata": {
                 "tags": []
             },
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "[[tensor([0., 0., 0., 0.], dtype=torch.float64),\n",
-                            "  tensor([[0.],\n",
-                            "          [0.],\n",
-                            "          [0.],\n",
-                            "          [0.]], dtype=torch.float64),\n",
-                            "  tensor([[[0.]],\n",
-                            "  \n",
-                            "          [[0.]],\n",
-                            "  \n",
-                            "          [[0.]],\n",
-                            "  \n",
-                            "          [[0.]]], dtype=torch.float64)]]"
+                            "[[[], [], []]]"
                         ]
                     },
                     "execution_count": 9,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -10852,15 +10750,15 @@
                 "# Note, this transformation map zero (parametric) state to zero (upto given order)\n",
                 "# This is true by construction\n",
                 "\n",
                 "def fn_01_02(x, w):\n",
                 "    return map_01_02(x + evaluate(first(pfp), [w]), w) - evaluate(first(pfp), [w])\n",
                 "\n",
                 "out = propagate((4, 1), (0, nw), identity((0, nw), [x, w]), [w], fn_01_02)\n",
-                "chop(out)\n",
+                "chop(out, replace=True)\n",
                 "out"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 10,
             "id": "cb80f040-10d2-4f0a-b2f9-654c71ac62f6",
@@ -10892,417 +10790,75 @@
             "execution_count": 12,
             "id": "15165c76-6665-4098-86b3-9a6d06b198ee",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "[[tensor([0., 0., 0., 0.], dtype=torch.float64),\n",
-                            "  tensor([[0.],\n",
-                            "          [0.],\n",
-                            "          [0.],\n",
-                            "          [0.]], dtype=torch.float64),\n",
-                            "  tensor([[[0.]],\n",
-                            "  \n",
-                            "          [[0.]],\n",
-                            "  \n",
-                            "          [[0.]],\n",
-                            "  \n",
-                            "          [[0.]]], dtype=torch.float64)],\n",
+                            "[[[], [], []],\n",
                             " [tensor([[1.000000000000e+00, 0.000000000000e+00, 0.000000000000e+00, 0.000000000000e+00],\n",
                             "          [0.000000000000e+00, 1.000000000000e+00, 0.000000000000e+00, 0.000000000000e+00],\n",
                             "          [0.000000000000e+00, 0.000000000000e+00, 1.000000000000e+00, 0.000000000000e+00],\n",
                             "          [0.000000000000e+00, 0.000000000000e+00, 0.000000000000e+00, 1.000000000000e+00]],\n",
                             "         dtype=torch.float64),\n",
-                            "  tensor([[[0., 0., 0., 0.]],\n",
-                            "  \n",
-                            "          [[0., 0., 0., 0.]],\n",
-                            "  \n",
-                            "          [[0., 0., 0., 0.]],\n",
-                            "  \n",
-                            "          [[0., 0., 0., 0.]]], dtype=torch.float64),\n",
-                            "  tensor([[[[0., 0., 0., 0.]]],\n",
-                            "  \n",
-                            "  \n",
-                            "          [[[0., 0., 0., 0.]]],\n",
-                            "  \n",
-                            "  \n",
-                            "          [[[0., 0., 0., 0.]]],\n",
-                            "  \n",
-                            "  \n",
-                            "          [[[0., 0., 0., 0.]]]], dtype=torch.float64)],\n",
-                            " [tensor([[[0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.]],\n",
-                            "  \n",
-                            "          [[0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.]],\n",
-                            "  \n",
-                            "          [[0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.]],\n",
-                            "  \n",
-                            "          [[0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.],\n",
-                            "           [0., 0., 0., 0.]]], dtype=torch.float64),\n",
-                            "  tensor([[[[0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.]]],\n",
-                            "  \n",
-                            "  \n",
-                            "          [[[0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.]]],\n",
-                            "  \n",
-                            "  \n",
-                            "          [[[0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.]]],\n",
-                            "  \n",
-                            "  \n",
-                            "          [[[0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.]]]], dtype=torch.float64),\n",
-                            "  tensor([[[[[0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.]]]],\n",
-                            "  \n",
-                            "  \n",
-                            "  \n",
-                            "          [[[[0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.]]]],\n",
-                            "  \n",
-                            "  \n",
-                            "  \n",
-                            "          [[[[0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.]]]],\n",
-                            "  \n",
-                            "  \n",
-                            "  \n",
-                            "          [[[[0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.]]]]], dtype=torch.float64)],\n",
-                            " [tensor([[[[0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.]],\n",
-                            "  \n",
-                            "           [[0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.]],\n",
-                            "  \n",
-                            "           [[0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.]],\n",
-                            "  \n",
-                            "           [[0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.]]],\n",
-                            "  \n",
-                            "  \n",
-                            "          [[[0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.]],\n",
-                            "  \n",
-                            "           [[0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.]],\n",
-                            "  \n",
-                            "           [[0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.]],\n",
-                            "  \n",
-                            "           [[0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.]]],\n",
-                            "  \n",
-                            "  \n",
-                            "          [[[0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.]],\n",
-                            "  \n",
-                            "           [[0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.]],\n",
-                            "  \n",
-                            "           [[0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.]],\n",
-                            "  \n",
-                            "           [[0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.]]],\n",
-                            "  \n",
-                            "  \n",
-                            "          [[[0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.]],\n",
-                            "  \n",
-                            "           [[0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.]],\n",
-                            "  \n",
-                            "           [[0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.]],\n",
-                            "  \n",
-                            "           [[0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.],\n",
-                            "            [0., 0., 0., 0.]]]], dtype=torch.float64),\n",
-                            "  tensor([[[[[0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.]],\n",
-                            "  \n",
-                            "            [[0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.]],\n",
-                            "  \n",
-                            "            [[0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.]],\n",
-                            "  \n",
-                            "            [[0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.]]]],\n",
-                            "  \n",
-                            "  \n",
-                            "  \n",
-                            "          [[[[0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.]],\n",
-                            "  \n",
-                            "            [[0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.]],\n",
-                            "  \n",
-                            "            [[0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.]],\n",
-                            "  \n",
-                            "            [[0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.]]]],\n",
-                            "  \n",
-                            "  \n",
-                            "  \n",
-                            "          [[[[0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.]],\n",
-                            "  \n",
-                            "            [[0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.]],\n",
-                            "  \n",
-                            "            [[0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.]],\n",
-                            "  \n",
-                            "            [[0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.]]]],\n",
-                            "  \n",
-                            "  \n",
-                            "  \n",
-                            "          [[[[0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.]],\n",
-                            "  \n",
-                            "            [[0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.]],\n",
-                            "  \n",
-                            "            [[0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.]],\n",
-                            "  \n",
-                            "            [[0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.],\n",
-                            "             [0., 0., 0., 0.]]]]], dtype=torch.float64),\n",
-                            "  tensor([[[[[[0., 0., 0., 0.],\n",
-                            "              [0., 0., 0., 0.],\n",
-                            "              [0., 0., 0., 0.],\n",
-                            "              [0., 0., 0., 0.]],\n",
-                            "  \n",
-                            "             [[0., 0., 0., 0.],\n",
-                            "              [0., 0., 0., 0.],\n",
-                            "              [0., 0., 0., 0.],\n",
-                            "              [0., 0., 0., 0.]],\n",
-                            "  \n",
-                            "             [[0., 0., 0., 0.],\n",
-                            "              [0., 0., 0., 0.],\n",
-                            "              [0., 0., 0., 0.],\n",
-                            "              [0., 0., 0., 0.]],\n",
-                            "  \n",
-                            "             [[0., 0., 0., 0.],\n",
-                            "              [0., 0., 0., 0.],\n",
-                            "              [0., 0., 0., 0.],\n",
-                            "              [0., 0., 0., 0.]]]]],\n",
-                            "  \n",
-                            "  \n",
-                            "  \n",
-                            "  \n",
-                            "          [[[[[0., 0., 0., 0.],\n",
-                            "              [0., 0., 0., 0.],\n",
-                            "              [0., 0., 0., 0.],\n",
-                            "              [0., 0., 0., 0.]],\n",
-                            "  \n",
-                            "             [[0., 0., 0., 0.],\n",
-                            "              [0., 0., 0., 0.],\n",
-                            "              [0., 0., 0., 0.],\n",
-                            "              [0., 0., 0., 0.]],\n",
-                            "  \n",
-                            "             [[0., 0., 0., 0.],\n",
-                            "              [0., 0., 0., 0.],\n",
-                            "              [0., 0., 0., 0.],\n",
-                            "              [0., 0., 0., 0.]],\n",
-                            "  \n",
-                            "             [[0., 0., 0., 0.],\n",
-                            "              [0., 0., 0., 0.],\n",
-                            "              [0., 0., 0., 0.],\n",
-                            "              [0., 0., 0., 0.]]]]],\n",
-                            "  \n",
-                            "  \n",
-                            "  \n",
-                            "  \n",
-                            "          [[[[[0., 0., 0., 0.],\n",
-                            "              [0., 0., 0., 0.],\n",
-                            "              [0., 0., 0., 0.],\n",
-                            "              [0., 0., 0., 0.]],\n",
-                            "  \n",
-                            "             [[0., 0., 0., 0.],\n",
-                            "              [0., 0., 0., 0.],\n",
-                            "              [0., 0., 0., 0.],\n",
-                            "              [0., 0., 0., 0.]],\n",
-                            "  \n",
-                            "             [[0., 0., 0., 0.],\n",
-                            "              [0., 0., 0., 0.],\n",
-                            "              [0., 0., 0., 0.],\n",
-                            "              [0., 0., 0., 0.]],\n",
-                            "  \n",
-                            "             [[0., 0., 0., 0.],\n",
-                            "              [0., 0., 0., 0.],\n",
-                            "              [0., 0., 0., 0.],\n",
-                            "              [0., 0., 0., 0.]]]]],\n",
-                            "  \n",
-                            "  \n",
-                            "  \n",
-                            "  \n",
-                            "          [[[[[0., 0., 0., 0.],\n",
-                            "              [0., 0., 0., 0.],\n",
-                            "              [0., 0., 0., 0.],\n",
-                            "              [0., 0., 0., 0.]],\n",
-                            "  \n",
-                            "             [[0., 0., 0., 0.],\n",
-                            "              [0., 0., 0., 0.],\n",
-                            "              [0., 0., 0., 0.],\n",
-                            "              [0., 0., 0., 0.]],\n",
-                            "  \n",
-                            "             [[0., 0., 0., 0.],\n",
-                            "              [0., 0., 0., 0.],\n",
-                            "              [0., 0., 0., 0.],\n",
-                            "              [0., 0., 0., 0.]],\n",
-                            "  \n",
-                            "             [[0., 0., 0., 0.],\n",
-                            "              [0., 0., 0., 0.],\n",
-                            "              [0., 0., 0., 0.],\n",
-                            "              [0., 0., 0., 0.]]]]]], dtype=torch.float64)]]"
+                            "  [],\n",
+                            "  []],\n",
+                            " [[], [], []],\n",
+                            " [[], [], []]]"
                         ]
                     },
                     "execution_count": 12,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "# Check\n",
                 "\n",
                 "out = propagate((4, 1), (nx, nw), t_inv, [w], t)\n",
-                "chop(out)\n",
+                "chop(out, replace=True)\n",
                 "out"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "1a64f7bd-e716-4653-95f6-ddc3ed0108d3",
             "metadata": {},
             "source": [
-                "# Example-29: Momenta"
+                "# Example-29: Momenta generator"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 1,
             "id": "fd671059-7f65-4e37-a093-63e5b90b6c35",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
-                "# In this example initial and final monemta are computed from given initial and final coordinates"
+                "# In this example initial and final monemta are computed from given initial and final coordinates\n",
+                "# Given an origing preserving mapping, its table representation can be computed upto some order\n",
+                "# This representation can be considered as exact\n",
+                "# Next, given initial and final coordinates, corresponding momenta can be computed using momenta generator"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 18,
+            "execution_count": 2,
             "id": "a8cfbb8f-8e87-4e6e-9e5d-b30fe8d87318",
             "metadata": {
                 "tags": []
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "False\n"
+                        "True\n"
                     ]
                 }
             ],
             "source": [
                 "# Import\n",
                 "\n",
                 "import numpy\n",
@@ -11324,30 +10880,30 @@
                 "\n",
                 "import warnings\n",
                 "warnings.filterwarnings(\"ignore\")"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 19,
+            "execution_count": 3,
             "id": "701fc087-f666-43e0-a90a-8b0580102a7f",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "# Set data type and device\n",
                 "\n",
                 "dtype = torch.float64\n",
                 "device = torch.device('cpu')"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 20,
+            "execution_count": 4,
             "id": "3094551a-2a92-464e-9121-d37f190864a4",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "# Set elements\n",
@@ -11572,25 +11128,25 @@
             "execution_count": 12,
             "id": "287c366c-dbe7-4675-8f79-209e7c9e1f78",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
-                "# Compute monemta generator\n",
+                "# Compute momenta generator\n",
                 "\n",
                 "# Note, computation order can be different from that of the input table\n",
                 "# Accuracy is strongly related to computation order and magnitude of initial coordinates\n",
                 "\n",
                 "m = momenta((nx, nw), x, [w], t)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 27,
+            "execution_count": 13,
             "id": "fa9a6e65-5a23-4d45-a76b-756da0491388",
             "metadata": {
                 "tags": []
             },
             "outputs": [
                 {
                     "name": "stdout",
@@ -11613,16 +11169,16 @@
                 }
             ],
             "source": [
                 "# Recover momenta from coordinates\n",
                 "\n",
                 "# Set deviations\n",
                 "\n",
-                "xi = torch.tensor([0.0005, 0.0001, -0.0005, -0.0001], dtype=dtype)\n",
-                "dw = torch.tensor(1*[0.0001], dtype=torch.float64)\n",
+                "xi = torch.tensor([0.0005, 0.0001, -0.0005, -0.0001], dtype=dtype, device=device)\n",
+                "dw = torch.tensor(1*[0.0001], dtype=dtype, device=device)\n",
                 "\n",
                 "# Evaluate final state using table representation\n",
                 "\n",
                 "xf = evaluate(t, [xi, dw])\n",
                 "\n",
                 "print(xf)\n",
                 "print()\n",
@@ -11646,14 +11202,987 @@
                 "print()\n",
                 "\n",
                 "# Evaluate generator using coordinates\n",
                 "\n",
                 "print(evaluate(m, [qs, 0*dw]))\n",
                 "print(evaluate(m, [qs, 1*dw]))"
             ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "9dcdb26f-f41a-428b-b3f1-0de458403dc3",
+            "metadata": {},
+            "source": [
+                "# Example-30: Factorization (kick)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 1,
+            "id": "5c9c3ebf-1980-4108-b5b0-58ffe61cb8fe",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "# Given a derivative table representation (taylor series) of an origin preserving mapping\n",
+                "# It is possible to factorize it into composition of linear and nonlinear table representations\n",
+                "# If original mapping represents a single turn, linear part can be brought to its normal form\n",
+                "# This can be done using linear theory\n",
+                "# The nonlinear part is a near identity transformation, it can be represented with Lie transformation\n",
+                "# t = tl o tn and tn = exp(-[h])\n",
+                "# In this example (generator) h is computed for a single kick\n",
+                "# It can be used to construct nonlinear normal forms or as a redundancy free representation"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 2,
+            "id": "186b19c2-a6a4-4eb7-b239-e9e0695cd7e4",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "True\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Import\n",
+                "\n",
+                "import torch\n",
+                "\n",
+                "from ndtorch.derivative import derivative\n",
+                "from ndtorch.signature import chop\n",
+                "from ndtorch.evaluate import evaluate\n",
+                "from ndtorch.propagate import identity\n",
+                "from ndtorch.propagate import propagate\n",
+                "from ndtorch.series import series\n",
+                "from ndtorch.series import clean\n",
+                "from ndtorch.taylor import taylor\n",
+                "from ndtorch.inverse import inverse\n",
+                "from ndtorch.factorization import hamiltonian\n",
+                "\n",
+                "torch.set_printoptions(precision=12, sci_mode=True)\n",
+                "print(torch.cuda.is_available())\n",
+                "\n",
+                "import warnings\n",
+                "warnings.filterwarnings(\"ignore\")"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 3,
+            "id": "56cd3c16-afee-4687-b711-9a248e9c9f0d",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "# Set data type and device\n",
+                "\n",
+                "dtype = torch.float64\n",
+                "device = torch.device('cpu')"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 4,
+            "id": "46182ddc-f0a7-47f0-873a-57c2eb80da81",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "tensor([0., 0., 0., 0.], dtype=torch.float64)\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Set transformation\n",
+                "\n",
+                "# Note, this transformation can be exactly represented with a taylor series (i.e. polynomial)\n",
+                "\n",
+                "def mapping(x, k, l):\n",
+                "    (qx, px, qy, py), (k, ), l = x, k, l/2\n",
+                "    qx, qy = qx + l*px, qy + l*py\n",
+                "    px, py = px - 1.0*l*k*(qx**2 - qy**2), py + 2.0*l*k*qx*qy\n",
+                "    qx, qy = qx + l*px, qy + l*py\n",
+                "    return torch.stack([qx, px, qy, py])\n",
+                "\n",
+                "# Test origin propagation\n",
+                "\n",
+                "x = torch.tensor(4*[0.0], dtype=dtype, device=device)\n",
+                "k = torch.tensor(1*[0.0], dtype=dtype, device=device)\n",
+                "\n",
+                "print(mapping(x, k, 0.1))"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 5,
+            "id": "281e3c38-c941-4622-8a3b-5f0619409511",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "# Compute table representation\n",
+                "\n",
+                "t = identity((2, 1), [x, k])\n",
+                "t = propagate((4, 1), (2, 1), t, [k], mapping, 0.1)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 6,
+            "id": "63a04154-d5da-4968-aa34-e6bcbbcf0576",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "tensor([1.009811250000e-01, 9.622500000000e-03, 5.102537625000e-02, 1.050752500000e-02],\n",
+                        "       dtype=torch.float64)\n",
+                        "tensor([1.009811250000e-01, 9.622500000000e-03, 5.102537625000e-02, 1.050752500000e-02],\n",
+                        "       dtype=torch.float64)\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Compare for some deviation\n",
+                "\n",
+                "dx = torch.tensor([0.1, 0.01, 0.05, 0.01], dtype=dtype, device=device)\n",
+                "dk = torch.tensor([1.0],dtype=dtype, device=device)\n",
+                "\n",
+                "print(mapping(x + dx, k + dk, 0.1))\n",
+                "print(evaluate(t, [dx, dk]))"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 7,
+            "id": "52aff165-c437-4e34-9d62-78dd396522d5",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "tensor([[1.000000000000e+00, 1.000000000000e-01, 0.000000000000e+00, 0.000000000000e+00],\n",
+                        "        [0.000000000000e+00, 1.000000000000e+00, 0.000000000000e+00, 0.000000000000e+00],\n",
+                        "        [0.000000000000e+00, 0.000000000000e+00, 1.000000000000e+00, 1.000000000000e-01],\n",
+                        "        [0.000000000000e+00, 0.000000000000e+00, 0.000000000000e+00, 1.000000000000e+00]],\n",
+                        "       dtype=torch.float64)\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Linear part is not near identity\n",
+                "\n",
+                "print(derivative(1, lambda x, k: evaluate(t, [x, k]), x, k, intermediate=False))"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 8,
+            "id": "1b25e630-6870-4be2-86d3-8d8dce231b3b",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "# Set linear part and compose with its inverse\n",
+                "\n",
+                "l = derivative(1, lambda x, k: evaluate(t, [x, k]), x, k)\n",
+                "t = propagate((4, 1), (2, 1), inverse(1, x, [k], l), [k], t)\n",
+                "chop(t)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 9,
+            "id": "c631a032-59f2-40b7-ace1-00b9e1243b25",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "tensor([[1.000000000000e+00, 0.000000000000e+00, 0.000000000000e+00, 0.000000000000e+00],\n",
+                        "        [0.000000000000e+00, 1.000000000000e+00, 0.000000000000e+00, 0.000000000000e+00],\n",
+                        "        [0.000000000000e+00, 0.000000000000e+00, 1.000000000000e+00, 0.000000000000e+00],\n",
+                        "        [0.000000000000e+00, 0.000000000000e+00, 0.000000000000e+00, 1.000000000000e+00]],\n",
+                        "       dtype=torch.float64)\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Now table represents a near identity transformation\n",
+                "\n",
+                "print(derivative(1, lambda x, k: evaluate(t, [x, k]), x, k, intermediate=False))"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 10,
+            "id": "6852653d-0193-4d28-8454-05530ab38812",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "(3, 0, 0, 0, 1) tensor(1.666666666667e-02, dtype=torch.float64)\n",
+                        "(2, 1, 0, 0, 1) tensor(-2.500000000000e-03, dtype=torch.float64)\n",
+                        "(1, 2, 0, 0, 1) tensor(1.250000000000e-04, dtype=torch.float64)\n",
+                        "(1, 0, 2, 0, 1) tensor(-5.000000000000e-02, dtype=torch.float64)\n",
+                        "(1, 0, 1, 1, 1) tensor(5.000000000000e-03, dtype=torch.float64)\n",
+                        "(1, 0, 0, 2, 1) tensor(-1.250000000000e-04, dtype=torch.float64)\n",
+                        "(0, 3, 0, 0, 1) tensor(-2.083333333333e-06, dtype=torch.float64)\n",
+                        "(0, 1, 2, 0, 1) tensor(2.500000000000e-03, dtype=torch.float64)\n",
+                        "(0, 1, 1, 1, 1) tensor(-2.500000000000e-04, dtype=torch.float64)\n",
+                        "(0, 1, 0, 2, 1) tensor(6.250000000000e-06, dtype=torch.float64)\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Compute single exponent generator\n",
+                "\n",
+                "h = hamiltonian((2, 1), x, [k], t)\n",
+                "chop(h)\n",
+                "\n",
+                "# Compute series representation\n",
+                "\n",
+                "# Note, each coefficient is proportional to strength\n",
+                "\n",
+                "s = clean(series((4, 1), (3, 1), h))\n",
+                "for index, value in s.items():\n",
+                "    print(index, value.squeeze())"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 11,
+            "id": "0bd97ea3-8875-4b60-904a-59e29890b8ce",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "tensor([1.009811250000e-01, 9.622500000000e-03, 5.102537625000e-02, 1.050752500000e-02],\n",
+                        "       dtype=torch.float64)\n",
+                        "tensor([1.009811250000e-01, 9.622500000000e-03, 5.102537625000e-02, 1.050752500000e-02],\n",
+                        "       dtype=torch.float64)\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# In this example, this hamiltonian generates exact solution with taylor intergator\n",
+                "\n",
+                "print(mapping(x + dx, k + dk, 0.1))\n",
+                "print(taylor(1, 1.0, lambda x, k: evaluate(h, [x, k]), evaluate(l, [dx, dk]), dk))"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "4168324a-1472-4574-9087-e60922704759",
+            "metadata": {},
+            "source": [
+                "# Example-31: Factorization (fodo)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 1,
+            "id": "d50ae1b9-9c66-4f96-b57c-3b6d9be7dae6",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "True\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Import\n",
+                "\n",
+                "import torch\n",
+                "\n",
+                "from ndtorch.derivative import derivative\n",
+                "from ndtorch.signature import chop\n",
+                "from ndtorch.evaluate import evaluate\n",
+                "from ndtorch.evaluate import compare\n",
+                "from ndtorch.propagate import identity\n",
+                "from ndtorch.propagate import propagate\n",
+                "from ndtorch.series import series\n",
+                "from ndtorch.series import clean\n",
+                "from ndtorch.taylor import taylor\n",
+                "from ndtorch.inverse import inverse\n",
+                "from ndtorch.factorization import hamiltonian\n",
+                "from ndtorch.factorization import solution\n",
+                "\n",
+                "torch.set_printoptions(precision=12, sci_mode=True)\n",
+                "print(torch.cuda.is_available())\n",
+                "\n",
+                "import warnings\n",
+                "warnings.filterwarnings(\"ignore\")"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 2,
+            "id": "d1824145-7e9f-45c8-8473-294bb7db7cf5",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [],
+            "source": [
+                "# Set data type and device\n",
+                "\n",
+                "dtype = torch.float64\n",
+                "device = torch.device('cpu')"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 3,
+            "id": "48d3e9e8-cde9-43f6-a74d-6caa49e5d233",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [],
+            "source": [
+                "# Set elements\n",
+                "\n",
+                "def drif(x, w, l):\n",
+                "    (qx, px, qy, py), (w, ), l = x, w, l\n",
+                "    return torch.stack([qx + l*px/(1 + w), px, qy + l*py/(1 + w), py])\n",
+                "\n",
+                "def quad(x, w, kq, l, n=5):\n",
+                "    (qx, px, qy, py), (w, ), kq, l = x, w, kq, l/(2.0*n)\n",
+                "    for _ in range(n):\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "        px, py = px - 2.0*l*kq*qx, py + 2.0*l*kq*qy\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "    return torch.stack([qx, px, qy, py])\n",
+                "\n",
+                "def sext(x, w, ks, l, n=1):\n",
+                "    (qx, px, qy, py), (w, ), ks, l = x, w, ks, l/(2.0*n)\n",
+                "    for _ in range(n):\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "        px, py = px - 1.0*l*ks*(qx**2 - qy**2), py + 2.0*l*ks*qx*qy\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "    return torch.stack([qx, px, qy, py])\n",
+                "\n",
+                "def bend(x, w, r, kq, ks, l, n=10):\n",
+                "    (qx, px, qy, py), (w, ), r, kq, ks, l = x, w, r, kq, ks, l/(2.0*n)\n",
+                "    for _ in range(n):\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "        px, py = px - 2.0*l*kq*qx - 1.0*l*ks*(qx**2 - qy**2) + 2.0*l/r**2*(w*r - qx), py + 2.0*l*kq*qy + 2.0*l*ks*qx*qy\n",
+                "        qx, qy = qx + l*px/(1 + w), qy + l*py/(1 + w)\n",
+                "    return torch.stack([qx, px, qy, py]) \n",
+                "\n",
+                "def kick(x, cx, cy):\n",
+                "    (qx, px, qy, py) = x\n",
+                "    return torch.stack([qx, px + cx, qy, py + cy])    \n",
+                "\n",
+                "def slip(x, dx, dy):\n",
+                "    (qx, px, qy, py) = x\n",
+                "    return torch.stack([qx + dx, px, qy + dy, py])"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 4,
+            "id": "a877a9b8-31a2-4329-8053-386b10f72dde",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [],
+            "source": [
+                "# Set fodo\n",
+                "\n",
+                "def fodo(x):\n",
+                "    x = quad(x, [0.0], 0.19, 0.50)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = sext(x, [0.0], 0.1, +0.5)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = bend(x, [0.0], 22.92, 0.015, 0.25, 3.0)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = sext(x, [0.0], 0.1, -0.5)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = quad(x, [0.0], -0.21, 0.50)\n",
+                "    x = quad(x, [0.0], -0.21, 0.50)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = sext(x, [0.0], 0.1, -0.5)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = bend(x, [0.0], 22.92, 0.015, 0.25, 3.0)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = sext(x, [0.0], 0.1, +0.5)\n",
+                "    x = drif(x, [0.0], 0.45)\n",
+                "    x = quad(x, [0.0], 0.19, 0.50)\n",
+                "    return x"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 5,
+            "id": "62358986-4d24-49f8-9e60-5facf10c0104",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "tensor([0., 0., 0., 0.], dtype=torch.float64)"
+                        ]
+                    },
+                    "execution_count": 5,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "# Set computation order & evaluation point\n",
+                "\n",
+                "n = 4\n",
+                "x = torch.tensor([0.0, 0.0, 0.0, 0.0], dtype=dtype, device=device)\n",
+                "\n",
+                "# Note, origin is preserved\n",
+                "\n",
+                "fodo(x)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 6,
+            "id": "b43b5788-9b64-414a-99ca-296fc0a1b0b9",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [],
+            "source": [
+                "# Compute derivative table\n",
+                "\n",
+                "t = identity((n, ), [x])\n",
+                "t = propagate((4, ), (n, ), t, [], lambda x: fodo(x))"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 7,
+            "id": "7d23b3ce-06ab-482a-939e-1a798c735974",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "[tensor([0., 0., 0., 0.], dtype=torch.float64),\n",
+                            " tensor([[8.259928915375e-02, 1.470387298165e+01, 0.000000000000e+00, 0.000000000000e+00],\n",
+                            "         [-6.754528950779e-02, 8.259928915375e-02, 0.000000000000e+00, 0.000000000000e+00],\n",
+                            "         [0.000000000000e+00, 0.000000000000e+00, 8.239443265215e-01, 6.857644998910e+00],\n",
+                            "         [0.000000000000e+00, 0.000000000000e+00, -4.682595072274e-02, 8.239443265215e-01]],\n",
+                            "        dtype=torch.float64)]"
+                        ]
+                    },
+                    "execution_count": 7,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "# Set linear part\n",
+                "\n",
+                "l = derivative(1, lambda x: evaluate(t, [x]), x)\n",
+                "l"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 8,
+            "id": "ac3be7e9-12ad-4bf8-986c-3dc318dd5b96",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "[tensor([0., 0., 0., 0.], dtype=torch.float64),\n",
+                            " tensor([[1.000000000000e+00, 0.000000000000e+00, 0.000000000000e+00, 0.000000000000e+00],\n",
+                            "         [0.000000000000e+00, 1.000000000000e+00, 0.000000000000e+00, 0.000000000000e+00],\n",
+                            "         [0.000000000000e+00, 0.000000000000e+00, 1.000000000000e+00, 0.000000000000e+00],\n",
+                            "         [0.000000000000e+00, 0.000000000000e+00, 0.000000000000e+00, 1.000000000000e+00]],\n",
+                            "        dtype=torch.float64)]"
+                        ]
+                    },
+                    "execution_count": 8,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "# Set nonlinear part\n",
+                "\n",
+                "u = propagate((4, ), (n, ), inverse(1, x, [], l), [], t)\n",
+                "chop(u)\n",
+                "derivative(1, lambda x: evaluate(u, [x]), x)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 9,
+            "id": "e614b69d-6596-4ea3-9a69-1eafc23c4994",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [],
+            "source": [
+                "# Compute hamiltonian\n",
+                "\n",
+                "h = hamiltonian((n, ), x, [], u)\n",
+                "chop(h)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 10,
+            "id": "d2a22f41-7484-4fb9-a743-dff32cf7c6d5",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "(3, 0, 0, 0) tensor(5.024988945080e-02, dtype=torch.float64)\n",
+                        "(2, 1, 0, 0) tensor(-8.027849817894e-01, dtype=torch.float64)\n",
+                        "(1, 2, 0, 0) tensor(1.242554019904e+01, dtype=torch.float64)\n",
+                        "(1, 0, 2, 0) tensor(-5.976214487541e-01, dtype=torch.float64)\n",
+                        "(1, 0, 1, 1) tensor(3.719621673904e+00, dtype=torch.float64)\n",
+                        "(1, 0, 0, 2) tensor(-6.659517059512e+00, dtype=torch.float64)\n",
+                        "(0, 3, 0, 0) tensor(-1.465736828313e+02, dtype=torch.float64)\n",
+                        "(0, 1, 2, 0) tensor(7.616595688746e+00, dtype=torch.float64)\n",
+                        "(0, 1, 1, 1) tensor(-6.812652464723e+01, dtype=torch.float64)\n",
+                        "(0, 1, 0, 2) tensor(1.637189795764e+02, dtype=torch.float64)\n",
+                        "(4, 0, 0, 0) tensor(-2.670453079972e-02, dtype=torch.float64)\n",
+                        "(3, 1, 0, 0) tensor(1.592046859279e+00, dtype=torch.float64)\n",
+                        "(2, 2, 0, 0) tensor(-4.015290100155e+01, dtype=torch.float64)\n",
+                        "(2, 0, 2, 0) tensor(1.098921583040e-02, dtype=torch.float64)\n",
+                        "(2, 0, 1, 1) tensor(-1.150214563563e+00, dtype=torch.float64)\n",
+                        "(2, 0, 0, 2) tensor(5.596016324538e+00, dtype=torch.float64)\n",
+                        "(1, 3, 0, 0) tensor(2.720415502394e+02, dtype=torch.float64)\n",
+                        "(1, 1, 2, 0) tensor(9.092563694884e+00, dtype=torch.float64)\n",
+                        "(1, 1, 1, 1) tensor(-7.311435065924e+01, dtype=torch.float64)\n",
+                        "(1, 1, 0, 2) tensor(1.043406910282e+02, dtype=torch.float64)\n",
+                        "(0, 4, 0, 0) tensor(-8.872464473277e+02, dtype=torch.float64)\n",
+                        "(0, 2, 2, 0) tensor(2.515413272498e+01, dtype=torch.float64)\n",
+                        "(0, 2, 1, 1) tensor(6.993401944277e+01, dtype=torch.float64)\n",
+                        "(0, 2, 0, 2) tensor(-3.593047920669e+02, dtype=torch.float64)\n",
+                        "(0, 0, 4, 0) tensor(-1.258999636146e+00, dtype=torch.float64)\n",
+                        "(0, 0, 3, 1) tensor(1.898846058062e+01, dtype=torch.float64)\n",
+                        "(0, 0, 2, 2) tensor(-1.062500223737e+02, dtype=torch.float64)\n",
+                        "(0, 0, 1, 3) tensor(2.608144282259e+02, dtype=torch.float64)\n",
+                        "(0, 0, 0, 4) tensor(-2.419706859670e+02, dtype=torch.float64)\n",
+                        "(5, 0, 0, 0) tensor(3.720153703396e-02, dtype=torch.float64)\n",
+                        "(4, 1, 0, 0) tensor(-2.470046738149e+00, dtype=torch.float64)\n",
+                        "(3, 2, 0, 0) tensor(5.465213020046e+01, dtype=torch.float64)\n",
+                        "(3, 0, 2, 0) tensor(6.994399435987e-02, dtype=torch.float64)\n",
+                        "(3, 0, 1, 1) tensor(-9.734770779462e-01, dtype=torch.float64)\n",
+                        "(3, 0, 0, 2) tensor(5.509140066922e-01, dtype=torch.float64)\n",
+                        "(2, 3, 0, 0) tensor(-7.728896235979e+02, dtype=torch.float64)\n",
+                        "(2, 1, 2, 0) tensor(1.614402519455e+01, dtype=torch.float64)\n",
+                        "(2, 1, 1, 1) tensor(-1.014114400601e+02, dtype=torch.float64)\n",
+                        "(2, 1, 0, 2) tensor(2.099498728183e+02, dtype=torch.float64)\n",
+                        "(1, 4, 0, 0) tensor(6.599464974629e+03, dtype=torch.float64)\n",
+                        "(1, 2, 2, 0) tensor(-1.831472433171e+02, dtype=torch.float64)\n",
+                        "(1, 2, 1, 1) tensor(1.658609587412e+03, dtype=torch.float64)\n",
+                        "(1, 2, 0, 2) tensor(-4.455648121228e+03, dtype=torch.float64)\n",
+                        "(1, 0, 4, 0) tensor(-2.372154036991e+00, dtype=torch.float64)\n",
+                        "(1, 0, 3, 1) tensor(3.120364861986e+01, dtype=torch.float64)\n",
+                        "(1, 0, 2, 2) tensor(-1.392873544053e+02, dtype=torch.float64)\n",
+                        "(1, 0, 1, 3) tensor(2.280297561995e+02, dtype=torch.float64)\n",
+                        "(1, 0, 0, 4) tensor(-5.830536198793e+01, dtype=torch.float64)\n",
+                        "(0, 5, 0, 0) tensor(-1.712807218852e+04, dtype=torch.float64)\n",
+                        "(0, 3, 2, 0) tensor(-5.278629070820e+02, dtype=torch.float64)\n",
+                        "(0, 3, 1, 1) tensor(3.474912442117e+03, dtype=torch.float64)\n",
+                        "(0, 3, 0, 2) tensor(1.999757814650e+02, dtype=torch.float64)\n",
+                        "(0, 1, 4, 0) tensor(2.874466602579e+01, dtype=torch.float64)\n",
+                        "(0, 1, 3, 1) tensor(-5.199961828427e+02, dtype=torch.float64)\n",
+                        "(0, 1, 2, 2) tensor(3.267795295152e+03, dtype=torch.float64)\n",
+                        "(0, 1, 1, 3) tensor(-8.677457594504e+03, dtype=torch.float64)\n",
+                        "(0, 1, 0, 4) tensor(8.128231575922e+03, dtype=torch.float64)\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Compute series representation\n",
+                "\n",
+                "s = clean(series((4, ), (n + 1, ), h), epsilon=1.0E-9)\n",
+                "for index, value in s.items():\n",
+                "    print(index, value.squeeze())"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 11,
+            "id": "f5bfe2b0-5796-45f5-8785-f30ed8a32cd6",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "True\n",
+                        "True\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Restore mapping table nonlinear part from hamiltonian\n",
+                "\n",
+                "print(compare(u, solution((n, ), x, [], h)))\n",
+                "print(compare(t, propagate((4, ), (n, ), l, [], solution((n, ), x, [], h))))"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "b6d8236a-9e84-47e0-ab5f-003cc8fd7f92",
+            "metadata": {},
+            "source": [
+                "# Example-32: Factorization (factorize)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 1,
+            "id": "ba8720f6-ac3f-447d-b74a-5f2a7cc5ed65",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "True\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Import\n",
+                "\n",
+                "import torch\n",
+                "from ndtorch.derivative import derivative\n",
+                "from ndtorch.signature import chop\n",
+                "from ndtorch.evaluate import evaluate\n",
+                "from ndtorch.evaluate import compare\n",
+                "from ndtorch.series import series\n",
+                "from ndtorch.series import clean\n",
+                "from ndtorch.series import split\n",
+                "from ndtorch.propagate import identity\n",
+                "from ndtorch.propagate import propagate\n",
+                "from ndtorch.bracket import bracket\n",
+                "from ndtorch.factorization import hamiltonian\n",
+                "from ndtorch.factorization import solution\n",
+                "from ndtorch.factorization import factorize\n",
+                "\n",
+                "torch.set_printoptions(precision=12, sci_mode=True)\n",
+                "print(torch.cuda.is_available())\n",
+                "\n",
+                "import warnings\n",
+                "warnings.filterwarnings(\"ignore\")"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 2,
+            "id": "f459d7a8-0c87-45a8-be50-3c6e0eaf4815",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [],
+            "source": [
+                "# Set data type and device\n",
+                "\n",
+                "dtype = torch.float64\n",
+                "device = torch.device('cpu')"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 3,
+            "id": "017b340b-4d9c-42ba-ad8b-c6a410514e10",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "{(3, 0, 0, 0): tensor(1.000000000000e+00, dtype=torch.float64),\n",
+                            " (2, 1, 0, 0): tensor(1.000000000000e+00, dtype=torch.float64),\n",
+                            " (1, 2, 0, 0): tensor(1.000000000000e+00, dtype=torch.float64),\n",
+                            " (0, 3, 0, 0): tensor(1.000000000000e+00, dtype=torch.float64),\n",
+                            " (3, 0, 1, 0): tensor(1.000000000000e+00, dtype=torch.float64),\n",
+                            " (3, 0, 2, 0): tensor(1.000000000000e+00, dtype=torch.float64),\n",
+                            " (4, 0, 0, 0): tensor(1.000000000000e+00, dtype=torch.float64),\n",
+                            " (3, 1, 0, 0): tensor(1.000000000000e+00, dtype=torch.float64),\n",
+                            " (2, 2, 0, 0): tensor(1.000000000000e+00, dtype=torch.float64),\n",
+                            " (1, 3, 0, 0): tensor(1.000000000000e+00, dtype=torch.float64),\n",
+                            " (0, 4, 0, 0): tensor(1.000000000000e+00, dtype=torch.float64),\n",
+                            " (4, 0, 0, 1): tensor(1.000000000000e+00, dtype=torch.float64),\n",
+                            " (5, 0, 0, 0): tensor(1.000000000000e+00, dtype=torch.float64),\n",
+                            " (4, 1, 0, 0): tensor(1.000000000000e+00, dtype=torch.float64),\n",
+                            " (3, 2, 0, 0): tensor(1.000000000000e+00, dtype=torch.float64),\n",
+                            " (2, 3, 0, 0): tensor(1.000000000000e+00, dtype=torch.float64),\n",
+                            " (1, 4, 0, 0): tensor(1.000000000000e+00, dtype=torch.float64),\n",
+                            " (0, 5, 0, 0): tensor(1.000000000000e+00, dtype=torch.float64)}"
+                        ]
+                    },
+                    "execution_count": 3,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "# Set test hamiltonian function and compute corresponding table representation\n",
+                "\n",
+                "# Note, test hamiltonian is near identity\n",
+                "\n",
+                "def h(x, u, v):\n",
+                "    q, p = x\n",
+                "    u, = u\n",
+                "    v, = v\n",
+                "    h1 = (1 + u + u**2)*q**3 + q**2*p + q*p**2 + p**3\n",
+                "    h2 = (1 + v)*q**4 + q**3*p + q**2*p**2 + q*p**3 + p**4\n",
+                "    h3 = q**5 + q**4*p + q**3*p**2 + q**2*p**3 + q*p**4 + p**5\n",
+                "    return h1 + h2 + h3\n",
+                "\n",
+                "x = torch.tensor([0.0, 0.0], dtype=dtype, device=device)\n",
+                "u = torch.tensor([0.0], dtype=dtype, device=device)\n",
+                "v = torch.tensor([0.0], dtype=dtype, device=device)\n",
+                "\n",
+                "h = derivative((5, 2, 1), h, x, u, v)\n",
+                "chop(h, replace=True)\n",
+                "\n",
+                "s, *_ = split(clean(series((2, 1, 1), (5, 2, 1), h)))\n",
+                "s"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 4,
+            "id": "1fcb9c0c-4136-49b9-9639-9532c15155b8",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [],
+            "source": [
+                "# Compute solution\n",
+                "\n",
+                "t = solution((4, 2, 1), x, [u, v], h)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 5,
+            "id": "c30313c7-b21d-4a38-9a1b-36651a60691e",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "True"
+                        ]
+                    },
+                    "execution_count": 5,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "# Compute hamiltonian from solution and compare\n",
+                "\n",
+                "compare(h, hamiltonian((4, 2, 1), x, [u, v], t))"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 6,
+            "id": "c7e423a0-73e0-4c22-8d83-6648b670f1f7",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [],
+            "source": [
+                "# Perform factorization\n",
+                "\n",
+                "h1, h2, h3, *_ = factorize((4, 2, 1), x, [u, v], t)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 7,
+            "id": "9a14155f-01b8-4224-a93f-55610417aa9a",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "{(3, 0, 0, 0): tensor(1.000000000000e+00, dtype=torch.float64),\n",
+                            " (2, 1, 0, 0): tensor(1.000000000000e+00, dtype=torch.float64),\n",
+                            " (1, 2, 0, 0): tensor(1.000000000000e+00, dtype=torch.float64),\n",
+                            " (0, 3, 0, 0): tensor(1.000000000000e+00, dtype=torch.float64),\n",
+                            " (3, 0, 1, 0): tensor(1.000000000000e+00, dtype=torch.float64)}"
+                        ]
+                    },
+                    "execution_count": 7,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "# Examine series representation\n",
+                "\n",
+                "s, *_ = split(clean(series((2, 1, 1), (5, 1), h1)))\n",
+                "s"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 8,
+            "id": "4c099717-836f-48b6-9dbb-84a3b9ce5455",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "{(4, 0, 0, 0): tensor(1.000000000000e+00, dtype=torch.float64),\n",
+                            " (3, 1, 0, 0): tensor(1.000000000000e+00, dtype=torch.float64),\n",
+                            " (2, 2, 0, 0): tensor(1.000000000000e+00, dtype=torch.float64),\n",
+                            " (1, 3, 0, 0): tensor(1.000000000000e+00, dtype=torch.float64),\n",
+                            " (0, 4, 0, 0): tensor(1.000000000000e+00, dtype=torch.float64),\n",
+                            " (4, 0, 0, 1): tensor(1.000000000000e+00, dtype=torch.float64)}"
+                        ]
+                    },
+                    "execution_count": 8,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "# Examine series representation\n",
+                "\n",
+                "s, *_ = split(clean(series((2, 1, 1), (5, 1), h2)))\n",
+                "s"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 9,
+            "id": "1f97e5ac-3cdb-4b24-a8bf-0e8c15d8a17f",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "{(5, 0, 0, 0): tensor(5.000000000000e-01, dtype=torch.float64),\n",
+                            " (4, 1, 0, 0): tensor(-5.000000000000e-01, dtype=torch.float64),\n",
+                            " (3, 2, 0, 0): tensor(-2.000000000000e+00, dtype=torch.float64),\n",
+                            " (2, 3, 0, 0): tensor(4.000000000000e+00, dtype=torch.float64),\n",
+                            " (1, 4, 0, 0): tensor(2.500000000000e+00, dtype=torch.float64),\n",
+                            " (0, 5, 0, 0): tensor(1.500000000000e+00, dtype=torch.float64),\n",
+                            " (5, 0, 0, 1): tensor(-2.000000000000e+00, dtype=torch.float64),\n",
+                            " (4, 1, 0, 1): tensor(-4.000000000000e+00, dtype=torch.float64),\n",
+                            " (3, 2, 0, 1): tensor(-6.000000000000e+00, dtype=torch.float64),\n",
+                            " (5, 0, 1, 0): tensor(1.500000000000e+00, dtype=torch.float64),\n",
+                            " (4, 1, 1, 0): tensor(3.000000000000e+00, dtype=torch.float64),\n",
+                            " (3, 2, 1, 0): tensor(4.500000000000e+00, dtype=torch.float64),\n",
+                            " (2, 3, 1, 0): tensor(6.000000000000e+00, dtype=torch.float64)}"
+                        ]
+                    },
+                    "execution_count": 9,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "# Examine series representation\n",
+                "\n",
+                "s, *_ = split(clean(series((2, 1, 1), (5, 1), h3)))\n",
+                "s"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 10,
+            "id": "fef41af0-cc19-4eaf-bc96-def01749691d",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [],
+            "source": [
+                "# Compute solutions\n",
+                "\n",
+                "t1 = solution((4, 2, 1), x, [u, v], h1)\n",
+                "t2 = solution((4, 2, 1), x, [u, v], h2)\n",
+                "t3 = solution((4, 2, 1) ,x, [u, v], h3)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 11,
+            "id": "5d3545d6-d9d4-40ee-bb5f-6b97bb268509",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "True"
+                        ]
+                    },
+                    "execution_count": 11,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "# Compose individual solutions and compare with initial solution\n",
+                "\n",
+                "T = identity((4, 2, 1), [x, u, v])\n",
+                "T = propagate((2, 1, 1), (4, 2, 1), T, [u, v], t1)\n",
+                "T = propagate((2, 1, 1), (4, 2, 1), T, [u, v], t2)\n",
+                "T = propagate((2, 1, 1), (4, 2, 1), T, [u, v], t3)\n",
+                "compare(t, T)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "bae67b59-1584-4879-9255-8096c603f900",
+            "metadata": {},
+            "outputs": [],
+            "source": []
         }
     ],
     "metadata": {
         "colab": {
             "collapsed_sections": [
                 "myt0_gMIOq7b",
                 "5d97819c"
@@ -11672,15 +12201,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.10"
+            "version": "3.11.2"
         },
         "latex_envs": {
             "LaTeX_envs_menu_present": true,
             "autoclose": false,
             "autocomplete": true,
             "bibliofile": "biblio.bib",
             "cite_by": "apalike",
```

### Comparing `ndtorch-0.1.5/pyproject.toml` & `ndtorch-0.1.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ndtorch"
-version = "0.1.5"
+version = "0.1.6"
 authors = [{name = "Ivan Morozov", email = "i.a.morozov@inp.nsk.su"}]
 description = "Higher order partial derivatives computation with respect to one or several tensor-like variables, application to nonlinear dynamics"
 readme = "README.MD"
 requires-python = ">=3.10"
 keywords = ["torch", "derivative"]
 license = {text = "MIT"}
 classifiers = ["Programming Language :: Python :: 3"]
```

