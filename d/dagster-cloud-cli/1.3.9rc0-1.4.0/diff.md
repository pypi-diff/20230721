# Comparing `tmp/dagster_cloud_cli-1.3.9rc0.tar.gz` & `tmp/dagster_cloud_cli-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster_cloud_cli-1.3.9rc0.tar", last modified: Thu Jun  8 18:31:24 2023, max compression
+gzip compressed data, was "dagster_cloud_cli-1.4.0.tar", last modified: Thu Jul 20 22:04:31 2023, max compression
```

## Comparing `dagster_cloud_cli-1.3.9rc0.tar` & `dagster_cloud_cli-1.4.0.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:31:24.881262 dagster_cloud_cli-1.3.9rc0/
--rw-r--r--   0 root         (0) root         (0)      132 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      317 2023-06-08 18:31:24.881262 dagster_cloud_cli-1.3.9rc0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:31:24.849262 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:31:24.853262 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/commands/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/commands/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:31:24.853262 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/commands/branch_deployment/
--rw-r--r--   0 root         (0) root         (0)     4612 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/commands/branch_deployment/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:31:24.857262 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/commands/ci/
--rw-r--r--   0 root         (0) root         (0)    26608 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/commands/ci/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4124 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/commands/ci/checks.py
--rw-r--r--   0 root         (0) root         (0)     1872 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/commands/ci/report.py
--rw-r--r--   0 root         (0) root         (0)     4114 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/commands/ci/state.py
--rw-r--r--   0 root         (0) root         (0)      508 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/commands/ci/utils.py
--rw-r--r--   0 root         (0) root         (0)     8622 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/commands/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:31:24.857262 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/commands/deployment/
--rw-r--r--   0 root         (0) root         (0)     1508 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/commands/deployment/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:31:24.857262 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/commands/deployment/alert_policies/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/commands/deployment/alert_policies/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1570 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/commands/deployment/alert_policies/commands.py
--rw-r--r--   0 root         (0) root         (0)     5883 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/commands/deployment/alert_policies/config_schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:31:24.857262 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/commands/job/
--rw-r--r--   0 root         (0) root         (0)     1926 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/commands/job/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4233 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/commands/metrics.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:31:24.857262 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/commands/organization/
--rw-r--r--   0 root         (0) root         (0)     2129 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/commands/organization/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:31:24.861262 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/commands/organization/saml/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/commands/organization/saml/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2707 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/commands/organization/saml/commands.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:31:24.861262 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/commands/run/
--rw-r--r--   0 root         (0) root         (0)      669 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/commands/run/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:31:24.861262 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/commands/serverless/
--rw-r--r--   0 root         (0) root         (0)     1499 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/commands/serverless/Dockerfile
--rw-r--r--   0 root         (0) root         (0)      628 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/commands/serverless/Dockerfile.dagster-cloud-cli
--rw-r--r--   0 root         (0) root         (0)    18121 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/commands/serverless/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:31:24.865262 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/commands/workspace/
--rw-r--r--   0 root         (0) root         (0)    11997 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/commands/workspace/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18291 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/config_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:31:24.869262 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/core/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)      424 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/core/_utils.py
--rw-r--r--   0 root         (0) root         (0)     1744 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/core/docker_runner.py
--rw-r--r--   0 root         (0) root         (0)     1122 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/core/errors.py
--rw-r--r--   0 root         (0) root         (0)     9228 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/core/graphql_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:31:24.869262 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/core/headers/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/core/headers/__init__.py
--rw-r--r--   0 root         (0) root         (0)      376 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/core/headers/auth.py
--rw-r--r--   0 root         (0) root         (0)      958 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/core/headers/impl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:31:24.869262 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/core/headers/versioning/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/core/headers/versioning/__init__.py
--rw-r--r--   0 root         (0) root         (0)       96 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/core/headers/versioning/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:31:24.877262 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/core/pex_builder/
--rw-r--r--   0 root         (0) root         (0)      172 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/core/pex_builder/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1680 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/core/pex_builder/code_location.py
--rw-r--r--   0 root         (0) root         (0)     9467 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/core/pex_builder/deploy.py
--rw-r--r--   0 root         (0) root         (0)    13847 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/core/pex_builder/deps.py
--rw-r--r--   0 root         (0) root         (0)      949 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/core/pex_builder/git_context.py
--rw-r--r--   0 root         (0) root         (0)     6992 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/core/pex_builder/github_context.py
--rw-r--r--   0 root         (0) root         (0)     1063 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/core/pex_builder/gitlab_context.py
--rw-r--r--   0 root         (0) root         (0)     1232 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/core/pex_builder/parse_workspace.py
--rw-r--r--   0 root         (0) root         (0)     4655 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/core/pex_builder/pex_registry.py
--rw-r--r--   0 root         (0) root         (0)      709 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/core/pex_builder/selftest.py
--rw-r--r--   0 root         (0) root         (0)     4787 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/core/pex_builder/source.py
--rw-r--r--   0 root         (0) root         (0)     5913 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/core/pex_builder/util.py
--rw-r--r--   0 root         (0) root         (0)     1920 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/core/pydantic_yaml.py
--rw-r--r--   0 root         (0) root         (0)     5384 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/core/workspace.py
--rw-r--r--   0 root         (0) root         (0)     2513 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/docker_utils.py
--rw-r--r--   0 root         (0) root         (0)     6700 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/entrypoint.py
--rw-r--r--   0 root         (0) root         (0)    18577 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/gql.py
--rw-r--r--   0 root         (0) root         (0)     5859 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/pex_utils.py
--rw-r--r--   0 root         (0) root         (0)     1487 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/types.py
--rw-r--r--   0 root         (0) root         (0)     2804 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/ui.py
--rw-r--r--   0 root         (0) root         (0)     3488 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/utils.py
--rw-r--r--   0 root         (0) root         (0)       25 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:31:24.853262 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli.egg-info/
--rw-r--r--   0 root         (0) root         (0)      317 2023-06-08 18:31:24.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2950 2023-06-08 18:31:24.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 18:31:24.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       67 2023-06-08 18:31:24.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       97 2023-06-08 18:31:24.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       42 2023-06-08 18:31:24.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:31:24.881262 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      189 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli_tests/conftest.py
--rw-r--r--   0 root         (0) root         (0)     3745 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli_tests/test_check.py
--rw-r--r--   0 root         (0) root         (0)    16129 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli_tests/test_ci_commands.py
--rw-r--r--   0 root         (0) root         (0)      659 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli_tests/test_gql.py
--rw-r--r--   0 root         (0) root         (0)     8872 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli_tests/test_metrics.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-08 18:31:24.881262 dagster_cloud_cli-1.3.9rc0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1101 2023-06-08 18:21:06.000000 dagster_cloud_cli-1.3.9rc0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:04:31.292167 dagster_cloud_cli-1.4.0/
+-rw-r--r--   0 root         (0) root         (0)      132 2023-07-20 21:53:47.000000 dagster_cloud_cli-1.4.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      314 2023-07-20 22:04:31.292167 dagster_cloud_cli-1.4.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:04:31.240167 dagster_cloud_cli-1.4.0/dagster_cloud_cli/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-20 21:53:47.000000 dagster_cloud_cli-1.4.0/dagster_cloud_cli/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:04:31.244167 dagster_cloud_cli-1.4.0/dagster_cloud_cli/commands/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-20 21:53:47.000000 dagster_cloud_cli-1.4.0/dagster_cloud_cli/commands/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:04:31.244167 dagster_cloud_cli-1.4.0/dagster_cloud_cli/commands/branch_deployment/
+-rw-r--r--   0 root         (0) root         (0)     4947 2023-07-20 21:53:47.000000 dagster_cloud_cli-1.4.0/dagster_cloud_cli/commands/branch_deployment/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:04:31.248167 dagster_cloud_cli-1.4.0/dagster_cloud_cli/commands/ci/
+-rw-r--r--   0 root         (0) root         (0)    26608 2023-07-20 21:53:47.000000 dagster_cloud_cli-1.4.0/dagster_cloud_cli/commands/ci/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4124 2023-07-20 21:53:47.000000 dagster_cloud_cli-1.4.0/dagster_cloud_cli/commands/ci/checks.py
+-rw-r--r--   0 root         (0) root         (0)     1872 2023-07-20 21:53:47.000000 dagster_cloud_cli-1.4.0/dagster_cloud_cli/commands/ci/report.py
+-rw-r--r--   0 root         (0) root         (0)     4114 2023-07-20 21:53:47.000000 dagster_cloud_cli-1.4.0/dagster_cloud_cli/commands/ci/state.py
+-rw-r--r--   0 root         (0) root         (0)      508 2023-07-20 21:53:47.000000 dagster_cloud_cli-1.4.0/dagster_cloud_cli/commands/ci/utils.py
+-rw-r--r--   0 root         (0) root         (0)     8597 2023-07-20 21:53:47.000000 dagster_cloud_cli-1.4.0/dagster_cloud_cli/commands/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:04:31.248167 dagster_cloud_cli-1.4.0/dagster_cloud_cli/commands/deployment/
+-rw-r--r--   0 root         (0) root         (0)     1508 2023-07-20 21:53:47.000000 dagster_cloud_cli-1.4.0/dagster_cloud_cli/commands/deployment/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:04:31.252167 dagster_cloud_cli-1.4.0/dagster_cloud_cli/commands/deployment/alert_policies/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-20 21:53:47.000000 dagster_cloud_cli-1.4.0/dagster_cloud_cli/commands/deployment/alert_policies/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1570 2023-07-20 21:53:47.000000 dagster_cloud_cli-1.4.0/dagster_cloud_cli/commands/deployment/alert_policies/commands.py
+-rw-r--r--   0 root         (0) root         (0)     5883 2023-07-20 21:53:47.000000 dagster_cloud_cli-1.4.0/dagster_cloud_cli/commands/deployment/alert_policies/config_schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:04:31.252167 dagster_cloud_cli-1.4.0/dagster_cloud_cli/commands/job/
+-rw-r--r--   0 root         (0) root         (0)     1926 2023-07-20 21:53:47.000000 dagster_cloud_cli-1.4.0/dagster_cloud_cli/commands/job/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4233 2023-07-20 21:53:47.000000 dagster_cloud_cli-1.4.0/dagster_cloud_cli/commands/metrics.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:04:31.252167 dagster_cloud_cli-1.4.0/dagster_cloud_cli/commands/organization/
+-rw-r--r--   0 root         (0) root         (0)     2129 2023-07-20 21:53:47.000000 dagster_cloud_cli-1.4.0/dagster_cloud_cli/commands/organization/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:04:31.256167 dagster_cloud_cli-1.4.0/dagster_cloud_cli/commands/organization/saml/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-20 21:53:47.000000 dagster_cloud_cli-1.4.0/dagster_cloud_cli/commands/organization/saml/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2707 2023-07-20 21:53:47.000000 dagster_cloud_cli-1.4.0/dagster_cloud_cli/commands/organization/saml/commands.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:04:31.256167 dagster_cloud_cli-1.4.0/dagster_cloud_cli/commands/run/
+-rw-r--r--   0 root         (0) root         (0)      669 2023-07-20 21:53:47.000000 dagster_cloud_cli-1.4.0/dagster_cloud_cli/commands/run/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:04:31.260167 dagster_cloud_cli-1.4.0/dagster_cloud_cli/commands/serverless/
+-rw-r--r--   0 root         (0) root         (0)     1499 2023-07-20 21:53:47.000000 dagster_cloud_cli-1.4.0/dagster_cloud_cli/commands/serverless/Dockerfile
+-rw-r--r--   0 root         (0) root         (0)      628 2023-07-20 21:53:47.000000 dagster_cloud_cli-1.4.0/dagster_cloud_cli/commands/serverless/Dockerfile.dagster-cloud-cli
+-rw-r--r--   0 root         (0) root         (0)    18121 2023-07-20 21:53:47.000000 dagster_cloud_cli-1.4.0/dagster_cloud_cli/commands/serverless/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:04:31.260167 dagster_cloud_cli-1.4.0/dagster_cloud_cli/commands/workspace/
+-rw-r--r--   0 root         (0) root         (0)    11992 2023-07-20 21:53:47.000000 dagster_cloud_cli-1.4.0/dagster_cloud_cli/commands/workspace/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18291 2023-07-20 21:53:47.000000 dagster_cloud_cli-1.4.0/dagster_cloud_cli/config_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:04:31.272167 dagster_cloud_cli-1.4.0/dagster_cloud_cli/core/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-20 21:53:47.000000 dagster_cloud_cli-1.4.0/dagster_cloud_cli/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      424 2023-07-20 21:53:47.000000 dagster_cloud_cli-1.4.0/dagster_cloud_cli/core/_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1744 2023-07-20 21:53:47.000000 dagster_cloud_cli-1.4.0/dagster_cloud_cli/core/docker_runner.py
+-rw-r--r--   0 root         (0) root         (0)     1122 2023-07-20 21:53:47.000000 dagster_cloud_cli-1.4.0/dagster_cloud_cli/core/errors.py
+-rw-r--r--   0 root         (0) root         (0)     9223 2023-07-20 21:53:47.000000 dagster_cloud_cli-1.4.0/dagster_cloud_cli/core/graphql_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:04:31.272167 dagster_cloud_cli-1.4.0/dagster_cloud_cli/core/headers/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-20 21:53:47.000000 dagster_cloud_cli-1.4.0/dagster_cloud_cli/core/headers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      376 2023-07-20 21:53:47.000000 dagster_cloud_cli-1.4.0/dagster_cloud_cli/core/headers/auth.py
+-rw-r--r--   0 root         (0) root         (0)      958 2023-07-20 21:53:47.000000 dagster_cloud_cli-1.4.0/dagster_cloud_cli/core/headers/impl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:04:31.272167 dagster_cloud_cli-1.4.0/dagster_cloud_cli/core/headers/versioning/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-20 21:53:47.000000 dagster_cloud_cli-1.4.0/dagster_cloud_cli/core/headers/versioning/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       96 2023-07-20 21:53:47.000000 dagster_cloud_cli-1.4.0/dagster_cloud_cli/core/headers/versioning/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:04:31.284167 dagster_cloud_cli-1.4.0/dagster_cloud_cli/core/pex_builder/
+-rw-r--r--   0 root         (0) root         (0)      172 2023-07-20 21:53:47.000000 dagster_cloud_cli-1.4.0/dagster_cloud_cli/core/pex_builder/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1680 2023-07-20 21:53:47.000000 dagster_cloud_cli-1.4.0/dagster_cloud_cli/core/pex_builder/code_location.py
+-rw-r--r--   0 root         (0) root         (0)     9467 2023-07-20 21:53:47.000000 dagster_cloud_cli-1.4.0/dagster_cloud_cli/core/pex_builder/deploy.py
+-rw-r--r--   0 root         (0) root         (0)    13847 2023-07-20 21:53:47.000000 dagster_cloud_cli-1.4.0/dagster_cloud_cli/core/pex_builder/deps.py
+-rw-r--r--   0 root         (0) root         (0)      949 2023-07-20 21:53:47.000000 dagster_cloud_cli-1.4.0/dagster_cloud_cli/core/pex_builder/git_context.py
+-rw-r--r--   0 root         (0) root         (0)     6992 2023-07-20 21:53:47.000000 dagster_cloud_cli-1.4.0/dagster_cloud_cli/core/pex_builder/github_context.py
+-rw-r--r--   0 root         (0) root         (0)     1063 2023-07-20 21:53:47.000000 dagster_cloud_cli-1.4.0/dagster_cloud_cli/core/pex_builder/gitlab_context.py
+-rw-r--r--   0 root         (0) root         (0)     1232 2023-07-20 21:53:47.000000 dagster_cloud_cli-1.4.0/dagster_cloud_cli/core/pex_builder/parse_workspace.py
+-rw-r--r--   0 root         (0) root         (0)     4655 2023-07-20 21:53:47.000000 dagster_cloud_cli-1.4.0/dagster_cloud_cli/core/pex_builder/pex_registry.py
+-rw-r--r--   0 root         (0) root         (0)      709 2023-07-20 21:53:47.000000 dagster_cloud_cli-1.4.0/dagster_cloud_cli/core/pex_builder/selftest.py
+-rw-r--r--   0 root         (0) root         (0)     4832 2023-07-20 21:53:47.000000 dagster_cloud_cli-1.4.0/dagster_cloud_cli/core/pex_builder/source.py
+-rw-r--r--   0 root         (0) root         (0)     5913 2023-07-20 21:53:47.000000 dagster_cloud_cli-1.4.0/dagster_cloud_cli/core/pex_builder/util.py
+-rw-r--r--   0 root         (0) root         (0)     1920 2023-07-20 21:53:47.000000 dagster_cloud_cli-1.4.0/dagster_cloud_cli/core/pydantic_yaml.py
+-rw-r--r--   0 root         (0) root         (0)     5384 2023-07-20 21:53:47.000000 dagster_cloud_cli-1.4.0/dagster_cloud_cli/core/workspace.py
+-rw-r--r--   0 root         (0) root         (0)     2463 2023-07-20 21:53:47.000000 dagster_cloud_cli-1.4.0/dagster_cloud_cli/docker_utils.py
+-rw-r--r--   0 root         (0) root         (0)     6700 2023-07-20 21:53:47.000000 dagster_cloud_cli-1.4.0/dagster_cloud_cli/entrypoint.py
+-rw-r--r--   0 root         (0) root         (0)    20241 2023-07-20 21:53:47.000000 dagster_cloud_cli-1.4.0/dagster_cloud_cli/gql.py
+-rw-r--r--   0 root         (0) root         (0)     5859 2023-07-20 21:53:47.000000 dagster_cloud_cli-1.4.0/dagster_cloud_cli/pex_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1487 2023-07-20 21:53:47.000000 dagster_cloud_cli-1.4.0/dagster_cloud_cli/types.py
+-rw-r--r--   0 root         (0) root         (0)     2804 2023-07-20 21:53:47.000000 dagster_cloud_cli-1.4.0/dagster_cloud_cli/ui.py
+-rw-r--r--   0 root         (0) root         (0)     3488 2023-07-20 21:53:47.000000 dagster_cloud_cli-1.4.0/dagster_cloud_cli/utils.py
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-20 21:53:47.000000 dagster_cloud_cli-1.4.0/dagster_cloud_cli/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:04:31.240167 dagster_cloud_cli-1.4.0/dagster_cloud_cli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      314 2023-07-20 22:04:31.000000 dagster_cloud_cli-1.4.0/dagster_cloud_cli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2950 2023-07-20 22:04:31.000000 dagster_cloud_cli-1.4.0/dagster_cloud_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 22:04:31.000000 dagster_cloud_cli-1.4.0/dagster_cloud_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       67 2023-07-20 22:04:31.000000 dagster_cloud_cli-1.4.0/dagster_cloud_cli.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       97 2023-07-20 22:04:31.000000 dagster_cloud_cli-1.4.0/dagster_cloud_cli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       42 2023-07-20 22:04:31.000000 dagster_cloud_cli-1.4.0/dagster_cloud_cli.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:04:31.292167 dagster_cloud_cli-1.4.0/dagster_cloud_cli_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-20 21:53:47.000000 dagster_cloud_cli-1.4.0/dagster_cloud_cli_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      189 2023-07-20 21:53:47.000000 dagster_cloud_cli-1.4.0/dagster_cloud_cli_tests/conftest.py
+-rw-r--r--   0 root         (0) root         (0)     3745 2023-07-20 21:53:47.000000 dagster_cloud_cli-1.4.0/dagster_cloud_cli_tests/test_check.py
+-rw-r--r--   0 root         (0) root         (0)    16129 2023-07-20 21:53:47.000000 dagster_cloud_cli-1.4.0/dagster_cloud_cli_tests/test_ci_commands.py
+-rw-r--r--   0 root         (0) root         (0)      659 2023-07-20 21:53:47.000000 dagster_cloud_cli-1.4.0/dagster_cloud_cli_tests/test_gql.py
+-rw-r--r--   0 root         (0) root         (0)     8872 2023-07-20 21:53:47.000000 dagster_cloud_cli-1.4.0/dagster_cloud_cli_tests/test_metrics.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-20 22:04:31.296167 dagster_cloud_cli-1.4.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1101 2023-07-20 21:53:47.000000 dagster_cloud_cli-1.4.0/setup.py
```

### Comparing `dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/commands/branch_deployment/__init__.py` & `dagster_cloud_cli-1.4.0/dagster_cloud_cli/commands/branch_deployment/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -119,7 +119,15 @@
                 pull_request_number=pull_request_number,
                 commit_message=commit_message,
                 author_name=author_name,
                 author_email=author_email,
                 author_avatar_url=author_avatar_url,
             )
         )
