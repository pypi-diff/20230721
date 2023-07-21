# Comparing `tmp/tencentcloud-sdk-python-asr-3.0.939.tar.gz` & `tmp/tencentcloud-sdk-python-asr-3.0.940.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-asr-3.0.939.tar", last modified: Thu Jul 20 00:17:30 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-asr-3.0.940.tar", last modified: Fri Jul 21 00:22:18 2023, max compression
```

## Comparing `tencentcloud-sdk-python-asr-3.0.939.tar` & `tencentcloud-sdk-python-asr-3.0.940.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 00:17:30.000000 tencentcloud-sdk-python-asr-3.0.939/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-20 00:17:30.000000 tencentcloud-sdk-python-asr-3.0.939/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 00:17:30.000000 tencentcloud-sdk-python-asr-3.0.939/tencentcloud_sdk_python_asr.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 00:17:30.000000 tencentcloud-sdk-python-asr-3.0.939/tencentcloud_sdk_python_asr.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-20 00:17:30.000000 tencentcloud-sdk-python-asr-3.0.939/tencentcloud_sdk_python_asr.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-20 00:17:30.000000 tencentcloud-sdk-python-asr-3.0.939/tencentcloud_sdk_python_asr.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-20 00:17:30.000000 tencentcloud-sdk-python-asr-3.0.939/tencentcloud_sdk_python_asr.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 00:17:30.000000 tencentcloud-sdk-python-asr-3.0.939/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 00:17:30.000000 tencentcloud-sdk-python-asr-3.0.939/tencentcloud/asr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 00:17:30.000000 tencentcloud-sdk-python-asr-3.0.939/tencentcloud/asr/v20190614/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-20 00:17:30.000000 tencentcloud-sdk-python-asr-3.0.939/tencentcloud/asr/v20190614/__init__.py
--rw-r--r--   0 root         (0) root         (0)    29417 2023-07-20 00:17:30.000000 tencentcloud-sdk-python-asr-3.0.939/tencentcloud/asr/v20190614/asr_client.py
--rw-r--r--   0 root         (0) root         (0)     7480 2023-07-20 00:17:30.000000 tencentcloud-sdk-python-asr-3.0.939/tencentcloud/asr/v20190614/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   111858 2023-07-20 00:17:30.000000 tencentcloud-sdk-python-asr-3.0.939/tencentcloud/asr/v20190614/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-20 00:17:30.000000 tencentcloud-sdk-python-asr-3.0.939/tencentcloud/asr/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-20 00:17:30.000000 tencentcloud-sdk-python-asr-3.0.939/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-20 00:17:30.000000 tencentcloud-sdk-python-asr-3.0.939/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-20 00:17:30.000000 tencentcloud-sdk-python-asr-3.0.939/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-20 00:17:30.000000 tencentcloud-sdk-python-asr-3.0.939/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:22:18.000000 tencentcloud-sdk-python-asr-3.0.940/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-21 00:22:18.000000 tencentcloud-sdk-python-asr-3.0.940/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:22:18.000000 tencentcloud-sdk-python-asr-3.0.940/tencentcloud_sdk_python_asr.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 00:22:18.000000 tencentcloud-sdk-python-asr-3.0.940/tencentcloud_sdk_python_asr.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-21 00:22:18.000000 tencentcloud-sdk-python-asr-3.0.940/tencentcloud_sdk_python_asr.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-21 00:22:18.000000 tencentcloud-sdk-python-asr-3.0.940/tencentcloud_sdk_python_asr.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-21 00:22:18.000000 tencentcloud-sdk-python-asr-3.0.940/tencentcloud_sdk_python_asr.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:22:18.000000 tencentcloud-sdk-python-asr-3.0.940/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:22:18.000000 tencentcloud-sdk-python-asr-3.0.940/tencentcloud/asr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:22:18.000000 tencentcloud-sdk-python-asr-3.0.940/tencentcloud/asr/v20190614/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 00:22:18.000000 tencentcloud-sdk-python-asr-3.0.940/tencentcloud/asr/v20190614/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    29417 2023-07-21 00:22:18.000000 tencentcloud-sdk-python-asr-3.0.940/tencentcloud/asr/v20190614/asr_client.py
+-rw-r--r--   0 root         (0) root         (0)     7480 2023-07-21 00:22:18.000000 tencentcloud-sdk-python-asr-3.0.940/tencentcloud/asr/v20190614/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   111945 2023-07-21 00:22:18.000000 tencentcloud-sdk-python-asr-3.0.940/tencentcloud/asr/v20190614/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 00:22:18.000000 tencentcloud-sdk-python-asr-3.0.940/tencentcloud/asr/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-21 00:22:18.000000 tencentcloud-sdk-python-asr-3.0.940/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-21 00:22:18.000000 tencentcloud-sdk-python-asr-3.0.940/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-21 00:22:18.000000 tencentcloud-sdk-python-asr-3.0.940/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-21 00:22:18.000000 tencentcloud-sdk-python-asr-3.0.940/README.rst
```

### Comparing `tencentcloud-sdk-python-asr-3.0.939/setup.py` & `tencentcloud-sdk-python-asr-3.0.940/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-asr-3.0.939/tencentcloud_sdk_python_asr.egg-info/PKG-INFO` & `tencentcloud-sdk-python-asr-3.0.940/tencentcloud_sdk_python_asr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-asr
-Version: 3.0.939
+Version: 3.0.940
 Summary: Tencent Cloud Asr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-asr-3.0.939/tencentcloud/asr/v20190614/asr_client.py` & `tencentcloud-sdk-python-asr-3.0.940/tencentcloud/asr/v20190614/asr_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-asr-3.0.939/tencentcloud/asr/v20190614/errorcodes.py` & `tencentcloud-sdk-python-asr-3.0.940/tencentcloud/asr/v20190614/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-asr-3.0.939/tencentcloud/asr/v20190614/models.py` & `tencentcloud-sdk-python-asr-3.0.940/tencentcloud/asr/v20190614/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -285,14 +285,15 @@
 • 16k_yue：粤语；
 • 16k_id：印度尼西亚语；
 • 16k_fil：菲律宾语；
 • 16k_th：泰语；
 • 16k_pt：葡萄牙语；
 • 16k_tr：土耳其语；
 • 16k_ar：阿拉伯语；
