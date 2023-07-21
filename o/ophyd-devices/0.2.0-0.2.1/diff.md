# Comparing `tmp/ophyd_devices-0.2.0.tar.gz` & `tmp/ophyd_devices-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ophyd_devices-0.2.0.tar", last modified: Tue Jul  4 15:35:52 2023, max compression
+gzip compressed data, was "ophyd_devices-0.2.1.tar", last modified: Fri Jul 21 09:29:38 2023, max compression
```

## Comparing `ophyd_devices-0.2.0.tar` & `ophyd_devices-0.2.1.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 15:35:52.644825 ophyd_devices-0.2.0/
--rw-rw-rw-   0 root         (0) root         (0)     1511 2023-06-28 12:14:54.000000 ophyd_devices-0.2.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2890 2023-07-04 15:35:52.644825 ophyd_devices-0.2.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2345 2023-06-28 12:25:42.000000 ophyd_devices-0.2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 15:35:52.634825 ophyd_devices-0.2.0/ophyd_devices/
--rw-r--r--   0 root         (0) root         (0)      485 2023-07-04 15:35:41.000000 ophyd_devices-0.2.0/ophyd_devices/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 15:35:52.635825 ophyd_devices-0.2.0/ophyd_devices/epics/
--rw-rw-rw-   0 root         (0) root         (0)     1898 2023-06-28 12:14:54.000000 ophyd_devices-0.2.0/ophyd_devices/epics/DeviceFactory.py
--rw-rw-rw-   0 root         (0) root         (0)      717 2023-06-28 12:14:54.000000 ophyd_devices-0.2.0/ophyd_devices/epics/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 15:35:52.638825 ophyd_devices-0.2.0/ophyd_devices/epics/devices/
--rw-r--r--   0 root         (0) root         (0)     7480 2023-07-04 15:35:41.000000 ophyd_devices-0.2.0/ophyd_devices/epics/devices/DelayGeneratorDG645.py
--rw-rw-rw-   0 root         (0) root         (0)     1104 2023-06-28 12:14:54.000000 ophyd_devices-0.2.0/ophyd_devices/epics/devices/InsertionDevice.py
--rw-rw-rw-   0 root         (0) root         (0)     3809 2023-06-28 12:14:54.000000 ophyd_devices-0.2.0/ophyd_devices/epics/devices/SpmBase.py
--rw-rw-rw-   0 root         (0) root         (0)    10676 2023-06-28 12:14:54.000000 ophyd_devices-0.2.0/ophyd_devices/epics/devices/X07MADevices.py
--rw-rw-rw-   0 root         (0) root         (0)     5233 2023-06-28 12:14:54.000000 ophyd_devices-0.2.0/ophyd_devices/epics/devices/XbpmBase.py
--rw-rw-rw-   0 root         (0) root         (0)      607 2023-06-28 12:14:54.000000 ophyd_devices-0.2.0/ophyd_devices/epics/devices/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      832 2023-06-28 12:14:54.000000 ophyd_devices-0.2.0/ophyd_devices/epics/devices/cSaxsVirtualMotors.py
--rw-rw-rw-   0 root         (0) root         (0)     4440 2023-06-28 12:14:54.000000 ophyd_devices-0.2.0/ophyd_devices/epics/devices/mono_dccm.py
--rw-rw-rw-   0 root         (0) root         (0)     2173 2023-06-28 12:14:54.000000 ophyd_devices-0.2.0/ophyd_devices/epics/devices/slits.py
--rw-rw-rw-   0 root         (0) root         (0)     2306 2023-06-28 12:14:54.000000 ophyd_devices-0.2.0/ophyd_devices/epics/devices/slsDetector.py
--rw-rw-rw-   0 root         (0) root         (0)     9182 2023-06-28 12:14:54.000000 ophyd_devices-0.2.0/ophyd_devices/epics/devices/specMotors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 15:35:52.638825 ophyd_devices-0.2.0/ophyd_devices/galil/
--rw-r--r--   0 root         (0) root         (0)       91 2023-07-04 15:35:41.000000 ophyd_devices-0.2.0/ophyd_devices/galil/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    19024 2023-06-28 12:14:54.000000 ophyd_devices-0.2.0/ophyd_devices/galil/galil_ophyd.py
--rw-r--r--   0 root         (0) root         (0)    19824 2023-07-04 15:35:41.000000 ophyd_devices-0.2.0/ophyd_devices/galil/sgalil_ophyd.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 15:35:52.639825 ophyd_devices-0.2.0/ophyd_devices/npoint/
--rw-rw-rw-   0 root         (0) root         (0)       49 2023-06-28 12:14:54.000000 ophyd_devices-0.2.0/ophyd_devices/npoint/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    16790 2023-06-28 12:14:54.000000 ophyd_devices-0.2.0/ophyd_devices/npoint/npoint.py
--rw-rw-rw-   0 root         (0) root         (0)    13172 2023-06-28 12:14:54.000000 ophyd_devices-0.2.0/ophyd_devices/npoint/npoint_ophyd.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 15:35:52.640825 ophyd_devices-0.2.0/ophyd_devices/rt_lamni/
--rw-rw-rw-   0 root         (0) root         (0)       60 2023-06-28 12:14:54.000000 ophyd_devices-0.2.0/ophyd_devices/rt_lamni/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    31617 2023-06-28 12:14:54.000000 ophyd_devices-0.2.0/ophyd_devices/rt_lamni/rt_lamni_ophyd.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 15:35:52.640825 ophyd_devices-0.2.0/ophyd_devices/sim/
--rw-rw-rw-   0 root         (0) root         (0)      122 2023-06-28 12:14:54.000000 ophyd_devices-0.2.0/ophyd_devices/sim/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    28877 2023-06-28 12:14:54.000000 ophyd_devices-0.2.0/ophyd_devices/sim/sim.py
--rw-rw-rw-   0 root         (0) root         (0)     7018 2023-06-28 12:14:54.000000 ophyd_devices-0.2.0/ophyd_devices/sim/sim_xtreme.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 15:35:52.642825 ophyd_devices-0.2.0/ophyd_devices/smaract/
--rw-rw-rw-   0 root         (0) root         (0)       90 2023-06-28 12:14:54.000000 ophyd_devices-0.2.0/ophyd_devices/smaract/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1303 2023-06-28 12:14:54.000000 ophyd_devices-0.2.0/ophyd_devices/smaract/serializer.py
--rw-rw-rw-   0 root         (0) root         (0)    19903 2023-06-28 12:14:54.000000 ophyd_devices-0.2.0/ophyd_devices/smaract/smaract_controller.py
--rw-rw-rw-   0 root         (0) root         (0)     5212 2023-06-28 12:14:54.000000 ophyd_devices-0.2.0/ophyd_devices/smaract/smaract_errors.py
--rw-rw-rw-   0 root         (0) root         (0)    10338 2023-06-28 12:14:54.000000 ophyd_devices-0.2.0/ophyd_devices/smaract/smaract_ophyd.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 15:35:52.643825 ophyd_devices-0.2.0/ophyd_devices/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-28 12:14:54.000000 ophyd_devices-0.2.0/ophyd_devices/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3269 2023-06-28 12:14:54.000000 ophyd_devices-0.2.0/ophyd_devices/utils/controller.py
--rw-rw-rw-   0 root         (0) root         (0)      457 2023-06-28 12:14:54.000000 ophyd_devices-0.2.0/ophyd_devices/utils/re_test.py
--rw-rw-rw-   0 root         (0) root         (0)     7014 2023-06-28 12:14:54.000000 ophyd_devices-0.2.0/ophyd_devices/utils/socket.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 15:35:52.643825 ophyd_devices-0.2.0/ophyd_devices.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2890 2023-07-04 15:35:52.000000 ophyd_devices-0.2.0/ophyd_devices.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1544 2023-07-04 15:35:52.000000 ophyd_devices-0.2.0/ophyd_devices.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-04 15:35:52.000000 ophyd_devices-0.2.0/ophyd_devices.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       89 2023-07-04 15:35:52.000000 ophyd_devices-0.2.0/ophyd_devices.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-07-04 15:35:52.000000 ophyd_devices-0.2.0/ophyd_devices.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      651 2023-07-04 15:35:52.644825 ophyd_devices-0.2.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      296 2023-07-04 15:35:50.000000 ophyd_devices-0.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 09:29:38.201900 ophyd_devices-0.2.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1511 2023-06-28 12:14:54.000000 ophyd_devices-0.2.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2890 2023-07-21 09:29:38.201900 ophyd_devices-0.2.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2345 2023-06-28 12:25:42.000000 ophyd_devices-0.2.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 09:29:38.188900 ophyd_devices-0.2.1/ophyd_devices/
+-rw-r--r--   0 root         (0) root         (0)      485 2023-07-04 15:35:41.000000 ophyd_devices-0.2.1/ophyd_devices/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 09:29:38.188900 ophyd_devices-0.2.1/ophyd_devices/epics/
+-rw-rw-rw-   0 root         (0) root         (0)     1898 2023-06-28 12:14:54.000000 ophyd_devices-0.2.1/ophyd_devices/epics/DeviceFactory.py
+-rw-rw-rw-   0 root         (0) root         (0)      717 2023-06-28 12:14:54.000000 ophyd_devices-0.2.1/ophyd_devices/epics/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 09:29:38.193900 ophyd_devices-0.2.1/ophyd_devices/epics/devices/
+-rw-r--r--   0 root         (0) root         (0)     7480 2023-07-04 15:35:41.000000 ophyd_devices-0.2.1/ophyd_devices/epics/devices/DelayGeneratorDG645.py
+-rw-rw-rw-   0 root         (0) root         (0)     1104 2023-06-28 12:14:54.000000 ophyd_devices-0.2.1/ophyd_devices/epics/devices/InsertionDevice.py
+-rw-rw-rw-   0 root         (0) root         (0)     3809 2023-06-28 12:14:54.000000 ophyd_devices-0.2.1/ophyd_devices/epics/devices/SpmBase.py
+-rw-rw-rw-   0 root         (0) root         (0)    10676 2023-06-28 12:14:54.000000 ophyd_devices-0.2.1/ophyd_devices/epics/devices/X07MADevices.py
+-rw-rw-rw-   0 root         (0) root         (0)     5233 2023-06-28 12:14:54.000000 ophyd_devices-0.2.1/ophyd_devices/epics/devices/XbpmBase.py
+-rw-rw-rw-   0 root         (0) root         (0)      607 2023-06-28 12:14:54.000000 ophyd_devices-0.2.1/ophyd_devices/epics/devices/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      832 2023-06-28 12:14:54.000000 ophyd_devices-0.2.1/ophyd_devices/epics/devices/cSaxsVirtualMotors.py
+-rw-rw-rw-   0 root         (0) root         (0)     4440 2023-06-28 12:14:54.000000 ophyd_devices-0.2.1/ophyd_devices/epics/devices/mono_dccm.py
+-rw-rw-rw-   0 root         (0) root         (0)     2173 2023-06-28 12:14:54.000000 ophyd_devices-0.2.1/ophyd_devices/epics/devices/slits.py
+-rw-rw-rw-   0 root         (0) root         (0)     2306 2023-06-28 12:14:54.000000 ophyd_devices-0.2.1/ophyd_devices/epics/devices/slsDetector.py
+-rw-rw-rw-   0 root         (0) root         (0)     9182 2023-06-28 12:14:54.000000 ophyd_devices-0.2.1/ophyd_devices/epics/devices/specMotors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 09:29:38.194900 ophyd_devices-0.2.1/ophyd_devices/galil/
+-rw-r--r--   0 root         (0) root         (0)       91 2023-07-04 15:35:41.000000 ophyd_devices-0.2.1/ophyd_devices/galil/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    19024 2023-06-28 12:14:54.000000 ophyd_devices-0.2.1/ophyd_devices/galil/galil_ophyd.py
+-rw-r--r--   0 root         (0) root         (0)    19824 2023-07-04 15:35:41.000000 ophyd_devices-0.2.1/ophyd_devices/galil/sgalil_ophyd.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 09:29:38.195900 ophyd_devices-0.2.1/ophyd_devices/npoint/
+-rw-rw-rw-   0 root         (0) root         (0)       49 2023-06-28 12:14:54.000000 ophyd_devices-0.2.1/ophyd_devices/npoint/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    16790 2023-06-28 12:14:54.000000 ophyd_devices-0.2.1/ophyd_devices/npoint/npoint.py
+-rw-rw-rw-   0 root         (0) root         (0)    13172 2023-06-28 12:14:54.000000 ophyd_devices-0.2.1/ophyd_devices/npoint/npoint_ophyd.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 09:29:38.195900 ophyd_devices-0.2.1/ophyd_devices/rt_lamni/
+-rw-rw-rw-   0 root         (0) root         (0)       60 2023-06-28 12:14:54.000000 ophyd_devices-0.2.1/ophyd_devices/rt_lamni/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    31617 2023-06-28 12:14:54.000000 ophyd_devices-0.2.1/ophyd_devices/rt_lamni/rt_lamni_ophyd.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 09:29:38.196900 ophyd_devices-0.2.1/ophyd_devices/sim/
+-rw-rw-rw-   0 root         (0) root         (0)      122 2023-06-28 12:14:54.000000 ophyd_devices-0.2.1/ophyd_devices/sim/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    28937 2023-07-21 09:29:26.000000 ophyd_devices-0.2.1/ophyd_devices/sim/sim.py
+-rw-rw-rw-   0 root         (0) root         (0)     7018 2023-06-28 12:14:54.000000 ophyd_devices-0.2.1/ophyd_devices/sim/sim_xtreme.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 09:29:38.198900 ophyd_devices-0.2.1/ophyd_devices/smaract/
+-rw-rw-rw-   0 root         (0) root         (0)       90 2023-06-28 12:14:54.000000 ophyd_devices-0.2.1/ophyd_devices/smaract/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1303 2023-06-28 12:14:54.000000 ophyd_devices-0.2.1/ophyd_devices/smaract/serializer.py
+-rw-rw-rw-   0 root         (0) root         (0)    19903 2023-06-28 12:14:54.000000 ophyd_devices-0.2.1/ophyd_devices/smaract/smaract_controller.py
+-rw-rw-rw-   0 root         (0) root         (0)     5212 2023-06-28 12:14:54.000000 ophyd_devices-0.2.1/ophyd_devices/smaract/smaract_errors.py
+-rw-rw-rw-   0 root         (0) root         (0)    10338 2023-06-28 12:14:54.000000 ophyd_devices-0.2.1/ophyd_devices/smaract/smaract_ophyd.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 09:29:38.199900 ophyd_devices-0.2.1/ophyd_devices/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-28 12:14:54.000000 ophyd_devices-0.2.1/ophyd_devices/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3269 2023-06-28 12:14:54.000000 ophyd_devices-0.2.1/ophyd_devices/utils/controller.py
+-rw-rw-rw-   0 root         (0) root         (0)      457 2023-06-28 12:14:54.000000 ophyd_devices-0.2.1/ophyd_devices/utils/re_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     7014 2023-06-28 12:14:54.000000 ophyd_devices-0.2.1/ophyd_devices/utils/socket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 09:29:38.200900 ophyd_devices-0.2.1/ophyd_devices.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2890 2023-07-21 09:29:38.000000 ophyd_devices-0.2.1/ophyd_devices.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1544 2023-07-21 09:29:38.000000 ophyd_devices-0.2.1/ophyd_devices.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 09:29:38.000000 ophyd_devices-0.2.1/ophyd_devices.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       89 2023-07-21 09:29:38.000000 ophyd_devices-0.2.1/ophyd_devices.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-07-21 09:29:38.000000 ophyd_devices-0.2.1/ophyd_devices.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      651 2023-07-21 09:29:38.201900 ophyd_devices-0.2.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      296 2023-07-21 09:29:36.000000 ophyd_devices-0.2.1/setup.py
```

### Comparing `ophyd_devices-0.2.0/LICENSE` & `ophyd_devices-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ophyd_devices-0.2.0/PKG-INFO` & `ophyd_devices-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ophyd_devices
-Version: 0.2.0
+Version: 0.2.1
 Summary: Custom device implementations based on the ophyd hardware abstraction layer
 Home-page: https://gitlab.psi.ch/bec/ophyd_devices
 License: UNKNOWN
 Project-URL: Bug Tracker, https://gitlab.psi.ch/bec/ophyd_devices/issues
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `ophyd_devices-0.2.0/README.md` & `ophyd_devices-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-0.2.0/ophyd_devices/epics/DeviceFactory.py` & `ophyd_devices-0.2.1/ophyd_devices/epics/DeviceFactory.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-0.2.0/ophyd_devices/epics/__init__.py` & `ophyd_devices-0.2.1/ophyd_devices/epics/__init__.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-0.2.0/ophyd_devices/epics/devices/DelayGeneratorDG645.py` & `ophyd_devices-0.2.1/ophyd_devices/epics/devices/DelayGeneratorDG645.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-0.2.0/ophyd_devices/epics/devices/InsertionDevice.py` & `ophyd_devices-0.2.1/ophyd_devices/epics/devices/InsertionDevice.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-0.2.0/ophyd_devices/epics/devices/SpmBase.py` & `ophyd_devices-0.2.1/ophyd_devices/epics/devices/SpmBase.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-0.2.0/ophyd_devices/epics/devices/X07MADevices.py` & `ophyd_devices-0.2.1/ophyd_devices/epics/devices/X07MADevices.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-0.2.0/ophyd_devices/epics/devices/XbpmBase.py` & `ophyd_devices-0.2.1/ophyd_devices/epics/devices/XbpmBase.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-0.2.0/ophyd_devices/epics/devices/__init__.py` & `ophyd_devices-0.2.1/ophyd_devices/epics/devices/__init__.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-0.2.0/ophyd_devices/epics/devices/cSaxsVirtualMotors.py` & `ophyd_devices-0.2.1/ophyd_devices/epics/devices/cSaxsVirtualMotors.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-0.2.0/ophyd_devices/epics/devices/mono_dccm.py` & `ophyd_devices-0.2.1/ophyd_devices/epics/devices/mono_dccm.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-0.2.0/ophyd_devices/epics/devices/slits.py` & `ophyd_devices-0.2.1/ophyd_devices/epics/devices/slits.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-0.2.0/ophyd_devices/epics/devices/slsDetector.py` & `ophyd_devices-0.2.1/ophyd_devices/epics/devices/slsDetector.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-0.2.0/ophyd_devices/epics/devices/specMotors.py` & `ophyd_devices-0.2.1/ophyd_devices/epics/devices/specMotors.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-0.2.0/ophyd_devices/galil/galil_ophyd.py` & `ophyd_devices-0.2.1/ophyd_devices/galil/galil_ophyd.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-0.2.0/ophyd_devices/galil/sgalil_ophyd.py` & `ophyd_devices-0.2.1/ophyd_devices/galil/sgalil_ophyd.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-0.2.0/ophyd_devices/npoint/npoint.py` & `ophyd_devices-0.2.1/ophyd_devices/npoint/npoint.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-0.2.0/ophyd_devices/npoint/npoint_ophyd.py` & `ophyd_devices-0.2.1/ophyd_devices/npoint/npoint_ophyd.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-0.2.0/ophyd_devices/rt_lamni/rt_lamni_ophyd.py` & `ophyd_devices-0.2.1/ophyd_devices/rt_lamni/rt_lamni_ophyd.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-0.2.0/ophyd_devices/sim/sim.py` & `ophyd_devices-0.2.1/ophyd_devices/sim/sim.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,14 +40,15 @@
         self._metadata.update(
             connected=True,
             write_access=False,
         )
 
     def get(self):
         self._readback = self.parent.sim_state["readback"]
+        self.parent.sim_state["readback_ts"] = ttime.time()
         return self._readback
 
     def describe(self):
         res = super().describe()
         # There should be only one key here, but for the sake of
         # generality....
         for k in res:
```

