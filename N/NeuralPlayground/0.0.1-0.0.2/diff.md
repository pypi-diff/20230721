# Comparing `tmp/NeuralPlayground-0.0.1.tar.gz` & `tmp/NeuralPlayground-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NeuralPlayground-0.0.1.tar", last modified: Fri Jul 21 10:21:48 2023, max compression
+gzip compressed data, was "NeuralPlayground-0.0.2.tar", last modified: Fri Jul 21 13:09:28 2023, max compression
```

## Comparing `NeuralPlayground-0.0.1.tar` & `NeuralPlayground-0.0.2.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 nsirmpilatze   (501) staff       (20)        0 2023-07-21 10:21:48.683923 NeuralPlayground-0.0.1/
--rw-r--r--   0 nsirmpilatze   (501) staff       (20)     2276 2023-07-13 09:41:39.000000 NeuralPlayground-0.0.1/.all-contributorsrc
-drwxr-xr-x   0 nsirmpilatze   (501) staff       (20)        0 2023-07-21 10:21:48.657013 NeuralPlayground-0.0.1/.github/
-drwxr-xr-x   0 nsirmpilatze   (501) staff       (20)        0 2023-07-21 10:21:48.663847 NeuralPlayground-0.0.1/.github/workflows/
--rw-r--r--   0 nsirmpilatze   (501) staff       (20)     1392 2023-06-01 14:51:08.000000 NeuralPlayground-0.0.1/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 nsirmpilatze   (501) staff       (20)      564 2023-06-01 14:51:08.000000 NeuralPlayground-0.0.1/.gitignore
--rw-r--r--   0 nsirmpilatze   (501) staff       (20)      687 2023-06-01 14:51:08.000000 NeuralPlayground-0.0.1/.pre-commit-config.yaml
--rw-r--r--   0 nsirmpilatze   (501) staff       (20)     1109 2023-06-01 14:51:08.000000 NeuralPlayground-0.0.1/LICENSE
--rw-r--r--   0 nsirmpilatze   (501) staff       (20)      234 2023-07-21 10:20:37.000000 NeuralPlayground-0.0.1/MANIFEST.in
-drwxr-xr-x   0 nsirmpilatze   (501) staff       (20)        0 2023-07-21 10:21:48.666004 NeuralPlayground-0.0.1/NeuralPlayground.egg-info/
--rw-r--r--   0 nsirmpilatze   (501) staff       (20)    13156 2023-07-21 10:21:48.000000 NeuralPlayground-0.0.1/NeuralPlayground.egg-info/PKG-INFO
--rw-r--r--   0 nsirmpilatze   (501) staff       (20)     1476 2023-07-21 10:21:48.000000 NeuralPlayground-0.0.1/NeuralPlayground.egg-info/SOURCES.txt
--rw-r--r--   0 nsirmpilatze   (501) staff       (20)        1 2023-07-21 10:21:48.000000 NeuralPlayground-0.0.1/NeuralPlayground.egg-info/dependency_links.txt
--rw-r--r--   0 nsirmpilatze   (501) staff       (20)      164 2023-07-21 10:21:48.000000 NeuralPlayground-0.0.1/NeuralPlayground.egg-info/requires.txt
--rw-r--r--   0 nsirmpilatze   (501) staff       (20)       17 2023-07-21 10:21:48.000000 NeuralPlayground-0.0.1/NeuralPlayground.egg-info/top_level.txt
--rw-r--r--   0 nsirmpilatze   (501) staff       (20)    13156 2023-07-21 10:21:48.683634 NeuralPlayground-0.0.1/PKG-INFO
--rw-r--r--   0 nsirmpilatze   (501) staff       (20)    11946 2023-07-13 09:41:39.000000 NeuralPlayground-0.0.1/README.md
-drwxr-xr-x   0 nsirmpilatze   (501) staff       (20)        0 2023-07-21 10:21:48.670999 NeuralPlayground-0.0.1/documents/
--rw-r--r--   0 nsirmpilatze   (501) staff       (20)      136 2023-06-01 14:51:08.000000 NeuralPlayground-0.0.1/documents/README.md
--rw-r--r--   0 nsirmpilatze   (501) staff       (20)      971 2023-06-01 14:51:08.000000 NeuralPlayground-0.0.1/documents/citation.cff
--rw-r--r--   0 nsirmpilatze   (501) staff       (20)     9275 2023-06-01 14:51:08.000000 NeuralPlayground-0.0.1/documents/code_of_conduct.md
--rw-r--r--   0 nsirmpilatze   (501) staff       (20)     2125 2023-06-01 14:51:08.000000 NeuralPlayground-0.0.1/documents/contributors.md
--rw-r--r--   0 nsirmpilatze   (501) staff       (20)     3642 2023-06-01 14:51:08.000000 NeuralPlayground-0.0.1/documents/licence.md
--rw-r--r--   0 nsirmpilatze   (501) staff       (20)     2357 2023-06-01 14:51:08.000000 NeuralPlayground-0.0.1/documents/road_map.md
--rw-r--r--   0 nsirmpilatze   (501) staff       (20)      611 2023-06-01 14:51:08.000000 NeuralPlayground-0.0.1/documents/style_guide.md
-drwxr-xr-x   0 nsirmpilatze   (501) staff       (20)        0 2023-07-21 10:21:48.672829 NeuralPlayground-0.0.1/neuralplayground/
--rw-r--r--   0 nsirmpilatze   (501) staff       (20)      185 2023-06-01 14:51:08.000000 NeuralPlayground-0.0.1/neuralplayground/README.md
--rw-r--r--   0 nsirmpilatze   (501) staff       (20)       26 2023-06-01 14:51:08.000000 NeuralPlayground-0.0.1/neuralplayground/__init__.py
-drwxr-xr-x   0 nsirmpilatze   (501) staff       (20)        0 2023-07-21 10:21:48.675965 NeuralPlayground-0.0.1/neuralplayground/agents/
--rw-r--r--   0 nsirmpilatze   (501) staff       (20)     2651 2023-06-01 14:51:08.000000 NeuralPlayground-0.0.1/neuralplayground/agents/README.md
--rw-r--r--   0 nsirmpilatze   (501) staff       (20)      160 2023-06-01 14:51:08.000000 NeuralPlayground-0.0.1/neuralplayground/agents/__init__.py
--rw-r--r--   0 nsirmpilatze   (501) staff       (20)     8167 2023-06-01 14:51:08.000000 NeuralPlayground-0.0.1/neuralplayground/agents/agent_core.py
--rw-r--r--   0 nsirmpilatze   (501) staff       (20)    16662 2023-06-01 14:51:08.000000 NeuralPlayground-0.0.1/neuralplayground/agents/stachenfeld_2018.py
--rw-r--r--   0 nsirmpilatze   (501) staff       (20)    17934 2023-06-01 14:51:08.000000 NeuralPlayground-0.0.1/neuralplayground/agents/weber_2018.py
-drwxr-xr-x   0 nsirmpilatze   (501) staff       (20)        0 2023-07-21 10:21:48.679419 NeuralPlayground-0.0.1/neuralplayground/arenas/
--rw-r--r--   0 nsirmpilatze   (501) staff       (20)     4027 2023-06-01 14:51:08.000000 NeuralPlayground-0.0.1/neuralplayground/arenas/README.md
--rw-r--r--   0 nsirmpilatze   (501) staff       (20)      276 2023-06-01 14:51:08.000000 NeuralPlayground-0.0.1/neuralplayground/arenas/__init__.py
--rw-r--r--   0 nsirmpilatze   (501) staff       (20)     7329 2023-06-01 14:51:08.000000 NeuralPlayground-0.0.1/neuralplayground/arenas/arena_core.py
--rw-r--r--   0 nsirmpilatze   (501) staff       (20)     2854 2023-06-01 14:51:08.000000 NeuralPlayground-0.0.1/neuralplayground/arenas/connected_rooms.py
--rw-r--r--   0 nsirmpilatze   (501) staff       (20)     9414 2023-07-13 09:41:39.000000 NeuralPlayground-0.0.1/neuralplayground/arenas/hafting_2008.py
--rw-r--r--   0 nsirmpilatze   (501) staff       (20)     3974 2023-06-01 14:51:08.000000 NeuralPlayground-0.0.1/neuralplayground/arenas/sargolini_2006.py
--rw-r--r--   0 nsirmpilatze   (501) staff       (20)    14509 2023-06-01 14:51:08.000000 NeuralPlayground-0.0.1/neuralplayground/arenas/simple2d.py
--rw-r--r--   0 nsirmpilatze   (501) staff       (20)    10034 2023-07-13 09:41:39.000000 NeuralPlayground-0.0.1/neuralplayground/arenas/wernle_2018.py
--rw-r--r--   0 nsirmpilatze   (501) staff       (20)     2103 2023-07-13 09:41:39.000000 NeuralPlayground-0.0.1/neuralplayground/datasets.py
-drwxr-xr-x   0 nsirmpilatze   (501) staff       (20)        0 2023-07-21 10:21:48.681523 NeuralPlayground-0.0.1/neuralplayground/experiments/
--rw-r--r--   0 nsirmpilatze   (501) staff       (20)     4514 2023-07-13 09:41:39.000000 NeuralPlayground-0.0.1/neuralplayground/experiments/README.md
--rw-r--r--   0 nsirmpilatze   (501) staff       (20)      208 2023-06-01 14:51:08.000000 NeuralPlayground-0.0.1/neuralplayground/experiments/__init__.py
--rw-r--r--   0 nsirmpilatze   (501) staff       (20)      107 2023-06-01 14:51:08.000000 NeuralPlayground-0.0.1/neuralplayground/experiments/experiment_core.py
--rw-r--r--   0 nsirmpilatze   (501) staff       (20)    22676 2023-07-13 09:41:39.000000 NeuralPlayground-0.0.1/neuralplayground/experiments/hafting_2008_data.py
--rw-r--r--   0 nsirmpilatze   (501) staff       (20)     9490 2023-07-13 09:41:39.000000 NeuralPlayground-0.0.1/neuralplayground/experiments/sargolini_2006_data.py
--rw-r--r--   0 nsirmpilatze   (501) staff       (20)    25566 2023-07-13 09:41:39.000000 NeuralPlayground-0.0.1/neuralplayground/experiments/wernle_2018_data.py
--rw-r--r--   0 nsirmpilatze   (501) staff       (20)    11834 2023-06-01 14:51:09.000000 NeuralPlayground-0.0.1/neuralplayground/utils.py
--rw-r--r--   0 nsirmpilatze   (501) staff       (20)     2252 2023-07-13 09:41:39.000000 NeuralPlayground-0.0.1/pyproject.toml
--rw-r--r--   0 nsirmpilatze   (501) staff       (20)       38 2023-07-21 10:21:48.683996 NeuralPlayground-0.0.1/setup.cfg
-drwxr-xr-x   0 nsirmpilatze   (501) staff       (20)        0 2023-07-21 10:21:48.683169 NeuralPlayground-0.0.1/tests/
--rw-r--r--   0 nsirmpilatze   (501) staff       (20)      825 2023-06-01 14:51:09.000000 NeuralPlayground-0.0.1/tests/README.md
--rw-r--r--   0 nsirmpilatze   (501) staff       (20)        0 2023-06-01 14:51:09.000000 NeuralPlayground-0.0.1/tests/__init__.py
--rw-r--r--   0 nsirmpilatze   (501) staff       (20)     4482 2023-06-01 14:51:09.000000 NeuralPlayground-0.0.1/tests/agent_test.py
--rw-r--r--   0 nsirmpilatze   (501) staff       (20)     4156 2023-06-01 14:51:09.000000 NeuralPlayground-0.0.1/tests/arena_exp_test.py
--rw-r--r--   0 nsirmpilatze   (501) staff       (20)      266 2023-06-01 14:51:09.000000 NeuralPlayground-0.0.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:09:28.793414 NeuralPlayground-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-07-21 13:09:19.000000 NeuralPlayground-0.0.2/.all-contributorsrc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:09:28.789414 NeuralPlayground-0.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:09:28.789414 NeuralPlayground-0.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-07-21 13:09:19.000000 NeuralPlayground-0.0.2/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-21 13:09:19.000000 NeuralPlayground-0.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-07-21 13:09:19.000000 NeuralPlayground-0.0.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-07-21 13:09:19.000000 NeuralPlayground-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-21 13:09:19.000000 NeuralPlayground-0.0.2/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:09:28.789414 NeuralPlayground-0.0.2/NeuralPlayground.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13583 2023-07-21 13:09:28.000000 NeuralPlayground-0.0.2/NeuralPlayground.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-07-21 13:09:28.000000 NeuralPlayground-0.0.2/NeuralPlayground.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 13:09:28.000000 NeuralPlayground-0.0.2/NeuralPlayground.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-21 13:09:28.000000 NeuralPlayground-0.0.2/NeuralPlayground.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-21 13:09:28.000000 NeuralPlayground-0.0.2/NeuralPlayground.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    13583 2023-07-21 13:09:28.793414 NeuralPlayground-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12373 2023-07-21 13:09:19.000000 NeuralPlayground-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:09:28.789414 NeuralPlayground-0.0.2/documents/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-21 13:09:19.000000 NeuralPlayground-0.0.2/documents/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-07-21 13:09:19.000000 NeuralPlayground-0.0.2/documents/citation.cff
+-rw-r--r--   0 runner    (1001) docker     (123)     9275 2023-07-21 13:09:19.000000 NeuralPlayground-0.0.2/documents/code_of_conduct.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-07-21 13:09:19.000000 NeuralPlayground-0.0.2/documents/contributors.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-07-21 13:09:19.000000 NeuralPlayground-0.0.2/documents/licence.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-07-21 13:09:19.000000 NeuralPlayground-0.0.2/documents/road_map.md
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-21 13:09:19.000000 NeuralPlayground-0.0.2/documents/style_guide.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:09:28.789414 NeuralPlayground-0.0.2/neuralplayground/
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-21 13:09:20.000000 NeuralPlayground-0.0.2/neuralplayground/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-21 13:09:20.000000 NeuralPlayground-0.0.2/neuralplayground/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:09:28.793414 NeuralPlayground-0.0.2/neuralplayground/agents/
+-rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-07-21 13:09:20.000000 NeuralPlayground-0.0.2/neuralplayground/agents/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-21 13:09:20.000000 NeuralPlayground-0.0.2/neuralplayground/agents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8167 2023-07-21 13:09:20.000000 NeuralPlayground-0.0.2/neuralplayground/agents/agent_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16662 2023-07-21 13:09:20.000000 NeuralPlayground-0.0.2/neuralplayground/agents/stachenfeld_2018.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17934 2023-07-21 13:09:20.000000 NeuralPlayground-0.0.2/neuralplayground/agents/weber_2018.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:09:28.793414 NeuralPlayground-0.0.2/neuralplayground/arenas/
+-rw-r--r--   0 runner    (1001) docker     (123)     4027 2023-07-21 13:09:20.000000 NeuralPlayground-0.0.2/neuralplayground/arenas/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-21 13:09:20.000000 NeuralPlayground-0.0.2/neuralplayground/arenas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7329 2023-07-21 13:09:20.000000 NeuralPlayground-0.0.2/neuralplayground/arenas/arena_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-07-21 13:09:20.000000 NeuralPlayground-0.0.2/neuralplayground/arenas/connected_rooms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9414 2023-07-21 13:09:20.000000 NeuralPlayground-0.0.2/neuralplayground/arenas/hafting_2008.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-07-21 13:09:20.000000 NeuralPlayground-0.0.2/neuralplayground/arenas/sargolini_2006.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14509 2023-07-21 13:09:20.000000 NeuralPlayground-0.0.2/neuralplayground/arenas/simple2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10034 2023-07-21 13:09:20.000000 NeuralPlayground-0.0.2/neuralplayground/arenas/wernle_2018.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-07-21 13:09:20.000000 NeuralPlayground-0.0.2/neuralplayground/datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:09:28.793414 NeuralPlayground-0.0.2/neuralplayground/experiments/
+-rw-r--r--   0 runner    (1001) docker     (123)     4514 2023-07-21 13:09:20.000000 NeuralPlayground-0.0.2/neuralplayground/experiments/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-21 13:09:20.000000 NeuralPlayground-0.0.2/neuralplayground/experiments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-21 13:09:20.000000 NeuralPlayground-0.0.2/neuralplayground/experiments/experiment_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22676 2023-07-21 13:09:20.000000 NeuralPlayground-0.0.2/neuralplayground/experiments/hafting_2008_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9490 2023-07-21 13:09:20.000000 NeuralPlayground-0.0.2/neuralplayground/experiments/sargolini_2006_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25566 2023-07-21 13:09:20.000000 NeuralPlayground-0.0.2/neuralplayground/experiments/wernle_2018_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11834 2023-07-21 13:09:20.000000 NeuralPlayground-0.0.2/neuralplayground/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-07-21 13:09:20.000000 NeuralPlayground-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 13:09:28.793414 NeuralPlayground-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:09:28.793414 NeuralPlayground-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-07-21 13:09:20.000000 NeuralPlayground-0.0.2/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 13:09:20.000000 NeuralPlayground-0.0.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-07-21 13:09:20.000000 NeuralPlayground-0.0.2/tests/agent_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-07-21 13:09:20.000000 NeuralPlayground-0.0.2/tests/arena_exp_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-21 13:09:20.000000 NeuralPlayground-0.0.2/tox.ini
```

### Comparing `NeuralPlayground-0.0.1/.all-contributorsrc` & `NeuralPlayground-0.0.2/.all-contributorsrc`

 * *Files identical despite different names*

### Comparing `NeuralPlayground-0.0.1/.github/workflows/test_and_deploy.yml` & `NeuralPlayground-0.0.2/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `NeuralPlayground-0.0.1/.pre-commit-config.yaml` & `NeuralPlayground-0.0.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `NeuralPlayground-0.0.1/LICENSE` & `NeuralPlayground-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `NeuralPlayground-0.0.1/NeuralPlayground.egg-info/PKG-INFO` & `NeuralPlayground-0.0.2/NeuralPlayground.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: NeuralPlayground
-Version: 0.0.1
+Version: 0.0.2
 Summary: The standardised environment for the hippocampus and entorhinal cortex models
 Author: Clementine Domine
 Author-email: Rodrigo Carrasco-Davis <rodrigo.carrasco.davis@gmail.com>
 License: MIT
-Project-URL: homepage, https://github.com/ClementineDomine/NeuralPlayground
-Project-URL: bug_tracker, https://github.com/ClementineDomine/NeuralPlayground/issues
-Project-URL: documentation, https://github.com/ClementineDomine/NeuralPlayground
-Project-URL: source_code, https://github.com/ClementineDomine/NeuralPlayground
-Project-URL: user_support, https://github.com/ClementineDomine/NeuralPlayground/issues
+Project-URL: Homepage, https://github.com/ClementineDomine/NeuralPlayground
+Project-URL: Bug tracker, https://github.com/ClementineDomine/NeuralPlayground/issues
+Project-URL: Documentation, https://github.com/ClementineDomine/NeuralPlayground
+Project-URL: Source code, https://github.com/ClementineDomine/NeuralPlayground
+Project-URL: User support, https://github.com/ClementineDomine/NeuralPlayground/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -59,32 +59,45 @@
 Altogether, we hope our framework, available at [github.com/NeuralPlayground](https://github.com/ClementineDomine/NeuralPlayground/), offers
 a foundation that the community will build upon, working toward a shared, standardized, open, and
 reproducible computational understanding of the hippocampus and entorhinal cortex.
 
 Try our short tutorial online in Colab. <a href="https://githubtocolab.com/SainsburyWellcomeCentre/NeuralPlayground/blob/main/examples/colab_example.ipynb" target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>
 
 ## 2. Installation
-You can create a new environment using conda, and the yml file with all the right
-dependencies by running
-```
-git clone https://github.com/SainsburyWellcomeCentre/NeuralPlayground/
-conda create --name NPG
-conda activate NPG
-conda install pip
-```
 
-For now, install using pip for local editing and testing
-```
-pip install -e .
+### Create a conda environment
+We advise you to install the package in a virtual environment,
+to avoid conflicts with other packages. For example, using `conda`:
+
+```python
+conda create --name NPG-env python=3.10
+conda activate NPG-env
 ```
