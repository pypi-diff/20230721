# Comparing `tmp/moku-3.0.0.tar.gz` & `tmp/moku-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moku-3.0.0.tar", last modified: Fri May 12 04:51:08 2023, max compression
+gzip compressed data, was "moku-3.1.0.tar", last modified: Fri Jul 21 01:14:15 2023, max compression
```

## Comparing `moku-3.0.0.tar` & `moku-3.1.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxr-x   0 sashi     (1001) sashi     (1001)        0 2023-05-12 04:51:08.925612 moku-3.0.0/
--rw-rw-r--   0 sashi     (1001) sashi     (1001)     1146 2023-05-12 04:51:08.929612 moku-3.0.0/PKG-INFO
--rw-rw-r--   0 sashi     (1001) sashi     (1001)     2674 2022-12-12 03:43:28.000000 moku-3.0.0/README.md
-drwxrwxr-x   0 sashi     (1001) sashi     (1001)        0 2023-05-12 04:51:08.925612 moku-3.0.0/moku/
--rw-rw-r--   0 sashi     (1001) sashi     (1001)    11336 2023-05-05 05:13:11.000000 moku-3.0.0/moku/__init__.py
--rw-rw-r--   0 sashi     (1001) sashi     (1001)     3758 2023-02-20 03:40:59.000000 moku-3.0.0/moku/cli.py
--rw-rw-r--   0 sashi     (1001) sashi     (1001)     1672 2023-01-27 07:08:13.000000 moku-3.0.0/moku/exceptions.py
--rw-rw-r--   0 sashi     (1001) sashi     (1001)     4353 2022-12-12 03:43:28.000000 moku-3.0.0/moku/finder.py
-drwxrwxr-x   0 sashi     (1001) sashi     (1001)        0 2023-05-12 04:51:08.925612 moku-3.0.0/moku/instruments/
--rw-rw-r--   0 sashi     (1001) sashi     (1001)      618 2023-02-20 03:40:59.000000 moku-3.0.0/moku/instruments/__init__.py
--rw-rw-r--   0 sashi     (1001) sashi     (1001)    11544 2023-04-30 23:41:00.000000 moku-3.0.0/moku/instruments/_awg.py
--rw-rw-r--   0 sashi     (1001) sashi     (1001)     5563 2023-01-27 07:08:13.000000 moku-3.0.0/moku/instruments/_cloudcompile.py
--rw-rw-r--   0 sashi     (1001) sashi     (1001)    13107 2023-02-20 03:40:59.000000 moku-3.0.0/moku/instruments/_datalogger.py
--rw-rw-r--   0 sashi     (1001) sashi     (1001)    29487 2023-04-30 23:41:00.000000 moku-3.0.0/moku/instruments/_digitalfilterbox.py
--rw-rw-r--   0 sashi     (1001) sashi     (1001)    34552 2023-04-30 23:41:00.000000 moku-3.0.0/moku/instruments/_firfilter.py
--rw-rw-r--   0 sashi     (1001) sashi     (1001)    14902 2023-04-30 23:41:00.000000 moku-3.0.0/moku/instruments/_fra.py
--rw-rw-r--   0 sashi     (1001) sashi     (1001)    35211 2023-04-30 23:41:00.000000 moku-3.0.0/moku/instruments/_laserlockbox.py
--rw-rw-r--   0 sashi     (1001) sashi     (1001)    27944 2023-02-20 03:40:59.000000 moku-3.0.0/moku/instruments/_lockinamp.py
--rw-rw-r--   0 sashi     (1001) sashi     (1001)    14999 2023-01-27 07:08:13.000000 moku-3.0.0/moku/instruments/_logicanalyzer.py
--rw-rw-r--   0 sashi     (1001) sashi     (1001)     6148 2023-04-10 23:20:50.000000 moku-3.0.0/moku/instruments/_mim.py
--rw-rw-r--   0 sashi     (1001) sashi     (1001)    24210 2023-04-30 23:41:00.000000 moku-3.0.0/moku/instruments/_oscilloscope.py
--rw-rw-r--   0 sashi     (1001) sashi     (1001)    17079 2023-05-05 05:13:01.000000 moku-3.0.0/moku/instruments/_phasemeter.py
--rw-rw-r--   0 sashi     (1001) sashi     (1001)    28679 2023-02-20 03:40:59.000000 moku-3.0.0/moku/instruments/_pidcontroller.py
--rw-rw-r--   0 sashi     (1001) sashi     (1001)    12184 2023-01-27 07:08:13.000000 moku-3.0.0/moku/instruments/_spectrumanalyzer.py
--rw-rw-r--   0 sashi     (1001) sashi     (1001)     4394 2023-02-20 03:40:59.000000 moku-3.0.0/moku/instruments/_stream.py
--rw-rw-r--   0 sashi     (1001) sashi     (1001)    15462 2023-04-30 23:41:00.000000 moku-3.0.0/moku/instruments/_waveformgenerator.py
--rw-rw-r--   0 sashi     (1001) sashi     (1001)     6189 2023-04-30 23:41:00.000000 moku-3.0.0/moku/session.py
--rw-rw-r--   0 sashi     (1001) sashi     (1001)      502 2023-02-09 22:36:03.000000 moku-3.0.0/moku/utilities.py
--rw-rw-r--   0 sashi     (1001) sashi     (1001)      311 2023-05-12 01:14:23.000000 moku-3.0.0/moku/version.py
-drwxrwxr-x   0 sashi     (1001) sashi     (1001)        0 2023-05-12 04:51:08.925612 moku-3.0.0/moku.egg-info/
--rw-rw-r--   0 sashi     (1001) sashi     (1001)     1146 2023-05-12 04:51:08.000000 moku-3.0.0/moku.egg-info/PKG-INFO
--rw-rw-r--   0 sashi     (1001) sashi     (1001)      883 2023-05-12 04:51:08.000000 moku-3.0.0/moku.egg-info/SOURCES.txt
--rw-rw-r--   0 sashi     (1001) sashi     (1001)        1 2023-05-12 04:51:08.000000 moku-3.0.0/moku.egg-info/dependency_links.txt
--rw-rw-r--   0 sashi     (1001) sashi     (1001)       40 2023-05-12 04:51:08.000000 moku-3.0.0/moku.egg-info/entry_points.txt
--rw-rw-r--   0 sashi     (1001) sashi     (1001)        1 2023-01-27 05:59:57.000000 moku-3.0.0/moku.egg-info/not-zip-safe
--rw-rw-r--   0 sashi     (1001) sashi     (1001)       26 2023-05-12 04:51:08.000000 moku-3.0.0/moku.egg-info/requires.txt
--rw-rw-r--   0 sashi     (1001) sashi     (1001)        5 2023-05-12 04:51:08.000000 moku-3.0.0/moku.egg-info/top_level.txt
--rw-rw-r--   0 sashi     (1001) sashi     (1001)       38 2023-05-12 04:51:08.929612 moku-3.0.0/setup.cfg
--rw-rw-r--   0 sashi     (1001) sashi     (1001)     1598 2023-05-12 04:50:47.000000 moku-3.0.0/setup.py
+drwxrwxr-x   0 sashi     (1001) sashi     (1001)        0 2023-07-21 01:14:15.517121 moku-3.1.0/
+-rw-rw-r--   0 sashi     (1001) sashi     (1001)     1146 2023-07-21 01:14:15.517121 moku-3.1.0/PKG-INFO
+-rw-rw-r--   0 sashi     (1001) sashi     (1001)     2674 2022-12-12 03:43:28.000000 moku-3.1.0/README.md
+drwxrwxr-x   0 sashi     (1001) sashi     (1001)        0 2023-07-21 01:14:15.517121 moku-3.1.0/moku/
+-rw-rw-r--   0 sashi     (1001) sashi     (1001)    11697 2023-07-21 01:01:36.000000 moku-3.1.0/moku/__init__.py
+-rw-rw-r--   0 sashi     (1001) sashi     (1001)     3758 2023-02-20 03:40:59.000000 moku-3.1.0/moku/cli.py
+-rw-rw-r--   0 sashi     (1001) sashi     (1001)     1672 2023-01-27 07:08:13.000000 moku-3.1.0/moku/exceptions.py
+-rw-rw-r--   0 sashi     (1001) sashi     (1001)     4353 2022-12-12 03:43:28.000000 moku-3.1.0/moku/finder.py
+drwxrwxr-x   0 sashi     (1001) sashi     (1001)        0 2023-07-21 01:14:15.517121 moku-3.1.0/moku/instruments/
+-rw-rw-r--   0 sashi     (1001) sashi     (1001)      618 2023-02-20 03:40:59.000000 moku-3.1.0/moku/instruments/__init__.py
+-rw-rw-r--   0 sashi     (1001) sashi     (1001)    11544 2023-04-30 23:41:00.000000 moku-3.1.0/moku/instruments/_awg.py
+-rw-rw-r--   0 sashi     (1001) sashi     (1001)     5785 2023-07-21 01:03:09.000000 moku-3.1.0/moku/instruments/_cloudcompile.py
+-rw-rw-r--   0 sashi     (1001) sashi     (1001)    13107 2023-02-20 03:40:59.000000 moku-3.1.0/moku/instruments/_datalogger.py
+-rw-rw-r--   0 sashi     (1001) sashi     (1001)    29487 2023-04-30 23:41:00.000000 moku-3.1.0/moku/instruments/_digitalfilterbox.py
+-rw-rw-r--   0 sashi     (1001) sashi     (1001)    34552 2023-04-30 23:41:00.000000 moku-3.1.0/moku/instruments/_firfilter.py
+-rw-rw-r--   0 sashi     (1001) sashi     (1001)    14902 2023-04-30 23:41:00.000000 moku-3.1.0/moku/instruments/_fra.py
+-rw-rw-r--   0 sashi     (1001) sashi     (1001)    35211 2023-04-30 23:41:00.000000 moku-3.1.0/moku/instruments/_laserlockbox.py
+-rw-rw-r--   0 sashi     (1001) sashi     (1001)    27944 2023-02-20 03:40:59.000000 moku-3.1.0/moku/instruments/_lockinamp.py
+-rw-rw-r--   0 sashi     (1001) sashi     (1001)    14999 2023-01-27 07:08:13.000000 moku-3.1.0/moku/instruments/_logicanalyzer.py
+-rw-rw-r--   0 sashi     (1001) sashi     (1001)     6168 2023-07-21 01:01:24.000000 moku-3.1.0/moku/instruments/_mim.py
+-rw-rw-r--   0 sashi     (1001) sashi     (1001)    24210 2023-04-30 23:41:00.000000 moku-3.1.0/moku/instruments/_oscilloscope.py
+-rw-rw-r--   0 sashi     (1001) sashi     (1001)    17106 2023-07-16 23:33:36.000000 moku-3.1.0/moku/instruments/_phasemeter.py
+-rw-rw-r--   0 sashi     (1001) sashi     (1001)    28679 2023-02-20 03:40:59.000000 moku-3.1.0/moku/instruments/_pidcontroller.py
+-rw-rw-r--   0 sashi     (1001) sashi     (1001)    12184 2023-01-27 07:08:13.000000 moku-3.1.0/moku/instruments/_spectrumanalyzer.py
+-rw-rw-r--   0 sashi     (1001) sashi     (1001)     4394 2023-02-20 03:40:59.000000 moku-3.1.0/moku/instruments/_stream.py
+-rw-rw-r--   0 sashi     (1001) sashi     (1001)    15462 2023-04-30 23:41:00.000000 moku-3.1.0/moku/instruments/_waveformgenerator.py
+-rw-rw-r--   0 sashi     (1001) sashi     (1001)     6189 2023-04-30 23:41:00.000000 moku-3.1.0/moku/session.py
+-rw-rw-r--   0 sashi     (1001) sashi     (1001)      502 2023-02-09 22:36:03.000000 moku-3.1.0/moku/utilities.py
+-rw-rw-r--   0 sashi     (1001) sashi     (1001)      311 2023-07-16 23:33:15.000000 moku-3.1.0/moku/version.py
+drwxrwxr-x   0 sashi     (1001) sashi     (1001)        0 2023-07-21 01:14:15.517121 moku-3.1.0/moku.egg-info/
+-rw-rw-r--   0 sashi     (1001) sashi     (1001)     1146 2023-07-21 01:14:15.000000 moku-3.1.0/moku.egg-info/PKG-INFO
+-rw-rw-r--   0 sashi     (1001) sashi     (1001)      883 2023-07-21 01:14:15.000000 moku-3.1.0/moku.egg-info/SOURCES.txt
+-rw-rw-r--   0 sashi     (1001) sashi     (1001)        1 2023-07-21 01:14:15.000000 moku-3.1.0/moku.egg-info/dependency_links.txt
+-rw-rw-r--   0 sashi     (1001) sashi     (1001)       40 2023-07-21 01:14:15.000000 moku-3.1.0/moku.egg-info/entry_points.txt
+-rw-rw-r--   0 sashi     (1001) sashi     (1001)        1 2023-01-27 05:59:57.000000 moku-3.1.0/moku.egg-info/not-zip-safe
+-rw-rw-r--   0 sashi     (1001) sashi     (1001)       26 2023-07-21 01:14:15.000000 moku-3.1.0/moku.egg-info/requires.txt
+-rw-rw-r--   0 sashi     (1001) sashi     (1001)        5 2023-07-21 01:14:15.000000 moku-3.1.0/moku.egg-info/top_level.txt
+-rw-rw-r--   0 sashi     (1001) sashi     (1001)       38 2023-07-21 01:14:15.517121 moku-3.1.0/setup.cfg
+-rw-rw-r--   0 sashi     (1001) sashi     (1001)     1598 2023-07-21 01:01:24.000000 moku-3.1.0/setup.py
```

### Comparing `moku-3.0.0/PKG-INFO` & `moku-3.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moku
-Version: 3.0.0
+Version: 3.1.0
 Summary: Python scripting interface to the Liquid Instruments Moku hardware
 Home-page: https://liquidinstruments.com
 Author: Liquid Instruments
 Author-email: info@liquidinstruments.com
 License: MIT
 Description: 
                 # Moku
