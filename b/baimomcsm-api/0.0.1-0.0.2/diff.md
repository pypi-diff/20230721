# Comparing `tmp/baimomcsm_api-0.0.1.tar.gz` & `tmp/baimomcsm_api-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\baimomcsm_api-0.0.1.tar", last modified: Fri Jul 21 05:36:17 2023, max compression
+gzip compressed data, was "dist\baimomcsm_api-0.0.2.tar", last modified: Fri Jul 21 05:45:03 2023, max compression
```

## Comparing `baimomcsm_api-0.0.1.tar` & `baimomcsm_api-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-07-21 05:36:17.650361 baimomcsm_api-0.0.1/
--rw-rw-rw-   0        0        0    11558 2023-07-20 13:08:31.000000 baimomcsm_api-0.0.1/LICENSE
--rw-rw-rw-   0        0        0       26 2023-07-21 05:28:13.000000 baimomcsm_api-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2162 2023-07-21 05:36:17.650361 baimomcsm_api-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      873 2023-07-21 05:00:19.000000 baimomcsm_api-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-21 05:36:17.639557 baimomcsm_api-0.0.1/baimomcsm_api/
--rw-rw-rw-   0        0        0       45 2023-07-21 05:33:57.000000 baimomcsm_api-0.0.1/baimomcsm_api/__init__.py
--rw-rw-rw-   0        0        0     3278 2023-07-21 04:56:37.000000 baimomcsm_api-0.0.1/baimomcsm_api/applications.py
--rw-rw-rw-   0        0        0      196 2023-07-20 11:37:00.000000 baimomcsm_api-0.0.1/baimomcsm_api/baimomcsm_error.py
--rw-rw-rw-   0        0        0     2549 2023-07-20 12:36:12.000000 baimomcsm_api-0.0.1/baimomcsm_api/common.py
--rw-rw-rw-   0        0        0      183 2023-07-20 08:13:27.000000 baimomcsm_api-0.0.1/baimomcsm_api/log_writer.py
--rw-rw-rw-   0        0        0     1328 2023-07-20 12:07:25.000000 baimomcsm_api-0.0.1/baimomcsm_api/request_sender.py
-drwxrwxrwx   0        0        0        0 2023-07-21 05:36:17.650361 baimomcsm_api-0.0.1/baimomcsm_api.egg-info/
--rw-rw-rw-   0        0        0     2162 2023-07-21 05:36:17.000000 baimomcsm_api-0.0.1/baimomcsm_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      395 2023-07-21 05:36:17.000000 baimomcsm_api-0.0.1/baimomcsm_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 05:36:17.000000 baimomcsm_api-0.0.1/baimomcsm_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-21 05:36:17.000000 baimomcsm_api-0.0.1/baimomcsm_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-21 05:36:17.000000 baimomcsm_api-0.0.1/baimomcsm_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-21 05:36:17.650361 baimomcsm_api-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1514 2023-07-21 05:35:16.000000 baimomcsm_api-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 05:45:03.602219 baimomcsm_api-0.0.2/
+-rw-rw-rw-   0        0        0    11558 2023-07-20 13:08:31.000000 baimomcsm_api-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0       37 2023-07-21 05:42:37.000000 baimomcsm_api-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     2431 2023-07-21 05:45:03.602219 baimomcsm_api-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1105 2023-07-21 05:41:37.000000 baimomcsm_api-0.0.2/README.html
+-rw-rw-rw-   0        0        0      873 2023-07-21 05:00:19.000000 baimomcsm_api-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-21 05:45:03.592224 baimomcsm_api-0.0.2/baimomcsm_api/
+-rw-rw-rw-   0        0        0       45 2023-07-21 05:33:57.000000 baimomcsm_api-0.0.2/baimomcsm_api/__init__.py
+-rw-rw-rw-   0        0        0     3278 2023-07-21 04:56:37.000000 baimomcsm_api-0.0.2/baimomcsm_api/applications.py
+-rw-rw-rw-   0        0        0      196 2023-07-20 11:37:00.000000 baimomcsm_api-0.0.2/baimomcsm_api/baimomcsm_error.py
+-rw-rw-rw-   0        0        0     2549 2023-07-20 12:36:12.000000 baimomcsm_api-0.0.2/baimomcsm_api/common.py
+-rw-rw-rw-   0        0        0      183 2023-07-20 08:13:27.000000 baimomcsm_api-0.0.2/baimomcsm_api/log_writer.py
+-rw-rw-rw-   0        0        0     1328 2023-07-20 12:07:25.000000 baimomcsm_api-0.0.2/baimomcsm_api/request_sender.py
+drwxrwxrwx   0        0        0        0 2023-07-21 05:45:03.602219 baimomcsm_api-0.0.2/baimomcsm_api.egg-info/
+-rw-rw-rw-   0        0        0     2431 2023-07-21 05:45:03.000000 baimomcsm_api-0.0.2/baimomcsm_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      407 2023-07-21 05:45:03.000000 baimomcsm_api-0.0.2/baimomcsm_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 05:45:03.000000 baimomcsm_api-0.0.2/baimomcsm_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-21 05:45:03.000000 baimomcsm_api-0.0.2/baimomcsm_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-21 05:45:03.000000 baimomcsm_api-0.0.2/baimomcsm_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-21 05:45:03.602219 baimomcsm_api-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1516 2023-07-21 05:44:49.000000 baimomcsm_api-0.0.2/setup.py
```

### Comparing `baimomcsm_api-0.0.1/LICENSE` & `baimomcsm_api-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `baimomcsm_api-0.0.1/PKG-INFO` & `baimomcsm_api-0.0.2/baimomcsm_api.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,136 +1,152 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 312e 310d 0a4e 616d 653a 2062 6169  : 1.1..Name: bai
-00000020: 6d6f 6d63 736d 5f61 7069 0d0a 5665 7273  momcsm_api..Vers
-00000030: 696f 6e3a 2030 2e30 2e31 0d0a 5375 6d6d  ion: 0.0.1..Summ
+00000020: 6d6f 6d63 736d 2d61 7069 0d0a 5665 7273  momcsm-api..Vers
+00000030: 696f 6e3a 2030 2e30 2e32 0d0a 5375 6d6d  ion: 0.0.2..Summ
 00000040: 6172 793a 204d 4353 4d61 6e61 6765 7220  ary: MCSManager 
 00000050: 4150 4920 666f 7220 5079 7468 6f6e 2028  API for Python (
 00000060: e5bc 80e5 8f91 e4b8 ad29 0d0a 486f 6d65  .........)..Home
 00000070: 2d70 6167 653a 2068 7474 7073 3a2f 2f67  -page: https://g
 00000080: 6974 6875 622e 636f 6d2f 5a68 6f75 2d53  ithub.com/Zhou-S
 00000090: 6869 6c69 6e2f 4261 696d 6f4d 4353 4d61  hilin/BaimoMCSMa
 000000a0: 6e61 6765 722d 4150 490d 0a41 7574 686f  nager-API..Autho
 000000b0: 723a 2042 6169 6d6f 5169 6c69 6e0d 0a41  r: BaimoQilin..A
 000000c0: 7574 686f 722d 656d 6169 6c3a 2061 646d  uthor-email: adm
 000000d0: 696e 4062 6169 6d6f 7169 6c69 6e2e 746f  in@baimoqilin.to
 000000e0: 700d 0a4c 6963 656e 7365 3a20 4170 6163  p..License: Apac
 000000f0: 6865 2032 2e30 0d0a 4465 7363 7269 7074  he 2.0..Descript
-00000100: 696f 6e3a 2023 2042 6169 6d6f 4d43 534d  ion: # BaimoMCSM
-00000110: 616e 6167 6572 2041 5049 2066 6f72 2060  anager API for `
-00000120: 5079 7468 6f6e 600d 0a20 2020 2020 2020  Python`..       
-00000130: 205b 215b 5052 7320 7765 6c63 6f6d 655d   [![PRs welcome]
-00000140: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
-00000150: 656c 6473 2e69 6f2f 6261 6467 652f 5052  elds.io/badge/PR
-00000160: 732d 7765 6c63 6f6d 652d 3230 4246 3230  s-welcome-20BF20
-00000170: 295d 2868 7474 7073 3a2f 2f67 6974 6875  )](https://githu
-00000180: 622e 636f 6d2f 5a68 6f75 2d53 6869 6c69  b.com/Zhou-Shili
-00000190: 6e2f 4261 696d 6f4d 4353 4d61 6e61 6765  n/BaimoMCSManage
-000001a0: 722d 4150 492f 7075 6c6c 7329 0d0a 2020  r-API/pulls)..  
-000001b0: 2020 2020 2020 215b 5375 7070 6f72 7420        ![Support 
-000001c0: 4d53 434d 2039 2e39 2e30 5d28 6874 7470  MSCM 9.9.0](http
-000001d0: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
-000001e0: 696f 2f62 6164 6765 2f53 7570 706f 7274  io/badge/Support
-000001f0: 2d4d 4353 4d5f 392e 392e 302d 626c 7565  -MCSM_9.9.0-blue
-00000200: 290d 0a20 2020 2020 2020 2021 5b41 7061  )..        ![Apa
-00000210: 6368 6520 4c69 6365 6e73 655d 2868 7474  che License](htt
-00000220: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
-00000230: 2e69 6f2f 6261 6467 652f 4c69 6365 6e73  .io/badge/Licens
-00000240: 652d 4170 6163 6865 2d72 6564 2920 200d  e-Apache-red)  .
-00000250: 0a20 2020 2020 2020 20e8 bf99 e698 afe4  .        .......
-00000260: b880 e4b8 aae9 8082 e794 a8e4 ba8e 5079  ..............Py
-00000270: 7468 6f6e e8af ade8 a880 e79a 84e7 acac  thon............
-00000280: e4b8 89e6 96b9 e5ba 93ef bc8c e8ae a9e4  ................
-00000290: bda0 e59c a850 7974 686f 6ee4 b8ad e69b  .....Python.....
-000002a0: b4e6 96b9 e4be bfe5 9cb0 e8b0 83e7 94a8  ................
-000002b0: 5b4d 4353 4d2d 4150 490d 0a20 2020 2020  [MCSM-API..     
-000002c0: 2020 205d 2868 7474 7073 3a2f 2f64 6f63     ](https://doc
-000002d0: 732e 6d63 736d 616e 6167 6572 2e63 6f6d  s.mcsmanager.com
-000002e0: 2f23 2f7a 682d 636e 2f61 7069 732f 7265  /#/zh-cn/apis/re
-000002f0: 6164 6d65 29e7 aea1 e790 86e4 bda0 e79a  adme)...........
-00000300: 84e6 9c8d e58a a1e5 99a8 e380 820d 0a20  ............... 
-00000310: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00000320: 2023 2320 e29a a0ef b88f e6b3 a8e6 848f   ## ............
-00000330: 0d0a 2020 2020 2020 2020 e8bf 99e4 b8aa  ..        ......
-00000340: e9a1 b9e7 9bae e4bb 8de5 9ca8 e5bc 80e5  ................
-00000350: 8f91 e4b8 adef bc8c e4bb 85e6 94af e68c  ................
-00000360: 81e9 83a8 e588 86e5 8a9f e883 bde3 8082  ................
-00000370: 2020 0d0a 2020 2020 2020 2020 2020 0d0a    ..          ..
-00000380: 2020 2020 2020 2020 e5bd 93e5 898d e8bf          ........
-00000390: 9be5 b195 efbc 9a0d 0a20 2020 2020 2020  .........       
-000003a0: 2020 2d20 5b78 5d20 e99d a2e6 9dbf e980    - [x] ........
-000003b0: 9ae7 94a8 e8ae bee7 bdae 2028 2060 636f  .......... ( `co
-000003c0: 6d6d 6f6e 2e70 7960 290d 0a20 2020 2020  mmon.py`)..     
-000003d0: 2020 2020 2d20 5b78 5d20 e5ba 94e7 94a8      - [x] ......
-000003e0: e5ae 9ee4 be8b e7ae a1e7 9086 2028 6061  ............ (`a
-000003f0: 7070 6c69 6361 7469 6f6e 732e 7079 6029  pplications.py`)
-00000400: 0d0a 2020 2020 2020 2020 202d 205b 205d  ..         - [ ]
-00000410: 20e5 ae9e e4be 8be6 9687 e4bb b6e7 aea1   ...............
-00000420: e790 8620 2860 6669 6c65 732e 7079 6029  ... (`files.py`)
-00000430: 0d0a 2020 2020 2020 2020 202d 205b 205d  ..         - [ ]
-00000440: 20e8 aea1 e588 92e4 bbbb e58a a1e7 aea1   ...............
-00000450: e790 8620 2860 706c 616e 732e 7079 6029  ... (`plans.py`)
-00000460: 0d0a 2020 2020 2020 2020 202d 205b 205d  ..         - [ ]
-00000470: 20e5 ae88 e68a a4e8 bf9b e7a8 8be7 aea1   ...............
-00000480: e790 8620 2820 6072 656d 6f74 655f 7365  ... ( `remote_se
-00000490: 7276 6963 652e 7079 6029 0d0a 2020 2020  rvice.py`)..    
-000004a0: 2020 2020 202d 205b 205d 20e5 a49a e794       - [ ] .....
-000004b0: a8e6 88b7 e7ae a1e7 9086 2028 6061 7574  .......... (`aut
-000004c0: 682e 7079 6029 0d0a 2020 2020 2020 2020  h.py`)..        
-000004d0: 0d0a 2020 2020 2020 2020 2323 20f0 9f93  ..        ## ...
-000004e0: 96e4 bdbf e794 a8e6 96b9 e6b3 950d 0a20  ............... 
-000004f0: 2020 2020 2020 20e6 96bd e5b7 a5e4 b8ad         .........
-00000500: e280 a6e2 80a6 0d0a 506c 6174 666f 726d  ........Platform
-00000510: 3a20 616c 6c0d 0a43 6c61 7373 6966 6965  : all..Classifie
-00000520: 723a 2049 6e74 656e 6465 6420 4175 6469  r: Intended Audi
-00000530: 656e 6365 203a 3a20 4465 7665 6c6f 7065  ence :: Develope
-00000540: 7273 0d0a 436c 6173 7369 6669 6572 3a20  rs..Classifier: 
-00000550: 4f70 6572 6174 696e 6720 5379 7374 656d  Operating System
-00000560: 203a 3a20 4f53 2049 6e64 6570 656e 6465   :: OS Independe
-00000570: 6e74 0d0a 436c 6173 7369 6669 6572 3a20  nt..Classifier: 
-00000580: 4e61 7475 7261 6c20 4c61 6e67 7561 6765  Natural Language
-00000590: 203a 3a20 4368 696e 6573 6520 2853 696d   :: Chinese (Sim
-000005a0: 706c 6966 6965 6429 0d0a 436c 6173 7369  plified)..Classi
-000005b0: 6669 6572 3a20 5072 6f67 7261 6d6d 696e  fier: Programmin
-000005c0: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-000005d0: 7468 6f6e 0d0a 436c 6173 7369 6669 6572  thon..Classifier
-000005e0: 3a20 5072 6f67 7261 6d6d 696e 6720 4c61  : Programming La
-000005f0: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-00000600: 203a 3a20 330d 0a43 6c61 7373 6966 6965   :: 3..Classifie
-00000610: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
-00000620: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
-00000630: 6e20 3a3a 2033 2e31 0d0a 436c 6173 7369  n :: 3.1..Classi
-00000640: 6669 6572 3a20 5072 6f67 7261 6d6d 696e  fier: Programmin
-00000650: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-00000660: 7468 6f6e 203a 3a20 332e 320d 0a43 6c61  thon :: 3.2..Cla
-00000670: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
-00000680: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-00000690: 2050 7974 686f 6e20 3a3a 2033 2e33 0d0a   Python :: 3.3..
-000006a0: 436c 6173 7369 6669 6572 3a20 5072 6f67  Classifier: Prog
-000006b0: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
-000006c0: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
-000006d0: 340d 0a43 6c61 7373 6966 6965 723a 2050  4..Classifier: P
-000006e0: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-000006f0: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
-00000700: 2033 2e35 0d0a 436c 6173 7369 6669 6572   3.5..Classifier
-00000710: 3a20 5072 6f67 7261 6d6d 696e 6720 4c61  : Programming La
-00000720: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-00000730: 203a 3a20 332e 360d 0a43 6c61 7373 6966   :: 3.6..Classif
-00000740: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
-00000750: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
-00000760: 686f 6e20 3a3a 2033 2e37 0d0a 436c 6173  hon :: 3.7..Clas
-00000770: 7369 6669 6572 3a20 5072 6f67 7261 6d6d  sifier: Programm
-00000780: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
-00000790: 5079 7468 6f6e 203a 3a20 332e 380d 0a43  Python :: 3.8..C
-000007a0: 6c61 7373 6966 6965 723a 2050 726f 6772  lassifier: Progr
-000007b0: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
-000007c0: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e39  :: Python :: 3.9
-000007d0: 0d0a 436c 6173 7369 6669 6572 3a20 5072  ..Classifier: Pr
-000007e0: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-000007f0: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-00000800: 332e 3130 0d0a 436c 6173 7369 6669 6572  3.10..Classifier
-00000810: 3a20 5072 6f67 7261 6d6d 696e 6720 4c61  : Programming La
-00000820: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-00000830: 203a 3a20 332e 3131 0d0a 436c 6173 7369   :: 3.11..Classi
-00000840: 6669 6572 3a20 546f 7069 6320 3a3a 2053  fier: Topic :: S
-00000850: 6f66 7477 6172 6520 4465 7665 6c6f 706d  oftware Developm
-00000860: 656e 7420 3a3a 204c 6962 7261 7269 6573  ent :: Libraries
-00000870: 0d0a                                     ..
+00000100: 696f 6e3a 203c 6831 2069 643d 2262 6169  ion: <h1 id="bai
+00000110: 6d6f 6d63 736d 616e 6167 6572 2d61 7069  momcsmanager-api
+00000120: 2d66 6f72 2d70 7974 686f 6e22 3e42 6169  -for-python">Bai
+00000130: 6d6f 4d43 534d 616e 6167 6572 2041 5049  moMCSManager API
+00000140: 2066 6f72 0d0a 2020 2020 2020 2020 3c63   for..        <c
+00000150: 6f64 653e 5079 7468 6f6e 3c2f 636f 6465  ode>Python</code
+00000160: 3e3c 2f68 313e 0d0a 2020 2020 2020 2020  ></h1>..        
+00000170: 3c70 3e3c 610d 0a20 2020 2020 2020 2068  <p><a..        h
+00000180: 7265 663d 2268 7474 7073 3a2f 2f67 6974  ref="https://git
+00000190: 6875 622e 636f 6d2f 5a68 6f75 2d53 6869  hub.com/Zhou-Shi
+000001a0: 6c69 6e2f 4261 696d 6f4d 4353 4d61 6e61  lin/BaimoMCSMana
+000001b0: 6765 722d 4150 492f 7075 6c6c 7322 3e3c  ger-API/pulls"><
+000001c0: 696d 670d 0a20 2020 2020 2020 2073 7263  img..        src
+000001d0: 3d22 6874 7470 733a 2f2f 696d 672e 7368  ="https://img.sh
+000001e0: 6965 6c64 732e 696f 2f62 6164 6765 2f50  ields.io/badge/P
+000001f0: 5273 2d77 656c 636f 6d65 2d32 3042 4632  Rs-welcome-20BF2
+00000200: 3022 0d0a 2020 2020 2020 2020 616c 743d  0"..        alt=
+00000210: 2250 5273 2077 656c 636f 6d65 2220 2f3e  "PRs welcome" />
+00000220: 3c2f 613e 203c 696d 670d 0a20 2020 2020  </a> <img..     
+00000230: 2020 2073 7263 3d22 6874 7470 733a 2f2f     src="https://
+00000240: 696d 672e 7368 6965 6c64 732e 696f 2f62  img.shields.io/b
+00000250: 6164 6765 2f53 7570 706f 7274 2d4d 4353  adge/Support-MCS
+00000260: 4d5f 392e 392e 302d 626c 7565 220d 0a20  M_9.9.0-blue".. 
+00000270: 2020 2020 2020 2061 6c74 3d22 5375 7070         alt="Supp
+00000280: 6f72 7420 4d53 434d 2039 2e39 2e30 2220  ort MSCM 9.9.0" 
+00000290: 2f3e 203c 696d 670d 0a20 2020 2020 2020  /> <img..       
+000002a0: 2073 7263 3d22 6874 7470 733a 2f2f 696d   src="https://im
+000002b0: 672e 7368 6965 6c64 732e 696f 2f62 6164  g.shields.io/bad
+000002c0: 6765 2f4c 6963 656e 7365 2d41 7061 6368  ge/License-Apach
+000002d0: 652d 7265 6422 0d0a 2020 2020 2020 2020  e-red"..        
+000002e0: 616c 743d 2241 7061 6368 6520 4c69 6365  alt="Apache Lice
+000002f0: 6e73 6522 202f 3e3c 6272 202f 3e0d 0a20  nse" /><br />.. 
+00000300: 2020 2020 2020 20e8 bf99 e698 afe4 b880         .........
+00000310: e4b8 aae9 8082 e794 a8e4 ba8e 5079 7468  ............Pyth
+00000320: 6f6e e8af ade8 a880 e79a 84e7 acac e4b8  on..............
+00000330: 89e6 96b9 e5ba 93ef bc8c e8ae a9e4 bda0  ................
+00000340: e59c a850 7974 686f 6ee4 b8ad e69b b4e6  ...Python.......
+00000350: 96b9 e4be bfe5 9cb0 e8b0 83e7 94a8 3c61  ..............<a
+00000360: 0d0a 2020 2020 2020 2020 6872 6566 3d22  ..        href="
+00000370: 6874 7470 733a 2f2f 646f 6373 2e6d 6373  https://docs.mcs
+00000380: 6d61 6e61 6765 722e 636f 6d2f 232f 7a68  manager.com/#/zh
+00000390: 2d63 6e2f 6170 6973 2f72 6561 646d 6522  -cn/apis/readme"
+000003a0: 3e4d 4353 4d2d 4150 493c 2f61 3ee7 aea1  >MCSM-API</a>...
+000003b0: e790 86e4 bda0 e79a 84e6 9c8d e58a a1e5  ................
+000003c0: 99a8 e380 823c 2f70 3e0d 0a20 2020 2020  .....</p>..     
+000003d0: 2020 203c 6832 2069 643d 22e6 b3a8 e684     <h2 id=".....
+000003e0: 8f22 3ee2 9aa0 efb8 8fe6 b3a8 e684 8f3c  .">............<
+000003f0: 2f68 323e 0d0a 2020 2020 2020 2020 3c70  /h2>..        <p
+00000400: 3ee8 bf99 e4b8 aae9 a1b9 e79b aee4 bb8d  >...............
+00000410: e59c a8e5 bc80 e58f 91e4 b8ad efbc 8ce4  ................
+00000420: bb85 e694 afe6 8c81 e983 a8e5 8886 e58a  ................
+00000430: 9fe8 83bd e380 823c 2f70 3e0d 0a20 2020  .......</p>..   
+00000440: 2020 2020 203c 703e e5bd 93e5 898d e8bf       <p>........
+00000450: 9be5 b195 efbc 9a20 2d20 5b78 5d20 e99d  ....... - [x] ..
+00000460: a2e6 9dbf e980 9ae7 94a8 e8ae bee7 bdae  ................
+00000470: 2028 203c 636f 6465 3e63 6f6d 6d6f 6e2e   ( <code>common.
+00000480: 7079 3c2f 636f 6465 3e29 202d 205b 785d  py</code>) - [x]
+00000490: 0d0a 2020 2020 2020 2020 e5ba 94e7 94a8  ..        ......
+000004a0: e5ae 9ee4 be8b e7ae a1e7 9086 2028 3c63  ............ (<c
+000004b0: 6f64 653e 6170 706c 6963 6174 696f 6e73  ode>applications
+000004c0: 2e70 793c 2f63 6f64 653e 2920 2d20 5b20  .py</code>) - [ 
+000004d0: 5d20 e5ae 9ee4 be8b e696 87e4 bbb6 e7ae  ] ..............
+000004e0: a1e7 9086 0d0a 2020 2020 2020 2020 283c  ......        (<
+000004f0: 636f 6465 3e66 696c 6573 2e70 793c 2f63  code>files.py</c
+00000500: 6f64 653e 2920 2d20 5b20 5d20 e8ae a1e5  ode>) - [ ] ....
+00000510: 8892 e4bb bbe5 8aa1 e7ae a1e7 9086 2028  .............. (
+00000520: 3c63 6f64 653e 706c 616e 732e 7079 3c2f  <code>plans.py</
+00000530: 636f 6465 3e29 202d 205b 205d 0d0a 2020  code>) - [ ]..  
+00000540: 2020 2020 2020 e5ae 88e6 8aa4 e8bf 9be7        ..........
+00000550: a88b e7ae a1e7 9086 2028 203c 636f 6465  ........ ( <code
+00000560: 3e72 656d 6f74 655f 7365 7276 6963 652e  >remote_service.
+00000570: 7079 3c2f 636f 6465 3e29 202d 205b 205d  py</code>) - [ ]
+00000580: 20e5 a49a e794 a8e6 88b7 e7ae a1e7 9086   ...............
+00000590: 0d0a 2020 2020 2020 2020 283c 636f 6465  ..        (<code
+000005a0: 3e61 7574 682e 7079 3c2f 636f 6465 3e29  >auth.py</code>)
+000005b0: 3c2f 703e 0d0a 2020 2020 2020 2020 3c68  </p>..        <h
+000005c0: 3220 6964 3d22 e4bd bfe7 94a8 e696 b9e6  2 id="..........
+000005d0: b395 223e f09f 9396 e4bd bfe7 94a8 e696  ..">............
+000005e0: b9e6 b395 3c2f 6832 3e0d 0a20 2020 2020  ....</h2>..     
+000005f0: 2020 203c 703e e696 bde5 b7a5 e4b8 ade2     <p>..........
+00000600: 80a6 e280 a63c 2f70 3e0d 0a20 2020 2020  .....</p>..     
+00000610: 2020 200d 0a50 6c61 7466 6f72 6d3a 2061     ..Platform: a
+00000620: 6c6c 0d0a 436c 6173 7369 6669 6572 3a20  ll..Classifier: 
+00000630: 496e 7465 6e64 6564 2041 7564 6965 6e63  Intended Audienc
+00000640: 6520 3a3a 2044 6576 656c 6f70 6572 730d  e :: Developers.
+00000650: 0a43 6c61 7373 6966 6965 723a 204f 7065  .Classifier: Ope
+00000660: 7261 7469 6e67 2053 7973 7465 6d20 3a3a  rating System ::
+00000670: 204f 5320 496e 6465 7065 6e64 656e 740d   OS Independent.
+00000680: 0a43 6c61 7373 6966 6965 723a 204e 6174  .Classifier: Nat
+00000690: 7572 616c 204c 616e 6775 6167 6520 3a3a  ural Language ::
+000006a0: 2043 6869 6e65 7365 2028 5369 6d70 6c69   Chinese (Simpli
+000006b0: 6669 6564 290d 0a43 6c61 7373 6966 6965  fied)..Classifie
+000006c0: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
+000006d0: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
+000006e0: 6e0d 0a43 6c61 7373 6966 6965 723a 2050  n..Classifier: P
+000006f0: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+00000700: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+00000710: 2033 0d0a 436c 6173 7369 6669 6572 3a20   3..Classifier: 
+00000720: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
+00000730: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
+00000740: 3a20 332e 310d 0a43 6c61 7373 6966 6965  : 3.1..Classifie
+00000750: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
+00000760: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
+00000770: 6e20 3a3a 2033 2e32 0d0a 436c 6173 7369  n :: 3.2..Classi
+00000780: 6669 6572 3a20 5072 6f67 7261 6d6d 696e  fier: Programmin
+00000790: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+000007a0: 7468 6f6e 203a 3a20 332e 330d 0a43 6c61  thon :: 3.3..Cla
+000007b0: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
+000007c0: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
+000007d0: 2050 7974 686f 6e20 3a3a 2033 2e34 0d0a   Python :: 3.4..
+000007e0: 436c 6173 7369 6669 6572 3a20 5072 6f67  Classifier: Prog
+000007f0: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+00000800: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
+00000810: 350d 0a43 6c61 7373 6966 6965 723a 2050  5..Classifier: P
+00000820: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+00000830: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+00000840: 2033 2e36 0d0a 436c 6173 7369 6669 6572   3.6..Classifier
+00000850: 3a20 5072 6f67 7261 6d6d 696e 6720 4c61  : Programming La
+00000860: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
+00000870: 203a 3a20 332e 370d 0a43 6c61 7373 6966   :: 3.7..Classif
+00000880: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
+00000890: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
+000008a0: 686f 6e20 3a3a 2033 2e38 0d0a 436c 6173  hon :: 3.8..Clas
+000008b0: 7369 6669 6572 3a20 5072 6f67 7261 6d6d  sifier: Programm
+000008c0: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+000008d0: 5079 7468 6f6e 203a 3a20 332e 390d 0a43  Python :: 3.9..C
+000008e0: 6c61 7373 6966 6965 723a 2050 726f 6772  lassifier: Progr
+000008f0: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
+00000900: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e31  :: Python :: 3.1
+00000910: 300d 0a43 6c61 7373 6966 6965 723a 2050  0..Classifier: P
+00000920: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+00000930: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+00000940: 2033 2e31 310d 0a43 6c61 7373 6966 6965   3.11..Classifie
+00000950: 723a 2054 6f70 6963 203a 3a20 536f 6674  r: Topic :: Soft
+00000960: 7761 7265 2044 6576 656c 6f70 6d65 6e74  ware Development
+00000970: 203a 3a20 4c69 6272 6172 6965 730d 0a     :: Libraries..
```

