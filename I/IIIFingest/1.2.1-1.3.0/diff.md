# Comparing `tmp/IIIFingest-1.2.1.tar.gz` & `tmp/IIIFingest-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IIIFingest-1.2.1.tar", last modified: Wed Nov 23 15:31:51 2022, max compression
+gzip compressed data, was "IIIFingest-1.3.0.tar", last modified: Fri Jul 21 15:15:25 2023, max compression
```

## Comparing `IIIFingest-1.2.1.tar` & `IIIFingest-1.3.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 colecrawford   (504) staff       (20)        0 2022-11-23 15:31:51.513506 IIIFingest-1.2.1/
--rw-r--r--   0 colecrawford   (504) staff       (20)      611 2022-03-29 15:40:02.000000 IIIFingest-1.2.1/LICENSE.md
--rw-r--r--   0 colecrawford   (504) staff       (20)     8623 2022-11-23 15:31:51.513605 IIIFingest-1.2.1/PKG-INFO
--rw-r--r--   0 colecrawford   (504) staff       (20)     7973 2022-11-22 19:36:21.000000 IIIFingest-1.2.1/README.md
--rw-r--r--   0 colecrawford   (504) staff       (20)      510 2022-11-17 14:09:29.000000 IIIFingest-1.2.1/pyproject.toml
--rw-r--r--   0 colecrawford   (504) staff       (20)     1201 2022-11-23 15:31:51.514058 IIIFingest-1.2.1/setup.cfg
-drwxr-xr-x   0 colecrawford   (504) staff       (20)        0 2022-11-23 15:31:51.509122 IIIFingest-1.2.1/src/
-drwxr-xr-x   0 colecrawford   (504) staff       (20)        0 2022-11-23 15:31:51.512387 IIIFingest-1.2.1/src/IIIFingest/
--rw-r--r--   0 colecrawford   (504) staff       (20)        0 2022-03-29 15:40:02.000000 IIIFingest-1.2.1/src/IIIFingest/__init__.py
--rw-r--r--   0 colecrawford   (504) staff       (20)     7706 2022-11-04 15:51:37.000000 IIIFingest-1.2.1/src/IIIFingest/asset.py
--rw-r--r--   0 colecrawford   (504) staff       (20)     5560 2022-11-17 14:09:25.000000 IIIFingest-1.2.1/src/IIIFingest/auth.py
--rw-r--r--   0 colecrawford   (504) staff       (20)     3924 2022-11-04 15:51:37.000000 IIIFingest-1.2.1/src/IIIFingest/bucket.py
--rw-r--r--   0 colecrawford   (504) staff       (20)    11591 2022-11-14 16:56:24.000000 IIIFingest-1.2.1/src/IIIFingest/client.py
--rw-r--r--   0 colecrawford   (504) staff       (20)    10385 2022-05-14 20:49:55.000000 IIIFingest-1.2.1/src/IIIFingest/generate_manifest.py
--rw-r--r--   0 colecrawford   (504) staff       (20)     4661 2022-11-17 14:09:25.000000 IIIFingest-1.2.1/src/IIIFingest/ingest.py
--rw-r--r--   0 colecrawford   (504) staff       (20)     1763 2022-11-04 15:51:37.000000 IIIFingest-1.2.1/src/IIIFingest/settings.py
-drwxr-xr-x   0 colecrawford   (504) staff       (20)        0 2022-11-23 15:31:51.513377 IIIFingest-1.2.1/src/IIIFingest.egg-info/
--rw-r--r--   0 colecrawford   (504) staff       (20)     8623 2022-11-23 15:31:51.000000 IIIFingest-1.2.1/src/IIIFingest.egg-info/PKG-INFO
--rw-r--r--   0 colecrawford   (504) staff       (20)      446 2022-11-23 15:31:51.000000 IIIFingest-1.2.1/src/IIIFingest.egg-info/SOURCES.txt
--rw-r--r--   0 colecrawford   (504) staff       (20)        1 2022-11-23 15:31:51.000000 IIIFingest-1.2.1/src/IIIFingest.egg-info/dependency_links.txt
--rw-r--r--   0 colecrawford   (504) staff       (20)      499 2022-11-23 15:31:51.000000 IIIFingest-1.2.1/src/IIIFingest.egg-info/requires.txt
--rw-r--r--   0 colecrawford   (504) staff       (20)       11 2022-11-23 15:31:51.000000 IIIFingest-1.2.1/src/IIIFingest.egg-info/top_level.txt
+drwxr-xr-x   0 colecrawford   (504) staff       (20)        0 2023-07-21 15:15:25.565458 IIIFingest-1.3.0/
+-rw-r--r--   0 colecrawford   (504) staff       (20)      611 2022-03-29 15:40:02.000000 IIIFingest-1.3.0/LICENSE.md
+-rw-r--r--   0 colecrawford   (504) staff       (20)     8623 2023-07-21 15:15:25.565569 IIIFingest-1.3.0/PKG-INFO
+-rw-r--r--   0 colecrawford   (504) staff       (20)     7973 2022-11-22 19:36:21.000000 IIIFingest-1.3.0/README.md
+-rw-r--r--   0 colecrawford   (504) staff       (20)      510 2022-11-17 14:09:29.000000 IIIFingest-1.3.0/pyproject.toml
+-rw-r--r--   0 colecrawford   (504) staff       (20)     1236 2023-07-21 15:15:25.566037 IIIFingest-1.3.0/setup.cfg
+drwxr-xr-x   0 colecrawford   (504) staff       (20)        0 2023-07-21 15:15:25.559976 IIIFingest-1.3.0/src/
+drwxr-xr-x   0 colecrawford   (504) staff       (20)        0 2023-07-21 15:15:25.564146 IIIFingest-1.3.0/src/IIIFingest/
+-rw-r--r--   0 colecrawford   (504) staff       (20)        0 2022-03-29 15:40:02.000000 IIIFingest-1.3.0/src/IIIFingest/__init__.py
+-rw-r--r--   0 colecrawford   (504) staff       (20)     7706 2022-11-04 15:51:37.000000 IIIFingest-1.3.0/src/IIIFingest/asset.py
+-rw-r--r--   0 colecrawford   (504) staff       (20)     5560 2022-11-17 14:09:25.000000 IIIFingest-1.3.0/src/IIIFingest/auth.py
+-rw-r--r--   0 colecrawford   (504) staff       (20)     3924 2022-11-04 15:51:37.000000 IIIFingest-1.3.0/src/IIIFingest/bucket.py
+-rw-r--r--   0 colecrawford   (504) staff       (20)    11591 2022-11-14 16:56:24.000000 IIIFingest-1.3.0/src/IIIFingest/client.py
+-rw-r--r--   0 colecrawford   (504) staff       (20)    10385 2022-05-14 20:49:55.000000 IIIFingest-1.3.0/src/IIIFingest/generate_manifest.py
+-rw-r--r--   0 colecrawford   (504) staff       (20)     4661 2022-11-17 14:09:25.000000 IIIFingest-1.3.0/src/IIIFingest/ingest.py
+-rw-r--r--   0 colecrawford   (504) staff       (20)     1763 2022-11-04 15:51:37.000000 IIIFingest-1.3.0/src/IIIFingest/settings.py
+drwxr-xr-x   0 colecrawford   (504) staff       (20)        0 2023-07-21 15:15:25.565317 IIIFingest-1.3.0/src/IIIFingest.egg-info/
+-rw-r--r--   0 colecrawford   (504) staff       (20)     8623 2023-07-21 15:15:25.000000 IIIFingest-1.3.0/src/IIIFingest.egg-info/PKG-INFO
+-rw-r--r--   0 colecrawford   (504) staff       (20)      456 2023-07-21 15:15:25.000000 IIIFingest-1.3.0/src/IIIFingest.egg-info/SOURCES.txt
+-rw-r--r--   0 colecrawford   (504) staff       (20)        1 2023-07-21 15:15:25.000000 IIIFingest-1.3.0/src/IIIFingest.egg-info/dependency_links.txt
+-rw-r--r--   0 colecrawford   (504) staff       (20)      545 2023-07-21 15:15:25.000000 IIIFingest-1.3.0/src/IIIFingest.egg-info/requires.txt
+-rw-r--r--   0 colecrawford   (504) staff       (20)       11 2023-07-21 15:15:25.000000 IIIFingest-1.3.0/src/IIIFingest.egg-info/top_level.txt
```

### Comparing `IIIFingest-1.2.1/LICENSE.md` & `IIIFingest-1.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `IIIFingest-1.2.1/PKG-INFO` & `IIIFingest-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IIIFingest
-Version: 1.2.1
+Version: 1.3.0
 Summary: A wrapper library for interacting with the MPS ingest system for IIIF resources
 Home-page: https://github.com/Harvard-ATG/lts-iiif-ingest-service
 Author: Cole Crawford
 Author-email: cole_crawford@fas.harvard.edu
 Project-URL: Bug Tracker, https://github.com/Harvard-ATG/lts-iiif-ingest-service/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `IIIFingest-1.2.1/README.md` & `IIIFingest-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `IIIFingest-1.2.1/setup.cfg` & `IIIFingest-1.3.0/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = IIIFingest
-version = 1.2.1
+version = 1.3.0
 author = Cole Crawford
 author_email = cole_crawford@fas.harvard.edu
 description = A wrapper library for interacting with the MPS ingest system for IIIF resources
 long_description = file: readme.md
 long_description_content_type = text/markdown
 url = https://github.com/Harvard-ATG/lts-iiif-ingest-service
 project_urls = 
@@ -17,34 +17,34 @@
 [options]
 package_dir = 
 	= src
 packages = find:
 python_requires = >=3.7
 install_requires = 
 	pyjwt ~= 2.4
-	cryptography ~= 3.3
+	cryptography >= 3.3,< 42.0
 	jsonschema ~= 4.15
 	boto3 ~= 1.26
-	Pillow ~= 9.3
+	Pillow >= 9.3,< 11.0
 	requests ~= 2.28
 	shortuuid ~= 1.0
 	pyIIIFpres ~= 0.1
 	python-magic ~= 0.4
 	Deprecated ~= 1.2
 	backports.zoneinfo ~= 0.2;python_version<"3.9"
 
 [options.extras_require]
 all = 
 	%(dev)s
 dev = 
-	pre-commit ~= 2.20
+	pre-commit >= 2.20,< 4.0
 	isort ~= 5.10
-	black ~= 22.8
-	flake8 ~= 5.0
-	python-dotenv ~= 0.21
+	black >= 22.8,< 24.0
+	flake8 >= 5,< 7
+	python-dotenv >= 0.21,< 2.0
 	moto ~= 4.0
 	pytest ~= 7.1
 	pytest-mock ~= 3.8
 	pytest-dotenv ~= 0.5
 	build ~= 0.9
 
 [options.packages.find]
```

