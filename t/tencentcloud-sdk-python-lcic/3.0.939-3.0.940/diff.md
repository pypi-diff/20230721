# Comparing `tmp/tencentcloud-sdk-python-lcic-3.0.939.tar.gz` & `tmp/tencentcloud-sdk-python-lcic-3.0.940.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-lcic-3.0.939.tar", last modified: Thu Jul 20 00:26:48 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-lcic-3.0.940.tar", last modified: Fri Jul 21 00:44:59 2023, max compression
```

## Comparing `tencentcloud-sdk-python-lcic-3.0.939.tar` & `tencentcloud-sdk-python-lcic-3.0.940.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 00:26:48.000000 tencentcloud-sdk-python-lcic-3.0.939/
--rw-r--r--   0 root         (0) root         (0)     1008 2023-07-20 00:26:48.000000 tencentcloud-sdk-python-lcic-3.0.939/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 00:26:48.000000 tencentcloud-sdk-python-lcic-3.0.939/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-20 00:26:48.000000 tencentcloud-sdk-python-lcic-3.0.939/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 00:26:48.000000 tencentcloud-sdk-python-lcic-3.0.939/tencentcloud/lcic/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 00:26:48.000000 tencentcloud-sdk-python-lcic-3.0.939/tencentcloud/lcic/v20220817/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-20 00:26:48.000000 tencentcloud-sdk-python-lcic-3.0.939/tencentcloud/lcic/v20220817/__init__.py
--rw-r--r--   0 root         (0) root         (0)    48865 2023-07-20 00:26:48.000000 tencentcloud-sdk-python-lcic-3.0.939/tencentcloud/lcic/v20220817/lcic_client.py
--rw-r--r--   0 root         (0) root         (0)     4414 2023-07-20 00:26:48.000000 tencentcloud-sdk-python-lcic-3.0.939/tencentcloud/lcic/v20220817/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   229644 2023-07-20 00:26:48.000000 tencentcloud-sdk-python-lcic-3.0.939/tencentcloud/lcic/v20220817/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-20 00:26:48.000000 tencentcloud-sdk-python-lcic-3.0.939/tencentcloud/lcic/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-20 00:26:48.000000 tencentcloud-sdk-python-lcic-3.0.939/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 00:26:48.000000 tencentcloud-sdk-python-lcic-3.0.939/tencentcloud_sdk_python_lcic.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 00:26:48.000000 tencentcloud-sdk-python-lcic-3.0.939/tencentcloud_sdk_python_lcic.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-07-20 00:26:48.000000 tencentcloud-sdk-python-lcic-3.0.939/tencentcloud_sdk_python_lcic.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-20 00:26:48.000000 tencentcloud-sdk-python-lcic-3.0.939/tencentcloud_sdk_python_lcic.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-20 00:26:48.000000 tencentcloud-sdk-python-lcic-3.0.939/tencentcloud_sdk_python_lcic.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-20 00:26:48.000000 tencentcloud-sdk-python-lcic-3.0.939/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      740 2023-07-20 00:26:48.000000 tencentcloud-sdk-python-lcic-3.0.939/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:44:59.000000 tencentcloud-sdk-python-lcic-3.0.940/
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-07-21 00:44:59.000000 tencentcloud-sdk-python-lcic-3.0.940/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:44:59.000000 tencentcloud-sdk-python-lcic-3.0.940/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-21 00:44:59.000000 tencentcloud-sdk-python-lcic-3.0.940/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:44:59.000000 tencentcloud-sdk-python-lcic-3.0.940/tencentcloud/lcic/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:44:59.000000 tencentcloud-sdk-python-lcic-3.0.940/tencentcloud/lcic/v20220817/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 00:44:59.000000 tencentcloud-sdk-python-lcic-3.0.940/tencentcloud/lcic/v20220817/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    48865 2023-07-21 00:44:59.000000 tencentcloud-sdk-python-lcic-3.0.940/tencentcloud/lcic/v20220817/lcic_client.py
+-rw-r--r--   0 root         (0) root         (0)     4414 2023-07-21 00:44:59.000000 tencentcloud-sdk-python-lcic-3.0.940/tencentcloud/lcic/v20220817/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   231333 2023-07-21 00:44:59.000000 tencentcloud-sdk-python-lcic-3.0.940/tencentcloud/lcic/v20220817/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 00:44:59.000000 tencentcloud-sdk-python-lcic-3.0.940/tencentcloud/lcic/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-21 00:44:59.000000 tencentcloud-sdk-python-lcic-3.0.940/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:44:59.000000 tencentcloud-sdk-python-lcic-3.0.940/tencentcloud_sdk_python_lcic.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 00:44:59.000000 tencentcloud-sdk-python-lcic-3.0.940/tencentcloud_sdk_python_lcic.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-07-21 00:44:59.000000 tencentcloud-sdk-python-lcic-3.0.940/tencentcloud_sdk_python_lcic.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-21 00:44:59.000000 tencentcloud-sdk-python-lcic-3.0.940/tencentcloud_sdk_python_lcic.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-21 00:44:59.000000 tencentcloud-sdk-python-lcic-3.0.940/tencentcloud_sdk_python_lcic.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-21 00:44:59.000000 tencentcloud-sdk-python-lcic-3.0.940/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      740 2023-07-21 00:44:59.000000 tencentcloud-sdk-python-lcic-3.0.940/README.rst
```

### Comparing `tencentcloud-sdk-python-lcic-3.0.939/setup.py` & `tencentcloud-sdk-python-lcic-3.0.940/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lcic-3.0.939/tencentcloud/__init__.py` & `tencentcloud-sdk-python-lcic-3.0.940/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-lcic-3.0.939/tencentcloud/lcic/v20220817/lcic_client.py` & `tencentcloud-sdk-python-lcic-3.0.940/tencentcloud/lcic/v20220817/lcic_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lcic-3.0.939/tencentcloud/lcic/v20220817/errorcodes.py` & `tencentcloud-sdk-python-lcic-3.0.940/tencentcloud/lcic/v20220817/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lcic-3.0.939/tencentcloud/lcic/v20220817/models.py` & `tencentcloud-sdk-python-lcic-3.0.940/tencentcloud/lcic/v20220817/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1669,14 +1669,16 @@
         :type EnableDirectControl: int
         :param _InteractionMode: 开启专注模式。
 0 收看全部角色音视频(默认)
 1 只看老师和助教
         :type InteractionMode: int
         :param _VideoOrientation: 横竖屏。0：横屏开播（默认值）; 1：竖屏开播，当前仅支持移动端的纯视频类型
         :type VideoOrientation: int
