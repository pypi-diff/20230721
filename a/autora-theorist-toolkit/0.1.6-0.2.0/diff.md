# Comparing `tmp/autora-theorist-toolkit-0.1.6.tar.gz` & `tmp/autora-theorist-toolkit-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autora-theorist-toolkit-0.1.6.tar", last modified: Mon Jul 17 20:52:54 2023, max compression
+gzip compressed data, was "autora-theorist-toolkit-0.2.0.tar", last modified: Fri Jul 21 18:46:24 2023, max compression
```

## Comparing `autora-theorist-toolkit-0.1.6.tar` & `autora-theorist-toolkit-0.2.0.tar`

### file list

```diff
@@ -1,67 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:52:54.348922 autora-theorist-toolkit-0.1.6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:52:54.340922 autora-theorist-toolkit-0.1.6/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-07-17 20:52:41.000000 autora-theorist-toolkit-0.1.6/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:52:54.340922 autora-theorist-toolkit-0.1.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-17 20:52:41.000000 autora-theorist-toolkit-0.1.6/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-07-17 20:52:41.000000 autora-theorist-toolkit-0.1.6/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:52:54.340922 autora-theorist-toolkit-0.1.6/.idea/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-17 20:52:41.000000 autora-theorist-toolkit-0.1.6/.idea/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-17 20:52:41.000000 autora-theorist-toolkit-0.1.6/.idea/autora-theorist-toolkit.iml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:52:54.340922 autora-theorist-toolkit-0.1.6/.idea/inspectionProfiles/
--rw-r--r--   0 runner    (1001) docker     (123)     6853 2023-07-17 20:52:41.000000 autora-theorist-toolkit-0.1.6/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-17 20:52:41.000000 autora-theorist-toolkit-0.1.6/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-17 20:52:41.000000 autora-theorist-toolkit-0.1.6/.idea/misc.xml
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-17 20:52:41.000000 autora-theorist-toolkit-0.1.6/.idea/modules.xml
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-17 20:52:41.000000 autora-theorist-toolkit-0.1.6/.idea/vcs.xml
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-17 20:52:41.000000 autora-theorist-toolkit-0.1.6/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     7212 2023-07-17 20:52:54.348922 autora-theorist-toolkit-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-07-17 20:52:41.000000 autora-theorist-toolkit-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:52:54.340922 autora-theorist-toolkit-0.1.6/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-07-17 20:52:41.000000 autora-theorist-toolkit-0.1.6/docs/Additional Example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-07-17 20:52:41.000000 autora-theorist-toolkit-0.1.6/docs/Basic Usage.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-17 20:52:41.000000 autora-theorist-toolkit-0.1.6/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:52:54.340922 autora-theorist-toolkit-0.1.6/docs/javascripts/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-17 20:52:41.000000 autora-theorist-toolkit-0.1.6/docs/javascripts/mathjax.js
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-17 20:52:41.000000 autora-theorist-toolkit-0.1.6/docs/quickstart.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:52:54.340922 autora-theorist-toolkit-0.1.6/mkdocs/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-17 20:52:41.000000 autora-theorist-toolkit-0.1.6/mkdocs/base.yml
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-17 20:52:41.000000 autora-theorist-toolkit-0.1.6/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-17 20:52:41.000000 autora-theorist-toolkit-0.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 20:52:54.348922 autora-theorist-toolkit-0.1.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:52:54.340922 autora-theorist-toolkit-0.1.6/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 20:52:41.000000 autora-theorist-toolkit-0.1.6/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:52:54.340922 autora-theorist-toolkit-0.1.6/src/autora/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 20:52:41.000000 autora-theorist-toolkit-0.1.6/src/autora/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:52:54.344922 autora-theorist-toolkit-0.1.6/src/autora/theorist/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 20:52:41.000000 autora-theorist-toolkit-0.1.6/src/autora/theorist/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:52:54.344922 autora-theorist-toolkit-0.1.6/src/autora/theorist/toolkit/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-17 20:52:41.000000 autora-theorist-toolkit-0.1.6/src/autora/theorist/toolkit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:52:54.344922 autora-theorist-toolkit-0.1.6/src/autora/theorist/toolkit/components/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 20:52:41.000000 autora-theorist-toolkit-0.1.6/src/autora/theorist/toolkit/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3954 2023-07-17 20:52:41.000000 autora-theorist-toolkit-0.1.6/src/autora/theorist/toolkit/components/nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-17 20:52:41.000000 autora-theorist-toolkit-0.1.6/src/autora/theorist/toolkit/components/primitives.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:52:54.344922 autora-theorist-toolkit-0.1.6/src/autora/theorist/toolkit/methods/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 20:52:41.000000 autora-theorist-toolkit-0.1.6/src/autora/theorist/toolkit/methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-07-17 20:52:41.000000 autora-theorist-toolkit-0.1.6/src/autora/theorist/toolkit/methods/fitting.py
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-07-17 20:52:41.000000 autora-theorist-toolkit-0.1.6/src/autora/theorist/toolkit/methods/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-07-17 20:52:41.000000 autora-theorist-toolkit-0.1.6/src/autora/theorist/toolkit/methods/regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-07-17 20:52:41.000000 autora-theorist-toolkit-0.1.6/src/autora/theorist/toolkit/methods/rules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:52:54.344922 autora-theorist-toolkit-0.1.6/src/autora/theorist/toolkit/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 20:52:41.000000 autora-theorist-toolkit-0.1.6/src/autora/theorist/toolkit/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3732 2023-07-17 20:52:41.000000 autora-theorist-toolkit-0.1.6/src/autora/theorist/toolkit/models/bayesian_machine_scientist.py
--rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-07-17 20:52:41.000000 autora-theorist-toolkit-0.1.6/src/autora/theorist/toolkit/models/bayesian_symbolic_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-07-17 20:52:41.000000 autora-theorist-toolkit-0.1.6/src/autora/theorist/toolkit/models/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-07-17 20:52:41.000000 autora-theorist-toolkit-0.1.6/src/autora/theorist/toolkit/models/parallel_symbolic_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)    10329 2023-07-17 20:52:41.000000 autora-theorist-toolkit-0.1.6/src/autora/theorist/toolkit/models/symbolic_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     3968 2023-07-17 20:52:41.000000 autora-theorist-toolkit-0.1.6/src/autora/theorist/toolkit/models/tree.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-17 20:52:41.000000 autora-theorist-toolkit-0.1.6/src/autora/theorist/toolkit/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:52:54.348922 autora-theorist-toolkit-0.1.6/src/autora_theorist_toolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7212 2023-07-17 20:52:54.000000 autora-theorist-toolkit-0.1.6/src/autora_theorist_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-07-17 20:52:54.000000 autora-theorist-toolkit-0.1.6/src/autora_theorist_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 20:52:54.000000 autora-theorist-toolkit-0.1.6/src/autora_theorist_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-17 20:52:54.000000 autora-theorist-toolkit-0.1.6/src/autora_theorist_toolkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-17 20:52:54.000000 autora-theorist-toolkit-0.1.6/src/autora_theorist_toolkit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:52:54.348922 autora-theorist-toolkit-0.1.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-07-17 20:52:41.000000 autora-theorist-toolkit-0.1.6/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 20:52:41.000000 autora-theorist-toolkit-0.1.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-17 20:52:41.000000 autora-theorist-toolkit-0.1.6/tests/test_toolkit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:46:24.142157 autora-theorist-toolkit-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:46:24.130157 autora-theorist-toolkit-0.2.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-07-21 18:46:11.000000 autora-theorist-toolkit-0.2.0/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:46:24.130157 autora-theorist-toolkit-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-21 18:46:11.000000 autora-theorist-toolkit-0.2.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-07-21 18:46:11.000000 autora-theorist-toolkit-0.2.0/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:46:24.134157 autora-theorist-toolkit-0.2.0/.idea/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-21 18:46:11.000000 autora-theorist-toolkit-0.2.0/.idea/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-21 18:46:11.000000 autora-theorist-toolkit-0.2.0/.idea/autora-theorist-toolkit.iml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:46:24.134157 autora-theorist-toolkit-0.2.0/.idea/inspectionProfiles/
+-rw-r--r--   0 runner    (1001) docker     (123)     6853 2023-07-21 18:46:11.000000 autora-theorist-toolkit-0.2.0/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-21 18:46:11.000000 autora-theorist-toolkit-0.2.0/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-21 18:46:11.000000 autora-theorist-toolkit-0.2.0/.idea/misc.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-21 18:46:11.000000 autora-theorist-toolkit-0.2.0/.idea/modules.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-21 18:46:11.000000 autora-theorist-toolkit-0.2.0/.idea/vcs.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-21 18:46:11.000000 autora-theorist-toolkit-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     7212 2023-07-21 18:46:24.142157 autora-theorist-toolkit-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-07-21 18:46:11.000000 autora-theorist-toolkit-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:46:24.134157 autora-theorist-toolkit-0.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-07-21 18:46:11.000000 autora-theorist-toolkit-0.2.0/docs/Additional Example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-07-21 18:46:11.000000 autora-theorist-toolkit-0.2.0/docs/Basic Usage.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-21 18:46:11.000000 autora-theorist-toolkit-0.2.0/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:46:24.134157 autora-theorist-toolkit-0.2.0/docs/javascripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-21 18:46:11.000000 autora-theorist-toolkit-0.2.0/docs/javascripts/mathjax.js
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-21 18:46:11.000000 autora-theorist-toolkit-0.2.0/docs/quickstart.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:46:24.134157 autora-theorist-toolkit-0.2.0/mkdocs/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-21 18:46:11.000000 autora-theorist-toolkit-0.2.0/mkdocs/base.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-21 18:46:11.000000 autora-theorist-toolkit-0.2.0/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-21 18:46:11.000000 autora-theorist-toolkit-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 18:46:24.142157 autora-theorist-toolkit-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:46:24.134157 autora-theorist-toolkit-0.2.0/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 18:46:11.000000 autora-theorist-toolkit-0.2.0/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:46:24.134157 autora-theorist-toolkit-0.2.0/src/autora/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 18:46:11.000000 autora-theorist-toolkit-0.2.0/src/autora/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:46:24.134157 autora-theorist-toolkit-0.2.0/src/autora/theorist/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 18:46:11.000000 autora-theorist-toolkit-0.2.0/src/autora/theorist/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:46:24.134157 autora-theorist-toolkit-0.2.0/src/autora/theorist/toolkit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 18:46:11.000000 autora-theorist-toolkit-0.2.0/src/autora/theorist/toolkit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:46:24.138157 autora-theorist-toolkit-0.2.0/src/autora/theorist/toolkit/components/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 18:46:11.000000 autora-theorist-toolkit-0.2.0/src/autora/theorist/toolkit/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-07-21 18:46:11.000000 autora-theorist-toolkit-0.2.0/src/autora/theorist/toolkit/components/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-21 18:46:11.000000 autora-theorist-toolkit-0.2.0/src/autora/theorist/toolkit/components/primitives.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:46:24.138157 autora-theorist-toolkit-0.2.0/src/autora/theorist/toolkit/methods/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 18:46:11.000000 autora-theorist-toolkit-0.2.0/src/autora/theorist/toolkit/methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-07-21 18:46:11.000000 autora-theorist-toolkit-0.2.0/src/autora/theorist/toolkit/methods/fitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-07-21 18:46:11.000000 autora-theorist-toolkit-0.2.0/src/autora/theorist/toolkit/methods/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-21 18:46:11.000000 autora-theorist-toolkit-0.2.0/src/autora/theorist/toolkit/methods/regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-21 18:46:11.000000 autora-theorist-toolkit-0.2.0/src/autora/theorist/toolkit/methods/rules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:46:24.142157 autora-theorist-toolkit-0.2.0/src/autora/theorist/toolkit/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 18:46:11.000000 autora-theorist-toolkit-0.2.0/src/autora/theorist/toolkit/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-07-21 18:46:11.000000 autora-theorist-toolkit-0.2.0/src/autora/theorist/toolkit/models/bayesian_machine_scientist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-07-21 18:46:11.000000 autora-theorist-toolkit-0.2.0/src/autora/theorist/toolkit/models/bayesian_symbolic_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 18:46:11.000000 autora-theorist-toolkit-0.2.0/src/autora/theorist/toolkit/models/ddm_bms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-07-21 18:46:11.000000 autora-theorist-toolkit-0.2.0/src/autora/theorist/toolkit/models/hierarchical_bayesian_symbolic_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-07-21 18:46:11.000000 autora-theorist-toolkit-0.2.0/src/autora/theorist/toolkit/models/hierarchical_symbolic_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-07-21 18:46:11.000000 autora-theorist-toolkit-0.2.0/src/autora/theorist/toolkit/models/hybrid_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-21 18:46:11.000000 autora-theorist-toolkit-0.2.0/src/autora/theorist/toolkit/models/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-07-21 18:46:11.000000 autora-theorist-toolkit-0.2.0/src/autora/theorist/toolkit/models/parallel_symbolic_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10785 2023-07-21 18:46:11.000000 autora-theorist-toolkit-0.2.0/src/autora/theorist/toolkit/models/symbolic_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-07-21 18:46:11.000000 autora-theorist-toolkit-0.2.0/src/autora/theorist/toolkit/models/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-21 18:46:11.000000 autora-theorist-toolkit-0.2.0/src/autora/theorist/toolkit/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:46:24.142157 autora-theorist-toolkit-0.2.0/src/autora_theorist_toolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7212 2023-07-21 18:46:24.000000 autora-theorist-toolkit-0.2.0/src/autora_theorist_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-07-21 18:46:24.000000 autora-theorist-toolkit-0.2.0/src/autora_theorist_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 18:46:24.000000 autora-theorist-toolkit-0.2.0/src/autora_theorist_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-21 18:46:24.000000 autora-theorist-toolkit-0.2.0/src/autora_theorist_toolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-21 18:46:24.000000 autora-theorist-toolkit-0.2.0/src/autora_theorist_toolkit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:46:24.142157 autora-theorist-toolkit-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-07-21 18:46:11.000000 autora-theorist-toolkit-0.2.0/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 18:46:11.000000 autora-theorist-toolkit-0.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-21 18:46:11.000000 autora-theorist-toolkit-0.2.0/tests/test_toolkit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-07-21 18:46:11.000000 autora-theorist-toolkit-0.2.0/tests/test_visual.py
```

### Comparing `autora-theorist-toolkit-0.1.6/.github/pull_request_template.md` & `autora-theorist-toolkit-0.2.0/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.1.6/.github/workflows/python-publish.yml` & `autora-theorist-toolkit-0.2.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.1.6/.gitignore` & `autora-theorist-toolkit-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.1.6/.idea/inspectionProfiles/Project_Default.xml` & `autora-theorist-toolkit-0.2.0/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.1.6/.pre-commit-config.yaml` & `autora-theorist-toolkit-0.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.1.6/PKG-INFO` & `autora-theorist-toolkit-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autora-theorist-toolkit
-Version: 0.1.6
+Version: 0.2.0
 Summary: Toolkit to build algorithms for model recovery
 Author-email: "Joshua T. S. Hewson" <joshua_hewson@brown.edu>
 License: MIT license
 Project-URL: homepage, http://www.empiricalresearch.ai
 Project-URL: repository, https://github.com/TheLemonPig/autora-theorist-toolkit
 Project-URL: documentation, https://autoresearch.github.io/autora/
 Requires-Python: <4,>=3.8
