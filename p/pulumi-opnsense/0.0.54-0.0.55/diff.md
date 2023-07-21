# Comparing `tmp/pulumi-opnsense-v0.0.54.tar.gz` & `tmp/pulumi-opnsense-v0.0.55.tar.gz`

## Comparing `pulumi-opnsense-v0.0.54.tar` & `pulumi-opnsense-v0.0.55.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwx------   0 runner    (1001) docker     (123)        0 2023-07-21 10:52:40.000000 ./
-drwx------   0 runner    (1001) docker     (123)        0 2023-07-21 10:52:40.000000 ./bin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:52:40.000000 ./bin/pulumi_opnsense.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-07-21 10:52:40.000000 ./bin/pulumi_opnsense.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 10:52:40.000000 ./bin/pulumi_opnsense.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-21 10:52:40.000000 ./bin/pulumi_opnsense.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-07-21 10:52:40.000000 ./bin/pulumi_opnsense.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-21 10:52:40.000000 ./bin/pulumi_opnsense.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 10:52:40.000000 ./bin/pulumi_opnsense.egg-info/dependency_links.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:52:40.000000 ./bin/build/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:52:40.000000 ./bin/build/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:52:40.000000 ./bin/build/lib/pulumi_opnsense/
--rw-------   0 runner    (1001) docker     (123)        0 2023-07-21 10:52:40.000000 ./bin/build/lib/pulumi_opnsense/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:52:40.000000 ./bin/build/lib/pulumi_opnsense/unbound/
--rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-07-21 10:52:40.000000 ./bin/build/lib/pulumi_opnsense/unbound/host_alias.py
--rw-r--r--   0 runner    (1001) docker     (123)     9983 2023-07-21 10:52:40.000000 ./bin/build/lib/pulumi_opnsense/unbound/host_override.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-21 10:52:40.000000 ./bin/build/lib/pulumi_opnsense/unbound/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-07-21 10:52:40.000000 ./bin/build/lib/pulumi_opnsense/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     8097 2023-07-21 10:52:40.000000 ./bin/build/lib/pulumi_opnsense/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-07-21 10:52:40.000000 ./bin/build/lib/pulumi_opnsense/__init__.py
--rw-------   0 runner    (1001) docker     (123)      113 2023-07-21 10:52:40.000000 ./bin/build/lib/pulumi_opnsense/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-07-21 10:52:40.000000 ./bin/README.md
--rw-------   0 runner    (1001) docker     (123)     1877 2023-07-21 10:52:40.000000 ./bin/setup.py
-drwx------   0 runner    (1001) docker     (123)        0 2023-07-21 10:52:40.000000 ./bin/pulumi_opnsense/
--rw-------   0 runner    (1001) docker     (123)        0 2023-07-21 10:52:40.000000 ./bin/pulumi_opnsense/py.typed
-drwx------   0 runner    (1001) docker     (123)        0 2023-07-21 10:52:40.000000 ./bin/pulumi_opnsense/unbound/
--rw-------   0 runner    (1001) docker     (123)     4485 2023-07-21 10:52:40.000000 ./bin/pulumi_opnsense/unbound/host_alias.py
--rw-------   0 runner    (1001) docker     (123)     9983 2023-07-21 10:52:40.000000 ./bin/pulumi_opnsense/unbound/host_override.py
--rw-------   0 runner    (1001) docker     (123)      290 2023-07-21 10:52:40.000000 ./bin/pulumi_opnsense/unbound/__init__.py
--rw-------   0 runner    (1001) docker     (123)     2722 2023-07-21 10:52:40.000000 ./bin/pulumi_opnsense/provider.py
--rw-------   0 runner    (1001) docker     (123)        0 2023-07-21 10:52:40.000000 ./bin/pulumi_opnsense/README.md
--rw-------   0 runner    (1001) docker     (123)     8097 2023-07-21 10:52:40.000000 ./bin/pulumi_opnsense/_utilities.py
--rw-------   0 runner    (1001) docker     (123)      864 2023-07-21 10:52:40.000000 ./bin/pulumi_opnsense/__init__.py
--rw-------   0 runner    (1001) docker     (123)      113 2023-07-21 10:52:40.000000 ./bin/pulumi_opnsense/pulumi-plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:52:40.000000 ./bin/dist/
--rw-r--r--   0 runner    (1001) docker     (123)     9705 2023-07-21 10:52:40.000000 ./bin/dist/pulumi_opnsense-0.0.54.tar.gz
--rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-07-21 10:52:37.000000 ./README.md
--rw-------   0 runner    (1001) docker     (123)     1875 2023-07-21 10:52:37.000000 ./setup.py
-drwx------   0 runner    (1001) docker     (123)        0 2023-07-21 10:52:37.000000 ./pulumi_opnsense/
--rw-------   0 runner    (1001) docker     (123)        0 2023-07-21 10:52:37.000000 ./pulumi_opnsense/py.typed
-drwx------   0 runner    (1001) docker     (123)        0 2023-07-21 10:52:37.000000 ./pulumi_opnsense/unbound/
--rw-------   0 runner    (1001) docker     (123)     4485 2023-07-21 10:52:37.000000 ./pulumi_opnsense/unbound/host_alias.py
--rw-------   0 runner    (1001) docker     (123)     9983 2023-07-21 10:52:37.000000 ./pulumi_opnsense/unbound/host_override.py
--rw-------   0 runner    (1001) docker     (123)      290 2023-07-21 10:52:37.000000 ./pulumi_opnsense/unbound/__init__.py
--rw-------   0 runner    (1001) docker     (123)     2722 2023-07-21 10:52:37.000000 ./pulumi_opnsense/provider.py
--rw-------   0 runner    (1001) docker     (123)        0 2023-07-21 10:52:37.000000 ./pulumi_opnsense/README.md
--rw-------   0 runner    (1001) docker     (123)     8097 2023-07-21 10:52:37.000000 ./pulumi_opnsense/_utilities.py
--rw-------   0 runner    (1001) docker     (123)      864 2023-07-21 10:52:37.000000 ./pulumi_opnsense/__init__.py
--rw-------   0 runner    (1001) docker     (123)      113 2023-07-21 10:52:37.000000 ./pulumi_opnsense/pulumi-plugin.json
+drwx------   0 runner    (1001) docker     (123)        0 2023-07-21 11:46:11.000000 ./
+drwx------   0 runner    (1001) docker     (123)        0 2023-07-21 11:46:11.000000 ./bin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:46:11.000000 ./bin/pulumi_opnsense.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-07-21 11:46:11.000000 ./bin/pulumi_opnsense.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 11:46:11.000000 ./bin/pulumi_opnsense.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-21 11:46:11.000000 ./bin/pulumi_opnsense.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-07-21 11:46:11.000000 ./bin/pulumi_opnsense.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-21 11:46:11.000000 ./bin/pulumi_opnsense.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 11:46:11.000000 ./bin/pulumi_opnsense.egg-info/dependency_links.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:46:11.000000 ./bin/build/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:46:11.000000 ./bin/build/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:46:11.000000 ./bin/build/lib/pulumi_opnsense/
+-rw-------   0 runner    (1001) docker     (123)        0 2023-07-21 11:46:11.000000 ./bin/build/lib/pulumi_opnsense/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:46:11.000000 ./bin/build/lib/pulumi_opnsense/unbound/
+-rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-07-21 11:46:11.000000 ./bin/build/lib/pulumi_opnsense/unbound/host_alias.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9983 2023-07-21 11:46:11.000000 ./bin/build/lib/pulumi_opnsense/unbound/host_override.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-21 11:46:11.000000 ./bin/build/lib/pulumi_opnsense/unbound/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-07-21 11:46:11.000000 ./bin/build/lib/pulumi_opnsense/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8097 2023-07-21 11:46:11.000000 ./bin/build/lib/pulumi_opnsense/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-07-21 11:46:11.000000 ./bin/build/lib/pulumi_opnsense/__init__.py
+-rw-------   0 runner    (1001) docker     (123)      113 2023-07-21 11:46:11.000000 ./bin/build/lib/pulumi_opnsense/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-07-21 11:46:11.000000 ./bin/README.md
+-rw-------   0 runner    (1001) docker     (123)     1877 2023-07-21 11:46:11.000000 ./bin/setup.py
+drwx------   0 runner    (1001) docker     (123)        0 2023-07-21 11:46:11.000000 ./bin/pulumi_opnsense/
+-rw-------   0 runner    (1001) docker     (123)        0 2023-07-21 11:46:11.000000 ./bin/pulumi_opnsense/py.typed
+drwx------   0 runner    (1001) docker     (123)        0 2023-07-21 11:46:11.000000 ./bin/pulumi_opnsense/unbound/
+-rw-------   0 runner    (1001) docker     (123)     4485 2023-07-21 11:46:11.000000 ./bin/pulumi_opnsense/unbound/host_alias.py
+-rw-------   0 runner    (1001) docker     (123)     9983 2023-07-21 11:46:11.000000 ./bin/pulumi_opnsense/unbound/host_override.py
+-rw-------   0 runner    (1001) docker     (123)      290 2023-07-21 11:46:11.000000 ./bin/pulumi_opnsense/unbound/__init__.py
+-rw-------   0 runner    (1001) docker     (123)     2722 2023-07-21 11:46:11.000000 ./bin/pulumi_opnsense/provider.py
+-rw-------   0 runner    (1001) docker     (123)        0 2023-07-21 11:46:11.000000 ./bin/pulumi_opnsense/README.md
+-rw-------   0 runner    (1001) docker     (123)     8097 2023-07-21 11:46:11.000000 ./bin/pulumi_opnsense/_utilities.py
+-rw-------   0 runner    (1001) docker     (123)      864 2023-07-21 11:46:11.000000 ./bin/pulumi_opnsense/__init__.py
+-rw-------   0 runner    (1001) docker     (123)      113 2023-07-21 11:46:11.000000 ./bin/pulumi_opnsense/pulumi-plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:46:11.000000 ./bin/dist/
+-rw-r--r--   0 runner    (1001) docker     (123)     9705 2023-07-21 11:46:11.000000 ./bin/dist/pulumi_opnsense-0.0.55.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-07-21 11:46:10.000000 ./README.md
+-rw-------   0 runner    (1001) docker     (123)     1875 2023-07-21 11:46:10.000000 ./setup.py
+drwx------   0 runner    (1001) docker     (123)        0 2023-07-21 11:46:10.000000 ./pulumi_opnsense/
+-rw-------   0 runner    (1001) docker     (123)        0 2023-07-21 11:46:10.000000 ./pulumi_opnsense/py.typed
+drwx------   0 runner    (1001) docker     (123)        0 2023-07-21 11:46:10.000000 ./pulumi_opnsense/unbound/
+-rw-------   0 runner    (1001) docker     (123)     4485 2023-07-21 11:46:10.000000 ./pulumi_opnsense/unbound/host_alias.py
+-rw-------   0 runner    (1001) docker     (123)     9983 2023-07-21 11:46:10.000000 ./pulumi_opnsense/unbound/host_override.py
+-rw-------   0 runner    (1001) docker     (123)      290 2023-07-21 11:46:10.000000 ./pulumi_opnsense/unbound/__init__.py
+-rw-------   0 runner    (1001) docker     (123)     2722 2023-07-21 11:46:10.000000 ./pulumi_opnsense/provider.py
+-rw-------   0 runner    (1001) docker     (123)        0 2023-07-21 11:46:10.000000 ./pulumi_opnsense/README.md
+-rw-------   0 runner    (1001) docker     (123)     8097 2023-07-21 11:46:10.000000 ./pulumi_opnsense/_utilities.py
+-rw-------   0 runner    (1001) docker     (123)      864 2023-07-21 11:46:10.000000 ./pulumi_opnsense/__init__.py
+-rw-------   0 runner    (1001) docker     (123)      113 2023-07-21 11:46:10.000000 ./pulumi_opnsense/pulumi-plugin.json
```

### ./bin/pulumi_opnsense.egg-info/PKG-INFO

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-opnsense
-Version: 0.0.54
+Version: 0.0.55
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # Pulumi Native Provider Boilerplate
 
 This repository is a boilerplate showing how to create a native Pulumi provider.
```

### ./bin/setup.py

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.0.54"
-PLUGIN_VERSION = "0.0.54"
+VERSION = "0.0.55"
+PLUGIN_VERSION = "0.0.55"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'opnsense', PLUGIN_VERSION, '--server', 'github://api.github.com/oss4u/pulumi-opnsense-native'])
         except OSError as error:
```

