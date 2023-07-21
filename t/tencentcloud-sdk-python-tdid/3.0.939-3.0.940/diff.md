# Comparing `tmp/tencentcloud-sdk-python-tdid-3.0.939.tar.gz` & `tmp/tencentcloud-sdk-python-tdid-3.0.940.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tdid-3.0.939.tar", last modified: Thu Jul 20 00:34:45 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tdid-3.0.940.tar", last modified: Fri Jul 21 00:50:43 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tdid-3.0.939.tar` & `tencentcloud-sdk-python-tdid-3.0.940.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 00:34:45.000000 tencentcloud-sdk-python-tdid-3.0.939/
--rw-r--r--   0 root         (0) root         (0)     1008 2023-07-20 00:34:44.000000 tencentcloud-sdk-python-tdid-3.0.939/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 00:34:45.000000 tencentcloud-sdk-python-tdid-3.0.939/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-20 00:34:44.000000 tencentcloud-sdk-python-tdid-3.0.939/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 00:34:45.000000 tencentcloud-sdk-python-tdid-3.0.939/tencentcloud/tdid/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 00:34:45.000000 tencentcloud-sdk-python-tdid-3.0.939/tencentcloud/tdid/v20210519/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-20 00:34:44.000000 tencentcloud-sdk-python-tdid-3.0.939/tencentcloud/tdid/v20210519/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17361 2023-07-20 00:34:44.000000 tencentcloud-sdk-python-tdid-3.0.939/tencentcloud/tdid/v20210519/tdid_client.py
--rw-r--r--   0 root         (0) root         (0)     1838 2023-07-20 00:34:44.000000 tencentcloud-sdk-python-tdid-3.0.939/tencentcloud/tdid/v20210519/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    63817 2023-07-20 00:34:44.000000 tencentcloud-sdk-python-tdid-3.0.939/tencentcloud/tdid/v20210519/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-20 00:34:44.000000 tencentcloud-sdk-python-tdid-3.0.939/tencentcloud/tdid/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-20 00:34:45.000000 tencentcloud-sdk-python-tdid-3.0.939/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 00:34:45.000000 tencentcloud-sdk-python-tdid-3.0.939/tencentcloud_sdk_python_tdid.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 00:34:45.000000 tencentcloud-sdk-python-tdid-3.0.939/tencentcloud_sdk_python_tdid.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-07-20 00:34:45.000000 tencentcloud-sdk-python-tdid-3.0.939/tencentcloud_sdk_python_tdid.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-20 00:34:45.000000 tencentcloud-sdk-python-tdid-3.0.939/tencentcloud_sdk_python_tdid.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-20 00:34:45.000000 tencentcloud-sdk-python-tdid-3.0.939/tencentcloud_sdk_python_tdid.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-20 00:34:45.000000 tencentcloud-sdk-python-tdid-3.0.939/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      740 2023-07-20 00:34:44.000000 tencentcloud-sdk-python-tdid-3.0.939/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:50:43.000000 tencentcloud-sdk-python-tdid-3.0.940/
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-07-21 00:50:43.000000 tencentcloud-sdk-python-tdid-3.0.940/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:50:43.000000 tencentcloud-sdk-python-tdid-3.0.940/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-21 00:50:43.000000 tencentcloud-sdk-python-tdid-3.0.940/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:50:43.000000 tencentcloud-sdk-python-tdid-3.0.940/tencentcloud/tdid/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:50:43.000000 tencentcloud-sdk-python-tdid-3.0.940/tencentcloud/tdid/v20210519/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 00:50:43.000000 tencentcloud-sdk-python-tdid-3.0.940/tencentcloud/tdid/v20210519/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14468 2023-07-21 00:50:43.000000 tencentcloud-sdk-python-tdid-3.0.940/tencentcloud/tdid/v20210519/tdid_client.py
+-rw-r--r--   0 root         (0) root         (0)     1838 2023-07-21 00:50:43.000000 tencentcloud-sdk-python-tdid-3.0.940/tencentcloud/tdid/v20210519/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    49215 2023-07-21 00:50:43.000000 tencentcloud-sdk-python-tdid-3.0.940/tencentcloud/tdid/v20210519/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 00:50:43.000000 tencentcloud-sdk-python-tdid-3.0.940/tencentcloud/tdid/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-21 00:50:43.000000 tencentcloud-sdk-python-tdid-3.0.940/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:50:43.000000 tencentcloud-sdk-python-tdid-3.0.940/tencentcloud_sdk_python_tdid.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 00:50:43.000000 tencentcloud-sdk-python-tdid-3.0.940/tencentcloud_sdk_python_tdid.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-07-21 00:50:43.000000 tencentcloud-sdk-python-tdid-3.0.940/tencentcloud_sdk_python_tdid.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-21 00:50:43.000000 tencentcloud-sdk-python-tdid-3.0.940/tencentcloud_sdk_python_tdid.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-21 00:50:43.000000 tencentcloud-sdk-python-tdid-3.0.940/tencentcloud_sdk_python_tdid.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-21 00:50:43.000000 tencentcloud-sdk-python-tdid-3.0.940/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      740 2023-07-21 00:50:43.000000 tencentcloud-sdk-python-tdid-3.0.940/README.rst
```

### Comparing `tencentcloud-sdk-python-tdid-3.0.939/setup.py` & `tencentcloud-sdk-python-tdid-3.0.940/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tdid-3.0.939/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tdid-3.0.940/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tdid-3.0.939/tencentcloud/tdid/v20210519/tdid_client.py` & `tencentcloud-sdk-python-tdid-3.0.940/tencentcloud/tdid/v20210519/tdid_client.py`

 * *Files 14% similar despite different names*

```diff
@@ -247,64 +247,14 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def GetConsortiumClusterList(self, request):
-        """下线已有内测接口，待上线正式版本的接口
-
-        获取联盟bcos网络列表
-
-        :param request: Request instance for GetConsortiumClusterList.
-        :type request: :class:`tencentcloud.tdid.v20210519.models.GetConsortiumClusterListRequest`
-        :rtype: :class:`tencentcloud.tdid.v20210519.models.GetConsortiumClusterListResponse`
-
-        """
-        try:
-            params = request._serialize()
-            headers = request.headers
-            body = self.call("GetConsortiumClusterList", params, headers=headers)
-            response = json.loads(body)
-            model = models.GetConsortiumClusterListResponse()
-            model._deserialize(response["Response"])
-            return model
-        except Exception as e:
-            if isinstance(e, TencentCloudSDKException):
-                raise
-            else:
-                raise TencentCloudSDKException(type(e).__name__, str(e))
-
-
-    def GetConsortiumList(self, request):
-        """下线已有内测接口，待上线正式版本的接口
-
-        获取联盟列表
-
-        :param request: Request instance for GetConsortiumList.
-        :type request: :class:`tencentcloud.tdid.v20210519.models.GetConsortiumListRequest`
-        :rtype: :class:`tencentcloud.tdid.v20210519.models.GetConsortiumListResponse`
-
-        """
-        try:
-            params = request._serialize()
-            headers = request.headers
-            body = self.call("GetConsortiumList", params, headers=headers)
-            response = json.loads(body)
-            model = models.GetConsortiumListResponse()
-            model._deserialize(response["Response"])
-            return model
-        except Exception as e:
-            if isinstance(e, TencentCloudSDKException):
-                raise
-            else:
-                raise TencentCloudSDKException(type(e).__name__, str(e))
-
-
     def GetCptInfo(self, request):
         """该接口不再使用
 
         凭证模版详情
 
         :param request: Request instance for GetCptInfo.
         :type request: :class:`tencentcloud.tdid.v20210519.models.GetCptInfoRequest`
@@ -320,39 +270,14 @@
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
-
-
-    def GetCredentialCptRank(self, request):
-        """下线已有内测接口，待上线正式版本的接口
-
-        凭证颁发按机构排行
-
-        :param request: Request instance for GetCredentialCptRank.
-        :type request: :class:`tencentcloud.tdid.v20210519.models.GetCredentialCptRankRequest`
-        :rtype: :class:`tencentcloud.tdid.v20210519.models.GetCredentialCptRankResponse`
-
-        """
-        try:
-            params = request._serialize()
-            headers = request.headers
-            body = self.call("GetCredentialCptRank", params, headers=headers)
-            response = json.loads(body)
-            model = models.GetCredentialCptRankResponse()
-            model._deserialize(response["Response"])
-            return model
-        except Exception as e:
-            if isinstance(e, TencentCloudSDKException):
-                raise
-            else:
-                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetCredentialStatus(self, request):
         """该接口不再使用
 
         获取凭证链上状态信息
