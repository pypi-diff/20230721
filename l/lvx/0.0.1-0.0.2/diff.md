# Comparing `tmp/lvx-0.0.1-py3-none-any.whl.zip` & `tmp/lvx-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,24 +1,25 @@
-Zip file size: 129214 bytes, number of entries: 22
+Zip file size: 131497 bytes, number of entries: 23
 -rw-rw-rw-  2.0 fat    61050 b- defN 23-Jul-21 11:50 lvx/__init__.py
 -rw-rw-rw-  2.0 fat     3603 b- defN 23-Jul-21 11:49 lvx/__version__.py
 -rw-rw-rw-  2.0 fat    16498 b- defN 23-Jul-21 11:49 lvx/_internal_utils.py
 -rw-rw-rw-  2.0 fat   189340 b- defN 23-Jul-21 11:50 lvx/adapters.py
+-rw-rw-rw-  2.0 fat    48862 b- defN 23-Jul-21 12:31 lvx/api.py
 -rw-rw-rw-  2.0 fat   121327 b- defN 23-Jul-21 11:50 lvx/auth.py
 -rw-rw-rw-  2.0 fat     4621 b- defN 23-Jul-21 11:50 lvx/certs.py
 -rw-rw-rw-  2.0 fat    24076 b- defN 23-Jul-21 11:50 lvx/compat.py
 -rw-rw-rw-  2.0 fat   210407 b- defN 23-Jul-21 11:50 lvx/cookies.py
 -rw-rw-rw-  2.0 fat    57454 b- defN 23-Jul-21 11:50 lvx/exceptions.py
 -rw-rw-rw-  2.0 fat    44924 b- defN 23-Jul-21 11:50 lvx/help.py
 -rw-rw-rw-  2.0 fat    10383 b- defN 23-Jul-21 11:49 lvx/hooks.py
 -rw-rw-rw-  2.0 fat   364872 b- defN 23-Jul-21 11:50 lvx/models.py
 -rw-rw-rw-  2.0 fat     9801 b- defN 23-Jul-21 11:49 lvx/packages.py
 -rw-rw-rw-  2.0 fat   284646 b- defN 23-Jul-21 11:50 lvx/sessions.py
 -rw-rw-rw-  2.0 fat    46021 b- defN 23-Jul-21 11:50 lvx/status_codes.py
 -rw-rw-rw-  2.0 fat    40215 b- defN 23-Jul-21 11:50 lvx/structures.py
 -rw-rw-rw-  2.0 fat   384190 b- defN 23-Jul-21 11:50 lvx/utils.py
--rw-rw-rw-  2.0 fat     1091 b- defN 23-Jul-21 12:01 lvx-0.0.1.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat      412 b- defN 23-Jul-21 12:01 lvx-0.0.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-21 12:01 lvx-0.0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        4 b- defN 23-Jul-21 12:01 lvx-0.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1608 b- defN 23-Jul-21 12:01 lvx-0.0.1.dist-info/RECORD
-22 files, 1876635 bytes uncompressed, 126732 bytes compressed:  93.2%
+-rw-rw-rw-  2.0 fat     1091 b- defN 23-Jul-21 12:34 lvx-0.0.2.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat      412 b- defN 23-Jul-21 12:34 lvx-0.0.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-21 12:34 lvx-0.0.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        4 b- defN 23-Jul-21 12:34 lvx-0.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1676 b- defN 23-Jul-21 12:34 lvx-0.0.2.dist-info/RECORD
+23 files, 1925565 bytes uncompressed, 128919 bytes compressed:  93.3%
```

## zipnote {}

```diff
@@ -6,14 +6,17 @@
 
 Filename: lvx/_internal_utils.py
 Comment: 
 
 Filename: lvx/adapters.py
 Comment: 
 
+Filename: lvx/api.py
+Comment: 
+
 Filename: lvx/auth.py
 Comment: 
 
 Filename: lvx/certs.py
 Comment: 
 
 Filename: lvx/compat.py
@@ -45,23 +48,23 @@
 
 Filename: lvx/structures.py
 Comment: 
 
 Filename: lvx/utils.py
 Comment: 
 
-Filename: lvx-0.0.1.dist-info/LICENSE.txt
+Filename: lvx-0.0.2.dist-info/LICENSE.txt
 Comment: 
 
