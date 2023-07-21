# Comparing `tmp/validio_cli-0.6.3.tar.gz` & `tmp/validio_cli-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "validio_cli-0.6.3.tar", max compression
+gzip compressed data, was "validio_cli-0.6.4.tar", max compression
```

## Comparing `validio_cli-0.6.3.tar` & `validio_cli-0.6.4.tar`

### file list

```diff
@@ -1,25 +1,26 @@
--rw-r--r--   0        0        0    11340 2023-07-10 07:22:31.790640 validio_cli-0.6.3/LICENSE
--rw-r--r--   0        0        0      227 2023-07-10 07:22:31.791640 validio_cli-0.6.3/README_PUBLIC.md
--rw-r--r--   0        0        0     1987 2023-07-10 07:22:47.882609 validio_cli-0.6.3/pyproject.toml
--rw-r--r--   0        0        0     6274 2023-07-10 07:22:31.792640 validio_cli-0.6.3/validio_cli/__init__.py
--rw-r--r--   0        0        0     2390 2023-07-10 07:22:31.792640 validio_cli-0.6.3/validio_cli/bin/entities/channels.py
--rw-r--r--   0        0        0    11640 2023-07-10 07:22:31.792640 validio_cli-0.6.3/validio_cli/bin/entities/code.py
--rw-r--r--   0        0        0     4335 2023-07-10 07:22:31.792640 validio_cli-0.6.3/validio_cli/bin/entities/config.py
--rw-r--r--   0        0        0     2506 2023-07-10 07:22:31.792640 validio_cli-0.6.3/validio_cli/bin/entities/credentials.py
--rw-r--r--   0        0        0     2306 2023-07-10 07:22:31.792640 validio_cli-0.6.3/validio_cli/bin/entities/destinations.py
--rw-r--r--   0        0        0     7429 2023-07-10 07:22:31.792640 validio_cli-0.6.3/validio_cli/bin/entities/incidents.py
--rw-r--r--   0        0        0     2336 2023-07-10 07:22:31.792640 validio_cli-0.6.3/validio_cli/bin/entities/metrics.py
--rw-r--r--   0        0        0     2867 2023-07-10 07:22:31.792640 validio_cli-0.6.3/validio_cli/bin/entities/notification_rules.py
--rw-r--r--   0        0        0     3334 2023-07-10 07:22:31.792640 validio_cli-0.6.3/validio_cli/bin/entities/recommendations.py
--rw-r--r--   0        0        0     2913 2023-07-10 07:22:31.792640 validio_cli-0.6.3/validio_cli/bin/entities/segmentations.py
--rw-r--r--   0        0        0     1902 2023-07-10 07:22:31.792640 validio_cli-0.6.3/validio_cli/bin/entities/segments.py
--rw-r--r--   0        0        0    26341 2023-07-10 07:22:31.792640 validio_cli-0.6.3/validio_cli/bin/entities/sources.py
--rw-r--r--   0        0        0     1174 2023-07-10 07:22:31.792640 validio_cli-0.6.3/validio_cli/bin/entities/users.py
--rw-r--r--   0        0        0     3743 2023-07-10 07:22:31.792640 validio_cli-0.6.3/validio_cli/bin/entities/validators.py
--rw-r--r--   0        0        0     2806 2023-07-10 07:22:31.792640 validio_cli-0.6.3/validio_cli/bin/entities/windows.py
--rw-r--r--   0        0        0     3259 2023-07-10 07:22:31.792640 validio_cli-0.6.3/validio_cli/bin/main.py
--rw-r--r--   0        0        0     2587 2023-07-10 07:22:31.792640 validio_cli-0.6.3/validio_cli/components.py
--rw-r--r--   0        0        0      265 2023-07-10 07:22:31.792640 validio_cli-0.6.3/validio_cli/metadata.py
--rw-r--r--   0        0        0      630 2023-07-10 07:22:31.792640 validio_cli-0.6.3/validio_cli/namespace.py
--rw-r--r--   0        0        0     1382 2023-07-10 07:22:31.792640 validio_cli-0.6.3/validio_cli/schema.py
--rw-r--r--   0        0        0     1116 1970-01-01 00:00:00.000000 validio_cli-0.6.3/PKG-INFO
+-rw-r--r--   0        0        0    11340 2023-07-21 13:06:24.618756 validio_cli-0.6.4/LICENSE
+-rw-r--r--   0        0        0      227 2023-07-21 13:06:24.618756 validio_cli-0.6.4/README_PUBLIC.md
+-rw-r--r--   0        0        0     1987 2023-07-21 13:06:36.369747 validio_cli-0.6.4/pyproject.toml
+-rw-r--r--   0        0        0     6274 2023-07-21 13:06:24.619756 validio_cli-0.6.4/validio_cli/__init__.py
+-rw-r--r--   0        0        0     2390 2023-07-21 13:06:24.619756 validio_cli-0.6.4/validio_cli/bin/entities/channels.py
+-rw-r--r--   0        0        0    14086 2023-07-21 13:06:24.619756 validio_cli-0.6.4/validio_cli/bin/entities/code.py
+-rw-r--r--   0        0        0     4335 2023-07-21 13:06:24.619756 validio_cli-0.6.4/validio_cli/bin/entities/config.py
+-rw-r--r--   0        0        0     2506 2023-07-21 13:06:24.619756 validio_cli-0.6.4/validio_cli/bin/entities/credentials.py
+-rw-r--r--   0        0        0     2306 2023-07-21 13:06:24.619756 validio_cli-0.6.4/validio_cli/bin/entities/destinations.py
+-rw-r--r--   0        0        0     7429 2023-07-21 13:06:24.619756 validio_cli-0.6.4/validio_cli/bin/entities/incidents.py
+-rw-r--r--   0        0        0     2336 2023-07-21 13:06:24.619756 validio_cli-0.6.4/validio_cli/bin/entities/metrics.py
+-rw-r--r--   0        0        0     2867 2023-07-21 13:06:24.619756 validio_cli-0.6.4/validio_cli/bin/entities/notification_rules.py
+-rw-r--r--   0        0        0     3334 2023-07-21 13:06:24.619756 validio_cli-0.6.4/validio_cli/bin/entities/recommendations.py
+-rw-r--r--   0        0        0     3961 2023-07-21 13:06:24.619756 validio_cli-0.6.4/validio_cli/bin/entities/resources.py
+-rw-r--r--   0        0        0     2913 2023-07-21 13:06:24.619756 validio_cli-0.6.4/validio_cli/bin/entities/segmentations.py
+-rw-r--r--   0        0        0     1902 2023-07-21 13:06:24.619756 validio_cli-0.6.4/validio_cli/bin/entities/segments.py
+-rw-r--r--   0        0        0    26341 2023-07-21 13:06:24.620756 validio_cli-0.6.4/validio_cli/bin/entities/sources.py
+-rw-r--r--   0        0        0     1174 2023-07-21 13:06:24.620756 validio_cli-0.6.4/validio_cli/bin/entities/users.py
+-rw-r--r--   0        0        0     3743 2023-07-21 13:06:24.620756 validio_cli-0.6.4/validio_cli/bin/entities/validators.py
+-rw-r--r--   0        0        0     2806 2023-07-21 13:06:24.620756 validio_cli-0.6.4/validio_cli/bin/entities/windows.py
+-rw-r--r--   0        0        0     3343 2023-07-21 13:06:24.620756 validio_cli-0.6.4/validio_cli/bin/main.py
+-rw-r--r--   0        0        0     3096 2023-07-21 13:06:24.620756 validio_cli-0.6.4/validio_cli/components.py
+-rw-r--r--   0        0        0      265 2023-07-21 13:06:24.620756 validio_cli-0.6.4/validio_cli/metadata.py
+-rw-r--r--   0        0        0      630 2023-07-21 13:06:24.620756 validio_cli-0.6.4/validio_cli/namespace.py
+-rw-r--r--   0        0        0     1382 2023-07-21 13:06:24.620756 validio_cli-0.6.4/validio_cli/schema.py
+-rw-r--r--   0        0        0     1116 1970-01-01 00:00:00.000000 validio_cli-0.6.4/PKG-INFO
```

### Comparing `validio_cli-0.6.3/LICENSE` & `validio_cli-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `validio_cli-0.6.3/pyproject.toml` & `validio_cli-0.6.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "validio-cli"
 # This version does not represent the released version or any tag. For each
 # release we automatically bump this before building and publishing so this
 # should be kept at 0.0.1dev1
-version = "0.6.3"
+version = "0.6.4"
 description = "CLI tool to interact with the Validio platform"
 authors = ["Validio <support@validio.io>"]
 license = "Apache-2.0"
 homepage = "https://validio.io/"
 documentation = "https://docs.validio.io/"
 packages = [{include = "validio_cli"}]
 readme = "README_PUBLIC.md"
```

