# Comparing `tmp/secrets-vault-0.1.8.tar.gz` & `tmp/secrets-vault-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secrets-vault-0.1.8.tar", last modified: Thu Jul 20 23:26:36 2023, max compression
+gzip compressed data, was "secrets-vault-0.1.9.tar", last modified: Fri Jul 21 14:45:22 2023, max compression
```

## Comparing `secrets-vault-0.1.8.tar` & `secrets-vault-0.1.9.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 23:26:36.625046 secrets-vault-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-20 23:26:11.000000 secrets-vault-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-07-20 23:26:36.625046 secrets-vault-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-07-20 23:26:11.000000 secrets-vault-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 23:26:36.621046 secrets-vault-0.1.8/secrets_vault/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-20 23:26:11.000000 secrets-vault-0.1.8/secrets_vault/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-07-20 23:26:11.000000 secrets-vault-0.1.8/secrets_vault/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-20 23:26:11.000000 secrets-vault-0.1.8/secrets_vault/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-20 23:26:11.000000 secrets-vault-0.1.8/secrets_vault/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4367 2023-07-20 23:26:11.000000 secrets-vault-0.1.8/secrets_vault/vault.py
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-20 23:26:11.000000 secrets-vault-0.1.8/secrets_vault/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 23:26:36.625046 secrets-vault-0.1.8/secrets_vault.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-07-20 23:26:36.000000 secrets-vault-0.1.8/secrets_vault.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-07-20 23:26:36.000000 secrets-vault-0.1.8/secrets_vault.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 23:26:36.000000 secrets-vault-0.1.8/secrets_vault.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-20 23:26:36.000000 secrets-vault-0.1.8/secrets_vault.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-20 23:26:36.000000 secrets-vault-0.1.8/secrets_vault.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-20 23:26:36.000000 secrets-vault-0.1.8/secrets_vault.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 23:26:36.625046 secrets-vault-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-07-20 23:26:11.000000 secrets-vault-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 23:26:36.625046 secrets-vault-0.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-07-20 23:26:11.000000 secrets-vault-0.1.8/tests/test_e2e.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:45:22.294222 secrets-vault-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-21 14:44:55.000000 secrets-vault-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6260 2023-07-21 14:45:22.294222 secrets-vault-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5762 2023-07-21 14:44:55.000000 secrets-vault-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:45:22.294222 secrets-vault-0.1.9/secrets_vault/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-21 14:44:55.000000 secrets-vault-0.1.9/secrets_vault/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-07-21 14:44:55.000000 secrets-vault-0.1.9/secrets_vault/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-07-21 14:44:55.000000 secrets-vault-0.1.9/secrets_vault/backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-21 14:44:55.000000 secrets-vault-0.1.9/secrets_vault/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-21 14:44:55.000000 secrets-vault-0.1.9/secrets_vault/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-07-21 14:44:55.000000 secrets-vault-0.1.9/secrets_vault/vault.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-21 14:44:55.000000 secrets-vault-0.1.9/secrets_vault/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:45:22.294222 secrets-vault-0.1.9/secrets_vault.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6260 2023-07-21 14:45:22.000000 secrets-vault-0.1.9/secrets_vault.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-07-21 14:45:22.000000 secrets-vault-0.1.9/secrets_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 14:45:22.000000 secrets-vault-0.1.9/secrets_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-21 14:45:22.000000 secrets-vault-0.1.9/secrets_vault.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-21 14:45:22.000000 secrets-vault-0.1.9/secrets_vault.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-21 14:45:22.000000 secrets-vault-0.1.9/secrets_vault.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 14:45:22.294222 secrets-vault-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-07-21 14:44:55.000000 secrets-vault-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:45:22.294222 secrets-vault-0.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-07-21 14:44:55.000000 secrets-vault-0.1.9/tests/test_backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-07-21 14:44:55.000000 secrets-vault-0.1.9/tests/test_vault.py
```

### Comparing `secrets-vault-0.1.8/LICENSE` & `secrets-vault-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `secrets-vault-0.1.8/PKG-INFO` & `secrets-vault-0.1.9/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,61 +1,59 @@
-Metadata-Version: 2.1
-Name: secrets-vault
-Version: 0.1.8
-Summary: Simple encrypted secrets for Python
-Home-page: https://github.com/anthonynsimon/secrets-vault
-Author: Anthony N. Simon
-License: MIT
-Platform: UNKNOWN
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # secrets-vault
 
 Simple encrypted secrets for Python.
 
-Inspired by Rails encrypted secrets, but for Python. It can be used as a standalone CLI tool or as a library. 
+Inspired by Rails encrypted secrets. It can be used as a standalone CLI tool or as a library. 
 
-The vault is JSON encoded and encrypted using [symmetric encryption](https://cryptography.io/en/latest/fernet/).
+The vault is JSON encoded and encrypted using [AES-GCM-256 authenticated encryption](https://cryptography.io/en/latest/hazmat/primitives/aead/#cryptography.hazmat.primitives.ciphers.aead.AESGCM).
 
 ## Quick start
 
-1. Install `pip install secrets-vault`.
-2. Run `secrets init`.
-3. Two files will be created: `master.key` and `secrets.json.enc`.
-4. You can now edit your secrets by running `secrets edit`, or list them via `secrets get`.
+> **Important:** You should keep the `master.key` secret. Ignore it in your `.gitignore` file. The `secrets.json.enc` file is safe to commit.
 
-**Important:** Keep the `master.key` safe. Do NOT commit it to VCS. The `secrets.json.enc` file is safe to commit.
+1. Install `pip install secrets-vault`.
+2. Run init:
+    ```bash
+    $ secrets init
+    Generated new secrets vault at ./secrets.json.enc
+    Generated new master key at ./master.key - keep it safe!
+    ``` 
+3. You can now edit your secrets:
+   ```bash
+    $ secrets edit
+   
+    >> Opening secrets file in editor...
+    {
+      "foo": "bar"
+    }
+    ```
 
 
 ## CLI usage
 
 You can view the help anytime by running `secrets --help`:
 
 ```
 Usage: secrets [OPTIONS] COMMAND [ARGS]...
 
   Manage a local secrets vault.
 
 Options:
