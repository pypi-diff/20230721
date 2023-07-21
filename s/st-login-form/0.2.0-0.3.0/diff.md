# Comparing `tmp/st-login-form-0.2.0.tar.gz` & `tmp/st-login-form-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "st-login-form-0.2.0.tar", last modified: Sat Jul 15 17:04:19 2023, max compression
+gzip compressed data, was "st-login-form-0.3.0.tar", last modified: Fri Jul 21 15:56:51 2023, max compression
```

## Comparing `st-login-form-0.2.0.tar` & `st-login-form-0.3.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 17:04:19.317008 st-login-form-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-07-15 17:04:03.000000 st-login-form-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-15 17:04:03.000000 st-login-form-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-07-15 17:04:19.317008 st-login-form-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-07-15 17:04:03.000000 st-login-form-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 17:04:19.317008 st-login-form-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-07-15 17:04:03.000000 st-login-form-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 17:04:19.317008 st-login-form-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 17:04:19.317008 st-login-form-0.2.0/src/st_login_form/
--rw-r--r--   0 runner    (1001) docker     (123)     6423 2023-07-15 17:04:03.000000 st-login-form-0.2.0/src/st_login_form/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 17:04:19.317008 st-login-form-0.2.0/src/st_login_form.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-07-15 17:04:19.000000 st-login-form-0.2.0/src/st_login_form.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-15 17:04:19.000000 st-login-form-0.2.0/src/st_login_form.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 17:04:19.000000 st-login-form-0.2.0/src/st_login_form.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-15 17:04:19.000000 st-login-form-0.2.0/src/st_login_form.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-15 17:04:19.000000 st-login-form-0.2.0/src/st_login_form.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:56:51.754086 st-login-form-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-07-21 15:56:42.000000 st-login-form-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-21 15:56:42.000000 st-login-form-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3967 2023-07-21 15:56:51.754086 st-login-form-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-07-21 15:56:42.000000 st-login-form-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 15:56:51.754086 st-login-form-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-21 15:56:42.000000 st-login-form-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:56:51.750085 st-login-form-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:56:51.750085 st-login-form-0.3.0/src/st_login_form/
+-rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-07-21 15:56:42.000000 st-login-form-0.3.0/src/st_login_form/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:56:51.754086 st-login-form-0.3.0/src/st_login_form.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3967 2023-07-21 15:56:51.000000 st-login-form-0.3.0/src/st_login_form.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-21 15:56:51.000000 st-login-form-0.3.0/src/st_login_form.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 15:56:51.000000 st-login-form-0.3.0/src/st_login_form.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-21 15:56:51.000000 st-login-form-0.3.0/src/st_login_form.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-21 15:56:51.000000 st-login-form-0.3.0/src/st_login_form.egg-info/top_level.txt
```

### Comparing `st-login-form-0.2.0/LICENSE` & `st-login-form-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `st-login-form-0.2.0/PKG-INFO` & `st-login-form-0.3.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,198 +1,183 @@
-00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
-00000010: 3a20 322e 310a 4e61 6d65 3a20 7374 2d6c  : 2.1.Name: st-l
-00000020: 6f67 696e 2d66 6f72 6d0a 5665 7273 696f  ogin-form.Versio
-00000030: 6e3a 2030 2e32 2e30 0a53 756d 6d61 7279  n: 0.2.0.Summary
-00000040: 3a20 4120 7374 7265 616d 6c69 7420 636f  : A streamlit co
-00000050: 6d70 6f6e 656e 7420 7468 6174 2063 7265  mponent that cre
-00000060: 6174 6573 2061 2075 7365 7220 6c6f 6769  ates a user logi
-00000070: 6e20 666f 726d 2063 6f6e 6e65 6374 6564  n form connected
-00000080: 2074 6f20 6120 5375 7061 6261 7365 2044   to a Supabase D
-00000090: 422e 2049 7420 6c65 7473 2075 7365 7273  B. It lets users
-000000a0: 2063 7265 6174 6520 6120 6e65 7720 7573   create a new us
-000000b0: 6572 6e61 6d65 2061 6e64 2070 6173 7377  ername and passw
-000000c0: 6f72 642c 206c 6f67 696e 2074 6f20 616e  ord, login to an
-000000d0: 2065 7869 7374 696e 6720 6163 636f 756e   existing accoun
-000000e0: 742c 206f 7220 6c6f 6769 6e20 6173 2061  t, or login as a
-000000f0: 6e20 616e 6f6e 796d 6f75 7320 6775 6573  n anonymous gues
-00000100: 742e 0a41 7574 686f 723a 2053 6964 6468  t..Author: Siddh
-00000110: 616e 7420 5361 6461 6e67 690a 4175 7468  ant Sadangi.Auth
-00000120: 6f72 2d65 6d61 696c 3a20 7369 6464 6861  or-email: siddha
-00000130: 6e74 2e73 6164 616e 6769 4067 6d61 696c  nt.sadangi@gmail
-00000140: 2e63 6f6d 0a4b 6579 776f 7264 733a 2073  .com.Keywords: s
-00000150: 7472 6561 6d6c 6974 2c6c 6f67 696e 0a43  treamlit,login.C
-00000160: 6c61 7373 6966 6965 723a 2045 6e76 6972  lassifier: Envir
-00000170: 6f6e 6d65 6e74 203a 3a20 506c 7567 696e  onment :: Plugin
-00000180: 730a 436c 6173 7369 6669 6572 3a20 496e  s.Classifier: In
-00000190: 7465 6e64 6564 2041 7564 6965 6e63 6520  tended Audience 
-000001a0: 3a3a 2044 6576 656c 6f70 6572 730a 436c  :: Developers.Cl
-000001b0: 6173 7369 6669 6572 3a20 4c69 6365 6e73  assifier: Licens
-000001c0: 6520 3a3a 204f 5349 2041 7070 726f 7665  e :: OSI Approve
-000001d0: 6420 3a3a 2047 4e55 2047 656e 6572 616c  d :: GNU General
-000001e0: 2050 7562 6c69 6320 4c69 6365 6e73 6520   Public License 
-000001f0: 7633 2028 4750 4c76 3329 0a43 6c61 7373  v3 (GPLv3).Class
-00000200: 6966 6965 723a 204f 7065 7261 7469 6e67  ifier: Operating
-00000210: 2053 7973 7465 6d20 3a3a 204f 5320 496e   System :: OS In
-00000220: 6465 7065 6e64 656e 740a 436c 6173 7369  dependent.Classi
-00000230: 6669 6572 3a20 5072 6f67 7261 6d6d 696e  fier: Programmin
-00000240: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-00000250: 7468 6f6e 0a43 6c61 7373 6966 6965 723a  thon.Classifier:
-00000260: 2054 6f70 6963 203a 3a20 536f 6674 7761   Topic :: Softwa
-00000270: 7265 2044 6576 656c 6f70 6d65 6e74 203a  re Development :
-00000280: 3a20 4c69 6272 6172 6965 7320 3a3a 2050  : Libraries :: P
-00000290: 7974 686f 6e20 4d6f 6475 6c65 730a 436c  ython Modules.Cl
-000002a0: 6173 7369 6669 6572 3a20 546f 7069 6320  assifier: Topic 
-000002b0: 3a3a 2053 6f66 7477 6172 6520 4465 7665  :: Software Deve
-000002c0: 6c6f 706d 656e 7420 3a3a 2055 7365 7220  lopment :: User 
-000002d0: 496e 7465 7266 6163 6573 0a52 6571 7569  Interfaces.Requi
-000002e0: 7265 732d 5079 7468 6f6e 3a20 3e3d 332e  res-Python: >=3.
-000002f0: 380a 4465 7363 7269 7074 696f 6e2d 436f  8.Description-Co
-00000300: 6e74 656e 742d 5479 7065 3a20 7465 7874  ntent-Type: text
-00000310: 2f6d 6172 6b64 6f77 6e0a 4c69 6365 6e73  /markdown.Licens
-00000320: 652d 4669 6c65 3a20 4c49 4345 4e53 450a  e-File: LICENSE.
-00000330: 0a23 203a 6c6f 636b 3a20 7374 2d6c 6f67  .# :lock: st-log
-00000340: 696e 2d66 6f72 6d0a 0a41 2073 7472 6561  in-form..A strea
-00000350: 6d6c 6974 2063 6f6d 706f 6e65 6e74 2074  mlit component t
-00000360: 6861 7420 6372 6561 7465 7320 6120 7573  hat creates a us
-00000370: 6572 206c 6f67 696e 2066 6f72 6d20 636f  er login form co
-00000380: 6e6e 6563 7465 6420 746f 2061 2053 7570  nnected to a Sup
-00000390: 6162 6173 6520 4442 2e20 4974 206c 6574  abase DB. It let
-000003a0: 7320 7573 6572 7320 6372 6561 7465 2061  s users create a
-000003b0: 206e 6577 2075 7365 726e 616d 6520 616e   new username an
-000003c0: 6420 7061 7373 776f 7264 2c20 6c6f 6769  d password, logi
-000003d0: 6e20 746f 2061 6e20 6578 6973 7469 6e67  n to an existing
-000003e0: 2061 6363 6f75 6e74 2c20 6f72 206c 6f67   account, or log
-000003f0: 696e 2061 7320 616e 2061 6e6f 6e79 6d6f  in as an anonymo
-00000400: 7573 2067 7565 7374 2e0a 0a21 5b46 6f72  us guest...![For
-00000410: 6d20 7363 7265 656e 7368 6f74 5d28 6173  m screenshot](as
-00000420: 7365 7473 2f73 6372 6565 6e73 686f 742e  sets/screenshot.
-00000430: 706e 6729 0a0a 5468 6520 6c6f 6769 6e20  png)..The login 
-00000440: 666f 726d 2063 6f6c 6c61 7073 6573 2061  form collapses a
-00000450: 6674 6572 206c 6f67 696e 2074 6f20 6672  fter login to fr
-00000460: 6565 2073 6372 6565 6e2d 7370 6163 652e  ee screen-space.
-00000470: 0a0a 2323 203a 636f 6d70 7574 6572 3a20  ..## :computer: 
-00000480: 4465 6d6f 2061 7070 0a5b 215b 4f70 656e  Demo app.[![Open
-00000490: 2069 6e20 5374 7265 616d 6c69 745d 2868   in Streamlit](h
-000004a0: 7474 7073 3a2f 2f73 7461 7469 632e 7374  ttps://static.st
-000004b0: 7265 616d 6c69 742e 696f 2f62 6164 6765  reamlit.io/badge
-000004c0: 732f 7374 7265 616d 6c69 745f 6261 6467  s/streamlit_badg
-000004d0: 655f 626c 6163 6b5f 7768 6974 652e 7376  e_black_white.sv
-000004e0: 6729 5d28 6874 7470 733a 2f2f 7374 2d6c  g)](https://st-l
-000004f0: 676e 2d66 6f72 6d2e 7374 7265 616d 6c69  gn-form.streamli
-00000500: 742e 6170 702f 290a 0a23 2320 3a63 6f6e  t.app/)..## :con
-00000510: 7374 7275 6374 696f 6e3a 2049 6e73 7461  struction: Insta
-00000520: 6c6c 6174 696f 6e20 0a0a 312e 2049 6e73  llation ..1. Ins
-00000530: 7461 6c6c 2060 7374 2d6c 6f67 696e 2d66  tall `st-login-f
-00000540: 6f72 6d60 200a 6060 6073 680a 7069 7020  orm` .```sh.pip 
-00000550: 696e 7374 616c 6c20 7374 2d6c 6f67 696e  install st-login
-00000560: 2d66 6f72 6d0a 6060 600a 322e 2043 7265  -form.```.2. Cre
-00000570: 6174 6520 6120 5375 7061 6261 7365 2070  ate a Supabase p
-00000580: 726f 6a65 6374 2061 7320 6d65 6e74 696f  roject as mentio
-00000590: 6e65 6420 5b68 6572 655d 2868 7474 7073  ned [here](https
-000005a0: 3a2f 2f64 6f63 732e 7374 7265 616d 6c69  ://docs.streamli
-000005b0: 742e 696f 2f6b 6e6f 776c 6564 6765 2d62  t.io/knowledge-b
-000005c0: 6173 652f 7475 746f 7269 616c 732f 6461  ase/tutorials/da
-000005d0: 7461 6261 7365 732f 7375 7061 6261 7365  tabases/supabase
-000005e0: 2373 6967 6e2d 696e 2d74 6f2d 7375 7061  #sign-in-to-supa
-000005f0: 6261 7365 2d61 6e64 2d63 7265 6174 652d  base-and-create-
-00000600: 612d 7072 6f6a 6563 7429 0a33 2e20 4372  a-project).3. Cr
-00000610: 6561 7465 2061 2074 6162 6c65 2074 6f20  eate a table to 
-00000620: 7374 6f72 6520 7468 6520 7573 6572 6e61  store the userna
-00000630: 6d65 7320 616e 6420 7061 7373 776f 7264  mes and password
-00000640: 732e 2054 6865 2074 6162 6c65 206e 616d  s. The table nam
-00000650: 6520 616e 6420 636f 6c75 6d6e 206e 616d  e and column nam
-00000660: 6573 2063 616e 2062 6520 6173 2070 6572  es can be as per
-00000670: 2079 6f75 7220 6368 6f69 6365 2e0a 6060   your choice..``
-00000680: 6073 716c 0a43 5245 4154 4520 5441 424c  `sql.CREATE TABL
-00000690: 4520 7573 6572 7320 280a 2020 2020 7573  E users (.    us
-000006a0: 6572 6e61 6d65 2074 6578 7420 6e6f 7420  ername text not 
-000006b0: 6e75 6c6c 2064 6566 6175 6c74 2027 273a  null default '':
-000006c0: 3a74 6578 742c 0a20 2020 2070 6173 7377  :text,.    passw
-000006d0: 6f72 6420 7465 7874 206e 6f74 206e 756c  ord text not nul
-000006e0: 6c2c 0a20 2020 2063 6f6e 7374 7261 696e  l,.    constrain
-000006f0: 7420 7573 6572 735f 706b 6579 2070 7269  t users_pkey pri
-00000700: 6d61 7279 206b 6579 2028 7573 6572 6e61  mary key (userna
-00000710: 6d65 292c 0a20 2020 2063 6f6e 7374 7261  me),.    constra
-00000720: 696e 7420 7573 6572 735f 7573 6572 6e61  int users_userna
-00000730: 6d65 5f6b 6579 2075 6e69 7175 6520 2875  me_key unique (u
-00000740: 7365 726e 616d 6529 2c0a 2020 2020 636f  sername),.    co
-00000750: 6e73 7472 6169 6e74 2075 7365 7273 5f70  nstraint users_p
-00000760: 6173 7377 6f72 645f 6368 6563 6b20 6368  assword_check ch
-00000770: 6563 6b20 280a 2020 2020 2020 280a 2020  eck (.      (.  
-00000780: 2020 2020 2020 6c65 6e67 7468 280a 2020        length(.  
-00000790: 2020 2020 2020 2020 7472 696d 280a 2020          trim(.  
-000007a0: 2020 2020 2020 2020 2020 626f 7468 0a20            both. 
-000007b0: 2020 2020 2020 2020 2020 2066 726f 6d0a             from.
-000007c0: 2020 2020 2020 2020 2020 2020 2020 7061                pa
-000007d0: 7373 776f 7264 0a20 2020 2020 2020 2020  ssword.         
-000007e0: 2029 0a20 2020 2020 2020 2029 203e 2031   ).        ) > 1
-000007f0: 0a20 2020 2020 2029 0a20 2020 2029 2c0a  .      ).    ),.
-00000800: 2020 2020 636f 6e73 7472 6169 6e74 2075      constraint u
-00000810: 7365 7273 5f75 7365 726e 616d 655f 6368  sers_username_ch
-00000820: 6563 6b20 6368 6563 6b20 280a 2020 2020  eck check (.    
-00000830: 2020 280a 2020 2020 2020 2020 6c65 6e67    (.        leng
-00000840: 7468 280a 2020 2020 2020 2020 2020 7472  th(.          tr
-00000850: 696d 280a 2020 2020 2020 2020 2020 2020  im(.            
-00000860: 626f 7468 0a20 2020 2020 2020 2020 2020  both.           
-00000870: 2066 726f 6d0a 2020 2020 2020 2020 2020   from.          
-00000880: 2020 2020 7573 6572 6e61 6d65 0a20 2020      username.   
-00000890: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-000008a0: 2029 203e 2031 0a20 2020 2020 2029 0a20   ) > 1.      ). 
-000008b0: 2020 2029 0a20 2029 2074 6162 6c65 7370     ).  ) tablesp
-000008c0: 6163 6520 7067 5f64 6566 6175 6c74 3b0a  ace pg_default;.
-000008d0: 6060 600a 342e 2046 6f6c 6c6f 7720 7468  ```.4. Follow th
-000008e0: 6520 7265 7374 206f 6620 7468 6520 7374  e rest of the st
-000008f0: 6570 7320 6672 6f6d 205b 6865 7265 5d28  eps from [here](
-00000900: 6874 7470 733a 2f2f 646f 6373 2e73 7472  https://docs.str
-00000910: 6561 6d6c 6974 2e69 6f2f 6b6e 6f77 6c65  eamlit.io/knowle
-00000920: 6467 652d 6261 7365 2f74 7574 6f72 6961  dge-base/tutoria
-00000930: 6c73 2f64 6174 6162 6173 6573 2f73 7570  ls/databases/sup
-00000940: 6162 6173 6523 636f 7079 2d79 6f75 722d  abase#copy-your-
-00000950: 6170 702d 7365 6372 6574 732d 746f 2d74  app-secrets-to-t
-00000960: 6865 2d63 6c6f 7564 2920 746f 2063 6f6e  he-cloud) to con
-00000970: 6e65 6374 2079 6f75 7220 5374 7265 616d  nect your Stream
-00000980: 6c69 7420 6170 7020 746f 2053 7570 6162  lit app to Supab
-00000990: 6173 650a 0a0a 2323 203a 7065 6e3a 2055  ase...## :pen: U
-000009a0: 7361 6765 0a0a 606c 6f67 696e 5f66 6f72  sage..`login_for
-000009b0: 6d28 2960 2073 6574 7320 6073 6573 7369  m()` sets `sessi
-000009c0: 6f6e 5f73 7461 7465 5b22 6175 7468 656e  on_state["authen
-000009d0: 7469 6361 7465 6422 5d60 2074 6f20 6054  ticated"]` to `T
-000009e0: 7275 6560 2069 6620 7468 6520 6c6f 6769  rue` if the logi
-000009f0: 6e20 6973 2073 7563 6365 7373 6675 6c2c  n is successful,
-00000a00: 2060 7365 7373 696f 6e5f 7374 6174 655b   `session_state[
-00000a10: 2275 7365 726e 616d 6522 5d60 2074 6f20  "username"]` to 
-00000a20: 7468 6520 6075 7365 726e 616d 6560 206f  the `username` o
-00000a30: 7220 6e65 7720 6f72 2065 7869 7374 696e  r new or existin
-00000a40: 6720 7573 6572 2c20 616e 6420 746f 2060  g user, and to `
-00000a50: 4e6f 6e65 6020 666f 7220 6775 6573 7420  None` for guest 
-00000a60: 6c6f 6769 6e2e 0a0a 5265 7475 726e 7320  login...Returns 
-00000a70: 7375 7061 6261 7365 2060 436c 6965 6e74  supabase `Client
-00000a80: 6020 696e 7374 616e 6365 2e0a 0a60 6060  ` instance...```
-00000a90: 7079 7468 6f6e 0a69 6d70 6f72 7420 7374  python.import st
-00000aa0: 7265 616d 6c69 7420 6173 2073 740a 0a66  reamlit as st..f
-00000ab0: 726f 6d20 7374 7265 616d 6c69 745f 6c6f  rom streamlit_lo
-00000ac0: 6769 6e20 696d 706f 7274 206c 6f67 696e  gin import login
-00000ad0: 5f66 6f72 6d0a 0a63 6c69 656e 7420 3d20  _form..client = 
-00000ae0: 6c6f 6769 6e5f 666f 726d 2829 0a0a 6966  login_form()..if
-00000af0: 2073 742e 7365 7373 696f 6e5f 7374 6174   st.session_stat
-00000b00: 655b 2261 7574 6865 6e74 6963 6174 6564  e["authenticated
-00000b10: 225d 3a0a 2020 2020 6966 2073 742e 7365  "]:.    if st.se
-00000b20: 7373 696f 6e5f 7374 6174 655b 2275 7365  ssion_state["use
-00000b30: 726e 616d 6522 5d3a 0a20 2020 2020 2020  rname"]:.       
-00000b40: 2073 742e 7375 6363 6573 7328 6622 5765   st.success(f"We
-00000b50: 6c63 6f6d 6520 7b73 742e 7365 7373 696f  lcome {st.sessio
-00000b60: 6e5f 7374 6174 655b 2775 7365 726e 616d  n_state['usernam
-00000b70: 6527 5d7d 2229 0a20 2020 2065 6c73 653a  e']}").    else:
-00000b80: 0a20 2020 2020 2020 2073 742e 7375 6363  .        st.succ
-00000b90: 6573 7328 2257 656c 636f 6d65 2067 7565  ess("Welcome gue
-00000ba0: 7374 2229 0a65 6c73 653a 0a20 2020 2073  st").else:.    s
-00000bb0: 742e 6572 726f 7228 224e 6f74 2061 7574  t.error("Not aut
-00000bc0: 6865 6e74 6963 6174 6564 2229 0a60 6060  henticated").```
-00000bd0: 0a0a 5b21 5b53 6565 2064 656d 6f20 696e  ..[![See demo in
-00000be0: 2053 7472 6561 6d6c 6974 5d28 6874 7470   Streamlit](http
-00000bf0: 733a 2f2f 7374 6174 6963 2e73 7472 6561  s://static.strea
-00000c00: 6d6c 6974 2e69 6f2f 6261 6467 6573 2f73  mlit.io/badges/s
-00000c10: 7472 6561 6d6c 6974 5f62 6164 6765 5f62  treamlit_badge_b
-00000c20: 6c61 636b 5f77 6869 7465 2e73 7667 295d  lack_white.svg)]
-00000c30: 2868 7474 7073 3a2f 2f73 742d 6c67 6e2d  (https://st-lgn-
-00000c40: 666f 726d 2e73 7472 6561 6d6c 6974 2e61  form.streamlit.a
-00000c50: 7070 2f29 0a                             pp/).
+00000000: 2320 3a6c 6f63 6b3a 2073 742d 6c6f 6769  # :lock: st-logi
+00000010: 6e2d 666f 726d 0a5b 215b 446f 776e 6c6f  n-form.[![Downlo
+00000020: 6164 735d 2868 7474 7073 3a2f 2f73 7461  ads](https://sta
+00000030: 7469 632e 7065 7079 2e74 6563 682f 7065  tic.pepy.tech/pe
+00000040: 7273 6f6e 616c 697a 6564 2d62 6164 6765  rsonalized-badge
+00000050: 2f73 742d 6c6f 6769 6e2d 666f 726d 3f70  /st-login-form?p
+00000060: 6572 696f 643d 746f 7461 6c26 756e 6974  eriod=total&unit
+00000070: 733d 696e 7465 726e 6174 696f 6e61 6c5f  s=international_
+00000080: 7379 7374 656d 266c 6566 745f 636f 6c6f  system&left_colo
+00000090: 723d 626c 6163 6b26 7269 6768 745f 636f  r=black&right_co
+000000a0: 6c6f 723d 6272 6967 6874 6772 6565 6e26  lor=brightgreen&
+000000b0: 6c65 6674 5f74 6578 743d 446f 776e 6c6f  left_text=Downlo
+000000c0: 6164 7329 5d28 6874 7470 733a 2f2f 7065  ads)](https://pe
+000000d0: 7079 2e74 6563 682f 7072 6f6a 6563 742f  py.tech/project/
+000000e0: 7374 2d6c 6f67 696e 2d66 6f72 6d29 0a0a  st-login-form)..
+000000f0: 4120 7374 7265 616d 6c69 7420 636f 6d70  A streamlit comp
+00000100: 6f6e 656e 7420 7468 6174 2063 7265 6174  onent that creat
+00000110: 6573 2061 2075 7365 7220 6c6f 6769 6e20  es a user login 
+00000120: 666f 726d 2063 6f6e 6e65 6374 6564 2074  form connected t
+00000130: 6f20 6120 5375 7061 6261 7365 2044 422e  o a Supabase DB.
+00000140: 2049 7420 6c65 7473 2075 7365 7273 2063   It lets users c
+00000150: 7265 6174 6520 6120 6e65 7720 7573 6572  reate a new user
+00000160: 6e61 6d65 2061 6e64 2070 6173 7377 6f72  name and passwor
+00000170: 642c 206c 6f67 696e 2074 6f20 616e 2065  d, login to an e
+00000180: 7869 7374 696e 6720 6163 636f 756e 742c  xisting account,
+00000190: 206f 7220 6c6f 6769 6e20 6173 2061 6e20   or login as an 
+000001a0: 616e 6f6e 796d 6f75 7320 6775 6573 742e  anonymous guest.
+000001b0: 0a0a 215b 466f 726d 2073 6372 6565 6e73  ..![Form screens
+000001c0: 686f 745d 2861 7373 6574 732f 7363 7265  hot](assets/scre
+000001d0: 656e 7368 6f74 2e70 6e67 290a 0a54 6865  enshot.png)..The
+000001e0: 206c 6f67 696e 2066 6f72 6d20 636f 6c6c   login form coll
+000001f0: 6170 7365 7320 6166 7465 7220 6c6f 6769  apses after logi
+00000200: 6e20 746f 2066 7265 6520 7363 7265 656e  n to free screen
+00000210: 2d73 7061 6365 2e0a 0a23 2320 3a63 6f6d  -space...## :com
+00000220: 7075 7465 723a 2044 656d 6f20 6170 700a  puter: Demo app.
+00000230: 5b21 5b4f 7065 6e20 696e 2053 7472 6561  [![Open in Strea
+00000240: 6d6c 6974 5d28 6874 7470 733a 2f2f 7374  mlit](https://st
+00000250: 6174 6963 2e73 7472 6561 6d6c 6974 2e69  atic.streamlit.i
+00000260: 6f2f 6261 6467 6573 2f73 7472 6561 6d6c  o/badges/streaml
+00000270: 6974 5f62 6164 6765 5f62 6c61 636b 5f77  it_badge_black_w
+00000280: 6869 7465 2e73 7667 295d 2868 7474 7073  hite.svg)](https
+00000290: 3a2f 2f73 742d 6c67 6e2d 666f 726d 2e73  ://st-lgn-form.s
+000002a0: 7472 6561 6d6c 6974 2e61 7070 2f29 0a0a  treamlit.app/)..
+000002b0: 2323 203a 636f 6e73 7472 7563 7469 6f6e  ## :construction
+000002c0: 3a20 496e 7374 616c 6c61 7469 6f6e 200a  : Installation .
+000002d0: 0a31 2e20 496e 7374 616c 6c20 6073 742d  .1. Install `st-
+000002e0: 6c6f 6769 6e2d 666f 726d 6020 0a60 6060  login-form` .```
+000002f0: 7368 0a70 6970 2069 6e73 7461 6c6c 2073  sh.pip install s
+00000300: 742d 6c6f 6769 6e2d 666f 726d 0a60 6060  t-login-form.```
+00000310: 0a32 2e20 4372 6561 7465 2061 2053 7570  .2. Create a Sup
+00000320: 6162 6173 6520 7072 6f6a 6563 7420 6173  abase project as
+00000330: 206d 656e 7469 6f6e 6564 205b 6865 7265   mentioned [here
+00000340: 5d28 6874 7470 733a 2f2f 646f 6373 2e73  ](https://docs.s
+00000350: 7472 6561 6d6c 6974 2e69 6f2f 6b6e 6f77  treamlit.io/know
+00000360: 6c65 6467 652d 6261 7365 2f74 7574 6f72  ledge-base/tutor
+00000370: 6961 6c73 2f64 6174 6162 6173 6573 2f73  ials/databases/s
+00000380: 7570 6162 6173 6523 7369 676e 2d69 6e2d  upabase#sign-in-
+00000390: 746f 2d73 7570 6162 6173 652d 616e 642d  to-supabase-and-
+000003a0: 6372 6561 7465 2d61 2d70 726f 6a65 6374  create-a-project
+000003b0: 290a 332e 2043 7265 6174 6520 6120 7461  ).3. Create a ta
+000003c0: 626c 6520 746f 2073 746f 7265 2074 6865  ble to store the
+000003d0: 2075 7365 726e 616d 6573 2061 6e64 2070   usernames and p
+000003e0: 6173 7377 6f72 6473 2e20 5468 6520 7461  asswords. The ta
+000003f0: 626c 6520 6e61 6d65 2061 6e64 2063 6f6c  ble name and col
+00000400: 756d 6e20 6e61 6d65 7320 6361 6e20 6265  umn names can be
+00000410: 2061 7320 7065 7220 796f 7572 2063 686f   as per your cho
+00000420: 6963 652e 0a60 6060 7371 6c0a 4352 4541  ice..```sql.CREA
+00000430: 5445 2054 4142 4c45 2075 7365 7273 2028  TE TABLE users (
+00000440: 0a20 2020 2075 7365 726e 616d 6520 7465  .    username te
+00000450: 7874 206e 6f74 206e 756c 6c20 6465 6661  xt not null defa
+00000460: 756c 7420 2727 3a3a 7465 7874 2c0a 2020  ult ''::text,.  
+00000470: 2020 7061 7373 776f 7264 2074 6578 7420    password text 
+00000480: 6e6f 7420 6e75 6c6c 2c0a 2020 2020 636f  not null,.    co
+00000490: 6e73 7472 6169 6e74 2075 7365 7273 5f70  nstraint users_p
+000004a0: 6b65 7920 7072 696d 6172 7920 6b65 7920  key primary key 
+000004b0: 2875 7365 726e 616d 6529 2c0a 2020 2020  (username),.    
+000004c0: 636f 6e73 7472 6169 6e74 2075 7365 7273  constraint users
+000004d0: 5f75 7365 726e 616d 655f 6b65 7920 756e  _username_key un
+000004e0: 6971 7565 2028 7573 6572 6e61 6d65 292c  ique (username),
+000004f0: 0a20 2020 2063 6f6e 7374 7261 696e 7420  .    constraint 
+00000500: 7573 6572 735f 7061 7373 776f 7264 5f63  users_password_c
+00000510: 6865 636b 2063 6865 636b 2028 0a20 2020  heck check (.   
+00000520: 2020 2028 0a20 2020 2020 2020 206c 656e     (.        len
+00000530: 6774 6828 0a20 2020 2020 2020 2020 2074  gth(.          t
+00000540: 7269 6d28 0a20 2020 2020 2020 2020 2020  rim(.           
+00000550: 2062 6f74 680a 2020 2020 2020 2020 2020   both.          
+00000560: 2020 6672 6f6d 0a20 2020 2020 2020 2020    from.         
+00000570: 2020 2020 2070 6173 7377 6f72 640a 2020       password.  
+00000580: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00000590: 2020 2920 3e20 310a 2020 2020 2020 290a    ) > 1.      ).
+000005a0: 2020 2020 292c 0a20 2020 2063 6f6e 7374      ),.    const
+000005b0: 7261 696e 7420 7573 6572 735f 7573 6572  raint users_user
+000005c0: 6e61 6d65 5f63 6865 636b 2063 6865 636b  name_check check
+000005d0: 2028 0a20 2020 2020 2028 0a20 2020 2020   (.      (.     
+000005e0: 2020 206c 656e 6774 6828 0a20 2020 2020     length(.     
+000005f0: 2020 2020 2074 7269 6d28 0a20 2020 2020       trim(.     
+00000600: 2020 2020 2020 2062 6f74 680a 2020 2020         both.    
+00000610: 2020 2020 2020 2020 6672 6f6d 0a20 2020          from.   
+00000620: 2020 2020 2020 2020 2020 2075 7365 726e             usern
+00000630: 616d 650a 2020 2020 2020 2020 2020 290a  ame.          ).
+00000640: 2020 2020 2020 2020 2920 3e20 310a 2020          ) > 1.  
+00000650: 2020 2020 290a 2020 2020 290a 2020 2920      ).    ).  ) 
+00000660: 7461 626c 6573 7061 6365 2070 675f 6465  tablespace pg_de
+00000670: 6661 756c 743b 0a60 6060 0a34 2e20 466f  fault;.```.4. Fo
+00000680: 6c6c 6f77 2074 6865 2072 6573 7420 6f66  llow the rest of
+00000690: 2074 6865 2073 7465 7073 2066 726f 6d20   the steps from 
+000006a0: 5b68 6572 655d 2868 7474 7073 3a2f 2f64  [here](https://d
+000006b0: 6f63 732e 7374 7265 616d 6c69 742e 696f  ocs.streamlit.io
+000006c0: 2f6b 6e6f 776c 6564 6765 2d62 6173 652f  /knowledge-base/
+000006d0: 7475 746f 7269 616c 732f 6461 7461 6261  tutorials/databa
+000006e0: 7365 732f 7375 7061 6261 7365 2363 6f70  ses/supabase#cop
+000006f0: 792d 796f 7572 2d61 7070 2d73 6563 7265  y-your-app-secre
+00000700: 7473 2d74 6f2d 7468 652d 636c 6f75 6429  ts-to-the-cloud)
+00000710: 2074 6f20 636f 6e6e 6563 7420 796f 7572   to connect your
+00000720: 2053 7472 6561 6d6c 6974 2061 7070 2074   Streamlit app t
+00000730: 6f20 5375 7061 6261 7365 0a0a 0a23 2320  o Supabase...## 
+00000740: 3a70 656e 3a20 5573 6167 650a 0a60 6c6f  :pen: Usage..`lo
+00000750: 6769 6e5f 666f 726d 2829 6020 7365 7473  gin_form()` sets
+00000760: 2060 7365 7373 696f 6e5f 7374 6174 655b   `session_state[
+00000770: 2261 7574 6865 6e74 6963 6174 6564 225d  "authenticated"]
+00000780: 6020 746f 2060 5472 7565 6020 6966 2074  ` to `True` if t
+00000790: 6865 206c 6f67 696e 2069 7320 7375 6363  he login is succ
+000007a0: 6573 7366 756c 2c20 6073 6573 7369 6f6e  essful, `session
+000007b0: 5f73 7461 7465 5b22 7573 6572 6e61 6d65  _state["username
+000007c0: 225d 6020 746f 2074 6865 2060 7573 6572  "]` to the `user
+000007d0: 6e61 6d65 6020 6f72 206e 6577 206f 7220  name` or new or 
+000007e0: 6578 6973 7469 6e67 2075 7365 722c 2061  existing user, a
+000007f0: 6e64 2074 6f20 604e 6f6e 6560 2066 6f72  nd to `None` for
+00000800: 2067 7565 7374 206c 6f67 696e 2e0a 0a52   guest login...R
+00000810: 6574 7572 6e73 2074 6865 2069 6e69 7469  eturns the initi
+00000820: 616c 697a 6564 2060 7375 7061 6261 7365  alized `supabase
+00000830: 2e43 6c69 656e 7460 2069 6e73 7461 6e63  .Client` instanc
+00000840: 6520 746f 206c 6574 2079 6f75 2069 6e74  e to let you int
+00000850: 6572 6163 7420 7769 7468 2074 6865 2064  eract with the d
+00000860: 6174 6162 7365 2064 6f77 6e73 7472 6561  atabse downstrea
+00000870: 6d20 696e 2074 6865 2073 6372 6970 742e  m in the script.
+00000880: 0a0a 6060 6070 7974 686f 6e0a 696d 706f  ..```python.impo
+00000890: 7274 2073 7472 6561 6d6c 6974 2061 7320  rt streamlit as 
+000008a0: 7374 0a0a 6672 6f6d 2073 7472 6561 6d6c  st..from streaml
+000008b0: 6974 5f6c 6f67 696e 2069 6d70 6f72 7420  it_login import 
+000008c0: 6c6f 6769 6e5f 666f 726d 0a0a 636c 6965  login_form..clie
+000008d0: 6e74 203d 206c 6f67 696e 5f66 6f72 6d28  nt = login_form(
+000008e0: 290a 0a69 6620 7374 2e73 6573 7369 6f6e  )..if st.session
+000008f0: 5f73 7461 7465 5b22 6175 7468 656e 7469  _state["authenti
+00000900: 6361 7465 6422 5d3a 0a20 2020 2069 6620  cated"]:.    if 
+00000910: 7374 2e73 6573 7369 6f6e 5f73 7461 7465  st.session_state
+00000920: 5b22 7573 6572 6e61 6d65 225d 3a0a 2020  ["username"]:.  
+00000930: 2020 2020 2020 7374 2e73 7563 6365 7373        st.success
+00000940: 2866 2257 656c 636f 6d65 207b 7374 2e73  (f"Welcome {st.s
+00000950: 6573 7369 6f6e 5f73 7461 7465 5b27 7573  ession_state['us
+00000960: 6572 6e61 6d65 275d 7d22 290a 2020 2020  ername']}").    
+00000970: 656c 7365 3a0a 2020 2020 2020 2020 7374  else:.        st
+00000980: 2e73 7563 6365 7373 2822 5765 6c63 6f6d  .success("Welcom
+00000990: 6520 6775 6573 7422 290a 656c 7365 3a0a  e guest").else:.
+000009a0: 2020 2020 7374 2e65 7272 6f72 2822 4e6f      st.error("No
+000009b0: 7420 6175 7468 656e 7469 6361 7465 6422  t authenticated"
+000009c0: 290a 6060 600a 0a5b 215b 5365 6520 6465  ).```..[![See de
+000009d0: 6d6f 2069 6e20 5374 7265 616d 6c69 745d  mo in Streamlit]
+000009e0: 2868 7474 7073 3a2f 2f73 7461 7469 632e  (https://static.
+000009f0: 7374 7265 616d 6c69 742e 696f 2f62 6164  streamlit.io/bad
+00000a00: 6765 732f 7374 7265 616d 6c69 745f 6261  ges/streamlit_ba
+00000a10: 6467 655f 626c 6163 6b5f 7768 6974 652e  dge_black_white.
+00000a20: 7376 6729 5d28 6874 7470 733a 2f2f 7374  svg)](https://st
+00000a30: 2d6c 676e 2d66 6f72 6d2e 7374 7265 616d  -lgn-form.stream
+00000a40: 6c69 742e 6170 702f 290a 0a23 2320 f09f  lit.app/)..## ..
+00000a50: a497 2057 616e 7420 746f 2073 7570 706f  .. Want to suppo
+00000a60: 7274 206d 7920 776f 726b 3f0a 3c70 2061  rt my work?.<p a
+00000a70: 6c69 676e 3d22 6365 6e74 6572 223e 0a20  lign="center">. 
+00000a80: 2020 203c 6120 6872 6566 3d22 6874 7470     <a href="http
+00000a90: 733a 2f2f 7777 772e 6275 796d 6561 636f  s://www.buymeaco
+00000aa0: 6666 6565 2e63 6f6d 2f73 6964 6468 616e  ffee.com/siddhan
+00000ab0: 7473 6164 616e 6769 2220 7461 7267 6574  tsadangi" target
+00000ac0: 3d22 5f62 6c61 6e6b 223e 3c69 6d67 2073  ="_blank"><img s
+00000ad0: 7263 3d22 6874 7470 733a 2f2f 6364 6e2e  rc="https://cdn.
+00000ae0: 6275 796d 6561 636f 6666 6565 2e63 6f6d  buymeacoffee.com
+00000af0: 2f62 7574 746f 6e73 2f76 322f 6465 6661  /buttons/v2/defa
+00000b00: 756c 742d 7965 6c6c 6f77 2e70 6e67 2220  ult-yellow.png" 
+00000b10: 616c 743d 2242 7579 204d 6520 4120 436f  alt="Buy Me A Co
+00000b20: 6666 6565 2220 7374 796c 653d 2268 6569  ffee" style="hei
+00000b30: 6768 743a 2036 3070 7820 2169 6d70 6f72  ght: 60px !impor
+00000b40: 7461 6e74 3b77 6964 7468 3a20 3231 3770  tant;width: 217p
+00000b50: 7820 2169 6d70 6f72 7461 6e74 3b22 3e0a  x !important;">.
+00000b60: 2020 2020 3c2f 613e 0a3c 2f70 3e0a           </a>.</p>.
```

### Comparing `st-login-form-0.2.0/setup.py` & `st-login-form-0.3.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,20 +3,25 @@
 import setuptools
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="st-login-form",
-    version="0.2.0",
+    version="0.3.0",
+    url="https://github.com/SiddhantSadangi/st_login_form",
     author="Siddhant Sadangi",
     author_email="siddhant.sadangi@gmail.com",
     description="A streamlit component that creates a user login form connected to a Supabase DB. It lets users create a new username and password, login to an existing account, or login as an anonymous guest.",
     long_description=long_description,
     long_description_content_type="text/markdown",
+    project_urls={
+        "Documentation": "https://github.com/SiddhantSadangi/st_login_form/blob/main/README.md",
+        "Support": "https://www.buymeacoffee.com/siddhantsadangi",
+    },
     packages=setuptools.find_packages(where="src"),
     package_dir={"": "src"},
     include_package_data=True,
     classifiers=[
         "Environment :: Plugins",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
```

### Comparing `st-login-form-0.2.0/src/st_login_form/__init__.py` & `st-login-form-0.3.0/src/st_login_form/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     allow_guest: bool = True,
     guest_title: str = "Guest login :ninja: ",
     create_username_label: str = "Create a unique username",
     create_username_placeholder: str = None,
     create_username_help: str = None,
     create_password_label: str = "Create a password",
     create_password_placeholder: str = None,
-    create_password_help: str = "⚠️ Password will be stored as plain text. Do not reuse from other websites. Password cannot be recovered.",
+    create_password_help: str = "⚠️ Remember your password. You won't be able to recover it if forgotten.",
     create_submit_label: str = "Create account",
     create_success_message: str = "Account created :tada:",
     login_username_label: str = "Enter your unique username",
     login_username_placeholder: str = None,
     login_username_help: str = None,
     login_password_label: str = "Enter your password",
     login_password_placeholder: str = None,
@@ -101,15 +101,17 @@
                     label=create_submit_label,
                     type="primary",
                     disabled=st.session_state["authenticated"],
                 ):
                     try:
                         data, _ = (
                             client.table(user_tablename)
-                            .insert({username_col: username, password_col: password})
+                            .insert(
+                                {username_col: username, password_col: hash(password)}
+                            )
                             .execute()
                         )
                     except Exception as e:
                         st.error(e.message)
                     else:
                         login_success(create_success_message, username)
 
@@ -136,15 +138,15 @@
                     disabled=st.session_state["authenticated"],
                     type="primary",
                 ):
                     data, _ = (
                         client.table(user_tablename)
                         .select(f"{username_col}, {password_col}")
                         .eq(username_col, username)
-                        .eq(password_col, password)
+                        .eq(password_col, hash(password))
                         .execute()
                     )
 
                     if len(data[-1]) > 0:
                         login_success(login_success_message, username)
                     else:
                         st.error(login_error_message)
@@ -161,14 +163,14 @@
 
         return client
 
 
 def main() -> None:
     login_form(
         create_username_placeholder="Username will be visible in the global leaderboard.",
-        create_password_placeholder="⚠️ Password will be stored as plain text. You won't be able to recover it if you forget.",
+        create_password_placeholder="⚠️ Remember your password. You won't be able to recover it if you forget.",
         guest_submit_label="Play as a guest ⚠️ Scores won't be saved",
     )
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `st-login-form-0.2.0/src/st_login_form.egg-info/PKG-INFO` & `st-login-form-0.3.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,198 +1,248 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7374 2d6c  : 2.1.Name: st-l
 00000020: 6f67 696e 2d66 6f72 6d0a 5665 7273 696f  ogin-form.Versio
-00000030: 6e3a 2030 2e32 2e30 0a53 756d 6d61 7279  n: 0.2.0.Summary
+00000030: 6e3a 2030 2e33 2e30 0a53 756d 6d61 7279  n: 0.3.0.Summary
 00000040: 3a20 4120 7374 7265 616d 6c69 7420 636f  : A streamlit co
 00000050: 6d70 6f6e 656e 7420 7468 6174 2063 7265  mponent that cre
 00000060: 6174 6573 2061 2075 7365 7220 6c6f 6769  ates a user logi
 00000070: 6e20 666f 726d 2063 6f6e 6e65 6374 6564  n form connected
 00000080: 2074 6f20 6120 5375 7061 6261 7365 2044   to a Supabase D
 00000090: 422e 2049 7420 6c65 7473 2075 7365 7273  B. It lets users
 000000a0: 2063 7265 6174 6520 6120 6e65 7720 7573   create a new us
 000000b0: 6572 6e61 6d65 2061 6e64 2070 6173 7377  ername and passw
 000000c0: 6f72 642c 206c 6f67 696e 2074 6f20 616e  ord, login to an
 000000d0: 2065 7869 7374 696e 6720 6163 636f 756e   existing accoun
 000000e0: 742c 206f 7220 6c6f 6769 6e20 6173 2061  t, or login as a
 000000f0: 6e20 616e 6f6e 796d 6f75 7320 6775 6573  n anonymous gues
-00000100: 742e 0a41 7574 686f 723a 2053 6964 6468  t..Author: Siddh
-00000110: 616e 7420 5361 6461 6e67 690a 4175 7468  ant Sadangi.Auth
-00000120: 6f72 2d65 6d61 696c 3a20 7369 6464 6861  or-email: siddha
-00000130: 6e74 2e73 6164 616e 6769 4067 6d61 696c  nt.sadangi@gmail
-00000140: 2e63 6f6d 0a4b 6579 776f 7264 733a 2073  .com.Keywords: s
-00000150: 7472 6561 6d6c 6974 2c6c 6f67 696e 0a43  treamlit,login.C
-00000160: 6c61 7373 6966 6965 723a 2045 6e76 6972  lassifier: Envir
-00000170: 6f6e 6d65 6e74 203a 3a20 506c 7567 696e  onment :: Plugin
-00000180: 730a 436c 6173 7369 6669 6572 3a20 496e  s.Classifier: In
-00000190: 7465 6e64 6564 2041 7564 6965 6e63 6520  tended Audience 
-000001a0: 3a3a 2044 6576 656c 6f70 6572 730a 436c  :: Developers.Cl
-000001b0: 6173 7369 6669 6572 3a20 4c69 6365 6e73  assifier: Licens
-000001c0: 6520 3a3a 204f 5349 2041 7070 726f 7665  e :: OSI Approve
-000001d0: 6420 3a3a 2047 4e55 2047 656e 6572 616c  d :: GNU General
-000001e0: 2050 7562 6c69 6320 4c69 6365 6e73 6520   Public License 
-000001f0: 7633 2028 4750 4c76 3329 0a43 6c61 7373  v3 (GPLv3).Class
-00000200: 6966 6965 723a 204f 7065 7261 7469 6e67  ifier: Operating
-00000210: 2053 7973 7465 6d20 3a3a 204f 5320 496e   System :: OS In
-00000220: 6465 7065 6e64 656e 740a 436c 6173 7369  dependent.Classi
-00000230: 6669 6572 3a20 5072 6f67 7261 6d6d 696e  fier: Programmin
-00000240: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-00000250: 7468 6f6e 0a43 6c61 7373 6966 6965 723a  thon.Classifier:
-00000260: 2054 6f70 6963 203a 3a20 536f 6674 7761   Topic :: Softwa
-00000270: 7265 2044 6576 656c 6f70 6d65 6e74 203a  re Development :
-00000280: 3a20 4c69 6272 6172 6965 7320 3a3a 2050  : Libraries :: P
-00000290: 7974 686f 6e20 4d6f 6475 6c65 730a 436c  ython Modules.Cl
-000002a0: 6173 7369 6669 6572 3a20 546f 7069 6320  assifier: Topic 
-000002b0: 3a3a 2053 6f66 7477 6172 6520 4465 7665  :: Software Deve
-000002c0: 6c6f 706d 656e 7420 3a3a 2055 7365 7220  lopment :: User 
-000002d0: 496e 7465 7266 6163 6573 0a52 6571 7569  Interfaces.Requi
-000002e0: 7265 732d 5079 7468 6f6e 3a20 3e3d 332e  res-Python: >=3.
-000002f0: 380a 4465 7363 7269 7074 696f 6e2d 436f  8.Description-Co
-00000300: 6e74 656e 742d 5479 7065 3a20 7465 7874  ntent-Type: text
-00000310: 2f6d 6172 6b64 6f77 6e0a 4c69 6365 6e73  /markdown.Licens
-00000320: 652d 4669 6c65 3a20 4c49 4345 4e53 450a  e-File: LICENSE.
-00000330: 0a23 203a 6c6f 636b 3a20 7374 2d6c 6f67  .# :lock: st-log
-00000340: 696e 2d66 6f72 6d0a 0a41 2073 7472 6561  in-form..A strea
-00000350: 6d6c 6974 2063 6f6d 706f 6e65 6e74 2074  mlit component t
-00000360: 6861 7420 6372 6561 7465 7320 6120 7573  hat creates a us
-00000370: 6572 206c 6f67 696e 2066 6f72 6d20 636f  er login form co
-00000380: 6e6e 6563 7465 6420 746f 2061 2053 7570  nnected to a Sup
-00000390: 6162 6173 6520 4442 2e20 4974 206c 6574  abase DB. It let
-000003a0: 7320 7573 6572 7320 6372 6561 7465 2061  s users create a
-000003b0: 206e 6577 2075 7365 726e 616d 6520 616e   new username an
-000003c0: 6420 7061 7373 776f 7264 2c20 6c6f 6769  d password, logi
-000003d0: 6e20 746f 2061 6e20 6578 6973 7469 6e67  n to an existing
-000003e0: 2061 6363 6f75 6e74 2c20 6f72 206c 6f67   account, or log
-000003f0: 696e 2061 7320 616e 2061 6e6f 6e79 6d6f  in as an anonymo
-00000400: 7573 2067 7565 7374 2e0a 0a21 5b46 6f72  us guest...![For
-00000410: 6d20 7363 7265 656e 7368 6f74 5d28 6173  m screenshot](as
-00000420: 7365 7473 2f73 6372 6565 6e73 686f 742e  sets/screenshot.
-00000430: 706e 6729 0a0a 5468 6520 6c6f 6769 6e20  png)..The login 
-00000440: 666f 726d 2063 6f6c 6c61 7073 6573 2061  form collapses a
-00000450: 6674 6572 206c 6f67 696e 2074 6f20 6672  fter login to fr
-00000460: 6565 2073 6372 6565 6e2d 7370 6163 652e  ee screen-space.
-00000470: 0a0a 2323 203a 636f 6d70 7574 6572 3a20  ..## :computer: 
-00000480: 4465 6d6f 2061 7070 0a5b 215b 4f70 656e  Demo app.[![Open
-00000490: 2069 6e20 5374 7265 616d 6c69 745d 2868   in Streamlit](h
-000004a0: 7474 7073 3a2f 2f73 7461 7469 632e 7374  ttps://static.st
-000004b0: 7265 616d 6c69 742e 696f 2f62 6164 6765  reamlit.io/badge
-000004c0: 732f 7374 7265 616d 6c69 745f 6261 6467  s/streamlit_badg
-000004d0: 655f 626c 6163 6b5f 7768 6974 652e 7376  e_black_white.sv
-000004e0: 6729 5d28 6874 7470 733a 2f2f 7374 2d6c  g)](https://st-l
-000004f0: 676e 2d66 6f72 6d2e 7374 7265 616d 6c69  gn-form.streamli
-00000500: 742e 6170 702f 290a 0a23 2320 3a63 6f6e  t.app/)..## :con
-00000510: 7374 7275 6374 696f 6e3a 2049 6e73 7461  struction: Insta
-00000520: 6c6c 6174 696f 6e20 0a0a 312e 2049 6e73  llation ..1. Ins
-00000530: 7461 6c6c 2060 7374 2d6c 6f67 696e 2d66  tall `st-login-f
-00000540: 6f72 6d60 200a 6060 6073 680a 7069 7020  orm` .```sh.pip 
-00000550: 696e 7374 616c 6c20 7374 2d6c 6f67 696e  install st-login
-00000560: 2d66 6f72 6d0a 6060 600a 322e 2043 7265  -form.```.2. Cre
-00000570: 6174 6520 6120 5375 7061 6261 7365 2070  ate a Supabase p
-00000580: 726f 6a65 6374 2061 7320 6d65 6e74 696f  roject as mentio
-00000590: 6e65 6420 5b68 6572 655d 2868 7474 7073  ned [here](https
-000005a0: 3a2f 2f64 6f63 732e 7374 7265 616d 6c69  ://docs.streamli
-000005b0: 742e 696f 2f6b 6e6f 776c 6564 6765 2d62  t.io/knowledge-b
-000005c0: 6173 652f 7475 746f 7269 616c 732f 6461  ase/tutorials/da
-000005d0: 7461 6261 7365 732f 7375 7061 6261 7365  tabases/supabase
-000005e0: 2373 6967 6e2d 696e 2d74 6f2d 7375 7061  #sign-in-to-supa
-000005f0: 6261 7365 2d61 6e64 2d63 7265 6174 652d  base-and-create-
-00000600: 612d 7072 6f6a 6563 7429 0a33 2e20 4372  a-project).3. Cr
-00000610: 6561 7465 2061 2074 6162 6c65 2074 6f20  eate a table to 
-00000620: 7374 6f72 6520 7468 6520 7573 6572 6e61  store the userna
-00000630: 6d65 7320 616e 6420 7061 7373 776f 7264  mes and password
-00000640: 732e 2054 6865 2074 6162 6c65 206e 616d  s. The table nam
-00000650: 6520 616e 6420 636f 6c75 6d6e 206e 616d  e and column nam
-00000660: 6573 2063 616e 2062 6520 6173 2070 6572  es can be as per
-00000670: 2079 6f75 7220 6368 6f69 6365 2e0a 6060   your choice..``
-00000680: 6073 716c 0a43 5245 4154 4520 5441 424c  `sql.CREATE TABL
-00000690: 4520 7573 6572 7320 280a 2020 2020 7573  E users (.    us
-000006a0: 6572 6e61 6d65 2074 6578 7420 6e6f 7420  ername text not 
-000006b0: 6e75 6c6c 2064 6566 6175 6c74 2027 273a  null default '':
-000006c0: 3a74 6578 742c 0a20 2020 2070 6173 7377  :text,.    passw
-000006d0: 6f72 6420 7465 7874 206e 6f74 206e 756c  ord text not nul
-000006e0: 6c2c 0a20 2020 2063 6f6e 7374 7261 696e  l,.    constrain
-000006f0: 7420 7573 6572 735f 706b 6579 2070 7269  t users_pkey pri
-00000700: 6d61 7279 206b 6579 2028 7573 6572 6e61  mary key (userna
-00000710: 6d65 292c 0a20 2020 2063 6f6e 7374 7261  me),.    constra
-00000720: 696e 7420 7573 6572 735f 7573 6572 6e61  int users_userna
-00000730: 6d65 5f6b 6579 2075 6e69 7175 6520 2875  me_key unique (u
-00000740: 7365 726e 616d 6529 2c0a 2020 2020 636f  sername),.    co
-00000750: 6e73 7472 6169 6e74 2075 7365 7273 5f70  nstraint users_p
-00000760: 6173 7377 6f72 645f 6368 6563 6b20 6368  assword_check ch
-00000770: 6563 6b20 280a 2020 2020 2020 280a 2020  eck (.      (.  
-00000780: 2020 2020 2020 6c65 6e67 7468 280a 2020        length(.  
-00000790: 2020 2020 2020 2020 7472 696d 280a 2020          trim(.  
-000007a0: 2020 2020 2020 2020 2020 626f 7468 0a20            both. 
-000007b0: 2020 2020 2020 2020 2020 2066 726f 6d0a             from.
-000007c0: 2020 2020 2020 2020 2020 2020 2020 7061                pa
-000007d0: 7373 776f 7264 0a20 2020 2020 2020 2020  ssword.         
-000007e0: 2029 0a20 2020 2020 2020 2029 203e 2031   ).        ) > 1
-000007f0: 0a20 2020 2020 2029 0a20 2020 2029 2c0a  .      ).    ),.
-00000800: 2020 2020 636f 6e73 7472 6169 6e74 2075      constraint u
-00000810: 7365 7273 5f75 7365 726e 616d 655f 6368  sers_username_ch
-00000820: 6563 6b20 6368 6563 6b20 280a 2020 2020  eck check (.    
-00000830: 2020 280a 2020 2020 2020 2020 6c65 6e67    (.        leng
-00000840: 7468 280a 2020 2020 2020 2020 2020 7472  th(.          tr
-00000850: 696d 280a 2020 2020 2020 2020 2020 2020  im(.            
-00000860: 626f 7468 0a20 2020 2020 2020 2020 2020  both.           
-00000870: 2066 726f 6d0a 2020 2020 2020 2020 2020   from.          
-00000880: 2020 2020 7573 6572 6e61 6d65 0a20 2020      username.   
-00000890: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-000008a0: 2029 203e 2031 0a20 2020 2020 2029 0a20   ) > 1.      ). 
-000008b0: 2020 2029 0a20 2029 2074 6162 6c65 7370     ).  ) tablesp
-000008c0: 6163 6520 7067 5f64 6566 6175 6c74 3b0a  ace pg_default;.
-000008d0: 6060 600a 342e 2046 6f6c 6c6f 7720 7468  ```.4. Follow th
-000008e0: 6520 7265 7374 206f 6620 7468 6520 7374  e rest of the st
-000008f0: 6570 7320 6672 6f6d 205b 6865 7265 5d28  eps from [here](
-00000900: 6874 7470 733a 2f2f 646f 6373 2e73 7472  https://docs.str
-00000910: 6561 6d6c 6974 2e69 6f2f 6b6e 6f77 6c65  eamlit.io/knowle
-00000920: 6467 652d 6261 7365 2f74 7574 6f72 6961  dge-base/tutoria
-00000930: 6c73 2f64 6174 6162 6173 6573 2f73 7570  ls/databases/sup
-00000940: 6162 6173 6523 636f 7079 2d79 6f75 722d  abase#copy-your-
-00000950: 6170 702d 7365 6372 6574 732d 746f 2d74  app-secrets-to-t
-00000960: 6865 2d63 6c6f 7564 2920 746f 2063 6f6e  he-cloud) to con
-00000970: 6e65 6374 2079 6f75 7220 5374 7265 616d  nect your Stream
-00000980: 6c69 7420 6170 7020 746f 2053 7570 6162  lit app to Supab
-00000990: 6173 650a 0a0a 2323 203a 7065 6e3a 2055  ase...## :pen: U
-000009a0: 7361 6765 0a0a 606c 6f67 696e 5f66 6f72  sage..`login_for
-000009b0: 6d28 2960 2073 6574 7320 6073 6573 7369  m()` sets `sessi
-000009c0: 6f6e 5f73 7461 7465 5b22 6175 7468 656e  on_state["authen
-000009d0: 7469 6361 7465 6422 5d60 2074 6f20 6054  ticated"]` to `T
-000009e0: 7275 6560 2069 6620 7468 6520 6c6f 6769  rue` if the logi
-000009f0: 6e20 6973 2073 7563 6365 7373 6675 6c2c  n is successful,
-00000a00: 2060 7365 7373 696f 6e5f 7374 6174 655b   `session_state[
-00000a10: 2275 7365 726e 616d 6522 5d60 2074 6f20  "username"]` to 
-00000a20: 7468 6520 6075 7365 726e 616d 6560 206f  the `username` o
-00000a30: 7220 6e65 7720 6f72 2065 7869 7374 696e  r new or existin
-00000a40: 6720 7573 6572 2c20 616e 6420 746f 2060  g user, and to `
-00000a50: 4e6f 6e65 6020 666f 7220 6775 6573 7420  None` for guest 
-00000a60: 6c6f 6769 6e2e 0a0a 5265 7475 726e 7320  login...Returns 
-00000a70: 7375 7061 6261 7365 2060 436c 6965 6e74  supabase `Client
-00000a80: 6020 696e 7374 616e 6365 2e0a 0a60 6060  ` instance...```
-00000a90: 7079 7468 6f6e 0a69 6d70 6f72 7420 7374  python.import st
-00000aa0: 7265 616d 6c69 7420 6173 2073 740a 0a66  reamlit as st..f
-00000ab0: 726f 6d20 7374 7265 616d 6c69 745f 6c6f  rom streamlit_lo
-00000ac0: 6769 6e20 696d 706f 7274 206c 6f67 696e  gin import login
-00000ad0: 5f66 6f72 6d0a 0a63 6c69 656e 7420 3d20  _form..client = 
-00000ae0: 6c6f 6769 6e5f 666f 726d 2829 0a0a 6966  login_form()..if
-00000af0: 2073 742e 7365 7373 696f 6e5f 7374 6174   st.session_stat
-00000b00: 655b 2261 7574 6865 6e74 6963 6174 6564  e["authenticated
-00000b10: 225d 3a0a 2020 2020 6966 2073 742e 7365  "]:.    if st.se
-00000b20: 7373 696f 6e5f 7374 6174 655b 2275 7365  ssion_state["use
-00000b30: 726e 616d 6522 5d3a 0a20 2020 2020 2020  rname"]:.       
-00000b40: 2073 742e 7375 6363 6573 7328 6622 5765   st.success(f"We
-00000b50: 6c63 6f6d 6520 7b73 742e 7365 7373 696f  lcome {st.sessio
-00000b60: 6e5f 7374 6174 655b 2775 7365 726e 616d  n_state['usernam
-00000b70: 6527 5d7d 2229 0a20 2020 2065 6c73 653a  e']}").    else:
-00000b80: 0a20 2020 2020 2020 2073 742e 7375 6363  .        st.succ
-00000b90: 6573 7328 2257 656c 636f 6d65 2067 7565  ess("Welcome gue
-00000ba0: 7374 2229 0a65 6c73 653a 0a20 2020 2073  st").else:.    s
-00000bb0: 742e 6572 726f 7228 224e 6f74 2061 7574  t.error("Not aut
-00000bc0: 6865 6e74 6963 6174 6564 2229 0a60 6060  henticated").```
-00000bd0: 0a0a 5b21 5b53 6565 2064 656d 6f20 696e  ..[![See demo in
-00000be0: 2053 7472 6561 6d6c 6974 5d28 6874 7470   Streamlit](http
-00000bf0: 733a 2f2f 7374 6174 6963 2e73 7472 6561  s://static.strea
-00000c00: 6d6c 6974 2e69 6f2f 6261 6467 6573 2f73  mlit.io/badges/s
-00000c10: 7472 6561 6d6c 6974 5f62 6164 6765 5f62  treamlit_badge_b
-00000c20: 6c61 636b 5f77 6869 7465 2e73 7667 295d  lack_white.svg)]
-00000c30: 2868 7474 7073 3a2f 2f73 742d 6c67 6e2d  (https://st-lgn-
-00000c40: 666f 726d 2e73 7472 6561 6d6c 6974 2e61  form.streamlit.a
-00000c50: 7070 2f29 0a                             pp/).
+00000100: 742e 0a48 6f6d 652d 7061 6765 3a20 6874  t..Home-page: ht
+00000110: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000120: 2f53 6964 6468 616e 7453 6164 616e 6769  /SiddhantSadangi
+00000130: 2f73 745f 6c6f 6769 6e5f 666f 726d 0a41  /st_login_form.A
+00000140: 7574 686f 723a 2053 6964 6468 616e 7420  uthor: Siddhant 
+00000150: 5361 6461 6e67 690a 4175 7468 6f72 2d65  Sadangi.Author-e
+00000160: 6d61 696c 3a20 7369 6464 6861 6e74 2e73  mail: siddhant.s
+00000170: 6164 616e 6769 4067 6d61 696c 2e63 6f6d  adangi@gmail.com
+00000180: 0a50 726f 6a65 6374 2d55 524c 3a20 446f  .Project-URL: Do
+00000190: 6375 6d65 6e74 6174 696f 6e2c 2068 7474  cumentation, htt
+000001a0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+000001b0: 5369 6464 6861 6e74 5361 6461 6e67 692f  SiddhantSadangi/
+000001c0: 7374 5f6c 6f67 696e 5f66 6f72 6d2f 626c  st_login_form/bl
+000001d0: 6f62 2f6d 6169 6e2f 5245 4144 4d45 2e6d  ob/main/README.m
+000001e0: 640a 5072 6f6a 6563 742d 5552 4c3a 2053  d.Project-URL: S
+000001f0: 7570 706f 7274 2c20 6874 7470 733a 2f2f  upport, https://
+00000200: 7777 772e 6275 796d 6561 636f 6666 6565  www.buymeacoffee
+00000210: 2e63 6f6d 2f73 6964 6468 616e 7473 6164  .com/siddhantsad
+00000220: 616e 6769 0a4b 6579 776f 7264 733a 2073  angi.Keywords: s
+00000230: 7472 6561 6d6c 6974 2c6c 6f67 696e 0a43  treamlit,login.C
+00000240: 6c61 7373 6966 6965 723a 2045 6e76 6972  lassifier: Envir
+00000250: 6f6e 6d65 6e74 203a 3a20 506c 7567 696e  onment :: Plugin
+00000260: 730a 436c 6173 7369 6669 6572 3a20 496e  s.Classifier: In
+00000270: 7465 6e64 6564 2041 7564 6965 6e63 6520  tended Audience 
+00000280: 3a3a 2044 6576 656c 6f70 6572 730a 436c  :: Developers.Cl
+00000290: 6173 7369 6669 6572 3a20 4c69 6365 6e73  assifier: Licens
+000002a0: 6520 3a3a 204f 5349 2041 7070 726f 7665  e :: OSI Approve
+000002b0: 6420 3a3a 2047 4e55 2047 656e 6572 616c  d :: GNU General
+000002c0: 2050 7562 6c69 6320 4c69 6365 6e73 6520   Public License 
+000002d0: 7633 2028 4750 4c76 3329 0a43 6c61 7373  v3 (GPLv3).Class
+000002e0: 6966 6965 723a 204f 7065 7261 7469 6e67  ifier: Operating
+000002f0: 2053 7973 7465 6d20 3a3a 204f 5320 496e   System :: OS In
+00000300: 6465 7065 6e64 656e 740a 436c 6173 7369  dependent.Classi
+00000310: 6669 6572 3a20 5072 6f67 7261 6d6d 696e  fier: Programmin
+00000320: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+00000330: 7468 6f6e 0a43 6c61 7373 6966 6965 723a  thon.Classifier:
+00000340: 2054 6f70 6963 203a 3a20 536f 6674 7761   Topic :: Softwa
+00000350: 7265 2044 6576 656c 6f70 6d65 6e74 203a  re Development :
+00000360: 3a20 4c69 6272 6172 6965 7320 3a3a 2050  : Libraries :: P
+00000370: 7974 686f 6e20 4d6f 6475 6c65 730a 436c  ython Modules.Cl
+00000380: 6173 7369 6669 6572 3a20 546f 7069 6320  assifier: Topic 
+00000390: 3a3a 2053 6f66 7477 6172 6520 4465 7665  :: Software Deve
+000003a0: 6c6f 706d 656e 7420 3a3a 2055 7365 7220  lopment :: User 
+000003b0: 496e 7465 7266 6163 6573 0a52 6571 7569  Interfaces.Requi
+000003c0: 7265 732d 5079 7468 6f6e 3a20 3e3d 332e  res-Python: >=3.
+000003d0: 380a 4465 7363 7269 7074 696f 6e2d 436f  8.Description-Co
+000003e0: 6e74 656e 742d 5479 7065 3a20 7465 7874  ntent-Type: text
+000003f0: 2f6d 6172 6b64 6f77 6e0a 4c69 6365 6e73  /markdown.Licens
+00000400: 652d 4669 6c65 3a20 4c49 4345 4e53 450a  e-File: LICENSE.
+00000410: 0a23 203a 6c6f 636b 3a20 7374 2d6c 6f67  .# :lock: st-log
+00000420: 696e 2d66 6f72 6d0a 5b21 5b44 6f77 6e6c  in-form.[![Downl
+00000430: 6f61 6473 5d28 6874 7470 733a 2f2f 7374  oads](https://st
+00000440: 6174 6963 2e70 6570 792e 7465 6368 2f70  atic.pepy.tech/p
+00000450: 6572 736f 6e61 6c69 7a65 642d 6261 6467  ersonalized-badg
+00000460: 652f 7374 2d6c 6f67 696e 2d66 6f72 6d3f  e/st-login-form?
+00000470: 7065 7269 6f64 3d74 6f74 616c 2675 6e69  period=total&uni
+00000480: 7473 3d69 6e74 6572 6e61 7469 6f6e 616c  ts=international
+00000490: 5f73 7973 7465 6d26 6c65 6674 5f63 6f6c  _system&left_col
+000004a0: 6f72 3d62 6c61 636b 2672 6967 6874 5f63  or=black&right_c
+000004b0: 6f6c 6f72 3d62 7269 6768 7467 7265 656e  olor=brightgreen
+000004c0: 266c 6566 745f 7465 7874 3d44 6f77 6e6c  &left_text=Downl
+000004d0: 6f61 6473 295d 2868 7474 7073 3a2f 2f70  oads)](https://p
+000004e0: 6570 792e 7465 6368 2f70 726f 6a65 6374  epy.tech/project
+000004f0: 2f73 742d 6c6f 6769 6e2d 666f 726d 290a  /st-login-form).
+00000500: 0a41 2073 7472 6561 6d6c 6974 2063 6f6d  .A streamlit com
+00000510: 706f 6e65 6e74 2074 6861 7420 6372 6561  ponent that crea
+00000520: 7465 7320 6120 7573 6572 206c 6f67 696e  tes a user login
+00000530: 2066 6f72 6d20 636f 6e6e 6563 7465 6420   form connected 
+00000540: 746f 2061 2053 7570 6162 6173 6520 4442  to a Supabase DB
+00000550: 2e20 4974 206c 6574 7320 7573 6572 7320  . It lets users 
+00000560: 6372 6561 7465 2061 206e 6577 2075 7365  create a new use
+00000570: 726e 616d 6520 616e 6420 7061 7373 776f  rname and passwo
+00000580: 7264 2c20 6c6f 6769 6e20 746f 2061 6e20  rd, login to an 
+00000590: 6578 6973 7469 6e67 2061 6363 6f75 6e74  existing account
+000005a0: 2c20 6f72 206c 6f67 696e 2061 7320 616e  , or login as an
+000005b0: 2061 6e6f 6e79 6d6f 7573 2067 7565 7374   anonymous guest
+000005c0: 2e0a 0a21 5b46 6f72 6d20 7363 7265 656e  ...![Form screen
+000005d0: 7368 6f74 5d28 6173 7365 7473 2f73 6372  shot](assets/scr
+000005e0: 6565 6e73 686f 742e 706e 6729 0a0a 5468  eenshot.png)..Th
+000005f0: 6520 6c6f 6769 6e20 666f 726d 2063 6f6c  e login form col
+00000600: 6c61 7073 6573 2061 6674 6572 206c 6f67  lapses after log
+00000610: 696e 2074 6f20 6672 6565 2073 6372 6565  in to free scree
+00000620: 6e2d 7370 6163 652e 0a0a 2323 203a 636f  n-space...## :co
+00000630: 6d70 7574 6572 3a20 4465 6d6f 2061 7070  mputer: Demo app
+00000640: 0a5b 215b 4f70 656e 2069 6e20 5374 7265  .[![Open in Stre
+00000650: 616d 6c69 745d 2868 7474 7073 3a2f 2f73  amlit](https://s
+00000660: 7461 7469 632e 7374 7265 616d 6c69 742e  tatic.streamlit.
+00000670: 696f 2f62 6164 6765 732f 7374 7265 616d  io/badges/stream
+00000680: 6c69 745f 6261 6467 655f 626c 6163 6b5f  lit_badge_black_
+00000690: 7768 6974 652e 7376 6729 5d28 6874 7470  white.svg)](http
+000006a0: 733a 2f2f 7374 2d6c 676e 2d66 6f72 6d2e  s://st-lgn-form.
+000006b0: 7374 7265 616d 6c69 742e 6170 702f 290a  streamlit.app/).
+000006c0: 0a23 2320 3a63 6f6e 7374 7275 6374 696f  .## :constructio
+000006d0: 6e3a 2049 6e73 7461 6c6c 6174 696f 6e20  n: Installation 
+000006e0: 0a0a 312e 2049 6e73 7461 6c6c 2060 7374  ..1. Install `st
+000006f0: 2d6c 6f67 696e 2d66 6f72 6d60 200a 6060  -login-form` .``
+00000700: 6073 680a 7069 7020 696e 7374 616c 6c20  `sh.pip install 
+00000710: 7374 2d6c 6f67 696e 2d66 6f72 6d0a 6060  st-login-form.``
+00000720: 600a 322e 2043 7265 6174 6520 6120 5375  `.2. Create a Su
+00000730: 7061 6261 7365 2070 726f 6a65 6374 2061  pabase project a
+00000740: 7320 6d65 6e74 696f 6e65 6420 5b68 6572  s mentioned [her
+00000750: 655d 2868 7474 7073 3a2f 2f64 6f63 732e  e](https://docs.
+00000760: 7374 7265 616d 6c69 742e 696f 2f6b 6e6f  streamlit.io/kno
+00000770: 776c 6564 6765 2d62 6173 652f 7475 746f  wledge-base/tuto
+00000780: 7269 616c 732f 6461 7461 6261 7365 732f  rials/databases/
+00000790: 7375 7061 6261 7365 2373 6967 6e2d 696e  supabase#sign-in
+000007a0: 2d74 6f2d 7375 7061 6261 7365 2d61 6e64  -to-supabase-and
+000007b0: 2d63 7265 6174 652d 612d 7072 6f6a 6563  -create-a-projec
+000007c0: 7429 0a33 2e20 4372 6561 7465 2061 2074  t).3. Create a t
+000007d0: 6162 6c65 2074 6f20 7374 6f72 6520 7468  able to store th
+000007e0: 6520 7573 6572 6e61 6d65 7320 616e 6420  e usernames and 
+000007f0: 7061 7373 776f 7264 732e 2054 6865 2074  passwords. The t
+00000800: 6162 6c65 206e 616d 6520 616e 6420 636f  able name and co
+00000810: 6c75 6d6e 206e 616d 6573 2063 616e 2062  lumn names can b
+00000820: 6520 6173 2070 6572 2079 6f75 7220 6368  e as per your ch
+00000830: 6f69 6365 2e0a 6060 6073 716c 0a43 5245  oice..```sql.CRE
+00000840: 4154 4520 5441 424c 4520 7573 6572 7320  ATE TABLE users 
+00000850: 280a 2020 2020 7573 6572 6e61 6d65 2074  (.    username t
+00000860: 6578 7420 6e6f 7420 6e75 6c6c 2064 6566  ext not null def
+00000870: 6175 6c74 2027 273a 3a74 6578 742c 0a20  ault ''::text,. 
+00000880: 2020 2070 6173 7377 6f72 6420 7465 7874     password text
+00000890: 206e 6f74 206e 756c 6c2c 0a20 2020 2063   not null,.    c
+000008a0: 6f6e 7374 7261 696e 7420 7573 6572 735f  onstraint users_
+000008b0: 706b 6579 2070 7269 6d61 7279 206b 6579  pkey primary key
+000008c0: 2028 7573 6572 6e61 6d65 292c 0a20 2020   (username),.   
+000008d0: 2063 6f6e 7374 7261 696e 7420 7573 6572   constraint user
+000008e0: 735f 7573 6572 6e61 6d65 5f6b 6579 2075  s_username_key u
+000008f0: 6e69 7175 6520 2875 7365 726e 616d 6529  nique (username)
+00000900: 2c0a 2020 2020 636f 6e73 7472 6169 6e74  ,.    constraint
+00000910: 2075 7365 7273 5f70 6173 7377 6f72 645f   users_password_
+00000920: 6368 6563 6b20 6368 6563 6b20 280a 2020  check check (.  
+00000930: 2020 2020 280a 2020 2020 2020 2020 6c65      (.        le
+00000940: 6e67 7468 280a 2020 2020 2020 2020 2020  ngth(.          
+00000950: 7472 696d 280a 2020 2020 2020 2020 2020  trim(.          
+00000960: 2020 626f 7468 0a20 2020 2020 2020 2020    both.         
+00000970: 2020 2066 726f 6d0a 2020 2020 2020 2020     from.        
+00000980: 2020 2020 2020 7061 7373 776f 7264 0a20        password. 
+00000990: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+000009a0: 2020 2029 203e 2031 0a20 2020 2020 2029     ) > 1.      )
+000009b0: 0a20 2020 2029 2c0a 2020 2020 636f 6e73  .    ),.    cons
+000009c0: 7472 6169 6e74 2075 7365 7273 5f75 7365  traint users_use
+000009d0: 726e 616d 655f 6368 6563 6b20 6368 6563  rname_check chec
+000009e0: 6b20 280a 2020 2020 2020 280a 2020 2020  k (.      (.    
+000009f0: 2020 2020 6c65 6e67 7468 280a 2020 2020      length(.    
+00000a00: 2020 2020 2020 7472 696d 280a 2020 2020        trim(.    
+00000a10: 2020 2020 2020 2020 626f 7468 0a20 2020          both.   
+00000a20: 2020 2020 2020 2020 2066 726f 6d0a 2020           from.  
+00000a30: 2020 2020 2020 2020 2020 2020 7573 6572              user
+00000a40: 6e61 6d65 0a20 2020 2020 2020 2020 2029  name.          )
+00000a50: 0a20 2020 2020 2020 2029 203e 2031 0a20  .        ) > 1. 
+00000a60: 2020 2020 2029 0a20 2020 2029 0a20 2029       ).    ).  )
+00000a70: 2074 6162 6c65 7370 6163 6520 7067 5f64   tablespace pg_d
+00000a80: 6566 6175 6c74 3b0a 6060 600a 342e 2046  efault;.```.4. F
+00000a90: 6f6c 6c6f 7720 7468 6520 7265 7374 206f  ollow the rest o
+00000aa0: 6620 7468 6520 7374 6570 7320 6672 6f6d  f the steps from
+00000ab0: 205b 6865 7265 5d28 6874 7470 733a 2f2f   [here](https://
+00000ac0: 646f 6373 2e73 7472 6561 6d6c 6974 2e69  docs.streamlit.i
+00000ad0: 6f2f 6b6e 6f77 6c65 6467 652d 6261 7365  o/knowledge-base
+00000ae0: 2f74 7574 6f72 6961 6c73 2f64 6174 6162  /tutorials/datab
+00000af0: 6173 6573 2f73 7570 6162 6173 6523 636f  ases/supabase#co
+00000b00: 7079 2d79 6f75 722d 6170 702d 7365 6372  py-your-app-secr
+00000b10: 6574 732d 746f 2d74 6865 2d63 6c6f 7564  ets-to-the-cloud
+00000b20: 2920 746f 2063 6f6e 6e65 6374 2079 6f75  ) to connect you
+00000b30: 7220 5374 7265 616d 6c69 7420 6170 7020  r Streamlit app 
+00000b40: 746f 2053 7570 6162 6173 650a 0a0a 2323  to Supabase...##
+00000b50: 203a 7065 6e3a 2055 7361 6765 0a0a 606c   :pen: Usage..`l
+00000b60: 6f67 696e 5f66 6f72 6d28 2960 2073 6574  ogin_form()` set
+00000b70: 7320 6073 6573 7369 6f6e 5f73 7461 7465  s `session_state
+00000b80: 5b22 6175 7468 656e 7469 6361 7465 6422  ["authenticated"
+00000b90: 5d60 2074 6f20 6054 7275 6560 2069 6620  ]` to `True` if 
+00000ba0: 7468 6520 6c6f 6769 6e20 6973 2073 7563  the login is suc
+00000bb0: 6365 7373 6675 6c2c 2060 7365 7373 696f  cessful, `sessio
+00000bc0: 6e5f 7374 6174 655b 2275 7365 726e 616d  n_state["usernam
+00000bd0: 6522 5d60 2074 6f20 7468 6520 6075 7365  e"]` to the `use
+00000be0: 726e 616d 6560 206f 7220 6e65 7720 6f72  rname` or new or
+00000bf0: 2065 7869 7374 696e 6720 7573 6572 2c20   existing user, 
+00000c00: 616e 6420 746f 2060 4e6f 6e65 6020 666f  and to `None` fo
+00000c10: 7220 6775 6573 7420 6c6f 6769 6e2e 0a0a  r guest login...
+00000c20: 5265 7475 726e 7320 7468 6520 696e 6974  Returns the init
+00000c30: 6961 6c69 7a65 6420 6073 7570 6162 6173  ialized `supabas
+00000c40: 652e 436c 6965 6e74 6020 696e 7374 616e  e.Client` instan
+00000c50: 6365 2074 6f20 6c65 7420 796f 7520 696e  ce to let you in
+00000c60: 7465 7261 6374 2077 6974 6820 7468 6520  teract with the 
+00000c70: 6461 7461 6273 6520 646f 776e 7374 7265  databse downstre
+00000c80: 616d 2069 6e20 7468 6520 7363 7269 7074  am in the script
+00000c90: 2e0a 0a60 6060 7079 7468 6f6e 0a69 6d70  ...```python.imp
+00000ca0: 6f72 7420 7374 7265 616d 6c69 7420 6173  ort streamlit as
+00000cb0: 2073 740a 0a66 726f 6d20 7374 7265 616d   st..from stream
+00000cc0: 6c69 745f 6c6f 6769 6e20 696d 706f 7274  lit_login import
+00000cd0: 206c 6f67 696e 5f66 6f72 6d0a 0a63 6c69   login_form..cli
+00000ce0: 656e 7420 3d20 6c6f 6769 6e5f 666f 726d  ent = login_form
+00000cf0: 2829 0a0a 6966 2073 742e 7365 7373 696f  ()..if st.sessio
+00000d00: 6e5f 7374 6174 655b 2261 7574 6865 6e74  n_state["authent
+00000d10: 6963 6174 6564 225d 3a0a 2020 2020 6966  icated"]:.    if
+00000d20: 2073 742e 7365 7373 696f 6e5f 7374 6174   st.session_stat
+00000d30: 655b 2275 7365 726e 616d 6522 5d3a 0a20  e["username"]:. 
+00000d40: 2020 2020 2020 2073 742e 7375 6363 6573         st.succes
+00000d50: 7328 6622 5765 6c63 6f6d 6520 7b73 742e  s(f"Welcome {st.
+00000d60: 7365 7373 696f 6e5f 7374 6174 655b 2775  session_state['u
+00000d70: 7365 726e 616d 6527 5d7d 2229 0a20 2020  sername']}").   
+00000d80: 2065 6c73 653a 0a20 2020 2020 2020 2073   else:.        s
+00000d90: 742e 7375 6363 6573 7328 2257 656c 636f  t.success("Welco
+00000da0: 6d65 2067 7565 7374 2229 0a65 6c73 653a  me guest").else:
+00000db0: 0a20 2020 2073 742e 6572 726f 7228 224e  .    st.error("N
+00000dc0: 6f74 2061 7574 6865 6e74 6963 6174 6564  ot authenticated
+00000dd0: 2229 0a60 6060 0a0a 5b21 5b53 6565 2064  ").```..[![See d
+00000de0: 656d 6f20 696e 2053 7472 6561 6d6c 6974  emo in Streamlit
+00000df0: 5d28 6874 7470 733a 2f2f 7374 6174 6963  ](https://static
+00000e00: 2e73 7472 6561 6d6c 6974 2e69 6f2f 6261  .streamlit.io/ba
+00000e10: 6467 6573 2f73 7472 6561 6d6c 6974 5f62  dges/streamlit_b
+00000e20: 6164 6765 5f62 6c61 636b 5f77 6869 7465  adge_black_white
+00000e30: 2e73 7667 295d 2868 7474 7073 3a2f 2f73  .svg)](https://s
+00000e40: 742d 6c67 6e2d 666f 726d 2e73 7472 6561  t-lgn-form.strea
+00000e50: 6d6c 6974 2e61 7070 2f29 0a0a 2323 20f0  mlit.app/)..## .
+00000e60: 9fa4 9720 5761 6e74 2074 6f20 7375 7070  ... Want to supp
+00000e70: 6f72 7420 6d79 2077 6f72 6b3f 0a3c 7020  ort my work?.<p 
+00000e80: 616c 6967 6e3d 2263 656e 7465 7222 3e0a  align="center">.
+00000e90: 2020 2020 3c61 2068 7265 663d 2268 7474      <a href="htt
+00000ea0: 7073 3a2f 2f77 7777 2e62 7579 6d65 6163  ps://www.buymeac
+00000eb0: 6f66 6665 652e 636f 6d2f 7369 6464 6861  offee.com/siddha
+00000ec0: 6e74 7361 6461 6e67 6922 2074 6172 6765  ntsadangi" targe
+00000ed0: 743d 225f 626c 616e 6b22 3e3c 696d 6720  t="_blank"><img 
+00000ee0: 7372 633d 2268 7474 7073 3a2f 2f63 646e  src="https://cdn
+00000ef0: 2e62 7579 6d65 6163 6f66 6665 652e 636f  .buymeacoffee.co
+00000f00: 6d2f 6275 7474 6f6e 732f 7632 2f64 6566  m/buttons/v2/def
+00000f10: 6175 6c74 2d79 656c 6c6f 772e 706e 6722  ault-yellow.png"
+00000f20: 2061 6c74 3d22 4275 7920 4d65 2041 2043   alt="Buy Me A C
+00000f30: 6f66 6665 6522 2073 7479 6c65 3d22 6865  offee" style="he
+00000f40: 6967 6874 3a20 3630 7078 2021 696d 706f  ight: 60px !impo
+00000f50: 7274 616e 743b 7769 6474 683a 2032 3137  rtant;width: 217
+00000f60: 7078 2021 696d 706f 7274 616e 743b 223e  px !important;">
+00000f70: 0a20 2020 203c 2f61 3e0a 3c2f 703e 0a    .    </a>.</p>.
```

