# Comparing `tmp/mse_cli-1.0.0.tar.gz` & `tmp/mse_cli-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mse_cli-1.0.0.tar", last modified: Tue Jul 18 12:29:00 2023, max compression
+gzip compressed data, was "mse_cli-1.0.1.tar", last modified: Fri Jul 21 11:06:39 2023, max compression
```

## Comparing `mse_cli-1.0.0.tar` & `mse_cli-1.0.1.tar`

### file list

```diff
@@ -1,122 +1,122 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:29:00.521840 mse_cli-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    16238 2023-07-18 12:29:00.521840 mse_cli-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15625 2023-07-18 12:28:30.000000 mse_cli-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:29:00.489840 mse_cli-1.0.0/mse_cli/
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-07-18 12:28:30.000000 mse_cli-1.0.0/mse_cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:29:00.493840 mse_cli-1.0.0/mse_cli/cloud/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-18 12:28:30.000000 mse_cli-1.0.0/mse_cli/cloud/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:29:00.497840 mse_cli-1.0.0/mse_cli/cloud/api/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-18 12:28:30.000000 mse_cli-1.0.0/mse_cli/cloud/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-07-18 12:28:30.000000 mse_cli-1.0.0/mse_cli/cloud/api/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     6505 2023-07-18 12:28:30.000000 mse_cli-1.0.0/mse_cli/cloud/api/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-18 12:28:30.000000 mse_cli-1.0.0/mse_cli/cloud/api/hardware.py
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-07-18 12:28:30.000000 mse_cli-1.0.0/mse_cli/cloud/api/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-07-18 12:28:30.000000 mse_cli-1.0.0/mse_cli/cloud/api/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-18 12:28:30.000000 mse_cli-1.0.0/mse_cli/cloud/api/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:29:00.501840 mse_cli-1.0.0/mse_cli/cloud/command/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-18 12:28:30.000000 mse_cli-1.0.0/mse_cli/cloud/command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-07-18 12:28:30.000000 mse_cli-1.0.0/mse_cli/cloud/command/context.py
--rw-r--r--   0 runner    (1001) docker     (123)    10978 2023-07-18 12:28:30.000000 mse_cli-1.0.0/mse_cli/cloud/command/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)     7710 2023-07-18 12:28:30.000000 mse_cli-1.0.0/mse_cli/cloud/command/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-07-18 12:28:30.000000 mse_cli-1.0.0/mse_cli/cloud/command/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-07-18 12:28:30.000000 mse_cli-1.0.0/mse_cli/cloud/command/list_all.py
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-07-18 12:28:30.000000 mse_cli-1.0.0/mse_cli/cloud/command/localtest.py
--rw-r--r--   0 runner    (1001) docker     (123)     7515 2023-07-18 12:28:30.000000 mse_cli-1.0.0/mse_cli/cloud/command/login.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-18 12:28:30.000000 mse_cli-1.0.0/mse_cli/cloud/command/logout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-07-18 12:28:30.000000 mse_cli-1.0.0/mse_cli/cloud/command/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-07-18 12:28:30.000000 mse_cli-1.0.0/mse_cli/cloud/command/scaffold.py
--rw-r--r--   0 runner    (1001) docker     (123)     6417 2023-07-18 12:28:30.000000 mse_cli-1.0.0/mse_cli/cloud/command/status.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-07-18 12:28:30.000000 mse_cli-1.0.0/mse_cli/cloud/command/stop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-07-18 12:28:30.000000 mse_cli-1.0.0/mse_cli/cloud/command/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-07-18 12:28:30.000000 mse_cli-1.0.0/mse_cli/cloud/command/verify.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:29:00.501840 mse_cli-1.0.0/mse_cli/cloud/model/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-18 12:28:30.000000 mse_cli-1.0.0/mse_cli/cloud/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9162 2023-07-18 12:28:30.000000 mse_cli-1.0.0/mse_cli/cloud/model/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-07-18 12:28:30.000000 mse_cli-1.0.0/mse_cli/cloud/model/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-18 12:28:30.000000 mse_cli-1.0.0/mse_cli/color.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:29:00.501840 mse_cli-1.0.0/mse_cli/common/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-18 12:28:30.000000 mse_cli-1.0.0/mse_cli/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6362 2023-07-18 12:28:30.000000 mse_cli-1.0.0/mse_cli/common/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:29:00.505840 mse_cli-1.0.0/mse_cli/core/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-18 12:28:30.000000 mse_cli-1.0.0/mse_cli/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-07-18 12:28:30.000000 mse_cli-1.0.0/mse_cli/core/base64.py
--rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-07-18 12:28:30.000000 mse_cli-1.0.0/mse_cli/core/bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-18 12:28:30.000000 mse_cli-1.0.0/mse_cli/core/clock_tick.py
--rw-r--r--   0 runner    (1001) docker     (123)    10440 2023-07-18 12:28:30.000000 mse_cli-1.0.0/mse_cli/core/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-07-18 12:28:30.000000 mse_cli-1.0.0/mse_cli/core/enclave.py
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-07-18 12:28:30.000000 mse_cli-1.0.0/mse_cli/core/fs.py
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-07-18 12:28:30.000000 mse_cli-1.0.0/mse_cli/core/ignore_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-07-18 12:28:30.000000 mse_cli-1.0.0/mse_cli/core/no_sgx_docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-07-18 12:28:30.000000 mse_cli-1.0.0/mse_cli/core/sgx_docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-07-18 12:28:30.000000 mse_cli-1.0.0/mse_cli/core/spinner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-07-18 12:28:30.000000 mse_cli-1.0.0/mse_cli/core/test_docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-07-18 12:28:30.000000 mse_cli-1.0.0/mse_cli/error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:29:00.505840 mse_cli-1.0.0/mse_cli/home/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-18 12:28:30.000000 mse_cli-1.0.0/mse_cli/home/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:29:00.505840 mse_cli-1.0.0/mse_cli/home/command/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-18 12:28:30.000000 mse_cli-1.0.0/mse_cli/home/command/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:29:00.509840 mse_cli-1.0.0/mse_cli/home/command/code_provider/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-18 12:28:30.000000 mse_cli-1.0.0/mse_cli/home/command/code_provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-07-18 12:28:30.000000 mse_cli-1.0.0/mse_cli/home/command/code_provider/decrypt.py
--rw-r--r--   0 runner    (1001) docker     (123)     5053 2023-07-18 12:28:30.000000 mse_cli-1.0.0/mse_cli/home/command/code_provider/localtest.py
--rw-r--r--   0 runner    (1001) docker     (123)     7665 2023-07-18 12:28:30.000000 mse_cli-1.0.0/mse_cli/home/command/code_provider/package.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-07-18 12:28:30.000000 mse_cli-1.0.0/mse_cli/home/command/code_provider/scaffold.py
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-07-18 12:28:30.000000 mse_cli-1.0.0/mse_cli/home/command/code_provider/seal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-07-18 12:28:30.000000 mse_cli-1.0.0/mse_cli/home/command/code_provider/verify.py
--rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-07-18 12:28:30.000000 mse_cli-1.0.0/mse_cli/home/command/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:29:00.509840 mse_cli-1.0.0/mse_cli/home/command/sgx_operator/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-18 12:28:30.000000 mse_cli-1.0.0/mse_cli/home/command/sgx_operator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4691 2023-07-18 12:28:30.000000 mse_cli-1.0.0/mse_cli/home/command/sgx_operator/evidence.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-18 12:28:30.000000 mse_cli-1.0.0/mse_cli/home/command/sgx_operator/list_all.py
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-18 12:28:30.000000 mse_cli-1.0.0/mse_cli/home/command/sgx_operator/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-18 12:28:30.000000 mse_cli-1.0.0/mse_cli/home/command/sgx_operator/restart.py
--rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-07-18 12:28:30.000000 mse_cli-1.0.0/mse_cli/home/command/sgx_operator/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-07-18 12:28:30.000000 mse_cli-1.0.0/mse_cli/home/command/sgx_operator/spawn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-07-18 12:28:30.000000 mse_cli-1.0.0/mse_cli/home/command/sgx_operator/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-07-18 12:28:30.000000 mse_cli-1.0.0/mse_cli/home/command/sgx_operator/stop.py
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-07-18 12:28:30.000000 mse_cli-1.0.0/mse_cli/home/command/sgx_operator/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:29:00.513840 mse_cli-1.0.0/mse_cli/home/model/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-18 12:28:30.000000 mse_cli-1.0.0/mse_cli/home/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-07-18 12:28:30.000000 mse_cli-1.0.0/mse_cli/home/model/evidence.py
--rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-07-18 12:28:30.000000 mse_cli-1.0.0/mse_cli/home/model/package.py
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-07-18 12:28:30.000000 mse_cli-1.0.0/mse_cli/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     5115 2023-07-18 12:28:30.000000 mse_cli-1.0.0/mse_cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:29:00.513840 mse_cli-1.0.0/mse_cli/template/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-18 12:28:30.000000 mse_cli-1.0.0/mse_cli/template/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-07-18 12:28:30.000000 mse_cli-1.0.0/mse_cli/template/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-18 12:28:30.000000 mse_cli-1.0.0/mse_cli/template/mse.toml.template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:29:00.513840 mse_cli-1.0.0/mse_cli/template/mse_src/
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-07-18 12:28:30.000000 mse_cli-1.0.0/mse_cli/template/mse_src/app.py.template
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-18 12:28:30.000000 mse_cli-1.0.0/mse_cli/template/mse_src/dotmseignore
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-18 12:28:30.000000 mse_cli-1.0.0/mse_cli/template/secrets.json
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-18 12:28:30.000000 mse_cli-1.0.0/mse_cli/template/secrets_to_seal.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:29:00.513840 mse_cli-1.0.0/mse_cli/template/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-07-18 12:28:30.000000 mse_cli-1.0.0/mse_cli/template/tests/conftest.py.template
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-07-18 12:28:30.000000 mse_cli-1.0.0/mse_cli/template/tests/test_app.py.template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:29:00.493840 mse_cli-1.0.0/mse_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16238 2023-07-18 12:29:00.000000 mse_cli-1.0.0/mse_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-07-18 12:29:00.000000 mse_cli-1.0.0/mse_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 12:29:00.000000 mse_cli-1.0.0/mse_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-18 12:29:00.000000 mse_cli-1.0.0/mse_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-18 12:29:00.000000 mse_cli-1.0.0/mse_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-18 12:29:00.000000 mse_cli-1.0.0/mse_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 12:29:00.000000 mse_cli-1.0.0/mse_cli.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-07-18 12:29:00.521840 mse_cli-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-07-18 12:28:30.000000 mse_cli-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:29:00.521840 mse_cli-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-18 12:28:30.000000 mse_cli-1.0.0/tests/test_base64.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-07-18 12:28:30.000000 mse_cli-1.0.0/tests/test_boostrap.py
--rw-r--r--   0 runner    (1001) docker     (123)    16332 2023-07-18 12:28:30.000000 mse_cli-1.0.0/tests/test_cli_cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     7476 2023-07-18 12:28:30.000000 mse_cli-1.0.0/tests/test_cli_cloud_error.py
--rw-r--r--   0 runner    (1001) docker     (123)    21005 2023-07-18 12:28:30.000000 mse_cli-1.0.0/tests/test_cli_home.py
--rw-r--r--   0 runner    (1001) docker     (123)    12426 2023-07-18 12:28:30.000000 mse_cli-1.0.0/tests/test_conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5889 2023-07-18 12:28:30.000000 mse_cli-1.0.0/tests/test_context.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-18 12:28:30.000000 mse_cli-1.0.0/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-18 12:28:30.000000 mse_cli-1.0.0/tests/test_ignore_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    28635 2023-07-18 12:28:30.000000 mse_cli-1.0.0/tests/test_model_evidence.py
--rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-07-18 12:28:30.000000 mse_cli-1.0.0/tests/test_model_package.py
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-07-18 12:28:30.000000 mse_cli-1.0.0/tests/test_no_sgx_docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     5514 2023-07-18 12:28:30.000000 mse_cli-1.0.0/tests/test_sgx_docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-07-18 12:28:30.000000 mse_cli-1.0.0/tests/test_test_docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-07-18 12:28:30.000000 mse_cli-1.0.0/tests/test_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-18 12:28:30.000000 mse_cli-1.0.0/tests/test_user_conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:06:39.804614 mse_cli-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    16238 2023-07-21 11:06:39.804614 mse_cli-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15625 2023-07-21 11:06:02.000000 mse_cli-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:06:39.768614 mse_cli-1.0.1/mse_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-07-21 11:06:02.000000 mse_cli-1.0.1/mse_cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:06:39.772614 mse_cli-1.0.1/mse_cli/cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-21 11:06:02.000000 mse_cli-1.0.1/mse_cli/cloud/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:06:39.776614 mse_cli-1.0.1/mse_cli/cloud/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-21 11:06:02.000000 mse_cli-1.0.1/mse_cli/cloud/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-07-21 11:06:02.000000 mse_cli-1.0.1/mse_cli/cloud/api/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6505 2023-07-21 11:06:02.000000 mse_cli-1.0.1/mse_cli/cloud/api/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-21 11:06:02.000000 mse_cli-1.0.1/mse_cli/cloud/api/hardware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-07-21 11:06:02.000000 mse_cli-1.0.1/mse_cli/cloud/api/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-07-21 11:06:02.000000 mse_cli-1.0.1/mse_cli/cloud/api/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-21 11:06:02.000000 mse_cli-1.0.1/mse_cli/cloud/api/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:06:39.780614 mse_cli-1.0.1/mse_cli/cloud/command/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-21 11:06:02.000000 mse_cli-1.0.1/mse_cli/cloud/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-07-21 11:06:02.000000 mse_cli-1.0.1/mse_cli/cloud/command/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11293 2023-07-21 11:06:02.000000 mse_cli-1.0.1/mse_cli/cloud/command/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7710 2023-07-21 11:06:02.000000 mse_cli-1.0.1/mse_cli/cloud/command/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-07-21 11:06:02.000000 mse_cli-1.0.1/mse_cli/cloud/command/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-07-21 11:06:02.000000 mse_cli-1.0.1/mse_cli/cloud/command/list_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-07-21 11:06:02.000000 mse_cli-1.0.1/mse_cli/cloud/command/localtest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7515 2023-07-21 11:06:02.000000 mse_cli-1.0.1/mse_cli/cloud/command/login.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-21 11:06:02.000000 mse_cli-1.0.1/mse_cli/cloud/command/logout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-07-21 11:06:02.000000 mse_cli-1.0.1/mse_cli/cloud/command/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-07-21 11:06:02.000000 mse_cli-1.0.1/mse_cli/cloud/command/scaffold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6417 2023-07-21 11:06:02.000000 mse_cli-1.0.1/mse_cli/cloud/command/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-07-21 11:06:02.000000 mse_cli-1.0.1/mse_cli/cloud/command/stop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-07-21 11:06:02.000000 mse_cli-1.0.1/mse_cli/cloud/command/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-07-21 11:06:02.000000 mse_cli-1.0.1/mse_cli/cloud/command/verify.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:06:39.784614 mse_cli-1.0.1/mse_cli/cloud/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-21 11:06:02.000000 mse_cli-1.0.1/mse_cli/cloud/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9162 2023-07-21 11:06:02.000000 mse_cli-1.0.1/mse_cli/cloud/model/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-07-21 11:06:02.000000 mse_cli-1.0.1/mse_cli/cloud/model/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-21 11:06:02.000000 mse_cli-1.0.1/mse_cli/color.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:06:39.784614 mse_cli-1.0.1/mse_cli/common/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-21 11:06:02.000000 mse_cli-1.0.1/mse_cli/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6823 2023-07-21 11:06:02.000000 mse_cli-1.0.1/mse_cli/common/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:06:39.788614 mse_cli-1.0.1/mse_cli/core/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-21 11:06:02.000000 mse_cli-1.0.1/mse_cli/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-07-21 11:06:02.000000 mse_cli-1.0.1/mse_cli/core/base64.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-07-21 11:06:02.000000 mse_cli-1.0.1/mse_cli/core/bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-21 11:06:02.000000 mse_cli-1.0.1/mse_cli/core/clock_tick.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10440 2023-07-21 11:06:02.000000 mse_cli-1.0.1/mse_cli/core/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-07-21 11:06:02.000000 mse_cli-1.0.1/mse_cli/core/enclave.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-07-21 11:06:02.000000 mse_cli-1.0.1/mse_cli/core/fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-07-21 11:06:02.000000 mse_cli-1.0.1/mse_cli/core/ignore_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-07-21 11:06:02.000000 mse_cli-1.0.1/mse_cli/core/no_sgx_docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-07-21 11:06:02.000000 mse_cli-1.0.1/mse_cli/core/sgx_docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-07-21 11:06:02.000000 mse_cli-1.0.1/mse_cli/core/spinner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-07-21 11:06:02.000000 mse_cli-1.0.1/mse_cli/core/test_docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-07-21 11:06:02.000000 mse_cli-1.0.1/mse_cli/error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:06:39.788614 mse_cli-1.0.1/mse_cli/home/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-21 11:06:02.000000 mse_cli-1.0.1/mse_cli/home/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:06:39.788614 mse_cli-1.0.1/mse_cli/home/command/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-21 11:06:02.000000 mse_cli-1.0.1/mse_cli/home/command/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:06:39.792614 mse_cli-1.0.1/mse_cli/home/command/code_provider/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-21 11:06:02.000000 mse_cli-1.0.1/mse_cli/home/command/code_provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-07-21 11:06:02.000000 mse_cli-1.0.1/mse_cli/home/command/code_provider/decrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5219 2023-07-21 11:06:02.000000 mse_cli-1.0.1/mse_cli/home/command/code_provider/localtest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7665 2023-07-21 11:06:02.000000 mse_cli-1.0.1/mse_cli/home/command/code_provider/package.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-07-21 11:06:02.000000 mse_cli-1.0.1/mse_cli/home/command/code_provider/scaffold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-07-21 11:06:02.000000 mse_cli-1.0.1/mse_cli/home/command/code_provider/seal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-07-21 11:06:02.000000 mse_cli-1.0.1/mse_cli/home/command/code_provider/verify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-07-21 11:06:02.000000 mse_cli-1.0.1/mse_cli/home/command/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:06:39.796614 mse_cli-1.0.1/mse_cli/home/command/sgx_operator/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-21 11:06:02.000000 mse_cli-1.0.1/mse_cli/home/command/sgx_operator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4691 2023-07-21 11:06:02.000000 mse_cli-1.0.1/mse_cli/home/command/sgx_operator/evidence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-21 11:06:02.000000 mse_cli-1.0.1/mse_cli/home/command/sgx_operator/list_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-21 11:06:02.000000 mse_cli-1.0.1/mse_cli/home/command/sgx_operator/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-21 11:06:02.000000 mse_cli-1.0.1/mse_cli/home/command/sgx_operator/restart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-07-21 11:06:02.000000 mse_cli-1.0.1/mse_cli/home/command/sgx_operator/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-07-21 11:06:02.000000 mse_cli-1.0.1/mse_cli/home/command/sgx_operator/spawn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-07-21 11:06:02.000000 mse_cli-1.0.1/mse_cli/home/command/sgx_operator/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-07-21 11:06:02.000000 mse_cli-1.0.1/mse_cli/home/command/sgx_operator/stop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-07-21 11:06:02.000000 mse_cli-1.0.1/mse_cli/home/command/sgx_operator/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:06:39.796614 mse_cli-1.0.1/mse_cli/home/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-21 11:06:02.000000 mse_cli-1.0.1/mse_cli/home/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-07-21 11:06:02.000000 mse_cli-1.0.1/mse_cli/home/model/evidence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-07-21 11:06:02.000000 mse_cli-1.0.1/mse_cli/home/model/package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-07-21 11:06:02.000000 mse_cli-1.0.1/mse_cli/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5115 2023-07-21 11:06:02.000000 mse_cli-1.0.1/mse_cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:06:39.800614 mse_cli-1.0.1/mse_cli/template/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-21 11:06:02.000000 mse_cli-1.0.1/mse_cli/template/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-07-21 11:06:02.000000 mse_cli-1.0.1/mse_cli/template/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-21 11:06:02.000000 mse_cli-1.0.1/mse_cli/template/mse.toml.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:06:39.800614 mse_cli-1.0.1/mse_cli/template/mse_src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-07-21 11:06:02.000000 mse_cli-1.0.1/mse_cli/template/mse_src/app.py.template
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-21 11:06:02.000000 mse_cli-1.0.1/mse_cli/template/mse_src/dotmseignore
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-21 11:06:02.000000 mse_cli-1.0.1/mse_cli/template/secrets.json
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-21 11:06:02.000000 mse_cli-1.0.1/mse_cli/template/secrets_to_seal.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:06:39.800614 mse_cli-1.0.1/mse_cli/template/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-07-21 11:06:02.000000 mse_cli-1.0.1/mse_cli/template/tests/conftest.py.template
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-07-21 11:06:02.000000 mse_cli-1.0.1/mse_cli/template/tests/test_app.py.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:06:39.772614 mse_cli-1.0.1/mse_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16238 2023-07-21 11:06:39.000000 mse_cli-1.0.1/mse_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-07-21 11:06:39.000000 mse_cli-1.0.1/mse_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 11:06:39.000000 mse_cli-1.0.1/mse_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-21 11:06:39.000000 mse_cli-1.0.1/mse_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-21 11:06:39.000000 mse_cli-1.0.1/mse_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-21 11:06:39.000000 mse_cli-1.0.1/mse_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 11:06:39.000000 mse_cli-1.0.1/mse_cli.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-07-21 11:06:39.804614 mse_cli-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-07-21 11:06:02.000000 mse_cli-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:06:39.804614 mse_cli-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-21 11:06:02.000000 mse_cli-1.0.1/tests/test_base64.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-07-21 11:06:02.000000 mse_cli-1.0.1/tests/test_boostrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16382 2023-07-21 11:06:02.000000 mse_cli-1.0.1/tests/test_cli_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-07-21 11:06:02.000000 mse_cli-1.0.1/tests/test_cli_cloud_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21075 2023-07-21 11:06:02.000000 mse_cli-1.0.1/tests/test_cli_home.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12426 2023-07-21 11:06:02.000000 mse_cli-1.0.1/tests/test_conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5889 2023-07-21 11:06:02.000000 mse_cli-1.0.1/tests/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-21 11:06:02.000000 mse_cli-1.0.1/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-21 11:06:02.000000 mse_cli-1.0.1/tests/test_ignore_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28635 2023-07-21 11:06:02.000000 mse_cli-1.0.1/tests/test_model_evidence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-07-21 11:06:02.000000 mse_cli-1.0.1/tests/test_model_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-07-21 11:06:02.000000 mse_cli-1.0.1/tests/test_no_sgx_docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5514 2023-07-21 11:06:02.000000 mse_cli-1.0.1/tests/test_sgx_docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-07-21 11:06:02.000000 mse_cli-1.0.1/tests/test_test_docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-07-21 11:06:02.000000 mse_cli-1.0.1/tests/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-21 11:06:02.000000 mse_cli-1.0.1/tests/test_user_conf.py
```

### Comparing `mse_cli-1.0.0/PKG-INFO` & `mse_cli-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mse_cli
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python CLI for Microservice Encryption
 Home-page: https://cosmian.com
 Author: Cosmian Tech
 Author-email: tech@cosmian.com
 License: MIT
 Project-URL: Documentation, https://docs.cosmian.com
 Project-URL: Source, https://github.com/Cosmian/mse-cli
