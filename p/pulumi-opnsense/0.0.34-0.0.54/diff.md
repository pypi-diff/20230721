# Comparing `tmp/pulumi-opnsense-.tar.gz` & `tmp/pulumi-opnsense-v0.0.54.tar.gz`

## Comparing `pulumi-opnsense-.tar` & `pulumi-opnsense-v0.0.54.tar`

### file list

```diff
@@ -1,43 +1,49 @@
-drwx------   0 runner    (1001) docker     (123)        0 2023-07-17 11:31:52.000000 ./
-drwx------   0 runner    (1001) docker     (123)        0 2023-07-17 11:31:53.000000 ./bin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:31:53.000000 ./bin/pulumi_opnsense.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-07-17 11:31:53.000000 ./bin/pulumi_opnsense.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 11:31:53.000000 ./bin/pulumi_opnsense.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-17 11:31:53.000000 ./bin/pulumi_opnsense.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-17 11:31:53.000000 ./bin/pulumi_opnsense.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-17 11:31:53.000000 ./bin/pulumi_opnsense.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 11:31:53.000000 ./bin/pulumi_opnsense.egg-info/dependency_links.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:31:53.000000 ./bin/build/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:31:53.000000 ./bin/build/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:31:53.000000 ./bin/build/lib/pulumi_opnsense/
--rw-------   0 runner    (1001) docker     (123)        0 2023-07-17 11:31:52.000000 ./bin/build/lib/pulumi_opnsense/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-07-17 11:31:52.000000 ./bin/build/lib/pulumi_opnsense/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4539 2023-07-17 11:31:52.000000 ./bin/build/lib/pulumi_opnsense/host_override.py
--rw-r--r--   0 runner    (1001) docker     (123)     8047 2023-07-17 11:31:52.000000 ./bin/build/lib/pulumi_opnsense/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-17 11:31:52.000000 ./bin/build/lib/pulumi_opnsense/__init__.py
--rw-------   0 runner    (1001) docker     (123)       45 2023-07-17 11:31:52.000000 ./bin/build/lib/pulumi_opnsense/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)     4425 2023-07-17 11:31:52.000000 ./bin/build/lib/pulumi_opnsense/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-07-17 11:31:52.000000 ./bin/README.md
--rw-------   0 runner    (1001) docker     (123)     1809 2023-07-17 11:31:52.000000 ./bin/setup.py
-drwx------   0 runner    (1001) docker     (123)        0 2023-07-17 11:31:52.000000 ./bin/pulumi_opnsense/
--rw-------   0 runner    (1001) docker     (123)        0 2023-07-17 11:31:52.000000 ./bin/pulumi_opnsense/py.typed
--rw-------   0 runner    (1001) docker     (123)     2722 2023-07-17 11:31:52.000000 ./bin/pulumi_opnsense/provider.py
--rw-------   0 runner    (1001) docker     (123)        0 2023-07-17 11:31:52.000000 ./bin/pulumi_opnsense/README.md
--rw-------   0 runner    (1001) docker     (123)     4539 2023-07-17 11:31:52.000000 ./bin/pulumi_opnsense/host_override.py
--rw-------   0 runner    (1001) docker     (123)     8047 2023-07-17 11:31:52.000000 ./bin/pulumi_opnsense/_utilities.py
--rw-------   0 runner    (1001) docker     (123)      696 2023-07-17 11:31:52.000000 ./bin/pulumi_opnsense/__init__.py
--rw-------   0 runner    (1001) docker     (123)       45 2023-07-17 11:31:52.000000 ./bin/pulumi_opnsense/pulumi-plugin.json
--rw-------   0 runner    (1001) docker     (123)     4425 2023-07-17 11:31:52.000000 ./bin/pulumi_opnsense/random.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:31:53.000000 ./bin/dist/
--rw-r--r--   0 runner    (1001) docker     (123)     8826 2023-07-17 11:31:53.000000 ./bin/dist/pulumi_opnsense-0.0.34.tar.gz
--rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-07-17 11:31:50.000000 ./README.md
--rw-------   0 runner    (1001) docker     (123)     1807 2023-07-17 11:31:49.000000 ./setup.py
-drwx------   0 runner    (1001) docker     (123)        0 2023-07-17 11:31:49.000000 ./pulumi_opnsense/
--rw-------   0 runner    (1001) docker     (123)        0 2023-07-17 11:31:49.000000 ./pulumi_opnsense/py.typed
--rw-------   0 runner    (1001) docker     (123)     2722 2023-07-17 11:31:49.000000 ./pulumi_opnsense/provider.py
--rw-------   0 runner    (1001) docker     (123)        0 2023-07-17 11:31:49.000000 ./pulumi_opnsense/README.md
--rw-------   0 runner    (1001) docker     (123)     4539 2023-07-17 11:31:49.000000 ./pulumi_opnsense/host_override.py
--rw-------   0 runner    (1001) docker     (123)     8047 2023-07-17 11:31:49.000000 ./pulumi_opnsense/_utilities.py
--rw-------   0 runner    (1001) docker     (123)      696 2023-07-17 11:31:49.000000 ./pulumi_opnsense/__init__.py
--rw-------   0 runner    (1001) docker     (123)       45 2023-07-17 11:31:49.000000 ./pulumi_opnsense/pulumi-plugin.json
--rw-------   0 runner    (1001) docker     (123)     4425 2023-07-17 11:31:49.000000 ./pulumi_opnsense/random.py
+drwx------   0 runner    (1001) docker     (123)        0 2023-07-21 10:52:40.000000 ./
+drwx------   0 runner    (1001) docker     (123)        0 2023-07-21 10:52:40.000000 ./bin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:52:40.000000 ./bin/pulumi_opnsense.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-07-21 10:52:40.000000 ./bin/pulumi_opnsense.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 10:52:40.000000 ./bin/pulumi_opnsense.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-21 10:52:40.000000 ./bin/pulumi_opnsense.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-07-21 10:52:40.000000 ./bin/pulumi_opnsense.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-21 10:52:40.000000 ./bin/pulumi_opnsense.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 10:52:40.000000 ./bin/pulumi_opnsense.egg-info/dependency_links.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:52:40.000000 ./bin/build/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:52:40.000000 ./bin/build/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:52:40.000000 ./bin/build/lib/pulumi_opnsense/
+-rw-------   0 runner    (1001) docker     (123)        0 2023-07-21 10:52:40.000000 ./bin/build/lib/pulumi_opnsense/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:52:40.000000 ./bin/build/lib/pulumi_opnsense/unbound/
+-rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-07-21 10:52:40.000000 ./bin/build/lib/pulumi_opnsense/unbound/host_alias.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9983 2023-07-21 10:52:40.000000 ./bin/build/lib/pulumi_opnsense/unbound/host_override.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-21 10:52:40.000000 ./bin/build/lib/pulumi_opnsense/unbound/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-07-21 10:52:40.000000 ./bin/build/lib/pulumi_opnsense/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8097 2023-07-21 10:52:40.000000 ./bin/build/lib/pulumi_opnsense/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-07-21 10:52:40.000000 ./bin/build/lib/pulumi_opnsense/__init__.py
+-rw-------   0 runner    (1001) docker     (123)      113 2023-07-21 10:52:40.000000 ./bin/build/lib/pulumi_opnsense/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-07-21 10:52:40.000000 ./bin/README.md
+-rw-------   0 runner    (1001) docker     (123)     1877 2023-07-21 10:52:40.000000 ./bin/setup.py
+drwx------   0 runner    (1001) docker     (123)        0 2023-07-21 10:52:40.000000 ./bin/pulumi_opnsense/
+-rw-------   0 runner    (1001) docker     (123)        0 2023-07-21 10:52:40.000000 ./bin/pulumi_opnsense/py.typed
+drwx------   0 runner    (1001) docker     (123)        0 2023-07-21 10:52:40.000000 ./bin/pulumi_opnsense/unbound/
+-rw-------   0 runner    (1001) docker     (123)     4485 2023-07-21 10:52:40.000000 ./bin/pulumi_opnsense/unbound/host_alias.py
+-rw-------   0 runner    (1001) docker     (123)     9983 2023-07-21 10:52:40.000000 ./bin/pulumi_opnsense/unbound/host_override.py
+-rw-------   0 runner    (1001) docker     (123)      290 2023-07-21 10:52:40.000000 ./bin/pulumi_opnsense/unbound/__init__.py
+-rw-------   0 runner    (1001) docker     (123)     2722 2023-07-21 10:52:40.000000 ./bin/pulumi_opnsense/provider.py
+-rw-------   0 runner    (1001) docker     (123)        0 2023-07-21 10:52:40.000000 ./bin/pulumi_opnsense/README.md
+-rw-------   0 runner    (1001) docker     (123)     8097 2023-07-21 10:52:40.000000 ./bin/pulumi_opnsense/_utilities.py
+-rw-------   0 runner    (1001) docker     (123)      864 2023-07-21 10:52:40.000000 ./bin/pulumi_opnsense/__init__.py
+-rw-------   0 runner    (1001) docker     (123)      113 2023-07-21 10:52:40.000000 ./bin/pulumi_opnsense/pulumi-plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:52:40.000000 ./bin/dist/
+-rw-r--r--   0 runner    (1001) docker     (123)     9705 2023-07-21 10:52:40.000000 ./bin/dist/pulumi_opnsense-0.0.54.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-07-21 10:52:37.000000 ./README.md
+-rw-------   0 runner    (1001) docker     (123)     1875 2023-07-21 10:52:37.000000 ./setup.py
+drwx------   0 runner    (1001) docker     (123)        0 2023-07-21 10:52:37.000000 ./pulumi_opnsense/
+-rw-------   0 runner    (1001) docker     (123)        0 2023-07-21 10:52:37.000000 ./pulumi_opnsense/py.typed
+drwx------   0 runner    (1001) docker     (123)        0 2023-07-21 10:52:37.000000 ./pulumi_opnsense/unbound/
+-rw-------   0 runner    (1001) docker     (123)     4485 2023-07-21 10:52:37.000000 ./pulumi_opnsense/unbound/host_alias.py
+-rw-------   0 runner    (1001) docker     (123)     9983 2023-07-21 10:52:37.000000 ./pulumi_opnsense/unbound/host_override.py
+-rw-------   0 runner    (1001) docker     (123)      290 2023-07-21 10:52:37.000000 ./pulumi_opnsense/unbound/__init__.py
+-rw-------   0 runner    (1001) docker     (123)     2722 2023-07-21 10:52:37.000000 ./pulumi_opnsense/provider.py
+-rw-------   0 runner    (1001) docker     (123)        0 2023-07-21 10:52:37.000000 ./pulumi_opnsense/README.md
+-rw-------   0 runner    (1001) docker     (123)     8097 2023-07-21 10:52:37.000000 ./pulumi_opnsense/_utilities.py
+-rw-------   0 runner    (1001) docker     (123)      864 2023-07-21 10:52:37.000000 ./pulumi_opnsense/__init__.py
+-rw-------   0 runner    (1001) docker     (123)      113 2023-07-21 10:52:37.000000 ./pulumi_opnsense/pulumi-plugin.json
```

