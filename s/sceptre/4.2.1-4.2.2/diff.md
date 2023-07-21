# Comparing `tmp/sceptre-4.2.1.tar.gz` & `tmp/sceptre-4.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sceptre-4.2.1.tar", max compression
+gzip compressed data, was "sceptre-4.2.2.tar", max compression
```

## Comparing `sceptre-4.2.1.tar` & `sceptre-4.2.2.tar`

### file list

```diff
@@ -1,64 +1,64 @@
--rw-r--r--   0        0        0      635 2023-06-14 17:04:31.466012 sceptre-4.2.1/LICENSE
--rw-r--r--   0        0        0    10458 2023-06-14 17:04:31.466012 sceptre-4.2.1/README.md
--rw-r--r--   0        0        0     3116 2023-06-14 17:04:31.478012 sceptre-4.2.1/pyproject.toml
--rw-r--r--   0        0        0      713 2023-06-14 17:04:31.478012 sceptre-4.2.1/sceptre/__init__.py
--rw-r--r--   0        0        0     3188 2023-06-14 17:04:31.478012 sceptre-4.2.1/sceptre/cli/__init__.py
--rw-r--r--   0        0        0     1877 2023-06-14 17:04:31.478012 sceptre-4.2.1/sceptre/cli/create.py
--rw-r--r--   0        0        0     2115 2023-06-14 17:04:31.478012 sceptre-4.2.1/sceptre/cli/delete.py
--rw-r--r--   0        0        0     2482 2023-06-14 17:04:31.478012 sceptre-4.2.1/sceptre/cli/describe.py
--rw-r--r--   0        0        0     7349 2023-06-14 17:04:31.478012 sceptre-4.2.1/sceptre/cli/diff.py
--rw-r--r--   0        0        0     3297 2023-06-14 17:04:31.478012 sceptre-4.2.1/sceptre/cli/drift.py
--rw-r--r--   0        0        0     4307 2023-06-14 17:04:31.478012 sceptre-4.2.1/sceptre/cli/dump.py
--rw-r--r--   0        0        0     1441 2023-06-14 17:04:31.478012 sceptre-4.2.1/sceptre/cli/execute.py
--rw-r--r--   0        0        0    14253 2023-06-14 17:04:31.478012 sceptre-4.2.1/sceptre/cli/helpers.py
--rw-r--r--   0        0        0     7611 2023-06-14 17:04:31.482012 sceptre-4.2.1/sceptre/cli/launch.py
--rw-r--r--   0        0        0     4357 2023-06-14 17:04:31.482012 sceptre-4.2.1/sceptre/cli/list.py
--rw-r--r--   0        0        0     5678 2023-06-14 17:04:31.482012 sceptre-4.2.1/sceptre/cli/new.py
--rw-r--r--   0        0        0     1366 2023-06-14 17:04:31.482012 sceptre-4.2.1/sceptre/cli/policy.py
--rw-r--r--   0        0        0     6488 2023-06-14 17:04:31.482012 sceptre-4.2.1/sceptre/cli/prune.py
--rw-r--r--   0        0        0     1162 2023-06-14 17:04:31.482012 sceptre-4.2.1/sceptre/cli/status.py
--rw-r--r--   0        0        0     4839 2023-06-14 17:04:31.482012 sceptre-4.2.1/sceptre/cli/template.py
--rw-r--r--   0        0        0     3152 2023-06-14 17:04:31.482012 sceptre-4.2.1/sceptre/cli/update.py
--rw-r--r--   0        0        0      408 2023-06-14 17:04:31.482012 sceptre-4.2.1/sceptre/config/__init__.py
--rw-r--r--   0        0        0     3318 2023-06-14 17:04:31.482012 sceptre-4.2.1/sceptre/config/graph.py
--rw-r--r--   0        0        0    24130 2023-06-14 17:04:31.482012 sceptre-4.2.1/sceptre/config/reader.py
--rw-r--r--   0        0        0     1450 2023-06-14 17:04:31.482012 sceptre-4.2.1/sceptre/config/strategies.py
--rw-r--r--   0        0        0    21662 2023-06-14 17:04:31.482012 sceptre-4.2.1/sceptre/connection_manager.py
--rw-r--r--   0        0        0     4781 2023-06-14 17:04:31.482012 sceptre-4.2.1/sceptre/context.py
--rw-r--r--   0        0        0        0 2023-06-14 17:04:31.482012 sceptre-4.2.1/sceptre/diffing/__init__.py
--rw-r--r--   0        0        0     8016 2023-06-14 17:04:31.482012 sceptre-4.2.1/sceptre/diffing/diff_writer.py
--rw-r--r--   0        0        0    19262 2023-06-14 17:04:31.482012 sceptre-4.2.1/sceptre/diffing/stack_differ.py
--rw-r--r--   0        0        0     4089 2023-06-14 17:04:31.482012 sceptre-4.2.1/sceptre/exceptions.py
--rw-r--r--   0        0        0     7703 2023-06-14 17:04:31.482012 sceptre-4.2.1/sceptre/helpers.py
--rw-r--r--   0        0        0     3885 2023-06-14 17:04:31.482012 sceptre-4.2.1/sceptre/hooks/__init__.py
--rw-r--r--   0        0        0     3268 2023-06-14 17:04:31.482012 sceptre-4.2.1/sceptre/hooks/asg_scaling_processes.py
--rw-r--r--   0        0        0      914 2023-06-14 17:04:31.482012 sceptre-4.2.1/sceptre/hooks/cmd.py
--rw-r--r--   0        0        0      786 2023-06-14 17:04:31.482012 sceptre-4.2.1/sceptre/logging.py
--rw-r--r--   0        0        0      408 2023-06-14 17:04:31.482012 sceptre-4.2.1/sceptre/plan/__init__.py
--rw-r--r--   0        0        0    40032 2023-06-14 17:04:31.482012 sceptre-4.2.1/sceptre/plan/actions.py
--rw-r--r--   0        0        0     1972 2023-06-14 17:04:31.482012 sceptre-4.2.1/sceptre/plan/executor.py
--rw-r--r--   0        0        0    14111 2023-06-14 17:04:31.482012 sceptre-4.2.1/sceptre/plan/plan.py
--rw-r--r--   0        0        0    20784 2023-06-14 17:04:31.482012 sceptre-4.2.1/sceptre/resolvers/__init__.py
--rw-r--r--   0        0        0      676 2023-06-14 17:04:31.482012 sceptre-4.2.1/sceptre/resolvers/environment_variable.py
--rw-r--r--   0        0        0      671 2023-06-14 17:04:31.482012 sceptre-4.2.1/sceptre/resolvers/file_contents.py
--rw-r--r--   0        0        0     1303 2023-06-14 17:04:31.482012 sceptre-4.2.1/sceptre/resolvers/join.py
--rw-r--r--   0        0        0      619 2023-06-14 17:04:31.482012 sceptre-4.2.1/sceptre/resolvers/no_value.py
--rw-r--r--   0        0        0     3622 2023-06-14 17:04:31.482012 sceptre-4.2.1/sceptre/resolvers/placeholders.py
--rw-r--r--   0        0        0     1855 2023-06-14 17:04:31.482012 sceptre-4.2.1/sceptre/resolvers/select.py
--rw-r--r--   0        0        0     1312 2023-06-14 17:04:31.482012 sceptre-4.2.1/sceptre/resolvers/split.py
--rw-r--r--   0        0        0     2074 2023-06-14 17:04:31.482012 sceptre-4.2.1/sceptre/resolvers/stack_attr.py
--rw-r--r--   0        0        0     5962 2023-06-14 17:04:31.482012 sceptre-4.2.1/sceptre/resolvers/stack_output.py
--rw-r--r--   0        0        0     1784 2023-06-14 17:04:31.482012 sceptre-4.2.1/sceptre/resolvers/sub.py
--rw-r--r--   0        0        0    18185 2023-06-14 17:04:31.482012 sceptre-4.2.1/sceptre/stack.py
--rw-r--r--   0        0        0      139 2023-06-14 17:04:31.482012 sceptre-4.2.1/sceptre/stack_policies/lock.json
--rw-r--r--   0        0        0      140 2023-06-14 17:04:31.482012 sceptre-4.2.1/sceptre/stack_policies/unlock.json
--rw-r--r--   0        0        0      539 2023-06-14 17:04:31.482012 sceptre-4.2.1/sceptre/stack_status.py
--rw-r--r--   0        0        0     2419 2023-06-14 17:04:31.482012 sceptre-4.2.1/sceptre/stack_status_colourer.py
--rw-r--r--   0        0        0     8848 2023-06-14 17:04:31.486012 sceptre-4.2.1/sceptre/template.py
--rw-r--r--   0        0        0     2937 2023-06-14 17:04:31.486012 sceptre-4.2.1/sceptre/template_handlers/__init__.py
--rw-r--r--   0        0        0     2305 2023-06-14 17:04:31.486012 sceptre-4.2.1/sceptre/template_handlers/file.py
--rw-r--r--   0        0        0     4800 2023-06-14 17:04:31.486012 sceptre-4.2.1/sceptre/template_handlers/helper.py
--rw-r--r--   0        0        0     5040 2023-06-14 17:04:31.486012 sceptre-4.2.1/sceptre/template_handlers/http.py
--rw-r--r--   0        0        0     3267 2023-06-14 17:04:31.486012 sceptre-4.2.1/sceptre/template_handlers/s3.py
--rw-r--r--   0        0        0    13669 1970-01-01 00:00:00.000000 sceptre-4.2.1/setup.py
--rw-r--r--   0        0        0    12622 1970-01-01 00:00:00.000000 sceptre-4.2.1/PKG-INFO
+-rw-r--r--   0        0        0      635 2023-07-18 14:59:42.745699 sceptre-4.2.2/LICENSE
+-rw-r--r--   0        0        0    10458 2023-07-18 14:59:42.745699 sceptre-4.2.2/README.md
+-rw-r--r--   0        0        0     3102 2023-07-18 14:59:42.753699 sceptre-4.2.2/pyproject.toml
+-rw-r--r--   0        0        0      713 2023-07-18 14:59:42.753699 sceptre-4.2.2/sceptre/__init__.py
+-rw-r--r--   0        0        0     3188 2023-07-18 14:59:42.753699 sceptre-4.2.2/sceptre/cli/__init__.py
+-rw-r--r--   0        0        0     1877 2023-07-18 14:59:42.753699 sceptre-4.2.2/sceptre/cli/create.py
+-rw-r--r--   0        0        0     2115 2023-07-18 14:59:42.753699 sceptre-4.2.2/sceptre/cli/delete.py
+-rw-r--r--   0        0        0     2482 2023-07-18 14:59:42.753699 sceptre-4.2.2/sceptre/cli/describe.py
+-rw-r--r--   0        0        0     7349 2023-07-18 14:59:42.753699 sceptre-4.2.2/sceptre/cli/diff.py
+-rw-r--r--   0        0        0     3297 2023-07-18 14:59:42.753699 sceptre-4.2.2/sceptre/cli/drift.py
+-rw-r--r--   0        0        0     4307 2023-07-18 14:59:42.753699 sceptre-4.2.2/sceptre/cli/dump.py
+-rw-r--r--   0        0        0     1441 2023-07-18 14:59:42.753699 sceptre-4.2.2/sceptre/cli/execute.py
+-rw-r--r--   0        0        0    14253 2023-07-18 14:59:42.753699 sceptre-4.2.2/sceptre/cli/helpers.py
+-rw-r--r--   0        0        0     7611 2023-07-18 14:59:42.753699 sceptre-4.2.2/sceptre/cli/launch.py
+-rw-r--r--   0        0        0     4357 2023-07-18 14:59:42.753699 sceptre-4.2.2/sceptre/cli/list.py
+-rw-r--r--   0        0        0     5678 2023-07-18 14:59:42.753699 sceptre-4.2.2/sceptre/cli/new.py
+-rw-r--r--   0        0        0     1366 2023-07-18 14:59:42.753699 sceptre-4.2.2/sceptre/cli/policy.py
+-rw-r--r--   0        0        0     6488 2023-07-18 14:59:42.753699 sceptre-4.2.2/sceptre/cli/prune.py
+-rw-r--r--   0        0        0     1162 2023-07-18 14:59:42.753699 sceptre-4.2.2/sceptre/cli/status.py
+-rw-r--r--   0        0        0     4839 2023-07-18 14:59:42.753699 sceptre-4.2.2/sceptre/cli/template.py
+-rw-r--r--   0        0        0     3152 2023-07-18 14:59:42.753699 sceptre-4.2.2/sceptre/cli/update.py
+-rw-r--r--   0        0        0      408 2023-07-18 14:59:42.753699 sceptre-4.2.2/sceptre/config/__init__.py
+-rw-r--r--   0        0        0     3318 2023-07-18 14:59:42.757699 sceptre-4.2.2/sceptre/config/graph.py
+-rw-r--r--   0        0        0    24130 2023-07-18 14:59:42.757699 sceptre-4.2.2/sceptre/config/reader.py
+-rw-r--r--   0        0        0     1450 2023-07-18 14:59:42.757699 sceptre-4.2.2/sceptre/config/strategies.py
+-rw-r--r--   0        0        0    21662 2023-07-18 14:59:42.757699 sceptre-4.2.2/sceptre/connection_manager.py
+-rw-r--r--   0        0        0     4781 2023-07-18 14:59:42.757699 sceptre-4.2.2/sceptre/context.py
+-rw-r--r--   0        0        0        0 2023-07-18 14:59:42.757699 sceptre-4.2.2/sceptre/diffing/__init__.py
+-rw-r--r--   0        0        0     8016 2023-07-18 14:59:42.757699 sceptre-4.2.2/sceptre/diffing/diff_writer.py
+-rw-r--r--   0        0        0    19262 2023-07-18 14:59:42.757699 sceptre-4.2.2/sceptre/diffing/stack_differ.py
+-rw-r--r--   0        0        0     4089 2023-07-18 14:59:42.757699 sceptre-4.2.2/sceptre/exceptions.py
+-rw-r--r--   0        0        0     7703 2023-07-18 14:59:42.757699 sceptre-4.2.2/sceptre/helpers.py
+-rw-r--r--   0        0        0     3885 2023-07-18 14:59:42.757699 sceptre-4.2.2/sceptre/hooks/__init__.py
+-rw-r--r--   0        0        0     3268 2023-07-18 14:59:42.757699 sceptre-4.2.2/sceptre/hooks/asg_scaling_processes.py
+-rw-r--r--   0        0        0      914 2023-07-18 14:59:42.757699 sceptre-4.2.2/sceptre/hooks/cmd.py
+-rw-r--r--   0        0        0      786 2023-07-18 14:59:42.757699 sceptre-4.2.2/sceptre/logging.py
+-rw-r--r--   0        0        0      408 2023-07-18 14:59:42.757699 sceptre-4.2.2/sceptre/plan/__init__.py
+-rw-r--r--   0        0        0    40032 2023-07-18 14:59:42.757699 sceptre-4.2.2/sceptre/plan/actions.py
+-rw-r--r--   0        0        0     1972 2023-07-18 14:59:42.757699 sceptre-4.2.2/sceptre/plan/executor.py
+-rw-r--r--   0        0        0    14111 2023-07-18 14:59:42.757699 sceptre-4.2.2/sceptre/plan/plan.py
+-rw-r--r--   0        0        0    20784 2023-07-18 14:59:42.757699 sceptre-4.2.2/sceptre/resolvers/__init__.py
+-rw-r--r--   0        0        0      676 2023-07-18 14:59:42.757699 sceptre-4.2.2/sceptre/resolvers/environment_variable.py
+-rw-r--r--   0        0        0      671 2023-07-18 14:59:42.757699 sceptre-4.2.2/sceptre/resolvers/file_contents.py
+-rw-r--r--   0        0        0     1303 2023-07-18 14:59:42.757699 sceptre-4.2.2/sceptre/resolvers/join.py
+-rw-r--r--   0        0        0      619 2023-07-18 14:59:42.757699 sceptre-4.2.2/sceptre/resolvers/no_value.py
+-rw-r--r--   0        0        0     3622 2023-07-18 14:59:42.757699 sceptre-4.2.2/sceptre/resolvers/placeholders.py
+-rw-r--r--   0        0        0     1855 2023-07-18 14:59:42.757699 sceptre-4.2.2/sceptre/resolvers/select.py
+-rw-r--r--   0        0        0     1312 2023-07-18 14:59:42.757699 sceptre-4.2.2/sceptre/resolvers/split.py
+-rw-r--r--   0        0        0     2074 2023-07-18 14:59:42.757699 sceptre-4.2.2/sceptre/resolvers/stack_attr.py
+-rw-r--r--   0        0        0     5962 2023-07-18 14:59:42.757699 sceptre-4.2.2/sceptre/resolvers/stack_output.py
+-rw-r--r--   0        0        0     1784 2023-07-18 14:59:42.757699 sceptre-4.2.2/sceptre/resolvers/sub.py
+-rw-r--r--   0        0        0    18185 2023-07-18 14:59:42.757699 sceptre-4.2.2/sceptre/stack.py
+-rw-r--r--   0        0        0      139 2023-07-18 14:59:42.757699 sceptre-4.2.2/sceptre/stack_policies/lock.json
+-rw-r--r--   0        0        0      140 2023-07-18 14:59:42.757699 sceptre-4.2.2/sceptre/stack_policies/unlock.json
+-rw-r--r--   0        0        0      539 2023-07-18 14:59:42.757699 sceptre-4.2.2/sceptre/stack_status.py
+-rw-r--r--   0        0        0     2419 2023-07-18 14:59:42.757699 sceptre-4.2.2/sceptre/stack_status_colourer.py
+-rw-r--r--   0        0        0     8848 2023-07-18 14:59:42.757699 sceptre-4.2.2/sceptre/template.py
+-rw-r--r--   0        0        0     2937 2023-07-18 14:59:42.757699 sceptre-4.2.2/sceptre/template_handlers/__init__.py
+-rw-r--r--   0        0        0     2305 2023-07-18 14:59:42.757699 sceptre-4.2.2/sceptre/template_handlers/file.py
+-rw-r--r--   0        0        0     4800 2023-07-18 14:59:42.757699 sceptre-4.2.2/sceptre/template_handlers/helper.py
+-rw-r--r--   0        0        0     5040 2023-07-18 14:59:42.757699 sceptre-4.2.2/sceptre/template_handlers/http.py
+-rw-r--r--   0        0        0     3267 2023-07-18 14:59:42.757699 sceptre-4.2.2/sceptre/template_handlers/s3.py
+-rw-r--r--   0        0        0    13675 1970-01-01 00:00:00.000000 sceptre-4.2.2/setup.py
+-rw-r--r--   0        0        0    12628 1970-01-01 00:00:00.000000 sceptre-4.2.2/PKG-INFO
```

### Comparing `sceptre-4.2.1/LICENSE` & `sceptre-4.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sceptre-4.2.1/README.md` & `sceptre-4.2.2/README.md`

 * *Files identical despite different names*

### Comparing `sceptre-4.2.1/pyproject.toml` & `sceptre-4.2.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sceptre"
-version = "4.2.1"
+version = "4.2.2"
 packages = [{ include = "sceptre" }]
 readme = "README.md"
 homepage = "https://github.com/Sceptre/sceptre"
 repository = "https://github.com/Sceptre/sceptre"
 documentation = "https://docs.sceptre-project.org"
 authors = ["Sceptre <sceptreorg@gmail.com>"]
 description = "An AWS Cloud Provisioning Tool"
