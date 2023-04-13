# Comparing `tmp/mypy-boto3-mediaconnect-1.26.0.post1.tar.gz` & `tmp/mypy-boto3-mediaconnect-1.26.113.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-mediaconnect-1.26.0.post1.tar", last modified: Tue Nov  1 21:43:42 2022, max compression
+gzip compressed data, was "mypy-boto3-mediaconnect-1.26.113.tar", last modified: Thu Apr 13 19:32:29 2023, max compression
```

## Comparing `mypy-boto3-mediaconnect-1.26.0.post1.tar` & `mypy-boto3-mediaconnect-1.26.113.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:42.976834 mypy-boto3-mediaconnect-1.26.0.post1/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-01 21:37:45.000000 mypy-boto3-mediaconnect-1.26.0.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    18566 2022-11-01 21:43:42.972834 mypy-boto3-mediaconnect-1.26.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    17105 2022-11-01 21:37:45.000000 mypy-boto3-mediaconnect-1.26.0.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:42.968834 mypy-boto3-mediaconnect-1.26.0.post1/mypy_boto3_mediaconnect/
--rw-r--r--   0 runner    (1001) docker     (121)     1664 2022-11-01 21:37:45.000000 mypy-boto3-mediaconnect-1.26.0.post1/mypy_boto3_mediaconnect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1663 2022-11-01 21:37:45.000000 mypy-boto3-mediaconnect-1.26.0.post1/mypy_boto3_mediaconnect/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      937 2022-11-01 21:37:45.000000 mypy-boto3-mediaconnect-1.26.0.post1/mypy_boto3_mediaconnect/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    26348 2022-11-01 21:37:47.000000 mypy-boto3-mediaconnect-1.26.0.post1/mypy_boto3_mediaconnect/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    26304 2022-11-01 21:37:47.000000 mypy-boto3-mediaconnect-1.26.0.post1/mypy_boto3_mediaconnect/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     9923 2022-11-01 21:37:47.000000 mypy-boto3-mediaconnect-1.26.0.post1/mypy_boto3_mediaconnect/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)     9921 2022-11-01 21:37:47.000000 mypy-boto3-mediaconnect-1.26.0.post1/mypy_boto3_mediaconnect/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     5003 2022-11-01 21:37:47.000000 mypy-boto3-mediaconnect-1.26.0.post1/mypy_boto3_mediaconnect/paginator.py
--rw-r--r--   0 runner    (1001) docker     (121)     4997 2022-11-01 21:37:47.000000 mypy-boto3-mediaconnect-1.26.0.post1/mypy_boto3_mediaconnect/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-01 21:37:45.000000 mypy-boto3-mediaconnect-1.26.0.post1/mypy_boto3_mediaconnect/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    40945 2022-11-01 21:37:48.000000 mypy-boto3-mediaconnect-1.26.0.post1/mypy_boto3_mediaconnect/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)    40888 2022-11-01 21:37:47.000000 mypy-boto3-mediaconnect-1.26.0.post1/mypy_boto3_mediaconnect/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-11-01 21:37:45.000000 mypy-boto3-mediaconnect-1.26.0.post1/mypy_boto3_mediaconnect/version.py
--rw-r--r--   0 runner    (1001) docker     (121)     3168 2022-11-01 21:37:47.000000 mypy-boto3-mediaconnect-1.26.0.post1/mypy_boto3_mediaconnect/waiter.py
--rw-r--r--   0 runner    (1001) docker     (121)     3165 2022-11-01 21:37:47.000000 mypy-boto3-mediaconnect-1.26.0.post1/mypy_boto3_mediaconnect/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:42.972834 mypy-boto3-mediaconnect-1.26.0.post1/mypy_boto3_mediaconnect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    18566 2022-11-01 21:43:42.000000 mypy-boto3-mediaconnect-1.26.0.post1/mypy_boto3_mediaconnect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      844 2022-11-01 21:43:42.000000 mypy-boto3-mediaconnect-1.26.0.post1/mypy_boto3_mediaconnect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:42.000000 mypy-boto3-mediaconnect-1.26.0.post1/mypy_boto3_mediaconnect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:42.000000 mypy-boto3-mediaconnect-1.26.0.post1/mypy_boto3_mediaconnect.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-01 21:43:42.000000 mypy-boto3-mediaconnect-1.26.0.post1/mypy_boto3_mediaconnect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-11-01 21:43:42.000000 mypy-boto3-mediaconnect-1.26.0.post1/mypy_boto3_mediaconnect.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-01 21:43:42.976834 mypy-boto3-mediaconnect-1.26.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2003 2022-11-01 21:37:45.000000 mypy-boto3-mediaconnect-1.26.0.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:32:29.140819 mypy-boto3-mediaconnect-1.26.113/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-13 19:32:15.000000 mypy-boto3-mediaconnect-1.26.113/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    22062 2023-04-13 19:32:29.140819 mypy-boto3-mediaconnect-1.26.113/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20553 2023-04-13 19:32:15.000000 mypy-boto3-mediaconnect-1.26.113/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:32:29.140819 mypy-boto3-mediaconnect-1.26.113/mypy_boto3_mediaconnect/
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-04-13 19:32:15.000000 mypy-boto3-mediaconnect-1.26.113/mypy_boto3_mediaconnect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-04-13 19:32:15.000000 mypy-boto3-mediaconnect-1.26.113/mypy_boto3_mediaconnect/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-04-13 19:32:15.000000 mypy-boto3-mediaconnect-1.26.113/mypy_boto3_mediaconnect/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40366 2023-04-13 19:32:16.000000 mypy-boto3-mediaconnect-1.26.113/mypy_boto3_mediaconnect/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40299 2023-04-13 19:32:15.000000 mypy-boto3-mediaconnect-1.26.113/mypy_boto3_mediaconnect/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11652 2023-04-13 19:32:16.000000 mypy-boto3-mediaconnect-1.26.113/mypy_boto3_mediaconnect/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11650 2023-04-13 19:32:16.000000 mypy-boto3-mediaconnect-1.26.113/mypy_boto3_mediaconnect/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8190 2023-04-13 19:32:16.000000 mypy-boto3-mediaconnect-1.26.113/mypy_boto3_mediaconnect/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8181 2023-04-13 19:32:16.000000 mypy-boto3-mediaconnect-1.26.113/mypy_boto3_mediaconnect/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 19:32:15.000000 mypy-boto3-mediaconnect-1.26.113/mypy_boto3_mediaconnect/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    64946 2023-04-13 19:32:18.000000 mypy-boto3-mediaconnect-1.26.113/mypy_boto3_mediaconnect/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64855 2023-04-13 19:32:17.000000 mypy-boto3-mediaconnect-1.26.113/mypy_boto3_mediaconnect/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-13 19:32:15.000000 mypy-boto3-mediaconnect-1.26.113/mypy_boto3_mediaconnect/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-04-13 19:32:16.000000 mypy-boto3-mediaconnect-1.26.113/mypy_boto3_mediaconnect/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-04-13 19:32:16.000000 mypy-boto3-mediaconnect-1.26.113/mypy_boto3_mediaconnect/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:32:29.140819 mypy-boto3-mediaconnect-1.26.113/mypy_boto3_mediaconnect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22062 2023-04-13 19:32:29.000000 mypy-boto3-mediaconnect-1.26.113/mypy_boto3_mediaconnect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-04-13 19:32:29.000000 mypy-boto3-mediaconnect-1.26.113/mypy_boto3_mediaconnect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 19:32:29.000000 mypy-boto3-mediaconnect-1.26.113/mypy_boto3_mediaconnect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 19:32:29.000000 mypy-boto3-mediaconnect-1.26.113/mypy_boto3_mediaconnect.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-13 19:32:29.000000 mypy-boto3-mediaconnect-1.26.113/mypy_boto3_mediaconnect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-13 19:32:29.000000 mypy-boto3-mediaconnect-1.26.113/mypy_boto3_mediaconnect.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 19:32:29.140819 mypy-boto3-mediaconnect-1.26.113/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-04-13 19:32:15.000000 mypy-boto3-mediaconnect-1.26.113/setup.py
```

### Comparing `mypy-boto3-mediaconnect-1.26.0.post1/LICENSE` & `mypy-boto3-mediaconnect-1.26.113/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Vlad Emelianov
+Copyright (c) 2023 Vlad Emelianov
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `mypy-boto3-mediaconnect-1.26.0.post1/mypy_boto3_mediaconnect/__main__.py` & `mypy-boto3-mediaconnect-1.26.113/mypy_boto3_mediaconnect/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.MediaConnect 1.26.0\nVersion:         1.26.0.post1\nBuilder"
-        " version: 7.11.10\nDocs:           "
+        "Type annotations for boto3.MediaConnect 1.26.113\nVersion:         1.26.113\nBuilder"
+        " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.0.post1")
+    print("1.26.113")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-mediaconnect-1.26.0.post1/mypy_boto3_mediaconnect/client.py` & `mypy-boto3-mediaconnect-1.26.113/mypy_boto3_mediaconnect/client.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,62 +14,102 @@
     ```
 """
 import sys
 from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
-from .literals import EntitlementStatusType, MediaStreamTypeType, ProtocolType
+from .literals import (
+    BridgePlacementType,
+    DesiredStateType,
+    EntitlementStatusType,
+    MediaStreamTypeType,
+    ProtocolType,
+)
 from .paginator import (
+    ListBridgesPaginator,
     ListEntitlementsPaginator,
     ListFlowsPaginator,
+    ListGatewayInstancesPaginator,
+    ListGatewaysPaginator,
     ListOfferingsPaginator,
     ListReservationsPaginator,
 )
 from .type_defs import (
+    AddBridgeOutputRequestTypeDef,
+    AddBridgeOutputsResponseTypeDef,
+    AddBridgeSourceRequestTypeDef,
+    AddBridgeSourcesResponseTypeDef,
+    AddEgressGatewayBridgeRequestTypeDef,
     AddFlowMediaStreamsResponseTypeDef,
     AddFlowOutputsResponseTypeDef,
     AddFlowSourcesResponseTypeDef,
     AddFlowVpcInterfacesResponseTypeDef,
+    AddIngressGatewayBridgeRequestTypeDef,
     AddMaintenanceTypeDef,
     AddMediaStreamRequestTypeDef,
     AddOutputRequestTypeDef,
+    CreateBridgeResponseTypeDef,
     CreateFlowResponseTypeDef,
+    CreateGatewayResponseTypeDef,
+    DeleteBridgeResponseTypeDef,
     DeleteFlowResponseTypeDef,
+    DeleteGatewayResponseTypeDef,
+    DeregisterGatewayInstanceResponseTypeDef,
+    DescribeBridgeResponseTypeDef,
     DescribeFlowResponseTypeDef,
+    DescribeGatewayInstanceResponseTypeDef,
+    DescribeGatewayResponseTypeDef,
     DescribeOfferingResponseTypeDef,
     DescribeReservationResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     FailoverConfigTypeDef,
+    GatewayNetworkTypeDef,
     GrantEntitlementRequestTypeDef,
     GrantFlowEntitlementsResponseTypeDef,
+    ListBridgesResponseTypeDef,
     ListEntitlementsResponseTypeDef,
     ListFlowsResponseTypeDef,
+    ListGatewayInstancesResponseTypeDef,
+    ListGatewaysResponseTypeDef,
     ListOfferingsResponseTypeDef,
     ListReservationsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     MediaStreamAttributesRequestTypeDef,
     MediaStreamOutputConfigurationRequestTypeDef,
     MediaStreamSourceConfigurationRequestTypeDef,
     PurchaseOfferingResponseTypeDef,
+    RemoveBridgeOutputResponseTypeDef,
+    RemoveBridgeSourceResponseTypeDef,
     RemoveFlowMediaStreamResponseTypeDef,
     RemoveFlowOutputResponseTypeDef,
     RemoveFlowSourceResponseTypeDef,
     RemoveFlowVpcInterfaceResponseTypeDef,
     RevokeFlowEntitlementResponseTypeDef,
     SetSourceRequestTypeDef,
     StartFlowResponseTypeDef,
     StopFlowResponseTypeDef,
+    UpdateBridgeFlowSourceRequestTypeDef,
+    UpdateBridgeNetworkOutputRequestTypeDef,
+    UpdateBridgeNetworkSourceRequestTypeDef,
+    UpdateBridgeOutputResponseTypeDef,
+    UpdateBridgeResponseTypeDef,
+    UpdateBridgeSourceResponseTypeDef,
+    UpdateBridgeStateResponseTypeDef,
+    UpdateEgressGatewayBridgeRequestTypeDef,
     UpdateEncryptionTypeDef,
     UpdateFailoverConfigTypeDef,
     UpdateFlowEntitlementResponseTypeDef,
     UpdateFlowMediaStreamResponseTypeDef,
     UpdateFlowOutputResponseTypeDef,
     UpdateFlowResponseTypeDef,
     UpdateFlowSourceResponseTypeDef,
+    UpdateGatewayBridgeSourceRequestTypeDef,
+    UpdateGatewayInstanceResponseTypeDef,
+    UpdateIngressGatewayBridgeRequestTypeDef,
     UpdateMaintenanceTypeDef,
     VpcInterfaceAttachmentTypeDef,
     VpcInterfaceRequestTypeDef,
 )
 from .waiter import FlowActiveWaiter, FlowDeletedWaiter, FlowStandbyWaiter
 
 if sys.version_info >= (3, 9):
@@ -89,15 +129,18 @@
         self.operation_name: str
 
 
 class Exceptions:
     AddFlowOutputs420Exception: Type[BotocoreClientError]
     BadRequestException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
+    ConflictException: Type[BotocoreClientError]
+    CreateBridge420Exception: Type[BotocoreClientError]
     CreateFlow420Exception: Type[BotocoreClientError]
+    CreateGateway420Exception: Type[BotocoreClientError]
     ForbiddenException: Type[BotocoreClientError]
     GrantFlowEntitlements420Exception: Type[BotocoreClientError]
     InternalServerErrorException: Type[BotocoreClientError]
     NotFoundException: Type[BotocoreClientError]
     ServiceUnavailableException: Type[BotocoreClientError]
     TooManyRequestsException: Type[BotocoreClientError]
 
@@ -115,14 +158,34 @@
         """
         MediaConnectClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/client/#exceptions)
         """
 
+    def add_bridge_outputs(
+        self, *, BridgeArn: str, Outputs: Sequence[AddBridgeOutputRequestTypeDef]
+    ) -> AddBridgeOutputsResponseTypeDef:
+        """
+        Adds outputs to an existing bridge.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.add_bridge_outputs)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/client/#add_bridge_outputs)
+        """
+
+    def add_bridge_sources(
+        self, *, BridgeArn: str, Sources: Sequence[AddBridgeSourceRequestTypeDef]
+    ) -> AddBridgeSourcesResponseTypeDef:
+        """
+        Adds sources to an existing bridge.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.add_bridge_sources)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/client/#add_bridge_sources)
+        """
+
     def add_flow_media_streams(
         self, *, FlowArn: str, MediaStreams: Sequence[AddMediaStreamRequestTypeDef]
     ) -> AddFlowMediaStreamsResponseTypeDef:
         """
         Adds media streams to an existing flow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.add_flow_media_streams)
@@ -173,14 +236,32 @@
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/client/#close)
         """
 
+    def create_bridge(
+        self,
+        *,
+        Name: str,
+        PlacementArn: str,
+        Sources: Sequence[AddBridgeSourceRequestTypeDef],
+        EgressGatewayBridge: AddEgressGatewayBridgeRequestTypeDef = ...,
+        IngressGatewayBridge: AddIngressGatewayBridgeRequestTypeDef = ...,
+        Outputs: Sequence[AddBridgeOutputRequestTypeDef] = ...,
+        SourceFailoverConfig: FailoverConfigTypeDef = ...
+    ) -> CreateBridgeResponseTypeDef:
+        """
+        Creates a new bridge.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.create_bridge)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/client/#create_bridge)
+        """
+
     def create_flow(
         self,
         *,
         Name: str,
         AvailabilityZone: str = ...,
         Entitlements: Sequence[GrantEntitlementRequestTypeDef] = ...,
         MediaStreams: Sequence[AddMediaStreamRequestTypeDef] = ...,
@@ -194,30 +275,96 @@
         """
         Creates a new flow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.create_flow)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/client/#create_flow)
         """
 
+    def create_gateway(
+        self,
+        *,
+        EgressCidrBlocks: Sequence[str],
+        Name: str,
+        Networks: Sequence[GatewayNetworkTypeDef]
+    ) -> CreateGatewayResponseTypeDef:
+        """
+        Creates a new gateway.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.create_gateway)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/client/#create_gateway)
+        """
+
+    def delete_bridge(self, *, BridgeArn: str) -> DeleteBridgeResponseTypeDef:
+        """
+        Deletes a bridge.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.delete_bridge)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/client/#delete_bridge)
+        """
+
     def delete_flow(self, *, FlowArn: str) -> DeleteFlowResponseTypeDef:
         """
         Deletes a flow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.delete_flow)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/client/#delete_flow)
         """
 
+    def delete_gateway(self, *, GatewayArn: str) -> DeleteGatewayResponseTypeDef:
+        """
+        Deletes a gateway.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.delete_gateway)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/client/#delete_gateway)
+        """
+
+    def deregister_gateway_instance(
+        self, *, GatewayInstanceArn: str, Force: bool = ...
+    ) -> DeregisterGatewayInstanceResponseTypeDef:
+        """
+        Deregisters an instance.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.deregister_gateway_instance)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/client/#deregister_gateway_instance)
+        """
+
+    def describe_bridge(self, *, BridgeArn: str) -> DescribeBridgeResponseTypeDef:
+        """
+        Displays the details of a bridge.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.describe_bridge)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/client/#describe_bridge)
+        """
+
     def describe_flow(self, *, FlowArn: str) -> DescribeFlowResponseTypeDef:
         """
         Displays the details of a flow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.describe_flow)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/client/#describe_flow)
         """
 
+    def describe_gateway(self, *, GatewayArn: str) -> DescribeGatewayResponseTypeDef:
+        """
+        Displays the details of a gateway.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.describe_gateway)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/client/#describe_gateway)
+        """
+
+    def describe_gateway_instance(
+        self, *, GatewayInstanceArn: str
+    ) -> DescribeGatewayInstanceResponseTypeDef:
+        """
+        Displays the details of an instance.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.describe_gateway_instance)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/client/#describe_gateway_instance)
+        """
+
     def describe_offering(self, *, OfferingArn: str) -> DescribeOfferingResponseTypeDef:
         """
         Displays the details of an offering.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.describe_offering)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/client/#describe_offering)
         """
@@ -250,14 +397,25 @@
         """
         Grants entitlements to an existing flow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.grant_flow_entitlements)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/client/#grant_flow_entitlements)
         """
 
+    def list_bridges(
+        self, *, FilterArn: str = ..., MaxResults: int = ..., NextToken: str = ...
+    ) -> ListBridgesResponseTypeDef:
+        """
+        Displays a list of bridges that are associated with this account and an
+        optionally specified Arn.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.list_bridges)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/client/#list_bridges)
+        """
+
     def list_entitlements(
         self, *, MaxResults: int = ..., NextToken: str = ...
     ) -> ListEntitlementsResponseTypeDef:
         """
         Displays a list of all entitlements that have been granted to this account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.list_entitlements)
