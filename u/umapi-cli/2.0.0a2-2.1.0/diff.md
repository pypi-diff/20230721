# Comparing `tmp/umapi_cli-2.0.0a2.tar.gz` & `tmp/umapi_cli-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "umapi_cli-2.0.0a2.tar", max compression
+gzip compressed data, was "umapi_cli-2.1.0.tar", max compression
```

## Comparing `umapi_cli-2.0.0a2.tar` & `umapi_cli-2.1.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    11335 2023-06-21 15:28:39.518313 umapi_cli-2.0.0a2/LICENSE
--rw-r--r--   0        0        0    24216 2023-06-29 22:55:29.426631 umapi_cli-2.0.0a2/README.md
--rw-r--r--   0        0        0      705 2023-06-30 05:28:16.965493 umapi_cli-2.0.0a2/pyproject.toml
--rw-r--r--   0        0        0      603 2023-06-21 16:29:58.311507 umapi_cli-2.0.0a2/umapi_cli/__init__.py
--rw-r--r--   0        0        0     3919 2023-06-29 00:01:19.698699 umapi_cli-2.0.0a2/umapi_cli/action_queue.py
--rw-r--r--   0        0        0    16607 2023-06-30 04:10:34.672428 umapi_cli-2.0.0a2/umapi_cli/cli.py
--rw-r--r--   0        0        0     1318 2023-06-21 16:29:28.366519 umapi_cli-2.0.0a2/umapi_cli/client.py
--rw-r--r--   0        0        0     1253 2023-06-21 16:29:35.143777 umapi_cli-2.0.0a2/umapi_cli/config.py
--rw-r--r--   0        0        0     5834 2023-06-28 23:07:34.517123 umapi_cli-2.0.0a2/umapi_cli/formatter.py
--rw-r--r--   0        0        0     1298 2023-06-21 16:29:14.623535 umapi_cli-2.0.0a2/umapi_cli/log.py
--rw-r--r--   0        0        0      628 2023-06-30 04:26:09.885809 umapi_cli-2.0.0a2/umapi_cli/version.py
--rw-r--r--   0        0        0    24970 1970-01-01 00:00:00.000000 umapi_cli-2.0.0a2/PKG-INFO
+-rw-r--r--   0        0        0    11335 2023-06-21 15:28:39.518313 umapi_cli-2.1.0/LICENSE
+-rw-r--r--   0        0        0    24835 2023-07-20 21:06:38.504997 umapi_cli-2.1.0/README.md
+-rw-r--r--   0        0        0      705 2023-07-20 23:33:25.470732 umapi_cli-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0      603 2023-06-21 16:29:58.311507 umapi_cli-2.1.0/umapi_cli/__init__.py
+-rw-r--r--   0        0        0     4036 2023-07-11 14:46:22.788370 umapi_cli-2.1.0/umapi_cli/action_queue.py
+-rw-r--r--   0        0        0    19409 2023-07-20 22:42:50.788101 umapi_cli-2.1.0/umapi_cli/cli.py
+-rw-r--r--   0        0        0     1504 2023-07-20 17:33:12.989018 umapi_cli-2.1.0/umapi_cli/client.py
+-rw-r--r--   0        0        0     1253 2023-06-21 16:29:35.143777 umapi_cli-2.1.0/umapi_cli/config.py
+-rw-r--r--   0        0        0     6167 2023-07-20 21:06:38.505918 umapi_cli-2.1.0/umapi_cli/formatter.py
+-rw-r--r--   0        0        0     1298 2023-06-21 16:29:14.623535 umapi_cli-2.1.0/umapi_cli/log.py
+-rw-r--r--   0        0        0      626 2023-07-20 23:33:17.625349 umapi_cli-2.1.0/umapi_cli/version.py
+-rw-r--r--   0        0        0    25587 1970-01-01 00:00:00.000000 umapi_cli-2.1.0/PKG-INFO
```

### Comparing `umapi_cli-2.0.0a2/LICENSE` & `umapi_cli-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `umapi_cli-2.0.0a2/README.md` & `umapi_cli-2.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,28 @@
+Metadata-Version: 2.1
+Name: umapi-cli
+Version: 2.1.0
+Summary: User Management API CLI Tool
+Home-page: https://github.com/adobe/umapi-cli/
+License: Apache 2.0
+Author: Andrew Dorton
+Author-email: adorton@adobe.com
+Requires-Python: >=3.9,<4.0
+Classifier: License :: Other/Proprietary License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: click (>=8.0,<9.0)
+Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
+Requires-Dist: schema (>=0.7.5,<0.8.0)
+Requires-Dist: umapi-client (>=3.0,<4.0)
+Project-URL: Repository, https://github.com/adobe/umapi-cli/
+Description-Content-Type: text/markdown
+
 # User Management API CLI Tool
 
 A simple command-line interface (CLI) client to the
 [Adobe User Management API](https://adobe-apiplatform.github.io/umapi-documentation/en/).
 
 ## Table of Contents
 
@@ -81,14 +102,17 @@
 
 ## Option 2 - Executable
 
 A self-contained executable is also available for Windows and macOS. The
 executable embeds a Python environment, so Python does not need to be installed
 on the system. Note that this build is slower to start when executing the tool.
 
+Executables can be found on the [latest
+releases](https://github.com/adobe/umapi-cli/releases/latest) page.
+
 # Usage Overview
 
 The tool operates on a series of commands. Each command performs a certain
 operation - read single user, read all users, create user/group, etc.
 
 ```
 $ umapi --help
