# Comparing `tmp/google-cloud-video-transcoder-1.8.2.tar.gz` & `tmp/google-cloud-video-transcoder-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-video-transcoder-1.8.2.tar", last modified: Wed Apr 12 14:13:05 2023, max compression
+gzip compressed data, was "google-cloud-video-transcoder-1.9.0.tar", last modified: Thu Apr 13 14:17:14 2023, max compression
```

## Comparing `google-cloud-video-transcoder-1.8.2.tar` & `google-cloud-video-transcoder-1.9.0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-12 14:13:05.276766 google-cloud-video-transcoder-1.8.2/
--rw-rw-r--   0 root         (0)     1003    11358 2023-04-12 14:10:27.000000 google-cloud-video-transcoder-1.8.2/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-04-12 14:10:27.000000 google-cloud-video-transcoder-1.8.2/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4752 2023-04-12 14:13:05.276766 google-cloud-video-transcoder-1.8.2/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3809 2023-04-12 14:10:27.000000 google-cloud-video-transcoder-1.8.2/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-12 14:13:05.268765 google-cloud-video-transcoder-1.8.2/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-12 14:13:05.268765 google-cloud-video-transcoder-1.8.2/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-12 14:13:05.268765 google-cloud-video-transcoder-1.8.2/google/cloud/video/
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-12 14:13:05.272766 google-cloud-video-transcoder-1.8.2/google/cloud/video/transcoder/
--rw-rw-r--   0 root         (0)     1003     2310 2023-04-12 14:10:27.000000 google-cloud-video-transcoder-1.8.2/google/cloud/video/transcoder/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-04-12 14:10:27.000000 google-cloud-video-transcoder-1.8.2/google/cloud/video/transcoder/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       90 2023-04-12 14:10:27.000000 google-cloud-video-transcoder-1.8.2/google/cloud/video/transcoder/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-12 14:13:05.272766 google-cloud-video-transcoder-1.8.2/google/cloud/video/transcoder_v1/
--rw-rw-r--   0 root         (0)     1003     2120 2023-04-12 14:10:27.000000 google-cloud-video-transcoder-1.8.2/google/cloud/video/transcoder_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     3578 2023-04-12 14:10:27.000000 google-cloud-video-transcoder-1.8.2/google/cloud/video/transcoder_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-04-12 14:10:27.000000 google-cloud-video-transcoder-1.8.2/google/cloud/video/transcoder_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       90 2023-04-12 14:10:27.000000 google-cloud-video-transcoder-1.8.2/google/cloud/video/transcoder_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-12 14:13:05.272766 google-cloud-video-transcoder-1.8.2/google/cloud/video/transcoder_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-04-12 14:10:27.000000 google-cloud-video-transcoder-1.8.2/google/cloud/video/transcoder_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-12 14:13:05.272766 google-cloud-video-transcoder-1.8.2/google/cloud/video/transcoder_v1/services/transcoder_service/
--rw-rw-r--   0 root         (0)     1003      781 2023-04-12 14:10:27.000000 google-cloud-video-transcoder-1.8.2/google/cloud/video/transcoder_v1/services/transcoder_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    44332 2023-04-12 14:10:27.000000 google-cloud-video-transcoder-1.8.2/google/cloud/video/transcoder_v1/services/transcoder_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    55027 2023-04-12 14:10:27.000000 google-cloud-video-transcoder-1.8.2/google/cloud/video/transcoder_v1/services/transcoder_service/client.py
--rw-rw-r--   0 root         (0)     1003    10757 2023-04-12 14:10:27.000000 google-cloud-video-transcoder-1.8.2/google/cloud/video/transcoder_v1/services/transcoder_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-12 14:13:05.276766 google-cloud-video-transcoder-1.8.2/google/cloud/video/transcoder_v1/services/transcoder_service/transports/
--rw-rw-r--   0 root         (0)     1003     1442 2023-04-12 14:10:27.000000 google-cloud-video-transcoder-1.8.2/google/cloud/video/transcoder_v1/services/transcoder_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     8996 2023-04-12 14:10:27.000000 google-cloud-video-transcoder-1.8.2/google/cloud/video/transcoder_v1/services/transcoder_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    19710 2023-04-12 14:10:27.000000 google-cloud-video-transcoder-1.8.2/google/cloud/video/transcoder_v1/services/transcoder_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    20116 2023-04-12 14:10:27.000000 google-cloud-video-transcoder-1.8.2/google/cloud/video/transcoder_v1/services/transcoder_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    45416 2023-04-12 14:10:27.000000 google-cloud-video-transcoder-1.8.2/google/cloud/video/transcoder_v1/services/transcoder_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-12 14:13:05.276766 google-cloud-video-transcoder-1.8.2/google/cloud/video/transcoder_v1/types/
--rw-rw-r--   0 root         (0)     1003     1810 2023-04-12 14:10:27.000000 google-cloud-video-transcoder-1.8.2/google/cloud/video/transcoder_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    80339 2023-04-12 14:10:27.000000 google-cloud-video-transcoder-1.8.2/google/cloud/video/transcoder_v1/types/resources.py
--rw-rw-r--   0 root         (0)     1003     9069 2023-04-12 14:10:27.000000 google-cloud-video-transcoder-1.8.2/google/cloud/video/transcoder_v1/types/services.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-12 14:13:05.276766 google-cloud-video-transcoder-1.8.2/google_cloud_video_transcoder.egg-info/
--rw-r--r--   0 root         (0)     1003     4752 2023-04-12 14:13:05.000000 google-cloud-video-transcoder-1.8.2/google_cloud_video_transcoder.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     1828 2023-04-12 14:13:05.000000 google-cloud-video-transcoder-1.8.2/google_cloud_video_transcoder.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-04-12 14:13:05.000000 google-cloud-video-transcoder-1.8.2/google_cloud_video_transcoder.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       39 2023-04-12 14:13:05.000000 google-cloud-video-transcoder-1.8.2/google_cloud_video_transcoder.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-04-12 14:13:05.000000 google-cloud-video-transcoder-1.8.2/google_cloud_video_transcoder.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      315 2023-04-12 14:13:05.000000 google-cloud-video-transcoder-1.8.2/google_cloud_video_transcoder.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-04-12 14:13:05.000000 google-cloud-video-transcoder-1.8.2/google_cloud_video_transcoder.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-04-12 14:13:05.280767 google-cloud-video-transcoder-1.8.2/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2985 2023-04-12 14:10:27.000000 google-cloud-video-transcoder-1.8.2/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-12 14:13:05.276766 google-cloud-video-transcoder-1.8.2/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-04-12 14:10:27.000000 google-cloud-video-transcoder-1.8.2/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-12 14:13:05.276766 google-cloud-video-transcoder-1.8.2/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-04-12 14:10:27.000000 google-cloud-video-transcoder-1.8.2/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-12 14:13:05.276766 google-cloud-video-transcoder-1.8.2/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-04-12 14:10:27.000000 google-cloud-video-transcoder-1.8.2/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-12 14:13:05.276766 google-cloud-video-transcoder-1.8.2/tests/unit/gapic/transcoder_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-04-12 14:10:27.000000 google-cloud-video-transcoder-1.8.2/tests/unit/gapic/transcoder_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   255932 2023-04-12 14:10:27.000000 google-cloud-video-transcoder-1.8.2/tests/unit/gapic/transcoder_v1/test_transcoder_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-13 14:17:14.208412 google-cloud-video-transcoder-1.9.0/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-04-13 14:14:36.000000 google-cloud-video-transcoder-1.9.0/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-04-13 14:14:36.000000 google-cloud-video-transcoder-1.9.0/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4752 2023-04-13 14:17:14.208412 google-cloud-video-transcoder-1.9.0/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3809 2023-04-13 14:14:36.000000 google-cloud-video-transcoder-1.9.0/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-13 14:17:14.200410 google-cloud-video-transcoder-1.9.0/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-13 14:17:14.200410 google-cloud-video-transcoder-1.9.0/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-13 14:17:14.200410 google-cloud-video-transcoder-1.9.0/google/cloud/video/
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-13 14:17:14.200410 google-cloud-video-transcoder-1.9.0/google/cloud/video/transcoder/
+-rw-rw-r--   0 root         (0)     1003     2310 2023-04-13 14:14:36.000000 google-cloud-video-transcoder-1.9.0/google/cloud/video/transcoder/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-04-13 14:14:36.000000 google-cloud-video-transcoder-1.9.0/google/cloud/video/transcoder/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       90 2023-04-13 14:14:36.000000 google-cloud-video-transcoder-1.9.0/google/cloud/video/transcoder/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-13 14:17:14.200410 google-cloud-video-transcoder-1.9.0/google/cloud/video/transcoder_v1/
+-rw-rw-r--   0 root         (0)     1003     2120 2023-04-13 14:14:36.000000 google-cloud-video-transcoder-1.9.0/google/cloud/video/transcoder_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     3578 2023-04-13 14:14:36.000000 google-cloud-video-transcoder-1.9.0/google/cloud/video/transcoder_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-04-13 14:14:36.000000 google-cloud-video-transcoder-1.9.0/google/cloud/video/transcoder_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       90 2023-04-13 14:14:36.000000 google-cloud-video-transcoder-1.9.0/google/cloud/video/transcoder_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-13 14:17:14.200410 google-cloud-video-transcoder-1.9.0/google/cloud/video/transcoder_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-04-13 14:14:36.000000 google-cloud-video-transcoder-1.9.0/google/cloud/video/transcoder_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-13 14:17:14.204411 google-cloud-video-transcoder-1.9.0/google/cloud/video/transcoder_v1/services/transcoder_service/
+-rw-rw-r--   0 root         (0)     1003      781 2023-04-13 14:14:36.000000 google-cloud-video-transcoder-1.9.0/google/cloud/video/transcoder_v1/services/transcoder_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    44332 2023-04-13 14:14:36.000000 google-cloud-video-transcoder-1.9.0/google/cloud/video/transcoder_v1/services/transcoder_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    55027 2023-04-13 14:14:36.000000 google-cloud-video-transcoder-1.9.0/google/cloud/video/transcoder_v1/services/transcoder_service/client.py
+-rw-rw-r--   0 root         (0)     1003    10757 2023-04-13 14:14:36.000000 google-cloud-video-transcoder-1.9.0/google/cloud/video/transcoder_v1/services/transcoder_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-13 14:17:14.204411 google-cloud-video-transcoder-1.9.0/google/cloud/video/transcoder_v1/services/transcoder_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1442 2023-04-13 14:14:36.000000 google-cloud-video-transcoder-1.9.0/google/cloud/video/transcoder_v1/services/transcoder_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8996 2023-04-13 14:14:36.000000 google-cloud-video-transcoder-1.9.0/google/cloud/video/transcoder_v1/services/transcoder_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    19710 2023-04-13 14:14:36.000000 google-cloud-video-transcoder-1.9.0/google/cloud/video/transcoder_v1/services/transcoder_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    20116 2023-04-13 14:14:36.000000 google-cloud-video-transcoder-1.9.0/google/cloud/video/transcoder_v1/services/transcoder_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    45416 2023-04-13 14:14:36.000000 google-cloud-video-transcoder-1.9.0/google/cloud/video/transcoder_v1/services/transcoder_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-13 14:17:14.204411 google-cloud-video-transcoder-1.9.0/google/cloud/video/transcoder_v1/types/
+-rw-rw-r--   0 root         (0)     1003     1810 2023-04-13 14:14:36.000000 google-cloud-video-transcoder-1.9.0/google/cloud/video/transcoder_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    81436 2023-04-13 14:14:36.000000 google-cloud-video-transcoder-1.9.0/google/cloud/video/transcoder_v1/types/resources.py
+-rw-rw-r--   0 root         (0)     1003     9069 2023-04-13 14:14:36.000000 google-cloud-video-transcoder-1.9.0/google/cloud/video/transcoder_v1/types/services.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-13 14:17:14.204411 google-cloud-video-transcoder-1.9.0/google_cloud_video_transcoder.egg-info/
+-rw-r--r--   0 root         (0)     1003     4752 2023-04-13 14:17:14.000000 google-cloud-video-transcoder-1.9.0/google_cloud_video_transcoder.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     1828 2023-04-13 14:17:14.000000 google-cloud-video-transcoder-1.9.0/google_cloud_video_transcoder.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-04-13 14:17:14.000000 google-cloud-video-transcoder-1.9.0/google_cloud_video_transcoder.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       39 2023-04-13 14:17:14.000000 google-cloud-video-transcoder-1.9.0/google_cloud_video_transcoder.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-04-13 14:17:14.000000 google-cloud-video-transcoder-1.9.0/google_cloud_video_transcoder.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      315 2023-04-13 14:17:14.000000 google-cloud-video-transcoder-1.9.0/google_cloud_video_transcoder.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-04-13 14:17:14.000000 google-cloud-video-transcoder-1.9.0/google_cloud_video_transcoder.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-04-13 14:17:14.208412 google-cloud-video-transcoder-1.9.0/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2985 2023-04-13 14:14:36.000000 google-cloud-video-transcoder-1.9.0/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-13 14:17:14.204411 google-cloud-video-transcoder-1.9.0/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-04-13 14:14:36.000000 google-cloud-video-transcoder-1.9.0/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-13 14:17:14.204411 google-cloud-video-transcoder-1.9.0/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-04-13 14:14:36.000000 google-cloud-video-transcoder-1.9.0/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-13 14:17:14.204411 google-cloud-video-transcoder-1.9.0/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-04-13 14:14:36.000000 google-cloud-video-transcoder-1.9.0/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-13 14:17:14.208412 google-cloud-video-transcoder-1.9.0/tests/unit/gapic/transcoder_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-04-13 14:14:36.000000 google-cloud-video-transcoder-1.9.0/tests/unit/gapic/transcoder_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   256938 2023-04-13 14:14:36.000000 google-cloud-video-transcoder-1.9.0/tests/unit/gapic/transcoder_v1/test_transcoder_service.py
```

### Comparing `google-cloud-video-transcoder-1.8.2/LICENSE` & `google-cloud-video-transcoder-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-video-transcoder-1.8.2/MANIFEST.in` & `google-cloud-video-transcoder-1.9.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-video-transcoder-1.8.2/PKG-INFO` & `google-cloud-video-transcoder-1.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-video-transcoder
-Version: 1.8.2
+Version: 1.9.0
 Summary: Google Cloud Video Transcoder API client library
 Home-page: https://github.com/googleapis/python-video-transcoder
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-video-transcoder-1.8.2/README.rst` & `google-cloud-video-transcoder-1.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-video-transcoder-1.8.2/google/cloud/video/transcoder/__init__.py` & `google-cloud-video-transcoder-1.9.0/google/cloud/video/transcoder/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-transcoder-1.8.2/google/cloud/video/transcoder/gapic_version.py` & `google-cloud-video-transcoder-1.9.0/google/cloud/video/transcoder/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "1.8.2"  # {x-release-please-version}
+__version__ = "1.9.0"  # {x-release-please-version}
```

### Comparing `google-cloud-video-transcoder-1.8.2/google/cloud/video/transcoder_v1/__init__.py` & `google-cloud-video-transcoder-1.9.0/google/cloud/video/transcoder_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-transcoder-1.8.2/google/cloud/video/transcoder_v1/gapic_metadata.json` & `google-cloud-video-transcoder-1.9.0/google/cloud/video/transcoder_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-video-transcoder-1.8.2/google/cloud/video/transcoder_v1/gapic_version.py` & `google-cloud-video-transcoder-1.9.0/google/cloud/video/transcoder_v1/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "1.8.2"  # {x-release-please-version}
+__version__ = "1.9.0"  # {x-release-please-version}
```

### Comparing `google-cloud-video-transcoder-1.8.2/google/cloud/video/transcoder_v1/services/__init__.py` & `google-cloud-video-transcoder-1.9.0/google/cloud/video/transcoder_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-transcoder-1.8.2/google/cloud/video/transcoder_v1/services/transcoder_service/__init__.py` & `google-cloud-video-transcoder-1.9.0/google/cloud/video/transcoder_v1/services/transcoder_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-transcoder-1.8.2/google/cloud/video/transcoder_v1/services/transcoder_service/async_client.py` & `google-cloud-video-transcoder-1.9.0/google/cloud/video/transcoder_v1/services/transcoder_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-transcoder-1.8.2/google/cloud/video/transcoder_v1/services/transcoder_service/client.py` & `google-cloud-video-transcoder-1.9.0/google/cloud/video/transcoder_v1/services/transcoder_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-transcoder-1.8.2/google/cloud/video/transcoder_v1/services/transcoder_service/pagers.py` & `google-cloud-video-transcoder-1.9.0/google/cloud/video/transcoder_v1/services/transcoder_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-transcoder-1.8.2/google/cloud/video/transcoder_v1/services/transcoder_service/transports/__init__.py` & `google-cloud-video-transcoder-1.9.0/google/cloud/video/transcoder_v1/services/transcoder_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-transcoder-1.8.2/google/cloud/video/transcoder_v1/services/transcoder_service/transports/base.py` & `google-cloud-video-transcoder-1.9.0/google/cloud/video/transcoder_v1/services/transcoder_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-transcoder-1.8.2/google/cloud/video/transcoder_v1/services/transcoder_service/transports/grpc.py` & `google-cloud-video-transcoder-1.9.0/google/cloud/video/transcoder_v1/services/transcoder_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-transcoder-1.8.2/google/cloud/video/transcoder_v1/services/transcoder_service/transports/grpc_asyncio.py` & `google-cloud-video-transcoder-1.9.0/google/cloud/video/transcoder_v1/services/transcoder_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-transcoder-1.8.2/google/cloud/video/transcoder_v1/services/transcoder_service/transports/rest.py` & `google-cloud-video-transcoder-1.9.0/google/cloud/video/transcoder_v1/services/transcoder_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-transcoder-1.8.2/google/cloud/video/transcoder_v1/types/__init__.py` & `google-cloud-video-transcoder-1.9.0/google/cloud/video/transcoder_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-transcoder-1.8.2/google/cloud/video/transcoder_v1/types/resources.py` & `google-cloud-video-transcoder-1.9.0/google/cloud/video/transcoder_v1/types/resources.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,21 +75,18 @@
             ``Job.config.output.uri`` or
             ``JobTemplate.config.output.uri`` when using template. URI
             for the output file(s). For example,
             ``gs://my-bucket/outputs/``. See `Supported input and output
             formats <https://cloud.google.com/transcoder/docs/concepts/supported-input-and-output-formats>`__.
         template_id (str):
             Input only. Specify the ``template_id`` to use for
