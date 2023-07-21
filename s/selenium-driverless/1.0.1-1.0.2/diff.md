# Comparing `tmp/selenium_driverless-1.0.1.tar.gz` & `tmp/selenium_driverless-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selenium_driverless-1.0.1.tar", last modified: Fri Jul 21 21:00:20 2023, max compression
+gzip compressed data, was "selenium_driverless-1.0.2.tar", last modified: Fri Jul 21 21:04:27 2023, max compression
```

## Comparing `selenium_driverless-1.0.1.tar` & `selenium_driverless-1.0.2.tar`

### file list

```diff
@@ -1,29 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-07-21 21:00:20.944766 selenium_driverless-1.0.1/
--rw-rw-rw-   0        0        0      688 2023-07-21 13:27:27.000000 selenium_driverless-1.0.1/LICENSE.md
--rw-rw-rw-   0        0        0       89 2023-01-11 09:10:16.000000 selenium_driverless-1.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     3329 2023-07-21 21:00:20.945795 selenium_driverless-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2013 2023-07-21 20:59:28.000000 selenium_driverless-1.0.1/README.md
--rw-rw-rw-   0        0        0      528 2023-07-21 13:29:57.000000 selenium_driverless-1.0.1/build_upload.md
--rw-rw-rw-   0        0        0      101 2022-11-24 08:05:09.000000 selenium_driverless-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      133 2023-07-21 21:00:20.946765 selenium_driverless-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1936 2023-07-21 20:56:42.000000 selenium_driverless-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-21 21:00:20.915272 selenium_driverless-1.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-07-21 21:00:20.935678 selenium_driverless-1.0.1/src/selenium_driverless/
--rw-rw-rw-   0        0        0       23 2023-07-21 21:00:08.000000 selenium_driverless-1.0.1/src/selenium_driverless/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 21:00:20.940680 selenium_driverless-1.0.1/src/selenium_driverless/files/
--rw-rw-rw-   0        0        0        0 2023-07-21 16:36:38.000000 selenium_driverless-1.0.1/src/selenium_driverless/files/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 21:00:20.942679 selenium_driverless-1.0.1/src/selenium_driverless/scripts/
--rw-rw-rw-   0        0        0        0 2022-11-29 13:10:11.000000 selenium_driverless-1.0.1/src/selenium_driverless/scripts/__init__.py
--rw-rw-rw-   0        0        0     1400 2023-01-11 12:23:14.000000 selenium_driverless-1.0.1/src/selenium_driverless/scripts/multi_thread.py
--rw-rw-rw-   0        0        0    15809 2023-07-21 20:46:21.000000 selenium_driverless-1.0.1/src/selenium_driverless/scripts/options.py
-drwxrwxrwx   0        0        0        0 2023-07-21 21:00:20.943763 selenium_driverless-1.0.1/src/selenium_driverless/utils/
--rw-rw-rw-   0        0        0     3569 2023-07-21 19:38:37.000000 selenium_driverless-1.0.1/src/selenium_driverless/utils/utils.py
--rw-rw-rw-   0        0        0      112 2023-07-21 15:10:50.000000 selenium_driverless-1.0.1/src/selenium_driverless/webdriver.py
-drwxrwxrwx   0        0        0        0 2023-07-21 21:00:20.939678 selenium_driverless-1.0.1/src/selenium_driverless.egg-info/
--rw-rw-rw-   0        0        0     3329 2023-07-21 21:00:20.000000 selenium_driverless-1.0.1/src/selenium_driverless.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      630 2023-07-21 21:00:20.000000 selenium_driverless-1.0.1/src/selenium_driverless.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 21:00:20.000000 selenium_driverless-1.0.1/src/selenium_driverless.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      132 2023-07-21 21:00:20.000000 selenium_driverless-1.0.1/src/selenium_driverless.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-07-21 21:00:20.000000 selenium_driverless-1.0.1/src/selenium_driverless.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-21 21:00:20.943763 selenium_driverless-1.0.1/tests/
--rw-rw-rw-   0        0        0     3238 2023-01-12 15:12:48.000000 selenium_driverless-1.0.1/tests/test_driverless.py
+drwxrwxrwx   0        0        0        0 2023-07-21 21:04:27.803971 selenium_driverless-1.0.2/
+-rw-rw-rw-   0        0        0      688 2023-07-21 13:27:27.000000 selenium_driverless-1.0.2/LICENSE.md
+-rw-rw-rw-   0        0        0       89 2023-01-11 09:10:16.000000 selenium_driverless-1.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     3329 2023-07-21 21:04:27.803971 selenium_driverless-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2013 2023-07-21 20:59:28.000000 selenium_driverless-1.0.2/README.md
+-rw-rw-rw-   0        0        0      528 2023-07-21 13:29:57.000000 selenium_driverless-1.0.2/build_upload.md
+-rw-rw-rw-   0        0        0      101 2022-11-24 08:05:09.000000 selenium_driverless-1.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0      133 2023-07-21 21:04:27.804684 selenium_driverless-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1936 2023-07-21 20:56:42.000000 selenium_driverless-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 21:04:27.781821 selenium_driverless-1.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-07-21 21:04:27.789901 selenium_driverless-1.0.2/src/selenium_driverless/
+-rw-rw-rw-   0        0        0       23 2023-07-21 21:03:39.000000 selenium_driverless-1.0.2/src/selenium_driverless/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 21:04:27.796898 selenium_driverless-1.0.2/src/selenium_driverless/async_/
+-rw-rw-rw-   0        0        0        0 2023-07-21 21:02:35.000000 selenium_driverless-1.0.2/src/selenium_driverless/async_/__init__.py
+-rw-rw-rw-   0        0        0     2720 2023-07-21 20:13:40.000000 selenium_driverless-1.0.2/src/selenium_driverless/async_/mobile.py
+-rw-rw-rw-   0        0        0    44379 2023-07-21 20:53:34.000000 selenium_driverless-1.0.2/src/selenium_driverless/async_/webdriver.py
+drwxrwxrwx   0        0        0        0 2023-07-21 21:04:27.797897 selenium_driverless-1.0.2/src/selenium_driverless/files/
+-rw-rw-rw-   0        0        0        0 2023-07-21 16:36:38.000000 selenium_driverless-1.0.2/src/selenium_driverless/files/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 21:04:27.799990 selenium_driverless-1.0.2/src/selenium_driverless/scripts/
+-rw-rw-rw-   0        0        0        0 2022-11-29 13:10:11.000000 selenium_driverless-1.0.2/src/selenium_driverless/scripts/__init__.py
+-rw-rw-rw-   0        0        0     1400 2023-01-11 12:23:14.000000 selenium_driverless-1.0.2/src/selenium_driverless/scripts/multi_thread.py
+-rw-rw-rw-   0        0        0    15809 2023-07-21 20:46:21.000000 selenium_driverless-1.0.2/src/selenium_driverless/scripts/options.py
+drwxrwxrwx   0        0        0        0 2023-07-21 21:04:27.801971 selenium_driverless-1.0.2/src/selenium_driverless/utils/
+-rw-rw-rw-   0        0        0        0 2023-07-21 21:02:48.000000 selenium_driverless-1.0.2/src/selenium_driverless/utils/__init__.py
+-rw-rw-rw-   0        0        0     3569 2023-07-21 19:38:37.000000 selenium_driverless-1.0.2/src/selenium_driverless/utils/utils.py
+-rw-rw-rw-   0        0        0      112 2023-07-21 15:10:50.000000 selenium_driverless-1.0.2/src/selenium_driverless/webdriver.py
+drwxrwxrwx   0        0        0        0 2023-07-21 21:04:27.794898 selenium_driverless-1.0.2/src/selenium_driverless.egg-info/
+-rw-rw-rw-   0        0        0     3329 2023-07-21 21:04:27.000000 selenium_driverless-1.0.2/src/selenium_driverless.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      800 2023-07-21 21:04:27.000000 selenium_driverless-1.0.2/src/selenium_driverless.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 21:04:27.000000 selenium_driverless-1.0.2/src/selenium_driverless.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      132 2023-07-21 21:04:27.000000 selenium_driverless-1.0.2/src/selenium_driverless.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-07-21 21:04:27.000000 selenium_driverless-1.0.2/src/selenium_driverless.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-21 21:04:27.802971 selenium_driverless-1.0.2/tests/
+-rw-rw-rw-   0        0        0     3238 2023-01-12 15:12:48.000000 selenium_driverless-1.0.2/tests/test_driverless.py
```

### Comparing `selenium_driverless-1.0.1/LICENSE.md` & `selenium_driverless-1.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.0.1/PKG-INFO` & `selenium_driverless-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selenium_driverless
-Version: 1.0.1
+Version: 1.0.2
 Summary: Undetected selenium without chromedriver usage
 Home-page: https://github.com/kaliiiiiiiiii/Selenium-Driverless
 Author: Aurin Aegerter
 Author-email: aurinliun@gmx.ch
 Project-URL: Documentation, https://github.com/kaliiiiiiiiii/Selenium-Driverless
 Project-URL: Bug Reports, https://github.com/kaliiiiiiiiii/Selenium-Driverless/issues
 Project-URL: Source Code, https://github.com/kaliiiiiiiiii/Selenium-Driverless