-  -m, --master-key-filepath TEXT  Path to the master.key file.
   -s, --secrets-filepath TEXT     Path to the encrypted secrets vault.
+  -m, --master-key-filepath TEXT  Path to the master.key file.
   --help                          Show this message and exit.
 
 Commands:
-  del     Delete a secret.
-  edit    Open the secrets vault in your configured $EDITOR.
-  envify  Prints a provided secret key as one or more env variables.
-  get     Get one or more secret values.
-  init    Generate a new secrets vault and master.key pair.
-  set     Store a secret.
+  del      Delete a secret.
+  edit     Open the secrets vault in your configured $EDITOR.
+  envify   Prints a provided secret key as one or more env variables.
+  get      Get one or more secret values.
+  init     Generate a new secrets vault and master.key pair.
+  set      Store a secret.
+  version  Show the package version.
 ```
 
 ## Reading secrets
 
 ### CLI commands
 
 List all secrets:
@@ -80,41 +78,43 @@
 > my-user: foo
 > my-password: supersecret
 ```
 
 
 ### In Python
 
+Simply call `get` with the key. Note that if the secret is missing it will return `None`
+
 ```python
 from secrets_vault import SecretsVault
 
 vault = SecretsVault()
 
 password = vault.get('my-password')
 ```
 
 
 ## Editing secrets
 
 ### CLI command
 
-You can also set secrets from the CLI with a key and value:
+You can set secrets from the CLI with a key and value:
 
 ```bash
 $ secrets set foo bar
 ```
 
 ### Interactive editor
 
 To edit secrets, run `secrets edit`, the file will be decrypted and your editor will open.
 
 ```bash
 $ secrets edit
 
->>> Opening secrets file in editor...
+>> Opening secrets file in editor...
 {
   "foo": "bar"
 }
 ```
 
 Any saved changes will be encrypted and saved to the file on disk when you close the editor.
 
