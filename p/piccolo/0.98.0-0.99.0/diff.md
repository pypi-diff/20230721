# Comparing `tmp/piccolo-0.98.0.tar.gz` & `tmp/piccolo-0.99.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/piccolo-0.98.0.tar", last modified: Fri Dec  2 12:16:11 2022, max compression
+gzip compressed data, was "dist/piccolo-0.99.0.tar", last modified: Fri Dec  2 13:06:22 2022, max compression
```

## Comparing `piccolo-0.98.0.tar` & `piccolo-0.99.0.tar`

### file list

```diff
@@ -1,439 +1,439 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 12:16:11.000000 piccolo-0.98.0/
--rw-r--r--   0 runner    (1001) docker     (122)     5591 2022-12-02 12:16:11.000000 piccolo-0.98.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3460 2022-12-02 12:15:55.000000 piccolo-0.98.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 12:16:11.000000 piccolo-0.98.0/piccolo/
--rw-r--r--   0 runner    (1001) docker     (122)       23 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 12:16:11.000000 piccolo-0.98.0/piccolo/apps/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 12:16:11.000000 piccolo-0.98.0/piccolo/apps/app/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/apps/app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 12:16:11.000000 piccolo-0.98.0/piccolo/apps/app/commands/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/apps/app/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2187 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/apps/app/commands/new.py
--rw-r--r--   0 runner    (1001) docker     (122)      252 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/apps/app/commands/show_all.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 12:16:11.000000 piccolo-0.98.0/piccolo/apps/app/commands/templates/
--rw-r--r--   0 runner    (1001) docker     (122)      428 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/apps/app/commands/templates/piccolo_app.py.jinja
--rw-r--r--   0 runner    (1001) docker     (122)       32 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/apps/app/commands/templates/tables.py.jinja
--rw-r--r--   0 runner    (1001) docker     (122)      340 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/apps/app/piccolo_app.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 12:16:11.000000 piccolo-0.98.0/piccolo/apps/asgi/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/apps/asgi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 12:16:11.000000 piccolo-0.98.0/piccolo/apps/asgi/commands/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/apps/asgi/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4160 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/apps/asgi/commands/new.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 12:16:10.000000 piccolo-0.98.0/piccolo/apps/asgi/commands/templates/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 12:16:11.000000 piccolo-0.98.0/piccolo/apps/asgi/commands/templates/app/
--rw-r--r--   0 runner    (1001) docker     (122)      214 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/apps/asgi/commands/templates/app/README.md.jinja
--rw-r--r--   0 runner    (1001) docker     (122)     3117 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/apps/asgi/commands/templates/app/_blacksheep_app.py.jinja
--rw-r--r--   0 runner    (1001) docker     (122)     2436 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/apps/asgi/commands/templates/app/_fastapi_app.py.jinja
--rw-r--r--   0 runner    (1001) docker     (122)     1271 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/apps/asgi/commands/templates/app/_starlette_app.py.jinja
--rw-r--r--   0 runner    (1001) docker     (122)     2889 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/apps/asgi/commands/templates/app/_starlite_app.py.jinja
--rw-r--r--   0 runner    (1001) docker     (122)     2855 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/apps/asgi/commands/templates/app/_xpresso_app.py.jinja
--rw-r--r--   0 runner    (1001) docker     (122)      387 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/apps/asgi/commands/templates/app/app.py.jinja
--rw-r--r--   0 runner    (1001) docker     (122)      497 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/apps/asgi/commands/templates/app/conftest.py.jinja
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 12:16:11.000000 piccolo-0.98.0/piccolo/apps/asgi/commands/templates/app/home/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/apps/asgi/commands/templates/app/home/__init__.py.jinja
--rw-r--r--   0 runner    (1001) docker     (122)      510 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/apps/asgi/commands/templates/app/home/_blacksheep_endpoints.py.jinja
--rw-r--r--   0 runner    (1001) docker     (122)      498 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/apps/asgi/commands/templates/app/home/_starlette_endpoints.py.jinja
--rw-r--r--   0 runner    (1001) docker     (122)      530 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/apps/asgi/commands/templates/app/home/_starlite_endpoints.py.jinja
--rw-r--r--   0 runner    (1001) docker     (122)      402 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/apps/asgi/commands/templates/app/home/_xpresso_endpoints.py.jinja
--rw-r--r--   0 runner    (1001) docker     (122)      351 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/apps/asgi/commands/templates/app/home/endpoints.py.jinja
--rw-r--r--   0 runner    (1001) docker     (122)      505 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/apps/asgi/commands/templates/app/home/piccolo_app.py.jinja
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 12:16:11.000000 piccolo-0.98.0/piccolo/apps/asgi/commands/templates/app/home/piccolo_migrations/
--rw-r--r--   0 runner    (1001) docker     (122)       59 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/apps/asgi/commands/templates/app/home/piccolo_migrations/README.md
--rw-r--r--   0 runner    (1001) docker     (122)      197 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/apps/asgi/commands/templates/app/home/tables.py.jinja
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 12:16:11.000000 piccolo-0.98.0/piccolo/apps/asgi/commands/templates/app/home/templates/
--rw-r--r--   0 runner    (1001) docker     (122)      451 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/apps/asgi/commands/templates/app/home/templates/base.html.jinja_raw
--rw-r--r--   0 runner    (1001) docker     (122)     2452 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/apps/asgi/commands/templates/app/home/templates/home.html.jinja_raw
--rw-r--r--   0 runner    (1001) docker     (122)      421 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/apps/asgi/commands/templates/app/main.py.jinja
--rw-r--r--   0 runner    (1001) docker     (122)      379 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/apps/asgi/commands/templates/app/piccolo_conf.py.jinja
--rw-r--r--   0 runner    (1001) docker     (122)      235 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/apps/asgi/commands/templates/app/piccolo_conf_test.py.jinja
--rw-r--r--   0 runner    (1001) docker     (122)      152 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/apps/asgi/commands/templates/app/requirements.txt.jinja
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 12:16:11.000000 piccolo-0.98.0/piccolo/apps/asgi/commands/templates/app/static/
--rw-r--r--   0 runner    (1001) docker     (122)     7406 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/apps/asgi/commands/templates/app/static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (122)     1056 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/apps/asgi/commands/templates/app/static/main.css
--rw-r--r--   0 runner    (1001) docker     (122)      217 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/apps/asgi/piccolo_app.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 12:16:11.000000 piccolo-0.98.0/piccolo/apps/fixtures/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/apps/fixtures/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 12:16:11.000000 piccolo-0.98.0/piccolo/apps/fixtures/commands/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/apps/fixtures/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3650 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/apps/fixtures/commands/dump.py
--rw-r--r--   0 runner    (1001) docker     (122)     2130 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/apps/fixtures/commands/load.py
--rw-r--r--   0 runner    (1001) docker     (122)     1462 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/apps/fixtures/commands/shared.py
--rw-r--r--   0 runner    (1001) docker     (122)      268 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/apps/fixtures/piccolo_app.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 12:16:11.000000 piccolo-0.98.0/piccolo/apps/meta/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/apps/meta/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 12:16:11.000000 piccolo-0.98.0/piccolo/apps/meta/commands/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/apps/meta/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      115 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/apps/meta/commands/version.py
--rw-r--r--   0 runner    (1001) docker     (122)      224 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/apps/meta/piccolo_app.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 12:16:11.000000 piccolo-0.98.0/piccolo/apps/migrations/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/apps/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 12:16:11.000000 piccolo-0.98.0/piccolo/apps/migrations/auto/
--rw-r--r--   0 runner    (1001) docker     (122)      191 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/apps/migrations/auto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6745 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/apps/migrations/auto/diffable_table.py
--rw-r--r--   0 runner    (1001) docker     (122)    29004 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/apps/migrations/auto/migration_manager.py
--rw-r--r--   0 runner    (1001) docker     (122)     1013 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/apps/migrations/auto/operations.py
--rw-r--r--   0 runner    (1001) docker     (122)    20546 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/apps/migrations/auto/schema_differ.py
--rw-r--r--   0 runner    (1001) docker     (122)     4439 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/apps/migrations/auto/schema_snapshot.py
--rw-r--r--   0 runner    (1001) docker     (122)    23745 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/apps/migrations/auto/serialisation.py
--rw-r--r--   0 runner    (1001) docker     (122)     1752 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/apps/migrations/auto/serialisation_legacy.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 12:16:11.000000 piccolo-0.98.0/piccolo/apps/migrations/commands/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/apps/migrations/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6533 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/apps/migrations/commands/backwards.py
--rw-r--r--   0 runner    (1001) docker     (122)     4473 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/apps/migrations/commands/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     3982 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/apps/migrations/commands/check.py
--rw-r--r--   0 runner    (1001) docker     (122)     2834 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/apps/migrations/commands/clean.py
--rw-r--r--   0 runner    (1001) docker     (122)     5362 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/apps/migrations/commands/forwards.py
--rw-r--r--   0 runner    (1001) docker     (122)     6603 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/apps/migrations/commands/new.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 12:16:11.000000 piccolo-0.98.0/piccolo/apps/migrations/commands/templates/
--rw-r--r--   0 runner    (1001) docker     (122)      681 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/apps/migrations/commands/templates/migration.py.jinja
--rw-r--r--   0 runner    (1001) docker     (122)      593 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/apps/migrations/piccolo_app.py
--rw-r--r--   0 runner    (1001) docker     (122)      799 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/apps/migrations/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 12:16:11.000000 piccolo-0.98.0/piccolo/apps/playground/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/apps/playground/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 12:16:11.000000 piccolo-0.98.0/piccolo/apps/playground/commands/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/apps/playground/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6949 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/apps/playground/commands/run.py
--rw-r--r--   0 runner    (1001) docker     (122)      222 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/apps/playground/piccolo_app.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 12:16:11.000000 piccolo-0.98.0/piccolo/apps/project/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/apps/project/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 12:16:11.000000 piccolo-0.98.0/piccolo/apps/project/commands/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/apps/project/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1513 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/apps/project/commands/new.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 12:16:11.000000 piccolo-0.98.0/piccolo/apps/project/commands/templates/
--rw-r--r--   0 runner    (1001) docker     (122)      408 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/apps/project/commands/templates/piccolo_conf.py.jinja
--rw-r--r--   0 runner    (1001) docker     (122)      220 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/apps/project/piccolo_app.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 12:16:11.000000 piccolo-0.98.0/piccolo/apps/schema/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/apps/schema/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 12:16:11.000000 piccolo-0.98.0/piccolo/apps/schema/commands/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/apps/schema/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      236 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/apps/schema/commands/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)    30631 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/apps/schema/commands/generate.py
--rw-r--r--   0 runner    (1001) docker     (122)     3190 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/apps/schema/commands/graph.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 12:16:11.000000 piccolo-0.98.0/piccolo/apps/schema/commands/templates/
--rw-r--r--   0 runner    (1001) docker     (122)     1443 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/apps/schema/commands/templates/graphviz.dot.jinja
--rw-r--r--   0 runner    (1001) docker     (122)      432 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/apps/schema/piccolo_app.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 12:16:11.000000 piccolo-0.98.0/piccolo/apps/shell/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/apps/shell/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 12:16:11.000000 piccolo-0.98.0/piccolo/apps/shell/commands/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/apps/shell/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1707 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/apps/shell/commands/run.py
--rw-r--r--   0 runner    (1001) docker     (122)      217 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/apps/shell/piccolo_app.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 12:16:11.000000 piccolo-0.98.0/piccolo/apps/sql_shell/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/apps/sql_shell/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 12:16:11.000000 piccolo-0.98.0/piccolo/apps/sql_shell/commands/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/apps/sql_shell/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1984 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/apps/sql_shell/commands/run.py
--rw-r--r--   0 runner    (1001) docker     (122)      221 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/apps/sql_shell/piccolo_app.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 12:16:11.000000 piccolo-0.98.0/piccolo/apps/tester/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/apps/tester/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 12:16:11.000000 piccolo-0.98.0/piccolo/apps/tester/commands/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/apps/tester/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2431 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/apps/tester/commands/run.py
--rw-r--r--   0 runner    (1001) docker     (122)      225 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/apps/tester/piccolo_app.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 12:16:11.000000 piccolo-0.98.0/piccolo/apps/user/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/apps/user/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 12:16:11.000000 piccolo-0.98.0/piccolo/apps/user/commands/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/apps/user/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      649 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/apps/user/commands/change_password.py
--rw-r--r--   0 runner    (1001) docker     (122)     1463 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/apps/user/commands/change_permissions.py
--rw-r--r--   0 runner    (1001) docker     (122)     2273 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/apps/user/commands/create.py
--rw-r--r--   0 runner    (1001) docker     (122)      729 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/apps/user/piccolo_app.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 12:16:11.000000 piccolo-0.98.0/piccolo/apps/user/piccolo_migrations/
--rw-r--r--   0 runner    (1001) docker     (122)     2139 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/apps/user/piccolo_migrations/2019-11-14T21-52-21.py
--rw-r--r--   0 runner    (1001) docker     (122)      982 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/apps/user/piccolo_migrations/2020-06-11T21-38-55.py
--rw-r--r--   0 runner    (1001) docker     (122)     1219 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/apps/user/piccolo_migrations/2021-04-30T16-14-15.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/apps/user/piccolo_migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8203 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/apps/user/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 12:16:11.000000 piccolo-0.98.0/piccolo/columns/
--rw-r--r--   0 runner    (1001) docker     (122)     1120 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/columns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    29532 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/columns/base.py
--rw-r--r--   0 runner    (1001) docker     (122)      723 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/columns/choices.py
--rw-r--r--   0 runner    (1001) docker     (122)    77060 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/columns/column_types.py
--rw-r--r--   0 runner    (1001) docker     (122)     5262 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/columns/combination.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 12:16:11.000000 piccolo-0.98.0/piccolo/columns/defaults/
--rw-r--r--   0 runner    (1001) docker     (122)      145 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/columns/defaults/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1854 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/columns/defaults/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     2455 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/columns/defaults/date.py
--rw-r--r--   0 runner    (1001) docker     (122)     1975 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/columns/defaults/interval.py
--rw-r--r--   0 runner    (1001) docker     (122)     2355 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/columns/defaults/time.py
--rw-r--r--   0 runner    (1001) docker     (122)     3526 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/columns/defaults/timestamp.py
--rw-r--r--   0 runner    (1001) docker     (122)     2057 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/columns/defaults/timestamptz.py
--rw-r--r--   0 runner    (1001) docker     (122)      443 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/columns/defaults/uuid.py
--rw-r--r--   0 runner    (1001) docker     (122)      372 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/columns/indexes.py
--rw-r--r--   0 runner    (1001) docker     (122)    13943 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/columns/m2m.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 12:16:11.000000 piccolo-0.98.0/piccolo/columns/operators/
--rw-r--r--   0 runner    (1001) docker     (122)      310 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/columns/operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       34 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/columns/operators/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     1253 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/columns/operators/comparison.py
--rw-r--r--   0 runner    (1001) docker     (122)      325 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/columns/operators/math.py
--rw-r--r--   0 runner    (1001) docker     (122)      142 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/columns/operators/string.py
--rw-r--r--   0 runner    (1001) docker     (122)     1485 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/columns/readable.py
--rw-r--r--   0 runner    (1001) docker     (122)     3573 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/columns/reference.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 12:16:11.000000 piccolo-0.98.0/piccolo/conf/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    17145 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/conf/apps.py
--rw-r--r--   0 runner    (1001) docker     (122)      444 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/custom_types.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 12:16:11.000000 piccolo-0.98.0/piccolo/engine/
--rw-r--r--   0 runner    (1001) docker     (122)      283 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3702 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/engine/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     1466 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/engine/cockroach.py
--rw-r--r--   0 runner    (1001) docker     (122)       44 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/engine/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)      507 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/engine/finder.py
--rw-r--r--   0 runner    (1001) docker     (122)    14653 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/engine/postgres.py
--rw-r--r--   0 runner    (1001) docker     (122)    18699 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/engine/sqlite.py
--rw-r--r--   0 runner    (1001) docker     (122)     5024 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/main.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 12:16:11.000000 piccolo-0.98.0/piccolo/query/
--rw-r--r--   0 runner    (1001) docker     (122)      562 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    16091 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/query/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 12:16:11.000000 piccolo-0.98.0/piccolo/query/methods/
--rw-r--r--   0 runner    (1001) docker     (122)      421 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/query/methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    14890 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/query/methods/alter.py
--rw-r--r--   0 runner    (1001) docker     (122)     1098 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/query/methods/count.py
--rw-r--r--   0 runner    (1001) docker     (122)     1636 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/query/methods/create.py
--rw-r--r--   0 runner    (1001) docker     (122)     2594 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/query/methods/create_index.py
--rw-r--r--   0 runner    (1001) docker     (122)     1564 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/query/methods/delete.py
--rw-r--r--   0 runner    (1001) docker     (122)     1043 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/query/methods/drop_index.py
--rw-r--r--   0 runner    (1001) docker     (122)     1169 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/query/methods/exists.py
--rw-r--r--   0 runner    (1001) docker     (122)     1083 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/query/methods/indexes.py
--rw-r--r--   0 runner    (1001) docker     (122)     2797 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/query/methods/insert.py
--rw-r--r--   0 runner    (1001) docker     (122)     8814 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/query/methods/objects.py
--rw-r--r--   0 runner    (1001) docker     (122)      600 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/query/methods/raw.py
--rw-r--r--   0 runner    (1001) docker     (122)     2616 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/query/methods/refresh.py
--rw-r--r--   0 runner    (1001) docker     (122)    21796 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/query/methods/select.py
--rw-r--r--   0 runner    (1001) docker     (122)     1143 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/query/methods/table_exists.py
--rw-r--r--   0 runner    (1001) docker     (122)     3431 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/query/methods/update.py
--rw-r--r--   0 runner    (1001) docker     (122)    14631 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/query/mixins.py
--rw-r--r--   0 runner    (1001) docker     (122)     5859 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/querystring.py
--rw-r--r--   0 runner    (1001) docker     (122)    46497 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/table.py
--rw-r--r--   0 runner    (1001) docker     (122)     7094 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/table_reflection.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 12:16:11.000000 piccolo-0.98.0/piccolo/testing/
--rw-r--r--   0 runner    (1001) docker     (122)       83 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5635 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/testing/model_builder.py
--rw-r--r--   0 runner    (1001) docker     (122)     2005 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/testing/random_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 12:16:11.000000 piccolo-0.98.0/piccolo/utils/
--rw-r--r--   0 runner    (1001) docker     (122)       36 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1886 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/utils/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (122)      765 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/utils/encoding.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 12:16:11.000000 piccolo-0.98.0/piccolo/utils/graphlib/
--rw-r--r--   0 runner    (1001) docker     (122)      200 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/utils/graphlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9677 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/utils/graphlib/_graphlib.py
--rw-r--r--   0 runner    (1001) docker     (122)     1912 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/utils/lazy_loader.py
--rw-r--r--   0 runner    (1001) docker     (122)      276 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/utils/naming.py
--rw-r--r--   0 runner    (1001) docker     (122)     1631 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/utils/objects.py
--rw-r--r--   0 runner    (1001) docker     (122)      310 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/utils/printing.py
--rw-r--r--   0 runner    (1001) docker     (122)    10749 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/utils/pydantic.py
--rw-r--r--   0 runner    (1001) docker     (122)      787 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/utils/repr.py
--rw-r--r--   0 runner    (1001) docker     (122)     1272 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/utils/sql_values.py
--rw-r--r--   0 runner    (1001) docker     (122)      819 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/utils/sync.py
--rw-r--r--   0 runner    (1001) docker     (122)     1247 2022-12-02 12:15:55.000000 piccolo-0.98.0/piccolo/utils/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 12:16:11.000000 piccolo-0.98.0/piccolo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     5591 2022-12-02 12:16:10.000000 piccolo-0.98.0/piccolo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    12783 2022-12-02 12:16:10.000000 piccolo-0.98.0/piccolo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-02 12:16:10.000000 piccolo-0.98.0/piccolo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       47 2022-12-02 12:16:10.000000 piccolo-0.98.0/piccolo.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      386 2022-12-02 12:16:10.000000 piccolo-0.98.0/piccolo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       24 2022-12-02 12:16:10.000000 piccolo-0.98.0/piccolo.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 12:16:11.000000 piccolo-0.98.0/profiling/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 12:15:55.000000 piccolo-0.98.0/profiling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      829 2022-12-02 12:15:55.000000 piccolo-0.98.0/profiling/run_profile.py
--rw-r--r--   0 runner    (1001) docker     (122)      756 2022-12-02 12:15:55.000000 piccolo-0.98.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-12-02 12:16:11.000000 piccolo-0.98.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     3008 2022-12-02 12:15:55.000000 piccolo-0.98.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 12:16:10.000000 piccolo-0.98.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 12:16:11.000000 piccolo-0.98.0/tests/apps/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 12:16:11.000000 piccolo-0.98.0/tests/apps/app/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/apps/app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 12:16:11.000000 piccolo-0.98.0/tests/apps/app/commands/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/apps/app/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1152 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/apps/app/commands/test_new.py
--rw-r--r--   0 runner    (1001) docker     (122)      551 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/apps/app/commands/test_show_all.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 12:16:11.000000 piccolo-0.98.0/tests/apps/asgi/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/apps/asgi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 12:16:11.000000 piccolo-0.98.0/tests/apps/asgi/commands/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/apps/asgi/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3097 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/apps/asgi/commands/test_new.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 12:16:11.000000 piccolo-0.98.0/tests/apps/fixtures/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/apps/fixtures/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 12:16:11.000000 piccolo-0.98.0/tests/apps/fixtures/commands/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/apps/fixtures/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7464 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/apps/fixtures/commands/test_dump_load.py
--rw-r--r--   0 runner    (1001) docker     (122)     2139 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/apps/fixtures/commands/test_shared.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 12:16:11.000000 piccolo-0.98.0/tests/apps/meta/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/apps/meta/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 12:16:11.000000 piccolo-0.98.0/tests/apps/meta/commands/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/apps/meta/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      316 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/apps/meta/commands/test_version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 12:16:11.000000 piccolo-0.98.0/tests/apps/migrations/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/apps/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 12:16:11.000000 piccolo-0.98.0/tests/apps/migrations/auto/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/apps/migrations/auto/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 12:16:11.000000 piccolo-0.98.0/tests/apps/migrations/auto/integration/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/apps/migrations/auto/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    32788 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/apps/migrations/auto/integration/test_migrations.py
--rw-r--r--   0 runner    (1001) docker     (122)     2932 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/apps/migrations/auto/test_diffable_table.py
--rw-r--r--   0 runner    (1001) docker     (122)    33919 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/apps/migrations/auto/test_migration_manager.py
--rw-r--r--   0 runner    (1001) docker     (122)    16245 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/apps/migrations/auto/test_schema_differ.py
--rw-r--r--   0 runner    (1001) docker     (122)     6196 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/apps/migrations/auto/test_schema_snapshot.py
--rw-r--r--   0 runner    (1001) docker     (122)    14170 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/apps/migrations/auto/test_serialisation.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 12:16:11.000000 piccolo-0.98.0/tests/apps/migrations/commands/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/apps/migrations/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1829 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/apps/migrations/commands/test_base.py
--rw-r--r--   0 runner    (1001) docker     (122)      630 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/apps/migrations/commands/test_check.py
--rw-r--r--   0 runner    (1001) docker     (122)     1124 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/apps/migrations/commands/test_clean.py
--rw-r--r--   0 runner    (1001) docker     (122)     7029 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/apps/migrations/commands/test_forwards_backwards.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 12:16:11.000000 piccolo-0.98.0/tests/apps/migrations/commands/test_migrations/
--rw-r--r--   0 runner    (1001) docker     (122)      601 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/apps/migrations/commands/test_migrations/2020-03-31T20-38-22.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/apps/migrations/commands/test_migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1699 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/apps/migrations/commands/test_new.py
--rw-r--r--   0 runner    (1001) docker     (122)      308 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/apps/migrations/test_migration.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 12:16:11.000000 piccolo-0.98.0/tests/apps/project/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/apps/project/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 12:16:11.000000 piccolo-0.98.0/tests/apps/project/commands/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/apps/project/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      409 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/apps/project/commands/test_new.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 12:16:11.000000 piccolo-0.98.0/tests/apps/schema/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/apps/schema/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 12:16:11.000000 piccolo-0.98.0/tests/apps/shell/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/apps/shell/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 12:16:11.000000 piccolo-0.98.0/tests/apps/shell/commands/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/apps/shell/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1132 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/apps/shell/commands/test_run.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 12:16:11.000000 piccolo-0.98.0/tests/apps/sql_shell/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/apps/sql_shell/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 12:16:11.000000 piccolo-0.98.0/tests/apps/sql_shell/commands/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/apps/sql_shell/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      425 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/apps/sql_shell/commands/test_run.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 12:16:11.000000 piccolo-0.98.0/tests/apps/tester/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/apps/tester/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 12:16:11.000000 piccolo-0.98.0/tests/apps/user/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/apps/user/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 12:16:11.000000 piccolo-0.98.0/tests/apps/user/commands/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/apps/user/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1051 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/apps/user/commands/test_change_password.py
--rw-r--r--   0 runner    (1001) docker     (122)     2108 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/apps/user/commands/test_change_permissions.py
--rw-r--r--   0 runner    (1001) docker     (122)     2250 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/apps/user/commands/test_create.py
--rw-r--r--   0 runner    (1001) docker     (122)     7583 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/apps/user/test_tables.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 12:16:11.000000 piccolo-0.98.0/tests/columns/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/columns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4856 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/columns/test_array.py
--rw-r--r--   0 runner    (1001) docker     (122)     3902 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/columns/test_base.py
--rw-r--r--   0 runner    (1001) docker     (122)     1149 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/columns/test_bigint.py
--rw-r--r--   0 runner    (1001) docker     (122)     1527 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/columns/test_boolean.py
--rw-r--r--   0 runner    (1001) docker     (122)     1580 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/columns/test_bytea.py
--rw-r--r--   0 runner    (1001) docker     (122)     1955 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/columns/test_choices.py
--rw-r--r--   0 runner    (1001) docker     (122)     1156 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/columns/test_combination.py
--rw-r--r--   0 runner    (1001) docker     (122)     1175 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/columns/test_date.py
--rw-r--r--   0 runner    (1001) docker     (122)     7567 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/columns/test_db_column_name.py
--rw-r--r--   0 runner    (1001) docker     (122)     2768 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/columns/test_defaults.py
--rw-r--r--   0 runner    (1001) docker     (122)      607 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/columns/test_double_precision.py
--rw-r--r--   0 runner    (1001) docker     (122)     2921 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/columns/test_interval.py
--rw-r--r--   0 runner    (1001) docker     (122)     3814 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/columns/test_json.py
--rw-r--r--   0 runner    (1001) docker     (122)     6821 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/columns/test_jsonb.py
--rw-r--r--   0 runner    (1001) docker     (122)    24609 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/columns/test_m2m.py
--rw-r--r--   0 runner    (1001) docker     (122)      813 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/columns/test_numeric.py
--rw-r--r--   0 runner    (1001) docker     (122)     5396 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/columns/test_primary_key.py
--rw-r--r--   0 runner    (1001) docker     (122)      802 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/columns/test_readable.py
--rw-r--r--   0 runner    (1001) docker     (122)      574 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/columns/test_real.py
--rw-r--r--   0 runner    (1001) docker     (122)     1507 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/columns/test_reference.py
--rw-r--r--   0 runner    (1001) docker     (122)     1514 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/columns/test_reserved_column_names.py
--rw-r--r--   0 runner    (1001) docker     (122)     1115 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/columns/test_smallint.py
--rw-r--r--   0 runner    (1001) docker     (122)     1742 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/columns/test_time.py
--rw-r--r--   0 runner    (1001) docker     (122)     1831 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/columns/test_timestamp.py
--rw-r--r--   0 runner    (1001) docker     (122)     2771 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/columns/test_timestamptz.py
--rw-r--r--   0 runner    (1001) docker     (122)      466 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/columns/test_uuid.py
--rw-r--r--   0 runner    (1001) docker     (122)      813 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/columns/test_varchar.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 12:16:11.000000 piccolo-0.98.0/tests/conf/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      346 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/conf/example.py
--rw-r--r--   0 runner    (1001) docker     (122)     7370 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/conf/test_apps.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 12:16:11.000000 piccolo-0.98.0/tests/engine/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1181 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/engine/test_extra_nodes.py
--rw-r--r--   0 runner    (1001) docker     (122)     2175 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/engine/test_nested_transaction.py
--rw-r--r--   0 runner    (1001) docker     (122)     3839 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/engine/test_pool.py
--rw-r--r--   0 runner    (1001) docker     (122)     7339 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/engine/test_transaction.py
--rw-r--r--   0 runner    (1001) docker     (122)      793 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/engine/test_version_parsing.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 12:16:11.000000 piccolo-0.98.0/tests/example_apps/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/example_apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 12:16:11.000000 piccolo-0.98.0/tests/example_apps/mega/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/example_apps/mega/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      363 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/example_apps/mega/piccolo_app.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 12:16:11.000000 piccolo-0.98.0/tests/example_apps/mega/piccolo_migrations/
--rw-r--r--   0 runner    (1001) docker     (122)    11834 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/example_apps/mega/piccolo_migrations/2021-09-20T21-23-25-698988.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/example_apps/mega/piccolo_migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2359 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/example_apps/mega/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 12:16:11.000000 piccolo-0.98.0/tests/example_apps/music/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/example_apps/music/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      568 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/example_apps/music/piccolo_app.py
--rw-r--r--   0 runner    (1001) docker     (122)     2267 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/example_apps/music/tables.py
--rw-r--r--   0 runner    (1001) docker     (122)     2240 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/example_apps/music/tables_detailed.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 12:16:11.000000 piccolo-0.98.0/tests/query/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/query/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 12:16:11.000000 piccolo-0.98.0/tests/query/mixins/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/query/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2025 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/query/mixins/test_columns_delegate.py
--rw-r--r--   0 runner    (1001) docker     (122)      507 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/query/mixins/test_order_by_delegate.py
--rw-r--r--   0 runner    (1001) docker     (122)      412 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/query/test_await.py
--rw-r--r--   0 runner    (1001) docker     (122)     1765 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/query/test_camelcase.py
--rw-r--r--   0 runner    (1001) docker     (122)     3419 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/query/test_freeze.py
--rw-r--r--   0 runner    (1001) docker     (122)      730 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/query/test_gather.py
--rw-r--r--   0 runner    (1001) docker     (122)      880 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/query/test_querystring.py
--rw-r--r--   0 runner    (1001) docker     (122)      994 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/query/test_slots.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 12:16:11.000000 piccolo-0.98.0/tests/table/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/table/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 12:16:11.000000 piccolo-0.98.0/tests/table/instance/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/table/instance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1105 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/table/instance/test_create.py
--rw-r--r--   0 runner    (1001) docker     (122)     1175 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/table/instance/test_get_related.py
--rw-r--r--   0 runner    (1001) docker     (122)     4690 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/table/instance/test_get_related_readable.py
--rw-r--r--   0 runner    (1001) docker     (122)      958 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/table/instance/test_instantiate.py
--rw-r--r--   0 runner    (1001) docker     (122)      648 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/table/instance/test_remove.py
--rw-r--r--   0 runner    (1001) docker     (122)     4388 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/table/instance/test_save.py
--rw-r--r--   0 runner    (1001) docker     (122)     3262 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/table/instance/test_to_dict.py
--rw-r--r--   0 runner    (1001) docker     (122)      667 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/table/test_all_columns.py
--rw-r--r--   0 runner    (1001) docker     (122)    10728 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/table/test_alter.py
--rw-r--r--   0 runner    (1001) docker     (122)     3740 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/table/test_batch.py
--rw-r--r--   0 runner    (1001) docker     (122)     6381 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/table/test_callback.py
--rw-r--r--   0 runner    (1001) docker     (122)      832 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/table/test_constructor.py
--rw-r--r--   0 runner    (1001) docker     (122)      285 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/table/test_count.py
--rw-r--r--   0 runner    (1001) docker     (122)     1431 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/table/test_create.py
--rw-r--r--   0 runner    (1001) docker     (122)      903 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/table/test_create_db_tables.py
--rw-r--r--   0 runner    (1001) docker     (122)     1341 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/table/test_create_table_class.py
--rw-r--r--   0 runner    (1001) docker     (122)      653 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/table/test_delete.py
--rw-r--r--   0 runner    (1001) docker     (122)     1116 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/table/test_drop_db_tables.py
--rw-r--r--   0 runner    (1001) docker     (122)      283 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/table/test_exists.py
--rw-r--r--   0 runner    (1001) docker     (122)      840 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/table/test_from_dict.py
--rw-r--r--   0 runner    (1001) docker     (122)     1990 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/table/test_indexes.py
--rw-r--r--   0 runner    (1001) docker     (122)     3034 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/table/test_inheritance.py
--rw-r--r--   0 runner    (1001) docker     (122)     2274 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/table/test_insert.py
--rw-r--r--   0 runner    (1001) docker     (122)    14109 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/table/test_join.py
--rw-r--r--   0 runner    (1001) docker     (122)     2637 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/table/test_metaclass.py
--rw-r--r--   0 runner    (1001) docker     (122)     7895 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/table/test_objects.py
--rw-r--r--   0 runner    (1001) docker     (122)     2980 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/table/test_output.py
--rw-r--r--   0 runner    (1001) docker     (122)     1683 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/table/test_raw.py
--rw-r--r--   0 runner    (1001) docker     (122)      269 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/table/test_ref.py
--rw-r--r--   0 runner    (1001) docker     (122)     2695 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/table/test_refresh.py
--rw-r--r--   0 runner    (1001) docker     (122)      411 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/table/test_repr.py
--rw-r--r--   0 runner    (1001) docker     (122)    34014 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/table/test_select.py
--rw-r--r--   0 runner    (1001) docker     (122)     1731 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/table/test_str.py
--rw-r--r--   0 runner    (1001) docker     (122)      375 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/table/test_table_exists.py
--rw-r--r--   0 runner    (1001) docker     (122)    17748 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/table/test_update.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 12:16:11.000000 piccolo-0.98.0/tests/testing/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4236 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/testing/test_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (122)     1694 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/testing/test_random_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 12:16:11.000000 piccolo-0.98.0/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1480 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/utils/test_dictionary.py
--rw-r--r--   0 runner    (1001) docker     (122)      326 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/utils/test_encoding.py
--rw-r--r--   0 runner    (1001) docker     (122)      998 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/utils/test_lazy_loader.py
--rw-r--r--   0 runner    (1001) docker     (122)      661 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/utils/test_naming.py
--rw-r--r--   0 runner    (1001) docker     (122)      668 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/utils/test_printing.py
--rw-r--r--   0 runner    (1001) docker     (122)    20917 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/utils/test_pydantic.py
--rw-r--r--   0 runner    (1001) docker     (122)     1630 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/utils/test_sql_values.py
--rw-r--r--   0 runner    (1001) docker     (122)      799 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/utils/test_sync.py
--rw-r--r--   0 runner    (1001) docker     (122)     3794 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/utils/test_table_reflection.py
--rw-r--r--   0 runner    (1001) docker     (122)      269 2022-12-02 12:15:55.000000 piccolo-0.98.0/tests/utils/test_warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:22.000000 piccolo-0.99.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     5591 2022-12-02 13:06:22.000000 piccolo-0.99.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3460 2022-12-02 13:06:06.000000 piccolo-0.99.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:21.000000 piccolo-0.99.0/piccolo/
+-rw-r--r--   0 runner    (1001) docker     (122)       23 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:21.000000 piccolo-0.99.0/piccolo/apps/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:21.000000 piccolo-0.99.0/piccolo/apps/app/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:21.000000 piccolo-0.99.0/piccolo/apps/app/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/app/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2187 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/app/commands/new.py
+-rw-r--r--   0 runner    (1001) docker     (122)      252 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/app/commands/show_all.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:21.000000 piccolo-0.99.0/piccolo/apps/app/commands/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)      428 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/app/commands/templates/piccolo_app.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (122)       32 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/app/commands/templates/tables.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (122)      340 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/app/piccolo_app.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:21.000000 piccolo-0.99.0/piccolo/apps/asgi/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/asgi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:21.000000 piccolo-0.99.0/piccolo/apps/asgi/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/asgi/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4160 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/asgi/commands/new.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:21.000000 piccolo-0.99.0/piccolo/apps/asgi/commands/templates/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:21.000000 piccolo-0.99.0/piccolo/apps/asgi/commands/templates/app/
+-rw-r--r--   0 runner    (1001) docker     (122)      214 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/asgi/commands/templates/app/README.md.jinja
+-rw-r--r--   0 runner    (1001) docker     (122)     3117 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/asgi/commands/templates/app/_blacksheep_app.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (122)     2436 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/asgi/commands/templates/app/_fastapi_app.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (122)     1271 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/asgi/commands/templates/app/_starlette_app.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (122)     2889 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/asgi/commands/templates/app/_starlite_app.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (122)     2855 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/asgi/commands/templates/app/_xpresso_app.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (122)      387 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/asgi/commands/templates/app/app.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (122)      497 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/asgi/commands/templates/app/conftest.py.jinja
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:21.000000 piccolo-0.99.0/piccolo/apps/asgi/commands/templates/app/home/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/asgi/commands/templates/app/home/__init__.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (122)      510 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/asgi/commands/templates/app/home/_blacksheep_endpoints.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (122)      498 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/asgi/commands/templates/app/home/_starlette_endpoints.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (122)      530 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/asgi/commands/templates/app/home/_starlite_endpoints.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (122)      402 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/asgi/commands/templates/app/home/_xpresso_endpoints.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (122)      351 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/asgi/commands/templates/app/home/endpoints.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (122)      505 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/asgi/commands/templates/app/home/piccolo_app.py.jinja
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:21.000000 piccolo-0.99.0/piccolo/apps/asgi/commands/templates/app/home/piccolo_migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)       59 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/asgi/commands/templates/app/home/piccolo_migrations/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      197 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/asgi/commands/templates/app/home/tables.py.jinja
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:21.000000 piccolo-0.99.0/piccolo/apps/asgi/commands/templates/app/home/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)      451 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/asgi/commands/templates/app/home/templates/base.html.jinja_raw
+-rw-r--r--   0 runner    (1001) docker     (122)     2452 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/asgi/commands/templates/app/home/templates/home.html.jinja_raw
+-rw-r--r--   0 runner    (1001) docker     (122)      421 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/asgi/commands/templates/app/main.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (122)      379 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/asgi/commands/templates/app/piccolo_conf.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (122)      235 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/asgi/commands/templates/app/piccolo_conf_test.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (122)      152 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/asgi/commands/templates/app/requirements.txt.jinja
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:21.000000 piccolo-0.99.0/piccolo/apps/asgi/commands/templates/app/static/
+-rw-r--r--   0 runner    (1001) docker     (122)     7406 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/asgi/commands/templates/app/static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (122)     1056 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/asgi/commands/templates/app/static/main.css
+-rw-r--r--   0 runner    (1001) docker     (122)      217 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/asgi/piccolo_app.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:21.000000 piccolo-0.99.0/piccolo/apps/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/fixtures/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:21.000000 piccolo-0.99.0/piccolo/apps/fixtures/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/fixtures/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3650 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/fixtures/commands/dump.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2130 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/fixtures/commands/load.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1462 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/fixtures/commands/shared.py
+-rw-r--r--   0 runner    (1001) docker     (122)      268 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/fixtures/piccolo_app.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:21.000000 piccolo-0.99.0/piccolo/apps/meta/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/meta/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:21.000000 piccolo-0.99.0/piccolo/apps/meta/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/meta/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      115 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/meta/commands/version.py
+-rw-r--r--   0 runner    (1001) docker     (122)      224 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/meta/piccolo_app.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:21.000000 piccolo-0.99.0/piccolo/apps/migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:21.000000 piccolo-0.99.0/piccolo/apps/migrations/auto/
+-rw-r--r--   0 runner    (1001) docker     (122)      191 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/migrations/auto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6745 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/migrations/auto/diffable_table.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29004 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/migrations/auto/migration_manager.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1013 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/migrations/auto/operations.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20546 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/migrations/auto/schema_differ.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4439 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/migrations/auto/schema_snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23745 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/migrations/auto/serialisation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1752 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/migrations/auto/serialisation_legacy.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:21.000000 piccolo-0.99.0/piccolo/apps/migrations/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/migrations/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6533 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/migrations/commands/backwards.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4473 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/migrations/commands/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3982 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/migrations/commands/check.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2834 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/migrations/commands/clean.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5362 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/migrations/commands/forwards.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6603 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/migrations/commands/new.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:21.000000 piccolo-0.99.0/piccolo/apps/migrations/commands/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)      681 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/migrations/commands/templates/migration.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (122)      593 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/migrations/piccolo_app.py
+-rw-r--r--   0 runner    (1001) docker     (122)      799 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/migrations/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:21.000000 piccolo-0.99.0/piccolo/apps/playground/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/playground/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:21.000000 piccolo-0.99.0/piccolo/apps/playground/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/playground/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6949 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/playground/commands/run.py
+-rw-r--r--   0 runner    (1001) docker     (122)      222 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/playground/piccolo_app.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:21.000000 piccolo-0.99.0/piccolo/apps/project/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/project/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:21.000000 piccolo-0.99.0/piccolo/apps/project/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/project/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1513 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/project/commands/new.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:21.000000 piccolo-0.99.0/piccolo/apps/project/commands/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)      408 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/project/commands/templates/piccolo_conf.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (122)      220 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/project/piccolo_app.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:21.000000 piccolo-0.99.0/piccolo/apps/schema/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/schema/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:21.000000 piccolo-0.99.0/piccolo/apps/schema/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/schema/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      236 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/schema/commands/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    30631 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/schema/commands/generate.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3190 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/schema/commands/graph.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:21.000000 piccolo-0.99.0/piccolo/apps/schema/commands/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)     1443 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/schema/commands/templates/graphviz.dot.jinja
+-rw-r--r--   0 runner    (1001) docker     (122)      432 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/schema/piccolo_app.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:21.000000 piccolo-0.99.0/piccolo/apps/shell/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/shell/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:21.000000 piccolo-0.99.0/piccolo/apps/shell/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/shell/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1707 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/shell/commands/run.py
+-rw-r--r--   0 runner    (1001) docker     (122)      217 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/shell/piccolo_app.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:21.000000 piccolo-0.99.0/piccolo/apps/sql_shell/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/sql_shell/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:21.000000 piccolo-0.99.0/piccolo/apps/sql_shell/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/sql_shell/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1984 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/sql_shell/commands/run.py
+-rw-r--r--   0 runner    (1001) docker     (122)      221 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/sql_shell/piccolo_app.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:21.000000 piccolo-0.99.0/piccolo/apps/tester/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/tester/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:21.000000 piccolo-0.99.0/piccolo/apps/tester/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/tester/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2431 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/tester/commands/run.py
+-rw-r--r--   0 runner    (1001) docker     (122)      225 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/tester/piccolo_app.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:21.000000 piccolo-0.99.0/piccolo/apps/user/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/user/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:22.000000 piccolo-0.99.0/piccolo/apps/user/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/user/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      649 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/user/commands/change_password.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1463 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/user/commands/change_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2273 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/user/commands/create.py
+-rw-r--r--   0 runner    (1001) docker     (122)      729 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/user/piccolo_app.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:22.000000 piccolo-0.99.0/piccolo/apps/user/piccolo_migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)     2139 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/user/piccolo_migrations/2019-11-14T21-52-21.py
+-rw-r--r--   0 runner    (1001) docker     (122)      982 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/user/piccolo_migrations/2020-06-11T21-38-55.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1219 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/user/piccolo_migrations/2021-04-30T16-14-15.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/user/piccolo_migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8203 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/apps/user/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:22.000000 piccolo-0.99.0/piccolo/columns/
+-rw-r--r--   0 runner    (1001) docker     (122)     1120 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/columns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29532 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/columns/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)      723 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/columns/choices.py
+-rw-r--r--   0 runner    (1001) docker     (122)    77060 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/columns/column_types.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5262 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/columns/combination.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:22.000000 piccolo-0.99.0/piccolo/columns/defaults/
+-rw-r--r--   0 runner    (1001) docker     (122)      145 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/columns/defaults/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1854 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/columns/defaults/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2455 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/columns/defaults/date.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1975 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/columns/defaults/interval.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2355 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/columns/defaults/time.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3526 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/columns/defaults/timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2057 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/columns/defaults/timestamptz.py
+-rw-r--r--   0 runner    (1001) docker     (122)      443 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/columns/defaults/uuid.py
+-rw-r--r--   0 runner    (1001) docker     (122)      372 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/columns/indexes.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13943 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/columns/m2m.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:22.000000 piccolo-0.99.0/piccolo/columns/operators/
+-rw-r--r--   0 runner    (1001) docker     (122)      310 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/columns/operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       34 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/columns/operators/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1253 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/columns/operators/comparison.py
+-rw-r--r--   0 runner    (1001) docker     (122)      325 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/columns/operators/math.py
+-rw-r--r--   0 runner    (1001) docker     (122)      142 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/columns/operators/string.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1485 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/columns/readable.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3573 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/columns/reference.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:22.000000 piccolo-0.99.0/piccolo/conf/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17145 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/conf/apps.py
+-rw-r--r--   0 runner    (1001) docker     (122)      444 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/custom_types.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:22.000000 piccolo-0.99.0/piccolo/engine/
+-rw-r--r--   0 runner    (1001) docker     (122)      283 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3702 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/engine/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1466 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/engine/cockroach.py
+-rw-r--r--   0 runner    (1001) docker     (122)       44 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/engine/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)      507 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/engine/finder.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14653 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/engine/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18699 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/engine/sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5024 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:22.000000 piccolo-0.99.0/piccolo/query/
+-rw-r--r--   0 runner    (1001) docker     (122)      562 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16091 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/query/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:22.000000 piccolo-0.99.0/piccolo/query/methods/
+-rw-r--r--   0 runner    (1001) docker     (122)      421 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/query/methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14890 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/query/methods/alter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1098 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/query/methods/count.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1636 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/query/methods/create.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2594 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/query/methods/create_index.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2147 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/query/methods/delete.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1043 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/query/methods/drop_index.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1169 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/query/methods/exists.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1083 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/query/methods/indexes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2797 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/query/methods/insert.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8814 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/query/methods/objects.py
+-rw-r--r--   0 runner    (1001) docker     (122)      600 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/query/methods/raw.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2616 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/query/methods/refresh.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21796 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/query/methods/select.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1143 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/query/methods/table_exists.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3431 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/query/methods/update.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14631 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/query/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5859 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/querystring.py
+-rw-r--r--   0 runner    (1001) docker     (122)    46497 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/table.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7094 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/table_reflection.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:22.000000 piccolo-0.99.0/piccolo/testing/
+-rw-r--r--   0 runner    (1001) docker     (122)       83 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5635 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/testing/model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2005 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/testing/random_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:22.000000 piccolo-0.99.0/piccolo/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)       36 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1886 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/utils/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (122)      765 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/utils/encoding.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:22.000000 piccolo-0.99.0/piccolo/utils/graphlib/
+-rw-r--r--   0 runner    (1001) docker     (122)      200 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/utils/graphlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9677 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/utils/graphlib/_graphlib.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1912 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/utils/lazy_loader.py
+-rw-r--r--   0 runner    (1001) docker     (122)      276 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/utils/naming.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1631 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/utils/objects.py
+-rw-r--r--   0 runner    (1001) docker     (122)      310 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/utils/printing.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10749 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/utils/pydantic.py
+-rw-r--r--   0 runner    (1001) docker     (122)      787 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/utils/repr.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1272 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/utils/sql_values.py
+-rw-r--r--   0 runner    (1001) docker     (122)      819 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/utils/sync.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1247 2022-12-02 13:06:06.000000 piccolo-0.99.0/piccolo/utils/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:21.000000 piccolo-0.99.0/piccolo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     5591 2022-12-02 13:06:21.000000 piccolo-0.99.0/piccolo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    12783 2022-12-02 13:06:21.000000 piccolo-0.99.0/piccolo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-02 13:06:21.000000 piccolo-0.99.0/piccolo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       47 2022-12-02 13:06:21.000000 piccolo-0.99.0/piccolo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      386 2022-12-02 13:06:21.000000 piccolo-0.99.0/piccolo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       24 2022-12-02 13:06:21.000000 piccolo-0.99.0/piccolo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:22.000000 piccolo-0.99.0/profiling/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/profiling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      829 2022-12-02 13:06:06.000000 piccolo-0.99.0/profiling/run_profile.py
+-rw-r--r--   0 runner    (1001) docker     (122)      756 2022-12-02 13:06:06.000000 piccolo-0.99.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2022-12-02 13:06:22.000000 piccolo-0.99.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     3008 2022-12-02 13:06:06.000000 piccolo-0.99.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:21.000000 piccolo-0.99.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:22.000000 piccolo-0.99.0/tests/apps/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:22.000000 piccolo-0.99.0/tests/apps/app/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/apps/app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:22.000000 piccolo-0.99.0/tests/apps/app/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/apps/app/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1152 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/apps/app/commands/test_new.py
+-rw-r--r--   0 runner    (1001) docker     (122)      551 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/apps/app/commands/test_show_all.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:22.000000 piccolo-0.99.0/tests/apps/asgi/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/apps/asgi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:22.000000 piccolo-0.99.0/tests/apps/asgi/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/apps/asgi/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3097 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/apps/asgi/commands/test_new.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:22.000000 piccolo-0.99.0/tests/apps/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/apps/fixtures/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:22.000000 piccolo-0.99.0/tests/apps/fixtures/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/apps/fixtures/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7464 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/apps/fixtures/commands/test_dump_load.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2139 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/apps/fixtures/commands/test_shared.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:22.000000 piccolo-0.99.0/tests/apps/meta/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/apps/meta/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:22.000000 piccolo-0.99.0/tests/apps/meta/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/apps/meta/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      316 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/apps/meta/commands/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:22.000000 piccolo-0.99.0/tests/apps/migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/apps/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:22.000000 piccolo-0.99.0/tests/apps/migrations/auto/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/apps/migrations/auto/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:22.000000 piccolo-0.99.0/tests/apps/migrations/auto/integration/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/apps/migrations/auto/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    32788 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/apps/migrations/auto/integration/test_migrations.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2932 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/apps/migrations/auto/test_diffable_table.py
+-rw-r--r--   0 runner    (1001) docker     (122)    33919 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/apps/migrations/auto/test_migration_manager.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16245 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/apps/migrations/auto/test_schema_differ.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6196 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/apps/migrations/auto/test_schema_snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14170 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/apps/migrations/auto/test_serialisation.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:22.000000 piccolo-0.99.0/tests/apps/migrations/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/apps/migrations/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1829 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/apps/migrations/commands/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (122)      630 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/apps/migrations/commands/test_check.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1124 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/apps/migrations/commands/test_clean.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7029 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/apps/migrations/commands/test_forwards_backwards.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:22.000000 piccolo-0.99.0/tests/apps/migrations/commands/test_migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)      601 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/apps/migrations/commands/test_migrations/2020-03-31T20-38-22.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/apps/migrations/commands/test_migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1699 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/apps/migrations/commands/test_new.py
+-rw-r--r--   0 runner    (1001) docker     (122)      308 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/apps/migrations/test_migration.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:22.000000 piccolo-0.99.0/tests/apps/project/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/apps/project/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:22.000000 piccolo-0.99.0/tests/apps/project/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/apps/project/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      409 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/apps/project/commands/test_new.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:22.000000 piccolo-0.99.0/tests/apps/schema/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/apps/schema/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:22.000000 piccolo-0.99.0/tests/apps/shell/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/apps/shell/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:22.000000 piccolo-0.99.0/tests/apps/shell/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/apps/shell/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1132 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/apps/shell/commands/test_run.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:22.000000 piccolo-0.99.0/tests/apps/sql_shell/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/apps/sql_shell/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:22.000000 piccolo-0.99.0/tests/apps/sql_shell/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/apps/sql_shell/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      425 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/apps/sql_shell/commands/test_run.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:22.000000 piccolo-0.99.0/tests/apps/tester/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/apps/tester/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:22.000000 piccolo-0.99.0/tests/apps/user/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/apps/user/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:22.000000 piccolo-0.99.0/tests/apps/user/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/apps/user/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1051 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/apps/user/commands/test_change_password.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2108 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/apps/user/commands/test_change_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2250 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/apps/user/commands/test_create.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7583 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/apps/user/test_tables.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:22.000000 piccolo-0.99.0/tests/columns/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/columns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4856 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/columns/test_array.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3902 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/columns/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1149 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/columns/test_bigint.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1527 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/columns/test_boolean.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1580 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/columns/test_bytea.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1955 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/columns/test_choices.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1156 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/columns/test_combination.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1175 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/columns/test_date.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7567 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/columns/test_db_column_name.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2768 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/columns/test_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (122)      607 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/columns/test_double_precision.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2921 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/columns/test_interval.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3814 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/columns/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6821 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/columns/test_jsonb.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24609 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/columns/test_m2m.py
+-rw-r--r--   0 runner    (1001) docker     (122)      813 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/columns/test_numeric.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5396 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/columns/test_primary_key.py
+-rw-r--r--   0 runner    (1001) docker     (122)      802 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/columns/test_readable.py
+-rw-r--r--   0 runner    (1001) docker     (122)      574 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/columns/test_real.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1507 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/columns/test_reference.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1514 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/columns/test_reserved_column_names.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1115 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/columns/test_smallint.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1742 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/columns/test_time.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1831 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/columns/test_timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2771 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/columns/test_timestamptz.py
+-rw-r--r--   0 runner    (1001) docker     (122)      466 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/columns/test_uuid.py
+-rw-r--r--   0 runner    (1001) docker     (122)      813 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/columns/test_varchar.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:22.000000 piccolo-0.99.0/tests/conf/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      346 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/conf/example.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7370 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/conf/test_apps.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:22.000000 piccolo-0.99.0/tests/engine/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1181 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/engine/test_extra_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2175 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/engine/test_nested_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3839 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/engine/test_pool.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7339 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/engine/test_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (122)      793 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/engine/test_version_parsing.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:22.000000 piccolo-0.99.0/tests/example_apps/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/example_apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:22.000000 piccolo-0.99.0/tests/example_apps/mega/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/example_apps/mega/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      363 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/example_apps/mega/piccolo_app.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:22.000000 piccolo-0.99.0/tests/example_apps/mega/piccolo_migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)    11834 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/example_apps/mega/piccolo_migrations/2021-09-20T21-23-25-698988.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/example_apps/mega/piccolo_migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2359 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/example_apps/mega/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:22.000000 piccolo-0.99.0/tests/example_apps/music/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/example_apps/music/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      568 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/example_apps/music/piccolo_app.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2267 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/example_apps/music/tables.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2240 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/example_apps/music/tables_detailed.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:22.000000 piccolo-0.99.0/tests/query/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/query/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:22.000000 piccolo-0.99.0/tests/query/mixins/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/query/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2025 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/query/mixins/test_columns_delegate.py
+-rw-r--r--   0 runner    (1001) docker     (122)      507 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/query/mixins/test_order_by_delegate.py
+-rw-r--r--   0 runner    (1001) docker     (122)      412 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/query/test_await.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1765 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/query/test_camelcase.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3419 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/query/test_freeze.py
+-rw-r--r--   0 runner    (1001) docker     (122)      730 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/query/test_gather.py
+-rw-r--r--   0 runner    (1001) docker     (122)      880 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/query/test_querystring.py
+-rw-r--r--   0 runner    (1001) docker     (122)      994 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/query/test_slots.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:22.000000 piccolo-0.99.0/tests/table/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/table/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:22.000000 piccolo-0.99.0/tests/table/instance/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/table/instance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1105 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/table/instance/test_create.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1175 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/table/instance/test_get_related.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4690 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/table/instance/test_get_related_readable.py
+-rw-r--r--   0 runner    (1001) docker     (122)      958 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/table/instance/test_instantiate.py
+-rw-r--r--   0 runner    (1001) docker     (122)      648 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/table/instance/test_remove.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4388 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/table/instance/test_save.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3262 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/table/instance/test_to_dict.py
+-rw-r--r--   0 runner    (1001) docker     (122)      667 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/table/test_all_columns.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10728 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/table/test_alter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3740 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/table/test_batch.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6381 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/table/test_callback.py
+-rw-r--r--   0 runner    (1001) docker     (122)      832 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/table/test_constructor.py
+-rw-r--r--   0 runner    (1001) docker     (122)      285 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/table/test_count.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1431 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/table/test_create.py
+-rw-r--r--   0 runner    (1001) docker     (122)      903 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/table/test_create_db_tables.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1341 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/table/test_create_table_class.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1252 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/table/test_delete.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1116 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/table/test_drop_db_tables.py
+-rw-r--r--   0 runner    (1001) docker     (122)      283 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/table/test_exists.py
+-rw-r--r--   0 runner    (1001) docker     (122)      840 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/table/test_from_dict.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1990 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/table/test_indexes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3034 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/table/test_inheritance.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2274 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/table/test_insert.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14109 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/table/test_join.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2637 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/table/test_metaclass.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7895 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/table/test_objects.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2980 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/table/test_output.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1683 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/table/test_raw.py
+-rw-r--r--   0 runner    (1001) docker     (122)      269 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/table/test_ref.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2695 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/table/test_refresh.py
+-rw-r--r--   0 runner    (1001) docker     (122)      411 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/table/test_repr.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34014 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/table/test_select.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1731 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/table/test_str.py
+-rw-r--r--   0 runner    (1001) docker     (122)      375 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/table/test_table_exists.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17748 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/table/test_update.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:22.000000 piccolo-0.99.0/tests/testing/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4236 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/testing/test_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1694 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/testing/test_random_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:22.000000 piccolo-0.99.0/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1480 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/utils/test_dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (122)      326 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/utils/test_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (122)      998 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/utils/test_lazy_loader.py
+-rw-r--r--   0 runner    (1001) docker     (122)      661 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/utils/test_naming.py
+-rw-r--r--   0 runner    (1001) docker     (122)      668 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/utils/test_printing.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20917 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/utils/test_pydantic.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1630 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/utils/test_sql_values.py
+-rw-r--r--   0 runner    (1001) docker     (122)      799 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/utils/test_sync.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3794 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/utils/test_table_reflection.py
+-rw-r--r--   0 runner    (1001) docker     (122)      269 2022-12-02 13:06:06.000000 piccolo-0.99.0/tests/utils/test_warnings.py
```

### Comparing `piccolo-0.98.0/PKG-INFO` & `piccolo-0.99.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piccolo
-Version: 0.98.0
+Version: 0.99.0
 Summary: A fast, user friendly ORM and query builder which supports asyncio.
 Home-page: https://github.com/piccolo-orm/piccolo
 Author: Daniel Townsend
 Author-email: dan@dantownsend.co.uk
 License: MIT
 Project-URL: Documentation, https://piccolo-orm.readthedocs.io/en/latest/index.html
 Project-URL: Source, https://github.com/piccolo-orm/piccolo
