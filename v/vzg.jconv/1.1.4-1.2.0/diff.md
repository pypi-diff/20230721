# Comparing `tmp/vzg.jconv-1.1.4.tar.gz` & `tmp/vzg.jconv-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vzg.jconv-1.1.4.tar", last modified: Wed Mar  8 09:21:00 2023, max compression
+gzip compressed data, was "vzg.jconv-1.2.0.tar", last modified: Fri Jul 21 15:39:31 2023, max compression
```

## Comparing `vzg.jconv-1.1.4.tar` & `vzg.jconv-1.2.0.tar`

### file list

```diff
@@ -1,51 +1,53 @@
-drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-03-08 09:21:00.573890 vzg.jconv-1.1.4/
--rw-rw-r--   0 teg       (1000) teg       (1000)    34520 2020-02-07 11:02:19.000000 vzg.jconv-1.1.4/LICENSE.txt
--rw-rw-r--   0 teg       (1000) teg       (1000)      149 2020-02-08 11:53:49.000000 vzg.jconv-1.1.4/MANIFEST.in
--rw-rw-r--   0 teg       (1000) teg       (1000)      843 2023-03-08 09:21:00.573890 vzg.jconv-1.1.4/PKG-INFO
--rw-rw-r--   0 teg       (1000) teg       (1000)      463 2023-02-16 10:38:51.000000 vzg.jconv-1.1.4/README.md
--rw-rw-r--   0 teg       (1000) teg       (1000)        6 2023-03-08 09:18:56.000000 vzg.jconv-1.1.4/VERSION.txt
--rw-rw-r--   0 teg       (1000) teg       (1000)       38 2023-03-08 09:21:00.573890 vzg.jconv-1.1.4/setup.cfg
--rw-rw-r--   0 teg       (1000) teg       (1000)     1679 2023-02-16 10:38:51.000000 vzg.jconv-1.1.4/setup.py
-drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-03-08 09:21:00.569890 vzg.jconv-1.1.4/src/
-drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-03-08 09:21:00.573890 vzg.jconv-1.1.4/src/vzg/
--rw-rw-r--   0 teg       (1000) teg       (1000)       80 2020-11-05 11:14:17.000000 vzg.jconv-1.1.4/src/vzg/__init__.py
-drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-03-08 09:21:00.573890 vzg.jconv-1.1.4/src/vzg/jconv/
--rw-rw-r--   0 teg       (1000) teg       (1000)      275 2020-02-07 09:30:55.000000 vzg.jconv-1.1.4/src/vzg/jconv/__init__.py
-drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-03-08 09:21:00.573890 vzg.jconv-1.1.4/src/vzg/jconv/converter/
--rw-rw-r--   0 teg       (1000) teg       (1000)      378 2020-02-07 13:03:16.000000 vzg.jconv-1.1.4/src/vzg/jconv/converter/__init__.py
--rw-rw-r--   0 teg       (1000) teg       (1000)    20291 2023-03-08 09:06:13.000000 vzg.jconv-1.1.4/src/vzg/jconv/converter/jats.py
--rw-rw-r--   0 teg       (1000) teg       (1000)      450 2020-07-07 11:26:12.000000 vzg.jconv-1.1.4/src/vzg/jconv/errors.py
--rw-rw-r--   0 teg       (1000) teg       (1000)     1091 2023-02-16 10:38:51.000000 vzg.jconv-1.1.4/src/vzg/jconv/gapi.py
--rw-rw-r--   0 teg       (1000) teg       (1000)      875 2020-02-08 12:51:55.000000 vzg.jconv-1.1.4/src/vzg/jconv/interfaces.py
-drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-03-08 09:21:00.573890 vzg.jconv-1.1.4/src/vzg/jconv/langcode/
--rw-rw-r--   0 teg       (1000) teg       (1000)     1156 2020-02-07 12:48:06.000000 vzg.jconv-1.1.4/src/vzg/jconv/langcode/__init__.py
--rw-rw-r--   0 teg       (1000) teg       (1000)    11245 2020-02-07 12:11:08.000000 vzg.jconv-1.1.4/src/vzg/jconv/langcode/language-codes.json
-drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-03-08 09:21:00.573890 vzg.jconv-1.1.4/src/vzg/jconv/person/
--rw-rw-r--   0 teg       (1000) teg       (1000)     5949 2023-03-08 09:15:09.000000 vzg.jconv-1.1.4/src/vzg/jconv/person/__init__.py
-drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-03-08 09:21:00.573890 vzg.jconv-1.1.4/src/vzg/jconv/publisher/
--rw-rw-r--   0 teg       (1000) teg       (1000)     1231 2023-02-16 10:38:51.000000 vzg.jconv-1.1.4/src/vzg/jconv/publisher/__init__.py
--rw-rw-r--   0 teg       (1000) teg       (1000)      263 2020-07-02 08:39:22.000000 vzg.jconv-1.1.4/src/vzg/jconv/publisher/publisher-codes.json
-drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-03-08 09:21:00.573890 vzg.jconv-1.1.4/src/vzg/jconv/schema/
--rw-rw-r--   0 teg       (1000) teg       (1000)    17321 2022-01-14 16:28:18.000000 vzg.jconv-1.1.4/src/vzg/jconv/schema/article_schema.json
-drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-03-08 09:21:00.573890 vzg.jconv-1.1.4/src/vzg/jconv/test/
--rw-rw-r--   0 teg       (1000) teg       (1000)      960 2020-02-11 12:04:12.000000 vzg.jconv-1.1.4/src/vzg/jconv/test/__init__.py
--rw-rw-r--   0 teg       (1000) teg       (1000)     6046 2023-02-16 12:12:31.000000 vzg.jconv-1.1.4/src/vzg/jconv/test/test_jats_article.py
--rw-rw-r--   0 teg       (1000) teg       (1000)     2733 2023-02-16 10:38:51.000000 vzg.jconv-1.1.4/src/vzg/jconv/test/test_jats_converter.py
--rw-rw-r--   0 teg       (1000) teg       (1000)     1038 2020-02-11 12:04:12.000000 vzg.jconv-1.1.4/src/vzg/jconv/test/test_langcode.py
--rw-rw-r--   0 teg       (1000) teg       (1000)     2803 2023-02-16 12:17:30.000000 vzg.jconv-1.1.4/src/vzg/jconv/test/test_person.py
--rw-rw-r--   0 teg       (1000) teg       (1000)     1029 2020-07-02 09:05:29.000000 vzg.jconv-1.1.4/src/vzg/jconv/test/test_publisher.py
-drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-03-08 09:21:00.573890 vzg.jconv-1.1.4/src/vzg/jconv/tools/
--rw-rw-r--   0 teg       (1000) teg       (1000)      378 2020-02-12 10:22:25.000000 vzg.jconv-1.1.4/src/vzg/jconv/tools/__init__.py
--rw-rw-r--   0 teg       (1000) teg       (1000)     6790 2023-02-16 12:40:49.000000 vzg.jconv-1.1.4/src/vzg/jconv/tools/simple_conv.py
-drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-03-08 09:21:00.573890 vzg.jconv-1.1.4/src/vzg/jconv/utils/
--rw-rw-r--   0 teg       (1000) teg       (1000)     2571 2023-02-16 12:17:30.000000 vzg.jconv-1.1.4/src/vzg/jconv/utils/__init__.py
--rw-rw-r--   0 teg       (1000) teg       (1000)     1644 2020-09-25 10:34:55.000000 vzg.jconv-1.1.4/src/vzg/jconv/utils/date.py
-drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-03-08 09:21:00.573890 vzg.jconv-1.1.4/src/vzg.jconv.egg-info/
--rw-rw-r--   0 teg       (1000) teg       (1000)      843 2023-03-08 09:21:00.000000 vzg.jconv-1.1.4/src/vzg.jconv.egg-info/PKG-INFO
--rw-rw-r--   0 teg       (1000) teg       (1000)     1138 2023-03-08 09:21:00.000000 vzg.jconv-1.1.4/src/vzg.jconv.egg-info/SOURCES.txt
--rw-rw-r--   0 teg       (1000) teg       (1000)        1 2023-03-08 09:21:00.000000 vzg.jconv-1.1.4/src/vzg.jconv.egg-info/dependency_links.txt
--rw-rw-r--   0 teg       (1000) teg       (1000)       65 2023-03-08 09:21:00.000000 vzg.jconv-1.1.4/src/vzg.jconv.egg-info/entry_points.txt
--rw-rw-r--   0 teg       (1000) teg       (1000)        4 2023-03-08 09:21:00.000000 vzg.jconv-1.1.4/src/vzg.jconv.egg-info/namespace_packages.txt
--rw-rw-r--   0 teg       (1000) teg       (1000)        1 2020-02-07 10:31:14.000000 vzg.jconv-1.1.4/src/vzg.jconv.egg-info/not-zip-safe
--rw-rw-r--   0 teg       (1000) teg       (1000)       48 2023-03-08 09:21:00.000000 vzg.jconv-1.1.4/src/vzg.jconv.egg-info/requires.txt
--rw-rw-r--   0 teg       (1000) teg       (1000)        4 2023-03-08 09:21:00.000000 vzg.jconv-1.1.4/src/vzg.jconv.egg-info/top_level.txt
+drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-07-21 15:39:31.545384 vzg.jconv-1.2.0/
+-rw-rw-r--   0 teg       (1000) teg       (1000)    34520 2020-02-07 11:02:19.000000 vzg.jconv-1.2.0/LICENSE.txt
+-rw-rw-r--   0 teg       (1000) teg       (1000)      149 2020-02-08 11:53:49.000000 vzg.jconv-1.2.0/MANIFEST.in
+-rw-rw-r--   0 teg       (1000) teg       (1000)      815 2023-07-21 15:39:31.545384 vzg.jconv-1.2.0/PKG-INFO
+-rw-rw-r--   0 teg       (1000) teg       (1000)      463 2023-02-16 10:38:51.000000 vzg.jconv-1.2.0/README.md
+-rw-rw-r--   0 teg       (1000) teg       (1000)        6 2023-07-21 15:36:56.000000 vzg.jconv-1.2.0/VERSION.txt
+-rw-rw-r--   0 teg       (1000) teg       (1000)       38 2023-07-21 15:39:31.545384 vzg.jconv-1.2.0/setup.cfg
+-rw-rw-r--   0 teg       (1000) teg       (1000)     1679 2023-02-16 10:38:51.000000 vzg.jconv-1.2.0/setup.py
+drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-07-21 15:39:31.541384 vzg.jconv-1.2.0/src/
+drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-07-21 15:39:31.545384 vzg.jconv-1.2.0/src/vzg/
+-rw-rw-r--   0 teg       (1000) teg       (1000)       80 2020-11-05 11:14:17.000000 vzg.jconv-1.2.0/src/vzg/__init__.py
+drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-07-21 15:39:31.545384 vzg.jconv-1.2.0/src/vzg/jconv/
+-rw-rw-r--   0 teg       (1000) teg       (1000)      275 2020-02-07 09:30:55.000000 vzg.jconv-1.2.0/src/vzg/jconv/__init__.py
+drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-07-21 15:39:31.545384 vzg.jconv-1.2.0/src/vzg/jconv/converter/
+-rw-rw-r--   0 teg       (1000) teg       (1000)      378 2020-02-07 13:03:16.000000 vzg.jconv-1.2.0/src/vzg/jconv/converter/__init__.py
+-rw-rw-r--   0 teg       (1000) teg       (1000)    22021 2023-07-21 15:36:18.000000 vzg.jconv-1.2.0/src/vzg/jconv/converter/jats.py
+-rw-rw-r--   0 teg       (1000) teg       (1000)      450 2020-07-07 11:26:12.000000 vzg.jconv-1.2.0/src/vzg/jconv/errors.py
+-rw-rw-r--   0 teg       (1000) teg       (1000)     1192 2023-07-21 15:36:18.000000 vzg.jconv-1.2.0/src/vzg/jconv/gapi.py
+-rw-rw-r--   0 teg       (1000) teg       (1000)      875 2020-02-08 12:51:55.000000 vzg.jconv-1.2.0/src/vzg/jconv/interfaces.py
+drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-07-21 15:39:31.545384 vzg.jconv-1.2.0/src/vzg/jconv/langcode/
+-rw-rw-r--   0 teg       (1000) teg       (1000)     1156 2020-02-07 12:48:06.000000 vzg.jconv-1.2.0/src/vzg/jconv/langcode/__init__.py
+-rw-rw-r--   0 teg       (1000) teg       (1000)    11245 2020-02-07 12:11:08.000000 vzg.jconv-1.2.0/src/vzg/jconv/langcode/language-codes.json
+drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-07-21 15:39:31.545384 vzg.jconv-1.2.0/src/vzg/jconv/person/
+-rw-rw-r--   0 teg       (1000) teg       (1000)     5949 2023-03-08 09:15:09.000000 vzg.jconv-1.2.0/src/vzg/jconv/person/__init__.py
+drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-07-21 15:39:31.545384 vzg.jconv-1.2.0/src/vzg/jconv/publisher/
+-rw-rw-r--   0 teg       (1000) teg       (1000)     1231 2023-02-16 10:38:51.000000 vzg.jconv-1.2.0/src/vzg/jconv/publisher/__init__.py
+-rw-rw-r--   0 teg       (1000) teg       (1000)      263 2020-07-02 08:39:22.000000 vzg.jconv-1.2.0/src/vzg/jconv/publisher/publisher-codes.json
+drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-07-21 15:39:31.545384 vzg.jconv-1.2.0/src/vzg/jconv/schema/
+-rw-rw-r--   0 teg       (1000) teg       (1000)    17321 2022-01-14 16:28:18.000000 vzg.jconv-1.2.0/src/vzg/jconv/schema/article_schema.json
+drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-07-21 15:39:31.545384 vzg.jconv-1.2.0/src/vzg/jconv/test/
+-rw-rw-r--   0 teg       (1000) teg       (1000)      960 2020-02-11 12:04:12.000000 vzg.jconv-1.2.0/src/vzg/jconv/test/__init__.py
+-rw-rw-r--   0 teg       (1000) teg       (1000)     1218 2023-07-21 09:37:23.000000 vzg.jconv-1.2.0/src/vzg/jconv/test/conftest.py
+-rw-rw-r--   0 teg       (1000) teg       (1000)     6068 2023-07-21 15:36:18.000000 vzg.jconv-1.2.0/src/vzg/jconv/test/test_jats_article.py
+-rw-rw-r--   0 teg       (1000) teg       (1000)     3151 2023-07-21 15:36:18.000000 vzg.jconv-1.2.0/src/vzg/jconv/test/test_jats_converter.py
+-rw-rw-r--   0 teg       (1000) teg       (1000)     4936 2023-07-21 15:36:18.000000 vzg.jconv-1.2.0/src/vzg/jconv/test/test_jats_degruyter.py
+-rw-rw-r--   0 teg       (1000) teg       (1000)     1038 2020-02-11 12:04:12.000000 vzg.jconv-1.2.0/src/vzg/jconv/test/test_langcode.py
+-rw-rw-r--   0 teg       (1000) teg       (1000)     2803 2023-02-16 12:17:30.000000 vzg.jconv-1.2.0/src/vzg/jconv/test/test_person.py
+-rw-rw-r--   0 teg       (1000) teg       (1000)     1029 2020-07-02 09:05:29.000000 vzg.jconv-1.2.0/src/vzg/jconv/test/test_publisher.py
+drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-07-21 15:39:31.545384 vzg.jconv-1.2.0/src/vzg/jconv/tools/
+-rw-rw-r--   0 teg       (1000) teg       (1000)      378 2020-02-12 10:22:25.000000 vzg.jconv-1.2.0/src/vzg/jconv/tools/__init__.py
+-rw-rw-r--   0 teg       (1000) teg       (1000)     6790 2023-02-16 12:40:49.000000 vzg.jconv-1.2.0/src/vzg/jconv/tools/simple_conv.py
+drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-07-21 15:39:31.545384 vzg.jconv-1.2.0/src/vzg/jconv/utils/
+-rw-rw-r--   0 teg       (1000) teg       (1000)     2571 2023-07-20 10:01:19.000000 vzg.jconv-1.2.0/src/vzg/jconv/utils/__init__.py
+-rw-rw-r--   0 teg       (1000) teg       (1000)     1644 2020-09-25 10:34:55.000000 vzg.jconv-1.2.0/src/vzg/jconv/utils/date.py
+drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-07-21 15:39:31.545384 vzg.jconv-1.2.0/src/vzg.jconv.egg-info/
+-rw-rw-r--   0 teg       (1000) teg       (1000)      815 2023-07-21 15:39:31.000000 vzg.jconv-1.2.0/src/vzg.jconv.egg-info/PKG-INFO
+-rw-rw-r--   0 teg       (1000) teg       (1000)     1211 2023-07-21 15:39:31.000000 vzg.jconv-1.2.0/src/vzg.jconv.egg-info/SOURCES.txt
+-rw-rw-r--   0 teg       (1000) teg       (1000)        1 2023-07-21 15:39:31.000000 vzg.jconv-1.2.0/src/vzg.jconv.egg-info/dependency_links.txt
+-rw-rw-r--   0 teg       (1000) teg       (1000)       64 2023-07-21 15:39:31.000000 vzg.jconv-1.2.0/src/vzg.jconv.egg-info/entry_points.txt
+-rw-rw-r--   0 teg       (1000) teg       (1000)        4 2023-07-21 15:39:31.000000 vzg.jconv-1.2.0/src/vzg.jconv.egg-info/namespace_packages.txt
+-rw-rw-r--   0 teg       (1000) teg       (1000)        1 2020-02-07 10:31:14.000000 vzg.jconv-1.2.0/src/vzg.jconv.egg-info/not-zip-safe
+-rw-rw-r--   0 teg       (1000) teg       (1000)       48 2023-07-21 15:39:31.000000 vzg.jconv-1.2.0/src/vzg.jconv.egg-info/requires.txt
+-rw-rw-r--   0 teg       (1000) teg       (1000)        4 2023-07-21 15:39:31.000000 vzg.jconv-1.2.0/src/vzg.jconv.egg-info/top_level.txt
```

### Comparing `vzg.jconv-1.1.4/LICENSE.txt` & `vzg.jconv-1.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vzg.jconv-1.1.4/PKG-INFO` & `vzg.jconv-1.2.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,20 @@
 Metadata-Version: 2.1
 Name: vzg.jconv