-            populating ``Job.config``. The default is ``preset/web-hd``.
+            populating ``Job.config``. The default is ``preset/web-hd``,
+            which is the only supported preset.
 
-            Preset Transcoder templates:
-
-            -  ``preset/{preset_id}``
-
-            -  User defined JobTemplate: ``{job_template_id}``
+            User defined JobTemplate: ``{job_template_id}``
 
             This field is a member of `oneof`_ ``job_config``.
         config (google.cloud.video.transcoder_v1.types.JobConfig):
             The configuration for this job.
 
             This field is a member of `oneof`_ ``job_config``.
         state (google.cloud.video.transcoder_v1.types.Job.ProcessingState):
@@ -110,14 +107,17 @@
         labels (MutableMapping[str, str]):
             The labels associated with this job. You can
             use these to organize and group your jobs.
         error (google.rpc.status_pb2.Status):
             Output only. An error object that describes the reason for
             the failure. This property is always present when ``state``
             is ``FAILED``.
+        mode (google.cloud.video.transcoder_v1.types.Job.ProcessingMode):
+            The processing mode of the job. The default is
+            ``PROCESSING_MODE_INTERACTIVE``.
     """
 
     class ProcessingState(proto.Enum):
         r"""The current state of the job.
 
         Values:
             PROCESSING_STATE_UNSPECIFIED (0):
