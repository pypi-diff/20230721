# Comparing `tmp/wiremind-kubernetes-7.3.0.tar.gz` & `tmp/wiremind-kubernetes-7.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wiremind-kubernetes-7.3.0.tar", last modified: Fri Jul 21 10:38:05 2023, max compression
+gzip compressed data, was "wiremind-kubernetes-7.4.0.tar", last modified: Fri Jul 21 15:11:24 2023, max compression
```

## Comparing `wiremind-kubernetes-7.3.0.tar` & `wiremind-kubernetes-7.4.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:38:05.882237 wiremind-kubernetes-7.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     7642 2023-07-21 10:37:54.000000 wiremind-kubernetes-7.3.0/LICENCE.md
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-21 10:37:54.000000 wiremind-kubernetes-7.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-21 10:38:05.882237 wiremind-kubernetes-7.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-07-21 10:37:54.000000 wiremind-kubernetes-7.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-21 10:37:54.000000 wiremind-kubernetes-7.3.0/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-21 10:37:54.000000 wiremind-kubernetes-7.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-07-21 10:38:05.882237 wiremind-kubernetes-7.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-07-21 10:37:54.000000 wiremind-kubernetes-7.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:38:05.874236 wiremind-kubernetes-7.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:38:05.878237 wiremind-kubernetes-7.3.0/src/wiremind_kubernetes/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-21 10:37:54.000000 wiremind-kubernetes-7.3.0/src/wiremind_kubernetes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-21 10:37:54.000000 wiremind-kubernetes-7.3.0/src/wiremind_kubernetes/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-07-21 10:37:54.000000 wiremind-kubernetes-7.3.0/src/wiremind_kubernetes/kube_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-07-21 10:37:54.000000 wiremind-kubernetes-7.3.0/src/wiremind_kubernetes/kubernetes_client_additional_arguments.py
--rw-r--r--   0 runner    (1001) docker     (123)    19836 2023-07-21 10:37:54.000000 wiremind-kubernetes-7.3.0/src/wiremind_kubernetes/kubernetes_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:38:05.878237 wiremind-kubernetes-7.3.0/src/wiremind_kubernetes/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 10:37:54.000000 wiremind-kubernetes-7.3.0/src/wiremind_kubernetes/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:38:05.878237 wiremind-kubernetes-7.3.0/src/wiremind_kubernetes/tests/e2e_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 10:37:54.000000 wiremind-kubernetes-7.3.0/src/wiremind_kubernetes/tests/e2e_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-07-21 10:37:54.000000 wiremind-kubernetes-7.3.0/src/wiremind_kubernetes/tests/e2e_tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-07-21 10:37:54.000000 wiremind-kubernetes-7.3.0/src/wiremind_kubernetes/tests/e2e_tests/create_job_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-07-21 10:37:54.000000 wiremind-kubernetes-7.3.0/src/wiremind_kubernetes/tests/e2e_tests/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-07-21 10:37:54.000000 wiremind-kubernetes-7.3.0/src/wiremind_kubernetes/tests/e2e_tests/start_stop_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:38:05.882237 wiremind-kubernetes-7.3.0/src/wiremind_kubernetes/tests/unit_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 10:37:54.000000 wiremind-kubernetes-7.3.0/src/wiremind_kubernetes/tests/unit_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-07-21 10:37:54.000000 wiremind-kubernetes-7.3.0/src/wiremind_kubernetes/tests/unit_tests/kube_config_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-07-21 10:37:54.000000 wiremind-kubernetes-7.3.0/src/wiremind_kubernetes/tests/unit_tests/kubernetes_client_additional_arguments_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-07-21 10:37:54.000000 wiremind-kubernetes-7.3.0/src/wiremind_kubernetes/tests/unit_tests/kubernetes_deployment_manager_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-07-21 10:37:54.000000 wiremind-kubernetes-7.3.0/src/wiremind_kubernetes/tests/unit_tests/namespaced_kubernetes_helper_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:38:05.882237 wiremind-kubernetes-7.3.0/src/wiremind_kubernetes/tests/unit_tests/utils_test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 10:37:54.000000 wiremind-kubernetes-7.3.0/src/wiremind_kubernetes/tests/unit_tests/utils_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-07-21 10:37:54.000000 wiremind-kubernetes-7.3.0/src/wiremind_kubernetes/tests/unit_tests/utils_test/retry_kubernetes_request_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4348 2023-07-21 10:37:54.000000 wiremind-kubernetes-7.3.0/src/wiremind_kubernetes/tests/unit_tests/utils_test/run_command_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3887 2023-07-21 10:37:54.000000 wiremind-kubernetes-7.3.0/src/wiremind_kubernetes/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:38:05.878237 wiremind-kubernetes-7.3.0/src/wiremind_kubernetes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-21 10:38:05.000000 wiremind-kubernetes-7.3.0/src/wiremind_kubernetes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-07-21 10:38:05.000000 wiremind-kubernetes-7.3.0/src/wiremind_kubernetes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 10:38:05.000000 wiremind-kubernetes-7.3.0/src/wiremind_kubernetes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-21 10:38:05.000000 wiremind-kubernetes-7.3.0/src/wiremind_kubernetes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-21 10:38:05.000000 wiremind-kubernetes-7.3.0/src/wiremind_kubernetes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 10:38:05.000000 wiremind-kubernetes-7.3.0/src/wiremind_kubernetes.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:11:24.399645 wiremind-kubernetes-7.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     7642 2023-07-21 15:11:14.000000 wiremind-kubernetes-7.4.0/LICENCE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-21 15:11:14.000000 wiremind-kubernetes-7.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-21 15:11:24.399645 wiremind-kubernetes-7.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-07-21 15:11:14.000000 wiremind-kubernetes-7.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-21 15:11:14.000000 wiremind-kubernetes-7.4.0/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-21 15:11:14.000000 wiremind-kubernetes-7.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-07-21 15:11:24.399645 wiremind-kubernetes-7.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-07-21 15:11:14.000000 wiremind-kubernetes-7.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:11:24.395645 wiremind-kubernetes-7.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:11:24.399645 wiremind-kubernetes-7.4.0/src/wiremind_kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-21 15:11:14.000000 wiremind-kubernetes-7.4.0/src/wiremind_kubernetes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-21 15:11:14.000000 wiremind-kubernetes-7.4.0/src/wiremind_kubernetes/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-07-21 15:11:14.000000 wiremind-kubernetes-7.4.0/src/wiremind_kubernetes/kube_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-07-21 15:11:14.000000 wiremind-kubernetes-7.4.0/src/wiremind_kubernetes/kubernetes_client_additional_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20016 2023-07-21 15:11:14.000000 wiremind-kubernetes-7.4.0/src/wiremind_kubernetes/kubernetes_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:11:24.399645 wiremind-kubernetes-7.4.0/src/wiremind_kubernetes/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 15:11:14.000000 wiremind-kubernetes-7.4.0/src/wiremind_kubernetes/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:11:24.399645 wiremind-kubernetes-7.4.0/src/wiremind_kubernetes/tests/e2e_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 15:11:14.000000 wiremind-kubernetes-7.4.0/src/wiremind_kubernetes/tests/e2e_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-07-21 15:11:14.000000 wiremind-kubernetes-7.4.0/src/wiremind_kubernetes/tests/e2e_tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-07-21 15:11:14.000000 wiremind-kubernetes-7.4.0/src/wiremind_kubernetes/tests/e2e_tests/create_job_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-07-21 15:11:14.000000 wiremind-kubernetes-7.4.0/src/wiremind_kubernetes/tests/e2e_tests/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-07-21 15:11:14.000000 wiremind-kubernetes-7.4.0/src/wiremind_kubernetes/tests/e2e_tests/start_stop_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:11:24.399645 wiremind-kubernetes-7.4.0/src/wiremind_kubernetes/tests/unit_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 15:11:14.000000 wiremind-kubernetes-7.4.0/src/wiremind_kubernetes/tests/unit_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-07-21 15:11:14.000000 wiremind-kubernetes-7.4.0/src/wiremind_kubernetes/tests/unit_tests/kube_config_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-07-21 15:11:14.000000 wiremind-kubernetes-7.4.0/src/wiremind_kubernetes/tests/unit_tests/kubernetes_client_additional_arguments_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-07-21 15:11:14.000000 wiremind-kubernetes-7.4.0/src/wiremind_kubernetes/tests/unit_tests/kubernetes_deployment_manager_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-07-21 15:11:14.000000 wiremind-kubernetes-7.4.0/src/wiremind_kubernetes/tests/unit_tests/namespaced_kubernetes_helper_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:11:24.399645 wiremind-kubernetes-7.4.0/src/wiremind_kubernetes/tests/unit_tests/utils_test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 15:11:14.000000 wiremind-kubernetes-7.4.0/src/wiremind_kubernetes/tests/unit_tests/utils_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-07-21 15:11:14.000000 wiremind-kubernetes-7.4.0/src/wiremind_kubernetes/tests/unit_tests/utils_test/retry_kubernetes_request_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4348 2023-07-21 15:11:14.000000 wiremind-kubernetes-7.4.0/src/wiremind_kubernetes/tests/unit_tests/utils_test/run_command_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3887 2023-07-21 15:11:14.000000 wiremind-kubernetes-7.4.0/src/wiremind_kubernetes/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:11:24.399645 wiremind-kubernetes-7.4.0/src/wiremind_kubernetes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-21 15:11:24.000000 wiremind-kubernetes-7.4.0/src/wiremind_kubernetes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-07-21 15:11:24.000000 wiremind-kubernetes-7.4.0/src/wiremind_kubernetes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 15:11:24.000000 wiremind-kubernetes-7.4.0/src/wiremind_kubernetes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-21 15:11:24.000000 wiremind-kubernetes-7.4.0/src/wiremind_kubernetes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-21 15:11:24.000000 wiremind-kubernetes-7.4.0/src/wiremind_kubernetes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 15:11:24.000000 wiremind-kubernetes-7.4.0/src/wiremind_kubernetes.egg-info/zip-safe
```

### Comparing `wiremind-kubernetes-7.3.0/LICENCE.md` & `wiremind-kubernetes-7.4.0/LICENCE.md`

 * *Files identical despite different names*

### Comparing `wiremind-kubernetes-7.3.0/PKG-INFO` & `wiremind-kubernetes-7.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wiremind-kubernetes
-Version: 7.3.0
+Version: 7.4.0
 Summary: Helper for Kubernetes.
 Home-page: https://github.com/wiremind/wiremind-kubernetes
 Author: Wiremind
 Author-email: dev@wiremind.io
 License: LGPLv3+
 Keywords: kubernetes
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `wiremind-kubernetes-7.3.0/README.md` & `wiremind-kubernetes-7.4.0/README.md`

 * *Files identical despite different names*

