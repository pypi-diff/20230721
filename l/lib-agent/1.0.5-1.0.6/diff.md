# Comparing `tmp/lib-agent-1.0.5.tar.gz` & `tmp/lib-agent-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib-agent-1.0.5.tar", last modified: Fri May 27 18:04:14 2022, max compression
+gzip compressed data, was "lib-agent-1.0.6.tar", last modified: Fri Jul 21 03:27:12 2023, max compression
```

## Comparing `lib-agent-1.0.5.tar` & `lib-agent-1.0.6.tar`

### file list

```diff
@@ -1,46 +1,47 @@
-drwxr-xr-x   0 t          (501) staff       (20)        0 2022-05-27 18:04:14.568164 lib-agent-1.0.5/
--rw-r--r--   0 t          (501) staff       (20)      895 2022-05-27 18:04:14.567906 lib-agent-1.0.5/PKG-INFO
--rw-r--r--   0 t          (501) staff       (20)     3076 2022-05-27 17:26:10.000000 lib-agent-1.0.5/README.md
-drwxr-xr-x   0 t          (501) staff       (20)        0 2022-05-27 18:04:14.547043 lib-agent-1.0.5/lib_agent.egg-info/
--rw-r--r--   0 t          (501) staff       (20)      895 2022-05-27 18:04:14.000000 lib-agent-1.0.5/lib_agent.egg-info/PKG-INFO
--rw-r--r--   0 t          (501) staff       (20)      909 2022-05-27 18:04:14.000000 lib-agent-1.0.5/lib_agent.egg-info/SOURCES.txt
--rw-r--r--   0 t          (501) staff       (20)        1 2022-05-27 18:04:14.000000 lib-agent-1.0.5/lib_agent.egg-info/dependency_links.txt
--rw-r--r--   0 t          (501) staff       (20)      265 2022-05-27 18:04:14.000000 lib-agent-1.0.5/lib_agent.egg-info/requires.txt
--rw-r--r--   0 t          (501) staff       (20)        9 2022-05-27 18:04:14.000000 lib-agent-1.0.5/lib_agent.egg-info/top_level.txt
-drwxr-xr-x   0 t          (501) staff       (20)        0 2022-05-27 18:04:14.549694 lib-agent-1.0.5/libagent/
--rw-r--r--   0 t          (501) staff       (20)       70 2022-05-27 17:26:10.000000 lib-agent-1.0.5/libagent/__init__.py
-drwxr-xr-x   0 t          (501) staff       (20)        0 2022-05-27 18:04:14.551031 lib-agent-1.0.5/libagent/age/
--rw-r--r--   0 t          (501) staff       (20)     5550 2022-05-27 17:26:10.000000 lib-agent-1.0.5/libagent/age/__init__.py
--rw-r--r--   0 t          (501) staff       (20)     1605 2022-05-27 17:26:10.000000 lib-agent-1.0.5/libagent/age/client.py
-drwxr-xr-x   0 t          (501) staff       (20)        0 2022-05-27 18:04:14.559339 lib-agent-1.0.5/libagent/device/
--rw-r--r--   0 t          (501) staff       (20)       77 2022-05-27 17:26:10.000000 lib-agent-1.0.5/libagent/device/__init__.py
--rw-r--r--   0 t          (501) staff       (20)     2612 2022-05-27 17:26:10.000000 lib-agent-1.0.5/libagent/device/fake_device.py
--rw-r--r--   0 t          (501) staff       (20)     4426 2022-05-27 17:26:10.000000 lib-agent-1.0.5/libagent/device/interface.py
--rw-r--r--   0 t          (501) staff       (20)     6135 2022-05-27 17:26:10.000000 lib-agent-1.0.5/libagent/device/jade.py
--rw-r--r--   0 t          (501) staff       (20)     1369 2022-05-27 17:41:12.000000 lib-agent-1.0.5/libagent/device/keepkey.py
--rw-r--r--   0 t          (501) staff       (20)      755 2022-05-27 17:26:10.000000 lib-agent-1.0.5/libagent/device/keepkey_defs.py
--rw-r--r--   0 t          (501) staff       (20)     4294 2022-05-27 17:26:10.000000 lib-agent-1.0.5/libagent/device/ledger.py
--rw-r--r--   0 t          (501) staff       (20)    20495 2022-05-27 17:26:10.000000 lib-agent-1.0.5/libagent/device/onlykey.py
--rw-r--r--   0 t          (501) staff       (20)      137 2022-05-27 17:26:10.000000 lib-agent-1.0.5/libagent/device/onlykey_defs.py
--rw-r--r--   0 t          (501) staff       (20)     6062 2022-05-27 17:26:10.000000 lib-agent-1.0.5/libagent/device/trezor.py
--rw-r--r--   0 t          (501) staff       (20)      975 2022-05-27 17:26:10.000000 lib-agent-1.0.5/libagent/device/trezor_defs.py
--rw-r--r--   0 t          (501) staff       (20)     5238 2022-05-27 17:26:10.000000 lib-agent-1.0.5/libagent/device/ui.py
--rw-r--r--   0 t          (501) staff       (20)     9271 2022-05-27 17:26:10.000000 lib-agent-1.0.5/libagent/formats.py
-drwxr-xr-x   0 t          (501) staff       (20)        0 2022-05-27 18:04:14.564099 lib-agent-1.0.5/libagent/gpg/
--rw-r--r--   0 t          (501) staff       (20)    15486 2022-05-27 17:26:10.000000 lib-agent-1.0.5/libagent/gpg/__init__.py
--rw-r--r--   0 t          (501) staff       (20)    12191 2022-05-27 17:26:10.000000 lib-agent-1.0.5/libagent/gpg/agent.py
--rw-r--r--   0 t          (501) staff       (20)     2161 2022-05-27 17:26:10.000000 lib-agent-1.0.5/libagent/gpg/client.py
--rw-r--r--   0 t          (501) staff       (20)    11509 2022-05-27 17:26:10.000000 lib-agent-1.0.5/libagent/gpg/decode.py
--rw-r--r--   0 t          (501) staff       (20)     4370 2022-05-27 17:26:10.000000 lib-agent-1.0.5/libagent/gpg/encode.py
--rw-r--r--   0 t          (501) staff       (20)     7760 2022-05-27 17:26:10.000000 lib-agent-1.0.5/libagent/gpg/keyring.py
--rw-r--r--   0 t          (501) staff       (20)     9968 2022-05-27 17:26:10.000000 lib-agent-1.0.5/libagent/gpg/protocol.py
--rw-r--r--   0 t          (501) staff       (20)     4438 2022-05-27 17:26:10.000000 lib-agent-1.0.5/libagent/server.py
-drwxr-xr-x   0 t          (501) staff       (20)        0 2022-05-27 18:04:14.564763 lib-agent-1.0.5/libagent/signify/
--rw-r--r--   0 t          (501) staff       (20)     3592 2022-05-27 17:26:10.000000 lib-agent-1.0.5/libagent/signify/__init__.py
-drwxr-xr-x   0 t          (501) staff       (20)        0 2022-05-27 18:04:14.567227 lib-agent-1.0.5/libagent/ssh/
--rw-r--r--   0 t          (501) staff       (20)    12221 2022-05-27 17:26:10.000000 lib-agent-1.0.5/libagent/ssh/__init__.py
--rw-r--r--   0 t          (501) staff       (20)     3131 2022-05-27 17:35:13.000000 lib-agent-1.0.5/libagent/ssh/client.py
--rw-r--r--   0 t          (501) staff       (20)     6197 2022-05-27 17:36:00.000000 lib-agent-1.0.5/libagent/ssh/protocol.py
--rw-r--r--   0 t          (501) staff       (20)     7157 2022-05-27 17:26:10.000000 lib-agent-1.0.5/libagent/util.py
--rw-r--r--   0 t          (501) staff       (20)       38 2022-05-27 18:04:14.568514 lib-agent-1.0.5/setup.cfg
--rwxr-xr-x   0 t          (501) staff       (20)     1580 2022-05-27 17:41:09.000000 lib-agent-1.0.5/setup.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-07-21 03:27:12.752518 lib-agent-1.0.6/
+-rw-r--r--   0 kali      (1000) kali      (1000)     7652 2023-07-21 03:25:10.000000 lib-agent-1.0.6/LICENSE
+-rw-r--r--   0 kali      (1000) kali      (1000)      876 2023-07-21 03:27:12.752518 lib-agent-1.0.6/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)     3040 2023-07-21 03:25:10.000000 lib-agent-1.0.6/README.md
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-07-21 03:27:12.744517 lib-agent-1.0.6/lib_agent.egg-info/
+-rw-r--r--   0 kali      (1000) kali      (1000)      876 2023-07-21 03:27:12.000000 lib-agent-1.0.6/lib_agent.egg-info/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)      917 2023-07-21 03:27:12.000000 lib-agent-1.0.6/lib_agent.egg-info/SOURCES.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-07-21 03:27:12.000000 lib-agent-1.0.6/lib_agent.egg-info/dependency_links.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)      265 2023-07-21 03:27:12.000000 lib-agent-1.0.6/lib_agent.egg-info/requires.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        9 2023-07-21 03:27:12.000000 lib-agent-1.0.6/lib_agent.egg-info/top_level.txt
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-07-21 03:27:12.744517 lib-agent-1.0.6/libagent/
+-rw-r--r--   0 kali      (1000) kali      (1000)       70 2023-07-21 03:25:10.000000 lib-agent-1.0.6/libagent/__init__.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-07-21 03:27:12.744517 lib-agent-1.0.6/libagent/age/
+-rw-r--r--   0 kali      (1000) kali      (1000)     5875 2023-07-21 03:25:10.000000 lib-agent-1.0.6/libagent/age/__init__.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     1605 2023-07-21 03:25:10.000000 lib-agent-1.0.6/libagent/age/client.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-07-21 03:27:12.748518 lib-agent-1.0.6/libagent/device/
+-rw-r--r--   0 kali      (1000) kali      (1000)       77 2023-07-21 03:25:10.000000 lib-agent-1.0.6/libagent/device/__init__.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     2612 2023-07-21 03:25:10.000000 lib-agent-1.0.6/libagent/device/fake_device.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     4426 2023-07-21 03:25:10.000000 lib-agent-1.0.6/libagent/device/interface.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     6140 2023-07-21 03:25:10.000000 lib-agent-1.0.6/libagent/device/jade.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     1369 2023-07-21 03:25:10.000000 lib-agent-1.0.6/libagent/device/keepkey.py
+-rw-r--r--   0 kali      (1000) kali      (1000)      755 2023-07-21 03:25:10.000000 lib-agent-1.0.6/libagent/device/keepkey_defs.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     6704 2023-07-21 03:25:10.000000 lib-agent-1.0.6/libagent/device/ledger.py
+-rw-r--r--   0 kali      (1000) kali      (1000)    22565 2023-07-21 03:25:10.000000 lib-agent-1.0.6/libagent/device/onlykey.py
+-rw-r--r--   0 kali      (1000) kali      (1000)      137 2023-07-21 03:25:10.000000 lib-agent-1.0.6/libagent/device/onlykey_defs.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     6062 2023-07-21 03:25:10.000000 lib-agent-1.0.6/libagent/device/trezor.py
+-rw-r--r--   0 kali      (1000) kali      (1000)      975 2023-07-21 03:25:10.000000 lib-agent-1.0.6/libagent/device/trezor_defs.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     5238 2023-07-21 03:25:10.000000 lib-agent-1.0.6/libagent/device/ui.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     9271 2023-07-21 03:25:10.000000 lib-agent-1.0.6/libagent/formats.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-07-21 03:27:12.752518 lib-agent-1.0.6/libagent/gpg/
+-rw-r--r--   0 kali      (1000) kali      (1000)    15486 2023-07-21 03:25:10.000000 lib-agent-1.0.6/libagent/gpg/__init__.py
+-rw-r--r--   0 kali      (1000) kali      (1000)    12240 2023-07-21 03:25:10.000000 lib-agent-1.0.6/libagent/gpg/agent.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     2223 2023-07-21 03:25:10.000000 lib-agent-1.0.6/libagent/gpg/client.py
+-rw-r--r--   0 kali      (1000) kali      (1000)    11509 2023-07-21 03:25:10.000000 lib-agent-1.0.6/libagent/gpg/decode.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     4366 2023-07-21 03:25:10.000000 lib-agent-1.0.6/libagent/gpg/encode.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     7760 2023-07-21 03:25:10.000000 lib-agent-1.0.6/libagent/gpg/keyring.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     9968 2023-07-21 03:25:10.000000 lib-agent-1.0.6/libagent/gpg/protocol.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     4437 2023-07-21 03:25:10.000000 lib-agent-1.0.6/libagent/server.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-07-21 03:27:12.752518 lib-agent-1.0.6/libagent/signify/
+-rw-r--r--   0 kali      (1000) kali      (1000)     4508 2023-07-21 03:25:10.000000 lib-agent-1.0.6/libagent/signify/__init__.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-07-21 03:27:12.752518 lib-agent-1.0.6/libagent/ssh/
+-rw-r--r--   0 kali      (1000) kali      (1000)    12218 2023-07-21 03:25:10.000000 lib-agent-1.0.6/libagent/ssh/__init__.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     3404 2023-07-21 03:25:10.000000 lib-agent-1.0.6/libagent/ssh/client.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     6303 2023-07-21 03:25:10.000000 lib-agent-1.0.6/libagent/ssh/protocol.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     7157 2023-07-21 03:25:10.000000 lib-agent-1.0.6/libagent/util.py
+-rw-r--r--   0 kali      (1000) kali      (1000)       38 2023-07-21 03:27:12.752518 lib-agent-1.0.6/setup.cfg
+-rwxr-xr-x   0 kali      (1000) kali      (1000)     1577 2023-07-21 03:25:10.000000 lib-agent-1.0.6/setup.py
```

### Comparing `lib-agent-1.0.5/PKG-INFO` & `lib-agent-1.0.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,22 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: lib-agent
-Version: 1.0.5
+Version: 1.0.6
 Summary: Using OnlyKey as hardware SSH and GPG agent