@@ -135,14 +135,32 @@
         """
         PROCESSING_STATE_UNSPECIFIED = 0
         PENDING = 1
         RUNNING = 2
         SUCCEEDED = 3
         FAILED = 4
 
+    class ProcessingMode(proto.Enum):
+        r"""The processing mode of the job.
+
+        Values:
+            PROCESSING_MODE_UNSPECIFIED (0):
+                The job processing mode is not specified.
+            PROCESSING_MODE_INTERACTIVE (1):
+                The job processing mode is interactive mode.
+                Interactive job will either be ran or rejected
+                if quota does not allow for it.
+            PROCESSING_MODE_BATCH (2):
+                The job processing mode is batch mode.
+                Batch mode allows queuing of jobs.
+        """
+        PROCESSING_MODE_UNSPECIFIED = 0
+        PROCESSING_MODE_INTERACTIVE = 1
+        PROCESSING_MODE_BATCH = 2
+
     name: str = proto.Field(
         proto.STRING,
         number=1,
     )
     input_uri: str = proto.Field(
         proto.STRING,
         number=2,
@@ -192,14 +210,19 @@
         number=16,
     )
     error: status_pb2.Status = proto.Field(
         proto.MESSAGE,
         number=17,
         message=status_pb2.Status,
     )
+    mode: ProcessingMode = proto.Field(
+        proto.ENUM,
+        number=20,
+        enum=ProcessingMode,
+    )
 
 
 class JobTemplate(proto.Message):
     r"""Transcoding job template resource.
 
     Attributes:
         name (str):
