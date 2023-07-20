# Comparing `tmp/dagster-msteams-0.19.9rc0.tar.gz` & `tmp/dagster-msteams-0.20.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-msteams-0.19.9rc0.tar", last modified: Thu Jun  8 18:28:39 2023, max compression
+gzip compressed data, was "dagster-msteams-0.20.0.tar", last modified: Thu Jul 20 22:03:37 2023, max compression
```

## Comparing `dagster-msteams-0.19.9rc0.tar` & `dagster-msteams-0.20.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:28:39.862958 dagster-msteams-0.19.9rc0/
--rw-r--r--   0 root         (0) root         (0)    11343 2023-06-08 18:20:46.000000 dagster-msteams-0.19.9rc0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       66 2023-06-08 18:20:46.000000 dagster-msteams-0.19.9rc0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      693 2023-06-08 18:28:39.862958 dagster-msteams-0.19.9rc0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      131 2023-06-08 18:20:46.000000 dagster-msteams-0.19.9rc0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:28:39.862958 dagster-msteams-0.19.9rc0/dagster_msteams/
--rw-r--r--   0 root         (0) root         (0)      510 2023-06-08 18:20:46.000000 dagster-msteams-0.19.9rc0/dagster_msteams/__init__.py
--rw-r--r--   0 root         (0) root         (0)      849 2023-06-08 18:20:46.000000 dagster-msteams-0.19.9rc0/dagster_msteams/card.py
--rw-r--r--   0 root         (0) root         (0)     1389 2023-06-08 18:20:46.000000 dagster-msteams-0.19.9rc0/dagster_msteams/client.py
--rw-r--r--   0 root         (0) root         (0)     3881 2023-06-08 18:20:46.000000 dagster-msteams-0.19.9rc0/dagster_msteams/hooks.py
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-08 18:20:46.000000 dagster-msteams-0.19.9rc0/dagster_msteams/py.typed
--rw-r--r--   0 root         (0) root         (0)     3553 2023-06-08 18:20:46.000000 dagster-msteams-0.19.9rc0/dagster_msteams/resources.py
--rw-r--r--   0 root         (0) root         (0)     5213 2023-06-08 18:20:46.000000 dagster-msteams-0.19.9rc0/dagster_msteams/sensors.py
--rw-r--r--   0 root         (0) root         (0)       26 2023-06-08 18:20:46.000000 dagster-msteams-0.19.9rc0/dagster_msteams/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:28:39.862958 dagster-msteams-0.19.9rc0/dagster_msteams.egg-info/
--rw-r--r--   0 root         (0) root         (0)      693 2023-06-08 18:28:39.000000 dagster-msteams-0.19.9rc0/dagster_msteams.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      491 2023-06-08 18:28:39.000000 dagster-msteams-0.19.9rc0/dagster_msteams.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 18:28:39.000000 dagster-msteams-0.19.9rc0/dagster_msteams.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 18:28:39.000000 dagster-msteams-0.19.9rc0/dagster_msteams.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       23 2023-06-08 18:28:39.000000 dagster-msteams-0.19.9rc0/dagster_msteams.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-06-08 18:28:39.000000 dagster-msteams-0.19.9rc0/dagster_msteams.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      162 2023-06-08 18:28:39.862958 dagster-msteams-0.19.9rc0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1163 2023-06-08 18:20:46.000000 dagster-msteams-0.19.9rc0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:03:37.847404 dagster-msteams-0.20.0/
+-rw-r--r--   0 root         (0) root         (0)    11343 2023-07-20 21:53:16.000000 dagster-msteams-0.20.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       66 2023-07-20 21:53:16.000000 dagster-msteams-0.20.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      640 2023-07-20 22:03:37.847404 dagster-msteams-0.20.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      131 2023-07-20 21:53:16.000000 dagster-msteams-0.20.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:03:37.847404 dagster-msteams-0.20.0/dagster_msteams/
+-rw-r--r--   0 root         (0) root         (0)      510 2023-07-20 21:53:16.000000 dagster-msteams-0.20.0/dagster_msteams/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      849 2023-07-20 21:53:16.000000 dagster-msteams-0.20.0/dagster_msteams/card.py
+-rw-r--r--   0 root         (0) root         (0)     1389 2023-07-20 21:53:16.000000 dagster-msteams-0.20.0/dagster_msteams/client.py
+-rw-r--r--   0 root         (0) root         (0)     3881 2023-07-20 21:53:16.000000 dagster-msteams-0.20.0/dagster_msteams/hooks.py
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-20 21:53:16.000000 dagster-msteams-0.20.0/dagster_msteams/py.typed
+-rw-r--r--   0 root         (0) root         (0)     3751 2023-07-20 21:53:16.000000 dagster-msteams-0.20.0/dagster_msteams/resources.py
+-rw-r--r--   0 root         (0) root         (0)     5213 2023-07-20 21:53:16.000000 dagster-msteams-0.20.0/dagster_msteams/sensors.py
+-rw-r--r--   0 root         (0) root         (0)       23 2023-07-20 21:53:16.000000 dagster-msteams-0.20.0/dagster_msteams/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:03:37.847404 dagster-msteams-0.20.0/dagster_msteams.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      640 2023-07-20 22:03:37.000000 dagster-msteams-0.20.0/dagster_msteams.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      491 2023-07-20 22:03:37.000000 dagster-msteams-0.20.0/dagster_msteams.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 22:03:37.000000 dagster-msteams-0.20.0/dagster_msteams.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 22:03:37.000000 dagster-msteams-0.20.0/dagster_msteams.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       30 2023-07-20 22:03:37.000000 dagster-msteams-0.20.0/dagster_msteams.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-07-20 22:03:37.000000 dagster-msteams-0.20.0/dagster_msteams.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      162 2023-07-20 22:03:37.847404 dagster-msteams-0.20.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1243 2023-07-20 21:53:16.000000 dagster-msteams-0.20.0/setup.py
```

### Comparing `dagster-msteams-0.19.9rc0/LICENSE` & `dagster-msteams-0.20.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-msteams-0.19.9rc0/PKG-INFO` & `dagster-msteams-0.20.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: dagster-msteams
-Version: 0.19.9rc0
+Version: 0.20.0
 Summary: A Microsoft Teams client resource for posting to Microsoft Teams
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-msteams
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 License-File: LICENSE
```

### Comparing `dagster-msteams-0.19.9rc0/dagster_msteams/card.py` & `dagster-msteams-0.20.0/dagster_msteams/card.py`

 * *Files identical despite different names*

### Comparing `dagster-msteams-0.19.9rc0/dagster_msteams/client.py` & `dagster-msteams-0.20.0/dagster_msteams/client.py`

 * *Files identical despite different names*

### Comparing `dagster-msteams-0.19.9rc0/dagster_msteams/hooks.py` & `dagster-msteams-0.20.0/dagster_msteams/hooks.py`

 * *Files identical despite different names*

### Comparing `dagster-msteams-0.19.9rc0/dagster_msteams/resources.py` & `dagster-msteams-0.20.0/dagster_msteams/resources.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from dagster import ConfigurableResource, resource
+from dagster._core.definitions.resource_definition import dagster_maintained_resource
 from pydantic import Field
 
 from dagster_msteams.client import TeamsClient
 
 
 class MSTeamsResource(ConfigurableResource):
     """This resource is for connecting to Microsoft Teams.
@@ -56,24 +57,29 @@
     http_proxy: str = Field(default=None, description="HTTP proxy URL")
     https_proxy: str = Field(default=None, description="HTTPS proxy URL")
     timeout: float = Field(default=60, description="Timeout for requests to MS Teams")
     verify: bool = Field(
         default=True, description="Whether to verify SSL certificates, defaults to True"
     )
 
+    @classmethod
+    def _is_dagster_maintained(cls) -> bool:
+        return True
+
     def get_client(self) -> TeamsClient:
         return TeamsClient(
             hook_url=self.hook_url,
             http_proxy=self.http_proxy,
             https_proxy=self.https_proxy,
             timeout=self.timeout,
             verify=self.verify,
         )
 
 
+@dagster_maintained_resource
 @resource(
     config_schema=MSTeamsResource.to_config_schema(),
     description="This resource is for connecting to MS Teams",
 )
 def msteams_resource(context) -> TeamsClient:
     """This resource is for connecting to Microsoft Teams.
