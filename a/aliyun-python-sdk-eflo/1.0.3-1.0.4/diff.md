# Comparing `tmp/aliyun-python-sdk-eflo-1.0.3.tar.gz` & `tmp/aliyun-python-sdk-eflo-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aliyun-python-sdk-eflo-1.0.3.tar", last modified: Thu Mar 30 09:58:24 2023, max compression
+gzip compressed data, was "dist/aliyun-python-sdk-eflo-1.0.4.tar", last modified: Thu Apr 13 08:25:20 2023, max compression
```

## Comparing `aliyun-python-sdk-eflo-1.0.3.tar` & `aliyun-python-sdk-eflo-1.0.4.tar`

### file list

```diff
@@ -1,44 +1,72 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 09:58:24.000000 aliyun-python-sdk-eflo-1.0.3/
--rw-r--r--   0 root         (0) root         (0)      575 2023-03-30 09:58:24.000000 aliyun-python-sdk-eflo-1.0.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)       40 2023-03-30 09:58:24.000000 aliyun-python-sdk-eflo-1.0.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1542 2023-03-30 09:58:24.000000 aliyun-python-sdk-eflo-1.0.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      529 2023-03-30 09:58:24.000000 aliyun-python-sdk-eflo-1.0.3/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 09:58:24.000000 aliyun-python-sdk-eflo-1.0.3/aliyun_python_sdk_eflo.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1542 2023-03-30 09:58:24.000000 aliyun-python-sdk-eflo-1.0.3/aliyun_python_sdk_eflo.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1792 2023-03-30 09:58:24.000000 aliyun-python-sdk-eflo-1.0.3/aliyun_python_sdk_eflo.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-30 09:58:24.000000 aliyun-python-sdk-eflo-1.0.3/aliyun_python_sdk_eflo.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-03-30 09:58:24.000000 aliyun-python-sdk-eflo-1.0.3/aliyun_python_sdk_eflo.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-03-30 09:58:24.000000 aliyun-python-sdk-eflo-1.0.3/aliyun_python_sdk_eflo.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 09:58:24.000000 aliyun-python-sdk-eflo-1.0.3/aliyunsdkeflo/
--rw-r--r--   0 root         (0) root         (0)       21 2023-03-30 09:58:24.000000 aliyun-python-sdk-eflo-1.0.3/aliyunsdkeflo/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 09:58:24.000000 aliyun-python-sdk-eflo-1.0.3/aliyunsdkeflo/request/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 09:58:24.000000 aliyun-python-sdk-eflo-1.0.3/aliyunsdkeflo/request/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 09:58:24.000000 aliyun-python-sdk-eflo-1.0.3/aliyunsdkeflo/request/v20220530/
--rw-r--r--   0 root         (0) root         (0)     2046 2023-03-30 09:58:24.000000 aliyun-python-sdk-eflo-1.0.3/aliyunsdkeflo/request/v20220530/AssignPrivateIpAddressRequest.py
--rw-r--r--   0 root         (0) root         (0)     2440 2023-03-30 09:58:24.000000 aliyun-python-sdk-eflo-1.0.3/aliyunsdkeflo/request/v20220530/CreateSubnetRequest.py
--rw-r--r--   0 root         (0) root         (0)     3618 2023-03-30 09:58:24.000000 aliyun-python-sdk-eflo-1.0.3/aliyunsdkeflo/request/v20220530/CreateVccRequest.py
--rw-r--r--   0 root         (0) root         (0)     1566 2023-03-30 09:58:24.000000 aliyun-python-sdk-eflo-1.0.3/aliyunsdkeflo/request/v20220530/CreateVpdGrantRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     3247 2023-03-30 09:58:24.000000 aliyun-python-sdk-eflo-1.0.3/aliyunsdkeflo/request/v20220530/CreateVpdRequest.py
--rw-r--r--   0 root         (0) root         (0)     1506 2023-03-30 09:58:24.000000 aliyun-python-sdk-eflo-1.0.3/aliyunsdkeflo/request/v20220530/DeleteSubnetRequest.py
--rw-r--r--   0 root         (0) root         (0)     1762 2023-03-30 09:58:24.000000 aliyun-python-sdk-eflo-1.0.3/aliyunsdkeflo/request/v20220530/DeleteVpdGrantRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     1156 2023-03-30 09:58:24.000000 aliyun-python-sdk-eflo-1.0.3/aliyunsdkeflo/request/v20220530/DeleteVpdRequest.py
--rw-r--r--   0 root         (0) root         (0)     1220 2023-03-30 09:58:24.000000 aliyun-python-sdk-eflo-1.0.3/aliyunsdkeflo/request/v20220530/DescribeSlrRequest.py
--rw-r--r--   0 root         (0) root         (0)     1622 2023-03-30 09:58:24.000000 aliyun-python-sdk-eflo-1.0.3/aliyunsdkeflo/request/v20220530/GetLniPrivateIpAddressRequest.py
--rw-r--r--   0 root         (0) root         (0)     1530 2023-03-30 09:58:24.000000 aliyun-python-sdk-eflo-1.0.3/aliyunsdkeflo/request/v20220530/GetSubnetRequest.py
--rw-r--r--   0 root         (0) root         (0)     1714 2023-03-30 09:58:24.000000 aliyun-python-sdk-eflo-1.0.3/aliyunsdkeflo/request/v20220530/GetVccRequest.py
--rw-r--r--   0 root         (0) root         (0)     1346 2023-03-30 09:58:24.000000 aliyun-python-sdk-eflo-1.0.3/aliyunsdkeflo/request/v20220530/GetVpdRequest.py
--rw-r--r--   0 root         (0) root         (0)     1224 2023-03-30 09:58:24.000000 aliyun-python-sdk-eflo-1.0.3/aliyunsdkeflo/request/v20220530/InitializeVccRequest.py
--rw-r--r--   0 root         (0) root         (0)     2134 2023-03-30 09:58:24.000000 aliyun-python-sdk-eflo-1.0.3/aliyunsdkeflo/request/v20220530/ListLniPrivateIpAddressRequest.py
--rw-r--r--   0 root         (0) root         (0)     2468 2023-03-30 09:58:24.000000 aliyun-python-sdk-eflo-1.0.3/aliyunsdkeflo/request/v20220530/ListNetworkInterfacesRequest.py
--rw-r--r--   0 root         (0) root         (0)     3216 2023-03-30 09:58:24.000000 aliyun-python-sdk-eflo-1.0.3/aliyunsdkeflo/request/v20220530/ListSubnetsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2712 2023-03-30 09:58:24.000000 aliyun-python-sdk-eflo-1.0.3/aliyunsdkeflo/request/v20220530/ListVccGrantRulesRequest.py
--rw-r--r--   0 root         (0) root         (0)     3556 2023-03-30 09:58:24.000000 aliyun-python-sdk-eflo-1.0.3/aliyunsdkeflo/request/v20220530/ListVccsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2712 2023-03-30 09:58:24.000000 aliyun-python-sdk-eflo-1.0.3/aliyunsdkeflo/request/v20220530/ListVpdGrantRulesRequest.py
--rw-r--r--   0 root         (0) root         (0)     3674 2023-03-30 09:58:24.000000 aliyun-python-sdk-eflo-1.0.3/aliyunsdkeflo/request/v20220530/ListVpdsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2030 2023-03-30 09:58:24.000000 aliyun-python-sdk-eflo-1.0.3/aliyunsdkeflo/request/v20220530/UnAssignPrivateIpAddressRequest.py
--rw-r--r--   0 root         (0) root         (0)     1892 2023-03-30 09:58:24.000000 aliyun-python-sdk-eflo-1.0.3/aliyunsdkeflo/request/v20220530/UpdateSubnetRequest.py
--rw-r--r--   0 root         (0) root         (0)     1686 2023-03-30 09:58:24.000000 aliyun-python-sdk-eflo-1.0.3/aliyunsdkeflo/request/v20220530/UpdateVccRequest.py
--rw-r--r--   0 root         (0) root         (0)     1524 2023-03-30 09:58:24.000000 aliyun-python-sdk-eflo-1.0.3/aliyunsdkeflo/request/v20220530/UpdateVpdRequest.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 09:58:24.000000 aliyun-python-sdk-eflo-1.0.3/aliyunsdkeflo/request/v20220530/__init__.py
--rw-r--r--   0 root         (0) root         (0)      102 2023-03-30 09:58:24.000000 aliyun-python-sdk-eflo-1.0.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2457 2023-03-30 09:58:24.000000 aliyun-python-sdk-eflo-1.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 08:25:20.000000 aliyun-python-sdk-eflo-1.0.4/
+-rw-r--r--   0 root         (0) root         (0)      575 2023-04-13 08:25:20.000000 aliyun-python-sdk-eflo-1.0.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       40 2023-04-13 08:25:20.000000 aliyun-python-sdk-eflo-1.0.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1542 2023-04-13 08:25:20.000000 aliyun-python-sdk-eflo-1.0.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      529 2023-04-13 08:25:20.000000 aliyun-python-sdk-eflo-1.0.4/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 08:25:20.000000 aliyun-python-sdk-eflo-1.0.4/aliyun_python_sdk_eflo.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1542 2023-04-13 08:25:20.000000 aliyun-python-sdk-eflo-1.0.4/aliyun_python_sdk_eflo.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3420 2023-04-13 08:25:20.000000 aliyun-python-sdk-eflo-1.0.4/aliyun_python_sdk_eflo.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 08:25:20.000000 aliyun-python-sdk-eflo-1.0.4/aliyun_python_sdk_eflo.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-04-13 08:25:20.000000 aliyun-python-sdk-eflo-1.0.4/aliyun_python_sdk_eflo.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-04-13 08:25:20.000000 aliyun-python-sdk-eflo-1.0.4/aliyun_python_sdk_eflo.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 08:25:20.000000 aliyun-python-sdk-eflo-1.0.4/aliyunsdkeflo/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-04-13 08:25:20.000000 aliyun-python-sdk-eflo-1.0.4/aliyunsdkeflo/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 08:25:20.000000 aliyun-python-sdk-eflo-1.0.4/aliyunsdkeflo/request/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 08:25:20.000000 aliyun-python-sdk-eflo-1.0.4/aliyunsdkeflo/request/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 08:25:20.000000 aliyun-python-sdk-eflo-1.0.4/aliyunsdkeflo/request/v20220530/
+-rw-r--r--   0 root         (0) root         (0)     2042 2023-04-13 08:25:20.000000 aliyun-python-sdk-eflo-1.0.4/aliyunsdkeflo/request/v20220530/AssignPrivateIpAddressRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2258 2023-04-13 08:25:20.000000 aliyun-python-sdk-eflo-1.0.4/aliyunsdkeflo/request/v20220530/CreateErAttachmentRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1558 2023-04-13 08:25:20.000000 aliyun-python-sdk-eflo-1.0.4/aliyunsdkeflo/request/v20220530/CreateErRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3600 2023-04-13 08:25:20.000000 aliyun-python-sdk-eflo-1.0.4/aliyunsdkeflo/request/v20220530/CreateErRouteMapRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2244 2023-04-13 08:25:20.000000 aliyun-python-sdk-eflo-1.0.4/aliyunsdkeflo/request/v20220530/CreateSubnetRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1566 2023-04-13 08:25:20.000000 aliyun-python-sdk-eflo-1.0.4/aliyunsdkeflo/request/v20220530/CreateVccGrantRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3804 2023-04-13 08:25:20.000000 aliyun-python-sdk-eflo-1.0.4/aliyunsdkeflo/request/v20220530/CreateVccRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1426 2023-04-13 08:25:20.000000 aliyun-python-sdk-eflo-1.0.4/aliyunsdkeflo/request/v20220530/CreateVccRouteEntryRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1566 2023-04-13 08:25:20.000000 aliyun-python-sdk-eflo-1.0.4/aliyunsdkeflo/request/v20220530/CreateVpdGrantRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2887 2023-04-13 08:25:20.000000 aliyun-python-sdk-eflo-1.0.4/aliyunsdkeflo/request/v20220530/CreateVpdRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1382 2023-04-13 08:25:20.000000 aliyun-python-sdk-eflo-1.0.4/aliyunsdkeflo/request/v20220530/DeleteErAttachmentRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1148 2023-04-13 08:25:20.000000 aliyun-python-sdk-eflo-1.0.4/aliyunsdkeflo/request/v20220530/DeleteErRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1454 2023-04-13 08:25:20.000000 aliyun-python-sdk-eflo-1.0.4/aliyunsdkeflo/request/v20220530/DeleteErRouteMapRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1506 2023-04-13 08:25:20.000000 aliyun-python-sdk-eflo-1.0.4/aliyunsdkeflo/request/v20220530/DeleteSubnetRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1554 2023-04-13 08:25:20.000000 aliyun-python-sdk-eflo-1.0.4/aliyunsdkeflo/request/v20220530/DeleteVccGrantRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1646 2023-04-13 08:25:20.000000 aliyun-python-sdk-eflo-1.0.4/aliyunsdkeflo/request/v20220530/DeleteVccRouteEntryRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1762 2023-04-13 08:25:20.000000 aliyun-python-sdk-eflo-1.0.4/aliyunsdkeflo/request/v20220530/DeleteVpdGrantRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1156 2023-04-13 08:25:20.000000 aliyun-python-sdk-eflo-1.0.4/aliyunsdkeflo/request/v20220530/DeleteVpdRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1220 2023-04-13 08:25:20.000000 aliyun-python-sdk-eflo-1.0.4/aliyunsdkeflo/request/v20220530/DescribeSlrRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1376 2023-04-13 08:25:20.000000 aliyun-python-sdk-eflo-1.0.4/aliyunsdkeflo/request/v20220530/GetErAttachmentRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1142 2023-04-13 08:25:20.000000 aliyun-python-sdk-eflo-1.0.4/aliyunsdkeflo/request/v20220530/GetErRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1376 2023-04-13 08:25:20.000000 aliyun-python-sdk-eflo-1.0.4/aliyunsdkeflo/request/v20220530/GetErRouteEntryRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1360 2023-04-13 08:25:20.000000 aliyun-python-sdk-eflo-1.0.4/aliyunsdkeflo/request/v20220530/GetErRouteMapRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1426 2023-04-13 08:25:20.000000 aliyun-python-sdk-eflo-1.0.4/aliyunsdkeflo/request/v20220530/GetLniPrivateIpAddressRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1432 2023-04-13 08:25:20.000000 aliyun-python-sdk-eflo-1.0.4/aliyunsdkeflo/request/v20220530/GetNetworkInterfaceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1334 2023-04-13 08:25:20.000000 aliyun-python-sdk-eflo-1.0.4/aliyunsdkeflo/request/v20220530/GetSubnetRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1756 2023-04-13 08:25:20.000000 aliyun-python-sdk-eflo-1.0.4/aliyunsdkeflo/request/v20220530/GetVccGrantRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1714 2023-04-13 08:25:20.000000 aliyun-python-sdk-eflo-1.0.4/aliyunsdkeflo/request/v20220530/GetVccRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1390 2023-04-13 08:25:20.000000 aliyun-python-sdk-eflo-1.0.4/aliyunsdkeflo/request/v20220530/GetVccRouteEntryRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1756 2023-04-13 08:25:20.000000 aliyun-python-sdk-eflo-1.0.4/aliyunsdkeflo/request/v20220530/GetVpdGrantRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1150 2023-04-13 08:25:20.000000 aliyun-python-sdk-eflo-1.0.4/aliyunsdkeflo/request/v20220530/GetVpdRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1390 2023-04-13 08:25:20.000000 aliyun-python-sdk-eflo-1.0.4/aliyunsdkeflo/request/v20220530/GetVpdRouteEntryRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1224 2023-04-13 08:25:20.000000 aliyun-python-sdk-eflo-1.0.4/aliyunsdkeflo/request/v20220530/InitializeVccRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3200 2023-04-13 08:25:20.000000 aliyun-python-sdk-eflo-1.0.4/aliyunsdkeflo/request/v20220530/ListErAttachmentsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2902 2023-04-13 08:25:20.000000 aliyun-python-sdk-eflo-1.0.4/aliyunsdkeflo/request/v20220530/ListErRouteEntriesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4168 2023-04-13 08:25:20.000000 aliyun-python-sdk-eflo-1.0.4/aliyunsdkeflo/request/v20220530/ListErRouteMapsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2470 2023-04-13 08:25:20.000000 aliyun-python-sdk-eflo-1.0.4/aliyunsdkeflo/request/v20220530/ListErsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2134 2023-04-13 08:25:20.000000 aliyun-python-sdk-eflo-1.0.4/aliyunsdkeflo/request/v20220530/ListLniPrivateIpAddressRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2468 2023-04-13 08:25:20.000000 aliyun-python-sdk-eflo-1.0.4/aliyunsdkeflo/request/v20220530/ListNetworkInterfacesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3216 2023-04-13 08:25:20.000000 aliyun-python-sdk-eflo-1.0.4/aliyunsdkeflo/request/v20220530/ListSubnetsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2712 2023-04-13 08:25:20.000000 aliyun-python-sdk-eflo-1.0.4/aliyunsdkeflo/request/v20220530/ListVccGrantRulesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2940 2023-04-13 08:25:20.000000 aliyun-python-sdk-eflo-1.0.4/aliyunsdkeflo/request/v20220530/ListVccRouteEntriesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3556 2023-04-13 08:25:20.000000 aliyun-python-sdk-eflo-1.0.4/aliyunsdkeflo/request/v20220530/ListVccsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2712 2023-04-13 08:25:20.000000 aliyun-python-sdk-eflo-1.0.4/aliyunsdkeflo/request/v20220530/ListVpdGrantRulesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2940 2023-04-13 08:25:20.000000 aliyun-python-sdk-eflo-1.0.4/aliyunsdkeflo/request/v20220530/ListVpdRouteEntriesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3478 2023-04-13 08:25:20.000000 aliyun-python-sdk-eflo-1.0.4/aliyunsdkeflo/request/v20220530/ListVpdsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1834 2023-04-13 08:25:20.000000 aliyun-python-sdk-eflo-1.0.4/aliyunsdkeflo/request/v20220530/UnAssignPrivateIpAddressRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1608 2023-04-13 08:25:20.000000 aliyun-python-sdk-eflo-1.0.4/aliyunsdkeflo/request/v20220530/UpdateErAttachmentRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1510 2023-04-13 08:25:20.000000 aliyun-python-sdk-eflo-1.0.4/aliyunsdkeflo/request/v20220530/UpdateErRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1562 2023-04-13 08:25:20.000000 aliyun-python-sdk-eflo-1.0.4/aliyunsdkeflo/request/v20220530/UpdateErRouteMapRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1696 2023-04-13 08:25:20.000000 aliyun-python-sdk-eflo-1.0.4/aliyunsdkeflo/request/v20220530/UpdateSubnetRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1686 2023-04-13 08:25:20.000000 aliyun-python-sdk-eflo-1.0.4/aliyunsdkeflo/request/v20220530/UpdateVccRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1328 2023-04-13 08:25:20.000000 aliyun-python-sdk-eflo-1.0.4/aliyunsdkeflo/request/v20220530/UpdateVpdRequest.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 08:25:20.000000 aliyun-python-sdk-eflo-1.0.4/aliyunsdkeflo/request/v20220530/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      102 2023-04-13 08:25:20.000000 aliyun-python-sdk-eflo-1.0.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2457 2023-04-13 08:25:20.000000 aliyun-python-sdk-eflo-1.0.4/setup.py
```

### Comparing `aliyun-python-sdk-eflo-1.0.3/LICENSE` & `aliyun-python-sdk-eflo-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.3/PKG-INFO` & `aliyun-python-sdk-eflo-1.0.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-eflo
-Version: 1.0.3
+Version: 1.0.4
 Summary: The eflo module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-eflo