### ./bin/pulumi_opnsense.egg-info/PKG-INFO

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-opnsense
-Version: 0.0.34
+Version: 0.0.54
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # Pulumi Native Provider Boilerplate
 
 This repository is a boilerplate showing how to create a native Pulumi provider.
```

### ./bin/pulumi_opnsense.egg-info/SOURCES.txt

```diff
@@ -1,15 +1,16 @@
 README.md
 setup.py
 pulumi_opnsense/__init__.py
 pulumi_opnsense/_utilities.py
-pulumi_opnsense/host_override.py
 pulumi_opnsense/provider.py
 pulumi_opnsense/pulumi-plugin.json
 pulumi_opnsense/py.typed
-pulumi_opnsense/random.py
 pulumi_opnsense.egg-info/PKG-INFO
 pulumi_opnsense.egg-info/SOURCES.txt
 pulumi_opnsense.egg-info/dependency_links.txt
 pulumi_opnsense.egg-info/not-zip-safe
 pulumi_opnsense.egg-info/requires.txt
-pulumi_opnsense.egg-info/top_level.txt
+pulumi_opnsense.egg-info/top_level.txt
+pulumi_opnsense/unbound/__init__.py
+pulumi_opnsense/unbound/host_alias.py
+pulumi_opnsense/unbound/host_override.py
```

### ./bin/build/lib/pulumi_opnsense/_utilities.py

```diff
@@ -243,8 +243,8 @@
         }).apply(lambda resolved_args: func(*resolved_args['args'],
                                             opts=opts,
                                             **resolved_args['kwargs']))
 
     return (lambda _: lifted_func)
 
 def get_plugin_download_url():
