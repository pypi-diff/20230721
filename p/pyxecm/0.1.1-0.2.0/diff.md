# Comparing `tmp/pyxecm-0.1.1.tar.gz` & `tmp/pyxecm-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyxecm-0.1.1.tar", last modified: Thu Jul 13 17:23:38 2023, max compression
+gzip compressed data, was "pyxecm-0.2.0.tar", last modified: Fri Jul 21 13:57:32 2023, max compression
```

## Comparing `pyxecm-0.1.1.tar` & `pyxecm-0.2.0.tar`

### file list

```diff
@@ -1,24 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 17:23:38.685356 pyxecm-0.1.1/
--rw-rw-rw-   0 root         (0) root         (0)    11360 2023-07-13 17:23:13.000000 pyxecm-0.1.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1640 2023-07-13 17:23:38.685356 pyxecm-0.1.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      854 2023-07-13 17:23:13.000000 pyxecm-0.1.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1087 2023-07-13 17:23:28.000000 pyxecm-0.1.1/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 17:23:38.683356 pyxecm-0.1.1/pyxecm/
--rw-rw-rw-   0 root         (0) root         (0)      176 2023-07-13 17:23:13.000000 pyxecm-0.1.1/pyxecm/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4518 2023-07-13 17:23:13.000000 pyxecm-0.1.1/pyxecm/assoc.py
--rw-rw-rw-   0 root         (0) root         (0)    33675 2023-07-13 17:23:13.000000 pyxecm-0.1.1/pyxecm/k8s.py
--rw-rw-rw-   0 root         (0) root         (0)     9536 2023-07-13 17:23:13.000000 pyxecm-0.1.1/pyxecm/otac.py
--rw-rw-rw-   0 root         (0) root         (0)   256444 2023-07-13 17:23:13.000000 pyxecm-0.1.1/pyxecm/otcs.py
--rw-rw-rw-   0 root         (0) root         (0)   129331 2023-07-13 17:23:13.000000 pyxecm-0.1.1/pyxecm/otds.py
--rw-rw-rw-   0 root         (0) root         (0)     1609 2023-07-13 17:23:13.000000 pyxecm-0.1.1/pyxecm/otiv.py
--rw-rw-rw-   0 root         (0) root         (0)    10222 2023-07-13 17:23:13.000000 pyxecm-0.1.1/pyxecm/otpd.py
--rw-rw-rw-   0 root         (0) root         (0)     2701 2023-07-13 17:23:13.000000 pyxecm-0.1.1/pyxecm/web.py
--rw-rw-rw-   0 root         (0) root         (0)    21830 2023-07-13 17:23:13.000000 pyxecm-0.1.1/pyxecm/xml.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 17:23:38.685356 pyxecm-0.1.1/pyxecm.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1640 2023-07-13 17:23:38.000000 pyxecm-0.1.1/pyxecm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      342 2023-07-13 17:23:38.000000 pyxecm-0.1.1/pyxecm.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 17:23:38.000000 pyxecm-0.1.1/pyxecm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       66 2023-07-13 17:23:38.000000 pyxecm-0.1.1/pyxecm.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-07-13 17:23:38.000000 pyxecm-0.1.1/pyxecm.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-13 17:23:38.685356 pyxecm-0.1.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       37 2023-07-13 17:23:13.000000 pyxecm-0.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 13:57:32.891350 pyxecm-0.2.0/
+-rw-rw-rw-   0 root         (0) root         (0)    11360 2023-07-21 13:57:10.000000 pyxecm-0.2.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1640 2023-07-21 13:57:32.891350 pyxecm-0.2.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      854 2023-07-21 13:57:10.000000 pyxecm-0.2.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1087 2023-07-21 13:57:22.000000 pyxecm-0.2.0/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 13:57:32.889351 pyxecm-0.2.0/pyxecm/
+-rw-rw-rw-   0 root         (0) root         (0)      241 2023-07-21 13:57:10.000000 pyxecm-0.2.0/pyxecm/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    59539 2023-07-21 13:57:10.000000 pyxecm-0.2.0/pyxecm/customizer.py
+-rw-rw-rw-   0 root         (0) root         (0)    33679 2023-07-21 13:57:10.000000 pyxecm-0.2.0/pyxecm/k8s.py
+-rw-rw-rw-   0 root         (0) root         (0)    77601 2023-07-21 13:57:10.000000 pyxecm-0.2.0/pyxecm/m365.py
+-rw-rw-rw-   0 root         (0) root         (0)     9541 2023-07-21 13:57:10.000000 pyxecm-0.2.0/pyxecm/otac.py
+-rw-rw-rw-   0 root         (0) root         (0)   256630 2023-07-21 13:57:10.000000 pyxecm-0.2.0/pyxecm/otcs.py
+-rw-rw-rw-   0 root         (0) root         (0)   129336 2023-07-21 13:57:10.000000 pyxecm-0.2.0/pyxecm/otds.py
+-rw-rw-rw-   0 root         (0) root         (0)     1605 2023-07-21 13:57:10.000000 pyxecm-0.2.0/pyxecm/otiv.py
+-rw-rw-rw-   0 root         (0) root         (0)    10227 2023-07-21 13:57:10.000000 pyxecm-0.2.0/pyxecm/otpd.py
+-rw-rw-rw-   0 root         (0) root         (0)   289068 2023-07-21 13:57:10.000000 pyxecm-0.2.0/pyxecm/payload.py
+-rw-rw-rw-   0 root         (0) root         (0)     5907 2023-07-21 13:57:10.000000 pyxecm-0.2.0/pyxecm/sap.py
+-rw-rw-rw-   0 root         (0) root         (0)     2705 2023-07-21 13:57:10.000000 pyxecm-0.2.0/pyxecm/translate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 13:57:32.890350 pyxecm-0.2.0/pyxecm.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1640 2023-07-21 13:57:32.000000 pyxecm-0.2.0/pyxecm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      386 2023-07-21 13:57:32.000000 pyxecm-0.2.0/pyxecm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 13:57:32.000000 pyxecm-0.2.0/pyxecm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       66 2023-07-21 13:57:32.000000 pyxecm-0.2.0/pyxecm.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-21 13:57:32.000000 pyxecm-0.2.0/pyxecm.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-21 13:57:32.891350 pyxecm-0.2.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       37 2023-07-21 13:57:10.000000 pyxecm-0.2.0/setup.py
```

### Comparing `pyxecm-0.1.1/LICENSE` & `pyxecm-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyxecm-0.1.1/PKG-INFO` & `pyxecm-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyxecm
-Version: 0.1.1
+Version: 0.2.0
 Summary: A Python library to interact with Opentext Extended ECM REST API
 Author-email: Kai Gatzweiler <kgatzweiler@opentext.com>, "Dr. Marc Diefenbruch" <mdiefenb@opentext.com>
 Project-URL: Homepage, https://ecm.glpages.otxlab.net/pyxecm/
 Keywords: opentext,extendedecm,contentserver,otds,appworks,archivecenter
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `pyxecm-0.1.1/README.md` & `pyxecm-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pyxecm-0.1.1/pyproject.toml` & `pyxecm-0.2.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -7,15 +7,15 @@
   classifiers = ["Development Status :: 4 - Beta", "Programming Language :: Python :: 3", "License :: OSI Approved :: Apache Software License", "Operating System :: OS Independent", "Intended Audience :: Developers", "Topic :: Internet :: WWW/HTTP :: Dynamic Content :: Content Management System"]
   dependencies = ["requests < 3", "requests_toolbelt", "setuptools", "kubernetes", "zipfile36", "suds"]
   description = "A Python library to interact with Opentext Extended ECM REST API"
   keywords = ["opentext", "extendedecm", "contentserver", "otds", "appworks", "archivecenter"]
   name = "pyxecm"
   readme = "README.md"
   requires-python = ">=3.10"
-  version = "0.1.1"
+  version = "0.2.0"
 
   [[project.authors]]
     email = "kgatzweiler@opentext.com"
     name = "Kai Gatzweiler"
 
   [[project.authors]]
     email = "mdiefenb@opentext.com"
```

