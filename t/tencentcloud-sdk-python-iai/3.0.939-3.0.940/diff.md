# Comparing `tmp/tencentcloud-sdk-python-iai-3.0.939.tar.gz` & `tmp/tencentcloud-sdk-python-iai-3.0.940.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-iai-3.0.939.tar", last modified: Thu Jul 20 00:25:20 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-iai-3.0.940.tar", last modified: Fri Jul 21 00:32:23 2023, max compression
```

## Comparing `tencentcloud-sdk-python-iai-3.0.939.tar` & `tencentcloud-sdk-python-iai-3.0.940.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 00:25:20.000000 tencentcloud-sdk-python-iai-3.0.939/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 00:25:20.000000 tencentcloud-sdk-python-iai-3.0.939/tencentcloud_sdk_python_iai.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 00:25:20.000000 tencentcloud-sdk-python-iai-3.0.939/tencentcloud_sdk_python_iai.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      603 2023-07-20 00:25:20.000000 tencentcloud-sdk-python-iai-3.0.939/tencentcloud_sdk_python_iai.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-20 00:25:20.000000 tencentcloud-sdk-python-iai-3.0.939/tencentcloud_sdk_python_iai.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-20 00:25:20.000000 tencentcloud-sdk-python-iai-3.0.939/tencentcloud_sdk_python_iai.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-20 00:25:20.000000 tencentcloud-sdk-python-iai-3.0.939/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 00:25:20.000000 tencentcloud-sdk-python-iai-3.0.939/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 00:25:20.000000 tencentcloud-sdk-python-iai-3.0.939/tencentcloud/iai/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 00:25:20.000000 tencentcloud-sdk-python-iai-3.0.939/tencentcloud/iai/v20200303/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-20 00:25:20.000000 tencentcloud-sdk-python-iai-3.0.939/tencentcloud/iai/v20200303/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12105 2023-07-20 00:25:20.000000 tencentcloud-sdk-python-iai-3.0.939/tencentcloud/iai/v20200303/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    49515 2023-07-20 00:25:20.000000 tencentcloud-sdk-python-iai-3.0.939/tencentcloud/iai/v20200303/iai_client.py
--rw-r--r--   0 root         (0) root         (0)   250300 2023-07-20 00:25:20.000000 tencentcloud-sdk-python-iai-3.0.939/tencentcloud/iai/v20200303/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 00:25:20.000000 tencentcloud-sdk-python-iai-3.0.939/tencentcloud/iai/v20180301/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-20 00:25:20.000000 tencentcloud-sdk-python-iai-3.0.939/tencentcloud/iai/v20180301/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11999 2023-07-20 00:25:20.000000 tencentcloud-sdk-python-iai-3.0.939/tencentcloud/iai/v20180301/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    46291 2023-07-20 00:25:20.000000 tencentcloud-sdk-python-iai-3.0.939/tencentcloud/iai/v20180301/iai_client.py
--rw-r--r--   0 root         (0) root         (0)   236125 2023-07-20 00:25:20.000000 tencentcloud-sdk-python-iai-3.0.939/tencentcloud/iai/v20180301/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-20 00:25:20.000000 tencentcloud-sdk-python-iai-3.0.939/tencentcloud/iai/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-20 00:25:20.000000 tencentcloud-sdk-python-iai-3.0.939/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-20 00:25:20.000000 tencentcloud-sdk-python-iai-3.0.939/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-20 00:25:20.000000 tencentcloud-sdk-python-iai-3.0.939/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-20 00:25:20.000000 tencentcloud-sdk-python-iai-3.0.939/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:32:23.000000 tencentcloud-sdk-python-iai-3.0.940/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:32:23.000000 tencentcloud-sdk-python-iai-3.0.940/tencentcloud_sdk_python_iai.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 00:32:23.000000 tencentcloud-sdk-python-iai-3.0.940/tencentcloud_sdk_python_iai.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      603 2023-07-21 00:32:23.000000 tencentcloud-sdk-python-iai-3.0.940/tencentcloud_sdk_python_iai.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-21 00:32:23.000000 tencentcloud-sdk-python-iai-3.0.940/tencentcloud_sdk_python_iai.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-21 00:32:23.000000 tencentcloud-sdk-python-iai-3.0.940/tencentcloud_sdk_python_iai.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-21 00:32:23.000000 tencentcloud-sdk-python-iai-3.0.940/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:32:23.000000 tencentcloud-sdk-python-iai-3.0.940/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:32:23.000000 tencentcloud-sdk-python-iai-3.0.940/tencentcloud/iai/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:32:23.000000 tencentcloud-sdk-python-iai-3.0.940/tencentcloud/iai/v20200303/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 00:32:23.000000 tencentcloud-sdk-python-iai-3.0.940/tencentcloud/iai/v20200303/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12105 2023-07-21 00:32:23.000000 tencentcloud-sdk-python-iai-3.0.940/tencentcloud/iai/v20200303/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    49515 2023-07-21 00:32:23.000000 tencentcloud-sdk-python-iai-3.0.940/tencentcloud/iai/v20200303/iai_client.py
+-rw-r--r--   0 root         (0) root         (0)   250300 2023-07-21 00:32:23.000000 tencentcloud-sdk-python-iai-3.0.940/tencentcloud/iai/v20200303/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:32:23.000000 tencentcloud-sdk-python-iai-3.0.940/tencentcloud/iai/v20180301/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 00:32:23.000000 tencentcloud-sdk-python-iai-3.0.940/tencentcloud/iai/v20180301/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11999 2023-07-21 00:32:23.000000 tencentcloud-sdk-python-iai-3.0.940/tencentcloud/iai/v20180301/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    46291 2023-07-21 00:32:23.000000 tencentcloud-sdk-python-iai-3.0.940/tencentcloud/iai/v20180301/iai_client.py
+-rw-r--r--   0 root         (0) root         (0)   236119 2023-07-21 00:32:23.000000 tencentcloud-sdk-python-iai-3.0.940/tencentcloud/iai/v20180301/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 00:32:23.000000 tencentcloud-sdk-python-iai-3.0.940/tencentcloud/iai/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-21 00:32:23.000000 tencentcloud-sdk-python-iai-3.0.940/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-21 00:32:23.000000 tencentcloud-sdk-python-iai-3.0.940/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-21 00:32:23.000000 tencentcloud-sdk-python-iai-3.0.940/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-21 00:32:23.000000 tencentcloud-sdk-python-iai-3.0.940/README.rst
```

### Comparing `tencentcloud-sdk-python-iai-3.0.939/tencentcloud_sdk_python_iai.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-iai-3.0.940/tencentcloud_sdk_python_iai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iai-3.0.939/tencentcloud_sdk_python_iai.egg-info/PKG-INFO` & `tencentcloud-sdk-python-iai-3.0.940/tencentcloud_sdk_python_iai.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-iai
-Version: 3.0.939
+Version: 3.0.940
 Summary: Tencent Cloud Iai SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-iai-3.0.939/setup.py` & `tencentcloud-sdk-python-iai-3.0.940/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iai-3.0.939/tencentcloud/iai/v20200303/errorcodes.py` & `tencentcloud-sdk-python-iai-3.0.940/tencentcloud/iai/v20200303/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iai-3.0.939/tencentcloud/iai/v20200303/iai_client.py` & `tencentcloud-sdk-python-iai-3.0.940/tencentcloud/iai/v20200303/iai_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iai-3.0.939/tencentcloud/iai/v20200303/models.py` & `tencentcloud-sdk-python-iai-3.0.940/tencentcloud/iai/v20200303/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iai-3.0.939/tencentcloud/iai/v20180301/errorcodes.py` & `tencentcloud-sdk-python-iai-3.0.940/tencentcloud/iai/v20180301/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iai-3.0.939/tencentcloud/iai/v20180301/iai_client.py` & `tencentcloud-sdk-python-iai-3.0.940/tencentcloud/iai/v20180301/iai_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iai-3.0.939/tencentcloud/iai/v20180301/models.py` & `tencentcloud-sdk-python-iai-3.0.940/tencentcloud/iai/v20180301/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -2840,15 +2840,15 @@
     若 FaceAttributesType 没有输入相关类型，则FaceDetaiAttributesInfo返回的细项不具备参考意义。
 
     """
 
     def __init__(self):
         r"""
         :param _Age: 年龄 [0,65]，其中65代表“65岁及以上”。 