```

### Comparing `mse_cli-1.0.0/README.md` & `mse_cli-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `mse_cli-1.0.0/mse_cli/__init__.py` & `mse_cli-1.0.1/mse_cli/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """MSE module."""
 
 import os
 import sys
 from pathlib import Path
 
-__version__ = "1.0.0"
+__version__ = "1.0.1"
 
 # This directory contains the login information of the user
 # and the context of all its deployments
 _DEFAULT_MSE_CONF_DIR = "~/.config"
 if sys.platform == "win32":
     _DEFAULT_MSE_CONF_DIR = os.getenv("APPDATA")
```

### Comparing `mse_cli-1.0.0/mse_cli/cloud/api/app.py` & `mse_cli-1.0.1/mse_cli/cloud/api/app.py`

 * *Files identical despite different names*

### Comparing `mse_cli-1.0.0/mse_cli/cloud/api/auth.py` & `mse_cli-1.0.1/mse_cli/cloud/api/auth.py`

 * *Files identical despite different names*

### Comparing `mse_cli-1.0.0/mse_cli/cloud/api/project.py` & `mse_cli-1.0.1/mse_cli/cloud/api/project.py`

 * *Files identical despite different names*

### Comparing `mse_cli-1.0.0/mse_cli/cloud/api/types.py` & `mse_cli-1.0.1/mse_cli/cloud/api/types.py`

 * *Files identical despite different names*

