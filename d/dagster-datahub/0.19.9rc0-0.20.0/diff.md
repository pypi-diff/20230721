# Comparing `tmp/dagster-datahub-0.19.9rc0.tar.gz` & `tmp/dagster-datahub-0.20.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-datahub-0.19.9rc0.tar", last modified: Thu Jun  8 18:30:25 2023, max compression
+gzip compressed data, was "dagster-datahub-0.20.0.tar", last modified: Thu Jul 20 22:01:03 2023, max compression
```

## Comparing `dagster-datahub-0.19.9rc0.tar` & `dagster-datahub-0.20.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:30:25.800431 dagster-datahub-0.19.9rc0/
--rw-r--r--   0 root         (0) root         (0)    11344 2023-06-08 18:20:46.000000 dagster-datahub-0.19.9rc0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      214 2023-06-08 18:20:46.000000 dagster-datahub-0.19.9rc0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      706 2023-06-08 18:30:25.800431 dagster-datahub-0.19.9rc0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      131 2023-06-08 18:20:46.000000 dagster-datahub-0.19.9rc0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:30:25.800431 dagster-datahub-0.19.9rc0/dagster_datahub/
--rw-r--r--   0 root         (0) root         (0)      492 2023-06-08 18:20:46.000000 dagster-datahub-0.19.9rc0/dagster_datahub/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 18:20:46.000000 dagster-datahub-0.19.9rc0/dagster_datahub/py.typed
--rw-r--r--   0 root         (0) root         (0)     3932 2023-06-08 18:20:46.000000 dagster-datahub-0.19.9rc0/dagster_datahub/resources.py
--rw-r--r--   0 root         (0) root         (0)       26 2023-06-08 18:20:46.000000 dagster-datahub-0.19.9rc0/dagster_datahub/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:30:25.800431 dagster-datahub-0.19.9rc0/dagster_datahub.egg-info/
--rw-r--r--   0 root         (0) root         (0)      706 2023-06-08 18:30:25.000000 dagster-datahub-0.19.9rc0/dagster_datahub.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      389 2023-06-08 18:30:25.000000 dagster-datahub-0.19.9rc0/dagster_datahub.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 18:30:25.000000 dagster-datahub-0.19.9rc0/dagster_datahub.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 18:30:25.000000 dagster-datahub-0.19.9rc0/dagster_datahub.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       87 2023-06-08 18:30:25.000000 dagster-datahub-0.19.9rc0/dagster_datahub.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-06-08 18:30:25.000000 dagster-datahub-0.19.9rc0/dagster_datahub.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      162 2023-06-08 18:30:25.800431 dagster-datahub-0.19.9rc0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1476 2023-06-08 18:20:46.000000 dagster-datahub-0.19.9rc0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:01:03.197237 dagster-datahub-0.20.0/
+-rw-r--r--   0 root         (0) root         (0)    11344 2023-07-20 21:53:16.000000 dagster-datahub-0.20.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      214 2023-07-20 21:53:16.000000 dagster-datahub-0.20.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      653 2023-07-20 22:01:03.197237 dagster-datahub-0.20.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      131 2023-07-20 21:53:16.000000 dagster-datahub-0.20.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:01:03.197237 dagster-datahub-0.20.0/dagster_datahub/
+-rw-r--r--   0 root         (0) root         (0)      492 2023-07-20 21:53:16.000000 dagster-datahub-0.20.0/dagster_datahub/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-20 21:53:16.000000 dagster-datahub-0.20.0/dagster_datahub/py.typed
+-rw-r--r--   0 root         (0) root         (0)     4242 2023-07-20 21:53:16.000000 dagster-datahub-0.20.0/dagster_datahub/resources.py
+-rw-r--r--   0 root         (0) root         (0)       23 2023-07-20 21:53:16.000000 dagster-datahub-0.20.0/dagster_datahub/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:01:03.197237 dagster-datahub-0.20.0/dagster_datahub.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      653 2023-07-20 22:01:03.000000 dagster-datahub-0.20.0/dagster_datahub.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      389 2023-07-20 22:01:03.000000 dagster-datahub-0.20.0/dagster_datahub.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 22:01:03.000000 dagster-datahub-0.20.0/dagster_datahub.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 22:01:03.000000 dagster-datahub-0.20.0/dagster_datahub.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       84 2023-07-20 22:01:03.000000 dagster-datahub-0.20.0/dagster_datahub.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-07-20 22:01:03.000000 dagster-datahub-0.20.0/dagster_datahub.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      162 2023-07-20 22:01:03.197237 dagster-datahub-0.20.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1424 2023-07-20 21:53:16.000000 dagster-datahub-0.20.0/setup.py
```

### Comparing `dagster-datahub-0.19.9rc0/LICENSE` & `dagster-datahub-0.20.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-datahub-0.19.9rc0/PKG-INFO` & `dagster-datahub-0.20.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: dagster-datahub
-Version: 0.19.9rc0
+Version: 0.20.0
 Summary: Package for Datahub-specific Dagster framework solid and resource components.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-datahub
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

