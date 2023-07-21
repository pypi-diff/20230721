# Comparing `tmp/bullhorn-0.0.2.tar.gz` & `tmp/bullhorn-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bullhorn-0.0.2.tar", last modified: Fri Jul  7 07:52:32 2023, max compression
+gzip compressed data, was "bullhorn-0.0.4.tar", last modified: Fri Jul 21 16:23:12 2023, max compression
```

## Comparing `bullhorn-0.0.2.tar` & `bullhorn-0.0.4.tar`

### file list

```diff
@@ -1,29 +1,47 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 07:52:32.496494 bullhorn-0.0.2/
--rw-rw-rw-   0        0        0     1088 2023-07-07 06:22:40.000000 bullhorn-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      532 2023-07-07 07:52:32.494491 bullhorn-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       66 2023-06-05 13:48:02.000000 bullhorn-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-07 07:52:32.410265 bullhorn-0.0.2/bullhorn/
--rw-rw-rw-   0        0        0       93 2023-07-07 07:50:10.000000 bullhorn-0.0.2/bullhorn/__init__.py
--rw-rw-rw-   0        0        0     6371 2023-07-07 07:48:05.000000 bullhorn-0.0.2/bullhorn/client.py
--rw-rw-rw-   0        0        0     4924 2023-07-07 06:20:06.000000 bullhorn-0.0.2/bullhorn/exceptions.py
--rw-rw-rw-   0        0        0     1739 2023-07-07 06:25:00.000000 bullhorn-0.0.2/bullhorn/route.py
-drwxrwxrwx   0        0        0        0 2023-07-07 07:52:32.476442 bullhorn-0.0.2/bullhorn/types/
--rw-rw-rw-   0        0        0        0 2023-06-06 16:02:11.000000 bullhorn-0.0.2/bullhorn/types/__init__.py
--rw-rw-rw-   0        0        0       70 2023-07-07 06:28:51.000000 bullhorn-0.0.2/bullhorn/types/candidate.py
--rw-rw-rw-   0        0        0       38 2023-06-13 12:11:53.000000 bullhorn-0.0.2/bullhorn/types/ping.py
--rw-rw-rw-   0        0        0      216 2023-07-07 06:10:37.000000 bullhorn-0.0.2/bullhorn/types/placement.py
-drwxrwxrwx   0        0        0        0 2023-07-07 07:52:32.465411 bullhorn-0.0.2/bullhorn.egg-info/
--rw-rw-rw-   0        0        0      532 2023-07-07 07:52:32.000000 bullhorn-0.0.2/bullhorn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      494 2023-07-07 07:52:32.000000 bullhorn-0.0.2/bullhorn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 07:52:32.000000 bullhorn-0.0.2/bullhorn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       79 2023-07-07 07:52:32.000000 bullhorn-0.0.2/bullhorn.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2023-07-07 07:52:32.000000 bullhorn-0.0.2/bullhorn.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-07 07:52:32.481456 bullhorn-0.0.2/examples/
--rw-rw-rw-   0        0        0        0 2023-06-06 16:02:11.000000 bullhorn-0.0.2/examples/__init__.py
--rw-rw-rw-   0        0        0      845 2023-07-07 07:48:13.000000 bullhorn-0.0.2/examples/get_placements_and_candidates.py
--rw-rw-rw-   0        0        0       42 2023-07-07 07:52:32.497496 bullhorn-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      867 2023-07-07 07:52:06.000000 bullhorn-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-07 07:52:32.490479 bullhorn-0.0.2/tests/
--rw-rw-rw-   0        0        0        0 2023-06-06 16:33:32.000000 bullhorn-0.0.2/tests/__init__.py
--rw-rw-rw-   0        0        0      994 2023-07-07 07:48:16.000000 bullhorn-0.0.2/tests/test_client.py
--rw-rw-rw-   0        0        0     1074 2023-07-04 16:16:33.000000 bullhorn-0.0.2/tests/test_route.py
+drwxrwxrwx   0        0        0        0 2023-07-21 16:23:12.115668 bullhorn-0.0.4/
+-rw-rw-rw-   0        0        0     1088 2023-07-07 06:22:40.000000 bullhorn-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     2240 2023-07-21 16:23:12.112628 bullhorn-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1774 2023-07-21 16:19:15.000000 bullhorn-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-21 16:23:11.954877 bullhorn-0.0.4/bullhorn/
+-rw-rw-rw-   0        0        0       93 2023-07-21 16:21:50.000000 bullhorn-0.0.4/bullhorn/__init__.py
+-rw-rw-rw-   0        0        0     8313 2023-07-21 15:12:58.000000 bullhorn-0.0.4/bullhorn/client.py
+-rw-rw-rw-   0        0        0     4864 2023-07-21 10:35:13.000000 bullhorn-0.0.4/bullhorn/exceptions.py
+-rw-rw-rw-   0        0        0     1739 2023-07-21 10:35:17.000000 bullhorn-0.0.4/bullhorn/route.py
+drwxrwxrwx   0        0        0        0 2023-07-21 16:23:12.087562 bullhorn-0.0.4/bullhorn/types/
+-rw-rw-rw-   0        0        0        0 2023-06-06 16:02:11.000000 bullhorn-0.0.4/bullhorn/types/__init__.py
+-rw-rw-rw-   0        0        0       32 2023-07-21 13:35:23.000000 bullhorn-0.0.4/bullhorn/types/agreement_line.py
+-rw-rw-rw-   0        0        0       33 2023-07-21 13:35:23.000000 bullhorn-0.0.4/bullhorn/types/billing_profile.py
+-rw-rw-rw-   0        0        0       25 2023-07-21 13:35:23.000000 bullhorn-0.0.4/bullhorn/types/branch.py
+-rw-rw-rw-   0        0        0     7532 2023-07-21 14:49:16.000000 bullhorn-0.0.4/bullhorn/types/candidate.py
+-rw-rw-rw-   0        0        0       27 2023-07-21 13:38:39.000000 bullhorn-0.0.4/bullhorn/types/category.py
+-rw-rw-rw-   0        0        0     3805 2023-07-21 13:36:23.000000 bullhorn-0.0.4/bullhorn/types/client_contact.py
+-rw-rw-rw-   0        0        0     2594 2023-07-21 14:10:39.000000 bullhorn-0.0.4/bullhorn/types/client_corporation.py
+-rw-rw-rw-   0        0        0      748 2023-07-21 11:40:00.000000 bullhorn-0.0.4/bullhorn/types/corporate_user.py
+-rw-rw-rw-   0        0        0       26 2023-07-21 13:54:17.000000 bullhorn-0.0.4/bullhorn/types/job_code.py
+-rw-rw-rw-   0        0        0     4816 2023-07-21 13:43:16.000000 bullhorn-0.0.4/bullhorn/types/job_order.py
+-rw-rw-rw-   0        0        0       32 2023-07-21 13:33:13.000000 bullhorn-0.0.4/bullhorn/types/job_submission.py
+-rw-rw-rw-   0        0        0       23 2023-07-21 13:54:17.000000 bullhorn-0.0.4/bullhorn/types/lead.py
+-rw-rw-rw-   0        0        0       27 2023-07-21 13:54:17.000000 bullhorn-0.0.4/bullhorn/types/location.py
+-rw-rw-rw-   0        0        0     3098 2023-07-21 13:54:17.000000 bullhorn-0.0.4/bullhorn/types/opportunity.py
+-rw-rw-rw-   0        0        0       81 2023-07-21 13:32:38.000000 bullhorn-0.0.4/bullhorn/types/person.py
+-rw-rw-rw-   0        0        0       38 2023-06-13 12:11:53.000000 bullhorn-0.0.4/bullhorn/types/ping.py
+-rw-rw-rw-   0        0        0     8325 2023-07-21 13:38:40.000000 bullhorn-0.0.4/bullhorn/types/placement.py
+-rw-rw-rw-   0        0        0      477 2023-07-21 14:58:56.000000 bullhorn-0.0.4/bullhorn/types/placement_commission.py
+-rw-rw-rw-   0        0        0      572 2023-07-21 13:36:49.000000 bullhorn-0.0.4/bullhorn/types/shift.py
+-rw-rw-rw-   0        0        0      190 2023-07-21 13:54:17.000000 bullhorn-0.0.4/bullhorn/types/workers_compensation.py
+-rw-rw-rw-   0        0        0      213 2023-07-21 13:54:17.000000 bullhorn-0.0.4/bullhorn/types/workers_compensation_rate.py
+drwxrwxrwx   0        0        0        0 2023-07-21 16:23:11.983303 bullhorn-0.0.4/bullhorn.egg-info/
+-rw-rw-rw-   0        0        0     2240 2023-07-21 16:23:11.000000 bullhorn-0.0.4/bullhorn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1055 2023-07-21 16:23:11.000000 bullhorn-0.0.4/bullhorn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 16:23:11.000000 bullhorn-0.0.4/bullhorn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-07-21 16:23:11.000000 bullhorn-0.0.4/bullhorn.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2023-07-21 16:23:11.000000 bullhorn-0.0.4/bullhorn.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-21 16:23:12.095583 bullhorn-0.0.4/examples/
+-rw-rw-rw-   0        0        0        0 2023-06-06 16:02:11.000000 bullhorn-0.0.4/examples/__init__.py
+-rw-rw-rw-   0        0        0      845 2023-07-21 10:46:50.000000 bullhorn-0.0.4/examples/get_placements_and_candidates.py
+-rw-rw-rw-   0        0        0       42 2023-07-21 16:23:12.116672 bullhorn-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      842 2023-07-21 10:38:28.000000 bullhorn-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 16:23:12.106611 bullhorn-0.0.4/tests/
+-rw-rw-rw-   0        0        0        0 2023-06-06 16:33:32.000000 bullhorn-0.0.4/tests/__init__.py
+-rw-rw-rw-   0        0        0     8197 2023-07-21 15:40:15.000000 bullhorn-0.0.4/tests/test_client.py
+-rw-rw-rw-   0        0        0     1069 2023-07-21 10:47:02.000000 bullhorn-0.0.4/tests/test_route.py
```

### Comparing `bullhorn-0.0.2/LICENSE` & `bullhorn-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bullhorn-0.0.2/bullhorn/exceptions.py` & `bullhorn-0.0.4/bullhorn/exceptions.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 from typing import Any, Dict, List, Optional, Tuple, Union
 
