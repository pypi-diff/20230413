# Comparing `tmp/tencentcloud-sdk-python-gme-3.0.871.tar.gz` & `tmp/tencentcloud-sdk-python-gme-3.0.872.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-gme-3.0.871.tar", last modified: Wed Apr 12 00:25:15 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-gme-3.0.872.tar", last modified: Thu Apr 13 00:42:06 2023, max compression
```

## Comparing `tencentcloud-sdk-python-gme-3.0.871.tar` & `tencentcloud-sdk-python-gme-3.0.872.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 00:25:15.000000 tencentcloud-sdk-python-gme-3.0.871/
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-12 00:25:15.000000 tencentcloud-sdk-python-gme-3.0.871/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 00:25:15.000000 tencentcloud-sdk-python-gme-3.0.871/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-12 00:25:14.000000 tencentcloud-sdk-python-gme-3.0.871/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 00:25:15.000000 tencentcloud-sdk-python-gme-3.0.871/tencentcloud/gme/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 00:25:15.000000 tencentcloud-sdk-python-gme-3.0.871/tencentcloud/gme/v20180711/
--rw-r--r--   0 root         (0) root         (0)    33250 2023-04-12 00:25:14.000000 tencentcloud-sdk-python-gme-3.0.871/tencentcloud/gme/v20180711/gme_client.py
--rw-r--r--   0 root         (0) root         (0)   102841 2023-04-12 00:25:14.000000 tencentcloud-sdk-python-gme-3.0.871/tencentcloud/gme/v20180711/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 00:25:14.000000 tencentcloud-sdk-python-gme-3.0.871/tencentcloud/gme/v20180711/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3906 2023-04-12 00:25:14.000000 tencentcloud-sdk-python-gme-3.0.871/tencentcloud/gme/v20180711/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 00:25:14.000000 tencentcloud-sdk-python-gme-3.0.871/tencentcloud/gme/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 00:25:15.000000 tencentcloud-sdk-python-gme-3.0.871/tencentcloud_sdk_python_gme.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-12 00:25:15.000000 tencentcloud-sdk-python-gme-3.0.871/tencentcloud_sdk_python_gme.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 00:25:15.000000 tencentcloud-sdk-python-gme-3.0.871/tencentcloud_sdk_python_gme.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-12 00:25:15.000000 tencentcloud-sdk-python-gme-3.0.871/tencentcloud_sdk_python_gme.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-04-12 00:25:15.000000 tencentcloud-sdk-python-gme-3.0.871/tencentcloud_sdk_python_gme.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-12 00:25:14.000000 tencentcloud-sdk-python-gme-3.0.871/README.rst
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-12 00:25:14.000000 tencentcloud-sdk-python-gme-3.0.871/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-12 00:25:15.000000 tencentcloud-sdk-python-gme-3.0.871/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 00:42:06.000000 tencentcloud-sdk-python-gme-3.0.872/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-13 00:42:06.000000 tencentcloud-sdk-python-gme-3.0.872/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 00:42:06.000000 tencentcloud-sdk-python-gme-3.0.872/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-13 00:42:06.000000 tencentcloud-sdk-python-gme-3.0.872/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 00:42:06.000000 tencentcloud-sdk-python-gme-3.0.872/tencentcloud/gme/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 00:42:06.000000 tencentcloud-sdk-python-gme-3.0.872/tencentcloud/gme/v20180711/
+-rw-r--r--   0 root         (0) root         (0)    33250 2023-04-13 00:42:06.000000 tencentcloud-sdk-python-gme-3.0.872/tencentcloud/gme/v20180711/gme_client.py
+-rw-r--r--   0 root         (0) root         (0)     3906 2023-04-13 00:42:06.000000 tencentcloud-sdk-python-gme-3.0.872/tencentcloud/gme/v20180711/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 00:42:06.000000 tencentcloud-sdk-python-gme-3.0.872/tencentcloud/gme/v20180711/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   102841 2023-04-13 00:42:06.000000 tencentcloud-sdk-python-gme-3.0.872/tencentcloud/gme/v20180711/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 00:42:06.000000 tencentcloud-sdk-python-gme-3.0.872/tencentcloud/gme/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 00:42:06.000000 tencentcloud-sdk-python-gme-3.0.872/tencentcloud_sdk_python_gme.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 00:42:06.000000 tencentcloud-sdk-python-gme-3.0.872/tencentcloud_sdk_python_gme.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-04-13 00:42:06.000000 tencentcloud-sdk-python-gme-3.0.872/tencentcloud_sdk_python_gme.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-13 00:42:06.000000 tencentcloud-sdk-python-gme-3.0.872/tencentcloud_sdk_python_gme.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-13 00:42:06.000000 tencentcloud-sdk-python-gme-3.0.872/tencentcloud_sdk_python_gme.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-13 00:42:06.000000 tencentcloud-sdk-python-gme-3.0.872/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-13 00:42:06.000000 tencentcloud-sdk-python-gme-3.0.872/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-13 00:42:06.000000 tencentcloud-sdk-python-gme-3.0.872/setup.cfg
```

### Comparing `tencentcloud-sdk-python-gme-3.0.871/PKG-INFO` & `tencentcloud-sdk-python-gme-3.0.872/tencentcloud_sdk_python_gme.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-gme
-Version: 3.0.871
+Version: 3.0.872
 Summary: Tencent Cloud Gme SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-gme-3.0.871/tencentcloud/__init__.py` & `tencentcloud-sdk-python-gme-3.0.872/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-gme-3.0.871/tencentcloud/gme/v20180711/gme_client.py` & `tencentcloud-sdk-python-gme-3.0.872/tencentcloud/gme/v20180711/gme_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-gme-3.0.871/tencentcloud/gme/v20180711/models.py` & `tencentcloud-sdk-python-gme-3.0.872/tencentcloud/gme/v20180711/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-gme-3.0.871/tencentcloud/gme/v20180711/errorcodes.py` & `tencentcloud-sdk-python-gme-3.0.872/tencentcloud/gme/v20180711/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-gme-3.0.871/tencentcloud_sdk_python_gme.egg-info/PKG-INFO` & `tencentcloud-sdk-python-gme-3.0.872/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-gme
-Version: 3.0.871
+Version: 3.0.872
 Summary: Tencent Cloud Gme SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-gme-3.0.871/README.rst` & `tencentcloud-sdk-python-gme-3.0.872/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-gme-3.0.871/setup.py` & `tencentcloud-sdk-python-gme-3.0.872/setup.py`

 * *Files identical despite different names*

