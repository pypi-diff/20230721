# Comparing `tmp/wiremind-kubernetes-7.2.0.tar.gz` & `tmp/wiremind-kubernetes-7.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wiremind-kubernetes-7.2.0.tar", last modified: Thu Jun 22 12:34:04 2023, max compression
+gzip compressed data, was "wiremind-kubernetes-7.3.0.tar", last modified: Fri Jul 21 10:38:05 2023, max compression
```

## Comparing `wiremind-kubernetes-7.2.0.tar` & `wiremind-kubernetes-7.3.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:34:04.231086 wiremind-kubernetes-7.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     7642 2023-06-22 12:33:48.000000 wiremind-kubernetes-7.2.0/LICENCE.md
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-22 12:33:48.000000 wiremind-kubernetes-7.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-06-22 12:34:04.231086 wiremind-kubernetes-7.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-06-22 12:33:48.000000 wiremind-kubernetes-7.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-22 12:33:48.000000 wiremind-kubernetes-7.2.0/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-22 12:33:48.000000 wiremind-kubernetes-7.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-06-22 12:34:04.231086 wiremind-kubernetes-7.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-06-22 12:33:48.000000 wiremind-kubernetes-7.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:34:04.227086 wiremind-kubernetes-7.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:34:04.231086 wiremind-kubernetes-7.2.0/src/wiremind_kubernetes/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-22 12:33:48.000000 wiremind-kubernetes-7.2.0/src/wiremind_kubernetes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-22 12:33:48.000000 wiremind-kubernetes-7.2.0/src/wiremind_kubernetes/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-06-22 12:33:48.000000 wiremind-kubernetes-7.2.0/src/wiremind_kubernetes/kube_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-06-22 12:33:48.000000 wiremind-kubernetes-7.2.0/src/wiremind_kubernetes/kubernetes_client_additional_arguments.py
--rw-r--r--   0 runner    (1001) docker     (123)    19825 2023-06-22 12:33:48.000000 wiremind-kubernetes-7.2.0/src/wiremind_kubernetes/kubernetes_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:34:04.231086 wiremind-kubernetes-7.2.0/src/wiremind_kubernetes/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 12:33:48.000000 wiremind-kubernetes-7.2.0/src/wiremind_kubernetes/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:34:04.231086 wiremind-kubernetes-7.2.0/src/wiremind_kubernetes/tests/e2e_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 12:33:48.000000 wiremind-kubernetes-7.2.0/src/wiremind_kubernetes/tests/e2e_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-06-22 12:33:48.000000 wiremind-kubernetes-7.2.0/src/wiremind_kubernetes/tests/e2e_tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-06-22 12:33:48.000000 wiremind-kubernetes-7.2.0/src/wiremind_kubernetes/tests/e2e_tests/create_job_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-06-22 12:33:48.000000 wiremind-kubernetes-7.2.0/src/wiremind_kubernetes/tests/e2e_tests/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-06-22 12:33:48.000000 wiremind-kubernetes-7.2.0/src/wiremind_kubernetes/tests/e2e_tests/start_stop_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:34:04.231086 wiremind-kubernetes-7.2.0/src/wiremind_kubernetes/tests/unit_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 12:33:48.000000 wiremind-kubernetes-7.2.0/src/wiremind_kubernetes/tests/unit_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-06-22 12:33:48.000000 wiremind-kubernetes-7.2.0/src/wiremind_kubernetes/tests/unit_tests/kube_config_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-06-22 12:33:48.000000 wiremind-kubernetes-7.2.0/src/wiremind_kubernetes/tests/unit_tests/kubernetes_client_additional_arguments_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-06-22 12:33:48.000000 wiremind-kubernetes-7.2.0/src/wiremind_kubernetes/tests/unit_tests/kubernetes_deployment_manager_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-06-22 12:33:48.000000 wiremind-kubernetes-7.2.0/src/wiremind_kubernetes/tests/unit_tests/namespaced_kubernetes_helper_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:34:04.231086 wiremind-kubernetes-7.2.0/src/wiremind_kubernetes/tests/unit_tests/utils_test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 12:33:48.000000 wiremind-kubernetes-7.2.0/src/wiremind_kubernetes/tests/unit_tests/utils_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-06-22 12:33:48.000000 wiremind-kubernetes-7.2.0/src/wiremind_kubernetes/tests/unit_tests/utils_test/retry_kubernetes_request_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4348 2023-06-22 12:33:48.000000 wiremind-kubernetes-7.2.0/src/wiremind_kubernetes/tests/unit_tests/utils_test/run_command_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3887 2023-06-22 12:33:48.000000 wiremind-kubernetes-7.2.0/src/wiremind_kubernetes/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:34:04.231086 wiremind-kubernetes-7.2.0/src/wiremind_kubernetes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-06-22 12:34:04.000000 wiremind-kubernetes-7.2.0/src/wiremind_kubernetes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-06-22 12:34:04.000000 wiremind-kubernetes-7.2.0/src/wiremind_kubernetes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 12:34:04.000000 wiremind-kubernetes-7.2.0/src/wiremind_kubernetes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-22 12:34:04.000000 wiremind-kubernetes-7.2.0/src/wiremind_kubernetes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-22 12:34:04.000000 wiremind-kubernetes-7.2.0/src/wiremind_kubernetes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 12:34:04.000000 wiremind-kubernetes-7.2.0/src/wiremind_kubernetes.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:38:05.882237 wiremind-kubernetes-7.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     7642 2023-07-21 10:37:54.000000 wiremind-kubernetes-7.3.0/LICENCE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-21 10:37:54.000000 wiremind-kubernetes-7.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-21 10:38:05.882237 wiremind-kubernetes-7.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-07-21 10:37:54.000000 wiremind-kubernetes-7.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-21 10:37:54.000000 wiremind-kubernetes-7.3.0/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-21 10:37:54.000000 wiremind-kubernetes-7.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-07-21 10:38:05.882237 wiremind-kubernetes-7.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-07-21 10:37:54.000000 wiremind-kubernetes-7.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:38:05.874236 wiremind-kubernetes-7.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:38:05.878237 wiremind-kubernetes-7.3.0/src/wiremind_kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-21 10:37:54.000000 wiremind-kubernetes-7.3.0/src/wiremind_kubernetes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-21 10:37:54.000000 wiremind-kubernetes-7.3.0/src/wiremind_kubernetes/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-07-21 10:37:54.000000 wiremind-kubernetes-7.3.0/src/wiremind_kubernetes/kube_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-07-21 10:37:54.000000 wiremind-kubernetes-7.3.0/src/wiremind_kubernetes/kubernetes_client_additional_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19836 2023-07-21 10:37:54.000000 wiremind-kubernetes-7.3.0/src/wiremind_kubernetes/kubernetes_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:38:05.878237 wiremind-kubernetes-7.3.0/src/wiremind_kubernetes/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 10:37:54.000000 wiremind-kubernetes-7.3.0/src/wiremind_kubernetes/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:38:05.878237 wiremind-kubernetes-7.3.0/src/wiremind_kubernetes/tests/e2e_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 10:37:54.000000 wiremind-kubernetes-7.3.0/src/wiremind_kubernetes/tests/e2e_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-07-21 10:37:54.000000 wiremind-kubernetes-7.3.0/src/wiremind_kubernetes/tests/e2e_tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-07-21 10:37:54.000000 wiremind-kubernetes-7.3.0/src/wiremind_kubernetes/tests/e2e_tests/create_job_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-07-21 10:37:54.000000 wiremind-kubernetes-7.3.0/src/wiremind_kubernetes/tests/e2e_tests/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-07-21 10:37:54.000000 wiremind-kubernetes-7.3.0/src/wiremind_kubernetes/tests/e2e_tests/start_stop_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:38:05.882237 wiremind-kubernetes-7.3.0/src/wiremind_kubernetes/tests/unit_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 10:37:54.000000 wiremind-kubernetes-7.3.0/src/wiremind_kubernetes/tests/unit_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-07-21 10:37:54.000000 wiremind-kubernetes-7.3.0/src/wiremind_kubernetes/tests/unit_tests/kube_config_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-07-21 10:37:54.000000 wiremind-kubernetes-7.3.0/src/wiremind_kubernetes/tests/unit_tests/kubernetes_client_additional_arguments_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-07-21 10:37:54.000000 wiremind-kubernetes-7.3.0/src/wiremind_kubernetes/tests/unit_tests/kubernetes_deployment_manager_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-07-21 10:37:54.000000 wiremind-kubernetes-7.3.0/src/wiremind_kubernetes/tests/unit_tests/namespaced_kubernetes_helper_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:38:05.882237 wiremind-kubernetes-7.3.0/src/wiremind_kubernetes/tests/unit_tests/utils_test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 10:37:54.000000 wiremind-kubernetes-7.3.0/src/wiremind_kubernetes/tests/unit_tests/utils_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-07-21 10:37:54.000000 wiremind-kubernetes-7.3.0/src/wiremind_kubernetes/tests/unit_tests/utils_test/retry_kubernetes_request_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4348 2023-07-21 10:37:54.000000 wiremind-kubernetes-7.3.0/src/wiremind_kubernetes/tests/unit_tests/utils_test/run_command_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3887 2023-07-21 10:37:54.000000 wiremind-kubernetes-7.3.0/src/wiremind_kubernetes/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:38:05.878237 wiremind-kubernetes-7.3.0/src/wiremind_kubernetes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-21 10:38:05.000000 wiremind-kubernetes-7.3.0/src/wiremind_kubernetes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-07-21 10:38:05.000000 wiremind-kubernetes-7.3.0/src/wiremind_kubernetes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 10:38:05.000000 wiremind-kubernetes-7.3.0/src/wiremind_kubernetes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-21 10:38:05.000000 wiremind-kubernetes-7.3.0/src/wiremind_kubernetes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-21 10:38:05.000000 wiremind-kubernetes-7.3.0/src/wiremind_kubernetes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 10:38:05.000000 wiremind-kubernetes-7.3.0/src/wiremind_kubernetes.egg-info/zip-safe
```

### Comparing `wiremind-kubernetes-7.2.0/LICENCE.md` & `wiremind-kubernetes-7.3.0/LICENCE.md`

 * *Files identical despite different names*

### Comparing `wiremind-kubernetes-7.2.0/PKG-INFO` & `wiremind-kubernetes-7.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wiremind-kubernetes
-Version: 7.2.0
+Version: 7.3.0
 Summary: Helper for Kubernetes.
 Home-page: https://github.com/wiremind/wiremind-kubernetes
 Author: Wiremind
 Author-email: dev@wiremind.io
 License: LGPLv3+
 Keywords: kubernetes
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `wiremind-kubernetes-7.2.0/README.md` & `wiremind-kubernetes-7.3.0/README.md`

 * *Files identical despite different names*