@@ -191,41 +191,50 @@
 ### Environment variable
 You can also provide it via an environment variable `MASTER_KEY`. For example:
 
 ```bash
 MASTER_KEY=my-super-secret-master-key secrets edit
 ```
 
+When a master key is provided via an environment variable, it takes precedence over the file on disk.
+
+
 ### In Python
 
 You can load the master_key from anywhere else and provide it when initializing the class:
 
 ```python
 from secrets_vault import SecretsVault
 
 # Load from somewhere else
 master_key = 'my-super-secret-master-key'
 
 vault = SecretsVault(master_key=master_key)
 ```
 
+The order of precedence for the master key is:
+1. Provided via the constructor
+2. Provided via the `MASTER_KEY` environment variable
+3. Loaded from the file on disk
 
 ## Configuring the default filepaths
 
 ### CLI command
 
 You can also provide them as a CLI arguments before the command:
 
 ```bash
 $ secrets \
   --master-key-filepath ./prod/master.key \
   --secrets-filepath ./prod/secrets.json.enc \
   init
 ```
 
+This can be used to separate your secrets by environments such as `prod`, `staging`, `dev`, each having with their own key.
+
 ### In Python
 
 You can also configure the filepaths at which your `secrets.json.enc` and `master.key` files are located.
 
 ```python
 from secrets_vault import SecretsVault
 
@@ -246,9 +255,7 @@
 
 Please check for any existing issues before openning a new Issue. If you'd like to work on something, please open a new Issue describing what you'd like to do before submitting a Pull Request.
 
 
 ## License
 
 See [LICENSE](https://github.com/anthonynsimon/secrets-vault/blob/master/LICENSE).
-
-
```

### Comparing `secrets-vault-0.1.8/README.md` & `secrets-vault-0.1.9/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,46 +1,74 @@
+Metadata-Version: 2.1
+Name: secrets-vault
+Version: 0.1.9
+Summary: Simple encrypted secrets for Python
+Home-page: https://github.com/anthonynsimon/secrets-vault
+Author: Anthony N. Simon
+License: MIT
+Platform: UNKNOWN
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # secrets-vault
 
 Simple encrypted secrets for Python.
 
-Inspired by Rails encrypted secrets, but for Python. It can be used as a standalone CLI tool or as a library. 
+Inspired by Rails encrypted secrets. It can be used as a standalone CLI tool or as a library. 
 
