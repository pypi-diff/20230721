# Comparing `tmp/chrislab-0.5.6.tar.gz` & `tmp/chrislab-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chrislab-0.5.6.tar", last modified: Mon Jul 10 03:20:34 2023, max compression
+gzip compressed data, was "chrislab-0.5.7.tar", last modified: Fri Jul 21 02:14:46 2023, max compression
```

## Comparing `chrislab-0.5.6.tar` & `chrislab-0.5.7.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 chrisjihee (1000016) users    (1000001)        0 2023-07-10 03:20:34.718400 chrislab-0.5.6/
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)     1066 2023-07-09 16:17:16.000000 chrislab-0.5.6/LICENSE
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)      830 2023-07-10 03:20:34.718400 chrislab-0.5.6/PKG-INFO
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)      291 2023-07-09 16:17:16.000000 chrislab-0.5.6/README.md
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)       81 2023-07-09 16:17:16.000000 chrislab-0.5.6/pyproject.toml
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)     1005 2023-07-10 03:20:34.718400 chrislab-0.5.6/setup.cfg
-drwxr-xr-x   0 chrisjihee (1000016) users    (1000001)        0 2023-07-10 03:20:34.714400 chrislab-0.5.6/src/
-drwxr-xr-x   0 chrisjihee (1000016) users    (1000001)        0 2023-07-10 03:20:34.714400 chrislab-0.5.6/src/chrislab/
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)        0 2023-07-09 16:17:16.000000 chrislab-0.5.6/src/chrislab/__init__.py
-drwxr-xr-x   0 chrisjihee (1000016) users    (1000001)        0 2023-07-10 03:20:34.714400 chrislab-0.5.6/src/chrislab/common/
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)        0 2023-07-09 16:17:16.000000 chrislab-0.5.6/src/chrislab/common/__init__.py
--rwxr-xr-x   0 chrisjihee (1000016) users    (1000001)     7852 2023-07-09 16:17:16.000000 chrislab-0.5.6/src/chrislab/common/downloader.py
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)    12638 2023-07-09 16:17:16.000000 chrislab-0.5.6/src/chrislab/common/tokenizer_korbert.py
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)    11372 2023-07-09 16:17:16.000000 chrislab-0.5.6/src/chrislab/common/util.py
-drwxr-xr-x   0 chrisjihee (1000016) users    (1000001)        0 2023-07-10 03:20:34.718400 chrislab-0.5.6/src/chrislab/language/
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)        0 2023-07-09 16:17:16.000000 chrislab-0.5.6/src/chrislab/language/__init__.py
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)     1319 2023-07-09 16:17:16.000000 chrislab-0.5.6/src/chrislab/language/cli.py
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)    14142 2023-07-09 16:17:16.000000 chrislab-0.5.6/src/chrislab/language/converter.py
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)     9408 2023-07-09 16:17:16.000000 chrislab-0.5.6/src/chrislab/language/evaluater.py
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)    39568 2023-07-09 16:17:16.000000 chrislab-0.5.6/src/chrislab/language/finetuner.py
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)     6833 2023-07-09 16:17:16.000000 chrislab-0.5.6/src/chrislab/language/modeling.py
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)    14491 2023-07-09 16:17:16.000000 chrislab-0.5.6/src/chrislab/language/predictor.py
-drwxr-xr-x   0 chrisjihee (1000016) users    (1000001)        0 2023-07-10 03:20:34.714400 chrislab-0.5.6/src/chrislab.egg-info/
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)      830 2023-07-10 03:20:34.000000 chrislab-0.5.6/src/chrislab.egg-info/PKG-INFO
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)     1541 2023-07-10 03:20:34.000000 chrislab-0.5.6/src/chrislab.egg-info/SOURCES.txt
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)        1 2023-07-10 03:20:34.000000 chrislab-0.5.6/src/chrislab.egg-info/dependency_links.txt
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)      132 2023-07-10 03:20:34.000000 chrislab-0.5.6/src/chrislab.egg-info/entry_points.txt
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)       97 2023-07-10 03:20:34.000000 chrislab-0.5.6/src/chrislab.egg-info/requires.txt
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)       17 2023-07-10 03:20:34.000000 chrislab-0.5.6/src/chrislab.egg-info/top_level.txt
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)        1 2023-07-10 03:20:34.000000 chrislab-0.5.6/src/chrislab.egg-info/zip-safe
-drwxr-xr-x   0 chrisjihee (1000016) users    (1000001)        0 2023-07-10 03:20:34.718400 chrislab-0.5.6/src/nlpbook/
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)       70 2023-07-10 02:57:42.000000 chrislab-0.5.6/src/nlpbook/__init__.py
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)    15545 2023-07-10 03:01:27.000000 chrislab-0.5.6/src/nlpbook/arguments.py
-drwxr-xr-x   0 chrisjihee (1000016) users    (1000001)        0 2023-07-10 03:20:34.718400 chrislab-0.5.6/src/nlpbook/cls/
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)       59 2023-07-09 16:17:16.000000 chrislab-0.5.6/src/nlpbook/cls/__init__.py
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)     8835 2023-07-09 16:17:16.000000 chrislab-0.5.6/src/nlpbook/cls/cli.py
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)     5177 2023-07-09 16:17:16.000000 chrislab-0.5.6/src/nlpbook/cls/corpus.py
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)     2646 2023-07-09 16:17:16.000000 chrislab-0.5.6/src/nlpbook/cls/task.py
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)     2246 2023-07-09 16:17:16.000000 chrislab-0.5.6/src/nlpbook/data_utils.py
-drwxr-xr-x   0 chrisjihee (1000016) users    (1000001)        0 2023-07-10 03:20:34.718400 chrislab-0.5.6/src/nlpbook/dp/
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)      142 2023-07-09 16:17:16.000000 chrislab-0.5.6/src/nlpbook/dp/__init__.py
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)    12298 2023-07-09 16:17:16.000000 chrislab-0.5.6/src/nlpbook/dp/cli.py
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)    18570 2023-07-09 16:17:16.000000 chrislab-0.5.6/src/nlpbook/dp/corpus.py
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)    11240 2023-07-09 16:17:16.000000 chrislab-0.5.6/src/nlpbook/dp/model.py
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)     6968 2023-07-09 16:17:16.000000 chrislab-0.5.6/src/nlpbook/dp/task.py
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)     2057 2023-07-09 16:17:16.000000 chrislab-0.5.6/src/nlpbook/factory.py
-drwxr-xr-x   0 chrisjihee (1000016) users    (1000001)        0 2023-07-10 03:20:34.718400 chrislab-0.5.6/src/nlpbook/generation/
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)      170 2023-07-09 16:17:16.000000 chrislab-0.5.6/src/nlpbook/generation/__init__.py
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)     4280 2023-07-09 16:17:16.000000 chrislab-0.5.6/src/nlpbook/generation/arguments.py
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)     5354 2023-07-09 16:17:16.000000 chrislab-0.5.6/src/nlpbook/generation/corpus.py
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)      882 2023-07-09 16:17:16.000000 chrislab-0.5.6/src/nlpbook/generation/deploy.py
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)     1293 2023-07-09 16:17:16.000000 chrislab-0.5.6/src/nlpbook/generation/task.py
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)     8968 2023-07-09 16:17:16.000000 chrislab-0.5.6/src/nlpbook/metrics.py
-drwxr-xr-x   0 chrisjihee (1000016) users    (1000001)        0 2023-07-10 03:20:34.718400 chrislab-0.5.6/src/nlpbook/ner/
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)       87 2023-07-09 16:17:16.000000 chrislab-0.5.6/src/nlpbook/ner/__init__.py
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)    18164 2023-07-09 16:17:16.000000 chrislab-0.5.6/src/nlpbook/ner/cli.py
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)    14181 2023-07-09 16:17:16.000000 chrislab-0.5.6/src/nlpbook/ner/corpus.py
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)    10013 2023-07-09 16:17:16.000000 chrislab-0.5.6/src/nlpbook/ner/task.py
-drwxr-xr-x   0 chrisjihee (1000016) users    (1000001)        0 2023-07-10 03:20:34.718400 chrislab-0.5.6/src/nlpbook/paircls/
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)       62 2023-07-09 16:17:16.000000 chrislab-0.5.6/src/nlpbook/paircls/__init__.py
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)     2654 2023-07-09 16:17:16.000000 chrislab-0.5.6/src/nlpbook/paircls/corpus.py
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)      641 2023-07-09 16:17:16.000000 chrislab-0.5.6/src/nlpbook/paircls/deploy.py
-drwxr-xr-x   0 chrisjihee (1000016) users    (1000001)        0 2023-07-10 03:20:34.718400 chrislab-0.5.6/src/nlpbook/qa/
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)      146 2023-07-09 16:17:16.000000 chrislab-0.5.6/src/nlpbook/qa/__init__.py
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)     4984 2023-07-09 16:17:16.000000 chrislab-0.5.6/src/nlpbook/qa/arguments.py
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)    17080 2023-07-09 16:17:16.000000 chrislab-0.5.6/src/nlpbook/qa/corpus.py
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)      639 2023-07-09 16:17:16.000000 chrislab-0.5.6/src/nlpbook/qa/deploy.py
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)     2072 2023-07-09 16:17:16.000000 chrislab-0.5.6/src/nlpbook/qa/task.py
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)     9761 2023-07-09 16:17:16.000000 chrislab-0.5.6/src/nlpbook/utils.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-07-21 02:14:46.121773 chrislab-0.5.7/
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1066 2023-07-21 00:41:08.000000 chrislab-0.5.7/LICENSE
+-rw-rw-r--   0 chris     (1000) chris     (1000)      830 2023-07-21 02:14:46.121773 chrislab-0.5.7/PKG-INFO
+-rw-rw-r--   0 chris     (1000) chris     (1000)      291 2023-07-21 00:41:08.000000 chrislab-0.5.7/README.md
+-rw-rw-r--   0 chris     (1000) chris     (1000)       81 2023-07-21 00:41:08.000000 chrislab-0.5.7/pyproject.toml
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1005 2023-07-21 02:14:46.121773 chrislab-0.5.7/setup.cfg
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-07-21 02:14:46.113773 chrislab-0.5.7/src/
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-07-21 02:14:46.117773 chrislab-0.5.7/src/chrislab/
+-rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-07-21 00:41:08.000000 chrislab-0.5.7/src/chrislab/__init__.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-07-21 02:14:46.117773 chrislab-0.5.7/src/chrislab/common/
+-rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-07-21 00:41:08.000000 chrislab-0.5.7/src/chrislab/common/__init__.py
+-rwxrwxr-x   0 chris     (1000) chris     (1000)     7852 2023-07-21 00:41:08.000000 chrislab-0.5.7/src/chrislab/common/downloader.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    12638 2023-07-21 00:41:08.000000 chrislab-0.5.7/src/chrislab/common/tokenizer_korbert.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    11372 2023-07-21 00:41:08.000000 chrislab-0.5.7/src/chrislab/common/util.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-07-21 02:14:46.117773 chrislab-0.5.7/src/chrislab/language/
+-rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-07-21 00:41:08.000000 chrislab-0.5.7/src/chrislab/language/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1319 2023-07-21 00:41:08.000000 chrislab-0.5.7/src/chrislab/language/cli.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    14142 2023-07-21 00:41:08.000000 chrislab-0.5.7/src/chrislab/language/converter.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     9408 2023-07-21 00:41:08.000000 chrislab-0.5.7/src/chrislab/language/evaluater.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    39568 2023-07-21 00:41:08.000000 chrislab-0.5.7/src/chrislab/language/finetuner.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     6833 2023-07-21 00:41:08.000000 chrislab-0.5.7/src/chrislab/language/modeling.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    14491 2023-07-21 00:41:08.000000 chrislab-0.5.7/src/chrislab/language/predictor.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-07-21 02:14:46.117773 chrislab-0.5.7/src/chrislab.egg-info/
+-rw-rw-r--   0 chris     (1000) chris     (1000)      830 2023-07-21 02:14:46.000000 chrislab-0.5.7/src/chrislab.egg-info/PKG-INFO
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1541 2023-07-21 02:14:46.000000 chrislab-0.5.7/src/chrislab.egg-info/SOURCES.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)        1 2023-07-21 02:14:46.000000 chrislab-0.5.7/src/chrislab.egg-info/dependency_links.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)      132 2023-07-21 02:14:46.000000 chrislab-0.5.7/src/chrislab.egg-info/entry_points.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)       97 2023-07-21 02:14:46.000000 chrislab-0.5.7/src/chrislab.egg-info/requires.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)       17 2023-07-21 02:14:46.000000 chrislab-0.5.7/src/chrislab.egg-info/top_level.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)        1 2023-07-21 02:14:46.000000 chrislab-0.5.7/src/chrislab.egg-info/zip-safe
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-07-21 02:14:46.117773 chrislab-0.5.7/src/nlpbook/
+-rw-rw-r--   0 chris     (1000) chris     (1000)       70 2023-07-21 00:41:08.000000 chrislab-0.5.7/src/nlpbook/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    13222 2023-07-21 01:58:50.000000 chrislab-0.5.7/src/nlpbook/arguments.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-07-21 02:14:46.117773 chrislab-0.5.7/src/nlpbook/cls/
+-rw-rw-r--   0 chris     (1000) chris     (1000)       59 2023-07-21 00:41:08.000000 chrislab-0.5.7/src/nlpbook/cls/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     8835 2023-07-21 00:41:08.000000 chrislab-0.5.7/src/nlpbook/cls/cli.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     5177 2023-07-21 00:41:08.000000 chrislab-0.5.7/src/nlpbook/cls/corpus.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     2646 2023-07-21 00:41:08.000000 chrislab-0.5.7/src/nlpbook/cls/task.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     2246 2023-07-21 00:41:08.000000 chrislab-0.5.7/src/nlpbook/data_utils.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-07-21 02:14:46.117773 chrislab-0.5.7/src/nlpbook/dp/
+-rw-rw-r--   0 chris     (1000) chris     (1000)      142 2023-07-21 00:41:08.000000 chrislab-0.5.7/src/nlpbook/dp/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    12276 2023-07-21 00:41:08.000000 chrislab-0.5.7/src/nlpbook/dp/cli.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    18570 2023-07-21 00:41:08.000000 chrislab-0.5.7/src/nlpbook/dp/corpus.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    10936 2023-07-21 00:41:08.000000 chrislab-0.5.7/src/nlpbook/dp/model.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     8265 2023-07-21 00:41:08.000000 chrislab-0.5.7/src/nlpbook/dp/task.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     2057 2023-07-21 00:41:08.000000 chrislab-0.5.7/src/nlpbook/factory.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-07-21 02:14:46.117773 chrislab-0.5.7/src/nlpbook/generation/
+-rw-rw-r--   0 chris     (1000) chris     (1000)      170 2023-07-21 00:41:08.000000 chrislab-0.5.7/src/nlpbook/generation/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     4280 2023-07-21 00:41:08.000000 chrislab-0.5.7/src/nlpbook/generation/arguments.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     5354 2023-07-21 00:41:08.000000 chrislab-0.5.7/src/nlpbook/generation/corpus.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      882 2023-07-21 00:41:08.000000 chrislab-0.5.7/src/nlpbook/generation/deploy.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1293 2023-07-21 00:41:08.000000 chrislab-0.5.7/src/nlpbook/generation/task.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     8966 2023-07-21 00:41:08.000000 chrislab-0.5.7/src/nlpbook/metrics.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-07-21 02:14:46.121773 chrislab-0.5.7/src/nlpbook/ner/
+-rw-rw-r--   0 chris     (1000) chris     (1000)       87 2023-07-21 00:41:08.000000 chrislab-0.5.7/src/nlpbook/ner/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    18044 2023-07-21 00:41:08.000000 chrislab-0.5.7/src/nlpbook/ner/cli.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    14181 2023-07-21 00:41:08.000000 chrislab-0.5.7/src/nlpbook/ner/corpus.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    11601 2023-07-21 00:41:08.000000 chrislab-0.5.7/src/nlpbook/ner/task.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-07-21 02:14:46.121773 chrislab-0.5.7/src/nlpbook/paircls/
+-rw-rw-r--   0 chris     (1000) chris     (1000)       62 2023-07-21 00:41:08.000000 chrislab-0.5.7/src/nlpbook/paircls/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     2654 2023-07-21 00:41:08.000000 chrislab-0.5.7/src/nlpbook/paircls/corpus.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      641 2023-07-21 00:41:08.000000 chrislab-0.5.7/src/nlpbook/paircls/deploy.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-07-21 02:14:46.121773 chrislab-0.5.7/src/nlpbook/qa/
+-rw-rw-r--   0 chris     (1000) chris     (1000)      146 2023-07-21 00:41:08.000000 chrislab-0.5.7/src/nlpbook/qa/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     4984 2023-07-21 00:41:08.000000 chrislab-0.5.7/src/nlpbook/qa/arguments.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    17080 2023-07-21 00:41:08.000000 chrislab-0.5.7/src/nlpbook/qa/corpus.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      639 2023-07-21 00:41:08.000000 chrislab-0.5.7/src/nlpbook/qa/deploy.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     2072 2023-07-21 00:41:08.000000 chrislab-0.5.7/src/nlpbook/qa/task.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     9761 2023-07-21 00:41:08.000000 chrislab-0.5.7/src/nlpbook/utils.py
```

### Comparing `chrislab-0.5.6/LICENSE` & `chrislab-0.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.6/PKG-INFO` & `chrislab-0.5.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chrislab
-Version: 0.5.6
+Version: 0.5.7
 Summary: An advanced tool for doing experimental study.
 Home-page: https://github.com/chrisjihee/chrislab
 Author: Jihee Ryu
 Author-email: chrisjihee@naver.com
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `chrislab-0.5.6/setup.cfg` & `chrislab-0.5.7/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = chrislab
-version = 0.5.6
+version = 0.5.7
 author = Jihee Ryu
 author_email = chrisjihee@naver.com
 url = https://github.com/chrisjihee/chrislab
 description = An advanced tool for doing experimental study.
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT License
```

