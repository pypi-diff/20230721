# Comparing `tmp/tencentcloud-sdk-python-essbasic-3.0.939.tar.gz` & `tmp/tencentcloud-sdk-python-essbasic-3.0.940.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-essbasic-3.0.939.tar", last modified: Thu Jul 20 00:24:09 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-essbasic-3.0.940.tar", last modified: Fri Jul 21 00:29:04 2023, max compression
```

## Comparing `tencentcloud-sdk-python-essbasic-3.0.939.tar` & `tencentcloud-sdk-python-essbasic-3.0.940.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 00:24:09.000000 tencentcloud-sdk-python-essbasic-3.0.939/
--rw-r--r--   0 root         (0) root         (0)     1016 2023-07-20 00:24:09.000000 tencentcloud-sdk-python-essbasic-3.0.939/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 00:24:09.000000 tencentcloud-sdk-python-essbasic-3.0.939/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 00:24:09.000000 tencentcloud-sdk-python-essbasic-3.0.939/tencentcloud/essbasic/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-20 00:24:09.000000 tencentcloud-sdk-python-essbasic-3.0.939/tencentcloud/essbasic/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 00:24:09.000000 tencentcloud-sdk-python-essbasic-3.0.939/tencentcloud/essbasic/v20210526/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-20 00:24:09.000000 tencentcloud-sdk-python-essbasic-3.0.939/tencentcloud/essbasic/v20210526/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16662 2023-07-20 00:24:09.000000 tencentcloud-sdk-python-essbasic-3.0.939/tencentcloud/essbasic/v20210526/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    55045 2023-07-20 00:24:09.000000 tencentcloud-sdk-python-essbasic-3.0.939/tencentcloud/essbasic/v20210526/essbasic_client.py
--rw-r--r--   0 root         (0) root         (0)   386805 2023-07-20 00:24:09.000000 tencentcloud-sdk-python-essbasic-3.0.939/tencentcloud/essbasic/v20210526/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 00:24:09.000000 tencentcloud-sdk-python-essbasic-3.0.939/tencentcloud/essbasic/v20201222/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-20 00:24:09.000000 tencentcloud-sdk-python-essbasic-3.0.939/tencentcloud/essbasic/v20201222/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5392 2023-07-20 00:24:09.000000 tencentcloud-sdk-python-essbasic-3.0.939/tencentcloud/essbasic/v20201222/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    54057 2023-07-20 00:24:09.000000 tencentcloud-sdk-python-essbasic-3.0.939/tencentcloud/essbasic/v20201222/essbasic_client.py
--rw-r--r--   0 root         (0) root         (0)   270905 2023-07-20 00:24:09.000000 tencentcloud-sdk-python-essbasic-3.0.939/tencentcloud/essbasic/v20201222/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-20 00:24:09.000000 tencentcloud-sdk-python-essbasic-3.0.939/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-20 00:24:09.000000 tencentcloud-sdk-python-essbasic-3.0.939/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1684 2023-07-20 00:24:09.000000 tencentcloud-sdk-python-essbasic-3.0.939/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      752 2023-07-20 00:24:09.000000 tencentcloud-sdk-python-essbasic-3.0.939/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 00:24:09.000000 tencentcloud-sdk-python-essbasic-3.0.939/tencentcloud_sdk_python_essbasic.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 00:24:09.000000 tencentcloud-sdk-python-essbasic-3.0.939/tencentcloud_sdk_python_essbasic.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      678 2023-07-20 00:24:09.000000 tencentcloud-sdk-python-essbasic-3.0.939/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1684 2023-07-20 00:24:09.000000 tencentcloud-sdk-python-essbasic-3.0.939/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-20 00:24:09.000000 tencentcloud-sdk-python-essbasic-3.0.939/tencentcloud_sdk_python_essbasic.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:29:04.000000 tencentcloud-sdk-python-essbasic-3.0.940/
+-rw-r--r--   0 root         (0) root         (0)     1016 2023-07-21 00:29:04.000000 tencentcloud-sdk-python-essbasic-3.0.940/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:29:04.000000 tencentcloud-sdk-python-essbasic-3.0.940/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:29:04.000000 tencentcloud-sdk-python-essbasic-3.0.940/tencentcloud/essbasic/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 00:29:04.000000 tencentcloud-sdk-python-essbasic-3.0.940/tencentcloud/essbasic/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:29:04.000000 tencentcloud-sdk-python-essbasic-3.0.940/tencentcloud/essbasic/v20210526/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 00:29:04.000000 tencentcloud-sdk-python-essbasic-3.0.940/tencentcloud/essbasic/v20210526/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16662 2023-07-21 00:29:04.000000 tencentcloud-sdk-python-essbasic-3.0.940/tencentcloud/essbasic/v20210526/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    55045 2023-07-21 00:29:04.000000 tencentcloud-sdk-python-essbasic-3.0.940/tencentcloud/essbasic/v20210526/essbasic_client.py
+-rw-r--r--   0 root         (0) root         (0)   387357 2023-07-21 00:29:04.000000 tencentcloud-sdk-python-essbasic-3.0.940/tencentcloud/essbasic/v20210526/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:29:04.000000 tencentcloud-sdk-python-essbasic-3.0.940/tencentcloud/essbasic/v20201222/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 00:29:04.000000 tencentcloud-sdk-python-essbasic-3.0.940/tencentcloud/essbasic/v20201222/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5392 2023-07-21 00:29:04.000000 tencentcloud-sdk-python-essbasic-3.0.940/tencentcloud/essbasic/v20201222/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    54057 2023-07-21 00:29:04.000000 tencentcloud-sdk-python-essbasic-3.0.940/tencentcloud/essbasic/v20201222/essbasic_client.py
+-rw-r--r--   0 root         (0) root         (0)   270905 2023-07-21 00:29:04.000000 tencentcloud-sdk-python-essbasic-3.0.940/tencentcloud/essbasic/v20201222/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-21 00:29:04.000000 tencentcloud-sdk-python-essbasic-3.0.940/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-21 00:29:04.000000 tencentcloud-sdk-python-essbasic-3.0.940/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-07-21 00:29:04.000000 tencentcloud-sdk-python-essbasic-3.0.940/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      752 2023-07-21 00:29:04.000000 tencentcloud-sdk-python-essbasic-3.0.940/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:29:04.000000 tencentcloud-sdk-python-essbasic-3.0.940/tencentcloud_sdk_python_essbasic.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 00:29:04.000000 tencentcloud-sdk-python-essbasic-3.0.940/tencentcloud_sdk_python_essbasic.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      678 2023-07-21 00:29:04.000000 tencentcloud-sdk-python-essbasic-3.0.940/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-07-21 00:29:04.000000 tencentcloud-sdk-python-essbasic-3.0.940/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-21 00:29:04.000000 tencentcloud-sdk-python-essbasic-3.0.940/tencentcloud_sdk_python_essbasic.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.939/setup.py` & `tencentcloud-sdk-python-essbasic-3.0.940/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.939/tencentcloud/essbasic/v20210526/errorcodes.py` & `tencentcloud-sdk-python-essbasic-3.0.940/tencentcloud/essbasic/v20210526/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.939/tencentcloud/essbasic/v20210526/essbasic_client.py` & `tencentcloud-sdk-python-essbasic-3.0.940/tencentcloud/essbasic/v20210526/essbasic_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.939/tencentcloud/essbasic/v20210526/models.py` & `tencentcloud-sdk-python-essbasic-3.0.940/tencentcloud/essbasic/v20210526/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -6095,28 +6095,36 @@
         :type OpenId: str
         :param _AutoJumpBack: Endpoint为"APP" 类型的签署链接，可以设置此值；支持调用方小程序打开签署链接，在电子签小程序完成签署后自动回跳至调用方小程序
         :type AutoJumpBack: bool
         :param _JumpUrl: 签署完之后的H5页面的跳转链接，针对Endpoint为CHANNEL时有效，最大长度1000个字符。
         :type JumpUrl: str
         :param _Operator: 暂未开放
         :type Operator: :class:`tencentcloud.essbasic.v20210526.models.UserInfo`