@@ -781,21 +804,21 @@
         )
         y: float = proto.Field(
             proto.DOUBLE,
             number=2,
         )
 
     class Image(proto.Message):
-        r"""Overlaid jpeg image.
+        r"""Overlaid image.
 
         Attributes:
             uri (str):
-                Required. URI of the JPEG image in Cloud Storage. For
-                example, ``gs://bucket/inputs/image.jpeg``. JPEG is the only
-                supported image type.
+                Required. URI of the image in Cloud Storage. For example,
+                ``gs://bucket/inputs/image.png``. Only PNG and JPEG images
+                are supported.
             resolution (google.cloud.video.transcoder_v1.types.Overlay.NormalizedCoordinate):
                 Normalized image resolution, based on output video
                 resolution. Valid values: ``0.0``–``1.0``. To respect the
                 original image aspect ratio, set either ``x`` or ``y`` to
                 ``0.0``. To use the original image resolution, set both
                 ``x`` and ``y`` to ``0.0``.
             alpha (float):
@@ -2043,17 +2066,19 @@
         sample_rate_hertz (int):
             The audio sample rate in Hertz. The default
             is 48000 Hertz.
         language_code (str):
             The BCP-47 language code, such as ``en-US`` or ``sr-Latn``.
             For more information, see
             https://www.unicode.org/reports/tr35/#Unicode_locale_identifier.