```

### Comparing `moku-3.0.0/README.md` & `moku-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `moku-3.0.0/moku/__init__.py` & `moku-3.1.0/moku/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,22 @@
+import pathlib
 import tarfile
 from hashlib import sha256
 from os import environ
 from pathlib import Path
 from shutil import which
 from subprocess import Popen, PIPE
 
 from pkg_resources import get_distribution, resource_filename
 
-from moku.exceptions import IncompatibleMokuException
+from moku.exceptions import IncompatibleMokuException, MokuException
 from moku.session import RequestSession
 from moku.utilities import validate_range
-from moku.version import compat_fw, cli_ver_major, cli_ver_minor, cli_ver_patch
+from moku.version import compat_fw, cli_ver_major, cli_ver_minor, \
+    cli_ver_patch
 
 __version__ = get_distribution("moku").version
 _data_path = environ.get('MOKU_DATA_PATH',
                          resource_filename("moku", 'data'))
 MOKU_DATA_PATH = Path(_data_path).expanduser()
 
 MOKU_CLI_PATH = environ.get('MOKU_CLI_PATH', which("mokucli"))
@@ -56,53 +58,60 @@
                 f"package supports firmware version"
                 f"{compat_fw} or above.")
 
         self.firmware_version = props['firmware']
         self.hardware = props['hardware'].replace(":", "").lower()
         self.bitstreams = props['bitstreams']
 
-    def _read_and_upload_stream(self, bs_name, chksum):
-        bs_path = MOKU_DATA_PATH.joinpath(bs_name)
-        if bs_path.exists():
-            bs_data = bs_path.read_bytes()
-            if not (chksum and sha256(bs_data).hexdigest() == chksum):
-                self.upload("bitstreams", bs_name, bs_data)
+    def _read_and_upload_stream(self, bs_name, chksum, bs_path=None):
+        if bs_path:
+            bs_path = pathlib.Path(bs_path)
+            if not bs_path.exists():
+                raise MokuException(f"Cannot find {bs_path}")
+            bs_file_name = bs_name
         else:
-            data_file = self._get_data_file(self.firmware_version)
+            bs_path = self._get_data_file(self.firmware_version)
             hw_dir = {"mokupro": "mokupro",
-                      "mokugo": "mokugo", 
+                      "mokugo": "mokugo",
                       "mokulab": "moku20"}
-            with tarfile.open(data_file) as _ts:
-                bs_tarinfo = _ts.getmember(
-                    f"{hw_dir[self.hardware]}/{bs_name}")
-                bs_file = _ts.extractfile(bs_tarinfo)
-                bs_data = bs_file.read()
-                if not (chksum and sha256(
-                        bs_data).hexdigest() == chksum):
-                    self.upload("bitstreams", bs_name, bs_data)
-                bs_file.close()
+            bs_file_name = f"{hw_dir[self.hardware]}/{bs_name}"
+
+        with tarfile.open(bs_path) as _ts:
+            bs_tar_info = _ts.getmember(bs_file_name)
+            bs_file = _ts.extractfile(bs_tar_info)
+            bs_data = bs_file.read()
+            if not (chksum and sha256(
+                    bs_data).hexdigest() == chksum):
+                self.upload("bitstreams", bs_name, bs_data)
+            bs_file.close()
 
-    def upload_bitstream(self, name):
+    def upload_bitstream(self, name, bs_path=None):
         matching = [b for b in self.bitstreams if b["name"] == name]
         chksum = matching[0].get("checksum") if matching else None
-        self._read_and_upload_stream(name, chksum)
+        self._read_and_upload_stream(name, chksum, bs_path)
 
     def set_connect_timeout(self, value):
         if not isinstance(value, tuple([int, float])):
             raise Exception("set_connect_timeout value should be "
                             "either integer or float")
         self.session.connect_timeout = value
 
     def set_read_timeout(self, value):
         if not isinstance(value, tuple([int, float])):
             raise Exception("read_timeout value should be either "
                             "integer or float")
         self.session.read_timeout = value
 
     def platform(self, platform_id):
+        platform_map = {"mokupro": [1, 4],
+                        "mokugo": [1, 2],
+                        "mokulab": [1, 2]}
+        if platform_id not in platform_map[self.hardware]:
+            raise MokuException(f"The platform_id {platform_id} is invalid. For '{self.hardware}' available options are {platform_map[self.hardware]}") # noqa
+            
         operation = f"platform/{platform_id}"
         self.upload_bitstream(f"{platform_id:02}-000")
         for i in range(0, platform_id):
             self.upload_bitstream(f"{platform_id:02}-000-{i:02}")
         return self.session.get("moku", operation)
 
     @staticmethod
```