### Comparing `mse_cli-1.0.0/mse_cli/cloud/command/context.py` & `mse_cli-1.0.1/mse_cli/cloud/command/context.py`

 * *Files identical despite different names*

### Comparing `mse_cli-1.0.0/mse_cli/cloud/command/deploy.py` & `mse_cli-1.0.1/mse_cli/cloud/command/deploy.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,14 +72,23 @@
     parser.add_argument(
         "--workspace",
         type=Path,
         required=False,
         help="directory to write the temporary files",
     )
 
+    parser.add_argument(
+        "--timeout",
+        type=int,
+        required=False,
+        default=24 * 60,
+        help="stop the deployment if the application does not "
+        "respond after a delay (in min). (Default: 1440 min)",
+    )
+
     parser.set_defaults(func=run)
 
 
 # pylint: disable=too-many-branches,too-many-statements
 def run(args) -> None:
     """Run the subcommand."""
     user_conf = UserConf.load()
@@ -130,15 +139,15 @@
     )
     app = deploy_app(conn, app_conf, tar_path)
 
     LOG.advice(  # type: ignore
         "To follow the app creation, you can run: \n\n\tmse cloud logs %s\n", app.id
     )
 
-    app = wait_app_creation(conn, app.id)
+    app = wait_app_creation(conn, app.id, args.timeout)
 
     context.run(
         app.id,
         enclave_size,
         app.config_domain_name,
         app.expires_at,
         app.ssl_certificate_origin,
@@ -168,15 +177,15 @@
     LOG.info("Sending secret key and decrypting the application code...")
     decrypt_private_data(
         context,
         ssl_private_key=cloud_conf.ssl.private_key_data if cloud_conf.ssl else None,
         app_secrets=cloud_conf.secrets_data,
     )
 
-    app = wait_app_start(conn, app.id)
+    app = wait_app_start(conn, app.id, args.timeout)
 
     LOG.success(  # type: ignore
         "Your application is now deployed and ready to be used on https://%s until %s",
         app.domain_name,
         app.expires_at.astimezone(),
     )
     LOG.info(
@@ -190,39 +199,39 @@
         "The context of this creation can be retrieved using: \n\n\t"
         "mse cloud context --export %s\n",
         app.id,
     )
 
     if app.ssl_certificate_origin == SSLCertificateOrigin.Self:
         LOG.advice(  # type: ignore
-            "You can now test your application doing `mse home test` "
+            "You can now test your application doing `mse cloud test` "
             "or use it as follow: \n\n\tcurl https://%s%s --cacert %s\n",
             app.domain_name,
             app.healthcheck_endpoint,
             context.config_cert_path,
         )
     else:
         LOG.advice(  # type: ignore
-            "You can now test your application doing `mse home test` "
+            "You can now test your application doing `mse cloud test` "
             "or use it as follow: \n\n\tcurl https://%s%s\n",
             app.domain_name,
             app.healthcheck_endpoint,
         )
 
     # Clean up the workspace
     # LOG.info("Cleaning up the temporary workspace...")
     # shutil.rmtree(context.workspace)
 
 
-def wait_app_start(conn: Connection, app_id: UUID) -> App:
+def wait_app_start(conn: Connection, app_id: UUID, timeout: int) -> App:
     """Wait for the app to be started."""
     with Spinner("Waiting for your application to be ready... "):
         clock = ClockTick(
             period=3,
-            timeout=15 * 60,
+            timeout=timeout * 60,
             message="MSE is at high capacity right now! Try again later.",
         )
         while clock.tick():
             app = get_app(conn=conn, app_id=app_id)
 
             if app.status == AppStatus.Spawning:
                 raise AppContainerBadState(
@@ -295,20 +304,20 @@
 
     if not r.ok:
         raise UnexpectedResponse(r.text)
 
     return App.from_dict(r.json())
 
 
-def wait_app_creation(conn: Connection, app_id: UUID) -> App:
+def wait_app_creation(conn: Connection, app_id: UUID, timeout: int) -> App:
     """Wait for the app to be deployed."""
     with Spinner(f"Creating app {app_id}... "):
         clock = ClockTick(
             period=3,
-            timeout=15 * 60,
+            timeout=timeout * 60,
             message="MSE is at high capacity right now! Try again later.",
         )
         while clock.tick():
             app = get_app(conn=conn, app_id=app_id)
 
             if app.status == AppStatus.Initializing:
                 break
```

### Comparing `mse_cli-1.0.0/mse_cli/cloud/command/helpers.py` & `mse_cli-1.0.1/mse_cli/cloud/command/helpers.py`

 * *Files identical despite different names*

### Comparing `mse_cli-1.0.0/mse_cli/cloud/command/init.py` & `mse_cli-1.0.1/mse_cli/cloud/command/init.py`

 * *Files identical despite different names*

### Comparing `mse_cli-1.0.0/mse_cli/cloud/command/list_all.py` & `mse_cli-1.0.1/mse_cli/cloud/command/list_all.py`

 * *Files identical despite different names*

### Comparing `mse_cli-1.0.0/mse_cli/cloud/command/localtest.py` & `mse_cli-1.0.1/mse_cli/cloud/command/localtest.py`

 * *Files 19% similar despite different names*

```diff
@@ -22,14 +22,20 @@
         "--path",
         type=Path,
         required=False,
         metavar="FILE",
         help="path to the MSE app to test (current directory if not set)",
     )
 
+    parser.add_argument(
+        "--no-tests",
+        action="store_true",
+        help="do not run the tests: just start the docker",
+    )
+
     parser.set_defaults(func=run)
 
 
 def run(args) -> None:
     """Run the subcommand."""
     app = AppConf.load(path=args.path)
     cloud_conf = app.cloud_or_raise()
@@ -57,8 +63,9 @@
         client,
         cloud_conf.docker,
         str(uuid.uuid4()),
         docker_config,
         cloud_conf.tests,
         None,
         None,
+        args.no_tests,
     )
