# Comparing `tmp/ipfs_stac-0.1.5.tar.gz` & `tmp/ipfs_stac-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipfs_stac-0.1.5.tar", last modified: Thu Jul 20 23:08:41 2023, max compression
+gzip compressed data, was "ipfs_stac-0.1.6.tar", last modified: Thu Jul 20 23:15:16 2023, max compression
```

## Comparing `ipfs_stac-0.1.5.tar` & `ipfs_stac-0.1.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 23:08:41.875232 ipfs_stac-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-20 23:08:30.000000 ipfs_stac-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-20 23:08:30.000000 ipfs_stac-0.1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-07-20 23:08:41.875232 ipfs_stac-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-07-20 23:08:30.000000 ipfs_stac-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 23:08:41.875232 ipfs_stac-0.1.5/ipfs_stac/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 23:08:30.000000 ipfs_stac-0.1.5/ipfs_stac/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4322 2023-07-20 23:08:30.000000 ipfs_stac-0.1.5/ipfs_stac/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 23:08:41.875232 ipfs_stac-0.1.5/ipfs_stac.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-07-20 23:08:41.000000 ipfs_stac-0.1.5/ipfs_stac.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-20 23:08:41.000000 ipfs_stac-0.1.5/ipfs_stac.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 23:08:41.000000 ipfs_stac-0.1.5/ipfs_stac.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-20 23:08:41.000000 ipfs_stac-0.1.5/ipfs_stac.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-20 23:08:41.000000 ipfs_stac-0.1.5/ipfs_stac.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 23:08:41.875232 ipfs_stac-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-07-20 23:08:30.000000 ipfs_stac-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 23:15:16.191617 ipfs_stac-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-20 23:15:06.000000 ipfs_stac-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-20 23:15:06.000000 ipfs_stac-0.1.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-07-20 23:15:16.191617 ipfs_stac-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-07-20 23:15:06.000000 ipfs_stac-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 23:15:16.187617 ipfs_stac-0.1.6/ipfs_stac/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 23:15:06.000000 ipfs_stac-0.1.6/ipfs_stac/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4322 2023-07-20 23:15:06.000000 ipfs_stac-0.1.6/ipfs_stac/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 23:15:16.191617 ipfs_stac-0.1.6/ipfs_stac.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-07-20 23:15:16.000000 ipfs_stac-0.1.6/ipfs_stac.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-20 23:15:16.000000 ipfs_stac-0.1.6/ipfs_stac.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 23:15:16.000000 ipfs_stac-0.1.6/ipfs_stac.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-20 23:15:16.000000 ipfs_stac-0.1.6/ipfs_stac.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-20 23:15:16.000000 ipfs_stac-0.1.6/ipfs_stac.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 23:15:16.191617 ipfs_stac-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-20 23:15:06.000000 ipfs_stac-0.1.6/setup.py
```

### Comparing `ipfs_stac-0.1.5/LICENSE` & `ipfs_stac-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ipfs_stac-0.1.5/PKG-INFO` & `ipfs_stac-0.1.6/ipfs_stac.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 Metadata-Version: 2.1
-Name: ipfs_stac
-Version: 0.1.5
+Name: ipfs-stac
+Version: 0.1.6
 Summary: The EASIER Data Initiative Python IPFS-STAC Client
 Author: The EASIER Data Initiative
 License: MIT
+Project-URL: Twitter, https://twitter.com/easierdataorg
+Project-URL: GitHub, https://github.com/easierdata/ipfs-stac
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # The EASIER Data Initiative's Python Client
 
 ### Features
```

### Comparing `ipfs_stac-0.1.5/README.md` & `ipfs_stac-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `ipfs_stac-0.1.5/ipfs_stac/client.py` & `ipfs_stac-0.1.6/ipfs_stac/client.py`

 * *Files identical despite different names*

### Comparing `ipfs_stac-0.1.5/ipfs_stac.egg-info/PKG-INFO` & `ipfs_stac-0.1.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 Metadata-Version: 2.1
-Name: ipfs-stac
-Version: 0.1.5
+Name: ipfs_stac
+Version: 0.1.6
 Summary: The EASIER Data Initiative Python IPFS-STAC Client
 Author: The EASIER Data Initiative
 License: MIT
+Project-URL: Twitter, https://twitter.com/easierdataorg
+Project-URL: GitHub, https://github.com/easierdata/ipfs-stac
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # The EASIER Data Initiative's Python Client
 
 ### Features
```

### Comparing `ipfs_stac-0.1.5/setup.py` & `ipfs_stac-0.1.6/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 from setuptools import find_packages, setup
 
 setup(
     name='ipfs_stac',
     packages=find_packages(include=['ipfs_stac']),
-    version='0.1.5',
+    version='0.1.6',
     description='The EASIER Data Initiative Python IPFS-STAC Client',
     author='The EASIER Data Initiative',
     license='MIT',
     install_requires=['ipfsspec', 'fsspec', 'requests', 'pandas', 'beautifulsoup4', 'pystac-client'],
     setup_requires=['pytest-runner'],
     tests_require=['pytest'],
     test_suite='tests',
     long_description=open('README.md').read(),
-    long_description_content_type='text/markdown'
+    long_description_content_type='text/markdown',
+    project_urls={
+        "Twitter": "https://twitter.com/easierdataorg",
+        "GitHub": "https://github.com/easierdata/ipfs-stac"
+    }
 )
```