```

### Comparing `aliyun-python-sdk-eflo-1.0.3/README.rst` & `aliyun-python-sdk-eflo-1.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.3/aliyun_python_sdk_eflo.egg-info/PKG-INFO` & `aliyun-python-sdk-eflo-1.0.4/aliyun_python_sdk_eflo.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-eflo
-Version: 1.0.3
+Version: 1.0.4
 Summary: The eflo module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-eflo
```

### Comparing `aliyun-python-sdk-eflo-1.0.3/aliyun_python_sdk_eflo.egg-info/SOURCES.txt` & `aliyun-python-sdk-eflo-1.0.4/aliyun_python_sdk_eflo.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -7,32 +7,60 @@
 aliyun_python_sdk_eflo.egg-info/SOURCES.txt
 aliyun_python_sdk_eflo.egg-info/dependency_links.txt
 aliyun_python_sdk_eflo.egg-info/requires.txt
 aliyun_python_sdk_eflo.egg-info/top_level.txt
 aliyunsdkeflo/__init__.py
 aliyunsdkeflo/request/__init__.py
 aliyunsdkeflo/request/v20220530/AssignPrivateIpAddressRequest.py
+aliyunsdkeflo/request/v20220530/CreateErAttachmentRequest.py
+aliyunsdkeflo/request/v20220530/CreateErRequest.py
+aliyunsdkeflo/request/v20220530/CreateErRouteMapRequest.py
 aliyunsdkeflo/request/v20220530/CreateSubnetRequest.py
