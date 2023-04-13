# Comparing `tmp/alibabacloud_eflo20220530-1.0.2.tar.gz` & `tmp/alibabacloud_eflo20220530-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_eflo20220530-1.0.2.tar", last modified: Thu Mar 30 10:00:00 2023, max compression
+gzip compressed data, was "dist/alibabacloud_eflo20220530-1.0.3.tar", last modified: Thu Apr 13 08:26:39 2023, max compression
```

## Comparing `alibabacloud_eflo20220530-1.0.2.tar` & `alibabacloud_eflo20220530-1.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 10:00:00.000000 alibabacloud_eflo20220530-1.0.2/
--rw-r--r--   0 root         (0) root         (0)       88 2023-03-30 10:00:00.000000 alibabacloud_eflo20220530-1.0.2/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-03-30 10:00:00.000000 alibabacloud_eflo20220530-1.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-03-30 10:00:00.000000 alibabacloud_eflo20220530-1.0.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2334 2023-03-30 10:00:00.000000 alibabacloud_eflo20220530-1.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1025 2023-03-30 10:00:00.000000 alibabacloud_eflo20220530-1.0.2/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1110 2023-03-30 10:00:00.000000 alibabacloud_eflo20220530-1.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 10:00:00.000000 alibabacloud_eflo20220530-1.0.2/alibabacloud_eflo20220530/
--rw-r--r--   0 root         (0) root         (0)       21 2023-03-30 10:00:00.000000 alibabacloud_eflo20220530-1.0.2/alibabacloud_eflo20220530/__init__.py
--rw-r--r--   0 root         (0) root         (0)    93938 2023-03-30 10:00:00.000000 alibabacloud_eflo20220530-1.0.2/alibabacloud_eflo20220530/client.py
--rw-r--r--   0 root         (0) root         (0)   232284 2023-03-30 10:00:00.000000 alibabacloud_eflo20220530-1.0.2/alibabacloud_eflo20220530/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 10:00:00.000000 alibabacloud_eflo20220530-1.0.2/alibabacloud_eflo20220530.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2334 2023-03-30 10:00:00.000000 alibabacloud_eflo20220530-1.0.2/alibabacloud_eflo20220530.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      428 2023-03-30 10:00:00.000000 alibabacloud_eflo20220530-1.0.2/alibabacloud_eflo20220530.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-30 10:00:00.000000 alibabacloud_eflo20220530-1.0.2/alibabacloud_eflo20220530.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2023-03-30 10:00:00.000000 alibabacloud_eflo20220530-1.0.2/alibabacloud_eflo20220530.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       26 2023-03-30 10:00:00.000000 alibabacloud_eflo20220530-1.0.2/alibabacloud_eflo20220530.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-03-30 10:00:00.000000 alibabacloud_eflo20220530-1.0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2615 2023-03-30 10:00:00.000000 alibabacloud_eflo20220530-1.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 08:26:39.000000 alibabacloud_eflo20220530-1.0.3/
+-rw-r--r--   0 root         (0) root         (0)      184 2023-04-13 08:26:39.000000 alibabacloud_eflo20220530-1.0.3/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-04-13 08:26:39.000000 alibabacloud_eflo20220530-1.0.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-04-13 08:26:39.000000 alibabacloud_eflo20220530-1.0.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2334 2023-04-13 08:26:39.000000 alibabacloud_eflo20220530-1.0.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1025 2023-04-13 08:26:39.000000 alibabacloud_eflo20220530-1.0.3/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1110 2023-04-13 08:26:39.000000 alibabacloud_eflo20220530-1.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 08:26:39.000000 alibabacloud_eflo20220530-1.0.3/alibabacloud_eflo20220530/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-04-13 08:26:39.000000 alibabacloud_eflo20220530-1.0.3/alibabacloud_eflo20220530/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   192902 2023-04-13 08:26:39.000000 alibabacloud_eflo20220530-1.0.3/alibabacloud_eflo20220530/client.py
+-rw-r--r--   0 root         (0) root         (0)   449281 2023-04-13 08:26:39.000000 alibabacloud_eflo20220530-1.0.3/alibabacloud_eflo20220530/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 08:26:39.000000 alibabacloud_eflo20220530-1.0.3/alibabacloud_eflo20220530.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2334 2023-04-13 08:26:39.000000 alibabacloud_eflo20220530-1.0.3/alibabacloud_eflo20220530.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      428 2023-04-13 08:26:39.000000 alibabacloud_eflo20220530-1.0.3/alibabacloud_eflo20220530.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 08:26:39.000000 alibabacloud_eflo20220530-1.0.3/alibabacloud_eflo20220530.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2023-04-13 08:26:39.000000 alibabacloud_eflo20220530-1.0.3/alibabacloud_eflo20220530.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2023-04-13 08:26:39.000000 alibabacloud_eflo20220530-1.0.3/alibabacloud_eflo20220530.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-04-13 08:26:39.000000 alibabacloud_eflo20220530-1.0.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2615 2023-04-13 08:26:39.000000 alibabacloud_eflo20220530-1.0.3/setup.py
```

### Comparing `alibabacloud_eflo20220530-1.0.2/LICENSE` & `alibabacloud_eflo20220530-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_eflo20220530-1.0.2/PKG-INFO` & `alibabacloud_eflo20220530-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_eflo20220530
-Version: 1.0.2
+Version: 1.0.3
 Summary: Alibaba Cloud eflo (20220530) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_eflo20220530-1.0.2/README-CN.md` & `alibabacloud_eflo20220530-1.0.3/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_eflo20220530-1.0.2/README.md` & `alibabacloud_eflo20220530-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_eflo20220530-1.0.2/alibabacloud_eflo20220530/models.py` & `alibabacloud_eflo20220530-1.0.3/alibabacloud_eflo20220530/models.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,62 +4,62 @@
 from typing import Dict, List, Any
 
 
 class AssignPrivateIpAddressRequest(TeaModel):
     def __init__(
         self,
         assign_mac: bool = None,
-        client_token: str = None,
         network_interface_id: str = None,
         private_ip_address: str = None,
         region_id: str = None,
+        skip_config: bool = None,
         subnet_id: str = None,
     ):
         self.assign_mac = assign_mac
-        self.client_token = client_token
         self.network_interface_id = network_interface_id
         self.private_ip_address = private_ip_address
         self.region_id = region_id
+        self.skip_config = skip_config
         self.subnet_id = subnet_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.assign_mac is not None:
             result['AssignMac'] = self.assign_mac
-        if self.client_token is not None:
-            result['ClientToken'] = self.client_token
         if self.network_interface_id is not None:
             result['NetworkInterfaceId'] = self.network_interface_id
         if self.private_ip_address is not None:
             result['PrivateIpAddress'] = self.private_ip_address
         if self.region_id is not None:
             result['RegionId'] = self.region_id
+        if self.skip_config is not None:
+            result['SkipConfig'] = self.skip_config
         if self.subnet_id is not None:
             result['SubnetId'] = self.subnet_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('AssignMac') is not None:
             self.assign_mac = m.get('AssignMac')
-        if m.get('ClientToken') is not None:
-            self.client_token = m.get('ClientToken')
         if m.get('NetworkInterfaceId') is not None:
             self.network_interface_id = m.get('NetworkInterfaceId')
         if m.get('PrivateIpAddress') is not None:
             self.private_ip_address = m.get('PrivateIpAddress')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