### Comparing `chrislab-0.5.6/src/chrislab/common/downloader.py` & `chrislab-0.5.7/src/chrislab/common/downloader.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.6/src/chrislab/common/tokenizer_korbert.py` & `chrislab-0.5.7/src/chrislab/common/tokenizer_korbert.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.6/src/chrislab/common/util.py` & `chrislab-0.5.7/src/chrislab/common/util.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.6/src/chrislab/language/cli.py` & `chrislab-0.5.7/src/chrislab/language/cli.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.6/src/chrislab/language/converter.py` & `chrislab-0.5.7/src/chrislab/language/converter.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.6/src/chrislab/language/evaluater.py` & `chrislab-0.5.7/src/chrislab/language/evaluater.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.6/src/chrislab/language/finetuner.py` & `chrislab-0.5.7/src/chrislab/language/finetuner.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.6/src/chrislab/language/modeling.py` & `chrislab-0.5.7/src/chrislab/language/modeling.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.6/src/chrislab/language/predictor.py` & `chrislab-0.5.7/src/chrislab/language/predictor.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.6/src/chrislab.egg-info/PKG-INFO` & `chrislab-0.5.7/src/chrislab.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chrislab
-Version: 0.5.6
+Version: 0.5.7
 Summary: An advanced tool for doing experimental study.
 Home-page: https://github.com/chrisjihee/chrislab
 Author: Jihee Ryu
 Author-email: chrisjihee@naver.com
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `chrislab-0.5.6/src/chrislab.egg-info/SOURCES.txt` & `chrislab-0.5.7/src/chrislab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.6/src/nlpbook/arguments.py` & `chrislab-0.5.7/src/nlpbook/arguments.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,41 +1,33 @@
 import logging
 import math
 import os
-import sys
 from dataclasses import dataclass, field
 from datetime import datetime
 from pathlib import Path
 from typing import List
 
 import pandas as pd
 import pytorch_lightning
 import transformers
 import typer
 from dataclasses_json import DataClassJsonMixin
 from pytorch_lightning.accelerators import Accelerator
 from pytorch_lightning.loggers import CSVLogger
 from pytorch_lightning.strategies import Strategy
 
-from chrisbase.io import files, make_parent_dir, hr, str_table, out_hr, out_table, get_hostname, get_hostaddr, running_file, first_or, cwd, configure_dual_logger, configure_unit_logger, LoggingFormat
+from chrisbase.data import TypedData, ProjectEnv
+from chrisbase.io import files, make_parent_dir, hr, str_table, out_hr, out_table, configure_dual_logger, LoggingFormat
 from chrisbase.time import now, str_delta
 from chrisbase.util import to_dataframe
 
 logger = logging.getLogger(__name__)
 
 
 @dataclass
-class TypedData(DataClassJsonMixin):
-    data_type = None
-
-    def __post_init__(self):
-        self.data_type = self.__class__.__name__
-
-
-@dataclass
 class OptionData(TypedData):
     def __post_init__(self):
         super().__post_init__()
 
 
 @dataclass
 class ResultData(TypedData):
@@ -142,59 +134,14 @@
     result: dict = field(init=False, default_factory=dict)
     global_step: int = field(init=False, default=0)
     global_epoch: float = field(init=False, default=0.0)
     epoch_per_step: float = field(init=False, default=0.0)
 
 
 @dataclass
-class ProjectEnv(TypedData):
-    project: str = field()
-    job_name: str = field(default=None)
-    hostname: str = field(init=False)
-    hostaddr: str = field(init=False)
-    python_path: Path = field(init=False)
-    working_path: Path = field(init=False)
-    running_file: Path = field(init=False)
-    command_args: List[str] = field(init=False)
-    output_home: str | Path | None = field(default=None)
-    logging_file: str | Path = field(default="message.out")
-    argument_file: str | Path = field(default="arguments.json")
-    debugging: bool = field(default=False)
-    msg_level: int = field(default=logging.INFO)
-    msg_format: str = field(default=logging.BASIC_FORMAT)
-    date_format: str = field(default="[%m.%d %H:%M:%S]")
-    csv_logger: CSVLogger | None = field(init=False, default=None)
-
-    def set(self, name: str = None):
-        self.job_name = name
-        return self
-
-    def __post_init__(self):
-        assert self.project, "Project name must be provided"
-        self.hostname = get_hostname()
-        self.hostaddr = get_hostaddr()
-        self.python_path = Path(sys.executable)
-        self.running_file = running_file()
-        self.project_path = first_or([x for x in self.running_file.parents if x.name.startswith(self.project)])
-        assert self.project_path, f"Could not find project path for {self.project} in {', '.join([str(x) for x in self.running_file.parents])}"
-        self.working_path = cwd(self.project_path)
-        self.running_file = self.running_file.relative_to(self.working_path)
-        self.command_args = sys.argv[1:]
-        self.logging_file = Path(self.logging_file)
-        self.argument_file = Path(self.argument_file)
-        if self.output_home:
-            self.output_home = Path(self.output_home)
-            configure_dual_logger(level=self.msg_level, fmt=self.msg_format, datefmt=self.date_format,
-                                  filename=self.output_home / self.logging_file)
-        else:
-            configure_unit_logger(level=self.msg_level, fmt=self.msg_format, datefmt=self.date_format,
-                                  stream=sys.stdout)
-
-
-@dataclass
 class CommonArguments(ArgumentGroupData):
     tag = "common"
     env: ProjectEnv = field()
     time: TimeChecker = field(default=TimeChecker())
     prog: ProgressChecker = field(default=ProgressChecker())
     data: DataOption | None = field(default=None)
     model: ModelOption | None = field(default=None)
```