+aliyunsdkeflo/request/v20220530/CreateVccGrantRuleRequest.py
 aliyunsdkeflo/request/v20220530/CreateVccRequest.py
+aliyunsdkeflo/request/v20220530/CreateVccRouteEntryRequest.py
 aliyunsdkeflo/request/v20220530/CreateVpdGrantRuleRequest.py
 aliyunsdkeflo/request/v20220530/CreateVpdRequest.py
+aliyunsdkeflo/request/v20220530/DeleteErAttachmentRequest.py
+aliyunsdkeflo/request/v20220530/DeleteErRequest.py
+aliyunsdkeflo/request/v20220530/DeleteErRouteMapRequest.py
 aliyunsdkeflo/request/v20220530/DeleteSubnetRequest.py
+aliyunsdkeflo/request/v20220530/DeleteVccGrantRuleRequest.py
+aliyunsdkeflo/request/v20220530/DeleteVccRouteEntryRequest.py
 aliyunsdkeflo/request/v20220530/DeleteVpdGrantRuleRequest.py
 aliyunsdkeflo/request/v20220530/DeleteVpdRequest.py
 aliyunsdkeflo/request/v20220530/DescribeSlrRequest.py
+aliyunsdkeflo/request/v20220530/GetErAttachmentRequest.py
+aliyunsdkeflo/request/v20220530/GetErRequest.py
+aliyunsdkeflo/request/v20220530/GetErRouteEntryRequest.py
+aliyunsdkeflo/request/v20220530/GetErRouteMapRequest.py
 aliyunsdkeflo/request/v20220530/GetLniPrivateIpAddressRequest.py