```

### Comparing `autora-theorist-toolkit-0.1.6/README.md` & `autora-theorist-toolkit-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.1.6/docs/Additional Example.ipynb` & `autora-theorist-toolkit-0.2.0/docs/Additional Example.ipynb`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.1.6/docs/Basic Usage.ipynb` & `autora-theorist-toolkit-0.2.0/docs/Basic Usage.ipynb`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.1.6/docs/index.md` & `autora-theorist-toolkit-0.2.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.1.6/mkdocs/base.yml` & `autora-theorist-toolkit-0.2.0/mkdocs/base.yml`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.1.6/pyproject.toml` & `autora-theorist-toolkit-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.1.6/src/autora/theorist/toolkit/components/nodes.py` & `autora-theorist-toolkit-0.2.0/src/autora/theorist/toolkit/components/nodes.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,46 +1,46 @@
-from typing import List, Callable
 from inspect import signature
+from typing import Callable, List
+
 from autora.theorist.toolkit.components.primitives import Arithmetic
 
 ###############
 #       Objects
 ###############
 
 
 ###
 # TreeNode
 ###
 # attributes:
 #   parent: Node object
 #   offspring: list of Node objects
 class TreeNode:
-
     def __init__(self, parent=None, children=None):
         self._parent: __class__.__name__ = parent
         self._children: List[__class__.__name__] = [] if children is None else children
 
     def __call__(self, x):
-        raise TypeError('Uninitialized Node cannot be evaluated')
+        raise TypeError("Uninitialized Node cannot be evaluated")
 
     def __getitem__(self, item):
         if isinstance(item, list):
             if len(item) > 0:
                 return self.__getitem__(item[0]).__getitem__(item[1:])
             else:
-                raise KeyError('Specified tree location does not exist')
+                raise KeyError("Specified tree location does not exist")
         else:
             if item == -1:
                 return self._parent
             else:
                 return self._children[item]
 
     # TODO: update __repr__ to collect node and all descendants
     def __repr__(self):
-        return '...'
+        return "..."
 
     def get_parent(self):
         return self._parent
 
     def get_children(self):
         return self._children
 
@@ -70,56 +70,58 @@
         self._children[self._children.index(old)] = new
 
     def replace_parent(self, parent):
         self._parent = parent
 
 
 class Symbol(TreeNode):
-
     def __init__(self, parent=None, children=None):
         super().__init__(parent, children)
         self._value = None
-        self._label = 'R'
+        self._label = "R"
 
     def __repr__(self):
         return self._label
 
     def is_initialized(self):
         return self._value is not None
 
     def is_filled(self):
-        return self.is_initialized() and all(children.is_filled() for children in self.get_children())
+        return self.is_initialized() and all(
+            children.is_filled() for children in self.get_children()
+        )
 
     def get_value(self):
         return self._value
 
     def args(self):
         return []
 
 
 class Variable(Symbol):
-
     def __init__(self, value, parent=None):
         super().__init__(parent=parent)
         self._label = value
         self._value: int = int(value[2:-1])
 
     def __call__(self, x):
         try:
             return x[self._label]
         except KeyError:
             try:
                 return x[self._value]
             except KeyError:
-                raise KeyError('Data does not contain label for variable: ' +
-                               self._label+', nor is large enough to imply')
+                raise KeyError(
+                    "Data does not contain label for variable: "
+                    + self._label
+                    + ", nor is large enough to imply"
+                )
 
 
 class Parameter(Symbol):
-
     def __init__(self, value=0.0, parent=None):
         super().__init__(parent=parent, children=None)
         self._value: float = value
 
     def __call__(self, x, *parameters):
         return self.get_value()
 
@@ -127,22 +129,34 @@
         self._label = label
 
     def set_value(self, num):
         self._value = num
 
 
 class Operator(Symbol):
-
     def __init__(self, value, parent=None):
-        super().__init__(parent=parent,
-                         children=[Symbol(parent=self) for _ in signature(value).parameters])
+        super().__init__(
+            parent=parent,
+            children=[Symbol(parent=self) for _ in signature(value).parameters],
+        )
         self._value: Callable = value
         self._label: str = str(value)
 
     def __repr__(self):
         if isinstance(self._value, Arithmetic):
-            return '('+self._children[0].__repr__() + str(self._value) + self._children[1].__repr__()+')'
+            return (
+                "("
+                + self._children[0].__repr__()
+                + str(self._value)
+                + self._children[1].__repr__()
+                + ")"
+            )
         else:
-            return str(self._value) + '(' + ','.join(child.__repr__() for child in self.get_children()) + ')'
+            return (
+                str(self._value)
+                + "("
+                + ",".join(child.__repr__() for child in self.get_children())
+                + ")"
+            )
 
     def args(self):
         return signature(self._value).parameters
```

