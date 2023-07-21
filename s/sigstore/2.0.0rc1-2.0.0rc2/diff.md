# Comparing `tmp/sigstore-2.0.0rc1.tar.gz` & `tmp/sigstore-2.0.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sigstore-2.0.0rc1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "sigstore-2.0.0rc2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `sigstore-2.0.0rc1.tar` & `sigstore-2.0.0rc2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0    11358 2023-06-23 14:03:49.126171 sigstore-2.0.0rc1/LICENSE
--rw-r--r--   0        0        0    20790 2023-06-23 14:03:49.126171 sigstore-2.0.0rc1/README.md
--rw-r--r--   0        0        0     4131 2023-06-23 14:03:49.126171 sigstore-2.0.0rc1/pyproject.toml
--rw-r--r--   0        0        0      958 2023-06-23 14:03:49.126171 sigstore-2.0.0rc1/sigstore/__init__.py
--rw-r--r--   0        0        0      726 2023-06-23 14:03:49.126171 sigstore-2.0.0rc1/sigstore/__main__.py
--rw-r--r--   0        0        0    34259 2023-06-23 14:03:49.126171 sigstore-2.0.0rc1/sigstore/_cli.py
--rw-r--r--   0        0        0      738 2023-06-23 14:03:49.126171 sigstore-2.0.0rc1/sigstore/_internal/__init__.py
--rw-r--r--   0        0        0      774 2023-06-23 14:03:49.126171 sigstore-2.0.0rc1/sigstore/_internal/ctfe.py
--rw-r--r--   0        0        0      883 2023-06-23 14:03:49.126171 sigstore-2.0.0rc1/sigstore/_internal/fulcio/__init__.py
--rw-r--r--   0        0        0    11831 2023-06-23 14:03:49.126171 sigstore-2.0.0rc1/sigstore/_internal/fulcio/client.py
--rw-r--r--   0        0        0     3891 2023-06-23 14:03:49.126171 sigstore-2.0.0rc1/sigstore/_internal/keyring.py
--rw-r--r--   0        0        0     4544 2023-06-23 14:03:49.126171 sigstore-2.0.0rc1/sigstore/_internal/merkle.py
--rw-r--r--   0        0        0      653 2023-06-23 14:03:49.126171 sigstore-2.0.0rc1/sigstore/_internal/oidc/__init__.py
--rw-r--r--   0        0        0    15958 2023-06-23 14:03:49.126171 sigstore-2.0.0rc1/sigstore/_internal/oidc/oauth.py
--rw-r--r--   0        0        0      748 2023-06-23 14:03:49.126171 sigstore-2.0.0rc1/sigstore/_internal/rekor/__init__.py
--rw-r--r--   0        0        0     7301 2023-06-23 14:03:49.126171 sigstore-2.0.0rc1/sigstore/_internal/rekor/checkpoint.py
--rw-r--r--   0        0        0     9313 2023-06-23 14:03:49.126171 sigstore-2.0.0rc1/sigstore/_internal/rekor/client.py
--rw-r--r--   0        0        0     9162 2023-06-23 14:03:49.126171 sigstore-2.0.0rc1/sigstore/_internal/sct.py
--rw-r--r--   0        0        0     1508 2023-06-23 14:03:49.126171 sigstore-2.0.0rc1/sigstore/_internal/set.py
--rw-r--r--   0        0        0     9403 2023-06-23 14:03:49.126171 sigstore-2.0.0rc1/sigstore/_internal/tuf.py
--rw-r--r--   0        0        0     1247 2023-06-23 14:03:49.126171 sigstore-2.0.0rc1/sigstore/_store/__init__.py
--rw-r--r--   0        0        0     6388 2023-06-23 14:03:49.126171 sigstore-2.0.0rc1/sigstore/_store/prod/root.json
--rw-r--r--   0        0        0     4567 2023-06-23 14:03:49.126171 sigstore-2.0.0rc1/sigstore/_store/prod/trusted_root.json
--rw-r--r--   0        0        0     1876 2023-06-23 14:03:49.126171 sigstore-2.0.0rc1/sigstore/_store/staging/root.json
--rw-r--r--   0        0        0     4521 2023-06-23 14:03:49.126171 sigstore-2.0.0rc1/sigstore/_store/staging/trusted_root.json
--rw-r--r--   0        0        0    10657 2023-06-23 14:03:49.126171 sigstore-2.0.0rc1/sigstore/_utils.py
--rw-r--r--   0        0        0     3247 2023-06-23 14:03:49.126171 sigstore-2.0.0rc1/sigstore/errors.py
--rw-r--r--   0        0        0    15934 2023-06-23 14:03:49.126171 sigstore-2.0.0rc1/sigstore/oidc.py
--rw-r--r--   0        0        0    12380 2023-06-23 14:03:49.126171 sigstore-2.0.0rc1/sigstore/sign.py
--rw-r--r--   0        0        0     4735 2023-06-23 14:03:49.126171 sigstore-2.0.0rc1/sigstore/transparency.py
--rw-r--r--   0        0        0     1932 2023-06-23 14:03:49.126171 sigstore-2.0.0rc1/sigstore/verify/__init__.py
--rw-r--r--   0        0        0    13404 2023-06-23 14:03:49.130168 sigstore-2.0.0rc1/sigstore/verify/models.py
--rw-r--r--   0        0        0     9824 2023-06-23 14:03:49.130168 sigstore-2.0.0rc1/sigstore/verify/policy.py
--rw-r--r--   0        0        0    11219 2023-06-23 14:03:49.130168 sigstore-2.0.0rc1/sigstore/verify/verifier.py
--rw-r--r--   0        0        0    23085 1970-01-01 00:00:00.000000 sigstore-2.0.0rc1/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-07-21 19:10:50.383551 sigstore-2.0.0rc2/LICENSE
+-rw-r--r--   0        0        0    20790 2023-07-21 19:10:50.383551 sigstore-2.0.0rc2/README.md
+-rw-r--r--   0        0        0     4102 2023-07-21 19:10:50.383551 sigstore-2.0.0rc2/pyproject.toml
+-rw-r--r--   0        0        0      958 2023-07-21 19:10:50.383551 sigstore-2.0.0rc2/sigstore/__init__.py
+-rw-r--r--   0        0        0      726 2023-07-21 19:10:50.383551 sigstore-2.0.0rc2/sigstore/__main__.py
+-rw-r--r--   0        0        0    34259 2023-07-21 19:10:50.383551 sigstore-2.0.0rc2/sigstore/_cli.py
+-rw-r--r--   0        0        0      738 2023-07-21 19:10:50.383551 sigstore-2.0.0rc2/sigstore/_internal/__init__.py
+-rw-r--r--   0        0        0      774 2023-07-21 19:10:50.383551 sigstore-2.0.0rc2/sigstore/_internal/ctfe.py
+-rw-r--r--   0        0        0      883 2023-07-21 19:10:50.383551 sigstore-2.0.0rc2/sigstore/_internal/fulcio/__init__.py
+-rw-r--r--   0        0        0    11984 2023-07-21 19:10:50.383551 sigstore-2.0.0rc2/sigstore/_internal/fulcio/client.py
+-rw-r--r--   0        0        0     3891 2023-07-21 19:10:50.383551 sigstore-2.0.0rc2/sigstore/_internal/keyring.py
+-rw-r--r--   0        0        0     4544 2023-07-21 19:10:50.383551 sigstore-2.0.0rc2/sigstore/_internal/merkle.py
+-rw-r--r--   0        0        0      653 2023-07-21 19:10:50.383551 sigstore-2.0.0rc2/sigstore/_internal/oidc/__init__.py
+-rw-r--r--   0        0        0    15958 2023-07-21 19:10:50.383551 sigstore-2.0.0rc2/sigstore/_internal/oidc/oauth.py
+-rw-r--r--   0        0        0      748 2023-07-21 19:10:50.383551 sigstore-2.0.0rc2/sigstore/_internal/rekor/__init__.py
+-rw-r--r--   0        0        0     7301 2023-07-21 19:10:50.383551 sigstore-2.0.0rc2/sigstore/_internal/rekor/checkpoint.py
+-rw-r--r--   0        0        0     9311 2023-07-21 19:10:50.383551 sigstore-2.0.0rc2/sigstore/_internal/rekor/client.py
+-rw-r--r--   0        0        0     9884 2023-07-21 19:10:50.387550 sigstore-2.0.0rc2/sigstore/_internal/sct.py
+-rw-r--r--   0        0        0     1729 2023-07-21 19:10:50.387550 sigstore-2.0.0rc2/sigstore/_internal/set.py
+-rw-r--r--   0        0        0     9403 2023-07-21 19:10:50.387550 sigstore-2.0.0rc2/sigstore/_internal/tuf.py
+-rw-r--r--   0        0        0     1247 2023-07-21 19:10:50.387550 sigstore-2.0.0rc2/sigstore/_store/__init__.py
+-rw-r--r--   0        0        0     6388 2023-07-21 19:10:50.387550 sigstore-2.0.0rc2/sigstore/_store/prod/root.json
+-rw-r--r--   0        0        0     4567 2023-07-21 19:10:50.387550 sigstore-2.0.0rc2/sigstore/_store/prod/trusted_root.json
+-rw-r--r--   0        0        0     1876 2023-07-21 19:10:50.387550 sigstore-2.0.0rc2/sigstore/_store/staging/root.json
+-rw-r--r--   0        0        0     4521 2023-07-21 19:10:50.387550 sigstore-2.0.0rc2/sigstore/_store/staging/trusted_root.json
+-rw-r--r--   0        0        0    10354 2023-07-21 19:10:50.387550 sigstore-2.0.0rc2/sigstore/_utils.py
+-rw-r--r--   0        0        0     3247 2023-07-21 19:10:50.387550 sigstore-2.0.0rc2/sigstore/errors.py
+-rw-r--r--   0        0        0    15934 2023-07-21 19:10:50.387550 sigstore-2.0.0rc2/sigstore/oidc.py
+-rw-r--r--   0        0        0    12464 2023-07-21 19:10:50.387550 sigstore-2.0.0rc2/sigstore/sign.py
+-rw-r--r--   0        0        0     5247 2023-07-21 19:10:50.387550 sigstore-2.0.0rc2/sigstore/transparency.py
+-rw-r--r--   0        0        0     1932 2023-07-21 19:10:50.387550 sigstore-2.0.0rc2/sigstore/verify/__init__.py
+-rw-r--r--   0        0        0    14711 2023-07-21 19:10:50.387550 sigstore-2.0.0rc2/sigstore/verify/models.py
+-rw-r--r--   0        0        0     9824 2023-07-21 19:10:50.387550 sigstore-2.0.0rc2/sigstore/verify/policy.py
+-rw-r--r--   0        0        0    11336 2023-07-21 19:10:50.387550 sigstore-2.0.0rc2/sigstore/verify/verifier.py
+-rw-r--r--   0        0        0    23086 1970-01-01 00:00:00.000000 sigstore-2.0.0rc2/PKG-INFO
```

### Comparing `sigstore-2.0.0rc1/LICENSE` & `sigstore-2.0.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `sigstore-2.0.0rc1/README.md` & `sigstore-2.0.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `sigstore-2.0.0rc1/pyproject.toml` & `sigstore-2.0.0rc2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [project]
 name = "sigstore"
 dynamic = ["version"]
 description = "A tool for signing Python package distributions"
 readme = "README.md"
 license = { file = "LICENSE" }
 authors = [
-  { name = "Sigstore Authors", email = "sigstore-dev@googlegroups.com" }
+  { name = "Sigstore Authors", email = "sigstore-dev@googlegroups.com" },
 ]
 classifiers = [
   "License :: OSI Approved :: Apache Software License",
   "Programming Language :: Python :: 3 :: Only",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
@@ -26,64 +26,53 @@
   "Topic :: Security :: Cryptography",
 ]
 dependencies = [
   "appdirs ~= 1.4",
   "cryptography >= 39",
   "id >= 1.0.0",
   "importlib_resources ~= 5.7; python_version < '3.11'",
-  "pydantic ~= 1.10",
+  "pydantic >= 2,< 3",
   "pyjwt >= 2.1",
   "pyOpenSSL >= 23.0.0",
   "requests",
   "securesystemslib",
-  "sigstore-protobuf-specs ~= 0.1.0",
+  "sigstore-protobuf-specs ~= 0.2.0",
   "tuf >= 2.1,< 4.0",
 ]
 requires-python = ">=3.7"
 
 [project.scripts]
 sigstore = "sigstore._cli:main"
 
 [project.urls]
 Homepage = "https://pypi.org/project/sigstore/"
 Issues = "https://github.com/sigstore/sigstore-python/issues"
 Source = "https://github.com/sigstore/sigstore-python"
 Documentation = "https://sigstore.github.io/sigstore-python/"
 
 [project.optional-dependencies]
