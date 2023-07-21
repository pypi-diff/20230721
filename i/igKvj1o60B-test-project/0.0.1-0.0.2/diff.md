# Comparing `tmp/igKvj1o60B-test-project-0.0.1.tar.gz` & `tmp/igKvj1o60B-test-project-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "igKvj1o60B-test-project-0.0.1.tar", last modified: Fri Jul 21 14:50:19 2023, max compression
+gzip compressed data, was "igKvj1o60B-test-project-0.0.2.tar", last modified: Fri Jul 21 15:19:20 2023, max compression
```

## Comparing `igKvj1o60B-test-project-0.0.1.tar` & `igKvj1o60B-test-project-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 zieglmeier  (1001) zieglmeier  (1001)        0 2023-07-21 14:50:19.482184 igKvj1o60B-test-project-0.0.1/
--rw-rw-r--   0 zieglmeier  (1001) zieglmeier  (1001)      154 2023-07-21 14:50:19.482184 igKvj1o60B-test-project-0.0.1/PKG-INFO
--rw-rw-r--   0 zieglmeier  (1001) zieglmeier  (1001)      138 2023-07-21 14:20:40.000000 igKvj1o60B-test-project-0.0.1/README.md
-drwxrwxr-x   0 zieglmeier  (1001) zieglmeier  (1001)        0 2023-07-21 14:50:19.482184 igKvj1o60B-test-project-0.0.1/igKvj1o60B_test_project.egg-info/
--rw-rw-r--   0 zieglmeier  (1001) zieglmeier  (1001)      154 2023-07-21 14:50:18.000000 igKvj1o60B-test-project-0.0.1/igKvj1o60B_test_project.egg-info/PKG-INFO
--rw-rw-r--   0 zieglmeier  (1001) zieglmeier  (1001)      252 2023-07-21 14:50:19.000000 igKvj1o60B-test-project-0.0.1/igKvj1o60B_test_project.egg-info/SOURCES.txt
--rw-rw-r--   0 zieglmeier  (1001) zieglmeier  (1001)        1 2023-07-21 14:50:19.000000 igKvj1o60B-test-project-0.0.1/igKvj1o60B_test_project.egg-info/dependency_links.txt
--rw-rw-r--   0 zieglmeier  (1001) zieglmeier  (1001)       14 2023-07-21 14:50:19.000000 igKvj1o60B-test-project-0.0.1/igKvj1o60B_test_project.egg-info/requires.txt
--rw-rw-r--   0 zieglmeier  (1001) zieglmeier  (1001)        1 2023-07-21 14:50:19.000000 igKvj1o60B-test-project-0.0.1/igKvj1o60B_test_project.egg-info/top_level.txt
--rw-rw-r--   0 zieglmeier  (1001) zieglmeier  (1001)       38 2023-07-21 14:50:19.482184 igKvj1o60B-test-project-0.0.1/setup.cfg
--rw-rw-r--   0 zieglmeier  (1001) zieglmeier  (1001)      299 2023-07-21 14:50:07.000000 igKvj1o60B-test-project-0.0.1/setup.py
+drwxrwxr-x   0 zieglmeier  (1001) zieglmeier  (1001)        0 2023-07-21 15:19:20.940335 igKvj1o60B-test-project-0.0.2/
+-rw-rw-r--   0 zieglmeier  (1001) zieglmeier  (1001)      194 2023-07-21 15:19:20.940335 igKvj1o60B-test-project-0.0.2/PKG-INFO
+-rw-rw-r--   0 zieglmeier  (1001) zieglmeier  (1001)      138 2023-07-21 14:20:40.000000 igKvj1o60B-test-project-0.0.2/README.md
+drwxrwxr-x   0 zieglmeier  (1001) zieglmeier  (1001)        0 2023-07-21 15:19:20.940335 igKvj1o60B-test-project-0.0.2/igKvj1o60B_test_project.egg-info/
+-rw-rw-r--   0 zieglmeier  (1001) zieglmeier  (1001)      194 2023-07-21 15:19:20.000000 igKvj1o60B-test-project-0.0.2/igKvj1o60B_test_project.egg-info/PKG-INFO
+-rw-rw-r--   0 zieglmeier  (1001) zieglmeier  (1001)      252 2023-07-21 15:19:20.000000 igKvj1o60B-test-project-0.0.2/igKvj1o60B_test_project.egg-info/SOURCES.txt
+-rw-rw-r--   0 zieglmeier  (1001) zieglmeier  (1001)        1 2023-07-21 15:19:20.000000 igKvj1o60B-test-project-0.0.2/igKvj1o60B_test_project.egg-info/dependency_links.txt
+-rw-rw-r--   0 zieglmeier  (1001) zieglmeier  (1001)       14 2023-07-21 15:19:20.000000 igKvj1o60B-test-project-0.0.2/igKvj1o60B_test_project.egg-info/requires.txt
+-rw-rw-r--   0 zieglmeier  (1001) zieglmeier  (1001)        1 2023-07-21 15:19:20.000000 igKvj1o60B-test-project-0.0.2/igKvj1o60B_test_project.egg-info/top_level.txt
+-rw-rw-r--   0 zieglmeier  (1001) zieglmeier  (1001)       38 2023-07-21 15:19:20.940335 igKvj1o60B-test-project-0.0.2/setup.cfg
+-rw-rw-r--   0 zieglmeier  (1001) zieglmeier  (1001)      337 2023-07-21 15:19:11.000000 igKvj1o60B-test-project-0.0.2/setup.py
```

