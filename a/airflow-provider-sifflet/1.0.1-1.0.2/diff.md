# Comparing `tmp/airflow-provider-sifflet-1.0.1.tar.gz` & `tmp/airflow-provider-sifflet-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airflow-provider-sifflet-1.0.1.tar", last modified: Thu Jun 16 06:44:34 2022, max compression
+gzip compressed data, was "airflow-provider-sifflet-1.0.2.tar", last modified: Fri Jul 21 09:37:08 2023, max compression
```

## Comparing `airflow-provider-sifflet-1.0.1.tar` & `airflow-provider-sifflet-1.0.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 baptiste   (501) staff       (20)        0 2022-06-16 06:44:34.905081 airflow-provider-sifflet-1.0.1/
--rw-r--r--   0 baptiste   (501) staff       (20)     2342 2022-06-16 06:44:34.904961 airflow-provider-sifflet-1.0.1/PKG-INFO
--rw-r--r--   0 baptiste   (501) staff       (20)     1709 2022-06-16 05:54:50.000000 airflow-provider-sifflet-1.0.1/README.md
-drwxr-xr-x   0 baptiste   (501) staff       (20)        0 2022-06-16 06:44:34.904141 airflow-provider-sifflet-1.0.1/airflow_provider_sifflet.egg-info/
--rw-r--r--   0 baptiste   (501) staff       (20)     2342 2022-06-16 06:44:34.000000 airflow-provider-sifflet-1.0.1/airflow_provider_sifflet.egg-info/PKG-INFO
--rw-r--r--   0 baptiste   (501) staff       (20)      572 2022-06-16 06:44:34.000000 airflow-provider-sifflet-1.0.1/airflow_provider_sifflet.egg-info/SOURCES.txt
--rw-r--r--   0 baptiste   (501) staff       (20)        1 2022-06-16 06:44:34.000000 airflow-provider-sifflet-1.0.1/airflow_provider_sifflet.egg-info/dependency_links.txt
--rw-r--r--   0 baptiste   (501) staff       (20)       95 2022-06-16 06:44:34.000000 airflow-provider-sifflet-1.0.1/airflow_provider_sifflet.egg-info/entry_points.txt
--rw-r--r--   0 baptiste   (501) staff       (20)       37 2022-06-16 06:44:34.000000 airflow-provider-sifflet-1.0.1/airflow_provider_sifflet.egg-info/requires.txt
--rw-r--r--   0 baptiste   (501) staff       (20)       17 2022-06-16 06:44:34.000000 airflow-provider-sifflet-1.0.1/airflow_provider_sifflet.egg-info/top_level.txt
--rw-r--r--   0 baptiste   (501) staff       (20)      284 2022-06-16 05:14:01.000000 airflow-provider-sifflet-1.0.1/pyproject.toml
--rw-r--r--   0 baptiste   (501) staff       (20)       38 2022-06-16 06:44:34.905120 airflow-provider-sifflet-1.0.1/setup.cfg
--rw-r--r--   0 baptiste   (501) staff       (20)     1511 2022-06-16 05:54:48.000000 airflow-provider-sifflet-1.0.1/setup.py
-drwxr-xr-x   0 baptiste   (501) staff       (20)        0 2022-06-16 06:44:34.904340 airflow-provider-sifflet-1.0.1/sifflet_provider/
--rw-r--r--   0 baptiste   (501) staff       (20)       27 2022-06-16 05:54:50.000000 airflow-provider-sifflet-1.0.1/sifflet_provider/__init__.py
--rw-r--r--   0 baptiste   (501) staff       (20)      904 2022-06-16 05:54:50.000000 airflow-provider-sifflet-1.0.1/sifflet_provider/get_provider_info.py
-drwxr-xr-x   0 baptiste   (501) staff       (20)        0 2022-06-16 06:44:34.904519 airflow-provider-sifflet-1.0.1/sifflet_provider/hooks/
--rw-r--r--   0 baptiste   (501) staff       (20)        0 2022-06-16 05:14:01.000000 airflow-provider-sifflet-1.0.1/sifflet_provider/hooks/__init__.py
--rw-r--r--   0 baptiste   (501) staff       (20)     1755 2022-06-16 05:14:01.000000 airflow-provider-sifflet-1.0.1/sifflet_provider/hooks/sifflet_hook.py
-drwxr-xr-x   0 baptiste   (501) staff       (20)        0 2022-06-16 06:44:34.904790 airflow-provider-sifflet-1.0.1/sifflet_provider/operators/
--rw-r--r--   0 baptiste   (501) staff       (20)        0 2022-06-16 05:14:01.000000 airflow-provider-sifflet-1.0.1/sifflet_provider/operators/__init__.py
--rw-r--r--   0 baptiste   (501) staff       (20)     1776 2022-06-16 05:54:50.000000 airflow-provider-sifflet-1.0.1/sifflet_provider/operators/dbt.py
--rw-r--r--   0 baptiste   (501) staff       (20)     1327 2022-06-16 05:14:01.000000 airflow-provider-sifflet-1.0.1/sifflet_provider/operators/rule.py
+drwxr-xr-x   0 baptiste   (501) staff       (20)        0 2023-07-21 09:37:08.241206 airflow-provider-sifflet-1.0.2/
+-rw-r--r--   0 baptiste   (501) staff       (20)     2672 2023-07-21 09:37:08.241073 airflow-provider-sifflet-1.0.2/PKG-INFO
+-rw-r--r--   0 baptiste   (501) staff       (20)     2059 2023-07-10 13:24:52.000000 airflow-provider-sifflet-1.0.2/README.md
+drwxr-xr-x   0 baptiste   (501) staff       (20)        0 2023-07-21 09:37:08.239960 airflow-provider-sifflet-1.0.2/airflow_provider_sifflet.egg-info/
+-rw-r--r--   0 baptiste   (501) staff       (20)     2672 2023-07-21 09:37:08.000000 airflow-provider-sifflet-1.0.2/airflow_provider_sifflet.egg-info/PKG-INFO
+-rw-r--r--   0 baptiste   (501) staff       (20)      572 2023-07-21 09:37:08.000000 airflow-provider-sifflet-1.0.2/airflow_provider_sifflet.egg-info/SOURCES.txt
+-rw-r--r--   0 baptiste   (501) staff       (20)        1 2023-07-21 09:37:08.000000 airflow-provider-sifflet-1.0.2/airflow_provider_sifflet.egg-info/dependency_links.txt
+-rw-r--r--   0 baptiste   (501) staff       (20)       95 2023-07-21 09:37:08.000000 airflow-provider-sifflet-1.0.2/airflow_provider_sifflet.egg-info/entry_points.txt
+-rw-r--r--   0 baptiste   (501) staff       (20)       65 2023-07-21 09:37:08.000000 airflow-provider-sifflet-1.0.2/airflow_provider_sifflet.egg-info/requires.txt
+-rw-r--r--   0 baptiste   (501) staff       (20)       17 2023-07-21 09:37:08.000000 airflow-provider-sifflet-1.0.2/airflow_provider_sifflet.egg-info/top_level.txt
+-rw-r--r--   0 baptiste   (501) staff       (20)      284 2022-08-11 16:27:52.000000 airflow-provider-sifflet-1.0.2/pyproject.toml
+-rw-r--r--   0 baptiste   (501) staff       (20)       38 2023-07-21 09:37:08.241245 airflow-provider-sifflet-1.0.2/setup.cfg
+-rw-r--r--   0 baptiste   (501) staff       (20)     1701 2023-07-20 17:15:24.000000 airflow-provider-sifflet-1.0.2/setup.py
+drwxr-xr-x   0 baptiste   (501) staff       (20)        0 2023-07-21 09:37:08.240211 airflow-provider-sifflet-1.0.2/sifflet_provider/
+-rw-r--r--   0 baptiste   (501) staff       (20)       27 2023-07-20 17:15:19.000000 airflow-provider-sifflet-1.0.2/sifflet_provider/__init__.py
+-rw-r--r--   0 baptiste   (501) staff       (20)      904 2023-01-16 14:54:26.000000 airflow-provider-sifflet-1.0.2/sifflet_provider/get_provider_info.py
+drwxr-xr-x   0 baptiste   (501) staff       (20)        0 2023-07-21 09:37:08.240471 airflow-provider-sifflet-1.0.2/sifflet_provider/hooks/
+-rw-r--r--   0 baptiste   (501) staff       (20)        0 2022-08-11 16:27:52.000000 airflow-provider-sifflet-1.0.2/sifflet_provider/hooks/__init__.py
+-rw-r--r--   0 baptiste   (501) staff       (20)     1674 2023-07-20 17:15:19.000000 airflow-provider-sifflet-1.0.2/sifflet_provider/hooks/sifflet_hook.py
+drwxr-xr-x   0 baptiste   (501) staff       (20)        0 2023-07-21 09:37:08.240859 airflow-provider-sifflet-1.0.2/sifflet_provider/operators/
+-rw-r--r--   0 baptiste   (501) staff       (20)        0 2022-08-11 16:27:52.000000 airflow-provider-sifflet-1.0.2/sifflet_provider/operators/__init__.py
+-rw-r--r--   0 baptiste   (501) staff       (20)     1780 2023-07-20 17:15:19.000000 airflow-provider-sifflet-1.0.2/sifflet_provider/operators/dbt.py
+-rw-r--r--   0 baptiste   (501) staff       (20)     1331 2023-07-20 17:15:19.000000 airflow-provider-sifflet-1.0.2/sifflet_provider/operators/rule.py
```

### Comparing `airflow-provider-sifflet-1.0.1/PKG-INFO` & `airflow-provider-sifflet-1.0.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: airflow-provider-sifflet
-Version: 1.0.1
+Version: 1.0.2
 Summary: Provider package airflow-provider-sifflet for Apache Airflow
 Home-page: https://www.siffletdata.com/
 Author: Sifflet
 Author-email: support@siffletdata.com
 License: Apache License 2.0
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Framework :: Apache Airflow
 Classifier: Framework :: Apache Airflow :: Provider
 Requires-Python: ~=3.7
