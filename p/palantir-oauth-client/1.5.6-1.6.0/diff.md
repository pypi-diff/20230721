# Comparing `tmp/palantir-oauth-client-1.5.6.tar.gz` & `tmp/palantir-oauth-client-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "palantir-oauth-client-1.5.6.tar", max compression
+gzip compressed data, was "palantir-oauth-client-1.6.0.tar", max compression
```

## Comparing `palantir-oauth-client-1.5.6.tar` & `palantir-oauth-client-1.6.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0    11357 2023-05-26 07:27:48.327569 palantir-oauth-client-1.5.6/LICENSE
--rw-r--r--   0        0        0     3585 2023-05-26 07:27:48.327569 palantir-oauth-client-1.5.6/README.md
--rw-r--r--   0        0        0      928 2023-05-26 07:27:48.327569 palantir-oauth-client-1.5.6/palantir_oauth_client/__init__.py
--rw-r--r--   0        0        0     3585 2023-05-26 07:27:48.327569 palantir-oauth-client-1.5.6/palantir_oauth_client/_client.py
--rw-r--r--   0        0        0     8217 2023-05-26 07:27:48.327569 palantir-oauth-client-1.5.6/palantir_oauth_client/_flow.py
--rw-r--r--   0        0        0     2179 2023-05-26 07:27:48.327569 palantir-oauth-client-1.5.6/palantir_oauth_client/_utils.py
--rw-r--r--   0        0        0       22 2023-05-26 07:27:48.483569 palantir-oauth-client-1.5.6/palantir_oauth_client/_version.py
--rw-r--r--   0        0        0     1512 2023-05-26 07:27:48.327569 palantir-oauth-client-1.5.6/palantir_oauth_client/_webserver.py
--rw-r--r--   0        0        0    10661 2023-05-26 07:27:48.327569 palantir-oauth-client-1.5.6/palantir_oauth_client/auth.py
--rw-r--r--   0        0        0     6354 2023-05-26 07:27:48.327569 palantir-oauth-client-1.5.6/palantir_oauth_client/cache.py
--rw-r--r--   0        0        0     7211 2023-05-26 07:27:48.327569 palantir-oauth-client-1.5.6/palantir_oauth_client/credentials.py
--rw-r--r--   0        0        0     1095 2023-05-26 07:27:48.327569 palantir-oauth-client-1.5.6/palantir_oauth_client/errors.py
--rw-r--r--   0        0        0      754 2023-05-26 07:27:48.931567 palantir-oauth-client-1.5.6/pyproject.toml
--rw-r--r--   0        0        0     4416 2023-05-26 07:27:49.916967 palantir-oauth-client-1.5.6/setup.py
--rw-r--r--   0        0        0     4297 2023-05-26 07:27:49.917483 palantir-oauth-client-1.5.6/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-21 11:46:40.847109 palantir-oauth-client-1.6.0/LICENSE
+-rw-r--r--   0        0        0     3585 2023-07-21 11:46:40.847109 palantir-oauth-client-1.6.0/README.md
+-rw-r--r--   0        0        0      928 2023-07-21 11:46:40.847109 palantir-oauth-client-1.6.0/palantir_oauth_client/__init__.py
+-rw-r--r--   0        0        0     3585 2023-07-21 11:46:40.847109 palantir-oauth-client-1.6.0/palantir_oauth_client/_client.py
+-rw-r--r--   0        0        0     8217 2023-07-21 11:46:40.847109 palantir-oauth-client-1.6.0/palantir_oauth_client/_flow.py
+-rw-r--r--   0        0        0     2192 2023-07-21 11:46:40.847109 palantir-oauth-client-1.6.0/palantir_oauth_client/_utils.py
+-rw-r--r--   0        0        0       22 2023-07-21 11:46:41.051109 palantir-oauth-client-1.6.0/palantir_oauth_client/_version.py
+-rw-r--r--   0        0        0     1512 2023-07-21 11:46:40.847109 palantir-oauth-client-1.6.0/palantir_oauth_client/_webserver.py
+-rw-r--r--   0        0        0    10661 2023-07-21 11:46:40.847109 palantir-oauth-client-1.6.0/palantir_oauth_client/auth.py
+-rw-r--r--   0        0        0     6354 2023-07-21 11:46:40.847109 palantir-oauth-client-1.6.0/palantir_oauth_client/cache.py
+-rw-r--r--   0        0        0     7093 2023-07-21 11:46:40.847109 palantir-oauth-client-1.6.0/palantir_oauth_client/credentials.py
+-rw-r--r--   0        0        0     1095 2023-07-21 11:46:40.847109 palantir-oauth-client-1.6.0/palantir_oauth_client/errors.py
+-rw-r--r--   0        0        0      754 2023-07-21 11:46:41.599112 palantir-oauth-client-1.6.0/pyproject.toml
+-rw-r--r--   0        0        0     4416 2023-07-21 11:46:42.634622 palantir-oauth-client-1.6.0/setup.py
+-rw-r--r--   0        0        0     4297 2023-07-21 11:46:42.635012 palantir-oauth-client-1.6.0/PKG-INFO
```

### Comparing `palantir-oauth-client-1.5.6/LICENSE` & `palantir-oauth-client-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `palantir-oauth-client-1.5.6/README.md` & `palantir-oauth-client-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `palantir-oauth-client-1.5.6/palantir_oauth_client/__init__.py` & `palantir-oauth-client-1.6.0/palantir_oauth_client/__init__.py`

 * *Files identical despite different names*

### Comparing `palantir-oauth-client-1.5.6/palantir_oauth_client/_client.py` & `palantir-oauth-client-1.6.0/palantir_oauth_client/_client.py`

 * *Files identical despite different names*

### Comparing `palantir-oauth-client-1.5.6/palantir_oauth_client/_flow.py` & `palantir-oauth-client-1.6.0/palantir_oauth_client/_flow.py`

 * *Files identical despite different names*

### Comparing `palantir-oauth-client-1.5.6/palantir_oauth_client/_utils.py` & `palantir-oauth-client-1.6.0/palantir_oauth_client/_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,19 +9,20 @@
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 import calendar
 import requests_oauthlib
