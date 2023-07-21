# Comparing `tmp/lbsnstructure-1.2.0.tar.gz` & `tmp/lbsnstructure-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lbsnstructure-1.2.0.tar", last modified: Mon May 15 11:14:09 2023, max compression
+gzip compressed data, was "lbsnstructure-1.3.0.tar", last modified: Fri Jul 21 06:21:54 2023, max compression
```

## Comparing `lbsnstructure-1.2.0.tar` & `lbsnstructure-1.3.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-15 11:14:09.634899 lbsnstructure-1.2.0/
--rw-rw-rw-   0 alex      (1000) alex      (1000)     1121 2019-07-11 10:53:20.000000 lbsnstructure-1.2.0/LICENSE.md
--rw-r--r--   0 alex      (1000) alex      (1000)     3119 2023-05-15 11:14:09.632896 lbsnstructure-1.2.0/PKG-INFO
--rwxrwxrwx   0 alex      (1000) alex      (1000)     2778 2023-05-10 06:12:09.000000 lbsnstructure-1.2.0/README.md
--rwxrwxrwx   0 alex      (1000) alex      (1000)     1115 2023-05-15 11:13:22.000000 lbsnstructure-1.2.0/pyproject.toml
--rw-r--r--   0 alex      (1000) alex      (1000)       38 2023-05-15 11:14:09.635274 lbsnstructure-1.2.0/setup.cfg
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-15 11:14:09.439451 lbsnstructure-1.2.0/src/
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-15 11:14:09.609557 lbsnstructure-1.2.0/src/lbsnstructure/
--rw-rw-rw-   0 alex      (1000) alex      (1000)      647 2023-05-15 11:05:47.000000 lbsnstructure-1.2.0/src/lbsnstructure/__init__.py
--rw-r--r--   0 alex      (1000) alex      (1000)     2703 2023-05-15 10:25:53.000000 lbsnstructure-1.2.0/src/lbsnstructure/interlinkage_pb2.py
--rw-r--r--   0 alex      (1000) alex      (1000)       27 2023-05-15 10:55:05.000000 lbsnstructure-1.2.0/src/lbsnstructure/py.typed
--rw-r--r--   0 alex      (1000) alex      (1000)     5527 2023-05-15 10:25:53.000000 lbsnstructure-1.2.0/src/lbsnstructure/social_pb2.py
--rw-r--r--   0 alex      (1000) alex      (1000)    16339 2023-05-15 10:25:53.000000 lbsnstructure-1.2.0/src/lbsnstructure/social_pb2.pyi
--rw-r--r--   0 alex      (1000) alex      (1000)     4172 2023-05-15 10:25:53.000000 lbsnstructure-1.2.0/src/lbsnstructure/spatial_pb2.py
--rw-r--r--   0 alex      (1000) alex      (1000)    10723 2023-05-15 10:25:54.000000 lbsnstructure-1.2.0/src/lbsnstructure/spatial_pb2.pyi
--rw-r--r--   0 alex      (1000) alex      (1000)     2693 2023-05-15 10:25:54.000000 lbsnstructure-1.2.0/src/lbsnstructure/temporal_pb2.py
--rw-r--r--   0 alex      (1000) alex      (1000)     6292 2023-05-15 10:25:54.000000 lbsnstructure-1.2.0/src/lbsnstructure/temporal_pb2.pyi
--rw-r--r--   0 alex      (1000) alex      (1000)     5119 2023-05-15 10:25:54.000000 lbsnstructure-1.2.0/src/lbsnstructure/topical_pb2.py
--rw-r--r--   0 alex      (1000) alex      (1000)    22233 2023-05-15 10:25:54.000000 lbsnstructure-1.2.0/src/lbsnstructure/topical_pb2.pyi
--rwxrwxrwx   0 alex      (1000) alex      (1000)       22 2023-05-15 11:13:40.000000 lbsnstructure-1.2.0/src/lbsnstructure/version.py
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-15 11:14:09.631063 lbsnstructure-1.2.0/src/lbsnstructure.egg-info/
--rw-r--r--   0 alex      (1000) alex      (1000)     3119 2023-05-15 11:14:09.000000 lbsnstructure-1.2.0/src/lbsnstructure.egg-info/PKG-INFO
--rw-r--r--   0 alex      (1000) alex      (1000)      671 2023-05-15 11:14:09.000000 lbsnstructure-1.2.0/src/lbsnstructure.egg-info/SOURCES.txt
--rw-r--r--   0 alex      (1000) alex      (1000)        1 2023-05-15 11:14:09.000000 lbsnstructure-1.2.0/src/lbsnstructure.egg-info/dependency_links.txt
--rw-r--r--   0 alex      (1000) alex      (1000)        1 2023-05-15 10:48:01.000000 lbsnstructure-1.2.0/src/lbsnstructure.egg-info/not-zip-safe
--rw-r--r--   0 alex      (1000) alex      (1000)        9 2023-05-15 11:14:09.000000 lbsnstructure-1.2.0/src/lbsnstructure.egg-info/requires.txt
--rw-r--r--   0 alex      (1000) alex      (1000)       14 2023-05-15 11:14:09.000000 lbsnstructure-1.2.0/src/lbsnstructure.egg-info/top_level.txt
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-07-21 06:21:54.502486 lbsnstructure-1.3.0/
+-rw-rw-rw-   0 alex      (1000) alex      (1000)     1121 2019-07-11 10:53:20.000000 lbsnstructure-1.3.0/LICENSE.md
+-rw-r--r--   0 alex      (1000) alex      (1000)     3246 2023-07-21 06:21:54.502486 lbsnstructure-1.3.0/PKG-INFO
+-rwxrwxrwx   0 alex      (1000) alex      (1000)     2910 2023-05-15 11:26:23.000000 lbsnstructure-1.3.0/README.md
+-rwxrwxrwx   0 alex      (1000) alex      (1000)     1115 2023-05-15 11:13:22.000000 lbsnstructure-1.3.0/pyproject.toml
+-rw-r--r--   0 alex      (1000) alex      (1000)       38 2023-07-21 06:21:54.505327 lbsnstructure-1.3.0/setup.cfg
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-07-21 06:21:54.298555 lbsnstructure-1.3.0/src/
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-07-21 06:21:54.478051 lbsnstructure-1.3.0/src/lbsnstructure/
+-rw-rw-rw-   0 alex      (1000) alex      (1000)      647 2023-05-15 11:05:47.000000 lbsnstructure-1.3.0/src/lbsnstructure/__init__.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     2703 2023-07-21 06:19:59.000000 lbsnstructure-1.3.0/src/lbsnstructure/interlinkage_pb2.py
+-rw-r--r--   0 alex      (1000) alex      (1000)       27 2023-05-15 10:55:05.000000 lbsnstructure-1.3.0/src/lbsnstructure/py.typed
+-rw-r--r--   0 alex      (1000) alex      (1000)     5566 2023-07-21 06:19:59.000000 lbsnstructure-1.3.0/src/lbsnstructure/social_pb2.py
+-rw-r--r--   0 alex      (1000) alex      (1000)    16442 2023-07-21 06:19:59.000000 lbsnstructure-1.3.0/src/lbsnstructure/social_pb2.pyi
+-rw-r--r--   0 alex      (1000) alex      (1000)     4172 2023-07-21 06:19:59.000000 lbsnstructure-1.3.0/src/lbsnstructure/spatial_pb2.py
+-rw-r--r--   0 alex      (1000) alex      (1000)    10723 2023-07-21 06:19:59.000000 lbsnstructure-1.3.0/src/lbsnstructure/spatial_pb2.pyi
+-rw-r--r--   0 alex      (1000) alex      (1000)     2693 2023-07-21 06:19:59.000000 lbsnstructure-1.3.0/src/lbsnstructure/temporal_pb2.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     6292 2023-07-21 06:19:59.000000 lbsnstructure-1.3.0/src/lbsnstructure/temporal_pb2.pyi
+-rw-r--r--   0 alex      (1000) alex      (1000)     5119 2023-07-21 06:20:00.000000 lbsnstructure-1.3.0/src/lbsnstructure/topical_pb2.py
+-rw-r--r--   0 alex      (1000) alex      (1000)    22233 2023-07-21 06:20:00.000000 lbsnstructure-1.3.0/src/lbsnstructure/topical_pb2.pyi
+-rwxrwxrwx   0 alex      (1000) alex      (1000)       22 2023-07-21 06:21:22.000000 lbsnstructure-1.3.0/src/lbsnstructure/version.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-07-21 06:21:54.498855 lbsnstructure-1.3.0/src/lbsnstructure.egg-info/
+-rw-r--r--   0 alex      (1000) alex      (1000)     3246 2023-07-21 06:21:54.000000 lbsnstructure-1.3.0/src/lbsnstructure.egg-info/PKG-INFO
+-rw-r--r--   0 alex      (1000) alex      (1000)      671 2023-07-21 06:21:54.000000 lbsnstructure-1.3.0/src/lbsnstructure.egg-info/SOURCES.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)        1 2023-07-21 06:21:54.000000 lbsnstructure-1.3.0/src/lbsnstructure.egg-info/dependency_links.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)        1 2023-05-15 10:48:01.000000 lbsnstructure-1.3.0/src/lbsnstructure.egg-info/not-zip-safe
+-rw-r--r--   0 alex      (1000) alex      (1000)        9 2023-07-21 06:21:54.000000 lbsnstructure-1.3.0/src/lbsnstructure.egg-info/requires.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)       14 2023-07-21 06:21:54.000000 lbsnstructure-1.3.0/src/lbsnstructure.egg-info/top_level.txt
```

### Comparing `lbsnstructure-1.2.0/LICENSE.md` & `lbsnstructure-1.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `lbsnstructure-1.2.0/PKG-INFO` & `lbsnstructure-1.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lbsnstructure
-Version: 1.2.0
+Version: 1.3.0
 Summary: A common language independent and cross-network social-media data scheme.
 Author: Filip Krumpe, Marc Löchner
 Author-email: Alexander Dunkel <alexander.dunkel@tu-dresden.de>
 License: MIT
 Project-URL: Homepage, https://lbsn.vgiscience.org/
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -15,22 +15,25 @@
 # LBSNSTRUCTURE
 
 A python compiled version of the [common location based social network (LBSN) data structure concept](https://gitlab.vgiscience.de/lbsn/concept) (ProtoBuf) to handle cross network Social Media data in Python.
 There are several motivations for prividing a common LBSN interchange data structure. Firstly, the [GDPR](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX%3A32016R0679) directly requests Social Media Network operators to allow users to transfer accounts and data inbetween services. 
 While there are attempts by Google, Facebook etc. (see [data-transfer-project](https://github.com/google/data-transfer-project)), it is not currently possible. With this structure concept, we follow an independent road.
 A primary goal is to systematically characterize LBSN data aspects in a common scheme that enables privacy-by-design for connected software, transfer scripts and database design.
 
+The Github-repository of this protobuf-derived package can be found here:
+https://github.com/Sieboldianus/lbsnstructure-python
+
 ## Quick Start
 
 Install with:  
 ```shell
 pip install --upgrade lbsnstructure
 ```
 
-Import to python projecty with:  
+Import to python project with:  
 ```python
 import lbsnstructure as lbsn
 post = lbsn.Post()
 place = lbsn.Place()
 ```
 
 .. or compile newest version from [Protofiles](https://gitlab.vgiscience.de/lbsn/concept)
```