-	return None
+	return "github://api.github.com/oss4u/pulumi-opnsense-native"
```

### ./bin/build/lib/pulumi_opnsense/__init__.py

```diff
@@ -1,27 +1,33 @@
 # coding=utf-8
 # *** WARNING: this file was generated by pulumi. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
 from . import _utilities
 import typing
 # Export this package's modules as members:
-from .host_override import *
 from .provider import *
-from .random import *
+
+# Make subpackages available:
+if typing.TYPE_CHECKING:
+    import pulumi_opnsense.unbound as __unbound
+    unbound = __unbound
+else:
+    unbound = _utilities.lazy_import('pulumi_opnsense.unbound')
+
 _utilities.register(
     resource_modules="""
 [
  {
   "pkg": "opnsense",
-  "mod": "index",
-  "fqn": "pulumi_opnsense",
+  "mod": "unbound",
+  "fqn": "pulumi_opnsense.unbound",
   "classes": {
-   "opnsense:index:HostOverride": "HostOverride",
-   "opnsense:index:Random": "Random"
+   "opnsense:unbound:HostAlias": "HostAlias",
+   "opnsense:unbound:HostOverride": "HostOverride"
   }
  }
 ]
 """,
     resource_packages="""
 [
  {
```

### ./bin/build/lib/pulumi_opnsense/pulumi-plugin.json

#### Pretty-printed

 * *Similarity: 0.6666666666666666%*

 * *Differences: {"'server'": "'github://api.github.com/oss4u/pulumi-opnsense-native'"}*

```diff
@@ -1,4 +1,5 @@
 {
     "name": "opnsense",
-    "resource": true
+    "resource": true,
+    "server": "github://api.github.com/oss4u/pulumi-opnsense-native"
 }
```

### ./bin/setup.py

```diff
@@ -4,22 +4,22 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.0.34"
-PLUGIN_VERSION = "0.0.34"
+VERSION = "0.0.54"
+PLUGIN_VERSION = "0.0.54"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
-            check_call(['pulumi', 'plugin', 'install', 'resource', 'opnsense', PLUGIN_VERSION])
+            check_call(['pulumi', 'plugin', 'install', 'resource', 'opnsense', PLUGIN_VERSION, '--server', 'github://api.github.com/oss4u/pulumi-opnsense-native'])
         except OSError as error:
             if error.errno == errno.ENOENT:
                 print(f"""
                 There was an error installing the opnsense resource provider plugin.
                 It looks like `pulumi` is not installed on your system.
                 Please visit https://pulumi.com/ to install the Pulumi CLI.
                 You may try manually installing the plugin by running
```

### ./bin/pulumi_opnsense/_utilities.py

```diff
@@ -243,8 +243,8 @@
         }).apply(lambda resolved_args: func(*resolved_args['args'],
                                             opts=opts,
                                             **resolved_args['kwargs']))
 
     return (lambda _: lifted_func)
 
 def get_plugin_download_url():
