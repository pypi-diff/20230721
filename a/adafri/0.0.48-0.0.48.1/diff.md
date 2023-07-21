# Comparing `tmp/adafri-0.0.48.tar.gz` & `tmp/adafri-0.0.48.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafri-0.0.48.tar", last modified: Fri Jul 21 20:55:05 2023, max compression
+gzip compressed data, was "adafri-0.0.48.1.tar", last modified: Fri Jul 21 20:56:56 2023, max compression
```

## Comparing `adafri-0.0.48.tar` & `adafri-0.0.48.1.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-21 20:55:05.144835 adafri-0.0.48/
--rw-r--r--   0 ibrahima   (502) staff       (20)      177 2023-07-21 20:55:05.144302 adafri-0.0.48/PKG-INFO
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-21 20:55:05.108765 adafri-0.0.48/adafri/
--rw-r--r--   0 ibrahima   (502) staff       (20)       80 2023-07-21 20:54:58.000000 adafri-0.0.48/adafri/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-21 20:55:05.116623 adafri-0.0.48/adafri/utils/
--rw-r--r--   0 ibrahima   (502) staff       (20)      101 2023-07-21 05:44:28.000000 adafri-0.0.48/adafri/utils/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     1252 2023-07-21 06:19:41.000000 adafri-0.0.48/adafri/utils/country.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     1494 2023-07-21 20:54:42.000000 adafri-0.0.48/adafri/utils/phone_number.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     1268 2023-07-11 19:28:16.000000 adafri-0.0.48/adafri/utils/response.py
--rw-r--r--   0 ibrahima   (502) staff       (20)    16874 2023-07-21 02:54:06.000000 adafri-0.0.48/adafri/utils/utils.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-21 20:55:05.117880 adafri-0.0.48/adafri/v1/
--rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-16 06:12:23.000000 adafri-0.0.48/adafri/v1/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-21 20:55:05.118913 adafri-0.0.48/adafri/v1/account/
--rw-r--r--   0 ibrahima   (502) staff       (20)      151 2023-07-12 07:06:08.000000 adafri-0.0.48/adafri/v1/account/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-21 20:55:05.121498 adafri-0.0.48/adafri/v1/account/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)       91 2023-07-12 06:20:02.000000 adafri-0.0.48/adafri/v1/account/models/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     4514 2023-07-20 05:14:32.000000 adafri-0.0.48/adafri/v1/account/models/account.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     3816 2023-07-12 22:09:50.000000 adafri-0.0.48/adafri/v1/account/models/account_fields.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-21 20:55:05.122925 adafri-0.0.48/adafri/v1/auth/
--rw-r--r--   0 ibrahima   (502) staff       (20)      249 2023-07-16 05:40:34.000000 adafri-0.0.48/adafri/v1/auth/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-21 20:55:05.124781 adafri-0.0.48/adafri/v1/auth/firebase_auth/
--rw-r--r--   0 ibrahima   (502) staff       (20)       39 2023-07-12 12:02:09.000000 adafri-0.0.48/adafri/v1/auth/firebase_auth/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     1226 2023-07-13 01:57:34.000000 adafri-0.0.48/adafri/v1/auth/firebase_auth/firebase_auth.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-21 20:55:05.125366 adafri-0.0.48/adafri/v1/auth/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)        0 2023-07-12 11:05:39.000000 adafri-0.0.48/adafri/v1/auth/models/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-21 20:55:05.126071 adafri-0.0.48/adafri/v1/auth/oauth/
--rw-r--r--   0 ibrahima   (502) staff       (20)      814 2023-07-18 00:36:46.000000 adafri-0.0.48/adafri/v1/auth/oauth/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-21 20:55:05.131287 adafri-0.0.48/adafri/v1/auth/oauth/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-12 11:08:07.000000 adafri-0.0.48/adafri/v1/auth/oauth/models/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     6761 2023-07-21 06:23:32.000000 adafri-0.0.48/adafri/v1/auth/oauth/models/client.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     4857 2023-07-13 16:12:18.000000 adafri-0.0.48/adafri/v1/auth/oauth/models/client_fields.py
--rw-r--r--   0 ibrahima   (502) staff       (20)    16078 2023-07-21 03:05:48.000000 adafri-0.0.48/adafri/v1/auth/oauth/models/grant.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     3635 2023-07-19 20:20:48.000000 adafri-0.0.48/adafri/v1/auth/oauth/models/grant_fields.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     9363 2023-07-21 03:03:35.000000 adafri-0.0.48/adafri/v1/auth/oauth/models/token.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     3710 2023-07-21 03:04:50.000000 adafri-0.0.48/adafri/v1/auth/oauth/models/token_fields.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-21 20:55:05.133556 adafri-0.0.48/adafri/v1/auth/oauth/server/
--rw-r--r--   0 ibrahima   (502) staff       (20)      163 2023-07-16 05:39:01.000000 adafri-0.0.48/adafri/v1/auth/oauth/server/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     1574 2023-07-20 05:43:11.000000 adafri-0.0.48/adafri/v1/auth/oauth/server/oidc_server.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     2685 2023-07-19 19:45:35.000000 adafri-0.0.48/adafri/v1/auth/oauth/server/server.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-21 20:55:05.135270 adafri-0.0.48/adafri/v1/base/
--rw-r--r--   0 ibrahima   (502) staff       (20)       71 2023-07-12 22:38:38.000000 adafri-0.0.48/adafri/v1/base/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     4240 2023-07-13 16:13:01.000000 adafri-0.0.48/adafri/v1/base/firebase_collection.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-21 20:55:05.140544 adafri-0.0.48/adafri/v1/user/
--rw-r--r--   0 ibrahima   (502) staff       (20)      129 2023-07-12 01:27:49.000000 adafri-0.0.48/adafri/v1/user/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-21 20:55:05.143344 adafri-0.0.48/adafri/v1/user/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)       78 2023-07-12 00:55:42.000000 adafri-0.0.48/adafri/v1/user/models/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     9309 2023-07-20 05:13:59.000000 adafri-0.0.48/adafri/v1/user/models/user.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     5205 2023-07-12 04:59:49.000000 adafri-0.0.48/adafri/v1/user/models/user_fields.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-21 20:55:05.111268 adafri-0.0.48/adafri.egg-info/
--rw-r--r--   0 ibrahima   (502) staff       (20)      177 2023-07-21 20:55:04.000000 adafri-0.0.48/adafri.egg-info/PKG-INFO
--rw-r--r--   0 ibrahima   (502) staff       (20)     1220 2023-07-21 20:55:05.000000 adafri-0.0.48/adafri.egg-info/SOURCES.txt
--rw-r--r--   0 ibrahima   (502) staff       (20)        1 2023-07-21 20:55:04.000000 adafri-0.0.48/adafri.egg-info/dependency_links.txt
--rw-r--r--   0 ibrahima   (502) staff       (20)        7 2023-07-21 20:55:04.000000 adafri-0.0.48/adafri.egg-info/top_level.txt
--rw-r--r--   0 ibrahima   (502) staff       (20)       38 2023-07-21 20:55:05.145099 adafri-0.0.48/setup.cfg
--rw-r--r--   0 ibrahima   (502) staff       (20)      684 2023-07-16 01:48:05.000000 adafri-0.0.48/setup.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-21 20:56:56.932754 adafri-0.0.48.1/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      179 2023-07-21 20:56:56.932376 adafri-0.0.48.1/PKG-INFO
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-21 20:56:56.895439 adafri-0.0.48.1/adafri/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       82 2023-07-21 20:56:51.000000 adafri-0.0.48.1/adafri/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-21 20:56:56.902779 adafri-0.0.48.1/adafri/utils/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      101 2023-07-21 05:44:28.000000 adafri-0.0.48.1/adafri/utils/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1252 2023-07-21 06:19:41.000000 adafri-0.0.48.1/adafri/utils/country.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1563 2023-07-21 20:56:42.000000 adafri-0.0.48.1/adafri/utils/phone_number.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1268 2023-07-11 19:28:16.000000 adafri-0.0.48.1/adafri/utils/response.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)    16874 2023-07-21 02:54:06.000000 adafri-0.0.48.1/adafri/utils/utils.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-21 20:56:56.907462 adafri-0.0.48.1/adafri/v1/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-16 06:12:23.000000 adafri-0.0.48.1/adafri/v1/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-21 20:56:56.908402 adafri-0.0.48.1/adafri/v1/account/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      151 2023-07-12 07:06:08.000000 adafri-0.0.48.1/adafri/v1/account/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-21 20:56:56.911514 adafri-0.0.48.1/adafri/v1/account/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       91 2023-07-12 06:20:02.000000 adafri-0.0.48.1/adafri/v1/account/models/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     4514 2023-07-20 05:14:32.000000 adafri-0.0.48.1/adafri/v1/account/models/account.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     3816 2023-07-12 22:09:50.000000 adafri-0.0.48.1/adafri/v1/account/models/account_fields.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-21 20:56:56.912373 adafri-0.0.48.1/adafri/v1/auth/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      249 2023-07-16 05:40:34.000000 adafri-0.0.48.1/adafri/v1/auth/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-21 20:56:56.914029 adafri-0.0.48.1/adafri/v1/auth/firebase_auth/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       39 2023-07-12 12:02:09.000000 adafri-0.0.48.1/adafri/v1/auth/firebase_auth/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1226 2023-07-13 01:57:34.000000 adafri-0.0.48.1/adafri/v1/auth/firebase_auth/firebase_auth.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-21 20:56:56.914939 adafri-0.0.48.1/adafri/v1/auth/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)        0 2023-07-12 11:05:39.000000 adafri-0.0.48.1/adafri/v1/auth/models/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-21 20:56:56.915358 adafri-0.0.48.1/adafri/v1/auth/oauth/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      814 2023-07-18 00:36:46.000000 adafri-0.0.48.1/adafri/v1/auth/oauth/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-21 20:56:56.921946 adafri-0.0.48.1/adafri/v1/auth/oauth/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-12 11:08:07.000000 adafri-0.0.48.1/adafri/v1/auth/oauth/models/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     6761 2023-07-21 06:23:32.000000 adafri-0.0.48.1/adafri/v1/auth/oauth/models/client.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     4857 2023-07-13 16:12:18.000000 adafri-0.0.48.1/adafri/v1/auth/oauth/models/client_fields.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)    16078 2023-07-21 03:05:48.000000 adafri-0.0.48.1/adafri/v1/auth/oauth/models/grant.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     3635 2023-07-19 20:20:48.000000 adafri-0.0.48.1/adafri/v1/auth/oauth/models/grant_fields.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     9363 2023-07-21 03:03:35.000000 adafri-0.0.48.1/adafri/v1/auth/oauth/models/token.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     3710 2023-07-21 03:04:50.000000 adafri-0.0.48.1/adafri/v1/auth/oauth/models/token_fields.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-21 20:56:56.924786 adafri-0.0.48.1/adafri/v1/auth/oauth/server/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      163 2023-07-16 05:39:01.000000 adafri-0.0.48.1/adafri/v1/auth/oauth/server/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1574 2023-07-20 05:43:11.000000 adafri-0.0.48.1/adafri/v1/auth/oauth/server/oidc_server.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     2685 2023-07-19 19:45:35.000000 adafri-0.0.48.1/adafri/v1/auth/oauth/server/server.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-21 20:56:56.926591 adafri-0.0.48.1/adafri/v1/base/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       71 2023-07-12 22:38:38.000000 adafri-0.0.48.1/adafri/v1/base/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     4240 2023-07-13 16:13:01.000000 adafri-0.0.48.1/adafri/v1/base/firebase_collection.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-21 20:56:56.927403 adafri-0.0.48.1/adafri/v1/user/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      129 2023-07-12 01:27:49.000000 adafri-0.0.48.1/adafri/v1/user/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-21 20:56:56.931170 adafri-0.0.48.1/adafri/v1/user/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       78 2023-07-12 00:55:42.000000 adafri-0.0.48.1/adafri/v1/user/models/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     9309 2023-07-20 05:13:59.000000 adafri-0.0.48.1/adafri/v1/user/models/user.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     5205 2023-07-12 04:59:49.000000 adafri-0.0.48.1/adafri/v1/user/models/user_fields.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-21 20:56:56.898296 adafri-0.0.48.1/adafri.egg-info/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      179 2023-07-21 20:56:56.000000 adafri-0.0.48.1/adafri.egg-info/PKG-INFO
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1220 2023-07-21 20:56:56.000000 adafri-0.0.48.1/adafri.egg-info/SOURCES.txt
+-rw-r--r--   0 ibrahima   (502) staff       (20)        1 2023-07-21 20:56:56.000000 adafri-0.0.48.1/adafri.egg-info/dependency_links.txt
+-rw-r--r--   0 ibrahima   (502) staff       (20)        7 2023-07-21 20:56:56.000000 adafri-0.0.48.1/adafri.egg-info/top_level.txt
+-rw-r--r--   0 ibrahima   (502) staff       (20)       38 2023-07-21 20:56:56.932959 adafri-0.0.48.1/setup.cfg
+-rw-r--r--   0 ibrahima   (502) staff       (20)      684 2023-07-16 01:48:05.000000 adafri-0.0.48.1/setup.py
```

### Comparing `adafri-0.0.48/adafri/utils/country.py` & `adafri-0.0.48.1/adafri/utils/country.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.48/adafri/utils/phone_number.py` & `adafri-0.0.48.1/adafri/utils/phone_number.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,18 +4,20 @@
     number: str;
     national_number: str;
     international_number: str;
     dialCode: str;
     country_code: str;
 
     def __init__(self, number, country_code=None):