### Comparing `chrislab-0.5.6/src/nlpbook/cls/cli.py` & `chrislab-0.5.7/src/nlpbook/cls/cli.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.6/src/nlpbook/cls/corpus.py` & `chrislab-0.5.7/src/nlpbook/cls/corpus.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.6/src/nlpbook/cls/task.py` & `chrislab-0.5.7/src/nlpbook/cls/task.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.6/src/nlpbook/data_utils.py` & `chrislab-0.5.7/src/nlpbook/data_utils.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.6/src/nlpbook/dp/cli.py` & `chrislab-0.5.7/src/nlpbook/dp/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import logging
 import re
 import sys
 from pathlib import Path
 from typing import Any, Dict, List, Tuple
 
+import lightning as L
 import torch
 import torch.nn.functional as F
 from torch.utils.data import DataLoader, RandomSampler, SequentialSampler
+from transformers import PreTrainedTokenizerFast, AutoTokenizer, AutoConfig, AutoModel, BertConfig, BertModel, RobertaConfig, RobertaModel, PreTrainedModel, PretrainedConfig
 from typer import Typer
 
-import lightning as L
 from chrisbase.io import JobTimer, pop_keys, err_hr
 from chrislab.common.util import time_tqdm_cls, mute_tqdm_cls
 from nlpbook import save_checkpoint
 from nlpbook.arguments import TrainerArguments, RuntimeChecking
 from nlpbook.dp.corpus import DPCorpus, DPDataset
 from nlpbook.dp.model import ModelForDependencyParsing
 from nlpbook.metrics import DPResult
