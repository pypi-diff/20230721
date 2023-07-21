# Comparing `tmp/adafri-0.0.46.tar.gz` & `tmp/adafri-0.0.47.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafri-0.0.46.tar", last modified: Fri Jul 21 02:56:27 2023, max compression
+gzip compressed data, was "adafri-0.0.47.tar", last modified: Fri Jul 21 06:23:57 2023, max compression
```

## Comparing `adafri-0.0.46.tar` & `adafri-0.0.47.tar`

### file list

```diff
@@ -1,53 +1,55 @@
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-21 02:56:27.801987 adafri-0.0.46/
--rw-r--r--   0 ibrahima   (502) staff       (20)      177 2023-07-21 02:56:27.801616 adafri-0.0.46/PKG-INFO
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-21 02:56:27.773625 adafri-0.0.46/adafri/
--rw-r--r--   0 ibrahima   (502) staff       (20)       80 2023-07-21 02:56:22.000000 adafri-0.0.46/adafri/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-21 02:56:27.778743 adafri-0.0.46/adafri/utils/
--rw-r--r--   0 ibrahima   (502) staff       (20)       44 2023-07-12 11:52:19.000000 adafri-0.0.46/adafri/utils/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     1268 2023-07-11 19:28:16.000000 adafri-0.0.46/adafri/utils/response.py
--rw-r--r--   0 ibrahima   (502) staff       (20)    16874 2023-07-21 02:54:06.000000 adafri-0.0.46/adafri/utils/utils.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-21 02:56:27.779499 adafri-0.0.46/adafri/v1/
--rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-16 06:12:23.000000 adafri-0.0.46/adafri/v1/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-21 02:56:27.780280 adafri-0.0.46/adafri/v1/account/
--rw-r--r--   0 ibrahima   (502) staff       (20)      151 2023-07-12 07:06:08.000000 adafri-0.0.46/adafri/v1/account/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-21 02:56:27.783007 adafri-0.0.46/adafri/v1/account/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)       91 2023-07-12 06:20:02.000000 adafri-0.0.46/adafri/v1/account/models/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     4514 2023-07-20 05:14:32.000000 adafri-0.0.46/adafri/v1/account/models/account.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     3816 2023-07-12 22:09:50.000000 adafri-0.0.46/adafri/v1/account/models/account_fields.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-21 02:56:27.783742 adafri-0.0.46/adafri/v1/auth/
--rw-r--r--   0 ibrahima   (502) staff       (20)      249 2023-07-16 05:40:34.000000 adafri-0.0.46/adafri/v1/auth/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-21 02:56:27.785023 adafri-0.0.46/adafri/v1/auth/firebase_auth/
--rw-r--r--   0 ibrahima   (502) staff       (20)       39 2023-07-12 12:02:09.000000 adafri-0.0.46/adafri/v1/auth/firebase_auth/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     1226 2023-07-13 01:57:34.000000 adafri-0.0.46/adafri/v1/auth/firebase_auth/firebase_auth.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-21 02:56:27.785970 adafri-0.0.46/adafri/v1/auth/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)        0 2023-07-12 11:05:39.000000 adafri-0.0.46/adafri/v1/auth/models/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-21 02:56:27.786725 adafri-0.0.46/adafri/v1/auth/oauth/
--rw-r--r--   0 ibrahima   (502) staff       (20)      814 2023-07-18 00:36:46.000000 adafri-0.0.46/adafri/v1/auth/oauth/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-21 02:56:27.791761 adafri-0.0.46/adafri/v1/auth/oauth/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-12 11:08:07.000000 adafri-0.0.46/adafri/v1/auth/oauth/models/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     6729 2023-07-20 06:02:29.000000 adafri-0.0.46/adafri/v1/auth/oauth/models/client.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     4857 2023-07-13 16:12:18.000000 adafri-0.0.46/adafri/v1/auth/oauth/models/client_fields.py
--rw-r--r--   0 ibrahima   (502) staff       (20)    16079 2023-07-20 08:27:11.000000 adafri-0.0.46/adafri/v1/auth/oauth/models/grant.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     3635 2023-07-19 20:20:48.000000 adafri-0.0.46/adafri/v1/auth/oauth/models/grant_fields.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     9269 2023-07-20 08:03:53.000000 adafri-0.0.46/adafri/v1/auth/oauth/models/token.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     3479 2023-07-19 01:37:50.000000 adafri-0.0.46/adafri/v1/auth/oauth/models/token_fields.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-21 02:56:27.794180 adafri-0.0.46/adafri/v1/auth/oauth/server/
--rw-r--r--   0 ibrahima   (502) staff       (20)      163 2023-07-16 05:39:01.000000 adafri-0.0.46/adafri/v1/auth/oauth/server/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     1574 2023-07-20 05:43:11.000000 adafri-0.0.46/adafri/v1/auth/oauth/server/oidc_server.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     2685 2023-07-19 19:45:35.000000 adafri-0.0.46/adafri/v1/auth/oauth/server/server.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-21 02:56:27.796285 adafri-0.0.46/adafri/v1/base/
--rw-r--r--   0 ibrahima   (502) staff       (20)       71 2023-07-12 22:38:38.000000 adafri-0.0.46/adafri/v1/base/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     4240 2023-07-13 16:13:01.000000 adafri-0.0.46/adafri/v1/base/firebase_collection.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-21 02:56:27.796954 adafri-0.0.46/adafri/v1/user/
--rw-r--r--   0 ibrahima   (502) staff       (20)      129 2023-07-12 01:27:49.000000 adafri-0.0.46/adafri/v1/user/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-21 02:56:27.800544 adafri-0.0.46/adafri/v1/user/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)       78 2023-07-12 00:55:42.000000 adafri-0.0.46/adafri/v1/user/models/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     9309 2023-07-20 05:13:59.000000 adafri-0.0.46/adafri/v1/user/models/user.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     5205 2023-07-12 04:59:49.000000 adafri-0.0.46/adafri/v1/user/models/user_fields.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-21 02:56:27.776121 adafri-0.0.46/adafri.egg-info/
--rw-r--r--   0 ibrahima   (502) staff       (20)      177 2023-07-21 02:56:27.000000 adafri-0.0.46/adafri.egg-info/PKG-INFO
--rw-r--r--   0 ibrahima   (502) staff       (20)     1167 2023-07-21 02:56:27.000000 adafri-0.0.46/adafri.egg-info/SOURCES.txt
--rw-r--r--   0 ibrahima   (502) staff       (20)        1 2023-07-21 02:56:27.000000 adafri-0.0.46/adafri.egg-info/dependency_links.txt
--rw-r--r--   0 ibrahima   (502) staff       (20)        7 2023-07-21 02:56:27.000000 adafri-0.0.46/adafri.egg-info/top_level.txt
--rw-r--r--   0 ibrahima   (502) staff       (20)       38 2023-07-21 02:56:27.802139 adafri-0.0.46/setup.cfg
--rw-r--r--   0 ibrahima   (502) staff       (20)      684 2023-07-16 01:48:05.000000 adafri-0.0.46/setup.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-21 06:23:57.280673 adafri-0.0.47/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      177 2023-07-21 06:23:57.280104 adafri-0.0.47/PKG-INFO
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-21 06:23:57.248440 adafri-0.0.47/adafri/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       80 2023-07-21 06:23:42.000000 adafri-0.0.47/adafri/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-21 06:23:57.254503 adafri-0.0.47/adafri/utils/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      101 2023-07-21 05:44:28.000000 adafri-0.0.47/adafri/utils/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1252 2023-07-21 06:19:41.000000 adafri-0.0.47/adafri/utils/country.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)      589 2023-07-21 06:23:09.000000 adafri-0.0.47/adafri/utils/phone_number.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1268 2023-07-11 19:28:16.000000 adafri-0.0.47/adafri/utils/response.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)    16874 2023-07-21 02:54:06.000000 adafri-0.0.47/adafri/utils/utils.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-21 06:23:57.255580 adafri-0.0.47/adafri/v1/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-16 06:12:23.000000 adafri-0.0.47/adafri/v1/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-21 06:23:57.256374 adafri-0.0.47/adafri/v1/account/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      151 2023-07-12 07:06:08.000000 adafri-0.0.47/adafri/v1/account/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-21 06:23:57.258696 adafri-0.0.47/adafri/v1/account/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       91 2023-07-12 06:20:02.000000 adafri-0.0.47/adafri/v1/account/models/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     4514 2023-07-20 05:14:32.000000 adafri-0.0.47/adafri/v1/account/models/account.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     3816 2023-07-12 22:09:50.000000 adafri-0.0.47/adafri/v1/account/models/account_fields.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-21 06:23:57.259591 adafri-0.0.47/adafri/v1/auth/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      249 2023-07-16 05:40:34.000000 adafri-0.0.47/adafri/v1/auth/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-21 06:23:57.260983 adafri-0.0.47/adafri/v1/auth/firebase_auth/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       39 2023-07-12 12:02:09.000000 adafri-0.0.47/adafri/v1/auth/firebase_auth/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1226 2023-07-13 01:57:34.000000 adafri-0.0.47/adafri/v1/auth/firebase_auth/firebase_auth.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-21 06:23:57.261878 adafri-0.0.47/adafri/v1/auth/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)        0 2023-07-12 11:05:39.000000 adafri-0.0.47/adafri/v1/auth/models/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-21 06:23:57.262374 adafri-0.0.47/adafri/v1/auth/oauth/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      814 2023-07-18 00:36:46.000000 adafri-0.0.47/adafri/v1/auth/oauth/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-21 06:23:57.268317 adafri-0.0.47/adafri/v1/auth/oauth/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-12 11:08:07.000000 adafri-0.0.47/adafri/v1/auth/oauth/models/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     6761 2023-07-21 06:23:32.000000 adafri-0.0.47/adafri/v1/auth/oauth/models/client.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     4857 2023-07-13 16:12:18.000000 adafri-0.0.47/adafri/v1/auth/oauth/models/client_fields.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)    16078 2023-07-21 03:05:48.000000 adafri-0.0.47/adafri/v1/auth/oauth/models/grant.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     3635 2023-07-19 20:20:48.000000 adafri-0.0.47/adafri/v1/auth/oauth/models/grant_fields.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     9363 2023-07-21 03:03:35.000000 adafri-0.0.47/adafri/v1/auth/oauth/models/token.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     3710 2023-07-21 03:04:50.000000 adafri-0.0.47/adafri/v1/auth/oauth/models/token_fields.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-21 06:23:57.271825 adafri-0.0.47/adafri/v1/auth/oauth/server/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      163 2023-07-16 05:39:01.000000 adafri-0.0.47/adafri/v1/auth/oauth/server/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1574 2023-07-20 05:43:11.000000 adafri-0.0.47/adafri/v1/auth/oauth/server/oidc_server.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     2685 2023-07-19 19:45:35.000000 adafri-0.0.47/adafri/v1/auth/oauth/server/server.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-21 06:23:57.274534 adafri-0.0.47/adafri/v1/base/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       71 2023-07-12 22:38:38.000000 adafri-0.0.47/adafri/v1/base/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     4240 2023-07-13 16:13:01.000000 adafri-0.0.47/adafri/v1/base/firebase_collection.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-21 06:23:57.275376 adafri-0.0.47/adafri/v1/user/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      129 2023-07-12 01:27:49.000000 adafri-0.0.47/adafri/v1/user/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-21 06:23:57.278799 adafri-0.0.47/adafri/v1/user/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       78 2023-07-12 00:55:42.000000 adafri-0.0.47/adafri/v1/user/models/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     9309 2023-07-20 05:13:59.000000 adafri-0.0.47/adafri/v1/user/models/user.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     5205 2023-07-12 04:59:49.000000 adafri-0.0.47/adafri/v1/user/models/user_fields.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-21 06:23:57.250842 adafri-0.0.47/adafri.egg-info/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      177 2023-07-21 06:23:57.000000 adafri-0.0.47/adafri.egg-info/PKG-INFO
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1220 2023-07-21 06:23:57.000000 adafri-0.0.47/adafri.egg-info/SOURCES.txt
+-rw-r--r--   0 ibrahima   (502) staff       (20)        1 2023-07-21 06:23:57.000000 adafri-0.0.47/adafri.egg-info/dependency_links.txt
+-rw-r--r--   0 ibrahima   (502) staff       (20)        7 2023-07-21 06:23:57.000000 adafri-0.0.47/adafri.egg-info/top_level.txt
+-rw-r--r--   0 ibrahima   (502) staff       (20)       38 2023-07-21 06:23:57.280974 adafri-0.0.47/setup.cfg
+-rw-r--r--   0 ibrahima   (502) staff       (20)      684 2023-07-16 01:48:05.000000 adafri-0.0.47/setup.py
```

### Comparing `adafri-0.0.46/adafri/utils/response.py` & `adafri-0.0.47/adafri/utils/response.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.46/adafri/utils/utils.py` & `adafri-0.0.47/adafri/utils/utils.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.46/adafri/v1/account/models/account.py` & `adafri-0.0.47/adafri/v1/account/models/account.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.46/adafri/v1/account/models/account_fields.py` & `adafri-0.0.47/adafri/v1/account/models/account_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.46/adafri/v1/auth/firebase_auth/firebase_auth.py` & `adafri-0.0.47/adafri/v1/auth/firebase_auth/firebase_auth.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.46/adafri/v1/auth/oauth/__init__.py` & `adafri-0.0.47/adafri/v1/auth/oauth/__init__.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.46/adafri/v1/auth/oauth/models/client.py` & `adafri-0.0.47/adafri/v1/auth/oauth/models/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,16 +97,16 @@
         
         if bool(client_model.name) is False:
             return ApiResponse(ResponseStatus.ERROR, StatusCode.status_400, None, Error("name required","INVALID_REQUEST", 1));
         
         if bool(client_model.uid) is False:
             return ApiResponse(ResponseStatus.ERROR, StatusCode.status_400, None, Error("uid required","INVALID_REQUEST", 1));
 