-The vault is JSON encoded and encrypted using [symmetric encryption](https://cryptography.io/en/latest/fernet/).
+The vault is JSON encoded and encrypted using [AES-GCM-256 authenticated encryption](https://cryptography.io/en/latest/hazmat/primitives/aead/#cryptography.hazmat.primitives.ciphers.aead.AESGCM).
 
 ## Quick start
 
-1. Install `pip install secrets-vault`.
-2. Run `secrets init`.
-3. Two files will be created: `master.key` and `secrets.json.enc`.
-4. You can now edit your secrets by running `secrets edit`, or list them via `secrets get`.
+> **Important:** You should keep the `master.key` secret. Ignore it in your `.gitignore` file. The `secrets.json.enc` file is safe to commit.
 
-**Important:** Keep the `master.key` safe. Do NOT commit it to VCS. The `secrets.json.enc` file is safe to commit.
+1. Install `pip install secrets-vault`.
+2. Run init:
+    ```bash
+    $ secrets init
+    Generated new secrets vault at ./secrets.json.enc
+    Generated new master key at ./master.key - keep it safe!
+    ``` 
+3. You can now edit your secrets:
+   ```bash
+    $ secrets edit
+   
+    >> Opening secrets file in editor...
+    {
+      "foo": "bar"
+    }
+    ```
 
 
 ## CLI usage
 
 You can view the help anytime by running `secrets --help`:
 
 ```
 Usage: secrets [OPTIONS] COMMAND [ARGS]...
 
   Manage a local secrets vault.
 
 Options:
-  -m, --master-key-filepath TEXT  Path to the master.key file.
   -s, --secrets-filepath TEXT     Path to the encrypted secrets vault.
+  -m, --master-key-filepath TEXT  Path to the master.key file.
   --help                          Show this message and exit.
 
 Commands:
-  del     Delete a secret.
-  edit    Open the secrets vault in your configured $EDITOR.
-  envify  Prints a provided secret key as one or more env variables.
-  get     Get one or more secret values.
-  init    Generate a new secrets vault and master.key pair.
-  set     Store a secret.
+  del      Delete a secret.
+  edit     Open the secrets vault in your configured $EDITOR.
+  envify   Prints a provided secret key as one or more env variables.
+  get      Get one or more secret values.
+  init     Generate a new secrets vault and master.key pair.
+  set      Store a secret.
+  version  Show the package version.
 ```
 
 ## Reading secrets
 
 ### CLI commands
 
 List all secrets:
@@ -65,41 +93,43 @@
 > my-user: foo
 > my-password: supersecret
 ```
 
 
 ### In Python
 
+Simply call `get` with the key. Note that if the secret is missing it will return `None`
+
 ```python
 from secrets_vault import SecretsVault
 
 vault = SecretsVault()
 
 password = vault.get('my-password')
 ```
 
 
 ## Editing secrets
 
 ### CLI command
 
-You can also set secrets from the CLI with a key and value:
+You can set secrets from the CLI with a key and value:
 
 ```bash
 $ secrets set foo bar
 ```
 
 ### Interactive editor
 
 To edit secrets, run `secrets edit`, the file will be decrypted and your editor will open.
 
 ```bash
 $ secrets edit
 
->>> Opening secrets file in editor...
+>> Opening secrets file in editor...
 {
   "foo": "bar"
 }
 ```
 
 Any saved changes will be encrypted and saved to the file on disk when you close the editor.
 
@@ -176,41 +206,50 @@
 ### Environment variable
 You can also provide it via an environment variable `MASTER_KEY`. For example:
 
 ```bash
 MASTER_KEY=my-super-secret-master-key secrets edit
 ```
 
+When a master key is provided via an environment variable, it takes precedence over the file on disk.
+
+
 ### In Python
 
 You can load the master_key from anywhere else and provide it when initializing the class:
 
 ```python
 from secrets_vault import SecretsVault
 
 # Load from somewhere else
 master_key = 'my-super-secret-master-key'
 
 vault = SecretsVault(master_key=master_key)
 ```
 
+The order of precedence for the master key is:
+1. Provided via the constructor
+2. Provided via the `MASTER_KEY` environment variable
+3. Loaded from the file on disk
 
 ## Configuring the default filepaths
 
 ### CLI command
 
 You can also provide them as a CLI arguments before the command:
 
 ```bash
 $ secrets \
   --master-key-filepath ./prod/master.key \
   --secrets-filepath ./prod/secrets.json.enc \
   init
 ```
 
+This can be used to separate your secrets by environments such as `prod`, `staging`, `dev`, each having with their own key.
+
 ### In Python
 
 You can also configure the filepaths at which your `secrets.json.enc` and `master.key` files are located.
 
 ```python
 from secrets_vault import SecretsVault
 
@@ -231,7 +270,9 @@
 
 Please check for any existing issues before openning a new Issue. If you'd like to work on something, please open a new Issue describing what you'd like to do before submitting a Pull Request.
 
 
 ## License
 
 See [LICENSE](https://github.com/anthonynsimon/secrets-vault/blob/master/LICENSE).
+
+
```

### Comparing `secrets-vault-0.1.8/secrets_vault/__main__.py` & `secrets-vault-0.1.9/secrets_vault/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,20 +19,22 @@
 
 @click.group(help="Manage a local secrets vault.")
 @click.option(
     "-s",
     "--secrets-filepath",
     default=constants.DEFAULT_SECRETS_FILEPATH,
     help="Path to the encrypted secrets vault.",
+    show_default=True,
 )
 @click.option(
     "-m",
     "--master-key-filepath",
     default=constants.DEFAULT_MASTER_KEY_FILEPATH,
     help="Path to the master.key file.",
+    show_default=True,
 )
 @click.pass_context
 def cli(ctx, **kwargs):
     ctx.obj = kwargs
 
 
 @cli.command(help="Show the package version.")
@@ -47,34 +49,29 @@
 @click.pass_context
 def init(ctx):
     try:
         SecretsVault.create(
             secrets_filepath=ctx.obj["secrets_filepath"], master_key_filepath=ctx.obj["master_key_filepath"]
         )
         click.echo(f"Generated new secrets vault at {ctx.obj['secrets_filepath']}")
-        click.echo(f"Generated new master key at {ctx.obj['master_key_filepath']}")
+        click.echo(f"Generated new master key at {ctx.obj['master_key_filepath']} - keep it safe!")
     except exceptions.SecretsFileAlreadyExists:
         print("Secrets file already exists, aborting...")
         exit(1)
 
 
 def with_vault(ctx, func):
     try:
         vault = SecretsVault(
             secrets_filepath=ctx.obj["secrets_filepath"], master_key_filepath=ctx.obj["master_key_filepath"]
         )
         func(vault)
-        exit(0)
-    except exceptions.MasterKeyNotFound:
-        click.echo(
-            f"No master key found. Set it via the environment variable 'MASTER_KEY', or in a file at '{constants.DEFAULT_MASTER_KEY_FILEPATH}'"
-        )
-    except exceptions.SecretsFileNotFound:
-        click.echo("Secrets file not found, aborting...")
-    exit(1)
+    except (exceptions.MasterKeyNotFound, exceptions.SecretsFileNotFound, exceptions.MasterKeyInvalid) as e:
+        click.echo(str(e))
+        exit(1)
 
 
 @cli.command(
     help="Get one or more secret values. If none are specified, all secrets are printed (eg. `secrets get`). You can also provide multiple keys to retrive more than one secret at a time (eg. secrets get foo1 foo2 foo3)."
 )
 @click.argument("key", required=False, nargs=-1)
 @click.pass_context
@@ -93,23 +90,24 @@
     with_vault(ctx, handler)
 
 
 @cli.command(
     help="Prints a provided secret key as one or more env variables. In case the value is a nested object, it will flatten the key=value pairs."
 )
 @click.argument("key")
+@click.option("--export", is_flag=True, help="Include the export modified for each environment variable.")
 @click.pass_context
-def envify(ctx, key):
+def envify(ctx, key, export):
     def handler(vault):
         value = vault.get(key)
         if isinstance(value, dict):
             for k, v in value.items():
-                click.echo(f"{k}={serialize(v)}")
+                click.echo(f"{'export ' if export else ''}{k}={serialize(v)}")
         else:
-            click.echo(f"{key}={serialize(value)}")
+            click.echo(f"{'export ' if export else ''}{key}={serialize(value)}")
 
     with_vault(ctx, handler)
 
 
 @cli.command(
     help="Store a secret. If the secret already exists, it will be overwritten. For example: `secrets set foo bar`"
 )
```

### Comparing `secrets-vault-0.1.8/secrets_vault/vault.py` & `secrets-vault-0.1.9/secrets_vault/vault.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,70 +1,63 @@
 import json
 import logging
 import os
 import tempfile
 from pathlib import Path
 from subprocess import call
 
-from cryptography.fernet import Fernet, InvalidToken
-
+from secrets_vault.backends import AES256GCMBackend
 from secrets_vault.constants import (
     DEFAULT_MASTER_KEY_FILEPATH,
     DEFAULT_SECRETS_FILEPATH,
 )
 from secrets_vault.exceptions import (
     MasterKeyNotFound,
-    MasterKeyInvalid,
     SecretsFileNotFound,
     SecretsFileAlreadyExists,
 )
 
 log = logging.getLogger(__name__)
 
 
 class SecretsVault:
     def __init__(
         self,
         master_key=None,
         secrets_filepath=DEFAULT_SECRETS_FILEPATH,
         master_key_filepath=DEFAULT_MASTER_KEY_FILEPATH,
+        backend=AES256GCMBackend,
     ):
         if master_key is None:
-            master_key = self._load_master_key(master_key_filepath)
-        try:
-            self.fernet = Fernet(master_key)
-            self.secrets_filename = secrets_filepath
-            self.secrets = dict()
-            self._load_secrets()
-        except InvalidToken:
-            raise MasterKeyInvalid("Master key is malformed or invalid")
+            self.master_key = self._load_master_key(master_key_filepath)
+        else:
+            self.master_key = master_key
+        self.secrets_filename = secrets_filepath
+        self.backend = backend(self.master_key)
+        self.secrets = dict()
+        self.load()
 
-    @staticmethod
+    @classmethod
     def create(
+        cls,
         secrets_filepath=DEFAULT_SECRETS_FILEPATH,
         master_key_filepath=DEFAULT_MASTER_KEY_FILEPATH,
+        backend=AES256GCMBackend,
     ):
         """
         Create a new secrets file and returns the master key - keep it safe!
         """
-        if Path(secrets_filepath).exists():
-            raise SecretsFileAlreadyExists(f"Secrets file {secrets_filepath} already exists")
-
-        log.info(f"Creating new secrets file {secrets_filepath}")
-        Path(master_key_filepath).parent.mkdir(parents=True, exist_ok=True)
-        Path(secrets_filepath).parent.mkdir(parents=True, exist_ok=True)
-        Path(secrets_filepath).touch()
+        cls._prepare_dirs(master_key_filepath, secrets_filepath)
 
-        master_key = Fernet.generate_key().decode()
+        master_key = backend.generate_master_key()
         with open(master_key_filepath, "w") as fout:
             fout.write(master_key)
 
         vault = SecretsVault(master_key, secrets_filepath)
-        vault.set("my-user", "foo")
-        vault.set("my-password", "supersecret")
+        vault.secrets = {"my-user": "foo", "my-password": "supersecret"}
         vault.save()
 
         return vault, master_key
 
     def require(self, key):
         return self.secrets[key]
 
@@ -78,53 +71,66 @@
         if key in self.secrets:
             del self.secrets[key]
 
     def edit_secrets(self):
         """
         Decrypts and opens the secrets file in an editor. On save, the file is encrypted again.
         """
-        self._load_secrets()
-        EDITOR = os.environ.get("EDITOR", "vim").split(" ")  # 'could be "code --wait"'
+        editor = os.environ.get("EDITOR", "").split(" ")  # 'could be "code --wait"'
+        if not editor:
+            raise RuntimeError("No interactive editor set. Set it as an environment variable 'EDITOR'")
+
+        self.load()
         with tempfile.NamedTemporaryFile(suffix=".tmp.yml") as tf:
             tf.write(self._serialize())
             tf.flush()
-            call([*EDITOR, tf.name])
+            call([*editor, tf.name])
             tf.seek(0)
             newsecrets = json.loads(tf.read())
 
         if self.secrets == newsecrets:
             log.info("No changes applied")
             return
+
         self.secrets = newsecrets
         self.save()
 
     def save(self):
         with open(self.secrets_filename, "wb") as fout:
-            fout.write(self.fernet.encrypt(self._serialize()))
+            fout.write(self.backend.encrypt(self._serialize()))
         log.info(f"Wrote encrypted secrets to {self.secrets_filename}")
 
+    def load(self):
+        log.info(f"Loading encrypted secrets from {self.secrets_filename}")
+        if not os.path.exists(self.secrets_filename):
+            raise SecretsFileNotFound(f"Could not find secrets file {self.secrets_filename}")
+        with open(self.secrets_filename, "rb") as fin:
+            contents = fin.read()
+            if contents:
+                self.secrets = json.loads(self.backend.decrypt(contents))
+            else:
+                self.secrets = dict()
+
     @staticmethod
-    def _load_master_key(master_key_filepath=None):
+    def _load_master_key(master_key_filepath=None) -> str:
         master_key = os.environ.get("MASTER_KEY")
         if not master_key and master_key_filepath and os.path.exists(master_key_filepath):
-            with open(Path(master_key_filepath).absolute()) as fin:
+            with open(Path(master_key_filepath).absolute(), "r") as fin:
                 master_key = fin.read().strip()
         if not master_key:
             raise MasterKeyNotFound(
                 "Could not find encryption master key. "
                 f"Set it as an environment variable 'MASTER_KEY', or in a file '{master_key_filepath}'"
             )
         return master_key
 
-    def _load_secrets(self):
-        log.info(f"Loading encrypted secrets from {self.secrets_filename}")
-        if not os.path.exists(self.secrets_filename):
-            raise SecretsFileNotFound(f"Could not find secrets file {self.secrets_filename}")
-        with open(self.secrets_filename, "r") as fin:
-            contents = fin.read()
-            if contents:
-                self.secrets = json.loads(self.fernet.decrypt(contents))
-            else:
-                self.secrets = dict()
-
-    def _serialize(self):
+    def _serialize(self) -> bytes:
         return json.dumps(self.secrets, sort_keys=False, indent=4).encode()
+
+    @classmethod
+    def _prepare_dirs(cls, master_key_filepath, secrets_filepath):
+        if Path(secrets_filepath).exists():
+            raise SecretsFileAlreadyExists(f"Secrets file {secrets_filepath} already exists")
+        log.info(f"Creating new secrets file {secrets_filepath}")
+        Path(master_key_filepath).parent.mkdir(parents=True, exist_ok=True)
+        Path(secrets_filepath).parent.mkdir(parents=True, exist_ok=True)
+        Path(secrets_filepath).touch()
```

### Comparing `secrets-vault-0.1.8/secrets_vault.egg-info/PKG-INFO` & `secrets-vault-0.1.9/secrets_vault.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: secrets-vault
-Version: 0.1.8
+Version: 0.1.9
 Summary: Simple encrypted secrets for Python
 Home-page: https://github.com/anthonynsimon/secrets-vault
 Author: Anthony N. Simon
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -13,49 +13,62 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # secrets-vault
 
 Simple encrypted secrets for Python.
 
-Inspired by Rails encrypted secrets, but for Python. It can be used as a standalone CLI tool or as a library. 
+Inspired by Rails encrypted secrets. It can be used as a standalone CLI tool or as a library. 
 
-The vault is JSON encoded and encrypted using [symmetric encryption](https://cryptography.io/en/latest/fernet/).
+The vault is JSON encoded and encrypted using [AES-GCM-256 authenticated encryption](https://cryptography.io/en/latest/hazmat/primitives/aead/#cryptography.hazmat.primitives.ciphers.aead.AESGCM).
 
 ## Quick start
 
-1. Install `pip install secrets-vault`.
-2. Run `secrets init`.
-3. Two files will be created: `master.key` and `secrets.json.enc`.
-4. You can now edit your secrets by running `secrets edit`, or list them via `secrets get`.
+> **Important:** You should keep the `master.key` secret. Ignore it in your `.gitignore` file. The `secrets.json.enc` file is safe to commit.
 
-**Important:** Keep the `master.key` safe. Do NOT commit it to VCS. The `secrets.json.enc` file is safe to commit.
+1. Install `pip install secrets-vault`.
+2. Run init:
+    ```bash
+    $ secrets init
+    Generated new secrets vault at ./secrets.json.enc
+    Generated new master key at ./master.key - keep it safe!
+    ``` 
+3. You can now edit your secrets:
+   ```bash
+    $ secrets edit
+   
+    >> Opening secrets file in editor...
+    {
+      "foo": "bar"
+    }
+    ```
 
 
 ## CLI usage
 
 You can view the help anytime by running `secrets --help`:
 
 ```
 Usage: secrets [OPTIONS] COMMAND [ARGS]...
 
   Manage a local secrets vault.
 
 Options:
-  -m, --master-key-filepath TEXT  Path to the master.key file.
   -s, --secrets-filepath TEXT     Path to the encrypted secrets vault.
+  -m, --master-key-filepath TEXT  Path to the master.key file.
   --help                          Show this message and exit.
 
 Commands:
-  del     Delete a secret.
-  edit    Open the secrets vault in your configured $EDITOR.
-  envify  Prints a provided secret key as one or more env variables.
-  get     Get one or more secret values.
-  init    Generate a new secrets vault and master.key pair.
-  set     Store a secret.
+  del      Delete a secret.
+  edit     Open the secrets vault in your configured $EDITOR.
+  envify   Prints a provided secret key as one or more env variables.
+  get      Get one or more secret values.
+  init     Generate a new secrets vault and master.key pair.
+  set      Store a secret.
+  version  Show the package version.
 ```
 
 ## Reading secrets
 
 ### CLI commands
 
 List all secrets:
@@ -80,41 +93,43 @@
 > my-user: foo
 > my-password: supersecret
 ```
 
 
 ### In Python
 
+Simply call `get` with the key. Note that if the secret is missing it will return `None`
+
 ```python
 from secrets_vault import SecretsVault
 
 vault = SecretsVault()
 
 password = vault.get('my-password')
 ```
 
 
 ## Editing secrets
 
 ### CLI command
 
-You can also set secrets from the CLI with a key and value:
+You can set secrets from the CLI with a key and value:
 
 ```bash
 $ secrets set foo bar
 ```
 
 ### Interactive editor
 
 To edit secrets, run `secrets edit`, the file will be decrypted and your editor will open.
 
 ```bash
 $ secrets edit
 
->>> Opening secrets file in editor...
+>> Opening secrets file in editor...
 {
   "foo": "bar"
 }
 ```
 
 Any saved changes will be encrypted and saved to the file on disk when you close the editor.
 
@@ -191,41 +206,50 @@
 ### Environment variable
 You can also provide it via an environment variable `MASTER_KEY`. For example:
 
 ```bash
 MASTER_KEY=my-super-secret-master-key secrets edit
 ```
 
+When a master key is provided via an environment variable, it takes precedence over the file on disk.
+
+
 ### In Python
 
 You can load the master_key from anywhere else and provide it when initializing the class:
 
 ```python
 from secrets_vault import SecretsVault
 
 # Load from somewhere else
 master_key = 'my-super-secret-master-key'
 
 vault = SecretsVault(master_key=master_key)
 ```
 
+The order of precedence for the master key is:
+1. Provided via the constructor
+2. Provided via the `MASTER_KEY` environment variable
+3. Loaded from the file on disk
 
 ## Configuring the default filepaths
 
 ### CLI command
 
 You can also provide them as a CLI arguments before the command:
 
 ```bash
 $ secrets \
   --master-key-filepath ./prod/master.key \
   --secrets-filepath ./prod/secrets.json.enc \
   init
 ```
 
+This can be used to separate your secrets by environments such as `prod`, `staging`, `dev`, each having with their own key.
+
 ### In Python
 
 You can also configure the filepaths at which your `secrets.json.enc` and `master.key` files are located.
 
 ```python
 from secrets_vault import SecretsVault
```

### Comparing `secrets-vault-0.1.8/setup.py` & `secrets-vault-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `secrets-vault-0.1.8/tests/test_e2e.py` & `secrets-vault-0.1.9/tests/test_vault.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     vault, master_key = SecretsVault.create(
         secrets_filepath=TEST_DATA_DIR / "secrets-1.json.enc",
         master_key_filepath=TEST_DATA_DIR / "master-1.key",
     )
 
     assert os.path.exists(TEST_DATA_DIR / "secrets-1.json.enc")
     assert os.path.exists(TEST_DATA_DIR / "master-1.key")
-    assert master_key is not None and len(master_key) == 44
+    assert master_key is not None and len(master_key) == 64
     with open(TEST_DATA_DIR / "master-1.key", "rb") as fin:
         assert fin.read().decode() == master_key
 
     vault = SecretsVault(
         secrets_filepath=TEST_DATA_DIR / "secrets-1.json.enc",
         master_key_filepath=TEST_DATA_DIR / "master-1.key",
     )
```

