# Comparing `tmp/tencentcloud-sdk-python-aiart-3.0.871.tar.gz` & `tmp/tencentcloud-sdk-python-aiart-3.0.872.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-aiart-3.0.871.tar", last modified: Wed Apr 12 00:14:22 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-aiart-3.0.872.tar", last modified: Thu Apr 13 00:16:46 2023, max compression
```

## Comparing `tencentcloud-sdk-python-aiart-3.0.871.tar` & `tencentcloud-sdk-python-aiart-3.0.872.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 00:14:22.000000 tencentcloud-sdk-python-aiart-3.0.871/
--rw-r--r--   0 root         (0) root         (0)     1669 2023-04-12 00:14:22.000000 tencentcloud-sdk-python-aiart-3.0.871/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 00:14:22.000000 tencentcloud-sdk-python-aiart-3.0.871/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 00:14:22.000000 tencentcloud-sdk-python-aiart-3.0.871/tencentcloud/aiart/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 00:14:22.000000 tencentcloud-sdk-python-aiart-3.0.871/tencentcloud/aiart/v20221229/
--rw-r--r--   0 root         (0) root         (0)    11656 2023-04-12 00:14:21.000000 tencentcloud-sdk-python-aiart-3.0.871/tencentcloud/aiart/v20221229/models.py
--rw-r--r--   0 root         (0) root         (0)     3668 2023-04-12 00:14:21.000000 tencentcloud-sdk-python-aiart-3.0.871/tencentcloud/aiart/v20221229/aiart_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 00:14:21.000000 tencentcloud-sdk-python-aiart-3.0.871/tencentcloud/aiart/v20221229/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3566 2023-04-12 00:14:21.000000 tencentcloud-sdk-python-aiart-3.0.871/tencentcloud/aiart/v20221229/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 00:14:21.000000 tencentcloud-sdk-python-aiart-3.0.871/tencentcloud/aiart/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-12 00:14:21.000000 tencentcloud-sdk-python-aiart-3.0.871/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)      743 2023-04-12 00:14:21.000000 tencentcloud-sdk-python-aiart-3.0.871/README.rst
--rw-r--r--   0 root         (0) root         (0)     1010 2023-04-12 00:14:21.000000 tencentcloud-sdk-python-aiart-3.0.871/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 00:14:22.000000 tencentcloud-sdk-python-aiart-3.0.871/tencentcloud_sdk_python_aiart.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1669 2023-04-12 00:14:22.000000 tencentcloud-sdk-python-aiart-3.0.871/tencentcloud_sdk_python_aiart.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 00:14:22.000000 tencentcloud-sdk-python-aiart-3.0.871/tencentcloud_sdk_python_aiart.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-12 00:14:22.000000 tencentcloud-sdk-python-aiart-3.0.871/tencentcloud_sdk_python_aiart.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      465 2023-04-12 00:14:22.000000 tencentcloud-sdk-python-aiart-3.0.871/tencentcloud_sdk_python_aiart.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-12 00:14:22.000000 tencentcloud-sdk-python-aiart-3.0.871/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 00:16:46.000000 tencentcloud-sdk-python-aiart-3.0.872/
+-rw-r--r--   0 root         (0) root         (0)      743 2023-04-13 00:16:46.000000 tencentcloud-sdk-python-aiart-3.0.872/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 00:16:46.000000 tencentcloud-sdk-python-aiart-3.0.872/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-13 00:16:46.000000 tencentcloud-sdk-python-aiart-3.0.872/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 00:16:46.000000 tencentcloud-sdk-python-aiart-3.0.872/tencentcloud/aiart/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 00:16:46.000000 tencentcloud-sdk-python-aiart-3.0.872/tencentcloud/aiart/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 00:16:46.000000 tencentcloud-sdk-python-aiart-3.0.872/tencentcloud/aiart/v20221229/
+-rw-r--r--   0 root         (0) root         (0)     3578 2023-04-13 00:16:46.000000 tencentcloud-sdk-python-aiart-3.0.872/tencentcloud/aiart/v20221229/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)     3668 2023-04-13 00:16:46.000000 tencentcloud-sdk-python-aiart-3.0.872/tencentcloud/aiart/v20221229/aiart_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 00:16:46.000000 tencentcloud-sdk-python-aiart-3.0.872/tencentcloud/aiart/v20221229/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11656 2023-04-13 00:16:46.000000 tencentcloud-sdk-python-aiart-3.0.872/tencentcloud/aiart/v20221229/models.py
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-04-13 00:16:46.000000 tencentcloud-sdk-python-aiart-3.0.872/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1010 2023-04-13 00:16:46.000000 tencentcloud-sdk-python-aiart-3.0.872/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-13 00:16:46.000000 tencentcloud-sdk-python-aiart-3.0.872/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 00:16:46.000000 tencentcloud-sdk-python-aiart-3.0.872/tencentcloud_sdk_python_aiart.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 00:16:46.000000 tencentcloud-sdk-python-aiart-3.0.872/tencentcloud_sdk_python_aiart.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      465 2023-04-13 00:16:46.000000 tencentcloud-sdk-python-aiart-3.0.872/tencentcloud_sdk_python_aiart.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-04-13 00:16:46.000000 tencentcloud-sdk-python-aiart-3.0.872/tencentcloud_sdk_python_aiart.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-13 00:16:46.000000 tencentcloud-sdk-python-aiart-3.0.872/tencentcloud_sdk_python_aiart.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-aiart-3.0.871/PKG-INFO` & `tencentcloud-sdk-python-aiart-3.0.872/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-aiart
-Version: 3.0.871
+Version: 3.0.872
 Summary: Tencent Cloud Aiart SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-aiart-3.0.871/tencentcloud/aiart/v20221229/models.py` & `tencentcloud-sdk-python-aiart-3.0.872/tencentcloud/aiart/v20221229/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-aiart-3.0.871/tencentcloud/aiart/v20221229/aiart_client.py` & `tencentcloud-sdk-python-aiart-3.0.872/tencentcloud/aiart/v20221229/aiart_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-aiart-3.0.871/tencentcloud/aiart/v20221229/errorcodes.py` & `tencentcloud-sdk-python-aiart-3.0.872/tencentcloud/aiart/v20221229/errorcodes.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,18 +64,18 @@
 
 # 输入文本过长，请更换短一点的文本后重试。
 INVALIDPARAMETERVALUE_TEXTLENGTHEXCEED = 'InvalidParameterValue.TextLengthExceed'
 
 # URL格式不合法。
 INVALIDPARAMETERVALUE_URLILLEGAL = 'InvalidParameterValue.UrlIllegal'
 
