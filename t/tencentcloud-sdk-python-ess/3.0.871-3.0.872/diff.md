# Comparing `tmp/tencentcloud-sdk-python-ess-3.0.871.tar.gz` & `tmp/tencentcloud-sdk-python-ess-3.0.872.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ess-3.0.871.tar", last modified: Wed Apr 12 00:24:30 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ess-3.0.872.tar", last modified: Thu Apr 13 00:41:18 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ess-3.0.871.tar` & `tencentcloud-sdk-python-ess-3.0.872.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 00:24:30.000000 tencentcloud-sdk-python-ess-3.0.871/
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-12 00:24:30.000000 tencentcloud-sdk-python-ess-3.0.871/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 00:24:30.000000 tencentcloud-sdk-python-ess-3.0.871/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-12 00:24:29.000000 tencentcloud-sdk-python-ess-3.0.871/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 00:24:30.000000 tencentcloud-sdk-python-ess-3.0.871/tencentcloud/ess/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 00:24:30.000000 tencentcloud-sdk-python-ess-3.0.871/tencentcloud/ess/v20201111/
--rw-r--r--   0 root         (0) root         (0)    47026 2023-04-12 00:24:29.000000 tencentcloud-sdk-python-ess-3.0.871/tencentcloud/ess/v20201111/ess_client.py
--rw-r--r--   0 root         (0) root         (0)   212473 2023-04-12 00:24:29.000000 tencentcloud-sdk-python-ess-3.0.871/tencentcloud/ess/v20201111/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 00:24:29.000000 tencentcloud-sdk-python-ess-3.0.871/tencentcloud/ess/v20201111/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23577 2023-04-12 00:24:29.000000 tencentcloud-sdk-python-ess-3.0.871/tencentcloud/ess/v20201111/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 00:24:29.000000 tencentcloud-sdk-python-ess-3.0.871/tencentcloud/ess/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 00:24:30.000000 tencentcloud-sdk-python-ess-3.0.871/tencentcloud_sdk_python_ess.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-12 00:24:30.000000 tencentcloud-sdk-python-ess-3.0.871/tencentcloud_sdk_python_ess.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 00:24:30.000000 tencentcloud-sdk-python-ess-3.0.871/tencentcloud_sdk_python_ess.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-12 00:24:30.000000 tencentcloud-sdk-python-ess-3.0.871/tencentcloud_sdk_python_ess.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-04-12 00:24:30.000000 tencentcloud-sdk-python-ess-3.0.871/tencentcloud_sdk_python_ess.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-12 00:24:29.000000 tencentcloud-sdk-python-ess-3.0.871/README.rst
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-12 00:24:29.000000 tencentcloud-sdk-python-ess-3.0.871/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-12 00:24:30.000000 tencentcloud-sdk-python-ess-3.0.871/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 00:41:18.000000 tencentcloud-sdk-python-ess-3.0.872/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-13 00:41:18.000000 tencentcloud-sdk-python-ess-3.0.872/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 00:41:18.000000 tencentcloud-sdk-python-ess-3.0.872/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-13 00:41:18.000000 tencentcloud-sdk-python-ess-3.0.872/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 00:41:18.000000 tencentcloud-sdk-python-ess-3.0.872/tencentcloud/ess/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 00:41:18.000000 tencentcloud-sdk-python-ess-3.0.872/tencentcloud/ess/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 00:41:18.000000 tencentcloud-sdk-python-ess-3.0.872/tencentcloud/ess/v20201111/
+-rw-r--r--   0 root         (0) root         (0)    47020 2023-04-13 00:41:18.000000 tencentcloud-sdk-python-ess-3.0.872/tencentcloud/ess/v20201111/ess_client.py
+-rw-r--r--   0 root         (0) root         (0)    23577 2023-04-13 00:41:18.000000 tencentcloud-sdk-python-ess-3.0.872/tencentcloud/ess/v20201111/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 00:41:18.000000 tencentcloud-sdk-python-ess-3.0.872/tencentcloud/ess/v20201111/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   212473 2023-04-13 00:41:18.000000 tencentcloud-sdk-python-ess-3.0.872/tencentcloud/ess/v20201111/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 00:41:18.000000 tencentcloud-sdk-python-ess-3.0.872/tencentcloud_sdk_python_ess.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 00:41:18.000000 tencentcloud-sdk-python-ess-3.0.872/tencentcloud_sdk_python_ess.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-04-13 00:41:18.000000 tencentcloud-sdk-python-ess-3.0.872/tencentcloud_sdk_python_ess.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-13 00:41:18.000000 tencentcloud-sdk-python-ess-3.0.872/tencentcloud_sdk_python_ess.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-13 00:41:18.000000 tencentcloud-sdk-python-ess-3.0.872/tencentcloud_sdk_python_ess.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-13 00:41:18.000000 tencentcloud-sdk-python-ess-3.0.872/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-13 00:41:18.000000 tencentcloud-sdk-python-ess-3.0.872/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-13 00:41:18.000000 tencentcloud-sdk-python-ess-3.0.872/setup.cfg
```

### Comparing `tencentcloud-sdk-python-ess-3.0.871/PKG-INFO` & `tencentcloud-sdk-python-ess-3.0.872/tencentcloud_sdk_python_ess.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ess
-Version: 3.0.871
+Version: 3.0.872
 Summary: Tencent Cloud Ess SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ess-3.0.871/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ess-3.0.872/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ess-3.0.871/tencentcloud/ess/v20201111/ess_client.py` & `tencentcloud-sdk-python-ess-3.0.872/tencentcloud/ess/v20201111/ess_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def CreateBatchCancelFlowUrl(self, request):