-test = [
-  "pytest",
-  "pytest-cov",
-  "pretend",
-  "coverage[toml]",
-]
+test = ["pytest", "pytest-cov", "pretend", "coverage[toml]"]
 lint = [
   "bandit",
   "black",
   "isort",
   "interrogate",
   "mypy ~= 1.1",
   # NOTE(ww): ruff is under active development, so we pin conservatively here
   # and let Dependabot periodically perform this update.
-  "ruff < 0.0.275",
+  "ruff < 0.0.279",
   "types-requests",
   # Needed for protocol typing in 3.7; remove when our minimum Python is 3.8.
   "typing-extensions; python_version < '3.8'",
   # TODO(ww): Re-enable once dependency on types-cryptography is dropped.
   # See: https://github.com/python/typeshed/issues/8699
   # "types-pyOpenSSL",
 ]
-doc = [
-  "pdoc",
-]
-dev = [
-  "build",
-  "bump >= 1.3.2",
-  "sigstore[doc,test,lint]",
-]
+doc = ["pdoc"]
+dev = ["build", "bump >= 1.3.2", "sigstore[doc,test,lint]"]
 
 [tool.isort]
 multi_line_output = 3
 known_first_party = "sigstore"
 include_trailing_comma = true
 
 [tool.coverage.run]
