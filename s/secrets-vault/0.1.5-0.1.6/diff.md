# Comparing `tmp/secrets-vault-0.1.5.tar.gz` & `tmp/secrets-vault-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secrets-vault-0.1.5.tar", last modified: Thu Jul 20 22:22:23 2023, max compression
+gzip compressed data, was "secrets-vault-0.1.6.tar", last modified: Thu Jul 20 22:42:07 2023, max compression
```

## Comparing `secrets-vault-0.1.5.tar` & `secrets-vault-0.1.6.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:22:23.908959 secrets-vault-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-20 22:22:05.000000 secrets-vault-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5600 2023-07-20 22:22:23.908959 secrets-vault-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5102 2023-07-20 22:22:05.000000 secrets-vault-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:22:23.904959 secrets-vault-0.1.5/secrets_vault/
--rw-r--r--   0 runner    (1001) docker     (123)     4218 2023-07-20 22:22:05.000000 secrets-vault-0.1.5/secrets_vault/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-07-20 22:22:05.000000 secrets-vault-0.1.5/secrets_vault/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-20 22:22:05.000000 secrets-vault-0.1.5/secrets_vault/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-20 22:22:05.000000 secrets-vault-0.1.5/secrets_vault/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:22:23.908959 secrets-vault-0.1.5/secrets_vault.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5600 2023-07-20 22:22:23.000000 secrets-vault-0.1.5/secrets_vault.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-20 22:22:23.000000 secrets-vault-0.1.5/secrets_vault.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 22:22:23.000000 secrets-vault-0.1.5/secrets_vault.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-20 22:22:23.000000 secrets-vault-0.1.5/secrets_vault.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-20 22:22:23.000000 secrets-vault-0.1.5/secrets_vault.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 22:22:23.908959 secrets-vault-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-07-20 22:22:05.000000 secrets-vault-0.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:22:23.908959 secrets-vault-0.1.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-07-20 22:22:05.000000 secrets-vault-0.1.5/tests/test_e2e.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:42:07.842967 secrets-vault-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-20 22:41:46.000000 secrets-vault-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5651 2023-07-20 22:42:07.842967 secrets-vault-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5153 2023-07-20 22:41:46.000000 secrets-vault-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:42:07.842967 secrets-vault-0.1.6/secrets_vault/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-20 22:41:46.000000 secrets-vault-0.1.6/secrets_vault/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-07-20 22:41:46.000000 secrets-vault-0.1.6/secrets_vault/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-20 22:41:46.000000 secrets-vault-0.1.6/secrets_vault/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-20 22:41:46.000000 secrets-vault-0.1.6/secrets_vault/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4218 2023-07-20 22:41:46.000000 secrets-vault-0.1.6/secrets_vault/vault.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:42:07.842967 secrets-vault-0.1.6/secrets_vault.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5651 2023-07-20 22:42:07.000000 secrets-vault-0.1.6/secrets_vault.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-20 22:42:07.000000 secrets-vault-0.1.6/secrets_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 22:42:07.000000 secrets-vault-0.1.6/secrets_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-20 22:42:07.000000 secrets-vault-0.1.6/secrets_vault.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-20 22:42:07.000000 secrets-vault-0.1.6/secrets_vault.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-20 22:42:07.000000 secrets-vault-0.1.6/secrets_vault.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 22:42:07.842967 secrets-vault-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-07-20 22:41:46.000000 secrets-vault-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 22:42:07.842967 secrets-vault-0.1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-07-20 22:41:46.000000 secrets-vault-0.1.6/tests/test_e2e.py
```

### Comparing `secrets-vault-0.1.5/LICENSE` & `secrets-vault-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `secrets-vault-0.1.5/PKG-INFO` & `secrets-vault-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: secrets-vault
-Version: 0.1.5
+Version: 0.1.6
 Summary: Simple encrypted secrets for Python
 Home-page: https://github.com/anthonynsimon/secrets-vault
 Author: Anthony N. Simon
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -149,15 +149,15 @@
 
 vault = SecretsVault()
 vault.delete('foo')
 vault.save()
 ```
 
 
-### Printing secrets as environment variables
+## Printing secrets as environment variables
 
 Sometimes you may want to print a secret as environment variables. It will also apply if you have nested objects. You can do so by running:
 
 ```bash
 $ secrets edit
 
 {
@@ -227,14 +227,17 @@
 
 vault = SecretsVault(master_key_filepath=..., secrets_filepath=...)
 ```
 
 
 ## Changelog
 