+aliyunsdkeflo/request/v20220530/GetNetworkInterfaceRequest.py
 aliyunsdkeflo/request/v20220530/GetSubnetRequest.py
+aliyunsdkeflo/request/v20220530/GetVccGrantRuleRequest.py
 aliyunsdkeflo/request/v20220530/GetVccRequest.py
+aliyunsdkeflo/request/v20220530/GetVccRouteEntryRequest.py
+aliyunsdkeflo/request/v20220530/GetVpdGrantRuleRequest.py
 aliyunsdkeflo/request/v20220530/GetVpdRequest.py
+aliyunsdkeflo/request/v20220530/GetVpdRouteEntryRequest.py
 aliyunsdkeflo/request/v20220530/InitializeVccRequest.py
+aliyunsdkeflo/request/v20220530/ListErAttachmentsRequest.py
+aliyunsdkeflo/request/v20220530/ListErRouteEntriesRequest.py
+aliyunsdkeflo/request/v20220530/ListErRouteMapsRequest.py
+aliyunsdkeflo/request/v20220530/ListErsRequest.py
 aliyunsdkeflo/request/v20220530/ListLniPrivateIpAddressRequest.py
 aliyunsdkeflo/request/v20220530/ListNetworkInterfacesRequest.py
 aliyunsdkeflo/request/v20220530/ListSubnetsRequest.py
 aliyunsdkeflo/request/v20220530/ListVccGrantRulesRequest.py
