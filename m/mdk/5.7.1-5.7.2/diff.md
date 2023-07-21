# Comparing `tmp/mdk-5.7.1.tar.gz` & `tmp/mdk-5.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdk-5.7.1.tar", last modified: Mon Nov  7 20:33:19 2022, max compression
+gzip compressed data, was "mdk-5.7.2.tar", last modified: Fri Jul 21 17:56:37 2023, max compression
```

## Comparing `mdk-5.7.1.tar` & `mdk-5.7.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 jatin     (1000) jatin     (1000)        0 2022-11-07 20:33:19.162999 mdk-5.7.1/
--rw-rw-r--   0 jatin     (1000) jatin     (1000)     1068 2022-08-11 20:00:25.000000 mdk-5.7.1/LICENSE
--rw-rw-r--   0 jatin     (1000) jatin     (1000)     1410 2022-11-07 20:33:19.162999 mdk-5.7.1/PKG-INFO
--rw-rw-r--   0 jatin     (1000) jatin     (1000)      921 2022-08-11 20:04:56.000000 mdk-5.7.1/README.md
-drwxrwxr-x   0 jatin     (1000) jatin     (1000)        0 2022-11-07 20:33:19.162999 mdk-5.7.1/mdk/
--rw-rw-r--   0 jatin     (1000) jatin     (1000)        0 2022-08-11 20:00:25.000000 mdk-5.7.1/mdk/__init__.py
--rwxrwxr-x   0 jatin     (1000) jatin     (1000)     3608 2022-11-05 01:21:43.000000 mdk-5.7.1/mdk/main.py
--rw-rw-r--   0 jatin     (1000) jatin     (1000)    16555 2022-11-07 20:33:00.000000 mdk-5.7.1/mdk/utils.py
-drwxrwxr-x   0 jatin     (1000) jatin     (1000)        0 2022-11-07 20:33:19.162999 mdk-5.7.1/mdk.egg-info/
--rw-rw-r--   0 jatin     (1000) jatin     (1000)     1410 2022-11-07 20:33:19.000000 mdk-5.7.1/mdk.egg-info/PKG-INFO
--rw-rw-r--   0 jatin     (1000) jatin     (1000)      241 2022-11-07 20:33:19.000000 mdk-5.7.1/mdk.egg-info/SOURCES.txt
--rw-rw-r--   0 jatin     (1000) jatin     (1000)        1 2022-11-07 20:33:19.000000 mdk-5.7.1/mdk.egg-info/dependency_links.txt
--rw-rw-r--   0 jatin     (1000) jatin     (1000)       37 2022-11-07 20:33:19.000000 mdk-5.7.1/mdk.egg-info/entry_points.txt
--rw-rw-r--   0 jatin     (1000) jatin     (1000)        9 2022-11-07 20:33:19.000000 mdk-5.7.1/mdk.egg-info/requires.txt
--rw-rw-r--   0 jatin     (1000) jatin     (1000)        4 2022-11-07 20:33:19.000000 mdk-5.7.1/mdk.egg-info/top_level.txt
--rw-rw-r--   0 jatin     (1000) jatin     (1000)       67 2022-11-07 20:33:19.162999 mdk-5.7.1/setup.cfg
--rw-rw-r--   0 jatin     (1000) jatin     (1000)      985 2022-08-11 20:00:25.000000 mdk-5.7.1/setup.py
+drwxrwxr-x   0 austin    (3007) ldap-eng  (2001)        0 2023-07-21 17:56:35.177949 mdk-5.7.2/
+-rw-rw-r--   0 austin    (3007) ldap-eng  (2001)     1068 2023-07-21 16:55:29.000000 mdk-5.7.2/LICENSE
+-rw-rw-r--   0 austin    (3007) ldap-eng  (2001)     1430 2023-07-21 17:56:35.177949 mdk-5.7.2/PKG-INFO
+-rw-rw-r--   0 austin    (3007) ldap-eng  (2001)      921 2023-07-21 16:55:29.000000 mdk-5.7.2/README.md
+drwxrwxr-x   0 austin    (3007) ldap-eng  (2001)        0 2023-07-21 17:56:35.173949 mdk-5.7.2/mdk/
+-rw-rw-r--   0 austin    (3007) ldap-eng  (2001)        0 2023-07-21 16:55:29.000000 mdk-5.7.2/mdk/__init__.py
+-rwxrwxr-x   0 austin    (3007) ldap-eng  (2001)     3620 2023-07-21 16:55:29.000000 mdk-5.7.2/mdk/main.py
+-rw-rw-r--   0 austin    (3007) ldap-eng  (2001)    16978 2023-07-21 17:49:24.000000 mdk-5.7.2/mdk/utils.py
+drwxrwxr-x   0 austin    (3007) ldap-eng  (2001)        0 2023-07-21 17:56:35.177949 mdk-5.7.2/mdk.egg-info/
+-rw-rw-r--   0 austin    (3007) ldap-eng  (2001)     1430 2023-07-21 17:56:31.000000 mdk-5.7.2/mdk.egg-info/PKG-INFO
+-rw-rw-r--   0 austin    (3007) ldap-eng  (2001)      241 2023-07-21 17:56:34.000000 mdk-5.7.2/mdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 austin    (3007) ldap-eng  (2001)        1 2023-07-21 17:56:34.000000 mdk-5.7.2/mdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 austin    (3007) ldap-eng  (2001)       38 2023-07-21 17:56:34.000000 mdk-5.7.2/mdk.egg-info/entry_points.txt
+-rw-rw-r--   0 austin    (3007) ldap-eng  (2001)        9 2023-07-21 17:56:34.000000 mdk-5.7.2/mdk.egg-info/requires.txt
+-rw-rw-r--   0 austin    (3007) ldap-eng  (2001)        4 2023-07-21 17:56:34.000000 mdk-5.7.2/mdk.egg-info/top_level.txt
+-rw-rw-r--   0 austin    (3007) ldap-eng  (2001)       67 2023-07-21 17:56:35.177949 mdk-5.7.2/setup.cfg
+-rw-rw-r--   0 austin    (3007) ldap-eng  (2001)      985 2023-07-21 16:55:29.000000 mdk-5.7.2/setup.py
```

### Comparing `mdk-5.7.1/LICENSE` & `mdk-5.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mdk-5.7.1/PKG-INFO` & `mdk-5.7.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: mdk
-Version: 5.7.1
+Version: 5.7.2
 Summary: a docker-compose helper
 Home-page: https://matician.com/
 Author: Michael Darr
 Author-email: mdarr@matician.com
 License: MIT
+Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3
 Description-Content-Type: text/markdown
@@ -39,7 +40,9 @@
 
 ## FAQ
 
 ### How do I add custom configuration to containers created by `mdk`?
 `mdk` automatically loads additional options from two files:
 * `ext.mdk.json` located in the same directory as `mdk.json`
 * `~/.config/mdk/mdk.json`
+
+
```

### Comparing `mdk-5.7.1/README.md` & `mdk-5.7.2/README.md`

 * *Files identical despite different names*

### Comparing `mdk-5.7.1/mdk/main.py` & `mdk-5.7.2/mdk/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 def mdk(*args, **kwargs):
     backend = MdkBackend()
 
     def nogpu_option(f):
         def callback(ctx, param, value):
             backend.no_gpu = value
         return click.option(
-            '--nogpu',
+            '--nogpu', '--no-gpu',
             default=False, is_flag=True, expose_value=False,
             callback=callback)(f)
 
     @click.group()
     @click.version_option(version=VERSION)
     def cli():
         pass
```

### Comparing `mdk-5.7.1/mdk/utils.py` & `mdk-5.7.2/mdk/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import socket
 import subprocess
 from typing import List, TypeVar, Optional, NoReturn
 import shlex
 import sys
 import time
 import pathlib
+import platform
 
 import click
 
 T = TypeVar('T')
 
 CONFIG_FILENAME: str = "mdk.json"
 CONFIG_EXTENSION_FILENAME: str = "ext.mdk.json"
@@ -91,15 +92,15 @@
         else:
             Log.fatal(f'{CONFIG_FILENAME} found in neither this directory nor any of its parents.')
 
         # load our configuration as a list of dicts, later configs override earlier ones
         self.conf_data = [json.load(open(path)) for path in self.conf_paths if path.is_file()]
 
         # ensure that we are new enough to properly parse this config
