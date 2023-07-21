# Comparing `tmp/dev-assistant-client-0.1.8.tar.gz` & `tmp/dev-assistant-client-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dev-assistant-client-0.1.8.tar", last modified: Sat Jul 15 02:54:42 2023, max compression
+gzip compressed data, was "dev-assistant-client-0.1.9.tar", last modified: Tue Jul 18 03:30:41 2023, max compression
```

## Comparing `dev-assistant-client-0.1.8.tar` & `dev-assistant-client-0.1.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 02:54:42.333324 dev-assistant-client-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-15 02:54:21.000000 dev-assistant-client-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-15 02:54:42.333324 dev-assistant-client-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-07-15 02:54:21.000000 dev-assistant-client-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 02:54:42.333324 dev-assistant-client-0.1.8/dev_assistant_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-15 02:54:42.000000 dev-assistant-client-0.1.8/dev_assistant_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-15 02:54:42.000000 dev-assistant-client-0.1.8/dev_assistant_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 02:54:42.000000 dev-assistant-client-0.1.8/dev_assistant_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-15 02:54:42.000000 dev-assistant-client-0.1.8/dev_assistant_client.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-15 02:54:42.000000 dev-assistant-client-0.1.8/dev_assistant_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 02:54:42.000000 dev-assistant-client-0.1.8/dev_assistant_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 02:54:42.333324 dev-assistant-client-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-07-15 02:54:21.000000 dev-assistant-client-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:30:41.586288 dev-assistant-client-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-18 03:30:17.000000 dev-assistant-client-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-18 03:30:41.586288 dev-assistant-client-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-07-18 03:30:17.000000 dev-assistant-client-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:30:41.586288 dev-assistant-client-0.1.9/dev_assistant_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-18 03:30:41.000000 dev-assistant-client-0.1.9/dev_assistant_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-18 03:30:41.000000 dev-assistant-client-0.1.9/dev_assistant_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 03:30:41.000000 dev-assistant-client-0.1.9/dev_assistant_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-18 03:30:41.000000 dev-assistant-client-0.1.9/dev_assistant_client.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-18 03:30:41.000000 dev-assistant-client-0.1.9/dev_assistant_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 03:30:41.000000 dev-assistant-client-0.1.9/dev_assistant_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 03:30:41.586288 dev-assistant-client-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-07-18 03:30:17.000000 dev-assistant-client-0.1.9/setup.py
```

### Comparing `dev-assistant-client-0.1.8/LICENSE` & `dev-assistant-client-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dev-assistant-client-0.1.8/README.md` & `dev-assistant-client-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `dev-assistant-client-0.1.8/setup.py` & `dev-assistant-client-0.1.9/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 setup(
     name='dev-assistant-client',
-    version='0.1.8',
+    version='0.1.9',
     url='https://github.com/lucianotonet/dev-assistant-client',
     author='Luciano Tonet',
     author_email='tonetlds@gmail.com',
     description='A local extension for ChatGPT plugin DevAssistant, which helps you with your development tasks straight in your machine.',
     packages=find_packages(),
     install_requires=required,
     entry_points={
```