### Comparing `validio_cli-0.6.3/validio_cli/__init__.py` & `validio_cli-0.6.4/validio_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `validio_cli-0.6.3/validio_cli/bin/entities/channels.py` & `validio_cli-0.6.4/validio_cli/bin/entities/channels.py`

 * *Files identical despite different names*

### Comparing `validio_cli-0.6.3/validio_cli/bin/entities/code.py` & `validio_cli-0.6.4/validio_cli/bin/entities/code.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,25 +2,27 @@
 import re
 import sys
 from collections.abc import Mapping
 from enum import Enum
 from typing import Any
 
 import classdiff  # type: ignore
-import prompt_toolkit
 import typer
+from validio_sdk.code import _import as code_import
 from validio_sdk.code import apply as code_apply
 from validio_sdk.code import plan as code_plan
 from validio_sdk.code import scaffold
 from validio_sdk.resource._diff import DiffContext, GraphDiff, ResourceUpdate
 from validio_sdk.resource._resource import Resource
 from validio_sdk.resource._util import SourceSchemaReinference
 from validio_sdk.validio_client import ValidioAPIClient
 
 from validio_cli import AsyncTyper, ConfigDir, get_client_and_config
+from validio_cli.bin.entities.resources import do_move
+from validio_cli.components import proceed_with_operation
 
 app = AsyncTyper(help="Plan or apply your configuration")
 
 
 class DiffOutput(str, Enum):
     """Available output formats for the CLI"""
 
