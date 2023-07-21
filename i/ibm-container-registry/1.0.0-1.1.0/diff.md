# Comparing `tmp/ibm-container-registry-1.0.0.tar.gz` & `tmp/ibm-container-registry-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ibm-container-registry-1.0.0.tar", last modified: Wed Jun 21 08:32:39 2023, max compression
+gzip compressed data, was "dist/ibm-container-registry-1.1.0.tar", last modified: Fri Jul 21 14:16:57 2023, max compression
```

## Comparing `ibm-container-registry-1.0.0.tar` & `ibm-container-registry-1.1.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-21 08:32:39.000000 ibm-container-registry-1.0.0/
--rw-rw-r--   0 travis    (2000) travis    (2000)    11357 2023-06-21 08:29:48.000000 ibm-container-registry-1.0.0/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)       70 2023-06-21 08:29:48.000000 ibm-container-registry-1.0.0/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)     4209 2023-06-21 08:32:39.000000 ibm-container-registry-1.0.0/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     3262 2023-06-21 08:29:48.000000 ibm-container-registry-1.0.0/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-21 08:32:39.000000 ibm-container-registry-1.0.0/ibm_container_registry/
--rw-rw-r--   0 travis    (2000) travis    (2000)      872 2023-06-21 08:29:48.000000 ibm-container-registry-1.0.0/ibm_container_registry/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2425 2023-06-21 08:29:48.000000 ibm-container-registry-1.0.0/ibm_container_registry/common.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   127358 2023-06-21 08:29:48.000000 ibm-container-registry-1.0.0/ibm_container_registry/container_registry_v1.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      667 2023-06-21 08:29:48.000000 ibm-container-registry-1.0.0/ibm_container_registry/version.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    97619 2023-06-21 08:29:48.000000 ibm-container-registry-1.0.0/ibm_container_registry/vulnerability_advisor_v4.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-21 08:32:39.000000 ibm-container-registry-1.0.0/ibm_container_registry.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4209 2023-06-21 08:32:39.000000 ibm-container-registry-1.0.0/ibm_container_registry.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      547 2023-06-21 08:32:39.000000 ibm-container-registry-1.0.0/ibm_container_registry.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-06-21 08:32:39.000000 ibm-container-registry-1.0.0/ibm_container_registry.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       85 2023-06-21 08:32:39.000000 ibm-container-registry-1.0.0/ibm_container_registry.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       23 2023-06-21 08:32:39.000000 ibm-container-registry-1.0.0/ibm_container_registry.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-06-21 08:30:27.000000 ibm-container-registry-1.0.0/ibm_container_registry.egg-info/zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)      173 2023-06-21 08:29:48.000000 ibm-container-registry-1.0.0/requirements-dev.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       85 2023-06-21 08:29:48.000000 ibm-container-registry-1.0.0/requirements.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2023-06-21 08:32:39.000000 ibm-container-registry-1.0.0/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     2609 2023-06-21 08:29:48.000000 ibm-container-registry-1.0.0/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-21 14:16:57.000000 ibm-container-registry-1.1.0/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11357 2023-07-21 14:14:03.000000 ibm-container-registry-1.1.0/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)       70 2023-07-21 14:14:03.000000 ibm-container-registry-1.1.0/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4209 2023-07-21 14:16:57.000000 ibm-container-registry-1.1.0/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3262 2023-07-21 14:14:03.000000 ibm-container-registry-1.1.0/README.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-21 14:16:57.000000 ibm-container-registry-1.1.0/ibm_container_registry/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      872 2023-07-21 14:14:03.000000 ibm-container-registry-1.1.0/ibm_container_registry/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2425 2023-07-21 14:14:03.000000 ibm-container-registry-1.1.0/ibm_container_registry/common.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   127407 2023-07-21 14:14:03.000000 ibm-container-registry-1.1.0/ibm_container_registry/container_registry_v1.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      667 2023-07-21 14:14:03.000000 ibm-container-registry-1.1.0/ibm_container_registry/version.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    97619 2023-07-21 14:14:03.000000 ibm-container-registry-1.1.0/ibm_container_registry/vulnerability_advisor_v4.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-21 14:16:57.000000 ibm-container-registry-1.1.0/ibm_container_registry.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4209 2023-07-21 14:16:57.000000 ibm-container-registry-1.1.0/ibm_container_registry.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)      547 2023-07-21 14:16:57.000000 ibm-container-registry-1.1.0/ibm_container_registry.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-07-21 14:16:57.000000 ibm-container-registry-1.1.0/ibm_container_registry.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       85 2023-07-21 14:16:57.000000 ibm-container-registry-1.1.0/ibm_container_registry.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       23 2023-07-21 14:16:57.000000 ibm-container-registry-1.1.0/ibm_container_registry.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-07-21 14:14:43.000000 ibm-container-registry-1.1.0/ibm_container_registry.egg-info/zip-safe
+-rw-rw-r--   0 travis    (2000) travis    (2000)      173 2023-07-21 14:14:03.000000 ibm-container-registry-1.1.0/requirements-dev.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       85 2023-07-21 14:14:03.000000 ibm-container-registry-1.1.0/requirements.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       38 2023-07-21 14:16:57.000000 ibm-container-registry-1.1.0/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2609 2023-07-21 14:14:03.000000 ibm-container-registry-1.1.0/setup.py
```

### Comparing `ibm-container-registry-1.0.0/LICENSE` & `ibm-container-registry-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ibm-container-registry-1.0.0/PKG-INFO` & `ibm-container-registry-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibm-container-registry
-Version: 1.0.0
+Version: 1.1.0
 Summary: IBM Cloud Container Registry Python SDK
 Home-page: https://github.com/IBM/container-registry-python-sdk
 Author: IBM
 Author-email: alchemy.registry.squad@uk.ibm.com
 License: Apache 2.0
 Keywords: ibm_container_registry
 Classifier: Programming Language :: Python