-	return None
+	return "github://api.github.com/oss4u/pulumi-opnsense-native"
```

### ./bin/pulumi_opnsense/__init__.py

```diff
@@ -1,27 +1,33 @@
 # coding=utf-8
 # *** WARNING: this file was generated by pulumi. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
 from . import _utilities
 import typing
 # Export this package's modules as members:
-from .host_override import *
 from .provider import *
-from .random import *
+
+# Make subpackages available:
+if typing.TYPE_CHECKING:
+    import pulumi_opnsense.unbound as __unbound
+    unbound = __unbound
+else:
+    unbound = _utilities.lazy_import('pulumi_opnsense.unbound')
+
 _utilities.register(
     resource_modules="""
 [
  {
   "pkg": "opnsense",
-  "mod": "index",
-  "fqn": "pulumi_opnsense",
+  "mod": "unbound",
+  "fqn": "pulumi_opnsense.unbound",
   "classes": {
-   "opnsense:index:HostOverride": "HostOverride",
-   "opnsense:index:Random": "Random"
+   "opnsense:unbound:HostAlias": "HostAlias",
+   "opnsense:unbound:HostOverride": "HostOverride"
   }
  }
 ]
 """,
     resource_packages="""
 [
  {
```

### ./bin/pulumi_opnsense/pulumi-plugin.json

#### Pretty-printed

 * *Similarity: 0.6666666666666666%*

 * *Differences: {"'server'": "'github://api.github.com/oss4u/pulumi-opnsense-native'"}*

```diff
@@ -1,4 +1,5 @@
 {
     "name": "opnsense",
-    "resource": true
+    "resource": true,
+    "server": "github://api.github.com/oss4u/pulumi-opnsense-native"
 }
```

### ./setup.py

```diff
@@ -11,15 +11,15 @@
 VERSION = "0.0.0"
 PLUGIN_VERSION = "0.0.0"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
-            check_call(['pulumi', 'plugin', 'install', 'resource', 'opnsense', PLUGIN_VERSION])
+            check_call(['pulumi', 'plugin', 'install', 'resource', 'opnsense', PLUGIN_VERSION, '--server', 'github://api.github.com/oss4u/pulumi-opnsense-native'])
         except OSError as error:
             if error.errno == errno.ENOENT:
                 print(f"""
                 There was an error installing the opnsense resource provider plugin.
                 It looks like `pulumi` is not installed on your system.
                 Please visit https://pulumi.com/ to install the Pulumi CLI.
                 You may try manually installing the plugin by running
```

### ./pulumi_opnsense/_utilities.py

```diff
@@ -243,8 +243,8 @@
         }).apply(lambda resolved_args: func(*resolved_args['args'],
                                             opts=opts,
                                             **resolved_args['kwargs']))
 
     return (lambda _: lifted_func)
 
 def get_plugin_download_url():