### Comparing `lbsnstructure-1.2.0/README.md` & `lbsnstructure-1.3.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -3,22 +3,25 @@
 # LBSNSTRUCTURE
 
 A python compiled version of the [common location based social network (LBSN) data structure concept](https://gitlab.vgiscience.de/lbsn/concept) (ProtoBuf) to handle cross network Social Media data in Python.
 There are several motivations for prividing a common LBSN interchange data structure. Firstly, the [GDPR](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX%3A32016R0679) directly requests Social Media Network operators to allow users to transfer accounts and data inbetween services. 
 While there are attempts by Google, Facebook etc. (see [data-transfer-project](https://github.com/google/data-transfer-project)), it is not currently possible. With this structure concept, we follow an independent road.
 A primary goal is to systematically characterize LBSN data aspects in a common scheme that enables privacy-by-design for connected software, transfer scripts and database design.
 
+The Github-repository of this protobuf-derived package can be found here:
+https://github.com/Sieboldianus/lbsnstructure-python
+
 ## Quick Start
 
 Install with:  
 ```shell
 pip install --upgrade lbsnstructure
 ```
 
-Import to python projecty with:  
+Import to python project with:  
 ```python
 import lbsnstructure as lbsn
 post = lbsn.Post()
 place = lbsn.Place()
 ```
 
 .. or compile newest version from [Protofiles](https://gitlab.vgiscience.de/lbsn/concept)
@@ -48,8 +51,8 @@
 For the releases available, see the [tags on this repository](/../tags). 
 The versioning (major.minor.patch) is automated using [python-semantic-release](https://github.com/relekang/python-semantic-release).
 Commit messages that follow the [Angular Commit Message Conventions](https://github.com/angular/angular.js/blob/master/DEVELOPERS.md#-git-commit-guidelines) will be automatically interpreted, 
 followed by version bumps if necessary. 
 
 ## License
 
-This project is licensed under the  MIT License.
+This project is licensed under the  MIT License.
```

### Comparing `lbsnstructure-1.2.0/pyproject.toml` & `lbsnstructure-1.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lbsnstructure-1.2.0/src/lbsnstructure/__init__.py` & `lbsnstructure-1.3.0/src/lbsnstructure/__init__.py`

 * *Files identical despite different names*

### Comparing `lbsnstructure-1.2.0/src/lbsnstructure/interlinkage_pb2.py` & `lbsnstructure-1.3.0/src/lbsnstructure/interlinkage_pb2.py`

 * *Files identical despite different names*

### Comparing `lbsnstructure-1.2.0/src/lbsnstructure/social_pb2.py` & `lbsnstructure-1.3.0/src/lbsnstructure/social_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1albsnstructure/social.proto\x12\x0elbsn.structure\x1a\x1fgoogle/protobuf/timestamp.proto\"\xc4\x03\n\x06Origin\x12\x32\n\torigin_id\x18\x01 \x01(\x0e\x32\x1f.lbsn.structure.Origin.OriginID\x12\x0c\n\x04name\x18\x02 \x01(\t\"\xf7\x02\n\x08OriginID\x12\x08\n\x04LBSN\x10\x00\x12\r\n\tINSTAGRAM\x10\x01\x12\n\n\x06\x46LICKR\x10\x02\x12\x0b\n\x07TWITTER\x10\x03\x12\x0c\n\x08\x46\x41\x43\x45\x42OOK\x10\x04\x12\x0e\n\nFOURSQUARE\x10\x05\x12\x0c\n\x08WIKIDATA\x10\x06\x12\r\n\tWIKIPEDIA\x10\x07\x12\n\n\x06REDDIT\x10\x08\x12\x0c\n\x08GEOGRAPH\x10\t\x12\x14\n\x10GOOGLEPLACEPHOTO\x10\n\x12\r\n\tPINTEREST\x10\x0b\x12\r\n\tMAPILLARY\x10\x0c\x12\x0c\n\x08SNAPCHAT\x10\r\x12\r\n\tPOKEMONGO\x10\x0e\x12\x14\n\x10WIKIMEDIACOMMONS\x10\x0f\x12\r\n\tWIKIMAPIA\x10\x10\x12\n\n\x06\x41IRBNB\x10\x11\x12\x12\n\x0ePORTALNINANTIC\x10\x12\x12\n\n\x06TIKTOK\x10\x13\x12\x0c\n\x08TELEGRAM\x10\x14\x12\x07\n\x03GAB\x10\x15\x12\t\n\x05IBIRD\x10\x16\x12\x0f\n\x0bINATURALIST\x10\x17\x12\x0f\n\x0bISPOTNATURE\x10\x18\"B\n\x0c\x43ompositeKey\x12&\n\x06origin\x18\x01 \x01(\x0b\x32\x16.lbsn.structure.Origin\x12\n\n\x02id\x18\x02 \x01(\t\"\xa1\x04\n\x04User\x12*\n\x04pkey\x18\x01 \x01(\x0b\x32\x1c.lbsn.structure.CompositeKey\x12\x11\n\tuser_name\x18\x02 \x01(\t\x12\x15\n\ruser_fullname\x18\x03 \x01(\t\x12\x0f\n\x07\x66ollows\x18\x04 \x01(\x03\x12\x10\n\x08\x66ollowed\x18\x05 \x01(\x03\x12\x13\n\x0bgroup_count\x18\x06 \x01(\x03\x12\x11\n\tbiography\x18\x07 \x01(\t\x12\x12\n\npost_count\x18\x08 \x01(\x03\x12\x0b\n\x03url\x18\t \x01(\t\x12\x12\n\nis_private\x18\n \x01(\x08\x12\x14\n\x0cis_available\x18\x0b \x01(\x08\x12/\n\ruser_language\x18\x0c \x01(\x0b\x32\x18.lbsn.structure.Language\x12\x15\n\ruser_location\x18\r \x01(\t\x12\x1a\n\x12user_location_geom\x18\x0e \x01(\t\x12\x13\n\x0bliked_count\x18\x0f \x01(\x03\x12\x30\n\x0c\x61\x63tive_since\x18\x10 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x19\n\x11profile_image_url\x18\x11 \x01(\t\x12\x15\n\ruser_timezone\x18\x12 \x01(\t\x12\x17\n\x0fuser_utc_offset\x18\x13 \x01(\x11\x12\x1a\n\x12user_groups_member\x18\x14 \x03(\t\x12\x1b\n\x13user_groups_follows\x18\x15 \x03(\t\"\xf5\x01\n\tUserGroup\x12*\n\x04pkey\x18\x01 \x01(\x0b\x32\x1c.lbsn.structure.CompositeKey\x12\x16\n\x0eusergroup_name\x18\x02 \x01(\t\x12\x1d\n\x15usergroup_description\x18\x03 \x01(\t\x12\x14\n\x0cmember_count\x18\x04 \x01(\x03\x12\x38\n\x14usergroup_createdate\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x35\n\x0fuser_owner_pkey\x18\x06 \x01(\x0b\x32\x1c.lbsn.structure.CompositeKey\"J\n\x08Language\x12\x16\n\x0elanguage_short\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x18\n\x10language_name_de\x18\x03 \x01(\tb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1albsnstructure/social.proto\x12\x0elbsn.structure\x1a\x1fgoogle/protobuf/timestamp.proto\"\xd5\x03\n\x06Origin\x12\x32\n\torigin_id\x18\x01 \x01(\x0e\x32\x1f.lbsn.structure.Origin.OriginID\x12\x0c\n\x04name\x18\x02 \x01(\t\"\x88\x03\n\x08OriginID\x12\x08\n\x04LBSN\x10\x00\x12\r\n\tINSTAGRAM\x10\x01\x12\n\n\x06\x46LICKR\x10\x02\x12\x0b\n\x07TWITTER\x10\x03\x12\x0c\n\x08\x46\x41\x43\x45\x42OOK\x10\x04\x12\x0e\n\nFOURSQUARE\x10\x05\x12\x0c\n\x08WIKIDATA\x10\x06\x12\r\n\tWIKIPEDIA\x10\x07\x12\n\n\x06REDDIT\x10\x08\x12\x0c\n\x08GEOGRAPH\x10\t\x12\x14\n\x10GOOGLEPLACEPHOTO\x10\n\x12\r\n\tPINTEREST\x10\x0b\x12\r\n\tMAPILLARY\x10\x0c\x12\x0c\n\x08SNAPCHAT\x10\r\x12\r\n\tPOKEMONGO\x10\x0e\x12\x14\n\x10WIKIMEDIACOMMONS\x10\x0f\x12\r\n\tWIKIMAPIA\x10\x10\x12\n\n\x06\x41IRBNB\x10\x11\x12\x12\n\x0ePORTALNINANTIC\x10\x12\x12\n\n\x06TIKTOK\x10\x13\x12\x0c\n\x08TELEGRAM\x10\x14\x12\x07\n\x03GAB\x10\x15\x12\t\n\x05\x45\x42IRD\x10\x16\x12\x0f\n\x0bINATURALIST\x10\x17\x12\x0f\n\x0bISPOTNATURE\x10\x18\x12\x0f\n\x0bTRIPADVISOR\x10\x19\"B\n\x0c\x43ompositeKey\x12&\n\x06origin\x18\x01 \x01(\x0b\x32\x16.lbsn.structure.Origin\x12\n\n\x02id\x18\x02 \x01(\t\"\xa1\x04\n\x04User\x12*\n\x04pkey\x18\x01 \x01(\x0b\x32\x1c.lbsn.structure.CompositeKey\x12\x11\n\tuser_name\x18\x02 \x01(\t\x12\x15\n\ruser_fullname\x18\x03 \x01(\t\x12\x0f\n\x07\x66ollows\x18\x04 \x01(\x03\x12\x10\n\x08\x66ollowed\x18\x05 \x01(\x03\x12\x13\n\x0bgroup_count\x18\x06 \x01(\x03\x12\x11\n\tbiography\x18\x07 \x01(\t\x12\x12\n\npost_count\x18\x08 \x01(\x03\x12\x0b\n\x03url\x18\t \x01(\t\x12\x12\n\nis_private\x18\n \x01(\x08\x12\x14\n\x0cis_available\x18\x0b \x01(\x08\x12/\n\ruser_language\x18\x0c \x01(\x0b\x32\x18.lbsn.structure.Language\x12\x15\n\ruser_location\x18\r \x01(\t\x12\x1a\n\x12user_location_geom\x18\x0e \x01(\t\x12\x13\n\x0bliked_count\x18\x0f \x01(\x03\x12\x30\n\x0c\x61\x63tive_since\x18\x10 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x19\n\x11profile_image_url\x18\x11 \x01(\t\x12\x15\n\ruser_timezone\x18\x12 \x01(\t\x12\x17\n\x0fuser_utc_offset\x18\x13 \x01(\x11\x12\x1a\n\x12user_groups_member\x18\x14 \x03(\t\x12\x1b\n\x13user_groups_follows\x18\x15 \x03(\t\"\xf5\x01\n\tUserGroup\x12*\n\x04pkey\x18\x01 \x01(\x0b\x32\x1c.lbsn.structure.CompositeKey\x12\x16\n\x0eusergroup_name\x18\x02 \x01(\t\x12\x1d\n\x15usergroup_description\x18\x03 \x01(\t\x12\x14\n\x0cmember_count\x18\x04 \x01(\x03\x12\x38\n\x14usergroup_createdate\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x35\n\x0fuser_owner_pkey\x18\x06 \x01(\x0b\x32\x1c.lbsn.structure.CompositeKey\"J\n\x08Language\x12\x16\n\x0elanguage_short\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x18\n\x10language_name_de\x18\x03 \x01(\tb\x06proto3')
 
 
 
 _ORIGIN = DESCRIPTOR.message_types_by_name['Origin']
 _COMPOSITEKEY = DESCRIPTOR.message_types_by_name['CompositeKey']
 _USER = DESCRIPTOR.message_types_by_name['User']
 _USERGROUP = DESCRIPTOR.message_types_by_name['UserGroup']
@@ -60,19 +60,19 @@
   })
 _sym_db.RegisterMessage(Language)
 
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   _ORIGIN._serialized_start=80
-  _ORIGIN._serialized_end=532
+  _ORIGIN._serialized_end=549
   _ORIGIN_ORIGINID._serialized_start=157
-  _ORIGIN_ORIGINID._serialized_end=532
-  _COMPOSITEKEY._serialized_start=534
-  _COMPOSITEKEY._serialized_end=600
-  _USER._serialized_start=603
-  _USER._serialized_end=1148
-  _USERGROUP._serialized_start=1151
-  _USERGROUP._serialized_end=1396
-  _LANGUAGE._serialized_start=1398
-  _LANGUAGE._serialized_end=1472
+  _ORIGIN_ORIGINID._serialized_end=549
+  _COMPOSITEKEY._serialized_start=551
+  _COMPOSITEKEY._serialized_end=617
+  _USER._serialized_start=620
+  _USER._serialized_end=1165
+  _USERGROUP._serialized_start=1168
+  _USERGROUP._serialized_end=1413
+  _LANGUAGE._serialized_start=1415
+  _LANGUAGE._serialized_end=1489
 # @@protoc_insertion_point(module_scope)
```

### Comparing `lbsnstructure-1.2.0/src/lbsnstructure/social_pb2.pyi` & `lbsnstructure-1.3.0/src/lbsnstructure/social_pb2.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -63,17 +63,18 @@
         WIKIMEDIACOMMONS: Origin._OriginID.ValueType  # 15
         WIKIMAPIA: Origin._OriginID.ValueType  # 16
         AIRBNB: Origin._OriginID.ValueType  # 17
         PORTALNINANTIC: Origin._OriginID.ValueType  # 18
         TIKTOK: Origin._OriginID.ValueType  # 19
         TELEGRAM: Origin._OriginID.ValueType  # 20
         GAB: Origin._OriginID.ValueType  # 21
-        IBIRD: Origin._OriginID.ValueType  # 22
+        EBIRD: Origin._OriginID.ValueType  # 22
         INATURALIST: Origin._OriginID.ValueType  # 23
         ISPOTNATURE: Origin._OriginID.ValueType  # 24
+        TRIPADVISOR: Origin._OriginID.ValueType  # 25
 
     class OriginID(_OriginID, metaclass=_OriginIDEnumTypeWrapper):
         """
         Predefined values for OriginID. Default origin id is LBSN (0)
         """
 
     LBSN: Origin.OriginID.ValueType  # 0
@@ -95,17 +96,18 @@
     WIKIMEDIACOMMONS: Origin.OriginID.ValueType  # 15
     WIKIMAPIA: Origin.OriginID.ValueType  # 16
     AIRBNB: Origin.OriginID.ValueType  # 17
     PORTALNINANTIC: Origin.OriginID.ValueType  # 18
     TIKTOK: Origin.OriginID.ValueType  # 19
     TELEGRAM: Origin.OriginID.ValueType  # 20
     GAB: Origin.OriginID.ValueType  # 21
-    IBIRD: Origin.OriginID.ValueType  # 22
+    EBIRD: Origin.OriginID.ValueType  # 22
     INATURALIST: Origin.OriginID.ValueType  # 23
     ISPOTNATURE: Origin.OriginID.ValueType  # 24
+    TRIPADVISOR: Origin.OriginID.ValueType  # 25
 
     ORIGIN_ID_FIELD_NUMBER: builtins.int
     NAME_FIELD_NUMBER: builtins.int
     origin_id: global___Origin.OriginID.ValueType
     """
     A unique Origin ID as a reference for the LBSN
     """
```

### Comparing `lbsnstructure-1.2.0/src/lbsnstructure/spatial_pb2.py` & `lbsnstructure-1.3.0/src/lbsnstructure/spatial_pb2.py`

 * *Files identical despite different names*

### Comparing `lbsnstructure-1.2.0/src/lbsnstructure/spatial_pb2.pyi` & `lbsnstructure-1.3.0/src/lbsnstructure/spatial_pb2.pyi`

 * *Files identical despite different names*

### Comparing `lbsnstructure-1.2.0/src/lbsnstructure/temporal_pb2.py` & `lbsnstructure-1.3.0/src/lbsnstructure/temporal_pb2.py`

 * *Files identical despite different names*

### Comparing `lbsnstructure-1.2.0/src/lbsnstructure/temporal_pb2.pyi` & `lbsnstructure-1.3.0/src/lbsnstructure/temporal_pb2.pyi`

 * *Files identical despite different names*

### Comparing `lbsnstructure-1.2.0/src/lbsnstructure/topical_pb2.py` & `lbsnstructure-1.3.0/src/lbsnstructure/topical_pb2.py`

 * *Files identical despite different names*

### Comparing `lbsnstructure-1.2.0/src/lbsnstructure/topical_pb2.pyi` & `lbsnstructure-1.3.0/src/lbsnstructure/topical_pb2.pyi`

 * *Files identical despite different names*

### Comparing `lbsnstructure-1.2.0/src/lbsnstructure.egg-info/PKG-INFO` & `lbsnstructure-1.3.0/src/lbsnstructure.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lbsnstructure
-Version: 1.2.0
+Version: 1.3.0
 Summary: A common language independent and cross-network social-media data scheme.
 Author: Filip Krumpe, Marc Löchner
 Author-email: Alexander Dunkel <alexander.dunkel@tu-dresden.de>
 License: MIT
 Project-URL: Homepage, https://lbsn.vgiscience.org/
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -15,22 +15,25 @@
 # LBSNSTRUCTURE
 
 A python compiled version of the [common location based social network (LBSN) data structure concept](https://gitlab.vgiscience.de/lbsn/concept) (ProtoBuf) to handle cross network Social Media data in Python.
 There are several motivations for prividing a common LBSN interchange data structure. Firstly, the [GDPR](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX%3A32016R0679) directly requests Social Media Network operators to allow users to transfer accounts and data inbetween services. 
 While there are attempts by Google, Facebook etc. (see [data-transfer-project](https://github.com/google/data-transfer-project)), it is not currently possible. With this structure concept, we follow an independent road.
 A primary goal is to systematically characterize LBSN data aspects in a common scheme that enables privacy-by-design for connected software, transfer scripts and database design.
 
+The Github-repository of this protobuf-derived package can be found here:
+https://github.com/Sieboldianus/lbsnstructure-python
+
 ## Quick Start
 
 Install with:  
 ```shell
 pip install --upgrade lbsnstructure
 ```
 
-Import to python projecty with:  
+Import to python project with:  
 ```python
 import lbsnstructure as lbsn
 post = lbsn.Post()
 place = lbsn.Place()
 ```
 
 .. or compile newest version from [Protofiles](https://gitlab.vgiscience.de/lbsn/concept)
```

### Comparing `lbsnstructure-1.2.0/src/lbsnstructure.egg-info/SOURCES.txt` & `lbsnstructure-1.3.0/src/lbsnstructure.egg-info/SOURCES.txt`

 * *Files identical despite different names*

