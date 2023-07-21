# Comparing `tmp/tencentcloud-sdk-python-faceid-3.0.939.tar.gz` & `tmp/tencentcloud-sdk-python-faceid-3.0.940.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-faceid-3.0.939.tar", last modified: Thu Jul 20 00:24:20 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-faceid-3.0.940.tar", last modified: Fri Jul 21 00:29:14 2023, max compression
```

## Comparing `tencentcloud-sdk-python-faceid-3.0.939.tar` & `tencentcloud-sdk-python-faceid-3.0.940.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 00:24:20.000000 tencentcloud-sdk-python-faceid-3.0.939/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 00:24:20.000000 tencentcloud-sdk-python-faceid-3.0.939/tencentcloud_sdk_python_faceid.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 00:24:20.000000 tencentcloud-sdk-python-faceid-3.0.939/tencentcloud_sdk_python_faceid.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      475 2023-07-20 00:24:20.000000 tencentcloud-sdk-python-faceid-3.0.939/tencentcloud_sdk_python_faceid.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1674 2023-07-20 00:24:20.000000 tencentcloud-sdk-python-faceid-3.0.939/tencentcloud_sdk_python_faceid.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-20 00:24:20.000000 tencentcloud-sdk-python-faceid-3.0.939/tencentcloud_sdk_python_faceid.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1012 2023-07-20 00:24:20.000000 tencentcloud-sdk-python-faceid-3.0.939/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 00:24:20.000000 tencentcloud-sdk-python-faceid-3.0.939/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-20 00:24:20.000000 tencentcloud-sdk-python-faceid-3.0.939/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 00:24:20.000000 tencentcloud-sdk-python-faceid-3.0.939/tencentcloud/faceid/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 00:24:20.000000 tencentcloud-sdk-python-faceid-3.0.939/tencentcloud/faceid/v20180301/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-20 00:24:20.000000 tencentcloud-sdk-python-faceid-3.0.939/tencentcloud/faceid/v20180301/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9370 2023-07-20 00:24:20.000000 tencentcloud-sdk-python-faceid-3.0.939/tencentcloud/faceid/v20180301/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    34162 2023-07-20 00:24:20.000000 tencentcloud-sdk-python-faceid-3.0.939/tencentcloud/faceid/v20180301/faceid_client.py
--rw-r--r--   0 root         (0) root         (0)   212180 2023-07-20 00:24:20.000000 tencentcloud-sdk-python-faceid-3.0.939/tencentcloud/faceid/v20180301/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-20 00:24:20.000000 tencentcloud-sdk-python-faceid-3.0.939/tencentcloud/faceid/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-20 00:24:20.000000 tencentcloud-sdk-python-faceid-3.0.939/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1674 2023-07-20 00:24:20.000000 tencentcloud-sdk-python-faceid-3.0.939/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      746 2023-07-20 00:24:20.000000 tencentcloud-sdk-python-faceid-3.0.939/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:29:14.000000 tencentcloud-sdk-python-faceid-3.0.940/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:29:14.000000 tencentcloud-sdk-python-faceid-3.0.940/tencentcloud_sdk_python_faceid.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 00:29:14.000000 tencentcloud-sdk-python-faceid-3.0.940/tencentcloud_sdk_python_faceid.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      475 2023-07-21 00:29:14.000000 tencentcloud-sdk-python-faceid-3.0.940/tencentcloud_sdk_python_faceid.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-07-21 00:29:14.000000 tencentcloud-sdk-python-faceid-3.0.940/tencentcloud_sdk_python_faceid.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-21 00:29:14.000000 tencentcloud-sdk-python-faceid-3.0.940/tencentcloud_sdk_python_faceid.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1012 2023-07-21 00:29:14.000000 tencentcloud-sdk-python-faceid-3.0.940/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:29:14.000000 tencentcloud-sdk-python-faceid-3.0.940/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-21 00:29:14.000000 tencentcloud-sdk-python-faceid-3.0.940/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:29:14.000000 tencentcloud-sdk-python-faceid-3.0.940/tencentcloud/faceid/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:29:14.000000 tencentcloud-sdk-python-faceid-3.0.940/tencentcloud/faceid/v20180301/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 00:29:14.000000 tencentcloud-sdk-python-faceid-3.0.940/tencentcloud/faceid/v20180301/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9370 2023-07-21 00:29:14.000000 tencentcloud-sdk-python-faceid-3.0.940/tencentcloud/faceid/v20180301/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    34162 2023-07-21 00:29:14.000000 tencentcloud-sdk-python-faceid-3.0.940/tencentcloud/faceid/v20180301/faceid_client.py
+-rw-r--r--   0 root         (0) root         (0)   212614 2023-07-21 00:29:14.000000 tencentcloud-sdk-python-faceid-3.0.940/tencentcloud/faceid/v20180301/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 00:29:14.000000 tencentcloud-sdk-python-faceid-3.0.940/tencentcloud/faceid/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-21 00:29:14.000000 tencentcloud-sdk-python-faceid-3.0.940/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-07-21 00:29:14.000000 tencentcloud-sdk-python-faceid-3.0.940/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      746 2023-07-21 00:29:14.000000 tencentcloud-sdk-python-faceid-3.0.940/README.rst
```

### Comparing `tencentcloud-sdk-python-faceid-3.0.939/tencentcloud_sdk_python_faceid.egg-info/PKG-INFO` & `tencentcloud-sdk-python-faceid-3.0.940/tencentcloud_sdk_python_faceid.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-faceid
-Version: 3.0.939
+Version: 3.0.940
 Summary: Tencent Cloud Faceid SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-faceid-3.0.939/setup.py` & `tencentcloud-sdk-python-faceid-3.0.940/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-faceid-3.0.939/tencentcloud/__init__.py` & `tencentcloud-sdk-python-faceid-3.0.940/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-faceid-3.0.939/tencentcloud/faceid/v20180301/errorcodes.py` & `tencentcloud-sdk-python-faceid-3.0.940/tencentcloud/faceid/v20180301/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-faceid-3.0.939/tencentcloud/faceid/v20180301/faceid_client.py` & `tencentcloud-sdk-python-faceid-3.0.940/tencentcloud/faceid/v20180301/faceid_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-faceid-3.0.939/tencentcloud/faceid/v20180301/models.py` & `tencentcloud-sdk-python-faceid-3.0.940/tencentcloud/faceid/v20180301/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -812,15 +812,15 @@
 图片存储于腾讯云的 Url 可保障更高的下载速度和稳定性，建议图片存储于腾讯云。
 非腾讯云存储的 Url 速度和稳定性可能受一定影响。
         :type ImageUrl: str
         :param _Config: 以下可选字段均为bool 类型，默认false：
 CopyWarn，复印件告警
 BorderCheckWarn，边框和框内遮挡告警
 ReshootWarn，翻拍告警