@@ -236,14 +260,19 @@
 
 Options:
   -h, --help                    Show this message and exit.
   -f, --format csv|json|pretty  Output format  [default: pretty]
   -e, --email TEXT              User email address  [required]
 ```
 
+**Note:** The CSV format for `user-read` is the same as `user-read-all` ([see
+below](#user-read-all)) with the exception of the `tags` column. This column can
+currently only be read on a user-by-user basis and thus is not included in
+`user-read-all` results.
+
 ## `user-read-all`
 
 Get details for all users in a given console. 
 
 Formats: [JSONL](http://jsonlines.org), CSV, or human-readable (default).
 
 This command writes to stdout by default, but can optionally write output to a
@@ -743,13 +772,19 @@
    
 To run the tool from source:
 
 1. Ensure dependencies are up to date with `poetry install`.
 2. Prefix invocations of the `umapi` command with `poetry run` (e.g. `poetry run
    umapi --help`). This runs the `umapi` entrypoint from the project's virtual
    environment.
+   
+> **Note:** if you are doing development work on the tool and wish to see full
+> error information when an error occurs, set the `UMAPI_DEBUG` environment
+> variable to `1`. This will dump more information on the error including a
+> stack trace.
 
 # Getting Help
 
 Should you run into any issues using this tool, or have any questions or
 comments, please create an [issue](https://github.com/adobe/umapi-cli/issues) to
 contact the development team.
+
```

### Comparing `umapi_cli-2.0.0a2/pyproject.toml` & `umapi_cli-2.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "umapi-cli"
-version = "2.0.0a2"
+version = "2.1.0"
 description = "User Management API CLI Tool"
 authors = ["Andrew Dorton <adorton@adobe.com>"]
 license = "Apache 2.0"
 readme = "README.md"
 repository = "https://github.com/adobe/umapi-cli/"
 
 [tool.poetry.dependencies]
@@ -18,11 +18,11 @@
 pytest = "^6.0"
 pyinstaller = { version = "^5.13.0", python = ">=3.9,<3.13" }
 pywin32-ctypes = "^0.2.0"
 pefile = "^2022.5"
 macholib = {version = "^1.16.2", platform = "darwin"}
 
 [tool.poetry.scripts]