@@ -31,21 +30,26 @@
 pip install airflow-provider-sifflet
 ```
 
 The package supports the following python versions: 3.7, 3.8, 3.9, 3.10
 
 ## Configuration
 
-In the Airflow user interface, configure a Connection for Sifflet.
-Configure the following fields:
+In the Airflow user interface, you can configure a Connection for Sifflet in
+`Admin` -> `Connections` -> `Add a new record`.
 
-    Conn Id: sifflet_default
-    Conn Type: Sifflet
-    Sifflet Tenant: <Your tenant name>
-    Sifflet Token: <Your Sifflet access token>
+You will need to fill out the following:
+
+    Connection Id: sifflet_default
+    Connection Type: Sifflet
+    Sifflet Tenant: <your_tenant_name>
+    Sifflet Token: <your_sifflet_access_token>
+
+`<your_tenant_name>`: if you access to Sifflet with "https://abcdef.siffletdata.com", then your tenant would be `abcdef`
+`<your_sifflet_access_token>`: you can find more information on how to generate it [here](https://docs.siffletdata.com/docs/generate-an-api-token)
 
 ## Modules
 
 ### Operators
 
 #### _SiffletDbtIngestOperator_
 
@@ -80,8 +84,7 @@
         "3e19eb3e-cd20-11ec-b38b-06bb20181849",
         "3e1a86f1-cd20-11ec-b38b-06bb20181849",
         "3e2e1fc3-cd20-11ec-b38b-06bb20181849",
     ],
     error_on_rule_fail=True
 )
 ```