```

### Comparing `piccolo-0.98.0/README.md` & `piccolo-0.99.0/README.md`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/piccolo/apps/app/commands/new.py` & `piccolo-0.99.0/piccolo/apps/app/commands/new.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/piccolo/apps/asgi/commands/new.py` & `piccolo-0.99.0/piccolo/apps/asgi/commands/new.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/piccolo/apps/asgi/commands/templates/app/_blacksheep_app.py.jinja` & `piccolo-0.99.0/piccolo/apps/asgi/commands/templates/app/_blacksheep_app.py.jinja`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/piccolo/apps/asgi/commands/templates/app/_fastapi_app.py.jinja` & `piccolo-0.99.0/piccolo/apps/asgi/commands/templates/app/_fastapi_app.py.jinja`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/piccolo/apps/asgi/commands/templates/app/_starlette_app.py.jinja` & `piccolo-0.99.0/piccolo/apps/asgi/commands/templates/app/_starlette_app.py.jinja`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/piccolo/apps/asgi/commands/templates/app/_starlite_app.py.jinja` & `piccolo-0.99.0/piccolo/apps/asgi/commands/templates/app/_starlite_app.py.jinja`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/piccolo/apps/asgi/commands/templates/app/_xpresso_app.py.jinja` & `piccolo-0.99.0/piccolo/apps/asgi/commands/templates/app/_xpresso_app.py.jinja`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/piccolo/apps/asgi/commands/templates/app/home/_starlite_endpoints.py.jinja` & `piccolo-0.99.0/piccolo/apps/asgi/commands/templates/app/home/_starlite_endpoints.py.jinja`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/piccolo/apps/asgi/commands/templates/app/home/templates/home.html.jinja_raw` & `piccolo-0.99.0/piccolo/apps/asgi/commands/templates/app/home/templates/home.html.jinja_raw`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/piccolo/apps/asgi/commands/templates/app/static/favicon.ico` & `piccolo-0.99.0/piccolo/apps/asgi/commands/templates/app/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/piccolo/apps/asgi/commands/templates/app/static/main.css` & `piccolo-0.99.0/piccolo/apps/asgi/commands/templates/app/static/main.css`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/piccolo/apps/fixtures/commands/dump.py` & `piccolo-0.99.0/piccolo/apps/fixtures/commands/dump.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/piccolo/apps/fixtures/commands/load.py` & `piccolo-0.99.0/piccolo/apps/fixtures/commands/load.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/piccolo/apps/fixtures/commands/shared.py` & `piccolo-0.99.0/piccolo/apps/fixtures/commands/shared.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/piccolo/apps/migrations/auto/diffable_table.py` & `piccolo-0.99.0/piccolo/apps/migrations/auto/diffable_table.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/piccolo/apps/migrations/auto/migration_manager.py` & `piccolo-0.99.0/piccolo/apps/migrations/auto/migration_manager.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/piccolo/apps/migrations/auto/operations.py` & `piccolo-0.99.0/piccolo/apps/migrations/auto/operations.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/piccolo/apps/migrations/auto/schema_differ.py` & `piccolo-0.99.0/piccolo/apps/migrations/auto/schema_differ.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/piccolo/apps/migrations/auto/schema_snapshot.py` & `piccolo-0.99.0/piccolo/apps/migrations/auto/schema_snapshot.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/piccolo/apps/migrations/auto/serialisation.py` & `piccolo-0.99.0/piccolo/apps/migrations/auto/serialisation.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/piccolo/apps/migrations/auto/serialisation_legacy.py` & `piccolo-0.99.0/piccolo/apps/migrations/auto/serialisation_legacy.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/piccolo/apps/migrations/commands/backwards.py` & `piccolo-0.99.0/piccolo/apps/migrations/commands/backwards.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/piccolo/apps/migrations/commands/base.py` & `piccolo-0.99.0/piccolo/apps/migrations/commands/base.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/piccolo/apps/migrations/commands/check.py` & `piccolo-0.99.0/piccolo/apps/migrations/commands/check.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/piccolo/apps/migrations/commands/clean.py` & `piccolo-0.99.0/piccolo/apps/migrations/commands/clean.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/piccolo/apps/migrations/commands/forwards.py` & `piccolo-0.99.0/piccolo/apps/migrations/commands/forwards.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/piccolo/apps/migrations/commands/new.py` & `piccolo-0.99.0/piccolo/apps/migrations/commands/new.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/piccolo/apps/migrations/commands/templates/migration.py.jinja` & `piccolo-0.99.0/piccolo/apps/migrations/commands/templates/migration.py.jinja`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/piccolo/apps/migrations/piccolo_app.py` & `piccolo-0.99.0/piccolo/apps/migrations/piccolo_app.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/piccolo/apps/migrations/tables.py` & `piccolo-0.99.0/piccolo/apps/migrations/tables.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/piccolo/apps/playground/commands/run.py` & `piccolo-0.99.0/piccolo/apps/playground/commands/run.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/piccolo/apps/project/commands/new.py` & `piccolo-0.99.0/piccolo/apps/project/commands/new.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/piccolo/apps/schema/commands/generate.py` & `piccolo-0.99.0/piccolo/apps/schema/commands/generate.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/piccolo/apps/schema/commands/graph.py` & `piccolo-0.99.0/piccolo/apps/schema/commands/graph.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/piccolo/apps/schema/commands/templates/graphviz.dot.jinja` & `piccolo-0.99.0/piccolo/apps/schema/commands/templates/graphviz.dot.jinja`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/piccolo/apps/shell/commands/run.py` & `piccolo-0.99.0/piccolo/apps/shell/commands/run.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/piccolo/apps/sql_shell/commands/run.py` & `piccolo-0.99.0/piccolo/apps/sql_shell/commands/run.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/piccolo/apps/tester/commands/run.py` & `piccolo-0.99.0/piccolo/apps/tester/commands/run.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/piccolo/apps/user/commands/change_password.py` & `piccolo-0.99.0/piccolo/apps/user/commands/change_password.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/piccolo/apps/user/commands/change_permissions.py` & `piccolo-0.99.0/piccolo/apps/user/commands/change_permissions.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/piccolo/apps/user/commands/create.py` & `piccolo-0.99.0/piccolo/apps/user/commands/create.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/piccolo/apps/user/piccolo_app.py` & `piccolo-0.99.0/piccolo/apps/user/piccolo_app.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/piccolo/apps/user/piccolo_migrations/2019-11-14T21-52-21.py` & `piccolo-0.99.0/piccolo/apps/user/piccolo_migrations/2019-11-14T21-52-21.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/piccolo/apps/user/piccolo_migrations/2020-06-11T21-38-55.py` & `piccolo-0.99.0/piccolo/apps/user/piccolo_migrations/2020-06-11T21-38-55.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/piccolo/apps/user/piccolo_migrations/2021-04-30T16-14-15.py` & `piccolo-0.99.0/piccolo/apps/user/piccolo_migrations/2021-04-30T16-14-15.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/piccolo/apps/user/tables.py` & `piccolo-0.99.0/piccolo/apps/user/tables.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/piccolo/columns/__init__.py` & `piccolo-0.99.0/piccolo/columns/__init__.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/piccolo/columns/base.py` & `piccolo-0.99.0/piccolo/columns/base.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/piccolo/columns/choices.py` & `piccolo-0.99.0/piccolo/columns/choices.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/piccolo/columns/column_types.py` & `piccolo-0.99.0/piccolo/columns/column_types.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/piccolo/columns/combination.py` & `piccolo-0.99.0/piccolo/columns/combination.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/piccolo/columns/defaults/base.py` & `piccolo-0.99.0/piccolo/columns/defaults/base.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/piccolo/columns/defaults/date.py` & `piccolo-0.99.0/piccolo/columns/defaults/date.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/piccolo/columns/defaults/interval.py` & `piccolo-0.99.0/piccolo/columns/defaults/interval.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/piccolo/columns/defaults/time.py` & `piccolo-0.99.0/piccolo/columns/defaults/time.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/piccolo/columns/defaults/timestamp.py` & `piccolo-0.99.0/piccolo/columns/defaults/timestamp.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/piccolo/columns/defaults/timestamptz.py` & `piccolo-0.99.0/piccolo/columns/defaults/timestamptz.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/piccolo/columns/m2m.py` & `piccolo-0.99.0/piccolo/columns/m2m.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/piccolo/columns/operators/comparison.py` & `piccolo-0.99.0/piccolo/columns/operators/comparison.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/piccolo/columns/readable.py` & `piccolo-0.99.0/piccolo/columns/readable.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/piccolo/columns/reference.py` & `piccolo-0.99.0/piccolo/columns/reference.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/piccolo/conf/apps.py` & `piccolo-0.99.0/piccolo/conf/apps.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/piccolo/engine/base.py` & `piccolo-0.99.0/piccolo/engine/base.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/piccolo/engine/cockroach.py` & `piccolo-0.99.0/piccolo/engine/cockroach.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/piccolo/engine/postgres.py` & `piccolo-0.99.0/piccolo/engine/postgres.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/piccolo/engine/sqlite.py` & `piccolo-0.99.0/piccolo/engine/sqlite.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/piccolo/main.py` & `piccolo-0.99.0/piccolo/main.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/piccolo/query/__init__.py` & `piccolo-0.99.0/piccolo/query/__init__.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/piccolo/query/base.py` & `piccolo-0.99.0/piccolo/query/base.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/piccolo/query/methods/alter.py` & `piccolo-0.99.0/piccolo/query/methods/alter.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/piccolo/query/methods/count.py` & `piccolo-0.99.0/piccolo/query/methods/count.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/piccolo/query/methods/create.py` & `piccolo-0.99.0/piccolo/query/methods/create.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/piccolo/query/methods/create_index.py` & `piccolo-0.99.0/piccolo/query/methods/create_index.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/piccolo/query/methods/delete.py` & `piccolo-0.99.0/piccolo/query/methods/delete.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,47 @@
 from __future__ import annotations
 
 import typing as t
 
 from piccolo.custom_types import Combinable
 from piccolo.query.base import Query
-from piccolo.query.mixins import WhereDelegate
+from piccolo.query.mixins import ReturningDelegate, WhereDelegate
 from piccolo.querystring import QueryString
 
 if t.TYPE_CHECKING:  # pragma: no cover
+    from piccolo.columns import Column
     from piccolo.table import Table
 
 
 class DeletionError(Exception):
     pass
 
 
 class Delete(Query):
 
-    __slots__ = ("force", "where_delegate")
+    __slots__ = (
+        "force",
+        "returning_delegate",
+        "where_delegate",
+    )
 
     def __init__(self, table: t.Type[Table], force: bool = False, **kwargs):
         super().__init__(table, **kwargs)
         self.force = force
+        self.returning_delegate = ReturningDelegate()
         self.where_delegate = WhereDelegate()
 
     def where(self, *where: Combinable) -> Delete:
         self.where_delegate.where(*where)
         return self
 
+    def returning(self, *columns: Column) -> Delete:
+        self.returning_delegate.returning(columns)
+        return self
+
     def _validate(self):
         """
         Don't let a deletion happen unless it has a where clause, or is
         explicitly forced.
         """
         if (not self.where_delegate._where) and (not self.force):
             classname = self.table.__name__
@@ -40,12 +50,25 @@
                 f"{classname}? If so, use {classname}.delete(force=True). "
                 "Otherwise, add a where clause."
             )
 
     @property
     def default_querystrings(self) -> t.Sequence[QueryString]:
         query = f"DELETE FROM {self.table._meta.tablename}"
+
+        querystring = QueryString(query)
+
         if self.where_delegate._where:
-            query += " WHERE {}"
-            return [QueryString(query, self.where_delegate._where.querystring)]
-        else:
-            return [QueryString(query)]
+            querystring = QueryString(
+                "{} WHERE {}",
+                querystring,
+                self.where_delegate._where.querystring,
+            )
+
+        if self.returning_delegate._returning:
+            querystring = QueryString(
+                "{}{}",
+                querystring,
+                self.returning_delegate._returning.querystring,
+            )
+
+        return [querystring]
```

