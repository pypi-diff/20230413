# Comparing `tmp/mypy-boto3-groundstation-1.26.6.tar.gz` & `tmp/mypy-boto3-groundstation-1.26.61.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-groundstation-1.26.6.tar", last modified: Wed Nov  9 20:50:02 2022, max compression
+gzip compressed data, was "mypy-boto3-groundstation-1.26.61.tar", last modified: Tue Jan 31 20:49:56 2023, max compression
```

## Comparing `mypy-boto3-groundstation-1.26.6.tar` & `mypy-boto3-groundstation-1.26.61.tar`

### file list

```diff
@@ -1,27 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 20:50:02.847553 mypy-boto3-groundstation-1.26.6/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-09 20:49:49.000000 mypy-boto3-groundstation-1.26.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    17815 2022-11-09 20:50:02.847553 mypy-boto3-groundstation-1.26.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    16356 2022-11-09 20:49:49.000000 mypy-boto3-groundstation-1.26.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 20:50:02.847553 mypy-boto3-groundstation-1.26.6/mypy_boto3_groundstation/
--rw-r--r--   0 runner    (1001) docker     (121)     1900 2022-11-09 20:49:49.000000 mypy-boto3-groundstation-1.26.6/mypy_boto3_groundstation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1899 2022-11-09 20:49:49.000000 mypy-boto3-groundstation-1.26.6/mypy_boto3_groundstation/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      929 2022-11-09 20:49:49.000000 mypy-boto3-groundstation-1.26.6/mypy_boto3_groundstation/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    24327 2022-11-09 20:49:50.000000 mypy-boto3-groundstation-1.26.6/mypy_boto3_groundstation/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    24283 2022-11-09 20:49:50.000000 mypy-boto3-groundstation-1.26.6/mypy_boto3_groundstation/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     9555 2022-11-09 20:49:50.000000 mypy-boto3-groundstation-1.26.6/mypy_boto3_groundstation/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)     9553 2022-11-09 20:49:50.000000 mypy-boto3-groundstation-1.26.6/mypy_boto3_groundstation/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     8978 2022-11-09 20:49:50.000000 mypy-boto3-groundstation-1.26.6/mypy_boto3_groundstation/paginator.py
--rw-r--r--   0 runner    (1001) docker     (121)     8969 2022-11-09 20:49:50.000000 mypy-boto3-groundstation-1.26.6/mypy_boto3_groundstation/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-09 20:49:49.000000 mypy-boto3-groundstation-1.26.6/mypy_boto3_groundstation/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    33053 2022-11-09 20:49:51.000000 mypy-boto3-groundstation-1.26.6/mypy_boto3_groundstation/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)    33018 2022-11-09 20:49:51.000000 mypy-boto3-groundstation-1.26.6/mypy_boto3_groundstation/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-11-09 20:49:49.000000 mypy-boto3-groundstation-1.26.6/mypy_boto3_groundstation/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 20:50:02.847553 mypy-boto3-groundstation-1.26.6/mypy_boto3_groundstation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    17815 2022-11-09 20:50:02.000000 mypy-boto3-groundstation-1.26.6/mypy_boto3_groundstation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      794 2022-11-09 20:50:02.000000 mypy-boto3-groundstation-1.26.6/mypy_boto3_groundstation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-09 20:50:02.000000 mypy-boto3-groundstation-1.26.6/mypy_boto3_groundstation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-09 20:50:02.000000 mypy-boto3-groundstation-1.26.6/mypy_boto3_groundstation.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-09 20:50:02.000000 mypy-boto3-groundstation-1.26.6/mypy_boto3_groundstation.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-09 20:50:02.000000 mypy-boto3-groundstation-1.26.6/mypy_boto3_groundstation.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-09 20:50:02.847553 mypy-boto3-groundstation-1.26.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2004 2022-11-09 20:49:48.000000 mypy-boto3-groundstation-1.26.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 20:49:56.862166 mypy-boto3-groundstation-1.26.61/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-01-31 20:48:28.000000 mypy-boto3-groundstation-1.26.61/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19249 2023-01-31 20:49:56.858166 mypy-boto3-groundstation-1.26.61/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17738 2023-01-31 20:48:28.000000 mypy-boto3-groundstation-1.26.61/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 20:49:56.850166 mypy-boto3-groundstation-1.26.61/mypy_boto3_groundstation/
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-01-31 20:48:28.000000 mypy-boto3-groundstation-1.26.61/mypy_boto3_groundstation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-01-31 20:48:28.000000 mypy-boto3-groundstation-1.26.61/mypy_boto3_groundstation/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-01-31 20:48:28.000000 mypy-boto3-groundstation-1.26.61/mypy_boto3_groundstation/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26979 2023-01-31 20:48:30.000000 mypy-boto3-groundstation-1.26.61/mypy_boto3_groundstation/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26931 2023-01-31 20:48:30.000000 mypy-boto3-groundstation-1.26.61/mypy_boto3_groundstation/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10404 2023-01-31 20:48:30.000000 mypy-boto3-groundstation-1.26.61/mypy_boto3_groundstation/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10402 2023-01-31 20:48:30.000000 mypy-boto3-groundstation-1.26.61/mypy_boto3_groundstation/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8978 2023-01-31 20:48:30.000000 mypy-boto3-groundstation-1.26.61/mypy_boto3_groundstation/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-01-31 20:48:30.000000 mypy-boto3-groundstation-1.26.61/mypy_boto3_groundstation/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-31 20:48:28.000000 mypy-boto3-groundstation-1.26.61/mypy_boto3_groundstation/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    39742 2023-01-31 20:48:31.000000 mypy-boto3-groundstation-1.26.61/mypy_boto3_groundstation/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39695 2023-01-31 20:48:31.000000 mypy-boto3-groundstation-1.26.61/mypy_boto3_groundstation/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-01-31 20:48:28.000000 mypy-boto3-groundstation-1.26.61/mypy_boto3_groundstation/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-01-31 20:48:30.000000 mypy-boto3-groundstation-1.26.61/mypy_boto3_groundstation/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-01-31 20:48:30.000000 mypy-boto3-groundstation-1.26.61/mypy_boto3_groundstation/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 20:49:56.858166 mypy-boto3-groundstation-1.26.61/mypy_boto3_groundstation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19249 2023-01-31 20:49:56.000000 mypy-boto3-groundstation-1.26.61/mypy_boto3_groundstation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-01-31 20:49:56.000000 mypy-boto3-groundstation-1.26.61/mypy_boto3_groundstation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-31 20:49:56.000000 mypy-boto3-groundstation-1.26.61/mypy_boto3_groundstation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-31 20:49:56.000000 mypy-boto3-groundstation-1.26.61/mypy_boto3_groundstation.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-01-31 20:49:56.000000 mypy-boto3-groundstation-1.26.61/mypy_boto3_groundstation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-01-31 20:49:56.000000 mypy-boto3-groundstation-1.26.61/mypy_boto3_groundstation.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-31 20:49:56.862166 mypy-boto3-groundstation-1.26.61/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-01-31 20:48:28.000000 mypy-boto3-groundstation-1.26.61/setup.py
```

### Comparing `mypy-boto3-groundstation-1.26.6/LICENSE` & `mypy-boto3-groundstation-1.26.61/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-groundstation-1.26.6/PKG-INFO` & `mypy-boto3-groundstation-1.26.61/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-groundstation
-Version: 1.26.6
-Summary: Type annotations for boto3.GroundStation 1.26.6 service generated with mypy-boto3-builder 7.11.10
+Version: 1.26.61
+Summary: Type annotations for boto3.GroundStation 1.26.61 service generated with mypy-boto3-builder 7.12.3
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -18,14 +18,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -37,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-groundstation.svg?color=blue)](https://pypi.org/project/mypy-boto3-groundstation)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-groundstation?color=blue)](https://pypistats.org/packages/mypy-boto3-groundstation)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.GroundStation 1.26.6](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation)
+[boto3.GroundStation 1.26.61](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.10](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-groundstation docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/).
 
 See how it helps to find and fix potential bugs:
 
@@ -72,14 +73,15 @@
     - [Sublime Text](#sublime-text)
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
+    - [Waiters annotations](#waiters-annotations)
     - [Literals](#literals)
     - [Typed dictionaries](#typed-dictionaries)
   - [How it works](#how-it-works)
   - [What's new](#what's-new)
     - [Implemented features](#implemented-features)
     - [Latest changes](#latest-changes)
   - [Versioning](#versioning)
@@ -307,26 +309,50 @@
 )
 list_mission_profiles_paginator: ListMissionProfilesPaginator = client.get_paginator(
     "list_mission_profiles"
 )
 list_satellites_paginator: ListSatellitesPaginator = client.get_paginator("list_satellites")
 ```
 
+<a id="waiters-annotations"></a>
+
+### Waiters annotations
+
+`mypy_boto3_groundstation.waiter` module contains type annotations for all
+waiters.
+
+```python
+from boto3.session import Session
+
+from mypy_boto3_groundstation import GroundStationClient
+from mypy_boto3_groundstation.waiter import ContactScheduledWaiter
+
+client: GroundStationClient = Session().client("groundstation")
+
+# Explicit type annotations are optional here
+# Types should be correctly discovered by mypy and IDEs
+contact_scheduled_waiter: ContactScheduledWaiter = client.get_waiter("contact_scheduled")
+```
+
 <a id="literals"></a>
 
 ### Literals
 
 `mypy_boto3_groundstation.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
 ```python
 from mypy_boto3_groundstation.literals import (
+    AgentStatusType,
     AngleUnitsType,
+    AuditResultsType,
     BandwidthUnitsType,
+    ComponentTypeType,
     ConfigCapabilityTypeType,
+    ContactScheduledWaiterName,
     ContactStatusType,
     CriticalityType,
     EirpUnitsType,
     EndpointStatusType,
     EphemerisInvalidReasonType,
     EphemerisSourceType,
     EphemerisStatusType,
@@ -339,64 +365,72 @@
     ListMissionProfilesPaginatorName,
     ListSatellitesPaginatorName,
     PolarizationType,
     GroundStationServiceName,
     ServiceName,
     ResourceServiceName,
     PaginatorName,
+    WaiterName,
     RegionName,
 )
 
 
-def check_value(value: AngleUnitsType) -> bool:
+def check_value(value: AgentStatusType) -> bool:
     ...
 ```
 
 <a id="typed-dictionaries"></a>
 
 ### Typed dictionaries
 
 `mypy_boto3_groundstation.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_groundstation.type_defs import (
+    ComponentVersionTypeDef,
+    AggregateStatusTypeDef,
     AntennaDemodDecodeDetailsTypeDef,
     DecodeConfigTypeDef,
     DemodulationConfigTypeDef,
     EirpTypeDef,
     CancelContactRequestRequestTypeDef,
+    ComponentStatusDataTypeDef,
     S3RecordingDetailsTypeDef,
     ResponseMetadataTypeDef,
     ConfigListItemTypeDef,
     DataflowEndpointConfigTypeDef,
     S3RecordingConfigTypeDef,
     TrackingConfigTypeDef,
     UplinkEchoConfigTypeDef,
+    SocketAddressTypeDef,
     ElevationTypeDef,
-    CreateMissionProfileRequestRequestTypeDef,
+    KmsKeyTypeDef,
     DataflowEndpointListItemTypeDef,
-    SocketAddressTypeDef,
     DeleteConfigRequestRequestTypeDef,
     DeleteDataflowEndpointGroupRequestRequestTypeDef,
     DeleteEphemerisRequestRequestTypeDef,
     DeleteMissionProfileRequestRequestTypeDef,
+    WaiterConfigTypeDef,
     DescribeContactRequestRequestTypeDef,
     DescribeEphemerisRequestRequestTypeDef,
+    DiscoveryDataTypeDef,
     SecurityDetailsTypeDef,
     S3ObjectTypeDef,
     EphemerisMetaDataTypeDef,
     FrequencyBandwidthTypeDef,
     FrequencyTypeDef,
+    GetAgentConfigurationRequestRequestTypeDef,
     GetConfigRequestRequestTypeDef,
     GetDataflowEndpointGroupRequestRequestTypeDef,
     GetMinuteUsageRequestRequestTypeDef,
     GetMissionProfileRequestRequestTypeDef,
     GetSatelliteRequestRequestTypeDef,
     GroundStationDataTypeDef,
+    IntegerRangeTypeDef,
     PaginatorConfigTypeDef,
     ListConfigsRequestRequestTypeDef,
     ListContactsRequestRequestTypeDef,
     ListDataflowEndpointGroupsRequestRequestTypeDef,
     ListEphemeridesRequestRequestTypeDef,
     ListGroundStationsRequestRequestTypeDef,
     ListMissionProfilesRequestRequestTypeDef,
@@ -404,71 +438,83 @@
     ListSatellitesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ReserveContactRequestRequestTypeDef,
     TimeRangeTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateEphemerisRequestRequestTypeDef,
-    UpdateMissionProfileRequestRequestTypeDef,
+    AgentDetailsTypeDef,
+    UpdateAgentStatusRequestRequestTypeDef,
     ConfigIdResponseTypeDef,
     ContactIdResponseTypeDef,
     DataflowEndpointGroupIdResponseTypeDef,
     EphemerisIdResponseTypeDef,
+    GetAgentConfigurationResponseTypeDef,
     GetMinuteUsageResponseTypeDef,
-    GetMissionProfileResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     MissionProfileIdResponseTypeDef,
+    RegisterAgentResponseTypeDef,
+    UpdateAgentStatusResponseTypeDef,
     ListConfigsResponseTypeDef,
+    ConnectionDetailsTypeDef,
+    DataflowEndpointTypeDef,
     ContactDataTypeDef,
+    CreateMissionProfileRequestRequestTypeDef,
+    GetMissionProfileResponseTypeDef,
+    UpdateMissionProfileRequestRequestTypeDef,
     ListDataflowEndpointGroupsResponseTypeDef,
-    DataflowEndpointTypeDef,
+    DescribeContactRequestContactScheduledWaitTypeDef,
     EphemerisDescriptionTypeDef,
     EphemerisItemTypeDef,
     OEMEphemerisTypeDef,
     GetSatelliteResponseTypeDef,
     SatelliteListItemTypeDef,
     SpectrumConfigTypeDef,
     UplinkSpectrumConfigTypeDef,
     ListGroundStationsResponseTypeDef,
+    RangedSocketAddressTypeDef,
     ListConfigsRequestListConfigsPaginateTypeDef,
     ListContactsRequestListContactsPaginateTypeDef,
     ListDataflowEndpointGroupsRequestListDataflowEndpointGroupsPaginateTypeDef,
     ListEphemeridesRequestListEphemeridesPaginateTypeDef,
     ListGroundStationsRequestListGroundStationsPaginateTypeDef,
     ListMissionProfilesRequestListMissionProfilesPaginateTypeDef,
     ListSatellitesRequestListSatellitesPaginateTypeDef,
     ListMissionProfilesResponseTypeDef,
     TLEDataTypeDef,
+    RegisterAgentRequestRequestTypeDef,
     ListContactsResponseTypeDef,
-    EndpointDetailsTypeDef,
     EphemerisTypeDescriptionTypeDef,
     ListEphemeridesResponseTypeDef,
     ListSatellitesResponseTypeDef,
     AntennaDownlinkConfigTypeDef,
     AntennaDownlinkDemodDecodeConfigTypeDef,
     AntennaUplinkConfigTypeDef,
+    RangedConnectionDetailsTypeDef,
     TLEEphemerisTypeDef,
-    ConfigDetailsTypeDef,
-    CreateDataflowEndpointGroupRequestRequestTypeDef,
-    GetDataflowEndpointGroupResponseTypeDef,
     DescribeEphemerisResponseTypeDef,
     ConfigTypeDataTypeDef,
+    AwsGroundStationAgentEndpointTypeDef,
     EphemerisDataTypeDef,
-    DestinationTypeDef,
-    SourceTypeDef,
     CreateConfigRequestRequestTypeDef,
     GetConfigResponseTypeDef,
     UpdateConfigRequestRequestTypeDef,
+    EndpointDetailsTypeDef,
     CreateEphemerisRequestRequestTypeDef,
+    ConfigDetailsTypeDef,
+    CreateDataflowEndpointGroupRequestRequestTypeDef,
+    GetDataflowEndpointGroupResponseTypeDef,
+    DestinationTypeDef,
+    SourceTypeDef,
     DataflowDetailTypeDef,
     DescribeContactResponseTypeDef,
 )
 
 
-def get_structure() -> AntennaDemodDecodeDetailsTypeDef:
+def get_structure() -> ComponentVersionTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-groundstation-1.26.6/README.md` & `mypy-boto3-groundstation-1.26.61/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-groundstation.svg?color=blue)](https://pypi.org/project/mypy-boto3-groundstation)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-groundstation?color=blue)](https://pypistats.org/packages/mypy-boto3-groundstation)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.GroundStation 1.26.6](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation)
+[boto3.GroundStation 1.26.61](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.10](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-groundstation docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/).
 
 See how it helps to find and fix potential bugs:
 
@@ -41,14 +41,15 @@
     - [Sublime Text](#sublime-text)
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
+    - [Waiters annotations](#waiters-annotations)
     - [Literals](#literals)
     - [Typed dictionaries](#typed-dictionaries)
   - [How it works](#how-it-works)
   - [What's new](#what's-new)
     - [Implemented features](#implemented-features)
     - [Latest changes](#latest-changes)
   - [Versioning](#versioning)
@@ -276,26 +277,50 @@
 )
 list_mission_profiles_paginator: ListMissionProfilesPaginator = client.get_paginator(
     "list_mission_profiles"
 )
 list_satellites_paginator: ListSatellitesPaginator = client.get_paginator("list_satellites")
 ```
 
+<a id="waiters-annotations"></a>
+
+### Waiters annotations
+
+`mypy_boto3_groundstation.waiter` module contains type annotations for all
+waiters.
+
+```python
+from boto3.session import Session
+
+from mypy_boto3_groundstation import GroundStationClient
+from mypy_boto3_groundstation.waiter import ContactScheduledWaiter
+
+client: GroundStationClient = Session().client("groundstation")
+
+# Explicit type annotations are optional here
+# Types should be correctly discovered by mypy and IDEs
+contact_scheduled_waiter: ContactScheduledWaiter = client.get_waiter("contact_scheduled")
+```
+
 <a id="literals"></a>
 
 ### Literals
 
 `mypy_boto3_groundstation.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
 ```python
 from mypy_boto3_groundstation.literals import (
+    AgentStatusType,
     AngleUnitsType,
+    AuditResultsType,
     BandwidthUnitsType,
+    ComponentTypeType,
     ConfigCapabilityTypeType,
+    ContactScheduledWaiterName,
     ContactStatusType,
     CriticalityType,
     EirpUnitsType,
     EndpointStatusType,
     EphemerisInvalidReasonType,
     EphemerisSourceType,
     EphemerisStatusType,
@@ -308,64 +333,72 @@
     ListMissionProfilesPaginatorName,
     ListSatellitesPaginatorName,
     PolarizationType,
     GroundStationServiceName,
     ServiceName,
     ResourceServiceName,
     PaginatorName,
+    WaiterName,
     RegionName,
 )
 
 
-def check_value(value: AngleUnitsType) -> bool:
+def check_value(value: AgentStatusType) -> bool:
     ...
 ```
 
 <a id="typed-dictionaries"></a>
 
 ### Typed dictionaries
 
 `mypy_boto3_groundstation.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_groundstation.type_defs import (
+    ComponentVersionTypeDef,
+    AggregateStatusTypeDef,
     AntennaDemodDecodeDetailsTypeDef,
     DecodeConfigTypeDef,
     DemodulationConfigTypeDef,
     EirpTypeDef,
     CancelContactRequestRequestTypeDef,
+    ComponentStatusDataTypeDef,
     S3RecordingDetailsTypeDef,
     ResponseMetadataTypeDef,
     ConfigListItemTypeDef,
     DataflowEndpointConfigTypeDef,
     S3RecordingConfigTypeDef,
     TrackingConfigTypeDef,
     UplinkEchoConfigTypeDef,
+    SocketAddressTypeDef,
     ElevationTypeDef,
-    CreateMissionProfileRequestRequestTypeDef,
+    KmsKeyTypeDef,
     DataflowEndpointListItemTypeDef,
-    SocketAddressTypeDef,
     DeleteConfigRequestRequestTypeDef,
     DeleteDataflowEndpointGroupRequestRequestTypeDef,
     DeleteEphemerisRequestRequestTypeDef,
     DeleteMissionProfileRequestRequestTypeDef,
+    WaiterConfigTypeDef,
     DescribeContactRequestRequestTypeDef,
     DescribeEphemerisRequestRequestTypeDef,
+    DiscoveryDataTypeDef,
     SecurityDetailsTypeDef,
     S3ObjectTypeDef,
     EphemerisMetaDataTypeDef,
     FrequencyBandwidthTypeDef,
     FrequencyTypeDef,
+    GetAgentConfigurationRequestRequestTypeDef,
     GetConfigRequestRequestTypeDef,
     GetDataflowEndpointGroupRequestRequestTypeDef,
     GetMinuteUsageRequestRequestTypeDef,
     GetMissionProfileRequestRequestTypeDef,
     GetSatelliteRequestRequestTypeDef,
     GroundStationDataTypeDef,
+    IntegerRangeTypeDef,
     PaginatorConfigTypeDef,
     ListConfigsRequestRequestTypeDef,
     ListContactsRequestRequestTypeDef,
     ListDataflowEndpointGroupsRequestRequestTypeDef,
     ListEphemeridesRequestRequestTypeDef,
     ListGroundStationsRequestRequestTypeDef,
     ListMissionProfilesRequestRequestTypeDef,
@@ -373,71 +406,83 @@
     ListSatellitesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ReserveContactRequestRequestTypeDef,
     TimeRangeTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateEphemerisRequestRequestTypeDef,
-    UpdateMissionProfileRequestRequestTypeDef,
+    AgentDetailsTypeDef,
+    UpdateAgentStatusRequestRequestTypeDef,
     ConfigIdResponseTypeDef,
     ContactIdResponseTypeDef,
     DataflowEndpointGroupIdResponseTypeDef,
     EphemerisIdResponseTypeDef,
+    GetAgentConfigurationResponseTypeDef,
     GetMinuteUsageResponseTypeDef,
-    GetMissionProfileResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     MissionProfileIdResponseTypeDef,
+    RegisterAgentResponseTypeDef,
+    UpdateAgentStatusResponseTypeDef,
     ListConfigsResponseTypeDef,
+    ConnectionDetailsTypeDef,
+    DataflowEndpointTypeDef,
     ContactDataTypeDef,
+    CreateMissionProfileRequestRequestTypeDef,
+    GetMissionProfileResponseTypeDef,
+    UpdateMissionProfileRequestRequestTypeDef,
     ListDataflowEndpointGroupsResponseTypeDef,
-    DataflowEndpointTypeDef,
+    DescribeContactRequestContactScheduledWaitTypeDef,
     EphemerisDescriptionTypeDef,
     EphemerisItemTypeDef,
     OEMEphemerisTypeDef,
     GetSatelliteResponseTypeDef,
     SatelliteListItemTypeDef,
     SpectrumConfigTypeDef,
     UplinkSpectrumConfigTypeDef,
     ListGroundStationsResponseTypeDef,
+    RangedSocketAddressTypeDef,
     ListConfigsRequestListConfigsPaginateTypeDef,
     ListContactsRequestListContactsPaginateTypeDef,
     ListDataflowEndpointGroupsRequestListDataflowEndpointGroupsPaginateTypeDef,
     ListEphemeridesRequestListEphemeridesPaginateTypeDef,
     ListGroundStationsRequestListGroundStationsPaginateTypeDef,
     ListMissionProfilesRequestListMissionProfilesPaginateTypeDef,
     ListSatellitesRequestListSatellitesPaginateTypeDef,
     ListMissionProfilesResponseTypeDef,
     TLEDataTypeDef,
+    RegisterAgentRequestRequestTypeDef,
     ListContactsResponseTypeDef,
-    EndpointDetailsTypeDef,
     EphemerisTypeDescriptionTypeDef,
     ListEphemeridesResponseTypeDef,
     ListSatellitesResponseTypeDef,
     AntennaDownlinkConfigTypeDef,
     AntennaDownlinkDemodDecodeConfigTypeDef,
     AntennaUplinkConfigTypeDef,
+    RangedConnectionDetailsTypeDef,
     TLEEphemerisTypeDef,
-    ConfigDetailsTypeDef,
-    CreateDataflowEndpointGroupRequestRequestTypeDef,
-    GetDataflowEndpointGroupResponseTypeDef,
     DescribeEphemerisResponseTypeDef,
     ConfigTypeDataTypeDef,
+    AwsGroundStationAgentEndpointTypeDef,
     EphemerisDataTypeDef,
-    DestinationTypeDef,
-    SourceTypeDef,
     CreateConfigRequestRequestTypeDef,
     GetConfigResponseTypeDef,
     UpdateConfigRequestRequestTypeDef,
+    EndpointDetailsTypeDef,
     CreateEphemerisRequestRequestTypeDef,
+    ConfigDetailsTypeDef,
+    CreateDataflowEndpointGroupRequestRequestTypeDef,
+    GetDataflowEndpointGroupResponseTypeDef,
+    DestinationTypeDef,
+    SourceTypeDef,
     DataflowDetailTypeDef,
     DescribeContactResponseTypeDef,
 )
 
 
-def get_structure() -> AntennaDemodDecodeDetailsTypeDef:
+def get_structure() -> ComponentVersionTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-groundstation-1.26.6/mypy_boto3_groundstation/__init__.py` & `mypy-boto3-groundstation-1.26.61/mypy_boto3_groundstation/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,27 +3,30 @@
 
 Usage::
 
     ```python
     from boto3.session import Session
     from mypy_boto3_groundstation import (
         Client,
+        ContactScheduledWaiter,
         GroundStationClient,
         ListConfigsPaginator,
         ListContactsPaginator,
         ListDataflowEndpointGroupsPaginator,
         ListEphemeridesPaginator,
         ListGroundStationsPaginator,
         ListMissionProfilesPaginator,
         ListSatellitesPaginator,
     )
 
     session = Session()
     client: GroundStationClient = session.client("groundstation")
 
+    contact_scheduled_waiter: ContactScheduledWaiter = client.get_waiter("contact_scheduled")
+
     list_configs_paginator: ListConfigsPaginator = client.get_paginator("list_configs")
     list_contacts_paginator: ListContactsPaginator = client.get_paginator("list_contacts")
     list_dataflow_endpoint_groups_paginator: ListDataflowEndpointGroupsPaginator = client.get_paginator("list_dataflow_endpoint_groups")
     list_ephemerides_paginator: ListEphemeridesPaginator = client.get_paginator("list_ephemerides")
     list_ground_stations_paginator: ListGroundStationsPaginator = client.get_paginator("list_ground_stations")
     list_mission_profiles_paginator: ListMissionProfilesPaginator = client.get_paginator("list_mission_profiles")
     list_satellites_paginator: ListSatellitesPaginator = client.get_paginator("list_satellites")
@@ -35,20 +38,22 @@
     ListContactsPaginator,
     ListDataflowEndpointGroupsPaginator,
     ListEphemeridesPaginator,
     ListGroundStationsPaginator,
     ListMissionProfilesPaginator,
     ListSatellitesPaginator,
 )
+from .waiter import ContactScheduledWaiter
 
 Client = GroundStationClient
 
 
 __all__ = (
     "Client",
+    "ContactScheduledWaiter",
     "GroundStationClient",
     "ListConfigsPaginator",
     "ListContactsPaginator",
     "ListDataflowEndpointGroupsPaginator",
     "ListEphemeridesPaginator",
     "ListGroundStationsPaginator",
     "ListMissionProfilesPaginator",
```

### Comparing `mypy-boto3-groundstation-1.26.6/mypy_boto3_groundstation/__init__.pyi` & `mypy-boto3-groundstation-1.26.61/mypy_boto3_groundstation/__init__.pyi`

 * *Files 19% similar despite different names*

```diff
@@ -3,27 +3,30 @@
 
 Usage::
 
     ```python
     from boto3.session import Session
     from mypy_boto3_groundstation import (
         Client,
+        ContactScheduledWaiter,
         GroundStationClient,
         ListConfigsPaginator,
         ListContactsPaginator,
         ListDataflowEndpointGroupsPaginator,
         ListEphemeridesPaginator,
         ListGroundStationsPaginator,
         ListMissionProfilesPaginator,
         ListSatellitesPaginator,
     )
 
     session = Session()
     client: GroundStationClient = session.client("groundstation")
 
+    contact_scheduled_waiter: ContactScheduledWaiter = client.get_waiter("contact_scheduled")
+
     list_configs_paginator: ListConfigsPaginator = client.get_paginator("list_configs")
     list_contacts_paginator: ListContactsPaginator = client.get_paginator("list_contacts")
     list_dataflow_endpoint_groups_paginator: ListDataflowEndpointGroupsPaginator = client.get_paginator("list_dataflow_endpoint_groups")
     list_ephemerides_paginator: ListEphemeridesPaginator = client.get_paginator("list_ephemerides")
     list_ground_stations_paginator: ListGroundStationsPaginator = client.get_paginator("list_ground_stations")
     list_mission_profiles_paginator: ListMissionProfilesPaginator = client.get_paginator("list_mission_profiles")
     list_satellites_paginator: ListSatellitesPaginator = client.get_paginator("list_satellites")
@@ -35,19 +38,21 @@
     ListContactsPaginator,
     ListDataflowEndpointGroupsPaginator,
     ListEphemeridesPaginator,
     ListGroundStationsPaginator,
     ListMissionProfilesPaginator,
     ListSatellitesPaginator,
 )
+from .waiter import ContactScheduledWaiter
 
 Client = GroundStationClient
 
 __all__ = (
     "Client",
+    "ContactScheduledWaiter",
     "GroundStationClient",
     "ListConfigsPaginator",
     "ListContactsPaginator",
     "ListDataflowEndpointGroupsPaginator",
     "ListEphemeridesPaginator",
     "ListGroundStationsPaginator",
     "ListMissionProfilesPaginator",
```

### Comparing `mypy-boto3-groundstation-1.26.6/mypy_boto3_groundstation/__main__.py` & `mypy-boto3-groundstation-1.26.61/mypy_boto3_groundstation/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.GroundStation 1.26.6\nVersion:         1.26.6\nBuilder version:"
-        " 7.11.10\nDocs:           "
+        "Type annotations for boto3.GroundStation 1.26.61\nVersion:         1.26.61\nBuilder"
+        " version: 7.12.3\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.6")
+    print("1.26.61")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-groundstation-1.26.6/mypy_boto3_groundstation/client.py` & `mypy-boto3-groundstation-1.26.61/mypy_boto3_groundstation/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,38 +26,47 @@
     ListDataflowEndpointGroupsPaginator,
     ListEphemeridesPaginator,
     ListGroundStationsPaginator,
     ListMissionProfilesPaginator,
     ListSatellitesPaginator,
 )
 from .type_defs import (
+    AgentDetailsTypeDef,
+    AggregateStatusTypeDef,
+    ComponentStatusDataTypeDef,
     ConfigIdResponseTypeDef,
     ConfigTypeDataTypeDef,
     ContactIdResponseTypeDef,
     DataflowEndpointGroupIdResponseTypeDef,
     DescribeContactResponseTypeDef,
     DescribeEphemerisResponseTypeDef,
+    DiscoveryDataTypeDef,
     EndpointDetailsTypeDef,
     EphemerisDataTypeDef,
     EphemerisIdResponseTypeDef,
+    GetAgentConfigurationResponseTypeDef,
     GetConfigResponseTypeDef,
     GetDataflowEndpointGroupResponseTypeDef,
     GetMinuteUsageResponseTypeDef,
     GetMissionProfileResponseTypeDef,
     GetSatelliteResponseTypeDef,
+    KmsKeyTypeDef,
     ListConfigsResponseTypeDef,
     ListContactsResponseTypeDef,
     ListDataflowEndpointGroupsResponseTypeDef,
     ListEphemeridesResponseTypeDef,
     ListGroundStationsResponseTypeDef,
     ListMissionProfilesResponseTypeDef,
     ListSatellitesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     MissionProfileIdResponseTypeDef,
+    RegisterAgentResponseTypeDef,
+    UpdateAgentStatusResponseTypeDef,
 )
+from .waiter import ContactScheduledWaiter
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 
@@ -128,15 +137,20 @@
         Creates a `Config` with the specified `configData` parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.create_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/client/#create_config)
         """
 
     def create_dataflow_endpoint_group(
-        self, *, endpointDetails: Sequence[EndpointDetailsTypeDef], tags: Mapping[str, str] = ...
+        self,
+        *,
+        endpointDetails: Sequence[EndpointDetailsTypeDef],
+        contactPostPassDurationSeconds: int = ...,
+        contactPrePassDurationSeconds: int = ...,
+        tags: Mapping[str, str] = ...
     ) -> DataflowEndpointGroupIdResponseTypeDef:
         """
         Creates a `DataflowEndpoint` group containing the specified list of
         `DataflowEndpoint` objects.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.create_dataflow_endpoint_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/client/#create_dataflow_endpoint_group)
@@ -166,14 +180,16 @@
         *,
         dataflowEdges: Sequence[Sequence[str]],
         minimumViableContactDurationSeconds: int,
         name: str,
         trackingConfigArn: str,
         contactPostPassDurationSeconds: int = ...,
         contactPrePassDurationSeconds: int = ...,
+        streamsKmsKey: KmsKeyTypeDef = ...,
+        streamsKmsRole: str = ...,
         tags: Mapping[str, str] = ...
     ) -> MissionProfileIdResponseTypeDef:
         """
         Creates a mission profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.create_mission_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/client/#create_mission_profile)
@@ -242,14 +258,22 @@
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/client/#generate_presigned_url)
         """
 
+    def get_agent_configuration(self, *, agentId: str) -> GetAgentConfigurationResponseTypeDef:
+        """
+        Gets the latest configuration information for a registered agent.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.get_agent_configuration)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/client/#get_agent_configuration)
+        """
+
     def get_config(
         self, *, configId: str, configType: ConfigCapabilityTypeType
     ) -> GetConfigResponseTypeDef:
         """
         Returns `Config` information.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.get_config)
@@ -380,14 +404,24 @@
         """
         Returns a list of tags for a specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/client/#list_tags_for_resource)
         """
 
+    def register_agent(
+        self, *, agentDetails: AgentDetailsTypeDef, discoveryData: DiscoveryDataTypeDef
+    ) -> RegisterAgentResponseTypeDef:
+        """
+        Registers a new agent with AWS Groundstation.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.register_agent)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/client/#register_agent)
+        """
+
     def reserve_contact(
         self,
         *,
         endTime: Union[datetime, str],
         groundStation: str,
         missionProfileArn: str,
         satelliteArn: str,
@@ -413,14 +447,29 @@
         """
         Deassigns a resource tag.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/client/#untag_resource)
         """
 
+    def update_agent_status(
+        self,
+        *,
+        agentId: str,
+        aggregateStatus: AggregateStatusTypeDef,
+        componentStatuses: Sequence[ComponentStatusDataTypeDef],
+        taskId: str
+    ) -> UpdateAgentStatusResponseTypeDef:
+        """
+        Update the status of the agent.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.update_agent_status)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/client/#update_agent_status)
+        """
+
     def update_config(
         self,
         *,
         configData: ConfigTypeDataTypeDef,
         configId: str,
         configType: ConfigCapabilityTypeType,
         name: str
@@ -448,14 +497,16 @@
         *,
         missionProfileId: str,
         contactPostPassDurationSeconds: int = ...,
         contactPrePassDurationSeconds: int = ...,
         dataflowEdges: Sequence[Sequence[str]] = ...,
         minimumViableContactDurationSeconds: int = ...,
         name: str = ...,
+        streamsKmsKey: KmsKeyTypeDef = ...,
+        streamsKmsRole: str = ...,
         trackingConfigArn: str = ...
     ) -> MissionProfileIdResponseTypeDef:
         """
         Updates a mission profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.update_mission_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/client/#update_mission_profile)
@@ -513,7 +564,13 @@
 
     @overload
     def get_paginator(self, operation_name: Literal["list_satellites"]) -> ListSatellitesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/client/#get_paginator)
         """
+
+    def get_waiter(self, waiter_name: Literal["contact_scheduled"]) -> ContactScheduledWaiter:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.get_waiter)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/client/#get_waiter)
+        """
```

### Comparing `mypy-boto3-groundstation-1.26.6/mypy_boto3_groundstation/client.pyi` & `mypy-boto3-groundstation-1.26.61/mypy_boto3_groundstation/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -26,38 +26,47 @@
     ListDataflowEndpointGroupsPaginator,
     ListEphemeridesPaginator,
     ListGroundStationsPaginator,
     ListMissionProfilesPaginator,
     ListSatellitesPaginator,
 )
 from .type_defs import (
+    AgentDetailsTypeDef,
+    AggregateStatusTypeDef,
+    ComponentStatusDataTypeDef,
     ConfigIdResponseTypeDef,
     ConfigTypeDataTypeDef,
     ContactIdResponseTypeDef,
     DataflowEndpointGroupIdResponseTypeDef,
     DescribeContactResponseTypeDef,
     DescribeEphemerisResponseTypeDef,
+    DiscoveryDataTypeDef,
     EndpointDetailsTypeDef,
     EphemerisDataTypeDef,
     EphemerisIdResponseTypeDef,
+    GetAgentConfigurationResponseTypeDef,
     GetConfigResponseTypeDef,
     GetDataflowEndpointGroupResponseTypeDef,
     GetMinuteUsageResponseTypeDef,
     GetMissionProfileResponseTypeDef,
     GetSatelliteResponseTypeDef,
+    KmsKeyTypeDef,
     ListConfigsResponseTypeDef,
     ListContactsResponseTypeDef,
     ListDataflowEndpointGroupsResponseTypeDef,
     ListEphemeridesResponseTypeDef,
     ListGroundStationsResponseTypeDef,
     ListMissionProfilesResponseTypeDef,
     ListSatellitesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     MissionProfileIdResponseTypeDef,
+    RegisterAgentResponseTypeDef,
+    UpdateAgentStatusResponseTypeDef,
 )
+from .waiter import ContactScheduledWaiter
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 __all__ = ("GroundStationClient",)
@@ -119,15 +128,20 @@
         """
         Creates a `Config` with the specified `configData` parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.create_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/client/#create_config)
         """
     def create_dataflow_endpoint_group(
-        self, *, endpointDetails: Sequence[EndpointDetailsTypeDef], tags: Mapping[str, str] = ...
+        self,
+        *,
+        endpointDetails: Sequence[EndpointDetailsTypeDef],
+        contactPostPassDurationSeconds: int = ...,
+        contactPrePassDurationSeconds: int = ...,
+        tags: Mapping[str, str] = ...
     ) -> DataflowEndpointGroupIdResponseTypeDef:
         """
         Creates a `DataflowEndpoint` group containing the specified list of
         `DataflowEndpoint` objects.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.create_dataflow_endpoint_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/client/#create_dataflow_endpoint_group)
@@ -155,14 +169,16 @@
         *,
         dataflowEdges: Sequence[Sequence[str]],
         minimumViableContactDurationSeconds: int,
         name: str,
         trackingConfigArn: str,
         contactPostPassDurationSeconds: int = ...,
         contactPrePassDurationSeconds: int = ...,
+        streamsKmsKey: KmsKeyTypeDef = ...,
+        streamsKmsRole: str = ...,
         tags: Mapping[str, str] = ...
     ) -> MissionProfileIdResponseTypeDef:
         """
         Creates a mission profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.create_mission_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/client/#create_mission_profile)
@@ -223,14 +239,21 @@
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/client/#generate_presigned_url)
         """
+    def get_agent_configuration(self, *, agentId: str) -> GetAgentConfigurationResponseTypeDef:
+        """
+        Gets the latest configuration information for a registered agent.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.get_agent_configuration)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/client/#get_agent_configuration)
+        """
     def get_config(
         self, *, configId: str, configType: ConfigCapabilityTypeType
     ) -> GetConfigResponseTypeDef:
         """
         Returns `Config` information.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.get_config)
