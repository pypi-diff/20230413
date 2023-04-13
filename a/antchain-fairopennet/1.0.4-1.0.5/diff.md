# Comparing `tmp/antchain_fairopennet-1.0.4.tar.gz` & `tmp/antchain_fairopennet-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/antchain_fairopennet-1.0.4.tar", last modified: Tue Apr 11 12:02:00 2023, max compression
+gzip compressed data, was "dist/antchain_fairopennet-1.0.5.tar", last modified: Thu Apr 13 02:34:51 2023, max compression
```

## Comparing `antchain_fairopennet-1.0.4.tar` & `antchain_fairopennet-1.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:02:00.000000 antchain_fairopennet-1.0.4/
--rw-r--r--   0 root         (0) root         (0)      600 2023-04-11 12:02:00.000000 antchain_fairopennet-1.0.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-04-11 12:02:00.000000 antchain_fairopennet-1.0.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2210 2023-04-11 12:02:00.000000 antchain_fairopennet-1.0.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      828 2023-04-11 12:02:00.000000 antchain_fairopennet-1.0.4/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1014 2023-04-11 12:02:00.000000 antchain_fairopennet-1.0.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:02:00.000000 antchain_fairopennet-1.0.4/antchain_fairopennet.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2210 2023-04-11 12:02:00.000000 antchain_fairopennet-1.0.4/antchain_fairopennet.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      387 2023-04-11 12:02:00.000000 antchain_fairopennet-1.0.4/antchain_fairopennet.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 12:02:00.000000 antchain_fairopennet-1.0.4/antchain_fairopennet.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2023-04-11 12:02:00.000000 antchain_fairopennet-1.0.4/antchain_fairopennet.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2023-04-11 12:02:00.000000 antchain_fairopennet-1.0.4/antchain_fairopennet.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:02:00.000000 antchain_fairopennet-1.0.4/antchain_sdk_fairopennet/
--rw-r--r--   0 root         (0) root         (0)       21 2023-04-11 12:02:00.000000 antchain_fairopennet-1.0.4/antchain_sdk_fairopennet/__init__.py
--rw-r--r--   0 root         (0) root         (0)    80220 2023-04-11 12:02:00.000000 antchain_fairopennet-1.0.4/antchain_sdk_fairopennet/client.py
--rw-r--r--   0 root         (0) root         (0)   124064 2023-04-11 12:02:00.000000 antchain_fairopennet-1.0.4/antchain_sdk_fairopennet/models.py
--rw-r--r--   0 root         (0) root         (0)       73 2023-04-11 12:02:00.000000 antchain_fairopennet-1.0.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2528 2023-04-11 12:02:00.000000 antchain_fairopennet-1.0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 02:34:51.000000 antchain_fairopennet-1.0.5/
+-rw-r--r--   0 root         (0) root         (0)      600 2023-04-13 02:34:50.000000 antchain_fairopennet-1.0.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-04-13 02:34:50.000000 antchain_fairopennet-1.0.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2210 2023-04-13 02:34:51.000000 antchain_fairopennet-1.0.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      828 2023-04-13 02:34:50.000000 antchain_fairopennet-1.0.5/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1014 2023-04-13 02:34:50.000000 antchain_fairopennet-1.0.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 02:34:51.000000 antchain_fairopennet-1.0.5/antchain_fairopennet.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2210 2023-04-13 02:34:51.000000 antchain_fairopennet-1.0.5/antchain_fairopennet.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      387 2023-04-13 02:34:51.000000 antchain_fairopennet-1.0.5/antchain_fairopennet.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 02:34:51.000000 antchain_fairopennet-1.0.5/antchain_fairopennet.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2023-04-13 02:34:51.000000 antchain_fairopennet-1.0.5/antchain_fairopennet.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2023-04-13 02:34:51.000000 antchain_fairopennet-1.0.5/antchain_fairopennet.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 02:34:51.000000 antchain_fairopennet-1.0.5/antchain_sdk_fairopennet/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-04-13 02:34:50.000000 antchain_fairopennet-1.0.5/antchain_sdk_fairopennet/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    80300 2023-04-13 02:34:50.000000 antchain_fairopennet-1.0.5/antchain_sdk_fairopennet/client.py
+-rw-r--r--   0 root         (0) root         (0)   124229 2023-04-13 02:34:50.000000 antchain_fairopennet-1.0.5/antchain_sdk_fairopennet/models.py
+-rw-r--r--   0 root         (0) root         (0)       73 2023-04-13 02:34:51.000000 antchain_fairopennet-1.0.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2528 2023-04-13 02:34:50.000000 antchain_fairopennet-1.0.5/setup.py
```

### Comparing `antchain_fairopennet-1.0.4/LICENSE` & `antchain_fairopennet-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `antchain_fairopennet-1.0.4/PKG-INFO` & `antchain_fairopennet-1.0.5/antchain_fairopennet.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: antchain_fairopennet
-Version: 1.0.4
+Name: antchain-fairopennet
+Version: 1.0.5
 Summary: Ant Chain FAIROPENNET SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_fairopennet-1.0.4/README-CN.md` & `antchain_fairopennet-1.0.5/README-CN.md`

 * *Files identical despite different names*

