# Comparing `tmp/glean_parser-7.2.1.tar.gz` & `tmp/glean_parser-8.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/glean_parser-7.2.1.tar", last modified: Tue May  9 08:26:10 2023, max compression
+gzip compressed data, was "dist/glean_parser-8.0.0.tar", last modified: Fri Jul 21 13:21:40 2023, max compression
```

## Comparing `glean_parser-7.2.1.tar` & `glean_parser-8.0.0.tar`

### file list

```diff
@@ -1,132 +1,138 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-09 08:26:10.000000 glean_parser-7.2.1/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-09 08:26:10.000000 glean_parser-7.2.1/.circleci/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6784 2023-05-09 08:25:52.000000 glean_parser-7.2.1/.circleci/config.yml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      292 2023-05-09 08:25:52.000000 glean_parser-7.2.1/.editorconfig
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-09 08:26:10.000000 glean_parser-7.2.1/.github/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      323 2023-05-09 08:25:52.000000 glean_parser-7.2.1/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      106 2023-05-09 08:25:52.000000 glean_parser-7.2.1/.github/dependabot.yml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      524 2023-05-09 08:25:52.000000 glean_parser-7.2.1/.github/pull_request_template.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1242 2023-05-09 08:25:52.000000 glean_parser-7.2.1/.gitignore
--rw-r--r--   0 circleci  (1001) circleci  (1002)      169 2023-05-09 08:25:52.000000 glean_parser-7.2.1/.swiftlint.yml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      455 2023-05-09 08:25:52.000000 glean_parser-7.2.1/AUTHORS.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)    24845 2023-05-09 08:25:52.000000 glean_parser-7.2.1/CHANGELOG.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      691 2023-05-09 08:25:52.000000 glean_parser-7.2.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6023 2023-05-09 08:25:52.000000 glean_parser-7.2.1/CONTRIBUTING.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16725 2023-05-09 08:25:52.000000 glean_parser-7.2.1/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)      350 2023-05-09 08:25:52.000000 glean_parser-7.2.1/MANIFEST.in
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2448 2023-05-09 08:25:52.000000 glean_parser-7.2.1/Makefile
--rw-r--r--   0 circleci  (1001) circleci  (1002)    33544 2023-05-09 08:26:10.000000 glean_parser-7.2.1/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2324 2023-05-09 08:25:52.000000 glean_parser-7.2.1/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-09 08:26:10.000000 glean_parser-7.2.1/docs/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      613 2023-05-09 08:25:52.000000 glean_parser-7.2.1/docs/Makefile
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-09 08:26:10.000000 glean_parser-7.2.1/docs/_static/
--rw-r--r--   0 circleci  (1001) circleci  (1002)   116026 2023-05-09 08:25:52.000000 glean_parser-7.2.1/docs/_static/glean.jpeg
--rw-r--r--   0 circleci  (1001) circleci  (1002)      455 2023-05-09 08:25:52.000000 glean_parser-7.2.1/docs/authors.md
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)     4921 2023-05-09 08:25:52.000000 glean_parser-7.2.1/docs/conf.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6023 2023-05-09 08:25:52.000000 glean_parser-7.2.1/docs/contributing.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)    24845 2023-05-09 08:25:52.000000 glean_parser-7.2.1/docs/history.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      484 2023-05-09 08:25:52.000000 glean_parser-7.2.1/docs/index.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      929 2023-05-09 08:25:52.000000 glean_parser-7.2.1/docs/installation.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      774 2023-05-09 08:25:52.000000 glean_parser-7.2.1/docs/make.bat
--rw-r--r--   0 circleci  (1001) circleci  (1002)      436 2023-05-09 08:25:52.000000 glean_parser-7.2.1/docs/metrics-yaml.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      415 2023-05-09 08:25:52.000000 glean_parser-7.2.1/docs/pings-yaml.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2324 2023-05-09 08:25:52.000000 glean_parser-7.2.1/docs/readme.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      415 2023-05-09 08:25:52.000000 glean_parser-7.2.1/docs/tags-yaml.rst
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-09 08:26:10.000000 glean_parser-7.2.1/glean_parser/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      533 2023-05-09 08:25:52.000000 glean_parser-7.2.1/glean_parser/__init__.py
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)     8631 2023-05-09 08:25:52.000000 glean_parser-7.2.1/glean_parser/__main__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4405 2023-05-09 08:25:52.000000 glean_parser-7.2.1/glean_parser/coverage.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2152 2023-05-09 08:25:52.000000 glean_parser-7.2.1/glean_parser/data_review.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11230 2023-05-09 08:25:52.000000 glean_parser-7.2.1/glean_parser/javascript.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12598 2023-05-09 08:25:52.000000 glean_parser-7.2.1/glean_parser/kotlin.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16303 2023-05-09 08:25:52.000000 glean_parser-7.2.1/glean_parser/lint.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9066 2023-05-09 08:25:52.000000 glean_parser-7.2.1/glean_parser/markdown.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12384 2023-05-09 08:25:52.000000 glean_parser-7.2.1/glean_parser/metrics.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15309 2023-05-09 08:25:52.000000 glean_parser-7.2.1/glean_parser/parser.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2815 2023-05-09 08:25:52.000000 glean_parser-7.2.1/glean_parser/pings.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6744 2023-05-09 08:25:52.000000 glean_parser-7.2.1/glean_parser/rust.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-09 08:26:10.000000 glean_parser-7.2.1/glean_parser/schemas/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    19566 2023-05-09 08:25:52.000000 glean_parser-7.2.1/glean_parser/schemas/metrics.1-0-0.schema.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)    23843 2023-05-09 08:25:52.000000 glean_parser-7.2.1/glean_parser/schemas/metrics.2-0-0.schema.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4315 2023-05-09 08:25:52.000000 glean_parser-7.2.1/glean_parser/schemas/pings.1-0-0.schema.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4363 2023-05-09 08:25:52.000000 glean_parser-7.2.1/glean_parser/schemas/pings.2-0-0.schema.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1231 2023-05-09 08:25:52.000000 glean_parser-7.2.1/glean_parser/schemas/tags.1-0-0.schema.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8379 2023-05-09 08:25:52.000000 glean_parser-7.2.1/glean_parser/swift.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1391 2023-05-09 08:25:52.000000 glean_parser-7.2.1/glean_parser/tags.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-09 08:26:10.000000 glean_parser-7.2.1/glean_parser/templates/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3287 2023-05-09 08:25:52.000000 glean_parser-7.2.1/glean_parser/templates/data_review.jinja2
--rw-r--r--   0 circleci  (1001) circleci  (1002)      474 2023-05-09 08:25:52.000000 glean_parser-7.2.1/glean_parser/templates/javascript.buildinfo.jinja2
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2669 2023-05-09 08:25:52.000000 glean_parser-7.2.1/glean_parser/templates/javascript.jinja2
--rw-r--r--   0 circleci  (1001) circleci  (1002)      920 2023-05-09 08:25:52.000000 glean_parser-7.2.1/glean_parser/templates/kotlin.buildinfo.jinja2
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5099 2023-05-09 08:25:52.000000 glean_parser-7.2.1/glean_parser/templates/kotlin.geckoview.jinja2
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5247 2023-05-09 08:25:52.000000 glean_parser-7.2.1/glean_parser/templates/kotlin.jinja2
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3425 2023-05-09 08:25:52.000000 glean_parser-7.2.1/glean_parser/templates/markdown.jinja2
--rw-r--r--   0 circleci  (1001) circleci  (1002)      156 2023-05-09 08:25:52.000000 glean_parser-7.2.1/glean_parser/templates/qmldir.jinja2
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10797 2023-05-09 08:25:52.000000 glean_parser-7.2.1/glean_parser/templates/rust.jinja2
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4809 2023-05-09 08:25:52.000000 glean_parser-7.2.1/glean_parser/templates/swift.jinja2
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7962 2023-05-09 08:25:52.000000 glean_parser-7.2.1/glean_parser/translate.py
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)     2037 2023-05-09 08:25:52.000000 glean_parser-7.2.1/glean_parser/translation_options.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16825 2023-05-09 08:25:52.000000 glean_parser-7.2.1/glean_parser/util.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2118 2023-05-09 08:25:52.000000 glean_parser-7.2.1/glean_parser/validate_ping.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-09 08:26:10.000000 glean_parser-7.2.1/glean_parser.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    33544 2023-05-09 08:26:10.000000 glean_parser-7.2.1/glean_parser.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3062 2023-05-09 08:26:10.000000 glean_parser-7.2.1/glean_parser.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-09 08:26:10.000000 glean_parser-7.2.1/glean_parser.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       69 2023-05-09 08:26:10.000000 glean_parser-7.2.1/glean_parser.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-09 08:26:10.000000 glean_parser-7.2.1/glean_parser.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (1001) circleci  (1002)      152 2023-05-09 08:26:10.000000 glean_parser-7.2.1/glean_parser.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-05-09 08:26:10.000000 glean_parser-7.2.1/glean_parser.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       83 2023-05-09 08:25:52.000000 glean_parser-7.2.1/pytest.ini
--rw-r--r--   0 circleci  (1001) circleci  (1002)      479 2023-05-09 08:25:52.000000 glean_parser-7.2.1/requirements_dev.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      155 2023-05-09 08:26:10.000000 glean_parser-7.2.1/setup.cfg
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)     2286 2023-05-09 08:25:52.000000 glean_parser-7.2.1/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-09 08:26:10.000000 glean_parser-7.2.1/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      504 2023-05-09 08:25:52.000000 glean_parser-7.2.1/tests/conftest.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-09 08:26:10.000000 glean_parser-7.2.1/tests/data/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1997 2023-05-09 08:25:52.000000 glean_parser-7.2.1/tests/data/all_metrics.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      525 2023-05-09 08:25:52.000000 glean_parser-7.2.1/tests/data/all_pings.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      885 2023-05-09 08:25:52.000000 glean_parser-7.2.1/tests/data/bad_ping.yamlx
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9453 2023-05-09 08:25:52.000000 glean_parser-7.2.1/tests/data/core.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      786 2023-05-09 08:25:52.000000 glean_parser-7.2.1/tests/data/duplicate_labeled.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      518 2023-05-09 08:25:52.000000 glean_parser-7.2.1/tests/data/duplicate_send_in_ping.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      104 2023-05-09 08:25:52.000000 glean_parser-7.2.1/tests/data/empty.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      755 2023-05-09 08:25:52.000000 glean_parser-7.2.1/tests/data/event_key_ordering.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      688 2023-05-09 08:25:52.000000 glean_parser-7.2.1/tests/data/events_with_types.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3539 2023-05-09 08:25:52.000000 glean_parser-7.2.1/tests/data/gecko.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      597 2023-05-09 08:25:52.000000 glean_parser-7.2.1/tests/data/invalid-ping-names.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      129 2023-05-09 08:25:52.000000 glean_parser-7.2.1/tests/data/invalid.yamlx
--rw-r--r--   0 circleci  (1001) circleci  (1002)      481 2023-05-09 08:25:52.000000 glean_parser-7.2.1/tests/data/jwe.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      714 2023-05-09 08:25:52.000000 glean_parser-7.2.1/tests/data/metric-with-tags.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      768 2023-05-09 08:25:52.000000 glean_parser-7.2.1/tests/data/mixed-expirations.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      672 2023-05-09 08:25:52.000000 glean_parser-7.2.1/tests/data/old_event_api.yamlx
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1232 2023-05-09 08:25:52.000000 glean_parser-7.2.1/tests/data/ordering.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1451 2023-05-09 08:25:52.000000 glean_parser-7.2.1/tests/data/pings.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1799 2023-05-09 08:25:52.000000 glean_parser-7.2.1/tests/data/rate.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2540 2023-05-09 08:25:52.000000 glean_parser-7.2.1/tests/data/schema-violation.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      548 2023-05-09 08:25:52.000000 glean_parser-7.2.1/tests/data/send_if_empty_with_metrics.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      488 2023-05-09 08:25:52.000000 glean_parser-7.2.1/tests/data/single_labeled.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      584 2023-05-09 08:25:52.000000 glean_parser-7.2.1/tests/data/smaller.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      445 2023-05-09 08:25:52.000000 glean_parser-7.2.1/tests/data/tags.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      601 2023-05-09 08:25:52.000000 glean_parser-7.2.1/tests/data/telemetry_mirror.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      973 2023-05-09 08:25:52.000000 glean_parser-7.2.1/tests/data/text.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1377 2023-05-09 08:25:52.000000 glean_parser-7.2.1/tests/data/text_invalid.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1535 2023-05-09 08:25:52.000000 glean_parser-7.2.1/tests/data/wrong_key.yamlx
--rw-r--r--   0 circleci  (1001) circleci  (1002)      551 2023-05-09 08:25:52.000000 glean_parser-7.2.1/tests/data/yaml_nits.yamlx
--rw-r--r--   0 circleci  (1001) circleci  (1002)       26 2023-05-09 08:25:52.000000 glean_parser-7.2.1/tests/detekt.yml
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)     7083 2023-05-09 08:25:52.000000 glean_parser-7.2.1/tests/test_cli.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13895 2023-05-09 08:25:52.000000 glean_parser-7.2.1/tests/test_javascript.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14509 2023-05-09 08:25:52.000000 glean_parser-7.2.1/tests/test_kotlin.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13113 2023-05-09 08:25:52.000000 glean_parser-7.2.1/tests/test_lint.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7306 2023-05-09 08:25:52.000000 glean_parser-7.2.1/tests/test_markdown.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5919 2023-05-09 08:25:52.000000 glean_parser-7.2.1/tests/test_metrics.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    32037 2023-05-09 08:25:52.000000 glean_parser-7.2.1/tests/test_parser.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2169 2023-05-09 08:25:52.000000 glean_parser-7.2.1/tests/test_pings.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8037 2023-05-09 08:25:52.000000 glean_parser-7.2.1/tests/test_rust.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10767 2023-05-09 08:25:52.000000 glean_parser-7.2.1/tests/test_swift.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1467 2023-05-09 08:25:52.000000 glean_parser-7.2.1/tests/test_tags.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7318 2023-05-09 08:25:52.000000 glean_parser-7.2.1/tests/test_translate.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1108 2023-05-09 08:25:52.000000 glean_parser-7.2.1/tests/test_utils.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1295 2023-05-09 08:25:52.000000 glean_parser-7.2.1/tests/test_validate_ping.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1571 2023-05-09 08:25:52.000000 glean_parser-7.2.1/tests/util.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-09 08:26:10.000000 glean_parser-7.2.1/tools/
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)     4713 2023-05-09 08:25:52.000000 glean_parser-7.2.1/tools/extract_data_categories.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-21 13:21:40.000000 glean_parser-8.0.0/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-21 13:21:40.000000 glean_parser-8.0.0/.circleci/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6784 2023-07-21 13:21:17.000000 glean_parser-8.0.0/.circleci/config.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      292 2023-07-21 13:21:17.000000 glean_parser-8.0.0/.editorconfig
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-21 13:21:40.000000 glean_parser-8.0.0/.github/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      323 2023-07-21 13:21:17.000000 glean_parser-8.0.0/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      106 2023-07-21 13:21:17.000000 glean_parser-8.0.0/.github/dependabot.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      524 2023-07-21 13:21:17.000000 glean_parser-8.0.0/.github/pull_request_template.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1242 2023-07-21 13:21:17.000000 glean_parser-8.0.0/.gitignore
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      169 2023-07-21 13:21:17.000000 glean_parser-8.0.0/.swiftlint.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      455 2023-07-21 13:21:17.000000 glean_parser-8.0.0/AUTHORS.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    25390 2023-07-21 13:21:17.000000 glean_parser-8.0.0/CHANGELOG.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      691 2023-07-21 13:21:17.000000 glean_parser-8.0.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6023 2023-07-21 13:21:17.000000 glean_parser-8.0.0/CONTRIBUTING.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16725 2023-07-21 13:21:17.000000 glean_parser-8.0.0/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      350 2023-07-21 13:21:17.000000 glean_parser-8.0.0/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2448 2023-07-21 13:21:17.000000 glean_parser-8.0.0/Makefile
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    28536 2023-07-21 13:21:40.000000 glean_parser-8.0.0/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2324 2023-07-21 13:21:17.000000 glean_parser-8.0.0/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-21 13:21:40.000000 glean_parser-8.0.0/docs/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      613 2023-07-21 13:21:17.000000 glean_parser-8.0.0/docs/Makefile
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-21 13:21:40.000000 glean_parser-8.0.0/docs/_static/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   116026 2023-07-21 13:21:17.000000 glean_parser-8.0.0/docs/_static/glean.jpeg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      455 2023-07-21 13:21:17.000000 glean_parser-8.0.0/docs/authors.md
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)     4921 2023-07-21 13:21:17.000000 glean_parser-8.0.0/docs/conf.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6023 2023-07-21 13:21:17.000000 glean_parser-8.0.0/docs/contributing.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    25390 2023-07-21 13:21:17.000000 glean_parser-8.0.0/docs/history.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      484 2023-07-21 13:21:17.000000 glean_parser-8.0.0/docs/index.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      929 2023-07-21 13:21:17.000000 glean_parser-8.0.0/docs/installation.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      774 2023-07-21 13:21:17.000000 glean_parser-8.0.0/docs/make.bat
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      436 2023-07-21 13:21:17.000000 glean_parser-8.0.0/docs/metrics-yaml.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      415 2023-07-21 13:21:17.000000 glean_parser-8.0.0/docs/pings-yaml.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2324 2023-07-21 13:21:17.000000 glean_parser-8.0.0/docs/readme.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      415 2023-07-21 13:21:17.000000 glean_parser-8.0.0/docs/tags-yaml.rst
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-21 13:21:40.000000 glean_parser-8.0.0/glean_parser/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      533 2023-07-21 13:21:17.000000 glean_parser-8.0.0/glean_parser/__init__.py
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)     8631 2023-07-21 13:21:17.000000 glean_parser-8.0.0/glean_parser/__main__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4405 2023-07-21 13:21:17.000000 glean_parser-8.0.0/glean_parser/coverage.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2152 2023-07-21 13:21:17.000000 glean_parser-8.0.0/glean_parser/data_review.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11230 2023-07-21 13:21:17.000000 glean_parser-8.0.0/glean_parser/javascript.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6004 2023-07-21 13:21:17.000000 glean_parser-8.0.0/glean_parser/javascript_server.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12598 2023-07-21 13:21:17.000000 glean_parser-8.0.0/glean_parser/kotlin.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18248 2023-07-21 13:21:17.000000 glean_parser-8.0.0/glean_parser/lint.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9066 2023-07-21 13:21:17.000000 glean_parser-8.0.0/glean_parser/markdown.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12431 2023-07-21 13:21:17.000000 glean_parser-8.0.0/glean_parser/metrics.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15309 2023-07-21 13:21:17.000000 glean_parser-8.0.0/glean_parser/parser.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2815 2023-07-21 13:21:17.000000 glean_parser-8.0.0/glean_parser/pings.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6744 2023-07-21 13:21:17.000000 glean_parser-8.0.0/glean_parser/rust.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-21 13:21:40.000000 glean_parser-8.0.0/glean_parser/schemas/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    19566 2023-07-21 13:21:17.000000 glean_parser-8.0.0/glean_parser/schemas/metrics.1-0-0.schema.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    25849 2023-07-21 13:21:17.000000 glean_parser-8.0.0/glean_parser/schemas/metrics.2-0-0.schema.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4315 2023-07-21 13:21:17.000000 glean_parser-8.0.0/glean_parser/schemas/pings.1-0-0.schema.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4363 2023-07-21 13:21:17.000000 glean_parser-8.0.0/glean_parser/schemas/pings.2-0-0.schema.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1231 2023-07-21 13:21:17.000000 glean_parser-8.0.0/glean_parser/schemas/tags.1-0-0.schema.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8379 2023-07-21 13:21:17.000000 glean_parser-8.0.0/glean_parser/swift.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1391 2023-07-21 13:21:17.000000 glean_parser-8.0.0/glean_parser/tags.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-21 13:21:40.000000 glean_parser-8.0.0/glean_parser/templates/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3287 2023-07-21 13:21:17.000000 glean_parser-8.0.0/glean_parser/templates/data_review.jinja2
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      474 2023-07-21 13:21:17.000000 glean_parser-8.0.0/glean_parser/templates/javascript.buildinfo.jinja2
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2669 2023-07-21 13:21:17.000000 glean_parser-8.0.0/glean_parser/templates/javascript.jinja2
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5246 2023-07-21 13:21:17.000000 glean_parser-8.0.0/glean_parser/templates/javascript_server.jinja2
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      920 2023-07-21 13:21:17.000000 glean_parser-8.0.0/glean_parser/templates/kotlin.buildinfo.jinja2
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5099 2023-07-21 13:21:17.000000 glean_parser-8.0.0/glean_parser/templates/kotlin.geckoview.jinja2
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5247 2023-07-21 13:21:17.000000 glean_parser-8.0.0/glean_parser/templates/kotlin.jinja2
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3425 2023-07-21 13:21:17.000000 glean_parser-8.0.0/glean_parser/templates/markdown.jinja2
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      156 2023-07-21 13:21:17.000000 glean_parser-8.0.0/glean_parser/templates/qmldir.jinja2
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3600 2023-07-21 13:21:17.000000 glean_parser-8.0.0/glean_parser/templates/rust.jinja2
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4809 2023-07-21 13:21:17.000000 glean_parser-8.0.0/glean_parser/templates/swift.jinja2
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8148 2023-07-21 13:21:17.000000 glean_parser-8.0.0/glean_parser/translate.py
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)     2037 2023-07-21 13:21:17.000000 glean_parser-8.0.0/glean_parser/translation_options.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16825 2023-07-21 13:21:17.000000 glean_parser-8.0.0/glean_parser/util.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2118 2023-07-21 13:21:17.000000 glean_parser-8.0.0/glean_parser/validate_ping.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-21 13:21:40.000000 glean_parser-8.0.0/glean_parser.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    28536 2023-07-21 13:21:40.000000 glean_parser-8.0.0/glean_parser.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3278 2023-07-21 13:21:40.000000 glean_parser-8.0.0/glean_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-07-21 13:21:40.000000 glean_parser-8.0.0/glean_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       68 2023-07-21 13:21:40.000000 glean_parser-8.0.0/glean_parser.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-07-21 13:21:40.000000 glean_parser-8.0.0/glean_parser.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      152 2023-07-21 13:21:40.000000 glean_parser-8.0.0/glean_parser.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-07-21 13:21:40.000000 glean_parser-8.0.0/glean_parser.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       83 2023-07-21 13:21:17.000000 glean_parser-8.0.0/pytest.ini
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      479 2023-07-21 13:21:17.000000 glean_parser-8.0.0/requirements_dev.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      155 2023-07-21 13:21:40.000000 glean_parser-8.0.0/setup.cfg
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)     2286 2023-07-21 13:21:17.000000 glean_parser-8.0.0/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-21 13:21:40.000000 glean_parser-8.0.0/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      504 2023-07-21 13:21:17.000000 glean_parser-8.0.0/tests/conftest.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-21 13:21:40.000000 glean_parser-8.0.0/tests/data/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1997 2023-07-21 13:21:17.000000 glean_parser-8.0.0/tests/data/all_metrics.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      525 2023-07-21 13:21:17.000000 glean_parser-8.0.0/tests/data/all_pings.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      885 2023-07-21 13:21:17.000000 glean_parser-8.0.0/tests/data/bad_ping.yamlx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9453 2023-07-21 13:21:17.000000 glean_parser-8.0.0/tests/data/core.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      786 2023-07-21 13:21:17.000000 glean_parser-8.0.0/tests/data/duplicate_labeled.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      518 2023-07-21 13:21:17.000000 glean_parser-8.0.0/tests/data/duplicate_send_in_ping.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      104 2023-07-21 13:21:17.000000 glean_parser-8.0.0/tests/data/empty.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      755 2023-07-21 13:21:17.000000 glean_parser-8.0.0/tests/data/event_key_ordering.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      688 2023-07-21 13:21:17.000000 glean_parser-8.0.0/tests/data/events_with_types.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      489 2023-07-21 13:21:17.000000 glean_parser-8.0.0/tests/data/fxa-server-metrics.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      420 2023-07-21 13:21:17.000000 glean_parser-8.0.0/tests/data/fxa-server-pings.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3539 2023-07-21 13:21:17.000000 glean_parser-8.0.0/tests/data/gecko.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      597 2023-07-21 13:21:17.000000 glean_parser-8.0.0/tests/data/invalid-ping-names.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      129 2023-07-21 13:21:17.000000 glean_parser-8.0.0/tests/data/invalid.yamlx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      481 2023-07-21 13:21:17.000000 glean_parser-8.0.0/tests/data/jwe.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      714 2023-07-21 13:21:17.000000 glean_parser-8.0.0/tests/data/metric-with-tags.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      768 2023-07-21 13:21:17.000000 glean_parser-8.0.0/tests/data/mixed-expirations.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      672 2023-07-21 13:21:17.000000 glean_parser-8.0.0/tests/data/old_event_api.yamlx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1232 2023-07-21 13:21:17.000000 glean_parser-8.0.0/tests/data/ordering.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1451 2023-07-21 13:21:17.000000 glean_parser-8.0.0/tests/data/pings.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1799 2023-07-21 13:21:17.000000 glean_parser-8.0.0/tests/data/rate.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2540 2023-07-21 13:21:17.000000 glean_parser-8.0.0/tests/data/schema-violation.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      548 2023-07-21 13:21:17.000000 glean_parser-8.0.0/tests/data/send_if_empty_with_metrics.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      488 2023-07-21 13:21:17.000000 glean_parser-8.0.0/tests/data/single_labeled.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      584 2023-07-21 13:21:17.000000 glean_parser-8.0.0/tests/data/smaller.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      445 2023-07-21 13:21:17.000000 glean_parser-8.0.0/tests/data/tags.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      601 2023-07-21 13:21:17.000000 glean_parser-8.0.0/tests/data/telemetry_mirror.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      975 2023-07-21 13:21:17.000000 glean_parser-8.0.0/tests/data/text.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1377 2023-07-21 13:21:17.000000 glean_parser-8.0.0/tests/data/text_invalid.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      799 2023-07-21 13:21:17.000000 glean_parser-8.0.0/tests/data/unknown_ping_used.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1535 2023-07-21 13:21:17.000000 glean_parser-8.0.0/tests/data/wrong_key.yamlx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      551 2023-07-21 13:21:17.000000 glean_parser-8.0.0/tests/data/yaml_nits.yamlx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       26 2023-07-21 13:21:17.000000 glean_parser-8.0.0/tests/detekt.yml
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)     7083 2023-07-21 13:21:17.000000 glean_parser-8.0.0/tests/test_cli.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13895 2023-07-21 13:21:17.000000 glean_parser-8.0.0/tests/test_javascript.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1869 2023-07-21 13:21:17.000000 glean_parser-8.0.0/tests/test_javascript_server.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14509 2023-07-21 13:21:17.000000 glean_parser-8.0.0/tests/test_kotlin.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13673 2023-07-21 13:21:17.000000 glean_parser-8.0.0/tests/test_lint.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7306 2023-07-21 13:21:17.000000 glean_parser-8.0.0/tests/test_markdown.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5919 2023-07-21 13:21:17.000000 glean_parser-8.0.0/tests/test_metrics.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    32039 2023-07-21 13:21:17.000000 glean_parser-8.0.0/tests/test_parser.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2169 2023-07-21 13:21:17.000000 glean_parser-8.0.0/tests/test_pings.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8037 2023-07-21 13:21:17.000000 glean_parser-8.0.0/tests/test_rust.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10767 2023-07-21 13:21:17.000000 glean_parser-8.0.0/tests/test_swift.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1467 2023-07-21 13:21:17.000000 glean_parser-8.0.0/tests/test_tags.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7318 2023-07-21 13:21:17.000000 glean_parser-8.0.0/tests/test_translate.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1108 2023-07-21 13:21:17.000000 glean_parser-8.0.0/tests/test_utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1295 2023-07-21 13:21:17.000000 glean_parser-8.0.0/tests/test_validate_ping.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1571 2023-07-21 13:21:17.000000 glean_parser-8.0.0/tests/util.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-21 13:21:40.000000 glean_parser-8.0.0/tools/
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)     4715 2023-07-21 13:21:17.000000 glean_parser-8.0.0/tools/extract_data_categories.py
```

### Comparing `glean_parser-7.2.1/.circleci/config.yml` & `glean_parser-8.0.0/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `glean_parser-7.2.1/.github/pull_request_template.md` & `glean_parser-8.0.0/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `glean_parser-7.2.1/.gitignore` & `glean_parser-8.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `glean_parser-7.2.1/CHANGELOG.md` & `glean_parser-8.0.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 # Changelog
 
 ## Unreleased
 
+## 8.0.0
+
+- BREAKING CHANGE: Remove exposed `lint_yaml_files` function ([#580](https://github.com/mozilla/glean_parser/pull/580))
+- Rust: Removed `__glean_metric_maps` from the Rust Jinja template. This functionality is better placed downstream ([Bug 1816526](https://bugzilla.mozilla.org/show_bug.cgi?id=1816526))
+- New lint: check that all referenced pings are known ([#584](https://github.com/mozilla/glean_parser/pull/584))
+- Add experimental server-side JavaScript outputter ([FXA-7922](https://mozilla-hub.atlassian.net/browse/FXA-7922))
+
 ## 7.2.1
 
 - Unbreak last minor release ([#579](https://github.com/mozilla/glean_parser/pull/579))
 
 ## 7.2.0
 
 - Remove yamllint integration ([#578](https://github.com/mozilla/glean_parser/pull/578))
```

