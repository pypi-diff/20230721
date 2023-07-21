# Comparing `tmp/tencentcloud-sdk-python-postgres-3.0.939.tar.gz` & `tmp/tencentcloud-sdk-python-postgres-3.0.940.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-postgres-3.0.939.tar", last modified: Thu Jul 20 00:29:09 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-postgres-3.0.940.tar", last modified: Fri Jul 21 00:47:29 2023, max compression
```

## Comparing `tencentcloud-sdk-python-postgres-3.0.939.tar` & `tencentcloud-sdk-python-postgres-3.0.940.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 00:29:09.000000 tencentcloud-sdk-python-postgres-3.0.939/
--rw-r--r--   0 root         (0) root         (0)     1016 2023-07-20 00:29:09.000000 tencentcloud-sdk-python-postgres-3.0.939/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 00:29:09.000000 tencentcloud-sdk-python-postgres-3.0.939/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-20 00:29:09.000000 tencentcloud-sdk-python-postgres-3.0.939/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 00:29:09.000000 tencentcloud-sdk-python-postgres-3.0.939/tencentcloud/postgres/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-20 00:29:09.000000 tencentcloud-sdk-python-postgres-3.0.939/tencentcloud/postgres/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 00:29:09.000000 tencentcloud-sdk-python-postgres-3.0.939/tencentcloud/postgres/v20170312/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-20 00:29:09.000000 tencentcloud-sdk-python-postgres-3.0.939/tencentcloud/postgres/v20170312/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20749 2023-07-20 00:29:09.000000 tencentcloud-sdk-python-postgres-3.0.939/tencentcloud/postgres/v20170312/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    86120 2023-07-20 00:29:09.000000 tencentcloud-sdk-python-postgres-3.0.939/tencentcloud/postgres/v20170312/postgres_client.py
--rw-r--r--   0 root         (0) root         (0)   446339 2023-07-20 00:29:09.000000 tencentcloud-sdk-python-postgres-3.0.939/tencentcloud/postgres/v20170312/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-20 00:29:09.000000 tencentcloud-sdk-python-postgres-3.0.939/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 00:29:09.000000 tencentcloud-sdk-python-postgres-3.0.939/tencentcloud_sdk_python_postgres.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 00:29:09.000000 tencentcloud-sdk-python-postgres-3.0.939/tencentcloud_sdk_python_postgres.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      495 2023-07-20 00:29:09.000000 tencentcloud-sdk-python-postgres-3.0.939/tencentcloud_sdk_python_postgres.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1684 2023-07-20 00:29:09.000000 tencentcloud-sdk-python-postgres-3.0.939/tencentcloud_sdk_python_postgres.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-20 00:29:09.000000 tencentcloud-sdk-python-postgres-3.0.939/tencentcloud_sdk_python_postgres.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1684 2023-07-20 00:29:09.000000 tencentcloud-sdk-python-postgres-3.0.939/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      752 2023-07-20 00:29:09.000000 tencentcloud-sdk-python-postgres-3.0.939/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:47:29.000000 tencentcloud-sdk-python-postgres-3.0.940/
+-rw-r--r--   0 root         (0) root         (0)     1016 2023-07-21 00:47:29.000000 tencentcloud-sdk-python-postgres-3.0.940/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:47:29.000000 tencentcloud-sdk-python-postgres-3.0.940/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-21 00:47:29.000000 tencentcloud-sdk-python-postgres-3.0.940/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:47:29.000000 tencentcloud-sdk-python-postgres-3.0.940/tencentcloud/postgres/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 00:47:29.000000 tencentcloud-sdk-python-postgres-3.0.940/tencentcloud/postgres/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:47:29.000000 tencentcloud-sdk-python-postgres-3.0.940/tencentcloud/postgres/v20170312/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 00:47:29.000000 tencentcloud-sdk-python-postgres-3.0.940/tencentcloud/postgres/v20170312/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20749 2023-07-21 00:47:29.000000 tencentcloud-sdk-python-postgres-3.0.940/tencentcloud/postgres/v20170312/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    86440 2023-07-21 00:47:29.000000 tencentcloud-sdk-python-postgres-3.0.940/tencentcloud/postgres/v20170312/postgres_client.py
+-rw-r--r--   0 root         (0) root         (0)   454366 2023-07-21 00:47:29.000000 tencentcloud-sdk-python-postgres-3.0.940/tencentcloud/postgres/v20170312/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-21 00:47:29.000000 tencentcloud-sdk-python-postgres-3.0.940/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 00:47:29.000000 tencentcloud-sdk-python-postgres-3.0.940/tencentcloud_sdk_python_postgres.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 00:47:29.000000 tencentcloud-sdk-python-postgres-3.0.940/tencentcloud_sdk_python_postgres.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      495 2023-07-21 00:47:29.000000 tencentcloud-sdk-python-postgres-3.0.940/tencentcloud_sdk_python_postgres.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-07-21 00:47:29.000000 tencentcloud-sdk-python-postgres-3.0.940/tencentcloud_sdk_python_postgres.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-21 00:47:29.000000 tencentcloud-sdk-python-postgres-3.0.940/tencentcloud_sdk_python_postgres.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-07-21 00:47:29.000000 tencentcloud-sdk-python-postgres-3.0.940/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      752 2023-07-21 00:47:29.000000 tencentcloud-sdk-python-postgres-3.0.940/README.rst
```

### Comparing `tencentcloud-sdk-python-postgres-3.0.939/setup.py` & `tencentcloud-sdk-python-postgres-3.0.940/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-postgres-3.0.939/tencentcloud/__init__.py` & `tencentcloud-sdk-python-postgres-3.0.940/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-postgres-3.0.939/tencentcloud/postgres/v20170312/errorcodes.py` & `tencentcloud-sdk-python-postgres-3.0.940/tencentcloud/postgres/v20170312/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-postgres-3.0.939/tencentcloud/postgres/v20170312/postgres_client.py` & `tencentcloud-sdk-python-postgres-3.0.940/tencentcloud/postgres/v20170312/postgres_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -185,14 +185,16 @@
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateInstances(self, request):
         """本接口 (CreateInstances) 用于创建一个或者多个PostgreSQL实例，通过此接口创建的实例无需进行初始化，可直接使用。
+        <li>实例创建成功后将自动开机启动，实例状态变为“运行中”。
+        <li>预付费实例的购买会预先扣除本次实例购买所需金额，按小时后付费实例购买会预先冻结本次实例购买一小时内所需金额，在调用本接口前请确保账户余额充足。
 
         :param request: Request instance for CreateInstances.
         :type request: :class:`tencentcloud.postgres.v20170312.models.CreateInstancesRequest`
         :rtype: :class:`tencentcloud.postgres.v20170312.models.CreateInstancesResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-postgres-3.0.939/tencentcloud/postgres/v20170312/models.py` & `tencentcloud-sdk-python-postgres-3.0.940/tencentcloud/postgres/v20170312/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -888,48 +888,67 @@
 
     """
 
     def __init__(self):
         r"""
         :param _DBInstanceId: 克隆的源实例ID。
         :type DBInstanceId: str
-        :param _SpecCode: 售卖规格ID。该参数可以通过调用DescribeProductConfig的返回值中的SpecCode字段来获取。
+        :param _SpecCode: 售卖规格码。该参数可以通过调用[DescribeClasses](https://cloud.tencent.com/document/api/409/89019)的返回值中的SpecCode字段来获取。
         :type SpecCode: str
         :param _Storage: 实例容量大小，单位：GB。
         :type Storage: int
-        :param _Period: 购买时长，单位：月。目前只支持1,2,3,4,5,6,7,8,9,10,11,12,24,36这些值，按量计费模式下该参数传1。
+        :param _Period: 购买时长，单位：月。
+<li>预付费：支持1,2,3,4,5,6,7,8,9,10,11,12,24,36
+<li>后付费：只支持1
         :type Period: int
-        :param _AutoRenewFlag: 续费标记：0-正常续费（默认）；1-自动续费。
+        :param _AutoRenewFlag: 续费标记：
+<li>0：手动续费
+<li>1：自动续费
+默认值：0
         :type AutoRenewFlag: int
-        :param _VpcId: 私有网络ID。
+        :param _VpcId: 私有网络ID，形如vpc-xxxxxxxx。有效的VpcId可通过登录控制台查询；也可以调用接口 [DescribeVpcEx](https://cloud.tencent.com/document/api/215/1372) ，从接口返回中的unVpcId字段获取。
         :type VpcId: str
-        :param _SubnetId: 已配置的私有网络中的子网ID。
+        :param _SubnetId: 私有网络子网ID，形如subnet-xxxxxxxx。有效的私有网络子网ID可通过登录控制台查询；也可以调用接口 [DescribeSubnets ](https://cloud.tencent.com/document/api/215/15784)，从接口返回中的unSubnetId字段获取。
         :type SubnetId: str
-        :param _Name: 新购实例的实例名称。
+        :param _Name: 新购的实例名称，仅支持长度小于60的中文/英文/数字/"_"/"-"，不指定实例名称则默认显示"未命名"。
         :type Name: str
-        :param _InstanceChargeType: 实例计费类型。目前支持：PREPAID（预付费，即包年包月），POSTPAID_BY_HOUR（后付费，即按量计费）。
+        :param _InstanceChargeType: 实例计费类型，目前支持：
+<li>PREPAID：预付费，即包年包月
+<li>POSTPAID_BY_HOUR：后付费，即按量计费
+默认值：PREPAID
         :type InstanceChargeType: str
-        :param _SecurityGroupIds: 安全组ID。
+        :param _SecurityGroupIds: 实例所属安全组，该参数可以通过调用 [DescribeSecurityGroups](https://cloud.tencent.com/document/api/215/15808) 的返回值中的sgId字段来获取。若不指定该参数，则绑定默认安全组。
+
         :type SecurityGroupIds: list of str
         :param _ProjectId: 项目ID。
         :type ProjectId: int
-        :param _TagList: 实例需要绑定的Tag信息，默认为空。
+        :param _TagList: 实例需要绑定的Tag信息，默认为空；可以通过调用 [DescribeTags](https://cloud.tencent.com/document/api/651/35316) 返回值中的 Tags 字段来获取。
         :type TagList: list of Tag
-        :param _DBNodeSet: 购买多可用区实例时填写。
+        :param _DBNodeSet: 实例节点部署信息，支持多可用区部署时需要指定每个节点的部署可用区信息。
+可用区信息可以通过调用 [DescribeZones](https://cloud.tencent.com/document/api/409/16769) 接口的返回值中的Zone字段来获取。
         :type DBNodeSet: list of DBNode
-        :param _AutoVoucher: 是否自动使用代金券。1（是），0（否），默认不使用。
+        :param _AutoVoucher: 是否自动使用代金券：
+<li>0：否
+<li>1：是
+默认值：0
         :type AutoVoucher: int
         :param _VoucherIds: 代金券ID列表。
         :type VoucherIds: str
         :param _ActivityId: 活动ID。
         :type ActivityId: int
         :param _BackupSetId: 基础备份集ID。
         :type BackupSetId: str
         :param _RecoveryTargetTime: 恢复时间点。
         :type RecoveryTargetTime: str
+        :param _SyncMode: 主从同步方式，支持： 
+<li>Semi-sync：半同步
+<li>Async：异步
+主实例默认值：Semi-sync
+只读实例默认值：Async
+        :type SyncMode: str
         """
         self._DBInstanceId = None
         self._SpecCode = None
         self._Storage = None
         self._Period = None
         self._AutoRenewFlag = None
         self._VpcId = None