```

### Comparing `mse_cli-1.0.0/mse_cli/cloud/command/login.py` & `mse_cli-1.0.1/mse_cli/cloud/command/login.py`

 * *Files identical despite different names*

### Comparing `mse_cli-1.0.0/mse_cli/cloud/command/logout.py` & `mse_cli-1.0.1/mse_cli/cloud/command/logout.py`

 * *Files identical despite different names*

### Comparing `mse_cli-1.0.0/mse_cli/cloud/command/logs.py` & `mse_cli-1.0.1/mse_cli/cloud/command/logs.py`

 * *Files identical despite different names*

### Comparing `mse_cli-1.0.0/mse_cli/cloud/command/scaffold.py` & `mse_cli-1.0.1/mse_cli/cloud/command/scaffold.py`

 * *Files identical despite different names*

### Comparing `mse_cli-1.0.0/mse_cli/cloud/command/status.py` & `mse_cli-1.0.1/mse_cli/cloud/command/status.py`

 * *Files identical despite different names*

### Comparing `mse_cli-1.0.0/mse_cli/cloud/command/stop.py` & `mse_cli-1.0.1/mse_cli/cloud/command/stop.py`

 * *Files identical despite different names*

### Comparing `mse_cli-1.0.0/mse_cli/cloud/command/test.py` & `mse_cli-1.0.1/mse_cli/cloud/command/test.py`

 * *Files identical despite different names*

### Comparing `mse_cli-1.0.0/mse_cli/cloud/command/verify.py` & `mse_cli-1.0.1/mse_cli/cloud/command/verify.py`

 * *Files identical despite different names*

### Comparing `mse_cli-1.0.0/mse_cli/cloud/model/context.py` & `mse_cli-1.0.1/mse_cli/cloud/model/context.py`

 * *Files identical despite different names*

### Comparing `mse_cli-1.0.0/mse_cli/cloud/model/user.py` & `mse_cli-1.0.1/mse_cli/cloud/model/user.py`

 * *Files identical despite different names*

### Comparing `mse_cli-1.0.0/mse_cli/color.py` & `mse_cli-1.0.1/mse_cli/color.py`

 * *Files identical despite different names*

### Comparing `mse_cli-1.0.0/mse_cli/common/helpers.py` & `mse_cli-1.0.1/mse_cli/common/helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -110,32 +110,46 @@
     client,
     docker_name,
     container_name: str,
     docker_config: TestDockerConfig,
     test_path: Path,
     secrets_path: Optional[Path],
     sealed_secrets_path: Optional[Path],
