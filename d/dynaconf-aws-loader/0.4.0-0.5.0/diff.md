# Comparing `tmp/dynaconf_aws_loader-0.4.0.tar.gz` & `tmp/dynaconf_aws_loader-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynaconf_aws_loader-0.4.0.tar", max compression
+gzip compressed data, was "dynaconf_aws_loader-0.5.0.tar", max compression
```

## Comparing `dynaconf_aws_loader-0.4.0.tar` & `dynaconf_aws_loader-0.5.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      965 2023-06-22 21:50:27.706709 dynaconf_aws_loader-0.4.0/CHANGELOG.md
--rw-r--r--   0        0        0     1072 2023-06-22 21:50:27.706709 dynaconf_aws_loader-0.4.0/LICENSE
--rw-r--r--   0        0        0     7962 2023-06-22 21:50:27.706709 dynaconf_aws_loader-0.4.0/README.rst
--rw-r--r--   0        0        0      369 2023-06-22 21:50:27.706709 dynaconf_aws_loader-0.4.0/dynaconf_aws_loader/__init__.py
--rw-r--r--   0        0        0     8797 2023-06-22 21:50:27.706709 dynaconf_aws_loader-0.4.0/dynaconf_aws_loader/loader.py
--rw-r--r--   0        0        0     1752 2023-06-22 21:50:27.706709 dynaconf_aws_loader-0.4.0/dynaconf_aws_loader/util.py
--rw-r--r--   0        0        0     1249 2023-06-22 21:50:27.710709 dynaconf_aws_loader-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     9054 1970-01-01 00:00:00.000000 dynaconf_aws_loader-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1340 2023-07-21 00:35:19.082614 dynaconf_aws_loader-0.5.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1072 2023-07-21 00:35:19.082614 dynaconf_aws_loader-0.5.0/LICENSE
+-rw-r--r--   0        0        0     7962 2023-07-21 00:35:19.082614 dynaconf_aws_loader-0.5.0/README.rst
+-rw-r--r--   0        0        0     1138 2023-07-21 00:35:19.082614 dynaconf_aws_loader-0.5.0/dynaconf_aws_loader/__init__.py
+-rw-r--r--   0        0        0     9522 2023-07-21 00:35:19.082614 dynaconf_aws_loader-0.5.0/dynaconf_aws_loader/loader.py
+-rw-r--r--   0        0        0     1752 2023-07-21 00:35:19.082614 dynaconf_aws_loader-0.5.0/dynaconf_aws_loader/util.py
+-rw-r--r--   0        0        0     1313 2023-07-21 00:35:19.082614 dynaconf_aws_loader-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     9054 1970-01-01 00:00:00.000000 dynaconf_aws_loader-0.5.0/PKG-INFO
```

### Comparing `dynaconf_aws_loader-0.4.0/CHANGELOG.md` & `dynaconf_aws_loader-0.5.0/CHANGELOG.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,25 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
+## [0.5.0] - 2023-07-20
+
+### Bug Fixes
+
+- Actually allow single-parameter loading to work
+
+### Miscellaneous Tasks
+
+- Reorganize Action workflow to utilize python cache
+- Add additional unit-ish tests for loader
+- Handle loader identifier changes between Dynaconf 3.1->3.2
+- Update workflow to utilize Dynaconf versions in test matrix
+- Replace warn logging with info/error
+
 ## [0.4.0] - 2023-06-22
 
 ### Bug Fixes
 
 - Add missing cleanup for parameter deletion
 
 ### Features