### Comparing `IIIFingest-1.2.1/src/IIIFingest/asset.py` & `IIIFingest-1.3.0/src/IIIFingest/asset.py`

 * *Files identical despite different names*

### Comparing `IIIFingest-1.2.1/src/IIIFingest/auth.py` & `IIIFingest-1.3.0/src/IIIFingest/auth.py`

 * *Files identical despite different names*

### Comparing `IIIFingest-1.2.1/src/IIIFingest/bucket.py` & `IIIFingest-1.3.0/src/IIIFingest/bucket.py`

 * *Files identical despite different names*

### Comparing `IIIFingest-1.2.1/src/IIIFingest/client.py` & `IIIFingest-1.3.0/src/IIIFingest/client.py`

 * *Files identical despite different names*

### Comparing `IIIFingest-1.2.1/src/IIIFingest/generate_manifest.py` & `IIIFingest-1.3.0/src/IIIFingest/generate_manifest.py`

 * *Files identical despite different names*

### Comparing `IIIFingest-1.2.1/src/IIIFingest/ingest.py` & `IIIFingest-1.3.0/src/IIIFingest/ingest.py`

 * *Files identical despite different names*

### Comparing `IIIFingest-1.2.1/src/IIIFingest/settings.py` & `IIIFingest-1.3.0/src/IIIFingest/settings.py`

 * *Files identical despite different names*

### Comparing `IIIFingest-1.2.1/src/IIIFingest.egg-info/PKG-INFO` & `IIIFingest-1.3.0/src/IIIFingest.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IIIFingest
-Version: 1.2.1
+Version: 1.3.0
 Summary: A wrapper library for interacting with the MPS ingest system for IIIF resources
 Home-page: https://github.com/Harvard-ATG/lts-iiif-ingest-service
 Author: Cole Crawford
 Author-email: cole_crawford@fas.harvard.edu
 Project-URL: Bug Tracker, https://github.com/Harvard-ATG/lts-iiif-ingest-service/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