### Comparing `piccolo-0.98.0/piccolo/query/methods/drop_index.py` & `piccolo-0.99.0/piccolo/query/methods/drop_index.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/piccolo/query/methods/exists.py` & `piccolo-0.99.0/piccolo/query/methods/exists.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/piccolo/query/methods/indexes.py` & `piccolo-0.99.0/piccolo/query/methods/indexes.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/piccolo/query/methods/insert.py` & `piccolo-0.99.0/piccolo/query/methods/insert.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/piccolo/query/methods/objects.py` & `piccolo-0.99.0/piccolo/query/methods/objects.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/piccolo/query/methods/raw.py` & `piccolo-0.99.0/piccolo/query/methods/raw.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/piccolo/query/methods/refresh.py` & `piccolo-0.99.0/piccolo/query/methods/refresh.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/piccolo/query/methods/select.py` & `piccolo-0.99.0/piccolo/query/methods/select.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/piccolo/query/methods/table_exists.py` & `piccolo-0.99.0/piccolo/query/methods/table_exists.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/piccolo/query/methods/update.py` & `piccolo-0.99.0/piccolo/query/methods/update.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/piccolo/query/mixins.py` & `piccolo-0.99.0/piccolo/query/mixins.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/piccolo/querystring.py` & `piccolo-0.99.0/piccolo/querystring.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/piccolo/table.py` & `piccolo-0.99.0/piccolo/table.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/piccolo/table_reflection.py` & `piccolo-0.99.0/piccolo/table_reflection.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/piccolo/testing/model_builder.py` & `piccolo-0.99.0/piccolo/testing/model_builder.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/piccolo/testing/random_builder.py` & `piccolo-0.99.0/piccolo/testing/random_builder.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/piccolo/utils/dictionary.py` & `piccolo-0.99.0/piccolo/utils/dictionary.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/piccolo/utils/encoding.py` & `piccolo-0.99.0/piccolo/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/piccolo/utils/graphlib/_graphlib.py` & `piccolo-0.99.0/piccolo/utils/graphlib/_graphlib.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/piccolo/utils/lazy_loader.py` & `piccolo-0.99.0/piccolo/utils/lazy_loader.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/piccolo/utils/objects.py` & `piccolo-0.99.0/piccolo/utils/objects.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/piccolo/utils/pydantic.py` & `piccolo-0.99.0/piccolo/utils/pydantic.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/piccolo/utils/repr.py` & `piccolo-0.99.0/piccolo/utils/repr.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/piccolo/utils/sql_values.py` & `piccolo-0.99.0/piccolo/utils/sql_values.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/piccolo/utils/sync.py` & `piccolo-0.99.0/piccolo/utils/sync.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/piccolo/utils/warnings.py` & `piccolo-0.99.0/piccolo/utils/warnings.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/piccolo.egg-info/PKG-INFO` & `piccolo-0.99.0/piccolo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piccolo
-Version: 0.98.0
+Version: 0.99.0
 Summary: A fast, user friendly ORM and query builder which supports asyncio.
 Home-page: https://github.com/piccolo-orm/piccolo
 Author: Daniel Townsend
 Author-email: dan@dantownsend.co.uk
 License: MIT
 Project-URL: Documentation, https://piccolo-orm.readthedocs.io/en/latest/index.html
 Project-URL: Source, https://github.com/piccolo-orm/piccolo