-Home-page: http://github.com/onlykey/onlykey-agent
+Home-page: https://github.com/onlykey/lib-agent
 Author: CryptoTrust
 Author-email: admin@crp.to
-License: UNKNOWN
-Description: UNKNOWN
 Platform: POSIX
 Classifier: Environment :: Console
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Networking
 Classifier: Topic :: Communications
 Classifier: Topic :: Security
 Classifier: Topic :: Utilities
+License-File: LICENSE
```

### Comparing `lib-agent-1.0.5/README.md` & `lib-agent-1.0.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-# Hardware-based SSH/GPG agent
+# Hardware-based SSH/GPG/age agent
 
 [![Build](https://github.com/romanz/trezor-agent/actions/workflows/ci.yml/badge.svg)](https://github.com/romanz/trezor-agent/actions)
 [![Chat](https://badges.gitter.im/romanz/trezor-agent.svg)](https://gitter.im/romanz/trezor-agent)
 
-This project allows you to use various hardware security devices to operate GPG and SSH.  Instead of keeping your key on your computer and decrypting it with a passphrase when you want to use it, the key is generated and stored on the device and never reaches your computer.  Read more about the design [here](doc/DESIGN.md).
+This project allows you to use various hardware security devices to operate GPG, SSH and age.  Instead of keeping your key on your computer and decrypting it with a passphrase when you want to use it, the key is generated and stored on the device and never reaches your computer.  Read more about the design [here](doc/DESIGN.md).
 
-You can do things like sign your emails, git commits, and software packages, manage your passwords (with [pass](https://www.passwordstore.org/) and [gopass](https://www.justwatch.com/gopass/), among others), authenticate web tunnels and file transfers, and more.
+You can do things like sign your emails, git commits, and software packages, manage your passwords (with [pass](https://www.passwordstore.org/) and [passage](https://github.com/FiloSottile/passage), among others), authenticate web tunnels and file transfers, and more.
 
 See the following blog posts about this tool:
 
 - [TREZOR Firmware 1.3.4 enables SSH login](https://medium.com/@satoshilabs/trezor-firmware-1-3-4-enables-ssh-login-86a622d7e609)
 - [TREZOR Firmware 1.3.6 — GPG Signing, SSH Login Updates and Advanced Transaction Features for Segwit](https://medium.com/@satoshilabs/trezor-firmware-1-3-6-20a7df6e692)
 - [TREZOR Firmware 1.4.0 — GPG decryption support](https://www.reddit.com/r/TREZOR/comments/50h8r9/new_trezor_firmware_fidou2f_and_initial_ethereum/d7420q7/)
 - [A Step by Step Guide to Securing your SSH Keys with the Ledger Nano S](https://thoughts.t37.net/a-step-by-step-guide-to-securing-your-ssh-keys-with-the-ledger-nano-s-92e58c64a005)
@@ -18,26 +18,25 @@
 
 ## Components
 
 This repository contains source code for one library as well as
 agents to interact with several different hardware devices:
 
 * [`libagent`](https://pypi.org/project/libagent/): shared library
-* [`trezor-agent`](https://pypi.org/project/trezor-agent/): Using Trezor as hardware-based SSH/PGP agent
+* [`trezor-agent`](https://pypi.org/project/trezor-agent/): Using Trezor as hardware-based SSH/PGP/age agent
 * [`ledger_agent`](https://pypi.org/project/ledger_agent/): Using Ledger as hardware-based SSH/PGP agent
 * [`jade_agent`](https://pypi.org/project/jade_agent/): Using Blockstream Jade as hardware-based SSH/PGP agent
 * [`keepkey_agent`](https://pypi.org/project/keepkey_agent/): Using KeepKey as hardware-based SSH/PGP agent
 * [`onlykey-agent`](https://pypi.org/project/onlykey-agent/): Using OnlyKey as hardware-based SSH/PGP agent
 
 
 The [/releases](/releases) page on Github contains the `libagent`
 releases.
 
 ## Documentation
 
 * **Installation** instructions are [here](doc/INSTALL.md)
 * **SSH** instructions and common use cases are [here](doc/README-SSH.md)
 
-    Note: If you're using Windows, see [trezor-ssh-agent](https://github.com/martin-lizner/trezor-ssh-agent) by Martin Lízner.
-
 * **GPG** instructions and common use cases are [here](doc/README-GPG.md)
+* **age** instructions and common use cases are [here](doc/README-age.md)
 * Instructions to configure a Trezor-style **PIN entry** program are [here](doc/README-PINENTRY.md)
```

### Comparing `lib-agent-1.0.5/lib_agent.egg-info/PKG-INFO` & `lib-agent-1.0.6/lib_agent.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,22 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: lib-agent
-Version: 1.0.5
+Version: 1.0.6
 Summary: Using OnlyKey as hardware SSH and GPG agent
-Home-page: http://github.com/onlykey/onlykey-agent
+Home-page: https://github.com/onlykey/lib-agent
 Author: CryptoTrust
 Author-email: admin@crp.to
-License: UNKNOWN
-Description: UNKNOWN
 Platform: POSIX
 Classifier: Environment :: Console
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Networking
 Classifier: Topic :: Communications
 Classifier: Topic :: Security
 Classifier: Topic :: Utilities
+License-File: LICENSE
```

### Comparing `lib-agent-1.0.5/lib_agent.egg-info/SOURCES.txt` & `lib-agent-1.0.6/lib_agent.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.py
 lib_agent.egg-info/PKG-INFO
 lib_agent.egg-info/SOURCES.txt
 lib_agent.egg-info/dependency_links.txt
 lib_agent.egg-info/requires.txt
 lib_agent.egg-info/top_level.txt
```

### Comparing `lib-agent-1.0.5/libagent/age/__init__.py` & `lib-agent-1.0.6/libagent/age/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,14 +7,15 @@
  - https://github.com/str4d/rage/
 """
 
 import argparse
 import base64
 import contextlib
 import datetime
+import io
 import logging
 import os
 import sys
 import traceback
 
 import bech32
 import pkg_resources
@@ -61,17 +62,24 @@
 def base64_decode(encoded: str) -> bytes:
     """Decode Base64-encoded data (after padding correctly with '=')."""
     k = len(encoded) % 4
     pad = (4 - k) if k else 0
     return base64.b64decode(encoded + ("=" * pad))
 
 
+# https://github.com/FiloSottile/age/blob/v1.1.0-rc.1/internal/format/format.go#L45
+BYTES_PER_LINE = 48
+
+
 def base64_encode(data: bytes) -> str:
     """Encode data using Base64 (and remove '=')."""
-    return base64.b64encode(data).replace(b"=", b"").decode()
+    reader = io.BytesIO(data)
+    chunks = map(base64.b64encode, iter(lambda: reader.read(BYTES_PER_LINE), b""))
+    chunks = (chunk.replace(b"=", b"") for chunk in chunks)
+    return b"\n".join(chunks).decode()
 
 
 def decrypt(key, encrypted):
     """Decrypt age-encrypted data."""
     cipher = ChaCha20Poly1305(key)
     try:
         return cipher.decrypt(
@@ -120,17 +128,18 @@
     sys.stdout.write('-> done\n\n')
     sys.stdout.flush()
     sys.stdout.close()
 
 
 def _handle_single_file(file_index, stanzas, identities, c):
     d = c.device.__class__.__name__
-    msg = base64_encode(f'Please confirm decryption on {d} device...'.encode())
     for peer_pubkey, encrypted in stanzas:
         for identity in identities:
+            id_str = identity.to_string()
+            msg = base64_encode(f'Please confirm {id_str} decryption on {d} device...'.encode())
             sys.stdout.write(f'-> msg\n{msg}\n')
             sys.stdout.flush()
 
             key = c.ecdh(identity=identity, peer_pubkey=peer_pubkey)
             result = decrypt(key=key, encrypted=encrypted)
             if not result:
                 continue
```

### Comparing `lib-agent-1.0.5/libagent/age/client.py` & `lib-agent-1.0.6/libagent/age/client.py`

 * *Files identical despite different names*

### Comparing `lib-agent-1.0.5/libagent/device/fake_device.py` & `lib-agent-1.0.6/libagent/device/fake_device.py`

 * *Files identical despite different names*

### Comparing `lib-agent-1.0.5/libagent/device/interface.py` & `lib-agent-1.0.6/libagent/device/interface.py`

 * *Files identical despite different names*

### Comparing `lib-agent-1.0.5/libagent/device/jade.py` & `lib-agent-1.0.6/libagent/device/jade.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Jade-related code (see https://www.keepkey.com/)."""
+"""Jade-related code (see https://blockstream.com/jade/)."""
 
 import logging
 
 import ecdsa
 import semver
 
 from .. import formats, util
```

### Comparing `lib-agent-1.0.5/libagent/device/keepkey.py` & `lib-agent-1.0.6/libagent/device/keepkey.py`

 * *Files identical despite different names*

### Comparing `lib-agent-1.0.5/libagent/device/keepkey_defs.py` & `lib-agent-1.0.6/libagent/device/keepkey_defs.py`

 * *Files identical despite different names*

### Comparing `lib-agent-1.0.5/libagent/device/ledger.py` & `lib-agent-1.0.6/libagent/device/ledger.py`

 * *Files 27% similar despite different names*

```diff
@@ -34,26 +34,55 @@
         result = b'\x00' + bytes(keyY)
     return bytes(result)
 
 
 class LedgerNanoS(interface.Device):
     """Connection to Ledger Nano S device."""
 
+    LEDGER_APP_NAME = "SSH/PGP Agent"
+    ledger_app_version = None
+    ledger_app_supports_end_of_frame_byte = True
+
+    def get_app_name_and_version(self, dongle):
+        """Retrieve currently running Ledger application name and its version string."""
+        device_version_answer = dongle.exchange(binascii.unhexlify('B001000000'))
+        offset = 1
+        app_name_length = struct.unpack_from("B", device_version_answer, offset)[0]
+        offset += 1
+        app_name = device_version_answer[offset: offset + app_name_length]
+        offset += app_name_length
+        app_version_length = struct.unpack_from("B", device_version_answer, offset)[0]
+        offset += 1
+        app_version = device_version_answer[offset: offset + app_version_length]
+        log.debug("running app %s, version %s", app_name, app_version)
+        return (app_name.decode(), app_version.decode())
+
     @classmethod
     def package_name(cls):
         """Python package name (at PyPI)."""
         return 'ledger-agent'
 
     def connect(self):
         """Enumerate and connect to the first USB HID interface."""
         try:
-            return comm.getDongle()
+            dongle = comm.getDongle(debug=True)
+            (app_name, self.ledger_app_version) = self.get_app_name_and_version(dongle)
+
+            version_parts = self.ledger_app_version.split(".")
+            if (version_parts[0] == "0" and version_parts[1] == "0" and int(version_parts[2]) <= 7):
+                self.ledger_app_supports_end_of_frame_byte = False
+
+            if app_name != LedgerNanoS.LEDGER_APP_NAME:
+                # we could launch the app here if we are in the dashboard
+                raise interface.DeviceError(f'{self} is not running {LedgerNanoS.LEDGER_APP_NAME}')
+
+            return dongle
         except comm.CommException as e:
-            raise interface.NotFoundError(
-                '{} not connected: "{}"'.format(self, e))
+            raise interface.DeviceError(
+                'Error ({}) communicating with {}'.format(e, self))
 
     def pubkey(self, identity, ecdh=False):
         """Get PublicKey object for specified BIP32 address and elliptic curve."""
         curve_name = identity.get_curve_name(ecdh)
         path = _expand_path(identity.get_bip32_address(ecdh))
         if curve_name == 'nist256p1':
             p2 = '01'
@@ -68,32 +97,52 @@
         log.debug('result: %r', result)
         return formats.decompress_pubkey(
             pubkey=_convert_public_key(curve_name, result[1:]),
             curve_name=identity.curve_name)
 
     def sign(self, identity, blob):
         """Sign given blob and return the signature (as bytes)."""
+        # pylint: disable=too-many-locals,too-many-branches
         path = _expand_path(identity.get_bip32_address(ecdh=False))
-        if identity.identity_dict['proto'] == 'ssh':
-            ins = '04'
-            p1 = '00'
-        else:
-            ins = '08'
-            p1 = '00'
-        if identity.curve_name == 'nist256p1':
-            p2 = '81' if identity.identity_dict['proto'] == 'ssh' else '01'
-        else:
-            p2 = '82' if identity.identity_dict['proto'] == 'ssh' else '02'
-        apdu = '80' + ins + p1 + p2
-        apdu = binascii.unhexlify(apdu)
-        apdu += bytearray([len(blob) + len(path) + 1])
-        apdu += bytearray([len(path) // 4]) + path
-        apdu += blob
-        log.debug('apdu: %r', apdu)
-        result = bytearray(self.conn.exchange(bytes(apdu)))
+        offset = 0
+        result = None
+        while offset != len(blob):
+            data = bytes()
+            if offset == 0:
+                data += bytearray([len(path) // 4]) + path
+            chunk_size = min(len(blob) - offset, 255 - len(data))
+            data += blob[offset:offset + chunk_size]
+
+            if identity.identity_dict['proto'] == 'ssh':
+                ins = '04'
+            else:
+                ins = '08'
+
+            if identity.curve_name == 'nist256p1':
+                p2 = '81' if identity.identity_dict['proto'] == 'ssh' else '01'
+            else:
+                p2 = '82' if identity.identity_dict['proto'] == 'ssh' else '02'
+
+            if offset + chunk_size == len(blob) and self.ledger_app_supports_end_of_frame_byte:
+                # mark that we are at the end of the frame
+                p1 = "80" if offset == 0 else "81"
+            else:
+                p1 = "00" if offset == 0 else "01"
+
+            apdu = binascii.unhexlify('80' + ins + p1 + p2) + len(data).to_bytes(1, 'little') + data
+
+            log.debug('apdu: %r', apdu)
+            try:
+                result = bytearray(self.conn.exchange(bytes(apdu)))
+            except comm.CommException as e:
+                raise interface.DeviceError(
+                    'Error ({}) communicating with {}'.format(e, self))
+
+            offset += chunk_size
+
         log.debug('result: %r', result)
         if identity.curve_name == 'nist256p1':
             offset = 3
             length = result[offset]
             r = result[offset+1:offset+1+length]
             if r[0] == 0:
                 r = r[1:]
@@ -116,11 +165,15 @@
             p2 = '02'
         apdu = '800a00' + p2
         apdu = binascii.unhexlify(apdu)
         apdu += bytearray([len(pubkey) + len(path) + 1])
         apdu += bytearray([len(path) // 4]) + path
         apdu += pubkey
         log.debug('apdu: %r', apdu)
-        result = bytearray(self.conn.exchange(bytes(apdu)))
+        try:
+            result = bytearray(self.conn.exchange(bytes(apdu)))
+        except comm.CommException as e:
+            raise interface.DeviceError(
+                'Error ({}) communicating with {}'.format(e, self))
         log.debug('result: %r', result)
         assert result[0] == 0x04
         return bytes(result)
```

### Comparing `lib-agent-1.0.5/libagent/device/onlykey.py` & `lib-agent-1.0.6/libagent/device/onlykey.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import codecs
 import os
 from os import path
 import time
 import ecdsa
 import nacl.signing
 import unidecode
+import re
 
 from . import interface
 
 # import pgpy
 # from pgpy import PGPKey
 
 
@@ -67,14 +68,35 @@
     def import_pub(self, pubkey):
         """Import PGP public key."""
         self.import_pubkey = pubkey
         log.debug('Public key to import = %s', pubkey)
         # self.import_pubkey_obj, _ = pgpy.PGPKey.from_blob(pubkey)
         # self.import_pubkey_bytes = bytes(self.import_pubkey_obj)
 
+    def get_key_by_keygrip(self, keygrip):
+        if keygrip is None:
+            return None
+        keygriplong = keygrip
+        keygrip = keygrip[:16]
+        log.info(keygrip)
+        keygrips = {}
+        keylabels = self.ok.getkeylabels()
+        for i in keylabels:
+            if i.number + 72 >= 100:
+                keygrips[i.label.replace("ÿ", " ").encode('ascii')] = i.number + 72
+            else:
+                keygrips[i.label.replace("ÿ", " ").encode('ascii')] = i.number - 24
+        if keygrip in keygrips:
+            return keygrips[keygrip]
+        for i in keylabels:
+            if re.search(r'[A-F0-9]{16}', i.label):
+                raise KeyError('keygrip %s not found' % keygriplong)
+        return None
+
+
     def get_sk_dk(self):
         """Get signing key and decryption key slots from config."""
         fpath = os.path.join(os.environ.get('AGENTHOMEDIR', os.environ.get('GNUPGHOME')), 'run-agent.sh')
         log.debug('Path to run-agent.sh = %s', fpath)
         if path.exists(fpath):
             with open(fpath) as f:
                 s = f.read()
@@ -116,17 +138,25 @@
         """Close connection."""
         log.info('disconnected from %s', self.device_name)
         self.ok.close()
 
     def pubkey(self, identity, ecdh=False):
         """Return public key."""
         curve_name = identity.get_curve_name(ecdh=ecdh)
-        if identity.identity_dict['proto'] != 'ssh' and hasattr('self', 'skeyslot') is False:
+        keygrip_slot_id = None
+        if identity.identity_dict['proto'] != 'ssh' and hasattr(self, 'skeyslot') is False:
             self.get_sk_dk()
-        if identity.identity_dict['proto'] != 'ssh' and self.dkeyslot < 132 and ecdh is True:
+        if identity.identity_dict['proto'] != 'ssh':
+            log.info('Looking for keygrip =%s', identity.identity_dict['keygrip'])
+            keygrip = identity.identity_dict['keygrip']
+            keygrip_slot_id = self.get_key_by_keygrip(keygrip)
+
+        if keygrip_slot_id is not None:
+            this_slot_id = keygrip_slot_id
+        elif identity.identity_dict['proto'] != 'ssh' and self.dkeyslot < 132 and ecdh is True:
             this_slot_id = self.dkeyslot
             log.info('Key Slot =%s', this_slot_id)
         elif self.skeyslot < 132 and ecdh is False:
             this_slot_id = self.skeyslot
             log.info('Key Slot =%s', this_slot_id)
         else:
             this_slot_id = 132
@@ -243,16 +273,21 @@
             return ok_pubkey
 
     def sign(self, identity, blob):
         """Sign given blob and return the signature (as bytes)."""
         curve_name = identity.get_curve_name(ecdh=False)
         log.debug('"%s" signing %r (%s) on %s',
                   identity.to_string(), blob, curve_name, self)
-        if identity.identity_dict['proto'] != 'ssh' and hasattr('self', 'skeyslot') is False:
+        keygrip_slot_id = None
+        if identity.identity_dict['proto'] != 'ssh' and hasattr(self, 'skeyslot') is False:
             self.get_sk_dk()
+        if identity.identity_dict['proto'] != 'ssh':
+            log.info('Looking for keygrip =%s', identity.identity_dict['keygrip'])
+            keygrip = identity.identity_dict['keygrip']
+            keygrip_slot_id = self.get_key_by_keygrip(keygrip)
         # Calculate hash for SSH signing
         if 'rsa' in curve_name:
             if self.sighash == b'rsa-sha2-512':
                 log.info('rsa-sha2-512')
                 h1 = hashlib.sha512()
                 h1.update(blob)
                 data = h1.hexdigest()
@@ -278,15 +313,22 @@
             data = h1.hexdigest()
             data = codecs.decode(data, 'hex_codec')
             log.info('Identity to hash =%s', id_parts)
             log.info('Identity hash =%s', data)
         # Determine type of key to derive on OnlyKey for signature
         # Slot 132 used for derived key, slots 101-116 used for stored ecc keys
         # slots 1-4 used for stored RSA keys
-        if self.skeyslot == 132:
+        if keygrip_slot_id is not None:
+            this_slot_id = keygrip_slot_id
+            log.info('Key Slot =%s', this_slot_id)
+            if curve_name != 'rsa':
+                raw_message = blob
+            else:
+                raw_message = data
+        elif self.skeyslot == 132:
             if curve_name == 'ed25519':
                 this_slot_id = 201
                 log.info('Key type ed25519')
             elif curve_name == 'nist256p1':
                 this_slot_id = 202
                 log.info('Key type nistp256')
             else:
@@ -351,15 +393,15 @@
                         t_end = time.time() + 1
                         # Todo know RSA type to know how many packets
                 except Exception as e:
                     raise interface.DeviceError(e)
 
             log.info('received= %s', repr(result))
             return bytes(result)
-        raise Exception('failed to sign challenge')
+        raise interface.Error('failed to sign challenge')
 
     def ecdh_with_pubkey(self, identity, pubkey):
         """Get shared session key using Elliptic Curve Diffie-Hellman & self public key."""
         self_pubkey = self.pubkey(ecdh=False, identity=identity)
         log.info('Using self_pubkey= %s', self_pubkey)
         session_key = self.ecdh(identity, pubkey)
         if self_pubkey:
@@ -385,27 +427,36 @@
         log.info('Identity to hash =%s', id_parts)
         data = h1.hexdigest()
         log.info('Identity hash =%s', data)
         data = codecs.decode(data, 'hex_codec')
         # Determine type of key to derive on OnlyKey for ecdh
         # Slot 132 used for derived key, slots 101-116 used for stored ecc keys,
         # slots 1-4 used for stored RSA keys
+        keygrip_slot_id = None
+        if identity.identity_dict['proto'] != 'ssh':
+            log.info('Looking for keygrip =%s', identity.identity_dict['keygrip'])
+            keygrip = identity.identity_dict['keygrip']
+            keygrip_slot_id = self.get_key_by_keygrip(keygrip)
+
         if self.dkeyslot == 132:
             if curve_name == 'curve25519':
                 this_slot_id = 204
                 log.info('Key type curve25519')
             elif curve_name == 'nist256p1':
                 this_slot_id = 202
                 log.info('Key type nistp256')
             else:
                 this_slot_id = 203
                 log.info('Key type secp256k1')
             raw_message = pubkey + data
         else:
-            this_slot_id = self.dkeyslot
+            if keygrip_slot_id is not None:
+                this_slot_id = keygrip_slot_id
+            else:
+                this_slot_id = self.dkeyslot
             raw_message = pubkey
         log.info('Key Slot =%s', this_slot_id)
         log.info('data hash =%s', data)
         h2 = hashlib.sha256()
         h2.update(raw_message)
         d = h2.digest()
         assert len(d) == 32
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `lib-agent-1.0.5/libagent/device/trezor.py` & `lib-agent-1.0.6/libagent/device/trezor.py`

 * *Files identical despite different names*

### Comparing `lib-agent-1.0.5/libagent/device/trezor_defs.py` & `lib-agent-1.0.6/libagent/device/trezor_defs.py`

 * *Files identical despite different names*

### Comparing `lib-agent-1.0.5/libagent/device/ui.py` & `lib-agent-1.0.6/libagent/device/ui.py`

 * *Files identical despite different names*

### Comparing `lib-agent-1.0.5/libagent/formats.py` & `lib-agent-1.0.6/libagent/formats.py`

 * *Files identical despite different names*

### Comparing `lib-agent-1.0.5/libagent/gpg/__init__.py` & `lib-agent-1.0.6/libagent/gpg/__init__.py`

 * *Files identical despite different names*

### Comparing `lib-agent-1.0.5/libagent/gpg/agent.py` & `lib-agent-1.0.6/libagent/gpg/agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -189,38 +189,38 @@
         pubkey_dict, user_ids = decode.load_by_keygrip(
             pubkey_bytes=self.pubkey_bytes, keygrip=keygrip_bytes)
         # We assume the first user ID is used to generate Agent-based GPG keys.
         user_id = user_ids[0]['value'].decode('utf-8')
         if pubkey_dict['algo'] not in {1, 2, 3}:
             curve_name = protocol.get_curve_name_by_oid(pubkey_dict['curve_oid'])
             ecdh = (pubkey_dict['algo'] == protocol.ECDH_ALGO_ID)
-            identity = client.create_identity(user_id=user_id, curve_name=curve_name)
+            identity = client.create_identity(user_id=user_id, curve_name=curve_name, keygrip=keygrip)
             verifying_key = self.client.pubkey(identity=identity, ecdh=ecdh)
             pubkey = protocol.PublicKey(
                 curve_name=curve_name, created=pubkey_dict['created'],
                 verifying_key=verifying_key, ecdh=ecdh)
             assert pubkey.key_id() == pubkey_dict['key_id']
             assert pubkey.keygrip() == keygrip_bytes
         elif len(pubkey_dict['_to_hash']) < 350:
-            identity = client.create_identity(user_id=user_id, curve_name='rsa2048')
+            identity = client.create_identity(user_id=user_id, curve_name='rsa2048', keygrip=keygrip)
             verifying_key = self.client.pubkey(identity=identity, ecdh=False)
             pubkey = protocol.PublicKey(
-            curve_name='rsa2048', created=pubkey_dict['created'],
-            verifying_key=verifying_key, ecdh=False)
+                curve_name='rsa2048', created=pubkey_dict['created'],
+                verifying_key=verifying_key, ecdh=False)
         elif len(pubkey_dict['_to_hash']) < 700:
-            identity = client.create_identity(user_id=user_id, curve_name='rsa4096')
+            identity = client.create_identity(user_id=user_id, curve_name='rsa4096', keygrip=keygrip)
             verifying_key = self.client.pubkey(identity=identity, ecdh=False)
             pubkey = protocol.PublicKey(
-            curve_name='rsa4096', created=pubkey_dict['created'],
-            verifying_key=verifying_key, ecdh=False)   
+                curve_name='rsa4096', created=pubkey_dict['created'],
+                verifying_key=verifying_key, ecdh=False)
         else:
             identity = 'unknown identity type'
             log.error(identity)
-            
-        log.info('IDENTITY(%s)', identity)   
+
+        log.info('IDENTITY(%s)', identity)
         return identity
 
     def pksign(self, conn):
         """Sign a message digest using a private EC key."""
         log.debug('signing %r digest (algo #%s)', self.digest, self.algo)
         identity = self.get_identity(keygrip=self.keygrip)
         if identity.curve_name == 'rsa2048' :
```

### Comparing `lib-agent-1.0.5/libagent/gpg/client.py` & `lib-agent-1.0.6/libagent/gpg/client.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,18 +4,19 @@
 
 from .. import formats, util
 from ..device import interface
 
 log = logging.getLogger(__name__)
 
 
-def create_identity(user_id, curve_name):
+def create_identity(user_id, curve_name, keygrip = None):
     """Create GPG identity for hardware device."""
     result = interface.Identity(identity_str='gpg://', curve_name=curve_name)
     result.identity_dict['host'] = user_id
+    result.identity_dict['keygrip'] = keygrip
     return result
 
 
 class Client:
     """Sign messages and get public keys from a hardware device."""
 
     def __init__(self, device):
```

### Comparing `lib-agent-1.0.5/libagent/gpg/decode.py` & `lib-agent-1.0.6/libagent/gpg/decode.py`

 * *Files identical despite different names*

### Comparing `lib-agent-1.0.5/libagent/gpg/encode.py` & `lib-agent-1.0.6/libagent/gpg/encode.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 log = logging.getLogger(__name__)
 
 
 def create_primary(user_id, pubkey, signer_func, secret_bytes=b''):
     """Export new primary GPG public key, ready for "gpg2 --import"."""
     pubkey_packet = protocol.packet(tag=(5 if secret_bytes else 6),
-                                    blob=(pubkey.data() + secret_bytes))
+                                    blob=pubkey.data() + secret_bytes)
     user_id_bytes = user_id.encode('utf-8')
     user_id_packet = protocol.packet(tag=13, blob=user_id_bytes)
     data_to_sign = (pubkey.data_to_hash() + user_id_packet[:1] +
                     util.prefix_len('>L', user_id_bytes))
     hashed_subpackets = [
         protocol.subpacket_time(pubkey.created),  # signature time
         # https://tools.ietf.org/html/rfc4880#section-5.2.3.7
@@ -47,15 +47,15 @@
     sign_packet = protocol.packet(tag=2, blob=signature)
     return pubkey_packet + user_id_packet + sign_packet
 
 
 def create_subkey(primary_bytes, subkey, signer_func, secret_bytes=b''):
     """Export new subkey to GPG primary key."""
     subkey_packet = protocol.packet(tag=(7 if secret_bytes else 14),
-                                    blob=(subkey.data() + secret_bytes))
+                                    blob=subkey.data() + secret_bytes)
     packets = list(decode.parse_packets(io.BytesIO(primary_bytes)))
     primary, user_id, signature = packets[:3]
 
     data_to_sign = primary['_to_hash'] + subkey.data_to_hash()
 
     if subkey.ecdh:
         embedded_sig = None
```

### Comparing `lib-agent-1.0.5/libagent/gpg/keyring.py` & `lib-agent-1.0.6/libagent/gpg/keyring.py`

 * *Files identical despite different names*

### Comparing `lib-agent-1.0.5/libagent/gpg/protocol.py` & `lib-agent-1.0.6/libagent/gpg/protocol.py`

 * *Files identical despite different names*

### Comparing `lib-agent-1.0.5/libagent/server.py` & `lib-agent-1.0.6/libagent/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,15 +130,15 @@
         try:
             conn = retry(accept_connection, socket.timeout, quit_event)
         except StopIteration:
             log.debug('server stopped')
             break
         # Handle connections from SSH concurrently.
         threading.Thread(target=handle_conn,
-                         kwargs=dict(conn=conn)).start()
+                         kwargs={'conn': conn}).start()
     log.debug('server thread stopped')
 
 
 @contextlib.contextmanager
 def spawn(func, kwargs):
     """Spawn a thread, and join it after the context is over."""
     t = threading.Thread(target=func, kwargs=kwargs)
```

### Comparing `lib-agent-1.0.5/libagent/signify/__init__.py` & `lib-agent-1.0.6/libagent/signify/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""TREZOR support for Ed25519 signify signatures."""
+"""TREZOR support for Ed25519 signify/minisign signatures."""
 
 import argparse
 import binascii
 import contextlib
 import functools
 import hashlib
 import logging
@@ -49,44 +49,61 @@
             sig, pubkey = self.device.sign_with_pubkey(blob=data, identity=identity)
             assert len(sig) == 64
             assert len(pubkey) == 33
             assert pubkey[:1] == b"\x00"
             return sig, pubkey[1:]
 
 
-def format_payload(pubkey, data):
+ALG_SIGNIFY = b'Ed'
+ALG_MINISIGN = b'ED'  # prehashes the data before signing
+
+
+def format_payload(pubkey, data, sig_alg):
     """See http://www.openbsd.org/papers/bsdcan-signify.html for details."""
     keynum = hashlib.sha256(pubkey).digest()[:8]
-    return binascii.b2a_base64(b"Ed" + keynum + data).decode("ascii")
+    return binascii.b2a_base64(sig_alg + keynum + data).decode("ascii")
 
 
 def run_pubkey(device_type, args):
     """Export hardware-based Signify public key."""
     util.setup_logging(verbosity=args.verbose)
     log.warning('This Signify tool is still in EXPERIMENTAL mode, '
                 'so please note that the key derivation, API, and features '
                 'may change without backwards compatibility!')
 
     identity = _create_identity(user_id=args.user_id)
     pubkey = Client(device=device_type()).pubkey(identity=identity)
     comment = f'untrusted comment: identity {identity.to_string()}\n'
-    result = comment + format_payload(pubkey=pubkey, data=pubkey)
-    print(result, end="")
+    payload = format_payload(pubkey=pubkey, data=pubkey, sig_alg=ALG_SIGNIFY)
+    print(comment + payload, end="")
 
 
 def run_sign(device_type, args):
-    """Sign an input blob using Ed25519."""
+    """Prehash & sign an input blob using Ed25519."""
     util.setup_logging(verbosity=args.verbose)
     identity = _create_identity(user_id=args.user_id)
-    data = sys.stdin.buffer.read()
-    sig, pubkey = Client(device=device_type()).sign_with_pubkey(identity, data)
-    pubkey_str = format_payload(pubkey=pubkey, data=pubkey)
-    comment = f'untrusted comment: pubkey {pubkey_str}'
-    result = comment + format_payload(pubkey=pubkey, data=sig)
-    print(result, end="")
+
+    data_to_sign = sys.stdin.buffer.read()
+    sig_alg = ALG_SIGNIFY
+    if args.prehash:
+        # See https://github.com/jedisct1/minisign/commit/6e1023d20758b6fdb2a4b697213b0bf608ba4020
+        # Released in https://github.com/jedisct1/minisign/releases/tag/0.6
+        sig_alg = ALG_MINISIGN
+        data_to_sign = hashlib.blake2b(data_to_sign).digest()
+
+    sig, pubkey = Client(device=device_type()).sign_with_pubkey(identity, data_to_sign)
+    pubkey_str = format_payload(pubkey=pubkey, data=pubkey, sig_alg=sig_alg)
+    sig_str = format_payload(pubkey=pubkey, data=sig, sig_alg=sig_alg)
+    untrusted_comment = f'untrusted comment: pubkey {pubkey_str}'
+    print(untrusted_comment + sig_str, end="")
+
+    comment_to_sign = sig + args.comment.encode()
+    sig, _ = Client(device=device_type()).sign_with_pubkey(identity, comment_to_sign)
+    sig_str = binascii.b2a_base64(sig).decode("ascii")
+    print(f'trusted comment: {args.comment}\n' + sig_str, end="")
 
 
 def main(device_type):
     """Parse command-line arguments."""
     parser = argparse.ArgumentParser()
 
     subparsers = parser.add_subparsers(title='Action', dest='action')
@@ -96,14 +113,16 @@
     p.add_argument('user_id')
     p.add_argument('-v', '--verbose', default=0, action='count')
     p.set_defaults(func=run_pubkey)
 
     p = subparsers.add_parser('sign')
     p.add_argument('user_id')
     p.add_argument('-v', '--verbose', default=0, action='count')
+    p.add_argument('-c', '--comment', default=time.asctime())
+    p.add_argument('-H', '--prehash', default=False, action='store_true')
     p.set_defaults(func=run_sign)
 
     args = parser.parse_args()
     device_type.ui = ui.UI(device_type=device_type, config=vars(args))
     device_type.ui.cached_passphrase_ack = util.ExpiringCache(seconds=float(60))
 
     return args.func(device_type=device_type, args=args)
```

### Comparing `lib-agent-1.0.5/libagent/ssh/__init__.py` & `lib-agent-1.0.6/libagent/ssh/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,17 +146,17 @@
     device_mutex = threading.Lock()
     with server.unix_domain_socket_server(sock_path) as sock:
         sock.settimeout(timeout)
         quit_event = threading.Event()
         handle_conn = functools.partial(server.handle_connection,
                                         handler=handler,
                                         mutex=device_mutex)
-        kwargs = dict(sock=sock,
-                      handle_conn=handle_conn,
-                      quit_event=quit_event)
+        kwargs = {'sock': sock,
+                  'handle_conn': handle_conn,
+                  'quit_event': quit_event}
         with server.spawn(server.server_thread, kwargs):
             try:
                 yield environ
             finally:
                 log.debug('closing server')
                 quit_event.set()
```

### Comparing `lib-agent-1.0.5/libagent/ssh/client.py` & `lib-agent-1.0.6/libagent/ssh/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,14 +29,15 @@
                 pubkeys.append(pubkey)
         return pubkeys
 
     def sign_ssh_challenge(self, blob, identity):
         """Sign given blob using a private key on the device."""
         log.debug('blob: %r', blob)
         msg = parse_ssh_blob(blob)
+        log.debug('parsed blob: %r', msg)
         if msg['sshsig']:
             log.info('please confirm "%s" signature for "%s" using %s...',
                      msg['namespace'], identity.to_string(), self.device)
         else:
             log.debug('%s: user %r via %r (%r)',
                       msg['conn'], msg['user'], msg['auth'], msg['key_type'])
             log.debug('nonce: %r', msg['nonce'])
@@ -64,14 +65,16 @@
         i = io.BytesIO(data[6:])
         # https://github.com/openssh/openssh-portable/blob/master/PROTOCOL.sshsig
         res['sshsig'] = True
         res['namespace'] = util.read_frame(i)
         res['reserved'] = util.read_frame(i)
         res['hashalg'] = util.read_frame(i)
         res['message'] = util.read_frame(i)
+        res['user'] = b'SSHSIG' # logging statements in client.py expect this to be there and raise without it
+        res['key_type'] = res['hashalg'] # logging statements in client.py expect this to be there and raise without it
     else:
         i = io.BytesIO(data)
         res['sshsig'] = False
         res['nonce'] = util.read_frame(i)
         i.read(1)  # SSH2_MSG_USERAUTH_REQUEST == 50 (from ssh2.h, line 108)
         res['user'] = util.read_frame(i)
         res['conn'] = util.read_frame(i)
```

### Comparing `lib-agent-1.0.5/libagent/ssh/protocol.py` & `lib-agent-1.0.6/libagent/ssh/protocol.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,41 +12,41 @@
 
 from . import formats, util
 
 log = logging.getLogger(__name__)
 
 
 # Taken from https://github.com/openssh/openssh-portable/blob/master/authfd.h
-COMMANDS = dict(
-    SSH_AGENTC_REQUEST_RSA_IDENTITIES=1,
-    SSH_AGENT_RSA_IDENTITIES_ANSWER=2,
-    SSH_AGENTC_RSA_CHALLENGE=3,
-    SSH_AGENT_RSA_RESPONSE=4,
-    SSH_AGENT_FAILURE=5,
-    SSH_AGENT_SUCCESS=6,
-    SSH_AGENTC_ADD_RSA_IDENTITY=7,
-    SSH_AGENTC_REMOVE_RSA_IDENTITY=8,
-    SSH_AGENTC_REMOVE_ALL_RSA_IDENTITIES=9,
-    SSH2_AGENTC_REQUEST_IDENTITIES=11,
-    SSH2_AGENT_IDENTITIES_ANSWER=12,
-    SSH2_AGENTC_SIGN_REQUEST=13,
-    SSH2_AGENT_SIGN_RESPONSE=14,
-    SSH2_AGENTC_ADD_IDENTITY=17,
-    SSH2_AGENTC_REMOVE_IDENTITY=18,
-    SSH2_AGENTC_REMOVE_ALL_IDENTITIES=19,
-    SSH_AGENTC_ADD_SMARTCARD_KEY=20,
-    SSH_AGENTC_REMOVE_SMARTCARD_KEY=21,
-    SSH_AGENTC_LOCK=22,
-    SSH_AGENTC_UNLOCK=23,
-    SSH_AGENTC_ADD_RSA_ID_CONSTRAINED=24,
-    SSH2_AGENTC_ADD_ID_CONSTRAINED=25,
-    SSH_AGENTC_ADD_SMARTCARD_KEY_CONSTRAINED=26,
-    SSH_AGENTC_EXTENSION=27,
-    SSH_AGENT_EXTENSION_FAILURE=28,
-)
+COMMANDS = {
+    "SSH_AGENTC_REQUEST_RSA_IDENTITIES": 1,
+    "SSH_AGENT_RSA_IDENTITIES_ANSWER": 2,
+    "SSH_AGENTC_RSA_CHALLENGE": 3,
+    "SSH_AGENT_RSA_RESPONSE": 4,
+    "SSH_AGENT_FAILURE": 5,
+    "SSH_AGENT_SUCCESS": 6,
+    "SSH_AGENTC_ADD_RSA_IDENTITY": 7,
+    "SSH_AGENTC_REMOVE_RSA_IDENTITY": 8,
+    "SSH_AGENTC_REMOVE_ALL_RSA_IDENTITIES": 9,
+    "SSH2_AGENTC_REQUEST_IDENTITIES": 11,
+    "SSH2_AGENT_IDENTITIES_ANSWER": 12,
+    "SSH2_AGENTC_SIGN_REQUEST": 13,
+    "SSH2_AGENT_SIGN_RESPONSE": 14,
+    "SSH2_AGENTC_ADD_IDENTITY": 17,
+    "SSH2_AGENTC_REMOVE_IDENTITY": 18,
+    "SSH2_AGENTC_REMOVE_ALL_IDENTITIES": 19,
+    "SSH_AGENTC_ADD_SMARTCARD_KEY": 20,
+    "SSH_AGENTC_REMOVE_SMARTCARD_KEY": 21,
+    "SSH_AGENTC_LOCK": 22,
+    "SSH_AGENTC_UNLOCK": 23,
+    "SSH_AGENTC_ADD_RSA_ID_CONSTRAINED": 24,
+    "SSH2_AGENTC_ADD_ID_CONSTRAINED": 25,
+    "SSH_AGENTC_ADD_SMARTCARD_KEY_CONSTRAINED": 26,
+    "SSH_AGENTC_EXTENSION": 27,
+    "SSH_AGENT_EXTENSION_FAILURE": 28,
+}
 
 
 def msg_code(name):
     """Convert string name into a integer message code."""
     return COMMANDS[name]
 
 
@@ -170,10 +170,10 @@
                 data = util.frame(util.frame(b'rsa-sha2-256'), util.frame(sig_bytes))
         else:
             data = util.frame(util.frame(key['type']), util.frame(sig_bytes))
         code = util.pack('B', msg_code('SSH2_AGENT_SIGN_RESPONSE'))
         return util.frame(code, data)
 
 
-def _unsupported_extension(buf):
+def _unsupported_extension(buf):  # pylint: disable=unused-argument
     code = util.pack('B', msg_code('SSH_AGENT_EXTENSION_FAILURE'))
     return util.frame(code)
```

### Comparing `lib-agent-1.0.5/libagent/util.py` & `lib-agent-1.0.6/libagent/util.py`

 * *Files identical despite different names*

### Comparing `lib-agent-1.0.5/setup.py` & `lib-agent-1.0.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='lib-agent',
-    version='1.0.5',
+    version='1.0.6',
     description='Using OnlyKey as hardware SSH and GPG agent',
     author='CryptoTrust',
     author_email='admin@crp.to',
-    url='http://github.com/onlykey/onlykey-agent',
+    url='https://github.com/onlykey/lib-agent',
     packages=[
         'libagent',
         'libagent.age',
         'libagent.device',
         'libagent.gpg',
         'libagent.signify',
         'libagent.ssh',
```

