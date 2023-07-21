# Comparing `tmp/bec-server-0.13.2.tar.gz` & `tmp/bec-server-0.13.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bec-server-0.13.2.tar", last modified: Fri Jul 21 07:52:35 2023, max compression
+gzip compressed data, was "bec-server-0.13.3.tar", last modified: Fri Jul 21 15:13:13 2023, max compression
```

## Comparing `bec-server-0.13.2.tar` & `bec-server-0.13.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 07:52:35.470386 bec-server-0.13.2/
--rw-r--r--   0 root         (0) root         (0)      443 2023-07-21 07:52:35.470386 bec-server-0.13.2/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 07:52:35.469386 bec-server-0.13.2/bec_server/
--rw-r--r--   0 root         (0) root         (0)       25 2023-07-08 15:47:18.000000 bec-server-0.13.2/bec_server/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1309 2023-07-08 15:47:18.000000 bec-server-0.13.2/bec_server/launch.py
--rw-r--r--   0 root         (0) root         (0)     3075 2023-07-08 15:47:18.000000 bec-server-0.13.2/bec_server/service_handler.py
--rw-r--r--   0 root         (0) root         (0)     2345 2023-07-08 15:47:18.000000 bec-server-0.13.2/bec_server/tmux_launch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 07:52:35.470386 bec-server-0.13.2/bec_server.egg-info/
--rw-r--r--   0 root         (0) root         (0)      443 2023-07-21 07:52:35.000000 bec-server-0.13.2/bec_server.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      332 2023-07-21 07:52:35.000000 bec-server-0.13.2/bec_server.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 07:52:35.000000 bec-server-0.13.2/bec_server.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       48 2023-07-21 07:52:35.000000 bec-server-0.13.2/bec_server.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       66 2023-07-21 07:52:35.000000 bec-server-0.13.2/bec_server.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-07-21 07:52:35.000000 bec-server-0.13.2/bec_server.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      503 2023-07-21 07:52:35.471386 bec-server-0.13.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1068 2023-07-08 15:47:18.000000 bec-server-0.13.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:13:13.149703 bec-server-0.13.3/
+-rw-r--r--   0 root         (0) root         (0)      443 2023-07-21 15:13:13.149703 bec-server-0.13.3/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:13:13.144703 bec-server-0.13.3/bec_server/
+-rw-r--r--   0 root         (0) root         (0)       25 2023-07-08 15:33:35.000000 bec-server-0.13.3/bec_server/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1391 2023-07-21 15:12:28.000000 bec-server-0.13.3/bec_server/launch.py
+-rw-r--r--   0 root         (0) root         (0)     3075 2023-07-08 15:33:35.000000 bec-server-0.13.3/bec_server/service_handler.py
+-rw-r--r--   0 root         (0) root         (0)     2716 2023-07-21 15:12:28.000000 bec-server-0.13.3/bec_server/tmux_launch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:13:13.149703 bec-server-0.13.3/bec_server.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      443 2023-07-21 15:13:13.000000 bec-server-0.13.3/bec_server.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      332 2023-07-21 15:13:13.000000 bec-server-0.13.3/bec_server.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 15:13:13.000000 bec-server-0.13.3/bec_server.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       48 2023-07-21 15:13:13.000000 bec-server-0.13.3/bec_server.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       79 2023-07-21 15:13:13.000000 bec-server-0.13.3/bec_server.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-07-21 15:13:13.000000 bec-server-0.13.3/bec_server.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      503 2023-07-21 15:13:13.150703 bec-server-0.13.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1400 2023-07-21 15:12:28.000000 bec-server-0.13.3/setup.py
```

### Comparing `bec-server-0.13.2/bec_server/launch.py` & `bec-server-0.13.3/bec_server/launch.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,17 +25,22 @@
         default=None,
         help="Path to the BEC service config file",
     )
     command.add_parser("status", help="Show the status of the BEC server")
 
     args = parser.parse_args()
 
+    if "config" in args:
+        config = args.config
+    else:
+        config = None
+
     service_handler = ServiceHandler(
         bec_path=os.path.dirname(os.path.dirname(os.path.dirname(os.path.abspath(__file__)))),
-        config_path=args.config,
+        config_path=config,
     )
     if args.command == "start":
         service_handler.start()
     elif args.command == "stop":
         service_handler.stop()
     elif args.command == "restart":
         service_handler.restart()
```

### Comparing `bec-server-0.13.2/bec_server/service_handler.py` & `bec-server-0.13.3/bec_server/service_handler.py`

 * *Files identical despite different names*

### Comparing `bec-server-0.13.2/bec_server/tmux_launch.py` & `bec-server-0.13.3/bec_server/tmux_launch.py`

 * *Files 23% similar despite different names*

```diff
@@ -8,22 +8,30 @@
     Activate the python environment for a service.
     """
 
     # check if the current file was install with pip install -e (editable mode)
     # if so, the venv is the service directory and it's called <service_name>_venv
     # otherwise, we simply take the currently running venv
 
+    base_dir = os.path.dirname(os.path.dirname(os.path.dirname(__file__)))
+
     if "site-packages" in __file__:
         venv_base_path = os.path.dirname(
             os.path.dirname(os.path.dirname(__file__.split("site-packages", maxsplit=1)[0]))
         )
         pane.send_keys(f"source {venv_base_path}/bin/activate")
         return
+    if os.path.exists(f"{service_path}/{service_name}_venv"):
+        pane.send_keys(f"source {service_path}/{service_name}_venv/bin/activate")
+        return
+    if os.path.exists(f"{base_dir}/bec_venv"):
+        pane.send_keys(f"source {base_dir}/bec_venv/bin/activate")
+        return
 
-    pane.send_keys(f"source {service_path}/{service_name}_venv/bin/activate")
+    raise RuntimeError(f"Could not find a virtual environment for {service_name}. ")
 
 
 def tmux_start(bec_path: str, config_path: str, services: dict):
     """
     Launch the BEC server in a tmux session. All services are launched in separate panes.
 
     Args:
```