### Comparing `wiremind-kubernetes-7.3.0/setup.cfg` & `wiremind-kubernetes-7.4.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `wiremind-kubernetes-7.3.0/setup.py` & `wiremind-kubernetes-7.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `wiremind-kubernetes-7.3.0/src/wiremind_kubernetes/exceptions.py` & `wiremind-kubernetes-7.4.0/src/wiremind_kubernetes/exceptions.py`

 * *Files identical despite different names*

### Comparing `wiremind-kubernetes-7.3.0/src/wiremind_kubernetes/kube_config.py` & `wiremind-kubernetes-7.4.0/src/wiremind_kubernetes/kube_config.py`

 * *Files identical despite different names*

### Comparing `wiremind-kubernetes-7.3.0/src/wiremind_kubernetes/kubernetes_client_additional_arguments.py` & `wiremind-kubernetes-7.4.0/src/wiremind_kubernetes/kubernetes_client_additional_arguments.py`

 * *Files 8% similar despite different names*

```diff
@@ -74,7 +74,12 @@
     def __init__(self, *args: Any, dry_run: bool = False, pretty: bool = False, **kwargs: Any) -> None:
         super().__init__(client=kubernetes.client.RbacAuthorizationV1Api, dry_run=dry_run, pretty=pretty)
 
 
 class NetworkingV1ApiWithArguments(ClientWithArguments):
     def __init__(self, *args: Any, dry_run: bool = False, pretty: bool = False, **kwargs: Any) -> None:
         super().__init__(client=kubernetes.client.NetworkingV1Api, dry_run=dry_run, pretty=pretty)
+
+
+class StorageV1ApiWithArguments(ClientWithArguments):
+    def __init__(self, *args: Any, dry_run: bool = False, pretty: bool = False, **kwargs: Any) -> None:
+        super().__init__(client=kubernetes.client.StorageV1Api, dry_run=dry_run, pretty=pretty)
```