@@ -941,14 +960,15 @@
         self._TagList = None
         self._DBNodeSet = None
         self._AutoVoucher = None
         self._VoucherIds = None
         self._ActivityId = None
         self._BackupSetId = None
         self._RecoveryTargetTime = None
+        self._SyncMode = None
 
     @property
     def DBInstanceId(self):
         return self._DBInstanceId
 
     @DBInstanceId.setter
     def DBInstanceId(self, DBInstanceId):
@@ -1086,14 +1106,22 @@
     def RecoveryTargetTime(self):
         return self._RecoveryTargetTime
 
     @RecoveryTargetTime.setter
     def RecoveryTargetTime(self, RecoveryTargetTime):
         self._RecoveryTargetTime = RecoveryTargetTime
 
+    @property
+    def SyncMode(self):
+        return self._SyncMode
+
+    @SyncMode.setter
+    def SyncMode(self, SyncMode):
+        self._SyncMode = SyncMode
+
 
     def _deserialize(self, params):
         self._DBInstanceId = params.get("DBInstanceId")
         self._SpecCode = params.get("SpecCode")
         self._Storage = params.get("Storage")
         self._Period = params.get("Period")
         self._AutoRenewFlag = params.get("AutoRenewFlag")
@@ -1116,14 +1144,15 @@
                 obj._deserialize(item)
                 self._DBNodeSet.append(obj)
         self._AutoVoucher = params.get("AutoVoucher")
         self._VoucherIds = params.get("VoucherIds")
         self._ActivityId = params.get("ActivityId")
         self._BackupSetId = params.get("BackupSetId")
         self._RecoveryTargetTime = params.get("RecoveryTargetTime")
