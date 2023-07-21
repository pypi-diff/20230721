# Comparing `tmp/mrsal-0.6.2a0.tar.gz` & `tmp/mrsal-0.6.3a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mrsal-0.6.2a0.tar", max compression
+gzip compressed data, was "mrsal-0.6.3a0.tar", max compression
```

## Comparing `mrsal-0.6.2a0.tar` & `mrsal-0.6.3a0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    35148 2022-09-08 10:55:29.050700 mrsal-0.6.2a0/LICENSE.txt
--rw-r--r--   0        0        0    10432 2023-07-19 13:31:36.191363 mrsal-0.6.2a0/README.md
--rw-r--r--   0        0        0        0 2022-08-17 10:39:13.102254 mrsal-0.6.2a0/mrsal/__init__.py
--rw-r--r--   0        0        0        0 2022-08-17 10:39:13.102254 mrsal-0.6.2a0/mrsal/config/__init__.py
--rw-r--r--   0        0        0     1349 2023-07-18 07:37:02.804267 mrsal-0.6.2a0/mrsal/config/config.py
--rw-r--r--   0        0        0      289 2023-07-17 11:17:31.722576 mrsal-0.6.2a0/mrsal/config/exceptions.py
--rw-r--r--   0        0        0     2443 2023-07-18 08:59:41.089318 mrsal-0.6.2a0/mrsal/config/logging.py
--rw-r--r--   0        0        0    36078 2023-07-18 08:57:30.540133 mrsal-0.6.2a0/mrsal/mrsal.py
--rw-r--r--   0        0        0      344 2023-07-18 09:00:30.088267 mrsal-0.6.2a0/mrsal/utils/utils.py
--rw-r--r--   0        0        0      675 2023-07-19 13:34:21.131729 mrsal-0.6.2a0/pyproject.toml
--rw-r--r--   0        0        0    11070 1970-01-01 00:00:00.000000 mrsal-0.6.2a0/PKG-INFO
+-rw-r--r--   0        0        0    35148 2022-09-08 10:55:29.050700 mrsal-0.6.3a0/LICENSE.txt
+-rw-r--r--   0        0        0    10432 2023-07-21 08:20:01.067051 mrsal-0.6.3a0/README.md
+-rw-r--r--   0        0        0        0 2022-08-17 10:39:13.102254 mrsal-0.6.3a0/mrsal/__init__.py
+-rw-r--r--   0        0        0        0 2022-08-17 10:39:13.102254 mrsal-0.6.3a0/mrsal/config/__init__.py
+-rw-r--r--   0        0        0     1349 2023-07-18 07:37:02.804267 mrsal-0.6.3a0/mrsal/config/config.py
+-rw-r--r--   0        0        0      289 2023-07-17 11:17:31.722576 mrsal-0.6.3a0/mrsal/config/exceptions.py
+-rw-r--r--   0        0        0     2443 2023-07-18 08:59:41.089318 mrsal-0.6.3a0/mrsal/config/logging.py
+-rw-r--r--   0        0        0    36078 2023-07-18 08:57:30.540133 mrsal-0.6.3a0/mrsal/mrsal.py
+-rw-r--r--   0        0        0      344 2023-07-18 09:00:30.088267 mrsal-0.6.3a0/mrsal/utils/utils.py
+-rw-r--r--   0        0        0      675 2023-07-21 08:19:42.995076 mrsal-0.6.3a0/pyproject.toml
+-rw-r--r--   0        0        0    11070 1970-01-01 00:00:00.000000 mrsal-0.6.3a0/PKG-INFO
```

### Comparing `mrsal-0.6.2a0/LICENSE.txt` & `mrsal-0.6.3a0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mrsal-0.6.2a0/README.md` & `mrsal-0.6.3a0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # MRSAL  <img align="right" width="125" alt="20200907_104224" src="https://github.com/NeoMedSys/mrsal/assets/9555305/ffb55c86-1e9d-4806-b1ca-c906d6985e3a">
-[![Release](https://img.shields.io/badge/release-v0.6.2--alpha-blue.svg)](https://pypi.org/project/mrsal/) [![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)](https://www.python.org/downloads/release/python-3103/) [![Documentation](https://img.shields.io/badge/doc-latest-blue.svg)](https://github.com/NeoMedSys/mrsal/blob/main/FullGuide.md)
+[![Release](https://img.shields.io/badge/release-v0.6.3--alpha-blue.svg)](https://pypi.org/project/mrsal/) [![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)](https://www.python.org/downloads/release/python-3103/) [![Documentation](https://img.shields.io/badge/doc-latest-blue.svg)](https://github.com/NeoMedSys/mrsal/blob/main/FullGuide.md)
 <!-- [![Build Status](https://github.com/NeoMedSys/fatty-model-deploy/actions/workflows/tester.yml/badge.svg)](https://github.com/NeoMedSys/fatty-model-deploy/actions/runs/5576890234) -->
 [![Tests Status](https://github.com/NeoMedSys/mrsal/assets/9555305/5d29b991-1e7f-4737-8e55-5ee2bc9bb5db)](./reports/junit/junit.xml) [![Coverage Status](https://github.com/NeoMedSys/mrsal/assets/9555305/852b4256-d52e-49da-9134-f0e7381935ba)](./reports/coverage/htmlcov/index.html) [![Flake8 Status](https://github.com/NeoMedSys/mrsal/assets/9555305/0113f279-7c5c-4ed8-bd2f-8b2cf84da2a9)](./reports/flake8/flake8.txt)
 
 ## Intro
 Mrsal is a simple to use message broker abstraction on top of [RabbitMQ](https://www.rabbitmq.com/) and [Pika](https://pika.readthedocs.io/en/stable/index.html). The goal is to make Mrsal trivial to re-use in all services of a distributed system and to make the use of advanced message queing protocols easy and safe. No more big chunks of repetive code across your services or bespoke solutions to handle dead letters. 
 
 ###### Mrsal is Arabic for a small arrow and is used to describe something that performs a task with lightness and speed.
```

### Comparing `mrsal-0.6.2a0/mrsal/config/config.py` & `mrsal-0.6.3a0/mrsal/config/config.py`

 * *Files identical despite different names*

### Comparing `mrsal-0.6.2a0/mrsal/config/logging.py` & `mrsal-0.6.3a0/mrsal/config/logging.py`

 * *Files identical despite different names*

### Comparing `mrsal-0.6.2a0/mrsal/mrsal.py` & `mrsal-0.6.3a0/mrsal/mrsal.py`

 * *Files identical despite different names*

### Comparing `mrsal-0.6.2a0/pyproject.toml` & `mrsal-0.6.3a0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 authors = ["Raafat <rafatzahran90@gmail.com>", "Jon E Nesvold <jnesvold@pm.me>"]
 description = "Mrsal is a simple to use message broker abstraction on top of RabbitMQ and Pika."
 keywords = ["message broker", "RabbitMQ", "Pika", "Mrsal"]
 license = ""
 maintainers = ["Raafat <rafatzahran90@gmail.com>", "Jon E Nesvold <jnesvold@pm.me>"]
 name = "mrsal"
 readme = "README.md"
-version = "0.6.2-alpha"
+version = "0.6.3-alpha"
 
 [tool.poetry.dependencies]
 colorlog = "^6.7.0"
 pika = "^1.3.0"
 python = "^3.10"
 retry = "^0.9.2"
```

### Comparing `mrsal-0.6.2a0/PKG-INFO` & `mrsal-0.6.3a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mrsal
-Version: 0.6.2a0
+Version: 0.6.3a0
 Summary: Mrsal is a simple to use message broker abstraction on top of RabbitMQ and Pika.
 Keywords: message broker,RabbitMQ,Pika,Mrsal
 Author: Raafat
 Author-email: rafatzahran90@gmail.com
 Maintainer: Raafat
 Maintainer-email: rafatzahran90@gmail.com
 Requires-Python: >=3.10,<4.0
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: colorlog (>=6.7.0,<7.0.0)
 Requires-Dist: pika (>=1.3.0,<2.0.0)
 Requires-Dist: retry (>=0.9.2,<0.10.0)
 Description-Content-Type: text/markdown
 
 # MRSAL  <img align="right" width="125" alt="20200907_104224" src="https://github.com/NeoMedSys/mrsal/assets/9555305/ffb55c86-1e9d-4806-b1ca-c906d6985e3a">
-[![Release](https://img.shields.io/badge/release-v0.6.2--alpha-blue.svg)](https://pypi.org/project/mrsal/) [![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)](https://www.python.org/downloads/release/python-3103/) [![Documentation](https://img.shields.io/badge/doc-latest-blue.svg)](https://github.com/NeoMedSys/mrsal/blob/main/FullGuide.md)
+[![Release](https://img.shields.io/badge/release-v0.6.3--alpha-blue.svg)](https://pypi.org/project/mrsal/) [![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)](https://www.python.org/downloads/release/python-3103/) [![Documentation](https://img.shields.io/badge/doc-latest-blue.svg)](https://github.com/NeoMedSys/mrsal/blob/main/FullGuide.md)
 <!-- [![Build Status](https://github.com/NeoMedSys/fatty-model-deploy/actions/workflows/tester.yml/badge.svg)](https://github.com/NeoMedSys/fatty-model-deploy/actions/runs/5576890234) -->
 [![Tests Status](https://github.com/NeoMedSys/mrsal/assets/9555305/5d29b991-1e7f-4737-8e55-5ee2bc9bb5db)](./reports/junit/junit.xml) [![Coverage Status](https://github.com/NeoMedSys/mrsal/assets/9555305/852b4256-d52e-49da-9134-f0e7381935ba)](./reports/coverage/htmlcov/index.html) [![Flake8 Status](https://github.com/NeoMedSys/mrsal/assets/9555305/0113f279-7c5c-4ed8-bd2f-8b2cf84da2a9)](./reports/flake8/flake8.txt)
 
 ## Intro
 Mrsal is a simple to use message broker abstraction on top of [RabbitMQ](https://www.rabbitmq.com/) and [Pika](https://pika.readthedocs.io/en/stable/index.html). The goal is to make Mrsal trivial to re-use in all services of a distributed system and to make the use of advanced message queing protocols easy and safe. No more big chunks of repetive code across your services or bespoke solutions to handle dead letters. 
 
 ###### Mrsal is Arabic for a small arrow and is used to describe something that performs a task with lightness and speed.
```