```

### Comparing `tencentcloud-sdk-python-tdid-3.0.939/tencentcloud/tdid/v20210519/errorcodes.py` & `tencentcloud-sdk-python-tdid-3.0.940/tencentcloud/tdid/v20210519/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tdid-3.0.939/tencentcloud/tdid/v20210519/models.py` & `tencentcloud-sdk-python-tdid-3.0.940/tencentcloud/tdid/v20210519/models.py`

 * *Files 19% similar despite different names*

```diff
@@ -84,215 +84,14 @@
         self._RequestId = RequestId
 
 
     def _deserialize(self, params):
         self._RequestId = params.get("RequestId")
 
 
-class BcosClusterItem(AbstractModel):
-    """bcos网络信息
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _ChainId: 网络索引id
-        :type ChainId: int
-        :param _ChainName: 网络名称
-        :type ChainName: str
-        :param _AgencyCount: 机构数量
-        :type AgencyCount: int
-        :param _ConsortiumId: 联盟id
-        :type ConsortiumId: int
-        :param _CreateTime: 创建时间
-        :type CreateTime: str
-        :param _ExpireTime: 过期时间
-        :type ExpireTime: str
-        :param _ChainStatus: 网络状态
-        :type ChainStatus: int
-        :param _ResourceId: 资源 id
-        :type ResourceId: str
-        :param _ClusterId: 集群id
-        :type ClusterId: str
-        :param _ConsortiumName: 组织名称
-        :type ConsortiumName: str
-        :param _AgencyId: 机构id
-        :type AgencyId: int
-        :param _AutoRenewFlag: 续费状态
-        :type AutoRenewFlag: int
-        :param _TotalNetworkNode: 网络模式
-        :type TotalNetworkNode: int
-        :param _TotalCreateNode: 创建节点数
-        :type TotalCreateNode: int
-        :param _TotalGroups: 总群组数量
-        :type TotalGroups: int
-        """
-        self._ChainId = None
-        self._ChainName = None
-        self._AgencyCount = None
-        self._ConsortiumId = None
-        self._CreateTime = None
-        self._ExpireTime = None
-        self._ChainStatus = None
-        self._ResourceId = None
-        self._ClusterId = None
-        self._ConsortiumName = None
-        self._AgencyId = None
-        self._AutoRenewFlag = None
-        self._TotalNetworkNode = None
-        self._TotalCreateNode = None
-        self._TotalGroups = None
-
-    @property
-    def ChainId(self):
-        return self._ChainId
-
-    @ChainId.setter
-    def ChainId(self, ChainId):
-        self._ChainId = ChainId
-
-    @property
-    def ChainName(self):
-        return self._ChainName
-
-    @ChainName.setter
-    def ChainName(self, ChainName):
-        self._ChainName = ChainName
-
-    @property
-    def AgencyCount(self):
-        return self._AgencyCount
-
-    @AgencyCount.setter
-    def AgencyCount(self, AgencyCount):
-        self._AgencyCount = AgencyCount
-
-    @property
-    def ConsortiumId(self):
-        return self._ConsortiumId
-
-    @ConsortiumId.setter
-    def ConsortiumId(self, ConsortiumId):
-        self._ConsortiumId = ConsortiumId
-
-    @property
-    def CreateTime(self):
-        return self._CreateTime
-
-    @CreateTime.setter
-    def CreateTime(self, CreateTime):
-        self._CreateTime = CreateTime
-
-    @property
-    def ExpireTime(self):
-        return self._ExpireTime
-
-    @ExpireTime.setter
-    def ExpireTime(self, ExpireTime):
-        self._ExpireTime = ExpireTime
-
-    @property
-    def ChainStatus(self):
-        return self._ChainStatus
-
-    @ChainStatus.setter
-    def ChainStatus(self, ChainStatus):
-        self._ChainStatus = ChainStatus
-
-    @property
-    def ResourceId(self):
-        return self._ResourceId
-
-    @ResourceId.setter
-    def ResourceId(self, ResourceId):
-        self._ResourceId = ResourceId
-
-    @property
-    def ClusterId(self):
-        return self._ClusterId
-
-    @ClusterId.setter
-    def ClusterId(self, ClusterId):
-        self._ClusterId = ClusterId
-
-    @property
-    def ConsortiumName(self):
-        return self._ConsortiumName
-
-    @ConsortiumName.setter
-    def ConsortiumName(self, ConsortiumName):
-        self._ConsortiumName = ConsortiumName
-
-    @property
-    def AgencyId(self):
-        return self._AgencyId
-
-    @AgencyId.setter
-    def AgencyId(self, AgencyId):
-        self._AgencyId = AgencyId
-
-    @property
-    def AutoRenewFlag(self):
-        return self._AutoRenewFlag
-
-    @AutoRenewFlag.setter
-    def AutoRenewFlag(self, AutoRenewFlag):
-        self._AutoRenewFlag = AutoRenewFlag
-
-    @property
-    def TotalNetworkNode(self):
-        return self._TotalNetworkNode
-
-    @TotalNetworkNode.setter
-    def TotalNetworkNode(self, TotalNetworkNode):
-        self._TotalNetworkNode = TotalNetworkNode
-
-    @property
-    def TotalCreateNode(self):
-        return self._TotalCreateNode
-
-    @TotalCreateNode.setter
-    def TotalCreateNode(self, TotalCreateNode):
-        self._TotalCreateNode = TotalCreateNode
-
-    @property
-    def TotalGroups(self):
-        return self._TotalGroups
-
-    @TotalGroups.setter
-    def TotalGroups(self, TotalGroups):
-        self._TotalGroups = TotalGroups
-
-
-    def _deserialize(self, params):
-        self._ChainId = params.get("ChainId")
-        self._ChainName = params.get("ChainName")
-        self._AgencyCount = params.get("AgencyCount")
-        self._ConsortiumId = params.get("ConsortiumId")
-        self._CreateTime = params.get("CreateTime")
-        self._ExpireTime = params.get("ExpireTime")
-        self._ChainStatus = params.get("ChainStatus")
-        self._ResourceId = params.get("ResourceId")
-        self._ClusterId = params.get("ClusterId")
-        self._ConsortiumName = params.get("ConsortiumName")
-        self._AgencyId = params.get("AgencyId")
-        self._AutoRenewFlag = params.get("AutoRenewFlag")
-        self._TotalNetworkNode = params.get("TotalNetworkNode")
-        self._TotalCreateNode = params.get("TotalCreateNode")
-        self._TotalGroups = params.get("TotalGroups")
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            property_name = name[1:]
-            if property_name in memeber_set:
-                memeber_set.remove(property_name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
 class CheckChainRequest(AbstractModel):
     """CheckChain请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -403,140 +202,14 @@
     def _deserialize(self, params):
         self._RoleType = params.get("RoleType")
         self._ChainId = params.get("ChainId")
         self._AppName = params.get("AppName")
         self._RequestId = params.get("RequestId")
 
 
-class ConsortiumItem(AbstractModel):
-    """联盟信息
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _Id: 联盟id
-        :type Id: int
-        :param _Name: 联盟名称
-        :type Name: str
-        """
-        self._Id = None
-        self._Name = None
-
-    @property
-    def Id(self):
-        return self._Id
-
-    @Id.setter
-    def Id(self, Id):
-        self._Id = Id
-
-    @property
-    def Name(self):
-        return self._Name
-
-    @Name.setter
-    def Name(self, Name):
-        self._Name = Name
-
-
-    def _deserialize(self, params):
-        self._Id = params.get("Id")
-        self._Name = params.get("Name")
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            property_name = name[1:]
-            if property_name in memeber_set:
-                memeber_set.remove(property_name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
-class CptIssueRank(AbstractModel):
-    """模板颁发量排名
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _CptName: 模板名称
-        :type CptName: str
-        :param _Rank: 名次
-        :type Rank: int
-        :param _Count: 颁发量
-        :type Count: int
-        :param _ApplyName: 应用名称
-        :type ApplyName: str
-        :param _ApplyId: 应用ID
-        :type ApplyId: int
-        """
-        self._CptName = None
-        self._Rank = None
-        self._Count = None
-        self._ApplyName = None
-        self._ApplyId = None
-
-    @property
-    def CptName(self):
-        return self._CptName
-
-    @CptName.setter
-    def CptName(self, CptName):
-        self._CptName = CptName
-
-    @property
-    def Rank(self):
-        return self._Rank
-
-    @Rank.setter
-    def Rank(self, Rank):
-        self._Rank = Rank
-
-    @property
-    def Count(self):
-        return self._Count
-
-    @Count.setter
-    def Count(self, Count):
-        self._Count = Count
-
-    @property
-    def ApplyName(self):
-        return self._ApplyName
-
-    @ApplyName.setter
-    def ApplyName(self, ApplyName):
-        self._ApplyName = ApplyName
-
-    @property
-    def ApplyId(self):
-        return self._ApplyId
-
-    @ApplyId.setter
-    def ApplyId(self, ApplyId):
-        self._ApplyId = ApplyId
-
-
-    def _deserialize(self, params):
-        self._CptName = params.get("CptName")
-        self._Rank = params.get("Rank")
-        self._Count = params.get("Count")
-        self._ApplyName = params.get("ApplyName")
-        self._ApplyId = params.get("ApplyId")
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            property_name = name[1:]
-            if property_name in memeber_set:
-                memeber_set.remove(property_name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
 class CreateCredentialRequest(AbstractModel):
     """CreateCredential请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -1411,137 +1084,14 @@
         self._Did = params.get("Did")
         self._Remark = params.get("Remark")
         self._RegisterTime = params.get("RegisterTime")
         self._RecognizeTime = params.get("RecognizeTime")
         self._RequestId = params.get("RequestId")
 
 
-class GetConsortiumClusterListRequest(AbstractModel):
-    """GetConsortiumClusterList请求参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _ConsortiumId: 联盟id
-        :type ConsortiumId: int
-        """
-        self._ConsortiumId = None
-
-    @property
-    def ConsortiumId(self):
-        return self._ConsortiumId
-
-    @ConsortiumId.setter
-    def ConsortiumId(self, ConsortiumId):
-        self._ConsortiumId = ConsortiumId
-
-
-    def _deserialize(self, params):
-        self._ConsortiumId = params.get("ConsortiumId")
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            property_name = name[1:]
-            if property_name in memeber_set:
-                memeber_set.remove(property_name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
-class GetConsortiumClusterListResponse(AbstractModel):
-    """GetConsortiumClusterList返回参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _ClusterList: 网络列表
-        :type ClusterList: list of BcosClusterItem
-        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
-        :type RequestId: str
-        """
-        self._ClusterList = None
-        self._RequestId = None
-
-    @property
-    def ClusterList(self):
-        return self._ClusterList
-
-    @ClusterList.setter
-    def ClusterList(self, ClusterList):
-        self._ClusterList = ClusterList
-
-    @property
-    def RequestId(self):
-        return self._RequestId
-
-    @RequestId.setter
-    def RequestId(self, RequestId):
-        self._RequestId = RequestId
-
-
-    def _deserialize(self, params):
-        if params.get("ClusterList") is not None:
-            self._ClusterList = []
-            for item in params.get("ClusterList"):
-                obj = BcosClusterItem()
-                obj._deserialize(item)
-                self._ClusterList.append(obj)
-        self._RequestId = params.get("RequestId")
-
-
-class GetConsortiumListRequest(AbstractModel):
-    """GetConsortiumList请求参数结构体
-
-    """
-
-
-class GetConsortiumListResponse(AbstractModel):
-    """GetConsortiumList返回参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _ConsortiumList: 联盟列表
-        :type ConsortiumList: list of ConsortiumItem
-        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
-        :type RequestId: str
-        """
-        self._ConsortiumList = None
-        self._RequestId = None
-
-    @property
-    def ConsortiumList(self):
-        return self._ConsortiumList
-
-    @ConsortiumList.setter
-    def ConsortiumList(self, ConsortiumList):
-        self._ConsortiumList = ConsortiumList
-
-    @property
-    def RequestId(self):
-        return self._RequestId
-
-    @RequestId.setter
-    def RequestId(self, RequestId):
-        self._RequestId = RequestId
-
-
-    def _deserialize(self, params):
-        if params.get("ConsortiumList") is not None:
-            self._ConsortiumList = []
-            for item in params.get("ConsortiumList"):
-                obj = ConsortiumItem()
-                obj._deserialize(item)
-                self._ConsortiumList.append(obj)
-        self._RequestId = params.get("RequestId")
-
-
 class GetCptInfoRequest(AbstractModel):
     """GetCptInfo请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -1604,113 +1154,14 @@
 
 
     def _deserialize(self, params):
         self._CptJsonData = params.get("CptJsonData")
         self._RequestId = params.get("RequestId")
 
 
-class GetCredentialCptRankRequest(AbstractModel):
-    """GetCredentialCptRank请求参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _StartTime: 开始时间（支持到天 2021-4-23）
-        :type StartTime: str
-        :param _EndTime: 结束时间（支持到天 2021-4-23）
-        :type EndTime: str
-        :param _ClusterId: 网络ID
-        :type ClusterId: str
-        """
-        self._StartTime = None
-        self._EndTime = None
-        self._ClusterId = None
-
-    @property
-    def StartTime(self):
-        return self._StartTime
-
-    @StartTime.setter
-    def StartTime(self, StartTime):
-        self._StartTime = StartTime
-
-    @property
-    def EndTime(self):
-        return self._EndTime
-
-    @EndTime.setter
-    def EndTime(self, EndTime):
-        self._EndTime = EndTime
-
-    @property
-    def ClusterId(self):
-        return self._ClusterId
-
-    @ClusterId.setter
-    def ClusterId(self, ClusterId):
-        self._ClusterId = ClusterId
-
-
-    def _deserialize(self, params):
-        self._StartTime = params.get("StartTime")
-        self._EndTime = params.get("EndTime")
-        self._ClusterId = params.get("ClusterId")
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            property_name = name[1:]
-            if property_name in memeber_set:
-                memeber_set.remove(property_name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
-class GetCredentialCptRankResponse(AbstractModel):
-    """GetCredentialCptRank返回参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _RankIssueResult: Rank集合
-        :type RankIssueResult: list of CptIssueRank
-        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
-        :type RequestId: str
-        """
-        self._RankIssueResult = None
-        self._RequestId = None
-
-    @property
-    def RankIssueResult(self):
-        return self._RankIssueResult
-
-    @RankIssueResult.setter
-    def RankIssueResult(self, RankIssueResult):
-        self._RankIssueResult = RankIssueResult
-
-    @property
-    def RequestId(self):
-        return self._RequestId
-
-    @RequestId.setter
-    def RequestId(self, RequestId):
-        self._RequestId = RequestId
-
-
-    def _deserialize(self, params):
-        if params.get("RankIssueResult") is not None:
-            self._RankIssueResult = []
-            for item in params.get("RankIssueResult"):
-                obj = CptIssueRank()
-                obj._deserialize(item)
-                self._RankIssueResult.append(obj)
-        self._RequestId = params.get("RequestId")
-
-
 class GetCredentialStatusRequest(AbstractModel):
     """GetCredentialStatus请求参数结构体
 
     """
 
     def __init__(self):
         r"""
```

### Comparing `tencentcloud-sdk-python-tdid-3.0.939/tencentcloud_sdk_python_tdid.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tdid-3.0.940/tencentcloud_sdk_python_tdid.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tdid
-Version: 3.0.939
+Version: 3.0.940
 Summary: Tencent Cloud Tdid SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tdid-3.0.939/PKG-INFO` & `tencentcloud-sdk-python-tdid-3.0.940/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tdid
-Version: 3.0.939
+Version: 3.0.940
 Summary: Tencent Cloud Tdid SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tdid-3.0.939/README.rst` & `tencentcloud-sdk-python-tdid-3.0.940/README.rst`

 * *Files identical despite different names*