### Comparing `moku-3.0.0/moku/cli.py` & `moku-3.1.0/moku/cli.py`

 * *Files identical despite different names*

### Comparing `moku-3.0.0/moku/exceptions.py` & `moku-3.1.0/moku/exceptions.py`

 * *Files identical despite different names*

### Comparing `moku-3.0.0/moku/finder.py` & `moku-3.1.0/moku/finder.py`

 * *Files identical despite different names*

### Comparing `moku-3.0.0/moku/instruments/__init__.py` & `moku-3.1.0/moku/instruments/__init__.py`

 * *Files identical despite different names*

### Comparing `moku-3.0.0/moku/instruments/_awg.py` & `moku-3.1.0/moku/instruments/_awg.py`

 * *Files identical despite different names*

### Comparing `moku-3.0.0/moku/instruments/_cloudcompile.py` & `moku-3.1.0/moku/instruments/_cloudcompile.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     """
                Cloud Compile - Custom Instrument
 
                """
 
     def __init__(self, ip=None, serial=None, force_connect=False,
                  ignore_busy=False, persist_state=False,
+                 bitstream=None,
                  connect_timeout=15, read_timeout=30, slot=None,
                  multi_instrument=None, **kwargs):
         self.id = 255
         self.operation_group = "cloudcompile"
 
         if multi_instrument is None:
             self.slot = 1
@@ -27,29 +28,33 @@
             super().__init__(ip=ip, force_connect=force_connect,
                              ignore_busy=ignore_busy,
                              persist_state=persist_state,
                              connect_timeout=connect_timeout,
                              read_timeout=read_timeout,
                              **kwargs)
             self.upload_bitstream(f'01-000')
-            self.upload_bitstream(f'01-{self.id:03}-00')
+            self.upload_bitstream(f'01-{self.id:03}-00',
+                                  bs_path=bitstream)
         else:
             self.platform_id = multi_instrument.platform_id
             self.slot = slot
             self.session = multi_instrument.session
             self.firmware_version = multi_instrument.firmware_version
             self.hardware = multi_instrument.hardware
             self.bitstreams = multi_instrument.bitstreams
             self.upload_bitstream(
-                f'{self.platform_id:02}-{self.id:03}-{self.slot - 1:02}')
+                f'{self.platform_id:02}-{self.id:03}-{self.slot - 1:02}', # noqa
+                bs_path=bitstream)
             self.session.get(f"slot{self.slot}", self.operation_group)
 
     @classmethod
-    def for_slot(cls, slot, multi_instrument):
-        return cls(slot=slot, multi_instrument=multi_instrument)
+    def for_slot(cls, slot, multi_instrument, **kwargs):
+        bitstream = kwargs.get("bitstream")
+        return cls(slot=slot, multi_instrument=multi_instrument,
+                   bitstream=bitstream)
 
     def set_controls(self, controls, strict=True):
         """
         set_controls.
 
         :type strict: `boolean`
         :param strict: Disable all implicit conversions and coercions.
