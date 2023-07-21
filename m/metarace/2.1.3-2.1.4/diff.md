# Comparing `tmp/metarace-2.1.3.tar.gz` & `tmp/metarace-2.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metarace-2.1.3.tar", last modified: Mon Jul 17 05:28:52 2023, max compression
+gzip compressed data, was "metarace-2.1.4.tar", last modified: Fri Jul 21 04:54:02 2023, max compression
```

## Comparing `metarace-2.1.3.tar` & `metarace-2.1.4.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 ndf       (1000) ndf       (1000)        0 2023-07-17 05:28:52.642412 metarace-2.1.3/
--rw-------   0 ndf       (1000) ndf       (1000)     1092 2023-07-11 12:51:50.000000 metarace-2.1.3/LICENSE
--rw-r--r--   0 ndf       (1000) ndf       (1000)       28 2022-05-31 01:20:37.000000 metarace-2.1.3/MANIFEST.in
--rw-r--r--   0 ndf       (1000) ndf       (1000)     4490 2023-07-17 05:28:52.638412 metarace-2.1.3/PKG-INFO
--rw-------   0 ndf       (1000) ndf       (1000)     3921 2023-07-11 12:41:25.000000 metarace-2.1.3/README.md
--rw-r--r--   0 ndf       (1000) ndf       (1000)      798 2023-07-17 05:27:44.000000 metarace-2.1.3/pyproject.toml
--rw-r--r--   0 ndf       (1000) ndf       (1000)       38 2023-07-17 05:28:52.642412 metarace-2.1.3/setup.cfg
-drwxr-xr-x   0 ndf       (1000) ndf       (1000)        0 2023-07-17 05:28:52.630412 metarace-2.1.3/src/
-drwxr-xr-x   0 ndf       (1000) ndf       (1000)        0 2023-07-17 05:28:52.634412 metarace-2.1.3/src/metarace/
--rw-r--r--   0 ndf       (1000) ndf       (1000)     9422 2023-07-17 03:19:05.000000 metarace-2.1.3/src/metarace/__init__.py
--rw-------   0 ndf       (1000) ndf       (1000)     4268 2023-06-25 00:11:43.000000 metarace-2.1.3/src/metarace/countback.py
-drwxr-xr-x   0 ndf       (1000) ndf       (1000)        0 2023-07-17 05:28:52.638412 metarace-2.1.3/src/metarace/data/
--rw-------   0 ndf       (1000) ndf       (1000)     3067 2022-01-22 22:18:40.000000 metarace-2.1.3/src/metarace/data/IOC_Codes.csv
--rw-r--r--   0 ndf       (1000) ndf       (1000)        0 2023-06-28 11:57:11.000000 metarace-2.1.3/src/metarace/data/__init__.py
--rw-r--r--   0 ndf       (1000) ndf       (1000)     1454 2022-01-22 22:18:40.000000 metarace-2.1.3/src/metarace/data/bg_armfin.svg
--rw-r--r--   0 ndf       (1000) ndf       (1000)     1454 2022-01-22 22:18:40.000000 metarace-2.1.3/src/metarace/data/bg_armint.svg
--rw-r--r--   0 ndf       (1000) ndf       (1000)     1454 2022-01-22 22:18:40.000000 metarace-2.1.3/src/metarace/data/bg_armstart.svg
--rw-r--r--   0 ndf       (1000) ndf       (1000)     1454 2022-01-22 22:18:40.000000 metarace-2.1.3/src/metarace/data/bg_idle.svg
--rw-r--r--   0 ndf       (1000) ndf       (1000)     2369 2022-01-22 22:18:40.000000 metarace-2.1.3/src/metarace/data/bg_src.svg
--rw-------   0 ndf       (1000) ndf       (1000)        4 2023-07-11 12:42:36.000000 metarace-2.1.3/src/metarace/data/metarace.json
--rw-------   0 ndf       (1000) ndf       (1000)     8729 2022-01-22 22:18:40.000000 metarace-2.1.3/src/metarace/data/metarace_icon.svg
--rw-------   0 ndf       (1000) ndf       (1000)     2048 2023-06-05 01:23:26.000000 metarace-2.1.3/src/metarace/data/pdf_template.json
-drwxr-xr-x   0 ndf       (1000) ndf       (1000)        0 2023-07-17 05:28:52.638412 metarace-2.1.3/src/metarace/decoder/
--rw-r--r--   0 ndf       (1000) ndf       (1000)     5721 2023-07-13 12:30:30.000000 metarace-2.1.3/src/metarace/decoder/__init__.py
--rw-------   0 ndf       (1000) ndf       (1000)    16233 2023-07-13 12:30:42.000000 metarace-2.1.3/src/metarace/decoder/rrs.py
--rw-------   0 ndf       (1000) ndf       (1000)    32727 2023-07-13 12:35:31.000000 metarace-2.1.3/src/metarace/decoder/rru.py
--rw-------   0 ndf       (1000) ndf       (1000)    25107 2023-07-17 04:57:46.000000 metarace-2.1.3/src/metarace/decoder/thbc.py
--rw-------   0 ndf       (1000) ndf       (1000)    11415 2023-07-13 12:29:27.000000 metarace-2.1.3/src/metarace/eventdb.py
--rw-------   0 ndf       (1000) ndf       (1000)     6290 2023-07-13 12:29:44.000000 metarace-2.1.3/src/metarace/export.py
--rw-------   0 ndf       (1000) ndf       (1000)     5970 2023-06-28 00:17:21.000000 metarace-2.1.3/src/metarace/htlib.py
--rw-------   0 ndf       (1000) ndf       (1000)    12251 2023-07-13 12:30:06.000000 metarace-2.1.3/src/metarace/jsonconfig.py
--rw-------   0 ndf       (1000) ndf       (1000)   204351 2023-07-13 12:29:15.000000 metarace-2.1.3/src/metarace/report.py
--rw-------   0 ndf       (1000) ndf       (1000)    25632 2023-07-16 01:35:36.000000 metarace-2.1.3/src/metarace/riderdb.py
--rw-------   0 ndf       (1000) ndf       (1000)    17918 2023-06-25 00:09:45.000000 metarace-2.1.3/src/metarace/strops.py
--rw-r--r--   0 ndf       (1000) ndf       (1000)    14783 2023-07-13 12:28:46.000000 metarace-2.1.3/src/metarace/telegraph.py
--rw-------   0 ndf       (1000) ndf       (1000)    16903 2023-07-15 05:11:51.000000 metarace-2.1.3/src/metarace/timy.py
--rw-r--r--   0 ndf       (1000) ndf       (1000)    20994 2023-07-13 12:27:42.000000 metarace-2.1.3/src/metarace/tod.py
--rw-------   0 ndf       (1000) ndf       (1000)     4485 2023-06-25 00:09:26.000000 metarace-2.1.3/src/metarace/unt4.py
-drwxr-xr-x   0 ndf       (1000) ndf       (1000)        0 2023-07-17 05:28:52.638412 metarace-2.1.3/src/metarace.egg-info/
--rw-r--r--   0 ndf       (1000) ndf       (1000)     4490 2023-07-17 05:28:52.000000 metarace-2.1.3/src/metarace.egg-info/PKG-INFO
--rw-r--r--   0 ndf       (1000) ndf       (1000)      969 2023-07-17 05:28:52.000000 metarace-2.1.3/src/metarace.egg-info/SOURCES.txt
--rw-r--r--   0 ndf       (1000) ndf       (1000)        1 2023-07-17 05:28:52.000000 metarace-2.1.3/src/metarace.egg-info/dependency_links.txt
--rw-r--r--   0 ndf       (1000) ndf       (1000)       67 2023-07-17 05:28:52.000000 metarace-2.1.3/src/metarace.egg-info/requires.txt
--rw-r--r--   0 ndf       (1000) ndf       (1000)        9 2023-07-17 05:28:52.000000 metarace-2.1.3/src/metarace.egg-info/top_level.txt
+drwxr-xr-x   0 ndf       (1000) ndf       (1000)        0 2023-07-21 04:54:02.231471 metarace-2.1.4/
+-rw-------   0 ndf       (1000) ndf       (1000)     1092 2023-07-11 12:51:50.000000 metarace-2.1.4/LICENSE
+-rw-r--r--   0 ndf       (1000) ndf       (1000)       28 2022-05-31 01:20:37.000000 metarace-2.1.4/MANIFEST.in
+-rw-r--r--   0 ndf       (1000) ndf       (1000)     4490 2023-07-21 04:54:02.231471 metarace-2.1.4/PKG-INFO
+-rw-------   0 ndf       (1000) ndf       (1000)     3921 2023-07-11 12:41:25.000000 metarace-2.1.4/README.md
+-rw-r--r--   0 ndf       (1000) ndf       (1000)      798 2023-07-21 04:52:20.000000 metarace-2.1.4/pyproject.toml
+-rw-r--r--   0 ndf       (1000) ndf       (1000)       38 2023-07-21 04:54:02.231471 metarace-2.1.4/setup.cfg
+drwxr-xr-x   0 ndf       (1000) ndf       (1000)        0 2023-07-21 04:54:02.215471 metarace-2.1.4/src/
+drwxr-xr-x   0 ndf       (1000) ndf       (1000)        0 2023-07-21 04:54:02.223471 metarace-2.1.4/src/metarace/
+-rw-r--r--   0 ndf       (1000) ndf       (1000)     9422 2023-07-21 04:52:36.000000 metarace-2.1.4/src/metarace/__init__.py
+-rw-------   0 ndf       (1000) ndf       (1000)     4268 2023-06-25 00:11:43.000000 metarace-2.1.4/src/metarace/countback.py
+drwxr-xr-x   0 ndf       (1000) ndf       (1000)        0 2023-07-21 04:54:02.227471 metarace-2.1.4/src/metarace/data/
+-rw-------   0 ndf       (1000) ndf       (1000)     3067 2022-01-22 22:18:40.000000 metarace-2.1.4/src/metarace/data/IOC_Codes.csv
+-rw-r--r--   0 ndf       (1000) ndf       (1000)        0 2023-06-28 11:57:11.000000 metarace-2.1.4/src/metarace/data/__init__.py
+-rw-r--r--   0 ndf       (1000) ndf       (1000)     1454 2022-01-22 22:18:40.000000 metarace-2.1.4/src/metarace/data/bg_armfin.svg
+-rw-r--r--   0 ndf       (1000) ndf       (1000)     1454 2022-01-22 22:18:40.000000 metarace-2.1.4/src/metarace/data/bg_armint.svg
+-rw-r--r--   0 ndf       (1000) ndf       (1000)     1454 2022-01-22 22:18:40.000000 metarace-2.1.4/src/metarace/data/bg_armstart.svg
+-rw-r--r--   0 ndf       (1000) ndf       (1000)     1454 2022-01-22 22:18:40.000000 metarace-2.1.4/src/metarace/data/bg_idle.svg
+-rw-r--r--   0 ndf       (1000) ndf       (1000)     2369 2022-01-22 22:18:40.000000 metarace-2.1.4/src/metarace/data/bg_src.svg
+-rw-------   0 ndf       (1000) ndf       (1000)        4 2023-07-11 12:42:36.000000 metarace-2.1.4/src/metarace/data/metarace.json
+-rw-------   0 ndf       (1000) ndf       (1000)     8729 2022-01-22 22:18:40.000000 metarace-2.1.4/src/metarace/data/metarace_icon.svg
+-rw-------   0 ndf       (1000) ndf       (1000)     2048 2023-06-05 01:23:26.000000 metarace-2.1.4/src/metarace/data/pdf_template.json
+drwxr-xr-x   0 ndf       (1000) ndf       (1000)        0 2023-07-21 04:54:02.227471 metarace-2.1.4/src/metarace/decoder/
+-rw-r--r--   0 ndf       (1000) ndf       (1000)     5721 2023-07-13 12:30:30.000000 metarace-2.1.4/src/metarace/decoder/__init__.py
+-rw-------   0 ndf       (1000) ndf       (1000)    16233 2023-07-13 12:30:42.000000 metarace-2.1.4/src/metarace/decoder/rrs.py
+-rw-------   0 ndf       (1000) ndf       (1000)    32745 2023-07-21 01:34:17.000000 metarace-2.1.4/src/metarace/decoder/rru.py
+-rw-------   0 ndf       (1000) ndf       (1000)    25107 2023-07-17 04:57:46.000000 metarace-2.1.4/src/metarace/decoder/thbc.py
+-rw-------   0 ndf       (1000) ndf       (1000)    11415 2023-07-13 12:29:27.000000 metarace-2.1.4/src/metarace/eventdb.py
+-rw-------   0 ndf       (1000) ndf       (1000)     6290 2023-07-13 12:29:44.000000 metarace-2.1.4/src/metarace/export.py
+-rw-------   0 ndf       (1000) ndf       (1000)     5970 2023-06-28 00:17:21.000000 metarace-2.1.4/src/metarace/htlib.py
+-rw-------   0 ndf       (1000) ndf       (1000)    12251 2023-07-13 12:30:06.000000 metarace-2.1.4/src/metarace/jsonconfig.py
+-rw-------   0 ndf       (1000) ndf       (1000)   204351 2023-07-13 12:29:15.000000 metarace-2.1.4/src/metarace/report.py
+-rw-------   0 ndf       (1000) ndf       (1000)    25632 2023-07-16 01:35:36.000000 metarace-2.1.4/src/metarace/riderdb.py
+-rw-------   0 ndf       (1000) ndf       (1000)    17984 2023-07-19 07:30:40.000000 metarace-2.1.4/src/metarace/strops.py
+-rw-r--r--   0 ndf       (1000) ndf       (1000)    14783 2023-07-13 12:28:46.000000 metarace-2.1.4/src/metarace/telegraph.py
+-rw-------   0 ndf       (1000) ndf       (1000)    16903 2023-07-15 05:11:51.000000 metarace-2.1.4/src/metarace/timy.py
+-rw-r--r--   0 ndf       (1000) ndf       (1000)    20994 2023-07-13 12:27:42.000000 metarace-2.1.4/src/metarace/tod.py
+-rw-------   0 ndf       (1000) ndf       (1000)     4485 2023-06-25 00:09:26.000000 metarace-2.1.4/src/metarace/unt4.py
+drwxr-xr-x   0 ndf       (1000) ndf       (1000)        0 2023-07-21 04:54:02.223471 metarace-2.1.4/src/metarace.egg-info/
+-rw-r--r--   0 ndf       (1000) ndf       (1000)     4490 2023-07-21 04:54:02.000000 metarace-2.1.4/src/metarace.egg-info/PKG-INFO
+-rw-r--r--   0 ndf       (1000) ndf       (1000)      969 2023-07-21 04:54:02.000000 metarace-2.1.4/src/metarace.egg-info/SOURCES.txt
+-rw-r--r--   0 ndf       (1000) ndf       (1000)        1 2023-07-21 04:54:02.000000 metarace-2.1.4/src/metarace.egg-info/dependency_links.txt
+-rw-r--r--   0 ndf       (1000) ndf       (1000)       67 2023-07-21 04:54:02.000000 metarace-2.1.4/src/metarace.egg-info/requires.txt
+-rw-r--r--   0 ndf       (1000) ndf       (1000)        9 2023-07-21 04:54:02.000000 metarace-2.1.4/src/metarace.egg-info/top_level.txt
```

### Comparing `metarace-2.1.3/LICENSE` & `metarace-2.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `metarace-2.1.3/PKG-INFO` & `metarace-2.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metarace
-Version: 2.1.3
+Version: 2.1.4
 Summary: Cyclesport results and timing toolkit
 Author-email: Nathan Fraser <ndf-zz@6-v.org>
 License: MIT
 Project-URL: homepage, https://github.com/ndf-zz/metarace
 Keywords: cyclesport,results,timing
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Other/Nonlisted Topic
```