+        :param _IsGradingRequiredPostClass: 开启课后评分。 0：不开启(默认)  1：开启
+        :type IsGradingRequiredPostClass: int
         """
         self._Name = None
         self._StartTime = None
         self._EndTime = None
         self._SdkAppId = None
         self._Resolution = None
         self._MaxMicNumber = None
@@ -1690,14 +1692,15 @@
         self._RTCAudienceNumber = None
         self._AudienceType = None
         self._RecordLayout = None
         self._GroupId = None
         self._EnableDirectControl = None
         self._InteractionMode = None
         self._VideoOrientation = None
+        self._IsGradingRequiredPostClass = None
 
     @property
     def Name(self):
         return self._Name
 
     @Name.setter
     def Name(self, Name):
@@ -1851,14 +1854,22 @@
     def VideoOrientation(self):
         return self._VideoOrientation
 
     @VideoOrientation.setter
     def VideoOrientation(self, VideoOrientation):
         self._VideoOrientation = VideoOrientation
 
+    @property
+    def IsGradingRequiredPostClass(self):
+        return self._IsGradingRequiredPostClass
+
+    @IsGradingRequiredPostClass.setter
+    def IsGradingRequiredPostClass(self, IsGradingRequiredPostClass):
+        self._IsGradingRequiredPostClass = IsGradingRequiredPostClass
+
 
     def _deserialize(self, params):
         self._Name = params.get("Name")
         self._StartTime = params.get("StartTime")
         self._EndTime = params.get("EndTime")
         self._SdkAppId = params.get("SdkAppId")
         self._Resolution = params.get("Resolution")
@@ -1873,14 +1884,15 @@
         self._RTCAudienceNumber = params.get("RTCAudienceNumber")
         self._AudienceType = params.get("AudienceType")
         self._RecordLayout = params.get("RecordLayout")
         self._GroupId = params.get("GroupId")
         self._EnableDirectControl = params.get("EnableDirectControl")
         self._InteractionMode = params.get("InteractionMode")
         self._VideoOrientation = params.get("VideoOrientation")
+        self._IsGradingRequiredPostClass = params.get("IsGradingRequiredPostClass")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -4007,14 +4019,16 @@
         :type EnableDirectControl: int
         :param _InteractionMode: 开启专注模式。
 0 收看全部角色音视频(默认)
 1 只看老师和助教
         :type InteractionMode: int
         :param _VideoOrientation: 横竖屏。0：横屏开播（默认值）; 1：竖屏开播，当前仅支持移动端的纯视频类型
         :type VideoOrientation: int
+        :param _IsGradingRequiredPostClass: 开启课后评分。 0：不开启(默认)  1：开启
+        :type IsGradingRequiredPostClass: int
         :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self._Name = None
         self._StartTime = None
         self._EndTime = None
         self._TeacherId = None
@@ -4028,14 +4042,15 @@
         self._Assistants = None
         self._RecordUrl = None
         self._Status = None
         self._GroupId = None
         self._EnableDirectControl = None
         self._InteractionMode = None
         self._VideoOrientation = None
+        self._IsGradingRequiredPostClass = None
         self._RequestId = None
 
     @property
     def Name(self):
         return self._Name
 
     @Name.setter
@@ -4175,14 +4190,22 @@
         return self._VideoOrientation
 
     @VideoOrientation.setter
     def VideoOrientation(self, VideoOrientation):
         self._VideoOrientation = VideoOrientation
 
     @property
+    def IsGradingRequiredPostClass(self):
+        return self._IsGradingRequiredPostClass
+
+    @IsGradingRequiredPostClass.setter
+    def IsGradingRequiredPostClass(self, IsGradingRequiredPostClass):
+        self._IsGradingRequiredPostClass = IsGradingRequiredPostClass
+
+    @property
     def RequestId(self):
         return self._RequestId
 
     @RequestId.setter
     def RequestId(self, RequestId):
         self._RequestId = RequestId
 
@@ -4202,14 +4225,15 @@
         self._Assistants = params.get("Assistants")
         self._RecordUrl = params.get("RecordUrl")
         self._Status = params.get("Status")
         self._GroupId = params.get("GroupId")
         self._EnableDirectControl = params.get("EnableDirectControl")
         self._InteractionMode = params.get("InteractionMode")
         self._VideoOrientation = params.get("VideoOrientation")
+        self._IsGradingRequiredPostClass = params.get("IsGradingRequiredPostClass")
         self._RequestId = params.get("RequestId")
 
 
 class DescribeRoomStatisticsRequest(AbstractModel):
     """DescribeRoomStatistics请求参数结构体
 
     """
@@ -6755,14 +6779,16 @@
         :type EnableDirectControl: int
         :param _InteractionMode: 开启专注模式。
 0 收看全部角色音视频(默认)
 1 只看老师和助教
         :type InteractionMode: int
         :param _VideoOrientation: 横竖屏。0：横屏开播（默认值）; 1：竖屏开播，当前仅支持移动端的纯视频类型
         :type VideoOrientation: int
+        :param _IsGradingRequiredPostClass: 开启课后评分。 0：不开启(默认)  1：开启
+        :type IsGradingRequiredPostClass: int
         """
         self._RoomId = None
         self._SdkAppId = None
         self._StartTime = None
         self._EndTime = None
         self._TeacherId = None
         self._Name = None