+### 0.1.6
+- Fix requirements not listed in package
+
 ### 0.1.5
 - Add envify command
 - Refactor CLI tool
 - Breaking Python API changes: persist() has been renamed to save(), and init() has been renamed to create().
 
 ### 0.1.4
 - Add del command
```

### Comparing `secrets-vault-0.1.5/README.md` & `secrets-vault-0.1.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -134,15 +134,15 @@
 
 vault = SecretsVault()
 vault.delete('foo')
 vault.save()
 ```
 
 
-### Printing secrets as environment variables
+## Printing secrets as environment variables
 
 Sometimes you may want to print a secret as environment variables. It will also apply if you have nested objects. You can do so by running:
 
 ```bash
 $ secrets edit
 
 {
@@ -212,14 +212,17 @@
 
 vault = SecretsVault(master_key_filepath=..., secrets_filepath=...)
 ```
 
 
 ## Changelog
 
+### 0.1.6
+- Fix requirements not listed in package
+
 ### 0.1.5
 - Add envify command
 - Refactor CLI tool
 - Breaking Python API changes: persist() has been renamed to save(), and init() has been renamed to create().
 
 ### 0.1.4
 - Add del command
```

### Comparing `secrets-vault-0.1.5/secrets_vault/__init__.py` & `secrets-vault-0.1.6/secrets_vault/vault.py`

 * *Files identical despite different names*

### Comparing `secrets-vault-0.1.5/secrets_vault/__main__.py` & `secrets-vault-0.1.6/secrets_vault/__main__.py`

 * *Files identical despite different names*

### Comparing `secrets-vault-0.1.5/secrets_vault.egg-info/PKG-INFO` & `secrets-vault-0.1.6/secrets_vault.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: secrets-vault
-Version: 0.1.5
+Version: 0.1.6
 Summary: Simple encrypted secrets for Python
 Home-page: https://github.com/anthonynsimon/secrets-vault
 Author: Anthony N. Simon
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -149,15 +149,15 @@
 
 vault = SecretsVault()
 vault.delete('foo')
 vault.save()
 ```
 
 
-### Printing secrets as environment variables
+## Printing secrets as environment variables
 
 Sometimes you may want to print a secret as environment variables. It will also apply if you have nested objects. You can do so by running:
 
 ```bash
 $ secrets edit
 
 {
@@ -227,14 +227,17 @@
 
 vault = SecretsVault(master_key_filepath=..., secrets_filepath=...)
 ```
 
 
 ## Changelog
 
+### 0.1.6
+- Fix requirements not listed in package
+
 ### 0.1.5
 - Add envify command
 - Refactor CLI tool
 - Breaking Python API changes: persist() has been renamed to save(), and init() has been renamed to create().
 
 ### 0.1.4
 - Add del command
```

### Comparing `secrets-vault-0.1.5/setup.py` & `secrets-vault-0.1.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,19 +4,21 @@
 
 from setuptools import find_packages, setup
 
 assert sys.version_info >= (3, 9), "Requires Python v3.9 or above."
 
 HERE = pathlib.Path(__file__).parent
 README = (HERE / "README.md").read_text()
-
+REQUIREMENTS = [
+    x.strip() for x in (HERE / "requirements.txt").read_text().split("\n") if not x.startswith("#") and x.strip()
+]
 
 setup(
     name="secrets-vault",
-    version="0.1.5",
+    version="0.1.6",
     author="Anthony N. Simon",
     url="https://github.com/anthonynsimon/secrets-vault",
     description="Simple encrypted secrets for Python",
     long_description=README,
     long_description_content_type="text/markdown",
     license="MIT",
     classifiers=[
@@ -29,9 +31,10 @@
     include_package_data=True,
     entry_points={
         "console_scripts": [
             "secrets-vault=secrets_vault.__main__:cli",
             "secrets=secrets_vault.__main__:cli",
         ]
     },
+    install_requires=REQUIREMENTS,
     tests_require=[],
 )
```

### Comparing `secrets-vault-0.1.5/tests/test_e2e.py` & `secrets-vault-0.1.6/tests/test_e2e.py`

 * *Files identical despite different names*

