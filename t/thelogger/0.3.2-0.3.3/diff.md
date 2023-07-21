# Comparing `tmp/thelogger-0.3.2-py3-none-any.whl.zip` & `tmp/thelogger-0.3.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 15243 bytes, number of entries: 13
+Zip file size: 15593 bytes, number of entries: 13
 -rw-rw-rw-  2.0 fat      486 b- defN 23-Jul-21 04:09 thelogger/__init__.py
 -rw-rw-rw-  2.0 fat     4234 b- defN 22-Feb-20 09:05 thelogger/__logger.py
 -rw-rw-rw-  2.0 fat      214 b- defN 23-Apr-27 17:46 thelogger/__ver.py
 -rw-rw-rw-  2.0 fat     1049 b- defN 23-Jun-17 05:10 thelogger/dirty_timer.py
--rw-rw-rw-  2.0 fat     3352 b- defN 23-Jul-21 04:17 thelogger/sys_meta.py
+-rw-rw-rw-  2.0 fat     4406 b- defN 23-Jul-21 20:00 thelogger/sys_meta.py
 -rw-rw-rw-  2.0 fat      140 b- defN 22-Feb-20 09:05 thelogger/notify/__init__.py
 -rw-rw-rw-  2.0 fat     3611 b- defN 22-Feb-20 09:49 thelogger/notify/decorator.py
 -rw-rw-rw-  2.0 fat     6990 b- defN 23-Feb-28 14:35 thelogger/notify/exec_func.py
--rw-rw-rw-  2.0 fat    11558 b- defN 23-Jul-21 04:19 thelogger-0.3.2.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     6692 b- defN 23-Jul-21 04:19 thelogger-0.3.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-21 04:19 thelogger-0.3.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       10 b- defN 23-Jul-21 04:19 thelogger-0.3.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1041 b- defN 23-Jul-21 04:19 thelogger-0.3.2.dist-info/RECORD
-13 files, 39469 bytes uncompressed, 13513 bytes compressed:  65.8%
+-rw-rw-rw-  2.0 fat    11558 b- defN 23-Jul-21 20:01 thelogger-0.3.3.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     6692 b- defN 23-Jul-21 20:01 thelogger-0.3.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-21 20:01 thelogger-0.3.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       10 b- defN 23-Jul-21 20:01 thelogger-0.3.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1041 b- defN 23-Jul-21 20:01 thelogger-0.3.3.dist-info/RECORD
+13 files, 40523 bytes uncompressed, 13863 bytes compressed:  65.8%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: thelogger/notify/decorator.py
 Comment: 
 
 Filename: thelogger/notify/exec_func.py
 Comment: 
 
-Filename: thelogger-0.3.2.dist-info/LICENSE
+Filename: thelogger-0.3.3.dist-info/LICENSE
 Comment: 
 
-Filename: thelogger-0.3.2.dist-info/METADATA
+Filename: thelogger-0.3.3.dist-info/METADATA
 Comment: 
 
-Filename: thelogger-0.3.2.dist-info/WHEEL
+Filename: thelogger-0.3.3.dist-info/WHEEL
 Comment: 
 
-Filename: thelogger-0.3.2.dist-info/top_level.txt
+Filename: thelogger-0.3.3.dist-info/top_level.txt
 Comment: 
 
-Filename: thelogger-0.3.2.dist-info/RECORD
+Filename: thelogger-0.3.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## thelogger/sys_meta.py

