# Comparing `tmp/threemystic_cloud_data_client-0.1.21.tar.gz` & `tmp/threemystic_cloud_data_client-0.1.22.tar.gz`

## Comparing `threemystic_cloud_data_client-0.1.21.tar` & `threemystic_cloud_data_client-0.1.22.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/__main__.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/__version__.py
--rw-r--r--   0        0        0     3895 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_data_client.py
--rw-r--r--   0        0        0     4150 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cli/__init__.py
--rw-r--r--   0        0        0     2950 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cli/actions/base_class/base.py
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cli/actions/config/__init__.py
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/aws/__init__.py
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/aws/base_class/base.py
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/aws/client/__init__.py
--rw-r--r--   0        0        0     1481 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/aws/client/actions/vmimage.py
--rw-r--r--   0        0        0     5122 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/aws/client/actions/base_class/base.py
--rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/aws/config/step_1.py
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/aws/config/base_class/base.py
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/azure/__init__.py
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/azure/base_class/base.py
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/azure/client/__init__.py
--rw-r--r--   0        0        0    23320 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/azure/client/actions/budget.py
--rw-r--r--   0        0        0     4713 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/azure/client/actions/certificates.py
--rw-r--r--   0        0        0     5509 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/azure/client/actions/cloudstorage.py
--rw-r--r--   0        0        0    11881 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/azure/client/actions/database.py
--rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/azure/client/actions/datawarehouse.py
--rw-r--r--   0        0        0    10131 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/azure/client/actions/dns.py
--rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/azure/client/actions/memorydb.py
--rw-r--r--   0        0        0     5731 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/azure/client/actions/secrets.py
--rw-r--r--   0        0        0    13068 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/azure/client/actions/storage.py
--rw-r--r--   0        0        0    11835 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vm.py
--rw-r--r--   0        0        0     3136 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vmimage.py
--rw-r--r--   0        0        0     3134 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vmss.py
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/azure/client/actions/base_class/base.py
--rw-r--r--   0        0        0     2917 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/azure/config/step_1.py
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/azure/config/base_class/base.py
--rw-r--r--   0        0        0     8657 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/base_class/base.py
--rw-r--r--   0        0        0    11700 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/base_class/base_client.py
--rw-r--r--   0        0        0    21547 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/base_class/base_data.py
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/general/__init__.py
--rw-r--r--   0        0        0     4709 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/general/config/step_1.py
--rw-r--r--   0        0        0    14025 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/general/config/step_2.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/general/config/base_class/base.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.21/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.21/LICENSE
--rw-r--r--   0        0        0     2715 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.21/README.md
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.21/hatch.toml
--rw-r--r--   0        0        0     3753 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.21/pyproject.toml
--rw-r--r--   0        0        0     4639 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.21/PKG-INFO
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.22/threemystic_cloud_data_client/__main__.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.22/threemystic_cloud_data_client/__version__.py
+-rw-r--r--   0        0        0     3895 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.22/threemystic_cloud_data_client/cloud_data_client.py
+-rw-r--r--   0        0        0     4150 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.22/threemystic_cloud_data_client/cli/__init__.py
+-rw-r--r--   0        0        0     2950 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.22/threemystic_cloud_data_client/cli/actions/base_class/base.py
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.22/threemystic_cloud_data_client/cli/actions/config/__init__.py
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.22/threemystic_cloud_data_client/cloud_providers/aws/__init__.py
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.22/threemystic_cloud_data_client/cloud_providers/aws/base_class/base.py
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.22/threemystic_cloud_data_client/cloud_providers/aws/client/__init__.py
+-rw-r--r--   0        0        0     1481 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.22/threemystic_cloud_data_client/cloud_providers/aws/client/actions/vmimage.py
+-rw-r--r--   0        0        0     5122 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.22/threemystic_cloud_data_client/cloud_providers/aws/client/actions/base_class/base.py
+-rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.22/threemystic_cloud_data_client/cloud_providers/aws/config/step_1.py
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.22/threemystic_cloud_data_client/cloud_providers/aws/config/base_class/base.py
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.22/threemystic_cloud_data_client/cloud_providers/azure/__init__.py
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.22/threemystic_cloud_data_client/cloud_providers/azure/base_class/base.py
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.22/threemystic_cloud_data_client/cloud_providers/azure/client/__init__.py
+-rw-r--r--   0        0        0    23320 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.22/threemystic_cloud_data_client/cloud_providers/azure/client/actions/budget.py
+-rw-r--r--   0        0        0     4629 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.22/threemystic_cloud_data_client/cloud_providers/azure/client/actions/certificates.py
+-rw-r--r--   0        0        0     5358 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.22/threemystic_cloud_data_client/cloud_providers/azure/client/actions/cloudstorage.py
+-rw-r--r--   0        0        0    11867 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.22/threemystic_cloud_data_client/cloud_providers/azure/client/actions/database.py
+-rw-r--r--   0        0        0     2315 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.22/threemystic_cloud_data_client/cloud_providers/azure/client/actions/datawarehouse.py
+-rw-r--r--   0        0        0    10075 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.22/threemystic_cloud_data_client/cloud_providers/azure/client/actions/dns.py
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.22/threemystic_cloud_data_client/cloud_providers/azure/client/actions/memorydb.py
+-rw-r--r--   0        0        0     5647 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.22/threemystic_cloud_data_client/cloud_providers/azure/client/actions/secrets.py
+-rw-r--r--   0        0        0    13040 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.22/threemystic_cloud_data_client/cloud_providers/azure/client/actions/storage.py
+-rw-r--r--   0        0        0    11527 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.22/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vm.py
+-rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.22/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vmimage.py
+-rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.22/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vmss.py
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.22/threemystic_cloud_data_client/cloud_providers/azure/client/actions/base_class/base.py
+-rw-r--r--   0        0        0     2917 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.22/threemystic_cloud_data_client/cloud_providers/azure/config/step_1.py
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.22/threemystic_cloud_data_client/cloud_providers/azure/config/base_class/base.py
+-rw-r--r--   0        0        0     8657 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.22/threemystic_cloud_data_client/cloud_providers/base_class/base.py
+-rw-r--r--   0        0        0    11700 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.22/threemystic_cloud_data_client/cloud_providers/base_class/base_client.py
+-rw-r--r--   0        0        0    21547 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.22/threemystic_cloud_data_client/cloud_providers/base_class/base_data.py
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.22/threemystic_cloud_data_client/cloud_providers/general/__init__.py
+-rw-r--r--   0        0        0     4709 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.22/threemystic_cloud_data_client/cloud_providers/general/config/step_1.py
+-rw-r--r--   0        0        0    14025 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.22/threemystic_cloud_data_client/cloud_providers/general/config/step_2.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.22/threemystic_cloud_data_client/cloud_providers/general/config/base_class/base.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.22/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.22/LICENSE
+-rw-r--r--   0        0        0     2715 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.22/README.md
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.22/hatch.toml
+-rw-r--r--   0        0        0     3753 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.22/pyproject.toml
+-rw-r--r--   0        0        0     4639 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.22/PKG-INFO
```

### Comparing `threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_data_client.py` & `threemystic_cloud_data_client-0.1.22/threemystic_cloud_data_client/cloud_data_client.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cli/__init__.py` & `threemystic_cloud_data_client-0.1.22/threemystic_cloud_data_client/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cli/actions/base_class/base.py` & `threemystic_cloud_data_client-0.1.22/threemystic_cloud_data_client/cli/actions/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cli/actions/config/__init__.py` & `threemystic_cloud_data_client-0.1.22/threemystic_cloud_data_client/cli/actions/config/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/aws/__init__.py` & `threemystic_cloud_data_client-0.1.22/threemystic_cloud_data_client/cloud_providers/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/aws/client/actions/vmimage.py` & `threemystic_cloud_data_client-0.1.22/threemystic_cloud_data_client/cloud_providers/aws/client/actions/vmimage.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/aws/client/actions/base_class/base.py` & `threemystic_cloud_data_client-0.1.22/threemystic_cloud_data_client/cloud_providers/aws/client/actions/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/aws/config/step_1.py` & `threemystic_cloud_data_client-0.1.22/threemystic_cloud_data_client/cloud_providers/aws/config/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/azure/__init__.py` & `threemystic_cloud_data_client-0.1.22/threemystic_cloud_data_client/cloud_providers/azure/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/azure/client/actions/budget.py` & `threemystic_cloud_data_client-0.1.22/threemystic_cloud_data_client/cloud_providers/azure/client/actions/budget.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/azure/client/actions/certificates.py` & `threemystic_cloud_data_client-0.1.22/threemystic_cloud_data_client/cloud_providers/azure/client/actions/certificates.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
       return []
     
   async def __process_get_resources_key_vaults(self, account, *args, **kwargs):    
     try:
       client = KeyVaultManagementClient(credential= self.get_cloud_client().get_tenant_credential(tenant= self.get_cloud_client().get_tenant_id(tenant= account, is_account= True)), subscription_id= self.get_cloud_client().get_account_id(account= account))
     
 
