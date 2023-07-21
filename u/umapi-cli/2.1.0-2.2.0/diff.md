# Comparing `tmp/umapi_cli-2.1.0.tar.gz` & `tmp/umapi_cli-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "umapi_cli-2.1.0.tar", max compression
+gzip compressed data, was "umapi_cli-2.2.0.tar", max compression
```

## Comparing `umapi_cli-2.1.0.tar` & `umapi_cli-2.2.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    11335 2023-06-21 15:28:39.518313 umapi_cli-2.1.0/LICENSE
--rw-r--r--   0        0        0    24835 2023-07-20 21:06:38.504997 umapi_cli-2.1.0/README.md
--rw-r--r--   0        0        0      705 2023-07-20 23:33:25.470732 umapi_cli-2.1.0/pyproject.toml
--rw-r--r--   0        0        0      603 2023-06-21 16:29:58.311507 umapi_cli-2.1.0/umapi_cli/__init__.py
--rw-r--r--   0        0        0     4036 2023-07-11 14:46:22.788370 umapi_cli-2.1.0/umapi_cli/action_queue.py
--rw-r--r--   0        0        0    19409 2023-07-20 22:42:50.788101 umapi_cli-2.1.0/umapi_cli/cli.py
--rw-r--r--   0        0        0     1504 2023-07-20 17:33:12.989018 umapi_cli-2.1.0/umapi_cli/client.py
--rw-r--r--   0        0        0     1253 2023-06-21 16:29:35.143777 umapi_cli-2.1.0/umapi_cli/config.py
--rw-r--r--   0        0        0     6167 2023-07-20 21:06:38.505918 umapi_cli-2.1.0/umapi_cli/formatter.py
--rw-r--r--   0        0        0     1298 2023-06-21 16:29:14.623535 umapi_cli-2.1.0/umapi_cli/log.py
--rw-r--r--   0        0        0      626 2023-07-20 23:33:17.625349 umapi_cli-2.1.0/umapi_cli/version.py
--rw-r--r--   0        0        0    25587 1970-01-01 00:00:00.000000 umapi_cli-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11335 2023-06-21 15:28:39.518313 umapi_cli-2.2.0/LICENSE
+-rw-r--r--   0        0        0    24861 2023-07-21 18:04:02.099453 umapi_cli-2.2.0/README.md
+-rw-r--r--   0        0        0      705 2023-07-21 19:37:26.148506 umapi_cli-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0      603 2023-06-21 16:29:58.311507 umapi_cli-2.2.0/umapi_cli/__init__.py
+-rw-r--r--   0        0        0     4036 2023-07-11 14:46:22.788370 umapi_cli-2.2.0/umapi_cli/action_queue.py
+-rw-r--r--   0        0        0    19529 2023-07-21 18:08:00.393196 umapi_cli-2.2.0/umapi_cli/cli.py
+-rw-r--r--   0        0        0     1504 2023-07-20 17:33:12.989018 umapi_cli-2.2.0/umapi_cli/client.py
+-rw-r--r--   0        0        0     1253 2023-06-21 16:29:35.143777 umapi_cli-2.2.0/umapi_cli/config.py
+-rw-r--r--   0        0        0     6187 2023-07-21 17:16:55.766777 umapi_cli-2.2.0/umapi_cli/formatter.py
+-rw-r--r--   0        0        0     1298 2023-06-21 16:29:14.623535 umapi_cli-2.2.0/umapi_cli/log.py
+-rw-r--r--   0        0        0      626 2023-07-21 19:37:19.403869 umapi_cli-2.2.0/umapi_cli/version.py
+-rw-r--r--   0        0        0    25613 1970-01-01 00:00:00.000000 umapi_cli-2.2.0/PKG-INFO
```

### Comparing `umapi_cli-2.1.0/LICENSE` & `umapi_cli-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `umapi_cli-2.1.0/README.md` & `umapi_cli-2.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -235,15 +235,15 @@
 $ umapi user-read --help
 Usage: umapi user-read [OPTIONS]
 
   Get details for a single user
 
 Options:
   -h, --help                    Show this message and exit.
-  -f, --format csv|json|pretty  Output format  [default: pretty]
+  -f, --format csv|json|pretty  Output format
   -e, --email TEXT              User email address  [required]
 ```
 
 **Note:** The CSV format for `user-read` is the same as `user-read-all` ([see
 below](#user-read-all)) with the exception of the `tags` column. This column can
 currently only be read on a user-by-user basis and thus is not included in
 `user-read-all` results.
@@ -268,16 +268,17 @@
 $ umapi user-read-all --help
 Usage: umapi user-read-all [OPTIONS]
 
   Get details for all users belonging to a console
 
 Options:
   -h, --help                    Show this message and exit.
-  -f, --format csv|json|pretty  Output format  [default: pretty]
+  -f, --format csv|json|pretty  Output format
   -o, --out-file FILENAME       Write output to this filename
+  -g, --in-group GROUP          Limit query to members of GROUP
 ```
 
 Names of columns/fields when writing to CSV or JSONL are the same.
 
 | Column Name | Purpose                                                               |
 |-------------|-----------------------------------------------------------------------|
 | `type`      | User's identity type (`enterpriseID`, `federatedID` or `adobeID`)     |
```

### Comparing `umapi_cli-2.1.0/pyproject.toml` & `umapi_cli-2.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "umapi-cli"
-version = "2.1.0"
+version = "2.2.0"
 description = "User Management API CLI Tool"
 authors = ["Andrew Dorton <adorton@adobe.com>"]
 license = "Apache 2.0"
 readme = "README.md"
 repository = "https://github.com/adobe/umapi-cli/"
 
 [tool.poetry.dependencies]
```

### Comparing `umapi_cli-2.1.0/umapi_cli/__init__.py` & `umapi_cli-2.2.0/umapi_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `umapi_cli-2.1.0/umapi_cli/action_queue.py` & `umapi_cli-2.2.0/umapi_cli/action_queue.py`

 * *Files identical despite different names*

### Comparing `umapi_cli-2.1.0/umapi_cli/cli.py` & `umapi_cli-2.2.0/umapi_cli/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,26 +100,27 @@
     fmtr.write()
 
 
 @app.command()
 @click.help_option('-h', '--help')
 @click.option('-f', '--format', 'output_format', help='Output format', metavar='csv|json|pretty', show_default=True)
 @click.option('-o', '--out-file', help='Write output to this filename', metavar='FILENAME')
+@click.option('-g', '--in-group', help="Limit query to members of GROUP", metavar='GROUP')
 @click.pass_context
-def user_read_all(ctx, output_format, out_file):
+def user_read_all(ctx, output_format, out_file, in_group):
     """Get details for all users belonging to a console"""
 
     if out_file is not None:
         output_format = infer_format(out_file)
     if output_format is None:
         output_format = 'pretty'
 
     fmtr = _formatter(output_format, _output_fh(out_file), OutputHandler('user_read_all'))
     umapi_conn = ctx.obj['conn']
-    query = UsersQuery(umapi_conn)
+    query = UsersQuery(umapi_conn, in_group=in_group)
     report_total = True
     for user in query:
         total, *_ = query.stats()
         if total is not None and report_total:
             log.info(f"Total records: {total}")
             report_total = False
         fmtr.record(user)
```

### Comparing `umapi_cli-2.1.0/umapi_cli/client.py` & `umapi_cli-2.2.0/umapi_cli/client.py`

 * *Files identical despite different names*

### Comparing `umapi_cli-2.1.0/umapi_cli/config.py` & `umapi_cli-2.2.0/umapi_cli/config.py`

 * *Files identical despite different names*

### Comparing `umapi_cli-2.1.0/umapi_cli/formatter.py` & `umapi_cli-2.2.0/umapi_cli/formatter.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,14 +109,15 @@
             "email",
             "firstname",
             "lastname",
             "country",
             "username",
             "domain",
             "groups",
+            "tags",
         ],
         'group_read': [
             'groupName',
             'type',
             'adminGroupName',
             'memberCount',
             'productName',
```

### Comparing `umapi_cli-2.1.0/umapi_cli/log.py` & `umapi_cli-2.2.0/umapi_cli/log.py`

 * *Files identical despite different names*

### Comparing `umapi_cli-2.1.0/umapi_cli/version.py` & `umapi_cli-2.2.0/umapi_cli/version.py`

 * *Files 25% similar despite different names*

```diff
@@ -4,8 +4,8 @@
 # of the License at http://www.apache.org/licenses/LICENSE-2.0
 
 # Unless required by applicable law or agreed to in writing, software distributed under
 # the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR REPRESENTATIONS
 # OF ANY KIND, either express or implied. See the License for the specific language
 # governing permissions and limitations under the License.
 
-__version__ = "2.1.0"
+__version__ = "2.2.0"
```

### Comparing `umapi_cli-2.1.0/PKG-INFO` & `umapi_cli-2.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: umapi-cli
-Version: 2.1.0
+Version: 2.2.0
 Summary: User Management API CLI Tool
 Home-page: https://github.com/adobe/umapi-cli/
 License: Apache 2.0
 Author: Andrew Dorton
 Author-email: adorton@adobe.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
@@ -256,15 +256,15 @@
 $ umapi user-read --help
 Usage: umapi user-read [OPTIONS]
 
   Get details for a single user
 
 Options:
   -h, --help                    Show this message and exit.
-  -f, --format csv|json|pretty  Output format  [default: pretty]
+  -f, --format csv|json|pretty  Output format
   -e, --email TEXT              User email address  [required]
 ```
 
 **Note:** The CSV format for `user-read` is the same as `user-read-all` ([see
 below](#user-read-all)) with the exception of the `tags` column. This column can
 currently only be read on a user-by-user basis and thus is not included in
 `user-read-all` results.
@@ -289,16 +289,17 @@
 $ umapi user-read-all --help
 Usage: umapi user-read-all [OPTIONS]
 
   Get details for all users belonging to a console
 
 Options:
   -h, --help                    Show this message and exit.
-  -f, --format csv|json|pretty  Output format  [default: pretty]
+  -f, --format csv|json|pretty  Output format
   -o, --out-file FILENAME       Write output to this filename
+  -g, --in-group GROUP          Limit query to members of GROUP
 ```
 
 Names of columns/fields when writing to CSV or JSONL are the same.
 
 | Column Name | Purpose                                                               |
 |-------------|-----------------------------------------------------------------------|
 | `type`      | User's identity type (`enterpriseID`, `federatedID` or `adobeID`)     |
```