-FaceAttributesType 不为含Age 或检测超过 5 张人脸时，此参数仍返回，但不具备参考意义。
+FaceAttributesType 不含Age 或检测超过 5 张人脸时，此参数仍返回，但不具备参考意义。
         :type Age: int
         :param _Beauty: 美丑打分[0,100]。 
 FaceAttributesType 不含 Beauty 或检测超过 5 张人脸时，此参数仍返回，但不具备参考意义。
         :type Beauty: int
         :param _Emotion: 情绪，可识别自然、高兴、惊讶、生气、悲伤、厌恶、害怕。 
 AttributeItem对应的Type为 —— 0：自然，1：高兴，2：惊讶，3：生气，4：悲伤，5：厌恶，6：害怕
 FaceAttributesType 不含Emotion 或检测超过 5 张人脸时，此参数仍返回，但不具备参考意义。
@@ -4941,15 +4941,15 @@
 
     def __init__(self):
         r"""
         :param _Style: 帽子佩戴状态信息。
 AttributeItem对应的Type为 —— 0：不戴帽子，1：普通帽子，2：头盔，3：保安帽。
         :type Style: :class:`tencentcloud.iai.v20180301.models.AttributeItem`
         :param _Color: 帽子颜色。
-AttributeItem对应的Type为 —— 0：不戴帽子，1：红色系，2：黄色系，3：蓝色系，4：黑色系，5：灰白色系，6：混色系子。
+AttributeItem对应的Type为 —— 0：不戴帽子，1：红色系，2：黄色系，3：蓝色系，4：黑色系，5：灰白色系，6：混色系。
         :type Color: :class:`tencentcloud.iai.v20180301.models.AttributeItem`
         """
         self._Style = None
         self._Color = None
 
     @property
     def Style(self):
```

### Comparing `tencentcloud-sdk-python-iai-3.0.939/tencentcloud/__init__.py` & `tencentcloud-sdk-python-iai-3.0.940/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-iai-3.0.939/PKG-INFO` & `tencentcloud-sdk-python-iai-3.0.940/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-iai
-Version: 3.0.939
+Version: 3.0.940
 Summary: Tencent Cloud Iai SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-iai-3.0.939/README.rst` & `tencentcloud-sdk-python-iai-3.0.940/README.rst`

 * *Files identical despite different names*