### Comparing `autora-theorist-toolkit-0.1.6/src/autora/theorist/toolkit/methods/fitting.py` & `autora-theorist-toolkit-0.2.0/src/autora/theorist/toolkit/methods/fitting.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-from sklearn.utils.validation import assert_all_finite
-import numpy as np
-from scipy.optimize import curve_fit, OptimizeWarning
-from typing import Callable
 import warnings
+from typing import Callable
+
+import numpy as np
+from scipy.optimize import OptimizeWarning, curve_fit
+from sklearn.utils.validation import assert_all_finite
 
 
 ###
 # scipy_curve_fit
 ###
 # takes: model [Callable], x [pandas/numpy], y [pandas/numpy]
 # uses: scipy curve_fit function
@@ -17,19 +18,18 @@
     warnings.filterwarnings("ignore", category=OptimizeWarning)
     warnings.filterwarnings("ignore", category=RuntimeWarning)
     try:
         fitted_parameters = curve_fit(expr_func, Xs, y)[0]
         assert_all_finite(fitted_parameters)
         return fitted_parameters
     except (ValueError, ZeroDivisionError, TypeError, RuntimeError) as err:
-        raise FittingError(err, 'scipy\'s curve fit failed')
+        raise FittingError(err, "scipy's curve fit failed")
 
 
 def fit_parameters(X: np.ndarray, y: np.ndarray, expr_func, fit_func=scipy_curve_fit):
     return fit_func(X, y, expr_func)
 
 
 class FittingError(Exception):
-
-    def __init__(self, err, message=''):
-        message += '\n'+str(err)
+    def __init__(self, err, message=""):
+        message += "\n" + str(err)
         super().__init__(message)
```

### Comparing `autora-theorist-toolkit-0.1.6/src/autora/theorist/toolkit/methods/metrics.py` & `autora-theorist-toolkit-0.2.0/src/autora/theorist/toolkit/methods/metrics.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import numpy as np
 from sklearn.metrics import mean_squared_error
+
 from autora.theorist.toolkit.models.symbolic_regression import SymbolicRegressor
 
 
 def continuous_log_loss(mse):
     return np.log(mse)
 
 
@@ -16,61 +17,55 @@
 def priors(prior_dict, expr_str):
     prior = 0
     for k in prior_dict.keys():
         prior += prior_dict[k] * expr_str.count(k)
     return prior
 
 
-def minimum_description_length(y_true, y_pred, n, k, prior_dict, expr_str, temperature=1.0):
+def minimum_description_length(
+    y_true, y_pred, n, k, prior_dict, expr_str, temperature=1.0
+):
     bic = continuous_bayesian_information_criterion(y_true, y_pred, n, k)
     prior = priors(prior_dict, expr_str)
-    return bic/2/temperature + prior
+    return bic / 2 / temperature + prior
 
 
 class Loss:
-
     def __init__(self):
         ...
 
     def __call__(self, y_true, y_pred) -> float:
-        ...
+        return 0.0
 
 
 class MinimumDescriptionLength:
-
     def __init__(self, n, k, prior_dict, expr_str, bic_temp=1, prior_temp=1):
         super().__init__()
         self.n = n
         self.k = k
         self.prior_dict = prior_dict
         self.expr_str = expr_str
         self.bic_temp = bic_temp
         self.prior_temp = prior_temp
 
     def __call__(self, y_true, y_pred) -> float:
-        return minimum_description_length(y_true, y_pred, self.n, self.k, self.prior_dict, self.expr_str)
+        return minimum_description_length(
+            y_true, y_pred, self.n, self.k, self.prior_dict, self.expr_str
+        )
 
 
 class MDLChange:
-
     def __init__(self, regressor: SymbolicRegressor, prior_dict, initial_mdl):
         self.regressor = regressor
         self.current_mdl = initial_mdl
         self.prior_dict = prior_dict
 
     def __call__(self, y_true, y_pred):
         n = len(y_pred)
         k = len(self.regressor.model_.get_parameters())
         expr_str = str(self.regressor.model_)
-        new_mdl = minimum_description_length(y_true, y_pred, n, k, self.prior_dict, expr_str)
+        new_mdl = minimum_description_length(
+            y_true, y_pred, n, k, self.prior_dict, expr_str
+        )
         mdl_change = new_mdl - self.current_mdl
         self.current_mdl = new_mdl
         return mdl_change