-DetectPsWarn，PS检测告警
+DetectPsWarn，PS检测告警（疑似存在PS痕迹）
 TempIdWarn，临时身份证告警
 Quality，图片质量告警（评价图片模糊程度）
 
 SDK 设置方式参考：
 Config = Json.stringify({"CopyWarn":true,"ReshootWarn":true})
 API 3.0 Explorer 设置方式参考：
 Config = {"CopyWarn":true,"ReshootWarn":true}
@@ -912,15 +912,15 @@
         :param _Warnings: 告警信息，当在Config中配置了告警信息会停止人像比对，Result返回错误（FailedOperation.OcrWarningOccurred）并有此告警信息，Code 告警码列表和释义：
 
 -9101 身份证边框不完整告警，
 -9102 身份证复印件告警，
 -9103 身份证翻拍告警，
 -9105 身份证框内遮挡告警，
 -9104 临时身份证告警，
--9106 身份证 PS 告警。
+-9106 身份证 PS 告警（疑似存在PS痕迹）。
 -8001 图片模糊告警
 多个会 |  隔开如 "-9101|-9106|-9104"
         :type Warnings: str
         :param _Quality: 图片质量分数，当请求Config中配置图片模糊告警该参数才有意义，取值范围（0～100），目前默认阈值是50分，低于50分会触发模糊告警。
         :type Quality: float
         :param _Encryption: 敏感数据加密信息。
 注意：此字段可能返回 null，表示取不到有效值。
