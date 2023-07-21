# Comparing `tmp/tencentcloud-sdk-python-partners-3.0.939.tar.gz` & `tmp/tencentcloud-sdk-python-partners-3.0.940.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-partners-3.0.939.tar", last modified: Thu Jul 20 00:28:58 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-partners-3.0.940.tar", last modified: Fri Jul 21 00:47:20 2023, max compression
```

## Comparing `tencentcloud-sdk-python-partners-3.0.939.tar` & `tencentcloud-sdk-python-partners-3.0.940.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 00:28:58.000000 tencentcloud-sdk-python-partners-3.0.939/
--rw-r--r--   0 root         (0) root         (0)     1016 2023-07-20 00:28:57.000000 tencentcloud-sdk-python-partners-3.0.939/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 00:28:58.000000 tencentcloud-sdk-python-partners-3.0.939/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 00:28:58.000000 tencentcloud-sdk-python-partners-3.0.939/tencentcloud/partners/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 00:28:58.000000 tencentcloud-sdk-python-partners-3.0.939/tencentcloud/partners/v20180321/
--rw-r--r--   0 root         (0) root         (0)    19410 2023-07-20 00:28:57.000000 tencentcloud-sdk-python-partners-3.0.939/tencentcloud/partners/v20180321/partners_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-20 00:28:57.000000 tencentcloud-sdk-python-partners-3.0.939/tencentcloud/partners/v20180321/__init__.py
--rw-r--r--   0 root         (0) root         (0)      885 2023-07-20 00:28:57.000000 tencentcloud-sdk-python-partners-3.0.939/tencentcloud/partners/v20180321/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   107514 2023-07-20 00:28:57.000000 tencentcloud-sdk-python-partners-3.0.939/tencentcloud/partners/v20180321/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-20 00:28:57.000000 tencentcloud-sdk-python-partners-3.0.939/tencentcloud/partners/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-20 00:28:57.000000 tencentcloud-sdk-python-partners-3.0.939/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-20 00:28:58.000000 tencentcloud-sdk-python-partners-3.0.939/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1684 2023-07-20 00:28:58.000000 tencentcloud-sdk-python-partners-3.0.939/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      752 2023-07-20 00:28:57.000000 tencentcloud-sdk-python-partners-3.0.939/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 00:28:58.000000 tencentcloud-sdk-python-partners-3.0.939/tencentcloud_sdk_python_partners.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 00:28:58.000000 tencentcloud-sdk-python-partners-3.0.939/tencentcloud_sdk_python_partners.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      495 2023-07-20 00:28:58.000000 tencentcloud-sdk-python-partners-3.0.939/tencentcloud_sdk_python_partners.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1684 2023-07-20 00:28:58.000000 tencentcloud-sdk-python-partners-3.0.939/tencentcloud_sdk_python_partners.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-20 00:28:58.000000 tencentcloud-sdk-python-partners-3.0.939/tencentcloud_sdk_python_partners.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:47:20.000000 tencentcloud-sdk-python-partners-3.0.940/
+-rw-r--r--   0 root         (0) root         (0)     1016 2023-07-21 00:47:20.000000 tencentcloud-sdk-python-partners-3.0.940/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:47:20.000000 tencentcloud-sdk-python-partners-3.0.940/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:47:20.000000 tencentcloud-sdk-python-partners-3.0.940/tencentcloud/partners/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:47:20.000000 tencentcloud-sdk-python-partners-3.0.940/tencentcloud/partners/v20180321/
+-rw-r--r--   0 root         (0) root         (0)    19410 2023-07-21 00:47:20.000000 tencentcloud-sdk-python-partners-3.0.940/tencentcloud/partners/v20180321/partners_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 00:47:20.000000 tencentcloud-sdk-python-partners-3.0.940/tencentcloud/partners/v20180321/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      885 2023-07-21 00:47:20.000000 tencentcloud-sdk-python-partners-3.0.940/tencentcloud/partners/v20180321/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   109523 2023-07-21 00:47:20.000000 tencentcloud-sdk-python-partners-3.0.940/tencentcloud/partners/v20180321/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 00:47:20.000000 tencentcloud-sdk-python-partners-3.0.940/tencentcloud/partners/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-21 00:47:20.000000 tencentcloud-sdk-python-partners-3.0.940/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-21 00:47:20.000000 tencentcloud-sdk-python-partners-3.0.940/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-07-21 00:47:20.000000 tencentcloud-sdk-python-partners-3.0.940/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      752 2023-07-21 00:47:20.000000 tencentcloud-sdk-python-partners-3.0.940/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:47:20.000000 tencentcloud-sdk-python-partners-3.0.940/tencentcloud_sdk_python_partners.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 00:47:20.000000 tencentcloud-sdk-python-partners-3.0.940/tencentcloud_sdk_python_partners.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      495 2023-07-21 00:47:20.000000 tencentcloud-sdk-python-partners-3.0.940/tencentcloud_sdk_python_partners.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-07-21 00:47:20.000000 tencentcloud-sdk-python-partners-3.0.940/tencentcloud_sdk_python_partners.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-21 00:47:20.000000 tencentcloud-sdk-python-partners-3.0.940/tencentcloud_sdk_python_partners.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-partners-3.0.939/setup.py` & `tencentcloud-sdk-python-partners-3.0.940/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-partners-3.0.939/tencentcloud/partners/v20180321/partners_client.py` & `tencentcloud-sdk-python-partners-3.0.940/tencentcloud/partners/v20180321/partners_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-partners-3.0.939/tencentcloud/partners/v20180321/errorcodes.py` & `tencentcloud-sdk-python-partners-3.0.940/tencentcloud/partners/v20180321/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-partners-3.0.939/tencentcloud/partners/v20180321/models.py` & `tencentcloud-sdk-python-partners-3.0.940/tencentcloud/partners/v20180321/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -656,14 +656,17 @@
         :type PaymentMethod: str
         :param _UpdateTime: 订单更新时间
 注意：此字段可能返回 null，表示取不到有效值。
         :type UpdateTime: str
         :param _ResourceIds: 资源id
 注意：此字段可能返回 null，表示取不到有效值。
         :type ResourceIds: list of str