```

### Comparing `selenium_driverless-1.0.1/README.md` & `selenium_driverless-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.0.1/build_upload.md` & `selenium_driverless-1.0.2/build_upload.md`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.0.1/setup.py` & `selenium_driverless-1.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.0.1/src/selenium_driverless/scripts/multi_thread.py` & `selenium_driverless-1.0.2/src/selenium_driverless/scripts/multi_thread.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.0.1/src/selenium_driverless/scripts/options.py` & `selenium_driverless-1.0.2/src/selenium_driverless/scripts/options.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.0.1/src/selenium_driverless/utils/utils.py` & `selenium_driverless-1.0.2/src/selenium_driverless/utils/utils.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.0.1/src/selenium_driverless.egg-info/PKG-INFO` & `selenium_driverless-1.0.2/src/selenium_driverless.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selenium-driverless
-Version: 1.0.1
+Version: 1.0.2
 Summary: Undetected selenium without chromedriver usage
 Home-page: https://github.com/kaliiiiiiiiii/Selenium-Driverless
 Author: Aurin Aegerter
 Author-email: aurinliun@gmx.ch
 Project-URL: Documentation, https://github.com/kaliiiiiiiiii/Selenium-Driverless
 Project-URL: Bug Reports, https://github.com/kaliiiiiiiiii/Selenium-Driverless/issues
 Project-URL: Source Code, https://github.com/kaliiiiiiiiii/Selenium-Driverless
```

### Comparing `selenium_driverless-1.0.1/src/selenium_driverless.egg-info/SOURCES.txt` & `selenium_driverless-1.0.2/src/selenium_driverless.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -8,13 +8,17 @@
 src/selenium_driverless/__init__.py
 src/selenium_driverless/webdriver.py
 src/selenium_driverless.egg-info/PKG-INFO
 src/selenium_driverless.egg-info/SOURCES.txt
 src/selenium_driverless.egg-info/dependency_links.txt
 src/selenium_driverless.egg-info/requires.txt
 src/selenium_driverless.egg-info/top_level.txt
+src/selenium_driverless/async_/__init__.py
+src/selenium_driverless/async_/mobile.py
+src/selenium_driverless/async_/webdriver.py
 src/selenium_driverless/files/__init__.py
 src/selenium_driverless/scripts/__init__.py
 src/selenium_driverless/scripts/multi_thread.py
 src/selenium_driverless/scripts/options.py
+src/selenium_driverless/utils/__init__.py
 src/selenium_driverless/utils/utils.py
 tests/test_driverless.py
```

### Comparing `selenium_driverless-1.0.1/tests/test_driverless.py` & `selenium_driverless-1.0.2/tests/test_driverless.py`

 * *Files identical despite different names*

