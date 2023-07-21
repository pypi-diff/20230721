# Comparing `tmp/tencentcloud-sdk-python-tiw-3.0.939.tar.gz` & `tmp/tencentcloud-sdk-python-tiw-3.0.940.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tiw-3.0.939.tar", last modified: Thu Jul 20 00:35:51 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tiw-3.0.940.tar", last modified: Fri Jul 21 00:51:51 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tiw-3.0.939.tar` & `tencentcloud-sdk-python-tiw-3.0.940.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 00:35:51.000000 tencentcloud-sdk-python-tiw-3.0.939/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 00:35:51.000000 tencentcloud-sdk-python-tiw-3.0.939/tencentcloud_sdk_python_tiw.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 00:35:51.000000 tencentcloud-sdk-python-tiw-3.0.939/tencentcloud_sdk_python_tiw.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-20 00:35:51.000000 tencentcloud-sdk-python-tiw-3.0.939/tencentcloud_sdk_python_tiw.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-20 00:35:51.000000 tencentcloud-sdk-python-tiw-3.0.939/tencentcloud_sdk_python_tiw.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-20 00:35:51.000000 tencentcloud-sdk-python-tiw-3.0.939/tencentcloud_sdk_python_tiw.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-20 00:35:51.000000 tencentcloud-sdk-python-tiw-3.0.939/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 00:35:51.000000 tencentcloud-sdk-python-tiw-3.0.939/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 00:35:51.000000 tencentcloud-sdk-python-tiw-3.0.939/tencentcloud/tiw/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 00:35:51.000000 tencentcloud-sdk-python-tiw-3.0.939/tencentcloud/tiw/v20190919/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-20 00:35:51.000000 tencentcloud-sdk-python-tiw-3.0.939/tencentcloud/tiw/v20190919/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6089 2023-07-20 00:35:51.000000 tencentcloud-sdk-python-tiw-3.0.939/tencentcloud/tiw/v20190919/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    60499 2023-07-20 00:35:51.000000 tencentcloud-sdk-python-tiw-3.0.939/tencentcloud/tiw/v20190919/tiw_client.py
--rw-r--r--   0 root         (0) root         (0)   280360 2023-07-20 00:35:51.000000 tencentcloud-sdk-python-tiw-3.0.939/tencentcloud/tiw/v20190919/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-20 00:35:51.000000 tencentcloud-sdk-python-tiw-3.0.939/tencentcloud/tiw/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-20 00:35:51.000000 tencentcloud-sdk-python-tiw-3.0.939/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-20 00:35:51.000000 tencentcloud-sdk-python-tiw-3.0.939/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-20 00:35:51.000000 tencentcloud-sdk-python-tiw-3.0.939/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-20 00:35:51.000000 tencentcloud-sdk-python-tiw-3.0.939/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:51:51.000000 tencentcloud-sdk-python-tiw-3.0.940/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:51:51.000000 tencentcloud-sdk-python-tiw-3.0.940/tencentcloud_sdk_python_tiw.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 00:51:51.000000 tencentcloud-sdk-python-tiw-3.0.940/tencentcloud_sdk_python_tiw.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-21 00:51:51.000000 tencentcloud-sdk-python-tiw-3.0.940/tencentcloud_sdk_python_tiw.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-21 00:51:51.000000 tencentcloud-sdk-python-tiw-3.0.940/tencentcloud_sdk_python_tiw.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-21 00:51:51.000000 tencentcloud-sdk-python-tiw-3.0.940/tencentcloud_sdk_python_tiw.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-21 00:51:51.000000 tencentcloud-sdk-python-tiw-3.0.940/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:51:51.000000 tencentcloud-sdk-python-tiw-3.0.940/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:51:51.000000 tencentcloud-sdk-python-tiw-3.0.940/tencentcloud/tiw/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:51:51.000000 tencentcloud-sdk-python-tiw-3.0.940/tencentcloud/tiw/v20190919/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 00:51:51.000000 tencentcloud-sdk-python-tiw-3.0.940/tencentcloud/tiw/v20190919/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6089 2023-07-21 00:51:51.000000 tencentcloud-sdk-python-tiw-3.0.940/tencentcloud/tiw/v20190919/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    60499 2023-07-21 00:51:51.000000 tencentcloud-sdk-python-tiw-3.0.940/tencentcloud/tiw/v20190919/tiw_client.py
+-rw-r--r--   0 root         (0) root         (0)   281650 2023-07-21 00:51:51.000000 tencentcloud-sdk-python-tiw-3.0.940/tencentcloud/tiw/v20190919/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 00:51:51.000000 tencentcloud-sdk-python-tiw-3.0.940/tencentcloud/tiw/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-21 00:51:51.000000 tencentcloud-sdk-python-tiw-3.0.940/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-21 00:51:51.000000 tencentcloud-sdk-python-tiw-3.0.940/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-21 00:51:51.000000 tencentcloud-sdk-python-tiw-3.0.940/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-21 00:51:51.000000 tencentcloud-sdk-python-tiw-3.0.940/README.rst
```

### Comparing `tencentcloud-sdk-python-tiw-3.0.939/tencentcloud_sdk_python_tiw.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tiw-3.0.940/tencentcloud_sdk_python_tiw.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tiw
-Version: 3.0.939
+Version: 3.0.940
 Summary: Tencent Cloud Tiw SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tiw-3.0.939/setup.py` & `tencentcloud-sdk-python-tiw-3.0.940/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tiw-3.0.939/tencentcloud/tiw/v20190919/errorcodes.py` & `tencentcloud-sdk-python-tiw-3.0.940/tencentcloud/tiw/v20190919/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tiw-3.0.939/tencentcloud/tiw/v20190919/tiw_client.py` & `tencentcloud-sdk-python-tiw-3.0.940/tencentcloud/tiw/v20190919/tiw_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tiw-3.0.939/tencentcloud/tiw/v20190919/models.py` & `tencentcloud-sdk-python-tiw-3.0.940/tencentcloud/tiw/v20190919/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -3548,14 +3548,23 @@
         :type CompressFileUrl: str
         :param _ResourceListUrl: 资源清单文件下载URL(内测体验)
 注意：此字段可能返回 null，表示取不到有效值。
         :type ResourceListUrl: str
         :param _Ext: 文档制作方式(内测体验)
 注意：此字段可能返回 null，表示取不到有效值。
         :type Ext: str