### Comparing `antchain_fairopennet-1.0.4/README.md` & `antchain_fairopennet-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `antchain_fairopennet-1.0.4/antchain_fairopennet.egg-info/PKG-INFO` & `antchain_fairopennet-1.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: antchain-fairopennet
-Version: 1.0.4
+Name: antchain_fairopennet
+Version: 1.0.5
 Summary: Ant Chain FAIROPENNET SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_fairopennet-1.0.4/antchain_sdk_fairopennet/client.py` & `antchain_fairopennet-1.0.5/antchain_sdk_fairopennet/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,15 +131,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.0.4',
+                    'sdk_version': '1.0.5',
                     '_prod_code': 'FAIROPENNET',
                     '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
@@ -235,15 +235,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.0.4',
+                    'sdk_version': '1.0.5',
                     '_prod_code': 'FAIROPENNET',
                     '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
@@ -1284,41 +1284,41 @@
         )
 
     def create_flow(
         self,
         request: fairopennet_models.CreateFlowRequest,
     ) -> fairopennet_models.CreateFlowResponse:
         """
-        Description: 创建一个工作流
+        Description: 创建一个工作流，传入partyId，和静态flow配置
         Summary: 创建一个工作流
         """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.create_flow_ex(request, headers, runtime)
 
     async def create_flow_async(
         self,
         request: fairopennet_models.CreateFlowRequest,
     ) -> fairopennet_models.CreateFlowResponse:
         """
-        Description: 创建一个工作流
+        Description: 创建一个工作流，传入partyId，和静态flow配置
         Summary: 创建一个工作流
         """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.create_flow_ex_async(request, headers, runtime)
 
     def create_flow_ex(
         self,
         request: fairopennet_models.CreateFlowRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> fairopennet_models.CreateFlowResponse:
         """
-        Description: 创建一个工作流
+        Description: 创建一个工作流，传入partyId，和静态flow配置
         Summary: 创建一个工作流
         """
         UtilClient.validate_model(request)
         return TeaCore.from_map(
             fairopennet_models.CreateFlowResponse(),
             self.do_request('1.0', 'antchain.fairopennet.flow.create', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
@@ -1326,15 +1326,15 @@
     async def create_flow_ex_async(
         self,
         request: fairopennet_models.CreateFlowRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> fairopennet_models.CreateFlowResponse:
         """
-        Description: 创建一个工作流
+        Description: 创建一个工作流，传入partyId，和静态flow配置
         Summary: 创建一个工作流
         """
         UtilClient.validate_model(request)
         return TeaCore.from_map(
             fairopennet_models.CreateFlowResponse(),
             await self.do_request_async('1.0', 'antchain.fairopennet.flow.create', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
@@ -1447,68 +1447,68 @@
         """
         UtilClient.validate_model(request)
         return TeaCore.from_map(
             fairopennet_models.StopFlowinstanceResponse(),
             await self.do_request_async('1.0', 'antchain.fairopennet.flowinstance.stop', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
-    def query_flowinstance_status(
+    def query_instance_status(
         self,
-        request: fairopennet_models.QueryFlowinstanceStatusRequest,
-    ) -> fairopennet_models.QueryFlowinstanceStatusResponse:
+        request: fairopennet_models.QueryInstanceStatusRequest,
+    ) -> fairopennet_models.QueryInstanceStatusResponse:
         """
         Description: 查询工作流实例状态
         Summary: 查询工作流实例状态
         """
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.query_flowinstance_status_ex(request, headers, runtime)
+        return self.query_instance_status_ex(request, headers, runtime)
 
-    async def query_flowinstance_status_async(
+    async def query_instance_status_async(
         self,
-        request: fairopennet_models.QueryFlowinstanceStatusRequest,
-    ) -> fairopennet_models.QueryFlowinstanceStatusResponse:
+        request: fairopennet_models.QueryInstanceStatusRequest,
+    ) -> fairopennet_models.QueryInstanceStatusResponse:
         """
         Description: 查询工作流实例状态
         Summary: 查询工作流实例状态
         """
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.query_flowinstance_status_ex_async(request, headers, runtime)
+        return await self.query_instance_status_ex_async(request, headers, runtime)
 
-    def query_flowinstance_status_ex(
+    def query_instance_status_ex(
         self,
-        request: fairopennet_models.QueryFlowinstanceStatusRequest,
+        request: fairopennet_models.QueryInstanceStatusRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
-    ) -> fairopennet_models.QueryFlowinstanceStatusResponse:
+    ) -> fairopennet_models.QueryInstanceStatusResponse:
         """
         Description: 查询工作流实例状态
         Summary: 查询工作流实例状态
         """
         UtilClient.validate_model(request)
         return TeaCore.from_map(
-            fairopennet_models.QueryFlowinstanceStatusResponse(),
-            self.do_request('1.0', 'antchain.fairopennet.flowinstance.status.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+            fairopennet_models.QueryInstanceStatusResponse(),
+            self.do_request('1.0', 'antchain.fairopennet.instance.status.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
-    async def query_flowinstance_status_ex_async(
+    async def query_instance_status_ex_async(
         self,
-        request: fairopennet_models.QueryFlowinstanceStatusRequest,
+        request: fairopennet_models.QueryInstanceStatusRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
-    ) -> fairopennet_models.QueryFlowinstanceStatusResponse:
+    ) -> fairopennet_models.QueryInstanceStatusResponse:
         """
         Description: 查询工作流实例状态
         Summary: 查询工作流实例状态
         """
         UtilClient.validate_model(request)
         return TeaCore.from_map(
-            fairopennet_models.QueryFlowinstanceStatusResponse(),
-            await self.do_request_async('1.0', 'antchain.fairopennet.flowinstance.status.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+            fairopennet_models.QueryInstanceStatusResponse(),
+            await self.do_request_async('1.0', 'antchain.fairopennet.instance.status.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def upload_file(
         self,
         request: fairopennet_models.UploadFileRequest,
     ) -> fairopennet_models.UploadFileResponse:
         """
```

### Comparing `antchain_fairopennet-1.0.4/antchain_sdk_fairopennet/models.py` & `antchain_fairopennet-1.0.5/antchain_sdk_fairopennet/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -830,15 +830,15 @@
         auto_start: bool = None,
         static_parameters: str = None,
         dynamic_parameters: str = None,
         total_components: int = None,
         completed_components: int = None,
         error_code: str = None,
         error_message: str = None,
-        status: int = None,
+        status: str = None,
     ):
         # 
         self.space_id = space_id
         # 
         self.flow_id = flow_id
         # 
         self.instance_id = instance_id
@@ -850,19 +850,19 @@
         self.static_parameters = static_parameters
         # 
         self.dynamic_parameters = dynamic_parameters
         # 
         self.total_components = total_components
         # 
         self.completed_components = completed_components
-        # 
+        # fair错误码
         self.error_code = error_code
-        # 
+        # Fair错误信息
         self.error_message = error_message
-        # 
+        # 工作流实力执行的状态码
         self.status = status
 
     def validate(self):
         self.validate_required(self.space_id, 'space_id')
         self.validate_required(self.flow_id, 'flow_id')
         self.validate_required(self.instance_id, 'instance_id')
         self.validate_required(self.consent_on, 'consent_on')
@@ -2786,57 +2786,54 @@
 
 class CreateFlowRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         product_instance_id: str = None,
         party_id: str = None,
-        config: StaticFlowConfig = None,
+        static_flow_config: str = None,
     ):
         # OAuth模式下的授权token
         self.auth_token = auth_token
         self.product_instance_id = product_instance_id
-        # 
+        # 参与方的partyId
         self.party_id = party_id
-        # 
-        self.config = config
+        # 静态工作流配置字符串
+        self.static_flow_config = static_flow_config
 
     def validate(self):
         self.validate_required(self.party_id, 'party_id')
-        self.validate_required(self.config, 'config')
-        if self.config:
-            self.config.validate()
+        self.validate_required(self.static_flow_config, 'static_flow_config')
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.product_instance_id is not None:
             result['product_instance_id'] = self.product_instance_id
         if self.party_id is not None:
             result['party_id'] = self.party_id
-        if self.config is not None:
-            result['config'] = self.config.to_map()
+        if self.static_flow_config is not None:
+            result['static_flow_config'] = self.static_flow_config
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('auth_token') is not None:
             self.auth_token = m.get('auth_token')
         if m.get('product_instance_id') is not None:
             self.product_instance_id = m.get('product_instance_id')
         if m.get('party_id') is not None:
             self.party_id = m.get('party_id')
-        if m.get('config') is not None:
-            temp_model = StaticFlowConfig()
-            self.config = temp_model.from_map(m['config'])
+        if m.get('static_flow_config') is not None:
+            self.static_flow_config = m.get('static_flow_config')
         return self
 
 
 class CreateFlowResponse(TeaModel):
     def __init__(
         self,
         req_msg_id: str = None,
@@ -2880,57 +2877,54 @@
 
 class RunFlowInstanceRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         product_instance_id: str = None,
         party_id: str = None,
-        config: DynamicFlowConfig = None,
+        dynamic_flow_config: str = None,
     ):
         # OAuth模式下的授权token
         self.auth_token = auth_token
         self.product_instance_id = product_instance_id
-        # 
+        # 参与方的partyId
         self.party_id = party_id
-        # 
-        self.config = config
+        # 动态工作流配置字符串
+        self.dynamic_flow_config = dynamic_flow_config
 
     def validate(self):
         self.validate_required(self.party_id, 'party_id')
-        self.validate_required(self.config, 'config')
-        if self.config:
-            self.config.validate()
+        self.validate_required(self.dynamic_flow_config, 'dynamic_flow_config')
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.product_instance_id is not None:
             result['product_instance_id'] = self.product_instance_id
         if self.party_id is not None:
             result['party_id'] = self.party_id
-        if self.config is not None:
-            result['config'] = self.config.to_map()
+        if self.dynamic_flow_config is not None:
+            result['dynamic_flow_config'] = self.dynamic_flow_config
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('auth_token') is not None:
             self.auth_token = m.get('auth_token')
         if m.get('product_instance_id') is not None:
             self.product_instance_id = m.get('product_instance_id')
         if m.get('party_id') is not None:
             self.party_id = m.get('party_id')
-        if m.get('config') is not None:
-            temp_model = DynamicFlowConfig()
-            self.config = temp_model.from_map(m['config'])
+        if m.get('dynamic_flow_config') is not None:
+            self.dynamic_flow_config = m.get('dynamic_flow_config')
         return self
 
 
 class RunFlowInstanceResponse(TeaModel):
     def __init__(
         self,
         req_msg_id: str = None,
@@ -3083,66 +3077,64 @@
         if m.get('result_code') is not None:
             self.result_code = m.get('result_code')
         if m.get('result_msg') is not None:
             self.result_msg = m.get('result_msg')
         return self
 
 
-class QueryFlowinstanceStatusRequest(TeaModel):
+class QueryInstanceStatusRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         product_instance_id: str = None,
-        config: FlowInstanceLocator = None,
-        extra: str = None,
+        flow_id: str = None,
+        instance_id: str = None,
     ):
         # OAuth模式下的授权token
         self.auth_token = auth_token
         self.product_instance_id = product_instance_id
-        # 
-        self.config = config
-        # 
-        self.extra = extra
+        # 工作流的flowId
+        self.flow_id = flow_id
+        # 工作流实例instanceId
+        self.instance_id = instance_id
 
     def validate(self):
-        self.validate_required(self.config, 'config')
-        if self.config:
-            self.config.validate()
+        self.validate_required(self.flow_id, 'flow_id')
+        self.validate_required(self.instance_id, 'instance_id')
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.product_instance_id is not None:
             result['product_instance_id'] = self.product_instance_id
-        if self.config is not None:
-            result['config'] = self.config.to_map()
-        if self.extra is not None:
-            result['extra'] = self.extra
+        if self.flow_id is not None:
+            result['flow_id'] = self.flow_id
+        if self.instance_id is not None:
+            result['instance_id'] = self.instance_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('auth_token') is not None:
             self.auth_token = m.get('auth_token')
         if m.get('product_instance_id') is not None:
             self.product_instance_id = m.get('product_instance_id')
-        if m.get('config') is not None:
-            temp_model = FlowInstanceLocator()
-            self.config = temp_model.from_map(m['config'])
-        if m.get('extra') is not None:
-            self.extra = m.get('extra')
+        if m.get('flow_id') is not None:
+            self.flow_id = m.get('flow_id')
+        if m.get('instance_id') is not None:
+            self.instance_id = m.get('instance_id')
         return self
 
 
-class QueryFlowinstanceStatusResponse(TeaModel):
+class QueryInstanceStatusResponse(TeaModel):
     def __init__(
         self,
         req_msg_id: str = None,
         result_code: str = None,
         result_msg: str = None,
         status: FlowInstanceStatus = None,
     ):
```

### Comparing `antchain_fairopennet-1.0.4/setup.py` & `antchain_fairopennet-1.0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for antchain_fairopennet.
 
-Created on 11/04/2023
+Created on 13/04/2023
 
 @author: Ant Chain SDK
 """
 
 PACKAGE = "antchain_sdk_fairopennet"
 NAME = "antchain_fairopennet" or "alibabacloud-package"
 DESCRIPTION = "Ant Chain FAIROPENNET SDK Library for Python"
```