-from transformers import PreTrainedTokenizerFast, AutoTokenizer, AutoConfig, AutoModel, BertConfig, BertModel, RobertaConfig, RobertaModel, PreTrainedModel, PretrainedConfig
 
 app = Typer()
 logger = logging.getLogger(__name__)
 term_pattern = re.compile(re.escape("{") + "(.+?)(:.+?)?" + re.escape("}"))
 
 
 @app.command()
@@ -32,29 +32,29 @@
     L.seed_everything(args.learning.seed)
 
     with JobTimer(f"chrialab.nlpbook.dp fabric_train {args_file}", mt=1, mb=1, rt=1, rb=1, rc='=', verbose=True, flush_sec=0.3):
         # Data
         tokenizer: PreTrainedTokenizerFast = AutoTokenizer.from_pretrained(args.model.pretrained, use_fast=True)
         assert isinstance(tokenizer, PreTrainedTokenizerFast), f"Our code support only PreTrainedTokenizerFast, but used {type(tokenizer)}"
         corpus = DPCorpus(args)
-        train_dataset = DPDataset("train", args=args, corpus=corpus, tokenizer=tokenizer)
+        train_dataset = DPDataset("train", corpus=corpus, tokenizer=tokenizer)
         train_dataloader = DataLoader(train_dataset,
                                       # sampler=SequentialSampler(train_dataset),  # TODO: temporary
                                       sampler=RandomSampler(train_dataset, replacement=False),
                                       num_workers=args.hardware.cpu_workers,
                                       batch_size=args.hardware.batch_size,
                                       collate_fn=corpus.encoded_examples_to_batch,
                                       # drop_last=True,
                                       drop_last=False,  # TODO: temporary
                                       )
         logger.info(f"Created train_dataset providing {len(train_dataset)} examples")
         logger.info(f"Created train_dataloader loading {len(train_dataloader)} batches")
         args.prog.epoch_per_step = 1 / len(train_dataloader)
         err_hr(c='-')
-        valid_dataset = DPDataset("valid", args=args, corpus=corpus, tokenizer=tokenizer)
+        valid_dataset = DPDataset("valid", corpus=corpus, tokenizer=tokenizer)
         valid_dataloader = DataLoader(valid_dataset,
                                       sampler=SequentialSampler(valid_dataset),
                                       num_workers=args.hardware.cpu_workers,
                                       batch_size=args.hardware.batch_size,
                                       collate_fn=corpus.encoded_examples_to_batch,
                                       # drop_last=True,
                                       drop_last=False,  # TODO: temporary
```

### Comparing `chrislab-0.5.6/src/nlpbook/dp/corpus.py` & `chrislab-0.5.7/src/nlpbook/dp/corpus.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.6/src/nlpbook/dp/model.py` & `chrislab-0.5.7/src/nlpbook/dp/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,33 +4,23 @@
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from torch.nn.parameter import Parameter
 from torch.nn.utils.rnn import pack_padded_sequence, pad_packed_sequence
 
 from nlpbook.dp.corpus import DPCorpus
-from nlpbook.metrics import DP_UASMacroF1, DP_UASMicroF1, DP_LASMacroF1, DP_LASMicroF1
 from transformers import PreTrainedModel
 from transformers.modeling_outputs import BaseModelOutputWithPoolingAndCrossAttentions
 
-metric_tools_for_DP = {
-    "UASa": DP_UASMacroF1,
-    "UASi": DP_UASMicroF1,
-    "LASa": DP_LASMacroF1,
-    "LASi": DP_LASMicroF1,
-}
-
 
 class ModelForDependencyParsing(nn.Module):
     def __init__(self,
                  corpus: DPCorpus,
-                 pretrained_model: PreTrainedModel,
-                 ):
+                 pretrained_model: PreTrainedModel):
         super().__init__()
-        self.metric_tools = nn.ModuleDict(metric_tools_for_DP)
         self.encoder_layers = 1  # Number of layers of encoder
         self.decoder_layers = 1  # Number of layers of decoder
         self.hidden_size = 768  # Number of hidden units in LSTM
         self.arc_space = 512  # Dimension of tag space
         self.type_space = 256  # Dimension of tag space
         self.pos_dim = 256  # Dimension of pos embedding
         self.input_size = pretrained_model.config.hidden_size
```

### Comparing `chrislab-0.5.6/src/nlpbook/dp/task.py` & `chrislab-0.5.7/src/nlpbook/dp/task.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,70 +1,81 @@
 import logging
-from typing import Dict, List
+from typing import List, Dict
 
 import torch
 import torch.nn.functional as F
 from pytorch_lightning import LightningModule, Trainer
 from torch.optim import AdamW
 from torch.optim.lr_scheduler import ExponentialLR
 
 from nlpbook.arguments import TesterArguments, TrainerArguments
 from nlpbook.dp import ModelForDependencyParsing
-from nlpbook.metrics import DPResult
+from nlpbook.metrics import DPResult, BasicMetricTool, DP_UAS_MacroF1, DP_UAS_MicroF1, DP_LAS_MacroF1, DP_LAS_MicroF1
 
 logger = logging.getLogger(__name__)
 
 
 class DPTask(LightningModule):
     def __init__(self,
                  args: TesterArguments | TrainerArguments,
                  model: ModelForDependencyParsing,
-                 trainer: Trainer):
+                 trainer: Trainer,
+                 epoch_steps: int):
         super().__init__()
         self.args: TesterArguments | TrainerArguments = args
         self.model: ModelForDependencyParsing = model
         self.trainer: Trainer = trainer
+        self.epoch_steps: int = epoch_steps
 
