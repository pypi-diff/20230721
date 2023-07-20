# Comparing `tmp/secrets-vault-0.1.7.tar.gz` & `tmp/secrets-vault-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secrets-vault-0.1.7.tar", last modified: Thu Jul 20 23:06:36 2023, max compression
+gzip compressed data, was "secrets-vault-0.1.8.tar", last modified: Thu Jul 20 23:26:36 2023, max compression
```

## Comparing `secrets-vault-0.1.7.tar` & `secrets-vault-0.1.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 23:06:36.518027 secrets-vault-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-20 23:06:20.000000 secrets-vault-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5497 2023-07-20 23:06:36.518027 secrets-vault-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4999 2023-07-20 23:06:20.000000 secrets-vault-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 23:06:36.514027 secrets-vault-0.1.7/secrets_vault/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-20 23:06:20.000000 secrets-vault-0.1.7/secrets_vault/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4981 2023-07-20 23:06:20.000000 secrets-vault-0.1.7/secrets_vault/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-20 23:06:20.000000 secrets-vault-0.1.7/secrets_vault/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-20 23:06:20.000000 secrets-vault-0.1.7/secrets_vault/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4218 2023-07-20 23:06:20.000000 secrets-vault-0.1.7/secrets_vault/vault.py
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-20 23:06:20.000000 secrets-vault-0.1.7/secrets_vault/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 23:06:36.514027 secrets-vault-0.1.7/secrets_vault.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5497 2023-07-20 23:06:36.000000 secrets-vault-0.1.7/secrets_vault.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-07-20 23:06:36.000000 secrets-vault-0.1.7/secrets_vault.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 23:06:36.000000 secrets-vault-0.1.7/secrets_vault.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-20 23:06:36.000000 secrets-vault-0.1.7/secrets_vault.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-20 23:06:36.000000 secrets-vault-0.1.7/secrets_vault.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-20 23:06:36.000000 secrets-vault-0.1.7/secrets_vault.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 23:06:36.518027 secrets-vault-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-07-20 23:06:20.000000 secrets-vault-0.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 23:06:36.514027 secrets-vault-0.1.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-07-20 23:06:20.000000 secrets-vault-0.1.7/tests/test_e2e.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 23:26:36.625046 secrets-vault-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-20 23:26:11.000000 secrets-vault-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-07-20 23:26:36.625046 secrets-vault-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-07-20 23:26:11.000000 secrets-vault-0.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 23:26:36.621046 secrets-vault-0.1.8/secrets_vault/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-20 23:26:11.000000 secrets-vault-0.1.8/secrets_vault/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-07-20 23:26:11.000000 secrets-vault-0.1.8/secrets_vault/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-20 23:26:11.000000 secrets-vault-0.1.8/secrets_vault/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-20 23:26:11.000000 secrets-vault-0.1.8/secrets_vault/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4367 2023-07-20 23:26:11.000000 secrets-vault-0.1.8/secrets_vault/vault.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-20 23:26:11.000000 secrets-vault-0.1.8/secrets_vault/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 23:26:36.625046 secrets-vault-0.1.8/secrets_vault.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-07-20 23:26:36.000000 secrets-vault-0.1.8/secrets_vault.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-07-20 23:26:36.000000 secrets-vault-0.1.8/secrets_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 23:26:36.000000 secrets-vault-0.1.8/secrets_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-20 23:26:36.000000 secrets-vault-0.1.8/secrets_vault.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-20 23:26:36.000000 secrets-vault-0.1.8/secrets_vault.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-20 23:26:36.000000 secrets-vault-0.1.8/secrets_vault.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 23:26:36.625046 secrets-vault-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-07-20 23:26:11.000000 secrets-vault-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 23:26:36.625046 secrets-vault-0.1.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-07-20 23:26:11.000000 secrets-vault-0.1.8/tests/test_e2e.py
```

### Comparing `secrets-vault-0.1.7/LICENSE` & `secrets-vault-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `secrets-vault-0.1.7/PKG-INFO` & `secrets-vault-0.1.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: secrets-vault
-Version: 0.1.7
+Version: 0.1.8
 Summary: Simple encrypted secrets for Python
 Home-page: https://github.com/anthonynsimon/secrets-vault
 Author: Anthony N. Simon
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -208,33 +208,37 @@
 vault = SecretsVault(master_key=master_key)
 ```
 
 
 ## Configuring the default filepaths
 
 ### CLI command
