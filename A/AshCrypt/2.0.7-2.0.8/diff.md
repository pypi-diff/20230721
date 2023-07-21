# Comparing `tmp/AshCrypt-2.0.7.tar.gz` & `tmp/AshCrypt-2.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/AshCrypt-2.0.7.tar", last modified: Thu Jul 20 21:11:51 2023, max compression
+gzip compressed data, was "dist/AshCrypt-2.0.8.tar", last modified: Fri Jul 21 15:01:51 2023, max compression
```

## Comparing `AshCrypt-2.0.7.tar` & `AshCrypt-2.0.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:11:51.000000 AshCrypt-2.0.7/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:11:51.000000 AshCrypt-2.0.7/AshCrypt/
--rw-r--r--   0 runner    (1001) docker     (123)    38210 2023-07-20 21:11:40.000000 AshCrypt-2.0.7/AshCrypt/AshCryptGUI.py
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-20 21:11:40.000000 AshCrypt-2.0.7/AshCrypt/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-20 21:11:40.000000 AshCrypt-2.0.7/AshCrypt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6560 2023-07-20 21:11:40.000000 AshCrypt-2.0.7/AshCrypt/clicrypt.py
--rw-r--r--   0 runner    (1001) docker     (123)     5073 2023-07-20 21:11:40.000000 AshCrypt-2.0.7/AshCrypt/crypt.py
--rw-r--r--   0 runner    (1001) docker     (123)     8681 2023-07-20 21:11:40.000000 AshCrypt-2.0.7/AshCrypt/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-07-20 21:11:40.000000 AshCrypt-2.0.7/AshCrypt/filecrypt.py
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-20 21:11:40.000000 AshCrypt-2.0.7/AshCrypt/qr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-07-20 21:11:40.000000 AshCrypt-2.0.7/AshCrypt/textcrypt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:11:51.000000 AshCrypt-2.0.7/AshCrypt/unittests/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-20 21:11:40.000000 AshCrypt-2.0.7/AshCrypt/unittests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-07-20 21:11:40.000000 AshCrypt-2.0.7/AshCrypt/unittests/unittest_crypt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:11:51.000000 AshCrypt-2.0.7/AshCrypt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-20 21:11:51.000000 AshCrypt-2.0.7/AshCrypt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-20 21:11:51.000000 AshCrypt-2.0.7/AshCrypt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 21:11:51.000000 AshCrypt-2.0.7/AshCrypt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-20 21:11:51.000000 AshCrypt-2.0.7/AshCrypt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-20 21:11:51.000000 AshCrypt-2.0.7/AshCrypt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-20 21:11:51.000000 AshCrypt-2.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21164 2023-07-20 21:11:40.000000 AshCrypt-2.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 21:11:51.000000 AshCrypt-2.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-07-20 21:11:40.000000 AshCrypt-2.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:01:51.000000 AshCrypt-2.0.8/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:01:51.000000 AshCrypt-2.0.8/AshCrypt/
+-rw-r--r--   0 runner    (1001) docker     (123)    38210 2023-07-21 15:01:40.000000 AshCrypt-2.0.8/AshCrypt/AshCryptGUI.py
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-21 15:01:40.000000 AshCrypt-2.0.8/AshCrypt/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-21 15:01:40.000000 AshCrypt-2.0.8/AshCrypt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6560 2023-07-21 15:01:40.000000 AshCrypt-2.0.8/AshCrypt/clicrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7145 2023-07-21 15:01:40.000000 AshCrypt-2.0.8/AshCrypt/crypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8681 2023-07-21 15:01:40.000000 AshCrypt-2.0.8/AshCrypt/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-07-21 15:01:40.000000 AshCrypt-2.0.8/AshCrypt/filecrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-21 15:01:40.000000 AshCrypt-2.0.8/AshCrypt/qr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-07-21 15:01:40.000000 AshCrypt-2.0.8/AshCrypt/textcrypt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:01:51.000000 AshCrypt-2.0.8/AshCrypt/unittests/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-21 15:01:40.000000 AshCrypt-2.0.8/AshCrypt/unittests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-07-21 15:01:40.000000 AshCrypt-2.0.8/AshCrypt/unittests/unittest_crypt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:01:51.000000 AshCrypt-2.0.8/AshCrypt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-21 15:01:51.000000 AshCrypt-2.0.8/AshCrypt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-21 15:01:51.000000 AshCrypt-2.0.8/AshCrypt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 15:01:51.000000 AshCrypt-2.0.8/AshCrypt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-21 15:01:51.000000 AshCrypt-2.0.8/AshCrypt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-21 15:01:51.000000 AshCrypt-2.0.8/AshCrypt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-21 15:01:51.000000 AshCrypt-2.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21164 2023-07-21 15:01:40.000000 AshCrypt-2.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 15:01:51.000000 AshCrypt-2.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-07-21 15:01:40.000000 AshCrypt-2.0.8/setup.py
```

### Comparing `AshCrypt-2.0.7/AshCrypt/AshCryptGUI.py` & `AshCrypt-2.0.8/AshCrypt/AshCryptGUI.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-2.0.7/AshCrypt/clicrypt.py` & `AshCrypt-2.0.8/AshCrypt/clicrypt.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-2.0.7/AshCrypt/database.py` & `AshCrypt-2.0.8/AshCrypt/database.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-2.0.7/AshCrypt/filecrypt.py` & `AshCrypt-2.0.8/AshCrypt/filecrypt.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-2.0.7/AshCrypt/textcrypt.py` & `AshCrypt-2.0.8/AshCrypt/textcrypt.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-2.0.7/AshCrypt/unittests/unittest_crypt.py` & `AshCrypt-2.0.8/AshCrypt/unittests/unittest_crypt.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
+import AshCrypt.crypt as cp
 import unittest
 import struct