+aliyunsdkeflo/request/v20220530/ListVccRouteEntriesRequest.py
 aliyunsdkeflo/request/v20220530/ListVccsRequest.py
 aliyunsdkeflo/request/v20220530/ListVpdGrantRulesRequest.py
+aliyunsdkeflo/request/v20220530/ListVpdRouteEntriesRequest.py
 aliyunsdkeflo/request/v20220530/ListVpdsRequest.py
 aliyunsdkeflo/request/v20220530/UnAssignPrivateIpAddressRequest.py
+aliyunsdkeflo/request/v20220530/UpdateErAttachmentRequest.py
+aliyunsdkeflo/request/v20220530/UpdateErRequest.py
+aliyunsdkeflo/request/v20220530/UpdateErRouteMapRequest.py
 aliyunsdkeflo/request/v20220530/UpdateSubnetRequest.py
 aliyunsdkeflo/request/v20220530/UpdateVccRequest.py
 aliyunsdkeflo/request/v20220530/UpdateVpdRequest.py
 aliyunsdkeflo/request/v20220530/__init__.py
```

### Comparing `aliyun-python-sdk-eflo-1.0.3/aliyunsdkeflo/request/v20220530/AssignPrivateIpAddressRequest.py` & `aliyun-python-sdk-eflo-1.0.4/aliyunsdkeflo/request/v20220530/AssignPrivateIpAddressRequest.py`

 * *Files 14% similar despite different names*

```diff
@@ -26,19 +26,19 @@
 		self.set_method('POST')
 
 	def get_SubnetId(self): # String
 		return self.get_body_params().get('SubnetId')
 
 	def set_SubnetId(self, SubnetId):  # String
 		self.add_body_params('SubnetId', SubnetId)
-	def get_ClientToken(self): # String
-		return self.get_body_params().get('ClientToken')
+	def get_SkipConfig(self): # Boolean
+		return self.get_body_params().get('SkipConfig')
 