-or
+### Pip install
+
+You can use `pip` get the latest release of NeuralPlayground from PyPI.
+```python
+# install the latest release
+pip install NeuralPlayground
+
+# upgrade to the latest release
+pip install -U NeuralPlayground
+
+# install a particular release
+pip install NeuralPlayground==0.0.1
 ```
+### Install for development
+
+If you want to contribute to the project, get the latest development version
+from GitHub, and install it in editable mode, including the "dev" dependencies:
+```bash
+git clone https://github.com/SainsburyWellcomeCentre/NeuralPlayground/
+cd NeuralPlayground
 pip install -e '.[dev]'
 ```
-if you want to install the dependencies for development.
 
 ## 3. Project
 
 Try our package! We are gathering opinions to focus our efforts on improving aspects of the code or adding new features, so if you tell us what you would like to have, we might just implement it ;) Please refer to the [Roadmap](https://github.com/ClementineDomine/NeuralPlayground/blob/main/documents/road_map.md) to understand the state of the project and get an idea of the direction it is going in. This open-source software was built to be collaborative and lasting. We hope that the framework will be simple enough to be adopted by a great number of neuroscientists, eventually guiding the path to the computational understanding of the HEC mechanisms. We follow reproducible, inclusive, and collaborative project design guidelines. All relevant documents can be found in [Documents](https://github.com/ClementineDomine/NeuralPlayground/blob/main/documents/).
 
 #### How to run a single module
```

### Comparing `NeuralPlayground-0.0.1/NeuralPlayground.egg-info/SOURCES.txt` & `NeuralPlayground-0.0.2/NeuralPlayground.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `NeuralPlayground-0.0.1/PKG-INFO` & `NeuralPlayground-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: NeuralPlayground
-Version: 0.0.1
+Version: 0.0.2
 Summary: The standardised environment for the hippocampus and entorhinal cortex models
 Author: Clementine Domine
 Author-email: Rodrigo Carrasco-Davis <rodrigo.carrasco.davis@gmail.com>
 License: MIT
-Project-URL: homepage, https://github.com/ClementineDomine/NeuralPlayground
-Project-URL: bug_tracker, https://github.com/ClementineDomine/NeuralPlayground/issues
-Project-URL: documentation, https://github.com/ClementineDomine/NeuralPlayground
-Project-URL: source_code, https://github.com/ClementineDomine/NeuralPlayground
-Project-URL: user_support, https://github.com/ClementineDomine/NeuralPlayground/issues
+Project-URL: Homepage, https://github.com/ClementineDomine/NeuralPlayground
+Project-URL: Bug tracker, https://github.com/ClementineDomine/NeuralPlayground/issues
+Project-URL: Documentation, https://github.com/ClementineDomine/NeuralPlayground
+Project-URL: Source code, https://github.com/ClementineDomine/NeuralPlayground
+Project-URL: User support, https://github.com/ClementineDomine/NeuralPlayground/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -59,32 +59,45 @@
 Altogether, we hope our framework, available at [github.com/NeuralPlayground](https://github.com/ClementineDomine/NeuralPlayground/), offers
 a foundation that the community will build upon, working toward a shared, standardized, open, and
 reproducible computational understanding of the hippocampus and entorhinal cortex.
 
 Try our short tutorial online in Colab. <a href="https://githubtocolab.com/SainsburyWellcomeCentre/NeuralPlayground/blob/main/examples/colab_example.ipynb" target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>
 
 ## 2. Installation
-You can create a new environment using conda, and the yml file with all the right
-dependencies by running
-```
-git clone https://github.com/SainsburyWellcomeCentre/NeuralPlayground/
-conda create --name NPG
-conda activate NPG
-conda install pip
-```
 
-For now, install using pip for local editing and testing
-```
-pip install -e .
+### Create a conda environment
+We advise you to install the package in a virtual environment,
+to avoid conflicts with other packages. For example, using `conda`:
+
+```python
+conda create --name NPG-env python=3.10
+conda activate NPG-env
 ```
-or
+### Pip install
+
+You can use `pip` get the latest release of NeuralPlayground from PyPI.
+```python
+# install the latest release
+pip install NeuralPlayground
+
+# upgrade to the latest release
+pip install -U NeuralPlayground
+
+# install a particular release
+pip install NeuralPlayground==0.0.1
 ```
+### Install for development
+
+If you want to contribute to the project, get the latest development version
+from GitHub, and install it in editable mode, including the "dev" dependencies:
+```bash
+git clone https://github.com/SainsburyWellcomeCentre/NeuralPlayground/
+cd NeuralPlayground
 pip install -e '.[dev]'
 ```
-if you want to install the dependencies for development.
 
 ## 3. Project
 
 Try our package! We are gathering opinions to focus our efforts on improving aspects of the code or adding new features, so if you tell us what you would like to have, we might just implement it ;) Please refer to the [Roadmap](https://github.com/ClementineDomine/NeuralPlayground/blob/main/documents/road_map.md) to understand the state of the project and get an idea of the direction it is going in. This open-source software was built to be collaborative and lasting. We hope that the framework will be simple enough to be adopted by a great number of neuroscientists, eventually guiding the path to the computational understanding of the HEC mechanisms. We follow reproducible, inclusive, and collaborative project design guidelines. All relevant documents can be found in [Documents](https://github.com/ClementineDomine/NeuralPlayground/blob/main/documents/).
 
 #### How to run a single module
```

### Comparing `NeuralPlayground-0.0.1/README.md` & `NeuralPlayground-0.0.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -33,32 +33,45 @@
 Altogether, we hope our framework, available at [github.com/NeuralPlayground](https://github.com/ClementineDomine/NeuralPlayground/), offers
 a foundation that the community will build upon, working toward a shared, standardized, open, and
 reproducible computational understanding of the hippocampus and entorhinal cortex.
 
 Try our short tutorial online in Colab. <a href="https://githubtocolab.com/SainsburyWellcomeCentre/NeuralPlayground/blob/main/examples/colab_example.ipynb" target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>
 
 ## 2. Installation
-You can create a new environment using conda, and the yml file with all the right
-dependencies by running
-```
-git clone https://github.com/SainsburyWellcomeCentre/NeuralPlayground/
-conda create --name NPG
-conda activate NPG
-conda install pip
-```
 
-For now, install using pip for local editing and testing
-```
-pip install -e .
+### Create a conda environment
+We advise you to install the package in a virtual environment,
+to avoid conflicts with other packages. For example, using `conda`:
+
+```python
+conda create --name NPG-env python=3.10
+conda activate NPG-env
 ```
-or
+### Pip install
+
+You can use `pip` get the latest release of NeuralPlayground from PyPI.
+```python
+# install the latest release
+pip install NeuralPlayground
+
+# upgrade to the latest release
+pip install -U NeuralPlayground
+
+# install a particular release
+pip install NeuralPlayground==0.0.1
 ```
+### Install for development
+
+If you want to contribute to the project, get the latest development version
+from GitHub, and install it in editable mode, including the "dev" dependencies:
+```bash
+git clone https://github.com/SainsburyWellcomeCentre/NeuralPlayground/
+cd NeuralPlayground
 pip install -e '.[dev]'
 ```
-if you want to install the dependencies for development.
 
 ## 3. Project
 
 Try our package! We are gathering opinions to focus our efforts on improving aspects of the code or adding new features, so if you tell us what you would like to have, we might just implement it ;) Please refer to the [Roadmap](https://github.com/ClementineDomine/NeuralPlayground/blob/main/documents/road_map.md) to understand the state of the project and get an idea of the direction it is going in. This open-source software was built to be collaborative and lasting. We hope that the framework will be simple enough to be adopted by a great number of neuroscientists, eventually guiding the path to the computational understanding of the HEC mechanisms. We follow reproducible, inclusive, and collaborative project design guidelines. All relevant documents can be found in [Documents](https://github.com/ClementineDomine/NeuralPlayground/blob/main/documents/).
 
 #### How to run a single module
```

#### html2text {}

```diff
@@ -36,24 +36,30 @@
 judgment of the quality of an Agent to replicate the brain mechanism. Instead,
 this only allows an objective and complete comparison to the current evidence
 in the field, as is typically done in publications. Altogether, we hope our
 framework, available at [github.com/NeuralPlayground](https://github.com/
 ClementineDomine/NeuralPlayground/), offers a foundation that the community
 will build upon, working toward a shared, standardized, open, and reproducible
 computational understanding of the hippocampus and entorhinal cortex. Try our
-short tutorial online in Colab. [Open_In_Colab] ## 2. Installation You can
-create a new environment using conda, and the yml file with all the right
-dependencies by running ``` git clone https://github.com/
-SainsburyWellcomeCentre/NeuralPlayground/ conda create --name NPG conda
-activate NPG conda install pip ``` For now, install using pip for local editing
-and testing ``` pip install -e . ``` or ``` pip install -e '.[dev]' ``` if you
-want to install the dependencies for development. ## 3. Project Try our
-package! We are gathering opinions to focus our efforts on improving aspects of
-the code or adding new features, so if you tell us what you would like to have,
-we might just implement it ;) Please refer to the [Roadmap](https://github.com/
+short tutorial online in Colab. [Open_In_Colab] ## 2. Installation ### Create a
+conda environment We advise you to install the package in a virtual
+environment, to avoid conflicts with other packages. For example, using
+`conda`: ```python conda create --name NPG-env python=3.10 conda activate NPG-
+env ``` ### Pip install You can use `pip` get the latest release of
+NeuralPlayground from PyPI. ```python # install the latest release pip install
+NeuralPlayground # upgrade to the latest release pip install -
+U NeuralPlayground # install a particular release pip install
+NeuralPlayground==0.0.1 ``` ### Install for development If you want to
+contribute to the project, get the latest development version from GitHub, and
+install it in editable mode, including the "dev" dependencies: ```bash git
+clone https://github.com/SainsburyWellcomeCentre/NeuralPlayground/ cd
+NeuralPlayground pip install -e '.[dev]' ``` ## 3. Project Try our package! We
+are gathering opinions to focus our efforts on improving aspects of the code or
+adding new features, so if you tell us what you would like to have, we might
+just implement it ;) Please refer to the [Roadmap](https://github.com/
 ClementineDomine/NeuralPlayground/blob/main/documents/road_map.md) to
 understand the state of the project and get an idea of the direction it is
 going in. This open-source software was built to be collaborative and lasting.
 We hope that the framework will be simple enough to be adopted by a great
 number of neuroscientists, eventually guiding the path to the computational
 understanding of the HEC mechanisms. We follow reproducible, inclusive, and
 collaborative project design guidelines. All relevant documents can be found in
```

### Comparing `NeuralPlayground-0.0.1/documents/citation.cff` & `NeuralPlayground-0.0.2/documents/citation.cff`

 * *Files identical despite different names*

### Comparing `NeuralPlayground-0.0.1/documents/code_of_conduct.md` & `NeuralPlayground-0.0.2/documents/code_of_conduct.md`

 * *Files identical despite different names*

### Comparing `NeuralPlayground-0.0.1/documents/contributors.md` & `NeuralPlayground-0.0.2/documents/contributors.md`

 * *Files identical despite different names*

### Comparing `NeuralPlayground-0.0.1/documents/licence.md` & `NeuralPlayground-0.0.2/documents/licence.md`

 * *Files identical despite different names*

### Comparing `NeuralPlayground-0.0.1/documents/road_map.md` & `NeuralPlayground-0.0.2/documents/road_map.md`

 * *Files identical despite different names*

### Comparing `NeuralPlayground-0.0.1/documents/style_guide.md` & `NeuralPlayground-0.0.2/documents/style_guide.md`

 * *Files identical despite different names*

### Comparing `NeuralPlayground-0.0.1/neuralplayground/agents/README.md` & `NeuralPlayground-0.0.2/neuralplayground/agents/README.md`

 * *Files identical despite different names*

### Comparing `NeuralPlayground-0.0.1/neuralplayground/agents/agent_core.py` & `NeuralPlayground-0.0.2/neuralplayground/agents/agent_core.py`

 * *Files identical despite different names*

### Comparing `NeuralPlayground-0.0.1/neuralplayground/agents/stachenfeld_2018.py` & `NeuralPlayground-0.0.2/neuralplayground/agents/stachenfeld_2018.py`

 * *Files identical despite different names*

### Comparing `NeuralPlayground-0.0.1/neuralplayground/agents/weber_2018.py` & `NeuralPlayground-0.0.2/neuralplayground/agents/weber_2018.py`

 * *Files identical despite different names*

### Comparing `NeuralPlayground-0.0.1/neuralplayground/arenas/README.md` & `NeuralPlayground-0.0.2/neuralplayground/arenas/README.md`

 * *Files identical despite different names*

### Comparing `NeuralPlayground-0.0.1/neuralplayground/arenas/arena_core.py` & `NeuralPlayground-0.0.2/neuralplayground/arenas/arena_core.py`

 * *Files identical despite different names*

### Comparing `NeuralPlayground-0.0.1/neuralplayground/arenas/connected_rooms.py` & `NeuralPlayground-0.0.2/neuralplayground/arenas/connected_rooms.py`

 * *Files identical despite different names*

### Comparing `NeuralPlayground-0.0.1/neuralplayground/arenas/hafting_2008.py` & `NeuralPlayground-0.0.2/neuralplayground/arenas/hafting_2008.py`

 * *Files identical despite different names*

### Comparing `NeuralPlayground-0.0.1/neuralplayground/arenas/sargolini_2006.py` & `NeuralPlayground-0.0.2/neuralplayground/arenas/sargolini_2006.py`

 * *Files identical despite different names*

### Comparing `NeuralPlayground-0.0.1/neuralplayground/arenas/simple2d.py` & `NeuralPlayground-0.0.2/neuralplayground/arenas/simple2d.py`

 * *Files identical despite different names*

### Comparing `NeuralPlayground-0.0.1/neuralplayground/arenas/wernle_2018.py` & `NeuralPlayground-0.0.2/neuralplayground/arenas/wernle_2018.py`

 * *Files identical despite different names*

### Comparing `NeuralPlayground-0.0.1/neuralplayground/datasets.py` & `NeuralPlayground-0.0.2/neuralplayground/datasets.py`

 * *Files identical despite different names*

### Comparing `NeuralPlayground-0.0.1/neuralplayground/experiments/README.md` & `NeuralPlayground-0.0.2/neuralplayground/experiments/README.md`

 * *Files identical despite different names*

### Comparing `NeuralPlayground-0.0.1/neuralplayground/experiments/hafting_2008_data.py` & `NeuralPlayground-0.0.2/neuralplayground/experiments/hafting_2008_data.py`

 * *Files identical despite different names*

### Comparing `NeuralPlayground-0.0.1/neuralplayground/experiments/sargolini_2006_data.py` & `NeuralPlayground-0.0.2/neuralplayground/experiments/sargolini_2006_data.py`

 * *Files identical despite different names*

### Comparing `NeuralPlayground-0.0.1/neuralplayground/experiments/wernle_2018_data.py` & `NeuralPlayground-0.0.2/neuralplayground/experiments/wernle_2018_data.py`

 * *Files identical despite different names*

### Comparing `NeuralPlayground-0.0.1/neuralplayground/utils.py` & `NeuralPlayground-0.0.2/neuralplayground/utils.py`

 * *Files identical despite different names*

### Comparing `NeuralPlayground-0.0.1/pyproject.toml` & `NeuralPlayground-0.0.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -33,19 +33,19 @@
   "deepdiff",
   "opencv-python",
   "gymnasium",
   "pooch",
 ]
 
 [project.urls]
-homepage = "https://github.com/ClementineDomine/NeuralPlayground"
-bug_tracker = "https://github.com/ClementineDomine/NeuralPlayground/issues"
-documentation = "https://github.com/ClementineDomine/NeuralPlayground"
-source_code = "https://github.com/ClementineDomine/NeuralPlayground"
-user_support = "https://github.com/ClementineDomine/NeuralPlayground/issues"
+"Homepage" = "https://github.com/ClementineDomine/NeuralPlayground"
+"Bug tracker" = "https://github.com/ClementineDomine/NeuralPlayground/issues"
+"Documentation" = "https://github.com/ClementineDomine/NeuralPlayground"
+"Source code" = "https://github.com/ClementineDomine/NeuralPlayground"
+"User support" = "https://github.com/ClementineDomine/NeuralPlayground/issues"
 
 [project.optional-dependencies]
 dev = [
   "pytest",
   "pytest-cov",
   "coverage",
   "tox",
```

### Comparing `NeuralPlayground-0.0.1/tests/README.md` & `NeuralPlayground-0.0.2/tests/README.md`

 * *Files identical despite different names*

### Comparing `NeuralPlayground-0.0.1/tests/agent_test.py` & `NeuralPlayground-0.0.2/tests/agent_test.py`

 * *Files identical despite different names*

### Comparing `NeuralPlayground-0.0.1/tests/arena_exp_test.py` & `NeuralPlayground-0.0.2/tests/arena_exp_test.py`

 * *Files identical despite different names*