@@ -270,14 +428,34 @@
         """
         Displays a list of flows that are associated with this account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.list_flows)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/client/#list_flows)
         """
 
+    def list_gateway_instances(
+        self, *, FilterArn: str = ..., MaxResults: int = ..., NextToken: str = ...
+    ) -> ListGatewayInstancesResponseTypeDef:
+        """
+        Displays a list of instances associated with the AWS account.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.list_gateway_instances)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/client/#list_gateway_instances)
+        """
+
+    def list_gateways(
+        self, *, MaxResults: int = ..., NextToken: str = ...
+    ) -> ListGatewaysResponseTypeDef:
+        """
+        Displays a list of gateways that are associated with this account.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.list_gateways)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/client/#list_gateways)
+        """
+
     def list_offerings(
         self, *, MaxResults: int = ..., NextToken: str = ...
     ) -> ListOfferingsResponseTypeDef:
         """
         Displays a list of all offerings that are available to this account in the
         current AWS Region.
 
@@ -311,14 +489,34 @@
         """
         Submits a request to purchase an offering.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.purchase_offering)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/client/#purchase_offering)
         """
 
+    def remove_bridge_output(
+        self, *, BridgeArn: str, OutputName: str
+    ) -> RemoveBridgeOutputResponseTypeDef:
+        """
+        Removes an output from a bridge.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.remove_bridge_output)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/client/#remove_bridge_output)
+        """
+
+    def remove_bridge_source(
+        self, *, BridgeArn: str, SourceName: str
+    ) -> RemoveBridgeSourceResponseTypeDef:
+        """
+        Removes a source from a bridge.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.remove_bridge_source)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/client/#remove_bridge_source)
+        """
+
     def remove_flow_media_stream(
         self, *, FlowArn: str, MediaStreamName: str
     ) -> RemoveFlowMediaStreamResponseTypeDef:
         """
         Removes a media stream from a flow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.remove_flow_media_stream)
@@ -397,14 +595,70 @@
         """
         Deletes specified tags from a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/client/#untag_resource)
         """
 
+    def update_bridge(
+        self,
+        *,
+        BridgeArn: str,
+        EgressGatewayBridge: UpdateEgressGatewayBridgeRequestTypeDef = ...,
+        IngressGatewayBridge: UpdateIngressGatewayBridgeRequestTypeDef = ...,
+        SourceFailoverConfig: UpdateFailoverConfigTypeDef = ...
+    ) -> UpdateBridgeResponseTypeDef:
+        """
+        Updates the bridge See also: [AWS API
+        Documentation](https://docs.aws.amazon.com/goto/WebAPI/mediaconnect-2018-11-14/UpdateBridge).
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.update_bridge)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/client/#update_bridge)
+        """
+
+    def update_bridge_output(
+        self,
+        *,
+        BridgeArn: str,
+        OutputName: str,
+        NetworkOutput: UpdateBridgeNetworkOutputRequestTypeDef = ...
+    ) -> UpdateBridgeOutputResponseTypeDef:
+        """
+        Updates an existing bridge output.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.update_bridge_output)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/client/#update_bridge_output)
+        """
+
+    def update_bridge_source(
+        self,
+        *,
+        BridgeArn: str,
+        SourceName: str,
+        FlowSource: UpdateBridgeFlowSourceRequestTypeDef = ...,
+        NetworkSource: UpdateBridgeNetworkSourceRequestTypeDef = ...
+    ) -> UpdateBridgeSourceResponseTypeDef:
+        """
+        Updates an existing bridge source.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.update_bridge_source)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/client/#update_bridge_source)
+        """
+
+    def update_bridge_state(
+        self, *, BridgeArn: str, DesiredState: DesiredStateType
+    ) -> UpdateBridgeStateResponseTypeDef:
+        """
+        Updates the bridge state See also: [AWS API
+        Documentation](https://docs.aws.amazon.com/goto/WebAPI/mediaconnect-2018-11-14/UpdateBridgeState).
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.update_bridge_state)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/client/#update_bridge_state)
+        """
+
     def update_flow(
         self,
         *,
         FlowArn: str,
         SourceFailoverConfig: UpdateFailoverConfigTypeDef = ...,
         Maintenance: UpdateMaintenanceTypeDef = ...
     ) -> UpdateFlowResponseTypeDef:
@@ -500,23 +754,41 @@
         Protocol: ProtocolType = ...,
         SenderControlPort: int = ...,
         SenderIpAddress: str = ...,
         SourceListenerAddress: str = ...,
         SourceListenerPort: int = ...,
         StreamId: str = ...,
         VpcInterfaceName: str = ...,
-        WhitelistCidr: str = ...
+        WhitelistCidr: str = ...,
+        GatewayBridgeSource: UpdateGatewayBridgeSourceRequestTypeDef = ...
     ) -> UpdateFlowSourceResponseTypeDef:
         """
         Updates the source of a flow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.update_flow_source)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/client/#update_flow_source)
         """
 
+    def update_gateway_instance(
+        self, *, GatewayInstanceArn: str, BridgePlacement: BridgePlacementType = ...
+    ) -> UpdateGatewayInstanceResponseTypeDef:
+        """
+        Updates the configuration of an existing Gateway Instance.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.update_gateway_instance)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/client/#update_gateway_instance)
+        """
+
+    @overload
+    def get_paginator(self, operation_name: Literal["list_bridges"]) -> ListBridgesPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/client/#get_paginator)
+        """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_entitlements"]
     ) -> ListEntitlementsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/client/#get_paginator)
@@ -526,14 +798,30 @@
     def get_paginator(self, operation_name: Literal["list_flows"]) -> ListFlowsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/client/#get_paginator)
         """
 
     @overload
+    def get_paginator(
+        self, operation_name: Literal["list_gateway_instances"]
+    ) -> ListGatewayInstancesPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/client/#get_paginator)
+        """
+
+    @overload
+    def get_paginator(self, operation_name: Literal["list_gateways"]) -> ListGatewaysPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/client/#get_paginator)
+        """
+
+    @overload
     def get_paginator(self, operation_name: Literal["list_offerings"]) -> ListOfferingsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/client/#get_paginator)
         """
 
     @overload
```

### Comparing `mypy-boto3-mediaconnect-1.26.0.post1/mypy_boto3_mediaconnect/client.pyi` & `mypy-boto3-mediaconnect-1.26.113/mypy_boto3_mediaconnect/client.pyi`

 * *Files 26% similar despite different names*

```diff
@@ -14,62 +14,102 @@
     ```
 """
 import sys
 from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
-from .literals import EntitlementStatusType, MediaStreamTypeType, ProtocolType
+from .literals import (
+    BridgePlacementType,
+    DesiredStateType,
+    EntitlementStatusType,
+    MediaStreamTypeType,
+    ProtocolType,
+)
 from .paginator import (
+    ListBridgesPaginator,
     ListEntitlementsPaginator,
     ListFlowsPaginator,
+    ListGatewayInstancesPaginator,
+    ListGatewaysPaginator,
     ListOfferingsPaginator,
     ListReservationsPaginator,
 )
 from .type_defs import (
+    AddBridgeOutputRequestTypeDef,
+    AddBridgeOutputsResponseTypeDef,
+    AddBridgeSourceRequestTypeDef,
+    AddBridgeSourcesResponseTypeDef,
+    AddEgressGatewayBridgeRequestTypeDef,
     AddFlowMediaStreamsResponseTypeDef,
     AddFlowOutputsResponseTypeDef,
     AddFlowSourcesResponseTypeDef,
     AddFlowVpcInterfacesResponseTypeDef,
+    AddIngressGatewayBridgeRequestTypeDef,
     AddMaintenanceTypeDef,
     AddMediaStreamRequestTypeDef,
     AddOutputRequestTypeDef,
+    CreateBridgeResponseTypeDef,
     CreateFlowResponseTypeDef,
+    CreateGatewayResponseTypeDef,
+    DeleteBridgeResponseTypeDef,
     DeleteFlowResponseTypeDef,
+    DeleteGatewayResponseTypeDef,
+    DeregisterGatewayInstanceResponseTypeDef,
+    DescribeBridgeResponseTypeDef,
     DescribeFlowResponseTypeDef,
+    DescribeGatewayInstanceResponseTypeDef,
+    DescribeGatewayResponseTypeDef,
     DescribeOfferingResponseTypeDef,
     DescribeReservationResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     FailoverConfigTypeDef,
+    GatewayNetworkTypeDef,
     GrantEntitlementRequestTypeDef,
     GrantFlowEntitlementsResponseTypeDef,
+    ListBridgesResponseTypeDef,
     ListEntitlementsResponseTypeDef,
     ListFlowsResponseTypeDef,
+    ListGatewayInstancesResponseTypeDef,
+    ListGatewaysResponseTypeDef,
     ListOfferingsResponseTypeDef,
     ListReservationsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     MediaStreamAttributesRequestTypeDef,
     MediaStreamOutputConfigurationRequestTypeDef,
     MediaStreamSourceConfigurationRequestTypeDef,
     PurchaseOfferingResponseTypeDef,
+    RemoveBridgeOutputResponseTypeDef,
+    RemoveBridgeSourceResponseTypeDef,
     RemoveFlowMediaStreamResponseTypeDef,
     RemoveFlowOutputResponseTypeDef,
     RemoveFlowSourceResponseTypeDef,
     RemoveFlowVpcInterfaceResponseTypeDef,
     RevokeFlowEntitlementResponseTypeDef,
     SetSourceRequestTypeDef,
     StartFlowResponseTypeDef,
     StopFlowResponseTypeDef,
+    UpdateBridgeFlowSourceRequestTypeDef,
+    UpdateBridgeNetworkOutputRequestTypeDef,
+    UpdateBridgeNetworkSourceRequestTypeDef,
+    UpdateBridgeOutputResponseTypeDef,
+    UpdateBridgeResponseTypeDef,
+    UpdateBridgeSourceResponseTypeDef,
+    UpdateBridgeStateResponseTypeDef,
+    UpdateEgressGatewayBridgeRequestTypeDef,
     UpdateEncryptionTypeDef,
     UpdateFailoverConfigTypeDef,
     UpdateFlowEntitlementResponseTypeDef,
     UpdateFlowMediaStreamResponseTypeDef,
     UpdateFlowOutputResponseTypeDef,
     UpdateFlowResponseTypeDef,
     UpdateFlowSourceResponseTypeDef,
+    UpdateGatewayBridgeSourceRequestTypeDef,
+    UpdateGatewayInstanceResponseTypeDef,
+    UpdateIngressGatewayBridgeRequestTypeDef,
     UpdateMaintenanceTypeDef,
     VpcInterfaceAttachmentTypeDef,
     VpcInterfaceRequestTypeDef,
 )
 from .waiter import FlowActiveWaiter, FlowDeletedWaiter, FlowStandbyWaiter
 
 if sys.version_info >= (3, 9):
@@ -86,15 +126,18 @@
         self.response: Dict[str, Any]
         self.operation_name: str
 
 class Exceptions:
     AddFlowOutputs420Exception: Type[BotocoreClientError]
     BadRequestException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
+    ConflictException: Type[BotocoreClientError]
+    CreateBridge420Exception: Type[BotocoreClientError]
     CreateFlow420Exception: Type[BotocoreClientError]
+    CreateGateway420Exception: Type[BotocoreClientError]
     ForbiddenException: Type[BotocoreClientError]
     GrantFlowEntitlements420Exception: Type[BotocoreClientError]
     InternalServerErrorException: Type[BotocoreClientError]
     NotFoundException: Type[BotocoreClientError]
     ServiceUnavailableException: Type[BotocoreClientError]
     TooManyRequestsException: Type[BotocoreClientError]
 
@@ -110,14 +153,32 @@
     def exceptions(self) -> Exceptions:
         """
         MediaConnectClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/client/#exceptions)
         """
+    def add_bridge_outputs(
+        self, *, BridgeArn: str, Outputs: Sequence[AddBridgeOutputRequestTypeDef]
+    ) -> AddBridgeOutputsResponseTypeDef:
+        """
+        Adds outputs to an existing bridge.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.add_bridge_outputs)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/client/#add_bridge_outputs)
+        """
+    def add_bridge_sources(
+        self, *, BridgeArn: str, Sources: Sequence[AddBridgeSourceRequestTypeDef]
+    ) -> AddBridgeSourcesResponseTypeDef:
+        """
+        Adds sources to an existing bridge.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.add_bridge_sources)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/client/#add_bridge_sources)
+        """
     def add_flow_media_streams(
         self, *, FlowArn: str, MediaStreams: Sequence[AddMediaStreamRequestTypeDef]
     ) -> AddFlowMediaStreamsResponseTypeDef:
         """
         Adds media streams to an existing flow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.add_flow_media_streams)
@@ -162,14 +223,31 @@
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/client/#close)
         """
+    def create_bridge(
+        self,
+        *,
+        Name: str,
+        PlacementArn: str,
+        Sources: Sequence[AddBridgeSourceRequestTypeDef],
+        EgressGatewayBridge: AddEgressGatewayBridgeRequestTypeDef = ...,
+        IngressGatewayBridge: AddIngressGatewayBridgeRequestTypeDef = ...,
+        Outputs: Sequence[AddBridgeOutputRequestTypeDef] = ...,
+        SourceFailoverConfig: FailoverConfigTypeDef = ...
+    ) -> CreateBridgeResponseTypeDef:
+        """
+        Creates a new bridge.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.create_bridge)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/client/#create_bridge)
+        """
     def create_flow(
         self,
         *,
         Name: str,
         AvailabilityZone: str = ...,
         Entitlements: Sequence[GrantEntitlementRequestTypeDef] = ...,
         MediaStreams: Sequence[AddMediaStreamRequestTypeDef] = ...,
@@ -182,28 +260,87 @@
     ) -> CreateFlowResponseTypeDef:
         """
         Creates a new flow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.create_flow)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/client/#create_flow)
         """
+    def create_gateway(
+        self,
+        *,
+        EgressCidrBlocks: Sequence[str],
+        Name: str,
+        Networks: Sequence[GatewayNetworkTypeDef]
+    ) -> CreateGatewayResponseTypeDef:
+        """
+        Creates a new gateway.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.create_gateway)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/client/#create_gateway)
+        """
+    def delete_bridge(self, *, BridgeArn: str) -> DeleteBridgeResponseTypeDef:
+        """
+        Deletes a bridge.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.delete_bridge)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/client/#delete_bridge)
+        """
     def delete_flow(self, *, FlowArn: str) -> DeleteFlowResponseTypeDef:
         """
         Deletes a flow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.delete_flow)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/client/#delete_flow)
         """
+    def delete_gateway(self, *, GatewayArn: str) -> DeleteGatewayResponseTypeDef:
+        """
+        Deletes a gateway.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.delete_gateway)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/client/#delete_gateway)
+        """
+    def deregister_gateway_instance(
+        self, *, GatewayInstanceArn: str, Force: bool = ...
+    ) -> DeregisterGatewayInstanceResponseTypeDef:
+        """
+        Deregisters an instance.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.deregister_gateway_instance)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/client/#deregister_gateway_instance)
+        """
+    def describe_bridge(self, *, BridgeArn: str) -> DescribeBridgeResponseTypeDef:
+        """
+        Displays the details of a bridge.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.describe_bridge)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/client/#describe_bridge)
+        """
     def describe_flow(self, *, FlowArn: str) -> DescribeFlowResponseTypeDef:
         """
         Displays the details of a flow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.describe_flow)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/client/#describe_flow)
         """
+    def describe_gateway(self, *, GatewayArn: str) -> DescribeGatewayResponseTypeDef:
+        """
+        Displays the details of a gateway.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.describe_gateway)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/client/#describe_gateway)
+        """
+    def describe_gateway_instance(
+        self, *, GatewayInstanceArn: str
+    ) -> DescribeGatewayInstanceResponseTypeDef:
+        """
+        Displays the details of an instance.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.describe_gateway_instance)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/client/#describe_gateway_instance)
+        """
     def describe_offering(self, *, OfferingArn: str) -> DescribeOfferingResponseTypeDef:
         """
         Displays the details of an offering.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.describe_offering)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/client/#describe_offering)
         """
@@ -232,14 +369,24 @@
     ) -> GrantFlowEntitlementsResponseTypeDef:
         """
         Grants entitlements to an existing flow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.grant_flow_entitlements)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/client/#grant_flow_entitlements)
         """
+    def list_bridges(
+        self, *, FilterArn: str = ..., MaxResults: int = ..., NextToken: str = ...
+    ) -> ListBridgesResponseTypeDef:
+        """
+        Displays a list of bridges that are associated with this account and an
+        optionally specified Arn.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.list_bridges)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/client/#list_bridges)
+        """
     def list_entitlements(
         self, *, MaxResults: int = ..., NextToken: str = ...
     ) -> ListEntitlementsResponseTypeDef:
         """
         Displays a list of all entitlements that have been granted to this account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.list_entitlements)
@@ -250,14 +397,32 @@
     ) -> ListFlowsResponseTypeDef:
         """
         Displays a list of flows that are associated with this account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.list_flows)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/client/#list_flows)
         """
+    def list_gateway_instances(
+        self, *, FilterArn: str = ..., MaxResults: int = ..., NextToken: str = ...
+    ) -> ListGatewayInstancesResponseTypeDef:
+        """
+        Displays a list of instances associated with the AWS account.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.list_gateway_instances)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/client/#list_gateway_instances)
+        """
+    def list_gateways(
+        self, *, MaxResults: int = ..., NextToken: str = ...
+    ) -> ListGatewaysResponseTypeDef:
+        """
+        Displays a list of gateways that are associated with this account.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.list_gateways)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/client/#list_gateways)
+        """
     def list_offerings(
         self, *, MaxResults: int = ..., NextToken: str = ...
     ) -> ListOfferingsResponseTypeDef:
         """
         Displays a list of all offerings that are available to this account in the
         current AWS Region.
 
@@ -287,14 +452,32 @@
     ) -> PurchaseOfferingResponseTypeDef:
         """
         Submits a request to purchase an offering.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.purchase_offering)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/client/#purchase_offering)
         """
+    def remove_bridge_output(
+        self, *, BridgeArn: str, OutputName: str
+    ) -> RemoveBridgeOutputResponseTypeDef:
+        """
+        Removes an output from a bridge.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.remove_bridge_output)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/client/#remove_bridge_output)
+        """
+    def remove_bridge_source(
+        self, *, BridgeArn: str, SourceName: str
+    ) -> RemoveBridgeSourceResponseTypeDef:
+        """
+        Removes a source from a bridge.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.remove_bridge_source)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/client/#remove_bridge_source)
+        """
     def remove_flow_media_stream(
         self, *, FlowArn: str, MediaStreamName: str
     ) -> RemoveFlowMediaStreamResponseTypeDef:
         """
         Removes a media stream from a flow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.remove_flow_media_stream)
@@ -364,14 +547,66 @@
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes specified tags from a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/client/#untag_resource)
         """
