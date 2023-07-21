# Comparing `tmp/nso-oc-2.72.0.tar.gz` & `tmp/nso-oc-2.73.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nso-oc-2.72.0.tar", last modified: Wed Jul 12 20:15:12 2023, max compression
+gzip compressed data, was "nso-oc-2.73.0.tar", last modified: Fri Jul 21 19:21:34 2023, max compression
```

## Comparing `nso-oc-2.72.0.tar` & `nso-oc-2.73.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:15:12.906918 nso-oc-2.72.0/
--rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-07-12 20:14:44.000000 nso-oc-2.72.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-12 20:14:44.000000 nso-oc-2.72.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-07-12 20:15:12.906918 nso-oc-2.72.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-07-12 20:14:44.000000 nso-oc-2.72.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:15:12.902918 nso-oc-2.72.0/nso_oc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-07-12 20:15:12.000000 nso-oc-2.72.0/nso_oc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-12 20:15:12.000000 nso-oc-2.72.0/nso_oc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 20:15:12.000000 nso-oc-2.72.0/nso_oc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-12 20:15:12.000000 nso-oc-2.72.0/nso_oc.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-12 20:15:12.000000 nso-oc-2.72.0/nso_oc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-12 20:15:12.000000 nso-oc-2.72.0/nso_oc.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:15:12.902918 nso-oc-2.72.0/package_nso_to_oc/
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-07-12 20:14:44.000000 nso-oc-2.72.0/package_nso_to_oc/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-12 20:14:44.000000 nso-oc-2.72.0/package_nso_to_oc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-07-12 20:14:44.000000 nso-oc-2.72.0/package_nso_to_oc/common.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3569 2023-07-12 20:14:44.000000 nso-oc-2.72.0/package_nso_to_oc/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:15:12.906918 nso-oc-2.72.0/package_nso_to_oc/xe/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-12 20:14:44.000000 nso-oc-2.72.0/package_nso_to_oc/xe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6067 2023-07-12 20:14:44.000000 nso-oc-2.72.0/package_nso_to_oc/xe/common_xe.py
--rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-07-12 20:14:44.000000 nso-oc-2.72.0/package_nso_to_oc/xe/main_xe.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    32603 2023-07-12 20:14:44.000000 nso-oc-2.72.0/package_nso_to_oc/xe/xe_acls.py
--rw-r--r--   0 runner    (1001) docker     (123)    36876 2023-07-12 20:14:44.000000 nso-oc-2.72.0/package_nso_to_oc/xe/xe_bgp.py
--rw-r--r--   0 runner    (1001) docker     (123)    63537 2023-07-12 20:14:44.000000 nso-oc-2.72.0/package_nso_to_oc/xe/xe_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     9004 2023-07-12 20:14:44.000000 nso-oc-2.72.0/package_nso_to_oc/xe/xe_mpls.py
--rw-r--r--   0 runner    (1001) docker     (123)    42337 2023-07-12 20:14:44.000000 nso-oc-2.72.0/package_nso_to_oc/xe/xe_network_instances.py
--rw-r--r--   0 runner    (1001) docker     (123)    40463 2023-07-12 20:14:44.000000 nso-oc-2.72.0/package_nso_to_oc/xe/xe_ospfv2.py
--rw-r--r--   0 runner    (1001) docker     (123)    29881 2023-07-12 20:14:44.000000 nso-oc-2.72.0/package_nso_to_oc/xe/xe_routing_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     8996 2023-07-12 20:14:44.000000 nso-oc-2.72.0/package_nso_to_oc/xe/xe_static_route.py
--rw-r--r--   0 runner    (1001) docker     (123)    32957 2023-07-12 20:14:44.000000 nso-oc-2.72.0/package_nso_to_oc/xe/xe_stp.py
--rw-r--r--   0 runner    (1001) docker     (123)   105916 2023-07-12 20:14:44.000000 nso-oc-2.72.0/package_nso_to_oc/xe/xe_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-07-12 20:14:44.000000 nso-oc-2.72.0/package_nso_to_oc/xe/xe_vlans.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:15:12.906918 nso-oc-2.72.0/package_nso_to_oc/xr/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-12 20:14:44.000000 nso-oc-2.72.0/package_nso_to_oc/xr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-12 20:14:44.000000 nso-oc-2.72.0/package_nso_to_oc/xr/common_xr.py
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-12 20:14:44.000000 nso-oc-2.72.0/package_nso_to_oc/xr/main_xr.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    23665 2023-07-12 20:14:44.000000 nso-oc-2.72.0/package_nso_to_oc/xr/xr_acls.py
--rw-r--r--   0 runner    (1001) docker     (123)    50090 2023-07-12 20:14:44.000000 nso-oc-2.72.0/package_nso_to_oc/xr/xr_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     8348 2023-07-12 20:14:44.000000 nso-oc-2.72.0/package_nso_to_oc/xr/xr_system.py
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-12 20:14:44.000000 nso-oc-2.72.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-12 20:15:12.906918 nso-oc-2.72.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-07-12 20:14:44.000000 nso-oc-2.72.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:21:34.484276 nso-oc-2.73.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-07-21 19:21:04.000000 nso-oc-2.73.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-21 19:21:04.000000 nso-oc-2.73.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-07-21 19:21:34.484276 nso-oc-2.73.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-07-21 19:21:04.000000 nso-oc-2.73.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:21:34.480276 nso-oc-2.73.0/nso_oc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-07-21 19:21:34.000000 nso-oc-2.73.0/nso_oc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-21 19:21:34.000000 nso-oc-2.73.0/nso_oc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 19:21:34.000000 nso-oc-2.73.0/nso_oc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-21 19:21:34.000000 nso-oc-2.73.0/nso_oc.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-21 19:21:34.000000 nso-oc-2.73.0/nso_oc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-21 19:21:34.000000 nso-oc-2.73.0/nso_oc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:21:34.480276 nso-oc-2.73.0/package_nso_to_oc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-07-21 19:21:04.000000 nso-oc-2.73.0/package_nso_to_oc/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-21 19:21:04.000000 nso-oc-2.73.0/package_nso_to_oc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-07-21 19:21:04.000000 nso-oc-2.73.0/package_nso_to_oc/common.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3569 2023-07-21 19:21:04.000000 nso-oc-2.73.0/package_nso_to_oc/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:21:34.484276 nso-oc-2.73.0/package_nso_to_oc/xe/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-21 19:21:04.000000 nso-oc-2.73.0/package_nso_to_oc/xe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6067 2023-07-21 19:21:04.000000 nso-oc-2.73.0/package_nso_to_oc/xe/common_xe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-07-21 19:21:04.000000 nso-oc-2.73.0/package_nso_to_oc/xe/main_xe.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33602 2023-07-21 19:21:04.000000 nso-oc-2.73.0/package_nso_to_oc/xe/xe_acls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36876 2023-07-21 19:21:04.000000 nso-oc-2.73.0/package_nso_to_oc/xe/xe_bgp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63537 2023-07-21 19:21:04.000000 nso-oc-2.73.0/package_nso_to_oc/xe/xe_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9004 2023-07-21 19:21:04.000000 nso-oc-2.73.0/package_nso_to_oc/xe/xe_mpls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42337 2023-07-21 19:21:04.000000 nso-oc-2.73.0/package_nso_to_oc/xe/xe_network_instances.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40463 2023-07-21 19:21:04.000000 nso-oc-2.73.0/package_nso_to_oc/xe/xe_ospfv2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29881 2023-07-21 19:21:04.000000 nso-oc-2.73.0/package_nso_to_oc/xe/xe_routing_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8996 2023-07-21 19:21:04.000000 nso-oc-2.73.0/package_nso_to_oc/xe/xe_static_route.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32957 2023-07-21 19:21:04.000000 nso-oc-2.73.0/package_nso_to_oc/xe/xe_stp.py
+-rw-r--r--   0 runner    (1001) docker     (123)   105916 2023-07-21 19:21:04.000000 nso-oc-2.73.0/package_nso_to_oc/xe/xe_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-07-21 19:21:04.000000 nso-oc-2.73.0/package_nso_to_oc/xe/xe_vlans.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:21:34.484276 nso-oc-2.73.0/package_nso_to_oc/xr/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-21 19:21:04.000000 nso-oc-2.73.0/package_nso_to_oc/xr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-21 19:21:04.000000 nso-oc-2.73.0/package_nso_to_oc/xr/common_xr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-21 19:21:04.000000 nso-oc-2.73.0/package_nso_to_oc/xr/main_xr.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23665 2023-07-21 19:21:04.000000 nso-oc-2.73.0/package_nso_to_oc/xr/xr_acls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50090 2023-07-21 19:21:04.000000 nso-oc-2.73.0/package_nso_to_oc/xr/xr_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8348 2023-07-21 19:21:04.000000 nso-oc-2.73.0/package_nso_to_oc/xr/xr_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-21 19:21:04.000000 nso-oc-2.73.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-21 19:21:34.484276 nso-oc-2.73.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-07-21 19:21:04.000000 nso-oc-2.73.0/setup.py
```

### Comparing `nso-oc-2.72.0/LICENSE` & `nso-oc-2.73.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nso-oc-2.72.0/PKG-INFO` & `nso-oc-2.73.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nso-oc
-Version: 2.72.0
+Version: 2.73.0
 Summary: Cisco NSO OpenConfig Tools
 Home-page: https://github.com/model-driven-devops/nso-oc-services
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## NSO NED device configuration to OpenConfig
 