-
-# class MDLChange(MDLLoss):
-#
-#     def __init__(self, n_old, n_new, k_old, k_new, prior_dict, expr_str_old, expr_str_new, bic_temp=1, prior_temp=1):
-#         self.old = super().__init__(n_old, k_old, prior_dict, expr_str_old, bic_temp, prior_temp)
-#         self.new = super().__init__(n_new, k_new, prior_dict, expr_str_new, bic_temp, prior_temp)
-#
-#     def __call__(self, y_true, y_pred) -> float:
-#         return self.new(y_true, y_pred) - self.old(y_true, y_pred)
```

### Comparing `autora-theorist-toolkit-0.1.6/src/autora/theorist/toolkit/methods/regression.py` & `autora-theorist-toolkit-0.2.0/src/autora/theorist/toolkit/methods/regression.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,40 @@
 import functools
 import warnings
-from autora.theorist.toolkit.methods.fitting import FittingError
-from sympy import sympify
+
 from scipy.optimize import OptimizeWarning
-import functools
+from sympy import sympify
+
+from autora.theorist.toolkit.methods.fitting import FittingError
 
 
 def regression_handler(func):
     @functools.wraps(func)
     def handler(obj, *args, **kwargs):
         warnings.filterwarnings("ignore", category=OptimizeWarning)
         warnings.filterwarnings("ignore", category=RuntimeWarning)
-        assert hasattr(obj, 'back_step'), 'Regression Handler assumes back_step method'
+        assert hasattr(obj, "back_step"), "Regression Handler assumes back_step method"
         with warnings.catch_warnings():
             warnings.filterwarnings("ignore")
             try:
                 func(obj, *args, **kwargs)
             except (FittingError, TypeError, ValueError, ZeroDivisionError):
                 obj.back_step()
+
     return handler
 
 
 def canonical(expr_str: str):
-    expr_str = expr_str.replace('np.', '')
+    expr_str = expr_str.replace("np.", "")
     expr_sym = sympify(expr_str)
     expr_str = str(expr_sym)
-    while '__a' in expr_str:
-        start = expr_str.index('__a')
-        stop = expr_str.index('__', start+1) + 2
-        expr_str = expr_str[:start]+'__c__'+expr_str[stop:]
+    while "__a" in expr_str:
+        start = expr_str.index("__a")
+        stop = expr_str.index("__", start + 1) + 2
+        expr_str = expr_str[:start] + "__c__" + expr_str[stop:]
     return expr_str
 
+
 def clean_equation(expr_str):
-    expr_str = expr_str.replace('np.', '')
+    expr_str = expr_str.replace("np.", "")
     expr_sym = sympify(expr_str)
     return str(expr_sym)
```

### Comparing `autora-theorist-toolkit-0.1.6/src/autora/theorist/toolkit/methods/rules.py` & `autora-theorist-toolkit-0.2.0/src/autora/theorist/toolkit/methods/rules.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-import numpy as np
 from random import random
 
+import numpy as np
+
 
 def less_than(a, b):
     return a < b
 
 
 def remove_root(mdl_change):
     return np.log(random()) < -mdl_change
@@ -28,21 +29,23 @@
 # Define its p(accept) rule
 
 
 def bms_accept():
     ...
 
 
-rulebook = dict({
-    'None/Root': add_root,
-    'Root/None': remove_root,
-    'Node/Node': replace_node,
-    'Node/Leaf': replace_node,
-    'Leaf/Node': replace_node,
-    # 'Node/Leaf': replace_elementary_tree,
-    # 'Leaf/Node': replace_elementary_tree,
-    'Leaf/Leaf': replace_node,
-})
+rulebook = dict(
+    {
+        "None/Root": add_root,
+        "Root/None": remove_root,
+        "Node/Node": replace_node,
+        "Node/Leaf": replace_node,
+        "Leaf/Node": replace_node,
+        # 'Node/Leaf': replace_elementary_tree,
+        # 'Leaf/Node': replace_elementary_tree,
+        "Leaf/Leaf": replace_node,
+    }
+)
 
 # if __name__ == '__main__':
 #     print(less_than(3, 4))
 #     print(less_than)
```

### Comparing `autora-theorist-toolkit-0.1.6/src/autora/theorist/toolkit/models/bayesian_symbolic_regression.py` & `autora-theorist-toolkit-0.2.0/src/autora/theorist/toolkit/models/bayesian_symbolic_regression.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,77 +1,90 @@
-from autora.theorist.toolkit.models.symbolic_regression import SymbolicRegressor
-from autora.theorist.toolkit.methods.rules import add_root, remove_root, replace_node
-from autora.theorist.toolkit.methods.metrics import minimum_description_length
+import random
+
 from autora.theorist.toolkit.methods.fitting import scipy_curve_fit
+from autora.theorist.toolkit.methods.metrics import minimum_description_length
 from autora.theorist.toolkit.methods.regression import regression_handler
-import random
+from autora.theorist.toolkit.methods.rules import add_root, remove_root, replace_node
+from autora.theorist.toolkit.models.symbolic_regression import SymbolicRegressor
 
 
 class BayesianSymbolicRegressor(SymbolicRegressor):
-
     def __init__(self, prior_dict, temperature=1.0, tree=None, moves=None):
         super().__init__(tree, moves)
         self.temperature = temperature
         self.prior_dict = prior_dict
 
     @regression_handler
     def mcmc_step(self, X, y, fitter=scipy_curve_fit):
         move = random.choice(self._moves)
         kwargs = self.get_stats(move, X, y)
 
         self.step(move=move)
         if not self.visited():
             self.optimize_parameters(X, y, fitter)
-            kwargs['new_mdl'] = minimum_description_length(y_true=y, y_pred=self.predict(X),
-                                                           n=X.shape[0], k=len(self.get_parameters()),
-                                                           prior_dict=self.prior_dict, expr_str=str(self.model_),
-                                                           temperature=self.temperature)
+            kwargs["new_mdl"] = minimum_description_length(
+                y_true=y,
+                y_pred=self.predict(X),
+                n=X.shape[0],
+                k=len(self.get_parameters()),
+                prior_dict=self.prior_dict,
+                expr_str=str(self.model_),
+                temperature=self.temperature,
+            )
             # mse = mean_squared_error(y, self.predict(X))
             # print(f"model: {str(self.model_)}, mse: {mse}, mdl: {kwargs['new_mdl']}")
             self._record_visit()
             if self.mcmc_ruling(move, **kwargs):
-                self._error = kwargs['new_mdl']
+                self._error = kwargs["new_mdl"]
             else:
                 self.back_step()
         else:
             self.back_step()
 
     # return relevant stats for this mcmc move
     def get_stats(self, move, X, y):
         stats = dict()
-        stats['X'], stats['y'] = X, y
-        stats['expr_str'] = str(self.model_)
-        stats['old_mdl'] = minimum_description_length(y_true=y, y_pred=self.predict(X),
-                                                      n=X.shape[0], k=len(self.get_parameters()),
-                                                      prior_dict=self.prior_dict, expr_str=str(self.model_),
-                                                      temperature=self.temperature)
-        if move == 'None/Root':
-            stats['num_rr'] = self.get_num_root_options()
-        elif move == 'Root/None':
+        stats["X"], stats["y"] = X, y
+        stats["expr_str"] = str(self.model_)
+        stats["old_mdl"] = minimum_description_length(
+            y_true=y,
+            y_pred=self.predict(X),
+            n=X.shape[0],
+            k=len(self.get_parameters()),
+            prior_dict=self.prior_dict,
+            expr_str=str(self.model_),
+            temperature=self.temperature,
+        )
+        if move == "None/Root":
+            stats["num_rr"] = self.get_num_root_options()
+        elif move == "Root/None":
             pass
-        elif move == 'Node/Node':
+        elif move == "Node/Node":
             pass
-        elif move == 'Node/Leaf':
+        elif move == "Node/Leaf":
             pass
-        elif move == 'Leaf/Node':
+        elif move == "Leaf/Node":
             pass
-        elif move == 'Leaf/Leaf':
+        elif move == "Leaf/Leaf":
             pass
         else:
-            raise KeyError(f'Unrecognized Move Type: {move}')
+            raise KeyError(f"Unrecognized Move Type: {move}")
             # case 'Node/Leaf':
             #     stats['num_options'] = self.get_num_options()
             # case 'Leaf/Node':
             #     stats['num_options'] = self.get_num_options()
         return stats
 
     # currently assumes operators of order 1 or 2 only
     def get_num_root_options(self):
         num_leaves = len(self._variables) + len(self.get_parameters())
