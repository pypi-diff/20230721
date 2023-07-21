# Comparing `tmp/enapter-0.7.2-py3-none-any.whl.zip` & `tmp/enapter-0.7.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,36 +1,37 @@
-Zip file size: 18718 bytes, number of entries: 34
--rw-r--r--  2.0 unx      182 b- defN 23-Jul-18 19:23 enapter/__init__.py
--rw-r--r--  2.0 unx       52 b- defN 23-Jul-18 19:23 enapter/types.py
--rw-r--r--  2.0 unx      109 b- defN 23-Jul-18 19:23 enapter/async_/__init__.py
--rw-r--r--  2.0 unx      300 b- defN 23-Jul-18 19:23 enapter/async_/generator.py
--rw-r--r--  2.0 unx     1770 b- defN 23-Jul-18 19:23 enapter/async_/routine.py
--rw-r--r--  2.0 unx      600 b- defN 23-Jul-18 19:23 enapter/log/__init__.py
--rw-r--r--  2.0 unx      705 b- defN 23-Jul-18 19:23 enapter/log/json_formatter.py
--rw-r--r--  2.0 unx       55 b- defN 23-Jul-18 19:23 enapter/mdns/__init__.py
--rw-r--r--  2.0 unx     1297 b- defN 23-Jul-18 19:23 enapter/mdns/resolver.py
--rw-r--r--  2.0 unx      336 b- defN 23-Jul-18 19:23 enapter/mqtt/__init__.py
--rw-r--r--  2.0 unx     5073 b- defN 23-Jul-18 19:23 enapter/mqtt/client.py
--rw-r--r--  2.0 unx     1092 b- defN 23-Jul-18 19:23 enapter/mqtt/command.py
--rw-r--r--  2.0 unx     1399 b- defN 23-Jul-18 19:23 enapter/mqtt/config.py
--rw-r--r--  2.0 unx     2501 b- defN 23-Jul-18 19:23 enapter/mqtt/device_channel.py
--rw-r--r--  2.0 unx      177 b- defN 23-Jul-18 19:23 enapter/vucm/__init__.py
--rw-r--r--  2.0 unx     1325 b- defN 23-Jul-18 19:23 enapter/vucm/app.py
--rw-r--r--  2.0 unx     1649 b- defN 23-Jul-18 19:23 enapter/vucm/config.py
--rw-r--r--  2.0 unx     2923 b- defN 23-Jul-18 19:23 enapter/vucm/device.py
--rw-r--r--  2.0 unx     1354 b- defN 23-Jul-18 19:23 enapter/vucm/logger.py
--rw-r--r--  2.0 unx      824 b- defN 23-Jul-18 19:23 enapter/vucm/ucm.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-18 19:23 tests/__init__.py
--rw-r--r--  2.0 unx      397 b- defN 23-Jul-18 19:23 tests/conftest.py
--rw-r--r--  2.0 unx      587 b- defN 23-Jul-18 19:23 tests/fake_data_generator.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-18 19:23 tests/integration/__init__.py
--rw-r--r--  2.0 unx     1617 b- defN 23-Jul-18 19:23 tests/integration/conftest.py
--rw-r--r--  2.0 unx     3889 b- defN 23-Jul-18 19:23 tests/integration/test_mqtt.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-18 19:23 tests/unit/__init__.py
--rw-r--r--  2.0 unx     4208 b- defN 23-Jul-18 19:23 tests/unit/test_async.py
--rw-r--r--  2.0 unx     1876 b- defN 23-Jul-18 19:23 tests/unit/test_log.py
--rw-r--r--  2.0 unx     2654 b- defN 23-Jul-18 19:23 tests/unit/test_mqtt.py
--rw-r--r--  2.0 unx     3159 b- defN 23-Jul-18 19:24 enapter-0.7.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-18 19:24 enapter-0.7.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       14 b- defN 23-Jul-18 19:24 enapter-0.7.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     2688 b- defN 23-Jul-18 19:24 enapter-0.7.2.dist-info/RECORD
-34 files, 44904 bytes uncompressed, 14450 bytes compressed:  67.8%
+Zip file size: 19058 bytes, number of entries: 35
+-rw-r--r--  2.0 unx      182 b- defN 23-Jul-21 16:34 enapter/__init__.py
+-rw-r--r--  2.0 unx       52 b- defN 23-Jul-21 16:34 enapter/types.py
+-rw-r--r--  2.0 unx      177 b- defN 23-Jul-21 16:34 enapter/async_/__init__.py
+-rw-r--r--  2.0 unx      300 b- defN 23-Jul-21 16:34 enapter/async_/generator.py
+-rw-r--r--  2.0 unx     1770 b- defN 23-Jul-21 16:34 enapter/async_/routine.py
+-rw-r--r--  2.0 unx      208 b- defN 23-Jul-21 16:34 enapter/async_/run_in_executor.py
+-rw-r--r--  2.0 unx      600 b- defN 23-Jul-21 16:34 enapter/log/__init__.py
+-rw-r--r--  2.0 unx      705 b- defN 23-Jul-21 16:34 enapter/log/json_formatter.py
+-rw-r--r--  2.0 unx       55 b- defN 23-Jul-21 16:34 enapter/mdns/__init__.py
+-rw-r--r--  2.0 unx     1297 b- defN 23-Jul-21 16:34 enapter/mdns/resolver.py
+-rw-r--r--  2.0 unx      336 b- defN 23-Jul-21 16:34 enapter/mqtt/__init__.py
+-rw-r--r--  2.0 unx     5073 b- defN 23-Jul-21 16:34 enapter/mqtt/client.py
+-rw-r--r--  2.0 unx     1092 b- defN 23-Jul-21 16:34 enapter/mqtt/command.py
+-rw-r--r--  2.0 unx     1399 b- defN 23-Jul-21 16:34 enapter/mqtt/config.py
+-rw-r--r--  2.0 unx     2501 b- defN 23-Jul-21 16:34 enapter/mqtt/device_channel.py
+-rw-r--r--  2.0 unx      177 b- defN 23-Jul-21 16:34 enapter/vucm/__init__.py
+-rw-r--r--  2.0 unx     1325 b- defN 23-Jul-21 16:34 enapter/vucm/app.py
+-rw-r--r--  2.0 unx     1649 b- defN 23-Jul-21 16:34 enapter/vucm/config.py
+-rw-r--r--  2.0 unx     2923 b- defN 23-Jul-21 16:34 enapter/vucm/device.py
+-rw-r--r--  2.0 unx     1354 b- defN 23-Jul-21 16:34 enapter/vucm/logger.py
+-rw-r--r--  2.0 unx      824 b- defN 23-Jul-21 16:34 enapter/vucm/ucm.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-21 16:34 tests/__init__.py
+-rw-r--r--  2.0 unx      397 b- defN 23-Jul-21 16:34 tests/conftest.py
+-rw-r--r--  2.0 unx      587 b- defN 23-Jul-21 16:34 tests/fake_data_generator.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-21 16:34 tests/integration/__init__.py
+-rw-r--r--  2.0 unx     1617 b- defN 23-Jul-21 16:34 tests/integration/conftest.py
+-rw-r--r--  2.0 unx     3889 b- defN 23-Jul-21 16:34 tests/integration/test_mqtt.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-21 16:34 tests/unit/__init__.py
+-rw-r--r--  2.0 unx     4208 b- defN 23-Jul-21 16:34 tests/unit/test_async.py
+-rw-r--r--  2.0 unx     1876 b- defN 23-Jul-21 16:34 tests/unit/test_log.py
+-rw-r--r--  2.0 unx     2654 b- defN 23-Jul-21 16:34 tests/unit/test_mqtt.py
+-rw-r--r--  2.0 unx     3159 b- defN 23-Jul-21 16:34 enapter-0.7.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-21 16:34 enapter-0.7.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       14 b- defN 23-Jul-21 16:34 enapter-0.7.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     2777 b- defN 23-Jul-21 16:34 enapter-0.7.3.dist-info/RECORD
+35 files, 45269 bytes uncompressed, 14648 bytes compressed:  67.6%
```

## zipnote {}

```diff
@@ -9,14 +9,17 @@
 
 Filename: enapter/async_/generator.py
 Comment: 
 
 Filename: enapter/async_/routine.py
 Comment: 
 
