# Comparing `tmp/tencentcloud-sdk-python-trtc-3.0.939.tar.gz` & `tmp/tencentcloud-sdk-python-trtc-3.0.940.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-trtc-3.0.939.tar", last modified: Thu Jul 20 00:36:34 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-trtc-3.0.940.tar", last modified: Fri Jul 21 00:52:40 2023, max compression
```

## Comparing `tencentcloud-sdk-python-trtc-3.0.939.tar` & `tencentcloud-sdk-python-trtc-3.0.940.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 00:36:34.000000 tencentcloud-sdk-python-trtc-3.0.939/
--rw-r--r--   0 root         (0) root         (0)     1008 2023-07-20 00:36:34.000000 tencentcloud-sdk-python-trtc-3.0.939/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 00:36:34.000000 tencentcloud-sdk-python-trtc-3.0.939/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 00:36:34.000000 tencentcloud-sdk-python-trtc-3.0.939/tencentcloud/trtc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 00:36:34.000000 tencentcloud-sdk-python-trtc-3.0.939/tencentcloud/trtc/v20190722/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-20 00:36:34.000000 tencentcloud-sdk-python-trtc-3.0.939/tencentcloud/trtc/v20190722/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9679 2023-07-20 00:36:34.000000 tencentcloud-sdk-python-trtc-3.0.939/tencentcloud/trtc/v20190722/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    65744 2023-07-20 00:36:34.000000 tencentcloud-sdk-python-trtc-3.0.939/tencentcloud/trtc/v20190722/trtc_client.py
--rw-r--r--   0 root         (0) root         (0)   287958 2023-07-20 00:36:34.000000 tencentcloud-sdk-python-trtc-3.0.939/tencentcloud/trtc/v20190722/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-20 00:36:34.000000 tencentcloud-sdk-python-trtc-3.0.939/tencentcloud/trtc/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-20 00:36:34.000000 tencentcloud-sdk-python-trtc-3.0.939/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-20 00:36:34.000000 tencentcloud-sdk-python-trtc-3.0.939/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-20 00:36:34.000000 tencentcloud-sdk-python-trtc-3.0.939/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      740 2023-07-20 00:36:34.000000 tencentcloud-sdk-python-trtc-3.0.939/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 00:36:34.000000 tencentcloud-sdk-python-trtc-3.0.939/tencentcloud_sdk_python_trtc.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 00:36:34.000000 tencentcloud-sdk-python-trtc-3.0.939/tencentcloud_sdk_python_trtc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-07-20 00:36:34.000000 tencentcloud-sdk-python-trtc-3.0.939/tencentcloud_sdk_python_trtc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-20 00:36:34.000000 tencentcloud-sdk-python-trtc-3.0.939/tencentcloud_sdk_python_trtc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-20 00:36:34.000000 tencentcloud-sdk-python-trtc-3.0.939/tencentcloud_sdk_python_trtc.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:52:40.000000 tencentcloud-sdk-python-trtc-3.0.940/
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-07-21 00:52:40.000000 tencentcloud-sdk-python-trtc-3.0.940/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:52:40.000000 tencentcloud-sdk-python-trtc-3.0.940/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:52:40.000000 tencentcloud-sdk-python-trtc-3.0.940/tencentcloud/trtc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:52:40.000000 tencentcloud-sdk-python-trtc-3.0.940/tencentcloud/trtc/v20190722/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 00:52:40.000000 tencentcloud-sdk-python-trtc-3.0.940/tencentcloud/trtc/v20190722/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9679 2023-07-21 00:52:40.000000 tencentcloud-sdk-python-trtc-3.0.940/tencentcloud/trtc/v20190722/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    65738 2023-07-21 00:52:40.000000 tencentcloud-sdk-python-trtc-3.0.940/tencentcloud/trtc/v20190722/trtc_client.py
+-rw-r--r--   0 root         (0) root         (0)   287958 2023-07-21 00:52:40.000000 tencentcloud-sdk-python-trtc-3.0.940/tencentcloud/trtc/v20190722/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 00:52:40.000000 tencentcloud-sdk-python-trtc-3.0.940/tencentcloud/trtc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-21 00:52:40.000000 tencentcloud-sdk-python-trtc-3.0.940/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-21 00:52:40.000000 tencentcloud-sdk-python-trtc-3.0.940/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-21 00:52:40.000000 tencentcloud-sdk-python-trtc-3.0.940/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      740 2023-07-21 00:52:40.000000 tencentcloud-sdk-python-trtc-3.0.940/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:52:40.000000 tencentcloud-sdk-python-trtc-3.0.940/tencentcloud_sdk_python_trtc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 00:52:40.000000 tencentcloud-sdk-python-trtc-3.0.940/tencentcloud_sdk_python_trtc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-07-21 00:52:40.000000 tencentcloud-sdk-python-trtc-3.0.940/tencentcloud_sdk_python_trtc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-21 00:52:40.000000 tencentcloud-sdk-python-trtc-3.0.940/tencentcloud_sdk_python_trtc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-21 00:52:40.000000 tencentcloud-sdk-python-trtc-3.0.940/tencentcloud_sdk_python_trtc.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-trtc-3.0.939/setup.py` & `tencentcloud-sdk-python-trtc-3.0.940/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-trtc-3.0.939/tencentcloud/trtc/v20190722/errorcodes.py` & `tencentcloud-sdk-python-trtc-3.0.940/tencentcloud/trtc/v20190722/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-trtc-3.0.939/tencentcloud/trtc/v20190722/trtc_client.py` & `tencentcloud-sdk-python-trtc-3.0.940/tencentcloud/trtc/v20190722/trtc_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -874,15 +874,15 @@
         3、设置多个cdn转推的目的地址，一个转推任务最多可以同时设置10个cdn转推地址，如果您需要转推非腾讯云的cdn地址时，需要联系腾讯云开通能力。
         4、设置多个回推房间列表，一个转推任务最多可以同时将混流回推到10个TRTC房间。
 
         目前已经支持如下几种布局模版，其中动态布局模版（悬浮模板、九宫格模板、屏幕分享模板）只支持单个TRTC房间，自定义模版支持混合多个TRTC房间内的音视频流。具体说明如下：
         1、悬浮模板：第一个进入房间的用户的视频画面会铺满整个屏幕，其他用户的视频画面从左下角依次水平排列，显示为小画面，最多4行，每行4个，小画面悬浮于大画面之上。最多支持1个大画面和15个小画面，如果用户只发送音频默认不占布局配置，也支持设置。每个子画面默认采用居中裁剪的方式进行渲染，也支持统一设置子画面的渲染方式。
         2、九宫格模板：所有用户的视频画面大小一致，平分整个屏幕，人数越多，每个画面的尺寸越小。最多支持16个画面，如果用户只发送音频，默认不占布局配置，也支持设置。每个子画面默认采用居中裁剪的方式进行渲染，也支持统一设置子画面的渲染方式。
         3、屏幕分享模板：适合视频会议和在线教育场景的布局，屏幕分享（或者主讲的摄像头）始终占据屏幕左侧的大画面位置，需要您明确设置占据大画面的混流用户信息。其他用户依次垂直排列于右侧，最多两列，每列最多8个小画面。最多支持1个大画面和15个小画面。若上行分辨率宽高比与画面输出宽高比不一致时，左侧大画面为了保持内容的完整性采用缩放方式处理，右侧小画面采用裁剪方式处理，也支持统一设置子画面的渲染方式。
