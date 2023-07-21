# Comparing `tmp/tencentcloud-sdk-python-eiam-3.0.939.tar.gz` & `tmp/tencentcloud-sdk-python-eiam-3.0.940.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-eiam-3.0.939.tar", last modified: Thu Jul 20 00:23:44 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-eiam-3.0.940.tar", last modified: Fri Jul 21 00:28:40 2023, max compression
```

## Comparing `tencentcloud-sdk-python-eiam-3.0.939.tar` & `tencentcloud-sdk-python-eiam-3.0.940.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 00:23:44.000000 tencentcloud-sdk-python-eiam-3.0.939/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 00:23:44.000000 tencentcloud-sdk-python-eiam-3.0.939/tencentcloud_sdk_python_eiam.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 00:23:44.000000 tencentcloud-sdk-python-eiam-3.0.939/tencentcloud_sdk_python_eiam.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-07-20 00:23:44.000000 tencentcloud-sdk-python-eiam-3.0.939/tencentcloud_sdk_python_eiam.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-20 00:23:44.000000 tencentcloud-sdk-python-eiam-3.0.939/tencentcloud_sdk_python_eiam.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-20 00:23:44.000000 tencentcloud-sdk-python-eiam-3.0.939/tencentcloud_sdk_python_eiam.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1008 2023-07-20 00:23:43.000000 tencentcloud-sdk-python-eiam-3.0.939/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 00:23:44.000000 tencentcloud-sdk-python-eiam-3.0.939/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-20 00:23:43.000000 tencentcloud-sdk-python-eiam-3.0.939/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 00:23:44.000000 tencentcloud-sdk-python-eiam-3.0.939/tencentcloud/eiam/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 00:23:44.000000 tencentcloud-sdk-python-eiam-3.0.939/tencentcloud/eiam/v20210420/
--rw-r--r--   0 root         (0) root         (0)    39100 2023-07-20 00:23:43.000000 tencentcloud-sdk-python-eiam-3.0.939/tencentcloud/eiam/v20210420/eiam_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-20 00:23:43.000000 tencentcloud-sdk-python-eiam-3.0.939/tencentcloud/eiam/v20210420/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9938 2023-07-20 00:23:43.000000 tencentcloud-sdk-python-eiam-3.0.939/tencentcloud/eiam/v20210420/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   218794 2023-07-20 00:23:43.000000 tencentcloud-sdk-python-eiam-3.0.939/tencentcloud/eiam/v20210420/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-20 00:23:43.000000 tencentcloud-sdk-python-eiam-3.0.939/tencentcloud/eiam/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-20 00:23:44.000000 tencentcloud-sdk-python-eiam-3.0.939/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-20 00:23:44.000000 tencentcloud-sdk-python-eiam-3.0.939/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      740 2023-07-20 00:23:43.000000 tencentcloud-sdk-python-eiam-3.0.939/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:28:40.000000 tencentcloud-sdk-python-eiam-3.0.940/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:28:40.000000 tencentcloud-sdk-python-eiam-3.0.940/tencentcloud_sdk_python_eiam.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 00:28:40.000000 tencentcloud-sdk-python-eiam-3.0.940/tencentcloud_sdk_python_eiam.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-07-21 00:28:40.000000 tencentcloud-sdk-python-eiam-3.0.940/tencentcloud_sdk_python_eiam.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-21 00:28:40.000000 tencentcloud-sdk-python-eiam-3.0.940/tencentcloud_sdk_python_eiam.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-21 00:28:40.000000 tencentcloud-sdk-python-eiam-3.0.940/tencentcloud_sdk_python_eiam.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-07-21 00:28:39.000000 tencentcloud-sdk-python-eiam-3.0.940/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:28:40.000000 tencentcloud-sdk-python-eiam-3.0.940/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-21 00:28:39.000000 tencentcloud-sdk-python-eiam-3.0.940/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:28:40.000000 tencentcloud-sdk-python-eiam-3.0.940/tencentcloud/eiam/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:28:40.000000 tencentcloud-sdk-python-eiam-3.0.940/tencentcloud/eiam/v20210420/
+-rw-r--r--   0 root         (0) root         (0)    39100 2023-07-21 00:28:39.000000 tencentcloud-sdk-python-eiam-3.0.940/tencentcloud/eiam/v20210420/eiam_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 00:28:39.000000 tencentcloud-sdk-python-eiam-3.0.940/tencentcloud/eiam/v20210420/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9938 2023-07-21 00:28:39.000000 tencentcloud-sdk-python-eiam-3.0.940/tencentcloud/eiam/v20210420/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   218794 2023-07-21 00:28:39.000000 tencentcloud-sdk-python-eiam-3.0.940/tencentcloud/eiam/v20210420/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 00:28:39.000000 tencentcloud-sdk-python-eiam-3.0.940/tencentcloud/eiam/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-21 00:28:40.000000 tencentcloud-sdk-python-eiam-3.0.940/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-21 00:28:40.000000 tencentcloud-sdk-python-eiam-3.0.940/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      740 2023-07-21 00:28:39.000000 tencentcloud-sdk-python-eiam-3.0.940/README.rst
```

### Comparing `tencentcloud-sdk-python-eiam-3.0.939/tencentcloud_sdk_python_eiam.egg-info/PKG-INFO` & `tencentcloud-sdk-python-eiam-3.0.940/tencentcloud_sdk_python_eiam.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-eiam
-Version: 3.0.939
+Version: 3.0.940
 Summary: Tencent Cloud Eiam SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-eiam-3.0.939/setup.py` & `tencentcloud-sdk-python-eiam-3.0.940/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-eiam-3.0.939/tencentcloud/__init__.py` & `tencentcloud-sdk-python-eiam-3.0.940/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-eiam-3.0.939/tencentcloud/eiam/v20210420/eiam_client.py` & `tencentcloud-sdk-python-eiam-3.0.940/tencentcloud/eiam/v20210420/eiam_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-eiam-3.0.939/tencentcloud/eiam/v20210420/errorcodes.py` & `tencentcloud-sdk-python-eiam-3.0.940/tencentcloud/eiam/v20210420/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-eiam-3.0.939/tencentcloud/eiam/v20210420/models.py` & `tencentcloud-sdk-python-eiam-3.0.940/tencentcloud/eiam/v20210420/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-eiam-3.0.939/PKG-INFO` & `tencentcloud-sdk-python-eiam-3.0.940/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-eiam
-Version: 3.0.939
+Version: 3.0.940
 Summary: Tencent Cloud Eiam SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-eiam-3.0.939/README.rst` & `tencentcloud-sdk-python-eiam-3.0.940/README.rst`

 * *Files identical despite different names*

