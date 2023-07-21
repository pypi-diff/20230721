# Comparing `tmp/corankco-7.0.0.tar.gz` & `tmp/corankco-7.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "corankco-7.0.0.tar", last modified: Thu Jul 20 07:46:42 2023, max compression
+gzip compressed data, was "corankco-7.0.1.tar", last modified: Fri Jul 21 08:17:57 2023, max compression
```

## Comparing `corankco-7.0.0.tar` & `corankco-7.0.1.tar`

### file list

```diff
@@ -1,128 +1,121 @@
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-07-20 07:46:42.864713 corankco-7.0.0/
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-07-20 07:46:42.852713 corankco-7.0.0/.github/
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-07-20 07:46:42.852713 corankco-7.0.0/.github/workflows/
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     1545 2023-07-09 21:49:42.000000 corankco-7.0.0/.github/workflows/python-package.yml
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     1789 2023-07-07 19:08:46.000000 corankco-7.0.0/.gitignore
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-07-20 07:46:42.852713 corankco-7.0.0/.idea/
--rw-rw-r--   0 pierre    (1000) pierre    (1000)      176 2021-09-08 13:22:17.000000 corankco-7.0.0/.idea/.gitignore
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     1369 2023-07-19 22:31:08.000000 corankco-7.0.0/.idea/corankco.iml
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-07-20 07:46:42.852713 corankco-7.0.0/.idea/dictionaries/
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     1004 2021-11-29 13:49:26.000000 corankco-7.0.0/.idea/dictionaries/pierre.xml
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-07-20 07:46:42.852713 corankco-7.0.0/.idea/inspectionProfiles/
--rw-rw-r--   0 pierre    (1000) pierre    (1000)      174 2021-09-08 13:23:29.000000 corankco-7.0.0/.idea/inspectionProfiles/profiles_settings.xml
--rw-rw-r--   0 pierre    (1000) pierre    (1000)      196 2021-09-08 13:23:51.000000 corankco-7.0.0/.idea/misc.xml
--rw-rw-r--   0 pierre    (1000) pierre    (1000)      268 2021-09-08 13:23:29.000000 corankco-7.0.0/.idea/modules.xml
--rw-rw-r--   0 pierre    (1000) pierre    (1000)      186 2021-11-27 09:49:32.000000 corankco-7.0.0/.idea/other.xml
--rw-rw-r--   0 pierre    (1000) pierre    (1000)      180 2021-09-08 13:23:29.000000 corankco-7.0.0/.idea/vcs.xml
--rw-rw-r--   0 pierre    (1000) pierre    (1000)      388 2023-07-09 01:51:24.000000 corankco-7.0.0/.idea/webResources.xml
--rw-rw-r--   0 pierre    (1000) pierre    (1000)      144 2023-07-18 14:58:34.000000 corankco-7.0.0/.readthedocs.yaml
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    18091 2023-07-08 21:25:07.000000 corankco-7.0.0/LICENSE
--rw-rw-r--   0 pierre    (1000) pierre    (1000)        0 2022-05-11 09:31:54.000000 corankco-7.0.0/MANIFEST.in
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     6355 2023-07-20 07:46:42.864713 corankco-7.0.0/PKG-INFO
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     5985 2023-07-20 07:40:02.000000 corankco-7.0.0/README.md
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-07-20 07:46:42.856713 corankco-7.0.0/corankco/
--rw-rw-r--   0 pierre    (1000) pierre    (1000)      515 2023-07-19 23:06:56.000000 corankco-7.0.0/corankco/__init__.py
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-07-20 07:46:42.856713 corankco-7.0.0/corankco/algorithms/
--rw-rw-r--   0 pierre    (1000) pierre    (1000)      523 2023-07-19 23:05:11.000000 corankco-7.0.0/corankco/algorithms/__init__.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     3262 2023-07-19 22:31:08.000000 corankco-7.0.0/corankco/algorithms/algorithm_choice.py
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-07-20 07:46:42.856713 corankco-7.0.0/corankco/algorithms/bioconsert/
--rw-rw-r--   0 pierre    (1000) pierre    (1000)      196 2023-07-19 22:35:38.000000 corankco-7.0.0/corankco/algorithms/bioconsert/__init__.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     1206 2023-07-19 22:31:08.000000 corankco-7.0.0/corankco/algorithms/bioconsert/bioco.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    12184 2023-07-19 22:31:08.000000 corankco-7.0.0/corankco/algorithms/bioconsert/bioconsert.py
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-07-20 07:46:42.856713 corankco-7.0.0/corankco/algorithms/borda/
--rw-rw-r--   0 pierre    (1000) pierre    (1000)      128 2023-07-19 22:43:16.000000 corankco-7.0.0/corankco/algorithms/borda/__init__.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     6817 2023-07-19 22:31:08.000000 corankco-7.0.0/corankco/algorithms/borda/borda.py
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-07-20 07:46:42.856713 corankco-7.0.0/corankco/algorithms/copeland/
--rw-rw-r--   0 pierre    (1000) pierre    (1000)      141 2023-07-19 22:43:16.000000 corankco-7.0.0/corankco/algorithms/copeland/__init__.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     6514 2023-07-19 22:31:08.000000 corankco-7.0.0/corankco/algorithms/copeland/copeland.py
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-07-20 07:46:42.856713 corankco-7.0.0/corankco/algorithms/exact/
--rw-rw-r--   0 pierre    (1000) pierre    (1000)      284 2023-07-19 22:31:34.000000 corankco-7.0.0/corankco/algorithms/exact/__init__.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     4376 2023-07-19 22:31:08.000000 corankco-7.0.0/corankco/algorithms/exact/exactalgorithm.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     2383 2023-07-19 22:31:08.000000 corankco-7.0.0/corankco/algorithms/exact/exactalgorithmbase.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    26179 2023-07-19 22:31:09.000000 corankco-7.0.0/corankco/algorithms/exact/exactalgorithmcplex.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     3899 2023-07-19 22:31:09.000000 corankco-7.0.0/corankco/algorithms/exact/exactalgorithmcplexforpaperoptim1.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    15601 2023-07-19 22:31:08.000000 corankco-7.0.0/corankco/algorithms/exact/exactalgorithmpulp.py
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-07-20 07:46:42.856713 corankco-7.0.0/corankco/algorithms/kwiksort/
--rw-rw-r--   0 pierre    (1000) pierre    (1000)      170 2023-07-19 22:43:16.000000 corankco-7.0.0/corankco/algorithms/kwiksort/__init__.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     7354 2023-07-19 22:31:08.000000 corankco-7.0.0/corankco/algorithms/kwiksort/kwiksortabs.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     5299 2023-07-19 22:31:08.000000 corankco-7.0.0/corankco/algorithms/kwiksort/kwiksortrandom.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    13583 2023-07-19 22:31:08.000000 corankco-7.0.0/corankco/algorithms/pairwisebasedalgorithm.py
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-07-20 07:46:42.856713 corankco-7.0.0/corankco/algorithms/parcons/
--rw-rw-r--   0 pierre    (1000) pierre    (1000)      126 2023-07-19 22:43:16.000000 corankco-7.0.0/corankco/algorithms/parcons/__init__.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     7375 2023-07-19 22:31:08.000000 corankco-7.0.0/corankco/algorithms/parcons/parcons.py
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-07-20 07:46:42.856713 corankco-7.0.0/corankco/algorithms/pickaperm/
--rw-rw-r--   0 pierre    (1000) pierre    (1000)      191 2023-07-19 22:44:52.000000 corankco-7.0.0/corankco/algorithms/pickaperm/__init__.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     5530 2023-07-19 22:31:08.000000 corankco-7.0.0/corankco/algorithms/pickaperm/pickaperm.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     4904 2023-07-19 22:31:08.000000 corankco-7.0.0/corankco/algorithms/rank_aggregation_algorithm.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    14330 2023-07-19 22:31:08.000000 corankco-7.0.0/corankco/consensus.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    24721 2023-07-19 22:31:09.000000 corankco-7.0.0/corankco/dataset.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     5067 2023-07-19 22:31:08.000000 corankco-7.0.0/corankco/element.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    13189 2023-07-19 22:31:08.000000 corankco-7.0.0/corankco/kemeny_score_computation.py
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-07-20 07:46:42.860713 corankco-7.0.0/corankco/partitioning/
--rw-rw-r--   0 pierre    (1000) pierre    (1000)      352 2023-07-19 22:43:16.000000 corankco-7.0.0/corankco/partitioning/__init__.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    11080 2023-07-19 23:44:24.000000 corankco-7.0.0/corankco/partitioning/ordered_partition.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    13738 2023-07-19 22:31:08.000000 corankco-7.0.0/corankco/ranking.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    16109 2023-07-19 22:31:08.000000 corankco-7.0.0/corankco/scoringscheme.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     5676 2023-07-19 22:31:08.000000 corankco-7.0.0/corankco/utils.py
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-07-20 07:46:42.856713 corankco-7.0.0/corankco.egg-info/
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     6355 2023-07-20 07:46:42.000000 corankco-7.0.0/corankco.egg-info/PKG-INFO
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     3169 2023-07-20 07:46:42.000000 corankco-7.0.0/corankco.egg-info/SOURCES.txt
--rw-rw-r--   0 pierre    (1000) pierre    (1000)        1 2023-07-20 07:46:42.000000 corankco-7.0.0/corankco.egg-info/dependency_links.txt
--rw-rw-r--   0 pierre    (1000) pierre    (1000)        1 2021-09-08 13:23:38.000000 corankco-7.0.0/corankco.egg-info/not-zip-safe
--rw-rw-r--   0 pierre    (1000) pierre    (1000)       78 2023-07-20 07:46:42.000000 corankco-7.0.0/corankco.egg-info/requires.txt
--rw-rw-r--   0 pierre    (1000) pierre    (1000)        9 2023-07-20 07:46:42.000000 corankco-7.0.0/corankco.egg-info/top_level.txt
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    21157 2023-07-20 07:35:15.000000 corankco-7.0.0/corankco_notebook.ipynb
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-07-20 07:46:42.860713 corankco-7.0.0/docs/
--rw-rw-r--   0 pierre    (1000) pierre    (1000)      638 2023-07-18 08:36:43.000000 corankco-7.0.0/docs/Makefile
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-07-20 07:46:42.852713 corankco-7.0.0/docs/build/
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-07-20 07:46:42.860713 corankco-7.0.0/docs/build/html/
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    35628 2023-07-18 15:17:21.000000 corankco-7.0.0/docs/build/html/consensus.html
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    55628 2023-07-18 15:17:21.000000 corankco-7.0.0/docs/build/html/dataset.html
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    14084 2023-07-18 15:17:21.000000 corankco-7.0.0/docs/build/html/element.html
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    24847 2023-07-18 15:17:21.000000 corankco-7.0.0/docs/build/html/genindex.html
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     8346 2023-07-18 15:17:21.000000 corankco-7.0.0/docs/build/html/index.html
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     5218 2023-07-18 15:17:21.000000 corankco-7.0.0/docs/build/html/py-modindex.html
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    23640 2023-07-18 15:17:21.000000 corankco-7.0.0/docs/build/html/ranking.html
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    40876 2023-07-18 15:17:21.000000 corankco-7.0.0/docs/build/html/scoring_scheme.html
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     4030 2023-07-18 15:17:21.000000 corankco-7.0.0/docs/build/html/search.html
--rw-rw-r--   0 pierre    (1000) pierre    (1000)      804 2023-07-18 08:36:43.000000 corankco-7.0.0/docs/make.bat
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-07-20 07:46:42.860713 corankco-7.0.0/docs/source/
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     1114 2023-07-19 22:31:08.000000 corankco-7.0.0/docs/source/conf.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)       79 2023-07-18 08:08:04.000000 corankco-7.0.0/docs/source/consensus.rst
--rw-rw-r--   0 pierre    (1000) pierre    (1000)      645 2023-07-20 07:10:24.000000 corankco-7.0.0/docs/source/corankco.algorithms.bioconsert.rst
--rw-rw-r--   0 pierre    (1000) pierre    (1000)      403 2023-07-20 07:10:24.000000 corankco-7.0.0/docs/source/corankco.algorithms.borda.rst
--rw-rw-r--   0 pierre    (1000) pierre    (1000)      430 2023-07-20 07:10:24.000000 corankco-7.0.0/docs/source/corankco.algorithms.copeland.rst
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     1362 2023-07-20 07:10:24.000000 corankco-7.0.0/docs/source/corankco.algorithms.exact.rst
--rw-rw-r--   0 pierre    (1000) pierre    (1000)      657 2023-07-20 07:10:24.000000 corankco-7.0.0/docs/source/corankco.algorithms.kwiksort.rst
--rw-rw-r--   0 pierre    (1000) pierre    (1000)      421 2023-07-20 07:10:24.000000 corankco-7.0.0/docs/source/corankco.algorithms.parcons.rst
--rw-rw-r--   0 pierre    (1000) pierre    (1000)      439 2023-07-20 07:10:24.000000 corankco-7.0.0/docs/source/corankco.algorithms.pickaperm.rst
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     1124 2023-07-20 07:10:24.000000 corankco-7.0.0/docs/source/corankco.algorithms.rst
--rw-rw-r--   0 pierre    (1000) pierre    (1000)      417 2023-07-20 07:10:24.000000 corankco-7.0.0/docs/source/corankco.partitioning.rst
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     1306 2023-07-20 07:10:24.000000 corankco-7.0.0/docs/source/corankco.rst
--rw-rw-r--   0 pierre    (1000) pierre    (1000)       75 2023-07-18 08:01:57.000000 corankco-7.0.0/docs/source/dataset.rst
--rw-rw-r--   0 pierre    (1000) pierre    (1000)       75 2023-07-18 08:07:40.000000 corankco-7.0.0/docs/source/element.rst
--rw-rw-r--   0 pierre    (1000) pierre    (1000)      503 2023-07-18 09:01:31.000000 corankco-7.0.0/docs/source/index.rst
--rw-rw-r--   0 pierre    (1000) pierre    (1000)       61 2023-07-20 07:10:24.000000 corankco-7.0.0/docs/source/modules.rst
--rw-rw-r--   0 pierre    (1000) pierre    (1000)       75 2023-07-09 00:54:24.000000 corankco-7.0.0/docs/source/ranking.rst
--rw-rw-r--   0 pierre    (1000) pierre    (1000)       88 2023-07-18 08:12:52.000000 corankco-7.0.0/docs/source/scoring_scheme.rst
--rw-rw-r--   0 pierre    (1000) pierre    (1000)      804 2023-07-01 08:05:34.000000 corankco-7.0.0/make.bat
--rw-rw-r--   0 pierre    (1000) pierre    (1000)       82 2023-07-20 07:23:22.000000 corankco-7.0.0/requirements.txt
--rw-rw-r--   0 pierre    (1000) pierre    (1000)       38 2023-07-20 07:46:42.864713 corankco-7.0.0/setup.cfg
--rw-rw-r--   0 pierre    (1000) pierre    (1000)      867 2023-07-20 07:46:07.000000 corankco-7.0.0/setup.py
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-07-20 07:46:42.864713 corankco-7.0.0/tests/
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-07-20 07:46:42.864713 corankco-7.0.0/tests/dataset_examples/
--rw-rw-r--   0 pierre    (1000) pierre    (1000)       93 2023-07-19 22:31:08.000000 corankco-7.0.0/tests/dataset_examples/dataset_example
--rw-rw-r--   0 pierre    (1000) pierre    (1000)       41 2023-07-19 22:31:08.000000 corankco-7.0.0/tests/dataset_examples/dataset_example_2
--rw-rw-r--   0 pierre    (1000) pierre    (1000)       44 2023-07-19 22:31:08.000000 corankco-7.0.0/tests/dataset_examples/dataset_example_3
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     3591 2023-07-20 07:26:30.000000 corankco-7.0.0/tests/exemple.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     2056 2023-07-19 22:31:08.000000 corankco-7.0.0/tests/test_BioCo.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     1764 2023-07-19 22:31:09.000000 corankco-7.0.0/tests/test_BioConsert.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     1652 2023-07-19 22:31:08.000000 corankco-7.0.0/tests/test_Borda.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     1874 2023-07-19 22:31:08.000000 corankco-7.0.0/tests/test_Copeland.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     2522 2023-07-07 19:08:46.000000 corankco-7.0.0/tests/test_Element.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     3320 2023-07-19 22:31:08.000000 corankco-7.0.0/tests/test_Ranking.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     3702 2023-07-19 22:31:08.000000 corankco-7.0.0/tests/test_ScoringScheme.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     4989 2023-07-19 22:31:08.000000 corankco-7.0.0/tests/test_dataset.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)      969 2023-07-19 22:31:08.000000 corankco-7.0.0/tests/test_exact_algorithms.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     6284 2023-07-19 22:31:08.000000 corankco-7.0.0/tests/test_kemenycomputation.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     4060 2023-07-19 22:51:32.000000 corankco-7.0.0/tests/test_median_ranking_algorithms.py
+drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-07-21 08:17:57.016008 corankco-7.0.1/
+drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-07-21 08:17:57.004008 corankco-7.0.1/.github/
+drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-07-21 08:17:57.008008 corankco-7.0.1/.github/workflows/
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     1545 2023-07-09 21:49:42.000000 corankco-7.0.1/.github/workflows/python-package.yml
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     1789 2023-07-07 19:08:46.000000 corankco-7.0.1/.gitignore
+drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-07-21 08:17:57.008008 corankco-7.0.1/.idea/
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)      176 2021-09-08 13:22:17.000000 corankco-7.0.1/.idea/.gitignore
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     1369 2023-07-19 22:31:08.000000 corankco-7.0.1/.idea/corankco.iml
+drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-07-21 08:17:57.008008 corankco-7.0.1/.idea/dictionaries/
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     1004 2021-11-29 13:49:26.000000 corankco-7.0.1/.idea/dictionaries/pierre.xml
+drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-07-21 08:17:57.008008 corankco-7.0.1/.idea/inspectionProfiles/
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)      174 2021-09-08 13:23:29.000000 corankco-7.0.1/.idea/inspectionProfiles/profiles_settings.xml
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)      196 2021-09-08 13:23:51.000000 corankco-7.0.1/.idea/misc.xml
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)      268 2021-09-08 13:23:29.000000 corankco-7.0.1/.idea/modules.xml
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)      186 2021-11-27 09:49:32.000000 corankco-7.0.1/.idea/other.xml
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)      180 2021-09-08 13:23:29.000000 corankco-7.0.1/.idea/vcs.xml
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)      388 2023-07-09 01:51:24.000000 corankco-7.0.1/.idea/webResources.xml
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)      144 2023-07-18 14:58:34.000000 corankco-7.0.1/.readthedocs.yaml
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    18091 2023-07-08 21:25:07.000000 corankco-7.0.1/LICENSE
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)        0 2022-05-11 09:31:54.000000 corankco-7.0.1/MANIFEST.in
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     6485 2023-07-21 08:17:57.016008 corankco-7.0.1/PKG-INFO
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     6115 2023-07-21 08:15:51.000000 corankco-7.0.1/README.md
+drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-07-21 08:17:57.008008 corankco-7.0.1/corankco/
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)      515 2023-07-19 23:06:56.000000 corankco-7.0.1/corankco/__init__.py
+drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-07-21 08:17:57.012009 corankco-7.0.1/corankco/algorithms/
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)      523 2023-07-19 23:05:11.000000 corankco-7.0.1/corankco/algorithms/__init__.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     3262 2023-07-19 22:31:08.000000 corankco-7.0.1/corankco/algorithms/algorithm_choice.py
+drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-07-21 08:17:57.012009 corankco-7.0.1/corankco/algorithms/bioconsert/
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)      196 2023-07-19 22:35:38.000000 corankco-7.0.1/corankco/algorithms/bioconsert/__init__.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     1206 2023-07-19 22:31:08.000000 corankco-7.0.1/corankco/algorithms/bioconsert/bioco.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    12184 2023-07-19 22:31:08.000000 corankco-7.0.1/corankco/algorithms/bioconsert/bioconsert.py
+drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-07-21 08:17:57.012009 corankco-7.0.1/corankco/algorithms/borda/
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)      128 2023-07-19 22:43:16.000000 corankco-7.0.1/corankco/algorithms/borda/__init__.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     6817 2023-07-19 22:31:08.000000 corankco-7.0.1/corankco/algorithms/borda/borda.py
+drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-07-21 08:17:57.012009 corankco-7.0.1/corankco/algorithms/copeland/
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)      141 2023-07-19 22:43:16.000000 corankco-7.0.1/corankco/algorithms/copeland/__init__.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     6514 2023-07-19 22:31:08.000000 corankco-7.0.1/corankco/algorithms/copeland/copeland.py
+drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-07-21 08:17:57.012009 corankco-7.0.1/corankco/algorithms/exact/
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)      284 2023-07-19 22:31:34.000000 corankco-7.0.1/corankco/algorithms/exact/__init__.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     4376 2023-07-19 22:31:08.000000 corankco-7.0.1/corankco/algorithms/exact/exactalgorithm.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     2383 2023-07-19 22:31:08.000000 corankco-7.0.1/corankco/algorithms/exact/exactalgorithmbase.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    26179 2023-07-19 22:31:09.000000 corankco-7.0.1/corankco/algorithms/exact/exactalgorithmcplex.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     3899 2023-07-19 22:31:09.000000 corankco-7.0.1/corankco/algorithms/exact/exactalgorithmcplexforpaperoptim1.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    15601 2023-07-19 22:31:08.000000 corankco-7.0.1/corankco/algorithms/exact/exactalgorithmpulp.py
+drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-07-21 08:17:57.012009 corankco-7.0.1/corankco/algorithms/kwiksort/
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)      170 2023-07-19 22:43:16.000000 corankco-7.0.1/corankco/algorithms/kwiksort/__init__.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     7354 2023-07-19 22:31:08.000000 corankco-7.0.1/corankco/algorithms/kwiksort/kwiksortabs.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     5299 2023-07-19 22:31:08.000000 corankco-7.0.1/corankco/algorithms/kwiksort/kwiksortrandom.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    13583 2023-07-19 22:31:08.000000 corankco-7.0.1/corankco/algorithms/pairwisebasedalgorithm.py
+drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-07-21 08:17:57.012009 corankco-7.0.1/corankco/algorithms/parcons/
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)      126 2023-07-19 22:43:16.000000 corankco-7.0.1/corankco/algorithms/parcons/__init__.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     7375 2023-07-19 22:31:08.000000 corankco-7.0.1/corankco/algorithms/parcons/parcons.py
+drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-07-21 08:17:57.012009 corankco-7.0.1/corankco/algorithms/pickaperm/
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)      191 2023-07-19 22:44:52.000000 corankco-7.0.1/corankco/algorithms/pickaperm/__init__.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     5530 2023-07-19 22:31:08.000000 corankco-7.0.1/corankco/algorithms/pickaperm/pickaperm.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     4904 2023-07-19 22:31:08.000000 corankco-7.0.1/corankco/algorithms/rank_aggregation_algorithm.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    14330 2023-07-19 22:31:08.000000 corankco-7.0.1/corankco/consensus.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    24721 2023-07-19 22:31:09.000000 corankco-7.0.1/corankco/dataset.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     5067 2023-07-19 22:31:08.000000 corankco-7.0.1/corankco/element.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    13189 2023-07-19 22:31:08.000000 corankco-7.0.1/corankco/kemeny_score_computation.py
+drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-07-21 08:17:57.012009 corankco-7.0.1/corankco/partitioning/
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)      352 2023-07-19 22:43:16.000000 corankco-7.0.1/corankco/partitioning/__init__.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    11080 2023-07-19 23:44:24.000000 corankco-7.0.1/corankco/partitioning/ordered_partition.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    13738 2023-07-19 22:31:08.000000 corankco-7.0.1/corankco/ranking.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    16109 2023-07-19 22:31:08.000000 corankco-7.0.1/corankco/scoringscheme.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     5676 2023-07-19 22:31:08.000000 corankco-7.0.1/corankco/utils.py
+drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-07-21 08:17:57.012009 corankco-7.0.1/corankco.egg-info/
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     6485 2023-07-21 08:17:56.000000 corankco-7.0.1/corankco.egg-info/PKG-INFO
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     2858 2023-07-21 08:17:56.000000 corankco-7.0.1/corankco.egg-info/SOURCES.txt
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)        1 2023-07-21 08:17:56.000000 corankco-7.0.1/corankco.egg-info/dependency_links.txt
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)        1 2021-09-08 13:23:38.000000 corankco-7.0.1/corankco.egg-info/not-zip-safe
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)       78 2023-07-21 08:17:56.000000 corankco-7.0.1/corankco.egg-info/requires.txt
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)        9 2023-07-21 08:17:56.000000 corankco-7.0.1/corankco.egg-info/top_level.txt
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    21157 2023-07-20 07:35:15.000000 corankco-7.0.1/corankco_notebook.ipynb
+drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-07-21 08:17:57.012009 corankco-7.0.1/docs/
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)      638 2023-07-18 08:36:43.000000 corankco-7.0.1/docs/Makefile
+drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-07-21 08:17:57.008008 corankco-7.0.1/docs/build/
+drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-07-21 08:17:57.016008 corankco-7.0.1/docs/build/html/
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    35628 2023-07-18 15:17:21.000000 corankco-7.0.1/docs/build/html/consensus.html
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    55628 2023-07-18 15:17:21.000000 corankco-7.0.1/docs/build/html/dataset.html
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    14084 2023-07-18 15:17:21.000000 corankco-7.0.1/docs/build/html/element.html
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    24847 2023-07-18 15:17:21.000000 corankco-7.0.1/docs/build/html/genindex.html
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     8346 2023-07-18 15:17:21.000000 corankco-7.0.1/docs/build/html/index.html
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     5218 2023-07-18 15:17:21.000000 corankco-7.0.1/docs/build/html/py-modindex.html
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    23640 2023-07-18 15:17:21.000000 corankco-7.0.1/docs/build/html/ranking.html
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    40876 2023-07-18 15:17:21.000000 corankco-7.0.1/docs/build/html/scoring_scheme.html
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     4030 2023-07-18 15:17:21.000000 corankco-7.0.1/docs/build/html/search.html
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)      804 2023-07-18 08:36:43.000000 corankco-7.0.1/docs/make.bat
+drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-07-21 08:17:57.016008 corankco-7.0.1/docs/source/
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     1114 2023-07-19 22:31:08.000000 corankco-7.0.1/docs/source/conf.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)       79 2023-07-18 08:08:04.000000 corankco-7.0.1/docs/source/consensus.rst
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     1124 2023-07-20 08:18:37.000000 corankco-7.0.1/docs/source/corankco.algorithms.rst
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)      417 2023-07-20 07:10:24.000000 corankco-7.0.1/docs/source/corankco.partitioning.rst
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     1306 2023-07-20 07:10:24.000000 corankco-7.0.1/docs/source/corankco.rst
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)       75 2023-07-18 08:01:57.000000 corankco-7.0.1/docs/source/dataset.rst
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)       75 2023-07-18 08:07:40.000000 corankco-7.0.1/docs/source/element.rst
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)      775 2023-07-20 08:10:47.000000 corankco-7.0.1/docs/source/index.rst
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)       61 2023-07-20 07:10:24.000000 corankco-7.0.1/docs/source/modules.rst
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)       75 2023-07-09 00:54:24.000000 corankco-7.0.1/docs/source/ranking.rst
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)       88 2023-07-18 08:12:52.000000 corankco-7.0.1/docs/source/scoring_scheme.rst
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)      804 2023-07-01 08:05:34.000000 corankco-7.0.1/make.bat
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)       82 2023-07-20 07:23:22.000000 corankco-7.0.1/requirements.txt
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)       38 2023-07-21 08:17:57.016008 corankco-7.0.1/setup.cfg
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)      867 2023-07-21 08:14:55.000000 corankco-7.0.1/setup.py
+drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-07-21 08:17:57.016008 corankco-7.0.1/tests/
+drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-07-21 08:17:57.016008 corankco-7.0.1/tests/dataset_examples/
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)       93 2023-07-19 22:31:08.000000 corankco-7.0.1/tests/dataset_examples/dataset_example
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)       41 2023-07-19 22:31:08.000000 corankco-7.0.1/tests/dataset_examples/dataset_example_2
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)       44 2023-07-19 22:31:08.000000 corankco-7.0.1/tests/dataset_examples/dataset_example_3
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     3591 2023-07-20 07:26:30.000000 corankco-7.0.1/tests/exemple.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     2056 2023-07-19 22:31:08.000000 corankco-7.0.1/tests/test_BioCo.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     1764 2023-07-19 22:31:09.000000 corankco-7.0.1/tests/test_BioConsert.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     1652 2023-07-19 22:31:08.000000 corankco-7.0.1/tests/test_Borda.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     1874 2023-07-19 22:31:08.000000 corankco-7.0.1/tests/test_Copeland.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     2522 2023-07-07 19:08:46.000000 corankco-7.0.1/tests/test_Element.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     3320 2023-07-19 22:31:08.000000 corankco-7.0.1/tests/test_Ranking.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     3702 2023-07-19 22:31:08.000000 corankco-7.0.1/tests/test_ScoringScheme.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     4989 2023-07-19 22:31:08.000000 corankco-7.0.1/tests/test_dataset.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)      969 2023-07-19 22:31:08.000000 corankco-7.0.1/tests/test_exact_algorithms.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     6284 2023-07-19 22:31:08.000000 corankco-7.0.1/tests/test_kemenycomputation.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     4060 2023-07-19 22:51:32.000000 corankco-7.0.1/tests/test_median_ranking_algorithms.py
```

### Comparing `corankco-7.0.0/.github/workflows/python-package.yml` & `corankco-7.0.1/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `corankco-7.0.0/.gitignore` & `corankco-7.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `corankco-7.0.0/.idea/corankco.iml` & `corankco-7.0.1/.idea/corankco.iml`

 * *Files identical despite different names*

### Comparing `corankco-7.0.0/.idea/dictionaries/pierre.xml` & `corankco-7.0.1/.idea/dictionaries/pierre.xml`

 * *Files identical despite different names*

### Comparing `corankco-7.0.0/LICENSE` & `corankco-7.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `corankco-7.0.0/PKG-INFO` & `corankco-7.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: corankco
-Version: 7.0.0
+Version: 7.0.1
 Summary: Kemeny-Young method for rank aggregation of incomplete rankings with ties
 Home-page: https://github.com/pierreandrieu/corankco
 Author: Pierre Andrieu
 Author-email: pierre.andrieu@lilo.org
 License: GPLv2
 Platform: UNKNOWN
 Requires-Python: >=3.8
@@ -21,15 +21,15 @@
 
 ## Installation
 
 Before installing `corankco`, make sure your system meets the following requirements:
 
 - Python >= 3.8
 - For the usage of the exact algorithm on big datasets (with many elements to rank), the installation of IBM ILOG CPLEX Optimization Studio is recommended. A free academic version can be downloaded from the [IBM website](https://www.ibm.com/products/ilog-cplex-optimization-studio). After downloading, follow the [instructions to install CPLEX](https://www.ibm.com/docs/en/icos/20.1.0?topic=studio-setting-up-python).
-
+[README.md](README.md)
 To install `corankco` from PyPI, you can use pip:
 
 ```bash
 pip3 install corankco
 ```
 
 ## Documentation
@@ -42,15 +42,15 @@
 
 ## Contributing
 
 We welcome contributions to `corankco`. If you'd like to contribute, feel free to fork the repository and submit your changes via a pull request.
 
 ## License
 
-`corankco` is licensed under the GPL-2.0 License. You can read more about it in the [LICENSE file](LICENSE).
+`corankco` is licensed under the GPL-2.0 License. You can read more about it in the [LICENSE file](https://github.com/pierreandrieu/corankco/blob/master/LICENSE).
 
 ## Example usage <a class="anchor" id="usage"></a>
 
 ```python
 from typing import List
 import corankco as crc
 
