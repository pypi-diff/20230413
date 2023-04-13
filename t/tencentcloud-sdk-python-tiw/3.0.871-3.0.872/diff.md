# Comparing `tmp/tencentcloud-sdk-python-tiw-3.0.871.tar.gz` & `tmp/tencentcloud-sdk-python-tiw-3.0.872.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tiw-3.0.871.tar", last modified: Wed Apr 12 00:44:15 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tiw-3.0.872.tar", last modified: Thu Apr 13 01:06:45 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tiw-3.0.871.tar` & `tencentcloud-sdk-python-tiw-3.0.872.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 00:44:15.000000 tencentcloud-sdk-python-tiw-3.0.871/
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-12 00:44:15.000000 tencentcloud-sdk-python-tiw-3.0.871/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 00:44:15.000000 tencentcloud-sdk-python-tiw-3.0.871/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-12 00:44:15.000000 tencentcloud-sdk-python-tiw-3.0.871/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 00:44:15.000000 tencentcloud-sdk-python-tiw-3.0.871/tencentcloud/tiw/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 00:44:15.000000 tencentcloud-sdk-python-tiw-3.0.871/tencentcloud/tiw/v20190919/
--rw-r--r--   0 root         (0) root         (0)   185677 2023-04-12 00:44:15.000000 tencentcloud-sdk-python-tiw-3.0.871/tencentcloud/tiw/v20190919/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 00:44:15.000000 tencentcloud-sdk-python-tiw-3.0.871/tencentcloud/tiw/v20190919/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6089 2023-04-12 00:44:15.000000 tencentcloud-sdk-python-tiw-3.0.871/tencentcloud/tiw/v20190919/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    60210 2023-04-12 00:44:15.000000 tencentcloud-sdk-python-tiw-3.0.871/tencentcloud/tiw/v20190919/tiw_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 00:44:15.000000 tencentcloud-sdk-python-tiw-3.0.871/tencentcloud/tiw/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 00:44:15.000000 tencentcloud-sdk-python-tiw-3.0.871/tencentcloud_sdk_python_tiw.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-12 00:44:15.000000 tencentcloud-sdk-python-tiw-3.0.871/tencentcloud_sdk_python_tiw.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 00:44:15.000000 tencentcloud-sdk-python-tiw-3.0.871/tencentcloud_sdk_python_tiw.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-12 00:44:15.000000 tencentcloud-sdk-python-tiw-3.0.871/tencentcloud_sdk_python_tiw.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-04-12 00:44:15.000000 tencentcloud-sdk-python-tiw-3.0.871/tencentcloud_sdk_python_tiw.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-12 00:44:15.000000 tencentcloud-sdk-python-tiw-3.0.871/README.rst
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-12 00:44:15.000000 tencentcloud-sdk-python-tiw-3.0.871/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-12 00:44:15.000000 tencentcloud-sdk-python-tiw-3.0.871/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 01:06:45.000000 tencentcloud-sdk-python-tiw-3.0.872/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-13 01:06:44.000000 tencentcloud-sdk-python-tiw-3.0.872/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 01:06:45.000000 tencentcloud-sdk-python-tiw-3.0.872/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 01:06:45.000000 tencentcloud-sdk-python-tiw-3.0.872/tencentcloud/tiw/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 01:06:44.000000 tencentcloud-sdk-python-tiw-3.0.872/tencentcloud/tiw/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 01:06:45.000000 tencentcloud-sdk-python-tiw-3.0.872/tencentcloud/tiw/v20190919/
+-rw-r--r--   0 root         (0) root         (0)     6089 2023-04-13 01:06:45.000000 tencentcloud-sdk-python-tiw-3.0.872/tencentcloud/tiw/v20190919/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    60247 2023-04-13 01:06:45.000000 tencentcloud-sdk-python-tiw-3.0.872/tencentcloud/tiw/v20190919/tiw_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 01:06:45.000000 tencentcloud-sdk-python-tiw-3.0.872/tencentcloud/tiw/v20190919/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   185714 2023-04-13 01:06:45.000000 tencentcloud-sdk-python-tiw-3.0.872/tencentcloud/tiw/v20190919/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-13 01:06:44.000000 tencentcloud-sdk-python-tiw-3.0.872/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-13 01:06:45.000000 tencentcloud-sdk-python-tiw-3.0.872/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-13 01:06:44.000000 tencentcloud-sdk-python-tiw-3.0.872/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-13 01:06:45.000000 tencentcloud-sdk-python-tiw-3.0.872/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 01:06:45.000000 tencentcloud-sdk-python-tiw-3.0.872/tencentcloud_sdk_python_tiw.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 01:06:45.000000 tencentcloud-sdk-python-tiw-3.0.872/tencentcloud_sdk_python_tiw.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-04-13 01:06:45.000000 tencentcloud-sdk-python-tiw-3.0.872/tencentcloud_sdk_python_tiw.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-13 01:06:45.000000 tencentcloud-sdk-python-tiw-3.0.872/tencentcloud_sdk_python_tiw.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-13 01:06:45.000000 tencentcloud-sdk-python-tiw-3.0.872/tencentcloud_sdk_python_tiw.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-tiw-3.0.871/PKG-INFO` & `tencentcloud-sdk-python-tiw-3.0.872/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tiw
-Version: 3.0.871
+Version: 3.0.872
 Summary: Tencent Cloud Tiw SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tiw-3.0.871/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tiw-3.0.872/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tiw-3.0.871/tencentcloud/tiw/v20190919/models.py` & `tencentcloud-sdk-python-tiw-3.0.872/tencentcloud/tiw/v20190919/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -314,15 +314,15 @@
 
     """
 
     def __init__(self):
         r"""
         :param SdkAppId: 客户的SdkAppId
         :type SdkAppId: int
