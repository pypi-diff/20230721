# Comparing `tmp/ansible-compat-4.1.4.dev0.tar.gz` & `tmp/ansible-compat-4.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansible-compat-4.1.4.dev0.tar", last modified: Thu Jul 20 10:38:52 2023, max compression
+gzip compressed data, was "ansible-compat-4.1.5.tar", last modified: Fri Jul 21 10:58:43 2023, max compression
```

## Comparing `ansible-compat-4.1.4.dev0.tar` & `ansible-compat-4.1.5.tar`

### file list

```diff
@@ -1,122 +1,125 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:38:52.589446 ansible-compat-4.1.4.dev0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:38:52.581446 ansible-compat-4.1.4.dev0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:38:52.581446 ansible-compat-4.1.4.dev0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/.github/workflows/ack.yml
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/.github/workflows/push.yml
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/.github/workflows/tox.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/.packit.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/.prettierignore
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/.prettierrc.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/.readthedocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:38:52.581446 ansible-compat-4.1.4.dev0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/.yamllint
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-07-20 10:38:52.589446 ansible-compat-4.1.4.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/ansible.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:38:52.581446 ansible-compat-4.1.4.dev0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/docs/api.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:38:52.581446 ansible-compat-4.1.4.dev0/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/docs/images/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)    10993 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/docs/images/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/docs/images/logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:38:52.573446 ansible-compat-4.1.4.dev0/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:38:52.581446 ansible-compat-4.1.4.dev0/examples/reqs_broken/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/examples/reqs_broken/requirements.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:38:52.581446 ansible-compat-4.1.4.dev0/examples/reqs_v1/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/examples/reqs_v1/requirements.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:38:52.581446 ansible-compat-4.1.4.dev0/examples/reqs_v2/
--rw-r--r--   0 runner    (1001) docker     (123)     7615 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/examples/reqs_v2/community-molecule-0.1.0.tar.gz
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/examples/reqs_v2/requirements.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4322 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     6305 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 10:38:52.589446 ansible-compat-4.1.4.dev0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:38:52.573446 ansible-compat-4.1.4.dev0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:38:52.585446 ansible-compat-4.1.4.dev0/src/ansible_compat/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/src/ansible_compat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16108 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/src/ansible_compat/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/src/ansible_compat/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/src/ansible_compat/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/src/ansible_compat/loaders.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/src/ansible_compat/ports.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/src/ansible_compat/prerun.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/src/ansible_compat/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    35618 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/src/ansible_compat/runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/src/ansible_compat/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/src/ansible_compat/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:38:52.585446 ansible-compat-4.1.4.dev0/src/ansible_compat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-07-20 10:38:52.000000 ansible-compat-4.1.4.dev0/src/ansible_compat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-07-20 10:38:52.000000 ansible-compat-4.1.4.dev0/src/ansible_compat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 10:38:52.000000 ansible-compat-4.1.4.dev0/src/ansible_compat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-20 10:38:52.000000 ansible-compat-4.1.4.dev0/src/ansible_compat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-20 10:38:52.000000 ansible-compat-4.1.4.dev0/src/ansible_compat.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:38:52.585446 ansible-compat-4.1.4.dev0/test/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:38:52.585446 ansible-compat-4.1.4.dev0/test/assets/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/test/assets/requirements-invalid-collection.yml
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/test/assets/requirements-invalid-role.yml
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/test/assets/validate0_data.json
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/test/assets/validate0_expected.json
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/test/assets/validate0_schema.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:38:52.577446 ansible-compat-4.1.4.dev0/test/collections/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:38:52.585446 ansible-compat-4.1.4.dev0/test/collections/acme.broken/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/test/collections/acme.broken/galaxy.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:38:52.585446 ansible-compat-4.1.4.dev0/test/collections/acme.goodies/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/test/collections/acme.goodies/galaxy.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:38:52.577446 ansible-compat-4.1.4.dev0/test/collections/acme.goodies/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:38:52.585446 ansible-compat-4.1.4.dev0/test/collections/acme.goodies/molecule/default/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/test/collections/acme.goodies/molecule/default/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/test/collections/acme.goodies/molecule/default/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:38:52.577446 ansible-compat-4.1.4.dev0/test/collections/acme.goodies/roles/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:38:52.577446 ansible-compat-4.1.4.dev0/test/collections/acme.goodies/roles/baz/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:38:52.577446 ansible-compat-4.1.4.dev0/test/collections/acme.goodies/roles/baz/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:38:52.585446 ansible-compat-4.1.4.dev0/test/collections/acme.goodies/roles/baz/molecule/deep_scenario/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/test/collections/acme.goodies/roles/baz/molecule/deep_scenario/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/test/collections/acme.goodies/roles/baz/molecule/deep_scenario/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:38:52.585446 ansible-compat-4.1.4.dev0/test/collections/acme.goodies/roles/baz/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/test/collections/acme.goodies/roles/baz/tasks/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:38:52.585446 ansible-compat-4.1.4.dev0/test/collections/acme.goodies/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/test/collections/acme.goodies/tests/requirements.yml
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/test/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:38:52.577446 ansible-compat-4.1.4.dev0/test/roles/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:38:52.589446 ansible-compat-4.1.4.dev0/test/roles/acme.missing_deps/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:38:52.589446 ansible-compat-4.1.4.dev0/test/roles/acme.missing_deps/meta/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/test/roles/acme.missing_deps/meta/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/test/roles/acme.missing_deps/requirements.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:38:52.577446 ansible-compat-4.1.4.dev0/test/roles/acme.sample2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:38:52.589446 ansible-compat-4.1.4.dev0/test/roles/acme.sample2/meta/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/test/roles/acme.sample2/meta/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:38:52.577446 ansible-compat-4.1.4.dev0/test/roles/ansible-role-sample/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:38:52.589446 ansible-compat-4.1.4.dev0/test/roles/ansible-role-sample/meta/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/test/roles/ansible-role-sample/meta/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:38:52.577446 ansible-compat-4.1.4.dev0/test/roles/sample3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:38:52.589446 ansible-compat-4.1.4.dev0/test/roles/sample3/meta/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/test/roles/sample3/meta/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:38:52.577446 ansible-compat-4.1.4.dev0/test/roles/sample4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:38:52.589446 ansible-compat-4.1.4.dev0/test/roles/sample4/meta/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/test/roles/sample4/meta/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/test/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/test/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/test/test_configuration_example.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/test/test_loaders.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/test/test_prerun.py
--rw-r--r--   0 runner    (1001) docker     (123)    27640 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/test/test_runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/test/test_runtime_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/test/test_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:38:52.589446 ansible-compat-4.1.4.dev0/tools/
--rwxr-xr-x   0 runner    (1001) docker     (123)      248 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/tools/get-version.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      240 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/tools/update-version.sh
--rw-r--r--   0 runner    (1001) docker     (123)     4431 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:58:43.393725 ansible-compat-4.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-21 10:58:17.000000 ansible-compat-4.1.5/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-21 10:58:17.000000 ansible-compat-4.1.5/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:58:43.353724 ansible-compat-4.1.5/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-21 10:58:17.000000 ansible-compat-4.1.5/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-21 10:58:17.000000 ansible-compat-4.1.5/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-21 10:58:17.000000 ansible-compat-4.1.5/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-21 10:58:17.000000 ansible-compat-4.1.5/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:58:43.353724 ansible-compat-4.1.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-21 10:58:17.000000 ansible-compat-4.1.5/.github/workflows/ack.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-21 10:58:17.000000 ansible-compat-4.1.5/.github/workflows/push.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-07-21 10:58:17.000000 ansible-compat-4.1.5/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-07-21 10:58:17.000000 ansible-compat-4.1.5/.github/workflows/tox.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-07-21 10:58:17.000000 ansible-compat-4.1.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-07-21 10:58:17.000000 ansible-compat-4.1.5/.packit.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-07-21 10:58:17.000000 ansible-compat-4.1.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-21 10:58:17.000000 ansible-compat-4.1.5/.prettierignore
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-21 10:58:17.000000 ansible-compat-4.1.5/.prettierrc.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-07-21 10:58:17.000000 ansible-compat-4.1.5/.readthedocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:58:43.357725 ansible-compat-4.1.5/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-21 10:58:17.000000 ansible-compat-4.1.5/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-21 10:58:17.000000 ansible-compat-4.1.5/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-21 10:58:17.000000 ansible-compat-4.1.5/.yamllint
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-21 10:58:17.000000 ansible-compat-4.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-07-21 10:58:43.393725 ansible-compat-4.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-21 10:58:17.000000 ansible-compat-4.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-21 10:58:17.000000 ansible-compat-4.1.5/ansible.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-21 10:58:17.000000 ansible-compat-4.1.5/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:58:43.357725 ansible-compat-4.1.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-21 10:58:17.000000 ansible-compat-4.1.5/docs/api.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:58:43.361724 ansible-compat-4.1.5/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-07-21 10:58:17.000000 ansible-compat-4.1.5/docs/images/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    10993 2023-07-21 10:58:17.000000 ansible-compat-4.1.5/docs/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-07-21 10:58:17.000000 ansible-compat-4.1.5/docs/images/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-21 10:58:17.000000 ansible-compat-4.1.5/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:58:43.321724 ansible-compat-4.1.5/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:58:43.361724 ansible-compat-4.1.5/examples/reqs_broken/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-21 10:58:17.000000 ansible-compat-4.1.5/examples/reqs_broken/requirements.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:58:43.361724 ansible-compat-4.1.5/examples/reqs_v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-21 10:58:17.000000 ansible-compat-4.1.5/examples/reqs_v1/requirements.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:58:43.361724 ansible-compat-4.1.5/examples/reqs_v2/
+-rw-r--r--   0 runner    (1001) docker     (123)     7615 2023-07-21 10:58:17.000000 ansible-compat-4.1.5/examples/reqs_v2/community-molecule-0.1.0.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-21 10:58:17.000000 ansible-compat-4.1.5/examples/reqs_v2/requirements.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-07-21 10:58:17.000000 ansible-compat-4.1.5/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-07-21 10:58:17.000000 ansible-compat-4.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-21 10:58:17.000000 ansible-compat-4.1.5/readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     6281 2023-07-21 10:58:17.000000 ansible-compat-4.1.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 10:58:43.393725 ansible-compat-4.1.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:58:43.325724 ansible-compat-4.1.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:58:43.369725 ansible-compat-4.1.5/src/ansible_compat/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-21 10:58:17.000000 ansible-compat-4.1.5/src/ansible_compat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-21 10:58:43.000000 ansible-compat-4.1.5/src/ansible_compat/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16108 2023-07-21 10:58:17.000000 ansible-compat-4.1.5/src/ansible_compat/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-07-21 10:58:17.000000 ansible-compat-4.1.5/src/ansible_compat/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-07-21 10:58:17.000000 ansible-compat-4.1.5/src/ansible_compat/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-21 10:58:17.000000 ansible-compat-4.1.5/src/ansible_compat/loaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-21 10:58:17.000000 ansible-compat-4.1.5/src/ansible_compat/ports.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-21 10:58:17.000000 ansible-compat-4.1.5/src/ansible_compat/prerun.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 10:58:17.000000 ansible-compat-4.1.5/src/ansible_compat/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    35618 2023-07-21 10:58:17.000000 ansible-compat-4.1.5/src/ansible_compat/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-07-21 10:58:17.000000 ansible-compat-4.1.5/src/ansible_compat/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-07-21 10:58:17.000000 ansible-compat-4.1.5/src/ansible_compat/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:58:43.373725 ansible-compat-4.1.5/src/ansible_compat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-07-21 10:58:43.000000 ansible-compat-4.1.5/src/ansible_compat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-07-21 10:58:43.000000 ansible-compat-4.1.5/src/ansible_compat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 10:58:43.000000 ansible-compat-4.1.5/src/ansible_compat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-21 10:58:43.000000 ansible-compat-4.1.5/src/ansible_compat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-21 10:58:43.000000 ansible-compat-4.1.5/src/ansible_compat.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:58:43.377725 ansible-compat-4.1.5/test/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-21 10:58:17.000000 ansible-compat-4.1.5/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:58:43.381725 ansible-compat-4.1.5/test/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-21 10:58:17.000000 ansible-compat-4.1.5/test/assets/requirements-invalid-collection.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-21 10:58:17.000000 ansible-compat-4.1.5/test/assets/requirements-invalid-role.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-21 10:58:17.000000 ansible-compat-4.1.5/test/assets/validate0_data.json
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-07-21 10:58:17.000000 ansible-compat-4.1.5/test/assets/validate0_expected.json
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-21 10:58:17.000000 ansible-compat-4.1.5/test/assets/validate0_schema.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:58:43.325724 ansible-compat-4.1.5/test/collections/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:58:43.381725 ansible-compat-4.1.5/test/collections/acme.broken/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-21 10:58:17.000000 ansible-compat-4.1.5/test/collections/acme.broken/galaxy.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:58:43.381725 ansible-compat-4.1.5/test/collections/acme.goodies/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-21 10:58:17.000000 ansible-compat-4.1.5/test/collections/acme.goodies/galaxy.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:58:43.329724 ansible-compat-4.1.5/test/collections/acme.goodies/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:58:43.385725 ansible-compat-4.1.5/test/collections/acme.goodies/molecule/default/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-21 10:58:17.000000 ansible-compat-4.1.5/test/collections/acme.goodies/molecule/default/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-21 10:58:17.000000 ansible-compat-4.1.5/test/collections/acme.goodies/molecule/default/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:58:43.329724 ansible-compat-4.1.5/test/collections/acme.goodies/roles/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:58:43.329724 ansible-compat-4.1.5/test/collections/acme.goodies/roles/baz/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:58:43.329724 ansible-compat-4.1.5/test/collections/acme.goodies/roles/baz/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:58:43.385725 ansible-compat-4.1.5/test/collections/acme.goodies/roles/baz/molecule/deep_scenario/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-21 10:58:17.000000 ansible-compat-4.1.5/test/collections/acme.goodies/roles/baz/molecule/deep_scenario/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-21 10:58:17.000000 ansible-compat-4.1.5/test/collections/acme.goodies/roles/baz/molecule/deep_scenario/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:58:43.385725 ansible-compat-4.1.5/test/collections/acme.goodies/roles/baz/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-21 10:58:17.000000 ansible-compat-4.1.5/test/collections/acme.goodies/roles/baz/tasks/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:58:43.389725 ansible-compat-4.1.5/test/collections/acme.goodies/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-21 10:58:17.000000 ansible-compat-4.1.5/test/collections/acme.goodies/tests/requirements.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-21 10:58:17.000000 ansible-compat-4.1.5/test/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:58:43.337724 ansible-compat-4.1.5/test/roles/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:58:43.389725 ansible-compat-4.1.5/test/roles/acme.missing_deps/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:58:43.389725 ansible-compat-4.1.5/test/roles/acme.missing_deps/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-21 10:58:17.000000 ansible-compat-4.1.5/test/roles/acme.missing_deps/meta/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-21 10:58:17.000000 ansible-compat-4.1.5/test/roles/acme.missing_deps/requirements.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:58:43.333724 ansible-compat-4.1.5/test/roles/acme.sample2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:58:43.389725 ansible-compat-4.1.5/test/roles/acme.sample2/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-21 10:58:17.000000 ansible-compat-4.1.5/test/roles/acme.sample2/meta/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:58:43.333724 ansible-compat-4.1.5/test/roles/ansible-role-sample/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:58:43.389725 ansible-compat-4.1.5/test/roles/ansible-role-sample/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-21 10:58:17.000000 ansible-compat-4.1.5/test/roles/ansible-role-sample/meta/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:58:43.337724 ansible-compat-4.1.5/test/roles/sample3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:58:43.389725 ansible-compat-4.1.5/test/roles/sample3/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-21 10:58:17.000000 ansible-compat-4.1.5/test/roles/sample3/meta/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:58:43.337724 ansible-compat-4.1.5/test/roles/sample4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:58:43.393725 ansible-compat-4.1.5/test/roles/sample4/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-21 10:58:17.000000 ansible-compat-4.1.5/test/roles/sample4/meta/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-21 10:58:17.000000 ansible-compat-4.1.5/test/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-07-21 10:58:17.000000 ansible-compat-4.1.5/test/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-21 10:58:17.000000 ansible-compat-4.1.5/test/test_configuration_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-21 10:58:17.000000 ansible-compat-4.1.5/test/test_loaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-21 10:58:17.000000 ansible-compat-4.1.5/test/test_prerun.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27640 2023-07-21 10:58:17.000000 ansible-compat-4.1.5/test/test_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-21 10:58:17.000000 ansible-compat-4.1.5/test/test_runtime_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-07-21 10:58:17.000000 ansible-compat-4.1.5/test/test_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:58:43.393725 ansible-compat-4.1.5/tools/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      248 2023-07-21 10:58:17.000000 ansible-compat-4.1.5/tools/get-version.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      240 2023-07-21 10:58:17.000000 ansible-compat-4.1.5/tools/update-version.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     4541 2023-07-21 10:58:17.000000 ansible-compat-4.1.5/tox.ini
```

### Comparing `ansible-compat-4.1.4.dev0/.github/dependabot.yml` & `ansible-compat-4.1.5/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.4.dev0/.github/workflows/release.yml` & `ansible-compat-4.1.5/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.4.dev0/.github/workflows/tox.yml` & `ansible-compat-4.1.5/.github/workflows/tox.yml`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.4.dev0/.gitignore` & `ansible-compat-4.1.5/.gitignore`

 * *Files 11% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 # C extensions
 *.so
 
 # Distribution / packaging
 .Python
 build/
 develop-eggs/