@@ -348,14 +371,23 @@
     def list_tags_for_resource(self, *, resourceArn: str) -> ListTagsForResourceResponseTypeDef:
         """
         Returns a list of tags for a specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/client/#list_tags_for_resource)
         """
+    def register_agent(
+        self, *, agentDetails: AgentDetailsTypeDef, discoveryData: DiscoveryDataTypeDef
+    ) -> RegisterAgentResponseTypeDef:
+        """
+        Registers a new agent with AWS Groundstation.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.register_agent)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/client/#register_agent)
+        """
     def reserve_contact(
         self,
         *,
         endTime: Union[datetime, str],
         groundStation: str,
         missionProfileArn: str,
         satelliteArn: str,
@@ -378,14 +410,28 @@
     def untag_resource(self, *, resourceArn: str, tagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         Deassigns a resource tag.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/client/#untag_resource)
         """
+    def update_agent_status(
+        self,
+        *,
+        agentId: str,
+        aggregateStatus: AggregateStatusTypeDef,
+        componentStatuses: Sequence[ComponentStatusDataTypeDef],
+        taskId: str
+    ) -> UpdateAgentStatusResponseTypeDef:
+        """
+        Update the status of the agent.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.update_agent_status)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/client/#update_agent_status)
+        """
     def update_config(
         self,
         *,
         configData: ConfigTypeDataTypeDef,
         configId: str,
         configType: ConfigCapabilityTypeType,
         name: str
@@ -411,14 +457,16 @@
         *,
         missionProfileId: str,
         contactPostPassDurationSeconds: int = ...,
         contactPrePassDurationSeconds: int = ...,
         dataflowEdges: Sequence[Sequence[str]] = ...,
         minimumViableContactDurationSeconds: int = ...,
         name: str = ...,
+        streamsKmsKey: KmsKeyTypeDef = ...,
+        streamsKmsRole: str = ...,
         trackingConfigArn: str = ...
     ) -> MissionProfileIdResponseTypeDef:
         """
         Updates a mission profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.update_mission_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/client/#update_mission_profile)
@@ -469,7 +517,12 @@
         """
     @overload
     def get_paginator(self, operation_name: Literal["list_satellites"]) -> ListSatellitesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/client/#get_paginator)
         """
+    def get_waiter(self, waiter_name: Literal["contact_scheduled"]) -> ContactScheduledWaiter:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.get_waiter)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/client/#get_waiter)
+        """
```

### Comparing `mypy-boto3-groundstation-1.26.6/mypy_boto3_groundstation/literals.py` & `mypy-boto3-groundstation-1.26.61/mypy_boto3_groundstation/literals.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,31 +2,35 @@
 Type annotations for groundstation service literal definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/literals/)
 
 Usage::
 
     ```python
-    from mypy_boto3_groundstation.literals import AngleUnitsType
+    from mypy_boto3_groundstation.literals import AgentStatusType
 
-    data: AngleUnitsType = "DEGREE_ANGLE"
+    data: AgentStatusType = "ACTIVE"
     ```
 """
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 
 __all__ = (
+    "AgentStatusType",
     "AngleUnitsType",
+    "AuditResultsType",
     "BandwidthUnitsType",
+    "ComponentTypeType",
     "ConfigCapabilityTypeType",
+    "ContactScheduledWaiterName",
     "ContactStatusType",
     "CriticalityType",
     "EirpUnitsType",
     "EndpointStatusType",
     "EphemerisInvalidReasonType",
     "EphemerisSourceType",
     "EphemerisStatusType",
@@ -39,29 +43,34 @@
     "ListMissionProfilesPaginatorName",
     "ListSatellitesPaginatorName",
     "PolarizationType",
     "GroundStationServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
+    "WaiterName",
     "RegionName",
 )
 
 
