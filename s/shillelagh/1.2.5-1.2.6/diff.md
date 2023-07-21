# Comparing `tmp/shillelagh-1.2.5.tar.gz` & `tmp/shillelagh-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shillelagh-1.2.5.tar", last modified: Fri Jul 14 22:08:44 2023, max compression
+gzip compressed data, was "shillelagh-1.2.6.tar", last modified: Fri Jul 21 01:41:24 2023, max compression
```

## Comparing `shillelagh-1.2.5.tar` & `shillelagh-1.2.6.tar`

### file list

```diff
@@ -1,201 +1,201 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:44.977698 shillelagh-1.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-07-14 22:08:32.000000 shillelagh-1.2.5/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-14 22:08:32.000000 shillelagh-1.2.5/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:44.961698 shillelagh-1.2.5/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-14 22:08:32.000000 shillelagh-1.2.5/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:44.961698 shillelagh-1.2.5/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-14 22:08:32.000000 shillelagh-1.2.5/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-14 22:08:32.000000 shillelagh-1.2.5/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-14 22:08:32.000000 shillelagh-1.2.5/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-07-14 22:08:32.000000 shillelagh-1.2.5/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:44.961698 shillelagh-1.2.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-07-14 22:08:32.000000 shillelagh-1.2.5/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-07-14 22:08:32.000000 shillelagh-1.2.5/.github/workflows/python-integration.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-14 22:08:32.000000 shillelagh-1.2.5/.github/workflows/python-package-daily.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-07-14 22:08:32.000000 shillelagh-1.2.5/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-14 22:08:32.000000 shillelagh-1.2.5/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-07-14 22:08:32.000000 shillelagh-1.2.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-14 22:08:32.000000 shillelagh-1.2.5/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-07-14 22:08:32.000000 shillelagh-1.2.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-14 22:08:32.000000 shillelagh-1.2.5/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-14 22:08:32.000000 shillelagh-1.2.5/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)    13954 2023-07-14 22:08:32.000000 shillelagh-1.2.5/ARCHITECTURE.rst
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-14 22:08:32.000000 shillelagh-1.2.5/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8712 2023-07-14 22:08:32.000000 shillelagh-1.2.5/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5223 2023-07-14 22:08:32.000000 shillelagh-1.2.5/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-07-14 22:08:32.000000 shillelagh-1.2.5/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-14 22:08:32.000000 shillelagh-1.2.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-07-14 22:08:32.000000 shillelagh-1.2.5/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     9934 2023-07-14 22:08:44.977698 shillelagh-1.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7573 2023-07-14 22:08:32.000000 shillelagh-1.2.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:44.961698 shillelagh-1.2.5/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-07-14 22:08:32.000000 shillelagh-1.2.5/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:44.961698 shillelagh-1.2.5/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-14 22:08:32.000000 shillelagh-1.2.5/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    18000 2023-07-14 22:08:32.000000 shillelagh-1.2.5/docs/adapters.rst
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-14 22:08:32.000000 shillelagh-1.2.5/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-14 22:08:32.000000 shillelagh-1.2.5/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9479 2023-07-14 22:08:32.000000 shillelagh-1.2.5/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    32853 2023-07-14 22:08:32.000000 shillelagh-1.2.5/docs/development.rst
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-14 22:08:32.000000 shillelagh-1.2.5/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-07-14 22:08:32.000000 shillelagh-1.2.5/docs/install.rst
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-14 22:08:32.000000 shillelagh-1.2.5/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-14 22:08:32.000000 shillelagh-1.2.5/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7428 2023-07-14 22:08:32.000000 shillelagh-1.2.5/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:44.961698 shillelagh-1.2.5/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-14 22:08:32.000000 shillelagh-1.2.5/examples/csvfile.py
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-14 22:08:32.000000 shillelagh-1.2.5/examples/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-07-14 22:08:32.000000 shillelagh-1.2.5/examples/datasette.py
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-07-14 22:08:32.000000 shillelagh-1.2.5/examples/generic_json.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-14 22:08:32.000000 shillelagh-1.2.5/examples/github.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-14 22:08:32.000000 shillelagh-1.2.5/examples/gsheets.py
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-07-14 22:08:32.000000 shillelagh-1.2.5/examples/socrata.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-14 22:08:32.000000 shillelagh-1.2.5/examples/test.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-07-14 22:08:32.000000 shillelagh-1.2.5/examples/weatherapi.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-14 22:08:32.000000 shillelagh-1.2.5/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-14 22:08:32.000000 shillelagh-1.2.5/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:44.961698 shillelagh-1.2.5/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-14 22:08:32.000000 shillelagh-1.2.5/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-14 22:08:32.000000 shillelagh-1.2.5/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-14 22:08:32.000000 shillelagh-1.2.5/requirements/test.in
--rw-r--r--   0 runner    (1001) docker     (123)     4052 2023-07-14 22:08:32.000000 shillelagh-1.2.5/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4337 2023-07-14 22:08:44.977698 shillelagh-1.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-14 22:08:32.000000 shillelagh-1.2.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:44.953698 shillelagh-1.2.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:44.965698 shillelagh-1.2.5/src/shillelagh/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:32.000000 shillelagh-1.2.5/src/shillelagh/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:44.965698 shillelagh-1.2.5/src/shillelagh/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:32.000000 shillelagh-1.2.5/src/shillelagh/adapters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:44.965698 shillelagh-1.2.5/src/shillelagh/adapters/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:32.000000 shillelagh-1.2.5/src/shillelagh/adapters/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-07-14 22:08:32.000000 shillelagh-1.2.5/src/shillelagh/adapters/api/datasette.py
--rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-07-14 22:08:32.000000 shillelagh-1.2.5/src/shillelagh/adapters/api/generic_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     7494 2023-07-14 22:08:32.000000 shillelagh-1.2.5/src/shillelagh/adapters/api/github.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:44.965698 shillelagh-1.2.5/src/shillelagh/adapters/api/gsheets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:32.000000 shillelagh-1.2.5/src/shillelagh/adapters/api/gsheets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26713 2023-07-14 22:08:32.000000 shillelagh-1.2.5/src/shillelagh/adapters/api/gsheets/adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8982 2023-07-14 22:08:32.000000 shillelagh-1.2.5/src/shillelagh/adapters/api/gsheets/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     8159 2023-07-14 22:08:32.000000 shillelagh-1.2.5/src/shillelagh/adapters/api/gsheets/lib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:44.965698 shillelagh-1.2.5/src/shillelagh/adapters/api/gsheets/parsing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:32.000000 shillelagh-1.2.5/src/shillelagh/adapters/api/gsheets/parsing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-07-14 22:08:32.000000 shillelagh-1.2.5/src/shillelagh/adapters/api/gsheets/parsing/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    16029 2023-07-14 22:08:32.000000 shillelagh-1.2.5/src/shillelagh/adapters/api/gsheets/parsing/date.py
--rw-r--r--   0 runner    (1001) docker     (123)    18376 2023-07-14 22:08:32.000000 shillelagh-1.2.5/src/shillelagh/adapters/api/gsheets/parsing/number.py
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-07-14 22:08:32.000000 shillelagh-1.2.5/src/shillelagh/adapters/api/gsheets/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-07-14 22:08:32.000000 shillelagh-1.2.5/src/shillelagh/adapters/api/gsheets/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-07-14 22:08:32.000000 shillelagh-1.2.5/src/shillelagh/adapters/api/html_table.py
--rw-r--r--   0 runner    (1001) docker     (123)    10603 2023-07-14 22:08:32.000000 shillelagh-1.2.5/src/shillelagh/adapters/api/s3select.py
--rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-07-14 22:08:32.000000 shillelagh-1.2.5/src/shillelagh/adapters/api/socrata.py
--rw-r--r--   0 runner    (1001) docker     (123)     7216 2023-07-14 22:08:32.000000 shillelagh-1.2.5/src/shillelagh/adapters/api/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     7461 2023-07-14 22:08:32.000000 shillelagh-1.2.5/src/shillelagh/adapters/api/weatherapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     8499 2023-07-14 22:08:32.000000 shillelagh-1.2.5/src/shillelagh/adapters/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:44.965698 shillelagh-1.2.5/src/shillelagh/adapters/file/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:32.000000 shillelagh-1.2.5/src/shillelagh/adapters/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10267 2023-07-14 22:08:32.000000 shillelagh-1.2.5/src/shillelagh/adapters/file/csvfile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:44.965698 shillelagh-1.2.5/src/shillelagh/adapters/memory/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:32.000000 shillelagh-1.2.5/src/shillelagh/adapters/memory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6047 2023-07-14 22:08:32.000000 shillelagh-1.2.5/src/shillelagh/adapters/memory/pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-07-14 22:08:32.000000 shillelagh-1.2.5/src/shillelagh/adapters/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:44.965698 shillelagh-1.2.5/src/shillelagh/backends/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:32.000000 shillelagh-1.2.5/src/shillelagh/backends/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:44.969698 shillelagh-1.2.5/src/shillelagh/backends/apsw/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:32.000000 shillelagh-1.2.5/src/shillelagh/backends/apsw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16401 2023-07-14 22:08:32.000000 shillelagh-1.2.5/src/shillelagh/backends/apsw/db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:44.969698 shillelagh-1.2.5/src/shillelagh/backends/apsw/dialects/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:32.000000 shillelagh-1.2.5/src/shillelagh/backends/apsw/dialects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-07-14 22:08:32.000000 shillelagh-1.2.5/src/shillelagh/backends/apsw/dialects/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7407 2023-07-14 22:08:32.000000 shillelagh-1.2.5/src/shillelagh/backends/apsw/dialects/gsheets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-07-14 22:08:32.000000 shillelagh-1.2.5/src/shillelagh/backends/apsw/dialects/safe.py
--rw-r--r--   0 runner    (1001) docker     (123)    20167 2023-07-14 22:08:32.000000 shillelagh-1.2.5/src/shillelagh/backends/apsw/vt.py
--rw-r--r--   0 runner    (1001) docker     (123)     6412 2023-07-14 22:08:32.000000 shillelagh-1.2.5/src/shillelagh/console.py
--rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-07-14 22:08:32.000000 shillelagh-1.2.5/src/shillelagh/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    21797 2023-07-14 22:08:32.000000 shillelagh-1.2.5/src/shillelagh/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)    11160 2023-07-14 22:08:32.000000 shillelagh-1.2.5/src/shillelagh/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-07-14 22:08:32.000000 shillelagh-1.2.5/src/shillelagh/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    17700 2023-07-14 22:08:32.000000 shillelagh-1.2.5/src/shillelagh/lib.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:32.000000 shillelagh-1.2.5/src/shillelagh/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-07-14 22:08:32.000000 shillelagh-1.2.5/src/shillelagh/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-07-14 22:08:32.000000 shillelagh-1.2.5/src/shillelagh/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:44.965698 shillelagh-1.2.5/src/shillelagh.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9934 2023-07-14 22:08:44.000000 shillelagh-1.2.5/src/shillelagh.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5196 2023-07-14 22:08:44.000000 shillelagh-1.2.5/src/shillelagh.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 22:08:44.000000 shillelagh-1.2.5/src/shillelagh.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-07-14 22:08:44.000000 shillelagh-1.2.5/src/shillelagh.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 22:08:44.000000 shillelagh-1.2.5/src/shillelagh.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-07-14 22:08:44.000000 shillelagh-1.2.5/src/shillelagh.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-14 22:08:44.000000 shillelagh-1.2.5/src/shillelagh.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:44.969698 shillelagh-1.2.5/talks/
--rw-r--r--   0 runner    (1001) docker     (123)  2331376 2023-07-14 22:08:32.000000 shillelagh-1.2.5/talks/Python Brasil 2021.pdf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:44.957698 shillelagh-1.2.5/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:44.969698 shillelagh-1.2.5/templates/adapter/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-14 22:08:32.000000 shillelagh-1.2.5/templates/adapter/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:44.969698 shillelagh-1.2.5/templates/adapter/hooks/
--rwxr-xr-x   0 runner    (1001) docker     (123)      267 2023-07-14 22:08:32.000000 shillelagh-1.2.5/templates/adapter/hooks/post_gen_project.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:44.969698 shillelagh-1.2.5/templates/adapter/{{cookiecutter.slug}}/
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-07-14 22:08:32.000000 shillelagh-1.2.5/templates/adapter/{{cookiecutter.slug}}/test_{{cookiecutter.slug}}.py
--rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-07-14 22:08:32.000000 shillelagh-1.2.5/templates/adapter/{{cookiecutter.slug}}/{{cookiecutter.slug}}.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:44.969698 shillelagh-1.2.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:32.000000 shillelagh-1.2.5/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:44.973698 shillelagh-1.2.5/tests/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:32.000000 shillelagh-1.2.5/tests/adapters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:44.973698 shillelagh-1.2.5/tests/adapters/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:32.000000 shillelagh-1.2.5/tests/adapters/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14353 2023-07-14 22:08:32.000000 shillelagh-1.2.5/tests/adapters/api/datasette_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7721 2023-07-14 22:08:32.000000 shillelagh-1.2.5/tests/adapters/api/generic_json_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    18505 2023-07-14 22:08:32.000000 shillelagh-1.2.5/tests/adapters/api/github_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:44.973698 shillelagh-1.2.5/tests/adapters/api/gsheets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:32.000000 shillelagh-1.2.5/tests/adapters/api/gsheets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    73731 2023-07-14 22:08:32.000000 shillelagh-1.2.5/tests/adapters/api/gsheets/adapter_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5300 2023-07-14 22:08:32.000000 shillelagh-1.2.5/tests/adapters/api/gsheets/fields_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    20327 2023-07-14 22:08:32.000000 shillelagh-1.2.5/tests/adapters/api/gsheets/integration_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9270 2023-07-14 22:08:32.000000 shillelagh-1.2.5/tests/adapters/api/gsheets/lib_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:44.973698 shillelagh-1.2.5/tests/adapters/api/gsheets/parsing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:32.000000 shillelagh-1.2.5/tests/adapters/api/gsheets/parsing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-07-14 22:08:32.000000 shillelagh-1.2.5/tests/adapters/api/gsheets/parsing/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    20013 2023-07-14 22:08:32.000000 shillelagh-1.2.5/tests/adapters/api/gsheets/parsing/date_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    14492 2023-07-14 22:08:32.000000 shillelagh-1.2.5/tests/adapters/api/gsheets/parsing/number_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-07-14 22:08:32.000000 shillelagh-1.2.5/tests/adapters/api/html_table_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7107 2023-07-14 22:08:32.000000 shillelagh-1.2.5/tests/adapters/api/s3select_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8515 2023-07-14 22:08:32.000000 shillelagh-1.2.5/tests/adapters/api/socrata_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9566 2023-07-14 22:08:32.000000 shillelagh-1.2.5/tests/adapters/api/system_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    17776 2023-07-14 22:08:32.000000 shillelagh-1.2.5/tests/adapters/api/weatherapi_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9512 2023-07-14 22:08:32.000000 shillelagh-1.2.5/tests/adapters/base_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:44.973698 shillelagh-1.2.5/tests/adapters/file/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:32.000000 shillelagh-1.2.5/tests/adapters/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11856 2023-07-14 22:08:32.000000 shillelagh-1.2.5/tests/adapters/file/csvfile_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:44.973698 shillelagh-1.2.5/tests/adapters/memory/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:32.000000 shillelagh-1.2.5/tests/adapters/memory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9285 2023-07-14 22:08:32.000000 shillelagh-1.2.5/tests/adapters/memory/pandas_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-07-14 22:08:32.000000 shillelagh-1.2.5/tests/adapters/registry_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:44.973698 shillelagh-1.2.5/tests/backends/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:32.000000 shillelagh-1.2.5/tests/backends/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:44.973698 shillelagh-1.2.5/tests/backends/apsw/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:32.000000 shillelagh-1.2.5/tests/backends/apsw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14748 2023-07-14 22:08:32.000000 shillelagh-1.2.5/tests/backends/apsw/db_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-07-14 22:08:32.000000 shillelagh-1.2.5/tests/backends/apsw/dbapi_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:44.973698 shillelagh-1.2.5/tests/backends/apsw/dialects/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:32.000000 shillelagh-1.2.5/tests/backends/apsw/dialects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-07-14 22:08:32.000000 shillelagh-1.2.5/tests/backends/apsw/dialects/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    15699 2023-07-14 22:08:32.000000 shillelagh-1.2.5/tests/backends/apsw/dialects/gsheets_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-14 22:08:32.000000 shillelagh-1.2.5/tests/backends/apsw/dialects/safe_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    16148 2023-07-14 22:08:32.000000 shillelagh-1.2.5/tests/backends/apsw/vt_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-07-14 22:08:32.000000 shillelagh-1.2.5/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5655 2023-07-14 22:08:32.000000 shillelagh-1.2.5/tests/console_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:44.977698 shillelagh-1.2.5/tests/fakes/
--rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-07-14 22:08:32.000000 shillelagh-1.2.5/tests/fakes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   400535 2023-07-14 22:08:32.000000 shillelagh-1.2.5/tests/fakes/cdc_data_response.json
--rw-r--r--   0 runner    (1001) docker     (123)   121689 2023-07-14 22:08:32.000000 shillelagh-1.2.5/tests/fakes/cdc_metadata_response.json
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-07-14 22:08:32.000000 shillelagh-1.2.5/tests/fakes/datasette_columns_response.json
--rw-r--r--   0 runner    (1001) docker     (123)   369983 2023-07-14 22:08:32.000000 shillelagh-1.2.5/tests/fakes/datasette_data_response_1.json
--rw-r--r--   0 runner    (1001) docker     (123)    60078 2023-07-14 22:08:32.000000 shillelagh-1.2.5/tests/fakes/datasette_data_response_2.json
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-07-14 22:08:32.000000 shillelagh-1.2.5/tests/fakes/datasette_metadata_response.json
--rw-r--r--   0 runner    (1001) docker     (123)   428142 2023-07-14 22:08:32.000000 shillelagh-1.2.5/tests/fakes/datasette_results.json
--rw-r--r--   0 runner    (1001) docker     (123)   220647 2023-07-14 22:08:32.000000 shillelagh-1.2.5/tests/fakes/github_response.json
--rw-r--r--   0 runner    (1001) docker     (123)    18818 2023-07-14 22:08:32.000000 shillelagh-1.2.5/tests/fakes/github_single_response.json
--rw-r--r--   0 runner    (1001) docker     (123)   165205 2023-07-14 22:08:32.000000 shillelagh-1.2.5/tests/fakes/incidents.json
--rw-r--r--   0 runner    (1001) docker     (123)    40785 2023-07-14 22:08:32.000000 shillelagh-1.2.5/tests/fakes/weatherapi_response.json
--rw-r--r--   0 runner    (1001) docker     (123)    13821 2023-07-14 22:08:32.000000 shillelagh-1.2.5/tests/fields_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9127 2023-07-14 22:08:32.000000 shillelagh-1.2.5/tests/filters_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-07-14 22:08:32.000000 shillelagh-1.2.5/tests/functions_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    13791 2023-07-14 22:08:32.000000 shillelagh-1.2.5/tests/lib_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-14 22:08:32.000000 shillelagh-1.2.5/tests/types_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:41:24.164822 shillelagh-1.2.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-07-21 01:41:12.000000 shillelagh-1.2.6/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-21 01:41:12.000000 shillelagh-1.2.6/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:41:24.148822 shillelagh-1.2.6/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-21 01:41:12.000000 shillelagh-1.2.6/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:41:24.148822 shillelagh-1.2.6/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-21 01:41:12.000000 shillelagh-1.2.6/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-21 01:41:12.000000 shillelagh-1.2.6/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-21 01:41:12.000000 shillelagh-1.2.6/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-07-21 01:41:12.000000 shillelagh-1.2.6/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:41:24.148822 shillelagh-1.2.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-07-21 01:41:12.000000 shillelagh-1.2.6/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-07-21 01:41:12.000000 shillelagh-1.2.6/.github/workflows/python-integration.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-21 01:41:12.000000 shillelagh-1.2.6/.github/workflows/python-package-daily.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-07-21 01:41:12.000000 shillelagh-1.2.6/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-21 01:41:12.000000 shillelagh-1.2.6/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-07-21 01:41:12.000000 shillelagh-1.2.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-21 01:41:12.000000 shillelagh-1.2.6/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-07-21 01:41:12.000000 shillelagh-1.2.6/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-21 01:41:12.000000 shillelagh-1.2.6/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-21 01:41:12.000000 shillelagh-1.2.6/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    13954 2023-07-21 01:41:12.000000 shillelagh-1.2.6/ARCHITECTURE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-21 01:41:12.000000 shillelagh-1.2.6/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8829 2023-07-21 01:41:12.000000 shillelagh-1.2.6/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5223 2023-07-21 01:41:12.000000 shillelagh-1.2.6/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-07-21 01:41:12.000000 shillelagh-1.2.6/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-21 01:41:12.000000 shillelagh-1.2.6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-07-21 01:41:12.000000 shillelagh-1.2.6/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     9934 2023-07-21 01:41:24.168822 shillelagh-1.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7573 2023-07-21 01:41:12.000000 shillelagh-1.2.6/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:41:24.152822 shillelagh-1.2.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-07-21 01:41:12.000000 shillelagh-1.2.6/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:41:24.152822 shillelagh-1.2.6/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-21 01:41:12.000000 shillelagh-1.2.6/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    18000 2023-07-21 01:41:12.000000 shillelagh-1.2.6/docs/adapters.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-21 01:41:12.000000 shillelagh-1.2.6/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-21 01:41:12.000000 shillelagh-1.2.6/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9479 2023-07-21 01:41:12.000000 shillelagh-1.2.6/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32853 2023-07-21 01:41:12.000000 shillelagh-1.2.6/docs/development.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-21 01:41:12.000000 shillelagh-1.2.6/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-07-21 01:41:12.000000 shillelagh-1.2.6/docs/install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-21 01:41:12.000000 shillelagh-1.2.6/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-21 01:41:12.000000 shillelagh-1.2.6/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7428 2023-07-21 01:41:12.000000 shillelagh-1.2.6/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:41:24.152822 shillelagh-1.2.6/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-21 01:41:12.000000 shillelagh-1.2.6/examples/csvfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-21 01:41:12.000000 shillelagh-1.2.6/examples/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-07-21 01:41:12.000000 shillelagh-1.2.6/examples/datasette.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-07-21 01:41:12.000000 shillelagh-1.2.6/examples/generic_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-21 01:41:12.000000 shillelagh-1.2.6/examples/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-21 01:41:12.000000 shillelagh-1.2.6/examples/gsheets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-07-21 01:41:12.000000 shillelagh-1.2.6/examples/socrata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-21 01:41:12.000000 shillelagh-1.2.6/examples/test.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-07-21 01:41:12.000000 shillelagh-1.2.6/examples/weatherapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-21 01:41:12.000000 shillelagh-1.2.6/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-21 01:41:12.000000 shillelagh-1.2.6/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:41:24.152822 shillelagh-1.2.6/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-21 01:41:12.000000 shillelagh-1.2.6/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-21 01:41:12.000000 shillelagh-1.2.6/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-21 01:41:12.000000 shillelagh-1.2.6/requirements/test.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4052 2023-07-21 01:41:12.000000 shillelagh-1.2.6/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4337 2023-07-21 01:41:24.168822 shillelagh-1.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-21 01:41:12.000000 shillelagh-1.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:41:24.136823 shillelagh-1.2.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:41:24.152822 shillelagh-1.2.6/src/shillelagh/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 01:41:12.000000 shillelagh-1.2.6/src/shillelagh/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:41:24.156822 shillelagh-1.2.6/src/shillelagh/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 01:41:12.000000 shillelagh-1.2.6/src/shillelagh/adapters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:41:24.156822 shillelagh-1.2.6/src/shillelagh/adapters/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 01:41:12.000000 shillelagh-1.2.6/src/shillelagh/adapters/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-07-21 01:41:12.000000 shillelagh-1.2.6/src/shillelagh/adapters/api/datasette.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-07-21 01:41:12.000000 shillelagh-1.2.6/src/shillelagh/adapters/api/generic_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7494 2023-07-21 01:41:12.000000 shillelagh-1.2.6/src/shillelagh/adapters/api/github.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:41:24.156822 shillelagh-1.2.6/src/shillelagh/adapters/api/gsheets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 01:41:12.000000 shillelagh-1.2.6/src/shillelagh/adapters/api/gsheets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26712 2023-07-21 01:41:12.000000 shillelagh-1.2.6/src/shillelagh/adapters/api/gsheets/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10314 2023-07-21 01:41:12.000000 shillelagh-1.2.6/src/shillelagh/adapters/api/gsheets/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8363 2023-07-21 01:41:12.000000 shillelagh-1.2.6/src/shillelagh/adapters/api/gsheets/lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:41:24.156822 shillelagh-1.2.6/src/shillelagh/adapters/api/gsheets/parsing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 01:41:12.000000 shillelagh-1.2.6/src/shillelagh/adapters/api/gsheets/parsing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4116 2023-07-21 01:41:12.000000 shillelagh-1.2.6/src/shillelagh/adapters/api/gsheets/parsing/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19127 2023-07-21 01:41:12.000000 shillelagh-1.2.6/src/shillelagh/adapters/api/gsheets/parsing/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18376 2023-07-21 01:41:12.000000 shillelagh-1.2.6/src/shillelagh/adapters/api/gsheets/parsing/number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-07-21 01:41:12.000000 shillelagh-1.2.6/src/shillelagh/adapters/api/gsheets/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-07-21 01:41:12.000000 shillelagh-1.2.6/src/shillelagh/adapters/api/gsheets/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-07-21 01:41:12.000000 shillelagh-1.2.6/src/shillelagh/adapters/api/html_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10603 2023-07-21 01:41:12.000000 shillelagh-1.2.6/src/shillelagh/adapters/api/s3select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-07-21 01:41:12.000000 shillelagh-1.2.6/src/shillelagh/adapters/api/socrata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7216 2023-07-21 01:41:12.000000 shillelagh-1.2.6/src/shillelagh/adapters/api/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7461 2023-07-21 01:41:12.000000 shillelagh-1.2.6/src/shillelagh/adapters/api/weatherapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8499 2023-07-21 01:41:12.000000 shillelagh-1.2.6/src/shillelagh/adapters/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:41:24.156822 shillelagh-1.2.6/src/shillelagh/adapters/file/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 01:41:12.000000 shillelagh-1.2.6/src/shillelagh/adapters/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10346 2023-07-21 01:41:12.000000 shillelagh-1.2.6/src/shillelagh/adapters/file/csvfile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:41:24.156822 shillelagh-1.2.6/src/shillelagh/adapters/memory/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 01:41:12.000000 shillelagh-1.2.6/src/shillelagh/adapters/memory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6047 2023-07-21 01:41:12.000000 shillelagh-1.2.6/src/shillelagh/adapters/memory/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-07-21 01:41:12.000000 shillelagh-1.2.6/src/shillelagh/adapters/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:41:24.156822 shillelagh-1.2.6/src/shillelagh/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 01:41:12.000000 shillelagh-1.2.6/src/shillelagh/backends/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:41:24.156822 shillelagh-1.2.6/src/shillelagh/backends/apsw/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 01:41:12.000000 shillelagh-1.2.6/src/shillelagh/backends/apsw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16401 2023-07-21 01:41:12.000000 shillelagh-1.2.6/src/shillelagh/backends/apsw/db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:41:24.156822 shillelagh-1.2.6/src/shillelagh/backends/apsw/dialects/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 01:41:12.000000 shillelagh-1.2.6/src/shillelagh/backends/apsw/dialects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-07-21 01:41:12.000000 shillelagh-1.2.6/src/shillelagh/backends/apsw/dialects/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7407 2023-07-21 01:41:12.000000 shillelagh-1.2.6/src/shillelagh/backends/apsw/dialects/gsheets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-07-21 01:41:12.000000 shillelagh-1.2.6/src/shillelagh/backends/apsw/dialects/safe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20167 2023-07-21 01:41:12.000000 shillelagh-1.2.6/src/shillelagh/backends/apsw/vt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6412 2023-07-21 01:41:12.000000 shillelagh-1.2.6/src/shillelagh/console.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-07-21 01:41:12.000000 shillelagh-1.2.6/src/shillelagh/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21797 2023-07-21 01:41:12.000000 shillelagh-1.2.6/src/shillelagh/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11160 2023-07-21 01:41:12.000000 shillelagh-1.2.6/src/shillelagh/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-07-21 01:41:12.000000 shillelagh-1.2.6/src/shillelagh/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17700 2023-07-21 01:41:12.000000 shillelagh-1.2.6/src/shillelagh/lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 01:41:12.000000 shillelagh-1.2.6/src/shillelagh/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-07-21 01:41:12.000000 shillelagh-1.2.6/src/shillelagh/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-07-21 01:41:12.000000 shillelagh-1.2.6/src/shillelagh/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:41:24.156822 shillelagh-1.2.6/src/shillelagh.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9934 2023-07-21 01:41:23.000000 shillelagh-1.2.6/src/shillelagh.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5196 2023-07-21 01:41:24.000000 shillelagh-1.2.6/src/shillelagh.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 01:41:23.000000 shillelagh-1.2.6/src/shillelagh.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-07-21 01:41:23.000000 shillelagh-1.2.6/src/shillelagh.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 01:41:23.000000 shillelagh-1.2.6/src/shillelagh.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-07-21 01:41:23.000000 shillelagh-1.2.6/src/shillelagh.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-21 01:41:23.000000 shillelagh-1.2.6/src/shillelagh.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:41:24.156822 shillelagh-1.2.6/talks/
+-rw-r--r--   0 runner    (1001) docker     (123)  2331376 2023-07-21 01:41:12.000000 shillelagh-1.2.6/talks/Python Brasil 2021.pdf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:41:24.140823 shillelagh-1.2.6/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:41:24.160822 shillelagh-1.2.6/templates/adapter/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-21 01:41:12.000000 shillelagh-1.2.6/templates/adapter/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:41:24.160822 shillelagh-1.2.6/templates/adapter/hooks/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      267 2023-07-21 01:41:12.000000 shillelagh-1.2.6/templates/adapter/hooks/post_gen_project.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:41:24.160822 shillelagh-1.2.6/templates/adapter/{{cookiecutter.slug}}/
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-07-21 01:41:12.000000 shillelagh-1.2.6/templates/adapter/{{cookiecutter.slug}}/test_{{cookiecutter.slug}}.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-07-21 01:41:12.000000 shillelagh-1.2.6/templates/adapter/{{cookiecutter.slug}}/{{cookiecutter.slug}}.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:41:24.160822 shillelagh-1.2.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 01:41:12.000000 shillelagh-1.2.6/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:41:24.160822 shillelagh-1.2.6/tests/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 01:41:12.000000 shillelagh-1.2.6/tests/adapters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:41:24.160822 shillelagh-1.2.6/tests/adapters/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 01:41:12.000000 shillelagh-1.2.6/tests/adapters/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14353 2023-07-21 01:41:12.000000 shillelagh-1.2.6/tests/adapters/api/datasette_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7721 2023-07-21 01:41:12.000000 shillelagh-1.2.6/tests/adapters/api/generic_json_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18505 2023-07-21 01:41:12.000000 shillelagh-1.2.6/tests/adapters/api/github_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:41:24.160822 shillelagh-1.2.6/tests/adapters/api/gsheets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 01:41:12.000000 shillelagh-1.2.6/tests/adapters/api/gsheets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73771 2023-07-21 01:41:12.000000 shillelagh-1.2.6/tests/adapters/api/gsheets/adapter_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-07-21 01:41:12.000000 shillelagh-1.2.6/tests/adapters/api/gsheets/fields_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20327 2023-07-21 01:41:12.000000 shillelagh-1.2.6/tests/adapters/api/gsheets/integration_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9488 2023-07-21 01:41:12.000000 shillelagh-1.2.6/tests/adapters/api/gsheets/lib_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:41:24.164822 shillelagh-1.2.6/tests/adapters/api/gsheets/parsing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 01:41:12.000000 shillelagh-1.2.6/tests/adapters/api/gsheets/parsing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-07-21 01:41:12.000000 shillelagh-1.2.6/tests/adapters/api/gsheets/parsing/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21594 2023-07-21 01:41:12.000000 shillelagh-1.2.6/tests/adapters/api/gsheets/parsing/date_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14588 2023-07-21 01:41:12.000000 shillelagh-1.2.6/tests/adapters/api/gsheets/parsing/number_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-07-21 01:41:12.000000 shillelagh-1.2.6/tests/adapters/api/html_table_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7107 2023-07-21 01:41:12.000000 shillelagh-1.2.6/tests/adapters/api/s3select_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8515 2023-07-21 01:41:12.000000 shillelagh-1.2.6/tests/adapters/api/socrata_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9566 2023-07-21 01:41:12.000000 shillelagh-1.2.6/tests/adapters/api/system_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17776 2023-07-21 01:41:12.000000 shillelagh-1.2.6/tests/adapters/api/weatherapi_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9512 2023-07-21 01:41:12.000000 shillelagh-1.2.6/tests/adapters/base_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:41:24.164822 shillelagh-1.2.6/tests/adapters/file/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 01:41:12.000000 shillelagh-1.2.6/tests/adapters/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12222 2023-07-21 01:41:12.000000 shillelagh-1.2.6/tests/adapters/file/csvfile_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:41:24.164822 shillelagh-1.2.6/tests/adapters/memory/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 01:41:12.000000 shillelagh-1.2.6/tests/adapters/memory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9285 2023-07-21 01:41:12.000000 shillelagh-1.2.6/tests/adapters/memory/pandas_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-07-21 01:41:12.000000 shillelagh-1.2.6/tests/adapters/registry_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:41:24.164822 shillelagh-1.2.6/tests/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 01:41:12.000000 shillelagh-1.2.6/tests/backends/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:41:24.164822 shillelagh-1.2.6/tests/backends/apsw/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 01:41:12.000000 shillelagh-1.2.6/tests/backends/apsw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14748 2023-07-21 01:41:12.000000 shillelagh-1.2.6/tests/backends/apsw/db_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-07-21 01:41:12.000000 shillelagh-1.2.6/tests/backends/apsw/dbapi_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:41:24.164822 shillelagh-1.2.6/tests/backends/apsw/dialects/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 01:41:12.000000 shillelagh-1.2.6/tests/backends/apsw/dialects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-07-21 01:41:12.000000 shillelagh-1.2.6/tests/backends/apsw/dialects/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15699 2023-07-21 01:41:12.000000 shillelagh-1.2.6/tests/backends/apsw/dialects/gsheets_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-21 01:41:12.000000 shillelagh-1.2.6/tests/backends/apsw/dialects/safe_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16148 2023-07-21 01:41:12.000000 shillelagh-1.2.6/tests/backends/apsw/vt_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-07-21 01:41:12.000000 shillelagh-1.2.6/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5655 2023-07-21 01:41:12.000000 shillelagh-1.2.6/tests/console_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:41:24.164822 shillelagh-1.2.6/tests/fakes/
+-rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-07-21 01:41:12.000000 shillelagh-1.2.6/tests/fakes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   400535 2023-07-21 01:41:12.000000 shillelagh-1.2.6/tests/fakes/cdc_data_response.json
+-rw-r--r--   0 runner    (1001) docker     (123)   121689 2023-07-21 01:41:12.000000 shillelagh-1.2.6/tests/fakes/cdc_metadata_response.json
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-07-21 01:41:12.000000 shillelagh-1.2.6/tests/fakes/datasette_columns_response.json
+-rw-r--r--   0 runner    (1001) docker     (123)   369983 2023-07-21 01:41:12.000000 shillelagh-1.2.6/tests/fakes/datasette_data_response_1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    60078 2023-07-21 01:41:12.000000 shillelagh-1.2.6/tests/fakes/datasette_data_response_2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-07-21 01:41:12.000000 shillelagh-1.2.6/tests/fakes/datasette_metadata_response.json
+-rw-r--r--   0 runner    (1001) docker     (123)   428142 2023-07-21 01:41:12.000000 shillelagh-1.2.6/tests/fakes/datasette_results.json
+-rw-r--r--   0 runner    (1001) docker     (123)   220647 2023-07-21 01:41:12.000000 shillelagh-1.2.6/tests/fakes/github_response.json
+-rw-r--r--   0 runner    (1001) docker     (123)    18818 2023-07-21 01:41:12.000000 shillelagh-1.2.6/tests/fakes/github_single_response.json
+-rw-r--r--   0 runner    (1001) docker     (123)   165205 2023-07-21 01:41:12.000000 shillelagh-1.2.6/tests/fakes/incidents.json
+-rw-r--r--   0 runner    (1001) docker     (123)    40785 2023-07-21 01:41:12.000000 shillelagh-1.2.6/tests/fakes/weatherapi_response.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13821 2023-07-21 01:41:12.000000 shillelagh-1.2.6/tests/fields_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9127 2023-07-21 01:41:12.000000 shillelagh-1.2.6/tests/filters_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-07-21 01:41:12.000000 shillelagh-1.2.6/tests/functions_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13799 2023-07-21 01:41:12.000000 shillelagh-1.2.6/tests/lib_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-21 01:41:12.000000 shillelagh-1.2.6/tests/types_test.py
```

### Comparing `shillelagh-1.2.5/.coveragerc` & `shillelagh-1.2.6/.coveragerc`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.5/.github/ISSUE_TEMPLATE/bug_report.md` & `shillelagh-1.2.6/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.5/.github/ISSUE_TEMPLATE/feature_request.md` & `shillelagh-1.2.6/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.5/.github/pull_request_template.md` & `shillelagh-1.2.6/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.5/.github/workflows/codeql-analysis.yml` & `shillelagh-1.2.6/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.5/.github/workflows/python-integration.yml` & `shillelagh-1.2.6/.github/workflows/python-integration.yml`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.5/.github/workflows/python-package-daily.yml` & `shillelagh-1.2.6/.github/workflows/python-package-daily.yml`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.5/.github/workflows/python-package.yml` & `shillelagh-1.2.6/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.5/.github/workflows/python-publish.yml` & `shillelagh-1.2.6/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.5/.gitignore` & `shillelagh-1.2.6/.gitignore`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.5/.pre-commit-config.yaml` & `shillelagh-1.2.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.5/.readthedocs.yml` & `shillelagh-1.2.6/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.5/ARCHITECTURE.rst` & `shillelagh-1.2.6/ARCHITECTURE.rst`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.5/CHANGELOG.rst` & `shillelagh-1.2.6/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 =========
 Changelog
 =========
 
 Next
 ====
 
+Version 1.2.6 - 2023-07-20
+==========================
+
+- Add support for querying durations in Google Sheets (#374)
+
 Version 1.2.5 - 2023-07-14
 ==========================
 
 - System adapter now supports memory (virtual/swap) queries (#369 and #372)
 
 Version 1.2.4 - 2023-05-15
 ==========================
```