-	def set_ClientToken(self, ClientToken):  # String
-		self.add_body_params('ClientToken', ClientToken)
+	def set_SkipConfig(self, SkipConfig):  # Boolean
+		self.add_body_params('SkipConfig', SkipConfig)
 	def get_AssignMac(self): # Boolean
 		return self.get_body_params().get('AssignMac')
 
 	def set_AssignMac(self, AssignMac):  # Boolean
 		self.add_body_params('AssignMac', AssignMac)
 	def get_PrivateIpAddress(self): # String
 		return self.get_body_params().get('PrivateIpAddress')
```

### Comparing `aliyun-python-sdk-eflo-1.0.3/aliyunsdkeflo/request/v20220530/CreateSubnetRequest.py` & `aliyun-python-sdk-eflo-1.0.4/aliyunsdkeflo/request/v20220530/CreateSubnetRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,19 +21,14 @@
 
 class CreateSubnetRequest(RpcRequest):
 
 	def __init__(self):
 		RpcRequest.__init__(self, 'eflo', '2022-05-30', 'CreateSubnet','eflo')
 		self.set_method('POST')
 
-	def get_ClientToken(self): # String
-		return self.get_body_params().get('ClientToken')
-
-	def set_ClientToken(self, ClientToken):  # String
-		self.add_body_params('ClientToken', ClientToken)
 	def get_Type(self): # String
 		return self.get_body_params().get('Type')
 
 	def set_Type(self, Type):  # String
 		self.add_body_params('Type', Type)
 	def get_Cidr(self): # String
 		return self.get_body_params().get('Cidr')
```

### Comparing `aliyun-python-sdk-eflo-1.0.3/aliyunsdkeflo/request/v20220530/CreateVccRequest.py` & `aliyun-python-sdk-eflo-1.0.4/aliyunsdkeflo/request/v20220530/CreateVccRequest.py`

 * *Files 3% similar despite different names*

```diff
@@ -70,14 +70,19 @@
 	def set_VccId(self, VccId):  # String
 		self.add_body_params('VccId', VccId)
 	def get_ConnectionType(self): # String
 		return self.get_body_params().get('ConnectionType')
 
 	def set_ConnectionType(self, ConnectionType):  # String
 		self.add_body_params('ConnectionType', ConnectionType)
+	def get_Bandwidth(self): # Integer
+		return self.get_body_params().get('Bandwidth')
+
+	def set_Bandwidth(self, Bandwidth):  # Integer
+		self.add_body_params('Bandwidth', Bandwidth)
 	def get_VSwitchId(self): # String
 		return self.get_body_params().get('VSwitchId')
 
 	def set_VSwitchId(self, VSwitchId):  # String
 		self.add_body_params('VSwitchId', VSwitchId)
 	def get_VpdId(self): # String
 		return self.get_body_params().get('VpdId')
```

### Comparing `aliyun-python-sdk-eflo-1.0.3/aliyunsdkeflo/request/v20220530/CreateVpdGrantRuleRequest.py` & `aliyun-python-sdk-eflo-1.0.4/aliyunsdkeflo/request/v20220530/CreateVpdGrantRuleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.3/aliyunsdkeflo/request/v20220530/CreateVpdRequest.py` & `aliyun-python-sdk-eflo-1.0.4/aliyunsdkeflo/request/v20220530/CreateVpdRequest.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,19 +21,14 @@
 
 class CreateVpdRequest(RpcRequest):
 
 	def __init__(self):
 		RpcRequest.__init__(self, 'eflo', '2022-05-30', 'CreateVpd','eflo')
 		self.set_method('POST')
 
-	def get_ClientToken(self): # String
-		return self.get_body_params().get('ClientToken')
-
-	def set_ClientToken(self, ClientToken):  # String
-		self.add_body_params('ClientToken', ClientToken)
 	def get_VpdName(self): # String
 		return self.get_body_params().get('VpdName')
 
 	def set_VpdName(self, VpdName):  # String
 		self.add_body_params('VpdName', VpdName)
 	def get_ResourceGroupId(self): # String
 		return self.get_body_params().get('ResourceGroupId')
@@ -48,16 +43,14 @@
 	def get_Subnetss(self): # RepeatList
 		return self.get_body_params().get('Subnets')
 
 	def set_Subnetss(self, Subnets):  # RepeatList
 		for depth1 in range(len(Subnets)):
 			if Subnets[depth1].get('RegionId') is not None:
 				self.add_body_params('Subnets.' + str(depth1 + 1) + '.RegionId', Subnets[depth1].get('RegionId'))
-			if Subnets[depth1].get('ClientToken') is not None:
-				self.add_body_params('Subnets.' + str(depth1 + 1) + '.ClientToken', Subnets[depth1].get('ClientToken'))
 			if Subnets[depth1].get('ZoneId') is not None:
 				self.add_body_params('Subnets.' + str(depth1 + 1) + '.ZoneId', Subnets[depth1].get('ZoneId'))
 			if Subnets[depth1].get('Cidr') is not None:
 				self.add_body_params('Subnets.' + str(depth1 + 1) + '.Cidr', Subnets[depth1].get('Cidr'))
 			if Subnets[depth1].get('SubnetName') is not None:
 				self.add_body_params('Subnets.' + str(depth1 + 1) + '.SubnetName', Subnets[depth1].get('SubnetName'))
 			if Subnets[depth1].get('Type') is not None:
```

### Comparing `aliyun-python-sdk-eflo-1.0.3/aliyunsdkeflo/request/v20220530/DeleteSubnetRequest.py` & `aliyun-python-sdk-eflo-1.0.4/aliyunsdkeflo/request/v20220530/DeleteSubnetRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.3/aliyunsdkeflo/request/v20220530/DeleteVpdGrantRuleRequest.py` & `aliyun-python-sdk-eflo-1.0.4/aliyunsdkeflo/request/v20220530/DeleteVpdGrantRuleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.3/aliyunsdkeflo/request/v20220530/DeleteVpdRequest.py` & `aliyun-python-sdk-eflo-1.0.4/aliyunsdkeflo/request/v20220530/DeleteVpdRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.3/aliyunsdkeflo/request/v20220530/DescribeSlrRequest.py` & `aliyun-python-sdk-eflo-1.0.4/aliyunsdkeflo/request/v20220530/DescribeSlrRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.3/aliyunsdkeflo/request/v20220530/GetLniPrivateIpAddressRequest.py` & `aliyun-python-sdk-eflo-1.0.4/aliyunsdkeflo/request/v20220530/GetNetworkInterfaceRequest.py`

 * *Files 17% similar despite different names*

```diff
@@ -15,28 +15,23 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 
-class GetLniPrivateIpAddressRequest(RpcRequest):
+class GetNetworkInterfaceRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'eflo', '2022-05-30', 'GetLniPrivateIpAddress','eflo')
+		RpcRequest.__init__(self, 'eflo', '2022-05-30', 'GetNetworkInterface','eflo')
 		self.set_method('POST')
 
-	def get_ClientToken(self): # String
-		return self.get_body_params().get('ClientToken')
+	def get_SubnetId(self): # String
+		return self.get_body_params().get('SubnetId')
 
-	def set_ClientToken(self, ClientToken):  # String
-		self.add_body_params('ClientToken', ClientToken)
-	def get_IpName(self): # String
-		return self.get_body_params().get('IpName')
-
-	def set_IpName(self, IpName):  # String
-		self.add_body_params('IpName', IpName)
+	def set_SubnetId(self, SubnetId):  # String
+		self.add_body_params('SubnetId', SubnetId)
 	def get_NetworkInterfaceId(self): # String
 		return self.get_body_params().get('NetworkInterfaceId')
 
 	def set_NetworkInterfaceId(self, NetworkInterfaceId):  # String
 		self.add_body_params('NetworkInterfaceId', NetworkInterfaceId)
```

### Comparing `aliyun-python-sdk-eflo-1.0.3/aliyunsdkeflo/request/v20220530/GetSubnetRequest.py` & `aliyun-python-sdk-eflo-1.0.4/aliyunsdkeflo/request/v20220530/GetSubnetRequest.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,17 +26,12 @@
 		self.set_method('POST')
 
 	def get_SubnetId(self): # String
 		return self.get_body_params().get('SubnetId')
 
 	def set_SubnetId(self, SubnetId):  # String
 		self.add_body_params('SubnetId', SubnetId)
-	def get_ClientToken(self): # String
-		return self.get_body_params().get('ClientToken')
-
-	def set_ClientToken(self, ClientToken):  # String
-		self.add_body_params('ClientToken', ClientToken)
 	def get_VpdId(self): # String
 		return self.get_body_params().get('VpdId')
 
 	def set_VpdId(self, VpdId):  # String
 		self.add_body_params('VpdId', VpdId)
```

### Comparing `aliyun-python-sdk-eflo-1.0.3/aliyunsdkeflo/request/v20220530/GetVccRequest.py` & `aliyun-python-sdk-eflo-1.0.4/aliyunsdkeflo/request/v20220530/GetVccRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.3/aliyunsdkeflo/request/v20220530/GetVpdRequest.py` & `aliyun-python-sdk-eflo-1.0.4/aliyunsdkeflo/request/v20220530/GetVpdRequest.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,17 +21,12 @@
 
 class GetVpdRequest(RpcRequest):
 
 	def __init__(self):
 		RpcRequest.__init__(self, 'eflo', '2022-05-30', 'GetVpd','eflo')
 		self.set_method('POST')
 
-	def get_ClientToken(self): # String
-		return self.get_body_params().get('ClientToken')
-
-	def set_ClientToken(self, ClientToken):  # String
-		self.add_body_params('ClientToken', ClientToken)
 	def get_VpdId(self): # String
 		return self.get_body_params().get('VpdId')
 
 	def set_VpdId(self, VpdId):  # String
 		self.add_body_params('VpdId', VpdId)
