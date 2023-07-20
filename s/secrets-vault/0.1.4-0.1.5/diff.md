# Comparing `tmp/secrets-vault-0.1.4.tar.gz` & `tmp/secrets-vault-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secrets-vault-0.1.4.tar", last modified: Thu Jul 20 15:57:34 2023, max compression
+gzip compressed data, was "secrets-vault-0.1.5.tar", last modified: Thu Jul 20 22:22:23 2023, max compression
```

## Comparing `secrets-vault-0.1.4.tar` & `secrets-vault-0.1.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:57:34.404354 secrets-vault-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-20 15:57:09.000000 secrets-vault-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-07-20 15:57:34.404354 secrets-vault-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-07-20 15:57:09.000000 secrets-vault-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:57:34.400354 secrets-vault-0.1.4/secrets_vault/
--rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-07-20 15:57:09.000000 secrets-vault-0.1.4/secrets_vault/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-07-20 15:57:09.000000 secrets-vault-0.1.4/secrets_vault/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-20 15:57:09.000000 secrets-vault-0.1.4/secrets_vault/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-20 15:57:09.000000 secrets-vault-0.1.4/secrets_vault/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:57:34.400354 secrets-vault-0.1.4/secrets_vault.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-07-20 15:57:34.000000 secrets-vault-0.1.4/secrets_vault.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-20 15:57:34.000000 secrets-vault-0.1.4/secrets_vault.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 15:57:34.000000 secrets-vault-0.1.4/secrets_vault.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-20 15:57:34.000000 secrets-vault-0.1.4/secrets_vault.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-20 15:57:34.000000 secrets-vault-0.1.4/secrets_vault.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 15:57:34.404354 secrets-vault-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-07-20 15:57:09.000000 secrets-vault-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:57:34.400354 secrets-vault-0.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-07-20 15:57:09.000000 secrets-vault-0.1.4/tests/test_e2e.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:22:23.908959 secrets-vault-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-20 22:22:05.000000 secrets-vault-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5600 2023-07-20 22:22:23.908959 secrets-vault-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5102 2023-07-20 22:22:05.000000 secrets-vault-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:22:23.904959 secrets-vault-0.1.5/secrets_vault/
+-rw-r--r--   0 runner    (1001) docker     (123)     4218 2023-07-20 22:22:05.000000 secrets-vault-0.1.5/secrets_vault/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-07-20 22:22:05.000000 secrets-vault-0.1.5/secrets_vault/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-20 22:22:05.000000 secrets-vault-0.1.5/secrets_vault/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-20 22:22:05.000000 secrets-vault-0.1.5/secrets_vault/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:22:23.908959 secrets-vault-0.1.5/secrets_vault.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5600 2023-07-20 22:22:23.000000 secrets-vault-0.1.5/secrets_vault.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-20 22:22:23.000000 secrets-vault-0.1.5/secrets_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 22:22:23.000000 secrets-vault-0.1.5/secrets_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-20 22:22:23.000000 secrets-vault-0.1.5/secrets_vault.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-20 22:22:23.000000 secrets-vault-0.1.5/secrets_vault.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 22:22:23.908959 secrets-vault-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-07-20 22:22:05.000000 secrets-vault-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:22:23.908959 secrets-vault-0.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-07-20 22:22:05.000000 secrets-vault-0.1.5/tests/test_e2e.py
```

### Comparing `secrets-vault-0.1.4/LICENSE` & `secrets-vault-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `secrets-vault-0.1.4/secrets_vault/__init__.py` & `secrets-vault-0.1.5/secrets_vault/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
             self.secrets_filename = secrets_filepath
             self.secrets = dict()
             self._load_secrets()
         except InvalidToken:
             raise MasterKeyInvalid("Master key is malformed or invalid")
 
     @staticmethod
-    def init(
+    def create(
         secrets_filepath=DEFAULT_SECRETS_FILEPATH,
         master_key_filepath=DEFAULT_MASTER_KEY_FILEPATH,
     ):
         """
         Create a new secrets file and returns the master key - keep it safe!
         """
         if Path(secrets_filepath).exists():
@@ -55,15 +55,15 @@
         master_key = Fernet.generate_key().decode()
         with open(master_key_filepath, "w") as fout:
             fout.write(master_key)
 
         vault = SecretsVault(master_key, secrets_filepath)
         vault.set("my-user", "foo")
         vault.set("my-password", "supersecret")
-        vault.persist()
+        vault.save()
 
         return vault, master_key
 
     def require(self, key):
         return self.secrets[key]
 
     def get(self, key, default=None):
@@ -89,17 +89,17 @@
             tf.seek(0)
             newsecrets = json.loads(tf.read())
 
         if self.secrets == newsecrets:
             log.info("No changes applied")
             return
         self.secrets = newsecrets
-        self.persist()
+        self.save()
 
-    def persist(self):
+    def save(self):
         with open(self.secrets_filename, "wb") as fout:
             fout.write(self.fernet.encrypt(self._serialize()))
         log.info(f"Wrote encrypted secrets to {self.secrets_filename}")
 
     @staticmethod
     def _load_master_key(master_key_filepath=None):
         master_key = os.environ.get("MASTER_KEY")
```