+        :param _CreateTime: 文档转码任务创建时间，单位s
+注意：此字段可能返回 null，表示取不到有效值。
+        :type CreateTime: int
+        :param _AssignTime: 文档转码任务分配时间，单位s
+注意：此字段可能返回 null，表示取不到有效值。
+        :type AssignTime: int
+        :param _FinishedTime: 文档转码任务完成时间，单位s
+注意：此字段可能返回 null，表示取不到有效值。
+        :type FinishedTime: int
         :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self._Pages = None
         self._Progress = None
         self._Resolution = None
         self._ResultUrl = None
@@ -3563,14 +3572,17 @@
         self._TaskId = None
         self._Title = None
         self._ThumbnailUrl = None
         self._ThumbnailResolution = None
         self._CompressFileUrl = None
         self._ResourceListUrl = None
         self._Ext = None
+        self._CreateTime = None
+        self._AssignTime = None
+        self._FinishedTime = None
         self._RequestId = None
 
     @property
     def Pages(self):
         return self._Pages
 
     @Pages.setter
@@ -3662,14 +3674,38 @@
         return self._Ext
 
     @Ext.setter
     def Ext(self, Ext):
         self._Ext = Ext
 
     @property
+    def CreateTime(self):
+        return self._CreateTime
+
+    @CreateTime.setter
+    def CreateTime(self, CreateTime):
+        self._CreateTime = CreateTime
+
+    @property
+    def AssignTime(self):
+        return self._AssignTime
+
+    @AssignTime.setter
+    def AssignTime(self, AssignTime):
+        self._AssignTime = AssignTime
+
+    @property
+    def FinishedTime(self):
+        return self._FinishedTime
+
+    @FinishedTime.setter
+    def FinishedTime(self, FinishedTime):
+        self._FinishedTime = FinishedTime
+
+    @property
     def RequestId(self):
         return self._RequestId
 
     @RequestId.setter
     def RequestId(self, RequestId):
         self._RequestId = RequestId
 
@@ -3683,14 +3719,17 @@
         self._TaskId = params.get("TaskId")
         self._Title = params.get("Title")
         self._ThumbnailUrl = params.get("ThumbnailUrl")
         self._ThumbnailResolution = params.get("ThumbnailResolution")
         self._CompressFileUrl = params.get("CompressFileUrl")
         self._ResourceListUrl = params.get("ResourceListUrl")
         self._Ext = params.get("Ext")
+        self._CreateTime = params.get("CreateTime")
+        self._AssignTime = params.get("AssignTime")
+        self._FinishedTime = params.get("FinishedTime")
         self._RequestId = params.get("RequestId")
 
 
 class DescribeTranscodeSearchRequest(AbstractModel):
     """DescribeTranscodeSearch请求参数结构体
 
     """
```

### Comparing `tencentcloud-sdk-python-tiw-3.0.939/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tiw-3.0.940/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tiw-3.0.939/PKG-INFO` & `tencentcloud-sdk-python-tiw-3.0.940/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tiw
-Version: 3.0.939
+Version: 3.0.940
 Summary: Tencent Cloud Tiw SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tiw-3.0.939/README.rst` & `tencentcloud-sdk-python-tiw-3.0.940/README.rst`

 * *Files identical despite different names*