### Comparing `shillelagh-1.2.5/CODE_OF_CONDUCT.md` & `shillelagh-1.2.6/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.5/CONTRIBUTING.rst` & `shillelagh-1.2.6/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.5/LICENSE.txt` & `shillelagh-1.2.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.5/Makefile` & `shillelagh-1.2.6/Makefile`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.5/PKG-INFO` & `shillelagh-1.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shillelagh
-Version: 1.2.5
+Version: 1.2.6
 Summary: Making it easy to query APIs via SQL
 Home-page: https://github.com/betodealmeida/shillelagh/
 Author: Beto Dealmeida
 Author-email: roberto@dealmeida.net
 License: mit
 Project-URL: Documentation, https://shillelagh.readthedocs.io/
 Description: ==========
```

### Comparing `shillelagh-1.2.5/README.rst` & `shillelagh-1.2.6/README.rst`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.5/docs/Makefile` & `shillelagh-1.2.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.5/docs/adapters.rst` & `shillelagh-1.2.6/docs/adapters.rst`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.5/docs/conf.py` & `shillelagh-1.2.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.5/docs/development.rst` & `shillelagh-1.2.6/docs/development.rst`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.5/docs/install.rst` & `shillelagh-1.2.6/docs/install.rst`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.5/docs/usage.rst` & `shillelagh-1.2.6/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.5/examples/csvfile.py` & `shillelagh-1.2.6/examples/csvfile.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.5/examples/dataframe.py` & `shillelagh-1.2.6/examples/dataframe.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.5/examples/datasette.py` & `shillelagh-1.2.6/examples/datasette.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.5/examples/generic_json.py` & `shillelagh-1.2.6/examples/generic_json.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.5/examples/weatherapi.py` & `shillelagh-1.2.6/examples/weatherapi.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.5/requirements/base.txt` & `shillelagh-1.2.6/requirements/base.txt`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.5/requirements/test.txt` & `shillelagh-1.2.6/requirements/test.txt`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.5/setup.cfg` & `shillelagh-1.2.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.5/src/shillelagh/adapters/api/datasette.py` & `shillelagh-1.2.6/src/shillelagh/adapters/api/datasette.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.5/src/shillelagh/adapters/api/generic_json.py` & `shillelagh-1.2.6/src/shillelagh/adapters/api/generic_json.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.5/src/shillelagh/adapters/api/github.py` & `shillelagh-1.2.6/src/shillelagh/adapters/api/github.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.5/src/shillelagh/adapters/api/gsheets/adapter.py` & `shillelagh-1.2.6/src/shillelagh/adapters/api/gsheets/adapter.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,14 @@
 JSON_PAYLOAD_PREFIX = ")]}'\n"
 
 # this is just a wild guess; used to estimate query cost
 AVERAGE_NUMBER_OF_ROWS = 1000
 
 
 class GSheetsAPI(Adapter):  # pylint: disable=too-many-instance-attributes