-        # initialize setting
-        self._log_kwargs = {
-            "batch_size": self.args.hardware.batch_size,
-            "sync_dist": True,
-            "prog_bar": True,
-            "logger": True,
+        # for validation
+        self.metric_tools: Dict[str, BasicMetricTool] = {
+            "UASa": DP_UAS_MacroF1,
+            "UASi": DP_UAS_MicroF1,
+            "LASa": DP_LAS_MacroF1,
+            "LASi": DP_LAS_MicroF1,
         }
 
         # initalize result
         self._valid_preds: List[DPResult] = []
         self._valid_labels: List[DPResult] = []
         self._valid_losses: List[torch.Tensor] = []
         self._train_losses: List[torch.Tensor] = []
 
-    def _learning_rate(self):
+    def _global_step(self) -> float:
+        return self.trainer.lightning_module.global_step * 1.0
+
+    def _global_epoch(self) -> float:
+        return self._global_step() / self.epoch_steps
+
+    def _learning_rate(self) -> float:
         return self.trainer.optimizers[0].param_groups[0]["lr"]
 
-    def _train_loss(self):
+    def _train_loss(self) -> torch.Tensor:
         return torch.tensor(self._train_losses).mean()
 
-    def _valid_loss(self):
+    def _valid_loss(self) -> torch.Tensor:
         return torch.tensor(self._valid_losses).mean()
 
-    def _valid_metric(self, tool):
-        tool.reset()
-        tool.update(self._valid_preds, self._valid_labels)
-        return tool.compute()
+    def _valid_metric(self, metric_tool: BasicMetricTool) -> torch.Tensor | float:
+        metric_tool.reset()
+        metric_tool.update(self._valid_preds, self._valid_labels)
+        return metric_tool.compute()
+
+    def _log_value(self, name: str, value: torch.Tensor | float):
+        self.log(name, value, batch_size=self.args.hardware.batch_size, sync_dist=True, prog_bar=True, logger=True)
 
     def configure_optimizers(self):
         optimizer = AdamW(self.parameters(), lr=self.args.learning.lr)
         scheduler = ExponentialLR(optimizer, gamma=0.9)
         return {
             'optimizer': optimizer,
             'lr_scheduler': scheduler,
         }
 
-    def training_step(self, batch: Dict[str, torch.Tensor], batch_idx: int) -> torch.Tensor:
+    def training_step(self, batch: Dict[str, torch.Tensor], batch_idx: int) -> Dict[str, torch.Tensor]:
         batch.pop("example_ids")
         inputs = {"input_ids": batch["input_ids"], "attention_mask": batch["attention_mask"]}
 
         batch_size = batch["head_ids"].size()[0]
         batch_index = torch.arange(0, int(batch_size)).long()
         max_word_length = batch["max_word_length"].item()
         head_index = (
@@ -98,20 +109,19 @@
         num = batch["mask_d"].sum()
 
         loss_arc = loss_arc[batch_index, head_index, batch["head_ids"].data.t()].transpose(0, 1)
         loss_type = loss_type[batch_index, head_index, batch["type_ids"].data.t()].transpose(0, 1)
         loss_arc = -loss_arc.sum() / num
         loss_type = -loss_type.sum() / num
         loss = loss_arc + loss_type
+        return {
+            "loss": loss,
+        }
 
-        # accumulate result
-        self._train_losses.append(loss)
-        return loss
-
-    def validation_step(self, batch: Dict[str, torch.Tensor], batch_idx: int) -> torch.Tensor:
+    def validation_step(self, batch: Dict[str, torch.Tensor], batch_idx: int) -> Dict[str, torch.Tensor | DPResult]:
         batch.pop("example_ids")
         inputs = {"input_ids": batch["input_ids"], "attention_mask": batch["attention_mask"]}
 
         batch_size = batch["head_ids"].size()[0]
         batch_index = torch.arange(0, int(batch_size)).long()
         max_word_length = batch["max_word_length"].item()
         head_index = (
@@ -152,36 +162,47 @@
         loss = loss_arc + loss_type
 
         # predict arc and its type
         pred_heads: torch.Tensor = torch.argmax(out_arc, dim=2)
         pred_types: torch.Tensor = torch.argmax(out_type, dim=2)
         preds = DPResult(pred_heads, pred_types)
         labels = DPResult(batch["head_ids"], batch["type_ids"])
-
-        # accumulate result
-        self._valid_preds.append(preds)
-        self._valid_labels.append(labels)
-        self._valid_losses.append(loss)
-        return loss
+        return {
+            "loss": loss,
+            "preds": preds,
+            "labels": labels,
+        }
 
     def on_train_epoch_start(self) -> None:
         self._train_losses.clear()
 
     def on_validation_epoch_start(self) -> None:
         self._valid_preds.clear()
         self._valid_labels.clear()
         self._valid_losses.clear()
 
     def on_train_batch_end(self, outputs: Dict[str, torch.Tensor], batch: Dict[str, torch.Tensor], batch_idx: int) -> None:
-        self.log("loss", outputs["loss"], **self._log_kwargs)
+        self._train_losses.append(outputs["loss"])
+        self._log_value("g_step", self._global_step())
+        self._log_value("g_epoch", self._global_epoch())
+        self._log_value("lr", self._learning_rate())
+        self._log_value("loss", outputs["loss"])
+        self._log_value("avg_loss", self._train_loss())
+
+    def on_validation_batch_end(self, outputs: Dict[str, torch.Tensor | DPResult], batch: Dict[str, torch.Tensor], batch_idx: int, dataloader_idx: int = 0) -> None:
+        self._valid_preds.append(outputs["preds"])
+        self._valid_labels.append(outputs["labels"])
+        self._valid_losses.append(outputs["loss"])
 
     def on_validation_epoch_end(self) -> None:
+        assert self._valid_preds
+        assert self._valid_labels
         assert len(self._valid_preds) == len(self._valid_labels)
-        self.log("lr", self._learning_rate(), **self._log_kwargs)
-        self.log("avg_loss", self._train_loss(), **self._log_kwargs)
-        self.log("val_loss", self._valid_loss(), **self._log_kwargs)
-        for name, tool in self.model.metric_tools.items():
-            self.log(f"val_{name}", self._valid_metric(tool), **self._log_kwargs)
-        self._valid_preds.clear()
-        self._valid_labels.clear()
-        self._valid_losses.clear()
-        self._train_losses.clear()
+        self._log_value("g_step", self._global_step())
+        self._log_value("g_epoch", self._global_epoch())
+        self._log_value("lr", self._learning_rate())
+        self._log_value("avg_loss", self._train_loss())
+        self._log_value("val_loss", self._valid_loss())
+        for name, tool in self.metric_tools.items():
+            self._log_value(f"val_{name}", self._valid_metric(tool))
+        self.on_validation_epoch_start()
+        self.on_train_epoch_start()  # reset accumulated train losses after validation
```

### Comparing `chrislab-0.5.6/src/nlpbook/factory.py` & `chrislab-0.5.7/src/nlpbook/factory.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.6/src/nlpbook/generation/arguments.py` & `chrislab-0.5.7/src/nlpbook/generation/arguments.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.6/src/nlpbook/generation/corpus.py` & `chrislab-0.5.7/src/nlpbook/generation/corpus.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.6/src/nlpbook/generation/deploy.py` & `chrislab-0.5.7/src/nlpbook/generation/deploy.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.6/src/nlpbook/generation/task.py` & `chrislab-0.5.7/src/nlpbook/generation/task.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.6/src/nlpbook/metrics.py` & `chrislab-0.5.7/src/nlpbook/metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,19 +33,19 @@
         self.targets = []
         self.metric_fn = metric_fn
 
     def reset(self) -> None:
         self.preds = []
         self.targets = []
 
-    def update(self, preds: torch.Tensor, targets: torch.Tensor) -> None:
+    def update(self, preds, targets) -> None:
         self.preds.append(preds)
         self.targets.append(targets)
 
-    def compute(self) -> Any:
+    def compute(self) -> torch.Tensor | float | int:
         preds = self.preds
         targets = self.targets
 
         if type(preds[0]) == torch.Tensor:
             preds = torch.cat(preds, dim=0)
             preds = preds.cpu().numpy()
         if type(targets[0]) == torch.Tensor:
@@ -62,20 +62,20 @@
     def __init__(
             self,
             metric_fn: Callable,
     ) -> None:
         super().__init__(metric_fn=metric_fn)
         self.label_info = None
 
-    def update(self, preds: torch.Tensor, targets: torch.Tensor, label_info: Optional[Any] = None) -> None:
+    def update(self, preds, targets, label_info: Optional[Any] = None) -> None:
         super().update(preds, targets)
         if self.label_info is None:
             self.label_info = label_info
 
-    def compute(self) -> Any:
+    def compute(self) -> torch.Tensor | float | int:
         preds = self.preds
         targets = self.targets
 
         if type(preds[0]) == torch.Tensor:
             preds = torch.cat(preds, dim=0)
             preds = preds.cpu().numpy()
         if type(targets[0]) == torch.Tensor:
@@ -93,15 +93,15 @@
 
     def __repr__(self):
         return f"""DPResult(
  - head={self.heads.tolist()},
  - types={self.types.tolist()})"""
 
 
-def klue_ner_entity_macro_f1(preds: List[int], labels: List[int], label_list: List[str]) -> Any:
+def klue_ner_entity_macro_f1(preds: np.ndarray, labels: np.ndarray, label_list: List[str]) -> Any:
     """KLUE-NER entity-level macro F1 (except O tag)"""
     preds = np.array(preds).flatten().tolist()
     labels = np.array(labels).flatten().tolist()
     preds_label = []
     labels_label = []
 
     for pred in preds:
@@ -109,27 +109,26 @@
     for label in labels:
         labels_label.append(label_list[label])
 
     entity_macro_f1 = se_metrics.f1_score([labels_label], [preds_label], average="macro", mode="strict", scheme=se_scheme.IOB2)
     return entity_macro_f1 * 100.0
 
 
-def klue_ner_char_macro_f1(preds: List[int], labels: List[int], label_list: List[str]) -> Any:
+def klue_ner_char_macro_f1(preds: np.ndarray, labels: np.ndarray, label_list: List[str]) -> Any:
     """KLUE-NER character level macro f1 (except O tag)"""
     label_indices = list(range(len(label_list)))
     preds = np.array(preds).flatten().tolist()
     trues = np.array(labels).flatten().tolist()
     return sk_metrics.f1_score(trues, preds, labels=label_indices, average="macro", zero_division=True) * 100.0
 
 
 def klue_dp_uas_macro_f1(preds: List[List[DPResult]], labels: List[List[DPResult]]) -> Any:
     """KLUE-DP UAS macro f1. (UAS : head correct / LAS : head + type correct)"""
     head_preds = list()
     head_labels = list()
-
     for pred, label in zip(preds[0], labels[0]):
         head_preds += pred.heads.cpu().flatten().tolist()
         head_labels += label.heads.cpu().flatten().tolist()
     head_preds = np.array(head_preds)
     head_labels = np.array(head_labels)
     index = [i for i, label in enumerate(head_labels) if label == -1]
     head_preds = np.delete(head_preds, index)
@@ -137,15 +136,14 @@
     return sk_metrics.f1_score(head_labels.tolist(), head_preds.tolist(), average="macro") * 100.0
 
 
 def klue_dp_uas_micro_f1(preds: List[List[DPResult]], labels: List[List[DPResult]]) -> Any:
     """KLUE-DP UAS micro f1. (UAS : head correct / LAS : head + type correct)"""
     head_preds = list()
     head_labels = list()
-
     for pred, label in zip(preds[0], labels[0]):
         head_preds += pred.heads.cpu().flatten().tolist()
         head_labels += label.heads.cpu().flatten().tolist()
     head_preds = np.array(head_preds)
     head_labels = np.array(head_labels)
     index = [i for i, label in enumerate(head_labels) if label == -1]
     head_preds = np.delete(head_preds, index)
@@ -230,13 +228,13 @@
     uas_correct = np.equal(head_preds, head_labels)
     uas_incorrect = np.nonzero(np.invert(uas_correct))
     for idx in uas_incorrect:
         type_preds[idx] = PAD
     return sk_metrics.f1_score(type_labels.tolist(), type_preds.tolist(), average="micro") * 100.0
 
 
-DP_UASMacroF1 = BasicMetricTool(klue_dp_uas_macro_f1)
-DP_UASMicroF1 = BasicMetricTool(klue_dp_uas_micro_f1)
-DP_LASMacroF1 = BasicMetricTool(klue_dp_las_macro_f1)
-DP_LASMicroF1 = BasicMetricTool(klue_dp_las_micro_f1)
-NER_CharMacroF1 = LabelMetricTool(klue_ner_char_macro_f1)
-NER_EntityMacroF1 = LabelMetricTool(klue_ner_entity_macro_f1)
+DP_UAS_MacroF1 = BasicMetricTool(klue_dp_uas_macro_f1)
+DP_UAS_MicroF1 = BasicMetricTool(klue_dp_uas_micro_f1)
+DP_LAS_MacroF1 = BasicMetricTool(klue_dp_las_macro_f1)
+DP_LAS_MicroF1 = BasicMetricTool(klue_dp_las_micro_f1)
+NER_Char_MacroF1 = LabelMetricTool(klue_ner_char_macro_f1)
+NER_Entity_MacroF1 = LabelMetricTool(klue_ner_entity_macro_f1)
```

### Comparing `chrislab-0.5.6/src/nlpbook/ner/cli.py` & `chrislab-0.5.7/src/nlpbook/ner/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,26 +13,21 @@
 from typer import Typer
 
 import nlpbook
 from chrisbase.io import JobTimer, pop_keys, err_hr, out_hr
 from chrislab.common.util import time_tqdm_cls, mute_tqdm_cls
 from nlpbook import save_checkpoint, TERM_IN_NAME_FORMAT
 from nlpbook.arguments import TrainerArguments, ServerArguments, TesterArguments, RuntimeChecking
-from nlpbook.metrics import accuracy, NER_CharMacroF1, NER_EntityMacroF1, klue_ner_char_macro_f1, klue_ner_entity_macro_f1
+from nlpbook.metrics import accuracy, klue_ner_char_macro_f1, klue_ner_entity_macro_f1
 from nlpbook.ner.corpus import NERCorpus, NERDataset, NEREncodedExample
 from nlpbook.ner.task import NERTask
 
 app = Typer()
 logger = logging.getLogger(__name__)
 
-metric_tools_for_NER = {
-    "F1c": NER_CharMacroF1,
-    "F1e": NER_EntityMacroF1,
-}
-
 
 @app.command()
 def fabric_train(args_file: Path | str):
     args_file = Path(args_file)
     assert args_file.exists(), f"No args_file: {args_file}"
     args: TrainerArguments = TrainerArguments.from_json(args_file.read_text()).show()
     L.seed_everything(args.learning.seed)
@@ -225,15 +220,15 @@
             config=pretrained_model_config
         )
         err_hr(c='-')
 
         with RuntimeChecking(args.reconfigure_output()):
             torch.set_float32_matmul_precision('high')
             trainer: pl.Trainer = nlpbook.make_trainer(args)
-            trainer.fit(NERTask(model=model, args=args, trainer=trainer, val_dataset=val_dataset,
+            trainer.fit(NERTask(model=model, args=args, trainer=trainer, valid_dataset=val_dataset,
                                 total_steps=len(train_dataloader) * args.learning.epochs),
                         train_dataloaders=train_dataloader,
                         val_dataloaders=val_dataloader)
 
 
 @app.command()
 def test(args_file: Path | str):
```

### Comparing `chrislab-0.5.6/src/nlpbook/ner/corpus.py` & `chrislab-0.5.7/src/nlpbook/ner/corpus.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.6/src/nlpbook/ner/task.py` & `chrislab-0.5.7/src/nlpbook/ner/task.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,175 +1,230 @@
 import logging
-from typing import List, Dict, Tuple
+from typing import Tuple, List, Dict
 
 import torch
 from pytorch_lightning import LightningModule, Trainer
 from torch.optim import AdamW
 from torch.optim.lr_scheduler import ExponentialLR
 from transformers import PreTrainedModel, CharSpan
 from transformers.modeling_outputs import TokenClassifierOutput
 
 from chrisbase.io import hr
 from nlpbook.arguments import TesterArguments, TrainerArguments
-from nlpbook.metrics import accuracy, klue_ner_char_macro_f1, klue_ner_entity_macro_f1
+from nlpbook.metrics import LabelMetricTool, accuracy, NER_Char_MacroF1, NER_Entity_MacroF1
 from nlpbook.ner import NERDataset, NEREncodedExample
 
 logger = logging.getLogger(__name__)
 
 
-def label_to_char_labels(label, num_char):
-    for i in range(num_char):
-        if i > 0 and ("-" in label):
-            yield "I-" + label.split("-", maxsplit=1)[-1]
-        else:
-            yield label
-
-
 class NERTask(LightningModule):
     def __init__(self,
                  args: TesterArguments | TrainerArguments,
                  model: PreTrainedModel,
                  trainer: Trainer,
-                 val_dataset: NERDataset,
-                 total_steps: int):
+                 epoch_steps: int,
+                 valid_dataset: NERDataset):
         super().__init__()
-        self.model: PreTrainedModel = model
         self.args: TesterArguments | TrainerArguments = args
+        self.model: PreTrainedModel = model
         self.trainer: Trainer = trainer
+        self.epoch_steps: int = epoch_steps
 
-        self.val_dataset: NERDataset = val_dataset
-        self._validation_char_pred_ids = None
-        self._validation_char_label_ids = None
-
-        self._labels: List[str] = self.val_dataset.get_labels()
+        # for validation
+        self.valid_dataset: NERDataset = valid_dataset
+        self._labels: List[str] = self.valid_dataset.get_labels()
         self._label_to_id: Dict[str, int] = {label: i for i, label in enumerate(self._labels)}
         self._id_to_label: Dict[int, str] = {i: label for i, label in enumerate(self._labels)}
+        self.metric_tools: Dict[str, LabelMetricTool] = {
+            "F1c": NER_Char_MacroF1,
+            "F1e": NER_Entity_MacroF1,
+        }
 
-        self.total_steps: int = total_steps
-        self.train_loss: float = -1.0
-        self.train_acc: float = -1.0
-
-    def get_labels(self):
-        return self._labels
-
-    def label_to_id(self, x):
-        return self._label_to_id[x]
-
-    def id_to_label(self, x):
-        return self._id_to_label[x]
-
-    def _global_step(self):
-        return self.trainer.lightning_module.global_step
+        # initalize result
+        self._valid_preds: List[int] = []
+        self._valid_labels: List[int] = []
+        self._valid_losses: List[torch.Tensor] = []
+        self._train_losses: List[torch.Tensor] = []
+        self._valid_accuracies: List[torch.Tensor] = []
+        self._train_accuracies: List[torch.Tensor] = []
+
+    def _global_step(self) -> float:
+        return self.trainer.lightning_module.global_step * 1.0
+
+    def _global_epoch(self) -> float:
+        return self._global_step() / self.epoch_steps
+
+    def _learning_rate(self) -> float:
+        return self.trainer.optimizers[0].param_groups[0]["lr"]
+
+    def _train_loss(self) -> torch.Tensor:
+        return torch.tensor(self._train_losses).mean()
+
+    def _valid_loss(self) -> torch.Tensor:
+        return torch.tensor(self._valid_losses).mean()
+
+    def _train_accuracy(self) -> torch.Tensor:
+        return torch.tensor(self._train_accuracies).mean()
+
+    def _valid_accuracy(self) -> torch.Tensor:
+        return torch.tensor(self._valid_accuracies).mean()
+
+    def _valid_metric(self, metric_tool: LabelMetricTool) -> torch.Tensor | float:
+        metric_tool.reset()
+        metric_tool.update(self._valid_preds, self._valid_labels, self._labels)
+        return metric_tool.compute()
 
-    def _trained_rate(self):
-        return self.trainer.lightning_module.global_step / self.total_steps
+    def _log_value(self, name: str, value: torch.Tensor | float):
+        self.log(name, value, batch_size=self.args.hardware.batch_size, sync_dist=True, prog_bar=True, logger=True)
 
     def configure_optimizers(self):
         optimizer = AdamW(self.parameters(), lr=self.args.learning.lr)
         scheduler = ExponentialLR(optimizer, gamma=0.9)
         return {
             'optimizer': optimizer,
             'lr_scheduler': scheduler,
         }
 
-    def training_step(self, batch: Dict[str, torch.Tensor], batch_idx: int) -> torch.Tensor:
+    def training_step(self, batch: Dict[str, torch.Tensor], batch_idx: int) -> Dict[str, torch.Tensor]:
         batch.pop("example_ids")
         outputs: TokenClassifierOutput = self.model(**batch)
         labels: torch.Tensor = batch["labels"]
         preds: torch.Tensor = outputs.logits.argmax(dim=-1)
         acc: torch.Tensor = accuracy(preds, labels, ignore_index=0)
-        self.train_loss = outputs.loss
-        self.train_acc = acc
-        return outputs.loss
-
-    def validation_step(self, batch: Dict[str, torch.Tensor], batch_idx: int) -> torch.Tensor:
-        logger.debug('')
-        logger.debug(f"[validation_step] batch_idx: {batch_idx}, global_step: {self._global_step()}")
-        for key in batch.keys():
-            if isinstance(batch[key], torch.Tensor):
-                logger.debug(f"  - batch[{key:14s}]     = {batch[key].shape} | {batch[key].tolist()}")
+        return {
+            "loss": outputs.loss,
+            "acc": acc,
+        }
+
+    @staticmethod
+    def label_to_char_labels(label, num_char):
+        for i in range(num_char):
+            if i > 0 and ("-" in label):
+                yield "I-" + label.split("-", maxsplit=1)[-1]
             else:
-                logger.debug(f"  - batch[{key:14s}]     = ({len(batch[key])}) | {batch[key]}")
+                yield label
+
+    def label_to_id(self, x):
+        return self._label_to_id[x]
+
+    def id_to_label(self, x):
+        return self._id_to_label[x]
+
+    def validation_step(self, batch: Dict[str, torch.Tensor], batch_idx: int) -> Dict[str, torch.Tensor | List[int]]:
+        if self.args.env.debugging:
+            logger.debug('')
+            logger.debug(f"[validation_step] batch_idx: {batch_idx}, global_step: {self.trainer.lightning_module.global_step}")
+            for key in batch.keys():
+                if isinstance(batch[key], torch.Tensor):
+                    logger.debug(f"  - batch[{key:14s}]     = {batch[key].shape} | {batch[key].tolist()}")
+                else:
+                    logger.debug(f"  - batch[{key:14s}]     = ({len(batch[key])}) | {batch[key]}")
         example_ids: List[int] = batch.pop("example_ids").tolist()
         outputs: TokenClassifierOutput = self.model(**batch)
         labels: torch.Tensor = batch["labels"]
         preds: torch.Tensor = outputs.logits.argmax(dim=-1)
-        acc: torch.Tensor = accuracy(preds, labels, ignore_index=0)
-
-        self.log(sync_dist=True, prog_bar=True, logger=False, on_epoch=True, name="global_step", value=self._global_step() * 1.0)
-        self.log(sync_dist=True, prog_bar=True, logger=False, on_epoch=True, name="trained_rate", value=self._trained_rate())
-        self.log(sync_dist=True, prog_bar=True, logger=False, on_epoch=True, name="train_loss", value=self.train_loss)
-        self.log(sync_dist=True, prog_bar=True, logger=False, on_epoch=True, name="train_acc", value=self.train_acc)
-        self.log(sync_dist=True, prog_bar=True, logger=False, on_epoch=True, name="val_loss", value=outputs.loss)
-        self.log(sync_dist=True, prog_bar=True, logger=False, on_epoch=True, name="val_acc", value=acc)
+        acc: torch.Tensor = accuracy(preds=preds, labels=labels, ignore_index=0)
 
         dict_of_token_pred_ids: Dict[int, List[int]] = {}
         dict_of_char_label_ids: Dict[int, List[int]] = {}
         dict_of_char_pred_ids: Dict[int, List[int]] = {}
         for token_pred_ids, example_id in zip(preds.tolist(), example_ids):
             token_pred_tags: List[str] = [self.id_to_label(x) for x in token_pred_ids]
-            encoded_example: NEREncodedExample = self.val_dataset[example_id]
+            encoded_example: NEREncodedExample = self.valid_dataset[example_id]
             offset_to_label: Dict[int, str] = encoded_example.raw.get_offset_label_dict()
             all_char_pair_tags: List[Tuple[str | None, str | None]] = [(None, None)] * len(encoded_example.raw.character_list)
             for token_id in range(self.args.model.seq_len):
                 token_span: CharSpan = encoded_example.encoded.token_to_chars(token_id)
                 if token_span:
-                    char_pred_tags = label_to_char_labels(token_pred_tags[token_id], token_span.end - token_span.start)
+                    char_pred_tags = NERTask.label_to_char_labels(token_pred_tags[token_id], token_span.end - token_span.start)
                     for offset, char_pred_tag in zip(range(token_span.start, token_span.end), char_pred_tags):
                         all_char_pair_tags[offset] = (offset_to_label[offset], char_pred_tag)
             valid_char_pair_tags = [(a, b) for a, b in all_char_pair_tags if a and b]
             valid_char_label_ids = [self.label_to_id(a) for a, b in valid_char_pair_tags]
             valid_char_pred_ids = [self.label_to_id(b) for a, b in valid_char_pair_tags]
             dict_of_token_pred_ids[example_id] = token_pred_ids
             dict_of_char_label_ids[example_id] = valid_char_label_ids
             dict_of_char_pred_ids[example_id] = valid_char_pred_ids
 
-        logger.debug(hr())
-        flatlist_of_char_pred_ids: List[int] = []
-        flatlist_of_char_label_ids: List[int] = []
-        for encoded_example in [self.val_dataset[i] for i in example_ids]:
-            token_pred_ids = dict_of_token_pred_ids[encoded_example.idx]
+        if self.args.env.debugging:
+            logger.debug(hr())
+        list_of_char_pred_ids: List[int] = []
+        list_of_char_label_ids: List[int] = []
+        for encoded_example in [self.valid_dataset[i] for i in example_ids]:
             char_label_ids = dict_of_char_label_ids[encoded_example.idx]
             char_pred_ids = dict_of_char_pred_ids[encoded_example.idx]
-            flatlist_of_char_pred_ids.extend(char_pred_ids)
-            flatlist_of_char_label_ids.extend(char_label_ids)
+            assert len(char_pred_ids) == len(char_label_ids)
+            list_of_char_pred_ids.extend(char_pred_ids)
+            list_of_char_label_ids.extend(char_label_ids)
+            if self.args.env.debugging:
+                token_pred_ids = dict_of_token_pred_ids[encoded_example.idx]
+                logger.debug(f"  - encoded_example.idx                = {encoded_example.idx}")
+                logger.debug(f"  - encoded_example.raw.entity_list    = ({len(encoded_example.raw.entity_list)}) {encoded_example.raw.entity_list}")
+                logger.debug(f"  - encoded_example.raw.origin         = ({len(encoded_example.raw.origin)}) {encoded_example.raw.origin}")
+                logger.debug(f"  - encoded_example.raw.character_list = ({len(encoded_example.raw.character_list)}) {' | '.join(f'{x}/{y}' for x, y in encoded_example.raw.character_list)}")
+                logger.debug(f"  - encoded_example.encoded.tokens()   = ({len(encoded_example.encoded.tokens())}) {' '.join(encoded_example.encoded.tokens())}")
+
+                def id_label(x):
+                    return f"{self.id_to_label(x):5s}"
+
+                logger.debug(f"  - encoded_example.label_ids          = ({len(encoded_example.label_ids)}) {' '.join(map(str, map(id_label, encoded_example.label_ids)))}")
+                logger.debug(f"  - encoded_example.token_pred_ids     = ({len(token_pred_ids)}) {' '.join(map(str, map(id_label, token_pred_ids)))}")
+                logger.debug(f"  - encoded_example.char_label_ids     = ({len(char_label_ids)}) {' '.join(map(str, map(id_label, char_label_ids)))}")
+                logger.debug(f"  - encoded_example.char_pred_ids      = ({len(char_pred_ids)}) {' '.join(map(str, map(id_label, char_pred_ids)))}")
+                logger.debug(hr('-'))
+        assert len(list_of_char_pred_ids) == len(list_of_char_label_ids)
+
+        if self.args.env.debugging:
+            def id_str(x):
+                return f"{x:02d}"
 
-            logger.debug(f"  - encoded_example.idx                = {encoded_example.idx}")
-            logger.debug(f"  - encoded_example.raw.entity_list    = ({len(encoded_example.raw.entity_list)}) {encoded_example.raw.entity_list}")
-            logger.debug(f"  - encoded_example.raw.origin         = ({len(encoded_example.raw.origin)}) {encoded_example.raw.origin}")
-            logger.debug(f"  - encoded_example.raw.character_list = ({len(encoded_example.raw.character_list)}) {' | '.join(f'{x}/{y}' for x, y in encoded_example.raw.character_list)}")
-            logger.debug(f"  - encoded_example.encoded.tokens()   = ({len(encoded_example.encoded.tokens())}) {' '.join(encoded_example.encoded.tokens())}")
-            current_repr = lambda x: f"{self.id_to_label(x):5s}"
-            logger.debug(f"  - encoded_example.label_ids          = ({len(encoded_example.label_ids)}) {' '.join(map(str, map(current_repr, encoded_example.label_ids)))}")
-            logger.debug(f"  - encoded_example.token_pred_ids     = ({len(token_pred_ids)}) {' '.join(map(str, map(current_repr, token_pred_ids)))}")
-            logger.debug(f"  - encoded_example.char_label_ids     = ({len(char_label_ids)}) {' '.join(map(str, map(current_repr, char_label_ids)))}")
-            logger.debug(f"  - encoded_example.char_pred_ids      = ({len(char_pred_ids)}) {' '.join(map(str, map(current_repr, char_pred_ids)))}")
-            logger.debug(hr('-'))
-
-        current_repr = lambda x: f"{x:02d}"
-        logger.debug(f"  - flatlist_of_char_label_ids = ({len(flatlist_of_char_label_ids)}) {' '.join(map(str, map(current_repr, flatlist_of_char_label_ids)))}")
-        logger.debug(f"  - flatlist_of_char_pred_ids  = ({len(flatlist_of_char_pred_ids)}) {' '.join(map(str, map(current_repr, flatlist_of_char_pred_ids)))}")
-        assert len(flatlist_of_char_label_ids) == len(flatlist_of_char_pred_ids)
-        self._validation_char_pred_ids.extend(flatlist_of_char_pred_ids)
-        self._validation_char_label_ids.extend(flatlist_of_char_label_ids)
-        return outputs.loss
-
-    def on_validation_start(self):
-        self._validation_char_pred_ids: List[int] = []
-        self._validation_char_label_ids: List[int] = []
-
-    def on_validation_epoch_end(self):
-        assert self._validation_char_pred_ids and self._validation_char_label_ids
-        assert len(self._validation_char_pred_ids) == len(self._validation_char_label_ids)
-        chr_f1 = klue_ner_char_macro_f1(preds=self._validation_char_pred_ids, labels=self._validation_char_label_ids, label_list=self._labels)
-        ent_f1 = klue_ner_entity_macro_f1(preds=self._validation_char_pred_ids, labels=self._validation_char_label_ids, label_list=self._labels)
-        self.log(sync_dist=True, prog_bar=True, logger=True, on_epoch=True, name="val_F1c", value=chr_f1)
-        self.log(sync_dist=True, prog_bar=True, logger=True, on_epoch=True, name="val_F1e", value=ent_f1)
+            logger.debug(f"  - list_of_char_label_ids = ({len(list_of_char_label_ids)}) {' '.join(map(str, map(id_str, list_of_char_label_ids)))}")
+            logger.debug(f"  - list_of_char_pred_ids  = ({len(list_of_char_pred_ids)}) {' '.join(map(str, map(id_str, list_of_char_pred_ids)))}")
+        return {
+            "loss": outputs.loss,
+            "acc": acc,
+            "preds": list_of_char_pred_ids,
+            "labels": list_of_char_label_ids
+        }
 
-    def test_step(self, batch, batch_idx) -> torch.Tensor:
-        outputs: TokenClassifierOutput = self.model(**batch)
-        labels: torch.Tensor = batch["labels"]
-        preds: torch.Tensor = outputs.logits.argmax(dim=-1)
-        acc: torch.Tensor = accuracy(preds, labels, ignore_index=0)
-        self.log(sync_dist=True, prog_bar=False, logger=True, on_epoch=True, name="test_loss", value=outputs.loss)
-        self.log(sync_dist=True, prog_bar=False, logger=True, on_epoch=True, name="test_acc", value=acc)
-        return outputs.loss
+    def on_train_epoch_start(self) -> None:
+        self._train_losses.clear()
+        self._train_accuracies.clear()
+
+    def on_validation_epoch_start(self) -> None:
+        self._valid_preds.clear()
+        self._valid_labels.clear()
+        self._valid_losses.clear()
+        self._valid_accuracies.clear()
+
+    def on_train_batch_end(self, outputs: Dict[str, torch.Tensor], batch: Dict[str, torch.Tensor], batch_idx: int) -> None:
+        self._train_losses.append(outputs["loss"])
+        self._train_accuracies.append(outputs["acc"])
+        self._log_value("g_step", self._global_step())
+        self._log_value("g_epoch", self._global_epoch())
+        self._log_value("lr", self._learning_rate())
+        self._log_value("loss", outputs["loss"])
+        self._log_value("acc", outputs["acc"])
+        self._log_value("avg_loss", self._train_loss())
+        self._log_value("avg_acc", self._train_accuracy())
+
+    def on_validation_batch_end(self, outputs: Dict[str, torch.Tensor | List[int]], batch: Dict[str, torch.Tensor], batch_idx: int, dataloader_idx: int = 0) -> None:
+        self._valid_preds.extend(outputs["preds"])
+        self._valid_labels.extend(outputs["labels"])
+        self._valid_losses.append(outputs["loss"])
+        self._valid_accuracies.append(outputs["acc"])
+
+    def on_validation_epoch_end(self) -> None:
+        assert self._valid_preds
+        assert self._valid_labels
+        assert len(self._valid_preds) == len(self._valid_labels)
+        self._log_value("g_step", self._global_step())
+        self._log_value("g_epoch", self._global_epoch())
+        self._log_value("lr", self._learning_rate())
+        self._log_value("avg_loss", self._train_loss())
+        self._log_value("avg_acc", self._train_accuracy())
+        self._log_value("val_loss", self._valid_loss())
+        self._log_value("val_acc", self._valid_accuracy())
+        for name, tool in self.metric_tools.items():
+            self._log_value(f"val_{name}", self._valid_metric(tool))
+        self.on_validation_epoch_start()
+        self.on_train_epoch_start()  # reset accumulated train losses after validation
```

### Comparing `chrislab-0.5.6/src/nlpbook/paircls/corpus.py` & `chrislab-0.5.7/src/nlpbook/paircls/corpus.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.6/src/nlpbook/paircls/deploy.py` & `chrislab-0.5.7/src/nlpbook/paircls/deploy.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.6/src/nlpbook/qa/arguments.py` & `chrislab-0.5.7/src/nlpbook/qa/arguments.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.6/src/nlpbook/qa/corpus.py` & `chrislab-0.5.7/src/nlpbook/qa/corpus.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.6/src/nlpbook/qa/deploy.py` & `chrislab-0.5.7/src/nlpbook/qa/deploy.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.6/src/nlpbook/qa/task.py` & `chrislab-0.5.7/src/nlpbook/qa/task.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.6/src/nlpbook/utils.py` & `chrislab-0.5.7/src/nlpbook/utils.py`

 * *Files identical despite different names*