@@ -75,21 +75,21 @@
 * Python 3.7 or above.
 
 ## Installation
 
 To install, use `pip` or `easy_install`:
 
 ```bash
-pip install --upgrade "ibm-container-registry>=1.0.0"
+pip install --upgrade "ibm-container-registry>=1.1.0"
 ```
 
 or
 
 ```bash
-easy_install --upgrade "ibm-container-registry>=1.0.0"
+easy_install --upgrade "ibm-container-registry>=1.1.0"
 ```
 
 ## Using the SDK
 For general SDK usage information, please see [this link](https://github.com/IBM/ibm-cloud-sdk-common/blob/main/README.md)
 
 ## Questions
```

### Comparing `ibm-container-registry-1.0.0/README.md` & `ibm-container-registry-1.1.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -52,21 +52,21 @@
 * Python 3.7 or above.
 
 ## Installation
 
 To install, use `pip` or `easy_install`:
 
 ```bash
-pip install --upgrade "ibm-container-registry>=1.0.0"
+pip install --upgrade "ibm-container-registry>=1.1.0"
 ```
 
 or
 
 ```bash
-easy_install --upgrade "ibm-container-registry>=1.0.0"
+easy_install --upgrade "ibm-container-registry>=1.1.0"
 ```
 
 ## Using the SDK
 For general SDK usage information, please see [this link](https://github.com/IBM/ibm-cloud-sdk-common/blob/main/README.md)
 
 ## Questions
```

### Comparing `ibm-container-registry-1.0.0/ibm_container_registry/__init__.py` & `ibm-container-registry-1.1.0/ibm_container_registry/__init__.py`

 * *Files identical despite different names*

### Comparing `ibm-container-registry-1.0.0/ibm_container_registry/common.py` & `ibm-container-registry-1.1.0/ibm_container_registry/common.py`

 * *Files identical despite different names*

### Comparing `ibm-container-registry-1.0.0/ibm_container_registry/container_registry_v1.py` & `ibm-container-registry-1.1.0/ibm_container_registry/container_registry_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-# IBM OpenAPI SDK Code Generator Version: 3.73.0-eeee85a9-20230607-165104
+# IBM OpenAPI SDK Code Generator Version: 3.75.0-726bc7e3-20230713-221716
 
 """
 Management interface for IBM Cloud Container Registry
 
 API Version: 1.1
 """
 
@@ -52,14 +52,15 @@
         'ap-north': 'https://jp.icr.io', # ap-north
         'jp-tok': 'https://jp.icr.io', # jp-tok
         'ap-south': 'https://au.icr.io', # ap-south
         'au-syd': 'https://au.icr.io', # au-syd
         'jp-osa': 'https://jp2.icr.io', # jp-osa
         'ca-tor': 'https://ca.icr.io', # ca-tor
         'br-sao': 'https://br.icr.io', # br-sao
+        'eu-fr2': 'https://fr2.icr.io', # eu-fr2
     }
 
     @classmethod
     def new_instance(
         cls,
         account: str,
         service_name: str = DEFAULT_SERVICE_NAME,
```

### Comparing `ibm-container-registry-1.0.0/ibm_container_registry/version.py` & `ibm-container-registry-1.1.0/ibm_container_registry/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
 Version of ibm_container_registry
 """
-__version__ = '1.0.0'
+__version__ = '1.1.0'
```

### Comparing `ibm-container-registry-1.0.0/ibm_container_registry/vulnerability_advisor_v4.py` & `ibm-container-registry-1.1.0/ibm_container_registry/vulnerability_advisor_v4.py`

 * *Files identical despite different names*

### Comparing `ibm-container-registry-1.0.0/ibm_container_registry.egg-info/PKG-INFO` & `ibm-container-registry-1.1.0/ibm_container_registry.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibm-container-registry
-Version: 1.0.0
+Version: 1.1.0
 Summary: IBM Cloud Container Registry Python SDK
 Home-page: https://github.com/IBM/container-registry-python-sdk
 Author: IBM
 Author-email: alchemy.registry.squad@uk.ibm.com
 License: Apache 2.0
 Keywords: ibm_container_registry
 Classifier: Programming Language :: Python
@@ -75,21 +75,21 @@
 * Python 3.7 or above.
 
 ## Installation
 
 To install, use `pip` or `easy_install`:
 
 ```bash
-pip install --upgrade "ibm-container-registry>=1.0.0"
+pip install --upgrade "ibm-container-registry>=1.1.0"
 ```
 
 or
 
 ```bash
-easy_install --upgrade "ibm-container-registry>=1.0.0"
+easy_install --upgrade "ibm-container-registry>=1.1.0"
 ```
 
 ## Using the SDK
 For general SDK usage information, please see [this link](https://github.com/IBM/ibm-cloud-sdk-common/blob/main/README.md)
 
 ## Questions
```

### Comparing `ibm-container-registry-1.0.0/ibm_container_registry.egg-info/SOURCES.txt` & `ibm-container-registry-1.1.0/ibm_container_registry.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ibm-container-registry-1.0.0/setup.py` & `ibm-container-registry-1.1.0/setup.py`

 * *Files identical despite different names*

```diff
@@ -15,15 +15,15 @@
 
 from setuptools import setup
 from setuptools.command.test import test as TestCommand
 import os
 import sys
 import pkg_resources
 
-__version__ = '1.0.0'
+__version__ = '1.1.0'
 PACKAGE_NAME = 'ibm_container_registry'
 PACKAGE_DESC = 'IBM Cloud Container Registry Python SDK'
 
 with open('requirements.txt') as f:
     install_requires = [
         str(req) for req in pkg_resources.parse_requirements(f)
     ]
```