+    def update_bridge(
+        self,
+        *,
+        BridgeArn: str,
+        EgressGatewayBridge: UpdateEgressGatewayBridgeRequestTypeDef = ...,
+        IngressGatewayBridge: UpdateIngressGatewayBridgeRequestTypeDef = ...,
+        SourceFailoverConfig: UpdateFailoverConfigTypeDef = ...
+    ) -> UpdateBridgeResponseTypeDef:
+        """
+        Updates the bridge See also: [AWS API
+        Documentation](https://docs.aws.amazon.com/goto/WebAPI/mediaconnect-2018-11-14/UpdateBridge).
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.update_bridge)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/client/#update_bridge)
+        """
+    def update_bridge_output(
+        self,
+        *,
+        BridgeArn: str,
+        OutputName: str,
+        NetworkOutput: UpdateBridgeNetworkOutputRequestTypeDef = ...
+    ) -> UpdateBridgeOutputResponseTypeDef:
+        """
+        Updates an existing bridge output.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.update_bridge_output)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/client/#update_bridge_output)
+        """
+    def update_bridge_source(
+        self,
+        *,
+        BridgeArn: str,
+        SourceName: str,
+        FlowSource: UpdateBridgeFlowSourceRequestTypeDef = ...,
+        NetworkSource: UpdateBridgeNetworkSourceRequestTypeDef = ...
+    ) -> UpdateBridgeSourceResponseTypeDef:
+        """
+        Updates an existing bridge source.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.update_bridge_source)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/client/#update_bridge_source)
+        """
+    def update_bridge_state(
+        self, *, BridgeArn: str, DesiredState: DesiredStateType
+    ) -> UpdateBridgeStateResponseTypeDef:
+        """
+        Updates the bridge state See also: [AWS API
+        Documentation](https://docs.aws.amazon.com/goto/WebAPI/mediaconnect-2018-11-14/UpdateBridgeState).
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.update_bridge_state)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/client/#update_bridge_state)
+        """
     def update_flow(
         self,
         *,
         FlowArn: str,
         SourceFailoverConfig: UpdateFailoverConfigTypeDef = ...,
         Maintenance: UpdateMaintenanceTypeDef = ...
     ) -> UpdateFlowResponseTypeDef:
@@ -463,22 +698,38 @@
         Protocol: ProtocolType = ...,
         SenderControlPort: int = ...,
         SenderIpAddress: str = ...,
         SourceListenerAddress: str = ...,
         SourceListenerPort: int = ...,
         StreamId: str = ...,
         VpcInterfaceName: str = ...,
-        WhitelistCidr: str = ...
+        WhitelistCidr: str = ...,
+        GatewayBridgeSource: UpdateGatewayBridgeSourceRequestTypeDef = ...
     ) -> UpdateFlowSourceResponseTypeDef:
         """
         Updates the source of a flow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.update_flow_source)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/client/#update_flow_source)
         """
+    def update_gateway_instance(
+        self, *, GatewayInstanceArn: str, BridgePlacement: BridgePlacementType = ...
+    ) -> UpdateGatewayInstanceResponseTypeDef:
+        """
+        Updates the configuration of an existing Gateway Instance.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.update_gateway_instance)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/client/#update_gateway_instance)
+        """
+    @overload
+    def get_paginator(self, operation_name: Literal["list_bridges"]) -> ListBridgesPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/client/#get_paginator)
+        """
     @overload
     def get_paginator(
         self, operation_name: Literal["list_entitlements"]
     ) -> ListEntitlementsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/client/#get_paginator)
@@ -486,14 +737,28 @@
     @overload
     def get_paginator(self, operation_name: Literal["list_flows"]) -> ListFlowsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/client/#get_paginator)
         """
     @overload
+    def get_paginator(
+        self, operation_name: Literal["list_gateway_instances"]
+    ) -> ListGatewayInstancesPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/client/#get_paginator)
+        """
+    @overload
+    def get_paginator(self, operation_name: Literal["list_gateways"]) -> ListGatewaysPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/client/#get_paginator)
+        """
+    @overload
     def get_paginator(self, operation_name: Literal["list_offerings"]) -> ListOfferingsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/client/#get_paginator)
         """
     @overload
     def get_paginator(
```

### Comparing `mypy-boto3-mediaconnect-1.26.0.post1/mypy_boto3_mediaconnect/literals.py` & `mypy-boto3-mediaconnect-1.26.113/mypy_boto3_mediaconnect/literals.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,26 +17,35 @@
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 
 __all__ = (
     "AlgorithmType",
+    "BridgePlacementType",
+    "BridgeStateType",
     "ColorimetryType",
+    "ConnectionStatusType",
+    "DesiredStateType",
     "DurationUnitsType",
     "EncoderProfileType",
     "EncodingNameType",
     "EntitlementStatusType",
     "FailoverModeType",
     "FlowActiveWaiterName",
     "FlowDeletedWaiterName",
     "FlowStandbyWaiterName",
+    "GatewayStateType",
+    "InstanceStateType",
     "KeyTypeType",
+    "ListBridgesPaginatorName",
     "ListEntitlementsPaginatorName",
     "ListFlowsPaginatorName",
+    "ListGatewayInstancesPaginatorName",
+    "ListGatewaysPaginatorName",
     "ListOfferingsPaginatorName",
     "ListReservationsPaginatorName",
     "MaintenanceDayType",
     "MediaStreamTypeType",
     "NetworkInterfaceTypeType",
     "PriceUnitsType",
     "ProtocolType",
@@ -54,26 +63,55 @@
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
 
 AlgorithmType = Literal["aes128", "aes192", "aes256"]
+BridgePlacementType = Literal["AVAILABLE", "LOCKED"]
+BridgeStateType = Literal[
+    "ACTIVE",
+    "CREATING",
+    "DELETED",
+    "DELETING",
+    "DEPLOYING",
+    "STANDBY",
+    "STARTING",
+    "START_FAILED",
+    "START_PENDING",
+    "STOPPING",
+    "STOP_FAILED",
+    "UPDATING",
+]
 ColorimetryType = Literal["BT2020", "BT2100", "BT601", "BT709", "ST2065-1", "ST2065-3", "XYZ"]
+ConnectionStatusType = Literal["CONNECTED", "DISCONNECTED"]
+DesiredStateType = Literal["ACTIVE", "DELETED", "STANDBY"]
 DurationUnitsType = Literal["MONTHS"]
 EncoderProfileType = Literal["high", "main"]
 EncodingNameType = Literal["jxsv", "pcm", "raw", "smpte291"]
 EntitlementStatusType = Literal["DISABLED", "ENABLED"]
 FailoverModeType = Literal["FAILOVER", "MERGE"]
 FlowActiveWaiterName = Literal["flow_active"]
 FlowDeletedWaiterName = Literal["flow_deleted"]
 FlowStandbyWaiterName = Literal["flow_standby"]
+GatewayStateType = Literal["ACTIVE", "CREATING", "DELETED", "DELETING", "ERROR", "UPDATING"]
+InstanceStateType = Literal[
+    "ACTIVE",
+    "DEREGISTERED",
+    "DEREGISTERING",
+    "DEREGISTRATION_ERROR",
+    "REGISTERING",
+    "REGISTRATION_ERROR",
+]
 KeyTypeType = Literal["speke", "srt-password", "static-key"]
+ListBridgesPaginatorName = Literal["list_bridges"]
 ListEntitlementsPaginatorName = Literal["list_entitlements"]
 ListFlowsPaginatorName = Literal["list_flows"]
+ListGatewayInstancesPaginatorName = Literal["list_gateway_instances"]
+ListGatewaysPaginatorName = Literal["list_gateways"]
 ListOfferingsPaginatorName = Literal["list_offerings"]
 ListReservationsPaginatorName = Literal["list_reservations"]
 MaintenanceDayType = Literal[
     "Friday", "Monday", "Saturday", "Sunday", "Thursday", "Tuesday", "Wednesday"
 ]
 MediaStreamTypeType = Literal["ancillary-data", "audio", "video"]
 NetworkInterfaceTypeType = Literal["efa", "ena"]
@@ -83,14 +121,15 @@
     "fujitsu-qos",
     "rist",
     "rtp",
     "rtp-fec",
     "srt-caller",
     "srt-listener",
     "st2110-jpegxs",
+    "udp",
     "zixi-pull",
     "zixi-push",
 ]
 RangeType = Literal["FULL", "FULLPROTECT", "NARROW"]
 ReservationStateType = Literal["ACTIVE", "CANCELED", "EXPIRED", "PROCESSING"]
 ResourceTypeType = Literal["Mbps_Outbound_Bandwidth"]
 ScanModeType = Literal["interlace", "progressive", "progressive-segmented-frame"]
@@ -121,14 +160,15 @@
     "application-autoscaling",
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
+    "arc-zonal-shift",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "backup",
     "backup-gateway",
     "backupstorage",
@@ -138,27 +178,31 @@
     "budgets",
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
+    "chime-sdk-voice",
+    "cleanrooms",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
+    "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
+    "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -187,14 +231,15 @@
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
     "docdb",
+    "docdb-elastic",
     "drs",
     "ds",
     "dynamodb",
     "dynamodbstreams",
     "ebs",
     "ec2",
     "ec2-instance-connect",
@@ -239,51 +284,57 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
+    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
+    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
     "iotfleetwise",
     "iotsecuretunneling",
     "iotsitewise",
     "iotthingsgraph",
     "iottwinmaker",
     "iotwireless",
     "ivs",
+    "ivs-realtime",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
+    "kendra-ranking",
     "keyspaces",
     "kinesis",
     "kinesis-video-archived-media",
     "kinesis-video-media",
     "kinesis-video-signaling",
+    "kinesis-video-webrtc-storage",
     "kinesisanalytics",
     "kinesisanalyticsv2",
     "kinesisvideo",
     "kms",
     "lakeformation",
     "lambda",
     "lex-models",
     "lex-runtime",
     "lexv2-models",
     "lexv2-runtime",
     "license-manager",
+    "license-manager-linux-subscriptions",
     "license-manager-user-subscriptions",
     "lightsail",
     "location",
     "logs",
     "lookoutequipment",
     "lookoutmetrics",
     "lookoutvision",
@@ -315,28 +366,32 @@
     "mq",
     "mturk",
     "mwaa",
     "neptune",
     "network-firewall",
     "networkmanager",
     "nimble",
+    "oam",
+    "omics",
     "opensearch",
+    "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
     "outposts",
     "panorama",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
     "pinpoint-email",
     "pinpoint-sms-voice",
     "pinpoint-sms-voice-v2",
+    "pipes",
     "polly",
     "pricing",
     "privatenetworks",
     "proton",
     "qldb",
     "qldb-session",
     "quicksight",
@@ -345,14 +400,15 @@
     "rds",
     "rds-data",
     "redshift",
     "redshift-data",
     "redshift-serverless",
     "rekognition",
     "resiliencehub",
+    "resource-explorer-2",
     "resource-groups",
     "resourcegroupstaggingapi",
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
@@ -363,55 +419,63 @@
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
     "sagemaker-edge",
     "sagemaker-featurestore-runtime",
+    "sagemaker-geospatial",
+    "sagemaker-metrics",
     "sagemaker-runtime",
     "savingsplans",
+    "scheduler",
     "schemas",
     "sdb",
     "secretsmanager",
     "securityhub",
+    "securitylake",
     "serverlessrepo",
     "service-quotas",
     "servicecatalog",
     "servicecatalog-appregistry",
     "servicediscovery",
     "ses",
     "sesv2",
     "shield",
     "signer",
+    "simspaceweaver",
     "sms",
     "sms-voice",
     "snow-device-management",
     "snowball",
     "sns",
     "sqs",
     "ssm",
     "ssm-contacts",
     "ssm-incidents",
+    "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
+    "tnb",
     "transcribe",
     "transfer",
     "translate",
     "voice-id",
+    "vpc-lattice",
     "waf",
     "waf-regional",
     "wafv2",
     "wellarchitected",
     "wisdom",
     "workdocs",
     "worklink",
@@ -429,15 +493,23 @@
     "glacier",
     "iam",
     "opsworks",
     "s3",
     "sns",
     "sqs",
 ]
-PaginatorName = Literal["list_entitlements", "list_flows", "list_offerings", "list_reservations"]
+PaginatorName = Literal[
+    "list_bridges",
+    "list_entitlements",
+    "list_flows",
+    "list_gateway_instances",
+    "list_gateways",
+    "list_offerings",
+    "list_reservations",
+]
 WaiterName = Literal["flow_active", "flow_deleted", "flow_standby"]
 RegionName = Literal[
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-south-1",
     "ap-southeast-1",
```

### Comparing `mypy-boto3-mediaconnect-1.26.0.post1/mypy_boto3_mediaconnect/literals.pyi` & `mypy-boto3-mediaconnect-1.26.113/mypy_boto3_mediaconnect/literals.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -16,26 +16,35 @@
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 __all__ = (
     "AlgorithmType",
+    "BridgePlacementType",
+    "BridgeStateType",
     "ColorimetryType",
+    "ConnectionStatusType",
+    "DesiredStateType",
     "DurationUnitsType",
     "EncoderProfileType",
     "EncodingNameType",
     "EntitlementStatusType",
     "FailoverModeType",
     "FlowActiveWaiterName",
     "FlowDeletedWaiterName",
     "FlowStandbyWaiterName",
+    "GatewayStateType",
+    "InstanceStateType",
     "KeyTypeType",
+    "ListBridgesPaginatorName",
     "ListEntitlementsPaginatorName",
     "ListFlowsPaginatorName",
+    "ListGatewayInstancesPaginatorName",
+    "ListGatewaysPaginatorName",
     "ListOfferingsPaginatorName",
     "ListReservationsPaginatorName",
     "MaintenanceDayType",
     "MediaStreamTypeType",
     "NetworkInterfaceTypeType",
     "PriceUnitsType",
     "ProtocolType",
@@ -52,26 +61,55 @@
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
 AlgorithmType = Literal["aes128", "aes192", "aes256"]
+BridgePlacementType = Literal["AVAILABLE", "LOCKED"]
+BridgeStateType = Literal[
+    "ACTIVE",
+    "CREATING",
+    "DELETED",
+    "DELETING",
+    "DEPLOYING",
+    "STANDBY",
+    "STARTING",
+    "START_FAILED",
+    "START_PENDING",
+    "STOPPING",
+    "STOP_FAILED",
+    "UPDATING",
+]
 ColorimetryType = Literal["BT2020", "BT2100", "BT601", "BT709", "ST2065-1", "ST2065-3", "XYZ"]
+ConnectionStatusType = Literal["CONNECTED", "DISCONNECTED"]
+DesiredStateType = Literal["ACTIVE", "DELETED", "STANDBY"]
 DurationUnitsType = Literal["MONTHS"]
 EncoderProfileType = Literal["high", "main"]
 EncodingNameType = Literal["jxsv", "pcm", "raw", "smpte291"]
 EntitlementStatusType = Literal["DISABLED", "ENABLED"]
 FailoverModeType = Literal["FAILOVER", "MERGE"]
 FlowActiveWaiterName = Literal["flow_active"]
 FlowDeletedWaiterName = Literal["flow_deleted"]
 FlowStandbyWaiterName = Literal["flow_standby"]
+GatewayStateType = Literal["ACTIVE", "CREATING", "DELETED", "DELETING", "ERROR", "UPDATING"]
+InstanceStateType = Literal[
+    "ACTIVE",
+    "DEREGISTERED",
+    "DEREGISTERING",
+    "DEREGISTRATION_ERROR",
+    "REGISTERING",
+    "REGISTRATION_ERROR",
+]
 KeyTypeType = Literal["speke", "srt-password", "static-key"]
+ListBridgesPaginatorName = Literal["list_bridges"]
 ListEntitlementsPaginatorName = Literal["list_entitlements"]
 ListFlowsPaginatorName = Literal["list_flows"]
+ListGatewayInstancesPaginatorName = Literal["list_gateway_instances"]
+ListGatewaysPaginatorName = Literal["list_gateways"]
 ListOfferingsPaginatorName = Literal["list_offerings"]
 ListReservationsPaginatorName = Literal["list_reservations"]
 MaintenanceDayType = Literal[
     "Friday", "Monday", "Saturday", "Sunday", "Thursday", "Tuesday", "Wednesday"
 ]
 MediaStreamTypeType = Literal["ancillary-data", "audio", "video"]
 NetworkInterfaceTypeType = Literal["efa", "ena"]
@@ -81,14 +119,15 @@
     "fujitsu-qos",
     "rist",
     "rtp",
     "rtp-fec",
     "srt-caller",
     "srt-listener",
     "st2110-jpegxs",
+    "udp",
     "zixi-pull",
     "zixi-push",
 ]
 RangeType = Literal["FULL", "FULLPROTECT", "NARROW"]
 ReservationStateType = Literal["ACTIVE", "CANCELED", "EXPIRED", "PROCESSING"]
 ResourceTypeType = Literal["Mbps_Outbound_Bandwidth"]
 ScanModeType = Literal["interlace", "progressive", "progressive-segmented-frame"]
@@ -119,14 +158,15 @@
     "application-autoscaling",
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
+    "arc-zonal-shift",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "backup",
     "backup-gateway",
     "backupstorage",
@@ -136,27 +176,31 @@
     "budgets",
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
+    "chime-sdk-voice",
+    "cleanrooms",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
+    "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
+    "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -185,14 +229,15 @@
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
     "docdb",
+    "docdb-elastic",
     "drs",
     "ds",
     "dynamodb",
     "dynamodbstreams",
     "ebs",
     "ec2",
     "ec2-instance-connect",
@@ -237,51 +282,57 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
+    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
+    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
     "iotfleetwise",
     "iotsecuretunneling",
     "iotsitewise",
     "iotthingsgraph",
     "iottwinmaker",
     "iotwireless",
     "ivs",
+    "ivs-realtime",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
+    "kendra-ranking",
     "keyspaces",
     "kinesis",
     "kinesis-video-archived-media",
     "kinesis-video-media",
     "kinesis-video-signaling",
+    "kinesis-video-webrtc-storage",
     "kinesisanalytics",
     "kinesisanalyticsv2",
     "kinesisvideo",
     "kms",
     "lakeformation",
     "lambda",
     "lex-models",
     "lex-runtime",
     "lexv2-models",
     "lexv2-runtime",
     "license-manager",
+    "license-manager-linux-subscriptions",
     "license-manager-user-subscriptions",
     "lightsail",
     "location",
     "logs",
     "lookoutequipment",
     "lookoutmetrics",
     "lookoutvision",
@@ -313,28 +364,32 @@
     "mq",
     "mturk",
     "mwaa",
     "neptune",
     "network-firewall",
     "networkmanager",
     "nimble",
+    "oam",
+    "omics",
     "opensearch",
+    "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
     "outposts",
     "panorama",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
     "pinpoint-email",
     "pinpoint-sms-voice",
     "pinpoint-sms-voice-v2",
+    "pipes",
     "polly",
     "pricing",
     "privatenetworks",
     "proton",
     "qldb",
     "qldb-session",
     "quicksight",
@@ -343,14 +398,15 @@
     "rds",
     "rds-data",
     "redshift",
     "redshift-data",
     "redshift-serverless",
     "rekognition",
     "resiliencehub",
+    "resource-explorer-2",
     "resource-groups",
     "resourcegroupstaggingapi",
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
@@ -361,55 +417,63 @@
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
     "sagemaker-edge",
     "sagemaker-featurestore-runtime",
+    "sagemaker-geospatial",
+    "sagemaker-metrics",
     "sagemaker-runtime",
     "savingsplans",
+    "scheduler",
     "schemas",
     "sdb",
     "secretsmanager",
     "securityhub",
+    "securitylake",
     "serverlessrepo",
     "service-quotas",
     "servicecatalog",
     "servicecatalog-appregistry",
     "servicediscovery",
     "ses",
     "sesv2",
     "shield",
     "signer",
+    "simspaceweaver",
     "sms",
     "sms-voice",
     "snow-device-management",
     "snowball",
     "sns",
     "sqs",
     "ssm",
     "ssm-contacts",
     "ssm-incidents",
+    "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
+    "tnb",
     "transcribe",
     "transfer",
     "translate",
     "voice-id",
+    "vpc-lattice",
     "waf",
     "waf-regional",
     "wafv2",
     "wellarchitected",
     "wisdom",
     "workdocs",
     "worklink",
@@ -427,15 +491,23 @@
     "glacier",
     "iam",
     "opsworks",
     "s3",
     "sns",
     "sqs",
 ]
-PaginatorName = Literal["list_entitlements", "list_flows", "list_offerings", "list_reservations"]
+PaginatorName = Literal[
+    "list_bridges",
+    "list_entitlements",
+    "list_flows",
+    "list_gateway_instances",
+    "list_gateways",
+    "list_offerings",
+    "list_reservations",
+]
 WaiterName = Literal["flow_active", "flow_deleted", "flow_standby"]
 RegionName = Literal[
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-south-1",
     "ap-southeast-1",
```

### Comparing `mypy-boto3-mediaconnect-1.26.0.post1/mypy_boto3_mediaconnect/type_defs.py` & `mypy-boto3-mediaconnect-1.26.113/mypy_boto3_mediaconnect/type_defs.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,29 +2,35 @@
 Type annotations for mediaconnect service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_mediaconnect.type_defs import ResponseMetadataTypeDef
+    from mypy_boto3_mediaconnect.type_defs import VpcInterfaceAttachmentTypeDef
 
-    data: ResponseMetadataTypeDef = {...}
+    data: VpcInterfaceAttachmentTypeDef = {...}
     ```
 """
 import sys
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     AlgorithmType,
+    BridgePlacementType,
+    BridgeStateType,
     ColorimetryType,