```

### Comparing `dynaconf_aws_loader-0.4.0/LICENSE` & `dynaconf_aws_loader-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dynaconf_aws_loader-0.4.0/README.rst` & `dynaconf_aws_loader-0.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `dynaconf_aws_loader-0.4.0/dynaconf_aws_loader/loader.py` & `dynaconf_aws_loader-0.5.0/dynaconf_aws_loader/loader.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 import os
 import logging
 import boto3
 from botocore.exceptions import ClientError, BotoCoreError, NoRegionError
 
 from dynaconf.utils.parse_conf import parse_conf_data
 
-from . import IDENTIFIER
 from .util import slashes_to_dict, pull_from_env_or_obj
+from . import generate_loader_identifier
 
 if t.TYPE_CHECKING:
     from mypy_boto3_ssm.client import SSMClient
     from dynaconf.base import Settings
 
 
 logger = logging.getLogger("dynaconf.aws_loader")
@@ -137,20 +137,23 @@
     for env_name in env_list:
         env_name = env_name.lower()
         path = f"/{project_prefix}/{env_name}"
 
         if namespace_prefix is not None:
             path = f"{path}/{namespace_prefix}"
 
+        loader_identifier = generate_loader_identifier(path, env)
+
         if key is not None:
             value = _fetch_single_parameter(
                 client,
                 project_prefix=project_prefix,
                 env_name=env_name,
                 namespace_prefix=namespace_prefix,
+                key=key,
                 silent=silent,
             )
             if value:
                 obj.set(key, value, validate=validate)
 
             return
         else:
@@ -160,22 +163,23 @@
             normal_results = _fetch_all_parameters(
                 client=client,
                 project_prefix=project_prefix,
                 env_name=env_name,
                 namespace_prefix=None,
                 silent=silent,
             )
+
             if normal_results:
                 filter_strategy = obj.get("AWS_SSM_NAMESPACE_FILTER_STRATEGY")
                 if filter_strategy:
                     normal_results = filter_strategy(normal_results)
 
                 obj.update(
                     normal_results,
-                    loader_identifier=IDENTIFIER,
+                    loader_identifier=loader_identifier,
                     validate=validate,
                 )
 
             if namespace_prefix is not None:
                 namespaced_results = _fetch_all_parameters(
                     client=client,
                     project_prefix=project_prefix,
@@ -183,55 +187,66 @@
                     namespace_prefix=namespace_prefix,
                     silent=silent,
                 )
 
                 if namespaced_results:
                     obj.update(
                         namespaced_results,
-                        loader_identifier=IDENTIFIER,
+                        loader_identifier=loader_identifier,
                         validate=validate,
                     )
 
 
 def _fetch_single_parameter(
     client,
     project_prefix: str,
     env_name: str,
-    namespace_prefix: str | None,
+    key: str,
+    namespace_prefix: str | None = None,
     silent: bool = True,
 ):
     """
     Fetch single parameter by path.
     """
 
     path = f"/{project_prefix}/{env_name}"
     if namespace_prefix is not None:
         path = f"{path}/{namespace_prefix}"
 
+    path = f"{path}/{key}"
+
     logger.debug("Attempting to load a single parameter %s from AWS SSM" % path)
 
     try:
         value = client.get_parameter(Name=path, WithDecryption=True)
-    except (ClientError, BotoCoreError) as exc:
-        logger.warn("Could not connect to AWS SSM.", exc_info=exc)
+    except ClientError as exc:
         if silent:
             return
+        if exc.response.get("Error", {}).get("Code") == "ParameterNotFound":
+            logger.info("Parameter with path %s does not exist in AWS SSM." % path)
+        raise
+    except BotoCoreError:
+        if silent:
+            return
+        logger.error(
+            "Could not connect to AWS SSM at endpoint %s." % client.meta.endpoint_url
+        )
         raise
 
     if data := value.get("Parameter"):
         value = parse_conf_data(data["Value"], tomlfy=True)
 
     return value
 
 
 def _fetch_all_parameters(
     client,
     project_prefix: str,
     env_name: str,
-    namespace_prefix: str | None,
+    namespace_prefix: str | None = None,
     silent: bool = True,
 ):
     """
     Fetch all keys by path segment.
     """
 
     path = f"/{project_prefix}/{env_name}"
@@ -244,18 +259,26 @@
     paginator = client.get_paginator("get_parameters_by_path")
 
     try:
         for page in paginator.paginate(Path=path, Recursive=True, WithDecryption=True):
             for parameter in page["Parameters"]:
                 data.append({parameter["Name"]: parameter["Value"]})
 
-    except (ClientError, BotoCoreError) as exc:
-        logger.warn("Could not connect to AWS SSM.", exc_info=exc)
+    except ClientError as exc:
         if silent:
             return
+        if exc.response.get("Error", {}).get("Code") == "ParameterNotFound":
+            logger.info("Parameter with path %s does not exist in AWS SSM." % path)
+        raise
+    except BotoCoreError:
+        if silent:
+            return
+        logger.error(
+            "Could not connect to AWS SSM at endpoint %s." % client.meta.endpoint_url
+        )
         raise
 
     result = parse_conf_data(data=slashes_to_dict(data), tomlfy=True)
 
     if result and project_prefix in result:
         # Prune out the prefixes before setting on the object
         result = result[project_prefix]
```

### Comparing `dynaconf_aws_loader-0.4.0/dynaconf_aws_loader/util.py` & `dynaconf_aws_loader-0.5.0/dynaconf_aws_loader/util.py`

 * *Files identical despite different names*

### Comparing `dynaconf_aws_loader-0.4.0/pyproject.toml` & `dynaconf_aws_loader-0.5.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dynaconf-aws-loader"
-version = "0.4.0"
+version = "0.5.0"
 description = "A custom loader for Dynaconf that uses AWS Systems Manager Parameter Store as a source of truth."
 homepage = "https://github.com/fictivekin/dynaconf-aws-loader"
 repository = "https://github.com/fictivekin/dynaconf-aws-loader"
 authors = [
     "Joël Perras <joel@fictivekin.com>",
 ]
 readme = "README.rst"
@@ -31,14 +31,18 @@
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 lovely-pytest-docker = "^0.3.1"
 boto3-stubs = {extras = ["ssm"], version = "^1.26"}
 localstack-client = "^2.1"
 pytest-env = "^0.8.1"
 
+
+[tool.poetry.group.test.dependencies]
+pytest-mock = "^3.11.1"
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 minversion = "7.0"
 addopts = "-ra"
```

### Comparing `dynaconf_aws_loader-0.4.0/PKG-INFO` & `dynaconf_aws_loader-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynaconf-aws-loader
-Version: 0.4.0
+Version: 0.5.0
 Summary: A custom loader for Dynaconf that uses AWS Systems Manager Parameter Store as a source of truth.
 Home-page: https://github.com/fictivekin/dynaconf-aws-loader
 License: MIT
 Keywords: dynaconf,AWS,SSM
 Author: Joël Perras
 Author-email: joel@fictivekin.com
 Requires-Python: >=3.8,<4.0
```

