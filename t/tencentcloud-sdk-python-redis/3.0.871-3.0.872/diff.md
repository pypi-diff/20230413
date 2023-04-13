# Comparing `tmp/tencentcloud-sdk-python-redis-3.0.871.tar.gz` & `tmp/tencentcloud-sdk-python-redis-3.0.872.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-redis-3.0.871.tar", last modified: Wed Apr 12 00:38:32 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-redis-3.0.872.tar", last modified: Thu Apr 13 00:54:14 2023, max compression
```

## Comparing `tencentcloud-sdk-python-redis-3.0.871.tar` & `tencentcloud-sdk-python-redis-3.0.872.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 00:38:32.000000 tencentcloud-sdk-python-redis-3.0.871/
--rw-r--r--   0 root         (0) root         (0)     1669 2023-04-12 00:38:32.000000 tencentcloud-sdk-python-redis-3.0.871/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 00:38:32.000000 tencentcloud-sdk-python-redis-3.0.871/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 00:38:32.000000 tencentcloud-sdk-python-redis-3.0.871/tencentcloud/redis/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 00:38:32.000000 tencentcloud-sdk-python-redis-3.0.871/tencentcloud/redis/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 00:38:32.000000 tencentcloud-sdk-python-redis-3.0.871/tencentcloud/redis/v20180412/
--rw-r--r--   0 root         (0) root         (0)   287397 2023-04-12 00:38:32.000000 tencentcloud-sdk-python-redis-3.0.871/tencentcloud/redis/v20180412/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 00:38:32.000000 tencentcloud-sdk-python-redis-3.0.871/tencentcloud/redis/v20180412/__init__.py
--rw-r--r--   0 root         (0) root         (0)    86530 2023-04-12 00:38:32.000000 tencentcloud-sdk-python-redis-3.0.871/tencentcloud/redis/v20180412/redis_client.py
--rw-r--r--   0 root         (0) root         (0)    12423 2023-04-12 00:38:32.000000 tencentcloud-sdk-python-redis-3.0.871/tencentcloud/redis/v20180412/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-12 00:38:32.000000 tencentcloud-sdk-python-redis-3.0.871/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 00:38:32.000000 tencentcloud-sdk-python-redis-3.0.871/tencentcloud_sdk_python_redis.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1669 2023-04-12 00:38:32.000000 tencentcloud-sdk-python-redis-3.0.871/tencentcloud_sdk_python_redis.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 00:38:32.000000 tencentcloud-sdk-python-redis-3.0.871/tencentcloud_sdk_python_redis.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-12 00:38:32.000000 tencentcloud-sdk-python-redis-3.0.871/tencentcloud_sdk_python_redis.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      465 2023-04-12 00:38:32.000000 tencentcloud-sdk-python-redis-3.0.871/tencentcloud_sdk_python_redis.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)      743 2023-04-12 00:38:32.000000 tencentcloud-sdk-python-redis-3.0.871/README.rst
--rw-r--r--   0 root         (0) root         (0)     1010 2023-04-12 00:38:32.000000 tencentcloud-sdk-python-redis-3.0.871/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-12 00:38:32.000000 tencentcloud-sdk-python-redis-3.0.871/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 00:54:14.000000 tencentcloud-sdk-python-redis-3.0.872/
+-rw-r--r--   0 root         (0) root         (0)      743 2023-04-13 00:54:13.000000 tencentcloud-sdk-python-redis-3.0.872/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 00:54:14.000000 tencentcloud-sdk-python-redis-3.0.872/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 00:54:14.000000 tencentcloud-sdk-python-redis-3.0.872/tencentcloud/redis/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 00:54:14.000000 tencentcloud-sdk-python-redis-3.0.872/tencentcloud/redis/v20180412/
+-rw-r--r--   0 root         (0) root         (0)    86576 2023-04-13 00:54:13.000000 tencentcloud-sdk-python-redis-3.0.872/tencentcloud/redis/v20180412/redis_client.py
+-rw-r--r--   0 root         (0) root         (0)    12423 2023-04-13 00:54:13.000000 tencentcloud-sdk-python-redis-3.0.872/tencentcloud/redis/v20180412/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 00:54:13.000000 tencentcloud-sdk-python-redis-3.0.872/tencentcloud/redis/v20180412/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   288285 2023-04-13 00:54:13.000000 tencentcloud-sdk-python-redis-3.0.872/tencentcloud/redis/v20180412/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 00:54:13.000000 tencentcloud-sdk-python-redis-3.0.872/tencentcloud/redis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-13 00:54:13.000000 tencentcloud-sdk-python-redis-3.0.872/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-04-13 00:54:14.000000 tencentcloud-sdk-python-redis-3.0.872/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1010 2023-04-13 00:54:13.000000 tencentcloud-sdk-python-redis-3.0.872/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-13 00:54:14.000000 tencentcloud-sdk-python-redis-3.0.872/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 00:54:14.000000 tencentcloud-sdk-python-redis-3.0.872/tencentcloud_sdk_python_redis.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 00:54:14.000000 tencentcloud-sdk-python-redis-3.0.872/tencentcloud_sdk_python_redis.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      465 2023-04-13 00:54:14.000000 tencentcloud-sdk-python-redis-3.0.872/tencentcloud_sdk_python_redis.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-04-13 00:54:14.000000 tencentcloud-sdk-python-redis-3.0.872/tencentcloud_sdk_python_redis.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-13 00:54:14.000000 tencentcloud-sdk-python-redis-3.0.872/tencentcloud_sdk_python_redis.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-redis-3.0.871/PKG-INFO` & `tencentcloud-sdk-python-redis-3.0.872/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-redis
-Version: 3.0.871
+Version: 3.0.872
 Summary: Tencent Cloud Redis SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-redis-3.0.871/tencentcloud/redis/v20180412/models.py` & `tencentcloud-sdk-python-redis-3.0.872/tencentcloud/redis/v20180412/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -301,23 +301,23 @@
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
 class BackupLimitVpcItem(AbstractModel):
