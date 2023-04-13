# Comparing `tmp/tencentcloud-sdk-python-tcaplusdb-3.0.871.tar.gz` & `tmp/tencentcloud-sdk-python-tcaplusdb-3.0.872.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tcaplusdb-3.0.871.tar", last modified: Wed Apr 12 00:41:45 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tcaplusdb-3.0.872.tar", last modified: Thu Apr 13 00:58:06 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tcaplusdb-3.0.871.tar` & `tencentcloud-sdk-python-tcaplusdb-3.0.872.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 00:41:45.000000 tencentcloud-sdk-python-tcaplusdb-3.0.871/
--rw-r--r--   0 root         (0) root         (0)     1689 2023-04-12 00:41:45.000000 tencentcloud-sdk-python-tcaplusdb-3.0.871/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 00:41:45.000000 tencentcloud-sdk-python-tcaplusdb-3.0.871/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 00:41:45.000000 tencentcloud-sdk-python-tcaplusdb-3.0.871/tencentcloud/tcaplusdb/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 00:41:45.000000 tencentcloud-sdk-python-tcaplusdb-3.0.871/tencentcloud/tcaplusdb/v20190823/
--rw-r--r--   0 root         (0) root         (0)   185698 2023-04-12 00:41:45.000000 tencentcloud-sdk-python-tcaplusdb-3.0.871/tencentcloud/tcaplusdb/v20190823/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 00:41:45.000000 tencentcloud-sdk-python-tcaplusdb-3.0.871/tencentcloud/tcaplusdb/v20190823/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3614 2023-04-12 00:41:45.000000 tencentcloud-sdk-python-tcaplusdb-3.0.871/tencentcloud/tcaplusdb/v20190823/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    45999 2023-04-12 00:41:45.000000 tencentcloud-sdk-python-tcaplusdb-3.0.871/tencentcloud/tcaplusdb/v20190823/tcaplusdb_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 00:41:45.000000 tencentcloud-sdk-python-tcaplusdb-3.0.871/tencentcloud/tcaplusdb/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-12 00:41:45.000000 tencentcloud-sdk-python-tcaplusdb-3.0.871/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)      755 2023-04-12 00:41:45.000000 tencentcloud-sdk-python-tcaplusdb-3.0.871/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 00:41:45.000000 tencentcloud-sdk-python-tcaplusdb-3.0.871/tencentcloud_sdk_python_tcaplusdb.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1689 2023-04-12 00:41:45.000000 tencentcloud-sdk-python-tcaplusdb-3.0.871/tencentcloud_sdk_python_tcaplusdb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 00:41:45.000000 tencentcloud-sdk-python-tcaplusdb-3.0.871/tencentcloud_sdk_python_tcaplusdb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-12 00:41:45.000000 tencentcloud-sdk-python-tcaplusdb-3.0.871/tencentcloud_sdk_python_tcaplusdb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      505 2023-04-12 00:41:45.000000 tencentcloud-sdk-python-tcaplusdb-3.0.871/tencentcloud_sdk_python_tcaplusdb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1018 2023-04-12 00:41:45.000000 tencentcloud-sdk-python-tcaplusdb-3.0.871/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-12 00:41:45.000000 tencentcloud-sdk-python-tcaplusdb-3.0.871/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 00:58:06.000000 tencentcloud-sdk-python-tcaplusdb-3.0.872/
+-rw-r--r--   0 root         (0) root         (0)      755 2023-04-13 00:58:06.000000 tencentcloud-sdk-python-tcaplusdb-3.0.872/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 00:58:06.000000 tencentcloud-sdk-python-tcaplusdb-3.0.872/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-13 00:58:06.000000 tencentcloud-sdk-python-tcaplusdb-3.0.872/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 00:58:06.000000 tencentcloud-sdk-python-tcaplusdb-3.0.872/tencentcloud/tcaplusdb/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 00:58:06.000000 tencentcloud-sdk-python-tcaplusdb-3.0.872/tencentcloud/tcaplusdb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 00:58:06.000000 tencentcloud-sdk-python-tcaplusdb-3.0.872/tencentcloud/tcaplusdb/v20190823/
+-rw-r--r--   0 root         (0) root         (0)    48988 2023-04-13 00:58:06.000000 tencentcloud-sdk-python-tcaplusdb-3.0.872/tencentcloud/tcaplusdb/v20190823/tcaplusdb_client.py
+-rw-r--r--   0 root         (0) root         (0)     3614 2023-04-13 00:58:06.000000 tencentcloud-sdk-python-tcaplusdb-3.0.872/tencentcloud/tcaplusdb/v20190823/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 00:58:06.000000 tencentcloud-sdk-python-tcaplusdb-3.0.872/tencentcloud/tcaplusdb/v20190823/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   195509 2023-04-13 00:58:06.000000 tencentcloud-sdk-python-tcaplusdb-3.0.872/tencentcloud/tcaplusdb/v20190823/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 00:58:06.000000 tencentcloud-sdk-python-tcaplusdb-3.0.872/tencentcloud_sdk_python_tcaplusdb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 00:58:06.000000 tencentcloud-sdk-python-tcaplusdb-3.0.872/tencentcloud_sdk_python_tcaplusdb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      505 2023-04-13 00:58:06.000000 tencentcloud-sdk-python-tcaplusdb-3.0.872/tencentcloud_sdk_python_tcaplusdb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1689 2023-04-13 00:58:06.000000 tencentcloud-sdk-python-tcaplusdb-3.0.872/tencentcloud_sdk_python_tcaplusdb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-13 00:58:06.000000 tencentcloud-sdk-python-tcaplusdb-3.0.872/tencentcloud_sdk_python_tcaplusdb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1689 2023-04-13 00:58:06.000000 tencentcloud-sdk-python-tcaplusdb-3.0.872/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1018 2023-04-13 00:58:06.000000 tencentcloud-sdk-python-tcaplusdb-3.0.872/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-13 00:58:06.000000 tencentcloud-sdk-python-tcaplusdb-3.0.872/setup.cfg
```

### Comparing `tencentcloud-sdk-python-tcaplusdb-3.0.871/PKG-INFO` & `tencentcloud-sdk-python-tcaplusdb-3.0.872/tencentcloud_sdk_python_tcaplusdb.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tcaplusdb
-Version: 3.0.871
+Version: 3.0.872
 Summary: Tencent Cloud Tcaplusdb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tcaplusdb-3.0.871/tencentcloud/tcaplusdb/v20190823/models.py` & `tencentcloud-sdk-python-tcaplusdb-3.0.872/tencentcloud/tcaplusdb/v20190823/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -190,14 +190,123 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class BackupExpireRuleInfo(AbstractModel):
