# Comparing `tmp/wiretap_sqlserver-4.2.0-py3-none-any.whl.zip` & `tmp/wiretap_sqlserver-5.0.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 2985 bytes, number of entries: 7
+Zip file size: 3033 bytes, number of entries: 7
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jan-27 19:36 __init__.py
 -rw-rw-rw-  2.0 fat       96 b- defN 23-Jan-27 19:49 wiretap_sqlserver/__init__.py
--rw-rw-rw-  2.0 fat     3446 b- defN 23-May-13 16:15 wiretap_sqlserver/sqlserverhandler.py
--rw-rw-rw-  2.0 fat      189 b- defN 23-May-13 16:16 wiretap_sqlserver-4.2.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-13 16:16 wiretap_sqlserver-4.2.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       27 b- defN 23-May-13 16:16 wiretap_sqlserver-4.2.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      580 b- defN 23-May-13 16:16 wiretap_sqlserver-4.2.0.dist-info/RECORD
-7 files, 4430 bytes uncompressed, 1941 bytes compressed:  56.2%
+-rw-rw-rw-  2.0 fat     3646 b- defN 23-Jul-20 19:55 wiretap_sqlserver/sqlserverhandler.py
+-rw-rw-rw-  2.0 fat      189 b- defN 23-Jul-21 12:41 wiretap_sqlserver-5.0.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-21 12:41 wiretap_sqlserver-5.0.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       27 b- defN 23-Jul-21 12:41 wiretap_sqlserver-5.0.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      580 b- defN 23-Jul-21 12:41 wiretap_sqlserver-5.0.0.dist-info/RECORD
+7 files, 4630 bytes uncompressed, 1989 bytes compressed:  57.0%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: wiretap_sqlserver/__init__.py
 Comment: 
 
 Filename: wiretap_sqlserver/sqlserverhandler.py
 Comment: 
 
-Filename: wiretap_sqlserver-4.2.0.dist-info/METADATA
+Filename: wiretap_sqlserver-5.0.0.dist-info/METADATA
 Comment: 
 
-Filename: wiretap_sqlserver-4.2.0.dist-info/WHEEL
+Filename: wiretap_sqlserver-5.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: wiretap_sqlserver-4.2.0.dist-info/top_level.txt
+Filename: wiretap_sqlserver-5.0.0.dist-info/top_level.txt
 Comment: 
 
-Filename: wiretap_sqlserver-4.2.0.dist-info/RECORD
+Filename: wiretap_sqlserver-5.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## wiretap_sqlserver/sqlserverhandler.py

```diff
@@ -5,15 +5,15 @@
 from datetime import datetime, timezone
 from logging import Handler
 from typing import Any, Dict, Protocol, runtime_checkable, cast
 
 import sqlalchemy  # type: ignore
 
 DEFAULT_INSERT = """
-INSERT INTO wiretap_log(
+INSERT INTO dev.wiretap_log(
     [parent], 
     [node], 
     [timestamp], 
     [scope], 
     [status], 
     [level], 
     [elapsed], 
@@ -73,27 +73,32 @@
                 "parent": recext.parent.__str__() if recext.parent else None,
                 "node": recext.node.__str__(),
                 "status": recext.status.lower(),
                 "elapsed": recext.elapsed,
                 "details": recext.details,
                 "attachment": recext.attachment
             }
+
+            if record.exc_text:
+                params["attachment"] = params["attachment"] + "\n\n" + record.exc_text if params["attachment"] else record.exc_text
+
         else:
             params = params | {
                 "parent": None,
                 "node": None,
                 "status": None,
                 "elapsed": None,
                 "details": None,
                 "attachment": None
             }
 
         try:
             with self.engine.connect() as c:
-                c.execute(self.insert, **params)
+                c.execute(self.insert, params)
+                c.commit()
         except:  # noqa
             # Disable this handler if an error occurs.
             self.setLevel(sys.maxsize)
             logging.exception(msg=f"Handler '{self.name}' could not log and has been disabled.", exc_info=True)
 
     def _cleanup(self):
         self.engine.dispose(close=True)
```

## Comparing `wiretap_sqlserver-4.2.0.dist-info/RECORD` & `wiretap_sqlserver-5.0.0.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 __init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 wiretap_sqlserver/__init__.py,sha256=nqZUltBgZ_SflgaKeWApt-luGYUdKWlcrpvPtVwIzP4,96
-wiretap_sqlserver/sqlserverhandler.py,sha256=m1qRwyrEiaUHBkRZQqHCB1ZrMS9bjEZ_4_rIeB1niYA,3446
-wiretap_sqlserver-4.2.0.dist-info/METADATA,sha256=WupoCUc0tRMLd-SRPaYQ0-5GUjQMuBZ9rholtqJ97s0,189
-wiretap_sqlserver-4.2.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-wiretap_sqlserver-4.2.0.dist-info/top_level.txt,sha256=ulA0TtAkY_FcwFu1cRdD0O4EblYR4uY30Y7sTpw7cVI,27
-wiretap_sqlserver-4.2.0.dist-info/RECORD,,
+wiretap_sqlserver/sqlserverhandler.py,sha256=_wB5cWANzjaYFxwFJ00kDwuK0ePuyNrc4U2i2mHkQNo,3646
+wiretap_sqlserver-5.0.0.dist-info/METADATA,sha256=YRCdQzLvixi8kXDeYQlte-chmHiySxLYMPU6CLFMD1U,189
+wiretap_sqlserver-5.0.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+wiretap_sqlserver-5.0.0.dist-info/top_level.txt,sha256=ulA0TtAkY_FcwFu1cRdD0O4EblYR4uY30Y7sTpw7cVI,27
+wiretap_sqlserver-5.0.0.dist-info/RECORD,,
```