-        client_model.id = Crypto().generate_id(client_model.name+"~"+client_model.uid);
         client_model.client_id = gen_salt(24)
+        client_model.id = Crypto().generate_id(client_model.name+"~"+client_model.uid+"~"+client_model.client_id);
         client_model.client_id_issued_at = int(time.time())
         
         if client_model.token_endpoint_auth_method == 'none':
             client_model.client_secret = ''
         else:
             client_model.client_secret = gen_salt(48)
         return ApiResponse(ResponseStatus.OK, StatusCode.status_200, client_model.to_json(), None);
@@ -150,8 +150,9 @@
         allowed = set(scope_to_list(self.scope))
         return list_to_scope([s for s in scope.split() if s in allowed])
     
     def check_redirect_uri(self, redirect_uri):
         return redirect_uri in self.allowed_redirect_uris
 
     def get_client_id(self):
-        return self.client_id
+        return self.client_id
+
```

### Comparing `adafri-0.0.46/adafri/v1/auth/oauth/models/client_fields.py` & `adafri-0.0.47/adafri/v1/auth/oauth/models/client_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.46/adafri/v1/auth/oauth/models/grant.py` & `adafri-0.0.47/adafri/v1/auth/oauth/models/grant.py`

 * *Files 0% similar despite different names*

```diff
@@ -99,15 +99,15 @@
         
         if bool(authorization_code_model.to_json()) is False:
             return ApiResponse(ResponseStatus.ERROR, StatusCode.status_400, None, Error("Empty request","INVALID_REQUEST", 1)).to_json()
         
         if bool(authorization_code_model.code) is False:
             return ApiResponse(ResponseStatus.ERROR, StatusCode.status_400, None, Error("name required","INVALID_REQUEST", 1));
 
