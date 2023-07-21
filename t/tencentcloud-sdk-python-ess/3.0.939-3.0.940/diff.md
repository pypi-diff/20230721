# Comparing `tmp/tencentcloud-sdk-python-ess-3.0.939.tar.gz` & `tmp/tencentcloud-sdk-python-ess-3.0.940.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ess-3.0.939.tar", last modified: Thu Jul 20 00:24:03 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ess-3.0.940.tar", last modified: Fri Jul 21 00:28:59 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ess-3.0.939.tar` & `tencentcloud-sdk-python-ess-3.0.940.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 00:24:03.000000 tencentcloud-sdk-python-ess-3.0.939/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-20 00:24:03.000000 tencentcloud-sdk-python-ess-3.0.939/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 00:24:03.000000 tencentcloud-sdk-python-ess-3.0.939/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-20 00:24:03.000000 tencentcloud-sdk-python-ess-3.0.939/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 00:24:03.000000 tencentcloud-sdk-python-ess-3.0.939/tencentcloud/ess/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 00:24:03.000000 tencentcloud-sdk-python-ess-3.0.939/tencentcloud/ess/v20201111/
--rw-r--r--   0 root         (0) root         (0)    62054 2023-07-20 00:24:03.000000 tencentcloud-sdk-python-ess-3.0.939/tencentcloud/ess/v20201111/ess_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-20 00:24:03.000000 tencentcloud-sdk-python-ess-3.0.939/tencentcloud/ess/v20201111/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25058 2023-07-20 00:24:03.000000 tencentcloud-sdk-python-ess-3.0.939/tencentcloud/ess/v20201111/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   431541 2023-07-20 00:24:03.000000 tencentcloud-sdk-python-ess-3.0.939/tencentcloud/ess/v20201111/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-20 00:24:03.000000 tencentcloud-sdk-python-ess-3.0.939/tencentcloud/ess/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-20 00:24:03.000000 tencentcloud-sdk-python-ess-3.0.939/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 00:24:03.000000 tencentcloud-sdk-python-ess-3.0.939/tencentcloud_sdk_python_ess.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 00:24:03.000000 tencentcloud-sdk-python-ess-3.0.939/tencentcloud_sdk_python_ess.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-20 00:24:03.000000 tencentcloud-sdk-python-ess-3.0.939/tencentcloud_sdk_python_ess.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-20 00:24:03.000000 tencentcloud-sdk-python-ess-3.0.939/tencentcloud_sdk_python_ess.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-20 00:24:03.000000 tencentcloud-sdk-python-ess-3.0.939/tencentcloud_sdk_python_ess.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-20 00:24:03.000000 tencentcloud-sdk-python-ess-3.0.939/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-20 00:24:03.000000 tencentcloud-sdk-python-ess-3.0.939/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:28:59.000000 tencentcloud-sdk-python-ess-3.0.940/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-21 00:28:59.000000 tencentcloud-sdk-python-ess-3.0.940/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:28:59.000000 tencentcloud-sdk-python-ess-3.0.940/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-21 00:28:59.000000 tencentcloud-sdk-python-ess-3.0.940/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:28:59.000000 tencentcloud-sdk-python-ess-3.0.940/tencentcloud/ess/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:28:59.000000 tencentcloud-sdk-python-ess-3.0.940/tencentcloud/ess/v20201111/
+-rw-r--r--   0 root         (0) root         (0)    62054 2023-07-21 00:28:59.000000 tencentcloud-sdk-python-ess-3.0.940/tencentcloud/ess/v20201111/ess_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 00:28:59.000000 tencentcloud-sdk-python-ess-3.0.940/tencentcloud/ess/v20201111/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25058 2023-07-21 00:28:59.000000 tencentcloud-sdk-python-ess-3.0.940/tencentcloud/ess/v20201111/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   432941 2023-07-21 00:28:59.000000 tencentcloud-sdk-python-ess-3.0.940/tencentcloud/ess/v20201111/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 00:28:59.000000 tencentcloud-sdk-python-ess-3.0.940/tencentcloud/ess/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-21 00:28:59.000000 tencentcloud-sdk-python-ess-3.0.940/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:28:59.000000 tencentcloud-sdk-python-ess-3.0.940/tencentcloud_sdk_python_ess.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 00:28:59.000000 tencentcloud-sdk-python-ess-3.0.940/tencentcloud_sdk_python_ess.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-21 00:28:59.000000 tencentcloud-sdk-python-ess-3.0.940/tencentcloud_sdk_python_ess.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-21 00:28:59.000000 tencentcloud-sdk-python-ess-3.0.940/tencentcloud_sdk_python_ess.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-21 00:28:59.000000 tencentcloud-sdk-python-ess-3.0.940/tencentcloud_sdk_python_ess.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-21 00:28:59.000000 tencentcloud-sdk-python-ess-3.0.940/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-21 00:28:59.000000 tencentcloud-sdk-python-ess-3.0.940/README.rst
```

### Comparing `tencentcloud-sdk-python-ess-3.0.939/setup.py` & `tencentcloud-sdk-python-ess-3.0.940/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.939/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ess-3.0.940/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ess-3.0.939/tencentcloud/ess/v20201111/ess_client.py` & `tencentcloud-sdk-python-ess-3.0.940/tencentcloud/ess/v20201111/ess_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.939/tencentcloud/ess/v20201111/errorcodes.py` & `tencentcloud-sdk-python-ess-3.0.940/tencentcloud/ess/v20201111/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.939/tencentcloud/ess/v20201111/models.py` & `tencentcloud-sdk-python-ess-3.0.940/tencentcloud/ess/v20201111/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -4944,25 +4944,33 @@
         :type FlowGroupId: str
         :param _PathType: 跳转页面 1: 小程序合同详情 2: 小程序合同列表页 0: 不传, 默认主页
         :type PathType: int
         :param _AutoJumpBack: 是否自动回跳 true：是， false：否。该参数只针对"APP" 类型的签署链接有效
         :type AutoJumpBack: bool
         :param _Agent: 代理相关应用信息，如集团主企业代子企业操作的场景中ProxyOrganizationId必填
         :type Agent: :class:`tencentcloud.ess.v20201111.models.Agent`