### Comparing `wiremind-kubernetes-7.2.0/setup.cfg` & `wiremind-kubernetes-7.3.0/setup.cfg`

 * *Files 27% similar despite different names*

```diff
@@ -16,14 +16,25 @@
 warn_redundant_casts = True
 warn_unused_ignores = True
 warn_unused_configs = True
 no_implicit_optional = True
 show_error_codes = True
 files = src
 
+[isort]
+src_paths = src,tests
+profile = black
+line_length = 120
+sections = FUTURE,STDLIB,THIRDPARTY,FIRSTPARTY,LOCALFOLDER
+no_lines_before = LOCALFOLDER
+multi_line_output = 3
+include_trailing_comma = True
+use_parentheses = True
+force_grid_wrap = 0
+
 [tool:pytest]
 log_level = INFO
 env = 
 	PYTHONHASHSEED=0
 filterwarnings = 
 	ignore::pytest.PytestUnknownMarkWarning
```

### Comparing `wiremind-kubernetes-7.2.0/setup.py` & `wiremind-kubernetes-7.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 wiremind-kubernetes
 """
-from setuptools import setup, find_packages
+from setuptools import find_packages, setup
 
 with open("VERSION") as version_file:
     version = version_file.read().strip()
 
 extra_require_test = [
     "mock",
     "pytest",
@@ -14,14 +14,16 @@
 extra_require_mypy = [
     "mypy",
 ]
 extra_require_dev = (
     [
         "flake8",
         "black",
+        "isort",
+        "bandit",
         "flake8-mutable",
         "pip-tools>=3.7.0",
         "pyupgrade",
         "safety",
     ]
     + extra_require_mypy
     + extra_require_test
```

### Comparing `wiremind-kubernetes-7.2.0/src/wiremind_kubernetes/exceptions.py` & `wiremind-kubernetes-7.3.0/src/wiremind_kubernetes/exceptions.py`

 * *Files identical despite different names*

### Comparing `wiremind-kubernetes-7.2.0/src/wiremind_kubernetes/kube_config.py` & `wiremind-kubernetes-7.3.0/src/wiremind_kubernetes/kube_config.py`

 * *Files identical despite different names*

### Comparing `wiremind-kubernetes-7.2.0/src/wiremind_kubernetes/kubernetes_client_additional_arguments.py` & `wiremind-kubernetes-7.3.0/src/wiremind_kubernetes/kubernetes_client_additional_arguments.py`

 * *Files identical despite different names*

### Comparing `wiremind-kubernetes-7.2.0/src/wiremind_kubernetes/kubernetes_helper.py` & `wiremind-kubernetes-7.3.0/src/wiremind_kubernetes/kubernetes_helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,21 +2,24 @@
 import pprint
 import time
 from typing import Any, Dict, Generator, List, Optional, Union
 
 import kubernetes
 
 from wiremind_kubernetes.exceptions import PodNotFound
-
 from .kube_config import load_kubernetes_config
 from .kubernetes_client_additional_arguments import (
-    AppV1ApiWithArguments, AutoscalingV1ApiWithArguments,
-    BatchV1ApiWithArguments, CoreV1ApiWithArguments,
-    CustomObjectsApiWithArguments, NetworkingV1ApiWithArguments,
-    RbacAuthorizationV1ApiWithArguments)
+    AppV1ApiWithArguments,
+    AutoscalingV1ApiWithArguments,
+    BatchV1ApiWithArguments,
+    CoreV1ApiWithArguments,
+    CustomObjectsApiWithArguments,
+    NetworkingV1ApiWithArguments,
+    RbacAuthorizationV1ApiWithArguments,
+)
 from .utils import retry_kubernetes_request, retry_kubernetes_request_no_ignore
 
 logger = logging.getLogger(__name__)
 
 HPA_ID_PREFIX = "wm--disabled--kube"
 
 
@@ -318,15 +321,15 @@
         # So we manually test for existence
         scaled: bool = False
         for priority_dict in expected_deployment_scale_dict.values():
             name: str
             expected_scale: int
             if len(priority_dict):
                 scaled = True
-                for (name, expected_scale) in priority_dict.items():
+                for name, expected_scale in priority_dict.items():
                     self.re_enable_hpa(deployment_name=name)
                     self.scale_up_deployment(name, expected_scale)
         if scaled:
             logger.info("Done scaling up application Deployments")
         else:
             logger.info("No Deployments to scale up")
```

### Comparing `wiremind-kubernetes-7.2.0/src/wiremind_kubernetes/tests/e2e_tests/conftest.py` & `wiremind-kubernetes-7.3.0/src/wiremind_kubernetes/tests/e2e_tests/conftest.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from typing import Generator
 
 import kubernetes
 import pytest
 from pytest_mock import MockerFixture
 
 import wiremind_kubernetes
-from wiremind_kubernetes.tests.e2e_tests.helpers import check_not_using_wiremind_cluster
+from wiremind_kubernetes.tests.e2e_tests.helpers import check_using_test_cluster
 from wiremind_kubernetes.utils import run_command
 
 E2E_CLUSTER_MANIFESTS = "tests/e2e_tests/manifests"
 absolute_path = os.path.dirname(os.path.join(os.path.abspath(wiremind_kubernetes.__file__)))
 TEST_NAMESPACE = "wiremind-kube-e2e-test"
 
 
@@ -23,15 +23,15 @@
 @pytest.fixture(scope="function")
 def k8s_client_request_function(mocker: MockerFixture) -> Generator:
     yield mocker.spy(kubernetes.client.api_client.ApiClient, "request")
 
 
 @pytest.fixture(scope="session", autouse=True)
 def setUpE2E() -> None:
-    check_not_using_wiremind_cluster()
+    check_using_test_cluster()
 
 
 def delete_namespace() -> None:
     run_command(
         f"kubectl delete namespace {TEST_NAMESPACE} --wait --grace-period=1",
     )
```

### Comparing `wiremind-kubernetes-7.2.0/src/wiremind_kubernetes/tests/e2e_tests/create_job_test.py` & `wiremind-kubernetes-7.3.0/src/wiremind_kubernetes/tests/e2e_tests/create_job_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import pprint
 import time
 
 import kubernetes
 from pytest_mock import MockerFixture
 
 from wiremind_kubernetes import KubernetesDeploymentManager
-
 from .conftest import TEST_NAMESPACE
 
 logger = logging.getLogger(__name__)
 
 
 def test_create_job(concerned_dm: KubernetesDeploymentManager, create_namespace: MockerFixture) -> None:
     """