-Version: 1.1.4
+Version: 1.2.0
 Summary: Python library to create JSON Data
 Home-page: https://github.com/gbv/vzg.jconv
 Author: Marc-J. Tegethoff
 Author-email: tegethoff@gbv.de
 License: GNU Affero General Public License v3
 Project-URL: PyPI, https://pypi.python.org/pypi/vzg.jconv
 Project-URL: Source, https://github.com/gbv/vzg.jconv
 Project-URL: Tracker, https://github.com/gbv/vzg.jconv/issues
 Keywords: VZG Python JSON XML JAST
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Requires-Python: >=3.10
 License-File: LICENSE.txt
-
-UNKNOWN
-
```

### Comparing `vzg.jconv-1.1.4/setup.py` & `vzg.jconv-1.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `vzg.jconv-1.1.4/src/vzg/jconv/converter/jats.py` & `vzg.jconv-1.2.0/src/vzg/jconv/converter/jats.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from zope.interface import implementer
 from vzg.jconv.interfaces import IArticle
 from vzg.jconv.interfaces import IConverter
 from vzg.jconv.gapi import NAMESPACES
 from vzg.jconv.gapi import JSON_SCHEMA
 from vzg.jconv.gapi import JATS_SPRINGER_PUBTYPE
 from vzg.jconv.gapi import JATS_SPRINGER_JOURNALTYPE
+from vzg.jconv.gapi import PUBTYPE_SOURCES
 from vzg.jconv.langcode import ISO_639
 from vzg.jconv.publisher import getPublisherId
 from vzg.jconv.errors import NoPublisherError
 from vzg.jconv.utils import node2text
 from vzg.jconv.utils import flatten_line
 from vzg.jconv.utils.date import JatsDate
 from lxml import etree
@@ -29,16 +30,21 @@
 import jsonschema
 
 __author__ = """Marc-J. Tegethoff <marc.tegethoff@gbv.de>"""
 __docformat__ = "plaintext"
 
 JATS_XPATHS = {}
 JATS_XPATHS["lang_code"] = "//article-meta/title-group/article-title/@xml:lang"
+JATS_XPATHS["primary_lang_code"] = "//article/@xml:lang"
 JATS_XPATHS["journal-title"] = "//journal-meta/journal-title-group/journal-title/text()"
 JATS_XPATHS["pub-date"] = """//article-meta/pub-date[@date-type="{pubtype}"]"""
+JATS_XPATHS["pub-date-pubtype"] = """//article-meta/pub-date[@pub-type]"""
+JATS_XPATHS[
+    "pub-date-pubtype-val"
+] = """//article-meta/pub-date[@pub-type="{pubtype}"]"""
 JATS_XPATHS[
     "pub-date-format"
 ] = """//article-meta/pub-date[@publication-format="{pubtype}"]"""
 JATS_XPATHS["pub-date-year"] = JATS_XPATHS["pub-date"] + """/year/text()"""
 JATS_XPATHS[
     "primary_id"
 ] = """//article-meta/article-id[@pub-id-type="publisher-id"]/text()"""
@@ -97,19 +103,27 @@
         Set or override the publisher entry
 
     Returns
     -------
     None
     """
 
-    def __init__(self, dom, pubtype, iso639=None, publisher=None):
+    def __init__(
+        self,
+        dom,
+        pubtype,
+        iso639=None,
+        publisher=None,
+        pubtype_source=PUBTYPE_SOURCES.basic,
+    ):
         self.dom = dom
         self.iso639 = ISO_639() if isinstance(iso639, type(None)) else iso639
         self.pubtype = pubtype
         self.publisher = publisher
+        self.pubtype_source = pubtype_source
 
     @property
     def abstracts(self):
         """Article abstracts"""
 
         logger = logging.getLogger(__name__)
 
@@ -190,15 +204,15 @@
 
         return dateOfProduction
 
     @property
     def lang_code(self):
         """Article lang_code"""
         logger = logging.getLogger(__name__)
-        attributes = self.xpath(JATS_XPATHS["lang_code"])
+        attributes = self.xpath(JATS_XPATHS["primary_lang_code"])
         lcode = []
 
         try:
             lcode.append(self.iso639.i1toi2[attributes[0]])
         except (IndexError, KeyError):
             logger.debug("no lang_code")
 
@@ -207,22 +221,21 @@
     @property
     def journal_date(self):
         """Look for the earliest date"""
         logger = logging.getLogger(__name__)
 
         date_node = None
 
-        expression = JATS_XPATHS["pub-date"].format(pubtype="pub")
-        nodes = self.dom.xpath(expression, namespaces=NAMESPACES)
-        basictype = len(nodes) > 0
-
         for pubtype in JATS_SPRINGER_PUBTYPE:
-            if basictype:
-                logger.debug("new pub")
+            if self.pubtype_source == PUBTYPE_SOURCES.springer:
                 expression = JATS_XPATHS["pub-date-format"].format(pubtype=pubtype.name)
+            elif self.pubtype_source == PUBTYPE_SOURCES.degruyter:
+                expression = JATS_XPATHS["pub-date-pubtype-val"].format(
+                    pubtype=pubtype.value
+                )
             else:
                 expression = JATS_XPATHS["pub-date"].format(pubtype=pubtype.value)
 
             node = self.dom.xpath(expression, namespaces=NAMESPACES)
 
             if len(node) > 0:
                 dnode = JatsDate(node[0])
@@ -240,21 +253,29 @@
         """Article journal"""
         logger = logging.getLogger(__name__)
 
         pdict = {"title": "", "year": "", "journal_ids": []}
 
         jids = {
             "emerald": [JATS_XPATHS["journal-id"].format(journaltype="publisher")],
-            "springer": [JATS_XPATHS["journal-id"].format(journaltype="publisher-id")],
+            "basic": [JATS_XPATHS["journal-id"].format(journaltype="publisher-id")],
             "doi": [JATS_XPATHS["journal-id"].format(journaltype="doi")],
-            self.pubtype.value: [
+        }
+
+        if self.pubtype_source == PUBTYPE_SOURCES.degruyter:
+            jids[JATS_SPRINGER_PUBTYPE.electronic.value] = [
+                JATS_XPATHS["journal-issn"].format(
+                    pubtype=JATS_SPRINGER_PUBTYPE.electronic.value
+                )
+            ]
+        else:
+            jids[self.pubtype.value] = [
                 JATS_XPATHS["journal-issn"].format(pubtype=self.pubtype.value),
                 JATS_XPATHS["journal-issn-pformat"].format(pubtype=self.pubtype.name),
-            ],
-        }
+            ]
 
         expression = JATS_XPATHS["journal-title"]
         node = self.xpath(expression)
         try:
             pdict["title"] = node[0].strip()
         except IndexError:
             logger.debug("no journal title")
@@ -276,14 +297,19 @@
                 if len(node) == 0:
                     msg = f"no {jtype} journal_id ({self.pubtype.value})"
                     logger.debug(msg)
                     continue
 
                 jid = {"type": jtype, "id": node[0]}
 
+                if jtype == "basic":
+                    jid["type"] = "springer"
+                    if self.pubtype_source == PUBTYPE_SOURCES.degruyter:
+                        jid["type"] = "degruyter"
+
                 if jid["type"] in JATS_SPRINGER_JOURNALTYPE.__members__:
                     jid["type"] = JATS_SPRINGER_JOURNALTYPE[jid["type"]].value
 
                 pdict["journal_ids"].append(jid)
 
         publisher = {}
 
@@ -605,14 +631,15 @@
     []
     """
 
     def __init__(self, jatspath, iso639=None, publisher=None, validate=False):
         self.jatspath = jatspath
         self.articles = []
         self.publisher = publisher
+        self.pubtype_source = PUBTYPE_SOURCES.basic
 
         if not self.jatspath.is_file():
             raise OSError
 
         with open(self.jatspath, "rb") as fh:
             self.dom = etree.parse(fh)
 
@@ -629,22 +656,35 @@
 
         Springer sets the date-type attribute to certain values
         """
         logger = logging.getLogger(__name__)
 
         pubtypes = []
 
+        # Springer
         expression = JATS_XPATHS["pub-date"].format(pubtype="pub")
         nodes = self.dom.xpath(expression, namespaces=NAMESPACES)
-        basictype = len(nodes) > 0
+        if len(nodes) > 0:
+            self.pubtype_source = PUBTYPE_SOURCES.springer
+
+        # deGruyter
+        if self.pubtype_source == PUBTYPE_SOURCES.basic:
+            expression = JATS_XPATHS["pub-date-pubtype"]
+            nodes = self.dom.xpath(expression, namespaces=NAMESPACES)
+            if len(nodes) > 0:
+                self.pubtype_source = PUBTYPE_SOURCES.degruyter
 
         for entry in JATS_SPRINGER_PUBTYPE:
-            if basictype:
+            if self.pubtype_source == PUBTYPE_SOURCES.springer:
                 logger.debug("new pub")
                 expression = JATS_XPATHS["pub-date-format"].format(pubtype=entry.name)
+            elif self.pubtype_source == PUBTYPE_SOURCES.degruyter:
+                expression = JATS_XPATHS["pub-date-pubtype-val"].format(
+                    pubtype=entry.value
+                )
             else:
                 expression = JATS_XPATHS["pub-date"].format(pubtype=entry.value)
 
             nodes = self.dom.xpath(expression, namespaces=NAMESPACES)
 
             if len(nodes) > 0:
                 pubtypes.append(entry)
@@ -653,16 +693,21 @@
 
         return pubtypes
 
     def run(self):
         """"""
         logger = logging.getLogger(__name__)
 
+        if self.dom.docinfo.root_name != "article":
+            return None
+
         for pubtype in self.pubtypes:
-            article = JatsArticle(self.dom, pubtype, self.iso639, self.publisher)
+            article = JatsArticle(
+                self.dom, pubtype, self.iso639, self.publisher, self.pubtype_source
+            )
 
             if self.validate:
                 try:
                     jsonschema.validate(instance=article.jdict, schema=JSON_SCHEMA)
                     self.articles.append(article)
                 except jsonschema.ValidationError as Exc:
                     logger.info(Exc, exc_info=False)
```

