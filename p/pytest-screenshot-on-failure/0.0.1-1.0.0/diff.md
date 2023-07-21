# Comparing `tmp/pytest_screenshot_on_failure-0.0.1.tar.gz` & `tmp/pytest_screenshot_on_failure-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_screenshot_on_failure-0.0.1.tar", last modified: Tue Jul 18 17:53:40 2023, max compression
+gzip compressed data, was "pytest_screenshot_on_failure-1.0.0.tar", last modified: Fri Jul 21 21:37:49 2023, max compression
```

## Comparing `pytest_screenshot_on_failure-0.0.1.tar` & `pytest_screenshot_on_failure-1.0.0.tar`

### file list

```diff
@@ -1,13 +1,17 @@
-drwxrwxr-x   0 kleber    (1000) kleber    (1000)        0 2023-07-18 17:53:40.358816 pytest_screenshot_on_failure-0.0.1/
--rw-rw-r--   0 kleber    (1000) kleber    (1000)     1071 2023-07-18 17:27:50.000000 pytest_screenshot_on_failure-0.0.1/LICENSE
--rw-rw-r--   0 kleber    (1000) kleber    (1000)      780 2023-07-18 17:53:40.358816 pytest_screenshot_on_failure-0.0.1/PKG-INFO
--rw-rw-r--   0 kleber    (1000) kleber    (1000)      141 2023-07-18 17:39:47.000000 pytest_screenshot_on_failure-0.0.1/README.md
-drwxrwxr-x   0 kleber    (1000) kleber    (1000)        0 2023-07-18 17:53:40.358816 pytest_screenshot_on_failure-0.0.1/pytest_screenshot_on_failure.egg-info/
--rw-rw-r--   0 kleber    (1000) kleber    (1000)      780 2023-07-18 17:53:40.000000 pytest_screenshot_on_failure-0.0.1/pytest_screenshot_on_failure.egg-info/PKG-INFO
--rw-rw-r--   0 kleber    (1000) kleber    (1000)      350 2023-07-18 17:53:40.000000 pytest_screenshot_on_failure-0.0.1/pytest_screenshot_on_failure.egg-info/SOURCES.txt
--rw-rw-r--   0 kleber    (1000) kleber    (1000)        1 2023-07-18 17:53:40.000000 pytest_screenshot_on_failure-0.0.1/pytest_screenshot_on_failure.egg-info/dependency_links.txt
--rw-rw-r--   0 kleber    (1000) kleber    (1000)       48 2023-07-18 17:53:40.000000 pytest_screenshot_on_failure-0.0.1/pytest_screenshot_on_failure.egg-info/entry_points.txt
--rw-rw-r--   0 kleber    (1000) kleber    (1000)       41 2023-07-18 17:53:40.000000 pytest_screenshot_on_failure-0.0.1/pytest_screenshot_on_failure.egg-info/requires.txt
--rw-rw-r--   0 kleber    (1000) kleber    (1000)        1 2023-07-18 17:53:40.000000 pytest_screenshot_on_failure-0.0.1/pytest_screenshot_on_failure.egg-info/top_level.txt
--rw-rw-r--   0 kleber    (1000) kleber    (1000)      116 2023-07-18 17:53:40.358816 pytest_screenshot_on_failure-0.0.1/setup.cfg
--rw-rw-r--   0 kleber    (1000) kleber    (1000)     1023 2023-07-18 17:48:33.000000 pytest_screenshot_on_failure-0.0.1/setup.py
+drwxrwxr-x   0 kleber    (1000) kleber    (1000)        0 2023-07-21 21:37:49.833675 pytest_screenshot_on_failure-1.0.0/
+-rw-rw-r--   0 kleber    (1000) kleber    (1000)     1071 2023-07-18 17:27:50.000000 pytest_screenshot_on_failure-1.0.0/LICENSE
+-rw-rw-r--   0 kleber    (1000) kleber    (1000)     3212 2023-07-21 21:37:49.833675 pytest_screenshot_on_failure-1.0.0/PKG-INFO
+-rw-rw-r--   0 kleber    (1000) kleber    (1000)     2399 2023-07-21 21:29:53.000000 pytest_screenshot_on_failure-1.0.0/README.md
+-rw-rw-r--   0 kleber    (1000) kleber    (1000)      116 2023-07-21 21:37:49.837675 pytest_screenshot_on_failure-1.0.0/setup.cfg
+-rw-rw-r--   0 kleber    (1000) kleber    (1000)     1297 2023-07-21 21:34:55.000000 pytest_screenshot_on_failure-1.0.0/setup.py
+drwxrwxr-x   0 kleber    (1000) kleber    (1000)        0 2023-07-21 21:37:49.833675 pytest_screenshot_on_failure-1.0.0/src/
+drwxrwxr-x   0 kleber    (1000) kleber    (1000)        0 2023-07-21 21:37:49.833675 pytest_screenshot_on_failure-1.0.0/src/pytest_screenshot_on_failure.egg-info/
+-rw-rw-r--   0 kleber    (1000) kleber    (1000)     3212 2023-07-21 21:37:49.000000 pytest_screenshot_on_failure-1.0.0/src/pytest_screenshot_on_failure.egg-info/PKG-INFO
+-rw-rw-r--   0 kleber    (1000) kleber    (1000)      429 2023-07-21 21:37:49.000000 pytest_screenshot_on_failure-1.0.0/src/pytest_screenshot_on_failure.egg-info/SOURCES.txt
+-rw-rw-r--   0 kleber    (1000) kleber    (1000)        1 2023-07-21 21:37:49.000000 pytest_screenshot_on_failure-1.0.0/src/pytest_screenshot_on_failure.egg-info/dependency_links.txt
+-rw-rw-r--   0 kleber    (1000) kleber    (1000)       72 2023-07-21 21:37:49.000000 pytest_screenshot_on_failure-1.0.0/src/pytest_screenshot_on_failure.egg-info/entry_points.txt
+-rw-rw-r--   0 kleber    (1000) kleber    (1000)       34 2023-07-21 21:37:49.000000 pytest_screenshot_on_failure-1.0.0/src/pytest_screenshot_on_failure.egg-info/requires.txt
+-rw-rw-r--   0 kleber    (1000) kleber    (1000)       29 2023-07-21 21:37:49.000000 pytest_screenshot_on_failure-1.0.0/src/pytest_screenshot_on_failure.egg-info/top_level.txt
+-rw-rw-r--   0 kleber    (1000) kleber    (1000)     5936 2023-07-21 20:38:02.000000 pytest_screenshot_on_failure-1.0.0/src/pytest_screenshot_on_failure.py
+drwxrwxr-x   0 kleber    (1000) kleber    (1000)        0 2023-07-21 21:37:49.833675 pytest_screenshot_on_failure-1.0.0/tests/
+-rw-rw-r--   0 kleber    (1000) kleber    (1000)    10573 2023-07-21 21:26:33.000000 pytest_screenshot_on_failure-1.0.0/tests/test_main.py
```

### Comparing `pytest_screenshot_on_failure-0.0.1/LICENSE` & `pytest_screenshot_on_failure-1.0.0/LICENSE`

 * *Files identical despite different names*