```diff
@@ -1,14 +1,15 @@
 import sys
 import pytz
 import socket
 import psutil 
 import datetime
 import platform
 import subprocess
+import pandas as pd
 from tzlocal import get_localzone
 from importlib.metadata import version
 
 def get_cpu_model():
     if platform.system() == 'Windows':
         try:
             command = 'wmic cpu get name /value'
@@ -55,30 +56,52 @@
     usage = dict(
         cpu_used = str(cpu_used) + '%',
         memory_used = str(memory_used)  + '%',
         datetime = dttm
         )
     return usage
 
+def try_version(x):
+    try:
+        ver = version(x)
+    except:
+        ver = '?'# std libs don't have versions
+    return ver
+
+def get_imported_package_versions():
+    # excludes std libs
+    package_names = set()
+    for module_name, module in sys.modules.items():
+        if (module and hasattr(module, '__package__') and module.__package__
+        and module_name[0] != '_'):
+            package_names.add(module.__package__)
+    imp_mod = pd.Series(list(package_names), name = 'pkgs')
+    imp_mod = imp_mod.str.split('.').str[0]
+    imp_mod = imp_mod.drop_duplicates()
+    imp_mod = pd.DataFrame(imp_mod)
+    imp_mod['version'] = imp_mod.pkgs.apply(lambda x: try_version(x))
+    imp_mod = imp_mod.loc[imp_mod.version != '?'].sort_values('pkgs')\
+        .reset_index(drop=True)
+    return imp_mod
+
 def get_env_info(pkgs = None):
     py_ver = ".".join(str(component) for component in sys.version_info[:3])
-    
-    pkg_ver = dict()
     pkgs = [pkgs] if type(pkgs) == str else pkgs
-    pkgs = pkgs if pkgs else list()
-    for pkg in pkgs:
-        pkg_ver[pkg] = version(pkg)
-        
+    imported_pkgs = get_imported_package_versions()
+    if pkgs:
+        imported_pkgs = imported_pkgs.loc[imported_pkgs.pkgs.isin(pkgs)] 
+    imported_pkgs = imported_pkgs.sort_values('pkgs')
+    pkg_ver = dict(zip(imported_pkgs.pkgs, imported_pkgs.version))
     env_info = dict(python_version = py_ver,
                     python_path = sys.executable,
                     package_versions = pkg_ver)
-    
     return env_info
         
 def sys_info(pkgs = None, tz = 'America/New_York'):
+    # pkgs: str or list to filter for only specific pkgs. pkg must be imported
     machine_info = get_machine_info()
     usage = get_resource_usage(tz)
     env_info = get_env_info(pkgs)
     out = dict(
         system_name = machine_info['machine_name'],
         system_timezone = machine_info['machine_timezone'],
         datetime = usage['datetime'],
```

## Comparing `thelogger-0.3.2.dist-info/LICENSE` & `thelogger-0.3.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `thelogger-0.3.2.dist-info/METADATA` & `thelogger-0.3.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thelogger
-Version: 0.3.2
+Version: 0.3.3
 Summary: Easy logging, timing and email notifications of code execution.
 Home-page: https://github.com/tom1919/TheLogger
 Author: Tom1919
 Author-email: py.notify1@gmail.com
 License: Apache 2.0
 Keywords: log,logging,logger,email,timimg,notification
 Platform: UNKNOWN
```

## Comparing `thelogger-0.3.2.dist-info/RECORD` & `thelogger-0.3.3.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 thelogger/__init__.py,sha256=dhhY16P4WEGhomsCWhVx3MWMdQBnHbydtr8V3vVC-ZE,486
 thelogger/__logger.py,sha256=JTyQbecMYpi1n7zKoVe9sohS6tTy87Bx2UnCDHb4-N4,4234
 thelogger/__ver.py,sha256=v27jnS60TKa54IbFVzSTknhDiKMS4J3KCuFTOffZqRU,214
 thelogger/dirty_timer.py,sha256=NxlxGSQ09Q3BRRKYlIRgFahGFgvAn78a9xb-xrNKkXc,1049
-thelogger/sys_meta.py,sha256=cTQdtPRjdO_eI467rXKAEHNGA9eJmQHMR3CKzjU4z10,3352
+thelogger/sys_meta.py,sha256=FihAGy_9Hfn7abX5tXnCne45o8Ei5jiUWyg-vvHjsbg,4406
 thelogger/notify/__init__.py,sha256=X0cVRenLKIbnOoapwPN9KJvtwXaHycKVb-ZTZ8tmuWQ,140
 thelogger/notify/decorator.py,sha256=kiiVpcCayMsdtGtiOtswHaa_v8OzSQjXnKnoSvrt0Uk,3611
 thelogger/notify/exec_func.py,sha256=uN4mbHtdmG4-djWnEzomVeFfbOJ6jHqlNmydolX5QwU,6990
-thelogger-0.3.2.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
-thelogger-0.3.2.dist-info/METADATA,sha256=7jayG_d7hntPotxpLtm_yhYVPglY-UABiiapQdJUgqo,6692
-thelogger-0.3.2.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
-thelogger-0.3.2.dist-info/top_level.txt,sha256=6qGJ7TaRPKJuypP1ToyTCDT03pcvwWZ-vqDreYaUfjQ,10
-thelogger-0.3.2.dist-info/RECORD,,
+thelogger-0.3.3.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
+thelogger-0.3.3.dist-info/METADATA,sha256=1SGIefTDy1JbAHKDK1ndwor_OZOzC-GHcKfpI-TgngQ,6692
+thelogger-0.3.3.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
+thelogger-0.3.3.dist-info/top_level.txt,sha256=6qGJ7TaRPKJuypP1ToyTCDT03pcvwWZ-vqDreYaUfjQ,10
+thelogger-0.3.3.dist-info/RECORD,,
```