+dist/
 downloads/
 eggs/
 .eggs/
 lib/
 lib64/
 parts/
 sdist/
@@ -126,7 +127,10 @@
 dmypy.json
 
 # Pyre type checker
 .pyre/
 .test-results
 *.lcov
 ansible_collections
+
+# Generated by setuptools-scm
+src/ansible_compat/_version.py
```

### Comparing `ansible-compat-4.1.4.dev0/.packit.yaml` & `ansible-compat-4.1.5/.packit.yaml`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.4.dev0/.pre-commit-config.yaml` & `ansible-compat-4.1.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.4.dev0/.readthedocs.yml` & `ansible-compat-4.1.5/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.4.dev0/.vscode/settings.json` & `ansible-compat-4.1.5/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.4.dev0/LICENSE` & `ansible-compat-4.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.4.dev0/PKG-INFO` & `ansible-compat-4.1.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansible-compat
-Version: 4.1.4.dev0
+Version: 4.1.5
 Summary: Ansible compatibility goodies
 Author-email: Sorin Sbarnea <ssbarnea@redhat.com>
 Maintainer-email: Sorin Sbarnea <ssbarnea@redhat.com>
 License: MIT
 Project-URL: homepage, https://github.com/ansible/ansible-compat
 Project-URL: documentation, https://ansible-compat.readthedocs.io/
 Project-URL: repository, https://github.com/ansible/ansible-compat
```