### Comparing `vzg.jconv-1.1.4/src/vzg/jconv/gapi.py` & `vzg.jconv-1.2.0/src/vzg/jconv/gapi.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # Copyright (c) 2020 Verbundzentrale des GBV.
 # All Rights Reserved.
 #
 ##############################################################################
 """
 
 # Imports
-from enum import Enum
+from enum import Enum, auto
 from pathlib import Path
 import json
 
 __author__ = """Marc-J. Tegethoff <marc.tegethoff@gbv.de>"""
 __docformat__ = "plaintext"
 
 
@@ -50,7 +50,13 @@
 
 
 class PERSON_ID_TYPES(Enum):
     """"""
 
     orcid = "orcid"
     unknown = "unknown"
+
+
+class PUBTYPE_SOURCES(Enum):
+    basic = auto()
+    degruyter = auto()
+    springer = auto()
```

### Comparing `vzg.jconv-1.1.4/src/vzg/jconv/interfaces.py` & `vzg.jconv-1.2.0/src/vzg/jconv/interfaces.py`

 * *Files identical despite different names*

### Comparing `vzg.jconv-1.1.4/src/vzg/jconv/langcode/__init__.py` & `vzg.jconv-1.2.0/src/vzg/jconv/langcode/__init__.py`

 * *Files identical despite different names*

### Comparing `vzg.jconv-1.1.4/src/vzg/jconv/langcode/language-codes.json` & `vzg.jconv-1.2.0/src/vzg/jconv/langcode/language-codes.json`

 * *Files identical despite different names*

### Comparing `vzg.jconv-1.1.4/src/vzg/jconv/person/__init__.py` & `vzg.jconv-1.2.0/src/vzg/jconv/person/__init__.py`

 * *Files identical despite different names*

### Comparing `vzg.jconv-1.1.4/src/vzg/jconv/publisher/__init__.py` & `vzg.jconv-1.2.0/src/vzg/jconv/publisher/__init__.py`

 * *Files identical despite different names*

### Comparing `vzg.jconv-1.1.4/src/vzg/jconv/schema/article_schema.json` & `vzg.jconv-1.2.0/src/vzg/jconv/schema/article_schema.json`

 * *Files identical despite different names*

### Comparing `vzg.jconv-1.1.4/src/vzg/jconv/test/__init__.py` & `vzg.jconv-1.2.0/src/vzg/jconv/test/__init__.py`

 * *Files identical despite different names*

### Comparing `vzg.jconv-1.1.4/src/vzg/jconv/test/test_jats_article.py` & `vzg.jconv-1.2.0/src/vzg/jconv/test/test_jats_article.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 ##############################################################################
 """
 
 # Imports
 import unittest
 import logging
 from vzg.jconv.converter.jats import JatsArticle
