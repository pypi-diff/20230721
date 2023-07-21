# Comparing `tmp/migrado-0.6.6.tar.gz` & `tmp/migrado-0.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "migrado-0.6.6.tar", max compression
+gzip compressed data, was "migrado-0.6.7.tar", max compression
```

## Comparing `migrado-0.6.6.tar` & `migrado-0.6.7.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0     1055 2022-08-19 14:07:57.639602 migrado-0.6.6/LICENSE.txt
--rw-r--r--   0        0        0     9044 2022-08-19 14:07:57.639602 migrado-0.6.6/README.md
--rw-r--r--   0        0        0       29 2022-08-19 14:07:57.672935 migrado-0.6.6/migrado/__init__.py
--rw-r--r--   0        0        0      435 2022-08-19 14:07:57.672935 migrado-0.6.6/migrado/constants.py
--rw-r--r--   0        0        0     6474 2022-08-19 14:07:57.672935 migrado-0.6.6/migrado/db_client.py
--rw-r--r--   0        0        0    16624 2022-08-19 14:07:57.676268 migrado-0.6.6/migrado/migrado.py
--rw-r--r--   0        0        0     2387 2022-08-19 14:07:57.676268 migrado-0.6.6/migrado/utils.py
--rw-r--r--   0        0        0      597 2022-12-09 10:43:36.257989 migrado-0.6.6/pyproject.toml
--rw-r--r--   0        0        0    10160 1970-01-01 00:00:00.000000 migrado-0.6.6/setup.py
--rw-r--r--   0        0        0     9814 1970-01-01 00:00:00.000000 migrado-0.6.6/PKG-INFO
+-rw-r--r--   0        0        0     1055 2022-08-19 14:07:57.639602 migrado-0.6.7/LICENSE.txt
+-rw-r--r--   0        0        0     9044 2022-08-19 14:07:57.639602 migrado-0.6.7/README.md
+-rw-r--r--   0        0        0       29 2022-08-19 14:07:57.672935 migrado-0.6.7/migrado/__init__.py
+-rw-r--r--   0        0        0      435 2022-08-19 14:07:57.672935 migrado-0.6.7/migrado/constants.py
+-rw-r--r--   0        0        0     6474 2022-08-19 14:07:57.672935 migrado-0.6.7/migrado/db_client.py
+-rw-r--r--   0        0        0    16624 2022-08-19 14:07:57.676268 migrado-0.6.7/migrado/migrado.py
+-rw-r--r--   0        0        0     2387 2022-08-19 14:07:57.676268 migrado-0.6.7/migrado/utils.py
+-rw-r--r--   0        0        0      597 2023-07-21 00:07:23.681162 migrado-0.6.7/pyproject.toml
+-rw-r--r--   0        0        0     9865 1970-01-01 00:00:00.000000 migrado-0.6.7/PKG-INFO
```

### Comparing `migrado-0.6.6/LICENSE.txt` & `migrado-0.6.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `migrado-0.6.6/README.md` & `migrado-0.6.7/README.md`

 * *Files identical despite different names*

### Comparing `migrado-0.6.6/migrado/db_client.py` & `migrado-0.6.7/migrado/db_client.py`

 * *Files identical despite different names*

### Comparing `migrado-0.6.6/migrado/migrado.py` & `migrado-0.6.7/migrado/migrado.py`

 * *Files identical despite different names*

### Comparing `migrado-0.6.6/migrado/utils.py` & `migrado-0.6.7/migrado/utils.py`

 * *Files identical despite different names*