+        self._SyncMode = params.get("SyncMode")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -1865,120 +1894,169 @@
 class CreateInstancesRequest(AbstractModel):
     """CreateInstances请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _SpecCode: 售卖规格ID。该参数可以通过调用DescribeClasses的返回值中的SpecCode字段来获取。
+        :param _Zone: 实例所属主可用区， 如：ap-guangzhou-3；若需要支持多可用区，在DBNodeSet.N字段中进行添加主可用区和备可用区信息；
+可用区信息可以通过调用 [DescribeZones](https://cloud.tencent.com/document/api/409/16769) 接口的返回值中的Zone字段来获取。
+        :type Zone: str
+        :param _SpecCode: 售卖规格码。该参数可以通过调用[DescribeClasses](https://cloud.tencent.com/document/api/409/89019)的返回值中的SpecCode字段来获取。
         :type SpecCode: str
         :param _Storage: 实例容量大小，单位：GB。
         :type Storage: int
-        :param _InstanceCount: 一次性购买的实例数量。取值1-10。
+        :param _InstanceCount: 购买实例数量，取值范围：[1-10]。一次性购买支持最大数量10个，若超过该数量，可进行多次调用进行购买。
         :type InstanceCount: int
-        :param _Period: 购买时长，单位：月。目前只支持1,2,3,4,5,6,7,8,9,10,11,12,24,36这些值，按量计费模式下该参数传1。
+        :param _Period: 购买时长，单位：月。
+<li>预付费：支持1,2,3,4,5,6,7,8,9,10,11,12,24,36
+<li>后付费：只支持1
         :type Period: int
-        :param _Zone: 可用区ID。该参数可以通过调用 DescribeZones 接口的返回值中的Zone字段来获取。
-        :type Zone: str
-        :param _Charset: 实例字符集，目前只支持：UTF8、LATIN1。
+        :param _Charset: 实例字符集，目前只支持：
+<li> UTF8
+<li> LATIN1
         :type Charset: str
-        :param _AdminName: 实例根账号用户名。
+        :param _AdminName: 实例根账号用户名，具体规范如下：
+<li>用户名需要1-16个字符，只能由字母、数字或下划线组成
+<li>不能为postgres
+<li>不能由数字和pg_开头
+<li>所有规则均不区分大小写
         :type AdminName: str
-        :param _AdminPassword: 实例根账号用户名对应的密码。
+        :param _AdminPassword: 实例根账号用户名对应的密码，长度8 ~ 32位，推荐使用12位以上的密码;不能以" / "开头;
+必须包含以下四项，字符种类:
+<li>小写字母： [a ~ z]
+<li>大写字母：[A ～ Z]
+<li>数字：0 - 9
+<li>特殊字符：()`~!@#$%^&*-+=_|{}[]:;'<>,.?/
         :type AdminPassword: str
-        :param _ProjectId: 项目ID。
-        :type ProjectId: int
-        :param _DBVersion: PostgreSQL版本。当输入该参数时，会基于此版本创建对应的最新内核版本号实例。该参数和DBMajorVersion、DBKernelVersion至少需要传递一个。
+        :param _DBMajorVersion: PostgreSQL大版本号，版本信息可从[DescribeDBVersions](https://cloud.tencent.com/document/api/409/89018)获取，目前支持10，11，12，13，14，15这几个大版本。
+当只输入该参数时，会基于此大版本号创建对应的最新小版本的最新内核版本号实例。
+该参数和DBVersion、DBKernelVersion需要至少指定一个，如无指定购买内核小版本需求时，只传入该参数即可。
+
+        :type DBMajorVersion: str
+        :param _DBVersion: PostgreSQL社区大版本+小版本号，如12.4，版本信息可从[DescribeDBVersions](https://cloud.tencent.com/document/api/409/89018)获取。
+当只输入该参数时，会基于此社区小版本号创建对应的最新内核版本实例。
+该参数和DBMajorVersion、DBKernelVersion需要至少指定一个。
         :type DBVersion: str
-        :param _InstanceChargeType: 实例计费类型。目前支持：PREPAID（预付费，即包年包月），POSTPAID_BY_HOUR（后付费，即按量计费）。默认值：PREPAID。
+        :param _DBKernelVersion: PostgreSQL内核版本号，如v12.7_r1.8，版本信息可从[DescribeDBVersions](https://cloud.tencent.com/document/api/409/89018)获取。
+当只输入该参数时，会创建指定的内核版本实例。只针对内核版本需要指定时使用，一般场景不推荐传入该参数。
+
+        :type DBKernelVersion: str
+        :param _InstanceChargeType: 实例计费类型，目前支持：
+<li>PREPAID：预付费，即包年包月
+<li>POSTPAID_BY_HOUR：后付费，即按量计费
+默认值：PREPAID
         :type InstanceChargeType: str
-        :param _AutoVoucher: 是否自动使用代金券。1（是），0（否），默认不使用。
-        :type AutoVoucher: int
-        :param _VoucherIds: 代金券ID列表，目前仅支持指定一张代金券。
-        :type VoucherIds: list of str
-        :param _VpcId: 私有网络ID。
+        :param _VpcId: 私有网络ID，形如vpc-xxxxxxxx。有效的VpcId可通过登录控制台查询；也可以调用接口 [DescribeVpcEx](https://cloud.tencent.com/document/api/215/1372) ，从接口返回中的unVpcId字段获取。
         :type VpcId: str
-        :param _SubnetId: 已配置的私有网络中的子网ID。
+        :param _SubnetId: 私有网络子网ID，形如subnet-xxxxxxxx。有效的私有网络子网ID可通过登录控制台查询；也可以调用接口 [DescribeSubnets ](https://cloud.tencent.com/document/api/215/15784)，从接口返回中的unSubnetId字段获取。
         :type SubnetId: str
-        :param _AutoRenewFlag: 续费标记：0-正常续费（默认）；1-自动续费。
+        :param _DBNodeSet: 实例节点部署信息，支持多可用区部署时需要指定每个节点的部署可用区信息。
+可用区信息可以通过调用 [DescribeZones](https://cloud.tencent.com/document/api/409/16769) 接口的返回值中的Zone字段来获取。
+        :type DBNodeSet: list of DBNode
+        :param _AutoRenewFlag: 续费标记：
+<li>0：手动续费
+<li>1：自动续费
+默认值：0
         :type AutoRenewFlag: int
+        :param _AutoVoucher: 是否自动使用代金券：
+<li>0：否
+<li>1：是
+默认值：0
+        :type AutoVoucher: int
+        :param _VoucherIds: 代金券ID列表，目前仅支持指定一张代金券。
+        :type VoucherIds: list of str
+        :param _ProjectId: 项目ID。
+        :type ProjectId: int
         :param _ActivityId: 活动ID。
         :type ActivityId: int
-        :param _Name: 实例名。
+        :param _Name: 实例名称，仅支持长度小于60的中文/英文/数字/"_"/"-"，不指定实例名称则默认显示"未命名"。
+
         :type Name: str
-        :param _NeedSupportIpv6: 是否需要支持Ipv6，1：是，0：否（默认）。
-        :type NeedSupportIpv6: int
-        :param _TagList: 实例需要绑定的Tag信息，默认为空。
+        :param _TagList: 实例需要绑定的Tag信息，默认为空；可以通过调用 [DescribeTags](https://cloud.tencent.com/document/api/651/35316) 返回值中的 Tags 字段来获取。
         :type TagList: list of Tag
-        :param _SecurityGroupIds: 安全组ID。
+        :param _SecurityGroupIds: 实例所属安全组，该参数可以通过调用 [DescribeSecurityGroups](https://cloud.tencent.com/document/api/215/15808) 的返回值中的sgId字段来获取。若不指定该参数，则绑定默认安全组。
+
         :type SecurityGroupIds: list of str
-        :param _DBMajorVersion: PostgreSQL主要版本。目前支持10，11，12，13这几个版本。当输入该参数时，会基于此版本创建对应的最新内核版本号实例。该参数和DBVersion、DBKernelVersion至少需要传递一个。
-        :type DBMajorVersion: str
-        :param _DBKernelVersion: PostgreSQL内核版本。当输入该参数时，会创建该内核版本号实例。该参数和DBVersion、DBMajorVersion至少需要传递一个。
-        :type DBKernelVersion: str
-        :param _DBNodeSet: 实例节点信息，购买跨可用区实例时填写。
-        :type DBNodeSet: list of DBNode
-        :param _NeedSupportTDE: 是否需要支持数据透明加密，1：是，0：否（默认）。
+        :param _NeedSupportTDE: 是否需要支持数据透明加密：
+<li>0：否
+<li>1：是
+默认值：0
+参考[数据透明加密概述](https://cloud.tencent.com/document/product/409/71748)
         :type NeedSupportTDE: int
         :param _KMSKeyId: 自定义密钥的KeyId，若选择自定义密匙加密，则需要传入自定义密匙的KeyId，KeyId是CMK的唯一标识。
+KeyId创建获取相关参考[开启透明数据加密](https://cloud.tencent.com/document/product/409/71749)
         :type KMSKeyId: str
         :param _KMSRegion: 使用KMS服务的地域，KMSRegion为空默认使用本地域的KMS，本地域不支持的情况下需自选其他KMS支持的地域。
+KMSRegion相关介绍参考[开启透明数据加密](https://cloud.tencent.com/document/product/409/71749)
         :type KMSRegion: str
         :param _DBEngine: 数据库引擎，支持：
-1、postgresql（云数据库PostgreSQL）；
-2、mssql_compatible（MSSQL兼容-云数据库PostgreSQL）；
-如不指定默认使用postgresql。
+<li>postgresql：云数据库PostgreSQL
+<li>mssql_compatible：MSSQL兼容-云数据库PostgreSQL
+默认值：postgresql
         :type DBEngine: str
         :param _DBEngineConfig: 数据库引擎的配置信息，配置格式如下：
 {"$key1":"$value1", "$key2":"$value2"}
-
 各引擎支持如下：
-1、mssql_compatible引擎：
-migrationMode：数据库模式，可选参数，可取值：single-db（单数据库模式），multi-db（多数据库模式）。默认为single-db。
-defaultLocale：排序区域规则，可选参数，在初始化后不可修改，默认为en_US，可选值如下：
+mssql_compatible引擎：
+<li>migrationMode：数据库模式，可选参数，可取值：single-db（单数据库模式），multi-db（多数据库模式）。默认为single-db。
+<li>defaultLocale：排序区域规则，可选参数，在初始化后不可修改，默认为en_US，可选值如下：
 "af_ZA", "sq_AL", "ar_DZ", "ar_BH", "ar_EG", "ar_IQ", "ar_JO", "ar_KW", "ar_LB", "ar_LY", "ar_MA", "ar_OM", "ar_QA", "ar_SA", "ar_SY", "ar_TN", "ar_AE", "ar_YE", "hy_AM", "az_Cyrl_AZ", "az_Latn_AZ", "eu_ES", "be_BY", "bg_BG", "ca_ES", "zh_HK", "zh_MO", "zh_CN", "zh_SG", "zh_TW", "hr_HR", "cs_CZ", "da_DK", "nl_BE", "nl_NL", "en_AU", "en_BZ", "en_CA", "en_IE", "en_JM", "en_NZ", "en_PH", "en_ZA", "en_TT", "en_GB", "en_US", "en_ZW", "et_EE", "fo_FO", "fa_IR", "fi_FI", "fr_BE", "fr_CA", "fr_FR", "fr_LU", "fr_MC", "fr_CH", "mk_MK", "ka_GE", "de_AT", "de_DE", "de_LI", "de_LU", "de_CH", "el_GR", "gu_IN", "he_IL", "hi_IN", "hu_HU", "is_IS", "id_ID", "it_IT", "it_CH", "ja_JP", "kn_IN", "kok_IN", "ko_KR", "ky_KG", "lv_LV", "lt_LT", "ms_BN", "ms_MY", "mr_IN", "mn_MN", "nb_NO", "nn_NO", "pl_PL", "pt_BR", "pt_PT", "pa_IN", "ro_RO", "ru_RU", "sa_IN", "sr_Cyrl_RS", "sr_Latn_RS", "sk_SK", "sl_SI", "es_AR", "es_BO", "es_CL", "es_CO", "es_CR", "es_DO", "es_EC", "es_SV", "es_GT", "es_HN", "es_MX", "es_NI", "es_PA", "es_PY","es_PE", "es_PR", "es_ES", "es_TRADITIONAL", "es_UY", "es_VE", "sw_KE", "sv_FI", "sv_SE", "tt_RU", "te_IN", "th_TH", "tr_TR", "uk_UA", "ur_IN", "ur_PK", "uz_Cyrl_UZ", "uz_Latn_UZ", "vi_VN"。
-serverCollationName：排序规则名称，可选参数，在初始化后不可修改，默认为sql_latin1_general_cp1_ci_as，可选值如下：
-"bbf_unicode_general_ci_as", "bbf_unicode_cp1_ci_as", "bbf_unicode_CP1250_ci_as", "bbf_unicode_CP1251_ci_as", "bbf_unicode_cp1253_ci_as", "bbf_unicode_cp1254_ci_as", "bbf_unicode_cp1255_ci_as", "bbf_unicode_cp1256_ci_as", "bbf_unicode_cp1257_ci_as", "bbf_unicode_cp1258_ci_as", "bbf_unicode_cp874_ci_as", "sql_latin1_general_cp1250_ci_as", "sql_latin1_general_cp1251_ci_as", "sql_latin1_general_cp1_ci_as", "sql_latin1_general_cp1253_ci_as", "sql_latin1_general_cp1254_ci_as", "sql_latin1_general_cp1255_ci_as","sql_latin1_general_cp1256_ci_as", "sql_latin1_general_cp1257_ci_as", "sql_latin1_general_cp1258_ci_as", "chinese_prc_ci_as", "cyrillic_general_ci_as", "finnish_swedish_ci_as", "french_ci_as", "japanese_ci_as", "korean_wansung_ci_as", "latin1_general_ci_as", "modern_spanish_ci_as", "polish_ci_as", "thai_ci_as", "traditional_spanish_ci_as", "turkish_ci_as", "ukrainian_ci_as", "vietnamese_ci_as"。
+<li>serverCollationName：排序规则名称，可选参数，在初始化后不可修改，默认为sql_latin1_general_cp1_ci_as，可选值如下："bbf_unicode_general_ci_as", "bbf_unicode_cp1_ci_as", "bbf_unicode_CP1250_ci_as", "bbf_unicode_CP1251_ci_as", "bbf_unicode_cp1253_ci_as", "bbf_unicode_cp1254_ci_as", "bbf_unicode_cp1255_ci_as", "bbf_unicode_cp1256_ci_as", "bbf_unicode_cp1257_ci_as", "bbf_unicode_cp1258_ci_as", "bbf_unicode_cp874_ci_as", "sql_latin1_general_cp1250_ci_as", "sql_latin1_general_cp1251_ci_as", "sql_latin1_general_cp1_ci_as", "sql_latin1_general_cp1253_ci_as", "sql_latin1_general_cp1254_ci_as", "sql_latin1_general_cp1255_ci_as","sql_latin1_general_cp1256_ci_as", "sql_latin1_general_cp1257_ci_as", "sql_latin1_general_cp1258_ci_as", "chinese_prc_ci_as", "cyrillic_general_ci_as", "finnish_swedish_ci_as", "french_ci_as", "japanese_ci_as", "korean_wansung_ci_as", "latin1_general_ci_as", "modern_spanish_ci_as", "polish_ci_as", "thai_ci_as", "traditional_spanish_ci_as", "turkish_ci_as", "ukrainian_ci_as", "vietnamese_ci_as"。
         :type DBEngineConfig: str
-        :param _SyncMode: 主从同步方式，可取值： 
-1、Semi-sync：半同步
-2、Async：异步 
-当前只支持Semi-sync
+        :param _SyncMode: 主从同步方式，支持： 
+<li>Semi-sync：半同步
+<li>Async：异步
+主实例默认值：Semi-sync
+只读实例默认值：Async
         :type SyncMode: str
+        :param _NeedSupportIpv6: 是否需要支持Ipv6：
+<li>0：否
+<li>1：是
+默认值：0
+        :type NeedSupportIpv6: int
         """