@@ -44,24 +44,24 @@
 [tool.poetry.plugins."sceptre.template_handlers"]
 "file" = "sceptre.template_handlers.file:File"
 "s3" = "sceptre.template_handlers.s3:S3"
 "http" = "sceptre.template_handlers.http:Http"
 
 [tool.poetry.dependencies]
 python = ">=3.7,<3.12"
-boto3 = ">=1.3.0,<2"
+boto3 = "^1.20.27"
 click = ">=7.0,<9.0"
 cfn-flip = "^1.2.3"
 deepdiff = "^5.5"
 deprecation = "^2.0"
 jinja2 = "^3.0"
-jsonschema = ">=3.2,<3.3"
-networkx = ">=2.6,<2.7"
+jsonschema = "~3.2"
+networkx = "~2.6"
 packaging = ">=16.8,<22.0"
-pyyaml = "^5.1"
+pyyaml = "^6.0"
 sceptre-cmd-resolver = "^2.0"
 sceptre-file-resolver = "^1.0"
 colorama = ">=0.2.5,<0.4.4"
 troposphere = { version = "^4", optional = true }
 sphinx = { version = ">=1.6.5,<=5.1.1", optional = true }
 sphinx-click = { version = ">=2.0.1,<4.0.0", optional = true }
 sphinx-rtd-theme = { version = "0.5.2", optional = true }