@@ -96,17 +85,17 @@
 # see: https://coverage.readthedocs.io/en/7.1.0/config.html#config-run-relative-files
 relative_files = true
 # don't attempt code coverage for the CLI entrypoints
 omit = ["sigstore/_cli.py"]
 
 [tool.coverage.report]
 exclude_lines = [
-    "@abc.abstractmethod",
-    "@typing.overload",
-    "if typing.TYPE_CHECKING",
+  "@abc.abstractmethod",
+  "@typing.overload",
+  "if typing.TYPE_CHECKING",
 ]
 
 [tool.interrogate]
 # don't enforce documentation coverage for packaging, testing, the virtual
 # environment, or the CLI (which is documented separately).
 exclude = ["env", "test", "sigstore/_cli.py"]
 ignore-semiprivate = true
```

### Comparing `sigstore-2.0.0rc1/sigstore/__init__.py` & `sigstore-2.0.0rc2/sigstore/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,8 +21,8 @@
 Otherwise, here are some quick starting points:
 
 * `sigstore.verify`: verifying of Sigstore signatures,
   including flexible policy control
 * `sigstore.sign`: creation of Sigstore signatures
 """
 
-__version__ = "2.0.0rc1"
+__version__ = "2.0.0rc2"
```

### Comparing `sigstore-2.0.0rc1/sigstore/__main__.py` & `sigstore-2.0.0rc2/sigstore/__main__.py`

 * *Files identical despite different names*

### Comparing `sigstore-2.0.0rc1/sigstore/_cli.py` & `sigstore-2.0.0rc2/sigstore/_cli.py`

 * *Files identical despite different names*

### Comparing `sigstore-2.0.0rc1/sigstore/_internal/__init__.py` & `sigstore-2.0.0rc2/sigstore/_internal/__init__.py`

 * *Files identical despite different names*

### Comparing `sigstore-2.0.0rc1/sigstore/_internal/ctfe.py` & `sigstore-2.0.0rc2/sigstore/_internal/ctfe.py`

 * *Files identical despite different names*

### Comparing `sigstore-2.0.0rc1/sigstore/_internal/fulcio/__init__.py` & `sigstore-2.0.0rc2/sigstore/_internal/fulcio/__init__.py`

 * *Files identical despite different names*

### Comparing `sigstore-2.0.0rc1/sigstore/_internal/fulcio/client.py` & `sigstore-2.0.0rc2/sigstore/_internal/fulcio/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 )
 from cryptography.x509.certificate_transparency import (
     LogEntryType,
     SignatureAlgorithm,
     SignedCertificateTimestamp,
     Version,
 )
-from pydantic import BaseModel, Field, validator
+from pydantic import BaseModel, ConfigDict, Field, validator
 
 from sigstore._utils import B64Str
 from sigstore.oidc import IdentityToken
 
 logger = logging.getLogger(__name__)
 
 DEFAULT_FULCIO_URL = "https://fulcio.sigstore.dev"
@@ -92,23 +92,25 @@
 
 
 class DetachedFulcioSCT(BaseModel):
     """
     Represents a "detached" SignedCertificateTimestamp from Fulcio.
     """
 
+    model_config = ConfigDict(populate_by_name=True, arbitrary_types_allowed=True)
+
     version: Version = Field(..., alias="sct_version")
     log_id: bytes = Field(..., alias="id")
     timestamp: datetime.datetime
     digitally_signed: bytes = Field(..., alias="signature")
     extension_bytes: bytes = Field(..., alias="extensions")
 
-    class Config:
-        allow_population_by_field_name = True
-        arbitrary_types_allowed = True
+    @validator("timestamp")
+    def _validate_timestamp(cls, v: datetime.datetime) -> datetime.datetime:
+        return v.replace(tzinfo=datetime.timezone.utc)
 
     @validator("digitally_signed", pre=True)
     def _validate_digitally_signed(cls, v: bytes) -> bytes:
         digitally_signed = base64.b64decode(v)
 
         if len(digitally_signed) <= 4:
             raise ValueError("impossibly small digitally-signed struct")
```

### Comparing `sigstore-2.0.0rc1/sigstore/_internal/keyring.py` & `sigstore-2.0.0rc2/sigstore/_internal/keyring.py`

 * *Files identical despite different names*

### Comparing `sigstore-2.0.0rc1/sigstore/_internal/merkle.py` & `sigstore-2.0.0rc2/sigstore/_internal/merkle.py`

 * *Files identical despite different names*

### Comparing `sigstore-2.0.0rc1/sigstore/_internal/oidc/__init__.py` & `sigstore-2.0.0rc2/sigstore/_internal/oidc/__init__.py`

 * *Files identical despite different names*

### Comparing `sigstore-2.0.0rc1/sigstore/_internal/oidc/oauth.py` & `sigstore-2.0.0rc2/sigstore/_internal/oidc/oauth.py`

 * *Files identical despite different names*

### Comparing `sigstore-2.0.0rc1/sigstore/_internal/rekor/__init__.py` & `sigstore-2.0.0rc2/sigstore/_internal/rekor/__init__.py`

 * *Files identical despite different names*

### Comparing `sigstore-2.0.0rc1/sigstore/_internal/rekor/checkpoint.py` & `sigstore-2.0.0rc2/sigstore/_internal/rekor/checkpoint.py`

 * *Files identical despite different names*

### Comparing `sigstore-2.0.0rc1/sigstore/_internal/rekor/client.py` & `sigstore-2.0.0rc2/sigstore/_internal/rekor/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -222,15 +222,15 @@
 
         resp: requests.Response = self.session.post(self.url, json=data)
         try:
             resp.raise_for_status()
         except requests.HTTPError as http_error:
             if http_error.response.status_code == 404:
                 return None
-            raise RekorClientError(resp.json()) from http_error
+            raise RekorClientError(resp.text) from http_error
 
         results = resp.json()
 
         # The response is a list of `{uuid: LogEntry}` objects.
         # We select the oldest entry for our actual return value,
         # since a malicious actor could conceivably spam the log with
         # newer duplicate entries.
```

### Comparing `sigstore-2.0.0rc1/sigstore/_internal/sct.py` & `sigstore-2.0.0rc2/sigstore/_internal/sct.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,28 +20,34 @@
 import struct
 from datetime import timezone
 from textwrap import dedent
 from typing import List, Optional
 
 from cryptography.hazmat.primitives import hashes, serialization
 from cryptography.hazmat.primitives.asymmetric import ec, rsa
-from cryptography.x509 import Certificate, ExtendedKeyUsage
+from cryptography.x509 import Certificate, ExtendedKeyUsage, ExtensionNotFound
 from cryptography.x509.certificate_transparency import (
     LogEntryType,
     SignedCertificateTimestamp,
 )
 from cryptography.x509.oid import ExtendedKeyUsageOID
 
 from sigstore._internal.ctfe import CTKeyring
 from sigstore._internal.keyring import (
     KeyringError,
     KeyringLookupError,
     KeyringSignatureError,
 )
-from sigstore._utils import DERCert, KeyID, key_id
+from sigstore._utils import (
+    DERCert,
+    InvalidCertError,
+    KeyID,
+    cert_is_ca,
+    key_id,
+)
 from sigstore.errors import Error
 
 logger = logging.getLogger(__name__)
 
 
 def _pack_signed_entry(
     sct: SignedCertificateTimestamp, cert: Certificate, issuer_key_id: Optional[bytes]
@@ -123,26 +129,40 @@
     )
     # fmt: on
 
     return data
 
 
 def _is_preissuer(issuer: Certificate) -> bool:
-    ext_key_usage = issuer.extensions.get_extension_for_class(ExtendedKeyUsage)
+    try:
+        ext_key_usage = issuer.extensions.get_extension_for_class(ExtendedKeyUsage)
+    # If we do not have any EKU, we certainly do not have CT Ext
+    except ExtensionNotFound:
+        return False
 
     return ExtendedKeyUsageOID.CERTIFICATE_TRANSPARENCY in ext_key_usage.value
 
 
 def _get_issuer_cert(chain: List[Certificate]) -> Certificate:
     issuer = chain[0]
     if _is_preissuer(issuer):
         issuer = chain[1]
     return issuer
 
 
+def _cert_is_ca(cert: Certificate) -> bool:
+    logger.debug(f"Found {cert.subject} as issuer, verifying if it is a ca")
+    try:
+        cert_is_ca(cert)
+    except InvalidCertError as e:
+        logger.debug(f"Invalid {cert.subject}: failed to validate as a CA: {e}")
+        return False
+    return True
+
+
 class InvalidSCTError(Error):
     """
     Raised during SCT verification if an SCT is invalid in some way.
     """
 
     def diagnostics(self) -> str:
         """Returns diagnostics for the error."""
@@ -227,15 +247,21 @@
 
     issuer_key_id = None
     if sct.entry_type == LogEntryType.PRE_CERTIFICATE:
         # If we're verifying an SCT for a precertificate, we need to
         # find its issuer in the chain and calculate a hash over
         # its public key information, as part of the "binding" proof
         # that ties the issuer to the final certificate.
-        issuer_pubkey = _get_issuer_cert(chain).public_key()
+        issuer_cert = _get_issuer_cert(chain)
+        issuer_pubkey = issuer_cert.public_key()
+
+        if not _cert_is_ca(issuer_cert):
+            raise InvalidSCTError(
+                f"Invalid issuer pubkey basicConstraint (not a CA): {issuer_pubkey}"
+            )
 
         if not isinstance(issuer_pubkey, (rsa.RSAPublicKey, ec.EllipticCurvePublicKey)):
             raise InvalidSCTError(
                 f"invalid issuer pubkey format (not ECDSA or RSA): {issuer_pubkey}"
             )
 
         issuer_key_id = key_id(issuer_pubkey)
```

### Comparing `sigstore-2.0.0rc1/sigstore/_internal/set.py` & `sigstore-2.0.0rc2/sigstore/_internal/set.py`

 * *Files 11% similar despite different names*

```diff
@@ -31,16 +31,21 @@
     """
 
     pass
 
 
 def verify_set(client: RekorClient, entry: LogEntry) -> None:
     """
-    Verify the Signed Entry Timestamp for a given Rekor `entry` using the given `client`.
+    Verify the inclusion promise (Signed Entry Timestamp) for a given transparency log
+    `entry` using the given `client`.
+
+    Fails if the given log entry does not contain an inclusion promise.
     """