```

### Comparing `moku-3.0.0/moku/instruments/_datalogger.py` & `moku-3.1.0/moku/instruments/_datalogger.py`

 * *Files identical despite different names*

### Comparing `moku-3.0.0/moku/instruments/_digitalfilterbox.py` & `moku-3.1.0/moku/instruments/_digitalfilterbox.py`

 * *Files identical despite different names*

### Comparing `moku-3.0.0/moku/instruments/_firfilter.py` & `moku-3.1.0/moku/instruments/_firfilter.py`

 * *Files identical despite different names*

### Comparing `moku-3.0.0/moku/instruments/_fra.py` & `moku-3.1.0/moku/instruments/_fra.py`

 * *Files identical despite different names*

### Comparing `moku-3.0.0/moku/instruments/_laserlockbox.py` & `moku-3.1.0/moku/instruments/_laserlockbox.py`

 * *Files identical despite different names*

### Comparing `moku-3.0.0/moku/instruments/_lockinamp.py` & `moku-3.1.0/moku/instruments/_lockinamp.py`

 * *Files identical despite different names*

### Comparing `moku-3.0.0/moku/instruments/_logicanalyzer.py` & `moku-3.1.0/moku/instruments/_logicanalyzer.py`

 * *Files identical despite different names*

### Comparing `moku-3.0.0/moku/instruments/_mim.py` & `moku-3.1.0/moku/instruments/_mim.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,30 +29,30 @@
                          persist_state=persist_state,
                          connect_timeout=connect_timeout,
                          read_timeout=read_timeout,
                          **kwargs)
 
         self.platform(self.platform_id)
 
