# Comparing `tmp/tencentcloud-sdk-python-faceid-3.0.871.tar.gz` & `tmp/tencentcloud-sdk-python-faceid-3.0.872.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-faceid-3.0.871.tar", last modified: Wed Apr 12 00:24:49 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-faceid-3.0.872.tar", last modified: Thu Apr 13 00:41:37 2023, max compression
```

## Comparing `tencentcloud-sdk-python-faceid-3.0.871.tar` & `tencentcloud-sdk-python-faceid-3.0.872.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 00:24:49.000000 tencentcloud-sdk-python-faceid-3.0.871/
--rw-r--r--   0 root         (0) root         (0)     1674 2023-04-12 00:24:49.000000 tencentcloud-sdk-python-faceid-3.0.871/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 00:24:49.000000 tencentcloud-sdk-python-faceid-3.0.871/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 00:24:49.000000 tencentcloud-sdk-python-faceid-3.0.871/tencentcloud/faceid/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 00:24:48.000000 tencentcloud-sdk-python-faceid-3.0.871/tencentcloud/faceid/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 00:24:49.000000 tencentcloud-sdk-python-faceid-3.0.871/tencentcloud/faceid/v20180301/
--rw-r--r--   0 root         (0) root         (0)   139320 2023-04-12 00:24:48.000000 tencentcloud-sdk-python-faceid-3.0.871/tencentcloud/faceid/v20180301/models.py
--rw-r--r--   0 root         (0) root         (0)    34030 2023-04-12 00:24:48.000000 tencentcloud-sdk-python-faceid-3.0.871/tencentcloud/faceid/v20180301/faceid_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 00:24:48.000000 tencentcloud-sdk-python-faceid-3.0.871/tencentcloud/faceid/v20180301/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9370 2023-04-12 00:24:48.000000 tencentcloud-sdk-python-faceid-3.0.871/tencentcloud/faceid/v20180301/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-12 00:24:48.000000 tencentcloud-sdk-python-faceid-3.0.871/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)      746 2023-04-12 00:24:48.000000 tencentcloud-sdk-python-faceid-3.0.871/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 00:24:49.000000 tencentcloud-sdk-python-faceid-3.0.871/tencentcloud_sdk_python_faceid.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1674 2023-04-12 00:24:49.000000 tencentcloud-sdk-python-faceid-3.0.871/tencentcloud_sdk_python_faceid.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 00:24:49.000000 tencentcloud-sdk-python-faceid-3.0.871/tencentcloud_sdk_python_faceid.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-12 00:24:49.000000 tencentcloud-sdk-python-faceid-3.0.871/tencentcloud_sdk_python_faceid.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      475 2023-04-12 00:24:49.000000 tencentcloud-sdk-python-faceid-3.0.871/tencentcloud_sdk_python_faceid.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1012 2023-04-12 00:24:48.000000 tencentcloud-sdk-python-faceid-3.0.871/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-12 00:24:49.000000 tencentcloud-sdk-python-faceid-3.0.871/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 00:41:37.000000 tencentcloud-sdk-python-faceid-3.0.872/
+-rw-r--r--   0 root         (0) root         (0)      746 2023-04-13 00:41:37.000000 tencentcloud-sdk-python-faceid-3.0.872/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 00:41:37.000000 tencentcloud-sdk-python-faceid-3.0.872/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 00:41:37.000000 tencentcloud-sdk-python-faceid-3.0.872/tencentcloud/faceid/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 00:41:37.000000 tencentcloud-sdk-python-faceid-3.0.872/tencentcloud/faceid/v20180301/
+-rw-r--r--   0 root         (0) root         (0)    34030 2023-04-13 00:41:37.000000 tencentcloud-sdk-python-faceid-3.0.872/tencentcloud/faceid/v20180301/faceid_client.py
+-rw-r--r--   0 root         (0) root         (0)     9370 2023-04-13 00:41:37.000000 tencentcloud-sdk-python-faceid-3.0.872/tencentcloud/faceid/v20180301/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 00:41:37.000000 tencentcloud-sdk-python-faceid-3.0.872/tencentcloud/faceid/v20180301/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   139760 2023-04-13 00:41:37.000000 tencentcloud-sdk-python-faceid-3.0.872/tencentcloud/faceid/v20180301/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 00:41:37.000000 tencentcloud-sdk-python-faceid-3.0.872/tencentcloud/faceid/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-13 00:41:37.000000 tencentcloud-sdk-python-faceid-3.0.872/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-04-13 00:41:37.000000 tencentcloud-sdk-python-faceid-3.0.872/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1012 2023-04-13 00:41:37.000000 tencentcloud-sdk-python-faceid-3.0.872/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 00:41:37.000000 tencentcloud-sdk-python-faceid-3.0.872/tencentcloud_sdk_python_faceid.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 00:41:37.000000 tencentcloud-sdk-python-faceid-3.0.872/tencentcloud_sdk_python_faceid.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      475 2023-04-13 00:41:37.000000 tencentcloud-sdk-python-faceid-3.0.872/tencentcloud_sdk_python_faceid.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-04-13 00:41:37.000000 tencentcloud-sdk-python-faceid-3.0.872/tencentcloud_sdk_python_faceid.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-13 00:41:37.000000 tencentcloud-sdk-python-faceid-3.0.872/tencentcloud_sdk_python_faceid.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-13 00:41:37.000000 tencentcloud-sdk-python-faceid-3.0.872/setup.cfg
```

### Comparing `tencentcloud-sdk-python-faceid-3.0.871/PKG-INFO` & `tencentcloud-sdk-python-faceid-3.0.872/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-faceid
-Version: 3.0.871
+Version: 3.0.872
 Summary: Tencent Cloud Faceid SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-faceid-3.0.871/tencentcloud/faceid/v20180301/models.py` & `tencentcloud-sdk-python-faceid-3.0.872/tencentcloud/faceid/v20180301/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1123,14 +1123,20 @@
         :type LivenessMode: int
         :param NFCRequestIds: nfc重复计费requestId列表
 注意：此字段可能返回 null，表示取不到有效值。
         :type NFCRequestIds: list of str
         :param NFCBillingCounts: nfc重复计费计数
 注意：此字段可能返回 null，表示取不到有效值。
         :type NFCBillingCounts: int
