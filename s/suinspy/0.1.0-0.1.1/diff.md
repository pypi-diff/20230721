# Comparing `tmp/suinspy-0.1.0.tar.gz` & `tmp/suinspy-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "suinspy-0.1.0.tar", max compression
+gzip compressed data, was "suinspy-0.1.1.tar", max compression
```

## Comparing `suinspy-0.1.0.tar` & `suinspy-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      374 2023-07-20 21:32:56.193773 suinspy-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       22 2023-07-20 21:32:56.193773 suinspy-0.1.0/suinspy/__init__.py
--rw-r--r--   0        0        0     3236 2023-07-20 21:32:56.193773 suinspy-0.1.0/suinspy/client.py
--rw-r--r--   0        0        0      452 2023-07-20 21:32:56.193773 suinspy-0.1.0/suinspy/types/objects.py
--rw-r--r--   0        0        0      140 2023-07-20 21:32:56.193773 suinspy-0.1.0/suinspy/utils/constants.py
--rw-r--r--   0        0        0      468 2023-07-20 21:32:56.193773 suinspy-0.1.0/suinspy/utils/parser.py
--rw-r--r--   0        0        0      702 2023-07-20 21:32:56.193773 suinspy-0.1.0/suinspy/utils/queries.py
--rw-r--r--   0        0        0      679 2023-07-20 21:33:11.014498 suinspy-0.1.0/setup.py
--rw-r--r--   0        0        0      359 2023-07-20 21:33:11.014689 suinspy-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      373 2023-07-20 21:57:15.471466 suinspy-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-07-20 21:32:56.193773 suinspy-0.1.1/suinspy/__init__.py
+-rw-r--r--   0        0        0     3236 2023-07-20 21:32:56.193773 suinspy-0.1.1/suinspy/client.py
+-rw-r--r--   0        0        0      452 2023-07-20 21:32:56.193773 suinspy-0.1.1/suinspy/types/objects.py
+-rw-r--r--   0        0        0      140 2023-07-20 21:32:56.193773 suinspy-0.1.1/suinspy/utils/constants.py
+-rw-r--r--   0        0        0      468 2023-07-20 21:32:56.193773 suinspy-0.1.1/suinspy/utils/parser.py
+-rw-r--r--   0        0        0      702 2023-07-20 21:32:56.193773 suinspy-0.1.1/suinspy/utils/queries.py
+-rw-r--r--   0        0        0      671 2023-07-20 21:57:19.908096 suinspy-0.1.1/setup.py
+-rw-r--r--   0        0        0      351 2023-07-20 21:57:19.908283 suinspy-0.1.1/PKG-INFO
```

### Comparing `suinspy-0.1.0/suinspy/client.py` & `suinspy-0.1.1/suinspy/client.py`

 * *Files identical despite different names*

### Comparing `suinspy-0.1.0/suinspy/utils/queries.py` & `suinspy-0.1.1/suinspy/utils/queries.py`

 * *Files identical despite different names*

### Comparing `suinspy-0.1.0/setup.py` & `suinspy-0.1.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 packages = \
 ['suinspy', 'suinspy.types', 'suinspy.utils']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['pysui>=0.27.1,<0.28.0', 'requests>=2.31.0,<3.0.0']
+['pysui==0.30.0', 'requests>=2.31.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'suinspy',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': 'Sui Name Service Python SDK Client',
     'long_description': None,
     'author': 'andreidev1',
     'author_email': 'd.andrei01@yahoo.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

