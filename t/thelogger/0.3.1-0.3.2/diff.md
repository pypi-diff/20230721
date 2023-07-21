# Comparing `tmp/thelogger-0.3.1-py3-none-any.whl.zip` & `tmp/thelogger-0.3.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,15 @@
-Zip file size: 13932 bytes, number of entries: 12
--rw-rw-rw-  2.0 fat      297 b- defN 23-Jun-17 04:40 thelogger/__init__.py
--rw-rw-rw-  2.0 fat      214 b- defN 23-Apr-27 17:46 thelogger/_ver.py
+Zip file size: 15243 bytes, number of entries: 13
+-rw-rw-rw-  2.0 fat      486 b- defN 23-Jul-21 04:09 thelogger/__init__.py
+-rw-rw-rw-  2.0 fat     4234 b- defN 22-Feb-20 09:05 thelogger/__logger.py
+-rw-rw-rw-  2.0 fat      214 b- defN 23-Apr-27 17:46 thelogger/__ver.py
 -rw-rw-rw-  2.0 fat     1049 b- defN 23-Jun-17 05:10 thelogger/dirty_timer.py
--rw-rw-rw-  2.0 fat     4234 b- defN 22-Feb-20 09:05 thelogger/logger.py
+-rw-rw-rw-  2.0 fat     3352 b- defN 23-Jul-21 04:17 thelogger/sys_meta.py
 -rw-rw-rw-  2.0 fat      140 b- defN 22-Feb-20 09:05 thelogger/notify/__init__.py
 -rw-rw-rw-  2.0 fat     3611 b- defN 22-Feb-20 09:49 thelogger/notify/decorator.py
 -rw-rw-rw-  2.0 fat     6990 b- defN 23-Feb-28 14:35 thelogger/notify/exec_func.py
--rw-rw-rw-  2.0 fat    11558 b- defN 23-Jun-17 05:11 thelogger-0.3.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     6627 b- defN 23-Jun-17 05:11 thelogger-0.3.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-17 05:11 thelogger-0.3.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       10 b- defN 23-Jun-17 05:11 thelogger-0.3.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      960 b- defN 23-Jun-17 05:11 thelogger-0.3.1.dist-info/RECORD
-12 files, 35782 bytes uncompressed, 12326 bytes compressed:  65.6%
+-rw-rw-rw-  2.0 fat    11558 b- defN 23-Jul-21 04:19 thelogger-0.3.2.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     6692 b- defN 23-Jul-21 04:19 thelogger-0.3.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-21 04:19 thelogger-0.3.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       10 b- defN 23-Jul-21 04:19 thelogger-0.3.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1041 b- defN 23-Jul-21 04:19 thelogger-0.3.2.dist-info/RECORD
+13 files, 39469 bytes uncompressed, 13513 bytes compressed:  65.8%
```

## zipnote {}

```diff
@@ -1,37 +1,40 @@
 Filename: thelogger/__init__.py
 Comment: 
 
-Filename: thelogger/_ver.py
+Filename: thelogger/__logger.py
+Comment: 
+
+Filename: thelogger/__ver.py
 Comment: 
 
 Filename: thelogger/dirty_timer.py
 Comment: 
 
-Filename: thelogger/logger.py
+Filename: thelogger/sys_meta.py
 Comment: 
 
 Filename: thelogger/notify/__init__.py
 Comment: 
 
 Filename: thelogger/notify/decorator.py
 Comment: 
 
 Filename: thelogger/notify/exec_func.py
 Comment: 
 
-Filename: thelogger-0.3.1.dist-info/LICENSE
+Filename: thelogger-0.3.2.dist-info/LICENSE
 Comment: 
 
-Filename: thelogger-0.3.1.dist-info/METADATA
+Filename: thelogger-0.3.2.dist-info/METADATA
 Comment: 
 
-Filename: thelogger-0.3.1.dist-info/WHEEL
+Filename: thelogger-0.3.2.dist-info/WHEEL
 Comment: 
 
-Filename: thelogger-0.3.1.dist-info/top_level.txt
+Filename: thelogger-0.3.2.dist-info/top_level.txt
 Comment: 
 
-Filename: thelogger-0.3.1.dist-info/RECORD
+Filename: thelogger-0.3.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## thelogger/__init__.py