-	return None
+	return "github://api.github.com/oss4u/pulumi-opnsense-native"
```

### ./pulumi_opnsense/__init__.py

```diff
@@ -1,27 +1,33 @@
 # coding=utf-8
 # *** WARNING: this file was generated by pulumi. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
 from . import _utilities
 import typing
 # Export this package's modules as members:
-from .host_override import *
 from .provider import *
-from .random import *
+
+# Make subpackages available:
+if typing.TYPE_CHECKING:
+    import pulumi_opnsense.unbound as __unbound
+    unbound = __unbound
+else:
+    unbound = _utilities.lazy_import('pulumi_opnsense.unbound')
+
 _utilities.register(
     resource_modules="""
 [
  {
   "pkg": "opnsense",
-  "mod": "index",
-  "fqn": "pulumi_opnsense",
+  "mod": "unbound",
+  "fqn": "pulumi_opnsense.unbound",
   "classes": {
-   "opnsense:index:HostOverride": "HostOverride",
-   "opnsense:index:Random": "Random"
+   "opnsense:unbound:HostAlias": "HostAlias",
+   "opnsense:unbound:HostOverride": "HostOverride"
   }
  }
 ]
 """,
     resource_packages="""
 [
  {
```

### ./pulumi_opnsense/pulumi-plugin.json

#### Pretty-printed

 * *Similarity: 0.6666666666666666%*

 * *Differences: {"'server'": "'github://api.github.com/oss4u/pulumi-opnsense-native'"}*

```diff
@@ -1,4 +1,5 @@
 {
     "name": "opnsense",
-    "resource": true
+    "resource": true,
+    "server": "github://api.github.com/oss4u/pulumi-opnsense-native"
 }
```

### Comparing `./bin/build/lib/pulumi_opnsense/host_override.py` & `./bin/build/lib/pulumi_opnsense/unbound/host_alias.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,64 +3,64 @@
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
-from . import _utilities
+from .. import _utilities
 
-__all__ = ['HostOverrideArgs', 'HostOverride']
+__all__ = ['HostAliasArgs', 'HostAlias']
 
 @pulumi.input_type
-class HostOverrideArgs:
+class HostAliasArgs:
     def __init__(__self__, *,
                  length: pulumi.Input[int]):
         """
-        The set of arguments for constructing a HostOverride resource.
+        The set of arguments for constructing a HostAlias resource.
         """
         pulumi.set(__self__, "length", length)
 
     @property
     @pulumi.getter
     def length(self) -> pulumi.Input[int]:
         return pulumi.get(self, "length")
 
     @length.setter
     def length(self, value: pulumi.Input[int]):
         pulumi.set(self, "length", value)
 
 
-class HostOverride(pulumi.CustomResource):
+class HostAlias(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  length: Optional[pulumi.Input[int]] = None,
                  __props__=None):
         """
-        Create a HostOverride resource with the given unique name, props, and options.
+        Create a HostAlias resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: HostOverrideArgs,
+                 args: HostAliasArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Create a HostOverride resource with the given unique name, props, and options.
+        Create a HostAlias resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
-        :param HostOverrideArgs args: The arguments to use to populate this resource's properties.
+        :param HostAliasArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(HostOverrideArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(HostAliasArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
@@ -69,45 +69,45 @@
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = HostOverrideArgs.__new__(HostOverrideArgs)
+            __props__ = HostAliasArgs.__new__(HostAliasArgs)
 
             if length is None and not opts.urn:
                 raise TypeError("Missing required property 'length'")
             __props__.__dict__["length"] = length
             __props__.__dict__["result"] = None
-        super(HostOverride, __self__).__init__(
-            'opnsense:index:HostOverride',
+        super(HostAlias, __self__).__init__(
+            'opnsense:unbound:HostAlias',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
-            opts: Optional[pulumi.ResourceOptions] = None) -> 'HostOverride':
+            opts: Optional[pulumi.ResourceOptions] = None) -> 'HostAlias':
         """
-        Get an existing HostOverride resource's state with the given name, id, and optional extra
+        Get an existing HostAlias resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = HostOverrideArgs.__new__(HostOverrideArgs)
+        __props__ = HostAliasArgs.__new__(HostAliasArgs)
 
         __props__.__dict__["length"] = None
         __props__.__dict__["result"] = None
-        return HostOverride(resource_name, opts=opts, __props__=__props__)
+        return HostAlias(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter
     def length(self) -> pulumi.Output[int]:
         return pulumi.get(self, "length")
 
     @property
```

### Comparing `./bin/build/lib/pulumi_opnsense/random.py` & `./bin/pulumi_opnsense/unbound/host_alias.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,64 +3,64 @@
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
-from . import _utilities
+from .. import _utilities
 
-__all__ = ['RandomArgs', 'Random']
+__all__ = ['HostAliasArgs', 'HostAlias']
 
 @pulumi.input_type
-class RandomArgs:
+class HostAliasArgs:
     def __init__(__self__, *,
                  length: pulumi.Input[int]):
         """
-        The set of arguments for constructing a Random resource.
+        The set of arguments for constructing a HostAlias resource.
         """
         pulumi.set(__self__, "length", length)
 
     @property
     @pulumi.getter
     def length(self) -> pulumi.Input[int]:
         return pulumi.get(self, "length")
 
     @length.setter
     def length(self, value: pulumi.Input[int]):
         pulumi.set(self, "length", value)
 
 
-class Random(pulumi.CustomResource):
+class HostAlias(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  length: Optional[pulumi.Input[int]] = None,
                  __props__=None):
         """
-        Create a Random resource with the given unique name, props, and options.
+        Create a HostAlias resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: RandomArgs,
+                 args: HostAliasArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Create a Random resource with the given unique name, props, and options.
+        Create a HostAlias resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
-        :param RandomArgs args: The arguments to use to populate this resource's properties.
+        :param HostAliasArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(RandomArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(HostAliasArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
@@ -69,45 +69,45 @@
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = RandomArgs.__new__(RandomArgs)
+            __props__ = HostAliasArgs.__new__(HostAliasArgs)
 
             if length is None and not opts.urn:
                 raise TypeError("Missing required property 'length'")
             __props__.__dict__["length"] = length
             __props__.__dict__["result"] = None
-        super(Random, __self__).__init__(
-            'opnsense:index:Random',
+        super(HostAlias, __self__).__init__(
+            'opnsense:unbound:HostAlias',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
-            opts: Optional[pulumi.ResourceOptions] = None) -> 'Random':
+            opts: Optional[pulumi.ResourceOptions] = None) -> 'HostAlias':
         """
-        Get an existing Random resource's state with the given name, id, and optional extra
+        Get an existing HostAlias resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = RandomArgs.__new__(RandomArgs)
+        __props__ = HostAliasArgs.__new__(HostAliasArgs)
 
         __props__.__dict__["length"] = None
         __props__.__dict__["result"] = None
-        return Random(resource_name, opts=opts, __props__=__props__)
+        return HostAlias(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter
     def length(self) -> pulumi.Output[int]:
         return pulumi.get(self, "length")
 
     @property
```

### Comparing `./bin/pulumi_opnsense/host_override.py` & `./pulumi_opnsense/unbound/host_alias.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,64 +3,64 @@
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
-from . import _utilities
+from .. import _utilities
 
-__all__ = ['HostOverrideArgs', 'HostOverride']
+__all__ = ['HostAliasArgs', 'HostAlias']
 
 @pulumi.input_type
-class HostOverrideArgs:
+class HostAliasArgs:
     def __init__(__self__, *,
                  length: pulumi.Input[int]):
         """
-        The set of arguments for constructing a HostOverride resource.
+        The set of arguments for constructing a HostAlias resource.
         """
         pulumi.set(__self__, "length", length)
 
     @property
     @pulumi.getter
     def length(self) -> pulumi.Input[int]:
         return pulumi.get(self, "length")
 
     @length.setter
     def length(self, value: pulumi.Input[int]):
         pulumi.set(self, "length", value)
 
 
-class HostOverride(pulumi.CustomResource):
+class HostAlias(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  length: Optional[pulumi.Input[int]] = None,
                  __props__=None):
         """
-        Create a HostOverride resource with the given unique name, props, and options.
+        Create a HostAlias resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: HostOverrideArgs,
+                 args: HostAliasArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Create a HostOverride resource with the given unique name, props, and options.
+        Create a HostAlias resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
-        :param HostOverrideArgs args: The arguments to use to populate this resource's properties.
+        :param HostAliasArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(HostOverrideArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(HostAliasArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
@@ -69,45 +69,45 @@
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = HostOverrideArgs.__new__(HostOverrideArgs)
+            __props__ = HostAliasArgs.__new__(HostAliasArgs)
 
             if length is None and not opts.urn:
                 raise TypeError("Missing required property 'length'")
             __props__.__dict__["length"] = length
             __props__.__dict__["result"] = None
-        super(HostOverride, __self__).__init__(
-            'opnsense:index:HostOverride',
+        super(HostAlias, __self__).__init__(
+            'opnsense:unbound:HostAlias',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
-            opts: Optional[pulumi.ResourceOptions] = None) -> 'HostOverride':
+            opts: Optional[pulumi.ResourceOptions] = None) -> 'HostAlias':
         """
-        Get an existing HostOverride resource's state with the given name, id, and optional extra
+        Get an existing HostAlias resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = HostOverrideArgs.__new__(HostOverrideArgs)
+        __props__ = HostAliasArgs.__new__(HostAliasArgs)
 
         __props__.__dict__["length"] = None
         __props__.__dict__["result"] = None
-        return HostOverride(resource_name, opts=opts, __props__=__props__)
+        return HostAlias(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter
     def length(self) -> pulumi.Output[int]:
         return pulumi.get(self, "length")
 
     @property
```