-        conf_version = self.conf("mdk-version")
+        conf_version = self.conf("mdk-version", str)
         if conf_version:
             try:
                 conf_version = version_tuple(conf_version)
             except ValueError:
                 Log.fatal(f'Config has invalid mdk-version {conf_version!r}.')
             if VERSION < conf_version:
                 Log.fatal(f'Project requires mdk>={version_string(conf_version)} '
@@ -121,18 +122,28 @@
         proc = subprocess.run(['docker', 'inspect', self.container_name()],
                               stdout=subprocess.PIPE, stderr=subprocess.PIPE)
         proc_out = json.loads(proc.stdout)  # docker returns valid JSON even if container is not found
         self._inspect = ContainerInspect(proc_out)
         return self._inspect
 
     def image_name(self) -> str:
-        return self.conf('image', required=True)
+        image_field = self.conf('image', required=True)
+        if isinstance(image_field, str):
+            return image_field
+        elif isinstance(image_field, dict):
+            arch = platform.machine()
+            if arch in image_field:
+                return image_field[arch]
+            else:
+                Log.fatal(f"mdk.json does not specify an image for {arch}")
+        else:
+            Log.fatal("Invalid type for \"image\"")
 
     def container_name(self) -> str:
-        container_name = self.conf("name")
+        container_name = self.conf("name", str)
         if container_name:
             return container_name
         return "mdk" + str(self.conf_root).replace('/', '_')
 
     def opts_hash(self) -> str:
         data_to_hash = '\0'.join(self.build_docker_opts(log_info=False, include_nfs=False)).encode()
         return hashlib.sha1(data_to_hash).hexdigest()
@@ -186,15 +197,14 @@
                     vol_src = str(self.conf_root) + vol_src[1:]
                 opt_builder += ['-v', vol_src + ':' + vol_tgt]
 
         if self.conf("shareX11", bool):
             opt_builder += [
                 "-v", "/tmp/.X11-unix:/tmp/.X11-unix:rw",
                 "--device", "/dev/dri:/dev/dri",
-                "--ipc", "host"
             ]
             display = os.getenv('DISPLAY')
             if display is not None:
                 opt_builder += ["-e", f"DISPLAY={display}"]
             xauth_file = os.getenv('XAUTHORITY', None)
             if xauth_file is not None:
                 opt_builder += ['-v', f"{xauth_file}:/tmp/.XAuthority",
@@ -247,15 +257,15 @@
                 v = f'{os.getuid()}'
             elif v in ('$GID', '${GID}'):
                 v = f'{os.getgid()}'
             else:
                 v = os.path.expandvars(v)
             opt_builder += ['-e', k + '=' + v]
 
-        workdir = self.conf('workdir')
+        workdir = self.conf('workdir', str)
         if workdir:
             opt_builder += ["-w", workdir]
 
         opt_builder += self.conf_list('options')
 
         # hacky way to allow overriding --gpus
         if self.no_gpu:
@@ -272,27 +282,27 @@
         # location but later when we start the container, we will symlink ~/.gitconfig to /.gitconfig
         gitconfig_path = os.path.expanduser("~/.gitconfig")
         if os.path.exists(gitconfig_path):
             opt_builder += ["-v", f"{gitconfig_path}:/.gitconfig"]
 
         return opt_builder
 
-    def conf(self, key: str, expected_type: type = str, required=False) -> Optional[T]:
+    def conf(self, key: str, expected_type: type = None, required=False) -> Optional[T]:
         # gather option in all configs
         all_data = [data[key] for data in self.conf_data if key in data]
 
         # case: conf option not found
         if not all_data:
             if required:
                 Log.fatal(f'Key {key!r} missing in mdk.json.')
             return None
 
         # validate and return
         res = all_data[-1]
-        if isinstance(res, expected_type):
+        if expected_type is None or isinstance(res, expected_type):
             return res
         Log.fatal(f'Key {key!r} expects a {expected_type.__name__}.')
 
     def conf_list(self, key: str) -> List[str]:
         all_data = [data[key] for data in self.conf_data if key in data]
         if all(isinstance(l, list) for l in all_data):
             res = [el for data in all_data for el in data]
```

### Comparing `mdk-5.7.1/mdk.egg-info/PKG-INFO` & `mdk-5.7.2/mdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: mdk
-Version: 5.7.1
+Version: 5.7.2
 Summary: a docker-compose helper
 Home-page: https://matician.com/
 Author: Michael Darr
 Author-email: mdarr@matician.com
 License: MIT
+Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3
 Description-Content-Type: text/markdown
@@ -39,7 +40,9 @@
 
 ## FAQ
 
 ### How do I add custom configuration to containers created by `mdk`?
 `mdk` automatically loads additional options from two files:
 * `ext.mdk.json` located in the same directory as `mdk.json`
 * `~/.config/mdk/mdk.json`
+
+
```

### Comparing `mdk-5.7.1/setup.py` & `mdk-5.7.2/setup.py`

 * *Files identical despite different names*