+        :param _Hides: 生成的签署链接在签署过程隐藏的按钮列表, 可以设置隐藏的按钮列表如下
+
+0:合同签署页面更多操作按钮
+1:合同签署页面更多操作的拒绝签署按钮
+2:合同签署页面更多操作的转他人处理按钮
+3:签署成功页的查看详情按钮
+        :type Hides: list of int
         """
         self._Operator = None
         self._OrganizationName = None
         self._Name = None
         self._Mobile = None
         self._EndPoint = None
         self._FlowId = None
         self._FlowGroupId = None
         self._PathType = None
         self._AutoJumpBack = None
         self._Agent = None
+        self._Hides = None
 
     @property
     def Operator(self):
         return self._Operator
 
     @Operator.setter
     def Operator(self, Operator):
@@ -5036,14 +5044,22 @@
     def Agent(self):
         return self._Agent
 
     @Agent.setter
     def Agent(self, Agent):
         self._Agent = Agent
 
+    @property
+    def Hides(self):
+        return self._Hides
+
+    @Hides.setter
+    def Hides(self, Hides):
+        self._Hides = Hides
+
 
     def _deserialize(self, params):
         if params.get("Operator") is not None:
             self._Operator = UserInfo()
             self._Operator._deserialize(params.get("Operator"))
         self._OrganizationName = params.get("OrganizationName")
         self._Name = params.get("Name")
@@ -5052,14 +5068,15 @@
         self._FlowId = params.get("FlowId")
         self._FlowGroupId = params.get("FlowGroupId")
         self._PathType = params.get("PathType")
         self._AutoJumpBack = params.get("AutoJumpBack")
         if params.get("Agent") is not None:
             self._Agent = Agent()
             self._Agent._deserialize(params.get("Agent"))
+        self._Hides = params.get("Hides")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -9619,15 +9636,15 @@
         :type PreReadTime: int
         :param _UserId: 签署方经办人的用户ID,和签署方经办人姓名+手机号+证件必须有一个。
         :type UserId: str
         :param _Required: 当前只支持true，默认为true
         :type Required: bool
         :param _ApproverSource: 签署人用户来源,企微侧用户请传入：WEWORKAPP
         :type ApproverSource: str
-        :param _CustomApproverTag: 客户自定义签署人标识，64位长度，保证唯一。非企微场景不使用此字段
+        :param _CustomApproverTag: 客户自定义签署人标识，64位长度，保证唯一。用于发起含有或签签署人的合同。或签参与人必须有此字段。不同或签参与人CustomApproverTag需要保证唯一。如果或签签署人为本方企微参与人，ApproverSource参数需要指定WEWORKAPP
         :type CustomApproverTag: str
         :param _RegisterInfo: 快速注册相关信息，目前暂未开放！
         :type RegisterInfo: :class:`tencentcloud.ess.v20201111.models.RegisterInfo`
         :param _ApproverOption: 签署人个性化能力值
         :type ApproverOption: :class:`tencentcloud.ess.v20201111.models.ApproverOption`
         :param _JumpUrl: 签署完前端跳转的url，暂未使用
         :type JumpUrl: str
@@ -12032,38 +12049,54 @@
 
     def __init__(self):
         r"""
         :param _LegalName: 法人姓名
         :type LegalName: str
         :param _Uscc: 社会统一信用代码
         :type Uscc: str
+        :param _UnifiedSocialCreditCode: 社会统一信用代码
+        :type UnifiedSocialCreditCode: str
         """
         self._LegalName = None
         self._Uscc = None
+        self._UnifiedSocialCreditCode = None
 
     @property
     def LegalName(self):
         return self._LegalName
 
     @LegalName.setter
     def LegalName(self, LegalName):
         self._LegalName = LegalName
 
     @property
     def Uscc(self):
+        warnings.warn("parameter `Uscc` is deprecated", DeprecationWarning) 
+
         return self._Uscc
 
     @Uscc.setter
     def Uscc(self, Uscc):
+        warnings.warn("parameter `Uscc` is deprecated", DeprecationWarning) 
+
         self._Uscc = Uscc
 
+    @property
+    def UnifiedSocialCreditCode(self):
+        return self._UnifiedSocialCreditCode
+
+    @UnifiedSocialCreditCode.setter
+    def UnifiedSocialCreditCode(self, UnifiedSocialCreditCode):
+        self._UnifiedSocialCreditCode = UnifiedSocialCreditCode
+
 
     def _deserialize(self, params):
         self._LegalName = params.get("LegalName")
         self._Uscc = params.get("Uscc")
+        self._UnifiedSocialCreditCode = params.get("UnifiedSocialCreditCode")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-ess-3.0.939/tencentcloud_sdk_python_ess.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ess-3.0.940/tencentcloud_sdk_python_ess.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ess
-Version: 3.0.939
+Version: 3.0.940
 Summary: Tencent Cloud Ess SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ess-3.0.939/PKG-INFO` & `tencentcloud-sdk-python-ess-3.0.940/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ess
-Version: 3.0.939
+Version: 3.0.940
 Summary: Tencent Cloud Ess SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ess-3.0.939/README.rst` & `tencentcloud-sdk-python-ess-3.0.940/README.rst`

 * *Files identical despite different names*