-from datetime import datetime, timedelta
+from datetime import datetime, timedelta, timezone
 from typing import Any, Mapping, Sequence, Tuple
 from urllib3.util import parse_url
 from urllib.parse import urlparse, parse_qs
 
+
 CLOCK_SKEW_SECONDS = 10
 CLOCK_SKEW = timedelta(seconds=CLOCK_SKEW_SECONDS)
 
 _REQUIRED_CONFIG_KEYS = frozenset(("auth_uri", "token_uri", "client_id"))
 
 
 def get_hostname(url: str) -> str:
@@ -30,15 +31,15 @@
     if _url.port is not None:
         hostname = hostname + ":" + str(_url.port)
     return hostname
 
 
 def utcnow() -> datetime:
     """Returns the current UTC datetime."""
-    return datetime.utcnow()
+    return datetime.now(tz=timezone.utc)
 
 
 def datetime_to_secs(value: datetime) -> int:
     """Convert a datetime object to the number of seconds since the UNIX epoch."""
     return calendar.timegm(value.utctimetuple())
 
 
@@ -51,16 +52,13 @@
     session = requests_oauthlib.OAuth2Session(
         client_id=client_config["client_id"], scope=scopes, **kwargs
     )
 
     return session, client_config
 
 
-def is_state_valid(
-    stored_state,
-    url
-) -> (bool, str):
+def is_state_valid(stored_state, url) -> (bool, str):
     parsed_url = urlparse(url)
     url_query = parse_qs(parsed_url.query)
     received_state = url_query.get("state", None)
 
     return received_state and stored_state == received_state[0]