-umapi = 'umapi_cli.cli:app'
+umapi = 'umapi_cli.cli:entry'
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
```

### Comparing `umapi_cli-2.0.0a2/umapi_cli/__init__.py` & `umapi_cli-2.1.0/umapi_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `umapi_cli-2.0.0a2/umapi_cli/action_queue.py` & `umapi_cli-2.1.0/umapi_cli/action_queue.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,19 +25,21 @@
         self.actions.append(user_action)
 
     def execute(self):
         completed = 0
         queued = len(self.actions)
         log.info(f'Number of actions to execute: {len(self.actions)}')
         for action in self.actions:
-            _, _, c = self.conn.execute_single(action)
-            if c > 0:
-                completed += c
-                log.info(f"Completion: {completed}/{queued} ({round(completed/queued*100, 2)}%)")
-        _, _, c = self.conn.execute_queued()
+            self.conn.execute_single(action)
+            completed += 1
+            if completed % 10 == 0:
+                log.info(f"Executed actions: {completed}/{queued} ({round(completed/queued*100, 2)}%)")
+        self.conn.execute_queued()
+        log.info(f"Executed actions: {completed}/{queued} ({round(completed/queued*100, 2)}%)")
+        return completed
 
     def errors(self):
         return [a.execution_errors() for a in self.actions if a.execution_errors()]
 
     def queue_user_create_action(self, id_type, email, country, firstname=None,
                                  lastname=None, username=None, domain=None, groups=None):
         if username is None or len(username) == 0:
```

### Comparing `umapi_cli-2.0.0a2/umapi_cli/cli.py` & `umapi_cli-2.1.0/umapi_cli/cli.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,22 +6,24 @@
 # Unless required by applicable law or agreed to in writing, software distributed under
 # the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR REPRESENTATIONS
 # OF ANY KIND, either express or implied. See the License for the specific language
 # governing permissions and limitations under the License.
 
 import click
 import sys
+import io
+import os
 from umapi_client import UserQuery, UsersQuery, GroupsQuery
 import dotenv
 from pathlib import Path
 from umapi_cli import config
 from umapi_cli import client
 from umapi_cli import formatter
 from umapi_cli.action_queue import ActionQueue
-from umapi_cli.formatter import normalize, InputHandler, OutputHandler
+from umapi_cli.formatter import normalize, InputHandler, OutputHandler, PassthroughHandler
 from umapi_cli import log
 from umapi_cli.version import __version__ as app_version
 
 def _formatter(data_format, fh, handler):
     fmtr_class = getattr(formatter, data_format, None)
     if fmtr_class is None:
         click.echo("Unknown format '{}'".format(data_format))
@@ -35,14 +37,22 @@
     return sys.stdout
 
 
 def _input_fh(in_file):
     return open(in_file, 'r')
 
 
+def infer_format(filename):
+    if filename.endswith('csv'):
+        return 'csv'
+    if filename.endswith('json') or filename.endswith('jsonl'):
+        return 'json'
+    return None
+
+
 @click.group()
 @click.option('--env', 'env_file', help="Path to .env file (optional)", default=None, type=click.Path())
 @click.option('-t', '--test', 'test_mode', help="Run command in test mode", default=False, show_default=False,
               is_flag=True)
 @click.option('-v', count=True, help="Enable verbose logging")
 @click.help_option('-h', '--help')
 @click.version_option(app_version, '--version', message='%(prog)s %(version)s')
@@ -56,14 +66,25 @@
         if env_file:
             dotenv.load_dotenv(env_file)
     ctx.ensure_object(dict)
     conf = config.get_options()
     ctx.obj['conn'] = client.create_conn(conf, test_mode)
 
 
+def entry():
+    debug = True if os.environ.get('UMAPI_DEBUG') == '1' else False
+    try:
+        app()
+    except Exception as e:
+        if not debug:
+            click.echo(f"ERROR: {e}")
+        else:
+            raise e
+
+
 @app.command()
 @click.help_option('-h', '--help')
 @click.option('-f', '--format', 'output_format', help='Output format', metavar='csv|json|pretty', default='pretty',
               show_default=True)
 @click.option('-e', '--email', help='User email address', required=True)
 @click.pass_context
 def user_read(ctx, output_format, email):
@@ -77,22 +98,26 @@
         sys.exit(1)
     fmtr.record(user)
     fmtr.write()
 
 
 @app.command()
 @click.help_option('-h', '--help')
