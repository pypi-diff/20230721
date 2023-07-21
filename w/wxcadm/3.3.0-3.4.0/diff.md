# Comparing `tmp/wxcadm-3.3.0.tar.gz` & `tmp/wxcadm-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wxcadm-3.3.0.tar", last modified: Wed Mar 29 17:53:19 2023, max compression
+gzip compressed data, was "wxcadm-3.4.0.tar", last modified: Fri Jul 21 14:11:41 2023, max compression
```

## Comparing `wxcadm-3.3.0.tar` & `wxcadm-3.4.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-03-29 17:53:19.890175 wxcadm-3.3.0/
--rw-rw-rw-   0        0        0    35823 2022-08-15 14:34:57.000000 wxcadm-3.3.0/LICENSE
--rw-rw-rw-   0        0        0       25 2022-08-15 14:34:57.000000 wxcadm-3.3.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2694 2023-03-29 17:53:19.887697 wxcadm-3.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     2372 2022-08-15 14:34:57.000000 wxcadm-3.3.0/README.md
--rw-rw-rw-   0        0        0       42 2023-03-29 17:53:19.891703 wxcadm-3.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1082 2023-03-29 17:53:04.000000 wxcadm-3.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-29 17:53:19.861931 wxcadm-3.3.0/wxcadm/
--rw-rw-rw-   0        0        0      412 2023-03-14 13:55:21.000000 wxcadm-3.3.0/wxcadm/__init__.py
--rw-rw-rw-   0        0        0     8774 2022-10-17 16:15:33.000000 wxcadm-3.3.0/wxcadm/applications.py
--rw-rw-rw-   0        0        0     2028 2022-08-23 16:22:45.000000 wxcadm-3.3.0/wxcadm/bifrost.py
--rw-rw-rw-   0        0        0    13245 2022-08-23 16:22:45.000000 wxcadm-3.3.0/wxcadm/call_routing.py
--rw-rw-rw-   0        0        0     3320 2023-01-13 19:47:24.000000 wxcadm-3.3.0/wxcadm/calls.py
--rw-rw-rw-   0        0        0    12665 2023-02-16 15:26:30.000000 wxcadm-3.3.0/wxcadm/common.py
--rw-rw-rw-   0        0        0    13686 2022-08-23 16:22:45.000000 wxcadm-3.3.0/wxcadm/cpapi.py
--rw-rw-rw-   0        0        0     4442 2022-08-23 16:22:45.000000 wxcadm-3.3.0/wxcadm/csdm.py
--rw-rw-rw-   0        0        0     2408 2023-02-16 15:26:30.000000 wxcadm-3.3.0/wxcadm/device.py
--rw-rw-rw-   0        0        0     1369 2022-08-23 16:22:45.000000 wxcadm-3.3.0/wxcadm/exceptions.py
--rw-rw-rw-   0        0        0    11475 2023-01-13 19:47:24.000000 wxcadm-3.3.0/wxcadm/location.py
--rw-rw-rw-   0        0        0    25643 2023-01-13 19:47:24.000000 wxcadm-3.3.0/wxcadm/location_features.py
--rw-rw-rw-   0        0        0    21700 2023-03-14 13:55:21.000000 wxcadm-3.3.0/wxcadm/meraki.py
--rw-rw-rw-   0        0        0      307 2023-02-16 15:26:30.000000 wxcadm-3.3.0/wxcadm/number.py
--rw-rw-rw-   0        0        0    38819 2023-02-23 15:27:49.000000 wxcadm-3.3.0/wxcadm/org.py
--rw-rw-rw-   0        0        0    57271 2023-02-16 15:26:30.000000 wxcadm-3.3.0/wxcadm/person.py
--rw-rw-rw-   0        0        0    30377 2023-03-14 13:55:21.000000 wxcadm-3.3.0/wxcadm/redsky.py
--rw-rw-rw-   0        0        0     5933 2022-10-17 16:15:33.000000 wxcadm-3.3.0/wxcadm/reports.py
--rw-rw-rw-   0        0        0     1283 2022-08-23 16:22:45.000000 wxcadm-3.3.0/wxcadm/terminus.py
--rw-rw-rw-   0        0        0    14453 2023-02-23 15:27:49.000000 wxcadm-3.3.0/wxcadm/webex.py
--rw-rw-rw-   0        0        0     8968 2022-08-23 16:22:45.000000 wxcadm-3.3.0/wxcadm/webhooks.py
--rw-rw-rw-   0        0        0     5728 2023-01-13 19:47:24.000000 wxcadm-3.3.0/wxcadm/wholesale.py
--rw-rw-rw-   0        0        0     8296 2023-02-16 15:26:30.000000 wxcadm-3.3.0/wxcadm/workspace.py
--rw-rw-rw-   0        0        0    72713 2023-01-13 19:47:24.000000 wxcadm-3.3.0/wxcadm/xsi.py
--rw-rw-rw-   0        0        0     1040 2022-08-23 16:22:45.000000 wxcadm-3.3.0/wxcadm/xsi_response.py
-drwxrwxrwx   0        0        0        0 2023-03-29 17:53:19.885480 wxcadm-3.3.0/wxcadm.egg-info/
--rw-rw-rw-   0        0        0     2694 2023-03-29 17:53:19.000000 wxcadm-3.3.0/wxcadm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      650 2023-03-29 17:53:19.000000 wxcadm-3.3.0/wxcadm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-29 17:53:19.000000 wxcadm-3.3.0/wxcadm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       92 2023-03-29 17:53:19.000000 wxcadm-3.3.0/wxcadm.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-03-29 17:53:19.000000 wxcadm-3.3.0/wxcadm.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-21 14:11:41.287548 wxcadm-3.4.0/
+-rw-rw-rw-   0        0        0    35823 2022-08-15 14:34:57.000000 wxcadm-3.4.0/LICENSE
+-rw-rw-rw-   0        0        0       25 2022-08-15 14:34:57.000000 wxcadm-3.4.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2694 2023-07-21 14:11:41.285029 wxcadm-3.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2372 2022-08-15 14:34:57.000000 wxcadm-3.4.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-21 14:11:41.288715 wxcadm-3.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     1082 2023-07-21 14:10:32.000000 wxcadm-3.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 14:11:41.259904 wxcadm-3.4.0/wxcadm/
+-rw-rw-rw-   0        0        0      412 2023-03-29 17:54:38.000000 wxcadm-3.4.0/wxcadm/__init__.py
+-rw-rw-rw-   0        0        0     7705 2023-07-21 13:31:28.000000 wxcadm-3.4.0/wxcadm/announcements.py
+-rw-rw-rw-   0        0        0     8835 2023-05-26 20:19:04.000000 wxcadm-3.4.0/wxcadm/applications.py
+-rw-rw-rw-   0        0        0     2028 2022-08-23 16:22:45.000000 wxcadm-3.4.0/wxcadm/bifrost.py
+-rw-rw-rw-   0        0        0    13245 2022-08-23 16:22:45.000000 wxcadm-3.4.0/wxcadm/call_routing.py
+-rw-rw-rw-   0        0        0     3320 2023-01-13 19:47:24.000000 wxcadm-3.4.0/wxcadm/calls.py
+-rw-rw-rw-   0        0        0    15267 2023-07-20 19:13:22.000000 wxcadm-3.4.0/wxcadm/common.py
+-rw-rw-rw-   0        0        0    13686 2022-08-23 16:22:45.000000 wxcadm-3.4.0/wxcadm/cpapi.py
+-rw-rw-rw-   0        0        0     5935 2023-05-30 19:13:35.000000 wxcadm-3.4.0/wxcadm/device.py
+-rw-rw-rw-   0        0        0     1369 2022-08-23 16:22:45.000000 wxcadm-3.4.0/wxcadm/exceptions.py
+-rw-rw-rw-   0        0        0    12101 2023-07-19 04:51:09.000000 wxcadm-3.4.0/wxcadm/location.py
+-rw-rw-rw-   0        0        0    25643 2023-01-13 19:47:24.000000 wxcadm-3.4.0/wxcadm/location_features.py
+-rw-rw-rw-   0        0        0    21700 2023-03-29 17:54:38.000000 wxcadm-3.4.0/wxcadm/meraki.py
+-rw-rw-rw-   0        0        0      307 2023-02-16 15:26:30.000000 wxcadm-3.4.0/wxcadm/number.py
+-rw-rw-rw-   0        0        0    40989 2023-07-20 20:39:12.000000 wxcadm-3.4.0/wxcadm/org.py
+-rw-rw-rw-   0        0        0    62036 2023-05-26 15:52:10.000000 wxcadm-3.4.0/wxcadm/person.py
+-rw-rw-rw-   0        0        0    31993 2023-07-21 14:08:13.000000 wxcadm-3.4.0/wxcadm/redsky.py
+-rw-rw-rw-   0        0        0     5933 2022-10-17 16:15:33.000000 wxcadm-3.4.0/wxcadm/reports.py
+-rw-rw-rw-   0        0        0     1283 2022-08-23 16:22:45.000000 wxcadm-3.4.0/wxcadm/terminus.py
+-rw-rw-rw-   0        0        0    14453 2023-02-23 15:27:49.000000 wxcadm-3.4.0/wxcadm/webex.py
+-rw-rw-rw-   0        0        0     8968 2022-08-23 16:22:45.000000 wxcadm-3.4.0/wxcadm/webhooks.py
+-rw-rw-rw-   0        0        0     5728 2023-01-13 19:47:24.000000 wxcadm-3.4.0/wxcadm/wholesale.py
+-rw-rw-rw-   0        0        0    12901 2023-05-26 18:07:46.000000 wxcadm-3.4.0/wxcadm/workspace.py
+-rw-rw-rw-   0        0        0    72713 2023-01-13 19:47:24.000000 wxcadm-3.4.0/wxcadm/xsi.py
+-rw-rw-rw-   0        0        0     1040 2022-08-23 16:22:45.000000 wxcadm-3.4.0/wxcadm/xsi_response.py
+drwxrwxrwx   0        0        0        0 2023-07-21 14:11:41.282450 wxcadm-3.4.0/wxcadm.egg-info/
+-rw-rw-rw-   0        0        0     2694 2023-07-21 14:11:40.000000 wxcadm-3.4.0/wxcadm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      659 2023-07-21 14:11:41.000000 wxcadm-3.4.0/wxcadm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 14:11:40.000000 wxcadm-3.4.0/wxcadm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       92 2023-07-21 14:11:40.000000 wxcadm-3.4.0/wxcadm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-21 14:11:40.000000 wxcadm-3.4.0/wxcadm.egg-info/top_level.txt
```

### Comparing `wxcadm-3.3.0/LICENSE` & `wxcadm-3.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wxcadm-3.3.0/PKG-INFO` & `wxcadm-3.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wxcadm
-Version: 3.3.0
+Version: 3.4.0
 Summary: A Python 3 Library for Webex Calling Administrators
 Home-page: https://github.com/kctrey/wxcadm
 Author: Trey Hilyard
 Author-email: kctrey@gmail.com
 License: GPL-3.0
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `wxcadm-3.3.0/README.md` & `wxcadm-3.4.0/README.md`

 * *Files identical despite different names*