```

### Comparing `palantir-oauth-client-1.5.6/palantir_oauth_client/_webserver.py` & `palantir-oauth-client-1.6.0/palantir_oauth_client/_webserver.py`

 * *Files identical despite different names*

### Comparing `palantir-oauth-client-1.5.6/palantir_oauth_client/auth.py` & `palantir-oauth-client-1.6.0/palantir_oauth_client/auth.py`

 * *Files identical despite different names*

### Comparing `palantir-oauth-client-1.5.6/palantir_oauth_client/cache.py` & `palantir-oauth-client-1.6.0/palantir_oauth_client/cache.py`

 * *Files identical despite different names*

### Comparing `palantir-oauth-client-1.5.6/palantir_oauth_client/credentials.py` & `palantir-oauth-client-1.6.0/palantir_oauth_client/credentials.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,37 +9,37 @@
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 import requests_oauthlib
-from datetime import datetime
+from datetime import datetime, timezone
 from typing import Any, List, Mapping, Optional
 
 from ._client import refresh_grant
 from ._utils import CLOCK_SKEW, utcnow
 from .errors import RefreshError
 
 
 class Credentials(object):
     """
     Credentials using OAuth 2.0 access and refresh tokens.
     """
 
     def __init__(
-            self,
-            token: str,
-            refresh_token: Optional[str] = None,
-            token_uri: Optional[str] = None,
-            client_id: Optional[str] = None,
-            client_secret: Optional[str] = None,
-            scopes: Optional[List[str]] = None,
-            default_scopes: Optional[List[str]] = None,
-            expiry: Optional[datetime] = None,
+        self,
+        token: str,
+        refresh_token: Optional[str] = None,
+        token_uri: Optional[str] = None,
+        client_id: Optional[str] = None,
+        client_secret: Optional[str] = None,
+        scopes: Optional[List[str]] = None,
+        default_scopes: Optional[List[str]] = None,
+        expiry: Optional[datetime] = None,
     ):
         """
         Args:
             token (Optional(str)): The OAuth 2.0 access token. Can be None if refresh information is provided.
             refresh_token (str): The OAuth 2.0 refresh token. If specified, credentials can be refreshed.
             token_uri (str): The OAuth 2.0 authorization server's token endpoint URI. Must be specified for refresh,
                 can be left as None if the token can not be refreshed.
@@ -61,17 +61,17 @@
         self._default_scopes = default_scopes
         self._token_uri = token_uri
         self._client_id = client_id
         self._client_secret = client_secret
 
     @classmethod
     def from_session(
-            cls,
-            session: requests_oauthlib.OAuth2Session,
-            client_config: Mapping[str, Any] = None,
+        cls,
+        session: requests_oauthlib.OAuth2Session,
+        client_config: Mapping[str, Any] = None,
     ):
         """
         Creates :class:`palantir_oauth_client.credentials.Credentials` from a :class:`requests_oauthlib.OAuth2Session`.
 
         :meth:`fetch_token` must be called on the session before calling this. This uses the session's auth token
         and the provided client configuration to create :class:`palantir_oauth_client.credentials.Credentials`.
         This allows you to use the credentials from the session with Foundry API client libraries.
@@ -88,17 +88,15 @@
             session.token["access_token"],
             refresh_token=session.token.get("refresh_token"),
             token_uri=client_config.get("token_uri"),
             client_id=client_config.get("client_id"),
             client_secret=client_config.get("client_secret"),
             scopes=session.scope,
         )
-        credentials.expiry = datetime.utcfromtimestamp(
-            session.token["expires_at"]
-        )
+        credentials.expiry = datetime.fromtimestamp(session.token["expires_at"], tz=timezone.utc)
         return credentials
 
     def __getstate__(self):
         return self.__dict__
 
     def __setstate__(self, d):
         self.token = d.get("token")
