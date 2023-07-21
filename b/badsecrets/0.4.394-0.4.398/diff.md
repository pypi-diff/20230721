# Comparing `tmp/badsecrets-0.4.394.tar.gz` & `tmp/badsecrets-0.4.398.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "badsecrets-0.4.394.tar", max compression
+gzip compressed data, was "badsecrets-0.4.398.tar", max compression
```

## Comparing `badsecrets-0.4.394.tar` & `badsecrets-0.4.398.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0    35149 2023-07-21 03:20:42.242225 badsecrets-0.4.394/LICENSE
--rw-r--r--   0        0        0    32418 2023-07-21 03:20:42.242225 badsecrets-0.4.394/README.md
--rw-r--r--   0        0        0      711 2023-07-21 03:20:42.242225 badsecrets-0.4.394/badsecrets/__init__.py
--rw-r--r--   0        0        0     7763 2023-07-21 03:20:42.242225 badsecrets-0.4.394/badsecrets/base.py
--rw-r--r--   0        0        0      233 2023-07-21 03:20:42.242225 badsecrets-0.4.394/badsecrets/errors.py
--rw-r--r--   0        0        0        0 2023-07-21 03:20:42.242225 badsecrets-0.4.394/badsecrets/examples/__init__.py
--rwxr-xr-x   0        0        0     4210 2023-07-21 03:20:42.242225 badsecrets-0.4.394/badsecrets/examples/blacklist3r.py
--rwxr-xr-x   0        0        0     7939 2023-07-21 03:20:42.242225 badsecrets-0.4.394/badsecrets/examples/cli.py
--rwxr-xr-x   0        0        0     3544 2023-07-21 03:20:42.242225 badsecrets-0.4.394/badsecrets/examples/symfony_knownkey.py
--rwxr-xr-x   0        0        0    10597 2023-07-21 03:20:42.246225 badsecrets-0.4.394/badsecrets/examples/telerik_knownkey.py
--rw-r--r--   0        0        0     5076 2023-07-21 03:20:42.246225 badsecrets-0.4.394/badsecrets/helpers.py
--rw-r--r--   0        0        0        0 2023-07-21 03:20:42.246225 badsecrets-0.4.394/badsecrets/modules/__init__.py
--rw-r--r--   0        0        0    10468 2023-07-21 03:20:42.246225 badsecrets-0.4.394/badsecrets/modules/aspnet_viewstate.py
--rw-r--r--   0        0        0     1006 2023-07-21 03:20:42.246225 badsecrets-0.4.394/badsecrets/modules/django_signedcookies.py
--rw-r--r--   0        0        0     2867 2023-07-21 03:20:42.246225 badsecrets-0.4.394/badsecrets/modules/express_signedcookies_cs.py
--rw-r--r--   0        0        0     2145 2023-07-21 03:20:42.246225 badsecrets-0.4.394/badsecrets/modules/express_signedcookies_es.py
--rw-r--r--   0        0        0     1120 2023-07-21 03:20:42.246225 badsecrets-0.4.394/badsecrets/modules/flask_signedcookies.py
--rw-r--r--   0        0        0     4087 2023-07-21 03:20:42.246225 badsecrets-0.4.394/badsecrets/modules/generic_jwt.py
--rw-r--r--   0        0        0    14881 2023-07-21 03:20:42.246225 badsecrets-0.4.394/badsecrets/modules/jsf_viewstate.py
--rw-r--r--   0        0        0     2192 2023-07-21 03:20:42.246225 badsecrets-0.4.394/badsecrets/modules/laravel_signedcookies.py
--rw-r--r--   0        0        0     1958 2023-07-21 03:20:42.246225 badsecrets-0.4.394/badsecrets/modules/peoplesoft_pstoken.py
--rw-r--r--   0        0        0     3097 2023-07-21 03:20:42.246225 badsecrets-0.4.394/badsecrets/modules/rails_secretkeybase.py
--rw-r--r--   0        0        0     2963 2023-07-21 03:20:42.246225 badsecrets-0.4.394/badsecrets/modules/symfony_signedurl.py
--rw-r--r--   0        0        0     5002 2023-07-21 03:20:42.246225 badsecrets-0.4.394/badsecrets/modules/telerik_encryptionkey.py
--rw-r--r--   0        0        0     3776 2023-07-21 03:20:42.246225 badsecrets-0.4.394/badsecrets/modules/telerik_hashkey.py
--rw-r--r--   0        0        0   654096 2023-07-21 03:20:42.250225 badsecrets-0.4.394/badsecrets/resources/aspnet_machinekeys.txt
--rw-r--r--   0        0        0    31178 2023-07-21 03:20:42.250225 badsecrets-0.4.394/badsecrets/resources/django_secret_keys.txt
--rw-r--r--   0        0        0    40993 2023-07-21 03:20:42.250225 badsecrets-0.4.394/badsecrets/resources/express_session_secrets.txt
--rw-r--r--   0        0        0  1777603 2023-07-21 03:20:42.270227 badsecrets-0.4.394/badsecrets/resources/flask_secret_keys.txt
--rw-r--r--   0        0        0       87 2023-07-21 03:20:42.270227 badsecrets-0.4.394/badsecrets/resources/jsf_viewstate_passwords.txt
--rw-r--r--   0        0        0     1257 2023-07-21 03:20:42.270227 badsecrets-0.4.394/badsecrets/resources/jsf_viewstate_passwords_b64.txt
--rw-r--r--   0        0        0     7785 2023-07-21 03:20:42.270227 badsecrets-0.4.394/badsecrets/resources/jwt_rsakeys_private.txt
--rw-r--r--   0        0        0     2122 2023-07-21 03:20:42.270227 badsecrets-0.4.394/badsecrets/resources/jwt_rsakeys_public.txt
--rw-r--r--   0        0        0   113170 2023-07-21 03:20:42.270227 badsecrets-0.4.394/badsecrets/resources/jwt_secrets.txt
--rw-r--r--   0        0        0    45086 2023-07-21 03:20:42.270227 badsecrets-0.4.394/badsecrets/resources/laravel_app_keys.txt
--rw-r--r--   0        0        0       78 2023-07-21 03:20:42.270227 badsecrets-0.4.394/badsecrets/resources/peoplesoft_passwords.txt
--rw-r--r--   0        0        0     6184 2023-07-21 03:20:42.270227 badsecrets-0.4.394/badsecrets/resources/rails_secret_key_base.txt
--rw-r--r--   0        0        0     3009 2023-07-21 03:20:42.270227 badsecrets-0.4.394/badsecrets/resources/symfony_appsecret.txt
--rw-r--r--   0        0        0    18037 2023-07-21 03:20:42.270227 badsecrets-0.4.394/badsecrets/resources/telerik_encryption_keys.txt
--rw-r--r--   0        0        0    17990 2023-07-21 03:20:42.270227 badsecrets-0.4.394/badsecrets/resources/telerik_hash_keys.txt
--rw-r--r--   0        0        0    76516 2023-07-21 03:20:42.274227 badsecrets-0.4.394/badsecrets/resources/top_10000_passwords.txt
--rw-r--r--   0        0        0      957 2023-07-21 03:21:08.551783 badsecrets-0.4.394/pyproject.toml
--rw-r--r--   0        0        0    33272 1970-01-01 00:00:00.000000 badsecrets-0.4.394/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-21 20:37:42.332475 badsecrets-0.4.398/LICENSE
+-rw-r--r--   0        0        0    32418 2023-07-21 20:37:42.332475 badsecrets-0.4.398/README.md
+-rw-r--r--   0        0        0      711 2023-07-21 20:37:42.332475 badsecrets-0.4.398/badsecrets/__init__.py
+-rw-r--r--   0        0        0     7763 2023-07-21 20:37:42.332475 badsecrets-0.4.398/badsecrets/base.py
+-rw-r--r--   0        0        0      233 2023-07-21 20:37:42.332475 badsecrets-0.4.398/badsecrets/errors.py
+-rw-r--r--   0        0        0        0 2023-07-21 20:37:42.332475 badsecrets-0.4.398/badsecrets/examples/__init__.py
+-rwxr-xr-x   0        0        0     4210 2023-07-21 20:37:42.332475 badsecrets-0.4.398/badsecrets/examples/blacklist3r.py
+-rwxr-xr-x   0        0        0     7939 2023-07-21 20:37:42.332475 badsecrets-0.4.398/badsecrets/examples/cli.py
+-rwxr-xr-x   0        0        0     3544 2023-07-21 20:37:42.332475 badsecrets-0.4.398/badsecrets/examples/symfony_knownkey.py
+-rwxr-xr-x   0        0        0    10597 2023-07-21 20:37:42.332475 badsecrets-0.4.398/badsecrets/examples/telerik_knownkey.py
+-rw-r--r--   0        0        0     5076 2023-07-21 20:37:42.332475 badsecrets-0.4.398/badsecrets/helpers.py
+-rw-r--r--   0        0        0        0 2023-07-21 20:37:42.332475 badsecrets-0.4.398/badsecrets/modules/__init__.py
+-rw-r--r--   0        0        0    10468 2023-07-21 20:37:42.332475 badsecrets-0.4.398/badsecrets/modules/aspnet_viewstate.py
+-rw-r--r--   0        0        0     1006 2023-07-21 20:37:42.332475 badsecrets-0.4.398/badsecrets/modules/django_signedcookies.py
+-rw-r--r--   0        0        0     2867 2023-07-21 20:37:42.332475 badsecrets-0.4.398/badsecrets/modules/express_signedcookies_cs.py
+-rw-r--r--   0        0        0     2287 2023-07-21 20:37:42.332475 badsecrets-0.4.398/badsecrets/modules/express_signedcookies_es.py
+-rw-r--r--   0        0        0     1120 2023-07-21 20:37:42.332475 badsecrets-0.4.398/badsecrets/modules/flask_signedcookies.py
+-rw-r--r--   0        0        0     4087 2023-07-21 20:37:42.332475 badsecrets-0.4.398/badsecrets/modules/generic_jwt.py
+-rw-r--r--   0        0        0    14881 2023-07-21 20:37:42.332475 badsecrets-0.4.398/badsecrets/modules/jsf_viewstate.py
+-rw-r--r--   0        0        0     2192 2023-07-21 20:37:42.332475 badsecrets-0.4.398/badsecrets/modules/laravel_signedcookies.py
+-rw-r--r--   0        0        0     1958 2023-07-21 20:37:42.332475 badsecrets-0.4.398/badsecrets/modules/peoplesoft_pstoken.py
+-rw-r--r--   0        0        0     3097 2023-07-21 20:37:42.332475 badsecrets-0.4.398/badsecrets/modules/rails_secretkeybase.py
+-rw-r--r--   0        0        0     2963 2023-07-21 20:37:42.332475 badsecrets-0.4.398/badsecrets/modules/symfony_signedurl.py
+-rw-r--r--   0        0        0     5002 2023-07-21 20:37:42.332475 badsecrets-0.4.398/badsecrets/modules/telerik_encryptionkey.py
+-rw-r--r--   0        0        0     3776 2023-07-21 20:37:42.332475 badsecrets-0.4.398/badsecrets/modules/telerik_hashkey.py
+-rw-r--r--   0        0        0   654096 2023-07-21 20:37:42.336475 badsecrets-0.4.398/badsecrets/resources/aspnet_machinekeys.txt
+-rw-r--r--   0        0        0    31178 2023-07-21 20:37:42.336475 badsecrets-0.4.398/badsecrets/resources/django_secret_keys.txt
+-rw-r--r--   0        0        0    40993 2023-07-21 20:37:42.336475 badsecrets-0.4.398/badsecrets/resources/express_session_secrets.txt
+-rw-r--r--   0        0        0  1777603 2023-07-21 20:37:42.356476 badsecrets-0.4.398/badsecrets/resources/flask_secret_keys.txt
+-rw-r--r--   0        0        0       87 2023-07-21 20:37:42.356476 badsecrets-0.4.398/badsecrets/resources/jsf_viewstate_passwords.txt
+-rw-r--r--   0        0        0     1257 2023-07-21 20:37:42.356476 badsecrets-0.4.398/badsecrets/resources/jsf_viewstate_passwords_b64.txt
+-rw-r--r--   0        0        0     7785 2023-07-21 20:37:42.356476 badsecrets-0.4.398/badsecrets/resources/jwt_rsakeys_private.txt
+-rw-r--r--   0        0        0     2122 2023-07-21 20:37:42.356476 badsecrets-0.4.398/badsecrets/resources/jwt_rsakeys_public.txt
+-rw-r--r--   0        0        0   113170 2023-07-21 20:37:42.356476 badsecrets-0.4.398/badsecrets/resources/jwt_secrets.txt
+-rw-r--r--   0        0        0    45086 2023-07-21 20:37:42.356476 badsecrets-0.4.398/badsecrets/resources/laravel_app_keys.txt
+-rw-r--r--   0        0        0       78 2023-07-21 20:37:42.356476 badsecrets-0.4.398/badsecrets/resources/peoplesoft_passwords.txt
+-rw-r--r--   0        0        0     6184 2023-07-21 20:37:42.356476 badsecrets-0.4.398/badsecrets/resources/rails_secret_key_base.txt
+-rw-r--r--   0        0        0     3009 2023-07-21 20:37:42.356476 badsecrets-0.4.398/badsecrets/resources/symfony_appsecret.txt
+-rw-r--r--   0        0        0    18037 2023-07-21 20:37:42.356476 badsecrets-0.4.398/badsecrets/resources/telerik_encryption_keys.txt
+-rw-r--r--   0        0        0    17990 2023-07-21 20:37:42.360476 badsecrets-0.4.398/badsecrets/resources/telerik_hash_keys.txt
+-rw-r--r--   0        0        0    76516 2023-07-21 20:37:42.360476 badsecrets-0.4.398/badsecrets/resources/top_10000_passwords.txt
+-rw-r--r--   0        0        0      957 2023-07-21 20:38:10.452760 badsecrets-0.4.398/pyproject.toml
+-rw-r--r--   0        0        0    33272 1970-01-01 00:00:00.000000 badsecrets-0.4.398/PKG-INFO
```

### Comparing `badsecrets-0.4.394/LICENSE` & `badsecrets-0.4.398/LICENSE`

 * *Files identical despite different names*

### Comparing `badsecrets-0.4.394/README.md` & `badsecrets-0.4.398/README.md`

 * *Files identical despite different names*

### Comparing `badsecrets-0.4.394/badsecrets/__init__.py` & `badsecrets-0.4.398/badsecrets/__init__.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.4.394/badsecrets/base.py` & `badsecrets-0.4.398/badsecrets/base.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.4.394/badsecrets/examples/blacklist3r.py` & `badsecrets-0.4.398/badsecrets/examples/blacklist3r.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.4.394/badsecrets/examples/cli.py` & `badsecrets-0.4.398/badsecrets/examples/cli.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.4.394/badsecrets/examples/symfony_knownkey.py` & `badsecrets-0.4.398/badsecrets/examples/symfony_knownkey.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.4.394/badsecrets/examples/telerik_knownkey.py` & `badsecrets-0.4.398/badsecrets/examples/telerik_knownkey.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.4.394/badsecrets/helpers.py` & `badsecrets-0.4.398/badsecrets/helpers.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.4.394/badsecrets/modules/aspnet_viewstate.py` & `badsecrets-0.4.398/badsecrets/modules/aspnet_viewstate.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.4.394/badsecrets/modules/django_signedcookies.py` & `badsecrets-0.4.398/badsecrets/modules/django_signedcookies.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.4.394/badsecrets/modules/express_signedcookies_cs.py` & `badsecrets-0.4.398/badsecrets/modules/express_signedcookies_cs.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.4.394/badsecrets/modules/express_signedcookies_es.py` & `badsecrets-0.4.398/badsecrets/modules/express_signedcookies_es.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,23 +31,25 @@
             hmac.HMAC(secret.encode(), payload.encode(), hash_algorithm).digest()
         )
 
     def expressVerify_es(self, value, secret):
         payload, signature = value.split(".")[0][4:], urllib.parse.unquote(value.split(".")[1])
 
         with suppress(binascii.Error):
