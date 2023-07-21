# Comparing `tmp/cloudfront_signed_cookies-1.0.tar.gz` & `tmp/cloudfront_signed_cookies-1.2.tar.gz`

## Comparing `cloudfront_signed_cookies-1.0.tar` & `cloudfront_signed_cookies-1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 cloudfront_signed_cookies-1.0/main.py
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 cloudfront_signed_cookies-1.0/requirements.txt
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 cloudfront_signed_cookies-1.0/cloudfront_signed_cookies/__about__.py
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 cloudfront_signed_cookies-1.0/cloudfront_signed_cookies/__init__.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 cloudfront_signed_cookies-1.0/cloudfront_signed_cookies/__main__.py
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 cloudfront_signed_cookies-1.0/cloudfront_signed_cookies/errors.py
--rw-r--r--   0        0        0     9054 2020-02-02 00:00:00.000000 cloudfront_signed_cookies-1.0/cloudfront_signed_cookies/signer.py
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 cloudfront_signed_cookies-1.0/cloudfront_signed_cookies/cli/__init__.py
--rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 cloudfront_signed_cookies-1.0/cloudfront_signed_cookies/cli/genkeys/__init__.py
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 cloudfront_signed_cookies-1.0/cloudfront_signed_cookies/cli/sign/__init__.py
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 cloudfront_signed_cookies-1.0/tests/__init__.py
--rw-r--r--   0        0        0     4648 2020-02-02 00:00:00.000000 cloudfront_signed_cookies-1.0/tests/test_signer.py
--rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 cloudfront_signed_cookies-1.0/.gitignore
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 cloudfront_signed_cookies-1.0/LICENSE.txt
--rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 cloudfront_signed_cookies-1.0/README.md
--rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 cloudfront_signed_cookies-1.0/pyproject.toml
--rw-r--r--   0        0        0     3140 2020-02-02 00:00:00.000000 cloudfront_signed_cookies-1.0/PKG-INFO
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 cloudfront_signed_cookies-1.2/main.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 cloudfront_signed_cookies-1.2/requirements.txt
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 cloudfront_signed_cookies-1.2/cloudfront_signed_cookies/__about__.py
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 cloudfront_signed_cookies-1.2/cloudfront_signed_cookies/__init__.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 cloudfront_signed_cookies-1.2/cloudfront_signed_cookies/__main__.py
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 cloudfront_signed_cookies-1.2/cloudfront_signed_cookies/errors.py
+-rw-r--r--   0        0        0     9693 2020-02-02 00:00:00.000000 cloudfront_signed_cookies-1.2/cloudfront_signed_cookies/signer.py
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 cloudfront_signed_cookies-1.2/cloudfront_signed_cookies/cli/__init__.py
+-rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 cloudfront_signed_cookies-1.2/cloudfront_signed_cookies/cli/genkeys/__init__.py
+-rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 cloudfront_signed_cookies-1.2/cloudfront_signed_cookies/cli/sign/__init__.py
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 cloudfront_signed_cookies-1.2/tests/__init__.py
+-rw-r--r--   0        0        0     4898 2020-02-02 00:00:00.000000 cloudfront_signed_cookies-1.2/tests/test_signer.py
+-rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 cloudfront_signed_cookies-1.2/.gitignore
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 cloudfront_signed_cookies-1.2/LICENSE.txt
+-rw-r--r--   0        0        0     2704 2020-02-02 00:00:00.000000 cloudfront_signed_cookies-1.2/README.md
+-rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 cloudfront_signed_cookies-1.2/pyproject.toml
+-rw-r--r--   0        0        0     3778 2020-02-02 00:00:00.000000 cloudfront_signed_cookies-1.2/PKG-INFO
```

### Comparing `cloudfront_signed_cookies-1.0/main.py` & `cloudfront_signed_cookies-1.2/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from cloudfront_signed_cookies.signer import Signer
 
 if __name__ == "__main__":
     signer = Signer(
         cloudfront_key_id="K36X4X2EO997HM",
-        priv_key_file="./certs/private_key.pem",
+        private_key="./certs/private_key.pem",
     )
 
     cookies: dict = signer.generate_cookies(
         # Resource="https://s3.amazonaws.com/somefile.txt",
         # Policy={},
         Policy={
             "Statement": [
```

### Comparing `cloudfront_signed_cookies-1.0/cloudfront_signed_cookies/signer.py` & `cloudfront_signed_cookies-1.2/cloudfront_signed_cookies/signer.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,39 +7,55 @@
 from cryptography.hazmat.primitives import serialization
 from cryptography.hazmat.primitives import hashes
 from cryptography.hazmat.primitives.asymmetric import padding
 from cloudfront_signed_cookies.errors import (
     InvalidCloudFrontKeyId,
     InvalidCustomPolicy,
     PrivateKeyNotFound,
+    InvalidPrivateKeyFormat,
 )
 
 
 class Signer:
-    def __init__(self, cloudfront_key_id: str, priv_key_file: str) -> None:
+    def __init__(self, cloudfront_key_id: str, private_key: str) -> None:
         """Initializes `Signer` object.
 
         Args:
             cloudfront_key_id(str): the ID assigned to the public key in CloudFront
-            priv_key_file(str): the path to the private PEM-formatted key
+            private_key(str): the path to the private PEM-formatted key
         """
         if not match(r"^[A-Z0-9]{1,}$", cloudfront_key_id):
             raise InvalidCloudFrontKeyId(
                 "CloudFront public key ID must match the following regex: ^[A-Z0-9]{1,}$"
             )
         else:
             self.cloudfront_key_id: str = cloudfront_key_id
-        if exists(priv_key_file):
-            with open(priv_key_file, mode="rb") as priv_file:
+        if exists(private_key):
+            with open(private_key, mode="rb") as priv_file:
                 key_bytes = priv_file.read()
+                try:
+                    self.priv_key = serialization.load_pem_private_key(
+                        key_bytes, password=None
+                    )
+                except ValueError:
+                    raise InvalidPrivateKeyFormat(
+                        "provided private key is not formatted correctly"
+                    )
+        elif type(private_key) is str:
+            key_bytes = bytes(private_key, "utf-8")
+            try:
                 self.priv_key = serialization.load_pem_private_key(
                     key_bytes, password=None
                 )
+            except ValueError:
+                raise InvalidPrivateKeyFormat(
+                    "provided private key is not formatted correctly"
+                )
         else:
-            raise PrivateKeyNotFound(f"{priv_key_file} not found")
+            raise PrivateKeyNotFound(f"{private_key} not found")
 
     def _sign(self, policy: str) -> bytes:
         """Generate signature from policy and the private key associated
         with the public key in the CloudFront trusted key group.
         """
         signature: bytes = self.priv_key.sign(
             data=policy.encode(), padding=padding.PKCS1v15(), algorithm=hashes.SHA1()
```

### Comparing `cloudfront_signed_cookies-1.0/cloudfront_signed_cookies/cli/sign/__init__.py` & `cloudfront_signed_cookies-1.2/cloudfront_signed_cookies/cli/sign/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,18 +16,18 @@
     print(f"--url '{url}'")
 
 
 @click.command(context_settings={"ignore_unknown_options": True})
 @click.option(
     "--priv-key",
     "-p",
-    "priv_key_file",
+    "private_key",
     type=str,
     required=True,
-    help="the path to the private key file",
+    help="the path to the private key file, or raw value of the private key",
 )
 @click.option(
     "--key-id",
     "-k",
     required=True,
     help="the ID assigned to the public key uploaded to CloudFront",
 )
@@ -40,26 +40,26 @@
     "-e",
     default=900,
     help="[optional] numbers of seconds before the URL expires",
 )
 @click.pass_context
 def sign(
     ctx: click.Context,
-    priv_key_file: str,
+    private_key: str,
     key_id: str,
     resource: str,
     policy,
     expires: int,
 ) -> None:
     if ctx.obj["DEBUG"]:
         logging.debug(
-            f"priv_key_file={priv_key_file},"
+            f"private_key={private_key},"
             f"key_id={key_id}, resource={resource}, policy={policy}, expires={expires}"
         )
     if policy:
         policy = loads(policy)
     else:
         policy = {}
     cookies = Signer(
-        cloudfront_key_id=key_id, priv_key_file=priv_key_file
+        cloudfront_key_id=key_id, private_key=private_key
     ).generate_cookies(Resource=resource, Policy=policy, SecondsBeforeExpires=expires)
     create_curl_command(resource, cookies)
```

### Comparing `cloudfront_signed_cookies-1.0/tests/test_signer.py` & `cloudfront_signed_cookies-1.2/tests/test_signer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import pytest
 from datetime import datetime
 from cloudfront_signed_cookies.signer import Signer
 from cloudfront_signed_cookies.errors import (
     InvalidCustomPolicy,
     PrivateKeyNotFound,
+    InvalidPrivateKeyFormat,
     InvalidCloudFrontKeyId,
 )
 
 signer: Signer = Signer(
     cloudfront_key_id="K36X4X2EO997HM",
-    priv_key_file="./certs/private_key.pem",
+    private_key="./certs/private_key.pem",
 )
 
 
 def test_generate_cookies():
     cookies: dict = signer.generate_cookies(
         Resource="https://s3.amazonaws.com/somefile.txt",
         Policy={},
@@ -22,15 +23,15 @@
     assert cookies != {}
 
 
 def test_private_key_file_not_exists():
     with pytest.raises(PrivateKeyNotFound):
         Signer(
             cloudfront_key_id="K2K0M437QMM888",
-            priv_key_file="./certs/file_not_exits.pem",
+            private_key="./certs/file_not_exits.pem",
         )
 
 
 def test_generated_cookies_with_custom_policy():
     signer.generate_cookies(
         Policy={
             "Statement": [
@@ -120,15 +121,15 @@
         )
 
 
 def test_for_invalid_cloudfront_key_id():
     with pytest.raises(InvalidCloudFrontKeyId):
         Signer(
             cloudfront_key_id="134041ajfdfadffljfdsg00",
-            priv_key_file="./certs/private_key.pem",
+            private_key="./certs/private_key.pem",
         )
 
 
 def test_for_invalid_custom_policy_date_range():
     with pytest.raises(InvalidCustomPolicy):
         signer.generate_cookies(
             Policy={
@@ -157,7 +158,15 @@
                             "DateGreaterThan": {"AWS:EpochTime": 1000},
                         },
                     }
                 ]
             },
             SecondsBeforeExpires=600,
         )
+
+
+def test_invalid_pem_key_formatted_file():
+    with pytest.raises(InvalidPrivateKeyFormat):
+        Signer(
+            cloudfront_key_id="K36X4X2EO997HM",
+            private_key="./certs/invalid_private_key.pem",
+        )
```

### Comparing `cloudfront_signed_cookies-1.0/.gitignore` & `cloudfront_signed_cookies-1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `cloudfront_signed_cookies-1.0/LICENSE.txt` & `cloudfront_signed_cookies-1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cloudfront_signed_cookies-1.0/README.md` & `cloudfront_signed_cookies-1.2/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 [![PyPI - Version](https://img.shields.io/pypi/v/cloudfront-signed-cookies.svg)](https://pypi.org/project/cloudfront-signed-cookies)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/cloudfront-signed-cookies.svg)](https://pypi.org/project/cloudfront-signed-cookies)
 [![Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)](https://github.com/pypa/hatch)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 -----
+**IF YOU'RE INTERESTED**, go checkout my [Medium blog post](https://bin3xish477.medium.com/creating-cloudfront-signed-cookies-c51464c84c97) for a deeper dive on what this package is doing and some usage examples.
 
 **Table of Contents**
 
 - [Installation](#installation)
 - [Usage](#usage)
 - [License](#license)
 
@@ -19,19 +20,35 @@
 pip install cloudfront-signed-cookies
 ```
 
 ## Usage
 
 ```python
 from cloudfront_signed_cookies.signer import Signer
+import os
 
 def main():
+    """
+    Method #1
+    Allow the signer to read your key from a file
+    """
     signer: Signer = Signer(
         cloudfront_key_id="K36X4X2EO997HM",
-        priv_key_file="./certs/private_key.pem",
+        private_key="./certs/private_key.pem",
+    )
+
+    """
+    Method #2
+    Alternatively you can pass the raw contents of the key in from
+    something such as an environment variable, for container (Docker)
+    based usage
+    """
+    signer: Signer = Signer(
+        cloudfront_key_id="K36X4X2EO997HM",
+        private_key=os.environ.get("PRIVATE_KEY")
     )
 
     cookies: dict = signer.generate_cookies(
         Policy={
             "Statement": [
                 {
                     "Resource": "https://domain.com/somefile.txt",
```

### Comparing `cloudfront_signed_cookies-1.0/pyproject.toml` & `cloudfront_signed_cookies-1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cloudfront_signed_cookies-1.0/PKG-INFO` & `cloudfront_signed_cookies-1.2/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: cloudfront-signed-cookies
-Version: 1.0
+Version: 1.2
 Summary: A Python package for controlling access to content sitting behind a CloudFront distribution using signed cookies.
 Project-URL: Documentation, https://github.com/unknown/cloudfront-signed-cookies#readme
 Project-URL: Source, https://github.com/bin3xish477/cloudfront-signed-cookies
 Author-email: Alexis Rodriguez <arodriguez99@protonmail.com>
+License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -24,14 +25,15 @@
 
 [![PyPI - Version](https://img.shields.io/pypi/v/cloudfront-signed-cookies.svg)](https://pypi.org/project/cloudfront-signed-cookies)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/cloudfront-signed-cookies.svg)](https://pypi.org/project/cloudfront-signed-cookies)
 [![Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)](https://github.com/pypa/hatch)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 -----
+**IF YOU'RE INTERESTED**, go checkout my [Medium blog post](https://bin3xish477.medium.com/creating-cloudfront-signed-cookies-c51464c84c97) for a deeper dive on what this package is doing and some usage examples.
 
 **Table of Contents**
 
 - [Installation](#installation)
 - [Usage](#usage)
 - [License](#license)
 
@@ -41,19 +43,35 @@
 pip install cloudfront-signed-cookies
 ```
 
 ## Usage
 
 ```python
 from cloudfront_signed_cookies.signer import Signer
+import os
 
 def main():
+    """
+    Method #1
+    Allow the signer to read your key from a file
+    """
     signer: Signer = Signer(
         cloudfront_key_id="K36X4X2EO997HM",
-        priv_key_file="./certs/private_key.pem",
+        private_key="./certs/private_key.pem",
+    )
+
+    """
+    Method #2
+    Alternatively you can pass the raw contents of the key in from
+    something such as an environment variable, for container (Docker)
+    based usage
+    """
+    signer: Signer = Signer(
+        cloudfront_key_id="K36X4X2EO997HM",
+        private_key=os.environ.get("PRIVATE_KEY")
     )
 
     cookies: dict = signer.generate_cookies(
         Policy={
             "Statement": [
                 {
                     "Resource": "https://domain.com/somefile.txt",
```