+AgentStatusType = Literal["ACTIVE", "FAILED", "INACTIVE", "SUCCESS"]
 AngleUnitsType = Literal["DEGREE_ANGLE", "RADIAN"]
+AuditResultsType = Literal["HEALTHY", "UNHEALTHY"]
 BandwidthUnitsType = Literal["GHz", "MHz", "kHz"]
+ComponentTypeType = Literal["DIGITIZER", "LAMINAR_FLOW", "PRISM"]
 ConfigCapabilityTypeType = Literal[
     "antenna-downlink",
     "antenna-downlink-demod-decode",
     "antenna-uplink",
     "dataflow-endpoint",
     "s3-recording",
     "tracking",
     "uplink-echo",
 ]
+ContactScheduledWaiterName = Literal["contact_scheduled"]
 ContactStatusType = Literal[
     "AVAILABLE",
     "AWS_CANCELLED",
     "AWS_FAILED",
     "CANCELLED",
     "CANCELLING",
     "COMPLETED",
@@ -115,14 +124,15 @@
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
@@ -132,27 +142,31 @@
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
@@ -181,14 +195,15 @@
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
@@ -236,14 +251,15 @@
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
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
@@ -254,30 +270,33 @@
     "iottwinmaker",
     "iotwireless",
     "ivs",
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
@@ -309,28 +328,32 @@
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
@@ -358,38 +381,44 @@
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
@@ -433,14 +462,15 @@
     "list_contacts",
     "list_dataflow_endpoint_groups",
     "list_ephemerides",
     "list_ground_stations",
     "list_mission_profiles",
     "list_satellites",
 ]