@@ -6773,14 +6799,15 @@
         self._SubType = None
         self._DisableRecord = None
         self._Assistants = None
         self._GroupId = None
         self._EnableDirectControl = None
         self._InteractionMode = None
         self._VideoOrientation = None
+        self._IsGradingRequiredPostClass = None
 
     @property
     def RoomId(self):
         return self._RoomId
 
     @RoomId.setter
     def RoomId(self, RoomId):
@@ -6910,14 +6937,22 @@
     def VideoOrientation(self):
         return self._VideoOrientation
 
     @VideoOrientation.setter
     def VideoOrientation(self, VideoOrientation):
         self._VideoOrientation = VideoOrientation
 
+    @property
+    def IsGradingRequiredPostClass(self):
+        return self._IsGradingRequiredPostClass
+
+    @IsGradingRequiredPostClass.setter
+    def IsGradingRequiredPostClass(self, IsGradingRequiredPostClass):
+        self._IsGradingRequiredPostClass = IsGradingRequiredPostClass
+
 
     def _deserialize(self, params):
         self._RoomId = params.get("RoomId")
         self._SdkAppId = params.get("SdkAppId")
         self._StartTime = params.get("StartTime")
         self._EndTime = params.get("EndTime")
         self._TeacherId = params.get("TeacherId")
@@ -6929,14 +6964,15 @@
         self._SubType = params.get("SubType")
         self._DisableRecord = params.get("DisableRecord")
         self._Assistants = params.get("Assistants")
         self._GroupId = params.get("GroupId")
         self._EnableDirectControl = params.get("EnableDirectControl")
         self._InteractionMode = params.get("InteractionMode")
         self._VideoOrientation = params.get("VideoOrientation")
+        self._IsGradingRequiredPostClass = params.get("IsGradingRequiredPostClass")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-lcic-3.0.939/tencentcloud_sdk_python_lcic.egg-info/PKG-INFO` & `tencentcloud-sdk-python-lcic-3.0.940/tencentcloud_sdk_python_lcic.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-lcic
-Version: 3.0.939
+Version: 3.0.940
 Summary: Tencent Cloud Lcic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-lcic-3.0.939/PKG-INFO` & `tencentcloud-sdk-python-lcic-3.0.940/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-lcic
-Version: 3.0.939
+Version: 3.0.940
 Summary: Tencent Cloud Lcic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-lcic-3.0.939/README.rst` & `tencentcloud-sdk-python-lcic-3.0.940/README.rst`

 * *Files identical despite different names*