-You can also provide them as a CLI arguments:
+
+You can also provide them as a CLI arguments before the command:
 
 ```bash
-$ secrets init --master-key-filepath ./prod/master.key --secrets-filepath ./prod/secrets.json.enc
+$ secrets \
+  --master-key-filepath ./prod/master.key \
+  --secrets-filepath ./prod/secrets.json.enc \
+  init
 ```
 
 ### In Python
 
 You can also configure the filepaths at which your `secrets.json.enc` and `master.key` files are located.
 
 ```python
 from secrets_vault import SecretsVault
 
 vault = SecretsVault(master_key_filepath=..., secrets_filepath=...)
 ```
 
 ## Changelog
 
-See [CHANGELOG](https://github.com/anthonynsimon/secrets-vault/blob/master/CHANGELOG) for the list of releases and relevant changes.
+See [CHANGELOG](https://github.com/anthonynsimon/secrets-vault/blob/master/CHANGELOG.md) for the list of releases.
 
 
 ## Security Disclosure
 
 If you discover any issue regarding security, please disclose the information responsibly by sending an email to [dyer.linseed0@icloud.com](mailto:dyer.linseed0@icloud.com). Do NOT create a Issue on the GitHub repo.
```

### Comparing `secrets-vault-0.1.7/README.md` & `secrets-vault-0.1.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -193,33 +193,37 @@
 vault = SecretsVault(master_key=master_key)
 ```
 
 
 ## Configuring the default filepaths
 
 ### CLI command
-You can also provide them as a CLI arguments:
+
+You can also provide them as a CLI arguments before the command:
 
 ```bash
-$ secrets init --master-key-filepath ./prod/master.key --secrets-filepath ./prod/secrets.json.enc
+$ secrets \
+  --master-key-filepath ./prod/master.key \
+  --secrets-filepath ./prod/secrets.json.enc \
+  init
 ```
 
 ### In Python
 
 You can also configure the filepaths at which your `secrets.json.enc` and `master.key` files are located.
 
 ```python
 from secrets_vault import SecretsVault
 
 vault = SecretsVault(master_key_filepath=..., secrets_filepath=...)
 ```
 
 ## Changelog
 
-See [CHANGELOG](https://github.com/anthonynsimon/secrets-vault/blob/master/CHANGELOG) for the list of releases and relevant changes.
+See [CHANGELOG](https://github.com/anthonynsimon/secrets-vault/blob/master/CHANGELOG.md) for the list of releases.
 
 
 ## Security Disclosure
 
 If you discover any issue regarding security, please disclose the information responsibly by sending an email to [dyer.linseed0@icloud.com](mailto:dyer.linseed0@icloud.com). Do NOT create a Issue on the GitHub repo.
```

### Comparing `secrets-vault-0.1.7/secrets_vault/__main__.py` & `secrets-vault-0.1.8/secrets_vault/__main__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,177 +1,148 @@
 import json
 
 import click
 
 from secrets_vault import SecretsVault, exceptions, constants, __version__
 
-common_options = [
-    click.option(
-        "-s",
-        "--secrets-filepath",
-        default=constants.DEFAULT_SECRETS_FILEPATH,
-        help="Path to the encrypted secrets vault.",
-    ),
-    click.option(
-        "-m",
-        "--master-key-filepath",
-        default=constants.DEFAULT_MASTER_KEY_FILEPATH,
-        help="Path to the master.key file.",
-    ),
-]
-
-
-def add_options(options):
-    def _add_options(func):
-        for option in options:
-            func = option(func)
-        return func
-
-    return _add_options
-
 
 def serialize(v):
     if not v:
         return ""
     if isinstance(v, str):
         return v
     if isinstance(v, int):
         return str(v)
     if isinstance(v, float):
         return str(v)
     return json.dumps(v, default=str, sort_keys=False)
 
 
 @click.group(help="Manage a local secrets vault.")
-@add_options(common_options)
-def cli(**kwargs):
-    pass
+@click.option(
+    "-s",
+    "--secrets-filepath",
+    default=constants.DEFAULT_SECRETS_FILEPATH,
+    help="Path to the encrypted secrets vault.",
+)
+@click.option(
+    "-m",
+    "--master-key-filepath",
+    default=constants.DEFAULT_MASTER_KEY_FILEPATH,
+    help="Path to the master.key file.",
+)
+@click.pass_context
+def cli(ctx, **kwargs):
+    ctx.obj = kwargs
 
 
 @cli.command(help="Show the package version.")
-def version(**kwargs):
+@click.pass_context
+def version(ctx):
     click.echo(f"secrets-vault v{__version__}")
 
 
 @cli.command(
     help="Generate a new secrets vault and master.key pair. If a secrets vault already exists, this will abort."
 )
-@add_options(common_options)
-def init(**kwargs):
+@click.pass_context
+def init(ctx):
     try:
         SecretsVault.create(
-            secrets_filepath=kwargs["secrets_filepath"], master_key_filepath=kwargs["master_key_filepath"]
+            secrets_filepath=ctx.obj["secrets_filepath"], master_key_filepath=ctx.obj["master_key_filepath"]
         )
-        click.echo(f"Generated new secrets vault at {kwargs['secrets_filepath']}")
-        click.echo(f"Generated new master key at {kwargs['master_key_filepath']}")
+        click.echo(f"Generated new secrets vault at {ctx.obj['secrets_filepath']}")
+        click.echo(f"Generated new master key at {ctx.obj['master_key_filepath']}")
     except exceptions.SecretsFileAlreadyExists:
         print("Secrets file already exists, aborting...")
         exit(1)
 
 
-def with_vault(func, secrets_filepath, master_key_filepath):
+def with_vault(ctx, func):
     try:
-        vault = SecretsVault(secrets_filepath=secrets_filepath, master_key_filepath=master_key_filepath)
+        vault = SecretsVault(
+            secrets_filepath=ctx.obj["secrets_filepath"], master_key_filepath=ctx.obj["master_key_filepath"]
+        )
         func(vault)
         exit(0)
     except exceptions.MasterKeyNotFound:
         click.echo(
             f"No master key found. Set it via the environment variable 'MASTER_KEY', or in a file at '{constants.DEFAULT_MASTER_KEY_FILEPATH}'"
         )
     except exceptions.SecretsFileNotFound:
         click.echo("Secrets file not found, aborting...")
     exit(1)
 
 
 @cli.command(
     help="Get one or more secret values. If none are specified, all secrets are printed (eg. `secrets get`). You can also provide multiple keys to retrive more than one secret at a time (eg. secrets get foo1 foo2 foo3)."
 )
-@add_options(common_options)
 @click.argument("key", required=False, nargs=-1)
-def get(key, **kwargs):
+@click.pass_context
+def get(ctx, key):
     def handler(vault):
         if key:
             if len(key) == 1:
                 click.echo(serialize(vault.get(key[0])))
             else:
                 for k in key:
                     click.echo(f"{k}: {serialize(vault.get(k))}")
         else:
             for k, v in vault.secrets.items():
                 click.echo(f"{k}: {serialize(v)}")
 
-    with_vault(
-        handler,
-        secrets_filepath=kwargs["secrets_filepath"],
-        master_key_filepath=kwargs["master_key_filepath"],
-    )
+    with_vault(ctx, handler)
 
 
 @cli.command(
     help="Prints a provided secret key as one or more env variables. In case the value is a nested object, it will flatten the key=value pairs."
 )
-@add_options(common_options)
 @click.argument("key")
-def envify(key, **kwargs):
+@click.pass_context
+def envify(ctx, key):
     def handler(vault):
         value = vault.get(key)
         if isinstance(value, dict):
             for k, v in value.items():
                 click.echo(f"{k}={serialize(v)}")
         else:
             click.echo(f"{key}={serialize(value)}")
 
-    with_vault(
-        handler,
-        secrets_filepath=kwargs["secrets_filepath"],
-        master_key_filepath=kwargs["master_key_filepath"],
-    )
+    with_vault(ctx, handler)
 
 
 @cli.command(
     help="Store a secret. If the secret already exists, it will be overwritten. For example: `secrets set foo bar`"
 )
-@add_options(common_options)
 @click.argument("key")
 @click.argument("value")
-def set(key, value, **kwargs):
+@click.pass_context
+def set(ctx, key, value):
     def handler(vault):
         vault.set(key, value)
         vault.save()
 
-    with_vault(
-        handler,
-        secrets_filepath=kwargs["secrets_filepath"],
-        master_key_filepath=kwargs["master_key_filepath"],
-    )
+    with_vault(ctx, handler)
 
 
 @cli.command("del", help="Delete a secret. For example: `secrets del foo`")
-@add_options(common_options)
 @click.argument("key")
-def delete(key, **kwargs):
+@click.pass_context
+def delete(ctx, key):
     def handler(vault):
         vault.delete(key)
         vault.save()
 
-    with_vault(
-        handler,
-        secrets_filepath=kwargs["secrets_filepath"],
-        master_key_filepath=kwargs["master_key_filepath"],
-    )
+    with_vault(ctx, handler)
 
 
 @cli.command(help="Open the secrets vault in your configured $EDITOR.")
-@add_options(common_options)
-def edit(**kwargs):
+@click.pass_context
+def edit(ctx):
     def handler(vault):
         vault.edit_secrets()
 
-    with_vault(
-        handler,
-        secrets_filepath=kwargs["secrets_filepath"],
-        master_key_filepath=kwargs["master_key_filepath"],
-    )
+    with_vault(ctx, handler)
 
 
 if __name__ == "__main__":
     cli()
```

### Comparing `secrets-vault-0.1.7/secrets_vault/vault.py` & `secrets-vault-0.1.8/secrets_vault/vault.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,14 +46,16 @@
         """
         Create a new secrets file and returns the master key - keep it safe!
         """
         if Path(secrets_filepath).exists():
             raise SecretsFileAlreadyExists(f"Secrets file {secrets_filepath} already exists")
 
         log.info(f"Creating new secrets file {secrets_filepath}")
+        Path(master_key_filepath).parent.mkdir(parents=True, exist_ok=True)
+        Path(secrets_filepath).parent.mkdir(parents=True, exist_ok=True)
         Path(secrets_filepath).touch()
 
         master_key = Fernet.generate_key().decode()
         with open(master_key_filepath, "w") as fout:
             fout.write(master_key)
 
         vault = SecretsVault(master_key, secrets_filepath)
```

### Comparing `secrets-vault-0.1.7/secrets_vault.egg-info/PKG-INFO` & `secrets-vault-0.1.8/secrets_vault.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: secrets-vault
-Version: 0.1.7
+Version: 0.1.8
 Summary: Simple encrypted secrets for Python
 Home-page: https://github.com/anthonynsimon/secrets-vault
 Author: Anthony N. Simon
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -208,33 +208,37 @@
 vault = SecretsVault(master_key=master_key)
 ```
 
 
 ## Configuring the default filepaths
 
 ### CLI command
-You can also provide them as a CLI arguments:
+
+You can also provide them as a CLI arguments before the command:
 
 ```bash
-$ secrets init --master-key-filepath ./prod/master.key --secrets-filepath ./prod/secrets.json.enc
+$ secrets \
+  --master-key-filepath ./prod/master.key \
+  --secrets-filepath ./prod/secrets.json.enc \
+  init
 ```
 
 ### In Python
 
 You can also configure the filepaths at which your `secrets.json.enc` and `master.key` files are located.
 
 ```python
 from secrets_vault import SecretsVault
 
 vault = SecretsVault(master_key_filepath=..., secrets_filepath=...)
 ```
 
 ## Changelog
 
-See [CHANGELOG](https://github.com/anthonynsimon/secrets-vault/blob/master/CHANGELOG) for the list of releases and relevant changes.
+See [CHANGELOG](https://github.com/anthonynsimon/secrets-vault/blob/master/CHANGELOG.md) for the list of releases.
 
 
 ## Security Disclosure
 
 If you discover any issue regarding security, please disclose the information responsibly by sending an email to [dyer.linseed0@icloud.com](mailto:dyer.linseed0@icloud.com). Do NOT create a Issue on the GitHub repo.
```

### Comparing `secrets-vault-0.1.7/setup.py` & `secrets-vault-0.1.8/setup.py`

 * *Files identical despite different names*

### Comparing `secrets-vault-0.1.7/tests/test_e2e.py` & `secrets-vault-0.1.8/tests/test_e2e.py`

 * *Files identical despite different names*