@@ -167,24 +169,16 @@
         diff_output=diff_output,
         show_secrets=show_secrets,
     )
 
     if diff.num_operations() == 0:
         return
 
-    print()
-    print("Do you want to perform these operations?")
-    print("\tOnly 'yes' is accepted to approve")
-
-    if not auto_approve:
-        session: prompt_toolkit.PromptSession = prompt_toolkit.PromptSession()
-        p = await session.prompt_async("Enter a value: ")
-        if p != "yes":
-            print("Cancelled")
-            return
+    if not await proceed_with_operation(auto_approve):
+        return
 
     print()
     print("Applying...")
 
     await code_apply.apply(
         namespace=namespace,
         client=client,
@@ -195,14 +189,94 @@
 
     print(
         f"Apply complete! Resources: {diff.num_creates()} created, "
         f"{diff.num_updates()} updated, {diff.num_deletes()} deleted"
     )
 
 
+@app.async_command(name="import", help="Import resources into the current project")
+async def _import(
+    directory: str = directory_option,
+    no_capture: bool = no_capture_option,
+    config_dir: str = ConfigDir,
+    output: pathlib.Path = typer.Option(
+        ...,
+        "--output",
+        "-o",
+        help=(
+            "The path to the file that will contain the generated resource declarations"
+        ),
+    ),
+    import_namespace: str = typer.Option(
+        None,
+        "--import-namespace",
+        help=(
+            "If providing file to move resources, this is a mandatory parameter"
+            " specifying the namespace containing those resources."
+        ),
+    ),
+    file: pathlib.Path = typer.Option(
+        None,
+        "--file",
+        "-f",
+        help=(
+            "Path to a JSON-encoded file containing a list of resource to be"
+            " moved into the current project before generating resource declarations."
+            " If provided, then --import-namespace must be specified"
+        ),
+    ),
+    auto_approve: bool = typer.Option(
+        False, help="Automatically approve and perform the import operation"
+    ),
+):
+    if (file is None) is not (import_namespace is None):
+        raise Exception(
+            "--import-namespace must be provided if -f is provided and vice versa"
+        )
+
+    dir_path = directory_or_default(directory)
+    client, _ = await get_client_and_config(config_dir)
+
+    namespace = get_namespace(dir_path)
+
+    if file and import_namespace:
+        num_moved_resources = await do_move(
+            client=client,
+            namespace=import_namespace,
+            target_namespace=namespace,
+            file=file,
+            auto_approve=auto_approve,
+        )
+        if num_moved_resources is None:
+            return
+
+        if num_moved_resources > 0:
+            print(f"Moved {num_moved_resources} resources")
+
+    diff, manifest_ctx = await _plan(
+        namespace=namespace,
+        client=client,
+        directory=dir_path,
+        schema_reinference=create_source_schema_reinference([], False),
+        destroy=False,
+        no_capture=no_capture,
+        show_schema=False,
+        show_secrets=False,
+        show_diff=False,
+    )
+
+    if diff.num_deletes() == 0:
+        _print_no_changes()
+        return
+
+    s = await code_import._import(ctx=diff.to_delete)
+    output.write_text(s)
+    print(f"Generated file {output.absolute()}")
+
+
 def get_namespace(directory: pathlib.Path) -> str:
     settings = scaffold._read_project_settings(directory)
     return settings.namespace
 
 
 def directory_or_default(directory: str) -> pathlib.Path:
     return (pathlib.Path(directory) if directory else pathlib.Path.cwd()).absolute()
@@ -214,36 +288,38 @@
     directory: pathlib.Path,
     schema_reinference: SourceSchemaReinference,
     destroy: bool,
     no_capture: bool,
     show_schema: bool = False,
     diff_output: DiffOutput = DiffOutput.FULL,
     show_secrets: bool = False,
+    show_diff: bool = True,
 ) -> tuple[GraphDiff, DiffContext]:
     (diff, manifest_ctx) = await code_plan.plan(
         namespace=namespace,
         client=client,
         directory=directory,
         schema_reinference=schema_reinference,
         destroy=destroy,
         no_capture=no_capture,
         show_secrets=show_secrets,
     )
 