+
+
+@app.command(name="delete")
+@dagster_cloud_options(allow_empty=True, requires_url=True)
+def delete(url: str, api_token: str, deployment: str):
+    """Allows deletion of a branch deployment by name."""
+    with gql.graphql_client_from_url(url, api_token) as client:
+        gql.delete_branch_deployment(client, deployment=deployment)
```

### Comparing `dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/commands/ci/__init__.py` & `dagster_cloud_cli-1.4.0/dagster_cloud_cli/commands/ci/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/commands/ci/checks.py` & `dagster_cloud_cli-1.4.0/dagster_cloud_cli/commands/ci/checks.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/commands/ci/report.py` & `dagster_cloud_cli-1.4.0/dagster_cloud_cli/commands/ci/report.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/commands/ci/state.py` & `dagster_cloud_cli-1.4.0/dagster_cloud_cli/commands/ci/state.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/commands/config.py` & `dagster_cloud_cli-1.4.0/dagster_cloud_cli/commands/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -180,16 +180,15 @@
             webbrowser.open(auth_url, new=0, autoraise=True)
             ui.print(
                 f"Opening browser...\nIf a window does not open automatically, visit {auth_url} to"
                 " finish authorization"
             )
         except webbrowser.Error as e:
             ui.warn(
-                f"Error launching web browser: {str(e)}\n\nTo finish authorization, visit"
-                f" {auth_url}\n"
+                f"Error launching web browser: {e}\n\nTo finish authorization, visit {auth_url}\n"
             )
 
         server = TokenServer(("localhost", port), nonce)
         server.serve_forever()
         new_org = server.get_organization()
         new_api_token = server.get_token()
         ui.print(f"Authorized for organization {ui.as_code(str(new_org))}\n")
