# Comparing `tmp/htscf-0.0.8.tar.gz` & `tmp/htscf-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "htscf-0.0.8.tar", last modified: Thu Jul 20 03:38:48 2023, max compression
+gzip compressed data, was "htscf-0.0.9.tar", last modified: Thu Jul 20 08:37:06 2023, max compression
```

## Comparing `htscf-0.0.8.tar` & `htscf-0.0.9.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2023-07-20 03:38:48.397004 htscf-0.0.8/
--rw-rw-rw-   0        0        0     1084 2022-03-29 00:57:11.000000 htscf-0.0.8/LICENSE
--rw-rw-rw-   0        0        0      209 2023-07-18 13:34:36.000000 htscf-0.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0      825 2023-07-20 03:38:48.397004 htscf-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      336 2022-08-09 08:26:17.000000 htscf-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-07-20 03:38:48.272336 htscf-0.0.8/htscf/
--rw-rw-rw-   0        0        0        0 2023-07-18 13:34:36.000000 htscf-0.0.8/htscf/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-20 03:38:48.344144 htscf-0.0.8/htscf/cli/
--rw-rw-rw-   0        0        0        0 2022-03-17 08:58:49.000000 htscf-0.0.8/htscf/cli/__init__.py
--rw-rw-rw-   0        0        0     1299 2023-07-18 13:34:36.000000 htscf-0.0.8/htscf/cli/bdc.py
--rw-rw-rw-   0        0        0     1182 2022-03-31 08:13:37.000000 htscf-0.0.8/htscf/cli/login.py
--rw-rw-rw-   0        0        0     1085 2022-03-31 08:05:58.000000 htscf-0.0.8/htscf/cli/logout.py
--rw-rw-rw-   0        0        0     1438 2023-07-18 12:36:26.000000 htscf-0.0.8/htscf/cli/main.py
-drwxrwxrwx   0        0        0        0 2023-07-20 03:38:48.353120 htscf-0.0.8/htscf/core/
--rw-rw-rw-   0        0        0        0 2021-10-09 11:42:50.000000 htscf-0.0.8/htscf/core/__init__.py
--rw-rw-rw-   0        0        0      802 2023-07-18 11:50:59.000000 htscf-0.0.8/htscf/core/createStep.py
--rw-rw-rw-   0        0        0     2838 2023-07-20 03:35:57.000000 htscf-0.0.8/htscf/core/flow.py
-drwxrwxrwx   0        0        0        0 2023-07-20 03:38:48.360101 htscf-0.0.8/htscf/db/
--rw-rw-rw-   0        0        0        0 2023-07-18 06:33:00.000000 htscf-0.0.8/htscf/db/__init__.py
--rw-rw-rw-   0        0        0      264 2023-07-18 06:38:01.000000 htscf-0.0.8/htscf/db/mongo.py
-drwxrwxrwx   0        0        0        0 2023-07-20 03:38:48.369112 htscf-0.0.8/htscf/io/
--rw-rw-rw-   0        0        0        0 2021-10-09 11:42:50.000000 htscf-0.0.8/htscf/io/__init__.py
--rw-rw-rw-   0        0        0     4919 2023-07-18 13:37:43.000000 htscf-0.0.8/htscf/io/vaspIO.py
-drwxrwxrwx   0        0        0        0 2023-07-20 03:38:48.376059 htscf-0.0.8/htscf/test/
--rw-rw-rw-   0        0        0        0 2023-07-18 13:07:06.000000 htscf-0.0.8/htscf/test/__init__.py
--rw-rw-rw-   0        0        0      175 2023-07-18 13:07:53.000000 htscf-0.0.8/htscf/test/test.py
-drwxrwxrwx   0        0        0        0 2023-07-20 03:38:48.396034 htscf-0.0.8/htscf/utils/
--rw-rw-rw-   0        0        0        0 2021-10-09 11:42:50.000000 htscf-0.0.8/htscf/utils/__init__.py
--rw-rw-rw-   0        0        0     1956 2023-07-18 13:04:20.000000 htscf-0.0.8/htscf/utils/qsub.py
--rw-rw-rw-   0        0        0     2740 2023-07-18 13:06:01.000000 htscf-0.0.8/htscf/utils/tools.py
-drwxrwxrwx   0        0        0        0 2023-07-20 03:38:48.311261 htscf-0.0.8/htscf.egg-info/
--rw-rw-rw-   0        0        0      825 2023-07-20 03:38:48.000000 htscf-0.0.8/htscf.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      634 2023-07-20 03:38:48.000000 htscf-0.0.8/htscf.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-20 03:38:48.000000 htscf-0.0.8/htscf.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-07-20 03:38:48.000000 htscf-0.0.8/htscf.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-07-18 13:18:21.000000 htscf-0.0.8/htscf.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       63 2023-07-20 03:38:48.000000 htscf-0.0.8/htscf.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-20 03:38:48.000000 htscf-0.0.8/htscf.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       80 2022-03-09 04:15:13.000000 htscf-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0      669 2023-07-20 03:38:48.398997 htscf-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      197 2023-07-18 13:08:10.000000 htscf-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-20 08:37:06.226092 htscf-0.0.9/
+-rw-rw-rw-   0        0        0     1084 2022-03-29 00:57:11.000000 htscf-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0      209 2023-07-18 13:34:36.000000 htscf-0.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0      825 2023-07-20 08:37:06.226092 htscf-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      336 2022-08-09 08:26:17.000000 htscf-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-07-20 08:37:06.108407 htscf-0.0.9/htscf/
+-rw-rw-rw-   0        0        0        0 2023-07-18 13:34:36.000000 htscf-0.0.9/htscf/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-20 08:37:06.172274 htscf-0.0.9/htscf/cli/
+-rw-rw-rw-   0        0        0        0 2022-03-17 08:58:49.000000 htscf-0.0.9/htscf/cli/__init__.py
+-rw-rw-rw-   0        0        0     1299 2023-07-18 13:34:36.000000 htscf-0.0.9/htscf/cli/bdc.py
+-rw-rw-rw-   0        0        0     1182 2022-03-31 08:13:37.000000 htscf-0.0.9/htscf/cli/login.py
+-rw-rw-rw-   0        0        0     1085 2022-03-31 08:05:58.000000 htscf-0.0.9/htscf/cli/logout.py
+-rw-rw-rw-   0        0        0     1438 2023-07-18 12:36:26.000000 htscf-0.0.9/htscf/cli/main.py
+drwxrwxrwx   0        0        0        0 2023-07-20 08:37:06.189190 htscf-0.0.9/htscf/core/
+-rw-rw-rw-   0        0        0        0 2021-10-09 11:42:50.000000 htscf-0.0.9/htscf/core/__init__.py
+-rw-rw-rw-   0        0        0      802 2023-07-18 11:50:59.000000 htscf-0.0.9/htscf/core/createStep.py
+-rw-rw-rw-   0        0        0     2838 2023-07-20 03:35:57.000000 htscf-0.0.9/htscf/core/flow.py
+drwxrwxrwx   0        0        0        0 2023-07-20 08:37:06.196203 htscf-0.0.9/htscf/db/
+-rw-rw-rw-   0        0        0        0 2023-07-18 06:33:00.000000 htscf-0.0.9/htscf/db/__init__.py
+-rw-rw-rw-   0        0        0      264 2023-07-18 06:38:01.000000 htscf-0.0.9/htscf/db/mongo.py
+drwxrwxrwx   0        0        0        0 2023-07-20 08:37:06.206174 htscf-0.0.9/htscf/io/
+-rw-rw-rw-   0        0        0        0 2021-10-09 11:42:50.000000 htscf-0.0.9/htscf/io/__init__.py
+-rw-rw-rw-   0        0        0     4919 2023-07-18 13:37:43.000000 htscf-0.0.9/htscf/io/vaspIO.py
+drwxrwxrwx   0        0        0        0 2023-07-20 08:37:06.213127 htscf-0.0.9/htscf/test/
+-rw-rw-rw-   0        0        0        0 2023-07-18 13:07:06.000000 htscf-0.0.9/htscf/test/__init__.py
+-rw-rw-rw-   0        0        0      175 2023-07-18 13:07:53.000000 htscf-0.0.9/htscf/test/test.py
+drwxrwxrwx   0        0        0        0 2023-07-20 08:37:06.225094 htscf-0.0.9/htscf/utils/
+-rw-rw-rw-   0        0        0        0 2021-10-09 11:42:50.000000 htscf-0.0.9/htscf/utils/__init__.py
+-rw-rw-rw-   0        0        0     1956 2023-07-18 13:04:20.000000 htscf-0.0.9/htscf/utils/qsub.py
+-rw-rw-rw-   0        0        0     3678 2023-07-20 08:36:45.000000 htscf-0.0.9/htscf/utils/tools.py
+drwxrwxrwx   0        0        0        0 2023-07-20 08:37:06.137401 htscf-0.0.9/htscf.egg-info/
+-rw-rw-rw-   0        0        0      825 2023-07-20 08:37:06.000000 htscf-0.0.9/htscf.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      634 2023-07-20 08:37:06.000000 htscf-0.0.9/htscf.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-20 08:37:06.000000 htscf-0.0.9/htscf.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-07-20 08:37:06.000000 htscf-0.0.9/htscf.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-07-18 13:18:21.000000 htscf-0.0.9/htscf.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       63 2023-07-20 08:37:06.000000 htscf-0.0.9/htscf.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-20 08:37:06.000000 htscf-0.0.9/htscf.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       80 2022-03-09 04:15:13.000000 htscf-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0      669 2023-07-20 08:37:06.228088 htscf-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      197 2023-07-18 13:08:10.000000 htscf-0.0.9/setup.py
```

### Comparing `htscf-0.0.8/LICENSE` & `htscf-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `htscf-0.0.8/PKG-INFO` & `htscf-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: htscf
-Version: 0.0.8
+Version: 0.0.9
 Summary: High-throughput computing flow
 Home-page: http://zhcloud.top
 Author: Hao Zhao
 Author-email: 601095001@qq.com
 License: OSI Approved :: MIT License
 Platform: Linux/Windows
 Classifier: Programming Language :: Python :: 3
```

