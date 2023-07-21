# Comparing `tmp/openid_whisperer-0.1.6.tar.gz` & `tmp/openid_whisperer-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openid_whisperer-0.1.6.tar", max compression
+gzip compressed data, was "openid_whisperer-0.1.7.tar", max compression
```

## Comparing `openid_whisperer-0.1.6.tar` & `openid_whisperer-0.1.7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1153 2023-06-25 20:59:05.837711 openid_whisperer-0.1.6/LICENSE
--rw-r--r--   0        0        0     6961 2023-07-13 23:19:52.650318 openid_whisperer-0.1.6/README.md
--rw-r--r--   0        0        0     2144 2023-07-20 21:04:06.890418 openid_whisperer-0.1.6/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-03 22:59:15.739113 openid_whisperer-0.1.6/src/openid_whisperer/__init__.py
--rw-r--r--   0        0        0       83 2023-06-03 22:59:15.739296 openid_whisperer-0.1.6/src/openid_whisperer/__main__.py
--rw-r--r--   0        0        0     8889 2023-07-19 16:17:02.507285 openid_whisperer-0.1.6/src/openid_whisperer/config.py
--rw-r--r--   0        0        0     2539 2023-07-13 16:49:06.224941 openid_whisperer-0.1.6/src/openid_whisperer/demo_certs/ca_cert.pem
--rw-r--r--   0        0        0     2681 2023-07-13 16:49:06.225650 openid_whisperer-0.1.6/src/openid_whisperer/demo_certs/cert.pem
--rw-r--r--   0        0        0     1675 2023-07-13 16:49:06.226302 openid_whisperer-0.1.6/src/openid_whisperer/demo_certs/key.pem
--rw-r--r--   0        0        0     1135 2023-07-20 14:49:18.489462 openid_whisperer-0.1.6/src/openid_whisperer/main.py
--rw-r--r--   0        0        0    22593 2023-07-20 20:58:33.784797 openid_whisperer-0.1.6/src/openid_whisperer/openid_blueprint.py
--rw-r--r--   0        0        0    32983 2023-07-20 20:12:41.163231 openid_whisperer-0.1.6/src/openid_whisperer/openid_interface.py
--rw-r--r--   0        0        0      910 2023-07-14 12:33:04.149317 openid_whisperer-0.1.6/src/openid_whisperer/openid_types.py
--rw-r--r--   0        0        0        0 2023-06-04 10:12:20.232971 openid_whisperer-0.1.6/src/openid_whisperer/py.typed
--rw-r--r--   0        0        0     7774 2023-07-04 18:12:57.431778 openid_whisperer-0.1.6/src/openid_whisperer/static/style.css
--rw-r--r--   0        0        0    29021 2023-07-19 16:34:51.108344 openid_whisperer-0.1.6/src/openid_whisperer/templates/authenticate.html
--rw-r--r--   0        0        0      451 2023-07-19 17:15:03.303758 openid_whisperer-0.1.6/src/openid_whisperer/templates/form_post_response.html
--rw-r--r--   0        0        0        0 2023-07-01 16:06:18.981399 openid_whisperer-0.1.6/src/openid_whisperer/utils/__init__.py
--rw-r--r--   0        0        0     5082 2023-07-14 12:36:54.560754 openid_whisperer-0.1.6/src/openid_whisperer/utils/cert_utils.py
--rw-r--r--   0        0        0     6840 2023-07-20 15:06:53.637647 openid_whisperer-0.1.6/src/openid_whisperer/utils/common.py
--rw-r--r--   0        0        0     6144 2023-07-14 12:22:20.152374 openid_whisperer-0.1.6/src/openid_whisperer/utils/config_utils.py
--rw-r--r--   0        0        0     4812 2023-07-14 14:21:24.986862 openid_whisperer-0.1.6/src/openid_whisperer/utils/credential_store.py
--rw-r--r--   0        0        0     3637 2023-07-20 14:49:18.532645 openid_whisperer-0.1.6/src/openid_whisperer/utils/test_utils.py
--rw-r--r--   0        0        0    19602 2023-07-20 16:34:57.398579 openid_whisperer-0.1.6/src/openid_whisperer/utils/token_store.py
--rw-r--r--   0        0        0     3188 2023-07-14 12:43:25.019940 openid_whisperer-0.1.6/src/openid_whisperer/utils/token_utils.py
--rw-r--r--   0        0        0    10641 2023-07-20 14:49:18.662763 openid_whisperer-0.1.6/src/openid_whisperer/utils/user_info_ext.py
--rw-r--r--   0        0        0     8047 1970-01-01 00:00:00.000000 openid_whisperer-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1153 2023-06-25 20:59:05.837711 openid_whisperer-0.1.7/LICENSE
+-rw-r--r--   0        0        0     6665 2023-07-21 19:06:13.430139 openid_whisperer-0.1.7/README.md
+-rw-r--r--   0        0        0     2144 2023-07-21 19:02:15.241990 openid_whisperer-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-03 22:59:15.739113 openid_whisperer-0.1.7/src/openid_whisperer/__init__.py
+-rw-r--r--   0        0        0       83 2023-06-03 22:59:15.739296 openid_whisperer-0.1.7/src/openid_whisperer/__main__.py
+-rw-r--r--   0        0        0     8889 2023-07-19 16:17:02.507285 openid_whisperer-0.1.7/src/openid_whisperer/config.py
+-rw-r--r--   0        0        0     2539 2023-07-13 16:49:06.224941 openid_whisperer-0.1.7/src/openid_whisperer/demo_certs/ca_cert.pem
+-rw-r--r--   0        0        0     2681 2023-07-13 16:49:06.225650 openid_whisperer-0.1.7/src/openid_whisperer/demo_certs/cert.pem
+-rw-r--r--   0        0        0     1675 2023-07-13 16:49:06.226302 openid_whisperer-0.1.7/src/openid_whisperer/demo_certs/key.pem
+-rw-r--r--   0        0        0     1135 2023-07-20 14:49:18.489462 openid_whisperer-0.1.7/src/openid_whisperer/main.py
+-rw-r--r--   0        0        0    22460 2023-07-21 15:38:16.110824 openid_whisperer-0.1.7/src/openid_whisperer/openid_blueprint.py
+-rw-r--r--   0        0        0    33492 2023-07-21 18:50:19.320462 openid_whisperer-0.1.7/src/openid_whisperer/openid_interface.py
+-rw-r--r--   0        0        0      910 2023-07-14 12:33:04.149317 openid_whisperer-0.1.7/src/openid_whisperer/openid_types.py
+-rw-r--r--   0        0        0        0 2023-06-04 10:12:20.232971 openid_whisperer-0.1.7/src/openid_whisperer/py.typed
+-rw-r--r--   0        0        0     7774 2023-07-04 18:12:57.431778 openid_whisperer-0.1.7/src/openid_whisperer/static/style.css
+-rw-r--r--   0        0        0    29021 2023-07-19 16:34:51.108344 openid_whisperer-0.1.7/src/openid_whisperer/templates/authenticate.html
+-rw-r--r--   0        0        0      451 2023-07-19 17:15:03.303758 openid_whisperer-0.1.7/src/openid_whisperer/templates/form_post_response.html
+-rw-r--r--   0        0        0        0 2023-07-01 16:06:18.981399 openid_whisperer-0.1.7/src/openid_whisperer/utils/__init__.py
+-rw-r--r--   0        0        0     5082 2023-07-14 12:36:54.560754 openid_whisperer-0.1.7/src/openid_whisperer/utils/cert_utils.py
+-rw-r--r--   0        0        0     6865 2023-07-21 12:59:14.882179 openid_whisperer-0.1.7/src/openid_whisperer/utils/common.py
+-rw-r--r--   0        0        0     6144 2023-07-14 12:22:20.152374 openid_whisperer-0.1.7/src/openid_whisperer/utils/config_utils.py
+-rw-r--r--   0        0        0     4812 2023-07-14 14:21:24.986862 openid_whisperer-0.1.7/src/openid_whisperer/utils/credential_store.py
+-rw-r--r--   0        0        0     3637 2023-07-20 14:49:18.532645 openid_whisperer-0.1.7/src/openid_whisperer/utils/test_utils.py
+-rw-r--r--   0        0        0    21923 2023-07-21 17:02:58.439662 openid_whisperer-0.1.7/src/openid_whisperer/utils/token_store.py
+-rw-r--r--   0        0        0     3188 2023-07-14 12:43:25.019940 openid_whisperer-0.1.7/src/openid_whisperer/utils/token_utils.py
+-rw-r--r--   0        0        0    10641 2023-07-20 14:49:18.662763 openid_whisperer-0.1.7/src/openid_whisperer/utils/user_info_ext.py
+-rw-r--r--   0        0        0     7751 1970-01-01 00:00:00.000000 openid_whisperer-0.1.7/PKG-INFO
```

### Comparing `openid_whisperer-0.1.6/LICENSE` & `openid_whisperer-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `openid_whisperer-0.1.6/README.md` & `openid_whisperer-0.1.7/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -64,30 +64,24 @@
 When the example code is run from the project_root folder, the configuration loads default environment
 variables from `.env_TEST`
 
 ### `example_src/msal_flows`
 The MSAL library is used as an alternative method for verifying OpenID protocol compliance, more
 specifically the complaince of ADFS or that of Azure.
 The following flow examples run through successfully:
+* `acquire_token_on_behalf_of_example.py`
+* `confidential_client_certificate_sample.py`
 * `device_code_flow.py`
 * `username_and_password_example.py`
 * `interactive_sample.py`
 * `migrate_rt.py` This example has API compatibility, however there is no functional implementation.
 
 To run these examples, you may have to alter the configuration parameters to suite you environment
 and by default an instance of Openid-Whisperer and OpenID Web/API protected service.
 
-## Microsoft Authentication Library MSAL
-MSAL is used for alternative testing kit to verify ADFS and Azure OpenID authentication flows. The
-following MSAL code examples run through successfully:
-* `device_code_flow.py`
-* `username_and_password_example.py`
-* `interactive_sample.py`
-* `migrate_rt.py` This example has API compatibility, however there is no functional implementation.
-
 ## Development
 Active development is on Python 3.11 on both Windows 10 and macOS 13.4. Testing is run using PyTest against these 
 environments as well as under Ubuntu 22.04 through GitHub Actions.
 
 ## Environment Setup
 1. Install Python, this project is developed with CPython ^3.11
 2. Upgrade pip
```