-      return { self.get_cloud_client().get_resource_id_from_resource(resource= kv):kv for kv in self.get_cloud_client().sdk_request(
+      return { self.get_cloud_client().get_resource_id(resource= kv):kv for kv in self.get_cloud_client().sdk_request(
           tenant= self.get_cloud_client().get_tenant_id(tenant= account, is_account= True), 
           lambda_sdk_command=lambda: client.vaults.list()
         )
       }
            
     except Exception as err:
       return {} 
@@ -65,25 +65,25 @@
     return {
         "account": account,
         "data": [ 
           # self.get_common().helper_type().dictionary().merge_dictionary([
           #   {},
           #   await self.get_base_return_data(
           #     account= self.get_cloud_client().serialize_resource(resource= account),
-          #     resource_id= self.get_cloud_client().get_resource_id_from_resource(resource= item),
+          #     resource_id= self.get_cloud_client().get_resource_id(resource= item),
           #     resource= item,
           #     region= self.get_cloud_client().get_resource_location(resource= item),
           #     resource_groups= [self.get_cloud_client().get_resource_group_from_resource(resource= item)],
           #   ),
           #   {
-          #     "extra_resource": self.get_cloud_client().serialize_resource(tasks["resource"].result().get(self.get_cloud_client().get_resource_id_from_resource(resource= item))),
-          #     "extra_availability_set": tasks["availability_sets"].result().get(self.get_cloud_client().get_resource_id_from_resource(resource= item)),
-          #     "extra_nics": tasks["nics"].result().get(self.get_cloud_client().get_resource_id_from_resource(resource= item)),
+          #     "extra_resource": self.get_cloud_client().serialize_resource(tasks["resource"].result().get(self.get_cloud_client().get_resource_id(resource= item))),
+          #     "extra_availability_set": tasks["availability_sets"].result().get(self.get_cloud_client().get_resource_id(resource= item)),
+          #     "extra_nics": tasks["nics"].result().get(self.get_cloud_client().get_resource_id(resource= item)),
           #     "extra_load_balancers": await self._process_account_data_get_vm_load_balancers(
-          #       vm_nics= tasks["nics"].result().get(self.get_cloud_client().get_resource_id_from_resource(resource= item)),
+          #       vm_nics= tasks["nics"].result().get(self.get_cloud_client().get_resource_id(resource= item)),
           #       load_balancers_by_nics = tasks["load_balancers"].result()
           #     ),
           #   },
           # ]) for item in self.get_cloud_client().sdk_request(
           #  tenant= self.get_cloud_client().get_tenant_id(tenant= account, is_account= True), 
           #  lambda_sdk_command=lambda: client.virtual_machines.list_all()
           # )
```

### Comparing `threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/azure/client/actions/cloudstorage.py` & `threemystic_cloud_data_client-0.1.22/threemystic_cloud_data_client/cloud_providers/azure/client/actions/cloudstorage.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,17 +10,15 @@
       data_action="cloudstorage", 
       logger_name= "cloud_data_client_azure_client_action_cloudstorage",
       *args, **kwargs)
   
   
   async def _process_account_data_storage_size(self, client, account, storage_account, **kwargs):
       try:
-        
-        storage_account_name= self.get_cloud_client().get_resource_name_from_resource(resource= storage_account)
-        storage_account_id= self.get_cloud_client().get_resource_id_from_resource(resource= storage_account)
+        storage_account_id= self.get_cloud_client().get_resource_id(resource= storage_account)
         storage_size = self.get_cloud_client().sdk_request(
           tenant= self.get_cloud_client().get_tenant_id(tenant= account, is_account= True), 
           lambda_sdk_command=lambda: client.metrics.list(
             resource_uri= storage_account_id,
             timespan= f'{self.get_common().helper_type().datetime().get_iso_datetime(dt= (self.get_data_start() - self.get_common().helper_type().datetime().time_delta(days= 1)))}/{self.get_common().helper_type().datetime().get_iso_datetime(dt= self.get_data_start())}',
             interval= "PT1H",
             metricnames= "UsedCapacity"
@@ -32,15 +30,15 @@
         for interval_value in storage_size.value:
           for ts in interval_value.timeseries:
             for data in ts.data:
               if data.average is not None:
                 sum_storage += Decimal(data.average)
               interval_count += 1
         
-        return Decimal(sum_storage/interval_count).quantize(Decimal('0'), ROUND_HALF_UP) 
+        return Decimal(sum_storage/interval_count).quantize(Decimal('0'), ROUND_HALF_UP)
       except Exception as err:
         return None
         
   async def _process_account_data_blob_containers(self, client:StorageManagementClient, account, storage_account, **kwargs):
       try:
         resource_group= self.get_cloud_client().get_resource_group_from_resource(resource= storage_account)
         storage_account_name= self.get_cloud_client().get_resource_name_from_resource(resource= storage_account)
@@ -79,15 +77,15 @@
       
     return {
         "account": account,
         "data": [ self.get_common().helper_type().dictionary().merge_dictionary([
           {},
           await self.get_base_return_data(
             account= self.get_cloud_client().serialize_resource(resource= account),
-            resource_id= self.get_cloud_client().get_resource_id_from_resource(resource= item.get("container") if item.get("container") is not None else item.get("storage_account")),
+            resource_id= self.get_cloud_client().get_resource_id(resource= item.get("container") if item.get("container") is not None else item.get("storage_account")),
             resource = item.get("container"),
             region= self.get_cloud_client().get_resource_location(resource= item.get("storage_account")),
             resource_groups= [self.get_cloud_client().get_resource_group_from_resource(resource= item.get("storage_account"))],
           ),
           {
             "extra_storage_account": item.get("storage_account")
           },
```

### Comparing `threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/azure/client/actions/database.py` & `threemystic_cloud_data_client-0.1.22/threemystic_cloud_data_client/cloud_providers/azure/client/actions/database.py`

 * *Files 1% similar despite different names*

```diff
@@ -246,15 +246,15 @@
       if db_data.result() is None:
         continue
       for item in db_data.result():
         return_data["data"].append( self.get_common().helper_type().dictionary().merge_dictionary([
             {},
             await self.get_base_return_data(
               account= self.get_cloud_client().serialize_resource(resource= account),
-              resource_id= self.get_cloud_client().get_resource_id_from_resource(resource= item.get("resource")),
+              resource_id= self.get_cloud_client().get_resource_id(resource= item.get("resource")),
               resource= item.get("resource"),
               region= self.get_cloud_client().get_resource_location(resource= item.get("resource")),
               resource_groups= [self.get_cloud_client().get_resource_group_from_resource(resource= item.get("resource"))],
             ),
             item.get("extra"),
           ]))
```

### Comparing `threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/azure/client/actions/datawarehouse.py` & `threemystic_cloud_data_client-0.1.22/threemystic_cloud_data_client/cloud_providers/azure/client/actions/datawarehouse.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     return {
         "account": account,
         "data": [
            self.get_common().helper_type().dictionary().merge_dictionary([
             {},
             await self.get_base_return_data(
               account= self.get_cloud_client().serialize_resource(resource= account),
-              resource_id= self.get_cloud_client().get_resource_id_from_resource(resource= item),
+              resource_id= self.get_cloud_client().get_resource_id(resource= item),
               resource= item,
               region= self.get_cloud_client().get_resource_location(resource= item),
               resource_groups= [self.get_cloud_client().get_resource_group_from_resource(resource= item)],
             ),
             {
               "extra_sql_pools": [
                 self.get_cloud_client().serialize_resource(resource= pool)
```

### Comparing `threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/azure/client/actions/dns.py` & `threemystic_cloud_data_client-0.1.22/threemystic_cloud_data_client/cloud_providers/azure/client/actions/dns.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     super().__init__(
       data_action="dns", 
       logger_name= "cloud_data_client_azure_client_action_dns",
       *args, **kwargs)
   
   async def __process_get_resources_public(self, client, account, *args, **kwargs):    
     try:      
-      return { self.get_cloud_client().get_resource_id_from_resource(resource= dns):dns for dns in self.get_cloud_client().sdk_request(
+      return { self.get_cloud_client().get_resource_id(resource= dns):dns for dns in self.get_cloud_client().sdk_request(
           tenant= self.get_cloud_client().get_tenant_id(tenant= account, is_account= True), 
           lambda_sdk_command=lambda: client.zones.list()
         )
       }
            
     except Exception as err:
       self.get_common().get_logger().exception(
@@ -45,15 +45,15 @@
           "exception": err
         }
       )
       return []
   
   async def __process_get_resources_private_dns(self, client, account, *args, **kwargs):    
     try:      
-      return { self.get_cloud_client().get_resource_id_from_resource(resource= dns):dns for dns in self.get_cloud_client().sdk_request(
+      return { self.get_cloud_client().get_resource_id(resource= dns):dns for dns in self.get_cloud_client().sdk_request(
           tenant= self.get_cloud_client().get_tenant_id(tenant= account, is_account= True), 
           lambda_sdk_command=lambda: client.private_zones.list()
         )
       }
            
     except Exception as err:
       self.get_common().get_logger().exception(
@@ -97,15 +97,15 @@
         }
       )
       return []
   
   async def __process_get_resources_resource_dns(self, account, *args, **kwargs):    
     resource_client = ResourceManagementClient(credential= self.get_cloud_client().get_tenant_credential(tenant= self.get_cloud_client().get_tenant_id(tenant= account, is_account= True)), subscription_id= self.get_cloud_client().get_account_id(account= account))
     try:
-        return {self.get_cloud_client().get_resource_id_from_resource(resource= resource): resource for resource in self.get_cloud_client().sdk_request(
+        return {self.get_cloud_client().get_resource_id(resource= resource): resource for resource in self.get_cloud_client().sdk_request(
            tenant= self.get_cloud_client().get_tenant_id(tenant= account, is_account= True), 
            lambda_sdk_command=lambda: resource_client.resources.list(filter="resourceType eq 'Microsoft.Network/privateDnsZones' or resourceType eq 'Microsoft.Network/dnsZones'", expand="createdTime,changedTime,provisioningState")
           )
         }
     except Exception as err:
       self.get_common().get_logger().exception(
         msg= f"__process_get_resources_resource_dns: {err}",
@@ -192,15 +192,15 @@
     return {
       "account": account,
       "data": [
           self.get_common().helper_type().dictionary().merge_dictionary([
           {},
           await self.get_base_return_data(
             account= self.get_cloud_client().serialize_resource(resource= account),
-            resource_id= self.get_cloud_client().get_resource_id_from_resource(resource= tasks_data[f'{id};item'].result()),
+            resource_id= self.get_cloud_client().get_resource_id(resource= tasks_data[f'{id};item'].result()),
             resource= tasks_data[f'{id};item'].result(),
             region= self.get_cloud_client().get_resource_location(resource= tasks_data[f'{id};item'].result()),
             resource_groups= [self.get_cloud_client().get_resource_group_from_resource(resource= tasks_data[f'{id};item'].result())],
           ),
           {
             "extra_record_sets": [ self.get_cloud_client().serialize_resource(resource= zone) for zone in tasks_data[f'{id};record_sets'].result() ] if tasks_data[f'{id};record_sets'].result() is not None else None,
             "extra_vnet_link": [ self.get_cloud_client().serialize_resource(resource= link) for link in tasks_data[f'{id};network'].result() ] if self.get_common().helper_type().string().set_case(string_value= raw_resource.type, case= "lower") == "microsoft.network/privatednszones" and tasks_data[f'{id};network'].result() is not None else None,
```

### Comparing `threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/azure/client/actions/memorydb.py` & `threemystic_cloud_data_client-0.1.22/threemystic_cloud_data_client/cloud_providers/azure/client/actions/memorydb.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     return {
         "account": account,
         "data": [
            self.get_common().helper_type().dictionary().merge_dictionary([
             {},
             await self.get_base_return_data(
               account= self.get_cloud_client().serialize_resource(resource= account),
-              resource_id= self.get_cloud_client().get_resource_id_from_resource(resource= item),
+              resource_id= self.get_cloud_client().get_resource_id(resource= item),
               resource= item,
               region= self.get_cloud_client().get_resource_location(resource= item),
               resource_groups= [self.get_cloud_client().get_resource_group_from_resource(resource= item)],
             ),
             {
               
             },
```

### Comparing `threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/azure/client/actions/secrets.py` & `threemystic_cloud_data_client-0.1.22/threemystic_cloud_data_client/cloud_providers/azure/client/actions/secrets.py`

 * *Files 8% similar despite different names*

```diff
@@ -57,15 +57,15 @@
       return []
     
   async def __process_get_resources_key_vaults(self, account, *args, **kwargs):    
     try:
       client = KeyVaultManagementClient(credential= self.get_cloud_client().get_tenant_credential(tenant= self.get_cloud_client().get_tenant_id(tenant= account, is_account= True)), subscription_id= self.get_cloud_client().get_account_id(account= account))
     
 
-      return { self.get_cloud_client().get_resource_id_from_resource(resource= kv):kv for kv in self.get_cloud_client().sdk_request(
+      return { self.get_cloud_client().get_resource_id(resource= kv):kv for kv in self.get_cloud_client().sdk_request(
           tenant= self.get_cloud_client().get_tenant_id(tenant= account, is_account= True), 
           lambda_sdk_command=lambda: client.vaults.list()
         )
       }
            
     except Exception as err:
       return {} 
@@ -84,25 +84,25 @@
     return {
         "account": account,
         "data": [
           #  self.get_common().helper_type().dictionary().merge_dictionary([
           #   {},
           #   await self.get_base_return_data(
           #     account= self.get_cloud_client().serialize_resource(resource= account),
-          #     resource_id= self.get_cloud_client().get_resource_id_from_resource(resource= item),
+          #     resource_id= self.get_cloud_client().get_resource_id(resource= item),
           #     resource= item,
           #     region= self.get_cloud_client().get_resource_location(resource= item),
           #     resource_groups= [self.get_cloud_client().get_resource_group_from_resource(resource= item)],
           #   ),
           #   {
-          #     "extra_resource": self.get_cloud_client().serialize_resource(tasks["resource"].result().get(self.get_cloud_client().get_resource_id_from_resource(resource= item))),
-          #     "extra_availability_set": tasks["availability_sets"].result().get(self.get_cloud_client().get_resource_id_from_resource(resource= item)),
-          #     "extra_nics": tasks["nics"].result().get(self.get_cloud_client().get_resource_id_from_resource(resource= item)),
+          #     "extra_resource": self.get_cloud_client().serialize_resource(tasks["resource"].result().get(self.get_cloud_client().get_resource_id(resource= item))),
+          #     "extra_availability_set": tasks["availability_sets"].result().get(self.get_cloud_client().get_resource_id(resource= item)),
+          #     "extra_nics": tasks["nics"].result().get(self.get_cloud_client().get_resource_id(resource= item)),
           #     "extra_load_balancers": await self._process_account_data_get_vm_load_balancers(
-          #       vm_nics= tasks["nics"].result().get(self.get_cloud_client().get_resource_id_from_resource(resource= item)),
+          #       vm_nics= tasks["nics"].result().get(self.get_cloud_client().get_resource_id(resource= item)),
           #       load_balancers_by_nics = tasks["load_balancers"].result()
           #     ),
           #   },
           # ]) for item in self.get_cloud_client().sdk_request(
           #  tenant= self.get_cloud_client().get_tenant_id(tenant= account, is_account= True), 
           #  lambda_sdk_command=lambda: client.virtual_machines.list_all()
           # )
```

### Comparing `threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/azure/client/actions/storage.py` & `threemystic_cloud_data_client-0.1.22/threemystic_cloud_data_client/cloud_providers/azure/client/actions/storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -190,23 +190,23 @@
     return return_data
 
   async def __get_account_disk_merged(self, account, cost_by_resource, item, loop, *args, **kwarg):
     return self.get_common().helper_type().dictionary().merge_dictionary([
         {},
         await self.get_base_return_data(
           account= self.get_cloud_client().serialize_resource(resource= account),
-          resource_id= self.get_cloud_client().get_resource_id_from_resource(resource= item),
+          resource_id= self.get_cloud_client().get_resource_id(resource= item),
           resource= item,
           region= self.get_cloud_client().get_resource_location(resource= item),
           resource_groups= [self.get_cloud_client().get_resource_group_from_resource(resource= item)],
         ),         
         {
           "extra_attached_devices": (await self.__get_attached_devices(account=account, disk= item, loop= loop)),
           "extra_resource_cost": {
-            "period": cost_by_resource_results.get(self.get_cloud_client().get_resource_id_from_resource(resource= item)) for period, cost_by_resource_results in cost_by_resource.items()
+            "period": cost_by_resource_results.get(self.get_cloud_client().get_resource_id(resource= item)) for period, cost_by_resource_results in cost_by_resource.items()
           }
         }])
 
   def __process_vmss_vm_disks_skip(self, vm: VirtualMachineScaleSetVM, *args, **kwarg):
     if not hasattr(vm, "storage_profile"):
       return True
```

### Comparing `threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vm.py` & `threemystic_cloud_data_client-0.1.22/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vm.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,28 +15,28 @@
   
   
 
   async def __process_get_resources_vm_public_ips(self, account, *args, **kwargs):    
     try:
         client = NetworkManagementClient(credential= self.get_cloud_client().get_tenant_credential(tenant= self.get_cloud_client().get_tenant_id(tenant= account, is_account= True)), subscription_id= self.get_cloud_client().get_account_id(account= account))
 
-        return { self.get_cloud_client().get_resource_id_from_resource(resource= public_ip):public_ip for public_ip in self.get_cloud_client().sdk_request(
+        return { self.get_cloud_client().get_resource_id(resource= public_ip):public_ip for public_ip in self.get_cloud_client().sdk_request(
            tenant= self.get_cloud_client().get_tenant_id(tenant= account, is_account= True), 
            lambda_sdk_command=lambda: client.public_ip_addresses.list_all()
           )
         }
            
     except Exception as err:
       return {} 
 
   async def __process_get_resources_vm_load_balancers(self, account, public_ips, *args, **kwargs):    
     try:
       client = NetworkManagementClient(credential= self.get_cloud_client().get_tenant_credential(tenant= self.get_cloud_client().get_tenant_id(tenant= account, is_account= True)), subscription_id= self.get_cloud_client().get_account_id(account= account))
       return_data = {}
-      load_balancers = {self.get_cloud_client().get_resource_id_from_resource(resource= lb): {"serialized": self.get_cloud_client().serialize_resource(resource= lb), "raw": lb} for lb in self.get_cloud_client().sdk_request(
+      load_balancers = {self.get_cloud_client().get_resource_id(resource= lb): {"serialized": self.get_cloud_client().serialize_resource(resource= lb), "raw": lb} for lb in self.get_cloud_client().sdk_request(
           tenant= self.get_cloud_client().get_tenant_id(tenant= account, is_account= True), 
           lambda_sdk_command=lambda: client.load_balancers.list_all()
         )}
 
       if len(load_balancers) < 1:
         return {}
       
@@ -48,15 +48,15 @@
           continue
         for frontend_ip in lb["raw"].frontend_ip_configurations:
           if frontend_ip.load_balancing_rules is None:
             continue
           for frontend_ip_load_balancing_rule in frontend_ip.load_balancing_rules:
             if frontend_ip_load_balancing_rule is None:
               continue
-            load_balancers_front_end[self.get_cloud_client().get_resource_id_from_resource(resource= frontend_ip_load_balancing_rule)] = self.get_cloud_client().get_resource_id_from_resource(resource= frontend_ip.public_ip_address)
+            load_balancers_front_end[self.get_cloud_client().get_resource_id(resource= frontend_ip_load_balancing_rule)] = self.get_cloud_client().get_resource_id(resource= frontend_ip.public_ip_address)
       
 
       for id_lb, lb in load_balancers.items():
         if lb["raw"].frontend_ip_configurations is None:
           continue
         vm_data = {
           "load_balancer": lb["serialized"],
@@ -70,22 +70,22 @@
             continue
           
           backend_frontend_connector = []
           for backend_address_load_balancing_rule in backend_address_pool.load_balancing_rules:            
             if backend_address_load_balancing_rule is None:
               continue
 
-            if load_balancers_front_end.get(self.get_cloud_client().get_resource_id_from_resource(resource= backend_address_load_balancing_rule)) is None:
+            if load_balancers_front_end.get(self.get_cloud_client().get_resource_id(resource= backend_address_load_balancing_rule)) is None:
               continue
-            backend_frontend_connector.append(load_balancers_front_end.get(self.get_cloud_client().get_resource_id_from_resource(resource= backend_address_load_balancing_rule)))
+            backend_frontend_connector.append(load_balancers_front_end.get(self.get_cloud_client().get_resource_id(resource= backend_address_load_balancing_rule)))
             
           for backend_address in backend_address_pool.load_balancer_backend_addresses:
             if backend_address.network_interface_ip_configuration is not None:
-              if self.get_cloud_client().get_resource_id_from_resource(resource= backend_address.network_interface_ip_configuration) is not None:
-                key = self.get_cloud_client().get_resource_id_from_resource(resource= backend_address.network_interface_ip_configuration)
+              if self.get_cloud_client().get_resource_id(resource= backend_address.network_interface_ip_configuration) is not None:
+                key = self.get_cloud_client().get_resource_id(resource= backend_address.network_interface_ip_configuration)
                 key = key[0:key.rfind("/ipconfigurations/")]
               else:
                 key = backend_address.ip_address
 
               if self.get_common().helper_type().string().is_null_or_whitespace(string_value= key):
                 continue
 
@@ -117,27 +117,27 @@
           if nic.virtual_machine is None:
             continue
           
           nic_data = self.get_common().helper_type().dictionary().merge_dictionary([
             {},
             {
               "extra_public_ips": [
-                self.get_cloud_client().serialize_resource(resource= public_ips[self.get_cloud_client().get_resource_id_from_resource(resource= ip_config.public_ip_address)])
-                for ip_config in nic.ip_configurations if self.get_cloud_client().get_resource_id_from_resource(resource= ip_config.public_ip_address) is not None]
+                self.get_cloud_client().serialize_resource(resource= public_ips[self.get_cloud_client().get_resource_id(resource= ip_config.public_ip_address)])
+                for ip_config in nic.ip_configurations if self.get_cloud_client().get_resource_id(resource= ip_config.public_ip_address) is not None]
             },
             self.get_cloud_client().serialize_resource(resource= nic)
           ])
-          if return_data.get( self.get_cloud_client().get_resource_id_from_resource(resource= nic.virtual_machine)) is not None:
-            return_data.get( self.get_cloud_client().get_resource_id_from_resource(resource= nic.virtual_machine)).append(
+          if return_data.get( self.get_cloud_client().get_resource_id(resource= nic.virtual_machine)) is not None:
+            return_data.get( self.get_cloud_client().get_resource_id(resource= nic.virtual_machine)).append(
               nic_data
             )
             continue
           
 
-          return_data[self.get_cloud_client().get_resource_id_from_resource(resource= nic.virtual_machine)] = [
+          return_data[self.get_cloud_client().get_resource_id(resource= nic.virtual_machine)] = [
             nic_data
           ]
       
       return return_data
           
         
            
@@ -149,39 +149,39 @@
       return_data = {}
 
       for availability_set in  self.get_cloud_client().sdk_request(
           tenant= self.get_cloud_client().get_tenant_id(tenant= account, is_account= True), 
           lambda_sdk_command=lambda: client.availability_sets.list_by_subscription()
         ):
           for vm in availability_set.virtual_machines:
-            return_data[self.get_cloud_client().get_resource_id_from_resource(resource= vm)] = self.get_cloud_client().serialize_resource(resource= availability_set)
+            return_data[self.get_cloud_client().get_resource_id(resource= vm)] = self.get_cloud_client().serialize_resource(resource= availability_set)
       
       return return_data
     except Exception as err:
       return {}
     
   async def __process_get_resources_vm(self, account, *args, **kwargs):
     resource_client = ResourceManagementClient(credential= self.get_cloud_client().get_tenant_credential(tenant= self.get_cloud_client().get_tenant_id(tenant= account, is_account= True)), subscription_id= self.get_cloud_client().get_account_id(account= account))
     try:
-        return {self.get_cloud_client().get_resource_id_from_resource(resource= resource): resource for resource in self.get_cloud_client().sdk_request(
+        return {self.get_cloud_client().get_resource_id(resource= resource): resource for resource in self.get_cloud_client().sdk_request(
            tenant= self.get_cloud_client().get_tenant_id(tenant= account, is_account= True), 
            lambda_sdk_command=lambda: resource_client.resources.list(filter="resourceType eq 'Microsoft.Compute/virtualMachines'", expand="createdTime,changedTime,provisioningState")
           )
         }
     except:
         return {}
 
   async def _process_account_data_get_vm_load_balancers(self, vm_nics, load_balancers_by_nics, *args, **kwargs):
     return_load_balancers = []
     
     for nic in vm_nics:
-      if load_balancers_by_nics.get(self.get_cloud_client().get_resource_id_from_resource(resource= nic)) is None:
+      if load_balancers_by_nics.get(self.get_cloud_client().get_resource_id(resource= nic)) is None:
         continue
         
-      return_load_balancers += (load_balancers_by_nics.get(self.get_cloud_client().get_resource_id_from_resource(resource= nic)))
+      return_load_balancers += (load_balancers_by_nics.get(self.get_cloud_client().get_resource_id(resource= nic)))
       # I might look into the whole private IP agress later, the issue is I have to validate networks
       
     
     return return_load_balancers
   
   async def _process_account_data(self, account, loop, *args, **kwargs):
     client = ComputeManagementClient(credential= self.get_cloud_client().get_tenant_credential(tenant= self.get_cloud_client().get_tenant_id(tenant= account, is_account= True)), subscription_id= self.get_cloud_client().get_account_id(account= account))
@@ -197,25 +197,25 @@
 
     return {
         "account": account,
         "data": [ self.get_common().helper_type().dictionary().merge_dictionary([
             {},
             await self.get_base_return_data(
               account= self.get_cloud_client().serialize_resource(resource= account),
-              resource_id= self.get_cloud_client().get_resource_id_from_resource(resource= item),
+              resource_id= self.get_cloud_client().get_resource_id(resource= item),
               resource= item,
               region= self.get_cloud_client().get_resource_location(resource= item),
               resource_groups= [self.get_cloud_client().get_resource_group_from_resource(resource= item)],
             ),
             {
-              "extra_resource": self.get_cloud_client().serialize_resource(tasks["resource"].result().get(self.get_cloud_client().get_resource_id_from_resource(resource= item))),
-              "extra_availability_set": tasks["availability_sets"].result().get(self.get_cloud_client().get_resource_id_from_resource(resource= item)),
-              "extra_nics": tasks["nics"].result().get(self.get_cloud_client().get_resource_id_from_resource(resource= item)),
+              "extra_resource": self.get_cloud_client().serialize_resource(tasks["resource"].result().get(self.get_cloud_client().get_resource_id(resource= item))),
+              "extra_availability_set": tasks["availability_sets"].result().get(self.get_cloud_client().get_resource_id(resource= item)),
+              "extra_nics": tasks["nics"].result().get(self.get_cloud_client().get_resource_id(resource= item)),
               "extra_load_balancers": await self._process_account_data_get_vm_load_balancers(
-                vm_nics= tasks["nics"].result().get(self.get_cloud_client().get_resource_id_from_resource(resource= item)),
+                vm_nics= tasks["nics"].result().get(self.get_cloud_client().get_resource_id(resource= item)),
                 load_balancers_by_nics = tasks["load_balancers"].result()
               ),
             },
           ]) for item in self.get_cloud_client().sdk_request(
            tenant= self.get_cloud_client().get_tenant_id(tenant= account, is_account= True), 
            lambda_sdk_command=lambda: client.virtual_machines.list_all()
           )
```

### Comparing `threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vmimage.py` & `threemystic_cloud_data_client-0.1.22/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vmimage.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,15 +24,15 @@
       for image in self.get_cloud_client().sdk_request(
           tenant= self.get_cloud_client().get_tenant_id(tenant= account, is_account= True), 
           lambda_sdk_command=lambda: client.gallery_images.list_by_gallery(
             resource_group_name= self.get_cloud_client().get_resource_group_from_resource(resource= gallery),
             gallery_name= gallery.name
           )
         ):
-        image_gallery_images[self.get_cloud_client().get_resource_id_from_resource(resource= gallery)] = self.get_common().helper_type().dictionary().merge_dictionary([
+        image_gallery_images[self.get_cloud_client().get_resource_id(resource= gallery)] = self.get_common().helper_type().dictionary().merge_dictionary([
           {},
           {"extra_versions": [
             self.get_cloud_client().serialize_resource(resource= image_version) 
             for image_version in self.get_cloud_client().sdk_request(
             tenant= self.get_cloud_client().get_tenant_id(tenant= account, is_account= True), 
             lambda_sdk_command=lambda: client.gallery_image_versions.list_by_gallery_image(
                 resource_group_name= self.get_cloud_client().get_resource_group_from_resource(resource= gallery),
@@ -49,16 +49,16 @@
     return {
       "account": account,
       "data": [
           self.get_common().helper_type().dictionary().merge_dictionary([
           {},
           await self.get_base_return_data(
             account= self.get_cloud_client().serialize_resource(resource= account),
-            resource_id= self.get_cloud_client().get_resource_id_from_resource(resource= item),
+            resource_id= self.get_cloud_client().get_resource_id(resource= item),
             resource= item,
             region= self.get_cloud_client().get_resource_location(resource= item),
             resource_groups= [self.get_cloud_client().get_resource_group_from_resource(resource= item)],
           ),
-          image_gallery_images[self.get_cloud_client().get_resource_id_from_resource(resource= item)],
+          image_gallery_images[self.get_cloud_client().get_resource_id(resource= item)],
         ]) for item in image_gallery_images
       ]
     }
```

### Comparing `threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vmss.py` & `threemystic_cloud_data_client-0.1.22/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vmss.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
       *args, **kwargs)
   
   
     
   async def __process_get_resources_vmss(self, account, *args, **kwargs):
     resource_client = ResourceManagementClient(credential= self.get_cloud_client().get_tenant_credential(tenant= self.get_cloud_client().get_tenant_id(tenant= account, is_account= True)), subscription_id= self.get_cloud_client().get_account_id(account= account))
     try:
-      return { self.get_cloud_client().get_resource_id_from_resource(resource= resource): resource for resource in self.get_cloud_client().sdk_request(
+      return { self.get_cloud_client().get_resource_id(resource= resource): resource for resource in self.get_cloud_client().sdk_request(
           tenant= self.get_cloud_client().get_tenant_id(tenant= account, is_account= True), 
           lambda_sdk_command=lambda: resource_client.resources.list(filter="resourceType eq 'Microsoft.Compute/virtualMachineScaleSets'", expand="createdTime,changedTime,provisioningState")
         )
       }
     except:
       return []
         
@@ -34,21 +34,21 @@
 
     return {
       "account": account,
       "data": [ self.get_common().helper_type().dictionary().merge_dictionary([
           {},
           await self.get_base_return_data(
             account= self.get_cloud_client().serialize_resource(resource= account),
-            resource_id= self.get_cloud_client().get_resource_id_from_resource(resource= item),
+            resource_id= self.get_cloud_client().get_resource_id(resource= item),
             resource= item,
             region= self.get_cloud_client().get_resource_location(resource= item),
             resource_groups= [self.get_cloud_client().get_resource_group_from_resource(resource= item)],
           ),
           {
-            "extra_resource": self.get_cloud_client().serialize_resource(tasks["resource"].result().get(self.get_cloud_client().get_resource_id_from_resource(resource= item))),
+            "extra_resource": self.get_cloud_client().serialize_resource(tasks["resource"].result().get(self.get_cloud_client().get_resource_id(resource= item))),
             "extra_vmss_vms": [ self.get_cloud_client().serialize_resource(vm) for vm in client.virtual_machine_scale_set_vms.list(resource_group_name= self.get_cloud_client().get_resource_group_from_resource(item), virtual_machine_scale_set_name= item.name) ]
           },
           ]) for item in self.get_cloud_client().sdk_request(
           tenant= self.get_cloud_client().get_tenant_id(tenant= account, is_account= True), 
           lambda_sdk_command=lambda: client.virtual_machine_scale_sets.list_all()
         )
       ]
```

### Comparing `threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/azure/client/actions/base_class/base.py` & `threemystic_cloud_data_client-0.1.22/threemystic_cloud_data_client/cloud_providers/azure/client/actions/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/azure/config/step_1.py` & `threemystic_cloud_data_client-0.1.22/threemystic_cloud_data_client/cloud_providers/azure/config/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/base_class/base.py` & `threemystic_cloud_data_client-0.1.22/threemystic_cloud_data_client/cloud_providers/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/base_class/base_client.py` & `threemystic_cloud_data_client-0.1.22/threemystic_cloud_data_client/cloud_providers/base_class/base_client.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/base_class/base_data.py` & `threemystic_cloud_data_client-0.1.22/threemystic_cloud_data_client/cloud_providers/base_class/base_data.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/general/__init__.py` & `threemystic_cloud_data_client-0.1.22/threemystic_cloud_data_client/cloud_providers/general/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/general/config/step_1.py` & `threemystic_cloud_data_client-0.1.22/threemystic_cloud_data_client/cloud_providers/general/config/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.21/threemystic_cloud_data_client/cloud_providers/general/config/step_2.py` & `threemystic_cloud_data_client-0.1.22/threemystic_cloud_data_client/cloud_providers/general/config/step_2.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.21/.gitignore` & `threemystic_cloud_data_client-0.1.22/.gitignore`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.21/LICENSE` & `threemystic_cloud_data_client-0.1.22/LICENSE`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.21/README.md` & `threemystic_cloud_data_client-0.1.22/README.md`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.21/hatch.toml` & `threemystic_cloud_data_client-0.1.22/hatch.toml`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.21/pyproject.toml` & `threemystic_cloud_data_client-0.1.22/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
   "colorama; platform_system == 'Windows'",
   "threemystic-common >= 0.1.15",
-  "threemystic-cloud-client >= 0.1.39",
+  "threemystic-cloud-client >= 0.1.40",
   "typing-extensions >= 4.4.0",
   "asyncio >= 3.4.3",
   "tqdm >= 4.65.0",
   "azure-mgmt-cosmosdb >= 9",
   "azure-mgmt-costmanagement >= 4",
   "azure-mgmt-dns >= 8",
   "azure-mgmt-keyvault >= 10",
```

### Comparing `threemystic_cloud_data_client-0.1.21/PKG-INFO` & `threemystic_cloud_data_client-0.1.22/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threemystic-cloud-data-client
-Version: 0.1.21
+Version: 0.1.22
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
-Requires-Dist: threemystic-cloud-client>=0.1.39
+Requires-Dist: threemystic-cloud-client>=0.1.40
 Requires-Dist: threemystic-common>=0.1.15
 Requires-Dist: tqdm>=4.65.0
 Requires-Dist: typing-extensions>=4.4.0
 Description-Content-Type: text/markdown
 
 # 3mystic_cloud_data_client
 A set of scripts to help uniformly pull data from the cloud providers for various resources.
```

