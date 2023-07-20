# Comparing `tmp/secrets-vault-0.1.6.tar.gz` & `tmp/secrets-vault-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secrets-vault-0.1.6.tar", last modified: Thu Jul 20 22:42:07 2023, max compression
+gzip compressed data, was "secrets-vault-0.1.7.tar", last modified: Thu Jul 20 23:06:36 2023, max compression
```

## Comparing `secrets-vault-0.1.6.tar` & `secrets-vault-0.1.7.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:42:07.842967 secrets-vault-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-20 22:41:46.000000 secrets-vault-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5651 2023-07-20 22:42:07.842967 secrets-vault-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5153 2023-07-20 22:41:46.000000 secrets-vault-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:42:07.842967 secrets-vault-0.1.6/secrets_vault/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-20 22:41:46.000000 secrets-vault-0.1.6/secrets_vault/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-07-20 22:41:46.000000 secrets-vault-0.1.6/secrets_vault/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-20 22:41:46.000000 secrets-vault-0.1.6/secrets_vault/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-20 22:41:46.000000 secrets-vault-0.1.6/secrets_vault/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4218 2023-07-20 22:41:46.000000 secrets-vault-0.1.6/secrets_vault/vault.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:42:07.842967 secrets-vault-0.1.6/secrets_vault.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5651 2023-07-20 22:42:07.000000 secrets-vault-0.1.6/secrets_vault.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-20 22:42:07.000000 secrets-vault-0.1.6/secrets_vault.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 22:42:07.000000 secrets-vault-0.1.6/secrets_vault.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-20 22:42:07.000000 secrets-vault-0.1.6/secrets_vault.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-20 22:42:07.000000 secrets-vault-0.1.6/secrets_vault.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-20 22:42:07.000000 secrets-vault-0.1.6/secrets_vault.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 22:42:07.842967 secrets-vault-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-07-20 22:41:46.000000 secrets-vault-0.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:42:07.842967 secrets-vault-0.1.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-07-20 22:41:46.000000 secrets-vault-0.1.6/tests/test_e2e.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 23:06:36.518027 secrets-vault-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-20 23:06:20.000000 secrets-vault-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5497 2023-07-20 23:06:36.518027 secrets-vault-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4999 2023-07-20 23:06:20.000000 secrets-vault-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 23:06:36.514027 secrets-vault-0.1.7/secrets_vault/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-20 23:06:20.000000 secrets-vault-0.1.7/secrets_vault/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4981 2023-07-20 23:06:20.000000 secrets-vault-0.1.7/secrets_vault/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-20 23:06:20.000000 secrets-vault-0.1.7/secrets_vault/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-20 23:06:20.000000 secrets-vault-0.1.7/secrets_vault/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4218 2023-07-20 23:06:20.000000 secrets-vault-0.1.7/secrets_vault/vault.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-20 23:06:20.000000 secrets-vault-0.1.7/secrets_vault/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 23:06:36.514027 secrets-vault-0.1.7/secrets_vault.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5497 2023-07-20 23:06:36.000000 secrets-vault-0.1.7/secrets_vault.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-07-20 23:06:36.000000 secrets-vault-0.1.7/secrets_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 23:06:36.000000 secrets-vault-0.1.7/secrets_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-20 23:06:36.000000 secrets-vault-0.1.7/secrets_vault.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-20 23:06:36.000000 secrets-vault-0.1.7/secrets_vault.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-20 23:06:36.000000 secrets-vault-0.1.7/secrets_vault.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 23:06:36.518027 secrets-vault-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-07-20 23:06:20.000000 secrets-vault-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 23:06:36.514027 secrets-vault-0.1.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-07-20 23:06:20.000000 secrets-vault-0.1.7/tests/test_e2e.py
```

### Comparing `secrets-vault-0.1.6/LICENSE` & `secrets-vault-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `secrets-vault-0.1.6/PKG-INFO` & `secrets-vault-0.1.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: secrets-vault
-Version: 0.1.6
+Version: 0.1.7
 Summary: Simple encrypted secrets for Python
 Home-page: https://github.com/anthonynsimon/secrets-vault
 Author: Anthony N. Simon
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -208,49 +208,33 @@
 vault = SecretsVault(master_key=master_key)
 ```
 
 
 ## Configuring the default filepaths
 
 ### CLI command