### Comparing `wxcadm-3.3.0/setup.py` & `wxcadm-3.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 ]
 
 with open('README.md', 'r', encoding='utf-8') as f:
     readme = f.read()
 
 setup(
     name='wxcadm',
-    version='3.3.0',
+    version='3.4.0',
     packages=packages,
     url='https://github.com/kctrey/wxcadm',
     license='GPL-3.0',
     author='Trey Hilyard',
     author_email='kctrey@gmail.com',
     description='A Python 3 Library for Webex Calling Administrators',
     long_description=readme,
```

### Comparing `wxcadm-3.3.0/wxcadm/applications.py` & `wxcadm-3.4.0/wxcadm/applications.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,17 @@
             WebexApplication: The application instance
 
         """
         found_apps = []
         for app in self.data:
             if app.name == name:
                 found_apps.append(app)
-        if len(found_apps) == 1:
+        if len(found_apps) == 0:
+            return None
+        elif len(found_apps) == 1:
             return found_apps[0]
         else:
             return found_apps
 
     def get_app_by_id(self, id: str) -> WebexApplication:
         """ Get a :py:class:`WebexApplication` instance by application ID
```

### Comparing `wxcadm-3.3.0/wxcadm/bifrost.py` & `wxcadm-3.4.0/wxcadm/bifrost.py`

 * *Files identical despite different names*

### Comparing `wxcadm-3.3.0/wxcadm/call_routing.py` & `wxcadm-3.4.0/wxcadm/call_routing.py`

 * *Files identical despite different names*

### Comparing `wxcadm-3.3.0/wxcadm/calls.py` & `wxcadm-3.4.0/wxcadm/calls.py`

 * *Files identical despite different names*

### Comparing `wxcadm-3.3.0/wxcadm/common.py` & `wxcadm-3.4.0/wxcadm/common.py`

 * *Files 10% similar despite different names*

```diff
@@ -149,14 +149,40 @@
                 if r.status_code == 429:
                     retry_after = int(r.headers.get('Retry-After', 30))
                     log.info(f"Received 429 Too Many Requests. Waiting {retry_after} seconds to retry.")
                     time.sleep(retry_after)
                     continue
                 else:
                     raise APIError(f"The Webex API returned an error: {r.text}")
+        elif method.lower() == "put_upload":
+            log.debug("Putting a file upload")
+            log.debug(payload)
+            session.headers['Content-Type'] = payload.content_type
+            r = session.put(url_base + url, params=params, data=payload)
+            log.debug(f"Response Headers: {r.headers}")
+            if r.ok:
+                try:
+                    response = r.json()
+                except requests.exceptions.JSONDecodeError:
+                    end = time.time()
+                    log.debug(f"__webex_api_call() completed in {end - start} seconds")
+                    return True
+                else:
+                    end = time.time()
+                    log.debug(f"__webex_api_call() completed in {end - start} seconds")
+                    return response
+            else:
+                log.warning("Webex API returned an error")
+                if r.status_code == 429:
+                    retry_after = int(r.headers.get('Retry-After', 30))
+                    log.info(f"Received 429 Too Many Requests. Waiting {retry_after} seconds to retry.")
+                    time.sleep(retry_after)
+                    continue
+                else:
+                    raise APIError(f"The Webex API returned an error: {r.text}")
         elif method.lower() == "post":
             log.debug(f"Post body: {payload}")
             r = session.post(url_base + url, params=params, json=payload)
             if r.ok:
                 try:
                     response = r.json()
                 except requests.exceptions.JSONDecodeError:
@@ -172,14 +198,40 @@
                 if r.status_code == 429:
                     retry_after = int(r.headers.get('Retry-After', 30))
                     log.info(f"Received 429 Too Many Requests. Waiting {retry_after} seconds to retry.")
                     time.sleep(retry_after)
                     continue
                 else:
                     raise APIError(f"The Webex API returned an error: {r.text}")
+        elif method.lower() == "post_upload":
+            log.debug("Posting a file upload")
+            log.debug(payload)
+            session.headers['Content-Type'] = payload.content_type
+            r = session.post(url_base + url, params=params, data=payload)
+            log.debug(f"Response Headers: {r.headers}")
+            if r.ok:
+                try:
+                    response = r.json()
+                except requests.exceptions.JSONDecodeError:
+                    end = time.time()
+                    log.debug(f"__webex_api_call() completed in {end - start} seconds")
+                    return True
+                else:
+                    end = time.time()
+                    log.debug(f"__webex_api_call() completed in {end - start} seconds")
+                    return response
+            else:
+                log.warning("Webex API returned an error")
+                if r.status_code == 429:
+                    retry_after = int(r.headers.get('Retry-After', 30))
+                    log.info(f"Received 429 Too Many Requests. Waiting {retry_after} seconds to retry.")
+                    time.sleep(retry_after)
+                    continue
+                else:
+                    raise APIError(f"The Webex API returned an error: {r.text}")
         elif method.lower() == "delete":
             r = session.delete(url_base + url, params=params)
             if r.ok:
                 try:
                     response = r.json()
                 except requests.exceptions.JSONDecodeError:
                     end = time.time()
```

### Comparing `wxcadm-3.3.0/wxcadm/cpapi.py` & `wxcadm-3.4.0/wxcadm/cpapi.py`

 * *Files identical despite different names*

### Comparing `wxcadm-3.3.0/wxcadm/exceptions.py` & `wxcadm-3.4.0/wxcadm/exceptions.py`

 * *Files identical despite different names*

### Comparing `wxcadm-3.3.0/wxcadm/location.py` & `wxcadm-3.4.0/wxcadm/location.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,14 +62,34 @@
         my_hunt_groups = []
         for hg in self._parent.hunt_groups:
             if hg.location == self.id:
                 my_hunt_groups.append(hg)
         return my_hunt_groups
 
     @property
+    def announcements(self):
+        """ List of :py:class:`Announcement` instances for the Location
+
+        .. note::
+            This does not include announcements built at the Organization level
+
+        """
+        annc_list = self._parent.announcements.get_by_location_id(self.id)
+        return annc_list
+
+    @property
+    def auto_attenndants(self):
+        """ List of AutoAttendant instances for this Location"""
+        aa_list = []
+        for aa in self._parent.auto_attendants:
+            if aa.location == self.id:
+                aa_list.append(aa)
+        return aa_list
+
+    @property
     def call_queues(self):
         """List of CallQueue instances for this Location"""
         my_call_queues = []
         for cq in self._parent.call_queues:
             if cq.location_id == self.id:
                 my_call_queues.append(cq)
         return my_call_queues
```

### Comparing `wxcadm-3.3.0/wxcadm/location_features.py` & `wxcadm-3.4.0/wxcadm/location_features.py`

 * *Files identical despite different names*

### Comparing `wxcadm-3.3.0/wxcadm/meraki.py` & `wxcadm-3.4.0/wxcadm/meraki.py`

 * *Files identical despite different names*

### Comparing `wxcadm-3.3.0/wxcadm/org.py` & `wxcadm-3.4.0/wxcadm/org.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,25 +4,26 @@
 import requests
 import re
 from typing import Union, Optional
 from wxcadm import log
 from .common import *
 from .common import _url_base
 from .exceptions import *
-from .csdm import CSDM
 from .cpapi import CPAPI
 from .location import Location
 from .location_features import PagingGroup, PickupGroup, HuntGroup, CallQueue, AutoAttendant
 from .webhooks import Webhooks
 from .person import UserGroups, Person
 from .applications import WebexApplications
+from .announcements import AnnouncementList
 from .workspace import Workspace, WorkspaceLocation
 from .call_routing import CallRouting
 from .reports import Reports
 from .calls import Calls
+from .device import Device
 
 
 class Org:
     def __init__(self,
                  name: str,
                  id: str,
                  parent: Webex = None,
@@ -56,16 +57,16 @@
         self._parent = parent
         self.call_queues: Optional[list] = None
         """The Call Queues for this Org"""
         self.hunt_groups: Optional[list] = None
         """The Hunt Groups for this Org"""
         self.pickup_groups: Optional[list] = None
         'A list of the PickupGroup instances for this Org'
-        self.locations: list = []
-        'A list of the Location instances for this Org'
+        self._locations: list | None = None
+        """ The cache of locations as used by the .locations property """
         self.name: str = name
         'The name of the Organization'
         self.id: str = id
         '''The Webex ID of the Organization'''
         self.xsi: dict = {}
         """The XSI details for the Organization"""
         self._params: dict = {"orgId": self.id}
@@ -79,29 +80,27 @@
         """A list of the Workspace Location instanced for this Org."""
         self._devices: Optional[list] = None
         """A list of the Devce instances for this Org"""
         self._auto_attendants: list = []
         """A list of the AutoAttendant instances for this Org"""
         self._usergroups: Optional[list] = None
         self._roles: Optional[dict] = None
+        self._announcements: Optional[AnnouncementList] = None
 
         self.call_routing = CallRouting(self)
         """ The :py:class:`CallRouting` instance for this Org """
         self.reports = Reports(self)
         """ The :py:class:`Reports` instance for this Org """
 
         # Set the Authorization header based on how the instance was built
         self._headers = parent.headers
 
         # Create a CPAPI instance for CPAPI work
         self._cpapi = CPAPI(self, self._parent._access_token)
 
-        # Create a CSDM instance for CSDM work
-        self._csdm = CSDM(self, self._parent._access_token)
-
         if locations:
             self.get_locations()
         if xsi:
             self.get_xsi_endpoints()
         if call_queues:
             self.get_call_queues()
         if hunt_groups:
@@ -142,14 +141,20 @@
     def licenses(self):
         """ A list of all licenses for the Organization as a dictionary of names and IDs """
         if self._licenses is None:
             self._licenses = self.__get_licenses()
         return self._licenses
 
     @property
+    def locations(self):
+        if self._locations is None:
+            self.get_locations()
+        return self._locations
+
+    @property
     def roles(self):
         """ A dict of user roles with the ID as the key and the Role name as the value """
         if self._roles is None:
             roles = {}
             response = webex_api_call('get', 'v1/roles')
             for role in response:
                 roles[role['id']] = role['name']
@@ -206,14 +211,18 @@
             for entry in response['locationPaging']:
                 location = self.get_location(id=entry['locationId'])
                 this_pg = PagingGroup(location, entry['id'], entry['name'])
                 paging_groups.append(this_pg)
             self._paging_groups = paging_groups
         return self._paging_groups
 
+    def get_supported_devices(self):
+        response = webex_api_call('get', f"/v1/telephony/config/supportedDevices", params={'orgId': self.id})
+        return response['devices']
+
     @property
     def webhooks(self):
         """ The :py:class:`Webhooks` list with the :py:class:`Webhook` instances for the Org"""
         return Webhooks()
 
     @property
     def usergroups(self):
@@ -222,14 +231,21 @@
 
     @property
     def applications(self):
         """ The :py:class:`WebexApplications` list with the :py:class:`WebexApplication` instances for this Org """
         return WebexApplications(parent=self)
 
     @property
+    def announcements(self):
+        """ The :py:class:`AnnouncementList` list with the :py:class:`Announcement` instances for this Org """
+        if self._announcements is None:
+            self._announcements = AnnouncementList(parent=self)
+        return self._announcements
+
+    @property
     def calls(self):
         """ The :py:class:`Calls` instance for this Org"""
         return Calls(parent=self)
 
 
     def get_paging_group(self, id: str = None, name: str = None, spark_id: str = None):
         """ Get the PagingGroup instance associated with a given ID, Name, or Spark ID
@@ -400,16 +416,37 @@
     @property
     def devices(self):
         """All the Device instances for the Org
 
         Returns:
             list[Device]: List of all Device instances
         """
-        self._devices = self._csdm.get_devices()
-        return self._devices
+        devices = []
+        response = webex_api_call("get", "/v1/devices", params={"orgId": self.id})
+        for device in response:
+            this_device = Device(self, config=device)
+            devices.append(this_device)
+        return devices
+
+    def get_device_by_id(self, device_id: str):
+        """ Get the :py:class:`Device` instance for a specific Device ID
+
+        Args:
+            device_id (str): The Device ID to return
+
+        Returns:
+            Device: The Device instance. False is returned if no match is found.
+
+        """
+        log.debug(f"Finding device with ID {device_id}")
+        for device in self.devices:
+            if device.id == device_id or decode_spark_id(device.id).split("/")[-1] == \
+                    decode_spark_id(device_id).split("/")[-1]:
+                return device
+        return False
 
     def get_location_by_name(self, name: str):
         """Get the Location instance associated with a given Location name
 
         .. deprecated:: 2.2.0
             Use :meth:`get_location` using the ```name``` argument instead.
 
@@ -658,40 +695,40 @@
         Also stores them in the Org.locations attribute.
 
         Returns:
             list[Location]: List of Location instance objects. See the Locations class for attributes.
 
         """
         log.info("get_locations() started")
-        self.locations.clear()
+        self._locations = []
         api_resp = webex_api_call("get", "v1/locations", headers=self._headers, params=self._params)
         for location in api_resp:
             this_location = Location(self,
                                      location['id'],
                                      location['name'],
                                      address=location['address'],
                                      time_zone=location['timeZone'],
                                      preferred_language=location['preferredLanguage'])
-            self.locations.append(this_location)
-        return self.locations
+            self._locations.append(this_location)
+        return self._locations
 
     def create_location(self,
                         name: str,
                         time_zone: str,
                         preferred_language: str,
                         announcement_language: str,
                         address: dict):
         payload = {
             'name': name,
             'timeZone': time_zone,
             'preferredLanguage': preferred_language,
             'announcementLanguage': announcement_language,
             'address': address
         }
-        response = webex_api_call('post', '/v1/locations', params={'orgId': self.id}, payload=payload)
+        response = webex_api_call('post', 'v1/locations', payload=payload)
         return response
 
     def get_workspaces(self):
         """Get the Workspaces and Workspace Locations for the Organizations.
 
         Also stores them in the Org.workspaces and Org.workspace_locations attributes.
 
@@ -711,14 +748,31 @@
         api_resp = webex_api_call("get", "v1/workspaceLocations", headers=self._headers, params=self._params)
         for location in api_resp:
             this_location = WorkspaceLocation(self, location['id'], location)
             self.workspace_locations.append(this_location)
 
         return self.workspaces
 
+    def get_workspace_by_id(self, id: str) -> Optional[Workspace]:
+        """ Get a :py:class:`Workspace` by its ID
+
+        Args:
+            id (str): The Workspace ID to serach for
+
+        Returns:
+            Workspace: The matching Workspace instance. None is returned if no match is found.
+
+        """
+        if self.workspaces is None:
+            self.get_workspaces()
+        for workspace in self.workspaces:
+            if workspace.id == id:
+                return workspace
+        return None
+
     def get_pickup_groups(self):
         """Get all of the Call Pickup Groups for an Organization.
 
         Also stores them in the Org.pickup_groups attribute.
 
         Returns:
             list[PickupGroup]: List of Call Pickup Groups as a list of dictionaries.
@@ -793,14 +847,15 @@
         Args:
             id (str): The CallQueue ID
 
         Returns:
             HuntGroup: The :class:`CallQueue` instance
 
         """
+        log.info(f"Getting Call Queue with ID {id}")
         if self.call_queues is None:
             self.get_call_queues()
         for cq in self.call_queues:
             if cq.id == id:
                 return cq
         return None
 
@@ -969,7 +1024,11 @@
             'from': start,
             'to': end,
             'actorId': actor_id,
         }
         response = webex_api_call('get', '/v1/adminAudit/events', params=params)
         return response
 
+    ### Method aliases
+    # Used for backwards compatibility to old method names as new methods are added/changed
+    refresh_locations = get_locations
+
```

### Comparing `wxcadm-3.3.0/wxcadm/person.py` & `wxcadm-3.4.0/wxcadm/person.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from requests_toolbelt import MultipartEncoder
 import base64
 import os
 from typing import Optional, Type
 from dataclasses import dataclass, field
 from collections import UserList
 
+import wxcadm.exceptions
 from .common import *
 from .xsi import XSI
 from .device import Device
 
 from wxcadm import log
 
 
@@ -307,24 +308,113 @@
             UserGroup: The :py:class:`UserGroup`. None is returned if the Person is not assigned to a Group
 
         """
         return self._parent.usergroups.find_person_assignment(self)
 
     @property
     def devices(self):
+        """ List of :py:class:`Device` instances for the Person
+
+        Returns:
+            List
+
+        """
         log.info(f"Collecting devices for {self.display_name}")
         devices = []
         response = webex_api_call('get', f'/v1/telephony/config/people/{self.id}/devices')
         log.debug(f"{response}")
         for item in response['devices']:
             this_device = Device(self, item)
             devices.append(this_device)
         return devices
 
+    def add_device(self, model: str, mac: Optional[str] = None, password: Optional[str] = None):
+        """ Add a new device to the Person
+
+        In order to use this method, you must know the model of the device that you are adding, as expected by the
+        Webex API. If you are adding a "Generic IPPhone Customer Managed" device, you can use that value or simply
+        send ``model='GENERIC'`` as an alias. You can find the full list of models with the
+        :py:meth:`Org.get_supported_devices()` method.
+
+        If the MAC address is passed, a device will be created with the provided MAC address. If no MAC address is
+        passed, an Activation Code will be generated and returned as part of the response. Your integration/token must
+        have the ``identity:placeonetimepassword_create`` scope to create Activation Codes for devices.
+
+        Args:
+            model (str): The model name of the device being added
+            mac (str, optional): The MAC address of the device being added
+            password (str, optional): Only valid when creating a Generic IPPhone Customer Managed device. If a
+                password is not provided, the Webex API will generate a unique, compliant SIP password and return it
+                in the response.
+
+        Returns:
+            dict: The dict values vary based on the type of device being activated. If the device fails for any reason,
+                False will be returned. At the moment, Webex doesn't provide very useful failure reasons, but those may
+                be added to the return value when they are available.
+
+        """
+        log.info(f"Adding a device to {self.display_name}")
+        payload = {
+            "personId": self.id,
+            "model": model
+        }
+        data_needed = False  # Flag that we need to get platform data once we have a Device ID
+        if mac is None:
+            # If no MAC address is provided, just generate an activation code for the device
+            try:
+                response = webex_api_call('post',
+                                          '/v1/devices/activationCode',
+                                          payload=payload,
+                                          params={'orgId': self._parent.id})
+                log.debug(f"\t{response}")
+            except wxcadm.exceptions.APIError:
+                return False
+
+            # Get the ID of the device we just inserted
+            device_id = response.get('id', None).replace('=', '')
 
+            results = {
+                'device_id': device_id,
+                'activation_code': response['code']
+            }
+        else:
+            payload['mac'] = mac
+            if model.upper() == "GENERIC" or model.upper() == "Generic IPPhone Customer Managed":
+                payload['model'] = "Generic IPPhone Customer Managed"  # Hard-code what the API expects (for now)
+                data_needed = True
+                if password is None:    # Generate a unique password
+                    response = webex_api_call('POST',
+                                                  f'/v1/telephony/config/locations/{self.location}/actions/'
+                                                  f'generatePassword/invoke')
+                    password = response['exampleSipPassword']
+                payload['password'] = password
+            response = webex_api_call('post', '/v1/devices', payload=payload)
+            log.debug(f"\t{response}")
+
+            # Get the ID of the device we just inserted
+            device_id = response.get('id', None).replace('=', '')
+
+            results = {
+                'device_id': device_id,
+                'mac': response['mac']
+            }
+
+            if data_needed is True:
+                response = webex_api_call('get', f'/v1/telephony/config/devices/{device_id}')
+                results['sip_auth_user'] = response['owner']['sipUserName']
+                results['line_port'] = response['owner']['linePort']
+                results['password'] = password
+                results['sip_userpart'] = response['owner']['linePort'].split('@')[0]
+                results['sip_hostpart'] = response['owner']['linePort'].split('@')[1]
+                results['sip_outbound_proxy'] = response['proxy']['outboundProxy']
+                results['sip_outbound_proxy_srv'] = f"_sips._tcp.{response['proxy']['outboundProxy']}"
+
+        # Provide the Device instance in the response as well
+        results['device_object'] = self._parent.get_device_by_id(device_id)
+        return results
 
     @property
     def hunt_groups(self):
         """The Hunt Groups that this user is an Agent for.
 
         Returns:
             list[HuntGroup]: A list of the `HuntGroup` instances the user belongs to
```

### Comparing `wxcadm-3.3.0/wxcadm/redsky.py` & `wxcadm-3.4.0/wxcadm/redsky.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 
         """
         # Log into Horizon and get access token info
         payload = {"username": username, "password": password}
         r = requests.post("https://api.wxc.e911cloud.com/auth-service/login", json=payload)
         if r.ok:
             response = r.json()
+            log.debug(response)
         else:
             raise APIError("Cannot log into RedSky Horizon")
         self._access_token = response['accessToken']
         self.org_id = response['userProfileTO']['company']['id']
         self._refresh_token = response['refreshTokenInfo']['id']
         self._full_config = response
         self._buildings = []
@@ -380,14 +381,51 @@
             for entry in current_lldp:
                 if entry['chassisId'].lower == chassis.lower():
                     return entry
         else:
             new_chassis = self._add_chassis_discovery(chassis, location, description)
             return new_chassis
 
+    def delete_lldp_chassis(self, chassis_id: str, delete_ports: bool = False):
+        """ Delete an LLDP mapping from Horizon Mobility
+
+        Args:
+            chassis_id (str): The chassis ID of the LLDp Discovery to delete
+            delete_ports (bool, optional): Whether to delete all ports first. Defaults to False
+
+        Returns:
+            bool: True on success, False otherwise
+
+        """
+        log.info(f"Deleting Chassis Discovery: {chassis_id}")
+        chassis_entry = self.get_lldp_discovery_by_chassis(chassis_id)
+
+        if delete_ports is True:
+            log.info("Deleting all ports")
+            for port in chassis_entry['ports']:
+                log.info(f"\tDeleting Port: {port['portId']}")
+                r = requests.delete(f"https://api.wxc.e911cloud.com/networking-service/networkSwitchPort/{port['id']}",
+                                    headers=self._headers,
+                                    params={
+                                        "companyId": self.org_id
+                                    })
+                log.debug(f"Response Code: {r.status_code}")
+
+        r = requests.delete(f"https://api.wxc.e911cloud.com/networking-service/networkSwitch/{chassis_entry['id']}",
+                            headers=self._headers,
+                            params={
+                                "companyId": self.org_id
+                            })
+        log.debug(f"Response Code: {r.status_code}")
+
+        if r.ok:
+            return True
+        else:
+            return False
+
     def update_lldp_location(self, entry_id: str, chassis: str, new_location: RedSkyLocation, description: str):
         payload = {
             'chassisId': chassis,
             'companyId': self.org_id,
             'id': entry_id,
             'locationId': new_location.id,
             'description': description
```

### Comparing `wxcadm-3.3.0/wxcadm/reports.py` & `wxcadm-3.4.0/wxcadm/reports.py`

 * *Files identical despite different names*

### Comparing `wxcadm-3.3.0/wxcadm/terminus.py` & `wxcadm-3.4.0/wxcadm/terminus.py`

 * *Files identical despite different names*

### Comparing `wxcadm-3.3.0/wxcadm/webex.py` & `wxcadm-3.4.0/wxcadm/webex.py`

 * *Files identical despite different names*

### Comparing `wxcadm-3.3.0/wxcadm/webhooks.py` & `wxcadm-3.4.0/wxcadm/webhooks.py`

 * *Files identical despite different names*

### Comparing `wxcadm-3.3.0/wxcadm/wholesale.py` & `wxcadm-3.4.0/wxcadm/wholesale.py`

 * *Files identical despite different names*

### Comparing `wxcadm-3.3.0/wxcadm/xsi.py` & `wxcadm-3.4.0/wxcadm/xsi.py`

 * *Files identical despite different names*

### Comparing `wxcadm-3.3.0/wxcadm/xsi_response.py` & `wxcadm-3.4.0/wxcadm/xsi_response.py`

 * *Files identical despite different names*

### Comparing `wxcadm-3.3.0/wxcadm.egg-info/PKG-INFO` & `wxcadm-3.4.0/wxcadm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wxcadm
-Version: 3.3.0
+Version: 3.4.0
 Summary: A Python 3 Library for Webex Calling Administrators
 Home-page: https://github.com/kctrey/wxcadm
 Author: Trey Hilyard
 Author-email: kctrey@gmail.com
 License: GPL-3.0
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `wxcadm-3.3.0/wxcadm.egg-info/SOURCES.txt` & `wxcadm-3.4.0/wxcadm.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.py
 wxcadm/__init__.py
+wxcadm/announcements.py
 wxcadm/applications.py
 wxcadm/bifrost.py
 wxcadm/call_routing.py
 wxcadm/calls.py
 wxcadm/common.py
 wxcadm/cpapi.py
-wxcadm/csdm.py
 wxcadm/device.py
 wxcadm/exceptions.py
 wxcadm/location.py
 wxcadm/location_features.py
 wxcadm/meraki.py
 wxcadm/number.py
 wxcadm/org.py
```

