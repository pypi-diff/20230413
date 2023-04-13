# Comparing `tmp/alibabacloud_eventbridge20200401-1.0.6.tar.gz` & `tmp/alibabacloud_eventbridge20200401-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_eventbridge20200401-1.0.6.tar", last modified: Fri Apr  7 03:45:29 2023, max compression
+gzip compressed data, was "dist/alibabacloud_eventbridge20200401-1.0.7.tar", last modified: Thu Apr 13 01:46:35 2023, max compression
```

## Comparing `alibabacloud_eventbridge20200401-1.0.6.tar` & `alibabacloud_eventbridge20200401-1.0.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 03:45:29.000000 alibabacloud_eventbridge20200401-1.0.6/
--rw-r--r--   0 root         (0) root         (0)      304 2023-04-07 03:45:29.000000 alibabacloud_eventbridge20200401-1.0.6/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-04-07 03:45:29.000000 alibabacloud_eventbridge20200401-1.0.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-04-07 03:45:29.000000 alibabacloud_eventbridge20200401-1.0.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2376 2023-04-07 03:45:29.000000 alibabacloud_eventbridge20200401-1.0.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1046 2023-04-07 03:45:29.000000 alibabacloud_eventbridge20200401-1.0.6/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1131 2023-04-07 03:45:29.000000 alibabacloud_eventbridge20200401-1.0.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 03:45:29.000000 alibabacloud_eventbridge20200401-1.0.6/alibabacloud_eventbridge20200401/
--rw-r--r--   0 root         (0) root         (0)       21 2023-04-07 03:45:29.000000 alibabacloud_eventbridge20200401-1.0.6/alibabacloud_eventbridge20200401/__init__.py
--rw-r--r--   0 root         (0) root         (0)   145253 2023-04-07 03:45:29.000000 alibabacloud_eventbridge20200401-1.0.6/alibabacloud_eventbridge20200401/client.py
--rw-r--r--   0 root         (0) root         (0)   729553 2023-04-07 03:45:29.000000 alibabacloud_eventbridge20200401-1.0.6/alibabacloud_eventbridge20200401/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 03:45:29.000000 alibabacloud_eventbridge20200401-1.0.6/alibabacloud_eventbridge20200401.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2376 2023-04-07 03:45:29.000000 alibabacloud_eventbridge20200401-1.0.6/alibabacloud_eventbridge20200401.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      484 2023-04-07 03:45:29.000000 alibabacloud_eventbridge20200401-1.0.6/alibabacloud_eventbridge20200401.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-07 03:45:29.000000 alibabacloud_eventbridge20200401-1.0.6/alibabacloud_eventbridge20200401.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2023-04-07 03:45:29.000000 alibabacloud_eventbridge20200401-1.0.6/alibabacloud_eventbridge20200401.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       33 2023-04-07 03:45:29.000000 alibabacloud_eventbridge20200401-1.0.6/alibabacloud_eventbridge20200401.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-04-07 03:45:29.000000 alibabacloud_eventbridge20200401-1.0.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2650 2023-04-07 03:45:29.000000 alibabacloud_eventbridge20200401-1.0.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 01:46:35.000000 alibabacloud_eventbridge20200401-1.0.7/
+-rw-r--r--   0 root         (0) root         (0)      351 2023-04-13 01:46:35.000000 alibabacloud_eventbridge20200401-1.0.7/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-04-13 01:46:35.000000 alibabacloud_eventbridge20200401-1.0.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-04-13 01:46:35.000000 alibabacloud_eventbridge20200401-1.0.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2376 2023-04-13 01:46:35.000000 alibabacloud_eventbridge20200401-1.0.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1046 2023-04-13 01:46:35.000000 alibabacloud_eventbridge20200401-1.0.7/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1131 2023-04-13 01:46:35.000000 alibabacloud_eventbridge20200401-1.0.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 01:46:35.000000 alibabacloud_eventbridge20200401-1.0.7/alibabacloud_eventbridge20200401/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-04-13 01:46:35.000000 alibabacloud_eventbridge20200401-1.0.7/alibabacloud_eventbridge20200401/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   148087 2023-04-13 01:46:35.000000 alibabacloud_eventbridge20200401-1.0.7/alibabacloud_eventbridge20200401/client.py
+-rw-r--r--   0 root         (0) root         (0)   733994 2023-04-13 01:46:35.000000 alibabacloud_eventbridge20200401-1.0.7/alibabacloud_eventbridge20200401/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 01:46:35.000000 alibabacloud_eventbridge20200401-1.0.7/alibabacloud_eventbridge20200401.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2376 2023-04-13 01:46:35.000000 alibabacloud_eventbridge20200401-1.0.7/alibabacloud_eventbridge20200401.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      484 2023-04-13 01:46:35.000000 alibabacloud_eventbridge20200401-1.0.7/alibabacloud_eventbridge20200401.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 01:46:35.000000 alibabacloud_eventbridge20200401-1.0.7/alibabacloud_eventbridge20200401.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2023-04-13 01:46:35.000000 alibabacloud_eventbridge20200401-1.0.7/alibabacloud_eventbridge20200401.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       33 2023-04-13 01:46:35.000000 alibabacloud_eventbridge20200401-1.0.7/alibabacloud_eventbridge20200401.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-04-13 01:46:35.000000 alibabacloud_eventbridge20200401-1.0.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2650 2023-04-13 01:46:35.000000 alibabacloud_eventbridge20200401-1.0.7/setup.py
```

### Comparing `alibabacloud_eventbridge20200401-1.0.6/LICENSE` & `alibabacloud_eventbridge20200401-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_eventbridge20200401-1.0.6/PKG-INFO` & `alibabacloud_eventbridge20200401-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_eventbridge20200401
-Version: 1.0.6
+Version: 1.0.7
 Summary: Alibaba Cloud eventbridge (20200401) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_eventbridge20200401-1.0.6/README-CN.md` & `alibabacloud_eventbridge20200401-1.0.7/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_eventbridge20200401-1.0.6/README.md` & `alibabacloud_eventbridge20200401-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_eventbridge20200401-1.0.6/alibabacloud_eventbridge20200401/client.py` & `alibabacloud_eventbridge20200401-1.0.7/alibabacloud_eventbridge20200401/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -2837,14 +2837,88 @@
     async def start_event_streaming_async(
         self,
         request: eventbridge_20200401_models.StartEventStreamingRequest,
     ) -> eventbridge_20200401_models.StartEventStreamingResponse:
         runtime = util_models.RuntimeOptions()
         return await self.start_event_streaming_with_options_async(request, runtime)
 