-
```

### Comparing `airflow-provider-sifflet-1.0.1/README.md` & `airflow-provider-sifflet-1.0.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -12,21 +12,26 @@
 pip install airflow-provider-sifflet
 ```
 
 The package supports the following python versions: 3.7, 3.8, 3.9, 3.10
 
 ## Configuration
 
-In the Airflow user interface, configure a Connection for Sifflet.
-Configure the following fields:
+In the Airflow user interface, you can configure a Connection for Sifflet in
+`Admin` -> `Connections` -> `Add a new record`.
 
-    Conn Id: sifflet_default
-    Conn Type: Sifflet
-    Sifflet Tenant: <Your tenant name>
-    Sifflet Token: <Your Sifflet access token>
+You will need to fill out the following:
+
+    Connection Id: sifflet_default
+    Connection Type: Sifflet
+    Sifflet Tenant: <your_tenant_name>
+    Sifflet Token: <your_sifflet_access_token>
+
+`<your_tenant_name>`: if you access to Sifflet with "https://abcdef.siffletdata.com", then your tenant would be `abcdef`
+`<your_sifflet_access_token>`: you can find more information on how to generate it [here](https://docs.siffletdata.com/docs/generate-an-api-token)
 
 ## Modules
 
 ### Operators
 
 #### _SiffletDbtIngestOperator_
 
@@ -60,8 +65,8 @@
         "3e2e2687-cd20-11ec-b38b-06bb20181849",
         "3e19eb3e-cd20-11ec-b38b-06bb20181849",
         "3e1a86f1-cd20-11ec-b38b-06bb20181849",
         "3e2e1fc3-cd20-11ec-b38b-06bb20181849",
     ],
     error_on_rule_fail=True
 )
-```
+```
```