### Comparing `metarace-2.1.3/README.md` & `metarace-2.1.4/README.md`

 * *Files identical despite different names*

### Comparing `metarace-2.1.3/pyproject.toml` & `metarace-2.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=62"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "metarace"
-version = "2.1.3"
+version = "2.1.4"
 description = "Cyclesport results and timing toolkit"
 readme = "README.md"
 requires-python = ">=3.9"
 license = {text = "MIT"}
 keywords = ["cyclesport", "results", "timing"]
 authors = [
     {email = "ndf-zz@6-v.org", name = "Nathan Fraser"}
```

### Comparing `metarace-2.1.3/src/metarace/__init__.py` & `metarace-2.1.4/src/metarace/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from shutil import copyfile
 from metarace import jsonconfig
 try:
     from importlib.resources import files, as_file
 except ImportError:
     print('Python >= 3.9 is required to use this module')
 
-VERSION = '2.1.3'
+VERSION = '2.1.4'
 DATA_PATH = os.path.realpath(
     os.path.expanduser(os.path.join('~', 'Documents', 'metarace')))
 DEFAULTS_PATH = os.path.join(DATA_PATH, 'default')
 RESOURCE_PKG = 'metarace.data'
 LOGO = 'metarace_icon.svg'
 SYSCONF = 'metarace.json'
 PDF_TEMPLATE = 'pdf_template.json'
```

### Comparing `metarace-2.1.3/src/metarace/countback.py` & `metarace-2.1.4/src/metarace/countback.py`

 * *Files identical despite different names*

### Comparing `metarace-2.1.3/src/metarace/data/IOC_Codes.csv` & `metarace-2.1.4/src/metarace/data/IOC_Codes.csv`

 * *Files identical despite different names*

### Comparing `metarace-2.1.3/src/metarace/data/bg_armfin.svg` & `metarace-2.1.4/src/metarace/data/bg_armfin.svg`

 * *Files identical despite different names*

### Comparing `metarace-2.1.3/src/metarace/data/bg_armint.svg` & `metarace-2.1.4/src/metarace/data/bg_armint.svg`

 * *Files identical despite different names*

### Comparing `metarace-2.1.3/src/metarace/data/bg_armstart.svg` & `metarace-2.1.4/src/metarace/data/bg_armstart.svg`

 * *Files identical despite different names*

### Comparing `metarace-2.1.3/src/metarace/data/bg_idle.svg` & `metarace-2.1.4/src/metarace/data/bg_idle.svg`

 * *Files identical despite different names*

### Comparing `metarace-2.1.3/src/metarace/data/bg_src.svg` & `metarace-2.1.4/src/metarace/data/bg_src.svg`

 * *Files identical despite different names*

### Comparing `metarace-2.1.3/src/metarace/data/metarace_icon.svg` & `metarace-2.1.4/src/metarace/data/metarace_icon.svg`

 * *Files identical despite different names*

### Comparing `metarace-2.1.3/src/metarace/data/pdf_template.json` & `metarace-2.1.4/src/metarace/data/pdf_template.json`

 * *Files identical despite different names*

### Comparing `metarace-2.1.3/src/metarace/decoder/__init__.py` & `metarace-2.1.4/src/metarace/decoder/__init__.py`

 * *Files identical despite different names*

### Comparing `metarace-2.1.3/src/metarace/decoder/rrs.py` & `metarace-2.1.4/src/metarace/decoder/rrs.py`

 * *Files identical despite different names*

### Comparing `metarace-2.1.3/src/metarace/decoder/rru.py` & `metarace-2.1.4/src/metarace/decoder/rru.py`

 * *Files 1% similar despite different names*

```diff
@@ -885,15 +885,15 @@
                     else:
                         _log.debug('%r error: %r', self._curreply, mv[1])
             elif mv[0] == 'AUTOBOOT':
                 _log.warning('Re-connecting restarted decoder')
                 self._request_pending = 1
                 self._sane()
             elif 'rrActive' in mv[0]:
-                _log.warning('Decoder reset - waiting for AUTOBOOT')
+                _log.warning('Decoder reset - waiting for it to start')
                 self._request_pending = 1
                 sleep(3.0)
                 self._dump_queue()
             else:
                 if self._curreply is not None:
                     self._handlereply(mv)
 
@@ -963,14 +963,14 @@
                     m = self._cqueue.get()
                 self._cqueue.task_done()
                 self._proccmd(m)
             except queue.Empty:
                 pass
             except serial.SerialException as e:
                 self._close()
-                _log.error('%s: %s', e.__class__.__name__, e)
+                _log.error('%s, decoder disconnected', e.__class__.__name__)
             except Exception as e:
                 _log.critical('%s: %s', e.__class__.__name__, e)
                 self._running = False
                 self._boxname = None
         self.setcb()
         _log.debug('Exiting')
```

### Comparing `metarace-2.1.3/src/metarace/decoder/thbc.py` & `metarace-2.1.4/src/metarace/decoder/thbc.py`

 * *Files identical despite different names*

### Comparing `metarace-2.1.3/src/metarace/eventdb.py` & `metarace-2.1.4/src/metarace/eventdb.py`

 * *Files identical despite different names*

### Comparing `metarace-2.1.3/src/metarace/export.py` & `metarace-2.1.4/src/metarace/export.py`

 * *Files identical despite different names*

### Comparing `metarace-2.1.3/src/metarace/htlib.py` & `metarace-2.1.4/src/metarace/htlib.py`

 * *Files identical despite different names*

### Comparing `metarace-2.1.3/src/metarace/jsonconfig.py` & `metarace-2.1.4/src/metarace/jsonconfig.py`

 * *Files identical despite different names*

### Comparing `metarace-2.1.3/src/metarace/report.py` & `metarace-2.1.4/src/metarace/report.py`

 * *Files identical despite different names*

### Comparing `metarace-2.1.3/src/metarace/riderdb.py` & `metarace-2.1.4/src/metarace/riderdb.py`

 * *Files identical despite different names*

### Comparing `metarace-2.1.3/src/metarace/strops.py` & `metarace-2.1.4/src/metarace/strops.py`

 * *Files 2% similar despite different names*

```diff
@@ -235,15 +235,17 @@
         '3': 'rd',
         '11': 'th',
         '12': 'th',
         '13': 'th'
     }
     ret = place
     if place.isdigit():