-
     r"""
     A Google Sheets adapter.
 
     The adapter uses two different APIs. When only ``SELECT``\s are used the
     adapter uses the Google Chart API, which queries in a dialect of SQL.
     The Chart API is efficient because the data can be filterd and sorted
     on the backend before being retrieved.
```

### Comparing `shillelagh-1.2.5/src/shillelagh/adapters/api/gsheets/fields.py` & `shillelagh-1.2.6/src/shillelagh/adapters/api/gsheets/fields.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Custom fields for the GSheets adapter.
 """
 import datetime
-from typing import Any, List, Optional, Type
+from typing import Any, List, Optional, Type, Union
 
 from shillelagh.adapters.api.gsheets.parsing.date import (
     format_date_time_pattern,
     parse_date_time_pattern,
 )
 from shillelagh.adapters.api.gsheets.parsing.number import (
     format_number_pattern,
@@ -16,14 +16,18 @@
 from shillelagh.filters import Filter
 
 # timestamp format used in SQL queries
 DATETIME_SQL_QUOTE = "%Y-%m-%d %H:%M:%S"
 DATE_SQL_QUOTE = "%Y-%m-%d"
 TIME_SQL_QUOTE = "%H:%M:%S"
 
+# When filtering a sheet based on a duration we need to convert it into a datetime
+# starting at 1899-12-30, for some reason. That is not documented anywhere, obviously.
+DURATION_OFFSET = datetime.datetime(1899, 12, 30)
+
 
 class GSheetsField(Field[Internal, External]):
     """
     A base class for GSheets fields.
     """
 
     # the default formats for date and datetime do not follow the same syntax
@@ -202,14 +206,48 @@
         # On SQL queries the timestamp should be prefix by "timeofday"
         value = parse_date_time_pattern(value, self.pattern, datetime.time).strftime(
             TIME_SQL_QUOTE,
         )
         return f"timeofday '{value}'"
 
 
+class GSheetsDuration(GSheetsField[str, datetime.timedelta]):
+    """
+    A GSheets duration.
+    """
+
+    type = "DURATION"
+    db_api_type = "DATETIME"
+
+    def parse(self, value: Optional[str]) -> Optional[datetime.timedelta]:
+        if self.pattern is None or value is None or value == "":
+            return None
+
+        return parse_date_time_pattern(value, self.pattern, datetime.timedelta)
+
+    def format(self, value: Optional[datetime.timedelta]) -> str:
+        # This method is used only when inserting or updating rows, so we
+        # encode NULLs as an empty string to match the Google Sheets API.
+        if self.pattern is None or value is None:
+            return ""
+
+        return format_date_time_pattern(value, self.pattern)
+
+    def quote(self, value: Optional[str]) -> str:
+        if self.pattern is None or value == "" or value is None:
+            return "null"
+
+        timestamp = DURATION_OFFSET + parse_date_time_pattern(
+            value,
+            self.pattern,
+            datetime.timedelta,
+        )
+        return f"datetime '{timestamp}'"
+
+
 class GSheetsBoolean(GSheetsField[str, bool]):
     """
     A GSheets boolean.
 
     Booleans in the Google Chart API are return as a string, either "TRUE"
     of "FALSE".
     """
@@ -264,15 +302,15 @@
             return ""
 
         if self.pattern is None or self.pattern == "General":
             return str(value)
 
         return format_number_pattern(value, self.pattern)
 
-    def quote(self, value: Optional[str]) -> str:
+    def quote(self, value: Optional[Union[str, int, float]]) -> str:
         if value == "" or value is None:
             return "null"
 
         return str(value)
 
 
 class GSheetsString(GSheetsField[str, str]):
```

### Comparing `shillelagh-1.2.5/src/shillelagh/adapters/api/gsheets/lib.py` & `shillelagh-1.2.6/src/shillelagh/adapters/api/gsheets/lib.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,19 +10,21 @@
 import google.oauth2.service_account
 from google.auth.credentials import Credentials
 
 from shillelagh.adapters.api.gsheets.fields import (
     GSheetsBoolean,
     GSheetsDate,
     GSheetsDateTime,
+    GSheetsDuration,
     GSheetsField,
     GSheetsNumber,
     GSheetsString,
     GSheetsTime,
 )
+from shillelagh.adapters.api.gsheets.parsing.date import infer_column_type
 from shillelagh.adapters.api.gsheets.types import SyncMode
 from shillelagh.adapters.api.gsheets.typing import (
     QueryResultsCell,
     QueryResultsColumn,
     QueryResultsError,
     UrlArgs,
 )
@@ -42,26 +44,27 @@
 def get_field(
     col: QueryResultsColumn,
     timezone: Optional[datetime.tzinfo] = None,
 ) -> Field:
     """
     Return a Shillelagh ``Field`` from a Google Chart API results column.
     """
-    # Fix for GSheets return an incorrect type. We should be able to detect the type based
-    # on the pattern, instead of relying on the return type.
-    if col["type"] == "datetime" and col.get("pattern") == "h:mm:ss am/pm":
-        col["type"] = "timeofday"
+    # GSheets returns type ``datetime`` for timestamps, but also for time of day and
+    # durations. We need to tokenize the pattern in order to figure out the correct type.
+    if col["type"] == "datetime" and "pattern" in col:
+        col["type"] = infer_column_type(col["pattern"])
 
     type_map: Dict[str, Tuple[Type[GSheetsField], List[Type[Filter]]]] = {
         "string": (GSheetsString, [Range, Equal, NotEqual, Like, IsNull, IsNotNull]),
         "number": (GSheetsNumber, [Range, Equal, NotEqual, IsNull, IsNotNull]),
         "boolean": (GSheetsBoolean, [Equal, NotEqual, IsNull, IsNotNull]),
         "date": (GSheetsDate, [Range, Equal, NotEqual, IsNull, IsNotNull]),
         "datetime": (GSheetsDateTime, [Range, Equal, NotEqual, IsNull, IsNotNull]),
         "timeofday": (GSheetsTime, [Range, Equal, NotEqual, IsNull, IsNotNull]),
+        "duration": (GSheetsDuration, [Range, Equal, NotEqual, IsNull, IsNotNull]),
     }
     class_, filters = type_map.get(
         col["type"],
         (GSheetsString, [Range, Equal, NotEqual, Like, IsNull, IsNotNull]),
     )
     return class_(
         filters=filters,
```

### Comparing `shillelagh-1.2.5/src/shillelagh/adapters/api/gsheets/parsing/base.py` & `shillelagh-1.2.6/src/shillelagh/adapters/api/gsheets/parsing/base.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,22 +15,30 @@
 
     regex: str
 
     def __init__(self, token: str):
         self.token = token
 
     @classmethod
-    def match(cls, pattern: str) -> bool:
+    def match(
+        cls,
+        pattern: str,
+        history: List["Token"],  # pylint: disable=unused-argument
+    ) -> bool:
         """
         Check if token handles the beginning of the pattern.
         """
         return bool(re.match(cls.regex, pattern))
 
     @classmethod
-    def consume(cls, pattern: str) -> Tuple["Token", str]:
+    def consume(
+        cls,
+        pattern: str,
+        history: List["Token"],  # pylint: disable=unused-argument
+    ) -> Tuple["Token", str]:
         """
         Consume the pattern, returning the token and the remaining pattern.
         """
         match = re.match(cls.regex, pattern)
         if not match:
             # pylint: disable=broad-exception-raised
             raise Exception("Token could not find match")
@@ -95,19 +103,19 @@
         return {}, value[size:]
 
 
 def tokenize(pattern: str, classes: List[Type[Token]]) -> Iterator[Token]:
     """
     Tokenize a pattern.
     """
-    tokens = []
+    tokens: List[Token] = []
     while pattern:
         for class_ in classes:  # pragma: no cover
-            if class_.match(pattern):
-                token, pattern = class_.consume(pattern)
+            if class_.match(pattern, tokens):
+                token, pattern = class_.consume(pattern, tokens)
                 tokens.append(token)
                 break
 
     # combine unescaped literals
     while tokens:
         token = tokens.pop(0)
         if is_unescaped_literal(token):
```

### Comparing `shillelagh-1.2.5/src/shillelagh/adapters/api/gsheets/parsing/date.py` & `shillelagh-1.2.6/src/shillelagh/adapters/api/gsheets/parsing/date.py`

 * *Files 15% similar despite different names*

```diff
@@ -242,59 +242,118 @@
     def format(self, value: Union[datetime, time], tokens: List[Token]) -> str:
         return super().format(value, tokens).zfill(2)
 
     def parse(self, value: str, tokens: List[Token]) -> Tuple[Dict[str, Any], str]:
         return {"second": int(value[:2])}, value[2:]
 
 
-class HPlusDuration(Token):
+class DurationToken(Token):  # pylint: disable=abstract-method
+    """
+    A token for durations.
+
+    Durations are special because often only the first token is annotated. For example:
+
+        - [h]:mm:ss
+        - [ss].000
+
+    But apparently it is valid to annotate subsequent tokens:
+
+        - [hh]:[mm]:[ss].000
+
+    Who knows?
+
+    Because of this, their regexes are dynamic, and depend on the token history.
+    """
+
+    is_duration = True
+    regexes: Tuple[str, str]
+
+    @classmethod
+    def match(
+        cls,
+        pattern: str,
+        history: List[Token],
+    ) -> bool:
+        if any(isinstance(token, DurationToken) for token in history):
+            regex = cls.regexes[1]
+        else:
+            regex = cls.regexes[0]
+
+        return bool(re.match(regex, pattern))
+
+    @classmethod
+    def consume(
+        cls,
+        pattern: str,
+        history: List[Token],
+    ) -> Tuple[Token, str]:
+        if any(isinstance(token, DurationToken) for token in history):
+            regex = cls.regexes[1]
+        else:
+            regex = cls.regexes[0]
+
+        match = re.match(regex, pattern)
+        if not match:
+            # pylint: disable=broad-exception-raised
+            raise Exception("Token could not find match")
+        token = match.group()
+        return cls(token), pattern[len(token) :]
+
+
+class HPlusDuration(DurationToken):
     """
     Number of elapsed hours in a time duration. Number of letters indicates
     minimum number of digits (adds leading 0s).
     """
 
-    regex = r"\[h+\]"
+    regexes = (r"\[h+\]", r"(h+)|(\[h+\])")
 
     def format(self, value: Union[timedelta], tokens: List[Token]) -> str:
         return str(int(value.total_seconds() // 3600)).zfill(len(self.token) - 2)
 
     def parse(self, value: str, tokens: List[Token]) -> Tuple[Dict[str, Any], str]:
-        size = len(self.token) - 2
+        match = re.match(r"\d+", value)
+        if not match:
+            raise Exception(f"Cannot parse value: {value}")
+        size = len(match.group())
         return {"hours": int(value[:size])}, value[size:]
 
 
-class MPlusDuration(Token):
+class MPlusDuration(DurationToken):
     """
     Number of elapsed minutes in a time duration. Number of letters indicates
     minimum number of digits (adds leading 0s).
     """
 
-    regex = r"\[m+\]"
+    regexes = (r"\[m+\]", r"(m+)|(\[m+\])")
 
     def format(self, value: Union[timedelta], tokens: List[Token]) -> str:
         seconds = value.total_seconds()
 
         if any(token.__class__.__name__ == "HPlusDuration" for token in tokens):
             # ignore hours
             seconds %= 3600
 
         return str(int(seconds // 60)).zfill(len(self.token) - 2)
 
     def parse(self, value: str, tokens: List[Token]) -> Tuple[Dict[str, Any], str]:
-        size = len(self.token) - 2
+        match = re.match(r"\d+", value)
+        if not match:
+            raise Exception(f"Cannot parse value: {value}")
+        size = len(match.group())
         return {"minutes": int(value[:size])}, value[size:]
 
 
-class SPlusDuration(Token):
+class SPlusDuration(DurationToken):
     """
     Number of elapsed seconds in a time duration. Number of letters indicates
     minimum number of digits (adds leading 0s).
     """
 
-    regex = r"\[s+\]"
+    regexes = (r"\[s+\]", r"(s+)|(\[s+\])")
 
     def format(self, value: Union[timedelta], tokens: List[Token]) -> str:
         seconds = value.total_seconds()
 
         if any(token.__class__.__name__ == "HPlusDuration" for token in tokens):
             # ignore hours
             seconds %= 3600
@@ -302,15 +361,18 @@
         if any(token.__class__.__name__ == "MPlusDuration" for token in tokens):
             # ignore minutes
             seconds %= 60
 
         return str(int(seconds)).zfill(len(self.token) - 2)
 
     def parse(self, value: str, tokens: List[Token]) -> Tuple[Dict[str, Any], str]:
-        size = len(self.token) - 2
+        match = re.match(r"\d+", value)
+        if not match:
+            raise Exception(f"Cannot parse value: {value}")
+        size = len(match.group())
         return {"seconds": int(value[:size])}, value[size:]
 
 
 class D(Token):
     """
     Day of the month, no leading 0 for numbers less than 10.
     """
@@ -466,37 +528,87 @@
 
     def parse(self, value: str, tokens: List[Token]) -> Tuple[Dict[str, Any], str]:
         letter = value[:2]
         meridiem = Meridiem.PM if letter.upper() == "PM" else Meridiem.AM
         return {"meridiem": meridiem}, value[2:]
 
 
+def infer_column_type(pattern: str) -> str:
+    """
+    Infer the correct date-related type.
+
+    GSheets returns ``datetime`` as the type for timestamps, but also for time of day and
+    durations. We need to parse the pattern to figure out the exact type.
+    """
+    classes = [
+        # durations should come first because they need to be modified
+        # after the first capture
+        HPlusDuration,
+        MPlusDuration,
+        SPlusDuration,
+        # then the rest
+        H,
+        HHPlus,
+        M,
+        MM,
+        MMM,
+        MMMM,
+        MMMMM,
+        S,
+        SS,
+        D,
+        DD,
+        DDD,
+        DDDDPlus,
+        YY,
+        YYYY,
+        AP,
+        AMPM,
+        ZERO,
+        LITERAL,
+    ]
+
+    tokens = list(tokenize(pattern, classes))
+
+    if any(isinstance(token, DurationToken) for token in tokens):
+        return "duration"
+
+    datetime_tokens = (D, DD, DDD, DDDDPlus, YY, YYYY)
+    if any(isinstance(token, datetime_tokens) for token in tokens):
+        return "datetime"
+
+    return "timeofday"
+
+
 def parse_date_time_pattern(
     value: str,
     pattern: str,
     class_: Type[DateTime],
 ) -> DateTime:
     """
     Parse a value using a given pattern.
 
     See https://developers.google.com/sheets/api/guides/formats?hl=en.
     """
     classes = [
+        # durations should come first because they need to be modified
+        # after the first capture
+        HPlusDuration,
+        MPlusDuration,
+        SPlusDuration,
+        # then the rest
         H,
         HHPlus,
         M,
         MM,
         MMM,
         MMMM,
         MMMMM,
         S,
         SS,
-        HPlusDuration,
-        MPlusDuration,
-        SPlusDuration,
         D,
         DD,
         DDD,
         DDDDPlus,
         YY,
         YYYY,
         AP,
@@ -535,26 +647,29 @@
 def format_date_time_pattern(value: DateTime, pattern: str) -> str:
     """
     Format a date/time related object to a given pattern.
 
     See https://developers.google.com/sheets/api/guides/formats?hl=en.
     """
     classes = [
+        # durations should come first because they need to be modified
+        # after the first capture
+        HPlusDuration,
+        MPlusDuration,
+        SPlusDuration,
+        # then the rest
         H,
         HHPlus,
         M,
         MM,
         MMM,
         MMMM,
         MMMMM,
         S,
         SS,
-        HPlusDuration,
-        MPlusDuration,
-        SPlusDuration,
         D,
         DD,
         DDD,
         DDDDPlus,
         YY,
         YYYY,
         AP,
```

### Comparing `shillelagh-1.2.5/src/shillelagh/adapters/api/gsheets/parsing/number.py` & `shillelagh-1.2.6/src/shillelagh/adapters/api/gsheets/parsing/number.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.5/src/shillelagh/adapters/api/gsheets/types.py` & `shillelagh-1.2.6/src/shillelagh/adapters/api/gsheets/types.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.5/src/shillelagh/adapters/api/gsheets/typing.py` & `shillelagh-1.2.6/src/shillelagh/adapters/api/gsheets/typing.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.5/src/shillelagh/adapters/api/html_table.py` & `shillelagh-1.2.6/src/shillelagh/adapters/api/html_table.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.5/src/shillelagh/adapters/api/s3select.py` & `shillelagh-1.2.6/src/shillelagh/adapters/api/s3select.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.5/src/shillelagh/adapters/api/socrata.py` & `shillelagh-1.2.6/src/shillelagh/adapters/api/socrata.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.5/src/shillelagh/adapters/api/system.py` & `shillelagh-1.2.6/src/shillelagh/adapters/api/system.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.5/src/shillelagh/adapters/api/weatherapi.py` & `shillelagh-1.2.6/src/shillelagh/adapters/api/weatherapi.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.5/src/shillelagh/adapters/base.py` & `shillelagh-1.2.6/src/shillelagh/adapters/base.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.5/src/shillelagh/adapters/file/csvfile.py` & `shillelagh-1.2.6/src/shillelagh/adapters/file/csvfile.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,14 @@
             yield row
 
     def __next__(self) -> Row:
         return self.iterable.__next__()
 
 
 class CSVFile(Adapter):
-
     r"""
     An adapter for CSV files.
 
     The files must be written with the ``QUOTE_NONNUMERIC`` format option, with
     strings explicitly quoted::
 
         "index","temperature","site"
@@ -273,15 +272,18 @@
     def close(self) -> None:
         """
         Garbage collect the file.
 
         This method will get rid of deleted rows in the files.
         """
         if not self.local:
-            self.path.unlink()
+            try:
+                self.path.unlink()
+            except FileNotFoundError:
+                pass
             return
 
         if not self.modified:
             return
 
         # garbage collect -- should we sort the data according to the initial sort
         # order when writing to the new file?
```

### Comparing `shillelagh-1.2.5/src/shillelagh/adapters/memory/pandas.py` & `shillelagh-1.2.6/src/shillelagh/adapters/memory/pandas.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.5/src/shillelagh/adapters/registry.py` & `shillelagh-1.2.6/src/shillelagh/adapters/registry.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.5/src/shillelagh/backends/apsw/db.py` & `shillelagh-1.2.6/src/shillelagh/backends/apsw/db.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.5/src/shillelagh/backends/apsw/dialects/base.py` & `shillelagh-1.2.6/src/shillelagh/backends/apsw/dialects/base.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.5/src/shillelagh/backends/apsw/dialects/gsheets.py` & `shillelagh-1.2.6/src/shillelagh/backends/apsw/dialects/gsheets.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.5/src/shillelagh/backends/apsw/dialects/safe.py` & `shillelagh-1.2.6/src/shillelagh/backends/apsw/dialects/safe.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.5/src/shillelagh/backends/apsw/vt.py` & `shillelagh-1.2.6/src/shillelagh/backends/apsw/vt.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.5/src/shillelagh/console.py` & `shillelagh-1.2.6/src/shillelagh/console.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.5/src/shillelagh/exceptions.py` & `shillelagh-1.2.6/src/shillelagh/exceptions.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.5/src/shillelagh/fields.py` & `shillelagh-1.2.6/src/shillelagh/fields.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.5/src/shillelagh/filters.py` & `shillelagh-1.2.6/src/shillelagh/filters.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.5/src/shillelagh/functions.py` & `shillelagh-1.2.6/src/shillelagh/functions.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.5/src/shillelagh/lib.py` & `shillelagh-1.2.6/src/shillelagh/lib.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.5/src/shillelagh/types.py` & `shillelagh-1.2.6/src/shillelagh/types.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.5/src/shillelagh/typing.py` & `shillelagh-1.2.6/src/shillelagh/typing.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.5/src/shillelagh.egg-info/PKG-INFO` & `shillelagh-1.2.6/src/shillelagh.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shillelagh
-Version: 1.2.5
+Version: 1.2.6
 Summary: Making it easy to query APIs via SQL
 Home-page: https://github.com/betodealmeida/shillelagh/
 Author: Beto Dealmeida
 Author-email: roberto@dealmeida.net
 License: mit
 Project-URL: Documentation, https://shillelagh.readthedocs.io/
 Description: ==========
```

### Comparing `shillelagh-1.2.5/src/shillelagh.egg-info/SOURCES.txt` & `shillelagh-1.2.6/src/shillelagh.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.5/src/shillelagh.egg-info/entry_points.txt` & `shillelagh-1.2.6/src/shillelagh.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.5/src/shillelagh.egg-info/requires.txt` & `shillelagh-1.2.6/src/shillelagh.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.5/talks/Python Brasil 2021.pdf` & `shillelagh-1.2.6/talks/Python Brasil 2021.pdf`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.5/templates/adapter/{{cookiecutter.slug}}/test_{{cookiecutter.slug}}.py` & `shillelagh-1.2.6/templates/adapter/{{cookiecutter.slug}}/test_{{cookiecutter.slug}}.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.5/templates/adapter/{{cookiecutter.slug}}/{{cookiecutter.slug}}.py` & `shillelagh-1.2.6/templates/adapter/{{cookiecutter.slug}}/{{cookiecutter.slug}}.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.5/tests/adapters/api/datasette_test.py` & `shillelagh-1.2.6/tests/adapters/api/datasette_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.5/tests/adapters/api/generic_json_test.py` & `shillelagh-1.2.6/tests/adapters/api/generic_json_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.5/tests/adapters/api/github_test.py` & `shillelagh-1.2.6/tests/adapters/api/github_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.5/tests/adapters/api/gsheets/adapter_test.py` & `shillelagh-1.2.6/tests/adapters/api/gsheets/adapter_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1913,17 +1913,18 @@
 def test_unidirectional_sync_mode(
     mocker: MockerFixture,
     simple_sheet_adapter: requests_mock.Adapter,
 ) -> None:
     """
     Test UNIDIRECTIONAL mode.
     """
+    credentials = mocker.MagicMock()
     mocker.patch(
         "shillelagh.adapters.api.gsheets.adapter.get_credentials",
-        return_value="SECRET",
+        return_value=credentials,
     )
 
     session = requests.Session()
     session.mount("https://", simple_sheet_adapter)
     mocker.patch(
         "shillelagh.adapters.api.gsheets.adapter.GSheetsAPI._get_session",
         return_value=session,
```

### Comparing `shillelagh-1.2.5/tests/adapters/api/gsheets/fields_test.py` & `shillelagh-1.2.6/tests/adapters/api/gsheets/fields_test.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,34 +6,35 @@
 
 import dateutil.tz
 
 from shillelagh.adapters.api.gsheets.fields import (
     GSheetsBoolean,
     GSheetsDate,
     GSheetsDateTime,
+    GSheetsDuration,
     GSheetsNumber,
     GSheetsString,
     GSheetsTime,
 )
 from shillelagh.fields import ISODateTime, Order
 
 
-def test_comparison():
+def test_comparison() -> None:
     """
     Test that a GSheets field is different from a standard field.
     """
     assert GSheetsDateTime([], Order.NONE, True) != ISODateTime([], Order.NONE, True)
     assert GSheetsDateTime([], Order.NONE, True) == GSheetsDateTime(
         [],
         Order.NONE,
         True,
     )
 
 
-def test_GSheetsDateTime():
+def test_GSheetsDateTime() -> None:
     """
     Test ``GSheetsDateTime``.
     """
     assert GSheetsDateTime().parse(None) is None
     assert GSheetsDateTime().parse("") is None
 
     assert GSheetsDateTime(pattern="M/d/yyyy H:mm:ss").parse(
@@ -59,15 +60,15 @@
     assert GSheetsDateTime().quote("") == "null"
     assert (
         GSheetsDateTime(pattern="M/d/yyyy H:mm:ss").quote("12/31/2020 12:34:56")
         == "datetime '2020-12-31 12:34:56'"
     )
 
 
-def test_GSheetsDateTime_timezone():
+def test_GSheetsDateTime_timezone() -> None:
     """
     Test GSheetsDateTime when timezone is set.
     """
     timezone = dateutil.tz.gettz("America/Los_Angeles")
 
     assert GSheetsDateTime(pattern="M/d/yyyy H:mm:ss", timezone=timezone).parse(
         "12/31/2020 12:34:56",
@@ -77,15 +78,15 @@
         GSheetsDateTime(pattern="M/d/yyyy H:mm:ss", timezone=timezone).format(
             datetime.datetime(2020, 12, 31, 12, 34, 56, tzinfo=datetime.timezone.utc),
         )
         == "12/31/2020 4:34:56"
     )
 
 
-def test_GSheetsDate():
+def test_GSheetsDate() -> None:
     """
     Test ``GSheetsDate``.
     """
     assert GSheetsDate().parse(None) is None
     assert GSheetsDate().parse("") is None
 
     assert GSheetsDate(pattern="M/d/yyyy").parse("12/31/2020") == datetime.date(
@@ -101,15 +102,15 @@
     )
 
     assert GSheetsDate().quote(None) == "null"
     assert GSheetsDate().quote("") == "null"
     assert GSheetsDate(pattern="M/d/yyyy").quote("12/31/2020") == "date '2020-12-31'"
 
 
-def test_GSheetsTime():
+def test_GSheetsTime() -> None:
     """
     Test ``GSheetsTime``.
     """
     assert GSheetsTime().parse(None) is None
     assert GSheetsTime().parse("") is None
 
     assert GSheetsTime(pattern="h:mm:ss am/pm").parse("12:34:56 AM") == datetime.time(
@@ -128,15 +129,44 @@
     assert GSheetsTime().quote("") == "null"
     assert (
         GSheetsTime(pattern="h:mm:ss am/pm").quote("12:34:56 AM")
         == "timeofday '00:34:56'"
     )
 
 
-def test_GSheetsBoolean():
+def test_GSheetsDuration() -> None:
+    """
+    Test ``GSheetsDuration``.
+    """
+    assert GSheetsDuration().parse(None) is None
+    assert GSheetsDuration().parse("") is None
+
+    assert GSheetsDuration(pattern="[h]:mm:ss").parse("12:34:56") == datetime.timedelta(
+        hours=12,
+        minutes=34,
+        seconds=56,
+    )
+
+    assert GSheetsDuration().format(None) == ""
+    assert (
+        GSheetsDuration(pattern="[h]:mm:ss").format(
+            datetime.timedelta(hours=12, minutes=34, seconds=56),
+        )
+        == "12:34:56"
+    )
+
+    assert GSheetsDuration().quote(None) == "null"
+    assert GSheetsDuration().quote("") == "null"
+    assert (
+        GSheetsDuration(pattern="[h]:mm:ss").quote("12:34:56")
+        == "datetime '1899-12-30 12:34:56'"
+    )
+
+
+def test_GSheetsBoolean() -> None:
     """
     Test ``GSheetsBoolean``.
     """
     assert GSheetsBoolean().parse(None) is None
     assert GSheetsBoolean().parse("") is None
     assert GSheetsBoolean().parse("TRUE") is True
     assert GSheetsBoolean().parse("FALSE") is False
@@ -147,15 +177,15 @@
 
     assert GSheetsBoolean().quote(None) == "null"
     assert GSheetsBoolean().quote("") == "null"
     assert GSheetsBoolean().quote("TRUE") == "true"
     assert GSheetsBoolean().quote("FALSE") == "false"
 
 
-def test_GSheetsNumber():
+def test_GSheetsNumber() -> None:
     """
     Test ``GSheetsNumber``.
     """
     assert GSheetsNumber().parse(None) is None
     assert GSheetsNumber().parse("") is None
     assert GSheetsNumber().parse("1") == 1.0
     assert GSheetsNumber().parse("1.0") == 1.0
@@ -171,15 +201,15 @@
 
     assert GSheetsNumber().quote(None) == "null"
     assert GSheetsNumber().quote("") == "null"
     assert GSheetsNumber().quote(1) == "1"
     assert GSheetsNumber().quote(1.0) == "1.0"
 
 
-def test_GSheetsString():
+def test_GSheetsString() -> None:
     """
     Test ``GSheetsString``.
     """
     assert GSheetsString().parse(None) is None
     assert GSheetsString().parse("") is None
     assert GSheetsString().parse("test") == "test"
```

### Comparing `shillelagh-1.2.5/tests/adapters/api/gsheets/integration_test.py` & `shillelagh-1.2.6/tests/adapters/api/gsheets/integration_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.5/tests/adapters/api/gsheets/lib_test.py` & `shillelagh-1.2.6/tests/adapters/api/gsheets/lib_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Tests for shillelagh.adapters.api.gsheets.lib.
 """
 import itertools
+from typing import List, cast
 
 import dateutil.tz
 import pytest
 from pytest_mock import MockerFixture
 
 from shillelagh.adapters.api.gsheets.fields import (
     GSheetsBoolean,
@@ -23,20 +24,21 @@
     get_index_from_letters,
     get_sync_mode,
     get_url,
     get_value_from_cell,
     get_values_from_row,
 )
 from shillelagh.adapters.api.gsheets.types import SyncMode
+from shillelagh.adapters.api.gsheets.typing import QueryResultsError
 from shillelagh.exceptions import ProgrammingError
 from shillelagh.fields import Order
 from shillelagh.filters import Equal, IsNotNull, IsNull, Like, NotEqual, Range
 
 
-def test_get_field():
+def test_get_field() -> None:
     """
     Test ``get_field``.
     """
     assert get_field({"type": "string"}, None) == GSheetsString(
         [Range, Equal, NotEqual, Like, IsNull, IsNotNull],
         Order.ANY,
         True,
@@ -89,15 +91,15 @@
     assert get_field({"type": "invalid"}, None) == GSheetsString(
         [Range, Equal, NotEqual, Like, IsNull, IsNotNull],
         Order.ANY,
         True,
     )
 
 
-def test_format_error_message():
+def test_format_error_message() -> None:
     """
     Test ``format_error_message``.
     """
     assert format_error_message([]) == ""
     response = {
         "version": "0.6",
         "reqId": "0",
@@ -106,18 +108,21 @@
             {
                 "reason": "invalid_query",
                 "message": "INVALID_QUERY",
                 "detailed_message": "Invalid query: NO_COLUMN: C",
             },
         ],
     }
-    assert format_error_message(response["errors"]) == "Invalid query: NO_COLUMN: C"
+    assert (
+        format_error_message(cast(List[QueryResultsError], response["errors"]))
+        == "Invalid query: NO_COLUMN: C"
+    )
 
 
-def test_get_url():
+def test_get_url() -> None:
     """
     Test ``get_url``.
     """
     assert (
         get_url(
             "https://docs.google.com/spreadsheets/d/1/edit#gid=0",
         )
@@ -142,15 +147,15 @@
         get_url(
             "https://docs.google.com/spreadsheets/d/1/edit?headers=2&sheet=some-sheet",
         )
         == "https://docs.google.com/spreadsheets/d/1/gviz/tq?headers=2&sheet=some-sheet"
     )
 
 
-def test_get_sync_mode():
+def test_get_sync_mode() -> None:
     """
     Test ``get_sync_mode``.
     """
     assert get_sync_mode("https://docs.google.com/spreadsheets/d/1/edit#gid=42") is None
     assert (
         get_sync_mode(
             "https://docs.google.com/spreadsheets/d/1/edit?sync_mode=BATCH#gid=42",
@@ -177,15 +182,15 @@
     with pytest.raises(ProgrammingError) as excinfo:
         get_sync_mode(
             "https://docs.google.com/spreadsheets/d/1/edit?sync_mode=INVALID#gid=42",
         )
     assert str(excinfo.value) == "Invalid sync mode: INVALID"
 
 
-def test_gen_letters():
+def test_gen_letters() -> None:
     """
     Test ``gen_letters``.
     """
     letters = list(itertools.islice(gen_letters(), 60))
     assert letters == [
         "A",
         "B",
@@ -246,26 +251,26 @@
         "AAE",
         "AAF",
         "AAG",
         "AAH",
     ]
 
 
-def test_get_index_from_letters():
+def test_get_index_from_letters() -> None:
     """
     Test ``get_index_from_letters``.
     """
     assert get_index_from_letters("A") == 0
     assert get_index_from_letters("Z") == 25
     assert get_index_from_letters("AA") == 26
     assert get_index_from_letters("AB") == 27
     assert get_index_from_letters("AAA") == 702
 
 
-def test_get_values_from_row():
+def test_get_values_from_row() -> None:
     """
     Test ``get_values_from_row``.
     """
     column_map = {"country": "A", "cnt": "C"}
     row = {"country": "BR", "cnt": 10}
     assert get_values_from_row(row, column_map) == ["BR", "", 10]
 
@@ -330,15 +335,15 @@
     # app_default_credentials
     get_credentials(app_default_credentials=True)
     credentials.assert_not_called()
     service_account.assert_not_called()
     app_default_credentials.assert_called()
 
 
-def test_get_value_from_cell():
+def test_get_value_from_cell() -> None:
     """
     Test ``get_value_from_cell``.
     """
     assert (
         get_value_from_cell({"v": "Date(2018,8,1,0,0,0)", "f": "9/1/2018 0:00:00"})
         == "9/1/2018 0:00:00"
     )
```

### Comparing `shillelagh-1.2.5/tests/adapters/api/gsheets/parsing/base_test.py` & `shillelagh-1.2.6/tests/adapters/api/gsheets/parsing/base_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,29 +11,29 @@
     InvalidValue,
     is_unescaped_literal,
     tokenize,
 )
 from shillelagh.adapters.api.gsheets.parsing.date import DD, MM, YYYY
 
 
-def test_literal_token():
+def test_literal_token() -> None:
     """
     Test the literal token.
     """
     classes = [
         DD,
         MM,
         YYYY,
         LITERAL,
     ]
 
-    assert LITERAL.match(r"\d")
-    assert LITERAL.match('"dd/mm/yy"')
+    assert LITERAL.match(r"\d", [])
+    assert LITERAL.match('"dd/mm/yy"', [])
     # matches eveything
-    assert LITERAL.match("d")
+    assert LITERAL.match("d", [])
 
     token = LITERAL("@")
     tokens = list(tokenize("@", classes))
     assert token.format(datetime(2021, 11, 12, 13, 14, 15, 16), tokens) == "@"
 
     token = LITERAL('"dd/mm/yy"')
     tokens = list(tokenize('"dd/mm/yy"', classes))
@@ -57,15 +57,15 @@
 
     token = LITERAL(r"\.")
     with pytest.raises(InvalidValue) as excinfo:
         token.parse("B", tokens)
     assert str(excinfo.value) == "B"
 
 
-def test_tokenize():
+def test_tokenize() -> None:
     """
     Test the tokenize function.
     """
     classes = [
         DD,
         MM,
         YYYY,
@@ -80,15 +80,15 @@
         YYYY("yyyy"),
         LITERAL(" -> ("),
         LITERAL('"dd/mm/yyyy"'),
         LITERAL(")"),
     ]
 
 
-def test_is_unescaped_literal():
+def test_is_unescaped_literal() -> None:
     """
     Test the is_unescaped_literal function.
     """
     assert is_unescaped_literal(LITERAL("a"))
     assert not is_unescaped_literal(LITERAL(r"\d"))
     assert not is_unescaped_literal(LITERAL('"hello"'))
     assert not is_unescaped_literal(YYYY("yyyy"))
```

### Comparing `shillelagh-1.2.5/tests/adapters/api/gsheets/parsing/date_test.py` & `shillelagh-1.2.6/tests/adapters/api/gsheets/parsing/date_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """
 Test the date/time pattern handling (parsing and formatting).
 """
 # pylint: disable=protected-access
 from datetime import date, datetime, time, timedelta
+from typing import cast
 
 import pytest
 
-from shillelagh.adapters.api.gsheets.parsing.base import LITERAL
+from shillelagh.adapters.api.gsheets.parsing.base import LITERAL, Token
 from shillelagh.adapters.api.gsheets.parsing.date import (
     AMPM,
     AP,
     DD,
     DDD,
     MM,
     MMM,
@@ -27,14 +28,15 @@
     HPlusDuration,
     M,
     Meridiem,
     MPlusDuration,
     S,
     SPlusDuration,
     format_date_time_pattern,
+    infer_column_type,
     parse_date_time_pattern,
     tokenize,
 )
 
 classes = [
     H,
     HHPlus,
@@ -57,15 +59,15 @@
     AP,
     AMPM,
     ZERO,
     LITERAL,
 ]
 
 
-def test_implementation():
+def test_implementation() -> None:
     """
     Test the examples from the reference.
 
     https://developers.google.com/sheets/api/guides/formats?hl=en
     """
     timestamp = datetime(2016, 4, 5, 16, 8, 53, 528000)
 
@@ -109,35 +111,35 @@
 
     assert format_date_time_pattern(duration, "[mmmm]:[ss].000") == "0193:41.255"
     assert (
         parse_date_time_pattern("0193:41.255", "[mmmm]:[ss].000", timedelta) == duration
     )
 
 
-def test_token():
+def test_token() -> None:
     """
     General tests for tokens.
     """
     assert H("h") == H("h")
     assert H("h") != M("m")
 
 
-def test_h_token():
+def test_h_token() -> None:
     """
     Test the h token.
     """
     token = H("h")
 
-    assert H.match("h:mm:ss")
-    assert not H.match("hh:mm:ss")
-    assert not H.match("s")
+    assert H.match("h:mm:ss", [])
+    assert not H.match("hh:mm:ss", [])
+    assert not H.match("s", [])
 
-    assert H.consume("h:mm:ss") == (token, ":mm:ss")
+    assert H.consume("h:mm:ss", []) == (token, ":mm:ss")
     with pytest.raises(Exception) as excinfo:
-        H.consume("hh:mm:ss")
+        H.consume("hh:mm:ss", [])
     assert str(excinfo.value) == "Token could not find match"
 
     tokens = list(tokenize("h:mm:ss", classes))
     assert token.format(datetime(2021, 11, 12, 13, 14, 15, 16), tokens) == "13"
     assert token.format(datetime(2021, 11, 12, 3, 14, 15, 16), tokens) == "3"
     tokens = list(tokenize("h:mm:ss a/p", classes))
     assert token.format(datetime(2021, 11, 12, 13, 14, 15, 16), tokens) == "1"
@@ -148,55 +150,55 @@
     assert token.parse("123", tokens) == ({"hour": 12}, "3")
     assert token.parse("303", tokens) == ({"hour": 3}, "03")
     with pytest.raises(Exception) as excinfo:
         token.parse("invalid", tokens)
     assert str(excinfo.value) == "Cannot parse value: invalid"
 
 
-def test_hhplus_token():
+def test_hhplus_token() -> None:
     """
     Test the hhh+ token.
     """
     token = HHPlus("hhh")
 
-    assert HHPlus.match("hhh:mm:ss")
-    assert HHPlus.match("hhhh:mm:ss")
-    assert not HHPlus.match("h:mm:ss")
+    assert HHPlus.match("hhh:mm:ss", [])
+    assert HHPlus.match("hhhh:mm:ss", [])
+    assert not HHPlus.match("h:mm:ss", [])
 
     tokens = list(tokenize("hhh:mm:ss", classes))
     assert token.format(datetime(2021, 11, 12, 13, 14, 15, 16), tokens) == "13"
     assert token.format(datetime(2021, 11, 12, 3, 14, 15, 16), tokens) == "03"
     tokens = list(tokenize("hhh:mm:ss a/p", classes))
     assert token.format(datetime(2021, 11, 12, 13, 14, 15, 16), tokens) == "01"
 
     tokens = list(tokenize("hhh:mm:ss", classes))
     assert token.parse("123", tokens) == ({"hour": 12}, "3")
     assert token.parse("303", tokens) == ({"hour": 30}, "3")
 
 
-def test_m_token():
+def test_m_token() -> None:
     """
     Test the m token.
     """
-    token = M("m")
+    token: Token = M("m")
 
-    assert M.match("m/d/y")
-    assert not M.match("mm/dd/yyyy")
-    assert not M.match("M/d/y")
+    assert M.match("m/d/y", [])
+    assert not M.match("mm/dd/yyyy", [])
+    assert not M.match("M/d/y", [])
 
-    assert M.consume("m/d/y") == (token, "/d/y")
+    assert M.consume("m/d/y", []) == (token, "/d/y")
 
     tokens = list(tokenize("m/d/y", classes))
-    token = tokens[0]
+    token = cast(M, tokens[0])
     assert token._is_minute(tokens) is False
     tokens = list(tokenize("h//m", classes))
-    token = tokens[2]
+    token = cast(M, tokens[2])
     assert token._is_minute(tokens) is True
     tokens = list(tokenize("m//s", classes))
-    token = tokens[0]
+    token = cast(M, tokens[0])
     assert token._is_minute(tokens) is True
 
     tokens = list(tokenize("m/d/y", classes))
     with pytest.raises(Exception) as excinfo:
         token.format(datetime(2021, 11, 12, 13, 14, 15, 16), tokens)
     assert str(excinfo.value) == "Token is not present in list of tokens"
     token = tokens[0]
@@ -218,137 +220,137 @@
     token = tokens[2]
     assert token.parse("14:15", tokens) == ({"minute": 14}, ":15")
     with pytest.raises(Exception) as excinfo:
         token.parse("invalid", tokens)
     assert str(excinfo.value) == "Cannot parse value: invalid"
 
 
-def test_mm_token():
+def test_mm_token() -> None:
     """
     Test the mm token.
     """
-    token = MM("mm")
+    token: Token = MM("mm")
 
-    assert MM.match("mm/dd/yyy")
-    assert not MM.match("mmm/dd/yyy")
+    assert MM.match("mm/dd/yyy", [])
+    assert not MM.match("mmm/dd/yyy", [])
 
-    assert MM.consume("mm/dd/yyyy") == (token, "/dd/yyyy")
+    assert MM.consume("mm/dd/yyyy", []) == (token, "/dd/yyyy")
 
     tokens = list(tokenize("mm/dd/yyy", classes))
     token = tokens[0]
     assert token.format(datetime(2021, 11, 12, 13, 14, 15, 16), tokens) == "11"
     assert token.parse("123", tokens) == ({"month": 12}, "3")
 
 
-def test_mmm_token():
+def test_mmm_token() -> None:
     """
     Test the mmm token.
     """
     token = MMM("mmm")
 
-    assert MMM.match("mmm/dd/yyy")
-    assert not MMM.match("mm/dd/yyy")
+    assert MMM.match("mmm/dd/yyy", [])
+    assert not MMM.match("mm/dd/yyy", [])
 
-    assert MMM.consume("mmm/dd/yyyy") == (token, "/dd/yyyy")
+    assert MMM.consume("mmm/dd/yyyy", []) == (token, "/dd/yyyy")
 
     tokens = list(tokenize("mmm/dd/yyy", classes))
     assert token.format(datetime(2021, 11, 12, 13, 14, 15, 16), tokens) == "Nov"
     assert token.parse("Mar 1st", tokens) == ({"month": 3}, " 1st")
 
 
-def test_mmmm_token():
+def test_mmmm_token() -> None:
     """
     Test the mmm token.
     """
     token = MMMM("mmmm")
 
-    assert MMMM.match("mmmm/dd/yyy")
-    assert not MMMM.match("mmm/dd/yyy")
+    assert MMMM.match("mmmm/dd/yyy", [])
+    assert not MMMM.match("mmm/dd/yyy", [])
 
-    assert MMMM.consume("mmmm/dd/yyyy") == (token, "/dd/yyyy")
+    assert MMMM.consume("mmmm/dd/yyyy", []) == (token, "/dd/yyyy")
 
     tokens = list(tokenize("mmmm/dd/yyy", classes))
     assert token.format(datetime(2021, 11, 12, 13, 14, 15, 16), tokens) == "November"
     assert token.parse("March 1st", tokens) == ({"month": 3}, " 1st")
 
 
-def test_mmmmm_token():
+def test_mmmmm_token() -> None:
     """
     Test the mmmmm token.
     """
     token = MMMMM("mmmmm")
 
-    assert MMMMM.match("mmmmm/dd/yyy")
-    assert not MMMMM.match("mmm/dd/yyy")
+    assert MMMMM.match("mmmmm/dd/yyy", [])
+    assert not MMMMM.match("mmm/dd/yyy", [])
 
-    assert MMMMM.consume("mmmmm/dd/yyyy") == (token, "/dd/yyyy")
+    assert MMMMM.consume("mmmmm/dd/yyyy", []) == (token, "/dd/yyyy")
 
     tokens = list(tokenize("mmmmm/dd/yyy", classes))
     assert token.format(datetime(2021, 11, 12, 13, 14, 15, 16), tokens) == "N"
-    assert token.parse("F 1st", token) == ({"month": 2}, " 1st")
+    assert token.parse("F 1st", tokens) == ({"month": 2}, " 1st")
     with pytest.raises(Exception) as excinfo:
         token.parse("Z 1st", tokens)
     assert str(excinfo.value) == "Unable to find month letter: Z"
     with pytest.raises(Exception) as excinfo:
         token.parse("M 1st", tokens)
     assert str(excinfo.value) == "Unable to parse month letter unambiguously: M"
 
 
-def test_s_token():
+def test_s_token() -> None:
     """
     Test the s token.
     """
     token = S("s")
 
-    assert S.match("s.00")
-    assert not S.match("ss.00")
+    assert S.match("s.00", [])
+    assert not S.match("ss.00", [])
 
-    assert S.consume("s.00") == (token, ".00")
+    assert S.consume("s.00", []) == (token, ".00")
 
     tokens = list(tokenize("h:m:s", classes))
     assert token.format(datetime(2021, 11, 12, 13, 14, 5, 16), tokens) == "5"
     assert token.format(datetime(2021, 11, 12, 13, 14, 5, 16), tokens) == "5"
     assert token.format(datetime(2021, 11, 12, 13, 14, 15, 16), tokens) == "15"
     assert token.parse("59.123", tokens) == ({"second": 59}, ".123")
     assert token.parse("60.123", tokens) == ({"second": 60}, ".123")
     assert token.parse("61.123", tokens) == ({"second": 61}, ".123")
     assert token.parse("62.123", tokens) == ({"second": 6}, "2.123")
     with pytest.raises(Exception) as excinfo:
         token.parse("invalid", tokens)
     assert str(excinfo.value) == "Cannot parse value: invalid"
 
 
-def test_ss_token():
+def test_ss_token() -> None:
     """
     Test the ss token.
     """
     token = SS("ss")
 
-    assert SS.match("ss.00")
-    assert not SS.match("s.00")
+    assert SS.match("ss.00", [])
+    assert not SS.match("s.00", [])
 
-    assert SS.consume("ss.00") == (token, ".00")
+    assert SS.consume("ss.00", []) == (token, ".00")
 
     tokens = list(tokenize("hh:mm:ss", classes))
     assert token.format(datetime(2021, 11, 12, 13, 14, 15, 16), tokens) == "15"
     assert token.format(datetime(2021, 11, 12, 13, 14, 5, 16), tokens) == "05"
     assert token.parse("59.123", tokens) == ({"second": 59}, ".123")
 
 
-def test_hplusduration_token():
+def test_hplusduration_token() -> None:
     """
     Test the [h+] token.
     """
     token = HPlusDuration("[hh]")
 
-    assert HPlusDuration.match("[h]")
-    assert HPlusDuration.match("[hh]")
-    assert not HPlusDuration.match("hh")
+    assert HPlusDuration.match("[h]", [])
+    assert HPlusDuration.match("[hh]", [])
+    assert not HPlusDuration.match("hh", [])
 
-    assert HPlusDuration.consume("[hh]:[mm]:[ss].000") == (token, ":[mm]:[ss].000")
+    assert HPlusDuration.consume("[hh]:[mm]:[ss].000", []) == (token, ":[mm]:[ss].000")
 
     tokens = list(tokenize("[hh]:[mm]:[ss].000", classes))
     assert (
         token.format(
             timedelta(days=1, hours=2, minutes=3, seconds=4, microseconds=500000),
             tokens,
         )
@@ -357,31 +359,36 @@
     assert (
         token.format(
             timedelta(hours=2, minutes=3, seconds=4, microseconds=500000),
             tokens,
         )
         == "02"
     )
-    assert token.parse("26:03:04.500", "[hh]:[mm]:[ss].000") == (
+    assert token.parse("26:03:04.500", []) == (
         {"hours": 26},
         ":03:04.500",
     )
 
+    # should never happen
+    with pytest.raises(Exception) as excinfo:
+        token.parse("invalid", [])
+    assert str(excinfo.value) == "Cannot parse value: invalid"
+
 
-def test_mplusduration_token():
+def test_mplusduration_token() -> None:
     """
     Test the [m+] token.
     """
     token = MPlusDuration("[mm]")
 
-    assert MPlusDuration.match("[m]")
-    assert MPlusDuration.match("[mm]")
-    assert not MPlusDuration.match("mm")
+    assert MPlusDuration.match("[m]", [])
+    assert MPlusDuration.match("[mm]", [])
+    assert not MPlusDuration.match("mm", [])
 
-    assert MPlusDuration.consume("[mm]:[ss].000") == (token, ":[ss].000")
+    assert MPlusDuration.consume("[mm]:[ss].000", []) == (token, ":[ss].000")
 
     tokens = list(tokenize("[hh]:[mm]:[ss].000", classes))
     assert (
         token.format(
             timedelta(days=1, hours=2, minutes=3, seconds=4, microseconds=500000),
             tokens,
         )
@@ -396,31 +403,41 @@
             tokens,
         )
         == "0123"
     )
 
     token = MPlusDuration("[mm]")
     tokens = list(tokenize("[hh]:[mm]:[ss].000", classes))
-    assert token.parse("03:04.500", "[hh]:[mm]:[ss].000") == (
+    assert token.parse("03:04.500", []) == (
         {"minutes": 3},
         ":04.500",
     )
 
+    # should never happen
+    with pytest.raises(Exception) as excinfo:
+        token.parse("invalid", [])
+    assert str(excinfo.value) == "Cannot parse value: invalid"
+
 
-def test_splusduration_token():
+def test_splusduration_token() -> None:
     """
     Test the [s+] token.
     """
     token = SPlusDuration("[ss]")
 
-    assert SPlusDuration.match("[s]")
-    assert SPlusDuration.match("[ss]")
-    assert not SPlusDuration.match("ss")
+    assert SPlusDuration.match("[s]", [])
+    assert SPlusDuration.match("[ss]", [])
+    assert not SPlusDuration.match("ss", [])
+
+    assert SPlusDuration.consume("[ss].000", []) == (token, ".000")
 
-    assert SPlusDuration.consume("[ss].000") == (token, ".000")
+    # should never happen
+    with pytest.raises(Exception) as excinfo:
+        SPlusDuration.consume("invalid", [])
+    assert str(excinfo.value) == "Token could not find match"
 
     tokens = list(tokenize("[hh]:[mm]:[ss].000", classes))
     assert (
         token.format(
             timedelta(days=1, hours=2, minutes=3, seconds=4, microseconds=500000),
             tokens,
         )
@@ -433,252 +450,262 @@
             timedelta(hours=2, minutes=3, seconds=4, microseconds=500000),
             tokens,
         )
         == "7384"
     )
 
     tokens = list(tokenize("[hh]:[mm]:[ss].000", classes))
-    assert token.parse("04.500", "[hh]:[mm]:[ss].000") == (
+    assert token.parse("04.500", []) == (
         {"seconds": 4},
         ".500",
     )
 
+    # should never happen
+    with pytest.raises(Exception) as excinfo:
+        token.parse("invalid", [])
+    assert str(excinfo.value) == "Cannot parse value: invalid"
 
-def test_d_token():
+
+def test_d_token() -> None:
     """
     Test the d token.
     """
     token = D("d")
 
-    assert D.match("d")
-    assert not D.match("dd")
+    assert D.match("d", [])
+    assert not D.match("dd", [])
 
-    assert D.consume("d/m/y") == (token, "/m/y")
+    assert D.consume("d/m/y", []) == (token, "/m/y")
 
     tokens = list(tokenize("d/m/y", classes))
     assert token.format(datetime(2021, 11, 12, 13, 14, 15, 16), tokens) == "12"
     assert token.format(datetime(2021, 11, 2, 13, 14, 15, 16), tokens) == "2"
     assert token.parse("12/11/21", tokens) == ({"day": 12}, "/11/21")
     with pytest.raises(Exception) as excinfo:
         token.parse("invalid", tokens)
     assert str(excinfo.value) == "Cannot parse value: invalid"
 
 
-def test_dd_token():
+def test_dd_token() -> None:
     """
     Test the dd token.
     """
     token = DD("dd")
 
-    assert DD.match("dd")
-    assert not DD.match("d")
-    assert not DD.match("ddd")
+    assert DD.match("dd", [])
+    assert not DD.match("d", [])
+    assert not DD.match("ddd", [])
 
-    assert DD.consume("dd/mm/yyyy") == (token, "/mm/yyyy")
+    assert DD.consume("dd/mm/yyyy", []) == (token, "/mm/yyyy")
 
     tokens = list(tokenize("dd/mm/yyyy", classes))
     assert token.format(datetime(2021, 11, 12, 13, 14, 15, 16), tokens) == "12"
     assert token.format(datetime(2021, 11, 2, 13, 14, 15, 16), tokens) == "02"
     assert token.parse("12/11/2021", tokens) == ({"day": 12}, "/11/2021")
 
 
-def test_ddd_token():
+def test_ddd_token() -> None:
     """
     Test the ddd token.
     """
     token = DDD("ddd")
 
-    assert DDD.match("ddd")
-    assert not DDD.match("dd")
-    assert not DDD.match("dddd")
+    assert DDD.match("ddd", [])
+    assert not DDD.match("dd", [])
+    assert not DDD.match("dddd", [])
 
-    assert DDD.consume("ddd, dd/mm/yyyy") == (token, ", dd/mm/yyyy")
+    assert DDD.consume("ddd, dd/mm/yyyy", []) == (token, ", dd/mm/yyyy")
 
     tokens = list(tokenize("ddd, dd/mm/yyyy", classes))
     assert token.format(datetime(2021, 11, 12, 13, 14, 15, 16), tokens) == "Fri"
     assert token.parse("Fri, 12/11/2021", tokens) == ({"weekday": 0}, ", 12/11/2021")
 
 
-def test_ddddplus_token():
+def test_ddddplus_token() -> None:
     """
     Test the dddd+ token.
     """
     token = DDDDPlus("dddd")
 
-    assert DDDDPlus.match("dddd")
-    assert DDDDPlus.match("ddddd")
-    assert not DDDDPlus.match("ddd")
+    assert DDDDPlus.match("dddd", [])
+    assert DDDDPlus.match("ddddd", [])
+    assert not DDDDPlus.match("ddd", [])
 
-    assert DDDDPlus.consume("dddd, dd/mm/yyyy") == (token, ", dd/mm/yyyy")
+    assert DDDDPlus.consume("dddd, dd/mm/yyyy", []) == (token, ", dd/mm/yyyy")
 
     tokens = list(tokenize("dddd, dd/mm/yyyy", classes))
     assert token.format(datetime(2021, 11, 12, 13, 14, 15, 16), tokens) == "Friday"
     assert token.parse("Friday, 12/11/2021", tokens) == ({"weekday": 0}, ", 12/11/2021")
 
 
-def test_yy_token():
+def test_yy_token() -> None:
     """
     Test the yy token.
     """
     token = YY("yy")
 
-    assert YY.match("y")
-    assert YY.match("yy")
-    assert not YY.match("yyy")
+    assert YY.match("y", [])
+    assert YY.match("yy", [])
+    assert not YY.match("yyy", [])
 
-    assert YY.consume("yy/mm/dd") == (token, "/mm/dd")
+    assert YY.consume("yy/mm/dd", []) == (token, "/mm/dd")
 
     tokens = list(tokenize("yy/mm/dd", classes))
     assert token.format(datetime(2021, 11, 12, 13, 14, 15, 16), tokens) == "21"
     assert token.parse("21/11/12", tokens) == ({"year": 2021}, "/11/12")
 
 
-def test_yyyy_token():
+def test_yyyy_token() -> None:
     """
     Test the yyyy token.
     """
     token = YYYY("yyyy")
 
-    assert YYYY.match("yyy")
-    assert YYYY.match("yyyy")
-    assert not YYYY.match("yy")
+    assert YYYY.match("yyy", [])
+    assert YYYY.match("yyyy", [])
+    assert not YYYY.match("yy", [])
 
-    assert YYYY.consume("yyyy/mm/dd") == (token, "/mm/dd")
+    assert YYYY.consume("yyyy/mm/dd", []) == (token, "/mm/dd")
 
     tokens = list(tokenize("yyyy/mm/dd", classes))
     assert token.format(datetime(2021, 11, 12, 13, 14, 15, 16), tokens) == "2021"
     assert token.parse("2021/11/12", tokens) == ({"year": 2021}, "/11/12")
 
 
-def test_zero_token():
+def test_zero_token() -> None:
     """
     Test the 00 token.
     """
     token = ZERO("00")
 
-    assert ZERO.match("0")
-    assert ZERO.match("00")
-    assert ZERO.match("000")
-    assert not ZERO.match("0000")
+    assert ZERO.match("0", [])
+    assert ZERO.match("00", [])
+    assert ZERO.match("000", [])
+    assert not ZERO.match("0000", [])
 
-    assert ZERO.consume("00") == (token, "")
+    assert ZERO.consume("00", []) == (token, "")
 
     tokens = list(tokenize("hh:mm:ss.000", classes))
     assert token.format(datetime(2021, 11, 12, 13, 14, 15, 167000), tokens) == "17"
 
     token = ZERO("000")
     assert token.format(datetime(2021, 11, 12, 13, 14, 15, 167000), tokens) == "167"
 
     assert token.parse("123", tokens) == ({"microsecond": 123000}, "")
 
 
-def test_ap_token():
+def test_ap_token() -> None:
     """
     Test the a/p token.
     """
     token = AP("a/p")
 
-    assert AP.match("a/p")
-    assert AP.match("A/P")
-    assert not AP.match("AM")
+    assert AP.match("a/p", [])
+    assert AP.match("A/P", [])
+    assert not AP.match("AM", [])
 
-    assert AP.consume("a/p hh:mm") == (token, " hh:mm")
+    assert AP.consume("a/p hh:mm", []) == (token, " hh:mm")
 
     tokens = list(tokenize("a/p hh:mm", classes))
     assert token.format(datetime(2021, 11, 12, 13, 14, 15, 16), tokens) == "p"
     assert token.format(datetime(2021, 11, 12, 1, 14, 15, 16), tokens) == "a"
 
     tokens = list(tokenize("A/P hh:mm", classes))
     token = AP("A/P")
     assert token.format(datetime(2021, 11, 12, 13, 14, 15, 16), tokens) == "P"
 
     assert token.parse("P 09:00", tokens) == ({"meridiem": Meridiem.PM}, " 09:00")
     assert token.parse("A 09:00", tokens) == ({"meridiem": Meridiem.AM}, " 09:00")
 
 
-def test_ampm_token():
+def test_ampm_token() -> None:
     """
     Test the am/pm token.
     """
     token = AMPM("am/pm")
 
-    assert AMPM.match("am/pm")
-    assert not AMPM.match("AM/PM")
-    assert not AMPM.match("AM")
+    assert AMPM.match("am/pm", [])
+    assert not AMPM.match("AM/PM", [])
+    assert not AMPM.match("AM", [])
 
-    assert AMPM.consume("am/pm hh:mm") == (token, " hh:mm")
+    assert AMPM.consume("am/pm hh:mm", []) == (token, " hh:mm")
 
     tokens = list(tokenize("am/pm hh:mm", classes))
     assert token.format(datetime(2021, 11, 12, 13, 14, 15, 16), tokens) == "PM"
     assert token.format(datetime(2021, 11, 12, 1, 14, 15, 16), tokens) == "AM"
 
     assert token.parse("PM 09:00", tokens) == ({"meridiem": Meridiem.PM}, " 09:00")
     assert token.parse("AM 09:00", tokens) == ({"meridiem": Meridiem.AM}, " 09:00")
 
 
-def test_parse_date_time_pattern():
+def test_parse_date_time_pattern() -> None:
     """
     Test the parse_date_time_pattern function.
     """
-    parsed = parse_date_time_pattern(
+    assert parse_date_time_pattern("0:38:19", "[h]:mm:ss", timedelta) == timedelta(
+        hours=0,
+        minutes=38,
+        seconds=19,
+    )
+
+    assert parse_date_time_pattern(
         "2021/11/12 13:14:15.167",
         "yyyy/mm/dd hh:mm:ss.000",
         datetime,
-    )
-    assert parsed == datetime(2021, 11, 12, 13, 14, 15, 167000)
+    ) == datetime(2021, 11, 12, 13, 14, 15, 167000)
 
-    parsed = parse_date_time_pattern(
+    assert parse_date_time_pattern(
         "2021/11/12 01:14:15.167 PM",
         "yyyy/mm/dd hh:mm:ss.000 am/pm",
         datetime,
-    )
-    assert parsed == datetime(2021, 11, 12, 13, 14, 15, 167000)
+    ) == datetime(2021, 11, 12, 13, 14, 15, 167000)
 
     # test that weekday is ignored
-    parsed = parse_date_time_pattern(
+    assert parse_date_time_pattern(
         "2021/11/12 Fri, 01:14:15.167 PM",
         "yyyy/mm/dd ddd, hh:mm:ss.000 am/pm",
         datetime,
-    )
-    assert parsed == datetime(2021, 11, 12, 13, 14, 15, 167000)
+    ) == datetime(2021, 11, 12, 13, 14, 15, 167000)
 
-    parsed = parse_date_time_pattern("60.123", "[ss].000", timedelta)
-    assert parsed == timedelta(seconds=60, microseconds=123000)
+    assert parse_date_time_pattern("60.123", "[ss].000", timedelta) == timedelta(
+        seconds=60,
+        microseconds=123000,
+    )
 
     with pytest.raises(Exception) as excinfo:
         parse_date_time_pattern("60.123", "[ss].000", datetime)
     assert str(excinfo.value) == "Unsupported format"
 
 
-def test_format_date_time_pattern():
+def test_format_date_time_pattern() -> None:
     """
     Test the format_date_time_pattern function.
     """
     assert (
         format_date_time_pattern(
             datetime(2021, 11, 12, 13, 14, 15, 16),
             "yyyy/mm/dd hh/mm/ss.000",
         )
         == "2021/11/12 13/14/15.000"
     )
 
 
-def test_parse_date_time_pattern_with_quotes():
+def test_parse_date_time_pattern_with_quotes() -> None:
     """
     Test parsing a timestamp with quotes.
     """
     parsed = parse_date_time_pattern(
         "1/1/2021",
         'm"/"d"/"yyyy',
         date,
     )
     assert parsed == date(2021, 1, 1)
 
 
-def test_parse_date_time_with_meridiem():
+def test_parse_date_time_with_meridiem() -> None:
     """
     Test parsing a timestamp with AM/PM in the hour.
     """
     parsed = parse_date_time_pattern(
         "12:34:56 AM",
         "h:mm:ss am/pm",
         time,
@@ -689,30 +716,38 @@
         "12:34:56 PM",
         "h:mm:ss am/pm",
         time,
     )
     assert parsed == time(12, 34, 56)
 
 
-def test_parse_date_time_without_meridiem():
+def test_parse_date_time_without_meridiem() -> None:
     """
     Test parsing a timestamp without AM/PM in the hour.
     """
     parsed = parse_date_time_pattern(
         "12/31/2020 12:34:56",
         "m/d/yyyy h:mm:ss",
         datetime,
     )
     assert parsed == datetime(2020, 12, 31, 12, 34, 56)
 
 
-def test_format_date_time_with_meridiem():
+def test_format_date_time_with_meridiem() -> None:
     """
     Test formatting a timestamp with AM/pM in the hour.
     """
     assert (
         format_date_time_pattern(
             time(12, 34, 56),
             "h:mm:ss am/pm",
         )
         == "12:34:56 PM"
     )
+
+
+def test_infer_column_type() -> None:
+    """
+    Test type inferring via patterns.
+    """
+    assert infer_column_type("h:mm:ss am/pm") == "timeofday"
+    assert infer_column_type("[h]:mm:ss") == "duration"
```

### Comparing `shillelagh-1.2.5/tests/adapters/api/gsheets/parsing/number_test.py` & `shillelagh-1.2.6/tests/adapters/api/gsheets/parsing/number_test.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     format_number_pattern,
     get_fraction,
     has_condition,
     parse_number_pattern,
 )
 
 
-def test_digits_token():
+def test_digits_token() -> None:
     """
     Test the digits token.
     """
     token = DIGITS("00")
     assert token.format(123, [token]) == "123"
     operation, rest = token.parse("123", [token])
     assert operation["operation"](0) == 123
@@ -80,15 +80,15 @@
 
     token = DIGITS("???")
     operation, rest = token.parse("  1", [token])
     assert operation["operation"](0) == 1
     assert rest == ""
 
 
-def test_digits_errors():
+def test_digits_errors() -> None:
     """
     Test errors with the digits token.
     """
     token = DIGITS("00")
     with pytest.raises(InvalidValue) as excinfo:
         token.parse("invalid", [token])
     assert str(excinfo.value) == "invalid"
@@ -100,71 +100,71 @@
 
     token = DIGITS("invalid")
     with pytest.raises(Exception) as excinfo:
         token.format(0.456, [DIGITS("0"), PERIOD("."), token])
     assert str(excinfo.value) == "Invalid token: i"
 
 
-def test_period_token():
+def test_period_token() -> None:
     """
     Test the period token.
     """
     token = PERIOD(".")
     assert token.format(123, [token]) == "."
     operation, rest = token.parse(".123", [token])
     assert operation == {}
     assert rest == "123"
 
     with pytest.raises(InvalidValue) as excinfo:
         token.parse("invalid", [token])
     assert str(excinfo.value) == "invalid"
 
 
-def test_multiple_periods():
+def test_multiple_periods() -> None:
     """
     Test that only the first period is tokenized to a ``PERIOD``.
     """
     tokens = list(fix_periods(tokenize("#.#...", [DIGITS, PERIOD, LITERAL])))
     assert tokens == [
         DIGITS("#"),
         PERIOD("."),
         DIGITS("#"),
         LITERAL("."),
         LITERAL("."),
         LITERAL("."),
     ]
 
 
-def test_percent_token():
+def test_percent_token() -> None:
     """
     Test the percent token.
     """
     token = PERCENT("%")
     assert token.format(123, [token]) == "%"
     operation, rest = token.parse("%", [token])
     assert operation["operation"](80) == 0.8
     assert rest == ""
 
     with pytest.raises(InvalidValue) as excinfo:
         token.parse("invalid", [token])
     assert str(excinfo.value) == "invalid"
 
 
-def test_comma_token():
+def test_comma_token() -> None:
     """
     Test the comma token.
     """
     token = COMMA(",,")
     assert token.format(123456789, [token]) == ""
     operation, rest = token.parse("", [token])
     assert operation["operation"](1.2) == 1200000
     assert rest == ""
 
 
-def test_e_token():
+def test_e_token() -> None:
     """
     Test the scientific notation token.
     """
     token = E("e+00")
     assert token.format(123456789, [token]) == "e+08"
     operation, rest = token.parse("e+08", [token])
     assert operation["operation"](1.2) == 120000000.0
@@ -188,15 +188,15 @@
 
     token = E("invalid")
     with pytest.raises(Exception) as excinfo:
         token.format(123, [token])
     assert str(excinfo.value) == "You are likely to be eaten by a grue."
 
 
-def test_fraction_token():
+def test_fraction_token() -> None:
     """
     Test the fraction token.
     """
     token = FRACTION("#/#")
     assert token.format(5.25, [token]) == "1/4"
     operation, rest = token.parse("1/4", [token])
     assert operation["operation"](5) == 5.25
@@ -214,26 +214,26 @@
 
     token = FRACTION("invalid")
     with pytest.raises(Exception) as excinfo:
         token.format(123, [token])
     assert str(excinfo.value) == "You are likely to be eaten by a grue."
 
 
-def test_star_token():
+def test_star_token() -> None:
     """
     Test the star token.
     """
     token = STAR("*")
     assert token.format(123, [token]) == ""
     operation, rest = token.parse("1", [token])
     assert operation == {}
     assert rest == "1"
 
 
-def test_underscore_token():
+def test_underscore_token() -> None:
     """
     Test the underscore token.
     """
     token = UNDERSCORE("_)")
     assert token.format(123, [token]) == " "
     operation, rest = token.parse(" ", [token])
     assert operation == {}
@@ -241,15 +241,15 @@
 
     token = UNDERSCORE("_)")
     with pytest.raises(Exception) as excinfo:
         token.parse("A", [token])
     assert str(excinfo.value) == "A"
 
 
-def test_at_token():
+def test_at_token() -> None:
     """
     Test the at token.
     """
     token = AT("@")
     assert token.format("123", [token]) == "123"
     operation, rest = token.parse("123", [token])
     assert operation["operation"](0) == "123"
@@ -262,15 +262,15 @@
     assert rest == " "
 
     with pytest.raises(InvalidValue) as excinfo:
         token.parse("123$", [token, UNDERSCORE("_)")])
     assert str(excinfo.value) == "123$"
 
 
-def test_color_token():
+def test_color_token() -> None:
     """
     Test the color token.
     """
     token = COLOR("[Black]")
     assert token.format(123, [token]) == ""
     operation, rest = token.parse("123", [token])
     assert operation == {}
```

### Comparing `shillelagh-1.2.5/tests/adapters/api/html_table_test.py` & `shillelagh-1.2.6/tests/adapters/api/html_table_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.5/tests/adapters/api/s3select_test.py` & `shillelagh-1.2.6/tests/adapters/api/s3select_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.5/tests/adapters/api/socrata_test.py` & `shillelagh-1.2.6/tests/adapters/api/socrata_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.5/tests/adapters/api/system_test.py` & `shillelagh-1.2.6/tests/adapters/api/system_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.5/tests/adapters/api/weatherapi_test.py` & `shillelagh-1.2.6/tests/adapters/api/weatherapi_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.5/tests/adapters/base_test.py` & `shillelagh-1.2.6/tests/adapters/base_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.5/tests/adapters/file/csvfile_test.py` & `shillelagh-1.2.6/tests/adapters/file/csvfile_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -392,14 +392,26 @@
 
     adapter = CSVFile("https://example.com/test.csv")
     assert adapter.path.exists()
     adapter.close()
     assert not adapter.path.exists()
 
 
+def test_cleanup_file_deleted(fs: FakeFilesystem, requests_mock: Mocker) -> None:
+    """
+    Test that no exception is raised if local file is deleted.
+    """
+    requests_mock.get("https://example.com/test.csv", text=CONTENTS)
+
+    adapter = CSVFile("https://example.com/test.csv")
+    assert adapter.path.exists()
+    adapter.path.unlink()
+    adapter.close()
+
+
 def test_supports(fs: FakeFilesystem, requests_mock: Mocker) -> None:
     """
     Test the ``supports`` method.
     """
     fs.create_file("test.csv", contents=CONTENTS)
     requests_mock.head(
         "https://example.com/csv/test",
```

### Comparing `shillelagh-1.2.5/tests/adapters/memory/pandas_test.py` & `shillelagh-1.2.6/tests/adapters/memory/pandas_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.5/tests/adapters/registry_test.py` & `shillelagh-1.2.6/tests/adapters/registry_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.5/tests/backends/apsw/db_test.py` & `shillelagh-1.2.6/tests/backends/apsw/db_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.5/tests/backends/apsw/dbapi_test.py` & `shillelagh-1.2.6/tests/backends/apsw/dbapi_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.5/tests/backends/apsw/dialects/base_test.py` & `shillelagh-1.2.6/tests/backends/apsw/dialects/base_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.5/tests/backends/apsw/dialects/gsheets_test.py` & `shillelagh-1.2.6/tests/backends/apsw/dialects/gsheets_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.5/tests/backends/apsw/dialects/safe_test.py` & `shillelagh-1.2.6/tests/backends/apsw/dialects/safe_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.5/tests/backends/apsw/vt_test.py` & `shillelagh-1.2.6/tests/backends/apsw/vt_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.5/tests/conftest.py` & `shillelagh-1.2.6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.5/tests/console_test.py` & `shillelagh-1.2.6/tests/console_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.5/tests/fakes/__init__.py` & `shillelagh-1.2.6/tests/fakes/__init__.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.5/tests/fakes/cdc_data_response.json` & `shillelagh-1.2.6/tests/fakes/cdc_data_response.json`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.5/tests/fakes/cdc_metadata_response.json` & `shillelagh-1.2.6/tests/fakes/cdc_metadata_response.json`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.5/tests/fakes/datasette_columns_response.json` & `shillelagh-1.2.6/tests/fakes/datasette_columns_response.json`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.5/tests/fakes/datasette_data_response_1.json` & `shillelagh-1.2.6/tests/fakes/datasette_data_response_1.json`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.5/tests/fakes/datasette_data_response_2.json` & `shillelagh-1.2.6/tests/fakes/datasette_data_response_2.json`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.5/tests/fakes/datasette_metadata_response.json` & `shillelagh-1.2.6/tests/fakes/datasette_metadata_response.json`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.5/tests/fakes/datasette_results.json` & `shillelagh-1.2.6/tests/fakes/datasette_results.json`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.5/tests/fakes/github_response.json` & `shillelagh-1.2.6/tests/fakes/github_response.json`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.5/tests/fakes/github_single_response.json` & `shillelagh-1.2.6/tests/fakes/github_single_response.json`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.5/tests/fakes/incidents.json` & `shillelagh-1.2.6/tests/fakes/incidents.json`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.5/tests/fakes/weatherapi_response.json` & `shillelagh-1.2.6/tests/fakes/weatherapi_response.json`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.5/tests/fields_test.py` & `shillelagh-1.2.6/tests/fields_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.5/tests/filters_test.py` & `shillelagh-1.2.6/tests/filters_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.5/tests/functions_test.py` & `shillelagh-1.2.6/tests/functions_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.5/tests/lib_test.py` & `shillelagh-1.2.6/tests/lib_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -316,15 +316,15 @@
 
 def test_serialize() -> None:
     """
     Test ``serialize``.
     """
     assert serialize(["O'Malley's"]) == "2wEAAAD6Ck8nTWFsbGV5J3M="
 
-    def func():
+    def func() -> int:
         return 42
 
     with pytest.raises(ProgrammingError) as excinfo:
         serialize(func)
     assert str(excinfo.value) == (
         f"The argument {func} is not serializable because it has type {type(func)}. "
         "Make sure only basic types (list, dicts, strings, numbers) are passed as "
@@ -339,14 +339,15 @@
     assert deserialize("2wEAAAD6Ck8nTWFsbGV5J3M=") == ["O'Malley's"]
 
 
 def test_combine_args_kwargs() -> None:
     """
     Test ``combine_args_kwargs``.
     """
+
     # pylint: disable=unused-argument, invalid-name
     def func(a: int = 0, b: str = "test", c: float = 10.0) -> None:
         pass
 
     args = ()
     kwargs = {"b": "TEST"}
     assert combine_args_kwargs(func, *args, **kwargs) == (0, "TEST", 10.0)
```

### Comparing `shillelagh-1.2.5/tests/types_test.py` & `shillelagh-1.2.6/tests/types_test.py`

 * *Files identical despite different names*

