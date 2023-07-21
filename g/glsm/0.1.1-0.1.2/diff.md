# Comparing `tmp/glsm-0.1.1.tar.gz` & `tmp/glsm-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glsm-0.1.1.tar", last modified: Fri Jun 30 03:36:26 2023, max compression
+gzip compressed data, was "glsm-0.1.2.tar", last modified: Fri Jul 21 19:45:43 2023, max compression
```

## Comparing `glsm-0.1.1.tar` & `glsm-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0 valar     (1000) valar     (1000)        0 2023-06-30 03:36:26.984862 glsm-0.1.1/
--rwxrwxrwx   0 valar     (1000) valar     (1000)     1091 2023-04-09 23:14:04.000000 glsm-0.1.1/LICENSE
--rwxrwxrwx   0 valar     (1000) valar     (1000)    15753 2023-06-30 03:36:26.981852 glsm-0.1.1/PKG-INFO
--rwxrwxrwx   0 valar     (1000) valar     (1000)    15086 2023-06-30 03:23:43.000000 glsm-0.1.1/README.md
-drwxrwxrwx   0 valar     (1000) valar     (1000)        0 2023-06-30 03:36:26.876275 glsm-0.1.1/glsm/
--rwxrwxrwx   0 valar     (1000) valar     (1000)        0 2023-03-30 19:17:50.000000 glsm-0.1.1/glsm/__init__.py
-drwxrwxrwx   0 valar     (1000) valar     (1000)        0 2023-06-30 03:36:26.962233 glsm-0.1.1/glsm.egg-info/
--rwxrwxrwx   0 valar     (1000) valar     (1000)    15753 2023-06-30 03:36:26.000000 glsm-0.1.1/glsm.egg-info/PKG-INFO
--rwxrwxrwx   0 valar     (1000) valar     (1000)      182 2023-06-30 03:36:26.000000 glsm-0.1.1/glsm.egg-info/SOURCES.txt
--rwxrwxrwx   0 valar     (1000) valar     (1000)        1 2023-06-30 03:36:26.000000 glsm-0.1.1/glsm.egg-info/dependency_links.txt
--rwxrwxrwx   0 valar     (1000) valar     (1000)      231 2023-06-30 03:36:26.000000 glsm-0.1.1/glsm.egg-info/requires.txt
--rwxrwxrwx   0 valar     (1000) valar     (1000)        5 2023-06-30 03:36:26.000000 glsm-0.1.1/glsm.egg-info/top_level.txt
--rwxrwxrwx   0 valar     (1000) valar     (1000)       38 2023-06-30 03:36:26.985864 glsm-0.1.1/setup.cfg
--rwxrwxrwx   0 valar     (1000) valar     (1000)     1552 2023-06-30 03:36:00.000000 glsm-0.1.1/setup.py
+drwxrwxrwx   0 valar     (1000) valar     (1000)        0 2023-07-21 19:45:43.526543 glsm-0.1.2/
+-rwxrwxrwx   0 valar     (1000) valar     (1000)     1091 2023-04-09 23:14:04.000000 glsm-0.1.2/LICENSE
+-rwxrwxrwx   0 valar     (1000) valar     (1000)    15753 2023-07-21 19:45:43.524539 glsm-0.1.2/PKG-INFO
+-rwxrwxrwx   0 valar     (1000) valar     (1000)    15086 2023-06-30 03:23:43.000000 glsm-0.1.2/README.md
+drwxrwxrwx   0 valar     (1000) valar     (1000)        0 2023-07-21 19:45:43.420488 glsm-0.1.2/glsm/
+-rwxrwxrwx   0 valar     (1000) valar     (1000)        0 2023-03-30 19:17:50.000000 glsm-0.1.2/glsm/__init__.py
+drwxrwxrwx   0 valar     (1000) valar     (1000)        0 2023-07-21 19:45:43.507533 glsm-0.1.2/glsm.egg-info/
+-rwxrwxrwx   0 valar     (1000) valar     (1000)    15753 2023-07-21 19:45:43.000000 glsm-0.1.2/glsm.egg-info/PKG-INFO
+-rwxrwxrwx   0 valar     (1000) valar     (1000)      182 2023-07-21 19:45:43.000000 glsm-0.1.2/glsm.egg-info/SOURCES.txt
+-rwxrwxrwx   0 valar     (1000) valar     (1000)        1 2023-07-21 19:45:43.000000 glsm-0.1.2/glsm.egg-info/dependency_links.txt
+-rwxrwxrwx   0 valar     (1000) valar     (1000)      231 2023-07-21 19:45:43.000000 glsm-0.1.2/glsm.egg-info/requires.txt
+-rwxrwxrwx   0 valar     (1000) valar     (1000)        5 2023-07-21 19:45:43.000000 glsm-0.1.2/glsm.egg-info/top_level.txt
+-rwxrwxrwx   0 valar     (1000) valar     (1000)       38 2023-07-21 19:45:43.527539 glsm-0.1.2/setup.cfg
+-rwxrwxrwx   0 valar     (1000) valar     (1000)     1552 2023-07-21 19:44:31.000000 glsm-0.1.2/setup.py
```

### Comparing `glsm-0.1.1/LICENSE` & `glsm-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `glsm-0.1.1/PKG-INFO` & `glsm-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glsm
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Python package that simplifies the process of building predictive and non-predictive lead scoring models.
 Author: Victor Valar
 Author-email: <valar@victorvalar.me>
 License: LICENSE.txt
 Keywords: python,lead score,modeling,lead generation,lead scoring,lead scoring model
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `glsm-0.1.1/README.md` & `glsm-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `glsm-0.1.1/glsm.egg-info/PKG-INFO` & `glsm-0.1.2/glsm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glsm
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Python package that simplifies the process of building predictive and non-predictive lead scoring models.
 Author: Victor Valar
 Author-email: <valar@victorvalar.me>
 License: LICENSE.txt
 Keywords: python,lead score,modeling,lead generation,lead scoring,lead scoring model
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `glsm-0.1.1/setup.py` & `glsm-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
 with open(requirements_filename) as f:
     INSTALL_REQUIRES = f.read().splitlines()
 
 # EXTRA_REQUIRES = ['pytest']
-VERSION = '0.1.1'
+VERSION = '0.1.2'
 DESCRIPTION = 'A Python package that simplifies the process of building predictive and non-predictive lead scoring ' \
               'models.'
 LONG_DESCRIPTION = long_description
 PACKAGE_LICENSE = 'LICENSE.txt'
 
 # Setting up
 setup(
```