+    ignore_tests: bool = False,
 ):
     """Try to start the app docker to test."""
     success = False
     try:
         container = run_app_test_docker(
             client,
             docker_name,
             container_name,
             docker_config,
             app_config.healthcheck_endpoint,
         )
 
-        success = run_tests(
-            app_config,
-            test_path,
-            secrets_path,
-            sealed_secrets_path,
-        )
+        if not ignore_tests:
+            success = run_tests(
+                app_config,
+                test_path,
+                secrets_path,
+                sealed_secrets_path,
+            )
+        else:
+            LOG.info(
+                "The docker '%s' is started. "
+                "You can now query your application on http://localhost:%s",
+                docker_name,
+                docker_config.port,
+            )
+
+            success = True
+
+            for line in container.logs(stream=True):
+                LOG.info(line.decode("utf-8").strip())
 
     except Exception as exc:
         raise exc
     finally:
         try:
             container = client.containers.get(container_name)
             if not success:
```

### Comparing `mse_cli-1.0.0/mse_cli/core/base64.py` & `mse_cli-1.0.1/mse_cli/core/base64.py`

 * *Files identical despite different names*

### Comparing `mse_cli-1.0.0/mse_cli/core/bootstrap.py` & `mse_cli-1.0.1/mse_cli/core/bootstrap.py`

 * *Files identical despite different names*

### Comparing `mse_cli-1.0.0/mse_cli/core/clock_tick.py` & `mse_cli-1.0.1/mse_cli/core/clock_tick.py`

 * *Files identical despite different names*

### Comparing `mse_cli-1.0.0/mse_cli/core/conf.py` & `mse_cli-1.0.1/mse_cli/core/conf.py`

 * *Files identical despite different names*

### Comparing `mse_cli-1.0.0/mse_cli/core/enclave.py` & `mse_cli-1.0.1/mse_cli/core/enclave.py`

 * *Files identical despite different names*

### Comparing `mse_cli-1.0.0/mse_cli/core/fs.py` & `mse_cli-1.0.1/mse_cli/core/fs.py`

 * *Files identical despite different names*

### Comparing `mse_cli-1.0.0/mse_cli/core/ignore_file.py` & `mse_cli-1.0.1/mse_cli/core/ignore_file.py`

 * *Files identical despite different names*

### Comparing `mse_cli-1.0.0/mse_cli/core/no_sgx_docker.py` & `mse_cli-1.0.1/mse_cli/core/no_sgx_docker.py`

 * *Files identical despite different names*

### Comparing `mse_cli-1.0.0/mse_cli/core/sgx_docker.py` & `mse_cli-1.0.1/mse_cli/core/sgx_docker.py`

 * *Files identical despite different names*

### Comparing `mse_cli-1.0.0/mse_cli/core/spinner.py` & `mse_cli-1.0.1/mse_cli/core/spinner.py`

 * *Files identical despite different names*

### Comparing `mse_cli-1.0.0/mse_cli/core/test_docker.py` & `mse_cli-1.0.1/mse_cli/core/test_docker.py`

 * *Files identical despite different names*

### Comparing `mse_cli-1.0.0/mse_cli/error.py` & `mse_cli-1.0.1/mse_cli/error.py`

 * *Files identical despite different names*

### Comparing `mse_cli-1.0.0/mse_cli/home/command/code_provider/decrypt.py` & `mse_cli-1.0.1/mse_cli/home/command/code_provider/decrypt.py`

 * *Files identical despite different names*

### Comparing `mse_cli-1.0.0/mse_cli/home/command/code_provider/localtest.py` & `mse_cli-1.0.1/mse_cli/home/command/code_provider/localtest.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,20 @@
 
     parser.add_argument(
         "--sealed-secrets",
         type=Path,
         help="the secrets JSON to seal file path (unsealed for the test purpose)",
     )
 