+        :param PassNo: 港澳台居住证通行证号码
+注意：此字段可能返回 null，表示取不到有效值。
+        :type PassNo: str
+        :param VisaNum: 港澳台居住证签发次数
+注意：此字段可能返回 null，表示取不到有效值。
+        :type VisaNum: str
         """
         self.ErrCode = None
         self.ErrMsg = None
         self.IdCard = None
         self.Name = None
         self.OcrNation = None
         self.OcrAddress = None
@@ -1150,14 +1156,16 @@
         self.Extra = None
         self.LivenessDetail = None
         self.Mobile = None
         self.CompareLibType = None
         self.LivenessMode = None
         self.NFCRequestIds = None
         self.NFCBillingCounts = None
+        self.PassNo = None
+        self.VisaNum = None
 
 
     def _deserialize(self, params):
         self.ErrCode = params.get("ErrCode")
         self.ErrMsg = params.get("ErrMsg")
         self.IdCard = params.get("IdCard")
         self.Name = params.get("Name")
@@ -1184,14 +1192,16 @@
                 obj._deserialize(item)
                 self.LivenessDetail.append(obj)
         self.Mobile = params.get("Mobile")
         self.CompareLibType = params.get("CompareLibType")
         self.LivenessMode = params.get("LivenessMode")
         self.NFCRequestIds = params.get("NFCRequestIds")
         self.NFCBillingCounts = params.get("NFCBillingCounts")
+        self.PassNo = params.get("PassNo")
+        self.VisaNum = params.get("VisaNum")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-faceid-3.0.871/tencentcloud/faceid/v20180301/faceid_client.py` & `tencentcloud-sdk-python-faceid-3.0.872/tencentcloud/faceid/v20180301/faceid_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-faceid-3.0.871/tencentcloud/faceid/v20180301/errorcodes.py` & `tencentcloud-sdk-python-faceid-3.0.872/tencentcloud/faceid/v20180301/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-faceid-3.0.871/tencentcloud/__init__.py` & `tencentcloud-sdk-python-faceid-3.0.872/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-faceid-3.0.871/README.rst` & `tencentcloud-sdk-python-faceid-3.0.872/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-faceid-3.0.871/tencentcloud_sdk_python_faceid.egg-info/PKG-INFO` & `tencentcloud-sdk-python-faceid-3.0.872/tencentcloud_sdk_python_faceid.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-faceid
-Version: 3.0.871
+Version: 3.0.872
 Summary: Tencent Cloud Faceid SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-faceid-3.0.871/setup.py` & `tencentcloud-sdk-python-faceid-3.0.872/setup.py`

 * *Files identical despite different names*