```

### Comparing `sceptre-4.2.1/sceptre/__init__.py` & `sceptre-4.2.2/sceptre/__init__.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.2.1/sceptre/cli/__init__.py` & `sceptre-4.2.2/sceptre/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.2.1/sceptre/cli/create.py` & `sceptre-4.2.2/sceptre/cli/create.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.2.1/sceptre/cli/delete.py` & `sceptre-4.2.2/sceptre/cli/delete.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.2.1/sceptre/cli/describe.py` & `sceptre-4.2.2/sceptre/cli/describe.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.2.1/sceptre/cli/diff.py` & `sceptre-4.2.2/sceptre/cli/diff.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.2.1/sceptre/cli/drift.py` & `sceptre-4.2.2/sceptre/cli/drift.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.2.1/sceptre/cli/dump.py` & `sceptre-4.2.2/sceptre/cli/dump.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.2.1/sceptre/cli/execute.py` & `sceptre-4.2.2/sceptre/cli/execute.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.2.1/sceptre/cli/helpers.py` & `sceptre-4.2.2/sceptre/cli/helpers.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.2.1/sceptre/cli/launch.py` & `sceptre-4.2.2/sceptre/cli/launch.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.2.1/sceptre/cli/list.py` & `sceptre-4.2.2/sceptre/cli/list.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.2.1/sceptre/cli/new.py` & `sceptre-4.2.2/sceptre/cli/new.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.2.1/sceptre/cli/policy.py` & `sceptre-4.2.2/sceptre/cli/policy.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.2.1/sceptre/cli/prune.py` & `sceptre-4.2.2/sceptre/cli/prune.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.2.1/sceptre/cli/status.py` & `sceptre-4.2.2/sceptre/cli/status.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.2.1/sceptre/cli/template.py` & `sceptre-4.2.2/sceptre/cli/template.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.2.1/sceptre/cli/update.py` & `sceptre-4.2.2/sceptre/cli/update.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.2.1/sceptre/config/graph.py` & `sceptre-4.2.2/sceptre/config/graph.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.2.1/sceptre/config/reader.py` & `sceptre-4.2.2/sceptre/config/reader.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.2.1/sceptre/config/strategies.py` & `sceptre-4.2.2/sceptre/config/strategies.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.2.1/sceptre/connection_manager.py` & `sceptre-4.2.2/sceptre/connection_manager.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.2.1/sceptre/context.py` & `sceptre-4.2.2/sceptre/context.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.2.1/sceptre/diffing/diff_writer.py` & `sceptre-4.2.2/sceptre/diffing/diff_writer.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.2.1/sceptre/diffing/stack_differ.py` & `sceptre-4.2.2/sceptre/diffing/stack_differ.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.2.1/sceptre/exceptions.py` & `sceptre-4.2.2/sceptre/exceptions.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.2.1/sceptre/helpers.py` & `sceptre-4.2.2/sceptre/helpers.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.2.1/sceptre/hooks/__init__.py` & `sceptre-4.2.2/sceptre/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.2.1/sceptre/hooks/asg_scaling_processes.py` & `sceptre-4.2.2/sceptre/hooks/asg_scaling_processes.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.2.1/sceptre/hooks/cmd.py` & `sceptre-4.2.2/sceptre/hooks/cmd.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.2.1/sceptre/logging.py` & `sceptre-4.2.2/sceptre/logging.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.2.1/sceptre/plan/actions.py` & `sceptre-4.2.2/sceptre/plan/actions.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.2.1/sceptre/plan/executor.py` & `sceptre-4.2.2/sceptre/plan/executor.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.2.1/sceptre/plan/plan.py` & `sceptre-4.2.2/sceptre/plan/plan.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.2.1/sceptre/resolvers/__init__.py` & `sceptre-4.2.2/sceptre/resolvers/__init__.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.2.1/sceptre/resolvers/environment_variable.py` & `sceptre-4.2.2/sceptre/resolvers/environment_variable.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.2.1/sceptre/resolvers/file_contents.py` & `sceptre-4.2.2/sceptre/resolvers/file_contents.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.2.1/sceptre/resolvers/join.py` & `sceptre-4.2.2/sceptre/resolvers/join.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.2.1/sceptre/resolvers/no_value.py` & `sceptre-4.2.2/sceptre/resolvers/no_value.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.2.1/sceptre/resolvers/placeholders.py` & `sceptre-4.2.2/sceptre/resolvers/placeholders.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.2.1/sceptre/resolvers/select.py` & `sceptre-4.2.2/sceptre/resolvers/select.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.2.1/sceptre/resolvers/split.py` & `sceptre-4.2.2/sceptre/resolvers/split.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.2.1/sceptre/resolvers/stack_attr.py` & `sceptre-4.2.2/sceptre/resolvers/stack_attr.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.2.1/sceptre/resolvers/stack_output.py` & `sceptre-4.2.2/sceptre/resolvers/stack_output.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.2.1/sceptre/resolvers/sub.py` & `sceptre-4.2.2/sceptre/resolvers/sub.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.2.1/sceptre/stack.py` & `sceptre-4.2.2/sceptre/stack.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.2.1/sceptre/stack_status.py` & `sceptre-4.2.2/sceptre/stack_status.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.2.1/sceptre/stack_status_colourer.py` & `sceptre-4.2.2/sceptre/stack_status_colourer.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.2.1/sceptre/template.py` & `sceptre-4.2.2/sceptre/template.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.2.1/sceptre/template_handlers/__init__.py` & `sceptre-4.2.2/sceptre/template_handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.2.1/sceptre/template_handlers/file.py` & `sceptre-4.2.2/sceptre/template_handlers/file.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.2.1/sceptre/template_handlers/helper.py` & `sceptre-4.2.2/sceptre/template_handlers/helper.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.2.1/sceptre/template_handlers/http.py` & `sceptre-4.2.2/sceptre/template_handlers/http.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.2.1/sceptre/template_handlers/s3.py` & `sceptre-4.2.2/sceptre/template_handlers/s3.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.2.1/setup.py` & `sceptre-4.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,25 +11,25 @@
  'sceptre.resolvers',
  'sceptre.template_handlers']
 
 package_data = \
 {'': ['*'], 'sceptre': ['stack_policies/*']}
 
 install_requires = \