+    parser.add_argument(
+        "--no-tests",
+        action="store_true",
+        help="do not run the tests: just start the docker",
+    )
+
     parser.set_defaults(func=run)
 
 
 def run(args) -> None:
     """Run the subcommand."""
     code_path: Path
     test_path: Path
@@ -141,14 +147,15 @@
         client,
         docker_name,
         container_name,
         docker_config,
         test_path,
         secrets_path,
         sealed_secrets_path,
+        args.no_tests,
     )
 
 
 def build_test_docker(client, dockerfile: Path, docker_name: str):
     """Build the test docker."""
     try:
         LOG.info("Building your docker image...")
```

### Comparing `mse_cli-1.0.0/mse_cli/home/command/code_provider/package.py` & `mse_cli-1.0.1/mse_cli/home/command/code_provider/package.py`

 * *Files identical despite different names*

### Comparing `mse_cli-1.0.0/mse_cli/home/command/code_provider/scaffold.py` & `mse_cli-1.0.1/mse_cli/home/command/code_provider/scaffold.py`

 * *Files identical despite different names*

### Comparing `mse_cli-1.0.0/mse_cli/home/command/code_provider/seal.py` & `mse_cli-1.0.1/mse_cli/home/command/code_provider/seal.py`

 * *Files identical despite different names*

### Comparing `mse_cli-1.0.0/mse_cli/home/command/code_provider/verify.py` & `mse_cli-1.0.1/mse_cli/home/command/code_provider/verify.py`

 * *Files identical despite different names*

### Comparing `mse_cli-1.0.0/mse_cli/home/command/helpers.py` & `mse_cli-1.0.1/mse_cli/home/command/helpers.py`

 * *Files identical despite different names*

### Comparing `mse_cli-1.0.0/mse_cli/home/command/sgx_operator/evidence.py` & `mse_cli-1.0.1/mse_cli/home/command/sgx_operator/evidence.py`

 * *Files identical despite different names*

### Comparing `mse_cli-1.0.0/mse_cli/home/command/sgx_operator/list_all.py` & `mse_cli-1.0.1/mse_cli/home/command/sgx_operator/list_all.py`

 * *Files identical despite different names*

### Comparing `mse_cli-1.0.0/mse_cli/home/command/sgx_operator/logs.py` & `mse_cli-1.0.1/mse_cli/home/command/sgx_operator/logs.py`

 * *Files identical despite different names*

### Comparing `mse_cli-1.0.0/mse_cli/home/command/sgx_operator/restart.py` & `mse_cli-1.0.1/mse_cli/home/command/sgx_operator/restart.py`

 * *Files identical despite different names*

### Comparing `mse_cli-1.0.0/mse_cli/home/command/sgx_operator/run.py` & `mse_cli-1.0.1/mse_cli/home/command/sgx_operator/run.py`

 * *Files identical despite different names*

### Comparing `mse_cli-1.0.0/mse_cli/home/command/sgx_operator/spawn.py` & `mse_cli-1.0.1/mse_cli/home/command/sgx_operator/spawn.py`

 * *Files identical despite different names*

### Comparing `mse_cli-1.0.0/mse_cli/home/command/sgx_operator/status.py` & `mse_cli-1.0.1/mse_cli/home/command/sgx_operator/status.py`

 * *Files identical despite different names*

### Comparing `mse_cli-1.0.0/mse_cli/home/command/sgx_operator/stop.py` & `mse_cli-1.0.1/mse_cli/home/command/sgx_operator/stop.py`

 * *Files identical despite different names*

### Comparing `mse_cli-1.0.0/mse_cli/home/command/sgx_operator/test.py` & `mse_cli-1.0.1/mse_cli/home/command/sgx_operator/test.py`

 * *Files identical despite different names*

### Comparing `mse_cli-1.0.0/mse_cli/home/model/evidence.py` & `mse_cli-1.0.1/mse_cli/home/model/evidence.py`

 * *Files identical despite different names*

### Comparing `mse_cli-1.0.0/mse_cli/home/model/package.py` & `mse_cli-1.0.1/mse_cli/home/model/package.py`

 * *Files identical despite different names*

### Comparing `mse_cli-1.0.0/mse_cli/log.py` & `mse_cli-1.0.1/mse_cli/log.py`

 * *Files identical despite different names*

### Comparing `mse_cli-1.0.0/mse_cli/main.py` & `mse_cli-1.0.1/mse_cli/main.py`

 * *Files identical despite different names*

### Comparing `mse_cli-1.0.0/mse_cli/template/README.md` & `mse_cli-1.0.1/mse_cli/template/README.md`

 * *Files identical despite different names*

### Comparing `mse_cli-1.0.0/mse_cli/template/mse_src/app.py.template` & `mse_cli-1.0.1/mse_cli/template/mse_src/app.py.template`

 * *Files identical despite different names*

### Comparing `mse_cli-1.0.0/mse_cli/template/tests/conftest.py.template` & `mse_cli-1.0.1/mse_cli/template/tests/conftest.py.template`

 * *Files identical despite different names*

### Comparing `mse_cli-1.0.0/mse_cli/template/tests/test_app.py.template` & `mse_cli-1.0.1/mse_cli/template/tests/test_app.py.template`

 * *Files identical despite different names*

### Comparing `mse_cli-1.0.0/mse_cli.egg-info/PKG-INFO` & `mse_cli-1.0.1/mse_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mse-cli
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python CLI for Microservice Encryption
 Home-page: https://cosmian.com
 Author: Cosmian Tech
 Author-email: tech@cosmian.com
 License: MIT
 Project-URL: Documentation, https://docs.cosmian.com
 Project-URL: Source, https://github.com/Cosmian/mse-cli