+    ConnectionStatusType,
+    DesiredStateType,
     EncoderProfileType,
     EncodingNameType,
     EntitlementStatusType,
     FailoverModeType,
+    GatewayStateType,
+    InstanceStateType,
     KeyTypeType,
     MaintenanceDayType,
     MediaStreamTypeType,
     NetworkInterfaceTypeType,
     ProtocolType,
     RangeType,
     ReservationStateType,
@@ -42,139 +48,251 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
+    "VpcInterfaceAttachmentTypeDef",
+    "AddBridgeNetworkOutputRequestTypeDef",
+    "AddBridgeNetworkSourceRequestTypeDef",
     "ResponseMetadataTypeDef",
+    "AddEgressGatewayBridgeRequestTypeDef",
     "VpcInterfaceRequestTypeDef",
     "VpcInterfaceTypeDef",
+    "AddIngressGatewayBridgeRequestTypeDef",
     "AddMaintenanceTypeDef",
     "EncryptionTypeDef",
-    "VpcInterfaceAttachmentTypeDef",
+    "BridgeFlowOutputTypeDef",
+    "BridgeNetworkOutputTypeDef",
+    "BridgeNetworkSourceTypeDef",
+    "EgressGatewayBridgeTypeDef",
+    "IngressGatewayBridgeTypeDef",
+    "MessageDetailTypeDef",
+    "GatewayNetworkTypeDef",
+    "DeleteBridgeRequestRequestTypeDef",
     "DeleteFlowRequestRequestTypeDef",
+    "DeleteGatewayRequestRequestTypeDef",
+    "DeregisterGatewayInstanceRequestRequestTypeDef",
+    "DescribeBridgeRequestRequestTypeDef",
     "WaiterConfigTypeDef",
     "DescribeFlowRequestRequestTypeDef",
     "MessagesTypeDef",
+    "DescribeGatewayInstanceRequestRequestTypeDef",
+    "DescribeGatewayRequestRequestTypeDef",
     "DescribeOfferingRequestRequestTypeDef",
     "DescribeReservationRequestRequestTypeDef",
     "InterfaceRequestTypeDef",
     "InterfaceTypeDef",
     "EncodingParametersRequestTypeDef",
     "EncodingParametersTypeDef",
     "SourcePriorityTypeDef",
     "MaintenanceTypeDef",
     "FmtpRequestTypeDef",
     "FmtpTypeDef",
     "PaginatorConfigTypeDef",
+    "ListBridgesRequestRequestTypeDef",
+    "ListedBridgeTypeDef",
     "ListEntitlementsRequestRequestTypeDef",
     "ListedEntitlementTypeDef",
     "ListFlowsRequestRequestTypeDef",
+    "ListGatewayInstancesRequestRequestTypeDef",
+    "ListedGatewayInstanceTypeDef",
+    "ListGatewaysRequestRequestTypeDef",
+    "ListedGatewayTypeDef",
     "ListOfferingsRequestRequestTypeDef",
     "ListReservationsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ResourceSpecificationTypeDef",
     "TransportTypeDef",
     "PurchaseOfferingRequestRequestTypeDef",
+    "RemoveBridgeOutputRequestRequestTypeDef",
+    "RemoveBridgeSourceRequestRequestTypeDef",
     "RemoveFlowMediaStreamRequestRequestTypeDef",
     "RemoveFlowOutputRequestRequestTypeDef",
     "RemoveFlowSourceRequestRequestTypeDef",
     "RemoveFlowVpcInterfaceRequestRequestTypeDef",
     "RevokeFlowEntitlementRequestRequestTypeDef",
     "StartFlowRequestRequestTypeDef",
     "StopFlowRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "UpdateBridgeNetworkOutputRequestTypeDef",
+    "UpdateBridgeNetworkSourceRequestTypeDef",
+    "UpdateEgressGatewayBridgeRequestTypeDef",
+    "UpdateIngressGatewayBridgeRequestTypeDef",
+    "UpdateBridgeStateRequestRequestTypeDef",
     "UpdateEncryptionTypeDef",
     "UpdateMaintenanceTypeDef",
+    "UpdateGatewayInstanceRequestRequestTypeDef",
+    "AddBridgeFlowSourceRequestTypeDef",
+    "BridgeFlowSourceTypeDef",
+    "GatewayBridgeSourceTypeDef",
+    "SetGatewayBridgeSourceRequestTypeDef",
+    "UpdateBridgeFlowSourceRequestTypeDef",
+    "UpdateGatewayBridgeSourceRequestTypeDef",
+    "AddBridgeOutputRequestTypeDef",
+    "DeleteBridgeResponseTypeDef",
     "DeleteFlowResponseTypeDef",
+    "DeleteGatewayResponseTypeDef",
+    "DeregisterGatewayInstanceResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
     "ListTagsForResourceResponseTypeDef",
+    "RemoveBridgeOutputResponseTypeDef",
+    "RemoveBridgeSourceResponseTypeDef",
     "RemoveFlowMediaStreamResponseTypeDef",
     "RemoveFlowOutputResponseTypeDef",
     "RemoveFlowSourceResponseTypeDef",
     "RemoveFlowVpcInterfaceResponseTypeDef",
     "RevokeFlowEntitlementResponseTypeDef",
     "StartFlowResponseTypeDef",
     "StopFlowResponseTypeDef",
+    "UpdateBridgeStateResponseTypeDef",
+    "UpdateGatewayInstanceResponseTypeDef",
     "AddFlowVpcInterfacesRequestRequestTypeDef",
     "AddFlowVpcInterfacesResponseTypeDef",
     "EntitlementTypeDef",
     "GrantEntitlementRequestTypeDef",
+    "BridgeOutputTypeDef",
+    "GatewayInstanceTypeDef",
+    "CreateGatewayRequestRequestTypeDef",
+    "GatewayTypeDef",
     "DescribeFlowRequestFlowActiveWaitTypeDef",
     "DescribeFlowRequestFlowDeletedWaitTypeDef",
     "DescribeFlowRequestFlowStandbyWaitTypeDef",
     "DestinationConfigurationRequestTypeDef",
     "InputConfigurationRequestTypeDef",
     "DestinationConfigurationTypeDef",
     "InputConfigurationTypeDef",
     "FailoverConfigTypeDef",
     "UpdateFailoverConfigTypeDef",
     "ListedFlowTypeDef",
     "MediaStreamAttributesRequestTypeDef",
     "MediaStreamAttributesTypeDef",
+    "ListBridgesRequestListBridgesPaginateTypeDef",
     "ListEntitlementsRequestListEntitlementsPaginateTypeDef",
     "ListFlowsRequestListFlowsPaginateTypeDef",
+    "ListGatewayInstancesRequestListGatewayInstancesPaginateTypeDef",
+    "ListGatewaysRequestListGatewaysPaginateTypeDef",
     "ListOfferingsRequestListOfferingsPaginateTypeDef",
     "ListReservationsRequestListReservationsPaginateTypeDef",
+    "ListBridgesResponseTypeDef",
     "ListEntitlementsResponseTypeDef",
+    "ListGatewayInstancesResponseTypeDef",
+    "ListGatewaysResponseTypeDef",
     "OfferingTypeDef",
     "ReservationTypeDef",
+    "UpdateBridgeOutputRequestRequestTypeDef",
     "UpdateFlowEntitlementRequestRequestTypeDef",
+    "AddBridgeSourceRequestTypeDef",
+    "BridgeSourceTypeDef",
+    "UpdateBridgeSourceRequestRequestTypeDef",
+    "AddBridgeOutputsRequestRequestTypeDef",
     "GrantFlowEntitlementsResponseTypeDef",
     "UpdateFlowEntitlementResponseTypeDef",
     "GrantFlowEntitlementsRequestRequestTypeDef",
+    "AddBridgeOutputsResponseTypeDef",
+    "UpdateBridgeOutputResponseTypeDef",
+    "DescribeGatewayInstanceResponseTypeDef",
+    "CreateGatewayResponseTypeDef",
+    "DescribeGatewayResponseTypeDef",
     "MediaStreamOutputConfigurationRequestTypeDef",
     "MediaStreamSourceConfigurationRequestTypeDef",
     "MediaStreamOutputConfigurationTypeDef",
     "MediaStreamSourceConfigurationTypeDef",
+    "UpdateBridgeRequestRequestTypeDef",
     "UpdateFlowRequestRequestTypeDef",
     "ListFlowsResponseTypeDef",
     "AddMediaStreamRequestTypeDef",
     "UpdateFlowMediaStreamRequestRequestTypeDef",
     "MediaStreamTypeDef",
     "DescribeOfferingResponseTypeDef",
     "ListOfferingsResponseTypeDef",
     "DescribeReservationResponseTypeDef",
     "ListReservationsResponseTypeDef",
     "PurchaseOfferingResponseTypeDef",
+    "AddBridgeSourcesRequestRequestTypeDef",
+    "CreateBridgeRequestRequestTypeDef",
+    "AddBridgeSourcesResponseTypeDef",
+    "BridgeTypeDef",
+    "UpdateBridgeSourceResponseTypeDef",
     "AddOutputRequestTypeDef",
     "UpdateFlowOutputRequestRequestTypeDef",
     "SetSourceRequestTypeDef",
     "UpdateFlowSourceRequestRequestTypeDef",
     "OutputTypeDef",
     "SourceTypeDef",
     "AddFlowMediaStreamsRequestRequestTypeDef",
     "AddFlowMediaStreamsResponseTypeDef",
     "UpdateFlowMediaStreamResponseTypeDef",
+    "CreateBridgeResponseTypeDef",
+    "DescribeBridgeResponseTypeDef",
+    "UpdateBridgeResponseTypeDef",
     "AddFlowOutputsRequestRequestTypeDef",
     "AddFlowSourcesRequestRequestTypeDef",
     "CreateFlowRequestRequestTypeDef",
     "AddFlowOutputsResponseTypeDef",
     "UpdateFlowOutputResponseTypeDef",
     "AddFlowSourcesResponseTypeDef",
     "FlowTypeDef",
     "UpdateFlowSourceResponseTypeDef",
     "CreateFlowResponseTypeDef",
     "DescribeFlowResponseTypeDef",
     "UpdateFlowResponseTypeDef",
 )
 
+VpcInterfaceAttachmentTypeDef = TypedDict(
+    "VpcInterfaceAttachmentTypeDef",
+    {
+        "VpcInterfaceName": str,
+    },
+    total=False,
+)
+
+AddBridgeNetworkOutputRequestTypeDef = TypedDict(
+    "AddBridgeNetworkOutputRequestTypeDef",
+    {
+        "IpAddress": str,
+        "Name": str,
+        "NetworkName": str,
+        "Port": int,
+        "Protocol": ProtocolType,
+        "Ttl": int,
+    },
+)
+
+AddBridgeNetworkSourceRequestTypeDef = TypedDict(
+    "AddBridgeNetworkSourceRequestTypeDef",
+    {
+        "MulticastIp": str,
+        "Name": str,
+        "NetworkName": str,
+        "Port": int,
+        "Protocol": ProtocolType,
+    },
+)
+
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
+AddEgressGatewayBridgeRequestTypeDef = TypedDict(
+    "AddEgressGatewayBridgeRequestTypeDef",
+    {
+        "MaxBitrate": int,
+    },
+)
+
 _RequiredVpcInterfaceRequestTypeDef = TypedDict(
     "_RequiredVpcInterfaceRequestTypeDef",
     {
         "Name": str,
         "RoleArn": str,
         "SecurityGroupIds": Sequence[str],
         "SubnetId": str,
@@ -203,14 +321,22 @@
         "NetworkInterfaceType": NetworkInterfaceTypeType,
         "RoleArn": str,
         "SecurityGroupIds": List[str],
         "SubnetId": str,
     },
 )
 
+AddIngressGatewayBridgeRequestTypeDef = TypedDict(
+    "AddIngressGatewayBridgeRequestTypeDef",
+    {
+        "MaxBitrate": int,
+        "MaxOutputs": int,
+    },
+)
+
 AddMaintenanceTypeDef = TypedDict(
     "AddMaintenanceTypeDef",
     {
         "MaintenanceDay": MaintenanceDayType,
         "MaintenanceStartHour": str,
     },
 )
@@ -237,29 +363,167 @@
 )
 
 
 class EncryptionTypeDef(_RequiredEncryptionTypeDef, _OptionalEncryptionTypeDef):
     pass
 
 