### Comparing `htscf-0.0.8/htscf/cli/bdc.py` & `htscf-0.0.9/htscf/cli/bdc.py`

 * *Files identical despite different names*

### Comparing `htscf-0.0.8/htscf/cli/login.py` & `htscf-0.0.9/htscf/cli/login.py`

 * *Files identical despite different names*

### Comparing `htscf-0.0.8/htscf/cli/logout.py` & `htscf-0.0.9/htscf/cli/logout.py`

 * *Files identical despite different names*

### Comparing `htscf-0.0.8/htscf/cli/main.py` & `htscf-0.0.9/htscf/cli/main.py`

 * *Files identical despite different names*

### Comparing `htscf-0.0.8/htscf/core/createStep.py` & `htscf-0.0.9/htscf/core/createStep.py`

 * *Files identical despite different names*

### Comparing `htscf-0.0.8/htscf/core/flow.py` & `htscf-0.0.9/htscf/core/flow.py`

 * *Files identical despite different names*

### Comparing `htscf-0.0.8/htscf/io/vaspIO.py` & `htscf-0.0.9/htscf/io/vaspIO.py`

 * *Files identical despite different names*

### Comparing `htscf-0.0.8/htscf/utils/qsub.py` & `htscf-0.0.9/htscf/utils/qsub.py`

 * *Files identical despite different names*