### Comparing `secrets-vault-0.1.4/setup.py` & `secrets-vault-0.1.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 HERE = pathlib.Path(__file__).parent
 README = (HERE / "README.md").read_text()
 
 
 setup(
     name="secrets-vault",
-    version="0.1.4",
+    version="0.1.5",
     author="Anthony N. Simon",
     url="https://github.com/anthonynsimon/secrets-vault",
     description="Simple encrypted secrets for Python",
     long_description=README,
     long_description_content_type="text/markdown",
     license="MIT",
     classifiers=[
@@ -25,13 +25,13 @@
         "Programming Language :: Python :: 3.9",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
     packages=find_packages(exclude=["tests"]),
     include_package_data=True,
     entry_points={
         "console_scripts": [
-            "secrets-vault=secrets_vault.__main__:main",
-            "secrets=secrets_vault.__main__:main",
+            "secrets-vault=secrets_vault.__main__:cli",
+            "secrets=secrets_vault.__main__:cli",
         ]
     },
     tests_require=[],
 )
```

### Comparing `secrets-vault-0.1.4/tests/test_e2e.py` & `secrets-vault-0.1.5/tests/test_e2e.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 
 from secrets_vault import SecretsVault, exceptions
 
 BASE_DIR = Path(__file__).parent
 TEST_DATA_DIR = BASE_DIR / "test-data"
 
 
-def test_init():
-    vault, master_key = SecretsVault.init(
+def test_create():
+    vault, master_key = SecretsVault.create(
         secrets_filepath=TEST_DATA_DIR / "secrets-1.json.enc",
         master_key_filepath=TEST_DATA_DIR / "master-1.key",
     )
 
     assert os.path.exists(TEST_DATA_DIR / "secrets-1.json.enc")
     assert os.path.exists(TEST_DATA_DIR / "master-1.key")
     assert master_key is not None and len(master_key) == 44
@@ -23,47 +23,67 @@
         secrets_filepath=TEST_DATA_DIR / "secrets-1.json.enc",
         master_key_filepath=TEST_DATA_DIR / "master-1.key",
     )
     assert vault.get("my-password") == "supersecret"
 
 
 def test_requires_master_key():
-    SecretsVault.init(
+    SecretsVault.create(
         secrets_filepath=TEST_DATA_DIR / "secrets-2.json.enc",
         master_key_filepath=TEST_DATA_DIR / "master-2.key",
     )
 
     try:
         SecretsVault(
             secrets_filepath=TEST_DATA_DIR / "secrets-2.json.enc",
             master_key_filepath=TEST_DATA_DIR / "master-456.key",
         )
         assert False, "Should throw"
     except Exception as e:
         assert isinstance(e, exceptions.MasterKeyNotFound)
 
 
+def test_provides_master_key_via_env_var():
+    SecretsVault.create(
+        secrets_filepath=TEST_DATA_DIR / "secrets-2a.json.enc",
+        master_key_filepath=TEST_DATA_DIR / "master-2a.key",
+    )
+
+    with open(TEST_DATA_DIR / "master-2a.key", "rb") as fin:
+        master_key = fin.read().decode()
+        os.environ["MASTER_KEY"] = master_key
+
+    vault = SecretsVault(
+        secrets_filepath=TEST_DATA_DIR / "secrets-2a.json.enc",
+        master_key_filepath=None,
+    )
+    assert vault.get("my-password") == "supersecret"
+
+    # Cleanup to not affect other tests
+    del os.environ["MASTER_KEY"]
+
+
 def test_requires_secrets_file():
-    SecretsVault.init(
+    SecretsVault.create(
         secrets_filepath=TEST_DATA_DIR / "secrets-3.json.enc",
         master_key_filepath=TEST_DATA_DIR / "master-3.key",
     )
 
     try:
-        vault = SecretsVault(
+        SecretsVault(
             secrets_filepath=TEST_DATA_DIR / "secrets-456.json.enc",
             master_key_filepath=TEST_DATA_DIR / "master-3.key",
         )
         assert False, "Should throw"
     except Exception as e:
         assert isinstance(e, exceptions.SecretsFileNotFound)
 
 
-def test_persist():
-    SecretsVault.init(
+def test_save():
+    SecretsVault.create(
         secrets_filepath=TEST_DATA_DIR / "secrets-4.json.enc",
         master_key_filepath=TEST_DATA_DIR / "master-4.key",
     )
 
     vault = SecretsVault(
         secrets_filepath=TEST_DATA_DIR / "secrets-4.json.enc",
         master_key_filepath=TEST_DATA_DIR / "master-4.key",
@@ -71,41 +91,41 @@
 
     assert vault.get("my-password") == "supersecret"
     assert vault.get("hello") is None
     assert vault.get("nested") is None
 
     vault.set("hello", "world")
     vault.set("nested", {"object": "value"})
-    vault.persist()
+    vault.save()
 
     assert vault.get("hello") == "world"
     assert vault.get("nested") == {"object": "value"}
 
 
 def test_large_secrets_file():
-    SecretsVault.init(
+    SecretsVault.create(
         secrets_filepath=TEST_DATA_DIR / "secrets-5.json.enc",
         master_key_filepath=TEST_DATA_DIR / "master-5.key",
     )
 
     vault = SecretsVault(
         secrets_filepath=TEST_DATA_DIR / "secrets-5.json.enc",
         master_key_filepath=TEST_DATA_DIR / "master-5.key",
     )
 
     for i in range(10000):
         vault.set(f"key-{i}", f"value-{i}")
-    vault.persist()
+    vault.save()
 
     for i in range(10000):
         assert vault.get(f"key-{i}") == f"value-{i}"
 
 
 def test_wrong_key():
-    SecretsVault.init(
+    SecretsVault.create(
         secrets_filepath=TEST_DATA_DIR / "secrets-6.json.enc",
         master_key_filepath=TEST_DATA_DIR / "master-6.key",
     )
 
     try:
         SecretsVault(
             secrets_filepath=TEST_DATA_DIR / "secrets-6.json.enc",
```