+            Not supported in MP4 files.
         display_name (str):
             The name for this particular audio stream
-            that will be added to the HLS/DASH manifest.
+            that will be added to the HLS/DASH manifest. Not
+            supported in MP4 files.
     """
 
     class AudioMapping(proto.Message):
         r"""The mapping for the ``Job.edit_list`` atoms with audio
         ``EditAtom.inputs``.
 
         Attributes:
@@ -2152,20 +2177,22 @@
             -  ``cea608``
             -  ``cea708``
             -  ``webvtt``
         language_code (str):
             The BCP-47 language code, such as ``en-US`` or ``sr-Latn``.
             For more information, see
             https://www.unicode.org/reports/tr35/#Unicode_locale_identifier.
+            Not supported in MP4 files.
         mapping_ (MutableSequence[google.cloud.video.transcoder_v1.types.TextStream.TextMapping]):
             The mapping for the ``Job.edit_list`` atoms with text
             ``EditAtom.inputs``.
         display_name (str):
             The name for this particular text stream that
-            will be added to the HLS/DASH manifest.
+            will be added to the HLS/DASH manifest. Not
+            supported in MP4 files.
     """
 
     class TextMapping(proto.Message):
         r"""The mapping for the ``Job.edit_list`` atoms with text
         ``EditAtom.inputs``.
 
         Attributes:
```

### Comparing `google-cloud-video-transcoder-1.8.2/google/cloud/video/transcoder_v1/types/services.py` & `google-cloud-video-transcoder-1.9.0/google/cloud/video/transcoder_v1/types/services.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-transcoder-1.8.2/google_cloud_video_transcoder.egg-info/PKG-INFO` & `google-cloud-video-transcoder-1.9.0/google_cloud_video_transcoder.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-video-transcoder
-Version: 1.8.2
+Version: 1.9.0
 Summary: Google Cloud Video Transcoder API client library
 Home-page: https://github.com/googleapis/python-video-transcoder
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-video-transcoder-1.8.2/google_cloud_video_transcoder.egg-info/SOURCES.txt` & `google-cloud-video-transcoder-1.9.0/google_cloud_video_transcoder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-video-transcoder-1.8.2/setup.py` & `google-cloud-video-transcoder-1.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-transcoder-1.8.2/tests/__init__.py` & `google-cloud-video-transcoder-1.9.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-transcoder-1.8.2/tests/unit/__init__.py` & `google-cloud-video-transcoder-1.9.0/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-transcoder-1.8.2/tests/unit/gapic/__init__.py` & `google-cloud-video-transcoder-1.9.0/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-transcoder-1.8.2/tests/unit/gapic/transcoder_v1/__init__.py` & `google-cloud-video-transcoder-1.9.0/tests/unit/gapic/transcoder_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-transcoder-1.8.2/tests/unit/gapic/transcoder_v1/test_transcoder_service.py` & `google-cloud-video-transcoder-1.9.0/tests/unit/gapic/transcoder_v1/test_transcoder_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -758,14 +758,15 @@
         # Designate an appropriate return value for the call.
         call.return_value = resources.Job(
             name="name_value",
             input_uri="input_uri_value",
             output_uri="output_uri_value",
             state=resources.Job.ProcessingState.PENDING,
             ttl_after_completion_days=2670,
+            mode=resources.Job.ProcessingMode.PROCESSING_MODE_INTERACTIVE,
             template_id="template_id_value",
         )
         response = client.create_job(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
@@ -774,14 +775,15 @@
     # Establish that the response is the type that we expect.
     assert isinstance(response, resources.Job)
     assert response.name == "name_value"
     assert response.input_uri == "input_uri_value"
     assert response.output_uri == "output_uri_value"
     assert response.state == resources.Job.ProcessingState.PENDING
     assert response.ttl_after_completion_days == 2670
+    assert response.mode == resources.Job.ProcessingMode.PROCESSING_MODE_INTERACTIVE
 
 
 def test_create_job_empty_call():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = TranscoderServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -815,14 +817,15 @@
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
             resources.Job(
                 name="name_value",
                 input_uri="input_uri_value",
                 output_uri="output_uri_value",
                 state=resources.Job.ProcessingState.PENDING,
                 ttl_after_completion_days=2670,
+                mode=resources.Job.ProcessingMode.PROCESSING_MODE_INTERACTIVE,
             )
         )
         response = await client.create_job(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
@@ -831,14 +834,15 @@
     # Establish that the response is the type that we expect.
     assert isinstance(response, resources.Job)
     assert response.name == "name_value"
     assert response.input_uri == "input_uri_value"
     assert response.output_uri == "output_uri_value"
     assert response.state == resources.Job.ProcessingState.PENDING
     assert response.ttl_after_completion_days == 2670
+    assert response.mode == resources.Job.ProcessingMode.PROCESSING_MODE_INTERACTIVE
 
 
 @pytest.mark.asyncio
 async def test_create_job_async_from_dict():
     await test_create_job_async(request_type=dict)
 
 
@@ -1437,14 +1441,15 @@
         # Designate an appropriate return value for the call.
         call.return_value = resources.Job(
             name="name_value",
             input_uri="input_uri_value",
             output_uri="output_uri_value",
             state=resources.Job.ProcessingState.PENDING,
             ttl_after_completion_days=2670,
+            mode=resources.Job.ProcessingMode.PROCESSING_MODE_INTERACTIVE,
             template_id="template_id_value",
         )
         response = client.get_job(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
@@ -1453,14 +1458,15 @@
     # Establish that the response is the type that we expect.
     assert isinstance(response, resources.Job)
     assert response.name == "name_value"
     assert response.input_uri == "input_uri_value"
     assert response.output_uri == "output_uri_value"
     assert response.state == resources.Job.ProcessingState.PENDING
     assert response.ttl_after_completion_days == 2670
+    assert response.mode == resources.Job.ProcessingMode.PROCESSING_MODE_INTERACTIVE
 
 
 def test_get_job_empty_call():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = TranscoderServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -1494,14 +1500,15 @@
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
             resources.Job(
                 name="name_value",
                 input_uri="input_uri_value",
                 output_uri="output_uri_value",
                 state=resources.Job.ProcessingState.PENDING,
                 ttl_after_completion_days=2670,
+                mode=resources.Job.ProcessingMode.PROCESSING_MODE_INTERACTIVE,
             )
         )
         response = await client.get_job(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
@@ -1510,14 +1517,15 @@
     # Establish that the response is the type that we expect.
     assert isinstance(response, resources.Job)
     assert response.name == "name_value"
     assert response.input_uri == "input_uri_value"
     assert response.output_uri == "output_uri_value"
     assert response.state == resources.Job.ProcessingState.PENDING
     assert response.ttl_after_completion_days == 2670
+    assert response.mode == resources.Job.ProcessingMode.PROCESSING_MODE_INTERACTIVE
 
 
 @pytest.mark.asyncio
 async def test_get_job_async_from_dict():
     await test_get_job_async(request_type=dict)
 
 
@@ -3298,26 +3306,28 @@
             "details": [
                 {
                     "type_url": "type.googleapis.com/google.protobuf.Duration",
                     "value": b"\x08\x0c\x10\xdb\x07",
                 }
             ],
         },
+        "mode": 1,
     }
     request = request_type(**request_init)
 
     # Mock the http request call within the method and fake a response.
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
         return_value = resources.Job(
             name="name_value",
             input_uri="input_uri_value",
             output_uri="output_uri_value",
             state=resources.Job.ProcessingState.PENDING,
             ttl_after_completion_days=2670,
+            mode=resources.Job.ProcessingMode.PROCESSING_MODE_INTERACTIVE,
             template_id="template_id_value",
         )
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         pb_return_value = resources.Job.pb(return_value)
@@ -3330,14 +3340,15 @@
     # Establish that the response is the type that we expect.
     assert isinstance(response, resources.Job)
     assert response.name == "name_value"
     assert response.input_uri == "input_uri_value"
     assert response.output_uri == "output_uri_value"
     assert response.state == resources.Job.ProcessingState.PENDING
     assert response.ttl_after_completion_days == 2670