+    if entry.inclusion_promise is None:
+        raise InvalidSETError("invalid log entry: no inclusion promise")
 
     signed_entry_ts = base64.b64decode(entry.inclusion_promise)
 
     try:
         client._rekor_keyring.verify(
             key_id=KeyID(bytes.fromhex(entry.log_id)),
             signature=signed_entry_ts,
```

### Comparing `sigstore-2.0.0rc1/sigstore/_internal/tuf.py` & `sigstore-2.0.0rc2/sigstore/_internal/tuf.py`

 * *Files identical despite different names*

### Comparing `sigstore-2.0.0rc1/sigstore/_store/__init__.py` & `sigstore-2.0.0rc2/sigstore/_store/__init__.py`

 * *Files identical despite different names*

### Comparing `sigstore-2.0.0rc1/sigstore/_store/prod/root.json` & `sigstore-2.0.0rc2/sigstore/_store/prod/root.json`

 * *Files identical despite different names*

### Comparing `sigstore-2.0.0rc1/sigstore/_store/prod/trusted_root.json` & `sigstore-2.0.0rc2/sigstore/_store/prod/trusted_root.json`

 * *Files identical despite different names*

### Comparing `sigstore-2.0.0rc1/sigstore/_store/staging/root.json` & `sigstore-2.0.0rc2/sigstore/_store/staging/root.json`

 * *Files identical despite different names*

### Comparing `sigstore-2.0.0rc1/sigstore/_store/staging/trusted_root.json` & `sigstore-2.0.0rc2/sigstore/_store/staging/trusted_root.json`

 * *Files identical despite different names*

### Comparing `sigstore-2.0.0rc1/sigstore/_utils.py` & `sigstore-2.0.0rc2/sigstore/_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -222,36 +222,32 @@
             )
 
         ca = basic_constraints.value.ca  # type: ignore
     except ExtensionNotFound:
         # No BasicConstrains means that this can't possibly be a CA.
         return False
 