### Comparing `openid_whisperer-0.1.6/pyproject.toml` & `openid_whisperer-0.1.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openid-whisperer"
-version = "0.1.6"
+version = "0.1.7"
 description = "OpenID 1.0 Mock Identity Service"
 license = "MIT"
 authors = ["Robert Betts <betts_robert@yahoo.com>"]
 maintainers = ["Robert Betts <betts_robert@yahoo.com>"]
 readme = "README.md"
 homepage = "https://github.com/robertbetts/openid-whisperer"
 repository = "https://github.com/robertbetts/openid-whisperer"
```

### Comparing `openid_whisperer-0.1.6/src/openid_whisperer/config.py` & `openid_whisperer-0.1.7/src/openid_whisperer/config.py`

 * *Files identical despite different names*

### Comparing `openid_whisperer-0.1.6/src/openid_whisperer/demo_certs/ca_cert.pem` & `openid_whisperer-0.1.7/src/openid_whisperer/demo_certs/ca_cert.pem`

 * *Files identical despite different names*

### Comparing `openid_whisperer-0.1.6/src/openid_whisperer/demo_certs/cert.pem` & `openid_whisperer-0.1.7/src/openid_whisperer/demo_certs/cert.pem`

 * *Files identical despite different names*

### Comparing `openid_whisperer-0.1.6/src/openid_whisperer/demo_certs/key.pem` & `openid_whisperer-0.1.7/src/openid_whisperer/demo_certs/key.pem`

 * *Files identical despite different names*

### Comparing `openid_whisperer-0.1.6/src/openid_whisperer/main.py` & `openid_whisperer-0.1.7/src/openid_whisperer/main.py`

 * *Files identical despite different names*

### Comparing `openid_whisperer-0.1.6/src/openid_whisperer/openid_blueprint.py` & `openid_whisperer-0.1.7/src/openid_whisperer/openid_blueprint.py`

 * *Files 1% similar despite different names*

```diff
@@ -313,20 +313,17 @@
                 key=f"openid-whisperer-token-{client_id}",
                 value=auth_cookie_token,
                 secure=True,
                 httponly=True,
             )
         return authorize_get_resp
 