@@ -145,27 +143,25 @@
 
         This is True if the credentials have a :attr:`token` and the token is not :attr:`expired`.
         """
         return self.token is not None and not self.expired
 
     def refresh(self):
         if (
-                self._refresh_token is None
-                or self._token_uri is None
-                or self._client_id is None
+            self._refresh_token is None
+            or self._token_uri is None
+            or self._client_id is None
         ):
             raise RefreshError(
                 "The credentials do not contain the necessary fields need to "
                 "refresh the access token. You must specify refresh_token, "
                 "token_uri, client_id."
             )
 
-        scopes = (
-            self._scopes if self._scopes is not None else self._default_scopes
-        )
+        scopes = self._scopes if self._scopes is not None else self._default_scopes
 
         access_token, refresh_token, expiry, grant_response = refresh_grant(
             self._token_uri,
             self._refresh_token,
             self._client_id,
             self._client_secret,
             scopes,
@@ -174,16 +170,14 @@
         self.token = access_token
         self.expiry = expiry
         self._refresh_token = refresh_token
 
         if scopes and "scopes" in grant_response:
             requested_scopes = frozenset(scopes)
             granted_scopes = frozenset(grant_response["scopes"].split())
-            scopes_requested_but_not_granted = (
-                    requested_scopes - granted_scopes
-            )
+            scopes_requested_but_not_granted = requested_scopes - granted_scopes
             if scopes_requested_but_not_granted:
                 raise RefreshError(
                     "Not all requested scopes were granted by the authorization server, missing scopes {}.".format(
                         ", ".join(scopes_requested_but_not_granted)
                     )
                 )
```

### Comparing `palantir-oauth-client-1.5.6/palantir_oauth_client/errors.py` & `palantir-oauth-client-1.6.0/palantir_oauth_client/errors.py`

 * *Files identical despite different names*

### Comparing `palantir-oauth-client-1.5.6/pyproject.toml` & `palantir-oauth-client-1.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "palantir-oauth-client"
-version = "1.5.6" # placeholder, updated by git describe during publish
+version = "1.6.0" # placeholder, updated by git describe during publish
 description = "OAuth2 client for Palantir Foundry"
 license = "Apache-2.0"
 authors = [
   "Thomas Powell <tpowell@palantir.com>",
   "Andrew Higgins <ahiggins@palantir.com>",
 ]
 readme = "README.md"
```

### Comparing `palantir-oauth-client-1.5.6/setup.py` & `palantir-oauth-client-1.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 install_requires = \
 ['oauthlib>=3.2.2,<4.0.0',
  'requests-oauthlib>=1.3.1,<2.0.0',
  'requests>=2.28.2,<3.0.0']
 
 setup_kwargs = {
     'name': 'palantir-oauth-client',
-    'version': '1.5.6',
+    'version': '1.6.0',
     'description': 'OAuth2 client for Palantir Foundry',
     'long_description': 'Palantir OAuth Client\n==============\n\nA library for performing OAuth2 authentication with Multipass in order to obtain credentials for querying Foundry APIs.\n\nThis library supports two modes of operation for the [Authorization code](https://oauth.net/2/grant-types/authorization-code/)\nOAuth2 flow:\n\n1. Command line prompt: A user will be prompted to navigate to Foundry and enter the resulting ``authorization_code``\n   in their console after successful authentication.\n   \n2. Local webserver: A local webserver will be created to receive the redirect after successful authentication. The token\n   exchange will be performed automatically.\n\nIf the ``offline_access`` scope is specified, the credential will additionally contain a refresh token. When loading\ncached credentials (see below), the refresh token will be used to update invalid or expired credentials. In the case\ncredentials cannot be obtained the user will be prompted to log in as above.\n\nUsage\n-----\nUse the ``palantir_oauth_client.get_user_credentials()`` function to authenticate to Foundry APIs. \n\n```python\nimport requests\nfrom palantir_oauth_client import get_user_credentials\n\nhostname = "127.0.0.1:8080"\nclient_id = "f5496be223e4db85c6a7c99bc5c2d81a"\ncredentials = get_user_credentials(["offline_access"], hostname, client_id)\n\nheaders = {"Authorization": "Bearer " + credentials.token}\nresponse = requests.get(f"https://{hostname}/multipass/api/me", headers=headers)\nprint("Hello, {}!".format(response.json().get("username")))\n```\n\n## Client Registration\n\nA third-party client application needs to have been created in Multipass and the ``client_id`` provided when calling\n``palantir_oauth_client.get_user_credentials()``. This client should be registered as a _Public client_ (native or single-page\napplication) when it is not possible to securely store the ``client_secret``. The library uses the\n[PKCE OAuth2 extension](https://oauth.net/2/pkce/) for all requests regardless of the type of client that has been\nregistered.\n\nThe following redirect URIs should use be specified for each mode of operation:\n\n1. Command line prompt: ``https://<hostname>/multipass/api/oauth2/callback``\n\n2. Local webserver: ``http://127.0.0.1/``\n\n## Caching\n\nWhen obtaining credentials using ``palantir_oauth_client.get_user_credentials()`` you may specify a\n``palantir_oauth_client.cache.CredentialsCache``. There are three implementations:\n\n1. ``palantir_oauth_client.cache.READ_WRITE`` (default): A read-write cache that will persist credentials to disk when\n   ``offline_access`` scope is requested. The cached refresh tokens will be used when obtaining credentials where\n   possible to avoid explicit re-authentication.\n   \n2. ``palantir_oauth_client.cache.REAUTH``: A write-only cache that will persist credentials to disk when ``offline_access``\n   scope is requested but will require reauthentication when obtaining credentials.\n   \n3. ``palantir_oauth_client.cache.NOOP``: Always requires reauthentication and never persists credentials to disk.\n\nPersisted credentials will be stored in the default user home directory at ``~/.foundry/oauth``. Caching should\nonly be used when this home directory is secure and inaccessible by other users who would not otherwise have access to\nthe Foundry credentials.\n\n## Contributing\n\nSee the [CONTRIBUTING.md](./CONTRIBUTING.md) document. Releases are published to [pypi](https://pypi.org/project/palantir-oauth-client/) on tag builds and are automatically re-published to conda using conda-forge.\n\n## License\nThis project is made available under the [Apache 2.0 License](/LICENSE).\n',
     'author': 'Thomas Powell',
     'author_email': 'tpowell@palantir.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/palantir/palantir-oauth-client',
```

### Comparing `palantir-oauth-client-1.5.6/PKG-INFO` & `palantir-oauth-client-1.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: palantir-oauth-client
-Version: 1.5.6
+Version: 1.6.0
 Summary: OAuth2 client for Palantir Foundry
 Home-page: https://github.com/palantir/palantir-oauth-client
 License: Apache-2.0
 Author: Thomas Powell
 Author-email: tpowell@palantir.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