-        (
-            self.number, self.national_number, 
-            self.international_number, self.dialCode,self.country_code
-        ) = self.parse(number,country_code)
+        parse = self.parse(number,country_code);
+        if parse is not None:
+            (
+                self.number, self.national_number, 
+                self.international_number, self.dialCode,self.country_code
+            ) = parse
 
     def parse(self, _number, _country_code=None):
         try:
             number = _number
             country_code = _country_code;
             parsed = phonenumbers.parse(number, country_code);
             national_number = phonenumbers.format_number(parsed, phonenumbers.PhoneNumberFormat.NATIONAL);
```

### Comparing `adafri-0.0.48/adafri/utils/response.py` & `adafri-0.0.48.1/adafri/utils/response.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.48/adafri/utils/utils.py` & `adafri-0.0.48.1/adafri/utils/utils.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.48/adafri/v1/account/models/account.py` & `adafri-0.0.48.1/adafri/v1/account/models/account.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.48/adafri/v1/account/models/account_fields.py` & `adafri-0.0.48.1/adafri/v1/account/models/account_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.48/adafri/v1/auth/firebase_auth/firebase_auth.py` & `adafri-0.0.48.1/adafri/v1/auth/firebase_auth/firebase_auth.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.48/adafri/v1/auth/oauth/__init__.py` & `adafri-0.0.48.1/adafri/v1/auth/oauth/__init__.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.48/adafri/v1/auth/oauth/models/client.py` & `adafri-0.0.48.1/adafri/v1/auth/oauth/models/client.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.48/adafri/v1/auth/oauth/models/client_fields.py` & `adafri-0.0.48.1/adafri/v1/auth/oauth/models/client_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.48/adafri/v1/auth/oauth/models/grant.py` & `adafri-0.0.48.1/adafri/v1/auth/oauth/models/grant.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.48/adafri/v1/auth/oauth/models/grant_fields.py` & `adafri-0.0.48.1/adafri/v1/auth/oauth/models/grant_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.48/adafri/v1/auth/oauth/models/token.py` & `adafri-0.0.48.1/adafri/v1/auth/oauth/models/token.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.48/adafri/v1/auth/oauth/models/token_fields.py` & `adafri-0.0.48.1/adafri/v1/auth/oauth/models/token_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.48/adafri/v1/auth/oauth/server/oidc_server.py` & `adafri-0.0.48.1/adafri/v1/auth/oauth/server/oidc_server.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.48/adafri/v1/auth/oauth/server/server.py` & `adafri-0.0.48.1/adafri/v1/auth/oauth/server/server.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.48/adafri/v1/base/firebase_collection.py` & `adafri-0.0.48.1/adafri/v1/base/firebase_collection.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.48/adafri/v1/user/models/user.py` & `adafri-0.0.48.1/adafri/v1/user/models/user.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.48/adafri/v1/user/models/user_fields.py` & `adafri-0.0.48.1/adafri/v1/user/models/user_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.48/adafri.egg-info/SOURCES.txt` & `adafri-0.0.48.1/adafri.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafri-0.0.48/setup.py` & `adafri-0.0.48.1/setup.py`

 * *Files identical despite different names*