-        """电子签企业版：指定需要批量撤回的签署流程Id，获取批量撤销链接
+        """指定需要批量撤回的签署流程Id，获取批量撤销链接
         客户指定需要撤回的签署流程Id，最多100个，超过100不处理；接口调用成功返回批量撤回合同的链接，通过链接跳转到电子签小程序完成批量撤回
 
         :param request: Request instance for CreateBatchCancelFlowUrl.
         :type request: :class:`tencentcloud.ess.v20201111.models.CreateBatchCancelFlowUrlRequest`
         :rtype: :class:`tencentcloud.ess.v20201111.models.CreateBatchCancelFlowUrlResponse`
 
         """
@@ -298,15 +298,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def CreateFlowSignUrl(self, request):
-        """创建签署链接，请联系客户经理申请使用
+        """创建集成页面签署链接，请联系客户经理申请使用
 
         :param request: Request instance for CreateFlowSignUrl.
         :type request: :class:`tencentcloud.ess.v20201111.models.CreateFlowSignUrlRequest`
         :rtype: :class:`tencentcloud.ess.v20201111.models.CreateFlowSignUrlResponse`
 
         """
         try:
@@ -344,15 +344,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def CreateIntegrationUserRoles(self, request):
-        """集成版绑定员工角色
+        """绑定员工与对应角色
 
         :param request: Request instance for CreateIntegrationUserRoles.
         :type request: :class:`tencentcloud.ess.v20201111.models.CreateIntegrationUserRolesRequest`
         :rtype: :class:`tencentcloud.ess.v20201111.models.CreateIntegrationUserRolesResponse`
 
         """
         try:
@@ -463,15 +463,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def CreateSchemeUrl(self, request):
-        """获取小程序跳转链接
+        """获取小程序签署链接
 
         适用场景：如果需要签署人在自己的APP、小程序、H5应用中签署，可以通过此接口获取跳转腾讯电子签小程序的签署跳转链接。
 
         注：如果签署人是在PC端扫码签署，可以通过生成跳转链接自主转换成二维码，让签署人在PC端扫码签署。
 
 
         跳转到小程序的实现，参考官方文档（分为<a href="https://developers.weixin.qq.com/miniprogram/dev/api/navigate/wx.navigateToMiniProgram.html">全屏</a>、<a href="https://developers.weixin.qq.com/miniprogram/dev/framework/open-ability/openEmbeddedMiniProgram.html">半屏</a>两种方式）
@@ -565,15 +565,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DeleteIntegrationRoleUsers(self, request):
-        """解绑用户角色绑定关系
+        """解绑员工与对应角色关系
 
         :param request: Request instance for DeleteIntegrationRoleUsers.
         :type request: :class:`tencentcloud.ess.v20201111.models.DeleteIntegrationRoleUsersRequest`
         :rtype: :class:`tencentcloud.ess.v20201111.models.DeleteIntegrationRoleUsersResponse`
 
         """
         try:
@@ -730,15 +730,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DescribeIntegrationEmployees(self, request):
-        """查询员工信息，每次返回的数据量最大为20
+        """查询企业员工列表，每次返回的数据量最大为20
 
         :param request: Request instance for DescribeIntegrationEmployees.
         :type request: :class:`tencentcloud.ess.v20201111.models.DescribeIntegrationEmployeesRequest`
         :rtype: :class:`tencentcloud.ess.v20201111.models.DescribeIntegrationEmployeesResponse`
 
         """
         try:
@@ -776,15 +776,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DescribeIntegrationRoles(self, request):
-        """查询集成版角色
+        """查询企业角色列表
 
         :param request: Request instance for DescribeIntegrationRoles.
         :type request: :class:`tencentcloud.ess.v20201111.models.DescribeIntegrationRolesRequest`
         :rtype: :class:`tencentcloud.ess.v20201111.models.DescribeIntegrationRolesResponse`
 
         """
         try:
@@ -988,15 +988,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def UpdateIntegrationEmployees(self, request):
-        """更新集成版员工信息(姓名，手机号，邮件)，用户实名后无法更改姓名与手机号
+        """更新员工信息(姓名，手机号，邮件)，用户实名后无法更改姓名与手机号
 
         :param request: Request instance for UpdateIntegrationEmployees.
         :type request: :class:`tencentcloud.ess.v20201111.models.UpdateIntegrationEmployeesRequest`
         :rtype: :class:`tencentcloud.ess.v20201111.models.UpdateIntegrationEmployeesResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-ess-3.0.871/tencentcloud/ess/v20201111/models.py` & `tencentcloud-sdk-python-ess-3.0.872/tencentcloud/ess/v20201111/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.871/tencentcloud/ess/v20201111/errorcodes.py` & `tencentcloud-sdk-python-ess-3.0.872/tencentcloud/ess/v20201111/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.871/tencentcloud_sdk_python_ess.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ess-3.0.872/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ess
-Version: 3.0.871
+Version: 3.0.872
 Summary: Tencent Cloud Ess SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ess-3.0.871/README.rst` & `tencentcloud-sdk-python-ess-3.0.872/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.871/setup.py` & `tencentcloud-sdk-python-ess-3.0.872/setup.py`

 * *Files identical despite different names*

