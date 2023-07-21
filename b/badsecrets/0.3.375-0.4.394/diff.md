# Comparing `tmp/badsecrets-0.3.375.tar.gz` & `tmp/badsecrets-0.4.394.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "badsecrets-0.3.375.tar", max compression
+gzip compressed data, was "badsecrets-0.4.394.tar", max compression
```

## Comparing `badsecrets-0.3.375.tar` & `badsecrets-0.4.394.tar`

### file list

```diff
@@ -1,42 +1,43 @@
--rw-r--r--   0        0        0    35149 2023-07-14 15:15:16.938012 badsecrets-0.3.375/LICENSE
--rw-r--r--   0        0        0    31950 2023-07-14 15:15:16.938012 badsecrets-0.3.375/README.md
--rw-r--r--   0        0        0      711 2023-07-14 15:15:16.938012 badsecrets-0.3.375/badsecrets/__init__.py
--rw-r--r--   0        0        0     6986 2023-07-14 15:15:16.938012 badsecrets-0.3.375/badsecrets/base.py
--rw-r--r--   0        0        0      233 2023-07-14 15:15:16.938012 badsecrets-0.3.375/badsecrets/errors.py
--rw-r--r--   0        0        0        0 2023-07-14 15:15:16.938012 badsecrets-0.3.375/badsecrets/examples/__init__.py
--rwxr-xr-x   0        0        0     4210 2023-07-14 15:15:16.938012 badsecrets-0.3.375/badsecrets/examples/blacklist3r.py
--rwxr-xr-x   0        0        0     7875 2023-07-14 15:15:16.938012 badsecrets-0.3.375/badsecrets/examples/cli.py
--rwxr-xr-x   0        0        0     3544 2023-07-14 15:15:16.938012 badsecrets-0.3.375/badsecrets/examples/symfony_knownkey.py
--rwxr-xr-x   0        0        0    10597 2023-07-14 15:15:16.938012 badsecrets-0.3.375/badsecrets/examples/telerik_knownkey.py
--rw-r--r--   0        0        0     5076 2023-07-14 15:15:16.938012 badsecrets-0.3.375/badsecrets/helpers.py
--rw-r--r--   0        0        0        0 2023-07-14 15:15:16.938012 badsecrets-0.3.375/badsecrets/modules/__init__.py
--rw-r--r--   0        0        0    10204 2023-07-14 15:15:16.938012 badsecrets-0.3.375/badsecrets/modules/aspnet_viewstate.py
--rw-r--r--   0        0        0      986 2023-07-14 15:15:16.938012 badsecrets-0.3.375/badsecrets/modules/django_signedcookies.py
--rw-r--r--   0        0        0     2022 2023-07-14 15:15:16.938012 badsecrets-0.3.375/badsecrets/modules/express_signedcookies.py
--rw-r--r--   0        0        0     1057 2023-07-14 15:15:16.938012 badsecrets-0.3.375/badsecrets/modules/flask_signedcookies.py
--rw-r--r--   0        0        0     4057 2023-07-14 15:15:16.938012 badsecrets-0.3.375/badsecrets/modules/generic_jwt.py
--rw-r--r--   0        0        0    14819 2023-07-14 15:15:16.938012 badsecrets-0.3.375/badsecrets/modules/jsf_viewstate.py
--rw-r--r--   0        0        0     2172 2023-07-14 15:15:16.938012 badsecrets-0.3.375/badsecrets/modules/laravel_signedcookies.py
--rw-r--r--   0        0        0     1931 2023-07-14 15:15:16.938012 badsecrets-0.3.375/badsecrets/modules/peoplesoft_pstoken.py
--rw-r--r--   0        0        0     3077 2023-07-14 15:15:16.938012 badsecrets-0.3.375/badsecrets/modules/rails_secretkeybase.py
--rw-r--r--   0        0        0     2932 2023-07-14 15:15:16.938012 badsecrets-0.3.375/badsecrets/modules/symfony_signedurl.py
--rw-r--r--   0        0        0     4949 2023-07-14 15:15:16.938012 badsecrets-0.3.375/badsecrets/modules/telerik_encryptionkey.py
--rw-r--r--   0        0        0     3718 2023-07-14 15:15:16.942012 badsecrets-0.3.375/badsecrets/modules/telerik_hashkey.py
--rw-r--r--   0        0        0   654096 2023-07-14 15:15:16.946012 badsecrets-0.3.375/badsecrets/resources/aspnet_machinekeys.txt
--rw-r--r--   0        0        0    31178 2023-07-14 15:15:16.946012 badsecrets-0.3.375/badsecrets/resources/django_secret_keys.txt
--rw-r--r--   0        0        0    40993 2023-07-14 15:15:16.946012 badsecrets-0.3.375/badsecrets/resources/express_session_secrets.txt
--rw-r--r--   0        0        0  1777603 2023-07-14 15:15:16.962013 badsecrets-0.3.375/badsecrets/resources/flask_secret_keys.txt
--rw-r--r--   0        0        0       87 2023-07-14 15:15:16.962013 badsecrets-0.3.375/badsecrets/resources/jsf_viewstate_passwords.txt
--rw-r--r--   0        0        0     1257 2023-07-14 15:15:16.962013 badsecrets-0.3.375/badsecrets/resources/jsf_viewstate_passwords_b64.txt
--rw-r--r--   0        0        0     7785 2023-07-14 15:15:16.962013 badsecrets-0.3.375/badsecrets/resources/jwt_rsakeys_private.txt
--rw-r--r--   0        0        0     2122 2023-07-14 15:15:16.962013 badsecrets-0.3.375/badsecrets/resources/jwt_rsakeys_public.txt
--rw-r--r--   0        0        0   113170 2023-07-14 15:15:16.966013 badsecrets-0.3.375/badsecrets/resources/jwt_secrets.txt
--rw-r--r--   0        0        0    45086 2023-07-14 15:15:16.966013 badsecrets-0.3.375/badsecrets/resources/laravel_app_keys.txt
--rw-r--r--   0        0        0       78 2023-07-14 15:15:16.966013 badsecrets-0.3.375/badsecrets/resources/peoplesoft_passwords.txt
--rw-r--r--   0        0        0     6184 2023-07-14 15:15:16.966013 badsecrets-0.3.375/badsecrets/resources/rails_secret_key_base.txt
--rw-r--r--   0        0        0     3009 2023-07-14 15:15:16.966013 badsecrets-0.3.375/badsecrets/resources/symfony_appsecret.txt
--rw-r--r--   0        0        0    18037 2023-07-14 15:15:16.966013 badsecrets-0.3.375/badsecrets/resources/telerik_encryption_keys.txt
--rw-r--r--   0        0        0    17990 2023-07-14 15:15:16.966013 badsecrets-0.3.375/badsecrets/resources/telerik_hash_keys.txt
--rw-r--r--   0        0        0    76516 2023-07-14 15:15:16.966013 badsecrets-0.3.375/badsecrets/resources/top_10000_passwords.txt
--rw-r--r--   0        0        0      957 2023-07-14 15:15:39.318575 badsecrets-0.3.375/pyproject.toml
--rw-r--r--   0        0        0    32804 1970-01-01 00:00:00.000000 badsecrets-0.3.375/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-21 03:20:42.242225 badsecrets-0.4.394/LICENSE
+-rw-r--r--   0        0        0    32418 2023-07-21 03:20:42.242225 badsecrets-0.4.394/README.md
+-rw-r--r--   0        0        0      711 2023-07-21 03:20:42.242225 badsecrets-0.4.394/badsecrets/__init__.py
+-rw-r--r--   0        0        0     7763 2023-07-21 03:20:42.242225 badsecrets-0.4.394/badsecrets/base.py
+-rw-r--r--   0        0        0      233 2023-07-21 03:20:42.242225 badsecrets-0.4.394/badsecrets/errors.py
+-rw-r--r--   0        0        0        0 2023-07-21 03:20:42.242225 badsecrets-0.4.394/badsecrets/examples/__init__.py
+-rwxr-xr-x   0        0        0     4210 2023-07-21 03:20:42.242225 badsecrets-0.4.394/badsecrets/examples/blacklist3r.py
+-rwxr-xr-x   0        0        0     7939 2023-07-21 03:20:42.242225 badsecrets-0.4.394/badsecrets/examples/cli.py
+-rwxr-xr-x   0        0        0     3544 2023-07-21 03:20:42.242225 badsecrets-0.4.394/badsecrets/examples/symfony_knownkey.py
+-rwxr-xr-x   0        0        0    10597 2023-07-21 03:20:42.246225 badsecrets-0.4.394/badsecrets/examples/telerik_knownkey.py
+-rw-r--r--   0        0        0     5076 2023-07-21 03:20:42.246225 badsecrets-0.4.394/badsecrets/helpers.py
+-rw-r--r--   0        0        0        0 2023-07-21 03:20:42.246225 badsecrets-0.4.394/badsecrets/modules/__init__.py
+-rw-r--r--   0        0        0    10468 2023-07-21 03:20:42.246225 badsecrets-0.4.394/badsecrets/modules/aspnet_viewstate.py
+-rw-r--r--   0        0        0     1006 2023-07-21 03:20:42.246225 badsecrets-0.4.394/badsecrets/modules/django_signedcookies.py
+-rw-r--r--   0        0        0     2867 2023-07-21 03:20:42.246225 badsecrets-0.4.394/badsecrets/modules/express_signedcookies_cs.py
+-rw-r--r--   0        0        0     2145 2023-07-21 03:20:42.246225 badsecrets-0.4.394/badsecrets/modules/express_signedcookies_es.py
+-rw-r--r--   0        0        0     1120 2023-07-21 03:20:42.246225 badsecrets-0.4.394/badsecrets/modules/flask_signedcookies.py
+-rw-r--r--   0        0        0     4087 2023-07-21 03:20:42.246225 badsecrets-0.4.394/badsecrets/modules/generic_jwt.py
+-rw-r--r--   0        0        0    14881 2023-07-21 03:20:42.246225 badsecrets-0.4.394/badsecrets/modules/jsf_viewstate.py
+-rw-r--r--   0        0        0     2192 2023-07-21 03:20:42.246225 badsecrets-0.4.394/badsecrets/modules/laravel_signedcookies.py
+-rw-r--r--   0        0        0     1958 2023-07-21 03:20:42.246225 badsecrets-0.4.394/badsecrets/modules/peoplesoft_pstoken.py
+-rw-r--r--   0        0        0     3097 2023-07-21 03:20:42.246225 badsecrets-0.4.394/badsecrets/modules/rails_secretkeybase.py
+-rw-r--r--   0        0        0     2963 2023-07-21 03:20:42.246225 badsecrets-0.4.394/badsecrets/modules/symfony_signedurl.py
+-rw-r--r--   0        0        0     5002 2023-07-21 03:20:42.246225 badsecrets-0.4.394/badsecrets/modules/telerik_encryptionkey.py
+-rw-r--r--   0        0        0     3776 2023-07-21 03:20:42.246225 badsecrets-0.4.394/badsecrets/modules/telerik_hashkey.py
+-rw-r--r--   0        0        0   654096 2023-07-21 03:20:42.250225 badsecrets-0.4.394/badsecrets/resources/aspnet_machinekeys.txt
+-rw-r--r--   0        0        0    31178 2023-07-21 03:20:42.250225 badsecrets-0.4.394/badsecrets/resources/django_secret_keys.txt
+-rw-r--r--   0        0        0    40993 2023-07-21 03:20:42.250225 badsecrets-0.4.394/badsecrets/resources/express_session_secrets.txt
+-rw-r--r--   0        0        0  1777603 2023-07-21 03:20:42.270227 badsecrets-0.4.394/badsecrets/resources/flask_secret_keys.txt
+-rw-r--r--   0        0        0       87 2023-07-21 03:20:42.270227 badsecrets-0.4.394/badsecrets/resources/jsf_viewstate_passwords.txt
+-rw-r--r--   0        0        0     1257 2023-07-21 03:20:42.270227 badsecrets-0.4.394/badsecrets/resources/jsf_viewstate_passwords_b64.txt
+-rw-r--r--   0        0        0     7785 2023-07-21 03:20:42.270227 badsecrets-0.4.394/badsecrets/resources/jwt_rsakeys_private.txt
+-rw-r--r--   0        0        0     2122 2023-07-21 03:20:42.270227 badsecrets-0.4.394/badsecrets/resources/jwt_rsakeys_public.txt
+-rw-r--r--   0        0        0   113170 2023-07-21 03:20:42.270227 badsecrets-0.4.394/badsecrets/resources/jwt_secrets.txt
+-rw-r--r--   0        0        0    45086 2023-07-21 03:20:42.270227 badsecrets-0.4.394/badsecrets/resources/laravel_app_keys.txt
+-rw-r--r--   0        0        0       78 2023-07-21 03:20:42.270227 badsecrets-0.4.394/badsecrets/resources/peoplesoft_passwords.txt
+-rw-r--r--   0        0        0     6184 2023-07-21 03:20:42.270227 badsecrets-0.4.394/badsecrets/resources/rails_secret_key_base.txt
+-rw-r--r--   0        0        0     3009 2023-07-21 03:20:42.270227 badsecrets-0.4.394/badsecrets/resources/symfony_appsecret.txt
+-rw-r--r--   0        0        0    18037 2023-07-21 03:20:42.270227 badsecrets-0.4.394/badsecrets/resources/telerik_encryption_keys.txt
+-rw-r--r--   0        0        0    17990 2023-07-21 03:20:42.270227 badsecrets-0.4.394/badsecrets/resources/telerik_hash_keys.txt
+-rw-r--r--   0        0        0    76516 2023-07-21 03:20:42.274227 badsecrets-0.4.394/badsecrets/resources/top_10000_passwords.txt
+-rw-r--r--   0        0        0      957 2023-07-21 03:21:08.551783 badsecrets-0.4.394/pyproject.toml
+-rw-r--r--   0        0        0    33272 1970-01-01 00:00:00.000000 badsecrets-0.4.394/PKG-INFO
```

### Comparing `badsecrets-0.3.375/LICENSE` & `badsecrets-0.4.394/LICENSE`

 * *Files identical despite different names*

### Comparing `badsecrets-0.3.375/README.md` & `badsecrets-0.4.394/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -27,15 +27,16 @@
 | Flask_SignedCookies  | Checks for weak Flask cookie signing password. Wrapper for [flask-unsign](https://github.com/Paradoxis/Flask-Unsign) |
 | Peoplesoft_PSToken  | Can check a peoplesoft PS_TOKEN for a bad/weak signing password |
 | Django_SignedCookies   | Checks django's session cookies (when in signed_cookie mode) for known django secret_key |
 | Rails_SecretKeyBase   | Checks Ruby on Rails signed or encrypted session cookies (from multiple major releases) for known secret_key_base |
 | Generic_JWT | Checks JWTs for known HMAC secrets or RSA private keys |
 | Jsf_viewstate | Checks Both Mojarra and Myfaces implimentations of Java Server Faces (JSF) for use of known or weak secret keys | 
 | Symfony_SignedURL | Checks symfony "_fragment" urls for known HMAC key. Operates on Full URL, including hash |
-| Express_SignedCookies | Checks express.js signed cookies and session cookies for known 'session secret' |
+| Express_SignedCookies_ES | Checks express.js express-session middleware for signed cookies and session cookies for known 'session secret' |
+| Express_SignedCookies_CS | Checks express.js cookie-session middleware for signed cookies and session cookies for known secret |
 | Laravel_SignedCookies | Checks 'laravel_session' cookies for known laravel 'APP_KEY' |
 
 ## Installation
 
 We have a [pypi](https://pypi.org/project/badsecrets/) package, so you can just do `pip install badsecrets` to make use of the library.
 
 ## Simple Usage
@@ -257,15 +258,16 @@
 Peoplesoft_PSToken = modules_loaded["peoplesoft_pstoken"]
 Telerik_HashKey = modules_loaded["telerik_hashkey"]
 Telerik_EncryptionKey = modules_loaded["telerik_encryptionkey"]
 Rails_SecretKeyBase = modules_loaded["rails_secretkeybase"]
 Generic_JWT = modules_loaded["generic_jwt"]
 Jsf_viewstate = modules_loaded["jsf_viewstate"]
 Symfony_SignedURL = modules_loaded["symfony_signedurl"]
-Express_SignedCookies = modules_loaded["express_signedcookies"]
+Express_SignedCookies_ES = modules_loaded["express_signedcookies_es"]
+Express_SignedCookies_CS = modules_loaded["express_signedcookies_cs"]
 Laravel_SignedCookies = modules_loaded["laravel_signedcookies"]
 
 x = ASPNET_Viewstate()
 print(f"###{str(x.__class__.__name__)}###")
 r = x.check_secret("AgF5WuyVO11CsYJ1K5rjyuLXqUGCITSOapG1cYNiriYQ6VTKochMpn8ws4eJRvft81nQIA==","EDD8C9AE")
 if r:
     print(r)
@@ -343,22 +345,30 @@
 r = x.check_secret("https://localhost/_fragment?_path=_controller%3Dsystem%26command%3Did%26return_value%3Dnull&_hash=Xnsvx/yLVQaimEd1CfepgH0rEXr422JnRSn/uaCE3gs=")
 if r:
     print(r)
 else:
     print("KEY NOT FOUND :(")
 
 
-x = Express_SignedCookies()
+x = Express_SignedCookies_ES()
 print(f"###{str(x.__class__.__name__)}###")
 r = x.check_secret("s%3A8FnPwdeM9kdGTZlWvdaVtQ0S1BCOhY5G.qys7H2oGSLLdRsEq7sqh7btOohHsaRKqyjV4LiVnBvc")
 if r:
     print(r)
 else:
     print("KEY NOT FOUND :(")
 
+x = Express_SignedCookies_CS()
+print(f"###{str(x.__class__.__name__)}###")
+r = x.check_secret("foo=eyJ1c2VybmFtZSI6IkJib3RJc0xpZmUifQ==","zOQU7v7aTe_3zu7tnVuHi1MJ2DU")
+if r:
+    print(r)
+else:
+    print("KEY NOT FOUND :(")
+
 
 x = Laravel_SignedCookies()
 print(f"###{str(x.__class__.__name__)}###")
 r = x.check_secret("eyJpdiI6IlhlNTZ2UjZUQWZKVHdIcG9nZFkwcGc9PSIsInZhbHVlIjoiRlUvY2grU1F1b01lSXdveXJ0T3N1WGJqeVVmZlNRQjNVOWxiSzljL1Z3RDhqYUdDbjZxMU9oSThWRzExT0YvUmthVzVKRE9kL0RvTEw1cFRhQkphOGw4S2loV1ZrMkkwTHd4am9sZkJQd2VCZ3R0VlFSeFo3ay9wTlBMb3lLSG8iLCJtYWMiOiJkMmU3M2ExNDc2NTc5YjAwMGMwMTdkYTQ1NThkMjRkNTY2YTE4OTg2MzY5MzE5NGZmOTM4YWVjOGZmMWU4NTk2IiwidGFnIjoiIn0%3D")
 if r:
     print(r)
 else:
```

### Comparing `badsecrets-0.3.375/badsecrets/__init__.py` & `badsecrets-0.4.394/badsecrets/__init__.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.3.375/badsecrets/base.py` & `badsecrets-0.4.394/badsecrets/base.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 generic_base64_regex = re.compile(
     r"^(?:[A-Za-z0-9+\/]{4}){8,}(?:[A-Za-z0-9+\/]{4}|[A-Za-z0-9+\/]{3}=|[A-Za-z0-9+\/]{2}={2})$"
 )
 
 
 class BadsecretsBase:
     identify_regex = re.compile(r".+")
-    description = {"product": "Undefined", "secret": "Undefined"}
+    description = {"product": "Undefined", "secret": "Undefined", "severity": "Undefined"}
 
     hash_sizes = {"SHA1": 20, "MD5": 16, "SHA256": 32, "SHA384": 48, "SHA512": 64}
     hash_algs = {
         "SHA1": hashlib.sha1,
         "MD5": hashlib.md5,
         "SHA256": hashlib.sha256,
         "SHA384": hashlib.sha384,
@@ -40,14 +40,17 @@
     def check_secret(self, secret):
         raise NotImplementedError
 
     @classmethod
     def get_description(self):
         return self.description
 
+    def get_product_from_carve(self, regex_search):
+        return regex_search.groups()[0]
+
     def get_hashcat_commands(self, s):
         return None
 
     def load_resources(self, resource_list):
         filepaths = []
         if self.custom_resource:
             filepaths.append(self.custom_resource)
@@ -94,26 +97,34 @@
                     r["type"] = "SecretFound"
                     r["product"] = v
                     r["location"] = "cookies"
                     results.append(r)
 
         if headers:
             for header_value in headers.values():
+                # Check if we have a match outright
                 r = self.check_secret(header_value)
                 if r:
                     r["type"] = "SecretFound"
                     r["product"] = header_value
                     r["location"] = "headers"
                     results.append(r)
+                # If we dont, we will only be able to add context if we have a match with carve_regex()
                 elif self.carve_regex():
                     s = re.search(self.carve_regex(), header_value)
                     if s:
-                        r = {"type": "IdentifyOnly"}
-                        r["hashcat"] = self.get_hashcat_commands(s.groups()[0])
-                        r["product"] = s.groups()[0]
+                        r = self.carve_to_check_secret(s)
+                        if r:
+                            r["type"] = "SecretFound"
+                        # the carve regex hit but no secret was found
+                        else:
+                            r = {"type": "IdentifyOnly"}
+                            r["hashcat"] = self.get_hashcat_commands(s)
+                        if "product" not in r.keys():
+                            r["product"] = self.get_product_from_carve(s)
                         r["location"] = "headers"
                         results.append(r)
 
         if body:
             if type(body) != str:
                 raise badsecrets.errors.CarveException("Body argument must be type str")
             if self.carve_regex():
@@ -121,15 +132,16 @@
                 if s:
                     r = self.carve_to_check_secret(s, url=kwargs.get("url", None))
                     if r:
                         r["type"] = "SecretFound"
                     else:
                         r = {"type": "IdentifyOnly"}
                         r["hashcat"] = self.get_hashcat_commands(s.groups()[0])
-                    r["product"] = s.groups()[0]
+                    if "product" not in r.keys():
+                        r["product"] = self.get_product_from_carve(s)
                     r["location"] = "body"
                     results.append(r)
 
         for r in results:
             r["description"] = self.get_description()
 
         # Don't report an IdentifyOnly result if we have a SecretFound result for the same 'product'
@@ -170,15 +182,18 @@
 def check_all_modules(*args, **kwargs):
     for m in BadsecretsBase.__subclasses__():
         x = m(custom_resource=kwargs.get("custom_resource", None))
         r = x.check_secret(*args[0 : x.check_secret_args])
         if r:
             r["detecting_module"] = m.__name__
             r["description"] = x.get_description()
-            r["product"] = args[0]
+
+            # allow the module to provide an amended product, if needed
+            if "product" not in r.keys():
+                r["product"] = args[0]
             r["location"] = "manual"
             return r
     return None
 
 
 def carve_all_modules(**kwargs):
     results = []
```

### Comparing `badsecrets-0.3.375/badsecrets/examples/blacklist3r.py` & `badsecrets-0.4.394/badsecrets/examples/blacklist3r.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.3.375/badsecrets/examples/cli.py` & `badsecrets-0.4.394/badsecrets/examples/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,14 +49,15 @@
 
     def print_report(self, report_message):
         print(report_message)
         print(f"Detecting Module: {self.x['detecting_module']}\n")
         print(f"Product Type: {self.x['description']['product']}")
         print(f"Product: {self.x['product']}")
         print(f"Secret Type: {self.x['description']['secret']}")
+        print(f"Severity: {self.x['description']['severity']}")
         print(f"Location: {self.x['location']}")
 
 
 class ReportSecret(BaseReport):
     def report(self):
         self.print_report(print_status("Known Secret Found!\n", color=Fore.GREEN, passthru=True))
         print_status(f"Secret: {self.x['secret']}", color=Fore.GREEN)
```

### Comparing `badsecrets-0.3.375/badsecrets/examples/symfony_knownkey.py` & `badsecrets-0.4.394/badsecrets/examples/symfony_knownkey.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.3.375/badsecrets/examples/telerik_knownkey.py` & `badsecrets-0.4.394/badsecrets/examples/telerik_knownkey.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.3.375/badsecrets/helpers.py` & `badsecrets-0.4.394/badsecrets/helpers.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.3.375/badsecrets/modules/aspnet_viewstate.py` & `badsecrets-0.4.394/badsecrets/modules/aspnet_viewstate.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from viewstate.exceptions import ViewStateException
 from badsecrets.base import BadsecretsBase, generic_base64_regex
 
 
 class ASPNET_Viewstate(BadsecretsBase):
     check_secret_args = 3
     identify_regex = generic_base64_regex
-    description = {"product": "ASP.NET Viewstate", "secret": "ASP.NET MachineKey"}
+    description = {"product": "ASP.NET Viewstate", "secret": "ASP.NET MachineKey", "severity": "CRITICAL"}
 
     def carve_regex(self):
         return re.compile(
             r"<input.+__VIEWSTATE\"\svalue=\"(.+)\"[\S\s]+<input.+__VIEWSTATEGENERATOR\"\svalue=\"(\w+)\""
         )
 
     def carve_to_check_secret(self, s, url=None):
@@ -191,15 +191,19 @@
                                 )
                                 if decryptionAlgo:
                                     confirmed_ekey = ekey
 
                         result = f"validationKey: {vkey} validationAlgo: {validationAlgo}"
                         if confirmed_ekey:
                             result += f" encryptionKey: {confirmed_ekey} encryptionAlgo: {decryptionAlgo}"
-                        return {"secret": result, "details": f"Mode [{mode}]"}
+
+                        product_string = f"Viewstate: {viewstate_B64}"
+                        if generator != "0000":
+                            product_string += f" Generator: {generator[::-1].hex().upper()}"
+                        return {"secret": result, "product": product_string, "details": f"Mode [{mode}]"}
         return None
 
 
 # Based on https://github.com/pwntester/ysoserial.net/blob/master/ysoserial/Plugins/ViewStatePlugin.cs and translated to python. All credit to ysoserial.net.
 class Simulate_dotnet45_kdf_context_parameters:
     def __init__(self, url):
         self.url = url
```

### Comparing `badsecrets-0.3.375/badsecrets/modules/django_signedcookies.py` & `badsecrets-0.4.394/badsecrets/modules/django_signedcookies.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import re
 from django.core.signing import loads as djangoLoads, BadSignature
 from badsecrets.base import BadsecretsBase
 
 
 class DjangoSignedCookies(BadsecretsBase):
     identify_regex = re.compile(r"^[\.a-zA-z-0-9]+:[\.a-zA-z-0-9:]+$")
-    description = {"product": "Djangno Signed Cookie", "secret": "Django secret_key"}
+    description = {"product": "Djangno Signed Cookie", "secret": "Django secret_key", "severity": "HIGH"}
 
     def check_secret(self, django_signed_cookie):
         if not self.identify(django_signed_cookie):
             return False
         for l in set(list(self.load_resources(["django_secret_keys.txt", "top_10000_passwords.txt"]))):
             secret_key = l.rstrip()
             try:
```

### Comparing `badsecrets-0.3.375/badsecrets/modules/express_signedcookies.py` & `badsecrets-0.4.394/badsecrets/modules/express_signedcookies_es.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,29 +7,35 @@
 from badsecrets.base import BadsecretsBase
 
 
 def no_padding_urlsafe_base64_decode(enc):
     return base64.urlsafe_b64decode(enc + "=" * (-len(enc) % 4))
 
 
-def no_padding_urlsafe_base64_encode(enc):
+def no_padding_urlsafe_base64_encode_es(enc):
     return base64.urlsafe_b64encode(enc).decode().rstrip("=").replace("-", "+").replace("_", "/")
 
 
-class ExpressSignedCookies(BadsecretsBase):
+class ExpressSignedCookies_ES(BadsecretsBase):
     identify_regex = re.compile(r"^s%3[Aa][^\.]+\.[a-zA-Z0-9%]{20,90}$")
-    description = {"product": "Express.js Signed Cookie", "secret": "Express.js SESSION_SECRET"}
+    description = {
+        "product": "Express.js Signed Cookie (express-session)",
+        "secret": "Express.js SESSION_SECRET (express-session)",
+        "severity": "LOW",
+    }
 
     def carve_regex(self):
         return re.compile(r"(s%3[Aa][^\.]+\.[a-zA-Z0-9%]{20,90})")
 
     def expressHMAC(self, payload, secret, hash_algorithm):
-        return no_padding_urlsafe_base64_encode(hmac.HMAC(secret.encode(), payload.encode(), hash_algorithm).digest())
+        return no_padding_urlsafe_base64_encode_es(
+            hmac.HMAC(secret.encode(), payload.encode(), hash_algorithm).digest()
+        )
 
-    def expressVerify(self, value, secret):
+    def expressVerify_es(self, value, secret):
         payload, signature = value.split(".")[0][4:], urllib.parse.unquote(value.split(".")[1])
 
         with suppress(binascii.Error):
             for hash_algorithm_str in self.search_dict(
                 self.hash_sizes, len(no_padding_urlsafe_base64_decode(signature))
             ):
                 hash_algorithm = self.hash_algs[hash_algorithm_str]
@@ -43,11 +49,11 @@
     def check_secret(self, express_signed_cookie):
         if not self.identify(express_signed_cookie):
             return False
 
         for l in set(list(self.load_resources(["express_session_secrets.txt", "top_10000_passwords.txt"]))):
             session_secret = l.rstrip()
 
-            r = self.expressVerify(express_signed_cookie, session_secret)
+            r = self.expressVerify_es(express_signed_cookie, session_secret)
 
             if r:
                 return {"secret": session_secret, "details": r}
```

### Comparing `badsecrets-0.3.375/badsecrets/modules/flask_signedcookies.py` & `badsecrets-0.4.394/badsecrets/modules/flask_signedcookies.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,26 +3,27 @@
 import re
 from flask_unsign import verify as flaskVerify
 from badsecrets.base import BadsecretsBase
 
 
 class Flask_SignedCookies(BadsecretsBase):
     identify_regex = re.compile(r"eyJ(?:[\w-]*\.)(?:[\w-]*\.)[\w-]*")
-    description = {"product": "Flask Signed Cookie", "secret": "Flask Password"}
+    description = {"product": "Flask Signed Cookie", "secret": "Flask Password", "severity": "HIGH"}
 
     def check_secret(self, flask_cookie):
         if not self.identify(flask_cookie):
             return None
         for l in set(list(self.load_resources(["flask_secret_keys.txt", "top_10000_passwords.txt"]))):
             password = l.rstrip()
             r = flaskVerify(value=flask_cookie, secret=password)
             if r:
                 return {"secret": password, "details": r}
         return None
 
-    def get_hashcat_commands(self, flask_cookie):
+    def get_hashcat_commands(self, flask_cookie, *args):
         return [
             {
                 "command": f"hashcat -m 29100 -a 0 {flask_cookie} <dictionary_file>",
                 "description": f"Flask Signed Cookie",
+                "severity": "HIGH",
             }
         ]
```

### Comparing `badsecrets-0.3.375/badsecrets/modules/generic_jwt.py` & `badsecrets-0.4.394/badsecrets/modules/generic_jwt.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     "http://www.w3.org/2007/05/xmldsig-more#sha384-rsa-MGF1": "PS384",
     "http://www.w3.org/2007/05/xmldsig-more#sha512-rsa-MGF1": "PS512",
 }
 
 
 class Generic_JWT(BadsecretsBase):
     identify_regex = re.compile(r"eyJ(?:[\w-]*\.)(?:[\w-]*\.)[\w-]*")
-    description = {"product": "JSON Web Token (JWT)", "secret": "HMAC/RSA Key"}
+    description = {"product": "JSON Web Token (JWT)", "secret": "HMAC/RSA Key", "severity": "HIGH"}
 
     @staticmethod
     def swap_algorithm(jwt, algorithm):
         header = j.get_unverified_header(jwt)
         header["alg"] = algorithm
         header_encoded = (
             base64.urlsafe_b64encode(json.dumps(header, separators=(",", ":")).encode()).rstrip(b"=").decode()
@@ -62,15 +62,15 @@
 
         if algorithm in XMLDSIG_table.keys():
             algorithm = XMLDSIG_table[algorithm]
             JWT = self.swap_algorithm(JWT, algorithm)
 
         return jwt_headers, algorithm, JWT
 
-    def get_hashcat_commands(self, JWT):
+    def get_hashcat_commands(self, JWT, *args):
         jwt_headers, algorithm, JWT = self.jwtLoad(JWT)
         if jwt_headers and algorithm and JWT:
             if algorithm[0].lower() != "h":
                 return None
 
             return [
                 {
@@ -90,20 +90,19 @@
         if algorithm[0].lower() == "h":
             for l in self.load_resources(["jwt_secrets.txt"]):
                 key = l.strip()
 
                 r = self.jwtVerify(JWT, key, algorithm)
                 if r:
                     r["jwt_headers"] = jwt_headers
-
                     return {"secret": key, "details": r}
 
         elif algorithm[0].lower() == "r":
             for l in self.load_resources(["jwt_rsakeys_public.txt"]):
                 private_key_name = l.split(":")[0]
                 public_key = f"{l.split(':')[1]}".rstrip().encode().replace(b"\\n", b"\n")
                 r = self.jwtVerify(JWT, public_key, algorithm)
-                r["jwt_headers"] = jwt_headers
                 if r:
+                    r["jwt_headers"] = jwt_headers
                     return {"secret": f"Private key Name: {private_key_name}", "details": r}
 
         return None
```

### Comparing `badsecrets-0.3.375/badsecrets/modules/jsf_viewstate.py` & `badsecrets-0.4.394/badsecrets/modules/jsf_viewstate.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,19 @@
 
 class Jsf_viewstate(BadsecretsBase):
     myfaces_candidate_decryption_algorithms = [DES3, AES, DES]
 
     identify_regex = re.compile(
         r"^(?:[%A-Za-z0-9+\/]{4}){8,}(?:[%A-Za-z0-9+\/]{4}|[%A-Za-z0-9+\/]{3}=|[%A-Za-z0-9+\/]{2}={2})$"
     )
-    description = {"product": "Java Server Faces Viewstate", "secret": "com.sun.faces.ClientStateSavingPassword"}
+    description = {
+        "product": "Java Server Faces Viewstate",
+        "secret": "com.sun.faces.ClientStateSavingPassword",
+        "severity": "CRITICAL",
+    }
 
     hashcat_hashalg_table = {"MD5": "50", "SHA1": "150", "SHA256": "1450", "SHA384": "10800", "SHA512": "1750"}
 
     @staticmethod
     def attempt_decompress(value):
         try:
             uncompressed = gzip.decompress(base64.b64decode(value))
@@ -174,15 +178,15 @@
 
         # The decryption key was valid, but the first block was not - this indicates that the mode is CBC and the IV is incorrect
         if invalid_iv_match:
             return invalid_iv_match
         else:
             return (None, None, None, None, None)
 
-    def get_hashcat_commands(self, jsf_viewstate_value):
+    def get_hashcat_commands(self, jsf_viewstate_value, *args):
         commands = []
         decoded_viewstate = base64.b64decode(urllib.parse.unquote(jsf_viewstate_value))
         sig = decoded_viewstate[:32]
         data = decoded_viewstate[32:]
 
         candidate_hash_algs = list(self.hash_sizes.keys())
         for hash_alg in candidate_hash_algs:
```

### Comparing `badsecrets-0.3.375/badsecrets/modules/laravel_signedcookies.py` & `badsecrets-0.4.394/badsecrets/modules/laravel_signedcookies.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         if mac == hmac.new(raw_secret, iv + value, hashlib.sha256).hexdigest():
             aes_crypt = AES.new(key=raw_secret, mode=AES.MODE_CBC, IV=base64.b64decode(iv))
             decrypted = unpad(aes_crypt.decrypt(base64.b64decode(value)))
             return decrypted
         return None
 
     identify_regex = re.compile(r"eyJ(?:[\w-])*")
-    description = {"product": "Laravel Signed Cookie", "secret": "Laravel APP_KEY"}
+    description = {"product": "Laravel Signed Cookie", "secret": "Laravel APP_KEY", "severity": "HIGH"}
 
     def laravelVerify(self, value, secret):
         # attempt to decode laravel cookie and load contents into JSON object
         try:
             json_value = json.loads(base64.b64decode(urllib.parse.unquote(value)))
 
             if not all(key in json_value.keys() for key in ["mac", "value", "iv"]):
```

### Comparing `badsecrets-0.3.375/badsecrets/modules/peoplesoft_pstoken.py` & `badsecrets-0.4.394/badsecrets/modules/peoplesoft_pstoken.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import base64
 import hashlib
 from badsecrets.base import BadsecretsBase, generic_base64_regex
 
 
 class Peoplesoft_PSToken(BadsecretsBase):
     identify_regex = generic_base64_regex
-    description = {"product": "Peoplesoft PS_TOKEN", "secret": "Peoplesoft Secret"}
+    description = {"product": "Peoplesoft PS_TOKEN", "secret": "Peoplesoft Secret", "severity": "HIGH"}
 
     def peoplesoft_load(self, PS_TOKEN_B64):
         PS_TOKEN = base64.b64decode(PS_TOKEN_B64)
         SHA1_mac = PS_TOKEN[44:64]
         try:
             PS_TOKEN_DATA = zlib.decompress(PS_TOKEN[76:])
         except zlib.error:
@@ -37,15 +37,15 @@
 
             h = hashlib.sha1(PS_TOKEN_DATA + password.encode("utf_16_le", errors="ignore"))
             if h.digest() == SHA1_mac:
                 return {"secret": f"Username: {username} Password: {password}", "details": None}
 
         return None
 
-    def get_hashcat_commands(self, PS_TOKEN_B64):
+    def get_hashcat_commands(self, PS_TOKEN_B64, *args):
         PS_TOKEN_DATA, SHA1_mac = self.peoplesoft_load(PS_TOKEN_B64)
 
         if not PS_TOKEN_DATA or not SHA1_mac:
             return None
         return [
             {
                 "command": f"hashcat -m 13500 -a 0 {SHA1_mac.hex()}:{PS_TOKEN_DATA.hex()}  <dictionary_file>",
```

### Comparing `badsecrets-0.3.375/badsecrets/modules/rails_secretkeybase.py` & `badsecrets-0.4.394/badsecrets/modules/rails_secretkeybase.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from Crypto.Util.Padding import unpad
 from Crypto.Protocol.KDF import PBKDF2
 from badsecrets.base import BadsecretsBase
 
 
 class Rails_SecretKeyBase(BadsecretsBase):
     identify_regex = re.compile(r"^[\.a-zA-z-0-9\%=]{32,}--[\.a-zA-z-0-9%=]{16,}$")
-    description = {"product": "Rails Signed Cookie", "secret": "Rails secret_key_base"}
+    description = {"product": "Rails Signed Cookie", "secret": "Rails secret_key_base", "severity": "HIGH"}
 
     def rails(self, rails_cookie, secret_key_base):
         split_rails_cookie = urllib.parse.unquote(rails_cookie).split("--")
         data = split_rails_cookie[0]
 
         # Cookie is likely signed but not encrypted
         if split_rails_cookie[0].startswith("eyJ"):
```

### Comparing `badsecrets-0.3.375/badsecrets/modules/symfony_signedurl.py` & `badsecrets-0.4.394/badsecrets/modules/symfony_signedurl.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from badsecrets.base import BadsecretsBase
 
 # Special thanks to Ambionics Security for their blog post: https://www.ambionics.io/blog/symfony-secret-fragment
 
 
 class Symfony_SignedURL(BadsecretsBase):
     identify_regex = re.compile(r"http(?:s)?:\/\/[^\/]+\/_fragment[^\s]+_hash=[\/a-zA-z-0-9\+=%]{24,132}")
-    description = {"product": "Symfony Signed URL", "secret": "Symfony APP_SECRET"}
+    description = {"product": "Symfony Signed URL", "secret": "Symfony APP_SECRET", "severity": "CRITICAL"}
 
     def carve_regex(self):
         return re.compile(r"(http(?:s)?:\/\/[^\/]+\/_fragment[^\s]+_hash=[\/a-zA-z-0-9\+=%]{24,132})")
 
     def symfonyHMAC(self, url, secret, hash_algorithm):
         return base64.b64encode(hmac.HMAC(secret.encode(), url.encode(), hash_algorithm).digest())
 
@@ -39,15 +39,15 @@
 
     def symfonyLoad(self, value):
         url, url_hash = value.split("&_hash=")
         for hash_algorithm_str in self.search_dict(self.hash_sizes, len(base64.b64decode(url_hash))):
             hash_algorithm = self.hash_algs[hash_algorithm_str]
         return url, url_hash, hash_algorithm
 
-    def get_hashcat_commands(self, signed_url):
+    def get_hashcat_commands(self, signed_url, *args):
         url, url_hash, hash_algorithm = self.symfonyLoad(signed_url)
         hash_algorithm_str = hash_algorithm.__name__.split("_")[1]
         hashcat_mode = None
 
         if hash_algorithm_str == "sha1":
             hashcat_mode = "150"
```

### Comparing `badsecrets-0.3.375/badsecrets/modules/telerik_encryptionkey.py` & `badsecrets-0.4.394/badsecrets/modules/telerik_encryptionkey.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,19 @@
 from badsecrets.errors import Telerik_EncryptionKey_Exception
 
 telerik_hardcoded_salt = [58, 84, 91, 25, 10, 34, 29, 68, 60, 88, 44, 51, 1]
 
 
 class Telerik_EncryptionKey(BadsecretsBase):
     identify_regex = re.compile(r"^(?:[A-Za-z0-9+\/=%]{32,})$")
-    description = {"product": "Telerik DialogParameters", "secret": "Telerik.Web.UI.DialogParametersEncryptionKey"}
+    description = {
+        "product": "Telerik DialogParameters",
+        "secret": "Telerik.Web.UI.DialogParametersEncryptionKey",
+        "severity": "MEDIUM",
+    }
 
     def carve_regex(self):
         return re.compile(r"{\"SerializedParameters\":\"([^\"]*)\"")
 
     def prepare_keylist(self, include_machinekeys=False):
         if include_machinekeys:
             for l in self.load_resources(["aspnet_machinekeys.txt"]):
```

### Comparing `badsecrets-0.3.375/badsecrets/modules/telerik_hashkey.py` & `badsecrets-0.4.394/badsecrets/modules/telerik_hashkey.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,19 @@
 import urllib.parse
 from contextlib import suppress
 from badsecrets.base import BadsecretsBase
 
 
 class Telerik_HashKey(BadsecretsBase):
     identify_regex = re.compile(r"^(?:[A-Za-z0-9+\/=%]{32,})$")
-    description = {"product": "Telerik DialogParameters", "secret": "Telerik.Upload.ConfigurationHashKey"}
+    description = {
+        "product": "Telerik DialogParameters",
+        "secret": "Telerik.Upload.ConfigurationHashKey",
+        "severity": "HIGH",
+    }
 
     def carve_regex(self):
         return re.compile(r"{\"SerializedParameters\":\"([^\"]*)\"")
 
     def prepare_keylist(self, include_machinekeys=True):
         if include_machinekeys:
             for l in self.load_resources(["aspnet_machinekeys.txt"]):
@@ -40,15 +44,15 @@
         for vkey in self.prepare_keylist():
             with suppress(binascii.Error):
                 h = hmac.new(vkey.encode(), dp_enc, self.hash_algs["SHA256"])
                 if base64.b64encode(h.digest()) == dp_hash:
                     return {"secret": vkey, "details": None}
         return None
 
-    def get_hashcat_commands(self, dialogParameters_raw):
+    def get_hashcat_commands(self, dialogParameters_raw, *args):
         dp_enc, dp_hash = self.telerik_hashkey_load(dialogParameters_raw)
         if not dp_enc or not dp_hash:
             return None
 
         try:
             dp_enc_decoded = base64.b64decode(dp_hash)
             dp_hash_decoded = base64.b64decode(dp_enc)
```

### Comparing `badsecrets-0.3.375/badsecrets/resources/aspnet_machinekeys.txt` & `badsecrets-0.4.394/badsecrets/resources/aspnet_machinekeys.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.3.375/badsecrets/resources/django_secret_keys.txt` & `badsecrets-0.4.394/badsecrets/resources/django_secret_keys.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.3.375/badsecrets/resources/express_session_secrets.txt` & `badsecrets-0.4.394/badsecrets/resources/express_session_secrets.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.3.375/badsecrets/resources/flask_secret_keys.txt` & `badsecrets-0.4.394/badsecrets/resources/flask_secret_keys.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.3.375/badsecrets/resources/jsf_viewstate_passwords_b64.txt` & `badsecrets-0.4.394/badsecrets/resources/jsf_viewstate_passwords_b64.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.3.375/badsecrets/resources/jwt_rsakeys_private.txt` & `badsecrets-0.4.394/badsecrets/resources/jwt_rsakeys_private.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.3.375/badsecrets/resources/jwt_rsakeys_public.txt` & `badsecrets-0.4.394/badsecrets/resources/jwt_rsakeys_public.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.3.375/badsecrets/resources/jwt_secrets.txt` & `badsecrets-0.4.394/badsecrets/resources/jwt_secrets.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.3.375/badsecrets/resources/laravel_app_keys.txt` & `badsecrets-0.4.394/badsecrets/resources/laravel_app_keys.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.3.375/badsecrets/resources/rails_secret_key_base.txt` & `badsecrets-0.4.394/badsecrets/resources/rails_secret_key_base.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.3.375/badsecrets/resources/symfony_appsecret.txt` & `badsecrets-0.4.394/badsecrets/resources/symfony_appsecret.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.3.375/badsecrets/resources/telerik_encryption_keys.txt` & `badsecrets-0.4.394/badsecrets/resources/telerik_encryption_keys.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.3.375/badsecrets/resources/telerik_hash_keys.txt` & `badsecrets-0.4.394/badsecrets/resources/telerik_hash_keys.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.3.375/badsecrets/resources/top_10000_passwords.txt` & `badsecrets-0.4.394/badsecrets/resources/top_10000_passwords.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.3.375/pyproject.toml` & `badsecrets-0.4.394/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "badsecrets"
-version = "v0.3.375"
+version = "v0.4.394"
 description = "About"
 authors = ["A library for detecting known or weak secrets on across many platforms"]
 license = "GPL-3.0"
 readme = "README.md"
 
 [tool.poetry.dev-dependencies]
 requests-mock = "^1.10.0"
@@ -33,8 +33,8 @@
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry-dynamic-versioning]
 enable = false
 metadata = true
-format = 'v0.3.{distance}'
+format = 'v0.4.{distance}'
```

### Comparing `badsecrets-0.3.375/PKG-INFO` & `badsecrets-0.4.394/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: badsecrets
-Version: 0.3.375
+Version: 0.4.394
 Summary: About
 License: GPL-3.0
 Author: A library for detecting known or weak secrets on across many platforms
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -49,15 +49,16 @@
 | Flask_SignedCookies  | Checks for weak Flask cookie signing password. Wrapper for [flask-unsign](https://github.com/Paradoxis/Flask-Unsign) |
 | Peoplesoft_PSToken  | Can check a peoplesoft PS_TOKEN for a bad/weak signing password |
 | Django_SignedCookies   | Checks django's session cookies (when in signed_cookie mode) for known django secret_key |
 | Rails_SecretKeyBase   | Checks Ruby on Rails signed or encrypted session cookies (from multiple major releases) for known secret_key_base |
 | Generic_JWT | Checks JWTs for known HMAC secrets or RSA private keys |
 | Jsf_viewstate | Checks Both Mojarra and Myfaces implimentations of Java Server Faces (JSF) for use of known or weak secret keys | 
 | Symfony_SignedURL | Checks symfony "_fragment" urls for known HMAC key. Operates on Full URL, including hash |
-| Express_SignedCookies | Checks express.js signed cookies and session cookies for known 'session secret' |
+| Express_SignedCookies_ES | Checks express.js express-session middleware for signed cookies and session cookies for known 'session secret' |
+| Express_SignedCookies_CS | Checks express.js cookie-session middleware for signed cookies and session cookies for known secret |
 | Laravel_SignedCookies | Checks 'laravel_session' cookies for known laravel 'APP_KEY' |
 
 ## Installation
 
 We have a [pypi](https://pypi.org/project/badsecrets/) package, so you can just do `pip install badsecrets` to make use of the library.
 
 ## Simple Usage
@@ -279,15 +280,16 @@
 Peoplesoft_PSToken = modules_loaded["peoplesoft_pstoken"]
 Telerik_HashKey = modules_loaded["telerik_hashkey"]
 Telerik_EncryptionKey = modules_loaded["telerik_encryptionkey"]
 Rails_SecretKeyBase = modules_loaded["rails_secretkeybase"]
 Generic_JWT = modules_loaded["generic_jwt"]
 Jsf_viewstate = modules_loaded["jsf_viewstate"]
 Symfony_SignedURL = modules_loaded["symfony_signedurl"]
-Express_SignedCookies = modules_loaded["express_signedcookies"]
+Express_SignedCookies_ES = modules_loaded["express_signedcookies_es"]
+Express_SignedCookies_CS = modules_loaded["express_signedcookies_cs"]
 Laravel_SignedCookies = modules_loaded["laravel_signedcookies"]
 
 x = ASPNET_Viewstate()
 print(f"###{str(x.__class__.__name__)}###")
 r = x.check_secret("AgF5WuyVO11CsYJ1K5rjyuLXqUGCITSOapG1cYNiriYQ6VTKochMpn8ws4eJRvft81nQIA==","EDD8C9AE")
 if r:
     print(r)
@@ -365,22 +367,30 @@
 r = x.check_secret("https://localhost/_fragment?_path=_controller%3Dsystem%26command%3Did%26return_value%3Dnull&_hash=Xnsvx/yLVQaimEd1CfepgH0rEXr422JnRSn/uaCE3gs=")
 if r:
     print(r)
 else:
     print("KEY NOT FOUND :(")
 
 
-x = Express_SignedCookies()
+x = Express_SignedCookies_ES()
 print(f"###{str(x.__class__.__name__)}###")
 r = x.check_secret("s%3A8FnPwdeM9kdGTZlWvdaVtQ0S1BCOhY5G.qys7H2oGSLLdRsEq7sqh7btOohHsaRKqyjV4LiVnBvc")
 if r:
     print(r)
 else:
     print("KEY NOT FOUND :(")
 
+x = Express_SignedCookies_CS()
+print(f"###{str(x.__class__.__name__)}###")
+r = x.check_secret("foo=eyJ1c2VybmFtZSI6IkJib3RJc0xpZmUifQ==","zOQU7v7aTe_3zu7tnVuHi1MJ2DU")
+if r:
+    print(r)
+else:
+    print("KEY NOT FOUND :(")
+
 
 x = Laravel_SignedCookies()
 print(f"###{str(x.__class__.__name__)}###")
 r = x.check_secret("eyJpdiI6IlhlNTZ2UjZUQWZKVHdIcG9nZFkwcGc9PSIsInZhbHVlIjoiRlUvY2grU1F1b01lSXdveXJ0T3N1WGJqeVVmZlNRQjNVOWxiSzljL1Z3RDhqYUdDbjZxMU9oSThWRzExT0YvUmthVzVKRE9kL0RvTEw1cFRhQkphOGw4S2loV1ZrMkkwTHd4am9sZkJQd2VCZ3R0VlFSeFo3ay9wTlBMb3lLSG8iLCJtYWMiOiJkMmU3M2ExNDc2NTc5YjAwMGMwMTdkYTQ1NThkMjRkNTY2YTE4OTg2MzY5MzE5NGZmOTM4YWVjOGZmMWU4NTk2IiwidGFnIjoiIn0%3D")
 if r:
     print(r)
 else:
```