-        num_rr = len(self._filter_primitives(1)) + len(self._filter_primitives(2)) * num_leaves
+        num_rr = (
+            len(self._filter_primitives(1))
+            + len(self._filter_primitives(2)) * num_leaves
+        )
         return num_rr
 
     # def get_num_options(self):
     #     num_options = sum(
     #         [
     #             int(len(self.ets[oi]) > 0 and (self.size + of - oi) <= self.max_size)
     #             for oi, of in self.move_types
@@ -79,30 +92,24 @@
     #     )
     #     return num_options
 
     # p(accept) rules courtesy of Guimera 2020: https://www.science.org/doi/10.1126/sciadv.aav6971
     # elementary tree p(accept) rule changed based on believed mistakes in author's code
     @staticmethod
     def mcmc_ruling(move, **kwargs):
-        mdl_change = kwargs['new_mdl'] - kwargs['old_mdl']
-        if move == 'None/Root':
-            accept = add_root(mdl_change=mdl_change, num_rr=kwargs['num_rr'])
-        elif move == 'Root/None':
+        mdl_change = kwargs["new_mdl"] - kwargs["old_mdl"]
+        if move == "None/Root":
+            accept = add_root(mdl_change=mdl_change, num_rr=kwargs["num_rr"])
+        elif move == "Root/None":
             accept = remove_root(mdl_change=mdl_change)
-        elif move == 'Node/Node':
+        elif move == "Node/Node":
             accept = replace_node(mdl_change=mdl_change)
-        elif move == 'Leaf/Leaf':
+        elif move == "Leaf/Leaf":
             accept = replace_node(mdl_change=mdl_change)
-        elif move == 'Node/Leaf':
-            # accept = replace_elementary_tree(mdl_change=mdl_change,
-            #                                  nfi=kwargs['num_options'], nif=self.get_num_options(),
-            #                                  )
+        elif move == "Node/Leaf":
             accept = replace_node(mdl_change=mdl_change)
-        elif move == 'Leaf/Node':
+        elif move == "Leaf/Node":
             # TODO: determine how to solve elementary tree p(accept) - very involved to implement
-            # accept = replace_elementary_tree(mdl_change=mdl_change,
-            #                                  nfi=kwargs['num_options'], nif=self.get_num_options(),
-            #                                  )
             accept = replace_node(mdl_change=mdl_change)
         else:
-            raise KeyError(f'Unrecognized move type: {move}')
+            raise KeyError(f"Unrecognized move type: {move}")
         return accept
```

### Comparing `autora-theorist-toolkit-0.1.6/src/autora/theorist/toolkit/models/memory.py` & `autora-theorist-toolkit-0.2.0/src/autora/theorist/toolkit/models/memory.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-from typing import List
+from typing import List, Optional
 
 
 class Stack:
-
-    def __init__(self, stack: List = None, limit: int = 10):
+    def __init__(self, stack: Optional[List] = None, limit: int = 10):
         self._list = list() if stack is None else stack
         self._max = limit
 
     def pop(self):
         try:
             return self._list.pop()
         except IndexError:
-            raise IndexError('No elements in stack to pop')
+            raise IndexError("No elements in stack to pop")
 
     def push(self, e):
         self._list.append(e)
         if self.size() > self._max:
             self._list = self._list[1:]
 
     def size(self):
```

### Comparing `autora-theorist-toolkit-0.1.6/src/autora/theorist/toolkit/models/parallel_symbolic_regression.py` & `autora-theorist-toolkit-0.2.0/src/autora/theorist/toolkit/models/parallel_symbolic_regression.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,90 +1,114 @@
-import numpy as np
 import logging
-from tqdm import tqdm
 import random
+
+import numpy as np
+from tqdm import tqdm
+
 from autora.theorist.toolkit.components.primitives import Arithmetic, SimpleFunction
-from autora.theorist.toolkit.models.symbolic_regression import SymbolicRegressor
 from autora.theorist.toolkit.methods.metrics import MinimumDescriptionLength
 from autora.theorist.toolkit.methods.rules import replace_node
+from autora.theorist.toolkit.models.symbolic_regression import SymbolicRegressor
 
 logging.basicConfig(level=logging.INFO)
 _logger = logging.getLogger(__name__)
 
 
 class ParallelSymbolicRegressor:
-
     def __init__(self, temperatures, prior_dict):
 
         self.temperatures = temperatures
         self.prior_dict = prior_dict
         self.theorists = [SymbolicRegressor() for _ in self.temperatures]
 
-    def fit(self, x, y):
+    def fit(self, x, y, epochs=100):
         n_swaps = 0
         for n in tqdm(range(epochs)):
             for i, theorist in enumerate(self.theorists):
-                metric = MinimumDescriptionLength(n=x.shape[0], k=len(theorist.model_.get_parameters()),
-                                                  prior_dict=self.prior_dict, expr_str=str(theorist.model_),
-                                                  bic_temp=self.temperatures[i])
+                metric = MinimumDescriptionLength(
+                    n=x.shape[0],
+                    k=len(theorist.model_.get_parameters()),
+                    prior_dict=self.prior_dict,
+                    expr_str=str(theorist.model_),
+                    bic_temp=self.temperatures[i],
+                )
                 theorist.fit_step(X=x, y=y, metric=metric)
                 _logger.debug("Finish iteration {}".format(n))
             n_swaps += int(self.tree_swap(x, y))
-        print(f'Number of Tree Swaps: {n_swaps} out of {epochs} epochs')
+        print(f"Number of Tree Swaps: {n_swaps} out of {epochs} epochs")
 
         for theorist in self.theorists:
-            loss = MinimumDescriptionLength(n=x.shape[0], k=len(theorist.model_.get_parameters()),
-                                            prior_dict=self.prior_dict, expr_str=str(theorist.model_),
-                                            bic_temp=self.temperatures[0])
-            print(f'best model: {theorist.model_}\nError: {loss(y, theorist.predict(x))}')
-            param_list = [param[0]+':'+str(param[1]) for param in theorist.model_.get_parameter_dict().items()]
-            print(', '.join(param_list))
+            loss = MinimumDescriptionLength(
+                n=x.shape[0],
+                k=len(theorist.model_.get_parameters()),
+                prior_dict=self.prior_dict,
+                expr_str=str(theorist.model_),
+                bic_temp=self.temperatures[0],
+            )
+            print(
+                f"best model: {theorist.model_}\nError: {loss(y, theorist.predict(x))}"
+            )
+            param_list = [
+                param[0] + ":" + str(param[1])
+                for param in theorist.model_.get_parameter_dict().items()
+            ]
+            print(", ".join(param_list))
 
     def tree_swap(self, x, y):
-        j = random.choice(range(len(self.temperatures)-1))
-        temp1, temp2 = self.temperatures[j:j+2]
-        theorist1, theorist2 = self.theorists[j:j+2]
+        j = random.choice(range(len(self.temperatures) - 1))
+        temp1, temp2 = self.temperatures[j : j + 2]
+        theorist1, theorist2 = self.theorists[j : j + 2]
         y_pred1 = theorist1.predict(x)
         if isinstance(y_pred1, float):
             y_pred1 = np.ones(y.shape) * y_pred1
         y_pred2 = theorist2.predict(x)
         if isinstance(y_pred2, float):
             y_pred2 = np.ones(y.shape) * y_pred2
-        loss1 = MinimumDescriptionLength(n=x.shape[0], k=len(theorist1.model_.get_parameters()),
-                                         prior_dict=self.prior_dict, expr_str=str(theorist1.model_),
-                                         bic_temp=temp1)(y, y_pred1)
-        loss2 = MinimumDescriptionLength(n=x.shape[0], k=len(theorist2.model_.get_parameters()),
-                                         prior_dict=self.prior_dict, expr_str=str(theorist2.model_),
-                                         bic_temp=temp2)(y, y_pred2)
-        mdl_change = loss1*(1/temp2-1/temp1) + loss2*(1/temp1-1/temp2)
+        loss1 = MinimumDescriptionLength(
+            n=x.shape[0],
+            k=len(theorist1.model_.get_parameters()),
+            prior_dict=self.prior_dict,
+            expr_str=str(theorist1.model_),
+            bic_temp=temp1,
+        )(y, y_pred1)
+        loss2 = MinimumDescriptionLength(
+            n=x.shape[0],
+            k=len(theorist2.model_.get_parameters()),
+            prior_dict=self.prior_dict,
+            expr_str=str(theorist2.model_),
+            bic_temp=temp2,
+        )(y, y_pred2)
+        mdl_change = loss1 * (1 / temp2 - 1 / temp1) + loss2 * (1 / temp1 - 1 / temp2)
         if replace_node(-mdl_change):