@@ -16,14 +16,15 @@
    ```
    export NSO_URL="http://x.x.x.x:8080"
    export NSO_USERNAME=admin
    export NSO_PASSWORD=admin
    export NSO_DEVICE=router1
    export DEVICE_OS=xe
    export TEST=False   <- if True, the generated OC configuration is sent back to NSO
+   export ACL_USE_EXISTING_SEQ=False   <- if True, existing ACL sequence numbers will be used. Could cause remark errors
    ```
    - For a file (to be used if you've previously pulled the NSO configuration)
    ```
    export NSO_NED_FILE="./device_configurations/$device_name/$device_name.json"
    export DEVICE_OS=xe
    ```
 2. Execute script
```

### Comparing `nso-oc-2.72.0/README.md` & `nso-oc-2.73.0/README.md`

 * *Files identical despite different names*

### Comparing `nso-oc-2.72.0/nso_oc.egg-info/PKG-INFO` & `nso-oc-2.73.0/nso_oc.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nso-oc
-Version: 2.72.0
+Version: 2.73.0
 Summary: Cisco NSO OpenConfig Tools
 Home-page: https://github.com/model-driven-devops/nso-oc-services
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## NSO NED device configuration to OpenConfig
 
@@ -16,14 +16,15 @@
    ```
    export NSO_URL="http://x.x.x.x:8080"
    export NSO_USERNAME=admin
    export NSO_PASSWORD=admin
    export NSO_DEVICE=router1
    export DEVICE_OS=xe
    export TEST=False   <- if True, the generated OC configuration is sent back to NSO
+   export ACL_USE_EXISTING_SEQ=False   <- if True, existing ACL sequence numbers will be used. Could cause remark errors
    ```
    - For a file (to be used if you've previously pulled the NSO configuration)
    ```
    export NSO_NED_FILE="./device_configurations/$device_name/$device_name.json"
    export DEVICE_OS=xe
    ```
 2. Execute script
```

### Comparing `nso-oc-2.72.0/nso_oc.egg-info/SOURCES.txt` & `nso-oc-2.73.0/nso_oc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nso-oc-2.72.0/package_nso_to_oc/README.md` & `nso-oc-2.73.0/package_nso_to_oc/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -8,14 +8,15 @@
    ```
    export NSO_URL="http://x.x.x.x:8080"
    export NSO_USERNAME=admin
    export NSO_PASSWORD=admin
    export NSO_DEVICE=router1
    export DEVICE_OS=xe
    export TEST=False   <- if True, the generated OC configuration is sent back to NSO
+   export ACL_USE_EXISTING_SEQ=False   <- if True, existing ACL sequence numbers will be used. Could cause remark errors
    ```
    - For a file (to be used if you've previously pulled the NSO configuration)
    ```
    export NSO_NED_FILE="./device_configurations/$device_name/$device_name.json"
    export DEVICE_OS=xe
    ```
 2. Execute script
```

### Comparing `nso-oc-2.72.0/package_nso_to_oc/common.py` & `nso-oc-2.73.0/package_nso_to_oc/common.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.72.0/package_nso_to_oc/main.py` & `nso-oc-2.73.0/package_nso_to_oc/main.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.72.0/package_nso_to_oc/xe/common_xe.py` & `nso-oc-2.73.0/package_nso_to_oc/xe/common_xe.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.72.0/package_nso_to_oc/xe/main_xe.py` & `nso-oc-2.73.0/package_nso_to_oc/xe/main_xe.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.72.0/package_nso_to_oc/xe/xe_acls.py` & `nso-oc-2.73.0/package_nso_to_oc/xe/xe_acls.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,17 +15,20 @@
 NSO_DEVICE - NSO device name for configuration translation
 TEST - True or False. True enables sending the OpenConfig to the NSO server after generation
 """
 
 import sys
 from importlib.util import find_spec
 from ipaddress import IPv4Network
+import os
 import socket
 import re
 
+ACL_USE_EXISTING_SEQ = os.environ.get("ACL_USE_EXISTING_SEQ", "False")
+
 acls_notes = []
 openconfig_acls = {
     "openconfig-acl:acl": {
         "openconfig-acl:acl-sets": {
             "openconfig-acl:acl-set": []
         },
         "openconfig-acl:interfaces": {
@@ -78,14 +81,15 @@
     'timestamp-reply': (14, 0),
     'timestamp-request': (13, 0),
     'unreachable': (3, 0)}
 # OC has an additional forwarding action, "DROP", which also translates to "deny" in XE.
 actions_xe_to_oc = {
     "permit": "ACCEPT",
     "deny": "REJECT",
+    "remark": "REMARK"
 }
 port_operators = ["range", "eq", "lt", "gt", "neq"]
 ACL_STD_TYPE = "ACL_IPV4_STANDARD"
 ACL_EXT_TYPE = "ACL_IPV4"
 
 
 def acls_note_add(note):
@@ -208,29 +212,47 @@
     def __set_rule_parts(self, access_rule, acl_set):
         rule_parts = access_rule.get("rule", "").split()
 
         if len(rule_parts) < 1:
             return
 
         success = True
-        if rule_parts[0].isdigit():  # if isdigit, then has sequence number
+        if rule_parts[0].isdigit() and ACL_USE_EXISTING_SEQ == 'True':  # if isdigit, then has sequence number
+            print('under True')
             seq_id = int(rule_parts[0])
             starting_index = 1
+        elif rule_parts[0].isdigit() and ACL_USE_EXISTING_SEQ == 'False':  # if isdigit, then has sequence number
+            seq_id = self.ace_seq_begin
+            self.ace_seq_begin += 10
+            starting_index = 1
         else:
             seq_id = self.ace_seq_begin
             self.ace_seq_begin += 10
             starting_index = 0
         if rule_parts[starting_index] == "remark":
             acls_note_add(f"""
                 Access-list {self._xe_acl_set.get("id")} sequence number {seq_id} is a remark.
-                ACL remarks are not supported in Openconfig
-                If you want to keep the below remark, you should add it to your source of truth:
+                ACL remarks are only supported in MDD OpenConfig using the forwarding action of "REMARK"
+                You may want to consider how you want to handle your ACL remarks.:
                 "{seq_id} {access_rule["rule"]}"
             """)
+            entry = {
+                "openconfig-acl:sequence-id": seq_id,
+                "openconfig-acl:config": {
+                    "openconfig-acl:sequence-id": seq_id,
+                    "openconfig-acl:description": " ".join(rule_parts[starting_index + 1:])
+                },
+                "openconfig-acl:actions": {
+                    "openconfig-acl:config": {
+                        "openconfig-acl:forwarding-action": "REMARK"}
+                }
+            }
+            acl_set["openconfig-acl:acl-entries"]["openconfig-acl:acl-entry"].append(entry)
             return success
+
         entry = {
             "openconfig-acl:sequence-id": seq_id,
             "openconfig-acl:config": {"openconfig-acl:sequence-id": seq_id},
             "openconfig-acl:actions": {
                 "openconfig-acl:config": {"openconfig-acl:forwarding-action": actions_xe_to_oc[rule_parts[starting_index]]}
             }
         }
```

### Comparing `nso-oc-2.72.0/package_nso_to_oc/xe/xe_bgp.py` & `nso-oc-2.73.0/package_nso_to_oc/xe/xe_bgp.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.72.0/package_nso_to_oc/xe/xe_interfaces.py` & `nso-oc-2.73.0/package_nso_to_oc/xe/xe_interfaces.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.72.0/package_nso_to_oc/xe/xe_mpls.py` & `nso-oc-2.73.0/package_nso_to_oc/xe/xe_mpls.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.72.0/package_nso_to_oc/xe/xe_network_instances.py` & `nso-oc-2.73.0/package_nso_to_oc/xe/xe_network_instances.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.72.0/package_nso_to_oc/xe/xe_ospfv2.py` & `nso-oc-2.73.0/package_nso_to_oc/xe/xe_ospfv2.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.72.0/package_nso_to_oc/xe/xe_routing_policy.py` & `nso-oc-2.73.0/package_nso_to_oc/xe/xe_routing_policy.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.72.0/package_nso_to_oc/xe/xe_static_route.py` & `nso-oc-2.73.0/package_nso_to_oc/xe/xe_static_route.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.72.0/package_nso_to_oc/xe/xe_stp.py` & `nso-oc-2.73.0/package_nso_to_oc/xe/xe_stp.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.72.0/package_nso_to_oc/xe/xe_system.py` & `nso-oc-2.73.0/package_nso_to_oc/xe/xe_system.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.72.0/package_nso_to_oc/xe/xe_vlans.py` & `nso-oc-2.73.0/package_nso_to_oc/xe/xe_vlans.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.72.0/package_nso_to_oc/xr/common_xr.py` & `nso-oc-2.73.0/package_nso_to_oc/xr/common_xr.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.72.0/package_nso_to_oc/xr/main_xr.py` & `nso-oc-2.73.0/package_nso_to_oc/xr/main_xr.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.72.0/package_nso_to_oc/xr/xr_acls.py` & `nso-oc-2.73.0/package_nso_to_oc/xr/xr_acls.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.72.0/package_nso_to_oc/xr/xr_interfaces.py` & `nso-oc-2.73.0/package_nso_to_oc/xr/xr_interfaces.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.72.0/package_nso_to_oc/xr/xr_system.py` & `nso-oc-2.73.0/package_nso_to_oc/xr/xr_system.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.72.0/setup.py` & `nso-oc-2.73.0/setup.py`

 * *Files identical despite different names*