-from aiohttp import ClientResponse
-
 
 class BullhornException(Exception):
     """Base exception class for the Bullhorn REST API wrapper library.
 
     This class serves as the base exception that can be caught to handle any exceptions raised from this library.
     """
 
@@ -16,15 +14,15 @@
     """Exception raised for HTTP-related errors when interacting with the Bullhorn REST API.
 
     This exception class contains information about the HTTP response, status code, and error message.
     """
 
     def __init__(
         self,
-        response: ClientResponse,
+        response,
         message: Optional[Union[str, Dict[str, Any]]] = None,
     ):
         """
         Initialize an HTTPException object.
 
         Args:
             response (ClientResponse):
@@ -51,16 +49,16 @@
                 If the message is a dictionary, it is retrieved from the "message" key.
                 Otherwise, it defaults to an empty string.
 
         Raises:
             None
 
         """
-        self.response: ClientResponse = response
-        self.status: int = response.status
+        self.response = response
+        self.status: int = response.status_code
         self.code: int
         self.text: str
 
         if isinstance(message, dict):
             self.code = message.get("code", 0)
             base = message.get("message", "")
             errors = message.get("errors")
@@ -72,15 +70,15 @@
                 self.text = base + "\n" + helpful
             else:
                 self.text = base
         else:
             self.text = message or ""
             self.code = 0
 