-from vzg.jconv.gapi import JATS_SPRINGER_PUBTYPE
+from vzg.jconv.gapi import JATS_SPRINGER_PUBTYPE, PUBTYPE_SOURCES
 from pathlib import Path
 import json
 from lxml import etree
 
 __author__ = """Marc-J. Tegethoff <marc.tegethoff@gbv.de>"""
 __docformat__ = "plaintext"
 
@@ -36,15 +36,19 @@
 
         with open(self.jpath) as fh:
             self.testdata = json.load(fh)
 
         with open(self.fpath, "rb") as fh:
             self.dom = etree.parse(fh)
 
-        self.jobj = JatsArticle(self.dom, JATS_SPRINGER_PUBTYPE.electronic)
+        self.jobj = JatsArticle(
+            self.dom,
+            JATS_SPRINGER_PUBTYPE.electronic,
+            pubtype_source=PUBTYPE_SOURCES.basic,
+        )
 
     def tearDown(self):
         unittest.TestCase.tearDown(self)
 
     def test01(self):
         """title"""
         self.assertEqual(self.jobj.title, self.testdata["title"], "title")
@@ -106,15 +110,19 @@
 
         with open(self.jpath) as fh:
             self.testdata = json.load(fh)
 
         with open(self.fpath, "rb") as fh:
             self.dom = etree.parse(fh)
 
