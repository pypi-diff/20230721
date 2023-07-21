# Comparing `tmp/kiara_plugin.service-0.4.6.tar.gz` & `tmp/kiara_plugin.service-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kiara_plugin.service-0.4.6.tar", last modified: Fri Jul 14 14:13:20 2023, max compression
+gzip compressed data, was "kiara_plugin.service-0.4.7.tar", last modified: Fri Jul 21 10:29:27 2023, max compression
```

## Comparing `kiara_plugin.service-0.4.6.tar` & `kiara_plugin.service-0.4.7.tar`

### file list

```diff
@@ -1,137 +1,137 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:13:20.513764 kiara_plugin.service-0.4.6/
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/.cruft.json
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/.envrc.disabled
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:13:20.501764 kiara_plugin.service-0.4.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:13:20.505764 kiara_plugin.service-0.4.6/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/.github/ISSUE_TEMPLATE/suggest-a-module.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:13:20.505764 kiara_plugin.service-0.4.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/.github/workflows/build-darwin.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     7488 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/.github/workflows/build-linux.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/.github/workflows/build-windows.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     5851 2023-07-14 14:13:20.513764 kiara_plugin.service-0.4.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:13:20.501764 kiara_plugin.service-0.4.6/ci/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:13:20.505764 kiara_plugin.service-0.4.6/ci/conda/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/ci/conda/conda-pkg-patch.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:13:20.505764 kiara_plugin.service-0.4.6/ci/conda/kiara_plugin.service/
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/ci/conda/kiara_plugin.service/meta.yaml.template
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/commitlint.config.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:13:20.505764 kiara_plugin.service-0.4.6/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/docs/SUMMARY.md
--rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/docs/development.md
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:13:20.505764 kiara_plugin.service-0.4.6/docs/stylesheets/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/docs/stylesheets/extra.css
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/docs/usage.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:13:20.501764 kiara_plugin.service-0.4.6/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:13:20.505764 kiara_plugin.service-0.4.6/examples/data/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/examples/data/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:13:20.505764 kiara_plugin.service-0.4.6/examples/data/journals/
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/examples/data/journals/JournalEdges1902.csv
--rw-r--r--   0 runner    (1001) docker     (123)    33121 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/examples/data/journals/JournalNodes1902.csv
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/examples/data/journals/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:13:20.505764 kiara_plugin.service-0.4.6/examples/jobs/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/examples/jobs/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:13:20.505764 kiara_plugin.service-0.4.6/examples/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/examples/pipelines/Readme.md
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/examples/pipelines/example_pipeline_service.yaml
--rw-r--r--   0 runner    (1001) docker     (123)   171640 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/kiara_import.profile
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:13:20.501764 kiara_plugin.service-0.4.6/scripts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:13:20.505764 kiara_plugin.service-0.4.6/scripts/documentation/
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/scripts/documentation/gen_api_doc_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/scripts/documentation/gen_info_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/scripts/documentation/gen_module_doc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-07-14 14:13:20.513764 kiara_plugin.service-0.4.6/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1393 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:13:20.501764 kiara_plugin.service-0.4.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:13:20.501764 kiara_plugin.service-0.4.6/src/kiara_plugin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:13:20.509764 kiara_plugin.service-0.4.6/src/kiara_plugin/service/
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/src/kiara_plugin/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/src/kiara_plugin/service/data_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/src/kiara_plugin/service/defaults.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:13:20.509764 kiara_plugin.service-0.4.6/src/kiara_plugin/service/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/src/kiara_plugin/service/interfaces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:13:20.509764 kiara_plugin.service-0.4.6/src/kiara_plugin/service/interfaces/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/src/kiara_plugin/service/interfaces/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:13:20.509764 kiara_plugin.service-0.4.6/src/kiara_plugin/service/interfaces/cli/service/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/src/kiara_plugin/service/interfaces/cli/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/src/kiara_plugin/service/interfaces/cli/service/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/src/kiara_plugin/service/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:13:20.509764 kiara_plugin.service-0.4.6/src/kiara_plugin/service/modules/
--rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/src/kiara_plugin/service/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:13:20.509764 kiara_plugin.service-0.4.6/src/kiara_plugin/service/openapi/
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/src/kiara_plugin/service/openapi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:13:20.509764 kiara_plugin.service-0.4.6/src/kiara_plugin/service/openapi/controllers/
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/src/kiara_plugin/service/openapi/controllers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/src/kiara_plugin/service/openapi/controllers/context_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/src/kiara_plugin/service/openapi/controllers/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/src/kiara_plugin/service/openapi/controllers/modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     8986 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/src/kiara_plugin/service/openapi/controllers/operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/src/kiara_plugin/service/openapi/controllers/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/src/kiara_plugin/service/openapi/controllers/render.py
--rw-r--r--   0 runner    (1001) docker     (123)    10337 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/src/kiara_plugin/service/openapi/controllers/values.py
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/src/kiara_plugin/service/openapi/controllers/workflows.py
--rw-r--r--   0 runner    (1001) docker     (123)    10579 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/src/kiara_plugin/service/openapi/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:13:20.509764 kiara_plugin.service-0.4.6/src/kiara_plugin/service/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/src/kiara_plugin/service/pipelines/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/src/kiara_plugin/service/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/src/kiara_plugin/service/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:13:20.509764 kiara_plugin.service-0.4.6/src/kiara_plugin/service/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/src/kiara_plugin/service/resources/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:13:20.509764 kiara_plugin.service-0.4.6/src/kiara_plugin/service/resources/static/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/src/kiara_plugin/service/resources/static/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/src/kiara_plugin/service/resources/static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/src/kiara_plugin/service/resources/static/input.css
--rw-r--r--   0 runner    (1001) docker     (123)    13783 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/src/kiara_plugin/service/resources/static/main.css
--rw-r--r--   0 runner    (1001) docker     (123)    10877 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/src/kiara_plugin/service/resources/static/simple.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:13:20.509764 kiara_plugin.service-0.4.6/src/kiara_plugin/service/resources/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/src/kiara_plugin/service/resources/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/src/kiara_plugin/service/resources/templates/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:13:20.509764 kiara_plugin.service-0.4.6/src/kiara_plugin/service/resources/templates/jobs/
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/src/kiara_plugin/service/resources/templates/jobs/job_finished.html
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/src/kiara_plugin/service/resources/templates/jobs/job_monitor.html
--rw-r--r--   0 runner    (1001) docker     (123)     8674 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/src/kiara_plugin/service/resources/templates/macros.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:13:20.513764 kiara_plugin.service-0.4.6/src/kiara_plugin/service/resources/templates/operations/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/src/kiara_plugin/service/resources/templates/operations/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/src/kiara_plugin/service/resources/templates/operations/operation_view.html
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/src/kiara_plugin/service/resources/templates/operations/operations.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:13:20.513764 kiara_plugin.service-0.4.6/src/kiara_plugin/service/resources/templates/values/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/src/kiara_plugin/service/resources/templates/values/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:13:20.513764 kiara_plugin.service-0.4.6/src/kiara_plugin/service/resources/templates/values/inputs/
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/src/kiara_plugin/service/resources/templates/values/inputs/base.html
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/src/kiara_plugin/service/resources/templates/values/inputs/base_scalar.html
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/src/kiara_plugin/service/resources/templates/values/inputs/boolean.html
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/src/kiara_plugin/service/resources/templates/values/inputs/generic-scalar.html
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/src/kiara_plugin/service/resources/templates/values/inputs/generic.html
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/src/kiara_plugin/service/resources/templates/values/inputs/table.html
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/src/kiara_plugin/service/resources/templates/values/value_inputs_form.html
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/src/kiara_plugin/service/resources/templates/values/value_select.html
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/src/kiara_plugin/service/resources/templates/values/value_view.html
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/src/kiara_plugin/service/resources/templates/values/values.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:13:20.509764 kiara_plugin.service-0.4.6/src/kiara_plugin.service.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5851 2023-07-14 14:13:20.000000 kiara_plugin.service-0.4.6/src/kiara_plugin.service.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-07-14 14:13:20.000000 kiara_plugin.service-0.4.6/src/kiara_plugin.service.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 14:13:20.000000 kiara_plugin.service-0.4.6/src/kiara_plugin.service.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-14 14:13:20.000000 kiara_plugin.service-0.4.6/src/kiara_plugin.service.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 14:12:53.000000 kiara_plugin.service-0.4.6/src/kiara_plugin.service.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-14 14:13:20.000000 kiara_plugin.service-0.4.6/src/kiara_plugin.service.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-14 14:13:20.000000 kiara_plugin.service-0.4.6/src/kiara_plugin.service.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/tailwind.config.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:13:20.513764 kiara_plugin.service-0.4.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:13:20.513764 kiara_plugin.service-0.4.6/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/tests/resources/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/tests/test_job_descs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      227 2023-07-14 14:12:44.000000 kiara_plugin.service-0.4.6/tests/test_kiara_modules_default.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:29:27.352850 kiara_plugin.service-0.4.7/
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-21 10:28:46.000000 kiara_plugin.service-0.4.7/.cruft.json
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-21 10:28:46.000000 kiara_plugin.service-0.4.7/.envrc.disabled
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-21 10:28:46.000000 kiara_plugin.service-0.4.7/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-21 10:28:46.000000 kiara_plugin.service-0.4.7/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:29:27.308850 kiara_plugin.service-0.4.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:29:27.328850 kiara_plugin.service-0.4.7/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-21 10:28:46.000000 kiara_plugin.service-0.4.7/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-21 10:28:46.000000 kiara_plugin.service-0.4.7/.github/ISSUE_TEMPLATE/suggest-a-module.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:29:27.328850 kiara_plugin.service-0.4.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-21 10:28:46.000000 kiara_plugin.service-0.4.7/.github/workflows/build-darwin.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     7492 2023-07-21 10:28:46.000000 kiara_plugin.service-0.4.7/.github/workflows/build-linux.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-21 10:28:46.000000 kiara_plugin.service-0.4.7/.github/workflows/build-windows.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-07-21 10:28:46.000000 kiara_plugin.service-0.4.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-07-21 10:28:46.000000 kiara_plugin.service-0.4.7/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-21 10:28:46.000000 kiara_plugin.service-0.4.7/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-21 10:28:46.000000 kiara_plugin.service-0.4.7/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-07-21 10:28:46.000000 kiara_plugin.service-0.4.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-21 10:28:46.000000 kiara_plugin.service-0.4.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-07-21 10:28:46.000000 kiara_plugin.service-0.4.7/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     5845 2023-07-21 10:29:27.352850 kiara_plugin.service-0.4.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-07-21 10:28:46.000000 kiara_plugin.service-0.4.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:29:27.312850 kiara_plugin.service-0.4.7/ci/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:29:27.328850 kiara_plugin.service-0.4.7/ci/conda/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-21 10:28:46.000000 kiara_plugin.service-0.4.7/ci/conda/conda-pkg-patch.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:29:27.328850 kiara_plugin.service-0.4.7/ci/conda/kiara_plugin.service/
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-07-21 10:28:46.000000 kiara_plugin.service-0.4.7/ci/conda/kiara_plugin.service/meta.yaml.template
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-21 10:28:46.000000 kiara_plugin.service-0.4.7/commitlint.config.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:29:27.328850 kiara_plugin.service-0.4.7/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-21 10:28:46.000000 kiara_plugin.service-0.4.7/docs/SUMMARY.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-07-21 10:28:46.000000 kiara_plugin.service-0.4.7/docs/development.md
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-07-21 10:28:46.000000 kiara_plugin.service-0.4.7/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:29:27.328850 kiara_plugin.service-0.4.7/docs/stylesheets/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-21 10:28:46.000000 kiara_plugin.service-0.4.7/docs/stylesheets/extra.css
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-21 10:28:46.000000 kiara_plugin.service-0.4.7/docs/usage.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:29:27.312850 kiara_plugin.service-0.4.7/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:29:27.328850 kiara_plugin.service-0.4.7/examples/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-21 10:28:46.000000 kiara_plugin.service-0.4.7/examples/data/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:29:27.328850 kiara_plugin.service-0.4.7/examples/data/journals/
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-07-21 10:28:46.000000 kiara_plugin.service-0.4.7/examples/data/journals/JournalEdges1902.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    33121 2023-07-21 10:28:46.000000 kiara_plugin.service-0.4.7/examples/data/journals/JournalNodes1902.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-21 10:28:46.000000 kiara_plugin.service-0.4.7/examples/data/journals/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:29:27.328850 kiara_plugin.service-0.4.7/examples/jobs/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-21 10:28:46.000000 kiara_plugin.service-0.4.7/examples/jobs/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:29:27.328850 kiara_plugin.service-0.4.7/examples/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-21 10:28:46.000000 kiara_plugin.service-0.4.7/examples/pipelines/Readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-21 10:28:46.000000 kiara_plugin.service-0.4.7/examples/pipelines/example_pipeline_service.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)   171640 2023-07-21 10:28:46.000000 kiara_plugin.service-0.4.7/kiara_import.profile
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-07-21 10:28:46.000000 kiara_plugin.service-0.4.7/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3829 2023-07-21 10:28:46.000000 kiara_plugin.service-0.4.7/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:29:27.312850 kiara_plugin.service-0.4.7/scripts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:29:27.332850 kiara_plugin.service-0.4.7/scripts/documentation/
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-21 10:28:46.000000 kiara_plugin.service-0.4.7/scripts/documentation/gen_api_doc_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-07-21 10:28:46.000000 kiara_plugin.service-0.4.7/scripts/documentation/gen_info_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-07-21 10:28:46.000000 kiara_plugin.service-0.4.7/scripts/documentation/gen_module_doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-07-21 10:29:27.352850 kiara_plugin.service-0.4.7/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1393 2023-07-21 10:28:46.000000 kiara_plugin.service-0.4.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:29:27.312850 kiara_plugin.service-0.4.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:29:27.312850 kiara_plugin.service-0.4.7/src/kiara_plugin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:29:27.336850 kiara_plugin.service-0.4.7/src/kiara_plugin/service/
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-07-21 10:28:46.000000 kiara_plugin.service-0.4.7/src/kiara_plugin/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-21 10:28:46.000000 kiara_plugin.service-0.4.7/src/kiara_plugin/service/data_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-21 10:28:46.000000 kiara_plugin.service-0.4.7/src/kiara_plugin/service/defaults.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:29:27.336850 kiara_plugin.service-0.4.7/src/kiara_plugin/service/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 10:28:46.000000 kiara_plugin.service-0.4.7/src/kiara_plugin/service/interfaces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:29:27.336850 kiara_plugin.service-0.4.7/src/kiara_plugin/service/interfaces/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 10:28:46.000000 kiara_plugin.service-0.4.7/src/kiara_plugin/service/interfaces/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:29:27.336850 kiara_plugin.service-0.4.7/src/kiara_plugin/service/interfaces/cli/service/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 10:28:46.000000 kiara_plugin.service-0.4.7/src/kiara_plugin/service/interfaces/cli/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-07-21 10:28:46.000000 kiara_plugin.service-0.4.7/src/kiara_plugin/service/interfaces/cli/service/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-07-21 10:28:46.000000 kiara_plugin.service-0.4.7/src/kiara_plugin/service/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:29:27.336850 kiara_plugin.service-0.4.7/src/kiara_plugin/service/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-07-21 10:28:46.000000 kiara_plugin.service-0.4.7/src/kiara_plugin/service/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:29:27.336850 kiara_plugin.service-0.4.7/src/kiara_plugin/service/openapi/
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-07-21 10:28:46.000000 kiara_plugin.service-0.4.7/src/kiara_plugin/service/openapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:29:27.340850 kiara_plugin.service-0.4.7/src/kiara_plugin/service/openapi/controllers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-21 10:28:46.000000 kiara_plugin.service-0.4.7/src/kiara_plugin/service/openapi/controllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-07-21 10:28:46.000000 kiara_plugin.service-0.4.7/src/kiara_plugin/service/openapi/controllers/context_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-07-21 10:28:46.000000 kiara_plugin.service-0.4.7/src/kiara_plugin/service/openapi/controllers/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-21 10:28:46.000000 kiara_plugin.service-0.4.7/src/kiara_plugin/service/openapi/controllers/modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8986 2023-07-21 10:28:46.000000 kiara_plugin.service-0.4.7/src/kiara_plugin/service/openapi/controllers/operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-07-21 10:28:46.000000 kiara_plugin.service-0.4.7/src/kiara_plugin/service/openapi/controllers/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-07-21 10:28:46.000000 kiara_plugin.service-0.4.7/src/kiara_plugin/service/openapi/controllers/render.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10337 2023-07-21 10:28:46.000000 kiara_plugin.service-0.4.7/src/kiara_plugin/service/openapi/controllers/values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-07-21 10:28:46.000000 kiara_plugin.service-0.4.7/src/kiara_plugin/service/openapi/controllers/workflows.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10579 2023-07-21 10:28:46.000000 kiara_plugin.service-0.4.7/src/kiara_plugin/service/openapi/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:29:27.340850 kiara_plugin.service-0.4.7/src/kiara_plugin/service/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 10:28:46.000000 kiara_plugin.service-0.4.7/src/kiara_plugin/service/pipelines/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-21 10:28:46.000000 kiara_plugin.service-0.4.7/src/kiara_plugin/service/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 10:28:46.000000 kiara_plugin.service-0.4.7/src/kiara_plugin/service/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:29:27.340850 kiara_plugin.service-0.4.7/src/kiara_plugin/service/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 10:28:46.000000 kiara_plugin.service-0.4.7/src/kiara_plugin/service/resources/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:29:27.344850 kiara_plugin.service-0.4.7/src/kiara_plugin/service/resources/static/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-21 10:28:46.000000 kiara_plugin.service-0.4.7/src/kiara_plugin/service/resources/static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-21 10:28:46.000000 kiara_plugin.service-0.4.7/src/kiara_plugin/service/resources/static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-21 10:28:46.000000 kiara_plugin.service-0.4.7/src/kiara_plugin/service/resources/static/input.css
+-rw-r--r--   0 runner    (1001) docker     (123)    13783 2023-07-21 10:28:46.000000 kiara_plugin.service-0.4.7/src/kiara_plugin/service/resources/static/main.css
+-rw-r--r--   0 runner    (1001) docker     (123)    10877 2023-07-21 10:28:46.000000 kiara_plugin.service-0.4.7/src/kiara_plugin/service/resources/static/simple.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:29:27.344850 kiara_plugin.service-0.4.7/src/kiara_plugin/service/resources/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-21 10:28:46.000000 kiara_plugin.service-0.4.7/src/kiara_plugin/service/resources/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-21 10:28:46.000000 kiara_plugin.service-0.4.7/src/kiara_plugin/service/resources/templates/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:29:27.344850 kiara_plugin.service-0.4.7/src/kiara_plugin/service/resources/templates/jobs/
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-21 10:28:46.000000 kiara_plugin.service-0.4.7/src/kiara_plugin/service/resources/templates/jobs/job_finished.html
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-21 10:28:46.000000 kiara_plugin.service-0.4.7/src/kiara_plugin/service/resources/templates/jobs/job_monitor.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8674 2023-07-21 10:28:46.000000 kiara_plugin.service-0.4.7/src/kiara_plugin/service/resources/templates/macros.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:29:27.348850 kiara_plugin.service-0.4.7/src/kiara_plugin/service/resources/templates/operations/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-21 10:28:46.000000 kiara_plugin.service-0.4.7/src/kiara_plugin/service/resources/templates/operations/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-21 10:28:46.000000 kiara_plugin.service-0.4.7/src/kiara_plugin/service/resources/templates/operations/operation_view.html
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-21 10:28:46.000000 kiara_plugin.service-0.4.7/src/kiara_plugin/service/resources/templates/operations/operations.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:29:27.348850 kiara_plugin.service-0.4.7/src/kiara_plugin/service/resources/templates/values/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-21 10:28:46.000000 kiara_plugin.service-0.4.7/src/kiara_plugin/service/resources/templates/values/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:29:27.348850 kiara_plugin.service-0.4.7/src/kiara_plugin/service/resources/templates/values/inputs/
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-21 10:28:46.000000 kiara_plugin.service-0.4.7/src/kiara_plugin/service/resources/templates/values/inputs/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-21 10:28:46.000000 kiara_plugin.service-0.4.7/src/kiara_plugin/service/resources/templates/values/inputs/base_scalar.html
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-21 10:28:46.000000 kiara_plugin.service-0.4.7/src/kiara_plugin/service/resources/templates/values/inputs/boolean.html
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-21 10:28:46.000000 kiara_plugin.service-0.4.7/src/kiara_plugin/service/resources/templates/values/inputs/generic-scalar.html
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-21 10:28:46.000000 kiara_plugin.service-0.4.7/src/kiara_plugin/service/resources/templates/values/inputs/generic.html
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-21 10:28:46.000000 kiara_plugin.service-0.4.7/src/kiara_plugin/service/resources/templates/values/inputs/table.html
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-21 10:28:46.000000 kiara_plugin.service-0.4.7/src/kiara_plugin/service/resources/templates/values/value_inputs_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-21 10:28:46.000000 kiara_plugin.service-0.4.7/src/kiara_plugin/service/resources/templates/values/value_select.html
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-21 10:28:46.000000 kiara_plugin.service-0.4.7/src/kiara_plugin/service/resources/templates/values/value_view.html
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-21 10:28:46.000000 kiara_plugin.service-0.4.7/src/kiara_plugin/service/resources/templates/values/values.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:29:27.332850 kiara_plugin.service-0.4.7/src/kiara_plugin.service.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5845 2023-07-21 10:29:27.000000 kiara_plugin.service-0.4.7/src/kiara_plugin.service.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-07-21 10:29:27.000000 kiara_plugin.service-0.4.7/src/kiara_plugin.service.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 10:29:27.000000 kiara_plugin.service-0.4.7/src/kiara_plugin.service.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-21 10:29:27.000000 kiara_plugin.service-0.4.7/src/kiara_plugin.service.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 10:28:56.000000 kiara_plugin.service-0.4.7/src/kiara_plugin.service.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-21 10:29:27.000000 kiara_plugin.service-0.4.7/src/kiara_plugin.service.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-21 10:29:27.000000 kiara_plugin.service-0.4.7/src/kiara_plugin.service.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-21 10:28:46.000000 kiara_plugin.service-0.4.7/tailwind.config.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:29:27.352850 kiara_plugin.service-0.4.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-07-21 10:28:46.000000 kiara_plugin.service-0.4.7/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:29:27.352850 kiara_plugin.service-0.4.7/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 10:28:46.000000 kiara_plugin.service-0.4.7/tests/resources/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-07-21 10:28:46.000000 kiara_plugin.service-0.4.7/tests/test_job_descs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      227 2023-07-21 10:28:46.000000 kiara_plugin.service-0.4.7/tests/test_kiara_modules_default.py
```

### Comparing `kiara_plugin.service-0.4.6/.cruft.json` & `kiara_plugin.service-0.4.7/.cruft.json`

 * *Files 23% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'commit'": "'8a773724c6c0b1b6df826fcda971c185f25234c8'"}*

```diff
@@ -1,10 +1,10 @@
 {
     "checkout": null,
-    "commit": "878ca1dc79be3cd9dd7e4ee9edfa2e5d0789aad7",
+    "commit": "8a773724c6c0b1b6df826fcda971c185f25234c8",
     "context": {
         "cookiecutter": {
             "_template": "https://github.com/DHARPA-Project/kiara_plugin.develop.git",
             "anaconda_user": "dharpa",
             "email": "markus@frkl.io",
             "full_name": "Markus Binsteiner",
             "github_user": "DHARPA-Project",
```

### Comparing `kiara_plugin.service-0.4.6/.github/ISSUE_TEMPLATE/bug_report.md` & `kiara_plugin.service-0.4.7/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.6/.github/ISSUE_TEMPLATE/suggest-a-module.md` & `kiara_plugin.service-0.4.7/.github/ISSUE_TEMPLATE/suggest-a-module.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.6/.github/workflows/build-darwin.yaml` & `kiara_plugin.service-0.4.7/.github/workflows/build-darwin.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.6/.github/workflows/build-linux.yaml` & `kiara_plugin.service-0.4.7/.github/workflows/build-linux.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -148,15 +148,15 @@
         run: python -m build
       - name: upload source package
         run: curl -F package=@$(ls dist/kiara*.tar.gz) https://${GEMFURY_PUSH_TOKEN}@dharpa.fury.land:443/pypi/
       - name: upload wheel
         run: curl -F package=@$(ls dist/kiara*.whl) https://${GEMFURY_PUSH_TOKEN}@dharpa.fury.land:443/pypi/
       - name: publish to PyPI
         if: startsWith(github.ref, 'refs/tags')
-        uses: pypa/gh-action-pypi-publish@master
+        uses: pypa/gh-action-pypi-publish@release/v1
         with:
           user: __token__
           password: "${{ secrets.PYPI_API_TOKEN }}"
 
   conda_package_build:
     name: conda package build (and upload if release)
     runs-on: ubuntu-latest
```

### Comparing `kiara_plugin.service-0.4.6/.github/workflows/build-windows.yaml` & `kiara_plugin.service-0.4.7/.github/workflows/build-windows.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.6/.gitignore` & `kiara_plugin.service-0.4.7/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -59,7 +59,9 @@
 .frkl
 .envrc
 build.sh
 onefile.spec
 *_complete.zsh.zwc
 ci/conda/**/build
 ci/conda/kiara_plugin.service/meta.yaml
+.pixi
+dev.py
```

### Comparing `kiara_plugin.service-0.4.6/.pre-commit-config.yaml` & `kiara_plugin.service-0.4.7/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     files: "^src/"
     pass_filenames: true
     args: ["--config-file", "setup.cfg", "--ignore-missing-imports", "--explicit-package-bases"]
     additional_dependencies: [pydantic>=1.8.0, rich>=10.0.0, ruamel.yaml, anyio>=3.0.0, pyzmq>=22.0.3, bidict, sqlalchemy-stubs, types-python-slugify, types-setuptools, types-python-dateutil, dag_cbor, multiformats, textual, regex, types-pytz, types-orjson]
 
 - repo: https://github.com/charliermarsh/ruff-pre-commit
   # Ruff version.
-  rev: 'v0.0.243'
+  rev: 'v0.0.272'
   hooks:
     - id: ruff
 
 - repo: https://github.com/Kludex/no-optional
   rev: 0.4.0
   hooks:
     - id: no_optional
```

### Comparing `kiara_plugin.service-0.4.6/LICENSE` & `kiara_plugin.service-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.6/Makefile` & `kiara_plugin.service-0.4.7/Makefile`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.6/PKG-INFO` & `kiara_plugin.service-0.4.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: kiara_plugin.service
-Version: 0.4.6
+Version: 0.4.7
 Summary: A plugin to create, run and manage a service for kiara functionality.
 Author-email: Markus Binsteiner <markus@frkl.io>
 License: MPL-2.0
 Project-URL: homepage, https://github.com/DHARPA-Project/kiara_plugin.service
 Project-URL: documentation, https://DHARPA-Project.github.io/kiara_plugin.service
 Project-URL: repository, https://github.com/DHARPA-Project/kiara_plugin.service
 Keywords: kiara
-Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
@@ -23,14 +22,15 @@
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: all_dev
 Provides-Extra: dev_all
 Provides-Extra: dev_documentation
 Provides-Extra: dev_testing
 Provides-Extra: dev_utils
+Provides-Extra: streamlit
 License-File: LICENSE
 License-File: AUTHORS.md
 
 [![PyPI status](https://img.shields.io/pypi/status/kiara_plugin.service.svg)](https://pypi.python.org/pypi/kiara_plugin.service/)
 [![PyPI version](https://img.shields.io/pypi/v/kiara_plugin.service.svg)](https://pypi.python.org/pypi/kiara_plugin.service/)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/kiara_plugin.service.svg)](https://pypi.python.org/pypi/kiara_plugin.service/)
 [![Build Status](https://img.shields.io/endpoint.svg?url=https%3A%2F%2Factions-badge.atrox.dev%2FDHARPA-Project%2Fkiara%2Fbadge%3Fref%3Ddevelop&style=flat)](https://actions-badge.atrox.dev/DHARPA-Project/kiara_plugin.service/goto?ref=develop)
```

### Comparing `kiara_plugin.service-0.4.6/README.md` & `kiara_plugin.service-0.4.7/README.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.6/ci/conda/kiara_plugin.service/meta.yaml.template` & `kiara_plugin.service-0.4.7/ci/conda/kiara_plugin.service/meta.yaml.template`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.6/docs/development.md` & `kiara_plugin.service-0.4.7/docs/development.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.6/docs/index.md` & `kiara_plugin.service-0.4.7/docs/index.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.6/examples/data/journals/JournalEdges1902.csv` & `kiara_plugin.service-0.4.7/examples/data/journals/JournalEdges1902.csv`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.6/examples/data/journals/JournalNodes1902.csv` & `kiara_plugin.service-0.4.7/examples/data/journals/JournalNodes1902.csv`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.6/examples/pipelines/example_pipeline_service.yaml` & `kiara_plugin.service-0.4.7/examples/pipelines/example_pipeline_service.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.6/kiara_import.profile` & `kiara_plugin.service-0.4.7/kiara_import.profile`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.6/mkdocs.yml` & `kiara_plugin.service-0.4.7/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.6/pyproject.toml` & `kiara_plugin.service-0.4.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -13,28 +13,27 @@
     {name = "Markus Binsteiner", email = "markus@frkl.io"}
 ]
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = ["kiara"]
 license = {text = "MPL-2.0"}
 classifiers = [
-    "Framework :: Django",
     "Programming Language :: Python :: 3",
     "Development Status :: 3 - Alpha",
     "License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11"
 ]
 dependencies = [
-    "kiara>=0.4.47",
+    "kiara>=0.4.49",
     "kiara_plugin.core_types>=0.4.20",
     "uvicorn>=0.22.0",
     "starlite==1.39.0",
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
@@ -46,14 +45,17 @@
 ]
 dev_utils = [
     "kiara[dev_utils]",
 ]
 dev_all = [
     "kiara[dev_all]"
 ]
+streamlit = [
+    "kiara_plugin.streamlit"
+]
 
 [project.entry-points."kiara.plugin"]
 service = "kiara_plugin.service"
 
 [project.entry-points."kiara.cli_subcommands"]
 service = "kiara_plugin.service.interfaces.cli.service.commands:service"
```

### Comparing `kiara_plugin.service-0.4.6/scripts/documentation/gen_api_doc_pages.py` & `kiara_plugin.service-0.4.7/scripts/documentation/gen_api_doc_pages.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.6/scripts/documentation/gen_info_pages.py` & `kiara_plugin.service-0.4.7/scripts/documentation/gen_info_pages.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.6/scripts/documentation/gen_module_doc.py` & `kiara_plugin.service-0.4.7/scripts/documentation/gen_module_doc.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.6/setup.cfg` & `kiara_plugin.service-0.4.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.6/setup.py` & `kiara_plugin.service-0.4.7/setup.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.6/src/kiara_plugin/service/__init__.py` & `kiara_plugin.service-0.4.7/src/kiara_plugin/service/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.6/src/kiara_plugin/service/defaults.py` & `kiara_plugin.service-0.4.7/src/kiara_plugin/service/defaults.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.6/src/kiara_plugin/service/interfaces/cli/service/commands.py` & `kiara_plugin.service-0.4.7/src/kiara_plugin/service/interfaces/cli/service/commands.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,14 +35,15 @@
         import uvloop
 
         uvloop.install()
     except Exception:
         pass
 
     kiara_api: KiaraAPI = ctx.obj.kiara_api
+
     kiara_service = KiaraOpenAPIService(kiara_api=kiara_api)
     import uvicorn
 
     app = kiara_service.app()
     config = uvicorn.Config(app=app, host=host, port=port, log_level="info")
     server = uvicorn.Server(config=config)
     server.run()
```

### Comparing `kiara_plugin.service-0.4.6/src/kiara_plugin/service/models.py` & `kiara_plugin.service-0.4.7/src/kiara_plugin/service/models.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.6/src/kiara_plugin/service/modules/__init__.py` & `kiara_plugin.service-0.4.7/src/kiara_plugin/service/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.6/src/kiara_plugin/service/openapi/__init__.py` & `kiara_plugin.service-0.4.7/src/kiara_plugin/service/openapi/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.6/src/kiara_plugin/service/openapi/controllers/__init__.py` & `kiara_plugin.service-0.4.7/src/kiara_plugin/service/openapi/controllers/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.6/src/kiara_plugin/service/openapi/controllers/context_info.py` & `kiara_plugin.service-0.4.7/src/kiara_plugin/service/openapi/controllers/context_info.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.6/src/kiara_plugin/service/openapi/controllers/jobs.py` & `kiara_plugin.service-0.4.7/src/kiara_plugin/service/openapi/controllers/jobs.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.6/src/kiara_plugin/service/openapi/controllers/modules.py` & `kiara_plugin.service-0.4.7/src/kiara_plugin/service/openapi/controllers/modules.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.6/src/kiara_plugin/service/openapi/controllers/operations.py` & `kiara_plugin.service-0.4.7/src/kiara_plugin/service/openapi/controllers/operations.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.6/src/kiara_plugin/service/openapi/controllers/pipeline.py` & `kiara_plugin.service-0.4.7/src/kiara_plugin/service/openapi/controllers/pipeline.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,21 +22,20 @@
     path = "/"
 
     @get(path="/structure/{pipeline:str}", api_func=get_pipeline_config)
     async def get_pipeline_structure(
         self, kiara_api: KiaraAPI, pipeline: str
     ) -> PipelineStructureInfo:
 
-        print(f"PIPELINE: {pipeline}")
-        pipeline_config = get_pipeline_config(pipeline=pipeline)
-        print(pipeline_config)
+        pipeline_config = get_pipeline_config(
+            pipeline=pipeline, kiara=kiara_api.context
+        )
         info = PipelineStructureInfo.create_from_instance(
             kiara=kiara_api.context, instance=pipeline_config.structure
         )
         return info
 
     @get(path="/list", api_func=get_pipeline_config)
     async def list_pipelines(self, kiara_api: KiaraAPI) -> List[str]:
 
         pipelines = kiara_api.list_operations(operation_types="pipeline")
-        print(pipelines)
         return list(pipelines.keys())
```

### Comparing `kiara_plugin.service-0.4.6/src/kiara_plugin/service/openapi/controllers/render.py` & `kiara_plugin.service-0.4.7/src/kiara_plugin/service/openapi/controllers/render.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.6/src/kiara_plugin/service/openapi/controllers/values.py` & `kiara_plugin.service-0.4.7/src/kiara_plugin/service/openapi/controllers/values.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.6/src/kiara_plugin/service/openapi/controllers/workflows.py` & `kiara_plugin.service-0.4.7/src/kiara_plugin/service/openapi/controllers/workflows.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.6/src/kiara_plugin/service/openapi/service.py` & `kiara_plugin.service-0.4.7/src/kiara_plugin/service/openapi/service.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.6/src/kiara_plugin/service/resources/static/favicon.ico` & `kiara_plugin.service-0.4.7/src/kiara_plugin/service/resources/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.6/src/kiara_plugin/service/resources/static/main.css` & `kiara_plugin.service-0.4.7/src/kiara_plugin/service/resources/static/main.css`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.6/src/kiara_plugin/service/resources/static/simple.css` & `kiara_plugin.service-0.4.7/src/kiara_plugin/service/resources/static/simple.css`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.6/src/kiara_plugin/service/resources/templates/jobs/job_finished.html` & `kiara_plugin.service-0.4.7/src/kiara_plugin/service/resources/templates/jobs/job_finished.html`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.6/src/kiara_plugin/service/resources/templates/macros.html` & `kiara_plugin.service-0.4.7/src/kiara_plugin/service/resources/templates/macros.html`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.6/src/kiara_plugin/service/resources/templates/values/inputs/base_scalar.html` & `kiara_plugin.service-0.4.7/src/kiara_plugin/service/resources/templates/values/inputs/base_scalar.html`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.6/src/kiara_plugin.service.egg-info/PKG-INFO` & `kiara_plugin.service-0.4.7/src/kiara_plugin.service.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: kiara-plugin.service
-Version: 0.4.6
+Version: 0.4.7
 Summary: A plugin to create, run and manage a service for kiara functionality.
 Author-email: Markus Binsteiner <markus@frkl.io>
 License: MPL-2.0
 Project-URL: homepage, https://github.com/DHARPA-Project/kiara_plugin.service
 Project-URL: documentation, https://DHARPA-Project.github.io/kiara_plugin.service
 Project-URL: repository, https://github.com/DHARPA-Project/kiara_plugin.service
 Keywords: kiara
-Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
@@ -23,14 +22,15 @@
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: all_dev
 Provides-Extra: dev_all
 Provides-Extra: dev_documentation
 Provides-Extra: dev_testing
 Provides-Extra: dev_utils
+Provides-Extra: streamlit
 License-File: LICENSE
 License-File: AUTHORS.md
 
 [![PyPI status](https://img.shields.io/pypi/status/kiara_plugin.service.svg)](https://pypi.python.org/pypi/kiara_plugin.service/)
 [![PyPI version](https://img.shields.io/pypi/v/kiara_plugin.service.svg)](https://pypi.python.org/pypi/kiara_plugin.service/)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/kiara_plugin.service.svg)](https://pypi.python.org/pypi/kiara_plugin.service/)
 [![Build Status](https://img.shields.io/endpoint.svg?url=https%3A%2F%2Factions-badge.atrox.dev%2FDHARPA-Project%2Fkiara%2Fbadge%3Fref%3Ddevelop&style=flat)](https://actions-badge.atrox.dev/DHARPA-Project/kiara_plugin.service/goto?ref=develop)
```

### Comparing `kiara_plugin.service-0.4.6/src/kiara_plugin.service.egg-info/SOURCES.txt` & `kiara_plugin.service-0.4.7/src/kiara_plugin.service.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.6/tests/conftest.py` & `kiara_plugin.service-0.4.7/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.6/tests/test_job_descs.py` & `kiara_plugin.service-0.4.7/tests/test_job_descs.py`

 * *Files identical despite different names*

