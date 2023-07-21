# Comparing `tmp/idds-client-1.3.2.tar.gz` & `tmp/idds-client-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idds-client-1.3.2.tar", last modified: Thu Jul 20 14:17:42 2023, max compression
+gzip compressed data, was "idds-client-1.3.3.tar", last modified: Fri Jul 21 07:10:56 2023, max compression
```

## Comparing `idds-client-1.3.2.tar` & `idds-client-1.3.3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:17:42.960405 idds-client-1.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-20 14:17:28.000000 idds-client-1.3.2/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-07-20 14:17:42.964406 idds-client-1.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-20 14:17:28.000000 idds-client-1.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:17:42.960405 idds-client-1.3.2/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)    14109 2023-07-20 14:17:28.000000 idds-client-1.3.2/bin/idds
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:17:42.960405 idds-client-1.3.2/etc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:17:42.960405 idds-client-1.3.2/etc/idds/
--rwxr-xr-x   0 runner    (1001) docker     (123)      649 2023-07-20 14:17:28.000000 idds-client-1.3.2/etc/idds/idds.cfg.client.template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:17:42.960405 idds-client-1.3.2/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:17:42.960405 idds-client-1.3.2/lib/idds/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-20 14:17:28.000000 idds-client-1.3.2/lib/idds/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:17:42.960405 idds-client-1.3.2/lib/idds/client/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-20 14:17:28.000000 idds-client-1.3.2/lib/idds/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-07-20 14:17:28.000000 idds-client-1.3.2/lib/idds/client/authclient.py
--rw-r--r--   0 runner    (1001) docker     (123)    12311 2023-07-20 14:17:28.000000 idds-client-1.3.2/lib/idds/client/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-07-20 14:17:28.000000 idds-client-1.3.2/lib/idds/client/cacherclient.py
--rw-r--r--   0 runner    (1001) docker     (123)     7322 2023-07-20 14:17:28.000000 idds-client-1.3.2/lib/idds/client/catalogclient.py
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-07-20 14:17:28.000000 idds-client-1.3.2/lib/idds/client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    29020 2023-07-20 14:17:28.000000 idds-client-1.3.2/lib/idds/client/clientmanager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-07-20 14:17:28.000000 idds-client-1.3.2/lib/idds/client/hpoclient.py
--rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-07-20 14:17:28.000000 idds-client-1.3.2/lib/idds/client/logsclient.py
--rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-07-20 14:17:28.000000 idds-client-1.3.2/lib/idds/client/messageclient.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-07-20 14:17:28.000000 idds-client-1.3.2/lib/idds/client/pingclient.py
--rw-r--r--   0 runner    (1001) docker     (123)     6849 2023-07-20 14:17:28.000000 idds-client-1.3.2/lib/idds/client/requestclient.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-20 14:17:38.000000 idds-client-1.3.2/lib/idds/client/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:17:42.960405 idds-client-1.3.2/lib/idds_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-07-20 14:17:42.000000 idds-client-1.3.2/lib/idds_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-07-20 14:17:42.000000 idds-client-1.3.2/lib/idds_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 14:17:42.000000 idds-client-1.3.2/lib/idds_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-20 14:17:42.000000 idds-client-1.3.2/lib/idds_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-20 14:17:42.000000 idds-client-1.3.2/lib/idds_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-20 14:17:42.964406 idds-client-1.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-07-20 14:17:28.000000 idds-client-1.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:17:42.960405 idds-client-1.3.2/tools/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:17:42.960405 idds-client-1.3.2/tools/env/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-20 14:17:38.000000 idds-client-1.3.2/tools/env/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:10:56.752869 idds-client-1.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-21 07:10:42.000000 idds-client-1.3.3/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-07-21 07:10:56.752869 idds-client-1.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-21 07:10:42.000000 idds-client-1.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:10:56.752869 idds-client-1.3.3/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14109 2023-07-21 07:10:42.000000 idds-client-1.3.3/bin/idds
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:10:56.752869 idds-client-1.3.3/etc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:10:56.752869 idds-client-1.3.3/etc/idds/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      649 2023-07-21 07:10:42.000000 idds-client-1.3.3/etc/idds/idds.cfg.client.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:10:56.752869 idds-client-1.3.3/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:10:56.752869 idds-client-1.3.3/lib/idds/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-21 07:10:42.000000 idds-client-1.3.3/lib/idds/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:10:56.752869 idds-client-1.3.3/lib/idds/client/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-21 07:10:42.000000 idds-client-1.3.3/lib/idds/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-07-21 07:10:42.000000 idds-client-1.3.3/lib/idds/client/authclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12311 2023-07-21 07:10:42.000000 idds-client-1.3.3/lib/idds/client/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-07-21 07:10:42.000000 idds-client-1.3.3/lib/idds/client/cacherclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7322 2023-07-21 07:10:42.000000 idds-client-1.3.3/lib/idds/client/catalogclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-07-21 07:10:42.000000 idds-client-1.3.3/lib/idds/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29020 2023-07-21 07:10:42.000000 idds-client-1.3.3/lib/idds/client/clientmanager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-07-21 07:10:42.000000 idds-client-1.3.3/lib/idds/client/hpoclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-07-21 07:10:42.000000 idds-client-1.3.3/lib/idds/client/logsclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-07-21 07:10:42.000000 idds-client-1.3.3/lib/idds/client/messageclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-07-21 07:10:42.000000 idds-client-1.3.3/lib/idds/client/pingclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6849 2023-07-21 07:10:42.000000 idds-client-1.3.3/lib/idds/client/requestclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-21 07:10:52.000000 idds-client-1.3.3/lib/idds/client/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:10:56.752869 idds-client-1.3.3/lib/idds_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-07-21 07:10:56.000000 idds-client-1.3.3/lib/idds_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-07-21 07:10:56.000000 idds-client-1.3.3/lib/idds_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 07:10:56.000000 idds-client-1.3.3/lib/idds_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-21 07:10:56.000000 idds-client-1.3.3/lib/idds_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-21 07:10:56.000000 idds-client-1.3.3/lib/idds_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-21 07:10:56.752869 idds-client-1.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-07-21 07:10:42.000000 idds-client-1.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:10:56.752869 idds-client-1.3.3/tools/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:10:56.752869 idds-client-1.3.3/tools/env/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-21 07:10:52.000000 idds-client-1.3.3/tools/env/environment.yml
```

### Comparing `idds-client-1.3.2/LICENSE.rst` & `idds-client-1.3.3/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `idds-client-1.3.2/PKG-INFO` & `idds-client-1.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idds-client
-Version: 1.3.2
+Version: 1.3.3
 Summary: intelligent Data Delivery Service(iDDS) Package
 Author: IRIS-HEP Team
 Author-email: atlas-adc-panda@cern.ch
 License: GPL
 Project-URL: Documentation, https://github.com/HSF/iDDS/wiki
 Project-URL: Source, https://github.com/HSF/iDDS
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `idds-client-1.3.2/bin/idds` & `idds-client-1.3.3/bin/idds`

 * *Files identical despite different names*

### Comparing `idds-client-1.3.2/etc/idds/idds.cfg.client.template` & `idds-client-1.3.3/etc/idds/idds.cfg.client.template`

 * *Files identical despite different names*

### Comparing `idds-client-1.3.2/lib/idds/client/authclient.py` & `idds-client-1.3.3/lib/idds/client/authclient.py`

 * *Files identical despite different names*

### Comparing `idds-client-1.3.2/lib/idds/client/base.py` & `idds-client-1.3.3/lib/idds/client/base.py`

 * *Files identical despite different names*

### Comparing `idds-client-1.3.2/lib/idds/client/cacherclient.py` & `idds-client-1.3.3/lib/idds/client/cacherclient.py`

 * *Files identical despite different names*

### Comparing `idds-client-1.3.2/lib/idds/client/catalogclient.py` & `idds-client-1.3.3/lib/idds/client/catalogclient.py`

 * *Files identical despite different names*

### Comparing `idds-client-1.3.2/lib/idds/client/client.py` & `idds-client-1.3.3/lib/idds/client/client.py`

 * *Files identical despite different names*

### Comparing `idds-client-1.3.2/lib/idds/client/clientmanager.py` & `idds-client-1.3.3/lib/idds/client/clientmanager.py`

 * *Files identical despite different names*

### Comparing `idds-client-1.3.2/lib/idds/client/hpoclient.py` & `idds-client-1.3.3/lib/idds/client/hpoclient.py`

 * *Files identical despite different names*

### Comparing `idds-client-1.3.2/lib/idds/client/logsclient.py` & `idds-client-1.3.3/lib/idds/client/logsclient.py`

 * *Files identical despite different names*

### Comparing `idds-client-1.3.2/lib/idds/client/messageclient.py` & `idds-client-1.3.3/lib/idds/client/messageclient.py`

 * *Files identical despite different names*

### Comparing `idds-client-1.3.2/lib/idds/client/pingclient.py` & `idds-client-1.3.3/lib/idds/client/pingclient.py`

 * *Files identical despite different names*

### Comparing `idds-client-1.3.2/lib/idds/client/requestclient.py` & `idds-client-1.3.3/lib/idds/client/requestclient.py`

 * *Files identical despite different names*

### Comparing `idds-client-1.3.2/lib/idds_client.egg-info/PKG-INFO` & `idds-client-1.3.3/lib/idds_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idds-client
-Version: 1.3.2
+Version: 1.3.3
 Summary: intelligent Data Delivery Service(iDDS) Package
 Author: IRIS-HEP Team
 Author-email: atlas-adc-panda@cern.ch
 License: GPL
 Project-URL: Documentation, https://github.com/HSF/iDDS/wiki
 Project-URL: Source, https://github.com/HSF/iDDS
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `idds-client-1.3.2/lib/idds_client.egg-info/SOURCES.txt` & `idds-client-1.3.3/lib/idds_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `idds-client-1.3.2/setup.py` & `idds-client-1.3.3/setup.py`

 * *Files identical despite different names*