-        if len(place) > 1 and place[-2:] in omap:
+        if place in omap:
+            ret = place + omap[place]
+        elif len(place) > 1 and place[-2:] in omap:
             ret = place + omap[place[-2:]]
         else:
             if len(place) > 1 and place[-1] in omap:  # last digit 1,2,3
                 ret = place + omap[place[-1]]
             else:
                 ret = place + 'th'
     return ret
```

### Comparing `metarace-2.1.3/src/metarace/telegraph.py` & `metarace-2.1.4/src/metarace/telegraph.py`

 * *Files identical despite different names*

### Comparing `metarace-2.1.3/src/metarace/timy.py` & `metarace-2.1.4/src/metarace/timy.py`

 * *Files identical despite different names*

### Comparing `metarace-2.1.3/src/metarace/tod.py` & `metarace-2.1.4/src/metarace/tod.py`

 * *Files identical despite different names*

### Comparing `metarace-2.1.3/src/metarace/unt4.py` & `metarace-2.1.4/src/metarace/unt4.py`

 * *Files identical despite different names*

### Comparing `metarace-2.1.3/src/metarace.egg-info/PKG-INFO` & `metarace-2.1.4/src/metarace.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metarace
-Version: 2.1.3
+Version: 2.1.4
 Summary: Cyclesport results and timing toolkit
 Author-email: Nathan Fraser <ndf-zz@6-v.org>
 License: MIT
 Project-URL: homepage, https://github.com/ndf-zz/metarace
 Keywords: cyclesport,results,timing
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Other/Nonlisted Topic
```

### Comparing `metarace-2.1.3/src/metarace.egg-info/SOURCES.txt` & `metarace-2.1.4/src/metarace.egg-info/SOURCES.txt`

 * *Files identical despite different names*