+        self._Zone = None
         self._SpecCode = None
         self._Storage = None
         self._InstanceCount = None
         self._Period = None
-        self._Zone = None
         self._Charset = None
         self._AdminName = None
         self._AdminPassword = None
-        self._ProjectId = None
+        self._DBMajorVersion = None
         self._DBVersion = None
+        self._DBKernelVersion = None
         self._InstanceChargeType = None
-        self._AutoVoucher = None
-        self._VoucherIds = None
         self._VpcId = None
         self._SubnetId = None
+        self._DBNodeSet = None
         self._AutoRenewFlag = None
+        self._AutoVoucher = None
+        self._VoucherIds = None
+        self._ProjectId = None
         self._ActivityId = None
         self._Name = None
-        self._NeedSupportIpv6 = None
         self._TagList = None
         self._SecurityGroupIds = None
-        self._DBMajorVersion = None
-        self._DBKernelVersion = None
-        self._DBNodeSet = None
         self._NeedSupportTDE = None
         self._KMSKeyId = None
         self._KMSRegion = None
         self._DBEngine = None
         self._DBEngineConfig = None
         self._SyncMode = None
+        self._NeedSupportIpv6 = None
+
+    @property
+    def Zone(self):
+        return self._Zone
+
+    @Zone.setter
+    def Zone(self, Zone):
+        self._Zone = Zone
 
     @property
     def SpecCode(self):
         return self._SpecCode
 
     @SpecCode.setter
     def SpecCode(self, SpecCode):
@@ -2005,22 +2083,14 @@
         return self._Period
 
     @Period.setter
     def Period(self, Period):
         self._Period = Period
 
     @property
-    def Zone(self):
-        return self._Zone
-
-    @Zone.setter
-    def Zone(self, Zone):
-        self._Zone = Zone
-
-    @property
     def Charset(self):
         return self._Charset
 
     @Charset.setter
     def Charset(self, Charset):
         self._Charset = Charset
 
@@ -2037,54 +2107,46 @@
         return self._AdminPassword
 
     @AdminPassword.setter
     def AdminPassword(self, AdminPassword):
         self._AdminPassword = AdminPassword
 
     @property
-    def ProjectId(self):
-        return self._ProjectId
+    def DBMajorVersion(self):
+        return self._DBMajorVersion
 
-    @ProjectId.setter
-    def ProjectId(self, ProjectId):
-        self._ProjectId = ProjectId
+    @DBMajorVersion.setter
+    def DBMajorVersion(self, DBMajorVersion):
+        self._DBMajorVersion = DBMajorVersion
 
     @property
     def DBVersion(self):
         return self._DBVersion
 
     @DBVersion.setter
     def DBVersion(self, DBVersion):
         self._DBVersion = DBVersion
 
     @property