```

### Comparing `mse_cli-1.0.0/mse_cli.egg-info/SOURCES.txt` & `mse_cli-1.0.1/mse_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mse_cli-1.0.0/setup.cfg` & `mse_cli-1.0.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `mse_cli-1.0.0/setup.py` & `mse_cli-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `mse_cli-1.0.0/tests/test_base64.py` & `mse_cli-1.0.1/tests/test_base64.py`

 * *Files identical despite different names*

### Comparing `mse_cli-1.0.0/tests/test_boostrap.py` & `mse_cli-1.0.1/tests/test_boostrap.py`

 * *Files identical despite different names*

### Comparing `mse_cli-1.0.0/tests/test_cli_cloud.py` & `mse_cli-1.0.1/tests/test_cli_cloud.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,15 +87,15 @@
 
     # The viability (is that runnable?) of the code will be tested later
     return conf
 
 
 def _test_localtest(f: io.StringIO, conf: Path) -> None:
     """Test the localtest subcommand."""
-    run_localtest(Namespace(**{"path": conf}))
+    run_localtest(Namespace(**{"path": conf, "no_tests": False}))
 
     assert "Tests successful" in capture_logs(f)
 
 
 def _test_test(f: io.StringIO, app_id: UUID) -> None:
     """Test the localtest subcommand."""
     run_test(Namespace(**{"app_id": app_id}))