### Comparing `migrado-0.6.6/pyproject.toml` & `migrado-0.6.7/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "migrado"
-version = "0.6.6"
+version = "0.6.7"
 description = "ArangoDB migrations and batch processing manager"
 authors = ["Eirik Krogstad <eirikkr@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/protojour/migrado"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 click = "^8.1.3"
 python-arango = "^7.1.0"
-pyyaml = "^5.4.1"
+pyyaml = "^6.0.1"
 rich = "^10.12.0"
 
 [tool.poetry.dev-dependencies]
 pylint = "^2.14.0"
 pytest = "^7.1.2"
 pytest-cov = "^3.0.0"
```

### Comparing `migrado-0.6.6/setup.py` & `migrado-0.6.7/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,37 +1,281 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: migrado
+Version: 0.6.7
+Summary: ArangoDB migrations and batch processing manager
+Home-page: https://github.com/protojour/migrado
+License: MIT
+Author: Eirik Krogstad
+Author-email: eirikkr@gmail.com
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: click (>=8.1.3,<9.0.0)
+Requires-Dist: python-arango (>=7.1.0,<8.0.0)
+Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
+Requires-Dist: rich (>=10.12.0,<11.0.0)
+Project-URL: Repository, https://github.com/protojour/migrado
+Description-Content-Type: text/markdown
 
-packages = \
-['migrado']
+Migrado
+=======
 
-package_data = \
-{'': ['*']}
+[![PyPI package](https://badge.fury.io/py/migrado.svg)](https://pypi.org/project/migrado/)
+[![Tests](https://github.com/protojour/migrado/actions/workflows/main.yml/badge.svg?branch=master)](https://github.com/protojour/migrado/actions/workflows/main.yml)
 
-install_requires = \
-['click>=8.1.3,<9.0.0',
- 'python-arango>=7.1.0,<8.0.0',
- 'pyyaml>=5.4.1,<6.0.0',
- 'rich>=10.12.0,<11.0.0']
-
-entry_points = \
-{'console_scripts': ['migrado = migrado:migrado']}
-
-setup_kwargs = {
-    'name': 'migrado',
-    'version': '0.6.6',
-    'description': 'ArangoDB migrations and batch processing manager',
-    'long_description': 'Migrado\n=======\n\n[![PyPI package](https://badge.fury.io/py/migrado.svg)](https://pypi.org/project/migrado/)\n[![Tests](https://github.com/protojour/migrado/actions/workflows/main.yml/badge.svg?branch=master)](https://github.com/protojour/migrado/actions/workflows/main.yml)\n\n🥑 ArangoDB migrations and batch processing manager.\n\nMigrado is a command-line client that can help build and run schema or data migrations against your ArangoDB instance. \n\nMigrado utilizes ArangoDB Transactions when running data migrations to ensure failed scripts are rolled back automatically. `arangosh` from the [ArangoDB Client Tools](https://www.arangodb.com/download-major/) is required to run schema migrations, however no transaction safety is available at this point.\n\n**Migrado should be considered beta software,** but it is well tested, and used in production settings. Make sure you understand how it operates.\n\nIf you have trouble, open an issue. Contributions are welcome.\n\nInstallation\n------------\n\nMigrado requires Python 3.6 or higher, and the ArangoDB `arangosh` client.\n\n```bash\n$ pip install --user migrado\n```\n\nIt is also available as a Docker image, see [Docker usage](#docker-usage).\n\nUsage\n-----\n\nMigrado can create a migrations directory and generate an initial set of collections from a given schema file:\n\n```bash\n$ migrado init --schema schema.yml\n```\n\nMigrado can also construct an initial migration from the current database structure (and automatically store it as the current state/schema):\n\n```bash\n$ migrado init --infer\n```\n\nSee [YAML schemas](#yaml-schemas) for details. If neither option is specified, Migrado will create an empty initial migration.\n\nTo autogenerate a schema migration script based on an updated schema:\n\n```bash\n$ migrado make --schema updated_schema.yml\n```\n\nTo make a new template data migration script:\n\n```bash\n$ migrado make --name rewrite_field_names\n```\n\nThis will create a new file, `migrations/0002_rewrite_field_names.js` (`--name` is optional), which you can edit as you see fit. See [Migration scripts](#migration-scripts) for details.\n\nWhen you are ready, run all migrations (not previously ran) against the database: \n\n```bash\n$ migrado run\n```\n\nMigrado stores migration state in a configurable collection, see `--help` or [Environment vars](#environment-vars) for details.\n\nIf you wrote a `reverse()` migration, you can revert to an earlier point by specifying a target migration id. To revert to the initial migration:\n\n```bash\n$ migrado run --target 0001\n```\n\nYou can inspect the current migration state with:\n\n```bash\n$ migrado inspect\n```\n\nYou can inspect the current schema (explicit or inferred) with:\n\n```bash\n$ migrado export\n```\n\nUse the `--help` option for help on any command when using the client.\n\nDocker usage\n------------\n\nIf you\'re using Migrado in a Docker context, you might as well use the [Docker image](https://hub.docker.com/r/protojour/migrado). `migrado` is set as entrypoint, so the image can be used like the Python client:\n\n```bash\n$ docker run protojour/migrado --help\n```\n\nYou\'d want to volume in your migrations folder:\n\n```bash\n$ docker run -v /path/to/migrations:/app/migrations protojour/migrado\n```\n\nOr, an example using docker-compose:\n\n```yaml\nmigrado:\n  image: protojour/migrado:latest\n  environment:\n    MIGRADO_DB: # ...\n    MIGRADO_HOST: # ...\n  volumes:\n    - ./migrations:/app/migrations\n```\n\nThen either add a `command:` (with a migrado sub-command, e.g. `command: run ...`), or use this as a starting point for a scripted migration strategy.\n\nYou may also use the base [Dockerfile](https://github.com/protojour/migrado/blob/master/Dockerfile) as a starting point.\n\nEnvironment vars\n----------------\n\nThe following environment variables are employed by Migrado:\n\n- `MIGRADO_PATH`: Specifies the path to the migrations directory, replaces `-p`, `--path` (default: `migrations`).\n- `MIGRADO_DB`: Specifies the ArangoDB database name for generated migrations to interact with, replaces `-d`, `--db` (no default, but required for the `run` command).\n- `MIGRADO_COLL`: Specifies ArangoDb collection name to store migration state in, replaces `-c`, `--state-coll` (default: `migrado`).\n- `MIGRADO_TLS`: Use TLS for connection when running migrations, replaces `-T`, `--tls` (default: `False`).\n- `MIGRADO_HOST`: Specifies the database host for running migrations, replaces `-H`, `--host` (default: `localhost`).\n- `MIGRADO_PORT`: Specifies the database port for running migrations, replaces `-P`, `--port` (default: `8529`).\n- `MIGRADO_USER`: Specifies the database username for running migrations, replaces `-U`, `--username` (no default).\n- `MIGRADO_PASS`: Specifies the database password for running migrations, replaces `-W`, `--password` (no default).\n\nYAML schemas\n------------\n\nArangoDB may be schemaless, but in a larger project it still makes sense to keep a schema spec up to date, both for an overview of collections and their data structures, and as a basis for [native collection-level validation](https://www.arangodb.com/docs/3.9/data-modeling-documents-schema-validation.html) (see the `-v/--validation` option).\n\nMigrado uses a schema model based on JSON Schema, in YAML, and can use this to generate an initial migration for the collections available in your database.\n\nExample schema:\n\n```yaml\nall: &all\n  _id:\n    type: string\n    readOnly: true\n  _key:\n    type: string\n    readOnly: true\n  _rev:\n    type: string\n    readOnly: true\n\nedges: &edges\n  _from:\n    type: string\n  _to:\n    type: string\n\ncollections:\n\n  books:\n    type: object\n    properties:\n      <<: *all\n      title:\n        type: string\n      isbn:\n        type: string\n    required:\n      - title\n      - isbn\n\n  authors:\n    # Note: you do not actually need to specify an object schema,\n    # but the schema can be used with ArangoDB\'s native validation \n    # using the -v/--validation option\n\nedge_collections:\n\n  # authors --> books \n  author_of:\n    type: object\n    properties:\n      <<: *all\n      <<: *edges\n    required:\n      - _from\n      - _to\n```\n\nMigration scripts\n-----------------\n\nMigration scripts are structured so they may be parsed and run easily by both Migrado and ArangoDB. In addition, they are structured so they may be run manually against ArangoDB using `arangosh`.\n\nThere are two types of script, **data** and **schema** migration scripts.\n\n### Data migrations\n\nYou need to declare all collections subject to write operations using the syntax `// write collection_name`, because ArangoDB needs this information for locking during transactions. We\'ve made the declaration explicit to reduce errors. _Attempting to write to collections not declared in this way will cause the migration to fail._\n\nIn general, a reverse migration should do the logical opposite of a forward migration. `forward()` and `reverse()` functions can contain anything that the ArangoDB V8 engine understands, but must be fully self-contained. _Anything outside these functions is ignored and unavailable when running migrations._\n\nHere\'s an example migration script for adding `new_field` in collection `things`:\n\n```javascript\n// write things\n\nfunction forward() {\n    var db = require("@arangodb").db\n    db._query(`\n        FOR thing IN things\n            UPDATE thing WITH { new_field: "some value" } IN things\n    `)\n}\n\nfunction reverse() {\n    var db = require("@arangodb").db\n    db._query(`\n        FOR thing IN things\n            REPLACE thing WITH UNSET(thing, "new_field") IN things\n    `)\n}\n```\n\nPlease make sure you read [limitations when running transactions](https://www.arangodb.com/docs/stable/transactions-limitations.html) in the ArangoDB documentation. In particular, _creation and deletion of databases, collections, and indexes_ is not allowed in transactions.\n\n### Schema migrations\n\nSchema migrations are stuctured in the same way as data migrations, but are run against `arangosh` as opposed to the HTTP API. There is no transaction safety when running schema migrations.\n\nSchema migrations are structured the same way as data migrations, but `// write` declarations are not required. All operations are allowed.\n\nHere\'s an example migration script generated from the YAML schema above (with no validation):\n\n```javascript\nfunction forward() {\n    var db = require("@arangodb").db\n    var schema = // schema to be written to disk\n    db._create("books", {}, "document")\n    db._create("authors", {}, "document")\n    db._create("author_of", {}, "edge")\n}\n\nfunction reverse() {\n    var db = require("@arangodb").db\n    db._drop("books")\n    db._drop("authors")\n    db._drop("author_of")\n}\n```\n\nPlease be careful when running schema migrations in reverse. As you can see, the `reverse()` function above would drop your collections (and lose your data) if you were to reverse beyond this point. Currently, you will not be able to do so for an initial migration.\n\nLicense\n-------\n\nMigrado is copyright © 2019 Protojour AS, and is licensed under MIT. See [LICENSE.txt](https://github.com/protojour/migrado/blob/master/LICENSE.txt) for details.\n',
-    'author': 'Eirik Krogstad',
-    'author_email': 'eirikkr@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/protojour/migrado',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.8,<4.0',
+🥑 ArangoDB migrations and batch processing manager.
+
+Migrado is a command-line client that can help build and run schema or data migrations against your ArangoDB instance. 
+
+Migrado utilizes ArangoDB Transactions when running data migrations to ensure failed scripts are rolled back automatically. `arangosh` from the [ArangoDB Client Tools](https://www.arangodb.com/download-major/) is required to run schema migrations, however no transaction safety is available at this point.
+
+**Migrado should be considered beta software,** but it is well tested, and used in production settings. Make sure you understand how it operates.
+
+If you have trouble, open an issue. Contributions are welcome.
+
+Installation
+------------
+
+Migrado requires Python 3.6 or higher, and the ArangoDB `arangosh` client.
+
+```bash
+$ pip install --user migrado
+```
+
+It is also available as a Docker image, see [Docker usage](#docker-usage).
+
+Usage
+-----
+
+Migrado can create a migrations directory and generate an initial set of collections from a given schema file:
+
+```bash
+$ migrado init --schema schema.yml
+```
+
+Migrado can also construct an initial migration from the current database structure (and automatically store it as the current state/schema):
+
+```bash
+$ migrado init --infer
+```
+
+See [YAML schemas](#yaml-schemas) for details. If neither option is specified, Migrado will create an empty initial migration.
+
+To autogenerate a schema migration script based on an updated schema:
+
+```bash
+$ migrado make --schema updated_schema.yml
+```
+
+To make a new template data migration script:
+
+```bash
+$ migrado make --name rewrite_field_names
+```
+
+This will create a new file, `migrations/0002_rewrite_field_names.js` (`--name` is optional), which you can edit as you see fit. See [Migration scripts](#migration-scripts) for details.
+
+When you are ready, run all migrations (not previously ran) against the database: 
+
+```bash
+$ migrado run
+```
+
+Migrado stores migration state in a configurable collection, see `--help` or [Environment vars](#environment-vars) for details.
+
+If you wrote a `reverse()` migration, you can revert to an earlier point by specifying a target migration id. To revert to the initial migration:
+
+```bash
+$ migrado run --target 0001
+```
+
+You can inspect the current migration state with:
+
+```bash
+$ migrado inspect
+```
+
+You can inspect the current schema (explicit or inferred) with:
+
+```bash
+$ migrado export
+```
+
+Use the `--help` option for help on any command when using the client.
+
+Docker usage
+------------
+
+If you're using Migrado in a Docker context, you might as well use the [Docker image](https://hub.docker.com/r/protojour/migrado). `migrado` is set as entrypoint, so the image can be used like the Python client:
+
+```bash
+$ docker run protojour/migrado --help
+```
+
+You'd want to volume in your migrations folder:
+
+```bash
+$ docker run -v /path/to/migrations:/app/migrations protojour/migrado
+```
+
+Or, an example using docker-compose:
+
+```yaml
+migrado:
+  image: protojour/migrado:latest
+  environment:
+    MIGRADO_DB: # ...
+    MIGRADO_HOST: # ...
+  volumes:
+    - ./migrations:/app/migrations
+```
+
+Then either add a `command:` (with a migrado sub-command, e.g. `command: run ...`), or use this as a starting point for a scripted migration strategy.
+
+You may also use the base [Dockerfile](https://github.com/protojour/migrado/blob/master/Dockerfile) as a starting point.
+
+Environment vars
+----------------
+
+The following environment variables are employed by Migrado:
+
+- `MIGRADO_PATH`: Specifies the path to the migrations directory, replaces `-p`, `--path` (default: `migrations`).
+- `MIGRADO_DB`: Specifies the ArangoDB database name for generated migrations to interact with, replaces `-d`, `--db` (no default, but required for the `run` command).
+- `MIGRADO_COLL`: Specifies ArangoDb collection name to store migration state in, replaces `-c`, `--state-coll` (default: `migrado`).
+- `MIGRADO_TLS`: Use TLS for connection when running migrations, replaces `-T`, `--tls` (default: `False`).
+- `MIGRADO_HOST`: Specifies the database host for running migrations, replaces `-H`, `--host` (default: `localhost`).
+- `MIGRADO_PORT`: Specifies the database port for running migrations, replaces `-P`, `--port` (default: `8529`).
+- `MIGRADO_USER`: Specifies the database username for running migrations, replaces `-U`, `--username` (no default).
+- `MIGRADO_PASS`: Specifies the database password for running migrations, replaces `-W`, `--password` (no default).
+
+YAML schemas
+------------
+
+ArangoDB may be schemaless, but in a larger project it still makes sense to keep a schema spec up to date, both for an overview of collections and their data structures, and as a basis for [native collection-level validation](https://www.arangodb.com/docs/3.9/data-modeling-documents-schema-validation.html) (see the `-v/--validation` option).
+
+Migrado uses a schema model based on JSON Schema, in YAML, and can use this to generate an initial migration for the collections available in your database.
+
+Example schema:
+
+```yaml
+all: &all
+  _id:
+    type: string
+    readOnly: true
+  _key:
+    type: string
+    readOnly: true
+  _rev:
+    type: string
+    readOnly: true
+
+edges: &edges
+  _from:
+    type: string
+  _to:
+    type: string
+
+collections:
+
+  books:
+    type: object
+    properties:
+      <<: *all
+      title:
+        type: string
+      isbn:
+        type: string
+    required:
+      - title
+      - isbn
+
+  authors:
+    # Note: you do not actually need to specify an object schema,
+    # but the schema can be used with ArangoDB's native validation 
+    # using the -v/--validation option
+
+edge_collections:
+
+  # authors --> books 
+  author_of:
+    type: object
+    properties:
+      <<: *all
+      <<: *edges
+    required:
+      - _from
+      - _to
+```
+
+Migration scripts
+-----------------
+
+Migration scripts are structured so they may be parsed and run easily by both Migrado and ArangoDB. In addition, they are structured so they may be run manually against ArangoDB using `arangosh`.
+
+There are two types of script, **data** and **schema** migration scripts.
+
+### Data migrations
+
+You need to declare all collections subject to write operations using the syntax `// write collection_name`, because ArangoDB needs this information for locking during transactions. We've made the declaration explicit to reduce errors. _Attempting to write to collections not declared in this way will cause the migration to fail._
+
+In general, a reverse migration should do the logical opposite of a forward migration. `forward()` and `reverse()` functions can contain anything that the ArangoDB V8 engine understands, but must be fully self-contained. _Anything outside these functions is ignored and unavailable when running migrations._
+
+Here's an example migration script for adding `new_field` in collection `things`:
+
+```javascript
+// write things
+
+function forward() {
+    var db = require("@arangodb").db
+    db._query(`
+        FOR thing IN things
+            UPDATE thing WITH { new_field: "some value" } IN things
+    `)
+}
+
+function reverse() {
+    var db = require("@arangodb").db
+    db._query(`
+        FOR thing IN things
+            REPLACE thing WITH UNSET(thing, "new_field") IN things
+    `)
+}
+```
+
+Please make sure you read [limitations when running transactions](https://www.arangodb.com/docs/stable/transactions-limitations.html) in the ArangoDB documentation. In particular, _creation and deletion of databases, collections, and indexes_ is not allowed in transactions.
+
+### Schema migrations
+
+Schema migrations are stuctured in the same way as data migrations, but are run against `arangosh` as opposed to the HTTP API. There is no transaction safety when running schema migrations.
+
+Schema migrations are structured the same way as data migrations, but `// write` declarations are not required. All operations are allowed.
+
+Here's an example migration script generated from the YAML schema above (with no validation):
+
+```javascript
+function forward() {
+    var db = require("@arangodb").db
+    var schema = // schema to be written to disk
+    db._create("books", {}, "document")
+    db._create("authors", {}, "document")
+    db._create("author_of", {}, "edge")
 }
 
+function reverse() {
+    var db = require("@arangodb").db
+    db._drop("books")
+    db._drop("authors")
+    db._drop("author_of")
+}
+```
+
+Please be careful when running schema migrations in reverse. As you can see, the `reverse()` function above would drop your collections (and lose your data) if you were to reverse beyond this point. Currently, you will not be able to do so for an initial migration.
+
+License
+-------
+
+Migrado is copyright © 2019 Protojour AS, and is licensed under MIT. See [LICENSE.txt](https://github.com/protojour/migrado/blob/master/LICENSE.txt) for details.
 
-setup(**setup_kwargs)
```