-        self.jobj = JatsArticle(self.dom, JATS_SPRINGER_PUBTYPE.print)
+        self.jobj = JatsArticle(
+            self.dom,
+            JATS_SPRINGER_PUBTYPE.print,
+            pubtype_source=PUBTYPE_SOURCES.basic,
+        )
 
     def tearDown(self):
         unittest.TestCase.tearDown(self)
 
     def test01(self):
         """title"""
         self.assertEqual(self.jobj.title, self.testdata["title"], "title")
@@ -197,13 +205,7 @@
         self.assertEqual(self.jobj.lang_code, self.testdata["lang_code"], "lang_code")
 
     def test03(self):
         """primary_id"""
         self.assertEqual(
             self.jobj.primary_id, self.testdata["primary_id"], "primary_id"
         )
-
-
-if __name__ == "__main__":
-    suite = unittest.TestSuite()
-    suite.addTest(unittest.makeSuite(EPubArticle))
-    unittest.TextTestRunner(verbosity=2).run(suite)
```

### Comparing `vzg.jconv-1.1.4/src/vzg/jconv/test/test_jats_converter.py` & `vzg.jconv-1.2.0/src/vzg/jconv/test/test_jats_converter.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,43 +1,48 @@
 # -*- coding: UTF-8 -*-
 """Beschreibung
 
 ##############################################################################
 #
-# Copyright (c) 2020 Verbundzentrale des GBV.
+# Copyright (c) 2020-2023 Verbundzentrale des GBV.
 # All Rights Reserved.
 #
 ##############################################################################
 """
 
 # Imports
 import sys
 import unittest
 import logging
 from pathlib import Path
 from vzg.jconv.converter.jats import JatsConverter
 from vzg.jconv.converter.jats import JatsArticle
 from lxml import etree