### Comparing `wiremind-kubernetes-7.3.0/src/wiremind_kubernetes/kubernetes_helper.py` & `wiremind-kubernetes-7.4.0/src/wiremind_kubernetes/kubernetes_helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     AppV1ApiWithArguments,
     AutoscalingV1ApiWithArguments,
     BatchV1ApiWithArguments,
     CoreV1ApiWithArguments,
     CustomObjectsApiWithArguments,
     NetworkingV1ApiWithArguments,
     RbacAuthorizationV1ApiWithArguments,
+    StorageV1ApiWithArguments,
 )
 from .utils import retry_kubernetes_request, retry_kubernetes_request_no_ignore
 
 logger = logging.getLogger(__name__)
 
 HPA_ID_PREFIX = "wm--disabled--kube"
 
@@ -62,14 +63,17 @@
         )
         self.client_rbac_authorization_v1_api: kubernetes.client.RbacAuthorizationV1Api = (
             RbacAuthorizationV1ApiWithArguments(dry_run=dry_run, pretty=pretty)
         )
         self.client_networking_v1_api: kubernetes.client.NetworkingV1Api = NetworkingV1ApiWithArguments(
             dry_run=dry_run, pretty=pretty
         )
+        self.client_storage_v1_api: kubernetes.client.StorageV1Api = StorageV1ApiWithArguments(
+            dry_run=dry_run, pretty=pretty
+        )
 
         self.dry_run: bool = dry_run
         self.pretty: bool = pretty
 
 
 def _get_namespace_from_kube() -> str:
     return open("/var/run/secrets/kubernetes.io/serviceaccount/namespace").read()