```

### Comparing `piccolo-0.98.0/piccolo.egg-info/SOURCES.txt` & `piccolo-0.99.0/piccolo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/profiling/run_profile.py` & `piccolo-0.99.0/profiling/run_profile.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/pyproject.toml` & `piccolo-0.99.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/setup.py` & `piccolo-0.99.0/setup.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/tests/apps/app/commands/test_new.py` & `piccolo-0.99.0/tests/apps/app/commands/test_new.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/tests/apps/app/commands/test_show_all.py` & `piccolo-0.99.0/tests/apps/app/commands/test_show_all.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/tests/apps/asgi/commands/test_new.py` & `piccolo-0.99.0/tests/apps/asgi/commands/test_new.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/tests/apps/fixtures/commands/test_dump_load.py` & `piccolo-0.99.0/tests/apps/fixtures/commands/test_dump_load.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/tests/apps/fixtures/commands/test_shared.py` & `piccolo-0.99.0/tests/apps/fixtures/commands/test_shared.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/tests/apps/migrations/auto/integration/test_migrations.py` & `piccolo-0.99.0/tests/apps/migrations/auto/integration/test_migrations.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/tests/apps/migrations/auto/test_diffable_table.py` & `piccolo-0.99.0/tests/apps/migrations/auto/test_diffable_table.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/tests/apps/migrations/auto/test_migration_manager.py` & `piccolo-0.99.0/tests/apps/migrations/auto/test_migration_manager.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/tests/apps/migrations/auto/test_schema_differ.py` & `piccolo-0.99.0/tests/apps/migrations/auto/test_schema_differ.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/tests/apps/migrations/auto/test_schema_snapshot.py` & `piccolo-0.99.0/tests/apps/migrations/auto/test_schema_snapshot.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/tests/apps/migrations/auto/test_serialisation.py` & `piccolo-0.99.0/tests/apps/migrations/auto/test_serialisation.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/tests/apps/migrations/commands/test_base.py` & `piccolo-0.99.0/tests/apps/migrations/commands/test_base.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/tests/apps/migrations/commands/test_check.py` & `piccolo-0.99.0/tests/apps/migrations/commands/test_check.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/tests/apps/migrations/commands/test_clean.py` & `piccolo-0.99.0/tests/apps/migrations/commands/test_clean.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/tests/apps/migrations/commands/test_forwards_backwards.py` & `piccolo-0.99.0/tests/apps/migrations/commands/test_forwards_backwards.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/tests/apps/migrations/commands/test_migrations/2020-03-31T20-38-22.py` & `piccolo-0.99.0/tests/apps/migrations/commands/test_migrations/2020-03-31T20-38-22.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/tests/apps/migrations/commands/test_new.py` & `piccolo-0.99.0/tests/apps/migrations/commands/test_new.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/tests/apps/shell/commands/test_run.py` & `piccolo-0.99.0/tests/apps/shell/commands/test_run.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/tests/apps/user/commands/test_change_password.py` & `piccolo-0.99.0/tests/apps/user/commands/test_change_password.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/tests/apps/user/commands/test_change_permissions.py` & `piccolo-0.99.0/tests/apps/user/commands/test_change_permissions.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/tests/apps/user/commands/test_create.py` & `piccolo-0.99.0/tests/apps/user/commands/test_create.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/tests/apps/user/test_tables.py` & `piccolo-0.99.0/tests/apps/user/test_tables.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/tests/columns/test_array.py` & `piccolo-0.99.0/tests/columns/test_array.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/tests/columns/test_base.py` & `piccolo-0.99.0/tests/columns/test_base.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/tests/columns/test_bigint.py` & `piccolo-0.99.0/tests/columns/test_bigint.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/tests/columns/test_boolean.py` & `piccolo-0.99.0/tests/columns/test_boolean.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/tests/columns/test_bytea.py` & `piccolo-0.99.0/tests/columns/test_bytea.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/tests/columns/test_choices.py` & `piccolo-0.99.0/tests/columns/test_choices.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/tests/columns/test_combination.py` & `piccolo-0.99.0/tests/columns/test_combination.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/tests/columns/test_date.py` & `piccolo-0.99.0/tests/columns/test_date.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/tests/columns/test_db_column_name.py` & `piccolo-0.99.0/tests/columns/test_db_column_name.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/tests/columns/test_defaults.py` & `piccolo-0.99.0/tests/columns/test_defaults.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/tests/columns/test_double_precision.py` & `piccolo-0.99.0/tests/columns/test_double_precision.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/tests/columns/test_interval.py` & `piccolo-0.99.0/tests/columns/test_interval.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/tests/columns/test_json.py` & `piccolo-0.99.0/tests/columns/test_json.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/tests/columns/test_jsonb.py` & `piccolo-0.99.0/tests/columns/test_jsonb.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/tests/columns/test_m2m.py` & `piccolo-0.99.0/tests/columns/test_m2m.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/tests/columns/test_numeric.py` & `piccolo-0.99.0/tests/columns/test_numeric.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/tests/columns/test_primary_key.py` & `piccolo-0.99.0/tests/columns/test_primary_key.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/tests/columns/test_readable.py` & `piccolo-0.99.0/tests/columns/test_readable.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/tests/columns/test_real.py` & `piccolo-0.99.0/tests/columns/test_real.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/tests/columns/test_reference.py` & `piccolo-0.99.0/tests/columns/test_reference.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/tests/columns/test_reserved_column_names.py` & `piccolo-0.99.0/tests/columns/test_reserved_column_names.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/tests/columns/test_smallint.py` & `piccolo-0.99.0/tests/columns/test_smallint.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/tests/columns/test_time.py` & `piccolo-0.99.0/tests/columns/test_time.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/tests/columns/test_timestamp.py` & `piccolo-0.99.0/tests/columns/test_timestamp.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/tests/columns/test_timestamptz.py` & `piccolo-0.99.0/tests/columns/test_timestamptz.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/tests/columns/test_varchar.py` & `piccolo-0.99.0/tests/columns/test_varchar.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/tests/conf/test_apps.py` & `piccolo-0.99.0/tests/conf/test_apps.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/tests/engine/test_extra_nodes.py` & `piccolo-0.99.0/tests/engine/test_extra_nodes.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/tests/engine/test_nested_transaction.py` & `piccolo-0.99.0/tests/engine/test_nested_transaction.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/tests/engine/test_pool.py` & `piccolo-0.99.0/tests/engine/test_pool.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/tests/engine/test_transaction.py` & `piccolo-0.99.0/tests/engine/test_transaction.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/tests/engine/test_version_parsing.py` & `piccolo-0.99.0/tests/engine/test_version_parsing.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/tests/example_apps/mega/piccolo_migrations/2021-09-20T21-23-25-698988.py` & `piccolo-0.99.0/tests/example_apps/mega/piccolo_migrations/2021-09-20T21-23-25-698988.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/tests/example_apps/mega/tables.py` & `piccolo-0.99.0/tests/example_apps/mega/tables.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/tests/example_apps/music/piccolo_app.py` & `piccolo-0.99.0/tests/example_apps/music/piccolo_app.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/tests/example_apps/music/tables.py` & `piccolo-0.99.0/tests/example_apps/music/tables.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/tests/example_apps/music/tables_detailed.py` & `piccolo-0.99.0/tests/example_apps/music/tables_detailed.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/tests/query/mixins/test_columns_delegate.py` & `piccolo-0.99.0/tests/query/mixins/test_columns_delegate.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/tests/query/test_camelcase.py` & `piccolo-0.99.0/tests/query/test_camelcase.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/tests/query/test_freeze.py` & `piccolo-0.99.0/tests/query/test_freeze.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/tests/query/test_gather.py` & `piccolo-0.99.0/tests/query/test_gather.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/tests/query/test_querystring.py` & `piccolo-0.99.0/tests/query/test_querystring.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/tests/query/test_slots.py` & `piccolo-0.99.0/tests/query/test_slots.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/tests/table/instance/test_create.py` & `piccolo-0.99.0/tests/table/instance/test_create.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/tests/table/instance/test_get_related.py` & `piccolo-0.99.0/tests/table/instance/test_get_related.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/tests/table/instance/test_get_related_readable.py` & `piccolo-0.99.0/tests/table/instance/test_get_related_readable.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/tests/table/instance/test_instantiate.py` & `piccolo-0.99.0/tests/table/instance/test_instantiate.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/tests/table/instance/test_remove.py` & `piccolo-0.99.0/tests/table/instance/test_remove.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/tests/table/instance/test_save.py` & `piccolo-0.99.0/tests/table/instance/test_save.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/tests/table/instance/test_to_dict.py` & `piccolo-0.99.0/tests/table/instance/test_to_dict.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/tests/table/test_all_columns.py` & `piccolo-0.99.0/tests/table/test_all_columns.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/tests/table/test_alter.py` & `piccolo-0.99.0/tests/table/test_alter.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/tests/table/test_batch.py` & `piccolo-0.99.0/tests/table/test_batch.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/tests/table/test_callback.py` & `piccolo-0.99.0/tests/table/test_callback.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/tests/table/test_constructor.py` & `piccolo-0.99.0/tests/table/test_constructor.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/tests/table/test_create.py` & `piccolo-0.99.0/tests/table/test_create.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/tests/table/test_create_db_tables.py` & `piccolo-0.99.0/tests/table/test_create_db_tables.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/tests/table/test_create_table_class.py` & `piccolo-0.99.0/tests/table/test_create_table_class.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/tests/table/test_drop_db_tables.py` & `piccolo-0.99.0/tests/table/test_drop_db_tables.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/tests/table/test_from_dict.py` & `piccolo-0.99.0/tests/table/test_from_dict.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/tests/table/test_indexes.py` & `piccolo-0.99.0/tests/table/test_indexes.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/tests/table/test_inheritance.py` & `piccolo-0.99.0/tests/table/test_inheritance.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/tests/table/test_insert.py` & `piccolo-0.99.0/tests/table/test_insert.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/tests/table/test_join.py` & `piccolo-0.99.0/tests/table/test_join.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/tests/table/test_metaclass.py` & `piccolo-0.99.0/tests/table/test_metaclass.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/tests/table/test_objects.py` & `piccolo-0.99.0/tests/table/test_objects.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/tests/table/test_output.py` & `piccolo-0.99.0/tests/table/test_output.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/tests/table/test_raw.py` & `piccolo-0.99.0/tests/table/test_raw.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/tests/table/test_refresh.py` & `piccolo-0.99.0/tests/table/test_refresh.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/tests/table/test_select.py` & `piccolo-0.99.0/tests/table/test_select.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/tests/table/test_str.py` & `piccolo-0.99.0/tests/table/test_str.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/tests/table/test_update.py` & `piccolo-0.99.0/tests/table/test_update.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/tests/testing/test_model_builder.py` & `piccolo-0.99.0/tests/testing/test_model_builder.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/tests/testing/test_random_builder.py` & `piccolo-0.99.0/tests/testing/test_random_builder.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/tests/utils/test_dictionary.py` & `piccolo-0.99.0/tests/utils/test_dictionary.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/tests/utils/test_lazy_loader.py` & `piccolo-0.99.0/tests/utils/test_lazy_loader.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/tests/utils/test_naming.py` & `piccolo-0.99.0/tests/utils/test_naming.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/tests/utils/test_printing.py` & `piccolo-0.99.0/tests/utils/test_printing.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/tests/utils/test_pydantic.py` & `piccolo-0.99.0/tests/utils/test_pydantic.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/tests/utils/test_sql_values.py` & `piccolo-0.99.0/tests/utils/test_sql_values.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/tests/utils/test_sync.py` & `piccolo-0.99.0/tests/utils/test_sync.py`

 * *Files identical despite different names*

### Comparing `piccolo-0.98.0/tests/utils/test_table_reflection.py` & `piccolo-0.99.0/tests/utils/test_table_reflection.py`

 * *Files identical despite different names*