+        :param _Hides: 生成的签署链接在签署过程隐藏的按钮列表, 可以设置隐藏的按钮列表如下
+
+0:合同签署页面更多操作按钮
+1:合同签署页面更多操作的拒绝签署按钮
+2:合同签署页面更多操作的转他人处理按钮
+3:签署成功页的查看详情按钮
+        :type Hides: list of int
         """
         self._Agent = None
         self._FlowIds = None
         self._FlowGroupId = None
         self._Endpoint = None
         self._GenerateType = None
         self._OrganizationName = None
         self._Name = None
         self._Mobile = None
         self._OrganizationOpenId = None
         self._OpenId = None
         self._AutoJumpBack = None
         self._JumpUrl = None
         self._Operator = None
+        self._Hides = None
 
     @property
     def Agent(self):
         return self._Agent
 
     @Agent.setter
     def Agent(self, Agent):
@@ -6218,14 +6226,22 @@
 
     @Operator.setter
     def Operator(self, Operator):
         warnings.warn("parameter `Operator` is deprecated", DeprecationWarning) 
 
         self._Operator = Operator
 
+    @property
+    def Hides(self):
+        return self._Hides
+
+    @Hides.setter
+    def Hides(self, Hides):
+        self._Hides = Hides
+
 
     def _deserialize(self, params):
         if params.get("Agent") is not None:
             self._Agent = Agent()
             self._Agent._deserialize(params.get("Agent"))
         self._FlowIds = params.get("FlowIds")
         self._FlowGroupId = params.get("FlowGroupId")
@@ -6237,14 +6253,15 @@
         self._OrganizationOpenId = params.get("OrganizationOpenId")
         self._OpenId = params.get("OpenId")
         self._AutoJumpBack = params.get("AutoJumpBack")
         self._JumpUrl = params.get("JumpUrl")
         if params.get("Operator") is not None:
             self._Operator = UserInfo()
             self._Operator._deserialize(params.get("Operator"))
+        self._Hides = params.get("Hides")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.939/tencentcloud/essbasic/v20201222/errorcodes.py` & `tencentcloud-sdk-python-essbasic-3.0.940/tencentcloud/essbasic/v20201222/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.939/tencentcloud/essbasic/v20201222/essbasic_client.py` & `tencentcloud-sdk-python-essbasic-3.0.940/tencentcloud/essbasic/v20201222/essbasic_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.939/tencentcloud/essbasic/v20201222/models.py` & `tencentcloud-sdk-python-essbasic-3.0.940/tencentcloud/essbasic/v20201222/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.939/tencentcloud/__init__.py` & `tencentcloud-sdk-python-essbasic-3.0.940/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-essbasic-3.0.939/PKG-INFO` & `tencentcloud-sdk-python-essbasic-3.0.940/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-essbasic
-Version: 3.0.939
+Version: 3.0.940
 Summary: Tencent Cloud Essbasic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.939/README.rst` & `tencentcloud-sdk-python-essbasic-3.0.940/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.939/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-essbasic-3.0.940/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.939/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO` & `tencentcloud-sdk-python-essbasic-3.0.940/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-essbasic
-Version: 3.0.939
+Version: 3.0.940
 Summary: Tencent Cloud Essbasic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