+    def DBKernelVersion(self):
+        return self._DBKernelVersion
+
+    @DBKernelVersion.setter
+    def DBKernelVersion(self, DBKernelVersion):
+        self._DBKernelVersion = DBKernelVersion
+
+    @property
     def InstanceChargeType(self):
         return self._InstanceChargeType
 
     @InstanceChargeType.setter
     def InstanceChargeType(self, InstanceChargeType):
         self._InstanceChargeType = InstanceChargeType
 
     @property
-    def AutoVoucher(self):
-        return self._AutoVoucher
-
-    @AutoVoucher.setter
-    def AutoVoucher(self, AutoVoucher):
-        self._AutoVoucher = AutoVoucher
-
-    @property
-    def VoucherIds(self):
-        return self._VoucherIds
-
-    @VoucherIds.setter
-    def VoucherIds(self, VoucherIds):
-        self._VoucherIds = VoucherIds
-
-    @property
     def VpcId(self):
         return self._VpcId
 
     @VpcId.setter
     def VpcId(self, VpcId):
         self._VpcId = VpcId
 
@@ -2093,22 +2155,54 @@
         return self._SubnetId
 
     @SubnetId.setter
     def SubnetId(self, SubnetId):
         self._SubnetId = SubnetId
 
     @property
+    def DBNodeSet(self):
+        return self._DBNodeSet
+
+    @DBNodeSet.setter
+    def DBNodeSet(self, DBNodeSet):
+        self._DBNodeSet = DBNodeSet
+
+    @property
     def AutoRenewFlag(self):
         return self._AutoRenewFlag
 
     @AutoRenewFlag.setter
     def AutoRenewFlag(self, AutoRenewFlag):
         self._AutoRenewFlag = AutoRenewFlag
 
     @property
+    def AutoVoucher(self):
+        return self._AutoVoucher
+
+    @AutoVoucher.setter
+    def AutoVoucher(self, AutoVoucher):
+        self._AutoVoucher = AutoVoucher
+
+    @property
+    def VoucherIds(self):
+        return self._VoucherIds
+
+    @VoucherIds.setter
+    def VoucherIds(self, VoucherIds):
+        self._VoucherIds = VoucherIds
+
+    @property
+    def ProjectId(self):
+        return self._ProjectId
+
+    @ProjectId.setter
+    def ProjectId(self, ProjectId):
+        self._ProjectId = ProjectId
+
+    @property
     def ActivityId(self):
         return self._ActivityId
 
     @ActivityId.setter
     def ActivityId(self, ActivityId):
         self._ActivityId = ActivityId
 
@@ -2117,22 +2211,14 @@
         return self._Name
 
     @Name.setter
     def Name(self, Name):
         self._Name = Name
 
     @property
-    def NeedSupportIpv6(self):
-        return self._NeedSupportIpv6
-
-    @NeedSupportIpv6.setter
-    def NeedSupportIpv6(self, NeedSupportIpv6):
-        self._NeedSupportIpv6 = NeedSupportIpv6
-
-    @property
     def TagList(self):
         return self._TagList
 
     @TagList.setter
     def TagList(self, TagList):
         self._TagList = TagList
 
@@ -2141,38 +2227,14 @@
         return self._SecurityGroupIds
 
     @SecurityGroupIds.setter
     def SecurityGroupIds(self, SecurityGroupIds):
         self._SecurityGroupIds = SecurityGroupIds
 
     @property
-    def DBMajorVersion(self):
-        return self._DBMajorVersion
-
-    @DBMajorVersion.setter
-    def DBMajorVersion(self, DBMajorVersion):
-        self._DBMajorVersion = DBMajorVersion
-
-    @property
-    def DBKernelVersion(self):
-        return self._DBKernelVersion
-
-    @DBKernelVersion.setter
-    def DBKernelVersion(self, DBKernelVersion):
-        self._DBKernelVersion = DBKernelVersion
-
-    @property
-    def DBNodeSet(self):
-        return self._DBNodeSet
-
-    @DBNodeSet.setter
-    def DBNodeSet(self, DBNodeSet):
-        self._DBNodeSet = DBNodeSet
-
-    @property
     def NeedSupportTDE(self):
         return self._NeedSupportTDE
 
     @NeedSupportTDE.setter
     def NeedSupportTDE(self, NeedSupportTDE):
         self._NeedSupportTDE = NeedSupportTDE
 
@@ -2212,56 +2274,64 @@
     def SyncMode(self):
         return self._SyncMode
 
     @SyncMode.setter
     def SyncMode(self, SyncMode):
         self._SyncMode = SyncMode
 
+    @property
+    def NeedSupportIpv6(self):
+        return self._NeedSupportIpv6
+
+    @NeedSupportIpv6.setter
+    def NeedSupportIpv6(self, NeedSupportIpv6):
+        self._NeedSupportIpv6 = NeedSupportIpv6
+
 
     def _deserialize(self, params):
+        self._Zone = params.get("Zone")
         self._SpecCode = params.get("SpecCode")
         self._Storage = params.get("Storage")
         self._InstanceCount = params.get("InstanceCount")
         self._Period = params.get("Period")
-        self._Zone = params.get("Zone")
         self._Charset = params.get("Charset")
         self._AdminName = params.get("AdminName")
         self._AdminPassword = params.get("AdminPassword")
-        self._ProjectId = params.get("ProjectId")
+        self._DBMajorVersion = params.get("DBMajorVersion")
         self._DBVersion = params.get("DBVersion")
+        self._DBKernelVersion = params.get("DBKernelVersion")
         self._InstanceChargeType = params.get("InstanceChargeType")
-        self._AutoVoucher = params.get("AutoVoucher")
-        self._VoucherIds = params.get("VoucherIds")
         self._VpcId = params.get("VpcId")
         self._SubnetId = params.get("SubnetId")
+        if params.get("DBNodeSet") is not None:
+            self._DBNodeSet = []
+            for item in params.get("DBNodeSet"):
+                obj = DBNode()
+                obj._deserialize(item)
+                self._DBNodeSet.append(obj)
         self._AutoRenewFlag = params.get("AutoRenewFlag")
+        self._AutoVoucher = params.get("AutoVoucher")
+        self._VoucherIds = params.get("VoucherIds")
+        self._ProjectId = params.get("ProjectId")
         self._ActivityId = params.get("ActivityId")
         self._Name = params.get("Name")
-        self._NeedSupportIpv6 = params.get("NeedSupportIpv6")
         if params.get("TagList") is not None:
             self._TagList = []
             for item in params.get("TagList"):
                 obj = Tag()
                 obj._deserialize(item)
                 self._TagList.append(obj)
         self._SecurityGroupIds = params.get("SecurityGroupIds")
-        self._DBMajorVersion = params.get("DBMajorVersion")
-        self._DBKernelVersion = params.get("DBKernelVersion")
-        if params.get("DBNodeSet") is not None:
-            self._DBNodeSet = []
-            for item in params.get("DBNodeSet"):
-                obj = DBNode()
-                obj._deserialize(item)
-                self._DBNodeSet.append(obj)
         self._NeedSupportTDE = params.get("NeedSupportTDE")
         self._KMSKeyId = params.get("KMSKeyId")
         self._KMSRegion = params.get("KMSRegion")
         self._DBEngine = params.get("DBEngine")
         self._DBEngineConfig = params.get("DBEngineConfig")
         self._SyncMode = params.get("SyncMode")