-Filename: lvx-0.0.1.dist-info/METADATA
+Filename: lvx-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: lvx-0.0.1.dist-info/WHEEL
+Filename: lvx-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: lvx-0.0.1.dist-info/top_level.txt
+Filename: lvx-0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: lvx-0.0.1.dist-info/RECORD
+Filename: lvx-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `lvx-0.0.1.dist-info/LICENSE.txt` & `lvx-0.0.2.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `lvx-0.0.1.dist-info/RECORD` & `lvx-0.0.2.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 lvx/__init__.py,sha256=4PT85uROyKuIqHqygh9yaCuzJij0LKiKJx3HP39faVk,61050
 lvx/__version__.py,sha256=2DMhdyHWjx4d2PbIcoXI5FOXg3Iu6dWY2FxM17loi4Y,3603
 lvx/_internal_utils.py,sha256=GUwZhXXnnOihmrRCgAd9KxVntSelQE14N2F-IO8XKFk,16498
 lvx/adapters.py,sha256=Z7d6qNsbYOijhLAw5rAW5tdUJkg80PZ7IVJdORPANbg,189340
+lvx/api.py,sha256=S-tWMgqel4mndiWlppecuSgB7ckPWnrDAgHKnPVuZR0,48862
 lvx/auth.py,sha256=8X1AI5i5xlPJWfitGRONf_Do19bdt9gVTnAB243_vqo,121327
 lvx/certs.py,sha256=ZT_D_PZkB7o4PKlcz1vZNtnQdvgfV7ZMWwQjCVWG9W8,4621
 lvx/compat.py,sha256=TLflUqlJahUZ4MpPenHZXzsS2aD32mNEyzFOi86PAQs,24076
 lvx/cookies.py,sha256=NrXhpFXotwbreSq488hU3ZwQLGRktUgFDxBZlJPjqV0,210407
 lvx/exceptions.py,sha256=Vin9Fp2-RukhDGKnUP-Fdfukf6Hzp5tPXNW3kCg2tLo,57454
 lvx/help.py,sha256=VzPEaH8foT1YSu8gXskpXqvgdQwIdCGP37FXmM0ZmEA,44924
 lvx/hooks.py,sha256=wknUUrXi_SjX0ZP26T2Okttn72Bv0VEllf68qYmCjxU,10383
 lvx/models.py,sha256=iQbbNl_oKcgFYA0uY_otKkE7guqlmOub6sGFjMIZCbg,364872
 lvx/packages.py,sha256=NRpg_SV0FnHPMFXVH_z-y5Zb-wE8s9wxSOnYEEuRKUk,9801
 lvx/sessions.py,sha256=fmdD2cFprI52jr-2N3fI4j-PP9x16QGGEAYkJB7S2Co,284646
 lvx/status_codes.py,sha256=qpmQ6djzsuRn0THWIGm4zp3rYeumggW3XHUkr8ABUGA,46021
 lvx/structures.py,sha256=RiVsFUD5l6hHmFAPhbN9aFDRfhPWST2M8G6ole2M2K4,40215
 lvx/utils.py,sha256=AlAHRPbiAKqShk-hqjDMpPdx4mui_NAVpTj9mywGwQs,384190
-lvx-0.0.1.dist-info/LICENSE.txt,sha256=6kbiFSfobTZ7beWiKnHpN902HgBx-Jzgcme0SvKqhKY,1091
-lvx-0.0.1.dist-info/METADATA,sha256=PFmFK7HpDTaHsI_AZDYt2Vnpb6SIs1hbN8b0P43cark,412
-lvx-0.0.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-lvx-0.0.1.dist-info/top_level.txt,sha256=Dr3bapc6_zXWB4UV0f9beo7NFMfnf1ogLelrj5MCpdg,4
-lvx-0.0.1.dist-info/RECORD,,
+lvx-0.0.2.dist-info/LICENSE.txt,sha256=6kbiFSfobTZ7beWiKnHpN902HgBx-Jzgcme0SvKqhKY,1091
+lvx-0.0.2.dist-info/METADATA,sha256=1wRCmTFApAkyWU4q1XGDtQ39SXc93R7ep0Y1rOtiRnM,412
+lvx-0.0.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+lvx-0.0.2.dist-info/top_level.txt,sha256=Dr3bapc6_zXWB4UV0f9beo7NFMfnf1ogLelrj5MCpdg,4
+lvx-0.0.2.dist-info/RECORD,,
```