-    else:  # only other possible option is a response_type is "token" or "id_token":
-        if "error" in openid_response:
-            response = openid_response
-        else:
-            response = openid_response["access_token"]
-        return json.dumps(response), status_code
+    else:
+        # only other possible option is a response_type of "token" or "id_token":
+        return json.dumps(openid_response), status_code
 
 
 @openid_blueprint.route("/<tenant>/oauth2/token", methods=["POST"])  # type: ignore[misc]
 def token(tenant: str) -> ResponseReturnValue:
     """Returns a token response payload for the support grant_types"""
     grant_type: str = request.form.get("grant_type", "")
     device_code: str = request.form.get("device_code", "")
```

### Comparing `openid_whisperer-0.1.6/src/openid_whisperer/openid_interface.py` & `openid_whisperer-0.1.7/src/openid_whisperer/openid_interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -683,17 +683,30 @@
             if token_response is None:
                 raise OpenidApiInterfaceException(
                     "token_error",
                     "Token issued for end user devicecode flow, has been revoked.",
                 )
 
         elif grant_type == "refresh_token":
-            # TODO: Implement for grant_type, "on-behalf-of flow"
-            raise OpenidApiInterfaceException(
-                "bad_token_request", f"grant_type '{grant_type}' not implemented"
+            logging.debug("refresh_token  flow")
+
+            # TODO: if scope is blank default to "openid" and update scope with client_id and resource
+            user_claims = self.credential_store.get_user_scope_claims(
+                username=username, scope=scope
+            )
+            audience = get_audience(client_id=client_id, scope=scope, resource=resource)
+
+            _, token_response = self.token_store.create_new_token(
+                client_id=client_id,
+                issuer=self.issuer_reference,
+                sub=username,
+                user_claims=user_claims,
+                audience=audience,
+                nonce=nonce,
+                refresh_token=refresh_token
             )
 
         elif grant_type == "authorization_code":
             """Client application submits a parameter name code to reference a previously received authentication_code
             for a token that has been created and is ready for issue out of the token store.
             """
             # TODO: check redirect_uri validation is required
@@ -702,15 +715,15 @@
             token_response = self.token_store.token_requests.pop(code)
             if token_response is None:
                 raise OpenidApiInterfaceException(
                     "token_error",
                     "Token issued for end user devicecode flow, has been revoked.",
                 )
 
-        elif grant_type == "password":
+        elif grant_type in "password":
             """End user information is provided as part of the request to issue a new token. There is no existing
             authentication flow related to this request.
             """
 
             if not self.credential_store.authenticate(
                 tenant=tenant,
                 username=username,
```

### Comparing `openid_whisperer-0.1.6/src/openid_whisperer/openid_types.py` & `openid_whisperer-0.1.7/src/openid_whisperer/openid_types.py`

 * *Files identical despite different names*

### Comparing `openid_whisperer-0.1.6/src/openid_whisperer/static/style.css` & `openid_whisperer-0.1.7/src/openid_whisperer/static/style.css`

 * *Files identical despite different names*

### Comparing `openid_whisperer-0.1.6/src/openid_whisperer/templates/authenticate.html` & `openid_whisperer-0.1.7/src/openid_whisperer/templates/authenticate.html`

 * *Files identical despite different names*

### Comparing `openid_whisperer-0.1.6/src/openid_whisperer/utils/cert_utils.py` & `openid_whisperer-0.1.7/src/openid_whisperer/utils/cert_utils.py`

 * *Files identical despite different names*

### Comparing `openid_whisperer-0.1.6/src/openid_whisperer/utils/common.py` & `openid_whisperer-0.1.7/src/openid_whisperer/utils/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -203,14 +203,15 @@
     elif grant_type not in GRANT_TYPES_SUPPORTED:
         error_message = f"The grant_type of '{grant_type}' is not supported"
 
     if error_message is None and grant_type not in (
         "authorization_code",
         "password",
         "client_credentials",
+        "refresh_token",
         "device_code",  # associated with urn:ietf:params:oauth:grant-type:device_code
         "urn:ietf:params:oauth:grant-type:device_code",
         "jwt-bearer",  # associated with urn:ietf:params:oauth:grant-type:jwt-bearer
         "urn:ietf:params:oauth:grant-type:jwt-bearer",
     ):
         error_message = f"The grant_type of '{grant_type}' is not implemented"
```

### Comparing `openid_whisperer-0.1.6/src/openid_whisperer/utils/config_utils.py` & `openid_whisperer-0.1.7/src/openid_whisperer/utils/config_utils.py`

 * *Files identical despite different names*

### Comparing `openid_whisperer-0.1.6/src/openid_whisperer/utils/credential_store.py` & `openid_whisperer-0.1.7/src/openid_whisperer/utils/credential_store.py`

 * *Files identical despite different names*

### Comparing `openid_whisperer-0.1.6/src/openid_whisperer/utils/test_utils.py` & `openid_whisperer-0.1.7/src/openid_whisperer/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `openid_whisperer-0.1.6/src/openid_whisperer/utils/token_store.py` & `openid_whisperer-0.1.7/src/openid_whisperer/utils/token_store.py`

 * *Files 4% similar despite different names*

```diff
@@ -73,15 +73,15 @@
         """
         self.token_issuer_key_id: str | None = None
         self.ca_cert_filename: str = ""
         self.org_key_filename: str = ""
         self.org_key_password: str = ""
         self.org_cert_filename: str = ""
         self.token_expiry_seconds: int | None = 600
-        self.refresh_token_expiry_seconds: int | None = 3600
+        self.refresh_token_expiry_seconds: int | None = None
 
         # Update class properties from kwargs
         for key, value in kwargs.items():
             if not hasattr(self, key):
                 logger.warning(
                     "Invalid initialization parameter, ignoring. %s: %s",
                     key,
@@ -93,15 +93,15 @@
         # Check config and update with reasonable defaults
         if self.token_expiry_seconds is None or self.token_expiry_seconds <= 0:
             self.token_expiry_seconds = 600  # 10 minutes
         if (
             self.refresh_token_expiry_seconds is None
             or self.refresh_token_expiry_seconds <= 0
         ):
-            self.refresh_token_expiry_seconds = 3600  # 1 hour
+            self.refresh_token_expiry_seconds = 60*60*14   # 24 hours
 
         # This value is hardcoded to RS256 and should not be changed after class initialisation
         self.token_issuer_algorithm: str = "RS256"
 
         # ca certificates Indexed on certificate serial number
         self.ca_certificates: Dict[str, x509.Certificate] = {}
         # org certificate/private key pairs Indexed on certificate serial number
@@ -111,16 +111,16 @@
         self.token_issuer_key_id: str | None = None
 
         # TODO: Track these in the background, processing expiry, revocation etc.
         self.tokens_issued: Dict[
             str, Tuple[Any, str]
         ] = {}  # (expires_in, authorization_code) indexed by jti
         self.refresh_tokens_issued: Dict[
-            str, Tuple[int, str]
-        ] = {}  # (expires_in, authorization_code) indexed by jti
+            str, Dict[str, Any]
+        ] = {}  # dict{expires_in, client_id, jti} indexed by refresh_token
         self.token_requests: Dict[
             str, Dict[str, Any]
         ] = {}  # token_request Dict indexed by authorisation_code
 
         # Client secret keys, this is experimental, self.add_client_secret(client_id, algorithm, public_key)
         self.client_secret_keys: Dict[str, List[Dict[str, Any]]] = {}
 
@@ -415,78 +415,126 @@
             algorithms=[algorithm],
             issuer=issuer,
             audience=token_audience,
         )
         logger.debug(claims)
         return claims
 
+    def create_refresh_token(self, client_id: str, jti: str, expiry_seconds: Optional[int] = None) -> str:
+        """ Returns a refresh_token, its expiry is defaulted to 24 hours,
+        is stored locally, until a refresh is requested.
+        :param client_id:
+        :param jti:
+        :param expiry_seconds:
+        """
+        expiry_seconds = expiry_seconds if expiry_seconds else self.token_expiry_seconds
+        expires_in = datetime.datetime.utcnow() + datetime.timedelta(seconds=expiry_seconds)
+        refresh_token = uuid4().hex
+        self.refresh_tokens_issued[refresh_token] = {
+            "expires_in": expires_in,
+            "client": client_id,
+            "jti": jti,
+        }
+        return refresh_token
+
     def create_new_token(
         self,
         client_id,
         issuer: str,
         sub: str,
         user_claims: Dict[str, Any],
         audience: List[str],
         nonce: str,
+        refresh_token: Optional[str] = None,
     ) -> Tuple[str, Dict[str, Any]]:
-        """Returns a response that include JWT.
+        """Returns a response that includes an id_token and access_token JWTs.
 
         The claims iss, sun, exp, iat, auth_time, appid, ver are overriden by the TokenIssuerCertificateStore
 
         :param client_id:
         :param issuer:
         :param sub:
         :param user_claims:
         :param audience:
         :param nonce:
+        :param refresh_token:
         :return:
         """
+
         auth_time = datetime.datetime.utcnow()
-        expires_in = auth_time + datetime.timedelta(seconds=self.token_expiry_seconds)
-        payload = {}
-        payload.update(user_claims)
-        payload["nonce"] = nonce
+        expires_in = get_seconds_epoch(auth_time + datetime.timedelta(seconds=self.token_expiry_seconds))
+        auth_time_epoch = get_seconds_epoch(auth_time)
+        expires_in_epoch = expires_in
+        auth_time_str = auth_time.isoformat(sep=" ")
+        aud = audience
         jti = uuid4().hex
-        payload.update(
+
+        if refresh_token:
+            previous_refresh = self.refresh_tokens_issued.get(refresh_token)
+            if previous_refresh is None:
+                raise TokenIssuerCertificateStoreException("invalid_refresh_token", "refresh token request is invalid")
+            if previous_refresh["jti"] not in self.tokens_issued:
+                raise TokenIssuerCertificateStoreException("invalid_refresh_token", "refresh token request is invalid")
+            prev_expiry, prev_auth_code = self.tokens_issued[previous_refresh["jti"]]
+            if prev_auth_code not in self.token_requests:
+                raise TokenIssuerCertificateStoreException("invalid_refresh_token", "refresh token request is invalid")
+            previous_token = self.token_requests[prev_auth_code]["id_token"]
+            refresh_claims = jwt.decode(previous_token, options={"verify_signature": False})
+            sub = refresh_claims["sub"]
+            aud = refresh_claims["aud"]
+            auth_time_str = refresh_claims["auth_time"]
+            user_claims.update(refresh_claims)
+
+
+        # For now both the access_token and id_token have the same claims
+        access_token_payload = {}
+        access_token_payload.update(user_claims)
+        access_token_payload["nonce"] = nonce
+        access_token_payload.update(
             {
                 "iss": issuer,
                 "sub": sub,
-                "aud": audience,
-                "exp": get_seconds_epoch(expires_in),
-                "nbf": get_seconds_epoch(auth_time),
-                "iat": get_seconds_epoch(auth_time),
-                "auth_time": auth_time.isoformat(sep=" "),
+                "aud": aud,
+                "exp": expires_in_epoch,
+                "nbf": auth_time_epoch,
+                "iat": auth_time_epoch,
+                "auth_time": auth_time_str,
                 "appid": client_id,
                 "jti": jti,
                 "ver": "1.0",
             }
         )
         headers = {
             "typ": "JWT",
             "alg": self.token_issuer_algorithm,
             "kid": self.token_issuer_key_id,
             "x5t": self.token_issuer_key_id,
         }
-        token = jwt.encode(
-            payload=payload,
+        access_token = jwt.encode(
+            payload=access_token_payload,
+            key=self.token_issuer_private_key,
+            algorithm=self.token_issuer_algorithm,
+            headers=headers,
+        )
+        id_token_payload = {}
+        id_token_payload.update(access_token_payload)
+        id_token = jwt.encode(
+            payload=id_token_payload,
             key=self.token_issuer_private_key,
             algorithm=self.token_issuer_algorithm,
             headers=headers,
         )
-        # TODO: Check conditions when to complete and return a refresh token
-        refresh_token = ""
-        refresh_token_expires_in = get_seconds_epoch(auth_time)
-        # TODO: Check when required to have both access_token and id_token in the return below
+        refresh_token = self.create_refresh_token(client_id, jti)
+        # TODO: Check when not required to have both access_token and id_token in the response
         token_response = {
-            "access_token": token,
-            "id_token": token,
+            "access_token": access_token,
+            "id_token": id_token,
             "token_type": "Bearer",
-            "expires_in": get_seconds_epoch(expires_in),
+            "expires_in": expires_in_epoch,
             "refresh_token": refresh_token,
-            "refresh_token_expires_in": refresh_token_expires_in,
         }
         authorisation_code = generate_s256_hash(json.dumps(token_response))
         self.tokens_issued[jti] = (expires_in, authorisation_code)
         self.token_requests[authorisation_code] = token_response
         return authorisation_code, token_response
 
     def decode_token(
```

### Comparing `openid_whisperer-0.1.6/src/openid_whisperer/utils/token_utils.py` & `openid_whisperer-0.1.7/src/openid_whisperer/utils/token_utils.py`

 * *Files identical despite different names*

### Comparing `openid_whisperer-0.1.6/src/openid_whisperer/utils/user_info_ext.py` & `openid_whisperer-0.1.7/src/openid_whisperer/utils/user_info_ext.py`

 * *Files identical despite different names*

### Comparing `openid_whisperer-0.1.6/PKG-INFO` & `openid_whisperer-0.1.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openid-whisperer
-Version: 0.1.6
+Version: 0.1.7
 Summary: OpenID 1.0 Mock Identity Service
 Home-page: https://github.com/robertbetts/openid-whisperer
 License: MIT
 Keywords: python,mock,api,oauth2,openid
 Author: Robert Betts
 Author-email: betts_robert@yahoo.com
 Maintainer: Robert Betts
@@ -92,30 +92,24 @@
 When the example code is run from the project_root folder, the configuration loads default environment
 variables from `.env_TEST`
 
 ### `example_src/msal_flows`
 The MSAL library is used as an alternative method for verifying OpenID protocol compliance, more
 specifically the complaince of ADFS or that of Azure.
 The following flow examples run through successfully:
+* `acquire_token_on_behalf_of_example.py`
+* `confidential_client_certificate_sample.py`
 * `device_code_flow.py`
 * `username_and_password_example.py`
 * `interactive_sample.py`
 * `migrate_rt.py` This example has API compatibility, however there is no functional implementation.
 
 To run these examples, you may have to alter the configuration parameters to suite you environment
 and by default an instance of Openid-Whisperer and OpenID Web/API protected service.
 
-## Microsoft Authentication Library MSAL
-MSAL is used for alternative testing kit to verify ADFS and Azure OpenID authentication flows. The
-following MSAL code examples run through successfully:
-* `device_code_flow.py`
-* `username_and_password_example.py`
-* `interactive_sample.py`
-* `migrate_rt.py` This example has API compatibility, however there is no functional implementation.
-
 ## Development
 Active development is on Python 3.11 on both Windows 10 and macOS 13.4. Testing is run using PyTest against these 
 environments as well as under Ubuntu 22.04 through GitHub Actions.
 
 ## Environment Setup
 1. Install Python, this project is developed with CPython ^3.11
 2. Upgrade pip
```