+        self._NeedSupportIpv6 = params.get("NeedSupportIpv6")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -3409,146 +3479,172 @@
 class DBInstance(AbstractModel):
     """描述实例的详细信息
 
     """
 
     def __init__(self):
         r"""
-        :param _Region: 实例所属地域，如: ap-guangzhou，对应RegionSet的Region字段
+        :param _Region: 实例所属地域，如: ap-guangzhou，对应RegionSet的Region字段。
         :type Region: str
-        :param _Zone: 实例所属可用区， 如：ap-guangzhou-3，对应ZoneSet的Zone字段
+        :param _Zone: 实例所属可用区， 如：ap-guangzhou-3，对应ZoneSet的Zone字段。
         :type Zone: str
-        :param _ProjectId: 项目ID
-        :type ProjectId: int
-        :param _VpcId: 私有网络ID
+        :param _VpcId: 私有网络ID，形如vpc-xxxxxxxx。有效的VpcId可通过登录控制台查询；也可以调用接口 [DescribeVpcEx](https://cloud.tencent.com/document/api/215/1372) ，从接口返回中的unVpcId字段获取。
         :type VpcId: str
-        :param _SubnetId: 子网ID
+        :param _SubnetId: 私有网络子网ID，形如subnet-xxxxxxxx。有效的私有网络子网ID可通过登录控制台查询；也可以调用接口 [DescribeSubnets ](https://cloud.tencent.com/document/api/215/15784)，从接口返回中的unSubnetId字段获取。
         :type SubnetId: str
-        :param _DBInstanceId: 实例ID
+        :param _DBInstanceId: 实例ID。
         :type DBInstanceId: str
-        :param _DBInstanceName: 实例名称
+        :param _DBInstanceName: 实例名称。
         :type DBInstanceName: str
-        :param _DBInstanceStatus: 实例状态，分别为：applying（申请中）、init(待初始化)、initing(初始化中)、running(运行中)、limited run（受限运行）、isolating（隔离中）、isolated（已隔离）、recycling（回收中）、recycled（已回收）、job running（任务执行中）、offline（下线）、migrating（迁移中）、expanding（扩容中）、waitSwitch（等待切换）、switching（切换中）、readonly（只读）、restarting（重启中）、network changing（网络变更中）、upgrading（内核版本升级中）
+        :param _DBInstanceStatus: 实例状态，分别为：applying（申请中）、init(待初始化)、initing(初始化中)、running(运行中)、limited run（受限运行）、isolating（隔离中）、isolated（已隔离）、recycling（回收中）、recycled（已回收）、job running（任务执行中）、offline（下线）、migrating（迁移中）、expanding（扩容中）、waitSwitch（等待切换）、switching（切换中）、readonly（只读）、restarting（重启中）、network changing（网络变更中）、upgrading（内核版本升级中）、audit-switching（审计状态变更中）、primary-switching（主备切换中）
         :type DBInstanceStatus: str
         :param _DBInstanceMemory: 实例分配的内存大小，单位：GB
         :type DBInstanceMemory: int
         :param _DBInstanceStorage: 实例分配的存储空间大小，单位：GB
         :type DBInstanceStorage: int
         :param _DBInstanceCpu: 实例分配的CPU数量，单位：个
         :type DBInstanceCpu: int
         :param _DBInstanceClass: 售卖规格ID
         :type DBInstanceClass: str
-        :param _DBInstanceType: 实例类型，类型有：1、primary（主实例）；2、readonly（只读实例）；3、guard（灾备实例）；4、temp（临时实例）
+        :param _DBMajorVersion: PostgreSQL大版本号，版本信息可从[DescribeDBVersions](https://cloud.tencent.com/document/api/409/89018)获取，目前支持10，11，12，13，14，15这几个大版本。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type DBMajorVersion: str
+        :param _DBVersion: PostgreSQL社区大版本+小版本号，如12.4，版本信息可从[DescribeDBVersions](https://cloud.tencent.com/document/api/409/89018)获取。
+        :type DBVersion: str
+        :param _DBKernelVersion: PostgreSQL内核版本号，如v12.7_r1.8，版本信息可从[DescribeDBVersions](https://cloud.tencent.com/document/api/409/89018)获取。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type DBKernelVersion: str
+        :param _DBInstanceType: 实例类型，类型有：
+<li>primary：主实例
+<li>readonly：只读实例
+<li>guard：灾备实例
+<li>temp：临时实例
         :type DBInstanceType: str
-        :param _DBInstanceVersion: 实例版本，目前只支持standard（双机高可用版, 一主一从）
+        :param _DBInstanceVersion: 实例版本，目前只支持standard（双机高可用版, 一主一从）。
         :type DBInstanceVersion: str
-        :param _DBCharset: 实例DB字符集
+        :param _DBCharset: 实例字符集，目前只支持：
+<li> UTF8
+<li> LATIN1
         :type DBCharset: str
-        :param _DBVersion: PostgreSQL版本
-        :type DBVersion: str
-        :param _CreateTime: 实例创建时间
+        :param _CreateTime: 实例创建时间。
         :type CreateTime: str
-        :param _UpdateTime: 实例执行最后一次更新的时间
+        :param _UpdateTime: 实例执行最后一次更新的时间。
         :type UpdateTime: str
-        :param _ExpireTime: 实例到期时间
+        :param _ExpireTime: 实例到期时间。
         :type ExpireTime: str
-        :param _IsolatedTime: 实例隔离时间
+        :param _IsolatedTime: 实例隔离时间。
         :type IsolatedTime: str
-        :param _PayType: 计费模式，1、prepaid（包年包月,预付费）；2、postpaid（按量计费，后付费）
+        :param _PayType: 计费模式：
+<li>prepaid：包年包月,预付费
+<li>postpaid：按量计费，后付费
         :type PayType: str
-        :param _AutoRenew: 是否自动续费，1：自动续费，0：不自动续费
+        :param _AutoRenew: 是否自动续费：
+<li>0：手动续费
+<li>1：自动续费
+默认值：0
         :type AutoRenew: int
-        :param _DBInstanceNetInfo: 实例网络连接信息
+        :param _DBInstanceNetInfo: 实例网络连接信息。
         :type DBInstanceNetInfo: list of DBInstanceNetInfo
-        :param _Type: 机器类型
+        :param _Type: 机器类型。
         :type Type: str
-        :param _AppId: 用户的AppId
+        :param _AppId: 用户的AppId。
         :type AppId: int
-        :param _Uid: 实例的Uid
+        :param _Uid: 实例的Uid。
         :type Uid: int
-        :param _SupportIpv6: 实例是否支持Ipv6，1：支持，0：不支持
-        :type SupportIpv6: int
-        :param _TagList: 实例绑定的标签信息
+        :param _ProjectId: 项目ID。
+        :type ProjectId: int
+        :param _TagList: 实例绑定的标签信息。
 注意：此字段可能返回 null，表示取不到有效值。
         :type TagList: list of Tag
-        :param _MasterDBInstanceId: 主实例信息，仅在实例为只读实例时返回
+        :param _MasterDBInstanceId: 主实例信息，仅在实例为只读实例时返回。
 注意：此字段可能返回 null，表示取不到有效值。
         :type MasterDBInstanceId: str
-        :param _ReadOnlyInstanceNum: 只读实例数量
+        :param _ReadOnlyInstanceNum: 只读实例数量。
 注意：此字段可能返回 null，表示取不到有效值。
         :type ReadOnlyInstanceNum: int
-        :param _StatusInReadonlyGroup: 只读实例在只读组中的状态
+        :param _StatusInReadonlyGroup: 只读实例在只读组中的状态。
 注意：此字段可能返回 null，表示取不到有效值。
         :type StatusInReadonlyGroup: str
-        :param _OfflineTime: 下线时间
+        :param _OfflineTime: 下线时间。
 注意：此字段可能返回 null，表示取不到有效值。
         :type OfflineTime: str
-        :param _DBKernelVersion: 数据库内核版本
-注意：此字段可能返回 null，表示取不到有效值。
-        :type DBKernelVersion: str
-        :param _NetworkAccessList: 实例网络信息列表（此字段已废弃）
-注意：此字段可能返回 null，表示取不到有效值。
-        :type NetworkAccessList: list of NetworkAccess
-        :param _DBMajorVersion: PostgreSQL主要版本
-注意：此字段可能返回 null，表示取不到有效值。
-        :type DBMajorVersion: str
-        :param _DBNodeSet: 实例的节点信息
+        :param _DBNodeSet: 实例的节点信息。
 注意：此字段可能返回 null，表示取不到有效值。
         :type DBNodeSet: list of DBNode
-        :param _IsSupportTDE: 实例是否支持TDE数据加密  0：不支持，1：支持
+        :param _IsSupportTDE: 实例是否支持TDE数据加密：
+<li>0：不支持
+<li>1：支持
+默认值：0
+TDE数据加密可参考[数据透明加密概述](https://cloud.tencent.com/document/product/409/71748)
 注意：此字段可能返回 null，表示取不到有效值。
         :type IsSupportTDE: int
         :param _DBEngine: 数据库引擎，支持：
-1、postgresql（云数据库PostgreSQL）；
-2、mssql_compatible（MSSQL兼容-云数据库PostgreSQL）；
+<li>postgresql：云数据库PostgreSQL
+<li>mssql_compatible：MSSQL兼容-云数据库PostgreSQL
+默认值：postgresql
 注意：此字段可能返回 null，表示取不到有效值。
         :type DBEngine: str
-        :param _DBEngineConfig: 数据库引擎的配置信息
+        :param _DBEngineConfig: 数据库引擎的配置信息，配置格式如下：
+{"$key1":"$value1", "$key2":"$value2"}
+各引擎支持如下：
+mssql_compatible引擎：
+<li>migrationMode：数据库模式，可选参数，可取值：single-db（单数据库模式），multi-db（多数据库模式）。默认为single-db。
+<li>defaultLocale：排序区域规则，可选参数，在初始化后不可修改，默认为en_US，可选值如下：
+"af_ZA", "sq_AL", "ar_DZ", "ar_BH", "ar_EG", "ar_IQ", "ar_JO", "ar_KW", "ar_LB", "ar_LY", "ar_MA", "ar_OM", "ar_QA", "ar_SA", "ar_SY", "ar_TN", "ar_AE", "ar_YE", "hy_AM", "az_Cyrl_AZ", "az_Latn_AZ", "eu_ES", "be_BY", "bg_BG", "ca_ES", "zh_HK", "zh_MO", "zh_CN", "zh_SG", "zh_TW", "hr_HR", "cs_CZ", "da_DK", "nl_BE", "nl_NL", "en_AU", "en_BZ", "en_CA", "en_IE", "en_JM", "en_NZ", "en_PH", "en_ZA", "en_TT", "en_GB", "en_US", "en_ZW", "et_EE", "fo_FO", "fa_IR", "fi_FI", "fr_BE", "fr_CA", "fr_FR", "fr_LU", "fr_MC", "fr_CH", "mk_MK", "ka_GE", "de_AT", "de_DE", "de_LI", "de_LU", "de_CH", "el_GR", "gu_IN", "he_IL", "hi_IN", "hu_HU", "is_IS", "id_ID", "it_IT", "it_CH", "ja_JP", "kn_IN", "kok_IN", "ko_KR", "ky_KG", "lv_LV", "lt_LT", "ms_BN", "ms_MY", "mr_IN", "mn_MN", "nb_NO", "nn_NO", "pl_PL", "pt_BR", "pt_PT", "pa_IN", "ro_RO", "ru_RU", "sa_IN", "sr_Cyrl_RS", "sr_Latn_RS", "sk_SK", "sl_SI", "es_AR", "es_BO", "es_CL", "es_CO", "es_CR", "es_DO", "es_EC", "es_SV", "es_GT", "es_HN", "es_MX", "es_NI", "es_PA", "es_PY","es_PE", "es_PR", "es_ES", "es_TRADITIONAL", "es_UY", "es_VE", "sw_KE", "sv_FI", "sv_SE", "tt_RU", "te_IN", "th_TH", "tr_TR", "uk_UA", "ur_IN", "ur_PK", "uz_Cyrl_UZ", "uz_Latn_UZ", "vi_VN"。
+<li>serverCollationName：排序规则名称，可选参数，在初始化后不可修改，默认为sql_latin1_general_cp1_ci_as，可选值如下："bbf_unicode_general_ci_as", "bbf_unicode_cp1_ci_as", "bbf_unicode_CP1250_ci_as", "bbf_unicode_CP1251_ci_as", "bbf_unicode_cp1253_ci_as", "bbf_unicode_cp1254_ci_as", "bbf_unicode_cp1255_ci_as", "bbf_unicode_cp1256_ci_as", "bbf_unicode_cp1257_ci_as", "bbf_unicode_cp1258_ci_as", "bbf_unicode_cp874_ci_as", "sql_latin1_general_cp1250_ci_as", "sql_latin1_general_cp1251_ci_as", "sql_latin1_general_cp1_ci_as", "sql_latin1_general_cp1253_ci_as", "sql_latin1_general_cp1254_ci_as", "sql_latin1_general_cp1255_ci_as","sql_latin1_general_cp1256_ci_as", "sql_latin1_general_cp1257_ci_as", "sql_latin1_general_cp1258_ci_as", "chinese_prc_ci_as", "cyrillic_general_ci_as", "finnish_swedish_ci_as", "french_ci_as", "japanese_ci_as", "korean_wansung_ci_as", "latin1_general_ci_as", "modern_spanish_ci_as", "polish_ci_as", "thai_ci_as", "traditional_spanish_ci_as", "turkish_ci_as", "ukrainian_ci_as", "vietnamese_ci_as"。
 注意：此字段可能返回 null，表示取不到有效值。
         :type DBEngineConfig: str
+        :param _NetworkAccessList: 实例网络信息列表（此字段已废弃）
+注意：此字段可能返回 null，表示取不到有效值。
+        :type NetworkAccessList: list of NetworkAccess
+        :param _SupportIpv6: 实例是否支持Ipv6：
+<li>0：否
+<li>1：是
+默认值：0
+        :type SupportIpv6: int
         """
         self._Region = None
         self._Zone = None