-['boto3>=1.3.0,<2',
+['boto3>=1.20.27,<2.0.0',
  'cfn-flip>=1.2.3,<2.0.0',
  'click>=7.0,<9.0',
  'colorama>=0.2.5,<0.4.4',
  'deepdiff>=5.5,<6.0',
  'deprecation>=2.0,<3.0',
  'jinja2>=3.0,<4.0',
  'jsonschema>=3.2,<3.3',
  'networkx>=2.6,<2.7',
  'packaging>=16.8,<22.0',
- 'pyyaml>=5.1,<6.0',
+ 'pyyaml>=6.0,<7.0',
  'sceptre-cmd-resolver>=2.0,<3.0',
  'sceptre-file-resolver>=1.0,<2.0']
 
 extras_require = \
 {'docs': ['sphinx>=1.6.5,<=5.1.1',
           'sphinx-click>=2.0.1,<4.0.0',
           'sphinx-rtd-theme==0.5.2',
@@ -58,15 +58,15 @@
                        'sub = sceptre.resolvers.sub:Sub'],
  'sceptre.template_handlers': ['file = sceptre.template_handlers.file:File',
                                'http = sceptre.template_handlers.http:Http',
                                's3 = sceptre.template_handlers.s3:S3']}
 
 setup_kwargs = {
     'name': 'sceptre',
-    'version': '4.2.1',
+    'version': '4.2.2',
     'description': 'An AWS Cloud Provisioning Tool',
     'long_description': '# Sceptre\n\n[![CircleCI](https://img.shields.io/circleci/build/github/Sceptre/sceptre?logo=circleci)](https://app.circleci.com/pipelines/github/Sceptre)\n[![Docker Image Version (latest semver)](https://img.shields.io/docker/v/sceptreorg/sceptre?logo=docker&sort=semver)](https://hub.docker.com/r/sceptreorg/sceptre)\n[![PyPI](https://img.shields.io/pypi/v/sceptre?logo=pypi)](https://pypi.org/project/sceptre/)\n[![PyPI - Status](https://img.shields.io/pypi/status/sceptre?logo=pypi)](https://pypi.org/project/sceptre/)\n[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/sceptre?logo=pypi)](https://pypi.org/project/sceptre/)\n[![PyPI - Downloads](https://img.shields.io/pypi/dm/sceptre?logo=pypi)](https://pypi.org/project/sceptre/)\n[![License](https://img.shields.io/pypi/l/sceptre?logo=apache)](https://github.com/Sceptre/sceptre/blob/main/LICENSE)\n\n## About\n\nSceptre is a tool to drive\n[AWS CloudFormation](https://aws.amazon.com/cloudformation). It automates the\nmundane, repetitive and error-prone tasks, enabling you to concentrate on\nbuilding better infrastructure.\n\n## Features\n\n- Code reuse by separating a Stack\'s template and its configuration\n- Support for templates written in JSON, YAML, Jinja2 or Python DSLs such as\n  Troposphere\n- Dependency resolution by passing of Stack outputs to parameters of dependent\n  Stacks\n- Stack Group support by bundling related Stacks into logical groups (e.g. dev\n  and prod)\n- Stack Group-level commands, such as creating multiple Stacks with a single\n  command\n- Fast, highly parallelised builds\n- Built in support for working with Stacks in multiple AWS accounts and regions\n- Infrastructure visibility with meta-operations such as Stack querying\n  protection\n- Support for inserting dynamic values in templates via customisable Resolvers\n- Support for running arbitrary code as Hooks before/after Stack builds\n\n## Benefits\n\n- Utilises cloud-native Infrastructure as Code engines (CloudFormation)\n- You do not need to manage state\n- Simple templates using popular templating syntax - Yaml & Jinja\n- Powerful flexibility using a mature programming language - Python\n- Easy to integrate as part of a CI/CD pipeline by using Hooks\n- Simple CLI and API\n- Unopinionated - Sceptre does not force a specific project structure\n\n## Install\n\n### Using pip\n\n`$ pip install sceptre`\n\nMore information on installing sceptre can be found in our\n[Installation Guide](https://docs.sceptre-project.org/latest/docs/install.html)\n\n### Using Docker Image\n\nView our [Docker repository](https://hub.docker.com/repositories/sceptreorg).\nImages available from version 2.0.0 onward.\n\nTo use our Docker image follow these instructions:\n\n1. Pull the image `docker pull sceptreorg/sceptre:[SCEPTRE_VERSION_NUMBER]` e.g.\n   `docker pull sceptreorg/sceptre:2.5.0`. Leave out the version number if you\n   wish to run `latest` or run `docker pull sceptreorg/sceptre:latest`.\n\n2. Run the image. You will need to mount the working directory where your\n   project resides to a directory called `project`. You will also need to mount\n   a volume with your AWS config to your docker container. E.g.\n\n`docker run -v $(pwd):/project -v /Users/me/.aws/:/root/.aws/:ro sceptreorg/sceptre:latest --help`\n\nIf you want to use a custom ENTRYPOINT simply amend the Docker command:\n\n`docker run -ti --entrypoint=\'\' sceptreorg/sceptre:latest sh`\n\nThe above command will enter you into the shell of the Docker container where\nyou can execute sceptre commands - useful for development.\n\nIf you have any other environment variables in your non-docker shell you will\nneed to pass these in on the Docker CLI using the `-e` flag. See Docker\ndocumentation on how to achieve this.\n\n## Example\n\nSceptre organises Stacks into "Stack Groups". Each Stack is represented by a\nYAML configuration file stored in a directory which represents the Stack Group.\nHere, we have two Stacks, `vpc` and `subnets`, in a Stack Group named `dev`:\n\n```sh\n$ tree\n.\n├── config\n│\xa0\xa0 └── dev\n│\xa0\xa0      ├── config.yaml\n│\xa0\xa0      ├── subnets.yaml\n│\xa0\xa0      └── vpc.yaml\n└── templates\n    ├── subnets.py\n    └── vpc.py\n```\n\nWe can create a Stack with the `create` command. This `vpc` Stack contains a\nVPC.\n\n```sh\n$ sceptre create dev/vpc.yaml\n\ndev/vpc - Creating stack dev/vpc\nVirtualPrivateCloud AWS::EC2::VPC CREATE_IN_PROGRESS\ndev/vpc VirtualPrivateCloud AWS::EC2::VPC CREATE_COMPLETE\ndev/vpc sceptre-demo-dev-vpc AWS::CloudFormation::Stack CREATE_COMPLETE\n```\n\nThe `subnets` Stack contains a subnet which must be created in the VPC. To do\nthis, we need to pass the VPC ID, which is exposed as a Stack output of the\n`vpc` Stack, to a parameter of the `subnets` Stack. Sceptre automatically\nresolves this dependency for us.\n\n```sh\n$ sceptre create dev/subnets.yaml\ndev/subnets - Creating stack\ndev/subnets Subnet AWS::EC2::Subnet CREATE_IN_PROGRESS\ndev/subnets Subnet AWS::EC2::Subnet CREATE_COMPLETE\ndev/subnets sceptre-demo-dev-subnets AWS::CloudFormation::Stack CREATE_COMPLETE\n```\n\nSceptre implements meta-operations, which allow us to find out information about\nour Stacks:\n\n```sh\n$ sceptre list resources dev/subnets.yaml\n\n- LogicalResourceId: Subnet\n  PhysicalResourceId: subnet-445e6e32\n  dev/vpc:\n- LogicalResourceId: VirtualPrivateCloud\n  PhysicalResourceId: vpc-c4715da0\n```\n\nSceptre provides Stack Group level commands. This one deletes the whole `dev`\nStack Group. The subnet exists within the vpc, so it must be deleted first.\nSceptre handles this automatically:\n\n```sh\n$ sceptre delete dev\n\nDeleting stack\ndev/subnets Subnet AWS::EC2::Subnet DELETE_IN_PROGRESS\ndev/subnets - Stack deleted\ndev/vpc Deleting stack\ndev/vpc VirtualPrivateCloud AWS::EC2::VPC DELETE_IN_PROGRESS\ndev/vpc - Stack deleted\n```\n\n> Note: Deleting Stacks will _only_ delete a given Stack, or the Stacks that are\n> directly in a given StackGroup. By default Stack dependencies that are\n> external to the StackGroup are not deleted.\n\nSceptre can also handle cross Stack Group dependencies, take the following\nexample project:\n\n```sh\n$ tree\n.\n├── config\n│\xa0\xa0 ├── dev\n│\xa0\xa0 │\xa0\xa0 ├── network\n│\xa0\xa0 │\xa0\xa0 │\xa0\xa0 └── vpc.yaml\n│\xa0\xa0 │\xa0\xa0 ├── users\n│\xa0\xa0 │\xa0\xa0 │\xa0\xa0 └── iam.yaml\n│\xa0\xa0 │\xa0\xa0 ├── compute\n│\xa0\xa0 │\xa0\xa0 │\xa0\xa0 └── ec2.yaml\n│\xa0\xa0 │\xa0\xa0 └── config.yaml\n│\xa0\xa0 └── staging\n│\xa0\xa0     └── eu\n│\xa0\xa0         ├── config.yaml\n│\xa0\xa0         └── stack.yaml\n├── hooks\n│\xa0\xa0 └── stack.py\n├── templates\n│\xa0\xa0 ├── network.json\n│\xa0\xa0 ├── iam.json\n│\xa0\xa0 ├── ec2.json\n│\xa0\xa0 └── stack.json\n└── vars\n    ├── dev.yaml\n    └── staging.yaml\n```\n\nIn this project `staging/eu/stack.yaml` has a dependency on the output of\n`dev/users/iam.yaml`. If you wanted to create the Stack `staging/eu/stack.yaml`,\nSceptre will resolve all of it\'s dependencies, including `dev/users/iam.yaml`,\nbefore attempting to create the Stack.\n\n## Usage\n\nSceptre can be used from the CLI, or imported as a Python package.\n\n## CLI\n\n```text\nUsage: sceptre [OPTIONS] COMMAND [ARGS]...\n\n  Sceptre is a tool to manage your cloud native infrastructure deployments.\n\nOptions:\n  --version                  Show the version and exit.\n  --debug                    Turn on debug logging.\n  --dir TEXT                 Specify sceptre directory.\n  --output [text|yaml|json]  The formatting style for command output.\n  --no-colour                Turn off output colouring.\n  --var TEXT                 A variable to replace the value of an item in\n                             config file.\n  --var-file FILENAME        A YAML file of variables to replace the values\n                             of items in config files.\n  --ignore-dependencies      Ignore dependencies when executing command.\n  --merge-vars               Merge variables from successive --vars and var\n                             files.\n  --help                     Show this message and exit.\n\nCommands:\n  create         Creates a stack or a change set.\n  delete         Deletes a stack or a change set.\n  describe       Commands for describing attributes of stacks.\n  estimate-cost  Estimates the cost of the template.\n  execute        Executes a Change Set.\n  generate       Prints the template.\n  launch         Launch a Stack or StackGroup.\n  list           Commands for listing attributes of stacks.\n  new            Commands for initialising Sceptre projects.\n  set-policy     Sets Stack policy.\n  status         Print status of stack or stack_group.\n  update         Update a stack.\n  validate       Validates the template.\n```\n\n## Python\n\nUsing Sceptre as a Python module is very straightforward. You need to create a\nSceptreContext, which tells Sceptre where your project path is and which path\nyou want to execute on, we call this the "command path".\n\nAfter you have created a SceptreContext you need to pass this into a\nSceptrePlan. On instantiation the SceptrePlan will handle all the required steps\nto make sure the action you wish to take on the command path are resolved.\n\nAfter you have instantiated a SceptrePlan you can access all the actions you can\ntake on a Stack, such as `validate()`, `launch()`, `list()` and `delete()`.\n\n```python\nfrom sceptre.context import SceptreContext\nfrom sceptre.plan.plan import SceptrePlan\n\ncontext = SceptreContext("/path/to/project", "command_path")\nplan = SceptrePlan(context)\nplan.launch()\n```\n\nFull API reference documentation can be found in the\n[Documentation](https://docs.sceptre-project.org/)\n\n## Tutorial and Documentation\n\n- [Get Started](https://docs.sceptre-project.org/latest/docs/get_started.html)\n- [Documentation](https://docs.sceptre-project.org/)\n\n## Communication\n\nSceptre community discussions happen in the #sceptre chanel in the\n[og-aws Slack](https://github.com/open-guides/og-aws).  To join click\non <http://slackhatesthe.cloud/> to create an account and join the\n#sceptre channel.\n\nFollow the [SceptreOrg Twitter account](https://twitter.com/SceptreOrg) to get announcements on the latest releases.\n\n## Contributing\n\nSee our [Contributing Guide](CONTRIBUTING.md)\n\n\n## Sponsors\n\n[![Sage Bionetworks](sponsors/sage_bionetworks_logo.png "Sage Bionetworks")](https://sagebionetworks.org)\n\n[![GoDaddy](sponsors/godaddy_logo.png "GoDaddy")](https://www.godaddy.com)\n\n[![Cloudreach](sponsors/cloudreach_logo.png "Cloudreach")](https://www.cloudreach.com)\n',
     'author': 'Sceptre',
     'author_email': 'sceptreorg@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/Sceptre/sceptre',
```

### Comparing `sceptre-4.2.1/PKG-INFO` & `sceptre-4.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sceptre
-Version: 4.2.1
+Version: 4.2.2
 Summary: An AWS Cloud Provisioning Tool
 Home-page: https://github.com/Sceptre/sceptre
 License: Apache-2.0
 Keywords: aws,cloud,devops,infrastructure,tools,cli
 Author: Sceptre
 Author-email: sceptreorg@gmail.com
 Requires-Python: >=3.7,<3.12
@@ -22,26 +22,26 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Provides-Extra: docs
 Provides-Extra: troposphere
-Requires-Dist: boto3 (>=1.3.0,<2)
+Requires-Dist: boto3 (>=1.20.27,<2.0.0)
 Requires-Dist: cfn-flip (>=1.2.3,<2.0.0)
 Requires-Dist: click (>=7.0,<9.0)
 Requires-Dist: colorama (>=0.2.5,<0.4.4)
 Requires-Dist: deepdiff (>=5.5,<6.0)
 Requires-Dist: deprecation (>=2.0,<3.0)
 Requires-Dist: docutils (<0.17) ; extra == "docs"
 Requires-Dist: jinja2 (>=3.0,<4.0)
 Requires-Dist: jsonschema (>=3.2,<3.3)
 Requires-Dist: networkx (>=2.6,<2.7)
 Requires-Dist: packaging (>=16.8,<22.0)
-Requires-Dist: pyyaml (>=5.1,<6.0)
+Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: sceptre-cmd-resolver (>=2.0,<3.0)
 Requires-Dist: sceptre-file-resolver (>=1.0,<2.0)
 Requires-Dist: sphinx (>=1.6.5,<=5.1.1) ; extra == "docs"
 Requires-Dist: sphinx-autodoc-typehints (==1.19.2) ; extra == "docs"
 Requires-Dist: sphinx-click (>=2.0.1,<4.0.0) ; extra == "docs"
 Requires-Dist: sphinx-rtd-theme (==0.5.2) ; extra == "docs"
 Requires-Dist: troposphere (>=4,<5) ; extra == "troposphere"
```