```

### Comparing `dagster-msteams-0.19.9rc0/dagster_msteams/sensors.py` & `dagster-msteams-0.20.0/dagster_msteams/sensors.py`

 * *Files identical despite different names*

### Comparing `dagster-msteams-0.19.9rc0/dagster_msteams.egg-info/PKG-INFO` & `dagster-msteams-0.20.0/dagster_msteams.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: dagster-msteams
-Version: 0.19.9rc0
+Version: 0.20.0
 Summary: A Microsoft Teams client resource for posting to Microsoft Teams
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-msteams
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 License-File: LICENSE
```

### Comparing `dagster-msteams-0.19.9rc0/setup.py` & `dagster-msteams-0.20.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,33 +7,35 @@
     version = {}
     with open(Path(__file__).parent / "dagster_msteams/version.py", encoding="utf8") as fp:
         exec(fp.read(), version)
 
     return version["__version__"]
 
 
+ver = get_version()
+# dont pin dev installs to avoid pip dep resolver issues
+pin = "" if ver == "1!0+dev" else f"=={ver}"
 setup(
     name="dagster-msteams",
     version=get_version(),
     author="Elementl",
     author_email="hello@elementl.com",
     license="Apache-2.0",
     description="A Microsoft Teams client resource for posting to Microsoft Teams",
     url=(
         "https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-msteams"
     ),
     classifiers=[
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_msteams_tests*"]),
     install_requires=[
-        "dagster",
+        "dagster==1.4.0",
         "requests>=2,<3",
     ],
     zip_safe=False,
 )
```