-        self._ProjectId = None
         self._VpcId = None
         self._SubnetId = None
         self._DBInstanceId = None
         self._DBInstanceName = None
         self._DBInstanceStatus = None
         self._DBInstanceMemory = None
         self._DBInstanceStorage = None
         self._DBInstanceCpu = None
         self._DBInstanceClass = None
+        self._DBMajorVersion = None
+        self._DBVersion = None
+        self._DBKernelVersion = None
         self._DBInstanceType = None
         self._DBInstanceVersion = None
         self._DBCharset = None
-        self._DBVersion = None
         self._CreateTime = None
         self._UpdateTime = None
         self._ExpireTime = None
         self._IsolatedTime = None
         self._PayType = None
         self._AutoRenew = None
         self._DBInstanceNetInfo = None
         self._Type = None
         self._AppId = None
         self._Uid = None
-        self._SupportIpv6 = None
+        self._ProjectId = None
         self._TagList = None
         self._MasterDBInstanceId = None
         self._ReadOnlyInstanceNum = None
         self._StatusInReadonlyGroup = None
         self._OfflineTime = None
-        self._DBKernelVersion = None
-        self._NetworkAccessList = None
-        self._DBMajorVersion = None
         self._DBNodeSet = None
         self._IsSupportTDE = None
         self._DBEngine = None
         self._DBEngineConfig = None
+        self._NetworkAccessList = None
+        self._SupportIpv6 = None
 
     @property
     def Region(self):
         return self._Region
 
     @Region.setter
     def Region(self, Region):
@@ -3559,22 +3655,14 @@
         return self._Zone
 
     @Zone.setter
     def Zone(self, Zone):
         self._Zone = Zone
 
     @property
-    def ProjectId(self):
-        return self._ProjectId
-
-    @ProjectId.setter
-    def ProjectId(self, ProjectId):
-        self._ProjectId = ProjectId
-
-    @property
     def VpcId(self):
         return self._VpcId
 
     @VpcId.setter
     def VpcId(self, VpcId):
         self._VpcId = VpcId
 
@@ -3639,14 +3727,38 @@
         return self._DBInstanceClass
 
     @DBInstanceClass.setter
     def DBInstanceClass(self, DBInstanceClass):
         self._DBInstanceClass = DBInstanceClass
 
     @property
