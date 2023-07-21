# Comparing `tmp/arcor2_execution-1.0.0.tar.gz` & `tmp/arcor2_execution-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arcor2_execution-1.0.0.tar", last modified: Tue Feb 14 12:55:49 2023, max compression
+gzip compressed data, was "arcor2_execution-1.1.0.tar", last modified: Thu Jul 20 11:09:54 2023, max compression
```

## Comparing `arcor2_execution-1.0.0.tar` & `arcor2_execution-1.1.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-02-14 12:55:49.863361 arcor2_execution-1.0.0/
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)       12 2023-02-14 12:55:49.000000 arcor2_execution-1.0.0/MANIFEST.in
--rw-rw-r--   0 zdenal    (1000) zdenal    (1000)     5195 2023-02-14 12:55:49.863361 arcor2_execution-1.0.0/PKG-INFO
-drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-02-14 12:55:49.859361 arcor2_execution-1.0.0/arcor2_execution/
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)        5 2023-02-14 12:55:49.000000 arcor2_execution-1.0.0/arcor2_execution/VERSION
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)       96 2023-02-14 12:55:49.000000 arcor2_execution-1.0.0/arcor2_execution/__init__.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)        0 2023-02-14 12:55:49.000000 arcor2_execution-1.0.0/arcor2_execution/py.typed
-drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-02-14 12:55:49.859361 arcor2_execution-1.0.0/arcor2_execution/scripts/
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)        0 2023-02-14 12:55:49.000000 arcor2_execution-1.0.0/arcor2_execution/scripts/__init__.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)    17100 2023-02-14 12:55:49.000000 arcor2_execution-1.0.0/arcor2_execution/scripts/execution.py
-drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-02-14 12:55:49.859361 arcor2_execution-1.0.0/arcor2_execution.egg-info/
--rw-rw-r--   0 zdenal    (1000) zdenal    (1000)     5195 2023-02-14 12:55:49.000000 arcor2_execution-1.0.0/arcor2_execution.egg-info/PKG-INFO
--rw-rw-r--   0 zdenal    (1000) zdenal    (1000)      482 2023-02-14 12:55:49.000000 arcor2_execution-1.0.0/arcor2_execution.egg-info/SOURCES.txt
--rw-rw-r--   0 zdenal    (1000) zdenal    (1000)        1 2023-02-14 12:55:49.000000 arcor2_execution-1.0.0/arcor2_execution.egg-info/dependency_links.txt
--rw-rw-r--   0 zdenal    (1000) zdenal    (1000)       77 2023-02-14 12:55:49.000000 arcor2_execution-1.0.0/arcor2_execution.egg-info/entry_points.txt
--rw-rw-r--   0 zdenal    (1000) zdenal    (1000)        1 2023-02-14 12:55:49.000000 arcor2_execution-1.0.0/arcor2_execution.egg-info/namespace_packages.txt
--rw-rw-r--   0 zdenal    (1000) zdenal    (1000)      217 2023-02-14 12:55:49.000000 arcor2_execution-1.0.0/arcor2_execution.egg-info/requires.txt
--rw-rw-r--   0 zdenal    (1000) zdenal    (1000)       17 2023-02-14 12:55:49.000000 arcor2_execution-1.0.0/arcor2_execution.egg-info/top_level.txt
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)      698 2023-02-14 12:55:49.000000 arcor2_execution-1.0.0/backend_shim.py
--rw-rw-r--   0 zdenal    (1000) zdenal    (1000)       38 2023-02-14 12:55:49.863361 arcor2_execution-1.0.0/setup.cfg
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)     6182 2023-02-14 12:55:49.000000 arcor2_execution-1.0.0/setup.py
+drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-07-20 11:09:54.586951 arcor2_execution-1.1.0/
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)       12 2023-07-20 11:09:54.000000 arcor2_execution-1.1.0/MANIFEST.in
+-rw-rw-r--   0 zdenal    (1000) zdenal    (1000)     5269 2023-07-20 11:09:54.586951 arcor2_execution-1.1.0/PKG-INFO
+drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-07-20 11:09:54.586951 arcor2_execution-1.1.0/arcor2_execution/
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)        5 2023-07-20 11:09:54.000000 arcor2_execution-1.1.0/arcor2_execution/VERSION
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)       96 2023-07-20 11:09:54.000000 arcor2_execution-1.1.0/arcor2_execution/__init__.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)        0 2023-07-20 11:09:54.000000 arcor2_execution-1.1.0/arcor2_execution/py.typed
+drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-07-20 11:09:54.586951 arcor2_execution-1.1.0/arcor2_execution/scripts/
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)        0 2023-07-20 11:09:54.000000 arcor2_execution-1.1.0/arcor2_execution/scripts/__init__.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)    17077 2023-07-20 11:09:54.000000 arcor2_execution-1.1.0/arcor2_execution/scripts/execution.py
+drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-07-20 11:09:54.586951 arcor2_execution-1.1.0/arcor2_execution.egg-info/
+-rw-rw-r--   0 zdenal    (1000) zdenal    (1000)     5269 2023-07-20 11:09:54.000000 arcor2_execution-1.1.0/arcor2_execution.egg-info/PKG-INFO
+-rw-rw-r--   0 zdenal    (1000) zdenal    (1000)      482 2023-07-20 11:09:54.000000 arcor2_execution-1.1.0/arcor2_execution.egg-info/SOURCES.txt
+-rw-rw-r--   0 zdenal    (1000) zdenal    (1000)        1 2023-07-20 11:09:54.000000 arcor2_execution-1.1.0/arcor2_execution.egg-info/dependency_links.txt
+-rw-rw-r--   0 zdenal    (1000) zdenal    (1000)       77 2023-07-20 11:09:54.000000 arcor2_execution-1.1.0/arcor2_execution.egg-info/entry_points.txt
+-rw-rw-r--   0 zdenal    (1000) zdenal    (1000)        1 2023-07-20 11:09:54.000000 arcor2_execution-1.1.0/arcor2_execution.egg-info/namespace_packages.txt
+-rw-rw-r--   0 zdenal    (1000) zdenal    (1000)      217 2023-07-20 11:09:54.000000 arcor2_execution-1.1.0/arcor2_execution.egg-info/requires.txt
+-rw-rw-r--   0 zdenal    (1000) zdenal    (1000)       17 2023-07-20 11:09:54.000000 arcor2_execution-1.1.0/arcor2_execution.egg-info/top_level.txt
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)      822 2023-07-20 11:09:54.000000 arcor2_execution-1.1.0/backend_shim.py
+-rw-rw-r--   0 zdenal    (1000) zdenal    (1000)       38 2023-07-20 11:09:54.586951 arcor2_execution-1.1.0/setup.cfg
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)     6256 2023-07-20 11:09:54.000000 arcor2_execution-1.1.0/setup.py
```

### Comparing `arcor2_execution-1.0.0/PKG-INFO` & `arcor2_execution-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arcor2_execution
-Version: 1.0.0
+Version: 1.1.0
 Summary: ARCOR2 Execution service
 Author: Robo@FIT
 Author-email: imaterna@fit.vut.cz
 License: LGPL
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
@@ -23,14 +23,20 @@
 - `ARCOR2_MAX_RPC_DURATION=0.1` - by default, a warning is emitted when any RPC call takes longer than 0.1 second.
 - `ARCOR2_EXECUTION_DEBUG=1` - switches logger to the `DEBUG` level.
 - `ARCOR2_ARSERVER_ASYNCIO_DEBUG=1` - turns on `asyncio` debug output (helpful to debug problems related to concurrency).
 # Changelog
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 
+## [1.1.0] - 2023-07-20
+
+### Added
+
+- Compatibility with `arcor2:1.1.0`.
+
 ## [1.0.0] - 2023-02-14
 
 ### Changed
 
 - Marked as a stable version.
 
 ## [0.22.0] - 2022-12-12