-    def set_instrument(self, slot, instrument):
+    def set_instrument(self, slot, instrument, **kwargs):
         if not 1 <= slot <= self.platform_id:
             raise Exception(f"Invalid slot for {self.platform_id} "
                             f"slot platform")
 
         if instrument not in [x[1] for x in getmembers(instruments,
                                                        isclass)]:
             raise Exception(f"{instrument} is not a valid instrument")
 
         empty_slots = [i for i, v in enumerate(self.get_instruments())
                        if i + 1 != slot and v == ""]
 
         for i in empty_slots:
             self.upload_bitstream(f"{self.platform_id:02}-000-{i:02}")
 
-        return instrument.for_slot(slot, self)
+        return instrument.for_slot(slot, self, **kwargs)
 
     def set_connections(self, connections):
         """
         set_connections.
 
         :type connections: `list`
         :param connections: List of map of source and destination points.
```

### Comparing `moku-3.0.0/moku/instruments/_oscilloscope.py` & `moku-3.1.0/moku/instruments/_oscilloscope.py`

 * *Files identical despite different names*

### Comparing `moku-3.0.0/moku/instruments/_phasemeter.py` & `moku-3.1.0/moku/instruments/_phasemeter.py`

 * *Files 1% similar despite different names*

```diff
@@ -239,16 +239,17 @@
 
     def generate_output(
             self,
             channel,
             signal,
             amplitude=0.5,
             frequency=1e6,
-            frequency_multplier=1,
+            frequency_multiplier=1,
             phase=0,
+            offset=0,
             phase_locked=False,
             scaling=0.001,
             strict=True):
         """
         generate_output.
 
         :type strict: `boolean`