@@ -1830,26 +1830,26 @@
         :param _WarnInfos: 身份证人像面告警码，开启身份证告警功能后才会返回，返回数组中可能出现的告警码如下：
 -9100 身份证有效日期不合法告警，
 -9101 身份证边框不完整告警，
 -9102 身份证复印件告警，
 -9103 身份证翻拍告警，
 -9105 身份证框内遮挡告警，
 -9104 临时身份证告警，
--9106 身份证 PS 告警，
+-9106 身份证 PS 告警（疑似存在PS痕迹），
 -9107 身份证反光告警。
 注意：此字段可能返回 null，表示取不到有效值。
         :type WarnInfos: list of int
         :param _BackWarnInfos: 身份证国徽面告警码，开启身份证告警功能后才会返回，返回数组中可能出现的告警码如下：
 -9100 身份证有效日期不合法告警，
 -9101 身份证边框不完整告警，
 -9102 身份证复印件告警，
 -9103 身份证翻拍告警，
 -9105 身份证框内遮挡告警，
 -9104 临时身份证告警，
--9106 身份证 PS 告警，
+-9106 身份证 PS 告警（疑似存在PS痕迹），
 -9107 身份证反光告警。
 注意：此字段可能返回 null，表示取不到有效值。
         :type BackWarnInfos: list of int
         """
         self._OcrFront = None
         self._OcrBack = None
         self._ProcessedFrontImage = None
@@ -2600,22 +2600,27 @@
     """敏感数据加密
 
     """
 
     def __init__(self):
         r"""
         :param _EncryptList: 在使用加密服务时，填入要被加密的字段。本接口中可填入加密后的一个或多个字段
+注意：此字段可能返回 null，表示取不到有效值。
         :type EncryptList: list of str
         :param _CiphertextBlob: 有加密需求的用户，接入传入kms的CiphertextBlob，关于数据加密可查阅<a href="https://cloud.tencent.com/document/product/1007/47180">数据加密</a> 文档。
+注意：此字段可能返回 null，表示取不到有效值。
         :type CiphertextBlob: str
         :param _Iv: 有加密需求的用户，传入CBC加密的初始向量（客户自定义字符串，长度16字符）。
+注意：此字段可能返回 null，表示取不到有效值。
         :type Iv: str
         :param _Algorithm: 加密使用的算法（支持'AES-256-CBC'、'SM4-GCM'），不传默认为'AES-256-CBC'
+注意：此字段可能返回 null，表示取不到有效值。
         :type Algorithm: str
         :param _TagList: SM4-GCM算法生成的消息摘要（校验消息完整性时使用）
+注意：此字段可能返回 null，表示取不到有效值。
         :type TagList: list of str
         """
         self._EncryptList = None
         self._CiphertextBlob = None
         self._Iv = None
         self._Algorithm = None
         self._TagList = None
```

### Comparing `tencentcloud-sdk-python-faceid-3.0.939/PKG-INFO` & `tencentcloud-sdk-python-faceid-3.0.940/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-faceid
-Version: 3.0.939
+Version: 3.0.940
 Summary: Tencent Cloud Faceid SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-faceid-3.0.939/README.rst` & `tencentcloud-sdk-python-faceid-3.0.940/README.rst`

 * *Files identical despite different names*