-VpcInterfaceAttachmentTypeDef = TypedDict(
-    "VpcInterfaceAttachmentTypeDef",
+BridgeFlowOutputTypeDef = TypedDict(
+    "BridgeFlowOutputTypeDef",
     {
-        "VpcInterfaceName": str,
+        "FlowArn": str,
+        "FlowSourceArn": str,
+        "Name": str,
+    },
+)
+
+BridgeNetworkOutputTypeDef = TypedDict(
+    "BridgeNetworkOutputTypeDef",
+    {
+        "IpAddress": str,
+        "Name": str,
+        "NetworkName": str,
+        "Port": int,
+        "Protocol": ProtocolType,
+        "Ttl": int,
+    },
+)
+
+BridgeNetworkSourceTypeDef = TypedDict(
+    "BridgeNetworkSourceTypeDef",
+    {
+        "MulticastIp": str,
+        "Name": str,
+        "NetworkName": str,
+        "Port": int,
+        "Protocol": ProtocolType,
+    },
+)
+
+_RequiredEgressGatewayBridgeTypeDef = TypedDict(
+    "_RequiredEgressGatewayBridgeTypeDef",
+    {
+        "MaxBitrate": int,
+    },
+)
+_OptionalEgressGatewayBridgeTypeDef = TypedDict(
+    "_OptionalEgressGatewayBridgeTypeDef",
+    {
+        "InstanceId": str,
+    },
+    total=False,
+)
+
+
+class EgressGatewayBridgeTypeDef(
+    _RequiredEgressGatewayBridgeTypeDef, _OptionalEgressGatewayBridgeTypeDef
+):
+    pass
+
+
+_RequiredIngressGatewayBridgeTypeDef = TypedDict(
+    "_RequiredIngressGatewayBridgeTypeDef",
+    {
+        "MaxBitrate": int,
+        "MaxOutputs": int,
+    },
+)
+_OptionalIngressGatewayBridgeTypeDef = TypedDict(
+    "_OptionalIngressGatewayBridgeTypeDef",
+    {
+        "InstanceId": str,
+    },
+    total=False,
+)
+
+
+class IngressGatewayBridgeTypeDef(
+    _RequiredIngressGatewayBridgeTypeDef, _OptionalIngressGatewayBridgeTypeDef
+):
+    pass
+
+
+_RequiredMessageDetailTypeDef = TypedDict(
+    "_RequiredMessageDetailTypeDef",
+    {
+        "Code": str,
+        "Message": str,
+    },
+)
+_OptionalMessageDetailTypeDef = TypedDict(
+    "_OptionalMessageDetailTypeDef",
+    {
+        "ResourceName": str,
     },
     total=False,
 )
 
+
+class MessageDetailTypeDef(_RequiredMessageDetailTypeDef, _OptionalMessageDetailTypeDef):
+    pass
+
+
+GatewayNetworkTypeDef = TypedDict(
+    "GatewayNetworkTypeDef",
+    {
+        "CidrBlock": str,
+        "Name": str,
+    },
+)
+
+DeleteBridgeRequestRequestTypeDef = TypedDict(
+    "DeleteBridgeRequestRequestTypeDef",
+    {
+        "BridgeArn": str,
+    },
+)
+
 DeleteFlowRequestRequestTypeDef = TypedDict(
     "DeleteFlowRequestRequestTypeDef",
     {
         "FlowArn": str,
     },
 )
 
+DeleteGatewayRequestRequestTypeDef = TypedDict(
+    "DeleteGatewayRequestRequestTypeDef",
+    {
+        "GatewayArn": str,
+    },
+)
+
+_RequiredDeregisterGatewayInstanceRequestRequestTypeDef = TypedDict(
+    "_RequiredDeregisterGatewayInstanceRequestRequestTypeDef",
+    {
+        "GatewayInstanceArn": str,
+    },
+)
+_OptionalDeregisterGatewayInstanceRequestRequestTypeDef = TypedDict(
+    "_OptionalDeregisterGatewayInstanceRequestRequestTypeDef",
+    {
+        "Force": bool,
+    },
+    total=False,
+)
+
+
+class DeregisterGatewayInstanceRequestRequestTypeDef(
+    _RequiredDeregisterGatewayInstanceRequestRequestTypeDef,
+    _OptionalDeregisterGatewayInstanceRequestRequestTypeDef,
+):
+    pass
+
+
+DescribeBridgeRequestRequestTypeDef = TypedDict(
+    "DescribeBridgeRequestRequestTypeDef",
+    {
+        "BridgeArn": str,
+    },
+)
+
 WaiterConfigTypeDef = TypedDict(
     "WaiterConfigTypeDef",
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
@@ -275,14 +539,28 @@
 MessagesTypeDef = TypedDict(
     "MessagesTypeDef",
     {
         "Errors": List[str],
     },
 )
 
+DescribeGatewayInstanceRequestRequestTypeDef = TypedDict(
+    "DescribeGatewayInstanceRequestRequestTypeDef",
+    {
+        "GatewayInstanceArn": str,
+    },
+)
+
+DescribeGatewayRequestRequestTypeDef = TypedDict(
+    "DescribeGatewayRequestRequestTypeDef",
+    {
+        "GatewayArn": str,
+    },
+)
+
 DescribeOfferingRequestRequestTypeDef = TypedDict(
     "DescribeOfferingRequestRequestTypeDef",
     {
         "OfferingArn": str,
     },
 )
 
@@ -376,14 +654,35 @@
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
+ListBridgesRequestRequestTypeDef = TypedDict(
+    "ListBridgesRequestRequestTypeDef",
+    {
+        "FilterArn": str,
+        "MaxResults": int,
+        "NextToken": str,
+    },
+    total=False,
+)
+
+ListedBridgeTypeDef = TypedDict(
+    "ListedBridgeTypeDef",
+    {
+        "BridgeArn": str,
+        "BridgeState": BridgeStateType,
+        "BridgeType": str,
+        "Name": str,
+        "PlacementArn": str,
+    },
+)
+
 ListEntitlementsRequestRequestTypeDef = TypedDict(
     "ListEntitlementsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -416,14 +715,65 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+ListGatewayInstancesRequestRequestTypeDef = TypedDict(
+    "ListGatewayInstancesRequestRequestTypeDef",
+    {
+        "FilterArn": str,
+        "MaxResults": int,
+        "NextToken": str,
+    },
+    total=False,
+)
+
+_RequiredListedGatewayInstanceTypeDef = TypedDict(
+    "_RequiredListedGatewayInstanceTypeDef",
+    {
+        "GatewayArn": str,
+        "GatewayInstanceArn": str,
+        "InstanceId": str,
+    },
+)
+_OptionalListedGatewayInstanceTypeDef = TypedDict(
+    "_OptionalListedGatewayInstanceTypeDef",
+    {
+        "InstanceState": InstanceStateType,
+    },
+    total=False,
+)
+
+
+class ListedGatewayInstanceTypeDef(
+    _RequiredListedGatewayInstanceTypeDef, _OptionalListedGatewayInstanceTypeDef
+):
+    pass
+
+
+ListGatewaysRequestRequestTypeDef = TypedDict(
+    "ListGatewaysRequestRequestTypeDef",
+    {
+        "MaxResults": int,
+        "NextToken": str,
+    },
+    total=False,
+)
+
+ListedGatewayTypeDef = TypedDict(
+    "ListedGatewayTypeDef",
+    {
+        "GatewayArn": str,
+        "GatewayState": GatewayStateType,
+        "Name": str,
+    },
+)
+
 ListOfferingsRequestRequestTypeDef = TypedDict(
     "ListOfferingsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -501,14 +851,30 @@
     {
         "OfferingArn": str,
         "ReservationName": str,
         "Start": str,
     },
 )
 
+RemoveBridgeOutputRequestRequestTypeDef = TypedDict(
+    "RemoveBridgeOutputRequestRequestTypeDef",
+    {
+        "BridgeArn": str,
+        "OutputName": str,
+    },
+)
+
+RemoveBridgeSourceRequestRequestTypeDef = TypedDict(
+    "RemoveBridgeSourceRequestRequestTypeDef",
+    {
+        "BridgeArn": str,
+        "SourceName": str,
+    },
+)
+
 RemoveFlowMediaStreamRequestRequestTypeDef = TypedDict(
     "RemoveFlowMediaStreamRequestRequestTypeDef",
     {
         "FlowArn": str,
         "MediaStreamName": str,
     },
 )
@@ -571,14 +937,62 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
+UpdateBridgeNetworkOutputRequestTypeDef = TypedDict(
+    "UpdateBridgeNetworkOutputRequestTypeDef",
+    {
+        "IpAddress": str,
+        "NetworkName": str,
+        "Port": int,
+        "Protocol": ProtocolType,
+        "Ttl": int,
+    },
+    total=False,
+)
+
+UpdateBridgeNetworkSourceRequestTypeDef = TypedDict(
+    "UpdateBridgeNetworkSourceRequestTypeDef",
+    {
+        "MulticastIp": str,
+        "NetworkName": str,
+        "Port": int,
+        "Protocol": ProtocolType,
+    },
+    total=False,
+)
+
+UpdateEgressGatewayBridgeRequestTypeDef = TypedDict(
+    "UpdateEgressGatewayBridgeRequestTypeDef",
+    {
+        "MaxBitrate": int,
+    },
+    total=False,
+)
+
+UpdateIngressGatewayBridgeRequestTypeDef = TypedDict(
+    "UpdateIngressGatewayBridgeRequestTypeDef",
+    {
+        "MaxBitrate": int,
+        "MaxOutputs": int,
+    },
+    total=False,
+)
+
+UpdateBridgeStateRequestRequestTypeDef = TypedDict(
+    "UpdateBridgeStateRequestRequestTypeDef",
+    {
+        "BridgeArn": str,
+        "DesiredState": DesiredStateType,
+    },
+)
+
 UpdateEncryptionTypeDef = TypedDict(
     "UpdateEncryptionTypeDef",
     {
         "Algorithm": AlgorithmType,
         "ConstantInitializationVector": str,
         "DeviceId": str,
         "KeyType": KeyTypeType,
@@ -597,23 +1011,181 @@
         "MaintenanceDay": MaintenanceDayType,
         "MaintenanceScheduledDate": str,
         "MaintenanceStartHour": str,
     },
     total=False,
 )
 
+_RequiredUpdateGatewayInstanceRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateGatewayInstanceRequestRequestTypeDef",
+    {
+        "GatewayInstanceArn": str,
+    },
+)
+_OptionalUpdateGatewayInstanceRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateGatewayInstanceRequestRequestTypeDef",
+    {
+        "BridgePlacement": BridgePlacementType,
+    },
+    total=False,
+)
+
+
+class UpdateGatewayInstanceRequestRequestTypeDef(
+    _RequiredUpdateGatewayInstanceRequestRequestTypeDef,
+    _OptionalUpdateGatewayInstanceRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredAddBridgeFlowSourceRequestTypeDef = TypedDict(
+    "_RequiredAddBridgeFlowSourceRequestTypeDef",
+    {
+        "FlowArn": str,
+        "Name": str,
+    },
+)
+_OptionalAddBridgeFlowSourceRequestTypeDef = TypedDict(
+    "_OptionalAddBridgeFlowSourceRequestTypeDef",
+    {
+        "FlowVpcInterfaceAttachment": VpcInterfaceAttachmentTypeDef,
+    },
+    total=False,
+)
+
+
+class AddBridgeFlowSourceRequestTypeDef(
+    _RequiredAddBridgeFlowSourceRequestTypeDef, _OptionalAddBridgeFlowSourceRequestTypeDef
+):
+    pass
+
+
+_RequiredBridgeFlowSourceTypeDef = TypedDict(
+    "_RequiredBridgeFlowSourceTypeDef",
+    {
+        "FlowArn": str,
+        "Name": str,
+    },
+)
+_OptionalBridgeFlowSourceTypeDef = TypedDict(
+    "_OptionalBridgeFlowSourceTypeDef",
+    {
+        "FlowVpcInterfaceAttachment": VpcInterfaceAttachmentTypeDef,
+        "OutputArn": str,
+    },
+    total=False,
+)
+
+
+class BridgeFlowSourceTypeDef(_RequiredBridgeFlowSourceTypeDef, _OptionalBridgeFlowSourceTypeDef):
+    pass
+
+
+_RequiredGatewayBridgeSourceTypeDef = TypedDict(
+    "_RequiredGatewayBridgeSourceTypeDef",
+    {
+        "BridgeArn": str,
+    },
+)
+_OptionalGatewayBridgeSourceTypeDef = TypedDict(
+    "_OptionalGatewayBridgeSourceTypeDef",
+    {
+        "VpcInterfaceAttachment": VpcInterfaceAttachmentTypeDef,
+    },
+    total=False,
+)
+
+
+class GatewayBridgeSourceTypeDef(
+    _RequiredGatewayBridgeSourceTypeDef, _OptionalGatewayBridgeSourceTypeDef
+):
+    pass
+
+
+_RequiredSetGatewayBridgeSourceRequestTypeDef = TypedDict(
+    "_RequiredSetGatewayBridgeSourceRequestTypeDef",
+    {
+        "BridgeArn": str,
+    },
+)
+_OptionalSetGatewayBridgeSourceRequestTypeDef = TypedDict(
+    "_OptionalSetGatewayBridgeSourceRequestTypeDef",
+    {
+        "VpcInterfaceAttachment": VpcInterfaceAttachmentTypeDef,
+    },
+    total=False,
+)
+
+
+class SetGatewayBridgeSourceRequestTypeDef(
+    _RequiredSetGatewayBridgeSourceRequestTypeDef, _OptionalSetGatewayBridgeSourceRequestTypeDef
+):
+    pass
+
+
+UpdateBridgeFlowSourceRequestTypeDef = TypedDict(
+    "UpdateBridgeFlowSourceRequestTypeDef",
+    {
+        "FlowArn": str,
+        "FlowVpcInterfaceAttachment": VpcInterfaceAttachmentTypeDef,
+    },
+    total=False,
+)
+
+UpdateGatewayBridgeSourceRequestTypeDef = TypedDict(
+    "UpdateGatewayBridgeSourceRequestTypeDef",
+    {
+        "BridgeArn": str,
+        "VpcInterfaceAttachment": VpcInterfaceAttachmentTypeDef,
+    },
+    total=False,
+)
+
+AddBridgeOutputRequestTypeDef = TypedDict(
+    "AddBridgeOutputRequestTypeDef",
+    {
+        "NetworkOutput": AddBridgeNetworkOutputRequestTypeDef,
+    },
+    total=False,
+)
+
+DeleteBridgeResponseTypeDef = TypedDict(
+    "DeleteBridgeResponseTypeDef",
+    {
+        "BridgeArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DeleteFlowResponseTypeDef = TypedDict(
     "DeleteFlowResponseTypeDef",
     {
         "FlowArn": str,
         "Status": StatusType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DeleteGatewayResponseTypeDef = TypedDict(
+    "DeleteGatewayResponseTypeDef",
+    {
+        "GatewayArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeregisterGatewayInstanceResponseTypeDef = TypedDict(
+    "DeregisterGatewayInstanceResponseTypeDef",
+    {
+        "GatewayInstanceArn": str,
+        "InstanceState": InstanceStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 EmptyResponseMetadataTypeDef = TypedDict(
     "EmptyResponseMetadataTypeDef",
     {
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
@@ -621,14 +1193,32 @@
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+RemoveBridgeOutputResponseTypeDef = TypedDict(
+    "RemoveBridgeOutputResponseTypeDef",
+    {
+        "BridgeArn": str,
+        "OutputName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RemoveBridgeSourceResponseTypeDef = TypedDict(
+    "RemoveBridgeSourceResponseTypeDef",
+    {
+        "BridgeArn": str,
+        "SourceName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 RemoveFlowMediaStreamResponseTypeDef = TypedDict(
     "RemoveFlowMediaStreamResponseTypeDef",
     {
         "FlowArn": str,
         "MediaStreamName": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -685,14 +1275,32 @@
     {
         "FlowArn": str,
         "Status": StatusType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+UpdateBridgeStateResponseTypeDef = TypedDict(
+    "UpdateBridgeStateResponseTypeDef",
+    {
+        "BridgeArn": str,
+        "DesiredState": DesiredStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateGatewayInstanceResponseTypeDef = TypedDict(
+    "UpdateGatewayInstanceResponseTypeDef",
+    {
+        "BridgePlacement": BridgePlacementType,
+        "GatewayInstanceArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 AddFlowVpcInterfacesRequestRequestTypeDef = TypedDict(
     "AddFlowVpcInterfacesRequestRequestTypeDef",
     {
         "FlowArn": str,
         "VpcInterfaces": Sequence[VpcInterfaceRequestTypeDef],
     },
 )
@@ -751,14 +1359,80 @@
 
 class GrantEntitlementRequestTypeDef(
     _RequiredGrantEntitlementRequestTypeDef, _OptionalGrantEntitlementRequestTypeDef
 ):
     pass
 
 
+BridgeOutputTypeDef = TypedDict(
+    "BridgeOutputTypeDef",
+    {
+        "FlowOutput": BridgeFlowOutputTypeDef,
+        "NetworkOutput": BridgeNetworkOutputTypeDef,
+    },
+    total=False,
+)
+
+_RequiredGatewayInstanceTypeDef = TypedDict(
+    "_RequiredGatewayInstanceTypeDef",
+    {
+        "BridgePlacement": BridgePlacementType,
+        "ConnectionStatus": ConnectionStatusType,
+        "GatewayArn": str,
+        "GatewayInstanceArn": str,
+        "InstanceId": str,
+        "InstanceState": InstanceStateType,
+        "RunningBridgeCount": int,
+    },
+)
+_OptionalGatewayInstanceTypeDef = TypedDict(
+    "_OptionalGatewayInstanceTypeDef",
+    {
+        "InstanceMessages": List[MessageDetailTypeDef],
+    },
+    total=False,
+)
+
+
+class GatewayInstanceTypeDef(_RequiredGatewayInstanceTypeDef, _OptionalGatewayInstanceTypeDef):
+    pass
+
+
+CreateGatewayRequestRequestTypeDef = TypedDict(
+    "CreateGatewayRequestRequestTypeDef",
+    {
+        "EgressCidrBlocks": Sequence[str],
+        "Name": str,
+        "Networks": Sequence[GatewayNetworkTypeDef],
+    },
+)
+
+_RequiredGatewayTypeDef = TypedDict(
+    "_RequiredGatewayTypeDef",
+    {
+        "EgressCidrBlocks": List[str],
+        "GatewayArn": str,
+        "Name": str,
+        "Networks": List[GatewayNetworkTypeDef],
+    },
+)
+_OptionalGatewayTypeDef = TypedDict(
+    "_OptionalGatewayTypeDef",
+    {
+        "GatewayMessages": List[MessageDetailTypeDef],
+        "GatewayState": GatewayStateType,
+    },
+    total=False,
+)
+
+
+class GatewayTypeDef(_RequiredGatewayTypeDef, _OptionalGatewayTypeDef):
+    pass
+
+
 _RequiredDescribeFlowRequestFlowActiveWaitTypeDef = TypedDict(
     "_RequiredDescribeFlowRequestFlowActiveWaitTypeDef",
     {
         "FlowArn": str,
     },
 )
 _OptionalDescribeFlowRequestFlowActiveWaitTypeDef = TypedDict(
@@ -929,14 +1603,23 @@
 
 class MediaStreamAttributesTypeDef(
     _RequiredMediaStreamAttributesTypeDef, _OptionalMediaStreamAttributesTypeDef
 ):
     pass
 
 
+ListBridgesRequestListBridgesPaginateTypeDef = TypedDict(
+    "ListBridgesRequestListBridgesPaginateTypeDef",
+    {
+        "FilterArn": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 ListEntitlementsRequestListEntitlementsPaginateTypeDef = TypedDict(
     "ListEntitlementsRequestListEntitlementsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -945,14 +1628,31 @@
     "ListFlowsRequestListFlowsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+ListGatewayInstancesRequestListGatewayInstancesPaginateTypeDef = TypedDict(
+    "ListGatewayInstancesRequestListGatewayInstancesPaginateTypeDef",
+    {
+        "FilterArn": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListGatewaysRequestListGatewaysPaginateTypeDef = TypedDict(
+    "ListGatewaysRequestListGatewaysPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 ListOfferingsRequestListOfferingsPaginateTypeDef = TypedDict(
     "ListOfferingsRequestListOfferingsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -961,23 +1661,50 @@
     "ListReservationsRequestListReservationsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+ListBridgesResponseTypeDef = TypedDict(
+    "ListBridgesResponseTypeDef",
+    {
+        "Bridges": List[ListedBridgeTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListEntitlementsResponseTypeDef = TypedDict(
     "ListEntitlementsResponseTypeDef",
     {
         "Entitlements": List[ListedEntitlementTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ListGatewayInstancesResponseTypeDef = TypedDict(
+    "ListGatewayInstancesResponseTypeDef",
+    {
+        "Instances": List[ListedGatewayInstanceTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListGatewaysResponseTypeDef = TypedDict(
+    "ListGatewaysResponseTypeDef",
+    {
+        "Gateways": List[ListedGatewayTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 OfferingTypeDef = TypedDict(
     "OfferingTypeDef",
     {
         "CurrencyCode": str,
         "Duration": int,
         "DurationUnits": Literal["MONTHS"],
         "OfferingArn": str,
@@ -1003,14 +1730,37 @@
         "ReservationName": str,
         "ReservationState": ReservationStateType,
         "ResourceSpecification": ResourceSpecificationTypeDef,
         "Start": str,
     },
 )
 
+_RequiredUpdateBridgeOutputRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateBridgeOutputRequestRequestTypeDef",
+    {
+        "BridgeArn": str,
+        "OutputName": str,
+    },
+)
+_OptionalUpdateBridgeOutputRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateBridgeOutputRequestRequestTypeDef",
+    {
+        "NetworkOutput": UpdateBridgeNetworkOutputRequestTypeDef,
+    },
+    total=False,
+)
+
+
+class UpdateBridgeOutputRequestRequestTypeDef(
+    _RequiredUpdateBridgeOutputRequestRequestTypeDef,
+    _OptionalUpdateBridgeOutputRequestRequestTypeDef,
+):
+    pass
+
+
 _RequiredUpdateFlowEntitlementRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFlowEntitlementRequestRequestTypeDef",
     {
         "EntitlementArn": str,
         "FlowArn": str,
     },
 )
@@ -1029,14 +1779,64 @@
 class UpdateFlowEntitlementRequestRequestTypeDef(
     _RequiredUpdateFlowEntitlementRequestRequestTypeDef,
     _OptionalUpdateFlowEntitlementRequestRequestTypeDef,
 ):
     pass
 
 
+AddBridgeSourceRequestTypeDef = TypedDict(
+    "AddBridgeSourceRequestTypeDef",
+    {
+        "FlowSource": AddBridgeFlowSourceRequestTypeDef,
+        "NetworkSource": AddBridgeNetworkSourceRequestTypeDef,
+    },
+    total=False,
+)
+
+BridgeSourceTypeDef = TypedDict(
+    "BridgeSourceTypeDef",
+    {
+        "FlowSource": BridgeFlowSourceTypeDef,
+        "NetworkSource": BridgeNetworkSourceTypeDef,
+    },
+    total=False,
+)
+
+_RequiredUpdateBridgeSourceRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateBridgeSourceRequestRequestTypeDef",
+    {
+        "BridgeArn": str,
+        "SourceName": str,
+    },
+)
+_OptionalUpdateBridgeSourceRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateBridgeSourceRequestRequestTypeDef",
+    {
+        "FlowSource": UpdateBridgeFlowSourceRequestTypeDef,
+        "NetworkSource": UpdateBridgeNetworkSourceRequestTypeDef,
+    },
+    total=False,
+)
+
+
+class UpdateBridgeSourceRequestRequestTypeDef(
+    _RequiredUpdateBridgeSourceRequestRequestTypeDef,
+    _OptionalUpdateBridgeSourceRequestRequestTypeDef,
+):
+    pass
+
+
+AddBridgeOutputsRequestRequestTypeDef = TypedDict(
+    "AddBridgeOutputsRequestRequestTypeDef",
+    {
+        "BridgeArn": str,
+        "Outputs": Sequence[AddBridgeOutputRequestTypeDef],
+    },
+)
+
 GrantFlowEntitlementsResponseTypeDef = TypedDict(
     "GrantFlowEntitlementsResponseTypeDef",
     {
         "Entitlements": List[EntitlementTypeDef],
         "FlowArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1055,14 +1855,56 @@
     "GrantFlowEntitlementsRequestRequestTypeDef",
     {
         "Entitlements": Sequence[GrantEntitlementRequestTypeDef],
         "FlowArn": str,
     },
 )
 
+AddBridgeOutputsResponseTypeDef = TypedDict(
+    "AddBridgeOutputsResponseTypeDef",
+    {
+        "BridgeArn": str,
+        "Outputs": List[BridgeOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateBridgeOutputResponseTypeDef = TypedDict(
+    "UpdateBridgeOutputResponseTypeDef",
+    {
+        "BridgeArn": str,
+        "Output": BridgeOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeGatewayInstanceResponseTypeDef = TypedDict(
+    "DescribeGatewayInstanceResponseTypeDef",
+    {
+        "GatewayInstance": GatewayInstanceTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateGatewayResponseTypeDef = TypedDict(
+    "CreateGatewayResponseTypeDef",
+    {
+        "Gateway": GatewayTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeGatewayResponseTypeDef = TypedDict(
+    "DescribeGatewayResponseTypeDef",
+    {
+        "Gateway": GatewayTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredMediaStreamOutputConfigurationRequestTypeDef = TypedDict(
     "_RequiredMediaStreamOutputConfigurationRequestTypeDef",
     {
         "EncodingName": EncodingNameType,
         "MediaStreamName": str,
     },
 )
@@ -1147,14 +1989,37 @@
 
 class MediaStreamSourceConfigurationTypeDef(
     _RequiredMediaStreamSourceConfigurationTypeDef, _OptionalMediaStreamSourceConfigurationTypeDef
 ):
     pass
 
 
+_RequiredUpdateBridgeRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateBridgeRequestRequestTypeDef",
+    {
+        "BridgeArn": str,
+    },
+)
+_OptionalUpdateBridgeRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateBridgeRequestRequestTypeDef",
+    {
+        "EgressGatewayBridge": UpdateEgressGatewayBridgeRequestTypeDef,
+        "IngressGatewayBridge": UpdateIngressGatewayBridgeRequestTypeDef,
+        "SourceFailoverConfig": UpdateFailoverConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class UpdateBridgeRequestRequestTypeDef(
+    _RequiredUpdateBridgeRequestRequestTypeDef, _OptionalUpdateBridgeRequestRequestTypeDef
+):
+    pass
+
+
 _RequiredUpdateFlowRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFlowRequestRequestTypeDef",
     {
         "FlowArn": str,
     },
 )
 _OptionalUpdateFlowRequestRequestTypeDef = TypedDict(
@@ -1298,14 +2163,93 @@
     "PurchaseOfferingResponseTypeDef",
     {
         "Reservation": ReservationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+AddBridgeSourcesRequestRequestTypeDef = TypedDict(
+    "AddBridgeSourcesRequestRequestTypeDef",
+    {
+        "BridgeArn": str,
+        "Sources": Sequence[AddBridgeSourceRequestTypeDef],
+    },
+)
+
+_RequiredCreateBridgeRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateBridgeRequestRequestTypeDef",
+    {
+        "Name": str,
+        "PlacementArn": str,
+        "Sources": Sequence[AddBridgeSourceRequestTypeDef],
+    },
+)
+_OptionalCreateBridgeRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateBridgeRequestRequestTypeDef",
+    {
+        "EgressGatewayBridge": AddEgressGatewayBridgeRequestTypeDef,
+        "IngressGatewayBridge": AddIngressGatewayBridgeRequestTypeDef,
+        "Outputs": Sequence[AddBridgeOutputRequestTypeDef],
+        "SourceFailoverConfig": FailoverConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class CreateBridgeRequestRequestTypeDef(
+    _RequiredCreateBridgeRequestRequestTypeDef, _OptionalCreateBridgeRequestRequestTypeDef
+):
+    pass
+
+
+AddBridgeSourcesResponseTypeDef = TypedDict(
+    "AddBridgeSourcesResponseTypeDef",
+    {
+        "BridgeArn": str,
+        "Sources": List[BridgeSourceTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredBridgeTypeDef = TypedDict(
+    "_RequiredBridgeTypeDef",
+    {
+        "BridgeArn": str,
+        "BridgeState": BridgeStateType,
+        "Name": str,
+        "PlacementArn": str,
+    },
+)
+_OptionalBridgeTypeDef = TypedDict(
+    "_OptionalBridgeTypeDef",
+    {
+        "BridgeMessages": List[MessageDetailTypeDef],
+        "EgressGatewayBridge": EgressGatewayBridgeTypeDef,
+        "IngressGatewayBridge": IngressGatewayBridgeTypeDef,
+        "Outputs": List[BridgeOutputTypeDef],
+        "SourceFailoverConfig": FailoverConfigTypeDef,
+        "Sources": List[BridgeSourceTypeDef],
+    },
+    total=False,
+)
+
+
+class BridgeTypeDef(_RequiredBridgeTypeDef, _OptionalBridgeTypeDef):
+    pass
+
+
+UpdateBridgeSourceResponseTypeDef = TypedDict(
+    "UpdateBridgeSourceResponseTypeDef",
+    {
+        "BridgeArn": str,
+        "Source": BridgeSourceTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredAddOutputRequestTypeDef = TypedDict(
     "_RequiredAddOutputRequestTypeDef",
     {
         "Protocol": ProtocolType,
     },
 )
 _OptionalAddOutputRequestTypeDef = TypedDict(
@@ -1387,14 +2331,15 @@
         "SenderControlPort": int,
         "SenderIpAddress": str,
         "SourceListenerAddress": str,
         "SourceListenerPort": int,
         "StreamId": str,
         "VpcInterfaceName": str,
         "WhitelistCidr": str,
+        "GatewayBridgeSource": SetGatewayBridgeSourceRequestTypeDef,
     },
     total=False,
 )
 
 _RequiredUpdateFlowSourceRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFlowSourceRequestRequestTypeDef",
     {
@@ -1418,14 +2363,15 @@
         "SenderControlPort": int,
         "SenderIpAddress": str,
         "SourceListenerAddress": str,
         "SourceListenerPort": int,
         "StreamId": str,
         "VpcInterfaceName": str,
         "WhitelistCidr": str,
+        "GatewayBridgeSource": UpdateGatewayBridgeSourceRequestTypeDef,
     },
     total=False,
 )
 
 
 class UpdateFlowSourceRequestRequestTypeDef(
     _RequiredUpdateFlowSourceRequestRequestTypeDef, _OptionalUpdateFlowSourceRequestRequestTypeDef
@@ -1450,14 +2396,16 @@
         "EntitlementArn": str,
         "ListenerAddress": str,
         "MediaLiveInputArn": str,
         "MediaStreamOutputConfigurations": List[MediaStreamOutputConfigurationTypeDef],
         "Port": int,
         "Transport": TransportTypeDef,
         "VpcInterfaceAttachment": VpcInterfaceAttachmentTypeDef,
+        "BridgeArn": str,
+        "BridgePorts": List[int],
     },
     total=False,
 )
 
 
 class OutputTypeDef(_RequiredOutputTypeDef, _OptionalOutputTypeDef):
     pass
@@ -1481,14 +2429,15 @@
         "IngestPort": int,
         "MediaStreamSourceConfigurations": List[MediaStreamSourceConfigurationTypeDef],
         "SenderControlPort": int,
         "SenderIpAddress": str,
         "Transport": TransportTypeDef,
         "VpcInterfaceName": str,
         "WhitelistCidr": str,
+        "GatewayBridgeSource": GatewayBridgeSourceTypeDef,
     },
     total=False,
 )
 
 
 class SourceTypeDef(_RequiredSourceTypeDef, _OptionalSourceTypeDef):
     pass
@@ -1516,14 +2465,38 @@
     {
         "FlowArn": str,
         "MediaStream": MediaStreamTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+CreateBridgeResponseTypeDef = TypedDict(
+    "CreateBridgeResponseTypeDef",
+    {
+        "Bridge": BridgeTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeBridgeResponseTypeDef = TypedDict(
+    "DescribeBridgeResponseTypeDef",
+    {
+        "Bridge": BridgeTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateBridgeResponseTypeDef = TypedDict(
+    "UpdateBridgeResponseTypeDef",
+    {
+        "Bridge": BridgeTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 AddFlowOutputsRequestRequestTypeDef = TypedDict(
     "AddFlowOutputsRequestRequestTypeDef",
     {
         "FlowArn": str,
         "Outputs": Sequence[AddOutputRequestTypeDef],
     },
 )
```

### Comparing `mypy-boto3-mediaconnect-1.26.0.post1/mypy_boto3_mediaconnect/type_defs.pyi` & `mypy-boto3-mediaconnect-1.26.113/mypy_boto3_mediaconnect/type_defs.pyi`

 * *Files 23% similar despite different names*

```diff
@@ -2,29 +2,35 @@
 Type annotations for mediaconnect service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_mediaconnect.type_defs import ResponseMetadataTypeDef
+    from mypy_boto3_mediaconnect.type_defs import VpcInterfaceAttachmentTypeDef
 
-    data: ResponseMetadataTypeDef = {...}
+    data: VpcInterfaceAttachmentTypeDef = {...}
     ```
 """
 import sys
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     AlgorithmType,
+    BridgePlacementType,
+    BridgeStateType,
     ColorimetryType,
+    ConnectionStatusType,
+    DesiredStateType,
     EncoderProfileType,
     EncodingNameType,
     EntitlementStatusType,
     FailoverModeType,
+    GatewayStateType,
+    InstanceStateType,
     KeyTypeType,
     MaintenanceDayType,
     MediaStreamTypeType,
     NetworkInterfaceTypeType,
     ProtocolType,
     RangeType,
     ReservationStateType,
@@ -41,139 +47,251 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
+    "VpcInterfaceAttachmentTypeDef",
+    "AddBridgeNetworkOutputRequestTypeDef",
+    "AddBridgeNetworkSourceRequestTypeDef",
     "ResponseMetadataTypeDef",
+    "AddEgressGatewayBridgeRequestTypeDef",
     "VpcInterfaceRequestTypeDef",
     "VpcInterfaceTypeDef",
+    "AddIngressGatewayBridgeRequestTypeDef",
     "AddMaintenanceTypeDef",
     "EncryptionTypeDef",
-    "VpcInterfaceAttachmentTypeDef",
+    "BridgeFlowOutputTypeDef",
+    "BridgeNetworkOutputTypeDef",
+    "BridgeNetworkSourceTypeDef",
+    "EgressGatewayBridgeTypeDef",
+    "IngressGatewayBridgeTypeDef",
+    "MessageDetailTypeDef",
+    "GatewayNetworkTypeDef",
+    "DeleteBridgeRequestRequestTypeDef",
     "DeleteFlowRequestRequestTypeDef",
+    "DeleteGatewayRequestRequestTypeDef",
+    "DeregisterGatewayInstanceRequestRequestTypeDef",
+    "DescribeBridgeRequestRequestTypeDef",
     "WaiterConfigTypeDef",
     "DescribeFlowRequestRequestTypeDef",
     "MessagesTypeDef",
+    "DescribeGatewayInstanceRequestRequestTypeDef",
+    "DescribeGatewayRequestRequestTypeDef",
     "DescribeOfferingRequestRequestTypeDef",
     "DescribeReservationRequestRequestTypeDef",
     "InterfaceRequestTypeDef",
     "InterfaceTypeDef",
     "EncodingParametersRequestTypeDef",
     "EncodingParametersTypeDef",
     "SourcePriorityTypeDef",
     "MaintenanceTypeDef",
     "FmtpRequestTypeDef",
     "FmtpTypeDef",
     "PaginatorConfigTypeDef",
+    "ListBridgesRequestRequestTypeDef",
+    "ListedBridgeTypeDef",
     "ListEntitlementsRequestRequestTypeDef",
     "ListedEntitlementTypeDef",
     "ListFlowsRequestRequestTypeDef",
+    "ListGatewayInstancesRequestRequestTypeDef",
+    "ListedGatewayInstanceTypeDef",
+    "ListGatewaysRequestRequestTypeDef",
+    "ListedGatewayTypeDef",
     "ListOfferingsRequestRequestTypeDef",
     "ListReservationsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ResourceSpecificationTypeDef",
     "TransportTypeDef",
     "PurchaseOfferingRequestRequestTypeDef",
+    "RemoveBridgeOutputRequestRequestTypeDef",
+    "RemoveBridgeSourceRequestRequestTypeDef",
     "RemoveFlowMediaStreamRequestRequestTypeDef",
     "RemoveFlowOutputRequestRequestTypeDef",
     "RemoveFlowSourceRequestRequestTypeDef",
     "RemoveFlowVpcInterfaceRequestRequestTypeDef",
     "RevokeFlowEntitlementRequestRequestTypeDef",
     "StartFlowRequestRequestTypeDef",
     "StopFlowRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "UpdateBridgeNetworkOutputRequestTypeDef",
+    "UpdateBridgeNetworkSourceRequestTypeDef",
+    "UpdateEgressGatewayBridgeRequestTypeDef",
+    "UpdateIngressGatewayBridgeRequestTypeDef",
+    "UpdateBridgeStateRequestRequestTypeDef",
     "UpdateEncryptionTypeDef",
     "UpdateMaintenanceTypeDef",
+    "UpdateGatewayInstanceRequestRequestTypeDef",
+    "AddBridgeFlowSourceRequestTypeDef",
+    "BridgeFlowSourceTypeDef",
+    "GatewayBridgeSourceTypeDef",
+    "SetGatewayBridgeSourceRequestTypeDef",
+    "UpdateBridgeFlowSourceRequestTypeDef",
+    "UpdateGatewayBridgeSourceRequestTypeDef",
+    "AddBridgeOutputRequestTypeDef",
+    "DeleteBridgeResponseTypeDef",
     "DeleteFlowResponseTypeDef",
+    "DeleteGatewayResponseTypeDef",
+    "DeregisterGatewayInstanceResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
     "ListTagsForResourceResponseTypeDef",
+    "RemoveBridgeOutputResponseTypeDef",
+    "RemoveBridgeSourceResponseTypeDef",
     "RemoveFlowMediaStreamResponseTypeDef",
     "RemoveFlowOutputResponseTypeDef",
     "RemoveFlowSourceResponseTypeDef",
     "RemoveFlowVpcInterfaceResponseTypeDef",
     "RevokeFlowEntitlementResponseTypeDef",
     "StartFlowResponseTypeDef",
     "StopFlowResponseTypeDef",
+    "UpdateBridgeStateResponseTypeDef",
+    "UpdateGatewayInstanceResponseTypeDef",
     "AddFlowVpcInterfacesRequestRequestTypeDef",
     "AddFlowVpcInterfacesResponseTypeDef",
     "EntitlementTypeDef",
     "GrantEntitlementRequestTypeDef",
+    "BridgeOutputTypeDef",
+    "GatewayInstanceTypeDef",
+    "CreateGatewayRequestRequestTypeDef",
+    "GatewayTypeDef",
     "DescribeFlowRequestFlowActiveWaitTypeDef",
     "DescribeFlowRequestFlowDeletedWaitTypeDef",
     "DescribeFlowRequestFlowStandbyWaitTypeDef",
     "DestinationConfigurationRequestTypeDef",
     "InputConfigurationRequestTypeDef",
     "DestinationConfigurationTypeDef",
     "InputConfigurationTypeDef",
     "FailoverConfigTypeDef",
     "UpdateFailoverConfigTypeDef",
     "ListedFlowTypeDef",
     "MediaStreamAttributesRequestTypeDef",
     "MediaStreamAttributesTypeDef",
+    "ListBridgesRequestListBridgesPaginateTypeDef",
     "ListEntitlementsRequestListEntitlementsPaginateTypeDef",
     "ListFlowsRequestListFlowsPaginateTypeDef",
+    "ListGatewayInstancesRequestListGatewayInstancesPaginateTypeDef",
+    "ListGatewaysRequestListGatewaysPaginateTypeDef",
     "ListOfferingsRequestListOfferingsPaginateTypeDef",
     "ListReservationsRequestListReservationsPaginateTypeDef",
+    "ListBridgesResponseTypeDef",
     "ListEntitlementsResponseTypeDef",
+    "ListGatewayInstancesResponseTypeDef",
+    "ListGatewaysResponseTypeDef",
     "OfferingTypeDef",
     "ReservationTypeDef",
+    "UpdateBridgeOutputRequestRequestTypeDef",
     "UpdateFlowEntitlementRequestRequestTypeDef",
+    "AddBridgeSourceRequestTypeDef",
+    "BridgeSourceTypeDef",
+    "UpdateBridgeSourceRequestRequestTypeDef",
+    "AddBridgeOutputsRequestRequestTypeDef",
     "GrantFlowEntitlementsResponseTypeDef",
     "UpdateFlowEntitlementResponseTypeDef",
     "GrantFlowEntitlementsRequestRequestTypeDef",
+    "AddBridgeOutputsResponseTypeDef",
+    "UpdateBridgeOutputResponseTypeDef",
+    "DescribeGatewayInstanceResponseTypeDef",
+    "CreateGatewayResponseTypeDef",
+    "DescribeGatewayResponseTypeDef",
     "MediaStreamOutputConfigurationRequestTypeDef",
     "MediaStreamSourceConfigurationRequestTypeDef",
     "MediaStreamOutputConfigurationTypeDef",
     "MediaStreamSourceConfigurationTypeDef",
+    "UpdateBridgeRequestRequestTypeDef",
     "UpdateFlowRequestRequestTypeDef",
     "ListFlowsResponseTypeDef",
     "AddMediaStreamRequestTypeDef",
     "UpdateFlowMediaStreamRequestRequestTypeDef",
     "MediaStreamTypeDef",
     "DescribeOfferingResponseTypeDef",
     "ListOfferingsResponseTypeDef",
     "DescribeReservationResponseTypeDef",
     "ListReservationsResponseTypeDef",
     "PurchaseOfferingResponseTypeDef",
+    "AddBridgeSourcesRequestRequestTypeDef",
+    "CreateBridgeRequestRequestTypeDef",
+    "AddBridgeSourcesResponseTypeDef",
+    "BridgeTypeDef",
+    "UpdateBridgeSourceResponseTypeDef",
     "AddOutputRequestTypeDef",
     "UpdateFlowOutputRequestRequestTypeDef",
     "SetSourceRequestTypeDef",
     "UpdateFlowSourceRequestRequestTypeDef",
     "OutputTypeDef",
     "SourceTypeDef",
     "AddFlowMediaStreamsRequestRequestTypeDef",
     "AddFlowMediaStreamsResponseTypeDef",
     "UpdateFlowMediaStreamResponseTypeDef",
+    "CreateBridgeResponseTypeDef",
+    "DescribeBridgeResponseTypeDef",
+    "UpdateBridgeResponseTypeDef",
     "AddFlowOutputsRequestRequestTypeDef",
     "AddFlowSourcesRequestRequestTypeDef",
     "CreateFlowRequestRequestTypeDef",
     "AddFlowOutputsResponseTypeDef",
     "UpdateFlowOutputResponseTypeDef",
     "AddFlowSourcesResponseTypeDef",
     "FlowTypeDef",
     "UpdateFlowSourceResponseTypeDef",
     "CreateFlowResponseTypeDef",
     "DescribeFlowResponseTypeDef",
     "UpdateFlowResponseTypeDef",
 )
 
+VpcInterfaceAttachmentTypeDef = TypedDict(
+    "VpcInterfaceAttachmentTypeDef",
+    {
+        "VpcInterfaceName": str,
+    },
+    total=False,
+)
+
+AddBridgeNetworkOutputRequestTypeDef = TypedDict(
+    "AddBridgeNetworkOutputRequestTypeDef",
+    {
+        "IpAddress": str,
+        "Name": str,
+        "NetworkName": str,
+        "Port": int,
+        "Protocol": ProtocolType,
+        "Ttl": int,
+    },
+)
+
+AddBridgeNetworkSourceRequestTypeDef = TypedDict(
+    "AddBridgeNetworkSourceRequestTypeDef",
+    {
+        "MulticastIp": str,
+        "Name": str,
+        "NetworkName": str,
+        "Port": int,
+        "Protocol": ProtocolType,
+    },
+)
+
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
+AddEgressGatewayBridgeRequestTypeDef = TypedDict(
+    "AddEgressGatewayBridgeRequestTypeDef",
+    {
+        "MaxBitrate": int,
+    },
+)
+
 _RequiredVpcInterfaceRequestTypeDef = TypedDict(
     "_RequiredVpcInterfaceRequestTypeDef",
     {
         "Name": str,
         "RoleArn": str,
         "SecurityGroupIds": Sequence[str],
         "SubnetId": str,
@@ -200,14 +318,22 @@
         "NetworkInterfaceType": NetworkInterfaceTypeType,
         "RoleArn": str,
         "SecurityGroupIds": List[str],
         "SubnetId": str,
     },
 )
 
+AddIngressGatewayBridgeRequestTypeDef = TypedDict(
+    "AddIngressGatewayBridgeRequestTypeDef",
+    {
+        "MaxBitrate": int,
+        "MaxOutputs": int,
+    },
+)
+
 AddMaintenanceTypeDef = TypedDict(
     "AddMaintenanceTypeDef",
     {
         "MaintenanceDay": MaintenanceDayType,
         "MaintenanceStartHour": str,
     },
 )
@@ -232,29 +358,159 @@
     },
     total=False,
 )
 
 class EncryptionTypeDef(_RequiredEncryptionTypeDef, _OptionalEncryptionTypeDef):
     pass
 
-VpcInterfaceAttachmentTypeDef = TypedDict(
-    "VpcInterfaceAttachmentTypeDef",
+BridgeFlowOutputTypeDef = TypedDict(
+    "BridgeFlowOutputTypeDef",
     {
-        "VpcInterfaceName": str,
+        "FlowArn": str,
+        "FlowSourceArn": str,
+        "Name": str,
+    },
+)
+
+BridgeNetworkOutputTypeDef = TypedDict(
+    "BridgeNetworkOutputTypeDef",
+    {
+        "IpAddress": str,
+        "Name": str,
+        "NetworkName": str,
+        "Port": int,
+        "Protocol": ProtocolType,
+        "Ttl": int,
+    },
+)
+
+BridgeNetworkSourceTypeDef = TypedDict(
+    "BridgeNetworkSourceTypeDef",
+    {
+        "MulticastIp": str,
+        "Name": str,
+        "NetworkName": str,
+        "Port": int,
+        "Protocol": ProtocolType,
+    },
+)
+
+_RequiredEgressGatewayBridgeTypeDef = TypedDict(
+    "_RequiredEgressGatewayBridgeTypeDef",
+    {
+        "MaxBitrate": int,
+    },
+)
+_OptionalEgressGatewayBridgeTypeDef = TypedDict(
+    "_OptionalEgressGatewayBridgeTypeDef",
+    {
+        "InstanceId": str,
     },
     total=False,
 )
 
+class EgressGatewayBridgeTypeDef(
+    _RequiredEgressGatewayBridgeTypeDef, _OptionalEgressGatewayBridgeTypeDef
+):
+    pass
+
+_RequiredIngressGatewayBridgeTypeDef = TypedDict(
+    "_RequiredIngressGatewayBridgeTypeDef",
+    {
+        "MaxBitrate": int,
+        "MaxOutputs": int,
+    },
+)
+_OptionalIngressGatewayBridgeTypeDef = TypedDict(
+    "_OptionalIngressGatewayBridgeTypeDef",
+    {
+        "InstanceId": str,
+    },
+    total=False,
+)
+
+class IngressGatewayBridgeTypeDef(
+    _RequiredIngressGatewayBridgeTypeDef, _OptionalIngressGatewayBridgeTypeDef
+):
+    pass
+
+_RequiredMessageDetailTypeDef = TypedDict(
+    "_RequiredMessageDetailTypeDef",
+    {
+        "Code": str,
+        "Message": str,
+    },
+)
+_OptionalMessageDetailTypeDef = TypedDict(
+    "_OptionalMessageDetailTypeDef",
+    {
+        "ResourceName": str,
+    },
+    total=False,
+)
+
+class MessageDetailTypeDef(_RequiredMessageDetailTypeDef, _OptionalMessageDetailTypeDef):
+    pass
+
+GatewayNetworkTypeDef = TypedDict(
+    "GatewayNetworkTypeDef",
+    {
+        "CidrBlock": str,
+        "Name": str,
+    },
+)
+
+DeleteBridgeRequestRequestTypeDef = TypedDict(
+    "DeleteBridgeRequestRequestTypeDef",
+    {
+        "BridgeArn": str,
+    },
+)
+
 DeleteFlowRequestRequestTypeDef = TypedDict(
     "DeleteFlowRequestRequestTypeDef",
     {
         "FlowArn": str,
     },
 )
 
+DeleteGatewayRequestRequestTypeDef = TypedDict(
+    "DeleteGatewayRequestRequestTypeDef",
+    {
+        "GatewayArn": str,
+    },
+)
+
+_RequiredDeregisterGatewayInstanceRequestRequestTypeDef = TypedDict(
+    "_RequiredDeregisterGatewayInstanceRequestRequestTypeDef",
+    {
+        "GatewayInstanceArn": str,
+    },
+)
+_OptionalDeregisterGatewayInstanceRequestRequestTypeDef = TypedDict(
+    "_OptionalDeregisterGatewayInstanceRequestRequestTypeDef",
+    {
+        "Force": bool,
+    },
+    total=False,
+)
+
+class DeregisterGatewayInstanceRequestRequestTypeDef(
+    _RequiredDeregisterGatewayInstanceRequestRequestTypeDef,
+    _OptionalDeregisterGatewayInstanceRequestRequestTypeDef,
+):
+    pass
+
+DescribeBridgeRequestRequestTypeDef = TypedDict(
+    "DescribeBridgeRequestRequestTypeDef",
+    {
+        "BridgeArn": str,
+    },
+)
+
 WaiterConfigTypeDef = TypedDict(
     "WaiterConfigTypeDef",
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
@@ -270,14 +526,28 @@
 MessagesTypeDef = TypedDict(
     "MessagesTypeDef",
     {
         "Errors": List[str],
     },
 )
 
+DescribeGatewayInstanceRequestRequestTypeDef = TypedDict(
+    "DescribeGatewayInstanceRequestRequestTypeDef",
+    {
+        "GatewayInstanceArn": str,
+    },
+)
+
+DescribeGatewayRequestRequestTypeDef = TypedDict(
+    "DescribeGatewayRequestRequestTypeDef",
+    {
+        "GatewayArn": str,
+    },
+)
+
 DescribeOfferingRequestRequestTypeDef = TypedDict(
     "DescribeOfferingRequestRequestTypeDef",
     {
         "OfferingArn": str,
     },
 )
 
@@ -371,14 +641,35 @@
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
+ListBridgesRequestRequestTypeDef = TypedDict(
+    "ListBridgesRequestRequestTypeDef",
+    {
+        "FilterArn": str,
+        "MaxResults": int,
+        "NextToken": str,
+    },
+    total=False,
+)
+
+ListedBridgeTypeDef = TypedDict(
+    "ListedBridgeTypeDef",
+    {
+        "BridgeArn": str,
+        "BridgeState": BridgeStateType,
+        "BridgeType": str,
+        "Name": str,
+        "PlacementArn": str,
+    },
+)
+
 ListEntitlementsRequestRequestTypeDef = TypedDict(
     "ListEntitlementsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -409,14 +700,63 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+ListGatewayInstancesRequestRequestTypeDef = TypedDict(
+    "ListGatewayInstancesRequestRequestTypeDef",
+    {
+        "FilterArn": str,
+        "MaxResults": int,
+        "NextToken": str,
+    },
+    total=False,
+)
+
+_RequiredListedGatewayInstanceTypeDef = TypedDict(
+    "_RequiredListedGatewayInstanceTypeDef",
+    {
+        "GatewayArn": str,
+        "GatewayInstanceArn": str,
+        "InstanceId": str,
+    },
+)
+_OptionalListedGatewayInstanceTypeDef = TypedDict(
+    "_OptionalListedGatewayInstanceTypeDef",
+    {
+        "InstanceState": InstanceStateType,
+    },
+    total=False,
+)
+
+class ListedGatewayInstanceTypeDef(
+    _RequiredListedGatewayInstanceTypeDef, _OptionalListedGatewayInstanceTypeDef
+):
+    pass
+
+ListGatewaysRequestRequestTypeDef = TypedDict(
+    "ListGatewaysRequestRequestTypeDef",
+    {
+        "MaxResults": int,
+        "NextToken": str,
+    },
+    total=False,
+)
+
+ListedGatewayTypeDef = TypedDict(
+    "ListedGatewayTypeDef",
+    {
+        "GatewayArn": str,
+        "GatewayState": GatewayStateType,
+        "Name": str,
+    },
+)
+
 ListOfferingsRequestRequestTypeDef = TypedDict(
     "ListOfferingsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -490,14 +830,30 @@
     {
         "OfferingArn": str,
         "ReservationName": str,
         "Start": str,
     },
 )
 
+RemoveBridgeOutputRequestRequestTypeDef = TypedDict(
+    "RemoveBridgeOutputRequestRequestTypeDef",
+    {
+        "BridgeArn": str,
+        "OutputName": str,
+    },
+)
+
+RemoveBridgeSourceRequestRequestTypeDef = TypedDict(
+    "RemoveBridgeSourceRequestRequestTypeDef",
+    {
+        "BridgeArn": str,
+        "SourceName": str,
+    },
+)
+
 RemoveFlowMediaStreamRequestRequestTypeDef = TypedDict(
     "RemoveFlowMediaStreamRequestRequestTypeDef",
     {
         "FlowArn": str,
         "MediaStreamName": str,
     },
 )
@@ -560,14 +916,62 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
+UpdateBridgeNetworkOutputRequestTypeDef = TypedDict(
+    "UpdateBridgeNetworkOutputRequestTypeDef",
+    {
+        "IpAddress": str,
+        "NetworkName": str,
+        "Port": int,
+        "Protocol": ProtocolType,
+        "Ttl": int,
+    },
+    total=False,
+)
+
+UpdateBridgeNetworkSourceRequestTypeDef = TypedDict(
+    "UpdateBridgeNetworkSourceRequestTypeDef",
+    {
+        "MulticastIp": str,
+        "NetworkName": str,
+        "Port": int,
+        "Protocol": ProtocolType,
+    },
+    total=False,
+)
+
+UpdateEgressGatewayBridgeRequestTypeDef = TypedDict(
+    "UpdateEgressGatewayBridgeRequestTypeDef",
+    {
+        "MaxBitrate": int,
+    },
+    total=False,
+)
+
+UpdateIngressGatewayBridgeRequestTypeDef = TypedDict(
+    "UpdateIngressGatewayBridgeRequestTypeDef",
+    {
+        "MaxBitrate": int,
+        "MaxOutputs": int,
+    },
+    total=False,
+)
+
+UpdateBridgeStateRequestRequestTypeDef = TypedDict(
+    "UpdateBridgeStateRequestRequestTypeDef",
+    {
+        "BridgeArn": str,
+        "DesiredState": DesiredStateType,
+    },
+)
+
 UpdateEncryptionTypeDef = TypedDict(
     "UpdateEncryptionTypeDef",
     {
         "Algorithm": AlgorithmType,
         "ConstantInitializationVector": str,
         "DeviceId": str,
         "KeyType": KeyTypeType,
@@ -586,23 +990,171 @@
         "MaintenanceDay": MaintenanceDayType,
         "MaintenanceScheduledDate": str,
         "MaintenanceStartHour": str,
     },
     total=False,
 )
 
+_RequiredUpdateGatewayInstanceRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateGatewayInstanceRequestRequestTypeDef",
+    {
+        "GatewayInstanceArn": str,
+    },
+)
+_OptionalUpdateGatewayInstanceRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateGatewayInstanceRequestRequestTypeDef",
+    {
+        "BridgePlacement": BridgePlacementType,
+    },
+    total=False,
+)
+
+class UpdateGatewayInstanceRequestRequestTypeDef(
+    _RequiredUpdateGatewayInstanceRequestRequestTypeDef,
+    _OptionalUpdateGatewayInstanceRequestRequestTypeDef,
+):
+    pass
+
+_RequiredAddBridgeFlowSourceRequestTypeDef = TypedDict(
+    "_RequiredAddBridgeFlowSourceRequestTypeDef",
+    {
+        "FlowArn": str,
+        "Name": str,
+    },
+)
+_OptionalAddBridgeFlowSourceRequestTypeDef = TypedDict(
+    "_OptionalAddBridgeFlowSourceRequestTypeDef",
+    {
+        "FlowVpcInterfaceAttachment": VpcInterfaceAttachmentTypeDef,
+    },
+    total=False,
+)
+
+class AddBridgeFlowSourceRequestTypeDef(
+    _RequiredAddBridgeFlowSourceRequestTypeDef, _OptionalAddBridgeFlowSourceRequestTypeDef
+):
+    pass
+
+_RequiredBridgeFlowSourceTypeDef = TypedDict(
+    "_RequiredBridgeFlowSourceTypeDef",
+    {
+        "FlowArn": str,
+        "Name": str,
+    },
+)
+_OptionalBridgeFlowSourceTypeDef = TypedDict(
+    "_OptionalBridgeFlowSourceTypeDef",
+    {
+        "FlowVpcInterfaceAttachment": VpcInterfaceAttachmentTypeDef,
+        "OutputArn": str,
+    },
+    total=False,
+)
+
+class BridgeFlowSourceTypeDef(_RequiredBridgeFlowSourceTypeDef, _OptionalBridgeFlowSourceTypeDef):
+    pass
+
+_RequiredGatewayBridgeSourceTypeDef = TypedDict(
+    "_RequiredGatewayBridgeSourceTypeDef",
+    {
+        "BridgeArn": str,
+    },
+)
+_OptionalGatewayBridgeSourceTypeDef = TypedDict(
+    "_OptionalGatewayBridgeSourceTypeDef",
+    {
+        "VpcInterfaceAttachment": VpcInterfaceAttachmentTypeDef,
+    },
+    total=False,
+)
+
+class GatewayBridgeSourceTypeDef(
+    _RequiredGatewayBridgeSourceTypeDef, _OptionalGatewayBridgeSourceTypeDef
+):
+    pass
+
+_RequiredSetGatewayBridgeSourceRequestTypeDef = TypedDict(
+    "_RequiredSetGatewayBridgeSourceRequestTypeDef",
+    {
+        "BridgeArn": str,
+    },
+)
+_OptionalSetGatewayBridgeSourceRequestTypeDef = TypedDict(
+    "_OptionalSetGatewayBridgeSourceRequestTypeDef",
+    {
+        "VpcInterfaceAttachment": VpcInterfaceAttachmentTypeDef,
+    },
+    total=False,
+)
+
+class SetGatewayBridgeSourceRequestTypeDef(
+    _RequiredSetGatewayBridgeSourceRequestTypeDef, _OptionalSetGatewayBridgeSourceRequestTypeDef
+):
+    pass
+
+UpdateBridgeFlowSourceRequestTypeDef = TypedDict(
+    "UpdateBridgeFlowSourceRequestTypeDef",
+    {
+        "FlowArn": str,
+        "FlowVpcInterfaceAttachment": VpcInterfaceAttachmentTypeDef,
+    },
+    total=False,
+)
+
+UpdateGatewayBridgeSourceRequestTypeDef = TypedDict(
+    "UpdateGatewayBridgeSourceRequestTypeDef",
+    {
+        "BridgeArn": str,
+        "VpcInterfaceAttachment": VpcInterfaceAttachmentTypeDef,
+    },
+    total=False,
+)
+
+AddBridgeOutputRequestTypeDef = TypedDict(
+    "AddBridgeOutputRequestTypeDef",
+    {
+        "NetworkOutput": AddBridgeNetworkOutputRequestTypeDef,
+    },
+    total=False,
+)
+
+DeleteBridgeResponseTypeDef = TypedDict(
+    "DeleteBridgeResponseTypeDef",
+    {
+        "BridgeArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DeleteFlowResponseTypeDef = TypedDict(
     "DeleteFlowResponseTypeDef",
     {
         "FlowArn": str,
         "Status": StatusType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DeleteGatewayResponseTypeDef = TypedDict(
+    "DeleteGatewayResponseTypeDef",
+    {
+        "GatewayArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeregisterGatewayInstanceResponseTypeDef = TypedDict(
+    "DeregisterGatewayInstanceResponseTypeDef",
+    {
+        "GatewayInstanceArn": str,
+        "InstanceState": InstanceStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 EmptyResponseMetadataTypeDef = TypedDict(
     "EmptyResponseMetadataTypeDef",
     {
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
@@ -610,14 +1162,32 @@
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+RemoveBridgeOutputResponseTypeDef = TypedDict(
+    "RemoveBridgeOutputResponseTypeDef",
+    {
+        "BridgeArn": str,
+        "OutputName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RemoveBridgeSourceResponseTypeDef = TypedDict(
+    "RemoveBridgeSourceResponseTypeDef",
+    {
+        "BridgeArn": str,
+        "SourceName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 RemoveFlowMediaStreamResponseTypeDef = TypedDict(
     "RemoveFlowMediaStreamResponseTypeDef",
     {
         "FlowArn": str,
         "MediaStreamName": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -674,14 +1244,32 @@
     {
         "FlowArn": str,
         "Status": StatusType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+UpdateBridgeStateResponseTypeDef = TypedDict(
+    "UpdateBridgeStateResponseTypeDef",
+    {
+        "BridgeArn": str,
+        "DesiredState": DesiredStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateGatewayInstanceResponseTypeDef = TypedDict(
+    "UpdateGatewayInstanceResponseTypeDef",
+    {
+        "BridgePlacement": BridgePlacementType,
+        "GatewayInstanceArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 AddFlowVpcInterfacesRequestRequestTypeDef = TypedDict(
     "AddFlowVpcInterfacesRequestRequestTypeDef",
     {
         "FlowArn": str,
         "VpcInterfaces": Sequence[VpcInterfaceRequestTypeDef],
     },
 )
@@ -736,14 +1324,76 @@
 )
 
 class GrantEntitlementRequestTypeDef(
     _RequiredGrantEntitlementRequestTypeDef, _OptionalGrantEntitlementRequestTypeDef
 ):
     pass
 
+BridgeOutputTypeDef = TypedDict(
+    "BridgeOutputTypeDef",
+    {
+        "FlowOutput": BridgeFlowOutputTypeDef,
+        "NetworkOutput": BridgeNetworkOutputTypeDef,
+    },
+    total=False,
+)
+
+_RequiredGatewayInstanceTypeDef = TypedDict(
+    "_RequiredGatewayInstanceTypeDef",
+    {
+        "BridgePlacement": BridgePlacementType,
+        "ConnectionStatus": ConnectionStatusType,
+        "GatewayArn": str,
+        "GatewayInstanceArn": str,
+        "InstanceId": str,
+        "InstanceState": InstanceStateType,
+        "RunningBridgeCount": int,
+    },
+)
+_OptionalGatewayInstanceTypeDef = TypedDict(
+    "_OptionalGatewayInstanceTypeDef",
+    {
+        "InstanceMessages": List[MessageDetailTypeDef],
+    },
+    total=False,
+)
+
+class GatewayInstanceTypeDef(_RequiredGatewayInstanceTypeDef, _OptionalGatewayInstanceTypeDef):
+    pass
+
+CreateGatewayRequestRequestTypeDef = TypedDict(
+    "CreateGatewayRequestRequestTypeDef",
+    {
+        "EgressCidrBlocks": Sequence[str],
+        "Name": str,
+        "Networks": Sequence[GatewayNetworkTypeDef],
+    },
+)
+
+_RequiredGatewayTypeDef = TypedDict(
+    "_RequiredGatewayTypeDef",
+    {
+        "EgressCidrBlocks": List[str],
+        "GatewayArn": str,
+        "Name": str,
+        "Networks": List[GatewayNetworkTypeDef],
+    },
+)
+_OptionalGatewayTypeDef = TypedDict(
+    "_OptionalGatewayTypeDef",
+    {
+        "GatewayMessages": List[MessageDetailTypeDef],
+        "GatewayState": GatewayStateType,
+    },
+    total=False,
+)
+
+class GatewayTypeDef(_RequiredGatewayTypeDef, _OptionalGatewayTypeDef):
+    pass
+
 _RequiredDescribeFlowRequestFlowActiveWaitTypeDef = TypedDict(
     "_RequiredDescribeFlowRequestFlowActiveWaitTypeDef",
     {
         "FlowArn": str,
     },
 )
 _OptionalDescribeFlowRequestFlowActiveWaitTypeDef = TypedDict(
@@ -904,14 +1554,23 @@
 )
 
 class MediaStreamAttributesTypeDef(
     _RequiredMediaStreamAttributesTypeDef, _OptionalMediaStreamAttributesTypeDef
 ):
     pass
 
+ListBridgesRequestListBridgesPaginateTypeDef = TypedDict(
+    "ListBridgesRequestListBridgesPaginateTypeDef",
+    {
+        "FilterArn": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 ListEntitlementsRequestListEntitlementsPaginateTypeDef = TypedDict(
     "ListEntitlementsRequestListEntitlementsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -920,14 +1579,31 @@
     "ListFlowsRequestListFlowsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+ListGatewayInstancesRequestListGatewayInstancesPaginateTypeDef = TypedDict(
+    "ListGatewayInstancesRequestListGatewayInstancesPaginateTypeDef",
+    {
+        "FilterArn": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListGatewaysRequestListGatewaysPaginateTypeDef = TypedDict(
+    "ListGatewaysRequestListGatewaysPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 ListOfferingsRequestListOfferingsPaginateTypeDef = TypedDict(
     "ListOfferingsRequestListOfferingsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -936,23 +1612,50 @@
     "ListReservationsRequestListReservationsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+ListBridgesResponseTypeDef = TypedDict(
+    "ListBridgesResponseTypeDef",
+    {
+        "Bridges": List[ListedBridgeTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListEntitlementsResponseTypeDef = TypedDict(
     "ListEntitlementsResponseTypeDef",
     {
         "Entitlements": List[ListedEntitlementTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ListGatewayInstancesResponseTypeDef = TypedDict(
+    "ListGatewayInstancesResponseTypeDef",
+    {
+        "Instances": List[ListedGatewayInstanceTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListGatewaysResponseTypeDef = TypedDict(
+    "ListGatewaysResponseTypeDef",
+    {
+        "Gateways": List[ListedGatewayTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 OfferingTypeDef = TypedDict(
     "OfferingTypeDef",
     {
         "CurrencyCode": str,
         "Duration": int,
         "DurationUnits": Literal["MONTHS"],
         "OfferingArn": str,
@@ -978,14 +1681,35 @@
         "ReservationName": str,
         "ReservationState": ReservationStateType,
         "ResourceSpecification": ResourceSpecificationTypeDef,
         "Start": str,
     },
 )
 
+_RequiredUpdateBridgeOutputRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateBridgeOutputRequestRequestTypeDef",
+    {
+        "BridgeArn": str,
+        "OutputName": str,
+    },
+)
+_OptionalUpdateBridgeOutputRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateBridgeOutputRequestRequestTypeDef",
+    {
+        "NetworkOutput": UpdateBridgeNetworkOutputRequestTypeDef,
+    },
+    total=False,
+)
+
+class UpdateBridgeOutputRequestRequestTypeDef(
+    _RequiredUpdateBridgeOutputRequestRequestTypeDef,
+    _OptionalUpdateBridgeOutputRequestRequestTypeDef,
+):
+    pass
+
 _RequiredUpdateFlowEntitlementRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFlowEntitlementRequestRequestTypeDef",
     {
         "EntitlementArn": str,
         "FlowArn": str,
     },
 )
@@ -1002,14 +1726,62 @@
 
 class UpdateFlowEntitlementRequestRequestTypeDef(
     _RequiredUpdateFlowEntitlementRequestRequestTypeDef,
     _OptionalUpdateFlowEntitlementRequestRequestTypeDef,
 ):
     pass
 
+AddBridgeSourceRequestTypeDef = TypedDict(
+    "AddBridgeSourceRequestTypeDef",
+    {
+        "FlowSource": AddBridgeFlowSourceRequestTypeDef,
+        "NetworkSource": AddBridgeNetworkSourceRequestTypeDef,
+    },
+    total=False,
+)
+
+BridgeSourceTypeDef = TypedDict(
+    "BridgeSourceTypeDef",
+    {
+        "FlowSource": BridgeFlowSourceTypeDef,
+        "NetworkSource": BridgeNetworkSourceTypeDef,
+    },
+    total=False,
+)
+
+_RequiredUpdateBridgeSourceRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateBridgeSourceRequestRequestTypeDef",
+    {
+        "BridgeArn": str,
+        "SourceName": str,
+    },
+)
+_OptionalUpdateBridgeSourceRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateBridgeSourceRequestRequestTypeDef",
+    {
+        "FlowSource": UpdateBridgeFlowSourceRequestTypeDef,
+        "NetworkSource": UpdateBridgeNetworkSourceRequestTypeDef,
+    },
+    total=False,
+)
+
+class UpdateBridgeSourceRequestRequestTypeDef(
+    _RequiredUpdateBridgeSourceRequestRequestTypeDef,
+    _OptionalUpdateBridgeSourceRequestRequestTypeDef,
+):
+    pass
+
+AddBridgeOutputsRequestRequestTypeDef = TypedDict(
+    "AddBridgeOutputsRequestRequestTypeDef",
+    {
+        "BridgeArn": str,
+        "Outputs": Sequence[AddBridgeOutputRequestTypeDef],
+    },
+)
+
 GrantFlowEntitlementsResponseTypeDef = TypedDict(
     "GrantFlowEntitlementsResponseTypeDef",
     {
         "Entitlements": List[EntitlementTypeDef],
         "FlowArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1028,14 +1800,56 @@
     "GrantFlowEntitlementsRequestRequestTypeDef",
     {
         "Entitlements": Sequence[GrantEntitlementRequestTypeDef],
         "FlowArn": str,
     },
 )
 
+AddBridgeOutputsResponseTypeDef = TypedDict(
+    "AddBridgeOutputsResponseTypeDef",
+    {
+        "BridgeArn": str,
+        "Outputs": List[BridgeOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateBridgeOutputResponseTypeDef = TypedDict(
+    "UpdateBridgeOutputResponseTypeDef",
+    {
+        "BridgeArn": str,
+        "Output": BridgeOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeGatewayInstanceResponseTypeDef = TypedDict(
+    "DescribeGatewayInstanceResponseTypeDef",
+    {
+        "GatewayInstance": GatewayInstanceTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateGatewayResponseTypeDef = TypedDict(
+    "CreateGatewayResponseTypeDef",
+    {
+        "Gateway": GatewayTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeGatewayResponseTypeDef = TypedDict(
+    "DescribeGatewayResponseTypeDef",
+    {
+        "Gateway": GatewayTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredMediaStreamOutputConfigurationRequestTypeDef = TypedDict(
     "_RequiredMediaStreamOutputConfigurationRequestTypeDef",
     {
         "EncodingName": EncodingNameType,
         "MediaStreamName": str,
     },
 )
@@ -1112,14 +1926,35 @@
 )
 
 class MediaStreamSourceConfigurationTypeDef(
     _RequiredMediaStreamSourceConfigurationTypeDef, _OptionalMediaStreamSourceConfigurationTypeDef
 ):
     pass
 
+_RequiredUpdateBridgeRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateBridgeRequestRequestTypeDef",
+    {
+        "BridgeArn": str,
+    },
+)
+_OptionalUpdateBridgeRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateBridgeRequestRequestTypeDef",
+    {
+        "EgressGatewayBridge": UpdateEgressGatewayBridgeRequestTypeDef,
+        "IngressGatewayBridge": UpdateIngressGatewayBridgeRequestTypeDef,
+        "SourceFailoverConfig": UpdateFailoverConfigTypeDef,
+    },
+    total=False,
+)
+
+class UpdateBridgeRequestRequestTypeDef(
+    _RequiredUpdateBridgeRequestRequestTypeDef, _OptionalUpdateBridgeRequestRequestTypeDef
+):
+    pass
+
 _RequiredUpdateFlowRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFlowRequestRequestTypeDef",
     {
         "FlowArn": str,
     },
 )
 _OptionalUpdateFlowRequestRequestTypeDef = TypedDict(
@@ -1255,14 +2090,89 @@
     "PurchaseOfferingResponseTypeDef",
     {
         "Reservation": ReservationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+AddBridgeSourcesRequestRequestTypeDef = TypedDict(
+    "AddBridgeSourcesRequestRequestTypeDef",
+    {
+        "BridgeArn": str,
+        "Sources": Sequence[AddBridgeSourceRequestTypeDef],
+    },
+)
+
+_RequiredCreateBridgeRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateBridgeRequestRequestTypeDef",
+    {
+        "Name": str,
+        "PlacementArn": str,
+        "Sources": Sequence[AddBridgeSourceRequestTypeDef],
+    },
+)
+_OptionalCreateBridgeRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateBridgeRequestRequestTypeDef",
+    {
+        "EgressGatewayBridge": AddEgressGatewayBridgeRequestTypeDef,
+        "IngressGatewayBridge": AddIngressGatewayBridgeRequestTypeDef,
+        "Outputs": Sequence[AddBridgeOutputRequestTypeDef],
+        "SourceFailoverConfig": FailoverConfigTypeDef,
+    },
+    total=False,
+)
+
+class CreateBridgeRequestRequestTypeDef(
+    _RequiredCreateBridgeRequestRequestTypeDef, _OptionalCreateBridgeRequestRequestTypeDef
+):
+    pass
+
+AddBridgeSourcesResponseTypeDef = TypedDict(
+    "AddBridgeSourcesResponseTypeDef",
+    {
+        "BridgeArn": str,
+        "Sources": List[BridgeSourceTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredBridgeTypeDef = TypedDict(
+    "_RequiredBridgeTypeDef",
+    {
+        "BridgeArn": str,
+        "BridgeState": BridgeStateType,
+        "Name": str,
+        "PlacementArn": str,
+    },
+)
+_OptionalBridgeTypeDef = TypedDict(
+    "_OptionalBridgeTypeDef",
+    {
+        "BridgeMessages": List[MessageDetailTypeDef],
+        "EgressGatewayBridge": EgressGatewayBridgeTypeDef,
+        "IngressGatewayBridge": IngressGatewayBridgeTypeDef,
+        "Outputs": List[BridgeOutputTypeDef],
+        "SourceFailoverConfig": FailoverConfigTypeDef,
+        "Sources": List[BridgeSourceTypeDef],
+    },
+    total=False,
+)
+
+class BridgeTypeDef(_RequiredBridgeTypeDef, _OptionalBridgeTypeDef):
+    pass
+
+UpdateBridgeSourceResponseTypeDef = TypedDict(
+    "UpdateBridgeSourceResponseTypeDef",
+    {
+        "BridgeArn": str,
+        "Source": BridgeSourceTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredAddOutputRequestTypeDef = TypedDict(
     "_RequiredAddOutputRequestTypeDef",
     {
         "Protocol": ProtocolType,
     },
 )
 _OptionalAddOutputRequestTypeDef = TypedDict(
@@ -1340,14 +2250,15 @@
         "SenderControlPort": int,
         "SenderIpAddress": str,
         "SourceListenerAddress": str,
         "SourceListenerPort": int,
         "StreamId": str,
         "VpcInterfaceName": str,
         "WhitelistCidr": str,
+        "GatewayBridgeSource": SetGatewayBridgeSourceRequestTypeDef,
     },
     total=False,
 )
 
 _RequiredUpdateFlowSourceRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFlowSourceRequestRequestTypeDef",
     {
@@ -1371,14 +2282,15 @@
         "SenderControlPort": int,
         "SenderIpAddress": str,
         "SourceListenerAddress": str,
         "SourceListenerPort": int,
         "StreamId": str,
         "VpcInterfaceName": str,
         "WhitelistCidr": str,
+        "GatewayBridgeSource": UpdateGatewayBridgeSourceRequestTypeDef,
     },
     total=False,
 )
 
 class UpdateFlowSourceRequestRequestTypeDef(
     _RequiredUpdateFlowSourceRequestRequestTypeDef, _OptionalUpdateFlowSourceRequestRequestTypeDef
 ):
@@ -1401,14 +2313,16 @@
         "EntitlementArn": str,
         "ListenerAddress": str,
         "MediaLiveInputArn": str,
         "MediaStreamOutputConfigurations": List[MediaStreamOutputConfigurationTypeDef],
         "Port": int,
         "Transport": TransportTypeDef,
         "VpcInterfaceAttachment": VpcInterfaceAttachmentTypeDef,
+        "BridgeArn": str,
+        "BridgePorts": List[int],
     },
     total=False,
 )
 
 class OutputTypeDef(_RequiredOutputTypeDef, _OptionalOutputTypeDef):
     pass
 
@@ -1430,14 +2344,15 @@
         "IngestPort": int,
         "MediaStreamSourceConfigurations": List[MediaStreamSourceConfigurationTypeDef],
         "SenderControlPort": int,
         "SenderIpAddress": str,
         "Transport": TransportTypeDef,
         "VpcInterfaceName": str,
         "WhitelistCidr": str,
+        "GatewayBridgeSource": GatewayBridgeSourceTypeDef,
     },
     total=False,
 )
 
 class SourceTypeDef(_RequiredSourceTypeDef, _OptionalSourceTypeDef):
     pass
 
@@ -1463,14 +2378,38 @@
     {
         "FlowArn": str,
         "MediaStream": MediaStreamTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+CreateBridgeResponseTypeDef = TypedDict(
+    "CreateBridgeResponseTypeDef",
+    {
+        "Bridge": BridgeTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeBridgeResponseTypeDef = TypedDict(
+    "DescribeBridgeResponseTypeDef",
+    {
+        "Bridge": BridgeTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateBridgeResponseTypeDef = TypedDict(
+    "UpdateBridgeResponseTypeDef",
+    {
+        "Bridge": BridgeTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 AddFlowOutputsRequestRequestTypeDef = TypedDict(
     "AddFlowOutputsRequestRequestTypeDef",
     {
         "FlowArn": str,
         "Outputs": Sequence[AddOutputRequestTypeDef],
     },
 )
```

### Comparing `mypy-boto3-mediaconnect-1.26.0.post1/mypy_boto3_mediaconnect/waiter.py` & `mypy-boto3-mediaconnect-1.26.113/mypy_boto3_mediaconnect/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediaconnect-1.26.0.post1/mypy_boto3_mediaconnect/waiter.pyi` & `mypy-boto3-mediaconnect-1.26.113/mypy_boto3_mediaconnect/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediaconnect-1.26.0.post1/mypy_boto3_mediaconnect.egg-info/SOURCES.txt` & `mypy-boto3-mediaconnect-1.26.113/mypy_boto3_mediaconnect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediaconnect-1.26.0.post1/setup.py` & `mypy-boto3-mediaconnect-1.26.113/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 """
 Setup script for mypy-boto3-mediaconnect.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-mediaconnect",
-    version="1.26.0.post1",
+    version="1.26.113",
     packages=["mypy_boto3_mediaconnect"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.MediaConnect 1.26.0 service generated with mypy-boto3-builder"
-        " 7.11.10"
+        "Type annotations for boto3.MediaConnect 1.26.113 service generated with mypy-boto3-builder"
+        " 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
         "Typing :: Typed",
     ],
     keywords="boto3 mediaconnect type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_mediaconnect": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_mediaconnect": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
-        "typing-extensions>=4.1.0",
+        'typing-extensions>=4.1.0; python_version<"3.9"',
     ],
     zip_safe=False,
 )
```