### Comparing `airflow-provider-sifflet-1.0.1/airflow_provider_sifflet.egg-info/PKG-INFO` & `airflow-provider-sifflet-1.0.2/airflow_provider_sifflet.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: airflow-provider-sifflet
-Version: 1.0.1
+Version: 1.0.2
 Summary: Provider package airflow-provider-sifflet for Apache Airflow
 Home-page: https://www.siffletdata.com/
 Author: Sifflet
 Author-email: support@siffletdata.com
 License: Apache License 2.0
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Framework :: Apache Airflow
 Classifier: Framework :: Apache Airflow :: Provider
 Requires-Python: ~=3.7
@@ -31,21 +30,26 @@
 pip install airflow-provider-sifflet
 ```
 
 The package supports the following python versions: 3.7, 3.8, 3.9, 3.10
 
 ## Configuration
 
-In the Airflow user interface, configure a Connection for Sifflet.
-Configure the following fields:
+In the Airflow user interface, you can configure a Connection for Sifflet in
+`Admin` -> `Connections` -> `Add a new record`.
 
-    Conn Id: sifflet_default
-    Conn Type: Sifflet
-    Sifflet Tenant: <Your tenant name>
-    Sifflet Token: <Your Sifflet access token>
+You will need to fill out the following:
+
+    Connection Id: sifflet_default
+    Connection Type: Sifflet
+    Sifflet Tenant: <your_tenant_name>
+    Sifflet Token: <your_sifflet_access_token>
+
+`<your_tenant_name>`: if you access to Sifflet with "https://abcdef.siffletdata.com", then your tenant would be `abcdef`
+`<your_sifflet_access_token>`: you can find more information on how to generate it [here](https://docs.siffletdata.com/docs/generate-an-api-token)
 
 ## Modules
 
 ### Operators
 
 #### _SiffletDbtIngestOperator_
 
@@ -80,8 +84,7 @@
         "3e19eb3e-cd20-11ec-b38b-06bb20181849",
         "3e1a86f1-cd20-11ec-b38b-06bb20181849",
         "3e2e1fc3-cd20-11ec-b38b-06bb20181849",
     ],
     error_on_rule_fail=True
 )
 ```