+    def DBMajorVersion(self):
+        return self._DBMajorVersion
+
+    @DBMajorVersion.setter
+    def DBMajorVersion(self, DBMajorVersion):
+        self._DBMajorVersion = DBMajorVersion
+
+    @property
+    def DBVersion(self):
+        return self._DBVersion
+
+    @DBVersion.setter
+    def DBVersion(self, DBVersion):
+        self._DBVersion = DBVersion
+
+    @property
+    def DBKernelVersion(self):
+        return self._DBKernelVersion
+
+    @DBKernelVersion.setter
+    def DBKernelVersion(self, DBKernelVersion):
+        self._DBKernelVersion = DBKernelVersion
+
+    @property
     def DBInstanceType(self):
         return self._DBInstanceType
 
     @DBInstanceType.setter
     def DBInstanceType(self, DBInstanceType):
         self._DBInstanceType = DBInstanceType
 
@@ -3663,22 +3775,14 @@
         return self._DBCharset
 
     @DBCharset.setter
     def DBCharset(self, DBCharset):
         self._DBCharset = DBCharset
 
     @property
-    def DBVersion(self):
-        return self._DBVersion
-
-    @DBVersion.setter
-    def DBVersion(self, DBVersion):
-        self._DBVersion = DBVersion
-
-    @property
     def CreateTime(self):
         return self._CreateTime
 
     @CreateTime.setter
     def CreateTime(self, CreateTime):
         self._CreateTime = CreateTime
 
@@ -3751,20 +3855,20 @@
         return self._Uid
 
     @Uid.setter
     def Uid(self, Uid):
         self._Uid = Uid
 
     @property
-    def SupportIpv6(self):
-        return self._SupportIpv6
+    def ProjectId(self):
+        return self._ProjectId
 
-    @SupportIpv6.setter
-    def SupportIpv6(self, SupportIpv6):
-        self._SupportIpv6 = SupportIpv6
+    @ProjectId.setter
+    def ProjectId(self, ProjectId):
+        self._ProjectId = ProjectId
 
     @property
     def TagList(self):
         return self._TagList
 
     @TagList.setter
     def TagList(self, TagList):
@@ -3799,38 +3903,14 @@
         return self._OfflineTime
 
     @OfflineTime.setter
     def OfflineTime(self, OfflineTime):
         self._OfflineTime = OfflineTime
 
     @property
-    def DBKernelVersion(self):
-        return self._DBKernelVersion
-
-    @DBKernelVersion.setter
-    def DBKernelVersion(self, DBKernelVersion):
-        self._DBKernelVersion = DBKernelVersion
-
-    @property
-    def NetworkAccessList(self):
-        return self._NetworkAccessList
-
-    @NetworkAccessList.setter
-    def NetworkAccessList(self, NetworkAccessList):
-        self._NetworkAccessList = NetworkAccessList
-
-    @property
-    def DBMajorVersion(self):
-        return self._DBMajorVersion
-
-    @DBMajorVersion.setter
-    def DBMajorVersion(self, DBMajorVersion):
-        self._DBMajorVersion = DBMajorVersion
-
-    @property
     def DBNodeSet(self):
         return self._DBNodeSet
 
     @DBNodeSet.setter
     def DBNodeSet(self, DBNodeSet):
         self._DBNodeSet = DBNodeSet
 
@@ -3854,32 +3934,49 @@
     def DBEngineConfig(self):
         return self._DBEngineConfig
 
     @DBEngineConfig.setter
     def DBEngineConfig(self, DBEngineConfig):
         self._DBEngineConfig = DBEngineConfig
 
+    @property
+    def NetworkAccessList(self):
+        return self._NetworkAccessList
+
+    @NetworkAccessList.setter
+    def NetworkAccessList(self, NetworkAccessList):
+        self._NetworkAccessList = NetworkAccessList
+
+    @property
+    def SupportIpv6(self):
+        return self._SupportIpv6
+
+    @SupportIpv6.setter
+    def SupportIpv6(self, SupportIpv6):
+        self._SupportIpv6 = SupportIpv6
+
 
     def _deserialize(self, params):
         self._Region = params.get("Region")
         self._Zone = params.get("Zone")
-        self._ProjectId = params.get("ProjectId")
         self._VpcId = params.get("VpcId")
         self._SubnetId = params.get("SubnetId")
         self._DBInstanceId = params.get("DBInstanceId")
         self._DBInstanceName = params.get("DBInstanceName")
         self._DBInstanceStatus = params.get("DBInstanceStatus")
         self._DBInstanceMemory = params.get("DBInstanceMemory")
         self._DBInstanceStorage = params.get("DBInstanceStorage")
         self._DBInstanceCpu = params.get("DBInstanceCpu")
         self._DBInstanceClass = params.get("DBInstanceClass")
+        self._DBMajorVersion = params.get("DBMajorVersion")
+        self._DBVersion = params.get("DBVersion")
+        self._DBKernelVersion = params.get("DBKernelVersion")
         self._DBInstanceType = params.get("DBInstanceType")
         self._DBInstanceVersion = params.get("DBInstanceVersion")
         self._DBCharset = params.get("DBCharset")
-        self._DBVersion = params.get("DBVersion")
         self._CreateTime = params.get("CreateTime")
         self._UpdateTime = params.get("UpdateTime")
         self._ExpireTime = params.get("ExpireTime")
         self._IsolatedTime = params.get("IsolatedTime")
         self._PayType = params.get("PayType")
         self._AutoRenew = params.get("AutoRenew")
         if params.get("DBInstanceNetInfo") is not None:
@@ -3887,42 +3984,41 @@
             for item in params.get("DBInstanceNetInfo"):
                 obj = DBInstanceNetInfo()
                 obj._deserialize(item)
                 self._DBInstanceNetInfo.append(obj)
         self._Type = params.get("Type")
         self._AppId = params.get("AppId")
         self._Uid = params.get("Uid")
-        self._SupportIpv6 = params.get("SupportIpv6")
+        self._ProjectId = params.get("ProjectId")
         if params.get("TagList") is not None:
             self._TagList = []
             for item in params.get("TagList"):
                 obj = Tag()
                 obj._deserialize(item)
                 self._TagList.append(obj)
         self._MasterDBInstanceId = params.get("MasterDBInstanceId")
         self._ReadOnlyInstanceNum = params.get("ReadOnlyInstanceNum")
         self._StatusInReadonlyGroup = params.get("StatusInReadonlyGroup")
         self._OfflineTime = params.get("OfflineTime")
-        self._DBKernelVersion = params.get("DBKernelVersion")
-        if params.get("NetworkAccessList") is not None:
-            self._NetworkAccessList = []
-            for item in params.get("NetworkAccessList"):
-                obj = NetworkAccess()
-                obj._deserialize(item)
-                self._NetworkAccessList.append(obj)
-        self._DBMajorVersion = params.get("DBMajorVersion")
         if params.get("DBNodeSet") is not None:
             self._DBNodeSet = []
             for item in params.get("DBNodeSet"):
                 obj = DBNode()
                 obj._deserialize(item)
                 self._DBNodeSet.append(obj)
         self._IsSupportTDE = params.get("IsSupportTDE")
         self._DBEngine = params.get("DBEngine")
         self._DBEngineConfig = params.get("DBEngineConfig")
+        if params.get("NetworkAccessList") is not None:
+            self._NetworkAccessList = []
+            for item in params.get("NetworkAccessList"):
+                obj = NetworkAccess()
+                obj._deserialize(item)
+                self._NetworkAccessList.append(obj)
+        self._SupportIpv6 = params.get("SupportIpv6")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-postgres-3.0.939/tencentcloud_sdk_python_postgres.egg-info/PKG-INFO` & `tencentcloud-sdk-python-postgres-3.0.940/tencentcloud_sdk_python_postgres.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-postgres
-Version: 3.0.939
+Version: 3.0.940
 Summary: Tencent Cloud Postgres SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-postgres-3.0.939/PKG-INFO` & `tencentcloud-sdk-python-postgres-3.0.940/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-postgres
-Version: 3.0.939
+Version: 3.0.940
 Summary: Tencent Cloud Postgres SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-postgres-3.0.939/README.rst` & `tencentcloud-sdk-python-postgres-3.0.940/README.rst`

 * *Files identical despite different names*