+        :param _RefundMap: 退款单的原订单信息。当前仅 DescribeClientDealsByCache 接口会返回该字段
+注意：此字段可能返回 null，表示取不到有效值。
+        :type RefundMap: list of RefundMap
         """
         self._DealId = None
         self._DealName = None
         self._GoodsCategoryId = None
         self._OwnerUin = None
         self._AppId = None
         self._GoodsNum = None
@@ -686,14 +689,15 @@
         self._PayerMode = None
         self._ActivityId = None
         self._OverdueTime = None
         self._ProductInfo = None
         self._PaymentMethod = None
         self._UpdateTime = None
         self._ResourceIds = None
+        self._RefundMap = None
 
     @property
     def DealId(self):
         return self._DealId
 
     @DealId.setter
     def DealId(self, DealId):
@@ -919,14 +923,22 @@
     def ResourceIds(self):
         return self._ResourceIds
 
     @ResourceIds.setter
     def ResourceIds(self, ResourceIds):
         self._ResourceIds = ResourceIds
 
+    @property
+    def RefundMap(self):
+        return self._RefundMap
+
+    @RefundMap.setter
+    def RefundMap(self, RefundMap):
+        self._RefundMap = RefundMap
+
 
     def _deserialize(self, params):
         self._DealId = params.get("DealId")
         self._DealName = params.get("DealName")
         self._GoodsCategoryId = params.get("GoodsCategoryId")
         self._OwnerUin = params.get("OwnerUin")
         self._AppId = params.get("AppId")
@@ -957,14 +969,20 @@
             for item in params.get("ProductInfo"):
                 obj = ProductInfoElem()
                 obj._deserialize(item)
                 self._ProductInfo.append(obj)
         self._PaymentMethod = params.get("PaymentMethod")
         self._UpdateTime = params.get("UpdateTime")
         self._ResourceIds = params.get("ResourceIds")
+        if params.get("RefundMap") is not None:
+            self._RefundMap = []
+            for item in params.get("RefundMap"):
+                obj = RefundMap()
+                obj._deserialize(item)
+                self._RefundMap.append(obj)
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -3666,14 +3684,61 @@
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class RefundMap(AbstractModel):
+    """退款单关联的原始订单信息
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _DealName: 退款单关联的原始子订单号
+注意：此字段可能返回 null，表示取不到有效值。
+        :type DealName: str
+        :param _RefundAmount: 退款金额，单位分
+注意：此字段可能返回 null，表示取不到有效值。
+        :type RefundAmount: int
+        """
+        self._DealName = None
+        self._RefundAmount = None
+
+    @property
+    def DealName(self):
+        return self._DealName
+
+    @DealName.setter
+    def DealName(self, DealName):
+        self._DealName = DealName
+
+    @property
+    def RefundAmount(self):
+        return self._RefundAmount
+
+    @RefundAmount.setter
+    def RefundAmount(self, RefundAmount):
+        self._RefundAmount = RefundAmount
+
+
+    def _deserialize(self, params):
+        self._DealName = params.get("DealName")
+        self._RefundAmount = params.get("RefundAmount")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
 class RemovePayRelationForClientRequest(AbstractModel):
     """RemovePayRelationForClient请求参数结构体
 
     """
```

### Comparing `tencentcloud-sdk-python-partners-3.0.939/tencentcloud/__init__.py` & `tencentcloud-sdk-python-partners-3.0.940/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.939'
+__version__ = '3.0.940'
```

### Comparing `tencentcloud-sdk-python-partners-3.0.939/PKG-INFO` & `tencentcloud-sdk-python-partners-3.0.940/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-partners
-Version: 3.0.939
+Version: 3.0.940
 Summary: Tencent Cloud Partners SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-partners-3.0.939/README.rst` & `tencentcloud-sdk-python-partners-3.0.940/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-partners-3.0.939/tencentcloud_sdk_python_partners.egg-info/PKG-INFO` & `tencentcloud-sdk-python-partners-3.0.940/tencentcloud_sdk_python_partners.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-partners
-Version: 3.0.939
+Version: 3.0.940
 Summary: Tencent Cloud Partners SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