### Comparing `ansible-compat-4.1.4.dev0/README.md` & `ansible-compat-4.1.5/README.md`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.4.dev0/docs/images/favicon.ico` & `ansible-compat-4.1.5/docs/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.4.dev0/docs/images/logo.png` & `ansible-compat-4.1.5/docs/images/logo.png`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.4.dev0/docs/images/logo.svg` & `ansible-compat-4.1.5/docs/images/logo.svg`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.4.dev0/examples/reqs_v2/community-molecule-0.1.0.tar.gz` & `ansible-compat-4.1.5/examples/reqs_v2/community-molecule-0.1.0.tar.gz`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.4.dev0/mkdocs.yml` & `ansible-compat-4.1.5/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.4.dev0/pyproject.toml` & `ansible-compat-4.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [build-system]
 requires = [
-  "setuptools >= 61.0", # PEP-621
-  "setuptools_scm[toml] >= 7.0.0",
+  "setuptools >= 65.3.0", # required by pyproject+setuptools_scm integration and editable installs
+  "setuptools_scm[toml] >= 7.0.5", # required for "no-local-version" scheme
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 # https://peps.python.org/pep-0621/#readme
 requires-python = ">=3.9"
 dynamic = ["version"]
@@ -151,7 +151,8 @@
 known-third-party = ["packaging"]
 
 [tool.ruff.per-file-ignores]
 "test/**/*.py" = ["SLF001", "S101", "FBT001"]
 
 [tool.setuptools_scm]
 local_scheme = "no-local-version"
+write_to = "src/ansible_compat/_version.py"
```

### Comparing `ansible-compat-4.1.4.dev0/requirements.txt` & `ansible-compat-4.1.5/requirements.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #
 # This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
-#    pip-compile --extra=docs --extra=test --output-file=requirements.txt --resolver=backtracking --strip-extras --unsafe-package=ansible-core --unsafe-package=resolvelib --unsafe-package=typing_extensions pyproject.toml
+#    pip-compile --extra=docs --extra=test --output-file=requirements.txt --strip-extras --unsafe-package=ansible-core --unsafe-package=resolvelib --unsafe-package=typing_extensions pyproject.toml
 #
 argparse-manpage==4.2
     # via ansible-compat (pyproject.toml)
 attrs==23.1.0
     # via jsonschema
 beautifulsoup4==4.12.1
     # via
```

### Comparing `ansible-compat-4.1.4.dev0/src/ansible_compat/config.py` & `ansible-compat-4.1.5/src/ansible_compat/config.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.4.dev0/src/ansible_compat/constants.py` & `ansible-compat-4.1.5/src/ansible_compat/constants.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.4.dev0/src/ansible_compat/errors.py` & `ansible-compat-4.1.5/src/ansible_compat/errors.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.4.dev0/src/ansible_compat/loaders.py` & `ansible-compat-4.1.5/src/ansible_compat/loaders.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.4.dev0/src/ansible_compat/prerun.py` & `ansible-compat-4.1.5/src/ansible_compat/prerun.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.4.dev0/src/ansible_compat/runtime.py` & `ansible-compat-4.1.5/src/ansible_compat/runtime.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.4.dev0/src/ansible_compat/schema.py` & `ansible-compat-4.1.5/src/ansible_compat/schema.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.4.dev0/src/ansible_compat/types.py` & `ansible-compat-4.1.5/src/ansible_compat/types.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.4.dev0/src/ansible_compat.egg-info/PKG-INFO` & `ansible-compat-4.1.5/src/ansible_compat.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansible-compat
-Version: 4.1.4.dev0
+Version: 4.1.5
 Summary: Ansible compatibility goodies
 Author-email: Sorin Sbarnea <ssbarnea@redhat.com>
 Maintainer-email: Sorin Sbarnea <ssbarnea@redhat.com>
 License: MIT
 Project-URL: homepage, https://github.com/ansible/ansible-compat
 Project-URL: documentation, https://ansible-compat.readthedocs.io/
 Project-URL: repository, https://github.com/ansible/ansible-compat
```

### Comparing `ansible-compat-4.1.4.dev0/src/ansible_compat.egg-info/SOURCES.txt` & `ansible-compat-4.1.5/src/ansible_compat.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+.git_archival.txt
+.gitattributes
 .gitignore
 .packit.yaml
 .pre-commit-config.yaml
 .prettierignore
 .prettierrc.yaml
 .readthedocs.yml
 .yamllint
@@ -30,14 +32,15 @@
 docs/images/logo.png
 docs/images/logo.svg
 examples/reqs_broken/requirements.yml
 examples/reqs_v1/requirements.yml
 examples/reqs_v2/community-molecule-0.1.0.tar.gz
 examples/reqs_v2/requirements.yml
 src/ansible_compat/__init__.py
+src/ansible_compat/_version.py
 src/ansible_compat/config.py
 src/ansible_compat/constants.py
 src/ansible_compat/errors.py
 src/ansible_compat/loaders.py
 src/ansible_compat/ports.py
 src/ansible_compat/prerun.py
 src/ansible_compat/py.typed
```

### Comparing `ansible-compat-4.1.4.dev0/test/assets/validate0_expected.json` & `ansible-compat-4.1.5/test/assets/validate0_expected.json`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.4.dev0/test/collections/acme.goodies/galaxy.yml` & `ansible-compat-4.1.5/test/collections/acme.goodies/galaxy.yml`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.4.dev0/test/conftest.py` & `ansible-compat-4.1.5/test/conftest.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.4.dev0/test/test_config.py` & `ansible-compat-4.1.5/test/test_config.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.4.dev0/test/test_runtime.py` & `ansible-compat-4.1.5/test/test_runtime.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.4.dev0/test/test_runtime_example.py` & `ansible-compat-4.1.5/test/test_runtime_example.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.4.dev0/test/test_schema.py` & `ansible-compat-4.1.5/test/test_schema.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.4.dev0/tox.ini` & `ansible-compat-4.1.5/tox.ini`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,17 @@
   lint
   pkg
   docs
   # matrix assumed current (implicit) is 2.13:
   py{39,310,311}{,-devel,-ansible212,-ansible213,-ansible214,-ansible215}
 isolated_build = true
 skip_missing_interpreters = True
+requires =
+  tox >= 4.6.3
+  setuptools >= 65.3.0 # editable installs
 
 [testenv]
 description =
   Run the tests with {basepython}
   devel: ansible devel branch
   ansible212: ansible-core 2.12
   ansible213: ansible-core 2.13
@@ -20,15 +23,15 @@
 
 deps =
   ansible212: ansible-core>=2.12,<2.13
   ansible213: ansible-core>=2.13,<2.14
   ansible214: ansible-core>=2.14,<2.15
   ansible215: ansible-core>=2.15,<2.16
 
-  devel: ansible-core @ git+https://github.com/ansible/ansible.git  # GPLv3+
+  devel: ansible-core @ git+https://github.com/ansible/ansible.git@c5d18c39d81e2b3b10856b2fb76747230e4fac4a  # GPLv3+
   # avoid installing ansible-core on -devel envs:
   !devel: ansible-core
 extras =
   test
 
 commands =
   sh -c "ansible --version | head -n 1"
```

