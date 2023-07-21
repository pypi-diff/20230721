# Comparing `tmp/destral-1.7.1.tar.gz` & `tmp/destral-1.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/destral-1.7.1.tar", last modified: Thu Oct 17 11:11:15 2019, max compression
+gzip compressed data, was "dist/destral-1.7.3.tar", last modified: Mon May  4 07:15:01 2020, max compression
```

## Comparing `destral-1.7.1.tar` & `destral-1.7.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 ecarreras  (1000) ecarreras  (1000)        0 2019-10-17 11:11:15.000000 destral-1.7.1/
--rw-r--r--   0 ecarreras  (1000) ecarreras  (1000)      666 2019-10-17 11:10:36.000000 destral-1.7.1/setup.py
--rw-r--r--   0 ecarreras  (1000) ecarreras  (1000)       38 2019-10-17 11:11:15.000000 destral-1.7.1/setup.cfg
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)      514 2016-04-20 15:07:39.000000 destral-1.7.1/README.rst
-drwxr-xr-x   0 ecarreras  (1000) ecarreras  (1000)        0 2019-10-17 11:11:15.000000 destral-1.7.1/destral.egg-info/
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)      102 2019-10-17 11:11:15.000000 destral-1.7.1/destral.egg-info/requires.txt
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)       49 2019-10-17 11:11:15.000000 destral-1.7.1/destral.egg-info/entry_points.txt
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)       13 2019-10-17 11:11:15.000000 destral-1.7.1/destral.egg-info/top_level.txt
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)      241 2019-10-17 11:11:15.000000 destral-1.7.1/destral.egg-info/PKG-INFO
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)      502 2019-10-17 11:11:15.000000 destral-1.7.1/destral.egg-info/SOURCES.txt
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)        1 2019-10-17 11:11:15.000000 destral-1.7.1/destral.egg-info/dependency_links.txt
-drwxr-xr-x   0 ecarreras  (1000) ecarreras  (1000)        0 2019-10-17 11:11:15.000000 destral-1.7.1/destral/
--rw-r--r--   0 ecarreras  (1000) ecarreras  (1000)     7019 2019-10-17 11:10:36.000000 destral-1.7.1/destral/utils.py
--rw-r--r--   0 ecarreras  (1000) ecarreras  (1000)      632 2019-06-19 08:04:29.000000 destral-1.7.1/destral/linter.py
--rw-r--r--   0 ecarreras  (1000) ecarreras  (1000)    13931 2019-10-17 11:10:32.000000 destral-1.7.1/destral/testing.py
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)     2380 2019-07-30 09:30:40.000000 destral-1.7.1/destral/patch.py
--rw-r--r--   0 ecarreras  (1000) ecarreras  (1000)      140 2019-10-17 11:10:36.000000 destral-1.7.1/destral/__init__.py
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)     6136 2018-07-11 10:12:13.000000 destral-1.7.1/destral/openerp.py
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)     2092 2015-09-21 05:57:09.000000 destral-1.7.1/destral/transaction.py
--rw-r--r--   0 ecarreras  (1000) ecarreras  (1000)     6620 2019-10-17 11:10:36.000000 destral-1.7.1/destral/cli.py
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)     7974 2018-03-12 09:35:17.000000 destral-1.7.1/destral/junitxml_testing.py
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)      760 2016-08-29 07:14:32.000000 destral-1.7.1/destral/cover.py
-drwxr-xr-x   0 ecarreras  (1000) ecarreras  (1000)        0 2019-10-17 11:11:15.000000 destral-1.7.1/spec/
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)        0 2016-08-12 10:10:11.000000 destral-1.7.1/spec/__init__.py
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)     1821 2016-08-12 10:10:11.000000 destral-1.7.1/spec/testing_spec.py
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)     3147 2017-07-07 11:19:26.000000 destral-1.7.1/spec/utils_spec.py
-drwxr-xr-x   0 ecarreras  (1000) ecarreras  (1000)        0 2019-10-17 11:11:15.000000 destral-1.7.1/spec/fixtures/
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)      126 2016-08-12 10:10:11.000000 destral-1.7.1/spec/fixtures/__init__.py
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)      522 2017-01-16 15:14:45.000000 destral-1.7.1/spec/patch_spec.py
--rw-r--r--   0 ecarreras  (1000) ecarreras  (1000)      241 2019-10-17 11:11:15.000000 destral-1.7.1/PKG-INFO
+drwxr-xr-x   0 afita     (1000) afita     (1000)        0 2020-05-04 07:15:01.000000 destral-1.7.3/
+-rw-r--r--   0 afita     (1000) afita     (1000)      241 2020-05-04 07:15:01.000000 destral-1.7.3/PKG-INFO
+-rw-r--r--   0 afita     (1000) afita     (1000)       38 2020-05-04 07:15:01.000000 destral-1.7.3/setup.cfg
+-rw-rw-r--   0 afita     (1000) afita     (1000)      666 2020-05-04 07:10:11.000000 destral-1.7.3/setup.py
+drwxr-xr-x   0 afita     (1000) afita     (1000)        0 2020-05-04 07:15:01.000000 destral-1.7.3/destral.egg-info/
+-rw-r--r--   0 afita     (1000) afita     (1000)       13 2020-05-04 07:15:01.000000 destral-1.7.3/destral.egg-info/top_level.txt
+-rw-r--r--   0 afita     (1000) afita     (1000)      502 2020-05-04 07:15:01.000000 destral-1.7.3/destral.egg-info/SOURCES.txt
+-rw-r--r--   0 afita     (1000) afita     (1000)      241 2020-05-04 07:15:01.000000 destral-1.7.3/destral.egg-info/PKG-INFO
+-rw-r--r--   0 afita     (1000) afita     (1000)       49 2020-05-04 07:15:01.000000 destral-1.7.3/destral.egg-info/entry_points.txt
+-rw-r--r--   0 afita     (1000) afita     (1000)        1 2020-05-04 07:15:01.000000 destral-1.7.3/destral.egg-info/dependency_links.txt
+-rw-r--r--   0 afita     (1000) afita     (1000)      102 2020-05-04 07:15:01.000000 destral-1.7.3/destral.egg-info/requires.txt
+-rw-rw-r--   0 afita     (1000) afita     (1000)      514 2020-02-11 09:01:06.000000 destral-1.7.3/README.rst
+drwxr-xr-x   0 afita     (1000) afita     (1000)        0 2020-05-04 07:15:01.000000 destral-1.7.3/destral/
+-rw-rw-r--   0 afita     (1000) afita     (1000)     6620 2020-02-11 09:01:06.000000 destral-1.7.3/destral/cli.py
+-rw-rw-r--   0 afita     (1000) afita     (1000)    13931 2020-02-11 09:01:06.000000 destral-1.7.3/destral/testing.py
+-rw-rw-r--   0 afita     (1000) afita     (1000)     7019 2020-02-11 09:01:06.000000 destral-1.7.3/destral/utils.py
+-rw-rw-r--   0 afita     (1000) afita     (1000)     7974 2020-02-11 09:01:06.000000 destral-1.7.3/destral/junitxml_testing.py
+-rw-rw-r--   0 afita     (1000) afita     (1000)      140 2020-02-11 09:01:06.000000 destral-1.7.3/destral/__init__.py
+-rw-rw-r--   0 afita     (1000) afita     (1000)     2380 2020-02-11 09:01:06.000000 destral-1.7.3/destral/patch.py
+-rw-rw-r--   0 afita     (1000) afita     (1000)      760 2020-02-11 09:01:06.000000 destral-1.7.3/destral/cover.py
+-rw-rw-r--   0 afita     (1000) afita     (1000)     2092 2020-02-11 09:01:06.000000 destral-1.7.3/destral/transaction.py
+-rw-rw-r--   0 afita     (1000) afita     (1000)     6136 2020-02-11 09:01:06.000000 destral-1.7.3/destral/openerp.py
+-rw-rw-r--   0 afita     (1000) afita     (1000)      632 2020-02-11 09:01:06.000000 destral-1.7.3/destral/linter.py
+drwxr-xr-x   0 afita     (1000) afita     (1000)        0 2020-05-04 07:15:01.000000 destral-1.7.3/spec/
+-rw-rw-r--   0 afita     (1000) afita     (1000)     1821 2020-02-11 09:01:06.000000 destral-1.7.3/spec/testing_spec.py
+-rw-rw-r--   0 afita     (1000) afita     (1000)      522 2020-02-11 09:01:06.000000 destral-1.7.3/spec/patch_spec.py
+-rw-rw-r--   0 afita     (1000) afita     (1000)     3147 2020-02-11 09:01:06.000000 destral-1.7.3/spec/utils_spec.py
+-rw-rw-r--   0 afita     (1000) afita     (1000)        0 2020-02-11 09:01:06.000000 destral-1.7.3/spec/__init__.py
+drwxr-xr-x   0 afita     (1000) afita     (1000)        0 2020-05-04 07:15:01.000000 destral-1.7.3/spec/fixtures/
+-rw-rw-r--   0 afita     (1000) afita     (1000)      126 2020-02-11 09:01:06.000000 destral-1.7.3/spec/fixtures/__init__.py
```

### Comparing `destral-1.7.1/setup.py` & `destral-1.7.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='destral',
-    version='1.7.1',
+    version='1.7.3',
     packages=find_packages(),
     url='https://github.com/gisce/destral',
     install_requires=[
         'osconf',
         'expects',
         'six',
         'click',
-        'mamba>=0.9.3',
+        'mamba<0.11.0',
         'coverage',
         'pylint',
         'python-dateutil',
         'babel>=2.4.0',
         'junit_xml',
         'psycopg2',
     ],
