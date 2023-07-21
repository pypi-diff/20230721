# Comparing `tmp/YahooRequests-0.1.5.1.tar.gz` & `tmp/YahooRequests-0.1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "YahooRequests-0.1.5.1.tar", last modified: Thu Jul 20 21:25:44 2023, max compression
+gzip compressed data, was "YahooRequests-0.1.5.2.tar", last modified: Fri Jul 21 11:57:31 2023, max compression
```

## Comparing `YahooRequests-0.1.5.1.tar` & `YahooRequests-0.1.5.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-20 21:25:44.264103 YahooRequests-0.1.5.1/
--rw-rw-rw-   0        0        0     1092 2023-07-19 12:31:31.000000 YahooRequests-0.1.5.1/LICENSE
--rw-rw-rw-   0        0        0     1092 2023-07-19 12:31:19.000000 YahooRequests-0.1.5.1/LICENSE.txt
--rw-rw-rw-   0        0        0     1656 2023-07-20 21:25:44.264103 YahooRequests-0.1.5.1/PKG-INFO
--rw-rw-rw-   0        0        0      738 2023-07-19 22:16:56.000000 YahooRequests-0.1.5.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-20 21:25:44.255107 YahooRequests-0.1.5.1/YahooRequests.egg-info/
--rw-rw-rw-   0        0        0     1656 2023-07-20 21:25:44.000000 YahooRequests-0.1.5.1/YahooRequests.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      329 2023-07-20 21:25:44.000000 YahooRequests-0.1.5.1/YahooRequests.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-20 21:25:44.000000 YahooRequests-0.1.5.1/YahooRequests.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-07-20 21:25:44.000000 YahooRequests-0.1.5.1/YahooRequests.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2023-07-20 21:25:44.000000 YahooRequests-0.1.5.1/YahooRequests.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-20 21:25:44.000000 YahooRequests-0.1.5.1/YahooRequests.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      492 2023-07-20 21:25:44.269115 YahooRequests-0.1.5.1/setup.cfg
--rw-rw-rw-   0        0        0     1263 2023-07-20 21:25:18.000000 YahooRequests-0.1.5.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-20 21:25:44.262111 YahooRequests-0.1.5.1/yahoorequests/
--rw-rw-rw-   0        0        0       73 2023-07-20 21:20:43.000000 YahooRequests-0.1.5.1/yahoorequests/__init__.py
--rw-rw-rw-   0        0        0     2178 2023-07-19 13:18:08.000000 YahooRequests-0.1.5.1/yahoorequests/yahoorequests.py
+drwxrwxrwx   0        0        0        0 2023-07-21 11:57:31.144018 YahooRequests-0.1.5.2/
+-rw-rw-rw-   0        0        0     1092 2023-07-19 12:31:31.000000 YahooRequests-0.1.5.2/LICENSE
+-rw-rw-rw-   0        0        0     1092 2023-07-19 12:31:19.000000 YahooRequests-0.1.5.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     1656 2023-07-21 11:57:31.145020 YahooRequests-0.1.5.2/PKG-INFO
+-rw-rw-rw-   0        0        0      738 2023-07-19 22:16:56.000000 YahooRequests-0.1.5.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-21 11:57:31.122048 YahooRequests-0.1.5.2/YahooRequests.egg-info/
+-rw-rw-rw-   0        0        0     1656 2023-07-21 11:57:30.000000 YahooRequests-0.1.5.2/YahooRequests.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      329 2023-07-21 11:57:30.000000 YahooRequests-0.1.5.2/YahooRequests.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 11:57:30.000000 YahooRequests-0.1.5.2/YahooRequests.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-07-21 11:57:30.000000 YahooRequests-0.1.5.2/YahooRequests.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2023-07-21 11:57:30.000000 YahooRequests-0.1.5.2/YahooRequests.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-21 11:57:30.000000 YahooRequests-0.1.5.2/YahooRequests.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      492 2023-07-21 11:57:31.152050 YahooRequests-0.1.5.2/setup.cfg
+-rw-rw-rw-   0        0        0     1281 2023-07-21 11:56:28.000000 YahooRequests-0.1.5.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 11:57:31.141019 YahooRequests-0.1.5.2/yahoorequests/
+-rw-rw-rw-   0        0        0       73 2023-07-20 21:20:43.000000 YahooRequests-0.1.5.2/yahoorequests/__init__.py
+-rw-rw-rw-   0        0        0     2178 2023-07-19 13:18:08.000000 YahooRequests-0.1.5.2/yahoorequests/yahoorequests.py
```

### Comparing `YahooRequests-0.1.5.1/LICENSE` & `YahooRequests-0.1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `YahooRequests-0.1.5.1/LICENSE.txt` & `YahooRequests-0.1.5.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `YahooRequests-0.1.5.1/PKG-INFO` & `YahooRequests-0.1.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: YahooRequests
-Version: 0.1.5.1
+Version: 0.1.5.2
 Summary: A simple Python library for getting stock prices and company names from Yahoo Finance.
 Home-page: https://github.com/TheodorGajhede/YahooRequests
 Download-URL: https://github.com/TheodorGajhede/YahooRequests/archive/refs/tags/0.1.5.tar.gz
 Author: Theodor Gajhede
 Author-email: theodorgajhede@gmail.com
 License: MIT
 Keywords: Stocks,Ticker,Yahoo
```

### Comparing `YahooRequests-0.1.5.1/README.md` & `YahooRequests-0.1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `YahooRequests-0.1.5.1/YahooRequests.egg-info/PKG-INFO` & `YahooRequests-0.1.5.2/YahooRequests.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: YahooRequests
-Version: 0.1.5.1
+Version: 0.1.5.2
 Summary: A simple Python library for getting stock prices and company names from Yahoo Finance.
 Home-page: https://github.com/TheodorGajhede/YahooRequests
 Download-URL: https://github.com/TheodorGajhede/YahooRequests/archive/refs/tags/0.1.5.tar.gz
 Author: Theodor Gajhede
 Author-email: theodorgajhede@gmail.com
 License: MIT
 Keywords: Stocks,Ticker,Yahoo
```

### Comparing `YahooRequests-0.1.5.1/setup.py` & `YahooRequests-0.1.5.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from distutils.core import setup
 setup(
     name='YahooRequests',
     packages=['yahoorequests'],
-    version='0.1.5.1',
+    version='0.1.5.2',
+    chmod=0o644,
     license='MIT',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     description='A simple Python library for getting stock prices and company names from Yahoo Finance.',
     author='Theodor Gajhede',
     author_email='theodorgajhede@gmail.com',
     url='https://github.com/TheodorGajhede/YahooRequests',
```

### Comparing `YahooRequests-0.1.5.1/yahoorequests/yahoorequests.py` & `YahooRequests-0.1.5.2/yahoorequests/yahoorequests.py`

 * *Files identical despite different names*