```

### Comparing `wiremind-kubernetes-7.2.0/src/wiremind_kubernetes/tests/e2e_tests/helpers.py` & `wiremind-kubernetes-7.3.0/src/wiremind_kubernetes/tests/e2e_tests/helpers.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,55 +1,92 @@
 import json
 import logging
 import subprocess
 import sys
 import urllib
-from typing import Any, Dict
+from typing import Any, Dict, List
+
+import kubernetes
 
 from wiremind_kubernetes import run_command
 
 logger = logging.getLogger(__name__)
 
+DEFAULT_TEST_IPS_WHITELISTED = [
+    "localhost",  # minikube
+    "127.0.0.1",  # kind
+    "kubernetes.docker.internal",  # Docker for Mac
+]
+
+DEFAULT_TEST_NODES_WHITELISTED = ["minikube", "kind-control-plane", "kind", "kind-worker"]
 
-def check_not_using_wiremind_cluster() -> None:
+
+def get_default_kube_context() -> str:
     """
-    Will sys.exit(1) if kubectl current context api server is not a test cluster (like kind, minikube, etc)
+    Retrieves the default kube context
     """
-    logger.info("[CLUSTER-CONFIG]: Making sure the tests are not running against the main cluster...")
+    try:
+        return kubernetes.config.list_kube_config_contexts()[1]["name"]
+    except kubernetes.config.config_exception.ConfigException:
+        # Inside a Container maybe. This will make it use the incluster config.
+        return ""
 