-    digital_signature = False
     key_cert_sign = False
     try:
         key_usage = cert.extensions.get_extension_for_oid(ExtensionOID.KEY_USAGE)
         key_cert_sign = key_usage.value.key_cert_sign  # type: ignore
-        digital_signature = key_usage.value.digital_signature  # type: ignore
     except ExtensionNotFound:
         raise InvalidCertError("invalid X.509 certificate: missing KeyUsage")
 
-    # If all three states are set, this is a CA.
-    if ca and key_cert_sign and digital_signature:
+    # If both states are set, this is a CA.
+    if ca and key_cert_sign:
         return True
 
-    # Non-CA in the Sigstore ecosystem have `digitalSignature` but neither of
-    # the CA states.
-    if digital_signature and not (ca or key_cert_sign):
+    if not (ca or key_cert_sign):
         return False
 
     # Anything else is an invalid state that should never occur.
     raise InvalidCertError(
-        f"invalid certificate states: KeyUsage.digitalSignature={digital_signature}, "
-        f"KeyUsage.keyCertSign={key_cert_sign}, BasicConstraints.ca={ca}"
+        f"invalid certificate states: KeyUsage.keyCertSign={key_cert_sign}"
+        f", BasicConstraints.ca={ca}"
     )
 
 
 def cert_is_root_ca(cert: Certificate) -> bool:
     """
     Returns `True` if and only if the given `Certificate` indicates
     that it's a root CA.
```

### Comparing `sigstore-2.0.0rc1/sigstore/errors.py` & `sigstore-2.0.0rc2/sigstore/errors.py`

 * *Files identical despite different names*

### Comparing `sigstore-2.0.0rc1/sigstore/oidc.py` & `sigstore-2.0.0rc2/sigstore/oidc.py`

 * *Files identical despite different names*

### Comparing `sigstore-2.0.0rc1/sigstore/sign.py` & `sigstore-2.0.0rc2/sigstore/sign.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,27 +16,27 @@
 API for signing artifacts.
 
 Example:
 
 ```python
 from pathlib import Path
 
-from sigstore.sign import Signer
+from sigstore.sign import SigningContext
 from sigstore.oidc import Issuer
 
 issuer = Issuer.production()
 identity = issuer.identity_token()
 
 # The artifact to sign
 artifact = Path("foo.txt")
 
-with artifact.open("rb") as a:
+with artifact.open("rb") as file:
     signing_ctx = SigningContext.production()
     with signing_ctx.signer(identity, cache=True) as signer:
-        result = signer.sign(input_=a, rekor=signing_ctx._rekor, fulcio=signing_ctx._fulcio)
+        result = signer.sign(file)
         print(result)
 ```
 """
 
 from __future__ import annotations
 
 import base64
@@ -133,18 +133,17 @@
     def _signing_cert(
         self,
         private_key: ec.EllipticCurvePrivateKey,
     ) -> FulcioCertificateSigningResponse:
         """Get or request a signing certificate from Fulcio."""
         # If it exists, verify if the current certificate is expired
         if self.__cached_signing_certificate:
-            if (
-                datetime.now(timezone.utc).timestamp()
-                > self.__cached_signing_certificate.cert.not_valid_after.timestamp()
-            ):
+            not_valid_after = self.__cached_signing_certificate.cert.not_valid_after
+            not_valid_after_tzutc = not_valid_after.replace(tzinfo=timezone.utc)
+            if datetime.now(timezone.utc) > not_valid_after_tzutc:
                 raise ExpiredCertificate
             return self.__cached_signing_certificate
 
         else:
             logger.debug("Retrieving signed certificate...")
 
             # Build an X.509 Certificiate Signing Request
@@ -350,26 +349,28 @@
             log_id=LogId(key_id=bytes.fromhex(self.log_entry.log_id)),
             kind_version=KindVersion(kind="hashedrekord", version="0.0.1"),
             integrated_time=self.log_entry.integrated_time,
             inclusion_promise=InclusionPromise(
                 signed_entry_timestamp=base64.b64decode(
                     self.log_entry.inclusion_promise
                 )
-            ),
+            )
+            if self.log_entry.inclusion_promise
+            else None,
             inclusion_proof=inclusion_proof,
             canonicalized_body=base64.b64decode(self.log_entry.body),
         )
 
         material = VerificationMaterial(
             x509_certificate_chain=chain,
             tlog_entries=[tlog_entry],
         )
 
         bundle = Bundle(
-            media_type="application/vnd.dev.sigstore.bundle+json;version=0.1",
+            media_type="application/vnd.dev.sigstore.bundle+json;version=0.2",
             verification_material=material,
             message_signature=MessageSignature(
                 message_digest=HashOutput(
                     algorithm=HashAlgorithm.SHA2_256,
                     digest=bytes.fromhex(self.input_digest),
                 ),
                 signature=base64.b64decode(self.b64_signature),
```

### Comparing `sigstore-2.0.0rc1/sigstore/transparency.py` & `sigstore-2.0.0rc2/sigstore/transparency.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,30 +14,78 @@
 
 """
 Transparency log data structures.
 """
 
 from __future__ import annotations
 
-from dataclasses import dataclass
 from typing import Any, Dict, List, Optional
 
-from pydantic import BaseModel, Field, StrictInt, StrictStr, validator
+from pydantic import (
+    BaseModel,
+    ConfigDict,
+    Field,
+    StrictInt,
+    StrictStr,
+    validator,
+)
+from pydantic.dataclasses import dataclass
 from securesystemslib.formats import encode_canonical
 
 from sigstore._utils import B64Str
 
 
+class LogInclusionProof(BaseModel):
+    """
+    Represents an inclusion proof for a transparency log entry.
+    """
+
+    model_config = ConfigDict(populate_by_name=True)
+
+    checkpoint: StrictStr = Field(..., alias="checkpoint")
+    hashes: List[StrictStr] = Field(..., alias="hashes")
+    log_index: StrictInt = Field(..., alias="logIndex")
+    root_hash: StrictStr = Field(..., alias="rootHash")
+    tree_size: StrictInt = Field(..., alias="treeSize")
+
+    @validator("log_index")
+    def _log_index_positive(cls, v: int) -> int:
+        if v < 0:
+            raise ValueError(f"Inclusion proof has invalid log index: {v} < 0")
+        return v
+
+    @validator("tree_size")
+    def _tree_size_positive(cls, v: int) -> int:
+        if v < 0:
+            raise ValueError(f"Inclusion proof has invalid tree size: {v} < 0")
+        return v
+
+    @validator("tree_size")
+    def _log_index_within_tree_size(
+        cls, v: int, values: Dict[str, Any], **kwargs: Any
+    ) -> int:
+        if "log_index" in values and v <= values["log_index"]:
+            raise ValueError(
+                "Inclusion proof has log index greater than or equal to tree size: "
+                f"{v} <= {values['log_index']}"
+            )
+        return v
+
+
 @dataclass(frozen=True)
 class LogEntry:
     """
     Represents a transparency log entry.
 
     Log entries are retrieved from the transparency log after signing or verification events,
     or loaded from "Sigstore" bundles provided by the user.
+
+    This representation allows for either a missing inclusion promise or a missing
+    inclusion proof, but not both: attempting to construct a `LogEntry` without
+    at least one will fail.
     """
 
     uuid: Optional[str]
     """
     This entry's unique ID in the log instance it was retrieved from.
 
     For sharded log deployments, IDs are unique per-shard.
@@ -64,25 +112,32 @@
     log_index: int
     """
     The index of this entry within the log.
     """
 
     inclusion_proof: Optional[LogInclusionProof]
     """
-    An optional inclusion proof for this log entry.
+    An inclusion proof for this log entry, if present.
     """
 
-    inclusion_promise: B64Str
+    inclusion_promise: Optional[B64Str]
     """
-    An inclusion promise for this log entry.
+    An inclusion promise for this log entry, if present.
 
     Internally, this is a base64-encoded Signed Entry Timestamp (SET) for this
     log entry.
     """
 
+    def __post_init__(self) -> None:
+        """
+        Invariant preservation.
+        """
+        if self.inclusion_proof is None and self.inclusion_promise is None:
+            raise ValueError("Log entry must have either inclusion proof or promise")
+
     @classmethod
     def _from_response(cls, dict_: dict[str, Any]) -> LogEntry:
         """
         Create a new `LogEntry` from the given API response.
         """
 
         # Assumes we only get one entry back
@@ -114,45 +169,7 @@
             "body": self.body,
             "integratedTime": self.integrated_time,
             "logID": self.log_id,
             "logIndex": self.log_index,
         }
 
         return encode_canonical(payload).encode()  # type: ignore
-
-
-class LogInclusionProof(BaseModel):
-    """
-    Represents an inclusion proof for a transparency log entry.
-    """
-
-    checkpoint: StrictStr = Field(..., alias="checkpoint")
-    hashes: List[StrictStr] = Field(..., alias="hashes")
-    log_index: StrictInt = Field(..., alias="logIndex")
-    root_hash: StrictStr = Field(..., alias="rootHash")
-    tree_size: StrictInt = Field(..., alias="treeSize")
-
-    class Config:
-        allow_population_by_field_name = True
-
-    @validator("log_index")
-    def _log_index_positive(cls, v: int) -> int:
-        if v < 0:
-            raise ValueError(f"Inclusion proof has invalid log index: {v} < 0")
-        return v
-
-    @validator("tree_size")
-    def _tree_size_positive(cls, v: int) -> int:
-        if v < 0:
-            raise ValueError(f"Inclusion proof has invalid tree size: {v} < 0")
-        return v
-
-    @validator("tree_size")
-    def _log_index_within_tree_size(
-        cls, v: int, values: Dict[str, Any], **kwargs: Any
-    ) -> int:
-        if "log_index" in values and v <= values["log_index"]:
-            raise ValueError(
-                "Inclusion proof has log index greater than or equal to tree size: "
-                f"{v} <= {values['log_index']}"
-            )
-        return v
```

### Comparing `sigstore-2.0.0rc1/sigstore/verify/__init__.py` & `sigstore-2.0.0rc2/sigstore/verify/__init__.py`

 * *Files identical despite different names*

### Comparing `sigstore-2.0.0rc1/sigstore/verify/models.py` & `sigstore-2.0.0rc2/sigstore/verify/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,14 +29,18 @@
 from cryptography.x509 import (
     Certificate,
     load_der_x509_certificate,
     load_pem_x509_certificate,
 )
 from pydantic import BaseModel
 from sigstore_protobuf_specs.dev.sigstore.bundle.v1 import Bundle
+from sigstore_protobuf_specs.dev.sigstore.rekor.v1 import (
+    InclusionPromise,
+    InclusionProof,
+)
 
 from sigstore._internal.rekor import RekorClient
 from sigstore._utils import (
     B64Str,
     PEMCert,
     base64_encode_pem_cert,
     cert_is_leaf,
@@ -44,14 +48,21 @@
     sha256_streaming,
 )
 from sigstore.errors import Error
 from sigstore.transparency import LogEntry, LogInclusionProof
 
 logger = logging.getLogger(__name__)
 
+_BUNDLE_0_1 = "application/vnd.dev.sigstore.bundle+json;version=0.1"
+_BUNDLE_0_2 = "application/vnd.dev.sigstore.bundle+json;version=0.2"
+_KNOWN_BUNDLE_TYPES = {
+    _BUNDLE_0_1,
+    _BUNDLE_0_2,
+}
+
 
 class VerificationResult(BaseModel):
     """
     Represents the result of a verification operation.
 
     Results are boolish, and failures contain a reason (and potentially
     some additional context).
@@ -238,14 +249,17 @@
         cls, *, input_: IO[bytes], bundle: Bundle, offline: bool = False
     ) -> VerificationMaterials:
         """
         Create a new `VerificationMaterials` from the given Sigstore bundle.
 
         Effect: `input_` is consumed as part of construction.
         """
+        if bundle.media_type not in _KNOWN_BUNDLE_TYPES:
+            raise InvalidMaterials(f"unsupported bundle format: {bundle.media_type}")
+
         certs = bundle.verification_material.x509_certificate_chain.certificates
 
         if len(certs) == 0:
             raise InvalidMaterials("expected non-empty certificate chain in bundle")
 
         # Per client policy in protobuf-specs: the first entry in the chain
         # MUST be a leaf certificate, and the rest of the chain MUST NOT
@@ -276,30 +290,47 @@
         tlog_entries = bundle.verification_material.tlog_entries
         if len(tlog_entries) != 1:
             raise InvalidMaterials(
                 f"expected exactly one log entry, got {len(tlog_entries)}"
             )
         tlog_entry = tlog_entries[0]
 
-        # NOTE: Bundles are not required to include inclusion proofs,
-        # since offline (or non-gossiped) verification of an inclusion proof is
-        # only as strong as verification of the inclusion promise, which
-        # is always provided.
-        inclusion_proof = tlog_entry.inclusion_proof
-        parsed_inclusion_proof: LogInclusionProof | None = None
-        if inclusion_proof:
-            checkpoint = inclusion_proof.checkpoint
-
-            # If the inclusion proof is provided, it must include its
-            # checkpoint.
-            if not checkpoint.envelope:
+        # Handling of inclusion promises and proofs varies between bundle
+        # format versions:
+        #
+        # * For 0.1, an inclusion promise is required; the client
+        #   MUST verify the inclusion promise.
+        #   The inclusion proof is NOT required. If provided, it might NOT
+        #   contain a checkpoint; in this case, we ignore it (since it's
+        #   useless without one).
+        #
+        # * For 0.2, an inclusion proof is required; the client MUST
+        #   verify the inclusion proof. The inclusion prof MUST contain
+        #   a checkpoint.
+        #   The inclusion promise is NOT required; if present, the client
+        #   SHOULD verify it.
+
+        inclusion_promise: InclusionPromise | None = tlog_entry.inclusion_promise
+        inclusion_proof: InclusionProof | None = tlog_entry.inclusion_proof
+        if bundle.media_type == _BUNDLE_0_1:
+            if not inclusion_promise:
+                raise InvalidMaterials("bundle must contain an inclusion promise")
+        elif bundle.media_type == _BUNDLE_0_2:
+            if not inclusion_proof:
+                raise InvalidMaterials("bundle must contain an inclusion proof")
+            if not inclusion_proof.checkpoint.envelope:
                 raise InvalidMaterials("expected checkpoint in inclusion proof")
 
+        parsed_inclusion_proof: InclusionProof | None = None
+        if (
+            inclusion_proof is not None
+            and inclusion_proof.checkpoint.envelope is not None
+        ):
             parsed_inclusion_proof = LogInclusionProof(
-                checkpoint=checkpoint.envelope,
+                checkpoint=inclusion_proof.checkpoint.envelope,
                 hashes=[h.hex() for h in inclusion_proof.hashes],
                 log_index=inclusion_proof.log_index,
                 root_hash=inclusion_proof.root_hash.hex(),
                 tree_size=inclusion_proof.tree_size,
             )
 
         entry = LogEntry(
@@ -332,28 +363,29 @@
 
         If false, `VerificationMaterials.rekor_entry()` performs an online lookup.
         """
         return self._rekor_entry is not None
 
     def rekor_entry(self, client: RekorClient) -> LogEntry:
         """
-        Returns a `RekorEntry` for the current signing materials.
+        Returns a `LogEntry` for the current signing materials.
         """
 
         # The Rekor entry we use depends on a few different states:
         # 1. If the user has requested offline verification and we've
         #    been given an offline Rekor entry to use, we use it.
         # 2. If the user has not requested offline verification,
         #    we *opportunistically* use the offline Rekor entry,
         #    so long as it contains an inclusion proof. If it doesn't
         #    contain an inclusion proof, then we do an online entry lookup.
         offline = self._offline
         has_rekor_entry = self.has_rekor_entry
         has_inclusion_proof = (
-            self.has_rekor_entry and self._rekor_entry.inclusion_proof is not None  # type: ignore
+            self.has_rekor_entry
+            and self._rekor_entry.inclusion_proof is not None  # type: ignore
         )
 
         entry: LogEntry | None
         if (offline and has_rekor_entry) or (not offline and has_inclusion_proof):
             logger.debug("using offline rekor entry")
             entry = self._rekor_entry
         else:
```

### Comparing `sigstore-2.0.0rc1/sigstore/verify/policy.py` & `sigstore-2.0.0rc2/sigstore/verify/policy.py`

 * *Files identical despite different names*

### Comparing `sigstore-2.0.0rc1/sigstore/verify/verifier.py` & `sigstore-2.0.0rc2/sigstore/verify/verifier.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 from cryptography.x509.oid import ExtendedKeyUsageOID
 from OpenSSL.crypto import (  # type: ignore[import]
     X509,
     X509Store,
     X509StoreContext,
     X509StoreContextError,
 )
+from pydantic import ConfigDict
 
 from sigstore._internal.merkle import (
     InvalidInclusionProofError,
     verify_merkle_inclusion,
 )
 from sigstore._internal.rekor.checkpoint import (
     CheckpointError,
@@ -84,22 +85,21 @@
 
 class CertificateVerificationFailure(VerificationFailure):
     """
     A specialization of `VerificationFailure` for certificate signature
     verification failures, with additional exception context.
     """
 
+    # Needed for the `exception` field above, since exceptions are
+    # not trivially serializable.
+    model_config = ConfigDict(arbitrary_types_allowed=True)
+
     reason: str = "Failed to verify signing certificate"
     exception: Exception
 
-    class Config:
-        # Needed for the `exception` field above, since exceptions are
-        # not trivially serializable.
-        arbitrary_types_allowed = True
-
 
 class Verifier:
     """
     The primary API for verification operations.
     """
 
     def __init__(
@@ -273,18 +273,21 @@
             return VerificationFailure(reason="missing Rekor inclusion proof")
         else:
             logger.warning(
                 "inclusion proof not present in bundle: skipping due to offline verification"
             )
 
         # 6) Verify the Signed Entry Timestamp (SET) supplied by Rekor for this artifact
-        try:
-            verify_set(self._rekor, entry)
-        except InvalidSETError as inval_set:
-            return VerificationFailure(reason=f"invalid Rekor entry SET: {inval_set}")
+        if entry.inclusion_promise:
+            try:
+                verify_set(self._rekor, entry)
+            except InvalidSETError as inval_set:
+                return VerificationFailure(
+                    reason=f"invalid Rekor entry SET: {inval_set}"
+                )
 
         # 7) Verify that the signing certificate was valid at the time of signing
         integrated_time = datetime.datetime.utcfromtimestamp(entry.integrated_time)
         if not (
             materials.certificate.not_valid_before
             <= integrated_time
             <= materials.certificate.not_valid_after
```

### Comparing `sigstore-2.0.0rc1/PKG-INFO` & `sigstore-2.0.0rc2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sigstore
-Version: 2.0.0rc1
+Version: 2.0.0rc2
 Summary: A tool for signing Python package distributions
 Author-email: Sigstore Authors <sigstore-dev@googlegroups.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
@@ -17,31 +17,31 @@
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Security
 Classifier: Topic :: Security :: Cryptography
 Requires-Dist: appdirs ~= 1.4
 Requires-Dist: cryptography >= 39
 Requires-Dist: id >= 1.0.0
 Requires-Dist: importlib_resources ~= 5.7; python_version < '3.11'
-Requires-Dist: pydantic ~= 1.10
+Requires-Dist: pydantic >= 2,< 3
 Requires-Dist: pyjwt >= 2.1
 Requires-Dist: pyOpenSSL >= 23.0.0
 Requires-Dist: requests
 Requires-Dist: securesystemslib
-Requires-Dist: sigstore-protobuf-specs ~= 0.1.0
+Requires-Dist: sigstore-protobuf-specs ~= 0.2.0
 Requires-Dist: tuf >= 2.1,< 4.0
 Requires-Dist: build ; extra == "dev"
 Requires-Dist: bump >= 1.3.2 ; extra == "dev"
 Requires-Dist: sigstore[doc,test,lint] ; extra == "dev"
 Requires-Dist: pdoc ; extra == "doc"
 Requires-Dist: bandit ; extra == "lint"
 Requires-Dist: black ; extra == "lint"
 Requires-Dist: isort ; extra == "lint"
 Requires-Dist: interrogate ; extra == "lint"
 Requires-Dist: mypy ~= 1.1 ; extra == "lint"
-Requires-Dist: ruff < 0.0.275 ; extra == "lint"
+Requires-Dist: ruff < 0.0.279 ; extra == "lint"
 Requires-Dist: types-requests ; extra == "lint"
 Requires-Dist: typing-extensions ; extra == "lint" and ( python_version < '3.8')
 Requires-Dist: pytest ; extra == "test"
 Requires-Dist: pytest-cov ; extra == "test"
 Requires-Dist: pretend ; extra == "test"
 Requires-Dist: coverage[toml] ; extra == "test"
 Project-URL: Documentation, https://sigstore.github.io/sigstore-python/
```