-from pprint import pprint
+
 
 __author__ = """Marc-J. Tegethoff <marc.tegethoff@gbv.de>"""
 __docformat__ = "plaintext"
 
 logger = logging.getLogger(__name__)
 logger.level = logging.INFO
 # stream_handler = logging.StreamHandler(sys.stdout)
 # logger.addHandler(stream_handler)
 
 
-class TestCase(unittest.TestCase):
+class AricleConverter(unittest.TestCase):
     def setUp(self):
         unittest.TestCase.setUp(self)
 
-        self.fpath = Path("data/tests/springer/article.xml")
-        self.fpaths = {"emerald": Path("data/tests/emerald/article_emerald.xml")}
+        self.fpaths = {
+            "emerald": Path("data/tests/emerald/article_emerald.xml"),
+            "degruyter": Path("data/tests/degruyter/article.xml"),
+            "springer": Path("data/tests/springer/article.xml"),
+        }
+
+        self.fpath = self.fpaths["springer"]
 
     def tearDown(self):
         unittest.TestCase.tearDown(self)
 
     def test01(self):
         """Wrong path"""
         tpath = Path("sddsdsds.xml")
@@ -73,29 +78,39 @@
 
         jconv.run()
 
         self.assertTrue(len(jconv.articles) == 2, "articles")
 
         for article in jconv.articles:
             self.assertIsInstance(article, JatsArticle, "article")