@@ -113,14 +113,15 @@
         Namespace(
             **{
                 "path": conf,
                 "y": False,
                 "no_verify": False,
                 "untrusted_ssl": untrusted_ssl,
                 "workspace": tmp_path,
+                "timeout": 15,
             }
         )
     )
 
     output = capture_logs(f)
 
     try:
```

### Comparing `mse_cli-1.0.0/tests/test_cli_cloud_error.py` & `mse_cli-1.0.1/tests/test_cli_cloud_error.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,14 +153,15 @@
             Namespace(
                 **{
                     "path": Path(__file__).parent / "data" / "non_free_plan.toml",
                     "y": False,
                     "no_verify": False,
                     "untrusted_ssl": False,
                     "workspace": tmp_path,
+                    "timeout": 15,
                 }
             )
         )
 
     assert (
         "Project `default` has not enough hardware available `64g-eu-001` to spawn app named `non_free`"
         in str(exception.value)
@@ -175,14 +176,15 @@
             Namespace(
                 **{
                     "path": Path(__file__).parent / "data" / "bad_project_name.toml",
                     "y": False,
                     "no_verify": False,
                     "untrusted_ssl": False,
                     "workspace": tmp_path,
+                    "timeout": 15,
                 }
             )
         )
 
     assert "Project notexist does not exist" in str(exception.value)
 
 
@@ -196,14 +198,15 @@
                     "path": Path(__file__).parent
                     / "data"
                     / "bad_python_application.toml",
                     "y": False,
                     "no_verify": False,
                     "untrusted_ssl": False,
                     "workspace": tmp_path,
+                    "timeout": 15,
                 }
             )
         )
 
     assert "Flask module 'app' not found in directory" in str(exception.value)
 
 
@@ -215,14 +218,15 @@
             Namespace(
                 **{
                     "path": Path(__file__).parent / "data" / "bad_docker.toml",
                     "y": False,
                     "no_verify": False,
                     "untrusted_ssl": False,
                     "workspace": tmp_path,
+                    "timeout": 15,
                 }
             )
         )
 
     assert (
         "Docker `ghcr.io/cosmian/mse-pytorch:notexist` is not approved or supported yet."
         in str(exception.value)
@@ -237,12 +241,13 @@
             Namespace(
                 **{
                     "path": Path(__file__).parent / "data" / "bad_docker_latest.toml",
                     "y": False,
                     "no_verify": False,
                     "untrusted_ssl": False,
                     "workspace": tmp_path,
+                    "timeout": 15,
                 }
             )
         )
 
     assert "You shouldn't use latest tag for the docker image" in str(exception.value)
```

### Comparing `mse_cli-1.0.0/tests/test_cli_home.py` & `mse_cli-1.0.1/tests/test_cli_home.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,14 +64,15 @@
                 "project": None,
                 "code": pytest.app_path / "mse_src",
                 "dockerfile": pytest.app_path / "Dockerfile",
                 "config": pytest.app_path / "mse.toml",
                 "secrets": pytest.app_path / "secrets.json",
                 "sealed_secrets": pytest.app_path / "secrets_to_seal.json",
                 "test": pytest.app_path / "tests",
+                "no_tests": False,
             }
         )
     )
 
     # Check the tar generation
     assert "Tests successful" in capture_logs(cmd_log)
 
@@ -86,14 +87,15 @@
                 "project": pytest.app_path,
                 "code": None,
                 "dockerfile": None,
                 "config": None,
                 "secrets": None,
                 "sealed_secrets": None,
                 "test": None,
+                "no_tests": False,
             }
         )
     )
 
     # Check the tar generation
     assert "Tests successful" in capture_logs(cmd_log)
```

### Comparing `mse_cli-1.0.0/tests/test_conf.py` & `mse_cli-1.0.1/tests/test_conf.py`

 * *Files identical despite different names*

### Comparing `mse_cli-1.0.0/tests/test_context.py` & `mse_cli-1.0.1/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `mse_cli-1.0.0/tests/test_ignore_file.py` & `mse_cli-1.0.1/tests/test_ignore_file.py`

 * *Files identical despite different names*

### Comparing `mse_cli-1.0.0/tests/test_model_evidence.py` & `mse_cli-1.0.1/tests/test_model_evidence.py`

 * *Files identical despite different names*

### Comparing `mse_cli-1.0.0/tests/test_model_package.py` & `mse_cli-1.0.1/tests/test_model_package.py`

 * *Files identical despite different names*

### Comparing `mse_cli-1.0.0/tests/test_no_sgx_docker.py` & `mse_cli-1.0.1/tests/test_no_sgx_docker.py`

 * *Files identical despite different names*

### Comparing `mse_cli-1.0.0/tests/test_sgx_docker.py` & `mse_cli-1.0.1/tests/test_sgx_docker.py`

 * *Files identical despite different names*

### Comparing `mse_cli-1.0.0/tests/test_test_docker.py` & `mse_cli-1.0.1/tests/test_test_docker.py`

 * *Files identical despite different names*

### Comparing `mse_cli-1.0.0/tests/test_types.py` & `mse_cli-1.0.1/tests/test_types.py`

 * *Files identical despite different names*