```

### Comparing `wiremind-kubernetes-7.3.0/src/wiremind_kubernetes/tests/e2e_tests/conftest.py` & `wiremind-kubernetes-7.4.0/src/wiremind_kubernetes/tests/e2e_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `wiremind-kubernetes-7.3.0/src/wiremind_kubernetes/tests/e2e_tests/create_job_test.py` & `wiremind-kubernetes-7.4.0/src/wiremind_kubernetes/tests/e2e_tests/create_job_test.py`

 * *Files identical despite different names*

### Comparing `wiremind-kubernetes-7.3.0/src/wiremind_kubernetes/tests/e2e_tests/helpers.py` & `wiremind-kubernetes-7.4.0/src/wiremind_kubernetes/tests/e2e_tests/helpers.py`

 * *Files identical despite different names*

### Comparing `wiremind-kubernetes-7.3.0/src/wiremind_kubernetes/tests/e2e_tests/start_stop_test.py` & `wiremind-kubernetes-7.4.0/src/wiremind_kubernetes/tests/e2e_tests/start_stop_test.py`

 * *Files identical despite different names*

### Comparing `wiremind-kubernetes-7.3.0/src/wiremind_kubernetes/tests/unit_tests/kube_config_test.py` & `wiremind-kubernetes-7.4.0/src/wiremind_kubernetes/tests/unit_tests/kube_config_test.py`

 * *Files identical despite different names*

### Comparing `wiremind-kubernetes-7.3.0/src/wiremind_kubernetes/tests/unit_tests/kubernetes_client_additional_arguments_test.py` & `wiremind-kubernetes-7.4.0/src/wiremind_kubernetes/tests/unit_tests/kubernetes_client_additional_arguments_test.py`

 * *Files identical despite different names*

### Comparing `wiremind-kubernetes-7.3.0/src/wiremind_kubernetes/tests/unit_tests/kubernetes_deployment_manager_test.py` & `wiremind-kubernetes-7.4.0/src/wiremind_kubernetes/tests/unit_tests/kubernetes_deployment_manager_test.py`

 * *Files identical despite different names*

### Comparing `wiremind-kubernetes-7.3.0/src/wiremind_kubernetes/tests/unit_tests/namespaced_kubernetes_helper_test.py` & `wiremind-kubernetes-7.4.0/src/wiremind_kubernetes/tests/unit_tests/namespaced_kubernetes_helper_test.py`

 * *Files identical despite different names*

### Comparing `wiremind-kubernetes-7.3.0/src/wiremind_kubernetes/tests/unit_tests/utils_test/retry_kubernetes_request_test.py` & `wiremind-kubernetes-7.4.0/src/wiremind_kubernetes/tests/unit_tests/utils_test/retry_kubernetes_request_test.py`

 * *Files identical despite different names*

### Comparing `wiremind-kubernetes-7.3.0/src/wiremind_kubernetes/tests/unit_tests/utils_test/run_command_test.py` & `wiremind-kubernetes-7.4.0/src/wiremind_kubernetes/tests/unit_tests/utils_test/run_command_test.py`

 * *Files identical despite different names*

### Comparing `wiremind-kubernetes-7.3.0/src/wiremind_kubernetes/utils.py` & `wiremind-kubernetes-7.4.0/src/wiremind_kubernetes/utils.py`

 * *Files identical despite different names*

### Comparing `wiremind-kubernetes-7.3.0/src/wiremind_kubernetes.egg-info/PKG-INFO` & `wiremind-kubernetes-7.4.0/src/wiremind_kubernetes.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wiremind-kubernetes
-Version: 7.3.0
+Version: 7.4.0
 Summary: Helper for Kubernetes.
 Home-page: https://github.com/wiremind/wiremind-kubernetes
 Author: Wiremind
 Author-email: dev@wiremind.io
 License: LGPLv3+
 Keywords: kubernetes
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `wiremind-kubernetes-7.3.0/src/wiremind_kubernetes.egg-info/SOURCES.txt` & `wiremind-kubernetes-7.4.0/src/wiremind_kubernetes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