-
```

### Comparing `airflow-provider-sifflet-1.0.1/airflow_provider_sifflet.egg-info/SOURCES.txt` & `airflow-provider-sifflet-1.0.2/airflow_provider_sifflet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `airflow-provider-sifflet-1.0.1/setup.py` & `airflow-provider-sifflet-1.0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         name="airflow-provider-sifflet",
         description="Provider package airflow-provider-sifflet for Apache Airflow",
         version=sifflet_provider.__version__,
         long_description=long_description,
         long_description_content_type="text/markdown",
         license="Apache License 2.0",
         packages=find_packages(include=["sifflet_provider", "sifflet_provider.*"]),
-        install_requires=["sifflet>=0.2.1"],
+        install_requires=["sifflet-sdk>=0.3.0"],
         setup_requires=["setuptools", "wheel"],
         author="Sifflet",
         author_email="support@siffletdata.com",
         url="https://www.siffletdata.com/",
         classifiers=[
             "Development Status :: 4 - Beta",
             "Environment :: Console",
@@ -32,14 +32,16 @@
             "Framework :: Apache Airflow :: Provider",
         ],
         python_requires="~=3.7",
         entry_points={
             "apache_airflow_provider": ["provider_info=sifflet_provider.get_provider_info:get_provider_info"]
         },
         extras_require={
-            "dev": ["apache-airflow"],
+            # 2023-07-10, the current released airflow package as dependency conflict with pydantic
+            # https://github.com/apache/airflow/pull/32312
+            "dev": ["apache-airflow", "pydantic>=1.10.0,<2.0.0"],
         },
     )
 
 
 if __name__ == "__main__":
     do_setup()
```

### Comparing `airflow-provider-sifflet-1.0.1/sifflet_provider/get_provider_info.py` & `airflow-provider-sifflet-1.0.2/sifflet_provider/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `airflow-provider-sifflet-1.0.1/sifflet_provider/hooks/sifflet_hook.py` & `airflow-provider-sifflet-1.0.2/sifflet_provider/hooks/sifflet_hook.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from typing import Dict
 
 from airflow.hooks.base import BaseHook
-
-from sifflet.configure.service import SiffletConfig
+from sifflet_sdk.config import SiffletConfig
 
 
 class SiffletHook(BaseHook):
     """
     Hook for Sifflet interaction.
 
     This hook requires authentication details:
@@ -41,10 +40,9 @@
     def get_conn(self) -> SiffletConfig:
         """Returns the SiffletConfig for the current connection id."""
         conn = self.get_connection(self.sifflet_conn_id)
         conn_params = conn.extra_dejson
 
         tenant = conn.schema
         token = conn.password
-        dev_mode = conn_params.get("dev_mode", False)
         debug = conn_params.get("debug", False)
-        return SiffletConfig(tenant=tenant, token=token, dev_mode=dev_mode, debug=debug)
+        return SiffletConfig(tenant=tenant, token=token, debug=debug)
```

### Comparing `airflow-provider-sifflet-1.0.1/sifflet_provider/operators/dbt.py` & `airflow-provider-sifflet-1.0.2/sifflet_provider/operators/dbt.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Sequence
 
 from airflow.models.baseoperator import BaseOperator
 from airflow.utils.trigger_rule import TriggerRule
+from sifflet_sdk.ingest.service import IngestionService
 
-from sifflet.ingest.service import IngestionService
 from sifflet_provider.hooks.sifflet_hook import SiffletHook
 
 
 class SiffletDbtIngestOperator(BaseOperator):
     ui_color = "#fff"
     ui_fgcolor = "#113e60"
```

### Comparing `airflow-provider-sifflet-1.0.1/sifflet_provider/operators/rule.py` & `airflow-provider-sifflet-1.0.2/sifflet_provider/operators/rule.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import List, Sequence
 
 from airflow.models.baseoperator import BaseOperator
+from sifflet_sdk.rules.service import RulesService
 
-from sifflet.rules.service import RulesService
 from sifflet_provider.hooks.sifflet_hook import SiffletHook
 
 
 class SiffletRunRuleOperator(BaseOperator):
     ui_color = "#fff"
     ui_fgcolor = "#113e60"
```