### Comparing `ophyd_devices-0.2.0/ophyd_devices/sim/sim_xtreme.py` & `ophyd_devices-0.2.1/ophyd_devices/sim/sim_xtreme.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-0.2.0/ophyd_devices/smaract/serializer.py` & `ophyd_devices-0.2.1/ophyd_devices/smaract/serializer.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-0.2.0/ophyd_devices/smaract/smaract_controller.py` & `ophyd_devices-0.2.1/ophyd_devices/smaract/smaract_controller.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-0.2.0/ophyd_devices/smaract/smaract_errors.py` & `ophyd_devices-0.2.1/ophyd_devices/smaract/smaract_errors.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-0.2.0/ophyd_devices/smaract/smaract_ophyd.py` & `ophyd_devices-0.2.1/ophyd_devices/smaract/smaract_ophyd.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-0.2.0/ophyd_devices/utils/controller.py` & `ophyd_devices-0.2.1/ophyd_devices/utils/controller.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-0.2.0/ophyd_devices/utils/socket.py` & `ophyd_devices-0.2.1/ophyd_devices/utils/socket.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-0.2.0/ophyd_devices.egg-info/PKG-INFO` & `ophyd_devices-0.2.1/ophyd_devices.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ophyd-devices
-Version: 0.2.0
+Version: 0.2.1
 Summary: Custom device implementations based on the ophyd hardware abstraction layer
 Home-page: https://gitlab.psi.ch/bec/ophyd_devices
 License: UNKNOWN
 Project-URL: Bug Tracker, https://gitlab.psi.ch/bec/ophyd_devices/issues
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `ophyd_devices-0.2.0/ophyd_devices.egg-info/SOURCES.txt` & `ophyd_devices-0.2.1/ophyd_devices.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ophyd_devices-0.2.0/setup.cfg` & `ophyd_devices-0.2.1/setup.cfg`

 * *Files identical despite different names*