+    assert response.mode == resources.Job.ProcessingMode.PROCESSING_MODE_INTERACTIVE
 
 
 def test_create_job_rest_required_fields(request_type=services.CreateJobRequest):
     transport_class = transports.TranscoderServiceRestTransport
 
     request_init = {}
     request_init["parent"] = ""
@@ -3717,14 +3728,15 @@
             "details": [
                 {
                     "type_url": "type.googleapis.com/google.protobuf.Duration",
                     "value": b"\x08\x0c\x10\xdb\x07",
                 }
             ],
         },
+        "mode": 1,
     }
     request = request_type(**request_init)
 
     # Mock the http request call within the method and fake a BadRequest error.
     with mock.patch.object(Session, "request") as req, pytest.raises(
         core_exceptions.BadRequest
     ):
@@ -4160,14 +4172,15 @@
         # Designate an appropriate value for the returned response.
         return_value = resources.Job(
             name="name_value",
             input_uri="input_uri_value",
             output_uri="output_uri_value",
             state=resources.Job.ProcessingState.PENDING,
             ttl_after_completion_days=2670,
+            mode=resources.Job.ProcessingMode.PROCESSING_MODE_INTERACTIVE,
             template_id="template_id_value",
         )
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         pb_return_value = resources.Job.pb(return_value)
@@ -4180,14 +4193,15 @@
     # Establish that the response is the type that we expect.
     assert isinstance(response, resources.Job)
     assert response.name == "name_value"
     assert response.input_uri == "input_uri_value"
     assert response.output_uri == "output_uri_value"
     assert response.state == resources.Job.ProcessingState.PENDING
     assert response.ttl_after_completion_days == 2670
+    assert response.mode == resources.Job.ProcessingMode.PROCESSING_MODE_INTERACTIVE
 
 
 def test_get_job_rest_required_fields(request_type=services.GetJobRequest):
     transport_class = transports.TranscoderServiceRestTransport
 
     request_init = {}
     request_init["name"] = ""
```