-        4、自定义布局模版：支持您主动根据业务需要设置布局位置，每个预设的布局位置支持具名设置（具名设置需要明确指定房间号和用户名）和不具名设置。当一个子画面具名设置时，该位置就为该用户预留，用户进房且上行音视频数据时会自动占据该位置，其它用户不会占据该位置。当预设的布局位置未具名时，排版引擎引擎会根据进房间顺序自动填充，预设位置填满时，不再混合其它用户的画面和声音。每个子画面位置支持设置占位图（BackgroundImageUrl），当用户未进房或者只上行音频数据时，该位置画面可显示对应的占位图画面。
+        4、自定义布局模版：支持您主动根据业务需要设置布局位置，每个预设的布局位置支持具名设置（具名设置需要明确指定房间号和用户名）和不具名设置。当一个子画面具名设置时，该位置就为该用户预留，用户进房且上行音视频数据时会自动占据该位置，其它用户不会占据该位置。当预设的布局位置未具名时，排版引擎会根据进房间顺序自动填充，预设位置填满时，不再混合其它用户的画面和声音。每个子画面位置支持设置占位图（BackgroundImageUrl），当用户未进房或者只上行音频数据时，该位置画面可显示对应的占位图画面。
 
         您可以控制台开通旁路转推回调功能实现转推cdn状态的事件监控，具体说明请参考官网文档：[旁路转推回调说明](https://cloud.tencent.com/document/product/647/88552)
         您使用转推api时根据使用特性可能会产生如下费用：
         MCU混流转码费用请参考文档：[云端混流转码计费说明](https://cloud.tencent.com/document/product/647/49446)
         转推非腾讯云CDN费用请参考文档：[云端转推计费说明](https://cloud.tencent.com/document/product/647/82155)
 
         参数的使用说明：
```

### Comparing `tencentcloud-sdk-python-trtc-3.0.939/tencentcloud/trtc/v20190722/models.py` & `tencentcloud-sdk-python-trtc-3.0.940/tencentcloud/trtc/v20190722/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-trtc-3.0.939/tencentcloud/__init__.py` & `tencentcloud-sdk-python-trtc-3.0.940/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-trtc-3.0.939/PKG-INFO` & `tencentcloud-sdk-python-trtc-3.0.940/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-trtc
-Version: 3.0.939
+Version: 3.0.940
 Summary: Tencent Cloud Trtc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-trtc-3.0.939/README.rst` & `tencentcloud-sdk-python-trtc-3.0.940/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-trtc-3.0.939/tencentcloud_sdk_python_trtc.egg-info/PKG-INFO` & `tencentcloud-sdk-python-trtc-3.0.940/tencentcloud_sdk_python_trtc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-trtc
-Version: 3.0.939
+Version: 3.0.940
 Summary: Tencent Cloud Trtc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

