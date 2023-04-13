# Comparing `tmp/tencentcloud-sdk-python-teo-3.0.871.tar.gz` & `tmp/tencentcloud-sdk-python-teo-3.0.872.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-teo-3.0.871.tar", last modified: Wed Apr 12 00:43:16 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-teo-3.0.872.tar", last modified: Thu Apr 13 01:02:44 2023, max compression
```

## Comparing `tencentcloud-sdk-python-teo-3.0.871.tar` & `tencentcloud-sdk-python-teo-3.0.872.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 00:43:16.000000 tencentcloud-sdk-python-teo-3.0.871/
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-12 00:43:16.000000 tencentcloud-sdk-python-teo-3.0.871/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 00:43:16.000000 tencentcloud-sdk-python-teo-3.0.871/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 00:43:16.000000 tencentcloud-sdk-python-teo-3.0.871/tencentcloud/teo/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 00:43:16.000000 tencentcloud-sdk-python-teo-3.0.871/tencentcloud/teo/v20220106/
--rw-r--r--   0 root         (0) root         (0)   468214 2023-04-12 00:43:16.000000 tencentcloud-sdk-python-teo-3.0.871/tencentcloud/teo/v20220106/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 00:43:16.000000 tencentcloud-sdk-python-teo-3.0.871/tencentcloud/teo/v20220106/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7631 2023-04-12 00:43:16.000000 tencentcloud-sdk-python-teo-3.0.871/tencentcloud/teo/v20220106/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    87643 2023-04-12 00:43:16.000000 tencentcloud-sdk-python-teo-3.0.871/tencentcloud/teo/v20220106/teo_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 00:43:16.000000 tencentcloud-sdk-python-teo-3.0.871/tencentcloud/teo/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 00:43:16.000000 tencentcloud-sdk-python-teo-3.0.871/tencentcloud/teo/v20220901/
--rw-r--r--   0 root         (0) root         (0)   504971 2023-04-12 00:43:16.000000 tencentcloud-sdk-python-teo-3.0.871/tencentcloud/teo/v20220901/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 00:43:16.000000 tencentcloud-sdk-python-teo-3.0.871/tencentcloud/teo/v20220901/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20875 2023-04-12 00:43:16.000000 tencentcloud-sdk-python-teo-3.0.871/tencentcloud/teo/v20220901/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    81864 2023-04-12 00:43:16.000000 tencentcloud-sdk-python-teo-3.0.871/tencentcloud/teo/v20220901/teo_client.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-12 00:43:16.000000 tencentcloud-sdk-python-teo-3.0.871/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-12 00:43:16.000000 tencentcloud-sdk-python-teo-3.0.871/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 00:43:16.000000 tencentcloud-sdk-python-teo-3.0.871/tencentcloud_sdk_python_teo.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-12 00:43:16.000000 tencentcloud-sdk-python-teo-3.0.871/tencentcloud_sdk_python_teo.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 00:43:16.000000 tencentcloud-sdk-python-teo-3.0.871/tencentcloud_sdk_python_teo.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-12 00:43:16.000000 tencentcloud-sdk-python-teo-3.0.871/tencentcloud_sdk_python_teo.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      603 2023-04-12 00:43:16.000000 tencentcloud-sdk-python-teo-3.0.871/tencentcloud_sdk_python_teo.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-12 00:43:16.000000 tencentcloud-sdk-python-teo-3.0.871/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-12 00:43:16.000000 tencentcloud-sdk-python-teo-3.0.871/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 01:02:44.000000 tencentcloud-sdk-python-teo-3.0.872/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-13 01:02:44.000000 tencentcloud-sdk-python-teo-3.0.872/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 01:02:44.000000 tencentcloud-sdk-python-teo-3.0.872/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 01:02:44.000000 tencentcloud-sdk-python-teo-3.0.872/tencentcloud/teo/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 01:02:44.000000 tencentcloud-sdk-python-teo-3.0.872/tencentcloud/teo/v20220106/
+-rw-r--r--   0 root         (0) root         (0)     7631 2023-04-13 01:02:44.000000 tencentcloud-sdk-python-teo-3.0.872/tencentcloud/teo/v20220106/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 01:02:44.000000 tencentcloud-sdk-python-teo-3.0.872/tencentcloud/teo/v20220106/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   468214 2023-04-13 01:02:44.000000 tencentcloud-sdk-python-teo-3.0.872/tencentcloud/teo/v20220106/models.py
+-rw-r--r--   0 root         (0) root         (0)    87643 2023-04-13 01:02:44.000000 tencentcloud-sdk-python-teo-3.0.872/tencentcloud/teo/v20220106/teo_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 01:02:44.000000 tencentcloud-sdk-python-teo-3.0.872/tencentcloud/teo/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 01:02:44.000000 tencentcloud-sdk-python-teo-3.0.872/tencentcloud/teo/v20220901/
+-rw-r--r--   0 root         (0) root         (0)    20875 2023-04-13 01:02:44.000000 tencentcloud-sdk-python-teo-3.0.872/tencentcloud/teo/v20220901/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 01:02:44.000000 tencentcloud-sdk-python-teo-3.0.872/tencentcloud/teo/v20220901/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   504803 2023-04-13 01:02:44.000000 tencentcloud-sdk-python-teo-3.0.872/tencentcloud/teo/v20220901/models.py
+-rw-r--r--   0 root         (0) root         (0)    81864 2023-04-13 01:02:44.000000 tencentcloud-sdk-python-teo-3.0.872/tencentcloud/teo/v20220901/teo_client.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-13 01:02:44.000000 tencentcloud-sdk-python-teo-3.0.872/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-13 01:02:44.000000 tencentcloud-sdk-python-teo-3.0.872/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 01:02:44.000000 tencentcloud-sdk-python-teo-3.0.872/tencentcloud_sdk_python_teo.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 01:02:44.000000 tencentcloud-sdk-python-teo-3.0.872/tencentcloud_sdk_python_teo.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      603 2023-04-13 01:02:44.000000 tencentcloud-sdk-python-teo-3.0.872/tencentcloud_sdk_python_teo.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-13 01:02:44.000000 tencentcloud-sdk-python-teo-3.0.872/tencentcloud_sdk_python_teo.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-13 01:02:44.000000 tencentcloud-sdk-python-teo-3.0.872/tencentcloud_sdk_python_teo.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-13 01:02:44.000000 tencentcloud-sdk-python-teo-3.0.872/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-13 01:02:44.000000 tencentcloud-sdk-python-teo-3.0.872/setup.cfg
```

### Comparing `tencentcloud-sdk-python-teo-3.0.871/PKG-INFO` & `tencentcloud-sdk-python-teo-3.0.872/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-teo
-Version: 3.0.871
+Version: 3.0.872
 Summary: Tencent Cloud Teo SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-teo-3.0.871/tencentcloud/teo/v20220106/models.py` & `tencentcloud-sdk-python-teo-3.0.872/tencentcloud/teo/v20220106/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.871/tencentcloud/teo/v20220106/errorcodes.py` & `tencentcloud-sdk-python-teo-3.0.872/tencentcloud/teo/v20220106/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.871/tencentcloud/teo/v20220106/teo_client.py` & `tencentcloud-sdk-python-teo-3.0.872/tencentcloud/teo/v20220106/teo_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.871/tencentcloud/teo/v20220901/models.py` & `tencentcloud-sdk-python-teo-3.0.872/tencentcloud/teo/v20220901/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -12960,17 +12960,17 @@
 
     def __init__(self):
         r"""
         :param Switch: 托管规则开关，取值有：
 <li> on：开启；</li>
 <li> off：关闭。</li>
         :type Switch: str
-        :param BlockRuleIDs: 黑名单，ID参考接口 [DescribeSecurityGroupManagedRules](https://tcloud4api.woa.com/document/product/1657/80807?!preview&!document=1)。
+        :param BlockRuleIDs: 黑名单ID列表，将规则ID加入本参数列表中代表该ID关闭，即该规则ID不再生效。
         :type BlockRuleIDs: list of int
-        :param ObserveRuleIDs: 观察模式ID列表，将规则ID加入本参数列表中代表该ID使用观察模式生效，即该规则ID进入观察模式。ID参考接口 [DescribeSecurityGroupManagedRules](https://tcloud4api.woa.com/document/product/1657/80807?!preview&!document=1)。
+        :param ObserveRuleIDs: 观察模式ID列表，将规则ID加入本参数列表中代表该ID使用观察模式生效，即该规则ID进入观察模式。
         :type ObserveRuleIDs: list of int
         """
         self.Switch = None
         self.BlockRuleIDs = None
         self.ObserveRuleIDs = None
```

### Comparing `tencentcloud-sdk-python-teo-3.0.871/tencentcloud/teo/v20220901/errorcodes.py` & `tencentcloud-sdk-python-teo-3.0.872/tencentcloud/teo/v20220901/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.871/tencentcloud/teo/v20220901/teo_client.py` & `tencentcloud-sdk-python-teo-3.0.872/tencentcloud/teo/v20220901/teo_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.871/tencentcloud/__init__.py` & `tencentcloud-sdk-python-teo-3.0.872/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-teo-3.0.871/README.rst` & `tencentcloud-sdk-python-teo-3.0.872/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.871/tencentcloud_sdk_python_teo.egg-info/PKG-INFO` & `tencentcloud-sdk-python-teo-3.0.872/tencentcloud_sdk_python_teo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-teo
-Version: 3.0.871
+Version: 3.0.872
 Summary: Tencent Cloud Teo SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-teo-3.0.871/tencentcloud_sdk_python_teo.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-teo-3.0.872/tencentcloud_sdk_python_teo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.871/setup.py` & `tencentcloud-sdk-python-teo-3.0.872/setup.py`

 * *Files identical despite different names*