```

### Comparing `aliyun-python-sdk-eflo-1.0.3/aliyunsdkeflo/request/v20220530/InitializeVccRequest.py` & `aliyun-python-sdk-eflo-1.0.4/aliyunsdkeflo/request/v20220530/InitializeVccRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.3/aliyunsdkeflo/request/v20220530/ListLniPrivateIpAddressRequest.py` & `aliyun-python-sdk-eflo-1.0.4/aliyunsdkeflo/request/v20220530/ListLniPrivateIpAddressRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.3/aliyunsdkeflo/request/v20220530/ListNetworkInterfacesRequest.py` & `aliyun-python-sdk-eflo-1.0.4/aliyunsdkeflo/request/v20220530/ListNetworkInterfacesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.3/aliyunsdkeflo/request/v20220530/ListSubnetsRequest.py` & `aliyun-python-sdk-eflo-1.0.4/aliyunsdkeflo/request/v20220530/ListSubnetsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.3/aliyunsdkeflo/request/v20220530/ListVccGrantRulesRequest.py` & `aliyun-python-sdk-eflo-1.0.4/aliyunsdkeflo/request/v20220530/ListVccGrantRulesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.3/aliyunsdkeflo/request/v20220530/ListVccsRequest.py` & `aliyun-python-sdk-eflo-1.0.4/aliyunsdkeflo/request/v20220530/ListVccsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.3/aliyunsdkeflo/request/v20220530/ListVpdGrantRulesRequest.py` & `aliyun-python-sdk-eflo-1.0.4/aliyunsdkeflo/request/v20220530/ListVpdGrantRulesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.3/aliyunsdkeflo/request/v20220530/ListVpdsRequest.py` & `aliyun-python-sdk-eflo-1.0.4/aliyunsdkeflo/request/v20220530/ListVpdsRequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,19 +21,14 @@
 
 class ListVpdsRequest(RpcRequest):
 
 	def __init__(self):
 		RpcRequest.__init__(self, 'eflo', '2022-05-30', 'ListVpds','eflo')
 		self.set_method('POST')
 
-	def get_ClientToken(self): # String
-		return self.get_body_params().get('ClientToken')
-
-	def set_ClientToken(self, ClientToken):  # String
-		self.add_body_params('ClientToken', ClientToken)
 	def get_VpdName(self): # String
 		return self.get_body_params().get('VpdName')
 
 	def set_VpdName(self, VpdName):  # String
 		self.add_body_params('VpdName', VpdName)
 	def get_PageNumber(self): # Integer
 		return self.get_body_params().get('PageNumber')
```

### Comparing `aliyun-python-sdk-eflo-1.0.3/aliyunsdkeflo/request/v20220530/UnAssignPrivateIpAddressRequest.py` & `aliyun-python-sdk-eflo-1.0.4/aliyunsdkeflo/request/v20220530/UnAssignPrivateIpAddressRequest.py`

 * *Files 18% similar despite different names*

```diff
@@ -26,19 +26,14 @@
 		self.set_method('POST')
 
 	def get_SubnetId(self): # String
 		return self.get_body_params().get('SubnetId')
 
 	def set_SubnetId(self, SubnetId):  # String
 		self.add_body_params('SubnetId', SubnetId)
-	def get_ClientToken(self): # String
-		return self.get_body_params().get('ClientToken')
-
-	def set_ClientToken(self, ClientToken):  # String
-		self.add_body_params('ClientToken', ClientToken)
 	def get_PrivateIpAddress(self): # String
 		return self.get_body_params().get('PrivateIpAddress')
 
 	def set_PrivateIpAddress(self, PrivateIpAddress):  # String
 		self.add_body_params('PrivateIpAddress', PrivateIpAddress)
 	def get_IpName(self): # String
 		return self.get_body_params().get('IpName')
```

### Comparing `aliyun-python-sdk-eflo-1.0.3/aliyunsdkeflo/request/v20220530/UpdateSubnetRequest.py` & `aliyun-python-sdk-eflo-1.0.4/aliyunsdkeflo/request/v20220530/UpdateSubnetRequest.py`

 * *Files 13% similar despite different names*

```diff
@@ -26,19 +26,14 @@
 		self.set_method('POST')
 
 	def get_SubnetId(self): # String
 		return self.get_body_params().get('SubnetId')
 
 	def set_SubnetId(self, SubnetId):  # String
 		self.add_body_params('SubnetId', SubnetId)
-	def get_Description(self): # String
-		return self.get_body_params().get('Description')
-
-	def set_Description(self, Description):  # String
-		self.add_body_params('Description', Description)
 	def get_VpdId(self): # String
 		return self.get_body_params().get('VpdId')
 
 	def set_VpdId(self, VpdId):  # String
 		self.add_body_params('VpdId', VpdId)
 	def get_ZoneId(self): # String
 		return self.get_body_params().get('ZoneId')
```

### Comparing `aliyun-python-sdk-eflo-1.0.3/aliyunsdkeflo/request/v20220530/UpdateVccRequest.py` & `aliyun-python-sdk-eflo-1.0.4/aliyunsdkeflo/request/v20220530/UpdateVccRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eflo-1.0.3/aliyunsdkeflo/request/v20220530/UpdateVpdRequest.py` & `aliyun-python-sdk-eflo-1.0.4/aliyunsdkeflo/request/v20220530/UpdateVpdRequest.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,19 +21,14 @@
 
 class UpdateVpdRequest(RpcRequest):
 
 	def __init__(self):
 		RpcRequest.__init__(self, 'eflo', '2022-05-30', 'UpdateVpd','eflo')
 		self.set_method('POST')
 
-	def get_ClientToken(self): # String
-		return self.get_body_params().get('ClientToken')
-
-	def set_ClientToken(self, ClientToken):  # String
-		self.add_body_params('ClientToken', ClientToken)
 	def get_VpdName(self): # String
 		return self.get_body_params().get('VpdName')
 
 	def set_VpdName(self, VpdName):  # String
 		self.add_body_params('VpdName', VpdName)
 	def get_VpdId(self): # String
 		return self.get_body_params().get('VpdId')
```

### Comparing `aliyun-python-sdk-eflo-1.0.3/setup.py` & `aliyun-python-sdk-eflo-1.0.4/setup.py`

 * *Files identical despite different names*

