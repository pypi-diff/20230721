# Comparing `tmp/thumbor_libs_blackhand-0.2.0.tar.gz` & `tmp/thumbor_libs_blackhand-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/bthill/PYT/thumbor-libs/dist/tmpwr_pff4y/thumbor_libs_blackhand-0.2.0.tar", last modified: Thu Oct 13 13:06:01 2022, max compression
+gzip compressed data, was "dist/thumbor_libs_blackhand-0.3.0.tar", last modified: Fri Jul 21 13:00:23 2023, max compression
```

## Comparing `thumbor_libs_blackhand-0.2.0.tar` & `thumbor_libs_blackhand-0.3.0.tar`

### file list

```diff
@@ -1,34 +1,26 @@
-drwxr-xr-x   0 bthill    (1000) bthill    (1000)        0 2022-10-13 13:06:01.000000 thumbor_libs_blackhand-0.2.0/
--rw-r--r--   0 bthill    (1000) bthill    (1000)     1079 2022-10-13 13:05:18.000000 thumbor_libs_blackhand-0.2.0/LICENSE
--rw-r--r--   0 bthill    (1000) bthill    (1000)      744 2022-10-13 13:06:01.000000 thumbor_libs_blackhand-0.2.0/PKG-INFO
--rw-r--r--   0 bthill    (1000) bthill    (1000)     6632 2022-10-13 13:05:18.000000 thumbor_libs_blackhand-0.2.0/README.md
--rw-r--r--   0 bthill    (1000) bthill    (1000)       38 2022-10-13 13:06:01.000000 thumbor_libs_blackhand-0.2.0/setup.cfg
--rw-r--r--   0 bthill    (1000) bthill    (1000)     1526 2022-10-13 13:05:18.000000 thumbor_libs_blackhand-0.2.0/setup.py
-drwxr-xr-x   0 bthill    (1000) bthill    (1000)        0 2022-10-13 13:06:01.000000 thumbor_libs_blackhand-0.2.0/thumbor_libs_blackhand/
-drwxr-xr-x   0 bthill    (1000) bthill    (1000)        0 2022-10-13 13:06:01.000000 thumbor_libs_blackhand-0.2.0/thumbor_libs_blackhand/loaders/
--rw-r--r--   0 bthill    (1000) bthill    (1000)      138 2022-10-13 13:05:18.000000 thumbor_libs_blackhand-0.2.0/thumbor_libs_blackhand/loaders/__init__.py
--rw-r--r--   0 bthill    (1000) bthill    (1000)     1910 2022-10-13 13:05:18.000000 thumbor_libs_blackhand-0.2.0/thumbor_libs_blackhand/loaders/mongodb_loader.py
--rw-r--r--   0 bthill    (1000) bthill    (1000)      533 2022-10-13 13:05:18.000000 thumbor_libs_blackhand-0.2.0/thumbor_libs_blackhand/loaders/spec_http_or_specb_loader.py
--rw-r--r--   0 bthill    (1000) bthill    (1000)     2521 2022-10-13 13:05:18.000000 thumbor_libs_blackhand-0.2.0/thumbor_libs_blackhand/loaders/specb_file_fallback_file_loader.py
-drwxr-xr-x   0 bthill    (1000) bthill    (1000)        0 2022-10-13 13:06:01.000000 thumbor_libs_blackhand-0.2.0/thumbor_libs_blackhand/metrics/
--rw-r--r--   0 bthill    (1000) bthill    (1000)      138 2022-10-13 13:05:18.000000 thumbor_libs_blackhand-0.2.0/thumbor_libs_blackhand/metrics/__init__.py
-drwxr-xr-x   0 bthill    (1000) bthill    (1000)        0 2022-10-13 13:06:01.000000 thumbor_libs_blackhand-0.2.0/thumbor_libs_blackhand/mongodb/
--rw-r--r--   0 bthill    (1000) bthill    (1000)     1781 2022-10-13 13:05:18.000000 thumbor_libs_blackhand-0.2.0/thumbor_libs_blackhand/mongodb/pool_result_storage.py
-drwxr-xr-x   0 bthill    (1000) bthill    (1000)        0 2022-10-13 13:06:01.000000 thumbor_libs_blackhand-0.2.0/thumbor_libs_blackhand/result_storages/
--rw-r--r--   0 bthill    (1000) bthill    (1000)      138 2022-10-13 13:05:18.000000 thumbor_libs_blackhand-0.2.0/thumbor_libs_blackhand/result_storages/__init__.py
--rw-r--r--   0 bthill    (1000) bthill    (1000)     6534 2022-10-13 13:05:18.000000 thumbor_libs_blackhand-0.2.0/thumbor_libs_blackhand/result_storages/hybrid_result_storage.py
--rw-r--r--   0 bthill    (1000) bthill    (1000)     3893 2022-10-13 13:05:18.000000 thumbor_libs_blackhand-0.2.0/thumbor_libs_blackhand/result_storages/mongodb_legacy_result_storage.py
--rw-r--r--   0 bthill    (1000) bthill    (1000)     5442 2022-10-13 13:05:18.000000 thumbor_libs_blackhand-0.2.0/thumbor_libs_blackhand/result_storages/mongodb_result_storage.py
--rw-r--r--   0 bthill    (1000) bthill    (1000)     3889 2022-10-13 13:05:18.000000 thumbor_libs_blackhand-0.2.0/thumbor_libs_blackhand/result_storages/mongodb_webp_result_storage.py
-drwxr-xr-x   0 bthill    (1000) bthill    (1000)        0 2022-10-13 13:06:01.000000 thumbor_libs_blackhand-0.2.0/thumbor_libs_blackhand/storages/
--rw-r--r--   0 bthill    (1000) bthill    (1000)      138 2022-10-13 13:05:18.000000 thumbor_libs_blackhand-0.2.0/thumbor_libs_blackhand/storages/__init__.py
--rw-r--r--   0 bthill    (1000) bthill    (1000)     4401 2022-10-13 13:05:18.000000 thumbor_libs_blackhand-0.2.0/thumbor_libs_blackhand/storages/mongodb_webp_storage.py
-drwxr-xr-x   0 bthill    (1000) bthill    (1000)        0 2022-10-13 13:06:01.000000 thumbor_libs_blackhand-0.2.0/thumbor_libs_blackhand/url_signers/
--rw-r--r--   0 bthill    (1000) bthill    (1000)      138 2022-10-13 13:05:18.000000 thumbor_libs_blackhand-0.2.0/thumbor_libs_blackhand/url_signers/__init__.py
--rw-r--r--   0 bthill    (1000) bthill    (1000)      583 2022-10-13 13:05:18.000000 thumbor_libs_blackhand-0.2.0/thumbor_libs_blackhand/url_signers/base64_hmac_sha1_trim.py
-drwxr-xr-x   0 bthill    (1000) bthill    (1000)        0 2022-10-13 13:06:01.000000 thumbor_libs_blackhand-0.2.0/thumbor_libs_blackhand.egg-info/
--rw-r--r--   0 bthill    (1000) bthill    (1000)      744 2022-10-13 13:06:01.000000 thumbor_libs_blackhand-0.2.0/thumbor_libs_blackhand.egg-info/PKG-INFO
--rw-r--r--   0 bthill    (1000) bthill    (1000)     1099 2022-10-13 13:06:01.000000 thumbor_libs_blackhand-0.2.0/thumbor_libs_blackhand.egg-info/SOURCES.txt
--rw-r--r--   0 bthill    (1000) bthill    (1000)        1 2022-10-13 13:06:01.000000 thumbor_libs_blackhand-0.2.0/thumbor_libs_blackhand.egg-info/dependency_links.txt
--rw-r--r--   0 bthill    (1000) bthill    (1000)       30 2022-10-13 13:06:01.000000 thumbor_libs_blackhand-0.2.0/thumbor_libs_blackhand.egg-info/requires.txt
--rw-r--r--   0 bthill    (1000) bthill    (1000)       23 2022-10-13 13:06:01.000000 thumbor_libs_blackhand-0.2.0/thumbor_libs_blackhand.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 13:00:23.000000 thumbor_libs_blackhand-0.3.0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 13:00:23.000000 thumbor_libs_blackhand-0.3.0/thumbor_libs_blackhand/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 13:00:23.000000 thumbor_libs_blackhand-0.3.0/thumbor_libs_blackhand/loaders/
+-rw-rw-r--   0 root         (0) root         (0)      138 2023-07-21 12:49:31.000000 thumbor_libs_blackhand-0.3.0/thumbor_libs_blackhand/loaders/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1910 2023-07-21 12:49:31.000000 thumbor_libs_blackhand-0.3.0/thumbor_libs_blackhand/loaders/mongodb_loader.py
+-rw-rw-r--   0 root         (0) root         (0)      533 2023-07-21 12:49:31.000000 thumbor_libs_blackhand-0.3.0/thumbor_libs_blackhand/loaders/spec_http_or_specb_loader.py
+-rw-rw-r--   0 root         (0) root         (0)     2521 2023-07-21 12:49:31.000000 thumbor_libs_blackhand-0.3.0/thumbor_libs_blackhand/loaders/specb_file_fallback_file_loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 13:00:23.000000 thumbor_libs_blackhand-0.3.0/thumbor_libs_blackhand/metrics/
+-rw-rw-r--   0 root         (0) root         (0)      138 2023-07-21 12:49:31.000000 thumbor_libs_blackhand-0.3.0/thumbor_libs_blackhand/metrics/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 13:00:23.000000 thumbor_libs_blackhand-0.3.0/thumbor_libs_blackhand/mongodb/
+-rw-rw-r--   0 root         (0) root         (0)     1781 2023-07-21 12:49:31.000000 thumbor_libs_blackhand-0.3.0/thumbor_libs_blackhand/mongodb/pool_result_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 13:00:23.000000 thumbor_libs_blackhand-0.3.0/thumbor_libs_blackhand/result_storages/
+-rw-rw-r--   0 root         (0) root         (0)      138 2023-07-21 12:49:31.000000 thumbor_libs_blackhand-0.3.0/thumbor_libs_blackhand/result_storages/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     6672 2023-07-21 12:49:31.000000 thumbor_libs_blackhand-0.3.0/thumbor_libs_blackhand/result_storages/hybrid_result_storage.py
+-rw-rw-r--   0 root         (0) root         (0)     3893 2023-07-21 12:49:31.000000 thumbor_libs_blackhand-0.3.0/thumbor_libs_blackhand/result_storages/mongodb_legacy_result_storage.py
+-rw-rw-r--   0 root         (0) root         (0)     5442 2023-07-21 12:49:31.000000 thumbor_libs_blackhand-0.3.0/thumbor_libs_blackhand/result_storages/mongodb_result_storage.py
+-rw-rw-r--   0 root         (0) root         (0)     5781 2023-07-21 12:49:31.000000 thumbor_libs_blackhand-0.3.0/thumbor_libs_blackhand/result_storages/mongodb_result_storage_v3.py
+-rw-rw-r--   0 root         (0) root         (0)     3889 2023-07-21 12:49:31.000000 thumbor_libs_blackhand-0.3.0/thumbor_libs_blackhand/result_storages/mongodb_webp_result_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 13:00:23.000000 thumbor_libs_blackhand-0.3.0/thumbor_libs_blackhand/storages/
+-rw-rw-r--   0 root         (0) root         (0)      138 2023-07-21 12:49:31.000000 thumbor_libs_blackhand-0.3.0/thumbor_libs_blackhand/storages/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     4401 2023-07-21 12:49:31.000000 thumbor_libs_blackhand-0.3.0/thumbor_libs_blackhand/storages/mongodb_webp_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 13:00:23.000000 thumbor_libs_blackhand-0.3.0/thumbor_libs_blackhand/url_signers/
+-rw-rw-r--   0 root         (0) root         (0)      138 2023-07-21 12:49:31.000000 thumbor_libs_blackhand-0.3.0/thumbor_libs_blackhand/url_signers/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      583 2023-07-21 12:49:31.000000 thumbor_libs_blackhand-0.3.0/thumbor_libs_blackhand/url_signers/base64_hmac_sha1_trim.py
+-rw-rw-r--   0 root         (0) root         (0)     1526 2023-07-21 12:49:31.000000 thumbor_libs_blackhand-0.3.0/setup.py
+-rw-r--r--   0 root         (0) root         (0)      761 2023-07-21 13:00:23.000000 thumbor_libs_blackhand-0.3.0/PKG-INFO
```

### Comparing `thumbor_libs_blackhand-0.2.0/PKG-INFO` & `thumbor_libs_blackhand-0.3.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.1
 Name: thumbor_libs_blackhand
