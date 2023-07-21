# Comparing `tmp/zerocap_websocket_test-1.0.0.tar.gz` & `tmp/zerocap_websocket_test-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zerocap_websocket_test-1.0.0.tar", last modified: Fri Jul 21 07:50:17 2023, max compression
+gzip compressed data, was "zerocap_websocket_test-1.0.1.tar", last modified: Fri Jul 21 10:13:57 2023, max compression
```

## Comparing `zerocap_websocket_test-1.0.0.tar` & `zerocap_websocket_test-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 gao        (501) staff       (20)        0 2023-07-21 07:50:17.721948 zerocap_websocket_test-1.0.0/
--rw-r--r--   0 gao        (501) staff       (20)    11323 2023-07-21 07:23:19.000000 zerocap_websocket_test-1.0.0/LICENSE.txt
--rw-r--r--   0 gao        (501) staff       (20)      959 2023-07-21 07:50:17.721565 zerocap_websocket_test-1.0.0/PKG-INFO
--rw-r--r--   0 gao        (501) staff       (20)       88 2023-07-21 07:17:19.000000 zerocap_websocket_test-1.0.0/README.rst
--rw-r--r--   0 gao        (501) staff       (20)       38 2023-07-21 07:50:17.722064 zerocap_websocket_test-1.0.0/setup.cfg
--rw-r--r--   0 gao        (501) staff       (20)     1183 2023-07-21 07:49:13.000000 zerocap_websocket_test-1.0.0/setup.py
-drwxr-xr-x   0 gao        (501) staff       (20)        0 2023-07-21 07:50:17.717904 zerocap_websocket_test-1.0.0/zerocap_websocket_test/
--rw-r--r--   0 gao        (501) staff       (20)        0 2023-06-19 05:47:41.000000 zerocap_websocket_test-1.0.0/zerocap_websocket_test/__init__.py
--rw-r--r--   0 gao        (501) staff       (20)     3414 2023-07-21 07:30:11.000000 zerocap_websocket_test-1.0.0/zerocap_websocket_test/main.py
-drwxr-xr-x   0 gao        (501) staff       (20)        0 2023-07-21 07:50:17.721043 zerocap_websocket_test-1.0.0/zerocap_websocket_test.egg-info/
--rw-r--r--   0 gao        (501) staff       (20)      959 2023-07-21 07:50:17.000000 zerocap_websocket_test-1.0.0/zerocap_websocket_test.egg-info/PKG-INFO
--rw-r--r--   0 gao        (501) staff       (20)      281 2023-07-21 07:50:17.000000 zerocap_websocket_test-1.0.0/zerocap_websocket_test.egg-info/SOURCES.txt
--rw-r--r--   0 gao        (501) staff       (20)        1 2023-07-21 07:50:17.000000 zerocap_websocket_test-1.0.0/zerocap_websocket_test.egg-info/dependency_links.txt
--rw-r--r--   0 gao        (501) staff       (20)       23 2023-07-21 07:50:17.000000 zerocap_websocket_test-1.0.0/zerocap_websocket_test.egg-info/top_level.txt
+drwxr-xr-x   0 gao        (501) staff       (20)        0 2023-07-21 10:13:57.604308 zerocap_websocket_test-1.0.1/
+-rw-r--r--   0 gao        (501) staff       (20)    11323 2023-07-21 07:23:19.000000 zerocap_websocket_test-1.0.1/LICENSE.txt
+-rw-r--r--   0 gao        (501) staff       (20)      873 2023-07-21 10:13:57.604037 zerocap_websocket_test-1.0.1/PKG-INFO
+-rw-r--r--   0 gao        (501) staff       (20)       18 2023-07-21 10:13:46.000000 zerocap_websocket_test-1.0.1/README.rst
+-rw-r--r--   0 gao        (501) staff       (20)       38 2023-07-21 10:13:57.604385 zerocap_websocket_test-1.0.1/setup.cfg
+-rw-r--r--   0 gao        (501) staff       (20)     1167 2023-07-21 10:13:46.000000 zerocap_websocket_test-1.0.1/setup.py
+drwxr-xr-x   0 gao        (501) staff       (20)        0 2023-07-21 10:13:57.600637 zerocap_websocket_test-1.0.1/zerocap_websocket_test/
+-rw-r--r--   0 gao        (501) staff       (20)       80 2023-07-21 08:10:24.000000 zerocap_websocket_test-1.0.1/zerocap_websocket_test/__init__.py
+-rw-r--r--   0 gao        (501) staff       (20)     2389 2023-07-21 10:05:12.000000 zerocap_websocket_test-1.0.1/zerocap_websocket_test/main.py
+drwxr-xr-x   0 gao        (501) staff       (20)        0 2023-07-21 10:13:57.603654 zerocap_websocket_test-1.0.1/zerocap_websocket_test.egg-info/
+-rw-r--r--   0 gao        (501) staff       (20)      873 2023-07-21 10:13:57.000000 zerocap_websocket_test-1.0.1/zerocap_websocket_test.egg-info/PKG-INFO
+-rw-r--r--   0 gao        (501) staff       (20)      281 2023-07-21 10:13:57.000000 zerocap_websocket_test-1.0.1/zerocap_websocket_test.egg-info/SOURCES.txt
+-rw-r--r--   0 gao        (501) staff       (20)        1 2023-07-21 10:13:57.000000 zerocap_websocket_test-1.0.1/zerocap_websocket_test.egg-info/dependency_links.txt
+-rw-r--r--   0 gao        (501) staff       (20)       23 2023-07-21 10:13:57.000000 zerocap_websocket_test-1.0.1/zerocap_websocket_test.egg-info/top_level.txt
```

### Comparing `zerocap_websocket_test-1.0.0/LICENSE.txt` & `zerocap_websocket_test-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zerocap_websocket_test-1.0.0/setup.py` & `zerocap_websocket_test-1.0.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from distutils.core import setup
 from setuptools import find_packages
 
 with open("README.rst", "r") as f:
   long_description = f.read()
 
 setup(name='zerocap_websocket_test',  # 包名
-      version='1.0.0',  # 版本号
-      description='A small example package',
+      version='1.0.1',  # 版本号
+      description='websocket_test',
       long_description=long_description,
-      author='mikezhou_talk',
+      author='gaogao',
       author_email='y18362683626@gmail.com',
       url='',
       install_requires=[],
       license='BSD License',
       packages=find_packages(),
       platforms=["all"],
       classifiers=[
```

