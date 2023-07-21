# Comparing `tmp/fpingwrppr-0.6.tar.gz` & `tmp/fpingwrppr-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fpingwrppr-0.6.tar", last modified: Fri Jul 21 12:03:52 2023, max compression
+gzip compressed data, was "fpingwrppr-0.7.tar", last modified: Fri Jul 21 12:44:44 2023, max compression
```

## Comparing `fpingwrppr-0.6.tar` & `fpingwrppr-0.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 gabriel   (1000) gabriel   (1000)        0 2023-07-21 12:03:52.343126 fpingwrppr-0.6/
--rw-r--r--   0 gabriel   (1000) gabriel   (1000)      119 2023-07-21 12:03:52.343126 fpingwrppr-0.6/PKG-INFO
-drwxr-xr-x   0 gabriel   (1000) gabriel   (1000)        0 2023-07-21 12:03:52.333127 fpingwrppr-0.6/fping/
--rw-r--r--   0 gabriel   (1000) gabriel   (1000)      751 2023-07-20 20:00:59.000000 fpingwrppr-0.6/fping/__init__.py
-drwxr-xr-x   0 gabriel   (1000) gabriel   (1000)        0 2023-07-21 12:03:52.343126 fpingwrppr-0.6/fping/backends/
--rw-r--r--   0 gabriel   (1000) gabriel   (1000)        2 2023-07-20 17:31:11.000000 fpingwrppr-0.6/fping/backends/__init__.py
--rw-r--r--   0 gabriel   (1000) gabriel   (1000)     1374 2023-07-20 19:54:24.000000 fpingwrppr-0.6/fping/backends/base.py
--rw-r--r--   0 gabriel   (1000) gabriel   (1000)     1413 2023-07-20 20:01:55.000000 fpingwrppr-0.6/fping/backends/fping.py
-drwxr-xr-x   0 gabriel   (1000) gabriel   (1000)        0 2023-07-21 12:03:52.343126 fpingwrppr-0.6/fpingwrppr.egg-info/
--rw-r--r--   0 gabriel   (1000) gabriel   (1000)      119 2023-07-21 12:03:52.000000 fpingwrppr-0.6/fpingwrppr.egg-info/PKG-INFO
--rw-r--r--   0 gabriel   (1000) gabriel   (1000)      317 2023-07-21 12:03:52.000000 fpingwrppr-0.6/fpingwrppr.egg-info/SOURCES.txt
--rw-r--r--   0 gabriel   (1000) gabriel   (1000)        1 2023-07-21 12:03:52.000000 fpingwrppr-0.6/fpingwrppr.egg-info/dependency_links.txt
--rw-r--r--   0 gabriel   (1000) gabriel   (1000)        6 2023-07-21 12:03:52.000000 fpingwrppr-0.6/fpingwrppr.egg-info/top_level.txt
--rw-r--r--   0 gabriel   (1000) gabriel   (1000)        1 2023-07-21 12:03:52.000000 fpingwrppr-0.6/fpingwrppr.egg-info/zip-safe
--rw-r--r--   0 gabriel   (1000) gabriel   (1000)       62 2023-07-21 12:03:52.343126 fpingwrppr-0.6/setup.cfg
--rw-r--r--   0 gabriel   (1000) gabriel   (1000)      630 2023-07-21 12:02:45.000000 fpingwrppr-0.6/setup.py
-drwxr-xr-x   0 gabriel   (1000) gabriel   (1000)        0 2023-07-21 12:03:52.343126 fpingwrppr-0.6/tests/
--rw-r--r--   0 gabriel   (1000) gabriel   (1000)      779 2023-07-20 17:34:56.000000 fpingwrppr-0.6/tests/test_backends.py
--rw-r--r--   0 gabriel   (1000) gabriel   (1000)      293 2023-07-20 17:34:56.000000 fpingwrppr-0.6/tests/test_base.py
+drwxr-xr-x   0 gabriel   (1000) gabriel   (1000)        0 2023-07-21 12:44:44.867707 fpingwrppr-0.7/
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)      119 2023-07-21 12:44:44.867707 fpingwrppr-0.7/PKG-INFO
+drwxr-xr-x   0 gabriel   (1000) gabriel   (1000)        0 2023-07-21 12:44:44.857707 fpingwrppr-0.7/fping/
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)      743 2023-07-21 12:43:14.000000 fpingwrppr-0.7/fping/__init__.py
+drwxr-xr-x   0 gabriel   (1000) gabriel   (1000)        0 2023-07-21 12:44:44.857707 fpingwrppr-0.7/fping/backends/
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)        2 2023-07-20 17:31:11.000000 fpingwrppr-0.7/fping/backends/__init__.py
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)     1370 2023-07-21 12:43:51.000000 fpingwrppr-0.7/fping/backends/base.py
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)     1413 2023-07-20 20:01:55.000000 fpingwrppr-0.7/fping/backends/fping.py
+drwxr-xr-x   0 gabriel   (1000) gabriel   (1000)        0 2023-07-21 12:44:44.867707 fpingwrppr-0.7/fpingwrppr.egg-info/
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)      119 2023-07-21 12:44:44.000000 fpingwrppr-0.7/fpingwrppr.egg-info/PKG-INFO
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)      317 2023-07-21 12:44:44.000000 fpingwrppr-0.7/fpingwrppr.egg-info/SOURCES.txt
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)        1 2023-07-21 12:44:44.000000 fpingwrppr-0.7/fpingwrppr.egg-info/dependency_links.txt
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)        6 2023-07-21 12:44:44.000000 fpingwrppr-0.7/fpingwrppr.egg-info/top_level.txt
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)        1 2023-07-21 12:44:44.000000 fpingwrppr-0.7/fpingwrppr.egg-info/zip-safe
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)       62 2023-07-21 12:44:44.867707 fpingwrppr-0.7/setup.cfg
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)      630 2023-07-21 12:44:26.000000 fpingwrppr-0.7/setup.py
+drwxr-xr-x   0 gabriel   (1000) gabriel   (1000)        0 2023-07-21 12:44:44.867707 fpingwrppr-0.7/tests/
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)      779 2023-07-20 17:34:56.000000 fpingwrppr-0.7/tests/test_backends.py
+-rw-r--r--   0 gabriel   (1000) gabriel   (1000)      293 2023-07-20 17:34:56.000000 fpingwrppr-0.7/tests/test_base.py
```

### Comparing `fpingwrppr-0.6/fping/__init__.py` & `fpingwrppr-0.7/fping/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,16 +11,16 @@
         if b:
             inst = b(**kwargs)
             if inst.is_available():
                 return inst
 
     raise RuntimeError("No pinger backends Available")
 