-@click.option('-f', '--format', 'output_format', help='Output format', metavar='csv|json|pretty', default='pretty',
-              show_default=True)
+@click.option('-f', '--format', 'output_format', help='Output format', metavar='csv|json|pretty', show_default=True)
 @click.option('-o', '--out-file', help='Write output to this filename', metavar='FILENAME')
 @click.pass_context
 def user_read_all(ctx, output_format, out_file):
     """Get details for all users belonging to a console"""
 
-    fmtr = _formatter(output_format, _output_fh(out_file), OutputHandler('user_read'))
+    if out_file is not None:
+        output_format = infer_format(out_file)
+    if output_format is None:
+        output_format = 'pretty'
+
+    fmtr = _formatter(output_format, _output_fh(out_file), OutputHandler('user_read_all'))
     umapi_conn = ctx.obj['conn']
     query = UsersQuery(umapi_conn)
     report_total = True
     for user in query:
         total, *_ = query.stats()
         if total is not None and report_total:
             log.info(f"Total records: {total}")
@@ -119,21 +144,26 @@
         fmtr.write()
     else:
         click.echo(f"Group '{group_name}' not found")
 
 
 @app.command()
 @click.help_option('-h', '--help')
-@click.option('-f', '--format', 'output_format', help='Output format', metavar='csv|json|pretty', default='pretty',
+@click.option('-f', '--format', 'output_format', help='Output format', metavar='csv|json|pretty',
               show_default=True)
 @click.option('-o', '--out-file', help='Write output to this filename', metavar='FILENAME')
 @click.pass_context
 def group_read_all(ctx, output_format, out_file):
     """Get details for all groups in a console"""
 
+    if out_file is not None:
+        output_format = infer_format(out_file)
+    if output_format is None:
+        output_format = 'pretty'
+
     fmtr = _formatter(output_format, _output_fh(out_file), OutputHandler('group_read'))
     umapi_conn = ctx.obj['conn']
     query = GroupsQuery(umapi_conn)
     for group in query:
         fmtr.record(group)
     fmtr.write()
 
@@ -171,15 +201,20 @@
     if groups is None:
         groups = []
     else:
         groups = groups.split(',')
     queue.queue_user_create_action(user_type, email, country, firstname, lastname,
                                    username, domain, groups)
     queue.execute()
-    click.echo("errors: {}".format(queue.errors()))
+    errors = queue.errors()
+    if errors:
+        click.echo("One or more errors occurred")
+        click.echo(render_errors(errors).strip())
+    else:
+        click.echo("Create operation succeeded")
 
 
 @app.command()
 @click.help_option('-h', '--help')
 @click.option('-f', '--format', 'input_format', help='Input file format', metavar='csv|json', default='csv',
               show_default=True)
 @click.option('-i', '--in-file', help='Input filename', metavar='FILENAME')
@@ -195,17 +230,17 @@
             user['domain'] = None
         queue.queue_user_create_action(id_type=user['type'],
                                        email=user['email'], username=user['username'],
                                        domain=user['domain'], groups=user['groups'],
                                        firstname=user['firstname'],
                                        lastname=user['lastname'],
                                        country=user['country'])
-    queue.execute()
-    for err in queue.errors():
-        click.echo("Error: {}".format(err))
+    completed = queue.execute()
+    errors = queue.errors()
+    print_bulk_summaries(completed, errors)
 
 
 @app.command()
 @click.help_option('-h', '--help')
 @click.option('-e', '--email', help='User email address', required=True)
 @click.option('-d', '--hard', 'hard_delete',
               help="Delete user from underlying directory instead of just the org level",
@@ -214,15 +249,20 @@
 def user_delete(ctx, email, hard_delete):
     """Delete a single user (from org and/or identity directory)"""
 
     umapi_conn = ctx.obj['conn']
     queue = ActionQueue(umapi_conn)
     queue.queue_delete_action(email, hard_delete)
     queue.execute()
-    click.echo("errors: {}".format(queue.errors()))
+    errors = queue.errors()
+    if errors:
+        click.echo("One or more errors occurred")
+        click.echo(render_errors(errors).strip())
+    else:
+        click.echo("Delete operation succeeded")
 
 
 @app.command()
 @click.help_option('-h', '--help')
 @click.option('-f', '--format', 'input_format', help='Input file format', metavar='csv|json', default='csv',
               show_default=True)
 @click.option('-i', '--in-file', help='Input filename', metavar='FILENAME')
@@ -232,17 +272,17 @@
 
     fmtr = _formatter(input_format, _input_fh(in_file), InputHandler('user_delete_bulk'))
     umapi_conn = ctx.obj['conn']
     queue = ActionQueue(umapi_conn)
     for user in fmtr.read():
         queue.queue_delete_action(user['email'],
                                   True if user['hard_delete'] == 'y' else False)
-    queue.execute()
-    for err in queue.errors():
-        click.echo("Error: {}".format(err))
+    completed = queue.execute()
+    errors = queue.errors()
+    print_bulk_summaries(completed, errors)
 
 
 @app.command()
 @click.help_option('-h', '--help')
 @click.option('-e', '--email', help='Email address that identifies the user', required=True)
 @click.option('-E', '--email-new', help="Updated email address", required=False)
 @click.option('-f', '--firstname', help="Updated given (first) name", required=False)
@@ -260,15 +300,20 @@
         groups_add = groups_add.split(',')
     if groups_remove is not None:
         groups_remove = groups_remove.split(',')
     queue.queue_update_action(email, email_new=email_new, firstname=firstname,
                               lastname=lastname, username=username, add_groups=groups_add,
                               remove_groups=groups_remove)
     queue.execute()
-    click.echo("errors: {}".format(queue.errors()))
+    errors = queue.errors()
+    if errors:
+        click.echo("One or more errors occurred")
+        click.echo(render_errors(errors).strip())
+    else:
+        click.echo("Update operation succeeded")
 
 
 @app.command()
 @click.help_option('-h', '--help')
 @click.option('-f', '--format', 'input_format', help='Input file format', metavar='csv|json', default='csv',
               show_default=True)
 @click.option('-i', '--in-file', help='Input filename', metavar='FILENAME')
@@ -277,17 +322,17 @@
     """Update users in bulk from input file"""
 
     fmtr = _formatter(input_format, _input_fh(in_file), InputHandler('user_update_bulk'))
     umapi_conn = ctx.obj['conn']
     queue = ActionQueue(umapi_conn)
     for user in fmtr.read():
         queue.queue_update_action(**user)
-    queue.execute()
-    for err in queue.errors():
-        click.echo("Error: {}".format(err))
+    completed = queue.execute()
+    errors = queue.errors()
+    print_bulk_summaries(completed, errors)
 
 
 @app.command()
 @click.help_option('-h', '--help')
 @click.option('--name', help="Name of group", required=True)
 @click.option('--description', help="Optional group description")
 @click.pass_context
@@ -301,15 +346,20 @@
              --description "Stock provisioning group"
     """
 
     umapi_conn = ctx.obj['conn']
     queue = ActionQueue(umapi_conn)
     queue.queue_group_create_action(name, description)
     queue.execute()
-    click.echo("errors: {}".format(queue.errors()))
+    errors = queue.errors()
+    if errors:
+        click.echo("One or more errors occurred")
+        click.echo(render_errors(errors).strip())
+    else:
+        click.echo("Create operation succeeded")
 
 
 @app.command()
 @click.help_option('-h', '--help')
 @click.option('-f', '--format', 'input_format', help='Input file format', metavar='csv|json', default='csv',
               show_default=True)
 @click.option('-i', '--in-file', help='Input filename', metavar='FILENAME')
@@ -318,17 +368,17 @@
     """Create groups in bulk from an input file"""
 
     fmtr = _formatter(input_format, _input_fh(in_file), InputHandler('group_create_bulk'))
     umapi_conn = ctx.obj['conn']
     queue = ActionQueue(umapi_conn)
     for group in fmtr.read():
         queue.queue_group_create_action(group['name'], group['description'])
-    queue.execute()
-    for err in queue.errors():
-        click.echo("Error: {}".format(err))
+    completed = queue.execute()
+    errors = queue.errors()
+    print_bulk_summaries(completed, errors)
 
 
 @app.command()
 @click.help_option('-h', '--help')
 @click.option('-n', '--name', help='Current name of group', required=True)
 @click.option('-N', '--name-new', help="New name to assign group", required=False)
 @click.option('-d', '--description', help="Updated group description", required=False)
@@ -350,15 +400,20 @@
         profiles_add = profiles_add.split(',')
     if profiles_remove is not None:
         profiles_remove = profiles_remove.split(',')
     queue.queue_group_update_action(name, name_new=name_new,
                                     description=description, add_users=users_add, remove_users=users_remove,
                                     add_profiles=profiles_add, remove_profiles=profiles_remove)
     queue.execute()
-    click.echo("errors: {}".format(queue.errors()))
+    errors = queue.errors()
+    if errors:
+        click.echo("One or more errors occurred")
+        click.echo(render_errors(errors).strip())
+    else:
+        click.echo("Update operation succeeded")
 
 
 @app.command()
 @click.help_option('-h', '--help')
 @click.option('-f', '--format', 'input_format', help='Input file format', metavar='csv|json', default='csv',
               show_default=True)
 @click.option('-i', '--in-file', help='Input filename', metavar='FILENAME')
@@ -367,31 +422,36 @@
     """Update groups in bulk from input file"""
 
     fmtr = _formatter(input_format, _input_fh(in_file), InputHandler('group_update_bulk'))
     umapi_conn = ctx.obj['conn']
     queue = ActionQueue(umapi_conn)
     for group in fmtr.read():
         queue.queue_group_update_action(**group)
-    queue.execute()
-    for err in queue.errors():
-        click.echo("Error: {}".format(err))
+    completed = queue.execute()
+    errors = queue.errors()
+    print_bulk_summaries(completed, errors)
 
 
 @app.command()
 @click.help_option('-h', '--help')
 @click.option('-n', '--name', help='Group name', required=True)
 @click.pass_context
 def group_delete(ctx, name):
     """Delete a single user group"""
 
     umapi_conn = ctx.obj['conn']
     queue = ActionQueue(umapi_conn)
     queue.queue_group_delete_action(name)
     queue.execute()
-    click.echo("errors: {}".format(queue.errors()))
+    errors = queue.errors()
+    if errors:
+        click.echo("One or more errors occurred")
+        click.echo(render_errors(errors).strip())
+    else:
+        click.echo("Delete operation succeeded")
 
 
 @app.command()
 @click.help_option('-h', '--help')
 @click.option('-f', '--format', 'input_format', help='Input file format', metavar='csv|json', default='csv',
               show_default=True)
 @click.option('-i', '--in-file', help='Input filename', metavar='FILENAME')
@@ -400,14 +460,54 @@
     """Delete groups in bulk from input file"""
 
     fmtr = _formatter(input_format, _input_fh(in_file), InputHandler('group_delete_bulk'))
     umapi_conn = ctx.obj['conn']
     queue = ActionQueue(umapi_conn)
     for group in fmtr.read():
         queue.queue_group_delete_action(group['name'])
-    queue.execute()
-    for err in queue.errors():
-        click.echo("Error: {}".format(err))
+    completed = queue.execute()
+    errors = queue.errors()
+    print_bulk_summaries(completed, errors)
+
+
+def render_errors(errors):
+    i = 1
+    error_str = []
+    for messages in errors:
+        error_str.append(f"Error {i} messages:")
+        error_io = io.StringIO()
+        fmtr = _formatter('pretty', error_io, PassthroughHandler())
+        for message in messages:
+            fmtr.record(message)
+        fmtr.write()
+        error_io.seek(0)
+        for l in error_io.getvalue().split('\n'):
+            error_str.append('   '+l)
+        i += 1
+    return '\n'.join(error_str)
+
+
+def render_summary(summary):
+    summary_io = io.StringIO()
+    fmtr = _formatter('pretty', summary_io, PassthroughHandler())
+    fmtr.record(summary)
+    fmtr.write()
+    summary_io.seek(0)
+    return summary_io.getvalue()
+
+def print_bulk_summaries(completed, errors):
+    summary = {
+        "Executed": completed,
+        "Succeeded": completed-len(errors),
+        "Errors": len(errors),
+    }
+    click.echo("--- Action Summary ---")
+    click.echo(render_summary(summary).strip())
+    click.echo("----------------------")
+    if errors:
+        click.echo("--- Error Summary ---")
+        click.echo(render_errors(errors).strip())
+        click.echo("--------------")
 
 
 if __name__ == '__main__':
-    app()
+    entry()
```

### Comparing `umapi_cli-2.0.0a2/umapi_cli/client.py` & `umapi_cli-2.1.0/umapi_cli/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 
 # Unless required by applicable law or agreed to in writing, software distributed under
 # the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR REPRESENTATIONS
 # OF ANY KIND, either express or implied. See the License for the specific language
 # governing permissions and limitations under the License.
 
 from umapi_client import OAuthS2S, Connection
+from .version import __version__ as app_version
+from . import log
 
 
 def create_conn(conf, test_mode):
     auth_args = {}
     if conf.get('UMAPI_AUTH_HOST') is not None:
         auth_args['auth_host'] = conf['UMAPI_AUTH_HOST']
     if conf.get('UMAPI_AUTH_ENDPOINT') is not None:
@@ -24,13 +26,17 @@
         **auth_args,
     )
 
     conn_args = {}
     if conf.get('UMAPI_URL') is not None:
         conn_args['endpoint'] = conf['UMAPI_URL']
 
+    user_agent = f"umapi-cli/{app_version}"
+    log.debug("User-Agent: %s", user_agent)
+
     return Connection(
         org_id=conf['UMAPI_ORG_ID'],
         auth=auth,
         test_mode=test_mode,
+        user_agent=user_agent,
         **conn_args,
     )
```

### Comparing `umapi_cli-2.0.0a2/umapi_cli/config.py` & `umapi_cli-2.1.0/umapi_cli/config.py`

 * *Files identical despite different names*

### Comparing `umapi_cli-2.0.0a2/umapi_cli/formatter.py` & `umapi_cli-2.1.0/umapi_cli/formatter.py`

 * *Files 4% similar despite different names*

```diff
@@ -88,14 +88,27 @@
 
 
 class OutputHandler:
     """Transform output and prepare for formatting"""
 
     formats = {
         'user_read': [
+            "id",
+            "type",
+            "email",
+            "firstname",
+            "lastname",
+            "country",
+            "username",
+            "domain",
+            "groups",
+            "tags",
+        ],
+        'user_read_all': [
+            "id",
             "type",
             "email",
             "firstname",
             "lastname",
             "country",
             "username",
             "domain",
@@ -111,17 +124,30 @@
         ],
     }
 
     def __init__(self, fmt):
         assert fmt in self.formats, "Invalid format"
         self.format = fmt
 
+    def get_fields(self):
+        return self.formats[self.format]
+
     def handle(self, record):
-        return {k: v for k, v in record.items() if k in self.formats[self.format]}
+        fields = self.get_fields()
+        return {k: v for k, v in record.items() if k in fields}
+
+
+class PassthroughHandler:
+    """Don't validate or transform. Used for error reporting"""
 
+    def __init__(self, _=None):
+        pass
+
+    def handle(self, record):
+        return record
 
 class Formatter:
     def __init__(self, fh, handler):
         self.records = []
         self.fh = fh
         self.handler = handler
 
@@ -161,30 +187,24 @@
         return self.records
 
 
 class CSVFormatter(Formatter):
     def write(self):
         if not self.records:
             return
-        writer = _csv.DictWriter(self.fh, self.fieldnames(self.records), lineterminator='\n')
+        writer = _csv.DictWriter(self.fh, self.handler.get_fields(), lineterminator='\n')
         writer.writeheader()
         writer.writerows(map(self.format_rec, self.records))
 
     def read(self):
         reader = _csv.DictReader(self.fh)
         for record in reader:
             self.record(self.handler.handle(record))
         return self.records
 
-    def fieldnames(self, records):
-        fieldnames = set()
-        for rec in (self.handler.handle(r) for r in records):
-            fieldnames.update(set(rec.keys()))
-        return sorted(list(fieldnames))
-
     def format_rec(self, record):
         formatted = {}
         formatted.update(record)
         for k, v in record.items():
             if isinstance(v, list):
                 formatted[k] = ','.join(v)
             else:
```

### Comparing `umapi_cli-2.0.0a2/umapi_cli/log.py` & `umapi_cli-2.1.0/umapi_cli/log.py`

 * *Files identical despite different names*

### Comparing `umapi_cli-2.0.0a2/umapi_cli/version.py` & `umapi_cli-2.1.0/umapi_cli/version.py`

 * *Files 25% similar despite different names*

```diff
@@ -4,8 +4,8 @@
 # of the License at http://www.apache.org/licenses/LICENSE-2.0
 
 # Unless required by applicable law or agreed to in writing, software distributed under
 # the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR REPRESENTATIONS
 # OF ANY KIND, either express or implied. See the License for the specific language
 # governing permissions and limitations under the License.
 
-__version__ = "2.0.0a2"
+__version__ = "2.1.0"
```

### Comparing `umapi_cli-2.0.0a2/PKG-INFO` & `umapi_cli-2.1.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,7 @@
-Metadata-Version: 2.1
-Name: umapi-cli
-Version: 2.0.0a2
-Summary: User Management API CLI Tool
-Home-page: https://github.com/adobe/umapi-cli/
-License: Apache 2.0
-Author: Andrew Dorton
-Author-email: adorton@adobe.com
-Requires-Python: >=3.9,<4.0
-Classifier: License :: Other/Proprietary License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: click (>=8.0,<9.0)
-Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
-Requires-Dist: schema (>=0.7.5,<0.8.0)
-Requires-Dist: umapi-client (>=3.0,<4.0)
-Project-URL: Repository, https://github.com/adobe/umapi-cli/
-Description-Content-Type: text/markdown
-
 # User Management API CLI Tool
 
 A simple command-line interface (CLI) client to the
 [Adobe User Management API](https://adobe-apiplatform.github.io/umapi-documentation/en/).
 
 ## Table of Contents
 
@@ -102,14 +81,17 @@
 
 ## Option 2 - Executable
 
 A self-contained executable is also available for Windows and macOS. The
 executable embeds a Python environment, so Python does not need to be installed
 on the system. Note that this build is slower to start when executing the tool.
 
+Executables can be found on the [latest
+releases](https://github.com/adobe/umapi-cli/releases/latest) page.
+
 # Usage Overview
 
 The tool operates on a series of commands. Each command performs a certain
 operation - read single user, read all users, create user/group, etc.
 
 ```
 $ umapi --help
@@ -257,14 +239,19 @@
 
 Options:
   -h, --help                    Show this message and exit.
   -f, --format csv|json|pretty  Output format  [default: pretty]
   -e, --email TEXT              User email address  [required]
 ```
 
+**Note:** The CSV format for `user-read` is the same as `user-read-all` ([see
+below](#user-read-all)) with the exception of the `tags` column. This column can
+currently only be read on a user-by-user basis and thus is not included in
+`user-read-all` results.
+
 ## `user-read-all`
 
 Get details for all users in a given console. 
 
 Formats: [JSONL](http://jsonlines.org), CSV, or human-readable (default).
 
 This command writes to stdout by default, but can optionally write output to a
@@ -764,14 +751,18 @@
    
 To run the tool from source:
 
 1. Ensure dependencies are up to date with `poetry install`.
 2. Prefix invocations of the `umapi` command with `poetry run` (e.g. `poetry run
    umapi --help`). This runs the `umapi` entrypoint from the project's virtual
    environment.
+   
+> **Note:** if you are doing development work on the tool and wish to see full
+> error information when an error occurs, set the `UMAPI_DEBUG` environment
+> variable to `1`. This will dump more information on the error including a
+> stack trace.
 
 # Getting Help
 
 Should you run into any issues using this tool, or have any questions or
 comments, please create an [issue](https://github.com/adobe/umapi-cli/issues) to
 contact the development team.
-
```