+WaiterName = Literal["contact_scheduled"]
 RegionName = Literal[
     "af-south-1",
     "ap-northeast-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "eu-central-1",
     "eu-north-1",
```

### Comparing `mypy-boto3-groundstation-1.26.6/mypy_boto3_groundstation/literals.pyi` & `mypy-boto3-groundstation-1.26.61/mypy_boto3_groundstation/literals.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -2,30 +2,34 @@
 Type annotations for groundstation service literal definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/literals/)
 
 Usage::
 
     ```python
-    from mypy_boto3_groundstation.literals import AngleUnitsType
+    from mypy_boto3_groundstation.literals import AgentStatusType
 
-    data: AngleUnitsType = "DEGREE_ANGLE"
+    data: AgentStatusType = "ACTIVE"
     ```
 """
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 __all__ = (
+    "AgentStatusType",
     "AngleUnitsType",
+    "AuditResultsType",
     "BandwidthUnitsType",
+    "ComponentTypeType",
     "ConfigCapabilityTypeType",
+    "ContactScheduledWaiterName",
     "ContactStatusType",
     "CriticalityType",
     "EirpUnitsType",
     "EndpointStatusType",
     "EphemerisInvalidReasonType",
     "EphemerisSourceType",
     "EphemerisStatusType",
@@ -38,28 +42,33 @@
     "ListMissionProfilesPaginatorName",
     "ListSatellitesPaginatorName",
     "PolarizationType",
     "GroundStationServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
+    "WaiterName",
     "RegionName",
 )
 
+AgentStatusType = Literal["ACTIVE", "FAILED", "INACTIVE", "SUCCESS"]
 AngleUnitsType = Literal["DEGREE_ANGLE", "RADIAN"]
+AuditResultsType = Literal["HEALTHY", "UNHEALTHY"]
 BandwidthUnitsType = Literal["GHz", "MHz", "kHz"]
+ComponentTypeType = Literal["DIGITIZER", "LAMINAR_FLOW", "PRISM"]
 ConfigCapabilityTypeType = Literal[
     "antenna-downlink",
     "antenna-downlink-demod-decode",
     "antenna-uplink",
     "dataflow-endpoint",
     "s3-recording",
     "tracking",
     "uplink-echo",
 ]
+ContactScheduledWaiterName = Literal["contact_scheduled"]
 ContactStatusType = Literal[
     "AVAILABLE",
     "AWS_CANCELLED",
     "AWS_FAILED",
     "CANCELLED",
     "CANCELLING",
     "COMPLETED",
@@ -113,14 +122,15 @@
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
@@ -130,27 +140,31 @@
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
@@ -179,14 +193,15 @@
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
@@ -234,14 +249,15 @@
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
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
@@ -252,30 +268,33 @@
     "iottwinmaker",
     "iotwireless",
     "ivs",
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
@@ -307,28 +326,32 @@
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
@@ -356,38 +379,44 @@
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
@@ -431,14 +460,15 @@
     "list_contacts",
     "list_dataflow_endpoint_groups",
     "list_ephemerides",
     "list_ground_stations",
     "list_mission_profiles",
     "list_satellites",
 ]
+WaiterName = Literal["contact_scheduled"]
 RegionName = Literal[
     "af-south-1",
     "ap-northeast-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "eu-central-1",
     "eu-north-1",
```

### Comparing `mypy-boto3-groundstation-1.26.6/mypy_boto3_groundstation/paginator.py` & `mypy-boto3-groundstation-1.26.61/mypy_boto3_groundstation/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-groundstation-1.26.6/mypy_boto3_groundstation/paginator.pyi` & `mypy-boto3-groundstation-1.26.61/mypy_boto3_groundstation/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-groundstation-1.26.6/mypy_boto3_groundstation/type_defs.py` & `mypy-boto3-groundstation-1.26.61/mypy_boto3_groundstation/type_defs.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,26 +2,29 @@
 Type annotations for groundstation service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_groundstation.type_defs import AntennaDemodDecodeDetailsTypeDef
+    from mypy_boto3_groundstation.type_defs import ComponentVersionTypeDef
 
-    data: AntennaDemodDecodeDetailsTypeDef = {...}
+    data: ComponentVersionTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
+    AgentStatusType,
     AngleUnitsType,
+    AuditResultsType,
     BandwidthUnitsType,
+    ComponentTypeType,
     ConfigCapabilityTypeType,
     ContactStatusType,
     CriticalityType,
     EndpointStatusType,
     EphemerisInvalidReasonType,
     EphemerisSourceType,
     EphemerisStatusType,
@@ -36,47 +39,54 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
+    "ComponentVersionTypeDef",
+    "AggregateStatusTypeDef",
     "AntennaDemodDecodeDetailsTypeDef",
     "DecodeConfigTypeDef",
     "DemodulationConfigTypeDef",
     "EirpTypeDef",
     "CancelContactRequestRequestTypeDef",
+    "ComponentStatusDataTypeDef",
     "S3RecordingDetailsTypeDef",
     "ResponseMetadataTypeDef",
     "ConfigListItemTypeDef",
     "DataflowEndpointConfigTypeDef",
     "S3RecordingConfigTypeDef",
     "TrackingConfigTypeDef",
     "UplinkEchoConfigTypeDef",
+    "SocketAddressTypeDef",
     "ElevationTypeDef",
-    "CreateMissionProfileRequestRequestTypeDef",
+    "KmsKeyTypeDef",
     "DataflowEndpointListItemTypeDef",
-    "SocketAddressTypeDef",
     "DeleteConfigRequestRequestTypeDef",
     "DeleteDataflowEndpointGroupRequestRequestTypeDef",
     "DeleteEphemerisRequestRequestTypeDef",
     "DeleteMissionProfileRequestRequestTypeDef",
+    "WaiterConfigTypeDef",
     "DescribeContactRequestRequestTypeDef",
     "DescribeEphemerisRequestRequestTypeDef",
+    "DiscoveryDataTypeDef",
     "SecurityDetailsTypeDef",
     "S3ObjectTypeDef",
     "EphemerisMetaDataTypeDef",
     "FrequencyBandwidthTypeDef",
     "FrequencyTypeDef",
+    "GetAgentConfigurationRequestRequestTypeDef",
     "GetConfigRequestRequestTypeDef",
     "GetDataflowEndpointGroupRequestRequestTypeDef",
     "GetMinuteUsageRequestRequestTypeDef",
     "GetMissionProfileRequestRequestTypeDef",
     "GetSatelliteRequestRequestTypeDef",
     "GroundStationDataTypeDef",
+    "IntegerRangeTypeDef",
     "PaginatorConfigTypeDef",
     "ListConfigsRequestRequestTypeDef",
     "ListContactsRequestRequestTypeDef",
     "ListDataflowEndpointGroupsRequestRequestTypeDef",
     "ListEphemeridesRequestRequestTypeDef",
     "ListGroundStationsRequestRequestTypeDef",
     "ListMissionProfilesRequestRequestTypeDef",
@@ -84,69 +94,108 @@
     "ListSatellitesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ReserveContactRequestRequestTypeDef",
     "TimeRangeTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateEphemerisRequestRequestTypeDef",
-    "UpdateMissionProfileRequestRequestTypeDef",
+    "AgentDetailsTypeDef",
+    "UpdateAgentStatusRequestRequestTypeDef",
     "ConfigIdResponseTypeDef",
     "ContactIdResponseTypeDef",
     "DataflowEndpointGroupIdResponseTypeDef",
     "EphemerisIdResponseTypeDef",
+    "GetAgentConfigurationResponseTypeDef",
     "GetMinuteUsageResponseTypeDef",
-    "GetMissionProfileResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "MissionProfileIdResponseTypeDef",
+    "RegisterAgentResponseTypeDef",
+    "UpdateAgentStatusResponseTypeDef",
     "ListConfigsResponseTypeDef",
+    "ConnectionDetailsTypeDef",
+    "DataflowEndpointTypeDef",
     "ContactDataTypeDef",
+    "CreateMissionProfileRequestRequestTypeDef",
+    "GetMissionProfileResponseTypeDef",
+    "UpdateMissionProfileRequestRequestTypeDef",
     "ListDataflowEndpointGroupsResponseTypeDef",
-    "DataflowEndpointTypeDef",
+    "DescribeContactRequestContactScheduledWaitTypeDef",
     "EphemerisDescriptionTypeDef",
     "EphemerisItemTypeDef",
     "OEMEphemerisTypeDef",
     "GetSatelliteResponseTypeDef",
     "SatelliteListItemTypeDef",
     "SpectrumConfigTypeDef",
     "UplinkSpectrumConfigTypeDef",
     "ListGroundStationsResponseTypeDef",
+    "RangedSocketAddressTypeDef",
     "ListConfigsRequestListConfigsPaginateTypeDef",
     "ListContactsRequestListContactsPaginateTypeDef",
     "ListDataflowEndpointGroupsRequestListDataflowEndpointGroupsPaginateTypeDef",
     "ListEphemeridesRequestListEphemeridesPaginateTypeDef",
     "ListGroundStationsRequestListGroundStationsPaginateTypeDef",
     "ListMissionProfilesRequestListMissionProfilesPaginateTypeDef",
     "ListSatellitesRequestListSatellitesPaginateTypeDef",
     "ListMissionProfilesResponseTypeDef",
     "TLEDataTypeDef",
+    "RegisterAgentRequestRequestTypeDef",
     "ListContactsResponseTypeDef",
-    "EndpointDetailsTypeDef",
     "EphemerisTypeDescriptionTypeDef",
     "ListEphemeridesResponseTypeDef",
     "ListSatellitesResponseTypeDef",
     "AntennaDownlinkConfigTypeDef",
     "AntennaDownlinkDemodDecodeConfigTypeDef",
     "AntennaUplinkConfigTypeDef",
+    "RangedConnectionDetailsTypeDef",
     "TLEEphemerisTypeDef",
-    "ConfigDetailsTypeDef",
-    "CreateDataflowEndpointGroupRequestRequestTypeDef",
-    "GetDataflowEndpointGroupResponseTypeDef",
     "DescribeEphemerisResponseTypeDef",
     "ConfigTypeDataTypeDef",
+    "AwsGroundStationAgentEndpointTypeDef",
     "EphemerisDataTypeDef",
-    "DestinationTypeDef",
-    "SourceTypeDef",
     "CreateConfigRequestRequestTypeDef",
     "GetConfigResponseTypeDef",
     "UpdateConfigRequestRequestTypeDef",
+    "EndpointDetailsTypeDef",
     "CreateEphemerisRequestRequestTypeDef",
+    "ConfigDetailsTypeDef",
+    "CreateDataflowEndpointGroupRequestRequestTypeDef",
+    "GetDataflowEndpointGroupResponseTypeDef",
+    "DestinationTypeDef",
+    "SourceTypeDef",
     "DataflowDetailTypeDef",
     "DescribeContactResponseTypeDef",
 )
 
+ComponentVersionTypeDef = TypedDict(
+    "ComponentVersionTypeDef",
+    {
+        "componentType": ComponentTypeType,
+        "versions": Sequence[str],
+    },
+)
+
+_RequiredAggregateStatusTypeDef = TypedDict(
+    "_RequiredAggregateStatusTypeDef",
+    {
+        "status": AgentStatusType,
+    },
+)
+_OptionalAggregateStatusTypeDef = TypedDict(
+    "_OptionalAggregateStatusTypeDef",
+    {
+        "signatureMap": Mapping[str, bool],
+    },
+    total=False,
+)
+
+
+class AggregateStatusTypeDef(_RequiredAggregateStatusTypeDef, _OptionalAggregateStatusTypeDef):
+    pass
+
+
 AntennaDemodDecodeDetailsTypeDef = TypedDict(
     "AntennaDemodDecodeDetailsTypeDef",
     {
         "outputNode": str,
     },
     total=False,
 )
@@ -176,14 +225,40 @@
 CancelContactRequestRequestTypeDef = TypedDict(
     "CancelContactRequestRequestTypeDef",
     {
         "contactId": str,
     },
 )
 
+_RequiredComponentStatusDataTypeDef = TypedDict(
+    "_RequiredComponentStatusDataTypeDef",
+    {
+        "capabilityArn": str,
+        "componentType": ComponentTypeType,
+        "dataflowId": str,
+        "status": AgentStatusType,
+    },
+)
+_OptionalComponentStatusDataTypeDef = TypedDict(
+    "_OptionalComponentStatusDataTypeDef",
+    {
+        "bytesReceived": int,
+        "bytesSent": int,
+        "packetsDropped": int,
+    },
+    total=False,
+)
+
+
+class ComponentStatusDataTypeDef(
+    _RequiredComponentStatusDataTypeDef, _OptionalComponentStatusDataTypeDef
+):
+    pass
+
+
 S3RecordingDetailsTypeDef = TypedDict(
     "S3RecordingDetailsTypeDef",
     {
         "bucketArn": str,
         "keyTemplate": str,
     },
     total=False,
@@ -265,66 +340,48 @@
     "UplinkEchoConfigTypeDef",
     {
         "antennaUplinkConfigArn": str,
         "enabled": bool,
     },
 )
 
+SocketAddressTypeDef = TypedDict(
+    "SocketAddressTypeDef",
+    {
+        "name": str,
+        "port": int,
+    },
+)
+
 ElevationTypeDef = TypedDict(
     "ElevationTypeDef",
     {
         "unit": AngleUnitsType,
         "value": float,
     },
 )
 
-_RequiredCreateMissionProfileRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateMissionProfileRequestRequestTypeDef",
+KmsKeyTypeDef = TypedDict(
+    "KmsKeyTypeDef",
     {
-        "dataflowEdges": Sequence[Sequence[str]],
-        "minimumViableContactDurationSeconds": int,
-        "name": str,
-        "trackingConfigArn": str,
-    },
-)
-_OptionalCreateMissionProfileRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateMissionProfileRequestRequestTypeDef",
-    {
-        "contactPostPassDurationSeconds": int,
-        "contactPrePassDurationSeconds": int,
-        "tags": Mapping[str, str],
+        "kmsAliasArn": str,
+        "kmsKeyArn": str,
     },
     total=False,
 )
 
-
-class CreateMissionProfileRequestRequestTypeDef(
-    _RequiredCreateMissionProfileRequestRequestTypeDef,
-    _OptionalCreateMissionProfileRequestRequestTypeDef,
-):
-    pass
-
-
 DataflowEndpointListItemTypeDef = TypedDict(
     "DataflowEndpointListItemTypeDef",
     {
         "dataflowEndpointGroupArn": str,
         "dataflowEndpointGroupId": str,
     },
     total=False,
 )
 
-SocketAddressTypeDef = TypedDict(
-    "SocketAddressTypeDef",
-    {
-        "name": str,
-        "port": int,
-    },
-)
-
 DeleteConfigRequestRequestTypeDef = TypedDict(
     "DeleteConfigRequestRequestTypeDef",
     {
         "configId": str,
         "configType": ConfigCapabilityTypeType,
     },
 )
@@ -346,28 +403,46 @@
 DeleteMissionProfileRequestRequestTypeDef = TypedDict(
     "DeleteMissionProfileRequestRequestTypeDef",
     {
         "missionProfileId": str,
     },
 )
 
+WaiterConfigTypeDef = TypedDict(
+    "WaiterConfigTypeDef",
+    {
+        "Delay": int,
+        "MaxAttempts": int,
+    },
+    total=False,
+)
+
 DescribeContactRequestRequestTypeDef = TypedDict(
     "DescribeContactRequestRequestTypeDef",
     {
         "contactId": str,
     },
 )
 
 DescribeEphemerisRequestRequestTypeDef = TypedDict(
     "DescribeEphemerisRequestRequestTypeDef",
     {
         "ephemerisId": str,
     },
 )
 
+DiscoveryDataTypeDef = TypedDict(
+    "DiscoveryDataTypeDef",
+    {
+        "capabilityArns": Sequence[str],
+        "privateIpAddresses": Sequence[str],
+        "publicIpAddresses": Sequence[str],
+    },
+)
+
 SecurityDetailsTypeDef = TypedDict(
     "SecurityDetailsTypeDef",
     {
         "roleArn": str,
         "securityGroupIds": Sequence[str],
         "subnetIds": Sequence[str],
     },
@@ -418,14 +493,21 @@
     "FrequencyTypeDef",
     {
         "units": FrequencyUnitsType,
         "value": float,
     },
 )
 
+GetAgentConfigurationRequestRequestTypeDef = TypedDict(
+    "GetAgentConfigurationRequestRequestTypeDef",
+    {
+        "agentId": str,
+    },
+)
+
 GetConfigRequestRequestTypeDef = TypedDict(
     "GetConfigRequestRequestTypeDef",
     {
         "configId": str,
         "configType": ConfigCapabilityTypeType,
     },
 )
@@ -465,14 +547,22 @@
         "groundStationId": str,
         "groundStationName": str,
         "region": str,
     },
     total=False,
 )
 
+IntegerRangeTypeDef = TypedDict(
+    "IntegerRangeTypeDef",
+    {
+        "maximum": int,
+        "minimum": int,
+    },
+)
+
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
@@ -663,41 +753,35 @@
 
 class UpdateEphemerisRequestRequestTypeDef(
     _RequiredUpdateEphemerisRequestRequestTypeDef, _OptionalUpdateEphemerisRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredUpdateMissionProfileRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateMissionProfileRequestRequestTypeDef",
+AgentDetailsTypeDef = TypedDict(
+    "AgentDetailsTypeDef",
     {
-        "missionProfileId": str,
+        "agentVersion": str,
+        "componentVersions": Sequence[ComponentVersionTypeDef],
+        "instanceId": str,
+        "instanceType": str,
+        "reservedCpuCores": Sequence[int],
     },
 )
-_OptionalUpdateMissionProfileRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateMissionProfileRequestRequestTypeDef",
+
+UpdateAgentStatusRequestRequestTypeDef = TypedDict(
+    "UpdateAgentStatusRequestRequestTypeDef",
     {
-        "contactPostPassDurationSeconds": int,
-        "contactPrePassDurationSeconds": int,
-        "dataflowEdges": Sequence[Sequence[str]],
-        "minimumViableContactDurationSeconds": int,
-        "name": str,
-        "trackingConfigArn": str,
+        "agentId": str,
+        "aggregateStatus": AggregateStatusTypeDef,
+        "componentStatuses": Sequence[ComponentStatusDataTypeDef],
+        "taskId": str,
     },
-    total=False,
 )
 
-
-class UpdateMissionProfileRequestRequestTypeDef(
-    _RequiredUpdateMissionProfileRequestRequestTypeDef,
-    _OptionalUpdateMissionProfileRequestRequestTypeDef,
-):
-    pass
-
-
 ConfigIdResponseTypeDef = TypedDict(
     "ConfigIdResponseTypeDef",
     {
         "configArn": str,
         "configId": str,
         "configType": ConfigCapabilityTypeType,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -724,43 +808,35 @@
     "EphemerisIdResponseTypeDef",
     {
         "ephemerisId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+GetAgentConfigurationResponseTypeDef = TypedDict(
+    "GetAgentConfigurationResponseTypeDef",
+    {
+        "agentId": str,
+        "taskingDocument": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 GetMinuteUsageResponseTypeDef = TypedDict(
     "GetMinuteUsageResponseTypeDef",
     {
         "estimatedMinutesRemaining": int,
         "isReservedMinutesCustomer": bool,
         "totalReservedMinuteAllocation": int,
         "totalScheduledMinutes": int,
         "upcomingMinutesScheduled": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetMissionProfileResponseTypeDef = TypedDict(
-    "GetMissionProfileResponseTypeDef",
-    {
-        "contactPostPassDurationSeconds": int,
-        "contactPrePassDurationSeconds": int,
-        "dataflowEdges": List[List[str]],
-        "minimumViableContactDurationSeconds": int,
-        "missionProfileArn": str,
-        "missionProfileId": str,
-        "name": str,
-        "region": str,
-        "tags": Dict[str, str],
-        "trackingConfigArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -769,23 +845,71 @@
     "MissionProfileIdResponseTypeDef",
     {
         "missionProfileId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+RegisterAgentResponseTypeDef = TypedDict(
+    "RegisterAgentResponseTypeDef",
+    {
+        "agentId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateAgentStatusResponseTypeDef = TypedDict(
+    "UpdateAgentStatusResponseTypeDef",
+    {
+        "agentId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListConfigsResponseTypeDef = TypedDict(
     "ListConfigsResponseTypeDef",
     {
         "configList": List[ConfigListItemTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredConnectionDetailsTypeDef = TypedDict(
+    "_RequiredConnectionDetailsTypeDef",
+    {
+        "socketAddress": SocketAddressTypeDef,
+    },
+)
+_OptionalConnectionDetailsTypeDef = TypedDict(
+    "_OptionalConnectionDetailsTypeDef",
+    {
+        "mtu": int,
+    },
+    total=False,
+)
+
+
+class ConnectionDetailsTypeDef(
+    _RequiredConnectionDetailsTypeDef, _OptionalConnectionDetailsTypeDef
+):
+    pass
+
+
+DataflowEndpointTypeDef = TypedDict(
+    "DataflowEndpointTypeDef",
+    {
+        "address": SocketAddressTypeDef,
+        "mtu": int,
+        "name": str,
+        "status": EndpointStatusType,
+    },
+    total=False,
+)
+
 ContactDataTypeDef = TypedDict(
     "ContactDataTypeDef",
     {
         "contactId": str,
         "contactStatus": ContactStatusType,
         "endTime": datetime,
         "errorMessage": str,
@@ -798,34 +922,122 @@
         "satelliteArn": str,
         "startTime": datetime,
         "tags": Dict[str, str],
     },
     total=False,
 )
 
+_RequiredCreateMissionProfileRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateMissionProfileRequestRequestTypeDef",
+    {
+        "dataflowEdges": Sequence[Sequence[str]],
+        "minimumViableContactDurationSeconds": int,
+        "name": str,
+        "trackingConfigArn": str,
+    },
+)
+_OptionalCreateMissionProfileRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateMissionProfileRequestRequestTypeDef",
+    {
+        "contactPostPassDurationSeconds": int,
+        "contactPrePassDurationSeconds": int,
+        "streamsKmsKey": KmsKeyTypeDef,
+        "streamsKmsRole": str,
+        "tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+
+class CreateMissionProfileRequestRequestTypeDef(
+    _RequiredCreateMissionProfileRequestRequestTypeDef,
+    _OptionalCreateMissionProfileRequestRequestTypeDef,
+):
+    pass
+
+
+GetMissionProfileResponseTypeDef = TypedDict(
+    "GetMissionProfileResponseTypeDef",
+    {
+        "contactPostPassDurationSeconds": int,
+        "contactPrePassDurationSeconds": int,
+        "dataflowEdges": List[List[str]],
+        "minimumViableContactDurationSeconds": int,
+        "missionProfileArn": str,
+        "missionProfileId": str,
+        "name": str,
+        "region": str,
+        "streamsKmsKey": KmsKeyTypeDef,
+        "streamsKmsRole": str,
+        "tags": Dict[str, str],
+        "trackingConfigArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredUpdateMissionProfileRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateMissionProfileRequestRequestTypeDef",
+    {
+        "missionProfileId": str,
+    },
+)
+_OptionalUpdateMissionProfileRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateMissionProfileRequestRequestTypeDef",
+    {
+        "contactPostPassDurationSeconds": int,
+        "contactPrePassDurationSeconds": int,
+        "dataflowEdges": Sequence[Sequence[str]],
+        "minimumViableContactDurationSeconds": int,
+        "name": str,
+        "streamsKmsKey": KmsKeyTypeDef,
+        "streamsKmsRole": str,
+        "trackingConfigArn": str,
+    },
+    total=False,
+)
+
+
+class UpdateMissionProfileRequestRequestTypeDef(
+    _RequiredUpdateMissionProfileRequestRequestTypeDef,
+    _OptionalUpdateMissionProfileRequestRequestTypeDef,
+):
+    pass
+
+
 ListDataflowEndpointGroupsResponseTypeDef = TypedDict(
     "ListDataflowEndpointGroupsResponseTypeDef",
     {
         "dataflowEndpointGroupList": List[DataflowEndpointListItemTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DataflowEndpointTypeDef = TypedDict(
-    "DataflowEndpointTypeDef",
+_RequiredDescribeContactRequestContactScheduledWaitTypeDef = TypedDict(
+    "_RequiredDescribeContactRequestContactScheduledWaitTypeDef",
     {
-        "address": SocketAddressTypeDef,
-        "mtu": int,
-        "name": str,
-        "status": EndpointStatusType,
+        "contactId": str,
+    },
+)
+_OptionalDescribeContactRequestContactScheduledWaitTypeDef = TypedDict(
+    "_OptionalDescribeContactRequestContactScheduledWaitTypeDef",
+    {
+        "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
+class DescribeContactRequestContactScheduledWaitTypeDef(
+    _RequiredDescribeContactRequestContactScheduledWaitTypeDef,
+    _OptionalDescribeContactRequestContactScheduledWaitTypeDef,
+):
+    pass
+
+
 EphemerisDescriptionTypeDef = TypedDict(
     "EphemerisDescriptionTypeDef",
     {
         "ephemerisData": str,
         "sourceS3Object": S3ObjectTypeDef,
     },
     total=False,
@@ -924,14 +1136,22 @@
     {
         "groundStationList": List[GroundStationDataTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+RangedSocketAddressTypeDef = TypedDict(
+    "RangedSocketAddressTypeDef",
+    {
+        "name": str,
+        "portRange": IntegerRangeTypeDef,
+    },
+)
+
 ListConfigsRequestListConfigsPaginateTypeDef = TypedDict(
     "ListConfigsRequestListConfigsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -1035,32 +1255,31 @@
     {
         "tleLine1": str,
         "tleLine2": str,
         "validTimeRange": TimeRangeTypeDef,
     },
 )
 
+RegisterAgentRequestRequestTypeDef = TypedDict(
+    "RegisterAgentRequestRequestTypeDef",
+    {
+        "agentDetails": AgentDetailsTypeDef,
+        "discoveryData": DiscoveryDataTypeDef,
+    },
+)
+
 ListContactsResponseTypeDef = TypedDict(
     "ListContactsResponseTypeDef",
     {
         "contactList": List[ContactDataTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-EndpointDetailsTypeDef = TypedDict(
-    "EndpointDetailsTypeDef",
-    {
-        "endpoint": DataflowEndpointTypeDef,
-        "securityDetails": SecurityDetailsTypeDef,
-    },
-    total=False,
-)
-
 EphemerisTypeDescriptionTypeDef = TypedDict(
     "EphemerisTypeDescriptionTypeDef",
     {
         "oem": EphemerisDescriptionTypeDef,
         "tle": EphemerisDescriptionTypeDef,
     },
     total=False,
@@ -1118,64 +1337,42 @@
 
 class AntennaUplinkConfigTypeDef(
     _RequiredAntennaUplinkConfigTypeDef, _OptionalAntennaUplinkConfigTypeDef
 ):
     pass
 
 
-TLEEphemerisTypeDef = TypedDict(
-    "TLEEphemerisTypeDef",
-    {
-        "s3Object": S3ObjectTypeDef,
-        "tleData": Sequence[TLEDataTypeDef],
-    },
-    total=False,
-)
-
-ConfigDetailsTypeDef = TypedDict(
-    "ConfigDetailsTypeDef",
-    {
-        "antennaDemodDecodeDetails": AntennaDemodDecodeDetailsTypeDef,
-        "endpointDetails": EndpointDetailsTypeDef,
-        "s3RecordingDetails": S3RecordingDetailsTypeDef,
-    },
-    total=False,
-)
-
-_RequiredCreateDataflowEndpointGroupRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateDataflowEndpointGroupRequestRequestTypeDef",
+_RequiredRangedConnectionDetailsTypeDef = TypedDict(
+    "_RequiredRangedConnectionDetailsTypeDef",
     {
-        "endpointDetails": Sequence[EndpointDetailsTypeDef],
+        "socketAddress": RangedSocketAddressTypeDef,
     },
 )
-_OptionalCreateDataflowEndpointGroupRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateDataflowEndpointGroupRequestRequestTypeDef",
+_OptionalRangedConnectionDetailsTypeDef = TypedDict(
+    "_OptionalRangedConnectionDetailsTypeDef",
     {
-        "tags": Mapping[str, str],
+        "mtu": int,
     },
     total=False,
 )
 
 
-class CreateDataflowEndpointGroupRequestRequestTypeDef(
-    _RequiredCreateDataflowEndpointGroupRequestRequestTypeDef,
-    _OptionalCreateDataflowEndpointGroupRequestRequestTypeDef,
+class RangedConnectionDetailsTypeDef(
+    _RequiredRangedConnectionDetailsTypeDef, _OptionalRangedConnectionDetailsTypeDef
 ):
     pass
 
 
-GetDataflowEndpointGroupResponseTypeDef = TypedDict(
-    "GetDataflowEndpointGroupResponseTypeDef",
+TLEEphemerisTypeDef = TypedDict(
+    "TLEEphemerisTypeDef",
     {
-        "dataflowEndpointGroupArn": str,
-        "dataflowEndpointGroupId": str,
-        "endpointsDetails": List[EndpointDetailsTypeDef],
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "s3Object": S3ObjectTypeDef,
+        "tleData": Sequence[TLEDataTypeDef],
     },
+    total=False,
 )
 
 DescribeEphemerisResponseTypeDef = TypedDict(
     "DescribeEphemerisResponseTypeDef",
     {
         "creationTime": datetime,
         "enabled": bool,
@@ -1201,41 +1398,43 @@
         "s3RecordingConfig": S3RecordingConfigTypeDef,
         "trackingConfig": TrackingConfigTypeDef,
         "uplinkEchoConfig": UplinkEchoConfigTypeDef,
     },
     total=False,
 )
 
-EphemerisDataTypeDef = TypedDict(
-    "EphemerisDataTypeDef",
+_RequiredAwsGroundStationAgentEndpointTypeDef = TypedDict(
+    "_RequiredAwsGroundStationAgentEndpointTypeDef",
     {
-        "oem": OEMEphemerisTypeDef,
-        "tle": TLEEphemerisTypeDef,
+        "egressAddress": ConnectionDetailsTypeDef,
+        "ingressAddress": RangedConnectionDetailsTypeDef,
+        "name": str,
     },
-    total=False,
 )
-
-DestinationTypeDef = TypedDict(
-    "DestinationTypeDef",
+_OptionalAwsGroundStationAgentEndpointTypeDef = TypedDict(
+    "_OptionalAwsGroundStationAgentEndpointTypeDef",
     {
-        "configDetails": ConfigDetailsTypeDef,
-        "configId": str,
-        "configType": ConfigCapabilityTypeType,
-        "dataflowDestinationRegion": str,
+        "agentStatus": AgentStatusType,
+        "auditResults": AuditResultsType,
     },
     total=False,
 )
 
-SourceTypeDef = TypedDict(
-    "SourceTypeDef",
+
+class AwsGroundStationAgentEndpointTypeDef(
+    _RequiredAwsGroundStationAgentEndpointTypeDef, _OptionalAwsGroundStationAgentEndpointTypeDef
+):
+    pass
+
+
+EphemerisDataTypeDef = TypedDict(
+    "EphemerisDataTypeDef",
     {
-        "configDetails": ConfigDetailsTypeDef,
-        "configId": str,
-        "configType": ConfigCapabilityTypeType,
-        "dataflowSourceRegion": str,
+        "oem": OEMEphemerisTypeDef,
+        "tle": TLEEphemerisTypeDef,
     },
     total=False,
 )
 
 _RequiredCreateConfigRequestRequestTypeDef = TypedDict(
     "_RequiredCreateConfigRequestRequestTypeDef",
     {
@@ -1277,14 +1476,24 @@
         "configData": ConfigTypeDataTypeDef,
         "configId": str,
         "configType": ConfigCapabilityTypeType,
         "name": str,
     },
 )
 
+EndpointDetailsTypeDef = TypedDict(
+    "EndpointDetailsTypeDef",
+    {
+        "awsGroundStationAgentEndpoint": AwsGroundStationAgentEndpointTypeDef,
+        "endpoint": DataflowEndpointTypeDef,
+        "securityDetails": SecurityDetailsTypeDef,
+    },
+    total=False,
+)
+
 _RequiredCreateEphemerisRequestRequestTypeDef = TypedDict(
     "_RequiredCreateEphemerisRequestRequestTypeDef",
     {
         "name": str,
         "satelliteId": str,
     },
 )
@@ -1304,14 +1513,83 @@
 
 class CreateEphemerisRequestRequestTypeDef(
     _RequiredCreateEphemerisRequestRequestTypeDef, _OptionalCreateEphemerisRequestRequestTypeDef
 ):
     pass
 
 
+ConfigDetailsTypeDef = TypedDict(
+    "ConfigDetailsTypeDef",
+    {
+        "antennaDemodDecodeDetails": AntennaDemodDecodeDetailsTypeDef,
+        "endpointDetails": EndpointDetailsTypeDef,
+        "s3RecordingDetails": S3RecordingDetailsTypeDef,
+    },
+    total=False,
+)
+
+_RequiredCreateDataflowEndpointGroupRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateDataflowEndpointGroupRequestRequestTypeDef",
+    {
+        "endpointDetails": Sequence[EndpointDetailsTypeDef],
+    },
+)
+_OptionalCreateDataflowEndpointGroupRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateDataflowEndpointGroupRequestRequestTypeDef",
+    {
+        "contactPostPassDurationSeconds": int,
+        "contactPrePassDurationSeconds": int,
+        "tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+
+class CreateDataflowEndpointGroupRequestRequestTypeDef(
+    _RequiredCreateDataflowEndpointGroupRequestRequestTypeDef,
+    _OptionalCreateDataflowEndpointGroupRequestRequestTypeDef,
+):
+    pass
+
+
+GetDataflowEndpointGroupResponseTypeDef = TypedDict(
+    "GetDataflowEndpointGroupResponseTypeDef",
+    {
+        "contactPostPassDurationSeconds": int,
+        "contactPrePassDurationSeconds": int,
+        "dataflowEndpointGroupArn": str,
+        "dataflowEndpointGroupId": str,
+        "endpointsDetails": List[EndpointDetailsTypeDef],
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DestinationTypeDef = TypedDict(
+    "DestinationTypeDef",
+    {
+        "configDetails": ConfigDetailsTypeDef,
+        "configId": str,
+        "configType": ConfigCapabilityTypeType,
+        "dataflowDestinationRegion": str,
+    },
+    total=False,
+)
+
+SourceTypeDef = TypedDict(
+    "SourceTypeDef",
+    {
+        "configDetails": ConfigDetailsTypeDef,
+        "configId": str,
+        "configType": ConfigCapabilityTypeType,
+        "dataflowSourceRegion": str,
+    },
+    total=False,
+)
+
 DataflowDetailTypeDef = TypedDict(
     "DataflowDetailTypeDef",
     {
         "destination": DestinationTypeDef,
         "errorMessage": str,
         "source": SourceTypeDef,
     },
```

### Comparing `mypy-boto3-groundstation-1.26.6/mypy_boto3_groundstation/type_defs.pyi` & `mypy-boto3-groundstation-1.26.61/mypy_boto3_groundstation/type_defs.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -2,26 +2,29 @@
 Type annotations for groundstation service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_groundstation.type_defs import AntennaDemodDecodeDetailsTypeDef
+    from mypy_boto3_groundstation.type_defs import ComponentVersionTypeDef
 
-    data: AntennaDemodDecodeDetailsTypeDef = {...}
+    data: ComponentVersionTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
+    AgentStatusType,
     AngleUnitsType,
+    AuditResultsType,
     BandwidthUnitsType,
+    ComponentTypeType,
     ConfigCapabilityTypeType,
     ContactStatusType,
     CriticalityType,
     EndpointStatusType,
     EphemerisInvalidReasonType,
     EphemerisSourceType,
     EphemerisStatusType,
@@ -35,47 +38,54 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
+    "ComponentVersionTypeDef",
+    "AggregateStatusTypeDef",
     "AntennaDemodDecodeDetailsTypeDef",
     "DecodeConfigTypeDef",
     "DemodulationConfigTypeDef",
     "EirpTypeDef",
     "CancelContactRequestRequestTypeDef",
+    "ComponentStatusDataTypeDef",
     "S3RecordingDetailsTypeDef",
     "ResponseMetadataTypeDef",
     "ConfigListItemTypeDef",
     "DataflowEndpointConfigTypeDef",
     "S3RecordingConfigTypeDef",
     "TrackingConfigTypeDef",
     "UplinkEchoConfigTypeDef",
+    "SocketAddressTypeDef",
     "ElevationTypeDef",
-    "CreateMissionProfileRequestRequestTypeDef",
+    "KmsKeyTypeDef",
     "DataflowEndpointListItemTypeDef",
-    "SocketAddressTypeDef",
     "DeleteConfigRequestRequestTypeDef",
     "DeleteDataflowEndpointGroupRequestRequestTypeDef",
     "DeleteEphemerisRequestRequestTypeDef",
     "DeleteMissionProfileRequestRequestTypeDef",
+    "WaiterConfigTypeDef",
     "DescribeContactRequestRequestTypeDef",
     "DescribeEphemerisRequestRequestTypeDef",
+    "DiscoveryDataTypeDef",
     "SecurityDetailsTypeDef",
     "S3ObjectTypeDef",
     "EphemerisMetaDataTypeDef",
     "FrequencyBandwidthTypeDef",
     "FrequencyTypeDef",
+    "GetAgentConfigurationRequestRequestTypeDef",
     "GetConfigRequestRequestTypeDef",
     "GetDataflowEndpointGroupRequestRequestTypeDef",
     "GetMinuteUsageRequestRequestTypeDef",
     "GetMissionProfileRequestRequestTypeDef",
     "GetSatelliteRequestRequestTypeDef",
     "GroundStationDataTypeDef",
+    "IntegerRangeTypeDef",
     "PaginatorConfigTypeDef",
     "ListConfigsRequestRequestTypeDef",
     "ListContactsRequestRequestTypeDef",
     "ListDataflowEndpointGroupsRequestRequestTypeDef",
     "ListEphemeridesRequestRequestTypeDef",
     "ListGroundStationsRequestRequestTypeDef",
     "ListMissionProfilesRequestRequestTypeDef",
@@ -83,69 +93,106 @@
     "ListSatellitesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ReserveContactRequestRequestTypeDef",
     "TimeRangeTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateEphemerisRequestRequestTypeDef",
-    "UpdateMissionProfileRequestRequestTypeDef",
+    "AgentDetailsTypeDef",
+    "UpdateAgentStatusRequestRequestTypeDef",
     "ConfigIdResponseTypeDef",
     "ContactIdResponseTypeDef",
     "DataflowEndpointGroupIdResponseTypeDef",
     "EphemerisIdResponseTypeDef",
+    "GetAgentConfigurationResponseTypeDef",
     "GetMinuteUsageResponseTypeDef",
-    "GetMissionProfileResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "MissionProfileIdResponseTypeDef",
+    "RegisterAgentResponseTypeDef",
+    "UpdateAgentStatusResponseTypeDef",
     "ListConfigsResponseTypeDef",
+    "ConnectionDetailsTypeDef",
+    "DataflowEndpointTypeDef",
     "ContactDataTypeDef",
+    "CreateMissionProfileRequestRequestTypeDef",
+    "GetMissionProfileResponseTypeDef",
+    "UpdateMissionProfileRequestRequestTypeDef",
     "ListDataflowEndpointGroupsResponseTypeDef",
-    "DataflowEndpointTypeDef",
+    "DescribeContactRequestContactScheduledWaitTypeDef",
     "EphemerisDescriptionTypeDef",
     "EphemerisItemTypeDef",
     "OEMEphemerisTypeDef",
     "GetSatelliteResponseTypeDef",
     "SatelliteListItemTypeDef",
     "SpectrumConfigTypeDef",
     "UplinkSpectrumConfigTypeDef",
     "ListGroundStationsResponseTypeDef",
+    "RangedSocketAddressTypeDef",
     "ListConfigsRequestListConfigsPaginateTypeDef",
     "ListContactsRequestListContactsPaginateTypeDef",
     "ListDataflowEndpointGroupsRequestListDataflowEndpointGroupsPaginateTypeDef",
     "ListEphemeridesRequestListEphemeridesPaginateTypeDef",
     "ListGroundStationsRequestListGroundStationsPaginateTypeDef",
     "ListMissionProfilesRequestListMissionProfilesPaginateTypeDef",
     "ListSatellitesRequestListSatellitesPaginateTypeDef",
     "ListMissionProfilesResponseTypeDef",
     "TLEDataTypeDef",
+    "RegisterAgentRequestRequestTypeDef",
     "ListContactsResponseTypeDef",
-    "EndpointDetailsTypeDef",
     "EphemerisTypeDescriptionTypeDef",
     "ListEphemeridesResponseTypeDef",
     "ListSatellitesResponseTypeDef",
     "AntennaDownlinkConfigTypeDef",
     "AntennaDownlinkDemodDecodeConfigTypeDef",
     "AntennaUplinkConfigTypeDef",
+    "RangedConnectionDetailsTypeDef",
     "TLEEphemerisTypeDef",
-    "ConfigDetailsTypeDef",
-    "CreateDataflowEndpointGroupRequestRequestTypeDef",
-    "GetDataflowEndpointGroupResponseTypeDef",
     "DescribeEphemerisResponseTypeDef",
     "ConfigTypeDataTypeDef",
+    "AwsGroundStationAgentEndpointTypeDef",
     "EphemerisDataTypeDef",
-    "DestinationTypeDef",
-    "SourceTypeDef",
     "CreateConfigRequestRequestTypeDef",
     "GetConfigResponseTypeDef",
     "UpdateConfigRequestRequestTypeDef",
+    "EndpointDetailsTypeDef",
     "CreateEphemerisRequestRequestTypeDef",
+    "ConfigDetailsTypeDef",
+    "CreateDataflowEndpointGroupRequestRequestTypeDef",
+    "GetDataflowEndpointGroupResponseTypeDef",
+    "DestinationTypeDef",
+    "SourceTypeDef",
     "DataflowDetailTypeDef",
     "DescribeContactResponseTypeDef",
 )
 
+ComponentVersionTypeDef = TypedDict(
+    "ComponentVersionTypeDef",
+    {
+        "componentType": ComponentTypeType,
+        "versions": Sequence[str],
+    },
+)
+
+_RequiredAggregateStatusTypeDef = TypedDict(
+    "_RequiredAggregateStatusTypeDef",
+    {
+        "status": AgentStatusType,
+    },
+)
+_OptionalAggregateStatusTypeDef = TypedDict(
+    "_OptionalAggregateStatusTypeDef",
+    {
+        "signatureMap": Mapping[str, bool],
+    },
+    total=False,
+)
+
+class AggregateStatusTypeDef(_RequiredAggregateStatusTypeDef, _OptionalAggregateStatusTypeDef):
+    pass
+
 AntennaDemodDecodeDetailsTypeDef = TypedDict(
     "AntennaDemodDecodeDetailsTypeDef",
     {
         "outputNode": str,
     },
     total=False,
 )
@@ -175,14 +222,38 @@
 CancelContactRequestRequestTypeDef = TypedDict(
     "CancelContactRequestRequestTypeDef",
     {
         "contactId": str,
     },
 )
 
+_RequiredComponentStatusDataTypeDef = TypedDict(
+    "_RequiredComponentStatusDataTypeDef",
+    {
+        "capabilityArn": str,
+        "componentType": ComponentTypeType,
+        "dataflowId": str,
+        "status": AgentStatusType,
+    },
+)
+_OptionalComponentStatusDataTypeDef = TypedDict(
+    "_OptionalComponentStatusDataTypeDef",
+    {
+        "bytesReceived": int,
+        "bytesSent": int,
+        "packetsDropped": int,
+    },
+    total=False,
+)
+
+class ComponentStatusDataTypeDef(
+    _RequiredComponentStatusDataTypeDef, _OptionalComponentStatusDataTypeDef
+):
+    pass
+
 S3RecordingDetailsTypeDef = TypedDict(
     "S3RecordingDetailsTypeDef",
     {
         "bucketArn": str,
         "keyTemplate": str,
     },
     total=False,
@@ -260,64 +331,48 @@
     "UplinkEchoConfigTypeDef",
     {
         "antennaUplinkConfigArn": str,
         "enabled": bool,
     },
 )
 
+SocketAddressTypeDef = TypedDict(
+    "SocketAddressTypeDef",
+    {
+        "name": str,
+        "port": int,
+    },
+)
+
 ElevationTypeDef = TypedDict(
     "ElevationTypeDef",
     {
         "unit": AngleUnitsType,
         "value": float,
     },
 )
 
-_RequiredCreateMissionProfileRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateMissionProfileRequestRequestTypeDef",
-    {
-        "dataflowEdges": Sequence[Sequence[str]],
-        "minimumViableContactDurationSeconds": int,
-        "name": str,
-        "trackingConfigArn": str,
-    },
-)
-_OptionalCreateMissionProfileRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateMissionProfileRequestRequestTypeDef",
+KmsKeyTypeDef = TypedDict(
+    "KmsKeyTypeDef",
     {
-        "contactPostPassDurationSeconds": int,
-        "contactPrePassDurationSeconds": int,
-        "tags": Mapping[str, str],
+        "kmsAliasArn": str,
+        "kmsKeyArn": str,
     },
     total=False,
 )
 
-class CreateMissionProfileRequestRequestTypeDef(
-    _RequiredCreateMissionProfileRequestRequestTypeDef,
-    _OptionalCreateMissionProfileRequestRequestTypeDef,
-):
-    pass
-
 DataflowEndpointListItemTypeDef = TypedDict(
     "DataflowEndpointListItemTypeDef",
     {
         "dataflowEndpointGroupArn": str,
         "dataflowEndpointGroupId": str,
     },
     total=False,
 )
 
-SocketAddressTypeDef = TypedDict(
-    "SocketAddressTypeDef",
-    {
-        "name": str,
-        "port": int,
-    },
-)
-
 DeleteConfigRequestRequestTypeDef = TypedDict(
     "DeleteConfigRequestRequestTypeDef",
     {
         "configId": str,
         "configType": ConfigCapabilityTypeType,
     },
 )
@@ -339,28 +394,46 @@
 DeleteMissionProfileRequestRequestTypeDef = TypedDict(
     "DeleteMissionProfileRequestRequestTypeDef",
     {
         "missionProfileId": str,
     },
 )
 
+WaiterConfigTypeDef = TypedDict(
+    "WaiterConfigTypeDef",
+    {
+        "Delay": int,
+        "MaxAttempts": int,
+    },
+    total=False,
+)
+
 DescribeContactRequestRequestTypeDef = TypedDict(
     "DescribeContactRequestRequestTypeDef",
     {
         "contactId": str,
     },
 )
 
 DescribeEphemerisRequestRequestTypeDef = TypedDict(
     "DescribeEphemerisRequestRequestTypeDef",
     {
         "ephemerisId": str,
     },
 )
 
+DiscoveryDataTypeDef = TypedDict(
+    "DiscoveryDataTypeDef",
+    {
+        "capabilityArns": Sequence[str],
+        "privateIpAddresses": Sequence[str],
+        "publicIpAddresses": Sequence[str],
+    },
+)
+
 SecurityDetailsTypeDef = TypedDict(
     "SecurityDetailsTypeDef",
     {
         "roleArn": str,
         "securityGroupIds": Sequence[str],
         "subnetIds": Sequence[str],
     },
@@ -409,14 +482,21 @@
     "FrequencyTypeDef",
     {
         "units": FrequencyUnitsType,
         "value": float,
     },
 )
 
+GetAgentConfigurationRequestRequestTypeDef = TypedDict(
+    "GetAgentConfigurationRequestRequestTypeDef",
+    {
+        "agentId": str,
+    },
+)
+
 GetConfigRequestRequestTypeDef = TypedDict(
     "GetConfigRequestRequestTypeDef",
     {
         "configId": str,
         "configType": ConfigCapabilityTypeType,
     },
 )
@@ -456,14 +536,22 @@
         "groundStationId": str,
         "groundStationName": str,
         "region": str,
     },
     total=False,
 )
 
+IntegerRangeTypeDef = TypedDict(
+    "IntegerRangeTypeDef",
+    {
+        "maximum": int,
+        "minimum": int,
+    },
+)
+
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
@@ -646,39 +734,35 @@
 )
 
 class UpdateEphemerisRequestRequestTypeDef(
     _RequiredUpdateEphemerisRequestRequestTypeDef, _OptionalUpdateEphemerisRequestRequestTypeDef
 ):
     pass
 
-_RequiredUpdateMissionProfileRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateMissionProfileRequestRequestTypeDef",
+AgentDetailsTypeDef = TypedDict(
+    "AgentDetailsTypeDef",
     {
-        "missionProfileId": str,
+        "agentVersion": str,
+        "componentVersions": Sequence[ComponentVersionTypeDef],
+        "instanceId": str,
+        "instanceType": str,
+        "reservedCpuCores": Sequence[int],
     },
 )
-_OptionalUpdateMissionProfileRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateMissionProfileRequestRequestTypeDef",
+
+UpdateAgentStatusRequestRequestTypeDef = TypedDict(
+    "UpdateAgentStatusRequestRequestTypeDef",
     {
-        "contactPostPassDurationSeconds": int,
-        "contactPrePassDurationSeconds": int,
-        "dataflowEdges": Sequence[Sequence[str]],
-        "minimumViableContactDurationSeconds": int,
-        "name": str,
-        "trackingConfigArn": str,
+        "agentId": str,
+        "aggregateStatus": AggregateStatusTypeDef,
+        "componentStatuses": Sequence[ComponentStatusDataTypeDef],
+        "taskId": str,
     },
-    total=False,
 )
 
-class UpdateMissionProfileRequestRequestTypeDef(
-    _RequiredUpdateMissionProfileRequestRequestTypeDef,
-    _OptionalUpdateMissionProfileRequestRequestTypeDef,
-):
-    pass
-
 ConfigIdResponseTypeDef = TypedDict(
     "ConfigIdResponseTypeDef",
     {
         "configArn": str,
         "configId": str,
         "configType": ConfigCapabilityTypeType,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -705,43 +789,35 @@
     "EphemerisIdResponseTypeDef",
     {
         "ephemerisId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+GetAgentConfigurationResponseTypeDef = TypedDict(
+    "GetAgentConfigurationResponseTypeDef",
+    {
+        "agentId": str,
+        "taskingDocument": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 GetMinuteUsageResponseTypeDef = TypedDict(
     "GetMinuteUsageResponseTypeDef",
     {
         "estimatedMinutesRemaining": int,
         "isReservedMinutesCustomer": bool,
         "totalReservedMinuteAllocation": int,
         "totalScheduledMinutes": int,
         "upcomingMinutesScheduled": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetMissionProfileResponseTypeDef = TypedDict(
-    "GetMissionProfileResponseTypeDef",
-    {
-        "contactPostPassDurationSeconds": int,
-        "contactPrePassDurationSeconds": int,
-        "dataflowEdges": List[List[str]],
-        "minimumViableContactDurationSeconds": int,
-        "missionProfileArn": str,
-        "missionProfileId": str,
-        "name": str,
-        "region": str,
-        "tags": Dict[str, str],
-        "trackingConfigArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -750,23 +826,69 @@
     "MissionProfileIdResponseTypeDef",
     {
         "missionProfileId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+RegisterAgentResponseTypeDef = TypedDict(
+    "RegisterAgentResponseTypeDef",
+    {
+        "agentId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateAgentStatusResponseTypeDef = TypedDict(
+    "UpdateAgentStatusResponseTypeDef",
+    {
+        "agentId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListConfigsResponseTypeDef = TypedDict(
     "ListConfigsResponseTypeDef",
     {
         "configList": List[ConfigListItemTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredConnectionDetailsTypeDef = TypedDict(
+    "_RequiredConnectionDetailsTypeDef",
+    {
+        "socketAddress": SocketAddressTypeDef,
+    },
+)
+_OptionalConnectionDetailsTypeDef = TypedDict(
+    "_OptionalConnectionDetailsTypeDef",
+    {
+        "mtu": int,
+    },
+    total=False,
+)
+
+class ConnectionDetailsTypeDef(
+    _RequiredConnectionDetailsTypeDef, _OptionalConnectionDetailsTypeDef
+):
+    pass
+
+DataflowEndpointTypeDef = TypedDict(
+    "DataflowEndpointTypeDef",
+    {
+        "address": SocketAddressTypeDef,
+        "mtu": int,
+        "name": str,
+        "status": EndpointStatusType,
+    },
+    total=False,
+)
+
 ContactDataTypeDef = TypedDict(
     "ContactDataTypeDef",
     {
         "contactId": str,
         "contactStatus": ContactStatusType,
         "endTime": datetime,
         "errorMessage": str,
@@ -779,34 +901,116 @@
         "satelliteArn": str,
         "startTime": datetime,
         "tags": Dict[str, str],
     },
     total=False,
 )
 
+_RequiredCreateMissionProfileRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateMissionProfileRequestRequestTypeDef",
+    {
+        "dataflowEdges": Sequence[Sequence[str]],
+        "minimumViableContactDurationSeconds": int,
+        "name": str,
+        "trackingConfigArn": str,
+    },
+)
+_OptionalCreateMissionProfileRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateMissionProfileRequestRequestTypeDef",
+    {
+        "contactPostPassDurationSeconds": int,
+        "contactPrePassDurationSeconds": int,
+        "streamsKmsKey": KmsKeyTypeDef,
+        "streamsKmsRole": str,
+        "tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+class CreateMissionProfileRequestRequestTypeDef(
+    _RequiredCreateMissionProfileRequestRequestTypeDef,
+    _OptionalCreateMissionProfileRequestRequestTypeDef,
+):
+    pass
+
+GetMissionProfileResponseTypeDef = TypedDict(
+    "GetMissionProfileResponseTypeDef",
+    {
+        "contactPostPassDurationSeconds": int,
+        "contactPrePassDurationSeconds": int,
+        "dataflowEdges": List[List[str]],
+        "minimumViableContactDurationSeconds": int,
+        "missionProfileArn": str,
+        "missionProfileId": str,
+        "name": str,
+        "region": str,
+        "streamsKmsKey": KmsKeyTypeDef,
+        "streamsKmsRole": str,
+        "tags": Dict[str, str],
+        "trackingConfigArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredUpdateMissionProfileRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateMissionProfileRequestRequestTypeDef",
+    {
+        "missionProfileId": str,
+    },
+)
+_OptionalUpdateMissionProfileRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateMissionProfileRequestRequestTypeDef",
+    {
+        "contactPostPassDurationSeconds": int,
+        "contactPrePassDurationSeconds": int,
+        "dataflowEdges": Sequence[Sequence[str]],
+        "minimumViableContactDurationSeconds": int,
+        "name": str,
+        "streamsKmsKey": KmsKeyTypeDef,
+        "streamsKmsRole": str,
+        "trackingConfigArn": str,
+    },
+    total=False,
+)
+
+class UpdateMissionProfileRequestRequestTypeDef(
+    _RequiredUpdateMissionProfileRequestRequestTypeDef,
+    _OptionalUpdateMissionProfileRequestRequestTypeDef,
+):
+    pass
+
 ListDataflowEndpointGroupsResponseTypeDef = TypedDict(
     "ListDataflowEndpointGroupsResponseTypeDef",
     {
         "dataflowEndpointGroupList": List[DataflowEndpointListItemTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DataflowEndpointTypeDef = TypedDict(
-    "DataflowEndpointTypeDef",
+_RequiredDescribeContactRequestContactScheduledWaitTypeDef = TypedDict(
+    "_RequiredDescribeContactRequestContactScheduledWaitTypeDef",
     {
-        "address": SocketAddressTypeDef,
-        "mtu": int,
-        "name": str,
-        "status": EndpointStatusType,
+        "contactId": str,
+    },
+)
+_OptionalDescribeContactRequestContactScheduledWaitTypeDef = TypedDict(
+    "_OptionalDescribeContactRequestContactScheduledWaitTypeDef",
+    {
+        "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+class DescribeContactRequestContactScheduledWaitTypeDef(
+    _RequiredDescribeContactRequestContactScheduledWaitTypeDef,
+    _OptionalDescribeContactRequestContactScheduledWaitTypeDef,
+):
+    pass
+
 EphemerisDescriptionTypeDef = TypedDict(
     "EphemerisDescriptionTypeDef",
     {
         "ephemerisData": str,
         "sourceS3Object": S3ObjectTypeDef,
     },
     total=False,
@@ -901,14 +1105,22 @@
     {
         "groundStationList": List[GroundStationDataTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+RangedSocketAddressTypeDef = TypedDict(
+    "RangedSocketAddressTypeDef",
+    {
+        "name": str,
+        "portRange": IntegerRangeTypeDef,
+    },
+)
+
 ListConfigsRequestListConfigsPaginateTypeDef = TypedDict(
     "ListConfigsRequestListConfigsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -1008,32 +1220,31 @@
     {
         "tleLine1": str,
         "tleLine2": str,
         "validTimeRange": TimeRangeTypeDef,
     },
 )
 
+RegisterAgentRequestRequestTypeDef = TypedDict(
+    "RegisterAgentRequestRequestTypeDef",
+    {
+        "agentDetails": AgentDetailsTypeDef,
+        "discoveryData": DiscoveryDataTypeDef,
+    },
+)
+
 ListContactsResponseTypeDef = TypedDict(
     "ListContactsResponseTypeDef",
     {
         "contactList": List[ContactDataTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-EndpointDetailsTypeDef = TypedDict(
-    "EndpointDetailsTypeDef",
-    {
-        "endpoint": DataflowEndpointTypeDef,
-        "securityDetails": SecurityDetailsTypeDef,
-    },
-    total=False,
-)
-
 EphemerisTypeDescriptionTypeDef = TypedDict(
     "EphemerisTypeDescriptionTypeDef",
     {
         "oem": EphemerisDescriptionTypeDef,
         "tle": EphemerisDescriptionTypeDef,
     },
     total=False,
@@ -1089,62 +1300,40 @@
 )
 
 class AntennaUplinkConfigTypeDef(
     _RequiredAntennaUplinkConfigTypeDef, _OptionalAntennaUplinkConfigTypeDef
 ):
     pass
 
-TLEEphemerisTypeDef = TypedDict(
-    "TLEEphemerisTypeDef",
-    {
-        "s3Object": S3ObjectTypeDef,
-        "tleData": Sequence[TLEDataTypeDef],
-    },
-    total=False,
-)
-
-ConfigDetailsTypeDef = TypedDict(
-    "ConfigDetailsTypeDef",
-    {
-        "antennaDemodDecodeDetails": AntennaDemodDecodeDetailsTypeDef,
-        "endpointDetails": EndpointDetailsTypeDef,
-        "s3RecordingDetails": S3RecordingDetailsTypeDef,
-    },
-    total=False,
-)
-
-_RequiredCreateDataflowEndpointGroupRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateDataflowEndpointGroupRequestRequestTypeDef",
+_RequiredRangedConnectionDetailsTypeDef = TypedDict(
+    "_RequiredRangedConnectionDetailsTypeDef",
     {
-        "endpointDetails": Sequence[EndpointDetailsTypeDef],
+        "socketAddress": RangedSocketAddressTypeDef,
     },
 )
-_OptionalCreateDataflowEndpointGroupRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateDataflowEndpointGroupRequestRequestTypeDef",
+_OptionalRangedConnectionDetailsTypeDef = TypedDict(
+    "_OptionalRangedConnectionDetailsTypeDef",
     {
-        "tags": Mapping[str, str],
+        "mtu": int,
     },
     total=False,
 )
 
-class CreateDataflowEndpointGroupRequestRequestTypeDef(
-    _RequiredCreateDataflowEndpointGroupRequestRequestTypeDef,
-    _OptionalCreateDataflowEndpointGroupRequestRequestTypeDef,
+class RangedConnectionDetailsTypeDef(
+    _RequiredRangedConnectionDetailsTypeDef, _OptionalRangedConnectionDetailsTypeDef
 ):
     pass
 
-GetDataflowEndpointGroupResponseTypeDef = TypedDict(
-    "GetDataflowEndpointGroupResponseTypeDef",
+TLEEphemerisTypeDef = TypedDict(
+    "TLEEphemerisTypeDef",
     {
-        "dataflowEndpointGroupArn": str,
-        "dataflowEndpointGroupId": str,
-        "endpointsDetails": List[EndpointDetailsTypeDef],
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "s3Object": S3ObjectTypeDef,
+        "tleData": Sequence[TLEDataTypeDef],
     },
+    total=False,
 )
 
 DescribeEphemerisResponseTypeDef = TypedDict(
     "DescribeEphemerisResponseTypeDef",
     {
         "creationTime": datetime,
         "enabled": bool,
@@ -1170,41 +1359,41 @@
         "s3RecordingConfig": S3RecordingConfigTypeDef,
         "trackingConfig": TrackingConfigTypeDef,
         "uplinkEchoConfig": UplinkEchoConfigTypeDef,
     },
     total=False,
 )
 
-EphemerisDataTypeDef = TypedDict(
-    "EphemerisDataTypeDef",
+_RequiredAwsGroundStationAgentEndpointTypeDef = TypedDict(
+    "_RequiredAwsGroundStationAgentEndpointTypeDef",
     {
-        "oem": OEMEphemerisTypeDef,
-        "tle": TLEEphemerisTypeDef,
+        "egressAddress": ConnectionDetailsTypeDef,
+        "ingressAddress": RangedConnectionDetailsTypeDef,
+        "name": str,
     },
-    total=False,
 )
-
-DestinationTypeDef = TypedDict(
-    "DestinationTypeDef",
+_OptionalAwsGroundStationAgentEndpointTypeDef = TypedDict(
+    "_OptionalAwsGroundStationAgentEndpointTypeDef",
     {
-        "configDetails": ConfigDetailsTypeDef,
-        "configId": str,
-        "configType": ConfigCapabilityTypeType,
-        "dataflowDestinationRegion": str,
+        "agentStatus": AgentStatusType,
+        "auditResults": AuditResultsType,
     },
     total=False,
 )
 
-SourceTypeDef = TypedDict(
-    "SourceTypeDef",
+class AwsGroundStationAgentEndpointTypeDef(
+    _RequiredAwsGroundStationAgentEndpointTypeDef, _OptionalAwsGroundStationAgentEndpointTypeDef
+):
+    pass
+
+EphemerisDataTypeDef = TypedDict(
+    "EphemerisDataTypeDef",
     {
-        "configDetails": ConfigDetailsTypeDef,
-        "configId": str,
-        "configType": ConfigCapabilityTypeType,
-        "dataflowSourceRegion": str,
+        "oem": OEMEphemerisTypeDef,
+        "tle": TLEEphemerisTypeDef,
     },
     total=False,
 )
 
 _RequiredCreateConfigRequestRequestTypeDef = TypedDict(
     "_RequiredCreateConfigRequestRequestTypeDef",
     {
@@ -1244,14 +1433,24 @@
         "configData": ConfigTypeDataTypeDef,
         "configId": str,
         "configType": ConfigCapabilityTypeType,
         "name": str,
     },
 )
 
+EndpointDetailsTypeDef = TypedDict(
+    "EndpointDetailsTypeDef",
+    {
+        "awsGroundStationAgentEndpoint": AwsGroundStationAgentEndpointTypeDef,
+        "endpoint": DataflowEndpointTypeDef,
+        "securityDetails": SecurityDetailsTypeDef,
+    },
+    total=False,
+)
+
 _RequiredCreateEphemerisRequestRequestTypeDef = TypedDict(
     "_RequiredCreateEphemerisRequestRequestTypeDef",
     {
         "name": str,
         "satelliteId": str,
     },
 )
@@ -1269,14 +1468,81 @@
 )
 
 class CreateEphemerisRequestRequestTypeDef(
     _RequiredCreateEphemerisRequestRequestTypeDef, _OptionalCreateEphemerisRequestRequestTypeDef
 ):
     pass
 
+ConfigDetailsTypeDef = TypedDict(
+    "ConfigDetailsTypeDef",
+    {
+        "antennaDemodDecodeDetails": AntennaDemodDecodeDetailsTypeDef,
+        "endpointDetails": EndpointDetailsTypeDef,
+        "s3RecordingDetails": S3RecordingDetailsTypeDef,
+    },
+    total=False,
+)
+
+_RequiredCreateDataflowEndpointGroupRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateDataflowEndpointGroupRequestRequestTypeDef",
+    {
+        "endpointDetails": Sequence[EndpointDetailsTypeDef],
+    },
+)
+_OptionalCreateDataflowEndpointGroupRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateDataflowEndpointGroupRequestRequestTypeDef",
+    {
+        "contactPostPassDurationSeconds": int,
+        "contactPrePassDurationSeconds": int,
+        "tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+class CreateDataflowEndpointGroupRequestRequestTypeDef(
+    _RequiredCreateDataflowEndpointGroupRequestRequestTypeDef,
+    _OptionalCreateDataflowEndpointGroupRequestRequestTypeDef,
+):
+    pass
+
+GetDataflowEndpointGroupResponseTypeDef = TypedDict(
+    "GetDataflowEndpointGroupResponseTypeDef",
+    {
+        "contactPostPassDurationSeconds": int,
+        "contactPrePassDurationSeconds": int,
+        "dataflowEndpointGroupArn": str,
+        "dataflowEndpointGroupId": str,
+        "endpointsDetails": List[EndpointDetailsTypeDef],
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DestinationTypeDef = TypedDict(
+    "DestinationTypeDef",
+    {
+        "configDetails": ConfigDetailsTypeDef,
+        "configId": str,
+        "configType": ConfigCapabilityTypeType,
+        "dataflowDestinationRegion": str,
+    },
+    total=False,
+)
+
+SourceTypeDef = TypedDict(
+    "SourceTypeDef",
+    {
+        "configDetails": ConfigDetailsTypeDef,
+        "configId": str,
+        "configType": ConfigCapabilityTypeType,
+        "dataflowSourceRegion": str,
+    },
+    total=False,
+)
+
 DataflowDetailTypeDef = TypedDict(
     "DataflowDetailTypeDef",
     {
         "destination": DestinationTypeDef,
         "errorMessage": str,
         "source": SourceTypeDef,
     },
```

### Comparing `mypy-boto3-groundstation-1.26.6/mypy_boto3_groundstation.egg-info/PKG-INFO` & `mypy-boto3-groundstation-1.26.61/mypy_boto3_groundstation.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-groundstation
-Version: 1.26.6
-Summary: Type annotations for boto3.GroundStation 1.26.6 service generated with mypy-boto3-builder 7.11.10
+Version: 1.26.61
+Summary: Type annotations for boto3.GroundStation 1.26.61 service generated with mypy-boto3-builder 7.12.3
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -18,14 +18,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -37,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-groundstation.svg?color=blue)](https://pypi.org/project/mypy-boto3-groundstation)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-groundstation?color=blue)](https://pypistats.org/packages/mypy-boto3-groundstation)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.GroundStation 1.26.6](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation)
+[boto3.GroundStation 1.26.61](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.10](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-groundstation docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/).
 
 See how it helps to find and fix potential bugs:
 
@@ -72,14 +73,15 @@
     - [Sublime Text](#sublime-text)
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
+    - [Waiters annotations](#waiters-annotations)
     - [Literals](#literals)
     - [Typed dictionaries](#typed-dictionaries)
   - [How it works](#how-it-works)
   - [What's new](#what's-new)
     - [Implemented features](#implemented-features)
     - [Latest changes](#latest-changes)
   - [Versioning](#versioning)
@@ -307,26 +309,50 @@
 )
 list_mission_profiles_paginator: ListMissionProfilesPaginator = client.get_paginator(
     "list_mission_profiles"
 )
 list_satellites_paginator: ListSatellitesPaginator = client.get_paginator("list_satellites")
 ```
 
+<a id="waiters-annotations"></a>
+
+### Waiters annotations
+
+`mypy_boto3_groundstation.waiter` module contains type annotations for all
+waiters.
+
+```python
+from boto3.session import Session
+
+from mypy_boto3_groundstation import GroundStationClient
+from mypy_boto3_groundstation.waiter import ContactScheduledWaiter
+
+client: GroundStationClient = Session().client("groundstation")
+
+# Explicit type annotations are optional here
+# Types should be correctly discovered by mypy and IDEs
+contact_scheduled_waiter: ContactScheduledWaiter = client.get_waiter("contact_scheduled")
+```
+
 <a id="literals"></a>
 
 ### Literals
 
 `mypy_boto3_groundstation.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
 ```python
 from mypy_boto3_groundstation.literals import (
+    AgentStatusType,
     AngleUnitsType,
+    AuditResultsType,
     BandwidthUnitsType,
+    ComponentTypeType,
     ConfigCapabilityTypeType,
+    ContactScheduledWaiterName,
     ContactStatusType,
     CriticalityType,
     EirpUnitsType,
     EndpointStatusType,
     EphemerisInvalidReasonType,
     EphemerisSourceType,
     EphemerisStatusType,
@@ -339,64 +365,72 @@
     ListMissionProfilesPaginatorName,
     ListSatellitesPaginatorName,
     PolarizationType,
     GroundStationServiceName,
     ServiceName,
     ResourceServiceName,
     PaginatorName,
+    WaiterName,
     RegionName,
 )
 
 
-def check_value(value: AngleUnitsType) -> bool:
+def check_value(value: AgentStatusType) -> bool:
     ...
 ```
 
 <a id="typed-dictionaries"></a>
 
 ### Typed dictionaries
 
 `mypy_boto3_groundstation.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_groundstation.type_defs import (
+    ComponentVersionTypeDef,
+    AggregateStatusTypeDef,
     AntennaDemodDecodeDetailsTypeDef,
     DecodeConfigTypeDef,
     DemodulationConfigTypeDef,
     EirpTypeDef,
     CancelContactRequestRequestTypeDef,
+    ComponentStatusDataTypeDef,
     S3RecordingDetailsTypeDef,
     ResponseMetadataTypeDef,
     ConfigListItemTypeDef,
     DataflowEndpointConfigTypeDef,
     S3RecordingConfigTypeDef,
     TrackingConfigTypeDef,
     UplinkEchoConfigTypeDef,
+    SocketAddressTypeDef,
     ElevationTypeDef,
-    CreateMissionProfileRequestRequestTypeDef,
+    KmsKeyTypeDef,
     DataflowEndpointListItemTypeDef,
-    SocketAddressTypeDef,
     DeleteConfigRequestRequestTypeDef,
     DeleteDataflowEndpointGroupRequestRequestTypeDef,
     DeleteEphemerisRequestRequestTypeDef,
     DeleteMissionProfileRequestRequestTypeDef,
+    WaiterConfigTypeDef,
     DescribeContactRequestRequestTypeDef,
     DescribeEphemerisRequestRequestTypeDef,
+    DiscoveryDataTypeDef,
     SecurityDetailsTypeDef,
     S3ObjectTypeDef,
     EphemerisMetaDataTypeDef,
     FrequencyBandwidthTypeDef,
     FrequencyTypeDef,
+    GetAgentConfigurationRequestRequestTypeDef,
     GetConfigRequestRequestTypeDef,
     GetDataflowEndpointGroupRequestRequestTypeDef,
     GetMinuteUsageRequestRequestTypeDef,
     GetMissionProfileRequestRequestTypeDef,
     GetSatelliteRequestRequestTypeDef,
     GroundStationDataTypeDef,
+    IntegerRangeTypeDef,
     PaginatorConfigTypeDef,
     ListConfigsRequestRequestTypeDef,
     ListContactsRequestRequestTypeDef,
     ListDataflowEndpointGroupsRequestRequestTypeDef,
     ListEphemeridesRequestRequestTypeDef,
     ListGroundStationsRequestRequestTypeDef,
     ListMissionProfilesRequestRequestTypeDef,
@@ -404,71 +438,83 @@
     ListSatellitesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ReserveContactRequestRequestTypeDef,
     TimeRangeTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateEphemerisRequestRequestTypeDef,
-    UpdateMissionProfileRequestRequestTypeDef,
+    AgentDetailsTypeDef,
+    UpdateAgentStatusRequestRequestTypeDef,
     ConfigIdResponseTypeDef,
     ContactIdResponseTypeDef,
     DataflowEndpointGroupIdResponseTypeDef,
     EphemerisIdResponseTypeDef,
+    GetAgentConfigurationResponseTypeDef,
     GetMinuteUsageResponseTypeDef,
-    GetMissionProfileResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     MissionProfileIdResponseTypeDef,
+    RegisterAgentResponseTypeDef,
+    UpdateAgentStatusResponseTypeDef,
     ListConfigsResponseTypeDef,
+    ConnectionDetailsTypeDef,
+    DataflowEndpointTypeDef,
     ContactDataTypeDef,
+    CreateMissionProfileRequestRequestTypeDef,
+    GetMissionProfileResponseTypeDef,
+    UpdateMissionProfileRequestRequestTypeDef,
     ListDataflowEndpointGroupsResponseTypeDef,
-    DataflowEndpointTypeDef,
+    DescribeContactRequestContactScheduledWaitTypeDef,
     EphemerisDescriptionTypeDef,
     EphemerisItemTypeDef,
     OEMEphemerisTypeDef,
     GetSatelliteResponseTypeDef,
     SatelliteListItemTypeDef,
     SpectrumConfigTypeDef,
     UplinkSpectrumConfigTypeDef,
     ListGroundStationsResponseTypeDef,
+    RangedSocketAddressTypeDef,
     ListConfigsRequestListConfigsPaginateTypeDef,
     ListContactsRequestListContactsPaginateTypeDef,
     ListDataflowEndpointGroupsRequestListDataflowEndpointGroupsPaginateTypeDef,
     ListEphemeridesRequestListEphemeridesPaginateTypeDef,
     ListGroundStationsRequestListGroundStationsPaginateTypeDef,
     ListMissionProfilesRequestListMissionProfilesPaginateTypeDef,
     ListSatellitesRequestListSatellitesPaginateTypeDef,
     ListMissionProfilesResponseTypeDef,
     TLEDataTypeDef,
+    RegisterAgentRequestRequestTypeDef,
     ListContactsResponseTypeDef,
-    EndpointDetailsTypeDef,
     EphemerisTypeDescriptionTypeDef,
     ListEphemeridesResponseTypeDef,
     ListSatellitesResponseTypeDef,
     AntennaDownlinkConfigTypeDef,
     AntennaDownlinkDemodDecodeConfigTypeDef,
     AntennaUplinkConfigTypeDef,
+    RangedConnectionDetailsTypeDef,
     TLEEphemerisTypeDef,
-    ConfigDetailsTypeDef,
-    CreateDataflowEndpointGroupRequestRequestTypeDef,
-    GetDataflowEndpointGroupResponseTypeDef,
     DescribeEphemerisResponseTypeDef,
     ConfigTypeDataTypeDef,
+    AwsGroundStationAgentEndpointTypeDef,
     EphemerisDataTypeDef,
-    DestinationTypeDef,
-    SourceTypeDef,
     CreateConfigRequestRequestTypeDef,
     GetConfigResponseTypeDef,
     UpdateConfigRequestRequestTypeDef,
+    EndpointDetailsTypeDef,
     CreateEphemerisRequestRequestTypeDef,
+    ConfigDetailsTypeDef,
+    CreateDataflowEndpointGroupRequestRequestTypeDef,
+    GetDataflowEndpointGroupResponseTypeDef,
+    DestinationTypeDef,
+    SourceTypeDef,
     DataflowDetailTypeDef,
     DescribeContactResponseTypeDef,
 )
 
 
-def get_structure() -> AntennaDemodDecodeDetailsTypeDef:
+def get_structure() -> ComponentVersionTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-groundstation-1.26.6/mypy_boto3_groundstation.egg-info/SOURCES.txt` & `mypy-boto3-groundstation-1.26.61/mypy_boto3_groundstation.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -10,13 +10,15 @@
 mypy_boto3_groundstation/literals.pyi
 mypy_boto3_groundstation/paginator.py
 mypy_boto3_groundstation/paginator.pyi
 mypy_boto3_groundstation/py.typed
 mypy_boto3_groundstation/type_defs.py
 mypy_boto3_groundstation/type_defs.pyi
 mypy_boto3_groundstation/version.py
+mypy_boto3_groundstation/waiter.py
+mypy_boto3_groundstation/waiter.pyi
 mypy_boto3_groundstation.egg-info/PKG-INFO
 mypy_boto3_groundstation.egg-info/SOURCES.txt
 mypy_boto3_groundstation.egg-info/dependency_links.txt
 mypy_boto3_groundstation.egg-info/not-zip-safe
 mypy_boto3_groundstation.egg-info/requires.txt
 mypy_boto3_groundstation.egg-info/top_level.txt
```

### Comparing `mypy-boto3-groundstation-1.26.6/setup.py` & `mypy-boto3-groundstation-1.26.61/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,45 +6,46 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
 
 
 setup(
     name="mypy-boto3-groundstation",
-    version="1.26.6",
+    version="1.26.61",
     packages=["mypy_boto3_groundstation"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.GroundStation 1.26.6 service generated with mypy-boto3-builder"
-        " 7.11.10"
+        "Type annotations for boto3.GroundStation 1.26.61 service generated with mypy-boto3-builder"
+        " 7.12.3"
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
     keywords="boto3 groundstation type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_groundstation": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_groundstation": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
```