### Comparing `htscf-0.0.8/htscf/utils/tools.py` & `htscf-0.0.9/htscf/utils/tools.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import os
 from functools import wraps
 from hashlib import md5
 from inspect import getattr_static
+from io import StringIO
 from os.path import join
 from pathlib import Path
 from re import Pattern, match
 from shutil import copy
 from typing import List, Union, Iterator
 
+from ase import Atoms
 from ase.io.cif import CIFBlock, parse_block
 from ase.io.cif_unicode import format_unicode
 
 
 def copyFile(src_dir, target_dir, file):
     if not os.path.exists(target_dir):
         os.makedirs(target_dir)
@@ -91,9 +93,37 @@
         line = lines.pop().strip()
         if not line or line.startswith('#'):
             continue
 
         yield parse_block(lines, line)
 
 
-def parse_cif_ase_string(s):
+def parse_cif_ase_string(s) -> Atoms:
     return list(parse_cif_ase(s))[0].get_atoms()
+
+
+def cif2poscar(cif_content: str):
+    sio = StringIO()
+    atoms = parse_cif_ase_string(cif_content)
+    atoms.write(sio, format="vasp")
+    sio.seek(0)
+    lines = sio.readlines()
+    symbol = lines[5].split()
+    number = lines[6].split()
+    positions = lines[8:]
+    d = {}
+    for s, n in zip(symbol, number):
+        n = int(n)
+        if s not in d.keys():
+            d.update({s: [0, []]})
+        d[s][0] = d[s][0] + n
+        d[s][1].extend([positions.pop(0) for _ in range(n)])
+    _symbol = []
+    _number = []
+    _positions = []
+    for k, v in d.items():
+        _symbol.append(k)
+        _number.append(str(v[0]))
+        _positions.extend(v[1])
+    name = "".join([f"{s}{n}" for s, n in zip(_symbol, _number)])
+    content = f"{name}\n{''.join(lines[1:5])}{' ' + ' '.join(_symbol)}\n{'  ' + ' '.join(_number)}\n{lines[7]}{''.join(_positions)}"
+    return content
```

### Comparing `htscf-0.0.8/htscf.egg-info/PKG-INFO` & `htscf-0.0.9/htscf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: htscf
-Version: 0.0.8
+Version: 0.0.9
 Summary: High-throughput computing flow
 Home-page: http://zhcloud.top
 Author: Hao Zhao
 Author-email: 601095001@qq.com
 License: OSI Approved :: MIT License
 Platform: Linux/Windows
 Classifier: Programming Language :: Python :: 3
```

### Comparing `htscf-0.0.8/htscf.egg-info/SOURCES.txt` & `htscf-0.0.9/htscf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `htscf-0.0.8/setup.cfg` & `htscf-0.0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2068 7473 6366 0d0a 7665 7273 696f   = htscf..versio
-00000020: 6e20 3d20 302e 302e 380d 0a64 6573 6372  n = 0.0.8..descr
+00000020: 6e20 3d20 302e 302e 390d 0a64 6573 6372  n = 0.0.9..descr
 00000030: 6970 7469 6f6e 203d 2048 6967 682d 7468  iption = High-th
 00000040: 726f 7567 6870 7574 2063 6f6d 7075 7469  roughput computi
 00000050: 6e67 2066 6c6f 770d 0a6c 6f6e 675f 6465  ng flow..long_de
 00000060: 7363 7269 7074 696f 6e20 3d20 6669 6c65  scription = file
 00000070: 3a20 5245 4144 4d45 2e6d 640d 0a6c 6f6e  : README.md..lon
 00000080: 675f 6465 7363 7269 7074 696f 6e5f 636f  g_description_co
 00000090: 6e74 656e 745f 7479 7065 203d 2074 6578  ntent_type = tex
```