@@ -262,16 +263,16 @@
 
         :type amplitude: `number`
         :param amplitude: Waveform peak-to-peak amplitude
 
         :type frequency: `number`
         :param frequency: Frequency of the wave
 
-        :type frequency_multplier: `number`
-        :param frequency_multplier: Frequency multiplier
+        :type frequency_multiplier: `number`
+        :param frequency_multiplier: Frequency multiplier
 
         :type phase: `number`
         :param phase: Phase offset of the wave
 
         :type phase_locked: `boolean`
         :param phase_locked: Locks the phase of the generated sinewave to the measured phase of the input signal
 
@@ -280,18 +281,18 @@
 
         """
         operation = "generate_output"
         params = dict(
             strict=strict,
             channel=channel,
             signal=validate_range(
-                signal, ['Sine', 'Phase', 'FrequencyOffset', 'Amptitude']),
+                signal, ['Sine', 'Phase', 'FrequencyOffset', 'Amplitude']),
             amplitude=amplitude,
             frequency=frequency,
-            frequency_multplier=frequency_multplier,
+            frequency_multiplier=frequency_multiplier,
             phase=phase,
             phase_locked=phase_locked,
             scaling=scaling,
         )
         return self.session.post(
             f"slot{self.slot}/{self.operation_group}",
             operation,
```

### Comparing `moku-3.0.0/moku/instruments/_pidcontroller.py` & `moku-3.1.0/moku/instruments/_pidcontroller.py`

 * *Files identical despite different names*

### Comparing `moku-3.0.0/moku/instruments/_spectrumanalyzer.py` & `moku-3.1.0/moku/instruments/_spectrumanalyzer.py`

 * *Files identical despite different names*

### Comparing `moku-3.0.0/moku/instruments/_stream.py` & `moku-3.1.0/moku/instruments/_stream.py`

 * *Files identical despite different names*

### Comparing `moku-3.0.0/moku/instruments/_waveformgenerator.py` & `moku-3.1.0/moku/instruments/_waveformgenerator.py`

 * *Files identical despite different names*

### Comparing `moku-3.0.0/moku/session.py` & `moku-3.1.0/moku/session.py`

 * *Files identical despite different names*

### Comparing `moku-3.0.0/moku.egg-info/PKG-INFO` & `moku-3.1.0/moku.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moku
-Version: 3.0.0
+Version: 3.1.0
 Summary: Python scripting interface to the Liquid Instruments Moku hardware
 Home-page: https://liquidinstruments.com
 Author: Liquid Instruments
 Author-email: info@liquidinstruments.com
 License: MIT
 Description: 
                 # Moku
```

### Comparing `moku-3.0.0/moku.egg-info/SOURCES.txt` & `moku-3.1.0/moku.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `moku-3.0.0/setup.py` & `moku-3.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 import os.path
 
 setup(
     name="moku",
-    version="3.0.0",
+    version="3.1.0",
     author='Liquid Instruments',
     author_email='info@liquidinstruments.com',
     packages=['moku'],
     package_dir={'moku': 'moku'},
     package_data={
         'moku': [
             os.path.join('instruments', '*'),
```