-        authorization_code_model.id = Crypto().generate_id(authorization_code_model.code+"~"+authorization_code_model.client_id);
+        authorization_code_model.id = Crypto().generate_id(authorization_code_model.uid+"~"+authorization_code_model.client_id);
         return ApiResponse(ResponseStatus.OK, StatusCode.status_200, authorization_code_model, None);
 
     def get_redirect_uri(self):
         return self.redirect_uri
     
     def get_scope(self):
        return self.scope
```

### Comparing `adafri-0.0.46/adafri/v1/auth/oauth/models/grant_fields.py` & `adafri-0.0.47/adafri/v1/auth/oauth/models/grant_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.46/adafri/v1/auth/oauth/models/token.py` & `adafri-0.0.47/adafri/v1/auth/oauth/models/token.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,16 @@
     access_token: str
     refresh_token: str
     scopes: list[str]
     scope: str
     expired_at: str
     expires_in: int
     revoked: bool
-    
+    type: str
+
     def __init__(self, token=None, **kwargs):
         (cls_object, keys, data_args) = init_class_kwargs(self, token, STANDARD_FIELDS, TokenFieldsProps, TOKEN_COLLECTION, ['id'], **kwargs)
         super().__init__(**data_args);
         for key in keys:
             setattr(self, key, cls_object[key]) 
 
 