-            for hash_algorithm_str in self.search_dict(
-                self.hash_sizes, len(no_padding_urlsafe_base64_decode(signature))
-            ):
-                hash_algorithm = self.hash_algs[hash_algorithm_str]
-                generated_hash = self.expressHMAC(payload, secret, hash_algorithm)
-                if generated_hash == signature:
-                    return {
-                        "hash algorithm": hash_algorithm.__name__.split("openssl_")[1],
-                    }
+            signature_candidates = self.search_dict(self.hash_sizes, len(no_padding_urlsafe_base64_decode(signature)))
+            if not signature_candidates:
+                return False
+            else:
+                for hash_algorithm_str in signature_candidates:
+                    hash_algorithm = self.hash_algs[hash_algorithm_str]
+                    generated_hash = self.expressHMAC(payload, secret, hash_algorithm)
+                    if generated_hash == signature:
+                        return {
+                            "hash algorithm": hash_algorithm.__name__.split("openssl_")[1],
+                        }
         return False
 
     def check_secret(self, express_signed_cookie):
         if not self.identify(express_signed_cookie):
             return False
 
         for l in set(list(self.load_resources(["express_session_secrets.txt", "top_10000_passwords.txt"]))):
```

### Comparing `badsecrets-0.4.394/badsecrets/modules/flask_signedcookies.py` & `badsecrets-0.4.398/badsecrets/modules/flask_signedcookies.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.4.394/badsecrets/modules/generic_jwt.py` & `badsecrets-0.4.398/badsecrets/modules/generic_jwt.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.4.394/badsecrets/modules/jsf_viewstate.py` & `badsecrets-0.4.398/badsecrets/modules/jsf_viewstate.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.4.394/badsecrets/modules/laravel_signedcookies.py` & `badsecrets-0.4.398/badsecrets/modules/laravel_signedcookies.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.4.394/badsecrets/modules/peoplesoft_pstoken.py` & `badsecrets-0.4.398/badsecrets/modules/peoplesoft_pstoken.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.4.394/badsecrets/modules/rails_secretkeybase.py` & `badsecrets-0.4.398/badsecrets/modules/rails_secretkeybase.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.4.394/badsecrets/modules/symfony_signedurl.py` & `badsecrets-0.4.398/badsecrets/modules/symfony_signedurl.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.4.394/badsecrets/modules/telerik_encryptionkey.py` & `badsecrets-0.4.398/badsecrets/modules/telerik_encryptionkey.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.4.394/badsecrets/modules/telerik_hashkey.py` & `badsecrets-0.4.398/badsecrets/modules/telerik_hashkey.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.4.394/badsecrets/resources/aspnet_machinekeys.txt` & `badsecrets-0.4.398/badsecrets/resources/aspnet_machinekeys.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.4.394/badsecrets/resources/django_secret_keys.txt` & `badsecrets-0.4.398/badsecrets/resources/django_secret_keys.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.4.394/badsecrets/resources/express_session_secrets.txt` & `badsecrets-0.4.398/badsecrets/resources/express_session_secrets.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.4.394/badsecrets/resources/flask_secret_keys.txt` & `badsecrets-0.4.398/badsecrets/resources/flask_secret_keys.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.4.394/badsecrets/resources/jsf_viewstate_passwords_b64.txt` & `badsecrets-0.4.398/badsecrets/resources/jsf_viewstate_passwords_b64.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.4.394/badsecrets/resources/jwt_rsakeys_private.txt` & `badsecrets-0.4.398/badsecrets/resources/jwt_rsakeys_private.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.4.394/badsecrets/resources/jwt_rsakeys_public.txt` & `badsecrets-0.4.398/badsecrets/resources/jwt_rsakeys_public.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.4.394/badsecrets/resources/jwt_secrets.txt` & `badsecrets-0.4.398/badsecrets/resources/jwt_secrets.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.4.394/badsecrets/resources/laravel_app_keys.txt` & `badsecrets-0.4.398/badsecrets/resources/laravel_app_keys.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.4.394/badsecrets/resources/rails_secret_key_base.txt` & `badsecrets-0.4.398/badsecrets/resources/rails_secret_key_base.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.4.394/badsecrets/resources/symfony_appsecret.txt` & `badsecrets-0.4.398/badsecrets/resources/symfony_appsecret.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.4.394/badsecrets/resources/telerik_encryption_keys.txt` & `badsecrets-0.4.398/badsecrets/resources/telerik_encryption_keys.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.4.394/badsecrets/resources/telerik_hash_keys.txt` & `badsecrets-0.4.398/badsecrets/resources/telerik_hash_keys.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.4.394/badsecrets/resources/top_10000_passwords.txt` & `badsecrets-0.4.398/badsecrets/resources/top_10000_passwords.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.4.394/pyproject.toml` & `badsecrets-0.4.398/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "badsecrets"
-version = "v0.4.394"
+version = "v0.4.398"
 description = "About"
 authors = ["A library for detecting known or weak secrets on across many platforms"]
 license = "GPL-3.0"
 readme = "README.md"
 
 [tool.poetry.dev-dependencies]
 requests-mock = "^1.10.0"
```

### Comparing `badsecrets-0.4.394/PKG-INFO` & `badsecrets-0.4.398/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: badsecrets
-Version: 0.4.394
+Version: 0.4.398
 Summary: About
 License: GPL-3.0
 Author: A library for detecting known or weak secrets on across many platforms
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

