# Comparing `tmp/tencentcloud-sdk-python-cvm-3.0.871.tar.gz` & `tmp/tencentcloud-sdk-python-cvm-3.0.872.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cvm-3.0.871.tar", last modified: Wed Apr 12 00:21:23 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cvm-3.0.872.tar", last modified: Thu Apr 13 00:30:03 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cvm-3.0.871.tar` & `tencentcloud-sdk-python-cvm-3.0.872.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 00:21:23.000000 tencentcloud-sdk-python-cvm-3.0.871/
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-12 00:21:23.000000 tencentcloud-sdk-python-cvm-3.0.871/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 00:21:23.000000 tencentcloud-sdk-python-cvm-3.0.871/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-12 00:21:23.000000 tencentcloud-sdk-python-cvm-3.0.871/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 00:21:23.000000 tencentcloud-sdk-python-cvm-3.0.871/tencentcloud/cvm/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 00:21:23.000000 tencentcloud-sdk-python-cvm-3.0.871/tencentcloud/cvm/v20170312/
--rw-r--r--   0 root         (0) root         (0)   119282 2023-04-12 00:21:23.000000 tencentcloud-sdk-python-cvm-3.0.871/tencentcloud/cvm/v20170312/cvm_client.py
--rw-r--r--   0 root         (0) root         (0)   429546 2023-04-12 00:21:23.000000 tencentcloud-sdk-python-cvm-3.0.871/tencentcloud/cvm/v20170312/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 00:21:23.000000 tencentcloud-sdk-python-cvm-3.0.871/tencentcloud/cvm/v20170312/__init__.py
--rw-r--r--   0 root         (0) root         (0)    42551 2023-04-12 00:21:23.000000 tencentcloud-sdk-python-cvm-3.0.871/tencentcloud/cvm/v20170312/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 00:21:23.000000 tencentcloud-sdk-python-cvm-3.0.871/tencentcloud/cvm/__init__.py
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-12 00:21:23.000000 tencentcloud-sdk-python-cvm-3.0.871/README.rst
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-12 00:21:23.000000 tencentcloud-sdk-python-cvm-3.0.871/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-12 00:21:23.000000 tencentcloud-sdk-python-cvm-3.0.871/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 00:21:23.000000 tencentcloud-sdk-python-cvm-3.0.871/tencentcloud_sdk_python_cvm.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-12 00:21:23.000000 tencentcloud-sdk-python-cvm-3.0.871/tencentcloud_sdk_python_cvm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 00:21:23.000000 tencentcloud-sdk-python-cvm-3.0.871/tencentcloud_sdk_python_cvm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-12 00:21:23.000000 tencentcloud-sdk-python-cvm-3.0.871/tencentcloud_sdk_python_cvm.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-04-12 00:21:23.000000 tencentcloud-sdk-python-cvm-3.0.871/tencentcloud_sdk_python_cvm.egg-info/SOURCES.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 00:30:03.000000 tencentcloud-sdk-python-cvm-3.0.872/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-13 00:30:03.000000 tencentcloud-sdk-python-cvm-3.0.872/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 00:30:03.000000 tencentcloud-sdk-python-cvm-3.0.872/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 00:30:03.000000 tencentcloud-sdk-python-cvm-3.0.872/tencentcloud/cvm/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 00:30:03.000000 tencentcloud-sdk-python-cvm-3.0.872/tencentcloud/cvm/v20170312/
+-rw-r--r--   0 root         (0) root         (0)   119282 2023-04-13 00:30:03.000000 tencentcloud-sdk-python-cvm-3.0.872/tencentcloud/cvm/v20170312/cvm_client.py
+-rw-r--r--   0 root         (0) root         (0)    42551 2023-04-13 00:30:03.000000 tencentcloud-sdk-python-cvm-3.0.872/tencentcloud/cvm/v20170312/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 00:30:03.000000 tencentcloud-sdk-python-cvm-3.0.872/tencentcloud/cvm/v20170312/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   429673 2023-04-13 00:30:03.000000 tencentcloud-sdk-python-cvm-3.0.872/tencentcloud/cvm/v20170312/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 00:30:03.000000 tencentcloud-sdk-python-cvm-3.0.872/tencentcloud/cvm/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-13 00:30:03.000000 tencentcloud-sdk-python-cvm-3.0.872/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-13 00:30:03.000000 tencentcloud-sdk-python-cvm-3.0.872/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-13 00:30:03.000000 tencentcloud-sdk-python-cvm-3.0.872/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-13 00:30:03.000000 tencentcloud-sdk-python-cvm-3.0.872/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 00:30:03.000000 tencentcloud-sdk-python-cvm-3.0.872/tencentcloud_sdk_python_cvm.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 00:30:03.000000 tencentcloud-sdk-python-cvm-3.0.872/tencentcloud_sdk_python_cvm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-04-13 00:30:03.000000 tencentcloud-sdk-python-cvm-3.0.872/tencentcloud_sdk_python_cvm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-13 00:30:03.000000 tencentcloud-sdk-python-cvm-3.0.872/tencentcloud_sdk_python_cvm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-13 00:30:03.000000 tencentcloud-sdk-python-cvm-3.0.872/tencentcloud_sdk_python_cvm.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-cvm-3.0.871/PKG-INFO` & `tencentcloud-sdk-python-cvm-3.0.872/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cvm
-Version: 3.0.871
+Version: 3.0.872
 Summary: Tencent Cloud Cvm SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cvm-3.0.871/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cvm-3.0.872/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cvm-3.0.871/tencentcloud/cvm/v20170312/cvm_client.py` & `tencentcloud-sdk-python-cvm-3.0.872/tencentcloud/cvm/v20170312/cvm_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cvm-3.0.871/tencentcloud/cvm/v20170312/models.py` & `tencentcloud-sdk-python-cvm-3.0.872/tencentcloud/cvm/v20170312/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -367,18 +367,20 @@
         :type ChcId: str
         :param InstanceName: 实例名称。
         :type InstanceName: str
         :param SerialNumber: 服务器序列号。
         :type SerialNumber: str
         :param InstanceState: CHC的状态<br/>
 <ul>
-<li>REGISTERED: 设备已录入。还未配置带外和部署网络</li>
-<li>VPC_READY: 已配置带外和部署网络</li>
+<li>INIT: 设备已录入。还未配置带外和部署网络</li>
+<li>READY: 已配置带外和部署网络</li>
 <li>PREPARED: 可分配云主机</li>
 <li>ONLINE: 已分配云主机</li>
+<li>OPERATING: 设备操作中，如正在配置带外网络等。</li>
+<li>CLEAR_NETWORK_FAILED: 清理带外和部署网络失败</li>
 </ul>
         :type InstanceState: str
         :param DeviceType: 设备类型。
 注意：此字段可能返回 null，表示取不到有效值。
         :type DeviceType: str
         :param Placement: 所属可用区
         :type Placement: :class:`tencentcloud.cvm.v20170312.models.Placement`
```

### Comparing `tencentcloud-sdk-python-cvm-3.0.871/tencentcloud/cvm/v20170312/errorcodes.py` & `tencentcloud-sdk-python-cvm-3.0.872/tencentcloud/cvm/v20170312/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cvm-3.0.871/README.rst` & `tencentcloud-sdk-python-cvm-3.0.872/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cvm-3.0.871/setup.py` & `tencentcloud-sdk-python-cvm-3.0.872/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cvm-3.0.871/tencentcloud_sdk_python_cvm.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cvm-3.0.872/tencentcloud_sdk_python_cvm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cvm
-Version: 3.0.871
+Version: 3.0.872
 Summary: Tencent Cloud Cvm SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