@@ -78,20 +79,22 @@
         
         if bool(token_model.to_json()) is False:
             return ApiResponse(ResponseStatus.ERROR, StatusCode.status_400, None, Error("Empty request","INVALID_REQUEST", 1)).to_json()
         
         if bool(token_model.access_token) is False:
             return ApiResponse(ResponseStatus.ERROR, StatusCode.status_400, None, Error("name required","INVALID_REQUEST", 1));
 
-        token_model.id = Crypto().generate_id(token_model.access_token+"~"+token_model.client_id);
+        token_model.id = Crypto().generate_id(token_model.uid+"~"+token_model.client_id+"~"+token_model.type);
         return ApiResponse(ResponseStatus.OK, StatusCode.status_200, token_model, None);
     
 
     def save(self, token, request):
         model = {**token, "client_id": request.client.client_id, "uid": request.user.uid, "revoked": False}
+        if 'type' not in model:
+            model['type'] = 'app_token'
         token_generate = OAuthToken.generate(**model);
         if token_generate.status == ResponseStatus.ERROR:
             return token_generate
         docRef = OAuthToken(token_generate.data.to_json()).document_reference();
         if docRef.get().exists:
             return ApiResponse(ResponseStatus.ERROR, StatusCode.status_400, None, Error(f"Location with name {token_generate.data.id} already exist","INVALID_REQUEST", 1));