```

### Comparing `arcor2_execution-1.0.0/arcor2_execution/scripts/execution.py` & `arcor2_execution-1.1.0/arcor2_execution/scripts/execution.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,26 +48,23 @@
 
 MAIN_SCRIPT_NAME = "script.py"
 
 EVENT_MAPPING = {evt.__name__: evt for evt in EVENTS}
 
 
 def process_running() -> bool:
-
     return PROCESS is not None and PROCESS.returncode is None
 
 
 async def package_state(event: PackageState) -> None:
-
     PACKAGE_STATE_EVENT.data = event.data
     await send_to_clients(event)
 
 
 async def read_proc_stdout() -> None:
-
     global PACKAGE_INFO_EVENT
     global RUNNING_PACKAGE_ID
 
     logger.info("Reading script stdout...")
 
     assert PROCESS is not None
     assert PROCESS.stdout is not None
@@ -111,32 +108,29 @@
         await send_to_clients(evt)
 
     PACKAGE_INFO_EVENT = None
 
     await PROCESS.communicate()  # otherwise returncode might be still None
 
     if PROCESS.returncode:
-
         if printed_out:
-
             # TODO remember this (until another package is started) and send it to new clients?
             last_line = printed_out[-1].strip()
 
             try:
                 exception_type, message = last_line.split(":", 1)
             except ValueError:
                 exception_type, message = "Unknown", last_line
 
             await send_to_clients(ProjectException(ProjectException.Data(message, exception_type)))
 
             async with aiofiles.open("traceback-{}.txt".format(time.strftime("%Y%m%d-%H%M%S")), "w") as tb_file:
                 await tb_file.write("".join(printed_out))
 
         else:
-
             await send_to_clients(
                 ProjectException(
                     ProjectException.Data(f"Process ended with non-zero return code ({PROCESS.returncode}).", "unknown")
                 )
             )
 
             logger.warn(
@@ -146,22 +140,20 @@
     await package_state(PackageState(PackageState.Data(PackageState.Data.StateEnum.STOPPED, RUNNING_PACKAGE_ID)))
     logger.info(f"Process finished with returncode {PROCESS.returncode}.")
 
     RUNNING_PACKAGE_ID = None
 
 
 async def check_script(script_path: str) -> None:
-
     if not await run_in_executor(os.path.exists, script_path):
         raise Arcor2Exception("Main script not found.")
 
 
 async def run_package_cb(req: rpc.RunPackage.Request, ui: WsClient) -> None:
     async def _update_executed(package_id: str) -> None:
-
         meta = await run_in_executor(read_package_meta, package_id)
         meta.executed = datetime.now(tz=timezone.utc)
         await run_in_executor(write_package_meta, package_id, meta)
 
     global PROCESS
     global TASK
     global RUNNING_PACKAGE_ID
@@ -215,15 +207,14 @@
 
     TASK = asyncio.create_task(read_proc_stdout())  # run task in background
     asyncio.create_task(_update_executed(req.args.id))
 
 
 async def stop_package_cb(req: rpc.StopPackage.Request, ui: WsClient) -> None:
     async def _terminate_task() -> None:
-
         global PACKAGE_INFO_EVENT
         global RUNNING_PACKAGE_ID
 
         assert PROCESS
         assert TASK
 
         logger.info("Terminating process")
@@ -241,15 +232,14 @@
 
     await package_state(PackageState(PackageState.Data(PackageState.Data.StateEnum.STOPPING, RUNNING_PACKAGE_ID)))
     asyncio.create_task(_terminate_task())
 
 
 async def pause_package_cb(req: rpc.PausePackage.Request, ui: WsClient) -> None:
     async def _pause() -> None:
-
         assert PROCESS is not None
         assert PROCESS.stdin is not None
 
         PROCESS.stdin.write("p\n".encode())
         await PROCESS.stdin.drain()
         logger.info("Package paused.")
 
@@ -259,15 +249,14 @@
     await package_state(PackageState(PackageState.Data(PackageState.Data.StateEnum.PAUSING, RUNNING_PACKAGE_ID)))
     assert process_running()
     asyncio.create_task(_pause())
 
 
 async def step_action_cb(req: rpc.StepAction.Request, ui: WsClient) -> None:
     async def _step() -> None:
-
         assert PROCESS is not None
         assert PROCESS.stdin is not None
 
         PROCESS.stdin.write("s\n".encode())
         await PROCESS.stdin.drain()
         logger.info("Stepping to a next action.")
 
@@ -277,15 +266,14 @@
     await package_state(PackageState(PackageState.Data(PackageState.Data.StateEnum.RESUMING, RUNNING_PACKAGE_ID)))
     assert process_running()
     asyncio.create_task(_step())
 
 
 async def resume_package_cb(req: rpc.ResumePackage.Request, ui: WsClient) -> None:
     async def _resume() -> None:
-
         assert PROCESS is not None
         assert PROCESS.stdin is not None
 
         PROCESS.stdin.write("r\n".encode())
         await PROCESS.stdin.drain()
         logger.info("Package resumed.")
 
@@ -296,27 +284,25 @@
 
     await package_state(PackageState(PackageState.Data(PackageState.Data.StateEnum.RESUMING, RUNNING_PACKAGE_ID)))
     asyncio.create_task(_resume())
 
 
 async def _upload_package_cb(req: rpc.UploadPackage.Request, ui: WsClient) -> None:
     async def _upload_event(path_to_package: str) -> None:
-
         summary = await get_summary(path_to_package)
         evt = events.PackageChanged(summary)
         evt.change_type = Event.Type.ADD
         await send_to_clients(evt)
         logger.info(f"Package '{summary.package_meta.name}' was added.")
 
     target_path = os.path.join(PROJECT_PATH, req.args.id)
 
     # TODO do not allow if there are manual changes?
 
     async with tempfile.TemporaryDirectory() as tmpdirname:
-
         zip_path = os.path.join(tmpdirname, "publish.zip")
 
         b64_bytes = req.args.data.encode()
         zip_content = base64.b64decode(b64_bytes)
 
         async with aiofiles.open(zip_path, mode="wb") as zip_file:
             await zip_file.write(zip_content)
@@ -339,23 +325,21 @@
             pass
         await run_in_executor(shutil.copytree, tmpdirname, target_path)
 
     asyncio.create_task(_upload_event(target_path))
 
 
 async def get_summary(path: str) -> PackageSummary:
-
     if summary := await get_opt_summary(path):
         return summary
 
     raise Arcor2Exception("Invalid package.")
 
 
 async def get_opt_summary(path: str) -> None | PackageSummary:
-
     if not os.path.isfile(os.path.join(path, MAIN_SCRIPT_NAME)):
         logger.warn(f"Package at {path} does not contain main script.")
         return None
 
     package_dir = os.path.basename(path)
     package_meta = read_package_meta(package_dir)
 
@@ -367,27 +351,25 @@
 
         return PackageSummary(package_dir, package_meta)
 
     return PackageSummary(package_dir, package_meta, ProjectMeta.from_project(project))
 
 
 async def list_packages_cb(req: rpc.ListPackages.Request, ui: WsClient) -> rpc.ListPackages.Response:
-
     resp = rpc.ListPackages.Response()
     subfolders = [f.path for f in os.scandir(PROJECT_PATH) if f.is_dir()]
     resp.data = [
         ps
         for ps in await asyncio.gather(*[get_opt_summary(folder_path) for folder_path in subfolders])
         if ps is not None
     ]
     return resp
 
 
 async def delete_package_cb(req: rpc.DeletePackage.Request, ui: WsClient) -> None:
-
     if RUNNING_PACKAGE_ID and RUNNING_PACKAGE_ID == req.args.id:
         raise Arcor2Exception("Package is being executed.")
 
     target_path = os.path.join(PROJECT_PATH, req.args.id)
     package_summary = await get_summary(target_path)
 
     try:
@@ -399,15 +381,14 @@
     evt.change_type = Event.Type.REMOVE
     asyncio.ensure_future(send_to_clients(evt))
     logger.info(f"Package '{package_summary.package_meta.name}' was removed.")
     return None
 
 
 async def rename_package_cb(req: rpc.RenamePackage.Request, ui: WsClient) -> None:
-
     target_path = os.path.join(PROJECT_PATH, req.args.package_id, "package.json")
 
     pm = read_package_meta(req.args.package_id)
     old_name = pm.name
     pm.name = req.args.new_name
 
     async with aiofiles.open(target_path, mode="w") as pkg_file:
@@ -423,25 +404,23 @@
 async def _version_cb(req: arcor2_rpc.common.Version.Request, ui: WsClient) -> arcor2_rpc.common.Version.Response:
     resp = arcor2_rpc.common.Version.Response()
     resp.data = resp.Data(await run_in_executor(arcor2_execution_data.version))
     return resp
 
 
 async def send_to_clients(event: events.Event) -> None:
-
     if isinstance(event, ProjectException):
         logger.error(f"Script raised {event.data.type}. {event.data.message}")
 
     if CLIENTS:
         data = event.to_json()
         await asyncio.wait([client.send(data) for client in CLIENTS])
 
 
 async def register(websocket: WsClient) -> None:
-
     logger.info("Registering new client")
     CLIENTS.add(websocket)
 
     tasks: list[Awaitable] = [websocket.send(PACKAGE_STATE_EVENT.to_json())]
 
     if PACKAGE_INFO_EVENT:
         tasks.append(websocket.send(PACKAGE_INFO_EVENT.to_json()))
@@ -465,15 +444,14 @@
     rpc.DeletePackage.__name__: (rpc.DeletePackage, delete_package_cb),
     rpc.RenamePackage.__name__: (rpc.RenamePackage, rename_package_cb),
     arcor2_rpc.common.Version.__name__: (arcor2_rpc.common.Version, _version_cb),
 }
 
 
 async def aio_main() -> None:
-
     if __debug__:
         logger.warn("Development mode. The service will shutdown on any unhandled exception.")
 
     logger.info(
         f"Execution service {arcor2_execution.version()} " f"(API version {arcor2_execution_data.version()}) started."
     )
 
@@ -481,15 +459,14 @@
         functools.partial(ws_server.server, logger=logger, register=register, unregister=unregister, rpc_dict=RPC_DICT),
         "0.0.0.0",
         port_from_url(URL),
     )
 
 
 def main() -> None:
-
     parser = argparse.ArgumentParser()
 
     parser.add_argument(
         "-d",
         "--debug",
         help="Set logging level to debug.",
         action="store_const",
```

### Comparing `arcor2_execution-1.0.0/arcor2_execution.egg-info/PKG-INFO` & `arcor2_execution-1.1.0/arcor2_execution.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arcor2-execution
-Version: 1.0.0
+Version: 1.1.0
 Summary: ARCOR2 Execution service
 Author: Robo@FIT
 Author-email: imaterna@fit.vut.cz
 License: LGPL
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
@@ -23,14 +23,20 @@
 - `ARCOR2_MAX_RPC_DURATION=0.1` - by default, a warning is emitted when any RPC call takes longer than 0.1 second.
 - `ARCOR2_EXECUTION_DEBUG=1` - switches logger to the `DEBUG` level.
 - `ARCOR2_ARSERVER_ASYNCIO_DEBUG=1` - turns on `asyncio` debug output (helpful to debug problems related to concurrency).
 # Changelog
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 
+## [1.1.0] - 2023-07-20
+
+### Added
+
+- Compatibility with `arcor2:1.1.0`.
+
 ## [1.0.0] - 2023-02-14
 
 ### Changed
 
 - Marked as a stable version.
 
 ## [0.22.0] - 2022-12-12
```

### Comparing `arcor2_execution-1.0.0/setup.py` & `arcor2_execution-1.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,20 +19,20 @@
     'description': 'ARCOR2 Execution service',
     'entry_points': {
         'console_scripts': [
             'arcor2_execution = arcor2_execution.scripts.execution:main',
         ],
     },
     'install_requires': (
-        'aiofiles~=22.1.0',
+        'aiofiles~=23.1.0',
         'aiologger~=0.7.0',
         'aiorun~=2022.11.1',
         'arcor2_execution_data~=1.0.0',
         'arcor2_runtime~=1.0.0',
-        'arcor2~=1.0.0',
+        'arcor2~=1.1.0',
         'dataclasses-jsonschema[apispec,fast-dateparsing,fast-uuid,fast-validation]~=2.16.0',
         'websockets~=10.4',
     ),
     'license': 'LGPL',
     'long_description': """# arcor2_execution
 
 ## Environment variables
@@ -41,14 +41,20 @@
 - `ARCOR2_MAX_RPC_DURATION=0.1` - by default, a warning is emitted when any RPC call takes longer than 0.1 second.
 - `ARCOR2_EXECUTION_DEBUG=1` - switches logger to the `DEBUG` level.
 - `ARCOR2_ARSERVER_ASYNCIO_DEBUG=1` - turns on `asyncio` debug output (helpful to debug problems related to concurrency).
 # Changelog
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 
+## [1.1.0] - 2023-07-20
+
+### Added
+
+- Compatibility with `arcor2:1.1.0`.
+
 ## [1.0.0] - 2023-02-14
 
 ### Changed
 
 - Marked as a stable version.
 
 ## [0.22.0] - 2022-12-12
@@ -218,9 +224,9 @@
         ),
     },
     'packages': (
         'arcor2_execution',
         'arcor2_execution.scripts',
     ),
     'python_requires': '==3.10.*',
-    'version': '1.0.0',
+    'version': '1.1.0',
 })
```