### Comparing `glean_parser-7.2.1/CODE_OF_CONDUCT.md` & `glean_parser-8.0.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `glean_parser-7.2.1/CONTRIBUTING.md` & `glean_parser-8.0.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `glean_parser-7.2.1/LICENSE` & `glean_parser-8.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `glean_parser-7.2.1/Makefile` & `glean_parser-8.0.0/Makefile`

 * *Files identical despite different names*

### Comparing `glean_parser-7.2.1/README.md` & `glean_parser-8.0.0/README.md`

 * *Files identical despite different names*

### Comparing `glean_parser-7.2.1/docs/Makefile` & `glean_parser-8.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `glean_parser-7.2.1/docs/_static/glean.jpeg` & `glean_parser-8.0.0/docs/_static/glean.jpeg`

 * *Files identical despite different names*

### Comparing `glean_parser-7.2.1/docs/conf.py` & `glean_parser-8.0.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `glean_parser-7.2.1/docs/contributing.md` & `glean_parser-8.0.0/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `glean_parser-7.2.1/docs/history.md` & `glean_parser-8.0.0/docs/history.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 # Changelog
 
 ## Unreleased
 
+## 8.0.0
+
+- BREAKING CHANGE: Remove exposed `lint_yaml_files` function ([#580](https://github.com/mozilla/glean_parser/pull/580))
+- Rust: Removed `__glean_metric_maps` from the Rust Jinja template. This functionality is better placed downstream ([Bug 1816526](https://bugzilla.mozilla.org/show_bug.cgi?id=1816526))
+- New lint: check that all referenced pings are known ([#584](https://github.com/mozilla/glean_parser/pull/584))
+- Add experimental server-side JavaScript outputter ([FXA-7922](https://mozilla-hub.atlassian.net/browse/FXA-7922))
+
 ## 7.2.1
 
 - Unbreak last minor release ([#579](https://github.com/mozilla/glean_parser/pull/579))
 
 ## 7.2.0
 
 - Remove yamllint integration ([#578](https://github.com/mozilla/glean_parser/pull/578))
```

### Comparing `glean_parser-7.2.1/docs/installation.md` & `glean_parser-8.0.0/docs/installation.md`

 * *Files identical despite different names*

### Comparing `glean_parser-7.2.1/docs/make.bat` & `glean_parser-8.0.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `glean_parser-7.2.1/docs/readme.md` & `glean_parser-8.0.0/docs/readme.md`

 * *Files identical despite different names*

### Comparing `glean_parser-7.2.1/glean_parser/__init__.py` & `glean_parser-8.0.0/glean_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `glean_parser-7.2.1/glean_parser/__main__.py` & `glean_parser-8.0.0/glean_parser/__main__.py`

 * *Files identical despite different names*

### Comparing `glean_parser-7.2.1/glean_parser/coverage.py` & `glean_parser-8.0.0/glean_parser/coverage.py`

 * *Files identical despite different names*

### Comparing `glean_parser-7.2.1/glean_parser/data_review.py` & `glean_parser-8.0.0/glean_parser/data_review.py`

 * *Files identical despite different names*

### Comparing `glean_parser-7.2.1/glean_parser/javascript.py` & `glean_parser-8.0.0/glean_parser/javascript.py`

 * *Files identical despite different names*

### Comparing `glean_parser-7.2.1/glean_parser/kotlin.py` & `glean_parser-8.0.0/glean_parser/kotlin.py`

 * *Files identical despite different names*

### Comparing `glean_parser-7.2.1/glean_parser/lint.py` & `glean_parser-8.0.0/glean_parser/lint.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,16 +23,20 @@
 from . import metrics
 from . import parser
 from . import pings
 from . import tags
 from . import util
 
 
+# Yield only an error message
 LintGenerator = Generator[str, None, None]
 
+# Yield fully constructed GlinterNits
+NitGenerator = Generator["GlinterNit", None, None]
+
 
 class CheckType(enum.Enum):
     warning = 0
     error = 1
 
 
 def _split_words(name: str) -> List[str]:
@@ -300,14 +304,48 @@
             yield ("The suffix 'ping' is redundant.")
         elif "ping" in ping_words:
             yield ("The word 'ping' is redundant.")
         elif "custom" in ping_words:
             yield ("The word 'custom' is redundant.")
 
 
+def check_unknown_ping(
+    check_name: str,
+    check_type: CheckType,
+    all_pings: Dict[str, pings.Ping],
+    metrics: Dict[str, metrics.Metric],
+    parser_config: Dict[str, Any],
+) -> NitGenerator:
+    """
+    Check that all pings in `send_in_pings` for all metrics are either a builtin ping
+    or in the list of defined custom pings.
+    """
+    available_pings = [p for p in all_pings]
+
+    for _, metric in metrics.items():
+        if check_name in metric.no_lint:
+            continue
+
+        send_in_pings = metric.send_in_pings
+        for target_ping in send_in_pings:
+            if target_ping in pings.RESERVED_PING_NAMES:
+                continue
+
+            if target_ping not in available_pings:
+                msg = f"Ping `{target_ping} `in `send_in_pings` is unknown."
+                name = ".".join([metric.category, metric.name])
+                nit = GlinterNit(
+                    check_name,
+                    name,
+                    msg,
+                    check_type,
+                )
+                yield nit
+
+
 # The checks that operate on an entire category of metrics:
 #    {NAME: (function, is_error)}
 CATEGORY_CHECKS: Dict[
     str, Tuple[Callable[[str, Iterable[metrics.Metric]], LintGenerator], CheckType]
 ] = {
     "COMMON_PREFIX": (check_common_prefix, CheckType.error),
     "CATEGORY_GENERIC": (check_category_generic, CheckType.error),
@@ -337,14 +375,28 @@
     str, Tuple[Callable[[pings.Ping, dict], LintGenerator], CheckType]
 ] = {
     "BUG_NUMBER": (check_bug_number, CheckType.error),
     "TAGS_REQUIRED": (check_tags_required, CheckType.error),
     "REDUNDANT_PING": (check_redundant_ping, CheckType.error),
 }
 
+ALL_OBJECT_CHECKS: Dict[
+    str,
+    Tuple[
+        Callable[
+            # check name, check type, pings, metrics, config
+            [str, CheckType, dict, dict, dict],
+            NitGenerator,
+        ],
+        CheckType,
+    ],
+] = {
+    "UNKNOWN_PING_REFERENCED": (check_unknown_ping, CheckType.error),
+}
+
 
 class GlinterNit:
     def __init__(self, check_name: str, name: str, msg: str, check_type: CheckType):
         self.check_name = check_name
         self.name = name
         self.msg = msg
         self.check_type = check_type
@@ -406,14 +458,37 @@
                 ping.metadata.get("tags", []),
                 valid_tag_names,
             )
         )
     return nits
 
 
+def _lint_all_objects(
+    objects: Dict[str, Dict[str, Union[metrics.Metric, pings.Ping, tags.Tag]]],
+    parser_config: Dict[str, Any],
+) -> List[GlinterNit]:
+    nits: List[GlinterNit] = []
+
+    pings = objects.get("pings")
+    if not pings:
+        return []
+
+    metrics = objects.get("all_metrics")
+    if not metrics:
+        return []
+
+    for check_name, (check_func, check_type) in ALL_OBJECT_CHECKS.items():
+        new_nits = list(
+            check_func(check_name, check_type, pings, metrics, parser_config)
+        )
+        nits.extend(new_nits)
+
+    return nits
+
+
 def lint_metrics(
     objs: metrics.ObjectTree,
     parser_config: Optional[Dict[str, Any]] = None,
     file=sys.stderr,
 ) -> List[GlinterNit]:
     """
     Performs glinter checks on a set of metrics objects.
@@ -423,14 +498,17 @@
     :returns: List of nits.
     """
     if parser_config is None:
         parser_config = {}
 
     nits: List[GlinterNit] = []
     valid_tag_names = [tag for tag in objs.get("tags", [])]
+
+    nits.extend(_lint_all_objects(objs, parser_config))
+
     for category_name, category in sorted(list(objs.items())):
         if category_name == "pings":
             nits.extend(_lint_pings(category, parser_config, valid_tag_names))
             continue
 
         if category_name == "tags":
             # currently we have no linting for tags
@@ -491,23 +569,14 @@
             "top-level to affect the entire file.",
             file=file,
         )
 
     return nits
 
 
-def lint_yaml_files(
-    input_filepaths: Iterable[Path],
-    file=sys.stderr,
-    parser_config: Optional[Dict[str, Any]] = None,
-) -> List:
-    """Always empty."""
-    return []
-
-
 def glinter(
     input_filepaths: Iterable[Path],
     parser_config: Optional[Dict[str, Any]] = None,
     file=sys.stderr,
 ) -> int:
     """
     Commandline helper for glinter.
```

### Comparing `glean_parser-7.2.1/glean_parser/markdown.py` & `glean_parser-8.0.0/glean_parser/markdown.py`

 * *Files identical despite different names*

### Comparing `glean_parser-7.2.1/glean_parser/metrics.py` & `glean_parser-8.0.0/glean_parser/metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,16 @@
     application = 1
     user = 2
 
 
 class DataSensitivity(enum.Enum):
     technical = 1
     interaction = 2
-    web_activity = 3
+    stored_content = 3
+    web_activity = 3  # Old, deprecated name
     highly_sensitive = 4
 
 
 class Metric:
     typename: str = "ERROR"
     glean_internal_metric_cat: str = "glean.internal.metrics"
     metric_types: Dict[str, Any] = {}
```

### Comparing `glean_parser-7.2.1/glean_parser/parser.py` & `glean_parser-8.0.0/glean_parser/parser.py`

 * *Files identical despite different names*

### Comparing `glean_parser-7.2.1/glean_parser/pings.py` & `glean_parser-8.0.0/glean_parser/pings.py`

 * *Files identical despite different names*

### Comparing `glean_parser-7.2.1/glean_parser/rust.py` & `glean_parser-8.0.0/glean_parser/rust.py`

 * *Files identical despite different names*

### Comparing `glean_parser-7.2.1/glean_parser/schemas/metrics.1-0-0.schema.yaml` & `glean_parser-8.0.0/glean_parser/schemas/metrics.1-0-0.schema.yaml`

 * *Files identical despite different names*

### Comparing `glean_parser-7.2.1/glean_parser/schemas/metrics.2-0-0.schema.yaml` & `glean_parser-8.0.0/glean_parser/schemas/metrics.2-0-0.schema.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -479,35 +479,68 @@
             Firefox during usage.
 
           - **Category 2: Interaction Data:** (`interaction`) Information about
             the user’s direct engagement with Firefox. Examples include how many
             tabs, addons, or windows a user has open; uses of specific Firefox
             features; session length, scrolls and clicks; and the status of
             discrete user preferences.
+            It also includes information about the user's in-product journeys
+            and product choices helpful to understand engagement (attitudes).
+            For example, selections of add-ons or tiles to determine
+            potential interest categories etc.
+
+          - **Category 3: Stored Content & Communications:**
+            (`stored_content`, formerly Web activity data, `web_activity`)
+            Information about what people store, sync, communicate or connect to
+            where the information is generally considered to be more sensitive
+            and personal in nature.
+            Examples include users' saved URLs or URL history,
+            specific web browsing history, general information
+            about their web browsing history
+            (such as TLDs or categories of webpages visited over time)
+            and potentially certain types of interaction data
+            about specific web pages or stories visited
+            (such as highlighted portions of a story).
+            It also includes information such as content saved by users to
+            an individual account like saved URLs, tags, notes, passwords
+            and files as well as communications that users have with one another
+            through a Mozilla service.
 
-          - **Category 3: Web activity data:** (`web_activity`) Information
-            about user web browsing that could be considered sensitive. Examples
-            include users’ specific web browsing history; general information
-            about their web browsing history (such as TLDs or categories of
-            webpages visited over time); and potentially certain types of
-            interaction data about specific webpages visited.
+          - **Category 4: Highly sensitive data
+            or clearly identifiable personal data:** (`highly_sensitive`)
 
-          - **Category 4: Highly sensitive data:** (`highly_sensitive`)
             Information that directly identifies a person, or if combined with
-            other data could identify a person. Examples include e-mail,
-            usernames, identifiers such as google ad id, apple id, fxaccount,
-            city or country (unless small ones are explicitly filtered out), or
-            certain cookies. It may be embedded within specific website content,
-            such as memory contents, dumps, captures of screen data, or DOM
-            data.
+            other data could identify a person.
+            This data may be embedded within specific website content,
+            such as memory contents, dumps, captures of screen data,
+            or DOM data.
+            Examples include account registration data like name, password,
+            and email address associated with an account,
+            payment data in connection with subscriptions or donations,
+            contact information such as phone numbers or mailing addresses,
+            email addresses associated with surveys, promotions
+            and customer support contacts.
+            It also includes any data from different categories that,
+            when combined, can identify a person, device, household or account.
+            For example Category 1 log data combined with Category 3 saved URLs.
+            Additional examples are: voice audio commands
+            (including a voice audio file), speech-to-text or text-to-speech
+            (including transcripts), biometric data, demographic information,
+            and precise location data associated with a persistent identifier,
+            individual or small population cohorts.
+            This is location inferred or determined from mechanisms
+            other than IP such as wi-fi access points, Bluetooth beacons,
+            cell phone towers or provided directly to us,
+            such as in a survey or a profile.
         type: array
         items:
           enum:
             - technical
             - interaction
+            - stored_content
             - web_activity
             - highly_sensitive
           type: string
         minLength: 1
         uniqueItems: true
 
       telemetry_mirror:
@@ -683,19 +716,21 @@
                 Text metrics must have ping or application lifetime.
               enum:
                 - ping
                 - application
 
             data_sensitivity:
               description: >
-                Text metrics require Category 3 (`web_activity`)
+                Text metrics require Category 3
+                (`stored_content` / `web_activity`)
                 or Category 4 (`highly_sensitive`).
               type: array
               items:
                 enum:
+                  - stored_content
                   - web_activity
                   - highly_sensitive
 
             send_in_pings:
               description: |
                 Text metrics can only be sent in custom pings.
                 Built-in pings are not allowed.
```

### Comparing `glean_parser-7.2.1/glean_parser/schemas/pings.1-0-0.schema.yaml` & `glean_parser-8.0.0/glean_parser/schemas/pings.1-0-0.schema.yaml`

 * *Files identical despite different names*

### Comparing `glean_parser-7.2.1/glean_parser/schemas/pings.2-0-0.schema.yaml` & `glean_parser-8.0.0/glean_parser/schemas/pings.2-0-0.schema.yaml`

 * *Files identical despite different names*

### Comparing `glean_parser-7.2.1/glean_parser/schemas/tags.1-0-0.schema.yaml` & `glean_parser-8.0.0/glean_parser/schemas/tags.1-0-0.schema.yaml`

 * *Files identical despite different names*

### Comparing `glean_parser-7.2.1/glean_parser/swift.py` & `glean_parser-8.0.0/glean_parser/swift.py`

 * *Files identical despite different names*

### Comparing `glean_parser-7.2.1/glean_parser/tags.py` & `glean_parser-8.0.0/glean_parser/tags.py`

 * *Files identical despite different names*

### Comparing `glean_parser-7.2.1/glean_parser/templates/data_review.jinja2` & `glean_parser-8.0.0/glean_parser/templates/data_review.jinja2`

 * *Files identical despite different names*

### Comparing `glean_parser-7.2.1/glean_parser/templates/javascript.jinja2` & `glean_parser-8.0.0/glean_parser/templates/javascript.jinja2`

 * *Files identical despite different names*

### Comparing `glean_parser-7.2.1/glean_parser/templates/kotlin.buildinfo.jinja2` & `glean_parser-8.0.0/glean_parser/templates/kotlin.buildinfo.jinja2`

 * *Files identical despite different names*

### Comparing `glean_parser-7.2.1/glean_parser/templates/kotlin.geckoview.jinja2` & `glean_parser-8.0.0/glean_parser/templates/kotlin.geckoview.jinja2`

 * *Files identical despite different names*

### Comparing `glean_parser-7.2.1/glean_parser/templates/kotlin.jinja2` & `glean_parser-8.0.0/glean_parser/templates/kotlin.jinja2`

 * *Files identical despite different names*

### Comparing `glean_parser-7.2.1/glean_parser/templates/markdown.jinja2` & `glean_parser-8.0.0/glean_parser/templates/markdown.jinja2`

 * *Files identical despite different names*

### Comparing `glean_parser-7.2.1/glean_parser/templates/swift.jinja2` & `glean_parser-8.0.0/glean_parser/templates/swift.jinja2`

 * *Files identical despite different names*

### Comparing `glean_parser-7.2.1/glean_parser/translate.py` & `glean_parser-8.0.0/glean_parser/translate.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import sys
 import tempfile
 from typing import Any, Callable, Dict, Iterable, List, Optional
 
 from . import lint
 from . import parser
 from . import javascript
+from . import javascript_server
 from . import kotlin
 from . import markdown
 from . import metrics
 from . import rust
 from . import swift
 from . import util
 
@@ -50,14 +51,16 @@
         self.output_func = output_func
         self.clear_patterns = clear_patterns
 
 
 OUTPUTTERS = {
     "javascript": Outputter(javascript.output_javascript, []),
     "typescript": Outputter(javascript.output_typescript, []),
+    "javascript_server": Outputter(javascript_server.output_javascript, []),
+    "typescript_server": Outputter(javascript_server.output_typescript, []),
     "kotlin": Outputter(kotlin.output_kotlin, ["*.kt"]),
     "markdown": Outputter(markdown.output_markdown, []),
     "swift": Outputter(swift.output_swift, ["*.swift"]),
     "rust": Outputter(rust.output_rust, []),
 }
```

### Comparing `glean_parser-7.2.1/glean_parser/translation_options.py` & `glean_parser-8.0.0/glean_parser/translation_options.py`

 * *Files identical despite different names*

### Comparing `glean_parser-7.2.1/glean_parser/util.py` & `glean_parser-8.0.0/glean_parser/util.py`

 * *Files identical despite different names*

### Comparing `glean_parser-7.2.1/glean_parser/validate_ping.py` & `glean_parser-8.0.0/glean_parser/validate_ping.py`

 * *Files identical despite different names*

### Comparing `glean_parser-7.2.1/glean_parser.egg-info/SOURCES.txt` & `glean_parser-8.0.0/glean_parser.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 docs/tags-yaml.rst
 docs/_static/glean.jpeg
 glean_parser/__init__.py
 glean_parser/__main__.py
 glean_parser/coverage.py
 glean_parser/data_review.py
 glean_parser/javascript.py
+glean_parser/javascript_server.py
 glean_parser/kotlin.py
 glean_parser/lint.py
 glean_parser/markdown.py
 glean_parser/metrics.py
 glean_parser/parser.py
 glean_parser/pings.py
 glean_parser/rust.py
@@ -59,25 +60,27 @@
 glean_parser/schemas/metrics.2-0-0.schema.yaml
 glean_parser/schemas/pings.1-0-0.schema.yaml
 glean_parser/schemas/pings.2-0-0.schema.yaml
 glean_parser/schemas/tags.1-0-0.schema.yaml
 glean_parser/templates/data_review.jinja2
 glean_parser/templates/javascript.buildinfo.jinja2
 glean_parser/templates/javascript.jinja2
+glean_parser/templates/javascript_server.jinja2
 glean_parser/templates/kotlin.buildinfo.jinja2
 glean_parser/templates/kotlin.geckoview.jinja2
 glean_parser/templates/kotlin.jinja2
 glean_parser/templates/markdown.jinja2
 glean_parser/templates/qmldir.jinja2
 glean_parser/templates/rust.jinja2
 glean_parser/templates/swift.jinja2
 tests/conftest.py
 tests/detekt.yml
 tests/test_cli.py
 tests/test_javascript.py
+tests/test_javascript_server.py
 tests/test_kotlin.py
 tests/test_lint.py
 tests/test_markdown.py
 tests/test_metrics.py
 tests/test_parser.py
 tests/test_pings.py
 tests/test_rust.py
@@ -92,14 +95,16 @@
 tests/data/bad_ping.yamlx
 tests/data/core.yaml
 tests/data/duplicate_labeled.yaml
 tests/data/duplicate_send_in_ping.yaml
 tests/data/empty.yaml
 tests/data/event_key_ordering.yaml
 tests/data/events_with_types.yaml
+tests/data/fxa-server-metrics.yaml
+tests/data/fxa-server-pings.yaml
 tests/data/gecko.yaml
 tests/data/invalid-ping-names.yaml
 tests/data/invalid.yamlx
 tests/data/jwe.yaml
 tests/data/metric-with-tags.yaml
 tests/data/mixed-expirations.yaml
 tests/data/old_event_api.yamlx
@@ -110,10 +115,11 @@
 tests/data/send_if_empty_with_metrics.yaml
 tests/data/single_labeled.yaml
 tests/data/smaller.yaml
 tests/data/tags.yaml
 tests/data/telemetry_mirror.yaml
 tests/data/text.yaml
 tests/data/text_invalid.yaml
+tests/data/unknown_ping_used.yaml
 tests/data/wrong_key.yamlx
 tests/data/yaml_nits.yamlx
 tools/extract_data_categories.py
```

### Comparing `glean_parser-7.2.1/setup.py` & `glean_parser-8.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `glean_parser-7.2.1/tests/data/all_metrics.yaml` & `glean_parser-8.0.0/tests/data/all_metrics.yaml`

 * *Files identical despite different names*

### Comparing `glean_parser-7.2.1/tests/data/all_pings.yaml` & `glean_parser-8.0.0/tests/data/all_pings.yaml`

 * *Files identical despite different names*

### Comparing `glean_parser-7.2.1/tests/data/bad_ping.yamlx` & `glean_parser-8.0.0/tests/data/bad_ping.yamlx`

 * *Files identical despite different names*

### Comparing `glean_parser-7.2.1/tests/data/core.yaml` & `glean_parser-8.0.0/tests/data/core.yaml`

 * *Files identical despite different names*

### Comparing `glean_parser-7.2.1/tests/data/duplicate_labeled.yaml` & `glean_parser-8.0.0/tests/data/duplicate_labeled.yaml`

 * *Files identical despite different names*

### Comparing `glean_parser-7.2.1/tests/data/duplicate_send_in_ping.yaml` & `glean_parser-8.0.0/tests/data/duplicate_send_in_ping.yaml`

 * *Files identical despite different names*

### Comparing `glean_parser-7.2.1/tests/data/event_key_ordering.yaml` & `glean_parser-8.0.0/tests/data/event_key_ordering.yaml`

 * *Files identical despite different names*

### Comparing `glean_parser-7.2.1/tests/data/events_with_types.yaml` & `glean_parser-8.0.0/tests/data/events_with_types.yaml`

 * *Files identical despite different names*

### Comparing `glean_parser-7.2.1/tests/data/gecko.yaml` & `glean_parser-8.0.0/tests/data/gecko.yaml`

 * *Files identical despite different names*

### Comparing `glean_parser-7.2.1/tests/data/invalid-ping-names.yaml` & `glean_parser-8.0.0/tests/data/invalid-ping-names.yaml`

 * *Files identical despite different names*

### Comparing `glean_parser-7.2.1/tests/data/metric-with-tags.yaml` & `glean_parser-8.0.0/tests/data/metric-with-tags.yaml`

 * *Files identical despite different names*

### Comparing `glean_parser-7.2.1/tests/data/mixed-expirations.yaml` & `glean_parser-8.0.0/tests/data/mixed-expirations.yaml`

 * *Files identical despite different names*

### Comparing `glean_parser-7.2.1/tests/data/old_event_api.yamlx` & `glean_parser-8.0.0/tests/data/old_event_api.yamlx`

 * *Files identical despite different names*

### Comparing `glean_parser-7.2.1/tests/data/ordering.yaml` & `glean_parser-8.0.0/tests/data/ordering.yaml`

 * *Files identical despite different names*

### Comparing `glean_parser-7.2.1/tests/data/pings.yaml` & `glean_parser-8.0.0/tests/data/pings.yaml`

 * *Files identical despite different names*

### Comparing `glean_parser-7.2.1/tests/data/rate.yaml` & `glean_parser-8.0.0/tests/data/rate.yaml`

 * *Files identical despite different names*

### Comparing `glean_parser-7.2.1/tests/data/schema-violation.yaml` & `glean_parser-8.0.0/tests/data/schema-violation.yaml`

 * *Files identical despite different names*

### Comparing `glean_parser-7.2.1/tests/data/send_if_empty_with_metrics.yaml` & `glean_parser-8.0.0/tests/data/send_if_empty_with_metrics.yaml`

 * *Files identical despite different names*

### Comparing `glean_parser-7.2.1/tests/data/smaller.yaml` & `glean_parser-8.0.0/tests/data/smaller.yaml`

 * *Files identical despite different names*

### Comparing `glean_parser-7.2.1/tests/data/telemetry_mirror.yaml` & `glean_parser-8.0.0/tests/data/telemetry_mirror.yaml`

 * *Files identical despite different names*

### Comparing `glean_parser-7.2.1/tests/data/text.yaml` & `glean_parser-8.0.0/tests/data/text.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -35,10 +35,10 @@
       - https://bugzilla.mozilla.org/11137353
     data_reviews:
       - http://example.com/reviews
     notification_emails:
       - CHANGE-ME@example.com
     expires: 2100-01-01
     data_sensitivity:
-      - web_activity
+      - stored_content
     no_lint:
       - EXPIRATION_DATE_TOO_FAR
```

### Comparing `glean_parser-7.2.1/tests/data/text_invalid.yaml` & `glean_parser-8.0.0/tests/data/text_invalid.yaml`

 * *Files identical despite different names*

### Comparing `glean_parser-7.2.1/tests/data/wrong_key.yamlx` & `glean_parser-8.0.0/tests/data/wrong_key.yamlx`

 * *Files identical despite different names*

### Comparing `glean_parser-7.2.1/tests/data/yaml_nits.yamlx` & `glean_parser-8.0.0/tests/data/yaml_nits.yamlx`

 * *Files identical despite different names*

### Comparing `glean_parser-7.2.1/tests/test_cli.py` & `glean_parser-8.0.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `glean_parser-7.2.1/tests/test_javascript.py` & `glean_parser-8.0.0/tests/test_javascript.py`

 * *Files identical despite different names*

### Comparing `glean_parser-7.2.1/tests/test_kotlin.py` & `glean_parser-8.0.0/tests/test_kotlin.py`

 * *Files identical despite different names*

### Comparing `glean_parser-7.2.1/tests/test_lint.py` & `glean_parser-8.0.0/tests/test_lint.py`

 * *Files 2% similar despite different names*

```diff
@@ -457,7 +457,22 @@
     assert len(errs) == 0
 
     nits = lint.lint_metrics(all_metrics.value, parser_config={})
     assert len(nits) == 1
     assert nits[0].check_name == "OLD_EVENT_API"
     assert nits[0].name == "old_event.name"
     assert "Extra keys require a type" in nits[0].msg
+
+
+def test_unknown_pings_lint():
+    """Test that the 'glinter' reports issues with unknown pings in send_in_pings."""
+    input = [ROOT / "data" / "unknown_ping_used.yaml", ROOT / "data" / "pings.yaml"]
+    all_objects = parser.parse_objects(input)
+
+    errs = list(all_objects)
+    assert len(errs) == 0
+
+    nits = lint.lint_metrics(all_objects.value, parser_config={})
+    assert len(nits) == 1
+    assert nits[0].check_name == "UNKNOWN_PING_REFERENCED"
+    assert nits[0].name == "all_metrics.non_existent_ping"
+    assert "does-not-exist" in nits[0].msg
```

### Comparing `glean_parser-7.2.1/tests/test_markdown.py` & `glean_parser-8.0.0/tests/test_markdown.py`

 * *Files identical despite different names*

### Comparing `glean_parser-7.2.1/tests/test_metrics.py` & `glean_parser-8.0.0/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `glean_parser-7.2.1/tests/test_parser.py` & `glean_parser-8.0.0/tests/test_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -901,15 +901,15 @@
 
     errors = list(all_metrics)
     assert len(errors) == 0
 
     assert all_metrics.value["valid.text"]["lifetime"].lifetime == metrics.Lifetime.ping
 
     assert all_metrics.value["valid.text"]["sensitivity"].data_sensitivity == [
-        metrics.DataSensitivity.web_activity
+        metrics.DataSensitivity.stored_content
     ]
 
 
 def test_text_invalid():
     """
     Ensure that `text` metrics parse properly.
     """
```

### Comparing `glean_parser-7.2.1/tests/test_pings.py` & `glean_parser-8.0.0/tests/test_pings.py`

 * *Files identical despite different names*

### Comparing `glean_parser-7.2.1/tests/test_rust.py` & `glean_parser-8.0.0/tests/test_rust.py`

 * *Files identical despite different names*

### Comparing `glean_parser-7.2.1/tests/test_swift.py` & `glean_parser-8.0.0/tests/test_swift.py`

 * *Files identical despite different names*

### Comparing `glean_parser-7.2.1/tests/test_tags.py` & `glean_parser-8.0.0/tests/test_tags.py`

 * *Files identical despite different names*

### Comparing `glean_parser-7.2.1/tests/test_translate.py` & `glean_parser-8.0.0/tests/test_translate.py`

 * *Files identical despite different names*

### Comparing `glean_parser-7.2.1/tests/test_utils.py` & `glean_parser-8.0.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `glean_parser-7.2.1/tests/test_validate_ping.py` & `glean_parser-8.0.0/tests/test_validate_ping.py`

 * *Files identical despite different names*

### Comparing `glean_parser-7.2.1/tests/util.py` & `glean_parser-8.0.0/tests/util.py`

 * *Files identical despite different names*

### Comparing `glean_parser-7.2.1/tools/extract_data_categories.py` & `glean_parser-8.0.0/tools/extract_data_categories.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 
 QUESTION = "what collection type of data do the requested measurements fall under?"
 
 
 CATEGORY_MAP = {
     1: "technical",
     2: "interaction",
-    3: "web_activity",
+    3: "stored_content",
     4: "highly_sensitive",
 }
 
 
 def fetch_url(url: str) -> str:
     """
     Fetch a web page containing a data review, caching it to avoid
```