-    if diff.num_operations() == 0:
-        print("No changes. The configuration is up-to-date!")
-        return diff, manifest_ctx
-
-    _show_resources_diff(
-        diff=diff,
-        show_schema=show_schema,
-        show_secrets=show_secrets,
-        escape=sys.stdout.isatty(),
-        diff_output=diff_output,
-    )
+    if show_diff:
+        if diff.num_operations() == 0:
+            _print_no_changes()
+            return diff, manifest_ctx
+
+        _show_resources_diff(
+            diff=diff,
+            show_schema=show_schema,
+            show_secrets=show_secrets,
+            escape=sys.stdout.isatty(),
+            diff_output=diff_output,
+        )
 
     return diff, manifest_ctx
 
 
 # https://stackoverflow.com/a/14693789/2274551
 ansi_escape = re.compile(
     r"""
@@ -410,9 +486,13 @@
         source_names = []
     elif len(schemas_to_update) > 0:
         source_names = schemas_to_update
 
     return SourceSchemaReinference(set(source_names) if source_names else None)
 
 
+def _print_no_changes():
+    print("No changes. The configuration is up-to-date!")
+
+
 if __name__ == "__main__":
     app()
```

### Comparing `validio_cli-0.6.3/validio_cli/bin/entities/config.py` & `validio_cli-0.6.4/validio_cli/bin/entities/config.py`

 * *Files identical despite different names*

### Comparing `validio_cli-0.6.3/validio_cli/bin/entities/credentials.py` & `validio_cli-0.6.4/validio_cli/bin/entities/credentials.py`

 * *Files identical despite different names*

### Comparing `validio_cli-0.6.3/validio_cli/bin/entities/destinations.py` & `validio_cli-0.6.4/validio_cli/bin/entities/destinations.py`

 * *Files identical despite different names*

### Comparing `validio_cli-0.6.3/validio_cli/bin/entities/incidents.py` & `validio_cli-0.6.4/validio_cli/bin/entities/incidents.py`

 * *Files identical despite different names*

### Comparing `validio_cli-0.6.3/validio_cli/bin/entities/metrics.py` & `validio_cli-0.6.4/validio_cli/bin/entities/metrics.py`

 * *Files identical despite different names*

### Comparing `validio_cli-0.6.3/validio_cli/bin/entities/notification_rules.py` & `validio_cli-0.6.4/validio_cli/bin/entities/notification_rules.py`

 * *Files identical despite different names*

### Comparing `validio_cli-0.6.3/validio_cli/bin/entities/recommendations.py` & `validio_cli-0.6.4/validio_cli/bin/entities/recommendations.py`

 * *Files identical despite different names*

### Comparing `validio_cli-0.6.3/validio_cli/bin/entities/segmentations.py` & `validio_cli-0.6.4/validio_cli/bin/entities/segmentations.py`

 * *Files identical despite different names*

### Comparing `validio_cli-0.6.3/validio_cli/bin/entities/segments.py` & `validio_cli-0.6.4/validio_cli/bin/entities/segments.py`

 * *Files identical despite different names*

### Comparing `validio_cli-0.6.3/validio_cli/bin/entities/sources.py` & `validio_cli-0.6.4/validio_cli/bin/entities/sources.py`

 * *Files identical despite different names*

### Comparing `validio_cli-0.6.3/validio_cli/bin/entities/users.py` & `validio_cli-0.6.4/validio_cli/bin/entities/users.py`

 * *Files identical despite different names*

### Comparing `validio_cli-0.6.3/validio_cli/bin/entities/validators.py` & `validio_cli-0.6.4/validio_cli/bin/entities/validators.py`

 * *Files identical despite different names*

### Comparing `validio_cli-0.6.3/validio_cli/bin/entities/windows.py` & `validio_cli-0.6.4/validio_cli/bin/entities/windows.py`

 * *Files identical despite different names*

### Comparing `validio_cli-0.6.3/validio_cli/bin/main.py` & `validio_cli-0.6.4/validio_cli/bin/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     code,
     credentials,
     destinations,
     incidents,
     metrics,
     notification_rules,
     recommendations,
+    resources,
     segmentations,
     segments,
     sources,
     users,
     validators,
     windows,
 )
@@ -33,14 +34,15 @@
 
 app.add_typer(channels.app, no_args_is_help=True, name="channels")
 app.add_typer(code.app, no_args_is_help=True, name="code")
 app.add_typer(credentials.app, no_args_is_help=True, name="credentials")
 app.add_typer(destinations.app, no_args_is_help=True, name="destinations")
 app.add_typer(incidents.app, no_args_is_help=True, name="incidents")
 app.add_typer(metrics.app, no_args_is_help=True, name="metrics")
+app.add_typer(resources.app, no_args_is_help=True, name="resources")
 app.add_typer(notification_rules.app, no_args_is_help=True, name="notification-rules")
 app.add_typer(recommendations.app, no_args_is_help=True, name="recommendations")
 app.add_typer(segmentations.app, no_args_is_help=True, name="segmentations")
 app.add_typer(segments.app, no_args_is_help=True, name="segments")
 app.add_typer(sources.app, no_args_is_help=True, name="sources")
 app.add_typer(users.app, no_args_is_help=True, name="users")
 app.add_typer(validators.app, no_args_is_help=True, name="validators")
```

### Comparing `validio_cli-0.6.3/validio_cli/components.py` & `validio_cli-0.6.4/validio_cli/components.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Components for the CLI."""
+from prompt_toolkit import PromptSession
 from prompt_toolkit.application import Application
 from prompt_toolkit.key_binding.defaults import load_key_bindings
 from prompt_toolkit.key_binding.key_bindings import KeyBindings, merge_key_bindings
 from prompt_toolkit.layout import Layout
 from prompt_toolkit.layout.containers import HSplit
 from prompt_toolkit.styles.base import BaseStyle
 from prompt_toolkit.widgets import Label, RadioList
@@ -74,7 +75,25 @@
         full_screen=False,
     )
 
     if async_:
         return application.run_async()
 
     return application.run()
+
+
+async def proceed_with_operation(auto_approve: bool) -> bool:
+    """Request confirmation before performing an operation."""
+    if auto_approve:
+        return True
+
+    print()
+    print("Do you want to perform these operations?")
+    print("\tOnly 'yes' is accepted to approve")
+
+    session: PromptSession = PromptSession()
+    p = await session.prompt_async("Enter a value: ")
+    if p != "yes":
+        print("Cancelled")
+        return False
+
+    return True
```

### Comparing `validio_cli-0.6.3/validio_cli/namespace.py` & `validio_cli-0.6.4/validio_cli/namespace.py`

 * *Files identical despite different names*

### Comparing `validio_cli-0.6.3/validio_cli/schema.py` & `validio_cli-0.6.4/validio_cli/schema.py`

 * *Files identical despite different names*

### Comparing `validio_cli-0.6.3/PKG-INFO` & `validio_cli-0.6.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: validio-cli
-Version: 0.6.3
+Version: 0.6.4
 Summary: CLI tool to interact with the Validio platform
 Home-page: https://validio.io/
 License: Apache-2.0
 Author: Validio
 Author-email: support@validio.io
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