+
+def is_ip_whitelisted(*, ips_whitelisted: List[str]) -> bool:
     api_server = subprocess.check_output(
         "kubectl config view --minify | grep server | cut -f 2- -d ':' | tr -d ' '",
         shell=True,
-        universal_newlines=True,
+        text=True,
     )
-    whitelisted_api_server_hostname_list = [
-        "localhost",  # minikube
-        "127.0.0.1",  # kind
-        "kubernetes.docker.internal",  # Docker for Mac
-    ]
+
     hostname = urllib.parse.urlparse(api_server.lower().strip()).hostname
-    if hostname not in whitelisted_api_server_hostname_list:
-        logger.error("Attempted to run tests with non-test cluster %s, abort!", api_server)
+    return hostname in ips_whitelisted
+
+
+def is_node_whitelisted(*, nodes_whitelisted: List[str]) -> bool:
+    output, *_ = run_command("kubectl get nodes -o name", return_result=True)
+    cluster_nodes = [x for x in output.replace("node/", "").split("\n") if x != ""]
+    for node in cluster_nodes:
+        if node not in nodes_whitelisted:
+            return False
+    return True
+
+
+def check_using_test_cluster(
+    *,
+    ips_whitelisted: List[str] = DEFAULT_TEST_IPS_WHITELISTED,
+    nodes_whitelisted: List[str] = DEFAULT_TEST_NODES_WHITELISTED,
+) -> bool:
+    """
+    Will sys.exit(1) if kubectl current context api server is not a test cluster (like kind, minikube, etc)
+    """
+    logger.info("[CLUSTER-CONFIG]: Making sure the tests are running against a test cluster...")
+
+    kube_context = get_default_kube_context()
+
+    if not is_ip_whitelisted(ips_whitelisted=ips_whitelisted) and not is_node_whitelisted(
+        nodes_whitelisted=nodes_whitelisted
+    ):
+        logger.error(f"Attempted to run tests with non-test cluster <{kube_context}>, aborting!")
         sys.exit(1)
