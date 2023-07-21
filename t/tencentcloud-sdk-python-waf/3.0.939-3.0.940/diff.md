# Comparing `tmp/tencentcloud-sdk-python-waf-3.0.939.tar.gz` & `tmp/tencentcloud-sdk-python-waf-3.0.940.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-waf-3.0.939.tar", last modified: Thu Jul 20 00:37:33 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-waf-3.0.940.tar", last modified: Fri Jul 21 00:55:55 2023, max compression
```

## Comparing `tencentcloud-sdk-python-waf-3.0.939.tar` & `tencentcloud-sdk-python-waf-3.0.940.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 00:37:33.000000 tencentcloud-sdk-python-waf-3.0.939/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-20 00:37:33.000000 tencentcloud-sdk-python-waf-3.0.939/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 00:37:33.000000 tencentcloud-sdk-python-waf-3.0.939/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-20 00:37:33.000000 tencentcloud-sdk-python-waf-3.0.939/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 00:37:33.000000 tencentcloud-sdk-python-waf-3.0.939/tencentcloud/waf/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 00:37:33.000000 tencentcloud-sdk-python-waf-3.0.939/tencentcloud/waf/v20180125/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-20 00:37:33.000000 tencentcloud-sdk-python-waf-3.0.939/tencentcloud/waf/v20180125/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3395 2023-07-20 00:37:33.000000 tencentcloud-sdk-python-waf-3.0.939/tencentcloud/waf/v20180125/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    47662 2023-07-20 00:37:33.000000 tencentcloud-sdk-python-waf-3.0.939/tencentcloud/waf/v20180125/waf_client.py
--rw-r--r--   0 root         (0) root         (0)   309127 2023-07-20 00:37:33.000000 tencentcloud-sdk-python-waf-3.0.939/tencentcloud/waf/v20180125/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-20 00:37:33.000000 tencentcloud-sdk-python-waf-3.0.939/tencentcloud/waf/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-20 00:37:33.000000 tencentcloud-sdk-python-waf-3.0.939/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-20 00:37:33.000000 tencentcloud-sdk-python-waf-3.0.939/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 00:37:33.000000 tencentcloud-sdk-python-waf-3.0.939/tencentcloud_sdk_python_waf.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 00:37:33.000000 tencentcloud-sdk-python-waf-3.0.939/tencentcloud_sdk_python_waf.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-20 00:37:33.000000 tencentcloud-sdk-python-waf-3.0.939/tencentcloud_sdk_python_waf.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-20 00:37:33.000000 tencentcloud-sdk-python-waf-3.0.939/tencentcloud_sdk_python_waf.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-20 00:37:33.000000 tencentcloud-sdk-python-waf-3.0.939/tencentcloud_sdk_python_waf.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-20 00:37:33.000000 tencentcloud-sdk-python-waf-3.0.939/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:55:55.000000 tencentcloud-sdk-python-waf-3.0.940/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-21 00:55:55.000000 tencentcloud-sdk-python-waf-3.0.940/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:55:55.000000 tencentcloud-sdk-python-waf-3.0.940/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-21 00:55:55.000000 tencentcloud-sdk-python-waf-3.0.940/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:55:55.000000 tencentcloud-sdk-python-waf-3.0.940/tencentcloud/waf/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:55:55.000000 tencentcloud-sdk-python-waf-3.0.940/tencentcloud/waf/v20180125/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 00:55:55.000000 tencentcloud-sdk-python-waf-3.0.940/tencentcloud/waf/v20180125/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3395 2023-07-21 00:55:55.000000 tencentcloud-sdk-python-waf-3.0.940/tencentcloud/waf/v20180125/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    47662 2023-07-21 00:55:55.000000 tencentcloud-sdk-python-waf-3.0.940/tencentcloud/waf/v20180125/waf_client.py
+-rw-r--r--   0 root         (0) root         (0)   309376 2023-07-21 00:55:55.000000 tencentcloud-sdk-python-waf-3.0.940/tencentcloud/waf/v20180125/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 00:55:55.000000 tencentcloud-sdk-python-waf-3.0.940/tencentcloud/waf/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-21 00:55:55.000000 tencentcloud-sdk-python-waf-3.0.940/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-21 00:55:55.000000 tencentcloud-sdk-python-waf-3.0.940/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:55:55.000000 tencentcloud-sdk-python-waf-3.0.940/tencentcloud_sdk_python_waf.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 00:55:55.000000 tencentcloud-sdk-python-waf-3.0.940/tencentcloud_sdk_python_waf.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-21 00:55:55.000000 tencentcloud-sdk-python-waf-3.0.940/tencentcloud_sdk_python_waf.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-21 00:55:55.000000 tencentcloud-sdk-python-waf-3.0.940/tencentcloud_sdk_python_waf.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-21 00:55:55.000000 tencentcloud-sdk-python-waf-3.0.940/tencentcloud_sdk_python_waf.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-21 00:55:55.000000 tencentcloud-sdk-python-waf-3.0.940/README.rst
```

### Comparing `tencentcloud-sdk-python-waf-3.0.939/setup.py` & `tencentcloud-sdk-python-waf-3.0.940/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-waf-3.0.939/tencentcloud/__init__.py` & `tencentcloud-sdk-python-waf-3.0.940/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-waf-3.0.939/tencentcloud/waf/v20180125/errorcodes.py` & `tencentcloud-sdk-python-waf-3.0.940/tencentcloud/waf/v20180125/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-waf-3.0.939/tencentcloud/waf/v20180125/waf_client.py` & `tencentcloud-sdk-python-waf-3.0.940/tencentcloud/waf/v20180125/waf_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-waf-3.0.939/tencentcloud/waf/v20180125/models.py` & `tencentcloud-sdk-python-waf-3.0.940/tencentcloud/waf/v20180125/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -946,15 +946,15 @@
         :type Domain: str
         :param _Rules: 需要添加的规则
         :type Rules: list of int non-negative
         :param _Url: 需要添加的规则url
         :type Url: str
         :param _Function: 规则的方法
         :type Function: str