-    """自定义的备份文件下载地址的 VPC 信息。
+    """已配置的备份文件下载地址对应的 VPC 信息。
 
     """
 
     def __init__(self):
         r"""
-        :param Region: 自定义下载备份文件的VPC 所属地域。
+        :param Region: 备份文件的下载地址对应VPC 所属的地域。
         :type Region: str
-        :param VpcList: 自定义下载备份文件的 VPC 列表。
+        :param VpcList: 备份文件下载地址的 VPC 列表。
         :type VpcList: list of str
         """
         self.Region = None
         self.VpcList = None
 
 
     def _deserialize(self, params):
@@ -3217,15 +3217,15 @@
 class DescribeParamTemplateInfoRequest(AbstractModel):
     """DescribeParamTemplateInfo请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param TemplateId: 参数模板 ID。
+        :param TemplateId: 指定查询的参数模板 ID。请通过接口[DescribeParamTemplates](https://cloud.tencent.com/document/product/239/58750)获取参数模板列表信息。
         :type TemplateId: str
         """
         self.TemplateId = None
 
 
     def _deserialize(self, params):
         self.TemplateId = params.get("TemplateId")
@@ -3241,25 +3241,35 @@
 class DescribeParamTemplateInfoResponse(AbstractModel):
     """DescribeParamTemplateInfo返回参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param TotalCount: 实例参数个数
+        :param TotalCount: 参数模板的参数数量。
         :type TotalCount: int
         :param TemplateId: 参数模板 ID。
         :type TemplateId: str
         :param Name: 参数模板名称。
         :type Name: str
-        :param ProductType: 产品类型：1 – Redis2.8内存版（集群架构），2 – Redis2.8内存版（标准架构），3 – CKV 3.2内存版(标准架构)，4 – CKV 3.2内存版(集群架构)，5 – Redis2.8内存版（单机），6 – Redis4.0内存版（标准架构），7 – Redis4.0内存版（集群架构），8 – Redis5.0内存版（标准架构），9 – Redis5.0内存版（集群架构）
+        :param ProductType: 产品类型。
+- 2：Redis 2.8内存版（标准架构）。
+- 3：CKV 3.2内存版（标准架构）。
+- 4：CKV 3.2内存版（集群架构）。
+- 5：Redis 2.8内存版（单机）。
+- 6：Redis 4.0内存版（标准架构）。
+- 7：Redis 4.0内存版（集群架构）。
+- 8：Redis 5.0内存版（标准架构）。
+- 9：Redis 5.0内存版（集群架构）。
+- 15：Redis 6.2内存版（标准架构）。
+- 16：Redis 6.2内存版（集群架构）。
         :type ProductType: int
-        :param Description: 参数模板描述
+        :param Description: 参数模板描述。
         :type Description: str
-        :param Items: 参数详情
+        :param Items: 参数详情。包含：参数的名称，当前运行值，默认值，最大值、最小值、枚举值等信息。
         :type Items: list of ParameterDetail
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self.TotalCount = None
         self.TemplateId = None
         self.Name = None
@@ -4263,15 +4273,15 @@
 class Groups(AbstractModel):
     """复制组信息
 
     """
 
     def __init__(self):
         r"""
-        :param AppId: 用户AppID
+        :param AppId: 用户 APPID。APPID是与账号ID有唯一对应关系的应用 ID，部分腾讯云产品会使用此 APPID。
         :type AppId: int
         :param RegionId: 地域ID 。
 - 1：广州 
 - 4：上海 
 - 5：中国香港 
 - 6：多伦多 
 - 7：上海金融 
@@ -4285,15 +4295,15 @@
 - 19：重庆 
 - 21：印度 
 - 22：美东（弗吉尼亚）
 - 23：泰国 
 - 24：俄罗斯 
 - 25：日本
         :type RegionId: int
-        :param GroupId: 复制组 ID。
+        :param GroupId: 复制组 ID。格式如：crs-rpl-deind****。
         :type GroupId: str
         :param GroupName: 复制组名称。
 注意：此字段可能返回 null，表示取不到有效值。
         :type GroupName: str
         :param Status: 复制组状态。
 - 37：绑定复制组中。
 - 38：复制组重连中。
@@ -4979,23 +4989,26 @@
 class InstanceParamHistory(AbstractModel):
     """实例参数修改历史
 
     """
 
     def __init__(self):
         r"""
-        :param ParamName: 参数名称
+        :param ParamName: 参数名称。
         :type ParamName: str
-        :param PreValue: 修改前值
+        :param PreValue: 参数修改之前的值。
         :type PreValue: str
-        :param NewValue: 修改后值
+        :param NewValue: 参数修改之后的值。
         :type NewValue: str
-        :param Status: 状态：1-参数配置修改中；2-参数配置修改成功；3-参数配置修改失败
+        :param Status: 参数配置状态。
+- 1：参数配置修改中。
+- 2：参数配置修改成功。
+- 3：参数配置修改失败。
         :type Status: int
-        :param ModifyTime: 修改时间
+        :param ModifyTime: 修改时间。
         :type ModifyTime: str
         """
         self.ParamName = None
         self.PreValue = None
         self.NewValue = None
         self.Status = None
         self.ModifyTime = None
@@ -5019,21 +5032,21 @@
 class InstanceProxySlowlogDetail(AbstractModel):
     """代理慢查询详情
 
     """
 
     def __init__(self):
         r"""
-        :param Duration: 慢查询耗时（单位：毫秒）。
+        :param Duration: 慢查询耗时时长。单位：毫秒。
         :type Duration: int
         :param Client: 客户端地址。
         :type Client: str
-        :param Command: 命令。
+        :param Command: 慢查询的命令。
         :type Command: str
-        :param CommandLine: 详细命令行信息。
+        :param CommandLine: 慢查询详细命令行信息。
         :type CommandLine: str
         :param ExecuteTime: 执行时间。
         :type ExecuteTime: str
         """
         self.Duration = None
         self.Client = None
         self.Command = None
@@ -5120,15 +5133,25 @@
         :type Port: int
         :param Createtime: 实例创建时间。
         :type Createtime: str
         :param Size: 实例容量大小，单位：MB。
         :type Size: float
         :param SizeUsed: 该字段已废弃。请使用腾讯云可观测平台API 接口 [GetMonitorData](https://cloud.tencent.com/document/product/248/31014) 获取实例已使用的内存容量。
         :type SizeUsed: float
-        :param Type: 实例类型：<ul><li>1：Redis2.8内存版（集群架构）。</li><li>2：Redis2.8内存版（标准架构）。</li><li>3：CKV 3.2内存版(标准架构)。</li><li>4：CKV 3.2内存版(集群架构)。</li><li>5：Redis2.8内存版（单机）。</li></li><li>6：Redis4.0内存版（标准架构）。</li></li><li>7：Redis4.0内存版（集群架构）。</li></li><li>8：Redis5.0内存版（标准架构）。</li></li><li>9：Redis5.0内存版（集群架构）。</li></ul>
+        :param Type: 实例类型。
+- 2：Redis 2.8内存版（标准架构）。
+- 3：CKV 3.2内存版（标准架构）。
+- 4：CKV 3.2内存版（集群架构）。
+- 5：Redis 2.8内存版（单机）。
+- 6：Redis 4.0内存版（标准架构）。
+- 7：Redis 4.0内存版（集群架构）。
+- 8：Redis 5.0内存版（标准架构）。
+- 9：Redis 5.0内存版（集群架构）。
+- 15：Redis 6.2内存版（标准架构）。
+- 16：Redis 6.2内存版（集群架构）。
         :type Type: int
         :param AutoRenewFlag: 实例是否设置自动续费标识。<ul><li>1：设置自动续费。</li><li>0：未设置自动续费。</li></ul>
         :type AutoRenewFlag: int
         :param DeadlineTime: 实例到期时间。
         :type DeadlineTime: str
         :param Engine: 引擎：社区版Redis、腾讯云CKV。
         :type Engine: str
@@ -5493,15 +5516,15 @@
 class Instances(AbstractModel):
     """复制组实例
 
     """
 
     def __init__(self):
         r"""
-        :param AppId: 用户AppID。
+        :param AppId: 用户APPID。APPID是与账号ID有唯一对应关系的应用 ID，部分腾讯云产品会使用此 APPID。
         :type AppId: int
         :param InstanceId: 实例 ID。
         :type InstanceId: str
         :param InstanceName: 实例名称。
         :type InstanceName: str
         :param RegionId: 地域ID。<ul><li>1：广州。</li><li>4：上海。</li><li> 5：香港。</li> <li> 6：多伦多。</li> <li> 7：上海金融。</li> <li> 8：北京。</li> <li> 9：新加坡。</li> <li> 11：深圳金融。</li> <li> 15：美西（硅谷）。</li> </ul>
         :type RegionId: int
@@ -5529,15 +5552,25 @@
         :type VpcID: int
         :param VPort: 实例端口。
         :type VPort: int
         :param Status: 实例状态。<ul><li>0：待初始化。</li><li>1：流程中。</li><li>2：运行中。</li><li>-2：已隔离。</li><li>-3：待删除。</li></ul>
         :type Status: int
         :param GrocerySysId: 仓库ID。
         :type GrocerySysId: int
-        :param ProductType: 实例类型。<ul><li>1：Redis 2.8 内存版（集群架构）。</li><li>2：Redis 2.8 内存版（标准架构）。</li><li>3：CKV 3.2 内存版（标准架构）。</li><li>4：CKV 3.2 内存版（集群架构）。</li><li>5：Redis 2.8 单机版。</li><li>6：Redis 4.0 内存版（标准架构）。</li><li>7：Redis 4.0 内存版（集群架构）。</li><li>8：Redis 5.0 内存版（标准架构）。</li><li>9：Redis 5.0 内存版（集群架构）。</li></ul>
+        :param ProductType: 实例类型。
+- 2：Redis 2.8内存版（标准架构）。
+- 3：CKV 3.2内存版（标准架构）。
+- 4：CKV 3.2内存版（集群架构）。
+- 5：Redis 2.8内存版（单机）。
+- 6：Redis 4.0内存版（标准架构）。
+- 7：Redis 4.0内存版（集群架构）。
+- 8：Redis 5.0内存版（标准架构）。
+- 9：Redis 5.0内存版（集群架构）。
+- 15：Redis 6.2内存版（标准架构）。
+- 16：Redis 6.2内存版（集群架构）。
         :type ProductType: int
         :param CreateTime: 实例加入复制组的时间。
         :type CreateTime: str
         :param UpdateTime: 复制组中实例更新的时间。
         :type UpdateTime: str
         """
         self.AppId = None
@@ -6552,21 +6585,30 @@
 class ParamTemplateInfo(AbstractModel):
     """参数模板信息
 
     """
 
     def __init__(self):
         r"""
-        :param TemplateId: 参数模板ID
+        :param TemplateId: 参数模板 ID。
         :type TemplateId: str
-        :param Name: 参数模板名称
+        :param Name: 参数模板名称。
         :type Name: str
-        :param Description: 参数模板描述
+        :param Description: 参数模板描述。
         :type Description: str
-        :param ProductType: 产品类型：1 – Redis2.8内存版（集群架构），2 – Redis2.8内存版（标准架构），3 – CKV 3.2内存版(标准架构)，4 – CKV 3.2内存版(集群架构)，5 – Redis2.8内存版（单机），6 – Redis4.0内存版（标准架构），7 – Redis4.0内存版（集群架构），8 – Redis5.0内存版（标准架构），9 – Redis5.0内存版（集群架构）
+        :param ProductType: 实例类型。
+- 2：Redis 2.8内存版（标准架构）。
+- 3：CKV 3.2内存版（标准架构）。
+- 4：CKV 3.2内存版（集群架构）。
+- 5：Redis 2.8内存版（单机）。
+- 6：Redis 4.0内存版（标准架构）。
+- 7：Redis 4.0内存版（集群架构）。
+- 8：Redis 5.0内存版（标准架构）。
+- 9：Redis 5.0内存版（集群架构）。
+
         :type ProductType: int
         """
         self.TemplateId = None
         self.Name = None
         self.Description = None
         self.ProductType = None
 
@@ -6588,33 +6630,35 @@
 class ParameterDetail(AbstractModel):
     """Redis参数模板参数详情
 
     """
 
     def __init__(self):
         r"""
-        :param Name: 参数名称
+        :param Name: 参数名称。
         :type Name: str
-        :param ParamType: 参数类型
+        :param ParamType: 参数类型。
         :type ParamType: str
-        :param Default: 参数默认值
+        :param Default: 参数默认值。
         :type Default: str
-        :param Description: 参数描述
+        :param Description: 参数描述。
         :type Description: str
-        :param CurrentValue: 参数当前值
+        :param CurrentValue: 参数当前值。
         :type CurrentValue: str
-        :param NeedReboot: 修改参数后，是否需要重启数据库以使参数生效。可能的值包括：0-不需要重启；1-需要重启
+        :param NeedReboot: 修改参数后，是否需要重启数据库以使参数生效。
+- 0：不需要重启。
+- 1：需要重启。
         :type NeedReboot: int
-        :param Max: 参数允许的最大值
+        :param Max: 参数允许的最大值。
 注意：此字段可能返回 null，表示取不到有效值。
         :type Max: str
-        :param Min: 参数允许的最小值
+        :param Min: 参数允许的最小值。
 注意：此字段可能返回 null，表示取不到有效值。
         :type Min: str
-        :param EnumValue: 参数的可选枚举值。如果为非枚举参数，则为空
+        :param EnumValue: 参数可选枚举值。如果为非枚举参数，则为空。
 注意：此字段可能返回 null，表示取不到有效值。
         :type EnumValue: list of str
         """
         self.Name = None
         self.ParamType = None
         self.Default = None
         self.Description = None
@@ -6844,41 +6888,50 @@
 class RedisCommonInstanceList(AbstractModel):
     """单个实例信息
 
     """
 
     def __init__(self):
         r"""
-        :param InstanceName: 实例名称
+        :param InstanceName: 实例名称。
         :type InstanceName: str
-        :param InstanceId: 实例id
+        :param InstanceId: 实例 ID。
         :type InstanceId: str
-        :param AppId: 用户id
+        :param AppId: 用户APPID。APPID是与账号ID有唯一对应关系的应用 ID，部分腾讯云产品会使用此 APPID。
         :type AppId: int
-        :param ProjectId: 实例所属项目id
+        :param ProjectId: 实例所属项目 ID。
         :type ProjectId: int
-        :param Region: 实例接入区域
+        :param Region: 实例接入区域。
         :type Region: str
-        :param Zone: 实例接入zone
+        :param Zone: 实例接入可用区。
         :type Zone: str
-        :param VpcId: 实例网络id
+        :param VpcId: 实例私有网络 ID。
         :type VpcId: str
-        :param SubnetId: 子网id
+        :param SubnetId: 私有网络所属子网 ID。
         :type SubnetId: str
-        :param Status: 实例状态信息，1-流程中 ,2-运行中, -2-实例已隔离 ,-3-实例待回收, -4-实例已删除
+        :param Status: 实例状态信息。
+- 1-流程中。
+- 2-运行中。
+- -2-实例已隔离。
+- -3-实例待回收。
+- -4-实例已删除。
         :type Status: str
-        :param Vips: 实例网络ip
+        :param Vips: 实例私有网络 IP 地址。
         :type Vips: list of str
-        :param Vport: 实例网络端口
+        :param Vport: 实例网络端口。
         :type Vport: int
-        :param Createtime: 实例创建时间
+        :param Createtime: 实例创建时间。
         :type Createtime: str
-        :param PayMode: 计费类型，0-按量计费，1-包年包月
+        :param PayMode: 计费类型。
+- 0：按量计费。
+- 1：包年包月。
         :type PayMode: int
-        :param NetType: 网络类型，0-基础网络，1-VPC网络
+        :param NetType: 网络类型。
+- 0：基础网络。
+- 1：VPC 网络。
         :type NetType: int
         """
         self.InstanceName = None
         self.InstanceId = None
         self.AppId = None
         self.ProjectId = None
         self.Region = None
@@ -7330,17 +7383,17 @@
 class ResourceTag(AbstractModel):
     """API购买实例绑定标签
 
     """
 
     def __init__(self):
         r"""
-        :param TagKey: 标签key
+        :param TagKey: 标签Key。
         :type TagKey: str
-        :param TagValue: 标签value
+        :param TagValue: 标签 Key 对应的 Value。
         :type TagValue: str
         """
         self.TagKey = None
         self.TagValue = None
 
 
     def _deserialize(self, params):
```

### Comparing `tencentcloud-sdk-python-redis-3.0.871/tencentcloud/redis/v20180412/redis_client.py` & `tencentcloud-sdk-python-redis-3.0.872/tencentcloud/redis/v20180412/redis_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1035,15 +1035,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DescribeParamTemplateInfo(self, request):
-        """查询参数模板详情。
+        """本接口（DescribeParamTemplateInfo）用于查询参数模板详情。
 
         :param request: Request instance for DescribeParamTemplateInfo.
         :type request: :class:`tencentcloud.redis.v20180412.models.DescribeParamTemplateInfoRequest`
         :rtype: :class:`tencentcloud.redis.v20180412.models.DescribeParamTemplateInfoResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-redis-3.0.871/tencentcloud/redis/v20180412/errorcodes.py` & `tencentcloud-sdk-python-redis-3.0.872/tencentcloud/redis/v20180412/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-redis-3.0.871/tencentcloud/__init__.py` & `tencentcloud-sdk-python-redis-3.0.872/tencentcloud/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.871'
+__version__ = '3.0.872'
```

### Comparing `tencentcloud-sdk-python-redis-3.0.871/tencentcloud_sdk_python_redis.egg-info/PKG-INFO` & `tencentcloud-sdk-python-redis-3.0.872/tencentcloud_sdk_python_redis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-redis
-Version: 3.0.871
+Version: 3.0.872
 Summary: Tencent Cloud Redis SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-redis-3.0.871/README.rst` & `tencentcloud-sdk-python-redis-3.0.872/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-redis-3.0.871/setup.py` & `tencentcloud-sdk-python-redis-3.0.872/setup.py`

 * *Files identical despite different names*