-        :param Url: 经过URL编码后的PPT文件地址。URL 编码会将字符转换为可通过因特网传输的格式，比如文档地址为http://example.com/测试.pptx，经过URL编码之后为http://example.com/%E6%B5%8B%E8%AF%95.pptx。为了提高URL解析的成功率，请对URL进行编码。
+        :param Url: 经过URL编码后的PPT文件地址。URL 编码会将字符转换为可通过因特网传输的格式，例如文档地址为http://example.com/测试.pptx，经过URL编码之后为http://example.com/%E6%B5%8B%E8%AF%95.pptx。为了提高URL解析的成功率，请对URL进行编码。
         :type Url: str
         :param AutoHandleUnsupportedElement: 是否对不支持元素开启自动处理的功能。默认不开启。
 
 在开启自动处理的情况下，会自动进行如下处理：
 1. 墨迹：移除不支持的墨迹（比如使用WPS画的）
 2. 自动翻页：移除PPT上所有的自动翻页设置，并设置为单击鼠标翻页
 3. 已损坏音视频：移除PPT上对损坏音视频的引用
@@ -3800,15 +3800,15 @@
 
     """
 
     def __init__(self):
         r"""
         :param SdkAppId: 客户的SdkAppId	
         :type SdkAppId: int
-        :param Callback: 进度回调地址，如果传空字符串会删除原来的回调地址配置，回调地址仅支持http或https协议，即回调地址以http://或https://开头。 回调数据格式请参考文档：https://cloud.tencent.com/document/product/1137/40260	
+        :param Callback: 进度回调地址，如果传空字符串会删除原来的回调地址配置，回调地址仅支持http或https协议，即回调地址以http://或https://开头。 回调数据格式请参考文档：https://cloud.tencent.com/document/product/1137/40260#c9cbe05f-fe1a-4410-b4dc-40cc301c7b81	
         :type Callback: str
         """
         self.SdkAppId = None
         self.Callback = None
 
 
     def _deserialize(self, params):
```

### Comparing `tencentcloud-sdk-python-tiw-3.0.871/tencentcloud/tiw/v20190919/errorcodes.py` & `tencentcloud-sdk-python-tiw-3.0.872/tencentcloud/tiw/v20190919/errorcodes.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,33 +31,33 @@
 
 # 文档格式错误，不支持转换只读文档或者已加密的文档。
 FAILEDOPERATION_FILEFORMATERROR = 'FailedOperation.FileFormatError'
 
 # 文档打开失败，请检查提交转码的文档是否加密或有其他格式问题。
 FAILEDOPERATION_FILEOPENFAIL = 'FailedOperation.FileOpenFail'
 
-# 转码后上传结果失败，请稍候重试。
+# 转码后上传结果失败，请稍后重试。
 FAILEDOPERATION_FILEUPLOADFAIL = 'FailedOperation.FileUploadFail'
 
 # 获取临时密钥失败。
 FAILEDOPERATION_GETCREDENTIALFAIL = 'FailedOperation.GetCredentialFail'
 
 # 转码预处理失败，具体请参考错误描述或联系客服人员。
 FAILEDOPERATION_PREPROCESS = 'FailedOperation.Preprocess'
 
-# 预处理服务出现内部错误，请稍候重试或联系客户人员。
+# 预处理服务出现内部错误，请稍后重试或联系客户人员。
 FAILEDOPERATION_PREPROCESSSERVERERROR = 'FailedOperation.PreprocessServerError'
 
 # 录制失败，具体请参考错误描述。
 FAILEDOPERATION_RECORD = 'FailedOperation.Record'
 
 # 转码失败，具体请参考错误描述或联系客服人员。
 FAILEDOPERATION_TRANSCODE = 'FailedOperation.Transcode'
 
-# 转码服务出现内部错误，请稍候重试或联系客户人员。
+# 转码服务出现内部错误，请稍后重试或联系客户人员。
 FAILEDOPERATION_TRANSCODESERVERERROR = 'FailedOperation.TranscodeServerError'
 
 # 白板推流失败，具体请参考错误描述。
 FAILEDOPERATION_WHITEBOARDPUSH = 'FailedOperation.WhiteboardPush'
 
 # 内部错误。
 INTERNALERROR = 'InternalError'
```

### Comparing `tencentcloud-sdk-python-tiw-3.0.871/tencentcloud/tiw/v20190919/tiw_client.py` & `tencentcloud-sdk-python-tiw-3.0.872/tencentcloud/tiw/v20190919/tiw_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1177,15 +1177,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def SetPPTCheckCallback(self, request):
-        """设置PPT检测任务回调地址，回调数据格式请参考文档：https://cloud.tencent.com/document/product/1137/40260
+        """设置PPT检测任务回调地址，回调数据格式请参考文档：https://cloud.tencent.com/document/product/1137/40260#c9cbe05f-fe1a-4410-b4dc-40cc301c7b81
 
         :param request: Request instance for SetPPTCheckCallback.
         :type request: :class:`tencentcloud.tiw.v20190919.models.SetPPTCheckCallbackRequest`
         :rtype: :class:`tencentcloud.tiw.v20190919.models.SetPPTCheckCallbackResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-tiw-3.0.871/tencentcloud_sdk_python_tiw.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tiw-3.0.872/tencentcloud_sdk_python_tiw.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tiw
-Version: 3.0.871
+Version: 3.0.872
 Summary: Tencent Cloud Tiw SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tiw-3.0.871/README.rst` & `tencentcloud-sdk-python-tiw-3.0.872/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tiw-3.0.871/setup.py` & `tencentcloud-sdk-python-tiw-3.0.872/setup.py`

 * *Files identical despite different names*

