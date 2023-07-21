# Comparing `tmp/tencentcloud-sdk-python-tke-3.0.939.tar.gz` & `tmp/tencentcloud-sdk-python-tke-3.0.940.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tke-3.0.939.tar", last modified: Thu Jul 20 00:35:56 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tke-3.0.940.tar", last modified: Fri Jul 21 00:51:57 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tke-3.0.939.tar` & `tencentcloud-sdk-python-tke-3.0.940.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 00:35:56.000000 tencentcloud-sdk-python-tke-3.0.939/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-20 00:35:56.000000 tencentcloud-sdk-python-tke-3.0.939/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 00:35:56.000000 tencentcloud-sdk-python-tke-3.0.939/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 00:35:56.000000 tencentcloud-sdk-python-tke-3.0.939/tencentcloud/tke/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-20 00:35:56.000000 tencentcloud-sdk-python-tke-3.0.939/tencentcloud/tke/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 00:35:56.000000 tencentcloud-sdk-python-tke-3.0.939/tencentcloud/tke/v20180525/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-20 00:35:56.000000 tencentcloud-sdk-python-tke-3.0.939/tencentcloud/tke/v20180525/__init__.py
--rw-r--r--   0 root         (0) root         (0)   191187 2023-07-20 00:35:56.000000 tencentcloud-sdk-python-tke-3.0.939/tencentcloud/tke/v20180525/tke_client.py
--rw-r--r--   0 root         (0) root         (0)    19591 2023-07-20 00:35:56.000000 tencentcloud-sdk-python-tke-3.0.939/tencentcloud/tke/v20180525/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)  1059069 2023-07-20 00:35:56.000000 tencentcloud-sdk-python-tke-3.0.939/tencentcloud/tke/v20180525/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-20 00:35:56.000000 tencentcloud-sdk-python-tke-3.0.939/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-20 00:35:56.000000 tencentcloud-sdk-python-tke-3.0.939/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-20 00:35:56.000000 tencentcloud-sdk-python-tke-3.0.939/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-20 00:35:56.000000 tencentcloud-sdk-python-tke-3.0.939/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 00:35:56.000000 tencentcloud-sdk-python-tke-3.0.939/tencentcloud_sdk_python_tke.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 00:35:56.000000 tencentcloud-sdk-python-tke-3.0.939/tencentcloud_sdk_python_tke.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-20 00:35:56.000000 tencentcloud-sdk-python-tke-3.0.939/tencentcloud_sdk_python_tke.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-20 00:35:56.000000 tencentcloud-sdk-python-tke-3.0.939/tencentcloud_sdk_python_tke.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-20 00:35:56.000000 tencentcloud-sdk-python-tke-3.0.939/tencentcloud_sdk_python_tke.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:51:57.000000 tencentcloud-sdk-python-tke-3.0.940/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-21 00:51:57.000000 tencentcloud-sdk-python-tke-3.0.940/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:51:57.000000 tencentcloud-sdk-python-tke-3.0.940/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:51:57.000000 tencentcloud-sdk-python-tke-3.0.940/tencentcloud/tke/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 00:51:57.000000 tencentcloud-sdk-python-tke-3.0.940/tencentcloud/tke/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:51:57.000000 tencentcloud-sdk-python-tke-3.0.940/tencentcloud/tke/v20180525/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 00:51:57.000000 tencentcloud-sdk-python-tke-3.0.940/tencentcloud/tke/v20180525/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   191187 2023-07-21 00:51:57.000000 tencentcloud-sdk-python-tke-3.0.940/tencentcloud/tke/v20180525/tke_client.py
+-rw-r--r--   0 root         (0) root         (0)    19591 2023-07-21 00:51:57.000000 tencentcloud-sdk-python-tke-3.0.940/tencentcloud/tke/v20180525/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)  1059143 2023-07-21 00:51:57.000000 tencentcloud-sdk-python-tke-3.0.940/tencentcloud/tke/v20180525/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-21 00:51:57.000000 tencentcloud-sdk-python-tke-3.0.940/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-21 00:51:57.000000 tencentcloud-sdk-python-tke-3.0.940/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-21 00:51:57.000000 tencentcloud-sdk-python-tke-3.0.940/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-21 00:51:57.000000 tencentcloud-sdk-python-tke-3.0.940/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:51:57.000000 tencentcloud-sdk-python-tke-3.0.940/tencentcloud_sdk_python_tke.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 00:51:57.000000 tencentcloud-sdk-python-tke-3.0.940/tencentcloud_sdk_python_tke.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-21 00:51:57.000000 tencentcloud-sdk-python-tke-3.0.940/tencentcloud_sdk_python_tke.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-21 00:51:57.000000 tencentcloud-sdk-python-tke-3.0.940/tencentcloud_sdk_python_tke.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-21 00:51:57.000000 tencentcloud-sdk-python-tke-3.0.940/tencentcloud_sdk_python_tke.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-tke-3.0.939/setup.py` & `tencentcloud-sdk-python-tke-3.0.940/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tke-3.0.939/tencentcloud/tke/v20180525/tke_client.py` & `tencentcloud-sdk-python-tke-3.0.940/tencentcloud/tke/v20180525/tke_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tke-3.0.939/tencentcloud/tke/v20180525/errorcodes.py` & `tencentcloud-sdk-python-tke-3.0.940/tencentcloud/tke/v20180525/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tke-3.0.939/tencentcloud/tke/v20180525/models.py` & `tencentcloud-sdk-python-tke-3.0.940/tencentcloud/tke/v20180525/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -23892,15 +23892,15 @@
     """
 
     def __init__(self):
         r"""
         :param _DesiredPodNumber: 该节点属于podCIDR大小自定义模式时，可指定节点上运行的pod数量上限
 注意：此字段可能返回 null，表示取不到有效值。
         :type DesiredPodNumber: int
-        :param _GPUArgs: GPU驱动相关参数
+        :param _GPUArgs: GPU驱动相关参数,相关的GPU参数获取:https://cloud.tencent.com/document/api/213/15715
 注意：此字段可能返回 null，表示取不到有效值。
         :type GPUArgs: :class:`tencentcloud.tke.v20180525.models.GPUArgs`
         :param _PreStartUserScript: base64 编码的用户脚本，在初始化节点之前执行，目前只对添加已有节点生效
 注意：此字段可能返回 null，表示取不到有效值。
         :type PreStartUserScript: str
         :param _Taints: 节点污点
 注意：此字段可能返回 null，表示取不到有效值。
```

### Comparing `tencentcloud-sdk-python-tke-3.0.939/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tke-3.0.940/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tke-3.0.939/PKG-INFO` & `tencentcloud-sdk-python-tke-3.0.940/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tke
-Version: 3.0.939
+Version: 3.0.940
 Summary: Tencent Cloud Tke SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tke-3.0.939/README.rst` & `tencentcloud-sdk-python-tke-3.0.940/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tke-3.0.939/tencentcloud_sdk_python_tke.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tke-3.0.940/tencentcloud_sdk_python_tke.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tke
-Version: 3.0.939
+Version: 3.0.940
 Summary: Tencent Cloud Tke SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