```

### Comparing `destral-1.7.1/README.rst` & `destral-1.7.3/README.rst`

 * *Files identical despite different names*

### Comparing `destral-1.7.1/destral/utils.py` & `destral-1.7.3/destral/utils.py`

 * *Files identical despite different names*

### Comparing `destral-1.7.1/destral/linter.py` & `destral-1.7.3/destral/linter.py`

 * *Files identical despite different names*

### Comparing `destral-1.7.1/destral/testing.py` & `destral-1.7.3/destral/testing.py`

 * *Files 0% similar despite different names*

```diff
@@ -183,15 +183,15 @@
     def test_translate_modules(self):
         """
         Test translated strings in the module using the .po and .pot files
         """
 
         from os.path import join, isdir
         from tools import trans_export
-        from cStringIO import StringIO
+        from six.moves import StringIO
         from utils import compare_pofiles, TempDir
 
         if not self.config['testing_langs']:
             logger.warning(
                 'Configuration variable "DESTRAL_TESTING_LANGS" has'
                 ' not been initialized'
             )
```

### Comparing `destral-1.7.1/destral/patch.py` & `destral-1.7.3/destral/patch.py`

 * *Files identical despite different names*

### Comparing `destral-1.7.1/destral/openerp.py` & `destral-1.7.3/destral/openerp.py`

 * *Files identical despite different names*

### Comparing `destral-1.7.1/destral/transaction.py` & `destral-1.7.3/destral/transaction.py`

 * *Files identical despite different names*

### Comparing `destral-1.7.1/destral/cli.py` & `destral-1.7.3/destral/cli.py`

 * *Files identical despite different names*

### Comparing `destral-1.7.1/destral/junitxml_testing.py` & `destral-1.7.3/destral/junitxml_testing.py`

 * *Files identical despite different names*

### Comparing `destral-1.7.1/destral/cover.py` & `destral-1.7.3/destral/cover.py`

 * *Files identical despite different names*

### Comparing `destral-1.7.1/spec/testing_spec.py` & `destral-1.7.3/spec/testing_spec.py`

 * *Files identical despite different names*

### Comparing `destral-1.7.1/spec/utils_spec.py` & `destral-1.7.3/spec/utils_spec.py`

 * *Files identical despite different names*

### Comparing `destral-1.7.1/spec/patch_spec.py` & `destral-1.7.3/spec/patch_spec.py`

 * *Files identical despite different names*