+        if m.get('SkipConfig') is not None:
+            self.skip_config = m.get('SkipConfig')
         if m.get('SubnetId') is not None:
             self.subnet_id = m.get('SubnetId')
         return self
 
 
 class AssignPrivateIpAddressResponseBodyContent(TeaModel):
     def __init__(
@@ -181,14 +181,569 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = AssignPrivateIpAddressResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class CreateErRequest(TeaModel):
+    def __init__(
+        self,
+        description: str = None,
+        er_name: str = None,
+        master_zone_id: str = None,
+        region_id: str = None,
+    ):
+        self.description = description
+        self.er_name = er_name
+        self.master_zone_id = master_zone_id
+        self.region_id = region_id
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
+        if self.description is not None:
+            result['Description'] = self.description
+        if self.er_name is not None:
+            result['ErName'] = self.er_name
+        if self.master_zone_id is not None:
+            result['MasterZoneId'] = self.master_zone_id
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Description') is not None:
+            self.description = m.get('Description')
+        if m.get('ErName') is not None:
+            self.er_name = m.get('ErName')
+        if m.get('MasterZoneId') is not None:
+            self.master_zone_id = m.get('MasterZoneId')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        return self
+
+
+class CreateErResponseBodyContent(TeaModel):
+    def __init__(
+        self,
+        er_id: str = None,
+    ):
+        self.er_id = er_id
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
+        if self.er_id is not None:
+            result['ErId'] = self.er_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ErId') is not None:
+            self.er_id = m.get('ErId')
+        return self
+
+
+class CreateErResponseBody(TeaModel):
+    def __init__(
+        self,
+        code: int = None,
+        content: CreateErResponseBodyContent = None,
+        message: str = None,
+        request_id: str = None,
+    ):
+        self.code = code
+        self.content = content
+        self.message = message
+        self.request_id = request_id
+
+    def validate(self):
+        if self.content:
+            self.content.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.content is not None:
+            result['Content'] = self.content.to_map()
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Content') is not None:
+            temp_model = CreateErResponseBodyContent()
+            self.content = temp_model.from_map(m['Content'])
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class CreateErResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: CreateErResponseBody = None,
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
+            temp_model = CreateErResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class CreateErAttachmentRequest(TeaModel):
+    def __init__(
+        self,
+        auto_receive_all_route: bool = None,
+        er_attachment_name: str = None,
+        er_id: str = None,
+        instance_id: str = None,
+        instance_type: str = None,
+        region_id: str = None,
+        resource_tenant_id: str = None,
+    ):
+        self.auto_receive_all_route = auto_receive_all_route
+        self.er_attachment_name = er_attachment_name
+        self.er_id = er_id
+        self.instance_id = instance_id
+        self.instance_type = instance_type
+        self.region_id = region_id
+        self.resource_tenant_id = resource_tenant_id
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
+        if self.auto_receive_all_route is not None:
+            result['AutoReceiveAllRoute'] = self.auto_receive_all_route
+        if self.er_attachment_name is not None:
+            result['ErAttachmentName'] = self.er_attachment_name
+        if self.er_id is not None:
+            result['ErId'] = self.er_id
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.instance_type is not None:
+            result['InstanceType'] = self.instance_type
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.resource_tenant_id is not None:
+            result['ResourceTenantId'] = self.resource_tenant_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('AutoReceiveAllRoute') is not None:
+            self.auto_receive_all_route = m.get('AutoReceiveAllRoute')
+        if m.get('ErAttachmentName') is not None:
+            self.er_attachment_name = m.get('ErAttachmentName')
+        if m.get('ErId') is not None:
+            self.er_id = m.get('ErId')
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('InstanceType') is not None:
+            self.instance_type = m.get('InstanceType')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('ResourceTenantId') is not None:
+            self.resource_tenant_id = m.get('ResourceTenantId')
+        return self
+
+
+class CreateErAttachmentResponseBodyContent(TeaModel):
+    def __init__(
+        self,
+        er_attachment_id: str = None,
+    ):
+        self.er_attachment_id = er_attachment_id
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
+        if self.er_attachment_id is not None:
+            result['ErAttachmentId'] = self.er_attachment_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ErAttachmentId') is not None:
+            self.er_attachment_id = m.get('ErAttachmentId')
+        return self
+
+
+class CreateErAttachmentResponseBody(TeaModel):
+    def __init__(
+        self,
+        code: int = None,
+        content: CreateErAttachmentResponseBodyContent = None,
+        message: str = None,
+        request_id: str = None,
+    ):
+        self.code = code
+        self.content = content
+        self.message = message
+        self.request_id = request_id
+
+    def validate(self):
+        if self.content:
+            self.content.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.content is not None:
+            result['Content'] = self.content.to_map()
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Content') is not None:
+            temp_model = CreateErAttachmentResponseBodyContent()
+            self.content = temp_model.from_map(m['Content'])
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class CreateErAttachmentResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: CreateErAttachmentResponseBody = None,
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
+            temp_model = CreateErAttachmentResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class CreateErRouteMapRequest(TeaModel):
+    def __init__(
+        self,
+        description: str = None,
+        destination_cidr_block: str = None,
+        er_id: str = None,
+        reception_instance_id: str = None,
+        reception_instance_owner: str = None,
+        reception_instance_type: str = None,
+        region_id: str = None,
+        route_map_action: str = None,
+        route_map_num: int = None,
+        transmission_instance_id: str = None,
+        transmission_instance_owner: str = None,
+        transmission_instance_type: str = None,
+    ):
+        self.description = description
+        self.destination_cidr_block = destination_cidr_block
+        self.er_id = er_id
+        self.reception_instance_id = reception_instance_id
+        self.reception_instance_owner = reception_instance_owner
+        self.reception_instance_type = reception_instance_type
+        self.region_id = region_id
+        self.route_map_action = route_map_action
+        self.route_map_num = route_map_num
+        self.transmission_instance_id = transmission_instance_id
+        self.transmission_instance_owner = transmission_instance_owner
+        self.transmission_instance_type = transmission_instance_type
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
+        if self.description is not None:
+            result['Description'] = self.description
+        if self.destination_cidr_block is not None:
+            result['DestinationCidrBlock'] = self.destination_cidr_block
+        if self.er_id is not None:
+            result['ErId'] = self.er_id
+        if self.reception_instance_id is not None:
+            result['ReceptionInstanceId'] = self.reception_instance_id
+        if self.reception_instance_owner is not None:
+            result['ReceptionInstanceOwner'] = self.reception_instance_owner
+        if self.reception_instance_type is not None:
+            result['ReceptionInstanceType'] = self.reception_instance_type
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.route_map_action is not None:
+            result['RouteMapAction'] = self.route_map_action
+        if self.route_map_num is not None:
+            result['RouteMapNum'] = self.route_map_num
+        if self.transmission_instance_id is not None:
+            result['TransmissionInstanceId'] = self.transmission_instance_id
+        if self.transmission_instance_owner is not None:
+            result['TransmissionInstanceOwner'] = self.transmission_instance_owner
+        if self.transmission_instance_type is not None:
+            result['TransmissionInstanceType'] = self.transmission_instance_type
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Description') is not None:
+            self.description = m.get('Description')
+        if m.get('DestinationCidrBlock') is not None:
+            self.destination_cidr_block = m.get('DestinationCidrBlock')
+        if m.get('ErId') is not None:
+            self.er_id = m.get('ErId')
+        if m.get('ReceptionInstanceId') is not None:
+            self.reception_instance_id = m.get('ReceptionInstanceId')
+        if m.get('ReceptionInstanceOwner') is not None:
+            self.reception_instance_owner = m.get('ReceptionInstanceOwner')
+        if m.get('ReceptionInstanceType') is not None:
+            self.reception_instance_type = m.get('ReceptionInstanceType')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('RouteMapAction') is not None:
+            self.route_map_action = m.get('RouteMapAction')
+        if m.get('RouteMapNum') is not None:
+            self.route_map_num = m.get('RouteMapNum')
+        if m.get('TransmissionInstanceId') is not None:
+            self.transmission_instance_id = m.get('TransmissionInstanceId')
+        if m.get('TransmissionInstanceOwner') is not None:
+            self.transmission_instance_owner = m.get('TransmissionInstanceOwner')
+        if m.get('TransmissionInstanceType') is not None:
+            self.transmission_instance_type = m.get('TransmissionInstanceType')
+        return self
+
+
+class CreateErRouteMapResponseBodyContent(TeaModel):
+    def __init__(
+        self,
+        er_route_map_id: str = None,
+    ):
+        self.er_route_map_id = er_route_map_id
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
+        if self.er_route_map_id is not None:
+            result['ErRouteMapId'] = self.er_route_map_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ErRouteMapId') is not None:
+            self.er_route_map_id = m.get('ErRouteMapId')
+        return self
+
+
+class CreateErRouteMapResponseBody(TeaModel):
+    def __init__(
+        self,
+        code: int = None,
+        content: CreateErRouteMapResponseBodyContent = None,
+        message: str = None,
+        request_id: str = None,
+    ):
+        self.code = code
+        self.content = content
+        self.message = message
+        self.request_id = request_id
+
+    def validate(self):
+        if self.content:
+            self.content.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.content is not None:
+            result['Content'] = self.content.to_map()
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Content') is not None:
+            temp_model = CreateErRouteMapResponseBodyContent()
+            self.content = temp_model.from_map(m['Content'])
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class CreateErRouteMapResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: CreateErRouteMapResponseBody = None,
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
+            temp_model = CreateErRouteMapResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class CreateSubnetRequestTag(TeaModel):
     def __init__(
         self,
         key: str = None,
         value: str = None,
     ):
         self.key = key
@@ -218,24 +773,22 @@
         return self
 
 
 class CreateSubnetRequest(TeaModel):
     def __init__(
         self,
         cidr: str = None,
-        client_token: str = None,
         region_id: str = None,
         subnet_name: str = None,
         tag: List[CreateSubnetRequestTag] = None,
         type: str = None,
         vpd_id: str = None,
         zone_id: str = None,
     ):
         self.cidr = cidr
-        self.client_token = client_token
         self.region_id = region_id
         self.subnet_name = subnet_name
         self.tag = tag
         self.type = type
         self.vpd_id = vpd_id
         self.zone_id = zone_id
 
@@ -249,16 +802,14 @@
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.cidr is not None:
             result['Cidr'] = self.cidr
-        if self.client_token is not None:
-            result['ClientToken'] = self.client_token
         if self.region_id is not None:
             result['RegionId'] = self.region_id
         if self.subnet_name is not None:
             result['SubnetName'] = self.subnet_name
         result['Tag'] = []
         if self.tag is not None:
             for k in self.tag:
@@ -271,16 +822,14 @@
             result['ZoneId'] = self.zone_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('Cidr') is not None:
             self.cidr = m.get('Cidr')
-        if m.get('ClientToken') is not None:
-            self.client_token = m.get('ClientToken')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
         if m.get('SubnetName') is not None:
             self.subnet_name = m.get('SubnetName')
         self.tag = []
         if m.get('Tag') is not None:
             for k in m.get('Tag'):
@@ -446,14 +995,15 @@
         return self
 
 
 class CreateVccRequest(TeaModel):
     def __init__(
         self,
         access_could_service: bool = None,
+        bandwidth: int = None,
         bgp_cidr: str = None,
         cen_id: str = None,
         connection_type: str = None,
         description: str = None,
         region_id: str = None,
         resource_group_id: str = None,
         tag: List[CreateVccRequestTag] = None,
@@ -461,14 +1011,15 @@
         vcc_id: str = None,
         vcc_name: str = None,
         vpc_id: str = None,
         vpd_id: str = None,
         zone_id: str = None,
     ):
         self.access_could_service = access_could_service
+        self.bandwidth = bandwidth
         self.bgp_cidr = bgp_cidr
         self.cen_id = cen_id
         self.connection_type = connection_type
         self.description = description
         self.region_id = region_id
         self.resource_group_id = resource_group_id
         self.tag = tag
@@ -489,14 +1040,16 @@
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.access_could_service is not None:
             result['AccessCouldService'] = self.access_could_service
+        if self.bandwidth is not None:
+            result['Bandwidth'] = self.bandwidth
         if self.bgp_cidr is not None:
             result['BgpCidr'] = self.bgp_cidr
         if self.cen_id is not None:
             result['CenId'] = self.cen_id
         if self.connection_type is not None:
             result['ConnectionType'] = self.connection_type
         if self.description is not None:
@@ -523,14 +1076,16 @@
             result['ZoneId'] = self.zone_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('AccessCouldService') is not None:
             self.access_could_service = m.get('AccessCouldService')
+        if m.get('Bandwidth') is not None:
+            self.bandwidth = m.get('Bandwidth')
         if m.get('BgpCidr') is not None:
             self.bgp_cidr = m.get('BgpCidr')
         if m.get('CenId') is not None:
             self.cen_id = m.get('CenId')
         if m.get('ConnectionType') is not None:
             self.connection_type = m.get('ConnectionType')
         if m.get('Description') is not None:
@@ -673,26 +1228,344 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = CreateVccResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class CreateVccGrantRuleRequest(TeaModel):
+    def __init__(
+        self,
+        er_id: str = None,
+        grant_tenant_id: str = None,
+        instance_id: str = None,
+        region_id: str = None,
+    ):
+        self.er_id = er_id
+        self.grant_tenant_id = grant_tenant_id
+        self.instance_id = instance_id
+        self.region_id = region_id
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
+        if self.er_id is not None:
+            result['ErId'] = self.er_id
+        if self.grant_tenant_id is not None:
+            result['GrantTenantId'] = self.grant_tenant_id
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ErId') is not None:
+            self.er_id = m.get('ErId')
+        if m.get('GrantTenantId') is not None:
+            self.grant_tenant_id = m.get('GrantTenantId')
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        return self
+
+
+class CreateVccGrantRuleResponseBodyContent(TeaModel):
+    def __init__(
+        self,
+        grant_rule_id: str = None,
+    ):
+        self.grant_rule_id = grant_rule_id
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
+        if self.grant_rule_id is not None:
+            result['GrantRuleId'] = self.grant_rule_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('GrantRuleId') is not None:
+            self.grant_rule_id = m.get('GrantRuleId')
+        return self
+
+
+class CreateVccGrantRuleResponseBody(TeaModel):
+    def __init__(
+        self,
+        code: int = None,
+        content: CreateVccGrantRuleResponseBodyContent = None,
+        message: str = None,
+        request_id: str = None,
+    ):
+        self.code = code
+        self.content = content
+        self.message = message
+        self.request_id = request_id
+
+    def validate(self):
+        if self.content:
+            self.content.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.content is not None:
+            result['Content'] = self.content.to_map()
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Content') is not None:
+            temp_model = CreateVccGrantRuleResponseBodyContent()
+            self.content = temp_model.from_map(m['Content'])
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class CreateVccGrantRuleResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: CreateVccGrantRuleResponseBody = None,
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
+            temp_model = CreateVccGrantRuleResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class CreateVccRouteEntryRequest(TeaModel):
+    def __init__(
+        self,
+        destination_cidr_block: str = None,
+        region_id: str = None,
+        vcc_id: str = None,
+    ):
+        self.destination_cidr_block = destination_cidr_block
+        self.region_id = region_id
+        self.vcc_id = vcc_id
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
+        if self.destination_cidr_block is not None:
+            result['DestinationCidrBlock'] = self.destination_cidr_block
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.vcc_id is not None:
+            result['VccId'] = self.vcc_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('DestinationCidrBlock') is not None:
+            self.destination_cidr_block = m.get('DestinationCidrBlock')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('VccId') is not None:
+            self.vcc_id = m.get('VccId')
+        return self
+
+
+class CreateVccRouteEntryResponseBodyContent(TeaModel):
+    def __init__(
+        self,
+        vcc_route_entry_id: str = None,
+    ):
+        self.vcc_route_entry_id = vcc_route_entry_id
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
+        if self.vcc_route_entry_id is not None:
+            result['VccRouteEntryId'] = self.vcc_route_entry_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('VccRouteEntryId') is not None:
+            self.vcc_route_entry_id = m.get('VccRouteEntryId')
+        return self
+
+
+class CreateVccRouteEntryResponseBody(TeaModel):
+    def __init__(
+        self,
+        code: int = None,
+        content: CreateVccRouteEntryResponseBodyContent = None,
+        message: str = None,
+        request_id: str = None,
+    ):
+        self.code = code
+        self.content = content
+        self.message = message
+        self.request_id = request_id
+
+    def validate(self):
+        if self.content:
+            self.content.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.content is not None:
+            result['Content'] = self.content.to_map()
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Content') is not None:
+            temp_model = CreateVccRouteEntryResponseBodyContent()
+            self.content = temp_model.from_map(m['Content'])
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class CreateVccRouteEntryResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: CreateVccRouteEntryResponseBody = None,
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
+            temp_model = CreateVccRouteEntryResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class CreateVpdRequestSubnets(TeaModel):
     def __init__(
         self,
         cidr: str = None,
-        client_token: str = None,
         region_id: str = None,
         subnet_name: str = None,
         type: str = None,
         zone_id: str = None,
     ):
         self.cidr = cidr
-        self.client_token = client_token
         self.region_id = region_id
         self.subnet_name = subnet_name
         self.type = type
         self.zone_id = zone_id
 
     def validate(self):
         pass
@@ -701,32 +1574,28 @@
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.cidr is not None:
             result['Cidr'] = self.cidr
-        if self.client_token is not None:
-            result['ClientToken'] = self.client_token
         if self.region_id is not None:
             result['RegionId'] = self.region_id
         if self.subnet_name is not None:
             result['SubnetName'] = self.subnet_name
         if self.type is not None:
             result['Type'] = self.type
         if self.zone_id is not None:
             result['ZoneId'] = self.zone_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('Cidr') is not None:
             self.cidr = m.get('Cidr')
-        if m.get('ClientToken') is not None:
-            self.client_token = m.get('ClientToken')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
         if m.get('SubnetName') is not None:
             self.subnet_name = m.get('SubnetName')
         if m.get('Type') is not None:
             self.type = m.get('Type')
         if m.get('ZoneId') is not None:
@@ -767,23 +1636,21 @@
         return self
 
 
 class CreateVpdRequest(TeaModel):
     def __init__(
         self,
         cidr: str = None,
-        client_token: str = None,
         region_id: str = None,
         resource_group_id: str = None,
         subnets: List[CreateVpdRequestSubnets] = None,
         tag: List[CreateVpdRequestTag] = None,
         vpd_name: str = None,
     ):
         self.cidr = cidr
-        self.client_token = client_token
         self.region_id = region_id
         self.resource_group_id = resource_group_id
         self.subnets = subnets
         self.tag = tag
         self.vpd_name = vpd_name
 
     def validate(self):
@@ -800,16 +1667,14 @@
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.cidr is not None:
             result['Cidr'] = self.cidr
-        if self.client_token is not None:
-            result['ClientToken'] = self.client_token
         if self.region_id is not None:
             result['RegionId'] = self.region_id
         if self.resource_group_id is not None:
             result['ResourceGroupId'] = self.resource_group_id
         result['Subnets'] = []
         if self.subnets is not None:
             for k in self.subnets:
@@ -822,16 +1687,14 @@
             result['VpdName'] = self.vpd_name
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('Cidr') is not None:
             self.cidr = m.get('Cidr')
-        if m.get('ClientToken') is not None:
-            self.client_token = m.get('ClientToken')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
         if m.get('ResourceGroupId') is not None:
             self.resource_group_id = m.get('ResourceGroupId')
         self.subnets = []
         if m.get('Subnets') is not None:
             for k in m.get('Subnets'):
@@ -1130,14 +1993,392 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = CreateVpdGrantRuleResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class DeleteErRequest(TeaModel):
+    def __init__(
+        self,
+        er_id: str = None,
+        region_id: str = None,
+    ):
+        self.er_id = er_id
+        self.region_id = region_id
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
+        if self.er_id is not None:
+            result['ErId'] = self.er_id
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ErId') is not None:
+            self.er_id = m.get('ErId')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        return self
+
+
+class DeleteErResponseBody(TeaModel):
+    def __init__(
+        self,
+        code: int = None,
+        content: Any = None,
+        message: str = None,
+        request_id: str = None,
+    ):
+        self.code = code
+        self.content = content
+        self.message = message
+        self.request_id = request_id
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
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.content is not None:
+            result['Content'] = self.content
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Content') is not None:
+            self.content = m.get('Content')
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class DeleteErResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: DeleteErResponseBody = None,
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
+            temp_model = DeleteErResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class DeleteErAttachmentRequest(TeaModel):
+    def __init__(
+        self,
+        er_attachment_id: str = None,
+        er_id: str = None,
+        region_id: str = None,
+    ):
+        self.er_attachment_id = er_attachment_id
+        self.er_id = er_id
+        self.region_id = region_id
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
+        if self.er_attachment_id is not None:
+            result['ErAttachmentId'] = self.er_attachment_id
+        if self.er_id is not None:
+            result['ErId'] = self.er_id
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ErAttachmentId') is not None:
+            self.er_attachment_id = m.get('ErAttachmentId')
+        if m.get('ErId') is not None:
+            self.er_id = m.get('ErId')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        return self
+
+
+class DeleteErAttachmentResponseBody(TeaModel):
+    def __init__(
+        self,
+        code: int = None,
+        content: Any = None,
+        message: str = None,
+        request_id: str = None,
+    ):
+        self.code = code
+        self.content = content
+        self.message = message
+        self.request_id = request_id
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
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.content is not None:
+            result['Content'] = self.content
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Content') is not None:
+            self.content = m.get('Content')
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class DeleteErAttachmentResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: DeleteErAttachmentResponseBody = None,
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
+            temp_model = DeleteErAttachmentResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class DeleteErRouteMapRequest(TeaModel):
+    def __init__(
+        self,
+        er_id: str = None,
+        er_route_map_ids: List[str] = None,
+        region_id: str = None,
+    ):
+        self.er_id = er_id
+        self.er_route_map_ids = er_route_map_ids
+        self.region_id = region_id
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
+        if self.er_id is not None:
+            result['ErId'] = self.er_id
+        if self.er_route_map_ids is not None:
+            result['ErRouteMapIds'] = self.er_route_map_ids
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ErId') is not None:
+            self.er_id = m.get('ErId')
+        if m.get('ErRouteMapIds') is not None:
+            self.er_route_map_ids = m.get('ErRouteMapIds')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        return self
+
+
+class DeleteErRouteMapResponseBody(TeaModel):
+    def __init__(
+        self,
+        code: int = None,
+        content: Any = None,
+        message: str = None,
+        request_id: str = None,
+    ):
+        self.code = code
+        self.content = content
+        self.message = message
+        self.request_id = request_id
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
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.content is not None:
+            result['Content'] = self.content
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Content') is not None:
+            self.content = m.get('Content')
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class DeleteErRouteMapResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: DeleteErRouteMapResponseBody = None,
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
+            temp_model = DeleteErRouteMapResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class DeleteSubnetRequest(TeaModel):
     def __init__(
         self,
         region_id: str = None,
         subnet_id: str = None,
         vpd_id: str = None,
         zone_id: str = None,
@@ -1264,14 +2505,282 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DeleteSubnetResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class DeleteVccGrantRuleRequest(TeaModel):
+    def __init__(
+        self,
+        er_id: str = None,
+        grant_rule_id: str = None,
+        instance_id: str = None,
+        region_id: str = None,
+    ):
+        self.er_id = er_id
+        self.grant_rule_id = grant_rule_id
+        self.instance_id = instance_id
+        self.region_id = region_id
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
+        if self.er_id is not None:
+            result['ErId'] = self.er_id
+        if self.grant_rule_id is not None:
+            result['GrantRuleId'] = self.grant_rule_id
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ErId') is not None:
+            self.er_id = m.get('ErId')
+        if m.get('GrantRuleId') is not None:
+            self.grant_rule_id = m.get('GrantRuleId')
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        return self
+
+
+class DeleteVccGrantRuleResponseBody(TeaModel):
+    def __init__(
+        self,
+        code: int = None,
+        content: Any = None,
+        message: str = None,
+        request_id: str = None,
+    ):
+        self.code = code
+        self.content = content
+        self.message = message
+        self.request_id = request_id
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
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.content is not None:
+            result['Content'] = self.content
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Content') is not None:
+            self.content = m.get('Content')
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class DeleteVccGrantRuleResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: DeleteVccGrantRuleResponseBody = None,
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
+            temp_model = DeleteVccGrantRuleResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class DeleteVccRouteEntryRequest(TeaModel):
+    def __init__(
+        self,
+        destination_cidr_block: str = None,
+        region_id: str = None,
+        vcc_id: str = None,
+        vcc_route_entry_id: str = None,
+    ):
+        self.destination_cidr_block = destination_cidr_block
+        self.region_id = region_id
+        self.vcc_id = vcc_id
+        self.vcc_route_entry_id = vcc_route_entry_id
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
+        if self.destination_cidr_block is not None:
+            result['DestinationCidrBlock'] = self.destination_cidr_block
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.vcc_id is not None:
+            result['VccId'] = self.vcc_id
+        if self.vcc_route_entry_id is not None:
+            result['VccRouteEntryId'] = self.vcc_route_entry_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('DestinationCidrBlock') is not None:
+            self.destination_cidr_block = m.get('DestinationCidrBlock')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('VccId') is not None:
+            self.vcc_id = m.get('VccId')
+        if m.get('VccRouteEntryId') is not None:
+            self.vcc_route_entry_id = m.get('VccRouteEntryId')
+        return self
+
+
+class DeleteVccRouteEntryResponseBody(TeaModel):
+    def __init__(
+        self,
+        code: int = None,
+        content: Any = None,
+        message: str = None,
+        request_id: str = None,
+    ):
+        self.code = code
+        self.content = content
+        self.message = message
+        self.request_id = request_id
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
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.content is not None:
+            result['Content'] = self.content
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Content') is not None:
+            self.content = m.get('Content')
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class DeleteVccRouteEntryResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: DeleteVccRouteEntryResponseBody = None,
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
+            temp_model = DeleteVccRouteEntryResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class DeleteVpdRequest(TeaModel):
     def __init__(
         self,
         region_id: str = None,
         vpd_id: str = None,
     ):
         self.region_id = region_id
@@ -1671,50 +3180,1367 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribeSlrResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class GetErRequest(TeaModel):
+    def __init__(
+        self,
+        er_id: str = None,
+        region_id: str = None,
+    ):
+        self.er_id = er_id
+        self.region_id = region_id
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
+        if self.er_id is not None:
+            result['ErId'] = self.er_id
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ErId') is not None:
+            self.er_id = m.get('ErId')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        return self
+
+
+class GetErResponseBodyContentErAttachments(TeaModel):
+    def __init__(
+        self,
+        across: bool = None,
+        auto_receive_all_route: bool = None,
+        create_time: str = None,
+        er_attachment_id: str = None,
+        er_attachment_name: str = None,
+        er_id: str = None,
+        gmt_modified: str = None,
+        instance_id: str = None,
+        instance_name: str = None,
+        instance_type: str = None,
+        message: str = None,
+        region_id: str = None,
+        resource_tenant_id: str = None,
+        status: str = None,
+        tenant_id: str = None,
+    ):
+        self.across = across
+        self.auto_receive_all_route = auto_receive_all_route
+        self.create_time = create_time
+        self.er_attachment_id = er_attachment_id
+        self.er_attachment_name = er_attachment_name
+        self.er_id = er_id
+        self.gmt_modified = gmt_modified
+        self.instance_id = instance_id
+        self.instance_name = instance_name
+        self.instance_type = instance_type
+        self.message = message
+        self.region_id = region_id
+        self.resource_tenant_id = resource_tenant_id
+        self.status = status
+        self.tenant_id = tenant_id
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
+        if self.across is not None:
+            result['Across'] = self.across
+        if self.auto_receive_all_route is not None:
+            result['AutoReceiveAllRoute'] = self.auto_receive_all_route
+        if self.create_time is not None:
+            result['CreateTime'] = self.create_time
+        if self.er_attachment_id is not None:
+            result['ErAttachmentId'] = self.er_attachment_id
+        if self.er_attachment_name is not None:
+            result['ErAttachmentName'] = self.er_attachment_name
+        if self.er_id is not None:
+            result['ErId'] = self.er_id
+        if self.gmt_modified is not None:
+            result['GmtModified'] = self.gmt_modified
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.instance_name is not None:
+            result['InstanceName'] = self.instance_name
+        if self.instance_type is not None:
+            result['InstanceType'] = self.instance_type
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.resource_tenant_id is not None:
+            result['ResourceTenantId'] = self.resource_tenant_id
+        if self.status is not None:
+            result['Status'] = self.status
+        if self.tenant_id is not None:
+            result['TenantId'] = self.tenant_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Across') is not None:
+            self.across = m.get('Across')
+        if m.get('AutoReceiveAllRoute') is not None:
+            self.auto_receive_all_route = m.get('AutoReceiveAllRoute')
+        if m.get('CreateTime') is not None:
+            self.create_time = m.get('CreateTime')
+        if m.get('ErAttachmentId') is not None:
+            self.er_attachment_id = m.get('ErAttachmentId')
+        if m.get('ErAttachmentName') is not None:
+            self.er_attachment_name = m.get('ErAttachmentName')
+        if m.get('ErId') is not None:
+            self.er_id = m.get('ErId')
+        if m.get('GmtModified') is not None:
+            self.gmt_modified = m.get('GmtModified')
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('InstanceName') is not None:
+            self.instance_name = m.get('InstanceName')
+        if m.get('InstanceType') is not None:
+            self.instance_type = m.get('InstanceType')
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('ResourceTenantId') is not None:
+            self.resource_tenant_id = m.get('ResourceTenantId')
+        if m.get('Status') is not None:
+            self.status = m.get('Status')
+        if m.get('TenantId') is not None:
+            self.tenant_id = m.get('TenantId')
+        return self
+
+
+class GetErResponseBodyContentErRouteEntrys(TeaModel):
+    def __init__(
+        self,
+        destination_cidr_block: str = None,
+        er_id: str = None,
+        er_route_entry_id: str = None,
+        gmt_modified: str = None,
+        next_hop_id: str = None,
+        next_hop_type: str = None,
+        region_id: str = None,
+        resource_tenant_id: str = None,
+        route_type: str = None,
+        status: str = None,
+        tenant_id: str = None,
+    ):
+        self.destination_cidr_block = destination_cidr_block
+        self.er_id = er_id
+        self.er_route_entry_id = er_route_entry_id
+        self.gmt_modified = gmt_modified
+        self.next_hop_id = next_hop_id
+        self.next_hop_type = next_hop_type
+        self.region_id = region_id
+        self.resource_tenant_id = resource_tenant_id
+        self.route_type = route_type
+        self.status = status
+        self.tenant_id = tenant_id
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
+        if self.destination_cidr_block is not None:
+            result['DestinationCidrBlock'] = self.destination_cidr_block
+        if self.er_id is not None:
+            result['ErId'] = self.er_id
+        if self.er_route_entry_id is not None:
+            result['ErRouteEntryId'] = self.er_route_entry_id
+        if self.gmt_modified is not None:
+            result['GmtModified'] = self.gmt_modified
+        if self.next_hop_id is not None:
+            result['NextHopId'] = self.next_hop_id
+        if self.next_hop_type is not None:
+            result['NextHopType'] = self.next_hop_type
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.resource_tenant_id is not None:
+            result['ResourceTenantId'] = self.resource_tenant_id
+        if self.route_type is not None:
+            result['RouteType'] = self.route_type
+        if self.status is not None:
+            result['Status'] = self.status
+        if self.tenant_id is not None:
+            result['TenantId'] = self.tenant_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('DestinationCidrBlock') is not None:
+            self.destination_cidr_block = m.get('DestinationCidrBlock')
+        if m.get('ErId') is not None:
+            self.er_id = m.get('ErId')
+        if m.get('ErRouteEntryId') is not None:
+            self.er_route_entry_id = m.get('ErRouteEntryId')
+        if m.get('GmtModified') is not None:
+            self.gmt_modified = m.get('GmtModified')
+        if m.get('NextHopId') is not None:
+            self.next_hop_id = m.get('NextHopId')
+        if m.get('NextHopType') is not None:
+            self.next_hop_type = m.get('NextHopType')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('ResourceTenantId') is not None:
+            self.resource_tenant_id = m.get('ResourceTenantId')
+        if m.get('RouteType') is not None:
+            self.route_type = m.get('RouteType')
+        if m.get('Status') is not None:
+            self.status = m.get('Status')
+        if m.get('TenantId') is not None:
+            self.tenant_id = m.get('TenantId')
+        return self
+
+
+class GetErResponseBodyContentErRouteMaps(TeaModel):
+    def __init__(
+        self,
+        action: str = None,
+        create_time: str = None,
+        description: str = None,
+        destination_cidr_block: str = None,
+        er_id: str = None,
+        er_route_map_id: str = None,
+        er_route_map_name: str = None,
+        gmt_modified: str = None,
+        message: str = None,
+        reception_instance_id: str = None,
+        reception_instance_name: str = None,
+        reception_instance_owner: str = None,
+        reception_instance_type: str = None,
+        region_id: str = None,
+        route_map_num: int = None,
+        status: str = None,
+        tenant_id: str = None,
+        transmission_instance_id: str = None,
+        transmission_instance_name: str = None,
+        transmission_instance_owner: str = None,
+        transmission_instance_type: str = None,
+    ):
+        self.action = action
+        self.create_time = create_time
+        self.description = description
+        self.destination_cidr_block = destination_cidr_block
+        self.er_id = er_id
+        self.er_route_map_id = er_route_map_id
+        self.er_route_map_name = er_route_map_name
+        self.gmt_modified = gmt_modified
+        self.message = message
+        self.reception_instance_id = reception_instance_id
+        self.reception_instance_name = reception_instance_name
+        self.reception_instance_owner = reception_instance_owner
+        self.reception_instance_type = reception_instance_type
+        self.region_id = region_id
+        self.route_map_num = route_map_num
+        self.status = status
+        self.tenant_id = tenant_id
+        self.transmission_instance_id = transmission_instance_id
+        self.transmission_instance_name = transmission_instance_name
+        self.transmission_instance_owner = transmission_instance_owner
+        self.transmission_instance_type = transmission_instance_type
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
+        if self.action is not None:
+            result['Action'] = self.action
+        if self.create_time is not None:
+            result['CreateTime'] = self.create_time
+        if self.description is not None:
+            result['Description'] = self.description
+        if self.destination_cidr_block is not None:
+            result['DestinationCidrBlock'] = self.destination_cidr_block
+        if self.er_id is not None:
+            result['ErId'] = self.er_id
+        if self.er_route_map_id is not None:
+            result['ErRouteMapId'] = self.er_route_map_id
+        if self.er_route_map_name is not None:
+            result['ErRouteMapName'] = self.er_route_map_name
+        if self.gmt_modified is not None:
+            result['GmtModified'] = self.gmt_modified
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.reception_instance_id is not None:
+            result['ReceptionInstanceId'] = self.reception_instance_id
+        if self.reception_instance_name is not None:
+            result['ReceptionInstanceName'] = self.reception_instance_name
+        if self.reception_instance_owner is not None:
+            result['ReceptionInstanceOwner'] = self.reception_instance_owner
+        if self.reception_instance_type is not None:
+            result['ReceptionInstanceType'] = self.reception_instance_type
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.route_map_num is not None:
+            result['RouteMapNum'] = self.route_map_num
+        if self.status is not None:
+            result['Status'] = self.status
+        if self.tenant_id is not None:
+            result['TenantId'] = self.tenant_id
+        if self.transmission_instance_id is not None:
+            result['TransmissionInstanceId'] = self.transmission_instance_id
+        if self.transmission_instance_name is not None:
+            result['TransmissionInstanceName'] = self.transmission_instance_name
+        if self.transmission_instance_owner is not None:
+            result['TransmissionInstanceOwner'] = self.transmission_instance_owner
+        if self.transmission_instance_type is not None:
+            result['TransmissionInstanceType'] = self.transmission_instance_type
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Action') is not None:
+            self.action = m.get('Action')
+        if m.get('CreateTime') is not None:
+            self.create_time = m.get('CreateTime')
+        if m.get('Description') is not None:
+            self.description = m.get('Description')
+        if m.get('DestinationCidrBlock') is not None:
+            self.destination_cidr_block = m.get('DestinationCidrBlock')
+        if m.get('ErId') is not None:
+            self.er_id = m.get('ErId')
+        if m.get('ErRouteMapId') is not None:
+            self.er_route_map_id = m.get('ErRouteMapId')
+        if m.get('ErRouteMapName') is not None:
+            self.er_route_map_name = m.get('ErRouteMapName')
+        if m.get('GmtModified') is not None:
+            self.gmt_modified = m.get('GmtModified')
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('ReceptionInstanceId') is not None:
+            self.reception_instance_id = m.get('ReceptionInstanceId')
+        if m.get('ReceptionInstanceName') is not None:
+            self.reception_instance_name = m.get('ReceptionInstanceName')
+        if m.get('ReceptionInstanceOwner') is not None:
+            self.reception_instance_owner = m.get('ReceptionInstanceOwner')
+        if m.get('ReceptionInstanceType') is not None:
+            self.reception_instance_type = m.get('ReceptionInstanceType')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('RouteMapNum') is not None:
+            self.route_map_num = m.get('RouteMapNum')
+        if m.get('Status') is not None:
+            self.status = m.get('Status')
+        if m.get('TenantId') is not None:
+            self.tenant_id = m.get('TenantId')
+        if m.get('TransmissionInstanceId') is not None:
+            self.transmission_instance_id = m.get('TransmissionInstanceId')
+        if m.get('TransmissionInstanceName') is not None:
+            self.transmission_instance_name = m.get('TransmissionInstanceName')
+        if m.get('TransmissionInstanceOwner') is not None:
+            self.transmission_instance_owner = m.get('TransmissionInstanceOwner')
+        if m.get('TransmissionInstanceType') is not None:
+            self.transmission_instance_type = m.get('TransmissionInstanceType')
+        return self
+
+
+class GetErResponseBodyContent(TeaModel):
+    def __init__(
+        self,
+        create_time: str = None,
+        description: str = None,
+        er_attachments: List[GetErResponseBodyContentErAttachments] = None,
+        er_id: str = None,
+        er_name: str = None,
+        er_route_entrys: List[GetErResponseBodyContentErRouteEntrys] = None,
+        er_route_maps: List[GetErResponseBodyContentErRouteMaps] = None,
+        gmt_modified: str = None,
+        master_zone_id: str = None,
+        message: str = None,
+        region_id: str = None,
+        status: str = None,
+        tenant_id: str = None,
+    ):
+        self.create_time = create_time
+        self.description = description
+        self.er_attachments = er_attachments
+        self.er_id = er_id
+        self.er_name = er_name
+        self.er_route_entrys = er_route_entrys
+        self.er_route_maps = er_route_maps
+        self.gmt_modified = gmt_modified
+        self.master_zone_id = master_zone_id
+        self.message = message
+        self.region_id = region_id
+        self.status = status
+        self.tenant_id = tenant_id
+
+    def validate(self):
+        if self.er_attachments:
+            for k in self.er_attachments:
+                if k:
+                    k.validate()
+        if self.er_route_entrys:
+            for k in self.er_route_entrys:
+                if k:
+                    k.validate()
+        if self.er_route_maps:
+            for k in self.er_route_maps:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.create_time is not None:
+            result['CreateTime'] = self.create_time
+        if self.description is not None:
+            result['Description'] = self.description
+        result['ErAttachments'] = []
+        if self.er_attachments is not None:
+            for k in self.er_attachments:
+                result['ErAttachments'].append(k.to_map() if k else None)
+        if self.er_id is not None:
+            result['ErId'] = self.er_id
+        if self.er_name is not None:
+            result['ErName'] = self.er_name
+        result['ErRouteEntrys'] = []
+        if self.er_route_entrys is not None:
+            for k in self.er_route_entrys:
+                result['ErRouteEntrys'].append(k.to_map() if k else None)
+        result['ErRouteMaps'] = []
+        if self.er_route_maps is not None:
+            for k in self.er_route_maps:
+                result['ErRouteMaps'].append(k.to_map() if k else None)
+        if self.gmt_modified is not None:
+            result['GmtModified'] = self.gmt_modified
+        if self.master_zone_id is not None:
+            result['MasterZoneId'] = self.master_zone_id
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.status is not None:
+            result['Status'] = self.status
+        if self.tenant_id is not None:
+            result['TenantId'] = self.tenant_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('CreateTime') is not None:
+            self.create_time = m.get('CreateTime')
+        if m.get('Description') is not None:
+            self.description = m.get('Description')
+        self.er_attachments = []
+        if m.get('ErAttachments') is not None:
+            for k in m.get('ErAttachments'):
+                temp_model = GetErResponseBodyContentErAttachments()
+                self.er_attachments.append(temp_model.from_map(k))
+        if m.get('ErId') is not None:
+            self.er_id = m.get('ErId')
+        if m.get('ErName') is not None:
+            self.er_name = m.get('ErName')
+        self.er_route_entrys = []
+        if m.get('ErRouteEntrys') is not None:
+            for k in m.get('ErRouteEntrys'):
+                temp_model = GetErResponseBodyContentErRouteEntrys()
+                self.er_route_entrys.append(temp_model.from_map(k))
+        self.er_route_maps = []
+        if m.get('ErRouteMaps') is not None:
+            for k in m.get('ErRouteMaps'):
+                temp_model = GetErResponseBodyContentErRouteMaps()
+                self.er_route_maps.append(temp_model.from_map(k))
+        if m.get('GmtModified') is not None:
+            self.gmt_modified = m.get('GmtModified')
+        if m.get('MasterZoneId') is not None:
+            self.master_zone_id = m.get('MasterZoneId')
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('Status') is not None:
+            self.status = m.get('Status')
+        if m.get('TenantId') is not None:
+            self.tenant_id = m.get('TenantId')
+        return self
+
+
+class GetErResponseBody(TeaModel):
+    def __init__(
+        self,
+        code: int = None,
+        content: GetErResponseBodyContent = None,
+        message: str = None,
+        request_id: str = None,
+    ):
+        self.code = code
+        self.content = content
+        self.message = message
+        self.request_id = request_id
+
+    def validate(self):
+        if self.content:
+            self.content.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.content is not None:
+            result['Content'] = self.content.to_map()
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Content') is not None:
+            temp_model = GetErResponseBodyContent()
+            self.content = temp_model.from_map(m['Content'])
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class GetErResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: GetErResponseBody = None,
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
+            temp_model = GetErResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class GetErAttachmentRequest(TeaModel):
+    def __init__(
+        self,
+        er_attachment_id: str = None,
+        er_id: str = None,
+        region_id: str = None,
+    ):
+        self.er_attachment_id = er_attachment_id
+        self.er_id = er_id
+        self.region_id = region_id
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
+        if self.er_attachment_id is not None:
+            result['ErAttachmentId'] = self.er_attachment_id
+        if self.er_id is not None:
+            result['ErId'] = self.er_id
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ErAttachmentId') is not None:
+            self.er_attachment_id = m.get('ErAttachmentId')
+        if m.get('ErId') is not None:
+            self.er_id = m.get('ErId')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        return self
+
+
+class GetErAttachmentResponseBodyContent(TeaModel):
+    def __init__(
+        self,
+        across: bool = None,
+        auto_receive_all_route: bool = None,
+        create_time: str = None,
+        er_attachment_id: str = None,
+        er_attachment_name: str = None,
+        er_id: str = None,
+        gmt_modified: str = None,
+        instance_id: str = None,
+        instance_name: str = None,
+        instance_type: str = None,
+        message: str = None,
+        region_id: str = None,
+        resource_tenant_id: str = None,
+        status: str = None,
+        tenant_id: str = None,
+    ):
+        self.across = across
+        self.auto_receive_all_route = auto_receive_all_route
+        self.create_time = create_time
+        self.er_attachment_id = er_attachment_id
+        self.er_attachment_name = er_attachment_name
+        self.er_id = er_id
+        self.gmt_modified = gmt_modified
+        self.instance_id = instance_id
+        self.instance_name = instance_name
+        self.instance_type = instance_type
+        self.message = message
+        self.region_id = region_id
+        self.resource_tenant_id = resource_tenant_id
+        self.status = status
+        self.tenant_id = tenant_id
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
+        if self.across is not None:
+            result['Across'] = self.across
+        if self.auto_receive_all_route is not None:
+            result['AutoReceiveAllRoute'] = self.auto_receive_all_route
+        if self.create_time is not None:
+            result['CreateTime'] = self.create_time
+        if self.er_attachment_id is not None:
+            result['ErAttachmentId'] = self.er_attachment_id
+        if self.er_attachment_name is not None:
+            result['ErAttachmentName'] = self.er_attachment_name
+        if self.er_id is not None:
+            result['ErId'] = self.er_id
+        if self.gmt_modified is not None:
+            result['GmtModified'] = self.gmt_modified
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.instance_name is not None:
+            result['InstanceName'] = self.instance_name
+        if self.instance_type is not None:
+            result['InstanceType'] = self.instance_type
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.resource_tenant_id is not None:
+            result['ResourceTenantId'] = self.resource_tenant_id
+        if self.status is not None:
+            result['Status'] = self.status
+        if self.tenant_id is not None:
+            result['TenantId'] = self.tenant_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Across') is not None:
+            self.across = m.get('Across')
+        if m.get('AutoReceiveAllRoute') is not None:
+            self.auto_receive_all_route = m.get('AutoReceiveAllRoute')
+        if m.get('CreateTime') is not None:
+            self.create_time = m.get('CreateTime')
+        if m.get('ErAttachmentId') is not None:
+            self.er_attachment_id = m.get('ErAttachmentId')
+        if m.get('ErAttachmentName') is not None:
+            self.er_attachment_name = m.get('ErAttachmentName')
+        if m.get('ErId') is not None:
+            self.er_id = m.get('ErId')
+        if m.get('GmtModified') is not None:
+            self.gmt_modified = m.get('GmtModified')
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('InstanceName') is not None:
+            self.instance_name = m.get('InstanceName')
+        if m.get('InstanceType') is not None:
+            self.instance_type = m.get('InstanceType')
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('ResourceTenantId') is not None:
+            self.resource_tenant_id = m.get('ResourceTenantId')
+        if m.get('Status') is not None:
+            self.status = m.get('Status')
+        if m.get('TenantId') is not None:
+            self.tenant_id = m.get('TenantId')
+        return self
+
+
+class GetErAttachmentResponseBody(TeaModel):
+    def __init__(
+        self,
+        code: int = None,
+        content: GetErAttachmentResponseBodyContent = None,
+        message: str = None,
+        request_id: str = None,
+    ):
+        self.code = code
+        self.content = content
+        self.message = message
+        self.request_id = request_id
+
+    def validate(self):
+        if self.content:
+            self.content.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.content is not None:
+            result['Content'] = self.content.to_map()
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Content') is not None:
+            temp_model = GetErAttachmentResponseBodyContent()
+            self.content = temp_model.from_map(m['Content'])
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class GetErAttachmentResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: GetErAttachmentResponseBody = None,
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
+            temp_model = GetErAttachmentResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class GetErRouteEntryRequest(TeaModel):
+    def __init__(
+        self,
+        er_id: str = None,
+        er_route_entry_id: str = None,
+        region_id: str = None,
+    ):
+        self.er_id = er_id
+        self.er_route_entry_id = er_route_entry_id
+        self.region_id = region_id
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
+        if self.er_id is not None:
+            result['ErId'] = self.er_id
+        if self.er_route_entry_id is not None:
+            result['ErRouteEntryId'] = self.er_route_entry_id
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ErId') is not None:
+            self.er_id = m.get('ErId')
+        if m.get('ErRouteEntryId') is not None:
+            self.er_route_entry_id = m.get('ErRouteEntryId')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        return self
+
+
+class GetErRouteEntryResponseBodyContent(TeaModel):
+    def __init__(
+        self,
+        destination_cidr_block: str = None,
+        er_id: str = None,
+        er_route_entry_id: str = None,
+        gmt_modified: str = None,
+        next_hop_id: str = None,
+        next_hop_type: str = None,
+        region_id: str = None,
+        route_type: str = None,
+        status: str = None,
+        tenant_id: str = None,
+    ):
+        self.destination_cidr_block = destination_cidr_block
+        self.er_id = er_id
+        self.er_route_entry_id = er_route_entry_id
+        self.gmt_modified = gmt_modified
+        self.next_hop_id = next_hop_id
+        self.next_hop_type = next_hop_type
+        self.region_id = region_id
+        self.route_type = route_type
+        self.status = status
+        self.tenant_id = tenant_id
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
+        if self.destination_cidr_block is not None:
+            result['DestinationCidrBlock'] = self.destination_cidr_block
+        if self.er_id is not None:
+            result['ErId'] = self.er_id
+        if self.er_route_entry_id is not None:
+            result['ErRouteEntryId'] = self.er_route_entry_id
+        if self.gmt_modified is not None:
+            result['GmtModified'] = self.gmt_modified
+        if self.next_hop_id is not None:
+            result['NextHopId'] = self.next_hop_id
+        if self.next_hop_type is not None:
+            result['NextHopType'] = self.next_hop_type
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.route_type is not None:
+            result['RouteType'] = self.route_type
+        if self.status is not None:
+            result['Status'] = self.status
+        if self.tenant_id is not None:
+            result['TenantId'] = self.tenant_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('DestinationCidrBlock') is not None:
+            self.destination_cidr_block = m.get('DestinationCidrBlock')
+        if m.get('ErId') is not None:
+            self.er_id = m.get('ErId')
+        if m.get('ErRouteEntryId') is not None:
+            self.er_route_entry_id = m.get('ErRouteEntryId')
+        if m.get('GmtModified') is not None:
+            self.gmt_modified = m.get('GmtModified')
+        if m.get('NextHopId') is not None:
+            self.next_hop_id = m.get('NextHopId')
+        if m.get('NextHopType') is not None:
+            self.next_hop_type = m.get('NextHopType')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('RouteType') is not None:
+            self.route_type = m.get('RouteType')
+        if m.get('Status') is not None:
+            self.status = m.get('Status')
+        if m.get('TenantId') is not None:
+            self.tenant_id = m.get('TenantId')
+        return self
+
+
+class GetErRouteEntryResponseBody(TeaModel):
+    def __init__(
+        self,
+        code: int = None,
+        content: GetErRouteEntryResponseBodyContent = None,
+        message: str = None,
+        request_id: str = None,
+    ):
+        self.code = code
+        self.content = content
+        self.message = message
+        self.request_id = request_id
+
+    def validate(self):
+        if self.content:
+            self.content.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.content is not None:
+            result['Content'] = self.content.to_map()
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Content') is not None:
+            temp_model = GetErRouteEntryResponseBodyContent()
+            self.content = temp_model.from_map(m['Content'])
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class GetErRouteEntryResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: GetErRouteEntryResponseBody = None,
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
+            temp_model = GetErRouteEntryResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class GetErRouteMapRequest(TeaModel):
+    def __init__(
+        self,
+        er_id: str = None,
+        er_route_map_id: str = None,
+        region_id: str = None,
+    ):
+        self.er_id = er_id
+        self.er_route_map_id = er_route_map_id
+        self.region_id = region_id
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
+        if self.er_id is not None:
+            result['ErId'] = self.er_id
+        if self.er_route_map_id is not None:
+            result['ErRouteMapId'] = self.er_route_map_id
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ErId') is not None:
+            self.er_id = m.get('ErId')
+        if m.get('ErRouteMapId') is not None:
+            self.er_route_map_id = m.get('ErRouteMapId')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        return self
+
+
+class GetErRouteMapResponseBodyContent(TeaModel):
+    def __init__(
+        self,
+        action: str = None,
+        description: str = None,
+        destination_cidr_block: str = None,
+        er_id: str = None,
+        er_route_map_id: str = None,
+        er_route_map_name: str = None,
+        gmt_create: str = None,
+        gmt_modified: str = None,
+        message: str = None,
+        reception_instance_id: str = None,
+        reception_instance_name: str = None,
+        reception_instance_owner: str = None,
+        reception_instance_type: str = None,
+        region_id: str = None,
+        route_map_num: int = None,
+        status: str = None,
+        tenant_id: str = None,
+        transmission_instance_id: str = None,
+        transmission_instance_name: str = None,
+        transmission_instance_owner: str = None,
+        transmission_instance_type: str = None,
+    ):
+        self.action = action
+        self.description = description
+        self.destination_cidr_block = destination_cidr_block
+        self.er_id = er_id
+        self.er_route_map_id = er_route_map_id
+        self.er_route_map_name = er_route_map_name
+        self.gmt_create = gmt_create
+        self.gmt_modified = gmt_modified
+        self.message = message
+        self.reception_instance_id = reception_instance_id
+        self.reception_instance_name = reception_instance_name
+        self.reception_instance_owner = reception_instance_owner
+        self.reception_instance_type = reception_instance_type
+        self.region_id = region_id
+        self.route_map_num = route_map_num
+        self.status = status
+        self.tenant_id = tenant_id
+        self.transmission_instance_id = transmission_instance_id
+        self.transmission_instance_name = transmission_instance_name
+        self.transmission_instance_owner = transmission_instance_owner
+        self.transmission_instance_type = transmission_instance_type
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
+        if self.action is not None:
+            result['Action'] = self.action
+        if self.description is not None:
+            result['Description'] = self.description
+        if self.destination_cidr_block is not None:
+            result['DestinationCidrBlock'] = self.destination_cidr_block
+        if self.er_id is not None:
+            result['ErId'] = self.er_id
+        if self.er_route_map_id is not None:
+            result['ErRouteMapId'] = self.er_route_map_id
+        if self.er_route_map_name is not None:
+            result['ErRouteMapName'] = self.er_route_map_name
+        if self.gmt_create is not None:
+            result['GmtCreate'] = self.gmt_create
+        if self.gmt_modified is not None:
+            result['GmtModified'] = self.gmt_modified
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.reception_instance_id is not None:
+            result['ReceptionInstanceId'] = self.reception_instance_id
+        if self.reception_instance_name is not None:
+            result['ReceptionInstanceName'] = self.reception_instance_name
+        if self.reception_instance_owner is not None:
+            result['ReceptionInstanceOwner'] = self.reception_instance_owner
+        if self.reception_instance_type is not None:
+            result['ReceptionInstanceType'] = self.reception_instance_type
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.route_map_num is not None:
+            result['RouteMapNum'] = self.route_map_num
+        if self.status is not None:
+            result['Status'] = self.status
+        if self.tenant_id is not None:
+            result['TenantId'] = self.tenant_id
+        if self.transmission_instance_id is not None:
+            result['TransmissionInstanceId'] = self.transmission_instance_id
+        if self.transmission_instance_name is not None:
+            result['TransmissionInstanceName'] = self.transmission_instance_name
+        if self.transmission_instance_owner is not None:
+            result['TransmissionInstanceOwner'] = self.transmission_instance_owner
+        if self.transmission_instance_type is not None:
+            result['TransmissionInstanceType'] = self.transmission_instance_type
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Action') is not None:
+            self.action = m.get('Action')
+        if m.get('Description') is not None:
+            self.description = m.get('Description')
+        if m.get('DestinationCidrBlock') is not None:
+            self.destination_cidr_block = m.get('DestinationCidrBlock')
+        if m.get('ErId') is not None:
+            self.er_id = m.get('ErId')
+        if m.get('ErRouteMapId') is not None:
+            self.er_route_map_id = m.get('ErRouteMapId')
+        if m.get('ErRouteMapName') is not None:
+            self.er_route_map_name = m.get('ErRouteMapName')
+        if m.get('GmtCreate') is not None:
+            self.gmt_create = m.get('GmtCreate')
+        if m.get('GmtModified') is not None:
+            self.gmt_modified = m.get('GmtModified')
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('ReceptionInstanceId') is not None:
+            self.reception_instance_id = m.get('ReceptionInstanceId')
+        if m.get('ReceptionInstanceName') is not None:
+            self.reception_instance_name = m.get('ReceptionInstanceName')
+        if m.get('ReceptionInstanceOwner') is not None:
+            self.reception_instance_owner = m.get('ReceptionInstanceOwner')
+        if m.get('ReceptionInstanceType') is not None:
+            self.reception_instance_type = m.get('ReceptionInstanceType')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('RouteMapNum') is not None:
+            self.route_map_num = m.get('RouteMapNum')
+        if m.get('Status') is not None:
+            self.status = m.get('Status')
+        if m.get('TenantId') is not None:
+            self.tenant_id = m.get('TenantId')
+        if m.get('TransmissionInstanceId') is not None:
+            self.transmission_instance_id = m.get('TransmissionInstanceId')
+        if m.get('TransmissionInstanceName') is not None:
+            self.transmission_instance_name = m.get('TransmissionInstanceName')
+        if m.get('TransmissionInstanceOwner') is not None:
+            self.transmission_instance_owner = m.get('TransmissionInstanceOwner')
+        if m.get('TransmissionInstanceType') is not None:
+            self.transmission_instance_type = m.get('TransmissionInstanceType')
+        return self
+
+
+class GetErRouteMapResponseBody(TeaModel):
+    def __init__(
+        self,
+        code: int = None,
+        content: GetErRouteMapResponseBodyContent = None,
+        message: str = None,
+        request_id: str = None,
+    ):
+        self.code = code
+        self.content = content
+        self.message = message
+        self.request_id = request_id
+
+    def validate(self):
+        if self.content:
+            self.content.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.content is not None:
+            result['Content'] = self.content.to_map()
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Content') is not None:
+            temp_model = GetErRouteMapResponseBodyContent()
+            self.content = temp_model.from_map(m['Content'])
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class GetErRouteMapResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: GetErRouteMapResponseBody = None,
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
+            temp_model = GetErRouteMapResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class GetLniPrivateIpAddressRequest(TeaModel):
     def __init__(
         self,
-        client_token: str = None,
         ip_name: str = None,
         network_interface_id: str = None,
         region_id: str = None,
     ):
-        self.client_token = client_token
         self.ip_name = ip_name
         self.network_interface_id = network_interface_id
         self.region_id = region_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.client_token is not None:
-            result['ClientToken'] = self.client_token
         if self.ip_name is not None:
             result['IpName'] = self.ip_name
         if self.network_interface_id is not None:
             result['NetworkInterfaceId'] = self.network_interface_id
         if self.region_id is not None:
             result['RegionId'] = self.region_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ClientToken') is not None:
-            self.client_token = m.get('ClientToken')
         if m.get('IpName') is not None:
             self.ip_name = m.get('IpName')
         if m.get('NetworkInterfaceId') is not None:
             self.network_interface_id = m.get('NetworkInterfaceId')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
         return self
@@ -1876,50 +4702,452 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = GetLniPrivateIpAddressResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class GetNetworkInterfaceRequest(TeaModel):
+    def __init__(
+        self,
+        network_interface_id: str = None,
+        region_id: str = None,
+        subnet_id: str = None,
+    ):
+        self.network_interface_id = network_interface_id
+        self.region_id = region_id
+        self.subnet_id = subnet_id
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
+        if self.network_interface_id is not None:
+            result['NetworkInterfaceId'] = self.network_interface_id
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.subnet_id is not None:
+            result['SubnetId'] = self.subnet_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('NetworkInterfaceId') is not None:
+            self.network_interface_id = m.get('NetworkInterfaceId')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('SubnetId') is not None:
+            self.subnet_id = m.get('SubnetId')
+        return self
+
+
+class GetNetworkInterfaceResponseBodyContentPrivateIpAddressMacGroup(TeaModel):
+    def __init__(
+        self,
+        ip_address_mac: str = None,
+        ip_name: str = None,
+        message: str = None,
+        private_ip_address: str = None,
+        status: str = None,
+    ):
+        self.ip_address_mac = ip_address_mac
+        self.ip_name = ip_name
+        self.message = message
+        self.private_ip_address = private_ip_address
+        self.status = status
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
+        if self.ip_address_mac is not None:
+            result['IpAddressMac'] = self.ip_address_mac
+        if self.ip_name is not None:
+            result['IpName'] = self.ip_name
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.private_ip_address is not None:
+            result['PrivateIpAddress'] = self.private_ip_address
+        if self.status is not None:
+            result['Status'] = self.status
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('IpAddressMac') is not None:
+            self.ip_address_mac = m.get('IpAddressMac')
+        if m.get('IpName') is not None:
+            self.ip_name = m.get('IpName')
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('PrivateIpAddress') is not None:
+            self.private_ip_address = m.get('PrivateIpAddress')
+        if m.get('Status') is not None:
+            self.status = m.get('Status')
+        return self
+
+
+class GetNetworkInterfaceResponseBodyContentSubnetBaseInfo(TeaModel):
+    def __init__(
+        self,
+        cidr: str = None,
+        create_time: str = None,
+        subnet_id: str = None,
+        subnet_name: str = None,
+    ):
+        self.cidr = cidr
+        self.create_time = create_time
+        self.subnet_id = subnet_id
+        self.subnet_name = subnet_name
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
+        if self.cidr is not None:
+            result['Cidr'] = self.cidr
+        if self.create_time is not None:
+            result['CreateTime'] = self.create_time
+        if self.subnet_id is not None:
+            result['SubnetId'] = self.subnet_id
+        if self.subnet_name is not None:
+            result['SubnetName'] = self.subnet_name
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Cidr') is not None:
+            self.cidr = m.get('Cidr')
+        if m.get('CreateTime') is not None:
+            self.create_time = m.get('CreateTime')
+        if m.get('SubnetId') is not None:
+            self.subnet_id = m.get('SubnetId')
+        if m.get('SubnetName') is not None:
+            self.subnet_name = m.get('SubnetName')
+        return self
+
+
+class GetNetworkInterfaceResponseBodyContentVpdBaseInfo(TeaModel):
+    def __init__(
+        self,
+        cidr: str = None,
+        create_time: str = None,
+        vpd_id: str = None,
+        vpd_name: str = None,
+    ):
+        self.cidr = cidr
+        self.create_time = create_time
+        self.vpd_id = vpd_id
+        self.vpd_name = vpd_name
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
+        if self.cidr is not None:
+            result['Cidr'] = self.cidr
+        if self.create_time is not None:
+            result['CreateTime'] = self.create_time
+        if self.vpd_id is not None:
+            result['VpdId'] = self.vpd_id
+        if self.vpd_name is not None:
+            result['VpdName'] = self.vpd_name
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Cidr') is not None:
+            self.cidr = m.get('Cidr')
+        if m.get('CreateTime') is not None:
+            self.create_time = m.get('CreateTime')
+        if m.get('VpdId') is not None:
+            self.vpd_id = m.get('VpdId')
+        if m.get('VpdName') is not None:
+            self.vpd_name = m.get('VpdName')
+        return self
+
+
+class GetNetworkInterfaceResponseBodyContent(TeaModel):
+    def __init__(
+        self,
+        create_time: str = None,
+        ethernet: List[str] = None,
+        gateway: str = None,
+        ip: str = None,
+        nc_type: str = None,
+        network_interface_id: str = None,
+        network_interface_name: str = None,
+        node_id: str = None,
+        private_ip_address_mac_group: List[GetNetworkInterfaceResponseBodyContentPrivateIpAddressMacGroup] = None,
+        quota: int = None,
+        region_id: str = None,
+        service_mac: str = None,
+        status: str = None,
+        subnet_base_info: GetNetworkInterfaceResponseBodyContentSubnetBaseInfo = None,
+        tenant_id: str = None,
+        vpd_base_info: GetNetworkInterfaceResponseBodyContentVpdBaseInfo = None,
+        zone_id: str = None,
+    ):
+        self.create_time = create_time
+        self.ethernet = ethernet
+        self.gateway = gateway
+        self.ip = ip
+        self.nc_type = nc_type
+        self.network_interface_id = network_interface_id
+        self.network_interface_name = network_interface_name
+        self.node_id = node_id
+        self.private_ip_address_mac_group = private_ip_address_mac_group
+        self.quota = quota
+        self.region_id = region_id
+        self.service_mac = service_mac
+        self.status = status
+        self.subnet_base_info = subnet_base_info
+        self.tenant_id = tenant_id
+        self.vpd_base_info = vpd_base_info
+        self.zone_id = zone_id
+
+    def validate(self):
+        if self.private_ip_address_mac_group:
+            for k in self.private_ip_address_mac_group:
+                if k:
+                    k.validate()
+        if self.subnet_base_info:
+            self.subnet_base_info.validate()
+        if self.vpd_base_info:
+            self.vpd_base_info.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.create_time is not None:
+            result['CreateTime'] = self.create_time
+        if self.ethernet is not None:
+            result['Ethernet'] = self.ethernet
+        if self.gateway is not None:
+            result['Gateway'] = self.gateway
+        if self.ip is not None:
+            result['Ip'] = self.ip
+        if self.nc_type is not None:
+            result['NcType'] = self.nc_type
+        if self.network_interface_id is not None:
+            result['NetworkInterfaceId'] = self.network_interface_id
+        if self.network_interface_name is not None:
+            result['NetworkInterfaceName'] = self.network_interface_name
+        if self.node_id is not None:
+            result['NodeId'] = self.node_id
+        result['PrivateIpAddressMacGroup'] = []
+        if self.private_ip_address_mac_group is not None:
+            for k in self.private_ip_address_mac_group:
+                result['PrivateIpAddressMacGroup'].append(k.to_map() if k else None)
+        if self.quota is not None:
+            result['Quota'] = self.quota
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.service_mac is not None:
+            result['ServiceMac'] = self.service_mac
+        if self.status is not None:
+            result['Status'] = self.status
+        if self.subnet_base_info is not None:
+            result['SubnetBaseInfo'] = self.subnet_base_info.to_map()
+        if self.tenant_id is not None:
+            result['TenantId'] = self.tenant_id
+        if self.vpd_base_info is not None:
+            result['VpdBaseInfo'] = self.vpd_base_info.to_map()
+        if self.zone_id is not None:
+            result['ZoneId'] = self.zone_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('CreateTime') is not None:
+            self.create_time = m.get('CreateTime')
+        if m.get('Ethernet') is not None:
+            self.ethernet = m.get('Ethernet')
+        if m.get('Gateway') is not None:
+            self.gateway = m.get('Gateway')
+        if m.get('Ip') is not None:
+            self.ip = m.get('Ip')
+        if m.get('NcType') is not None:
+            self.nc_type = m.get('NcType')
+        if m.get('NetworkInterfaceId') is not None:
+            self.network_interface_id = m.get('NetworkInterfaceId')
+        if m.get('NetworkInterfaceName') is not None:
+            self.network_interface_name = m.get('NetworkInterfaceName')
+        if m.get('NodeId') is not None:
+            self.node_id = m.get('NodeId')
+        self.private_ip_address_mac_group = []
+        if m.get('PrivateIpAddressMacGroup') is not None:
+            for k in m.get('PrivateIpAddressMacGroup'):
+                temp_model = GetNetworkInterfaceResponseBodyContentPrivateIpAddressMacGroup()
+                self.private_ip_address_mac_group.append(temp_model.from_map(k))
+        if m.get('Quota') is not None:
+            self.quota = m.get('Quota')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('ServiceMac') is not None:
+            self.service_mac = m.get('ServiceMac')
+        if m.get('Status') is not None:
+            self.status = m.get('Status')
+        if m.get('SubnetBaseInfo') is not None:
+            temp_model = GetNetworkInterfaceResponseBodyContentSubnetBaseInfo()
+            self.subnet_base_info = temp_model.from_map(m['SubnetBaseInfo'])
+        if m.get('TenantId') is not None:
+            self.tenant_id = m.get('TenantId')
+        if m.get('VpdBaseInfo') is not None:
+            temp_model = GetNetworkInterfaceResponseBodyContentVpdBaseInfo()
+            self.vpd_base_info = temp_model.from_map(m['VpdBaseInfo'])
+        if m.get('ZoneId') is not None:
+            self.zone_id = m.get('ZoneId')
+        return self
+
+
+class GetNetworkInterfaceResponseBody(TeaModel):
+    def __init__(
+        self,
+        code: int = None,
+        content: GetNetworkInterfaceResponseBodyContent = None,
+        message: str = None,
+        request_id: str = None,
+    ):
+        self.code = code
+        self.content = content
+        self.message = message
+        self.request_id = request_id
+
+    def validate(self):
+        if self.content:
+            self.content.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.content is not None:
+            result['Content'] = self.content.to_map()
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Content') is not None:
+            temp_model = GetNetworkInterfaceResponseBodyContent()
+            self.content = temp_model.from_map(m['Content'])
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class GetNetworkInterfaceResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: GetNetworkInterfaceResponseBody = None,
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
+            temp_model = GetNetworkInterfaceResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class GetSubnetRequest(TeaModel):
     def __init__(
         self,
-        client_token: str = None,
         region_id: str = None,
         subnet_id: str = None,
         vpd_id: str = None,
     ):
-        self.client_token = client_token
         self.region_id = region_id
         self.subnet_id = subnet_id
         self.vpd_id = vpd_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.client_token is not None:
-            result['ClientToken'] = self.client_token
         if self.region_id is not None:
             result['RegionId'] = self.region_id
         if self.subnet_id is not None:
             result['SubnetId'] = self.subnet_id
         if self.vpd_id is not None:
             result['VpdId'] = self.vpd_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ClientToken') is not None:
-            self.client_token = m.get('ClientToken')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
         if m.get('SubnetId') is not None:
             self.subnet_id = m.get('SubnetId')
         if m.get('VpdId') is not None:
             self.vpd_id = m.get('VpdId')
         return self
@@ -2005,15 +5233,14 @@
 
 class GetSubnetResponseBodyContent(TeaModel):
     def __init__(
         self,
         available_ips: int = None,
         cidr: str = None,
         create_time: str = None,
-        description: str = None,
         gmt_modified: str = None,
         lb_count: int = None,
         message: str = None,
         nc_count: int = None,
         region_id: str = None,
         resource_group_id: str = None,
         status: str = None,
@@ -2025,15 +5252,14 @@
         vpd_base_info: GetSubnetResponseBodyContentVpdBaseInfo = None,
         vpd_id: str = None,
         zone_id: str = None,
     ):
         self.available_ips = available_ips
         self.cidr = cidr
         self.create_time = create_time
-        self.description = description
         self.gmt_modified = gmt_modified
         self.lb_count = lb_count
         self.message = message
         self.nc_count = nc_count
         self.region_id = region_id
         self.resource_group_id = resource_group_id
         self.status = status
@@ -2062,16 +5288,14 @@
         result = dict()
         if self.available_ips is not None:
             result['AvailableIps'] = self.available_ips
         if self.cidr is not None:
             result['Cidr'] = self.cidr
         if self.create_time is not None:
             result['CreateTime'] = self.create_time
-        if self.description is not None:
-            result['Description'] = self.description
         if self.gmt_modified is not None:
             result['GmtModified'] = self.gmt_modified
         if self.lb_count is not None:
             result['LbCount'] = self.lb_count
         if self.message is not None:
             result['Message'] = self.message
         if self.nc_count is not None:
@@ -2106,16 +5330,14 @@
         m = m or dict()
         if m.get('AvailableIps') is not None:
             self.available_ips = m.get('AvailableIps')
         if m.get('Cidr') is not None:
             self.cidr = m.get('Cidr')
         if m.get('CreateTime') is not None:
             self.create_time = m.get('CreateTime')
-        if m.get('Description') is not None:
-            self.description = m.get('Description')
         if m.get('GmtModified') is not None:
             self.gmt_modified = m.get('GmtModified')
         if m.get('LbCount') is not None:
             self.lb_count = m.get('LbCount')
         if m.get('Message') is not None:
             self.message = m.get('Message')
         if m.get('NcCount') is not None:
@@ -2968,46 +6190,474 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = GetVccResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class GetVccGrantRuleRequest(TeaModel):
+    def __init__(
+        self,
+        er_id: str = None,
+        grant_rule_id: str = None,
+        grant_tenant_id: str = None,
+        instance_id: str = None,
+        region_id: str = None,
+    ):
+        self.er_id = er_id
+        self.grant_rule_id = grant_rule_id
+        self.grant_tenant_id = grant_tenant_id
+        self.instance_id = instance_id
+        self.region_id = region_id
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
+        if self.er_id is not None:
+            result['ErId'] = self.er_id
+        if self.grant_rule_id is not None:
+            result['GrantRuleId'] = self.grant_rule_id
+        if self.grant_tenant_id is not None:
+            result['GrantTenantId'] = self.grant_tenant_id
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ErId') is not None:
+            self.er_id = m.get('ErId')
+        if m.get('GrantRuleId') is not None:
+            self.grant_rule_id = m.get('GrantRuleId')
+        if m.get('GrantTenantId') is not None:
+            self.grant_tenant_id = m.get('GrantTenantId')
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        return self
+
+
+class GetVccGrantRuleResponseBodyContent(TeaModel):
+    def __init__(
+        self,
+        create_time: str = None,
+        er_id: str = None,
+        grant_rule_id: str = None,
+        grant_tenant_id: str = None,
+        instance_id: str = None,
+        instance_name: str = None,
+        product: str = None,
+        region_id: str = None,
+        tenant_id: str = None,
+        used: bool = None,
+    ):
+        self.create_time = create_time
+        self.er_id = er_id
+        self.grant_rule_id = grant_rule_id
+        self.grant_tenant_id = grant_tenant_id
+        self.instance_id = instance_id
+        self.instance_name = instance_name
+        self.product = product
+        self.region_id = region_id
+        self.tenant_id = tenant_id
+        self.used = used
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
+        if self.create_time is not None:
+            result['CreateTime'] = self.create_time
+        if self.er_id is not None:
+            result['ErId'] = self.er_id
+        if self.grant_rule_id is not None:
+            result['GrantRuleId'] = self.grant_rule_id
+        if self.grant_tenant_id is not None:
+            result['GrantTenantId'] = self.grant_tenant_id
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.instance_name is not None:
+            result['InstanceName'] = self.instance_name
+        if self.product is not None:
+            result['Product'] = self.product
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.tenant_id is not None:
+            result['TenantId'] = self.tenant_id
+        if self.used is not None:
+            result['Used'] = self.used
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('CreateTime') is not None:
+            self.create_time = m.get('CreateTime')
+        if m.get('ErId') is not None:
+            self.er_id = m.get('ErId')
+        if m.get('GrantRuleId') is not None:
+            self.grant_rule_id = m.get('GrantRuleId')
+        if m.get('GrantTenantId') is not None:
+            self.grant_tenant_id = m.get('GrantTenantId')
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('InstanceName') is not None:
+            self.instance_name = m.get('InstanceName')
+        if m.get('Product') is not None:
+            self.product = m.get('Product')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('TenantId') is not None:
+            self.tenant_id = m.get('TenantId')
+        if m.get('Used') is not None:
+            self.used = m.get('Used')
+        return self
+
+
+class GetVccGrantRuleResponseBody(TeaModel):
+    def __init__(
+        self,
+        code: int = None,
+        content: GetVccGrantRuleResponseBodyContent = None,
+        message: str = None,
+        request_id: str = None,
+    ):
+        self.code = code
+        self.content = content
+        self.message = message
+        self.request_id = request_id
+
+    def validate(self):
+        if self.content:
+            self.content.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.content is not None:
+            result['Content'] = self.content.to_map()
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Content') is not None:
+            temp_model = GetVccGrantRuleResponseBodyContent()
+            self.content = temp_model.from_map(m['Content'])
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class GetVccGrantRuleResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: GetVccGrantRuleResponseBody = None,
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
+            temp_model = GetVccGrantRuleResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class GetVccRouteEntryRequest(TeaModel):
+    def __init__(
+        self,
+        region_id: str = None,
+        vcc_id: str = None,
+        vcc_route_entry_id: str = None,
+    ):
+        self.region_id = region_id
+        self.vcc_id = vcc_id
+        self.vcc_route_entry_id = vcc_route_entry_id
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
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.vcc_id is not None:
+            result['VccId'] = self.vcc_id
+        if self.vcc_route_entry_id is not None:
+            result['VccRouteEntryId'] = self.vcc_route_entry_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('VccId') is not None:
+            self.vcc_id = m.get('VccId')
+        if m.get('VccRouteEntryId') is not None:
+            self.vcc_route_entry_id = m.get('VccRouteEntryId')
+        return self
+
+
+class GetVccRouteEntryResponseBodyContent(TeaModel):
+    def __init__(
+        self,
+        destination_cidr_block: str = None,
+        gmt_modified: str = None,
+        next_hop_id: str = None,
+        next_hop_type: str = None,
+        region_id: str = None,
+        route_type: str = None,
+        status: str = None,
+        tenant_id: str = None,
+        vcc_id: str = None,
+        vcc_route_entry_id: str = None,
+    ):
+        self.destination_cidr_block = destination_cidr_block
+        self.gmt_modified = gmt_modified
+        self.next_hop_id = next_hop_id
+        self.next_hop_type = next_hop_type
+        self.region_id = region_id
+        self.route_type = route_type
+        self.status = status
+        self.tenant_id = tenant_id
+        self.vcc_id = vcc_id
+        self.vcc_route_entry_id = vcc_route_entry_id
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
+        if self.destination_cidr_block is not None:
+            result['DestinationCidrBlock'] = self.destination_cidr_block
+        if self.gmt_modified is not None:
+            result['GmtModified'] = self.gmt_modified
+        if self.next_hop_id is not None:
+            result['NextHopId'] = self.next_hop_id
+        if self.next_hop_type is not None:
+            result['NextHopType'] = self.next_hop_type
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.route_type is not None:
+            result['RouteType'] = self.route_type
+        if self.status is not None:
+            result['Status'] = self.status
+        if self.tenant_id is not None:
+            result['TenantId'] = self.tenant_id
+        if self.vcc_id is not None:
+            result['VccId'] = self.vcc_id
+        if self.vcc_route_entry_id is not None:
+            result['VccRouteEntryId'] = self.vcc_route_entry_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('DestinationCidrBlock') is not None:
+            self.destination_cidr_block = m.get('DestinationCidrBlock')
+        if m.get('GmtModified') is not None:
+            self.gmt_modified = m.get('GmtModified')
+        if m.get('NextHopId') is not None:
+            self.next_hop_id = m.get('NextHopId')
+        if m.get('NextHopType') is not None:
+            self.next_hop_type = m.get('NextHopType')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('RouteType') is not None:
+            self.route_type = m.get('RouteType')
+        if m.get('Status') is not None:
+            self.status = m.get('Status')
+        if m.get('TenantId') is not None:
+            self.tenant_id = m.get('TenantId')
+        if m.get('VccId') is not None:
+            self.vcc_id = m.get('VccId')
+        if m.get('VccRouteEntryId') is not None:
+            self.vcc_route_entry_id = m.get('VccRouteEntryId')
+        return self
+
+
+class GetVccRouteEntryResponseBody(TeaModel):
+    def __init__(
+        self,
+        code: int = None,
+        content: GetVccRouteEntryResponseBodyContent = None,
+        message: str = None,
+        request_id: str = None,
+    ):
+        self.code = code
+        self.content = content
+        self.message = message
+        self.request_id = request_id
+
+    def validate(self):
+        if self.content:
+            self.content.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.content is not None:
+            result['Content'] = self.content.to_map()
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Content') is not None:
+            temp_model = GetVccRouteEntryResponseBodyContent()
+            self.content = temp_model.from_map(m['Content'])
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class GetVccRouteEntryResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: GetVccRouteEntryResponseBody = None,
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
+            temp_model = GetVccRouteEntryResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class GetVpdRequest(TeaModel):
     def __init__(
         self,
-        client_token: str = None,
         region_id: str = None,
         vpd_id: str = None,
     ):
-        self.client_token = client_token
         self.region_id = region_id
         self.vpd_id = vpd_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.client_token is not None:
-            result['ClientToken'] = self.client_token
         if self.region_id is not None:
             result['RegionId'] = self.region_id
         if self.vpd_id is not None:
             result['VpdId'] = self.vpd_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ClientToken') is not None:
-            self.client_token = m.get('ClientToken')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
         if m.get('VpdId') is not None:
             self.vpd_id = m.get('VpdId')
         return self
 
 
@@ -3358,14 +7008,448 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = GetVpdResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class GetVpdGrantRuleRequest(TeaModel):
+    def __init__(
+        self,
+        er_id: str = None,
+        grant_rule_id: str = None,
+        grant_tenant_id: str = None,
+        instance_id: str = None,
+        region_id: str = None,
+    ):
+        self.er_id = er_id
+        self.grant_rule_id = grant_rule_id
+        self.grant_tenant_id = grant_tenant_id
+        self.instance_id = instance_id
+        self.region_id = region_id
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
+        if self.er_id is not None:
+            result['ErId'] = self.er_id
+        if self.grant_rule_id is not None:
+            result['GrantRuleId'] = self.grant_rule_id
+        if self.grant_tenant_id is not None:
+            result['GrantTenantId'] = self.grant_tenant_id
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ErId') is not None:
+            self.er_id = m.get('ErId')
+        if m.get('GrantRuleId') is not None:
+            self.grant_rule_id = m.get('GrantRuleId')
+        if m.get('GrantTenantId') is not None:
+            self.grant_tenant_id = m.get('GrantTenantId')
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        return self
+
+
+class GetVpdGrantRuleResponseBodyContent(TeaModel):
+    def __init__(
+        self,
+        create_time: str = None,
+        er_id: str = None,
+        grant_rule_id: str = None,
+        grant_tenant_id: str = None,
+        instance_id: str = None,
+        instance_name: str = None,
+        product: str = None,
+        region_id: str = None,
+        tenant_id: str = None,
+        used: bool = None,
+    ):
+        self.create_time = create_time
+        self.er_id = er_id
+        self.grant_rule_id = grant_rule_id
+        self.grant_tenant_id = grant_tenant_id
+        self.instance_id = instance_id
+        self.instance_name = instance_name
+        self.product = product
+        self.region_id = region_id
+        self.tenant_id = tenant_id
+        self.used = used
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
+        if self.create_time is not None:
+            result['CreateTime'] = self.create_time
+        if self.er_id is not None:
+            result['ErId'] = self.er_id
+        if self.grant_rule_id is not None:
+            result['GrantRuleId'] = self.grant_rule_id
+        if self.grant_tenant_id is not None:
+            result['GrantTenantId'] = self.grant_tenant_id
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.instance_name is not None:
+            result['InstanceName'] = self.instance_name
+        if self.product is not None:
+            result['Product'] = self.product
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.tenant_id is not None:
+            result['TenantId'] = self.tenant_id
+        if self.used is not None:
+            result['Used'] = self.used
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('CreateTime') is not None:
+            self.create_time = m.get('CreateTime')
+        if m.get('ErId') is not None:
+            self.er_id = m.get('ErId')
+        if m.get('GrantRuleId') is not None:
+            self.grant_rule_id = m.get('GrantRuleId')
+        if m.get('GrantTenantId') is not None:
+            self.grant_tenant_id = m.get('GrantTenantId')
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('InstanceName') is not None:
+            self.instance_name = m.get('InstanceName')
+        if m.get('Product') is not None:
+            self.product = m.get('Product')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('TenantId') is not None:
+            self.tenant_id = m.get('TenantId')
+        if m.get('Used') is not None:
+            self.used = m.get('Used')
+        return self
+
+
+class GetVpdGrantRuleResponseBody(TeaModel):
+    def __init__(
+        self,
+        code: int = None,
+        content: GetVpdGrantRuleResponseBodyContent = None,
+        message: str = None,
+        request_id: str = None,
+    ):
+        self.code = code
+        self.content = content
+        self.message = message
+        self.request_id = request_id
+
+    def validate(self):
+        if self.content:
+            self.content.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.content is not None:
+            result['Content'] = self.content.to_map()
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Content') is not None:
+            temp_model = GetVpdGrantRuleResponseBodyContent()
+            self.content = temp_model.from_map(m['Content'])
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class GetVpdGrantRuleResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: GetVpdGrantRuleResponseBody = None,
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
+            temp_model = GetVpdGrantRuleResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class GetVpdRouteEntryRequest(TeaModel):
+    def __init__(
+        self,
+        region_id: str = None,
+        vpd_id: str = None,
+        vpd_route_entry_id: str = None,
+    ):
+        self.region_id = region_id
+        self.vpd_id = vpd_id
+        self.vpd_route_entry_id = vpd_route_entry_id
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
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.vpd_id is not None:
+            result['VpdId'] = self.vpd_id
+        if self.vpd_route_entry_id is not None:
+            result['VpdRouteEntryId'] = self.vpd_route_entry_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('VpdId') is not None:
+            self.vpd_id = m.get('VpdId')
+        if m.get('VpdRouteEntryId') is not None:
+            self.vpd_route_entry_id = m.get('VpdRouteEntryId')
+        return self
+
+
+class GetVpdRouteEntryResponseBodyContent(TeaModel):
+    def __init__(
+        self,
+        destination_cidr_block: str = None,
+        gmt_modified: str = None,
+        next_hop_id: str = None,
+        next_hop_type: str = None,
+        region_id: str = None,
+        route_type: str = None,
+        status: str = None,
+        tenant_id: str = None,
+        vpd_id: str = None,
+        vpd_route_entry_id: str = None,
+    ):
+        self.destination_cidr_block = destination_cidr_block
+        self.gmt_modified = gmt_modified
+        self.next_hop_id = next_hop_id
+        self.next_hop_type = next_hop_type
+        self.region_id = region_id
+        self.route_type = route_type
+        self.status = status
+        self.tenant_id = tenant_id
+        self.vpd_id = vpd_id
+        self.vpd_route_entry_id = vpd_route_entry_id
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
+        if self.destination_cidr_block is not None:
+            result['DestinationCidrBlock'] = self.destination_cidr_block
+        if self.gmt_modified is not None:
+            result['GmtModified'] = self.gmt_modified
+        if self.next_hop_id is not None:
+            result['NextHopId'] = self.next_hop_id
+        if self.next_hop_type is not None:
+            result['NextHopType'] = self.next_hop_type
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.route_type is not None:
+            result['RouteType'] = self.route_type
+        if self.status is not None:
+            result['Status'] = self.status
+        if self.tenant_id is not None:
+            result['TenantId'] = self.tenant_id
+        if self.vpd_id is not None:
+            result['VpdId'] = self.vpd_id
+        if self.vpd_route_entry_id is not None:
+            result['VpdRouteEntryId'] = self.vpd_route_entry_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('DestinationCidrBlock') is not None:
+            self.destination_cidr_block = m.get('DestinationCidrBlock')
+        if m.get('GmtModified') is not None:
+            self.gmt_modified = m.get('GmtModified')
+        if m.get('NextHopId') is not None:
+            self.next_hop_id = m.get('NextHopId')
+        if m.get('NextHopType') is not None:
+            self.next_hop_type = m.get('NextHopType')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('RouteType') is not None:
+            self.route_type = m.get('RouteType')
+        if m.get('Status') is not None:
+            self.status = m.get('Status')
+        if m.get('TenantId') is not None:
+            self.tenant_id = m.get('TenantId')
+        if m.get('VpdId') is not None:
+            self.vpd_id = m.get('VpdId')
+        if m.get('VpdRouteEntryId') is not None:
+            self.vpd_route_entry_id = m.get('VpdRouteEntryId')
+        return self
+
+
+class GetVpdRouteEntryResponseBody(TeaModel):
+    def __init__(
+        self,
+        code: int = None,
+        content: GetVpdRouteEntryResponseBodyContent = None,
+        message: str = None,
+        request_id: str = None,
+    ):
+        self.code = code
+        self.content = content
+        self.message = message
+        self.request_id = request_id
+
+    def validate(self):
+        if self.content:
+            self.content.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.content is not None:
+            result['Content'] = self.content.to_map()
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Content') is not None:
+            temp_model = GetVpdRouteEntryResponseBodyContent()
+            self.content = temp_model.from_map(m['Content'])
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class GetVpdRouteEntryResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: GetVpdRouteEntryResponseBody = None,
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
+            temp_model = GetVpdRouteEntryResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class InitializeVccRequest(TeaModel):
     def __init__(
         self,
         resource_group_id: str = None,
     ):
         self.resource_group_id = resource_group_id
 
@@ -3509,14 +7593,1340 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = InitializeVccResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class ListErAttachmentsRequest(TeaModel):
+    def __init__(
+        self,
+        auto_receive_all_route: bool = None,
+        enable_page: bool = None,
+        er_attachment_id: str = None,
+        er_attachment_name: str = None,
+        er_id: str = None,
+        instance_id: str = None,
+        instance_type: str = None,
+        page_number: int = None,
+        page_size: int = None,
+        region_id: str = None,
+        resource_tenant_id: str = None,
+        status: str = None,
+    ):
+        self.auto_receive_all_route = auto_receive_all_route
+        self.enable_page = enable_page
+        self.er_attachment_id = er_attachment_id
+        self.er_attachment_name = er_attachment_name
+        self.er_id = er_id
+        self.instance_id = instance_id
+        self.instance_type = instance_type
+        self.page_number = page_number
+        self.page_size = page_size
+        self.region_id = region_id
+        self.resource_tenant_id = resource_tenant_id
+        self.status = status
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
+        if self.auto_receive_all_route is not None:
+            result['AutoReceiveAllRoute'] = self.auto_receive_all_route
+        if self.enable_page is not None:
+            result['EnablePage'] = self.enable_page
+        if self.er_attachment_id is not None:
+            result['ErAttachmentId'] = self.er_attachment_id
+        if self.er_attachment_name is not None:
+            result['ErAttachmentName'] = self.er_attachment_name
+        if self.er_id is not None:
+            result['ErId'] = self.er_id
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.instance_type is not None:
+            result['InstanceType'] = self.instance_type
+        if self.page_number is not None:
+            result['PageNumber'] = self.page_number
+        if self.page_size is not None:
+            result['PageSize'] = self.page_size
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.resource_tenant_id is not None:
+            result['ResourceTenantId'] = self.resource_tenant_id
+        if self.status is not None:
+            result['Status'] = self.status
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('AutoReceiveAllRoute') is not None:
+            self.auto_receive_all_route = m.get('AutoReceiveAllRoute')
+        if m.get('EnablePage') is not None:
+            self.enable_page = m.get('EnablePage')
+        if m.get('ErAttachmentId') is not None:
+            self.er_attachment_id = m.get('ErAttachmentId')
+        if m.get('ErAttachmentName') is not None:
+            self.er_attachment_name = m.get('ErAttachmentName')
+        if m.get('ErId') is not None:
+            self.er_id = m.get('ErId')
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('InstanceType') is not None:
+            self.instance_type = m.get('InstanceType')
+        if m.get('PageNumber') is not None:
+            self.page_number = m.get('PageNumber')
+        if m.get('PageSize') is not None:
+            self.page_size = m.get('PageSize')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('ResourceTenantId') is not None:
+            self.resource_tenant_id = m.get('ResourceTenantId')
+        if m.get('Status') is not None:
+            self.status = m.get('Status')
+        return self
+
+
+class ListErAttachmentsResponseBodyContentData(TeaModel):
+    def __init__(
+        self,
+        across: bool = None,
+        auto_receive_all_route: bool = None,
+        create_time: str = None,
+        er_attachment_id: str = None,
+        er_attachment_name: str = None,
+        er_id: str = None,
+        gmt_modified: str = None,
+        instance_id: str = None,
+        instance_name: str = None,
+        instance_type: str = None,
+        message: str = None,
+        region_id: str = None,
+        resource_tenant_id: str = None,
+        status: str = None,
+        tenant_id: str = None,
+    ):
+        self.across = across
+        self.auto_receive_all_route = auto_receive_all_route
+        self.create_time = create_time
+        self.er_attachment_id = er_attachment_id
+        self.er_attachment_name = er_attachment_name
+        self.er_id = er_id
+        self.gmt_modified = gmt_modified
+        self.instance_id = instance_id
+        self.instance_name = instance_name
+        self.instance_type = instance_type
+        self.message = message
+        self.region_id = region_id
+        self.resource_tenant_id = resource_tenant_id
+        self.status = status
+        self.tenant_id = tenant_id
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
+        if self.across is not None:
+            result['Across'] = self.across
+        if self.auto_receive_all_route is not None:
+            result['AutoReceiveAllRoute'] = self.auto_receive_all_route
+        if self.create_time is not None:
+            result['CreateTime'] = self.create_time
+        if self.er_attachment_id is not None:
+            result['ErAttachmentId'] = self.er_attachment_id
+        if self.er_attachment_name is not None:
+            result['ErAttachmentName'] = self.er_attachment_name
+        if self.er_id is not None:
+            result['ErId'] = self.er_id
+        if self.gmt_modified is not None:
+            result['GmtModified'] = self.gmt_modified
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.instance_name is not None:
+            result['InstanceName'] = self.instance_name
+        if self.instance_type is not None:
+            result['InstanceType'] = self.instance_type
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.resource_tenant_id is not None:
+            result['ResourceTenantId'] = self.resource_tenant_id
+        if self.status is not None:
+            result['Status'] = self.status
+        if self.tenant_id is not None:
+            result['TenantId'] = self.tenant_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Across') is not None:
+            self.across = m.get('Across')
+        if m.get('AutoReceiveAllRoute') is not None:
+            self.auto_receive_all_route = m.get('AutoReceiveAllRoute')
+        if m.get('CreateTime') is not None:
+            self.create_time = m.get('CreateTime')
+        if m.get('ErAttachmentId') is not None:
+            self.er_attachment_id = m.get('ErAttachmentId')
+        if m.get('ErAttachmentName') is not None:
+            self.er_attachment_name = m.get('ErAttachmentName')
+        if m.get('ErId') is not None:
+            self.er_id = m.get('ErId')
+        if m.get('GmtModified') is not None:
+            self.gmt_modified = m.get('GmtModified')
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('InstanceName') is not None:
+            self.instance_name = m.get('InstanceName')
+        if m.get('InstanceType') is not None:
+            self.instance_type = m.get('InstanceType')
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('ResourceTenantId') is not None:
+            self.resource_tenant_id = m.get('ResourceTenantId')
+        if m.get('Status') is not None:
+            self.status = m.get('Status')
+        if m.get('TenantId') is not None:
+            self.tenant_id = m.get('TenantId')
+        return self
+
+
+class ListErAttachmentsResponseBodyContent(TeaModel):
+    def __init__(
+        self,
+        data: List[ListErAttachmentsResponseBodyContentData] = None,
+        total: int = None,
+    ):
+        self.data = data
+        self.total = total
+
+    def validate(self):
+        if self.data:
+            for k in self.data:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['Data'] = []
+        if self.data is not None:
+            for k in self.data:
+                result['Data'].append(k.to_map() if k else None)
+        if self.total is not None:
+            result['Total'] = self.total
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.data = []
+        if m.get('Data') is not None:
+            for k in m.get('Data'):
+                temp_model = ListErAttachmentsResponseBodyContentData()
+                self.data.append(temp_model.from_map(k))
+        if m.get('Total') is not None:
+            self.total = m.get('Total')
+        return self
+
+
+class ListErAttachmentsResponseBody(TeaModel):
+    def __init__(
+        self,
+        code: int = None,
+        content: ListErAttachmentsResponseBodyContent = None,
+        message: str = None,
+        request_id: str = None,
+    ):
+        self.code = code
+        self.content = content
+        self.message = message
+        self.request_id = request_id
+
+    def validate(self):
+        if self.content:
+            self.content.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.content is not None:
+            result['Content'] = self.content.to_map()
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Content') is not None:
+            temp_model = ListErAttachmentsResponseBodyContent()
+            self.content = temp_model.from_map(m['Content'])
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class ListErAttachmentsResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: ListErAttachmentsResponseBody = None,
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
+            temp_model = ListErAttachmentsResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class ListErRouteEntriesRequest(TeaModel):
+    def __init__(
+        self,
+        destination_cidr_block: str = None,
+        enable_page: bool = None,
+        er_id: str = None,
+        instance_id: str = None,
+        next_hop_id: str = None,
+        next_hop_type: str = None,
+        page_number: int = None,
+        page_size: int = None,
+        region_id: str = None,
+        route_type: str = None,
+        status: str = None,
+    ):
+        self.destination_cidr_block = destination_cidr_block
+        self.enable_page = enable_page
+        self.er_id = er_id
+        self.instance_id = instance_id
+        self.next_hop_id = next_hop_id
+        self.next_hop_type = next_hop_type
+        self.page_number = page_number
+        self.page_size = page_size
+        self.region_id = region_id
+        self.route_type = route_type
+        self.status = status
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
+        if self.destination_cidr_block is not None:
+            result['DestinationCidrBlock'] = self.destination_cidr_block
+        if self.enable_page is not None:
+            result['EnablePage'] = self.enable_page
+        if self.er_id is not None:
+            result['ErId'] = self.er_id
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.next_hop_id is not None:
+            result['NextHopId'] = self.next_hop_id
+        if self.next_hop_type is not None:
+            result['NextHopType'] = self.next_hop_type
+        if self.page_number is not None:
+            result['PageNumber'] = self.page_number
+        if self.page_size is not None:
+            result['PageSize'] = self.page_size
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.route_type is not None:
+            result['RouteType'] = self.route_type
+        if self.status is not None:
+            result['Status'] = self.status
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('DestinationCidrBlock') is not None:
+            self.destination_cidr_block = m.get('DestinationCidrBlock')
+        if m.get('EnablePage') is not None:
+            self.enable_page = m.get('EnablePage')
+        if m.get('ErId') is not None:
+            self.er_id = m.get('ErId')
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('NextHopId') is not None:
+            self.next_hop_id = m.get('NextHopId')
+        if m.get('NextHopType') is not None:
+            self.next_hop_type = m.get('NextHopType')
+        if m.get('PageNumber') is not None:
+            self.page_number = m.get('PageNumber')
+        if m.get('PageSize') is not None:
+            self.page_size = m.get('PageSize')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('RouteType') is not None:
+            self.route_type = m.get('RouteType')
+        if m.get('Status') is not None:
+            self.status = m.get('Status')
+        return self
+
+
+class ListErRouteEntriesResponseBodyContentData(TeaModel):
+    def __init__(
+        self,
+        destination_cidr_block: str = None,
+        er_id: str = None,
+        er_route_entry_id: str = None,
+        gmt_modified: str = None,
+        next_hop_id: str = None,
+        next_hop_type: str = None,
+        region_id: str = None,
+        resource_tenant_id: str = None,
+        route_type: str = None,
+        status: str = None,
+        tenant_id: str = None,
+    ):
+        self.destination_cidr_block = destination_cidr_block
+        self.er_id = er_id
+        self.er_route_entry_id = er_route_entry_id
+        self.gmt_modified = gmt_modified
+        self.next_hop_id = next_hop_id
+        self.next_hop_type = next_hop_type
+        self.region_id = region_id
+        self.resource_tenant_id = resource_tenant_id
+        self.route_type = route_type
+        self.status = status
+        self.tenant_id = tenant_id
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
+        if self.destination_cidr_block is not None:
+            result['DestinationCidrBlock'] = self.destination_cidr_block
+        if self.er_id is not None:
+            result['ErId'] = self.er_id
+        if self.er_route_entry_id is not None:
+            result['ErRouteEntryId'] = self.er_route_entry_id
+        if self.gmt_modified is not None:
+            result['GmtModified'] = self.gmt_modified
+        if self.next_hop_id is not None:
+            result['NextHopId'] = self.next_hop_id
+        if self.next_hop_type is not None:
+            result['NextHopType'] = self.next_hop_type
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.resource_tenant_id is not None:
+            result['ResourceTenantId'] = self.resource_tenant_id
+        if self.route_type is not None:
+            result['RouteType'] = self.route_type
+        if self.status is not None:
+            result['Status'] = self.status
+        if self.tenant_id is not None:
+            result['TenantId'] = self.tenant_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('DestinationCidrBlock') is not None:
+            self.destination_cidr_block = m.get('DestinationCidrBlock')
+        if m.get('ErId') is not None:
+            self.er_id = m.get('ErId')
+        if m.get('ErRouteEntryId') is not None:
+            self.er_route_entry_id = m.get('ErRouteEntryId')
+        if m.get('GmtModified') is not None:
+            self.gmt_modified = m.get('GmtModified')
+        if m.get('NextHopId') is not None:
+            self.next_hop_id = m.get('NextHopId')
+        if m.get('NextHopType') is not None:
+            self.next_hop_type = m.get('NextHopType')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('ResourceTenantId') is not None:
+            self.resource_tenant_id = m.get('ResourceTenantId')
+        if m.get('RouteType') is not None:
+            self.route_type = m.get('RouteType')
+        if m.get('Status') is not None:
+            self.status = m.get('Status')
+        if m.get('TenantId') is not None:
+            self.tenant_id = m.get('TenantId')
+        return self
+
+
+class ListErRouteEntriesResponseBodyContent(TeaModel):
+    def __init__(
+        self,
+        data: List[ListErRouteEntriesResponseBodyContentData] = None,
+        total: int = None,
+    ):
+        self.data = data
+        self.total = total
+
+    def validate(self):
+        if self.data:
+            for k in self.data:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['Data'] = []
+        if self.data is not None:
+            for k in self.data:
+                result['Data'].append(k.to_map() if k else None)
+        if self.total is not None:
+            result['Total'] = self.total
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.data = []
+        if m.get('Data') is not None:
+            for k in m.get('Data'):
+                temp_model = ListErRouteEntriesResponseBodyContentData()
+                self.data.append(temp_model.from_map(k))
+        if m.get('Total') is not None:
+            self.total = m.get('Total')
+        return self
+
+
+class ListErRouteEntriesResponseBody(TeaModel):
+    def __init__(
+        self,
+        code: int = None,
+        content: ListErRouteEntriesResponseBodyContent = None,
+        message: str = None,
+        request_id: str = None,
+    ):
+        self.code = code
+        self.content = content
+        self.message = message
+        self.request_id = request_id
+
+    def validate(self):
+        if self.content:
+            self.content.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.content is not None:
+            result['Content'] = self.content.to_map()
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Content') is not None:
+            temp_model = ListErRouteEntriesResponseBodyContent()
+            self.content = temp_model.from_map(m['Content'])
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class ListErRouteEntriesResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: ListErRouteEntriesResponseBody = None,
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
+            temp_model = ListErRouteEntriesResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class ListErRouteMapsRequest(TeaModel):
+    def __init__(
+        self,
+        destination_cidr_block: str = None,
+        enable_page: bool = None,
+        er_id: str = None,
+        er_route_map_id: str = None,
+        er_route_map_num: int = None,
+        page_number: int = None,
+        page_size: int = None,
+        reception_instance_id: str = None,
+        reception_instance_name: str = None,
+        reception_instance_type: str = None,
+        region_id: str = None,
+        route_map_action: str = None,
+        transmission_instance_id: str = None,
+        transmission_instance_name: str = None,
+        transmission_instance_type: str = None,
+    ):
+        self.destination_cidr_block = destination_cidr_block
+        self.enable_page = enable_page
+        self.er_id = er_id
+        self.er_route_map_id = er_route_map_id
+        self.er_route_map_num = er_route_map_num
+        self.page_number = page_number
+        self.page_size = page_size
+        self.reception_instance_id = reception_instance_id
+        self.reception_instance_name = reception_instance_name
+        self.reception_instance_type = reception_instance_type
+        self.region_id = region_id
+        self.route_map_action = route_map_action
+        self.transmission_instance_id = transmission_instance_id
+        self.transmission_instance_name = transmission_instance_name
+        self.transmission_instance_type = transmission_instance_type
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
+        if self.destination_cidr_block is not None:
+            result['DestinationCidrBlock'] = self.destination_cidr_block
+        if self.enable_page is not None:
+            result['EnablePage'] = self.enable_page
+        if self.er_id is not None:
+            result['ErId'] = self.er_id
+        if self.er_route_map_id is not None:
+            result['ErRouteMapId'] = self.er_route_map_id
+        if self.er_route_map_num is not None:
+            result['ErRouteMapNum'] = self.er_route_map_num
+        if self.page_number is not None:
+            result['PageNumber'] = self.page_number
+        if self.page_size is not None:
+            result['PageSize'] = self.page_size
+        if self.reception_instance_id is not None:
+            result['ReceptionInstanceId'] = self.reception_instance_id
+        if self.reception_instance_name is not None:
+            result['ReceptionInstanceName'] = self.reception_instance_name
+        if self.reception_instance_type is not None:
+            result['ReceptionInstanceType'] = self.reception_instance_type
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.route_map_action is not None:
+            result['RouteMapAction'] = self.route_map_action
+        if self.transmission_instance_id is not None:
+            result['TransmissionInstanceId'] = self.transmission_instance_id
+        if self.transmission_instance_name is not None:
+            result['TransmissionInstanceName'] = self.transmission_instance_name
+        if self.transmission_instance_type is not None:
+            result['TransmissionInstanceType'] = self.transmission_instance_type
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('DestinationCidrBlock') is not None:
+            self.destination_cidr_block = m.get('DestinationCidrBlock')
+        if m.get('EnablePage') is not None:
+            self.enable_page = m.get('EnablePage')
+        if m.get('ErId') is not None:
+            self.er_id = m.get('ErId')
+        if m.get('ErRouteMapId') is not None:
+            self.er_route_map_id = m.get('ErRouteMapId')
+        if m.get('ErRouteMapNum') is not None:
+            self.er_route_map_num = m.get('ErRouteMapNum')
+        if m.get('PageNumber') is not None:
+            self.page_number = m.get('PageNumber')
+        if m.get('PageSize') is not None:
+            self.page_size = m.get('PageSize')
+        if m.get('ReceptionInstanceId') is not None:
+            self.reception_instance_id = m.get('ReceptionInstanceId')
+        if m.get('ReceptionInstanceName') is not None:
+            self.reception_instance_name = m.get('ReceptionInstanceName')
+        if m.get('ReceptionInstanceType') is not None:
+            self.reception_instance_type = m.get('ReceptionInstanceType')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('RouteMapAction') is not None:
+            self.route_map_action = m.get('RouteMapAction')
+        if m.get('TransmissionInstanceId') is not None:
+            self.transmission_instance_id = m.get('TransmissionInstanceId')
+        if m.get('TransmissionInstanceName') is not None:
+            self.transmission_instance_name = m.get('TransmissionInstanceName')
+        if m.get('TransmissionInstanceType') is not None:
+            self.transmission_instance_type = m.get('TransmissionInstanceType')
+        return self
+
+
+class ListErRouteMapsResponseBodyContentData(TeaModel):
+    def __init__(
+        self,
+        action: str = None,
+        create_time: str = None,
+        description: str = None,
+        destination_cidr_block: str = None,
+        er_id: str = None,
+        er_route_map_id: str = None,
+        gmt_modified: str = None,
+        message: str = None,
+        reception_instance_id: str = None,
+        reception_instance_name: str = None,
+        reception_instance_owner: str = None,
+        reception_instance_type: str = None,
+        region_id: str = None,
+        route_map_num: int = None,
+        status: str = None,
+        tenant_id: str = None,
+        transmission_instance_id: str = None,
+        transmission_instance_name: str = None,
+        transmission_instance_owner: str = None,
+        transmission_instance_type: str = None,
+    ):
+        self.action = action
+        self.create_time = create_time
+        self.description = description
+        self.destination_cidr_block = destination_cidr_block
+        self.er_id = er_id
+        self.er_route_map_id = er_route_map_id
+        self.gmt_modified = gmt_modified
+        self.message = message
+        self.reception_instance_id = reception_instance_id
+        self.reception_instance_name = reception_instance_name
+        self.reception_instance_owner = reception_instance_owner
+        self.reception_instance_type = reception_instance_type
+        self.region_id = region_id
+        self.route_map_num = route_map_num
+        self.status = status
+        self.tenant_id = tenant_id
+        self.transmission_instance_id = transmission_instance_id
+        self.transmission_instance_name = transmission_instance_name
+        self.transmission_instance_owner = transmission_instance_owner
+        self.transmission_instance_type = transmission_instance_type
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
+        if self.action is not None:
+            result['Action'] = self.action
+        if self.create_time is not None:
+            result['CreateTime'] = self.create_time
+        if self.description is not None:
+            result['Description'] = self.description
+        if self.destination_cidr_block is not None:
+            result['DestinationCidrBlock'] = self.destination_cidr_block
+        if self.er_id is not None:
+            result['ErId'] = self.er_id
+        if self.er_route_map_id is not None:
+            result['ErRouteMapId'] = self.er_route_map_id
+        if self.gmt_modified is not None:
+            result['GmtModified'] = self.gmt_modified
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.reception_instance_id is not None:
+            result['ReceptionInstanceId'] = self.reception_instance_id
+        if self.reception_instance_name is not None:
+            result['ReceptionInstanceName'] = self.reception_instance_name
+        if self.reception_instance_owner is not None:
+            result['ReceptionInstanceOwner'] = self.reception_instance_owner
+        if self.reception_instance_type is not None:
+            result['ReceptionInstanceType'] = self.reception_instance_type
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.route_map_num is not None:
+            result['RouteMapNum'] = self.route_map_num
+        if self.status is not None:
+            result['Status'] = self.status
+        if self.tenant_id is not None:
+            result['TenantId'] = self.tenant_id
+        if self.transmission_instance_id is not None:
+            result['TransmissionInstanceId'] = self.transmission_instance_id
+        if self.transmission_instance_name is not None:
+            result['TransmissionInstanceName'] = self.transmission_instance_name
+        if self.transmission_instance_owner is not None:
+            result['TransmissionInstanceOwner'] = self.transmission_instance_owner
+        if self.transmission_instance_type is not None:
+            result['TransmissionInstanceType'] = self.transmission_instance_type
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Action') is not None:
+            self.action = m.get('Action')
+        if m.get('CreateTime') is not None:
+            self.create_time = m.get('CreateTime')
+        if m.get('Description') is not None:
+            self.description = m.get('Description')
+        if m.get('DestinationCidrBlock') is not None:
+            self.destination_cidr_block = m.get('DestinationCidrBlock')
+        if m.get('ErId') is not None:
+            self.er_id = m.get('ErId')
+        if m.get('ErRouteMapId') is not None:
+            self.er_route_map_id = m.get('ErRouteMapId')
+        if m.get('GmtModified') is not None:
+            self.gmt_modified = m.get('GmtModified')
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('ReceptionInstanceId') is not None:
+            self.reception_instance_id = m.get('ReceptionInstanceId')
+        if m.get('ReceptionInstanceName') is not None:
+            self.reception_instance_name = m.get('ReceptionInstanceName')
+        if m.get('ReceptionInstanceOwner') is not None:
+            self.reception_instance_owner = m.get('ReceptionInstanceOwner')
+        if m.get('ReceptionInstanceType') is not None:
+            self.reception_instance_type = m.get('ReceptionInstanceType')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('RouteMapNum') is not None:
+            self.route_map_num = m.get('RouteMapNum')
+        if m.get('Status') is not None:
+            self.status = m.get('Status')
+        if m.get('TenantId') is not None:
+            self.tenant_id = m.get('TenantId')
+        if m.get('TransmissionInstanceId') is not None:
+            self.transmission_instance_id = m.get('TransmissionInstanceId')
+        if m.get('TransmissionInstanceName') is not None:
+            self.transmission_instance_name = m.get('TransmissionInstanceName')
+        if m.get('TransmissionInstanceOwner') is not None:
+            self.transmission_instance_owner = m.get('TransmissionInstanceOwner')
+        if m.get('TransmissionInstanceType') is not None:
+            self.transmission_instance_type = m.get('TransmissionInstanceType')
+        return self
+
+
+class ListErRouteMapsResponseBodyContent(TeaModel):
+    def __init__(
+        self,
+        data: List[ListErRouteMapsResponseBodyContentData] = None,
+        total: int = None,
+    ):
+        self.data = data
+        self.total = total
+
+    def validate(self):
+        if self.data:
+            for k in self.data:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['Data'] = []
+        if self.data is not None:
+            for k in self.data:
+                result['Data'].append(k.to_map() if k else None)
+        if self.total is not None:
+            result['Total'] = self.total
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.data = []
+        if m.get('Data') is not None:
+            for k in m.get('Data'):
+                temp_model = ListErRouteMapsResponseBodyContentData()
+                self.data.append(temp_model.from_map(k))
+        if m.get('Total') is not None:
+            self.total = m.get('Total')
+        return self
+
+
+class ListErRouteMapsResponseBody(TeaModel):
+    def __init__(
+        self,
+        code: int = None,
+        content: ListErRouteMapsResponseBodyContent = None,
+        message: str = None,
+        request_id: str = None,
+    ):
+        self.code = code
+        self.content = content
+        self.message = message
+        self.request_id = request_id
+
+    def validate(self):
+        if self.content:
+            self.content.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.content is not None:
+            result['Content'] = self.content.to_map()
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Content') is not None:
+            temp_model = ListErRouteMapsResponseBodyContent()
+            self.content = temp_model.from_map(m['Content'])
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class ListErRouteMapsResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: ListErRouteMapsResponseBody = None,
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
+            temp_model = ListErRouteMapsResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class ListErsRequest(TeaModel):
+    def __init__(
+        self,
+        enable_page: bool = None,
+        er_id: str = None,
+        er_name: str = None,
+        instance_id: str = None,
+        instance_type: str = None,
+        master_zone_id: str = None,
+        page_number: int = None,
+        page_size: int = None,
+        region_id: str = None,
+    ):
+        self.enable_page = enable_page
+        self.er_id = er_id
+        self.er_name = er_name
+        self.instance_id = instance_id
+        self.instance_type = instance_type
+        self.master_zone_id = master_zone_id
+        self.page_number = page_number
+        self.page_size = page_size
+        self.region_id = region_id
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
+        if self.enable_page is not None:
+            result['EnablePage'] = self.enable_page
+        if self.er_id is not None:
+            result['ErId'] = self.er_id
+        if self.er_name is not None:
+            result['ErName'] = self.er_name
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.instance_type is not None:
+            result['InstanceType'] = self.instance_type
+        if self.master_zone_id is not None:
+            result['MasterZoneId'] = self.master_zone_id
+        if self.page_number is not None:
+            result['PageNumber'] = self.page_number
+        if self.page_size is not None:
+            result['PageSize'] = self.page_size
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('EnablePage') is not None:
+            self.enable_page = m.get('EnablePage')
+        if m.get('ErId') is not None:
+            self.er_id = m.get('ErId')
+        if m.get('ErName') is not None:
+            self.er_name = m.get('ErName')
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('InstanceType') is not None:
+            self.instance_type = m.get('InstanceType')
+        if m.get('MasterZoneId') is not None:
+            self.master_zone_id = m.get('MasterZoneId')
+        if m.get('PageNumber') is not None:
+            self.page_number = m.get('PageNumber')
+        if m.get('PageSize') is not None:
+            self.page_size = m.get('PageSize')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        return self
+
+
+class ListErsResponseBodyContentData(TeaModel):
+    def __init__(
+        self,
+        connections: int = None,
+        create_time: str = None,
+        description: str = None,
+        er_id: str = None,
+        er_name: str = None,
+        gmt_modified: str = None,
+        master_zone_id: str = None,
+        message: str = None,
+        region_id: str = None,
+        route_maps: int = None,
+        status: str = None,
+        tenant_id: str = None,
+    ):
+        self.connections = connections
+        self.create_time = create_time
+        self.description = description
+        self.er_id = er_id
+        self.er_name = er_name
+        self.gmt_modified = gmt_modified
+        self.master_zone_id = master_zone_id
+        self.message = message
+        self.region_id = region_id
+        self.route_maps = route_maps
+        self.status = status
+        self.tenant_id = tenant_id
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
+        if self.connections is not None:
+            result['Connections'] = self.connections
+        if self.create_time is not None:
+            result['CreateTime'] = self.create_time
+        if self.description is not None:
+            result['Description'] = self.description
+        if self.er_id is not None:
+            result['ErId'] = self.er_id
+        if self.er_name is not None:
+            result['ErName'] = self.er_name
+        if self.gmt_modified is not None:
+            result['GmtModified'] = self.gmt_modified
+        if self.master_zone_id is not None:
+            result['MasterZoneId'] = self.master_zone_id
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.route_maps is not None:
+            result['RouteMaps'] = self.route_maps
+        if self.status is not None:
+            result['Status'] = self.status
+        if self.tenant_id is not None:
+            result['TenantId'] = self.tenant_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Connections') is not None:
+            self.connections = m.get('Connections')
+        if m.get('CreateTime') is not None:
+            self.create_time = m.get('CreateTime')
+        if m.get('Description') is not None:
+            self.description = m.get('Description')
+        if m.get('ErId') is not None:
+            self.er_id = m.get('ErId')
+        if m.get('ErName') is not None:
+            self.er_name = m.get('ErName')
+        if m.get('GmtModified') is not None:
+            self.gmt_modified = m.get('GmtModified')
+        if m.get('MasterZoneId') is not None:
+            self.master_zone_id = m.get('MasterZoneId')
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('RouteMaps') is not None:
+            self.route_maps = m.get('RouteMaps')
+        if m.get('Status') is not None:
+            self.status = m.get('Status')
+        if m.get('TenantId') is not None:
+            self.tenant_id = m.get('TenantId')
+        return self
+
+
+class ListErsResponseBodyContent(TeaModel):
+    def __init__(
+        self,
+        data: List[ListErsResponseBodyContentData] = None,
+        total: int = None,
+    ):
+        self.data = data
+        self.total = total
+
+    def validate(self):
+        if self.data:
+            for k in self.data:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['Data'] = []
+        if self.data is not None:
+            for k in self.data:
+                result['Data'].append(k.to_map() if k else None)
+        if self.total is not None:
+            result['Total'] = self.total
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.data = []
+        if m.get('Data') is not None:
+            for k in m.get('Data'):
+                temp_model = ListErsResponseBodyContentData()
+                self.data.append(temp_model.from_map(k))
+        if m.get('Total') is not None:
+            self.total = m.get('Total')
+        return self
+
+
+class ListErsResponseBody(TeaModel):
+    def __init__(
+        self,
+        code: int = None,
+        content: ListErsResponseBodyContent = None,
+        message: str = None,
+        request_id: str = None,
+    ):
+        self.code = code
+        self.content = content
+        self.message = message
+        self.request_id = request_id
+
+    def validate(self):
+        if self.content:
+            self.content.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.content is not None:
+            result['Content'] = self.content.to_map()
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Content') is not None:
+            temp_model = ListErsResponseBodyContent()
+            self.content = temp_model.from_map(m['Content'])
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class ListErsResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: ListErsResponseBody = None,
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
+            temp_model = ListErsResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class ListLniPrivateIpAddressRequest(TeaModel):
     def __init__(
         self,
         enable_page: bool = None,
         ip: str = None,
         ip_name: str = None,
         network_interface_id: str = None,
@@ -3903,52 +9313,52 @@
         return self
 
 
 class ListNetworkInterfacesResponseBodyContentDataSubnetBaseInfo(TeaModel):
     def __init__(
         self,
         cidr: str = None,
-        gmt_create: str = None,
-        name: str = None,
+        create_time: str = None,
         subnet_id: str = None,
+        subnet_name: str = None,
     ):
         self.cidr = cidr
-        self.gmt_create = gmt_create
-        self.name = name
+        self.create_time = create_time
         self.subnet_id = subnet_id
+        self.subnet_name = subnet_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.cidr is not None:
             result['Cidr'] = self.cidr
-        if self.gmt_create is not None:
-            result['GmtCreate'] = self.gmt_create
-        if self.name is not None:
-            result['Name'] = self.name
+        if self.create_time is not None:
+            result['CreateTime'] = self.create_time
         if self.subnet_id is not None:
             result['SubnetId'] = self.subnet_id
+        if self.subnet_name is not None:
+            result['SubnetName'] = self.subnet_name
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('Cidr') is not None:
             self.cidr = m.get('Cidr')
-        if m.get('GmtCreate') is not None:
-            self.gmt_create = m.get('GmtCreate')
-        if m.get('Name') is not None:
-            self.name = m.get('Name')
+        if m.get('CreateTime') is not None:
+            self.create_time = m.get('CreateTime')
         if m.get('SubnetId') is not None:
             self.subnet_id = m.get('SubnetId')
+        if m.get('SubnetName') is not None:
+            self.subnet_name = m.get('SubnetName')
         return self
 
 
 class ListNetworkInterfacesResponseBodyContentDataVpdBaseInfo(TeaModel):
     def __init__(
         self,
         cidr: str = None,
@@ -3998,14 +9408,15 @@
         self,
         create_time: str = None,
         ethernet: List[str] = None,
         gateway: str = None,
         ip: str = None,
         nc_type: str = None,
         network_interface_id: str = None,
+        network_interface_name: str = None,
         node_id: str = None,
         private_ip_address_mac_group: List[ListNetworkInterfacesResponseBodyContentDataPrivateIpAddressMacGroup] = None,
         quota: int = None,
         region_id: str = None,
         service_mac: str = None,
         status: str = None,
         subnet_base_info: ListNetworkInterfacesResponseBodyContentDataSubnetBaseInfo = None,
@@ -4015,14 +9426,15 @@
     ):
         self.create_time = create_time
         self.ethernet = ethernet
         self.gateway = gateway
         self.ip = ip
         self.nc_type = nc_type
         self.network_interface_id = network_interface_id
+        self.network_interface_name = network_interface_name
         self.node_id = node_id
         self.private_ip_address_mac_group = private_ip_address_mac_group
         self.quota = quota
         self.region_id = region_id
         self.service_mac = service_mac
         self.status = status
         self.subnet_base_info = subnet_base_info
@@ -4054,14 +9466,16 @@
             result['Gateway'] = self.gateway
         if self.ip is not None:
             result['Ip'] = self.ip
         if self.nc_type is not None:
             result['NcType'] = self.nc_type
         if self.network_interface_id is not None:
             result['NetworkInterfaceId'] = self.network_interface_id
+        if self.network_interface_name is not None:
+            result['NetworkInterfaceName'] = self.network_interface_name
         if self.node_id is not None:
             result['NodeId'] = self.node_id
         result['PrivateIpAddressMacGroup'] = []
         if self.private_ip_address_mac_group is not None:
             for k in self.private_ip_address_mac_group:
                 result['PrivateIpAddressMacGroup'].append(k.to_map() if k else None)
         if self.quota is not None:
@@ -4092,14 +9506,16 @@
             self.gateway = m.get('Gateway')
         if m.get('Ip') is not None:
             self.ip = m.get('Ip')
         if m.get('NcType') is not None:
             self.nc_type = m.get('NcType')
         if m.get('NetworkInterfaceId') is not None:
             self.network_interface_id = m.get('NetworkInterfaceId')
+        if m.get('NetworkInterfaceName') is not None:
+            self.network_interface_name = m.get('NetworkInterfaceName')
         if m.get('NodeId') is not None:
             self.node_id = m.get('NodeId')
         self.private_ip_address_mac_group = []
         if m.get('PrivateIpAddressMacGroup') is not None:
             for k in m.get('PrivateIpAddressMacGroup'):
                 temp_model = ListNetworkInterfacesResponseBodyContentDataPrivateIpAddressMacGroup()
                 self.private_ip_address_mac_group.append(temp_model.from_map(k))
@@ -5018,14 +10434,320 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ListVccGrantRulesResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class ListVccRouteEntriesRequest(TeaModel):
+    def __init__(
+        self,
+        destination_cidr_block: str = None,
+        enable_page: bool = None,
+        next_hop_id: str = None,
+        next_hop_type: str = None,
+        page_number: int = None,
+        page_size: int = None,
+        region_id: str = None,
+        route_type: str = None,
+        status: str = None,
+        vcc_id: str = None,
+        vpd_route_entry_id: str = None,
+    ):
+        self.destination_cidr_block = destination_cidr_block
+        self.enable_page = enable_page
+        self.next_hop_id = next_hop_id
+        self.next_hop_type = next_hop_type
+        self.page_number = page_number
+        self.page_size = page_size
+        self.region_id = region_id
+        self.route_type = route_type
+        self.status = status
+        self.vcc_id = vcc_id
+        self.vpd_route_entry_id = vpd_route_entry_id
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
+        if self.destination_cidr_block is not None:
+            result['DestinationCidrBlock'] = self.destination_cidr_block
+        if self.enable_page is not None:
+            result['EnablePage'] = self.enable_page
+        if self.next_hop_id is not None:
+            result['NextHopId'] = self.next_hop_id
+        if self.next_hop_type is not None:
+            result['NextHopType'] = self.next_hop_type
+        if self.page_number is not None:
+            result['PageNumber'] = self.page_number
+        if self.page_size is not None:
+            result['PageSize'] = self.page_size
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.route_type is not None:
+            result['RouteType'] = self.route_type
+        if self.status is not None:
+            result['Status'] = self.status
+        if self.vcc_id is not None:
+            result['VccId'] = self.vcc_id
+        if self.vpd_route_entry_id is not None:
+            result['VpdRouteEntryId'] = self.vpd_route_entry_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('DestinationCidrBlock') is not None:
+            self.destination_cidr_block = m.get('DestinationCidrBlock')
+        if m.get('EnablePage') is not None:
+            self.enable_page = m.get('EnablePage')
+        if m.get('NextHopId') is not None:
+            self.next_hop_id = m.get('NextHopId')
+        if m.get('NextHopType') is not None:
+            self.next_hop_type = m.get('NextHopType')
+        if m.get('PageNumber') is not None:
+            self.page_number = m.get('PageNumber')
+        if m.get('PageSize') is not None:
+            self.page_size = m.get('PageSize')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('RouteType') is not None:
+            self.route_type = m.get('RouteType')
+        if m.get('Status') is not None:
+            self.status = m.get('Status')
+        if m.get('VccId') is not None:
+            self.vcc_id = m.get('VccId')
+        if m.get('VpdRouteEntryId') is not None:
+            self.vpd_route_entry_id = m.get('VpdRouteEntryId')
+        return self
+
+
+class ListVccRouteEntriesResponseBodyContentData(TeaModel):
+    def __init__(
+        self,
+        destination_cidr_block: str = None,
+        gmt_modified: str = None,
+        next_hop_id: str = None,
+        next_hop_type: str = None,
+        region_id: str = None,
+        resource_tenant_id: str = None,
+        route_type: str = None,
+        status: str = None,
+        tenant_id: str = None,
+        vcc_id: str = None,
+        vcc_route_entry_id: str = None,
+    ):
+        self.destination_cidr_block = destination_cidr_block
+        self.gmt_modified = gmt_modified
+        self.next_hop_id = next_hop_id
+        self.next_hop_type = next_hop_type
+        self.region_id = region_id
+        self.resource_tenant_id = resource_tenant_id
+        self.route_type = route_type
+        self.status = status
+        self.tenant_id = tenant_id
+        self.vcc_id = vcc_id
+        self.vcc_route_entry_id = vcc_route_entry_id
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
+        if self.destination_cidr_block is not None:
+            result['DestinationCidrBlock'] = self.destination_cidr_block
+        if self.gmt_modified is not None:
+            result['GmtModified'] = self.gmt_modified
+        if self.next_hop_id is not None:
+            result['NextHopId'] = self.next_hop_id
+        if self.next_hop_type is not None:
+            result['NextHopType'] = self.next_hop_type
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.resource_tenant_id is not None:
+            result['ResourceTenantId'] = self.resource_tenant_id
+        if self.route_type is not None:
+            result['RouteType'] = self.route_type
+        if self.status is not None:
+            result['Status'] = self.status
+        if self.tenant_id is not None:
+            result['TenantId'] = self.tenant_id
+        if self.vcc_id is not None:
+            result['VccId'] = self.vcc_id
+        if self.vcc_route_entry_id is not None:
+            result['VccRouteEntryId'] = self.vcc_route_entry_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('DestinationCidrBlock') is not None:
+            self.destination_cidr_block = m.get('DestinationCidrBlock')
+        if m.get('GmtModified') is not None:
+            self.gmt_modified = m.get('GmtModified')
+        if m.get('NextHopId') is not None:
+            self.next_hop_id = m.get('NextHopId')
+        if m.get('NextHopType') is not None:
+            self.next_hop_type = m.get('NextHopType')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('ResourceTenantId') is not None:
+            self.resource_tenant_id = m.get('ResourceTenantId')
+        if m.get('RouteType') is not None:
+            self.route_type = m.get('RouteType')
+        if m.get('Status') is not None:
+            self.status = m.get('Status')
+        if m.get('TenantId') is not None:
+            self.tenant_id = m.get('TenantId')
+        if m.get('VccId') is not None:
+            self.vcc_id = m.get('VccId')
+        if m.get('VccRouteEntryId') is not None:
+            self.vcc_route_entry_id = m.get('VccRouteEntryId')
+        return self
+
+
+class ListVccRouteEntriesResponseBodyContent(TeaModel):
+    def __init__(
+        self,
+        data: List[ListVccRouteEntriesResponseBodyContentData] = None,
+        total: int = None,
+    ):
+        self.data = data
+        self.total = total
+
+    def validate(self):
+        if self.data:
+            for k in self.data:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['Data'] = []
+        if self.data is not None:
+            for k in self.data:
+                result['Data'].append(k.to_map() if k else None)
+        if self.total is not None:
+            result['Total'] = self.total
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.data = []
+        if m.get('Data') is not None:
+            for k in m.get('Data'):
+                temp_model = ListVccRouteEntriesResponseBodyContentData()
+                self.data.append(temp_model.from_map(k))
+        if m.get('Total') is not None:
+            self.total = m.get('Total')
+        return self
+
+
+class ListVccRouteEntriesResponseBody(TeaModel):
+    def __init__(
+        self,
+        code: int = None,
+        content: ListVccRouteEntriesResponseBodyContent = None,
+        message: str = None,
+        request_id: str = None,
+    ):
+        self.code = code
+        self.content = content
+        self.message = message
+        self.request_id = request_id
+
+    def validate(self):
+        if self.content:
+            self.content.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.content is not None:
+            result['Content'] = self.content.to_map()
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Content') is not None:
+            temp_model = ListVccRouteEntriesResponseBodyContent()
+            self.content = temp_model.from_map(m['Content'])
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class ListVccRouteEntriesResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: ListVccRouteEntriesResponseBody = None,
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
+            temp_model = ListVccRouteEntriesResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class ListVccsRequestTag(TeaModel):
     def __init__(
         self,
         key: str = None,
         value: str = None,
     ):
         self.key = key
@@ -5970,14 +11692,320 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ListVpdGrantRulesResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class ListVpdRouteEntriesRequest(TeaModel):
+    def __init__(
+        self,
+        destination_cidr_block: str = None,
+        enable_page: bool = None,
+        next_hop_id: str = None,
+        next_hop_type: str = None,
+        page_number: int = None,
+        page_size: int = None,
+        region_id: str = None,
+        route_type: str = None,
+        status: str = None,
+        vpd_id: str = None,
+        vpd_route_entry_id: str = None,
+    ):
+        self.destination_cidr_block = destination_cidr_block
+        self.enable_page = enable_page
+        self.next_hop_id = next_hop_id
+        self.next_hop_type = next_hop_type
+        self.page_number = page_number
+        self.page_size = page_size
+        self.region_id = region_id
+        self.route_type = route_type
+        self.status = status
+        self.vpd_id = vpd_id
+        self.vpd_route_entry_id = vpd_route_entry_id
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
+        if self.destination_cidr_block is not None:
+            result['DestinationCidrBlock'] = self.destination_cidr_block
+        if self.enable_page is not None:
+            result['EnablePage'] = self.enable_page
+        if self.next_hop_id is not None:
+            result['NextHopId'] = self.next_hop_id
+        if self.next_hop_type is not None:
+            result['NextHopType'] = self.next_hop_type
+        if self.page_number is not None:
+            result['PageNumber'] = self.page_number
+        if self.page_size is not None:
+            result['PageSize'] = self.page_size
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.route_type is not None:
+            result['RouteType'] = self.route_type
+        if self.status is not None:
+            result['Status'] = self.status
+        if self.vpd_id is not None:
+            result['VpdId'] = self.vpd_id
+        if self.vpd_route_entry_id is not None:
+            result['VpdRouteEntryId'] = self.vpd_route_entry_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('DestinationCidrBlock') is not None:
+            self.destination_cidr_block = m.get('DestinationCidrBlock')
+        if m.get('EnablePage') is not None:
+            self.enable_page = m.get('EnablePage')
+        if m.get('NextHopId') is not None:
+            self.next_hop_id = m.get('NextHopId')
+        if m.get('NextHopType') is not None:
+            self.next_hop_type = m.get('NextHopType')
+        if m.get('PageNumber') is not None:
+            self.page_number = m.get('PageNumber')
+        if m.get('PageSize') is not None:
+            self.page_size = m.get('PageSize')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('RouteType') is not None:
+            self.route_type = m.get('RouteType')
+        if m.get('Status') is not None:
+            self.status = m.get('Status')
+        if m.get('VpdId') is not None:
+            self.vpd_id = m.get('VpdId')
+        if m.get('VpdRouteEntryId') is not None:
+            self.vpd_route_entry_id = m.get('VpdRouteEntryId')
+        return self
+
+
+class ListVpdRouteEntriesResponseBodyContentData(TeaModel):
+    def __init__(
+        self,
+        destination_cidr_block: str = None,
+        gmt_modified: str = None,
+        next_hop_id: str = None,
+        next_hop_type: str = None,
+        region_id: str = None,
+        resource_tenant_id: str = None,
+        route_type: str = None,
+        status: str = None,
+        tenant_id: str = None,
+        vpd_id: str = None,
+        vpd_route_entry_id: str = None,
+    ):
+        self.destination_cidr_block = destination_cidr_block
+        self.gmt_modified = gmt_modified
+        self.next_hop_id = next_hop_id
+        self.next_hop_type = next_hop_type
+        self.region_id = region_id
+        self.resource_tenant_id = resource_tenant_id
+        self.route_type = route_type
+        self.status = status
+        self.tenant_id = tenant_id
+        self.vpd_id = vpd_id
+        self.vpd_route_entry_id = vpd_route_entry_id
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
+        if self.destination_cidr_block is not None:
+            result['DestinationCidrBlock'] = self.destination_cidr_block
+        if self.gmt_modified is not None:
+            result['GmtModified'] = self.gmt_modified
+        if self.next_hop_id is not None:
+            result['NextHopId'] = self.next_hop_id
+        if self.next_hop_type is not None:
+            result['NextHopType'] = self.next_hop_type
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.resource_tenant_id is not None:
+            result['ResourceTenantId'] = self.resource_tenant_id
+        if self.route_type is not None:
+            result['RouteType'] = self.route_type
+        if self.status is not None:
+            result['Status'] = self.status
+        if self.tenant_id is not None:
+            result['TenantId'] = self.tenant_id
+        if self.vpd_id is not None:
+            result['VpdId'] = self.vpd_id
+        if self.vpd_route_entry_id is not None:
+            result['VpdRouteEntryId'] = self.vpd_route_entry_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('DestinationCidrBlock') is not None:
+            self.destination_cidr_block = m.get('DestinationCidrBlock')
+        if m.get('GmtModified') is not None:
+            self.gmt_modified = m.get('GmtModified')
+        if m.get('NextHopId') is not None:
+            self.next_hop_id = m.get('NextHopId')
+        if m.get('NextHopType') is not None:
+            self.next_hop_type = m.get('NextHopType')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('ResourceTenantId') is not None:
+            self.resource_tenant_id = m.get('ResourceTenantId')
+        if m.get('RouteType') is not None:
+            self.route_type = m.get('RouteType')
+        if m.get('Status') is not None:
+            self.status = m.get('Status')
+        if m.get('TenantId') is not None:
+            self.tenant_id = m.get('TenantId')
+        if m.get('VpdId') is not None:
+            self.vpd_id = m.get('VpdId')
+        if m.get('VpdRouteEntryId') is not None:
+            self.vpd_route_entry_id = m.get('VpdRouteEntryId')
+        return self
+
+
+class ListVpdRouteEntriesResponseBodyContent(TeaModel):
+    def __init__(
+        self,
+        data: List[ListVpdRouteEntriesResponseBodyContentData] = None,
+        total: int = None,
+    ):
+        self.data = data
+        self.total = total
+
+    def validate(self):
+        if self.data:
+            for k in self.data:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['Data'] = []
+        if self.data is not None:
+            for k in self.data:
+                result['Data'].append(k.to_map() if k else None)
+        if self.total is not None:
+            result['Total'] = self.total
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.data = []
+        if m.get('Data') is not None:
+            for k in m.get('Data'):
+                temp_model = ListVpdRouteEntriesResponseBodyContentData()
+                self.data.append(temp_model.from_map(k))
+        if m.get('Total') is not None:
+            self.total = m.get('Total')
+        return self
+
+
+class ListVpdRouteEntriesResponseBody(TeaModel):
+    def __init__(
+        self,
+        code: int = None,
+        content: ListVpdRouteEntriesResponseBodyContent = None,
+        message: str = None,
+        request_id: str = None,
+    ):
+        self.code = code
+        self.content = content
+        self.message = message
+        self.request_id = request_id
+
+    def validate(self):
+        if self.content:
+            self.content.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.content is not None:
+            result['Content'] = self.content.to_map()
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Content') is not None:
+            temp_model = ListVpdRouteEntriesResponseBodyContent()
+            self.content = temp_model.from_map(m['Content'])
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class ListVpdRouteEntriesResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: ListVpdRouteEntriesResponseBody = None,
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
+            temp_model = ListVpdRouteEntriesResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class ListVpdsRequestTag(TeaModel):
     def __init__(
         self,
         key: str = None,
         value: str = None,
     ):
         self.key = key
@@ -6006,30 +12034,28 @@
             self.value = m.get('Value')
         return self
 
 
 class ListVpdsRequest(TeaModel):
     def __init__(
         self,
-        client_token: str = None,
         enable_page: bool = None,
         filter_er_id: str = None,
         for_select: bool = None,
         page_number: int = None,
         page_size: int = None,
         region_id: str = None,
         resource_group_id: str = None,
         status: str = None,
         tag: List[ListVpdsRequestTag] = None,
         vpd_id: str = None,
         vpd_name: str = None,
         with_dependence: bool = None,
         without_vcc: bool = None,
     ):
-        self.client_token = client_token
         self.enable_page = enable_page
         self.filter_er_id = filter_er_id
         self.for_select = for_select
         self.page_number = page_number
         self.page_size = page_size
         self.region_id = region_id
         self.resource_group_id = resource_group_id
@@ -6048,16 +12074,14 @@
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.client_token is not None:
-            result['ClientToken'] = self.client_token
         if self.enable_page is not None:
             result['EnablePage'] = self.enable_page
         if self.filter_er_id is not None:
             result['FilterErId'] = self.filter_er_id
         if self.for_select is not None:
             result['ForSelect'] = self.for_select
         if self.page_number is not None:
@@ -6082,16 +12106,14 @@
             result['WithDependence'] = self.with_dependence
         if self.without_vcc is not None:
             result['WithoutVcc'] = self.without_vcc
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ClientToken') is not None:
-            self.client_token = m.get('ClientToken')
         if m.get('EnablePage') is not None:
             self.enable_page = m.get('EnablePage')
         if m.get('FilterErId') is not None:
             self.filter_er_id = m.get('FilterErId')
         if m.get('ForSelect') is not None:
             self.for_select = m.get('ForSelect')
         if m.get('PageNumber') is not None:
@@ -6512,22 +12534,20 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class UnAssignPrivateIpAddressRequest(TeaModel):
     def __init__(
         self,
-        client_token: str = None,
         ip_name: str = None,
         network_interface_id: str = None,
         private_ip_address: str = None,
         region_id: str = None,
         subnet_id: str = None,
     ):
-        self.client_token = client_token
         self.ip_name = ip_name
         self.network_interface_id = network_interface_id
         self.private_ip_address = private_ip_address
         self.region_id = region_id
         self.subnet_id = subnet_id
 
     def validate(self):
@@ -6535,32 +12555,28 @@
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.client_token is not None:
-            result['ClientToken'] = self.client_token
         if self.ip_name is not None:
             result['IpName'] = self.ip_name
         if self.network_interface_id is not None:
             result['NetworkInterfaceId'] = self.network_interface_id
         if self.private_ip_address is not None:
             result['PrivateIpAddress'] = self.private_ip_address
         if self.region_id is not None:
             result['RegionId'] = self.region_id
         if self.subnet_id is not None:
             result['SubnetId'] = self.subnet_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ClientToken') is not None:
-            self.client_token = m.get('ClientToken')
         if m.get('IpName') is not None:
             self.ip_name = m.get('IpName')
         if m.get('NetworkInterfaceId') is not None:
             self.network_interface_id = m.get('NetworkInterfaceId')
         if m.get('PrivateIpAddress') is not None:
             self.private_ip_address = m.get('PrivateIpAddress')
         if m.get('RegionId') is not None:
@@ -6690,25 +12706,425 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = UnAssignPrivateIpAddressResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class UpdateSubnetRequest(TeaModel):
+class UpdateErRequest(TeaModel):
     def __init__(
         self,
         description: str = None,
+        er_id: str = None,
+        er_name: str = None,
+        region_id: str = None,
+    ):
+        self.description = description
+        self.er_id = er_id
+        self.er_name = er_name
+        self.region_id = region_id
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
+        if self.description is not None:
+            result['Description'] = self.description
+        if self.er_id is not None:
+            result['ErId'] = self.er_id
+        if self.er_name is not None:
+            result['ErName'] = self.er_name
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Description') is not None:
+            self.description = m.get('Description')
+        if m.get('ErId') is not None:
+            self.er_id = m.get('ErId')
+        if m.get('ErName') is not None:
+            self.er_name = m.get('ErName')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        return self
+
+
+class UpdateErResponseBody(TeaModel):
+    def __init__(
+        self,
+        code: int = None,
+        content: Dict[str, Any] = None,
+        message: str = None,
+        request_id: str = None,
+    ):
+        self.code = code
+        self.content = content
+        self.message = message
+        self.request_id = request_id
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
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.content is not None:
+            result['Content'] = self.content
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Content') is not None:
+            self.content = m.get('Content')
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class UpdateErResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: UpdateErResponseBody = None,
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
+            temp_model = UpdateErResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class UpdateErAttachmentRequest(TeaModel):
+    def __init__(
+        self,
+        er_attachment_id: str = None,
+        er_attachment_name: str = None,
+        er_id: str = None,
+        region_id: str = None,
+    ):
+        self.er_attachment_id = er_attachment_id
+        self.er_attachment_name = er_attachment_name
+        self.er_id = er_id
+        self.region_id = region_id
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
+        if self.er_attachment_id is not None:
+            result['ErAttachmentId'] = self.er_attachment_id
+        if self.er_attachment_name is not None:
+            result['ErAttachmentName'] = self.er_attachment_name
+        if self.er_id is not None:
+            result['ErId'] = self.er_id
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ErAttachmentId') is not None:
+            self.er_attachment_id = m.get('ErAttachmentId')
+        if m.get('ErAttachmentName') is not None:
+            self.er_attachment_name = m.get('ErAttachmentName')
+        if m.get('ErId') is not None:
+            self.er_id = m.get('ErId')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        return self
+
+
+class UpdateErAttachmentResponseBody(TeaModel):
+    def __init__(
+        self,
+        code: int = None,
+        content: Dict[str, Any] = None,
+        message: str = None,
+        request_id: str = None,
+    ):
+        self.code = code
+        self.content = content
+        self.message = message
+        self.request_id = request_id
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
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.content is not None:
+            result['Content'] = self.content
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Content') is not None:
+            self.content = m.get('Content')
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class UpdateErAttachmentResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: UpdateErAttachmentResponseBody = None,
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
+            temp_model = UpdateErAttachmentResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class UpdateErRouteMapRequest(TeaModel):
+    def __init__(
+        self,
+        description: str = None,
+        er_id: str = None,
+        er_route_map_id: str = None,
+        region_id: str = None,
+    ):
+        self.description = description
+        self.er_id = er_id
+        self.er_route_map_id = er_route_map_id
+        self.region_id = region_id
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
+        if self.description is not None:
+            result['Description'] = self.description
+        if self.er_id is not None:
+            result['ErId'] = self.er_id
+        if self.er_route_map_id is not None:
+            result['ErRouteMapId'] = self.er_route_map_id
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Description') is not None:
+            self.description = m.get('Description')
+        if m.get('ErId') is not None:
+            self.er_id = m.get('ErId')
+        if m.get('ErRouteMapId') is not None:
+            self.er_route_map_id = m.get('ErRouteMapId')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        return self
+
+
+class UpdateErRouteMapResponseBody(TeaModel):
+    def __init__(
+        self,
+        code: int = None,
+        content: Dict[str, Any] = None,
+        message: str = None,
+        request_id: str = None,
+    ):
+        self.code = code
+        self.content = content
+        self.message = message
+        self.request_id = request_id
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
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.content is not None:
+            result['Content'] = self.content
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Content') is not None:
+            self.content = m.get('Content')
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class UpdateErRouteMapResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: UpdateErRouteMapResponseBody = None,
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
+            temp_model = UpdateErRouteMapResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class UpdateSubnetRequest(TeaModel):
+    def __init__(
+        self,
         region_id: str = None,
         subnet_id: str = None,
         subnet_name: str = None,
         vpd_id: str = None,
         zone_id: str = None,
     ):
-        self.description = description
         self.region_id = region_id
         self.subnet_id = subnet_id
         self.subnet_name = subnet_name
         self.vpd_id = vpd_id
         self.zone_id = zone_id
 
     def validate(self):
@@ -6716,32 +13132,28 @@
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.description is not None:
-            result['Description'] = self.description
         if self.region_id is not None:
             result['RegionId'] = self.region_id
         if self.subnet_id is not None:
             result['SubnetId'] = self.subnet_id
         if self.subnet_name is not None:
             result['SubnetName'] = self.subnet_name
         if self.vpd_id is not None:
             result['VpdId'] = self.vpd_id
         if self.zone_id is not None:
             result['ZoneId'] = self.zone_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('Description') is not None:
-            self.description = m.get('Description')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
         if m.get('SubnetId') is not None:
             self.subnet_id = m.get('SubnetId')
         if m.get('SubnetName') is not None:
             self.subnet_name = m.get('SubnetName')
         if m.get('VpdId') is not None:
@@ -7037,47 +13449,41 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class UpdateVpdRequest(TeaModel):
     def __init__(
         self,
-        client_token: str = None,
         region_id: str = None,
         vpd_id: str = None,
         vpd_name: str = None,
     ):
-        self.client_token = client_token
         self.region_id = region_id
         self.vpd_id = vpd_id
         self.vpd_name = vpd_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.client_token is not None:
-            result['ClientToken'] = self.client_token
         if self.region_id is not None:
             result['RegionId'] = self.region_id
         if self.vpd_id is not None:
             result['VpdId'] = self.vpd_id
         if self.vpd_name is not None:
             result['VpdName'] = self.vpd_name
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ClientToken') is not None:
-            self.client_token = m.get('ClientToken')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
         if m.get('VpdId') is not None:
             self.vpd_id = m.get('VpdId')
         if m.get('VpdName') is not None:
             self.vpd_name = m.get('VpdName')
         return self
```

### Comparing `alibabacloud_eflo20220530-1.0.2/alibabacloud_eflo20220530.egg-info/PKG-INFO` & `alibabacloud_eflo20220530-1.0.3/alibabacloud_eflo20220530.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-eflo20220530
-Version: 1.0.2
+Version: 1.0.3
 Summary: Alibaba Cloud eflo (20220530) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_eflo20220530-1.0.2/setup.py` & `alibabacloud_eflo20220530-1.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_eflo20220530.
 
-Created on 30/03/2023
+Created on 13/04/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_eflo20220530"
 NAME = "alibabacloud_eflo20220530" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud eflo (20220530) SDK Library for Python"
```