+    """备份保留策略详情
+    集群策略： ClueterId=集群Id， TableGroupId=-1,  TableName="-1"
+    集群+表格组策略： ClueterId=集群Id， TableGroupId=表格组Id,  TableName="-1"
+    集群+表格组+表格策略： ClueterId=集群Id， TableGroupId=表格组Id,  TableName="表格名"
+
+    FileTag=0 txh引擎文件， =1 ulog流水文件， 当要设置为=1时， 这两项不可变 TableGroupId=-1和TableName="-1"
+    ExpireDay为大于等于1，小于999的整形数字
+    OperType=0 代表动作为新增， =1 代表动作为删除， =2 代表动作为修改， 其中0和2可以混用，后端实现兼容
+
+    """
+
+    def __init__(self):
+        r"""
+        :param TableGroupId: 所属表格组ID
+        :type TableGroupId: str
+        :param TableName: 表名称
+        :type TableName: str
+        :param FileTag: 文件标签，见上面描述
+        :type FileTag: int
+        :param ExpireDay: 淘汰天数，见上面描述
+        :type ExpireDay: int
+        :param OperType: 操作类型，见上面描述
+        :type OperType: int
+        """
+        self.TableGroupId = None
+        self.TableName = None
+        self.FileTag = None
+        self.ExpireDay = None
+        self.OperType = None
+
+
+    def _deserialize(self, params):
+        self.TableGroupId = params.get("TableGroupId")
+        self.TableName = params.get("TableName")
+        self.FileTag = params.get("FileTag")
+        self.ExpireDay = params.get("ExpireDay")
+        self.OperType = params.get("OperType")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class BackupRecords(AbstractModel):
+    """备份记录
+    作为出参时，每个字段都会填充
+    作为入参时， 原封不动将每个字段填回结构体， 注意只有FIleTag=OSDATA才可以调用此接口
+
+    """
+
+    def __init__(self):
+        r"""
+        :param ZoneId: 表格组ID
+        :type ZoneId: int
+        :param TableName: 表名称
+        :type TableName: str
+        :param BackupType: 备份源
+        :type BackupType: str
+        :param FileTag: 文件标签：TCAPLUS_FULL或OSDATA
+        :type FileTag: str
+        :param ShardCount: 分片数量
+        :type ShardCount: int
+        :param BackupBatchTime: 备份批次日期
+        :type BackupBatchTime: str
+        :param BackupFileSize: 备份文件汇总大小
+        :type BackupFileSize: int
+        :param BackupSuccRate: 备份成功率
+        :type BackupSuccRate: str
+        :param BackupExpireTime: 备份文件过期时间
+        :type BackupExpireTime: str
+        :param AppId: 业务ID
+        :type AppId: int
+        """
+        self.ZoneId = None
+        self.TableName = None
+        self.BackupType = None
+        self.FileTag = None
+        self.ShardCount = None
+        self.BackupBatchTime = None
+        self.BackupFileSize = None
+        self.BackupSuccRate = None
+        self.BackupExpireTime = None
+        self.AppId = None
+
+
+    def _deserialize(self, params):
+        self.ZoneId = params.get("ZoneId")
+        self.TableName = params.get("TableName")
+        self.BackupType = params.get("BackupType")
+        self.FileTag = params.get("FileTag")
+        self.ShardCount = params.get("ShardCount")
+        self.BackupBatchTime = params.get("BackupBatchTime")
+        self.BackupFileSize = params.get("BackupFileSize")
+        self.BackupSuccRate = params.get("BackupSuccRate")
+        self.BackupExpireTime = params.get("BackupExpireTime")
+        self.AppId = params.get("AppId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class ClearTablesRequest(AbstractModel):
     """ClearTables请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -933,14 +1042,69 @@
             for item in params.get("TableResults"):
                 obj = TableResultNew()
                 obj._deserialize(item)
                 self.TableResults.append(obj)
         self.RequestId = params.get("RequestId")
 
 
+class DeleteBackupRecordsRequest(AbstractModel):
+    """DeleteBackupRecords请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param ClusterId: 待删除备份记录的所在集群ID
+        :type ClusterId: str
+        :param BackupRecords: 待删除备份记录的详情
+        :type BackupRecords: list of BackupRecords
+        """
+        self.ClusterId = None
+        self.BackupRecords = None
+
+
+    def _deserialize(self, params):
+        self.ClusterId = params.get("ClusterId")
+        if params.get("BackupRecords") is not None:
+            self.BackupRecords = []
+            for item in params.get("BackupRecords"):
+                obj = BackupRecords()
+                obj._deserialize(item)
+                self.BackupRecords.append(obj)
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DeleteBackupRecordsResponse(AbstractModel):
+    """DeleteBackupRecords返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param TaskId: TaskId由 AppInstanceId-taskId 组成，以区分不同集群的任务
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TaskId: str
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.TaskId = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.TaskId = params.get("TaskId")
+        self.RequestId = params.get("RequestId")
+
+
 class DeleteClusterRequest(AbstractModel):
     """DeleteCluster请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -1424,14 +1588,84 @@
                 obj = Application()
                 obj._deserialize(item)
                 self.Applications.append(obj)
         self.TotalCount = params.get("TotalCount")
         self.RequestId = params.get("RequestId")
 
 
+class DescribeBackupRecordsRequest(AbstractModel):
+    """DescribeBackupRecords请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param ClusterId: 集群ID，用于获取指定集群的单据
+        :type ClusterId: str
+        :param Limit: 分页
+        :type Limit: int
+        :param Offset: 分页
+        :type Offset: int
+        :param TableGroupId: 表格组id，用于过滤
+        :type TableGroupId: str
+        :param TableName: 表格名，用于过滤
+        :type TableName: str
+        """
+        self.ClusterId = None
+        self.Limit = None
+        self.Offset = None
+        self.TableGroupId = None
+        self.TableName = None
+
+
+    def _deserialize(self, params):
+        self.ClusterId = params.get("ClusterId")
+        self.Limit = params.get("Limit")
+        self.Offset = params.get("Offset")
+        self.TableGroupId = params.get("TableGroupId")
+        self.TableName = params.get("TableName")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeBackupRecordsResponse(AbstractModel):
+    """DescribeBackupRecords返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param BackupRecords: 备份记录详情
+        :type BackupRecords: list of BackupRecords
+        :param TotalCount: 返回记录条数
+        :type TotalCount: int
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.BackupRecords = None
+        self.TotalCount = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        if params.get("BackupRecords") is not None:
+            self.BackupRecords = []
+            for item in params.get("BackupRecords"):
+                obj = BackupRecords()
+                obj._deserialize(item)
+                self.BackupRecords.append(obj)
+        self.TotalCount = params.get("TotalCount")
+        self.RequestId = params.get("RequestId")
+
+
 class DescribeClusterTagsRequest(AbstractModel):
     """DescribeClusterTags请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -4226,14 +4460,69 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class SetBackupExpireRuleRequest(AbstractModel):
+    """SetBackupExpireRule请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param ClusterId: 表所属集群实例ID
+        :type ClusterId: str
+        :param BackupExpireRules: 淘汰策略数组
+        :type BackupExpireRules: list of BackupExpireRuleInfo
+        """
+        self.ClusterId = None
+        self.BackupExpireRules = None
+
+
+    def _deserialize(self, params):
+        self.ClusterId = params.get("ClusterId")
+        if params.get("BackupExpireRules") is not None:
+            self.BackupExpireRules = []
+            for item in params.get("BackupExpireRules"):
+                obj = BackupExpireRuleInfo()
+                obj._deserialize(item)
+                self.BackupExpireRules.append(obj)
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class SetBackupExpireRuleResponse(AbstractModel):
+    """SetBackupExpireRule返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param TaskId: TaskId由 AppInstanceId-taskId 组成，以区分不同集群的任务
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TaskId: str
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.TaskId = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.TaskId = params.get("TaskId")
+        self.RequestId = params.get("RequestId")
+
+
 class SetTableDataFlowRequest(AbstractModel):
     """SetTableDataFlow请求参数结构体
 
     """
 
     def __init__(self):
         r"""
```

### Comparing `tencentcloud-sdk-python-tcaplusdb-3.0.871/tencentcloud/tcaplusdb/v20190823/errorcodes.py` & `tencentcloud-sdk-python-tcaplusdb-3.0.872/tencentcloud/tcaplusdb/v20190823/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tcaplusdb-3.0.871/tencentcloud/tcaplusdb/v20190823/tcaplusdb_client.py` & `tencentcloud-sdk-python-tcaplusdb-3.0.872/tencentcloud/tcaplusdb/v20190823/tcaplusdb_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -183,14 +183,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def DeleteBackupRecords(self, request):
+        """删除手工备份
+
+        :param request: Request instance for DeleteBackupRecords.
+        :type request: :class:`tencentcloud.tcaplusdb.v20190823.models.DeleteBackupRecordsRequest`
+        :rtype: :class:`tencentcloud.tcaplusdb.v20190823.models.DeleteBackupRecordsResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DeleteBackupRecords", params, headers=headers)
+            response = json.loads(body)
+            model = models.DeleteBackupRecordsResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def DeleteCluster(self, request):
         """删除TcaplusDB集群，必须在集群所属所有资源（包括表格组，表）都已经释放的情况下才会成功。
 
         :param request: Request instance for DeleteCluster.
         :type request: :class:`tencentcloud.tcaplusdb.v20190823.models.DeleteClusterRequest`
         :rtype: :class:`tencentcloud.tcaplusdb.v20190823.models.DeleteClusterResponse`
 
@@ -367,14 +390,41 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def DescribeBackupRecords(self, request):
+        """查询备份记录
+
+        查询集群级别时， 将TableGroupId设置为"-1", 将TableName设置为"-1"
+        查询集群+表格组级别时， 将TableName设置为"-1"
+        查询集群+表格组+表格级别时， 都不能设置为“-1”
+
+        :param request: Request instance for DescribeBackupRecords.
+        :type request: :class:`tencentcloud.tcaplusdb.v20190823.models.DescribeBackupRecordsRequest`
+        :rtype: :class:`tencentcloud.tcaplusdb.v20190823.models.DescribeBackupRecordsResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeBackupRecords", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeBackupRecordsResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def DescribeClusterTags(self, request):
         """获取集群关联的标签列表
 
         :param request: Request instance for DescribeClusterTags.
         :type request: :class:`tencentcloud.tcaplusdb.v20190823.models.DescribeClusterTagsRequest`
         :rtype: :class:`tencentcloud.tcaplusdb.v20190823.models.DescribeClusterTagsResponse`
 
@@ -1078,14 +1128,37 @@
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
+
+
+    def SetBackupExpireRule(self, request):
+        """新增、删除、修改备份过期策略， ClusterId必须为具体的集群Id（appid）
+
+        :param request: Request instance for SetBackupExpireRule.
+        :type request: :class:`tencentcloud.tcaplusdb.v20190823.models.SetBackupExpireRuleRequest`
+        :rtype: :class:`tencentcloud.tcaplusdb.v20190823.models.SetBackupExpireRuleResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("SetBackupExpireRule", params, headers=headers)
+            response = json.loads(body)
+            model = models.SetBackupExpireRuleResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
 
 
     def SetTableDataFlow(self, request):
         """新增、修改表格数据订阅
 
         :param request: Request instance for SetTableDataFlow.
         :type request: :class:`tencentcloud.tcaplusdb.v20190823.models.SetTableDataFlowRequest`
```

### Comparing `tencentcloud-sdk-python-tcaplusdb-3.0.871/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tcaplusdb-3.0.872/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tcaplusdb-3.0.871/README.rst` & `tencentcloud-sdk-python-tcaplusdb-3.0.872/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tcaplusdb-3.0.871/tencentcloud_sdk_python_tcaplusdb.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tcaplusdb-3.0.872/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tcaplusdb
-Version: 3.0.871
+Version: 3.0.872
 Summary: Tencent Cloud Tcaplusdb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tcaplusdb-3.0.871/setup.py` & `tencentcloud-sdk-python-tcaplusdb-3.0.872/setup.py`

 * *Files identical despite different names*