+• 16k_es：西班牙语；
         :type EngineType: str
         :param _Url: 语音流地址，支持rtmp、rtsp等流媒体协议，以及各类基于http协议的直播流(不支持hls, m3u8)
         :type Url: str
         :param _CallbackUrl: 支持HTTP和HTTPS协议，用于接收识别结果，您需要自行搭建公网可调用的服务。回调格式&内容详见：[语音流异步识别回调说明](https://cloud.tencent.com/document/product/1093/52633)
         :type CallbackUrl: str
         :param _SignToken: 用于生成回调通知中的签名
         :type SignToken: str
@@ -603,14 +604,15 @@
 • 16k_ms：马来语；
 • 16k_id：印度尼西亚语；
 • 16k_fil：菲律宾语；
 • 16k_th：泰语；
 • 16k_pt：葡萄牙语；
 • 16k_tr：土耳其语；
 • 16k_ar：阿拉伯语；
+• 16k_es：西班牙语；
 • 16k_zh_dialect：多方言，支持23种方言（上海话、四川话、武汉话、贵阳话、昆明话、西安话、郑州话、太原话、兰州话、银川话、西宁话、南京话、合肥话、南昌话、长沙话、苏州话、杭州话、济南话、天津话、石家庄话、黑龙江话、吉林话、辽宁话）；
         :type EngineModelType: str
         :param _ChannelNum: 识别声道数。1：单声道（非电话场景，直接选择单声道即可，忽略音频声道数）；2：双声道（仅支持8k_zh电话场景，双声道应分别对应通话双方）。注意：双声道的电话音频已物理分离说话人，无需再开启说话人分离功能。
         :type ChannelNum: int
         :param _ResTextFormat: 识别结果返回形式。0： 识别结果文本(含分段时间戳)； 1：词级别粒度的[详细识别结果](https://cloud.tencent.com/document/api/1093/37824#SentenceDetail)(不含标点，含语速值)；2：词级别粒度的详细识别结果（包含标点、语速值）；3: 标点符号分段，包含每段时间戳，特别适用于字幕场景（包含词级时间、标点、语速值）。4：【增值付费功能】对识别结果按照语义分段，并展示词级别粒度的详细识别结果，仅支持8k_zh、16k_zh引擎，需购买对应资源包使用（注意：如果账号后付费功能开启并使用此功能，将[自动计费](https://cloud.tencent.com/document/product/1093/35686)）
         :type ResTextFormat: int
         :param _SourceType: 语音数据来源。0：语音 URL；1：语音数据（post body）。
@@ -2282,14 +2284,15 @@
 • 16k_ms：马来语；
 • 16k_id：印度尼西亚语；
 • 16k_fil：菲律宾语；
 • 16k_th：泰语；
 • 16k_pt：葡萄牙语；
 • 16k_tr：土耳其语；
 • 16k_ar：阿拉伯语；
+• 16k_es：西班牙语；
 • 16k_zh_dialect：多方言，支持23种方言（上海话、四川话、武汉话、贵阳话、昆明话、西安话、郑州话、太原话、兰州话、银川话、西宁话、南京话、合肥话、南昌话、长沙话、苏州话、杭州话、济南话、天津话、石家庄话、黑龙江话、吉林话、辽宁话）；
         :type EngSerViceType: str
         :param _SourceType: 语音数据来源。0：语音 URL；1：语音数据（post body）。
         :type SourceType: int
         :param _VoiceFormat: 识别音频的音频格式，支持wav、pcm、ogg-opus、speex、silk、mp3、m4a、aac、amr。
         :type VoiceFormat: str
         :param _ProjectId: 腾讯云项目 ID，废弃参数，填写0即可。
```

### Comparing `tencentcloud-sdk-python-asr-3.0.939/tencentcloud/__init__.py` & `tencentcloud-sdk-python-asr-3.0.940/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-asr-3.0.939/PKG-INFO` & `tencentcloud-sdk-python-asr-3.0.940/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-asr
-Version: 3.0.939
+Version: 3.0.940
 Summary: Tencent Cloud Asr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-asr-3.0.939/README.rst` & `tencentcloud-sdk-python-asr-3.0.940/README.rst`

 * *Files identical despite different names*