-            self.theorists[j:j+2] = theorist2, theorist1
+            self.theorists[j : j + 2] = theorist2, theorist1
             return True
         else:
             return False
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     # create synthetic data
     x1 = np.linspace(1, 5, 100).reshape(-1, 1)
     x2 = np.linspace(7, 2, 100).reshape(-1, 1)
-    y_ = x1 ** 2 + x1 + 1
+    y_ = x1**2 + x1 + 1
     x_ = np.hstack((x1, x2))
     # initialize regressor
-    primitives = [
-        Arithmetic(operator) for operator in ['+', '-', '*', '/', '**']
+    primitives = [Arithmetic(operator) for operator in ["+", "-", "*", "/", "**"]]
+    primitives += [
+        SimpleFunction(operator)
+        for operator in ["np.sin", "np.cos", "np.exp", "np.log"]
     ]
-    primitives += [SimpleFunction(operator) for operator in ['np.sin', 'np.cos', 'np.exp', 'np.log']]
-    epochs = 300
-    temps = [1.04 ** n for n in range(20)]
+    epochs_ = 300
+    temps = [1.04**n for n in range(20)]
     # temperatures = [1.0]
-    prior_dict_ = {'+': 10.0,
-                   '-': 3.0,
-                   '*': 10.0,
-                   '/': 3.0,
-                   '**': 10.0,
-                   'sin': 0.01,
-                   'exp': 0.01,
-                   'log': 0.01}
+    prior_dict_ = {
+        "+": 10.0,
+        "-": 3.0,
+        "*": 10.0,
+        "/": 3.0,
+        "**": 10.0,
+        "sin": 0.01,
+        "exp": 0.01,
+        "log": 0.01,
+    }
     bsr = ParallelSymbolicRegressor(temperatures=temps, prior_dict=prior_dict_)
-    bsr.fit(x_, y_)
-
+    bsr.fit(x_, y_, epochs_)
```

### Comparing `autora-theorist-toolkit-0.1.6/src/autora/theorist/toolkit/models/symbolic_regression.py` & `autora-theorist-toolkit-0.2.0/src/autora/theorist/toolkit/models/symbolic_regression.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,42 +1,53 @@
-import numpy as np
-from sklearn.metrics import mean_squared_error
-from sklearn.base import BaseEstimator
-import matplotlib.pyplot as plt
-from tqdm import tqdm
+import random
+from copy import deepcopy
 from inspect import signature
 from typing import List
-from copy import deepcopy
+
+import matplotlib.pyplot as plt
+import numpy as np
 import pandas as pd
-import random
+import scipy
+from sklearn.base import BaseEstimator
+from sklearn.metrics import mean_squared_error
+from tqdm import tqdm
 
-from autora.theorist.toolkit.components.nodes import Variable, Parameter, Operator
+from autora.theorist.toolkit.components.nodes import Operator, Parameter, Variable
 from autora.theorist.toolkit.components.primitives import default_primitives
-from autora.theorist.toolkit.models.tree import Tree
-from autora.theorist.toolkit.models.memory import Stack
 from autora.theorist.toolkit.methods.fitting import scipy_curve_fit
-from autora.theorist.toolkit.methods.regression import regression_handler, canonical
+from autora.theorist.toolkit.methods.regression import canonical, regression_handler
 from autora.theorist.toolkit.methods.rules import less_than
+from autora.theorist.toolkit.models.memory import Stack
+from autora.theorist.toolkit.models.tree import Tree
 
 
 class SymbolicRegressor(BaseEstimator):
 
     # TODO: replace tree=None with expression=None once build_tree() is made
-    def __init__(self, tree=None, moves=None, primitives=None,
-                 metric=None):
+    def __init__(self, tree=None, moves=None, primitives=None, metric=None):
         self.DVs = dict()  # currently unused
         self.IVs = dict()  # currently unused
         self.model_ = Tree() if tree is None else tree
         self.metric = mean_squared_error if metric is None else metric
         self._primitives = default_primitives if primitives is None else primitives
         self._expression = None
         self._value = None
         self._cache: Stack = Stack()
-        self._moves: List[str] = ['Root/None', 'None/Root', 'Node/Node', 'Node/Leaf', 'Leaf/Node', 'Leaf/Leaf']\
-            if moves is None else moves
+        self._moves: List[str] = (
+            [
+                "Root/None",
+                "None/Root",
+                "Node/Node",
+                "Node/Leaf",
+                "Leaf/Node",
+                "Leaf/Leaf",
+            ]
+            if moves is None
+            else moves
+        )
         self._variables: List[str] = list()
         self._trace: List[float] = []
         self._complete(depth=0)
         self._history = []
         self._visit_list = set()
         self._error = np.inf
 
@@ -48,47 +59,68 @@
             # Sci-kit Learn __repr__ method
             super().__repr__(N_CHAR_MAX)
 
     def load_data(self, x, y):
         if isinstance(x, pd.DataFrame) and isinstance(y, pd.DataFrame):
             dv_variables, iv_variables = x.columns, y.columns
         elif isinstance(x, np.ndarray):
-            dv_variables = ['_x' + str(i) + '_' for i in range(x.shape[1])]
-            iv_variables = ['_y' + str(i) + '_' for i in range(y.shape[1])]
+            dv_variables = ["_x" + str(i) + "_" for i in range(x.shape[1])]
+            iv_variables = ["_y" + str(i) + "_" for i in range(y.shape[1])]
         else:
-            raise TypeError('Only valid types for x and y are pandas DataFrames and Numpy nd-arrays')
-        self.DVs = {dv_variables[i]: np.array(x[:, i]) for i in range(len(dv_variables))}
-        self.IVs = {iv_variables[i]: np.array(y[:, i]) for i in range(len(iv_variables))}
+            raise TypeError(
+                "Only valid types for x and y are pandas DataFrames and Numpy nd-arrays"
+            )
+        self.DVs = {
+            dv_variables[i]: np.array(x[:, i]) for i in range(len(dv_variables))
+        }
+        self.IVs = {
+            iv_variables[i]: np.array(y[:, i]) for i in range(len(iv_variables))
+        }
         self._variables = dv_variables
 
-    def fit(self, X: np.ndarray, y: np.ndarray, epochs=1000,
-            fitter=scipy_curve_fit, metric=mean_squared_error, accept=less_than,
-            verbose=False):
+    def fit(
+        self,
+        X: np.ndarray,
+        y: np.ndarray,
+        epochs=1000,
+        fitter=scipy_curve_fit,
+        metric=mean_squared_error,
+        accept=less_than,
+        verbose=False,
+    ):
         self.load_data(X, y)
         y_pred = self.predict(X)
         self._error = metric(y, y_pred)
         for _ in tqdm(range(epochs)):
             self.fit_step(X=X, y=y, fitter=fitter, metric=metric, accept=accept)
             self._history.append(str(self.model_))
             self._trace.append(self._error)
         if verbose:
-            print(f'best model: {self.model_}\nError: {self._error}')
+            print(f"best model: {self.model_}\nError: {self._error}")
         return self
 
     @regression_handler
-    def fit_step(self, X: np.ndarray, y: np.ndarray, move=None,
-                 fitter=scipy_curve_fit, metric=mean_squared_error, accept=less_than,
-                 *args, **kwargs):
+    def fit_step(
+        self,
+        X: np.ndarray,
+        y: np.ndarray,
+        move=None,
+        fitter=scipy_curve_fit,
+        metric=mean_squared_error,
+        accept=less_than,
+        *args,
+        **kwargs,
+    ):
         self.load_data(X, y)
         self.step(move=move)
         if not self.visited():
             self.optimize_parameters(X, y, fitter)
+            self._record_visit()
             y_pred = self.predict(X)
             error = metric(y, y_pred, *args, **kwargs)
-            self._record_visit()
             if accept(error, self._error):
                 self._error = error
             else:
                 self.back_step()
         else:
             self.back_step()
 
@@ -101,39 +133,39 @@
             plt.show()
         try:
             y_pred = self._expression(Xs)
             if isinstance(y_pred, float):
                 y_pred = np.ones(X.shape[0]) * y_pred
             return y_pred
         except NameError:
-            raise NameError(f'Why is this caused again?\n{self.model_}')
+            raise NameError(f"Why is this caused again?\n{self.model_}")
 
     def get_expression(self):
         return self._expression
 
-    def step(self, move='', path=1):
+    def step(self, move="", path=1):
         self.cache()
         moves = []
         for steps in range(path):
             if move not in self._moves:
                 move = random.choice(self._moves)
-            if move == 'Root/None':
+            if move == "Root/None":
                 self.remove_root()
-            elif move == 'None/Root':
+            elif move == "None/Root":
                 self.add_root()
-            elif move == 'Node/Node':
+            elif move == "Node/Node":
                 self.replace_node()
-            elif move == 'Node/Leaf':
+            elif move == "Node/Leaf":
                 self.replace_node_with_leaf()
-            elif move == 'Leaf/Node':
+            elif move == "Leaf/Node":
                 self.replace_leaf_with_node()
-            elif move == 'Leaf/Leaf':
+            elif move == "Leaf/Leaf":
                 self.replace_leaf()
             else:
-                raise KeyError('Unknown move type')
+                raise KeyError("Unknown move type")
             moves.append(move)
         self._compile()
         return moves
 
     def optimize_parameters(self, X, y, fitter):
         if len(self.model_.get_parameters()) > 0:
             fitted_parameters = fitter(X, y, self.get_expression())
@@ -153,34 +185,40 @@
     def remove_root(self):
         if self.model_.get_root().has_children():
             new_root = random.choice(self.model_.get_root().get_children())
             new_root._parent = None
             self.model_._root = new_root
 
     def add_root(self):
-        new_root = self.make_node(random.choice(list(set(self.order(node) for node in self._primitives))))
+        new_root = self.make_node(
+            random.choice(list(set(self.order(node) for node in self._primitives)))
+        )
         old_root = self.model_.get_root()
         self.model_._root = new_root
         if self.model_.get_root().has_children():
             self.replace(random.choice(self.model_.get_root().get_children()), old_root)
 
     def replace_node(self):
         nodes = [node for node in self.model_.get_all_nodes() if node.has_children()]
         if not self.model_.get_root().has_children():
             nodes.append(self.model_.get_root())
         node = random.choice(list(node for node in nodes))
         self.replace(node)
 
     def replace_node_with_leaf(self):
-        nodes = [node for node in self.model_.get_all_nodes() if not node.has_children()]
+        nodes = [
+            node for node in self.model_.get_all_nodes() if not node.has_children()
+        ]
         node = random.choice(list(node for node in nodes))
         self.replace(node)
 
     def replace_leaf(self):
-        leaves = [node for node in self.model_.get_all_nodes() if not node.has_children()]
+        leaves = [
+            node for node in self.model_.get_all_nodes() if not node.has_children()
+        ]
         node = random.choice(list(node for node in leaves))
         self.replace(node)
 
     def replace_leaf_with_node(self):
         leaves = [node for node in self.model_.get_all_nodes() if node.has_children()]
         if not self.model_.get_root().has_children():
             leaves.append(self.model_.get_root())
@@ -198,67 +236,79 @@
         if order == 0:
             node_types = [Parameter()]
             # If there are variables (i.e. always except during __init__) add variables
             if len(self._variables) > 0:
                 node_types += [Variable(value=random.choice(list(self.DVs.keys())))]
         else:
             node_types = [Operator(value=random.choice(filtered_primitives))]
-        # assert len(weights) == len(node_types), 'number of weights must correspond to number of node types'
         return random.choices(node_types, k=1)[0]
 
     def _complete(self, depth=0):
         while not self.model_.is_filled():
             for node in self.model_.get_uninitialized():
                 new_node = self.make_node(order=depth)
                 self.model_.replace(node, new_node)
             depth -= 1
         self._compile()
 
     def _compile(self, x_type=tuple):
         self.model_.catalog()
         str_repr = self._sub_in_x(self.model_.__repr__(), x_type=x_type)
-        func_str = 'def func(X,' + ','.join(
-            [item[0] + '=' + str(item[1]) for item in self.model_.get_parameter_dict().items()]) + '): '
-        func_str += 'return ' + str_repr
-        namespace = {str(parameter): parameter.get_value() for parameter in self.model_.get_parameters()}
-        exec(func_str, {'np': np}, namespace)
-        self._expression = namespace['func']
-        return 'func', namespace
+        func_str = (
+            "def func(X,"
+            + ",".join(
+                [
+                    item[0] + "=" + str(item[1])
+                    for item in self.model_.get_parameter_dict().items()
+                ]
+            )
+            + "): "
+        )
+        func_str += "return " + str_repr
+        namespace = {
+            str(parameter): parameter.get_value()
+            for parameter in self.model_.get_parameters()
+        }
+        exec(func_str, {"np": np, "scipy": scipy}, namespace)
+        self._expression = namespace["func"]
+        return "func", namespace
 
     def visited(self):
         return canonical(str(self.model_)) in self._visit_list
 
     def get_parameters(self):
         return self.model_.get_parameters()
 
     def _record_visit(self):
         self._visit_list.add(canonical(str(self.model_)))
 
     def _filter_primitives(self, order):
-        return [primitive for primitive in self._primitives
-                if len(signature(primitive).parameters)
-                == order]
+        return [
+            primitive
+            for primitive in self._primitives
+            if len(signature(primitive).parameters) == order
+        ]
 
     @staticmethod
     def order(node):
         return len(signature(node).parameters)
 
     @staticmethod
     def _sub_in_x(str_repr, x_type=tuple):
-        while '_x' in str_repr:
-            start = str_repr.index('_x')
-            stop = str_repr.index('_', start + 1)
-            num = str_repr[start + 2:stop]
+        while "_x" in str_repr:
+            start = str_repr.index("_x")
+            stop = str_repr.index("_", start + 1)
+            num = str_repr[start + 2 : stop]
             if x_type is tuple:
-                str_repr = str_repr[:start] + 'X[' + num + ']' + str_repr[stop + 1:]
+                str_repr = str_repr[:start] + "X[" + num + "]" + str_repr[stop + 1 :]
             elif x_type is np.ndarray:
-                str_repr = str_repr[:start] + 'X[,:' + num + ']' + str_repr[stop + 1:]
+                str_repr = str_repr[:start] + "X[,:" + num + "]" + str_repr[stop + 1 :]
             else:
-                raise ValueError('Invalid data-type for X-variable')
+                raise ValueError("Invalid data-type for X-variable")
         return str_repr
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     model = SymbolicRegressor()
     for _ in range(30):
         model.step()
     print(model.model_)
```

### Comparing `autora-theorist-toolkit-0.1.6/src/autora/theorist/toolkit/models/tree.py` & `autora-theorist-toolkit-0.2.0/src/autora/theorist/toolkit/models/tree.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-from autora.theorist.toolkit.components.nodes import Symbol, Parameter
 from typing import List
 
+from autora.theorist.toolkit.components.nodes import Parameter, Symbol
+
 
 ###
 # Tree(Model)
 ###
 # attributes:
 #   root: Node object
 #   value: function object with arguments for x and parameters
@@ -12,15 +13,14 @@
 #
 # methods:
 # fit: calls the object-free fit function above and then updates its parameters
 # predict: sklearn format for predict
 # __call__: calls the object-oriented predict method above
 #
 class Tree:
-
     def __init__(self):
         super().__init__()
         self._root: Symbol = Symbol()
         self._nodes: List[Symbol] = []
         self._leaves: List[Symbol] = []
         self._parameters: List[Parameter] = []
         self._parameter_dict: dict[str, float] = {}
@@ -74,15 +74,15 @@
             for node in old_node.get_children():
                 self.fill(node, new_node)
         else:
             self.replace(old_node, new_node)
 
     # replace old node with new node
     def replace(self, old_node: Symbol, new_node: Symbol, **kwargs):
-        if 'NR' in kwargs:
+        if "NR" in kwargs:
             assert len(old_node.get_children()) == len(new_node.get_children())
             for i, child in enumerate(old_node.get_children()):
                 child.replace_parent(new_node)
                 new_node.replace_child(old=new_node[i], new=child)
         else:
             if old_node.has_parent():
                 old_node.get_parent().replace_child(old_node, new_node)
@@ -105,23 +105,23 @@
             else:
                 self._root = node
             if isinstance(node, Parameter):
                 self._parameters.append(node)
                 self._label_parameter(node)
 
     def size(self):
-        return len(set([self._root]+self._nodes+self._leaves))
+        return len(set([self._root] + self._nodes + self._leaves))
 
     # reset node lists
     def _clear(self):
         self._root = None
         self._nodes = []
         self._leaves = []
         self._parameters = []
         self._parameter_dict = {}
 
     def _label_parameter(self, node: Parameter):
         digit_label = 0
-        while '__a'+str(digit_label)+'__' in self._parameter_dict.keys():
+        while "__a" + str(digit_label) + "__" in self._parameter_dict.keys():
             digit_label += 1
-        node.label('__a'+str(digit_label)+'__')
+        node.label("__a" + str(digit_label) + "__")
         self._parameter_dict.update({str(node): node.get_value()})
```

### Comparing `autora-theorist-toolkit-0.1.6/src/autora/theorist/toolkit/utils.py` & `autora-theorist-toolkit-0.2.0/src/autora/theorist/toolkit/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,25 +13,24 @@
 #     parsed_expr = []
 
 
 ###
 # decision_sample
 ###
 # takes: takes a list of lists of floats corresponding to weights for choices
-# gives: list of integers, with each integer corresponding to the index chosen for each list of floats given
+# gives: list of integers, with each integer...
+# corresponding to the index chosen for each list of floats given
 def decision_sample(search_space):
     sample = []
     for options in search_space:
         sample.append(random.choices(range(len(options)), weights=options, k=1))
     return sample
 
 
 ###
 # (hamiltonian) mcmc sample
 ###
-# takes: model, search space with markov chain weights, number of hamiltonian steps (probability for bernoulli dist)
+# takes: model, search space with markov chain weights,
+# ... number of hamiltonian steps (probability for bernoulli dist)
 # gives: new model
 # def mcmc_sample():
 #    ...
-
-
-
```

### Comparing `autora-theorist-toolkit-0.1.6/src/autora_theorist_toolkit.egg-info/PKG-INFO` & `autora-theorist-toolkit-0.2.0/src/autora_theorist_toolkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autora-theorist-toolkit
-Version: 0.1.6
+Version: 0.2.0
 Summary: Toolkit to build algorithms for model recovery
 Author-email: "Joshua T. S. Hewson" <joshua_hewson@brown.edu>
 License: MIT license
 Project-URL: homepage, http://www.empiricalresearch.ai
 Project-URL: repository, https://github.com/TheLemonPig/autora-theorist-toolkit
 Project-URL: documentation, https://autoresearch.github.io/autora/
 Requires-Python: <4,>=3.8
```

### Comparing `autora-theorist-toolkit-0.1.6/src/autora_theorist_toolkit.egg-info/SOURCES.txt` & `autora-theorist-toolkit-0.2.0/src/autora_theorist_toolkit.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -30,19 +30,24 @@
 src/autora/theorist/toolkit/methods/fitting.py
 src/autora/theorist/toolkit/methods/metrics.py
 src/autora/theorist/toolkit/methods/regression.py
 src/autora/theorist/toolkit/methods/rules.py
 src/autora/theorist/toolkit/models/__init__.py
 src/autora/theorist/toolkit/models/bayesian_machine_scientist.py
 src/autora/theorist/toolkit/models/bayesian_symbolic_regression.py
+src/autora/theorist/toolkit/models/ddm_bms.py
+src/autora/theorist/toolkit/models/hierarchical_bayesian_symbolic_regression.py
+src/autora/theorist/toolkit/models/hierarchical_symbolic_regressor.py
+src/autora/theorist/toolkit/models/hybrid_regression.py
 src/autora/theorist/toolkit/models/memory.py
 src/autora/theorist/toolkit/models/parallel_symbolic_regression.py
 src/autora/theorist/toolkit/models/symbolic_regression.py
 src/autora/theorist/toolkit/models/tree.py
 src/autora_theorist_toolkit.egg-info/PKG-INFO
 src/autora_theorist_toolkit.egg-info/SOURCES.txt
 src/autora_theorist_toolkit.egg-info/dependency_links.txt
 src/autora_theorist_toolkit.egg-info/requires.txt
 src/autora_theorist_toolkit.egg-info/top_level.txt
 tests/README.md
 tests/__init__.py
-tests/test_toolkit.py
+tests/test_toolkit.py
+tests/test_visual.py
```

### Comparing `autora-theorist-toolkit-0.1.6/tests/README.md` & `autora-theorist-toolkit-0.2.0/tests/README.md`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.1.6/tests/test_toolkit.py` & `autora-theorist-toolkit-0.2.0/tests/test_toolkit.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,46 +1,57 @@
-from src.autora.theorist.toolkit.models.symbolic_regression import SymbolicRegressor
-from src.autora.theorist.toolkit.models.parallel_symbolic_regression import ParallelSymbolicRegressor
-from src.autora.theorist.toolkit.models.bayesian_symbolic_regression import BayesianSymbolicRegressor
-from src.autora.theorist.toolkit.models.bayesian_machine_scientist import BayesianMachineScientist
-from src.autora.theorist.toolkit.models.tree import Tree
-from src.autora.theorist.toolkit.models.memory import Stack
 import numpy as np
 
+from autora.theorist.toolkit.models.bayesian_machine_scientist import (
+    BayesianMachineScientist,
+)
+from autora.theorist.toolkit.models.bayesian_symbolic_regression import (
+    BayesianSymbolicRegressor,
+)
+from autora.theorist.toolkit.models.memory import Stack
+from autora.theorist.toolkit.models.parallel_symbolic_regression import (
+    ParallelSymbolicRegressor,
+)
+from autora.theorist.toolkit.models.symbolic_regression import SymbolicRegressor
+from autora.theorist.toolkit.models.tree import Tree
+
 
 def test_symbolic_regression_initialization():
     theorist = SymbolicRegressor()
     assert theorist is not None
     assert isinstance(theorist.model_, Tree)
     assert isinstance(theorist._cache, Stack)
-    assert str(theorist) == '__a0__'
+    assert str(theorist) == "__a0__"
     assert isinstance(theorist.predict(np.ones((100, 1))), np.ndarray)
 
 
 def test_bayesian_symbolic_regression_initialization():
-    prior_dict_ = {'+': 1.0}
+    prior_dict_ = {"+": 1.0}
     theorist = BayesianSymbolicRegressor(prior_dict=prior_dict_)
     assert theorist is not None
     assert isinstance(theorist.model_, Tree)
     assert isinstance(theorist._cache, Stack)
-    assert str(theorist) == '__a0__'
+    assert str(theorist) == "__a0__"
     assert isinstance(theorist.predict(np.ones((100, 1))), np.ndarray)
 
 
 def test_parallel_symbolic_regression_initialization():
-    prior_dict_ = {'+': 1.0}
-    temperatures_ = [1.04 ** t for t in range(20)]
-    theorist = ParallelSymbolicRegressor(temperatures=temperatures_, prior_dict=prior_dict_)
+    prior_dict_ = {"+": 1.0}
+    temperatures_ = [1.04**t for t in range(20)]
+    theorist = ParallelSymbolicRegressor(
+        temperatures=temperatures_, prior_dict=prior_dict_
+    )
     assert theorist is not None
 
 
 def test_bayesian_machine_scientist_initialization():
-    prior_dict_ = {'+': 1.0}
-    temperatures_ = [1.04 ** t for t in range(20)]
-    theorist = BayesianMachineScientist(temperatures=temperatures_, prior_dict=prior_dict_)
+    prior_dict_ = {"+": 1.0}
+    temperatures_ = [1.04**t for t in range(20)]
+    theorist = BayesianMachineScientist(
+        temperatures=temperatures_, prior_dict=prior_dict_
+    )
     assert theorist is not None
 
 
 if __name__ == "__main__":
     test_symbolic_regression_initialization()
     test_bayesian_symbolic_regression_initialization()
     test_parallel_symbolic_regression_initialization()
```