-        :param _Status: 规则的开关
+        :param _Status: 规则的开关，0表示规则关闭，1表示规则打开
         :type Status: int
         """
         self._Domain = None
         self._Rules = None
         self._Url = None
         self._Function = None
         self._Status = None
@@ -3689,15 +3689,15 @@
 
     """
 
     def __init__(self):
         r"""
         :param _Domain: 域名
         :type Domain: str
-        :param _Offset: 偏移
+        :param _Offset: 偏移量
         :type Offset: int
         :param _Limit: 容量
         :type Limit: int
         :param _Filters: 过滤数组,name可以是如下的值： RuleID,RuleName,Match
         :type Filters: list of FiltersItemNew
         :param _Order: asc或者desc
         :type Order: str
@@ -9301,15 +9301,15 @@
         :type Domain: str
         :param _AttackThreshold: 触发IP封禁的攻击次数阈值，范围为2~100次
         :type AttackThreshold: int
         :param _TimeThreshold: IP封禁统计时间，范围为1-60分钟
         :type TimeThreshold: int
         :param _DenyTimeThreshold: 触发IP封禁后的封禁时间，范围为5~360分钟
         :type DenyTimeThreshold: int
-        :param _DefenseStatus: 自动封禁状态
+        :param _DefenseStatus: 自动封禁状态，0表示关闭，1表示打开
         :type DefenseStatus: int
         """
         self._Domain = None
         self._AttackThreshold = None
         self._TimeThreshold = None
         self._DenyTimeThreshold = None
         self._DefenseStatus = None
@@ -10888,17 +10888,18 @@
 
     def __init__(self):
         r"""
         :param _Domain: 域名
         :type Domain: str
         :param _Ids: 规则列表
         :type Ids: list of int non-negative
-        :param _Status: 开关状态
+        :param _Status: 开关状态，0表示关闭，1表示开启，2表示只观察
         :type Status: int
-        :param _Reason: 设置为观察模式原因
+        :param _Reason: 设置为观察模式原因，
+1表示业务自身原因观察，2表示系统规则误报上报，3表示核心业务灰度观察，4表示其他
         :type Reason: int
         """
         self._Domain = None
         self._Ids = None
         self._Status = None
         self._Reason = None
```

### Comparing `tencentcloud-sdk-python-waf-3.0.939/PKG-INFO` & `tencentcloud-sdk-python-waf-3.0.940/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-waf
-Version: 3.0.939
+Version: 3.0.940
 Summary: Tencent Cloud Waf SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-waf-3.0.939/tencentcloud_sdk_python_waf.egg-info/PKG-INFO` & `tencentcloud-sdk-python-waf-3.0.940/tencentcloud_sdk_python_waf.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-waf
-Version: 3.0.939
+Version: 3.0.940
 Summary: Tencent Cloud Waf SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-waf-3.0.939/README.rst` & `tencentcloud-sdk-python-waf-3.0.940/README.rst`

 * *Files identical despite different names*