-You can also provide them as a CLI argument before any command:
+You can also provide them as a CLI arguments:
 
 ```bash
-$ secrets --master-key-filepath foo1 --secrets-filepath foo2 edit
+$ secrets init --master-key-filepath ./prod/master.key --secrets-filepath ./prod/secrets.json.enc
 ```
 
 ### In Python
 
 You can also configure the filepaths at which your `secrets.json.enc` and `master.key` files are located.
 
 ```python
 from secrets_vault import SecretsVault
 
 vault = SecretsVault(master_key_filepath=..., secrets_filepath=...)
 ```
 
-
 ## Changelog
 
-### 0.1.6
-- Fix requirements not listed in package
-
-### 0.1.5
-- Add envify command
-- Refactor CLI tool
-- Breaking Python API changes: persist() has been renamed to save(), and init() has been renamed to create().
-
-### 0.1.4
-- Add del command
-
-### 0.1.3
-- Add set command
-
-### 0.1.2
-- Initial release
+See [CHANGELOG](https://github.com/anthonynsimon/secrets-vault/blob/master/CHANGELOG) for the list of releases and relevant changes.
 
 
 ## Security Disclosure
 
 If you discover any issue regarding security, please disclose the information responsibly by sending an email to [dyer.linseed0@icloud.com](mailto:dyer.linseed0@icloud.com). Do NOT create a Issue on the GitHub repo.
```

### Comparing `secrets-vault-0.1.6/README.md` & `secrets-vault-0.1.7/secrets_vault.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: secrets-vault
+Version: 0.1.7
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
 
 Inspired by Rails encrypted secrets, but for Python. It can be used as a standalone CLI tool or as a library. 
 
 The vault is JSON encoded and encrypted using [symmetric encryption](https://cryptography.io/en/latest/fernet/).
@@ -193,49 +208,33 @@
 vault = SecretsVault(master_key=master_key)
 ```
 
 
 ## Configuring the default filepaths
 
 ### CLI command
-You can also provide them as a CLI argument before any command:
+You can also provide them as a CLI arguments:
 
 ```bash
-$ secrets --master-key-filepath foo1 --secrets-filepath foo2 edit
+$ secrets init --master-key-filepath ./prod/master.key --secrets-filepath ./prod/secrets.json.enc
 ```
 
 ### In Python
 
 You can also configure the filepaths at which your `secrets.json.enc` and `master.key` files are located.
 
 ```python
 from secrets_vault import SecretsVault
 
 vault = SecretsVault(master_key_filepath=..., secrets_filepath=...)
 ```
 
-
 ## Changelog
 
-### 0.1.6
-- Fix requirements not listed in package
-
-### 0.1.5
-- Add envify command
-- Refactor CLI tool
-- Breaking Python API changes: persist() has been renamed to save(), and init() has been renamed to create().
-
-### 0.1.4
-- Add del command
-
-### 0.1.3
-- Add set command
-
-### 0.1.2
-- Initial release
+See [CHANGELOG](https://github.com/anthonynsimon/secrets-vault/blob/master/CHANGELOG) for the list of releases and relevant changes.
 
 
 ## Security Disclosure
 
 If you discover any issue regarding security, please disclose the information responsibly by sending an email to [dyer.linseed0@icloud.com](mailto:dyer.linseed0@icloud.com). Do NOT create a Issue on the GitHub repo.
 
 
@@ -243,7 +242,9 @@
 
 Please check for any existing issues before openning a new Issue. If you'd like to work on something, please open a new Issue describing what you'd like to do before submitting a Pull Request.
 
 
 ## License
 
 See [LICENSE](https://github.com/anthonynsimon/secrets-vault/blob/master/LICENSE).
+
+
```

### Comparing `secrets-vault-0.1.6/secrets_vault/__main__.py` & `secrets-vault-0.1.7/secrets_vault/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import json
 
 import click
 
-from secrets_vault import SecretsVault, exceptions, constants
+from secrets_vault import SecretsVault, exceptions, constants, __version__
 
 common_options = [
     click.option(
         "-s",
         "--secrets-filepath",
         default=constants.DEFAULT_SECRETS_FILEPATH,
         help="Path to the encrypted secrets vault.",
@@ -43,14 +43,19 @@
 
 @click.group(help="Manage a local secrets vault.")
 @add_options(common_options)
 def cli(**kwargs):
     pass
 
 
+@cli.command(help="Show the package version.")
+def version(**kwargs):
+    click.echo(f"secrets-vault v{__version__}")
+
+
 @cli.command(
     help="Generate a new secrets vault and master.key pair. If a secrets vault already exists, this will abort."
 )
 @add_options(common_options)
 def init(**kwargs):
     try:
         SecretsVault.create(
@@ -69,15 +74,15 @@
         func(vault)
         exit(0)
     except exceptions.MasterKeyNotFound:
         click.echo(
             f"No master key found. Set it via the environment variable 'MASTER_KEY', or in a file at '{constants.DEFAULT_MASTER_KEY_FILEPATH}'"
         )
     except exceptions.SecretsFileNotFound:
-        click.echo("Secrets file already exists, aborting...")
+        click.echo("Secrets file not found, aborting...")
     exit(1)
 
 
 @cli.command(
     help="Get one or more secret values. If none are specified, all secrets are printed (eg. `secrets get`). You can also provide multiple keys to retrive more than one secret at a time (eg. secrets get foo1 foo2 foo3)."
 )
 @add_options(common_options)
```

### Comparing `secrets-vault-0.1.6/secrets_vault/vault.py` & `secrets-vault-0.1.7/secrets_vault/vault.py`

 * *Files identical despite different names*

### Comparing `secrets-vault-0.1.6/secrets_vault.egg-info/PKG-INFO` & `secrets-vault-0.1.7/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: secrets-vault
-Version: 0.1.6
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
 
 Inspired by Rails encrypted secrets, but for Python. It can be used as a standalone CLI tool or as a library. 
 
 The vault is JSON encoded and encrypted using [symmetric encryption](https://cryptography.io/en/latest/fernet/).
@@ -208,49 +193,33 @@
 vault = SecretsVault(master_key=master_key)
 ```
 
 
 ## Configuring the default filepaths
 
 ### CLI command
-You can also provide them as a CLI argument before any command:
+You can also provide them as a CLI arguments:
 
 ```bash
-$ secrets --master-key-filepath foo1 --secrets-filepath foo2 edit
+$ secrets init --master-key-filepath ./prod/master.key --secrets-filepath ./prod/secrets.json.enc
 ```
 
 ### In Python
 
 You can also configure the filepaths at which your `secrets.json.enc` and `master.key` files are located.
 
 ```python
 from secrets_vault import SecretsVault
 
 vault = SecretsVault(master_key_filepath=..., secrets_filepath=...)
 ```
 
-
 ## Changelog
 
-### 0.1.6
-- Fix requirements not listed in package
-
-### 0.1.5
-- Add envify command
-- Refactor CLI tool
-- Breaking Python API changes: persist() has been renamed to save(), and init() has been renamed to create().
-
-### 0.1.4
-- Add del command
-
-### 0.1.3
-- Add set command
-
-### 0.1.2
-- Initial release
+See [CHANGELOG](https://github.com/anthonynsimon/secrets-vault/blob/master/CHANGELOG) for the list of releases and relevant changes.
 
 
 ## Security Disclosure
 
 If you discover any issue regarding security, please disclose the information responsibly by sending an email to [dyer.linseed0@icloud.com](mailto:dyer.linseed0@icloud.com). Do NOT create a Issue on the GitHub repo.
 
 
@@ -258,9 +227,7 @@
 
 Please check for any existing issues before openning a new Issue. If you'd like to work on something, please open a new Issue describing what you'd like to do before submitting a Pull Request.
 
 
 ## License
 
 See [LICENSE](https://github.com/anthonynsimon/secrets-vault/blob/master/LICENSE).
-
-
```

### Comparing `secrets-vault-0.1.6/setup.py` & `secrets-vault-0.1.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,17 +8,20 @@
 
 HERE = pathlib.Path(__file__).parent
 README = (HERE / "README.md").read_text()
 REQUIREMENTS = [
     x.strip() for x in (HERE / "requirements.txt").read_text().split("\n") if not x.startswith("#") and x.strip()
 ]
 
+# Load version without importing anything from the package
+exec(open("secrets_vault/version.py").read())
+
 setup(
     name="secrets-vault",
-    version="0.1.6",
+    version=__version__,
     author="Anthony N. Simon",
     url="https://github.com/anthonynsimon/secrets-vault",
     description="Simple encrypted secrets for Python",
     long_description=README,
     long_description_content_type="text/markdown",
     license="MIT",
     classifiers=[
```

### Comparing `secrets-vault-0.1.6/tests/test_e2e.py` & `secrets-vault-0.1.7/tests/test_e2e.py`

 * *Files identical despite different names*

