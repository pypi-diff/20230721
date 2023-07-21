# Comparing `tmp/hserv-0.0.5.tar.gz` & `tmp/hserv-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hserv-0.0.5.tar", last modified: Thu Jul 20 15:12:23 2023, max compression
+gzip compressed data, was "hserv-0.0.6.tar", last modified: Fri Jul 21 12:01:36 2023, max compression
```

## Comparing `hserv-0.0.5.tar` & `hserv-0.0.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 15:12:23.576403 hserv-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (122)    35149 2023-07-20 15:12:12.000000 hserv-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       58 2023-07-20 15:12:12.000000 hserv-0.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      297 2023-07-20 15:12:23.576403 hserv-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       69 2023-07-20 15:12:12.000000 hserv-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 15:12:23.572403 hserv-0.0.5/hserv/
--rw-r--r--   0 runner    (1001) docker     (122)       36 2023-07-20 15:12:12.000000 hserv-0.0.5/hserv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       20 2023-07-20 15:12:12.000000 hserv-0.0.5/hserv/__version__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4117 2023-07-20 15:12:12.000000 hserv-0.0.5/hserv/server.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 15:12:23.576403 hserv-0.0.5/hserv/supabase/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 15:12:12.000000 hserv-0.0.5/hserv/supabase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1984 2023-07-20 15:12:12.000000 hserv-0.0.5/hserv/supabase/config.py
--rw-r--r--   0 runner    (1001) docker     (122)    12184 2023-07-20 15:12:12.000000 hserv-0.0.5/hserv/supabase/controller.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 15:12:23.576403 hserv-0.0.5/hserv.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      297 2023-07-20 15:12:23.000000 hserv-0.0.5/hserv.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      335 2023-07-20 15:12:23.000000 hserv-0.0.5/hserv.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-20 15:12:23.000000 hserv-0.0.5/hserv.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       47 2023-07-20 15:12:23.000000 hserv-0.0.5/hserv.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-07-20 15:12:23.000000 hserv-0.0.5/hserv.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       46 2023-07-20 15:12:12.000000 hserv-0.0.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-20 15:12:23.576403 hserv-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      704 2023-07-20 15:12:12.000000 hserv-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 12:01:36.775465 hserv-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (122)    35149 2023-07-21 12:01:15.000000 hserv-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       58 2023-07-21 12:01:15.000000 hserv-0.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      297 2023-07-21 12:01:36.775465 hserv-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2023-07-21 12:01:15.000000 hserv-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 12:01:36.771465 hserv-0.0.6/hserv/
+-rw-r--r--   0 runner    (1001) docker     (122)       36 2023-07-21 12:01:15.000000 hserv-0.0.6/hserv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       20 2023-07-21 12:01:15.000000 hserv-0.0.6/hserv/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5519 2023-07-21 12:01:15.000000 hserv-0.0.6/hserv/server.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 12:01:36.775465 hserv-0.0.6/hserv/supabase/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-21 12:01:15.000000 hserv-0.0.6/hserv/supabase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3054 2023-07-21 12:01:15.000000 hserv-0.0.6/hserv/supabase/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10422 2023-07-21 12:01:15.000000 hserv-0.0.6/hserv/supabase/controller.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 12:01:36.775465 hserv-0.0.6/hserv.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      297 2023-07-21 12:01:36.000000 hserv-0.0.6/hserv.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      335 2023-07-21 12:01:36.000000 hserv-0.0.6/hserv.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-21 12:01:36.000000 hserv-0.0.6/hserv.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       47 2023-07-21 12:01:36.000000 hserv-0.0.6/hserv.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-07-21 12:01:36.000000 hserv-0.0.6/hserv.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       46 2023-07-21 12:01:15.000000 hserv-0.0.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-21 12:01:36.775465 hserv-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      704 2023-07-21 12:01:15.000000 hserv-0.0.6/setup.py
```

### Comparing `hserv-0.0.5/LICENSE` & `hserv-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `hserv-0.0.5/hserv/server.py` & `hserv-0.0.6/hserv/server.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,40 @@
-from typing import Union, Optional, cast
-from dataclasses import dataclass
+from typing import Union, Optional, cast, Dict, Any, TYPE_CHECKING
+from dataclasses import dataclass, field
 import re
 import io
 import os
 import shutil
 
-from fabric import Connection
+from fabric import Connection, Result
 
+if TYPE_CHECKING:
+    from hserv.supabase.controller import SupabaseController
 
 @dataclass
 class HydrocodeServer(object):
     connection: str = 'localhost'
+    username: Optional[str] = None
+    _supabase_projects: Dict[str, 'SupabaseController'] = field(default_factory=dict, init=False)
 
     @property
     def run(self):
         # create a remote warpper            
         def _run(*args, **kwargs):
-            with Connection(self.connection) as con:
+            with Connection(self.connection, user=self.username) as con:
                 return con.run(*args, **kwargs)
         
         # create a local wrapper
         def _run_local(*args, **kwargs):
             with Connection(self.connection) as con:
-                return con.local(*args, **kwargs)
+                res = con.local(*args, **kwargs)
+                if res is None:
+                    return Result(connection=con)
+                else:
+                    return res
 
         # check which one to use
         if 'localhost' in self.connection:
             return _run_local
         else:
             return _run
 
@@ -85,14 +93,26 @@
 
         # check which one to use
         if 'localhost' in self.connection:
             return _get_local
         else:
             return _get                
 
+    def exists(self, path: str) -> bool:
+        # create the remote wrapper
+        res = self.run(f"python -c \"import os; print(os.path.exists('{path}'))\"", hide=True)
+        return res.stdout == 'True'
+
+    @property
+    def cwd(self):
+        return self.run("pwd", hide=True).stdout
+
+    def cp(self, src: str, dst: str):
+        self.run(f"cp {src} {dst}", hide=True)
+
     def _extract_semver(self, command: str) -> str:
         # get git version
         try:
             v = self.run(command, hide='both')
             s = re.search(r'(\d+\.\d+\.\d+)', v.stdout)
         except Exception:
             s = None
@@ -114,14 +134,29 @@
             curl_version=self._extract_semver('curl --version'),
         )
 
         # return
         return info
     
     def get_free_port(self) -> int:
-        cmd = "import socket; s = socket.socket(); s.bind(('', 0)); print(s.getsockname()[1]); s.close()"
+        cmd = "python -c \"import socket; s = socket.socket(); s.bind(('', 0)); print(s.getsockname()[1]); s.close()\""
 
         res = self.run(cmd, hide='both')
         return int(res.stdout)
 
-    def supabase(self, project: str):
-        pass
+    def supabase(self, project: str, **kwargs) -> 'SupabaseController':
+        # check if we have an instance of that project
+        if project in self._supabase_projects:
+            return self._supabase_projects[project]
+        else:
+            # initialize a new supabase controller
+            from hserv.supabase.controller import SupabaseController
+
+            # update the kwargs
+            kwargs['public_url'] = self.connection
+            controller = SupabaseController(project, **kwargs)
+
+            # cache the controller
+            self._supabase_projects[project] = controller
+
+            # return
+            return controller
```

### Comparing `hserv-0.0.5/setup.py` & `hserv-0.0.6/setup.py`

 * *Files identical despite different names*

