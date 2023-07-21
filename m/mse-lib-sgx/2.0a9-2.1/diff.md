# Comparing `tmp/mse_lib_sgx-2.0a9.tar.gz` & `tmp/mse_lib_sgx-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mse_lib_sgx-2.0a9.tar", last modified: Mon May 22 09:01:46 2023, max compression
+gzip compressed data, was "mse_lib_sgx-2.1.tar", last modified: Fri Jul 21 08:22:29 2023, max compression
```

## Comparing `mse_lib_sgx-2.0a9.tar` & `mse_lib_sgx-2.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 09:01:46.084179 mse_lib_sgx-2.0a9/
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-05-22 09:01:46.084179 mse_lib_sgx-2.0a9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-05-22 09:00:53.000000 mse_lib_sgx-2.0a9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-22 09:01:46.084179 mse_lib_sgx-2.0a9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-05-22 09:00:53.000000 mse_lib_sgx-2.0a9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 09:01:46.080179 mse_lib_sgx-2.0a9/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 09:01:46.080179 mse_lib_sgx-2.0a9/src/mse_lib_sgx/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-22 09:00:53.000000 mse_lib_sgx-2.0a9/src/mse_lib_sgx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-22 09:00:53.000000 mse_lib_sgx-2.0a9/src/mse_lib_sgx/base64url.py
--rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-05-22 09:00:53.000000 mse_lib_sgx-2.0a9/src/mse_lib_sgx/certificate.py
--rw-r--r--   0 runner    (1001) docker     (123)     8627 2023-05-22 09:00:53.000000 mse_lib_sgx-2.0a9/src/mse_lib_sgx/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-22 09:00:53.000000 mse_lib_sgx-2.0a9/src/mse_lib_sgx/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-22 09:00:53.000000 mse_lib_sgx-2.0a9/src/mse_lib_sgx/globs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4586 2023-05-22 09:00:53.000000 mse_lib_sgx-2.0a9/src/mse_lib_sgx/http_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-05-22 09:00:53.000000 mse_lib_sgx-2.0a9/src/mse_lib_sgx/import_hook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 09:01:46.080179 mse_lib_sgx-2.0a9/src/mse_lib_sgx/sgx/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-22 09:00:53.000000 mse_lib_sgx-2.0a9/src/mse_lib_sgx/sgx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-22 09:00:53.000000 mse_lib_sgx-2.0a9/src/mse_lib_sgx/sgx/key.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-22 09:00:53.000000 mse_lib_sgx-2.0a9/src/mse_lib_sgx/sgx/quote.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 09:01:46.080179 mse_lib_sgx-2.0a9/src/mse_lib_sgx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-05-22 09:01:46.000000 mse_lib_sgx-2.0a9/src/mse_lib_sgx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-22 09:01:46.000000 mse_lib_sgx-2.0a9/src/mse_lib_sgx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 09:01:46.000000 mse_lib_sgx-2.0a9/src/mse_lib_sgx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-22 09:01:46.000000 mse_lib_sgx-2.0a9/src/mse_lib_sgx.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 09:01:45.000000 mse_lib_sgx-2.0a9/src/mse_lib_sgx.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-22 09:01:46.000000 mse_lib_sgx-2.0a9/src/mse_lib_sgx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-22 09:01:46.000000 mse_lib_sgx-2.0a9/src/mse_lib_sgx.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 09:01:46.084179 mse_lib_sgx-2.0a9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-05-22 09:00:53.000000 mse_lib_sgx-2.0a9/tests/test_cert_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-05-22 09:00:53.000000 mse_lib_sgx-2.0a9/tests/test_conf_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:22:29.841664 mse_lib_sgx-2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-07-21 08:22:29.841664 mse_lib_sgx-2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-07-21 08:21:43.000000 mse_lib_sgx-2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-21 08:22:29.841664 mse_lib_sgx-2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-07-21 08:21:43.000000 mse_lib_sgx-2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:22:29.837664 mse_lib_sgx-2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:22:29.841664 mse_lib_sgx-2.1/src/mse_lib_sgx/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-21 08:21:43.000000 mse_lib_sgx-2.1/src/mse_lib_sgx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-21 08:21:43.000000 mse_lib_sgx-2.1/src/mse_lib_sgx/base64url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-07-21 08:21:43.000000 mse_lib_sgx-2.1/src/mse_lib_sgx/certificate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8874 2023-07-21 08:21:43.000000 mse_lib_sgx-2.1/src/mse_lib_sgx/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-07-21 08:21:43.000000 mse_lib_sgx-2.1/src/mse_lib_sgx/copy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-07-21 08:21:43.000000 mse_lib_sgx-2.1/src/mse_lib_sgx/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-07-21 08:21:43.000000 mse_lib_sgx-2.1/src/mse_lib_sgx/globs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4592 2023-07-21 08:21:43.000000 mse_lib_sgx-2.1/src/mse_lib_sgx/http_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:22:29.841664 mse_lib_sgx-2.1/src/mse_lib_sgx/sgx/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-21 08:21:43.000000 mse_lib_sgx-2.1/src/mse_lib_sgx/sgx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-21 08:21:43.000000 mse_lib_sgx-2.1/src/mse_lib_sgx/sgx/key.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-21 08:21:43.000000 mse_lib_sgx-2.1/src/mse_lib_sgx/sgx/quote.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:22:29.841664 mse_lib_sgx-2.1/src/mse_lib_sgx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-07-21 08:22:29.000000 mse_lib_sgx-2.1/src/mse_lib_sgx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-07-21 08:22:29.000000 mse_lib_sgx-2.1/src/mse_lib_sgx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 08:22:29.000000 mse_lib_sgx-2.1/src/mse_lib_sgx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-21 08:22:29.000000 mse_lib_sgx-2.1/src/mse_lib_sgx.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 08:22:29.000000 mse_lib_sgx-2.1/src/mse_lib_sgx.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-21 08:22:29.000000 mse_lib_sgx-2.1/src/mse_lib_sgx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-21 08:22:29.000000 mse_lib_sgx-2.1/src/mse_lib_sgx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:22:29.841664 mse_lib_sgx-2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-07-21 08:21:43.000000 mse_lib_sgx-2.1/tests/test_cert_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-07-21 08:21:43.000000 mse_lib_sgx-2.1/tests/test_conf_server.py
```

### Comparing `mse_lib_sgx-2.0a9/PKG-INFO` & `mse_lib_sgx-2.1/src/mse_lib_sgx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: mse_lib_sgx
-Version: 2.0a9
+Name: mse-lib-sgx
+Version: 2.1
 Summary: Library for Cosmian MSE to bootstrap Flask application
 Home-page: https://cosmian.com
 Author: Cosmian Tech
 Author-email: tech@cosmian.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mse_lib_sgx-2.0a9/README.md` & `mse_lib_sgx-2.1/README.md`

 * *Files identical despite different names*

### Comparing `mse_lib_sgx-2.0a9/setup.py` & `mse_lib_sgx-2.1/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -29,19 +29,19 @@
     description="Library for Cosmian MSE to bootstrap Flask application",
     packages=find_packages("src"),
     package_dir={"": "src"},
     long_description=Path("README.md").read_text(),
     long_description_content_type="text/markdown",
     zip_safe=False,
     install_requires=[
-        "cryptography>=40.0.2,<40.1.0",
-        "intel-sgx-ra==2.0a3",
+        "cryptography>=41.0.1,<42.0.0",
+        "intel-sgx-ra>=2.0,<3.0",
         "hypercorn[uvloop]>=0.14.3,<0.15.0",
         "h2>=4.1.0,<4.2.0",
-        "mse-lib-crypto>=1.2,<2.0",
+        "mse-lib-crypto>=1.3,<2.0",
     ],
     entry_points={
         "console_scripts": ["mse-bootstrap = mse_lib_sgx.cli:run"],
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
```

### Comparing `mse_lib_sgx-2.0a9/src/mse_lib_sgx/base64url.py` & `mse_lib_sgx-2.1/src/mse_lib_sgx/base64url.py`

 * *Files identical despite different names*

### Comparing `mse_lib_sgx-2.0a9/src/mse_lib_sgx/certificate.py` & `mse_lib_sgx-2.1/src/mse_lib_sgx/certificate.py`

 * *Files identical despite different names*

### Comparing `mse_lib_sgx-2.0a9/src/mse_lib_sgx/cli.py` & `mse_lib_sgx-2.1/src/mse_lib_sgx/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from hypercorn.asyncio import serve
 from hypercorn.config import Config
 from mse_lib_crypto.x25519 import x25519_pk_from_sk
 from mse_lib_crypto.xsalsa20_poly1305 import decrypt_directory
 
 from mse_lib_sgx import __version__, globs
 from mse_lib_sgx.certificate import Certificate
+from mse_lib_sgx.copy import copytree
 from mse_lib_sgx.error import SecurityError
 from mse_lib_sgx.http_server import serve as serve_sgx_secrets
 from mse_lib_sgx.sgx.key import get_mrenclave_key
 
 
 def parse_args() -> argparse.Namespace:
     """Argument parser."""
@@ -127,24 +128,20 @@
     - (--no-ssl) If the app owner and the users trust the operator (cosmian)
       then don't use https connection.
     """
     args: argparse.Namespace = parse_args()
 
     globs.HOME_DIR_PATH.mkdir(exist_ok=True)
     globs.KEY_DIR_PATH.mkdir(exist_ok=True)
-    globs.MODULE_DIR_PATH.mkdir(exist_ok=True)
 
     logging.basicConfig(
         level=logging.DEBUG if args.debug else logging.INFO,
         format="[%(asctime)s] [%(levelname)s] %(message)s",
     )
 
-    if args.plaincode:
-        globs.PLAINCODE = True
-
     if args.timeout:
         globs.TIMEOUT = args.timeout
 
     ssl_private_key_path = None
     expiration_date = datetime.now() + timedelta(hours=10)
 
     ssl_app_mode: SslAppMode
@@ -160,77 +157,83 @@
     else:
         # The conf server and the app server will use the same self-signed cert
         ssl_app_mode = SslAppMode.RATLS_CERTIFICATE
         expiration_date = datetime.utcfromtimestamp(args.ratls)
 
     logging.info("Generating self-signed certificate...")
 
+    enclave_sk: bytes
+    enclave_pk: bytes
     if not globs.ENCLAVE_SK_PATH.exists():
-        globs.ENCLAVE_SK_PATH.write_bytes(get_mrenclave_key())
+        enclave_sk = get_mrenclave_key()
+        globs.ENCLAVE_SK_PATH.write_bytes(enclave_sk)
+        enclave_pk = x25519_pk_from_sk(globs.ENCLAVE_SK_PATH.read_bytes())
+
+        if len(enclave_pk) != 32:
+            raise SecurityError("Bad enclave pk length!")
 
-    enclave_pk: bytes = x25519_pk_from_sk(globs.ENCLAVE_SK_PATH.read_bytes())
+        globs.ENCLAVE_PK_PATH.write_bytes(enclave_pk)
+    else:
+        enclave_sk = globs.ENCLAVE_SK_PATH.read_bytes()
+        enclave_pk = globs.ENCLAVE_PK_PATH.read_bytes()
 
-    if len(enclave_pk) != 32:
-        raise SecurityError("Bad enclave pk length!")
+        if len(enclave_sk) != 32:
+            raise SecurityError("Bad enclave sk length!")
+
+        if x25519_pk_from_sk(enclave_sk) != enclave_pk:
+            raise SecurityError("Malformed enclave's keypair!")
 
     cert: Certificate = Certificate(
         subject_alternative_name=args.san if args.san else "localhost",
         subject=(
             x509.Name.from_rfc4514_string(args.subject)
             if args.subject
             else globs.SUBJECT
         ),
         root_path=globs.KEY_DIR_PATH,
         expiration_date=expiration_date,
         ratls=enclave_pk,
     )
 
-    if not globs.CODE_KEY_PATH.exists():
+    if not globs.MODULE_DIR_PATH.exists():
         logging.info("Starting the configuration server...")
         # The app owner will send:
         # - the uuid of the app (see as an uniq token allowing to query the API)
         # - the key to decrypt the code
         # - (optional) the SSL private key if AppConnection.OWNER_CERTFICIATE
         serve_sgx_secrets(
             hostname=args.host,
             port=args.port,
             certificate=cert,
             app_id=args.id,
             need_ssl_private_key=ssl_app_mode == SslAppMode.CUSTOM_CERTIFICATE,
             timeout=globs.TIMEOUT,
         )
 
-        if not globs.PLAINCODE and globs.CODE_SECRET_KEY is None:
-            raise SecurityError("Code secret key not provided")
-
-        if not globs.PLAINCODE and globs.CODE_SECRET_KEY is not None:
+        if globs.CODE_SECRET_KEY is not None:
             globs.CODE_KEY_PATH.write_bytes(globs.CODE_SECRET_KEY)
+            globs.MODULE_DIR_PATH.mkdir()
+            decrypt_directory(
+                dir_path=args.app_dir,
+                key=globs.CODE_KEY_PATH.read_bytes(),
+                ext=".enc",
+                out_dir_path=globs.MODULE_DIR_PATH,
+            )
+        else:
+            copytree(
+                src=args.app_dir, dst=globs.MODULE_DIR_PATH, copy_function=shutil.copy
+            )
 
         if (
             ssl_app_mode == SslAppMode.CUSTOM_CERTIFICATE
             and globs.SSL_PRIVATE_KEY
             and ssl_private_key_path is not None
         ):
             ssl_private_key_path.write_text(globs.SSL_PRIVATE_KEY)
 
-    if globs.PLAINCODE:
-        shutil.copytree(
-            src=args.app_dir,
-            dst=globs.MODULE_DIR_PATH,
-            copy_function=shutil.copy,
-            dirs_exist_ok=True,
-        )
-    else:
-        decrypt_directory(
-            dir_path=args.app_dir,
-            key=globs.CODE_KEY_PATH.read_bytes(),
-            ext=".enc",
-            out_dir_path=globs.MODULE_DIR_PATH,
-        )
-
     config_map = {
         "bind": f"{args.host}:{args.port}",
         "alpn_protocols": ["h2"],
         "workers": 1,
         "accesslog": "-",
         "errorlog": "-",
         "worker_class": "uvloop",
```

### Comparing `mse_lib_sgx-2.0a9/src/mse_lib_sgx/globs.py` & `mse_lib_sgx-2.1/src/mse_lib_sgx/globs.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,26 +13,26 @@
 
 EXIT_EVENT: threading.Event = threading.Event()
 
 ID: Optional[UUID] = None
 
 SSL_PRIVATE_KEY: Optional[str] = None
 NEED_SSL_PRIVATE_KEY: bool = False
-PLAINCODE: bool = False
 
 HOME_DIR_PATH: Path = Path(os.getenv("HOME", "/root"))
 KEY_DIR_PATH: Path = Path(os.getenv("KEY_PATH", "/key"))
 SECRETS_PATH: Path = Path(os.getenv("SECRETS_PATH", "/root/.cache/mse/secrets.json"))
 SEALED_SECRETS_PATH: Path = Path(
     os.getenv("SEALED_SECRETS_PATH", "/root/.cache/mse/sealed_secrets.json")
 )
 MODULE_DIR_PATH: Path = Path(os.getenv("MODULE_PATH", "/mse-app"))
 
 CODE_KEY_PATH: Path = KEY_DIR_PATH / "code.key"
 ENCLAVE_SK_PATH: Path = KEY_DIR_PATH / "enclave.key"
+ENCLAVE_PK_PATH: Path = KEY_DIR_PATH / "enclave.pub"
 
 SUBJECT: x509.Name = x509.Name(
     [
         x509.NameAttribute(NameOID.COUNTRY_NAME, "FR"),
         x509.NameAttribute(NameOID.STATE_OR_PROVINCE_NAME, "Ile-de-France"),
         x509.NameAttribute(NameOID.LOCALITY_NAME, "Paris"),
         x509.NameAttribute(NameOID.ORGANIZATION_NAME, "Cosmian Tech"),
```

### Comparing `mse_lib_sgx-2.0a9/src/mse_lib_sgx/http_server.py` & `mse_lib_sgx-2.1/src/mse_lib_sgx/http_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,15 @@
                 self.send_response_only(401)
                 self.end_headers()
                 return
 
             if globs.NEED_SSL_PRIVATE_KEY:
                 globs.SSL_PRIVATE_KEY = data["ssl_private_key"]
 
-            if not globs.PLAINCODE:
+            if "code_secret_key" in data:
                 globs.CODE_SECRET_KEY = bytes.fromhex(data["code_secret_key"])
 
                 if len(globs.CODE_SECRET_KEY) != 32:
                     raise CryptoError("Incorrect key length!")
         # might be: KeyError, ValueError, json.JSONDecodeError, CryptoError
         except Exception as exc:  # pylint: disable=broad-exception-caught
             logging.error(exc)
```

### Comparing `mse_lib_sgx-2.0a9/src/mse_lib_sgx/sgx/key.py` & `mse_lib_sgx-2.1/src/mse_lib_sgx/sgx/key.py`

 * *Files identical despite different names*

### Comparing `mse_lib_sgx-2.0a9/src/mse_lib_sgx/sgx/quote.py` & `mse_lib_sgx-2.1/src/mse_lib_sgx/sgx/quote.py`

 * *Files identical despite different names*

### Comparing `mse_lib_sgx-2.0a9/src/mse_lib_sgx.egg-info/PKG-INFO` & `mse_lib_sgx-2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: mse-lib-sgx
-Version: 2.0a9
+Name: mse_lib_sgx
+Version: 2.1
 Summary: Library for Cosmian MSE to bootstrap Flask application
 Home-page: https://cosmian.com
 Author: Cosmian Tech
 Author-email: tech@cosmian.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mse_lib_sgx-2.0a9/src/mse_lib_sgx.egg-info/SOURCES.txt` & `mse_lib_sgx-2.1/src/mse_lib_sgx.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 README.md
 setup.cfg
 setup.py
 src/mse_lib_sgx/__init__.py
 src/mse_lib_sgx/base64url.py
 src/mse_lib_sgx/certificate.py
 src/mse_lib_sgx/cli.py
+src/mse_lib_sgx/copy.py
 src/mse_lib_sgx/error.py
 src/mse_lib_sgx/globs.py
 src/mse_lib_sgx/http_server.py
-src/mse_lib_sgx/import_hook.py
 src/mse_lib_sgx.egg-info/PKG-INFO
 src/mse_lib_sgx.egg-info/SOURCES.txt
 src/mse_lib_sgx.egg-info/dependency_links.txt
 src/mse_lib_sgx.egg-info/entry_points.txt
 src/mse_lib_sgx.egg-info/not-zip-safe
 src/mse_lib_sgx.egg-info/requires.txt
 src/mse_lib_sgx.egg-info/top_level.txt
```

### Comparing `mse_lib_sgx-2.0a9/tests/test_cert_utils.py` & `mse_lib_sgx-2.1/tests/test_cert_utils.py`

 * *Files identical despite different names*

### Comparing `mse_lib_sgx-2.0a9/tests/test_conf_server.py` & `mse_lib_sgx-2.1/tests/test_conf_server.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,36 +30,14 @@
     ctx.check_hostname = False
     ctx.verify_mode = ssl.CERT_NONE
 
     with pytest.raises(urllib.error.HTTPError):
         urllib.request.urlopen(req, data, context=ctx)
 
 
-def test_no_secret_key(
-    set_env,
-    uuid,
-    host,
-    port,
-    conf_server,
-):
-    assert conf_server.is_alive()
-
-    req = urllib.request.Request(
-        url=f"https://{host}:{port}", headers={"Content-Type": "application/json"}
-    )
-    data: bytes = json.dumps({"uuid": str(uuid)}).encode("utf-8")
-    req.add_header("Content-Length", str(len(data)))
-    ctx = ssl.create_default_context()
-    ctx.check_hostname = False
-    ctx.verify_mode = ssl.CERT_NONE
-
-    with pytest.raises(urllib.error.HTTPError):
-        urllib.request.urlopen(req, data, context=ctx)
-
-
 def test_no_uuid(
     set_env,
     code_secret_key,
     host,
     port,
     conf_server,
 ):
```