-            # pprint(article.json)
 
     def test05(self):
         """validate emerald"""
         jconv = JatsConverter(self.fpaths["emerald"], validate=True)
 
         self.assertTrue(len(jconv.articles) == 0, "articles")
 
         jconv.run()
 
         self.assertTrue(len(jconv.articles) == 1, "articles")
 
         for article in jconv.articles:
             self.assertIsInstance(article, JatsArticle, "article")
-            # pprint(article.jdict)
-            # print(article.json)
+
+    def test06(self):
+        """validate degruyter"""
+        jconv = JatsConverter(self.fpaths["degruyter"], validate=True)
+
+        self.assertTrue(len(jconv.articles) == 0, "articles")
+
+        jconv.run()
+
+        self.assertTrue(len(jconv.articles) == 2, "articles")
+
+        for article in jconv.articles:
+            self.assertIsInstance(article, JatsArticle, "article")
 
 
-if __name__ == "__main__":
-    suite = unittest.TestSuite()
-    suite.addTest(unittest.makeSuite(TestCase))
-    unittest.TextTestRunner(verbosity=2).run(suite)
+# if __name__ == "__main__":
+#     suite = unittest.TestSuite()
+#     suite.addTest(unittest.makeSuite(AricleConverter))
+#     unittest.TextTestRunner(verbosity=2).run(suite)
```

### Comparing `vzg.jconv-1.1.4/src/vzg/jconv/test/test_langcode.py` & `vzg.jconv-1.2.0/src/vzg/jconv/test/test_langcode.py`

 * *Files identical despite different names*

### Comparing `vzg.jconv-1.1.4/src/vzg/jconv/test/test_person.py` & `vzg.jconv-1.2.0/src/vzg/jconv/test/test_person.py`

 * *Files identical despite different names*

### Comparing `vzg.jconv-1.1.4/src/vzg/jconv/test/test_publisher.py` & `vzg.jconv-1.2.0/src/vzg/jconv/test/test_publisher.py`

 * *Files identical despite different names*

### Comparing `vzg.jconv-1.1.4/src/vzg/jconv/tools/simple_conv.py` & `vzg.jconv-1.2.0/src/vzg/jconv/tools/simple_conv.py`

 * *Files identical despite different names*

### Comparing `vzg.jconv-1.1.4/src/vzg/jconv/utils/__init__.py` & `vzg.jconv-1.2.0/src/vzg/jconv/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `vzg.jconv-1.1.4/src/vzg/jconv/utils/date.py` & `vzg.jconv-1.2.0/src/vzg/jconv/utils/date.py`

 * *Files identical despite different names*