### Comparing `dagster-datahub-0.19.9rc0/dagster_datahub/resources.py` & `dagster-datahub-0.20.0/dagster_datahub/resources.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import Any, Dict, List, Optional
 
 from dagster import InitResourceContext, resource
 from dagster._config.pythonic_config import Config, ConfigurableResource
+from dagster._core.definitions.resource_definition import dagster_maintained_resource
 from datahub.emitter.kafka_emitter import (
     DEFAULT_MCE_KAFKA_TOPIC,
     DEFAULT_MCP_KAFKA_TOPIC,
     MCE_KEY,
     MCP_KEY,
     DatahubKafkaEmitter,
     KafkaEmitterConfig,
@@ -23,14 +24,18 @@
     retry_methods: Optional[List[str]] = None
     retry_max_times: Optional[int] = None
     extra_headers: Optional[Dict[str, str]] = None
     ca_certificate_path: Optional[str] = None
     server_telemetry_id: Optional[str] = None
     disable_ssl_verification: bool = False
 
+    @classmethod
+    def _is_dagster_maintained(cls) -> bool:
+        return True
+
     def get_emitter(self) -> DatahubRestEmitter:
         return DatahubRestEmitter(
             gms_server=self.connection,
             token=self.token,
             connect_timeout_sec=self.connect_timeout_sec,
             read_timeout_sec=self.read_timeout_sec,
             retry_status_codes=self.retry_status_codes,
@@ -39,14 +44,15 @@
             extra_headers=self.extra_headers,
             ca_certificate_path=self.ca_certificate_path,
             server_telemetry_id=self.server_telemetry_id,
             disable_ssl_verification=self.disable_ssl_verification,
         )
 
 
+@dagster_maintained_resource
 @resource(config_schema=DatahubRESTEmitterResource.to_config_schema())
 def datahub_rest_emitter(init_context: InitResourceContext) -> DatahubRestEmitter:
     emitter = DatahubRestEmitter(
         gms_server=init_context.resource_config.get("connection"),
         token=init_context.resource_config.get("token"),
         connect_timeout_sec=init_context.resource_config.get("connect_timeout_sec"),
         read_timeout_sec=init_context.resource_config.get("read_timeout_sec"),
@@ -77,16 +83,21 @@
     topic_routes: Dict[str, str] = Field(
         default={
             MCE_KEY: DEFAULT_MCE_KAFKA_TOPIC,
             MCP_KEY: DEFAULT_MCP_KAFKA_TOPIC,
         }
     )
 
+    @classmethod
+    def _is_dagster_maintained(cls) -> bool:
+        return True
+
     def get_emitter(self) -> DatahubKafkaEmitter:
         return DatahubKafkaEmitter(
             KafkaEmitterConfig.parse_obj(self._convert_to_config_dictionary())
         )
 
 
+@dagster_maintained_resource
 @resource(config_schema=DatahubKafkaEmitterResource.to_config_schema())
 def datahub_kafka_emitter(init_context: InitResourceContext) -> DatahubKafkaEmitter:
     return DatahubKafkaEmitter(KafkaEmitterConfig.parse_obj(init_context.resource_config))
```

### Comparing `dagster-datahub-0.19.9rc0/dagster_datahub.egg-info/PKG-INFO` & `dagster-datahub-0.20.0/dagster_datahub.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: dagster-datahub
-Version: 0.19.9rc0
+Version: 0.20.0
 Summary: Package for Datahub-specific Dagster framework solid and resource components.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-datahub
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

### Comparing `dagster-datahub-0.19.9rc0/setup.py` & `dagster-datahub-0.20.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,26 +22,25 @@
     author_email="hello@elementl.com",
     license="Apache-2.0",
     description="Package for Datahub-specific Dagster framework solid and resource components.",
     url=(
         "https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-datahub"
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
     packages=find_packages(exclude=["dagster_datahub_tests*"]),
     include_package_data=True,
     install_requires=[
         "acryl-datahub[datahub-rest, datahub-kafka]<=0.10.2",
-        "dagster==1.3.9rc0",
+        "dagster==1.4.0",
         "packaging",
         "requests",
     ],
     extras_require={},
     zip_safe=False,
 )
```

