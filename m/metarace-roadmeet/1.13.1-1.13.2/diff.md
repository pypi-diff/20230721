# Comparing `tmp/metarace-roadmeet-1.13.1.tar.gz` & `tmp/metarace-roadmeet-1.13.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metarace-roadmeet-1.13.1.tar", last modified: Wed Jun 28 13:24:28 2023, max compression
+gzip compressed data, was "metarace-roadmeet-1.13.2.tar", last modified: Fri Jul 21 05:04:06 2023, max compression
```

## Comparing `metarace-roadmeet-1.13.1.tar` & `metarace-roadmeet-1.13.2.tar`

### file list

```diff
@@ -1,33 +1,32 @@
-drwxr-xr-x   0 ndf       (1000) ndf       (1000)        0 2023-06-28 13:24:28.009016 metarace-roadmeet-1.13.1/
--rw-r--r--   0 ndf       (1000) ndf       (1000)     1063 2022-11-24 00:04:20.000000 metarace-roadmeet-1.13.1/LICENSE
--rw-r--r--   0 ndf       (1000) ndf       (1000)       26 2022-11-24 00:09:22.000000 metarace-roadmeet-1.13.1/MANIFEST.in
--rw-r--r--   0 ndf       (1000) ndf       (1000)     1610 2023-06-28 13:24:28.009016 metarace-roadmeet-1.13.1/PKG-INFO
--rw-r--r--   0 ndf       (1000) ndf       (1000)     1051 2023-06-28 10:18:08.000000 metarace-roadmeet-1.13.1/README.md
--rw-r--r--   0 ndf       (1000) ndf       (1000)      746 2023-06-28 13:23:58.000000 metarace-roadmeet-1.13.1/pyproject.toml
--rw-r--r--   0 ndf       (1000) ndf       (1000)       38 2023-06-28 13:24:28.009016 metarace-roadmeet-1.13.1/setup.cfg
-drwxr-xr-x   0 ndf       (1000) ndf       (1000)        0 2023-06-28 13:24:28.005016 metarace-roadmeet-1.13.1/src/
-drwxr-xr-x   0 ndf       (1000) ndf       (1000)        0 2023-06-28 13:24:28.005016 metarace-roadmeet-1.13.1/src/metarace_roadmeet.egg-info/
--rw-r--r--   0 ndf       (1000) ndf       (1000)     1610 2023-06-28 13:24:27.000000 metarace-roadmeet-1.13.1/src/metarace_roadmeet.egg-info/PKG-INFO
--rw-r--r--   0 ndf       (1000) ndf       (1000)      738 2023-06-28 13:24:27.000000 metarace-roadmeet-1.13.1/src/metarace_roadmeet.egg-info/SOURCES.txt
--rw-r--r--   0 ndf       (1000) ndf       (1000)        1 2023-06-28 13:24:27.000000 metarace-roadmeet-1.13.1/src/metarace_roadmeet.egg-info/dependency_links.txt
--rw-r--r--   0 ndf       (1000) ndf       (1000)       43 2023-06-28 13:24:27.000000 metarace-roadmeet-1.13.1/src/metarace_roadmeet.egg-info/entry_points.txt
--rw-r--r--   0 ndf       (1000) ndf       (1000)       16 2023-06-28 13:24:27.000000 metarace-roadmeet-1.13.1/src/metarace_roadmeet.egg-info/requires.txt
--rw-r--r--   0 ndf       (1000) ndf       (1000)        9 2023-06-28 13:24:27.000000 metarace-roadmeet-1.13.1/src/metarace_roadmeet.egg-info/top_level.txt
-drwxr-xr-x   0 ndf       (1000) ndf       (1000)        0 2023-06-28 13:24:28.009016 metarace-roadmeet-1.13.1/src/roadmeet/
--rw-r--r--   0 ndf       (1000) ndf       (1000)    83719 2023-06-28 13:24:12.000000 metarace-roadmeet-1.13.1/src/roadmeet/__init__.py
--rw-r--r--   0 ndf       (1000) ndf       (1000)       79 2022-11-24 06:32:10.000000 metarace-roadmeet-1.13.1/src/roadmeet/__main__.py
--rw-r--r--   0 ndf       (1000) ndf       (1000)   107594 2023-06-23 23:51:59.000000 metarace-roadmeet-1.13.1/src/roadmeet/irtt.py
--rw-r--r--   0 ndf       (1000) ndf       (1000)   179865 2023-06-25 10:23:12.000000 metarace-roadmeet-1.13.1/src/roadmeet/rms.py
--rw-r--r--   0 ndf       (1000) ndf       (1000)    62271 2023-06-23 12:39:08.000000 metarace-roadmeet-1.13.1/src/roadmeet/trtt.py
-drwxr-xr-x   0 ndf       (1000) ndf       (1000)        0 2023-06-28 13:24:28.009016 metarace-roadmeet-1.13.1/src/roadmeet/ui/
--rw-r--r--   0 ndf       (1000) ndf       (1000)        0 2023-06-28 12:18:14.000000 metarace-roadmeet-1.13.1/src/roadmeet/ui/__init__.py
--rw-------   0 ndf       (1000) ndf       (1000)    13762 2023-05-30 11:27:50.000000 metarace-roadmeet-1.13.1/src/roadmeet/ui/edit_times.ui
--rw-------   0 ndf       (1000) ndf       (1000)     4496 2023-05-30 11:27:50.000000 metarace-roadmeet-1.13.1/src/roadmeet/ui/irtt.ui
--rw-------   0 ndf       (1000) ndf       (1000)     7206 2023-06-01 06:00:37.000000 metarace-roadmeet-1.13.1/src/roadmeet/ui/new_start.ui
--rw-------   0 ndf       (1000) ndf       (1000)     2356 2023-06-24 03:51:06.000000 metarace-roadmeet-1.13.1/src/roadmeet/ui/rider_context.ui
--rw-------   0 ndf       (1000) ndf       (1000)     5625 2023-05-30 11:27:50.000000 metarace-roadmeet-1.13.1/src/roadmeet/ui/rms.ui
--rw-------   0 ndf       (1000) ndf       (1000)     5657 2023-06-14 12:44:18.000000 metarace-roadmeet-1.13.1/src/roadmeet/ui/rms_context.ui
--rw-r--r--   0 ndf       (1000) ndf       (1000)    44070 2023-06-13 02:56:48.000000 metarace-roadmeet-1.13.1/src/roadmeet/ui/roadmeet.ui
--rw-------   0 ndf       (1000) ndf       (1000)     8749 2023-05-30 11:27:50.000000 metarace-roadmeet-1.13.1/src/roadmeet/ui/swap_rider.ui
--rw-------   0 ndf       (1000) ndf       (1000)     4389 2023-05-30 11:27:50.000000 metarace-roadmeet-1.13.1/src/roadmeet/ui/tod_context.ui
--rw-r--r--   0 ndf       (1000) ndf       (1000)    37130 2023-06-27 13:33:24.000000 metarace-roadmeet-1.13.1/src/roadmeet/uiutil.py
+drwxr-xr-x   0 ndf       (1000) ndf       (1000)        0 2023-07-21 05:04:06.075077 metarace-roadmeet-1.13.2/
+-rw-r--r--   0 ndf       (1000) ndf       (1000)     1063 2023-07-07 01:56:04.000000 metarace-roadmeet-1.13.2/LICENSE
+-rw-r--r--   0 ndf       (1000) ndf       (1000)       26 2022-11-24 00:09:22.000000 metarace-roadmeet-1.13.2/MANIFEST.in
+-rw-r--r--   0 ndf       (1000) ndf       (1000)     1970 2023-07-21 05:04:06.075077 metarace-roadmeet-1.13.2/PKG-INFO
+-rw-r--r--   0 ndf       (1000) ndf       (1000)     1411 2023-07-17 02:48:09.000000 metarace-roadmeet-1.13.2/README.md
+-rw-r--r--   0 ndf       (1000) ndf       (1000)      746 2023-07-21 05:03:25.000000 metarace-roadmeet-1.13.2/pyproject.toml
+-rw-r--r--   0 ndf       (1000) ndf       (1000)       38 2023-07-21 05:04:06.075077 metarace-roadmeet-1.13.2/setup.cfg
+drwxr-xr-x   0 ndf       (1000) ndf       (1000)        0 2023-07-21 05:04:06.067076 metarace-roadmeet-1.13.2/src/
+drwxr-xr-x   0 ndf       (1000) ndf       (1000)        0 2023-07-21 05:04:06.067076 metarace-roadmeet-1.13.2/src/metarace_roadmeet.egg-info/
+-rw-r--r--   0 ndf       (1000) ndf       (1000)     1970 2023-07-21 05:04:05.000000 metarace-roadmeet-1.13.2/src/metarace_roadmeet.egg-info/PKG-INFO
+-rw-r--r--   0 ndf       (1000) ndf       (1000)      708 2023-07-21 05:04:06.000000 metarace-roadmeet-1.13.2/src/metarace_roadmeet.egg-info/SOURCES.txt
+-rw-r--r--   0 ndf       (1000) ndf       (1000)        1 2023-07-21 05:04:05.000000 metarace-roadmeet-1.13.2/src/metarace_roadmeet.egg-info/dependency_links.txt
+-rw-r--r--   0 ndf       (1000) ndf       (1000)       43 2023-07-21 05:04:05.000000 metarace-roadmeet-1.13.2/src/metarace_roadmeet.egg-info/entry_points.txt
+-rw-r--r--   0 ndf       (1000) ndf       (1000)       16 2023-07-21 05:04:05.000000 metarace-roadmeet-1.13.2/src/metarace_roadmeet.egg-info/requires.txt
+-rw-r--r--   0 ndf       (1000) ndf       (1000)        9 2023-07-21 05:04:05.000000 metarace-roadmeet-1.13.2/src/metarace_roadmeet.egg-info/top_level.txt
+drwxr-xr-x   0 ndf       (1000) ndf       (1000)        0 2023-07-21 05:04:06.071076 metarace-roadmeet-1.13.2/src/roadmeet/
+-rw-r--r--   0 ndf       (1000) ndf       (1000)    83826 2023-07-21 04:48:30.000000 metarace-roadmeet-1.13.2/src/roadmeet/__init__.py
+-rw-r--r--   0 ndf       (1000) ndf       (1000)       79 2022-11-24 06:32:10.000000 metarace-roadmeet-1.13.2/src/roadmeet/__main__.py
+-rw-r--r--   0 ndf       (1000) ndf       (1000)   110436 2023-07-20 09:05:00.000000 metarace-roadmeet-1.13.2/src/roadmeet/irtt.py
+-rw-r--r--   0 ndf       (1000) ndf       (1000)   189881 2023-07-20 14:47:52.000000 metarace-roadmeet-1.13.2/src/roadmeet/rms.py
+-rw-r--r--   0 ndf       (1000) ndf       (1000)    60325 2023-07-20 06:54:09.000000 metarace-roadmeet-1.13.2/src/roadmeet/trtt.py
+drwxr-xr-x   0 ndf       (1000) ndf       (1000)        0 2023-07-21 05:04:06.075077 metarace-roadmeet-1.13.2/src/roadmeet/ui/
+-r--r--r--   0 ndf       (1000) ndf       (1000)        0 2023-06-28 12:18:14.000000 metarace-roadmeet-1.13.2/src/roadmeet/ui/__init__.py
+-r--r--r--   0 ndf       (1000) ndf       (1000)     4496 2023-05-30 11:27:50.000000 metarace-roadmeet-1.13.2/src/roadmeet/ui/irtt.ui
+-r--r--r--   0 ndf       (1000) ndf       (1000)     7206 2023-06-01 06:00:37.000000 metarace-roadmeet-1.13.2/src/roadmeet/ui/new_start.ui
+-r--r--r--   0 ndf       (1000) ndf       (1000)     2356 2023-06-24 03:51:06.000000 metarace-roadmeet-1.13.2/src/roadmeet/ui/rider_context.ui
+-r--r--r--   0 ndf       (1000) ndf       (1000)     5625 2023-05-30 11:27:50.000000 metarace-roadmeet-1.13.2/src/roadmeet/ui/rms.ui
+-r--r--r--   0 ndf       (1000) ndf       (1000)     5657 2023-06-14 12:44:18.000000 metarace-roadmeet-1.13.2/src/roadmeet/ui/rms_context.ui
+-r--r--r--   0 ndf       (1000) ndf       (1000)    42196 2023-07-16 04:51:22.000000 metarace-roadmeet-1.13.2/src/roadmeet/ui/roadmeet.ui
+-r--r--r--   0 ndf       (1000) ndf       (1000)     8749 2023-05-30 11:27:50.000000 metarace-roadmeet-1.13.2/src/roadmeet/ui/swap_rider.ui
+-r--r--r--   0 ndf       (1000) ndf       (1000)     4389 2023-05-30 11:27:50.000000 metarace-roadmeet-1.13.2/src/roadmeet/ui/tod_context.ui
+-rw-r--r--   0 ndf       (1000) ndf       (1000)    45889 2023-07-21 04:36:10.000000 metarace-roadmeet-1.13.2/src/roadmeet/uiutil.py
```

### Comparing `metarace-roadmeet-1.13.1/LICENSE` & `metarace-roadmeet-1.13.2/LICENSE`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 ndf-zz
+Copyright (c) 2023 ndf-zz
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `metarace-roadmeet-1.13.1/PKG-INFO` & `metarace-roadmeet-1.13.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metarace-roadmeet
-Version: 1.13.1
+Version: 1.13.2
 Summary: Timing and result application for road cycling events
 Author-email: Nathan Fraser <ndf-zz@6-v.org>
 License: MIT
 Project-URL: homepage, https://github.com/ndf-zz/metarace-roadmeet
 Keywords: roadrace,timetrial,transponder
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Other/Nonlisted Topic
@@ -18,37 +18,63 @@
 
 Timing and result application for UCI Part 2 Road Races,
 UCI Part 5 Cyclo-Cross, criterium, road handicap and
 ad-hoc time trial events.
 
 ![roadmeet screenshot](screenshot.png "roadmeet")
 
+
+## Usage
+
+Create a new meet and open it:
+
+	$ roadmeet
+
+Open an existing road meet:
+
+	$ roadmeet PATH
+
+Edit default configuration:
+
+	$ roadmeet --edit-default
+
+
 ## Requirements
 
    - Python >= 3.9
    - Gtk >= 3.0
    - metarace >= 2.1.1
    - tex-gyre fonts (optional, recommended)
    - evince (optional, recommended)
    - mosquitto (optional)
 
 
 ## Installation
 
+Download the debian installer script and run:
+
+	$ sh install_deb.sh
+
+Alternatively perform the steps listed below.
+
 ### Debian 11+
 
 Install system requirements for roadmeet and metarace with apt:
 
 	$ sudo apt install python3-venv python3-pip python3-cairo python3-gi python3-gi-cairo
 	$ sudo apt install gir1.2-gtk-3.0 gir1.2-rsvg-2.0 gir1.2-pango-1.0 tex-gyre
 	$ sudo apt install python3-serial python3-paho-mqtt python3-dateutil python3-xlwt
 
+Optionally add PDF viewer and MQTT broker:
+
+	$ sudo apt install evince mosquitto
+
 If not already created, add a virtualenv for metarace packages:
 
 	$ mkdir -p ~/Documents/metarace
 	$ python3 -m venv --system-site-packages ~/Documents/metarace/venv
 
-Activate the virtualenv and install ttstart with pip:
+Activate the virtualenv and install roadmeet with pip:
 
 	$ source ~/Documents/metarace/venv/bin/activate
 	(venv) $ pip3 install metarace-roadmeet
```

### Comparing `metarace-roadmeet-1.13.1/pyproject.toml` & `metarace-roadmeet-1.13.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=62"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "metarace-roadmeet"
-version = "1.13.1"
+version = "1.13.2"
 description = "Timing and result application for road cycling events"
 readme = "README.md"
 requires-python = ">=3.9"
 license = {text = "MIT"}
 keywords = ["roadrace", "timetrial", "transponder"]
 authors = [
     {email = "ndf-zz@6-v.org", name = "Nathan Fraser"}
@@ -16,15 +16,15 @@
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Topic :: Other/Nonlisted Topic",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
 ]
 dependencies = [
-    "metarace>=2.1.2",
+    "metarace>=2.1.4",
 ]
 [project.urls]
 homepage = "https://github.com/ndf-zz/metarace-roadmeet"
 
 [project.scripts]
 roadmeet = "roadmeet:main"
```

### Comparing `metarace-roadmeet-1.13.1/src/metarace_roadmeet.egg-info/PKG-INFO` & `metarace-roadmeet-1.13.2/src/metarace_roadmeet.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metarace-roadmeet
-Version: 1.13.1
+Version: 1.13.2
 Summary: Timing and result application for road cycling events
 Author-email: Nathan Fraser <ndf-zz@6-v.org>
 License: MIT
 Project-URL: homepage, https://github.com/ndf-zz/metarace-roadmeet
 Keywords: roadrace,timetrial,transponder
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Other/Nonlisted Topic
@@ -18,37 +18,63 @@
 
 Timing and result application for UCI Part 2 Road Races,
 UCI Part 5 Cyclo-Cross, criterium, road handicap and
 ad-hoc time trial events.
 
 ![roadmeet screenshot](screenshot.png "roadmeet")
 
+
+## Usage
+
+Create a new meet and open it:
+
+	$ roadmeet
+
+Open an existing road meet:
+
+	$ roadmeet PATH
+
+Edit default configuration:
+
+	$ roadmeet --edit-default
+
+
 ## Requirements
 
    - Python >= 3.9
    - Gtk >= 3.0
    - metarace >= 2.1.1
    - tex-gyre fonts (optional, recommended)
    - evince (optional, recommended)
    - mosquitto (optional)
 
 
 ## Installation
 
+Download the debian installer script and run:
+
+	$ sh install_deb.sh
+
+Alternatively perform the steps listed below.
+
 ### Debian 11+
 
 Install system requirements for roadmeet and metarace with apt:
 
 	$ sudo apt install python3-venv python3-pip python3-cairo python3-gi python3-gi-cairo
 	$ sudo apt install gir1.2-gtk-3.0 gir1.2-rsvg-2.0 gir1.2-pango-1.0 tex-gyre
 	$ sudo apt install python3-serial python3-paho-mqtt python3-dateutil python3-xlwt
 
+Optionally add PDF viewer and MQTT broker:
+
+	$ sudo apt install evince mosquitto
+
 If not already created, add a virtualenv for metarace packages:
 
 	$ mkdir -p ~/Documents/metarace
 	$ python3 -m venv --system-site-packages ~/Documents/metarace/venv
 
-Activate the virtualenv and install ttstart with pip:
+Activate the virtualenv and install roadmeet with pip:
 
 	$ source ~/Documents/metarace/venv/bin/activate
 	(venv) $ pip3 install metarace-roadmeet
```

### Comparing `metarace-roadmeet-1.13.1/src/metarace_roadmeet.egg-info/SOURCES.txt` & `metarace-roadmeet-1.13.2/src/metarace_roadmeet.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 src/roadmeet/__init__.py
 src/roadmeet/__main__.py
 src/roadmeet/irtt.py
 src/roadmeet/rms.py
 src/roadmeet/trtt.py
 src/roadmeet/uiutil.py
 src/roadmeet/ui/__init__.py
-src/roadmeet/ui/edit_times.ui
 src/roadmeet/ui/irtt.ui
 src/roadmeet/ui/new_start.ui
 src/roadmeet/ui/rider_context.ui
 src/roadmeet/ui/rms.ui
 src/roadmeet/ui/rms_context.ui
 src/roadmeet/ui/roadmeet.ui
 src/roadmeet/ui/swap_rider.ui
```

### Comparing `metarace-roadmeet-1.13.1/src/roadmeet/__init__.py` & `metarace-roadmeet-1.13.2/src/roadmeet/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,217 +17,254 @@
 
 gi.require_version("Gdk", "3.0")
 from gi.repository import Gdk
 
 from metarace import jsonconfig
 from metarace import tod
 from metarace import riderdb
-from metarace import eventdb
-from metarace.telegraph import telegraph
-from metarace import export
+from metarace.telegraph import telegraph, _CONFIG_SCHEMA as _TG_SCHEMA
+from metarace.export import mirror, _CONFIG_SCHEMA as _EXPORT_SCHEMA
 from metarace.decoder import decoder
-from metarace.decoder.rru import rru
-from metarace.decoder.rrs import rrs
-from metarace.decoder.thbc import thbc
-from metarace.timy import timy
+from metarace.decoder.rru import rru, _CONFIG_SCHEMA as _RRU_SCHEMA
+from metarace.decoder.rrs import rrs, _CONFIG_SCHEMA as _RRS_SCHEMA
+from metarace.decoder.thbc import thbc, _CONFIG_SCHEMA as _THBC_SCHEMA
+from metarace.timy import timy, _CONFIG_SCHEMA as _TIMY_SCHEMA
 from metarace import strops
 from metarace import report
 
 from . import uiutil
-from roadmeet.rms import rms
-from roadmeet.irtt import irtt
-from roadmeet.trtt import trtt
+from roadmeet.rms import rms, _CONFIG_SCHEMA as _RMS_SCHEMA
+from roadmeet.irtt import irtt, _CONFIG_SCHEMA as _IRTT_SCHEMA
+from roadmeet.trtt import trtt, _CONFIG_SCHEMA as _TRTT_SCHEMA
 
-VERSION = '1.13.1'
+VERSION = '1.13.2'
 LOGFILE = 'event.log'
 LOGFILE_LEVEL = logging.DEBUG
 CONFIGFILE = 'config.json'
-ROADMEET_ID = 'roadmeet_3.1'  # configuration versioning
+ROADMEET_ID = 'roadmeet-3.2'  # configuration versioning
 EXPORTPATH = 'export'
-_log = logging.getLogger('metarace.roadmeet')
+_log = logging.getLogger('roadmeet')
 _log.setLevel(logging.DEBUG)
 ROADRACE_TYPES = {
     'road': 'Road Race',
     'circuit': 'Circuit',
     'criterium': 'Criterium',
     'handicap': 'Handicap',
     'cross': 'Cyclocross',
     'irtt': 'Individual Time Trial',
     'trtt': 'Team Time Trial',
 }
-_DEFAULT_HANDLER = 'null'
 _HANDLERS = {
     'null': decoder,
     'thbc': thbc,
     'rrs': rrs,
     'rru': rru,
 }
 _CONFIG_SCHEMA = {
+    'mtype': {
+        'prompt': 'Meet Information',
+        'control': 'section',
+    },
     'etype': {
         'prompt': 'Type:',
         'control': 'choice',
         'attr': 'etype',
         'defer': True,
         'options': ROADRACE_TYPES,
+        'default': 'road',
     },
     'title': {
         'prompt': 'Title:',
         'hint': 'Meet title',
-        'attr': 'title_str'
+        'attr': 'title',
+        'default': '',
     },
     'subtitle': {
         'prompt': 'Subtitle:',
         'hint': 'Meet subtitle',
-        'attr': 'subtitle_str'
+        'attr': 'subtitle',
+        'default': '',
     },
     'host': {
         'prompt': 'Host:',
         'hint': 'Text for the meet host / sponsor line',
-        'attr': 'host_str'
+        'attr': 'host',
+        'default': '',
     },
     'document': {
         'prompt': 'Location:',
         'hint': 'Text for the meet location / document line',
-        'attr': 'document_str'
+        'attr': 'document',
+        'default': '',
     },
     'date': {
         'prompt': 'Date:',
         'hint': 'Date of the meet as human-readable text',
-        'attr': 'date_str'
+        'attr': 'date',
+        'default': '',
     },
-    'commissaire': {
+    'pcp': {
         'prompt': 'PCP:',
         'hint': 'Name of the president of the commissaires panel',
-        'attr': 'commissaire_str'
+        'attr': 'pcp',
+        'default': '',
     },
     'organiser': {
         'prompt': 'Organiser:',
         'hint': 'Name of the meet organiser',
-        'attr': 'organiser_str'
+        'attr': 'organiser',
+        'default': '',
     },
     'distance': {
         'prompt': 'Distance:',
         'hint': 'Advertised distance of the meet (if applicable)',
         'type': 'float',
         'control': 'short',
         'subtext': 'km',
         'attr': 'distance'
     },
     'diststr': {
         'prompt': 'Dist String:',
         'hint': 'Override distance string for crit/cat races',
-        'attr': 'diststr'
+        'attr': 'diststr',
+        'default': '',
     },
     'provisionalstart': {
         'prompt': 'Startlist:',
         'control': 'check',
         'type': 'bool',
         'subtext': 'Provisional?',
         'hint': 'Mark startlist reports as provisional',
-        'attr': 'provisionalstart'
+        'attr': 'provisionalstart',
+        'default': True,
     },
     'sectele': {
         'control': 'section',
-        'prompt': 'Telegraph'
+        'prompt': 'Telegraph',
     },
     'anntopic': {
         'prompt': 'Announce:',
         'hint': 'Base topic for announcer messages',
-        'attr': 'anntopic'
+        'attr': 'anntopic',
+    },
+    'announceresult': {
+        'prompt': 'Announce Result:',
+        'control': 'check',
+        'type': 'bool',
+        'subtext': 'Publish result to telegraph?',
+        'hint': 'Announce result to telegraph on export',
+        'attr': 'announceresult',
+        'default': False,
     },
     'timertopic': {
         'prompt': 'Timer:',
         'hint': 'Full topic for timer messages',
-        'attr': 'timertopic'
+        'attr': 'timertopic',
     },
-    'remote_enable': {
+    'remoteenable': {
         'prompt': 'Option:',
         'control': 'check',
         'type': 'bool',
         'subtext': 'Receive remote timer messages?',
         'hint': 'Receive remote timer messages from timer topic',
-        'attr': 'remote_enable'
+        'attr': 'remoteenable',
+        'default': False,
     },
     'sechw': {
         'control': 'section',
-        'prompt': 'Hardware'
+        'prompt': 'Hardware',
     },
     'timer': {
         'prompt': 'Transponders:',
         'hint': 'Transponder decoder spec TYPE:ADDR, eg: rrs:10.1.2.3',
         'defer': True,
-        'attr': 'timer_port'
+        'attr': 'timer',
     },
     'alttimer': {
         'prompt': 'Impulse:',
         'hint': 'Impulse timer port eg: /dev/ttyS0',
         'defer': True,
-        'attr': 'alttimer_port'
+        'attr': 'alttimer'
     },
     'secexp': {
         'control': 'section',
-        'prompt': 'Export'
+        'prompt': 'Export',
     },
     'mirrorcmd': {
         'prompt': 'Command:',
-        'hint': 'Export command',
-        'attr': 'mirrorcmd'
+        'hint': 'Command to run if export script is enabled',
+        'attr': 'mirrorcmd',
     },
     'mirrorpath': {
         'prompt': 'Path:',
         'hint': 'Result export path',
-        'attr': 'mirrorpath'
+        'attr': 'mirrorpath',
     },
     'mirrorfile': {
         'prompt': 'Filename:',
         'hint': 'Result export filename prefix',
-        'attr': 'mirrorfile'
+        'attr': 'mirrorfile',
     },
     'shortname': {
         'prompt': 'Short Name:',
         'hint': 'Short meet name on web export header',
-        'attr': 'shortname'
+        'attr': 'shortname',
     },
     'eventcode': {
         'prompt': 'Event Code:',
         'hint': 'Event code saved in reports',
-        'attr': 'eventcode'
+        'attr': 'eventcode',
     },
     'resfiles': {
         'prompt': 'Result Files:',
         'control': 'check',
         'type': 'bool',
         'subtext': 'Build results on export?',
         'hint': 'Build result files with export',
-        'attr': 'resfiles'
-    },
-    'announceresult': {
-        'prompt': 'Announce Result:',
-        'control': 'check',
-        'type': 'bool',
-        'subtext': 'Publish result to telegraph?',
-        'hint': 'Announce result to telegraph on export',
-        'attr': 'announceresult'
+        'attr': 'resfiles',
+        'default': True,
     },
     'lifexport': {
         'prompt': 'LIF Export:',
         'control': 'check',
         'type': 'bool',
         'subtext': 'Build LIF file on export?',
         'hint': 'Export LIF result file with results',
-        'attr': 'lifexport'
+        'attr': 'lifexport',
+        'default': False,
+    },
+    # the following are currently used for html export, but are likely
+    # to be removed in later versions
+    'linkbase': {
+        'attr': 'linkbase',
+        'control': 'none',
+        'default': '.',
+    },
+    'indexlink': {
+        'attr': 'indexlink',
+        'control': 'none',
+    },
+    'prevlink': {
+        'attr': 'prevlink',
+        'control': 'none',
+    },
+    'nextlink': {
+        'attr': 'nextlink',
+        'control': 'none',
     },
 }
 
 
-def mkdevice(portstr='', curdev=None):
+def mkdevice(portstr=None, curdev=None):
     """Return a decoder handle for the provided port specification."""
     # Note: If possible, returns the current device
+    if portstr is None:
+        portstr = ''
     ret = curdev
-    devtype = _DEFAULT_HANDLER
+    devtype = 'null'
     if metarace.sysconf.has_option('decoder', 'default'):
         devtype = metarace.sysconf.get('decoder', 'default')
         _log.debug('Default type set to %r from sysconf', devtype)
     (a, b, c) = portstr.partition(':')
     if b:
         a = a.lower()
         if a in _HANDLERS:
@@ -268,54 +305,140 @@
         """Return the <= 16 char shortname."""
         return self.shortname
 
     def cat_but_auto_clicked(self, but, entry, data=None):
         """Lookup cats and write them into the supplied entry."""
         entry.set_text(' '.join(self.rdb.listcats()))
 
+    def menu_race_decisions_activate_cb(self, menuitem, data=None):
+        """Edit decisions of the commissaires panel."""
+        if self.curevent is not None:
+            self.curevent.decisions = uiutil.decisions_dlg(
+                self.window, self.curevent.decisions)
+
     def menu_race_properties_activate_cb(self, menuitem, data=None):
         """Edit race specific properties."""
         if self.curevent is not None:
             _log.debug('Editing race properties')
             if self.curevent.edit_event_properties(self.window):
                 _log.info('Event re-start required')
-                self.menu_race_run_activate_cb()
+                self.event_reload()
 
     def menu_meet_properties_cb(self, menuitem, data=None):
         """Edit meet properties."""
-        res = uiutil.options_dlg(window=self.window,
-                                 title='Meet Properties',
-                                 schema=_CONFIG_SCHEMA,
-                                 obj=self)
+        metarace.sysconf.add_section('export', _EXPORT_SCHEMA)
+        metarace.sysconf.add_section('telegraph', _TG_SCHEMA)
+        metarace.sysconf.add_section('thbc', _THBC_SCHEMA)
+        metarace.sysconf.add_section('rru', _RRU_SCHEMA)
+        metarace.sysconf.add_section('rrs', _RRS_SCHEMA)
+        metarace.sysconf.add_section('timy', _TIMY_SCHEMA)
+        cfgres = uiutil.options_dlg(window=self.window,
+                                    title='Meet Properties',
+                                    sections={
+                                        'meet': {
+                                            'title': 'Meet',
+                                            'schema': _CONFIG_SCHEMA,
+                                            'object': self,
+                                        },
+                                        'export': {
+                                            'title': 'Export',
+                                            'schema': _EXPORT_SCHEMA,
+                                            'object': metarace.sysconf,
+                                        },
+                                        'telegraph': {
+                                            'title': 'Telegraph',
+                                            'schema': _TG_SCHEMA,
+                                            'object': metarace.sysconf,
+                                        },
+                                        'timy': {
+                                            'title': 'Timy',
+                                            'schema': _TIMY_SCHEMA,
+                                            'object': metarace.sysconf,
+                                        },
+                                        'thbc': {
+                                            'title': 'THBC',
+                                            'schema': _THBC_SCHEMA,
+                                            'object': metarace.sysconf,
+                                        },
+                                        'rru': {
+                                            'title': 'RR USB',
+                                            'schema': _RRU_SCHEMA,
+                                            'object': metarace.sysconf,
+                                        },
+                                        'rrs': {
+                                            'title': 'RR System',
+                                            'schema': _RRS_SCHEMA,
+                                            'object': metarace.sysconf,
+                                        },
+                                    })
+
+        # check for sysconf changes:
+        syschange = False
+        timychg = False
+        timerchg = False
+        tgchg = False
+        for sec in ('export', 'timy', 'rru', 'rrs', 'telegraph', 'thbc'):
+            for key in cfgres[sec]:
+                if cfgres[sec][key][0]:
+                    syschange = True
+                    if sec == 'telegraph':
+                        tgchg = True
+                    elif sec in ('rru', 'rrs', 'thbc'):
+                        timerchg = True
+                    elif sec == 'timy':
+                        timerchg = True
+                        timychg = True
+        if syschange:
+            _log.info('Saving config updates to meet folder')
+            with metarace.savefile(metarace.SYSCONF, perm=0o600) as f:
+                metarace.sysconf.write(f)
+
+        # reset telegraph connection if required
+        if tgchg:
+            _log.info('Re-start telegraph')
+            newannounce = telegraph()
+            newannounce.setcb(self._controlcb)
+            newannounce.start()
+            oldannounce = self.announce
+            self.announce = newannounce
+            oldannounce.exit()
+
+        # reset alttimer connection if required
+        if timychg:
+            _log.info('Re-start alt timer')
+            newtimy = timy()
+            newtimy.setcb(self._alttimercb)
+            newtimy.start()
+            oldtimy = self._alttimer
+            self._alttimer = newtimy
+            oldtimy.exit()
 
+        res = cfgres['meet']
         # handle a change in announce topic
-        if res['anntopic'][0]:
+        if res['anntopic'][0] or tgchg:
             otopic = res['anntopic'][1]
             if otopic:
                 self.announce.unsubscribe('/'.join((otopic, 'control', '#')))
             if self.anntopic:
                 self.announce.subscribe('/'.join(
                     (self.anntopic, 'control', '#')))
 
         # handle change in timer topic
-        if res['timertopic'][0]:
+        if res['timertopic'][0] or tgchg:
             otopic = res['timertopic'][1]
             if otopic:
                 self.announce.unsubscribe(otopic)
 
         # reset remote option
-        if res['timertopic'][0] or res['remote_enable'][0]:
+        if res['timertopic'][0] or res['remoteenable'][0] or tgchg:
             self.remote_reset()
 
-        # reset timer ports
-        if res['timer'][0] or res['alttimer'][0]:
-            self.menu_timing_reconnect_activate_cb(None)
-
         # if type has changed, backup config and reload
         if res['etype'][0]:
+            timerchg = True
             reopen = False
             if self.curevent is not None:
                 reopen = True
                 conf = self.curevent.configfile
                 self.close_event()
                 backup = conf + '.bak'
                 _log.warning('Event type change, backing up old config to %r',
@@ -323,50 +446,54 @@
                 try:
                     if os.path.exists(backup):
                         os.unlink(backup)
                     os.link(conf, backup)
                 except Exception as e:
                     _log.warning('%s saving event backup: %s',
                                  e.__class__.__name__, e)
-            eh = self.edb.getfirst()
-            eh['type'] = self.etype
             if reopen:
-                self.open_event(eh)
+                self.open_event()
+
+        # reset timer ports
+        if res['timer'][0] or res['alttimer'][0] or timerchg:
+            self.menu_timing_reconnect_activate_cb(None)
+
         self.set_title()
 
-    def print_report(self, sections=[], provisional=False):
-        """Print the pre-formatted sections in a standard report."""
-        rep = report.report()
-        rep.provisional = provisional
-        rep.strings['title'] = self.title_str
-        rep.strings['subtitle'] = self.subtitle_str
-        rep.strings['host'] = self.host_str
-        rep.strings['docstr'] = self.document_str
-        rep.strings['datestr'] = strops.promptstr('Date:', self.date_str)
-        rep.strings['commstr'] = strops.promptstr('Chief Commissaire:',
-                                                  self.commissaire_str)
-        rep.strings['orgstr'] = strops.promptstr('Organiser:',
-                                                 self.organiser_str)
+    def report_strings(self, rep):
+        """Copy meet information into the supplied report."""
+        rep.strings['title'] = self.title
+        rep.strings['subtitle'] = self.subtitle
+        rep.strings['host'] = self.host
+        rep.strings['docstr'] = self.document
+        rep.strings['datestr'] = strops.promptstr('Date:', self.date)
+        rep.strings['commstr'] = strops.promptstr('PCP:', self.pcp)
+        rep.strings['orgstr'] = strops.promptstr('Organiser:', self.organiser)
         if self.distance:
             rep.strings['diststr'] = strops.promptstr(
                 'Distance:',
                 str(self.distance) + '\u2006km')
         else:
             rep.strings['diststr'] = self.diststr
-
         if self.eventcode:
             rep.eventid = self.eventcode
         if self.prevlink:
             rep.prevlink = self.prevlink
         if self.nextlink:
             rep.nextlink = self.nextlink
         if self.indexlink:
             rep.indexlink = self.indexlink
         if self.shortname:
             rep.shortname = self.shortname
+
+    def print_report(self, sections=[], provisional=False):
+        """Print the pre-formatted sections in a standard report."""
+        rep = report.report()
+        rep.provisional = provisional
+        self.report_strings(rep)
         for sec in sections:
             rep.add_section(sec)
 
         print_op = Gtk.PrintOperation.new()
         print_op.set_allow_async(True)
         print_op.set_print_settings(self.printprefs)
         print_op.set_default_page_setup(self.pageset)
@@ -400,33 +527,20 @@
         rep.set_context(context.get_cairo_context())
         rep.draw_page(page_nr)
 
     def menu_meet_quit_cb(self, menuitem, data=None):
         """Quit the application."""
         self.window.close()
 
-    ## Race Menu Callbacks
-    def menu_race_run_activate_cb(self, menuitem=None, data=None):
+    def event_reload(self):
         """Open the event handler."""
-        eh = self.edb.getfirst()
-        if eh is not None:
-            self.open_event(eh)
-            self.set_title()
+        self.open_event()
+        self.set_title()
         return False
 
-    def menu_race_close_activate_cb(self, menuitem, data=None):
-        """Close callback - disabled in roadrace."""
-        self.close_event()
-
-    def menu_race_abort_activate_cb(self, menuitem, data=None):
-        """Close the currently open event without saving."""
-        if self.curevent is not None:
-            self.curevent.readonly = True
-        self.close_event()
-
     def menu_race_armstart_activate_cb(self, menuitem, data=None):
         """Default armstart handler."""
         _log.info('Arm Start')
         try:
             self.curevent.armstart()
         except Exception as e:
             _log.error('Arm start %s: %s', e.__class__.__name__, e)
@@ -451,55 +565,45 @@
         """Default finished handler."""
         _log.info('Finished')
         try:
             self.curevent.set_finished()
         except Exception as e:
             _log.error('Set finished %s: %s', e.__class__.__name__, e)
 
-    def open_event(self, eventhdl=None):
+    def open_event(self):
         """Open provided event handle."""
-        if eventhdl is not None:
-            self.close_event()
-            if self.etype not in ROADRACE_TYPES:
-                _log.warning('Unknown event type %r', self.etype)
-            if self.etype == 'irtt':
-                self.curevent = irtt(self, eventhdl, True)
-            elif self.etype == 'trtt':
-                self.curevent = trtt(self, eventhdl, True)
-            else:
-                self.curevent = rms(self, eventhdl, True)
-
-            self.curevent.loadconfig()
-            self.race_box.add(self.curevent.frame)
-
-            # re-populate the rider command model.
-            cmdo = self.curevent.get_ridercmdorder()
-            cmds = self.curevent.get_ridercmds()
-            if cmds is not None:
-                self.action_model.clear()
-                for cmd in cmdo:
-                    self.action_model.append([cmd, cmds[cmd]])
-                self.action_combo.set_active(0)
-
-            self.menu_race_close.set_sensitive(True)
-            self.menu_race_abort.set_sensitive(True)
-            starters = eventhdl['star']
-            if starters is not None and starters != '':
-                self.curevent.race_ctrl('add', starters)
-                eventhdl['star'] = ''  # and clear
-            self.curevent.show()
+        self.close_event()
+        if self.etype not in ROADRACE_TYPES:
+            _log.warning('Unknown event type %r', self.etype)
+        if self.etype == 'irtt':
+            self.curevent = irtt(self, self.etype, True)
+        elif self.etype == 'trtt':
+            self.curevent = trtt(self, self.etype, True)
+        else:
+            self.curevent = rms(self, self.etype, True)
+
+        self.curevent.loadconfig()
+        self.race_box.add(self.curevent.frame)
+
+        # re-populate the rider command model.
+        cmdo = self.curevent.get_ridercmdorder()
+        cmds = self.curevent.get_ridercmds()
+        if cmds is not None:
+            self.action_model.clear()
+            for cmd in cmdo:
+                self.action_model.append([cmd, cmds[cmd]])
+            self.action_combo.set_active(0)
+        self.curevent.show()
 
     def close_event(self):
         """Close the currently opened race."""
         if self.curevent is not None:
             if self.curevent.frame in self.race_box.get_children():
                 self.race_box.remove(self.curevent.frame)
             self.curevent.destroy()
-            self.menu_race_close.set_sensitive(False)
-            self.menu_race_abort.set_sensitive(False)
             self.curevent = None
             self.stat_but.update('idle', 'Closed')
             self.stat_but.set_sensitive(False)
 
     ## Reports menu callbacks.
     def menu_reports_startlist_activate_cb(self, menuitem, data=None):
         """Generate a startlist."""
@@ -563,36 +667,33 @@
                                      parent=self.window,
                                      path='.')
         if sfile is not None:
             try:
                 self.rdb.clear(notify=False)
                 count = self.rdb.load(sfile)
                 _log.info('Loaded %d entries from %r', count, sfile)
-                #self.menu_race_run_activate_cb()
             except Exception as e:
                 _log.error('%s loading riders: %s', e.__class__.__name__, e)
         else:
             _log.debug('Import riders cancelled')
 
     def menu_data_clear_activate_cb(self, menuitem, data=None):
         """Clear rider db."""
         self.rdb.clear()
         _log.info('Cleared rider db')
-        #self.menu_race_run_activate_cb()
 
     def menu_import_riders_activate_cb(self, menuitem, data=None):
         """Add riders to database."""
         sfile = uiutil.chooseCsvFile(title='Select rider file to import',
                                      parent=self.window,
                                      path='.')
         if sfile is not None:
             try:
                 count = self.rdb.load(sfile, overwrite=True)
                 _log.info('Imported %d rider entries from %r', count, sfile)
-                #self.menu_race_run_activate_cb()
             except Exception as e:
                 _log.error('%s importing riders: %s', e.__class__.__name__, e)
         else:
             _log.debug('Import riders cancelled')
 
     def menu_import_chipfile_activate_cb(self, menuitem, data=None):
         """Import a transponder chipfile."""
@@ -622,17 +723,16 @@
     def import_starters(self, sfile):
         """Import starters from the nominated csvfile"""
         if os.path.isfile(sfile):
             count = 0
             with open(sfile, encoding='utf-8', errors='replace') as f:
                 cr = csv.reader(f)
                 for r in cr:
-                    if len(r) > 1 and r[1].isalnum() and r[1].lower() not in [
-                            'no', 'no.'
-                    ]:
+                    if len(r) > 1 and r[1].isalnum() and r[1].lower() not in (
+                            'no', 'no.'):
                         bib = r[1].strip().lower()
                         series = ''
                         if len(r) > 2:
                             series = r[2].strip()
                         self.curevent.addrider(bib, series)
                         start = tod.mktod(r[0])
                         if start is not None:
@@ -733,15 +833,15 @@
             _log.info('Export startlist cancelled')
 
     def export_result_maker(self):
         if self.mirrorfile:
             filebase = self.mirrorfile
         else:
             filebase = '.'
-        if filebase in ['', '.']:
+        if filebase in ('', '.'):
             filebase = ''
             if self.resfiles:
                 _log.warn('Using default filenames for export')
         else:
             pass
 
         fnv = []
@@ -749,45 +849,24 @@
             fnv.append(filebase)
         fnv.append('startlist')
         sfile = '_'.join(fnv)
         fnv[-1] = 'result'
         ffile = '_'.join(fnv)
 
         # Write out a startlist unless event finished
-        if self.resfiles and self.curevent.timerstat not in ['finished']:
+        if self.resfiles and self.curevent.timerstat != 'finished':
             filename = sfile
             rep = report.report()
-            rep.strings['title'] = self.title_str
-            rep.strings['subtitle'] = self.subtitle_str
-            rep.strings['host'] = self.host_str
-            rep.strings['docstr'] = self.document_str
-            rep.strings['datestr'] = strops.promptstr('Date:', self.date_str)
-            rep.strings['commstr'] = strops.promptstr('Chief Commissaire:',
-                                                      self.commissaire_str)
-            rep.strings['orgstr'] = strops.promptstr('Organiser:',
-                                                     self.organiser_str)
-            if self.distance:
-                rep.strings['diststr'] = strops.promptstr(
-                    'Distance:',
-                    str(self.distance) + '\u2006km')
-            else:
-                rep.strings['diststr'] = self.diststr
+            self.report_strings(rep)
             if self.provisionalstart:
                 rep.set_provisional(True)
-            rep.indexlink = 'index'
-            if self.eventcode:
-                rep.eventid = self.eventcode
             if self.prevlink:
                 rep.prevlink = '_'.join((self.prevlink, 'startlist'))
             if self.nextlink:
                 rep.nextlink = '_'.join((self.nextlink, 'startlist'))
-            if self.indexlink:
-                rep.indexlink = self.indexlink
-            if self.shortname:
-                rep.shortname = self.shortname
             rep.resultlink = ffile
             for sec in self.curevent.startlist_report():
                 rep.add_section(sec)
 
             lb = os.path.join(self.linkbase, filename)
             lt = ['pdf', 'xls']
             rep.canonical = '.'.join([lb, 'json'])
@@ -802,51 +881,29 @@
                 rep.output_json(f)
             ofile = os.path.join(self.exportpath, filename + '.html')
             with metarace.savefile(ofile) as f:
                 rep.output_html(f, linkbase=lb, linktypes=lt)
 
         # Then export a result
         rep = report.report()
-        rep.strings['title'] = self.title_str
-        rep.strings['subtitle'] = self.subtitle_str
-        rep.strings['host'] = self.host_str
-        rep.strings['docstr'] = self.document_str
-        rep.strings['datestr'] = strops.promptstr('Date:', self.date_str)
-        rep.strings['commstr'] = strops.promptstr('Chief Commissaire:',
-                                                  self.commissaire_str)
-        rep.strings['orgstr'] = strops.promptstr('Organiser:',
-                                                 self.organiser_str)
-        if self.distance:
-            rep.strings['diststr'] = strops.promptstr(
-                'Distance:',
-                str(self.distance) + '\u2006km')
-        else:
-            rep.strings['diststr'] = self.diststr
+        self.report_strings(rep)
 
-        # Set provisional status	# TODO: other tests for prov flag?
+        # Set provisional status
         if self.curevent.timerstat != 'finished':
             rep.set_provisional(True)
         else:
-            rep.reportstatus = 'final'  # TODO: write in other phases
+            rep.reportstatus = 'final'
         for sec in self.curevent.result_report():
             rep.add_section(sec)
-
         filename = ffile
-        rep.indexlink = 'index'
-        if self.eventcode:
-            rep.eventid = self.eventcode
+        rep.startlink = sfile
         if self.prevlink:
             rep.prevlink = '_'.join((self.prevlink, 'result'))
         if self.nextlink:
             rep.nextlink = '_'.join((self.nextlink, 'result'))
-        if self.indexlink:
-            rep.indexlink = self.indexlink
-        if self.shortname:
-            rep.shortname = self.shortname
-        rep.startlink = sfile
         lb = os.path.join(self.linkbase, filename)
         lt = ['pdf', 'xls']
         rep.canonical = '.'.join([lb, 'json'])
 
         # announce to telegraph if enabled
         if self.announceresult:
             self.obj_announce(command='result', obj=rep.serialise())
@@ -879,31 +936,26 @@
                     cw = csv.writer(f, quoting=csv.QUOTE_MINIMAL)
                     for r in lifdat:
                         cw.writerow(r)
         if self.resfiles or self.announceresult:
             self.export_result_maker()
         GLib.idle_add(self.mirror_start)
 
-    ## Directory utilities
-    def event_configfile(self, evno):
-        """Return a config filename for the given event no."""
-        return 'event_{}.json'.format(str(evno))
-
     ## Timing menu callbacks
     def menu_timing_status_cb(self, menuitem, data=None):
-        if self.timer_port:
-            if self.timer.connected():
+        if self.timer:
+            if self._timer.connected():
                 _log.info('Request timer status')
-                self.timer.status()
+                self._timer.status()
             else:
                 _log.info('Decoder disconnected')
         else:
             _log.info('No decoder configured')
         # always call into alt timer
-        self.alttimer.status()
+        self._alttimer.status()
 
     def menu_timing_start_activate_cb(self, menuitem, data=None):
         """Manually set race elapsed time via trigger."""
         if self.curevent is None:
             _log.info('No event open to set elapsed time on')
         else:
             self.curevent.elapsed_dlg()
@@ -923,51 +975,74 @@
             nte.set_text((ft - st).timestr())
 
     def menu_timing_clear_activate_cb(self, menuitem, data=None):
         """Start a new timing session in attached timers"""
         # Note: clear will perform reset, stop_session, clear,
         # sync, and start_session in whatever order is appropriate
         # for the decoder type
-        self.timer.clear()
-        self.alttimer.clrmem()
+        self._timer.clear()
+        self._alttimer.clrmem()
+
+    def set_altchannels(self):
+        self._alttimer.armlock()  # lock the arm to capture all hits
+        self._alttimer.arm(0)  # start line
+        self._alttimer.arm(1)  # finish line (primary)
+        self._alttimer.dearm(6)
+        self._alttimer.dearm(7)
+        self._alttimer.dearm(8)
+        if self.etype == 'irtt':
+            self._alttimer.write('DTS05.00')
+            self._alttimer.write('DTF00.01')
+            self._alttimer.arm(2)  # finish line (photo cell)
+            self._alttimer.arm(3)  # finish line (plunger)
+            self._alttimer.arm(4)  # start line (backup)
+            self._alttimer.arm(5)  # spare
+        else:
+            self._alttimer.write('DTS00.01')
+            if self.etype == 'trtt':
+                self._alttimer.write('DTF00.01')
+            else:
+                # assume 1 second gaps at finish for road types
+                self._alttimer.write('DTF01.00')
+            self._alttimer.dearm(2)
+            self._alttimer.dearm(3)
+            self._alttimer.dearm(4)
+            self._alttimer.dearm(5)
 
     def menu_timing_reconnect_activate_cb(self, menuitem, data=None):
         """Drop current timer connection and re-connect"""
-        self.set_timer(self.timer_port, force=True)
-        self.alttimer.setport(self.alttimer_port)
-        self.alttimer.sane()
-        if self.etype == 'irtt':
-            self.alttimer.write('DTS05.00')
-            self.alttimer.write('DTF00.01')
-        else:
-            # assume 1 second gaps at finish
-            self.alttimer.write('DTF01.00')
+        self.set_timer(self.timer, force=True)
+        self._alttimer.setport(self.alttimer)
+        self._alttimer.sane()
+        self.set_altchannels()
         _log.info('Re-connect/re-start attached timers')
 
     def restart_decoder(self, data=None):
         """Request re-start of decoder."""
-        self.timer.start_session()
+        self._timer.start_session()
         return None
 
     def menu_timing_configure_activate_cb(self, menuitem, data=None):
         """Attempt to re-configure the attached decoder from saved config."""
-        if self.timer.__class__.__name__ == 'thbc':
-            if not timer.connected():
+        if self._timer.__class__.__name__ == 'thbc':
+            if not self._timer.connected():
                 _log.info('Timer not connected, config not possible')
                 return False
             if not uiutil.questiondlg(
-                    self.window, 'Re-configure THBC Decoder Settings?',
-                    'Note: Passings will not be captured while decoder is updating.'
-            ):
+                    window=self.window,
+                    question='Re-configure THBC Decoder IP Settings?',
+                    subtext=
+                    'Note: Passings will not be captured while decoder is updating.',
+                    title='Update Decoder IP?'):
                 _log.debug('Config aborted')
                 return False
-            self.timer.stop_session()
-            self.timer.sane()
+            self._timer.stop_session()
+            self._timer.sane()
             GLib.timeout_add_seconds(60, self.restart_decoder)
-            self.timer.ipconfig()
+            self._timer.ipconfig()
         else:
             _log.info('Decoder config not available')
         return None
 
     ## Help menu callbacks
     def menu_help_about_cb(self, menuitem, data=None):
         """Display metarace about dialog."""
@@ -1015,33 +1090,33 @@
                     self.curevent.timeout()
 
                 # update the menu status button
                 nt = tod.now().meridiem()
                 if self.rfuact:
                     self.rfustat.update('activity', nt)
                 else:
-                    if self.timer_port:
-                        if self.timer.connected():
+                    if self.timer:
+                        if self._timer.connected():
                             self.rfustat.update('ok', nt)
                         else:
                             self.rfustat.update('error', nt)
                     else:
                         self.rfustat.update('idle', nt)
                 self.rfuact = False
 
                 # attempt to heal a broken link
-                if self.timer_port:
-                    if self.timer.connected():
+                if self.timer:
+                    if self._timer.connected():
                         self.rfufail = 0
                     else:
                         self.rfufail += 1
-                        if self.rfufail > 10:
+                        if self.rfufail > 20:
                             self.rfufail = 0
-                            eport = self.timer_port.split(':', 1)[-1]
-                            self.timer.setport(eport)
+                            eport = self.timer.split(':', 1)[-1]
+                            self._timer.setport(eport)
                 else:
                     self.rfufail = 0
             else:
                 return False
         except Exception as e:
             _log.critical('%s in meet timeout: %s', e.__class__.__name__, e)
         return True
@@ -1049,18 +1124,18 @@
     ## Window methods
     def set_title(self, extra=''):
         """Update window title from meet properties."""
         tv = []
         if self.etype in ROADRACE_TYPES:
             tv.append(ROADRACE_TYPES[self.etype] + ':')
 
-        title = self.title_str.strip()
+        title = self.title.strip()
         if title:
             tv.append(title)
-        subtitle = self.subtitle_str.strip()
+        subtitle = self.subtitle.strip()
         if subtitle:
             tv.append(subtitle)
         self.window.set_title(' '.join(tv))
         if self.curevent is not None:
             self.curevent.set_titlestr(subtitle)
 
     def meet_destroy_cb(self, window, msg=''):
@@ -1087,229 +1162,121 @@
     def key_event(self, widget, event):
         """Collect key events on main window and send to race."""
         if event.type == Gdk.EventType.KEY_PRESS:
             key = Gdk.keyval_name(event.keyval) or 'None'
             if event.state & Gdk.ModifierType.CONTROL_MASK:
                 key = key.lower()
                 t = tod.now(chan='MAN', refid=str(key))
-                if key in ['0', '1']:
+                if key in ('0', '1'):
                     # trigger
                     t.refid = ''
                     t.chan = strops.id2chan(strops.chan2id(key))
                     self._alttimercb(t)
                     return True
-                elif key in ['2', '3', '4', '5', '6', '7', '8', '9']:
+                elif key in ('2', '3', '4', '5', '6', '7', '8', '9'):
                     # passing
                     self._timercb(t)
                     return True
             if self.curevent is not None:
                 return self.curevent.key_event(widget, event)
         return False
 
     def shutdown(self, msg=''):
         """Shutdown worker threads and close application."""
         self.started = False
         self.announce.exit(msg)
-        self.timer.exit(msg)
-        self.alttimer.exit(msg)
+        self._timer.exit(msg)
+        self._alttimer.exit(msg)
         _log.info('Waiting for workers')
         if self.mirror is not None:
             _log.debug('Result export')
             self.mirror.join()
             self.mirror = None
         _log.debug('Telegraph/announce')
         self.announce.join()
 
     def start(self):
         """Start the timer and rfu threads."""
         if not self.started:
             _log.debug('Meet startup')
             self.announce.start()
-            self.timer.start()
-            self.alttimer.start()
+            self._timer.start()
+            self._alttimer.start()
             self.started = True
 
     ## Roadmeet functions
     def saveconfig(self):
         """Save current meet data to disk."""
         if self.curevent is not None and self.curevent.winopen:
             self.curevent.saveconfig()
         cw = jsonconfig.config()
-        cw.add_section('roadmeet')
+        cw.add_section('roadmeet', _CONFIG_SCHEMA)
+        cw.import_section('roadmeet', self)
         cw.set('roadmeet', 'id', ROADMEET_ID)
-        cw.set('roadmeet', 'anntopic', self.anntopic)
-        cw.set('roadmeet', 'timertopic', self.timertopic)
-        cw.set('roadmeet', 'remote_enable', self.remote_enable)
-        cw.set('roadmeet', 'timer', self.timer_port)
-        cw.set('roadmeet', 'alttimer', self.alttimer_port)
-        cw.set('roadmeet', 'shortname', self.shortname)
-        cw.set('roadmeet', 'linkbase', self.linkbase)
-        cw.set('roadmeet', 'indexlink', self.indexlink)
-        cw.set('roadmeet', 'nextlink', self.nextlink)
-        cw.set('roadmeet', 'prevlink', self.prevlink)
-        cw.set('roadmeet', 'title', self.title_str)
-        cw.set('roadmeet', 'host', self.host_str)
-        cw.set('roadmeet', 'subtitle', self.subtitle_str)
-        cw.set('roadmeet', 'document', self.document_str)
-        cw.set('roadmeet', 'date', self.date_str)
-        cw.set('roadmeet', 'organiser', self.organiser_str)
-        cw.set('roadmeet', 'commissaire', self.commissaire_str)
-        cw.set('roadmeet', 'lifexport', self.lifexport)
-        cw.set('roadmeet', 'resfiles', self.resfiles)
-        cw.set('roadmeet', 'announceresult', self.announceresult)
-        cw.set('roadmeet', 'provisionalstart', self.provisionalstart)
-        cw.set('roadmeet', 'distance', self.distance)
-        cw.set('roadmeet', 'diststr', self.diststr)
-        cw.set('roadmeet', 'mirrorpath', self.mirrorpath)
-        cw.set('roadmeet', 'mirrorcmd', self.mirrorcmd)
-        cw.set('roadmeet', 'mirrorfile', self.mirrorfile)
-        cw.set('roadmeet', 'eventcode', self.eventcode)
-
         with metarace.savefile(CONFIGFILE) as f:
             cw.write(f)
         self.rdb.save('riders.csv')
-        self.edb.save('events.csv')
         _log.info('Meet configuration saved')
 
     def set_timer(self, newdevice='', force=False):
         """Re-set the main timer device and connect callback."""
-        if newdevice != self.timer_port or force:
-            self.timer = mkdevice(newdevice, self.timer)
-            self.timer_port = newdevice
+        if newdevice != self.timer or force:
+            self._timer = mkdevice(newdevice, self._timer)
+            self.timer = newdevice
         else:
             _log.debug('set_timer - No change required')
-        self.timer.setcb(self._timercb)
+        self._timer.setcb(self._timercb)
 
     def loadconfig(self):
         """Load meet config from disk."""
-        cr = jsonconfig.config({
-            'roadmeet': {
-                'shortname': None,
-                'title': '',
-                'host': '',
-                'subtitle': '',
-                'document': '',
-                'date': '',
-                'organiser': '',
-                'commissaire': '',
-                'distance': None,
-                'diststr': '',
-                'timer': '',
-                'alttimer': '',
-                'anntopic': None,
-                'timertopic': None,
-                'remote_enable': False,
-                'linkbase': '.',
-                'indexlink': None,
-                'nextlink': None,
-                'prevlink': None,
-                'lifexport': False,
-                'resfiles': True,
-                'announceresult': True,
-                'provisionalstart': False,
-                'mirrorpath': None,
-                'mirrorcmd': None,
-                'mirrorfile': None,
-                'eventcode': '',
-                'id': ''
-            }
-        })
-        cr.add_section('roadmeet')
+        cr = jsonconfig.config()
+        cr.add_section('roadmeet', _CONFIG_SCHEMA)
 
         # re-set main log file
         _log.debug('Adding meet logfile handler %r', LOGFILE)
         rootlogger = logging.getLogger()
         if self.loghandler is not None:
             rootlogger.removeHandler(self.loghandler)
             self.loghandler.close()
             self.loghandler = None
         self.loghandler = logging.FileHandler(LOGFILE)
         self.loghandler.setLevel(LOGFILE_LEVEL)
         self.loghandler.setFormatter(logging.Formatter(metarace.LOGFILEFORMAT))
         rootlogger.addHandler(self.loghandler)
 
         cr.merge(metarace.sysconf, 'roadmeet')
-        _log.debug('Load system meet defaults')
         cr.load(CONFIGFILE)
+        cr.export_section('roadmeet', self)
 
-        # set timer port (decoder)
-        self.set_timer(cr.get('roadmeet', 'timer'))
-
-        # set alt timer port (timy)
-        nport = cr.get('roadmeet', 'alttimer')
-        if nport != self.alttimer_port:
-            self.alttimer_port = nport
-            self.alttimer.setport(nport)
-            self.alttimer.sane()
-
-        # set the default announce topic and subscribe to control topic
-        self.anntopic = cr.get('roadmeet', 'anntopic')
+        # update hardware ports and telegraph setting
+        self.set_timer(self.timer, force=True)
+        if self.alttimer:
+            self._alttimer.setport(self.alttimer)
+            self._alttimer.sane()
+            self.set_altchannels()
         if self.anntopic:
             self.announce.subscribe('/'.join((self.anntopic, 'control', '#')))
-
-        # fetch the remote timer topic and update remote control
-        self.timertopic = cr.get('roadmeet', 'timertopic')
-        self.remote_enable = cr.get_bool('roadmeet', 'remote_enable')
         self.remote_reset()
 
-        # set meet meta, and then copy into text entries
-        self.shortname = cr.get('roadmeet', 'shortname')
-        self.title_str = cr.get('roadmeet', 'title')
-        self.host_str = cr.get('roadmeet', 'host')
-        self.subtitle_str = cr.get('roadmeet', 'subtitle')
-        self.document_str = cr.get('roadmeet', 'document')
-        self.date_str = cr.get('roadmeet', 'date')
-        self.organiser_str = cr.get('roadmeet', 'organiser')
-        self.commissaire_str = cr.get('roadmeet', 'commissaire')
-        self.distance = cr.get_float('roadmeet', 'distance')
-        self.diststr = cr.get('roadmeet', 'diststr')
-        self.linkbase = cr.get('roadmeet', 'linkbase')
-        self.indexlink = cr.get('roadmeet', 'indexlink')
-        self.prevlink = cr.get('roadmeet', 'prevlink')
-        self.nextlink = cr.get('roadmeet', 'nextlink')
-        self.mirrorpath = cr.get('roadmeet', 'mirrorpath')
-        self.mirrorcmd = cr.get('roadmeet', 'mirrorcmd')
-        self.mirrorfile = cr.get('roadmeet', 'mirrorfile')
-        self.eventcode = cr.get('roadmeet', 'eventcode')
-        self.lifexport = cr.get_bool('roadmeet', 'lifexport')
-        self.resfiles = cr.get_bool('roadmeet', 'resfiles')
-        self.announceresult = cr.get_bool('roadmeet', 'announceresult')
-        self.provisionalstart = cr.get_bool('roadmeet', 'provisionalstart')
-
-        # Re-Initialise rider and event databases
+        # Re-Initialise rider database
         self.rdb.clear(notify=False)
         _log.debug('meet load riders from riders.csv')
         self.rdb.load('riders.csv')
-        self.edb.clear()
-        self.edb.load('events.csv')
-        event = self.edb.getfirst()
-        if event is None:  # add a new event of the right type
-            event = self.edb.add_empty(evno='0')
-            event['type'] = self.etype
-        else:
-            self.etype = event['type']
-            _log.debug('Existing event in db: %r', self.etype)
-        self.open_event(event)  # always open on load if posible
-        self.set_title()
 
-        # alt timer config post event load
-        if self.etype == 'irtt':
-            self.alttimer.write('DTS05.00')
-            self.alttimer.write('DTF00.01')
-        else:
-            # assume 1 second gaps at finish
-            self.alttimer.write('DTF01.00')
+        # Open the event
+        self.open_event()
+        self.set_title()
 
         # make sure export path exists
         if not os.path.exists(self.exportpath):
             os.mkdir(self.exportpath)
             _log.info('Created export path: %r', self.exportpath)
 
         # check and warn of config mismatch
-        cid = cr.get('roadmeet', 'id')
+        cid = cr.get_value('roadmeet', 'id')
         if cid != ROADMEET_ID:
             _log.warning('Meet config mismatch: %r != %r', cid, ROADMEET_ID)
 
     def get_distance(self):
         """Return race distance in km."""
         return self.distance
 
@@ -1329,19 +1296,19 @@
     def rider_announce(self, rvec, command='rider'):
         """Issue a serialised rider vector to announcer."""
         # Deprecated UNT-style list
         self.cmd_announce(command, '\x1f'.join(rvec))
 
     def timer_announce(self, evt, timer=None, source=''):
         """Send message into announce for remote control."""
-        if not self.remote_enable and self.timertopic is not None:
+        if not self.remoteenable and self.timertopic is not None:
             if timer is None:
-                timer = self.timer
+                timer = self._timer
             prec = 4
-            if timer is self.timer:
+            if timer is self._timer:
                 prec = 3  # transponders have reduced precision
             elif 'M' in evt.chan:
                 prec = 3
             if evt.source is not None:
                 source = evt.source
             tvec = (evt.index, source, evt.chan, evt.refid, evt.rawtime(prec),
                     '')
@@ -1349,25 +1316,25 @@
         self.rfustat.update('activity')
         self.rfuact = True
         return False
 
     def mirror_start(self):
         """Create a new mirror thread unless already in progress."""
         if self.mirrorpath and self.mirror is None:
-            self.mirror = export.mirror(localpath=os.path.join('export', ''),
-                                        remotepath=self.mirrorpath,
-                                        mirrorcmd=self.mirrorcmd)
+            self.mirror = mirror(localpath=os.path.join(EXPORTPATH, ''),
+                                 remotepath=self.mirrorpath,
+                                 mirrorcmd=self.mirrorcmd)
             self.mirror.start()
         return False  # for idle_add
 
     def remote_reset(self):
         """Reset remote input of timer messages."""
         _log.debug('Remote control reset')
         if self.timertopic is not None:
-            if self.remote_enable:
+            if self.remoteenable:
                 _log.debug('Listening for remote timer at %r', self.timertopic)
                 self.announce.subscribe(self.timertopic)
             else:
                 _log.debug('Remote timer disabled')
                 self.announce.unsubscribe(self.timertopic)
         else:
             _log.debug('Remote timer topic not cofigured')
@@ -1399,15 +1366,15 @@
                 _log.warning('Error reading timer msg %r: %s', msg, e)
         else:
             _log.debug('Invalid remote timer message: %r', tv)
 
     def remote_command(self, topic, msg):
         """Handle a remote control message."""
         if topic == self.timertopic:
-            if self.remote_enable:
+            if self.remoteenable:
                 self.remote_timer(msg)
         else:
             _log.debug('Unsupported remote command %r:%r', topic, msg)
         return False
 
     def getrefid(self, refid):
         """Return a handle to the rider with the suplied refid or None."""
@@ -1505,34 +1472,33 @@
             _log.debug('Re-built refid tagmap: %d entries', len(self._tagmap))
         if self.curevent is not None:
             self.curevent.ridercb(rider)
 
     def _timercb(self, evt, data=None):
         if self.timercb is not None:
             GLib.idle_add(self.timercb, evt, priority=GLib.PRIORITY_HIGH)
-        GLib.idle_add(self.timer_announce, evt, self.timer, 'rfid')
+        GLib.idle_add(self.timer_announce, evt, self._timer, 'rfid')
 
     def _alttimercb(self, evt, data=None):
         if self.alttimercb is not None:
             GLib.idle_add(self.alttimercb, evt, priority=GLib.PRIORITY_HIGH)
-        GLib.idle_add(self.timer_announce, evt, self.alttimer, 'timy')
+        GLib.idle_add(self.timer_announce, evt, self._alttimer, 'timy')
 
     def _controlcb(self, topic=None, message=None):
         GLib.idle_add(self.remote_command, topic, message)
 
     def _rcb(self, rider):
         GLib.idle_add(self.ridercb, rider)
 
     def _catcol_cb(self, cell, path, new_text, col):
         """Callback for editing category info"""
         new_text = new_text.strip()
         bib = self._clm[path][0]
         self._clm[path][col] = new_text
         r = self.rdb.get_rider(bib, 'cat')
-        # TODO: fix the disconnect here between col and field
         if r is not None:
             if col == 1:
                 if new_text != r['title']:
                     r['title'] = new_text
             elif col == 2:
                 if new_text != r['subtitle']:
                     r['subtitle'] = new_text
@@ -1558,15 +1524,14 @@
     def _editcol_cb(self, cell, path, new_text, col):
         """Callback for editing a transponder ID"""
         new_text = new_text.strip()
         bib = self._rlm[path][0]
         series = self._rlm[path][1]
         self._rlm[path][col] = new_text
         r = self.rdb.get_rider(bib, series)
-        # TODO: fix the disconnect here between col and field
         if r is not None:
             if col == 3:
                 if new_text != r['org']:
                     r['org'] = new_text
             elif col == 4:
                 if new_text.upper() != r['cat']:
                     r['cat'] = new_text.upper()
@@ -1603,19 +1568,24 @@
             nser = 'cat'
         dbr = riderdb.rider(series=nser)
         schema = dbr.get_schema()
         rtype = schema['rtype']['prompt']
         short = 'Create New %s' % (rtype)
         res = uiutil.options_dlg(window=self.window,
                                  title=short,
-                                 schema=schema,
-                                 obj=dbr)
+                                 sections={
+                                     'rdb': {
+                                         'title': 'Rider',
+                                         'schema': schema,
+                                         'object': dbr,
+                                     },
+                                 })
         chg = False
-        for k in res:
-            if res[k][0]:
+        for k in res['rdb']:
+            if res['rdb'][k][0]:
                 chg = True
                 break
         if chg:
             rider = self.rdb.add_rider(dbr, overwrite=False)
             GLib.idle_add(self.select_row, rider)
 
     def select_row(self, rider):
@@ -1644,74 +1614,80 @@
             rider = self._cur_rider_sel
             dbr = self.rdb[rider]
             schema = dbr.get_schema()
             rtype = schema['rtype']['prompt']
             short = 'Edit %s %s' % (rtype, dbr.get_bibstr())
             res = uiutil.options_dlg(window=self.window,
                                      title=short,
-                                     schema=schema,
-                                     obj=dbr)
+                                     sections={
+                                         'rdb': {
+                                             'title': 'Rider',
+                                             'schema': schema,
+                                             'object': dbr,
+                                         },
+                                     })
             if rtype == 'Team':
                 # Patch the org value which is not visible, without notify
                 dbr.set_value('org', dbr['no'].upper())
-            if res['no'][0] or res['series'][0]:
+            if res['rdb']['no'][0] or res['rdb']['series'][0]:
                 # change of number or series requires some care
                 self._cur_rider_sel = None
                 newrider = self.rdb.add_rider(dbr,
                                               notify=False,
                                               overwrite=False)
                 if rtype == 'Category':
                     if uiutil.questiondlg(
                             window=self.window,
                             question='Update rider categories?',
                             subtext=
                             'Riders in the old category will be updated to the new one',
                             title='Update Cats?'):
-                        self.rdb.update_cats(res['no'][1],
-                                             res['no'][2],
+                        self.rdb.update_cats(res['rdb']['no'][1],
+                                             res['rdb']['no'][2],
                                              notify=False)
                         # and current event
                         if self.curevent is not None:
-                            if res['no'][1].upper() in self.curevent.cats:
+                            if res['rdb']['no'][1].upper(
+                            ) in self.curevent.cats:
                                 nc = []
                                 for c in self.curevent.cats:
-                                    if c == res['no'][1].upper():
-                                        nc.append(res['no'][2].upper())
+                                    if c == res['rdb']['no'][1].upper():
+                                        nc.append(res['rdb']['no'][2].upper())
                                     else:
                                         nc.append(c)
                                 self.curevent.loadcats(nc)
                                 doreopen = True
                 else:
                     # update curevent
                     if self.curevent is not None:
-                        if self.curevent.getrider(res['no'][1],
-                                                  res['series'][1]):
+                        if self.curevent.getrider(res['rdb']['no'][1],
+                                                  res['rdb']['series'][1]):
                             # rider was in event, add new one
                             self.curevent.addrider(dbr['no'], dbr['series'])
                             if self.curevent.timerstat == 'idle':
-                                self.curevent.delrider(res['no'][1],
-                                                       res['series'][1])
+                                self.curevent.delrider(res['rdb']['no'][1],
+                                                       res['rdb']['series'][1])
                             else:
                                 _log.warning(
                                     'Changed rider number %r => %r, check data',
-                                    res['no'][1], res['no'][2])
+                                    res['rdb']['no'][1], res['rdb']['no'][2])
 
                 # del triggers a global notify
                 del (self.rdb[rider])
 
                 # then try to select the modified row
                 GLib.idle_add(self.select_row, newrider)
 
                 # then reopen curevent if flagged after notify
                 if doreopen:
-                    GLib.idle_add(self.menu_race_run_activate_cb)
+                    GLib.idle_add(self.event_reload)
             else:
                 # notify meet and event of any changes, once
-                for k in res:
-                    if res[k][0]:
+                for k in res['rdb']:
+                    if res['rdb'][k][0]:
                         dbr.notify()
                         break
 
     def rider_lookup_cb(self, menuitem, data=None):
         _log.info('Rider lookup not yet enabled')
 
     def rider_delete_cb(self, menuitem, data=None):
@@ -1751,49 +1727,48 @@
                                   subtext=info,
                                   title='Delete?'):
                 if self.curevent is not None:
                     if series == 'cat':
                         cat = dbr['no'].upper()
                         if cat in self.curevent.cats:
                             _log.warning('Deleted cat %s in open event', cat)
-                    elif series not in ['ds', 'spare', 'team']:
+                    elif series not in ('ds', 'spare', 'team'):
                         self.curevent.delrider(dbr['no'], series)
                         _log.info('Remove rider %s from event', short)
                 del (self.rdb[self._cur_rider_sel])
                 _log.info('Deleted %s', short)
                 self._cur_rider_sel = None
             else:
-                _log.debug('Aborted')
+                _log.debug('Rider delete aborted')
 
     def __init__(self, etype=None, lockfile=None):
         """Meet constructor."""
         self.loghandler = None  # set in loadconfig to meet dir
         self.exportpath = EXPORTPATH
         if etype not in ROADRACE_TYPES:
             etype = 'road'
-        self.meetlock = lockfile
         self.etype = etype
+        self.meetlock = lockfile
         self.shortname = None
-        self.title_str = ''
-        self.host_str = ''
-        self.subtitle_str = ''
-        self.document_str = ''
-        self.date_str = ''
-        self.organiser_str = ''
-        self.commissaire_str = ''
+        self.title = ''
+        self.host = ''
+        self.subtitle = ''
+        self.document = ''
+        self.date = ''
+        self.organiser = ''
+        self.pcp = ''
         self.distance = None
         self.diststr = ''
         self.linkbase = '.'
         self.provisionalstart = False
         self.indexlink = None
         self.nextlink = None
         self.prevlink = None
 
-        self.bibs_in_results = True
-        self.remote_enable = False
+        self.remoteenable = False
         self.lifexport = False
         self.resfiles = True
         self.announceresult = True
 
         # printer preferences
         paper = Gtk.PaperSize.new_custom('metarace-full', 'A4 for reports',
                                          595, 842, Gtk.Unit.POINTS)
@@ -1804,21 +1779,21 @@
         self.pageset.set_top_margin(0, Gtk.Unit.POINTS)
         self.pageset.set_bottom_margin(0, Gtk.Unit.POINTS)
         self.pageset.set_left_margin(0, Gtk.Unit.POINTS)
         self.pageset.set_right_margin(0, Gtk.Unit.POINTS)
 
         # hardware connections
         self.timertopic = None  # remote timer topic
-        self.timer = decoder()
-        self.timer_port = ''
-        self.timer.setcb(self._timercb)
+        self._timer = decoder()
+        self.timer = ''
+        self._timer.setcb(self._timercb)
         self.timercb = None  # set by event app
-        self.alttimer = timy()  # alttimer is always timy
-        self.alttimer_port = ''
-        self.alttimer.setcb(self._alttimercb)
+        self._alttimer = timy()  # alttimer is always timy
+        self.alttimer = ''
+        self._alttimer.setcb(self._alttimercb)
         self.alttimercb = None  # set by event app
         self.announce = telegraph()
         self.announce.setcb(self._controlcb)
         self.anntopic = None
         self.mirrorpath = ''
         self.mirrorcmd = None
         self.mirrorfile = ''
@@ -1836,16 +1811,14 @@
         self.rfufail = 0
         self.status = b.get_object('status')
         self.log_buffer = b.get_object('log_buffer')
         self.log_view = b.get_object('log_view')
         #self.log_view.modify_font(uiutil.LOGVIEWFONT)
         self.log_scroll = b.get_object('log_box').get_vadjustment()
         self.context = self.status.get_context_id('metarace meet')
-        self.menu_race_close = b.get_object('menu_race_close')
-        self.menu_race_abort = b.get_object('menu_race_abort')
         self.decoder_configure = b.get_object('menu_timing_configure')
         self.race_box = b.get_object('race_box')
         self.stat_but = uiutil.statButton()
         b.get_object('race_stat_but').add(self.stat_but)
         self.action_model = b.get_object('race_action_model')
         self.action_combo = b.get_object('race_action_combo')
         self.action_entry = b.get_object('race_action_entry')
@@ -1958,142 +1931,182 @@
 
         t.show()
         t.connect('button_press_event', self._view_button_press)
         self._clv = t
         b.get_object('cat_box').add(t)
 
         # get rider db
-        _log.debug('Add riderdb and eventdb')
+        _log.debug('Add riderdb')
         self.rdb = riderdb.riderdb()
         self.rdb.set_notify(self._rcb)
         self._tagmap = {}
         self._maptag = {}
 
-        ## get event db -> loadconfig adds empty event if one not present
-        self.edb = eventdb.eventdb([])
-
         # select event page in notebook.
         b.get_object('meet_nb').set_current_page(0)
 
         # start timer
         GLib.timeout_add_seconds(1, self.timeout)
 
 
 class fakemeet(roadmeet):
     """Non-interactive meet wrapper"""
 
-    def __init__(self, edb, rdb):
-        self.edb = edb
+    def __init__(self, rdb):
+        self.etype = 'road'
         self.rdb = rdb
-        self.timer = decoder()
-        self.alttimer = timy()
+        self._timer = decoder()
+        self._alttimer = timy()
         self.stat_but = uiutil.statButton()
         self.action_model = Gtk.ListStore(str, str)
         self.action_model.append(['a', 'a'])
         self.action_combo = Gtk.ComboBox()
         self.action_combo.set_model(self.action_model)
         self.action_combo.set_active(0)
         self.announce = telegraph()
-        self.title_str = ''
-        self.host_str = ''
-        self.subtitle_str = ''
-        self.date_str = ''
-        self.organiser_str = ''
-        self.commissaire_str = ''
+        self.title = ''
+        self.host = ''
+        self.subtitle = ''
+        self.date = ''
+        self.organiser = ''
+        self.pcp = ''
         self.distance = None
         self.linkbase = '.'
         self.provisionalstart = False
         self.indexlink = None
         self.nextlink = None
         self.prevlink = None
-        self.bibs_in_results = True
 
     def cmd_announce(self, command, msg):
         return False
 
     def rider_announce(self, rvec):
         return False
 
     def timer_announce(self, evt, timer=None, source=''):
         return False
 
-    def report_strings(self, rep):
-        """Copy the meet strings into the supplied report."""
-        rep.strings['title'] = self.title_str
-        rep.strings['subtitle'] = self.subtitle_str
-        rep.strings['host'] = self.host_str
-        rep.strings['docstr'] = self.document_str
-        rep.strings['datestr'] = strops.promptstr('Date:', self.date_str)
-        rep.strings['commstr'] = strops.promptstr('Chief Commissaire:',
-                                                  self.commissaire_str)
-        rep.strings['orgstr'] = strops.promptstr('Organiser:',
-                                                 self.organiser_str)
-        if self.distance:
-            rep.strings['diststr'] = strops.promptstr(
-                'Distance:',
-                str(self.distance) + '\u2006km')
-        else:
-            rep.strings['diststr'] = self.diststr
-
-        if self.eventcode:
-            rep.eventid = self.eventcode
-        if self.prevlink:
-            rep.prevlink = self.prevlink
-        if self.nextlink:
-            rep.nextlink = self.nextlink
-        if self.indexlink:
-            rep.indexlink = self.indexlink
-        if self.shortname:
-            rep.shortname = self.shortname
-
     def loadconfig(self):
         """Load meet config from disk."""
-        cr = jsonconfig.config({
-            'roadmeet': {
-                'title': '',
-                'shortname': '',
-                'subtitle': '',
-                'host': '',
-                'document': '',
-                'date': '',
-                'organiser': '',
-                'commissaire': '',
-                'distance': None,
-                'diststr': '',
-                'linkbase': '.',
-                'indexlink': None,
-                'nextlink': None,
-                'prevlink': None,
-                'provisionalstart': False,
-                'eventcode': '',
-                'id': ''
-            }
-        })
-        cr.add_section('roadmeet')
+        cr = jsonconfig.config()
+        cr.add_section('roadmeet', _CONFIG_SCHEMA)
         cr.merge(metarace.sysconf, 'roadmeet')
-        cr.load('config.json')
+        cr.load(CONFIGFILE)
+        cr.export_section('roadmeet', self)
 
-        # set meet meta, and then copy into text entries
-        self.shortname = cr.get('roadmeet', 'shortname')
-        self.title_str = cr.get('roadmeet', 'title')
-        self.host_str = cr.get('roadmeet', 'host')
-        self.subtitle_str = cr.get('roadmeet', 'subtitle')
-        self.document_str = cr.get('roadmeet', 'document')
-        self.date_str = cr.get('roadmeet', 'date')
-        self.organiser_str = cr.get('roadmeet', 'organiser')
-        self.commissaire_str = cr.get('roadmeet', 'commissaire')
-        self.linkbase = cr.get('roadmeet', 'linkbase')
-        self.distance = cr.get_float('roadmeet', 'distance')
-        self.diststr = cr.get('roadmeet', 'diststr')
-        self.eventcode = cr.get('roadmeet', 'eventcode')
-        self.linkbase = cr.get('roadmeet', 'linkbase')
-        self.indexlink = cr.get('roadmeet', 'indexlink')
-        self.prevlink = cr.get('roadmeet', 'prevlink')
-        self.nextlink = cr.get('roadmeet', 'nextlink')
-        self.provisionalstart = cr.get_bool('roadmeet', 'provisionalstart')
+
+def edit_defaults():
+    """Run a sysconf editor dialog"""
+    metarace.sysconf.add_section('roadmeet', _CONFIG_SCHEMA)
+    metarace.sysconf.add_section('rms', _RMS_SCHEMA)
+    metarace.sysconf.add_section('irtt', _IRTT_SCHEMA)
+    metarace.sysconf.add_section('trtt', _TRTT_SCHEMA)
+    metarace.sysconf.add_section('export', _EXPORT_SCHEMA)
+    metarace.sysconf.add_section('telegraph', _TG_SCHEMA)
+    metarace.sysconf.add_section('thbc', _THBC_SCHEMA)
+    metarace.sysconf.add_section('rru', _RRU_SCHEMA)
+    metarace.sysconf.add_section('rrs', _RRS_SCHEMA)
+    metarace.sysconf.add_section('timy', _TIMY_SCHEMA)
+    cfgres = uiutil.options_dlg(title='Edit Default Configuration',
+                                sections={
+                                    'roadmeet': {
+                                        'title': 'Meet',
+                                        'schema': _CONFIG_SCHEMA,
+                                        'object': metarace.sysconf,
+                                    },
+                                    'rms': {
+                                        'title': 'Road/Cross',
+                                        'schema': _RMS_SCHEMA,
+                                        'object': metarace.sysconf,
+                                    },
+                                    'irtt': {
+                                        'title': 'Individual TT',
+                                        'schema': _IRTT_SCHEMA,
+                                        'object': metarace.sysconf,
+                                    },
+                                    'trtt': {
+                                        'title': 'Teams TT',
+                                        'schema': _TRTT_SCHEMA,
+                                        'object': metarace.sysconf,
+                                    },
+                                    'export': {
+                                        'title': 'Export',
+                                        'schema': _EXPORT_SCHEMA,
+                                        'object': metarace.sysconf,
+                                    },
+                                    'telegraph': {
+                                        'title': 'Telegraph',
+                                        'schema': _TG_SCHEMA,
+                                        'object': metarace.sysconf,
+                                    },
+                                    'timy': {
+                                        'title': 'Timy',
+                                        'schema': _TIMY_SCHEMA,
+                                        'object': metarace.sysconf,
+                                    },
+                                    'thbc': {
+                                        'title': 'THBC',
+                                        'schema': _THBC_SCHEMA,
+                                        'object': metarace.sysconf,
+                                    },
+                                    'rru': {
+                                        'title': 'RR USB',
+                                        'schema': _RRU_SCHEMA,
+                                        'object': metarace.sysconf,
+                                    },
+                                    'rrs': {
+                                        'title': 'RR System',
+                                        'schema': _RRS_SCHEMA,
+                                        'object': metarace.sysconf,
+                                    },
+                                })
+
+    # check for sysconf changes:
+    syschange = False
+    for sec in cfgres:
+        for key in cfgres[sec]:
+            if cfgres[sec][key][0]:
+                syschange = True
+                break
+    if syschange:
+        backup = metarace.SYSCONF + '.bak'
+        _log.info('Backing up old defaults to %r', backup)
+        try:
+            if os.path.exists(backup):
+                os.unlink(backup)
+            os.link(metarace.SYSCONF, backup)
+        except Exception as e:
+            _log.warning('%s saving defaults backup: %s', e.__class__.__name__,
+                         e)
+        _log.info('Edit default: Saving sysconf to %r', metarace.SYSCONF)
+        with metarace.savefile(metarace.SYSCONF, perm=0o600) as f:
+            metarace.sysconf.write(f)
+    else:
+        _log.info('Edit default: No changes to save')
+    return 0
+
+
+def createmeet():
+    """Create a new empty meet folder"""
+    ret = None
+    count = 0
+    dname = 'road_' + tod.datetime.now().date().isoformat()
+    cname = dname
+    while count < 100:
+        mpath = os.path.join(metarace.DATA_PATH, cname)
+        if not os.path.exists(mpath):
+            os.makedirs(mpath)
+            _log.info('Created empty meet folder: %r', mpath)
+            ret = mpath
+            break
+        count += 1
+        cname = dname + '_%02d' % (count)
+    if ret is None:
+        _log.error('Unable to create empty meet folder')
+    return ret
 
 
 def main():
     """Run the road meet application as a console script."""
     chk = Gtk.init_check()
     if not chk[0]:
         print('Unable to init Gtk display')
@@ -2102,67 +2115,70 @@
     # attach a console log handler to the root logger
     ch = logging.StreamHandler()
     ch.setLevel(metarace.LOGLEVEL)
     fh = logging.Formatter(metarace.LOGFORMAT)
     ch.setFormatter(fh)
     logging.getLogger().addHandler(ch)
 
-    metarace.init()
-
     # try to set the menubar accel and logo
     try:
         lfile = metarace.default_file(metarace.LOGO)
         Gtk.Window.set_default_icon_from_file(lfile)
         mset = Gtk.Settings.get_default()
         mset.set_property('gtk-menu-bar-accel', 'F24')
     except Exception as e:
         _log.debug('%s setting property: %s', e.__class__.__name__, e)
 
-    configpath = metarace.DATA_PATH
+    doconfig = False
+    configpath = None
     if len(sys.argv) > 2:
-        _log.error('Usage: roadmeet [configdir]')
+        _log.error('Usage: roadmeet [PATH]')
         sys.exit(1)
     elif len(sys.argv) == 2:
-        configpath = sys.argv[1]
+        if sys.argv[1] == '--edit-default':
+            doconfig = True
+            configpath = metarace.DEFAULTS_PATH
+            _log.debug('Edit defaults, configpath: %r', configpath)
+        else:
+            configpath = sys.argv[1]
+    else:
+        configpath = createmeet()
     configpath = metarace.config_path(configpath)
     if configpath is None:
-        _log.error('Unable to open meet config %r', sys.argv[1])
+        _log.debug('Missing path, command: %r', sys.argv)
+        _log.error('Error opening meet')
         if not os.isatty(sys.stdout.fileno()):
-            err = Gtk.MessageDialog(None, Gtk.DialogFlags.MODAL,
-                                    Gtk.MessageType.ERROR,
-                                    Gtk.ButtonsType.CLOSE,
-                                    'Error reading meet config.')
-            err.set_title('roadmeet: Error')
-            err.format_secondary_text(
-                'Check config file and event log for error messages')
-            err.run()
+            uiutil.messagedlg(
+                message='Error opening meet.',
+                title='roadmeet: Error',
+                subtext='Roadmeet was unable to open a meet folder.')
         sys.exit(-1)
-    app = runapp(configpath)
-    return Gtk.main()
 
-
-def runapp(configpath, etype=None):
-    """Create the roadmeet object, start in configpath and return a handle."""
     lf = metarace.lockpath(configpath)
     if lf is None:
         _log.error('Unable to lock meet config, already in use')
         if not os.isatty(sys.stdout.fileno()):
-            err = Gtk.MessageDialog(None, Gtk.DialogFlags.MODAL,
-                                    Gtk.MessageType.ERROR,
-                                    Gtk.ButtonsType.CLOSE,
-                                    'Meet folder is locked.')
-            err.format_secondary_text(
+            uiutil.messagedlg(
+                message='Meet folder is locked.',
+                title='roadmeet: Locked',
+                subtext=
                 'Another application has locked the meet folder for use.')
-            err.set_title('roadmeet: Locked')
-            err.run()
         sys.exit(-1)
     _log.debug('Entering meet folder %r', configpath)
     os.chdir(configpath)
-    app = roadmeet(etype, lf)
-    app.loadconfig()
-    app.window.show()
-    app.start()
-    return app
+    metarace.init()
+    if doconfig:
+        return edit_defaults()
+    else:
+        app = roadmeet(None, lf)
+        mp = configpath
+        if mp.startswith(metarace.DATA_PATH):
+            mp = mp.replace(metarace.DATA_PATH + '/', '')
+        app.status.push(app.context, 'Meet Folder: ' + mp)
+        app.loadconfig()
+        app.window.show()
+        app.start()
+        return Gtk.main()
 
 
 if __name__ == '__main__':
     sys.exit(main())
```

### Comparing `metarace-roadmeet-1.13.1/src/roadmeet/irtt.py` & `metarace-roadmeet-1.13.2/src/roadmeet/irtt.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,38 +21,39 @@
 from metarace import riderdb
 from metarace import strops
 from metarace import countback
 from metarace import report
 from metarace import jsonconfig
 from . import uiutil
 
-from roadmeet.rms import rms, RESERVED_SOURCES
+from roadmeet.rms import rms, RESERVED_SOURCES, GAPTHRESH
 
-_log = logging.getLogger('metarace.irtt')
+_log = logging.getLogger('irtt')
 _log.setLevel(logging.DEBUG)
 
 # rider commands
 RIDER_COMMANDS_ORD = [
-    'add', 'del', 'que', 'dns', 'otl', 'dnf', 'dsq', 'com', ''
+    'add', 'del', 'que', 'dns', 'otl', 'dnf', 'dsq', 'dec', ''
 ]
 RIDER_COMMANDS = {
     'dns': 'Did not start',
     'dnf': 'Did not finish',
     'add': 'Add starters',
     'del': 'Remove starters',
     'que': 'Query riders',
-    'com': 'Add comment',
+    'dec': 'Add decision',
     'otl': 'Outside time limit',
     'dsq': 'Disqualify',
     'onc': 'Riders on course',
     '': '',
 }
 
 DNFCODES = ['otl', 'dsq', 'dnf', 'dns']
 STARTFUDGE = tod.tod(30)
+STARTGAP = tod.tod('1:00')
 ARRIVALTIMEOUT = tod.tod('2:30')
 
 # startlist model columns
 COL_BIB = 0
 COL_NAMESTR = 1
 COL_SHORTNAME = 2
 COL_CAT = 3
@@ -87,162 +88,164 @@
 
 # extended function key mappings
 key_abort = 'F5'  # + ctrl for clear/abort
 key_announce = 'F4'  # clear scratch
 # IRTT does not use confirm keys
 
 # config version string
-EVENT_ID = 'roadtt-3.2'
+EVENT_ID = 'roadtt-3.4'
 
 _CONFIG_SCHEMA = {
     'etype': {
         'prompt': 'Individual Time Trial',
         'control': 'section'
     },
     'categories': {
         'prompt': 'Categories:',
         'hint': 'Startlist and result categories',
-        'defer': True
+        'defer': True,
+        'default': '',
     },
     'minlap': {
         'prompt': 'Minimum Lap:',
         'control': 'short',
         'places': 1,
         'type': 'tod',
         'hint': 'Reject laps shorter than minimum lap time',
-        'attr': 'minlap'
+        'attr': 'minlap',
+        'default': STARTFUDGE,
     },
     'totlaps': {
         'prompt': 'Laps:',
         'control': 'short',
         'type': 'int',
         'attr': 'totlaps',
         'subtext': '(Cat laps override)',
-        'hint': 'Default target number of laps for event'
+        'hint': 'Default target number of laps for event',
     },
     'startgap': {
         'prompt': 'Start Gap:',
         'control': 'short',
         'type': 'tod',
         'places': 0,
         'attr': 'startgap',
-        'hint': 'Time gap between rider start times'
+        'hint': 'Time gap between rider start times',
+        'default': STARTGAP,
     },
     'autoimpulse': {
         'prompt': 'Autotime:',
         'control': 'check',
         'type': 'bool',
         'defer': True,
         'attr': 'autoimpulse',
         'subtext': 'Match impulses to transponder?',
         'hint': 'Impulses automatically matched to transponder readings',
+        'default': False,
     },
     'startloop': {
         'prompt': 'Start Loop:',
         'control': 'short',
         'type': 'chan',
         'defer': True,
         'attr': 'startloop',
-        'hint': 'Transponder loop/channel ID at start line'
+        'hint': 'Transponder loop/channel ID at start line',
     },
     'finishloop': {
         'prompt': 'Finish Loop:',
         'control': 'short',
         'type': 'chan',
         'defer': True,
         'attr': 'finishloop',
-        'hint': 'Transponder loop/channel ID at finish line'
+        'hint': 'Transponder loop/channel ID at finish line',
     },
     'strictstart': {
         'prompt': 'Start:',
         'control': 'check',
         'type': 'bool',
         'defer': True,
         'attr': 'strictstart',
         'subtext': 'Start times are strict?',
         'hint': 'Check rider start times against schedule',
+        'default': True,
+    },
+    'showtimers': {
+        'prompt': 'Manual Timers:',
+        'subtext': 'Show?',
+        'hint': 'Show manual timer controls',
+        'type': 'bool',
+        'control': 'check',
+        'attr': 'showtimers',
+        'default': True,
     },
     'arrivaltimeout': {
         'prompt': 'Arvl Timeout:',
         'control': 'short',
         'type': 'tod',
         'places': 0,
         'attr': 'arrivaltimeout',
-        'hint': 'Clear arrivals off report after this long'
+        'hint': 'Clear arrivals off report after this long',
+        'default': ARRIVALTIMEOUT,
     },
     'onestartlist': {
         'prompt': 'Startlist:',
         'control': 'check',
         'type': 'bool',
         'attr': 'onestartlist',
         'subtext': 'Combine categories?',
         'hint': 'Report all categories in a single startlist',
+        'default': True,
     },
     'autoexport': {
         'prompt': 'Export:',
         'control': 'check',
         'type': 'bool',
         'attr': 'autoexport',
         'subtext': 'Automatically export?',
         'hint': 'Export result automatically',
+        'default': False,
     },
     'timelimit': {
         'prompt': 'Time Limit:',
         'control': 'short',
         'attr': 'timelimit',
         'hint': 'Time limit eg: 12%  +1:23  4h00:00',
     },
-    # Clubmode does not function well with irtt
     'clubmode': {
         'prompt': 'Club Mode:',
         'control': 'check',
         'type': 'bool',
         'attr': 'clubmode',
         'subtext': 'Add starters by transponder passing?',
         'hint': 'Add riders to event on passing',
+        'default': False,
     },
     # Spare bikes should be handled manually on irtt
     'allowspares': {
         'prompt': 'Spares:',
-        'control': 'check',
+        'control': 'none',
         'type': 'bool',
         'attr': 'allowspares',
         'subtext': 'Record spare bike passings?',
         'readonly': True,
         'hint': 'Add spare bike passings to event as placeholders',
+        'default': False,
+    },
+    # Provided for alignment with rms and trtt
+    'gapthresh': {
+        'prompt': 'Time Gap:',
+        'control': 'none',
+        'type': 'tod',
+        'places': 2,
+        'hint': 'Threshold for automatic time gap insertion',
+        'attr': 'gapthresh',
+        'default': GAPTHRESH,
     },
 }
 
 
-def jsob(inmap):
-    """Return a json'able map."""
-    ret = None
-    if inmap is not None:
-        ret = {}
-        for key in inmap:
-            if key in ['minelap', 'maxelap']:
-                ret[key] = inmap[key].rawtime()
-            else:
-                ret[key] = inmap[key]
-    return ret
-
-
-def unjsob(inmap):
-    """Un-jsob the provided map."""
-    ret = None
-    if inmap is not None:
-        ret = {}
-        for key in inmap:
-            if key in ['minelap', 'maxelap']:
-                ret[key] = tod.mktod(inmap[key])
-            else:
-                ret[key] = inmap[key]
-    return ret
-
-
 class irtt(rms):
     """Data handling for road time trial."""
 
     def resettimer(self):
         """Return event to idle and remove all results"""
         _log.debug('Reset')
         self.startpasses.clear()
@@ -274,17 +277,19 @@
     def key_event(self, widget, event):
         """Race window key press handler."""
         if event.type == Gdk.EventType.KEY_PRESS:
             key = Gdk.keyval_name(event.keyval) or 'None'
             if event.state & Gdk.ModifierType.CONTROL_MASK:
                 if key == key_abort:  # override ctrl+f5
                     if uiutil.questiondlg(
-                            self.meet.window, 'Reset event to idle?',
-                            'Note: All result and timing data will be cleared.'
-                    ):
+                            window=self.meet.window,
+                            question='Reset event to idle?',
+                            subtext=
+                            'Note: All result and timing data will be cleared.',
+                            title='Reset event?'):
                         self.resettimer()
                     return True
             if key[0] == 'F':
                 if key == key_announce:
                     self.meet.cmd_announce('clear', 'all')
                     self._doannounce = True
                     return True
@@ -301,15 +306,15 @@
             self.timerstat = 'running'
             self.meet.stat_but.update('ok', 'Running')
             self.meet.stat_but.set_sensitive(True)
         else:
             self.timerstat = 'finished'
             self.meet.stat_but.update('idle', 'Finished')
             self.meet.stat_but.set_sensitive(False)
-            self.hidetimers = True
+            self.showtimers = False
             self.timerframe.hide()
 
     def armfinish(self):
         if self.timerstat == 'running':
             if self.fl.getstatus() != 'finish' and self.fl.getstatus(
             ) != 'armfin':
                 self.fl.toarmfin()
@@ -320,40 +325,61 @@
     def armstart(self):
         if self.timerstat == 'idle':
             _log.info('Armed for timing sync')
             self.timerstat = 'armstart'
         elif self.timerstat == 'armstart':
             self.resetall()
         elif self.timerstat == 'running':
-            if self.sl.getstatus() in ['armstart', 'running']:
+            if self.sl.getstatus() in ('armstart', 'running'):
                 self.sl.toidle()
             elif self.sl.getstatus() != 'running':
                 self.sl.toarmstart()
 
     def delayed_announce(self):
         """Re-announce arrivals."""
         rep = report.report()
         arrivals = self.arrival_report()  # fetch all arrivals
         if len(arrivals) > 0:
             self.meet.obj_announce('arrivals', arrivals[0].serialize(rep))
         return False
 
-    def wallstartstr(self, col, cr, model, iter, data=None):
+    def editstart(self, cell, path, new_text, col=None):
+        """Edit the rider's start time."""
+        newst = tod.mktod(new_text)
+        if newst is not None:
+            if self.riders[path][COL_TODSTART] is not None:
+                self.riders[path][COL_TODSTART] = newst
+                _log.info(
+                    'Adjusted rider %s start time: %s',
+                    strops.bibser2bibstr(self.riders[path][COL_BIB],
+                                         self.riders[path][COL_SERIES]),
+                    newst.rawtime())
+            else:
+                newst = newst.truncate(0)
+                self.riders[path][COL_WALLSTART] = newst
+                _log.info(
+                    'Adjusted rider %s advertised start time: %s',
+                    strops.bibser2bibstr(self.riders[path][COL_BIB],
+                                         self.riders[path][COL_SERIES]),
+                    newst.rawtime(0))
+            self._dorecalc = True
+
+    def startstr(self, col, cr, model, iter, data=None):
         """Format start time into text for listview."""
         st = model.get_value(iter, COL_TODSTART)
         if st is not None:
-            cr.set_property('text', st.timestr(2))  # time from tapeswitch
+            cr.set_property('text', st.rawtime(2))
             cr.set_property('style', uiutil.STYLE_NORMAL)
         else:
-            cr.set_property('style', uiutil.STYLE_OBLIQUE)
             wt = model.get_value(iter, COL_WALLSTART)
             if wt is not None:
-                cr.set_property('text', wt.timestr(0))  # adv start
+                cr.set_property('text', wt.rawtime(0))
             else:
                 cr.set_property('text', '')  # no info on start time
+            cr.set_property('style', uiutil.STYLE_OBLIQUE)
 
     def announce_rider(self,
                        place='',
                        bib='',
                        namestr='',
                        shortname='',
                        cat='',
@@ -370,17 +396,16 @@
         self.meet.rider_announce([place, bib, namestr, cat, rts], 'finish')
 
     def geteta(self, iter):
         """Return a best guess rider's ET."""
         ret = self.getelapsed(iter)
         if ret is None:
             # scan each inter from farthest to nearest
-            for ipt in [
-                    COL_INTERE, COL_INTERD, COL_INTERC, COL_INTERB, COL_INTERA
-            ]:
+            for ipt in (COL_INTERE, COL_INTERD, COL_INTERC, COL_INTERB,
+                        COL_INTERA):
                 if ipt in self.ischem and self.ischem[ipt] is not None:
                     dist = self.ischem[ipt]['dist']
                     inter = self.riders.get_value(iter, ipt)
                     if inter is not None and dist is not None:
                         totdist = 1000.0 * self.meet.distance
                         st = self.riders.get_value(iter, COL_TODSTART)
                         if st is None:  # defer to start time
@@ -389,52 +414,33 @@
                             et = inter - st
                             spd = (1000.0 * dist) / float(et.timeval)
                             ret = tod.tod(str(totdist / spd))
                             self.riders.set_value(iter, COL_DIST, int(dist))
                             break
         return ret
 
-    def lrgetelapsed(self, lr, runtime=False):
-        """Return a tod elapsed for a tree row"""
-        ret = None
-        ft = lr[COL_TODFINISH]
-        if ft is not None:
-            st = lr[COL_TODSTART]
-            if st is None:  # defer to start time
-                st = lr[COL_WALLSTART]
-            if st is not None:  # still none is error
-                pt = lr[COL_TODPENALTY]
-                # penalties are added into stage result - for consistency
-                ret = (ft - st) + pt
-        elif runtime:
-            st = lr[COL_TODSTART]
-            if st is None:  # defer to start time
-                st = lr[COL_WALLSTART]
-            if st is not None:  # still none is error
-                ret = tod.now() - st  # runtime increases!
-        return ret
-
     def getelapsed(self, iter, runtime=False):
         """Return a tod elapsed time for an iter"""
         ret = None
         ft = self.riders.get_value(iter, COL_TODFINISH)
         if ft is not None:
             st = self.riders.get_value(iter, COL_TODSTART)
             if st is None:  # defer to start time
                 st = self.riders.get_value(iter, COL_WALLSTART)
             if st is not None:  # still none is error
                 pt = self.riders.get_value(iter, COL_TODPENALTY)
                 # penalties are added into stage result - for consistency
-                ret = (ft - st) + pt
+                ret = ((ft - st) + pt).round(self.precision)
         elif runtime:
             st = self.riders.get_value(iter, COL_TODSTART)
             if st is None:  # defer to start time
                 st = self.riders.get_value(iter, COL_WALLSTART)
             if st is not None:  # still none is error
-                ret = tod.now() - st  # runtime increases!
+                # truncate rolling time
+                ret = (tod.now() - st).truncate(self.precision)
         return ret
 
     def checkplaces(self, rlist='', dnf=True):
         """Check the proposed places against current race model."""
         ret = True
         placeset = set()
         for no in strops.reformat_bibserlist(rlist).split():
@@ -499,15 +505,14 @@
         elif acode == 'del':
             rlist = strops.reformat_bibserlist(rlist)
             for bibstr in rlist.split():
                 bib, ser = strops.bibstr2bibser(bibstr)
                 self.delrider(bib, ser)
             return True
         elif acode == 'add':
-            _log.info('Add starter deprecated: Use startlist import')
             rlist = strops.reformat_bibserlist(rlist)
             for bibstr in rlist.split():
                 bib, ser = strops.bibstr2bibser(bibstr)
                 self.addrider(bib, ser)
             return True
         elif acode == 'dnf':
             self.dnfriders(strops.reformat_bibserlist(rlist))
@@ -530,16 +535,16 @@
         elif acode == 'man':
             # crude hack tool for now
             self.manpassing(strops.reformat_bibserlist(rlist))
             return True
         elif acode == 'fin':
             _log.info('Finish places ignored')
             return True
-        elif acode == 'com':
-            self.add_comment(rlist)
+        elif acode == 'dec':
+            self.add_decision(rlist)
             return True
         else:
             _log.error('Ignoring invalid action %r', acode)
         return False
 
     def elapstr(self, col, cr, model, iter, data=None):
         """Format elapsed time into text for listview."""
@@ -549,15 +554,15 @@
             if st is None:  # defer to wall start time
                 st = model.get_value(iter, COL_WALLSTART)
                 cr.set_property('style', uiutil.STYLE_OBLIQUE)
             else:
                 cr.set_property('style', uiutil.STYLE_NORMAL)
             et = self.getelapsed(iter)
             if et is not None:
-                cr.set_property('text', et.timestr(2))
+                cr.set_property('text', et.rawtime(self.precision))
             else:
                 cr.set_property('text', '[ERR]')
         else:
             cr.set_property('text', '')
 
     def loadconfig(self):
         """Load race config from disk."""
@@ -565,101 +570,55 @@
         self.riders.clear()
         self.results = {'': tod.todlist('UNCAT')}
         self.cats = []
 
         cr = jsonconfig.config({
             'irtt': {
                 'startlist': '',
-                'id': EVENT_ID,
-                'start': '0',
-                'comment': [],
-                'categories': [],
-                'arrivaltimeout': ARRIVALTIMEOUT,
-                'lstart': '0',
-                'startgap': '1:00',
-                'precision': 2,
-                'autoexport': False,
+                'start': tod.ZERO,
+                'finished': False,
+                'decisions': [],
+                'lstart': tod.ZERO,
                 'intermeds': [],
                 'contests': [],
-                'minlap': STARTFUDGE,
-                'strictstart': True,
-                'autoimpulse': False,
-                'startloop': None,
-                'finishloop': None,
-                'totlaps': None,
-                'interloops': {},
-                'interlaps': {},
                 'tallys': [],
-                'onestartlist': True,
-                'hidetimers': False,
                 'startpasses': [],
                 'finishpasses': [],
-                'timelimit': None,
-                'finished': False,
                 'showinter': None,
                 'intera': None,
                 'interb': None,
                 'interc': None,
                 'interd': None,
                 'intere': None,
+                'interloops': {},
+                'interlaps': {},
             }
         })
-        cr.add_section('irtt')
+        cr.add_section('irtt', _CONFIG_SCHEMA)
         cr.add_section('riders')
         cr.add_section('stagebonus')
         cr.add_section('stagepenalty')
         cr.merge(metarace.sysconf, 'irtt')
         if not cr.load(self.configfile):
             _log.info('%r not read, loading defaults', self.configfile)
+        cr.export_section('irtt', self)
 
-        # load default gap
-        self.startgap = tod.mktod(cr.get('irtt', 'startgap'))
-        if self.startgap is None:
-            self.startgap = tod.tod('1:00')
-
-        # load result precision - allow manual downgrade
-        self.precision = cr.get_posint('irtt', 'precision', 1)
-        if self.precision > 2:  # posint forbids negatives
-            self.precision = 2
-
-        # load minimum elapsed time
-        self.minlap = tod.mktod(cr.get('irtt', 'minlap'))
-        if self.minlap is None:
-            self.minlap = STARTFUDGE
-        self.timelimit = cr.get('irtt', 'timelimit')  # save as str
-
-        # allow auto export
-        self.autoexport = cr.get_bool('irtt', 'autoexport')
-        # sloppy start times
-        self.strictstart = cr.get_bool('irtt', 'strictstart')
-        # sloppy impulse mode (aka auto timing)
-        self.autoimpulse = cr.get_bool('irtt', 'autoimpulse')
-        # count of finish passings to set finish time
-        self.totlaps = cr.get_posint('irtt', 'totlaps', None)
         if self.totlaps is not None:
             if self.totlaps > 1:
                 _log.debug('Set default target laps: %d', self.totlaps)
             else:
                 _log.debug('Invalid target lap count (%d) ignored',
                            self.totlaps)
                 self.totlaps = None
-        # hide timer panes (for auto-timed setup)
-        self.hidetimers = cr.get_bool('irtt', 'hidetimers')
-        if self.hidetimers:
+
+        # hide timer panes
+        if not self.showtimers:
             self.timerframe.hide()
 
         # transponder timing options
-        self.startloop = strops.chan2id(cr.get('irtt', 'startloop'))
-        if self.startloop < 0:
-            _log.warning('Invalid start loop channel ignored')
-            self.startloop = None
-        self.finishloop = strops.chan2id(cr.get('irtt', 'finishloop'))
-        if self.finishloop < 0:
-            _log.warning('Invalid finish loop channel ignored')
-            self.finishloop = None
         if self.startloop is not None or self.finishloop is not None:
             if self.autoimpulse:
                 configok = True
                 if self.startloop is None or self.finishloop is None:
                     _log.error(
                         'Invalid timing mode: autoimpulse=%r, startloop=%r, finishloop=%r',
                         self.autoimpulse, self.startloop, self.finishloop)
@@ -673,26 +632,25 @@
                 # timing is set by transponder passing time
                 self.precision = 1
                 _log.debug(
                     'Transponder timing mode, precision set to 1: startloop=%r finishloop=%r, autoimpulse=%r',
                     self.startloop, self.finishloop, self.autoimpulse)
 
         # load intermediate split schema
-        self.showinter = strops.confopt_posint(cr.get('irtt', 'showinter'),
-                                               None)
-        self.ischem[COL_INTERA] = unjsob(cr.get('irtt', 'intera'))
-        self.ischem[COL_INTERB] = unjsob(cr.get('irtt', 'interb'))
-        self.ischem[COL_INTERC] = unjsob(cr.get('irtt', 'interc'))
-        self.ischem[COL_INTERD] = unjsob(cr.get('irtt', 'interd'))
-        self.ischem[COL_INTERE] = unjsob(cr.get('irtt', 'intere'))
+        self.showinter = cr.get_posint('irtt', 'showinter', None)
+        self.ischem[COL_INTERA] = cr.get('irtt', 'intera')
+        self.ischem[COL_INTERB] = cr.get('irtt', 'interb')
+        self.ischem[COL_INTERC] = cr.get('irtt', 'interc')
+        self.ischem[COL_INTERD] = cr.get('irtt', 'interd')
+        self.ischem[COL_INTERE] = cr.get('irtt', 'intere')
         self.interloops = cr.get('irtt', 'interloops')
         self.interlaps = cr.get('irtt', 'interlaps')
 
         # load _result_ categories
-        self.loadcats(cr.get('irtt', 'categories'))
+        self.loadcats(cr.get_value('irtt', 'categories').upper().split())
 
         # add the category result and inter holders
         for cat in self.cats:
             self.results[cat] = tod.todlist(cat)
             self.inters[COL_INTERA][cat] = tod.todlist(cat)
             self.inters[COL_INTERB][cat] = tod.todlist(cat)
             self.inters[COL_INTERC][cat] = tod.todlist(cat)
@@ -701,19 +659,19 @@
 
         # pre-load lap targets
         self.load_cat_data()
 
         # restore stage inters, points and bonuses
         self.loadstageinters(cr, 'irtt')
 
-        # re-join any existing timer state -> no, just do a start
-        self.set_syncstart(tod.mktod(cr.get('irtt', 'start')),
-                           tod.mktod(cr.get('irtt', 'lstart')))
+        # set master reference time
+        self.set_syncstart(cr.get_tod('irtt', 'start'),
+                           cr.get_tod('irtt', 'lstart'))
 
-        # re-load starters/results
+        # re-load starters/results - note this does not support lookup
         self.onestart = False
         for rs in cr.get('irtt', 'startlist').split():
             (r, s) = strops.bibstr2bibser(rs)
             i = self.addrider(r, s)
             nr = Gtk.TreeModelRow(self.riders, i)
             wst = None
             tst = None
@@ -721,17 +679,18 @@
             pt = None
             ima = None
             imb = None
             imc = None
             imd = None
             ime = None
             lpass = None
+            seed = 0
             pcnt = 0
             if cr.has_option('riders', rs):
-                # bbb.sss = comment,wall_start,timy_start,finish,penalty,place
+                # bbb.sss = comment,wall_start,...
                 ril = cr.get('riders', rs)  # vec
                 lr = len(ril)
                 if lr > 0:
                     nr[COL_COMMENT] = ril[0]
                 if lr > 1:
                     wst = tod.mktod(ril[1])
                 if lr > 2:
@@ -750,137 +709,111 @@
                     imd = tod.mktod(ril[9])
                 if lr > 10:
                     ime = tod.mktod(ril[10])
                 if lr > 11:
                     pcnt = strops.confopt_posint(ril[11])
                 if lr > 12:
                     lpass = tod.mktod(ril[12])
+                if lr > 13:
+                    seed = strops.confopt_posint(ril[13])
             nri = i
             self.settimes(nri, wst, tst, ft, pt, doplaces=False)
             self.setpasses(nri, pcnt)
             self.setinter(nri, ima, COL_INTERA)
             self.setinter(nri, imb, COL_INTERB)
             self.setinter(nri, imc, COL_INTERC)
             self.setinter(nri, imd, COL_INTERD)
             self.setinter(nri, ime, COL_INTERE)
             self.riders.set_value(nri, COL_LASTSEEN, lpass)
+            self.riders.set_value(nri, COL_SEED, seed)
             # record any extra bonus/penalty to rider model
             if cr.has_option('stagebonus', rs):
-                nr[COL_BONUS] = tod.mktod(cr.get('stagebonus', rs))
+                nr[COL_BONUS] = cr.get_tod('stagebonus', rs)
             if cr.has_option('stagepenalty', rs):
-                nr[COL_PENALTY] = tod.mktod(cr.get('stagepenalty', rs))
+                nr[COL_PENALTY] = cr.get_tod('stagepenalty', rs)
 
         self.startpasses.clear()
         fp = cr.get('irtt', 'startpasses')
         if isinstance(fp, list):
-            for p in fp:
-                t = tod.mktod(p)
-                if t is not None:
-                    self.startpasses.insert(t, prec=4)
+            for t in fp:
+                self.startpasses.insert(t)
 
         self.finishpasses.clear()
         fp = cr.get('irtt', 'finishpasses')
         if isinstance(fp, list):
-            for p in fp:
-                t = tod.mktod(p)
-                if t is not None:
-                    self.finishpasses.insert(t, prec=4)
+            for t in fp:
+                self.finishpasses.insert(t)
 
         # display config
         startmode = 'Relaxed'
         if self.strictstart:
             startmode = 'Strict'
         timingmode = 'Armed'
         if self.autoimpulse:
             timingmode = 'Auto'
         elif self.finishloop is not None or self.startloop is not None:
             timingmode = 'Transponder'
         _log.info(
             'Start mode: %s; Timing mode: %s; Precision: %d; Default Laps: %r',
             startmode, timingmode, self.precision, self.totlaps)
 
-        # recalculate rankings
-        self.recalculate()
-
-        self.comment = cr.get('irtt', 'comment')
-        self.arrivaltimeout = tod.mktod(cr.get('irtt', 'arrivaltimeout'))
-
-        if strops.confopt_bool(cr.get('irtt', 'finished')):
+        self.decisions = cr.get('irtt', 'decisions')
+        if cr.get_bool('irtt', 'finished'):
             self.set_finished()
-        self.onestartlist = strops.confopt_bool(cr.get('irtt', 'onestartlist'))
+        self.recalculate()
 
-        # After load complete - check config and report. This ensures
-        # an error message is left on top of status stack. This is not
-        # always a hard fail and the user should be left to determine
-        # an appropriate outcome.
-        eid = cr.get('irtt', 'id')
-        if eid and eid != EVENT_ID:
+        # After load complete - check config and report.
+        eid = cr.get_value('irtt', 'id')
+        if eid is not None and eid != EVENT_ID:
             _log.info('Event config mismatch: %r != %r', eid, EVENT_ID)
             self.readonly = True
 
     def saveconfig(self):
         """Save race to disk."""
         if self.readonly:
             _log.error('Attempt to save readonly event')
             return
         cw = jsonconfig.config()
-        cw.add_section('irtt')
-        if self.start is not None:
-            cw.set('irtt', 'start', self.start.rawtime())
-        if self.lstart is not None:
-            cw.set('irtt', 'lstart', self.lstart.rawtime())
-        cw.set('irtt', 'comment', self.comment)
-        if self.startgap is not None:
-            cw.set('irtt', 'startgap', self.startgap.rawtime(0))
-        else:
-            cw.set('irtt', 'startgap', None)
-        if self.minlap is not None:
-            cw.set('irtt', 'minlap', self.minlap.rawtime())
-        else:
-            cw.set('irtt', 'minlap', None)
-        if self.arrivaltimeout is not None:
-            cw.set('irtt', 'arrivaltimeout', self.arrivaltimeout.rawtime())
-        else:
-            cw.set('irtt', 'arrivaltimeout', None)
+        cw.add_section('irtt', _CONFIG_SCHEMA)
+        cw.import_section('irtt', self)
+        cw.set('irtt', 'start', self.start)
+        cw.set('irtt', 'lstart', self.lstart)
+        cw.set('irtt', 'decisions', self.decisions)
 
+        # preserve timer info in finish and start passes
         fp = []
         for t in self.startpasses:
-            fp.append(t[0].rawtime(5))
+            fp.append(tod.tod(t[0]))
         cw.set('irtt', 'startpasses', fp)
         fp = []
         for t in self.finishpasses:
-            fp.append(t[0].rawtime(5))
+            fp.append(tod.tod(t[0]))
         cw.set('irtt', 'finishpasses', fp)
 
-        cw.set('irtt', 'strictstart', self.strictstart)
-        cw.set('irtt', 'autoimpulse', self.autoimpulse)
-        cw.set('irtt', 'autoexport', self.autoexport)
-        cw.set('irtt', 'startloop', self.startloop)
-        cw.set('irtt', 'finishloop', self.finishloop)
-        cw.set('irtt', 'totlaps', self.totlaps)
-        cw.set('irtt', 'onestartlist', self.onestartlist)
-        cw.set('irtt', 'precision', self.precision)
-        cw.set('irtt', 'timelimit', self.timelimit)
-        cw.set('irtt', 'hidetimers', self.hidetimers)
+        # deprecated inters - save with config for now
         cw.set('irtt', 'interloops', self.interloops)
         cw.set('irtt', 'interlaps', self.interlaps)
         cw.set('irtt', 'showinter', self.showinter)
-        cw.set('irtt', 'intera', jsob(self.ischem[COL_INTERA]))
+        cw.set('irtt', 'intera', self.ischem[COL_INTERA])
+        cw.set('irtt', 'interb', self.ischem[COL_INTERB])
+        cw.set('irtt', 'interc', self.ischem[COL_INTERC])
+        cw.set('irtt', 'interd', self.ischem[COL_INTERD])
+        cw.set('irtt', 'intere', self.ischem[COL_INTERE])
 
         # save stage inters, points and bonuses
         self.savestageinters(cw, 'irtt')
 
         # save riders
         cw.add_section('stagebonus')
         cw.add_section('stagepenalty')
         cw.set('irtt', 'startlist', self.get_startlist())
         if self.autocats:
-            cw.set('irtt', 'categories', ['AUTO'])
+            cw.set('irtt', 'categories', 'AUTO')
         else:
-            cw.set('irtt', 'categories', self.get_catlist())
+            cw.set('irtt', 'categories', ' '.join(self.get_catlist()).strip())
         cw.add_section('riders')
         for r in self.riders:
             if r[COL_BIB] != '':
                 bib = r[COL_BIB]
                 ser = r[COL_SERIES]
                 bs = strops.bibser2bibstr(bib, ser)
                 # place is saved for info only
@@ -915,21 +848,21 @@
                 if r[COL_PASS] is not None:
                     pcnt = str(r[COL_PASS])
                 lpass = ''
                 if r[COL_LASTSEEN] is not None:
                     lpass = r[COL_LASTSEEN].rawtime()
                 slice = [
                     r[COL_COMMENT], wst, tst, tft, tpt, r[COL_PLACE], tima,
-                    timb, timc, timd, tine, pcnt, lpass
+                    timb, timc, timd, tine, pcnt, lpass, r[COL_SEED]
                 ]
                 cw.set('riders', bs, slice)
                 if r[COL_BONUS] is not None:
-                    cw.set('stagebonus', bs, r[COL_BONUS].rawtime())
+                    cw.set('stagebonus', bs, r[COL_BONUS])
                 if r[COL_PENALTY] is not None:
-                    cw.set('stagepenalty', bs, r[COL_PENALTY].rawtime())
+                    cw.set('stagepenalty', bs, r[COL_PENALTY])
 
         cw.set('irtt', 'finished', self.timerstat == 'finished')
         cw.set('irtt', 'id', EVENT_ID)
         _log.debug('Saving event config %r', self.configfile)
         with metarace.savefile(self.configfile) as f:
             cw.write(f)
 
@@ -1022,15 +955,14 @@
         if self.onestartlist:
             for rc in self.get_catlist():
                 dbr = self.meet.rdb.get_rider(rc, 'cat')
                 if dbr is not None:
                     cname = dbr['title']
                     if cname:
                         catnamecache[rc] = cname
-        """Return a startlist report (rough style)."""
         ret = []
         sec = report.rttstartlist('startlist')
         sec.heading = 'Start Order'
         if catname:
             sec.heading += ': ' + catname
             sec.subheading = subhead
         rcnt = 0
@@ -1064,26 +996,30 @@
                     lt = r[COL_WALLSTART]
                 cstr = None
                 if self.onestartlist and pricat != cat:
                     cstr = pricat
                     if cstr in catnamecache and len(catnamecache[cstr]) < 8:
                         cstr = catnamecache[cstr]
                 sec.lines.append([stxt, bstr, name, ucicode, '____', cstr])
-                if cstr in ['MB', 'WB']:
+                if cstr in ('MB', 'WB'):
                     # lookup pilot - series lookup
                     dbr = self.meet.rdb.get_rider(r[COL_BIB], 'pilot')
                     if dbr is not None:
                         puci = dbr['uci id']
                         pnam = dbr.listname()
                         sec.lines.append(['', '', pnam, puci, '', 'pilot'])
 
-        ret.append(sec)
+        fvc = []
+        if footer:
+            fvc.append(footer)
         if rcnt > 1:
-            sec = report.bullet_text('ridercnt')
-            sec.lines.append(['', 'Total riders: ' + str(rcnt)])
+            fvc.append('Total riders: ' + str(rcnt))
+        if fvc:
+            sec.footer = '\t'.join(fvc)
+        if cat or len(sec.lines) > 0 or len(self.cats) < 2:
             ret.append(sec)
         return ret
 
     def arrival_report(self):
         """Return an arrival report."""
         # build aux table
         aux = []
@@ -1110,15 +1046,15 @@
                 ## only show for a short while
                 to = self.arrivaltimeout
                 if to is None:
                     to = ARRIVALTIMEOUT
                 until = r[COL_TODFINISH] + to
                 if nowtime < until:
                     rarr = r[COL_TODFINISH]
-                    et = self.lrgetelapsed(r)
+                    et = self.getelapsed(r.iter)
                     reta = et
                     ets = et.rawtime(self.precision)
                     rankstr = '(' + plstr + '.)'
                     #speedstr = ''
                     # cat distance should override this
                     #if self.meet.distance is not None:
                     #speedstr = et.speedstr(1000.0 * self.meet.distance)
@@ -1190,15 +1126,14 @@
             sec.lines.append(hr)
         ret = []
         ret.append(sec)
         return ret
 
     def analysis_report(self):
         """Return judges report."""
-        # TODO: return info on splits and speeds with result links
         return self.camera_report()
 
     def camera_report(self):
         """Return a judges report."""
 
         # build aux table
         aux = []
@@ -1223,15 +1158,15 @@
                     sts = r[COL_WALLSTART].rawtime(0) + '   '
                 fts = '-'
                 ft = tod.MAX
                 if r[COL_TODFINISH] is not None:
                     ft = r[COL_TODFINISH]
                     fts = r[COL_TODFINISH].rawtime(2)
 
-                et = self.lrgetelapsed(r)
+                et = self.getelapsed(r.iter)
                 ets = '-'
                 unplaced = False
                 if et is not None:
                     ets = et.rawtime(self.precision)
                 elif r[COL_COMMENT] != '':
                     rkstr = r[COL_COMMENT]
                     unplaced = True
@@ -1256,38 +1191,42 @@
                 sec.lines.append([None, None, None])
         ret = []
         if len(sec.lines) > 0:
             ret.append(sec)
         return ret
 
     def single_catresult(self, cat=''):
+        _log.debug('Cat result for cat=%r', cat)
         ret = []
         allin = False
         catname = cat
+        secid = 'result'
         if cat == '':
             if len(self.cats) > 1:
                 catname = 'Uncategorised Riders'
             else:
                 # There is only one cat - so all riders are in it
                 allin = True
+        else:
+            secid = 'result-' + cat.lower()
         subhead = ''
         footer = ''
         distance = self.meet.distance  # fall on meet dist
         dbr = self.meet.rdb.get_rider(cat, 'cat')
         if dbr is not None:
             catname = dbr['title']
             subhead = dbr['subtitle']
             footer = dbr['fooer']
             dist = dbr['distance']
             if dist:
                 try:
                     distance = float(dist)
                 except Exception:
                     _log.warning('Invalid distance %r for cat %r', dist, cat)
-        sec = report.section('result-' + cat)
+        sec = report.section(secid)
         ct = None
         lt = None
         lpstr = None
         totcount = 0
         dnscount = 0
         dnfcount = 0
         hdcount = 0
@@ -1300,23 +1239,24 @@
             incat = False
             if allin or (cat and cat in rcats):
                 incat = True  # rider is in this category
             elif not cat:  # is the rider uncategorised?
                 if rcats[0] == '':
                     incat = True
                 else:
-                    incat = rcats[0] not in self.cats  # backward logic
+                    # exclude properly categorised riders
+                    incat = rcats[0] not in self.cats
             if incat:
                 if cat:
                     rcat = cat
                 else:
                     rcat = rcats[0]  # (work-around mis-categorised rider)
                 placed = False
                 totcount += 1
-                ft = self.lrgetelapsed(r)
+                ft = self.getelapsed(r.iter)
                 bstr = r[COL_BIB]
                 nstr = r[COL_NAMESTR]
                 cstr = ''
                 if cat == '':  # categorised result does not need cat
                     cstr = rcat
                 dbr = self.meet.rdb.get_rider(bstr, self.series)
                 if dbr is not None:
@@ -1349,41 +1289,44 @@
                 if ft is not None:
                     tstr = ft.rawtime(self.precision)
                 dstr = None
                 if ct is not None and ft is not None and ct != ft:
                     dstr = '+' + (ft - ct).rawtime(1)
                 if placed:
                     sec.lines.append([pstr, bstr, nstr, cstr, tstr, dstr])
-                    if cat in ['WB', 'MB']:  #also look up pilots
+                    if cat in ('WB', 'MB'):  #also look up pilots
                         # lookup pilot - series lookup
                         dbr = self.meet.rdb.get_rider(r[COL_BIB], 'pilot')
                         if dbr is not None:
                             puci = dbr['uci id']
                             pnam = dbr.listname()
                             sec.lines.append(['', 'pilot', pnam, puci, '', ''])
 
         residual = totcount - (fincount + dnfcount + dnscount + hdcount)
 
-        if self.timerstat == 'finished':  # THIS OVERRIDES RESIDUAL
+        if self.timerstat == 'finished':
             sec.heading = 'Result'
         else:
             if self.racestat == 'prerace':
-                sec.heading = ''  # anything better?
+                sec.heading = 'Result'
             else:
                 if residual > 0:
                     sec.heading = 'Standings'
                 else:
                     sec.heading = 'Provisional Result'
 
-        # Append all result categories and uncat if riders
-        if cat or totcount > 0:
+        # Append all result categories and uncat if appropriate
+        if cat or totcount > 0 or len(self.cats) < 2:
             ret.append(sec)
             rsec = sec
             # Race metadata / UCI comments
-            sec = report.bullet_text('uci' + cat)
+            secid = 'resultmeta'
+            if cat:
+                secid = 'resultmeta-' + cat.lower()
+            sec = report.bullet_text(secid)
             if ct is not None:
                 if distance is not None:
                     avgprompt = 'Average speed of the winner: '
                     if residual > 0:
                         avgprompt = 'Average speed of the leader: '
                     sec.lines.append(
                         [None, avgprompt + ct.speedstr(1000.0 * distance)])
@@ -1430,20 +1373,17 @@
 
         # show all intermediates here
         for i in self.intermeds:
             im = self.intermap[i]
             if im['places'] and im['show']:
                 ret.extend(self.int_report(i))
 
-        if len(self.comment) > 0:
-            s = report.bullet_text('comms')
-            s.heading = 'Decisions of the commissaires panel'
-            for comment in self.comment:
-                s.lines.append([None, comment])
-            ret.append(s)
+        # append a decisions section
+        ret.append(self.decision_section())
+
         return ret
 
     def startlist_gen(self, cat=''):
         """Generator function to export a startlist."""
         mcat = self.ridercat(cat)
         # order this export by start time as per callup
         self.reorder_callup()
@@ -1487,17 +1427,17 @@
                 if mcat:
                     rcat = mcat
                 else:
                     rcat = rcats[0]
                 bib = r[COL_BIB]
                 ser = r[COL_SERIES]
                 bs = strops.bibser2bibstr(bib, ser)
-                ft = self.lrgetelapsed(r)
+                ft = self.getelapsed(r.iter)
                 if ft is not None:
-                    ft = ft.truncate(self.precision)
+                    ft = ft.round(self.precision)
                 crank = None
                 rank = None
                 if r[COL_PLACE].isdigit():
                     rcount += 1
                     rank = int(r[COL_PLACE])
                     if rank != lrank:
                         crank = rcount
@@ -1793,85 +1733,95 @@
         self._doannounce = True
 
         return False
 
     def timertrig(self, e):
         """Process transponder passing event."""
         chan = strops.chan2id(e.chan)
-        if e.refid in ['', '255']:
-            if self.finishloop is not None and chan == self.finishloop:
+        if e.refid in ('', '255'):
+            if self.finishloop is not None and chan in (self.finishloop, -1):
                 self.fin_trig(e)
-            elif self.startloop is not None and chan == self.startloop:
+            elif self.startloop is not None and chan in (self.startloop, -1):
                 self.start_trig(e)
             else:
                 _log.info('Spurious trigger: %s@%s/%s', e.chan, e.rawtime(2),
                           e.source)
             return False
 
         r = self.meet.getrefid(e.refid)
         if r is None:
             _log.info('Unknown rider: %s:%s@%s/%s', e.refid, e.chan,
                       e.rawtime(2), e.source)
             return False
 
         bib = r['no']
         series = r['series']
+        bibstr = strops.bibser2bibstr(bib, series)
         lr = self.getrider(bib, series)
-        if lr is not None:
-            # distinguish a shared finish / start loop
-            okfin = False
-            st = lr[COL_WALLSTART]
-            if lr[COL_TODSTART] is not None:
-                st = lr[COL_TODSTART]
-            # is e beyond the start threshold?
-            ## TODO: guard e near a recorded start time, handle sloppy
-            ##       start offset properly
-            if st is not None and e > st and e - st > self.minlap:
-                okfin = True
-
-            bibstr = strops.bibser2bibstr(bib, series)
+        if lr is None:
+            if self.clubmode and self.timerstat == 'running':
+                ri = self.addrider(bib, series)
+                lr = Gtk.TreeModelRow(self.riders, ri)
+                _log.info('Added new starter: %s:%s@%s/%s', bibstr, e.chan,
+                          e.rawtime(2), e.source)
+            else:
+                _log.info('Non-starter: %s:%s@%s/%s', bibstr, e.chan,
+                          e.rawtime(2), e.source)
+                return False
 
-            # switch on loop source mode
-            if okfin and self.finishloop is not None and chan == self.finishloop:
-                # this path also handles lap counting rfid modes
-                return self.finish_by_rfid(lr, e, bibstr)
-            elif self.startloop is not None and chan == self.startloop:
-                return self.start_by_rfid(lr, e, bibstr)
-            elif chan in self.interloops:
-                return self.rfidinttrig(lr, e, bibstr, bib, series)
-            elif self.finishloop is not None and chan == self.finishloop:
-                # handle the case where source matches, but timing is off
-                _log.info('Early arrival at finish: %s:%s@%s/%s', bibstr,
+        # distinguish a shared finish / start loop
+        okfin = False
+        st = lr[COL_WALLSTART]
+        if lr[COL_TODSTART] is not None:
+            st = lr[COL_TODSTART]
+        # is e beyond the start threshold?
+        if st is not None and e > st and e - st > self.minlap:
+            okfin = True
+
+        # switch on loop source mode
+        if okfin and self.finishloop is not None and chan in (self.finishloop,
+                                                              -1):
+            # this path also handles lap counting rfid modes
+            return self.finish_by_rfid(lr, e, bibstr)
+        elif self.startloop is not None and chan in (self.startloop, -1):
+            return self.start_by_rfid(lr, e, bibstr)
+        elif chan in self.interloops:
+            return self.rfidinttrig(lr, e, bibstr, bib, series)
+        elif self.finishloop is not None and chan in (self.finishloop, -1):
+            # handle the case where source matches, but timing is off
+            _log.info('Early arrival at finish: %s:%s@%s/%s', bibstr, e.chan,
+                      e.rawtime(2), e.source)
+            return False
+        else:
+            # match not found for the passing
+            if self.finishloop is not None or self.startloop is not None:
+                _log.info('No match found for passing: %s:%s@%s/%s', bibstr,
                           e.chan, e.rawtime(2), e.source)
                 return False
 
-            if lr[COL_TODFINISH] is not None:
-                _log.info('Finished rider: %s:%s@%s/%s', bibstr, e.chan,
-                          e.rawtime(2), e.source)
-                return False
+        if lr[COL_TODFINISH] is not None:
+            _log.info('Finished rider: %s:%s@%s/%s', bibstr, e.chan,
+                      e.rawtime(2), e.source)
+            return False
 
-            if self.fl.getstatus() not in ['armfin']:
-                st = lr[COL_WALLSTART]
-                if lr[COL_TODSTART] is not None:
-                    st = lr[COL_TODSTART]
-                if st is not None and e > st and e - st > self.minlap:
-                    self.fl.setrider(lr[COL_BIB], lr[COL_SERIES])
-                    self.armfinish()
-                    _log.info('Arm finish: %s:%s@%s/%s', bibstr, e.chan,
-                              e.rawtime(2), e.source)
-                else:
-                    _log.info('Early arrival at finish: %s:%s@%s/%s', bibstr,
-                              e.chan, e.rawtime(2), e.source)
-            else:
-                _log.info('Finish blocked: %s:%s@%s/%s', bibstr, e.chan,
+        if self.fl.getstatus() != 'armfin':
+            st = lr[COL_WALLSTART]
+            if lr[COL_TODSTART] is not None:
+                st = lr[COL_TODSTART]
+            if st is not None and e > st and e - st > self.minlap:
+                self.fl.setrider(lr[COL_BIB], lr[COL_SERIES])
+                self.armfinish()
+                _log.info('Arm finish: %s:%s@%s/%s', bibstr, e.chan,
                           e.rawtime(2), e.source)
+            else:
+                _log.info('Early arrival at finish: %s:%s@%s/%s', bibstr,
+                          e.chan, e.rawtime(2), e.source)
         else:
-            _log.info('Non-starter: %s:%s@%s/%s', bibstr, e.chan, e.rawtime(2),
-                      e.source)
-        return False
+            _log.info('Finish blocked: %s:%s@%s/%s', bibstr, e.chan,
+                      e.rawtime(2), e.source)
 
     def int_trig(self, t):
         """Register intermediate trigger."""
         _log.info('Intermediate cell: %s', t.rawtime(2))
 
     def fin_trig(self, t):
         """Register finish trigger."""
@@ -1907,15 +1857,15 @@
 
                 else:
                     _log.error('Missing rider at finish')
                     self.sl.toidle()
                 # flag announce
                 self._doannounce = True
             # save passing to start passing store
-            self.finishpasses.insert(t, prec=4)
+            self.finishpasses.insert(t)
         elif self.timerstat == 'armstart':
             self.set_syncstart(t)
 
     def start_trig(self, t):
         """Register start trigger."""
         _log.info('Start trigger %s@%s/%s', t.chan, t.rawtime(4), t.source)
         if self.timerstat == 'running':
@@ -1926,15 +1876,15 @@
                 if i is not None:
                     self.settimes(i, tst=t, doplaces=False)
                     self.sl.torunning()
                 else:
                     _log.error('Missing rider at start')
                     self.sl.toidle()
             # save passing to start passing store
-            self.startpasses.insert(t, prec=4)
+            self.startpasses.insert(t)
         elif self.timerstat == 'armstart':
             self.set_syncstart(t, tod.now())
 
     def alttimertrig(self, e):
         """Handle chronometer callbacks."""
         # note: these impulses are sourced from alttimer device and keyboard
         #       transponder triggers are collected separately in timertrig()
@@ -1975,28 +1925,28 @@
             self.recalculate()
             if self.autoexport:
                 GLib.idle_add(self.meet.menu_data_results_cb, None)
 
         if self.timerstat == 'running':
             nowoft = (tod.now() - self.lstart).truncate(0)
 
-            # auto load/clear start lane if not in sloppy impulse mode
-            if not self.autoimpulse:
-                if self.sl.getstatus() in ['idle', 'load']:
+            # auto load/clear start lane if start loop is not set
+            if self.startloop is None:
+                if self.sl.getstatus() in ('idle', 'load'):
                     if nowoft.timeval % 5 == 0:  # every five
                         self.on_start(nowoft)
                 else:
                     if nowoft == self.start_unload:
                         self.sl.toidle()
 
-            # after manips, then re-set start time
-            self.sl.set_time(nowoft.timestr(0))
+                # after manips, then re-set start time
+                self.sl.set_time(nowoft.timestr(0))
 
             # if finish lane loaded, set the elapsed time
-            if self.fl.getstatus() in ['load', 'running', 'armfin']:
+            if self.fl.getstatus() in ('load', 'running', 'armfin'):
                 bib = self.fl.bibent.get_text()
                 series = self.fl.serent.get_text()
                 i = self.getiter(bib, series)
                 if i is not None:
                     et = self.getelapsed(i, runtime=True)
                     self.fl.set_time(et.timestr(0))
                     self.announce_rider('',
@@ -2056,48 +2006,56 @@
         """Edit event specifics."""
 
         # flatten current cat list
         _CONFIG_SCHEMA['categories']['value'] = ' '.join(
             self.get_catlist()).strip()
         res = uiutil.options_dlg(window=self.meet.window,
                                  title='Event Properties',
-                                 schema=_CONFIG_SCHEMA,
-                                 obj=self)
+                                 sections={
+                                     'event': {
+                                         'title': 'Event',
+                                         'schema': _CONFIG_SCHEMA,
+                                         'object': self,
+                                     },
+                                 })
         # handle a change in result categories
-        if res['categories'][0]:
-            self.loadcats(res['categories'][2].split())
+        if res['event']['categories'][0]:
+            self.loadcats(res['event']['categories'][2].upper().split())
 
         # flag reload for anything that may change result lists
         ret = False
         for k in ('categories', 'autoimpulse', 'startloop', 'finishloop',
                   'strictstart'):
-            if res[k][0]:
+            if res['event'][k][0]:
                 ret = True
                 break
 
         return ret
 
     def starttime(self, start=None, bib='', series=''):
         """Adjust start time for the rider."""
         r = self.getrider(bib, series)
         if r is not None:
             r[COL_WALLSTART] = start
+            _log.debug('Set start time for %s: %s',
+                       strops.bibser2bibstr(bib, series), start.rawtime(0))
             #self.unstart(bib, series, wst=start)
 
     def delrider(self, bib='', series=''):
-        """Delete the specificed rider from the race model."""
+        """Delete the specified rider from the race model."""
         i = self.getiter(bib, series)
         if i is not None:
+            self.settimes(i)
             self.riders.remove(i)
+        if (bib, series) in self.ridernos:
             self.ridernos.remove((bib, series))
 
     def addrider(self, bib='', series=''):
         """Add specified rider to race model."""
         if bib and (bib, series) in self.ridernos:
-            _log.warning('Rider %r.%r already in viewmodel', bib)
             return None
 
         if bib:
             nr = [
                 bib, '', '', '', '', True, '', 0, 0, None, None, None,
                 tod.ZERO, None, None, None, None, None, None, None, None, None,
                 0, 0, series
@@ -2147,19 +2105,19 @@
         """Update the local record lr with data from riderdb handle r"""
         lr[COL_NAMESTR] = r.listname()
         lr[COL_CAT] = r['cat']
         lr[COL_SHORTNAME] = r.fitname(24)
 
     def info_time_edit_clicked_cb(self, button, data=None):
         """Toggle the visibility of timer panes"""
-        self.hidetimers = not self.hidetimers
-        if self.hidetimers:
-            self.timerframe.hide()
-        else:
+        self.showtimers = not self.showtimers
+        if self.showtimers:
             self.timerframe.show()
+        else:
+            self.timerframe.hide()
 
     def editcol_cb(self, cell, path, new_text, col):
         """Update value in edited cell."""
         new_text = new_text.strip()
         if col == COL_PASS:
             if new_text.isdigit():
                 self.riders[path][COL_PASS] = int(new_text)
@@ -2219,15 +2177,15 @@
                     _log.error('Extra result for rider %r', np)
 
         # check counts for racestat
         self.racestat = 'prerace'
         fullcnt = len(self.riders)
         placed = 0
         for r in self.riders:
-            if r[COL_PLACE] and r[COL_PLACE] in ['dns', 'dnf', 'dsq']:
+            if r[COL_PLACE] and r[COL_PLACE] in ('dns', 'dnf', 'dsq'):
                 r[COL_ETA] = None
             else:
                 i = r.iter
                 r[COL_ETA] = self.geteta(i)
             if r[COL_PLACE]:
                 placed += 1
         _log.debug('placed = ' + str(placed) + ', total = ' + str(fullcnt))
@@ -2242,17 +2200,14 @@
                     self.racestat = 'provisional'
         _log.debug('Racestat set to: ' + repr(self.racestat))
 
         # compute any intermediates
         for c in self.contests:
             self.assign_places(c)
 
-        # re-order view
-        # todo
-
         return False
 
     def get_placelist(self):
         """Return place list."""
         # assume this follows a place sorting.
         fp = None
         ret = ''
@@ -2286,15 +2241,15 @@
                 allpts = points[0]
             if len(bonuses) > 0:
                 allbonus = bonuses[0]
         placestr = ''
         if src == 'fin':
             placestr = self.get_placelist()
             _log.info('Using placestr %r', placestr)
-            if tally in ['sprint', 'crit']:  # really only for sprints/crits
+            if tally in ('sprint', 'crit'):  # really only for sprints/crits
                 countbackwinner = True
         elif src == 'reg':
             placestr = self.get_startlist()
         elif src == 'start':
             placestr = self.get_starters()
         else:
             placestr = self.intermap[src]['places']
@@ -2400,22 +2355,22 @@
         res.remove(bib, series)
 
         # save intermed tod to rider model
         self.riders.set_value(iter, inter, imed)
         tst = self.riders.get_value(iter, COL_TODSTART)
         wst = self.riders.get_value(iter, COL_WALLSTART)
 
-        # determine start time
+        # if started, return rank at inter
         if imed is not None:
-            if tst is not None:  # got a start trigger
-                res.insert(imed - tst, None, bib, series)
-                ret = res.rank(bib, series)
-            elif wst is not None:  # start on wall time
-                res.insert(imed - wst, None, bib, series)
-                ret = res.rank(bib, series)
+            if tst is not None:
+                ret = res.insert((imed - tst).round(self.precision), None, bib,
+                                 series)
+            elif wst is not None:
+                ret = res.insert((imed - wst).round(self.precision), None, bib,
+                                 series)
             else:
                 _log.error('No start time for intermediate ' +
                            strops.bibser2bibstr(bib, series))
         return ret
 
     def setpasses(self, iter, passes=None):
         """Set rider pass count."""
@@ -2454,27 +2409,25 @@
             self.riders.set_value(iter, COL_TODPENALTY, pt)
         else:
             pt = self.riders.get_value(iter, COL_TODPENALTY)
 
         # save result
         if tft is not None:
             self.onestart = True
-            if tst is not None:  # got a start trigger
+            if tst is not None:
                 self.results[cat].insert(
-                    (tft - tst).truncate(self.precision) + pt, None, bib,
-                    series)
-            elif wst is not None:  # start on wall time
+                    (tft - tst).round(self.precision) + pt, None, bib, series)
+            elif wst is not None:
                 self.results[cat].insert(
-                    (tft - wst).truncate(self.precision) + pt, None, bib,
-                    series)
+                    (tft - wst).round(self.precision) + pt, None, bib, series)
             else:
                 _log.error('No start time for rider ' +
                            strops.bibser2bibstr(bib, series))
         elif tst is not None:
-            #self.oncourse(bib, series)	# started but not finished
+            # started but not finished
             pass
 
         # if reqd, do places
         if doplaces and oft != tft:
             self._dorecalc = True
             self._doannounce = True
 
@@ -2491,15 +2444,15 @@
         """Manually register a finish time."""
         thetime = tod.mktod(entry.get_text())
         if thetime is not None:
             bib = tp.bibent.get_text().strip()
             series = tp.serent.get_text().strip()
             if bib != '':
                 self.armfinish()
-                self.meet.alttimer.trig(thetime, chan=1, index='MANU')
+                self.meet._alttimer.trig(thetime, chan=1, index='MANU')
                 entry.set_text('')
                 tp.grab_focus()
         else:
             _log.error('Invalid finish time.')
 
     def lanelookup(self, bib=None, series=''):
         """Prepare name string for timer lane."""
@@ -2558,17 +2511,20 @@
     def tod_context_rel_activate_cb(self, menuitem, data=None):
         """Relegate rider."""
         _log.info('Relegate not implemented for time trial.')
         pass
 
     def tod_context_ntr_activate_cb(self, menuitem, data=None):
         """Register no time recorded for rider and place last."""
-        ## TODO
-        _log.info('NTR not implemented for time trial.')
-        pass
+        sel = self.view.get_selection().get_selected()
+        if sel is not None:
+            i = sel[1]  # grab off row iter
+            bib = self.riders.get_value(i, COL_BIB)
+            series = self.riders.get_value(i, COL_SERIES)
+            self.dnfriders(strops.bibser2bibstr(bib, series), 'ntr')
 
     def tod_context_clear_activate_cb(self, menuitem, data=None):
         """Clear times for selected rider."""
         sel = self.view.get_selection().get_selected()
         if sel is not None:
             self.riders.set_value(sel[1], COL_COMMENT, '')
             self.riders.set_value(sel[1], COL_PASS, 0)
@@ -2578,135 +2534,257 @@
 
     def now_button_clicked_cb(self, button, entry=None):
         """Set specified entry to the current time."""
         if entry is not None:
             entry.set_text(tod.now().timestr())
 
     def tod_context_edit_activate_cb(self, menuitem, data=None):
-        """Run edit time dialog."""
+        """Edit rider start/finish/etc."""
         sel = self.view.get_selection().get_selected()
-        if sel is not None:
-            i = sel[1]  # grab off row iter and read in cur times
-            tst = self.riders.get_value(i, COL_TODSTART)
-            tft = self.riders.get_value(i, COL_TODFINISH)
-            tpt = self.riders.get_value(i, COL_TODPENALTY)
+        if sel is None:
+            return False
 
-            # prepare text entry boxes
-            st = ''
-            if tst is not None:
-                st = tst.timestr()
-            ft = ''
-            if tft is not None:
-                ft = tft.timestr()
-            bt = ''
-            pt = '0'
-            if tpt is not None:
-                pt = tpt.timestr()
-
-            # run the dialog
-            (ret, st, ft, bt, pt) = uiutil.edit_times_dlg(self.meet.window,
-                                                          st,
-                                                          ft,
-                                                          bt,
-                                                          pt,
-                                                          bonus=False,
-                                                          penalty=True)
-            if ret == 1:
-                stod = tod.mktod(st)
-                ftod = tod.mktod(ft)
-                ptod = tod.mktod(pt)
-                if ptod is None:
-                    ptod = tod.ZERO
-                bib = self.riders.get_value(i, COL_BIB)
-                series = self.riders.get_value(i, COL_SERIES)
-                self.settimes(i, tst=stod, tft=ftod, pt=ptod)  # update model
-                _log.info('Race times manually adjusted for rider ' +
-                          strops.bibser2bibstr(bib, series))
-            else:
-                _log.info('Edit race times cancelled.')
+        lr = Gtk.TreeModelRow(self.riders, sel[1])
+        bibstr = strops.bibser2bibstr(lr[COL_BIB], lr[COL_SERIES])
+        placestr = ''
+        placeopts = {
+            '': ' Not yet classified',
+            'dns': 'Did not start',
+            'otl': 'Outside time limit',
+            'dnf': 'Did not finish',
+            'dsq': 'Disqualified',
+        }
+        if lr[COL_PLACE] and lr[COL_PLACE] not in placeopts:
+            placestr = 'Ranked ' + strops.rank2ord(lr[COL_PLACE])
+        elif lr[COL_PLACE] in placeopts:
+            placestr = placeopts[lr[COL_PLACE]]
+        else:
+            placestr = placeopts['']
+        sections = {
+            'result': {
+                'object': None,
+                'title': 'result',
+                'schema': {
+                    'title': {
+                        'prompt': bibstr + ' ' + lr[COL_NAMESTR],
+                        'control': 'section',
+                    },
+                    'seed': {
+                        'prompt': 'Seed:',
+                        'hint': 'Seeding number for startlists',
+                        'control': 'short',
+                        'type': 'int',
+                        'value': lr[COL_SEED],
+                        'index': COL_SEED,
+                    },
+                    'class': {
+                        'prompt': 'Classification:',
+                        'hint': 'Rider classification for event',
+                        'control': 'label',
+                        'value': placestr,
+                    },
+                    'wallstart': {
+                        'prompt': 'Wall Start:',
+                        'hint': 'Advertised start time',
+                        'type': 'tod',
+                        'places': 0,
+                        'control': 'short',
+                        'value': lr[COL_WALLSTART],
+                        'index': COL_WALLSTART,
+                    },
+                    'laps': {
+                        'prompt': 'Laps:',
+                        'hint': 'Rider lap/passing count',
+                        'control': 'short',
+                        'type': 'int',
+                        'value': lr[COL_PASS],
+                        'index': COL_PASS,
+                    },
+                    'lpass': {
+                        'prompt': 'Last Pass:',
+                        'hint': 'Time last seen on finish loop',
+                        'type': 'tod',
+                        'places': 4,
+                        'readonly': 'true',
+                        'control': 'short',
+                        'value': lr[COL_LASTSEEN],
+                    },
+                    'start': {
+                        'prompt': 'Start:',
+                        'hint': 'Recorded start time',
+                        'type': 'tod',
+                        'places': 4,
+                        'value': lr[COL_TODSTART],
+                        'nowbut': True,
+                        'control': 'short',
+                        'subtext': 'Set start time to now',
+                        'index': COL_TODSTART,
+                    },
+                    'finish': {
+                        'prompt': 'Finish:',
+                        'hint': 'Recorded finish time',
+                        'type': 'tod',
+                        'places': 4,
+                        'value': lr[COL_TODFINISH],
+                        'nowbut': True,
+                        'control': 'short',
+                        'subtext': 'Set finish time to now',
+                        'index': COL_TODFINISH,
+                    },
+                    'evtpenalty': {
+                        'prompt': 'Penalty:',
+                        'hint': 'Event penalty time',
+                        'subtext': 'Applies to ranking',
+                        'type': 'tod',
+                        'places': 0,
+                        'value': lr[COL_TODPENALTY],
+                        'control': 'short',
+                        'default': 0,
+                        'index': COL_TODPENALTY,
+                    },
+                    'bonus': {
+                        'prompt': 'Stage Bonus:',
+                        'hint': 'Additional stage bonus time',
+                        'type': 'tod',
+                        'places': 0,
+                        'value': lr[COL_BONUS],
+                        'control': 'short',
+                        'index': COL_BONUS,
+                    },
+                    'penalty': {
+                        'prompt': 'Stage Penalty:',
+                        'hint': 'Additional stage penalty time',
+                        'type': 'tod',
+                        'places': 0,
+                        'value': lr[COL_PENALTY],
+                        'control': 'short',
+                        'index': COL_PENALTY,
+                    },
+                },
+            },
+        }
+        res = uiutil.options_dlg(window=self.meet.window,
+                                 title='Edit times',
+                                 sections=sections)
+        changed = False
+        dotimes = False
+        for option in res['result']:
+            if res['result'][option][0]:
+                changed = True
+                if 'index' in sections['result']['schema'][option]:
+                    index = sections['result']['schema'][option]['index']
+                    lr[index] = res['result'][option][2]
+                    _log.debug('Updated %s to: %r', option,
+                               res['result'][option][2])
+                    if option in ('wallstart', 'start', 'finish',
+                                  'evtpenalty'):
+                        dotimes = True
+                else:
+                    _log.debug('Unknown option %r changed', option)
+        if dotimes:
+            if lr[COL_TODPENALTY] is None:
+                lr[COL_TODPENALTY] = tod.ZERO
+            self.settimes(lr.iter,
+                          tst=lr[COL_TODSTART],
+                          tft=lr[COL_TODFINISH],
+                          pt=lr[COL_TODPENALTY])
+        if changed:
+            self.recalculate()
 
     def tod_context_del_activate_cb(self, menuitem, data=None):
         """Delete selected row from race model."""
         sel = self.view.get_selection().get_selected()
         if sel is not None:
             i = sel[1]  # grab off row iter
+            bib = self.riders.get_value(i, COL_BIB)
+            series = self.riders.get_value(i, COL_SERIES)
             self.settimes(i)  # clear times
             if self.riders.remove(i):
                 pass  # re-select?
+            if (bib, series) in self.ridernos:
+                self.ridernos.remove((bib, series))
 
     def log_clear(self, bib, series):
         """Print clear time log."""
         _log.info('Time cleared for rider ' +
                   strops.bibser2bibstr(bib, series))
 
     def set_titlestr(self, titlestr=None):
         """Update the title string label."""
         if titlestr is None or titlestr == '':
             titlestr = 'Individual Road Time Trial'
         self.title_namestr.set_text(titlestr)
 
-    def __init__(self, meet, event, ui=True):
+    def __init__(self, meet, etype, ui=True):
         self.meet = meet
-        self.event = event
-        self.evno = event['evid']
+        self.etype = etype
         # series is specified per-rider
         self.series = ''
-        self.configfile = meet.event_configfile(self.evno)
+        self.configfile = 'event.json'
         self.readonly = not ui
         rstr = ''
         if self.readonly:
             rstr = 'readonly '
-        _log.debug('Init %r event %r', rstr, self.evno)
+        _log.debug('Init %r event', rstr)
 
         self.recalclock = threading.Lock()
         self._dorecalc = False
 
         # properties
         self.strictstart = True
         self.autoimpulse = False
         self.autoexport = False
         self.finishloop = None
         self.startloop = None
         self.precision = 2
         self.totlaps = None
-        self.hidetimers = False
+        self.showtimers = False
         self.clubmode = False
+        self.allowspares = False
         self.minlap = STARTFUDGE
         self.arrivaltimeout = ARRIVALTIMEOUT
+        self.timelimit = None
+        self.gapthresh = GAPTHRESH
 
         # race run time attributes
+        self.live_announce = False
+        self.curlap = -1
+        self.onlap = 1
+        self.lapstart = None
+        self.lapfin = None
         self.onestart = False
         self.winopen = True
         self.timerstat = 'idle'
         self.racestat = 'prerace'
         self.start = None
+        self.finish = None
         self.lstart = None
         self.start_unload = None
         self.startgap = None
         self.cats = []  # the ordered list of cats for results
         self.autocats = False
         self.startpasses = tod.todlist('start')
         self.finishpasses = tod.todlist('finish')
         self.results = {'': tod.todlist('UNCAT')}
         self.inters = {}
         self.ischem = {}
         self.showinter = None
-        for im in [COL_INTERA, COL_INTERB, COL_INTERC, COL_INTERD, COL_INTERE]:
+        for im in (COL_INTERA, COL_INTERB, COL_INTERC, COL_INTERD, COL_INTERE):
             self.inters[im] = {'': tod.todlist('UNCAT')}
             self.ischem[im] = None
         self.interloops = {}  # map of loop ids to inter splits
         self.interlaps = {}  # map of lap counts to inter splits
         self.curfintod = None
         self._doannounce = False
         self.onestartlist = False
         self.curcat = ''
         self.catstarts = {}
         self.catplaces = {}
         self.catlaps = {}
-        self.comment = []
+        self.decisions = []
         self.places = ''
 
         self.bonuses = {}
         self.points = {}
         self.pointscb = {}
 
         # stage intermediates
@@ -2766,45 +2844,44 @@
         self.fl.bibent.connect('activate', self.bibent_cb, self.fl)
         self.fl.serent.connect('activate', self.bibent_cb, self.fl)
         self.fl.tment.connect('activate', self.tment_cb, self.fl)
         mf.pack_start(self.sl.frame, True, True, 0)
         mf.pack_start(self.fl.frame, True, True, 0)
         mf.set_focus_chain([self.sl.frame, self.fl.frame, self.sl.frame])
         self.timerframe = mf
+        self.lapentry = Gtk.Label()
+        self.totlapentry = Gtk.Label()
 
         # Result Pane
         t = Gtk.TreeView(self.riders)
         self.view = t
         t.set_reorderable(True)
         t.set_rules_hint(True)
 
         self.context_menu = None
         if ui:
             t.connect('button_press_event', self.treeview_button_press)
-            # TODO: show team name & club but pop up for rider list
             uiutil.mkviewcolbibser(t, bibcol=COL_BIB, sercol=COL_SERIES)
             uiutil.mkviewcoltxt(t, 'Rider', COL_NAMESTR, expand=True)
             uiutil.mkviewcoltxt(t, 'Cat', COL_CAT, self.editcol_cb)
-            uiutil.mkviewcoltxt(t, 'Passes', COL_PASS, self.editcol_cb)
-            # -> Add in start time field with edit!
-            uiutil.mkviewcoltod(t, 'Start', cb=self.wallstartstr)
+            uiutil.mkviewcoltxt(t,
+                                'Pass',
+                                COL_PASS,
+                                self.editcol_cb,
+                                calign=1.0)
+            uiutil.mkviewcoltod(t,
+                                'Start',
+                                cb=self.startstr,
+                                editcb=self.editstart)
             uiutil.mkviewcoltod(t, 'Time', cb=self.elapstr)
             uiutil.mkviewcoltxt(t, 'Rank', COL_PLACE, halign=0.5, calign=0.5)
             t.show()
             b.get_object('race_result_win').add(t)
             b.connect_signals(self)
 
             b = uiutil.builder('tod_context.ui')
             self.context_menu = b.get_object('tod_context')
             b.connect_signals(self)
 
-            # reconfigure the chronometer
-            self.meet.alttimer.armlock()  # lock the arm to capture all hits
-            self.meet.alttimer.arm(0)  # start line
-            self.meet.alttimer.arm(1)  # finish line (primary)
-            self.meet.alttimer.arm(2)  # use for backup trigger a
-            self.meet.alttimer.arm(3)  # use for backup trigger b
-            self.meet.alttimer.delaytime('0.01')
-
             # connect timer callback functions
             self.meet.timercb = self.timertrig  # transponders
             self.meet.alttimercb = self.alttimertrig  # chronometer
```

### Comparing `metarace-roadmeet-1.13.1/src/roadmeet/rms.py` & `metarace-roadmeet-1.13.2/src/roadmeet/rms.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from metarace import riderdb
 from metarace import strops
 from metarace import countback
 from metarace import report
 from metarace import jsonconfig
 from . import uiutil
 
-_log = logging.getLogger('metarace.rms')
+_log = logging.getLogger('rms')
 _log.setLevel(logging.DEBUG)
 
 # Model columns
 
 # basic infos
 COL_BIB = 0
 COL_NAMESTR = 1
@@ -67,45 +67,43 @@
     'cross': 'Cyclocross',
     'irtt': 'Individual Time Trial',
     'trtt': 'Team Time Trial',
 }
 
 # rider commands
 RIDER_COMMANDS_ORD = [
-    'add', 'del', 'que', 'dns', 'otl', 'wd', 'dnf', 'dsq', 'com', 'ret', 'man',
+    'add', 'del', 'que', 'dns', 'otl', 'wd', 'dnf', 'dsq', 'dec', 'ret', 'man',
     '', 'fin'
 ]  # then intermediates...
 RIDER_COMMANDS = {
     'dns': 'Did not start',
     'otl': 'Outside time limit',
     'dnf': 'Did not finish',
     'wd': 'Withdraw',
     'dsq': 'Disqualify',
     'add': 'Add starters',
     'del': 'Remove starters',
     'que': 'Query riders',
     'fin': 'Final places',
-    'com': 'Add comment',
+    'dec': 'Add decision',
     'ret': 'Return to race',
     'man': 'Manual passing',
     '': '',
 }
 
 RESERVED_SOURCES = [
     'fin',  # finished stage
     'reg',  # registered to stage
     'start',  # started stage
 ]
 
 DNFCODES = ['otl', 'wd', 'dsq', 'dnf', 'dns']
 GAPTHRESH = tod.tod('1.12')
-MINPASSSTR = '20.0'
-MINPASSTIME = tod.tod(MINPASSSTR)
-MAXELAPSTR = '12h00:00'
-MAXELAP = tod.tod(MAXELAPSTR)
+MINPASSTIME = tod.tod(20)
+MAXELAP = tod.tod('12h00:00')
 
 # timing keys
 key_announce = 'F4'
 key_armstart = 'F5'
 key_armlap = 'F6'
 key_placesto = 'F7'  # fill places to selected rider
 key_appendplace = 'F8'  # append sepected rider to places
@@ -114,103 +112,112 @@
 
 # extended fn keys      (ctrl + key)
 key_abort = 'F5'
 key_clearfrom = 'F7'  # clear places on selected rider and all following
 key_clearplace = 'F8'  # clear rider from place list
 
 # config version string
-EVENT_ID = 'roadrace-4.1'
+EVENT_ID = 'rms-4.2'
 
 _CONFIG_SCHEMA = {
     'etype': {
-        'prompt': '',
+        'prompt': 'Roadrace/Criterium/Cyclocross',
         'control': 'section'
     },
     'categories': {
         'prompt': 'Categories:',
         'hint': 'Startlist and result categories',
-        'defer': True
+        'defer': True,
+        'default': '',
     },
     'minlap': {
         'prompt': 'Minimum Lap:',
         'control': 'short',
         'places': 1,
         'type': 'tod',
         'hint': 'Reject laps shorter than minimum lap time',
-        'attr': 'minlap'
+        'attr': 'minlap',
+        'default': MINPASSTIME,
     },
     'totlaps': {
         'prompt': 'Laps:',
         'control': 'short',
         'type': 'int',
         'attr': 'totlaps',
         'subtext': '(Cat laps override)',
-        'hint': 'Default target number of laps for event'
+        'hint': 'Default target number of laps for event',
     },
     'autofinish': {
         'prompt': 'Finish:',
         'control': 'check',
         'type': 'bool',
-        'attr': 'targetlaps',
+        'attr': 'autofinish',
         'subtext': 'Automatically Finish?',
         'hint': 'Automatically finish riders on target lap',
+        'default': True,
     },
     'autoexport': {
         'prompt': 'Export:',
         'control': 'check',
         'type': 'bool',
         'attr': 'autoexport',
         'subtext': 'Automatically export?',
         'hint': 'Export result automatically',
+        'default': False,
     },
     'showdowntimes': {
         'prompt': 'Down Times:',
         'control': 'check',
         'type': 'bool',
         'attr': 'showdowntimes',
         'subtext': 'Show on result?',
         'hint': 'Display down times on result',
+        'default': True,
     },
     'dofastestlap': {
         'prompt': 'Fastest Lap:',
         'control': 'check',
         'type': 'bool',
         'attr': 'dofastestlap',
         'subtext': 'Report with result?',
         'hint': 'Report fastest lap time with categorised result',
+        'default': False,
     },
     'timelimit': {
         'prompt': 'Time Limit:',
         'control': 'short',
         'attr': 'timelimit',
-        'hint': 'Time limit eg: 12%  +1:23  4h00:00'
+        'hint': 'Time limit eg: 12%  +1:23  4h00:00',
     },
     'gapthresh': {
         'prompt': 'Time Gap:',
         'control': 'short',
         'type': 'tod',
         'places': 2,
         'hint': 'Threshold for automatic time gap insertion',
-        'attr': 'gapthresh'
+        'attr': 'gapthresh',
+        'default': GAPTHRESH,
     },
     'clubmode': {
         'prompt': 'Club Mode:',
         'control': 'check',
         'type': 'bool',
         'attr': 'clubmode',
         'subtext': 'Add starters by transponder passing?',
         'hint': 'Add riders to event on passing',
+        'default': False,
     },
     'allowspares': {
         'prompt': 'Spares:',
         'control': 'check',
         'type': 'bool',
         'attr': 'allowspares',
         'subtext': 'Record spare bike passings?',
         'hint': 'Add spare bike passings to event as placeholders',
+        'default': False,
     },
 }
 
 
 class rms:
     """Road race handler."""
 
@@ -229,15 +236,15 @@
             self.cats = list(self.meet.rdb.listcats())
             self.autocats = True
         else:
             self.autocats = False
             for cat in cats:
                 if cat != '':
                     cat = cat.upper()
-                    if cat not in ['CAT', 'SPARE', 'TEAM', 'DS']:
+                    if cat not in ('CAT', 'SPARE', 'TEAM', 'DS'):
                         self.cats.append(cat)
                     else:
                         _log.warning('Invalid result category: %r', cat)
         self.cats.append('')  # always include one empty cat
 
         # update reserved sources list with any cat finish labels
         if len(self.cats) > 1:
@@ -391,83 +398,68 @@
 
     def loadconfig(self):
         """Load event config from disk."""
         self.ridernos.clear()
         self.riders.clear()
         self.resettimer()
         self.cats = []
-        DEFDOWNTIMES = True
-        if self.event['type'] == 'criterium':
-            DEFDOWNTIMES = False
+        if self.etype == 'criterium':
+            _CONFIG_SCHEMA['showdowntimes']['default'] = False
         cr = jsonconfig.config({
             'rms': {
                 'start': None,
-                'id': EVENT_ID,
                 'finish': None,
                 'finished': False,
-                'showdowntimes': DEFDOWNTIMES,
                 'places': '',
-                'comment': [],
+                'decisions': [],
                 'hidecols': [INCOLUMN],
-                'categories': [],
                 'intermeds': [],
-                'allowspares': False,
                 'contests': [],
                 'tallys': [],
                 'lapstart': None,
-                'dofastestlap': False,
-                'minlap': MINPASSSTR,
                 'lapfin': None,
                 'curlap': -1,
                 'passlabels': {},
                 'catonlap': {},
-                'gapthresh': None,
-                'totlaps': None,
-                'autofinish': DEFDOWNTIMES,
                 'passingsource': [],
                 'laptimes': [],
-                'clubmode': False,
-                'timelimit': None,
                 'startlist': '',
-                'autoexport': False,
             }
         })
-        cr.add_section('rms')
+        cr.add_section('rms', _CONFIG_SCHEMA)
         cr.add_section('riders')
         cr.add_section('stagebonus')
         cr.add_section('stagepenalty')
         cr.merge(metarace.sysconf, 'rms')
         if not cr.load(self.configfile):
             _log.info('%r not read, loading defaults', self.configfile)
+        cr.export_section('rms', self)
 
         # load result categories
-        self.loadcats(cr.get('rms', 'categories'))
+        self.loadcats(cr.get_value('rms', 'categories').upper().split())
 
         self.passlabels = cr.get('rms', 'passlabels')
         self.catonlap = cr.get('rms', 'catonlap')
         self.passingsource = []
         for source in cr.get('rms', 'passingsource'):
             self.passingsource.append(source.lower())  # force lower case
 
-        # fetch time gap threshold
-        ngt = tod.mktod(cr.get('rms', 'gapthresh'))
-        if ngt is not None:
-            self.gapthresh = ngt
-            if self.gapthresh != GAPTHRESH:
-                _log.warning('Set time gap threshold %s',
-                             self.gapthresh.rawtime(2))
+        # check gapthresh
+        if self.gapthresh != GAPTHRESH:
+            _log.warning('Set time gap threshold %s',
+                         self.gapthresh.rawtime(2))
+        _log.debug('Minimum lap time: %s', self.minlap.rawtime(1))
 
         # restore stage inters, points and bonuses
         self.loadstageinters(cr, 'rms')
 
         # load competitors
         starters = strops.riderlist_split(
             cr.get('rms', 'startlist').upper().strip(), self.meet.rdb)
 
-        self.allowspares = cr.get_bool('rms', 'allowspares')
         onestoft = False
         oneseed = False
         for r in starters:
             ri = self.addrider(r)
             if ri is not None:
                 nr = Gtk.TreeModelRow(self.riders, ri)
                 if cr.has_option('riders', r):
@@ -497,55 +489,41 @@
                     if lr > 7:
                         for i in range(7, lr):
                             laptod = tod.mktod(ril[i])
                             if laptod is not None:
                                 nr[COL_RFSEEN].append(laptod)
                 # record any extra bonus/penalty to rider model
                 if cr.has_option('stagebonus', r):
-                    nr[COL_BONUS] = tod.mktod(cr.get('stagebonus', r))
+                    nr[COL_BONUS] = cr.get_tod('stagebonus', r)
                 if cr.has_option('stagepenalty', r):
-                    nr[COL_PENALTY] = tod.mktod(cr.get('stagepenalty', r))
+                    nr[COL_PENALTY] = cr.get_tod('stagepenalty', r)
 
-        self.laptimes = []
-        ltin = cr.get('rms', 'laptimes')
-        for ts in ltin:
-            nlt = tod.mktod(ts)
-            if nlt is not None:
-                self.laptimes.append(nlt)
-
-        self.set_start(cr.get('rms', 'start'))
-        self.set_finish(cr.get('rms', 'finish'))
-        self.lapstart = tod.mktod(cr.get('rms', 'lapstart'))
-        self.lapfin = tod.mktod(cr.get('rms', 'lapfin'))
-        self.minlap = tod.mktod(cr.get('rms', 'minlap'))
-        if self.minlap is None:
-            self.minlap = MINPASSTIME
-        _log.debug('Minimum lap time: %s', self.minlap.rawtime())
-        self.curlap = cr.get('rms', 'curlap')
-        self.totlaps = cr.get('rms', 'totlaps')
-        self.timelimit = cr.get('rms', 'timelimit')
+        self.laptimes = cr.get('rms', 'laptimes')
+        self.set_start(cr.get_tod('rms', 'start'))
+        self.set_finish(cr.get_tod('rms', 'finish'))
+        self.lapstart = cr.get_tod('rms', 'lapstart')
+        self.lapfin = cr.get_tod('rms', 'lapfin')
+
+        self.curlap = cr.get_int('rms', 'curlap', -1)
+        self.totlaps = cr.get_int('rms', 'totlaps', None)
         self.places = strops.reformat_placelist(cr.get('rms', 'places'))
-        self.comment = cr.get('rms', 'comment')
-        self.dofastestlap = cr.get_bool('rms', 'dofastestlap')
-        self.autoexport = cr.get_bool('rms', 'autoexport')
+        self.decisions = cr.get('rms', 'decisions')
         if cr.get_bool('rms', 'finished'):
             self.set_finished()
-        self.showdowntimes = cr.get_bool('rms', 'showdowntimes')
-        self.clubmode = cr.get_bool('rms', 'clubmode')
         self.recalculate()
 
         self.hidecols = cr.get('rms', 'hidecols')
         for col in self.hidecols:
             target = strops.confopt_posint(col)
             if target is not None:
                 self.hidecolumn(target)
 
         # load starts and targets and then handle lap situation
         self.load_cat_data()
-        if self.event['type'] != 'handicap':
+        if self.etype != 'handicap':
             for c in self.catstarts:
                 if self.catstarts[c] is not None:
                     onestoft = True
         else:
             # don't autohide the start column for handicaps
             onestoft = True
 
@@ -553,35 +531,31 @@
         if not onestoft:
             self.hidecolumn(STARTCOLUMN)
 
         # auto-hide the seed column
         if not oneseed:
             self.hidecolumn(SEEDCOLUMN)
 
-        if self.targetlaps:
+        if self.autofinish:
             self.curlap = -1
             self.lapentry.set_text('')
             self.lapentry.set_sensitive(False)
         else:
             if self.curlap is not None and self.curlap >= 0:
                 self.lapentry.set_text(str(self.curlap))
             else:
                 self.lapentry.set_text('')
             self.lapentry.set_sensitive(True)
 
         if self.totlaps is not None:
             self.totlapentry.set_text(str(self.totlaps))
 
-        if cr.get_bool('rms', 'autofinish'):
-            # then override targetlaps if autofinish was set
-            self.targetlaps = True
-
         # After load complete - check config and report.
-        eid = cr.get('rms', 'id')
-        if eid and eid != EVENT_ID:
+        eid = cr.get_value('rms', 'id')
+        if eid is not None and eid != EVENT_ID:
             _log.info('Event config mismatch: %r != %r', eid, EVENT_ID)
             self.readonly = True
 
     def get_ridercmdorder(self):
         """Return rider command list order."""
         ret = RIDER_COMMANDS_ORD[0:]
         for i in self.intermeds:
@@ -677,60 +651,44 @@
 
     def saveconfig(self):
         """Save event config to disk."""
         if self.readonly:
             _log.error('Attempt to save readonly event')
             return
         cw = jsonconfig.config()
-        cw.add_section('rms')
-        if self.start is not None:
-            cw.set('rms', 'start', self.start.rawtime())
-        if self.finish is not None:
-            cw.set('rms', 'finish', self.finish.rawtime())
-        if self.lapstart is not None:
-            cw.set('rms', 'lapstart', self.lapstart.rawtime())
-        if self.lapfin is not None:
-            cw.set('rms', 'lapfin', self.lapfin.rawtime())
-        cw.set('rms', 'showdowntimes', self.showdowntimes)
-        cw.set('rms', 'minlap', self.minlap.rawtime())
-        cw.set('rms', 'gapthresh', self.gapthresh.rawtime())
+        cw.add_section('rms', _CONFIG_SCHEMA)
+        cw.import_section('rms', self)
+        cw.set('rms', 'start', self.start)
+        cw.set('rms', 'finish', self.finish)
+        cw.set('rms', 'lapstart', self.lapstart)
+        cw.set('rms', 'lapfin', self.lapfin)
         cw.set('rms', 'finished', self.timerstat == 'finished')
         cw.set('rms', 'places', self.places)
         cw.set('rms', 'curlap', self.curlap)
         cw.set('rms', 'onlap', self.onlap)
-        cw.set('rms', 'totlaps', self.totlaps)
-        cw.set('rms', 'allowspares', self.allowspares)
-        cw.set('rms', 'timelimit', self.timelimit)
         cw.set('rms', 'passlabels', self.passlabels)
         cw.set('rms', 'catonlap', self.catonlap)
-        cw.set('rms', 'dofastestlap', self.dofastestlap)
-        cw.set('rms', 'autoexport', self.autoexport)
         cw.set('rms', 'passingsource', self.passingsource)
-        cw.set('rms', 'clubmode', self.clubmode)
-        cw.set('rms', 'autofinish', self.targetlaps)
-        ltout = []
-        for lt in self.laptimes:
-            ltout.append(lt.rawtime())
-        cw.set('rms', 'laptimes', ltout)
+        cw.set('rms', 'laptimes', self.laptimes)
 
         # save stage inters, points and bonuses
         self.savestageinters(cw, 'rms')
 
         # save riders
         evtriders = self.get_startlist()
         if evtriders:
             cw.set('rms', 'startlist', self.get_startlist())
         else:
             if self.autostartlist is not None:
                 cw.set('rms', 'startlist', self.autostartlist)
         if self.autocats:
-            cw.set('rms', 'categories', ['AUTO'])
+            cw.set('rms', 'categories', 'AUTO')
         else:
-            cw.set('rms', 'categories', self.get_catlist())
-        cw.set('rms', 'comment', self.comment)
+            cw.set('rms', 'categories', ' '.join(self.get_catlist()).strip())
+        cw.set('rms', 'decisions', self.decisions)
         cw.set('rms', 'hidecols', self.hidecols)
 
         cw.add_section('riders')
         # sections for commissaire awarded bonus/penalty
         cw.add_section('stagebonus')
         cw.add_section('stagepenalty')
         for r in self.riders:
@@ -750,17 +708,17 @@
                 mb, sto
             ]
             for t in r[COL_RFSEEN]:
                 if t is not None:
                     slice.append(t.rawtime())  # retain 'precision' here too
             cw.set('riders', bib, slice)
             if r[COL_BONUS] is not None:
-                cw.set('stagebonus', bib, r[COL_BONUS].rawtime())
+                cw.set('stagebonus', bib, r[COL_BONUS])
             if r[COL_PENALTY] is not None:
-                cw.set('stagepenalty', bib, r[COL_PENALTY].rawtime())
+                cw.set('stagepenalty', bib, r[COL_PENALTY])
         cw.set('rms', 'id', EVENT_ID)
         _log.debug('Saving event config %r', self.configfile)
         with metarace.savefile(self.configfile) as f:
             cw.write(f)
 
     def show(self):
         """Show event container."""
@@ -773,17 +731,16 @@
     def title_close_clicked_cb(self, button, entry=None):
         """Close and save the race."""
         self.meet.close_event()
 
     def set_titlestr(self, titlestr=None):
         """Update the title string label."""
         if titlestr is None or titlestr == '':
-            etype = self.event['type']
-            if etype in ROADRACE_TYPES:
-                titlestr = '[' + ROADRACE_TYPES[etype] + ']'
+            if self.etype in ROADRACE_TYPES:
+                titlestr = '[' + ROADRACE_TYPES[self.etype] + ']'
             else:
                 titlestr = '[Road Event]'
         self.title_namestr.set_text(titlestr)
 
     def destroy(self):
         """Emit destroy signal to race handler."""
         if self.context_menu is not None:
@@ -992,15 +949,14 @@
                         ls = lt
                         onetarget = True
                     else:
                         onemissing = True
             self.catstarts[c] = cs
             self.catlaps[c] = ls
         if onetarget:
-            self.targetlaps = True
             if onemissing:
                 # There's one or more cats without a target, issue warning
                 missing = []
                 for c in self.catlaps:
                     if self.catlaps[c] is None:
                         missing.append(repr(c))
                 if missing:
@@ -1033,15 +989,14 @@
                     catnm = c
                     dbr = self.meet.rdb.get_rider(c, 'cat')
                     if dbr is not None:
                         catnm = dbr['title']
                     catcache[c] = catnm
 
         ret = []
-        sec = None
         sec = report.twocol_startlist('startlist')
         if callup:
             sec.heading = 'Call-up'
         else:
             sec.heading = 'Startlist'
         if catname:
             sec.heading += ': ' + catname
@@ -1065,15 +1020,15 @@
                 if not r[COL_INRACE]:
                     cmt = r[COL_COMMENT]
                     if cmt == 'dns':
                         comment = cmt
                 riderno = r[COL_BIB].translate(strops.INTEGER_UTRANS)
                 sec.lines.append([comment, riderno, name, ucicode])
                 # Look up pilots
-                if cat in ['MB', 'WB']:
+                if cat in ('MB', 'WB'):
                     # lookup pilot
                     dbr = self.meet.rdb.get_rider(r[COL_BIB], 'pilot')
                     if dbr is not None:
                         sec.even = True  # force even first column
                         puci = dbr['uci id']
                         pnam = dbr.listname()
                         sec.lines.append(['', '', pnam, puci])
@@ -1081,45 +1036,42 @@
         fvc = []
         if footer:
             fvc.append(footer)
         if rcnt > 1:
             fvc.append('Total riders: ' + str(rcnt))
         if fvc:
             sec.footer = '\t'.join(fvc)
-        if len(sec.lines) > 0:
+        if cat or len(sec.lines) > 0 or len(self.cats) < 2:
             ret.append(sec)
             if uncat:
                 _log.warning('%r uncategorised riders', len(sec.lines))
-        else:
-            if cat:
-                _log.warning('No starters for category %r', cat)
 
         return ret
 
     def analysis_report(self):
         """Return an analysis report."""
         # temporary fall through to camera report
         return self.camera_report()
 
     def camera_report(self):
         """Return the judges (camera) report."""
         # Note: camera report treats all riders as a single blob
         ret = []
         self.recalculate()  # fill places and bunch info
-        pthresh = self.meet.timer.photothresh()
+        pthresh = self.meet._timer.photothresh()
         totcount = 0
         dnscount = 0
         dnfcount = 0
         fincount = 0
         lcomment = ''
         insertgap = True
         if self.timerstat != 'idle':
             sec = report.judgerep('judging')
             sec.heading = 'Judges Report'
-            if self.event['type'] == 'cross':
+            if self.etype == 'cross':
                 sec.colheader = [
                     '', 'no', 'rider', 'lap', 'finish', 'lap avg', 'passings'
                 ]
             else:
                 sec.colheader = [
                     '', 'no', 'rider', 'lap', 'finish', 'rftime', 'passings'
                 ]
@@ -1143,15 +1095,15 @@
                 placed = False
                 timed = False
                 photo = False
                 rbib = r[COL_BIB]
                 rcat = r[COL_CAT]
                 ecat = self.ridercat(riderdb.primary_cat(rcat))
                 catstart = None
-                if ecat in self.catstarts and self.event['type'] != 'cross':
+                if ecat in self.catstarts and self.etype != 'cross':
                     catstart = self.catstarts[ecat]
                 laplist = []
                 if r[COL_RFTIME] is not None:
                     for lt in r[COL_RFSEEN]:
                         if lt <= r[COL_RFTIME]:
                             laplist.append(lt)
                 else:
@@ -1173,15 +1125,15 @@
                             if not pset and lrf is not None:
                                 if r[COL_RFTIME] - lrf < pthresh:
                                     photo = True
                                     if not sec.lines[-1][7]:  # not placed
                                         sec.lines[-1][8] = True
                             if self.start is not None:
                                 et = r[COL_RFTIME] - self.start
-                                if self.event['type'] == 'cross':
+                                if self.etype == 'cross':
                                     if r[COL_LAPS] > 0:
                                         al = tod.mktod(et.timeval /
                                                        r[COL_LAPS])
                                         es = al.rawtime(1)
                                 else:
                                     es = et.rawtime(2)
                             else:
@@ -1194,15 +1146,17 @@
                         if ft is None:
                             ft = bt
                             bs = ft.rawtime(0)
                         else:
                             if bt > lt:
                                 # New bunch
                                 sec.lines.append([None, None, None])
-                                bs = '+' + (bt - ft).rawtime(0)
+                                down = bt - ft
+                                if down < MAXELAP:
+                                    bs = '+' + down.rawtime(0)
                             else:
                                 # Same time
                                 pass
                         lt = bt
                         # sep placed and unplaced
                         insertgap = False
                         if lplaced and placed != lplaced:
@@ -1280,20 +1234,23 @@
         return ret
 
     def single_catresult(self, cat):
         _log.debug('Cat result for cat=%r', cat)
         ret = []
         allin = False
         catname = cat
+        secid = 'result'
         if cat == '':
             if len(self.cats) > 1:
                 catname = 'Uncategorised Riders'
             else:
                 # There is only one cat - so all riders are in it
                 allin = True
+        else:
+            secid = 'result-' + cat.lower()
         subhead = ''
         footer = ''
         distance = self.meet.get_distance()
         laps = self.totlaps
         if cat in self.catlaps and self.catlaps[cat] is not None:
             laps = self.catlaps[cat]
         doflap = self.dofastestlap
@@ -1309,15 +1266,15 @@
             footer = dbr['footer']
             dist = dbr['distance']
             if dist:
                 try:
                     distance = float(dist)
                 except Exception:
                     _log.warning('Invalid distance %r for cat %r', dist, cat)
-        sec = report.section('result-' + cat)
+        sec = report.section(secid)
 
         wt = None
         bwt = None
         leadpass = None
         leadlap = None
         leadsplits = None
         lt = None
@@ -1342,15 +1299,16 @@
             incat = False
             if allin or (cat and cat in rcats):
                 incat = True  # rider is in this category
             elif not cat:  # is the rider uncategorised?
                 if rcats[0] == '':
                     incat = True
                 else:
-                    incat = rcats[0] not in self.cats  # backward logic
+                    # exclude properly categorised riders
+                    incat = rcats[0] not in self.cats
             if incat:
                 if cat:
                     rcat = cat
                 else:
                     rcat = rcats[0]  # (work-around mis-categorised rider)
                 totcount += 1
                 sof = None  # all riders have a start time offset
@@ -1386,15 +1344,15 @@
                         lp = ''
                     plcnt += 1
                     pstr = ''
                     if lp is not None and lp != '':
                         pstr = lp + '.'
                         jcnt += 1
                     bt = self.vbunch(r[COL_CBUNCH], r[COL_MBUNCH])
-                    if self.event['type'] == 'cross':
+                    if self.etype == 'cross':
                         ronlap = True
                         risleader = False
                         dtlap = rlap
                         if leadpass is None and rlap > 0:
                             risleader = True
                             leadlap = rlap
                             if len(r[COL_RFSEEN]) > 0:
@@ -1464,15 +1422,17 @@
                         if wt is None:  # first finish time
                             wt = et
                             if rlap != laps:
                                 # assume the distance is invalid
                                 distance = None
                         if bwt is not None:
                             if self.showdowntimes:
-                                dstr = '+' + (et - bwt).rawtime(0)
+                                down = et - bwt
+                                if down < MAXELAP:
+                                    dstr = '+' + down.rawtime(0)
                         else:
                             dstr = et.rawtime(0)
                         first = False
                         if bwt is None:
                             bwt = et
                     lt = bt
                 else:
@@ -1492,36 +1452,38 @@
                         bt = self.vbunch(r[COL_CBUNCH], r[COL_MBUNCH])
                         if bt is not None and self.showdowntimes:
                             if not first and wt is not None:
                                 et = bt
                                 if sof is not None:
                                     # apply a start offset
                                     et = bt - sof
-                                dstr = '+' + (et - wt).rawtime(0)
+                                down = et - wt
+                                if down < MAXELAP:
+                                    dstr = '+' + down.rawtime(0)
                         hdcount += 1
                     else:
                         dnfcount += 1
                     pstr = comment
                 if placed or timed or virtual:
                     sec.lines.append([pstr, bstr, nstr, cstr, tstr, dstr])
                     ## and look up pilots?
-                    if cat in ['MB', 'WB']:
+                    if cat in ('MB', 'WB'):
                         sec.even = True  # twocol result
                         # lookup pilot
                         dbr = self.meet.rdb.get_rider(bstr, 'pilot')
                         if dbr is not None:
                             puci = dbr['uci id']
                             pnam = dbr.listname()
                             sec.lines.append(['', 'pilot', pnam, puci, '', ''])
                 if doflap and comment != 'dns':
                     if len(r[COL_RFSEEN]) > 0:
                         # only consider laps between stime and ftime
                         stime = self.start
                         if sof is not None:
-                            time += sof
+                            stime += sof
                         ftime = tod.now()
                         if r[COL_RFTIME] is not None:
                             ftime = r[COL_RFTIME]
                         ls = stime
                         lt = None
                         lc = 0
                         for p in r[COL_RFSEEN]:
@@ -1541,41 +1503,42 @@
                                     pass
                                     # short lap
                                 ls = p
                 rcnt += 1
             else:
                 # not in this category.
                 pass
-        if self.timerstat == 'finished':
+        if self.timerstat in ('idle', 'finished'):
             sec.heading = 'Result'
-        elif self.timerstat in ['idle', 'armstart']:
-            sec.heading = ''
-        elif self.timerstat in ['running', 'armfinish']:
+        elif self.timerstat in ('armstart', 'running', 'armfinish'):
             # set status if number of judged riders greater than jtgt
             jtgt = 10
             javail = totcount - (dnfcount + dnscount + hdcount)
-            if javail < 16:
-                jtgt = 1
+            if javail < 10:
+                jtgt = min(3, javail)
             if javail > 0 and jcnt >= jtgt:
                 sec.heading = 'Provisional Result'
             elif vcnt > 0:
                 sec.heading = 'Virtual Standing'
             else:
                 sec.heading = 'Race In Progress'
         else:
             sec.heading = 'Provisional Result'
         if footer:
             sec.footer = footer
 
-        # Append all result categories and uncat if riders
-        if cat or totcount > 0:
+        # Append all result categories and uncat if appropriate
+        if cat or totcount > 0 or len(self.cats) < 2:
             ret.append(sec)
             rsec = sec
             # Race metadata / UCI comments
-            sec = report.bullet_text('uci-' + cat)
+            secid = 'resultmeta'
+            if cat:
+                secid = 'resultmeta-' + cat.lower()
+            sec = report.bullet_text(secid)
             if wt is not None:
                 if distance is not None:
                     sec.lines.append([
                         None, 'Average speed of the winner: ' +
                         wt.speedstr(1000.0 * distance)
                     ])
             if doflap and fno is not None:
@@ -1618,36 +1581,91 @@
 
     def result_report(self):
         """Return a result report."""
         ret = []
         self.recalculate()
 
         # check if a categorised report is required
-        if (self.event['type'] == 'cross'
-                or (self.event['type'] != 'handicap' and len(self.cats) > 1)):
-            ret.extend(self.catresult_report())
-        else:
+        if self.etype == 'handicap':
             ret.extend(self.handicap_report())
+        else:
+            ret.extend(self.catresult_report())
 
         # show all intermediates here
         for i in self.intermeds:
             im = self.intermap[i]
             if im['places'] and im['show']:
                 ret.extend(self.int_report(i))
 
-        if len(self.comment) > 0:
-            s = report.bullet_text('comms')
-            s.heading = 'Decisions of the commissaires panel'
-            for comment in self.comment:
-                s.lines.append([None, comment])
-            ret.append(s)
+        # append a decisions section
+        ret.append(self.decision_section())
+
+        return ret
+
+    def decision_section(self):
+        """Return an officials decision section"""
+        ret = report.bullet_text('decisions')
+        if self.decisions:
+            ret.heading = 'Decisions of the commissaires panel'
+            for decision in self.decisions:
+                if decision:
+                    ret.lines.append((None, self.decision_format(decision)))
         return ret
 
+    def decision_format(self, decision):
+        """Crudely macro format a commissaire decision string"""
+        ret = []
+        for line in decision.split('\n'):
+            if line:
+                ol = []
+                for word in line.split():
+                    if word.startswith('r:'):
+                        punc = ''
+                        if not word[-1].isalnum():
+                            punc = word[-1]
+                            word = word[0:-1]
+                        rep = word
+                        look = word.split(':', 1)[-1]
+                        _log.debug('Look up rider: %r', look)
+                        rid = self.meet.rdb.get_id(look)
+                        if rid is not None:
+                            rep = self.meet.rdb[rid].name_bib()
+                        ol.append(rep + punc)
+                    elif word.startswith('t:'):
+                        punc = ''
+                        if not word[-1].isalnum():
+                            punc = word[-1]
+                            word = word[0:-1]
+                        rep = word
+                        look = word.split(':', 1)[-1]
+                        _log.debug('Look up team: %r', look)
+                        rid = self.meet.rdb.get_id(look, 'team')
+                        if rid is not None:
+                            rep = self.meet.rdb[rid][
+                                'first'] + ' (' + look.upper() + ')'
+                        ol.append(rep + punc)
+                    elif word.startswith('d:'):
+                        punc = ''
+                        if not word[-1].isalnum():
+                            punc = word[-1]
+                            word = word[0:-1]
+                        rep = word
+                        look = word.split(':', 1)[-1]
+                        _log.debug('Look up ds: %r', look)
+                        rid = self.meet.rdb.get_id(look, 'ds')
+                        if rid is not None:
+                            rep = self.meet.rdb[rid].fitname(48)
+                        ol.append(rep + punc)
+                    else:
+                        ol.append(word)
+                ret.append(' '.join(ol))
+        return '\n'.join(ret)
+
     def handicap_report(self):
-        _log.debug('Result report in uncat/handicap path')
+        _log.debug('Result report in handicap path')
         ret = []
         wt = None
         we = None
         dofastest = False  # ftime for handicaps
         fastest = None
         vfastest = None
         curelap = None
@@ -1666,176 +1684,170 @@
             if c != '':
                 catnm = c
                 dbr = self.meet.rdb.get_rider(c, 'cat')
                 if dbr is not None:
                     catnm = dbr['title']
                 catcache[c] = catnm
         lt = None
-        if self.places or self.timerstat != 'idle':
-            sec = report.section('result')
-            if self.event['type'] == 'handicap':
-                sec.colheader = [None, None, None, None, 'Elapsed', 'Time/Gap']
-            if self.racestat == 'final':
-                sec.heading = 'Result'
-            elif self.racestat == 'provisional':
-                sec.heading = 'Provisional Result'
-            else:
-                sec.heading = 'Race In Progress'
+        sec = report.section('result')
+        sec.colheader = [None, None, None, None, 'Elapsed', 'Time/Gap']
+        if self.racestat in ('prerace', 'final'):
+            sec.heading = 'Result'
+        elif self.racestat == 'provisional':
+            sec.heading = 'Provisional Result'
+        else:
+            sec.heading = 'Race In Progress'
 
-            first = True
-            for r in self.riders:
-                totcount += 1
-                bstr = r[COL_BIB]  # 'bib'
-                nstr = r[COL_NAMESTR]  # 'name'
-                # in handicap / flat result - only first category is considered
-                cs = r[COL_CAT]
-                cstr = riderdb.primary_cat(cs)  # 'cat'
-                rcat = self.ridercat(cstr)
-                if cstr.upper() in catcache:
-                    cstr = catcache[cstr.upper()]
-                dbr = self.meet.rdb.get_rider(bstr, self.series)
-                if dbr is not None:
-                    cstr = dbr['uci id']
-                pstr = ''  # 'place'
-                tstr = ''  # 'elap' (hcp only)
-                dstr = ''  # 'time/gap'
-                placed = False  # placed at finish
-                timed = False  # timed at finish
-                if r[COL_INRACE]:
-                    psrc = r[COL_PLACE]
-                    if psrc != '':
-                        pstr = psrc + '.'
-                        placed = True
+        first = True
+        for r in self.riders:
+            totcount += 1
+            bstr = r[COL_BIB]  # 'bib'
+            nstr = r[COL_NAMESTR]  # 'name'
+            # in handicap - only primary category is considered
+            cs = r[COL_CAT]
+            cstr = riderdb.primary_cat(cs)  # 'cat'
+            rcat = self.ridercat(cstr)
+            # in handicap result, cat overrides UCIID
+            if cstr.upper() in catcache:
+                cstr = catcache[cstr.upper()]
+            pstr = ''  # 'place'
+            tstr = ''  # 'elap' (hcp only)
+            dstr = ''  # 'time/gap'
+            placed = False  # placed at finish
+            timed = False  # timed at finish
+            if r[COL_INRACE]:
+                psrc = r[COL_PLACE]
+                if psrc != '':
+                    pstr = psrc + '.'
+                    placed = True
+                bt = self.vbunch(r[COL_CBUNCH], r[COL_MBUNCH])
+                if bt is not None:
+                    timed = True
+                    fincount += 1  # for accounting, use bunch time
+                    if wt is None:  # first finish time
+                        wt = bt
+                        first = False
+                        # for hcap, first time is always race time
+                        dstr = wt.rawtime(0)
+                    else:
+                        # for handicap, time gap is always
+                        # down on winner's uncorrected time
+                        if self.showdowntimes:
+                            down = bt - wt
+                            if down < MAXELAP:
+                                dstr = '+' + down.rawtime(0)
+
+                    # show elapsed for hcp ...*
+                    tstr = bt.rawtime(0)
+                    et = bt
+                    sof = None
+                    if r[COL_STOFT] is not None:  # apply a start offset
+                        sof = r[COL_STOFT]
+                    elif rcat in self.catstarts:
+                        sof = self.catstarts[rcat]
+                    if sof is not None:
+                        dofastest = True  # will need to report!
+                        et = bt - sof
+                        # *... adjust if a start offset is present
+                        tstr = et.rawtime(0)
+                        if we is None:
+                            we = et
+                    if fastest is None or et < fastest:
+                        fastest = et
+                        fastestbib = r[COL_BIB]
+                else:  # check virtual finish time
+                    sof = None
+                    if r[COL_STOFT] is not None:
+                        sof = r[COL_STOFT]
+                    elif rcat in self.catstarts and self.catstarts[
+                            rcat] != tod.ZERO:
+                        sof = self.catstarts[rcat]
+                    if sof is not None and curelap is not None:
+                        vt = curelap - sof
+                        if vfastest is None or vt < vfastest:
+                            vfastest = vt
+                lt = bt
+            else:
+                # Non-finishers dns, dnf, otl, dsq
+                placed = True  # for purpose of listing
+                comment = r[COL_COMMENT]
+                if comment == '':
+                    comment = 'dnf'
+                if comment != lcomment:
+                    sec.lines.append([None, None, None])  # new bunch
+                lcomment = comment
+                # account for special cases
+                if comment == 'dns':
+                    dnscount += 1
+                elif comment == 'otl':
+                    # otl special case: also show down time if possible
                     bt = self.vbunch(r[COL_CBUNCH], r[COL_MBUNCH])
                     if bt is not None:
-                        timed = True
-                        fincount += 1  # for accounting, use bunch time
-                        if wt is None:  # first finish time
-                            wt = bt
-                            first = False
-                            # for uncat/hcap first time is always race time
-                            dstr = wt.rawtime(0)
-                        else:
-                            # for uncat/handicap, time gap is always
-                            # down on winner's uncorrected time
-                            if self.showdowntimes:
-                                dstr = '+' + (bt - wt).rawtime(0)
-
-                        # compute elapsed, or corrected time
-                        if self.event['type'] == 'handicap':
-                            # always show elap for hcp, even if no stof*
-                            tstr = bt.rawtime(0)
-                        et = bt
-                        sof = None
-                        if r[COL_STOFT] is not None:  # apply a start offset
-                            sof = r[COL_STOFT]
-                        elif rcat in self.catstarts:
-                            sof = self.catstarts[rcat]
-                        if sof is not None:
-                            dofastest = True  # will need to report!
-                            et = bt - sof
-                            # *but, adjust tstr if a start offset is present
-                            tstr = et.rawtime(0)
-                            if we is None:
-                                we = et
-                        if fastest is None or et < fastest:
-                            fastest = et
-                            fastestbib = r[COL_BIB]
-                    else:  # check virtual finish time
-                        sof = None
-                        if r[COL_STOFT] is not None:
-                            sof = r[COL_STOFT]
-                        elif rcat in self.catstarts and self.catstarts[
-                                rcat] != tod.ZERO:
-                            sof = self.catstarts[rcat]
-                        if sof is not None:
-                            vt = curelap - sof
-                            if vfastest is None or vt < vfastest:
-                                vfastest = vt
-                    lt = bt
-                else:
-                    # Non-finishers dns, dnf, otl, dsq
-                    placed = True  # for purpose of listing
-                    comment = r[COL_COMMENT]
-                    if comment == '':
-                        comment = 'dnf'
-                    if comment != lcomment:
-                        sec.lines.append([None, None, None])  # new bunch
-                    lcomment = comment
-                    # account for special cases
-                    if comment == 'dns':
-                        dnscount += 1
-                    elif comment == 'otl':
-                        # otl special case: also show down time if possible
-                        bt = self.vbunch(r[COL_CBUNCH], r[COL_MBUNCH])
-                        if bt is not None:
-                            if not first and wt is not None:
-                                et = bt
-                                sof = None
-                                if r[COL_STOFT] is not None:
-                                    sof = r[COL_STOFT]
-                                elif rcat in self.catstarts:
-                                    sof = self.catstarts[rcat]
-                                if sof is not None:
-                                    # apply a start offset
-                                    et = bt - sof
-                                dstr = '+' + (et - wt).rawtime(0)
-                        hdcount += 1
-                    else:
-                        dnfcount += 1
-                    pstr = comment
-                if placed or timed:
-                    sec.lines.append([pstr, bstr, nstr, cstr, tstr, dstr])
-            ret.append(sec)
-
-            # Race metadata / UCI comments
-            sec = report.bullet_text('resultuci')
-            if wt is not None:
-                sec.lines.append([None, 'Race time: ' + wt.rawtime(0)])
-                if we is None:
-                    we = wt
-                dval = self.meet.get_distance()
-                if dval is not None:
-                    sec.lines.append([
-                        None, 'Average speed of the winner: ' +
-                        we.speedstr(1000.0 * dval)
-                    ])
-            if self.event['type'] == 'handicap' and dofastest:
-                if vfastest and vfastest < fastest:
-                    _log.info('Fastest time not yet available')
+                        if not first and wt is not None:
+                            et = bt
+                            sof = None
+                            if r[COL_STOFT] is not None:
+                                sof = r[COL_STOFT]
+                            elif rcat in self.catstarts:
+                                sof = self.catstarts[rcat]
+                            if sof is not None:
+                                # apply a start offset
+                                et = bt - sof
+                            down = et - wt
+                            if down < MAXELAP:
+                                dstr = '+' + down.rawtime(0)
+                    hdcount += 1
                 else:
-                    ftr = self.getrider(fastestbib)
-                    fts = ''
-                    if ftr is not None:
-                        fts = ftr[COL_SHORTNAME]
-                    fmsg = ('Fastest time: ' + fastest.rawtime(0) + '  ' +
-                            fastestbib + ' ' + fts)
-                    smsg = ('Fastest time - ' + fts + ' ' + fastest.rawtime(0))
-                    sec.lines.append([None, fmsg])
-                    if not self.readonly:  # in a ui window?
-                        self.meet.cmd_announce('resultmsg', fmsg)
-                        self.meet.cmd_announce('scrollmsg', smsg)
+                    dnfcount += 1
+                pstr = comment
+            if placed or timed:
+                sec.lines.append([pstr, bstr, nstr, cstr, tstr, dstr])
+        ret.append(sec)
 
-            sec.lines.append(
-                [None, 'Number of starters: ' + str(totcount - dnscount)])
-            if hdcount > 0:
+        # Race metadata / UCI comments
+        sec = report.bullet_text('resultmeta')
+        if wt is not None:
+            sec.lines.append([None, 'Race time: ' + wt.rawtime(0)])
+            if we is None:
+                we = wt
+            dval = self.meet.get_distance()
+            if dval is not None:
                 sec.lines.append([
-                    None,
-                    'Riders finishing out of time limits: ' + str(hdcount)
+                    None, 'Average speed of the winner: ' +
+                    we.speedstr(1000.0 * dval)
                 ])
-            if dnfcount > 0:
-                sec.lines.append(
-                    [None, 'Riders abandoning the event: ' + str(dnfcount)])
-            residual = totcount - (fincount + dnfcount + dnscount + hdcount)
-            if residual > 0:
-                _log.info('%r unaccounted for', residual)
-            ret.append(sec)
+        if dofastest:
+            if vfastest and vfastest < fastest:
+                _log.info('Fastest time not yet available')
+            else:
+                ftr = self.getrider(fastestbib)
+                fts = ''
+                if ftr is not None:
+                    fts = ftr[COL_SHORTNAME]
+                fmsg = ('Fastest time: ' + fastest.rawtime(0) + '  ' +
+                        fastestbib + ' ' + fts)
+                smsg = ('Fastest time - ' + fts + ' ' + fastest.rawtime(0))
+                sec.lines.append([None, fmsg])
+                if not self.readonly:  # in a ui window?
+                    self.meet.cmd_announce('resultmsg', fmsg)
+                    self.meet.cmd_announce('scrollmsg', smsg)
+
+        sec.lines.append(
+            [None, 'Number of starters: ' + str(totcount - dnscount)])
+        if hdcount > 0:
+            sec.lines.append(
+                [None, 'Riders finishing out of time limits: ' + str(hdcount)])
+        if dnfcount > 0:
+            sec.lines.append(
+                [None, 'Riders abandoning the event: ' + str(dnfcount)])
+        residual = totcount - (fincount + dnfcount + dnscount + hdcount)
+        if residual > 0:
+            _log.info('%r unaccounted for', residual)
+        ret.append(sec)
 
-        else:
-            _log.warning('No data available for result report')
         return ret
 
     def stat_but_clicked(self, button=None):
         """Deal with a status button click in the main container."""
         _log.debug('Stat button clicked')
 
     def ctrl_change(self, acode='', entry=None):
@@ -1918,25 +1930,25 @@
             return self.race_ctrl_add(rlist)
         elif acode == 'que':
             rlist = strops.reformat_biblist(rlist)
             if rlist != '':
                 for bib in rlist.split():
                     self.query_rider(bib)
             return True
-        elif acode == 'com':
-            self.add_comment(rlist)
+        elif acode == 'dec':
+            self.add_decision(rlist)
             return True
         else:
             _log.error('Ignoring invalid action %r', acode)
         return False
 
-    def add_comment(self, comment=''):
-        """Append a commissaires comment."""
-        self.comment.append(comment.strip())
-        _log.info('Added comment: %r', comment)
+    def add_decision(self, decision=''):
+        """Append a decision of the commissaires panel."""
+        self.decisions.append(decision.strip())
+        _log.debug('Added decision: %r', decision)
 
     def query_rider(self, bib=None):
         """List info on selected rider in the scratchpad."""
         _log.info('Query rider: %r', bib)
         r = self.getrider(bib)
         if r is not None:
             ns = strops.truncpad(r[COL_NAMESTR] + ' ' + r[COL_CAT], 30)
@@ -2001,16 +2013,15 @@
         if self.start is not None:
             st = self.start
         sno = '1'
         if self.meet.mirrorpath:
             sno = self.meet.mirrorfile
         rdx = 1
         odat = [[
-            sno, '1', '1', self.meet.subtitle_str, '', '', '', '', '', '', '',
-            ''
+            sno, '1', '1', self.meet.subtitle, '', '', '', '', '', '', '', ''
         ]]
 
         for r in self.riders:
             bib = r[COL_BIB]
             if r[COL_INRACE]:
                 if r[COL_RFTIME]:
                     last = ''
@@ -2080,15 +2091,15 @@
                     ft = bt
                     sof = None
                     if r[COL_STOFT] is not None:
                         sof = r[COL_STOFT]
                     elif rcat in self.catstarts:
                         sof = self.catstarts[rcat]
                     if sof is not None and bt is not None:
-                        if self.event['type'] == 'cross':
+                        if self.etype == 'cross':
                             if lavg is None:
                                 llaps = r[COL_LAPS]
                                 lpass = r[COL_RFSEEN]
                                 lavg = tod.tod(ft.timeval / llaps)
                                 lbib = bib
                                 ft = bt - sof
                                 lft = ft
@@ -2106,15 +2117,15 @@
                                     if bt < ft:
                                         # is this a valid finish time?
                                         _log.error(
                                             '%r finish time %s ahead of cat leader %r: %s',
                                             bib, ft.rawtime(0), lbib,
                                             lft.rawtime(0))
                                 ft = bt + lxtra - sof
-                        elif self.event['type'] == 'handicap':
+                        elif self.etype == 'handicap':
                             # for handicap, time is stage time, bonus
                             # carries the start offset, elapsed is:
                             # stage - bonus
                             ft = bt
                             bonus = sof
                         else:
                             ft = bt - sof
@@ -2125,16 +2136,16 @@
                         crank = rcount
                     else:
                         crank = lcrank
                     lcrank = crank
                     lrank = rank
                 else:
                     crank = r[COL_COMMENT]
-                if self.event['type'] != 'handicap' and (
-                        bib in self.bonuses or r[COL_BONUS] is not None):
+                if self.etype != 'handicap' and (bib in self.bonuses
+                                                 or r[COL_BONUS] is not None):
                     bonus = tod.ZERO
                     if bib in self.bonuses:
                         bonus += self.bonuses[bib]
                     if r[COL_BONUS] is not None:
                         bonus += r[COL_BONUS]
                 penalty = None
                 if r[COL_PENALTY] is not None:
@@ -2232,19 +2243,19 @@
             seed = strops.confopt_posint(r['notes'])
             if seed is not None:
                 lr[COL_SEED] = seed
 
     def resettimer(self):
         """Reset event timer."""
         _log.info('Reset event to idle')
-        self.meet.alttimer.dearm(1)
         self.set_finish()
         self.set_start()
         self.clear_results()
         self.timerstat = 'idle'
+        self.racestat = 'prerace'
         self.meet.cmd_announce('timerstat', 'idle')
         self.meet.stat_but.update('idle', 'Idle')
         self.meet.stat_but.set_sensitive(True)
         self.curlap = -1
         self.onlap = 1
         self.resetcatonlaps()
         self.lapentry.set_text('')
@@ -2257,15 +2268,15 @@
             self.timerstat = 'armstart'
             self.meet.cmd_announce('timerstat', 'armstart')
             self.meet.stat_but.update('activity', 'Arm Start')
             self.resetcatonlaps()
             self.armlap()
             if self.live_announce:
                 self.meet.cmd_announce('clear', 'all')
-                if self.event['type'] in ['criterium', 'circuit', 'cross']:
+                if self.etype in ('criterium', 'circuit', 'cross'):
                     self.armlap()
 
         elif self.timerstat == 'armstart':
             self.timerstat = 'idle'
             self.meet.cmd_announce('timerstat', 'idle')
             self.meet.stat_but.update('idle', 'Idle')
 
@@ -2277,29 +2288,26 @@
             if target:
                 onechange = True
         if onechange:
             self.announcecatlap()
 
     def armfinish(self):
         """Process an armfinish request."""
-        if self.timerstat in ['running', 'finished']:
+        if self.timerstat in ('running', 'finished'):
             if self.finish is None and self.curlap:
                 # No finish passing yet
                 self.armlap()
             elif self.totlaps == 0:
                 # Unbound lap count
                 self.armlap()
             self.timerstat = 'armfinish'
             self.meet.cmd_announce('timerstat', 'armfinish')
             self.meet.stat_but.update('error', 'Arm Finish')
             self.meet.stat_but.set_sensitive(True)
-            self.meet.alttimer.armlock(True)
-            self.meet.alttimer.arm(1)
         elif self.timerstat == 'armfinish':
-            self.meet.alttimer.dearm(1)
             self.timerstat = 'running'
             self.meet.cmd_announce('timerstat', 'running')
             self.meet.stat_but.update('ok', 'Running')
 
     def last_rftime(self):
         """Find the last rider with a RFID finish time set."""
         ret = None
@@ -2313,17 +2321,17 @@
         if self.curlap is None or self.curlap < 0:
             self.curlap = 0  # manual override lap counts
         self.scratch_map = {}
         self.scratch_ord = []
         titlestr = self.title_namestr.get_text()
         if self.live_announce:
             self.meet.cmd_announce('clear', 'all')
-        if self.timerstat in ['idle', 'armstart', 'armfinish']:
+        if self.timerstat in ('idle', 'armstart', 'armfinish'):
             self.meet.cmd_announce('finstr', self.meet.get_short_name())
-            if self.timerstat in ['idle', 'armstart']:
+            if self.timerstat in ('idle', 'armstart'):
                 self.reannounce_times()  # otherwise not called
                 self.meet.cmd_announce('title', titlestr)  # enforce
                 return False  # no arm till event underway
         if self.curlap <= 0 or self.lapfin is not None:
             self.curlap += 1  # increment
 
             if self.totlaps and self.curlap > self.totlaps:
@@ -2346,15 +2354,15 @@
                 self.meet.cmd_announce('onlap', str(self.onlap))
 
         # update curlap entry whatever happened
         self.lapentry.set_text(str(self.curlap))
 
         # Write lap time fields
         lapstr = None
-        if self.timerstat not in ['armfinish', 'finished']:
+        if self.timerstat not in ('armfinish', 'finished'):
             self.meet.cmd_announce('bunches', 'laps')
             self.meet.cmd_announce('finstr', None)
             ## Step 1: lap time handling
             if self.lapfin:
                 # roll over to lap start
                 self.lapstart = self.lapfin
             elif self.lapstart:  # assume still waiting for same lap
@@ -2368,15 +2376,16 @@
                     self.totlapentry.set_text(str(self.totlaps))
                 else:  # 0 flags unknown total
                     lapstr = ''
                     passkey = str(self.curlap)
                     if passkey in self.passlabels:
                         lapstr = 'At ' + self.passlabels[passkey]
                     else:
-                        lapstr = ('Lap ' + str(self.onlap))
+                        if self.etype in ('circuit', 'criterium', 'cross'):
+                            lapstr = 'Lap ' + str(self.onlap)
                 self.meet.cmd_announce('laplbl', lapstr)
             else:
                 # make sure something is displayed in this path
                 self.meet.cmd_announce('laplbl', None)
                 self.meet.cmd_announce('finstr', self.meet.get_short_name())
             self.lapfin = None
         else:
@@ -2389,17 +2398,19 @@
     def key_event(self, widget, event):
         """Handle global key presses in event."""
         if event.type == Gdk.EventType.KEY_PRESS:
             key = Gdk.keyval_name(event.keyval) or 'None'
             if event.state & Gdk.ModifierType.CONTROL_MASK:
                 if key == key_abort:  # override ctrl+f5
                     if uiutil.questiondlg(
-                            self.meet.window, 'Reset event to idle?',
+                            window=self.meet.window,
+                            question='Reset event to idle?',
+                            subtext=
                             'Note: All result and timing data will be cleared.',
-                            'Reset Event?'):
+                            title='Reset Event?'):
                         self.resettimer()
                     return True
                 elif key == key_announce:  # re-send current announce vars
                     self.reannounce_times()
                     return True
                 elif key == key_clearfrom:  # clear all places from selected
                     self.clear_places_from_selection()
@@ -2590,16 +2601,14 @@
                     _log.debug('Ignored update on non-starter %r', rider)
                 # a change in team may alter team data mapping
                 self.updateteam(rider)
             elif rider[1] == 'cat':
                 # if cat is a result category in this event
                 if self.ridercat(rider[0]):
                     self.load_cat_data()
-                ## TODO: verify if recalc required
-                #self._dorecalc = True
             elif rider[1] == 'team':
                 # team changes may require recalc
                 self.updateteam(rider)
             else:
                 _log.debug('Ignore out of series rider %r', rider)
         else:
             _log.debug('Update all cats')
@@ -2613,16 +2622,14 @@
                     self.updaterider(lr, r)
                     count += 1
                 else:
                     _log.debug('Ignored rider not in riderdb %r', bib)
             _log.debug('Updated %d riders', count)
             _log.debug('Update teams')
             self.updateteam()
-            ## TODO: verify if recalc required
-            #self._dorecalc = True
 
     def retriders(self, biblist=''):
         """Return all listed riders to the event."""
         recalc = False
         for bib in biblist.split():
             r = self.getrider(bib)
             if r is not None:
@@ -2648,15 +2655,15 @@
         """Process a start trigger signal."""
         # Note: in rms all triggers other than C1 from alttimer
         #       are assumed to be for the start
         if self.timerstat == 'armstart':
             _log.info('Start trigger: %s@%s/%s', e.chan, e.rawtime(), e.source)
             self.set_start(e)
             self.resetcatonlaps()
-            if self.event['type'] in ['criterium', 'circuit', 'cross']:
+            if self.etype in ('criterium', 'circuit', 'cross'):
                 GLib.idle_add(self.armlap)
         else:
             _log.info('Trigger: %s@%s/%s', e.chan, e.rawtime(), e.source)
         return False
 
     def set_lap_finish(self, e):
         """Write lap time into model and emit changed state."""
@@ -2674,15 +2681,16 @@
     def alttimertrig(self, e):
         """Record timer message from alttimer."""
         # note: these impulses are sourced from alttimer device and keyboard
         #       transponder triggers are collected separately in timertrig()
         _log.debug('Alt timer: %s@%s/%s', e.chan, e.rawtime(), e.source)
         channo = strops.chan2id(e.chan)
         if channo == 1:
-            # this is a finish impulse, treat as bunch time
+            _log.info('Trigger: %s@%s/%s', e.chan, e.rawtime(), e.source)
+            # if finish armed, treat as bunch time
             if self.timerstat == 'armfinish':
                 if self.altfinish is not None:
                     dt = e - self.altfinish
                     _log.info('New bunch time: +%s', dt.rawtime(0))
                 else:
                     _log.debug('Recording first bunch finish: %s', e.rawtime())
                     self.altfinish = e
@@ -2737,15 +2745,15 @@
                     else:
                         _log.debug('No data for %r cat lap', cat)
 
     def timertrig(self, e):
         """Process transponder passing event."""
 
         # all impulses from transponder timer are considered start triggers
-        if e.refid in ['', '255']:
+        if e.refid in ('', '255'):
             return self.starttrig(e)
 
         # fetch rider data from riderdb using refid lookup
         r = self.meet.getrefid(e.refid)
         if r is None:
             _log.info('Unknown rider: %s:%s@%s/%s', e.refid, e.chan,
                       e.rawtime(2), e.source)
@@ -2754,35 +2762,32 @@
         bib = r['no']
         ser = r['series']
         if ser != self.series:
             _log.info('Non-series rider: %s.%s', bib, ser)
             return False
 
         # if there's a source filter set, discard any unknown sources
-        # todo: channel should be the primary source identifier
         if len(self.passingsource) > 0:
             if e.source.lower() not in self.passingsource:
                 _log.info('Invalid passing: %s:%s@%s/%s', bib, e.chan,
                           e.rawtime(2), e.source)
                 return False
 
         # check for a spare bike in riderdb cat, before clubmode additions
         spcat = r.primary_cat()
-        if self.allowspares and spcat == 'SPARE' and self.timerstat in [
-                'running', 'armfinish'
-        ]:
+        if self.allowspares and spcat == 'SPARE' and self.timerstat in (
+                'running', 'armfinish'):
             _log.warning('Adding spare bike: %r', bib)
             self.addrider(bib)
 
         # fetch event info for rider
         lr = self.getrider(bib)
         if lr is None:
-            if self.clubmode and self.timerstat in [
-                    'armstart', 'running', 'armfinish'
-            ]:
+            if self.clubmode and self.timerstat in ('armstart', 'running',
+                                                    'armfinish'):
                 ri = self.addrider(bib)
                 lr = Gtk.TreeModelRow(self.riders, ri)
                 _log.info('Added new starter: %s:%s@%s/%s', bib, e.chan,
                           e.rawtime(2), e.source)
             else:
                 _log.info('Non-starter: %s:%s@%s/%s', bib, e.chan,
                           e.rawtime(2), e.source)
@@ -2793,15 +2798,15 @@
             _log.warning('Withdrawn rider: %s:%s@%s/%s', bib, e.chan,
                          e.rawtime(2), e.source)
             # but continue as if still in race
         else:
             _log.info('Saw: %s:%s@%s/%s', bib, e.chan, e.rawtime(2), e.source)
 
         # check run state
-        if self.timerstat in ['idle', 'armstart', 'finished']:
+        if self.timerstat in ('idle', 'armstart', 'finished'):
             return False
 
         # fetch primary category IN event
         rcat = self.ridercat(r.primary_cat())
 
         # check for start and minimum passing time
         st = tod.ZERO
@@ -2816,15 +2821,14 @@
         # ignore all passings from before first allowed time
         if e <= st:
             _log.info('Ignored early passing: %s:%s@%s/%s < %s', bib, e.chan,
                       e.rawtime(2), e.source, st.rawtime(2))
             return False
 
         # check this passing against previous passing records
-        # TODO: compare the source against the passing in question
         lastchk = None
         ipos = bisect.bisect_right(lr[COL_RFSEEN], e)
         if ipos == 0:  # first in-race passing, accept
             pass
         else:  # always one to the 'left' of e
             # check previous passing for min lap time
             lastseen = lr[COL_RFSEEN][ipos - 1]
@@ -2850,23 +2854,23 @@
 
     def riderlap(self, bib, lr, rcat, e):
         """Process an accepted rider lap passing"""
         # check if lap mode is target-based
         lapfinish = False
         doarm = False
         targetlap = None
-        if self.targetlaps:
+        if self.autofinish:
             # category laps override event laps
             if rcat in self.catlaps and self.catlaps[rcat]:
                 targetlap = self.catlaps[rcat]
             else:
                 targetlap = self.totlaps
             if targetlap and lr[COL_LAPS] >= targetlap - 1:
                 lapfinish = True  # arm just this rider
-                if self.event['type'] == 'cross':
+                if self.etype == 'cross':
                     doarm = True
 
         # for cross races when targets apply, armfinish is set automatically
         if doarm and lapfinish and self.timerstat != 'armfinish':
             self.armfinish()
 
         # finishing rider path
@@ -2902,23 +2906,23 @@
                                             lr[COL_CAT], e, lr[COL_LAPS])
             else:
                 _log.info('Duplicate finish rider %s:%s@%s/%s', bib, e.chan,
                           e.rawtime(2), e.source)
         # end finishing rider path
 
         # lapping rider path
-        elif self.timerstat in ['running']:  # not finished, not armed
+        elif self.timerstat == 'running':
             self._dorecalc = True
             if lr[COL_INRACE] and (lr[COL_PLACE] or lr[COL_CBUNCH] is None):
                 # rider in the race, not yet finished: increment own lap count
                 lr[COL_LAPS] += 1
                 onlap = False
 
                 # category and target lap counting
-                if self.targetlaps:
+                if self.autofinish:
                     catlap = 0
                     if rcat in self.catonlap:
                         catlap = self.catonlap[rcat]
                     else:
                         self.catonlap[rcat] = 0  # init
 
                     if lr[COL_LAPS] > catlap:
@@ -2949,25 +2953,25 @@
                                 'Passing on previous lap: %s:%s@%s/%s < %s',
                                 bib, e.chan, e.rawtime(2), e.source,
                                 curlapstart.rawtime(2))
                         else:
                             if lr[COL_LAPS] == self.curlap:
                                 onlap = True
                             elif lr[COL_LAPS] < self.curlap:
-                                if self.event['type'] == 'criterium':
+                                if self.etype == 'criterium':
                                     # push them on to the current lap
                                     lr[COL_LAPS] = self.curlap
                                     onlap = True
                                 else:
                                     # rider is not on current event lap
                                     pass
                             else:
                                 if e < curlapstart + self.minlap:
                                     # passing cannot be for a new lap yet
-                                    if self.event['type'] == 'criterium':
+                                    if self.etype == 'criterium':
                                         # push them back to the current lap
                                         lr[COL_LAPS] = self.curlap
                                         onlap = True
                                     else:
                                         _log.warning(
                                             'Invalid laps %r: %r / %r', bib,
                                             lr[COL_LAPS], self.curlap)
@@ -3006,24 +3010,22 @@
         newlap = None
         try:
             newlap = int(reqlap)
         except Exception:
             _log.debug('Invalid lap count %r', reqlap)
 
         if newlap is not None and newlap > 0:
-            if self.event['type'] == 'criterium':
+            if self.etype == 'criterium':
                 # force all in riders onto the desired lap
                 for r in self.riders:
                     if r[COL_INRACE]:
                         r[COL_LAPS] = newlap - 1
             else:
                 # correct all rider lap counts, saturated at desired lap
                 for r in self.riders:
-                    # TODO: olap should only include laps recorded after
-                    #       catstart - which may have changed
                     olap = len(r[COL_RFSEEN])
                     if r[COL_INRACE]:
                         if olap > newlap - 1:
                             olap = newlap - 1
                     r[COL_LAPS] = olap
             if self.lapfin is not None:
                 self.curlap = newlap - 1
@@ -3032,21 +3034,21 @@
             self.armlap()
         else:
             self.curlap = -1
             self.lapstart = None
             self.lapfin = None
             maxlap = 1
             entry.set_text('')
-            if self.timerstat not in ['idle', 'armstart', 'finished']:
+            if self.timerstat not in ('idle', 'armstart', 'finished'):
                 maxlap = 0
                 for r in self.riders:
                     r[COL_LAPS] = len(r[COL_RFSEEN])
                     maxlap = max(r[COL_LAPS] + 1, maxlap)
             self.onlap = maxlap
-            if self.event['type'] in ['criterium', 'circuit', 'cross']:
+            if self.etype in ('criterium', 'circuit', 'cross'):
                 self.armlap()
 
     def totlapentry_activate_cb(self, entry, data=None):
         """Transfer total lap entry string into model if possible."""
         try:
             nt = entry.get_text()
             if nt:  # not empty
@@ -3073,15 +3075,15 @@
             self.meet.cmd_announce('title', titlestr + ': Provisional')
         self.meet.cmd_announce('bunches', 'final')
         placeset = set()
         idx = 0
         st = tod.ZERO
         if self.start is not None:
             st = self.start
-        # result is sent in weird hybrid units TODO: fix the amb
+        # result elapsed time is sent in hybrid units
         wt = None
         lb = None
         scrollcnt = 0
         for placegroup in places.split():
             curplace = idx + 1
             for bib in placegroup.split('-'):
                 if bib not in placeset:
@@ -3170,15 +3172,14 @@
                 sec.units = 'pt'
             ret.append(sec)
         return ret
 
     def intsprint(self, acode='', places=''):
         """Display an intermediate sprint 'provisional' result."""
 
-        ## TODO : Fix offset time calcs - too many off by ones
         if acode not in self.intermeds:
             _log.debug('Attempt to display non-existent inter: %r', acode)
             return
         descr = acode
         if self.intermap[acode]['descr']:
             descr = self.intermap[acode]['descr']
         self.live_announce = False
@@ -3232,28 +3233,29 @@
         if self.onlap is not None:
             onlap = str(self.onlap)
         self.meet.cmd_announce('onlap', onlap)
         self.meet.cmd_announce('curlap', curlap)
         self.meet.cmd_announce('totlaps', totlaps)
         # Write lap time fields
         lapstr = None
-        if self.timerstat not in ['armfinish', 'finished']:
+        if self.timerstat not in ('armfinish', 'finished'):
             self.meet.cmd_announce('finstr', None)
             if self.onlap is not None:
                 if self.totlaps is not None and self.totlaps > 0:
                     lapstr = ('Lap ' + str(self.onlap) + '/' +
                               str(self.totlaps))
                     self.totlapentry.set_text(str(self.totlaps))
                 else:  # 0 flags unknown total
                     lapstr = ''
                     passkey = str(self.curlap)
                     if passkey in self.passlabels:
                         lapstr = 'At ' + self.passlabels[passkey]
                     else:
-                        lapstr = ('Lap ' + str(self.onlap))
+                        if self.etype in ('circuit', 'criterium', 'cross'):
+                            lapstr = ('Lap ' + str(self.onlap))
                 self.meet.cmd_announce('laplbl', lapstr)
             else:
                 # make sure something is displayed in this path
                 self.meet.cmd_announce('laplbl', None)
                 self.meet.cmd_announce('finstr', self.meet.get_short_name())
 
         if self.timerstat == 'idle':
@@ -3296,15 +3298,17 @@
             et = nt - self.start
         if et is not None:
             evec = []
             if self.finish is not None:
                 # event down time is on first finisher
                 ft = (self.finish - self.start).truncate(0)
                 evec.append(ft.rawtime(0))
-                evec.append('+' + (et - ft).rawtime(0))
+                rt = et - ft
+                if rt < MAXELAP:
+                    evec.append('+' + rt.rawtime(0))
 
                 # time limit is applied to total event time/first finisher
                 limit = self.decode_limit(self.timelimit, ft)
                 if limit is not None:
                     evec.append('Limit: +' + (limit - ft).rawtime(0))
             else:
                 evec.append(et.rawtime(0))
@@ -3312,53 +3316,58 @@
                     # prev lap time
                     if self.lapstart is not None:
                         evec.append('Lap: ' +
                                     (self.lapfin - self.lapstart).rawtime(0))
                     # lap down time
                     dt = nt - self.lapfin
                     if dt < MAXELAP:
-                        evec.append('+' + (dt).rawtime(0))
+                        evec.append('+' + dt.rawtime(0))
             elapmsg = '\u2003'.join(evec)
             self.elaplbl.set_text(elapmsg)
             self.meet.cmd_announce('elapmsg', elapmsg)
         else:
             self.elaplbl.set_text('')
             self.meet.cmd_announce('elapmsg', '')
         return True
 
-    def set_start(self, start=''):
+    def set_start(self, start=None):
         """Set the start time."""
         wasidle = self.start is None
-        self.start = tod.mktod(start)
+        if start is not None:
+            if type(start) is not tod.tod:
+                _log.warning('Ignored invalid start time %r', start)
+                start = None
+        self.start = start
         if self.start is not None:
             if wasidle:
                 self.lapstart = None
                 self.lapfin = None
                 self.curlap = -1  # reset lap count at start
                 self.onlap = 1  # leaders are 'onlap'
                 self.meet.cmd_announce('onlap', str(self.onlap))
             if self.finish is None:
                 self.set_running()
             self.meet.cmd_announce('start', self.start.rawtime())
         else:
             self.meet.cmd_announce('start', None)
 
-    def set_finish(self, finish=''):
+    def set_finish(self, finish=None):
         """Set the finish time."""
-        if type(finish) is tod.tod:
-            self.finish = finish
-        else:
-            self.finish = tod.mktod(finish)
+        if finish is not None:
+            if type(finish) is not tod.tod:
+                _log.warning('Ignored invalid finish time %r', finish)
+                finish = None
+        self.finish = finish
         if self.finish is None:
             if self.start is not None:
                 self.set_running()
         else:
             self.meet.cmd_announce('finish', self.finish.rawtime())
             if self.start is None:
-                self.set_start('0')
+                self.set_start(tod.ZERO)
             else:
                 elap = self.finish - self.start
                 dval = self.meet.get_distance()
                 if dval is not None:
                     self.meet.cmd_announce('average',
                                            elap.rawspeed(1000.0 * dval))
 
@@ -3384,33 +3393,61 @@
         self.meet.stat_but.set_sensitive(False)
         if self.finish is None:
             self.set_finish(tod.now())
             _log.info('Finish time forced: %s', self.finish.rawtime())
 
     def info_time_edit_clicked_cb(self, button, data=None):
         """Run an edit times dialog to update event time."""
-        st = ''
-        if self.start is not None:
-            st = self.start.rawtime(2)
-        ft = ''
-        if self.finish is not None:
-            ft = self.finish.rawtime(2)
-        ret = uiutil.edit_times_dlg(self.meet.window, stxt=st, ftxt=ft)
-        if ret[0] == 1:
-            wasrunning = self.timerstat in ['running', 'armfinish']
-            self.set_finish(ret[2])
-            self.set_start(ret[1])
+        sections = {
+            'times': {
+                'object': None,
+                'title': 'times',
+                'schema': {
+                    'title': {
+                        'prompt': 'Manually adjust event time',
+                        'control': 'section',
+                    },
+                    'start': {
+                        'prompt': 'Start:',
+                        'hint': 'Event start time',
+                        'type': 'tod',
+                        'places': 4,
+                        'control': 'short',
+                        'nowbut': True,
+                        'value': self.start,
+                    },
+                    'finish': {
+                        'prompt': 'Finish:',
+                        'hint': 'Event finish time',
+                        'type': 'tod',
+                        'places': 4,
+                        'control': 'short',
+                        'nowbut': True,
+                        'value': self.finish,
+                    },
+                },
+            },
+        }
+        res = uiutil.options_dlg(window=self.meet.window,
+                                 title='Edit times',
+                                 sections=sections)
+        if res['times']['start'][0] or res['times']['finish'][0]:
+            wasrunning = self.timerstat in ('running', 'armfinish')
+            self.set_finish(res['times']['finish'][2])
+            self.set_start(res['times']['start'][2])
             if wasrunning:
                 # flag a recalculate
                 self._dorecalc = True
             else:
                 self.resetcatonlaps()
-                if self.event['type'] in ['criterium', 'circuit', 'cross']:
+                if self.etype in ('criterium', 'circuit', 'cross'):
                     GLib.idle_add(self.armlap)
-            _log.info('Adjusted event times')
+            _log.info('Manually adjusted event times')
+        else:
+            _log.debug('Edit times: no change.')
 
     def editcol_cb(self, cell, path, new_text, col):
         """Edit column callback."""
         new_text = new_text.strip()
         self.riders[path][col] = new_text
 
     def editlap_cb(self, cell, path, new_text, col):
@@ -3484,26 +3521,31 @@
             if rcat in self.catstarts and self.catstarts[rcat] is not None:
                 otxt = self.catstarts[rcat].rawtime(0)
         cr.set_property('text', otxt)
 
     def edit_event_properties(self, window, data=None):
         """Edit event specifics."""
         # set current event type label
-        _CONFIG_SCHEMA['etype']['prompt'] = ROADRACE_TYPES[self.event['type']]
+        _CONFIG_SCHEMA['etype']['prompt'] = ROADRACE_TYPES[self.etype]
 
         # flatten current cat list
         _CONFIG_SCHEMA['categories']['value'] = ' '.join(
             self.get_catlist()).strip()
         res = uiutil.options_dlg(window=self.meet.window,
                                  title='Event Properties',
-                                 schema=_CONFIG_SCHEMA,
-                                 obj=self)
+                                 sections={
+                                     'event': {
+                                         'title': 'Event',
+                                         'schema': _CONFIG_SCHEMA,
+                                         'object': self,
+                                     },
+                                 })
         # handle a change in result categories
-        if res['categories'][0]:
-            self.loadcats(res['categories'][2].upper().split())
+        if res['event']['categories'][0]:
+            self.loadcats(res['event']['categories'][2].upper().split())
             self.load_cat_data()
             if len(self.cats) > 1:
                 _log.info('Loaded result categories: %s',
                           ', '.join(self.cats[0:-1]))
             else:
                 _log.info('Result categories cleared')
         return False
@@ -3577,52 +3619,141 @@
         if newst:
             newst = newst.truncate(0)
         self.riders[path][COL_STOFT] = newst
 
     def editbunch_cb(self, cell, path, new_text, col=None):
         """Edit bunch time on rider view."""
         new_text = new_text.strip()
-        dorecalc = False
-        if not self.showdowntimes:
-            self.showdowntimes = True  # assume edit implies required on result
-        if new_text == '':  # user request to clear also clears RFTIME
-            self.riders[path][COL_RFTIME] = None
-            self.riders[path][COL_MBUNCH] = None
-            self.riders[path][COL_CBUNCH] = None
-            dorecalc = True
-        else:
-            # get 'current bunch time'
-            omb = self.vbunch(self.riders[path][COL_CBUNCH],
-                              self.riders[path][COL_MBUNCH])
-
-            # assign new bunch time
-            nmb = None
-            if '+' in new_text:  # assume a down time
-                oft = tod.ZERO
-                if self.winbunch is not None:
-                    oft = self.winbunch
-                nmb = tod.mktod(new_text.replace('+', ''))
-                if nmb is not None:
-                    nmb += oft
-            elif new_text.startswith('s'):
-                # assume same time as previous rider
-                i = int(path) - 1
-                if i >= 0:
-                    nmb = self.vbunch(self.riders[i][COL_CBUNCH],
-                                      self.riders[i][COL_MBUNCH])
-                else:
-                    _log.info('Ignored same time on first rider')
-            else:
-                nmb = tod.mktod(new_text)
-            if self.riders[path][COL_MBUNCH] != nmb:
-                self.riders[path][COL_MBUNCH] = nmb
-                dorecalc = True
+        dorecalc = self.edit_mbunch(self.riders[path], new_text)
         if dorecalc:
             self.recalculate()
 
+    def get_leader(self, lr=None):
+        """Return the lead rider's bib and bunch time if possible"""
+        leader = None
+        lbt = None
+        if lr is not None and len(self.cats) > 1:
+            cs = lr[COL_CAT]
+            rcat = self.ridercat(riderdb.primary_cat(cs))
+            for r in self.riders:
+                if r[COL_BIB] == lr[COL_BIB]:
+                    _log.debug('Search rider %s is cat %s leader', lr[COL_BIB],
+                               rcat)
+                    break
+                # match against primary cat
+                if rcat == self.ridercat(riderdb.primary_cat(r[COL_CAT])):
+                    lbt = self.vbunch(r[COL_CBUNCH], r[COL_MBUNCH])
+                    if lbt is not None:
+                        leader = r[COL_BIB]
+                        _log.debug('Found cat %s leader: %s', rcat, r[COL_BIB])
+                        break
+        else:
+            lbt = self.vbunch(self.riders[0][COL_CBUNCH],
+                              self.riders[0][COL_MBUNCH])
+            if lbt is not None:
+                leader = self.riders[0][COL_BIB]
+            if lr is not None:
+                if leader == lr[COL_BIB]:
+                    _log.debug('Search rider %s is event leader', lr[COL_BIB])
+                    leader = None
+        return (leader, lbt)
+
+    def edit_mbunch(self, lr=None, bunch=None):
+        """Update manual bunch time and return true if recalc required"""
+        # possible values:
+        #   - Empty or None:  clear manual bunch entry
+        #   - Event time eg:   1h23:45
+        #   - Down time from cat leader eg:  +1:23
+        #   - Same time as previous rider: s
+        #   - Own time (manual time gap): g
+        # Assumes model is in bunch order (work in progress)
+        ret = False
+        if bunch is None or bunch == '':
+            # clear values
+            lr[COL_MBUNCH] = None
+            lr[COL_CBUNCH] = None
+            ret = True
+            _log.info('Cleared manual bunch time for rider %s', lr[COL_BIB])
+        elif lr[COL_PLACE] or lr[COL_COMMENT] == 'otl':
+            bunch = bunch.lower()
+
+            # get current bunch for the rider in question
+            vbt = self.vbunch(lr[COL_CBUNCH], lr[COL_MBUNCH])
+
+            # get previous and next rider info
+            pr = lr.get_previous()
+            pt = None
+            if pr is not None:
+                pt = self.vbunch(pr[COL_CBUNCH], pr[COL_MBUNCH])
+            nr = lr.get_next()
+            nt = None
+            if nr is not None:
+                nt = self.vbunch(nr[COL_CBUNCH], nr[COL_MBUNCH])
+
+            if bunch.startswith('s'):
+                if pr is not None and pt is not None:
+                    ret = True
+                    lr[COL_MBUNCH] = pt
+                    _log.info('Rider %s assigned same bunch as %s: %s',
+                              lr[COL_BIB], pr[COL_BIB], pt.rawtime(0))
+                    if nt is not None and nt == vbt:
+                        # next rider was same time
+                        if nr[COL_MBUNCH] is not None:
+                            nr[COL_MBUNCH] = pt
+                else:
+                    _log.error('No previous rider to set bunch time')
+            elif bunch.startswith('g'):
+                if lr[COL_RFTIME] is not None:
+                    st = tod.ZERO
+                    if self.start is not None:
+                        st = self.start
+                    ret = True
+                    lr[COL_MBUNCH] = (lr[COL_RFTIME] - st).truncate(0)
+                    _log.info('Rider %s assigned new bunch time: %s',
+                              lr[COL_BIB], lr[COL_MBUNCH].rawtime(0))
+                    if nt is not None and nt == vbt:
+                        # next rider was same time
+                        if nr[COL_MBUNCH] is not None:
+                            nr[COL_MBUNCH] = lr[COL_MBUNCH]
+                else:
+                    _log.error('Rider %s does not have arrival time',
+                               lr[COL_BIB])
+            else:
+                # manual override of one bunch time
+                nbt = None
+                if bunch.startswith('+'):
+                    oft = tod.mktod(bunch[1:])
+                    if oft is not None:
+                        leadrider, leadbunch = self.get_leader(lr)
+                        if leadrider is not None and lr[COL_BIB] != leadrider:
+                            nbt = leadbunch + oft
+                            _log.debug('Using rider %s as cat leader',
+                                       leadrider)
+                        else:
+                            _log.debug('No lead rider, %s down time ignored',
+                                       lr[COL_BIB])
+                else:
+                    nbt = tod.mktod(bunch)
+
+                if nbt is not None:
+                    lr[COL_MBUNCH] = nbt.truncate(0)
+                    ret = True
+                    _log.info('Rider %s bunch time set to: %s', lr[COL_BIB],
+                              lr[COL_MBUNCH].rawtime(0))
+                    if nt is not None and nt == vbt:
+                        # next rider was at same time, preserve orignal bunch
+                        nr[COL_MBUNCH] = vbt
+                else:
+                    _log.warning('Invalid bunch time ignored for rider %s',
+                                 lr[COL_BIB])
+        else:
+            _log.error('Cannot edit bunch time on un-placed rider %s',
+                       lr[COL_BIB])
+        return ret
+
     def checkplaces(self, rlist='', dnf=True):
         """Check the proposed places against current event model."""
         ret = True
         placeset = set()
         for no in strops.reformat_biblist(rlist).split():
             if no != 'x':
                 # repetition? - already in place set?
@@ -3720,20 +3851,18 @@
                 if ri is not None:
                     lr = Gtk.TreeModelRow(self.riders, ri)
                     _log.info('Added non-starter from finish places: %r', bib)
                     lr[COL_PLACE] = xfer[bib]
 
     def assign_places(self, contest):
         """Transfer points and bonuses into the named contest."""
-        # fetch context meta infos
         src = self.contestmap[contest]['source']
         if src not in self.reserved_sources and src not in self.intermeds:
             _log.info('Invalid inter source %r in contest %r', src, contest)
             return
-        # todo: remove this countback flag - does not work as expected
         countbackwinner = False  # for stage finish only track winner in cb
         category = self.contestmap[contest]['category']
         tally = self.contestmap[contest]['tally']
         bonuses = self.contestmap[contest]['bonuses']
         points = self.contestmap[contest]['points']
         allsrc = self.contestmap[contest]['all_source']
         allpts = 0
@@ -3742,15 +3871,15 @@
             if len(points) > 0:
                 allpts = points[0]
             if len(bonuses) > 0:
                 allbonus = bonuses[0]
         placestr = ''
         if src == 'fin':
             placestr = self.places
-            if tally in ['sprint', 'crit']:  # really only for sprints/crits
+            if tally in ('sprint', 'crit'):  # really only for sprints/crits
                 countbackwinner = True
         elif src == 'reg':
             placestr = self.get_startlist()
         elif src == 'start':
             placestr = self.get_starters()
         elif src in self.catplaces:  # ERROR -> cat climb tally needs type?
             placestr = self.get_cat_placesr(self.catplaces[src])
@@ -3879,23 +4008,23 @@
             if r[COL_RFTIME] is not None:
                 rftime = r[COL_RFTIME]
             rlaps = r[COL_LAPS]
             lastpass = tod.MAX
             if len(r[COL_RFSEEN]) > 0:
                 lastpass = r[COL_RFSEEN][-1]
                 # in cross scoring, rftime is same as last passing
-                if self.event['type'] == 'cross':
+                if self.etype == 'cross':
                     rftime = lastpass
             if not rplace or not r[COL_INRACE]:
-                rplace = r[COL_COMMENT]
+                rplace == ''
             if not r[COL_INRACE]:
                 rlaps = 0
                 rftime = tod.MAX
                 lastpass = tod.MAX
-            if self.event['type'] in ['road', 'criterium']:
+            if self.etype in ('road', 'criterium'):
                 # partition into seen and not seen
                 if r[COL_INRACE]:
                     if rftime < tod.MAX or lastpass < tod.MAX:
                         rlaps = 999
                     else:
                         rlaps = 0
             auxtbl.append(
@@ -3915,48 +4044,48 @@
         ll = None  # lap count of previous competitor for cross scoring
         bt = None  # the 'current' bunch time
         if self.start is not None:
             for r in self.riders:
                 rcomment = r[COL_COMMENT]
                 if r[COL_INRACE] or rcomment == 'otl':
                     rtime = r[COL_RFTIME]
-                    if self.event['type'] in ['cross', 'circuit']:
+                    if self.etype in ('cross', 'circuit'):
                         if ll is None or ll != r[COL_LAPS]:
                             # invalidate last passing since on a different lap
                             lt = None
                             bt = None
                             ll = r[COL_LAPS]
                     if r[COL_MBUNCH] is not None:
                         bt = r[COL_MBUNCH]  # override with manual bunch
                         r[COL_CBUNCH] = bt
                         if ft is None:
                             ft = bt
-                        lt = bt
+                        lt = rtime
                     elif rtime is not None:
                         # establish elapsed, but allow subsequent override
                         if rtime > self.maxfinish:
                             self.maxfinish = rtime
                         et = rtime - self.start
 
                         # establish bunch time
                         if ft is None and r[COL_RFTIME] is not None:
                             racefinish = r[COL_RFTIME]  # save race finish
                             ft = et.truncate(0)  # compute first time
                             bt = ft
                         else:
-                            if lt is not None and (et < lt or
-                                                   et - lt < self.gapthresh):
+                            if lt is not None and (
+                                    rtime < lt or rtime - lt < self.gapthresh):
                                 # same time
                                 pass
                             else:
                                 bt = et.truncate(0)
 
                         # assign and continue
                         r[COL_CBUNCH] = bt
-                        lt = et
+                        lt = rtime
                     else:
                         # empty rftime with non-empty rank implies no time gap
                         if r[COL_PLACE]:
                             r[COL_CBUNCH] = bt  # use current bunch time
                         else:
                             r[COL_CBUNCH] = None
 
@@ -3968,31 +4097,30 @@
 
         # if racefinish defined, call set finish
         if racefinish:
             self.set_finish(racefinish)
 
         # re-sort on in,vbunch (not valid for cross scoring)
         # at this point all finished riders will have valid bunch time
-        if self.event['type'] != 'cross':
+        if self.etype != 'cross':
             auxtbl = []
             idx = 0
             for r in self.riders:
                 # aux cols: ind, bib, in, place, vbunch
                 rbib = r[COL_BIB]
                 rplace = r[COL_PLACE]
                 rlaps = r[COL_LAPS]
                 rbunch = self.vbunch(r[COL_CBUNCH], r[COL_MBUNCH])
                 if rbunch is None:
                     rbunch = tod.MAX
-                if not rplace or not r[COL_INRACE]:
-                    rplace = r[COL_COMMENT]
                 if not r[COL_INRACE]:
+                    rplace = r[COL_COMMENT]
                     rlaps = 0
-                elif self.event['type'] in ['road', 'criterium']:
-                    # group all finished riders
+                elif self.etype in ('road', 'criterium'):
+                    # group all finished riders on same 'lap'
                     if rbunch < tod.MAX or r[COL_RFTIME] is not None:
                         rlaps = 999
                 auxtbl.append((not r[COL_INRACE], strops.dnfcode_key(rplace),
                                -rlaps, rbunch, idx))
                 idx += 1
             if len(auxtbl) > 1:
                 auxtbl.sort()
@@ -4027,16 +4155,14 @@
                                 r[COL_COMMENT] = 'otl'
                                 handled += 1
                             else:  # and clear if not
                                 if r[COL_COMMENT] == 'otl':
                                     r[COL_COMMENT] = ''
                 else:
                     handled += 1
-            if ft is not None:
-                self.winbunch = ft
             if self.timerstat == 'finished' or handled == tot:
                 self.racestat = 'final'
             else:
                 if placed >= 10 or (placed > 0 and tot < 16):
                     self.racestat = 'provisional'
                 else:
                     self.racestat = 'virtual'
@@ -4055,23 +4181,23 @@
     def new_start_trigger(self, rfid):
         """Collect a timer trigger signal and apply it to the model."""
         if self.newstartdlg is not None and self.newstartent is not None:
             et = tod.mktod(self.newstartent.get_text())
             if et is not None:
                 dlg = self.newstartdlg
                 self.newstartdlg = None
-                wasrunning = self.timerstat in ['running', 'armfinish']
+                wasrunning = self.timerstat in ('running', 'armfinish')
                 st = rfid - et
                 self.set_start(st)
                 if wasrunning:
                     # flag a recalculate
                     self._dorecalc = True
                 else:
                     self.resetcatonlaps()
-                    if self.event['type'] in ['criterium', 'circuit', 'cross']:
+                    if self.etype in ('criterium', 'circuit', 'cross'):
                         GLib.idle_add(self.armlap)
                 dlg.response(1)
             else:
                 _log.warning('Invalid elapsed time: Start not updated')
         return False
 
     def new_start_trig(self, button, entry=None):
@@ -4115,15 +4241,15 @@
         finally:
             self.meet.timercb = self.timertrig
             dlg.destroy()
 
     #def treerow_selected(self, treeview, path, view_column, data=None):
     #"""Select row, confirm only selected place"""
     ## filter on running/armfinish
-    #if self.timerstat not in ['idle', 'armstart', 'finished']:
+    #if self.timerstat not in ('idle', 'armstart', 'finished'):
     #if self.finish is not None:
     #rbib = self.riders[path][COL_BIB]
     #_log.info('Confirmed next place by tree selection: %r/%r',
     #rbib, path)
     #self.append_selected_place()
 
     def treeview_button_press(self, treeview, event):
@@ -4257,18 +4383,17 @@
         if ret == 1:
             dstbib = dst_ent.get_text()
             if dstbib != srcbib:
                 dr = self.getrider(dstbib)
                 if dr is not None:
                     self.placeswap(dstbib, srcbib)
                     sr = self.getrider(srcbib)
-                    for col in [
-                            COL_COMMENT, COL_INRACE, COL_PLACE, COL_LAPS,
-                            COL_RFTIME, COL_CBUNCH, COL_MBUNCH, COL_RFSEEN
-                    ]:
+                    for col in (COL_COMMENT, COL_INRACE, COL_PLACE, COL_LAPS,
+                                COL_RFTIME, COL_CBUNCH, COL_MBUNCH,
+                                COL_RFSEEN):
                         tv = dr[col]
                         dr[col] = sr[col]
                         sr[col] = tv
                     _log.info('Swap riders %r <=> %r', srcbib, dstbib)
                     # If srcrider was a spare bike, remove the spare and patch
                     if spare:
                         ac = [t for t in sr[COL_RFSEEN]]
@@ -4286,49 +4411,181 @@
         else:
             _log.info('Swap rider cancelled')
         dlg.destroy()
 
     def rms_context_edit_activate_cb(self, menuitem, data=None):
         """Edit rider start/finish/etc."""
         sel = self.view.get_selection().get_selected()
-        if sel is not None:
-            stx = ''
-            ftx = ''
-            btx = ''
-            ptx = ''
-            st = self.riders.get_value(sel[1], COL_STOFT)
-            ft = self.riders.get_value(sel[1], COL_RFTIME)
-            bt = self.riders.get_value(sel[1], COL_BONUS)
-            pt = self.riders.get_value(sel[1], COL_PENALTY)
-            if st:
-                stx = st.rawtime()
-            if ft:
-                ftx = ft.rawtime()
-            if bt:
-                btx = bt.rawtime()
-            if pt:
-                ptx = pt.rawtime()
-            tvec = uiutil.edit_times_dlg(self.meet.window, stx, ftx, btx, ptx,
-                                         True, True)  # enable bon+pen
-            if len(tvec) > 4 and tvec[0] == 1:
-                self.riders.set_value(sel[1], COL_STOFT, tod.mktod(tvec[1]))
-                self.riders.set_value(sel[1], COL_RFTIME, tod.mktod(tvec[2]))
-                self.riders.set_value(sel[1], COL_BONUS, tod.mktod(tvec[3]))
-                self.riders.set_value(sel[1], COL_PENALTY, tod.mktod(tvec[4]))
-                bib = self.riders.get_value(sel[1], COL_BIB)
-                nst = '-'
-                st = self.riders.get_value(sel[1], COL_STOFT)
-                if st:
-                    nst = st.rawtime(0)
-                nft = '-'
-                ft = self.riders.get_value(sel[1], COL_RFTIME)
-                if ft:
-                    nft = ft.rawtime(2)
-                _log.info('Adjust rider %r start:%s, finish:%s', bib, nst, nft)
-                self.recalculate()
+        if sel is None:
+            return False
+
+        lr = Gtk.TreeModelRow(self.riders, sel[1])
+        st = lr[COL_STOFT]
+        stextra = ''
+        if not st:
+            # check for a category start time
+            cs = lr[COL_CAT]
+            rcat = self.ridercat(riderdb.primary_cat(cs))
+            if rcat in self.catstarts and self.catstarts[rcat] is not None:
+                st = self.catstarts[rcat]
+                stextra = '[Cat start: %s]' % (rcat)
+
+        lastpass = None
+        if len(lr[COL_RFSEEN]) > 0:
+            lastpass = lr[COL_RFSEEN][-1]
+        placestr = None
+        if lr[COL_COMMENT]:
+            placestr = lr[COL_COMMENT]
+        placeopts = {
+            '': 'Unclassified',
+            'dns': 'Did not start',
+            'otl': 'Outside time limit',
+            'dnf': 'Did not finish',
+            'dsq': 'Disqualified',
+        }
+        if lr[COL_PLACE]:
+            placeopts['plc'] = 'Placed ' + strops.rank2ord(lr[COL_PLACE])
+        if lr[COL_INRACE]:
+            if lr[COL_PLACE]:
+                placestr = 'plc'
+        if placestr is not None and placestr not in placeopts:
+            placeopts[placestr] = placestr
+        manbunch = None
+        if lr[COL_MBUNCH] is not None:
+            manbunch = lr[COL_MBUNCH].rawtime(0)
+        sections = {
+            'result': {
+                'object': None,
+                'title': 'result',
+                'schema': {
+                    'title': {
+                        'prompt': lr[COL_BIB] + ' ' + lr[COL_NAMESTR],
+                        'control': 'section',
+                    },
+                    'seed': {
+                        'prompt': 'Seed:',
+                        'hint': 'Seeding number for startlists',
+                        'control': 'short',
+                        'type': 'int',
+                        'value': lr[COL_SEED],
+                        'index': COL_SEED,
+                    },
+                    'class': {
+                        'prompt': 'Classification:',
+                        'hint': 'Rider classification for event',
+                        'control': 'choice',
+                        'value': placestr,
+                        'options': placeopts,
+                        'default': '',
+                    },
+                    'start': {
+                        'prompt': 'Start Offset:',
+                        'hint': 'Start offset',
+                        'type': 'tod',
+                        'places': 0,
+                        'control': 'short',
+                        'value': st,
+                        'subtext': stextra,
+                        'index': COL_STOFT,
+                    },
+                    'laps': {
+                        'prompt': 'Laps:',
+                        'hint': 'Rider lap count',
+                        'control': 'short',
+                        'type': 'int',
+                        'value': lr[COL_LAPS],
+                        'index': COL_LAPS,
+                    },
+                    'lpass': {
+                        'prompt': 'Last Pass:',
+                        'hint': 'Time last seen at finish line',
+                        'type': 'tod',
+                        'places': 4,
+                        'readonly': 'true',
+                        'control': 'short',
+                        'value': lastpass,
+                    },
+                    'rftime': {
+                        'prompt': 'Finish:',
+                        'hint': 'Time of arrival at event finish',
+                        'type': 'tod',
+                        'places': 4,
+                        'value': lr[COL_RFTIME],
+                        'nowbut': True,
+                        'control': 'short',
+                        'subtext': 'Set finish time to now',
+                        'index': COL_RFTIME,
+                    },
+                    'cbunch': {
+                        'prompt': 'Bunch:',
+                        'hint': 'Computed bunch time',
+                        'type': 'tod',
+                        'places': 0,
+                        'value': lr[COL_CBUNCH],
+                        'control': 'short',
+                        'readonly': 'true',
+                    },
+                    'mbunch': {
+                        'prompt': 'Man Bunch:',
+                        'hint': 'Override computed bunch time',
+                        'places': 0,
+                        'value': manbunch,
+                        'control': 'short',
+                    },
+                    'bonus': {
+                        'prompt': 'Stage Bonus:',
+                        'hint': 'Additional stage bonus time',
+                        'type': 'tod',
+                        'places': 0,
+                        'value': lr[COL_BONUS],
+                        'control': 'short',
+                        'index': COL_BONUS,
+                    },
+                    'penalty': {
+                        'prompt': 'Stage Penalty:',
+                        'hint': 'Additional stage penalty time',
+                        'type': 'tod',
+                        'places': 0,
+                        'value': lr[COL_PENALTY],
+                        'control': 'short',
+                        'index': COL_PENALTY,
+                    },
+                },
+            },
+        }
+        res = uiutil.options_dlg(window=self.meet.window,
+                                 title='Edit times',
+                                 sections=sections)
+        changed = False
+        for option in res['result']:
+            if res['result'][option][0]:
+                changed = True
+                if 'index' in sections['result']['schema'][option]:
+                    index = sections['result']['schema'][option]['index']
+                    lr[index] = res['result'][option][2]
+                    _log.debug('Updated %s to: %r', option,
+                               res['result'][option][2])
+                elif option == 'class':
+                    newclass = res['result'][option][2]
+                    if newclass is None:
+                        newclass = ''
+                    if newclass in ('dns', 'otl', 'dnf', 'dsq'):
+                        lr[COL_INRACE] = False
+                    else:
+                        lr[COL_INRACE] = True
+                    if newclass != 'plc':
+                        lr[COL_COMMENT] = newclass
+                        if res['result'][option][1] == 'plc':
+                            self.clear_place(lr[COL_BIB])
+                elif option == 'mbunch':
+                    self.edit_mbunch(lr, res['result'][option][2])
+                else:
+                    _log.debug('Unknown option %r changed', option)
+        if changed:
+            self.recalculate()
 
     def rms_context_chg_activate_cb(self, menuitem, data=None):
         """Update selected rider from event."""
         change = menuitem.get_label().lower()
         sel = self.view.get_selection().get_selected()
         bib = None
         if sel is not None:
@@ -4347,56 +4604,54 @@
                 if splits is not None and len(splits) > 0:
                     nf = splits[-1]
                     _log.info(
                         'Set raw finish for rider %r to last passing: %s',
                         selbib, nf.rawtime(2))
                     self.riders.set_value(i, COL_RFTIME, nf)
                     self.recalculate()
-            elif change in ['dns', 'dnf', 'wd', 'otl', 'dsq']:
+            elif change in ('dns', 'dnf', 'wd', 'otl', 'dsq'):
                 self.dnfriders(selbib, change)
             elif change == 'return':
                 self.retriders(selbib)
             elif change == 'passing':
                 self.manpassing(selbib)
             else:
                 _log.info('Unknown rider change %r ignored', change)
 
-    def __init__(self, meet, event, ui=True):
+    def __init__(self, meet, etype, ui=True):
         self.meet = meet
-        self.event = event
-        self.evno = event['evid']
-        self.series = event['seri']
-        self.configfile = meet.event_configfile(self.evno)
+        self.etype = etype
+        self.series = ''
+        self.configfile = 'event.json'
         self.readonly = not ui
         rstr = ''
         if self.readonly:
             rstr = 'readonly '
-        _log.debug('Init %r event %r', rstr, self.evno)
+        _log.debug('Init %r event', rstr)
 
         self.recalclock = threading.Lock()
         self._dorecalc = False
 
         # event run time attributes
         self.calcset = False
         self.start = None
         self.finish = None
         self.altfinish = None
         self.maxfinish = None
         self.showdowntimes = True
-        self.winbunch = None  # bunch time of winner (overall race time)
         self.winopen = True
         self.timerstat = 'idle'
         self.racestat = 'prerace'
         self.places = ''
         self.laptimes = []
-        self.comment = []
+        self.decisions = []
         self.hidecols = []
         self.cats = []
         self.passingsource = []  # list of decoders we accept passings from
-        self.targetlaps = False  # true if finish is det by target
+        self.autofinish = False  # true if finish is det by target
         self.catlaps = {}  # cache of cat lap counts
         self.catstarts = {}  # cache of cat start times
         self.catplaces = {}
         self.autocats = False
         self.autostartlist = None
         self.bonuses = {}
         self.points = {}
```

### Comparing `metarace-roadmeet-1.13.1/src/roadmeet/trtt.py` & `metarace-roadmeet-1.13.2/src/roadmeet/trtt.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from metarace import strops
 from metarace import report
 from metarace import jsonconfig
 from . import uiutil
 
 from roadmeet.rms import rms, RESERVED_SOURCES, GAPTHRESH
 
-_log = logging.getLogger('metarace.trtt')
+_log = logging.getLogger('trtt')
 _log.setLevel(logging.DEBUG)
 
 # trtt adds team reference to rms model
 # basic infos
 COL_BIB = 0
 COL_NAMESTR = 1
 COL_SHORTNAME = 2
@@ -50,126 +50,145 @@
 
 # Nth wheel decides whose time is counted to the team
 NTH_WHEEL = 3
 
 # Minimum lap/elap time, should be at least the same as start gaps
 MINLAP = tod.tod('2:00')
 
-# Add a gap in the startlist when gap is larger than TEAMGAP
-TEAMGAP = tod.tod('4:00')
+# Add a gap in the startlist when gap is larger than STARTGAP
+STARTGAP = tod.tod('4:00')
 
 # config version string
 EVENT_ID = 'trtt-3.1'
 
 _CONFIG_SCHEMA = {
     'etype': {
         'prompt': 'Team Time Trial',
-        'control': 'section'
+        'control': 'section',
     },
     'categories': {
         'prompt': 'Categories:',
         'hint': 'Startlist and result categories',
-        'defer': True
+        'defer': True,
+        'default': '',
     },
     'minlap': {
         'prompt': 'Minimum Lap:',
         'control': 'short',
         'places': 1,
         'type': 'tod',
         'hint': 'Reject laps shorter than minimum lap time',
-        'attr': 'minlap'
+        'attr': 'minlap',
+        'default': MINLAP,
     },
     'totlaps': {
         'prompt': 'Laps:',
         'control': 'short',
         'type': 'int',
         'attr': 'totlaps',
         'subtext': '(Cat laps override)',
-        'hint': 'Default target number of laps for event'
+        'hint': 'Default target number of laps for event',
     },
     'defaultnth': {
         'prompt': 'Nth Wheel:',
         'control': 'short',
         'type': 'int',
         'attr': 'defaultnth',
-        'hint': 'Default wheel to determine team time'
+        'hint': 'Default wheel to determine team time',
+        'default': NTH_WHEEL,
     },
     'owntime': {
         'prompt': 'Own Time:',
         'control': 'check',
         'type': 'bool',
         'attr': 'owntime',
         'subtext': 'Dropped riders get own time?',
         'hint': 'Award riders finishing behind team their own time',
+        'default': True,
     },
     'showriders': {
         'prompt': 'Show Riders:',
         'control': 'check',
         'type': 'bool',
         'attr': 'showriders',
         'subtext': 'Display team member names on reports?',
         'hint': 'Include rider names on startlists and results',
+        'default': True,
+    },
+    'startgap': {
+        'prompt': 'Start Gap:',
+        'control': 'short',
+        'type': 'tod',
+        'places': 0,
+        'attr': 'startgap',
+        'hint': 'Time gap between team start times',
+        'default': STARTGAP,
     },
     'relativestart': {
         'prompt': 'Relative:',
         'control': 'check',
         'type': 'bool',
         'attr': 'relativestart',
         'subtext': 'Team start times are relative?',
         'hint': 'Team start times are relative to event start',
+        'default': False,
     },
     'autofinish': {
         'prompt': 'Finish:',
         'control': 'check',
         'type': 'bool',
-        'attr': 'targetlaps',
+        'attr': 'autofinish',
         'subtext': 'Automatically Finish?',
         'hint': 'Automatically finish riders on target lap',
+        'default': True,
     },
     'autoexport': {
         'prompt': 'Export:',
         'control': 'check',
         'type': 'bool',
         'attr': 'autoexport',
         'subtext': 'Automatically export?',
         'hint': 'Export result automatically',
+        'default': False,
     },
     # Note: on trtt, time limit usually requires manual intervention
     'timelimit': {
         'prompt': 'Time Limit:',
-        'control': 'short',
+        'control': 'none',
         'attr': 'timelimit',
         'readonly': True,
-        'hint': 'Time limit eg: 12%  +1:23  4h00:00'
+        'hint': 'Time limit eg: 12%  +1:23  4h00:00',
     },
     'gapthresh': {
         'prompt': 'Time Gap:',
         'control': 'short',
         'type': 'tod',
         'places': 2,
         'hint': 'Threshold for automatic time gap insertion',
-        'attr': 'gapthresh'
+        'attr': 'gapthresh',
+        'default': GAPTHRESH,
     },
-    # Clubmode may trigger problems with team data, todo: fix addrider
     'clubmode': {
         'prompt': 'Club Mode:',
-        'control': 'check',
+        'control': 'none',
         'type': 'bool',
         'attr': 'clubmode',
         'readonly': True,
         'subtext': 'Add starters by transponder passing?',
         'hint': 'Add riders to event on passing',
+        'default': False,
     },
     'allowspares': {
         'prompt': 'Spares:',
         'control': 'check',
         'type': 'bool',
         'attr': 'allowspares',
         'subtext': 'Record spare bike passings?',
         'hint': 'Add spare bike passings to event as placeholders',
+        'default': False,
     },
 }
 
 
 class trtt(rms):
 
     def team_start_times(self):
@@ -215,79 +234,66 @@
         self.riders.clear()
         self.resettimer()
         self.cats = []
 
         cr = jsonconfig.config({
             'trtt': {
                 'start': None,
-                'id': EVENT_ID,
                 'finished': False,
-                'relativestart': False,
-                'showriders': True,
                 'places': '',
-                'comment': [],
-                'categories': [],
+                'decisions': [],
                 'intermeds': [],
-                'allowspares': False,
                 'contests': [],
                 'tallys': [],
-                'owntime': True,
-                'gapthresh': None,
-                'totlaps': None,
                 'passingsource': [],
-                'defaultnth': NTH_WHEEL,
-                'minlap': None,
-                'clubmode': False,
                 'nthwheel': {},
                 'startlist': '',
-                'autofinish': False,
-                'autoexport': False,
             }
         })
-        cr.add_section('trtt')
+        cr.add_section('trtt', _CONFIG_SCHEMA)
         cr.add_section('riders')
         cr.add_section('stagebonus')
         cr.add_section('stagepenalty')
         cr.merge(metarace.sysconf, 'trtt')
         if not cr.load(self.configfile):
             _log.info('%r not read, loading defaults', self.configfile)
+        cr.export_section('trtt', self)
 
         # load result categories
-        self.loadcats(cr.get('trtt', 'categories'))
+        self.loadcats(cr.get_value('trtt', 'categories').upper().split())
 
-        # read in default and category specific nth wheel values
-        self.defaultnth = cr.get_posint('trtt', 'defaultnth')
+        # read in category specific nth wheel overrides
         _log.debug('Default Nth Wheel: %r', self.defaultnth)
         self.nthwheel = cr.get('trtt', 'nthwheel')
         if not isinstance(self.nthwheel, dict):
             _log.warning('Invalid nthwheel setting ignored: %r', self.nthwheel)
             self.nthwheel = {}
         if len(self.nthwheel) > 0:
             _log.debug('Nth Wheel: %r', self.nthwheel)
 
         self.passingsource = []
         for source in cr.get('trtt', 'passingsource'):
             self.passingsource.append(source.lower())  # force lower case
 
-        # fetch time gap threshold
-        ngt = tod.mktod(cr.get('trtt', 'gapthresh'))
-        if ngt is not None:
-            self.gapthresh = ngt
-            if self.gapthresh != GAPTHRESH:
-                _log.warning('Set time gap threshold %s',
-                             self.gapthresh.rawtime(2))
+        # check gapthresh
+        if self.gapthresh != GAPTHRESH:
+            _log.warning('Set time gap threshold %s',
+                         self.gapthresh.rawtime(2))
+        _log.debug('Minimum lap time: %s', self.minlap.rawtime(1))
+
+        # team start gap
+        if self.startgap != STARTGAP:
+            _log.info('Team start gap %s', self.startgap.rawtime(0))
 
         # restore stage inters, points and bonuses
         self.loadstageinters(cr, 'trtt')
 
         # load competitors
-        starters = cr.get('trtt', 'startlist').split()
-        if len(starters) == 1 and starters[0] == 'all':
-            starters = strops.riderlist_split('all', self.meet.rdb)
-        self.allowspares = cr.get_bool('trtt', 'allowspares')
+        starters = strops.riderlist_split(
+            cr.get('trtt', 'startlist').upper().strip(), self.meet.rdb)
         for r in starters:
             ri = self.addrider(r)
             if ri is not None:
                 nr = Gtk.TreeModelRow(self.riders, ri)
                 if cr.has_option('riders', r):
                     # bib = comment,in,laps,rftod,mbunch,rfseen...
                     ril = cr.get('riders', r)  # rider op is vec
@@ -307,51 +313,36 @@
                     if lr > 6:
                         for i in range(6, lr):
                             laptod = tod.mktod(ril[i])
                             if laptod is not None:
                                 nr[COL_RFSEEN].append(laptod)
                 # record any extra bonus/penalty to rider model
                 if cr.has_option('stagebonus', r):
-                    nr[COL_BONUS] = tod.mktod(cr.get('stagebonus', r))
+                    nr[COL_BONUS] = cr.get_tod('stagebonus', r)
                 if cr.has_option('stagepenalty', r):
-                    nr[COL_PENALTY] = tod.mktod(cr.get('stagepenalty', r))
-
-        self.owntime = cr.get_bool('trtt', 'owntime')
-        self.minlap = tod.mktod(cr.get('trtt', 'minlap'))
-        if self.minlap is None:
-            self.minlap = MINLAP
-        _log.debug('Minimum lap time: %s', self.minlap.rawtime())
+                    nr[COL_PENALTY] = cr.get_tod('stagepenalty', r)
 
         self.set_start(cr.get('trtt', 'start'))
-        self.totlaps = cr.get('trtt', 'totlaps')
         self.places = strops.reformat_placelist(cr.get('trtt', 'places'))
-        self.comment = cr.get('trtt', 'comment')
-        self.autoexport = cr.get_bool('trtt', 'autoexport')
-        self.showriders = cr.get_bool('trtt', 'showriders')
-        self.relativestart = cr.get_bool('trtt', 'relativestart')
+        self.decisions = cr.get('trtt', 'decisions')
         if strops.confopt_bool(cr.get('trtt', 'finished')):
             self.set_finished()
-        self.clubmode = cr.get_bool('trtt', 'clubmode')
         self.recalculate()
 
         self.load_cat_data()
 
         if self.totlaps is not None:
             self.totlapentry.set_text(str(self.totlaps))
 
         # patch team start times from riderdb
         self.team_start_times()
 
-        if cr.get_bool('trtt', 'autofinish'):
-            # then override targetlaps if autofinish was set
-            self.targetlaps = True
-
         # After load complete - check config and report.
-        eid = cr.get('trtt', 'id')
-        if eid and eid != EVENT_ID:
+        eid = cr.get_value('trtt', 'id')
+        if eid is not None and eid != EVENT_ID:
             _log.info('Event config mismatch: %r != %r', eid, EVENT_ID)
             self.readonly = True
 
     def load_cat_data(self):
         self.catlaps = {}
         onetarget = False
         onemissing = False
@@ -365,15 +356,15 @@
                     if lt:
                         ls = lt
                         onetarget = True
                     else:
                         onemissing = True
             self.catlaps[c] = ls
         if onetarget:
-            self.targetlaps = True
+            self.autofinish = True
             if onemissing:
                 # There's one or more cats without a target, issue warning
                 missing = []
                 for c in self.catlaps:
                     if self.catlaps[c] is None:
                         missing.append(repr(c))
                 if missing:
@@ -383,51 +374,37 @@
 
     def saveconfig(self):
         """Save event config to disk."""
         if self.readonly:
             _log.error('Attempt to save readonly event')
             return
         cw = jsonconfig.config()
-        cw.add_section('trtt')
-        if self.start is not None:
-            cw.set('trtt', 'start', self.start.rawtime())
-        if self.minlap is not None:
-            cw.set('trtt', 'minlap', self.minlap.rawtime())
-        else:
-            cw.set('trtt', 'minlap', None)
-        cw.set('trtt', 'showriders', self.showriders)
-        cw.set('trtt', 'relativestart', self.relativestart)
-        cw.set('trtt', 'gapthresh', self.gapthresh.rawtime())
+        cw.add_section('trtt', _CONFIG_SCHEMA)
+        cw.import_section('trtt', self)
+        cw.set('trtt', 'start', self.start)
         cw.set('trtt', 'finished', self.timerstat == 'finished')
         cw.set('trtt', 'places', self.places)
-        cw.set('trtt', 'totlaps', self.totlaps)
-        cw.set('trtt', 'allowspares', self.allowspares)
-        cw.set('trtt', 'defaultnth', self.defaultnth)
-        cw.set('trtt', 'owntime', self.owntime)
-        cw.set('trtt', 'autofinish', self.targetlaps)
-        cw.set('trtt', 'autoexport', self.autoexport)
         cw.set('trtt', 'passingsource', self.passingsource)
-        cw.set('trtt', 'clubmode', self.clubmode)
         cw.set('trtt', 'nthwheel', self.nthwheel)  # dict of cat keys
 
         # save stage inters, points and bonuses
         self.savestageinters(cw, 'trtt')
 
         # save riders
         evtriders = self.get_startlist()
         if evtriders:
             cw.set('trtt', 'startlist', self.get_startlist())
         else:
             if self.autostartlist is not None:
                 cw.set('trtt', 'startlist', self.autostartlist)
         if self.autocats:
-            cw.set('trtt', 'categories', ['AUTO'])
+            cw.set('trtt', 'categories', 'AUTO')
         else:
-            cw.set('trtt', 'categories', self.get_catlist())
-        cw.set('trtt', 'comment', self.comment)
+            cw.set('trtt', 'categories', ' '.join(self.get_catlist()).strip())
+        cw.set('trtt', 'decisions', self.decisions)
 
         cw.add_section('riders')
         # sections for commissaire awarded bonus/penalty
         cw.add_section('stagebonus')
         cw.add_section('stagepenalty')
         for r in self.riders:
             rt = ''
@@ -443,35 +420,40 @@
             bib = r[COL_BIB]
             slice = [r[COL_COMMENT], r[COL_INRACE], r[COL_LAPS], rt, mb, sto]
             for t in r[COL_RFSEEN]:
                 if t is not None:
                     slice.append(t.rawtime())
             cw.set('riders', bib, slice)
             if r[COL_BONUS] is not None:
-                cw.set('stagebonus', bib, r[COL_BONUS].rawtime())
+                cw.set('stagebonus', bib, r[COL_BONUS])
             if r[COL_PENALTY] is not None:
-                cw.set('stagepenalty', bib, r[COL_PENALTY].rawtime())
+                cw.set('stagepenalty', bib, r[COL_PENALTY])
         cw.set('trtt', 'id', EVENT_ID)
         _log.debug('Saving event config %r', self.configfile)
         with metarace.savefile(self.configfile) as f:
             cw.write(f)
 
     def edit_event_properties(self, window, data=None):
         """Edit event specifics."""
 
         # flatten current cat list
         _CONFIG_SCHEMA['categories']['value'] = ' '.join(
             self.get_catlist()).strip()
         res = uiutil.options_dlg(window=self.meet.window,
                                  title='Event Properties',
-                                 schema=_CONFIG_SCHEMA,
-                                 obj=self)
+                                 sections={
+                                     'event': {
+                                         'title': 'Event',
+                                         'schema': _CONFIG_SCHEMA,
+                                         'object': self,
+                                     },
+                                 })
         # handle a change in result categories
-        if res['categories'][0]:
-            self.loadcats(res['categories'][2].split())
+        if res['event']['categories'][0]:
+            self.loadcats(res['event']['categories'][2].upper().split())
             self.load_cat_data()
         return False
 
     def set_titlestr(self, titlestr=None):
         """Update the title string label."""
         if titlestr is None or titlestr == '':
             titlestr = '[Team Time Trial]'
@@ -521,15 +503,14 @@
             rteam = r[COL_TEAM]
             rstart = r[COL_STOFT]
             ruci = None
             tuci = None
             if rstart is None:
                 rstart = tod.MAX
             if rteam != lteam:  # issue team time
-                ltod = None
                 cs = r[COL_CAT]
                 tcat = self.ridercat(riderdb.primary_cat(cs))
                 dbr = self.meet.rdb.get_rider(rteam, 'team')
                 if dbr is not None:
                     tuci = dbr['uci id']
                 if not tuci and tcat == '':
                     tuci = cs
@@ -555,15 +536,15 @@
                         if footer:
                             sec.footer = footer
                 lcat = tcat
 
                 tname = rteam  # use key and only replace if avail
                 if rteam in self.teamnames:
                     tname = self.teamnames[rteam]
-                if ltod is not None and rstart - ltod > TEAMGAP:
+                if ltod is not None and rstart - ltod > self.startgap:
                     sec.lines.append([])
                 ltod = rstart
                 cstr = ''
                 tcount += 1
                 tcodestr = rteam.upper()
                 if rteam.isdigit():
                     tcodestr = None
@@ -631,15 +612,15 @@
         return cnt
 
     def camera_report(self):
         """Return the judges (camera) report."""
         # Note: camera report treats all riders as a single blob
         ret = []
         self.recalculate()  # fill places and bunch info, order by arrival
-        pthresh = self.meet.timer.photothresh()
+        pthresh = self.meet._timer.photothresh()
         totcount = 0
         dnscount = 0
         dnfcount = 0
         fincount = 0
         lcomment = ''
         insertgap = True
         teamCount = {}
@@ -807,39 +788,42 @@
             _log.warning('Event is idle, report not available')
         return ret
 
     def single_catresult(self, cat):
         _log.debug('Cat result for cat=%r', cat)
         ret = []
         allin = False
-        catname = cat  # fallback emergency
+        catname = cat
+        secid = 'result'
         if cat == '':
             if len(self.cats) > 1:
                 catname = 'Uncategorised Riders'
             else:
                 # There is only one cat - so all riders are in it
                 allin = True
+        else:
+            secid = 'result-' + cat.lower()
         subhead = ''
         footer = ''
         distance = self.meet.get_distance()
         laps = self.totlaps
-        if self.catlaps[cat] is not None:
+        if cat in self.catlaps and self.catlaps[cat] is not None:
             laps = self.catlaps[cat]
         dbr = self.meet.rdb.get_rider(cat, 'cat')
         if dbr is not None:
             catname = dbr['title']
             subhead = dbr['subtitle']
             footer = dbr['footer']
             dist = dbr['distance']
             if dist:
                 try:
                     distance = float(dist)
                 except Exception:
                     _log.warning('Invalid distance %r for cat %r', dist, cat)
-        sec = report.section('result-' + cat)
+        sec = report.section(secid)
 
         teamRes = {}
         teamAux = []
         teamCnt = 0
         finCnt = 0
 
         # find all teams and riders in the chosen cat
@@ -848,15 +832,19 @@
             rcats = ['']
             if rcat.strip():
                 rcats = rcat.split()
             incat = False
             if allin or (cat and cat in rcats):
                 incat = True  # rider is in this category
             elif not cat:  # is the rider uncategorised?
-                incat = rcats[0] not in self.cats  # backward logic
+                if rcats[0] == '':
+                    incat = True
+                else:
+                    # exclude properly categorised riders
+                    incat = rcats[0] not in self.cats
             if incat:
                 rteam = r[COL_TEAM]
                 if rteam not in teamRes:
                     teamCnt += 1
                     teamRes[rteam] = {}
                     teamRes[rteam]['time'] = None
                     teamRes[rteam]['rlines'] = []
@@ -919,51 +907,44 @@
             first = False
             sec.lines.append(teamRes[team]['tline'])
             if self.showriders:
                 sec.lines.extend(teamRes[team]['rlines'])
 
             lt = teamTime
 
-        if self.timerstat == 'finished':
+        if self.timerstat in ('idle', 'finished'):
             sec.heading = 'Result'
-        elif self.timerstat in ['idle', 'armstart']:
-            sec.heading = ''
-        elif self.timerstat in ['running', 'armfinish']:
+        elif self.timerstat in ('armstart', 'running', 'armfinish'):
             if teamCnt == finCnt:
                 sec.heading = 'Provisional Result'
             elif finCnt > 0:
                 sec.heading = 'Virtual Standing'
             else:
                 sec.heading = 'Event in Progress'
         else:
             sec.heading = 'Provisional Result'
         if footer:
             sec.footer = footer
 
-        # Append all result categories and uncat if riders
-        if cat or finCnt > 0:
+        # Append all result categories and uncat if appropriate
+        if cat or teamCnt > 0 or len(self.cats) < 2:
             ret.append(sec)
             rsec = sec
             # Race metadata / UCI comments
-            sec = report.bullet_text('uci-' + cat)
+            secid = 'resultmeta'
+            if cat:
+                secid = 'resultmeta-' + cat.lower()
+            sec = report.bullet_text(secid)
             if wt is not None:
                 if distance is not None:
                     sec.lines.append([
                         None, 'Average speed of the winner: ' +
                         wt.speedstr(1000.0 * distance)
                     ])
             sec.lines.append([None, 'Number of teams: ' + str(teamCnt)])
-            #if dnfcount > 0:
-            #sec.lines.append([
-            #None,
-            #u'Teams not completing the event: ' + unicode(dnfcount)
-            #])
-            #residual = totcount - (fincount + dnfcount + dnscount + hdcount)
-            #if residual > 0:
-            #_log.info(u'%r teams unaccounted for: %r', cat, residual)
             ret.append(sec)
 
             # finish report title manipulation
             if catname:
                 cv = []
                 if rsec.heading:
                     cv.append(rsec.heading)
@@ -983,20 +964,17 @@
 
         # show all intermediates here
         for i in self.intermeds:
             im = self.intermap[i]
             if im['places'] and im['show']:
                 ret.extend(self.int_report(i))
 
-        if len(self.comment) > 0:
-            s = report.bullet_text('comms')
-            s.heading = 'Decisions of the commissaires panel'
-            for comment in self.comment:
-                s.lines.append([None, comment])
-            ret.append(s)
+        # append a decisions section
+        ret.append(self.decision_section())
+
         return ret
 
     def race_ctrl_add(self, rlist):
         """Add the supplied riders to event model with lookup"""
         rlist = strops.riderlist_split(rlist, self.meet.rdb, self.series)
         for bib in rlist:
             self.addrider(bib)
@@ -1148,37 +1126,33 @@
         """Handle a change in team data"""
         # assume the worst and recalc all riders
         self.team_start_times()
 
     def resettimer(self):
         """Reset race timer."""
         _log.info('Reset event to idle')
-        self.meet.alttimer.dearm(1)
         self.set_start()
         self.clear_results()
         self.teamtimes = {}
         self.timerstat = 'idle'
         self.meet.cmd_announce('timerstat', 'idle')
         self.meet.stat_but.update('idle', 'Idle')
         self.meet.stat_but.set_sensitive(True)
         self.elaplbl.set_text('')
         self.live_announce = True
 
     def armfinish(self):
         """Process an armfinish request."""
-        if self.timerstat in ['running', 'finished']:
+        if self.timerstat in ('running', 'finished'):
             self.armlap()
             self.timerstat = 'armfinish'
             self.meet.cmd_announce('timerstat', 'armfinish')
             self.meet.stat_but.update('error', 'Arm Finish')
             self.meet.stat_but.set_sensitive(True)
-            self.meet.alttimer.armlock(True)
-            self.meet.alttimer.arm(1)
         elif self.timerstat == 'armfinish':
-            self.meet.alttimer.dearm(1)
             self.timerstat = 'running'
             self.meet.cmd_announce('timerstat', 'running')
             self.meet.stat_but.update('ok', 'Running')
 
     def armlap(self):
         ## announce text handling...
         self.scratch_map = {}
@@ -1204,27 +1178,28 @@
     def alttimertrig(self, e):
         """Record timer message from alttimer."""
         # note: these impulses are sourced from alttimer device and keyboard
         #       transponder triggers are collected separately in timertrig()
         _log.debug('Alt timer: %s@%s/%s', e.chan, e.rawtime(), e.source)
         channo = strops.chan2id(e.chan)
         if channo == 1:
-            # this is a finish impulse, treat as an n'th wheel indicator
+            _log.info('Trigger: %s@%s/%s', e.chan, e.rawtime(), e.source)
+            # if finish armed, treat as an n'th wheel indicator
             if self.timerstat == 'armfinish':
                 _log.info('Team finish: %s', e.rawtime())
         else:
             # send through to catch-all trigger handler
             self.starttrig(e)
 
     def riderlap(self, bib, lr, rcat, e):
         """Process an accepted rider lap passing"""
         # check if lap mode is target-based
         lapfinish = False
         targetlap = None
-        if self.targetlaps:
+        if self.autofinish:
             # category laps override event laps
             if rcat in self.catlaps and self.catlaps[rcat]:
                 targetlap = self.catlaps[rcat]
             else:
                 targetlap = self.totlaps
             if targetlap and lr[COL_LAPS] >= targetlap - 1:
                 lapfinish = True  # arm just this rider
@@ -1245,32 +1220,30 @@
                                             lr[COL_CAT], e)
             else:
                 _log.info('Duplicate finish rider %s:%s@%s/%s', bib, e.chan,
                           e.rawtime(2), e.source)
         # end finishing rider path
 
         # lapping rider path
-        elif self.timerstat in ['running']:  # not finished, not armed
+        elif self.timerstat == 'running':
             self._dorecalc = True
             if lr[COL_INRACE] and (lr[COL_PLACE] or lr[COL_CBUNCH] is None):
                 # rider in the race, not yet finished: increment own lap count
                 lr[COL_LAPS] += 1
 
                 # announce all rider passings
                 self.announce_rider('', bib, lr[COL_NAMESTR], lr[COL_CAT], e)
         return False
 
     def finsprint(self, places):
         """Display a final sprint 'provisional' result."""
-        # TODO: output team result from here
         pass
 
     def reannounce_times(self):
         """Re-send the current timing values."""
-        # TODO
         self.meet.cmd_announce('timerstat', self.timerstat)
         return False
 
     def timeout(self):
         """Update elapsed time and recalculate if required."""
         if not self.winopen:
             return False
@@ -1298,25 +1271,41 @@
         self.meet.cmd_announce('timerstat', 'finished')
         self.meet.cmd_announce('laplbl', None)
         self.meet.stat_but.update('idle', 'Finished')
         self.meet.stat_but.set_sensitive(False)
 
     def info_time_edit_clicked_cb(self, button, data=None):
         """Run an edit times dialog to update event time."""
-        st = ''
-        if self.start is not None:
-            st = self.start.rawtime(2)
-        ft = '[n/a]'
-        ret = uiutil.edit_times_dlg(self.meet.window,
-                                    stxt=st,
-                                    ftxt=ft,
-                                    finish=False)
-        if ret[0] == 1:
-            wasrunning = self.timerstat in ['running', 'armfinish']
-            self.set_start(ret[1])
+        sections = {
+            'times': {
+                'object': None,
+                'title': 'times',
+                'schema': {
+                    'title': {
+                        'prompt': 'Manually adjust event time',
+                        'control': 'section',
+                    },
+                    'start': {
+                        'prompt': 'Start:',
+                        'hint': 'Event start time',
+                        'type': 'tod',
+                        'places': 4,
+                        'control': 'short',
+                        'nowbut': True,
+                        'value': self.start,
+                    },
+                },
+            },
+        }
+        res = uiutil.options_dlg(window=self.meet.window,
+                                 title='Edit times',
+                                 sections=sections)
+        if res['times']['start'][0]:
+            wasrunning = self.timerstat in ('running', 'armfinish')
+            self.set_start(res['times']['start'][2])
             if wasrunning:
                 # flag a recalculate
                 self._dorecalc = True
             _log.info('Adjusted event times')
 
     def editcat_cb(self, cell, path, new_text, col):
         """Edit the cat field if valid."""
@@ -1331,37 +1320,14 @@
         """Draw start time offset in rider view."""
         st = model.get_value(iter, COL_STOFT)
         otxt = ''
         if st is not None:
             otxt = st.rawtime(0)
         cr.set_property('text', otxt)
 
-    def editbunch_cb(self, cell, path, new_text, col=None):
-        """Edit bunch time on rider view."""
-        new_text = new_text.strip()
-        dorecalc = False
-        if new_text == '':  # user request to clear RFTIME?
-            self.riders[path][COL_RFTIME] = None
-            self.riders[path][COL_MBUNCH] = None
-            self.riders[path][COL_CBUNCH] = None
-            dorecalc = True
-        else:
-            # get 'current bunch time'
-            omb = self.vbunch(self.riders[path][COL_CBUNCH],
-                              self.riders[path][COL_MBUNCH])
-
-            # assign new bunch time
-            # note: ttt does not use + times or cascade
-            nmb = tod.mktod(new_text)
-            if self.riders[path][COL_MBUNCH] != nmb:
-                self.riders[path][COL_MBUNCH] = nmb
-                dorecalc = True
-        if dorecalc:
-            self.recalculate()
-
     def bounceteam(self, team, cat, time):
         """Bounce a teamname and time onto the panel"""
         team = team.upper()
         tname = ''
         tcat = self.ridercat(cat)
         # lookup team name in rdb
         dbr = self.meet.rdb.get_rider(team, 'team')
@@ -1472,15 +1438,15 @@
         for t in self.teammap:
             # unless team has n finishers, there is no time
             tlist = self.teammap[t]
             nth_wheel = self.teamnth[t]
             if len(tlist) >= nth_wheel:
                 ct = (tlist[nth_wheel - 1][COL_RFTIME] - self.start -
                       tlist[nth_wheel - 1][COL_STOFT])
-                thetime = ct.truncate(1)
+                thetime = ct.round(1)
                 self.teamtimes[t] = thetime  # save to times map
                 if (t not in self.announced_teams and
                     (self.announce_team is None or self.announce_team == t)):
                     # bounce this time onto the panel? HACK
                     self.announced_teams.add(t)
                     self.running_team = None  # cancel a running time
                     self.bounceteam(t, self.teamcats[t], thetime)
@@ -1488,15 +1454,15 @@
                 for r in tlist[0:nth_wheel]:
                     r[COL_CBUNCH] = thetime
                 for r in tlist[nth_wheel:]:
                     et = r[COL_RFTIME] - self.start - r[COL_STOFT]
                     if self.owntime and (et > ct and
                                          (et - ct) > self.gapthresh):
                         # TIME GAP!
-                        thetime = et.truncate(1)
+                        thetime = et.round(1)
                     r[COL_CBUNCH] = thetime
                     ct = et
 
         # leave mode sorted by arrival order
         self.reorder_arrivals()  # re-order view by arrivals at finish
 
         # if final places in view, update text entry
@@ -1504,25 +1470,24 @@
             self.meet.action_combo.get_active_iter(), 0)
         if curact == 'fin':
             self.meet.action_entry.set_text(self.places)
         #_log.debug(u'Event status: %r', self.racestat)
         self.calcset = True
         return False  # allow idle add
 
-    def __init__(self, meet, event, ui=True):
+    def __init__(self, meet, etype, ui=True):
         self.meet = meet
-        self.event = event
-        self.evno = event['evid']
-        self.series = event['seri']
-        self.configfile = meet.event_configfile(self.evno)
+        self.etype = etype
+        self.series = ''
+        self.configfile = 'event.json'
         self.readonly = not ui
         rstr = ''
         if self.readonly:
             rstr = 'readonly '
-        _log.debug('Init %r event %r', rstr, self.evno)
+        _log.debug('Init %r event', rstr)
 
         self.recalclock = threading.Lock()
         self._dorecalc = False
 
         self.teamnames = {}
         self.teamtimes = {}
         self.teamnth = {}
@@ -1539,22 +1504,23 @@
         self.relativestart = False
         self.showriders = True
         self.owntime = True  # dropped riders get own time
         self.start = None
         self.calcset = False
         self.maxfinish = tod.ZERO
         self.minlap = None
+        self.startgap = None
         self.winopen = True
         self.timerstat = 'idle'
         self.places = ''
-        self.comment = []
+        self.decisions = []
         self.ridermark = None
         self.cats = []
         self.passingsource = []  # list of decoders we accept passings from
-        self.targetlaps = False  # true if finish is det by target
+        self.autofinish = False  # true if finish is det by target
         self.catplaces = {}
         self.catlaps = {}  # cache of cat lap counts
         self.defaultnth = NTH_WHEEL
         self.nthwheel = {}
         self.autocats = False
         self.autostartlist = None
         self.bonuses = {}
```

### Comparing `metarace-roadmeet-1.13.1/src/roadmeet/ui/irtt.ui` & `metarace-roadmeet-1.13.2/src/roadmeet/ui/irtt.ui`

 * *Files identical despite different names*

### Comparing `metarace-roadmeet-1.13.1/src/roadmeet/ui/new_start.ui` & `metarace-roadmeet-1.13.2/src/roadmeet/ui/new_start.ui`

 * *Files identical despite different names*

### Comparing `metarace-roadmeet-1.13.1/src/roadmeet/ui/rider_context.ui` & `metarace-roadmeet-1.13.2/src/roadmeet/ui/rider_context.ui`

 * *Files identical despite different names*

### Comparing `metarace-roadmeet-1.13.1/src/roadmeet/ui/rms.ui` & `metarace-roadmeet-1.13.2/src/roadmeet/ui/rms.ui`

 * *Files identical despite different names*

### Comparing `metarace-roadmeet-1.13.1/src/roadmeet/ui/rms_context.ui` & `metarace-roadmeet-1.13.2/src/roadmeet/ui/rms_context.ui`

 * *Files identical despite different names*

### Comparing `metarace-roadmeet-1.13.1/src/roadmeet/ui/roadmeet.ui` & `metarace-roadmeet-1.13.2/src/roadmeet/ui/roadmeet.ui`

 * *Files 1% similar despite different names*

#### Comparing `metarace-roadmeet-1.13.1/src/roadmeet/ui/roadmeet.ui` & `metarace-roadmeet-1.13.2/src/roadmeet/ui/roadmeet.ui`

```diff
@@ -78,38 +78,14 @@
                     <property name="visible">True</property>
                     <property name="label" translatable="yes">_Event</property>
                     <property name="use_underline">True</property>
                     <child type="submenu">
                       <object class="GtkMenu" id="menu6">
                         <property name="visible">True</property>
                         <child>
-                          <object class="GtkImageMenuItem" id="menu_race_run">
-                            <property name="label" translatable="yes">_Run</property>
-                            <property name="visible">True</property>
-                            <property name="tooltip_text" translatable="yes">Run the selected event</property>
-                            <property name="use_underline">True</property>
-                            <property name="image">image5</property>
-                            <property name="use_stock">False</property>
-                            <accelerator key="Return" signal="activate" modifiers="GDK_CONTROL_MASK"/>
-                            <signal name="activate" handler="menu_race_run_activate_cb"/>
-                          </object>
-                        </child>
-                        <child>
-                          <object class="GtkImageMenuItem" id="menu_race_close">
-                            <property name="label">C_lose</property>
-                            <property name="visible">True</property>
-                            <property name="sensitive">False</property>
-                            <property name="tooltip_text" translatable="yes">Save and close the current event</property>
-                            <property name="use_underline">True</property>
-                            <property name="image">image6</property>
-                            <property name="use_stock">False</property>
-                            <signal name="activate" handler="menu_race_close_activate_cb"/>
-                          </object>
-                        </child>
-                        <child>
                           <object class="GtkImageMenuItem" id="menu_race_properties">
                             <property name="label">gtk-properties</property>
                             <property name="visible">True</property>
                             <property name="tooltip_text" translatable="yes">Edit event specific parameters</property>
                             <property name="use_underline">True</property>
                             <property name="use_stock">True</property>
                             <signal name="activate" handler="menu_race_properties_activate_cb"/>
@@ -157,27 +133,24 @@
                             <property name="tooltip_text" translatable="yes">Mark event as finished</property>
                             <property name="use_underline">True</property>
                             <accelerator key="F10" signal="activate"/>
                             <signal name="activate" handler="menu_race_finished_activate_cb"/>
                           </object>
                         </child>
                         <child>
-                          <object class="GtkSeparatorMenuItem" id="separatormenuitem1">
+                          <object class="GtkSeparatorMenuItem" id="menu_race_sep21">
                             <property name="visible">True</property>
                           </object>
                         </child>
                         <child>
-                          <object class="GtkImageMenuItem" id="menu_race_abort">
-                            <property name="label">gtk-cancel</property>
+                          <object class="GtkMenuItem" id="menu_race_decisions">
                             <property name="visible">True</property>
-                            <property name="sensitive">False</property>
-                            <property name="tooltip_text" translatable="yes">Abort the current event without saving</property>
-                            <property name="use_underline">True</property>
-                            <property name="use_stock">True</property>
-                            <signal name="activate" handler="menu_race_abort_activate_cb"/>
+                            <property name="label" translatable="yes">Decisions</property>
+                            <property name="tooltip_text" translatable="yes">Edit decisions of the commissaires panel</property>
+                            <signal name="activate" handler="menu_race_decisions_activate_cb"/>
                           </object>
                         </child>
                       </object>
                     </child>
                   </object>
                 </child>
                 <child>
```

### Comparing `metarace-roadmeet-1.13.1/src/roadmeet/ui/swap_rider.ui` & `metarace-roadmeet-1.13.2/src/roadmeet/ui/swap_rider.ui`

 * *Files identical despite different names*

### Comparing `metarace-roadmeet-1.13.1/src/roadmeet/ui/tod_context.ui` & `metarace-roadmeet-1.13.2/src/roadmeet/ui/tod_context.ui`

 * *Files identical despite different names*

### Comparing `metarace-roadmeet-1.13.1/src/roadmeet/uiutil.py` & `metarace-roadmeet-1.13.2/src/roadmeet/uiutil.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,17 +14,18 @@
 
 gi.require_version('Pango', '1.0')
 from gi.repository import Pango
 
 import metarace
 from metarace import tod
 from metarace import strops
+from metarace.jsonconfig import config
 from metarace.riderdb import rider
 
-_log = logging.getLogger('roadmeet.uiutil')
+_log = logging.getLogger('uiutil')
 _log.setLevel(logging.DEBUG)
 
 # Resources package
 RESOURCE_PKG = 'roadmeet.ui'
 
 # Font-overrides
 DIGITFONT = Pango.FontDescription('Noto Mono Medium 22')
@@ -438,15 +439,14 @@
         h.show()
 
         v.pack_start(h, False, True, 0)
 
         # Clock row 'HHhMM:SS.DCMZ'
         self.ck = Gtk.Label.new(FIELDWIDTH)
         self.ck.set_alignment(0.5, 0.5)
-        # todo: alternate text modification via css
         self.ck.modify_font(DIGITFONT)
         self.ck.show()
         v.pack_start(self.ck, True, True, 0)
 
         # Timer ctrl/status button
         #h = Gtk.HBox(False, 5)
         h = Gtk.Box.new(Gtk.Orientation.HORIZONTAL, 5)
@@ -474,58 +474,53 @@
         self.splitlbls = []  # ordered set of split ids
         self.toidle()
 
 
 def builder(resource=None):
     """Create and return a Gtk.Builder loaded from named resource"""
     ret = None
-    _log.debug('Creating Gtk Build for resource %r', resource)
+    _log.debug('Creating Gtk Builder for resource %r', resource)
     rf = files(RESOURCE_PKG).joinpath(resource)
     if rf is not None and rf.is_file():
         ret = Gtk.Builder()
         ret.add_from_string(rf.read_text(encoding='utf-8'))
     else:
         _log.error('Unable to read resource %r: %r', resource, rf)
     return ret
 
 
-def riderview(rdb):
-    """Create a rider db view"""
-    l = Gtk.Label.new('riders...')
-    l.show()
-    return l
-
-
 def about_dlg(window, version=None):
     """Display shared about dialog."""
-    dlg = Gtk.AboutDialog(modal=True, destroy_with_parent=True)
+    modal = window is not None
+    dlg = Gtk.AboutDialog(modal=modal, destroy_with_parent=True)
     dlg.set_transient_for(window)
-    dlg.set_program_name(u'roadmeet')
+    dlg.set_program_name('roadmeet')
     vtxt = 'Library: ' + metarace.VERSION
     if version:
         vtxt = 'Application: ' + version + '; ' + vtxt
     dlg.set_version(vtxt)
     dlg.set_copyright(
-        u'Copyright \u00a9 2012-2023 Nathan Fraser and contributors')
-    dlg.set_comments(u'Road cycle race result handler')
+        'Copyright \u00a9 2012-2023 Nathan Fraser and contributors')
+    dlg.set_comments('Road cycle race result handler')
     dlg.set_license_type(Gtk.License.MIT_X11)
     dlg.set_license(metarace.LICENSETEXT)
     dlg.set_wrap_license(True)
     dlg.run()
     dlg.hide()
     dlg.destroy()
 
 
 def chooseCsvFile(title='',
                   mode=Gtk.FileChooserAction.OPEN,
                   parent=None,
                   path=None,
                   hintfile=None):
     ret = None
-    dlg = Gtk.FileChooserNative(title=title, modal=True)
+    modal = parent is not None
+    dlg = Gtk.FileChooserNative(title=title, modal=modal)
     dlg.set_transient_for(parent)
     dlg.set_action(mode)
     cfilt = Gtk.FileFilter()
     cfilt.set_name('CSV Files')
     cfilt.add_mime_type('text/csv')
     cfilt.add_pattern('*.csv')
     dlg.add_filter(cfilt)
@@ -569,41 +564,58 @@
                  cb=None,
                  width=None,
                  halign=None,
                  calign=None,
                  expand=False,
                  editcb=None,
                  maxwidth=None,
+                 minwidth=None,
+                 charwidth=None,
                  bgcol=None,
                  fontdesc=None,
-                 fixed=False):
+                 wrap=None,
+                 fixed=False,
+                 valign=None):
     """Return a text view column."""
     i = Gtk.CellRendererText()
     if cb is not None:
         i.set_property('editable', True)
         i.connect('edited', cb, colno)
     if calign is not None:
         i.set_property('xalign', calign)
+    if valign is not None:
+        i.set_property('yalign', valign)
     if fontdesc is not None:
         i.set_property('font_desc', fontdesc)
+    if charwidth is not None:
+        i.set_property('width_chars', charwidth)
+    if wrap is not None:
+        if minwidth is None:
+            minwidth = 400
+        if wrap:
+            i.set_property('wrap-mode', Pango.WrapMode.WORD_CHAR)
+            i.set_property('wrap-width', minwidth)
+        else:
+            i.set_property('wrap-width', -1)
+
     j = Gtk.TreeViewColumn(header, i, text=colno)
     if bgcol is not None:
         j.add_attribute(i, 'background', bgcol)
     if halign is not None:
         j.set_alignment(halign)
     if fixed:
         j.set_sizing(Gtk.TreeViewColumnSizing.FIXED)
     if expand:
         if width is not None:
             j.set_min_width(width)
         j.set_expand(True)
     else:
         if width is not None:
             j.set_min_width(width)
-    if maxwidth is not None:
+    if maxwidth is not None and wrap is None:
         j.set_max_width(maxwidth)
     view.append_column(j)
     if editcb is not None:
         i.connect('editing-started', editcb)
     return i
 
 
@@ -690,95 +702,123 @@
     else:
         if width is not None:
             j.set_min_width(width)
     view.append_column(j)
     return i
 
 
-def questiondlg(window, question, subtext=None, title=None):
-    """Display a question dialog and return True/False."""
-    dlg = Gtk.MessageDialog(modal=True,
-                            message_type=Gtk.MessageType.QUESTION,
-                            buttons=Gtk.ButtonsType.OK_CANCEL,
-                            text=question,
+def messagedlg(window=None,
+               message='Message',
+               message_type=Gtk.MessageType.ERROR,
+               buttons=Gtk.ButtonsType.CLOSE,
+               subtext=None,
+               title=None):
+    """Display a message dialog."""
+    modal = window is not None
+    dlg = Gtk.MessageDialog(modal=modal,
+                            message_type=message_type,
+                            buttons=buttons,
+                            text=message,
                             destroy_with_parent=True)
     dlg.set_transient_for(window)
     if title:
         dlg.set_title(title)
     if subtext is not None:
         dlg.format_secondary_text(subtext)
     ret = False
     response = dlg.run()
+    _log.debug('Message dialog %r returned: %r', title, response)
     dlg.hide()
     if response == Gtk.ResponseType.OK:
         ret = True
     dlg.destroy()
     return ret
 
 
-def now_button_clicked_cb(button, entry=None):
-    """Copy the current time of day into the supplied entry."""
-    if entry is not None:
-        entry.set_text(tod.now().timestr())
+def questiondlg(window=None, question='Question?', subtext=None, title=None):
+    """Display a question dialog and return True/False."""
+    return messagedlg(window=window,
+                      message=question,
+                      message_type=Gtk.MessageType.QUESTION,
+                      buttons=Gtk.ButtonsType.OK_CANCEL,
+                      subtext=subtext,
+                      title=title)
 
 
 class option:
     """Base class for configuration option"""
 
-    def __init__(self, key, schema, obj=None):
+    def __init__(self, key, schema, obj=None, section=None):
         self.key = key
-        self._obj = None
+        self._obj = obj
+        self._section = section
         self._attr = None
         self._value = None
         self._oldvalue = None
+        self._default = None
         self._type = 'str'
         self._prompt = None
         self._hint = None
         self._subtext = None
         self._control = None
         self._options = {}
         self._places = 0
+        self._nowbut = False
         self._readonly = False
         self._defer = False
 
         # import schema
-        if obj is not None and 'attr' in schema:
-            self._obj = obj
-            if isinstance(self._obj, rider):
-                self._attr = schema['attr']
-            else:
-                if schema['attr'] is not None and hasattr(
-                        self._obj, schema['attr']):
+        if 'type' in schema:
+            self._type = schema['type']
+        if obj is not None:
+            if isinstance(self._obj, config):
+                self._attr = key
+            elif 'attr' in schema:
+                if isinstance(self._obj, (rider, dict)):
                     self._attr = schema['attr']
+                else:
+                    if schema['attr'] is not None and hasattr(
+                            self._obj, schema['attr']):
+                        self._attr = schema['attr']
+        if 'default' in schema:
+            self._default = schema['default']
         if 'value' in schema:
             self._value = schema['value']
         if self._attr is not None and self._value is None:
             if isinstance(self._obj, rider):
                 self._value = self._obj[self._attr]
+            elif isinstance(self._obj, config):
+                self._value = self._obj.get_value(self._section, self._attr)
+            elif isinstance(self._obj, dict):
+                if self._attr in self._obj:
+                    valid, value = self.parse_value(self._obj[self._attr])
+                    if valid:
+                        self._value = value
             else:
                 self._value = getattr(self._obj, self._attr)
         self._oldvalue = self._value
-        if 'type' in schema:
-            self._type = schema['type']
         if 'prompt' in schema:
             self._prompt = schema['prompt']
         else:
             self._prompt = key
         if 'hint' in schema:
             self._hint = schema['hint']
         if 'subtext' in schema:
             self._subtext = schema['subtext']
         if 'places' in schema:
             self._places = strops.confopt_posint(schema['places'], 0)
         if 'readonly' in schema:
             self._readonly = bool(schema['readonly'])
+        if 'nowbut' in schema:
+            self._nowbut = bool(schema['nowbut'])
         if 'defer' in schema:
             self._defer = bool(schema['defer'])
         if 'options' in schema:
             if isinstance(schema['options'], dict):
+                self._options[''] = '[Not set]'
                 for kv in schema['options']:
                     k = str(kv)
                     v = schema['options'][kv]
                     self._options[k] = v
 
     def changed(self):
         """Return true if current value differ from original"""
@@ -795,27 +835,27 @@
     def reset(self):
         self.set_value(self._oldvalue)
 
     def validate(self):
         """Check proposed value in control"""
         return self.read_value(self._control.get_text())
 
-    def read_value(self, newtext):
-        """Try to read and update value from newtext"""
+    def parse_value(self, newtext):
+        """Return a value of the correct type for this option"""
         ret = False
         newval = None
         if self._type == 'tod':
             if newtext:
                 newval = tod.mktod(newtext)
                 if newval is not None:
                     ret = True
             else:
                 ret = True
         elif self._type == 'int':
-            if newtext:
+            if newtext is not None and newtext != '':
                 newval = strops.confopt_int(newtext)
                 if newval is not None:
                     ret = True
             else:
                 ret = True
         elif self._type == 'bool':
             newval = strops.confopt_bool(newtext)
@@ -831,22 +871,31 @@
             if newtext:
                 newval = strops.confopt_float(newtext)
                 if newval is not None:
                     ret = True
             else:
                 ret = True
         elif self._type == 'str':
-            newval = str(newtext)
+            if newtext is not None:
+                newval = str(newtext)
+                if not newval:
+                    # Allow unset of values without default
+                    if self._default is None:
+                        newval = None
             ret = True
         else:
             _log.warning('Unknown option value type %r=%r', self._type,
                          newtext)
             newval = newtext
             ret = True
+        return ret, newval
 
+    def read_value(self, newtext):
+        """Try to read and update value from newtext"""
+        ret, newval = self.parse_value(newtext)
         if ret:
             self.set_value(newval)
         return ret
 
     def format_value(self):
         """Return a string for use in a text entry"""
         ret = ''
@@ -861,14 +910,18 @@
     def set_value(self, newval):
         """Store new value in object and update obj if provided"""
         self._value = newval
         if self._obj is not None and self._attr is not None:
             if isinstance(self._obj, rider):
                 # Don't trigger notify in this path - leave that to the caller
                 self._obj.set_value(self._attr, self._value)
+            elif isinstance(self._obj, config):
+                self._obj.set(self._section, self._attr, self._value)
+            elif isinstance(self._obj, dict):
+                self._obj[self._attr] = self._value
             else:
                 # assume object.attribute
                 setattr(self._obj, self._attr, self._value)
         if self.changed():
             _log.debug('Option %r update value: %r=>%r (%s)', self.key,
                        self._oldvalue, self._value,
                        self._value.__class__.__name__)
@@ -878,165 +931,225 @@
         """Handle update event on control"""
         if self.read_value(control.get_text()):
             control.set_text(self.format_value())
             return True
         else:
             return False
 
-    def add_control(self, grid, row):
-        """Create a new control and add it to the provided grid"""
+    def _prompt_label(self):
+        """Return a prompt label"""
         lbl = Gtk.Label(label=self._prompt)
         lbl.set_single_line_mode(True)
-        lbl.set_halign(Gtk.Align.FILL)
-        lbl.set_xalign(0.0)
-        lbl.set_hexpand(True)
+        lbl.set_halign(Gtk.Align.START)
         lbl.show()
-        grid.attach(lbl, 0, row, 1, 1)
+        return lbl
+
+    def add_control(self, grid, row):
+        """Create a new control and add it to the provided grid"""
+        grid.attach(self._prompt_label(), 0, row, 1, 1)
 
         self._control = Gtk.Entry()
         self._control.set_width_chars(32)
         self._control.set_activates_default(True)
         if self._value is not None:
             self._control.set_text(self.format_value())
         if self._hint is not None:
             self._control.set_tooltip_text(self._hint)
         self._control.show()
         if not self._defer:
             self._control.connect('activate', self._updated)
         if self._readonly:
-            self._control.set_sensitive(False)
-        grid.attach(self._control, 1, row, 2, 1)
+            self._control.set_editable(False)
+        grid.attach(self._control, 1, row, 4, 1)
+        return 1
 
 
 class optionShort(option):
 
+    def _now_press(self, widget, event):
+        """Transfer now into value and re-validate"""
+        self._value = tod.now().truncate(self._places)
+        self._control.set_text(self.format_value())
+
     def add_control(self, grid, row):
         """Create a new control and add it to the provided grid"""
-        lbl = Gtk.Label(label=self._prompt)
-        lbl.set_single_line_mode(True)
-        lbl.set_halign(Gtk.Align.FILL)
-        lbl.set_xalign(0.0)
-        lbl.set_hexpand(True)
-        lbl.show()
-        grid.attach(lbl, 0, row, 1, 1)
+        grid.attach(self._prompt_label(), 0, row, 1, 1)
 
         self._control = Gtk.Entry()
-        self._control.set_width_chars(11)
+        self._control.set_width_chars(12)
         self._control.set_activates_default(True)
         if self._value is not None:
             self._control.set_text(self.format_value())
         if self._hint is not None:
             self._control.set_tooltip_text(self._hint)
         self._control.show()
         if not self._defer:
             self._control.connect('activate', self._updated)
         if self._readonly:
-            self._control.set_sensitive(False)
+            self._control.set_editable(False)
         grid.attach(self._control, 1, row, 1, 1)
 
-        if self._subtext:
-            lbl = Gtk.Label(label=self._subtext)
+        if self._nowbut:
+            but = Gtk.Button()
+            but.set_label('Now')
+            but.set_halign(Gtk.Align.START)
+            but.set_can_focus(False)
+            but.show()
+            if self._subtext:
+                but.set_tooltip_text(self._subtext)
+            else:
+                but.set_tooltip_text('Set the tod entry to now')
+            but.connect('button-press-event', self._now_press)
+            grid.attach(but, 2, row, 1, 1)
+        else:
+            subtext = ''
+            if self._subtext:
+                subtext = self._subtext
+            lbl = Gtk.Label(label=subtext)
             lbl.set_single_line_mode(True)
-            lbl.set_halign(Gtk.Align.FILL)
-            lbl.set_xalign(0.0)
-            lbl.set_hexpand(True)
+            lbl.set_halign(Gtk.Align.START)
             lbl.show()
-            grid.attach(lbl, 2, row, 1, 1)
+            grid.attach(lbl, 2, row, 3, 1)
+        return 1
 
 
 class optionCheck(option):
 
     def validate(self):
         """Check proposed value in control"""
         return self.read_value(self._control.get_active())
 
     def _updated(self, control):
         """Handle update event on control"""
         return self.read_value(self._control.get_active())
 
     def add_control(self, grid, row):
         """Create a new control and add it to the provided grid"""
-        lbl = Gtk.Label(label=self._prompt)
-        lbl.set_single_line_mode(True)
-        lbl.set_halign(Gtk.Align.FILL)
-        lbl.set_xalign(0.0)
-        lbl.set_hexpand(True)
-        lbl.show()
-        grid.attach(lbl, 0, row, 1, 1)
+        grid.attach(self._prompt_label(), 0, row, 1, 1)
 
         st = ''
         if self._subtext:
             st = self._subtext
         self._control = Gtk.CheckButton.new_with_label(st)
         if self._value:
             self._control.set_active(True)
         if self._hint is not None:
             self._control.set_tooltip_text(self._hint)
         self._control.show()
         if not self._defer:
             self._control.connect('toggled', self._updated)
         if self._readonly:
             self._control.set_sensitive(False)
-        grid.attach(self._control, 1, row, 2, 1)
+        grid.attach(self._control, 1, row, 3, 1)
+        return 1
+
+
+class optionHidden(option):
+    """Hidden option with value and type"""
+
+    def add_control(self, grid, row):
+        return 0
+
+    def validate(self):
+        return True
+
+
+class optionLabel(option):
+
+    def add_control(self, grid, row):
+        grid.attach(self._prompt_label(), 0, row, 1, 1)
+
+        self._control = Gtk.Label()
+        self._control.set_halign(Gtk.Align.START)
+        self._control.set_selectable(True)
+        self._control.set_margin_top(4)
+        self._control.set_margin_bottom(4)
+        if self._value is not None:
+            self._control.set_text(self.format_value())
+        if self._hint is not None:
+            self._control.set_tooltip_text(self._hint)
+        self._control.show()
+        grid.attach(self._control, 1, row, 4, 1)
+        return 1
+
+    def validate(self):
+        return True
 
 
 class optionChoice(option):
 
     def validate(self):
         """Check proposed value in control"""
-        return self.read_value(self._control.get_active_id())
+        newval = self._control.get_active_id()
+        if newval == '':
+            # Allow un-set of option value
+            newval = None
+        return self.read_value(newval)
 
     def _updated(self, control):
         """Handle update event on control"""
-        return self.read_value(self._control.get_active_id())
+        return self.validate()
 
     def add_control(self, grid, row):
         """Create a new control and add it to the provided grid"""
-        lbl = Gtk.Label(label=self._prompt)
-        lbl.set_single_line_mode(True)
-        lbl.set_halign(Gtk.Align.FILL)
-        lbl.set_xalign(0.0)
-        lbl.set_hexpand(True)
-        lbl.show()
-        grid.attach(lbl, 0, row, 1, 1)
+        grid.attach(self._prompt_label(), 0, row, 1, 1)
 
         self._control = Gtk.ComboBoxText.new()
         for k in self._options:
             self._control.append(k, self._options[k])
         if self._value is not None:
             self._control.set_active_id(self.format_value())
+        else:
+            self._control.set_active_id('')
         self._control.show()
         if not self._defer:
             self._control.connect('changed', self._updated)
         if self._readonly:
             self._control.set_sensitive(False)
-        grid.attach(self._control, 1, row, 2, 1)
+        if self._hint is not None:
+            self._control.set_tooltip_text(self._hint)
+        grid.attach(self._control, 1, row, 3, 1)
+
+        subtext = ''
+        if self._subtext:
+            subtext = self._subtext
+        lbl = Gtk.Label(label=subtext)
+        lbl.set_single_line_mode(True)
+        lbl.show()
+        grid.attach(lbl, 4, row, 1, 1)
+
+        return 1
 
 
 class optionSection(option):
 
     def validate(self):
         return True
 
     def add_control(self, grid, row):
         """Create a new control and add it to the provided grid"""
         lbl = Gtk.Label(label=self._prompt)
         lbl.set_single_line_mode(True)
-        lbl.set_width_chars(42)
-        lbl.set_halign(Gtk.Align.FILL)
-        lbl.set_xalign(0.0)
-        lbl.set_hexpand(True)
+        lbl.set_halign(Gtk.Align.START)
+        lbl.set_attributes(Pango.AttrList.from_string('0 -1 style oblique'))
+        if row != 0:
+            lbl.set_margin_top(15)
         lbl.show()
-        grid.attach(lbl, 0, row, 3, 1)
+        grid.attach(lbl, 0, row, 5, 1)
+        return 1
 
 
-def options_dlg(window=None, title='Options', schema={}, obj=None):
-    """Build and display an option editor for the provided schema
+def options_dlg(window=None, title='Options', sections={}):
+    """Build and display an option editor for the provided sections
 
-          schema = {
+      sections={
+        "section": {
+          "object": OBJECT, rider or section
+          "title": section label
+          "schema": {
             "key": {
               "value": [Original value],
               "control": [Control type],
               "type" : [Value type],
               "prompt": [Prompt text],
               "subtext": [Extra info],
               "hint": [Tooltip],
@@ -1054,134 +1167,248 @@
          float: floating point number
          chan: timing channel
          bool: True/False
          tod: Time of day object with number of places in schema
 
        Control types:
 
+         none: nothing displayed for the config option
+         label: prompt and value as readonly text
          section: section delimiter
          text: standard text input
          short: short text input, extra info displayed right of input
          check: on/off selection, extra info displayed right of input
          choice: select box, choice of options provided in schema
 
-    Return value is a dict with one tuple per key:
+    Return value is a dict of dicts with one tuple per key:
 
-        "key": (changed, oldval, newval)
+        "section": {"key": (changed, oldval, newval), ...}, ...
 
     Note: section controls return (False, None, None)
     """
     omap = {}
     # read schema into options map
-    for key in schema:
-        oschema = schema[key]
-        otype = 'text'
-        if 'control' in oschema:
-            otype = oschema['control']
-        if otype == 'section':
-            omap[key] = optionSection(key, oschema, obj)
-        elif otype == 'short':
-            omap[key] = optionShort(key, oschema, obj)
-        elif otype == 'check':
-            omap[key] = optionCheck(key, oschema, obj)
-        elif otype == 'choice':
-            omap[key] = optionChoice(key, oschema, obj)
-        else:
-            omap[key] = option(key, oschema, obj)
+    for sec in sections:
+        omap[sec] = {'title': sections[sec]['title'], 'options': {}}
+        for key in sections[sec]['schema']:
+            oschema = sections[sec]['schema'][key]
+            obj = sections[sec]['object']
+            otype = 'text'
+            if 'control' in oschema:
+                otype = oschema['control']
+            if otype == 'section':
+                omap[sec]['options'][key] = optionSection(
+                    key, oschema, obj, sec)
+            elif otype == 'short':
+                omap[sec]['options'][key] = optionShort(key, oschema, obj, sec)
+            elif otype == 'check':
+                omap[sec]['options'][key] = optionCheck(key, oschema, obj, sec)
+            elif otype == 'label':
+                omap[sec]['options'][key] = optionLabel(key, oschema, obj, sec)
+            elif otype == 'choice':
+                omap[sec]['options'][key] = optionChoice(
+                    key, oschema, obj, sec)
+            elif otype == 'none':
+                omap[sec]['options'][key] = optionHidden(
+                    key, oschema, obj, sec)
+            else:
+                omap[sec]['options'][key] = option(key, oschema, obj, sec)
 
     # build dialog
-    dlg = Gtk.Dialog(title=title, modal=True, destroy_with_parent=True)
+    modal = window is not None
+    dlg = Gtk.Dialog(title=title, modal=modal, destroy_with_parent=True)
     dlg.set_transient_for(window)
     dlg.add_buttons("Cancel", 2, "OK", 0)
     dlg.set_default_response(0)
-    scr = Gtk.ScrolledWindow()
-    scr.set_policy(Gtk.PolicyType.NEVER, Gtk.PolicyType.AUTOMATIC)
-    scr.set_propagate_natural_height(True)
-    scr.show()
-    grid = Gtk.Grid()
-    grid.props.margin = 8
-    grid.set_row_spacing(4)
-    grid.set_column_spacing(8)
-    grid.set_row_homogeneous(True)
-    row = 0
-    for key in omap:
-        omap[key].add_control(grid, row)
-        row += 1
-    grid.show()
-    scr.add(grid)
-    dlg.get_content_area().pack_start(scr, True, True, 0)
+
+    # container type depends on number of config sections
+    ctr = None
+    onePage = False
+    if len(omap) == 1:
+        ctr = Gtk.ScrolledWindow()
+        ctr.set_policy(Gtk.PolicyType.NEVER, Gtk.PolicyType.AUTOMATIC)
+        ctr.set_propagate_natural_height(True)
+        onePage = True
+    else:
+        ctr = Gtk.Notebook()
+        ctr.set_tab_pos(Gtk.PositionType.LEFT)
+    ctr.show()
+    dlg.get_content_area().pack_start(ctr, True, True, 0)
+
+    for section in omap:
+        grid = Gtk.Grid()
+        grid.props.margin = 8
+        grid.set_row_spacing(4)
+        grid.set_column_spacing(8)
+        grid.set_column_homogeneous(False)
+        grid.set_row_homogeneous(False)
+        row = 0
+        for key in omap[section]['options']:
+            rows = omap[section]['options'][key].add_control(grid, row)
+            row += rows
+        grid.show()
+        if onePage:
+            ctr.add(grid)
+        else:
+            scr = Gtk.ScrolledWindow()
+            scr.set_policy(Gtk.PolicyType.NEVER, Gtk.PolicyType.AUTOMATIC)
+            scr.set_propagate_natural_height(True)
+            scr.add(grid)
+            scr.show()
+            l = Gtk.Label()
+            l.set_text(omap[section]['title'])
+            l.set_width_chars(12)
+            l.show()
+            ctr.append_page(scr, l)
+
     retval = dlg.run()
     dlg.hide()
 
     # change report
     res = {}
     if retval == 2:
         # on cancel, reset all values and report no changes
-        for key in omap:
-            o = omap[key]
-            o.reset()
-            res[key] = (False, o.get_prev(), o.get_prev())
+        for section in omap:
+            res[section] = {}
+            sec = omap[section]['options']
+            for key in sec:
+                o = sec[key]
+                o.reset()
+                res[section][key] = (False, o.get_prev(), o.get_prev())
     else:
         # re-validate all entries and report changes
-        for key in omap:
-            o = omap[key]
-            if not o.validate():
-                _log.warning('Invalid value for option %r ignored', key)
-            res[key] = (o.changed(), o.get_prev(), o.get_value())
+        for section in omap:
+            res[section] = {}
+            sec = omap[section]['options']
+            for key in sec:
+                o = sec[key]
+                if not o.validate():
+                    _log.warning('Invalid value for option %r ignored', key)
+                res[section][key] = (o.changed(), o.get_prev(), o.get_value())
 
     dlg.destroy()
     return res
 
 
-def edit_times_dlg(window,
-                   stxt=None,
-                   ftxt=None,
-                   btxt=None,
-                   ptxt=None,
-                   bonus=False,
-                   penalty=False,
-                   finish=True):
-    """Display times edit dialog and return updated time strings."""
-    b = builder('edit_times.ui')
-    dlg = b.get_object('timing')
-    dlg.set_transient_for(window)
-
-    se = b.get_object('timing_start_entry')
-    se.modify_font(MONOFONT)
-    if stxt is not None:
-        se.set_text(stxt)
-    b.get_object('timing_start_now').connect('clicked', now_button_clicked_cb,
-                                             se)
-
-    fe = b.get_object('timing_finish_entry')
-    fe.modify_font(MONOFONT)
-    if ftxt is not None:
-        fe.set_text(ftxt)
-    if finish:
-        b.get_object('timing_finish_now').connect('clicked',
-                                                  now_button_clicked_cb, fe)
-    else:
-        b.get_object('timing_finish_now').set_sensitive(False)
+class decisionEditor:
 
-    be = b.get_object('timing_bonus_entry')
-    be.modify_font(MONOFONT)
-    if btxt is not None:
-        be.set_text(btxt)
-    if bonus:
-        be.show()
-        b.get_object('timing_bonus_label').show()
-
-    pe = b.get_object('timing_penalty_entry')
-    pe.modify_font(MONOFONT)
-    if ptxt is not None:
-        pe.set_text(ptxt)
-    if penalty:
-        pe.show()
-        b.get_object('timing_penalty_label').show()
-
-    ret = dlg.run()
-    stxt = se.get_text().strip()
-    ftxt = fe.get_text().strip()
-    btxt = be.get_text().strip()
-    ptxt = pe.get_text().strip()
-    dlg.destroy()
-    return (ret, stxt, ftxt, btxt, ptxt)
+    def __init__(self, window=None, decisions=[]):
+        modal = window is not None
+        self._dlg = Gtk.Dialog(
+            title="Edit Decisions of the Commissaires Panel",
+            modal=modal,
+            destroy_with_parent=True)
+        self._dlg.set_transient_for(window)
+        self._dlg.add_buttons("Done", 0)
+
+        self._model = Gtk.ListStore(str, str)
+        for d in decisions:
+            self._model.append((
+                '\u2023',
+                d.strip(),
+            ))
+        self._view = Gtk.TreeView(self._model)
+        self._view.set_reorderable(True)
+        self._view.set_rules_hint(False)
+        self._view.set_headers_visible(False)
+        self._view.set_property('height-request', 200)
+        mkviewcoltxt(self._view, 'Bullet', 0, charwidth=2, valign=0.0)
+        mkviewcoltxt(self._view,
+                     'Decision',
+                     1,
+                     expand=True,
+                     width=400,
+                     charwidth=66,
+                     cb=self.edit_decision,
+                     wrap=True,
+                     valign=0.0)
+        self._view.show()
+        ctr = Gtk.ScrolledWindow()
+        ctr.set_policy(Gtk.PolicyType.NEVER, Gtk.PolicyType.AUTOMATIC)
+        ctr.set_propagate_natural_height(True)
+        ctr.add(self._view)
+        ctr.show()
+        self._dlg.get_content_area().pack_start(ctr, True, True, 4)
+        bb = Gtk.ButtonBox()
+        bb.set_layout(Gtk.ButtonBoxStyle.START)
+        bb.show()
+
+        but = Gtk.Button.new_from_icon_name('list-add',
+                                            Gtk.IconSize.LARGE_TOOLBAR)
+        but.set_always_show_image(True)
+        but.show()
+        but.connect('clicked', self.add_empty)
+        bb.pack_start(but, False, False, 0)
+        bb.set_child_non_homogeneous(but, True)
+
+        but = Gtk.Button.new_from_icon_name('list-remove',
+                                            Gtk.IconSize.LARGE_TOOLBAR)
+        but.set_always_show_image(True)
+        but.show()
+        but.connect('clicked', self.del_selected)
+        bb.pack_start(but, False, False, 0)
+        bb.set_child_non_homogeneous(but, True)
+
+        but = Gtk.Button.new_from_icon_name('pan-up-symbolic',
+                                            Gtk.IconSize.LARGE_TOOLBAR)
+        but.set_always_show_image(True)
+        but.show()
+        but.connect('clicked', self.move_up)
+        bb.pack_start(but, False, False, 0)
+        bb.set_child_non_homogeneous(but, True)
+
+        but = Gtk.Button.new_from_icon_name('pan-down-symbolic',
+                                            Gtk.IconSize.LARGE_TOOLBAR)
+        but.set_always_show_image(True)
+        but.show()
+        but.connect('clicked', self.move_down)
+        bb.pack_start(but, False, False, 0)
+        bb.set_child_non_homogeneous(but, True)
+
+        self._dlg.get_content_area().pack_start(bb, False, False, 4)
+
+    def del_selected(self, button):
+        """Delete the selected row."""
+        model, i = self._view.get_selection().get_selected()
+        if i is not None:
+            self._model.remove(i)
+
+    def move_up(self, button):
+        """Move selected row up one slot"""
+        model, i = self._view.get_selection().get_selected()
+        if i is not None:
+            j = self._model.iter_previous(i)
+            if j is not None:
+                self._model.swap(i, j)
+
+    def move_down(self, button):
+        """Move selected row down one slot"""
+        model, i = self._view.get_selection().get_selected()
+        if i is not None:
+            j = self._model.iter_next(i)
+            if j is not None:
+                self._model.swap(i, j)
+
+    def add_empty(self, button):
+        """Add an empty row and trigger editing the content"""
+        i = self._model.append(('\u2023', ''))
+        path = Gtk.TreeModelRow(self._model, i).path
+        self._view.set_cursor(path, self._view.get_column(1), True)
+
+    def edit_decision(self, cell, path, new_text, col):
+        """Edit column callback."""
+        new_text = new_text.strip()
+        self._model[path][col] = new_text
+
+    def run(self):
+        # for now, ignore dialog return value
+        self._dlg.run()
+        self._dlg.hide()
+        res = [d[1] for d in self._model]
+        self._dlg.destroy()
+        return res
+
+
+def decisions_dlg(window=None, decisions=[]):
+    """Edit decisions of the commissaires panel and return an updated list"""
+    dlg = decisionEditor(window=window, decisions=decisions)
+    return dlg.run()
```