-        fmt = f"{self.response.status} {self.response.reason} (error code: {self.code})"
+        fmt = f"{self.response.status_code} {self.response.reason} (error code: {self.code})"
         if len(self.text):
             fmt += f": {self.text}"
 
         super().__init__(fmt)
 
 
 class Forbidden(HTTPException):
```

### Comparing `bullhorn-0.0.2/bullhorn/route.py` & `bullhorn-0.0.4/bullhorn/route.py`

 * *Files identical despite different names*

### Comparing `bullhorn-0.0.2/examples/get_placements_and_candidates.py` & `bullhorn-0.0.4/examples/get_placements_and_candidates.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 import os
 
 from bullhorn.client import BullhornClient
 
 
 def get_placements_and_candidates():
     # Set credentials
-    token = os.environ.get("BULLHORN_SESSION_TOKEN")
+    session_token = os.environ.get("BULLHORN_SESSION_TOKEN")
     rest_url = os.environ.get("BULLHORN_REST_URL")
 
     # Initialise client
     bc = BullhornClient(
-        token=token,
+        token=session_token,
         rest_url=rest_url,
     )
-    bc.login()
 
     # Get placements result
     placements = bc.get_placements(
         query="dateLastModified:{2023/01/01 TO *}",
         fields="id,candidate,comments,dateAdded,dateBegin,dateEnd,dateLastModified,referralFee,salary,status",
     )
     print("Success: %r" % (placements))
```

### Comparing `bullhorn-0.0.2/setup.py` & `bullhorn-0.0.4/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,27 @@
+from bullhorn import __version__, __title__, __author__, __license__
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setup(
-    name="bullhorn",
-    version="0.0.2",
-    author="lloydtao (Lewis Lloyd)",
+    version=__version__,
+    name=__title__,
+    author=__author__,
+    license=__license__,
     author_email="lewis@recruit-hub.com",
     description="Python wrapper for the Bullhorn REST API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/recruithub/bullhorn",
     packages=find_packages(),
     install_requires=[
-        "aiohttp==3.8.4",
-        "black==23.3.0",
-        "coverage==7.2.7",
-        "pytest==7.3.1",
-        "pytest-mock==3.10.0",
+        "requests==2.31.0",
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.10",
```

### Comparing `bullhorn-0.0.2/tests/test_route.py` & `bullhorn-0.0.4/tests/test_route.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
         path,
         path_params,
         query_params,
     )
     assert route.url == "https://rest123.bullhornstaffing.com/rest-services/1234/ping"
 
 
-def test_route_with_params_url():
+def test_route_url_params():
     method = "GET"
     path = (
         "https://rest123.bullhornstaffing.com/rest-services/1234/"
         + "entity/{entityType}/{entityId}"
     )
     path_params = {
         "entityType": "Candidate",
```