### Comparing `vzg.jconv-1.1.4/src/vzg.jconv.egg-info/PKG-INFO` & `vzg.jconv-1.2.0/src/vzg.jconv.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,20 @@
 Metadata-Version: 2.1
 Name: vzg.jconv
-Version: 1.1.4
+Version: 1.2.0
 Summary: Python library to create JSON Data
 Home-page: https://github.com/gbv/vzg.jconv
 Author: Marc-J. Tegethoff
 Author-email: tegethoff@gbv.de
 License: GNU Affero General Public License v3
 Project-URL: PyPI, https://pypi.python.org/pypi/vzg.jconv
 Project-URL: Source, https://github.com/gbv/vzg.jconv
 Project-URL: Tracker, https://github.com/gbv/vzg.jconv/issues
 Keywords: VZG Python JSON XML JAST
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Requires-Python: >=3.10
 License-File: LICENSE.txt
-
-UNKNOWN
-
```

### Comparing `vzg.jconv-1.1.4/src/vzg.jconv.egg-info/SOURCES.txt` & `vzg.jconv-1.2.0/src/vzg.jconv.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -22,16 +22,18 @@
 src/vzg/jconv/langcode/__init__.py
 src/vzg/jconv/langcode/language-codes.json
 src/vzg/jconv/person/__init__.py
 src/vzg/jconv/publisher/__init__.py
 src/vzg/jconv/publisher/publisher-codes.json
 src/vzg/jconv/schema/article_schema.json
 src/vzg/jconv/test/__init__.py
+src/vzg/jconv/test/conftest.py
 src/vzg/jconv/test/test_jats_article.py
 src/vzg/jconv/test/test_jats_converter.py
+src/vzg/jconv/test/test_jats_degruyter.py
 src/vzg/jconv/test/test_langcode.py
 src/vzg/jconv/test/test_person.py
 src/vzg/jconv/test/test_publisher.py
 src/vzg/jconv/tools/__init__.py
 src/vzg/jconv/tools/simple_conv.py
 src/vzg/jconv/utils/__init__.py
 src/vzg/jconv/utils/date.py
```

