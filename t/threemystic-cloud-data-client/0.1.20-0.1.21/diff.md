# Comparing `tmp/threemystic_cloud_data_client-0.1.20.tar.gz` & `tmp/threemystic_cloud_data_client-0.1.21.tar.gz`

## Comparing `threemystic_cloud_data_client-0.1.20.tar` & `threemystic_cloud_data_client-0.1.21.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.20/threemystic_cloud_data_client/__main__.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.20/threemystic_cloud_data_client/__version__.py
--rw-r--r--   0        0        0     3895 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.20/threemystic_cloud_data_client/cloud_data_client.py
--rw-r--r--   0        0        0     4150 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.20/threemystic_cloud_data_client/cli/__init__.py
--rw-r--r--   0        0        0     2950 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.20/threemystic_cloud_data_client/cli/actions/base_class/base.py
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.20/threemystic_cloud_data_client/cli/actions/config/__init__.py
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.20/threemystic_cloud_data_client/cloud_providers/aws/__init__.py
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.20/threemystic_cloud_data_client/cloud_providers/aws/base_class/base.py
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.20/threemystic_cloud_data_client/cloud_providers/aws/client/__init__.py
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.20/threemystic_cloud_data_client/cloud_providers/aws/client/actions/vmimage.py
--rw-r--r--   0        0        0     5122 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.20/threemystic_cloud_data_client/cloud_providers/aws/client/actions/base_class/base.py
--rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.20/threemystic_cloud_data_client/cloud_providers/aws/config/step_1.py
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.20/threemystic_cloud_data_client/cloud_providers/aws/config/base_class/base.py
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.20/threemystic_cloud_data_client/cloud_providers/azure/__init__.py
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.20/threemystic_cloud_data_client/cloud_providers/azure/base_class/base.py
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.20/threemystic_cloud_data_client/cloud_providers/azure/client/__init__.py
--rw-r--r--   0        0        0    23358 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.20/threemystic_cloud_data_client/cloud_providers/azure/client/actions/budget.py
--rw-r--r--   0        0        0     4752 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.20/threemystic_cloud_data_client/cloud_providers/azure/client/actions/certificates.py
--rw-r--r--   0        0        0     5548 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.20/threemystic_cloud_data_client/cloud_providers/azure/client/actions/cloudstorage.py
--rw-r--r--   0        0        0    11920 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.20/threemystic_cloud_data_client/cloud_providers/azure/client/actions/database.py
--rw-r--r--   0        0        0     2368 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.20/threemystic_cloud_data_client/cloud_providers/azure/client/actions/datawarehouse.py
--rw-r--r--   0        0        0    10170 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.20/threemystic_cloud_data_client/cloud_providers/azure/client/actions/dns.py
--rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.20/threemystic_cloud_data_client/cloud_providers/azure/client/actions/memorydb.py
--rw-r--r--   0        0        0     5770 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.20/threemystic_cloud_data_client/cloud_providers/azure/client/actions/secrets.py
--rw-r--r--   0        0        0    13107 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.20/threemystic_cloud_data_client/cloud_providers/azure/client/actions/storage.py
--rw-r--r--   0        0        0    11874 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.20/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vm.py
--rw-r--r--   0        0        0     3175 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.20/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vmimage.py
--rw-r--r--   0        0        0     3172 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.20/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vmss.py
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.20/threemystic_cloud_data_client/cloud_providers/azure/client/actions/base_class/base.py
--rw-r--r--   0        0        0     2917 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.20/threemystic_cloud_data_client/cloud_providers/azure/config/step_1.py
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.20/threemystic_cloud_data_client/cloud_providers/azure/config/base_class/base.py
--rw-r--r--   0        0        0     8657 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.20/threemystic_cloud_data_client/cloud_providers/base_class/base.py
--rw-r--r--   0        0        0    11700 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.20/threemystic_cloud_data_client/cloud_providers/base_class/base_client.py
--rw-r--r--   0        0        0    21820 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.20/threemystic_cloud_data_client/cloud_providers/base_class/base_data.py
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.20/threemystic_cloud_data_client/cloud_providers/general/__init__.py
--rw-r--r--   0        0        0     4709 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.20/threemystic_cloud_data_client/cloud_providers/general/config/step_1.py
--rw-r--r--   0        0        0    14025 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.20/threemystic_cloud_data_client/cloud_providers/general/config/step_2.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.20/threemystic_cloud_data_client/cloud_providers/general/config/base_class/base.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.20/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.20/LICENSE
--rw-r--r--   0        0        0     2715 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.20/README.md
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.20/hatch.toml
--rw-r--r--   0        0        0     3753 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.20/pyproject.toml
--rw-r--r--   0        0        0     4639 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.20/PKG-INFO
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/__main__.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/__version__.py
+-rw-r--r--   0        0        0     3895 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_data_client.py
+-rw-r--r--   0        0        0     4150 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cli/__init__.py
+-rw-r--r--   0        0        0     2950 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cli/actions/base_class/base.py
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cli/actions/config/__init__.py
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/aws/__init__.py
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/aws/base_class/base.py
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/aws/client/__init__.py
+-rw-r--r--   0        0        0     1481 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/aws/client/actions/vmimage.py
+-rw-r--r--   0        0        0     5122 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/aws/client/actions/base_class/base.py
+-rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/aws/config/step_1.py
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/aws/config/base_class/base.py
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/azure/__init__.py
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/azure/base_class/base.py
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/azure/client/__init__.py
+-rw-r--r--   0        0        0    23320 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/azure/client/actions/budget.py
+-rw-r--r--   0        0        0     4713 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/azure/client/actions/certificates.py
+-rw-r--r--   0        0        0     5509 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/azure/client/actions/cloudstorage.py
+-rw-r--r--   0        0        0    11881 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/azure/client/actions/database.py
+-rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/azure/client/actions/datawarehouse.py
+-rw-r--r--   0        0        0    10131 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/azure/client/actions/dns.py
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/azure/client/actions/memorydb.py
+-rw-r--r--   0        0        0     5731 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/azure/client/actions/secrets.py
+-rw-r--r--   0        0        0    13068 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/azure/client/actions/storage.py
+-rw-r--r--   0        0        0    11835 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vm.py
+-rw-r--r--   0        0        0     3136 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vmimage.py
+-rw-r--r--   0        0        0     3134 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vmss.py
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/azure/client/actions/base_class/base.py
+-rw-r--r--   0        0        0     2917 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/azure/config/step_1.py
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/azure/config/base_class/base.py
+-rw-r--r--   0        0        0     8657 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/base_class/base.py
+-rw-r--r--   0        0        0    11700 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/base_class/base_client.py
+-rw-r--r--   0        0        0    21547 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/base_class/base_data.py
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/general/__init__.py
+-rw-r--r--   0        0        0     4709 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/general/config/step_1.py
+-rw-r--r--   0        0        0    14025 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/general/config/step_2.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/general/config/base_class/base.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.21/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.21/LICENSE
+-rw-r--r--   0        0        0     2715 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.21/README.md
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.21/hatch.toml
+-rw-r--r--   0        0        0     3753 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.21/pyproject.toml
+-rw-r--r--   0        0        0     4639 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.21/PKG-INFO
```

### Comparing `threemystic_cloud_data_client-0.1.20/threemystic_cloud_data_client/cloud_data_client.py` & `threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_data_client.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.20/threemystic_cloud_data_client/cli/__init__.py` & `threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.20/threemystic_cloud_data_client/cli/actions/base_class/base.py` & `threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cli/actions/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.20/threemystic_cloud_data_client/cli/actions/config/__init__.py` & `threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cli/actions/config/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.20/threemystic_cloud_data_client/cloud_providers/aws/__init__.py` & `threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.20/threemystic_cloud_data_client/cloud_providers/aws/client/actions/vmimage.py` & `threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/aws/client/actions/vmimage.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from threemystic_cloud_data_client.cloud_providers.aws.client.actions.base_class.base import cloud_data_client_aws_client_action_base as base
 import asyncio
 
 
 class cloud_data_client_aws_client_action(base):
   def __init__(self, *args, **kwargs):
     super().__init__(
-      data_action="ami", 
-      logger_name= "cloud_data_client_aws_client_action",
-      uniqueid_lambda = lambda: True,
+      data_action="vmimage",
+      logger_name= "cloud_data_client_aws_client_action_vmimage",
       *args, **kwargs)
     
     
     self.data_id_name = "ImageId"
     
     self.arn_lambda = (lambda item: self.get_cloud_client().get_resource_general_arn(
       resource_type= "ec2",
```

### Comparing `threemystic_cloud_data_client-0.1.20/threemystic_cloud_data_client/cloud_providers/aws/client/actions/base_class/base.py` & `threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/aws/client/actions/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.20/threemystic_cloud_data_client/cloud_providers/aws/config/step_1.py` & `threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/aws/config/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.20/threemystic_cloud_data_client/cloud_providers/azure/__init__.py` & `threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/azure/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.20/threemystic_cloud_data_client/cloud_providers/azure/client/actions/budget.py` & `threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/azure/client/actions/budget.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from azure.mgmt.costmanagement.models import GranularityType,ForecastDefinition,ForecastType,ForecastTimeframe,ForecastTimePeriod,QueryDefinition,TimeframeType,ExportType,QueryTimePeriod
 
 class cloud_data_client_azure_client_action(base):
   def __init__(self, *args, **kwargs):
     super().__init__(
       data_action="budget", 
       logger_name= "cloud_data_client_azure_client_action_budget",
-      uniqueid_lambda = lambda: True,
       *args, **kwargs)
   
   def __process_get_cost_generate_data(self, account, client, cost_filter, is_forcast = False, *args, **kwargs):
     if not is_forcast:
       return self.get_cloud_client().sdk_request(
         tenant= self.get_cloud_client().get_tenant_id(tenant= account, is_account= True), 
         lambda_sdk_command=lambda: client.query.usage(
```

### Comparing `threemystic_cloud_data_client-0.1.20/threemystic_cloud_data_client/cloud_providers/azure/client/actions/certificates.py` & `threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/azure/client/actions/certificates.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,15 @@
 from azure.keyvault.keys import KeyClient
 
 
 class cloud_data_client_azure_client_action(base):
   def __init__(self, *args, **kwargs):
     super().__init__(
       data_action="certificates", 
-      logger_name= "cloud_data_client_azure_client_action_certificates", 
-      uniqueid_lambda = lambda: True,
+      logger_name= "cloud_data_client_azure_client_action_certificates",
       *args, **kwargs)
   
   async def __process_get_resources_key_vault_keys(self, account, key_vault, *args, **kwargs):    
     try:
       client = KeyClient(vault_url= f'https://{key_vault}.vault.azure.net/', credential= self.get_cloud_client().get_tenant_credential(tenant= self.get_cloud_client().get_tenant_id(tenant= account, is_account= True)), subscription_id= self.get_cloud_client().get_account_id(account= account))
       
       return [ key for key in self.get_cloud_client().sdk_request(
```

### Comparing `threemystic_cloud_data_client-0.1.20/threemystic_cloud_data_client/cloud_providers/azure/client/actions/cloudstorage.py` & `threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/azure/client/actions/cloudstorage.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,15 @@
 from azure.mgmt.monitor import MonitorManagementClient
 from decimal import Decimal, ROUND_HALF_UP
 
 class cloud_data_client_azure_client_action(base):
   def __init__(self, *args, **kwargs):
     super().__init__(
       data_action="cloudstorage", 
-      logger_name= "cloud_data_client_azure_client_action_cloudstorage", 
-      uniqueid_lambda = lambda: True,
+      logger_name= "cloud_data_client_azure_client_action_cloudstorage",
       *args, **kwargs)
   
   
   async def _process_account_data_storage_size(self, client, account, storage_account, **kwargs):
       try:
         
         storage_account_name= self.get_cloud_client().get_resource_name_from_resource(resource= storage_account)
```

### Comparing `threemystic_cloud_data_client-0.1.20/threemystic_cloud_data_client/cloud_providers/azure/client/actions/database.py` & `threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/azure/client/actions/database.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,16 +7,15 @@
 from azure.mgmt.rdbms.mariadb import MariaDBManagementClient
 from azure.mgmt.rdbms.postgresql import PostgreSQLManagementClient
 
 class cloud_data_client_azure_client_action(base):
   def __init__(self, *args, **kwargs):
     super().__init__(
       data_action="database", 
-      logger_name= "cloud_data_client_azure_client_action_database", 
-      uniqueid_lambda = lambda: True,
+      logger_name= "cloud_data_client_azure_client_action_database",
       *args, **kwargs)
   
   async def __process_get_db_sql(self, client, account, *args, **kwargs):    
     try:
       return_data = []
       for db in self.get_cloud_client().sdk_request(
         tenant= self.get_cloud_client().get_tenant_id(tenant= account, is_account= True),
```

### Comparing `threemystic_cloud_data_client-0.1.20/threemystic_cloud_data_client/cloud_providers/azure/client/actions/datawarehouse.py` & `threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/azure/client/actions/datawarehouse.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,16 +3,15 @@
 from azure.mgmt.synapse import SynapseManagementClient
 
 
 class cloud_data_client_azure_client_action(base):
   def __init__(self, *args, **kwargs):
     super().__init__(
       data_action="datawarehouse", 
-      logger_name= "cloud_data_client_azure_client_action_datawarehouse", 
-      uniqueid_lambda = lambda: True,
+      logger_name= "cloud_data_client_azure_client_action_datawarehouse",
       *args, **kwargs)
   
  
   async def _process_account_data(self, account, loop, *args, **kwargs):
     
     client = SynapseManagementClient(credential= self.get_cloud_client().get_tenant_credential(tenant= self.get_cloud_client().get_tenant_id(tenant= account, is_account= True)), subscription_id= self.get_cloud_client().get_account_id(account= account))
```

### Comparing `threemystic_cloud_data_client-0.1.20/threemystic_cloud_data_client/cloud_providers/azure/client/actions/dns.py` & `threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/azure/client/actions/dns.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,16 +6,15 @@
 
 
 
 class cloud_data_client_azure_client_action(base):
   def __init__(self, *args, **kwargs):
     super().__init__(
       data_action="dns", 
-      logger_name= "cloud_data_client_azure_client_action_dns", 
-      uniqueid_lambda = lambda: True,
+      logger_name= "cloud_data_client_azure_client_action_dns",
       *args, **kwargs)
   
   async def __process_get_resources_public(self, client, account, *args, **kwargs):    
     try:      
       return { self.get_cloud_client().get_resource_id_from_resource(resource= dns):dns for dns in self.get_cloud_client().sdk_request(
           tenant= self.get_cloud_client().get_tenant_id(tenant= account, is_account= True), 
           lambda_sdk_command=lambda: client.zones.list()
```

### Comparing `threemystic_cloud_data_client-0.1.20/threemystic_cloud_data_client/cloud_providers/azure/client/actions/memorydb.py` & `threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/azure/client/actions/memorydb.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,16 +3,15 @@
 from azure.mgmt.redis import RedisManagementClient
 
 
 class cloud_data_client_azure_client_action(base):
   def __init__(self, *args, **kwargs):
     super().__init__(
       data_action="memorydb", 
-      logger_name= "cloud_data_client_azure_client_action_memorydb", 
-      uniqueid_lambda = lambda: True,
+      logger_name= "cloud_data_client_azure_client_action_memorydb",
       *args, **kwargs)
   
  
   async def _process_account_data(self, account, loop, *args, **kwargs):
     
     client = RedisManagementClient(credential= self.get_cloud_client().get_tenant_credential(tenant= self.get_cloud_client().get_tenant_id(tenant= account, is_account= True)), subscription_id= self.get_cloud_client().get_account_id(account= account))
```

### Comparing `threemystic_cloud_data_client-0.1.20/threemystic_cloud_data_client/cloud_providers/azure/client/actions/secrets.py` & `threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/azure/client/actions/secrets.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,15 @@
 from azure.keyvault.administration import KeyVaultAccessControlClient
 
 
 class cloud_data_client_azure_client_action(base):
   def __init__(self, *args, **kwargs):
     super().__init__(
       data_action="secrets", 
-      logger_name= "cloud_data_client_azure_client_action_secrets", 
-      uniqueid_lambda = lambda: True,
+      logger_name= "cloud_data_client_azure_client_action_secrets",
       *args, **kwargs)
   
   async def __process_get_resources_key_vault_access_key(self, account, key_vault, *args, **kwargs):    
     try:
       client = KeyVaultAccessControlClient(vault_url= f'https://{key_vault}.vault.azure.net/', credential= self.get_cloud_client().get_tenant_credential(tenant= self.get_cloud_client().get_tenant_id(tenant= account, is_account= True)), subscription_id= self.get_cloud_client().get_account_id(account= account))
       
       # oid = print(self.get_cloud_client().get_tenant_credential_full(tenant= self.get_cloud_client().get_tenant_id(tenant= account, is_account= True)).get("jwt").get("oid"))
```

### Comparing `threemystic_cloud_data_client-0.1.20/threemystic_cloud_data_client/cloud_providers/azure/client/actions/storage.py` & `threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/azure/client/actions/storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,15 @@
 from threemystic_cloud_data_client.cloud_providers.azure.client.actions.vm import cloud_data_client_azure_client_action as vm_action
 from threemystic_cloud_data_client.cloud_providers.azure.client.actions.vmss import cloud_data_client_azure_client_action as vmss_action
 
 class cloud_data_client_azure_client_action(base):
   def __init__(self, *args, **kwargs):
     super().__init__(
       data_action="storage", 
-      logger_name= "cloud_data_client_azure_client_action_storage", 
-      uniqueid_lambda = lambda: True,
+      logger_name= "cloud_data_client_azure_client_action_storage",
       *args, **kwargs)
   
   
     
   def __get_cost_by_resource_query_definition_mtd(self):
     mtd = self.get_cloud_client().get_default_querydefinition()
     mtd.timeframe = TimeframeType.MONTH_TO_DATE
```

### Comparing `threemystic_cloud_data_client-0.1.20/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vm.py` & `threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vm.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,16 +6,15 @@
 from azure.mgmt.network.models import LoadBalancer
 
 
 class cloud_data_client_azure_client_action(base):
   def __init__(self, *args, **kwargs):
     super().__init__(
       data_action="vm", 
-      logger_name= "cloud_data_client_azure_client_action_vm", 
-      uniqueid_lambda = lambda: True,
+      logger_name= "cloud_data_client_azure_client_action_vm",
       *args, **kwargs)
   
   
 
   async def __process_get_resources_vm_public_ips(self, account, *args, **kwargs):    
     try:
         client = NetworkManagementClient(credential= self.get_cloud_client().get_tenant_credential(tenant= self.get_cloud_client().get_tenant_id(tenant= account, is_account= True)), subscription_id= self.get_cloud_client().get_account_id(account= account))
```

### Comparing `threemystic_cloud_data_client-0.1.20/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vmimage.py` & `threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vmimage.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,15 @@
 
 
 
 class cloud_data_client_azure_client_action(base):
   def __init__(self, *args, **kwargs):
     super().__init__(
       data_action="vmimage", 
-      logger_name= "cloud_data_client_azure_client_action_vmimage", 
-      uniqueid_lambda = lambda: True,
+      logger_name= "cloud_data_client_azure_client_action_vmimage",
       *args, **kwargs)
       
   async def _process_account_data(self, account, loop, *args, **kwargs):
     client = ComputeManagementClient(credential= self.get_cloud_client().get_tenant_credential(tenant= self.get_cloud_client().get_tenant_id(tenant= account, is_account= True)), subscription_id= self.get_cloud_client().get_account_id(account= account))
     image_galleries = self.get_cloud_client().sdk_request(
            tenant= self.get_cloud_client().get_tenant_id(tenant= account, is_account= True), 
            lambda_sdk_command=lambda: client.galleries.list()
```

### Comparing `threemystic_cloud_data_client-0.1.20/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vmss.py` & `threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vmss.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,15 @@
 from azure.mgmt.resource import ResourceManagementClient
 
 
 class cloud_data_client_azure_client_action(base):
   def __init__(self, *args, **kwargs):
     super().__init__(
       data_action="vmss", 
-      logger_name= "cloud_data_client_azure_client_action_vmss", 
-      uniqueid_lambda = lambda: True, 
+      logger_name= "cloud_data_client_azure_client_action_vmss",  
       *args, **kwargs)
   
   
     
   async def __process_get_resources_vmss(self, account, *args, **kwargs):
     resource_client = ResourceManagementClient(credential= self.get_cloud_client().get_tenant_credential(tenant= self.get_cloud_client().get_tenant_id(tenant= account, is_account= True)), subscription_id= self.get_cloud_client().get_account_id(account= account))
     try:
```

### Comparing `threemystic_cloud_data_client-0.1.20/threemystic_cloud_data_client/cloud_providers/azure/client/actions/base_class/base.py` & `threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/azure/client/actions/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.20/threemystic_cloud_data_client/cloud_providers/azure/config/step_1.py` & `threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/azure/config/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.20/threemystic_cloud_data_client/cloud_providers/base_class/base.py` & `threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.20/threemystic_cloud_data_client/cloud_providers/base_class/base_client.py` & `threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/base_class/base_client.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.20/threemystic_cloud_data_client/cloud_providers/base_class/base_data.py` & `threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/base_class/base_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 
 class cloud_data_client_provider_base_data(base):
   def __init__(self, *args, **kwargs):
     super().__init__(*args, **kwargs)   
     
     self._set_cloud_data_client(*args, **kwargs)
     self._set_client_name(*args, **kwargs)
-    self._set_resource_uniqueid_lambda(*args, **kwargs)
     self._set_max_process_pool(*args, **kwargs)
     self._set_max_thread_pool(*args, **kwargs)
     self._set_data_start(*args, **kwargs)
 
   @abstractmethod
   def get_accounts(self):
     pass
@@ -53,20 +52,14 @@
     self._cloud_data_client = cloud_data_client
 
   def get_client_name(self, *args, **kwargs):
     return self._client_name
   
   def _set_client_name(self, data_action, *args, **kwargs):
     self._client_name = f"{self.get_provider()}-{data_action}-data"
-
-  def get_resource_uniqueid_lambda(self, *args, **kwargs):
-    return self._uniqueid_lambda
-  
-  def _set_resource_uniqueid_lambda(self, uniqueid_lambda, *args, **kwargs):
-    self._uniqueid_lambda = uniqueid_lambda
   
   async def _pre_load_main_process(self, *args, **kwargs):
     pass
 
   async def _get_environment(self, account = None, resource = None, *args, **kwargs):
     resource_name = self.get_common().helper_type().string().set_case(string_value= self.get_cloud_client().get_resource_name(resource= resource), case= "lower")
     account_name = self.get_common().helper_type().string().set_case(string_value= self.get_cloud_client().get_account_name(account= account), case= "lower")
```

### Comparing `threemystic_cloud_data_client-0.1.20/threemystic_cloud_data_client/cloud_providers/general/__init__.py` & `threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/general/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.20/threemystic_cloud_data_client/cloud_providers/general/config/step_1.py` & `threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/general/config/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.20/threemystic_cloud_data_client/cloud_providers/general/config/step_2.py` & `threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/general/config/step_2.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.20/.gitignore` & `threemystic_cloud_data_client-0.1.21/.gitignore`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.20/LICENSE` & `threemystic_cloud_data_client-0.1.21/LICENSE`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.20/README.md` & `threemystic_cloud_data_client-0.1.21/README.md`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.20/hatch.toml` & `threemystic_cloud_data_client-0.1.21/hatch.toml`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.20/pyproject.toml` & `threemystic_cloud_data_client-0.1.21/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
   "colorama; platform_system == 'Windows'",
   "threemystic-common >= 0.1.15",
-  "threemystic-cloud-client >= 0.1.38",
+  "threemystic-cloud-client >= 0.1.39",
   "typing-extensions >= 4.4.0",
   "asyncio >= 3.4.3",
   "tqdm >= 4.65.0",
   "azure-mgmt-cosmosdb >= 9",
   "azure-mgmt-costmanagement >= 4",
   "azure-mgmt-dns >= 8",
   "azure-mgmt-keyvault >= 10",
```

### Comparing `threemystic_cloud_data_client-0.1.20/PKG-INFO` & `threemystic_cloud_data_client-0.1.21/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threemystic-cloud-data-client
-Version: 0.1.20
+Version: 0.1.21
 Summary: A tool for collecting data from various cloud providers
 Project-URL: Homepage, https://github.com/3MysticApes/3mystic_cloud_data_client
 Project-URL: Bug Tracker, https://github.com/3MysticApes/3mystic_cloud_data_client/issues
 Author: Ron Truex
 License-Expression: MIT
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
@@ -34,15 +34,15 @@
 Requires-Dist: azure-mgmt-redis>=14
 Requires-Dist: azure-mgmt-resourcegraph>=8
 Requires-Dist: azure-mgmt-sql>=3
 Requires-Dist: azure-mgmt-sqlvirtualmachine>=0.6
 Requires-Dist: azure-mgmt-subscription>=3
 Requires-Dist: azure-mgmt-synapse>=2
 Requires-Dist: colorama; platform_system == 'Windows'
-Requires-Dist: threemystic-cloud-client>=0.1.38
+Requires-Dist: threemystic-cloud-client>=0.1.39
 Requires-Dist: threemystic-common>=0.1.15
 Requires-Dist: tqdm>=4.65.0
 Requires-Dist: typing-extensions>=4.4.0
 Description-Content-Type: text/markdown
 
 # 3mystic_cloud_data_client
 A set of scripts to help uniformly pull data from the cloud providers for various resources.
```