### Comparing `baimomcsm_api-0.0.1/README.md` & `baimomcsm_api-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `baimomcsm_api-0.0.1/baimomcsm_api/applications.py` & `baimomcsm_api-0.0.2/baimomcsm_api/applications.py`

 * *Files identical despite different names*

### Comparing `baimomcsm_api-0.0.1/baimomcsm_api/common.py` & `baimomcsm_api-0.0.2/baimomcsm_api/common.py`

 * *Files identical despite different names*

### Comparing `baimomcsm_api-0.0.1/baimomcsm_api/request_sender.py` & `baimomcsm_api-0.0.2/baimomcsm_api/request_sender.py`

 * *Files identical despite different names*

### Comparing `baimomcsm_api-0.0.1/baimomcsm_api.egg-info/PKG-INFO` & `baimomcsm_api-0.0.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,136 +1,152 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 312e 310d 0a4e 616d 653a 2062 6169  : 1.1..Name: bai
-00000020: 6d6f 6d63 736d 2d61 7069 0d0a 5665 7273  momcsm-api..Vers
-00000030: 696f 6e3a 2030 2e30 2e31 0d0a 5375 6d6d  ion: 0.0.1..Summ
+00000020: 6d6f 6d63 736d 5f61 7069 0d0a 5665 7273  momcsm_api..Vers
+00000030: 696f 6e3a 2030 2e30 2e32 0d0a 5375 6d6d  ion: 0.0.2..Summ
 00000040: 6172 793a 204d 4353 4d61 6e61 6765 7220  ary: MCSManager 
 00000050: 4150 4920 666f 7220 5079 7468 6f6e 2028  API for Python (
 00000060: e5bc 80e5 8f91 e4b8 ad29 0d0a 486f 6d65  .........)..Home
 00000070: 2d70 6167 653a 2068 7474 7073 3a2f 2f67  -page: https://g
 00000080: 6974 6875 622e 636f 6d2f 5a68 6f75 2d53  ithub.com/Zhou-S
 00000090: 6869 6c69 6e2f 4261 696d 6f4d 4353 4d61  hilin/BaimoMCSMa
 000000a0: 6e61 6765 722d 4150 490d 0a41 7574 686f  nager-API..Autho
 000000b0: 723a 2042 6169 6d6f 5169 6c69 6e0d 0a41  r: BaimoQilin..A
 000000c0: 7574 686f 722d 656d 6169 6c3a 2061 646d  uthor-email: adm
 000000d0: 696e 4062 6169 6d6f 7169 6c69 6e2e 746f  in@baimoqilin.to
 000000e0: 700d 0a4c 6963 656e 7365 3a20 4170 6163  p..License: Apac
 000000f0: 6865 2032 2e30 0d0a 4465 7363 7269 7074  he 2.0..Descript
