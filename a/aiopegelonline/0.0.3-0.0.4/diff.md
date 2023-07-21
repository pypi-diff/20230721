# Comparing `tmp/aiopegelonline-0.0.3-py3-none-any.whl.zip` & `tmp/aiopegelonline-0.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 7892 bytes, number of entries: 10
--rw-r--r--  2.0 unx     4276 b- defN 23-Jul-21 18:56 aiopegelonline/__init__.py
--rw-r--r--  2.0 unx      300 b- defN 23-Jul-21 18:56 aiopegelonline/const.py
--rw-r--r--  2.0 unx      434 b- defN 23-Jul-21 18:56 aiopegelonline/exceptions.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-21 18:56 aiopegelonline/py.typed
--rw-r--r--  2.0 unx    11357 b- defN 23-Jul-21 18:56 aiopegelonline-0.0.3.dist-info/LICENSE
--rw-r--r--  2.0 unx      771 b- defN 23-Jul-21 18:56 aiopegelonline-0.0.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-21 18:56 aiopegelonline-0.0.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       15 b- defN 23-Jul-21 18:56 aiopegelonline-0.0.3.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Jul-21 18:56 aiopegelonline-0.0.3.dist-info/zip-safe
--rw-rw-r--  2.0 unx      837 b- defN 23-Jul-21 18:56 aiopegelonline-0.0.3.dist-info/RECORD
-10 files, 18083 bytes uncompressed, 6444 bytes compressed:  64.4%
+Zip file size: 8465 bytes, number of entries: 10
+-rw-r--r--  2.0 unx     4155 b- defN 23-Jul-21 20:24 aiopegelonline/__init__.py
+-rw-r--r--  2.0 unx      300 b- defN 23-Jul-21 20:24 aiopegelonline/const.py
+-rw-r--r--  2.0 unx      434 b- defN 23-Jul-21 20:24 aiopegelonline/exceptions.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-21 20:24 aiopegelonline/py.typed
+-rw-r--r--  2.0 unx    11357 b- defN 23-Jul-21 20:24 aiopegelonline-0.0.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2566 b- defN 23-Jul-21 20:24 aiopegelonline-0.0.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-21 20:24 aiopegelonline-0.0.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       15 b- defN 23-Jul-21 20:24 aiopegelonline-0.0.4.dist-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Jul-21 20:24 aiopegelonline-0.0.4.dist-info/zip-safe
+-rw-rw-r--  2.0 unx      838 b- defN 23-Jul-21 20:24 aiopegelonline-0.0.4.dist-info/RECORD
+10 files, 19758 bytes uncompressed, 7017 bytes compressed:  64.5%
```

## zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: aiopegelonline/exceptions.py
 Comment: 
 
 Filename: aiopegelonline/py.typed
 Comment: 
 
-Filename: aiopegelonline-0.0.3.dist-info/LICENSE
+Filename: aiopegelonline-0.0.4.dist-info/LICENSE
 Comment: 
 
-Filename: aiopegelonline-0.0.3.dist-info/METADATA
+Filename: aiopegelonline-0.0.4.dist-info/METADATA
 Comment: 
 
-Filename: aiopegelonline-0.0.3.dist-info/WHEEL
+Filename: aiopegelonline-0.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: aiopegelonline-0.0.3.dist-info/top_level.txt
+Filename: aiopegelonline-0.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: aiopegelonline-0.0.3.dist-info/zip-safe
+Filename: aiopegelonline-0.0.4.dist-info/zip-safe
 Comment: 
 
-Filename: aiopegelonline-0.0.3.dist-info/RECORD
+Filename: aiopegelonline-0.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## aiopegelonline/__init__.py

```diff
@@ -121,21 +121,18 @@
             station.get("longitude"),
             station.get("latitude"),
             station["water"]["longname"],
         )
 
     async def async_get_station_measurement(self, uuid: str) -> CurrentMeasurement:
         """Get current measurement of a station."""
-        station = await self._async_do_request(
-            f"{BASE_URL}/stations/{uuid}.json",
+        measurement = await self._async_do_request(
+            f"{BASE_URL}/stations/{uuid}/W.json",
             {
                 "prettyprint": "false",
-                "includeTimeseries": "true",
                 "includeCurrentMeasurement": "true",
-                "timeseries": "W",
             },
         )
 
-        measurement = station["timeseries"][0]
         return CurrentMeasurement(
             measurement["unit"], measurement["currentMeasurement"]["value"]
         )
```

## Comparing `aiopegelonline-0.0.3.dist-info/LICENSE` & `aiopegelonline-0.0.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `aiopegelonline-0.0.3.dist-info/RECORD` & `aiopegelonline-0.0.4.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-aiopegelonline/__init__.py,sha256=Ur4d0SsYRDj9wH4Mi1Ujanso-MbZNJJnhxA8QMwhO9k,4276
+aiopegelonline/__init__.py,sha256=A8LoxD0pJt2UAErvU0Sy1UpX8yEMQ0Tel4--YD65hDU,4155
 aiopegelonline/const.py,sha256=_OYsBFes9WqOUF93JsSMpwiXxVPJ2AxUsUbKh8ypzYw,300
 aiopegelonline/exceptions.py,sha256=K7TOHttF36zhu3zLThA3FOfnrgrbQUpECTk4rgJpn94,434
 aiopegelonline/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-aiopegelonline-0.0.3.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-aiopegelonline-0.0.3.dist-info/METADATA,sha256=l1-dtz4P5z_A9k2ZZNyP1rGZ-Fyj3eLtH875teks7HE,771
-aiopegelonline-0.0.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-aiopegelonline-0.0.3.dist-info/top_level.txt,sha256=vxcBtWrluLbvB3sff65v0Oh2kghBcTXJGMacsV35BNE,15
-aiopegelonline-0.0.3.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-aiopegelonline-0.0.3.dist-info/RECORD,,
+aiopegelonline-0.0.4.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+aiopegelonline-0.0.4.dist-info/METADATA,sha256=2dom-qAV2OaS12zRNMeb6jzwdiLgoGd57R2milf1Syg,2566
+aiopegelonline-0.0.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+aiopegelonline-0.0.4.dist-info/top_level.txt,sha256=vxcBtWrluLbvB3sff65v0Oh2kghBcTXJGMacsV35BNE,15
+aiopegelonline-0.0.4.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+aiopegelonline-0.0.4.dist-info/RECORD,,
```