-Version: 0.2.0
+Version: 0.3.0
 Summary: libs thumbor
 Home-page: https://github.com/Bkhand/thumbor_libs_blackhand
 Author: Bertrand Thill
 Author-email: github@blackhand.org
 License: GNU
+Description: This module enable mongodb support and fallback for thumbor.
+        
 Keywords: thumbor,fallback,images,nfs,mongodb
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: French
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Multimedia :: Graphics :: Presentation
-License-File: LICENSE
-
-This module enable mongodb support and fallback for thumbor.
```

### Comparing `thumbor_libs_blackhand-0.2.0/setup.py` & `thumbor_libs_blackhand-0.3.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # http://www.opensource.org/licenses/mit-license
 
 
 from distutils.core import setup
 
 setup(
     name = "thumbor_libs_blackhand",
-    version = "0.2.0",
+    version = "0.3.0",
     description = "libs thumbor",
     author = "Bertrand Thill",
     author_email = "github@blackhand.org",
     keywords = ["thumbor", "fallback", "images", "nfs", "mongodb"],
     license = 'GNU',
     url = 'https://github.com/Bkhand/thumbor_libs_blackhand',
     packages=[
```

### Comparing `thumbor_libs_blackhand-0.2.0/thumbor_libs_blackhand/loaders/mongodb_loader.py` & `thumbor_libs_blackhand-0.3.0/thumbor_libs_blackhand/loaders/mongodb_loader.py`

 * *Files identical despite different names*

### Comparing `thumbor_libs_blackhand-0.2.0/thumbor_libs_blackhand/loaders/spec_http_or_specb_loader.py` & `thumbor_libs_blackhand-0.3.0/thumbor_libs_blackhand/loaders/spec_http_or_specb_loader.py`

 * *Files identical despite different names*

### Comparing `thumbor_libs_blackhand-0.2.0/thumbor_libs_blackhand/loaders/specb_file_fallback_file_loader.py` & `thumbor_libs_blackhand-0.3.0/thumbor_libs_blackhand/loaders/specb_file_fallback_file_loader.py`

 * *Files identical despite different names*

### Comparing `thumbor_libs_blackhand-0.2.0/thumbor_libs_blackhand/mongodb/pool_result_storage.py` & `thumbor_libs_blackhand-0.3.0/thumbor_libs_blackhand/mongodb/pool_result_storage.py`

 * *Files identical despite different names*

### Comparing `thumbor_libs_blackhand-0.2.0/thumbor_libs_blackhand/result_storages/hybrid_result_storage.py` & `thumbor_libs_blackhand-0.3.0/thumbor_libs_blackhand/result_storages/hybrid_result_storage.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,15 +43,15 @@
           uric = ('mongodb://'+ user +':' + password + '@' + self.context.config.MONGO_RESULT_STORAGE_SERVER_HOSTS
                   + '/?authSource=' + self.context.config.MONGO_RESULT_STORAGE_SERVER_DB
                   + "&replicaSet=" + self.context.config.MONGO_RESULT_STORAGE_SERVER_REPLICASET
                   + "&readPreference=" + self.context.config.MONGO_RESULT_STORAGE_SERVER_READ_PREFERENCE)
 
         db_name = self.context.config.MONGO_RESULT_STORAGE_SERVER_DB
         col_name = self.context.config.MONGO_RESULT_STORAGE_SERVER_COLLECTION
-        
+
         try:
             uri = self.context.config.MONGO_RESULT_STORAGE_URI
         except AttributeError:
             uri=uric
 
         try:
             host = self.context.config.MONGO_RESULT_STORAGE_SERVER_HOST
@@ -107,21 +107,21 @@
         return self.context.config.RESULT_STORAGE_EXPIRATION_SECONDS
 
     async def put(self, image_bytes):
         key = self.get_key_from_request()
         #max_age = self.get_max_age()
         #result_ttl = self.get_max_age()
         try:
-            CACHE_PATH = self.context.config.CACHE_PATH           
+            CACHE_PATH = self.context.config.CACHE_PATH
         except AttributeError:
             raise
-
-        mkpath = (CACHE_PATH + '/' + datetime.now().strftime('%Y') + '/' 
-                  + datetime.now().strftime('%m') + '/' + datetime.now().strftime('%d') 
+        imgpath = ( datetime.now().strftime('%Y') + '/'
+                  + datetime.now().strftime('%m') + '/' + datetime.now().strftime('%d')
                   + '/' + datetime.now().strftime('%H'))
+        mkpath = (CACHE_PATH + '/' + imgpath)
         self.ensure_dir(mkpath)
 
         #os.makedirs(mkpath)
         ref_img = ''
         ref_img = re.findall(r'/[a-zA-Z0-9]{24}(?:$|/)', key)
         if ref_img:
             ref_img2 = ref_img[0].replace('/','')
@@ -140,15 +140,15 @@
             'path': key,
             'created_at': datetime.utcnow(),
             'data': "",
             'metadata': metadata,
             'content_type': BaseEngine.get_mimetype(image_bytes),
             'ref_id': ref_img2,
             'content_length' : len(image_bytes),
-            'cache_path': mkpath,
+            'cache_path': imgpath,
             'cache_id' : cache_id
             }
         doc_cpm = dict(doc)
 
 
         fichier = open(endingpath, "wb")
         try:
@@ -161,15 +161,18 @@
         return key
 
 
     async def get(self):
 
         key = self.get_key_from_request()
         logger.debug("[RESULT_STORAGE] image not found at %s", key)
-
+        try:
+            CACHE_PATH = self.context.config.CACHE_PATH
+        except AttributeError:
+            raise
         age = datetime.utcnow() - timedelta(
             seconds=self.get_max_age()
         )
         stored = await self.storage.find_one({
             'path': key,
             'created_at': {
                 '$gte': age
@@ -191,16 +194,16 @@
         metadata = stored['metadata']
         metadata['LastModified'] = stored['created_at'].replace(
             tzinfo=pytz.utc
         )
         metadata['Cache-Control'] = "max-age=60,public"
         metadata['ContentLength'] = stored['content_length']
         metadata['ContentType'] = stored['content_type']
-        cachefile = stored['cache_path'] + "/" + stored['cache_id']
-      
+        cachefile = CACHE_PATH + '/' + stored['cache_path'] + "/" + stored['cache_id']
+
         fichier = open(cachefile, "rb")
         try:
             tosend = fichier.read()
         finally:
             fichier.close()
 
         return ResultStorageResult(
```

### Comparing `thumbor_libs_blackhand-0.2.0/thumbor_libs_blackhand/result_storages/mongodb_legacy_result_storage.py` & `thumbor_libs_blackhand-0.3.0/thumbor_libs_blackhand/result_storages/mongodb_legacy_result_storage.py`

 * *Files identical despite different names*

### Comparing `thumbor_libs_blackhand-0.2.0/thumbor_libs_blackhand/result_storages/mongodb_result_storage.py` & `thumbor_libs_blackhand-0.3.0/thumbor_libs_blackhand/result_storages/mongodb_result_storage.py`

 * *Files identical despite different names*

### Comparing `thumbor_libs_blackhand-0.2.0/thumbor_libs_blackhand/result_storages/mongodb_webp_result_storage.py` & `thumbor_libs_blackhand-0.3.0/thumbor_libs_blackhand/result_storages/mongodb_webp_result_storage.py`

 * *Files identical despite different names*

### Comparing `thumbor_libs_blackhand-0.2.0/thumbor_libs_blackhand/storages/mongodb_webp_storage.py` & `thumbor_libs_blackhand-0.3.0/thumbor_libs_blackhand/storages/mongodb_webp_storage.py`

 * *Files identical despite different names*

### Comparing `thumbor_libs_blackhand-0.2.0/thumbor_libs_blackhand/url_signers/base64_hmac_sha1_trim.py` & `thumbor_libs_blackhand-0.3.0/thumbor_libs_blackhand/url_signers/base64_hmac_sha1_trim.py`

 * *Files identical despite different names*