-00000100: 696f 6e3a 2023 2042 6169 6d6f 4d43 534d  ion: # BaimoMCSM
-00000110: 616e 6167 6572 2041 5049 2066 6f72 2060  anager API for `
-00000120: 5079 7468 6f6e 600d 0a20 2020 2020 2020  Python`..       
-00000130: 205b 215b 5052 7320 7765 6c63 6f6d 655d   [![PRs welcome]
-00000140: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
-00000150: 656c 6473 2e69 6f2f 6261 6467 652f 5052  elds.io/badge/PR
-00000160: 732d 7765 6c63 6f6d 652d 3230 4246 3230  s-welcome-20BF20
-00000170: 295d 2868 7474 7073 3a2f 2f67 6974 6875  )](https://githu
-00000180: 622e 636f 6d2f 5a68 6f75 2d53 6869 6c69  b.com/Zhou-Shili
-00000190: 6e2f 4261 696d 6f4d 4353 4d61 6e61 6765  n/BaimoMCSManage
-000001a0: 722d 4150 492f 7075 6c6c 7329 0d0a 2020  r-API/pulls)..  
-000001b0: 2020 2020 2020 215b 5375 7070 6f72 7420        ![Support 
-000001c0: 4d53 434d 2039 2e39 2e30 5d28 6874 7470  MSCM 9.9.0](http
-000001d0: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
-000001e0: 696f 2f62 6164 6765 2f53 7570 706f 7274  io/badge/Support
-000001f0: 2d4d 4353 4d5f 392e 392e 302d 626c 7565  -MCSM_9.9.0-blue
-00000200: 290d 0a20 2020 2020 2020 2021 5b41 7061  )..        ![Apa
-00000210: 6368 6520 4c69 6365 6e73 655d 2868 7474  che License](htt
-00000220: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
-00000230: 2e69 6f2f 6261 6467 652f 4c69 6365 6e73  .io/badge/Licens
-00000240: 652d 4170 6163 6865 2d72 6564 2920 200d  e-Apache-red)  .
-00000250: 0a20 2020 2020 2020 20e8 bf99 e698 afe4  .        .......
-00000260: b880 e4b8 aae9 8082 e794 a8e4 ba8e 5079  ..............Py
-00000270: 7468 6f6e e8af ade8 a880 e79a 84e7 acac  thon............
-00000280: e4b8 89e6 96b9 e5ba 93ef bc8c e8ae a9e4  ................
-00000290: bda0 e59c a850 7974 686f 6ee4 b8ad e69b  .....Python.....
-000002a0: b4e6 96b9 e4be bfe5 9cb0 e8b0 83e7 94a8  ................
-000002b0: 5b4d 4353 4d2d 4150 490d 0a20 2020 2020  [MCSM-API..     
-000002c0: 2020 205d 2868 7474 7073 3a2f 2f64 6f63     ](https://doc
-000002d0: 732e 6d63 736d 616e 6167 6572 2e63 6f6d  s.mcsmanager.com
-000002e0: 2f23 2f7a 682d 636e 2f61 7069 732f 7265  /#/zh-cn/apis/re
-000002f0: 6164 6d65 29e7 aea1 e790 86e4 bda0 e79a  adme)...........
-00000300: 84e6 9c8d e58a a1e5 99a8 e380 820d 0a20  ............... 
-00000310: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00000320: 2023 2320 e29a a0ef b88f e6b3 a8e6 848f   ## ............
-00000330: 0d0a 2020 2020 2020 2020 e8bf 99e4 b8aa  ..        ......
-00000340: e9a1 b9e7 9bae e4bb 8de5 9ca8 e5bc 80e5  ................
-00000350: 8f91 e4b8 adef bc8c e4bb 85e6 94af e68c  ................
-00000360: 81e9 83a8 e588 86e5 8a9f e883 bde3 8082  ................
-00000370: 2020 0d0a 2020 2020 2020 2020 2020 0d0a    ..          ..
-00000380: 2020 2020 2020 2020 e5bd 93e5 898d e8bf          ........
-00000390: 9be5 b195 efbc 9a0d 0a20 2020 2020 2020  .........       
-000003a0: 2020 2d20 5b78 5d20 e99d a2e6 9dbf e980    - [x] ........
-000003b0: 9ae7 94a8 e8ae bee7 bdae 2028 2060 636f  .......... ( `co
-000003c0: 6d6d 6f6e 2e70 7960 290d 0a20 2020 2020  mmon.py`)..     
-000003d0: 2020 2020 2d20 5b78 5d20 e5ba 94e7 94a8      - [x] ......
-000003e0: e5ae 9ee4 be8b e7ae a1e7 9086 2028 6061  ............ (`a
-000003f0: 7070 6c69 6361 7469 6f6e 732e 7079 6029  pplications.py`)
-00000400: 0d0a 2020 2020 2020 2020 202d 205b 205d  ..         - [ ]
-00000410: 20e5 ae9e e4be 8be6 9687 e4bb b6e7 aea1   ...............
-00000420: e790 8620 2860 6669 6c65 732e 7079 6029  ... (`files.py`)
-00000430: 0d0a 2020 2020 2020 2020 202d 205b 205d  ..         - [ ]
-00000440: 20e8 aea1 e588 92e4 bbbb e58a a1e7 aea1   ...............
-00000450: e790 8620 2860 706c 616e 732e 7079 6029  ... (`plans.py`)
-00000460: 0d0a 2020 2020 2020 2020 202d 205b 205d  ..         - [ ]
-00000470: 20e5 ae88 e68a a4e8 bf9b e7a8 8be7 aea1   ...............
-00000480: e790 8620 2820 6072 656d 6f74 655f 7365  ... ( `remote_se
-00000490: 7276 6963 652e 7079 6029 0d0a 2020 2020  rvice.py`)..    
-000004a0: 2020 2020 202d 205b 205d 20e5 a49a e794       - [ ] .....
-000004b0: a8e6 88b7 e7ae a1e7 9086 2028 6061 7574  .......... (`aut
-000004c0: 682e 7079 6029 0d0a 2020 2020 2020 2020  h.py`)..        
-000004d0: 0d0a 2020 2020 2020 2020 2323 20f0 9f93  ..        ## ...
-000004e0: 96e4 bdbf e794 a8e6 96b9 e6b3 950d 0a20  ............... 
-000004f0: 2020 2020 2020 20e6 96bd e5b7 a5e4 b8ad         .........
-00000500: e280 a6e2 80a6 0d0a 506c 6174 666f 726d  ........Platform
-00000510: 3a20 616c 6c0d 0a43 6c61 7373 6966 6965  : all..Classifie
-00000520: 723a 2049 6e74 656e 6465 6420 4175 6469  r: Intended Audi
-00000530: 656e 6365 203a 3a20 4465 7665 6c6f 7065  ence :: Develope
-00000540: 7273 0d0a 436c 6173 7369 6669 6572 3a20  rs..Classifier: 
-00000550: 4f70 6572 6174 696e 6720 5379 7374 656d  Operating System
-00000560: 203a 3a20 4f53 2049 6e64 6570 656e 6465   :: OS Independe
-00000570: 6e74 0d0a 436c 6173 7369 6669 6572 3a20  nt..Classifier: 
-00000580: 4e61 7475 7261 6c20 4c61 6e67 7561 6765  Natural Language
-00000590: 203a 3a20 4368 696e 6573 6520 2853 696d   :: Chinese (Sim
-000005a0: 706c 6966 6965 6429 0d0a 436c 6173 7369  plified)..Classi
-000005b0: 6669 6572 3a20 5072 6f67 7261 6d6d 696e  fier: Programmin
-000005c0: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-000005d0: 7468 6f6e 0d0a 436c 6173 7369 6669 6572  thon..Classifier
-000005e0: 3a20 5072 6f67 7261 6d6d 696e 6720 4c61  : Programming La
-000005f0: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-00000600: 203a 3a20 330d 0a43 6c61 7373 6966 6965   :: 3..Classifie
-00000610: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
-00000620: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
-00000630: 6e20 3a3a 2033 2e31 0d0a 436c 6173 7369  n :: 3.1..Classi
-00000640: 6669 6572 3a20 5072 6f67 7261 6d6d 696e  fier: Programmin
-00000650: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-00000660: 7468 6f6e 203a 3a20 332e 320d 0a43 6c61  thon :: 3.2..Cla
-00000670: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
-00000680: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-00000690: 2050 7974 686f 6e20 3a3a 2033 2e33 0d0a   Python :: 3.3..
-000006a0: 436c 6173 7369 6669 6572 3a20 5072 6f67  Classifier: Prog
-000006b0: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
-000006c0: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
-000006d0: 340d 0a43 6c61 7373 6966 6965 723a 2050  4..Classifier: P
-000006e0: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-000006f0: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
-00000700: 2033 2e35 0d0a 436c 6173 7369 6669 6572   3.5..Classifier
-00000710: 3a20 5072 6f67 7261 6d6d 696e 6720 4c61  : Programming La
-00000720: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-00000730: 203a 3a20 332e 360d 0a43 6c61 7373 6966   :: 3.6..Classif
-00000740: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
-00000750: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
-00000760: 686f 6e20 3a3a 2033 2e37 0d0a 436c 6173  hon :: 3.7..Clas
-00000770: 7369 6669 6572 3a20 5072 6f67 7261 6d6d  sifier: Programm
-00000780: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
-00000790: 5079 7468 6f6e 203a 3a20 332e 380d 0a43  Python :: 3.8..C
-000007a0: 6c61 7373 6966 6965 723a 2050 726f 6772  lassifier: Progr
-000007b0: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
-000007c0: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e39  :: Python :: 3.9
-000007d0: 0d0a 436c 6173 7369 6669 6572 3a20 5072  ..Classifier: Pr
-000007e0: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-000007f0: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-00000800: 332e 3130 0d0a 436c 6173 7369 6669 6572  3.10..Classifier
-00000810: 3a20 5072 6f67 7261 6d6d 696e 6720 4c61  : Programming La
-00000820: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-00000830: 203a 3a20 332e 3131 0d0a 436c 6173 7369   :: 3.11..Classi
-00000840: 6669 6572 3a20 546f 7069 6320 3a3a 2053  fier: Topic :: S
-00000850: 6f66 7477 6172 6520 4465 7665 6c6f 706d  oftware Developm
-00000860: 656e 7420 3a3a 204c 6962 7261 7269 6573  ent :: Libraries
-00000870: 0d0a                                     ..
+00000100: 696f 6e3a 203c 6831 2069 643d 2262 6169  ion: <h1 id="bai
+00000110: 6d6f 6d63 736d 616e 6167 6572 2d61 7069  momcsmanager-api
+00000120: 2d66 6f72 2d70 7974 686f 6e22 3e42 6169  -for-python">Bai
+00000130: 6d6f 4d43 534d 616e 6167 6572 2041 5049  moMCSManager API
+00000140: 2066 6f72 0d0a 2020 2020 2020 2020 3c63   for..        <c
+00000150: 6f64 653e 5079 7468 6f6e 3c2f 636f 6465  ode>Python</code
+00000160: 3e3c 2f68 313e 0d0a 2020 2020 2020 2020  ></h1>..        
+00000170: 3c70 3e3c 610d 0a20 2020 2020 2020 2068  <p><a..        h
+00000180: 7265 663d 2268 7474 7073 3a2f 2f67 6974  ref="https://git
+00000190: 6875 622e 636f 6d2f 5a68 6f75 2d53 6869  hub.com/Zhou-Shi
+000001a0: 6c69 6e2f 4261 696d 6f4d 4353 4d61 6e61  lin/BaimoMCSMana
+000001b0: 6765 722d 4150 492f 7075 6c6c 7322 3e3c  ger-API/pulls"><
+000001c0: 696d 670d 0a20 2020 2020 2020 2073 7263  img..        src
+000001d0: 3d22 6874 7470 733a 2f2f 696d 672e 7368  ="https://img.sh
+000001e0: 6965 6c64 732e 696f 2f62 6164 6765 2f50  ields.io/badge/P
+000001f0: 5273 2d77 656c 636f 6d65 2d32 3042 4632  Rs-welcome-20BF2
+00000200: 3022 0d0a 2020 2020 2020 2020 616c 743d  0"..        alt=
+00000210: 2250 5273 2077 656c 636f 6d65 2220 2f3e  "PRs welcome" />
+00000220: 3c2f 613e 203c 696d 670d 0a20 2020 2020  </a> <img..     
+00000230: 2020 2073 7263 3d22 6874 7470 733a 2f2f     src="https://
+00000240: 696d 672e 7368 6965 6c64 732e 696f 2f62  img.shields.io/b
+00000250: 6164 6765 2f53 7570 706f 7274 2d4d 4353  adge/Support-MCS
+00000260: 4d5f 392e 392e 302d 626c 7565 220d 0a20  M_9.9.0-blue".. 
+00000270: 2020 2020 2020 2061 6c74 3d22 5375 7070         alt="Supp
+00000280: 6f72 7420 4d53 434d 2039 2e39 2e30 2220  ort MSCM 9.9.0" 
+00000290: 2f3e 203c 696d 670d 0a20 2020 2020 2020  /> <img..       
+000002a0: 2073 7263 3d22 6874 7470 733a 2f2f 696d   src="https://im
+000002b0: 672e 7368 6965 6c64 732e 696f 2f62 6164  g.shields.io/bad
+000002c0: 6765 2f4c 6963 656e 7365 2d41 7061 6368  ge/License-Apach
+000002d0: 652d 7265 6422 0d0a 2020 2020 2020 2020  e-red"..        
+000002e0: 616c 743d 2241 7061 6368 6520 4c69 6365  alt="Apache Lice
+000002f0: 6e73 6522 202f 3e3c 6272 202f 3e0d 0a20  nse" /><br />.. 
+00000300: 2020 2020 2020 20e8 bf99 e698 afe4 b880         .........
+00000310: e4b8 aae9 8082 e794 a8e4 ba8e 5079 7468  ............Pyth
+00000320: 6f6e e8af ade8 a880 e79a 84e7 acac e4b8  on..............
+00000330: 89e6 96b9 e5ba 93ef bc8c e8ae a9e4 bda0  ................
+00000340: e59c a850 7974 686f 6ee4 b8ad e69b b4e6  ...Python.......
+00000350: 96b9 e4be bfe5 9cb0 e8b0 83e7 94a8 3c61  ..............<a
+00000360: 0d0a 2020 2020 2020 2020 6872 6566 3d22  ..        href="
+00000370: 6874 7470 733a 2f2f 646f 6373 2e6d 6373  https://docs.mcs
+00000380: 6d61 6e61 6765 722e 636f 6d2f 232f 7a68  manager.com/#/zh
+00000390: 2d63 6e2f 6170 6973 2f72 6561 646d 6522  -cn/apis/readme"
+000003a0: 3e4d 4353 4d2d 4150 493c 2f61 3ee7 aea1  >MCSM-API</a>...
+000003b0: e790 86e4 bda0 e79a 84e6 9c8d e58a a1e5  ................
+000003c0: 99a8 e380 823c 2f70 3e0d 0a20 2020 2020  .....</p>..     
+000003d0: 2020 203c 6832 2069 643d 22e6 b3a8 e684     <h2 id=".....
+000003e0: 8f22 3ee2 9aa0 efb8 8fe6 b3a8 e684 8f3c  .">............<
+000003f0: 2f68 323e 0d0a 2020 2020 2020 2020 3c70  /h2>..        <p
+00000400: 3ee8 bf99 e4b8 aae9 a1b9 e79b aee4 bb8d  >...............
+00000410: e59c a8e5 bc80 e58f 91e4 b8ad efbc 8ce4  ................
+00000420: bb85 e694 afe6 8c81 e983 a8e5 8886 e58a  ................
+00000430: 9fe8 83bd e380 823c 2f70 3e0d 0a20 2020  .......</p>..   
+00000440: 2020 2020 203c 703e e5bd 93e5 898d e8bf       <p>........
+00000450: 9be5 b195 efbc 9a20 2d20 5b78 5d20 e99d  ....... - [x] ..
+00000460: a2e6 9dbf e980 9ae7 94a8 e8ae bee7 bdae  ................
+00000470: 2028 203c 636f 6465 3e63 6f6d 6d6f 6e2e   ( <code>common.
+00000480: 7079 3c2f 636f 6465 3e29 202d 205b 785d  py</code>) - [x]
+00000490: 0d0a 2020 2020 2020 2020 e5ba 94e7 94a8  ..        ......
+000004a0: e5ae 9ee4 be8b e7ae a1e7 9086 2028 3c63  ............ (<c
+000004b0: 6f64 653e 6170 706c 6963 6174 696f 6e73  ode>applications
+000004c0: 2e70 793c 2f63 6f64 653e 2920 2d20 5b20  .py</code>) - [ 
+000004d0: 5d20 e5ae 9ee4 be8b e696 87e4 bbb6 e7ae  ] ..............
+000004e0: a1e7 9086 0d0a 2020 2020 2020 2020 283c  ......        (<
+000004f0: 636f 6465 3e66 696c 6573 2e70 793c 2f63  code>files.py</c
+00000500: 6f64 653e 2920 2d20 5b20 5d20 e8ae a1e5  ode>) - [ ] ....
+00000510: 8892 e4bb bbe5 8aa1 e7ae a1e7 9086 2028  .............. (
+00000520: 3c63 6f64 653e 706c 616e 732e 7079 3c2f  <code>plans.py</
+00000530: 636f 6465 3e29 202d 205b 205d 0d0a 2020  code>) - [ ]..  
+00000540: 2020 2020 2020 e5ae 88e6 8aa4 e8bf 9be7        ..........
+00000550: a88b e7ae a1e7 9086 2028 203c 636f 6465  ........ ( <code
+00000560: 3e72 656d 6f74 655f 7365 7276 6963 652e  >remote_service.
+00000570: 7079 3c2f 636f 6465 3e29 202d 205b 205d  py</code>) - [ ]
+00000580: 20e5 a49a e794 a8e6 88b7 e7ae a1e7 9086   ...............
+00000590: 0d0a 2020 2020 2020 2020 283c 636f 6465  ..        (<code
+000005a0: 3e61 7574 682e 7079 3c2f 636f 6465 3e29  >auth.py</code>)
+000005b0: 3c2f 703e 0d0a 2020 2020 2020 2020 3c68  </p>..        <h
+000005c0: 3220 6964 3d22 e4bd bfe7 94a8 e696 b9e6  2 id="..........
+000005d0: b395 223e f09f 9396 e4bd bfe7 94a8 e696  ..">............
+000005e0: b9e6 b395 3c2f 6832 3e0d 0a20 2020 2020  ....</h2>..     
+000005f0: 2020 203c 703e e696 bde5 b7a5 e4b8 ade2     <p>..........
+00000600: 80a6 e280 a63c 2f70 3e0d 0a20 2020 2020  .....</p>..     
+00000610: 2020 200d 0a50 6c61 7466 6f72 6d3a 2061     ..Platform: a
+00000620: 6c6c 0d0a 436c 6173 7369 6669 6572 3a20  ll..Classifier: 
+00000630: 496e 7465 6e64 6564 2041 7564 6965 6e63  Intended Audienc
+00000640: 6520 3a3a 2044 6576 656c 6f70 6572 730d  e :: Developers.
+00000650: 0a43 6c61 7373 6966 6965 723a 204f 7065  .Classifier: Ope
+00000660: 7261 7469 6e67 2053 7973 7465 6d20 3a3a  rating System ::
+00000670: 204f 5320 496e 6465 7065 6e64 656e 740d   OS Independent.
+00000680: 0a43 6c61 7373 6966 6965 723a 204e 6174  .Classifier: Nat
+00000690: 7572 616c 204c 616e 6775 6167 6520 3a3a  ural Language ::
+000006a0: 2043 6869 6e65 7365 2028 5369 6d70 6c69   Chinese (Simpli
+000006b0: 6669 6564 290d 0a43 6c61 7373 6966 6965  fied)..Classifie
+000006c0: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
+000006d0: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
+000006e0: 6e0d 0a43 6c61 7373 6966 6965 723a 2050  n..Classifier: P
+000006f0: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+00000700: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+00000710: 2033 0d0a 436c 6173 7369 6669 6572 3a20   3..Classifier: 
+00000720: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
+00000730: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
+00000740: 3a20 332e 310d 0a43 6c61 7373 6966 6965  : 3.1..Classifie
+00000750: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
+00000760: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
+00000770: 6e20 3a3a 2033 2e32 0d0a 436c 6173 7369  n :: 3.2..Classi
+00000780: 6669 6572 3a20 5072 6f67 7261 6d6d 696e  fier: Programmin
+00000790: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+000007a0: 7468 6f6e 203a 3a20 332e 330d 0a43 6c61  thon :: 3.3..Cla
+000007b0: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
+000007c0: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
+000007d0: 2050 7974 686f 6e20 3a3a 2033 2e34 0d0a   Python :: 3.4..
+000007e0: 436c 6173 7369 6669 6572 3a20 5072 6f67  Classifier: Prog
+000007f0: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+00000800: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
+00000810: 350d 0a43 6c61 7373 6966 6965 723a 2050  5..Classifier: P
+00000820: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+00000830: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+00000840: 2033 2e36 0d0a 436c 6173 7369 6669 6572   3.6..Classifier
+00000850: 3a20 5072 6f67 7261 6d6d 696e 6720 4c61  : Programming La
+00000860: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
+00000870: 203a 3a20 332e 370d 0a43 6c61 7373 6966   :: 3.7..Classif
+00000880: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
+00000890: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
+000008a0: 686f 6e20 3a3a 2033 2e38 0d0a 436c 6173  hon :: 3.8..Clas
+000008b0: 7369 6669 6572 3a20 5072 6f67 7261 6d6d  sifier: Programm
+000008c0: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+000008d0: 5079 7468 6f6e 203a 3a20 332e 390d 0a43  Python :: 3.9..C
+000008e0: 6c61 7373 6966 6965 723a 2050 726f 6772  lassifier: Progr
+000008f0: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
+00000900: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e31  :: Python :: 3.1
+00000910: 300d 0a43 6c61 7373 6966 6965 723a 2050  0..Classifier: P
+00000920: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+00000930: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+00000940: 2033 2e31 310d 0a43 6c61 7373 6966 6965   3.11..Classifie
+00000950: 723a 2054 6f70 6963 203a 3a20 536f 6674  r: Topic :: Soft
+00000960: 7761 7265 2044 6576 656c 6f70 6d65 6e74  ware Development
+00000970: 203a 3a20 4c69 6272 6172 6965 730d 0a     :: Libraries..
```

### Comparing `baimomcsm_api-0.0.1/setup.py` & `baimomcsm_api-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from distutils.core import setup
 from setuptools import find_packages
 
-with open("README.md", "r", encoding="utf-8") as f:
+with open("README.html", "r", encoding="utf-8") as f:
   long_description = f.read()
 
 setup(name='baimomcsm_api',  # 包名
-      version='0.0.1',  # 版本号
+      version='0.0.2',  # 版本号
       description='MCSManager API for Python (开发中)',
       long_description=long_description,
       author='BaimoQilin',
       author_email='admin@baimoqilin.top',
       url='https://github.com/Zhou-Shilin/BaimoMCSManager-API',
       install_requires=["requests"],
       license='Apache 2.0',
```