+    return True
 
 
 def get_k8s_username() -> str:
     """
     Return the Kind cluster's username.
     """
     command = """kubectl config view -o json | jq '. as $o
     | ."current-context" as $current_context_name
     | $o.contexts[] | select(.name == $current_context_name) as $context
     | $o.users[] | select(.name == $context.context.user) as $user
     | $user.name'"""
     # dex-k8s-authenticator sets the user to: user={{ .Username}}-{{.ClusterName }}`
     # https://github.com/mintel/dex-k8s-authenticator/blob/master/templates/linux-mac-common.html#L101
-    username = (
-        subprocess.check_output(command, shell=True, universal_newlines=True).replace('"', "").strip().split("-")[0]
-    )
+    username = subprocess.check_output(command, shell=True, text=True).replace('"', "").strip().split("-")[0]
     assert username
     return username
 
 
 def kubectl_get_json(*, resource: str, namespace: str, name: str) -> Dict[str, Any]:
     output, *_ = run_command(
         f"kubectl get {resource} {name} -n {namespace} --ignore-not-found -o json", return_result=True
```

### Comparing `wiremind-kubernetes-7.2.0/src/wiremind_kubernetes/tests/e2e_tests/start_stop_test.py` & `wiremind-kubernetes-7.3.0/src/wiremind_kubernetes/tests/e2e_tests/start_stop_test.py`

 * *Files identical despite different names*

### Comparing `wiremind-kubernetes-7.2.0/src/wiremind_kubernetes/tests/unit_tests/kube_config_test.py` & `wiremind-kubernetes-7.3.0/src/wiremind_kubernetes/tests/unit_tests/kube_config_test.py`

 * *Files identical despite different names*

### Comparing `wiremind-kubernetes-7.2.0/src/wiremind_kubernetes/tests/unit_tests/kubernetes_client_additional_arguments_test.py` & `wiremind-kubernetes-7.3.0/src/wiremind_kubernetes/tests/unit_tests/kubernetes_client_additional_arguments_test.py`

 * *Files identical despite different names*

### Comparing `wiremind-kubernetes-7.2.0/src/wiremind_kubernetes/tests/unit_tests/kubernetes_deployment_manager_test.py` & `wiremind-kubernetes-7.3.0/src/wiremind_kubernetes/tests/unit_tests/kubernetes_deployment_manager_test.py`

 * *Files identical despite different names*

### Comparing `wiremind-kubernetes-7.2.0/src/wiremind_kubernetes/tests/unit_tests/namespaced_kubernetes_helper_test.py` & `wiremind-kubernetes-7.3.0/src/wiremind_kubernetes/tests/unit_tests/namespaced_kubernetes_helper_test.py`

 * *Files identical despite different names*

### Comparing `wiremind-kubernetes-7.2.0/src/wiremind_kubernetes/tests/unit_tests/utils_test/retry_kubernetes_request_test.py` & `wiremind-kubernetes-7.3.0/src/wiremind_kubernetes/tests/unit_tests/utils_test/retry_kubernetes_request_test.py`

 * *Files identical despite different names*

### Comparing `wiremind-kubernetes-7.2.0/src/wiremind_kubernetes/tests/unit_tests/utils_test/run_command_test.py` & `wiremind-kubernetes-7.3.0/src/wiremind_kubernetes/tests/unit_tests/utils_test/run_command_test.py`

 * *Files identical despite different names*

### Comparing `wiremind-kubernetes-7.2.0/src/wiremind_kubernetes/utils.py` & `wiremind-kubernetes-7.3.0/src/wiremind_kubernetes/utils.py`

 * *Files identical despite different names*

### Comparing `wiremind-kubernetes-7.2.0/src/wiremind_kubernetes.egg-info/PKG-INFO` & `wiremind-kubernetes-7.3.0/src/wiremind_kubernetes.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wiremind-kubernetes
-Version: 7.2.0
+Version: 7.3.0
 Summary: Helper for Kubernetes.
 Home-page: https://github.com/wiremind/wiremind-kubernetes
 Author: Wiremind
 Author-email: dev@wiremind.io
 License: LGPLv3+
 Keywords: kubernetes
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `wiremind-kubernetes-7.2.0/src/wiremind_kubernetes.egg-info/SOURCES.txt` & `wiremind-kubernetes-7.3.0/src/wiremind_kubernetes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