```diff
@@ -3,12 +3,24 @@
 Created on Sat Oct 23 04:36:47 2019
 
 Easy logging, timing and email notifications of code execution.
 
 @author: tommy
 """
 
-from .logger import logger, log, lg
+from .__logger import logger, log, lg
 from .notify import notify
 from .dirty_timer import beg, end, timer
+from .sys_meta import (
+    get_cpu_model,
+    get_machine_info,
+    get_resource_usage,
+    get_env_info,
+    sys_info
+    )
 
-from ._ver import __version__
+from .__ver import __version__
+
+try:
+    del __ver, __logger
+except:
+    pass
```

## Comparing `thelogger/logger.py` & `thelogger/__logger.py`

 * *Files identical despite different names*

## Comparing `thelogger-0.3.1.dist-info/LICENSE` & `thelogger-0.3.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `thelogger-0.3.1.dist-info/METADATA` & `thelogger-0.3.2.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thelogger
-Version: 0.3.1
+Version: 0.3.2
 Summary: Easy logging, timing and email notifications of code execution.
 Home-page: https://github.com/tom1919/TheLogger
 Author: Tom1919
 Author-email: py.notify1@gmail.com
 License: Apache 2.0
 Keywords: log,logging,logger,email,timimg,notification
 Platform: UNKNOWN
@@ -17,14 +17,17 @@
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Requires-Python: >3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pandas
 Requires-Dist: tabulate
+Requires-Dist: pytz
+Requires-Dist: psutil
+Requires-Dist: tzlocal
 Requires-Dist: importlib-metadata (>=1.0) ; python_version < "3.8"
 
 # TheLogger
 
 Easy logging, timing and email notifications of code execution.
 
 ### Installation
```

## Comparing `thelogger-0.3.1.dist-info/RECORD` & `thelogger-0.3.2.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-thelogger/__init__.py,sha256=U3tUK5KxRlqkApfmoLuUDPs9_vLFuPWjFt5FTymkaCU,297
-thelogger/_ver.py,sha256=v27jnS60TKa54IbFVzSTknhDiKMS4J3KCuFTOffZqRU,214
+thelogger/__init__.py,sha256=dhhY16P4WEGhomsCWhVx3MWMdQBnHbydtr8V3vVC-ZE,486
+thelogger/__logger.py,sha256=JTyQbecMYpi1n7zKoVe9sohS6tTy87Bx2UnCDHb4-N4,4234
+thelogger/__ver.py,sha256=v27jnS60TKa54IbFVzSTknhDiKMS4J3KCuFTOffZqRU,214
 thelogger/dirty_timer.py,sha256=NxlxGSQ09Q3BRRKYlIRgFahGFgvAn78a9xb-xrNKkXc,1049
-thelogger/logger.py,sha256=JTyQbecMYpi1n7zKoVe9sohS6tTy87Bx2UnCDHb4-N4,4234
+thelogger/sys_meta.py,sha256=cTQdtPRjdO_eI467rXKAEHNGA9eJmQHMR3CKzjU4z10,3352
 thelogger/notify/__init__.py,sha256=X0cVRenLKIbnOoapwPN9KJvtwXaHycKVb-ZTZ8tmuWQ,140
 thelogger/notify/decorator.py,sha256=kiiVpcCayMsdtGtiOtswHaa_v8OzSQjXnKnoSvrt0Uk,3611
 thelogger/notify/exec_func.py,sha256=uN4mbHtdmG4-djWnEzomVeFfbOJ6jHqlNmydolX5QwU,6990
-thelogger-0.3.1.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
-thelogger-0.3.1.dist-info/METADATA,sha256=8q_eMh-PN56d3sp7CPNklaRqzxkPzelCJDC8gkbsUKM,6627
-thelogger-0.3.1.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
-thelogger-0.3.1.dist-info/top_level.txt,sha256=6qGJ7TaRPKJuypP1ToyTCDT03pcvwWZ-vqDreYaUfjQ,10
-thelogger-0.3.1.dist-info/RECORD,,
+thelogger-0.3.2.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
+thelogger-0.3.2.dist-info/METADATA,sha256=7jayG_d7hntPotxpLtm_yhYVPglY-UABiiapQdJUgqo,6692
+thelogger-0.3.2.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
+thelogger-0.3.2.dist-info/top_level.txt,sha256=6qGJ7TaRPKJuypP1ToyTCDT03pcvwWZ-vqDreYaUfjQ,10
+thelogger-0.3.2.dist-info/RECORD,,
```

