# Comparing `tmp/tencentcloud-sdk-python-cme-3.0.939.tar.gz` & `tmp/tencentcloud-sdk-python-cme-3.0.940.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cme-3.0.939.tar", last modified: Thu Jul 20 00:21:10 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cme-3.0.940.tar", last modified: Fri Jul 21 00:26:06 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cme-3.0.939.tar` & `tencentcloud-sdk-python-cme-3.0.940.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 00:21:10.000000 tencentcloud-sdk-python-cme-3.0.939/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-20 00:21:10.000000 tencentcloud-sdk-python-cme-3.0.939/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 00:21:10.000000 tencentcloud-sdk-python-cme-3.0.939/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-20 00:21:10.000000 tencentcloud-sdk-python-cme-3.0.939/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 00:21:10.000000 tencentcloud-sdk-python-cme-3.0.939/tencentcloud/cme/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 00:21:10.000000 tencentcloud-sdk-python-cme-3.0.939/tencentcloud/cme/v20191029/
--rw-r--r--   0 root         (0) root         (0)    55451 2023-07-20 00:21:10.000000 tencentcloud-sdk-python-cme-3.0.939/tencentcloud/cme/v20191029/cme_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-20 00:21:10.000000 tencentcloud-sdk-python-cme-3.0.939/tencentcloud/cme/v20191029/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8415 2023-07-20 00:21:10.000000 tencentcloud-sdk-python-cme-3.0.939/tencentcloud/cme/v20191029/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   444358 2023-07-20 00:21:10.000000 tencentcloud-sdk-python-cme-3.0.939/tencentcloud/cme/v20191029/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-20 00:21:10.000000 tencentcloud-sdk-python-cme-3.0.939/tencentcloud/cme/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-20 00:21:10.000000 tencentcloud-sdk-python-cme-3.0.939/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 00:21:10.000000 tencentcloud-sdk-python-cme-3.0.939/tencentcloud_sdk_python_cme.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 00:21:10.000000 tencentcloud-sdk-python-cme-3.0.939/tencentcloud_sdk_python_cme.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-20 00:21:10.000000 tencentcloud-sdk-python-cme-3.0.939/tencentcloud_sdk_python_cme.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-20 00:21:10.000000 tencentcloud-sdk-python-cme-3.0.939/tencentcloud_sdk_python_cme.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-20 00:21:10.000000 tencentcloud-sdk-python-cme-3.0.939/tencentcloud_sdk_python_cme.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-20 00:21:10.000000 tencentcloud-sdk-python-cme-3.0.939/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-20 00:21:10.000000 tencentcloud-sdk-python-cme-3.0.939/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:26:06.000000 tencentcloud-sdk-python-cme-3.0.940/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-21 00:26:06.000000 tencentcloud-sdk-python-cme-3.0.940/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:26:06.000000 tencentcloud-sdk-python-cme-3.0.940/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-21 00:26:06.000000 tencentcloud-sdk-python-cme-3.0.940/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:26:06.000000 tencentcloud-sdk-python-cme-3.0.940/tencentcloud/cme/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:26:06.000000 tencentcloud-sdk-python-cme-3.0.940/tencentcloud/cme/v20191029/
+-rw-r--r--   0 root         (0) root         (0)    55451 2023-07-21 00:26:06.000000 tencentcloud-sdk-python-cme-3.0.940/tencentcloud/cme/v20191029/cme_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 00:26:06.000000 tencentcloud-sdk-python-cme-3.0.940/tencentcloud/cme/v20191029/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8415 2023-07-21 00:26:06.000000 tencentcloud-sdk-python-cme-3.0.940/tencentcloud/cme/v20191029/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   444800 2023-07-21 00:26:06.000000 tencentcloud-sdk-python-cme-3.0.940/tencentcloud/cme/v20191029/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 00:26:06.000000 tencentcloud-sdk-python-cme-3.0.940/tencentcloud/cme/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-21 00:26:06.000000 tencentcloud-sdk-python-cme-3.0.940/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:26:06.000000 tencentcloud-sdk-python-cme-3.0.940/tencentcloud_sdk_python_cme.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 00:26:06.000000 tencentcloud-sdk-python-cme-3.0.940/tencentcloud_sdk_python_cme.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-21 00:26:06.000000 tencentcloud-sdk-python-cme-3.0.940/tencentcloud_sdk_python_cme.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-21 00:26:06.000000 tencentcloud-sdk-python-cme-3.0.940/tencentcloud_sdk_python_cme.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-21 00:26:06.000000 tencentcloud-sdk-python-cme-3.0.940/tencentcloud_sdk_python_cme.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-21 00:26:06.000000 tencentcloud-sdk-python-cme-3.0.940/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-21 00:26:06.000000 tencentcloud-sdk-python-cme-3.0.940/README.rst
```

### Comparing `tencentcloud-sdk-python-cme-3.0.939/setup.py` & `tencentcloud-sdk-python-cme-3.0.940/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cme-3.0.939/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cme-3.0.940/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cme-3.0.939/tencentcloud/cme/v20191029/cme_client.py` & `tencentcloud-sdk-python-cme-3.0.940/tencentcloud/cme/v20191029/cme_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cme-3.0.939/tencentcloud/cme/v20191029/errorcodes.py` & `tencentcloud-sdk-python-cme-3.0.940/tencentcloud/cme/v20191029/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cme-3.0.939/tencentcloud/cme/v20191029/models.py` & `tencentcloud-sdk-python-cme-3.0.940/tencentcloud/cme/v20191029/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -8369,22 +8369,25 @@
         :type OutputMediaSetting: :class:`tencentcloud.cme.v20191029.models.MediaCastOutputMediaSetting`
         :param _PlaySetting: 播放参数。
         :type PlaySetting: :class:`tencentcloud.cme.v20191029.models.MediaCastPlaySetting`
         :param _StartTime: 项目启动时间。采用 [ISO 日期格式](https://cloud.tencent.com/document/product/266/11732#I)。
         :type StartTime: str
         :param _StopTime: 项目结束时间。采用 [ISO 日期格式](https://cloud.tencent.com/document/product/266/11732#I)。如果项目还在运行中，该字段为空。
         :type StopTime: str
+        :param _Duration: 推流时长，单位：秒。项目结束后，返回上次项目运行时的推流时长。如果项目是 Working 状态，返回的时长是0。
+        :type Duration: float
         """
         self._Status = None
         self._SourceInfos = None
         self._DestinationInfos = None
         self._OutputMediaSetting = None
         self._PlaySetting = None
         self._StartTime = None
         self._StopTime = None
+        self._Duration = None
 
     @property
     def Status(self):
         return self._Status
 
     @Status.setter
     def Status(self, Status):
@@ -8434,14 +8437,22 @@
     def StopTime(self):
         return self._StopTime
 
     @StopTime.setter
     def StopTime(self, StopTime):
         self._StopTime = StopTime
 
+    @property
+    def Duration(self):
+        return self._Duration
+
+    @Duration.setter
+    def Duration(self, Duration):
+        self._Duration = Duration
+
 
     def _deserialize(self, params):
         self._Status = params.get("Status")
         if params.get("SourceInfos") is not None:
             self._SourceInfos = []
             for item in params.get("SourceInfos"):
                 obj = MediaCastSourceInfo()
@@ -8457,14 +8468,15 @@
             self._OutputMediaSetting = MediaCastOutputMediaSetting()
             self._OutputMediaSetting._deserialize(params.get("OutputMediaSetting"))
         if params.get("PlaySetting") is not None:
             self._PlaySetting = MediaCastPlaySetting()
             self._PlaySetting._deserialize(params.get("PlaySetting"))
         self._StartTime = params.get("StartTime")
         self._StopTime = params.get("StopTime")
+        self._Duration = params.get("Duration")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-cme-3.0.939/tencentcloud_sdk_python_cme.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cme-3.0.940/tencentcloud_sdk_python_cme.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cme
-Version: 3.0.939
+Version: 3.0.940
 Summary: Tencent Cloud Cme SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cme-3.0.939/PKG-INFO` & `tencentcloud-sdk-python-cme-3.0.940/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cme
-Version: 3.0.939
+Version: 3.0.940
 Summary: Tencent Cloud Cme SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cme-3.0.939/README.rst` & `tencentcloud-sdk-python-cme-3.0.940/README.rst`

 * *Files identical despite different names*

