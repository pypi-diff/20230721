# Comparing `tmp/onlykey-agent-1.1.15.tar.gz` & `tmp/onlykey-agent-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onlykey-agent-1.1.15.tar", last modified: Fri Jul 21 03:39:09 2023, max compression
+gzip compressed data, was "dist/onlykey-agent-1.1.9.tar", last modified: Mon Aug 17 14:03:00 2020, max compression
```

## Comparing `onlykey-agent-1.1.15.tar` & `onlykey-agent-1.1.9.tar`

### file list

```diff
@@ -1,14 +1,13 @@
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-07-21 03:39:09.461454 onlykey-agent-1.1.15/
--rw-r--r--   0 kali      (1000) kali      (1000)     7652 2023-07-21 03:38:26.000000 onlykey-agent-1.1.15/LICENSE
--rw-r--r--   0 kali      (1000) kali      (1000)     1028 2023-07-21 03:39:09.461454 onlykey-agent-1.1.15/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)      100 2023-07-21 03:38:26.000000 onlykey-agent-1.1.15/README.md
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-07-21 03:39:09.461454 onlykey-agent-1.1.15/onlykey_agent.egg-info/
--rw-r--r--   0 kali      (1000) kali      (1000)     1028 2023-07-21 03:39:09.000000 onlykey-agent-1.1.15/onlykey_agent.egg-info/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)      267 2023-07-21 03:39:09.000000 onlykey-agent-1.1.15/onlykey_agent.egg-info/SOURCES.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-07-21 03:39:09.000000 onlykey-agent-1.1.15/onlykey_agent.egg-info/dependency_links.txt
--rw-r--r--   0 kali      (1000) kali      (1000)      139 2023-07-21 03:39:09.000000 onlykey-agent-1.1.15/onlykey_agent.egg-info/entry_points.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       33 2023-07-21 03:39:09.000000 onlykey-agent-1.1.15/onlykey_agent.egg-info/requires.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       14 2023-07-21 03:39:09.000000 onlykey-agent-1.1.15/onlykey_agent.egg-info/top_level.txt
--rw-r--r--   0 kali      (1000) kali      (1000)      253 2023-07-21 03:38:26.000000 onlykey-agent-1.1.15/onlykey_agent.py
--rw-r--r--   0 kali      (1000) kali      (1000)       38 2023-07-21 03:39:09.461454 onlykey-agent-1.1.15/setup.cfg
--rw-r--r--   0 kali      (1000) kali      (1000)     1416 2023-07-21 03:38:26.000000 onlykey-agent-1.1.15/setup.py
+drwxr-xr-x   0 t          (501) staff       (20)        0 2020-08-17 14:03:00.000000 onlykey-agent-1.1.9/
+-rw-r--r--   0 t          (501) staff       (20)     1043 2020-08-17 14:03:00.000000 onlykey-agent-1.1.9/PKG-INFO
+-rw-r--r--   0 t          (501) staff       (20)     4158 2020-08-17 13:55:46.000000 onlykey-agent-1.1.9/README.md
+drwxr-xr-x   0 t          (501) staff       (20)        0 2020-08-17 14:03:00.000000 onlykey-agent-1.1.9/onlykey_agent.egg-info/
+-rw-r--r--   0 t          (501) staff       (20)     1043 2020-08-17 14:03:00.000000 onlykey-agent-1.1.9/onlykey_agent.egg-info/PKG-INFO
+-rw-r--r--   0 t          (501) staff       (20)      259 2020-08-17 14:03:00.000000 onlykey-agent-1.1.9/onlykey_agent.egg-info/SOURCES.txt
+-rw-r--r--   0 t          (501) staff       (20)        1 2020-08-17 14:03:00.000000 onlykey-agent-1.1.9/onlykey_agent.egg-info/dependency_links.txt
+-rw-r--r--   0 t          (501) staff       (20)      140 2020-08-17 14:03:00.000000 onlykey-agent-1.1.9/onlykey_agent.egg-info/entry_points.txt
+-rw-r--r--   0 t          (501) staff       (20)       33 2020-08-17 14:03:00.000000 onlykey-agent-1.1.9/onlykey_agent.egg-info/requires.txt
+-rw-r--r--   0 t          (501) staff       (20)        1 2020-08-17 14:03:00.000000 onlykey-agent-1.1.9/onlykey_agent.egg-info/top_level.txt
+-rw-r--r--   0 t          (501) staff       (20)      253 2020-08-17 13:30:40.000000 onlykey-agent-1.1.9/onlykey_agent.py
+-rw-r--r--   0 t          (501) staff       (20)       38 2020-08-17 14:03:00.000000 onlykey-agent-1.1.9/setup.cfg
+-rw-r--r--   0 t          (501) staff       (20)     1415 2020-08-17 14:00:25.000000 onlykey-agent-1.1.9/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `onlykey-agent-1.1.15/PKG-INFO` & `onlykey-agent-1.1.9/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,16 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.1
 Name: onlykey-agent
-Version: 1.1.15
+Version: 1.1.9
 Summary: Using OnlyKey as hardware SSH/GPG agent
 Home-page: http://github.com/trustcrypto/onlykey-agent
 Author: CryptoTrust
 Author-email: admin@crp.to
+License: UNKNOWN
+Description: UNKNOWN
 Platform: POSIX
 Classifier: Environment :: Console
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
@@ -18,8 +20,7 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Networking
 Classifier: Topic :: Communications
 Classifier: Topic :: Security
 Classifier: Topic :: Utilities
-License-File: LICENSE
```

### Comparing `onlykey-agent-1.1.15/onlykey_agent.egg-info/PKG-INFO` & `onlykey-agent-1.1.9/onlykey_agent.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,16 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.1
 Name: onlykey-agent
-Version: 1.1.15
+Version: 1.1.9
 Summary: Using OnlyKey as hardware SSH/GPG agent
 Home-page: http://github.com/trustcrypto/onlykey-agent
 Author: CryptoTrust
 Author-email: admin@crp.to
+License: UNKNOWN
+Description: UNKNOWN
 Platform: POSIX
 Classifier: Environment :: Console
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
@@ -18,8 +20,7 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Networking
 Classifier: Topic :: Communications
 Classifier: Topic :: Security
 Classifier: Topic :: Utilities
-License-File: LICENSE
```

### Comparing `onlykey-agent-1.1.15/setup.py` & `onlykey-agent-1.1.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='onlykey-agent',
-    version='1.1.15',
+    version='1.1.9',
     description='Using OnlyKey as hardware SSH/GPG agent',
     author='CryptoTrust',
     author_email='admin@crp.to',
     url='http://github.com/trustcrypto/onlykey-agent',
     scripts=['onlykey_agent.py'],
     install_requires=[
-        'lib-agent>=1.0.6',
-        'onlykey>=1.2.10'
+        'lib-agent>=0.14.2',
+        'onlykey>=1.2.0'
     ],
     platforms=['POSIX'],
     classifiers=[
         'Environment :: Console',
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'Intended Audience :: Information Technology',
```