-import AshCrypt.crypt as cp
 
 
-class AshModuleTesting(unittest.TestCase):
+class CryptModuleTesting(unittest.TestCase):
     def setUp(self) -> None:
         self.message1 = 'Hello there testing if it works'
         self.message2 = b'this is bytes now'
         self.mainkey = '6ce113be19e898c2b98df82b7fa8efb166928925fc05574a54eb1114c3410900'
         self.ins1 = cp.Enc(message=self.message1, mainkey=self.mainkey)
         self.string_message = self.ins1.enc_to_str()
         self.bytes_message = self.ins1.enc_to_bytes()
@@ -22,15 +22,15 @@
     def test_KeyType(self):
         self.assertIs(str, type(cp.Enc.genkey()))
 
     def test_HMAC(self):
         self.assertTrue(self.bytes_message[:64] == self.ins1.hmac())
 
     def test_IV(self):
-        self.assertTrue(self.bytes_message[64:80] == self.ins1.iv)
+        self.assertTrue(self.bytes_message[64:80] == self.ins1._iv)
 
     def test_Salt(self):
         self.assertTrue(self.bytes_message[80:96] == self.ins1.salt)
 
     def test_Pepper(self):
         self.assertTrue(self.bytes_message[96:112] == self.ins1.pepper)
 
@@ -53,15 +53,15 @@
     def test_EncOutputString(self):
         self.assertIs(str, type(self.ins1.enc_to_str()))
 
     def test_HMAC_Comp(self):
         self.assertEqual(self.ins1.hmac(), self.ins2.rec_hmac)
 
     def test_IV_Comp(self):
-        self.assertEqual(self.ins1.iv, self.ins2.rec_iv)
+        self.assertEqual(self.ins1._iv, self.ins2.rec_iv)
 
     def test_Salt_Comp(self):
         self.assertEqual(self.ins1.salt, self.ins2.rec_salt)
 
     def test_Pepper_Comp(self):
         self.assertEqual(self.ins1.pepper, self.ins2.rec_pepper)
```

### Comparing `AshCrypt-2.0.7/AshCrypt.egg-info/PKG-INFO` & `AshCrypt-2.0.8/AshCrypt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AshCrypt
-Version: 2.0.7
+Version: 2.0.8
 Summary: Comprehensive AES-256 Cryptography App & library equipped with files & text handling modules along with a database module to store encrypted content.
 Home-page: https://github.com/AshGw/AES-256.git
 Author: Ashref Gwader
 Author-email: AshrefGw@proton.me
 License: UNKNOWN
 Description: # Cryptography App &  Library : AES-256
         ##  Objective ##
```

### Comparing `AshCrypt-2.0.7/PKG-INFO` & `AshCrypt-2.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AshCrypt
-Version: 2.0.7
+Version: 2.0.8
 Summary: Comprehensive AES-256 Cryptography App & library equipped with files & text handling modules along with a database module to store encrypted content.
 Home-page: https://github.com/AshGw/AES-256.git
 Author: Ashref Gwader
 Author-email: AshrefGw@proton.me
 License: UNKNOWN
 Description: # Cryptography App &  Library : AES-256
         ##  Objective ##
```

### Comparing `AshCrypt-2.0.7/README.md` & `AshCrypt-2.0.8/README.md`

 * *Files identical despite different names*

### Comparing `AshCrypt-2.0.7/setup.py` & `AshCrypt-2.0.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup , find_packages
 
 with open('AshCrypt/README.md','r') as f:
     readme = f.read()
 
 setup(
     name='AshCrypt',
-    version='2.0.7',
+    version='2.0.8',
     author='Ashref Gwader',
     author_email='AshrefGw@proton.me',
     python_requires='>=3.7',
     description="Comprehensive AES-256 Cryptography App & library equipped with files & text handling modules along with"
                 " a database module to store encrypted content.",
     long_description_content_type='text/markdown',
     long_description=readme,
```