-# 图片包含非法信息，审核不通过。
+# 图片包含违法违规信息，审核不通过。
 OPERATIONDENIED_IMAGEILLEGALDETECTED = 'OperationDenied.ImageIllegalDetected'
 
-# 文本包含非法信息，审核不通过。
+# 文本包含违法违规信息，审核不通过。
 OPERATIONDENIED_TEXTILLEGALDETECTED = 'OperationDenied.TextIllegalDetected'
 
 # 请求的次数超过了频率限制。
 REQUESTLIMITEXCEEDED = 'RequestLimitExceeded'
 
 # 资源正在发货中。
 RESOURCEUNAVAILABLE_DELIVERING = 'ResourceUnavailable.Delivering'
```

### Comparing `tencentcloud-sdk-python-aiart-3.0.871/tencentcloud/__init__.py` & `tencentcloud-sdk-python-aiart-3.0.872/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-aiart-3.0.871/README.rst` & `tencentcloud-sdk-python-aiart-3.0.872/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-aiart-3.0.871/setup.py` & `tencentcloud-sdk-python-aiart-3.0.872/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-aiart-3.0.871/tencentcloud_sdk_python_aiart.egg-info/PKG-INFO` & `tencentcloud-sdk-python-aiart-3.0.872/tencentcloud_sdk_python_aiart.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-aiart
-Version: 3.0.871
+Version: 3.0.872
 Summary: Tencent Cloud Aiart SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