### Comparing `pyxecm-0.1.1/pyxecm/k8s.py` & `pyxecm-0.2.0/pyxecm/k8s.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 from kubernetes import client, config
 from kubernetes.stream import stream
 from kubernetes.client.exceptions import ApiException
 
 # Configure Kubernetes API authentication to use pod serviceAccount
 # config.load_incluster_config()
 
-logger = logging.getLogger("pyxecm")
+logger = logging.getLogger("pyxecm.k8s")
 
 class K8s(object):
     """Used to automate stettings in Kubernetes."""
 
     _core_v1_api = None
     _apps_v1_api = None
     _networking_v1_api = None
```

### Comparing `pyxecm-0.1.1/pyxecm/otac.py` & `pyxecm-0.2.0/pyxecm/otac.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 import requests
 import os
 import logging
 import base64
 
 from suds.client import Client
 
-logger = logging.getLogger("pyxecm")
+logger = logging.getLogger("pyxecm.otac")
 
 requestHeaders = {"Content-Type": "application/x-www-form-urlencoded"}
 
 
 class OTAC:
     """Used to automate stettings in OpenText Archive Center."""
```

### Comparing `pyxecm-0.1.1/pyxecm/otcs.py` & `pyxecm-0.2.0/pyxecm/otcs.py`

 * *Files 0% similar despite different names*

```diff
@@ -148,17 +148,17 @@
 import os
 import logging
 import requests
 import json
 import urllib.parse
 from datetime import datetime
 import zipfile