+    def test_event_pattern_with_options(
+        self,
+        request: eventbridge_20200401_models.TestEventPatternRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> eventbridge_20200401_models.TestEventPatternResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.event):
+            body['Event'] = request.event
+        if not UtilClient.is_unset(request.event_pattern):
+            body['EventPattern'] = request.event_pattern
+        req = open_api_models.OpenApiRequest(
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='TestEventPattern',
+            version='2020-04-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            eventbridge_20200401_models.TestEventPatternResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def test_event_pattern_with_options_async(
+        self,
+        request: eventbridge_20200401_models.TestEventPatternRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> eventbridge_20200401_models.TestEventPatternResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.event):
+            body['Event'] = request.event
+        if not UtilClient.is_unset(request.event_pattern):
+            body['EventPattern'] = request.event_pattern
+        req = open_api_models.OpenApiRequest(
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='TestEventPattern',
+            version='2020-04-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            eventbridge_20200401_models.TestEventPatternResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def test_event_pattern(
+        self,
+        request: eventbridge_20200401_models.TestEventPatternRequest,
+    ) -> eventbridge_20200401_models.TestEventPatternResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.test_event_pattern_with_options(request, runtime)
+
+    async def test_event_pattern_async(
+        self,
+        request: eventbridge_20200401_models.TestEventPatternRequest,
+    ) -> eventbridge_20200401_models.TestEventPatternResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.test_event_pattern_with_options_async(request, runtime)
+
     def update_api_destination_with_options(
         self,
         tmp_req: eventbridge_20200401_models.UpdateApiDestinationRequest,
         runtime: util_models.RuntimeOptions,
     ) -> eventbridge_20200401_models.UpdateApiDestinationResponse:
         UtilClient.validate_model(tmp_req)
         request = eventbridge_20200401_models.UpdateApiDestinationShrinkRequest()
```

### Comparing `alibabacloud_eventbridge20200401-1.0.6/alibabacloud_eventbridge20200401/models.py` & `alibabacloud_eventbridge20200401-1.0.7/alibabacloud_eventbridge20200401/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -17844,14 +17844,171 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = StartEventStreamingResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class TestEventPatternRequest(TeaModel):
+    def __init__(
+        self,
+        event: str = None,
+        event_pattern: str = None,
+    ):
+        self.event = event
+        self.event_pattern = event_pattern
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.event is not None:
+            result['Event'] = self.event
+        if self.event_pattern is not None:
+            result['EventPattern'] = self.event_pattern
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Event') is not None:
+            self.event = m.get('Event')
+        if m.get('EventPattern') is not None:
+            self.event_pattern = m.get('EventPattern')
+        return self
+
+
+class TestEventPatternResponseBodyData(TeaModel):
+    def __init__(
+        self,
+        result: bool = None,
+    ):
+        self.result = result
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.result is not None:
+            result['Result'] = self.result
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Result') is not None:
+            self.result = m.get('Result')
+        return self
+
+
+class TestEventPatternResponseBody(TeaModel):
+    def __init__(
+        self,
+        code: str = None,
+        data: TestEventPatternResponseBodyData = None,
+        message: str = None,
+        request_id: str = None,
+        success: bool = None,
+    ):
+        self.code = code
+        self.data = data
+        self.message = message
+        self.request_id = request_id
+        self.success = success
+
+    def validate(self):
+        if self.data:
+            self.data.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.data is not None:
+            result['Data'] = self.data.to_map()
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.success is not None:
+            result['Success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Data') is not None:
+            temp_model = TestEventPatternResponseBodyData()
+            self.data = temp_model.from_map(m['Data'])
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
+        return self
+
+
+class TestEventPatternResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: TestEventPatternResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = TestEventPatternResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class UpdateApiDestinationRequestHttpApiParameters(TeaModel):
     def __init__(
         self,
         endpoint: str = None,
         method: str = None,
     ):
         self.endpoint = endpoint
```

### Comparing `alibabacloud_eventbridge20200401-1.0.6/alibabacloud_eventbridge20200401.egg-info/PKG-INFO` & `alibabacloud_eventbridge20200401-1.0.7/alibabacloud_eventbridge20200401.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-eventbridge20200401
-Version: 1.0.6
+Version: 1.0.7
 Summary: Alibaba Cloud eventbridge (20200401) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_eventbridge20200401-1.0.6/setup.py` & `alibabacloud_eventbridge20200401-1.0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_eventbridge20200401.
 
-Created on 07/04/2023
+Created on 13/04/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_eventbridge20200401"
 NAME = "alibabacloud_eventbridge20200401" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud eventbridge (20200401) SDK Library for Python"
```