-def ping_one(host):
-    return get_backend().ping_one(host)
+def ping(host):
+    return get_backend().ping(host)
 
 def ping_many_updown(hosts):
     return get_backend().ping_many_updown(hosts)
 
 def ping_many_updown_iter(hosts):
     return get_backend().ping_many_updown_iter(hosts)
```

### Comparing `fpingwrppr-0.6/fping/backends/base.py` & `fpingwrppr-0.7/fping/backends/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         try :
             p = subprocess.Popen([self.program_path, self.help_argument],stdout=subprocess.PIPE, stderr=subprocess.PIPE)
             p.communicate()
             return p.wait() == self.help_return_code
         except OSError:
             return False
     
-    def ping_one(self, host):
+    def ping(self, host):
         """Ping a single host, return True or False"""
         up = self.ping_many([host])
         return len(up) == 1
 
     def ping_many_updown(self, hosts):
         """Ping many hosts, return a tuple of up hosts, down hosts"""
         raise NotImplementedError()
```

### Comparing `fpingwrppr-0.6/fping/backends/fping.py` & `fpingwrppr-0.7/fping/backends/fping.py`

 * *Files identical despite different names*

### Comparing `fpingwrppr-0.6/setup.py` & `fpingwrppr-0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 import sys, os
 
-version = '0.6'
+version = '0.7'
 
 setup(name='fpingwrppr',
       version=version,
       description="Fping Wrapper",
       long_description="""\
 """,
       classifiers=[], # Get strings from http://pypi.python.org/pypi?%3Aaction=list_classifiers
```

### Comparing `fpingwrppr-0.6/tests/test_backends.py` & `fpingwrppr-0.7/tests/test_backends.py`

 * *Files identical despite different names*