```

### Comparing `dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/commands/deployment/__init__.py` & `dagster_cloud_cli-1.4.0/dagster_cloud_cli/commands/deployment/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/commands/deployment/alert_policies/commands.py` & `dagster_cloud_cli-1.4.0/dagster_cloud_cli/commands/deployment/alert_policies/commands.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/commands/deployment/alert_policies/config_schema.py` & `dagster_cloud_cli-1.4.0/dagster_cloud_cli/commands/deployment/alert_policies/config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/commands/job/__init__.py` & `dagster_cloud_cli-1.4.0/dagster_cloud_cli/commands/job/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/commands/metrics.py` & `dagster_cloud_cli-1.4.0/dagster_cloud_cli/commands/metrics.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/commands/organization/__init__.py` & `dagster_cloud_cli-1.4.0/dagster_cloud_cli/commands/organization/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/commands/organization/saml/commands.py` & `dagster_cloud_cli-1.4.0/dagster_cloud_cli/commands/organization/saml/commands.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/commands/run/__init__.py` & `dagster_cloud_cli-1.4.0/dagster_cloud_cli/commands/run/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/commands/serverless/Dockerfile` & `dagster_cloud_cli-1.4.0/dagster_cloud_cli/commands/serverless/Dockerfile`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/commands/serverless/Dockerfile.dagster-cloud-cli` & `dagster_cloud_cli-1.4.0/dagster_cloud_cli/commands/serverless/Dockerfile.dagster-cloud-cli`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/commands/serverless/__init__.py` & `dagster_cloud_cli-1.4.0/dagster_cloud_cli/commands/serverless/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/commands/workspace/__init__.py` & `dagster_cloud_cli-1.4.0/dagster_cloud_cli/commands/workspace/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -174,15 +174,15 @@
                 == "PythonError"
             ]
 
             if error_locations:
                 error_string = "Some locations failed to load after being synced by the agent:\n" + "\n".join(
                     [
                         f"Error loading {error_location}:"
-                        f" {str(nodes_by_location[error_location]['locationOrLoadError'])}"
+                        f" {nodes_by_location[error_location]['locationOrLoadError']}"
                         for error_location in error_locations
                     ]
                 )
                 raise ui.error(error_string)
             else:
                 ui.print(
                     f"Agent synced changes to {list_locations(locations)}. Changes should now be"
```

### Comparing `dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/config_utils.py` & `dagster_cloud_cli-1.4.0/dagster_cloud_cli/config_utils.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/core/docker_runner.py` & `dagster_cloud_cli-1.4.0/dagster_cloud_cli/core/docker_runner.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/core/errors.py` & `dagster_cloud_cli-1.4.0/dagster_cloud_cli/core/errors.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/core/graphql_client.py` & `dagster_cloud_cli-1.4.0/dagster_cloud_cli/core/graphql_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -183,15 +183,15 @@
             raise DagsterCloudMaintenanceException(
                 message=maintenance_info.get("message"),
                 timeout=maintenance_info.get("timeout"),
                 retry_interval=maintenance_info.get("retry_interval"),
             )
 
         if "errors" in result:
-            raise GraphQLStorageError(f"Error in GraphQL response: {str(result['errors'])}")
+            raise GraphQLStorageError(f"Error in GraphQL response: {result['errors']}")
         else:
             return result
 
 
 def get_agent_headers(config_value: Dict[str, Any], scope: DagsterCloudInstanceScope):
     return get_dagster_cloud_api_headers(
         config_value["agent_token"],
```

### Comparing `dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/core/headers/impl.py` & `dagster_cloud_cli-1.4.0/dagster_cloud_cli/core/headers/impl.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/core/pex_builder/code_location.py` & `dagster_cloud_cli-1.4.0/dagster_cloud_cli/core/pex_builder/code_location.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/core/pex_builder/deploy.py` & `dagster_cloud_cli-1.4.0/dagster_cloud_cli/core/pex_builder/deploy.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/core/pex_builder/deps.py` & `dagster_cloud_cli-1.4.0/dagster_cloud_cli/core/pex_builder/deps.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/core/pex_builder/git_context.py` & `dagster_cloud_cli-1.4.0/dagster_cloud_cli/core/pex_builder/git_context.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/core/pex_builder/github_context.py` & `dagster_cloud_cli-1.4.0/dagster_cloud_cli/core/pex_builder/github_context.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/core/pex_builder/gitlab_context.py` & `dagster_cloud_cli-1.4.0/dagster_cloud_cli/core/pex_builder/gitlab_context.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/core/pex_builder/parse_workspace.py` & `dagster_cloud_cli-1.4.0/dagster_cloud_cli/core/pex_builder/parse_workspace.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/core/pex_builder/pex_registry.py` & `dagster_cloud_cli-1.4.0/dagster_cloud_cli/core/pex_builder/pex_registry.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/core/pex_builder/selftest.py` & `dagster_cloud_cli-1.4.0/dagster_cloud_cli/core/pex_builder/selftest.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/core/pex_builder/source.py` & `dagster_cloud_cli-1.4.0/dagster_cloud_cli/core/pex_builder/source.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,24 @@
 
 import click
 
 from . import deps, util
 
 # inspired by https://github.com/github/gitignore/blob/main/Python.gitignore
 # would be nice to just read the gitignore and use that
-IGNORED_PATTERNS = [".git", "__pycache__", ".pytest_cache", ".tox", ".nox", "*.pyc", ".mypy_cache"]
+IGNORED_PATTERNS = [
+    ".git",
+    "__pycache__",
+    ".pytest_cache",
+    ".tox",
+    ".nox",
+    "*.pyc",
+    ".mypy_cache",
+    ".cache",
+]
 
 
 def build_source_pex(
     code_directory: str, local_package_paths: List[str], output_directory, python_version
 ):
     output_directory = os.path.abspath(output_directory)
     os.makedirs(output_directory, exist_ok=True)
```

### Comparing `dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/core/pex_builder/util.py` & `dagster_cloud_cli-1.4.0/dagster_cloud_cli/core/pex_builder/util.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/core/pydantic_yaml.py` & `dagster_cloud_cli-1.4.0/dagster_cloud_cli/core/pydantic_yaml.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/core/workspace.py` & `dagster_cloud_cli-1.4.0/dagster_cloud_cli/core/workspace.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/docker_utils.py` & `dagster_cloud_cli-1.4.0/dagster_cloud_cli/docker_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -57,18 +57,15 @@
         raise ui.error(
             "No registry found. You may need to wait for your Dagster serverless deployment to"
             " activate."
         )
 
     username, password = base64.b64decode(aws_token).decode("utf-8").split(":")
     subprocess.check_output(
-        (
-            f"echo {str(password)} | docker login --username {str(username)} --password-stdin"
-            f" {registry}"
-        ),
+        f"echo {password} | docker login --username {username} --password-stdin {registry}",
         shell=True,
     )
     return subprocess.call(
         ["docker", "push", f"{registry}:{image}"], stderr=sys.stderr, stdout=sys.stdout
     )
```

### Comparing `dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/entrypoint.py` & `dagster_cloud_cli-1.4.0/dagster_cloud_cli/entrypoint.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/gql.py` & `dagster_cloud_cli-1.4.0/dagster_cloud_cli/gql.py`

 * *Files 9% similar despite different names*

```diff
@@ -217,15 +217,15 @@
 
 def delete_code_location(client: GqlShimClient, location_name: str) -> None:
     result = client.execute(
         DELETE_LOCATION_MUTATION, variable_values={"locationName": location_name}
     )
 
     if result["data"]["deleteLocation"]["__typename"] != "DeleteLocationSuccess":
-        raise Exception(f"Unable to delete location: {str(result['data']['deleteLocation'])}")
+        raise Exception(f"Unable to delete location: {result['data']['deleteLocation']}")
 
 
 RECONCILE_LOCATIONS_FROM_DOCUMENT_MUTATION = """
 mutation CliReconcileLocationsFromDoc($document: GenericScalar!) {
     reconcileLocationsFromDocument(document: $document) {
         __typename
         ... on ReconcileLocationsSuccess {
@@ -262,15 +262,15 @@
                 location["locationName"]
                 for location in result["data"]["reconcileLocationsFromDocument"]["locations"]
             ]
         )
     elif result["data"]["reconcileLocationsFromDocument"] == "InvalidLocationError":
         raise Exception("Error in workspace config:\n" + "\n".join(result["errors"]))
     else:
-        raise Exception(f"Unable to sync locations: {str(result)}")
+        raise Exception(f"Unable to sync locations: {result}")
 
 
 GET_LOCATIONS_AS_DOCUMENT_QUERY = """
 query CliLocationsAsDocument {
     locationsAsDocument {
         __typename
         document
@@ -307,15 +307,15 @@
 def set_deployment_settings(client: GqlShimClient, deployment_settings: Dict[str, Any]) -> None:
     result = client.execute(
         SET_DEPLOYMENT_SETTINGS_MUTATION,
         variable_values={"deploymentSettings": deployment_settings},
     )
 
     if result["data"]["setDeploymentSettings"]["__typename"] != "DeploymentSettings":
-        raise Exception(f"Unable to set deployment settings: {str(result)}")
+        raise Exception(f"Unable to set deployment settings: {result}")
 
 
 DEPLOYMENT_SETTINGS_QUERY = """
     query CliDeploymentSettings {
         deploymentSettings {
             settings
         }
@@ -323,15 +323,15 @@
 """
 
 
 def get_deployment_settings(client: GqlShimClient) -> Dict[str, Any]:
     result = client.execute(DEPLOYMENT_SETTINGS_QUERY)
 
     if result.get("data", {}).get("deploymentSettings", {}).get("settings") is None:
-        raise Exception(f"Unable to get deployment settings: {str(result)}")
+        raise Exception(f"Unable to get deployment settings: {result}")
 
     return result["data"]["deploymentSettings"]["settings"]
 
 
 ALERT_POLICIES_QUERY = """
     query CliAlertPolicies {
         alertPolicies {
@@ -357,15 +357,15 @@
 """
 
 
 def get_alert_policies(client: GqlShimClient) -> Dict[str, Any]:
     result = client.execute(ALERT_POLICIES_QUERY)
 
     if result.get("data", {}).get("alertPolicies", {}) is None:
-        raise Exception(f"Unable to get deployment settings: {str(result)}")
+        raise Exception(f"Unable to get deployment settings: {result}")
 
     return result["data"]["alertPolicies"]
 
 
 RECONCILE_ALERT_POLICIES_FROM_DOCUMENT_MUTATION = """
     mutation CliReconcileAlertPoliciesFromDocumentMutation($document: GenericScalar!) {
         reconcileAlertPoliciesFromDocument(document: $document) {
@@ -429,15 +429,15 @@
 def set_organization_settings(client: GqlShimClient, organization_settings: Dict[str, Any]) -> None:
     result = client.execute(
         SET_ORGANIZATION_SETTINGS_MUTATION,
         variable_values={"organizationSettings": organization_settings},
     )
 
     if result["data"]["setOrganizationSettings"]["__typename"] != "OrganizationSettings":
-        raise Exception(f"Unable to set organization settings: {str(result)}")
+        raise Exception(f"Unable to set organization settings: {result}")
 
 
 ORGANIZATION_SETTINGS_QUERY = """
     query CliOrganizationSettings {
         organizationSettings {
             settings
         }
@@ -445,15 +445,15 @@
 """
 
 
 def get_organization_settings(client: GqlShimClient) -> Dict[str, Any]:
     result = client.execute(ORGANIZATION_SETTINGS_QUERY)
 
     if result.get("data", {}).get("organizationSettings", {}).get("settings") is None:
-        raise Exception(f"Unable to get organization settings: {str(result)}")
+        raise Exception(f"Unable to get organization settings: {result}")
 
     return result["data"]["organizationSettings"]["settings"]
 
 
 CREATE_OR_UPDATE_BRANCH_DEPLOYMENT = """
 mutation CliCreateOrUpdateBranchDeployment(
     $branchData: CreateOrUpdateBranchDeploymentInput!
@@ -510,15 +510,15 @@
                 "authorAvatarUrl": author_avatar_url,
             },
         },
     )
 
     name = result.get("data", {}).get("createOrUpdateBranchDeployment", {}).get("deploymentName")
     if name is None:
-        raise Exception(f"Unable to create or update branch deployment: {str(result)}")
+        raise Exception(f"Unable to create or update branch deployment: {result}")
 
     return cast(str, name)
 
 
 LAUNCH_RUN_MUTATION = """
     mutation CliLaunchRun($executionParams: ExecutionParams!) {
         launchRun(executionParams: $executionParams) {
@@ -571,15 +571,15 @@
     }
     result = client.execute(
         LAUNCH_RUN_MUTATION,
         variable_values={"executionParams": params},
     )
 
     if result["data"]["launchRun"]["__typename"] != "LaunchRunSuccess":
-        raise Exception(f"Unable to launch run: {str(result)}")
+        raise Exception(f"Unable to launch run: {result}")
 
     return result["data"]["launchRun"]["run"]["runId"]
 
 
 GET_ECR_CREDS_QUERY = """
 query CliGetEcrInfo {
     serverless {
@@ -656,7 +656,63 @@
                 "durationSeconds": duration_seconds,
                 "success": success,
                 "tags": tags,
                 "message": message,
             },
         )
         return res["data"]["markCliEvent"] == "ok"
+
+
+GET_DEPLOYMENT_BY_NAME_QUERY = """
+query DeploymentByNameQuery($deploymentName: String!) {
+    deploymentByName(name: $deploymentName) {
+        __typename
+        ... on DagsterCloudDeployment {
+            deploymentName
+            deploymentId
+            deploymentType
+        }
+    }
+}
+"""
+
+DELETE_DEPLOYMENT_MUTATION = """
+mutation CliDeleteDeployment($deploymentId: Int!) {
+    deleteDeployment(deploymentId: $deploymentId) {
+        __typename
+        ... on DagsterCloudDeployment {
+            deploymentId
+        }
+        ... on PythonError {
+            message
+            stack
+        }
+    }
+}
+"""
+
+
+def get_deployment_by_name(client: GqlShimClient, deployment: str) -> Dict[str, Any]:
+    result = client.execute(
+        GET_DEPLOYMENT_BY_NAME_QUERY, variable_values={"deploymentName": deployment}
+    )["data"]["deploymentByName"]
+    if not result["__typename"] == "DagsterCloudDeployment":
+        raise Exception(f"Unable to find deployment {deployment}")
+
+    return result
+    raise Exception(f"Unable to find deployment {deployment}")
+
+
+def delete_branch_deployment(client: GqlShimClient, deployment: str) -> Any:
+    deployment_info = get_deployment_by_name(client, deployment)
+    if not deployment_info["deploymentType"] == "BRANCH":
+        raise Exception(f"Deployment {deployment} is not a branch deployment")
+
+    result = client.execute(
+        DELETE_DEPLOYMENT_MUTATION,
+        variable_values={"deploymentId": deployment_info["deploymentId"]},
+    )
+
+    if result["data"]["deleteDeployment"]["__typename"] != "DagsterCloudDeployment":
+        raise Exception(f"Unable to delete deployment: {result}")
+
+    return result["data"]["deleteDeployment"]["deploymentId"]
```

### Comparing `dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/pex_utils.py` & `dagster_cloud_cli-1.4.0/dagster_cloud_cli/pex_utils.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/types.py` & `dagster_cloud_cli-1.4.0/dagster_cloud_cli/types.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/ui.py` & `dagster_cloud_cli-1.4.0/dagster_cloud_cli/ui.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli/utils.py` & `dagster_cloud_cli-1.4.0/dagster_cloud_cli/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,15 +80,15 @@
             },
         )
 
         @functools.wraps(to_wrap)
         def wrap_function(*args, **kwargs):
             modified_kwargs = kwargs
             if not has_kwargs and not hasattr(to_wrap, "modified_options"):
-                modified_kwargs: dict[Any, Any] = {
+                modified_kwargs: Dict[Any, Any] = {
                     k: v for k, v in kwargs.items() if k in to_wrap_sig.parameters
                 }
             return to_wrap(*args, **modified_kwargs)
 
         wrap_function.__signature__ = sig
         wrap_function.modified_options = True
         return wrap_function
```

### Comparing `dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli.egg-info/SOURCES.txt` & `dagster_cloud_cli-1.4.0/dagster_cloud_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli_tests/test_check.py` & `dagster_cloud_cli-1.4.0/dagster_cloud_cli_tests/test_check.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli_tests/test_ci_commands.py` & `dagster_cloud_cli-1.4.0/dagster_cloud_cli_tests/test_ci_commands.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli_tests/test_gql.py` & `dagster_cloud_cli-1.4.0/dagster_cloud_cli_tests/test_gql.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.9rc0/dagster_cloud_cli_tests/test_metrics.py` & `dagster_cloud_cli-1.4.0/dagster_cloud_cli_tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.9rc0/setup.py` & `dagster_cloud_cli-1.4.0/setup.py`

 * *Files identical despite different names*