+Filename: enapter/async_/run_in_executor.py
+Comment: 
+
 Filename: enapter/log/__init__.py
 Comment: 
 
 Filename: enapter/log/json_formatter.py
 Comment: 
 
 Filename: enapter/mdns/__init__.py
@@ -84,20 +87,20 @@
 
 Filename: tests/unit/test_log.py
 Comment: 
 
 Filename: tests/unit/test_mqtt.py
 Comment: 
 
-Filename: enapter-0.7.2.dist-info/METADATA
+Filename: enapter-0.7.3.dist-info/METADATA
 Comment: 
 
-Filename: enapter-0.7.2.dist-info/WHEEL
+Filename: enapter-0.7.3.dist-info/WHEEL
 Comment: 
 
-Filename: enapter-0.7.2.dist-info/top_level.txt
+Filename: enapter-0.7.3.dist-info/top_level.txt
 Comment: 
 
-Filename: enapter-0.7.2.dist-info/RECORD
+Filename: enapter-0.7.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## enapter/__init__.py

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.7.2"
+__version__ = "0.7.3"
 
 from . import async_, log, mdns, mqtt, types, vucm
 
 __all__ = [
     "__version__",
     "async_",
     "log",
```

## enapter/async_/__init__.py

```diff
@@ -1,7 +1,9 @@
 from .generator import generator
 from .routine import Routine
+from .run_in_executor import run_in_executor
 
 __all__ = [
     "generator",
     "Routine",
+    "run_in_executor",
 ]
```

## Comparing `enapter-0.7.2.dist-info/METADATA` & `enapter-0.7.3.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enapter
-Version: 0.7.2
+Version: 0.7.3
 Summary: Enapter Python SDK
 Home-page: https://github.com/Enapter/python-sdk
 Author: Roman Novatorov
 Author-email: rnovatorov@enapter.com
 Description-Content-Type: text/markdown
 Requires-Dist: aiomqtt (==1.0.*)
 Requires-Dist: dnspython (==2.2.*)
```

## Comparing `enapter-0.7.2.dist-info/RECORD` & `enapter-0.7.3.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-enapter/__init__.py,sha256=KEX0qxXIayHPcrYVMVHLcbwwPXda38oMl6zkvGM0spc,182
+enapter/__init__.py,sha256=6Dgka_TwSG3cKbuFdTS1oOlSvzB_zv36EXM-0FJAaQk,182
 enapter/types.py,sha256=2366bx_VI7bIBNnIaG5sol7G4k0PqaQ6oS74dzM4l1M,52
-enapter/async_/__init__.py,sha256=JuiRI2bN2AgB-HLfAUoSsZpEziwFRftNNEp59Evnd0M,109
+enapter/async_/__init__.py,sha256=8T5zccEtvc-keLwUtet3qMfOJ2NyIvNOWtQlTr5elYc,177
 enapter/async_/generator.py,sha256=qBhnt36Gl2166sJFnZHsREbZu8l43M4DfxybUMIv6W4,300
 enapter/async_/routine.py,sha256=A5fG4XnCEQT0Qa_JNh1N43Fv5lnLaCoGF4xt6pOAdNs,1770
+enapter/async_/run_in_executor.py,sha256=V4z54_L11Jjx4wG1LSinZmLtL2DJccVQPjx83HtKgUE,208
 enapter/log/__init__.py,sha256=n1sWMDKJSs_ebZzjbTrVdfg-oi0V1tvliTxgIV-msJ0,600
 enapter/log/json_formatter.py,sha256=P46zEdU5-dr3mDMkUjBy7z_FSMPi61RUgEYyBEfqVNQ,705
 enapter/mdns/__init__.py,sha256=uwsg8wJ0Lcsr9oOEW1PkEV3jVgWzgA7RG2ur_MRLtM0,55
 enapter/mdns/resolver.py,sha256=FFQuZiaKOaNtfSgI2YOaSdG-BuZwOKmYVy06Sc735Zo,1297
 enapter/mqtt/__init__.py,sha256=D_RK-cScavukvDvwahEwvlvGLHSPsVLjG_JpdvpC2ok,336
 enapter/mqtt/client.py,sha256=63mCTcTzo7TcoXjuX6bHGLNDjLM3t105f-Jbv0bKKeM,5073
 enapter/mqtt/command.py,sha256=ozhDTjRrdCWv_bzPTjVFpL8tx7nhirm3JtQaD45wTdo,1092
@@ -24,11 +25,11 @@
 tests/integration/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/integration/conftest.py,sha256=TpbUrExImSsLp77FIp1O-6wJrxgTmyxCgmmATIDEmL4,1617
 tests/integration/test_mqtt.py,sha256=7n7BvJOEMHB-5m6ee-uZ5wcQyK7465wlKB6ZnUoWQtQ,3889
 tests/unit/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/unit/test_async.py,sha256=KwhwKBSeSb7Qyaf50Ca2LGB7gm3m5j5wgGgWnvYY98k,4208
 tests/unit/test_log.py,sha256=DQD1OCVkYYzy-Kq-jH_xsaRDtiwIqULuTgMitjSeiuo,1876
 tests/unit/test_mqtt.py,sha256=HGECSG_WGeods6zE4ZcmRh8m0NPnNyd3dwBMkGqqKlo,2654
-enapter-0.7.2.dist-info/METADATA,sha256=h7H0GcdQ-eUe6SkDpJBd6FX7SdwHRJ_c4qRwKthBso4,3159
-enapter-0.7.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-enapter-0.7.2.dist-info/top_level.txt,sha256=DsMzVradd7z3A0fm7zmn9oh08ijO41RtzglrnPlx54w,14
-enapter-0.7.2.dist-info/RECORD,,
+enapter-0.7.3.dist-info/METADATA,sha256=8VzNMRwX-5vgizyXVKwF6N0Y2ra5UTwngZrsa_huaj0,3159
+enapter-0.7.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+enapter-0.7.3.dist-info/top_level.txt,sha256=DsMzVradd7z3A0fm7zmn9oh08ijO41RtzglrnPlx54w,14
+enapter-0.7.3.dist-info/RECORD,,
```

