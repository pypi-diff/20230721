# Comparing `tmp/tencentcloud-sdk-python-vpc-3.0.939.tar.gz` & `tmp/tencentcloud-sdk-python-vpc-3.0.940.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-vpc-3.0.939.tar", last modified: Thu Jul 20 00:37:23 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-vpc-3.0.940.tar", last modified: Fri Jul 21 00:55:44 2023, max compression
```

## Comparing `tencentcloud-sdk-python-vpc-3.0.939.tar` & `tencentcloud-sdk-python-vpc-3.0.940.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 00:37:23.000000 tencentcloud-sdk-python-vpc-3.0.939/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-20 00:37:23.000000 tencentcloud-sdk-python-vpc-3.0.939/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 00:37:23.000000 tencentcloud-sdk-python-vpc-3.0.939/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 00:37:23.000000 tencentcloud-sdk-python-vpc-3.0.939/tencentcloud/vpc/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-20 00:37:23.000000 tencentcloud-sdk-python-vpc-3.0.939/tencentcloud/vpc/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 00:37:23.000000 tencentcloud-sdk-python-vpc-3.0.939/tencentcloud/vpc/v20170312/
--rw-r--r--   0 root         (0) root         (0)   333624 2023-07-20 00:37:23.000000 tencentcloud-sdk-python-vpc-3.0.939/tencentcloud/vpc/v20170312/vpc_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-20 00:37:23.000000 tencentcloud-sdk-python-vpc-3.0.939/tencentcloud/vpc/v20170312/__init__.py
--rw-r--r--   0 root         (0) root         (0)    42776 2023-07-20 00:37:23.000000 tencentcloud-sdk-python-vpc-3.0.939/tencentcloud/vpc/v20170312/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)  1312049 2023-07-20 00:37:23.000000 tencentcloud-sdk-python-vpc-3.0.939/tencentcloud/vpc/v20170312/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-20 00:37:23.000000 tencentcloud-sdk-python-vpc-3.0.939/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-20 00:37:23.000000 tencentcloud-sdk-python-vpc-3.0.939/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-20 00:37:23.000000 tencentcloud-sdk-python-vpc-3.0.939/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 00:37:23.000000 tencentcloud-sdk-python-vpc-3.0.939/tencentcloud_sdk_python_vpc.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 00:37:23.000000 tencentcloud-sdk-python-vpc-3.0.939/tencentcloud_sdk_python_vpc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-20 00:37:23.000000 tencentcloud-sdk-python-vpc-3.0.939/tencentcloud_sdk_python_vpc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-20 00:37:23.000000 tencentcloud-sdk-python-vpc-3.0.939/tencentcloud_sdk_python_vpc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-20 00:37:23.000000 tencentcloud-sdk-python-vpc-3.0.939/tencentcloud_sdk_python_vpc.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-20 00:37:23.000000 tencentcloud-sdk-python-vpc-3.0.939/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:55:44.000000 tencentcloud-sdk-python-vpc-3.0.940/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-21 00:55:44.000000 tencentcloud-sdk-python-vpc-3.0.940/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:55:44.000000 tencentcloud-sdk-python-vpc-3.0.940/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:55:44.000000 tencentcloud-sdk-python-vpc-3.0.940/tencentcloud/vpc/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 00:55:44.000000 tencentcloud-sdk-python-vpc-3.0.940/tencentcloud/vpc/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:55:44.000000 tencentcloud-sdk-python-vpc-3.0.940/tencentcloud/vpc/v20170312/
+-rw-r--r--   0 root         (0) root         (0)   333624 2023-07-21 00:55:44.000000 tencentcloud-sdk-python-vpc-3.0.940/tencentcloud/vpc/v20170312/vpc_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 00:55:44.000000 tencentcloud-sdk-python-vpc-3.0.940/tencentcloud/vpc/v20170312/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    42776 2023-07-21 00:55:44.000000 tencentcloud-sdk-python-vpc-3.0.940/tencentcloud/vpc/v20170312/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)  1312271 2023-07-21 00:55:44.000000 tencentcloud-sdk-python-vpc-3.0.940/tencentcloud/vpc/v20170312/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-21 00:55:44.000000 tencentcloud-sdk-python-vpc-3.0.940/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-21 00:55:44.000000 tencentcloud-sdk-python-vpc-3.0.940/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-21 00:55:44.000000 tencentcloud-sdk-python-vpc-3.0.940/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:55:44.000000 tencentcloud-sdk-python-vpc-3.0.940/tencentcloud_sdk_python_vpc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 00:55:44.000000 tencentcloud-sdk-python-vpc-3.0.940/tencentcloud_sdk_python_vpc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-21 00:55:44.000000 tencentcloud-sdk-python-vpc-3.0.940/tencentcloud_sdk_python_vpc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-21 00:55:44.000000 tencentcloud-sdk-python-vpc-3.0.940/tencentcloud_sdk_python_vpc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-21 00:55:44.000000 tencentcloud-sdk-python-vpc-3.0.940/tencentcloud_sdk_python_vpc.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-21 00:55:44.000000 tencentcloud-sdk-python-vpc-3.0.940/README.rst
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.939/setup.py` & `tencentcloud-sdk-python-vpc-3.0.940/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vpc-3.0.939/tencentcloud/vpc/v20170312/vpc_client.py` & `tencentcloud-sdk-python-vpc-3.0.940/tencentcloud/vpc/v20170312/vpc_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vpc-3.0.939/tencentcloud/vpc/v20170312/errorcodes.py` & `tencentcloud-sdk-python-vpc-3.0.940/tencentcloud/vpc/v20170312/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vpc-3.0.939/tencentcloud/vpc/v20170312/models.py` & `tencentcloud-sdk-python-vpc-3.0.940/tencentcloud/vpc/v20170312/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -17924,15 +17924,15 @@
     """
 
     def __init__(self):
         r"""
         :param _NatGatewayIds: NAT网关ID。
         :type NatGatewayIds: list of str
         :param _Filters: 过滤条件:
-参数不支持同时指定NatGatewayIds和Filters。
+参数不支持同时指定NatGatewayIds和Filters。每次请求的Filters的上限为10，Filter.Values的上限为5
 <li> nat-gateway-id，NAT网关的ID，如`nat-0yi4hekt`</li>
 <li> vpc-id，私有网络VPC的ID，如`vpc-0yi4hekt`</li>
 <li> public-ip-address， 弹性IP，如`139.199.232.238`。</li>
 <li>public-port， 公网端口。</li>
 <li>private-ip-address， 内网IP，如`10.0.0.1`。</li>
 <li>private-port， 内网端口。</li>
 <li>description，规则描述。</li>
@@ -18312,17 +18312,17 @@
 class DescribeNatGatewaysRequest(AbstractModel):
     """DescribeNatGateways请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _NatGatewayIds: NAT网关统一 ID，形如：`nat-123xx454`。
+        :param _NatGatewayIds: NAT网关统一 ID，形如：`nat-123xx454`。每次请求的实例上限为100。参数不支持同时指定NatGatewayIds和Filters。
         :type NatGatewayIds: list of str
-        :param _Filters: 过滤条件，参数不支持同时指定NatGatewayIds和Filters。
+        :param _Filters: 过滤条件，参数不支持同时指定NatGatewayIds和Filters。每次请求的Filters的上限为10，Filter.Values的上限为5。
 <li>nat-gateway-id - String - （过滤条件）协议端口模板实例ID，形如：`nat-123xx454`。</li>
 <li>vpc-id - String - （过滤条件）私有网络 唯一ID，形如：`vpc-123xx454`。</li>
 <li>nat-gateway-name - String - （过滤条件）协议端口模板实例ID，形如：`test_nat`。</li>
 <li>tag-key - String - （过滤条件）标签键，形如：`test-key`。</li>
         :type Filters: list of Filter
         :param _Offset: 偏移量，默认为0。
         :type Offset: int
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.939/tencentcloud/__init__.py` & `tencentcloud-sdk-python-vpc-3.0.940/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-vpc-3.0.939/PKG-INFO` & `tencentcloud-sdk-python-vpc-3.0.940/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-vpc
-Version: 3.0.939
+Version: 3.0.940
 Summary: Tencent Cloud Vpc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.939/tencentcloud_sdk_python_vpc.egg-info/PKG-INFO` & `tencentcloud-sdk-python-vpc-3.0.940/tencentcloud_sdk_python_vpc.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-vpc
-Version: 3.0.939
+Version: 3.0.940
 Summary: Tencent Cloud Vpc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.939/README.rst` & `tencentcloud-sdk-python-vpc-3.0.940/README.rst`

 * *Files identical despite different names*