```

### Comparing `adafri-0.0.46/adafri/v1/auth/oauth/models/token_fields.py` & `adafri-0.0.47/adafri/v1/auth/oauth/models/token_fields.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     access_token = "access_token"
     refresh_token = "refresh_token"
     scopes = "scopes"
     scope = "scope"
     expires_in = "expires_in"
     expired_at = "expired_at"
     expires = "expires"
+    type = "type"
 
     @staticmethod
     def keys():
         return DictUtils.get_keys(TokenFieldsProps);
 
     @staticmethod
     def filtered_keys(field, condition=True):
@@ -75,14 +76,23 @@
         "type": str,
         "required": True,
         "mutable": True,
         "editable": False,
         "interactive": True,
         "default_value": "",
         "pickable": True
+    },
+    TokenFields.type: {
+        "type": str,
+        "required": True,
+        "mutable": True,
+        "editable": False,
+        "interactive": True,
+        "default_value": "",
+        "pickable": True
     },
     TokenFields.access_token: {
         "type": str,
         "required": True,
         "mutable": True,
         "editable": False,
         "interactive": True,
```

### Comparing `adafri-0.0.46/adafri/v1/auth/oauth/server/oidc_server.py` & `adafri-0.0.47/adafri/v1/auth/oauth/server/oidc_server.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.46/adafri/v1/auth/oauth/server/server.py` & `adafri-0.0.47/adafri/v1/auth/oauth/server/server.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.46/adafri/v1/base/firebase_collection.py` & `adafri-0.0.47/adafri/v1/base/firebase_collection.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.46/adafri/v1/user/models/user.py` & `adafri-0.0.47/adafri/v1/user/models/user.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.46/adafri/v1/user/models/user_fields.py` & `adafri-0.0.47/adafri/v1/user/models/user_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.46/adafri.egg-info/SOURCES.txt` & `adafri-0.0.47/adafri.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 setup.py
 adafri/__init__.py
 adafri.egg-info/PKG-INFO
 adafri.egg-info/SOURCES.txt
 adafri.egg-info/dependency_links.txt
 adafri.egg-info/top_level.txt
 adafri/utils/__init__.py
+adafri/utils/country.py
+adafri/utils/phone_number.py
 adafri/utils/response.py
 adafri/utils/utils.py
 adafri/v1/__init__.py
 adafri/v1/account/__init__.py
 adafri/v1/account/models/__init__.py
 adafri/v1/account/models/account.py
 adafri/v1/account/models/account_fields.py
```

### Comparing `adafri-0.0.46/setup.py` & `adafri-0.0.47/setup.py`

 * *Files identical despite different names*