-from .xml import XML
+from pyxecm.helper.xml import XML
 
-logger = logging.getLogger("pyxecm")
+logger = logging.getLogger("pyxecm.otcs")
 
 requestJsonHeaders = {
     "accept": "application/json;charset=utf-8",
     "Content-Type": "application/json",
 }
 
 requestFormHeaders = {
@@ -168,18 +168,18 @@
 
 requestDownloadHeaders = {
     "accept": "application/octet-stream",
     "Content-Type": "application/json",
 }
 
 
-class OTCS(object):
+class OTCS:
     """Used to automate stettings in OpenText Extended ECM."""
 
-    _config = None
+    _config: dict
     _cookie = None
 
     def __init__(
         self,
         protocol: str,
         hostname: str,
         port: int,
@@ -625,28 +625,28 @@
 
     def getResultValue(
         self,
         response: dict,
         key: str,
         index: int = 0,
         property_name: str = "properties",
-    ) -> str:
+    ) -> int:
         """Read an item value from the REST API response. This is considering
            the most typical structures delivered by V2 REST API of Extended ECM.
            See developer.opentext.com for more details.
 
         Args:
             response (dictionary): REST API response object
             key (string): key to find (e.g. "id", "name", ...)
             index (integer, optional): In case a list of results is delivered the index
                                        to use (1st element has index  0). Defaults to 0.
             property_name (string, optional): name of the sub dictionary holding the actual values.
                                               Default is "properties".
         Returns:
-            string: value of the item with the given key
+            int: value of the item with the given key
         """
 
         # First do some sanity checks:
         if not response:
             logger.info("Empty REST response - returning None")
             return None
         if not "results" in response:
@@ -946,26 +946,26 @@
     def addUser(
         self,
         name: str,
         password: str,
         first_name: str,
         last_name: str,
         email: str,
-        base_group: str,
+        base_group: int,
         privileges: list = ["Login", "Public Access"],
     ) -> dict:
         """Add Content Server user.
 
         Args:
             name (string): login name of the user
             password (string): password of the user
             first_name (string): first name of the user
             last_name (string): last name of the user
             email (string): email address of the user
-            base_group (string): base group of the user (e.g. department)
+            base_group (int): base group id of the user (e.g. department)
             privileges (list, optional): values are Login, Public Access, Content Manager,
                                          Modify Users, Modify Groups, User Admin Rights,
                                          Grant Discovery, System Admin Rights
         Returns:
             dictionary: User information or None if the user couldn't be created (e.g. because it exisits already).
         """
 
@@ -3249,19 +3249,23 @@
             zfile.extractall(zip_file_folder)
 
         modified = False
 
         # Replace search pattern with replace string in all XML files in the directory and its subdirectories
         for replacement in replacements:
             if not "value" in replacement:
-                logger.error("Replacement needs a value but it is not specified. Skipping...")
+                logger.error(
+                    "Replacement needs a value but it is not specified. Skipping..."
+                )
                 continue
             if "enabled" in replacement and not replacement["enabled"]:
                 logger.info(
-                    "Replacement for transport -> {} is disabled. Skipping...".format(zip_file_path)
+                    "Replacement for transport -> {} is disabled. Skipping...".format(
+                        zip_file_path
+                    )
                 )
                 continue
             # there are two types of replacements:
             # 1. XPath - more elegant and powerful
             # 2. Search & Replace - basically treat the XML file like a like file and do a search & replace
             if "xpath" in replacement:
                 logger.info(
@@ -3277,28 +3281,32 @@
                     )
                 if "assoc_elem" in replacement:
                     logger.info(
                         "Looking up assoc element -> {} in XML element".format(
                             replacement["assoc_elem"]
                         )
                     )
-            else: # we have a simple "search & replace" replacement
+            else:  # we have a simple "search & replace" replacement
                 if not "placeholder" in replacement:
-                    logger.error("Replacement without an xpath needs a placeholder value but it is not specified. Skipping...")
+                    logger.error(
+                        "Replacement without an xpath needs a placeholder value but it is not specified. Skipping..."
+                    )
                     continue
                 if replacement.get("placeholder") == replacement["value"]:
                     logger.info(
                         "Placeholder and replacement are identical -> {}. Skipping...".format(
                             replacement["value"]
                         )
                     )
                     continue
                 logger.info(
                     "Replace -> {} with -> {} in Transport package -> {}".format(
-                        replacement["placeholder"], replacement["value"], zip_file_folder
+                        replacement["placeholder"],
+                        replacement["value"],
+                        zip_file_folder,
                     )
                 )
 
             found = XML.replaceInXmlFiles(
                 zip_file_folder,
                 replacement.get("placeholder"),
                 replacement["value"],
```

### Comparing `pyxecm-0.1.1/pyxecm/otds.py` & `pyxecm-0.2.0/pyxecm/otds.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,15 +92,15 @@
 
 import os
 import logging
 import requests
 import json
 import base64
 
-logger = logging.getLogger("pyxecm")
+logger = logging.getLogger("pyxecm.otpd")
 
 requestHeaders = {
     "accept": "application/json;charset=utf-8",
     "Content-Type": "application/json",
 }
 
 requestFormHeaders = {
```

### Comparing `pyxecm-0.1.1/pyxecm/otiv.py` & `pyxecm-0.2.0/pyxecm/otiv.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,21 +14,21 @@
 __credits__ = ["Kai-Philip Gatzweiler"]
 __maintainer__ = "Dr. Marc Diefenbruch"
 __email__ = "mdiefenb@opentext.com"
 
 import os
 import logging
 
-logger = logging.getLogger("pyxecm")
+logger = logging.getLogger("pyxecm.otiv")
 
 
-class OTIV(object):
+class OTIV:
     """Used to manage stettings for OpenText Intelligent Viewing."""
 
-    _config = None
+    _config: dict
 
     def __init__(
         self,
         resource_name: str,
         product_name: str,
         product_description: str,
         license_file: str,
```

### Comparing `pyxecm-0.1.1/pyxecm/otpd.py` & `pyxecm-0.2.0/pyxecm/otpd.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 import json
 import requests
 from requests.auth import HTTPBasicAuth
 from requests_toolbelt.multipart.encoder import MultipartEncoder
 import os
 import logging
 
-logger = logging.getLogger("pyxecm")
+logger = logging.getLogger("pyxecm.otpd")
 
 requestHeaders = {
     "accept": "application/json;charset=utf-8",
     "Connection": "keep-alive",
     "Content-Type": "application/json",
 }
```

### Comparing `pyxecm-0.1.1/pyxecm.egg-info/PKG-INFO` & `pyxecm-0.2.0/pyxecm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyxecm
-Version: 0.1.1
+Version: 0.2.0
 Summary: A Python library to interact with Opentext Extended ECM REST API
 Author-email: Kai Gatzweiler <kgatzweiler@opentext.com>, "Dr. Marc Diefenbruch" <mdiefenb@opentext.com>
 Project-URL: Homepage, https://ecm.glpages.otxlab.net/pyxecm/
 Keywords: opentext,extendedecm,contentserver,otds,appworks,archivecenter
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