@@ -135,10 +135,10 @@
 print(all_opt)
 
 
  ```
 
  ## Jupiter Notebook for code execution and more examples
 
- More detailed examples and use cases, please refer to our [Jupyter Notebook](corankco_notebook.ipynb).
+ More detailed examples and use cases, please refer to our [Jupyter Notebook](https://github.com/pierreandrieu/corankco/blob/master/corankco_notebook.ipynb).
```

### Comparing `corankco-7.0.0/README.md` & `corankco-7.0.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 ## Installation
 
 Before installing `corankco`, make sure your system meets the following requirements:
 
 - Python >= 3.8
 - For the usage of the exact algorithm on big datasets (with many elements to rank), the installation of IBM ILOG CPLEX Optimization Studio is recommended. A free academic version can be downloaded from the [IBM website](https://www.ibm.com/products/ilog-cplex-optimization-studio). After downloading, follow the [instructions to install CPLEX](https://www.ibm.com/docs/en/icos/20.1.0?topic=studio-setting-up-python).
-
+[README.md](README.md)
 To install `corankco` from PyPI, you can use pip:
 
 ```bash
 pip3 install corankco
 ```
 
 ## Documentation
@@ -29,15 +29,15 @@
 
 ## Contributing
 
 We welcome contributions to `corankco`. If you'd like to contribute, feel free to fork the repository and submit your changes via a pull request.
 
 ## License
 
-`corankco` is licensed under the GPL-2.0 License. You can read more about it in the [LICENSE file](LICENSE).
+`corankco` is licensed under the GPL-2.0 License. You can read more about it in the [LICENSE file](https://github.com/pierreandrieu/corankco/blob/master/LICENSE).
 
 ## Example usage <a class="anchor" id="usage"></a>
 
 ```python
 from typing import List
 import corankco as crc
 
@@ -122,8 +122,8 @@
 print(all_opt)
 
 
  ```
 
  ## Jupiter Notebook for code execution and more examples
 
- More detailed examples and use cases, please refer to our [Jupyter Notebook](corankco_notebook.ipynb).
+ More detailed examples and use cases, please refer to our [Jupyter Notebook](https://github.com/pierreandrieu/corankco/blob/master/corankco_notebook.ipynb).
```

### Comparing `corankco-7.0.0/corankco/__init__.py` & `corankco-7.0.1/corankco/__init__.py`

 * *Files identical despite different names*

### Comparing `corankco-7.0.0/corankco/algorithms/__init__.py` & `corankco-7.0.1/corankco/algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `corankco-7.0.0/corankco/algorithms/algorithm_choice.py` & `corankco-7.0.1/corankco/algorithms/algorithm_choice.py`

 * *Files identical despite different names*

### Comparing `corankco-7.0.0/corankco/algorithms/bioconsert/bioco.py` & `corankco-7.0.1/corankco/algorithms/bioconsert/bioco.py`

 * *Files identical despite different names*

### Comparing `corankco-7.0.0/corankco/algorithms/bioconsert/bioconsert.py` & `corankco-7.0.1/corankco/algorithms/bioconsert/bioconsert.py`

 * *Files identical despite different names*

### Comparing `corankco-7.0.0/corankco/algorithms/borda/borda.py` & `corankco-7.0.1/corankco/algorithms/borda/borda.py`

 * *Files identical despite different names*

### Comparing `corankco-7.0.0/corankco/algorithms/copeland/copeland.py` & `corankco-7.0.1/corankco/algorithms/copeland/copeland.py`

 * *Files identical despite different names*

### Comparing `corankco-7.0.0/corankco/algorithms/exact/exactalgorithm.py` & `corankco-7.0.1/corankco/algorithms/exact/exactalgorithm.py`

 * *Files identical despite different names*

### Comparing `corankco-7.0.0/corankco/algorithms/exact/exactalgorithmbase.py` & `corankco-7.0.1/corankco/algorithms/exact/exactalgorithmbase.py`

 * *Files identical despite different names*

### Comparing `corankco-7.0.0/corankco/algorithms/exact/exactalgorithmcplex.py` & `corankco-7.0.1/corankco/algorithms/exact/exactalgorithmcplex.py`

 * *Files identical despite different names*

### Comparing `corankco-7.0.0/corankco/algorithms/exact/exactalgorithmcplexforpaperoptim1.py` & `corankco-7.0.1/corankco/algorithms/exact/exactalgorithmcplexforpaperoptim1.py`

 * *Files identical despite different names*

### Comparing `corankco-7.0.0/corankco/algorithms/exact/exactalgorithmpulp.py` & `corankco-7.0.1/corankco/algorithms/exact/exactalgorithmpulp.py`

 * *Files identical despite different names*

### Comparing `corankco-7.0.0/corankco/algorithms/kwiksort/kwiksortabs.py` & `corankco-7.0.1/corankco/algorithms/kwiksort/kwiksortabs.py`

 * *Files identical despite different names*

### Comparing `corankco-7.0.0/corankco/algorithms/kwiksort/kwiksortrandom.py` & `corankco-7.0.1/corankco/algorithms/kwiksort/kwiksortrandom.py`

 * *Files identical despite different names*

### Comparing `corankco-7.0.0/corankco/algorithms/pairwisebasedalgorithm.py` & `corankco-7.0.1/corankco/algorithms/pairwisebasedalgorithm.py`

 * *Files identical despite different names*

### Comparing `corankco-7.0.0/corankco/algorithms/parcons/parcons.py` & `corankco-7.0.1/corankco/algorithms/parcons/parcons.py`

 * *Files identical despite different names*

### Comparing `corankco-7.0.0/corankco/algorithms/pickaperm/pickaperm.py` & `corankco-7.0.1/corankco/algorithms/pickaperm/pickaperm.py`

 * *Files identical despite different names*

### Comparing `corankco-7.0.0/corankco/algorithms/rank_aggregation_algorithm.py` & `corankco-7.0.1/corankco/algorithms/rank_aggregation_algorithm.py`

 * *Files identical despite different names*

### Comparing `corankco-7.0.0/corankco/consensus.py` & `corankco-7.0.1/corankco/consensus.py`

 * *Files identical despite different names*

### Comparing `corankco-7.0.0/corankco/dataset.py` & `corankco-7.0.1/corankco/dataset.py`

 * *Files identical despite different names*

### Comparing `corankco-7.0.0/corankco/element.py` & `corankco-7.0.1/corankco/element.py`

 * *Files identical despite different names*

### Comparing `corankco-7.0.0/corankco/kemeny_score_computation.py` & `corankco-7.0.1/corankco/kemeny_score_computation.py`

 * *Files identical despite different names*

### Comparing `corankco-7.0.0/corankco/partitioning/ordered_partition.py` & `corankco-7.0.1/corankco/partitioning/ordered_partition.py`

 * *Files identical despite different names*

### Comparing `corankco-7.0.0/corankco/ranking.py` & `corankco-7.0.1/corankco/ranking.py`

 * *Files identical despite different names*

### Comparing `corankco-7.0.0/corankco/scoringscheme.py` & `corankco-7.0.1/corankco/scoringscheme.py`

 * *Files identical despite different names*

### Comparing `corankco-7.0.0/corankco/utils.py` & `corankco-7.0.1/corankco/utils.py`

 * *Files identical despite different names*

### Comparing `corankco-7.0.0/corankco.egg-info/PKG-INFO` & `corankco-7.0.1/corankco.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: corankco
-Version: 7.0.0
+Version: 7.0.1
 Summary: Kemeny-Young method for rank aggregation of incomplete rankings with ties
 Home-page: https://github.com/pierreandrieu/corankco
 Author: Pierre Andrieu
 Author-email: pierre.andrieu@lilo.org
 License: GPLv2
 Platform: UNKNOWN
 Requires-Python: >=3.8
@@ -21,15 +21,15 @@
 
 ## Installation
 
 Before installing `corankco`, make sure your system meets the following requirements:
 
 - Python >= 3.8
 - For the usage of the exact algorithm on big datasets (with many elements to rank), the installation of IBM ILOG CPLEX Optimization Studio is recommended. A free academic version can be downloaded from the [IBM website](https://www.ibm.com/products/ilog-cplex-optimization-studio). After downloading, follow the [instructions to install CPLEX](https://www.ibm.com/docs/en/icos/20.1.0?topic=studio-setting-up-python).
-
+[README.md](README.md)
 To install `corankco` from PyPI, you can use pip:
 
 ```bash
 pip3 install corankco
 ```
 
 ## Documentation
@@ -42,15 +42,15 @@
 
 ## Contributing
 
 We welcome contributions to `corankco`. If you'd like to contribute, feel free to fork the repository and submit your changes via a pull request.
 
 ## License
 
-`corankco` is licensed under the GPL-2.0 License. You can read more about it in the [LICENSE file](LICENSE).
+`corankco` is licensed under the GPL-2.0 License. You can read more about it in the [LICENSE file](https://github.com/pierreandrieu/corankco/blob/master/LICENSE).
 
 ## Example usage <a class="anchor" id="usage"></a>
 
 ```python
 from typing import List
 import corankco as crc
 
@@ -135,10 +135,10 @@
 print(all_opt)
 
 
  ```
 
  ## Jupiter Notebook for code execution and more examples
 
- More detailed examples and use cases, please refer to our [Jupyter Notebook](corankco_notebook.ipynb).
+ More detailed examples and use cases, please refer to our [Jupyter Notebook](https://github.com/pierreandrieu/corankco/blob/master/corankco_notebook.ipynb).
```

### Comparing `corankco-7.0.0/corankco.egg-info/SOURCES.txt` & `corankco-7.0.1/corankco.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -66,21 +66,14 @@
 docs/build/html/index.html
 docs/build/html/py-modindex.html
 docs/build/html/ranking.html
 docs/build/html/scoring_scheme.html
 docs/build/html/search.html
 docs/source/conf.py
 docs/source/consensus.rst
-docs/source/corankco.algorithms.bioconsert.rst
-docs/source/corankco.algorithms.borda.rst
-docs/source/corankco.algorithms.copeland.rst
-docs/source/corankco.algorithms.exact.rst
-docs/source/corankco.algorithms.kwiksort.rst
-docs/source/corankco.algorithms.parcons.rst
-docs/source/corankco.algorithms.pickaperm.rst
 docs/source/corankco.algorithms.rst
 docs/source/corankco.partitioning.rst
 docs/source/corankco.rst
 docs/source/dataset.rst
 docs/source/element.rst
 docs/source/index.rst
 docs/source/modules.rst
```

### Comparing `corankco-7.0.0/corankco_notebook.ipynb` & `corankco-7.0.1/corankco_notebook.ipynb`

 * *Files identical despite different names*

### Comparing `corankco-7.0.0/docs/Makefile` & `corankco-7.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `corankco-7.0.0/docs/build/html/consensus.html` & `corankco-7.0.1/docs/build/html/consensus.html`

 * *Files identical despite different names*

### Comparing `corankco-7.0.0/docs/build/html/dataset.html` & `corankco-7.0.1/docs/build/html/dataset.html`

 * *Files identical despite different names*

### Comparing `corankco-7.0.0/docs/build/html/element.html` & `corankco-7.0.1/docs/build/html/element.html`

 * *Files identical despite different names*

### Comparing `corankco-7.0.0/docs/build/html/genindex.html` & `corankco-7.0.1/docs/build/html/genindex.html`

 * *Files identical despite different names*

### Comparing `corankco-7.0.0/docs/build/html/index.html` & `corankco-7.0.1/docs/build/html/index.html`

 * *Files identical despite different names*

### Comparing `corankco-7.0.0/docs/build/html/py-modindex.html` & `corankco-7.0.1/docs/build/html/py-modindex.html`

 * *Files identical despite different names*

### Comparing `corankco-7.0.0/docs/build/html/ranking.html` & `corankco-7.0.1/docs/build/html/ranking.html`

 * *Files identical despite different names*

### Comparing `corankco-7.0.0/docs/build/html/scoring_scheme.html` & `corankco-7.0.1/docs/build/html/scoring_scheme.html`

 * *Files identical despite different names*

### Comparing `corankco-7.0.0/docs/build/html/search.html` & `corankco-7.0.1/docs/build/html/search.html`

 * *Files identical despite different names*

### Comparing `corankco-7.0.0/docs/make.bat` & `corankco-7.0.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `corankco-7.0.0/docs/source/conf.py` & `corankco-7.0.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `corankco-7.0.0/docs/source/corankco.algorithms.rst` & `corankco-7.0.1/docs/source/corankco.algorithms.rst`

 * *Files identical despite different names*

### Comparing `corankco-7.0.0/docs/source/corankco.rst` & `corankco-7.0.1/docs/source/corankco.rst`

 * *Files identical despite different names*

### Comparing `corankco-7.0.0/make.bat` & `corankco-7.0.1/make.bat`

 * *Files identical despite different names*

### Comparing `corankco-7.0.0/setup.py` & `corankco-7.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 def readme():
     with open('README.md') as f:
         return f.read()
 
 
 setup(name='corankco',
-      version='7.0.0',
+      version='7.0.1',
       description='Kemeny-Young method for rank aggregation of incomplete rankings with ties',
       long_description_content_type='text/markdown',
       long_description=readme(),
       url='https://github.com/pierreandrieu/corankco',
       author='Pierre Andrieu',
       author_email='pierre.andrieu@lilo.org',
       license='GPLv2',
```

### Comparing `corankco-7.0.0/tests/exemple.py` & `corankco-7.0.1/tests/exemple.py`

 * *Files identical despite different names*

### Comparing `corankco-7.0.0/tests/test_BioCo.py` & `corankco-7.0.1/tests/test_BioCo.py`

 * *Files identical despite different names*

### Comparing `corankco-7.0.0/tests/test_BioConsert.py` & `corankco-7.0.1/tests/test_BioConsert.py`

 * *Files identical despite different names*

### Comparing `corankco-7.0.0/tests/test_Borda.py` & `corankco-7.0.1/tests/test_Borda.py`

 * *Files identical despite different names*

### Comparing `corankco-7.0.0/tests/test_Copeland.py` & `corankco-7.0.1/tests/test_Copeland.py`

 * *Files identical despite different names*

### Comparing `corankco-7.0.0/tests/test_Element.py` & `corankco-7.0.1/tests/test_Element.py`

 * *Files identical despite different names*

### Comparing `corankco-7.0.0/tests/test_Ranking.py` & `corankco-7.0.1/tests/test_Ranking.py`

 * *Files identical despite different names*

### Comparing `corankco-7.0.0/tests/test_ScoringScheme.py` & `corankco-7.0.1/tests/test_ScoringScheme.py`

 * *Files identical despite different names*

### Comparing `corankco-7.0.0/tests/test_dataset.py` & `corankco-7.0.1/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `corankco-7.0.0/tests/test_exact_algorithms.py` & `corankco-7.0.1/tests/test_exact_algorithms.py`

 * *Files identical despite different names*

### Comparing `corankco-7.0.0/tests/test_kemenycomputation.py` & `corankco-7.0.1/tests/test_kemenycomputation.py`

 * *Files identical despite different names*

### Comparing `corankco-7.0.0/tests/test_median_ranking_algorithms.py` & `corankco-7.0.1/tests/test_median_ranking_algorithms.py`

 * *Files identical despite different names*

